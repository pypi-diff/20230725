# Comparing `tmp/nb_cli_plugin_littlepaimon-1.0.0rc3.tar.gz` & `tmp/nb_cli_plugin_littlepaimon-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nb_cli_plugin_littlepaimon-1.0.0rc3.tar", max compression
+gzip compressed data, was "nb_cli_plugin_littlepaimon-1.0.1.tar", max compression
```

## Comparing `nb_cli_plugin_littlepaimon-1.0.0rc3.tar` & `nb_cli_plugin_littlepaimon-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    34523 2023-01-30 12:27:36.653344 nb_cli_plugin_littlepaimon-1.0.0rc3/LICENSE
--rw-r--r--   0        0        0     2553 2023-01-30 12:27:36.653344 nb_cli_plugin_littlepaimon-1.0.0rc3/README.md
--rw-r--r--   0        0        0      235 2023-01-30 12:27:36.653344 nb_cli_plugin_littlepaimon-1.0.0rc3/nb_cli_plugin_littlepaimon/__init__.py
--rw-r--r--   0        0        0     2067 2023-01-30 12:27:36.653344 nb_cli_plugin_littlepaimon-1.0.0rc3/nb_cli_plugin_littlepaimon/cli.py
--rw-r--r--   0        0        0      137 2023-01-30 12:27:36.653344 nb_cli_plugin_littlepaimon-1.0.0rc3/nb_cli_plugin_littlepaimon/commands/__init__.py
--rw-r--r--   0        0        0    12534 2023-01-30 12:27:36.653344 nb_cli_plugin_littlepaimon-1.0.0rc3/nb_cli_plugin_littlepaimon/commands/create.py
--rw-r--r--   0        0        0     1898 2023-01-30 12:27:36.653344 nb_cli_plugin_littlepaimon-1.0.0rc3/nb_cli_plugin_littlepaimon/commands/install.py
--rw-r--r--   0        0        0     7224 2023-01-30 12:27:36.653344 nb_cli_plugin_littlepaimon-1.0.0rc3/nb_cli_plugin_littlepaimon/commands/resources.py
--rw-r--r--   0        0        0     1333 2023-01-30 12:27:36.653344 nb_cli_plugin_littlepaimon-1.0.0rc3/nb_cli_plugin_littlepaimon/commands/run.py
--rw-r--r--   0        0        0     1311 2023-01-30 12:27:36.653344 nb_cli_plugin_littlepaimon-1.0.0rc3/nb_cli_plugin_littlepaimon/commands/update.py
--rw-r--r--   0        0        0     3239 2023-01-30 12:27:36.653344 nb_cli_plugin_littlepaimon-1.0.0rc3/nb_cli_plugin_littlepaimon/config_template.yml
--rw-r--r--   0        0        0      105 2023-01-30 12:27:36.653344 nb_cli_plugin_littlepaimon-1.0.0rc3/nb_cli_plugin_littlepaimon/handlers/__init__.py
--rw-r--r--   0        0        0     2468 2023-01-30 12:27:36.653344 nb_cli_plugin_littlepaimon-1.0.0rc3/nb_cli_plugin_littlepaimon/handlers/cmd.py
--rw-r--r--   0        0        0     1828 2023-01-30 12:27:36.653344 nb_cli_plugin_littlepaimon-1.0.0rc3/nb_cli_plugin_littlepaimon/handlers/download.py
--rw-r--r--   0        0        0     1512 2023-01-30 12:27:36.653344 nb_cli_plugin_littlepaimon-1.0.0rc3/nb_cli_plugin_littlepaimon/handlers/gocq.py
--rw-r--r--   0        0        0     1443 2023-01-30 12:27:36.653344 nb_cli_plugin_littlepaimon-1.0.0rc3/nb_cli_plugin_littlepaimon/meta.py
--rw-r--r--   0        0        0      209 2023-01-30 12:27:36.653344 nb_cli_plugin_littlepaimon-1.0.0rc3/nb_cli_plugin_littlepaimon/plugin.py
--rw-r--r--   0        0        0      722 2023-01-30 12:27:36.653344 nb_cli_plugin_littlepaimon-1.0.0rc3/pyproject.toml
--rw-r--r--   0        0        0     3328 1970-01-01 00:00:00.000000 nb_cli_plugin_littlepaimon-1.0.0rc3/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-07-25 05:09:45.892779 nb_cli_plugin_littlepaimon-1.0.1/LICENSE
+-rw-r--r--   0        0        0     3010 2023-07-25 05:09:45.892779 nb_cli_plugin_littlepaimon-1.0.1/README.md
+-rw-r--r--   0        0        0      235 2023-07-25 05:09:45.892779 nb_cli_plugin_littlepaimon-1.0.1/nb_cli_plugin_littlepaimon/__init__.py
+-rw-r--r--   0        0        0     2067 2023-07-25 05:09:45.892779 nb_cli_plugin_littlepaimon-1.0.1/nb_cli_plugin_littlepaimon/cli.py
+-rw-r--r--   0        0        0      137 2023-07-25 05:09:45.892779 nb_cli_plugin_littlepaimon-1.0.1/nb_cli_plugin_littlepaimon/commands/__init__.py
+-rw-r--r--   0        0        0    13187 2023-07-25 05:09:45.892779 nb_cli_plugin_littlepaimon-1.0.1/nb_cli_plugin_littlepaimon/commands/create.py
+-rw-r--r--   0        0        0     1696 2023-07-25 05:09:45.892779 nb_cli_plugin_littlepaimon-1.0.1/nb_cli_plugin_littlepaimon/commands/install.py
+-rw-r--r--   0        0        0     9212 2023-07-25 05:09:45.892779 nb_cli_plugin_littlepaimon-1.0.1/nb_cli_plugin_littlepaimon/commands/resources.py
+-rw-r--r--   0        0        0     1704 2023-07-25 05:09:45.892779 nb_cli_plugin_littlepaimon-1.0.1/nb_cli_plugin_littlepaimon/commands/run.py
+-rw-r--r--   0        0        0     1323 2023-07-25 05:09:45.892779 nb_cli_plugin_littlepaimon-1.0.1/nb_cli_plugin_littlepaimon/commands/update.py
+-rw-r--r--   0        0        0     3239 2023-07-25 05:09:45.892779 nb_cli_plugin_littlepaimon-1.0.1/nb_cli_plugin_littlepaimon/config_template.yml
+-rw-r--r--   0        0        0      105 2023-07-25 05:09:45.892779 nb_cli_plugin_littlepaimon-1.0.1/nb_cli_plugin_littlepaimon/handlers/__init__.py
+-rw-r--r--   0        0        0     2089 2023-07-25 05:09:45.892779 nb_cli_plugin_littlepaimon-1.0.1/nb_cli_plugin_littlepaimon/handlers/cmd.py
+-rw-r--r--   0        0        0     1828 2023-07-25 05:09:45.892779 nb_cli_plugin_littlepaimon-1.0.1/nb_cli_plugin_littlepaimon/handlers/download.py
+-rw-r--r--   0        0        0     1512 2023-07-25 05:09:45.892779 nb_cli_plugin_littlepaimon-1.0.1/nb_cli_plugin_littlepaimon/handlers/gocq.py
+-rw-r--r--   0        0        0     1443 2023-07-25 05:09:45.892779 nb_cli_plugin_littlepaimon-1.0.1/nb_cli_plugin_littlepaimon/meta.py
+-rw-r--r--   0        0        0      209 2023-07-25 05:09:45.892779 nb_cli_plugin_littlepaimon-1.0.1/nb_cli_plugin_littlepaimon/plugin.py
+-rw-r--r--   0        0        0     1102 2023-07-25 05:09:45.892779 nb_cli_plugin_littlepaimon-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3782 1970-01-01 00:00:00.000000 nb_cli_plugin_littlepaimon-1.0.1/PKG-INFO
```

### Comparing `nb_cli_plugin_littlepaimon-1.0.0rc3/LICENSE` & `nb_cli_plugin_littlepaimon-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nb_cli_plugin_littlepaimon-1.0.0rc3/README.md` & `nb_cli_plugin_littlepaimon-1.0.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -94,17 +94,21 @@
 
 ## 使用
 
 - `nb paimon` 交互式使用
   - `nb paimon create` 
     - 交互式指引安装[LittlePaimon](https://github.com/CMHopeSunshine/LittlePaimon)
     - 自动克隆源码、创建虚拟环境、安装依赖，下载并配置go-cqhttp
-  - `nb paimon run` 启动小派蒙
-    - 实际上和`nb run`一样，不过去掉了不常用的参数 
+    - 添加`-g`参数，则是只下载go-cqhttp
+  - `nb paimon run` 运行python命令或启动小派蒙
+    - 当接有命令时，使用该目录的下python解释器运行命令，例如`nb paimon run playwright install`
+    - 当没有命令时，使用该目录的下python解释器启动小派蒙，实际上等价于`nb run`，不过去掉了不常用的参数 
   - `nb paimon install` 安装依赖库到小派蒙环境中
+    - 当接有参数时，使用该目录的下pip安装依赖，例如`nb paimon install httpx`
+    - 当没有参数时，则是使用该目录的下pip安装`requirements.txt`中的依赖
   - `nb paimon res` 下载或更新小派蒙的资源
   - `nb paimon update` 更新小派蒙，和`git pull`一样
   - `nb paimon logo` 展示小派蒙的logo
 - `nb paimon (指令) --help` 查看帮助
 
 ## TODO
```

#### html2text {}

```diff
@@ -10,16 +10,23 @@
 éè¿ nb-cli å®è£ ```shell nb self install nb-cli-plugin-littlepaimon ```
 éè¿ pipx å®è£ ```shell pipx inject nb-cli nb-cli-plugin-littlepaimon ```
 éè¿ pip å®è£ ```shell pip install nb-cli-plugin-littlepaimon ```   --
 -  å®è£Git ~~è½ä¸Githubçè¯ï¼åºè¯¥é½ä¼è£Gitå§)~~  ## ä½¿ç¨ - `nb
 paimon` äº¤äºå¼ä½¿ç¨ - `nb paimon create` - äº¤äºå¼æå¼å®è£
 [LittlePaimon](https://github.com/CMHopeSunshine/LittlePaimon) -
 èªå¨åéæºç ãåå»ºèæç¯å¢ãå®è£ä¾èµï¼ä¸è½½å¹¶éç½®go-
-cqhttp - `nb paimon run` å¯å¨å°æ´¾è - å®éä¸å`nb
-run`ä¸æ ·ï¼ä¸è¿å»æäºä¸å¸¸ç¨çåæ° - `nb paimon install`
-å®è£ä¾èµåºå°å°æ´¾èç¯å¢ä¸­ - `nb paimon res`
-ä¸è½½ææ´æ°å°æ´¾èçèµæº - `nb paimon update`
+cqhttp - æ·»å `-g`åæ°ï¼åæ¯åªä¸è½½go-cqhttp - `nb paimon run`
+è¿è¡pythonå½ä»¤æå¯å¨å°æ´¾è -
+å½æ¥æå½ä»¤æ¶ï¼ä½¿ç¨è¯¥ç®å½çä¸pythonè§£éå¨è¿è¡å½ä»¤ï¼ä¾å¦`nb
+paimon run playwright install` -
+å½æ²¡æå½ä»¤æ¶ï¼ä½¿ç¨è¯¥ç®å½çä¸pythonè§£éå¨å¯å¨å°æ´¾èï¼å®éä¸ç­ä»·äº`nb
+run`ï¼ä¸è¿å»æäºä¸å¸¸ç¨çåæ° - `nb paimon install`
+å®è£ä¾èµåºå°å°æ´¾èç¯å¢ä¸­ -
+å½æ¥æåæ°æ¶ï¼ä½¿ç¨è¯¥ç®å½çä¸pipå®è£ä¾èµï¼ä¾å¦`nb paimon
+install httpx` -
+å½æ²¡æåæ°æ¶ï¼åæ¯ä½¿ç¨è¯¥ç®å½çä¸pipå®è£`requirements.txt`ä¸­çä¾èµ
+- `nb paimon res` ä¸è½½ææ´æ°å°æ´¾èçèµæº - `nb paimon update`
 æ´æ°å°æ´¾èï¼å`git pull`ä¸æ · - `nb paimon logo` å±ç¤ºå°æ´¾èçlogo
 - `nb paimon (æä»¤) --help` æ¥çå¸®å© ## TODO - [x] æ´æ°èµæº - [ ]
 ä¸ä¾èµgit - [ ] ä¿®æ¹éç½® - [ ] å®è£å°æ´¾èæä»¶ - [ ] more ##
 ç¸å³é¡¹ç® - [nb-cli](https://github.com/nonebot/nb-cli) - [LittlePaimon]
 (https://github.com/CMHopeSunshine/LittlePaimon)
```

### Comparing `nb_cli_plugin_littlepaimon-1.0.0rc3/nb_cli_plugin_littlepaimon/cli.py` & `nb_cli_plugin_littlepaimon-1.0.1/nb_cli_plugin_littlepaimon/cli.py`

 * *Files identical despite different names*

### Comparing `nb_cli_plugin_littlepaimon-1.0.0rc3/nb_cli_plugin_littlepaimon/commands/create.py` & `nb_cli_plugin_littlepaimon-1.0.1/nb_cli_plugin_littlepaimon/commands/create.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,66 +1,74 @@
-import asyncio
-import contextlib
 import os
-import shutil
 import stat
+import shutil
+import asyncio
+import contextlib
 from pathlib import Path
 from typing import Optional
 
 import click
-from nb_cli.cli import ClickAliasedCommand, run_async, CLI_DEFAULT_STYLE
-from nb_cli.cli.commands.project import project_name_validator
 from nb_cli.consts import WINDOWS
-from nb_cli.handlers import create_virtualenv, call_pip_install
-from noneprompt import Choice, ListPrompt, CancelledError, ConfirmPrompt, InputPrompt
+from nb_cli.cli.commands.project import project_name_validator
+from nb_cli.handlers import call_pip_install, create_virtualenv
+from nb_cli.cli import CLI_DEFAULT_STYLE, ClickAliasedCommand, run_async
+from noneprompt import (
+    Choice,
+    ListPrompt,
+    InputPrompt,
+    ConfirmPrompt,
+    CancelledError,
+)
 
+from ..handlers.gocq import EXECUTABLE_EXT, download_gocq
 from ..handlers.cmd import check_git, clone_paimon, install_dependencies
-from ..handlers.gocq import download_gocq, EXECUTABLE_EXT
-from ..meta import LOGO
 
 
 @click.command(
     cls=ClickAliasedCommand,
     aliases=['new', 'init'],
     context_settings={'ignore_unknown_options': True},
     help='在当前目录下安装小派蒙以及go-cqhttp.',
 )
 @click.option(
     '-p',
     '--python-interpreter',
     default=None,
     help='指定Python解释器的路径',
 )
-@click.option('-i',
-              '--index-url',
-              'index_url',
-              default=None,
-              help='pip下载所使用的镜像源')
-@click.option('-q',
-              '--only-gocq',
-              'only_gocq',
-              default=False,
-              is_flag=True,
-              help='是否只下载go-cqhttp本体')
+@click.option(
+    '-i', '--index-url', 'index_url', default=None, help='pip下载所使用的镜像源'
+)
+@click.option(
+    '-q',
+    '--only-gocq',
+    'only_gocq',
+    default=False,
+    is_flag=True,
+    help='是否只下载go-cqhttp本体',
+)
 @click.pass_context
 @run_async
-async def create(ctx: click.Context,
-                 python_interpreter: Optional[str],
-                 index_url: Optional[str],
-                 only_gocq: bool = False):
+async def create(
+    ctx: click.Context,
+    python_interpreter: Optional[str],
+    index_url: Optional[str],
+    only_gocq: bool = False,
+):
     """在当前目录下安装小派蒙以及go-cqhttp."""
     click.clear()
-    click.secho(LOGO, fg='green', bold=True)
     if only_gocq:
         with contextlib.suppress(CancelledError):
             gocq_download_domain = await ListPrompt(
                 '要使用的go-cqhttp下载源?',
-                [Choice('Github官方源(国外推荐)', 'github.com'),
-                 Choice('FastGit镜像源(国内推荐)', 'download.fgit.ml')],
-                default_select=1
+                [
+                    Choice('Github官方源(国外推荐)', 'github.com'),
+                    Choice('FastGit镜像源(国内推荐)', 'download.fgit.ml'),
+                ],
+                default_select=1,
             ).prompt_async(style=CLI_DEFAULT_STYLE)
             gocq_path = None
             try:
                 click.secho('下载go-cqhttp中...', fg='yellow')
                 gocq_path = download_gocq(gocq_download_domain.data)
             except CancelledError as e:
                 raise e
@@ -68,23 +76,25 @@
                 click.secho(f'下载go-cqhttp失败: {e}', fg='red')
             if gocq_path and gocq_path.exists():
                 bot_qq = await InputPrompt(
                     '机器人的QQ号:',
                     validator=lambda x: x.isdigit(),
                 ).prompt_async(style=CLI_DEFAULT_STYLE)
                 password = await InputPrompt(
-                    '机器人的密码(留空则为扫码登录):',
-                    is_password=True
+                    '机器人的密码(留空则为扫码登录):', is_password=True
                 ).prompt_async(style=CLI_DEFAULT_STYLE)
                 config_data = (
-                    (Path(__file__).parent.parent / 'config_template.yml').read_text(encoding='utf-8')
+                    (Path(__file__).parent.parent / 'config_template.yml')
+                    .read_text(encoding='utf-8')
                     .replace('{{ qq }}', bot_qq)
                     .replace('{{ password }}', password)
                 )
-                (Path('.') / 'go-cqhttp' / 'config.yml').write_text(config_data, encoding='utf-8')
+                (Path('.') / 'go-cqhttp' / 'config.yml').write_text(
+                    config_data, encoding='utf-8'
+                )
                 click.secho('go-cqhttp下载并配置完成')
             else:
                 click.secho('go-cqhttp下载失败, 请稍后手动安装', fg='red')
         ctx.exit()
 
     click.secho('检查前置环境...', fg='yellow')
     if not await check_git():
@@ -95,75 +105,95 @@
     try:
         is_clone = False
         while True:
             # 项目名称
             project_name = await InputPrompt(
                 '项目名称:',
                 default_text='LittlePaimon',
-                validator=project_name_validator
+                validator=project_name_validator,
             ).prompt_async(style=CLI_DEFAULT_STYLE)
             project_name = project_name.replace(' ', '-')
 
             # 检查项目是否存在
             if (Path('.') / project_name).is_dir():
                 dir_choice = await ListPrompt(
                     '当前目录下已存在同名项目文件夹，如何操作?',
                     [
                         Choice('删除该文件夹并重新克隆', 'delete'),
                         Choice('使用该文件夹中的内容并继续', 'use'),
                         Choice('重新命名', 'rename'),
                         Choice('取消安装', 'exit'),
                     ],
-                    default_select=0
+                    default_select=0,
                 ).prompt_async(style=CLI_DEFAULT_STYLE)
                 if dir_choice.data == 'rename':
                     pass
                 elif dir_choice.data == 'delete':
 
                     def delete(func, path_, execinfo):
                         os.chmod(path_, stat.S_IWUSR)
                         func(path_)
 
-                    shutil.rmtree((Path('.') / project_name).absolute(), onerror=delete)
+                    shutil.rmtree(
+                        (Path('.') / project_name).absolute(), onerror=delete
+                    )
                     await asyncio.sleep(0.2)
                     break
                 elif dir_choice.data == 'use':
                     is_clone = True
                     break
                 else:
                     ctx.exit()
             else:
                 break
 
         if not is_clone:
             git_url = await ListPrompt(
                 '要使用的克隆源?',
-                [Choice('github官方源(国外推荐)', 'https://github.com/CMHopeSunshine/LittlePaimon'),
-                 Choice('cherishmoon镜像源(国内推荐)',
-                        'https://github.cherishmoon.fun/https://github.com/CMHopeSunshine/LittlePaimon'),
-                 Choice('ghproxy镜像源(国内备选1)',
-                        'https://ghproxy.com/https://github.com/CMHopeSunshine/LittlePaimon'),
-                 Choice('gitee镜像源(国内备选2)', 'https://gitee.com/cherishmoon/LittlePaimon')],
-                default_select=1
+                [
+                    Choice(
+                        'github官方源(国外推荐)',
+                        'https://github.com/CMHopeSunshine/LittlePaimon',
+                    ),
+                    Choice(
+                        'cherishmoon镜像源(国内推荐)',
+                        'https://github.cherishmoon.fun/https://github.com/CMHopeSunshine/LittlePaimon',
+                    ),
+                    Choice(
+                        'ghproxy镜像源(国内备选1)',
+                        'https://ghproxy.com/https://github.com/CMHopeSunshine/LittlePaimon',
+                    ),
+                    Choice(
+                        'gitee镜像源(国内备选2)',
+                        'https://gitee.com/cherishmoon/LittlePaimon',
+                    ),
+                ],
+                default_select=1,
             ).prompt_async(style=CLI_DEFAULT_STYLE)
             click.secho(f'在 {project_name} 文件夹克隆源码...', fg='yellow')
             clone_result = await clone_paimon(git_url.data, project_name)
             await clone_result.wait()
 
             if not (Path('.') / project_name / '.env.prod').is_file():
                 ctx.exit()
 
-            env_file = (Path('.') / project_name / '.env.prod').read_text(encoding='utf-8')
+            env_file = (Path('.') / project_name / '.env.prod').read_text(
+                encoding='utf-8'
+            )
             superusers = await InputPrompt(
                 '超级用户QQ(即你自己的QQ号，多个用空格隔开):',
                 validator=lambda x: x.replace(' ', '').isdigit(),
             ).prompt_async(style=CLI_DEFAULT_STYLE)
             if superusers := superusers.replace(' ', '", "'):
-                env_file = env_file.replace('SUPERUSERS=["123456"]', f'SUPERUSERS=["{superusers}"]')
-            (Path('.') / project_name / '.env.prod').write_text(env_file, encoding='utf-8')
+                env_file = env_file.replace(
+                    'SUPERUSERS=["123456"]', f'SUPERUSERS=["{superusers}"]'
+                )
+            (Path('.') / project_name / '.env.prod').write_text(
+                env_file, encoding='utf-8'
+            )
 
         is_install_dependencies = await ConfirmPrompt(
             '立刻安装依赖?', default_choice=True
         ).prompt_async(style=CLI_DEFAULT_STYLE)
         venv_dir = Path('.') / project_name / '.venv'
 
         python_path = None
@@ -175,56 +205,73 @@
             python_path = None
             if is_use_venv:
                 click.secho(
                     f'在 {venv_dir} 中创建虚拟环境...',
                     fg='yellow',
                 )
                 await create_virtualenv(
-                    venv_dir, prompt=project_name, python_path=python_interpreter
+                    venv_dir,
+                    prompt=project_name,
+                    python_path=python_interpreter,
                 )
                 python_path = (
-                        venv_dir
-                        / ("Scripts" if WINDOWS else "bin")
-                        / ("python.exe" if WINDOWS else "python")
+                    venv_dir
+                    / ("Scripts" if WINDOWS else "bin")
+                    / ("python.exe" if WINDOWS else "python")
                 )
 
             click.secho('开始安装相关依赖...', fg='yellow')
-            proc = await install_dependencies(file_path=Path('.') / project_name / 'requirements.txt',
-                                              python_path=python_path,
-                                              pip_args=['-i', index_url] if index_url else None)
+            proc = await install_dependencies(
+                file_path=Path('.') / project_name / 'requirements.txt',
+                python_path=python_path,
+                pip_args=['-i', index_url] if index_url else None,
+            )
             await proc.wait()
 
         if not (Path('.') / project_name).is_dir():
             ctx.exit()
 
         # go-cqhttp
         gocq_type = 0
         if (Path('.') / 'go-cqhttp' / f'go-cqhttp{EXECUTABLE_EXT}').exists():
             click.secho('检测到当前目录下已有go-cqhttp本体，跳过安装go-cqhttp', fg='yellow')
         else:
             install_gocq_type = await ListPrompt(
                 'go-cqhttp安装和使用方式?',
-                [Choice('nonebot-plugin-gocqhttp插件', 'plugin'),
-                 Choice('go-cqhttp本体', 'gocq'),
-                 Choice('我已安装或稍候自行安装', 'skip')],
-                default_select=0).prompt_async(style=CLI_DEFAULT_STYLE)
+                [
+                    Choice('nonebot-plugin-gocqhttp插件', 'plugin'),
+                    Choice('go-cqhttp本体', 'gocq'),
+                    Choice('我已安装或稍候自行安装', 'skip'),
+                ],
+                default_select=0,
+            ).prompt_async(style=CLI_DEFAULT_STYLE)
 
             if install_gocq_type.data == 'plugin':
                 gocq_type = 1
-                proc = await call_pip_install('nonebot-plugin-gocqhttp', python_path=python_path)
+                proc = await call_pip_install(
+                    'nonebot-plugin-gocqhttp', python_path=python_path
+                )
                 await proc.wait()
-                toml_file = (Path('.') / project_name / 'pyproject.toml').read_text(encoding='utf-8')
-                toml_file = toml_file.replace('plugins = []', 'plugins = ["nonebot_plugin_gocqhttp"]')
-                (Path('.') / project_name / 'pyproject.toml').write_text(toml_file, encoding='utf-8')
+                toml_file = (
+                    Path('.') / project_name / 'pyproject.toml'
+                ).read_text(encoding='utf-8')
+                toml_file = toml_file.replace(
+                    'plugins = []', 'plugins = ["nonebot_plugin_gocqhttp"]'
+                )
+                (Path('.') / project_name / 'pyproject.toml').write_text(
+                    toml_file, encoding='utf-8'
+                )
             elif install_gocq_type.data == 'gocq':
                 gocq_download_domain = await ListPrompt(
                     '要使用的go-cqhttp下载源?',
-                    [Choice('Github官方源(国外推荐)', 'github.com'),
-                     Choice('FastGit镜像源(国内推荐)', 'download.fgit.ml')],
-                    default_select=1
+                    [
+                        Choice('Github官方源(国外推荐)', 'github.com'),
+                        Choice('FastGit镜像源(国内推荐)', 'download.fgit.ml'),
+                    ],
+                    default_select=1,
                 ).prompt_async(style=CLI_DEFAULT_STYLE)
                 gocq_path = None
                 try:
                     click.secho('下载go-cqhttp中...', fg='yellow')
                     gocq_path = download_gocq(gocq_download_domain.data)
                 except CancelledError as e:
                     raise e
@@ -233,23 +280,25 @@
                 if gocq_path and gocq_path.exists():
                     gocq_type = 2
                     bot_qq = await InputPrompt(
                         '机器人的QQ号:',
                         validator=lambda x: x.isdigit(),
                     ).prompt_async(style=CLI_DEFAULT_STYLE)
                     password = await InputPrompt(
-                        '机器人的密码(留空则为扫码登录):',
-                        is_password=True
+                        '机器人的密码(留空则为扫码登录):', is_password=True
                     ).prompt_async(style=CLI_DEFAULT_STYLE)
                     config_data = (
-                        (Path(__file__).parent.parent / 'config_template.yml').read_text(encoding='utf-8')
+                        (Path(__file__).parent.parent / 'config_template.yml')
+                        .read_text(encoding='utf-8')
                         .replace('{{ qq }}', bot_qq)
                         .replace('{{ password }}', password)
                     )
-                    (Path('.') / 'go-cqhttp' / 'config.yml').write_text(config_data, encoding='utf-8')
+                    (Path('.') / 'go-cqhttp' / 'config.yml').write_text(
+                        config_data, encoding='utf-8'
+                    )
                 else:
                     click.secho('go-cqhttp安装失败, 请稍后手动安装', fg='red')
         click.secho('安装完成!', fg='green')
         click.secho('运行以下命令来启动你的小派蒙:', fg='green')
         if gocq_type == 2:
             if WINDOWS:
                 click.secho(f'  cd {project_name}', fg='green')
```

### Comparing `nb_cli_plugin_littlepaimon-1.0.0rc3/nb_cli_plugin_littlepaimon/commands/install.py` & `nb_cli_plugin_littlepaimon-1.0.1/nb_cli_plugin_littlepaimon/commands/install.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,55 +1,58 @@
 from pathlib import Path
-from typing import Optional, List
+from typing import List, Optional
 
 import click
-from nb_cli.cli import run_async, ClickAliasedCommand
-from nb_cli.handlers import detect_virtualenv, call_pip_install
+from nb_cli.cli import ClickAliasedCommand, run_async
+from nb_cli.handlers import call_pip_install, detect_virtualenv
 
 from ..handlers.cmd import install_dependencies
 
 
 @click.command(
     cls=ClickAliasedCommand,
     aliases=['add'],
     context_settings={"ignore_unknown_options": True},
-    help='安装依赖库到小派蒙项目中.'
+    help='安装依赖库到小派蒙中.',
+)
+@click.argument('name', nargs=-1, required=False, default=None)
+@click.option(
+    '-f',
+    '--file',
+    default='requirements.txt',
+    type=click.Path(exists=True),
+    help='指定依赖文件的路径',
+)
+@click.option(
+    '-i', '--index-url', 'index_url', default=None, help='pip下载所使用的镜像源'
 )
-@click.argument('name',
-                nargs=-1,
-                required=False,
-                default=None)
-@click.option('-f',
-              '--file',
-              default='requirements.txt',
-              type=click.Path(exists=True),
-              help='指定依赖文件的路径')
-@click.option('-i',
-              '--index-url',
-              'index_url',
-              default=None,
-              help='pip下载所使用的镜像源')
 @click.pass_context
 @run_async
-async def install(ctx: click.Context, name: Optional[List[str]], file: Path, index_url: Optional[str]):
+async def install(
+    ctx: click.Context,
+    name: Optional[List[str]],
+    file: Path,
+    index_url: Optional[str],
+):
     file_path = Path(file).absolute()
-    if not ((file_path.parent / 'LittlePaimon').is_dir() and (file_path.parent / 'bot.py').is_file()):
+    if not (
+        (file_path.parent / 'LittlePaimon').is_dir()
+        and (file_path.parent / 'bot.py').is_file()
+    ):
         click.secho('未检测到当前目录下有小派蒙项目，请确保目录无误', fg='red')
         ctx.exit()
     if python_path := detect_virtualenv(file_path.parent):
-        click.secho(
-            f'使用虚拟环境: {python_path}',
-            fg="green"
-        )
+        click.secho(f'使用虚拟环境: {python_path}', fg="green")
     proc = (
         await call_pip_install(
             name,
             python_path=python_path,
-            pip_args=['-i', index_url] if index_url else None
+            pip_args=['-i', index_url] if index_url else None,
         )
         if name
-        else await install_dependencies(file_path=file_path,
-                                        python_path=python_path,
-                                        pip_args=['-i', index_url] if index_url else None
-                                        )
+        else await install_dependencies(
+            file_path=file_path,
+            python_path=python_path,
+            pip_args=['-i', index_url] if index_url else None,
+        )
     )
     await proc.wait()
```

### Comparing `nb_cli_plugin_littlepaimon-1.0.0rc3/nb_cli_plugin_littlepaimon/commands/resources.py` & `nb_cli_plugin_littlepaimon-1.0.1/nb_cli_plugin_littlepaimon/commands/resources.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,164 +1,222 @@
 import hashlib
 import zipfile
 from pathlib import Path
 from typing import Optional
 
 import click
-from nb_cli.cli import run_async, ClickAliasedCommand, CLI_DEFAULT_STYLE
-from noneprompt import Choice, ListPrompt, CancelledError, CheckboxPrompt, ConfirmPrompt
+from rich.console import Console
+from nb_cli.cli import CLI_DEFAULT_STYLE, ClickAliasedCommand, run_async
+from noneprompt import (
+    Choice,
+    ListPrompt,
+    ConfirmPrompt,
+    CancelledError,
+    CheckboxPrompt,
+)
+
+from ..handlers import download_json, download_with_bar
 
-from ..handlers import download_with_bar, download_json
+console = Console()
 
 
 @click.command(
     cls=ClickAliasedCommand,
     aliases=['res'],
     context_settings={"ignore_unknown_options": True},
-    help='下载或更新小派蒙的资源.'
+    help='下载或更新小派蒙资源.',
 )
 @click.option(
-    '-f',
-    '--force',
-    default=False,
-    is_flag=True,
-    help='是否强制下载资源，不管是否在小派蒙目录中.'
+    '-f', '--force', default=False, is_flag=True, help='是否强制下载资源，不管是否在小派蒙目录中.'
 )
 @click.option(
     '-u',
     '--url',
     'only_url',
     default=False,
     is_flag=True,
-    help='是否只展示下载链接而不进行下载.'
+    help='是否只展示下载链接而不进行下载.',
 )
 @click.pass_context
 @run_async
-async def resources(ctx: click.Context,
-                    force: Optional[bool] = False,
-                    only_url: Optional[bool] = False):
+async def resources(
+    ctx: click.Context,
+    force: Optional[bool] = False,
+    only_url: Optional[bool] = False,
+):
     if only_url:
         click.secho(
             '小派蒙基础必需资源: https://raw.githubusercontent.com/CMHopeSunshine/LittlePaimonRes/main/resources.zip',
-            fg='yellow')
+            fg='yellow',
+        )
         # click.secho(
         #     '原神数据信息: https://raw.githubusercontent.com/CMHopeSunshine/GenshinWikiMap/master/data/data.zip',
         #     fg='yellow')
         click.secho(
             '原神图标资源: https://raw.githubusercontent.com/CMHopeSunshine/GenshinWikiMap/master/resources/genshin_resources.zip',
-            fg='yellow')
+            fg='yellow',
+        )
+        click.secho(
+            '原神图标资源: https://raw.githubusercontent.com/CMHopeSunshine/GenshinWikiMap/master/resources/genshin_splash.zip',
+            fg='yellow',
+        )
         click.secho('如有需要请自行下载!', fg='yellow')
         ctx.exit()
     cwd_path = Path('.')
-    if not force and not ((cwd_path / 'LittlePaimon').is_dir() and (cwd_path / 'pyproject.toml').is_file()):
+    if not force and not (
+        (cwd_path / 'LittlePaimon').is_dir()
+        and (cwd_path / 'pyproject.toml').is_file()
+    ):
         click.secho('未检测到当前文件夹有小派蒙项目', fg='red')
         ctx.exit()
     try:
         confirm = False
         res_type = []
         while not confirm:
             res_type = await CheckboxPrompt(
                 '你要下载(更新)哪些资源?',
                 [
                     Choice('小派蒙基础必需资源', 'base'),
                     # Choice('原神数据信息', 'data'),
-                    Choice('原神图标资源', 'icon')
+                    Choice('原神图标资源', 'icon'),
+                    Choice('原神立绘资源', 'splash'),
                 ],
-                default_select=[0, 1]
+                default_select=[0, 1, 2],
             ).prompt_async(style=CLI_DEFAULT_STYLE)
             confirm = (
                 True
                 if res_type
                 else await ConfirmPrompt(
                     '你还没选择任何资源',
                     default_choice=False,
                 ).prompt_async(style=CLI_DEFAULT_STYLE)
             )
         if not (res_type := [res.data for res in res_type]):
             ctx.exit()
         download_url = await ListPrompt(
             '要使用的资源下载源?',
-            [Choice('github官方源(国外推荐)', ''),
-             Choice('cherishmoon镜像源(国内推荐)',
-                    'https://github.cherishmoon.fun/'),
-             Choice('ghproxy镜像源(国内备选)',
-                    'https://ghproxy.com/')],
-            default_select=1
+            [
+                Choice('github官方源(国外推荐)', ''),
+                Choice(
+                    'cherishmoon镜像源(国内推荐)', 'https://github.cherishmoon.fun/'
+                ),
+                Choice('ghproxy镜像源(国内备选)', 'https://ghproxy.com/'),
+            ],
+            default_select=1,
         ).prompt_async(style=CLI_DEFAULT_STYLE)
         download_url = download_url.data
         if 'base' in res_type:
             resources_path = cwd_path / 'resources'
             resources_path.mkdir(exist_ok=True, parents=True)
             base_zip_path = cwd_path / 'base.zip'
-            if (
-                    not force and
-                    ((resources_path / 'fonts').is_dir() and
-                     (resources_path / 'LittlePaimon').is_dir()
-                     and len(list((resources_path / 'LittlePaimon').rglob('*'))) >= 50)
+            if not force and (
+                (resources_path / 'fonts').is_dir()
+                and (resources_path / 'LittlePaimon').is_dir()
+                and len(list((resources_path / 'LittlePaimon').rglob('*')))
+                >= 50
             ):
                 click.secho('检测到已有部分基础资源，进行增量更新...', fg='yellow')
                 base_resources_list = download_json(
-                    f'{download_url}https://raw.githubusercontent.com/CMHopeSunshine/LittlePaimonRes/main/resources_list.json')
+                    f'{download_url}https://raw.githubusercontent.com/CMHopeSunshine/LittlePaimonRes/main/resources_list.json'
+                )
                 for resource in base_resources_list:
                     file_path = resources_path / resource['path']
                     if file_path.exists():
-                        if not resource['lock'] or hashlib.md5(file_path.read_bytes()).hexdigest() == resource['hash']:
+                        if (
+                            not resource['lock']
+                            or hashlib.md5(file_path.read_bytes()).hexdigest()
+                            == resource['hash']
+                        ):
                             continue
                         else:
                             file_path.unlink()
                     try:
                         download_with_bar(
                             url=f'{download_url}https://raw.githubusercontent.com/CMHopeSunshine/LittlePaimonRes/main/{resource["path"]}',
-                            save_path=file_path, show_name='基础资源' + resource['path'])
+                            save_path=file_path,
+                            show_name='基础资源' + resource['path'],
+                        )
                     except CancelledError as e:
                         raise e
                     except Exception as e:
-                        click.secho(f'下载基础资源{resource["path"]}出错: {e}', fg='red')
+                        click.secho(
+                            f'下载基础资源{resource["path"]}出错: {e}', fg='red'
+                        )
             else:
                 try:
                     download_with_bar(
                         f'{download_url}https://raw.githubusercontent.com/CMHopeSunshine/LittlePaimonRes/main/resources.zip',
-                        base_zip_path, '小派蒙基础资源')
-                    zipfile.ZipFile(base_zip_path).extractall(resources_path)
-                    click.secho('小派蒙基础资源下载完成', fg='green')
+                        base_zip_path,
+                        '小派蒙基础资源',
+                    )
+                    with console.status(
+                        "[bold yellow]解压小派蒙基础资源中..."
+                    ) as status:
+                        zipfile.ZipFile(base_zip_path).extractall(
+                            resources_path
+                        )
                 except CancelledError as e:
                     raise e
                 except Exception as e:
                     click.secho(f'下载小派蒙基础资源时出错: {e}', fg='red')
                 if base_zip_path.is_file():
                     base_zip_path.unlink()
 
         if 'data' in res_type:
             data_path = cwd_path / 'data' / 'LittlePaimon' / 'genshin_data'
             data_path.mkdir(exist_ok=True, parents=True)
             data_zip_path = cwd_path / 'data.zip'
             try:
                 download_with_bar(
                     f'{download_url}https://raw.githubusercontent.com/CMHopeSunshine/GenshinWikiMap/master/data/data.zip',
-                    data_zip_path, '原神数据信息')
-                zipfile.ZipFile(data_zip_path).extractall(data_path)
+                    data_zip_path,
+                    '原神数据信息',
+                )
+                with console.status("[bold yellow]解压原神数据资源中...") as status:
+                    zipfile.ZipFile(data_zip_path).extractall(data_path)
             except CancelledError as e:
                 raise e
             except Exception as e:
                 click.secho(f'下载原神数据信息时出错: {e}', fg='red')
             if data_zip_path.is_file():
                 data_zip_path.unlink()
         if 'icon' in res_type:
             resources_path = cwd_path / 'resources' / 'LittlePaimon'
             resources_path.mkdir(exist_ok=True, parents=True)
             icon_zip_path = cwd_path / 'icon.zip'
             try:
                 download_with_bar(
                     f'{download_url}https://raw.githubusercontent.com/CMHopeSunshine/GenshinWikiMap/master/resources/genshin_resources.zip',
-                    icon_zip_path, '原神图标资源')
-                zipfile.ZipFile(icon_zip_path).extractall(resources_path)
+                    icon_zip_path,
+                    '原神图标资源',
+                )
+                with console.status("[bold yellow]解压原神图标资源中...") as status:
+                    zipfile.ZipFile(icon_zip_path).extractall(resources_path)
             except CancelledError as e:
                 raise e
             except Exception as e:
                 click.secho(f'下载原神图标资源时出错: {e}', fg='red')
             if icon_zip_path.is_file():
                 icon_zip_path.unlink()
+        if 'splash' in res_type:
+            resources_path = cwd_path / 'resources' / 'LittlePaimon' / 'splash'
+            resources_path.mkdir(exist_ok=True, parents=True)
+            splash_zip_path = cwd_path / 'splash.zip'
+            try:
+                download_with_bar(
+                    f'{download_url}https://raw.githubusercontent.com/CMHopeSunshine/GenshinWikiMap/master/resources/genshin_splash.zip',
+                    splash_zip_path,
+                    '原神图标资源',
+                )
+                with console.status("[bold yellow]解压原神立绘资源中...") as status:
+                    zipfile.ZipFile(splash_zip_path).extractall(resources_path)
+            except CancelledError as e:
+                raise e
+            except Exception as e:
+                click.secho(f'下载原神立绘资源时出错: {e}', fg='red')
+            if splash_zip_path.is_file():
+                splash_zip_path.unlink()
 
-        click.secho('全部资源更新完成', fg='green')
+        click.secho('资源更新完成', fg='green', bold=True)
 
     except CancelledError:
         ctx.exit()
```

### Comparing `nb_cli_plugin_littlepaimon-1.0.0rc3/nb_cli_plugin_littlepaimon/commands/run.py` & `nb_cli_plugin_littlepaimon-1.0.1/nb_cli_plugin_littlepaimon/commands/update.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,48 @@
 import asyncio
 from pathlib import Path
 
 import click
 from nb_cli.cli import ClickAliasedCommand, run_async
 from nb_cli.handlers import (
-    detect_virtualenv,
-    register_signal_handler,
     terminate_process,
-    run_project,
-    remove_signal_handler
+    remove_signal_handler,
+    register_signal_handler,
 )
 
+from ..handlers import git_pull
+
 
 @click.command(
-    cls=ClickAliasedCommand, aliases=['start'], help='在当前目录下启动小派蒙Bot.'
+    cls=ClickAliasedCommand, aliases=['upgrade'], help='检测更新并更新小派蒙.'
 )
 @click.option("-d", "--cwd", default=".", help='指定工作目录.')
 @click.pass_context
 @run_async
-async def run(ctx: click.Context, cwd: str):
-    if not ((Path(cwd) / 'LittlePaimon').is_dir() and (Path(cwd) / 'bot.py').is_file()):
+async def update(ctx: click.Context, cwd: str):
+    if not (
+        (Path(cwd) / 'LittlePaimon').is_dir()
+        and (Path(cwd) / 'bot.py').is_file()
+    ):
         click.secho('未检测到当前目录下有小派蒙项目，请确保目录无误', fg='red')
         ctx.exit()
-    if python_path := detect_virtualenv(Path(cwd)):
-        click.secho(
-            f'使用虚拟环境: {python_path}',
-            fg="green"
-        )
+    if not (Path(cwd) / '.git').is_dir():
+        click.secho('未检测到当前目录下有git仓库，无法通过git更新', fg='red')
+        ctx.exit()
+
     should_exit = asyncio.Event()
 
     def shutdown(signum, frame):
         should_exit.set()
 
     register_signal_handler(shutdown)
 
     async def wait_for_exit():
         await should_exit.wait()
         await terminate_process(proc)
 
-    proc = await run_project(python_path=python_path, cwd=Path(cwd))
+    proc = await git_pull(cwd=Path(cwd))
     task = asyncio.create_task(wait_for_exit())
     await proc.wait()
     should_exit.set()
     await task
     remove_signal_handler(shutdown)
```

### Comparing `nb_cli_plugin_littlepaimon-1.0.0rc3/nb_cli_plugin_littlepaimon/config_template.yml` & `nb_cli_plugin_littlepaimon-1.0.1/nb_cli_plugin_littlepaimon/config_template.yml`

 * *Files identical despite different names*

### Comparing `nb_cli_plugin_littlepaimon-1.0.0rc3/nb_cli_plugin_littlepaimon/handlers/cmd.py` & `nb_cli_plugin_littlepaimon-1.0.1/nb_cli_plugin_littlepaimon/handlers/cmd.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,71 +1,84 @@
 import asyncio
 from pathlib import Path
-from typing import Optional, List
+from typing import List, Optional
 
 from nb_cli.handlers import get_default_python
 
 
-async def clone_paimon(git_url: str,
-                       dir_name: Optional[str] = 'LittlePaimon'):
+async def clone_paimon(git_url: str, dir_name: Optional[str] = 'LittlePaimon'):
     """
     克隆派蒙项目
 
     :param git_url: git仓库地址
     :param dir_name: 要存放的文件夹名
     """
-    return await asyncio.create_subprocess_exec('git',
-                                                'clone',
-                                                '--depth=1',
-                                                '--single-branch',
-                                                git_url,
-                                                dir_name)
+    return await asyncio.create_subprocess_exec(
+        'git', 'clone', '--depth=1', '--single-branch', git_url, dir_name
+    )
 
 
-async def install_dependencies(file_path: Path,
-                               python_path: Optional[str] = None,
-                               pip_args: Optional[List[str]] = None):
+async def install_dependencies(
+    file_path: Path,
+    python_path: Optional[str] = None,
+    pip_args: Optional[List[str]] = None,
+):
     """
     安装requirements.txt中的依赖
 
     :param file_path: 依赖库文件路径
     :param python_path: python解释器路径
     :param pip_args: pip参数
     """
     if pip_args is None:
         pip_args = []
     if python_path is None:
         python_path = await get_default_python()
     if isinstance(python_path, Path):
         python_path = python_path.absolute()
-    return await asyncio.create_subprocess_exec(python_path,
-                                                '-m',
-                                                'pip',
-                                                'install',
-                                                '-r',
-                                                file_path.name,
-                                                *pip_args,
-                                                cwd=file_path.parent.absolute())
+    return await asyncio.create_subprocess_exec(
+        python_path,
+        '-m',
+        'pip',
+        'install',
+        '-r',
+        file_path.name,
+        *pip_args,
+        cwd=file_path.parent.absolute(),
+    )
+
+
+async def run_python_command(
+    command: List[str],
+    python_path: Optional[str] = None,
+    cwd: Optional[Path] = None,
+):
+    if python_path is None:
+        python_path = await get_default_python()
+    return await asyncio.create_subprocess_exec(
+        python_path, '-m', *command, cwd=cwd
+    )
 
 
 async def check_git() -> bool:
     """
     检查环境变量中是否存在 git
 
     :return: 布尔值
     """
-    process = await asyncio.create_subprocess_shell('git --version',
-                                                    stdout=asyncio.subprocess.PIPE,
-                                                    stderr=asyncio.subprocess.PIPE)
+    process = await asyncio.create_subprocess_shell(
+        'git --version',
+        stdout=asyncio.subprocess.PIPE,
+        stderr=asyncio.subprocess.PIPE,
+    )
     stdout, _ = await process.communicate()
     return bool(stdout)
 
 
 async def git_pull(cwd: Optional[Path] = None):
     """
     通过git更新派蒙项目
 
     """
-    process = await asyncio.create_subprocess_shell('git pull',
-                                                    cwd=cwd)
+    process = await asyncio.create_subprocess_shell('git pull', cwd=cwd)
     stdout, _ = await process.communicate()
     return process
```

### Comparing `nb_cli_plugin_littlepaimon-1.0.0rc3/nb_cli_plugin_littlepaimon/handlers/download.py` & `nb_cli_plugin_littlepaimon-1.0.1/nb_cli_plugin_littlepaimon/handlers/download.py`

 * *Files identical despite different names*

### Comparing `nb_cli_plugin_littlepaimon-1.0.0rc3/nb_cli_plugin_littlepaimon/handlers/gocq.py` & `nb_cli_plugin_littlepaimon-1.0.1/nb_cli_plugin_littlepaimon/handlers/gocq.py`

 * *Files identical despite different names*

### Comparing `nb_cli_plugin_littlepaimon-1.0.0rc3/nb_cli_plugin_littlepaimon/meta.py` & `nb_cli_plugin_littlepaimon-1.0.1/nb_cli_plugin_littlepaimon/meta.py`

 * *Files identical despite different names*

### Comparing `nb_cli_plugin_littlepaimon-1.0.0rc3/PKG-INFO` & `nb_cli_plugin_littlepaimon-1.0.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nb-cli-plugin-littlepaimon
-Version: 1.0.0rc3
+Version: 1.0.1
 Summary: Nonebot Cli plugin for LittlePaimon
 Home-page: https://github.com/CMHopeSunshine/nb-cli-plugin-littlepaimon
 License: AGPL
 Keywords: nonebot2,nb-cli
 Author: CMHopeSunshine
 Author-email: 277073121@qq.com
 Requires-Python: >=3.8,<4.0
@@ -115,17 +115,21 @@
 
 ## 使用
 
 - `nb paimon` 交互式使用
   - `nb paimon create` 
     - 交互式指引安装[LittlePaimon](https://github.com/CMHopeSunshine/LittlePaimon)
     - 自动克隆源码、创建虚拟环境、安装依赖，下载并配置go-cqhttp
-  - `nb paimon run` 启动小派蒙
-    - 实际上和`nb run`一样，不过去掉了不常用的参数 
+    - 添加`-g`参数，则是只下载go-cqhttp
+  - `nb paimon run` 运行python命令或启动小派蒙
+    - 当接有命令时，使用该目录的下python解释器运行命令，例如`nb paimon run playwright install`
+    - 当没有命令时，使用该目录的下python解释器启动小派蒙，实际上等价于`nb run`，不过去掉了不常用的参数 
   - `nb paimon install` 安装依赖库到小派蒙环境中
+    - 当接有参数时，使用该目录的下pip安装依赖，例如`nb paimon install httpx`
+    - 当没有参数时，则是使用该目录的下pip安装`requirements.txt`中的依赖
   - `nb paimon res` 下载或更新小派蒙的资源
   - `nb paimon update` 更新小派蒙，和`git pull`一样
   - `nb paimon logo` 展示小派蒙的logo
 - `nb paimon (指令) --help` 查看帮助
 
 ## TODO
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: nb-cli-plugin-littlepaimon Version: 1.0.0rc3
-Summary: Nonebot Cli plugin for LittlePaimon Home-page: https://github.com/
+Metadata-Version: 2.1 Name: nb-cli-plugin-littlepaimon Version: 1.0.1 Summary:
+Nonebot Cli plugin for LittlePaimon Home-page: https://github.com/
 CMHopeSunshine/nb-cli-plugin-littlepaimon License: AGPL Keywords: nonebot2,nb-
 cli Author: CMHopeSunshine Author-email: 277073121@qq.com Requires-Python:
 >=3.8,<4.0 Classifier: License :: Other/Proprietary License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Requires-Dist: nb-cli (>=1.0.2,<2.0.0) Requires-Dist: py-cpuinfo
@@ -21,16 +21,23 @@
 éè¿ nb-cli å®è£ ```shell nb self install nb-cli-plugin-littlepaimon ```
 éè¿ pipx å®è£ ```shell pipx inject nb-cli nb-cli-plugin-littlepaimon ```
 éè¿ pip å®è£ ```shell pip install nb-cli-plugin-littlepaimon ```   --
 -  å®è£Git ~~è½ä¸Githubçè¯ï¼åºè¯¥é½ä¼è£Gitå§)~~  ## ä½¿ç¨ - `nb
 paimon` äº¤äºå¼ä½¿ç¨ - `nb paimon create` - äº¤äºå¼æå¼å®è£
 [LittlePaimon](https://github.com/CMHopeSunshine/LittlePaimon) -
 èªå¨åéæºç ãåå»ºèæç¯å¢ãå®è£ä¾èµï¼ä¸è½½å¹¶éç½®go-
-cqhttp - `nb paimon run` å¯å¨å°æ´¾è - å®éä¸å`nb
-run`ä¸æ ·ï¼ä¸è¿å»æäºä¸å¸¸ç¨çåæ° - `nb paimon install`
-å®è£ä¾èµåºå°å°æ´¾èç¯å¢ä¸­ - `nb paimon res`
-ä¸è½½ææ´æ°å°æ´¾èçèµæº - `nb paimon update`
+cqhttp - æ·»å `-g`åæ°ï¼åæ¯åªä¸è½½go-cqhttp - `nb paimon run`
+è¿è¡pythonå½ä»¤æå¯å¨å°æ´¾è -
+å½æ¥æå½ä»¤æ¶ï¼ä½¿ç¨è¯¥ç®å½çä¸pythonè§£éå¨è¿è¡å½ä»¤ï¼ä¾å¦`nb
+paimon run playwright install` -
+å½æ²¡æå½ä»¤æ¶ï¼ä½¿ç¨è¯¥ç®å½çä¸pythonè§£éå¨å¯å¨å°æ´¾èï¼å®éä¸ç­ä»·äº`nb
+run`ï¼ä¸è¿å»æäºä¸å¸¸ç¨çåæ° - `nb paimon install`
+å®è£ä¾èµåºå°å°æ´¾èç¯å¢ä¸­ -
+å½æ¥æåæ°æ¶ï¼ä½¿ç¨è¯¥ç®å½çä¸pipå®è£ä¾èµï¼ä¾å¦`nb paimon
+install httpx` -
+å½æ²¡æåæ°æ¶ï¼åæ¯ä½¿ç¨è¯¥ç®å½çä¸pipå®è£`requirements.txt`ä¸­çä¾èµ
+- `nb paimon res` ä¸è½½ææ´æ°å°æ´¾èçèµæº - `nb paimon update`
 æ´æ°å°æ´¾èï¼å`git pull`ä¸æ · - `nb paimon logo` å±ç¤ºå°æ´¾èçlogo
 - `nb paimon (æä»¤) --help` æ¥çå¸®å© ## TODO - [x] æ´æ°èµæº - [ ]
 ä¸ä¾èµgit - [ ] ä¿®æ¹éç½® - [ ] å®è£å°æ´¾èæä»¶ - [ ] more ##
 ç¸å³é¡¹ç® - [nb-cli](https://github.com/nonebot/nb-cli) - [LittlePaimon]
 (https://github.com/CMHopeSunshine/LittlePaimon)
```

