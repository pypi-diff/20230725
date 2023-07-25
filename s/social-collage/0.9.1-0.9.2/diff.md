# Comparing `tmp/social_collage-0.9.1.tar.gz` & `tmp/social_collage-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "social_collage-0.9.1.tar", last modified: Tue Jul 25 17:44:23 2023, max compression
+gzip compressed data, was "social_collage-0.9.2.tar", last modified: Tue Jul 25 17:47:32 2023, max compression
```

## Comparing `social_collage-0.9.1.tar` & `social_collage-0.9.2.tar`

### file list

```diff
@@ -1,16 +1,22 @@
-drwxrwxr-x   0 meequz    (1000) meequz    (1000)        0 2023-07-25 17:44:23.218991 social_collage-0.9.1/
--rw-rw-r--   0 meequz    (1000) meequz    (1000)      209 2023-07-25 17:43:16.000000 social_collage-0.9.1/MANIFEST.in
--rw-rw-r--   0 meequz    (1000) meequz    (1000)      795 2023-07-25 17:44:23.218991 social_collage-0.9.1/PKG-INFO
--rw-rw-r--   0 meequz    (1000) meequz    (1000)       16 2023-07-24 16:41:59.000000 social_collage-0.9.1/README.md
--rw-rw-r--   0 meequz    (1000) meequz    (1000)       18 2023-07-25 15:36:36.000000 social_collage-0.9.1/requirements.txt
--rw-rw-r--   0 meequz    (1000) meequz    (1000)       38 2023-07-25 17:44:23.218991 social_collage-0.9.1/setup.cfg
--rw-rw-r--   0 meequz    (1000) meequz    (1000)     1047 2023-07-25 17:44:17.000000 social_collage-0.9.1/setup.py
-drwxrwxr-x   0 meequz    (1000) meequz    (1000)        0 2023-07-25 17:44:23.214991 social_collage-0.9.1/social_collage/
--rw-rw-r--   0 meequz    (1000) meequz    (1000)     5069 2023-07-25 17:44:19.000000 social_collage-0.9.1/social_collage/__init__.py
--rw-rw-r--   0 meequz    (1000) meequz    (1000)      473 2023-07-25 15:23:51.000000 social_collage-0.9.1/social_collage/example.py
-drwxrwxr-x   0 meequz    (1000) meequz    (1000)        0 2023-07-25 17:44:23.218991 social_collage-0.9.1/social_collage.egg-info/
--rw-rw-r--   0 meequz    (1000) meequz    (1000)      795 2023-07-25 17:44:23.000000 social_collage-0.9.1/social_collage.egg-info/PKG-INFO
--rw-rw-r--   0 meequz    (1000) meequz    (1000)      289 2023-07-25 17:44:23.000000 social_collage-0.9.1/social_collage.egg-info/SOURCES.txt
--rw-rw-r--   0 meequz    (1000) meequz    (1000)        1 2023-07-25 17:44:23.000000 social_collage-0.9.1/social_collage.egg-info/dependency_links.txt
--rw-rw-r--   0 meequz    (1000) meequz    (1000)        7 2023-07-25 17:44:23.000000 social_collage-0.9.1/social_collage.egg-info/requires.txt
--rw-rw-r--   0 meequz    (1000) meequz    (1000)       15 2023-07-25 17:44:23.000000 social_collage-0.9.1/social_collage.egg-info/top_level.txt
+drwxrwxr-x   0 meequz    (1000) meequz    (1000)        0 2023-07-25 17:47:32.711550 social_collage-0.9.2/
+-rw-rw-r--   0 meequz    (1000) meequz    (1000)      284 2023-07-25 17:46:54.000000 social_collage-0.9.2/MANIFEST.in
+-rw-rw-r--   0 meequz    (1000) meequz    (1000)      795 2023-07-25 17:47:32.711550 social_collage-0.9.2/PKG-INFO
+-rw-rw-r--   0 meequz    (1000) meequz    (1000)       16 2023-07-24 16:41:59.000000 social_collage-0.9.2/README.md
+-rw-rw-r--   0 meequz    (1000) meequz    (1000)       18 2023-07-25 15:36:36.000000 social_collage-0.9.2/requirements.txt
+-rw-rw-r--   0 meequz    (1000) meequz    (1000)       38 2023-07-25 17:47:32.711550 social_collage-0.9.2/setup.cfg
+-rw-rw-r--   0 meequz    (1000) meequz    (1000)     1047 2023-07-25 17:47:10.000000 social_collage-0.9.2/setup.py
+drwxrwxr-x   0 meequz    (1000) meequz    (1000)        0 2023-07-25 17:47:32.699550 social_collage-0.9.2/social_collage/
+-rw-rw-r--   0 meequz    (1000) meequz    (1000)     5069 2023-07-25 17:47:14.000000 social_collage-0.9.2/social_collage/__init__.py
+-rw-rw-r--   0 meequz    (1000) meequz    (1000)      473 2023-07-25 15:23:51.000000 social_collage-0.9.2/social_collage/example.py
+drwxrwxr-x   0 meequz    (1000) meequz    (1000)        0 2023-07-25 17:47:32.707550 social_collage-0.9.2/social_collage/example_images/
+-rw-rw-r--   0 meequz    (1000) meequz    (1000)   331923 2023-07-25 15:08:59.000000 social_collage-0.9.2/social_collage/example_images/00.jpg
+-rw-rw-r--   0 meequz    (1000) meequz    (1000)   369043 2023-07-25 15:09:28.000000 social_collage-0.9.2/social_collage/example_images/01.jpg
+-rw-rw-r--   0 meequz    (1000) meequz    (1000)   303748 2023-07-25 15:09:31.000000 social_collage-0.9.2/social_collage/example_images/02.jpg
+-rw-rw-r--   0 meequz    (1000) meequz    (1000)   614614 2023-07-25 15:21:11.000000 social_collage-0.9.2/social_collage/example_images/03.jpg
+-rw-rw-r--   0 meequz    (1000) meequz    (1000)   364729 2023-07-25 15:09:37.000000 social_collage-0.9.2/social_collage/example_images/04.jpg
+drwxrwxr-x   0 meequz    (1000) meequz    (1000)        0 2023-07-25 17:47:32.703550 social_collage-0.9.2/social_collage.egg-info/
+-rw-rw-r--   0 meequz    (1000) meequz    (1000)      795 2023-07-25 17:47:32.000000 social_collage-0.9.2/social_collage.egg-info/PKG-INFO
+-rw-rw-r--   0 meequz    (1000) meequz    (1000)      474 2023-07-25 17:47:32.000000 social_collage-0.9.2/social_collage.egg-info/SOURCES.txt
+-rw-rw-r--   0 meequz    (1000) meequz    (1000)        1 2023-07-25 17:47:32.000000 social_collage-0.9.2/social_collage.egg-info/dependency_links.txt
+-rw-rw-r--   0 meequz    (1000) meequz    (1000)        7 2023-07-25 17:47:32.000000 social_collage-0.9.2/social_collage.egg-info/requires.txt
+-rw-rw-r--   0 meequz    (1000) meequz    (1000)       15 2023-07-25 17:47:32.000000 social_collage-0.9.2/social_collage.egg-info/top_level.txt
```

### Comparing `social_collage-0.9.1/PKG-INFO` & `social_collage-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: social_collage
-Version: 0.9.1
+Version: 0.9.2
 Summary: Create image collages in social networks style
 Home-page: https://github.com/meequz/social_collage
 Author: Mikhail Varantsou
 Author-email: meequz@gmail.com
 License: MIT
 Keywords: collage
 Platform: UNKNOWN
```

### Comparing `social_collage-0.9.1/setup.py` & `social_collage-0.9.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 with open('README.md') as f:
     long_description = f.read()
 
 
 setup(
     name='social_collage',
-    version='0.9.1',
+    version='0.9.2',
     packages=['social_collage'],
     description='Create image collages in social networks style',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/meequz/social_collage',
     author='Mikhail Varantsou',
     license='MIT',
```

### Comparing `social_collage-0.9.1/social_collage/__init__.py` & `social_collage-0.9.2/social_collage/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from PIL import Image
 
 
-__version__ = '0.9.1'
+__version__ = '0.9.2'
 __author__ = 'Mikhail Varantsou'
 
 
 BG_COLOR = (255, 255, 255, 255)
 SPACE_SHARE = 150
```

### Comparing `social_collage-0.9.1/social_collage.egg-info/PKG-INFO` & `social_collage-0.9.2/social_collage.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: social-collage
-Version: 0.9.1
+Version: 0.9.2
 Summary: Create image collages in social networks style
 Home-page: https://github.com/meequz/social_collage
 Author: Mikhail Varantsou
 Author-email: meequz@gmail.com
 License: MIT
 Keywords: collage
 Platform: UNKNOWN
```

