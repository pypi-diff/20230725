# Comparing `tmp/TinetApiRequest-1.0.2.tar.gz` & `tmp/TinetApiRequest-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\TinetApiRequest-1.0.2.tar", last modified: Thu Jul 20 11:57:31 2023, max compression
+gzip compressed data, was "dist\TinetApiRequest-1.0.3.tar", last modified: Tue Jul 25 06:18:11 2023, max compression
```

## Comparing `TinetApiRequest-1.0.2.tar` & `TinetApiRequest-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 11:57:31.000000 TinetApiRequest-1.0.2/
--rw-rw-rw-   0        0        0      272 2023-07-20 11:57:31.000000 TinetApiRequest-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3725 2023-07-14 02:58:39.000000 TinetApiRequest-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-20 11:57:31.000000 TinetApiRequest-1.0.2/TinetApiRequest.egg-info/
--rw-rw-rw-   0        0        0      272 2023-07-20 11:57:31.000000 TinetApiRequest-1.0.2/TinetApiRequest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      343 2023-07-20 11:57:31.000000 TinetApiRequest-1.0.2/TinetApiRequest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 11:57:31.000000 TinetApiRequest-1.0.2/TinetApiRequest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      188 2023-07-20 11:57:31.000000 TinetApiRequest-1.0.2/TinetApiRequest.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-20 11:57:31.000000 TinetApiRequest-1.0.2/TinetApiRequest.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-20 11:57:31.000000 TinetApiRequest-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      713 2023-07-20 10:09:15.000000 TinetApiRequest-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-20 11:57:31.000000 TinetApiRequest-1.0.2/tinet/
--rw-rw-rw-   0        0        0    22202 2023-07-20 11:43:44.000000 TinetApiRequest-1.0.2/tinet/APIRequest.py
--rw-rw-rw-   0        0        0     6911 2023-07-17 07:53:30.000000 TinetApiRequest-1.0.2/tinet/ApiConfig.py
--rw-rw-rw-   0        0        0     1082 2023-07-11 08:50:04.000000 TinetApiRequest-1.0.2/tinet/LogUtil.py
--rw-rw-rw-   0        0        0     3401 2023-07-20 11:56:57.000000 TinetApiRequest-1.0.2/tinet/RequestUtil.py
--rw-rw-rw-   0        0        0     2958 2023-07-11 08:50:04.000000 TinetApiRequest-1.0.2/tinet/SignUtil.py
--rw-rw-rw-   0        0        0     7314 2023-06-13 08:06:01.000000 TinetApiRequest-1.0.2/tinet/YamlUtil.py
--rw-rw-rw-   0        0        0      164 2023-06-09 08:49:02.000000 TinetApiRequest-1.0.2/tinet/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 06:18:11.000000 TinetApiRequest-1.0.3/
+-rw-rw-rw-   0        0        0      272 2023-07-25 06:18:11.000000 TinetApiRequest-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3725 2023-07-14 02:58:39.000000 TinetApiRequest-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 06:18:11.000000 TinetApiRequest-1.0.3/TinetApiRequest.egg-info/
+-rw-rw-rw-   0        0        0      272 2023-07-25 06:18:11.000000 TinetApiRequest-1.0.3/TinetApiRequest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      343 2023-07-25 06:18:11.000000 TinetApiRequest-1.0.3/TinetApiRequest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 06:18:11.000000 TinetApiRequest-1.0.3/TinetApiRequest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      188 2023-07-25 06:18:11.000000 TinetApiRequest-1.0.3/TinetApiRequest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-25 06:18:11.000000 TinetApiRequest-1.0.3/TinetApiRequest.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-25 06:18:11.000000 TinetApiRequest-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      713 2023-07-25 06:18:06.000000 TinetApiRequest-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 06:18:11.000000 TinetApiRequest-1.0.3/tinet/
+-rw-rw-rw-   0        0        0    22254 2023-07-25 06:11:50.000000 TinetApiRequest-1.0.3/tinet/APIRequest.py
+-rw-rw-rw-   0        0        0     6911 2023-07-17 07:53:30.000000 TinetApiRequest-1.0.3/tinet/ApiConfig.py
+-rw-rw-rw-   0        0        0     1082 2023-07-11 08:50:04.000000 TinetApiRequest-1.0.3/tinet/LogUtil.py
+-rw-rw-rw-   0        0        0     3479 2023-07-20 12:03:44.000000 TinetApiRequest-1.0.3/tinet/RequestUtil.py
+-rw-rw-rw-   0        0        0     2958 2023-07-11 08:50:04.000000 TinetApiRequest-1.0.3/tinet/SignUtil.py
+-rw-rw-rw-   0        0        0     7314 2023-06-13 08:06:01.000000 TinetApiRequest-1.0.3/tinet/YamlUtil.py
+-rw-rw-rw-   0        0        0      164 2023-06-09 08:49:02.000000 TinetApiRequest-1.0.3/tinet/__init__.py
```

### Comparing `TinetApiRequest-1.0.2/README.md` & `TinetApiRequest-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `TinetApiRequest-1.0.2/setup.py` & `TinetApiRequest-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 BASE_DIR = Path(__file__).parent
 with open(Path(BASE_DIR, "requirements.txt"), "r") as file:
     required_packages = [ln.strip() for ln in file.readlines()]
 
 # Define our package
 setup(
     name="TinetApiRequest",
-    version="1.0.2",
+    version="1.0.3",
     description="天润接口测试库",
     author="天润-测试",
     author_email="zhupeng@ti-net.com.cn",
     url="https://www.ti-net.com.cn/",
     python_requires=">=3.7",
     packages=find_namespace_packages(),
     install_requires=[required_packages],
```

### Comparing `TinetApiRequest-1.0.2/tinet/APIRequest.py` & `TinetApiRequest-1.0.3/tinet/APIRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 接口测试核心类
 """
 import json
+import os
 import time
 from urllib.parse import urlparse
 
 import pytest
 import allure
 import jsonpath
 from requests_toolbelt import MultipartEncoder
@@ -44,15 +45,15 @@
         yamlId = yaml.get('id')
         yamlName = yaml.get('name')
         yamlKind = yaml.get('kind')
         yamlTestcase = yaml.get('testcases')
         # 先拿到所有testcase
         log.info(f"开始执行测试用例name: {yamlName}, id: {yamlId} , 测试用例: {yamlTestcase}")
         allure.attach(f"{yamlTestcase}", name=f"开始执行测试用例name: {yamlName}, id: {yamlId} ", attachment_type=allure.attachment_type.TEXT)
-        request = HttpClient()
+        request = HttpClient()  # todo 定制化接口HttpClient
         # 开始遍历testcase
         # allure.dynamic.title(yamlName)
         for testcase in yamlTestcase:
             with allure.step(testcase.get('name')):
                 # 拿到用例如果是common的去common文件路径中拿测试用例
                 if testcase.get('skip'):  # 判断是否跳过
                     log.info(f"用例: {json.dumps(testcase.get('name'), indent=4, ensure_ascii=False)}跳过")
@@ -151,40 +152,40 @@
                 self.assertChoose(1 > 2, f"提取{ass.get(key)[0]}失败，断言失败, response结果: {json.dumps(response.text, indent=4, ensure_ascii=False)}", failType)
                 continue
             if 'eq' in ass:
                 # 相等判断 都转为str进行判断
                 expectedResults = PlaceholderYaml(attrObj=bean, reString=ass.get('eq')[1]).replace().replaced_str
                 # 判断 expectedResults 是否在 jsonpathResults list中  判断类型
                 assResults = str(expectedResults) in [str(item) for item in jsonpathResults]
-                self.assertChoose(assResults is True, f"eq断言失败: {jsonpathResults} 不等于 {expectedResults}", failType)
                 log.info(f"断言eq结束: {jsonpathResults} 等于 {expectedResults}")
                 allure.attach(f"{jsonpathResults} 等于 {expectedResults}", name=f"断言eq结束", attachment_type=allure.attachment_type.TEXT)
+                self.assertChoose(assResults is True, f"eq断言失败: {jsonpathResults} 不等于 {expectedResults}", failType)
             elif 'sge' in ass:
                 # size greater than or equal
                 expectedResults = PlaceholderYaml(attrObj=bean, reString=ass.get('sge')[1]).replace().replaced_str
-                self.assertChoose(len(jsonpathResults) >= int(expectedResults), f"sge断言失败: {jsonpathResults} 不等于 {expectedResults}", failType)
                 log.info(f"断言sge结束: {jsonpathResults} size >= {expectedResults}")
                 allure.attach(f" {jsonpathResults} size >= {expectedResults}", name=f"断言sge结束",
                               attachment_type=allure.attachment_type.TEXT)
+                self.assertChoose(len(jsonpathResults) >= int(expectedResults), f"sge断言失败: {jsonpathResults} 小于 {expectedResults}", failType)
             elif 'ne' in ass:
                 # not eq 断言
                 return 'ne'
             elif 'nn' in ass:
                 # not none
                 # 判断json path 是否不为空 返回FALSE
-                self.assertChoose(jsonpathResults is not None,
-                                  f"not none断言失败: {ass.get('nn')[0]}  ,jsonpath结果: {jsonpathResults}", failType)
                 log.info(f"断言not none结束: {jsonpathResults}")
                 allure.attach(f" {jsonpathResults} ", name=f"断言not none结束", attachment_type=allure.attachment_type.TEXT)
+                self.assertChoose(jsonpathResults is not None,
+                                  f"not none断言失败: {ass.get('nn')[0]}  ,jsonpath结果: {jsonpathResults}", failType)
             elif 'none' in ass:
                 # 判断json path 是否 返回FALSE
-                self.assertChoose(jsonpathResults is True,
-                                  f"none断言失败: {ass.get('none')[0]}  ,jsonpath结果: {jsonpathResults}", failType)
                 log.info(f"断言none结束: {jsonpathResults}")
                 allure.attach(f" {jsonpathResults} ", name=f"断言none结束", attachment_type=allure.attachment_type.TEXT)
+                self.assertChoose(jsonpathResults is True,
+                                  f"none断言失败: {ass.get('none')[0]}  ,jsonpath结果: {jsonpathResults}", failType)
 
     # 根据data从response中根据json还是其他方法来获取response中的值
     def addAttrSaveBean(self, bean, globalBean, data: list, response):
         # 先解析data 如果data为空则直接返回
         if data is None:
             return
         for d in data:
@@ -307,15 +308,15 @@
     # 根据common路径跟id 去重新赋值testcase
     def getCommonTestCase(self, testcase, commonFile, caseId):
         # 先判断 self.commonCase 是否为空,如果不为空则需要读取commonFile,否则读取用例类自定义commonfile
         if self.commonCase is None:
             # 读取commonFile
             commonFile = commonFile
         else:
-            commonFile = commonFile.split('common\\')[0] + 'common\\' + self.commonCase
+            commonFile = os.path.join(commonFile.split('common')[0], f'common/{self.commonCase}')
         log.info(f"开始读取commonFile: {commonFile}")
         allure.attach(f"{commonFile}", name=f"开始读取commonFile", attachment_type=allure.attachment_type.TEXT)
         yaml = ReadYaml(commonFile).load_yaml()
         # 获取所有case
         commonCase = yaml.get('testcases')
         log.info(f"读取完成commonFile: {commonCase}")
         allure.attach(f"{commonCase}", name=f"读取完成commonFile", attachment_type=allure.attachment_type.TEXT)
```

### Comparing `TinetApiRequest-1.0.2/tinet/ApiConfig.py` & `TinetApiRequest-1.0.3/tinet/ApiConfig.py`

 * *Files identical despite different names*

### Comparing `TinetApiRequest-1.0.2/tinet/LogUtil.py` & `TinetApiRequest-1.0.3/tinet/LogUtil.py`

 * *Files identical despite different names*

### Comparing `TinetApiRequest-1.0.2/tinet/RequestUtil.py` & `TinetApiRequest-1.0.3/tinet/RequestUtil.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         :param method: str 请求方法，例如 GET、POST、PUT 等。
         :param url: str 请求 URL，会和 base_url 拼接成完整的 URL。
         :param kwargs: dict 其他 requests.request 方法支持的参数。
         :return: requests.Response 响应对象。
         """
 
         response = self.session.request(method, url, **kwargs)
-        # 判断请求url 是否包含 openapi_login
+        # 判断请求url 是否包含 openapi_login  用于处理 单点登录到系统后进行系统的接口请求鉴权处理
         if 'openapi_login' in url:
             # 需要请求接口 获取 Tsessionid
             # 先从url 中解析出请求域名
             parsed_url = urlparse(url)
             domain = parsed_url.scheme + '://' + parsed_url.netloc
             # 进行接口请求 拿到响应
             personalResponse = self.session.request(method='GET', url=domain + '/api/personal/info/get')
```

### Comparing `TinetApiRequest-1.0.2/tinet/SignUtil.py` & `TinetApiRequest-1.0.3/tinet/SignUtil.py`

 * *Files identical despite different names*

### Comparing `TinetApiRequest-1.0.2/tinet/YamlUtil.py` & `TinetApiRequest-1.0.3/tinet/YamlUtil.py`

 * *Files identical despite different names*

