# Comparing `tmp/AZMusicAPI-0.9.8.tar.gz` & `tmp/AZMusicAPI-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AZMusicAPI-0.9.8.tar", last modified: Mon Jul 24 11:37:00 2023, max compression
+gzip compressed data, was "AZMusicAPI-1.0.2.tar", last modified: Tue Jul 25 06:33:39 2023, max compression
```

## Comparing `AZMusicAPI-0.9.8.tar` & `AZMusicAPI-1.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 11:37:00.419615 AZMusicAPI-0.9.8/
-drwxrwxrwx   0        0        0        0 2023-07-24 11:37:00.391283 AZMusicAPI-0.9.8/AZMusicAPI/
--rw-rw-rw-   0        0        0     4486 2023-07-24 03:33:51.000000 AZMusicAPI-0.9.8/AZMusicAPI/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 11:37:00.413332 AZMusicAPI-0.9.8/AZMusicAPI.egg-info/
--rw-rw-rw-   0        0        0     1526 2023-07-24 11:37:00.000000 AZMusicAPI-0.9.8/AZMusicAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      200 2023-07-24 11:37:00.000000 AZMusicAPI-0.9.8/AZMusicAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 11:37:00.000000 AZMusicAPI-0.9.8/AZMusicAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-24 11:37:00.000000 AZMusicAPI-0.9.8/AZMusicAPI.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-24 11:37:00.000000 AZMusicAPI-0.9.8/AZMusicAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1526 2023-07-24 11:37:00.417374 AZMusicAPI-0.9.8/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-24 11:37:00.419615 AZMusicAPI-0.9.8/setup.cfg
--rw-rw-rw-   0        0        0      517 2023-07-24 11:36:47.000000 AZMusicAPI-0.9.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 06:33:39.152103 AZMusicAPI-1.0.2/
+drwxrwxrwx   0        0        0        0 2023-07-25 06:33:39.088105 AZMusicAPI-1.0.2/AZMusicAPI/
+-rw-rw-rw-   0        0        0     4639 2023-07-25 06:29:11.000000 AZMusicAPI-1.0.2/AZMusicAPI/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 06:33:39.138103 AZMusicAPI-1.0.2/AZMusicAPI.egg-info/
+-rw-rw-rw-   0        0        0     1643 2023-07-25 06:33:38.000000 AZMusicAPI-1.0.2/AZMusicAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      200 2023-07-25 06:33:38.000000 AZMusicAPI-1.0.2/AZMusicAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 06:33:38.000000 AZMusicAPI-1.0.2/AZMusicAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-25 06:33:38.000000 AZMusicAPI-1.0.2/AZMusicAPI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-25 06:33:38.000000 AZMusicAPI-1.0.2/AZMusicAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1643 2023-07-25 06:33:39.150101 AZMusicAPI-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-25 06:33:39.152103 AZMusicAPI-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      517 2023-07-25 06:30:29.000000 AZMusicAPI-1.0.2/setup.py
```

### Comparing `AZMusicAPI-0.9.8/AZMusicAPI/__init__.py` & `AZMusicAPI-1.0.2/AZMusicAPI/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import requests
 
 # AZ Studio版权所有
 # 该项目仅供娱乐 请勿用于违法事业 违者与AZ Studio无关
 
-def getmusic(keyword):
+def getmusic(keyword,number=20):
+    number=int(number)
     #获得指定关键词的歌曲 关键词可为 歌手/歌曲名/专辑名
-    #keyword：关键词
+    #keyword：关键词 number:返回歌曲数量,可选,默认20
     #返回值说明：正常返回列表  "Error 0"：没有结果 "Error 1":用户未输入
     headers = {
         "Accept": "application/json, text/plain, */*",
         "Accept-Encoding": "gzip, deflate, br",
         "Accept-Language": "zh-CN,zh;q=0.9",
         "Connection": "keep-alive",
         "Cookie": "Hm_lvt_cdb524f42f0ce19b169a8071123a4797=1690028471; _ga=GA1.2.291025627.1690028471; _gid=GA1.2.1906759595.1690028471; SL_G_WPT_TO=zh; SL_GWPT_Show_Hide_tmp=1; SL_wptGlobTipTmp=1; Hm_lpvt_cdb524f42f0ce19b169a8071123a4797=1690028564; _gat=1; Hm_Iuvt_cdb524f42f0ce19b169b8072123a4727=WjT5ktibAJwfEFyQFeJAEFcTxpwYHCeK; _ga_ETPBRPM9ML=GS1.2.1690028471.1.1.1690028577.47.0.0",
@@ -36,23 +37,25 @@
     if len(keyword)>0:
         response_data = requests.get(search_url, params=search_data, headers=headers, timeout=20).json()
         songs_data = response_data['data']['list']
         if int(response_data['data']['total']) <= 0:
             return "Error 0"
         else:
             data=[]
-            for i in range(len(songs_data)):      
+            w_r=len(songs_data)-number
+            number=len(songs_data)-w_r
+            for i in range(number):      
                 try:       
                     data.append({"songname":songs_data[i]['name'],"singer":songs_data[i]['artist'],"album":songs_data[i]['album'],"pic":songs_data[i]['albumpic'],"rid":songs_data[i]['rid'],"reqId":response_data['reqId']})
                 except:
-                    pass                                                                        
+                    continue                                                                        
             return data
     else:
         return "Error 1"
-
+    
 def geturl(rid,reqId):
     #获取音乐的音频地址
     #rid:你要解析的歌曲在getmusic返回的rid reqId:你要解析的歌曲在getmusic返回的reqId
     #返回值：正常返回音频链接 "Error 3":歌曲需要单曲付费或rid/reqId不正确
     headers = {
         "Accept": "application/json, text/plain, */*",
         "Accept-Encoding": "gzip, deflate, br",
@@ -72,8 +75,8 @@
     }
     music_url = 'https://www.kuwo.cn/api/v1/www/music/playUrl?mid={}&type=music&httpsStatus=1&reqId={}&plat=web_www&from='.format(rid, reqId)
     response_data = requests.get(music_url,headers=headers).json()
     try:
         song_url = response_data['data'].get('url')
     except:
         return "Error 3"
-    return song_url
+    return song_url
```

### Comparing `AZMusicAPI-0.9.8/AZMusicAPI.egg-info/PKG-INFO` & `AZMusicAPI-1.0.2/AZMusicAPI.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,52 +1,59 @@
 Metadata-Version: 2.1
 Name: AZMusicAPI
-Version: 0.9.8
+Version: 1.0.2
 Summary: 轻松访问音乐信息和歌曲音频链接 | Easy access to music information and song audio links
 Author: AZ Studio
 Project-URL: GitHub, https://github.com/AZ-Studio-2023/AZMusicAPI/
 Description-Content-Type: text/markdown
 
 # AZMusicAPI
 轻松访问音乐信息和歌曲音频链接 | Easy access to music information and song audio links
 
-# AZ Studio版权所有
-# 该项目仅供娱乐 请勿用于违法事业 违者与AZ Studio无关
+### AZ Studio版权所有
+### 该项目仅供娱乐 请勿用于违法事业 违者与AZ Studio无关
 
-# 安装
+# AZMusicAPI模块使用指南
+
+## 安装
 
 ```pip install AZMusicAPI```
 
-# AZMusicAPI模块使用指南
+## 导入
+
+``` import AZMusicAPI```
+
+## 函数使用
+
 
 ```
-AZMusicAPI.getmusic(keyword)
+AZMusicAPI.getmusic(keyword,number)
 ```
 
-## 作用：获得指定关键词的歌曲
+### 作用：获得指定关键词的歌曲
 
-* keyword：关键词
+* keyword：关键词 number:返回歌曲数量,可选,默认20
 
 * 关键词可为 歌手/歌曲名/专辑名
 
 ### 返回值说明：正常返回列表  "Error 0"：没有结果 "Error 1":用户未输入
 
 ```
 AZMusicAPI.geturl(rid,reqId)
 ```
 
-## 作用：获取音乐的音频地址
+### 作用：获取音乐的音频地址
 
 * rid:你要解析的歌曲在getmusic返回的rid    
 * reqId:你要解析的歌曲在getmusic返回的reqId
 
 ### 返回值：正常返回音频链接 "Error 3":歌曲需要单曲付费或rid/reqId不正确
 
 ## 代码示例
-#### 仅需7行代码即可完成一个音乐音频地址获取器
+### 仅需7行代码即可完成一个音乐音频地址获取器
 
 ```
 import AZMusicAPI as MusicAPI 
 u=input("请输入您需要的歌曲名称：")
 data=MusicAPI.getmusic(u)
 song=data[0]["songname"]
 singer=data[0]["singer"]
```

### Comparing `AZMusicAPI-0.9.8/PKG-INFO` & `AZMusicAPI-1.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,52 +1,59 @@
 Metadata-Version: 2.1
 Name: AZMusicAPI
-Version: 0.9.8
+Version: 1.0.2
 Summary: 轻松访问音乐信息和歌曲音频链接 | Easy access to music information and song audio links
 Author: AZ Studio
 Project-URL: GitHub, https://github.com/AZ-Studio-2023/AZMusicAPI/
 Description-Content-Type: text/markdown
 
 # AZMusicAPI
 轻松访问音乐信息和歌曲音频链接 | Easy access to music information and song audio links
 
-# AZ Studio版权所有
-# 该项目仅供娱乐 请勿用于违法事业 违者与AZ Studio无关
+### AZ Studio版权所有
+### 该项目仅供娱乐 请勿用于违法事业 违者与AZ Studio无关
 
-# 安装
+# AZMusicAPI模块使用指南
+
+## 安装
 
 ```pip install AZMusicAPI```
 
-# AZMusicAPI模块使用指南
+## 导入
+
+``` import AZMusicAPI```
+
+## 函数使用
+
 
 ```
-AZMusicAPI.getmusic(keyword)
+AZMusicAPI.getmusic(keyword,number)
 ```
 
-## 作用：获得指定关键词的歌曲
+### 作用：获得指定关键词的歌曲
 
-* keyword：关键词
+* keyword：关键词 number:返回歌曲数量,可选,默认20
 
 * 关键词可为 歌手/歌曲名/专辑名
 
 ### 返回值说明：正常返回列表  "Error 0"：没有结果 "Error 1":用户未输入
 
 ```
 AZMusicAPI.geturl(rid,reqId)
 ```
 
-## 作用：获取音乐的音频地址
+### 作用：获取音乐的音频地址
 
 * rid:你要解析的歌曲在getmusic返回的rid    
 * reqId:你要解析的歌曲在getmusic返回的reqId
 
 ### 返回值：正常返回音频链接 "Error 3":歌曲需要单曲付费或rid/reqId不正确
 
 ## 代码示例
-#### 仅需7行代码即可完成一个音乐音频地址获取器
+### 仅需7行代码即可完成一个音乐音频地址获取器
 
 ```
 import AZMusicAPI as MusicAPI 
 u=input("请输入您需要的歌曲名称：")
 data=MusicAPI.getmusic(u)
 song=data[0]["songname"]
 singer=data[0]["singer"]
```

### Comparing `AZMusicAPI-0.9.8/setup.py` & `AZMusicAPI-1.0.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='AZMusicAPI',
-    version='0.9.8',
+    version='1.0.2',
     author='AZ Studio',
     description='轻松访问音乐信息和歌曲音频链接 | Easy access to music information and song audio links',
     long_description = open('readme.md', encoding='utf-8').read(),
     long_description_content_type="text/markdown",
     packages=['AZMusicAPI'],
     install_requires=['requests'],
     project_urls={
```

