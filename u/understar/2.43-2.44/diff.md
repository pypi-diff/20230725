# Comparing `tmp/understar-2.43.tar.gz` & `tmp/understar-2.44.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "understar-2.43.tar", last modified: Wed Jul 19 07:43:29 2023, max compression
+gzip compressed data, was "understar-2.44.tar", last modified: Tue Jul 25 09:07:05 2023, max compression
```

## Comparing `understar-2.43.tar` & `understar-2.44.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-19 07:43:29.104736 understar-2.43/
--rw-r--r--   0 maxence    (501) staff       (20)     1188 2023-05-26 01:06:57.000000 understar-2.43/LICENSE.md
--rw-r--r--   0 maxence    (501) staff       (20)      590 2023-07-19 07:43:29.104557 understar-2.43/PKG-INFO
--rw-r--r--   0 maxence    (501) staff       (20)       45 2023-05-26 01:06:57.000000 understar-2.43/README.md
--rw-r--r--   0 maxence    (501) staff       (20)       38 2023-07-19 07:43:29.104787 understar-2.43/setup.cfg
--rw-r--r--   0 maxence    (501) staff       (20)     1885 2023-07-19 05:42:26.000000 understar-2.43/setup.py
-drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-19 07:43:29.098090 understar-2.43/understar/
--rw-r--r--   0 maxence    (501) staff       (20)        5 2023-07-19 07:39:39.000000 understar-2.43/understar/.version
--rw-r--r--   0 maxence    (501) staff       (20)       25 2023-07-19 04:14:38.000000 understar-2.43/understar/__init__.py
-drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-19 07:43:29.099144 understar-2.43/understar/system/
--rw-r--r--   0 maxence    (501) staff       (20)       22 2023-07-16 04:49:43.000000 understar-2.43/understar/system/__init__.py
-drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-19 07:43:29.099431 understar-2.43/understar/system/app/
--rw-r--r--   0 maxence    (501) staff       (20)       89 2023-07-16 04:47:12.000000 understar-2.43/understar/system/app/__init__.py
-drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-19 07:43:29.099854 understar-2.43/understar/system/app/config/
--rw-r--r--   0 maxence    (501) staff       (20)    20066 2023-07-19 04:34:41.000000 understar-2.43/understar/system/app/config/__init__.py
-drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-19 07:43:29.101083 understar-2.43/understar/system/app/config/apt/
--rw-r--r--   0 maxence    (501) staff       (20)       32 2023-07-12 03:26:34.000000 understar-2.43/understar/system/app/config/apt/__init__.py
--rw-r--r--   0 maxence    (501) staff       (20)     3351 2023-07-19 04:34:43.000000 understar-2.43/understar/system/app/config/apt/install.py
--rw-r--r--   0 maxence    (501) staff       (20)     1329 2023-07-19 04:34:44.000000 understar-2.43/understar/system/app/config/apt/uninstall.py
-drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-19 07:43:29.101310 understar-2.43/understar/system/app/maintenance/
--rw-r--r--   0 maxence    (501) staff       (20)      902 2023-07-19 04:34:46.000000 understar-2.43/understar/system/app/maintenance/__init__.py
-drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-19 07:43:29.104039 understar-2.43/understar/system/lib/
--rw-r--r--   0 maxence    (501) staff       (20)      149 2023-07-12 03:30:52.000000 understar-2.43/understar/system/lib/__init__.py
--rw-r--r--   0 maxence    (501) staff       (20)     5517 2023-07-19 02:04:00.000000 understar-2.43/understar/system/lib/app.py
--rw-r--r--   0 maxence    (501) staff       (20)     1015 2023-06-23 09:10:23.000000 understar-2.43/understar/system/lib/com.py
--rw-r--r--   0 maxence    (501) staff       (20)    11757 2023-06-19 00:59:20.000000 understar-2.43/understar/system/lib/event.py
--rw-r--r--   0 maxence    (501) staff       (20)     3784 2023-06-19 05:27:26.000000 understar-2.43/understar/system/lib/save.py
--rw-r--r--   0 maxence    (501) staff       (20)     2716 2023-07-19 04:01:29.000000 understar-2.43/understar/system/lib/store.py
--rw-r--r--   0 maxence    (501) staff       (20)      174 2023-06-23 09:10:04.000000 understar-2.43/understar/system/lib/types.py
--rw-r--r--   0 maxence    (501) staff       (20)     5159 2023-07-19 06:50:46.000000 understar-2.43/understar/system/lib/utils.py
--rw-r--r--   0 maxence    (501) staff       (20)    31915 2023-07-19 07:35:47.000000 understar-2.43/understar/understar.py
-drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-19 07:43:29.099020 understar-2.43/understar.egg-info/
--rw-r--r--   0 maxence    (501) staff       (20)      590 2023-07-19 07:43:29.000000 understar-2.43/understar.egg-info/PKG-INFO
--rw-r--r--   0 maxence    (501) staff       (20)      774 2023-07-19 07:43:29.000000 understar-2.43/understar.egg-info/SOURCES.txt
--rw-r--r--   0 maxence    (501) staff       (20)        1 2023-07-19 07:43:29.000000 understar-2.43/understar.egg-info/dependency_links.txt
--rw-r--r--   0 maxence    (501) staff       (20)       49 2023-07-19 07:43:29.000000 understar-2.43/understar.egg-info/requires.txt
--rw-r--r--   0 maxence    (501) staff       (20)       10 2023-07-19 07:43:29.000000 understar-2.43/understar.egg-info/top_level.txt
+drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-25 09:07:05.255045 understar-2.44/
+-rw-r--r--   0 maxence    (501) staff       (20)     1188 2023-05-26 01:06:57.000000 understar-2.44/LICENSE.md
+-rw-r--r--   0 maxence    (501) staff       (20)      590 2023-07-25 09:07:05.254930 understar-2.44/PKG-INFO
+-rw-r--r--   0 maxence    (501) staff       (20)       45 2023-05-26 01:06:57.000000 understar-2.44/README.md
+-rw-r--r--   0 maxence    (501) staff       (20)       38 2023-07-25 09:07:05.255113 understar-2.44/setup.cfg
+-rw-r--r--   0 maxence    (501) staff       (20)     1885 2023-07-19 05:42:26.000000 understar-2.44/setup.py
+drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-25 09:07:05.248754 understar-2.44/understar/
+-rw-r--r--   0 maxence    (501) staff       (20)        5 2023-07-25 09:06:50.000000 understar-2.44/understar/.version
+-rw-r--r--   0 maxence    (501) staff       (20)       25 2023-07-19 04:14:38.000000 understar-2.44/understar/__init__.py
+drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-25 09:07:05.250048 understar-2.44/understar/system/
+-rw-r--r--   0 maxence    (501) staff       (20)       22 2023-07-16 04:49:43.000000 understar-2.44/understar/system/__init__.py
+drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-25 09:07:05.250455 understar-2.44/understar/system/app/
+-rw-r--r--   0 maxence    (501) staff       (20)       89 2023-07-16 04:47:12.000000 understar-2.44/understar/system/app/__init__.py
+drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-25 09:07:05.250805 understar-2.44/understar/system/app/config/
+-rw-r--r--   0 maxence    (501) staff       (20)    20066 2023-07-19 04:34:41.000000 understar-2.44/understar/system/app/config/__init__.py
+drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-25 09:07:05.251809 understar-2.44/understar/system/app/config/apt/
+-rw-r--r--   0 maxence    (501) staff       (20)       32 2023-07-12 03:26:34.000000 understar-2.44/understar/system/app/config/apt/__init__.py
+-rw-r--r--   0 maxence    (501) staff       (20)     3351 2023-07-19 04:34:43.000000 understar-2.44/understar/system/app/config/apt/install.py
+-rw-r--r--   0 maxence    (501) staff       (20)     1321 2023-07-25 09:05:39.000000 understar-2.44/understar/system/app/config/apt/uninstall.py
+drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-25 09:07:05.252074 understar-2.44/understar/system/app/maintenance/
+-rw-r--r--   0 maxence    (501) staff       (20)      902 2023-07-19 04:34:46.000000 understar-2.44/understar/system/app/maintenance/__init__.py
+drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-25 09:07:05.254532 understar-2.44/understar/system/lib/
+-rw-r--r--   0 maxence    (501) staff       (20)      149 2023-07-12 03:30:52.000000 understar-2.44/understar/system/lib/__init__.py
+-rw-r--r--   0 maxence    (501) staff       (20)     5517 2023-07-19 02:04:00.000000 understar-2.44/understar/system/lib/app.py
+-rw-r--r--   0 maxence    (501) staff       (20)     1015 2023-06-23 09:10:23.000000 understar-2.44/understar/system/lib/com.py
+-rw-r--r--   0 maxence    (501) staff       (20)    11757 2023-06-19 00:59:20.000000 understar-2.44/understar/system/lib/event.py
+-rw-r--r--   0 maxence    (501) staff       (20)     3784 2023-06-19 05:27:26.000000 understar-2.44/understar/system/lib/save.py
+-rw-r--r--   0 maxence    (501) staff       (20)     2716 2023-07-19 04:01:29.000000 understar-2.44/understar/system/lib/store.py
+-rw-r--r--   0 maxence    (501) staff       (20)      174 2023-06-23 09:10:04.000000 understar-2.44/understar/system/lib/types.py
+-rw-r--r--   0 maxence    (501) staff       (20)     5159 2023-07-19 06:50:46.000000 understar-2.44/understar/system/lib/utils.py
+-rw-r--r--   0 maxence    (501) staff       (20)    31915 2023-07-19 07:35:47.000000 understar-2.44/understar/understar.py
+drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-25 09:07:05.249880 understar-2.44/understar.egg-info/
+-rw-r--r--   0 maxence    (501) staff       (20)      590 2023-07-25 09:07:05.000000 understar-2.44/understar.egg-info/PKG-INFO
+-rw-r--r--   0 maxence    (501) staff       (20)      774 2023-07-25 09:07:05.000000 understar-2.44/understar.egg-info/SOURCES.txt
+-rw-r--r--   0 maxence    (501) staff       (20)        1 2023-07-25 09:07:05.000000 understar-2.44/understar.egg-info/dependency_links.txt
+-rw-r--r--   0 maxence    (501) staff       (20)       49 2023-07-25 09:07:05.000000 understar-2.44/understar.egg-info/requires.txt
+-rw-r--r--   0 maxence    (501) staff       (20)       10 2023-07-25 09:07:05.000000 understar-2.44/understar.egg-info/top_level.txt
```

### Comparing `understar-2.43/LICENSE.md` & `understar-2.44/LICENSE.md`

 * *Files identical despite different names*

### Comparing `understar-2.43/PKG-INFO` & `understar-2.44/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: understar
-Version: 2.43
+Version: 2.44
 Summary: A discord bot framewrok
 Home-page: https://github.com/GalTechDev/UnderStar-OS
 Download-URL: https://github.com/GalTechDev/UnderStar-OS/tarball/master
 Author: GalTech
 Author-email: poussigalitv@gmail.com
 License: MIT
 Keywords: discord,bot,discord.py,understar,os,framework
```

### Comparing `understar-2.43/setup.py` & `understar-2.44/setup.py`

 * *Files identical despite different names*

### Comparing `understar-2.43/understar/system/app/config/__init__.py` & `understar-2.44/understar/system/app/config/__init__.py`

 * *Files identical despite different names*

### Comparing `understar-2.43/understar/system/app/config/apt/install.py` & `understar-2.44/understar/system/app/config/apt/install.py`

 * *Files identical despite different names*

### Comparing `understar-2.43/understar/system/app/config/apt/uninstall.py` & `understar-2.44/understar/system/app/config/apt/uninstall.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,12 +23,12 @@
 #@Lib.app.slash(name="delete", description="delete from machine", guilds=None)
 #@discord.app_commands.check(Lib.is_in_staff)
 async def delete(ctx:discord.Interaction, app_name:str, remove_save:bool=False):
     if Lib.store.is_downloaded(app_name):
         rmtree(f"app/{app_name}")
         app_name = app_name
 
-        Lib.store.installed_app.all_app.pop(app_name)
+        Lib.store.installed_app.pop(app_name)
         await ctx.response.send_message("Supprimé.", ephemeral=True)
 
     else:
         await ctx.response.send_message("Application non trouvée", ephemeral=True)
```

### Comparing `understar-2.43/understar/system/app/maintenance/__init__.py` & `understar-2.44/understar/system/app/maintenance/__init__.py`

 * *Files identical despite different names*

### Comparing `understar-2.43/understar/system/lib/app.py` & `understar-2.44/understar/system/lib/app.py`

 * *Files identical despite different names*

### Comparing `understar-2.43/understar/system/lib/com.py` & `understar-2.44/understar/system/lib/com.py`

 * *Files identical despite different names*

### Comparing `understar-2.43/understar/system/lib/event.py` & `understar-2.44/understar/system/lib/event.py`

 * *Files identical despite different names*

### Comparing `understar-2.43/understar/system/lib/save.py` & `understar-2.44/understar/system/lib/save.py`

 * *Files identical despite different names*

### Comparing `understar-2.43/understar/system/lib/store.py` & `understar-2.44/understar/system/lib/store.py`

 * *Files identical despite different names*

### Comparing `understar-2.43/understar/system/lib/utils.py` & `understar-2.44/understar/system/lib/utils.py`

 * *Files identical despite different names*

### Comparing `understar-2.43/understar/understar.py` & `understar-2.44/understar/understar.py`

 * *Files identical despite different names*

### Comparing `understar-2.43/understar.egg-info/PKG-INFO` & `understar-2.44/understar.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: understar
-Version: 2.43
+Version: 2.44
 Summary: A discord bot framewrok
 Home-page: https://github.com/GalTechDev/UnderStar-OS
 Download-URL: https://github.com/GalTechDev/UnderStar-OS/tarball/master
 Author: GalTech
 Author-email: poussigalitv@gmail.com
 License: MIT
 Keywords: discord,bot,discord.py,understar,os,framework
```

### Comparing `understar-2.43/understar.egg-info/SOURCES.txt` & `understar-2.44/understar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

