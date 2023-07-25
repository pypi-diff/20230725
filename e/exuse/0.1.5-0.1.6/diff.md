# Comparing `tmp/exuse-0.1.5.tar.gz` & `tmp/exuse-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exuse-0.1.5.tar", last modified: Tue Sep 27 02:17:19 2022, max compression
+gzip compressed data, was "exuse-0.1.6.tar", last modified: Tue Jul 25 02:31:19 2023, max compression
```

## Comparing `exuse-0.1.5.tar` & `exuse-0.1.6.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 barwe     (1000) barwe     (1000)        0 2022-09-27 02:17:19.545401 exuse-0.1.5/
--rw-r--r--   0 barwe     (1000) barwe     (1000)      210 2022-09-27 02:17:19.545401 exuse-0.1.5/PKG-INFO
--rw-r--r--   0 barwe     (1000) barwe     (1000)     1302 2022-09-27 02:17:12.000000 exuse-0.1.5/README.md
-drwxr-xr-x   0 barwe     (1000) barwe     (1000)        0 2022-09-27 02:17:19.545401 exuse-0.1.5/exuse/
--rw-r--r--   0 barwe     (1000) barwe     (1000)      296 2022-09-19 07:38:42.000000 exuse-0.1.5/exuse/__init__.py
--rw-r--r--   0 barwe     (1000) barwe     (1000)     4352 2022-09-27 02:16:53.000000 exuse-0.1.5/exuse/exargparse.py
--rw-r--r--   0 barwe     (1000) barwe     (1000)      916 2022-09-20 12:25:42.000000 exuse-0.1.5/exuse/exio.py
--rw-r--r--   0 barwe     (1000) barwe     (1000)      558 2022-09-20 02:33:12.000000 exuse-0.1.5/exuse/exlogging.py
--rw-r--r--   0 barwe     (1000) barwe     (1000)     3760 2022-09-21 03:38:51.000000 exuse-0.1.5/exuse/expath.py
--rw-r--r--   0 barwe     (1000) barwe     (1000)      319 2022-08-01 03:18:17.000000 exuse-0.1.5/exuse/extime.py
--rw-r--r--   0 barwe     (1000) barwe     (1000)      617 2022-09-19 07:38:42.000000 exuse-0.1.5/exuse/extypings.py
-drwxr-xr-x   0 barwe     (1000) barwe     (1000)        0 2022-09-27 02:17:19.545401 exuse-0.1.5/exuse.egg-info/
--rw-r--r--   0 barwe     (1000) barwe     (1000)      210 2022-09-27 02:17:19.000000 exuse-0.1.5/exuse.egg-info/PKG-INFO
--rw-r--r--   0 barwe     (1000) barwe     (1000)      256 2022-09-27 02:17:19.000000 exuse-0.1.5/exuse.egg-info/SOURCES.txt
--rw-r--r--   0 barwe     (1000) barwe     (1000)        1 2022-09-27 02:17:19.000000 exuse-0.1.5/exuse.egg-info/dependency_links.txt
--rw-r--r--   0 barwe     (1000) barwe     (1000)        6 2022-09-27 02:17:19.000000 exuse-0.1.5/exuse.egg-info/top_level.txt
--rw-r--r--   0 barwe     (1000) barwe     (1000)       38 2022-09-27 02:17:19.545401 exuse-0.1.5/setup.cfg
--rw-r--r--   0 barwe     (1000) barwe     (1000)      327 2022-09-27 02:16:58.000000 exuse-0.1.5/setup.py
+drwxr-xr-x   0 barwe     (1000) barwe     (1000)        0 2023-07-25 02:31:19.137711 exuse-0.1.6/
+-rw-r--r--   0 barwe     (1000) barwe     (1000)      210 2023-07-25 02:31:19.137711 exuse-0.1.6/PKG-INFO
+-rw-r--r--   0 barwe     (1000) barwe     (1000)     1268 2023-07-25 02:30:43.000000 exuse-0.1.6/README.md
+drwxr-xr-x   0 barwe     (1000) barwe     (1000)        0 2023-07-25 02:31:19.137711 exuse-0.1.6/exuse/
+-rw-r--r--   0 barwe     (1000) barwe     (1000)      296 2023-07-25 02:27:34.000000 exuse-0.1.6/exuse/__init__.py
+-rw-r--r--   0 barwe     (1000) barwe     (1000)     4301 2023-07-25 02:27:39.000000 exuse-0.1.6/exuse/exargparse.py
+-rw-r--r--   0 barwe     (1000) barwe     (1000)      922 2023-07-25 02:27:48.000000 exuse-0.1.6/exuse/exio.py
+-rw-r--r--   0 barwe     (1000) barwe     (1000)      558 2023-07-25 02:27:47.000000 exuse-0.1.6/exuse/exlogging.py
+-rw-r--r--   0 barwe     (1000) barwe     (1000)     3817 2023-07-25 02:27:46.000000 exuse-0.1.6/exuse/expath.py
+-rw-r--r--   0 barwe     (1000) barwe     (1000)      323 2023-07-25 02:27:44.000000 exuse-0.1.6/exuse/extime.py
+-rw-r--r--   0 barwe     (1000) barwe     (1000)      617 2023-07-25 02:27:42.000000 exuse-0.1.6/exuse/extypings.py
+-rw-r--r--   0 barwe     (1000) barwe     (1000)      504 2023-07-25 02:27:41.000000 exuse-0.1.6/exuse/subprocess.py
+drwxr-xr-x   0 barwe     (1000) barwe     (1000)        0 2023-07-25 02:31:19.137711 exuse-0.1.6/exuse.egg-info/
+-rw-r--r--   0 barwe     (1000) barwe     (1000)      210 2023-07-25 02:31:19.000000 exuse-0.1.6/exuse.egg-info/PKG-INFO
+-rw-r--r--   0 barwe     (1000) barwe     (1000)      276 2023-07-25 02:31:19.000000 exuse-0.1.6/exuse.egg-info/SOURCES.txt
+-rw-r--r--   0 barwe     (1000) barwe     (1000)        1 2023-07-25 02:31:19.000000 exuse-0.1.6/exuse.egg-info/dependency_links.txt
+-rw-r--r--   0 barwe     (1000) barwe     (1000)        6 2023-07-25 02:31:19.000000 exuse-0.1.6/exuse.egg-info/top_level.txt
+-rw-r--r--   0 barwe     (1000) barwe     (1000)       38 2023-07-25 02:31:19.137711 exuse-0.1.6/setup.cfg
+-rw-r--r--   0 barwe     (1000) barwe     (1000)      328 2023-07-25 02:27:24.000000 exuse-0.1.6/setup.py
```

### Comparing `exuse-0.1.5/README.md` & `exuse-0.1.6/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+# 打包和发布
+
+```bash
+N=5 && python setup.py sdist && pip install dist/exuse-0.1.$N.tar.gz && twine upload dist/exuse-0.1.$N.tar.gz
+# python setup.py sdist && pip install dist/exuse-0.1.3.tar.gz --force-reinstall
+```
+
+
+
 # exargparse
 
 ## BaseHandler
 
 当一个（子）解析器需要使用 `action` 选项执行不同的事务时，我们可以在 `BaseHandler` 的子类（**处理器**）中实现这些动作。使用 `@staticmethod` 装饰器将每个动作定义为类的静态方法（方法名与动作名相同），该方法只接受一个参数 `args`，代表解析器返回的参数对象（`Namespace` 实例）。参数解析完成后调用处理器的 `run()` 方法并传入解析的参数对象执行程序。
 
 ## SmartFormatter
@@ -12,11 +21,7 @@
 
 继承自 `argparse` 提供的 `ArgumentParser` 类，做了一些简单的封装，主要内容有：
 1. 使用 `SmartFormatter` 作为默认的消息格式化工具
 2. 提供 `get_subparser` 方法快速创建子解析器对象
 3. 提供 `set_callback` 方法设置（子）解析器的回调函数或者回调处理器
 4. 提供 `run` 方法调用预设的回调工具执行程序
 
-python setup.py sdist && pip install dist/exuse-0.1.3.tar.gz --force-reinstall
-
-N=5 && python setup.py sdist && pip install dist/exuse-0.1.$N.tar.gz
-N=5 && python setup.py sdist && pip install dist/exuse-0.1.$N.tar.gz && twine upload dist/exuse-0.1.$N.tar.gz
```

### Comparing `exuse-0.1.5/exuse/exargparse.py` & `exuse-0.1.6/exuse/exargparse.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,66 +1,65 @@
 from ast import arg
 import logging
 from typing import Callable, List
 from argparse import ArgumentParser, HelpFormatter
+
 # for export
 from argparse import Namespace
 
 
 class BaseHandler(object):
     """
-    If program has an `action` argument to handle different transactions, you 
-    can realize these actions in the subclass of `BaseHandler`. Each action 
-    can be defined as a static method using `@staticmethod` decorator. The 
-    static method has only one parameter named `args` which is generated by 
+    If program has an `action` argument to handle different transactions, you
+    can realize these actions in the subclass of `BaseHandler`. Each action
+    can be defined as a static method using `@staticmethod` decorator. The
+    static method has only one parameter named `args` which is generated by
     argument parsers, so that `action` method can access the arguments provided
     by command line. Call `set_default` or other methods of the arugment parser
     to bind the custom handler.
     """
 
     @classmethod
     def _run(cls, args):
         try:
             return getattr(cls, args.action)(args)
         except AttributeError as e:
             if str(e) == "'Namespace' object has no attribute 'action'":
-                print(
-                    "ERROR: `action` positional argument must be provided when using `BaseHandler` class")
+                print("ERROR: `action` positional argument must be provided when using `BaseHandler` class")
             else:
                 raise e
 
 
 class SmartFormatter(HelpFormatter):
     """
     Set help message by a multi-line string quoting by `\"\"\"` or `'''`).
     """
 
     def _split_lines(self, text: str, width: int) -> List[str]:
         # return [*[s.strip(' \n') for s in text.strip(' \n').split('\n')], '']
-        return [s.strip(' \n') for s in text.strip(' \n').split('\n')]
+        return [s.strip(" \n") for s in text.strip(" \n").split("\n")]
 
 
 class ExArgumentParser(ArgumentParser):
     """
     Extend the default `ArgumentParser`. Main contents appended:
     - set our custom `SmartFormatter` as the default formatter class
     - provide `get_subparser` method to get a subparser quickly
     - provide `set_callback` method to set callback function or Callback class
       for current parser or subparser. If you use `action` argument to process
-      different transactions, pass a `Callback` class inheritted from 
+      different transactions, pass a `Callback` class inheritted from
       `BaseHandler` is not a bad idea.
     - provide `run` method to run program by calling the given callback.
     """
 
     def __init__(self, formatter_class=SmartFormatter, **kwargs):
         super().__init__(formatter_class=formatter_class, **kwargs)
         self.__subparsers = None
-        levels = 'DEBUG|INFO|WARNING|ERROR|CRITICAL'
-        self.add_argument('--log-level', '-l', choices=levels.split('|'),
-                          default='INFO', metavar=levels, help="set logging level")
+        levels = "DEBUG|INFO|WARNING|ERROR|CRITICAL"
+        self.add_argument("--log-level", "-l", choices=levels.split("|"), default="INFO", metavar=levels, help="set logging level")
 
     @property
     def subparsers(self):
         if self.__subparsers is None:
             self.__subparsers = self.add_subparsers()
         return self.__subparsers
 
@@ -74,15 +73,15 @@
 
         """
         if callback is not None:
             self.set_defaults(callback=callback, Callback=None)
         elif Callback is not None:
             self.set_defaults(callback=None, Callback=Callback)
         else:
-            raise Exception('`Callback` and `callback` cannot be both `None`.')
+            raise Exception("`Callback` and `callback` cannot be both `None`.")
 
     def set_callback_function(self, func: Callable):
         """
         set callback function for current parser or subparser.
 
         Args:
             callback (Callable): a function to run main program
@@ -103,18 +102,18 @@
         """
         Run callback function.
         """
         args = self.parse_args()
         log_level: str = args.log_level
         logging.getLogger().setLevel(log_level)
 
-        if hasattr(args, 'callback') and args.callback is not None:
+        if hasattr(args, "callback") and args.callback is not None:
             callback: Callable = args.callback
             callback(args)
-        elif hasattr(args, 'Callback') and args.Callback is not None:
+        elif hasattr(args, "Callback") and args.Callback is not None:
             Callback: BaseHandler = args.Callback
             Callback._run(args)
         else:
             self.print_help()
 
     def get_subparser(self, *args, **kwargs):
         return self.subparsers.add_parser(*args, **kwargs)
```

### Comparing `exuse-0.1.5/exuse/exio.py` & `exuse-0.1.6/exuse/exio.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,43 @@
 import json
 
 
 def load_json(fp: str):
-    '''read json from a file'''
+    """read json from a file"""
     with open(fp) as rd:
         return json.load(rd)
 
 
 def dump_json(obj, fp: str, indent=4):
-    '''save json to a file'''
-    with open(fp, 'w') as wt:
+    """save json to a file"""
+    with open(fp, "w") as wt:
         json.dump(obj, wt, indent=indent)
 
 
 def read_jsonlike_file(fp: str):
     "根据文件扩展名自动读取文件内容"
-    if fp.endswith('toml'):
+    if fp.endswith("toml"):
         import toml
+
         return toml.load(fp)
-    elif fp.endswith('yaml'):
+    elif fp.endswith("yaml"):
         import yaml
+
         with open(fp) as r:
             return yaml.load(r)
-    elif fp.endswith('json'):
+    elif fp.endswith("json"):
         import json
+
         with open(fp) as r:
             return json.load(r)
     else:
         raise ValueError(f"Unsupported file extension: {fp.split('.')[-1]}")
 
+
 def read_file(fp: str) -> str:
     with open(fp) as r:
         return r.read().strip()
 
+
 def write(text: str, fp: str) -> None:
-    with open(fp, 'w') as w:
-        w.write(text)
+    with open(fp, "w") as w:
+        w.write(text)
```

### Comparing `exuse-0.1.5/exuse/expath.py` & `exuse-0.1.6/exuse/expath.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,37 +35,40 @@
     target = dirname(path) if is_file else path
 
     if not exists(target):
         makedirs(target)
     elif report_exist_error:
         raise DirectoryExistsError(target)
     elif copy_if_exists:
-        new_target = join(dirname(target), f'{basename(target)}_{timestamp()}')
-        logging.debug(f'mv {target} to {new_target}')
+        new_target = join(dirname(target), f"{basename(target)}_{timestamp()}")
+        logging.debug(f"mv {target} to {new_target}")
         move(target, new_target)
         makedirs(new_target)
 
     return path
 
 
+create_dir_if_not_exists = create_dir
+
+
 def must_exist(*path_parts: str):
     "拼接路径，并保证路径一定存在"
     path = join(*path_parts)
     if not exists(path):
         raise PathNotFoundError(path)
     return path
 
 
 def split_basename(filepath: str):
     "从文件路径的 basename 中拆分出 (filename, extname)"
     _base = basename(filepath)
-    if '.' not in filepath:
+    if "." not in filepath:
         return (_base, None)
     else:
-        arr = _base[::-1].split('.', 1)
+        arr = _base[::-1].split(".", 1)
         return (arr[1][::-1], arr[0][::-1])
 
 
 def filename(fp: str):
     """文件名：从文件 basename 中移除了文件扩展名"""
     return split_basename(fp)[0]
 
@@ -82,39 +85,42 @@
         for r in glob(pattern):
             results.append(r)
     return results
 
 
 def list_files(dp: str, extensions=None):
     files = []
-    if extensions is None: extensions = []
+    if extensions is None:
+        extensions = []
     exts = [f".{i.strip('.')}" for i in extensions]
-    if len(exts) == 0: exts = ['']
+    if len(exts) == 0:
+        exts = [""]
     for ext in exts:
-        for x in glob(f'{dp}/*{ext}'):
+        for x in glob(f"{dp}/*{ext}"):
             files.append(x)
-        for x in glob(f'{dp}/**/*{ext}'):
+        for x in glob(f"{dp}/**/*{ext}"):
             files.append(x)
     return files
 
+
 def get_path_by_filename(name: str, dirs: List[str], exts=None, report_dup_error=False):
     "通过 filename 查找指定目录列表下是否存在对应文件"
     if exts is None:
-        exts = ['json', 'toml', 'yaml']
+        exts = ["json", "toml", "yaml"]
     for dir in dirs:
-        r = glob_list([f'{dir}/{name}.*', f'{dir}/**/{name}.*'])
+        r = glob_list([f"{dir}/{name}.*", f"{dir}/**/{name}.*"])
         if len(r) == 1:
             return r[0]
         elif len(r) > 1:
             if report_dup_error:
-                raise Exception(f'more than one file found for {name}')
+                raise Exception(f"more than one file found for {name}")
             else:
                 target = r[0]
-                Q = {x.split('.')[-1]: i for i, x in enumerate(r)}
+                Q = {x.split(".")[-1]: i for i, x in enumerate(r)}
                 for k in exts:
                     if Q.get(k) is not None:
                         target = r[Q[k]]
                         break
-                logging.warning(f'more than one file found for {name}')
+                logging.warning(f"more than one file found for {name}")
                 return target
 
-    raise FileNotFoundError(f'no related file for {name}')
+    raise FileNotFoundError(f"no related file for {name}")
```

### Comparing `exuse-0.1.5/exuse/extypings.py` & `exuse-0.1.6/exuse/extypings.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Mapping, TypeVar
 from typing import List, Generator, Callable, Mapping, Generic, Dict, Sequence, Union, Tuple
 from typing_extensions import Self
 
-T = TypeVar('T')
-K = TypeVar('K')
-V = TypeVar('V')
+T = TypeVar("T")
+K = TypeVar("K")
+V = TypeVar("V")
 
 Record = Mapping[K, V]
 SRecord = Mapping[str, V]
 SSRecord = Mapping[str, str]
 SNRecord = Mapping[str, int]
 SBRecord = Mapping[str, bool]
 Array = List
```

