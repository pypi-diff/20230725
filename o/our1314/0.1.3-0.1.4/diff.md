# Comparing `tmp/our1314-0.1.3.tar.gz` & `tmp/our1314-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "our1314-0.1.3.tar", last modified: Tue Jul 25 03:10:00 2023, max compression
+gzip compressed data, was "our1314-0.1.4.tar", last modified: Tue Jul 25 06:03:52 2023, max compression
```

## Comparing `our1314-0.1.3.tar` & `our1314-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 03:10:00.683952 our1314-0.1.3/
--rw-rw-rw-   0        0        0     1082 2023-07-25 01:35:24.000000 our1314-0.1.3/LICENSE
--rw-rw-rw-   0        0        0      263 2023-07-25 03:10:00.683952 our1314-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0       39 2023-07-25 01:35:24.000000 our1314-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-25 03:10:00.669953 our1314-0.1.3/our1314/
--rw-rw-rw-   0        0        0        0 2023-07-25 02:10:04.000000 our1314-0.1.3/our1314/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 03:10:00.683952 our1314-0.1.3/our1314/myutils/
--rw-rw-rw-   0        0        0        0 2023-07-25 02:10:04.000000 our1314-0.1.3/our1314/myutils/__init__.py
--rw-rw-rw-   0        0        0     1430 2023-07-10 10:51:17.000000 our1314-0.1.3/our1314/myutils/exportsd.py
--rw-rw-rw-   0        0        0     2370 2023-07-10 10:51:17.000000 our1314-0.1.3/our1314/myutils/importsd.py
--rw-rw-rw-   0        0        0     5665 2023-07-25 01:36:14.000000 our1314-0.1.3/our1314/myutils/myutils.py
-drwxrwxrwx   0        0        0        0 2023-07-25 03:10:00.681952 our1314-0.1.3/our1314.egg-info/
--rw-rw-rw-   0        0        0      263 2023-07-25 03:10:00.000000 our1314-0.1.3/our1314.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      281 2023-07-25 03:10:00.000000 our1314-0.1.3/our1314.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 03:10:00.000000 our1314-0.1.3/our1314.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-25 03:10:00.000000 our1314-0.1.3/our1314.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-25 03:10:00.684953 our1314-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      417 2023-07-25 03:08:47.000000 our1314-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 06:03:52.151418 our1314-0.1.4/
+-rw-rw-rw-   0        0        0     1082 2023-07-25 01:35:24.000000 our1314-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0      263 2023-07-25 06:03:52.150417 our1314-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0       39 2023-07-25 01:35:24.000000 our1314-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 06:03:52.124415 our1314-0.1.4/our1314/
+-rw-rw-rw-   0        0        0        0 2023-07-25 02:10:04.000000 our1314-0.1.4/our1314/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 06:03:52.149416 our1314-0.1.4/our1314/myutils/
+-rw-rw-rw-   0        0        0        0 2023-07-25 02:10:04.000000 our1314-0.1.4/our1314/myutils/__init__.py
+-rw-rw-rw-   0        0        0     1430 2023-07-10 10:51:17.000000 our1314-0.1.4/our1314/myutils/exportsd.py
+-rw-rw-rw-   0        0        0     2370 2023-07-10 10:51:17.000000 our1314-0.1.4/our1314/myutils/importsd.py
+-rw-rw-rw-   0        0        0     5426 2023-07-25 05:56:11.000000 our1314-0.1.4/our1314/myutils/myutils.py
+drwxrwxrwx   0        0        0        0 2023-07-25 06:03:52.137415 our1314-0.1.4/our1314.egg-info/
+-rw-rw-rw-   0        0        0      263 2023-07-25 06:03:52.000000 our1314-0.1.4/our1314.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      281 2023-07-25 06:03:52.000000 our1314-0.1.4/our1314.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 06:03:52.000000 our1314-0.1.4/our1314.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-25 06:03:52.000000 our1314-0.1.4/our1314.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-25 06:03:52.151418 our1314-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      417 2023-07-25 06:02:46.000000 our1314-0.1.4/setup.py
```

### Comparing `our1314-0.1.3/LICENSE` & `our1314-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `our1314-0.1.3/our1314/myutils/exportsd.py` & `our1314-0.1.4/our1314/myutils/exportsd.py`

 * *Files identical despite different names*

### Comparing `our1314-0.1.3/our1314/myutils/importsd.py` & `our1314-0.1.4/our1314/myutils/importsd.py`

 * *Files identical despite different names*

### Comparing `our1314-0.1.3/our1314/myutils/myutils.py` & `our1314-0.1.4/our1314/myutils/myutils.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,26 +2,27 @@
 import os
 import cv2
 import numpy as np
 import torch
 import torchvision
 from PIL import Image
 from torch.nn import Module
+from math import *
 import halcon
+from halcon.numpy_interop import himage_from_numpy_array, himage_as_numpy_array
+
 
 def pil2mat(image):
     mat = cv2.cvtColor(np.asarray(image), cv2.COLOR_RGB2BGR)
     return mat
 
-
 def mat2pil(mat):
     image = Image.fromarray(cv2.cvtColor(mat, cv2.COLOR_BGR2RGB))
     return image
 
-
 def tensor2mat(data, dtype=np.uint8):
     """
     将给定的张量转换为Mat
     :param data:张量,三个维度，[c,h,w]
     :param dtype:模板数据类型，默认np.uint8
     :return:OpenCV Mat，三个维度，[h,w,c]
     """
@@ -34,20 +35,18 @@
     img = img.copy()  # 没有这句会报错：Layout of the output array img is incompatible with cv::Mat
     img *= 255
     img = img.astype(np.uint8)
     img = np.transpose(img, (1, 2, 0))  # c,h,w → h,w,c
     img = img.copy()
     return img
 
-
 def mat2tensor(mat, dtype=np.uint8):
     tensor = torchvision.transforms.ToTensor()(mat)
     return tensor
 
-
 def drawgrid(img, size, color=(0, 0, 255), linewidth=2):
     """
     在图像上绘制指定格式的网络线
     :param img:
     :param size:
     :param color:
     :param linewidth:
@@ -76,15 +75,14 @@
         _p1, _p2 = p1[i], p2[i]  # type:np.ndarray
         _p1 = _p1.astype(np.int)
         _p2 = _p2.astype(np.int)
         cv2.line(img, _p1, _p2, color)
 
     return img
 
-
 def rectangle(img, center, wh, color, thickness):
     """
     给定中心和宽高绘制矩阵
     :param img:
     :param center:
     :param wh:
     :param color:
@@ -93,16 +91,14 @@
     """
     pt1 = center - wh / 2.0  # type: np.ndarray
     pt2 = center + wh / 2.0  # type: np.ndarray
     pt1 = pt1.astype(np.int)
     pt2 = pt2.astype(np.int)
     cv2.rectangle(img, pt1, pt2, color, thickness)
     return img
-
-
 # 按比例将长边缩放至目标尺寸
 class Resize3:
     def __init__(self, width):
         # self.resize = torchvision.transforms.Resize()
         self.width = width
 
     def __call__(self, x):
@@ -158,40 +154,34 @@
         a = s.split(' ')
         a = [f.strip() for f in a]
         a = [f for f in a if f != ""]
         data.append((int(a[0]), float(a[1]), float(a[2]), float(a[3]), float(a[4])))
     return data
 
 def ndarray2hobject(mat):
-    himg=[]
-    h,w,ch = mat.shape
-    if ch==1:
-        himg = halcon.gen_image1(type='byte', width=w, height=h, pixel_pointer=mat.data)
-    elif ch==3:
-        b,g,r=mat[:,:,0],mat[:,:,1],mat[:,:,2]
-        himg = halcon.gen_image3(type='byte', width=w, height=h, pixel_pointer_red=r, pixel_pointer_green=g, pixel_pointer_blue=b)
-    return himg
+    return himage_from_numpy_array(mat)
 
 def hobject2ndarray(hobj):
-    channels = halcon.count_channels(hobj)
-    if channels==1:
-        p, type, w, h = halcon.get_image_pointer1(hobj)
+    return himage_as_numpy_array(hobj)
 
+def deg(rad):
+    return rad*180/pi
 
+def rad(deg):
+    return deg*180/pi
 
 
 if __name__ == '__main__':
     # a = getlastfile('D:/work/proj/xray/test_learn_python/image_classification/cnn_imgcls/run/train/oqa_agl/weights', '.pth')
     # x = torch.rand((1, 3, 110, 310))
     # x = Resize3(330)(x)
     # x = PadSquare()(x)
     
     # resize = torchvision.transforms.Resize((100, 100))
     # x = resize(x)
     # pass
 
     img = cv2.imread('d:/desktop/tmp.png', cv2.IMREAD_COLOR)
     hobj = ndarray2hobject(img)
-    size = halcon.get_image_size(hobj)
-
-    # halcon.dev_open_window (0, 0, , Height/4, 'black', WindowHandle)
-    # halcon.dev_display (Image)
+    w, h = halcon.get_image_size(hobj)
+    # halcon.dev_open_window(0, 0, w, h, 'black', WindowHandle)
+    # halcon.dev_display (Image)
```

