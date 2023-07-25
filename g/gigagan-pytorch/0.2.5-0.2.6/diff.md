# Comparing `tmp/gigagan-pytorch-0.2.5.tar.gz` & `tmp/gigagan-pytorch-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gigagan-pytorch-0.2.5.tar", last modified: Mon Jul 24 16:41:33 2023, max compression
+gzip compressed data, was "gigagan-pytorch-0.2.6.tar", last modified: Tue Jul 25 00:13:11 2023, max compression
```

## Comparing `gigagan-pytorch-0.2.5.tar` & `gigagan-pytorch-0.2.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:41:33.611274 gigagan-pytorch-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-24 16:41:19.000000 gigagan-pytorch-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-24 16:41:33.611274 gigagan-pytorch-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9503 2023-07-24 16:41:19.000000 gigagan-pytorch-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:41:33.611274 gigagan-pytorch-0.2.5/gigagan_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-24 16:41:19.000000 gigagan-pytorch-0.2.5/gigagan_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-07-24 16:41:19.000000 gigagan-pytorch-0.2.5/gigagan_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-07-24 16:41:19.000000 gigagan-pytorch-0.2.5/gigagan_pytorch/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    83641 2023-07-24 16:41:19.000000 gigagan-pytorch-0.2.5/gigagan_pytorch/gigagan_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-07-24 16:41:19.000000 gigagan-pytorch-0.2.5/gigagan_pytorch/open_clip.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-24 16:41:19.000000 gigagan-pytorch-0.2.5/gigagan_pytorch/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    18189 2023-07-24 16:41:19.000000 gigagan-pytorch-0.2.5/gigagan_pytorch/unet_upsampler.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 16:41:19.000000 gigagan-pytorch-0.2.5/gigagan_pytorch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:41:33.611274 gigagan-pytorch-0.2.5/gigagan_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-24 16:41:33.000000 gigagan-pytorch-0.2.5/gigagan_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-24 16:41:33.000000 gigagan-pytorch-0.2.5/gigagan_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 16:41:33.000000 gigagan-pytorch-0.2.5/gigagan_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-24 16:41:33.000000 gigagan-pytorch-0.2.5/gigagan_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-24 16:41:33.000000 gigagan-pytorch-0.2.5/gigagan_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-24 16:41:19.000000 gigagan-pytorch-0.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 16:41:33.611274 gigagan-pytorch-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-24 16:41:19.000000 gigagan-pytorch-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:13:11.577897 gigagan-pytorch-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-25 00:12:58.000000 gigagan-pytorch-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-25 00:13:11.577897 gigagan-pytorch-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9503 2023-07-25 00:12:58.000000 gigagan-pytorch-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:13:11.573897 gigagan-pytorch-0.2.6/gigagan_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-25 00:12:58.000000 gigagan-pytorch-0.2.6/gigagan_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-07-25 00:12:58.000000 gigagan-pytorch-0.2.6/gigagan_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-07-25 00:12:58.000000 gigagan-pytorch-0.2.6/gigagan_pytorch/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83976 2023-07-25 00:12:58.000000 gigagan-pytorch-0.2.6/gigagan_pytorch/gigagan_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-07-25 00:12:58.000000 gigagan-pytorch-0.2.6/gigagan_pytorch/open_clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-25 00:12:58.000000 gigagan-pytorch-0.2.6/gigagan_pytorch/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18497 2023-07-25 00:12:58.000000 gigagan-pytorch-0.2.6/gigagan_pytorch/unet_upsampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-25 00:12:58.000000 gigagan-pytorch-0.2.6/gigagan_pytorch/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:13:11.577897 gigagan-pytorch-0.2.6/gigagan_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-25 00:13:11.000000 gigagan-pytorch-0.2.6/gigagan_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-25 00:13:11.000000 gigagan-pytorch-0.2.6/gigagan_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 00:13:11.000000 gigagan-pytorch-0.2.6/gigagan_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-25 00:13:11.000000 gigagan-pytorch-0.2.6/gigagan_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-25 00:13:11.000000 gigagan-pytorch-0.2.6/gigagan_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-25 00:12:58.000000 gigagan-pytorch-0.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 00:13:11.577897 gigagan-pytorch-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-25 00:12:58.000000 gigagan-pytorch-0.2.6/setup.py
```

### Comparing `gigagan-pytorch-0.2.5/LICENSE` & `gigagan-pytorch-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.2.5/PKG-INFO` & `gigagan-pytorch-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gigagan-pytorch
-Version: 0.2.5
+Version: 0.2.6
 Summary: GigaGAN - Pytorch
 Home-page: https://github.com/lucidrains/ETSformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,generative adversarial networks
 Classifier: Development Status :: 4 - Beta
```

### Comparing `gigagan-pytorch-0.2.5/README.md` & `gigagan-pytorch-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.2.5/gigagan_pytorch/__init__.py` & `gigagan-pytorch-0.2.6/gigagan_pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.2.5/gigagan_pytorch/attend.py` & `gigagan-pytorch-0.2.6/gigagan_pytorch/attend.py`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.2.5/gigagan_pytorch/data.py` & `gigagan-pytorch-0.2.6/gigagan_pytorch/data.py`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.2.5/gigagan_pytorch/gigagan_pytorch.py` & `gigagan-pytorch-0.2.6/gigagan_pytorch/gigagan_pytorch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1610,14 +1610,15 @@
 
         else:
             assert not any([*map(exists, (texts, text_embeds))])
 
         x = images
 
         image_size = (self.image_size, self.image_size)
+
         assert x.shape[-2:] == image_size
 
         batch = x.shape[0]
 
         # index the rgbs by resolution
 
         rgbs_index = {t.shape[-1]: t for t in rgbs} if exists(rgbs) else {}
@@ -1830,14 +1831,19 @@
 
         # use _base to designate unwrapped models
 
         self.G = generator
         self.D = discriminator
         self.VD = vision_aided_discriminator
 
+        # validate multiscale input resolutions
+
+        if train_upsampler:
+            assert is_empty(set(discriminator.multiscale_input_resolutions) - set(generator.allowable_rgb_resolutions)), f'only multiscale input resolutions of {generator.allowable_rgb_resolutions} is allowed based on the unet input and output image size'
+
         # ema
 
         self.has_ema_generator = False
 
         if self.is_main and create_ema_generator_at_init:
             self.create_ema_generator()
```

### Comparing `gigagan-pytorch-0.2.5/gigagan_pytorch/open_clip.py` & `gigagan-pytorch-0.2.6/gigagan_pytorch/open_clip.py`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.2.5/gigagan_pytorch/optimizer.py` & `gigagan-pytorch-0.2.6/gigagan_pytorch/optimizer.py`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.2.5/gigagan_pytorch/unet_upsampler.py` & `gigagan-pytorch-0.2.6/gigagan_pytorch/unet_upsampler.py`

 * *Files 2% similar despite different names*

```diff
@@ -446,14 +446,21 @@
 
         # determine the projection of the style embedding to convolutional modulation weights (+ adaptive kernel selection weights) for all layers
 
         self.style_to_conv_modulations = nn.Linear(style_network.dim, sum(style_embed_split_dims))
         self.style_embed_split_dims = style_embed_split_dims
 
     @property
+    def allowable_rgb_resolutions(self):
+        input_res_base = int(log2(self.input_image_size))
+        output_res_base = int(log2(self.image_size))
+        allowed_rgb_res_base = list(range(input_res_base + 1, output_res_base))
+        return [*map(lambda p: 2 ** p, allowed_rgb_res_base)]
+
+    @property
     def device(self):
         return next(self.parameters()).device
 
     @property
     def total_params(self):
         return sum([p.numel() for p in self.parameters()])
 
@@ -580,15 +587,15 @@
         rgb = rgb + self.final_to_rgb(x)
 
         if not return_all_rgbs:
             return rgb
 
         # only keep those rgbs whose feature map is greater than the input image to be upsampled
 
-        rgbs = list(filter(lambda t: t.shape[-1] <= shape[-1], rgbs))
+        rgbs = list(filter(lambda t: t.shape[-1] > shape[-1], rgbs))
 
         if not replace_rgb_with_input_lowres_image:
             return rgb, rgbs
 
         # replace the rgb of the corresponding same dimension as the input low res image
 
         output_rgbs = []
```

### Comparing `gigagan-pytorch-0.2.5/gigagan_pytorch.egg-info/PKG-INFO` & `gigagan-pytorch-0.2.6/gigagan_pytorch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gigagan-pytorch
-Version: 0.2.5
+Version: 0.2.6
 Summary: GigaGAN - Pytorch
 Home-page: https://github.com/lucidrains/ETSformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,generative adversarial networks
 Classifier: Development Status :: 4 - Beta
```

### Comparing `gigagan-pytorch-0.2.5/setup.py` & `gigagan-pytorch-0.2.6/setup.py`

 * *Files identical despite different names*

