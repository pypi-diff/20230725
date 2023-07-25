# Comparing `tmp/tme_api-2023.3.24.post1.tar.gz` & `tmp/tme_api-2023.7.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\tme_api-2023.3.24.post1.tar", last modified: Fri Mar 24 03:39:30 2023, max compression
+gzip compressed data, was "dist\tme_api-2023.7.25.tar", last modified: Tue Jul 25 08:58:15 2023, max compression
```

## Comparing `tme_api-2023.3.24.post1.tar` & `tme_api-2023.7.25.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-03-24 03:39:30.000000 tme_api-2023.3.24.post1/
--rw-rw-rw-   0        0        0      615 2023-03-24 03:39:30.000000 tme_api-2023.3.24.post1/PKG-INFO
--rw-rw-rw-   0        0        0       44 2022-01-26 09:14:36.000000 tme_api-2023.3.24.post1/README.md
--rw-rw-rw-   0        0        0       42 2023-03-24 03:39:30.000000 tme_api-2023.3.24.post1/setup.cfg
--rw-rw-rw-   0        0        0     5329 2023-03-24 03:35:57.000000 tme_api-2023.3.24.post1/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-24 03:39:30.000000 tme_api-2023.3.24.post1/tme_api/
-drwxrwxrwx   0        0        0        0 2023-03-24 03:39:30.000000 tme_api-2023.3.24.post1/tme_api/cms/
--rw-rw-rw-   0        0        0    26444 2022-10-20 08:36:17.000000 tme_api-2023.3.24.post1/tme_api/cms/api.py
--rw-rw-rw-   0        0        0     7533 2023-03-20 11:00:57.000000 tme_api-2023.3.24.post1/tme_api/cms/enums.py
--rw-rw-rw-   0        0        0      656 2020-09-28 03:45:55.000000 tme_api-2023.3.24.post1/tme_api/cms/exception.py
--rw-rw-rw-   0        0        0    16736 2023-03-24 03:17:22.000000 tme_api-2023.3.24.post1/tme_api/cms/model.py
--rw-rw-rw-   0        0        0    20729 2022-10-20 08:34:07.000000 tme_api-2023.3.24.post1/tme_api/cms/requests.py
--rw-rw-rw-   0        0        0    28475 2023-03-24 03:34:04.000000 tme_api-2023.3.24.post1/tme_api/cms/responses.py
--rw-rw-rw-   0        0        0     1566 2021-11-08 10:41:13.000000 tme_api-2023.3.24.post1/tme_api/cms/utils.py
--rw-rw-rw-   0        0        0        0 2020-09-01 10:18:32.000000 tme_api-2023.3.24.post1/tme_api/cms/__init__.py
--rw-rw-rw-   0        0        0        0 2020-09-01 10:18:32.000000 tme_api-2023.3.24.post1/tme_api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-24 03:39:30.000000 tme_api-2023.3.24.post1/tme_api.egg-info/
--rw-rw-rw-   0        0        0        1 2023-03-24 03:39:30.000000 tme_api-2023.3.24.post1/tme_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      615 2023-03-24 03:39:30.000000 tme_api-2023.3.24.post1/tme_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       49 2023-03-24 03:39:30.000000 tme_api-2023.3.24.post1/tme_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0      372 2023-03-24 03:39:30.000000 tme_api-2023.3.24.post1/tme_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        8 2023-03-24 03:39:30.000000 tme_api-2023.3.24.post1/tme_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-25 08:58:15.000000 tme_api-2023.7.25/
+-rw-rw-rw-   0        0        0      609 2023-07-25 08:58:15.000000 tme_api-2023.7.25/PKG-INFO
+-rw-rw-rw-   0        0        0       44 2022-01-26 09:14:36.000000 tme_api-2023.7.25/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-25 08:58:15.000000 tme_api-2023.7.25/setup.cfg
+-rw-rw-rw-   0        0        0     5334 2023-07-25 08:57:15.000000 tme_api-2023.7.25/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 08:58:15.000000 tme_api-2023.7.25/tme_api/
+drwxrwxrwx   0        0        0        0 2023-07-25 08:58:15.000000 tme_api-2023.7.25/tme_api/cms/
+-rw-rw-rw-   0        0        0    26444 2022-10-20 08:36:17.000000 tme_api-2023.7.25/tme_api/cms/api.py
+-rw-rw-rw-   0        0        0     7533 2023-03-20 11:00:57.000000 tme_api-2023.7.25/tme_api/cms/enums.py
+-rw-rw-rw-   0        0        0      656 2020-09-28 03:45:55.000000 tme_api-2023.7.25/tme_api/cms/exception.py
+-rw-rw-rw-   0        0        0    16771 2023-07-25 08:55:55.000000 tme_api-2023.7.25/tme_api/cms/model.py
+-rw-rw-rw-   0        0        0    20739 2023-07-25 08:55:55.000000 tme_api-2023.7.25/tme_api/cms/requests.py
+-rw-rw-rw-   0        0        0    28480 2023-07-25 08:55:55.000000 tme_api-2023.7.25/tme_api/cms/responses.py
+-rw-rw-rw-   0        0        0     1566 2021-11-08 10:41:13.000000 tme_api-2023.7.25/tme_api/cms/utils.py
+-rw-rw-rw-   0        0        0        0 2020-09-01 10:18:32.000000 tme_api-2023.7.25/tme_api/cms/__init__.py
+-rw-rw-rw-   0        0        0        0 2020-09-01 10:18:32.000000 tme_api-2023.7.25/tme_api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 08:58:15.000000 tme_api-2023.7.25/tme_api.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-25 08:58:14.000000 tme_api-2023.7.25/tme_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      609 2023-07-25 08:58:14.000000 tme_api-2023.7.25/tme_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       56 2023-07-25 08:58:14.000000 tme_api-2023.7.25/tme_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      372 2023-07-25 08:58:14.000000 tme_api-2023.7.25/tme_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        8 2023-07-25 08:58:14.000000 tme_api-2023.7.25/tme_api.egg-info/top_level.txt
```

### Comparing `tme_api-2023.3.24.post1/PKG-INFO` & `tme_api-2023.7.25/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tme_api
-Version: 2023.3.24.post1
+Version: 2023.7.25
 Summary: tme_api
 Home-page: https://github.com/ldsxp/tme_api
 Author: lds
 Author-email: 85176878@qq.com
 License: GNU GPL 3
 Download-URL: https://pypi.org/project/tme_api
 Description: 访问 icms.tmeoa.com 的api
```

### Comparing `tme_api-2023.3.24.post1/setup.py` & `tme_api-2023.7.25/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ﻿import os
 import sys
 from setuptools import setup, find_packages
 
-version = '2023.3.24-1'
+version = '2023.7.25'
 
 # 创建一个源码包
 # python setup.py sdist
 # 对于 Windows，可以执行python setup.py bdist_wininst 生成一个exe文件；
 # 若要生成 RPM 包，执行 python setup.py bdist_rpm，但系统必须有 rpm 命令的支持。
 # 可以运行下面的命令查看所有格式的支持：
 # python setup.py bdist --help-formats
@@ -124,15 +124,15 @@
         'Programming Language :: Python',
         'Programming Language :: Python :: 3.6',
     ],
     # 需要安装的依赖包
     install_requires=[
         'requests_toolbelt',
         'requests',
-        'pydantic',
+        'pydantic>=1.9.2',
         'spider-utils',
         # 'xlrd>=1.1.0',
         # 'colorama',
         # 'chardet',
         # 'pyperclip',
         # 'requests',
         # 'html2text',
```

### Comparing `tme_api-2023.3.24.post1/tme_api/cms/api.py` & `tme_api-2023.7.25/tme_api/cms/api.py`

 * *Files identical despite different names*

### Comparing `tme_api-2023.3.24.post1/tme_api/cms/enums.py` & `tme_api-2023.7.25/tme_api/cms/enums.py`

 * *Files identical despite different names*

### Comparing `tme_api-2023.3.24.post1/tme_api/cms/exception.py` & `tme_api-2023.7.25/tme_api/cms/exception.py`

 * *Files identical despite different names*

### Comparing `tme_api-2023.3.24.post1/tme_api/cms/model.py` & `tme_api-2023.7.25/tme_api/cms/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,15 +117,15 @@
     contract_type: ContractTypeEnum = Field(None, title="签约类型")
     # （1：未确定；2：可维权；3：不可维权）
     can_legal_rights: CanLegalRightsEnum = Field(None, title="可维权")
     # （1：否；2：是；）
     can_cover: CanCoverEnum = Field(None, title="可翻唱")
     auth_area: str = Field(None, title="授权区域", max_length=250)  # （ID，”,”分割）
 
-    @validator('auth_relation', pre=True, whole=True)
+    @validator('auth_relation', pre=True, each_item=False)
     def auth_relation_to_none(cls, v):
         # print('auth_relation_to_none', type(v), v)
         if not v:
             # print('auth_relation_to_none return None')
             return None
         return v
 
@@ -175,38 +175,38 @@
             return None
         if isinstance(v, list) and len(v) == 1:
             return v[0]
         elif isinstance(v, dict):
             return v
         raise ValueError(f'music 字段, 不能转换为字典 {v}')
 
-    # @validator('artist', pre=True, whole=True)
+    # @validator('artist', pre=True, each_item=False)
     # def blank_character_to_none(cls, v):
     #     """
     #     空白字符的时候返回 None
     #     """
     #     # print('SongModel character_to_none', type(v), v)
     #     if not v:
     #         return None
     #     return v
 
-    @validator('artist', pre=True, whole=True)
+    @validator('artist', pre=True, each_item=False)
     def artist_to_list(cls, v):
         """
         如果内容不为真，那么我们返回空列表
         """
         # print('SongModel artist_to_list', type(v), v)
         if not v:
             return []
         # 因为录入错误，所以应该是列表的时候，内容为0
         elif v == '0':
             return None
         return v
 
-    @validator('text_lyrics', pre=True, whole=True)
+    @validator('text_lyrics', pre=True, each_item=False)
     def text_lyrics_to_list(cls, v):
         """
         """
         # print('SongModel text_lyrics_to_list', type(v), v)
         if not v:
             return []
         return v
@@ -243,34 +243,34 @@
     copyright_company: str = Field(None, title="所属公司", max_length=250)  # 保存的时候不需要
     signsubject_id: int = Field(None, title="签约主体ID")
     signsubject: str = Field(None, title="签约主体名称", max_length=250)  # 保存的时候不需要
     status: StatusEnum = Field(0, title="状态")  # 保存的时候不需要
     finish_status: FinishStatusEnum = Field(None, title="完善状态")  # 自动判断   # 保存的时候不需要，获取专辑详情的时候也没有了
     song_list: List[SongModel] = Field([], title="歌曲列表")
 
-    @validator('artist', pre=True, whole=True)
+    @validator('artist', pre=True, each_item=False)
     def artist_to_none(cls, v):
         # print('artist_to_none', type(v), v)
         if not v:
             # print('artist_to_none return None')
             return None
         # 因为录入错误，所以应该是列表的时候，内容为0
         elif v == '0':
             return None
         return v
 
-    @validator('auth_file', pre=True, whole=True)
+    @validator('auth_file', pre=True, each_item=False)
     def auth_file_to_none(cls, v):
         # print('auth_file_to_none', type(v), v)
         if not v:
             # print('auth_file_to_none return None')
             return None
         return v
 
-    @validator('song_list', pre=True, whole=True)
+    @validator('song_list', pre=True, each_item=False)
     def song_list_to_list(cls, v):
         # print('song_list_to_list', type(v), v)
         if not v:
             # print('song_list_to_list return None')
             return []
         return v
```

### Comparing `tme_api-2023.3.24.post1/tme_api/cms/requests.py` & `tme_api-2023.7.25/tme_api/cms/requests.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,15 @@
     @validator('text_lyrics', 'music', pre=True)
     def list_data_to_str(cls, v):
         """
         转换列表数据为后端需要的json字符串
         """
         return convert_to_list_string(v)
 
-    @validator('artist', pre=True, whole=True)
+    @validator('artist', pre=True, each_item=False)
     def artist_data(cls, v):
         """
         转换保存专家需要的歌手数据
         """
         return convert_to_character_array_list(v)
 
 
@@ -172,15 +172,15 @@
         for file_data in v:
             if 'url' in file_data:
                 del file_data['url']
             r.append(file_data)
 
         return json.dumps(r, ensure_ascii=False)
 
-    @validator('artist', pre=True, whole=True)
+    @validator('artist', pre=True, each_item=False)
     def artist_data(cls, v):
         """
         转换保存专家需要的歌手数据
         """
         # print(f'{cls.__name__} list_data_to_str', type(v), v)
         return convert_to_character_array_list(v, delimiter=',')
```

### Comparing `tme_api-2023.3.24.post1/tme_api/cms/responses.py` & `tme_api-2023.7.25/tme_api/cms/responses.py`

 * *Files 0% similar despite different names*

```diff
@@ -273,15 +273,15 @@
     # authorized_mode: AuthorizedModeEnum = Field(None, title="授权形式")  # 1：代表独家；2：代表非独家
     authorized_mode: str = Field(None, title="授权形式", max_length=250)  # 授权形式(1：代表独家；2：代表非独家)
     authorized_mode_desc: str = Field(None, title="授权形式说明", max_length=250)
     word_share: str = Field(None, title="词权利比例", max_length=250)
     music_share: str = Field(None, title="曲权利比例", max_length=250)
     record_share: str = Field(None, title="录音权利比例", max_length=250)
 
-    @validator('auth_relation', pre=True, whole=True)
+    @validator('auth_relation', pre=True, each_item=False)
     def auth_relation_to_none(cls, v):
         # print('auth_relation_to_none', type(v), v)
         if not v:
             # print('auth_relation_to_none return None')
             return None
         return v
```

### Comparing `tme_api-2023.3.24.post1/tme_api/cms/utils.py` & `tme_api-2023.7.25/tme_api/cms/utils.py`

 * *Files identical despite different names*

### Comparing `tme_api-2023.3.24.post1/tme_api.egg-info/PKG-INFO` & `tme_api-2023.7.25/tme_api.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tme-api
-Version: 2023.3.24.post1
+Version: 2023.7.25
 Summary: tme_api
 Home-page: https://github.com/ldsxp/tme_api
 Author: lds
 Author-email: 85176878@qq.com
 License: GNU GPL 3
 Download-URL: https://pypi.org/project/tme_api
 Description: 访问 icms.tmeoa.com 的api
```

