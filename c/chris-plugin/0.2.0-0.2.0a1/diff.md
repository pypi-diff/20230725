# Comparing `tmp/chris_plugin-0.2.0.tar.gz` & `tmp/chris_plugin-0.2.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chris_plugin-0.2.0.tar", last modified: Tue Jul 25 04:23:48 2023, max compression
+gzip compressed data, was "chris_plugin-0.2.0a1.tar", last modified: Tue Feb 28 21:32:31 2023, max compression
```

## Comparing `chris_plugin-0.2.0.tar` & `chris_plugin-0.2.0a1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 04:23:48.181984 chris_plugin-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-25 04:23:42.000000 chris_plugin-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-07-25 04:23:48.181984 chris_plugin-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-25 04:23:42.000000 chris_plugin-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 04:23:48.181984 chris_plugin-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-07-25 04:23:42.000000 chris_plugin-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 04:23:48.177984 chris_plugin-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 04:23:48.177984 chris_plugin-0.2.0/src/chris_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-07-25 04:23:42.000000 chris_plugin-0.2.0/src/chris_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-25 04:23:42.000000 chris_plugin-0.2.0/src/chris_plugin/_atypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-25 04:23:42.000000 chris_plugin-0.2.0/src/chris_plugin/_registration.py
--rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-07-25 04:23:42.000000 chris_plugin-0.2.0/src/chris_plugin/chris_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-25 04:23:42.000000 chris_plugin-0.2.0/src/chris_plugin/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-25 04:23:42.000000 chris_plugin-0.2.0/src/chris_plugin/limits.py
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-25 04:23:42.000000 chris_plugin-0.2.0/src/chris_plugin/links.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-25 04:23:42.000000 chris_plugin-0.2.0/src/chris_plugin/main_function.py
--rw-r--r--   0 runner    (1001) docker     (123)    12642 2023-07-25 04:23:42.000000 chris_plugin-0.2.0/src/chris_plugin/mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-07-25 04:23:42.000000 chris_plugin-0.2.0/src/chris_plugin/parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 04:23:48.181984 chris_plugin-0.2.0/src/chris_plugin/tool/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 04:23:42.000000 chris_plugin-0.2.0/src/chris_plugin/tool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6512 2023-07-25 04:23:42.000000 chris_plugin-0.2.0/src/chris_plugin/tool/chris_plugin_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-07-25 04:23:42.000000 chris_plugin-0.2.0/src/chris_plugin/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 04:23:48.177984 chris_plugin-0.2.0/src/chris_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-07-25 04:23:48.000000 chris_plugin-0.2.0/src/chris_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-25 04:23:48.000000 chris_plugin-0.2.0/src/chris_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 04:23:48.000000 chris_plugin-0.2.0/src/chris_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-25 04:23:48.000000 chris_plugin-0.2.0/src/chris_plugin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-25 04:23:48.000000 chris_plugin-0.2.0/src/chris_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-25 04:23:48.000000 chris_plugin-0.2.0/src/chris_plugin.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 21:32:31.484109 chris_plugin-0.2.0a1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-02-28 21:32:27.000000 chris_plugin-0.2.0a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-02-28 21:32:31.484109 chris_plugin-0.2.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-02-28 21:32:27.000000 chris_plugin-0.2.0a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-28 21:32:31.484109 chris_plugin-0.2.0a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-02-28 21:32:27.000000 chris_plugin-0.2.0a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 21:32:31.480109 chris_plugin-0.2.0a1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 21:32:31.480109 chris_plugin-0.2.0a1/src/chris_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-02-28 21:32:27.000000 chris_plugin-0.2.0a1/src/chris_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-02-28 21:32:27.000000 chris_plugin-0.2.0a1/src/chris_plugin/_atypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-02-28 21:32:27.000000 chris_plugin-0.2.0a1/src/chris_plugin/_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-02-28 21:32:27.000000 chris_plugin-0.2.0a1/src/chris_plugin/chris_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-02-28 21:32:27.000000 chris_plugin-0.2.0a1/src/chris_plugin/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-02-28 21:32:27.000000 chris_plugin-0.2.0a1/src/chris_plugin/limits.py
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-02-28 21:32:27.000000 chris_plugin-0.2.0a1/src/chris_plugin/links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-02-28 21:32:27.000000 chris_plugin-0.2.0a1/src/chris_plugin/main_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10475 2023-02-28 21:32:27.000000 chris_plugin-0.2.0a1/src/chris_plugin/mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-02-28 21:32:27.000000 chris_plugin-0.2.0a1/src/chris_plugin/parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 21:32:31.484109 chris_plugin-0.2.0a1/src/chris_plugin/tool/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 21:32:27.000000 chris_plugin-0.2.0a1/src/chris_plugin/tool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6512 2023-02-28 21:32:27.000000 chris_plugin-0.2.0a1/src/chris_plugin/tool/chris_plugin_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-02-28 21:32:27.000000 chris_plugin-0.2.0a1/src/chris_plugin/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 21:32:31.484109 chris_plugin-0.2.0a1/src/chris_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-02-28 21:32:31.000000 chris_plugin-0.2.0a1/src/chris_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-02-28 21:32:31.000000 chris_plugin-0.2.0a1/src/chris_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-28 21:32:31.000000 chris_plugin-0.2.0a1/src/chris_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-02-28 21:32:31.000000 chris_plugin-0.2.0a1/src/chris_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-02-28 21:32:31.000000 chris_plugin-0.2.0a1/src/chris_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-28 21:32:31.000000 chris_plugin-0.2.0a1/src/chris_plugin.egg-info/top_level.txt
```

### Comparing `chris_plugin-0.2.0/LICENSE` & `chris_plugin-0.2.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `chris_plugin-0.2.0/PKG-INFO` & `chris_plugin-0.2.0a1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chris_plugin
-Version: 0.2.0
+Version: 0.2.0a1
 Summary: ChRIS plugin helper
 Home-page: https://github.com/FNNDSC/chris_plugin
 Author: Jennings Zhang
 Author-email: dev@babyMRI.org
 License: MIT
 Project-URL: Documentation, https://fnndsc.github.io/chris_plugin/
 Project-URL: Source, https://github.com/FNNDSC/chris_plugin
```

### Comparing `chris_plugin-0.2.0/README.md` & `chris_plugin-0.2.0a1/README.md`

 * *Files identical despite different names*

### Comparing `chris_plugin-0.2.0/setup.py` & `chris_plugin-0.2.0a1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 with open(path.join(path.dirname(path.abspath(__file__)), "README.md")) as f:
     readme = f.read()
 
 
 setup(
     name="chris_plugin",
-    version="0.2.0",
+    version="0.2.0a1",
     packages=find_packages(where="src"),
     package_dir={"": "src", "chris_plugin": "src/chris_plugin"},
     url="https://github.com/FNNDSC/chris_plugin",
     project_urls={
         "Documentation": "https://fnndsc.github.io/chris_plugin/",
         "Source": "https://github.com/FNNDSC/chris_plugin",
         "Tracker": "https://github.com/FNNDSC/chris_plugin/issues",
```

### Comparing `chris_plugin-0.2.0/src/chris_plugin/__init__.py` & `chris_plugin-0.2.0a1/src/chris_plugin/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,13 +46,13 @@
         print(f'Copying {input_file} to {output_file}')
         shutil.copy(input_file, output_file)
 ```
 
 """
 
 from chris_plugin.chris_plugin import chris_plugin
-from chris_plugin.mapper import PathMapper, curry_name_mapper
+from chris_plugin.mapper import PathMapper
 import chris_plugin.types as types
 
 __docformat__ = "numpy"
 
-__all__ = ["chris_plugin", "PathMapper", "curry_name_mapper", "types"]
+__all__ = ["chris_plugin", "PathMapper", "types"]
```

### Comparing `chris_plugin-0.2.0/src/chris_plugin/_atypes.py` & `chris_plugin-0.2.0a1/src/chris_plugin/_atypes.py`

 * *Files identical despite different names*

### Comparing `chris_plugin-0.2.0/src/chris_plugin/_registration.py` & `chris_plugin-0.2.0a1/src/chris_plugin/_registration.py`

 * *Files identical despite different names*

### Comparing `chris_plugin-0.2.0/src/chris_plugin/chris_plugin.py` & `chris_plugin-0.2.0a1/src/chris_plugin/chris_plugin.py`

 * *Files identical despite different names*

### Comparing `chris_plugin-0.2.0/src/chris_plugin/constants.py` & `chris_plugin-0.2.0a1/src/chris_plugin/constants.py`

 * *Files identical despite different names*

### Comparing `chris_plugin-0.2.0/src/chris_plugin/limits.py` & `chris_plugin-0.2.0a1/src/chris_plugin/limits.py`

 * *Files identical despite different names*

### Comparing `chris_plugin-0.2.0/src/chris_plugin/main_function.py` & `chris_plugin-0.2.0a1/src/chris_plugin/main_function.py`

 * *Files identical despite different names*

### Comparing `chris_plugin-0.2.0/src/chris_plugin/mapper.py` & `chris_plugin-0.2.0a1/src/chris_plugin/mapper.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import sys
 from pathlib import Path
 from typing import Callable, Iterable, Iterator, Tuple, Optional, Sequence, Union
 from dataclasses import dataclass, field
 
 NameMapper = Callable[[Path, Path], Path]
 
-
 # Private Helpers
 ########
 
 
 def _verbatim(input_file: Path, output_dir: Path) -> Path:
     return output_dir / input_file
 
@@ -21,77 +20,14 @@
 def _curry_suffix(suffix: str) -> NameMapper:
     def append_suffix(input_file: Path, output_dir: Path) -> Path:
         return (output_dir / input_file).with_suffix(suffix)
 
     return append_suffix
 
 
-def curry_name_mapper(output_template: str) -> Callable[[Path, Path], Path]:
-    """
-    A helper function which creates a function that is a suitable value for
-    the `PathMapper.name_mapper` arguments to `PathMapper` constructor functions.
-
-    Woah! Sorry, I don't really know how better to describe it. Please see the
-    example, or better yet, my tests.
-
-    Examples
-    --------
-
-    A common use case is for a *ChRIS* plugin to have the option to give an output
-    file name template. For example:
-
-    ```shell
-    $ myplugin --output-template 'yummy_{}_processed.txt' inputdir/ outputdir/
-    inputdir/fruits/pear.dat -> outputdir/fruits/yummy_pear_processed.txt
-    inputdir/fruits/apple.dat -> outputdir/fruits/yummy_apple_processed.txt
-    ```
-
-    This can be achieved by:
-
-    ```python
-    from argparse import ArgumentParser
-    import shutil
-    from chris_plugin import chris_plugin, PathMapper, curry_name_mapper
-
-    parser = ArgumentParser()
-    parser.add_argument('-o', '--output-template', type=str,
-                        default='copied_{}.dat',
-                        help='output file name template')
-
-    @chris_plugin(parser)
-    def main(options, inputdir, outputdir):
-        name_mapper = curry_name_mapper(options.output_template)
-        mapper = PathMapper.file_mapper(inputdir, outputdir, name_mapper=name_mapper)
-        for input_file, output_file in mapper:
-            shutil.copy(input_file, output_file)
-    ```
-
-    Parameters
-    ----------
-    output_template: str
-        output file template
-
-    Returns
-    -------
-    name_mapper
-        A function which can be given to `PathMapper` as the parameter for `name_mapper`.
-    """
-
-    def name_mapper(rel_path: Path, output_dir: Path) -> Path:
-        # if output file template ends with {}, then keep file extension
-        if output_template.endswith("{}"):
-            template = output_template[:-2] + rel_path.name
-        else:  # otherwise, drop file extension
-            template = output_template
-        name = template.replace("{}", rel_path.stem).replace("{{}}", "{}")
-        return output_dir / rel_path.with_name(name)
-
-    return name_mapper
-
-
 # Public Classes
 ########
 
 
 @dataclass(frozen=True)
 class PathMapper(Iterable[Tuple[Path, Path]]):
     """
```

### Comparing `chris_plugin-0.2.0/src/chris_plugin/parameters.py` & `chris_plugin-0.2.0a1/src/chris_plugin/parameters.py`

 * *Files identical despite different names*

### Comparing `chris_plugin-0.2.0/src/chris_plugin/tool/chris_plugin_info.py` & `chris_plugin-0.2.0a1/src/chris_plugin/tool/chris_plugin_info.py`

 * *Files identical despite different names*

### Comparing `chris_plugin-0.2.0/src/chris_plugin/types.py` & `chris_plugin-0.2.0a1/src/chris_plugin/types.py`

 * *Files identical despite different names*

### Comparing `chris_plugin-0.2.0/src/chris_plugin.egg-info/PKG-INFO` & `chris_plugin-0.2.0a1/src/chris_plugin.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chris-plugin
-Version: 0.2.0
+Version: 0.2.0a1
 Summary: ChRIS plugin helper
 Home-page: https://github.com/FNNDSC/chris_plugin
 Author: Jennings Zhang
 Author-email: dev@babyMRI.org
 License: MIT
 Project-URL: Documentation, https://fnndsc.github.io/chris_plugin/
 Project-URL: Source, https://github.com/FNNDSC/chris_plugin
```

### Comparing `chris_plugin-0.2.0/src/chris_plugin.egg-info/SOURCES.txt` & `chris_plugin-0.2.0a1/src/chris_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

