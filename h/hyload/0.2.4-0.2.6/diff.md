# Comparing `tmp/hyload-0.2.4-py3-none-any.whl.zip` & `tmp/hyload-0.2.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 27368 bytes, number of entries: 17
+Zip file size: 27493 bytes, number of entries: 17
 -rw-rw-rw-  2.0 fat      171 b- defN 23-Jul-19 05:41 hyload/__init__.py
--rw-rw-rw-  2.0 fat       17 b- defN 23-Jul-22 23:53 hyload/cfg.py
+-rw-rw-rw-  2.0 fat       17 b- defN 23-Jul-25 10:57 hyload/cfg.py
 -rw-rw-rw-  2.0 fat    19401 b- defN 23-Jul-23 00:11 hyload/httpclient.py
 -rw-rw-rw-  2.0 fat     2627 b- defN 23-Jul-23 00:12 hyload/logger.py
--rw-rw-rw-  2.0 fat    11344 b- defN 23-Jul-23 00:16 hyload/stats.py
+-rw-rw-rw-  2.0 fat    11771 b- defN 23-Jul-23 23:50 hyload/stats.py
 -rw-rw-rw-  2.0 fat      979 b- defN 23-Jul-08 14:54 hyload/util.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jul-08 14:54 hyload/tools/__init__.py
 -rw-rw-rw-  2.0 fat     3667 b- defN 23-Jul-08 14:54 hyload/tools/plotperf.py
 -rw-rw-rw-  2.0 fat     2802 b- defN 23-Jul-08 14:54 hyload/tools/plotresource.py
 -rw-rw-rw-  2.0 fat    39521 b- defN 23-Jul-08 14:54 hyload/tools/puttyagents.py
 -rw-rw-rw-  2.0 fat     4007 b- defN 23-Jul-21 06:07 hyload/tools/remoteop.py
 -rw-rw-rw-  2.0 fat     7493 b- defN 23-Jul-14 12:12 hyload/tools/statshub.py
--rw-rw-rw-  2.0 fat     1100 b- defN 23-Jul-23 01:45 hyload-0.2.4.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     1509 b- defN 23-Jul-23 01:45 hyload-0.2.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-23 01:45 hyload-0.2.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 23-Jul-23 01:45 hyload-0.2.4.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1311 b- defN 23-Jul-23 01:45 hyload-0.2.4.dist-info/RECORD
-17 files, 96048 bytes uncompressed, 25244 bytes compressed:  73.7%
+-rw-rw-rw-  2.0 fat     1100 b- defN 23-Jul-25 10:58 hyload-0.2.6.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     1509 b- defN 23-Jul-25 10:58 hyload-0.2.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-25 10:58 hyload-0.2.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 23-Jul-25 10:58 hyload-0.2.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1311 b- defN 23-Jul-25 10:58 hyload-0.2.6.dist-info/RECORD
+17 files, 96475 bytes uncompressed, 25369 bytes compressed:  73.7%
```

## zipnote {}

```diff
@@ -30,23 +30,23 @@
 
 Filename: hyload/tools/remoteop.py
 Comment: 
 
 Filename: hyload/tools/statshub.py
 Comment: 
 
-Filename: hyload-0.2.4.dist-info/LICENSE.txt
+Filename: hyload-0.2.6.dist-info/LICENSE.txt
 Comment: 
 
-Filename: hyload-0.2.4.dist-info/METADATA
+Filename: hyload-0.2.6.dist-info/METADATA
 Comment: 
 
-Filename: hyload-0.2.4.dist-info/WHEEL
+Filename: hyload-0.2.6.dist-info/WHEEL
 Comment: 
 
-Filename: hyload-0.2.4.dist-info/top_level.txt
+Filename: hyload-0.2.6.dist-info/top_level.txt
 Comment: 
 
-Filename: hyload-0.2.4.dist-info/RECORD
+Filename: hyload-0.2.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hyload/cfg.py

```diff
@@ -1 +1 @@
-Version = '0.2.4'
+Version = '0.2.6'
```

## hyload/stats.py

```diff
@@ -1,13 +1,15 @@
 from hyload.util import getCurTime
 import time,sys,json,socket,os,gevent
 import http.client
 from urllib.parse import quote_plus
 from .logger import TestLogger
 from typing import Union
+from datetime import datetime
+from random import randint
 
 class bcolors:
     HEADER = '\033[95m'
     OKBLUE = '\033[94m'
     OKCYAN = '\033[96m'
     OKGREEN = '\033[92m'
     YELLOW = '\033[33m'
@@ -23,38 +25,32 @@
             value = arg.replace(f'{argName}=','')
             return value
     
     return None
 
 # 控制台程序地址
 ConsoleAddr = getCommandArg('console')
-
-# 统计数据文件
-StatsFile = getCommandArg('statsfile')
-
 if ConsoleAddr:
     # print (f'Console addr:{ConsoleAddr}')
     # consoleConnection = http.client.HTTPConnection(
     #                             ConsoleAddr,  #ConsoleAddr 'httpbin.org'
     #                             timeout=0.3)
 
     # Create a UDP socket at client side
 
     UDPClientSocket = socket.socket(family=socket.AF_INET, type=socket.SOCK_DGRAM)
     parts = ConsoleAddr.split(':')
     UDPServerAddr = parts[0],int(parts[1])
     # print(UDPServerAddr)
 
-if StatsFile:
-    statsDir = os.path.dirname(StatsFile)
-    if statsDir:
-        os.makedirs(statsDir,exist_ok=True)
-    foStats = open(StatsFile,'wb')
+
+
 
 class Stats:
+    foStats = None
     
     @staticmethod
     def wait_for_tasks_done(tasks:list=None):
         gevent.wait(tasks) # wait for tasks end
         time.sleep(1) # wait for stats routine to send last second stats
         print('\n==== 运行结束 ====')
 
@@ -230,27 +226,42 @@
         # 统计对象数据序列化为字节
         statsBytes = json.dumps(statsOneSecond).encode()
 
         # 发给console集中显示
         if ConsoleAddr:
             cls._sendStatsToConsoleUdp(statsBytes)
 
-        if StatsFile:
-            foStats.write(statsBytes+b'\n')
-            foStats.flush()
+        if cls.foStats:
+            cls.foStats.write(statsBytes+b'\n')
+            cls.foStats.flush()
 
         # 发送到 console的 并发连接数量 数据
         # 目前侦测到连接断开比较麻烦，暂时先不做并发连接的统计
         # cls._sendStatsToConsoleUdp({'connNum':cls.connectionNumber})
 
     @classmethod
     def start(cls):
         """
         Run stats routine.
         """
+
+        # 统计数据文件
+        statsfile = getCommandArg('statsfile')
+        if not statsfile:  
+            statsfile = os.path.join(
+                'stats_perf', 
+                datetime.now().strftime('%Y-%m-%d_%H.%M.%S.%f')[:23].replace("-0", "-") + '.sts')
+        
+        statsDir = os.path.dirname(statsfile)
+        if statsDir:
+            os.makedirs(statsDir,exist_ok=True)
+        cls.foStats = open(statsfile,'wb')
+
+        
+
         cls.clear()
         cls.runFlag = True  # 启动标识
 
         gevent.spawn(cls._independent_check)
 
                 
     # 独立检查协程，检查上一秒统计数据是否发出了
@@ -280,14 +291,18 @@
         """
         Stop stats routine.
         """
         # wait for more than 1 second, so stats greenlet could count last second
         time.sleep(1.2)
         cls.runFlag = False
 
+        if cls.foStats:
+            cls.foStats.close()
+            cls.foStats = None
+
     # 更新 以秒为单位的统计表
     @classmethod
     def _measure_per_second(cls, recTable, addAmount, curTime=None):
         
         if curTime is None:
             curTime = getCurTime()
```

## Comparing `hyload-0.2.4.dist-info/LICENSE.txt` & `hyload-0.2.6.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `hyload-0.2.4.dist-info/METADATA` & `hyload-0.2.6.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyload
-Version: 0.2.4
+Version: 0.2.6
 Summary: Framework for load testing
 Home-page: http://www.byhy.net
 Download-URL: https://pypi.python.org/pypi/hyload
 Author: baiyueheiyu 白月黑羽
 Author-email: jcyrss@gmail.com
 License: Apache License 2.0
 Keywords: hyload loadtesting
```

## Comparing `hyload-0.2.4.dist-info/RECORD` & `hyload-0.2.6.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 hyload/__init__.py,sha256=wXjdLCvcOlQV8a7Mku2cQbyWRXheGf7dGkHfjvBqKu8,171
-hyload/cfg.py,sha256=cdNJF8QEyAN-FijrgwJpayHDazweFlMrOghMDR5x47w,17
+hyload/cfg.py,sha256=o9buJSZqLK87y7pzqM6v4uXwbX6dEUO6vdeGbsg4uBc,17
 hyload/httpclient.py,sha256=8fjF_T6i8q4Y1HEVKv97Qdn14SgdpqFBnDbup3RtAr4,19401
 hyload/logger.py,sha256=CfxUQM7oPiWuiuXmtiQiD5ViXkdY1t5yo8-SvRWO1q8,2627
-hyload/stats.py,sha256=eiC1a-c-_QBXqE5LUKEbCZcSPQLZyIARwPGk3BKBG74,11344
+hyload/stats.py,sha256=1BCif-2OTVWEPvSMEIxY_WoJQ0v7I2WxJlkLAXDoIxA,11771
 hyload/util.py,sha256=lNKVVW4vYFueXcvOC4HoIMIiXFUz6skR9shSA7iPsWU,979
 hyload/tools/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 hyload/tools/plotperf.py,sha256=H1OszxmfgAYAxX4YEp-_aX66w6slynz9tjDGdpraMMo,3667
 hyload/tools/plotresource.py,sha256=9ydos2xFSA__ANhQ4b_fr5ORJPwWVLCgXoYnYdO5cA4,2802
 hyload/tools/puttyagents.py,sha256=NvL3VhYYka69kh7QTdRzjm7dLN3dB5MuU__K1GmGsW8,39521
 hyload/tools/remoteop.py,sha256=eJ7gSwJNzNIZfOU--5F_MNiy8laA9EBqIXtsuE83ZH8,4007
 hyload/tools/statshub.py,sha256=bPyj9h6eewxRJSJmQpqtkx3DFbvoYbQsWpcFvATFang,7493
-hyload-0.2.4.dist-info/LICENSE.txt,sha256=OGhxEO0MAMle3LEQV8Us5uo4C8pk-jWmCBKyQ7U_gCE,1100
-hyload-0.2.4.dist-info/METADATA,sha256=Yx6QaPhZosD0qVlOfbEOXmsnLPcOPP-4ES459-PFQ1o,1509
-hyload-0.2.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-hyload-0.2.4.dist-info/top_level.txt,sha256=ivEyc-v2p5WU0itBl-u9QARFubEqBlHfczIhYbuD_U8,7
-hyload-0.2.4.dist-info/RECORD,,
+hyload-0.2.6.dist-info/LICENSE.txt,sha256=OGhxEO0MAMle3LEQV8Us5uo4C8pk-jWmCBKyQ7U_gCE,1100
+hyload-0.2.6.dist-info/METADATA,sha256=JwVE1kkckhxtR9Lqese-ClWYoZOAToF0ft_V2Onkkhw,1509
+hyload-0.2.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+hyload-0.2.6.dist-info/top_level.txt,sha256=ivEyc-v2p5WU0itBl-u9QARFubEqBlHfczIhYbuD_U8,7
+hyload-0.2.6.dist-info/RECORD,,
```

