# Comparing `tmp/zheinit-0.0.8.tar.gz` & `tmp/zheinit-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zheinit-0.0.8.tar", last modified: Tue Jul 25 11:16:34 2023, max compression
+gzip compressed data, was "zheinit-0.0.9.tar", last modified: Tue Jul 25 11:32:25 2023, max compression
```

## Comparing `zheinit-0.0.8.tar` & `zheinit-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-25 11:16:34.939952 zheinit-0.0.8/
--rw-r--r--   0 dengyifan   (501) staff       (20)       21 2023-07-23 14:48:03.000000 zheinit-0.0.8/MANIFEST.in
--rw-r--r--   0 dengyifan   (501) staff       (20)      375 2023-07-25 11:16:34.939782 zheinit-0.0.8/PKG-INFO
--rw-r--r--   0 dengyifan   (501) staff       (20)      138 2023-07-23 13:52:05.000000 zheinit-0.0.8/README.md
--rw-r--r--   0 dengyifan   (501) staff       (20)       38 2023-07-25 11:16:34.940010 zheinit-0.0.8/setup.cfg
--rw-r--r--   0 dengyifan   (501) staff       (20)      799 2023-07-25 04:07:00.000000 zheinit-0.0.8/setup.py
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-25 11:16:34.938766 zheinit-0.0.8/zheinit/
--rw-r--r--   0 dengyifan   (501) staff       (20)        0 2023-07-23 14:24:47.000000 zheinit-0.0.8/zheinit/__init__.py
--rw-r--r--   0 dengyifan   (501) staff       (20)     3773 2023-07-23 13:48:55.000000 zheinit-0.0.8/zheinit/bash_config.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)     7081 2023-07-25 10:05:01.000000 zheinit-0.0.8/zheinit/init.py
--rw-r--r--   0 dengyifan   (501) staff       (20)     6852 2023-07-25 11:15:58.000000 zheinit-0.0.8/zheinit/run.py
--rw-r--r--   0 dengyifan   (501) staff       (20)     4412 2023-07-23 15:00:41.000000 zheinit-0.0.8/zheinit/utils.py
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-25 11:16:34.939568 zheinit-0.0.8/zheinit.egg-info/
--rw-r--r--   0 dengyifan   (501) staff       (20)      375 2023-07-25 11:16:34.000000 zheinit-0.0.8/zheinit.egg-info/PKG-INFO
--rw-r--r--   0 dengyifan   (501) staff       (20)      310 2023-07-25 11:16:34.000000 zheinit-0.0.8/zheinit.egg-info/SOURCES.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)        1 2023-07-25 11:16:34.000000 zheinit-0.0.8/zheinit.egg-info/dependency_links.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)       42 2023-07-25 11:16:34.000000 zheinit-0.0.8/zheinit.egg-info/entry_points.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)       23 2023-07-25 11:16:34.000000 zheinit-0.0.8/zheinit.egg-info/requires.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)        8 2023-07-25 11:16:34.000000 zheinit-0.0.8/zheinit.egg-info/top_level.txt
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-25 11:32:25.317185 zheinit-0.0.9/
+-rw-r--r--   0 dengyifan   (501) staff       (20)       21 2023-07-23 14:48:03.000000 zheinit-0.0.9/MANIFEST.in
+-rw-r--r--   0 dengyifan   (501) staff       (20)      375 2023-07-25 11:32:25.317016 zheinit-0.0.9/PKG-INFO
+-rw-r--r--   0 dengyifan   (501) staff       (20)      138 2023-07-23 13:52:05.000000 zheinit-0.0.9/README.md
+-rw-r--r--   0 dengyifan   (501) staff       (20)       38 2023-07-25 11:32:25.317242 zheinit-0.0.9/setup.cfg
+-rw-r--r--   0 dengyifan   (501) staff       (20)      799 2023-07-25 11:32:17.000000 zheinit-0.0.9/setup.py
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-25 11:32:25.315907 zheinit-0.0.9/zheinit/
+-rw-r--r--   0 dengyifan   (501) staff       (20)        0 2023-07-23 14:24:47.000000 zheinit-0.0.9/zheinit/__init__.py
+-rw-r--r--   0 dengyifan   (501) staff       (20)     3773 2023-07-23 13:48:55.000000 zheinit-0.0.9/zheinit/bash_config.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)     7305 2023-07-25 11:20:43.000000 zheinit-0.0.9/zheinit/init.py
+-rw-r--r--   0 dengyifan   (501) staff       (20)     7089 2023-07-25 11:32:08.000000 zheinit-0.0.9/zheinit/run.py
+-rw-r--r--   0 dengyifan   (501) staff       (20)     4412 2023-07-23 15:00:41.000000 zheinit-0.0.9/zheinit/utils.py
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-25 11:32:25.316782 zheinit-0.0.9/zheinit.egg-info/
+-rw-r--r--   0 dengyifan   (501) staff       (20)      375 2023-07-25 11:32:25.000000 zheinit-0.0.9/zheinit.egg-info/PKG-INFO
+-rw-r--r--   0 dengyifan   (501) staff       (20)      310 2023-07-25 11:32:25.000000 zheinit-0.0.9/zheinit.egg-info/SOURCES.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)        1 2023-07-25 11:32:25.000000 zheinit-0.0.9/zheinit.egg-info/dependency_links.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)       42 2023-07-25 11:32:25.000000 zheinit-0.0.9/zheinit.egg-info/entry_points.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)       23 2023-07-25 11:32:25.000000 zheinit-0.0.9/zheinit.egg-info/requires.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)        8 2023-07-25 11:32:25.000000 zheinit-0.0.9/zheinit.egg-info/top_level.txt
```

### Comparing `zheinit-0.0.8/setup.py` & `zheinit-0.0.9/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # coding: utf-8
 
 from setuptools import setup, find_packages
 
 setup(
     name='zheinit',
-    version='0.0.8',
+    version='0.0.9',
     author='deng1fan',
     author_email='dengyifan@iie.ac.cn',
     url='https://github.com/deng1fan',
     description=u'Init zhei environment.',
     long_description=open("README.md", "r", encoding='utf-8').read(),
     long_description_content_type="text/markdown",
     packages=find_packages(),
```

### Comparing `zheinit-0.0.8/zheinit/bash_config.txt` & `zheinit-0.0.9/zheinit/bash_config.txt`

 * *Files identical despite different names*

### Comparing `zheinit-0.0.8/zheinit/init.py` & `zheinit-0.0.9/zheinit/init.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import os
 from zheinit.utils import show_available_version, run_cmd, echo, get_cmd_output
 
 
 def init():
     if "bash" not in get_cmd_output("echo $SHELL"):
         if "bash" not in get_cmd_output("cat /etc/shells"):
-            print("未找到 bash 环境，请先安装 bash 环境！")
+            echo("未找到 bash 环境，请先安装 bash 环境！", "red")
         else:        
-            print("请在 bash 环境下运行本工具！")
-        print("您可以通过以下命令查看所支持的 Shell 类型：\ncat /etc/shells")
-        print("您可以通过以下命令切换 Shell 类型：\nchsh -s /bin/bash")
+            echo("请在 bash 环境下运行本工具！")
+        echo("您可以通过以下命令查看所支持的 Shell 类型：\ncat /etc/shells", "red")
+        echo("您可以通过以下命令切换 Shell 类型：\nchsh -s /bin/bash", "red")
         exit()
 
     pkg_current_path = os.path.dirname(os.path.abspath(__file__))
     python_version = "3.9"
     env_name = "zhei"
 
     # 读取 ~/.bashrc 文件内容
@@ -49,28 +49,28 @@
     echo("")
     echo("             欢迎使用服务器环境初始化工具 zhei-init ！", "green")
     echo("   本工具将会帮助您初始化服务器环境，下面是功能菜单，可输入序号进行配置", "green")
 
     step = "-1"
     while step != "0":
         if step != "-1":
-            echo("是否继续配置？（y/n）", "yellow")
+            echo("\n是否继续配置？（y/n）", "yellow")
             conti = input()
             if conti != "y":
                 break
         echo(" ", "blue")
         echo("1、设置 pip 源", "blue") 
         echo("2、安装 MiniConda", "blue")
         echo("3、安装 ranger 并自动配置", "blue")
         echo("4、创建 Conda  Pytorch 环境", "blue")
         echo("5、生成公钥", "blue")
         echo("6、生成 zhei 项目模板", "blue")
         echo("0、退出", "blue")
         echo(" ", "blue")
-        echo("请输入操作序号：", "yellow")
+        echo("请在下方输入操作序号：", "yellow")
         step = input()
         if step == "1":
             # ---------------------------------------------------------------------------- #
             #                         设置 pip 源                                     
             # ---------------------------------------------------------------------------- #
             pip_source = [
                 "conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/pkgs/free/",
@@ -100,39 +100,42 @@
             ]
             run_cmd(ranger)
 
         elif step == "4":
             # ---------------------------------------------------------------------------- #
             #                         创建 zhei 环境                                     
             # ---------------------------------------------------------------------------- #
-            python_version = input("请输入 Python 版本号，默认为 3.9：")
-            env_name = input("请输入环境名称，将会自动安装 zhei 包，默认名称为 zhei：")
+            echo("即将创建 zhei 环境，请在下方输入 Python 版本号，默认为 3.9：", "yellow")
+            python_version = input()
+            echo("即将创建 zhei 环境，请在下方输入环境名称，将会自动安装 zhei 包，默认名称为 zhei：", "yellow")
+            env_name = input()
             zhei = [
                 "conda create -n {} python={}".format(env_name, python_version),
                 "conda activate {}".format(env_name),
                 "pip install zhei --upgrade",
             ]
             run_cmd(zhei)
 
-            cuda_version = input("请输入 CUDA 版本号：")
+            echo("即将安装 Pytorch，请选择 CUDA 版本号，默认为 11.8：", "yellow")
+            cuda_version = input()
             torch_url, torchvision_url, torchaudio_url = show_available_version(cuda_version, python_version)
 
-            print("即将从以下链接安装 torch：\n {}".format(torch_url))
+            echo("即将从以下链接安装 torch：\n {}".format(torch_url))
             torch_install = [
                 "pip install {}".format(torch_url),
             ]   
             run_cmd(torch_install)
 
-            print("即将从以下链接安装 torchvision：\n {}".format(torchvision_url))  
+            echo("即将从以下链接安装 torchvision：\n {}".format(torchvision_url))  
             torchvision_install = [
                 "pip install {}".format(torchvision_url),
             ]
             run_cmd(torchvision_install)
 
-            print("即将从以下链接安装 torchaudio：\n {}".format(torchaudio_url))
+            echo("即将从以下链接安装 torchaudio：\n {}".format(torchaudio_url))
             torchaudio_install = [
                 "pip install {}".format(torchaudio_url),
             ]   
             run_cmd(torchaudio_install)
             
         elif step == "5":
             run_cmd([
```

### Comparing `zheinit-0.0.8/zheinit/run.py` & `zheinit-0.0.9/zheinit/run.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import os
-from utils import run_cmd, echo, get_cmd_output
+from zheinit.utils import run_cmd, echo, get_cmd_output
 import yaml
 import datetime
 import time
 
 
 def read_yaml(path):
     with open(path, 'r') as f:
         data = yaml.load(f, Loader=yaml.SafeLoader)
     return data
 
 
 def run():
     
-    project_path = "/Users/dengyifan/Desktop/Github仓库/zheinit/zheinit/ProjectTemplate"
-    # project_path = os.getcwd()
+    # project_path = "/Users/dengyifan/Desktop/Github仓库/zheinit/zheinit/ProjectTemplate"
+    project_path = os.getcwd()
     echo("")
     echo("")
     echo("")
     echo("      _____                          _      ____                  _")
     echo("     |  __ \\                        | |    |  _ \\                | |")
     echo("     | |__) |____      _____ _ __ __| |    | |_) |_   _          | |")
     echo("     |  ___/ _ \\ \\ /\\ / / _ \\ '__/ _` |    |  _ <| | | |     _   | |")
@@ -44,16 +44,22 @@
     echo("\n请在下方输入您的项目名或直接选择序号：")
     project_name = input()
     if project_name.isdigit():
         project_name = projects[int(project_name) - 1]
     
     echo("\n选择启动 {} 项目计划的模式，目前支持 “nohup”、“tmux”、“python”，默认为 “nohup”：".format(project_name))
     start_mode = input()
+    conda_env = ""
     if start_mode not in ["nohup", "tmux", "python"] or start_mode == "":
         start_mode = "nohup"
+    if start_mode == "tmux":
+        echo("\n请在下方输入您的 conda 环境名，默认 zhei：")
+        conda_env = input("")
+        if conda_env == "":
+            conda_env = "zhei"
     
     # ---------------------------------------------------------------------------- #
     #                         获取实验计划                                     
     # ---------------------------------------------------------------------------- #
     exp_plan_path = os.path.join(project_path, "configs/exps/{}/exp_plan.yaml".format(project_name))
     exp_plan = read_yaml(exp_plan_path)
     
@@ -118,15 +124,15 @@
             cmd += hyper_params_str
             cmd += " +tmux_session=\"{}\"".format(tmux_session)
             cmd += " +experiments={}".format(exp_cfg_path)
             
             run_cmd("tmux new-session -d -s {}".format(tmux_session))
             run_cmd("tmux send-keys -t {} {}".format(tmux_session, "cd {}".format(project_path)))
             run_cmd("tmux send-keys -t {} {}".format(tmux_session, "C-m"))
-            run_cmd("tmux send-keys -t {} {}".format(tmux_session, "conda activate zhei"))
+            run_cmd("tmux send-keys -t {} {}".format(tmux_session, "conda activate {}".format(conda_env)))
             run_cmd("tmux send-keys -t {} {}".format(tmux_session, "C-m"))
             run_cmd("tmux send-keys -t {} {}".format(tmux_session, cmd))
             run_cmd("tmux send-keys -t {} {}".format(tmux_session, "C-m"))
         
             echo(cmd, "yellow")
             echo("查看日志：tmux attach -t {}".format(tmux_session))
             echo("关闭日志：tmux kill-session -t {}".format(tmux_session))
```

### Comparing `zheinit-0.0.8/zheinit/utils.py` & `zheinit-0.0.9/zheinit/utils.py`

 * *Files identical despite different names*

