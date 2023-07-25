# Comparing `tmp/vulcan-py-2.0.4.tar.gz` & `tmp/vulcan-py-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vulcan-py-2.0.4.tar", last modified: Fri Dec  9 15:54:18 2022, max compression
+gzip compressed data, was "vulcan-py-2.1.0.tar", last modified: Tue Jul 25 14:37:51 2023, max compression
```

## Comparing `vulcan-py-2.0.4.tar` & `vulcan-py-2.1.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 15:54:18.936090 vulcan-py-2.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    10762 2022-12-09 15:53:58.000000 vulcan-py-2.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      168 2022-12-09 15:53:58.000000 vulcan-py-2.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12845 2022-12-09 15:54:18.936090 vulcan-py-2.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12208 2022-12-09 15:53:58.000000 vulcan-py-2.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2022-12-09 15:53:58.000000 vulcan-py-2.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-09 15:54:18.936090 vulcan-py-2.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 15:54:18.936090 vulcan-py-2.0.4/vulcan/
--rw-r--r--   0 runner    (1001) docker     (123)     6909 2022-12-09 15:53:58.000000 vulcan-py-2.0.4/vulcan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6356 2022-12-09 15:53:58.000000 vulcan-py-2.0.4/vulcan/build_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2022-12-09 15:53:58.000000 vulcan-py-2.0.4/vulcan/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    10015 2022-12-09 15:53:58.000000 vulcan-py-2.0.4/vulcan/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4917 2022-12-09 15:53:58.000000 vulcan-py-2.0.4/vulcan/isolation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2022-12-09 15:53:58.000000 vulcan-py-2.0.4/vulcan/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 15:54:18.936090 vulcan-py-2.0.4/vulcan/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-09 15:53:58.000000 vulcan-py-2.0.4/vulcan/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6328 2022-12-09 15:53:58.000000 vulcan-py-2.0.4/vulcan/scripts/setuppy_to_pep621.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2022-12-09 15:53:58.000000 vulcan-py-2.0.4/vulcan/scripts/vulcan_1_to_2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 15:54:18.936090 vulcan-py-2.0.4/vulcan_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12845 2022-12-09 15:54:18.000000 vulcan-py-2.0.4/vulcan_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      452 2022-12-09 15:54:18.000000 vulcan-py-2.0.4/vulcan_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-09 15:54:18.000000 vulcan-py-2.0.4/vulcan_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      220 2022-12-09 15:54:18.000000 vulcan-py-2.0.4/vulcan_py.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2022-12-09 15:54:18.000000 vulcan-py-2.0.4/vulcan_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2022-12-09 15:54:18.000000 vulcan-py-2.0.4/vulcan_py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:37:51.177558 vulcan-py-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10762 2023-07-25 14:37:26.000000 vulcan-py-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-25 14:37:26.000000 vulcan-py-2.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12845 2023-07-25 14:37:51.177558 vulcan-py-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12208 2023-07-25 14:37:26.000000 vulcan-py-2.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-07-25 14:37:26.000000 vulcan-py-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 14:37:51.177558 vulcan-py-2.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:37:51.177558 vulcan-py-2.1.0/vulcan/
+-rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-07-25 14:37:26.000000 vulcan-py-2.1.0/vulcan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-07-25 14:37:26.000000 vulcan-py-2.1.0/vulcan/build_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-07-25 14:37:26.000000 vulcan-py-2.1.0/vulcan/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10065 2023-07-25 14:37:26.000000 vulcan-py-2.1.0/vulcan/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4901 2023-07-25 14:37:26.000000 vulcan-py-2.1.0/vulcan/isolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-07-25 14:37:26.000000 vulcan-py-2.1.0/vulcan/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:37:51.177558 vulcan-py-2.1.0/vulcan/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:37:26.000000 vulcan-py-2.1.0/vulcan/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6311 2023-07-25 14:37:26.000000 vulcan-py-2.1.0/vulcan/scripts/setuppy_to_pep621.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-07-25 14:37:26.000000 vulcan-py-2.1.0/vulcan/scripts/vulcan_1_to_2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:37:51.177558 vulcan-py-2.1.0/vulcan_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12845 2023-07-25 14:37:51.000000 vulcan-py-2.1.0/vulcan_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-25 14:37:51.000000 vulcan-py-2.1.0/vulcan_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 14:37:51.000000 vulcan-py-2.1.0/vulcan_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-25 14:37:51.000000 vulcan-py-2.1.0/vulcan_py.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-25 14:37:51.000000 vulcan-py-2.1.0/vulcan_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-25 14:37:51.000000 vulcan-py-2.1.0/vulcan_py.egg-info/top_level.txt
```

### Comparing `vulcan-py-2.0.4/LICENSE` & `vulcan-py-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vulcan-py-2.0.4/PKG-INFO` & `vulcan-py-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: vulcan-py
-Version: 2.0.4
+Version: 2.1.0
 Summary: Tool for leveraging lockfiles to pin dependencies in wheels and sdists
 Author-email: Joel Christiansen <joelchristiansen@optiver.com>
 License: Apache License Version 2.0
 Project-URL: github, https://github.com/optiver/vulcan-py
 Keywords: build,tooling
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: cli
 Provides-Extra: convert
 License-File: LICENSE
 
 ![Vulcan](https://raw.githubusercontent.com/optiver/vulcan-py/master/images/Vulcan_Logo.png)
 
 ---
 
-Vulcan supports building python>=3.6. Vulcan itself may only be installed in python>=3.7. 
+Vulcan supports building python>=3.6. Vulcan itself may only be installed in python>=3.8. 
 The recommended installation is via pipx. This will save a lot of pain with respect to conflicting versions,
 as well as having multiple python versions in various projects.
 
 ---
 
 [//]: # ( TODO: build status indicator here )
```

### Comparing `vulcan-py-2.0.4/README.md` & `vulcan-py-2.1.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ![Vulcan](https://raw.githubusercontent.com/optiver/vulcan-py/master/images/Vulcan_Logo.png)
 
 ---
 
-Vulcan supports building python>=3.6. Vulcan itself may only be installed in python>=3.7. 
+Vulcan supports building python>=3.6. Vulcan itself may only be installed in python>=3.8. 
 The recommended installation is via pipx. This will save a lot of pain with respect to conflicting versions,
 as well as having multiple python versions in various projects.
 
 ---
 
 [//]: # ( TODO: build status indicator here )
```

### Comparing `vulcan-py-2.0.4/pyproject.toml` & `vulcan-py-2.1.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [project]
 name = "vulcan-py"
-version = "2.0.4"
+version = "2.1.0"
 description = "Tool for leveraging lockfiles to pin dependencies in wheels and sdists"
 authors = [{name="Joel Christiansen", email="joelchristiansen@optiver.com"}]
 urls = {github="https://github.com/optiver/vulcan-py"}
 license = {text="Apache License Version 2.0"}
-keywords = [ "build", "tooling" ] 
+keywords = [ "build", "tooling" ]
 classifiers = [
     "Topic :: Software Development :: Build Tools",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "License :: OSI Approved :: Apache Software License"
 ]
 readme = {file = "README.md", content-type = "text/markdown"}
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 dynamic = ["dependencies", "optional-dependencies"]
 
 [project.scripts]
 vulcan="vulcan.cli:main"
 convert_pep621="vulcan.scripts.setuppy_to_pep621:convert"
 convert_vulcan2="vulcan.scripts.vulcan_1_to_2:convert"
 
@@ -29,62 +29,59 @@
 [tool.setuptools.packages.find]
 include = ["vulcan*"]
 
 
 # e.g. if these are specified, like `pip install vulcan[cli]
 [tool.vulcan.extras]
 cli=["shiv~=0.5.2","build[virtualenv]~=0.8.0", "click~=8.0"]
-convert=["pkginfo~=1.7"]
+convert=["pkginfo~=1.9"]
 
 [tool.vulcan.dependencies]
 setuptools='~=63.0'
 wheel='~=0.36.2'
-typing_extensions= "~=3.7; python_version<='3.7'"
 tomlkit = "~=0.11"
-importlib_metadata = "~=4.6; python_version<='3.7'"
-editables = '~=0.2'
+editables = '~=0.5'
 packaging = "~=22.0"
 
 [tool.vulcan.dev-dependencies.test]
 pytest=""
 pytest-asyncio=""
 pkginfo=""
 coverage=""
 
 [tool.vulcan.dev-dependencies.static-analysis]
 flake8=""
 mypy=""
+pkginfo=""
 types-click=""
 types-dataclasses=""
 types-setuptools=""
 
 
 [build-system]
 # in other build systems, this would says "requires=['setuptools', 'vulcan']" and that is all that is needed
 # to correctly install and use this tool
 requires=['setuptools~=63.0',
           'tomlkit~=0.9',
           'wheel',
-          "typing_extensions; python_version<='3.7'", 
-          'editables~=0.2',
-          "importlib_metadata; python_version<='3.7'"]
+          'editables~=0.5']
 build-backend="vulcan.build_backend"
 backend-path=["."]  # and this line should be removed for all other projects
 
 [tool.pytest.ini_options]
-filterwarnings = [ 
+filterwarnings = [
  "ignore:.*the imp module is deprecated in favour of importl.*:DeprecationWarning",
  "ignore:.*The loop argument is deprecated since Python 3.8, and scheduled for removal in Python 3.10.*:DeprecationWarning" ]
 junit_family="xunit1"
 testpaths = [ "tests", ]
 markers = [ "cli: Tests that require full cli dependencies" ]
 asyncio_mode = 'auto'
 
 [tool.mypy]
-files = ["vulcan","tests"]
+packages = ["vulcan","tests"]
 # the following configs are the equivalent of --strict, with the exception of --no-implicit-optional
 no_implicit_optional = false
 check_untyped_defs = true
 disallow_any_generics = true
 disallow_incomplete_defs = true
 disallow_subclassing_any = true
 disallow_untyped_calls = true
@@ -94,11 +91,7 @@
 warn_return_any = true
 warn_unused_configs = true
 
 # extra warnings
 warn_unused_ignores = true
 warn_unreachable = true
 strict_equality = true
-
-[[tool.mypy.overrides]]
-module = ['vulcan.isolation']
-warn_unused_ignores = false
```

### Comparing `vulcan-py-2.0.4/vulcan/__init__.py` & `vulcan-py-2.1.0/vulcan/__init__.py`

 * *Files identical despite different names*

### Comparing `vulcan-py-2.0.4/vulcan/build_backend.py` & `vulcan-py-2.1.0/vulcan/build_backend.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import subprocess
 import sys
 import tempfile
 from contextlib import contextmanager
 from pathlib import Path
 from typing import Callable, Dict, Generator, List, Optional, Tuple
 
-from editables import EditableProject  # type: ignore
+from editables import EditableProject
 
 from vulcan import Vulcan
 from vulcan.plugins import PluginRunner
 
 version: Callable[[str], str]
 if sys.version_info >= (3, 8):
     from importlib.metadata import version
@@ -33,15 +33,15 @@
 def build(outdir: str, config_settings: Dict[str, str] = None) -> str:
     config = Vulcan.from_source(Path().absolute())
 
     # https://setuptools.readthedocs.io/en/latest/userguide/keywords.html
     # https://docs.python.org/3/distutils/apiref.html
     with PluginRunner(config):
         dist = config.setup(config_settings=config_settings)
-    rel_dist = Path(dist.dist_files[0][-1])  # type: ignore[attr-defined]
+    rel_dist = Path(dist.dist_files[0][-1])
     shutil.move(str(rel_dist), Path(outdir) / rel_dist.name)
     return rel_dist.name
 
 
 def build_wheel(wheel_directory: str, config_settings: Dict[str, str] = None, metadata_directory: str = None) -> str:
     with patch_argv(['bdist_wheel']):
         return build(wheel_directory, config_settings)
@@ -81,30 +81,33 @@
     out = subprocess.check_output([str(python_callable), '-m', 'pip', '--version'], encoding='utf-8')
     m = re.search(r'pip (\d+\.\d+(\.\d+)?)', out)
     if not m:
         return None
     return tuple((int(n) for n in m.group(1).split('.')))
 
 
-def install_develop() -> None:
+def install_develop(build_isolation: bool) -> None:
     config = Vulcan.from_source(Path().absolute())
 
     try:
         virtual_env = get_virtualenv_python()
     except RuntimeError:
         exit('may not use vulcan develop outside of a virtualenv')
     pip_version = get_pip_version(virtual_env)
     if pip_version is None or pip_version < (21, 3):
         print(f"pip version {pip_version} does not support editable installs for PEP517 projects,"
               " Please upgrade your pip")
 
     path = str(Path().absolute())
     if config.configured_extras:
         path = f'{path}[{",".join(config.configured_extras)}]'
-    subprocess.check_call([str(virtual_env), '-m', 'pip', 'install', '-e', path])
+    pip_call = [str(virtual_env), '-m', 'pip', 'install', '-e', path]
+    if not build_isolation:
+        pip_call.append('--no-build-isolation')
+    subprocess.check_call(pip_call)
 
 
 # pep660 functions
 def unpack(whl: Path) -> Path:
     with tempfile.TemporaryDirectory() as tmp:
         subprocess.check_output(f'wheel unpack {whl} -d {tmp}'.split())
         unpacked = list(Path(tmp).glob('*'))
@@ -156,14 +159,20 @@
     project = EditableProject(project_name, Path().absolute())
     packages = (p for p in unpacked_whl_dir.iterdir() if not p.name.endswith('.dist-info'))
     for package in packages:
         project.map(package.name, _find_local_package(package.name))
         # removing the actual code packages because they will conflict with the .pth files, and take
         # precendence over them
         shutil.rmtree(unpacked_whl_dir / package.name)
+
+    # None of the IDEs/static type tools support PEP 660
+    # As a fall-back for static analysis also provide the path in the .pth file
+    # https://github.com/microsoft/pylance-release/blob/main/TROUBLESHOOTING.md#editable-install-modules-not-found
+    project.add_to_path(project.project_dir)
+
     for name, content in project.files():
         (unpacked_whl_dir / name).write_text(content)
 
     assert whl == pack(unpacked_whl_dir), 'pre-wheel and post-wheel should be the same path'
     shutil.rmtree(unpacked_whl_dir)
```

### Comparing `vulcan-py-2.0.4/vulcan/builder.py` & `vulcan-py-2.1.0/vulcan/builder.py`

 * *Files identical despite different names*

### Comparing `vulcan-py-2.0.4/vulcan/cli.py` & `vulcan-py-2.1.0/vulcan/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -168,33 +168,33 @@
 @main.command()
 @click.argument('req', type=Requirement.parse)
 @click.option('--lock/--no-lock', '_lock', default=True)
 @pass_vulcan  # order matters, closest to the function definition comes first
 @click.pass_context
 def add(ctx: click.Context, config: Vulcan, req: Requirement, _lock: bool) -> None:
     "Add new top-level dependency and regenerate lockfile"
-    name: str = req.name  # type: ignore
+    name: str = req.name
     if req.extras:
         name = f'{name}[{",".join(req.extras)}]'
     try:
         venv_python = get_virtualenv_python()
     except RuntimeError:
         exit("Must be in a virtualenv to use `vulcan add`")
     subprocess.check_call([str(venv_python), '-m', 'pip', 'install', str(req)])
-    if req.specifier:  # type: ignore
+    if req.specifier:
         # if the user gave a version spec, we blindly take that
-        version = str(req.specifier)  # type: ignore
+        version = str(req.specifier)
     else:
         # otherwise, we take a freeze to see what was actually installed
         freeze = subprocess.check_output([str(venv_python), '-m', 'pip', 'freeze'], encoding='utf-8').strip()
         try:
             # try and find the thing we just added
-            line = next(ln for ln in freeze.split('\n') if ln.startswith(req.name))  # type: ignore
+            line = next(ln for ln in freeze.split('\n') if ln.startswith(req.name))
             # and parse it to a version
-            spec = packaging.version.parse(str(Requirement.parse(line.strip()).specifier  # type: ignore
+            spec = packaging.version.parse(str(Requirement.parse(line.strip()).specifier
                                                )[2:])  # remove the == at the start
             version = f'~={spec.major}.{spec.minor}'
         except StopIteration:
             # failed to find the thing we just installed, give up.
             version = ''
     with open('pyproject.toml') as f:
         parse = tomlkit.parse(f.read())
@@ -233,14 +233,15 @@
                     [str(virtual_env), '-m', 'pip', 'install', *(flatten_reqs(section) or [])],
                     encoding='utf-8'),
                       flush=True)
 
 
 @main.command()
 @click.argument('dev_deps_target', required=False, type=str)
-def develop(dev_deps_target: Optional[str]) -> None:
-    install_develop()
+@click.option('--build-isolation/--no-build-isolation', '_build_isolation', default=True)
+def develop(dev_deps_target: Optional[str], _build_isolation: bool) -> None:
+    install_develop(_build_isolation)
     install_dev_dependencies(target=dev_deps_target)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `vulcan-py-2.0.4/vulcan/isolation.py` & `vulcan-py-2.1.0/vulcan/isolation.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,8 +108,8 @@
                                                       stdout=asyncio.subprocess.PIPE)
 
         out, err = await frozen.communicate()
         assert frozen.returncode is not None
         if frozen.returncode != 0:
             raise subprocess.CalledProcessError(returncode=frozen.returncode, cmd=cmd, output=out, stderr=err)
         reqs = [Requirement.parse(line) for line in out.decode().split('\n') if line]
-        return {Requirement.parse(req.name): req for req in reqs}  # type: ignore
+        return {Requirement.parse(req.name): req for req in reqs}
```

### Comparing `vulcan-py-2.0.4/vulcan/plugins.py` & `vulcan-py-2.1.0/vulcan/plugins.py`

 * *Files identical despite different names*

### Comparing `vulcan-py-2.0.4/vulcan/scripts/setuppy_to_pep621.py` & `vulcan-py-2.1.0/vulcan/scripts/setuppy_to_pep621.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from argparse import ArgumentParser
 from collections import defaultdict
 from configparser import ConfigParser
 from io import StringIO
 from pathlib import Path
 from typing import Dict, List, NamedTuple, Optional, cast
 
-import pkginfo  # type: ignore
+import pkginfo
 import tomlkit
 from pkg_resources import Requirement
 
 
 class BuildData(NamedTuple):
     wheel: pkginfo.Wheel
     table: tomlkit.items.Table
@@ -25,15 +25,15 @@
     return parser
 
 
 def wheel() -> BuildData:
 
     with tempfile.TemporaryDirectory(suffix='.vulcan-migrate') as tmp:
         subprocess.run(['pip', 'wheel', '--no-deps', '-w', tmp, '.'])
-        whl = pkginfo.Wheel(next(Path(tmp).glob('*.whl')))
+        whl = pkginfo.Wheel(str(next(Path(tmp).glob('*.whl'))))
         eps: Dict[str, Dict[str, str]] = defaultdict(dict)
         with zipfile.ZipFile(whl.filename) as zf:
             dist_info = f'{whl.name.replace("-", "_")}-{whl.version}.dist-info'
             try:
                 with zf.open(f'{dist_info}/entry_points.txt') as f:
                     cp = ConfigParser()
                     cp.read_file(StringIO(f.read().decode()))
@@ -102,19 +102,19 @@
     project['name'] = whl.name
     project['dynamic'] = ['version']
     if whl.author or whl.author_email:
         project['authors'] = contributors(whl.author, whl.author_email)
     if whl.maintainer or whl.maintainer_email:
         project['maintainers'] = contributors(whl.maintainer, whl.maintainer_email)
     if whl.classifiers:
-        project['classifiers'] = tomlkit.array(whl.classifiers).multiline(True)
+        project['classifiers'] = tomlkit.array(str(whl.classifiers)).multiline(True)
     if whl.summary:
         project['description'] = whl.summary
     if whl.keywords:
-        project['keywords'] = tomlkit.array(whl.keywords.split(',')).multiline(True)
+        project['keywords'] = tomlkit.array(str(whl.keywords.split(','))).multiline(True)
     if whl.license:
         project['license'] = whl.license
     if whl.project_urls:
         project['urls'] = {k: v for k, v in [u.split(', ') for u in whl.project_urls]}
     try:
         readme = next(p for p in Path().iterdir() if p.name.lower().startswith('readme'))
         project['readme'] = str(readme)
@@ -125,15 +125,15 @@
         project['dynamic'].append('dependencies')  # type: ignore[attr-defined]
         vulcan['dependencies'] = {}
         for req in whl.requires_dist:
             parsed_req = Requirement.parse(req)
             if '; extra == "' in str(parsed_req):
                 # extra, swing back to this
                 continue
-            name = parsed_req.name  # type: ignore
+            name = parsed_req.name
             if parsed_req.extras:
                 name = f'{name}[{",".join(parsed_req.extras)}]'
             vulcan['dependencies'][name] = str(parsed_req.specifier)  # type: ignore
     if whl.provides_extras:
         project['dynamic'].append('optional-dependencies')  # type: ignore[attr-defined]
         extras = tomlkit.table()
         vulcan['extras'] = extras
```

### Comparing `vulcan-py-2.0.4/vulcan/scripts/vulcan_1_to_2.py` & `vulcan-py-2.1.0/vulcan/scripts/vulcan_1_to_2.py`

 * *Files identical despite different names*

### Comparing `vulcan-py-2.0.4/vulcan_py.egg-info/PKG-INFO` & `vulcan-py-2.1.0/vulcan_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: vulcan-py
-Version: 2.0.4
+Version: 2.1.0
 Summary: Tool for leveraging lockfiles to pin dependencies in wheels and sdists
 Author-email: Joel Christiansen <joelchristiansen@optiver.com>
 License: Apache License Version 2.0
 Project-URL: github, https://github.com/optiver/vulcan-py
 Keywords: build,tooling
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: cli
 Provides-Extra: convert
 License-File: LICENSE
 
 ![Vulcan](https://raw.githubusercontent.com/optiver/vulcan-py/master/images/Vulcan_Logo.png)
 
 ---
 
-Vulcan supports building python>=3.6. Vulcan itself may only be installed in python>=3.7. 
+Vulcan supports building python>=3.6. Vulcan itself may only be installed in python>=3.8. 
 The recommended installation is via pipx. This will save a lot of pain with respect to conflicting versions,
 as well as having multiple python versions in various projects.
 
 ---
 
 [//]: # ( TODO: build status indicator here )
```

