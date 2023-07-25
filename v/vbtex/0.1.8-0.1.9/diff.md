# Comparing `tmp/vbtex-0.1.8.tar.gz` & `tmp/vbtex-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vbtex-0.1.8.tar", max compression
+gzip compressed data, was "vbtex-0.1.9.tar", max compression
```

## Comparing `vbtex-0.1.8.tar` & `vbtex-0.1.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2023-06-21 16:42:53.861422 vbtex-0.1.8/README.md
--rw-r--r--   0        0        0      370 2023-07-25 05:00:58.594573 vbtex-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-07-20 05:43:48.477861 vbtex-0.1.8/vbtex/.DS_Store
--rw-r--r--   0        0        0        0 2023-06-21 16:42:53.861342 vbtex-0.1.8/vbtex/__init__.py
--rw-r--r--   0        0        0       47 2023-06-21 16:47:15.593234 vbtex-0.1.8/vbtex/__main__.py
--rw-r--r--   0        0        0     1236 2023-07-19 10:33:59.070206 vbtex-0.1.8/vbtex/choice_option.py
--rw-r--r--   0        0        0     2893 2023-07-25 05:00:45.304273 vbtex-0.1.8/vbtex/framed.py
--rw-r--r--   0        0        0      299 2023-07-19 12:20:17.191249 vbtex-0.1.8/vbtex/main.py
--rw-r--r--   0        0        0     1191 2023-07-19 12:29:13.505367 vbtex-0.1.8/vbtex/padded.py
--rw-r--r--   0        0        0      340 1970-01-01 00:00:00.000000 vbtex-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-21 16:42:53.861422 vbtex-0.1.9/README.md
+-rw-r--r--   0        0        0      370 2023-07-25 05:06:54.963952 vbtex-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-07-20 05:43:48.477861 vbtex-0.1.9/vbtex/.DS_Store
+-rw-r--r--   0        0        0        0 2023-06-21 16:42:53.861342 vbtex-0.1.9/vbtex/__init__.py
+-rw-r--r--   0        0        0       47 2023-06-21 16:47:15.593234 vbtex-0.1.9/vbtex/__main__.py
+-rw-r--r--   0        0        0     1236 2023-07-19 10:33:59.070206 vbtex-0.1.9/vbtex/choice_option.py
+-rw-r--r--   0        0        0     3063 2023-07-25 05:06:47.437205 vbtex-0.1.9/vbtex/framed.py
+-rw-r--r--   0        0        0      299 2023-07-19 12:20:17.191249 vbtex-0.1.9/vbtex/main.py
+-rw-r--r--   0        0        0     1191 2023-07-19 12:29:13.505367 vbtex-0.1.9/vbtex/padded.py
+-rw-r--r--   0        0        0      340 1970-01-01 00:00:00.000000 vbtex-0.1.9/PKG-INFO
```

### Comparing `vbtex-0.1.8/vbtex/.DS_Store` & `vbtex-0.1.9/vbtex/.DS_Store`

 * *Files identical despite different names*

### Comparing `vbtex-0.1.8/vbtex/choice_option.py` & `vbtex-0.1.9/vbtex/choice_option.py`

 * *Files identical despite different names*

### Comparing `vbtex-0.1.8/vbtex/framed.py` & `vbtex-0.1.9/vbtex/framed.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,23 @@
     prompt='Format',
     type=click.Choice(['SQUARE + VRECT', 'SQUARE', 'VRECT', 'HRECT']),
     cls=ChoiceOption,
     default=1,
     show_default=True,
     help="Format of the output"
 )
-def framed(input_text, size):
+@click.option(
+    '-b',
+    '--background',
+    type=click.Path(),
+    default=f'$BG/Wheat.jpg',
+    show_default=True,
+    help="Background file for png"
+)
+def framed(input_text, size, background):
    
     def get_file_name_png(size):
         now = datetime.now()
         file_name = now.strftime("%Y_%m_%d@%H:%M:%S")
         return f'{file_name}_{size.lower()}.png'
 
     if input_text is None:
```

### Comparing `vbtex-0.1.8/vbtex/padded.py` & `vbtex-0.1.9/vbtex/padded.py`

 * *Files identical despite different names*

