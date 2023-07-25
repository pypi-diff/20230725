# Comparing `tmp/our1314-0.0.8.tar.gz` & `tmp/our1314-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "our1314-0.0.8.tar", last modified: Wed May 18 03:39:49 2022, max compression
+gzip compressed data, was "our1314-0.0.9.tar", last modified: Wed May 18 03:54:07 2022, max compression
```

## Comparing `our1314-0.0.8.tar` & `our1314-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2022-05-18 03:39:49.113183 our1314-0.0.8/
--rw-rw-rw-   0        0        0     1082 2022-05-08 00:45:17.000000 our1314-0.0.8/LICENSE
--rw-rw-rw-   0        0        0        0 2022-05-08 00:17:16.000000 our1314-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0      276 2022-05-18 03:39:49.113183 our1314-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0        0 2022-05-08 00:16:44.000000 our1314-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2022-05-18 03:39:49.097522 our1314-0.0.8/our1314/
--rw-rw-rw-   0        0        0      743 2022-05-18 01:25:22.000000 our1314-0.0.8/our1314/Work.py
--rw-rw-rw-   0        0        0        0 2022-05-08 00:18:26.000000 our1314-0.0.8/our1314/__init__.py
-drwxrwxrwx   0        0        0        0 2022-05-18 03:39:49.113183 our1314-0.0.8/our1314.egg-info/
--rw-rw-rw-   0        0        0      276 2022-05-18 03:39:48.000000 our1314-0.0.8/our1314.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      208 2022-05-18 03:39:48.000000 our1314-0.0.8/our1314.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-05-18 03:39:48.000000 our1314-0.0.8/our1314.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2022-05-18 03:39:48.000000 our1314-0.0.8/our1314.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-05-18 03:39:49.113183 our1314-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      417 2022-05-18 03:39:14.000000 our1314-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-05-18 03:54:07.640294 our1314-0.0.9/
+-rw-rw-rw-   0        0        0     1082 2022-05-08 00:45:17.000000 our1314-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0        0 2022-05-08 00:17:16.000000 our1314-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      276 2022-05-18 03:54:07.640294 our1314-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2022-05-08 00:16:44.000000 our1314-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2022-05-18 03:54:07.609053 our1314-0.0.9/our1314/
+-rw-rw-rw-   0        0        0      644 2022-05-18 03:53:44.000000 our1314-0.0.9/our1314/Work.py
+-rw-rw-rw-   0        0        0        0 2022-05-08 00:18:26.000000 our1314-0.0.9/our1314/__init__.py
+drwxrwxrwx   0        0        0        0 2022-05-18 03:54:07.640294 our1314-0.0.9/our1314.egg-info/
+-rw-rw-rw-   0        0        0      276 2022-05-18 03:54:06.000000 our1314-0.0.9/our1314.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      208 2022-05-18 03:54:07.000000 our1314-0.0.9/our1314.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-05-18 03:54:07.000000 our1314-0.0.9/our1314.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2022-05-18 03:54:07.000000 our1314-0.0.9/our1314.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-05-18 03:54:07.640294 our1314-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      417 2022-05-18 03:53:51.000000 our1314-0.0.9/setup.py
```

### Comparing `our1314-0.0.8/LICENSE` & `our1314-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `our1314-0.0.8/our1314/Work.py` & `our1314-0.0.9/our1314/Work.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 import cv2
 import torch
 import numpy as np
 import torchvision.transforms
 
 
-class Work:
-    def __init__(self):
-        print('Work')
-
-    def torch_tensor2mat(img):
-        if len(img.size()) == 4:
-            img = torch.squeeze(img, 0)  # 删除第0维
-
-        img = torch.permute(img, (1, 2, 0))  # 交换维度
-        img = img.detach().numpy()
-        img = img * 255
-        img = np.uint8(img)
-        img = cv2.cvtColor(img, cv2.COLOR_RGB2BGR)#rgb 转 bgr,否则后续opencv操作会报错
-        return img
+def torch_tensor2mat(img):
+    if len(img.size()) == 4:
+        img = torch.squeeze(img, 0)  # 删除第0维
+
+    img = torch.permute(img, (1, 2, 0))  # 交换维度
+    img = img.detach().numpy()
+    img = img * 255
+    img = np.uint8(img)
+    img = cv2.cvtColor(img, cv2.COLOR_RGB2BGR)#rgb 转 bgr,否则后续opencv操作会报错
+    return img
 
 if __name__ == '__main__':
     img = 128 * np.ones((100,200,3), dtype=np.uint8)
     img = torchvision.transforms.ToTensor()(img)
 
     # Work().torch_tensor2mat(img)
```

