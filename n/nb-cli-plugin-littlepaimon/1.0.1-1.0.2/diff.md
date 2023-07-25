# Comparing `tmp/nb_cli_plugin_littlepaimon-1.0.1.tar.gz` & `tmp/nb_cli_plugin_littlepaimon-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nb_cli_plugin_littlepaimon-1.0.1.tar", max compression
+gzip compressed data, was "nb_cli_plugin_littlepaimon-1.0.2.tar", max compression
```

## Comparing `nb_cli_plugin_littlepaimon-1.0.1.tar` & `nb_cli_plugin_littlepaimon-1.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    34523 2023-07-25 05:09:45.892779 nb_cli_plugin_littlepaimon-1.0.1/LICENSE
--rw-r--r--   0        0        0     3010 2023-07-25 05:09:45.892779 nb_cli_plugin_littlepaimon-1.0.1/README.md
--rw-r--r--   0        0        0      235 2023-07-25 05:09:45.892779 nb_cli_plugin_littlepaimon-1.0.1/nb_cli_plugin_littlepaimon/__init__.py
--rw-r--r--   0        0        0     2067 2023-07-25 05:09:45.892779 nb_cli_plugin_littlepaimon-1.0.1/nb_cli_plugin_littlepaimon/cli.py
--rw-r--r--   0        0        0      137 2023-07-25 05:09:45.892779 nb_cli_plugin_littlepaimon-1.0.1/nb_cli_plugin_littlepaimon/commands/__init__.py
--rw-r--r--   0        0        0    13187 2023-07-25 05:09:45.892779 nb_cli_plugin_littlepaimon-1.0.1/nb_cli_plugin_littlepaimon/commands/create.py
--rw-r--r--   0        0        0     1696 2023-07-25 05:09:45.892779 nb_cli_plugin_littlepaimon-1.0.1/nb_cli_plugin_littlepaimon/commands/install.py
--rw-r--r--   0        0        0     9212 2023-07-25 05:09:45.892779 nb_cli_plugin_littlepaimon-1.0.1/nb_cli_plugin_littlepaimon/commands/resources.py
--rw-r--r--   0        0        0     1704 2023-07-25 05:09:45.892779 nb_cli_plugin_littlepaimon-1.0.1/nb_cli_plugin_littlepaimon/commands/run.py
--rw-r--r--   0        0        0     1323 2023-07-25 05:09:45.892779 nb_cli_plugin_littlepaimon-1.0.1/nb_cli_plugin_littlepaimon/commands/update.py
--rw-r--r--   0        0        0     3239 2023-07-25 05:09:45.892779 nb_cli_plugin_littlepaimon-1.0.1/nb_cli_plugin_littlepaimon/config_template.yml
--rw-r--r--   0        0        0      105 2023-07-25 05:09:45.892779 nb_cli_plugin_littlepaimon-1.0.1/nb_cli_plugin_littlepaimon/handlers/__init__.py
--rw-r--r--   0        0        0     2089 2023-07-25 05:09:45.892779 nb_cli_plugin_littlepaimon-1.0.1/nb_cli_plugin_littlepaimon/handlers/cmd.py
--rw-r--r--   0        0        0     1828 2023-07-25 05:09:45.892779 nb_cli_plugin_littlepaimon-1.0.1/nb_cli_plugin_littlepaimon/handlers/download.py
--rw-r--r--   0        0        0     1512 2023-07-25 05:09:45.892779 nb_cli_plugin_littlepaimon-1.0.1/nb_cli_plugin_littlepaimon/handlers/gocq.py
--rw-r--r--   0        0        0     1443 2023-07-25 05:09:45.892779 nb_cli_plugin_littlepaimon-1.0.1/nb_cli_plugin_littlepaimon/meta.py
--rw-r--r--   0        0        0      209 2023-07-25 05:09:45.892779 nb_cli_plugin_littlepaimon-1.0.1/nb_cli_plugin_littlepaimon/plugin.py
--rw-r--r--   0        0        0     1102 2023-07-25 05:09:45.892779 nb_cli_plugin_littlepaimon-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     3782 1970-01-01 00:00:00.000000 nb_cli_plugin_littlepaimon-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-07-25 05:17:44.072371 nb_cli_plugin_littlepaimon-1.0.2/LICENSE
+-rw-r--r--   0        0        0     3010 2023-07-25 05:17:44.072371 nb_cli_plugin_littlepaimon-1.0.2/README.md
+-rw-r--r--   0        0        0      235 2023-07-25 05:17:44.072371 nb_cli_plugin_littlepaimon-1.0.2/nb_cli_plugin_littlepaimon/__init__.py
+-rw-r--r--   0        0        0     2067 2023-07-25 05:17:44.072371 nb_cli_plugin_littlepaimon-1.0.2/nb_cli_plugin_littlepaimon/cli.py
+-rw-r--r--   0        0        0      137 2023-07-25 05:17:44.072371 nb_cli_plugin_littlepaimon-1.0.2/nb_cli_plugin_littlepaimon/commands/__init__.py
+-rw-r--r--   0        0        0    13187 2023-07-25 05:17:44.072371 nb_cli_plugin_littlepaimon-1.0.2/nb_cli_plugin_littlepaimon/commands/create.py
+-rw-r--r--   0        0        0     1696 2023-07-25 05:17:44.072371 nb_cli_plugin_littlepaimon-1.0.2/nb_cli_plugin_littlepaimon/commands/install.py
+-rw-r--r--   0        0        0     9093 2023-07-25 05:17:44.072371 nb_cli_plugin_littlepaimon-1.0.2/nb_cli_plugin_littlepaimon/commands/resources.py
+-rw-r--r--   0        0        0     1704 2023-07-25 05:17:44.072371 nb_cli_plugin_littlepaimon-1.0.2/nb_cli_plugin_littlepaimon/commands/run.py
+-rw-r--r--   0        0        0     1323 2023-07-25 05:17:44.072371 nb_cli_plugin_littlepaimon-1.0.2/nb_cli_plugin_littlepaimon/commands/update.py
+-rw-r--r--   0        0        0     3239 2023-07-25 05:17:44.072371 nb_cli_plugin_littlepaimon-1.0.2/nb_cli_plugin_littlepaimon/config_template.yml
+-rw-r--r--   0        0        0      105 2023-07-25 05:17:44.072371 nb_cli_plugin_littlepaimon-1.0.2/nb_cli_plugin_littlepaimon/handlers/__init__.py
+-rw-r--r--   0        0        0     2089 2023-07-25 05:17:44.072371 nb_cli_plugin_littlepaimon-1.0.2/nb_cli_plugin_littlepaimon/handlers/cmd.py
+-rw-r--r--   0        0        0     1828 2023-07-25 05:17:44.072371 nb_cli_plugin_littlepaimon-1.0.2/nb_cli_plugin_littlepaimon/handlers/download.py
+-rw-r--r--   0        0        0     1512 2023-07-25 05:17:44.072371 nb_cli_plugin_littlepaimon-1.0.2/nb_cli_plugin_littlepaimon/handlers/gocq.py
+-rw-r--r--   0        0        0     1443 2023-07-25 05:17:44.072371 nb_cli_plugin_littlepaimon-1.0.2/nb_cli_plugin_littlepaimon/meta.py
+-rw-r--r--   0        0        0      209 2023-07-25 05:17:44.072371 nb_cli_plugin_littlepaimon-1.0.2/nb_cli_plugin_littlepaimon/plugin.py
+-rw-r--r--   0        0        0     1102 2023-07-25 05:17:44.072371 nb_cli_plugin_littlepaimon-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3782 1970-01-01 00:00:00.000000 nb_cli_plugin_littlepaimon-1.0.2/PKG-INFO
```

### Comparing `nb_cli_plugin_littlepaimon-1.0.1/LICENSE` & `nb_cli_plugin_littlepaimon-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nb_cli_plugin_littlepaimon-1.0.1/README.md` & `nb_cli_plugin_littlepaimon-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `nb_cli_plugin_littlepaimon-1.0.1/nb_cli_plugin_littlepaimon/cli.py` & `nb_cli_plugin_littlepaimon-1.0.2/nb_cli_plugin_littlepaimon/cli.py`

 * *Files identical despite different names*

### Comparing `nb_cli_plugin_littlepaimon-1.0.1/nb_cli_plugin_littlepaimon/commands/create.py` & `nb_cli_plugin_littlepaimon-1.0.2/nb_cli_plugin_littlepaimon/commands/create.py`

 * *Files identical despite different names*

### Comparing `nb_cli_plugin_littlepaimon-1.0.1/nb_cli_plugin_littlepaimon/commands/install.py` & `nb_cli_plugin_littlepaimon-1.0.2/nb_cli_plugin_littlepaimon/commands/install.py`

 * *Files identical despite different names*

### Comparing `nb_cli_plugin_littlepaimon-1.0.1/nb_cli_plugin_littlepaimon/commands/resources.py` & `nb_cli_plugin_littlepaimon-1.0.2/nb_cli_plugin_littlepaimon/commands/resources.py`

 * *Files 3% similar despite different names*

```diff
@@ -144,17 +144,15 @@
             else:
                 try:
                     download_with_bar(
                         f'{download_url}https://raw.githubusercontent.com/CMHopeSunshine/LittlePaimonRes/main/resources.zip',
                         base_zip_path,
                         '小派蒙基础资源',
                     )
-                    with console.status(
-                        "[bold yellow]解压小派蒙基础资源中..."
-                    ) as status:
+                    with console.status("[bold yellow]解压小派蒙基础资源中..."):
                         zipfile.ZipFile(base_zip_path).extractall(
                             resources_path
                         )
                 except CancelledError as e:
                     raise e
                 except Exception as e:
                     click.secho(f'下载小派蒙基础资源时出错: {e}', fg='red')
@@ -163,55 +161,55 @@
 
         if 'data' in res_type:
             data_path = cwd_path / 'data' / 'LittlePaimon' / 'genshin_data'
             data_path.mkdir(exist_ok=True, parents=True)
             data_zip_path = cwd_path / 'data.zip'
             try:
                 download_with_bar(
-                    f'{download_url}https://raw.githubusercontent.com/CMHopeSunshine/GenshinWikiMap/master/data/data.zip',
+                    f'{download_url}https://github.com/CMHopeSunshine/GenshinWikiMap/raw/master/data/data.zip',
                     data_zip_path,
                     '原神数据信息',
                 )
-                with console.status("[bold yellow]解压原神数据资源中...") as status:
+                with console.status("[bold yellow]解压原神数据资源中..."):
                     zipfile.ZipFile(data_zip_path).extractall(data_path)
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
-                    f'{download_url}https://raw.githubusercontent.com/CMHopeSunshine/GenshinWikiMap/master/resources/genshin_resources.zip',
+                    f'{download_url}https://github.com/CMHopeSunshine/GenshinWikiMap/raw/master/resources/genshin_resources.zip',
                     icon_zip_path,
                     '原神图标资源',
                 )
-                with console.status("[bold yellow]解压原神图标资源中...") as status:
+                with console.status("[bold yellow]解压原神图标资源中..."):
                     zipfile.ZipFile(icon_zip_path).extractall(resources_path)
             except CancelledError as e:
                 raise e
             except Exception as e:
                 click.secho(f'下载原神图标资源时出错: {e}', fg='red')
             if icon_zip_path.is_file():
                 icon_zip_path.unlink()
         if 'splash' in res_type:
             resources_path = cwd_path / 'resources' / 'LittlePaimon' / 'splash'
             resources_path.mkdir(exist_ok=True, parents=True)
             splash_zip_path = cwd_path / 'splash.zip'
             try:
                 download_with_bar(
-                    f'{download_url}https://raw.githubusercontent.com/CMHopeSunshine/GenshinWikiMap/master/resources/genshin_splash.zip',
+                    f'{download_url}https://github.com/CMHopeSunshine/GenshinWikiMap/raw/master/resources/genshin_splash.zip',
                     splash_zip_path,
-                    '原神图标资源',
+                    '原神立绘资源',
                 )
-                with console.status("[bold yellow]解压原神立绘资源中...") as status:
+                with console.status("[bold yellow]解压原神立绘资源中..."):
                     zipfile.ZipFile(splash_zip_path).extractall(resources_path)
             except CancelledError as e:
                 raise e
             except Exception as e:
                 click.secho(f'下载原神立绘资源时出错: {e}', fg='red')
             if splash_zip_path.is_file():
                 splash_zip_path.unlink()
```

### Comparing `nb_cli_plugin_littlepaimon-1.0.1/nb_cli_plugin_littlepaimon/commands/run.py` & `nb_cli_plugin_littlepaimon-1.0.2/nb_cli_plugin_littlepaimon/commands/run.py`

 * *Files identical despite different names*

### Comparing `nb_cli_plugin_littlepaimon-1.0.1/nb_cli_plugin_littlepaimon/commands/update.py` & `nb_cli_plugin_littlepaimon-1.0.2/nb_cli_plugin_littlepaimon/commands/update.py`

 * *Files identical despite different names*

### Comparing `nb_cli_plugin_littlepaimon-1.0.1/nb_cli_plugin_littlepaimon/config_template.yml` & `nb_cli_plugin_littlepaimon-1.0.2/nb_cli_plugin_littlepaimon/config_template.yml`

 * *Files identical despite different names*

### Comparing `nb_cli_plugin_littlepaimon-1.0.1/nb_cli_plugin_littlepaimon/handlers/cmd.py` & `nb_cli_plugin_littlepaimon-1.0.2/nb_cli_plugin_littlepaimon/handlers/cmd.py`

 * *Files identical despite different names*

### Comparing `nb_cli_plugin_littlepaimon-1.0.1/nb_cli_plugin_littlepaimon/handlers/download.py` & `nb_cli_plugin_littlepaimon-1.0.2/nb_cli_plugin_littlepaimon/handlers/download.py`

 * *Files identical despite different names*

### Comparing `nb_cli_plugin_littlepaimon-1.0.1/nb_cli_plugin_littlepaimon/handlers/gocq.py` & `nb_cli_plugin_littlepaimon-1.0.2/nb_cli_plugin_littlepaimon/handlers/gocq.py`

 * *Files identical despite different names*

### Comparing `nb_cli_plugin_littlepaimon-1.0.1/nb_cli_plugin_littlepaimon/meta.py` & `nb_cli_plugin_littlepaimon-1.0.2/nb_cli_plugin_littlepaimon/meta.py`

 * *Files identical despite different names*

### Comparing `nb_cli_plugin_littlepaimon-1.0.1/pyproject.toml` & `nb_cli_plugin_littlepaimon-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nb-cli-plugin-littlepaimon"
-version = "1.0.1"
+version = "1.0.2"
 description = "Nonebot Cli plugin for LittlePaimon"
 authors = ["CMHopeSunshine <277073121@qq.com>"]
 keywords = ["nonebot2", "nb-cli"]
 homepage = "https://github.com/CMHopeSunshine/nb-cli-plugin-littlepaimon"
 readme = "README.md"
 license = "AGPL"
```

### Comparing `nb_cli_plugin_littlepaimon-1.0.1/PKG-INFO` & `nb_cli_plugin_littlepaimon-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nb-cli-plugin-littlepaimon
-Version: 1.0.1
+Version: 1.0.2
 Summary: Nonebot Cli plugin for LittlePaimon
 Home-page: https://github.com/CMHopeSunshine/nb-cli-plugin-littlepaimon
 License: AGPL
 Keywords: nonebot2,nb-cli
 Author: CMHopeSunshine
 Author-email: 277073121@qq.com
 Requires-Python: >=3.8,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nb-cli-plugin-littlepaimon Version: 1.0.1 Summary:
+Metadata-Version: 2.1 Name: nb-cli-plugin-littlepaimon Version: 1.0.2 Summary:
 Nonebot Cli plugin for LittlePaimon Home-page: https://github.com/
 CMHopeSunshine/nb-cli-plugin-littlepaimon License: AGPL Keywords: nonebot2,nb-
 cli Author: CMHopeSunshine Author-email: 277073121@qq.com Requires-Python:
 >=3.8,<4.0 Classifier: License :: Other/Proprietary License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```

