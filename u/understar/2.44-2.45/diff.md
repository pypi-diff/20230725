# Comparing `tmp/understar-2.44.tar.gz` & `tmp/understar-2.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "understar-2.44.tar", last modified: Tue Jul 25 09:07:05 2023, max compression
+gzip compressed data, was "understar-2.45.tar", last modified: Tue Jul 25 09:56:09 2023, max compression
```

## Comparing `understar-2.44.tar` & `understar-2.45.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-25 09:07:05.255045 understar-2.44/
--rw-r--r--   0 maxence    (501) staff       (20)     1188 2023-05-26 01:06:57.000000 understar-2.44/LICENSE.md
--rw-r--r--   0 maxence    (501) staff       (20)      590 2023-07-25 09:07:05.254930 understar-2.44/PKG-INFO
--rw-r--r--   0 maxence    (501) staff       (20)       45 2023-05-26 01:06:57.000000 understar-2.44/README.md
--rw-r--r--   0 maxence    (501) staff       (20)       38 2023-07-25 09:07:05.255113 understar-2.44/setup.cfg
--rw-r--r--   0 maxence    (501) staff       (20)     1885 2023-07-19 05:42:26.000000 understar-2.44/setup.py
-drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-25 09:07:05.248754 understar-2.44/understar/
--rw-r--r--   0 maxence    (501) staff       (20)        5 2023-07-25 09:06:50.000000 understar-2.44/understar/.version
--rw-r--r--   0 maxence    (501) staff       (20)       25 2023-07-19 04:14:38.000000 understar-2.44/understar/__init__.py
-drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-25 09:07:05.250048 understar-2.44/understar/system/
--rw-r--r--   0 maxence    (501) staff       (20)       22 2023-07-16 04:49:43.000000 understar-2.44/understar/system/__init__.py
-drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-25 09:07:05.250455 understar-2.44/understar/system/app/
--rw-r--r--   0 maxence    (501) staff       (20)       89 2023-07-16 04:47:12.000000 understar-2.44/understar/system/app/__init__.py
-drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-25 09:07:05.250805 understar-2.44/understar/system/app/config/
--rw-r--r--   0 maxence    (501) staff       (20)    20066 2023-07-19 04:34:41.000000 understar-2.44/understar/system/app/config/__init__.py
-drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-25 09:07:05.251809 understar-2.44/understar/system/app/config/apt/
--rw-r--r--   0 maxence    (501) staff       (20)       32 2023-07-12 03:26:34.000000 understar-2.44/understar/system/app/config/apt/__init__.py
--rw-r--r--   0 maxence    (501) staff       (20)     3351 2023-07-19 04:34:43.000000 understar-2.44/understar/system/app/config/apt/install.py
--rw-r--r--   0 maxence    (501) staff       (20)     1321 2023-07-25 09:05:39.000000 understar-2.44/understar/system/app/config/apt/uninstall.py
-drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-25 09:07:05.252074 understar-2.44/understar/system/app/maintenance/
--rw-r--r--   0 maxence    (501) staff       (20)      902 2023-07-19 04:34:46.000000 understar-2.44/understar/system/app/maintenance/__init__.py
-drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-25 09:07:05.254532 understar-2.44/understar/system/lib/
--rw-r--r--   0 maxence    (501) staff       (20)      149 2023-07-12 03:30:52.000000 understar-2.44/understar/system/lib/__init__.py
--rw-r--r--   0 maxence    (501) staff       (20)     5517 2023-07-19 02:04:00.000000 understar-2.44/understar/system/lib/app.py
--rw-r--r--   0 maxence    (501) staff       (20)     1015 2023-06-23 09:10:23.000000 understar-2.44/understar/system/lib/com.py
--rw-r--r--   0 maxence    (501) staff       (20)    11757 2023-06-19 00:59:20.000000 understar-2.44/understar/system/lib/event.py
--rw-r--r--   0 maxence    (501) staff       (20)     3784 2023-06-19 05:27:26.000000 understar-2.44/understar/system/lib/save.py
--rw-r--r--   0 maxence    (501) staff       (20)     2716 2023-07-19 04:01:29.000000 understar-2.44/understar/system/lib/store.py
--rw-r--r--   0 maxence    (501) staff       (20)      174 2023-06-23 09:10:04.000000 understar-2.44/understar/system/lib/types.py
--rw-r--r--   0 maxence    (501) staff       (20)     5159 2023-07-19 06:50:46.000000 understar-2.44/understar/system/lib/utils.py
--rw-r--r--   0 maxence    (501) staff       (20)    31915 2023-07-19 07:35:47.000000 understar-2.44/understar/understar.py
-drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-25 09:07:05.249880 understar-2.44/understar.egg-info/
--rw-r--r--   0 maxence    (501) staff       (20)      590 2023-07-25 09:07:05.000000 understar-2.44/understar.egg-info/PKG-INFO
--rw-r--r--   0 maxence    (501) staff       (20)      774 2023-07-25 09:07:05.000000 understar-2.44/understar.egg-info/SOURCES.txt
--rw-r--r--   0 maxence    (501) staff       (20)        1 2023-07-25 09:07:05.000000 understar-2.44/understar.egg-info/dependency_links.txt
--rw-r--r--   0 maxence    (501) staff       (20)       49 2023-07-25 09:07:05.000000 understar-2.44/understar.egg-info/requires.txt
--rw-r--r--   0 maxence    (501) staff       (20)       10 2023-07-25 09:07:05.000000 understar-2.44/understar.egg-info/top_level.txt
+drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-25 09:56:09.504172 understar-2.45/
+-rw-r--r--   0 maxence    (501) staff       (20)     1188 2023-05-26 01:06:57.000000 understar-2.45/LICENSE.md
+-rw-r--r--   0 maxence    (501) staff       (20)      590 2023-07-25 09:56:09.504056 understar-2.45/PKG-INFO
+-rw-r--r--   0 maxence    (501) staff       (20)       45 2023-05-26 01:06:57.000000 understar-2.45/README.md
+-rw-r--r--   0 maxence    (501) staff       (20)       38 2023-07-25 09:56:09.504236 understar-2.45/setup.cfg
+-rw-r--r--   0 maxence    (501) staff       (20)     1885 2023-07-19 05:42:26.000000 understar-2.45/setup.py
+drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-25 09:56:09.498778 understar-2.45/understar/
+-rw-r--r--   0 maxence    (501) staff       (20)        5 2023-07-25 09:55:45.000000 understar-2.45/understar/.version
+-rw-r--r--   0 maxence    (501) staff       (20)       25 2023-07-19 04:14:38.000000 understar-2.45/understar/__init__.py
+drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-25 09:56:09.500058 understar-2.45/understar/system/
+-rw-r--r--   0 maxence    (501) staff       (20)       22 2023-07-16 04:49:43.000000 understar-2.45/understar/system/__init__.py
+drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-25 09:56:09.500339 understar-2.45/understar/system/app/
+-rw-r--r--   0 maxence    (501) staff       (20)       89 2023-07-16 04:47:12.000000 understar-2.45/understar/system/app/__init__.py
+drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-25 09:56:09.500606 understar-2.45/understar/system/app/config/
+-rw-r--r--   0 maxence    (501) staff       (20)    20066 2023-07-19 04:34:41.000000 understar-2.45/understar/system/app/config/__init__.py
+drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-25 09:56:09.501379 understar-2.45/understar/system/app/config/apt/
+-rw-r--r--   0 maxence    (501) staff       (20)       32 2023-07-12 03:26:34.000000 understar-2.45/understar/system/app/config/apt/__init__.py
+-rw-r--r--   0 maxence    (501) staff       (20)     3343 2023-07-25 09:10:06.000000 understar-2.45/understar/system/app/config/apt/install.py
+-rw-r--r--   0 maxence    (501) staff       (20)     1321 2023-07-25 09:05:39.000000 understar-2.45/understar/system/app/config/apt/uninstall.py
+drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-25 09:56:09.501519 understar-2.45/understar/system/app/maintenance/
+-rw-r--r--   0 maxence    (501) staff       (20)      902 2023-07-19 04:34:46.000000 understar-2.45/understar/system/app/maintenance/__init__.py
+drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-25 09:56:09.503641 understar-2.45/understar/system/lib/
+-rw-r--r--   0 maxence    (501) staff       (20)      149 2023-07-12 03:30:52.000000 understar-2.45/understar/system/lib/__init__.py
+-rw-r--r--   0 maxence    (501) staff       (20)     5517 2023-07-19 02:04:00.000000 understar-2.45/understar/system/lib/app.py
+-rw-r--r--   0 maxence    (501) staff       (20)     1015 2023-06-23 09:10:23.000000 understar-2.45/understar/system/lib/com.py
+-rw-r--r--   0 maxence    (501) staff       (20)    11757 2023-06-19 00:59:20.000000 understar-2.45/understar/system/lib/event.py
+-rw-r--r--   0 maxence    (501) staff       (20)     3784 2023-06-19 05:27:26.000000 understar-2.45/understar/system/lib/save.py
+-rw-r--r--   0 maxence    (501) staff       (20)     2716 2023-07-19 04:01:29.000000 understar-2.45/understar/system/lib/store.py
+-rw-r--r--   0 maxence    (501) staff       (20)      174 2023-06-23 09:10:04.000000 understar-2.45/understar/system/lib/types.py
+-rw-r--r--   0 maxence    (501) staff       (20)     5159 2023-07-19 06:50:46.000000 understar-2.45/understar/system/lib/utils.py
+-rw-r--r--   0 maxence    (501) staff       (20)    31915 2023-07-19 07:35:47.000000 understar-2.45/understar/understar.py
+drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-25 09:56:09.499908 understar-2.45/understar.egg-info/
+-rw-r--r--   0 maxence    (501) staff       (20)      590 2023-07-25 09:56:09.000000 understar-2.45/understar.egg-info/PKG-INFO
+-rw-r--r--   0 maxence    (501) staff       (20)      774 2023-07-25 09:56:09.000000 understar-2.45/understar.egg-info/SOURCES.txt
+-rw-r--r--   0 maxence    (501) staff       (20)        1 2023-07-25 09:56:09.000000 understar-2.45/understar.egg-info/dependency_links.txt
+-rw-r--r--   0 maxence    (501) staff       (20)       49 2023-07-25 09:56:09.000000 understar-2.45/understar.egg-info/requires.txt
+-rw-r--r--   0 maxence    (501) staff       (20)       10 2023-07-25 09:56:09.000000 understar-2.45/understar.egg-info/top_level.txt
```

### Comparing `understar-2.44/LICENSE.md` & `understar-2.45/LICENSE.md`

 * *Files identical despite different names*

### Comparing `understar-2.44/PKG-INFO` & `understar-2.45/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: understar
-Version: 2.44
+Version: 2.45
 Summary: A discord bot framewrok
 Home-page: https://github.com/GalTechDev/UnderStar-OS
 Download-URL: https://github.com/GalTechDev/UnderStar-OS/tarball/master
 Author: GalTech
 Author-email: poussigalitv@gmail.com
 License: MIT
 Keywords: discord,bot,discord.py,understar,os,framework
```

### Comparing `understar-2.44/setup.py` & `understar-2.45/setup.py`

 * *Files identical despite different names*

### Comparing `understar-2.44/understar/system/app/config/__init__.py` & `understar-2.45/understar/system/app/config/__init__.py`

 * *Files identical despite different names*

### Comparing `understar-2.44/understar/system/app/config/apt/install.py` & `understar-2.45/understar/system/app/config/apt/install.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
             if len(listdir(path_folder))==2:
                 remove(file_path)
                 old_name = listdir(path_folder)[0]
                 move(f"{path_folder}/{old_name}", "app")
                 rename(f"app/{old_name}", f'app/{app_name.replace("-", "_")}')
                 
                 rmtree(path_folder)
-                Lib.store.installed_app.all_app.update({app_name:None})
+                Lib.store.installed_app.update({app_name:None})
                 await ctx.response.send_message("Installé", ephemeral=True)
 
             else:
                 await ctx.response.send_message("Plus d'un élément trouvé dans l'archive, installation ignorée", ephemeral=True)
                 rmtree(path_folder)
 
         else:
```

### Comparing `understar-2.44/understar/system/app/config/apt/uninstall.py` & `understar-2.45/understar/system/app/config/apt/uninstall.py`

 * *Files identical despite different names*

### Comparing `understar-2.44/understar/system/app/maintenance/__init__.py` & `understar-2.45/understar/system/app/maintenance/__init__.py`

 * *Files identical despite different names*

### Comparing `understar-2.44/understar/system/lib/app.py` & `understar-2.45/understar/system/lib/app.py`

 * *Files identical despite different names*

### Comparing `understar-2.44/understar/system/lib/com.py` & `understar-2.45/understar/system/lib/com.py`

 * *Files identical despite different names*

### Comparing `understar-2.44/understar/system/lib/event.py` & `understar-2.45/understar/system/lib/event.py`

 * *Files identical despite different names*

### Comparing `understar-2.44/understar/system/lib/save.py` & `understar-2.45/understar/system/lib/save.py`

 * *Files identical despite different names*

### Comparing `understar-2.44/understar/system/lib/store.py` & `understar-2.45/understar/system/lib/store.py`

 * *Files identical despite different names*

### Comparing `understar-2.44/understar/system/lib/utils.py` & `understar-2.45/understar/system/lib/utils.py`

 * *Files identical despite different names*

### Comparing `understar-2.44/understar/understar.py` & `understar-2.45/understar/understar.py`

 * *Files identical despite different names*

### Comparing `understar-2.44/understar.egg-info/PKG-INFO` & `understar-2.45/understar.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: understar
-Version: 2.44
+Version: 2.45
 Summary: A discord bot framewrok
 Home-page: https://github.com/GalTechDev/UnderStar-OS
 Download-URL: https://github.com/GalTechDev/UnderStar-OS/tarball/master
 Author: GalTech
 Author-email: poussigalitv@gmail.com
 License: MIT
 Keywords: discord,bot,discord.py,understar,os,framework
```

### Comparing `understar-2.44/understar.egg-info/SOURCES.txt` & `understar-2.45/understar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

