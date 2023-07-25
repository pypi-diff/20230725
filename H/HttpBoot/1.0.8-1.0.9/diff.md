# Comparing `tmp/HttpBoot-1.0.8.tar.gz` & `tmp/HttpBoot-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/HttpBoot-1.0.8.tar", last modified: Wed Feb 22 08:42:24 2023, max compression
+gzip compressed data, was "dist/HttpBoot-1.0.9.tar", last modified: Tue Jul 25 14:04:36 2023, max compression
```

## Comparing `HttpBoot-1.0.8.tar` & `HttpBoot-1.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 shi       (1000) shi       (1000)        0 2023-02-22 08:42:24.000000 HttpBoot-1.0.8/
-drwxr-xr-x   0 shi       (1000) shi       (1000)        0 2023-02-22 08:42:24.000000 HttpBoot-1.0.8/HttpBoot/
--rw-r--r--   0 shi       (1000) shi       (1000)      480 2023-01-05 00:36:55.000000 HttpBoot-1.0.8/HttpBoot/__init__.py
--rw-r--r--   0 shi       (1000) shi       (1000)     1450 2022-11-01 00:31:46.000000 HttpBoot-1.0.8/HttpBoot/extractor.py
--rw-r--r--   0 shi       (1000) shi       (1000)    12851 2022-12-08 06:44:27.000000 HttpBoot-1.0.8/HttpBoot/http_boot.py
--rw-r--r--   0 shi       (1000) shi       (1000)     1533 2022-07-29 08:58:32.000000 HttpBoot-1.0.8/HttpBoot/locust_boot.py
--rw-r--r--   0 shi       (1000) shi       (1000)     1100 2022-09-01 02:51:33.000000 HttpBoot-1.0.8/HttpBoot/locust_main.py
--rw-r--r--   0 shi       (1000) shi       (1000)     1712 2022-11-01 00:31:46.000000 HttpBoot-1.0.8/HttpBoot/response_wrapper.py
--rw-r--r--   0 shi       (1000) shi       (1000)     2772 2022-11-01 00:31:46.000000 HttpBoot-1.0.8/HttpBoot/validator.py
-drwxr-xr-x   0 shi       (1000) shi       (1000)        0 2023-02-22 08:42:24.000000 HttpBoot-1.0.8/HttpBoot.egg-info/
--rw-r--r--   0 shi       (1000) shi       (1000)    13123 2023-02-22 08:42:24.000000 HttpBoot-1.0.8/HttpBoot.egg-info/PKG-INFO
--rw-r--r--   0 shi       (1000) shi       (1000)      407 2023-02-22 08:42:24.000000 HttpBoot-1.0.8/HttpBoot.egg-info/SOURCES.txt
--rw-r--r--   0 shi       (1000) shi       (1000)        1 2023-02-22 08:42:24.000000 HttpBoot-1.0.8/HttpBoot.egg-info/dependency_links.txt
--rw-r--r--   0 shi       (1000) shi       (1000)       92 2023-02-22 08:42:24.000000 HttpBoot-1.0.8/HttpBoot.egg-info/entry_points.txt
--rw-r--r--   0 shi       (1000) shi       (1000)        1 2023-01-05 00:36:16.000000 HttpBoot-1.0.8/HttpBoot.egg-info/not-zip-safe
--rw-r--r--   0 shi       (1000) shi       (1000)       45 2023-02-22 08:42:24.000000 HttpBoot-1.0.8/HttpBoot.egg-info/requires.txt
--rw-r--r--   0 shi       (1000) shi       (1000)        9 2023-02-22 08:42:24.000000 HttpBoot-1.0.8/HttpBoot.egg-info/top_level.txt
--rw-r--r--   0 shi       (1000) shi       (1000)    13123 2023-02-22 08:42:24.000000 HttpBoot-1.0.8/PKG-INFO
--rw-r--r--   0 shi       (1000) shi       (1000)    12170 2022-12-07 02:18:01.000000 HttpBoot-1.0.8/README.md
--rw-r--r--   0 shi       (1000) shi       (1000)       38 2023-02-22 08:42:24.000000 HttpBoot-1.0.8/setup.cfg
--rw-r--r--   0 shi       (1000) shi       (1000)     1861 2022-08-26 00:53:31.000000 HttpBoot-1.0.8/setup.py
+drwxr-xr-x   0 shi       (1000) shi       (1000)        0 2023-07-25 14:04:36.000000 HttpBoot-1.0.9/
+drwxr-xr-x   0 shi       (1000) shi       (1000)        0 2023-07-25 14:04:36.000000 HttpBoot-1.0.9/HttpBoot/
+-rw-r--r--   0 shi       (1000) shi       (1000)      544 2023-03-29 12:49:23.000000 HttpBoot-1.0.9/HttpBoot/__init__.py
+-rw-r--r--   0 shi       (1000) shi       (1000)     1205 2023-05-30 12:03:06.000000 HttpBoot-1.0.9/HttpBoot/extractor.py
+-rw-r--r--   0 shi       (1000) shi       (1000)    13323 2023-07-25 13:15:08.000000 HttpBoot-1.0.9/HttpBoot/http_boot.py
+-rw-r--r--   0 shi       (1000) shi       (1000)     1826 2023-07-25 13:54:41.000000 HttpBoot-1.0.9/HttpBoot/locust_boot.py
+-rw-r--r--   0 shi       (1000) shi       (1000)     1218 2023-05-12 14:12:46.000000 HttpBoot-1.0.9/HttpBoot/locust_main.py
+-rw-r--r--   0 shi       (1000) shi       (1000)     1606 2023-05-30 12:03:06.000000 HttpBoot-1.0.9/HttpBoot/response_wrapper.py
+-rw-r--r--   0 shi       (1000) shi       (1000)     1176 2023-05-16 15:27:19.000000 HttpBoot-1.0.9/HttpBoot/validator.py
+drwxr-xr-x   0 shi       (1000) shi       (1000)        0 2023-07-25 14:04:36.000000 HttpBoot-1.0.9/HttpBoot.egg-info/
+-rw-r--r--   0 shi       (1000) shi       (1000)    14232 2023-07-25 14:04:35.000000 HttpBoot-1.0.9/HttpBoot.egg-info/PKG-INFO
+-rw-r--r--   0 shi       (1000) shi       (1000)      407 2023-07-25 14:04:36.000000 HttpBoot-1.0.9/HttpBoot.egg-info/SOURCES.txt
+-rw-r--r--   0 shi       (1000) shi       (1000)        1 2023-07-25 14:04:35.000000 HttpBoot-1.0.9/HttpBoot.egg-info/dependency_links.txt
+-rw-r--r--   0 shi       (1000) shi       (1000)       92 2023-07-25 14:04:36.000000 HttpBoot-1.0.9/HttpBoot.egg-info/entry_points.txt
+-rw-r--r--   0 shi       (1000) shi       (1000)        1 2022-07-29 14:37:25.000000 HttpBoot-1.0.9/HttpBoot.egg-info/not-zip-safe
+-rw-r--r--   0 shi       (1000) shi       (1000)       45 2023-07-25 14:04:36.000000 HttpBoot-1.0.9/HttpBoot.egg-info/requires.txt
+-rw-r--r--   0 shi       (1000) shi       (1000)        9 2023-07-25 14:04:36.000000 HttpBoot-1.0.9/HttpBoot.egg-info/top_level.txt
+-rw-r--r--   0 shi       (1000) shi       (1000)    14232 2023-07-25 14:04:36.000000 HttpBoot-1.0.9/PKG-INFO
+-rw-r--r--   0 shi       (1000) shi       (1000)    13279 2023-07-25 14:00:28.000000 HttpBoot-1.0.9/README.md
+-rw-r--r--   0 shi       (1000) shi       (1000)       38 2023-07-25 14:04:36.000000 HttpBoot-1.0.9/setup.cfg
+-rw-r--r--   0 shi       (1000) shi       (1000)     1914 2023-04-16 05:50:24.000000 HttpBoot-1.0.9/setup.py
```

### Comparing `HttpBoot-1.0.8/HttpBoot/extractor.py` & `HttpBoot-1.0.9/HttpBoot/validator.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,45 +1,37 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
-from requests import Response
+import re
 from HttpBoot.response_wrapper import ResponseWrap
-from pyutilb.util import *
-from pyutilb import log
+from requests import Response
+from pyutilb.log import log
+from pyutilb import BaseValidator
 
-# 抽取器
-class Extractor(ResponseWrap):
+# 校验器
+class Validator(BaseValidator, ResponseWrap):
 
     def __init__(self, res: Response = None):
-        super(Extractor, self).__init__(res)
+        super(Validator, self).__init__(res)
 
-    # 抽取参数
+    # 执行校验
     def run(self, config):
-        if 'extract_by_jsonpath' in config:
-            return self.run_type('jsonpath', config['extract_by_jsonpath'])
+        if 'validate_by_jsonpath' in config:
+            return self.run_type('jsonpath', config['validate_by_jsonpath'])
+
+        if 'validate_by_css' in config:
+            return self.run_type('css', config['validate_by_css'])
+
+        if 'validate_by_xpath' in config:
+            return self.run_type('xpath', config['validate_by_xpath'])
+
+        if 'validate_by_id' in config:
+            return self.run_type('id', config['validate_by_id'])
 
-        if 'extract_by_css' in config:
-            return self.run_type('css', config['extract_by_css'])
+        if 'validate_by_aid' in config:
+            return self.run_type('aid', config['validate_by_aid'])
 
-        if 'extract_by_xpath' in config:
-            return self.run_type('xpath', config['extract_by_xpath'])
+        if 'validate_by_class' in config:
+            return self.run_type('class', config['validate_by_class'])
 
-        if 'extract_by_id' in config:
-            return self.run_type('id', config['extract_by_id'])
-
-        if 'extract_by_aid' in config:
-            return self.run_type('aid', config['extract_by_aid'])
-
-        if 'extract_by_class' in config:
-            return self.run_type('class', config['extract_by_class'])
-
-        if 'extract_by_eval' in config:
-            return self.run_type('eval', config['extract_by_eval'])
-
-    # 执行单个类型的抽取
-    def run_type(self, type, fields):
-        for var, path in fields.items():
-            # 获得字段值
-            val = self._get_val_by(type, path)
-            # 抽取单个字段
-            set_var(var, val)
-            log.debug(f"Extract variable from response: {var}={val}")
+        if 'validate_by_eval' in config:
+            return self.run_type('eval', config['validate_by_eval'])
```

### Comparing `HttpBoot-1.0.8/HttpBoot/http_boot.py` & `HttpBoot-1.0.9/HttpBoot/http_boot.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,20 +2,23 @@
 # -*- coding: utf-8 -*-
 
 import os
 import sys
 import fnmatch
 import requests
 from pyutilb.util import *
+from pyutilb.file import *
+from pyutilb.cmd import *
 from HttpBoot.validator import Validator
 from HttpBoot.extractor import Extractor
 from requests.sessions import Session
 import curlify
 import threading
-from pyutilb import log, YamlBoot, BreakException, ocr_youdao
+from pyutilb import YamlBoot, BreakException, ocr_youdao
+from pyutilb.log import log
 if hasattr(os, 'posix_spawnp'):
     import gevent
     from locust.clients import HttpSession
 
 # 改造 requests.Session.request() -- 支持打印curl + fix get请求不能传递data + fix不能传递cookie
 if Session.request.__name__ != 'request2': # fix bug: 两次执行此处, 从而导致 Session.request 被改写两次, 从而导致打了2次log
     request1 = Session.request
@@ -52,33 +55,34 @@
 class HttpBoot(YamlBoot):
 
     def __init__(self):
         super().__init__()
         # 动作映射函数
         actions = {
             'base_url': self.base_url,
-            'common_data': self.common_data,
-            'common_headers': self.common_headers,
+            'common_req': self.common_req,
             'get': self.get,
             'post': self.post,
             'upload': self.upload,
             'download': self.download,
             'recognize_captcha': self.recognize_captcha,
             'concurrent': self.concurrent,
         }
         self.add_actions(actions)
 
         # 已下载过的url对应的文件，key是url，value是文件
         self.downloaded_files = {}
         # 基础url
         self._base_url = None
         # 公共请求参数
-        self._common_data = None
-        # 公共请求头
-        self._common_headers = None
+        self._common_req = {
+            'data': None,
+            'headers': None,
+            'json': None,
+        }
         # 当前url
         self.curr_url = None
         # 当前session
         self.session = requests.Session()
         # 记录响应时间
         self.res_times = []
         # 错误次数
@@ -90,15 +94,15 @@
     # :param args 其他参数，包含2个数: 1 concurrency 并发数 2 req_num 每个线程的请求数
     def concurrent(self, steps, args):
         if args == None or len(args) < 2:
             raise Exception(f'Miss concurrency and req_num parameter')
 
         concurrency = int(args[0]) # 并发数
         req_num = int(args[1]) # 每个线程的请求数
-        log.debug(f"-- Concurrent({concurrency},{req_num}) start --")
+        log.debug(f"-- Concurrent(%s,%s) start --", concurrency, req_num)
         # 清空响应时间+错误次数
         self.res_times.clear()
         self.err_num = 0
 
         # 每个线程的处理
         def run_thread():
             for i in range(0, req_num):
@@ -124,15 +128,15 @@
         for t in range(concurrency):
             threads[t].start()
         for j in range(concurrency):
             threads[j].join()
         t2 = time.time()
         n = len(self.res_times)
         cost_time = t2 - t1
-        log.debug(f"-- Concurrent({concurrency},{req_num}) finish --")
+        log.debug(f"-- Concurrent(%s,%s) finish --", concurrency, req_num)
         log.debug("total costtime(s): %s", cost_time)
         log.debug('response num: %s', n)
         log.debug('success num: %s', n - self.err_num)
         log.debug('fail num: %s', self.err_num)
         log.debug('max costtime(s): %s', max(self.res_times))
         log.debug('min costtime(s): %s', min(self.res_times))
         log.debug('avg costtime(s): %s', sum(self.res_times) / n)
@@ -160,53 +164,63 @@
         # 添加基url
         if (self._base_url is not None) and ("http" not in url):
             url = self._base_url + url
         self.curr_url = url
         return url
 
     # 设置公共请求参数
-    # :param data
-    def common_data(self, data):
-        # self.session.params = replace_var(data, False) # 只挂在url的query参数中
-        self._common_data = replace_var(data, False) # 如果是get请求, 则挂在query参数, 否则挂在post参数中
+    # :param req
+    def common_req(self, req):
+        #  # self.session.headers = replace_var(req['headers'], False)
+        # self.session.params = replace_var(req['data'], False) # 只挂在url的query参数中
+        self._common_req.update(replace_var(req, False)) # 如果是get请求, 则挂在query参数, 否则挂在post参数中
 
-    # 构建参数
+    # 构建post参数
     def _get_data(self, config):
         if 'data' not in config:
-            return self._common_data
+            return self._common_req['data']
 
         # 当前参数
         curr_data = replace_var(config['data'], False)
         # 合并公共参数
-        if isinstance(self._common_data, dict):
+        if isinstance(self._common_req['data'], dict):
             r = {}
-            r.update(self._common_data)
+            r.update(self._common_req['data'])
             r.update(curr_data) # 公共参数会被当前参数覆盖
             return r
 
         return curr_data
 
-    # 设置公共请求头
-    # :param headers
-    def common_headers(self, headers):
-        # 经测试:两种实现是一样效果的
-        # self.session.headers = replace_var(headers, False)
-        self._common_headers = replace_var(headers, False)
+    # 构建json参数
+    def _get_json(self, config):
+        if 'json' not in config:
+            return self._common_req['json']
+
+        # 当前参数
+        curr_json = replace_var(config['json'], False)
+        # 合并公共参数
+        if isinstance(self._common_req['json'], dict):
+            r = {}
+            r.update(self._common_req['json'])
+            r.update(curr_json) # 公共参数会被当前参数覆盖
+            return r
+
+        return curr_json
 
     # 构建参数
     def _get_headers(self, config):
         if 'headers' not in config:
-            return self._common_headers
+            return self._common_req['headers']
 
         # 当前参数
         curr_headers = replace_var(config['headers'], False)
         # 合并公共参数
-        if isinstance(self._common_headers, dict):
+        if isinstance(self._common_req['headers'], dict):
             r = {}
-            r.update(self._common_headers)
+            r.update(self._common_req['headers'])
             r.update(curr_headers)  # 公共参数会被当前参数覆盖
             return r
 
         return curr_headers
 
     # 构建requests方法的其他参数
     # 如 verify: false 控制不检查https证书
@@ -232,17 +246,18 @@
         self._analyze_response(res, config)
 
     # post请求
     # :param config {url, headers, data, validate_by_jsonpath, validate_by_css, validate_by_xpath, extract_by_jsonpath, extract_by_css, extract_by_xpath, extract_by_eval}
     def post(self, config = {}):
         url = self._get_url(config)
         data = self._get_data(config)
+        json = self._get_json(config)
         headers = self._get_headers(config)
         opt = self._get_options(config)
-        res = self.session.post(url, headers=headers, data=data, **opt)
+        res = self.session.post(url, headers=headers, data=data, json=json, **opt)
         # 解析响应
         self._analyze_response(res, config)
 
     # 上传文件
     # :param config {url, headers, files, validate_by_jsonpath, validate_by_css, validate_by_xpath, extract_by_jsonpath, extract_by_css, extract_by_xpath, extract_by_eval}
     def upload(self, config = {}):
         url = self._get_url(config)
@@ -276,15 +291,15 @@
         res = self.session.get(url, headers=headers, data=data, **opt)
 
         # 保存响应的文件
         write_byte_file(save_file, res.content)
         # 设置变量
         set_var('download_file', save_file)
         self.downloaded_files[url] = save_file
-        log.debug(f"Dowload file: url is {url}, save path is{save_file}")
+        log.debug(f"Dowload file: url is %s, save path is %s", url, save_file)
         return save_file
 
     # 获得文件名
     # config['save_dir'] + config['save_file'] 或 url中的默认文件名
     def _prepare_save_file(self, config, url):
         # 获得保存的目录
         if 'save_dir' in config:
@@ -327,31 +342,31 @@
         # 1 使用 pytesseract 识别图片 -- wrong: 默认没训练过的识别不了
         # img = Image.open(file_path)
         # captcha = pytesseract.image_to_string(img)
         # 2 使用有道ocr
         captcha = ocr_youdao.recognize_text(file_path)
         # 设置变量
         set_var('captcha', captcha)
-        log.debug(f"Recognize captcha: image file is {file_path}, captcha is {captcha}")
+        log.debug(f"Recognize captcha: image file is %s, captcha is %s", file_path, captcha)
         # 删除文件
         #os.remove(file)
 
 # cli入口
 def main():
     # 基于yaml的执行器
     boot = HttpBoot()
     # 读元数据：author/version/description
     dir = os.path.dirname(__file__)
     meta = read_init_file_meta(dir + os.sep + '__init__.py')
     # 步骤配置的yaml
-    step_files = parse_cmd('HttpBoot', meta['version'])
+    step_files, option = parse_cmd('HttpBoot', meta['version'])
     if len(step_files) == 0:
         raise Exception("Miss step config file or directory")
     try:
         # 执行yaml配置的步骤
         boot.run(step_files)
     except Exception as ex:
-        log.error(f"Exception occurs: current step file is {boot.step_file}, current url is {boot.curr_url}", exc_info = ex)
+        log.error(f"Exception occurs: current step file is %s, current url is %s", boot.step_file, boot.curr_url, exc_info = ex)
         raise ex
 
 if __name__ == '__main__':
     main()
```

### Comparing `HttpBoot-1.0.8/HttpBoot/locust_boot.py` & `HttpBoot-1.0.9/HttpBoot/locust_boot.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
 import sys
-from locust import HttpUser, argument_parser,events
+from locust import HttpUser, FastHttpUser, argument_parser, events
 from pyutilb.util import *
+from pyutilb.file import *
 from HttpBoot.http_boot import HttpBoot
 
 
 # 将步骤yml添加为locust参数, 这样locust命令才不会校验报错
 @events.init_command_line_parser.add_listener
 def _(parser):
     parser.add_argument(
@@ -28,15 +29,20 @@
 # 根据步骤生成locust任务函数
 def build_task(steps):
     def run_task(self):
         self.boot.run_steps(steps)
     return run_task
 
 # user类
-class BootUser(HttpUser):
+# FastHttpUser 相对于 HttpUser 能提升5-6倍的并发量; 单个locust进程(1核cpu)下，FastHttpUser 可以做到16000 qps，HttpUser 做到 4000 qps
+if hasattr(os, 'posix_spawnp'):
+    UserClass = FastHttpUser
+else:
+    UserClass = HttpUser
+class BootUser(UserClass):
     tasks = [build_task(config['task'])] # task下的多个步骤只当做一个任务，反正locust监控的是请求级，而不是任务级
     host = config['base_url']
     min_wait = 1000
     max_wait = 5000
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
```

### Comparing `HttpBoot-1.0.8/HttpBoot/locust_main.py` & `HttpBoot-1.0.9/HttpBoot/locust_main.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,37 +1,43 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 import os
 import sys
-from pyutilb import log
+from pyutilb.log import log
 from pyutilb.util import *
+from pyutilb.file import *
+from pyutilb.cmd import *
 
 def main():
     try:
         # 读元数据：author/version/description
         dir = os.path.dirname(__file__)
         meta = read_init_file_meta(dir + os.sep + '__init__.py')
+
         # 步骤配置的yaml
-        step_files = parse_cmd('LocustBoot', meta['version'])
+        step_files, option = parse_cmd('LocustBoot', meta['version'])
         if len(step_files) == 0:
             raise Exception("Miss step config file")
         step_file = step_files[0]
 
-        # locust_file
-        #locust_file = os.path.abspath('locust_boot.py')
-        locust_file = __file__.replace('locust_main.py', 'locust_boot.py')
+        # 运行locust命令
+        run_locust_boot(step_file, option.locustopt)
+    except Exception as ex:
+        log.error(f"Exception occurs: current step file is %s", step_file, exc_info = ex)
+        raise ex
 
-        # 其他命令选项
+# 运行locust命令
+def run_locust_boot(step_file, options):
+    # locust_file
+    # locust_file = os.path.abspath('locust_boot.py')
+    locust_file = __file__.replace('locust_main.py', 'locust_boot.py')
+    # 选项
+    if options is None:
         options = ''
-        if len(sys.argv) > 2:
-            options = ' '.join(sys.argv[2:])
+    # 执行locust命令
+    cmd = f'locust -f {locust_file} -b {step_file} {options}'
+    log.debug(cmd)
+    os.system(cmd)
 
-        # 执行locust命令
-        cmd = f'locust -f {locust_file} -b {step_file} {options}'
-        log.debug(cmd)
-        os.system(cmd)
-    except Exception as ex:
-        log.error(f"Exception occurs: current step file is {step_file}", exc_info = ex)
-        raise ex
 
 if __name__ == '__main__':
     main()
```

### Comparing `HttpBoot-1.0.8/HttpBoot/response_wrapper.py` & `HttpBoot-1.0.9/HttpBoot/response_wrapper.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
 import re
 from pyutilb.util import *
+from pyutilb.file import *
 from lxml import etree
 from requests import Response
 from jsonpath import jsonpath
 
 # 响应包装器
 class ResponseWrap(object):
 
@@ -33,17 +34,14 @@
             data = self.res.json()
             return jsonpath(data, path)[0]
 
         if type == 'id':
             html = etree.parse(self.res.text, etree.HTMLParser())
             return html.get_element_by_id(path).text
 
-        if type == 'eval':
-            return eval(path, globals(), bvars) # 丢失本地与全局变量, 如引用不了json模块
-
         raise Exception(f"Invalid find type: {type}")
 
 
     # 获得元素的属性值或文本
     def get_prop_or_text(self, ele, prop):
         # 响应元素
         if isinstance(ele, etree._Element):
```

### Comparing `HttpBoot-1.0.8/HttpBoot.egg-info/PKG-INFO` & `HttpBoot-1.0.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: HttpBoot
-Version: 1.0.8
-Summary: HttpBoot: make an easy way (yaml) to HTTP(S) API automation testing, also support using yaml to call locust performance test
-Home-page: https://github.com/shigebeyond/HttpBoot
-Author: shigebeyond
-Author-email: 772910474@qq.com
-License: BSD
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Topic :: Software Development :: Testing
-Classifier: Topic :: Software Development :: Quality Assurance
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
 [GitHub](https://github.com/shigebeyond/HttpBoot) | [Gitee](https://gitee.com/shigebeyond/HttpBoot)
 
 # HttpBoot - yaml驱动http接口自动化测试+性能测试
 
 ## 概述
 一般测试http接口，要写python代码；
 
@@ -43,14 +21,21 @@
 3. 支持校验器
 4. 支持识别验证码(使用有道ocr)
 5. 支持类似python`for`/`if`/`break`语义的步骤动作，灵活适应各种场景
 6. 支持`include`引用其他的yaml配置文件，以便解耦与复用
 7. 支持用多线程来并发测试
 8. 整合locust来做压力测试
 
+## 同类yaml驱动测试框架
+[SeleniumBoot](https://github.com/shigebeyond/SeleniumBoot)
+[AppiumBoot](https://github.com/shigebeyond/AppiumBoot)
+[MiniumBoot](https://github.com/shigebeyond/MiniumBoot)
+[ExcelBoot](https://github.com/shigebeyond/ExcelBoot)
+[MonitorBoot](https://github.com/shigebeyond/MonitorBoot)
+
 ## todo
 1. 支持更多的动作
 
 ## 安装
 ```
 pip3 install HttpBoot
 ```
@@ -111,20 +96,20 @@
 
 每个步骤可以有多个动作，但单个步骤中动作名不能相同（yaml语法要求）;
 
 动作代表一种http请求，如get/post/upload等
 
 下面详细介绍每个动作:
 
-1. sleep: 线程睡眠; 
+1. sleep: 线程睡眠;
 ```yaml
 sleep: 2 # 线程睡眠2秒
 ```
 
-2. print: 打印, 支持输出变量/函数; 
+2. print: 打印, 支持输出变量/函数;
 ```yaml
 # 调试打印
 print: "总申请数=${dyn_data.total_apply}, 剩余份数=${dyn_data.quantity_remain}"
 ```
 
 变量格式:
 ```
@@ -146,78 +131,74 @@
 ```
 
 3. base_url: 设置基础url
 ```yaml
 base_url: https://www.taobao.com/
 ```
 
-4. common_data: 设置公共请求参数;
-如果是get请求, 则挂在query参数, 否则挂在post参数中
-```yaml
-common_data:
-    uid: 1
-```
-
-5. common_headers: 设置公共请求头
+4. common_req: 设置公共请求参数或请求头;
 ```yaml
-common_headers:
+common_req:
+  data: # 请求参数: 如果是get请求, 则挂在query参数, 否则挂在post参数中
     uid: 1
+  headers: # 请求头
+    token: "110"
 ```
 
-6. get: 发get请求; 
+5. get: 发get请求;
 ```yaml
 get:
     url: $dyn_data_url # url,支持写变量, 如果设置了base_url, 则可以写相对url
     extract_by_eval:
       dyn_data: "json.loads(response.text[16:-1])" # 变量response是响应对象
 ```
 
-7. post: 发post请求; 
+6. post: 发post请求;
 ```yaml
 post:
     url: http://admin.jym1.com/store/add_store # url,支持写变量, 如果设置了base_url, 则可以写相对url
     is_ajax: true
     data: # post的参数
       # 参数名:参数值
       store_name: teststore-${random_str(6)}
       store_logo_url: '$img'
 ```
 
-8. upload: 上传文件; 
+7. upload: 上传文件;
 ```yaml
 upload: # 上传文件/图片
     url: http://admin.jym1.com/upload/common_upload_img/store_img # url,支持写变量, 如果设置了base_url, 则可以写相对url
     files: # 上传的多个文件
       # 参数名:文件本地路径
       file: /home/shi/fruit.jpeg
     extract_by_jsonpath:
       img: $.data.url
 ```
 
-9. download: 下载文件; 
-变量`download_file`记录最新下载的单个文件
+8. download: 下载文件;
+   变量`download_file`记录最新下载的单个文件
 ```yaml
 download:
     url: https://img.alicdn.com/tfscom/TB1t84NPuL2gK0jSZPhXXahvXXa.jpg_q90.jpg # url,支持写变量, 如果设置了base_url, 则可以写相对url
     save_dir: downloads # 保存的目录，默认为 downloads
     save_file: test.jpg # 保存的文件名，默认为url中最后一级的文件名
 ```
 
-10. recognize_captcha: 识别验证码; 
-参数同 `download` 动作， 因为内部就是调用 `download`;
-而变量`captcha`记录识别出来的验证码
+9. recognize_captcha: 识别验证码;
+   参数同 `download` 动作， 因为内部就是调用 `download`;
+   而变量`captcha`记录识别出来的验证码
 ```
 recognize_captcha:
     url: http://admin.jym1.com/login/verify_image
     # save_dir: downloads # 保存的目录，默认为 downloads
     # save_file: test.jpg # 保存的文件名，默认为url中最后一级的文件名
 ```
 
-11. for: 循环; 
-for动作下包含一系列子步骤，表示循环执行这系列子步骤；变量`for_i`记录是第几次迭代（从1开始）,变量`for_v`记录是每次迭代的元素值（仅当是list类型的变量迭代时有效）
+10. for: 循环;
+    for动作下包含一系列子步骤，表示循环执行这系列子步骤；变量`for_i`记录是第几次迭代（从1开始）,变量`for_v`记录是每次迭代的元素值（仅当是list类型的变量迭代时有效）
 ```yaml
 # 循环3次
 for(3) :
   # 每次迭代要执行的子步骤
   - get:
       url: https://www.baidu.com
     sleep: 2
@@ -235,59 +216,69 @@
   # 每次迭代要执行的子步骤
   - break_if: for_i>2 # 满足条件则跳出循环
     get:
       url: https://www.baidu.com
     sleep: 2
 ```
 
-12. once: 只执行一次，等价于 `for(1)`; 
-once 结合 moveon_if，可以模拟 python 的 `if` 语法效果
+11. once: 只执行一次，等价于 `for(1)`;
+    once 结合 moveon_if，可以模拟 python 的 `if` 语法效果
 ```yaml
 once:
   # 每次迭代要执行的子步骤
   - moveon_if: for_i<=2 # 满足条件则往下走，否则跳出循环
     get:
       url: https://www.baidu.com
     sleep: 2
 ```
 
-13. break_if: 满足条件则跳出循环; 
-只能定义在for/once循环的子步骤中
+12. break_if: 满足条件则跳出循环;
+    只能定义在for/once循环的子步骤中
 ```yaml
 break_if: for_i>2 # 条件表达式，python语法
 ```
 
-14. moveon_if: 满足条件则往下走，否则跳出循环; 
-只能定义在for/once循环的子步骤中
+13. moveon_if: 满足条件则往下走，否则跳出循环;
+    只能定义在for/once循环的子步骤中
 ```yaml
 moveon_if: for_i<=2 # 条件表达式，python语法
 ```
 
-15. 并发处理 
+14. if/else: 满足条件则执行if分支，否则执行else分支
+```yaml
+- extract_by_css:
+    txt: '#J_NewIndexTipBtn'
+- if(txt=='进入首页'): # 括号中包含的是布尔表达式，如果表达式结果为true，则执行if动作下的子步骤，否则执行else动作下的子步骤
+    - print: '----- 执行if -----'
+  else:
+    - print: '----- 执行else -----'
+```
+
+15. 并发处理
 ```yaml
 concurrent(5,10): # 并发线程数为5, 每线程处理请求数据为10
   # 每次迭代要执行的子步骤
   - get:
       url: https://www.baidu.com
 ```
 
-16. include: 包含其他步骤文件，如记录公共的步骤，或记录配置数据(如用户名密码); 
+16. include: 包含其他步骤文件，如记录公共的步骤，或记录配置数据(如用户名密码);
 ```yaml
 include: part-common.yml
 ```
 
-17. set_vars: 设置变量; 
+17. set_vars: 设置变量;
 ```yaml
 set_vars:
   name: shi
   password: 123456
   birthday: 5-27
 ```
 
-18. print_vars: 打印所有变量; 
+18. print_vars: 打印所有变量;
 ```yaml
 print_vars:
 ```
 
 19. exec: 执行命令, 可用于执行 HttpBoot/SeleniumBoot/AppiumBoot/MiniumBoot 等命令，以便打通多端的用例流程
 ```yaml
 exec: ls
@@ -302,42 +293,65 @@
 ```yaml
 validate_by_xpath:
   "//div[@id='goods_id']": # 元素的xpath路径
     '>': 0 # 校验符号或函数: 校验的值, 即 id 元素的值>0
   "//div[@id='goods_title']":
     contains: 衬衫 # 即 title 元素的值包含'衬衫'
 ```
+可简写为:
+```yaml
+validate_by_xpath:
+  - "//div[@id='goods_id'] > 0"
+  - "//div[@id='goods_title'] contains 衬衫"
+```
 
 2. validate_by_css: 
 从html的响应中解析 css selector 模式对应的元素的值
 ```yaml
 validate_by_css:
   '#id': # 元素的css selector 模式
     '>': 0 # 校验符号或函数: 校验的值, 即 id 元素的值>0
   '#goods_title':
     contains: 衬衫 # 即 title 元素的值包含'衬衫'
 ```
+可简写为:
+```yaml
+validate_by_css:
+  - '#id > 0'
+  - '#goods_title contains 衬衫'
+```
 
 3. validate_by_jsonpath: 
 从json响应中解析 多层属性 的值
 ```yaml
 validate_by_jsonpath:
   '$.data.goods_id':
      '>': 0 # 校验符号或函数: 校验的值, 即 id 元素的值>0
   '$.data.goods_title':
     contains: 衬衫 # 即 title 元素的值包含'衬衫'
 ```
+可简写为:
+```yaml
+validate_by_jsonpath:
+  - '$.data.goods_id > 0'
+  - '$.data.goods_title contains 衬衫'
+```
 
 4. validate_by_eval:
 使用 `eval(表达式)` 执行表达式, 并校验执行结果
 ```yaml
 validate_by_eval:
   'response.status_code':
     '=': 200
 ```
+可简写为:
+```yaml
+validate_by_eval:
+  - 'response.status_code = 200'
+```
 
 #### 校验符号或函数
 1. `=`: 相同
 2. `>`: 大于
 3. `<`: 小于
 4. `>=`: 大于等于
 5. `<=`: 小于等于
@@ -377,8 +391,8 @@
 
 4. extract_by_eval:
 使用 `eval(表达式)` 执行表达式, 并将执行结果记录到变量中
 ```yaml
 extract_by_eval:
     # 变量名: 表达式（python语法）
     dyn_data: "json.loads(response.text[16:-1])" # 变量response是响应对象
-```
+```
```

### Comparing `HttpBoot-1.0.8/PKG-INFO` & `HttpBoot-1.0.9/HttpBoot.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HttpBoot
-Version: 1.0.8
+Version: 1.0.9
 Summary: HttpBoot: make an easy way (yaml) to HTTP(S) API automation testing, also support using yaml to call locust performance test
 Home-page: https://github.com/shigebeyond/HttpBoot
 Author: shigebeyond
 Author-email: 772910474@qq.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Testing
@@ -43,14 +43,21 @@
 3. 支持校验器
 4. 支持识别验证码(使用有道ocr)
 5. 支持类似python`for`/`if`/`break`语义的步骤动作，灵活适应各种场景
 6. 支持`include`引用其他的yaml配置文件，以便解耦与复用
 7. 支持用多线程来并发测试
 8. 整合locust来做压力测试
 
+## 同类yaml驱动测试框架
+[SeleniumBoot](https://github.com/shigebeyond/SeleniumBoot)
+[AppiumBoot](https://github.com/shigebeyond/AppiumBoot)
+[MiniumBoot](https://github.com/shigebeyond/MiniumBoot)
+[ExcelBoot](https://github.com/shigebeyond/ExcelBoot)
+[MonitorBoot](https://github.com/shigebeyond/MonitorBoot)
+
 ## todo
 1. 支持更多的动作
 
 ## 安装
 ```
 pip3 install HttpBoot
 ```
@@ -111,20 +118,20 @@
 
 每个步骤可以有多个动作，但单个步骤中动作名不能相同（yaml语法要求）;
 
 动作代表一种http请求，如get/post/upload等
 
 下面详细介绍每个动作:
 
-1. sleep: 线程睡眠; 
+1. sleep: 线程睡眠;
 ```yaml
 sleep: 2 # 线程睡眠2秒
 ```
 
-2. print: 打印, 支持输出变量/函数; 
+2. print: 打印, 支持输出变量/函数;
 ```yaml
 # 调试打印
 print: "总申请数=${dyn_data.total_apply}, 剩余份数=${dyn_data.quantity_remain}"
 ```
 
 变量格式:
 ```
@@ -146,78 +153,74 @@
 ```
 
 3. base_url: 设置基础url
 ```yaml
 base_url: https://www.taobao.com/
 ```
 
-4. common_data: 设置公共请求参数;
-如果是get请求, 则挂在query参数, 否则挂在post参数中
-```yaml
-common_data:
-    uid: 1
-```
-
-5. common_headers: 设置公共请求头
+4. common_req: 设置公共请求参数或请求头;
 ```yaml
-common_headers:
+common_req:
+  data: # 请求参数: 如果是get请求, 则挂在query参数, 否则挂在post参数中
     uid: 1
+  headers: # 请求头
+    token: "110"
 ```
 
-6. get: 发get请求; 
+5. get: 发get请求;
 ```yaml
 get:
     url: $dyn_data_url # url,支持写变量, 如果设置了base_url, 则可以写相对url
     extract_by_eval:
       dyn_data: "json.loads(response.text[16:-1])" # 变量response是响应对象
 ```
 
-7. post: 发post请求; 
+6. post: 发post请求;
 ```yaml
 post:
     url: http://admin.jym1.com/store/add_store # url,支持写变量, 如果设置了base_url, 则可以写相对url
     is_ajax: true
     data: # post的参数
       # 参数名:参数值
       store_name: teststore-${random_str(6)}
       store_logo_url: '$img'
 ```
 
-8. upload: 上传文件; 
+7. upload: 上传文件;
 ```yaml
 upload: # 上传文件/图片
     url: http://admin.jym1.com/upload/common_upload_img/store_img # url,支持写变量, 如果设置了base_url, 则可以写相对url
     files: # 上传的多个文件
       # 参数名:文件本地路径
       file: /home/shi/fruit.jpeg
     extract_by_jsonpath:
       img: $.data.url
 ```
 
-9. download: 下载文件; 
-变量`download_file`记录最新下载的单个文件
+8. download: 下载文件;
+   变量`download_file`记录最新下载的单个文件
 ```yaml
 download:
     url: https://img.alicdn.com/tfscom/TB1t84NPuL2gK0jSZPhXXahvXXa.jpg_q90.jpg # url,支持写变量, 如果设置了base_url, 则可以写相对url
     save_dir: downloads # 保存的目录，默认为 downloads
     save_file: test.jpg # 保存的文件名，默认为url中最后一级的文件名
 ```
 
-10. recognize_captcha: 识别验证码; 
-参数同 `download` 动作， 因为内部就是调用 `download`;
-而变量`captcha`记录识别出来的验证码
+9. recognize_captcha: 识别验证码;
+   参数同 `download` 动作， 因为内部就是调用 `download`;
+   而变量`captcha`记录识别出来的验证码
 ```
 recognize_captcha:
     url: http://admin.jym1.com/login/verify_image
     # save_dir: downloads # 保存的目录，默认为 downloads
     # save_file: test.jpg # 保存的文件名，默认为url中最后一级的文件名
 ```
 
-11. for: 循环; 
-for动作下包含一系列子步骤，表示循环执行这系列子步骤；变量`for_i`记录是第几次迭代（从1开始）,变量`for_v`记录是每次迭代的元素值（仅当是list类型的变量迭代时有效）
+10. for: 循环;
+    for动作下包含一系列子步骤，表示循环执行这系列子步骤；变量`for_i`记录是第几次迭代（从1开始）,变量`for_v`记录是每次迭代的元素值（仅当是list类型的变量迭代时有效）
 ```yaml
 # 循环3次
 for(3) :
   # 每次迭代要执行的子步骤
   - get:
       url: https://www.baidu.com
     sleep: 2
@@ -235,59 +238,69 @@
   # 每次迭代要执行的子步骤
   - break_if: for_i>2 # 满足条件则跳出循环
     get:
       url: https://www.baidu.com
     sleep: 2
 ```
 
-12. once: 只执行一次，等价于 `for(1)`; 
-once 结合 moveon_if，可以模拟 python 的 `if` 语法效果
+11. once: 只执行一次，等价于 `for(1)`;
+    once 结合 moveon_if，可以模拟 python 的 `if` 语法效果
 ```yaml
 once:
   # 每次迭代要执行的子步骤
   - moveon_if: for_i<=2 # 满足条件则往下走，否则跳出循环
     get:
       url: https://www.baidu.com
     sleep: 2
 ```
 
-13. break_if: 满足条件则跳出循环; 
-只能定义在for/once循环的子步骤中
+12. break_if: 满足条件则跳出循环;
+    只能定义在for/once循环的子步骤中
 ```yaml
 break_if: for_i>2 # 条件表达式，python语法
 ```
 
-14. moveon_if: 满足条件则往下走，否则跳出循环; 
-只能定义在for/once循环的子步骤中
+13. moveon_if: 满足条件则往下走，否则跳出循环;
+    只能定义在for/once循环的子步骤中
 ```yaml
 moveon_if: for_i<=2 # 条件表达式，python语法
 ```
 
-15. 并发处理 
+14. if/else: 满足条件则执行if分支，否则执行else分支
+```yaml
+- extract_by_css:
+    txt: '#J_NewIndexTipBtn'
+- if(txt=='进入首页'): # 括号中包含的是布尔表达式，如果表达式结果为true，则执行if动作下的子步骤，否则执行else动作下的子步骤
+    - print: '----- 执行if -----'
+  else:
+    - print: '----- 执行else -----'
+```
+
+15. 并发处理
 ```yaml
 concurrent(5,10): # 并发线程数为5, 每线程处理请求数据为10
   # 每次迭代要执行的子步骤
   - get:
       url: https://www.baidu.com
 ```
 
-16. include: 包含其他步骤文件，如记录公共的步骤，或记录配置数据(如用户名密码); 
+16. include: 包含其他步骤文件，如记录公共的步骤，或记录配置数据(如用户名密码);
 ```yaml
 include: part-common.yml
 ```
 
-17. set_vars: 设置变量; 
+17. set_vars: 设置变量;
 ```yaml
 set_vars:
   name: shi
   password: 123456
   birthday: 5-27
 ```
 
-18. print_vars: 打印所有变量; 
+18. print_vars: 打印所有变量;
 ```yaml
 print_vars:
 ```
 
 19. exec: 执行命令, 可用于执行 HttpBoot/SeleniumBoot/AppiumBoot/MiniumBoot 等命令，以便打通多端的用例流程
 ```yaml
 exec: ls
@@ -302,42 +315,65 @@
 ```yaml
 validate_by_xpath:
   "//div[@id='goods_id']": # 元素的xpath路径
     '>': 0 # 校验符号或函数: 校验的值, 即 id 元素的值>0
   "//div[@id='goods_title']":
     contains: 衬衫 # 即 title 元素的值包含'衬衫'
 ```
+可简写为:
+```yaml
+validate_by_xpath:
+  - "//div[@id='goods_id'] > 0"
+  - "//div[@id='goods_title'] contains 衬衫"
+```
 
 2. validate_by_css: 
 从html的响应中解析 css selector 模式对应的元素的值
 ```yaml
 validate_by_css:
   '#id': # 元素的css selector 模式
     '>': 0 # 校验符号或函数: 校验的值, 即 id 元素的值>0
   '#goods_title':
     contains: 衬衫 # 即 title 元素的值包含'衬衫'
 ```
+可简写为:
+```yaml
+validate_by_css:
+  - '#id > 0'
+  - '#goods_title contains 衬衫'
+```
 
 3. validate_by_jsonpath: 
 从json响应中解析 多层属性 的值
 ```yaml
 validate_by_jsonpath:
   '$.data.goods_id':
      '>': 0 # 校验符号或函数: 校验的值, 即 id 元素的值>0
   '$.data.goods_title':
     contains: 衬衫 # 即 title 元素的值包含'衬衫'
 ```
+可简写为:
+```yaml
+validate_by_jsonpath:
+  - '$.data.goods_id > 0'
+  - '$.data.goods_title contains 衬衫'
+```
 
 4. validate_by_eval:
 使用 `eval(表达式)` 执行表达式, 并校验执行结果
 ```yaml
 validate_by_eval:
   'response.status_code':
     '=': 200
 ```
+可简写为:
+```yaml
+validate_by_eval:
+  - 'response.status_code = 200'
+```
 
 #### 校验符号或函数
 1. `=`: 相同
 2. `>`: 大于
 3. `<`: 小于
 4. `>=`: 大于等于
 5. `<=`: 小于等于
```

### Comparing `HttpBoot-1.0.8/README.md` & `HttpBoot-1.0.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: HttpBoot
+Version: 1.0.9
+Summary: HttpBoot: make an easy way (yaml) to HTTP(S) API automation testing, also support using yaml to call locust performance test
+Home-page: https://github.com/shigebeyond/HttpBoot
+Author: shigebeyond
+Author-email: 772910474@qq.com
+License: BSD
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Topic :: Software Development :: Testing
+Classifier: Topic :: Software Development :: Quality Assurance
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+
 [GitHub](https://github.com/shigebeyond/HttpBoot) | [Gitee](https://gitee.com/shigebeyond/HttpBoot)
 
 # HttpBoot - yaml驱动http接口自动化测试+性能测试
 
 ## 概述
 一般测试http接口，要写python代码；
 
@@ -21,14 +43,21 @@
 3. 支持校验器
 4. 支持识别验证码(使用有道ocr)
 5. 支持类似python`for`/`if`/`break`语义的步骤动作，灵活适应各种场景
 6. 支持`include`引用其他的yaml配置文件，以便解耦与复用
 7. 支持用多线程来并发测试
 8. 整合locust来做压力测试
 
+## 同类yaml驱动测试框架
+[SeleniumBoot](https://github.com/shigebeyond/SeleniumBoot)
+[AppiumBoot](https://github.com/shigebeyond/AppiumBoot)
+[MiniumBoot](https://github.com/shigebeyond/MiniumBoot)
+[ExcelBoot](https://github.com/shigebeyond/ExcelBoot)
+[MonitorBoot](https://github.com/shigebeyond/MonitorBoot)
+
 ## todo
 1. 支持更多的动作
 
 ## 安装
 ```
 pip3 install HttpBoot
 ```
@@ -89,20 +118,20 @@
 
 每个步骤可以有多个动作，但单个步骤中动作名不能相同（yaml语法要求）;
 
 动作代表一种http请求，如get/post/upload等
 
 下面详细介绍每个动作:
 
-1. sleep: 线程睡眠; 
+1. sleep: 线程睡眠;
 ```yaml
 sleep: 2 # 线程睡眠2秒
 ```
 
-2. print: 打印, 支持输出变量/函数; 
+2. print: 打印, 支持输出变量/函数;
 ```yaml
 # 调试打印
 print: "总申请数=${dyn_data.total_apply}, 剩余份数=${dyn_data.quantity_remain}"
 ```
 
 变量格式:
 ```
@@ -124,78 +153,74 @@
 ```
 
 3. base_url: 设置基础url
 ```yaml
 base_url: https://www.taobao.com/
 ```
 
-4. common_data: 设置公共请求参数;
-如果是get请求, 则挂在query参数, 否则挂在post参数中
-```yaml
-common_data:
-    uid: 1
-```
-
-5. common_headers: 设置公共请求头
+4. common_req: 设置公共请求参数或请求头;
 ```yaml
-common_headers:
+common_req:
+  data: # 请求参数: 如果是get请求, 则挂在query参数, 否则挂在post参数中
     uid: 1
+  headers: # 请求头
+    token: "110"
 ```
 
-6. get: 发get请求; 
+5. get: 发get请求;
 ```yaml
 get:
     url: $dyn_data_url # url,支持写变量, 如果设置了base_url, 则可以写相对url
     extract_by_eval:
       dyn_data: "json.loads(response.text[16:-1])" # 变量response是响应对象
 ```
 
-7. post: 发post请求; 
+6. post: 发post请求;
 ```yaml
 post:
     url: http://admin.jym1.com/store/add_store # url,支持写变量, 如果设置了base_url, 则可以写相对url
     is_ajax: true
     data: # post的参数
       # 参数名:参数值
       store_name: teststore-${random_str(6)}
       store_logo_url: '$img'
 ```
 
-8. upload: 上传文件; 
+7. upload: 上传文件;
 ```yaml
 upload: # 上传文件/图片
     url: http://admin.jym1.com/upload/common_upload_img/store_img # url,支持写变量, 如果设置了base_url, 则可以写相对url
     files: # 上传的多个文件
       # 参数名:文件本地路径
       file: /home/shi/fruit.jpeg
     extract_by_jsonpath:
       img: $.data.url
 ```
 
-9. download: 下载文件; 
-变量`download_file`记录最新下载的单个文件
+8. download: 下载文件;
+   变量`download_file`记录最新下载的单个文件
 ```yaml
 download:
     url: https://img.alicdn.com/tfscom/TB1t84NPuL2gK0jSZPhXXahvXXa.jpg_q90.jpg # url,支持写变量, 如果设置了base_url, 则可以写相对url
     save_dir: downloads # 保存的目录，默认为 downloads
     save_file: test.jpg # 保存的文件名，默认为url中最后一级的文件名
 ```
 
-10. recognize_captcha: 识别验证码; 
-参数同 `download` 动作， 因为内部就是调用 `download`;
-而变量`captcha`记录识别出来的验证码
+9. recognize_captcha: 识别验证码;
+   参数同 `download` 动作， 因为内部就是调用 `download`;
+   而变量`captcha`记录识别出来的验证码
 ```
 recognize_captcha:
     url: http://admin.jym1.com/login/verify_image
     # save_dir: downloads # 保存的目录，默认为 downloads
     # save_file: test.jpg # 保存的文件名，默认为url中最后一级的文件名
 ```
 
-11. for: 循环; 
-for动作下包含一系列子步骤，表示循环执行这系列子步骤；变量`for_i`记录是第几次迭代（从1开始）,变量`for_v`记录是每次迭代的元素值（仅当是list类型的变量迭代时有效）
+10. for: 循环;
+    for动作下包含一系列子步骤，表示循环执行这系列子步骤；变量`for_i`记录是第几次迭代（从1开始）,变量`for_v`记录是每次迭代的元素值（仅当是list类型的变量迭代时有效）
 ```yaml
 # 循环3次
 for(3) :
   # 每次迭代要执行的子步骤
   - get:
       url: https://www.baidu.com
     sleep: 2
@@ -213,59 +238,69 @@
   # 每次迭代要执行的子步骤
   - break_if: for_i>2 # 满足条件则跳出循环
     get:
       url: https://www.baidu.com
     sleep: 2
 ```
 
-12. once: 只执行一次，等价于 `for(1)`; 
-once 结合 moveon_if，可以模拟 python 的 `if` 语法效果
+11. once: 只执行一次，等价于 `for(1)`;
+    once 结合 moveon_if，可以模拟 python 的 `if` 语法效果
 ```yaml
 once:
   # 每次迭代要执行的子步骤
   - moveon_if: for_i<=2 # 满足条件则往下走，否则跳出循环
     get:
       url: https://www.baidu.com
     sleep: 2
 ```
 
-13. break_if: 满足条件则跳出循环; 
-只能定义在for/once循环的子步骤中
+12. break_if: 满足条件则跳出循环;
+    只能定义在for/once循环的子步骤中
 ```yaml
 break_if: for_i>2 # 条件表达式，python语法
 ```
 
-14. moveon_if: 满足条件则往下走，否则跳出循环; 
-只能定义在for/once循环的子步骤中
+13. moveon_if: 满足条件则往下走，否则跳出循环;
+    只能定义在for/once循环的子步骤中
 ```yaml
 moveon_if: for_i<=2 # 条件表达式，python语法
 ```
 
-15. 并发处理 
+14. if/else: 满足条件则执行if分支，否则执行else分支
+```yaml
+- extract_by_css:
+    txt: '#J_NewIndexTipBtn'
+- if(txt=='进入首页'): # 括号中包含的是布尔表达式，如果表达式结果为true，则执行if动作下的子步骤，否则执行else动作下的子步骤
+    - print: '----- 执行if -----'
+  else:
+    - print: '----- 执行else -----'
+```
+
+15. 并发处理
 ```yaml
 concurrent(5,10): # 并发线程数为5, 每线程处理请求数据为10
   # 每次迭代要执行的子步骤
   - get:
       url: https://www.baidu.com
 ```
 
-16. include: 包含其他步骤文件，如记录公共的步骤，或记录配置数据(如用户名密码); 
+16. include: 包含其他步骤文件，如记录公共的步骤，或记录配置数据(如用户名密码);
 ```yaml
 include: part-common.yml
 ```
 
-17. set_vars: 设置变量; 
+17. set_vars: 设置变量;
 ```yaml
 set_vars:
   name: shi
   password: 123456
   birthday: 5-27
 ```
 
-18. print_vars: 打印所有变量; 
+18. print_vars: 打印所有变量;
 ```yaml
 print_vars:
 ```
 
 19. exec: 执行命令, 可用于执行 HttpBoot/SeleniumBoot/AppiumBoot/MiniumBoot 等命令，以便打通多端的用例流程
 ```yaml
 exec: ls
@@ -280,42 +315,65 @@
 ```yaml
 validate_by_xpath:
   "//div[@id='goods_id']": # 元素的xpath路径
     '>': 0 # 校验符号或函数: 校验的值, 即 id 元素的值>0
   "//div[@id='goods_title']":
     contains: 衬衫 # 即 title 元素的值包含'衬衫'
 ```
+可简写为:
+```yaml
+validate_by_xpath:
+  - "//div[@id='goods_id'] > 0"
+  - "//div[@id='goods_title'] contains 衬衫"
+```
 
 2. validate_by_css: 
 从html的响应中解析 css selector 模式对应的元素的值
 ```yaml
 validate_by_css:
   '#id': # 元素的css selector 模式
     '>': 0 # 校验符号或函数: 校验的值, 即 id 元素的值>0
   '#goods_title':
     contains: 衬衫 # 即 title 元素的值包含'衬衫'
 ```
+可简写为:
+```yaml
+validate_by_css:
+  - '#id > 0'
+  - '#goods_title contains 衬衫'
+```
 
 3. validate_by_jsonpath: 
 从json响应中解析 多层属性 的值
 ```yaml
 validate_by_jsonpath:
   '$.data.goods_id':
      '>': 0 # 校验符号或函数: 校验的值, 即 id 元素的值>0
   '$.data.goods_title':
     contains: 衬衫 # 即 title 元素的值包含'衬衫'
 ```
+可简写为:
+```yaml
+validate_by_jsonpath:
+  - '$.data.goods_id > 0'
+  - '$.data.goods_title contains 衬衫'
+```
 
 4. validate_by_eval:
 使用 `eval(表达式)` 执行表达式, 并校验执行结果
 ```yaml
 validate_by_eval:
   'response.status_code':
     '=': 200
 ```
+可简写为:
+```yaml
+validate_by_eval:
+  - 'response.status_code = 200'
+```
 
 #### 校验符号或函数
 1. `=`: 相同
 2. `>`: 大于
 3. `<`: 小于
 4. `>=`: 大于等于
 5. `<=`: 小于等于
@@ -355,8 +413,8 @@
 
 4. extract_by_eval:
 使用 `eval(表达式)` 执行表达式, 并将执行结果记录到变量中
 ```yaml
 extract_by_eval:
     # 变量名: 表达式（python语法）
     dyn_data: "json.loads(response.text[16:-1])" # 变量response是响应对象
-```
+```
```

### Comparing `HttpBoot-1.0.8/setup.py` & `HttpBoot-1.0.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # coding=utf-8
 import re
 import ast
 from setuptools import setup, find_packages
 from os.path import dirname, join, abspath
 import setuptools
 from pyutilb.util import *
+from pyutilb.file import *
+from pyutilb.cmd import *
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 # 读元数据：author/version/description
 meta = read_init_file_meta('HttpBoot/__init__.py')
```

