# Comparing `tmp/pipen_log2file-0.3.2.tar.gz` & `tmp/pipen_log2file-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipen_log2file-0.3.2.tar", max compression
+gzip compressed data, was "pipen_log2file-0.3.3.tar", max compression
```

## Comparing `pipen_log2file-0.3.2.tar` & `pipen_log2file-0.3.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1063 2023-06-11 00:14:20.381404 pipen_log2file-0.3.2/LICENSE
--rwxr-xr-x   0        0        0      984 2023-06-11 00:14:20.381404 pipen_log2file-0.3.2/README.md
--rwxr-xr-x   0        0        0     6219 2023-06-11 00:14:20.381404 pipen_log2file-0.3.2/pipen_log2file.py
--rwxr-xr-x   0        0        0      892 2023-06-11 00:14:20.381404 pipen_log2file-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     1733 1970-01-01 00:00:00.000000 pipen_log2file-0.3.2/setup.py
--rw-r--r--   0        0        0     1684 1970-01-01 00:00:00.000000 pipen_log2file-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-07-24 21:56:11.759926 pipen_log2file-0.3.3/LICENSE
+-rwxr-xr-x   0        0        0      984 2023-07-24 21:56:11.759926 pipen_log2file-0.3.3/README.md
+-rwxr-xr-x   0        0        0     6239 2023-07-24 21:56:11.759926 pipen_log2file-0.3.3/pipen_log2file.py
+-rwxr-xr-x   0        0        0      915 2023-07-24 21:56:11.759926 pipen_log2file-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     1733 1970-01-01 00:00:00.000000 pipen_log2file-0.3.3/setup.py
+-rw-r--r--   0        0        0     1684 1970-01-01 00:00:00.000000 pipen_log2file-0.3.3/PKG-INFO
```

### Comparing `pipen_log2file-0.3.2/LICENSE` & `pipen_log2file-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pipen_log2file-0.3.2/README.md` & `pipen_log2file-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `pipen_log2file-0.3.2/pipen_log2file.py` & `pipen_log2file-0.3.3/pipen_log2file.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from xqute.utils import logger as xqute_logger
 from pipen import plugin
 
 if TYPE_CHECKING:  # pragma: no cover
     from pipen import Pipen, Proc
     from pipen.job import Job
 
-__version__ = "0.3.2"
+__version__ = "0.3.3"
 
 xqute_logger_handlers = xqute_logger.handlers
 
 
 def _remove_rich_tags(text: str) -> str:
     """Remove rich tags from text"""
     return "".join(text for _, text, _ in _parse(text) if text)
@@ -56,14 +56,15 @@
         record.msg = _remove_rich_tags(record.msg)
         return True
 
 
 class PipenLog2FilePlugin:
     """pipen-log2file plugin: Save running logs to file"""
     name = "log2file"
+    priority = 1000
     __version__: str = __version__
 
     def __init__(self) -> None:
         self._handler: logging.FileHandler | None = None
         self._job_progress: List[str] = []
         self._xqute_handler: logging.Handler | None = None
```

### Comparing `pipen_log2file-0.3.2/pyproject.toml` & `pipen_log2file-0.3.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pipen-log2file"
-version = "0.3.2"
+version = "0.3.3"
 description = "Add verbosal information in logs for pipen."
 authors = ["pwwang <pwwang@pwwang.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/pwwang/pipen-log2file"
 repository = "https://github.com/pwwang/pipen-log2file"
 
@@ -12,14 +12,15 @@
 python = "^3.8"
 pipen = "^0.10.0"
 
 [tool.poetry.build]
 generate-setup-file = true
 
 [tool.poetry.dev-dependencies]
+pipen-args = "^0.10.3"
 pytest = "^7"
 pytest-cov = "^4"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `pipen_log2file-0.3.2/setup.py` & `pipen_log2file-0.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ['pipen>=0.10.0,<0.11.0']
 
 entry_points = \
 {'pipen': ['log2file = pipen_log2file:log2file_plugin']}
 
 setup_kwargs = {
     'name': 'pipen-log2file',
-    'version': '0.3.2',
+    'version': '0.3.3',
     'description': 'Add verbosal information in logs for pipen.',
     'long_description': '# pipen-log2file\n\nSave running logs to file for [pipen][1].\n\nThe log file is saved to `<workdir>/<pipeline>/.logs/run-<date-time>.log` by default.\nA symlink `<workdir>/<pipeline>/run-latest.log` is created to the latest log file.\n\nThe xqute logs are also saved to `<workdir>/<pipeline>/<proc>/proc.xqute.log`\n\nNote that the original handler of xqute logger is removed during pipeline running.\n\n## Options\n\n- `plugin_opts.log2file_xqute`: Whether to save xqute logs. Default: `True`.\n    if False, the xqute logger will be kept intact.\n- `plugin_opts.log2file_xqute_level`: The log level for xqute logger. Default: `INFO`.\n- `plugin_opts.log2file_xqute_append`: Whether to append to the log file. Default: `False`.\n\n## Installation\n\n```\npip install -U pipen-log2file\n```\n\n## Enabling/Disabling the plugin\n\nThe plugin is registered via entrypoints. It\'s by default enabled. To disable it:\n`plugins=[..., "no:log2file"]`, or uninstall this plugin.\n\n\n[1]: https://github.com/pwwang/pipen\n',
     'author': 'pwwang',
     'author_email': 'pwwang@pwwang.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/pwwang/pipen-log2file',
```

### Comparing `pipen_log2file-0.3.2/PKG-INFO` & `pipen_log2file-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipen-log2file
-Version: 0.3.2
+Version: 0.3.3
 Summary: Add verbosal information in logs for pipen.
 Home-page: https://github.com/pwwang/pipen-log2file
 License: MIT
 Author: pwwang
 Author-email: pwwang@pwwang.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

