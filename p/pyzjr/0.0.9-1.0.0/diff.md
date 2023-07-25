# Comparing `tmp/pyzjr-0.0.9.tar.gz` & `tmp/pyzjr-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyzjr-0.0.9.tar", last modified: Fri Jul  7 11:36:33 2023, max compression
+gzip compressed data, was "dist\pyzjr-1.0.0.tar", last modified: Tue Jul 25 03:00:20 2023, max compression
```

## Comparing `pyzjr-0.0.9.tar` & `pyzjr-1.0.0.tar`

### file list

```diff
@@ -1,22 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 11:36:33.000000 pyzjr-0.0.9/
--rw-rw-rw-   0        0        0     1591 2023-07-07 11:36:33.000000 pyzjr-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0      664 2023-07-07 11:35:18.000000 pyzjr-0.0.9/README.md
-drwxrwxrwx   0        0        0        0 2023-07-07 11:36:33.000000 pyzjr-0.0.9/pyzjr/
--rw-rw-rw-   0        0        0     3959 2023-07-02 08:05:46.000000 pyzjr-0.0.9/pyzjr/ColorModule.py
--rw-rw-rw-   0        0        0    18267 2023-07-04 09:37:15.000000 pyzjr-0.0.9/pyzjr/Enimage.py
--rw-rw-rw-   0        0        0     9091 2023-07-07 11:28:19.000000 pyzjr-0.0.9/pyzjr/MinIO.py
--rw-rw-rw-   0        0        0     3624 2023-06-10 05:53:05.000000 pyzjr-0.0.9/pyzjr/PIC.py
--rw-rw-rw-   0        0        0     4544 2023-07-04 09:36:13.000000 pyzjr-0.0.9/pyzjr/TrackBar.py
--rw-rw-rw-   0        0        0      104 2023-06-10 05:53:05.000000 pyzjr-0.0.9/pyzjr/Z.py
--rw-rw-rw-   0        0        0     1357 2023-07-07 11:29:39.000000 pyzjr-0.0.9/pyzjr/__init__.py
--rw-rw-rw-   0        0        0     5028 2023-07-07 11:31:29.000000 pyzjr-0.0.9/pyzjr/definition.py
--rw-rw-rw-   0        0        0     4073 2023-06-10 05:53:05.000000 pyzjr-0.0.9/pyzjr/utils.py
--rw-rw-rw-   0        0        0     2784 2023-06-10 05:53:05.000000 pyzjr-0.0.9/pyzjr/video.py
--rw-rw-rw-   0        0        0     2334 2023-07-04 09:41:55.000000 pyzjr-0.0.9/pyzjr/zmath.py
-drwxrwxrwx   0        0        0        0 2023-07-07 11:36:33.000000 pyzjr-0.0.9/pyzjr.egg-info/
--rw-rw-rw-   0        0        0     1591 2023-07-07 11:36:33.000000 pyzjr-0.0.9/pyzjr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2023-07-07 11:36:33.000000 pyzjr-0.0.9/pyzjr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 11:36:33.000000 pyzjr-0.0.9/pyzjr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-07 11:36:33.000000 pyzjr-0.0.9/pyzjr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-07 11:36:33.000000 pyzjr-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0     1734 2023-07-07 11:29:41.000000 pyzjr-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 03:00:20.000000 pyzjr-1.0.0/
+-rw-rw-rw-   0        0        0     2733 2023-07-25 03:00:20.000000 pyzjr-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1547 2023-07-25 03:00:07.000000 pyzjr-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 03:00:20.000000 pyzjr-1.0.0/pyzjr/
+-rw-rw-rw-   0        0        0     3959 2023-07-02 08:05:46.000000 pyzjr-1.0.0/pyzjr/ColorModule.py
+-rw-rw-rw-   0        0        0    17203 2023-07-11 01:30:30.000000 pyzjr-1.0.0/pyzjr/Enimage.py
+-rw-rw-rw-   0        0        0     3932 2023-07-21 17:30:08.000000 pyzjr-1.0.0/pyzjr/FM.py
+-rw-rw-rw-   0        0        0     9085 2023-07-15 12:01:54.000000 pyzjr-1.0.0/pyzjr/MinIO.py
+-rw-rw-rw-   0        0        0     6343 2023-07-15 12:04:40.000000 pyzjr-1.0.0/pyzjr/PIC.py
+-rw-rw-rw-   0        0        0     6361 2023-07-16 03:00:08.000000 pyzjr-1.0.0/pyzjr/Showimage.py
+-rw-rw-rw-   0        0        0     4544 2023-07-04 09:36:13.000000 pyzjr-1.0.0/pyzjr/TrackBar.py
+-rw-rw-rw-   0        0        0      312 2023-07-12 11:15:25.000000 pyzjr-1.0.0/pyzjr/Z.py
+-rw-rw-rw-   0        0        0      976 2023-07-25 03:00:09.000000 pyzjr-1.0.0/pyzjr/__init__.py
+-rw-rw-rw-   0        0        0     6164 2023-07-22 02:13:00.000000 pyzjr-1.0.0/pyzjr/definition.py
+-rw-rw-rw-   0        0        0     2356 2023-07-16 02:19:11.000000 pyzjr-1.0.0/pyzjr/utils.py
+-rw-rw-rw-   0        0        0     4832 2023-07-24 15:58:50.000000 pyzjr-1.0.0/pyzjr/video.py
+-rw-rw-rw-   0        0        0     2786 2023-07-24 16:00:54.000000 pyzjr-1.0.0/pyzjr/zmath.py
+drwxrwxrwx   0        0        0        0 2023-07-25 03:00:20.000000 pyzjr-1.0.0/pyzjr.egg-info/
+-rw-rw-rw-   0        0        0     2733 2023-07-25 03:00:20.000000 pyzjr-1.0.0/pyzjr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      371 2023-07-25 03:00:20.000000 pyzjr-1.0.0/pyzjr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 03:00:20.000000 pyzjr-1.0.0/pyzjr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       85 2023-07-25 03:00:20.000000 pyzjr-1.0.0/pyzjr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-25 03:00:20.000000 pyzjr-1.0.0/pyzjr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-25 03:00:20.000000 pyzjr-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     2020 2023-07-25 03:00:08.000000 pyzjr-1.0.0/setup.py
```

### Comparing `pyzjr-0.0.9/pyzjr/ColorModule.py` & `pyzjr-1.0.0/pyzjr/ColorModule.py`

 * *Files identical despite different names*

### Comparing `pyzjr-0.0.9/pyzjr/Enimage.py` & `pyzjr-1.0.0/pyzjr/Enimage.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,45 +1,42 @@
 """
 - author:Auorui(夏天是冰红茶)
 - creation time:2023.5.11
-- blog ： https://blog.csdn.net/m0_62919535/category_11936595.html?spm=1001.2014.3001.5482
+- blog : https://blog.csdn.net/m0_62919535/category_11936595.html?spm=1001.2014.3001.5482
 - 图形处理相关
 - 滤波算法
     类Filter()
-    - 中值滤波 ： median_filtering
-    - 双边滤波 ： Bilateral_filtering
-    - 均值滤波 ： Arerage_Filtering
-    - 高斯滤波 ： Gaussian_Filtering
+    - 中值滤波 : median_filtering
+    - 双边滤波 : Bilateral_filtering
+    - 均值滤波 : Arerage_Filtering
+    - 高斯滤波 : Gaussian_Filtering
 -增广算法
     类Enhance()
-    - 旋转 ： Rotated_image
-    - 亮度调整 ： Adjusted_image
-    - 裁剪 ： Cut_image
-    - 拼接 ： Stitcher_image
+    - 旋转 : Rotated_image
+    - 亮度调整 : Adjusted_image
+    - 裁剪 : Cut_image
+    - 拼接 : Stitcher_image
     类Random_Enhance()
-    - 垂直或水平翻转 ： horizontal_flip
-    - 随机参数 ： random_generate
-    - 随机翻转 ： random_flip_batch
-    - 随机明暗调整 ： random_brightness_batch
+    - 垂直或水平翻转 : horizontal_flip
+    - 随机参数 : random_generate
+    - 随机翻转 : random_flip_batch
+    - 随机明暗调整 : random_brightness_batch
     - 随机裁剪 : random_Cropping_batch
 -增强算法
     类Retinex()
-    - 单尺度 ： SSR
+    - 单尺度 : SSR
     - 多尺度 : MSR
     - 多尺度自适应增益 : MSRCR
--其他
-    - 图像修补 ： repair_Img
 """
 import numpy as np
 import cv2
 import pyzjr.utils as zjr
 from pyzjr.utils import empty
 import random
-import pyzjr.TrackBar as Trace
-import pyzjr.Z as Z
+
 
 class Filter():
     def median_filtering(self, img,ksize=3):
         """
         中值滤波
         :param img:输入图像
         :param ksize: 核大小
@@ -413,35 +410,15 @@
                 result[:, :, z]=result[:, :, z]*G_ratio
                 img_light[:, :, z] += cv2.resize(img_smooth, (c, r))
 
         img_msrcr = np.exp(result+img_light) - 1
         img_msrcr = np.uint8(cv2.normalize(img_msrcr, None, 0, 255, cv2.NORM_MINMAX))
         return img_msrcr
     
-def repair_Img(img,r=5,flags=Z.repair_NS,mode=0):
-    """
-    * 用于修复图像
-    :param img: 输入图像
-    :param r: 修复半径，即掩膜的像素周围需要参考的区域半径
-    :param flags: 修复算法的标志，有Z.repair_NS、Z.repair_TELEA，默认为Z.repair_NS，
-    :param mode: 是否采用HSV例模式，默认为0，自定义模式，可通过Color下的TrackBar文件中获得
-    :return: 返回修复后的图片
-    """
-    hsvvals = Trace.HSV(mode)
-    tr=Trace.getMask()
-    if hsvvals == 0:
-        hmin, smin, vmin, hmax, smax, vmax = map(int, input().split(','))
-        hsvval=[[hmin, smin, vmin],[hmax, smax, vmax]]
-        imgResult, mask, imgHSV = tr.MaskZone(img, hsvval)
-        dst = cv2.inpaint(img, mask, r, flags)
-        return dst
-    else:
-        imgResult, mask, imgHSV = tr.MaskZone(img, hsvvals)
-        dst = cv2.inpaint(img, mask, r, flags)
-        return dst
+
 
 if __name__=="__main__":
     path= r'../resources/AI2.png'
     img=cv2.imread(path)
     Re=Retinex()
     imgSSR=Re.SSR(img,7)
     imgMSR=Re.MSR(img, [1, 3, 5])
```

### Comparing `pyzjr-0.0.9/pyzjr/MinIO.py` & `pyzjr-1.0.0/pyzjr/MinIO.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 def Creatclient(endpoint,access_key,secret_key,mode=1):
     """
     :param endpoint:  S3服务的主机名
     :param access_key: 用户ID
     :param secret_key: 密码
-    :param mode: 默认为1，自定义，为0，表示使用游乐场测试与开发
+    :param mode: 默认为1,自定义,为0,表示使用游乐场测试与开发
     :return: 返回创建的客户端
     """
     if mode==0:
         client = Minio(
                 endpoint="play.min.io",
                 access_key="Q3AM3UQ867SPQQA43P2F",
                 secret_key="zuf+tfteSlswRu7BJ86wekitnifILbZam1KYY3TG",
```

### Comparing `pyzjr-0.0.9/pyzjr/PIC.py` & `pyzjr-1.0.0/pyzjr/FM.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from tqdm import tqdm
 import requests
 import cv2
 import os, shutil
 from matplotlib import pyplot as plt
+from PIL import Image
+
 
 def download_file(url):
     """
     :param url:下载文件所在url链接
     :return: 下载的位置处于根目录
     """
     print("------", "Start download with urllib")
@@ -22,38 +24,43 @@
         print("File total size is:  ", content_size)
         for data in tqdm(iterable=resp.iter_content(1024), total=content_size, unit='k', desc=name):
             file.write(data)
     print("------", "finish download with urllib\n\n")
 
 def getPhotopath(paths):
     """
-    * 批量读取文件夹下的图片
-    :param paths:输入图片所在位置
-    :return: 该目录下所有的图片
+    * log
+        0.0.19以后修改了一个比较大的bug,使用os读取的路径是“\\”,本来是没有问题的，
+    但如果使用列表循环读取,居然变成了单斜杠。
+    批量读取文件夹下的图片路径
+    :param paths: 文件夹路径
+    :return: 包含图片路径的列表
     """
     imgfile = []
     file_list = os.listdir(paths)
     for i in file_list:
-        newph = os.path.join(paths, i)
+        if i[0] in ['n', 't', 'r', 'b', 'f'] or i[0].isdigit():
+            print(f"Error: 文件名 {i} 开头出现错误！")
+        newph = os.path.join(paths, i).replace("\\","/")
         imgfile.append(newph)
     return imgfile
 
 
-def Pic_rename(img_folder,object='Crack',format='.jpg',num=0):
+def Pic_rename(img_folder,object='Crack',format='jpg',num=0):
     """
     * 用于批量修改图像的命名
     :param img_folder:存放图片的路径
     :param object: 图像的对象
-    :param format: 图片格式，可自行命名，这里给出jpg
+    :param format: 图片格式,可自行命名,这里给出jpg
     :param num: 对图片进行计数
     :return: 用dst替换src
     """
     for img_name in os.listdir(img_folder):
         src = os.path.join(img_folder, img_name)
-        dst = os.path.join(img_folder, object+ str(num) + format)
+        dst = os.path.join(img_folder, object+ str(num) +'.'+ format)
         num= num+1
         os.rename(src, dst)
 
 def read_resize_image(path, size=1.0, show=False, space=False):
     """
     :param path:图片的路径
     :param size: 希望得到图片的大小,cat.0为原始图像
@@ -76,16 +83,16 @@
         print(originalimage.shape)
     return originalimage
 
 
 def load_images_from_folder(folder_path):
     """
     加载一个文件夹下的图片，并存入列表中并返回
-    :param folder_path: 目标图片路径
-    :return: 含有该文件夹下的所有图片
+    :param folder_path: 
+    :return: 
     """
     images = []
     for filename in os.listdir(folder_path):
         if filename.endswith(".jpg") or filename.endswith(".png"):
             img_path = os.path.join(folder_path, filename)
             img = cv2.imread(img_path)
             if img is not None:
```

### Comparing `pyzjr-0.0.9/pyzjr/TrackBar.py` & `pyzjr-1.0.0/pyzjr/TrackBar.py`

 * *Files identical despite different names*

### Comparing `pyzjr-0.0.9/pyzjr/definition.py` & `pyzjr-1.0.0/pyzjr/definition.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 """
 - author:Auorui(夏天是冰红茶)
 - creation time:2022.11.19
 - blog:https://blog.csdn.net/m0_62919535/article/details/127818006
 """
 import cv2
 import math
-from pyzjr.PIC import getPhotopath
+from pyzjr.FM import getPhotopath
 import numpy as np
 import pyzjr.Z as Z
+import numpy as np
+import scipy.ndimage as ndi
+from skimage.filters import sobel
 
 class Clear_quantification():
     def brenner(self,img):
         '''
         Brenner梯度函数
         :param img:narray 二维灰度图像
         :return: int 图像越清晰越大
@@ -56,15 +59,15 @@
         :param img:narray 二维灰度图像
         :return: int 图像越清晰越大
         '''
         return cv2.Laplacian(img, Z.Lap_64F).var()
 
     def SMD(self,img):
         '''
-        SMD（灰度方差）函数
+        SMD(灰度方差)函数
         :param img:narray 二维灰度图像
         :return: int 图像越清晰越大
         '''
         shape = np.shape(img)
         output = 0
         for x in range(1, shape[0] - 1):
             for y in range(0, shape[1]):
@@ -95,15 +98,15 @@
         quanti=Clear_quantification()
         imggray = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)
         imageVar = quanti.Laplacian(imggray)
         return imageVar
 
     def getTest(self,imgfile):
         """
-        :param imgfile: getPhotopath（）
+        :param imgfile: getPhotopath()
         :return: 模糊值排序
         """
         c = []
         for i in imgfile:
             # print(i)
             img = cv2.imread(i)
             image = self.getImgVar(img)
@@ -125,34 +128,61 @@
         imgfile2 = getPhotopath(pathStd)
         a = self.getTest(imgfile1)
         b = self.getTest(imgfile2)
         thr = (a[0], b[0])
         # print(thr)
         return thr
 
-def vagueJudge(image, show_minandmax=True):
+def vagueJudge(img, show_minandmax=True):
     """
-    :param image: 图片
+    :param img: 图片
     :param show_minandmax:是否输出模糊未知区间
     :return: 模糊数值打印在图片上显示
     """
     Fuzzy = Fuzzy_image()
-    img = cv2.imread(image)
     imgVar = Fuzzy.getImgVar(img)
     minThr, maxThr = Fuzzy.getThr()
     if imgVar > maxThr:
         cv2.putText(img, f"Not Vague{imgVar:.2f}", (12, 70), cv2.FONT_HERSHEY_PLAIN, 3,
                         (255, 0, 0), 3)
     else:
         cv2.putText(img, f"Vague{imgVar:.2f}", (12, 70), cv2.FONT_HERSHEY_PLAIN, 3,
                         (255, 0, 0), 3)
     if show_minandmax:
         print(minThr, maxThr)
     else:
         pass
-    cv2.imshow("img", img)
-    k = cv2.waitKey(0) & 0xFF
+    return img
 
 
+def Bulrmetric(img, size=11):
+    """
+    计算指示图像中模糊强度的度量(0表示无模糊,1表示最大模糊)
+    但实际上还是要根据我们的标准图与模糊图得到模糊区间
+    :param img: 图片,最好是BGR格式读进来,因为这个要对单通道进行处理
+    :param size: 重新模糊过滤器的大小
+    :return: float
+    """
+    image = cv2.cvtColor(img, cv2.COLOR_BGR2GRAY)
+    image = np.array(image, dtype=np.float32) / 255
+    n_axes = image.ndim
+    shape = image.shape
+    blur_metric = []
+
+    slices = tuple([slice(2, s - 1) for s in shape])
+    for ax in range(n_axes):
+        filt_im = ndi.uniform_filter1d(image, size, axis=ax)
+        im_sharp = np.abs(sobel(image, axis=ax))
+        im_blur = np.abs(sobel(filt_im, axis=ax))
+        T = np.maximum(0, im_sharp - im_blur)
+        M1 = np.sum(im_sharp[slices])
+        M2 = np.sum(T[slices])
+        blur_metric.append(np.abs((M1 - M2)) / M1)
+
+    return np.max(blur_metric) if len(blur_metric) > 0 else 0.0
+
 if __name__ == "__main__":
-    image="./test/01.jpg"   #需要进行测试的图片
-    vagueJudge(image)
+    image="./ces/test/01.jpg"   #需要进行测试的图片
+    image=cv2.imread(image)
+    img=vagueJudge(image)
+    cv2.imshow("img", img)
+    k = cv2.waitKey(0) & 0xFF
```

### Comparing `pyzjr-0.0.9/pyzjr/zmath.py` & `pyzjr-1.0.0/pyzjr/zmath.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,30 @@
+import numpy as np
+from decimal import Decimal
+
 def EuclideanDis(pts1, pts2):
     """
-    欧式距离
-    :param pts1: 位置（x1,y1）
-    :param pts2: 位置（x2,y2）
-    :return: 两点间距离
+    欧式距离与中心点
+    :param pts1: 位置(x1,y1)
+    :param pts2: 位置(x2,y2)
+    :return: (两点间距离, 中心点)
     """
-    return ((pts2[0] - pts1[0]) ** 2 + (pts2[1] - pts1[1]) ** 2) ** 0.5
-
-
-
-
-
-
-
-
+    distance = ((pts2[0] - pts1[0]) ** 2 + (pts2[1] - pts1[1]) ** 2) ** 0.5
+    center = ((pts1[0] + pts2[0]) / 2, (pts1[1] + pts2[1]) / 2)
+    return distance, center
+
+def retain(val,t=2):
+    """精准保留小数,默认2位"""
+    value=Decimal(val)
+    return round(value,t)
+
+def normal(x, mu, sigma):
+    """正态分布（高斯分布）概率密度函数"""
+    p = 1 / np.sqrt(2 * np.pi * sigma**2)
+    return p * np.exp(-0.5 / sigma**2 * (x - mu)**2)
 
 class pysort():
     def insertion_sort(self, arr):
         """
         直接插入排序
         :param arr:
         :return:
```

### Comparing `pyzjr-0.0.9/setup.py` & `pyzjr-1.0.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,38 +15,49 @@
 
 # these things are needed for the README.md show on pypi (if you dont need delete it)
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-# you need to change all these
-VERSION = '0.0.9'
-DESCRIPTION = ' a computer vision library that supports both Win and Mac '
-LONG_DESCRIPTION = 'pyzjr is a computer vision library that supports both Win and Mac'
+
+VERSION = '1.0.0'
+DESCRIPTION = ' A computer vision library that supports Win, packaged with patches for visual libraries such as \
+                Opencv, matplotlib, and image. In the future, Pytorch will also be supported, all of which are personal (Auorui) \
+                engineering code experience. '
+LONG_DESCRIPTION = 'pyzjr is a computer vision library that supports Win'
 
 setup(
     name="pyzjr",
     version=VERSION,
     author="Auorui",
     author_email='zjricetea@gmail.com',
     url='https://github.com/Auorui/pyzjr',
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
     license='MIT',
-    install_requires=[],
-    keywords=['python', 'computer vision', 'pyzjr','windows','mac','linux'],
+    install_requires=[
+        'requests',
+        'tqdm',
+        'matplotlib',
+        'numpy',
+        'imageio',
+        'scikit-image',
+        'torch',
+        'opencv-python',
+        'pillow',
+        'minio'
+    ],
+    keywords=['python', 'computer vision', 'pyzjr','windows'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
-        "Operating System :: Unix",
-        "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
     ]
 )
```

