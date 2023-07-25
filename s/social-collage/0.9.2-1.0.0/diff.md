# Comparing `tmp/social_collage-0.9.2.tar.gz` & `tmp/social_collage-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "social_collage-0.9.2.tar", last modified: Tue Jul 25 17:47:32 2023, max compression
+gzip compressed data, was "social_collage-1.0.0.tar", last modified: Tue Jul 25 19:34:26 2023, max compression
```

## Comparing `social_collage-0.9.2.tar` & `social_collage-1.0.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 meequz    (1000) meequz    (1000)        0 2023-07-25 17:47:32.711550 social_collage-0.9.2/
--rw-rw-r--   0 meequz    (1000) meequz    (1000)      284 2023-07-25 17:46:54.000000 social_collage-0.9.2/MANIFEST.in
--rw-rw-r--   0 meequz    (1000) meequz    (1000)      795 2023-07-25 17:47:32.711550 social_collage-0.9.2/PKG-INFO
--rw-rw-r--   0 meequz    (1000) meequz    (1000)       16 2023-07-24 16:41:59.000000 social_collage-0.9.2/README.md
--rw-rw-r--   0 meequz    (1000) meequz    (1000)       18 2023-07-25 15:36:36.000000 social_collage-0.9.2/requirements.txt
--rw-rw-r--   0 meequz    (1000) meequz    (1000)       38 2023-07-25 17:47:32.711550 social_collage-0.9.2/setup.cfg
--rw-rw-r--   0 meequz    (1000) meequz    (1000)     1047 2023-07-25 17:47:10.000000 social_collage-0.9.2/setup.py
-drwxrwxr-x   0 meequz    (1000) meequz    (1000)        0 2023-07-25 17:47:32.699550 social_collage-0.9.2/social_collage/
--rw-rw-r--   0 meequz    (1000) meequz    (1000)     5069 2023-07-25 17:47:14.000000 social_collage-0.9.2/social_collage/__init__.py
--rw-rw-r--   0 meequz    (1000) meequz    (1000)      473 2023-07-25 15:23:51.000000 social_collage-0.9.2/social_collage/example.py
-drwxrwxr-x   0 meequz    (1000) meequz    (1000)        0 2023-07-25 17:47:32.707550 social_collage-0.9.2/social_collage/example_images/
--rw-rw-r--   0 meequz    (1000) meequz    (1000)   331923 2023-07-25 15:08:59.000000 social_collage-0.9.2/social_collage/example_images/00.jpg
--rw-rw-r--   0 meequz    (1000) meequz    (1000)   369043 2023-07-25 15:09:28.000000 social_collage-0.9.2/social_collage/example_images/01.jpg
--rw-rw-r--   0 meequz    (1000) meequz    (1000)   303748 2023-07-25 15:09:31.000000 social_collage-0.9.2/social_collage/example_images/02.jpg
--rw-rw-r--   0 meequz    (1000) meequz    (1000)   614614 2023-07-25 15:21:11.000000 social_collage-0.9.2/social_collage/example_images/03.jpg
--rw-rw-r--   0 meequz    (1000) meequz    (1000)   364729 2023-07-25 15:09:37.000000 social_collage-0.9.2/social_collage/example_images/04.jpg
-drwxrwxr-x   0 meequz    (1000) meequz    (1000)        0 2023-07-25 17:47:32.703550 social_collage-0.9.2/social_collage.egg-info/
--rw-rw-r--   0 meequz    (1000) meequz    (1000)      795 2023-07-25 17:47:32.000000 social_collage-0.9.2/social_collage.egg-info/PKG-INFO
--rw-rw-r--   0 meequz    (1000) meequz    (1000)      474 2023-07-25 17:47:32.000000 social_collage-0.9.2/social_collage.egg-info/SOURCES.txt
--rw-rw-r--   0 meequz    (1000) meequz    (1000)        1 2023-07-25 17:47:32.000000 social_collage-0.9.2/social_collage.egg-info/dependency_links.txt
--rw-rw-r--   0 meequz    (1000) meequz    (1000)        7 2023-07-25 17:47:32.000000 social_collage-0.9.2/social_collage.egg-info/requires.txt
--rw-rw-r--   0 meequz    (1000) meequz    (1000)       15 2023-07-25 17:47:32.000000 social_collage-0.9.2/social_collage.egg-info/top_level.txt
+drwxrwxr-x   0 meequz    (1000) meequz    (1000)        0 2023-07-25 19:34:26.935811 social_collage-1.0.0/
+-rw-rw-r--   0 meequz    (1000) meequz    (1000)     1073 2023-07-25 19:26:36.000000 social_collage-1.0.0/LICENSE
+-rw-rw-r--   0 meequz    (1000) meequz    (1000)      103 2023-07-25 18:16:33.000000 social_collage-1.0.0/MANIFEST.in
+-rw-rw-r--   0 meequz    (1000) meequz    (1000)     2880 2023-07-25 19:34:26.935811 social_collage-1.0.0/PKG-INFO
+-rw-rw-r--   0 meequz    (1000) meequz    (1000)     2079 2023-07-25 19:31:25.000000 social_collage-1.0.0/README.md
+-rw-rw-r--   0 meequz    (1000) meequz    (1000)       18 2023-07-25 15:36:36.000000 social_collage-1.0.0/requirements.txt
+-rw-rw-r--   0 meequz    (1000) meequz    (1000)       38 2023-07-25 19:34:26.935811 social_collage-1.0.0/setup.cfg
+-rw-rw-r--   0 meequz    (1000) meequz    (1000)     1277 2023-07-25 19:19:30.000000 social_collage-1.0.0/setup.py
+drwxrwxr-x   0 meequz    (1000) meequz    (1000)        0 2023-07-25 19:34:26.927811 social_collage-1.0.0/social_collage/
+-rw-rw-r--   0 meequz    (1000) meequz    (1000)     5545 2023-07-25 19:19:36.000000 social_collage-1.0.0/social_collage/__init__.py
+drwxrwxr-x   0 meequz    (1000) meequz    (1000)        0 2023-07-25 19:34:26.935811 social_collage-1.0.0/social_collage/example_images/
+-rw-rw-r--   0 meequz    (1000) meequz    (1000)   331923 2023-07-25 15:08:59.000000 social_collage-1.0.0/social_collage/example_images/00.jpg
+-rw-rw-r--   0 meequz    (1000) meequz    (1000)   369043 2023-07-25 15:09:28.000000 social_collage-1.0.0/social_collage/example_images/01.jpg
+-rw-rw-r--   0 meequz    (1000) meequz    (1000)   303748 2023-07-25 15:09:31.000000 social_collage-1.0.0/social_collage/example_images/02.jpg
+-rw-rw-r--   0 meequz    (1000) meequz    (1000)   614614 2023-07-25 15:21:11.000000 social_collage-1.0.0/social_collage/example_images/03.jpg
+-rw-rw-r--   0 meequz    (1000) meequz    (1000)   364729 2023-07-25 15:09:37.000000 social_collage-1.0.0/social_collage/example_images/04.jpg
+drwxrwxr-x   0 meequz    (1000) meequz    (1000)        0 2023-07-25 19:34:26.927811 social_collage-1.0.0/social_collage.egg-info/
+-rw-rw-r--   0 meequz    (1000) meequz    (1000)     2880 2023-07-25 19:34:26.000000 social_collage-1.0.0/social_collage.egg-info/PKG-INFO
+-rw-rw-r--   0 meequz    (1000) meequz    (1000)      456 2023-07-25 19:34:26.000000 social_collage-1.0.0/social_collage.egg-info/SOURCES.txt
+-rw-rw-r--   0 meequz    (1000) meequz    (1000)        1 2023-07-25 19:34:26.000000 social_collage-1.0.0/social_collage.egg-info/dependency_links.txt
+-rw-rw-r--   0 meequz    (1000) meequz    (1000)        7 2023-07-25 19:34:26.000000 social_collage-1.0.0/social_collage.egg-info/requires.txt
+-rw-rw-r--   0 meequz    (1000) meequz    (1000)       15 2023-07-25 19:34:26.000000 social_collage-1.0.0/social_collage.egg-info/top_level.txt
```

### Comparing `social_collage-0.9.2/setup.py` & `social_collage-1.0.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 
 with open('README.md') as f:
     long_description = f.read()
 
 
 setup(
     name='social_collage',
-    version='0.9.2',
+    version='1.0.0',
     packages=['social_collage'],
+    package_data={'social_collage': ['example_images/*.jpg']},
     description='Create image collages in social networks style',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/meequz/social_collage',
     author='Mikhail Varantsou',
     license='MIT',
     author_email='meequz@gmail.com',
@@ -28,7 +29,12 @@
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
     ],
     python_requires='>=3.6',
 )
+
+# Publish new version:
+# - change version in __init__.py and in setup.py, commit
+# - run 'python setup.py sdist'
+# - run 'twine upload dist/social_collage-{}.tar.gz'
```

### Comparing `social_collage-0.9.2/social_collage/__init__.py` & `social_collage-1.0.0/social_collage/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,14 @@
+import glob
+from pathlib import Path
+
 from PIL import Image
 
 
-__version__ = '0.9.2'
+__version__ = '1.0.0'
 __author__ = 'Mikhail Varantsou'
 
 
 BG_COLOR = (255, 255, 255, 255)
 SPACE_SHARE = 150
 
 
@@ -23,15 +26,15 @@
         height = imwidth / ratio
         indent = (imheight - height) / 2
         return img.crop((0, int(indent), imwidth, int(height + indent)))
 
 
 def _prepare_imgs(images, length):
     if len(images) < length:
-        raise ValueError(f'Not enough images, have to be {length}')
+        raise ValueError(f'Provided {len(images)} images, have to be {length}')
 
     converted = [img.convert(mode='RGBA') for img in images]
     return converted
 
 
 def _calc_space(width, spaceshare):
     if spaceshare:
@@ -161,7 +164,21 @@
     clg = _new_collage(total_w, total_h, bgcolor, crimg0, space)
     clg.paste(crimg1, (space, crimg0_h + space * 2))
     clg.paste(crimg2, (btm_img_w + space * 2, crimg0_h + space * 2))
     clg.paste(crimg3, (space, crimg0_h + btm_img_h + space * 3))
     clg.paste(crimg4, (btm_img_w + space * 2, crimg0_h + btm_img_h + space * 3))
 
     return clg
+
+
+def example():
+    # Read image files into a list of PIL objects
+    dirc = Path(__file__).resolve(strict=True).parent / 'example_images'
+    imgs = []
+    for imgpath in sorted(glob.glob(str(dirc / '*.jpg'))):
+        imgs.append(Image.open(imgpath))
+
+    # Send list of PIL images to a collage function
+    collage = collage_5_1(imgs)
+
+    # Show the returned PIL image containing the resulting collage
+    collage.show()
```

### Comparing `social_collage-0.9.2/social_collage/example_images/00.jpg` & `social_collage-1.0.0/social_collage/example_images/00.jpg`

 * *Files identical despite different names*

### Comparing `social_collage-0.9.2/social_collage/example_images/01.jpg` & `social_collage-1.0.0/social_collage/example_images/01.jpg`

 * *Files identical despite different names*

### Comparing `social_collage-0.9.2/social_collage/example_images/02.jpg` & `social_collage-1.0.0/social_collage/example_images/02.jpg`

 * *Files identical despite different names*

### Comparing `social_collage-0.9.2/social_collage/example_images/03.jpg` & `social_collage-1.0.0/social_collage/example_images/03.jpg`

 * *Files identical despite different names*

### Comparing `social_collage-0.9.2/social_collage/example_images/04.jpg` & `social_collage-1.0.0/social_collage/example_images/04.jpg`

 * *Files identical despite different names*

