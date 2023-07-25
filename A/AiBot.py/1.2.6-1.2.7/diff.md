# Comparing `tmp/AiBot.py-1.2.6.tar.gz` & `tmp/AiBot.py-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AiBot.py-1.2.6.tar", last modified: Fri Jul 14 01:15:52 2023, max compression
+gzip compressed data, was "AiBot.py-1.2.7.tar", last modified: Tue Jul 25 01:21:30 2023, max compression
```

## Comparing `AiBot.py-1.2.6.tar` & `AiBot.py-1.2.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 chenxun    (501) staff       (20)        0 2023-07-14 01:15:52.693468 AiBot.py-1.2.6/
-drwxr-xr-x   0 chenxun    (501) staff       (20)        0 2023-07-14 01:15:52.688877 AiBot.py-1.2.6/AiBot/
--rw-r--r--   0 chenxun    (501) staff       (20)    54124 2023-07-14 01:10:01.000000 AiBot.py-1.2.6/AiBot/_AndroidBot.py
--rw-r--r--   0 chenxun    (501) staff       (20)    21135 2023-03-13 02:59:10.000000 AiBot.py-1.2.6/AiBot/_WebBot.py
--rw-r--r--   0 chenxun    (501) staff       (20)    35796 2023-07-14 01:14:57.000000 AiBot.py-1.2.6/AiBot/_WinBot.py
--rw-r--r--   0 chenxun    (501) staff       (20)      162 2022-12-11 09:17:44.000000 AiBot.py-1.2.6/AiBot/__init__.py
--rw-r--r--   0 chenxun    (501) staff       (20)     5044 2022-08-31 16:13:27.000000 AiBot.py-1.2.6/AiBot/_loguru_format.py
--rw-r--r--   0 chenxun    (501) staff       (20)     1712 2023-03-22 01:46:17.000000 AiBot.py-1.2.6/AiBot/_utils.py
-drwxr-xr-x   0 chenxun    (501) staff       (20)        0 2023-07-14 01:15:52.691084 AiBot.py-1.2.6/AiBot.py.egg-info/
--rw-r--r--   0 chenxun    (501) staff       (20)      249 2023-07-14 01:15:52.000000 AiBot.py-1.2.6/AiBot.py.egg-info/PKG-INFO
--rw-r--r--   0 chenxun    (501) staff       (20)      368 2023-07-14 01:15:52.000000 AiBot.py-1.2.6/AiBot.py.egg-info/SOURCES.txt
--rw-r--r--   0 chenxun    (501) staff       (20)        1 2023-07-14 01:15:52.000000 AiBot.py-1.2.6/AiBot.py.egg-info/dependency_links.txt
--rw-r--r--   0 chenxun    (501) staff       (20)       14 2023-07-14 01:15:52.000000 AiBot.py-1.2.6/AiBot.py.egg-info/requires.txt
--rw-r--r--   0 chenxun    (501) staff       (20)        6 2023-07-14 01:15:52.000000 AiBot.py-1.2.6/AiBot.py.egg-info/top_level.txt
--rw-r--r--   0 chenxun    (501) staff       (20)     1056 2022-08-31 16:13:27.000000 AiBot.py-1.2.6/LICENSE
--rw-r--r--   0 chenxun    (501) staff       (20)      249 2023-07-14 01:15:52.692932 AiBot.py-1.2.6/PKG-INFO
--rw-r--r--   0 chenxun    (501) staff       (20)     5253 2022-12-16 13:41:49.000000 AiBot.py-1.2.6/README.md
--rw-r--r--   0 chenxun    (501) staff       (20)      104 2022-08-31 16:13:27.000000 AiBot.py-1.2.6/pyproject.toml
--rw-r--r--   0 chenxun    (501) staff       (20)       38 2023-07-14 01:15:52.693606 AiBot.py-1.2.6/setup.cfg
--rw-r--r--   0 chenxun    (501) staff       (20)      622 2023-07-14 01:12:34.000000 AiBot.py-1.2.6/setup.py
-drwxr-xr-x   0 chenxun    (501) staff       (20)        0 2023-07-14 01:15:52.692439 AiBot.py-1.2.6/test/
--rw-r--r--   0 chenxun    (501) staff       (20)     1534 2023-07-14 01:10:12.000000 AiBot.py-1.2.6/test/test_android.py
--rw-r--r--   0 chenxun    (501) staff       (20)      796 2023-02-16 09:55:43.000000 AiBot.py-1.2.6/test/test_web.py
--rw-r--r--   0 chenxun    (501) staff       (20)      370 2022-12-11 09:17:44.000000 AiBot.py-1.2.6/test/test_win.py
+drwxr-xr-x   0 chenxun    (501) staff       (20)        0 2023-07-25 01:21:30.154239 AiBot.py-1.2.7/
+drwxr-xr-x   0 chenxun    (501) staff       (20)        0 2023-07-25 01:21:30.144803 AiBot.py-1.2.7/AiBot/
+-rw-r--r--   0 chenxun    (501) staff       (20)    55472 2023-07-25 01:14:14.000000 AiBot.py-1.2.7/AiBot/_AndroidBot.py
+-rw-r--r--   0 chenxun    (501) staff       (20)    21135 2023-03-13 02:59:10.000000 AiBot.py-1.2.7/AiBot/_WebBot.py
+-rw-r--r--   0 chenxun    (501) staff       (20)    35796 2023-07-14 01:14:57.000000 AiBot.py-1.2.7/AiBot/_WinBot.py
+-rw-r--r--   0 chenxun    (501) staff       (20)      162 2022-12-11 09:17:44.000000 AiBot.py-1.2.7/AiBot/__init__.py
+-rw-r--r--   0 chenxun    (501) staff       (20)     5044 2022-08-31 16:13:27.000000 AiBot.py-1.2.7/AiBot/_loguru_format.py
+-rw-r--r--   0 chenxun    (501) staff       (20)     1712 2023-03-22 01:46:17.000000 AiBot.py-1.2.7/AiBot/_utils.py
+drwxr-xr-x   0 chenxun    (501) staff       (20)        0 2023-07-25 01:21:30.151237 AiBot.py-1.2.7/AiBot.py.egg-info/
+-rw-r--r--   0 chenxun    (501) staff       (20)      249 2023-07-25 01:21:30.000000 AiBot.py-1.2.7/AiBot.py.egg-info/PKG-INFO
+-rw-r--r--   0 chenxun    (501) staff       (20)      368 2023-07-25 01:21:30.000000 AiBot.py-1.2.7/AiBot.py.egg-info/SOURCES.txt
+-rw-r--r--   0 chenxun    (501) staff       (20)        1 2023-07-25 01:21:30.000000 AiBot.py-1.2.7/AiBot.py.egg-info/dependency_links.txt
+-rw-r--r--   0 chenxun    (501) staff       (20)       14 2023-07-25 01:21:30.000000 AiBot.py-1.2.7/AiBot.py.egg-info/requires.txt
+-rw-r--r--   0 chenxun    (501) staff       (20)        6 2023-07-25 01:21:30.000000 AiBot.py-1.2.7/AiBot.py.egg-info/top_level.txt
+-rw-r--r--   0 chenxun    (501) staff       (20)     1056 2022-08-31 16:13:27.000000 AiBot.py-1.2.7/LICENSE
+-rw-r--r--   0 chenxun    (501) staff       (20)      249 2023-07-25 01:21:30.153834 AiBot.py-1.2.7/PKG-INFO
+-rw-r--r--   0 chenxun    (501) staff       (20)     5253 2022-12-16 13:41:49.000000 AiBot.py-1.2.7/README.md
+-rw-r--r--   0 chenxun    (501) staff       (20)      104 2022-08-31 16:13:27.000000 AiBot.py-1.2.7/pyproject.toml
+-rw-r--r--   0 chenxun    (501) staff       (20)       38 2023-07-25 01:21:30.154359 AiBot.py-1.2.7/setup.cfg
+-rw-r--r--   0 chenxun    (501) staff       (20)      622 2023-07-25 01:21:01.000000 AiBot.py-1.2.7/setup.py
+drwxr-xr-x   0 chenxun    (501) staff       (20)        0 2023-07-25 01:21:30.153359 AiBot.py-1.2.7/test/
+-rw-r--r--   0 chenxun    (501) staff       (20)     1534 2023-07-14 01:10:12.000000 AiBot.py-1.2.7/test/test_android.py
+-rw-r--r--   0 chenxun    (501) staff       (20)      796 2023-02-16 09:55:43.000000 AiBot.py-1.2.7/test/test_web.py
+-rw-r--r--   0 chenxun    (501) staff       (20)      370 2022-12-11 09:17:44.000000 AiBot.py-1.2.7/test/test_win.py
```

### Comparing `AiBot.py-1.2.6/AiBot/_AndroidBot.py` & `AiBot.py-1.2.7/AiBot/_AndroidBot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import abc
 import json
 import socket
 import socketserver
 import sys
 import threading
 import time
-import re
 from ast import literal_eval
+from datetime import datetime
 from typing import Optional, Dict, List, Tuple, Union
 
 from loguru import logger
 
 from ._utils import _protect, _Region, _Algorithm, _SubColors
 
 
@@ -79,24 +79,31 @@
     代替 Point 元组
     """
 
     def __init__(self, p1: Point, p2: Point):
         self.p1 = p1
         self.p2 = p2
 
-    def click(self, offset_x: float = 0, offset_y: float = 0):
+    def click(self, offset_x: float = 0, offset_y: float = 0) -> bool:
         """
-        点击2元组中，2个坐标点的中间位置
+        点击元素的中心坐标
 
         :param offset_x:
         :param offset_y:
         :return:
         """
-        point = self.p1.get_points_center(self.p2)
-        return point.click(offset_x=offset_x, offset_y=offset_y)
+        return self.central_point().click(offset_x=offset_x, offset_y=offset_y)
+
+    def central_point(self) -> Point:
+        """
+        获取元素的中心坐标
+
+        :return:
+        """
+        return self.p1.get_points_center(self.p2)
 
     def __getitem__(self, item):
         if item == 0:
             return self.p1
         elif item == 1:
             return self.p2
         else:
@@ -613,15 +620,15 @@
         return self.__send_data("dispatchGesture", gesture_path_str, duration) == "true"
 
     def press(self, point: _Point_Tuple, duration: float) -> bool:
         """
         手指按下
 
         :param point: 坐标
-        :param duration: 持续时间
+        :param duration: 持续时间，单位秒
         :return:
         """
         return self.__send_data("press", point[0], point[1], duration * 1000) == "true"
 
     def move(self, point: _Point_Tuple, duration: float) -> bool:
         """
         手指移动
@@ -634,27 +641,45 @@
 
     def release(self) -> bool:
         """手指抬起"""
         return self.__send_data("release") == "true"
 
     def press_release(self, point: _Point_Tuple, duration: float) -> bool:
         """
-        按下屏幕并释放
+        按下屏幕坐标点并释放
 
+        :param point: 按压坐标
+        :param duration: 按压时长，单位秒
         :return:
         """
         result = self.press(point, duration)
         if not result:
             return False
         time.sleep(duration)
         result2 = self.release()
         if not result2:
             return False
         return True
 
+    def press_release_by_ele(self, xpath, duration: float, wait_time: float = None,
+                             interval_time: float = None, ) -> bool:
+        """
+        按压元素并释放
+
+        :param xpath: 要按压的元素
+        :param duration: 按压时长，单位秒
+        :param wait_time: 查找元素的最长等待时间
+        :param interval_time: 查找元素的轮询间隔时间
+        :return:
+        """
+        point2s = self.get_element_rect(xpath, wait_time=wait_time, interval_time=interval_time, raise_err=False)
+        if point2s is None:
+            return False
+        return self.press_release(point2s.central_point(), duration)
+
     # ##############
     #   OCR 相关   #
     ################
     @staticmethod
     def __parse_ocr(text: str) -> list:
         """
         解析 OCR 识别出出来的信息
@@ -700,15 +725,15 @@
             scale = 1.0
 
         response = self.__send_data("ocr", *region, algorithm_type, threshold, max_val, scale)
         if response == "null" or response == "":
             return []
         return self.__parse_ocr(response)
 
-    def init_ocr_server(self, ip: str, port: int=9752) -> bool:
+    def init_ocr_server(self, ip: str, port: int = 9752) -> bool:
         """
         初始化 OCR 服务
 
         :param ip:
         :param port:
         :return:
         """
@@ -1259,14 +1284,27 @@
 
         :param text: 弹窗内容
         :param duration: 弹窗持续时间，单位：秒
         :return:
         """
         return self.__send_data("showToast", text, duration * 1000) == "true"
 
+    def sleep(self, wait_time: float, interval_time: float = 1.5):
+        """
+        强制等待
+
+        :param wait_time: 等待时长
+        :param interval_time: 等待时轮询间隔时间
+        :return:
+        """
+        end_time = datetime.now().timestamp() + wait_time
+        while datetime.now().timestamp() < end_time:
+            self.show_toast("等待中...", 1)
+            time.sleep(interval_time)
+
     def send_keys(self, text: str) -> bool:
         """
         发送文本，需要打开 AiBot 输入法
 
         :param text: 文本内容
         :return:
         """
```

### Comparing `AiBot.py-1.2.6/AiBot/_WebBot.py` & `AiBot.py-1.2.7/AiBot/_WebBot.py`

 * *Files identical despite different names*

### Comparing `AiBot.py-1.2.6/AiBot/_WinBot.py` & `AiBot.py-1.2.7/AiBot/_WinBot.py`

 * *Files identical despite different names*

### Comparing `AiBot.py-1.2.6/AiBot/_loguru_format.py` & `AiBot.py-1.2.7/AiBot/_loguru_format.py`

 * *Files identical despite different names*

### Comparing `AiBot.py-1.2.6/AiBot/_utils.py` & `AiBot.py-1.2.7/AiBot/_utils.py`

 * *Files identical despite different names*

### Comparing `AiBot.py-1.2.6/LICENSE` & `AiBot.py-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `AiBot.py-1.2.6/README.md` & `AiBot.py-1.2.7/README.md`

 * *Files identical despite different names*

### Comparing `AiBot.py-1.2.6/setup.py` & `AiBot.py-1.2.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 install_requires = [
     "loguru~=0.6.0"
 ]
 
 setup_kwargs = {
     'name': 'AiBot.py',
-    'version': '1.2.6',
+    'version': '1.2.7',
     'description': '...',
     'long_description': '...',
     'long_description_content_type': 'text/markdown',
     'author': 'waitan2018',
     'author_email': None,
     'maintainer': 'waitan2018',
     'maintainer_email': None,
```

### Comparing `AiBot.py-1.2.6/test/test_android.py` & `AiBot.py-1.2.7/test/test_android.py`

 * *Files identical despite different names*

### Comparing `AiBot.py-1.2.6/test/test_web.py` & `AiBot.py-1.2.7/test/test_web.py`

 * *Files identical despite different names*

