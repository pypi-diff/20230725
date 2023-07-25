# Comparing `tmp/pydbtools-5.5.6.tar.gz` & `tmp/pydbtools-5.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydbtools-5.5.6.tar", max compression
+gzip compressed data, was "pydbtools-5.5.7.tar", max compression
```

## Comparing `pydbtools-5.5.6.tar` & `pydbtools-5.5.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     9632 2023-05-05 15:48:50.967806 pydbtools-5.5.6/README.md
--rw-r--r--   0        0        0      855 2023-05-05 15:48:50.971806 pydbtools-5.5.6/pydbtools/__init__.py
--rw-r--r--   0        0        0     1130 2023-05-05 15:48:50.971806 pydbtools-5.5.6/pydbtools/_sql_render.py
--rw-r--r--   0        0        0    23104 2023-05-05 15:48:50.971806 pydbtools-5.5.6/pydbtools/_wrangler.py
--rw-r--r--   0        0        0     6391 2023-05-05 15:48:50.971806 pydbtools-5.5.6/pydbtools/utils.py
--rw-r--r--   0        0        0      647 2023-05-05 15:48:50.971806 pydbtools-5.5.6/pyproject.toml
--rw-r--r--   0        0        0    10475 1970-01-01 00:00:00.000000 pydbtools-5.5.6/PKG-INFO
+-rw-r--r--   0        0        0       48 2023-07-25 14:30:31.049731 pydbtools-5.5.7/docs/README.md
+-rw-r--r--   0        0        0      855 2023-07-25 14:30:31.053731 pydbtools-5.5.7/pydbtools/__init__.py
+-rw-r--r--   0        0        0     1130 2023-07-25 14:30:31.053731 pydbtools-5.5.7/pydbtools/_sql_render.py
+-rw-r--r--   0        0        0    23104 2023-07-25 14:30:31.053731 pydbtools-5.5.7/pydbtools/_wrangler.py
+-rw-r--r--   0        0        0     6391 2023-07-25 14:30:31.053731 pydbtools-5.5.7/pydbtools/utils.py
+-rw-r--r--   0        0        0      857 2023-07-25 14:30:31.053731 pydbtools-5.5.7/pyproject.toml
+-rw-r--r--   0        0        0      941 1970-01-01 00:00:00.000000 pydbtools-5.5.7/PKG-INFO
```

### Comparing `pydbtools-5.5.6/pydbtools/__init__.py` & `pydbtools-5.5.7/pydbtools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,8 +29,8 @@
     create_table,
 )
 
 from ._sql_render import get_sql_from_file, render_sql_template  # noqa: F401
 
 from .utils import s3_path_join  # noqa: F401
 
-__version__ = "5.5.6"
+__version__ = "5.5.7"
```

### Comparing `pydbtools-5.5.6/pydbtools/_sql_render.py` & `pydbtools-5.5.7/pydbtools/_sql_render.py`

 * *Files identical despite different names*

### Comparing `pydbtools-5.5.6/pydbtools/_wrangler.py` & `pydbtools-5.5.7/pydbtools/_wrangler.py`

 * *Files identical despite different names*

### Comparing `pydbtools-5.5.6/pydbtools/utils.py` & `pydbtools-5.5.7/pydbtools/utils.py`

 * *Files identical despite different names*

