# Comparing `tmp/openplugin-py-0.0.4.tar.gz` & `tmp/openplugin-py-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openplugin-py-0.0.4.tar", last modified: Wed Jul 12 05:07:36 2023, max compression
+gzip compressed data, was "openplugin-py-0.0.5.tar", last modified: Tue Jul 25 03:37:58 2023, max compression
```

## Comparing `openplugin-py-0.0.4.tar` & `openplugin-py-0.0.5.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-12 05:07:36.323142 openplugin-py-0.0.4/
--rw-r--r--   0 4paradigm   (501) staff       (20)    11357 2023-06-28 13:02:04.000000 openplugin-py-0.0.4/LICENSE
--rw-r--r--   0 4paradigm   (501) staff       (20)     3838 2023-07-12 05:07:36.322995 openplugin-py-0.0.4/PKG-INFO
--rw-r--r--   0 4paradigm   (501) staff       (20)     2757 2023-07-12 03:42:45.000000 openplugin-py-0.0.4/README.md
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-12 05:07:36.315893 openplugin-py-0.0.4/openplugin/
--rw-r--r--   0 4paradigm   (501) staff       (20)     1114 2023-07-06 10:55:36.000000 openplugin-py-0.0.4/openplugin/__init__.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-12 05:07:36.316258 openplugin-py-0.0.4/openplugin/cli/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-06-26 08:37:33.000000 openplugin-py-0.0.4/openplugin/cli/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3080 2023-07-02 15:52:03.000000 openplugin-py-0.0.4/openplugin/cli/cli.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-12 05:07:36.317027 openplugin-py-0.0.4/openplugin/install/
--rw-r--r--   0 4paradigm   (501) staff       (20)     2656 2023-07-12 02:25:08.000000 openplugin-py-0.0.4/openplugin/install/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1528 2023-07-12 02:25:06.000000 openplugin-py-0.0.4/openplugin/install/local_install.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-12 05:07:36.317903 openplugin-py-0.0.4/openplugin/plugin/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-07-12 02:12:45.000000 openplugin-py-0.0.4/openplugin/plugin/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      928 2023-07-12 02:20:17.000000 openplugin-py-0.0.4/openplugin/plugin/base_plugin.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2194 2023-07-12 02:25:08.000000 openplugin-py-0.0.4/openplugin/plugin/webapp_plugin.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-12 05:07:36.318530 openplugin-py-0.0.4/openplugin/run/
--rw-r--r--   0 4paradigm   (501) staff       (20)     1259 2023-07-12 02:25:06.000000 openplugin-py-0.0.4/openplugin/run/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1014 2023-07-12 02:25:06.000000 openplugin-py-0.0.4/openplugin/run/local_run.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-12 05:07:36.320116 openplugin-py-0.0.4/openplugin/template/
--rw-r--r--   0 4paradigm   (501) staff       (20)      876 2023-07-02 15:52:03.000000 openplugin-py-0.0.4/openplugin/template/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1192 2023-07-02 15:52:03.000000 openplugin-py-0.0.4/openplugin/template/base_template.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      901 2023-07-02 15:52:03.000000 openplugin-py-0.0.4/openplugin/template/json_template.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      901 2023-07-02 15:52:03.000000 openplugin-py-0.0.4/openplugin/template/utils.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      902 2023-07-02 15:52:03.000000 openplugin-py-0.0.4/openplugin/template/yaml_template.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-12 05:07:36.321740 openplugin-py-0.0.4/openplugin/utils/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-06-26 08:58:04.000000 openplugin-py-0.0.4/openplugin/utils/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    17531 2023-06-30 09:22:51.000000 openplugin-py-0.0.4/openplugin/utils/app_util.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      915 2023-06-30 09:22:51.000000 openplugin-py-0.0.4/openplugin/utils/errors.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      989 2023-07-12 02:25:06.000000 openplugin-py-0.0.4/openplugin/utils/local_plugin_utils.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1798 2023-07-12 02:25:06.000000 openplugin-py-0.0.4/openplugin/utils/network_utils.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2321 2023-07-12 02:25:06.000000 openplugin-py-0.0.4/openplugin/utils/util.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-12 05:07:36.322786 openplugin-py-0.0.4/openplugin_py.egg-info/
--rw-r--r--   0 4paradigm   (501) staff       (20)     3838 2023-07-12 05:07:36.000000 openplugin-py-0.0.4/openplugin_py.egg-info/PKG-INFO
--rw-r--r--   0 4paradigm   (501) staff       (20)      897 2023-07-12 05:07:36.000000 openplugin-py-0.0.4/openplugin_py.egg-info/SOURCES.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)        1 2023-07-12 05:07:36.000000 openplugin-py-0.0.4/openplugin_py.egg-info/dependency_links.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)       46 2023-07-12 05:07:36.000000 openplugin-py-0.0.4/openplugin_py.egg-info/entry_points.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)      167 2023-07-12 05:07:36.000000 openplugin-py-0.0.4/openplugin_py.egg-info/requires.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)       11 2023-07-12 05:07:36.000000 openplugin-py-0.0.4/openplugin_py.egg-info/top_level.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)       38 2023-07-12 05:07:36.323193 openplugin-py-0.0.4/setup.cfg
--rw-r--r--   0 4paradigm   (501) staff       (20)     2869 2023-06-30 09:40:35.000000 openplugin-py-0.0.4/setup.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-25 03:37:58.595705 openplugin-py-0.0.5/
+-rw-r--r--   0 4paradigm   (501) staff       (20)    11357 2023-06-28 13:02:04.000000 openplugin-py-0.0.5/LICENSE
+-rw-r--r--   0 4paradigm   (501) staff       (20)     4113 2023-07-25 03:37:58.595571 openplugin-py-0.0.5/PKG-INFO
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3032 2023-07-25 03:33:26.000000 openplugin-py-0.0.5/README.md
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-25 03:37:58.589037 openplugin-py-0.0.5/openplugin/
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1114 2023-07-12 05:10:25.000000 openplugin-py-0.0.5/openplugin/__init__.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-25 03:37:58.589534 openplugin-py-0.0.5/openplugin/cli/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-06-26 08:37:33.000000 openplugin-py-0.0.5/openplugin/cli/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3080 2023-07-02 15:52:03.000000 openplugin-py-0.0.5/openplugin/cli/cli.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-25 03:37:58.590299 openplugin-py-0.0.5/openplugin/install/
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2855 2023-07-25 02:58:36.000000 openplugin-py-0.0.5/openplugin/install/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1528 2023-07-12 02:25:06.000000 openplugin-py-0.0.5/openplugin/install/local_install.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1799 2023-07-25 03:23:23.000000 openplugin-py-0.0.5/openplugin/install/zip_install.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-25 03:37:58.591118 openplugin-py-0.0.5/openplugin/plugin/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-07-12 02:12:45.000000 openplugin-py-0.0.5/openplugin/plugin/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      928 2023-07-12 02:20:17.000000 openplugin-py-0.0.5/openplugin/plugin/base_plugin.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2194 2023-07-12 02:25:08.000000 openplugin-py-0.0.5/openplugin/plugin/webapp_plugin.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-25 03:37:58.591611 openplugin-py-0.0.5/openplugin/run/
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1259 2023-07-12 02:25:06.000000 openplugin-py-0.0.5/openplugin/run/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1014 2023-07-12 02:25:06.000000 openplugin-py-0.0.5/openplugin/run/local_run.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-25 03:37:58.592925 openplugin-py-0.0.5/openplugin/template/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      876 2023-07-02 15:52:03.000000 openplugin-py-0.0.5/openplugin/template/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1192 2023-07-02 15:52:03.000000 openplugin-py-0.0.5/openplugin/template/base_template.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      901 2023-07-02 15:52:03.000000 openplugin-py-0.0.5/openplugin/template/json_template.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      901 2023-07-02 15:52:03.000000 openplugin-py-0.0.5/openplugin/template/utils.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      902 2023-07-02 15:52:03.000000 openplugin-py-0.0.5/openplugin/template/yaml_template.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-25 03:37:58.594495 openplugin-py-0.0.5/openplugin/utils/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-06-26 08:58:04.000000 openplugin-py-0.0.5/openplugin/utils/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    17531 2023-06-30 09:22:51.000000 openplugin-py-0.0.5/openplugin/utils/app_util.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      915 2023-06-30 09:22:51.000000 openplugin-py-0.0.5/openplugin/utils/errors.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1022 2023-07-25 03:26:46.000000 openplugin-py-0.0.5/openplugin/utils/local_plugin_utils.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1798 2023-07-12 02:25:06.000000 openplugin-py-0.0.5/openplugin/utils/network_utils.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2321 2023-07-12 02:25:06.000000 openplugin-py-0.0.5/openplugin/utils/util.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-25 03:37:58.595393 openplugin-py-0.0.5/openplugin_py.egg-info/
+-rw-r--r--   0 4paradigm   (501) staff       (20)     4113 2023-07-25 03:37:58.000000 openplugin-py-0.0.5/openplugin_py.egg-info/PKG-INFO
+-rw-r--r--   0 4paradigm   (501) staff       (20)      931 2023-07-25 03:37:58.000000 openplugin-py-0.0.5/openplugin_py.egg-info/SOURCES.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)        1 2023-07-25 03:37:58.000000 openplugin-py-0.0.5/openplugin_py.egg-info/dependency_links.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)       46 2023-07-25 03:37:58.000000 openplugin-py-0.0.5/openplugin_py.egg-info/entry_points.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)      167 2023-07-25 03:37:58.000000 openplugin-py-0.0.5/openplugin_py.egg-info/requires.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)       11 2023-07-25 03:37:58.000000 openplugin-py-0.0.5/openplugin_py.egg-info/top_level.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)       38 2023-07-25 03:37:58.595754 openplugin-py-0.0.5/setup.cfg
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2869 2023-06-30 09:40:35.000000 openplugin-py-0.0.5/setup.py
```

### Comparing `openplugin-py-0.0.4/LICENSE` & `openplugin-py-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `openplugin-py-0.0.4/PKG-INFO` & `openplugin-py-0.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openplugin-py
-Version: 0.0.4
+Version: 0.0.5
 Summary: Toolkit and Collection for Plugins of Large Language Models
 Home-page: https://github.com/OpenRL-Lab/openplugin
 Author: openrl contributors
 Author-email: huangsy1314@163.com
 Project-URL: Code, https://github.com/OpenRL-Lab/openplugin
 Project-URL: Documentation, https://openplugin.readthedocs.io/
 Keywords: LLM plugin toolkit
@@ -28,14 +28,15 @@
 
 [![PyPI](https://img.shields.io/pypi/v/openplugin-py)](https://pypi.org/project/openplugin-py/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/openplugin-py)
 [![Hits-of-Code](https://hitsofcode.com/github/OpenRL-Lab/OpenPlugin?branch=main)](https://hitsofcode.com/github/OpenRL-Lab/OpenPlugin/view?branch=main)
 
 [![Documentation Status](https://readthedocs.org/projects/openplugin/badge/?version=latest)](https://openplugin.readthedocs.io/en/latest/?badge=latest)
 
+[[demo video](https://youtu.be/QByu8i9zO04)] | [[bilibili video](https://www.bilibili.com/video/BV1AM4y1s7Qu)]
 
 Toolkit for managing plugins of Large Language Model (LLM). You can install, uninstall, run and list plugins with `op`.
 
 ## Installation
 
 - `pip install openplugin-py` (or clone this repo and `pip install -e .`).
 
@@ -45,25 +46,27 @@
 We provide plugins in [Plugin Store](https://openrl.net/plugin-store/). Users can download these plugins and use them with `op`.
 
 ## Usage
 
 - Check OpenPlugin's version with: `op --version`
 - Check system information: `op --system_info`
 - Install a plugin: `op install <plugin_name>`. You can also install local plugins with `op install ./`.
+  - You can also install a plugin from a zip file: `op install <zip_file_path>`.
 - Uninstall a plugin: `op uninstall <plugin_name>`
 - Start a plugin: `op run <plugin_name>`. You can use `-p` to specify the port of the plugin. By default, the port is 5003.  You can also run a local plugin with `op run ./`.
 - List installed plugins: `op list`
 - Reinstall plugin: `op reinstall <plugin_name>`
 
 ## An example for using QRcode_plugin
 
 - Install QRcode_plugin: `op install QRcode_plugin`
 - Or You can install QRcode_plugin from local:
   - Go to the directory of QRcode_plugin: `cd plugins/QRcode_plugin`
   - Install QRcode_plugin: `op install ./`
+- Or you can install QRcode_plugin from a zip file: `op install QRcode_plugin.zip`
 - Start QRcode_plugin: `op run QRcode_plugin -p server_port`
 - Or you can start QRcode_plugin from local:
   - Go to the directory of QRcode_plugin: `cd plugins/QRcode_plugin`
   - Start QRcode_plugin: `op run ./ -p server_port`
 - Then you can get the `ai-plugin.json` file via visiting `http://<server_ip>:server_port/ai-plugin.json`
 - You can get the `openaip.yaml` file via visiting `http://<server_ip>:server_port/openaip.yaml`
```

### Comparing `openplugin-py-0.0.4/README.md` & `openplugin-py-0.0.5/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 [![PyPI](https://img.shields.io/pypi/v/openplugin-py)](https://pypi.org/project/openplugin-py/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/openplugin-py)
 [![Hits-of-Code](https://hitsofcode.com/github/OpenRL-Lab/OpenPlugin?branch=main)](https://hitsofcode.com/github/OpenRL-Lab/OpenPlugin/view?branch=main)
 
 [![Documentation Status](https://readthedocs.org/projects/openplugin/badge/?version=latest)](https://openplugin.readthedocs.io/en/latest/?badge=latest)
 
+[[demo video](https://youtu.be/QByu8i9zO04)] | [[bilibili video](https://www.bilibili.com/video/BV1AM4y1s7Qu)]
 
 Toolkit for managing plugins of Large Language Model (LLM). You can install, uninstall, run and list plugins with `op`.
 
 ## Installation
 
 - `pip install openplugin-py` (or clone this repo and `pip install -e .`).
 
@@ -19,25 +20,27 @@
 We provide plugins in [Plugin Store](https://openrl.net/plugin-store/). Users can download these plugins and use them with `op`.
 
 ## Usage
 
 - Check OpenPlugin's version with: `op --version`
 - Check system information: `op --system_info`
 - Install a plugin: `op install <plugin_name>`. You can also install local plugins with `op install ./`.
+  - You can also install a plugin from a zip file: `op install <zip_file_path>`.
 - Uninstall a plugin: `op uninstall <plugin_name>`
 - Start a plugin: `op run <plugin_name>`. You can use `-p` to specify the port of the plugin. By default, the port is 5003.  You can also run a local plugin with `op run ./`.
 - List installed plugins: `op list`
 - Reinstall plugin: `op reinstall <plugin_name>`
 
 ## An example for using QRcode_plugin
 
 - Install QRcode_plugin: `op install QRcode_plugin`
 - Or You can install QRcode_plugin from local:
   - Go to the directory of QRcode_plugin: `cd plugins/QRcode_plugin`
   - Install QRcode_plugin: `op install ./`
+- Or you can install QRcode_plugin from a zip file: `op install QRcode_plugin.zip`
 - Start QRcode_plugin: `op run QRcode_plugin -p server_port`
 - Or you can start QRcode_plugin from local:
   - Go to the directory of QRcode_plugin: `cd plugins/QRcode_plugin`
   - Start QRcode_plugin: `op run ./ -p server_port`
 - Then you can get the `ai-plugin.json` file via visiting `http://<server_ip>:server_port/ai-plugin.json`
 - You can get the `openaip.yaml` file via visiting `http://<server_ip>:server_port/openaip.yaml`
```

### Comparing `openplugin-py-0.0.4/openplugin/__init__.py` & `openplugin-py-0.0.5/openplugin/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """"""
 
 
 __TITLE__ = "openplugin"
-__VERSION__ = "v0.0.4"
+__VERSION__ = "v0.0.5"
 __DESCRIPTION__ = "Toolkit and Collection for Plugins of Large Language Models"
 __AUTHOR__ = "OpenRL Contributors"
 __EMAIL__ = "huangshiyu@4paradigm.com"
 __version__ = __VERSION__
 
 import platform
```

### Comparing `openplugin-py-0.0.4/openplugin/cli/__init__.py` & `openplugin-py-0.0.5/openplugin/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `openplugin-py-0.0.4/openplugin/cli/cli.py` & `openplugin-py-0.0.5/openplugin/cli/cli.py`

 * *Files identical despite different names*

### Comparing `openplugin-py-0.0.4/openplugin/install/__init__.py` & `openplugin-py-0.0.5/openplugin/install/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,27 +18,32 @@
 import io
 import shutil
 import zipfile
 
 import requests
 
 from openplugin.install.local_install import install_local_plugin
+from openplugin.install.zip_install import install_zip_plugin
 from openplugin.utils.util import (
     get_plugin_directory,
     get_plugin_list,
     get_zip_file_url,
 )
 
 
 # import urllib
 def install_plugin(plugin_name: str) -> bool:
     if plugin_name == "./":
         print("Installing current directory as plugin...")
         return install_local_plugin()
 
+    if plugin_name.endswith(".zip"):
+        print("Installing plugin from zip file...")
+        return install_zip_plugin(plugin_name)
+
     plugin_list = get_plugin_list()
     if plugin_name in plugin_list:
         print("Plugin {} already installed!".format(plugin_name))
         return True
 
     print("Installing plugin: {}...".format(plugin_name))
     zip_file_url = get_zip_file_url(plugin_name)
```

### Comparing `openplugin-py-0.0.4/openplugin/install/local_install.py` & `openplugin-py-0.0.5/openplugin/install/local_install.py`

 * *Files identical despite different names*

### Comparing `openplugin-py-0.0.4/openplugin/plugin/__init__.py` & `openplugin-py-0.0.5/openplugin/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `openplugin-py-0.0.4/openplugin/plugin/base_plugin.py` & `openplugin-py-0.0.5/openplugin/plugin/base_plugin.py`

 * *Files identical despite different names*

### Comparing `openplugin-py-0.0.4/openplugin/plugin/webapp_plugin.py` & `openplugin-py-0.0.5/openplugin/plugin/webapp_plugin.py`

 * *Files identical despite different names*

### Comparing `openplugin-py-0.0.4/openplugin/run/__init__.py` & `openplugin-py-0.0.5/openplugin/run/__init__.py`

 * *Files identical despite different names*

### Comparing `openplugin-py-0.0.4/openplugin/run/local_run.py` & `openplugin-py-0.0.5/openplugin/run/local_run.py`

 * *Files identical despite different names*

### Comparing `openplugin-py-0.0.4/openplugin/template/__init__.py` & `openplugin-py-0.0.5/openplugin/template/__init__.py`

 * *Files identical despite different names*

### Comparing `openplugin-py-0.0.4/openplugin/template/base_template.py` & `openplugin-py-0.0.5/openplugin/template/base_template.py`

 * *Files identical despite different names*

### Comparing `openplugin-py-0.0.4/openplugin/template/json_template.py` & `openplugin-py-0.0.5/openplugin/template/json_template.py`

 * *Files identical despite different names*

### Comparing `openplugin-py-0.0.4/openplugin/template/utils.py` & `openplugin-py-0.0.5/openplugin/template/utils.py`

 * *Files identical despite different names*

### Comparing `openplugin-py-0.0.4/openplugin/template/yaml_template.py` & `openplugin-py-0.0.5/openplugin/template/yaml_template.py`

 * *Files identical despite different names*

### Comparing `openplugin-py-0.0.4/openplugin/utils/__init__.py` & `openplugin-py-0.0.5/openplugin/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `openplugin-py-0.0.4/openplugin/utils/app_util.py` & `openplugin-py-0.0.5/openplugin/utils/app_util.py`

 * *Files identical despite different names*

### Comparing `openplugin-py-0.0.4/openplugin/utils/errors.py` & `openplugin-py-0.0.5/openplugin/utils/errors.py`

 * *Files identical despite different names*

### Comparing `openplugin-py-0.0.4/openplugin/utils/local_plugin_utils.py` & `openplugin-py-0.0.5/openplugin/utils/local_plugin_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 # limitations under the License.
 
 """"""
 import json
 from pathlib import Path
 
 
-def check_local_plugin() -> str:
-    info_file = Path("info.json")
+def check_local_plugin(plugin_path:str = "./") -> str:
+    info_file = Path(plugin_path)/"info.json"
+
     assert info_file.exists(), "info.json not found"
-    info_dict = json.load(open("info.json", "r"))
+    info_dict = json.load(open(info_file, "r"))
     assert "plugin_name" in info_dict, "plugin_name not found in info.json"
     plugin_name = info_dict["plugin_name"]
     return plugin_name
```

### Comparing `openplugin-py-0.0.4/openplugin/utils/network_utils.py` & `openplugin-py-0.0.5/openplugin/utils/network_utils.py`

 * *Files identical despite different names*

### Comparing `openplugin-py-0.0.4/openplugin/utils/util.py` & `openplugin-py-0.0.5/openplugin/utils/util.py`

 * *Files identical despite different names*

### Comparing `openplugin-py-0.0.4/openplugin_py.egg-info/PKG-INFO` & `openplugin-py-0.0.5/openplugin_py.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openplugin-py
-Version: 0.0.4
+Version: 0.0.5
 Summary: Toolkit and Collection for Plugins of Large Language Models
 Home-page: https://github.com/OpenRL-Lab/openplugin
 Author: openrl contributors
 Author-email: huangsy1314@163.com
 Project-URL: Code, https://github.com/OpenRL-Lab/openplugin
 Project-URL: Documentation, https://openplugin.readthedocs.io/
 Keywords: LLM plugin toolkit
@@ -28,14 +28,15 @@
 
 [![PyPI](https://img.shields.io/pypi/v/openplugin-py)](https://pypi.org/project/openplugin-py/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/openplugin-py)
 [![Hits-of-Code](https://hitsofcode.com/github/OpenRL-Lab/OpenPlugin?branch=main)](https://hitsofcode.com/github/OpenRL-Lab/OpenPlugin/view?branch=main)
 
 [![Documentation Status](https://readthedocs.org/projects/openplugin/badge/?version=latest)](https://openplugin.readthedocs.io/en/latest/?badge=latest)
 
+[[demo video](https://youtu.be/QByu8i9zO04)] | [[bilibili video](https://www.bilibili.com/video/BV1AM4y1s7Qu)]
 
 Toolkit for managing plugins of Large Language Model (LLM). You can install, uninstall, run and list plugins with `op`.
 
 ## Installation
 
 - `pip install openplugin-py` (or clone this repo and `pip install -e .`).
 
@@ -45,25 +46,27 @@
 We provide plugins in [Plugin Store](https://openrl.net/plugin-store/). Users can download these plugins and use them with `op`.
 
 ## Usage
 
 - Check OpenPlugin's version with: `op --version`
 - Check system information: `op --system_info`
 - Install a plugin: `op install <plugin_name>`. You can also install local plugins with `op install ./`.
+  - You can also install a plugin from a zip file: `op install <zip_file_path>`.
 - Uninstall a plugin: `op uninstall <plugin_name>`
 - Start a plugin: `op run <plugin_name>`. You can use `-p` to specify the port of the plugin. By default, the port is 5003.  You can also run a local plugin with `op run ./`.
 - List installed plugins: `op list`
 - Reinstall plugin: `op reinstall <plugin_name>`
 
 ## An example for using QRcode_plugin
 
 - Install QRcode_plugin: `op install QRcode_plugin`
 - Or You can install QRcode_plugin from local:
   - Go to the directory of QRcode_plugin: `cd plugins/QRcode_plugin`
   - Install QRcode_plugin: `op install ./`
+- Or you can install QRcode_plugin from a zip file: `op install QRcode_plugin.zip`
 - Start QRcode_plugin: `op run QRcode_plugin -p server_port`
 - Or you can start QRcode_plugin from local:
   - Go to the directory of QRcode_plugin: `cd plugins/QRcode_plugin`
   - Start QRcode_plugin: `op run ./ -p server_port`
 - Then you can get the `ai-plugin.json` file via visiting `http://<server_ip>:server_port/ai-plugin.json`
 - You can get the `openaip.yaml` file via visiting `http://<server_ip>:server_port/openaip.yaml`
```

### Comparing `openplugin-py-0.0.4/openplugin_py.egg-info/SOURCES.txt` & `openplugin-py-0.0.5/openplugin_py.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 README.md
 setup.py
 openplugin/__init__.py
 openplugin/cli/__init__.py
 openplugin/cli/cli.py
 openplugin/install/__init__.py
 openplugin/install/local_install.py
+openplugin/install/zip_install.py
 openplugin/plugin/__init__.py
 openplugin/plugin/base_plugin.py
 openplugin/plugin/webapp_plugin.py
 openplugin/run/__init__.py
 openplugin/run/local_run.py
 openplugin/template/__init__.py
 openplugin/template/base_template.py
```

### Comparing `openplugin-py-0.0.4/setup.py` & `openplugin-py-0.0.5/setup.py`

 * *Files identical despite different names*

