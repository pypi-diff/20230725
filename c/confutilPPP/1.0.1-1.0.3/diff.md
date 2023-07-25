# Comparing `tmp/confutilPPP-1.0.1.tar.gz` & `tmp/confutilPPP-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "confutilPPP-1.0.1.tar", last modified: Wed Jul 12 11:12:32 2023, max compression
+gzip compressed data, was "confutilPPP-1.0.3.tar", last modified: Tue Jul 25 14:06:59 2023, max compression
```

## Comparing `confutilPPP-1.0.1.tar` & `confutilPPP-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 11:12:32.641007 confutilPPP-1.0.1/
--rw-rw-rw-   0        0        0      157 2023-07-12 11:12:32.640007 confutilPPP-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       80 2023-07-11 17:32:43.000000 confutilPPP-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-12 11:12:32.635449 confutilPPP-1.0.1/confutilPPP.egg-info/
--rw-rw-rw-   0        0        0      157 2023-07-12 11:12:32.000000 confutilPPP-1.0.1/confutilPPP.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2023-07-12 11:12:32.000000 confutilPPP-1.0.1/confutilPPP.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 11:12:32.000000 confutilPPP-1.0.1/confutilPPP.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-07-12 11:12:32.000000 confutilPPP-1.0.1/confutilPPP.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-12 11:12:32.000000 confutilPPP-1.0.1/confutilPPP.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-12 11:12:32.641007 confutilPPP-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      463 2023-07-12 10:58:48.000000 confutilPPP-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-12 11:12:32.628468 confutilPPP-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-12 11:12:32.638441 confutilPPP-1.0.1/src/confutilPPP/
--rw-rw-rw-   0        0        0      203 2023-07-12 10:57:03.000000 confutilPPP-1.0.1/src/confutilPPP/__init__.py
--rw-rw-rw-   0        0        0     2154 2023-07-11 17:14:17.000000 confutilPPP-1.0.1/src/confutilPPP/_confutil.py
+drwxrwxrwx   0        0        0        0 2023-07-25 14:06:59.916196 confutilPPP-1.0.3/
+-rw-rw-rw-   0        0        0      157 2023-07-25 14:06:59.916196 confutilPPP-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      391 2023-07-25 13:32:01.000000 confutilPPP-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 14:06:59.900579 confutilPPP-1.0.3/confutilPPP.egg-info/
+-rw-rw-rw-   0        0        0      157 2023-07-25 14:06:59.000000 confutilPPP-1.0.3/confutilPPP.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2023-07-25 14:06:59.000000 confutilPPP-1.0.3/confutilPPP.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 14:06:59.000000 confutilPPP-1.0.3/confutilPPP.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-07-25 14:06:59.000000 confutilPPP-1.0.3/confutilPPP.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-25 14:06:59.000000 confutilPPP-1.0.3/confutilPPP.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-25 14:06:59.916196 confutilPPP-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      463 2023-07-12 10:58:48.000000 confutilPPP-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 14:06:59.900579 confutilPPP-1.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-07-25 14:06:59.900579 confutilPPP-1.0.3/src/confutilPPP/
+-rw-rw-rw-   0        0        0      205 2023-07-25 14:05:05.000000 confutilPPP-1.0.3/src/confutilPPP/__init__.py
+-rw-rw-rw-   0        0        0     2310 2023-07-25 13:26:52.000000 confutilPPP-1.0.3/src/confutilPPP/_confutil.py
```

### Comparing `confutilPPP-1.0.1/src/confutilPPP/_confutil.py` & `confutilPPP-1.0.3/src/confutilPPP/_confutil.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,22 +14,23 @@
     def _parse_arguments():
         parser = argparse.ArgumentParser()
         parser.add_argument("--configpath", nargs="+", help="配置文件")
         return parser.parse_args()
 
     # 检查解析参数
     @staticmethod
-    def check_config(_object=None, filename='config'):
-        if _object is None:
-            _object = {}
+    def check_config(_object=None, _filename='config'):
         # 解析参数
         args = confutil._parse_arguments()
         args_config_path = args.configpath
         # 默认自定义配置
-        default_path = os.path.join(os.getcwd(), f'{filename}.yaml')
+        default_path = os.path.join(os.getcwd(), f'{_filename}.yaml')
+        # 如果*.yaml文件不存在或者为空
+        if not os.path.isfile(default_path) or os.path.getsize(default_path) == 0:
+            default_path = os.path.join(os.getcwd(), f'{_filename}.yml')
         if not args_config_path:
             logPPP.warning("未填写自定义配置文件路径参数.")
         else:
             default_path = args_config_path[0]  # 自定义配置
         config_full_path_ = os.path.join(os.getcwd(), default_path)
 
         # 如果文件不存在或者为空，创建文件并写入
```

