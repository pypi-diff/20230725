# Comparing `tmp/pytest-mypy-plugins-2.0.0.tar.gz` & `tmp/pytest-mypy-plugins-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-mypy-plugins-2.0.0.tar", last modified: Thu Jun 29 07:14:44 2023, max compression
+gzip compressed data, was "pytest-mypy-plugins-3.0.0.tar", last modified: Tue Jul 25 12:46:50 2023, max compression
```

## Comparing `pytest-mypy-plugins-2.0.0.tar` & `pytest-mypy-plugins-3.0.0.tar`

### file list

```diff
@@ -1,34 +1,49 @@
-drwxr-xr-x   0 sobolev    (501) staff       (20)        0 2023-06-29 07:14:44.534921 pytest-mypy-plugins-2.0.0/
--rw-r--r--   0 sobolev    (501) staff       (20)     1054 2023-06-29 06:58:38.000000 pytest-mypy-plugins-2.0.0/LICENSE
--rw-r--r--   0 sobolev    (501) staff       (20)       68 2023-06-29 06:58:38.000000 pytest-mypy-plugins-2.0.0/MANIFEST.in
--rw-r--r--   0 sobolev    (501) staff       (20)     8316 2023-06-29 07:14:44.534748 pytest-mypy-plugins-2.0.0/PKG-INFO
--rw-r--r--   0 sobolev    (501) staff       (20)     7535 2023-06-29 07:14:33.000000 pytest-mypy-plugins-2.0.0/README.md
--rw-r--r--   0 sobolev    (501) staff       (20)      313 2023-06-29 06:58:38.000000 pytest-mypy-plugins-2.0.0/mypy.ini
--rw-r--r--   0 sobolev    (501) staff       (20)      115 2023-06-29 06:58:38.000000 pytest-mypy-plugins-2.0.0/pyproject.toml
--rw-r--r--   0 sobolev    (501) staff       (20)      125 2023-06-29 06:58:38.000000 pytest-mypy-plugins-2.0.0/pytest.ini
-drwxr-xr-x   0 sobolev    (501) staff       (20)        0 2023-06-29 07:14:44.532066 pytest-mypy-plugins-2.0.0/pytest_mypy_plugins/
--rw-r--r--   0 sobolev    (501) staff       (20)        0 2023-06-29 06:58:38.000000 pytest-mypy-plugins-2.0.0/pytest_mypy_plugins/__init__.py
--rw-r--r--   0 sobolev    (501) staff       (20)     7257 2023-06-29 07:14:33.000000 pytest-mypy-plugins-2.0.0/pytest_mypy_plugins/collect.py
--rw-r--r--   0 sobolev    (501) staff       (20)    14684 2023-06-29 06:58:38.000000 pytest-mypy-plugins-2.0.0/pytest_mypy_plugins/item.py
--rw-r--r--   0 sobolev    (501) staff       (20)        0 2023-06-29 06:58:38.000000 pytest-mypy-plugins-2.0.0/pytest_mypy_plugins/py.typed
-drwxr-xr-x   0 sobolev    (501) staff       (20)        0 2023-06-29 07:14:44.533996 pytest-mypy-plugins-2.0.0/pytest_mypy_plugins/tests/
-drwxr-xr-x   0 sobolev    (501) staff       (20)        0 2023-06-29 07:14:44.534409 pytest-mypy-plugins-2.0.0/pytest_mypy_plugins/tests/__pycache__/
--rw-r--r--   0 sobolev    (501) staff       (20)      824 2023-06-29 07:07:03.000000 pytest-mypy-plugins-2.0.0/pytest_mypy_plugins/tests/__pycache__/reveal_type_hook.cpython-311.pyc
--rw-r--r--   0 sobolev    (501) staff       (20)    11558 2023-06-29 07:07:03.000000 pytest-mypy-plugins-2.0.0/pytest_mypy_plugins/tests/__pycache__/test_utils.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0 sobolev    (501) staff       (20)      354 2023-06-29 06:58:38.000000 pytest-mypy-plugins-2.0.0/pytest_mypy_plugins/tests/reveal_type_hook.py
--rw-r--r--   0 sobolev    (501) staff       (20)      183 2023-06-29 06:58:38.000000 pytest-mypy-plugins-2.0.0/pytest_mypy_plugins/tests/test-extension.yml
--rw-r--r--   0 sobolev    (501) staff       (20)     1242 2023-06-29 07:14:33.000000 pytest-mypy-plugins-2.0.0/pytest_mypy_plugins/tests/test-parametrized.yml
--rw-r--r--   0 sobolev    (501) staff       (20)      338 2023-06-29 06:58:38.000000 pytest-mypy-plugins-2.0.0/pytest_mypy_plugins/tests/test-paths-from-env.yml
--rw-r--r--   0 sobolev    (501) staff       (20)     1179 2023-06-29 06:58:38.000000 pytest-mypy-plugins-2.0.0/pytest_mypy_plugins/tests/test-regex_assertions.yml
--rw-r--r--   0 sobolev    (501) staff       (20)     1987 2023-06-29 06:58:38.000000 pytest-mypy-plugins-2.0.0/pytest_mypy_plugins/tests/test-simple-cases.yml
--rw-r--r--   0 sobolev    (501) staff       (20)     8631 2023-06-29 06:58:38.000000 pytest-mypy-plugins-2.0.0/pytest_mypy_plugins/tests/test_utils.py
--rw-r--r--   0 sobolev    (501) staff       (20)    12670 2023-06-29 06:58:38.000000 pytest-mypy-plugins-2.0.0/pytest_mypy_plugins/utils.py
-drwxr-xr-x   0 sobolev    (501) staff       (20)        0 2023-06-29 07:14:44.532972 pytest-mypy-plugins-2.0.0/pytest_mypy_plugins.egg-info/
--rw-r--r--   0 sobolev    (501) staff       (20)     8316 2023-06-29 07:14:44.000000 pytest-mypy-plugins-2.0.0/pytest_mypy_plugins.egg-info/PKG-INFO
--rw-r--r--   0 sobolev    (501) staff       (20)      960 2023-06-29 07:14:44.000000 pytest-mypy-plugins-2.0.0/pytest_mypy_plugins.egg-info/SOURCES.txt
--rw-r--r--   0 sobolev    (501) staff       (20)        1 2023-06-29 07:14:44.000000 pytest-mypy-plugins-2.0.0/pytest_mypy_plugins.egg-info/dependency_links.txt
--rw-r--r--   0 sobolev    (501) staff       (20)       61 2023-06-29 07:14:44.000000 pytest-mypy-plugins-2.0.0/pytest_mypy_plugins.egg-info/entry_points.txt
--rw-r--r--   0 sobolev    (501) staff       (20)       64 2023-06-29 07:14:44.000000 pytest-mypy-plugins-2.0.0/pytest_mypy_plugins.egg-info/requires.txt
--rw-r--r--   0 sobolev    (501) staff       (20)       20 2023-06-29 07:14:44.000000 pytest-mypy-plugins-2.0.0/pytest_mypy_plugins.egg-info/top_level.txt
--rw-r--r--   0 sobolev    (501) staff       (20)       38 2023-06-29 07:14:44.534968 pytest-mypy-plugins-2.0.0/setup.cfg
--rw-r--r--   0 sobolev    (501) staff       (20)     1365 2023-06-29 07:14:33.000000 pytest-mypy-plugins-2.0.0/setup.py
+drwxr-xr-x   0 sobolev    (501) staff       (20)        0 2023-07-25 12:46:50.790980 pytest-mypy-plugins-3.0.0/
+-rw-r--r--   0 sobolev    (501) staff       (20)     1054 2023-07-19 10:57:48.000000 pytest-mypy-plugins-3.0.0/LICENSE
+-rw-r--r--   0 sobolev    (501) staff       (20)       96 2023-07-25 12:45:42.000000 pytest-mypy-plugins-3.0.0/MANIFEST.in
+-rw-r--r--   0 sobolev    (501) staff       (20)     8826 2023-07-25 12:46:50.790802 pytest-mypy-plugins-3.0.0/PKG-INFO
+-rw-r--r--   0 sobolev    (501) staff       (20)     8047 2023-07-25 12:45:42.000000 pytest-mypy-plugins-3.0.0/README.md
+-rw-r--r--   0 sobolev    (501) staff       (20)      609 2023-07-25 12:45:42.000000 pytest-mypy-plugins-3.0.0/pyproject.toml
+drwxr-xr-x   0 sobolev    (501) staff       (20)        0 2023-07-25 12:46:50.785227 pytest-mypy-plugins-3.0.0/pytest_mypy_plugins/
+-rw-r--r--   0 sobolev    (501) staff       (20)        0 2023-07-19 10:57:48.000000 pytest-mypy-plugins-3.0.0/pytest_mypy_plugins/__init__.py
+-rw-r--r--   0 sobolev    (501) staff       (20)     7503 2023-07-25 12:45:42.000000 pytest-mypy-plugins-3.0.0/pytest_mypy_plugins/collect.py
+-rw-r--r--   0 sobolev    (501) staff       (20)     2361 2023-07-25 12:45:42.000000 pytest-mypy-plugins-3.0.0/pytest_mypy_plugins/configs.py
+-rw-r--r--   0 sobolev    (501) staff       (20)    15460 2023-07-25 12:45:42.000000 pytest-mypy-plugins-3.0.0/pytest_mypy_plugins/item.py
+-rw-r--r--   0 sobolev    (501) staff       (20)        0 2023-07-19 10:57:48.000000 pytest-mypy-plugins-3.0.0/pytest_mypy_plugins/py.typed
+drwxr-xr-x   0 sobolev    (501) staff       (20)        0 2023-07-25 12:46:50.787534 pytest-mypy-plugins-3.0.0/pytest_mypy_plugins/tests/
+drwxr-xr-x   0 sobolev    (501) staff       (20)        0 2023-07-25 12:46:50.788288 pytest-mypy-plugins-3.0.0/pytest_mypy_plugins/tests/__pycache__/
+-rw-r--r--   0 sobolev    (501) staff       (20)      824 2023-07-19 11:08:19.000000 pytest-mypy-plugins-3.0.0/pytest_mypy_plugins/tests/__pycache__/reveal_type_hook.cpython-311.pyc
+-rw-r--r--   0 sobolev    (501) staff       (20)     2472 2023-07-25 12:29:54.000000 pytest-mypy-plugins-3.0.0/pytest_mypy_plugins/tests/__pycache__/test_explicit_configs.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0 sobolev    (501) staff       (20)    11558 2023-07-19 11:08:19.000000 pytest-mypy-plugins-3.0.0/pytest_mypy_plugins/tests/__pycache__/test_utils.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0 sobolev    (501) staff       (20)      354 2023-07-19 10:57:48.000000 pytest-mypy-plugins-3.0.0/pytest_mypy_plugins/tests/reveal_type_hook.py
+-rw-r--r--   0 sobolev    (501) staff       (20)      183 2023-07-19 10:57:48.000000 pytest-mypy-plugins-3.0.0/pytest_mypy_plugins/tests/test-extension.yml
+-rw-r--r--   0 sobolev    (501) staff       (20)      249 2023-07-25 12:45:42.000000 pytest-mypy-plugins-3.0.0/pytest_mypy_plugins/tests/test-mypy-config.yml
+-rw-r--r--   0 sobolev    (501) staff       (20)     1242 2023-07-19 10:57:48.000000 pytest-mypy-plugins-3.0.0/pytest_mypy_plugins/tests/test-parametrized.yml
+-rw-r--r--   0 sobolev    (501) staff       (20)      338 2023-07-19 10:57:48.000000 pytest-mypy-plugins-3.0.0/pytest_mypy_plugins/tests/test-paths-from-env.yml
+-rw-r--r--   0 sobolev    (501) staff       (20)     1179 2023-07-19 10:57:48.000000 pytest-mypy-plugins-3.0.0/pytest_mypy_plugins/tests/test-regex_assertions.yml
+-rw-r--r--   0 sobolev    (501) staff       (20)     1809 2023-07-25 12:45:42.000000 pytest-mypy-plugins-3.0.0/pytest_mypy_plugins/tests/test-simple-cases.yml
+drwxr-xr-x   0 sobolev    (501) staff       (20)        0 2023-07-25 12:46:50.789847 pytest-mypy-plugins-3.0.0/pytest_mypy_plugins/tests/test_configs/
+drwxr-xr-x   0 sobolev    (501) staff       (20)        0 2023-07-25 12:46:50.790390 pytest-mypy-plugins-3.0.0/pytest_mypy_plugins/tests/test_configs/__pycache__/
+-rw-r--r--   0 sobolev    (501) staff       (20)      424 2023-07-19 11:59:29.000000 pytest-mypy-plugins-3.0.0/pytest_mypy_plugins/tests/test_configs/__pycache__/test_join_files.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0 sobolev    (501) staff       (20)     5785 2023-07-25 12:29:54.000000 pytest-mypy-plugins-3.0.0/pytest_mypy_plugins/tests/test_configs/__pycache__/test_join_toml_configs.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0 sobolev    (501) staff       (20)       29 2023-07-25 12:45:42.000000 pytest-mypy-plugins-3.0.0/pytest_mypy_plugins/tests/test_configs/mypy1.ini
+-rw-r--r--   0 sobolev    (501) staff       (20)        8 2023-07-25 12:45:42.000000 pytest-mypy-plugins-3.0.0/pytest_mypy_plugins/tests/test_configs/mypy2.ini
+-rw-r--r--   0 sobolev    (501) staff       (20)      189 2023-07-25 12:45:42.000000 pytest-mypy-plugins-3.0.0/pytest_mypy_plugins/tests/test_configs/pyproject1.toml
+-rw-r--r--   0 sobolev    (501) staff       (20)       49 2023-07-25 12:45:42.000000 pytest-mypy-plugins-3.0.0/pytest_mypy_plugins/tests/test_configs/pyproject2.toml
+-rw-r--r--   0 sobolev    (501) staff       (20)       29 2023-07-25 12:45:42.000000 pytest-mypy-plugins-3.0.0/pytest_mypy_plugins/tests/test_configs/setup1.cfg
+-rw-r--r--   0 sobolev    (501) staff       (20)        8 2023-07-25 12:45:42.000000 pytest-mypy-plugins-3.0.0/pytest_mypy_plugins/tests/test_configs/setup2.cfg
+-rw-r--r--   0 sobolev    (501) staff       (20)     2769 2023-07-25 12:45:42.000000 pytest-mypy-plugins-3.0.0/pytest_mypy_plugins/tests/test_configs/test_join_toml_configs.py
+-rw-r--r--   0 sobolev    (501) staff       (20)     1271 2023-07-25 12:45:42.000000 pytest-mypy-plugins-3.0.0/pytest_mypy_plugins/tests/test_explicit_configs.py
+-rw-r--r--   0 sobolev    (501) staff       (20)     8631 2023-07-19 10:57:48.000000 pytest-mypy-plugins-3.0.0/pytest_mypy_plugins/tests/test_utils.py
+-rw-r--r--   0 sobolev    (501) staff       (20)    12282 2023-07-25 12:45:42.000000 pytest-mypy-plugins-3.0.0/pytest_mypy_plugins/utils.py
+drwxr-xr-x   0 sobolev    (501) staff       (20)        0 2023-07-25 12:46:50.786044 pytest-mypy-plugins-3.0.0/pytest_mypy_plugins.egg-info/
+-rw-r--r--   0 sobolev    (501) staff       (20)     8826 2023-07-25 12:46:50.000000 pytest-mypy-plugins-3.0.0/pytest_mypy_plugins.egg-info/PKG-INFO
+-rw-r--r--   0 sobolev    (501) staff       (20)     1755 2023-07-25 12:46:50.000000 pytest-mypy-plugins-3.0.0/pytest_mypy_plugins.egg-info/SOURCES.txt
+-rw-r--r--   0 sobolev    (501) staff       (20)        1 2023-07-25 12:46:50.000000 pytest-mypy-plugins-3.0.0/pytest_mypy_plugins.egg-info/dependency_links.txt
+-rw-r--r--   0 sobolev    (501) staff       (20)       61 2023-07-25 12:46:50.000000 pytest-mypy-plugins-3.0.0/pytest_mypy_plugins.egg-info/entry_points.txt
+-rw-r--r--   0 sobolev    (501) staff       (20)       78 2023-07-25 12:46:50.000000 pytest-mypy-plugins-3.0.0/pytest_mypy_plugins.egg-info/requires.txt
+-rw-r--r--   0 sobolev    (501) staff       (20)       20 2023-07-25 12:46:50.000000 pytest-mypy-plugins-3.0.0/pytest_mypy_plugins.egg-info/top_level.txt
+-rw-r--r--   0 sobolev    (501) staff       (20)       63 2023-07-19 10:57:48.000000 pytest-mypy-plugins-3.0.0/requirements.txt
+-rw-r--r--   0 sobolev    (501) staff       (20)       38 2023-07-25 12:46:50.791033 pytest-mypy-plugins-3.0.0/setup.cfg
+-rw-r--r--   0 sobolev    (501) staff       (20)     1379 2023-07-25 12:45:42.000000 pytest-mypy-plugins-3.0.0/setup.py
+-rw-r--r--   0 sobolev    (501) staff       (20)       82 2023-07-19 10:57:48.000000 pytest-mypy-plugins-3.0.0/tox.ini
```

### Comparing `pytest-mypy-plugins-2.0.0/LICENSE` & `pytest-mypy-plugins-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-mypy-plugins-2.0.0/PKG-INFO` & `pytest-mypy-plugins-3.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: pytest-mypy-plugins
-Version: 2.0.0
+Version: 3.0.0
 Summary: pytest plugin for writing tests for mypy plugins
 Home-page: https://github.com/TypedDjango/pytest-mypy-plugins
 Author: Maksim Kurnikov
 Author-email: maxim.kurnikov@gmail.com
 Maintainer: Nikita Sobolev
 Maintainer-email: mail@sobolevn.me
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <img src="http://mypy-lang.org/static/mypy_light.svg" alt="mypy logo" width="300px"/>
 
 # pytest plugin for testing mypy types, stubs, and plugins
 
@@ -86,15 +86,15 @@
 
 | Property        | Type                                                   | Description                                                                                                         |
 | --------------- | ------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------- |
 | `case`          | `str`                                                  | Name of the test case, complies to `[a-zA-Z0-9]` pattern                                                            |
 | `main`          | `str`                                                  | Portion of the code as if written in `.py` file                                                                     |
 | `files`         | `Optional[List[File]]=[]`\*                            | List of extra files to simulate imports if needed                                                                   |
 | `disable_cache` | `Optional[bool]=False`                                 | Set to `true` disables `mypy` caching                                                                               |
-| `mypy_config`   | `Optional[Dict[str, Union[str, int, bool, float]]]={}` | Inline `mypy` configuration, passed directly to `mypy` as `--config-file` option                                    |
+| `mypy_config`   | `Optional[Dict[str, Union[str, int, bool, float]]]={}` | Inline `mypy` configuration, passed directly to `mypy` as `--config-file` option, possibly joined with `--mypy-pyproject-toml-file` or `--mypy-ini-file` contents if they are passed. By default is treated as `ini`, treated as `toml` only if `--mypy-pyproject-toml-file` is passed |
 | `env`           | `Optional[Dict[str, str]]={}`                          | Environmental variables to be provided inside of test run                                                           |
 | `parametrized`  | `Optional[List[Parameter]]=[]`\*                       | List of parameters, similar to [`@pytest.mark.parametrize`](https://docs.pytest.org/en/stable/parametrize.html)     |
 | `skip`          | `str`                                                  | Expression evaluated with following globals set: `sys`, `os`, `pytest` and `platform`                               |
 | `expect_fail`   | `bool`                                                 | Mark test case as an expected failure, like [`@pytest.mark.xfail`](https://docs.pytest.org/en/stable/skipping.html) |
 | `regex`         | `str`                                                  | Allow regular expressions in comments to be matched against actual output. Defaults to "no", i.e. matches full text.|
 
 (*) Appendix to **pseudo** types used above:
@@ -188,19 +188,26 @@
 
 ## Options
 
 ```
 mypy-tests:
   --mypy-testing-base=MYPY_TESTING_BASE
                         Base directory for tests to use
+  --mypy-pyproject-toml-file=MYPY_PYPROJECT_TOML_FILE
+                        Which `pyproject.toml` file to use
+                        as a default config for tests.
+                        Incompatible with `--mypy-ini-file`
   --mypy-ini-file=MYPY_INI_FILE
-                        Which .ini file to use as a default config for tests
-  --mypy-same-process   Run in the same process. Useful for debugging, will create problems with import cache
+                        Which `.ini` file to use as a default config for tests.
+                        Incompatible with `--mypy-pyproject-toml-file`
+  --mypy-same-process   Run in the same process. Useful for debugging,
+                        will create problems with import cache
   --mypy-extension-hook=MYPY_EXTENSION_HOOK
-                        Fully qualified path to the extension hook function, in case you need custom yaml keys. Has to be top-level.
+                        Fully qualified path to the extension hook function,
+                        in case you need custom yaml keys. Has to be top-level
   --mypy-only-local-stub
                         mypy will ignore errors from site-packages
 
 ```
 
 ## Further reading
```

### Comparing `pytest-mypy-plugins-2.0.0/README.md` & `pytest-mypy-plugins-3.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
 | Property        | Type                                                   | Description                                                                                                         |
 | --------------- | ------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------- |
 | `case`          | `str`                                                  | Name of the test case, complies to `[a-zA-Z0-9]` pattern                                                            |
 | `main`          | `str`                                                  | Portion of the code as if written in `.py` file                                                                     |
 | `files`         | `Optional[List[File]]=[]`\*                            | List of extra files to simulate imports if needed                                                                   |
 | `disable_cache` | `Optional[bool]=False`                                 | Set to `true` disables `mypy` caching                                                                               |
-| `mypy_config`   | `Optional[Dict[str, Union[str, int, bool, float]]]={}` | Inline `mypy` configuration, passed directly to `mypy` as `--config-file` option                                    |
+| `mypy_config`   | `Optional[Dict[str, Union[str, int, bool, float]]]={}` | Inline `mypy` configuration, passed directly to `mypy` as `--config-file` option, possibly joined with `--mypy-pyproject-toml-file` or `--mypy-ini-file` contents if they are passed. By default is treated as `ini`, treated as `toml` only if `--mypy-pyproject-toml-file` is passed |
 | `env`           | `Optional[Dict[str, str]]={}`                          | Environmental variables to be provided inside of test run                                                           |
 | `parametrized`  | `Optional[List[Parameter]]=[]`\*                       | List of parameters, similar to [`@pytest.mark.parametrize`](https://docs.pytest.org/en/stable/parametrize.html)     |
 | `skip`          | `str`                                                  | Expression evaluated with following globals set: `sys`, `os`, `pytest` and `platform`                               |
 | `expect_fail`   | `bool`                                                 | Mark test case as an expected failure, like [`@pytest.mark.xfail`](https://docs.pytest.org/en/stable/skipping.html) |
 | `regex`         | `str`                                                  | Allow regular expressions in comments to be matched against actual output. Defaults to "no", i.e. matches full text.|
 
 (*) Appendix to **pseudo** types used above:
@@ -166,19 +166,26 @@
 
 ## Options
 
 ```
 mypy-tests:
   --mypy-testing-base=MYPY_TESTING_BASE
                         Base directory for tests to use
+  --mypy-pyproject-toml-file=MYPY_PYPROJECT_TOML_FILE
+                        Which `pyproject.toml` file to use
+                        as a default config for tests.
+                        Incompatible with `--mypy-ini-file`
   --mypy-ini-file=MYPY_INI_FILE
-                        Which .ini file to use as a default config for tests
-  --mypy-same-process   Run in the same process. Useful for debugging, will create problems with import cache
+                        Which `.ini` file to use as a default config for tests.
+                        Incompatible with `--mypy-pyproject-toml-file`
+  --mypy-same-process   Run in the same process. Useful for debugging,
+                        will create problems with import cache
   --mypy-extension-hook=MYPY_EXTENSION_HOOK
-                        Fully qualified path to the extension hook function, in case you need custom yaml keys. Has to be top-level.
+                        Fully qualified path to the extension hook function,
+                        in case you need custom yaml keys. Has to be top-level
   --mypy-only-local-stub
                         mypy will ignore errors from site-packages
 
 ```
 
 ## Further reading
```

### Comparing `pytest-mypy-plugins-2.0.0/pytest_mypy_plugins/collect.py` & `pytest-mypy-plugins-3.0.0/pytest_mypy_plugins/collect.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 import pathlib
 import platform
 import sys
 import tempfile
+from dataclasses import dataclass
 from typing import (
     TYPE_CHECKING,
     Any,
     Dict,
     Hashable,
     Iterator,
     List,
@@ -24,18 +25,18 @@
 
 from pytest_mypy_plugins import utils
 
 if TYPE_CHECKING:
     from pytest_mypy_plugins.item import YamlTestItem
 
 
+@dataclass
 class File:
-    def __init__(self, path: str, content: str) -> None:
-        self.path = path
-        self.content = content
+    path: str
+    content: str
 
 
 def parse_test_files(test_files: List[Dict[str, Any]]) -> List[File]:
     files: List[File] = []
     for test_file in test_files:
         path = test_file.get("path", "main.py")
         file = File(path=path, content=test_file.get("content", ""))
@@ -73,15 +74,15 @@
 
 
 class SafeLineLoader(yaml.SafeLoader):
     def construct_mapping(self, node: yaml.MappingNode, deep: bool = False) -> Dict[Hashable, Any]:
         mapping = super().construct_mapping(node, deep=deep)
         # Add 1 so line numbering starts at 1
         starting_line = node.start_mark.line + 1
-        for title_node, contents_node in node.value:
+        for title_node, _contents_node in node.value:
             if title_node.value == "main":
                 starting_line = title_node.start_mark.line + 1
         mapping["__line__"] = starting_line
         return mapping
 
 
 class YamlTestFile(pytest.File):
@@ -168,15 +169,24 @@
 
 
 def pytest_addoption(parser: Parser) -> None:
     group = parser.getgroup("mypy-tests")
     group.addoption(
         "--mypy-testing-base", type=str, default=tempfile.gettempdir(), help="Base directory for tests to use"
     )
-    group.addoption("--mypy-ini-file", type=str, help="Which .ini file to use as a default config for tests")
+    group.addoption(
+        "--mypy-pyproject-toml-file",
+        type=str,
+        help="Which `pyproject.toml` file to use as a default config for tests. Incompatible with `--mypy-ini-file`",
+    )
+    group.addoption(
+        "--mypy-ini-file",
+        type=str,
+        help="Which `.ini` file to use as a default config for tests. Incompatible with `--mypy-pyproject-toml-file`",
+    )
     group.addoption(
         "--mypy-same-process",
         action="store_true",
         help="Run in the same process. Useful for debugging, will create problems with import cache",
     )
     group.addoption(
         "--mypy-extension-hook",
```

### Comparing `pytest-mypy-plugins-2.0.0/pytest_mypy_plugins/item.py` & `pytest-mypy-plugins-3.0.0/pytest_mypy_plugins/item.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,35 @@
 import importlib
+import io
 import os
 import subprocess
 import sys
 import tempfile
-from configparser import ConfigParser
 from pathlib import Path
-from typing import (
-    TYPE_CHECKING,
-    Any,
-    Callable,
-    Dict,
-    List,
-    Optional,
-    Tuple,
-    Union,
-    no_type_check,
-)
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, TextIO, Tuple, Union
 
 import py
 import pytest
 from _pytest._code import ExceptionInfo
 from _pytest._code.code import ReprEntry, ReprFileLocation, TerminalRepr
 from _pytest._io import TerminalWriter
 from _pytest.config import Config
 from mypy import build
 from mypy.fscache import FileSystemCache
 from mypy.main import process_options
 
 if TYPE_CHECKING:
     from _pytest._code.code import _TracebackStyle
 
-from pytest_mypy_plugins import utils
+from pytest_mypy_plugins import configs, utils
 from pytest_mypy_plugins.collect import File, YamlTestFile
 from pytest_mypy_plugins.utils import (
     OutputMatcher,
     TypecheckAssertionError,
     assert_expected_matched_actual,
-    capture_std_streams,
     fname_to_module,
 )
 
 
 class TraceLastReprEntry(ReprEntry):
     def toterminal(self, tw: TerminalWriter) -> None:
         if not self.reprfileloc:
@@ -83,32 +72,32 @@
 
 class ReturnCodes:
     SUCCESS = 0
     FAIL = 1
     FATAL_ERROR = 2
 
 
-def run_mypy_typechecking(cmd_options: List[str]) -> Optional[Union[str, int]]:
+def run_mypy_typechecking(cmd_options: List[str], stdout: TextIO, stderr: TextIO) -> Optional[Union[str, int]]:
     fscache = FileSystemCache()
     sources, options = process_options(cmd_options, fscache=fscache)
 
     error_messages = []
 
     def flush_errors(new_messages: List[str], serious: bool) -> None:
         error_messages.extend(new_messages)
-        f = sys.stderr if serious else sys.stdout
+        f = stderr if serious else stdout
         try:
             for msg in new_messages:
                 f.write(msg + "\n")
             f.flush()
         except BrokenPipeError:
             sys.exit(ReturnCodes.FATAL_ERROR)
 
     try:
-        build.build(sources, options, flush_errors=flush_errors, fscache=fscache)
+        build.build(sources, options, flush_errors=flush_errors, fscache=fscache, stdout=stdout, stderr=stderr)
 
     except SystemExit as sysexit:
         return sysexit.code
     finally:
         fscache.flush()
 
     if error_messages:
@@ -143,18 +132,27 @@
         self.additional_mypy_config = mypy_config
         self.parsed_test_data = parsed_test_data
         self.same_process = self.config.option.mypy_same_process
         self.test_only_local_stub = self.config.option.mypy_only_local_stub
 
         # config parameters
         self.root_directory = self.config.option.mypy_testing_base
+
+        # You cannot use both `.ini` and `pyproject.toml` files at the same time:
+        if self.config.option.mypy_ini_file and self.config.option.mypy_pyproject_toml_file:
+            raise ValueError("Cannot specify both `--mypy-ini-file` and `--mypy-pyproject-toml-file`")
+
         if self.config.option.mypy_ini_file:
             self.base_ini_fpath = os.path.abspath(self.config.option.mypy_ini_file)
         else:
             self.base_ini_fpath = None
+        if self.config.option.mypy_pyproject_toml_file:
+            self.base_pyproject_toml_fpath = os.path.abspath(self.config.option.mypy_pyproject_toml_file)
+        else:
+            self.base_pyproject_toml_fpath = None
         self.incremental_cache_dir = os.path.join(self.root_directory, ".mypy_cache")
 
     def make_test_file(self, file: File) -> None:
         current_directory = Path.cwd()
         fpath = current_directory / file.path
         fpath.parent.mkdir(parents=True, exist_ok=True)
         fpath.write_text(file.content)
@@ -200,16 +198,15 @@
 
         # Windows requires this to be set, otherwise the interpreter crashes
         if "SYSTEMROOT" in os.environ:
             self.environment_variables["SYSTEMROOT"] = os.environ["SYSTEMROOT"]
 
         completed = subprocess.run(
             [mypy_executable, *mypy_cmd_options],
-            stdout=subprocess.PIPE,
-            stderr=subprocess.PIPE,
+            capture_output=True,
             cwd=os.getcwd(),
             env=self.environment_variables,
         )
         captured_stdout = completed.stdout.decode()
         captured_stderr = completed.stderr.decode()
         return completed.returncode, (captured_stdout, captured_stderr)
 
@@ -220,18 +217,23 @@
             # add custom environment variables
             for key, val in self.environment_variables.items():
                 os.environ[key] = val
 
             # add current directory to path
             sys.path.insert(0, str(execution_path))
 
-            with capture_std_streams() as (stdout, stderr):
-                return_code = run_mypy_typechecking(mypy_cmd_options)
+            stdout = io.StringIO()
+            stderr = io.StringIO()
+
+            with stdout, stderr:
+                return_code = run_mypy_typechecking(mypy_cmd_options, stdout=stdout, stderr=stderr)
+                stdout_value = stdout.getvalue()
+                stderr_value = stderr.getvalue()
 
-            return return_code, (stdout.getvalue(), stderr.getvalue())
+            return return_code, (stdout_value, stderr_value)
 
     def execute_extension_hook(self) -> None:
         extension_hook_fqname = self.config.option.mypy_extension_hook
         module_name, func_name = extension_hook_fqname.rsplit(".", maxsplit=1)
         module = importlib.import_module(module_name)
         extension_hook = getattr(module, func_name)
         extension_hook(self)
@@ -305,33 +307,35 @@
             "--hide-error-context",
         ]
         if not self.test_only_local_stub:
             mypy_cmd_options.append("--no-silence-site-packages")
         if not self.disable_cache:
             mypy_cmd_options.extend(["--cache-dir", self.incremental_cache_dir])
 
-        # Merge `self.base_ini_fpath` and `self.additional_mypy_config`
-        # into one file and copy to the typechecking folder:
-        mypy_ini_config = ConfigParser()
-        if self.base_ini_fpath:
-            mypy_ini_config.read(self.base_ini_fpath)
-        if self.additional_mypy_config:
-            additional_config = self.additional_mypy_config
-            if "[mypy]" not in additional_config:
-                additional_config = "[mypy]\n" + additional_config
-            mypy_ini_config.read_string(additional_config)
-
-        if mypy_ini_config.sections():
-            mypy_config_file_path = execution_path / "mypy.ini"
-            with mypy_config_file_path.open("w") as f:
-                mypy_ini_config.write(f)
-            mypy_cmd_options.append(f"--config-file={str(mypy_config_file_path)}")
+        config_file = self.prepare_config_file(execution_path)
+        if config_file:
+            mypy_cmd_options.append(f"--config-file={config_file}")
 
         return mypy_cmd_options
 
+    def prepare_config_file(self, execution_path: Path) -> Optional[str]:
+        # Merge (`self.base_ini_fpath` or `base_pyproject_toml_fpath`)
+        # and `self.additional_mypy_config`
+        # into one file and copy to the typechecking folder:
+        if self.base_pyproject_toml_fpath:
+            return configs.join_toml_configs(
+                self.base_pyproject_toml_fpath, self.additional_mypy_config, execution_path
+            )
+        elif self.base_ini_fpath or self.additional_mypy_config:
+            # We might have `self.base_ini_fpath` set as well.
+            # Or this might be a legacy case: only `mypy_config:` is set in the `yaml` test case.
+            # This means that no real file is provided.
+            return configs.join_ini_configs(self.base_ini_fpath, self.additional_mypy_config, execution_path)
+        return None
+
     def repr_failure(
         self, excinfo: ExceptionInfo[BaseException], style: Optional["_TracebackStyle"] = None
     ) -> Union[str, TerminalRepr]:
         if excinfo.errisinstance(SystemExit):
             # We assume that before doing exit() (which raises SystemExit) we've printed
             # enough context about what happened so that a stack trace is not useful.
             # In particular, uncaught exceptions during semantic analysis or type checking
@@ -348,18 +352,18 @@
                 exception_repr.reprtraceback.reprentries[-1].lines[1:], None, None, repr_file_location, "short"
             )
             exception_repr.reprtraceback.reprentries = [repr_tb_entry]
             return exception_repr
         else:
             return super().repr_failure(excinfo, style="native")
 
-    @no_type_check
     def reportinfo(self) -> Tuple[Union[py.path.local, Path, str], Optional[int], str]:
         # To support both Pytest 6.x and 7.x
         path = getattr(self, "path", None) or getattr(self, "fspath")
+        assert path
         return path, None, self.name
 
     def _collect_python_path(
         self,
         rootdir: Optional[Path],
         execution_path: Path,
     ) -> None:
```

### Comparing `pytest-mypy-plugins-2.0.0/pytest_mypy_plugins/tests/__pycache__/reveal_type_hook.cpython-311.pyc` & `pytest-mypy-plugins-3.0.0/pytest_mypy_plugins/tests/__pycache__/reveal_type_hook.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x9e2b9d64 (Thu Jun 29 06:58:38 2023 UTC)
+moddate:  0xacc1b764 (Wed Jul 19 10:57:48 2023 UTC)
 files sz: 354
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `pytest-mypy-plugins-2.0.0/pytest_mypy_plugins/tests/__pycache__/test_utils.cpython-311-pytest-7.4.0.pyc` & `pytest-mypy-plugins-3.0.0/pytest_mypy_plugins/tests/__pycache__/test_utils.cpython-311-pytest-7.4.0.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x9e2b9d64 (Thu Jun 29 06:58:38 2023 UTC)
+moddate:  0xacc1b764 (Wed Jul 19 10:57:48 2023 UTC)
 files sz: 8631
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 13
    flags     : 0
    code
```

### Comparing `pytest-mypy-plugins-2.0.0/pytest_mypy_plugins/tests/test-parametrized.yml` & `pytest-mypy-plugins-3.0.0/pytest_mypy_plugins/tests/test-parametrized.yml`

 * *Files identical despite different names*

### Comparing `pytest-mypy-plugins-2.0.0/pytest_mypy_plugins/tests/test-regex_assertions.yml` & `pytest-mypy-plugins-3.0.0/pytest_mypy_plugins/tests/test-regex_assertions.yml`

 * *Files identical despite different names*

### Comparing `pytest-mypy-plugins-2.0.0/pytest_mypy_plugins/tests/test-simple-cases.yml` & `pytest-mypy-plugins-3.0.0/pytest_mypy_plugins/tests/test-simple-cases.yml`

 * *Files 20% similar despite different names*

```diff
@@ -56,23 +56,14 @@
 
 - case: error_case
   main: |
     a = 1
     a.lower()  # E: "int" has no attribute "lower"  [attr-defined]
 
 
-- case: custom_mypy_config_strict_optional_true_set
-  main: |
-    from typing import Optional
-    a: Optional[int] = None
-    a + 1
-  mypy_config: |
-    strict_optional = False
-
-
 - case: skip_incorrect_test_case
   skip: yes
   main: |
     a = 1
     reveal_type(a)  # N: boom!
 
 
@@ -97,8 +88,8 @@
 
 - case: fail_if_message_from_outdoes_not_match
   expect_fail: yes
   main: |
     a = 'abc'
     reveal_type(a)
   out: |
-    main:2: note: Some other message
+    main:2: note: Some other message
```

### Comparing `pytest-mypy-plugins-2.0.0/pytest_mypy_plugins/tests/test_utils.py` & `pytest-mypy-plugins-3.0.0/pytest_mypy_plugins/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pytest-mypy-plugins-2.0.0/pytest_mypy_plugins/utils.py` & `pytest-mypy-plugins-3.0.0/pytest_mypy_plugins/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,16 +160,16 @@
 
     max_len = max(len(s1), len(s2))
     extra = ""
     if max_len > maxw:
         extra = "..."
 
     # Write a chunk of both lines, aligned.
-    error_message += "  E: {}{}\n".format(s1[:maxw], extra)
-    error_message += "  A: {}{}\n".format(s2[:maxw], extra)
+    error_message += f"  E: {s1[:maxw]}{extra}\n"
+    error_message += f"  A: {s2[:maxw]}{extra}\n"
     # Write an indicator character under the different columns.
     error_message += "     "
     # sys.stderr.write('     ')
     for j in range(min(maxw, max(len(s1), len(s2)))):
         if s1[j : j + 1] != s2[j : j + 1]:
             error_message += "^"
             break
@@ -204,18 +204,18 @@
 def assert_expected_matched_actual(expected: List[OutputMatcher], actual: List[str]) -> None:
     """Assert that two string arrays are equal.
 
     Display any differences in a human-readable form.
     """
 
     def format_mismatched_line(line: str) -> str:
-        return "  {:<45} (diff)".format(str(line))
+        return f"  {str(line):<45} (diff)"
 
     def format_matched_line(line: str, width: int = 100) -> str:
-        return " {}...".format(line[:width]) if len(line) > width else " {}".format(line)
+        return f" {line[:width]}..." if len(line) > width else f" {line}"
 
     def format_error_lines(lines: List[str]) -> str:
         return "\n".join(lines) if lines else "  (empty)"
 
     expected = sorted(expected, key=lambda om: (om.fname, om.lnum))
     actual = sorted_by_file_and_line(remove_empty_lines(actual))
 
@@ -376,19 +376,7 @@
     if isinstance(path, Path):
         path = path.as_posix()
     os.chdir(str(path))
     try:
         yield
     finally:
         os.chdir(prev_cwd)
-
-
-@contextmanager
-def capture_std_streams() -> Iterator[Tuple[io.StringIO, io.StringIO]]:
-    """Context manager to temporarily capture stdout and stderr.
-
-    Returns ``(stdout, stderr)``.
-    """
-    out = io.StringIO()
-    err = io.StringIO()
-    with contextlib.redirect_stdout(out), contextlib.redirect_stderr(err):
-        yield out, err
```

### Comparing `pytest-mypy-plugins-2.0.0/pytest_mypy_plugins.egg-info/PKG-INFO` & `pytest-mypy-plugins-3.0.0/pytest_mypy_plugins.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: pytest-mypy-plugins
-Version: 2.0.0
+Version: 3.0.0
 Summary: pytest plugin for writing tests for mypy plugins
 Home-page: https://github.com/TypedDjango/pytest-mypy-plugins
 Author: Maksim Kurnikov
 Author-email: maxim.kurnikov@gmail.com
 Maintainer: Nikita Sobolev
 Maintainer-email: mail@sobolevn.me
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <img src="http://mypy-lang.org/static/mypy_light.svg" alt="mypy logo" width="300px"/>
 
 # pytest plugin for testing mypy types, stubs, and plugins
 
@@ -86,15 +86,15 @@
 
 | Property        | Type                                                   | Description                                                                                                         |
 | --------------- | ------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------- |
 | `case`          | `str`                                                  | Name of the test case, complies to `[a-zA-Z0-9]` pattern                                                            |
 | `main`          | `str`                                                  | Portion of the code as if written in `.py` file                                                                     |
 | `files`         | `Optional[List[File]]=[]`\*                            | List of extra files to simulate imports if needed                                                                   |
 | `disable_cache` | `Optional[bool]=False`                                 | Set to `true` disables `mypy` caching                                                                               |
-| `mypy_config`   | `Optional[Dict[str, Union[str, int, bool, float]]]={}` | Inline `mypy` configuration, passed directly to `mypy` as `--config-file` option                                    |
+| `mypy_config`   | `Optional[Dict[str, Union[str, int, bool, float]]]={}` | Inline `mypy` configuration, passed directly to `mypy` as `--config-file` option, possibly joined with `--mypy-pyproject-toml-file` or `--mypy-ini-file` contents if they are passed. By default is treated as `ini`, treated as `toml` only if `--mypy-pyproject-toml-file` is passed |
 | `env`           | `Optional[Dict[str, str]]={}`                          | Environmental variables to be provided inside of test run                                                           |
 | `parametrized`  | `Optional[List[Parameter]]=[]`\*                       | List of parameters, similar to [`@pytest.mark.parametrize`](https://docs.pytest.org/en/stable/parametrize.html)     |
 | `skip`          | `str`                                                  | Expression evaluated with following globals set: `sys`, `os`, `pytest` and `platform`                               |
 | `expect_fail`   | `bool`                                                 | Mark test case as an expected failure, like [`@pytest.mark.xfail`](https://docs.pytest.org/en/stable/skipping.html) |
 | `regex`         | `str`                                                  | Allow regular expressions in comments to be matched against actual output. Defaults to "no", i.e. matches full text.|
 
 (*) Appendix to **pseudo** types used above:
@@ -188,19 +188,26 @@
 
 ## Options
 
 ```
 mypy-tests:
   --mypy-testing-base=MYPY_TESTING_BASE
                         Base directory for tests to use
+  --mypy-pyproject-toml-file=MYPY_PYPROJECT_TOML_FILE
+                        Which `pyproject.toml` file to use
+                        as a default config for tests.
+                        Incompatible with `--mypy-ini-file`
   --mypy-ini-file=MYPY_INI_FILE
-                        Which .ini file to use as a default config for tests
-  --mypy-same-process   Run in the same process. Useful for debugging, will create problems with import cache
+                        Which `.ini` file to use as a default config for tests.
+                        Incompatible with `--mypy-pyproject-toml-file`
+  --mypy-same-process   Run in the same process. Useful for debugging,
+                        will create problems with import cache
   --mypy-extension-hook=MYPY_EXTENSION_HOOK
-                        Fully qualified path to the extension hook function, in case you need custom yaml keys. Has to be top-level.
+                        Fully qualified path to the extension hook function,
+                        in case you need custom yaml keys. Has to be top-level
   --mypy-only-local-stub
                         mypy will ignore errors from site-packages
 
 ```
 
 ## Further reading
```

### Comparing `pytest-mypy-plugins-2.0.0/pytest_mypy_plugins.egg-info/SOURCES.txt` & `pytest-mypy-plugins-3.0.0/pytest_mypy_plugins.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,40 @@
 LICENSE
 MANIFEST.in
 README.md
-mypy.ini
 pyproject.toml
-pytest.ini
+requirements.txt
 setup.py
+tox.ini
 pytest_mypy_plugins/__init__.py
 pytest_mypy_plugins/collect.py
+pytest_mypy_plugins/configs.py
 pytest_mypy_plugins/item.py
 pytest_mypy_plugins/py.typed
 pytest_mypy_plugins/utils.py
 pytest_mypy_plugins.egg-info/PKG-INFO
 pytest_mypy_plugins.egg-info/SOURCES.txt
 pytest_mypy_plugins.egg-info/dependency_links.txt
 pytest_mypy_plugins.egg-info/entry_points.txt
 pytest_mypy_plugins.egg-info/requires.txt
 pytest_mypy_plugins.egg-info/top_level.txt
 pytest_mypy_plugins/tests/reveal_type_hook.py
 pytest_mypy_plugins/tests/test-extension.yml
+pytest_mypy_plugins/tests/test-mypy-config.yml
 pytest_mypy_plugins/tests/test-parametrized.yml
 pytest_mypy_plugins/tests/test-paths-from-env.yml
 pytest_mypy_plugins/tests/test-regex_assertions.yml
 pytest_mypy_plugins/tests/test-simple-cases.yml
+pytest_mypy_plugins/tests/test_explicit_configs.py
 pytest_mypy_plugins/tests/test_utils.py
 pytest_mypy_plugins/tests/__pycache__/reveal_type_hook.cpython-311.pyc
-pytest_mypy_plugins/tests/__pycache__/test_utils.cpython-311-pytest-7.4.0.pyc
+pytest_mypy_plugins/tests/__pycache__/test_explicit_configs.cpython-311-pytest-7.4.0.pyc
+pytest_mypy_plugins/tests/__pycache__/test_utils.cpython-311-pytest-7.4.0.pyc
+pytest_mypy_plugins/tests/test_configs/mypy1.ini
+pytest_mypy_plugins/tests/test_configs/mypy2.ini
+pytest_mypy_plugins/tests/test_configs/pyproject1.toml
+pytest_mypy_plugins/tests/test_configs/pyproject2.toml
+pytest_mypy_plugins/tests/test_configs/setup1.cfg
+pytest_mypy_plugins/tests/test_configs/setup2.cfg
+pytest_mypy_plugins/tests/test_configs/test_join_toml_configs.py
+pytest_mypy_plugins/tests/test_configs/__pycache__/test_join_files.cpython-311-pytest-7.4.0.pyc
+pytest_mypy_plugins/tests/test_configs/__pycache__/test_join_toml_configs.cpython-311-pytest-7.4.0.pyc
```

### Comparing `pytest-mypy-plugins-2.0.0/setup.py` & `pytest-mypy-plugins-3.0.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,46 +1,47 @@
 from setuptools import setup
 
-with open("README.md", "r") as f:
+with open("README.md") as f:
     readme = f.read()
 
 dependencies = [
     "pytest>=7.0.0",
     "mypy>=1.3",
     "decorator",
     "pyyaml",
     "Jinja2",
     "regex",
     "packaging",
+    "tomlkit>=0.11",
 ]
 
 setup(
     name="pytest-mypy-plugins",
-    version="2.0.0",
+    version="3.0.0",
     description="pytest plugin for writing tests for mypy plugins",
     long_description=readme,
     long_description_content_type="text/markdown",
     license="MIT",
     url="https://github.com/TypedDjango/pytest-mypy-plugins",
     author="Maksim Kurnikov",
     author_email="maxim.kurnikov@gmail.com",
     maintainer="Nikita Sobolev",
     maintainer_email="mail@sobolevn.me",
     packages=["pytest_mypy_plugins"],
     # the following makes a plugin available to pytest
     entry_points={"pytest11": ["pytest-mypy-plugins = pytest_mypy_plugins.collect"]},
     install_requires=dependencies,
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     package_data={
         "pytest_mypy_plugins": ["py.typed"],
     },
     classifiers=[
         "Development Status :: 4 - Beta",
         "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Typing :: Typed",
     ],
 )
```

