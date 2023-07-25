# Comparing `tmp/zheinit-0.0.73.tar.gz` & `tmp/zheinit-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zheinit-0.0.73.tar", last modified: Sun Jul 23 15:03:36 2023, max compression
+gzip compressed data, was "zheinit-0.0.8.tar", last modified: Tue Jul 25 11:16:34 2023, max compression
```

## Comparing `zheinit-0.0.73.tar` & `zheinit-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-23 15:03:36.544463 zheinit-0.0.73/
--rw-r--r--   0 dengyifan   (501) staff       (20)       21 2023-07-23 14:48:03.000000 zheinit-0.0.73/MANIFEST.in
--rw-r--r--   0 dengyifan   (501) staff       (20)      376 2023-07-23 15:03:36.544270 zheinit-0.0.73/PKG-INFO
--rw-r--r--   0 dengyifan   (501) staff       (20)      138 2023-07-23 13:52:05.000000 zheinit-0.0.73/README.md
--rw-r--r--   0 dengyifan   (501) staff       (20)       38 2023-07-23 15:03:36.544513 zheinit-0.0.73/setup.cfg
--rw-r--r--   0 dengyifan   (501) staff       (20)      784 2023-07-23 15:03:34.000000 zheinit-0.0.73/setup.py
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-23 15:03:36.542871 zheinit-0.0.73/zheinit/
--rw-r--r--   0 dengyifan   (501) staff       (20)        0 2023-07-23 14:24:47.000000 zheinit-0.0.73/zheinit/__init__.py
--rw-r--r--   0 dengyifan   (501) staff       (20)     3773 2023-07-23 13:48:55.000000 zheinit-0.0.73/zheinit/bash_config.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)     6000 2023-07-23 15:03:24.000000 zheinit-0.0.73/zheinit/env.py
--rw-r--r--   0 dengyifan   (501) staff       (20)     4412 2023-07-23 15:00:41.000000 zheinit-0.0.73/zheinit/utils.py
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-23 15:03:36.544030 zheinit-0.0.73/zheinit.egg-info/
--rw-r--r--   0 dengyifan   (501) staff       (20)      376 2023-07-23 15:03:36.000000 zheinit-0.0.73/zheinit.egg-info/PKG-INFO
--rw-r--r--   0 dengyifan   (501) staff       (20)      294 2023-07-23 15:03:36.000000 zheinit-0.0.73/zheinit.egg-info/SOURCES.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)        1 2023-07-23 15:03:36.000000 zheinit-0.0.73/zheinit.egg-info/dependency_links.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)       42 2023-07-23 15:03:36.000000 zheinit-0.0.73/zheinit.egg-info/entry_points.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)       18 2023-07-23 15:03:36.000000 zheinit-0.0.73/zheinit.egg-info/requires.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)        8 2023-07-23 15:03:36.000000 zheinit-0.0.73/zheinit.egg-info/top_level.txt
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-25 11:16:34.939952 zheinit-0.0.8/
+-rw-r--r--   0 dengyifan   (501) staff       (20)       21 2023-07-23 14:48:03.000000 zheinit-0.0.8/MANIFEST.in
+-rw-r--r--   0 dengyifan   (501) staff       (20)      375 2023-07-25 11:16:34.939782 zheinit-0.0.8/PKG-INFO
+-rw-r--r--   0 dengyifan   (501) staff       (20)      138 2023-07-23 13:52:05.000000 zheinit-0.0.8/README.md
+-rw-r--r--   0 dengyifan   (501) staff       (20)       38 2023-07-25 11:16:34.940010 zheinit-0.0.8/setup.cfg
+-rw-r--r--   0 dengyifan   (501) staff       (20)      799 2023-07-25 04:07:00.000000 zheinit-0.0.8/setup.py
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-25 11:16:34.938766 zheinit-0.0.8/zheinit/
+-rw-r--r--   0 dengyifan   (501) staff       (20)        0 2023-07-23 14:24:47.000000 zheinit-0.0.8/zheinit/__init__.py
+-rw-r--r--   0 dengyifan   (501) staff       (20)     3773 2023-07-23 13:48:55.000000 zheinit-0.0.8/zheinit/bash_config.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)     7081 2023-07-25 10:05:01.000000 zheinit-0.0.8/zheinit/init.py
+-rw-r--r--   0 dengyifan   (501) staff       (20)     6852 2023-07-25 11:15:58.000000 zheinit-0.0.8/zheinit/run.py
+-rw-r--r--   0 dengyifan   (501) staff       (20)     4412 2023-07-23 15:00:41.000000 zheinit-0.0.8/zheinit/utils.py
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-25 11:16:34.939568 zheinit-0.0.8/zheinit.egg-info/
+-rw-r--r--   0 dengyifan   (501) staff       (20)      375 2023-07-25 11:16:34.000000 zheinit-0.0.8/zheinit.egg-info/PKG-INFO
+-rw-r--r--   0 dengyifan   (501) staff       (20)      310 2023-07-25 11:16:34.000000 zheinit-0.0.8/zheinit.egg-info/SOURCES.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)        1 2023-07-25 11:16:34.000000 zheinit-0.0.8/zheinit.egg-info/dependency_links.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)       42 2023-07-25 11:16:34.000000 zheinit-0.0.8/zheinit.egg-info/entry_points.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)       23 2023-07-25 11:16:34.000000 zheinit-0.0.8/zheinit.egg-info/requires.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)        8 2023-07-25 11:16:34.000000 zheinit-0.0.8/zheinit.egg-info/top_level.txt
```

### Comparing `zheinit-0.0.73/setup.py` & `zheinit-0.0.8/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 #!/usr/bin/env python
 # coding: utf-8
 
 from setuptools import setup, find_packages
 
 setup(
     name='zheinit',
-    version='0.0.73',
+    version='0.0.8',
     author='deng1fan',
     author_email='dengyifan@iie.ac.cn',
     url='https://github.com/deng1fan',
     description=u'Init zhei environment.',
     long_description=open("README.md", "r", encoding='utf-8').read(),
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=[
         'bs4',
         'requests',
         'rich',
+        'yaml',
     ],
     exclude=["*.tests", "*.tests.*", "tests"],
     include_package_data=True,
     python_requires='>=3.6',
     entry_points = {
         'console_scripts' : [
             # 这一行是安装到命令行运行的关键
-            'init = zheinit.env:init'
+            'ini = zheinit.init:init'
         ]
     }
 )
```

### Comparing `zheinit-0.0.73/zheinit/bash_config.txt` & `zheinit-0.0.8/zheinit/bash_config.txt`

 * *Files identical despite different names*

### Comparing `zheinit-0.0.73/zheinit/env.py` & `zheinit-0.0.8/zheinit/init.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import os
 from zheinit.utils import show_available_version, run_cmd, echo, get_cmd_output
+
+
 def init():
     if "bash" not in get_cmd_output("echo $SHELL"):
         if "bash" not in get_cmd_output("cat /etc/shells"):
             print("未找到 bash 环境，请先安装 bash 环境！")
         else:        
             print("请在 bash 环境下运行本工具！")
         print("您可以通过以下命令查看所支持的 Shell 类型：\ncat /etc/shells")
@@ -27,16 +29,28 @@
             "cd ~/",
             "cat {}/bash_config.txt >> ~/.bashrc".format(pkg_current_path),
             "conda init bash",
             "source ~/.bashrc",
         ]
         run_cmd(bash)
         
-
-
+    echo("")
+    echo("")
+    echo("")
+    echo("      _____                          _      ____                  _")
+    echo("     |  __ \\                        | |    |  _ \\                | |")
+    echo("     | |__) |____      _____ _ __ __| |    | |_) |_   _          | |")
+    echo("     |  ___/ _ \\ \\ /\\ / / _ \\ '__/ _` |    |  _ <| | | |     _   | |")
+    echo("     | |  | (_) \\ V  V /  __/ | | (_| |    | |_) | |_| |    | |__| |")
+    echo("     |_|   \\___/ \\_/\\_/ \\___|_|  \\__,_|    |____/ \\__, |     \\____/")
+    echo("                                                   __/ |")
+    echo("                                                  |___/")
+    echo("")
+    echo("")
+    echo("")
     echo("             欢迎使用服务器环境初始化工具 zhei-init ！", "green")
     echo("   本工具将会帮助您初始化服务器环境，下面是功能菜单，可输入序号进行配置", "green")
 
     step = "-1"
     while step != "0":
         if step != "-1":
             echo("是否继续配置？（y/n）", "yellow")
@@ -45,14 +59,15 @@
                 break
         echo(" ", "blue")
         echo("1、设置 pip 源", "blue") 
         echo("2、安装 MiniConda", "blue")
         echo("3、安装 ranger 并自动配置", "blue")
         echo("4、创建 Conda  Pytorch 环境", "blue")
         echo("5、生成公钥", "blue")
+        echo("6、生成 zhei 项目模板", "blue")
         echo("0、退出", "blue")
         echo(" ", "blue")
         echo("请输入操作序号：", "yellow")
         step = input()
         if step == "1":
             # ---------------------------------------------------------------------------- #
             #                         设置 pip 源                                     
@@ -122,12 +137,20 @@
         elif step == "5":
             run_cmd([
                 "cd ~/.ssh",
                 "ssh-keygen -t rsa",
                 "cat id_rsa.pub"
             ])
             
+        elif step == "6":
+            target_path = input("请输入项目路径（包含新的项目文件夹名），默认为 ~/code/zhei_project：")
+            run_cmd([
+                "cp -r {}/ProjectTemplate {}".format(pkg_current_path, target_path),        
+            ])
+            
         elif step == "0":
             exit()
 
         else:
-            continue
+            continue
+        
+
```

### Comparing `zheinit-0.0.73/zheinit/utils.py` & `zheinit-0.0.8/zheinit/utils.py`

 * *Files identical despite different names*

