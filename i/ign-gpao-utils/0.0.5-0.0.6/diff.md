# Comparing `tmp/ign-gpao-utils-0.0.5.tar.gz` & `tmp/ign-gpao-utils-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ign-gpao-utils-0.0.5.tar", last modified: Thu Jul 20 08:22:04 2023, max compression
+gzip compressed data, was "ign-gpao-utils-0.0.6.tar", last modified: Tue Jul 25 09:09:48 2023, max compression
```

## Comparing `ign-gpao-utils-0.0.5.tar` & `ign-gpao-utils-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:22:04.491248 ign-gpao-utils-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-20 08:22:04.491248 ign-gpao-utils-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-20 08:22:00.000000 ign-gpao-utils-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:22:04.491248 ign-gpao-utils-0.0.5/gpao_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 08:22:00.000000 ign-gpao-utils-0.0.5/gpao_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-20 08:22:00.000000 ign-gpao-utils-0.0.5/gpao_utils/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-20 08:22:00.000000 ign-gpao-utils-0.0.5/gpao_utils/interface_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-07-20 08:22:00.000000 ign-gpao-utils-0.0.5/gpao_utils/utils_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:22:04.491248 ign-gpao-utils-0.0.5/ign_gpao_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-20 08:22:04.000000 ign-gpao-utils-0.0.5/ign_gpao_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-20 08:22:04.000000 ign-gpao-utils-0.0.5/ign_gpao_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 08:22:04.000000 ign-gpao-utils-0.0.5/ign_gpao_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-20 08:22:04.000000 ign-gpao-utils-0.0.5/ign_gpao_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 08:22:04.491248 ign-gpao-utils-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-20 08:22:00.000000 ign-gpao-utils-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:22:04.491248 ign-gpao-utils-0.0.5/test/
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-20 08:22:00.000000 ign-gpao-utils-0.0.5/test/test_utils_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:09:48.144046 ign-gpao-utils-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-25 09:09:48.144046 ign-gpao-utils-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-25 09:09:42.000000 ign-gpao-utils-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:09:48.140046 ign-gpao-utils-0.0.6/gpao_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 09:09:42.000000 ign-gpao-utils-0.0.6/gpao_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-25 09:09:42.000000 ign-gpao-utils-0.0.6/gpao_utils/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-25 09:09:42.000000 ign-gpao-utils-0.0.6/gpao_utils/interface_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-07-25 09:09:42.000000 ign-gpao-utils-0.0.6/gpao_utils/utils_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:09:48.140046 ign-gpao-utils-0.0.6/ign_gpao_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-25 09:09:48.000000 ign-gpao-utils-0.0.6/ign_gpao_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-25 09:09:48.000000 ign-gpao-utils-0.0.6/ign_gpao_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 09:09:48.000000 ign-gpao-utils-0.0.6/ign_gpao_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-25 09:09:48.000000 ign-gpao-utils-0.0.6/ign_gpao_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 09:09:48.144046 ign-gpao-utils-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-25 09:09:42.000000 ign-gpao-utils-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:09:48.140046 ign-gpao-utils-0.0.6/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-25 09:09:42.000000 ign-gpao-utils-0.0.6/test/test_utils_store.py
```

### Comparing `ign-gpao-utils-0.0.5/gpao_utils/utils_store.py` & `ign-gpao-utils-0.0.6/gpao_utils/utils_store.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,11 +25,12 @@
         return res
 
 def frame_store(i: int, L: list):
     if len(L)!=i :
         raise RuntimeError(f"Not the same number of store in parameters. Number : {i}, List : {L}")
     layout_store = []
     for j in range(i):
+        layout_store.append([   sg.Text(L[j].upper())   ])
         layout_store.append([   sg.Text(f" {j} - Lettre (sur ma machine Windows)", size=(iu.size_text, 1)), sg.InputText(sg.user_settings_get_entry(f"-MAP-STORE{j}-WIN-LETTER", "L:"), key=f"-MAP-STORE{j}-WIN-LETTER", size=(iu.size_text_big,{j})) ])
         layout_store.append([   sg.Text(f" {j} - store Windows ", size=(iu.size_text, 1)), sg.InputText(sg.user_settings_get_entry(f"-MAP-STORE{j}-WIN", f"//store.ign.fr/{L[j]}"), key=f"-MAP-STORE{j}-WIN", size=(iu.size_text_big, 1))])
         layout_store.append([   sg.Text(f" {j} - store Linux ", size=(iu.size_text, 1)), sg.InputText(sg.user_settings_get_entry(f"-MAP-STORE{j}-UNIX", f"/var/data/{L[j]}"), key=f"-MAP-STORE{j}-UNIX", size=(iu.size_text_big, 1)) ])
     return sg.Frame("", layout_store)
```

### Comparing `ign-gpao-utils-0.0.5/setup.py` & `ign-gpao-utils-0.0.6/setup.py`

 * *Files identical despite different names*

