# Comparing `tmp/CaptchaCracker-0.0.6.tar.gz` & `tmp/CaptchaCracker-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CaptchaCracker-0.0.6.tar", last modified: Wed Dec 29 08:49:21 2021, max compression
+gzip compressed data, was "CaptchaCracker-0.0.7.tar", last modified: Tue Jul 25 02:09:51 2023, max compression
```

## Comparing `CaptchaCracker-0.0.6.tar` & `CaptchaCracker-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2021-12-29 08:49:21.834923 CaptchaCracker-0.0.6/
-drwxrwxrwx   0        0        0        0 2021-12-29 08:49:21.775697 CaptchaCracker-0.0.6/CaptchaCracker/
--rw-rw-rw-   0        0        0      312 2021-12-29 08:48:44.000000 CaptchaCracker-0.0.6/CaptchaCracker/__init__.py
--rw-rw-rw-   0        0        0    13721 2021-12-29 08:41:24.000000 CaptchaCracker-0.0.6/CaptchaCracker/core.py
-drwxrwxrwx   0        0        0        0 2021-12-29 08:49:21.831921 CaptchaCracker-0.0.6/CaptchaCracker.egg-info/
--rw-rw-rw-   0        0        0     3962 2021-12-29 08:49:21.000000 CaptchaCracker-0.0.6/CaptchaCracker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      228 2021-12-29 08:49:21.000000 CaptchaCracker-0.0.6/CaptchaCracker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-12-29 08:49:21.000000 CaptchaCracker-0.0.6/CaptchaCracker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2021-12-29 08:49:21.000000 CaptchaCracker-0.0.6/CaptchaCracker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1081 2021-12-16 15:35:21.000000 CaptchaCracker-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     3962 2021-12-29 08:49:21.833924 CaptchaCracker-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     2616 2021-12-24 10:19:05.000000 CaptchaCracker-0.0.6/README.md
--rw-rw-rw-   0        0        0       42 2021-12-29 08:49:21.835924 CaptchaCracker-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      792 2021-12-29 08:48:39.000000 CaptchaCracker-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:09:51.078933 CaptchaCracker-0.0.7/
+drwxrwxrwx   0        0        0        0 2023-07-25 02:09:51.050781 CaptchaCracker-0.0.7/CaptchaCracker/
+-rw-rw-rw-   0        0        0      312 2023-07-25 02:08:57.000000 CaptchaCracker-0.0.7/CaptchaCracker/__init__.py
+-rw-rw-rw-   0        0        0    14002 2023-07-25 02:08:36.000000 CaptchaCracker-0.0.7/CaptchaCracker/core.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:09:51.075941 CaptchaCracker-0.0.7/CaptchaCracker.egg-info/
+-rw-rw-rw-   0        0        0     4256 2023-07-25 02:09:50.000000 CaptchaCracker-0.0.7/CaptchaCracker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      228 2023-07-25 02:09:50.000000 CaptchaCracker-0.0.7/CaptchaCracker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 02:09:50.000000 CaptchaCracker-0.0.7/CaptchaCracker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-07-25 02:09:50.000000 CaptchaCracker-0.0.7/CaptchaCracker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1081 2023-07-25 02:01:55.000000 CaptchaCracker-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     4256 2023-07-25 02:09:51.076942 CaptchaCracker-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3701 2023-07-25 02:01:55.000000 CaptchaCracker-0.0.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-25 02:09:51.078933 CaptchaCracker-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      792 2023-07-25 02:09:13.000000 CaptchaCracker-0.0.7/setup.py
```

### Comparing `CaptchaCracker-0.0.6/CaptchaCracker/core.py` & `CaptchaCracker-0.0.7/CaptchaCracker/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import os
 import glob
 import numpy as np
 
+import io
+from PIL import Image
 from pathlib import Path
 from collections import Counter
 
 import tensorflow as tf
 from tensorflow import keras
 from tensorflow.keras import layers
 
@@ -235,31 +237,37 @@
     
     def predict(self, target_img_path):
         target_img = self.encode_single_sample(target_img_path)['image']
         target_img = tf.reshape(target_img, shape=[1,self.img_width,self.img_height,1])
         pred_val = self.prediction_model.predict(target_img)
         pred = self.decode_batch_predictions(pred_val)[0]
         return pred
-        
+
+    def predict_from_bytes(self, image_bytes):
+        target_img = self.encode_single_sample_from_bytes(image_bytes)['image']
+        target_img = tf.expand_dims(target_img, 0)
+        pred_val = self.prediction_model.predict(target_img)
+        pred = self.decode_batch_predictions(pred_val)[0]
+        return pred
+
     def encode_single_sample(self, img_path):
-        # 1. Read image
         img = tf.io.read_file(img_path)
-        # 2. Decode and convert to grayscale
         img = tf.io.decode_png(img, channels=1)
-        # 3. Convert to float32 in [0, 1] range
         img = tf.image.convert_image_dtype(img, tf.float32)
-        # 4. Resize to the desired size
         img = tf.image.resize(img, [self.img_height, self.img_width])
-        # 5. Transpose the image because we want the time
-        # dimension to correspond to the width of the image.
         img = tf.transpose(img, perm=[1, 0, 2])
-        # 6. Map the characters in label to numbers
-        # 7. Return a dict as our model is expecting two inputs
         return {"image": img}
-    
+
+    def encode_single_sample_from_bytes(self, image_bytes):
+        img = tf.io.decode_image(image_bytes, channels=1)
+        img = tf.image.convert_image_dtype(img, tf.float32)
+        img = tf.image.resize(img, [self.img_height, self.img_width])
+        img = tf.transpose(img, perm=[1, 0, 2])
+        return {"image": img}
+
     def build_model(self):
         # Inputs to the model
         input_img = layers.Input(
             shape=(self.img_width, self.img_height, 1), name="image", dtype="float32"
         )
         labels = layers.Input(name="label", shape=(None,), dtype="float32")
```

### Comparing `CaptchaCracker-0.0.6/LICENSE` & `CaptchaCracker-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `CaptchaCracker-0.0.6/setup.py` & `CaptchaCracker-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="CaptchaCracker",
-    version="0.0.6",
+    version="0.0.7",
     license='MIT',
     author="Wooil Jeong",
     author_email="wooil@kakao.com",
     description="CaptchaCracker is an open source Python library that provides functions to create and apply deep learning models for Captcha Image recognition.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/WooilJeong/CaptchaCracker",
```

