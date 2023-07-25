# Comparing `tmp/pytch-fetch-1.0.1.tar.gz` & `tmp/pytch-fetch-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytch-fetch-1.0.1.tar", last modified: Mon Jul 24 15:35:19 2023, max compression
+gzip compressed data, was "pytch-fetch-1.1.0.tar", last modified: Tue Jul 25 16:15:23 2023, max compression
```

## Comparing `pytch-fetch-1.0.1.tar` & `pytch-fetch-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 krit      (1000) krit      (1001)        0 2023-07-24 15:35:19.776999 pytch-fetch-1.0.1/
--rw-r--r--   0 krit      (1000) krit      (1001)     1066 2023-07-24 09:11:38.000000 pytch-fetch-1.0.1/LICENSE
--rw-r--r--   0 krit      (1000) krit      (1001)     4099 2023-07-24 15:35:19.776999 pytch-fetch-1.0.1/PKG-INFO
--rw-r--r--   0 krit      (1000) krit      (1001)     1658 2023-07-24 15:21:55.000000 pytch-fetch-1.0.1/README.md
--rw-r--r--   0 krit      (1000) krit      (1001)     1298 2023-07-24 15:34:52.000000 pytch-fetch-1.0.1/pyproject.toml
--rw-r--r--   0 krit      (1000) krit      (1001)       38 2023-07-24 15:35:19.776999 pytch-fetch-1.0.1/setup.cfg
-drwxr-xr-x   0 krit      (1000) krit      (1001)        0 2023-07-24 15:35:19.773999 pytch-fetch-1.0.1/src/
-drwxr-xr-x   0 krit      (1000) krit      (1001)        0 2023-07-24 15:35:19.774999 pytch-fetch-1.0.1/src/pytch/
--rw-r--r--   0 krit      (1000) krit      (1001)        0 2023-07-24 09:11:38.000000 pytch-fetch-1.0.1/src/pytch/__init__.py
--rwxr-xr-x   0 krit      (1000) krit      (1001)     2207 2023-07-24 15:34:37.000000 pytch-fetch-1.0.1/src/pytch/__main__.py
--rw-r--r--   0 krit      (1000) krit      (1001)    19845 2023-07-24 13:46:09.000000 pytch-fetch-1.0.1/src/pytch/art.py
--rw-r--r--   0 krit      (1000) krit      (1001)     4596 2023-07-24 15:34:15.000000 pytch-fetch-1.0.1/src/pytch/funcs.py
-drwxr-xr-x   0 krit      (1000) krit      (1001)        0 2023-07-24 15:35:19.776999 pytch-fetch-1.0.1/src/pytch_fetch.egg-info/
--rw-r--r--   0 krit      (1000) krit      (1001)     4099 2023-07-24 15:35:19.000000 pytch-fetch-1.0.1/src/pytch_fetch.egg-info/PKG-INFO
--rw-r--r--   0 krit      (1000) krit      (1001)      310 2023-07-24 15:35:19.000000 pytch-fetch-1.0.1/src/pytch_fetch.egg-info/SOURCES.txt
--rw-r--r--   0 krit      (1000) krit      (1001)        1 2023-07-24 15:35:19.000000 pytch-fetch-1.0.1/src/pytch_fetch.egg-info/dependency_links.txt
--rw-r--r--   0 krit      (1000) krit      (1001)       46 2023-07-24 15:35:19.000000 pytch-fetch-1.0.1/src/pytch_fetch.egg-info/entry_points.txt
--rw-r--r--   0 krit      (1000) krit      (1001)        6 2023-07-24 15:35:19.000000 pytch-fetch-1.0.1/src/pytch_fetch.egg-info/top_level.txt
+drwxr-xr-x   0 krit      (1000) krit      (1001)        0 2023-07-25 16:15:23.363761 pytch-fetch-1.1.0/
+-rw-r--r--   0 krit      (1000) krit      (1001)     1066 2023-07-24 09:11:38.000000 pytch-fetch-1.1.0/LICENSE
+-rw-r--r--   0 krit      (1000) krit      (1001)     4220 2023-07-25 16:15:23.363761 pytch-fetch-1.1.0/PKG-INFO
+-rw-r--r--   0 krit      (1000) krit      (1001)     1779 2023-07-25 16:13:59.000000 pytch-fetch-1.1.0/README.md
+-rw-r--r--   0 krit      (1000) krit      (1001)     1298 2023-07-25 16:13:59.000000 pytch-fetch-1.1.0/pyproject.toml
+-rw-r--r--   0 krit      (1000) krit      (1001)       38 2023-07-25 16:15:23.363761 pytch-fetch-1.1.0/setup.cfg
+drwxr-xr-x   0 krit      (1000) krit      (1001)        0 2023-07-25 16:15:23.361761 pytch-fetch-1.1.0/src/
+drwxr-xr-x   0 krit      (1000) krit      (1001)        0 2023-07-25 16:15:23.363761 pytch-fetch-1.1.0/src/pytch/
+-rw-r--r--   0 krit      (1000) krit      (1001)        0 2023-07-24 09:11:38.000000 pytch-fetch-1.1.0/src/pytch/__init__.py
+-rwxr-xr-x   0 krit      (1000) krit      (1001)     3505 2023-07-25 16:13:59.000000 pytch-fetch-1.1.0/src/pytch/__main__.py
+-rw-r--r--   0 krit      (1000) krit      (1001)    21003 2023-07-25 16:13:59.000000 pytch-fetch-1.1.0/src/pytch/art.py
+-rw-r--r--   0 krit      (1000) krit      (1001)     6373 2023-07-25 16:13:59.000000 pytch-fetch-1.1.0/src/pytch/funcs.py
+drwxr-xr-x   0 krit      (1000) krit      (1001)        0 2023-07-25 16:15:23.363761 pytch-fetch-1.1.0/src/pytch_fetch.egg-info/
+-rw-r--r--   0 krit      (1000) krit      (1001)     4220 2023-07-25 16:15:23.000000 pytch-fetch-1.1.0/src/pytch_fetch.egg-info/PKG-INFO
+-rw-r--r--   0 krit      (1000) krit      (1001)      310 2023-07-25 16:15:23.000000 pytch-fetch-1.1.0/src/pytch_fetch.egg-info/SOURCES.txt
+-rw-r--r--   0 krit      (1000) krit      (1001)        1 2023-07-25 16:15:23.000000 pytch-fetch-1.1.0/src/pytch_fetch.egg-info/dependency_links.txt
+-rw-r--r--   0 krit      (1000) krit      (1001)       46 2023-07-25 16:15:23.000000 pytch-fetch-1.1.0/src/pytch_fetch.egg-info/entry_points.txt
+-rw-r--r--   0 krit      (1000) krit      (1001)        6 2023-07-25 16:15:23.000000 pytch-fetch-1.1.0/src/pytch_fetch.egg-info/top_level.txt
```

### Comparing `pytch-fetch-1.0.1/LICENSE` & `pytch-fetch-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytch-fetch-1.0.1/PKG-INFO` & `pytch-fetch-1.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytch-fetch
-Version: 1.0.1
+Version: 1.1.0
 Summary: Pytch Yields Technical Characteristics Hastily
 Author-email: Krit Dass <dasskrit@gmail.com>
 Maintainer-email: Krit Dass <dasskrit@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Krit Dass
         
@@ -54,20 +54,21 @@
 
 <br/>
 
 ![](https://lh3.googleusercontent.com/pw/AIL4fc_Z8qwS2and18m9T_TictE9eg82GOBcLVCsdvM5rJSt1ytndTxPbYtbkLVOrwiVev-Kq19oc5ge2c-dVKi65ec8FOF5__IceoUDGE-tGR0HxpO-Wa-j8peliYgIpedMdh-3SdkB1dNd_kG6uN3YghYH=w577-h811-s-no)
 
 ## Description
 
-Pytch is a small and efficient fetch script written in Python with no dependencies. It has a relatively fast execution time of ~20ms and is tested on Python versions 3.7 or newer and PyPy (it will probably work on earlier versions but has not been tested as such). It is configured by editing its source code, though the Python used is relatively simple and readable. Rest assured, if you do not understand something, open up an issue and I will be happy to explain it to you. At its current state, Pytch only supports a few popular Linux distributions (see [this function](https://github.com/kritdass/pytch/blob/src/pytch/funcs.py#L118) for a list though most are not tested). If support is lacking for your distribution, please open up an issue and I will add support for your distribution. Pull requests are welcome and encouraged, please do not hesitate.
+Pytch is a small and efficient fetch script written in Python with no dependencies. It has a relatively fast execution time of ~20ms and is tested on Python versions 3.7 or newer and PyPy (it will probably work on earlier versions but has not been tested as such). It is configured by editing its source code, though the Python used is relatively simple and readable. Rest assured, if you do not understand something, open up an issue and I will be happy to explain it to you. At its current state, Pytch only supports a few popular Linux distributions and macOS (see [this function](https://github.com/kritdass/pytch/blob/main/src/pytch/funcs.py#L151) for a list though most are not tested). If support is lacking for your distribution, please open up an issue and I will add support for your distribution. Pull requests are welcome and encouraged, please do not hesitate.
 
 ## Installation
 
 ```
   $ pip install pytch-fetch
 ```
 You will need a [Nerd Font](https://www.nerdfonts.com/) to see the icons. I use [JetFlow](https://github.com/kritdass/JetFlow).
 
 ## Acknowlegements
 
 - [@ssleert](https://github.com/ssleert) for creating [nitch](https://github.com/ssleert/nitch), which inspired this project
-- [@dylanaraps](https://github.com/dylanaraps) for creating [neofetch](https://github.com/dylanaraps/neofetch), which was a source of reference and logos for distributions
+- [@dylanaraps](https://github.com/dylanaraps) for creating [neofetch](https://github.com/dylanaraps/neofetch), which was a source of reference and logos
+- [@willrson](https://github.com/willrson) and [@kapoorkrish](https://github.com/kapoorkrish) for helping add macOS support
```

### Comparing `pytch-fetch-1.0.1/README.md` & `pytch-fetch-1.1.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -4,20 +4,21 @@
 
 <br/>
 
 ![](https://lh3.googleusercontent.com/pw/AIL4fc_Z8qwS2and18m9T_TictE9eg82GOBcLVCsdvM5rJSt1ytndTxPbYtbkLVOrwiVev-Kq19oc5ge2c-dVKi65ec8FOF5__IceoUDGE-tGR0HxpO-Wa-j8peliYgIpedMdh-3SdkB1dNd_kG6uN3YghYH=w577-h811-s-no)
 
 ## Description
 
-Pytch is a small and efficient fetch script written in Python with no dependencies. It has a relatively fast execution time of ~20ms and is tested on Python versions 3.7 or newer and PyPy (it will probably work on earlier versions but has not been tested as such). It is configured by editing its source code, though the Python used is relatively simple and readable. Rest assured, if you do not understand something, open up an issue and I will be happy to explain it to you. At its current state, Pytch only supports a few popular Linux distributions (see [this function](https://github.com/kritdass/pytch/blob/src/pytch/funcs.py#L118) for a list though most are not tested). If support is lacking for your distribution, please open up an issue and I will add support for your distribution. Pull requests are welcome and encouraged, please do not hesitate.
+Pytch is a small and efficient fetch script written in Python with no dependencies. It has a relatively fast execution time of ~20ms and is tested on Python versions 3.7 or newer and PyPy (it will probably work on earlier versions but has not been tested as such). It is configured by editing its source code, though the Python used is relatively simple and readable. Rest assured, if you do not understand something, open up an issue and I will be happy to explain it to you. At its current state, Pytch only supports a few popular Linux distributions and macOS (see [this function](https://github.com/kritdass/pytch/blob/main/src/pytch/funcs.py#L151) for a list though most are not tested). If support is lacking for your distribution, please open up an issue and I will add support for your distribution. Pull requests are welcome and encouraged, please do not hesitate.
 
 ## Installation
 
 ```
   $ pip install pytch-fetch
 ```
 You will need a [Nerd Font](https://www.nerdfonts.com/) to see the icons. I use [JetFlow](https://github.com/kritdass/JetFlow).
 
 ## Acknowlegements
 
 - [@ssleert](https://github.com/ssleert) for creating [nitch](https://github.com/ssleert/nitch), which inspired this project
-- [@dylanaraps](https://github.com/dylanaraps) for creating [neofetch](https://github.com/dylanaraps/neofetch), which was a source of reference and logos for distributions
+- [@dylanaraps](https://github.com/dylanaraps) for creating [neofetch](https://github.com/dylanaraps/neofetch), which was a source of reference and logos
+- [@willrson](https://github.com/willrson) and [@kapoorkrish](https://github.com/kapoorkrish) for helping add macOS support
```

### Comparing `pytch-fetch-1.0.1/pyproject.toml` & `pytch-fetch-1.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pytch-fetch"
-version = "1.0.1"
+version = "1.1.0"
 description="Pytch Yields Technical Characteristics Hastily"
 readme = "README.md"
 authors = [{ name = "Krit Dass", email = "dasskrit@gmail.com" }]
 maintainers = [{ name = "Krit Dass", email = "dasskrit@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
   "Development Status :: 1 - Planning",
```

### Comparing `pytch-fetch-1.0.1/src/pytch/__main__.py` & `pytch-fetch-1.1.0/src/pytch/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python3
 
 from os import getlogin
 from argparse import ArgumentParser
 from pytch.funcs import (
+    get_output,
     get_name,
     get_uptime,
     get_shell,
     get_packages,
     get_memory,
     get_kernel,
     art,
@@ -25,37 +26,77 @@
         "-l",
         "--logo",
         metavar="DISTRO",
         dest="logo",
         help="use an alternate distribution's logo",
     )
 
-    parser.add_argument("-v", "--version", action="version", version="1.0.1")
+    parser.add_argument("-v", "--version", action="version", version="1.1.0")
 
     args = parser.parse_args()
 
     attrs = [
         {"name": "user", "value": getlogin(), "icon": "", "color": "red"},
-        {"name": "os", "value": get_name(), "icon": "", "color": "yellow"},
+        {
+            "name": "os",
+            "value": (
+                get_name()
+                if get_name() != "Darwin"
+                else get_output("sw_vers -productName").strip()
+            ),
+            "icon": "",
+            "color": "yellow",
+        },
         {"name": "kernel", "value": get_kernel(), "icon": "", "color": "green"},
         {"name": "uptime", "value": get_uptime(), "icon": "", "color": "blue"},
         {"name": "shell", "value": get_shell(), "icon": "", "color": "magenta"},
         {"name": "pkgs", "value": get_packages(), "icon": "", "color": "red"},
         {"name": "memory", "value": get_memory(), "icon": "󰍛", "color": "cyan"},
     ]
 
     print("\n" + art(args.logo or get_name())["art"])
 
     name_width = max([len(attr["name"]) for attr in attrs])
-    value_width = max([len(attr["value"]) for attr in attrs])
+    value_width = max(
+        [
+            (
+                len(attr["value"])
+                if isinstance(attr["value"], str)
+                else max([len(s) for s in attr["value"]])
+            )
+            for attr in attrs
+        ]
+    )
     gap = art(args.logo or get_name())["length"] - name_width - value_width - 8
 
     print("╭─────╮" + (" " * (name_width + value_width + gap - 2)) + "╭─╮")
 
     for attr in attrs:
+        if attr["name"] == "pkgs":
+            if len(attr["value"]) > 1:
+                for i, packager in enumerate(attr["value"]):
+                    print(
+                        "│ "
+                        + color(
+                            (" " + (attr["icon"] if not i else " ") + "  ")
+                            + (attr["name"] if not i else "")
+                            + (name_width + gap - (len(attr["name"]) if not i else 0))
+                            * " ",
+                            attr["color"],
+                        )
+                        + color(
+                            (" " * (value_width - len(packager))) + packager,
+                            attr["color"],
+                        )
+                        + " │"
+                    )
+                continue
+            else:
+                attr["value"] = attr["value"][0].split(" ")[0]
+
         print(
             "│ "
             + color(
                 (" " + attr["icon"] + "  ")
                 + attr["name"]
                 + (name_width + gap - len(attr["name"])) * " ",
                 attr["color"],
```

### Comparing `pytch-fetch-1.0.1/src/pytch/art.py` & `pytch-fetch-1.1.0/src/pytch/art.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,26 @@
 art_dict = {
-    "Ubuntu": {
+    "default": {
+        "colors": ["white", "black", "yellow"],
+        "ascii": r"""
+${c2}        #####
+${c2}       #######
+${c2}       ##${c1}O${c2}#${c1}O${c2}##
+${c2}       #${c3}#####${c2}#
+${c2}     ##${c1}##${c3}###${c1}##${c2}##
+${c2}    #${c1}##########${c2}##
+${c2}   #${c1}############${c2}##
+${c2}   #${c1}############${c2}###
+${c3}  ##${c2}#${c1}###########${c2}##${c3}#
+${c3}######${c2}#${c1}#######${c2}#${c3}######
+${c3}#######${c2}#${c1}#####${c2}#${c3}#######
+${c3}  #####${c2}#######${c3}#####
+        """,
+    },
+    "ubuntu": {
         "colors": ["red", "white"],
         "ascii": r"""
 ${c1}            .-/+oossssoo+\-.
         ´:+ssssssssssssssssss+:`
       -+ssssssssssssssssssyyssss+-
     .ossssssssssssssssss${c2}dMMMNy${c1}sssso.
    /sssssssssss${c2}hdmmNNmmyNMMMMh${c1}ssssss\
@@ -20,15 +37,15 @@
    \sssssssssss${c2}hdmNNNNmyNMMMMh${c1}ssssss/
     .ossssssssssssssssss${c2}dMMMNy${c1}sssso.
       -+sssssssssssssssss${c2}yyy${c1}ssss+-
         `:+ssssssssssssssssss+:`
             .-\+oossssoo+/-.
             """,
     },
-    "Debian": {
+    "debian": {
         "colors": ["red", "white"],
         "ascii": """
 ${c2}       _,met$$$$$gg.
     ,g$$$$$$$$$$$$$$$P.
   ,g$$P"        \"""Y$$.".
  ,$$P'              `$$$.
 ',$$P       ,ggs.     `$$b:
@@ -42,15 +59,15 @@
    `Y$$.
      `$$b.
        `Y$$b.
           `"Y$b._
               `\"""
             """,
     },
-    "Linux Mint": {
+    "linux mint": {
         "colors": ["green", "white"],
         "ascii": r"""
 ${c2}             ...-:::::-...
 ${c2}          .-MMMMMMMMMMMMMMM-.
       .-MMMM${c1}`..-:::::::-..`${c2}MMMM-.
     .:MMMM${c1}.:MMMMMMMMMMMMMMM:.${c2}MMMM:.
    -MMM${c1}-M---MMMMMMMMMMMMMMMMMMM.${c2}MMM-
@@ -66,15 +83,15 @@
    .MMM${c1}.MMMM:--------------:MMMM.${c2}MMM.
      '-MMMM${c1}.-MMMMMMMMMMMMMMM-.${c2}MMMM-'
        '.-MMMM${c1}``--:::::--``${c2}MMMM-.'
 ${c2}            '-MMMMMMMMMMMMM-'
 ${c2}               ``-:::::-``
             """,
     },
-    "PopOS": {
+    "popos": {
         "colors": ["cyan", "white"],
         "ascii": r"""
 ${c1}             /////////////
          /////////////////////
       ///////${c2}*767${c1}////////////////
     //////${c2}7676767676*${c1}//////////////
    /////${c2}76767${c1}//${c2}7676767${c1}//////////////
@@ -91,15 +108,15 @@
    //////${c2}.7676767676767676767,${c1}//////
     /////${c2}767676767676767676767${c1}/////
       ///////////////////////////
          /////////////////////
              /////////////
             """,
     },
-    "Raspbian": {
+    "raspbian": {
         "colors": ["green", "red"],
         "ascii": r"""
 ${c1}  `.::///+:/-.        --///+//-:``
  `+oooooooooooo:   `+oooooooooooo:
   /oooo++//ooooo:  ooooo+//+ooooo.
   `+ooooooo:-:oo-  +o+::/ooooooo:
    `:oooooooo+``    `.oooooooo+-
@@ -119,15 +136,15 @@
    .:::::::  -::::::::. ::::::::
     `-:::::`   ..--.`   ::::::.
       `...`  `...--..`  `...`
             .::::::::::
              `.-::::-`
             """,
     },
-    "Arch": {
+    "arch": {
         "colors": ["blue", "blue"],
         "ascii": r"""
 ${c1}                   -`
                   .o+`
                  `ooo/
                 `+oooo:
                `+oooooo:
@@ -143,15 +160,15 @@
      /ossssssss/        +ssssooo/-
    `/ossssso+/:-        -:/+osssso+-
   `+sso+:-`                 `.-/+oso:
  `++:.                           `-/+/
  .`                                 `/
             """,
     },
-    "EndeavourOS": {
+    "endeavouros": {
         "colors": ["red", "magenta", "blue"],
         "ascii": r"""
 ${c1}                     ./${c2}o${c3}.
 ${c1}                   ./${c2}sssso${c3}-
 ${c1}                 `:${c2}osssssss+${c3}-
 ${c1}               `:+${c2}sssssssssso${c3}/.
 ${c1}             `-/o${c2}ssssssssssssso${c3}/.
@@ -163,15 +180,15 @@
 ${c1}  `:////${c2}ssssssssssssssssssssssssssso${c3}+++.
 ${c1}`-////+${c2}ssssssssssssssssssssssssssso${c3}++++-
 ${c1} `..-+${c2}oosssssssssssssssssssssssso${c3}+++++/`
    ./++++++++++++++++++++++++++++++/:.
   `:::::::::::::::::::::::::------``
             """,
     },
-    "Artix": {
+    "artix": {
         "colors": ["cyan"],
         "ascii": r"""
 ${c1}                   '
                   'o'
                  'ooo'
                 'ooxoo'
                'ooxxxoo'
@@ -188,15 +205,15 @@
     'ooooxxxxxoi:::'`       .;ioxo'
    'ooooxooi::'`         .:iiixkxxo'
   'ooooi:'`                `'';ioxxo'
  'i:'`                          '':io'
 '`                                   `'
             """,
     },
-    "Manjaro": {
+    "manjaro": {
         "colors": ["green"],
         "ascii": r"""
 ${c1}██████████████████  ████████
 ██████████████████  ████████
 ██████████████████  ████████
 ██████████████████  ████████
 ████████            ████████
@@ -207,15 +224,15 @@
 ████████  ████████  ████████
 ████████  ████████  ████████
 ████████  ████████  ████████
 ████████  ████████  ████████
 ████████  ████████  ████████
             """,
     },
-    "ArcoLinux": {
+    "archlinux": {
         "colors": ["white", "blue"],
         "ascii": r"""
 ${c2}                    /-
                    ooo:
                   yoooo/
                  yooooooo
                 yooooooooo
@@ -232,15 +249,15 @@
     :ooooooooo   ${c1}/ooooooooooooooooooo${c2}
    :ooooooooo      ${c1}.-ooooooooooooooooo.${c2}
   ooooooooo-             ${c1}-ooooooooooooo.${c2}
  ooooooooo-                 ${c1}.-oooooooooo.${c2}
 ooooooooo.                     ${c1}-ooooooooo${c2}
             """,
     },
-    "Archcraft": {
+    "archcraft": {
         "colors": ["cyan"],
         "ascii": r"""
 ${c1}                   -m:
                   :NMM+      .+
                  +MMMMMo    -NMy
                 sMMMMMMMy  -MMMMh`
                yMMMMMMMMMd` oMMMMd`
@@ -255,15 +272,15 @@
     .mMMMMMm.        :hN/   `dMMMMMN- -NMMMN:
    -NMMMMMd`           -hh`  `yMMMMMN: .mMMMM/
   :NMMMMMy         `s`   :h.   oMMMMMM+ `-----
  +MMMMMMo         .dMm.   `o.   +MMMMMMo
 sMMMMMM+         .mMMMN:    :`   :NMMMMMy
             """,
     },
-    "Garuda": {
+    "garuda": {
         "colors": ["blue", "blue", "yellow", "white", "green", "blue"],
         "ascii": r"""
 ${c3}
                      .%;888:8898898:
                    x;XxXB%89b8:b8%b88:
                 .8Xxd                8X:.
               .8Xx;                    8x:.
@@ -278,15 +295,15 @@
      dxXd    dB8b8b8B8B08bB88b998888b88x.
       dxx8o                      .@@;.
         dx88                   .t@x.
           d:SS@8ba89aa67a853Sxxad.
             .d988999889889899dd.
             """,
     },
-    "NixOS": {
+    "nixos": {
         "colors": ["blue", "cyan"],
         "ascii": r"""
 ${c1}          ▗▄▄▄       ${c2}▗▄▄▄▄    ▄▄▄▖
 ${c1}          ▜███▙       ${c2}▜███▙  ▟███▛
 ${c1}           ▜███▙       ${c2}▜███▙▟███▛
 ${c1}            ▜███▙       ${c2}▜██████▛
 ${c1}     ▟█████████████████▙ ${c2}▜████▛     ${c1}▟▙
@@ -303,15 +320,15 @@
 ${c2}     ▜▛     ${c1}▟████▙ ${c2}▜████████████████▛
 ${c1}           ▟██████▙       ${c2}▜███▙
 ${c1}          ▟███▛▜███▙       ${c2}▜███▙
 ${c1}         ▟███▛  ▜███▙       ${c2}▜███▙
 ${c1}         ▝▀▀▀    ▀▀▀▀▘       ${c2}▀▀▀▘
             """,
     },
-    "Fedora": {
+    "fedora": {
         "colors": ["blue", "white"],
         "ascii": r"""
 ${c1}             .',;::::;,'.
          .';:cccccccccccc:;,.
       .;cccccccccccccccccccccc;.
     .:cccccccccccccccccccccccccc:.
   .;ccccccccccccc;${c2}.:dddl:.${c1};ccccccc;.
@@ -327,15 +344,15 @@
 cccccc;${c2}dNMWXXXWM0:${c1};cccccccccccccc:,
 cccccccc;${c2}.:odl:.${c1};cccccccccccccc:,.
 :cccccccccccccccccccccccccccc:'.
 .:cccccccccccccccccccccc:;,..
   '::cccccccccccccc::;,.
             """,
     },
-    "CentOS": {
+    "centos": {
         "colors": ["yellow", "green", "blue", "magenta"],
         "ascii": r"""
 ${c1}                 ..
                .PLTJ.
               <><><><>
      ${c2}KKSSV' 4KKK ${c1}LJ${c4} KKKL.'VSSKK
      ${c2}KKV' 4KKKKK ${c1}LJ${c4} KKKKAL 'VKK
@@ -351,15 +368,15 @@
      ${c3}KKA. 'KKKKK ${c2}LJ ${c1}KKKKK' .4KK
      ${c3}KKSSA. VKKK ${c2}LJ ${c1}KKKV .4SSKK
 ${c2}              <><><><>
                'MKKM'
                  ''
             """,
     },
-    "SUSE": {
+    "suse": {
         "colors": ["green", "white"],
         "ascii": r"""
 ${c2}           .;ldkO0000Okdl;.
        .;d00xl:^''''''^:ok00d;.
      .d00l'                'o00d.
    .d0Kd'${c1}  Okxol:;,.          ${c2}:O0d.
   .OK${c1}KKK0kOKKKKKKKKKKOxo:,      ${c2}lKO.
@@ -374,15 +391,15 @@
   'kK${c1}KKOxddxkOO00000Okxoc;''   ${c2}.dKk'
     l0Ko.                    .c00l'
      'l0Kk:.              .;xK0l'
         'lkK0xl:;,,,,;:ldO0kl'
             '^:ldxkkkkxdl:^'
             """,
     },
-    "openSUSE Tumbleweed": {
+    "opensuse tumbleweed": {
         "colors": ["green", "green"],
         "ascii": r"""
 ${c2}                                     ......
      .,cdxxxoc,.               .:kKMMMNWMMMNk:.
     cKMMN0OOOKWMMXo. ;        ;0MWk:.      .:OMMk.
   ;WMK;.       .lKMMNM,     :NMK,             .OMW;
  cMW;            'WMMMN   ,XMK,                 oMM'
@@ -392,15 +409,15 @@
  KM0               .kMM0. .dl:,..               .WMd
  .XM0.           ,OMMK,    OMMMK.              .XMK
    oWMO:.    .;xNMMk,       NNNMKl.          .xWMx
      :ONMMNXMMMKx;          .  ,xNMWKkxllox0NMWk,
          .....                    .:dOOXXKOxl,
             """,
     },
-    "openSUSE Leap": {
+    "opensuse leap": {
         "colors": ["green", "green"],
         "ascii": r"""
 ${c2}                 `-++:`
                ./oooooo/-
             `:oooooooooooo:.
           -+oooooooooooooooo+-`
        ./oooooooooooooooooooooo/-
@@ -413,15 +430,15 @@
         -/oooooo:.    ./oooooo+-
           `:+ooooo+-:+oooooo:`
              ./oooooooooo/.
                 -/oooo+:`
                   `:/.
             """,
     },
-    "RHEL": {
+    "rhel": {
         "colors": ["red"],
         "ascii": r"""
 ${c1}           .MMM..:MMMMMMM
           MMMMMMMMMMMMMMMMMM
           MMMMMMMMMMMMMMMMMMMM.
          MMMMMMMMMMMMMMMMMMMMMM
         ,MMMMMMMMMMMMMMMMMMMMMM:
@@ -436,15 +453,15 @@
     MMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMM
       MMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMM:
          MMMMMMMMMMMMMMMMMMMMMMMMMMMMMM
             `MMMMMMMMMMMMMMMMMMMMMMMM:
                 ``MMMMMMMMMMMMMMMMM'
             """,
     },
-    "Void": {
+    "void": {
         "colors": ["green", "black"],
         "ascii": r"""
 ${c1}                __.;=====;.__
             _.=+==++=++=+=+===;.
              -=+++=+===+=+=+++++=_
         .     -=:``     `--==+=++==.
        _vi,    `            --+=++++:
@@ -459,15 +476,15 @@
        +vnvnvns.           .      :=-
         -Invnvvnsi..___..=sv=.     `
           +Invnvnvnnnnnnnnvvnn;.
             ~|Invnvnvvnvvvnnv}+`
                -~|{*l}*|~
             """,
     },
-    "Gentoo": {
+    "gentoo": {
         "colors": ["magenta", "white"],
         "ascii": r"""
 ${c1}         -/oyddmdhs+:.
      -o${c2}dNMMMMMMMMNNmhy+${c1}-`
    -y${c2}NMMMMMMMMMMMNNNmmdhy${c1}+-
  `o${c2}mMMMMMMMMMMMMNmdmmmmddhhy${c1}/`
  om${c2}MMMMMMMMMMMN${c1}hhyyyo${c2}hmdddhhhd${c1}o`
@@ -482,15 +499,15 @@
 +M${c2}MMMMMMNNNNNmmmmdmNMNdso${c1}/-
 yM${c2}MNNNNNNNmmmmmNNMmhs+/${c1}-`
 /h${c2}MMNNNNNNNNMNdhs++/${c1}-`
 `/${c2}ohdmmddhys+++/:${c1}.`
   `-//////:--.
             """,
     },
-    "ChromeOS": {
+    "chromeos": {
         "colors": ["green", "red", "yellow", "blue", "white"],
         "ascii": r"""
 ${c2}            .,:loool:,.
         .,coooooooooooooc,.
      .,lllllllllllllllllllll,.
     ;ccccccccccccccccccccccccc;
 ${c1}  '${c2}ccccccccccccccccccccccccccccc.
@@ -505,8 +522,30 @@
 ${c1}  .:ccccccccllllllllo${c3}O0000000OOO,
 ${c1}    ,:ccccccccclllcd${c3}0000OOOOOOl.
 ${c1}      '::ccccccccc${c3}dOOOOOOOkx:.
 ${c1}        ..,::cccc${c3}xOOOkkko;.
 ${c1}            ..,:${c3}dOkxl:.
             """,
     },
+    "darwin": {
+        "colors": ["green", "yellow", "red", "red", "magenta", "blue"],
+        "ascii": r"""
+${c1}                    c.'
+                 ,xNMM.
+               .OMMMMo
+               lMM"
+     .;loddo:.  .olloddol;.
+   cKMMMMMMMMMMNWMMMMMMMMMM0:
+${c2} .KMMMMMMMMMMMMMMMMMMMMMMMWd.
+ XMMMMMMMMMMMMMMMMMMMMMMMX.
+${c3};MMMMMMMMMMMMMMMMMMMMMMMM:
+:MMMMMMMMMMMMMMMMMMMMMMMM:
+${c4}.MMMMMMMMMMMMMMMMMMMMMMMMX.
+ kMMMMMMMMMMMMMMMMMMMMMMMMWd.
+ ${c5}'XMMMMMMMMMMMMMMMMMMMMMMMMMMk
+  'XMMMMMMMMMMMMMMMMMMMMMMMMK.
+    ${c6}kMMMMMMMMMMMMMMMMMMMMMMd
+     ;KMMMMMMMWXXWMMMMMMMk.
+       "cooc*"    "*coo'"
+        """,
+    },
 }
```

### Comparing `pytch-fetch-1.0.1/src/pytch_fetch.egg-info/PKG-INFO` & `pytch-fetch-1.1.0/src/pytch_fetch.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytch-fetch
-Version: 1.0.1
+Version: 1.1.0
 Summary: Pytch Yields Technical Characteristics Hastily
 Author-email: Krit Dass <dasskrit@gmail.com>
 Maintainer-email: Krit Dass <dasskrit@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Krit Dass
         
@@ -54,20 +54,21 @@
 
 <br/>
 
 ![](https://lh3.googleusercontent.com/pw/AIL4fc_Z8qwS2and18m9T_TictE9eg82GOBcLVCsdvM5rJSt1ytndTxPbYtbkLVOrwiVev-Kq19oc5ge2c-dVKi65ec8FOF5__IceoUDGE-tGR0HxpO-Wa-j8peliYgIpedMdh-3SdkB1dNd_kG6uN3YghYH=w577-h811-s-no)
 
 ## Description
 
-Pytch is a small and efficient fetch script written in Python with no dependencies. It has a relatively fast execution time of ~20ms and is tested on Python versions 3.7 or newer and PyPy (it will probably work on earlier versions but has not been tested as such). It is configured by editing its source code, though the Python used is relatively simple and readable. Rest assured, if you do not understand something, open up an issue and I will be happy to explain it to you. At its current state, Pytch only supports a few popular Linux distributions (see [this function](https://github.com/kritdass/pytch/blob/src/pytch/funcs.py#L118) for a list though most are not tested). If support is lacking for your distribution, please open up an issue and I will add support for your distribution. Pull requests are welcome and encouraged, please do not hesitate.
+Pytch is a small and efficient fetch script written in Python with no dependencies. It has a relatively fast execution time of ~20ms and is tested on Python versions 3.7 or newer and PyPy (it will probably work on earlier versions but has not been tested as such). It is configured by editing its source code, though the Python used is relatively simple and readable. Rest assured, if you do not understand something, open up an issue and I will be happy to explain it to you. At its current state, Pytch only supports a few popular Linux distributions and macOS (see [this function](https://github.com/kritdass/pytch/blob/main/src/pytch/funcs.py#L151) for a list though most are not tested). If support is lacking for your distribution, please open up an issue and I will add support for your distribution. Pull requests are welcome and encouraged, please do not hesitate.
 
 ## Installation
 
 ```
   $ pip install pytch-fetch
 ```
 You will need a [Nerd Font](https://www.nerdfonts.com/) to see the icons. I use [JetFlow](https://github.com/kritdass/JetFlow).
 
 ## Acknowlegements
 
 - [@ssleert](https://github.com/ssleert) for creating [nitch](https://github.com/ssleert/nitch), which inspired this project
-- [@dylanaraps](https://github.com/dylanaraps) for creating [neofetch](https://github.com/dylanaraps/neofetch), which was a source of reference and logos for distributions
+- [@dylanaraps](https://github.com/dylanaraps) for creating [neofetch](https://github.com/dylanaraps/neofetch), which was a source of reference and logos
+- [@willrson](https://github.com/willrson) and [@kapoorkrish](https://github.com/kapoorkrish) for helping add macOS support
```

