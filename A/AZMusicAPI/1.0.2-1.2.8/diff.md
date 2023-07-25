# Comparing `tmp/AZMusicAPI-1.0.2.tar.gz` & `tmp/AZMusicAPI-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AZMusicAPI-1.0.2.tar", last modified: Tue Jul 25 06:33:39 2023, max compression
+gzip compressed data, was "AZMusicAPI-1.2.8.tar", last modified: Tue Jul 25 08:02:50 2023, max compression
```

## Comparing `AZMusicAPI-1.0.2.tar` & `AZMusicAPI-1.2.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 06:33:39.152103 AZMusicAPI-1.0.2/
-drwxrwxrwx   0        0        0        0 2023-07-25 06:33:39.088105 AZMusicAPI-1.0.2/AZMusicAPI/
--rw-rw-rw-   0        0        0     4639 2023-07-25 06:29:11.000000 AZMusicAPI-1.0.2/AZMusicAPI/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 06:33:39.138103 AZMusicAPI-1.0.2/AZMusicAPI.egg-info/
--rw-rw-rw-   0        0        0     1643 2023-07-25 06:33:38.000000 AZMusicAPI-1.0.2/AZMusicAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      200 2023-07-25 06:33:38.000000 AZMusicAPI-1.0.2/AZMusicAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 06:33:38.000000 AZMusicAPI-1.0.2/AZMusicAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-25 06:33:38.000000 AZMusicAPI-1.0.2/AZMusicAPI.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-25 06:33:38.000000 AZMusicAPI-1.0.2/AZMusicAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1643 2023-07-25 06:33:39.150101 AZMusicAPI-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-25 06:33:39.152103 AZMusicAPI-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      517 2023-07-25 06:30:29.000000 AZMusicAPI-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 08:02:50.955143 AZMusicAPI-1.2.8/
+drwxrwxrwx   0        0        0        0 2023-07-25 08:02:50.412083 AZMusicAPI-1.2.8/AZMusicAPI/
+-rw-rw-rw-   0        0        0     6865 2023-07-25 07:58:48.000000 AZMusicAPI-1.2.8/AZMusicAPI/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 08:02:50.942062 AZMusicAPI-1.2.8/AZMusicAPI.egg-info/
+-rw-rw-rw-   0        0        0     1856 2023-07-25 08:02:47.000000 AZMusicAPI-1.2.8/AZMusicAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      200 2023-07-25 08:02:48.000000 AZMusicAPI-1.2.8/AZMusicAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 08:02:47.000000 AZMusicAPI-1.2.8/AZMusicAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-25 08:02:47.000000 AZMusicAPI-1.2.8/AZMusicAPI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-25 08:02:47.000000 AZMusicAPI-1.2.8/AZMusicAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1856 2023-07-25 08:02:50.954170 AZMusicAPI-1.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-25 08:02:50.956145 AZMusicAPI-1.2.8/setup.cfg
+-rw-rw-rw-   0        0        0      517 2023-07-25 08:02:14.000000 AZMusicAPI-1.2.8/setup.py
```

### Comparing `AZMusicAPI-1.0.2/AZMusicAPI/__init__.py` & `AZMusicAPI-1.2.8/AZMusicAPI/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -25,37 +25,38 @@
         "sec-ch-ua-mobile": "?0",
         "sec-ch-ua-platform": "\"Windows\""
     }
     search_url = 'https://www.kuwo.cn/api/www/search/searchMusicBykeyWord?'
     search_data = {
         'key': keyword,
         'pn': '1',
-        'rn': '20',
+        'rn': number,
         'httpsStatus': '1',
         'reqId': '7d9e2c60-288a-11ee-9cdf-3f476f1ba25e',
         "plat":"web_www"
     }
     if len(keyword)>0:
-        response_data = requests.get(search_url, params=search_data, headers=headers, timeout=20).json()
+        try:
+            response_data = requests.get(search_url, params=search_data, headers=headers, timeout=20).json()
+        except:
+            return "NetError"
         songs_data = response_data['data']['list']
         if int(response_data['data']['total']) <= 0:
             return "Error 0"
         else:
             data=[]
-            w_r=len(songs_data)-number
-            number=len(songs_data)-w_r
-            for i in range(number):      
+            for i in range(len(songs_data)):      
                 try:       
                     data.append({"songname":songs_data[i]['name'],"singer":songs_data[i]['artist'],"album":songs_data[i]['album'],"pic":songs_data[i]['albumpic'],"rid":songs_data[i]['rid'],"reqId":response_data['reqId']})
                 except:
                     continue                                                                        
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
@@ -70,13 +71,61 @@
         "Secret": "09362e5991f0846bff719a26e1a0e0ac7bd0b3c9f8ab5fdf000c7b88ecfa727000a0ba6e",
         "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36",
         "sec-ch-ua": "\"Not.A/Brand\";v=\"8\", \"Chromium\";v=\"114\", \"Google Chrome\";v=\"114\"",
         "sec-ch-ua-mobile": "?0",
         "sec-ch-ua-platform": "\"Windows\""
     }
     music_url = 'https://www.kuwo.cn/api/v1/www/music/playUrl?mid={}&type=music&httpsStatus=1&reqId={}&plat=web_www&from='.format(rid, reqId)
-    response_data = requests.get(music_url,headers=headers).json()
+    try:
+        response_data = requests.get(music_url,headers=headers).json()
+    except:
+        return "NetError"
     try:
         song_url = response_data['data'].get('url')
     except:
         return "Error 3"
-    return song_url
+    return song_url
+
+def searchkey(value):
+    #通过关键字得到音乐/歌手/专辑名
+    #value:关键字
+    headers = {
+        "Accept": "application/json, text/plain, */*",
+        "Accept-Encoding": "gzip, deflate, br",
+        "Accept-Language": "zh-CN,zh;q=0.9",
+        "Connection": "keep-alive",
+        "Cookie": "Hm_lvt_cdb524f42f0ce19b169a8071123a4797=1690028471; _ga=GA1.2.291025627.1690028471; _gid=GA1.2.1906759595.1690028471; SL_G_WPT_TO=zh; SL_GWPT_Show_Hide_tmp=1; SL_wptGlobTipTmp=1; Hm_lpvt_cdb524f42f0ce19b169a8071123a4797=1690028564; _gat=1; Hm_Iuvt_cdb524f42f0ce19b169b8072123a4727=WjT5ktibAJwfEFyQFeJAEFcTxpwYHCeK; _ga_ETPBRPM9ML=GS1.2.1690028471.1.1.1690028577.47.0.0",
+        "Host": "www.kuwo.cn",
+        "Referer": "https://www.kuwo.cn/search/list?key=%E7%AC%BC",
+        "Sec-Fetch-Dest": "empty",
+        "Sec-Fetch-Mode": "cors",
+        "Sec-Fetch-Site": "same-origin",
+        "Secret": "09362e5991f0846bff719a26e1a0e0ac7bd0b3c9f8ab5fdf000c7b88ecfa727000a0ba6e",
+        "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36",
+        "sec-ch-ua": "\"Not.A/Brand\";v=\"8\", \"Chromium\";v=\"114\", \"Google Chrome\";v=\"114\"",
+        "sec-ch-ua-mobile": "?0",
+        "sec-ch-ua-platform": "\"Windows\""
+    }
+    if len(value)>0:
+        apiurl="https://kuwo.cn/api/www/search/searchKey?"
+        search_data = {
+            'key': value,
+            'httpsStatus': '1',
+            'reqId': '7d9e2c60-288a-11ee-9cdf-3f476f1ba25e',
+            "plat":"web_www"
+        }        
+        try:
+            data = requests.get(apiurl,headers=headers,params=search_data)
+        except:
+            return "NetError"
+        data = data.json()
+        data = data["data"]
+        r_data = []
+        for i in range(len(data)):
+            string=data[i]
+            start_index = string.find("RELWORD=") + len("RELWORD=")
+            end_index = string.find("\r", start_index)
+            extracted_text = string[start_index:end_index]
+            r_data.append(extracted_text)
+        return r_data
+    else:
+        return "Error 1"
```

### Comparing `AZMusicAPI-1.0.2/AZMusicAPI.egg-info/PKG-INFO` & `AZMusicAPI-1.2.8/AZMusicAPI.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AZMusicAPI
-Version: 1.0.2
+Version: 1.2.8
 Summary: 轻松访问音乐信息和歌曲音频链接 | Easy access to music information and song audio links
 Author: AZ Studio
 Project-URL: GitHub, https://github.com/AZ-Studio-2023/AZMusicAPI/
 Description-Content-Type: text/markdown
 
 # AZMusicAPI
 轻松访问音乐信息和歌曲音频链接 | Easy access to music information and song audio links
@@ -21,36 +21,46 @@
 ## 导入
 
 ``` import AZMusicAPI```
 
 ## 函数使用
 
 
-```
-AZMusicAPI.getmusic(keyword,number)
-```
+```AZMusicAPI.getmusic(keyword,number)```
 
 ### 作用：获得指定关键词的歌曲
 
 * keyword：关键词 number:返回歌曲数量,可选,默认20
 
 * 关键词可为 歌手/歌曲名/专辑名
 
-### 返回值说明：正常返回列表  "Error 0"：没有结果 "Error 1":用户未输入
+### 返回值类型：列表  
 
-```
-AZMusicAPI.geturl(rid,reqId)
-```
+```AZMusicAPI.geturl(rid,reqId)```
 
 ### 作用：获取音乐的音频地址
 
 * rid:你要解析的歌曲在getmusic返回的rid    
 * reqId:你要解析的歌曲在getmusic返回的reqId
 
-### 返回值：正常返回音频链接 "Error 3":歌曲需要单曲付费或rid/reqId不正确
+### 返回值类型：字符串 
+
+``` AZMusicAPI.searchkey(value)```
+
+### 作用：通过关键字得到音乐/歌手/专辑名
+
+* value:关键字
+
+### 返回值类型：列表
+
+## 错误返回
+* "Error 0"：没有结果 
+* "Error 1":用户未输入
+* "NetError":网络错误 / 服务器宕机 / IP被封禁
+* "Error 3":歌曲需要单曲付费或rid/reqId不正确
 
 ## 代码示例
 ### 仅需7行代码即可完成一个音乐音频地址获取器
 
 ```
 import AZMusicAPI as MusicAPI 
 u=input("请输入您需要的歌曲名称：")
```

### Comparing `AZMusicAPI-1.0.2/PKG-INFO` & `AZMusicAPI-1.2.8/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AZMusicAPI
-Version: 1.0.2
+Version: 1.2.8
 Summary: 轻松访问音乐信息和歌曲音频链接 | Easy access to music information and song audio links
 Author: AZ Studio
 Project-URL: GitHub, https://github.com/AZ-Studio-2023/AZMusicAPI/
 Description-Content-Type: text/markdown
 
 # AZMusicAPI
 轻松访问音乐信息和歌曲音频链接 | Easy access to music information and song audio links
@@ -21,36 +21,46 @@
 ## 导入
 
 ``` import AZMusicAPI```
 
 ## 函数使用
 
 
-```
-AZMusicAPI.getmusic(keyword,number)
-```
+```AZMusicAPI.getmusic(keyword,number)```
 
 ### 作用：获得指定关键词的歌曲
 
 * keyword：关键词 number:返回歌曲数量,可选,默认20
 
 * 关键词可为 歌手/歌曲名/专辑名
 
-### 返回值说明：正常返回列表  "Error 0"：没有结果 "Error 1":用户未输入
+### 返回值类型：列表  
 
-```
-AZMusicAPI.geturl(rid,reqId)
-```
+```AZMusicAPI.geturl(rid,reqId)```
 
 ### 作用：获取音乐的音频地址
 
 * rid:你要解析的歌曲在getmusic返回的rid    
 * reqId:你要解析的歌曲在getmusic返回的reqId
 
-### 返回值：正常返回音频链接 "Error 3":歌曲需要单曲付费或rid/reqId不正确
+### 返回值类型：字符串 
+
+``` AZMusicAPI.searchkey(value)```
+
+### 作用：通过关键字得到音乐/歌手/专辑名
+
+* value:关键字
+
+### 返回值类型：列表
+
+## 错误返回
+* "Error 0"：没有结果 
+* "Error 1":用户未输入
+* "NetError":网络错误 / 服务器宕机 / IP被封禁
+* "Error 3":歌曲需要单曲付费或rid/reqId不正确
 
 ## 代码示例
 ### 仅需7行代码即可完成一个音乐音频地址获取器
 
 ```
 import AZMusicAPI as MusicAPI 
 u=input("请输入您需要的歌曲名称：")
```

### Comparing `AZMusicAPI-1.0.2/setup.py` & `AZMusicAPI-1.2.8/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='AZMusicAPI',
-    version='1.0.2',
+    version='1.2.8',
     author='AZ Studio',
     description='轻松访问音乐信息和歌曲音频链接 | Easy access to music information and song audio links',
     long_description = open('readme.md', encoding='utf-8').read(),
     long_description_content_type="text/markdown",
     packages=['AZMusicAPI'],
     install_requires=['requests'],
     project_urls={
```

