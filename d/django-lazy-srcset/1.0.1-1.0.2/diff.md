# Comparing `tmp/django-lazy-srcset-1.0.1.tar.gz` & `tmp/django-lazy-srcset-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-lazy-srcset-1.0.1.tar", last modified: Mon Jul 24 11:29:03 2023, max compression
+gzip compressed data, was "django-lazy-srcset-1.0.2.tar", last modified: Tue Jul 25 10:39:12 2023, max compression
```

## Comparing `django-lazy-srcset-1.0.1.tar` & `django-lazy-srcset-1.0.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-07-24 11:29:03.582717 django-lazy-srcset-1.0.1/
--rw-r--r--   0 quantra    (501) staff       (20)     1076 2023-05-02 22:05:05.000000 django-lazy-srcset-1.0.1/LICENSE
--rw-r--r--   0 quantra    (501) staff       (20)       73 2023-06-29 00:05:50.000000 django-lazy-srcset-1.0.1/MANIFEST.in
--rw-r--r--   0 quantra    (501) staff       (20)     9915 2023-07-24 11:29:03.582822 django-lazy-srcset-1.0.1/PKG-INFO
--rw-r--r--   0 quantra    (501) staff       (20)     8408 2023-07-24 11:21:20.000000 django-lazy-srcset-1.0.1/README.rst
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-07-24 11:29:03.574347 django-lazy-srcset-1.0.1/django_lazy_srcset.egg-info/
--rw-r--r--   0 quantra    (501) staff       (20)     9915 2023-07-24 11:29:03.000000 django-lazy-srcset-1.0.1/django_lazy_srcset.egg-info/PKG-INFO
--rw-r--r--   0 quantra    (501) staff       (20)      576 2023-07-24 11:29:03.000000 django-lazy-srcset-1.0.1/django_lazy_srcset.egg-info/SOURCES.txt
--rw-r--r--   0 quantra    (501) staff       (20)       40 2023-07-24 11:29:03.000000 django-lazy-srcset-1.0.1/django_lazy_srcset.egg-info/dependency_links.txt
--rw-r--r--   0 quantra    (501) staff       (20)       35 2023-07-24 11:29:03.000000 django-lazy-srcset-1.0.1/django_lazy_srcset.egg-info/requires.txt
--rw-r--r--   0 quantra    (501) staff       (20)       20 2023-07-24 11:29:03.000000 django-lazy-srcset-1.0.1/django_lazy_srcset.egg-info/top_level.txt
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-07-24 11:29:03.577616 django-lazy-srcset-1.0.1/lazy_srcset/
--rw-r--r--   0 quantra    (501) staff       (20)        0 2023-06-26 14:12:57.000000 django-lazy-srcset-1.0.1/lazy_srcset/__init__.py
--rw-r--r--   0 quantra    (501) staff       (20)       96 2023-06-26 17:31:28.000000 django-lazy-srcset-1.0.1/lazy_srcset/apps.py
--rw-r--r--   0 quantra    (501) staff       (20)     2227 2023-07-13 22:02:32.000000 django-lazy-srcset-1.0.1/lazy_srcset/conf.py
--rw-r--r--   0 quantra    (501) staff       (20)      679 2023-06-26 19:06:25.000000 django-lazy-srcset-1.0.1/lazy_srcset/imagegenerators.py
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-07-24 11:29:03.580309 django-lazy-srcset-1.0.1/lazy_srcset/management/
--rw-r--r--   0 quantra    (501) staff       (20)        0 2023-06-27 22:41:58.000000 django-lazy-srcset-1.0.1/lazy_srcset/management/__init__.py
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-07-24 11:29:03.581365 django-lazy-srcset-1.0.1/lazy_srcset/management/commands/
--rw-r--r--   0 quantra    (501) staff       (20)        0 2023-06-27 22:41:50.000000 django-lazy-srcset-1.0.1/lazy_srcset/management/commands/__init__.py
--rw-r--r--   0 quantra    (501) staff       (20)     3299 2023-06-29 00:03:00.000000 django-lazy-srcset-1.0.1/lazy_srcset/management/commands/imagekit_cleanup.py
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-07-24 11:29:03.582540 django-lazy-srcset-1.0.1/lazy_srcset/templatetags/
--rw-r--r--   0 quantra    (501) staff       (20)        0 2023-06-26 14:12:57.000000 django-lazy-srcset-1.0.1/lazy_srcset/templatetags/__init__.py
--rw-r--r--   0 quantra    (501) staff       (20)    12157 2023-07-12 20:39:22.000000 django-lazy-srcset-1.0.1/lazy_srcset/templatetags/lazy_srcset.py
--rw-r--r--   0 quantra    (501) staff       (20)       89 2023-06-26 19:06:22.000000 django-lazy-srcset-1.0.1/pyproject.toml
--rw-r--r--   0 quantra    (501) staff       (20)     1936 2023-07-24 11:29:03.586634 django-lazy-srcset-1.0.1/setup.cfg
--rw-r--r--   0 quantra    (501) staff       (20)       38 2023-06-26 17:04:23.000000 django-lazy-srcset-1.0.1/setup.py
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-07-25 10:39:12.527100 django-lazy-srcset-1.0.2/
+-rw-r--r--   0 quantra    (501) staff       (20)     1076 2023-05-02 22:05:05.000000 django-lazy-srcset-1.0.2/LICENSE
+-rw-r--r--   0 quantra    (501) staff       (20)       73 2023-06-29 00:05:50.000000 django-lazy-srcset-1.0.2/MANIFEST.in
+-rw-r--r--   0 quantra    (501) staff       (20)     9915 2023-07-25 10:39:12.527201 django-lazy-srcset-1.0.2/PKG-INFO
+-rw-r--r--   0 quantra    (501) staff       (20)     8408 2023-07-24 11:21:20.000000 django-lazy-srcset-1.0.2/README.rst
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-07-25 10:39:12.520798 django-lazy-srcset-1.0.2/django_lazy_srcset.egg-info/
+-rw-r--r--   0 quantra    (501) staff       (20)     9915 2023-07-25 10:39:12.000000 django-lazy-srcset-1.0.2/django_lazy_srcset.egg-info/PKG-INFO
+-rw-r--r--   0 quantra    (501) staff       (20)      576 2023-07-25 10:39:12.000000 django-lazy-srcset-1.0.2/django_lazy_srcset.egg-info/SOURCES.txt
+-rw-r--r--   0 quantra    (501) staff       (20)       40 2023-07-25 10:39:12.000000 django-lazy-srcset-1.0.2/django_lazy_srcset.egg-info/dependency_links.txt
+-rw-r--r--   0 quantra    (501) staff       (20)       35 2023-07-25 10:39:12.000000 django-lazy-srcset-1.0.2/django_lazy_srcset.egg-info/requires.txt
+-rw-r--r--   0 quantra    (501) staff       (20)       20 2023-07-25 10:39:12.000000 django-lazy-srcset-1.0.2/django_lazy_srcset.egg-info/top_level.txt
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-07-25 10:39:12.524121 django-lazy-srcset-1.0.2/lazy_srcset/
+-rw-r--r--   0 quantra    (501) staff       (20)        0 2023-06-26 14:12:57.000000 django-lazy-srcset-1.0.2/lazy_srcset/__init__.py
+-rw-r--r--   0 quantra    (501) staff       (20)       96 2023-06-26 17:31:28.000000 django-lazy-srcset-1.0.2/lazy_srcset/apps.py
+-rw-r--r--   0 quantra    (501) staff       (20)     2227 2023-07-24 21:31:27.000000 django-lazy-srcset-1.0.2/lazy_srcset/conf.py
+-rw-r--r--   0 quantra    (501) staff       (20)      679 2023-06-26 19:06:25.000000 django-lazy-srcset-1.0.2/lazy_srcset/imagegenerators.py
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-07-25 10:39:12.524926 django-lazy-srcset-1.0.2/lazy_srcset/management/
+-rw-r--r--   0 quantra    (501) staff       (20)        0 2023-06-27 22:41:58.000000 django-lazy-srcset-1.0.2/lazy_srcset/management/__init__.py
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-07-25 10:39:12.525803 django-lazy-srcset-1.0.2/lazy_srcset/management/commands/
+-rw-r--r--   0 quantra    (501) staff       (20)        0 2023-06-27 22:41:50.000000 django-lazy-srcset-1.0.2/lazy_srcset/management/commands/__init__.py
+-rw-r--r--   0 quantra    (501) staff       (20)     3818 2023-07-25 10:31:56.000000 django-lazy-srcset-1.0.2/lazy_srcset/management/commands/imagekit_cleanup.py
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-07-25 10:39:12.526940 django-lazy-srcset-1.0.2/lazy_srcset/templatetags/
+-rw-r--r--   0 quantra    (501) staff       (20)        0 2023-06-26 14:12:57.000000 django-lazy-srcset-1.0.2/lazy_srcset/templatetags/__init__.py
+-rw-r--r--   0 quantra    (501) staff       (20)    12157 2023-07-12 20:39:22.000000 django-lazy-srcset-1.0.2/lazy_srcset/templatetags/lazy_srcset.py
+-rw-r--r--   0 quantra    (501) staff       (20)       89 2023-06-26 19:06:22.000000 django-lazy-srcset-1.0.2/pyproject.toml
+-rw-r--r--   0 quantra    (501) staff       (20)     1936 2023-07-25 10:39:12.531265 django-lazy-srcset-1.0.2/setup.cfg
+-rw-r--r--   0 quantra    (501) staff       (20)       38 2023-06-26 17:04:23.000000 django-lazy-srcset-1.0.2/setup.py
```

### Comparing `django-lazy-srcset-1.0.1/LICENSE` & `django-lazy-srcset-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-lazy-srcset-1.0.1/PKG-INFO` & `django-lazy-srcset-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-lazy-srcset
-Version: 1.0.1
+Version: 1.0.2
 Summary: Lazy srcset and responsive image generation for Django. Minimum effort required. No database required.
 Home-page: https://github.com/Quantra/django-lazy-srcset
 Author: Vince Coleman
 Author-email: vince@shystudios.co.uk
 License: MIT
 Project-URL: Source, https://github.com/Quantra/django-lazy-srcset
 Keywords: django,django-lazy-srcset,django lazy srcset,django srcset,django responsive images,django responsive
```

### Comparing `django-lazy-srcset-1.0.1/README.rst` & `django-lazy-srcset-1.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `django-lazy-srcset-1.0.1/django_lazy_srcset.egg-info/PKG-INFO` & `django-lazy-srcset-1.0.2/django_lazy_srcset.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-lazy-srcset
-Version: 1.0.1
+Version: 1.0.2
 Summary: Lazy srcset and responsive image generation for Django. Minimum effort required. No database required.
 Home-page: https://github.com/Quantra/django-lazy-srcset
 Author: Vince Coleman
 Author-email: vince@shystudios.co.uk
 License: MIT
 Project-URL: Source, https://github.com/Quantra/django-lazy-srcset
 Keywords: django,django-lazy-srcset,django lazy srcset,django srcset,django responsive images,django responsive
```

### Comparing `django-lazy-srcset-1.0.1/django_lazy_srcset.egg-info/SOURCES.txt` & `django-lazy-srcset-1.0.2/django_lazy_srcset.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-lazy-srcset-1.0.1/lazy_srcset/conf.py` & `django-lazy-srcset-1.0.2/lazy_srcset/conf.py`

 * *Files identical despite different names*

### Comparing `django-lazy-srcset-1.0.1/lazy_srcset/imagegenerators.py` & `django-lazy-srcset-1.0.2/lazy_srcset/imagegenerators.py`

 * *Files identical despite different names*

### Comparing `django-lazy-srcset-1.0.1/lazy_srcset/management/commands/imagekit_cleanup.py` & `django-lazy-srcset-1.0.2/lazy_srcset/management/commands/imagekit_cleanup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,61 +9,80 @@
 For these reasons this remains an undocumented and untested feature.
 """
 
 import re
 from pathlib import Path
 
 from django.conf import settings
-from django.contrib.staticfiles import finders
 from django.core.cache import caches
 from django.core.files.storage import get_storage_class
 from django.core.management import BaseCommand
 
 
 class Command(BaseCommand):
     help = (
         "Deletes generated files for sources that no longer exist.  Ie you clean up your media files and this will"
         "clean up the imagekit files.  Suggest running once per day."
     )
     storage = None
+    static_storage = None
     root_path = None
     cache = None
 
+    def file_exists(self, path, file):
+        """
+        Check the storage and static storage for the file.
+        The file can have a different extension.
+        """
+        file_stem = Path(file).stem
+        for storage in [self.storage, self.static_storage]:
+            try:
+                directories, files = storage.listdir(path)
+            except FileNotFoundError:
+                continue
+
+            for f in files:
+                if Path(f).stem == file_stem:
+                    return True
+
+        return False
+
     def process_file(self, file, path):
         """
         Delete images that no longer have a source.
         """
         source_path = path.relative_to(self.root_path)
         source_file = re.sub(r"\.[a-z0-9]+\.", ".", file)  # noqa
-        source_filepath = source_path / source_file
 
-        if not self.storage.exists(source_filepath) and not finders.find(
-            source_filepath
-        ):
-            cache_key = f"{settings.IMAGEKIT_CACHE_PREFIX}{file}-state"
+        if not self.file_exists(source_path, source_file):
+            filepath = path / file
+
+            cache_key = f"{settings.IMAGEKIT_CACHE_PREFIX}{filepath.relative_to(self.root_path.parent)}-state"
             self.cache.delete(cache_key)
 
-            filepath = path / file
             self.storage.delete(filepath)
             self.stdout.write(f"Deleted: {filepath}")
 
-    def process_directory(self, directories, files, path):
+    def process_directory(self, path):
         """
         Recursively walk through directories.
         """
+        directories, files = self.storage.listdir(path)
+
         for file in files:
             self.process_file(file, path)
 
         for directory in directories:
-            path = path / directory
-            self.process_directory(*self.storage.listdir(path), path)
+            next_path = path / directory
+
+            self.process_directory(next_path)
 
             # Delete empty dirs
-            if not any(self.storage.listdir(path)):
-                self.storage.delete(path)
+            if not any(self.storage.listdir(next_path)):
+                self.storage.delete(next_path)
 
     def handle(self, *args, **options):
         """
         Using the appropriate storage walk through the directories in settings.IMAGEKIT_CACHEFILE_DIR
         For each image file find its source name by removing the hash and settings.IMAGEKIT_CACHEFILE_DIR
         Check if the source exists in media or static if it does continue
         If the source doesn't exist delete the imagekit file, work out the cache key and delete from cache
@@ -73,17 +92,18 @@
             self.stdout.write(
                 "imagekit_cleanup will only work if you use the %s namer."
                 % compatible_namer
             )
             return
 
         self.storage = get_storage_class(settings.IMAGEKIT_DEFAULT_FILE_STORAGE)()
+        self.static_storage = get_storage_class(settings.STATICFILES_STORAGE)()
         self.cache = caches[settings.IMAGEKIT_CACHE_BACKEND]
 
         try:
             path = Path(self.storage.location)
         except AttributeError:
             path = Path("/")
 
         self.root_path = path / settings.IMAGEKIT_CACHEFILE_DIR
 
-        self.process_directory(*self.storage.listdir(self.root_path), self.root_path)
+        self.process_directory(self.root_path)
```

### Comparing `django-lazy-srcset-1.0.1/lazy_srcset/templatetags/lazy_srcset.py` & `django-lazy-srcset-1.0.2/lazy_srcset/templatetags/lazy_srcset.py`

 * *Files identical despite different names*

### Comparing `django-lazy-srcset-1.0.1/setup.cfg` & `django-lazy-srcset-1.0.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-lazy-srcset
-version = 1.0.1
+version = 1.0.2
 description = Lazy srcset and responsive image generation for Django. Minimum effort required. No database required.
 long_description = file:README.rst
 url = https://github.com/Quantra/django-lazy-srcset
 author = Vince Coleman
 author_email = vince@shystudios.co.uk
 license = MIT
 classifiers =
```

