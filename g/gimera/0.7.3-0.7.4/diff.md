# Comparing `tmp/gimera-0.7.3.tar.gz` & `tmp/gimera-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gimera-0.7.3.tar", last modified: Mon Jul 24 22:29:47 2023, max compression
+gzip compressed data, was "gimera-0.7.4.tar", last modified: Mon Jul 24 22:34:46 2023, max compression
```

## Comparing `gimera-0.7.3.tar` & `gimera-0.7.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:29:47.524883 gimera-0.7.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-24 22:29:00.000000 gimera-0.7.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-07-24 22:29:47.524883 gimera-0.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-07-24 22:29:00.000000 gimera-0.7.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:29:47.524883 gimera-0.7.3/gimera/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-24 22:29:00.000000 gimera-0.7.3/gimera/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10482 2023-07-24 22:29:00.000000 gimera-0.7.3/gimera/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-24 22:29:00.000000 gimera-0.7.3/gimera/consts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    28893 2023-07-24 22:29:00.000000 gimera-0.7.3/gimera/gimera.py
--rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-07-24 22:29:00.000000 gimera-0.7.3/gimera/gitcommands.py
--rw-r--r--   0 runner    (1001) docker     (123)    14437 2023-07-24 22:29:00.000000 gimera-0.7.3/gimera/patches.py
--rw-r--r--   0 runner    (1001) docker     (123)    12993 2023-07-24 22:29:00.000000 gimera-0.7.3/gimera/repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-07-24 22:29:00.000000 gimera-0.7.3/gimera/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:29:47.524883 gimera-0.7.3/gimera.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-07-24 22:29:47.000000 gimera-0.7.3/gimera.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-24 22:29:47.000000 gimera-0.7.3/gimera.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 22:29:47.000000 gimera-0.7.3/gimera.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-24 22:29:47.000000 gimera-0.7.3/gimera.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-24 22:29:47.000000 gimera-0.7.3/gimera.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-24 22:29:47.000000 gimera-0.7.3/gimera.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-24 22:29:47.524883 gimera-0.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-07-24 22:29:00.000000 gimera-0.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:34:46.139651 gimera-0.7.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-24 22:33:58.000000 gimera-0.7.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-07-24 22:34:46.139651 gimera-0.7.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-07-24 22:33:58.000000 gimera-0.7.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:34:46.139651 gimera-0.7.4/gimera/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-24 22:33:58.000000 gimera-0.7.4/gimera/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10613 2023-07-24 22:33:58.000000 gimera-0.7.4/gimera/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-24 22:33:58.000000 gimera-0.7.4/gimera/consts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    28893 2023-07-24 22:33:58.000000 gimera-0.7.4/gimera/gimera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-07-24 22:33:58.000000 gimera-0.7.4/gimera/gitcommands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14437 2023-07-24 22:33:58.000000 gimera-0.7.4/gimera/patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12993 2023-07-24 22:33:58.000000 gimera-0.7.4/gimera/repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-07-24 22:33:58.000000 gimera-0.7.4/gimera/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:34:46.139651 gimera-0.7.4/gimera.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-07-24 22:34:46.000000 gimera-0.7.4/gimera.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-24 22:34:46.000000 gimera-0.7.4/gimera.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 22:34:46.000000 gimera-0.7.4/gimera.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-24 22:34:46.000000 gimera-0.7.4/gimera.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-24 22:34:46.000000 gimera-0.7.4/gimera.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-24 22:34:46.000000 gimera-0.7.4/gimera.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-24 22:34:46.139651 gimera-0.7.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-07-24 22:33:58.000000 gimera-0.7.4/setup.py
```

### Comparing `gimera-0.7.3/LICENSE.txt` & `gimera-0.7.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gimera-0.7.3/PKG-INFO` & `gimera-0.7.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gimera
-Version: 0.7.3
+Version: 0.7.4
 Summary: Handling git submodules and patches per yml
 Home-page: https://github.com/marcwimmer/gimera
 Author: Marc-Christian Wimmer
 Author-email: marc@itewimmer.de
 License: MIT
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
```

### Comparing `gimera-0.7.3/README.md` & `gimera-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `gimera-0.7.3/gimera/config.py` & `gimera-0.7.4/gimera/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,15 +109,18 @@
             if Path(repo["path"]) == param_repo.path:
                 for k, v in value.items():
                     repo[k] = v
                 break
         else:
             config["repos"].append(value)
         for k, v in value.items():
-            setattr(param_repo, k, v)
+            try:
+                setattr(param_repo, k, v)
+            except AttributeError as ex:
+                raise Exception(f"Cannot set attribute {k}") from ex
         self.config_file.write_text(yaml.dump(config, default_flow_style=False))
         main_repo.please_no_staged_files()
         if self.config_file.resolve() in [
             x.resolve() for x in main_repo.all_dirty_files
         ]:
             main_repo.X("git", "add", self.config_file)
         if main_repo.staged_files:
```

### Comparing `gimera-0.7.3/gimera/gimera.py` & `gimera-0.7.4/gimera/gimera.py`

 * *Files identical despite different names*

### Comparing `gimera-0.7.3/gimera/gitcommands.py` & `gimera-0.7.4/gimera/gitcommands.py`

 * *Files identical despite different names*

### Comparing `gimera-0.7.3/gimera/patches.py` & `gimera-0.7.4/gimera/patches.py`

 * *Files identical despite different names*

### Comparing `gimera-0.7.3/gimera/repo.py` & `gimera-0.7.4/gimera/repo.py`

 * *Files identical despite different names*

### Comparing `gimera-0.7.3/gimera/tools.py` & `gimera-0.7.4/gimera/tools.py`

 * *Files identical despite different names*

### Comparing `gimera-0.7.3/gimera.egg-info/PKG-INFO` & `gimera-0.7.4/gimera.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gimera
-Version: 0.7.3
+Version: 0.7.4
 Summary: Handling git submodules and patches per yml
 Home-page: https://github.com/marcwimmer/gimera
 Author: Marc-Christian Wimmer
 Author-email: marc@itewimmer.de
 License: MIT
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
```

### Comparing `gimera-0.7.3/setup.py` & `gimera-0.7.4/setup.py`

 * *Files identical despite different names*

