# Comparing `tmp/pynthlib-0.0.2.tar.gz` & `tmp/pynthlib-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynthlib-0.0.2.tar", last modified: Sat Jul 22 22:11:10 2023, max compression
+gzip compressed data, was "pynthlib-0.0.3.tar", last modified: Tue Jul 25 20:57:00 2023, max compression
```

## Comparing `pynthlib-0.0.2.tar` & `pynthlib-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-22 22:11:10.981271 pynthlib-0.0.2/
--rw-rw-rw-   0        0        0     1076 2023-01-19 14:17:33.000000 pynthlib-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0     3309 2023-07-22 22:11:10.982778 pynthlib-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2652 2023-07-22 22:08:50.000000 pynthlib-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-22 22:11:10.956199 pynthlib-0.0.2/pynthlib/
--rw-rw-rw-   0        0        0       20 2023-07-22 22:05:39.000000 pynthlib-0.0.2/pynthlib/__init__.py
--rw-rw-rw-   0        0        0     1929 2023-07-22 21:50:38.000000 pynthlib-0.0.2/pynthlib/eval.py
--rw-rw-rw-   0        0        0    29271 2023-07-22 18:28:51.000000 pynthlib-0.0.2/pynthlib/pynth.py
-drwxrwxrwx   0        0        0        0 2023-07-22 22:11:10.980265 pynthlib-0.0.2/pynthlib.egg-info/
--rw-rw-rw-   0        0        0     3309 2023-07-22 22:11:10.000000 pynthlib-0.0.2/pynthlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      261 2023-07-22 22:11:10.000000 pynthlib-0.0.2/pynthlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-22 22:11:10.000000 pynthlib-0.0.2/pynthlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       79 2023-07-22 22:11:10.000000 pynthlib-0.0.2/pynthlib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-22 22:11:10.000000 pynthlib-0.0.2/pynthlib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-01-19 14:15:59.000000 pynthlib-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0      811 2023-07-22 22:11:10.989788 pynthlib-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-25 20:57:00.902320 pynthlib-0.0.3/
+-rw-rw-rw-   0        0        0     1076 2023-01-19 14:17:33.000000 pynthlib-0.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     3587 2023-07-25 20:57:00.902320 pynthlib-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2930 2023-07-25 20:52:46.000000 pynthlib-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 20:57:00.878316 pynthlib-0.0.3/pynthlib/
+-rw-rw-rw-   0        0        0       20 2023-07-22 22:05:39.000000 pynthlib-0.0.3/pynthlib/__init__.py
+-rw-rw-rw-   0        0        0     1929 2023-07-22 21:50:38.000000 pynthlib-0.0.3/pynthlib/eval.py
+-rw-rw-rw-   0        0        0    29271 2023-07-22 18:28:51.000000 pynthlib-0.0.3/pynthlib/pynth.py
+drwxrwxrwx   0        0        0        0 2023-07-25 20:57:00.898311 pynthlib-0.0.3/pynthlib.egg-info/
+-rw-rw-rw-   0        0        0     3587 2023-07-25 20:57:00.000000 pynthlib-0.0.3/pynthlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      261 2023-07-25 20:57:00.000000 pynthlib-0.0.3/pynthlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 20:57:00.000000 pynthlib-0.0.3/pynthlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       94 2023-07-25 20:57:00.000000 pynthlib-0.0.3/pynthlib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-25 20:57:00.000000 pynthlib-0.0.3/pynthlib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-01-19 14:15:59.000000 pynthlib-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0      828 2023-07-25 20:57:00.906322 pynthlib-0.0.3/setup.cfg
```

### Comparing `pynthlib-0.0.2/LICENSE.txt` & `pynthlib-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pynthlib-0.0.2/PKG-INFO` & `pynthlib-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynthlib
-Version: 0.0.2
+Version: 0.0.3
 Summary: Intuitive sound synthesis in python.
 Home-page: https://github.com/MatejBevec/pynth
 Author: Matej Bevec
 Author-email: matejbevec98@gmail.com
 License: MIT
 Project-URL: repository, https://github.com/MatejBevec/pynth
 Classifier: Development Status :: 1 - Planning
@@ -31,15 +31,17 @@
 
 Or directly from this repo:
 ```
 git clone https://github.com/MatejBevec/pynth
 pip install ./pynthlib
 ```
 
- 
+To visualize the computation graphs, you will also need to install Graphviz, which
+
+Note that the `graphviz` library, used to visualize computation graphs, requires an installation of the *Graphviz* sofware. See https://pypi.org/project/graphviz/ for installation instructions.
 
 ## Usage
 
 Below are some usage examples. 
 For more info, feel free to read `DESCRIPTION.pdf` and check out `examples.py`.
 
 Please note that this project is in a prototype stage and is not optimized in terms of performance and reliability and is missing many planned features.
```

### Comparing `pynthlib-0.0.2/README.md` & `pynthlib-0.0.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -12,15 +12,17 @@
 
 Or directly from this repo:
 ```
 git clone https://github.com/MatejBevec/pynth
 pip install ./pynthlib
 ```
 
- 
+To visualize the computation graphs, you will also need to install Graphviz, which
+
+Note that the `graphviz` library, used to visualize computation graphs, requires an installation of the *Graphviz* sofware. See https://pypi.org/project/graphviz/ for installation instructions.
 
 ## Usage
 
 Below are some usage examples. 
 For more info, feel free to read `DESCRIPTION.pdf` and check out `examples.py`.
 
 Please note that this project is in a prototype stage and is not optimized in terms of performance and reliability and is missing many planned features.
```

### Comparing `pynthlib-0.0.2/pynthlib/eval.py` & `pynthlib-0.0.3/pynthlib/eval.py`

 * *Files identical despite different names*

### Comparing `pynthlib-0.0.2/pynthlib/pynth.py` & `pynthlib-0.0.3/pynthlib/pynth.py`

 * *Files identical despite different names*

### Comparing `pynthlib-0.0.2/pynthlib.egg-info/PKG-INFO` & `pynthlib-0.0.3/pynthlib.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynthlib
-Version: 0.0.2
+Version: 0.0.3
 Summary: Intuitive sound synthesis in python.
 Home-page: https://github.com/MatejBevec/pynth
 Author: Matej Bevec
 Author-email: matejbevec98@gmail.com
 License: MIT
 Project-URL: repository, https://github.com/MatejBevec/pynth
 Classifier: Development Status :: 1 - Planning
@@ -31,15 +31,17 @@
 
 Or directly from this repo:
 ```
 git clone https://github.com/MatejBevec/pynth
 pip install ./pynthlib
 ```
 
- 
+To visualize the computation graphs, you will also need to install Graphviz, which
+
+Note that the `graphviz` library, used to visualize computation graphs, requires an installation of the *Graphviz* sofware. See https://pypi.org/project/graphviz/ for installation instructions.
 
 ## Usage
 
 Below are some usage examples. 
 For more info, feel free to read `DESCRIPTION.pdf` and check out `examples.py`.
 
 Please note that this project is in a prototype stage and is not optimized in terms of performance and reliability and is missing many planned features.
```

### Comparing `pynthlib-0.0.2/setup.cfg` & `pynthlib-0.0.3/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 796e 7468 6c69 620d 0a76 6572   = pynthlib..ver
-00000020: 7369 6f6e 203d 2030 2e30 2e32 0d0a 6175  sion = 0.0.2..au
+00000020: 7369 6f6e 203d 2030 2e30 2e33 0d0a 6175  sion = 0.0.3..au
 00000030: 7468 6f72 203d 204d 6174 656a 2042 6576  thor = Matej Bev
 00000040: 6563 0d0a 6175 7468 6f72 5f65 6d61 696c  ec..author_email
 00000050: 203d 206d 6174 656a 6265 7665 6339 3840   = matejbevec98@
 00000060: 676d 6169 6c2e 636f 6d0d 0a64 6573 6372  gmail.com..descr
 00000070: 6970 7469 6f6e 203d 2049 6e74 7569 7469  iption = Intuiti
 00000080: 7665 2073 6f75 6e64 2073 796e 7468 6573  ve sound synthes
 00000090: 6973 2069 6e20 7079 7468 6f6e 2e0d 0a6c  is in python...l
@@ -41,11 +41,12 @@
 00000280: 6573 203d 203e 3d33 2e38 0d0a 696e 7374  es = >=3.8..inst
 00000290: 616c 6c5f 7265 7175 6972 6573 203d 200d  all_requires = .
 000002a0: 0a09 6b65 7962 6f61 7264 3e3d 302e 3133  ..keyboard>=0.13
 000002b0: 2c0d 0a09 6e75 6d70 793e 3d31 2e32 312e  ,...numpy>=1.21.
 000002c0: 302c 0d0a 0973 6369 7079 3e3d 312e 372e  0,...scipy>=1.7.
 000002d0: 302c 0d0a 0973 6f75 6e64 6465 7669 6365  0,...sounddevice
 000002e0: 3e3d 302e 342e 322c 0d0a 096d 6174 706c  >=0.4.2,...matpl
-000002f0: 6f74 6c69 623e 3d33 2e32 2e30 2c0d 0a0d  otlib>=3.2.0,...
-00000300: 0a5b 6567 675f 696e 666f 5d0d 0a74 6167  .[egg_info]..tag
-00000310: 5f62 7569 6c64 203d 200d 0a74 6167 5f64  _build = ..tag_d
-00000320: 6174 6520 3d20 300d 0a0d 0a              ate = 0....
+000002f0: 6f74 6c69 623e 3d33 2e32 2e30 2c0d 0a09  otlib>=3.2.0,...
+00000300: 6772 6170 6876 697a 3e3d 302e 3134 0d0a  graphviz>=0.14..
+00000310: 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a 7461  ..[egg_info]..ta
+00000320: 675f 6275 696c 6420 3d20 0d0a 7461 675f  g_build = ..tag_
+00000330: 6461 7465 203d 2030 0d0a 0d0a            date = 0....
```

