# Comparing `tmp/poocr-0.0.8.tar.gz` & `tmp/poocr-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poocr-0.0.8.tar", last modified: Thu Apr 20 14:36:10 2023, max compression
+gzip compressed data, was "poocr-0.0.9.tar", last modified: Tue Jul 25 15:18:24 2023, max compression
```

## Comparing `poocr-0.0.8.tar` & `poocr-0.0.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 14:36:10.607901 poocr-0.0.8/
--rw-rw-rw-   0        0        0     1093 2022-09-13 01:21:27.000000 poocr-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     4115 2023-04-20 14:36:10.608898 poocr-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     3594 2023-04-18 15:02:36.000000 poocr-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-04-20 14:36:10.545657 poocr-0.0.8/poocr/
--rw-rw-rw-   0        0        0      522 2023-04-18 16:20:50.000000 poocr-0.0.8/poocr/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-20 14:36:10.585176 poocr-0.0.8/poocr/api/
--rw-rw-rw-   0        0        0      265 2023-03-25 11:08:27.000000 poocr-0.0.8/poocr/api/__init__.py
--rw-rw-rw-   0        0        0    20975 2023-01-30 12:39:04.000000 poocr-0.0.8/poocr/api/ocr.py
--rw-rw-rw-   0        0        0     3438 2023-04-20 14:35:27.000000 poocr-0.0.8/poocr/api/ocr2excel.py
-drwxrwxrwx   0        0        0        0 2023-04-20 14:36:10.589672 poocr-0.0.8/poocr/core/
--rw-rw-rw-   0        0        0     4071 2023-01-30 12:39:04.000000 poocr-0.0.8/poocr/core/OCR.py
--rw-rw-rw-   0        0        0      223 2023-01-22 06:56:13.000000 poocr-0.0.8/poocr/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-20 14:36:10.602898 poocr-0.0.8/poocr/lib/
--rw-rw-rw-   0        0        0     1017 2023-01-28 13:49:56.000000 poocr-0.0.8/poocr/lib/CommonUtils.py
--rw-rw-rw-   0        0        0     1132 2023-01-30 12:39:04.000000 poocr-0.0.8/poocr/lib/Config.py
--rw-rw-rw-   0        0        0      852 2023-01-30 12:39:04.000000 poocr-0.0.8/poocr/lib/Const.py
--rw-rw-rw-   0        0        0        0 2023-01-22 10:20:33.000000 poocr-0.0.8/poocr/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-20 14:36:10.568668 poocr-0.0.8/poocr.egg-info/
--rw-rw-rw-   0        0        0     4115 2023-04-20 14:36:10.000000 poocr-0.0.8/poocr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      455 2023-04-20 14:36:10.000000 poocr-0.0.8/poocr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 14:36:10.000000 poocr-0.0.8/poocr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-18 16:20:22.000000 poocr-0.0.8/poocr.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       47 2023-04-20 14:36:10.000000 poocr-0.0.8/poocr.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-20 14:36:10.000000 poocr-0.0.8/poocr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      741 2023-04-20 14:36:10.611922 poocr-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      389 2022-10-23 08:47:10.000000 poocr-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-20 14:36:10.606896 poocr-0.0.8/tests/
--rw-rw-rw-   0        0        0      181 2023-01-30 12:39:04.000000 poocr-0.0.8/tests/__init__.py
--rw-rw-rw-   0        0        0      947 2023-04-19 16:14:45.000000 poocr-0.0.8/tests/test_tencent.py
+drwxrwxrwx   0        0        0        0 2023-07-25 15:18:24.611761 poocr-0.0.9/
+-rw-rw-rw-   0        0        0     1093 2022-09-13 01:21:27.000000 poocr-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     4318 2023-07-25 15:18:24.612771 poocr-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3797 2023-07-25 15:17:58.000000 poocr-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 15:18:24.526912 poocr-0.0.9/poocr/
+-rw-rw-rw-   0        0        0      522 2023-04-18 16:20:50.000000 poocr-0.0.9/poocr/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 15:18:24.581227 poocr-0.0.9/poocr/api/
+-rw-rw-rw-   0        0        0      265 2023-03-25 11:08:27.000000 poocr-0.0.9/poocr/api/__init__.py
+-rw-rw-rw-   0        0        0    25192 2023-07-25 15:11:46.000000 poocr-0.0.9/poocr/api/ocr.py
+-rw-rw-rw-   0        0        0     3488 2023-07-23 15:33:05.000000 poocr-0.0.9/poocr/api/ocr2excel.py
+drwxrwxrwx   0        0        0        0 2023-07-25 15:18:24.589228 poocr-0.0.9/poocr/core/
+-rw-rw-rw-   0        0        0     4271 2023-07-25 15:06:57.000000 poocr-0.0.9/poocr/core/OCR.py
+-rw-rw-rw-   0        0        0      223 2023-01-22 06:56:13.000000 poocr-0.0.9/poocr/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 15:18:24.603246 poocr-0.0.9/poocr/lib/
+-rw-rw-rw-   0        0        0     1017 2023-01-28 13:49:56.000000 poocr-0.0.9/poocr/lib/CommonUtils.py
+-rw-rw-rw-   0        0        0     1132 2023-01-30 12:39:04.000000 poocr-0.0.9/poocr/lib/Config.py
+-rw-rw-rw-   0        0        0      852 2023-01-30 12:39:04.000000 poocr-0.0.9/poocr/lib/Const.py
+-rw-rw-rw-   0        0        0        0 2023-01-22 10:20:33.000000 poocr-0.0.9/poocr/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 15:18:24.562328 poocr-0.0.9/poocr.egg-info/
+-rw-rw-rw-   0        0        0     4318 2023-07-25 15:18:24.000000 poocr-0.0.9/poocr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      455 2023-07-25 15:18:24.000000 poocr-0.0.9/poocr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 15:18:24.000000 poocr-0.0.9/poocr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-25 15:08:56.000000 poocr-0.0.9/poocr.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       47 2023-07-25 15:18:24.000000 poocr-0.0.9/poocr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-25 15:18:24.000000 poocr-0.0.9/poocr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      741 2023-07-25 15:18:24.614769 poocr-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      389 2022-10-23 08:47:10.000000 poocr-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 15:18:24.609251 poocr-0.0.9/tests/
+-rw-rw-rw-   0        0        0      181 2023-01-30 12:39:04.000000 poocr-0.0.9/tests/__init__.py
+-rw-rw-rw-   0        0        0      947 2023-04-19 16:14:45.000000 poocr-0.0.9/tests/test_tencent.py
```

### Comparing `poocr-0.0.8/LICENSE` & `poocr-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `poocr-0.0.8/PKG-INFO` & `poocr-0.0.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poocr
-Version: 0.0.8
+Version: 0.0.9
 Summary: pip install poocr
 Home-page: https://www.python-office.com/
 Author: CoderWanFeng
 Author-email: 1957875073@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CoderWanFeng/poocr/issues
 Project-URL: Documentation, https://github.com/CoderWanFeng/poocr/blob/main/README.md
@@ -31,15 +31,15 @@
 </p>
 
 
 <p align="center" name="'github">
   	<a href="https://mp.weixin.qq.com/s/yaSmFKO3RrBpyanW3nvRAQ">
 	<img src="https://img.shields.io/badge/QQ-163434413-orange"/>
   </a>
-    	<a href="https://mp.weixin.qq.com/s/wx-JkgOUoJhb-7ZESxl93w">
+    	<a href="https://mp.weixin.qq.com/s/NN2pX2bQPpczOeGF4ARNtw">
 	<img src="https://img.shields.io/badge/%E5%BE%AE%E4%BF%A1-%E4%BA%A4%E6%B5%81%E7%BE%A4-brightgreen"/>
   </a>
 </p>
 
 
 -------------------------------------------------------------------------------
 
@@ -64,15 +64,15 @@
 ```
 
 
 -------------------------------------------------------------------------------
 
 ## 📝功能
 
-- [📘官网：https://www.python-office.com/](https://www.python-office.com/)
+- [📘Python自动化办公的官网：https://www.python-office.com/](https://www.python-office.com/)
 
 -  💻所有功能的列表👉[点我直达](https://www.python-office.com/video/poocr.html)
 
 
 ## 常见问题
 
 1. 如何配置poocr-config.toml？
@@ -107,8 +107,12 @@
 
 -------------------------------------------------------------------------------
 
 
 ## 📌联系作者
 
 
-![CoderWanFeng](https://python-office-1300615378.cos.ap-chongqing.myqcloud.com/python-office-qr.jpg)
+<p align="center" id='开源交流群-banner'>
+<a target="_blank" href='https://python-office-1300615378.cos.ap-chongqing.myqcloud.com/python-office.jpg'>
+<img src="https://python-office-1300615378.cos.ap-chongqing.myqcloud.com/python-office-qr.jpg" width="100%"/>
+</a> 
+</p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: poocr Version: 0.0.8 Summary: pip install poocr
+Metadata-Version: 2.1 Name: poocr Version: 0.0.9 Summary: pip install poocr
 Home-page: https://www.python-office.com/ Author: CoderWanFeng Author-email:
 1957875073@qq.com License: MIT Project-URL: Bug Tracker, https://github.com/
 CoderWanFeng/poocr/issues Project-URL: Documentation, https://github.com/
 CoderWanFeng/poocr/blob/main/README.md Project-URL: Source Code, https://
 github.com/CoderWanFeng/poocr Platform: any Requires-Python: >=3.7 Description-
 Content-Type: text/markdown License-File: LICENSE
 [https://website-python-1300615378.cos.ap-nanjing.myqcloud.com/ads%2F1040x100-
@@ -15,17 +15,18 @@
 - ## ðç®ä» poocr æ¯å¿«éè°ç¨è¾è®¯äºAIå¹³å°åè½çæ¥å£åéã
 ``poocr``ææåè½çå®ç°ï¼é½ä¾æäºè¾è®¯äºçæå­è¯å«ï¼å¦ææ¯å°ç½ç¨æ·ï¼å¯ä»¥**æ«ç ä¸å¾ï¼åè´¹å¼é**~
 ![](https://article-1300615378.cos.ap-nanjing.myqcloud.com/potencent%2Fapi-
 doc%2Fshare.jpg) --------------------------------------------------------------
 ----------------- ## ð¦å®è£ ### ðpip èªå¨ä¸è½½&æ´æ° ``` pip install
 -i https://mirrors.aliyun.com/pypi/simple/ poocr -U ``` -----------------------
 -------------------------------------------------------- ## ðåè½ -
-[ðå®ç½ï¼https://www.python-office.com/](https://www.python-office.com/) -
-ð»ææåè½çåè¡¨ð[ç¹æç´è¾¾](https://www.python-office.com/
-video/poocr.html) ## å¸¸è§é®é¢ 1. å¦ä½éç½®poocr-config.tomlï¼
+[ðPythonèªå¨ååå¬çå®ç½ï¼https://www.python-office.com/](https://
+www.python-office.com/) - ð»ææåè½çåè¡¨ð[ç¹æç´è¾¾](https://
+www.python-office.com/video/poocr.html) ## å¸¸è§é®é¢ 1. å¦ä½éç½®poocr-
+config.tomlï¼
 ç¬¬ä¸æ­¥ï¼ä½ éè¦å¼éè¾è®¯äºçåç¥¨è¯å«åè½ï¼æ¶è´¹åè½ï¼å¾ä¾¿å®ï¼ï¼
 [ç¹æç´è¾¾](https://cloud.tencent.com/act/cps/
 redirect?redirect=10098&cps_key=ca76be5a2293ba3906d6d5407aea15ee)
 ç¬¬äºæ­¥ï¼ä½ éè¦è®¾ç½®ä¸ä¸ªå­è´¦æ·ï¼ä¸è±é±ï¼ï¼[ç¹æç´è¾¾]
 (https://cloud.tencent.com/act/cps/
 redirect?redirect=36394&cps_key=ca76be5a2293ba3906d6d5407aea15ee)
 å¦æä»¥ä¸éç½®ï¼èªå·±ä¸æææ¯ï¼é¾ä»¥å®ç°çè¯ï¼å¯ä»¥ä»è´¹æ¾æå¸®ä½ éç½®ãæçå¾®ä¿¡ï¼ç¹å»ç´è¾¾ð
@@ -40,9 +41,10 @@
 ç»å½GiteeæGithubå¨ä½ é¦é¡µå¯ä»¥çå°ä¸ä¸ª pull request
 æé®ï¼ç¹å»å®ï¼å¡«åä¸äºè¯´æä¿¡æ¯ï¼ç¶åæäº¤å°masteråæ¯å³å¯ã
 6. ç­å¾ç»´æ¤èåå¹¶ ### ðæä¾bugåé¦æå»ºè®®
 æäº¤é®é¢åé¦æ¶ï¼è¯·å¡å¿å¡«ååpython-
 officeä»£ç æ¬èº«æå³çé®é¢ï¼ä¸è¿è¡æå³pythonå­¦ä¹ ï¼çè³æ¯ä¸ªäººç»ä¹ çç¥è¯ç­çåè®¨è®ºã
 - [Github issue](https://github.com/CoderWanFeng/pobaidu/issues) --------------
 ----------------------------------------------------------------- ##
-ðèç³»ä½è ![CoderWanFeng](https://python-office-1300615378.cos.ap-
-chongqing.myqcloud.com/python-office-qr.jpg)
+ðèç³»ä½è
+[https://python-office-1300615378.cos.ap-chongqing.myqcloud.com/python-office-
+                                    qr.jpg]
```

### Comparing `poocr-0.0.8/README.md` & `poocr-0.0.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 </p>
 
 
 <p align="center" name="'github">
   	<a href="https://mp.weixin.qq.com/s/yaSmFKO3RrBpyanW3nvRAQ">
 	<img src="https://img.shields.io/badge/QQ-163434413-orange"/>
   </a>
-    	<a href="https://mp.weixin.qq.com/s/wx-JkgOUoJhb-7ZESxl93w">
+    	<a href="https://mp.weixin.qq.com/s/NN2pX2bQPpczOeGF4ARNtw">
 	<img src="https://img.shields.io/badge/%E5%BE%AE%E4%BF%A1-%E4%BA%A4%E6%B5%81%E7%BE%A4-brightgreen"/>
   </a>
 </p>
 
 
 -------------------------------------------------------------------------------
 
@@ -48,15 +48,15 @@
 ```
 
 
 -------------------------------------------------------------------------------
 
 ## 📝功能
 
-- [📘官网：https://www.python-office.com/](https://www.python-office.com/)
+- [📘Python自动化办公的官网：https://www.python-office.com/](https://www.python-office.com/)
 
 -  💻所有功能的列表👉[点我直达](https://www.python-office.com/video/poocr.html)
 
 
 ## 常见问题
 
 1. 如何配置poocr-config.toml？
@@ -91,8 +91,12 @@
 
 -------------------------------------------------------------------------------
 
 
 ## 📌联系作者
 
 
-![CoderWanFeng](https://python-office-1300615378.cos.ap-chongqing.myqcloud.com/python-office-qr.jpg)
+<p align="center" id='开源交流群-banner'>
+<a target="_blank" href='https://python-office-1300615378.cos.ap-chongqing.myqcloud.com/python-office.jpg'>
+<img src="https://python-office-1300615378.cos.ap-chongqing.myqcloud.com/python-office-qr.jpg" width="100%"/>
+</a> 
+</p>
```

#### html2text {}

```diff
@@ -8,17 +8,18 @@
 - ## ðç®ä» poocr æ¯å¿«éè°ç¨è¾è®¯äºAIå¹³å°åè½çæ¥å£åéã
 ``poocr``ææåè½çå®ç°ï¼é½ä¾æäºè¾è®¯äºçæå­è¯å«ï¼å¦ææ¯å°ç½ç¨æ·ï¼å¯ä»¥**æ«ç ä¸å¾ï¼åè´¹å¼é**~
 ![](https://article-1300615378.cos.ap-nanjing.myqcloud.com/potencent%2Fapi-
 doc%2Fshare.jpg) --------------------------------------------------------------
 ----------------- ## ð¦å®è£ ### ðpip èªå¨ä¸è½½&æ´æ° ``` pip install
 -i https://mirrors.aliyun.com/pypi/simple/ poocr -U ``` -----------------------
 -------------------------------------------------------- ## ðåè½ -
-[ðå®ç½ï¼https://www.python-office.com/](https://www.python-office.com/) -
-ð»ææåè½çåè¡¨ð[ç¹æç´è¾¾](https://www.python-office.com/
-video/poocr.html) ## å¸¸è§é®é¢ 1. å¦ä½éç½®poocr-config.tomlï¼
+[ðPythonèªå¨ååå¬çå®ç½ï¼https://www.python-office.com/](https://
+www.python-office.com/) - ð»ææåè½çåè¡¨ð[ç¹æç´è¾¾](https://
+www.python-office.com/video/poocr.html) ## å¸¸è§é®é¢ 1. å¦ä½éç½®poocr-
+config.tomlï¼
 ç¬¬ä¸æ­¥ï¼ä½ éè¦å¼éè¾è®¯äºçåç¥¨è¯å«åè½ï¼æ¶è´¹åè½ï¼å¾ä¾¿å®ï¼ï¼
 [ç¹æç´è¾¾](https://cloud.tencent.com/act/cps/
 redirect?redirect=10098&cps_key=ca76be5a2293ba3906d6d5407aea15ee)
 ç¬¬äºæ­¥ï¼ä½ éè¦è®¾ç½®ä¸ä¸ªå­è´¦æ·ï¼ä¸è±é±ï¼ï¼[ç¹æç´è¾¾]
 (https://cloud.tencent.com/act/cps/
 redirect?redirect=36394&cps_key=ca76be5a2293ba3906d6d5407aea15ee)
 å¦æä»¥ä¸éç½®ï¼èªå·±ä¸æææ¯ï¼é¾ä»¥å®ç°çè¯ï¼å¯ä»¥ä»è´¹æ¾æå¸®ä½ éç½®ãæçå¾®ä¿¡ï¼ç¹å»ç´è¾¾ð
@@ -33,9 +34,10 @@
 ç»å½GiteeæGithubå¨ä½ é¦é¡µå¯ä»¥çå°ä¸ä¸ª pull request
 æé®ï¼ç¹å»å®ï¼å¡«åä¸äºè¯´æä¿¡æ¯ï¼ç¶åæäº¤å°masteråæ¯å³å¯ã
 6. ç­å¾ç»´æ¤èåå¹¶ ### ðæä¾bugåé¦æå»ºè®®
 æäº¤é®é¢åé¦æ¶ï¼è¯·å¡å¿å¡«ååpython-
 officeä»£ç æ¬èº«æå³çé®é¢ï¼ä¸è¿è¡æå³pythonå­¦ä¹ ï¼çè³æ¯ä¸ªäººç»ä¹ çç¥è¯ç­çåè®¨è®ºã
 - [Github issue](https://github.com/CoderWanFeng/pobaidu/issues) --------------
 ----------------------------------------------------------------- ##
-ðèç³»ä½è ![CoderWanFeng](https://python-office-1300615378.cos.ap-
-chongqing.myqcloud.com/python-office-qr.jpg)
+ðèç³»ä½è
+[https://python-office-1300615378.cos.ap-chongqing.myqcloud.com/python-office-
+                                    qr.jpg]
```

### Comparing `poocr-0.0.8/poocr/__init__.py` & `poocr-0.0.9/poocr/__init__.py`

 * *Files identical despite different names*

### Comparing `poocr-0.0.8/poocr/api/ocr.py` & `poocr-0.0.9/poocr/api/ocr.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,585 +3,663 @@
 @Author  ：程序员晚枫，B站/抖音/微博/小红书/公众号
 @WeChat     ：CoderWanFeng
 @Blog      ：www.python-office.com
 @Date    ：2023/1/22 15:23
 @Description     ：
 '''
 
+import sys
+
 from poocr.core.OCR import OCR
 from poocr.lib.CommonUtils import img2base64
-import sys
 
 
-def get_ocr(configPath):
+def get_ocr(configPath, id, key):
     ocr = OCR()
-    ocr.set_config(configPath)
+    ocr.set_config(configPath, id, key)
     return ocr
 
 
-def do_api(OCR_NAME, img_path, img_url, configPath):
+def do_api(OCR_NAME, img_path, img_url, configPath, id, key):
     """
     通过类的方法名，直接调用方法
     :return:
     """
-    ocr = get_ocr(configPath)
+    ocr = get_ocr(configPath, id, key)
     if img_url:
         ocr_res = ocr.DoOCR(OCR_NAME, ImageBase64=img_path, ImageUrl=img_url)
     else:
         ImageBase64 = img2base64(img_path)
         ocr_res = ocr.DoOCR(OCR_NAME, ImageBase64=ImageBase64, ImageUrl=img_url)
     return ocr_res
 
 
-def AdvertiseOCR(img_path=None, img_url=None, configPath=None):
+def AdvertiseOCR(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
-                  configPath=configPath)
+                  configPath=configPath,
+                  id=id, key=key)
 
 
-def ArithmeticOCR(img_path=None, img_url=None, configPath=None):
+def ArithmeticOCR(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
-                  configPath=configPath)
+                  configPath=configPath,
+                  id=id, key=key)
 
 
-def BankCardOCR(img_path=None, img_url=None, configPath=None):
+def BankCardOCR(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
-                  configPath=configPath)
+                  configPath=configPath,
+                  id=id, key=key)
 
 
-def BankSlipOCR(img_path=None, img_url=None, configPath=None):
+def BankSlipOCR(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
-                  configPath=configPath)
+                  configPath=configPath,
+                  id=id, key=key)
 
 
-def BizLicenseOCR(img_path=None, img_url=None, configPath=None):
+def BizLicenseOCR(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
-                  configPath=configPath)
+                  configPath=configPath,
+                  id=id, key=key)
 
 
-def BusInvoiceOCR(img_path=None, img_url=None, configPath=None):
+def BusInvoiceOCR(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
-                  configPath=configPath)
+                  configPath=configPath,
+                  id=id, key=key)
 
 
-def BusinessCardOCR(img_path=None, img_url=None, configPath=None):
+def BusinessCardOCR(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
-                  configPath=configPath)
+                  configPath=configPath,
+                  id=id, key=key)
 
 
-def CarInvoiceOCR(img_path=None, img_url=None, configPath=None):
+def CarInvoiceOCR(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
-                  configPath=configPath)
+                  configPath=configPath,
+                  id=id, key=key)
 
 
-def ClassifyDetectOCR(img_path=None, img_url=None, configPath=None):
+def ClassifyDetectOCR(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
-                  configPath=configPath)
+                  configPath=configPath,
+                  id=id, key=key)
 
 
-def DriverLicenseOCR(img_path=None, img_url=None, configPath=None):
+def DriverLicenseOCR(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
-                  configPath=configPath)
+                  configPath=configPath,
+                  id=id, key=key)
 
 
-def DutyPaidProofOCR(img_path=None, img_url=None, configPath=None):
+def DutyPaidProofOCR(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
-                  configPath=configPath)
+                  configPath=configPath,
+                  id=id, key=key)
 
 
-def EduPaperOCR(img_path=None, img_url=None, configPath=None):
+def EduPaperOCR(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
-                  configPath=configPath)
+                  configPath=configPath,
+                  id=id, key=key)
 
 
-def EnglishOCR(img_path=None, img_url=None, configPath=None):
+def EnglishOCR(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
-                  configPath=configPath)
+                  configPath=configPath,
+                  id=id, key=key)
 
 
-def EnterpriseLicenseOCR(img_path=None, img_url=None, configPath=None):
+def EnterpriseLicenseOCR(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
-                  configPath=configPath)
+                  configPath=configPath,
+                  id=id, key=key)
 
 
-def EstateCertOCR(img_path=None, img_url=None, configPath=None):
+def EstateCertOCR(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
-                  configPath=configPath)
+                  configPath=configPath,
+                  id=id, key=key)
 
 
-def FinanBillOCR(img_path=None, img_url=None, configPath=None):
+def FinanBillOCR(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
-                  configPath=configPath)
+                  configPath=configPath,
+                  id=id, key=key)
 
 
-def FinanBillSliceOCR(img_path=None, img_url=None, configPath=None):
+def FinanBillSliceOCR(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
-                  configPath=configPath)
+                  configPath=configPath,
+                  id=id, key=key)
 
 
-def FlightInvoiceOCR(img_path=None, img_url=None, configPath=None):
+def FlightInvoiceOCR(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
-                  configPath=configPath)
+                  configPath=configPath,
+                  id=id, key=key)
 
 
-def FormulaOCR(img_path=None, img_url=None, configPath=None):
+def FormulaOCR(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
-                  configPath=configPath)
+                  configPath=configPath,
+                  id=id, key=key)
 
 
-def GeneralAccurateOCR(img_path=None, img_url=None, configPath=None):
+def GeneralAccurateOCR(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
-                  configPath=configPath)
+                  configPath=configPath,
+                  id=id, key=key)
 
 
-def GeneralBasicOCR(img_path=None, img_url=None, configPath=None):
+def GeneralBasicOCR(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
-                  configPath=configPath)
+                  configPath=configPath,
+                  id=id, key=key)
 
 
-def GeneralEfficientOCR(img_path=None, img_url=None, configPath=None):
+def GeneralEfficientOCR(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
-                  configPath=configPath)
+                  configPath=configPath,
+                  id=id, key=key)
 
 
-def GeneralFastOCR(img_path=None, img_url=None, configPath=None):
+def GeneralFastOCR(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
-                  configPath=configPath)
+                  configPath=configPath,
+                  id=id, key=key)
 
 
-def GeneralHandwritingOCR(img_path=None, img_url=None, configPath=None):
+def GeneralHandwritingOCR(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
-                  configPath=configPath)
+                  configPath=configPath,
+                  id=id, key=key)
 
 
-def HKIDCardOCR(img_path=None, img_url=None, configPath=None):
+def HKIDCardOCR(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
-                  configPath=configPath)
+                  configPath=configPath,
+                  id=id, key=key)
 
 
-def HmtResidentPermitOCR(img_path=None, img_url=None, configPath=None):
+def HmtResidentPermitOCR(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
-                  configPath=configPath)
+                  configPath=configPath,
+                  id=id, key=key)
 
 
-def IDCardOCR(img_path=None, img_url=None, configPath=None):
+def IDCardOCR(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
-                  configPath=configPath)
+                  configPath=configPath,
+                  id=id, key=key)
 
 
-def ImageEnhancement(img_path=None, img_url=None, configPath=None):
+def ImageEnhancement(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
-                  configPath=configPath)
+                  configPath=configPath,
+                  id=id, key=key)
 
 
-def InstitutionOCR(img_path=None, img_url=None, configPath=None):
+def InstitutionOCR(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
-                  configPath=configPath)
+                  configPath=configPath,
+                  id=id, key=key)
 
 
-def InsuranceBillOCR(img_path=None, img_url=None, configPath=None):
+def InsuranceBillOCR(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
-                  configPath=configPath)
+                  configPath=configPath,
+                  id=id, key=key)
 
 
-def InvoiceGeneralOCR(img_path=None, img_url=None, configPath=None):
+def InvoiceGeneralOCR(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
-                  configPath=configPath)
+                  configPath=configPath,
+                  id=id, key=key)
 
 
-def LicensePlateOCR(img_path=None, img_url=None, configPath=None):
+def LicensePlateOCR(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
-                  configPath=configPath)
+                  configPath=configPath,
+                  id=id, key=key)
 
 
-def MLIDCardOCR(img_path=None, img_url=None, configPath=None):
+def MLIDCardOCR(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
-                  configPath=configPath)
+                  configPath=configPath,
+                  id=id, key=key)
 
 
-def MLIDPassportOCR(img_path=None, img_url=None, configPath=None):
+def MLIDPassportOCR(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
-                  configPath=configPath)
+                  configPath=configPath,
+                  id=id, key=key)
 
 
-def MainlandPermitOCR(img_path=None, img_url=None, configPath=None):
+def MainlandPermitOCR(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
-                  configPath=configPath)
+                  configPath=configPath,
+                  id=id, key=key)
 
 
-def MixedInvoiceDetect(img_path=None, img_url=None, configPath=None):
+def MixedInvoiceDetect(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
-                  configPath=configPath)
+                  configPath=configPath,
+                  id=id, key=key)
 
 
-def MixedInvoiceOCR(img_path=None, img_url=None, configPath=None):
+def MixedInvoiceOCR(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
-                  configPath=configPath)
+                  configPath=configPath,
+                  id=id, key=key)
 
 
-def OrgCodeCertOCR(img_path=None, img_url=None, configPath=None):
+def OrgCodeCertOCR(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
-                  configPath=configPath)
+                  configPath=configPath,
+                  id=id, key=key)
 
 
-def PassportOCR(img_path=None, img_url=None, configPath=None):
+def PassportOCR(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
-                  configPath=configPath)
+                  configPath=configPath,
+                  id=id, key=key)
 
 
-def PermitOCR(img_path=None, img_url=None, configPath=None):
+def PermitOCR(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
-                  configPath=configPath)
+                  configPath=configPath,
+                  id=id, key=key)
 
 
-def PropOwnerCertOCR(img_path=None, img_url=None, configPath=None):
+def PropOwnerCertOCR(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
-                  configPath=configPath)
+                  configPath=configPath,
+                  id=id, key=key)
 
 
-def QrcodeOCR(img_path=None, img_url=None, configPath=None):
+def QrcodeOCR(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
-                  configPath=configPath)
+                  configPath=configPath,
+                  id=id, key=key)
 
 
-def QueryBarCode(img_path=None, img_url=None, configPath=None):
+def QueryBarCode(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
-                  configPath=configPath)
+                  configPath=configPath,
+                  id=id, key=key)
 
 
-def QuotaInvoiceOCR(img_path=None, img_url=None, configPath=None):
+def QuotaInvoiceOCR(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
-                  configPath=configPath)
+                  configPath=configPath,
+                  id=id, key=key)
 
 
-def RecognizeContainerOCR(img_path=None, img_url=None, configPath=None):
+def RecognizeContainerOCR(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
-                  configPath=configPath)
+                  configPath=configPath,
+                  id=id, key=key)
 
 
-def RecognizeHealthCodeOCR(img_path=None, img_url=None, configPath=None):
+def RecognizeHealthCodeOCR(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
-                  configPath=configPath)
+                  configPath=configPath,
+                  id=id, key=key)
 
 
-def RecognizeIndonesiaIDCardOCR(img_path=None, img_url=None, configPath=None):
+def RecognizeIndonesiaIDCardOCR(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
-                  configPath=configPath)
+                  configPath=configPath,
+                  id=id, key=key)
 
 
-def RecognizeMedicalInvoiceOCR(img_path=None, img_url=None, configPath=None):
+def RecognizeMedicalInvoiceOCR(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
-                  configPath=configPath)
+                  configPath=configPath,
+                  id=id, key=key)
 
 
-def RecognizeOnlineTaxiItineraryOCR(img_path=None, img_url=None, configPath=None):
+def RecognizeOnlineTaxiItineraryOCR(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
-                  configPath=configPath)
+                  configPath=configPath,
+                  id=id, key=key)
 
 
-def RecognizePhilippinesDrivingLicenseOCR(img_path=None, img_url=None, configPath=None):
+def RecognizePhilippinesDrivingLicenseOCR(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
-                  configPath=configPath)
+                  configPath=configPath,
+                  id=id, key=key)
 
 
-def RecognizePhilippinesVoteIDOCR(img_path=None, img_url=None, configPath=None):
+def RecognizePhilippinesVoteIDOCR(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
-                  configPath=configPath)
+                  configPath=configPath,
+                  id=id, key=key)
 
 
-def RecognizeTableOCR(img_path=None, img_url=None, configPath=None):
+def RecognizeTableOCR(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
-                  configPath=configPath)
+                  configPath=configPath,
+                  id=id, key=key)
 
 
-def RecognizeThaiIDCardOCR(img_path=None, img_url=None, configPath=None):
+def RecognizeThaiIDCardOCR(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
-                  configPath=configPath)
+                  configPath=configPath,
+                  id=id, key=key)
 
 
-def RecognizeTravelCardOCR(img_path=None, img_url=None, configPath=None):
+def RecognizeTravelCardOCR(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
-                  configPath=configPath)
+                  configPath=configPath,
+                  id=id, key=key)
 
 
-def ResidenceBookletOCR(img_path=None, img_url=None, configPath=None):
+def ResidenceBookletOCR(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
-                  configPath=configPath)
+                  configPath=configPath,
+                  id=id, key=key)
 
 
-def RideHailingDriverLicenseOCR(img_path=None, img_url=None, configPath=None):
+def RideHailingDriverLicenseOCR(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
-                  configPath=configPath)
+                  configPath=configPath,
+                  id=id, key=key)
 
 
-def RideHailingTransportLicenseOCR(img_path=None, img_url=None, configPath=None):
+def RideHailingTransportLicenseOCR(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
-                  configPath=configPath)
+                  configPath=configPath,
+                  id=id, key=key)
 
 
-def SealOCR(img_path=None, img_url=None, configPath=None):
+def SealOCR(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
-                  configPath=configPath)
+                  configPath=configPath,
+                  id=id, key=key)
 
 
-def ShipInvoiceOCR(img_path=None, img_url=None, configPath=None):
+def ShipInvoiceOCR(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
-                  configPath=configPath)
+                  configPath=configPath,
+                  id=id, key=key)
 
 
-def SmartStructuralOCR(img_path=None, img_url=None, configPath=None):
+def SmartStructuralOCR(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
-                  configPath=configPath)
+                  configPath=configPath,
+                  id=id, key=key)
 
 
-def TableOCR(img_path=None, img_url=None, configPath=None):
+def TableOCR(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
-                  configPath=configPath)
+                  configPath=configPath,
+                  id=id, key=key)
 
 
-def TaxiInvoiceOCR(img_path=None, img_url=None, configPath=None):
+def TaxiInvoiceOCR(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
-                  configPath=configPath)
+                  configPath=configPath,
+                  id=id, key=key)
 
 
-def TextDetect(img_path=None, img_url=None, configPath=None):
+def TextDetect(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
-                  configPath=configPath)
+                  configPath=configPath,
+                  id=id, key=key)
 
 
-def TollInvoiceOCR(img_path=None, img_url=None, configPath=None):
+def TollInvoiceOCR(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
-                  configPath=configPath)
+                  configPath=configPath,
+                  id=id, key=key)
 
 
-def TrainTicketOCR(img_path=None, img_url=None, configPath=None):
+def TrainTicketOCR(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
-                  configPath=configPath)
+                  configPath=configPath,
+                  id=id, key=key)
 
 
-def VatInvoiceOCR(img_path=None, img_url=None, configPath=None):
+def VatInvoiceOCR(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
-                  configPath=configPath)
+                  configPath=configPath,
+                  id=id, key=key)
 
 
-def VatInvoiceVerify(img_path=None, img_url=None, configPath=None):
+def VatInvoiceVerify(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
-                  configPath=configPath)
+                  configPath=configPath,
+                  id=id, key=key)
 
 
-def VatInvoiceVerifyNew(img_path=None, img_url=None, configPath=None):
+def VatInvoiceVerifyNew(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
-                  configPath=configPath)
+                  configPath=configPath,
+                  id=id, key=key)
 
 
-def VatRollInvoiceOCR(img_path=None, img_url=None, configPath=None):
+def VatRollInvoiceOCR(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
-                  configPath=configPath)
+                  configPath=configPath,
+                  id=id, key=key)
 
 
-def VehicleLicenseOCR(img_path=None, img_url=None, configPath=None):
+def VehicleLicenseOCR(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
-                  configPath=configPath)
+                  configPath=configPath,
+                  id=id, key=key)
 
 
-def VehicleRegCertOCR(img_path=None, img_url=None, configPath=None):
+def VehicleRegCertOCR(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
-                  configPath=configPath)
+                  configPath=configPath,
+                  id=id, key=key)
 
 
-def VerifyBasicBizLicense(img_path=None, img_url=None, configPath=None):
+def VerifyBasicBizLicense(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
-                  configPath=configPath)
+                  configPath=configPath,
+                  id=id, key=key)
 
 
-def VerifyBizLicense(img_path=None, img_url=None, configPath=None):
+def VerifyBizLicense(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
-                  configPath=configPath)
+                  configPath=configPath,
+                  id=id, key=key)
 
 
-def VerifyEnterpriseFourFactors(img_path=None, img_url=None, configPath=None):
+def VerifyEnterpriseFourFactors(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
-                  configPath=configPath)
+                  configPath=configPath,
+                  id=id, key=key)
 
 
-def VerifyOfdVatInvoiceOCR(img_path=None, img_url=None, configPath=None):
+def VerifyOfdVatInvoiceOCR(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
-                  configPath=configPath)
+                  configPath=configPath,
+                  id=id, key=key)
 
 
-def VinOCR(img_path=None, img_url=None, configPath=None):
+def VinOCR(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
-                  configPath=configPath)
+                  configPath=configPath,
+                  id=id, key=key)
 
 
-def WaybillOCR(img_path=None, img_url=None, configPath=None):
+def WaybillOCR(img_path=None, img_url=None, configPath=None, id=None, key=None):
     return do_api(OCR_NAME=str(sys._getframe().f_code.co_name),
                   img_path=img_path,
                   img_url=img_url,
-                  configPath=configPath)
+                  configPath=configPath,
+                  id=id, key=key)
 
-# def VatInvoiceOCR(img_path=None, img_url=None, configPath=None):
+# def VatInvoiceOCR(img_path=None, img_url=None, configPath=None, id=None, key=None):
 #     """
 #     增值税发票的识别
 #     :param img_path: 必填，发票的图片位置
 #     :param configPath: 选填，配置文件的位置，有默认值
 #     :return:
 #     """
 #
 #     ocr = get_ocr(configPath)
 #     if img_url:
 #         ocr_res = ocr.VatInvoiceOCR(ImageBase64=img_path, ImageUrl=img_url)
 #     else:
 #         ImageBase64 = img2base64(img_path)
 #         ocr_res = ocr.VatInvoiceOCR(ImageBase64=ImageBase64, ImageUrl=img_url)
-#     return ocr_res
+#     return ocr_res
```

### Comparing `poocr-0.0.8/poocr/api/ocr2excel.py` & `poocr-0.0.9/poocr/api/ocr2excel.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: UTF-8 -*-
 '''
-@Author  ：B站/抖音/微博/小红书/公众号，都叫：程序员晚枫
-@WeChat     ：CoderWanFeng
-@Blog      ：www.python-office.com
+@作者 ：B站/抖音/微博/小红书/公众号，都叫：程序员晚枫
+@微信 ：CoderWanFeng : https://mp.weixin.qq.com/s/yFcocJbfS9Hs375NhE8Gbw
+@个人网站 ：www.python-office.com
 @Date    ：2023/3/25 18:53 
 @Description     ：
 '''
 import json
 from pathlib import Path
 
 import pandas as pd
```

### Comparing `poocr-0.0.8/poocr/core/OCR.py` & `poocr-0.0.9/poocr/core/OCR.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,42 +2,46 @@
 '''
 @Author  ：程序员晚枫，B站/抖音/微博/小红书/公众号
 @WeChat     ：CoderWanFeng
 @Blog      ：www.python-office.com
 @Date    ：2023/1/22 18:45
 @Description     ：文字识别功能，可以单独调用
 '''
-from poocr.lib.Const import NO_FILE_ERROR
-from poocr.lib.Config import poocrConfig
-
 from tencentcloud.common import credential
 from tencentcloud.common.exception.tencent_cloud_sdk_exception import TencentCloudSDKException
 from tencentcloud.common.profile.client_profile import ClientProfile
 from tencentcloud.common.profile.http_profile import HttpProfile
 from tencentcloud.ocr.v20181119 import ocr_client, models
 
+from poocr.lib.Config import poocrConfig
+from poocr.lib.Const import NO_FILE_ERROR
+
 
 class OCR(poocrConfig):
     def __init__(self):
         self.TENCENT_AI_CFG = None
         self.TENCENTCLOUD_SECRET_ID = None
         self.TENCENTCLOUD_SECRET_KEY = None
         self.CLIENT = None
 
-    def set_config(self, configPath):
+    def set_config(self, configPath, id, key):
         """
-        加载配置信息，生成client
+        加载配置信息，生成client，获取配置信息：
         :param configPath: 可以自定义config文件的名称和位置，有默认值
         :return:
         """
-        self.TENCENT_AI_CFG = self.get_config(configPath)
-        if self.TENCENT_AI_CFG['tencent-ai']['TENCENTCLOUD_SECRET_ID'] and self.TENCENT_AI_CFG['tencent-ai'][
-            'TENCENTCLOUD_SECRET_KEY']:
-            self.TENCENTCLOUD_SECRET_ID = self.TENCENT_AI_CFG['tencent-ai']['TENCENTCLOUD_SECRET_ID']
-            self.TENCENTCLOUD_SECRET_KEY = self.TENCENT_AI_CFG['tencent-ai']['TENCENTCLOUD_SECRET_KEY']
+        if id != None and key != None:
+            self.TENCENTCLOUD_SECRET_ID = id
+            self.TENCENTCLOUD_SECRET_KEY = key
+        else:
+            self.TENCENT_AI_CFG = self.get_config(configPath)
+            if self.TENCENT_AI_CFG['tencent-ai']['TENCENTCLOUD_SECRET_ID'] and self.TENCENT_AI_CFG['tencent-ai'][
+                'TENCENTCLOUD_SECRET_KEY']:
+                self.TENCENTCLOUD_SECRET_ID = self.TENCENT_AI_CFG['tencent-ai']['TENCENTCLOUD_SECRET_ID']
+                self.TENCENTCLOUD_SECRET_KEY = self.TENCENT_AI_CFG['tencent-ai']['TENCENTCLOUD_SECRET_KEY']
         cred = credential.Credential(self.TENCENTCLOUD_SECRET_ID, self.TENCENTCLOUD_SECRET_KEY)
         httpProfile = HttpProfile()
         httpProfile.endpoint = "ocr.tencentcloudapi.com"
         clientProfile = ClientProfile()
         clientProfile.httpProfile = httpProfile
         self.client = ocr_client.OcrClient(cred, "ap-beijing", clientProfile)
         return self.client
@@ -66,15 +70,14 @@
             ocr_func = getattr(self.client, f'{OCR_NAME}', None)
             resp = ocr_func(req)
             return resp
 
         except TencentCloudSDKException as err:
             print(err)
 
-
     # def VatInvoiceOCR(self, ImageBase64, ImageUrl):
     #     """
     #     本接口支持增值税专用发票、增值税普通发票、增值税电子发票全字段的内容检测和识别，
     #     包括发票代码、发票号码、打印发票代码、打印发票号码、开票日期、合计金额、校验码、税率、合计税额、价税合计、购买方识别号、复核、销售方识别号、开票人、密码区1、密码区2、密码区3、密码区4、发票名称、购买方名称、销售方名称、服务名称、备注、规格型号、数量、单价、金额、税额、收款人等字段。
     #
     #     默认接口请求频率限制：10次/秒。
     #     图片的 ImageUrl、ImageBase64 必须提供一个，如果都提供，只使用 ImageUrl。
```

### Comparing `poocr-0.0.8/poocr/lib/CommonUtils.py` & `poocr-0.0.9/poocr/lib/CommonUtils.py`

 * *Files identical despite different names*

### Comparing `poocr-0.0.8/poocr/lib/Config.py` & `poocr-0.0.9/poocr/lib/Config.py`

 * *Files identical despite different names*

### Comparing `poocr-0.0.8/poocr/lib/Const.py` & `poocr-0.0.9/poocr/lib/Const.py`

 * *Files identical despite different names*

### Comparing `poocr-0.0.8/poocr.egg-info/PKG-INFO` & `poocr-0.0.9/poocr.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poocr
-Version: 0.0.8
+Version: 0.0.9
 Summary: pip install poocr
 Home-page: https://www.python-office.com/
 Author: CoderWanFeng
 Author-email: 1957875073@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CoderWanFeng/poocr/issues
 Project-URL: Documentation, https://github.com/CoderWanFeng/poocr/blob/main/README.md
@@ -31,15 +31,15 @@
 </p>
 
 
 <p align="center" name="'github">
   	<a href="https://mp.weixin.qq.com/s/yaSmFKO3RrBpyanW3nvRAQ">
 	<img src="https://img.shields.io/badge/QQ-163434413-orange"/>
   </a>
-    	<a href="https://mp.weixin.qq.com/s/wx-JkgOUoJhb-7ZESxl93w">
+    	<a href="https://mp.weixin.qq.com/s/NN2pX2bQPpczOeGF4ARNtw">
 	<img src="https://img.shields.io/badge/%E5%BE%AE%E4%BF%A1-%E4%BA%A4%E6%B5%81%E7%BE%A4-brightgreen"/>
   </a>
 </p>
 
 
 -------------------------------------------------------------------------------
 
@@ -64,15 +64,15 @@
 ```
 
 
 -------------------------------------------------------------------------------
 
 ## 📝功能
 
-- [📘官网：https://www.python-office.com/](https://www.python-office.com/)
+- [📘Python自动化办公的官网：https://www.python-office.com/](https://www.python-office.com/)
 
 -  💻所有功能的列表👉[点我直达](https://www.python-office.com/video/poocr.html)
 
 
 ## 常见问题
 
 1. 如何配置poocr-config.toml？
@@ -107,8 +107,12 @@
 
 -------------------------------------------------------------------------------
 
 
 ## 📌联系作者
 
 
-![CoderWanFeng](https://python-office-1300615378.cos.ap-chongqing.myqcloud.com/python-office-qr.jpg)
+<p align="center" id='开源交流群-banner'>
+<a target="_blank" href='https://python-office-1300615378.cos.ap-chongqing.myqcloud.com/python-office.jpg'>
+<img src="https://python-office-1300615378.cos.ap-chongqing.myqcloud.com/python-office-qr.jpg" width="100%"/>
+</a> 
+</p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: poocr Version: 0.0.8 Summary: pip install poocr
+Metadata-Version: 2.1 Name: poocr Version: 0.0.9 Summary: pip install poocr
 Home-page: https://www.python-office.com/ Author: CoderWanFeng Author-email:
 1957875073@qq.com License: MIT Project-URL: Bug Tracker, https://github.com/
 CoderWanFeng/poocr/issues Project-URL: Documentation, https://github.com/
 CoderWanFeng/poocr/blob/main/README.md Project-URL: Source Code, https://
 github.com/CoderWanFeng/poocr Platform: any Requires-Python: >=3.7 Description-
 Content-Type: text/markdown License-File: LICENSE
 [https://website-python-1300615378.cos.ap-nanjing.myqcloud.com/ads%2F1040x100-
@@ -15,17 +15,18 @@
 - ## ðç®ä» poocr æ¯å¿«éè°ç¨è¾è®¯äºAIå¹³å°åè½çæ¥å£åéã
 ``poocr``ææåè½çå®ç°ï¼é½ä¾æäºè¾è®¯äºçæå­è¯å«ï¼å¦ææ¯å°ç½ç¨æ·ï¼å¯ä»¥**æ«ç ä¸å¾ï¼åè´¹å¼é**~
 ![](https://article-1300615378.cos.ap-nanjing.myqcloud.com/potencent%2Fapi-
 doc%2Fshare.jpg) --------------------------------------------------------------
 ----------------- ## ð¦å®è£ ### ðpip èªå¨ä¸è½½&æ´æ° ``` pip install
 -i https://mirrors.aliyun.com/pypi/simple/ poocr -U ``` -----------------------
 -------------------------------------------------------- ## ðåè½ -
-[ðå®ç½ï¼https://www.python-office.com/](https://www.python-office.com/) -
-ð»ææåè½çåè¡¨ð[ç¹æç´è¾¾](https://www.python-office.com/
-video/poocr.html) ## å¸¸è§é®é¢ 1. å¦ä½éç½®poocr-config.tomlï¼
+[ðPythonèªå¨ååå¬çå®ç½ï¼https://www.python-office.com/](https://
+www.python-office.com/) - ð»ææåè½çåè¡¨ð[ç¹æç´è¾¾](https://
+www.python-office.com/video/poocr.html) ## å¸¸è§é®é¢ 1. å¦ä½éç½®poocr-
+config.tomlï¼
 ç¬¬ä¸æ­¥ï¼ä½ éè¦å¼éè¾è®¯äºçåç¥¨è¯å«åè½ï¼æ¶è´¹åè½ï¼å¾ä¾¿å®ï¼ï¼
 [ç¹æç´è¾¾](https://cloud.tencent.com/act/cps/
 redirect?redirect=10098&cps_key=ca76be5a2293ba3906d6d5407aea15ee)
 ç¬¬äºæ­¥ï¼ä½ éè¦è®¾ç½®ä¸ä¸ªå­è´¦æ·ï¼ä¸è±é±ï¼ï¼[ç¹æç´è¾¾]
 (https://cloud.tencent.com/act/cps/
 redirect?redirect=36394&cps_key=ca76be5a2293ba3906d6d5407aea15ee)
 å¦æä»¥ä¸éç½®ï¼èªå·±ä¸æææ¯ï¼é¾ä»¥å®ç°çè¯ï¼å¯ä»¥ä»è´¹æ¾æå¸®ä½ éç½®ãæçå¾®ä¿¡ï¼ç¹å»ç´è¾¾ð
@@ -40,9 +41,10 @@
 ç»å½GiteeæGithubå¨ä½ é¦é¡µå¯ä»¥çå°ä¸ä¸ª pull request
 æé®ï¼ç¹å»å®ï¼å¡«åä¸äºè¯´æä¿¡æ¯ï¼ç¶åæäº¤å°masteråæ¯å³å¯ã
 6. ç­å¾ç»´æ¤èåå¹¶ ### ðæä¾bugåé¦æå»ºè®®
 æäº¤é®é¢åé¦æ¶ï¼è¯·å¡å¿å¡«ååpython-
 officeä»£ç æ¬èº«æå³çé®é¢ï¼ä¸è¿è¡æå³pythonå­¦ä¹ ï¼çè³æ¯ä¸ªäººç»ä¹ çç¥è¯ç­çåè®¨è®ºã
 - [Github issue](https://github.com/CoderWanFeng/pobaidu/issues) --------------
 ----------------------------------------------------------------- ##
-ðèç³»ä½è ![CoderWanFeng](https://python-office-1300615378.cos.ap-
-chongqing.myqcloud.com/python-office-qr.jpg)
+ðèç³»ä½è
+[https://python-office-1300615378.cos.ap-chongqing.myqcloud.com/python-office-
+                                    qr.jpg]
```

### Comparing `poocr-0.0.8/setup.cfg` & `poocr-0.0.9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 6f6f 6372 0d0a 7665 7273 696f   = poocr..versio
-00000020: 6e20 3d20 302e 302e 380d 0a64 6573 6372  n = 0.0.8..descr
+00000020: 6e20 3d20 302e 302e 390d 0a64 6573 6372  n = 0.0.9..descr
 00000030: 6970 7469 6f6e 203d 2070 6970 2069 6e73  iption = pip ins
 00000040: 7461 6c6c 2070 6f6f 6372 0d0a 6c6f 6e67  tall poocr..long
 00000050: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
 00000060: 696c 653a 2052 4541 444d 452e 6d64 0d0a  ile: README.md..
 00000070: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 00000080: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type = 
 00000090: 7465 7874 2f6d 6172 6b64 6f77 6e0d 0a75  text/markdown..u
```

### Comparing `poocr-0.0.8/tests/test_tencent.py` & `poocr-0.0.9/tests/test_tencent.py`

 * *Files identical despite different names*

