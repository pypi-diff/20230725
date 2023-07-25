# Comparing `tmp/tockloader-1.8.0.tar.gz` & `tmp/tockloader-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tockloader-1.8.0.tar", last modified: Mon Aug 30 19:09:49 2021, max compression
+gzip compressed data, was "tockloader-1.9.0.tar", last modified: Mon Sep  5 15:26:01 2022, max compression
```

## Comparing `tockloader-1.8.0.tar` & `tockloader-1.9.0.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 bradjc     (501) staff       (20)        0 2021-08-30 19:09:49.514117 tockloader-1.8.0/
--rw-r--r--   0 bradjc     (501) staff       (20)     1084 2021-06-25 15:59:01.000000 tockloader-1.8.0/LICENSE
--rw-r--r--   0 bradjc     (501) staff       (20)      342 2021-08-30 19:09:49.513511 tockloader-1.8.0/PKG-INFO
--rw-r--r--   0 bradjc     (501) staff       (20)     8507 2021-08-30 19:08:57.000000 tockloader-1.8.0/README.md
--rw-r--r--   0 bradjc     (501) staff       (20)       38 2021-08-30 19:09:49.514394 tockloader-1.8.0/setup.cfg
--rw-r--r--   0 bradjc     (501) staff       (20)     1162 2021-08-09 21:13:54.000000 tockloader-1.8.0/setup.py
-drwxr-xr-x   0 bradjc     (501) staff       (20)        0 2021-08-30 19:09:49.487555 tockloader-1.8.0/static/
--rw-r--r--   0 bradjc     (501) staff       (20)   404986 2021-06-25 15:59:01.000000 tockloader-1.8.0/static/bscan_spi_xc7a100t.bit
-drwxr-xr-x   0 bradjc     (501) staff       (20)        0 2021-08-30 19:09:49.507683 tockloader-1.8.0/tockloader/
--rw-r--r--   0 bradjc     (501) staff       (20)       34 2021-06-25 15:59:01.000000 tockloader-1.8.0/tockloader/__init__.py
--rw-r--r--   0 bradjc     (501) staff       (20)       22 2021-08-30 19:08:33.000000 tockloader-1.8.0/tockloader/_version.py
--rw-r--r--   0 bradjc     (501) staff       (20)    10722 2021-08-09 21:13:55.000000 tockloader-1.8.0/tockloader/app_installed.py
--rw-r--r--   0 bradjc     (501) staff       (20)     2423 2021-08-09 21:13:55.000000 tockloader-1.8.0/tockloader/app_padding.py
--rw-r--r--   0 bradjc     (501) staff       (20)    16096 2021-08-11 18:39:15.000000 tockloader-1.8.0/tockloader/app_tab.py
--rw-r--r--   0 bradjc     (501) staff       (20)    20570 2021-08-26 14:03:28.000000 tockloader-1.8.0/tockloader/board_interface.py
--rw-r--r--   0 bradjc     (501) staff       (20)    54815 2021-08-11 20:38:09.000000 tockloader-1.8.0/tockloader/bootloader_serial.py
--rw-r--r--   0 bradjc     (501) staff       (20)      109 2021-08-09 21:13:54.000000 tockloader-1.8.0/tockloader/exceptions.py
--rw-r--r--   0 bradjc     (501) staff       (20)     3788 2021-08-25 20:21:46.000000 tockloader-1.8.0/tockloader/flash_file.py
--rw-r--r--   0 bradjc     (501) staff       (20)     4430 2021-08-09 21:13:55.000000 tockloader-1.8.0/tockloader/helpers.py
--rw-r--r--   0 bradjc     (501) staff       (20)    18092 2021-08-25 20:21:44.000000 tockloader-1.8.0/tockloader/jlinkexe.py
--rw-r--r--   0 bradjc     (501) staff       (20)    29587 2021-08-25 20:21:46.000000 tockloader-1.8.0/tockloader/main.py
--rw-r--r--   0 bradjc     (501) staff       (20)    14391 2021-08-25 20:21:46.000000 tockloader-1.8.0/tockloader/openocd.py
--rw-r--r--   0 bradjc     (501) staff       (20)    11071 2021-08-25 20:21:46.000000 tockloader-1.8.0/tockloader/tab.py
--rw-r--r--   0 bradjc     (501) staff       (20)    27739 2021-08-09 21:13:56.000000 tockloader-1.8.0/tockloader/tbfh.py
--rw-r--r--   0 bradjc     (501) staff       (20)    56346 2021-08-25 20:21:48.000000 tockloader-1.8.0/tockloader/tockloader.py
-drwxr-xr-x   0 bradjc     (501) staff       (20)        0 2021-08-30 19:09:49.512732 tockloader-1.8.0/tockloader.egg-info/
--rw-r--r--   0 bradjc     (501) staff       (20)      342 2021-08-30 19:09:48.000000 tockloader-1.8.0/tockloader.egg-info/PKG-INFO
--rw-r--r--   0 bradjc     (501) staff       (20)      644 2021-08-30 19:09:48.000000 tockloader-1.8.0/tockloader.egg-info/SOURCES.txt
--rw-r--r--   0 bradjc     (501) staff       (20)        1 2021-08-30 19:09:48.000000 tockloader-1.8.0/tockloader.egg-info/dependency_links.txt
--rw-r--r--   0 bradjc     (501) staff       (20)       53 2021-08-30 19:09:48.000000 tockloader-1.8.0/tockloader.egg-info/entry_points.txt
--rw-r--r--   0 bradjc     (501) staff       (20)       91 2021-08-30 19:09:48.000000 tockloader-1.8.0/tockloader.egg-info/requires.txt
--rw-r--r--   0 bradjc     (501) staff       (20)       11 2021-08-30 19:09:48.000000 tockloader-1.8.0/tockloader.egg-info/top_level.txt
+drwxr-xr-x   0 bradjc     (501) staff       (20)        0 2022-09-05 15:26:01.198732 tockloader-1.9.0/
+-rw-r--r--   0 bradjc     (501) staff       (20)     1084 2021-06-25 15:59:01.000000 tockloader-1.9.0/LICENSE
+-rw-r--r--   0 bradjc     (501) staff       (20)      342 2022-09-05 15:26:01.198215 tockloader-1.9.0/PKG-INFO
+-rw-r--r--   0 bradjc     (501) staff       (20)     8572 2022-09-01 03:52:18.000000 tockloader-1.9.0/README.md
+-rw-r--r--   0 bradjc     (501) staff       (20)       38 2022-09-05 15:26:01.198845 tockloader-1.9.0/setup.cfg
+-rw-r--r--   0 bradjc     (501) staff       (20)     1193 2022-08-31 03:03:56.000000 tockloader-1.9.0/setup.py
+drwxr-xr-x   0 bradjc     (501) staff       (20)        0 2022-09-05 15:26:01.174596 tockloader-1.9.0/static/
+-rw-r--r--   0 bradjc     (501) staff       (20)   404986 2022-07-21 17:56:06.000000 tockloader-1.9.0/static/bscan_spi_xc7a100t.bit
+drwxr-xr-x   0 bradjc     (501) staff       (20)        0 2022-09-05 15:26:01.194196 tockloader-1.9.0/tockloader/
+-rw-r--r--   0 bradjc     (501) staff       (20)       34 2021-06-25 15:59:01.000000 tockloader-1.9.0/tockloader/__init__.py
+-rw-r--r--   0 bradjc     (501) staff       (20)       22 2022-09-05 15:24:52.000000 tockloader-1.9.0/tockloader/_version.py
+-rw-r--r--   0 bradjc     (501) staff       (20)    11113 2022-08-31 21:42:45.000000 tockloader-1.9.0/tockloader/app_installed.py
+-rw-r--r--   0 bradjc     (501) staff       (20)     2423 2022-07-21 17:56:06.000000 tockloader-1.9.0/tockloader/app_padding.py
+-rw-r--r--   0 bradjc     (501) staff       (20)    16245 2022-09-02 17:06:57.000000 tockloader-1.9.0/tockloader/app_tab.py
+-rw-r--r--   0 bradjc     (501) staff       (20)    21520 2022-09-05 15:23:33.000000 tockloader-1.9.0/tockloader/board_interface.py
+-rw-r--r--   0 bradjc     (501) staff       (20)    54815 2022-07-21 17:56:06.000000 tockloader-1.9.0/tockloader/bootloader_serial.py
+-rw-r--r--   0 bradjc     (501) staff       (20)     3487 2022-09-02 17:50:30.000000 tockloader-1.9.0/tockloader/display.py
+-rw-r--r--   0 bradjc     (501) staff       (20)      109 2022-07-21 17:56:06.000000 tockloader-1.9.0/tockloader/exceptions.py
+-rw-r--r--   0 bradjc     (501) staff       (20)     3788 2022-07-21 17:56:06.000000 tockloader-1.9.0/tockloader/flash_file.py
+-rw-r--r--   0 bradjc     (501) staff       (20)     5522 2022-08-31 03:25:57.000000 tockloader-1.9.0/tockloader/helpers.py
+-rw-r--r--   0 bradjc     (501) staff       (20)    18092 2022-07-21 17:56:06.000000 tockloader-1.9.0/tockloader/jlinkexe.py
+-rw-r--r--   0 bradjc     (501) staff       (20)    31097 2022-09-01 03:56:48.000000 tockloader-1.9.0/tockloader/main.py
+-rw-r--r--   0 bradjc     (501) staff       (20)    17379 2022-08-22 17:52:34.000000 tockloader-1.9.0/tockloader/openocd.py
+-rw-r--r--   0 bradjc     (501) staff       (20)    11276 2022-09-02 17:06:57.000000 tockloader-1.9.0/tockloader/tab.py
+-rw-r--r--   0 bradjc     (501) staff       (20)    30208 2022-08-31 21:43:18.000000 tockloader-1.9.0/tockloader/tbfh.py
+-rw-r--r--   0 bradjc     (501) staff       (20)    57465 2022-09-05 15:23:33.000000 tockloader-1.9.0/tockloader/tockloader.py
+drwxr-xr-x   0 bradjc     (501) staff       (20)        0 2022-09-05 15:26:01.197492 tockloader-1.9.0/tockloader.egg-info/
+-rw-r--r--   0 bradjc     (501) staff       (20)      342 2022-09-05 15:25:59.000000 tockloader-1.9.0/tockloader.egg-info/PKG-INFO
+-rw-r--r--   0 bradjc     (501) staff       (20)      666 2022-09-05 15:26:00.000000 tockloader-1.9.0/tockloader.egg-info/SOURCES.txt
+-rw-r--r--   0 bradjc     (501) staff       (20)        1 2022-09-05 15:26:00.000000 tockloader-1.9.0/tockloader.egg-info/dependency_links.txt
+-rw-r--r--   0 bradjc     (501) staff       (20)       52 2022-09-05 15:26:00.000000 tockloader-1.9.0/tockloader.egg-info/entry_points.txt
+-rw-r--r--   0 bradjc     (501) staff       (20)      109 2022-09-05 15:26:00.000000 tockloader-1.9.0/tockloader.egg-info/requires.txt
+-rw-r--r--   0 bradjc     (501) staff       (20)       11 2022-09-05 15:26:00.000000 tockloader-1.9.0/tockloader.egg-info/top_level.txt
```

### Comparing `tockloader-1.8.0/LICENSE` & `tockloader-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tockloader-1.8.0/README.md` & `tockloader-1.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -231,14 +231,15 @@
 --------
 
 - Supported communication protocols
   - Serial over USB
   - Segger JLinkExe JTAG support
   - OpenOCD JTAG support
 - JLink RTT listener
+- JSON output using `--output-format json` for certain commands.
 
 
 Complete Install Instructions
 -----------------------------
 
 Tockloader is a Python script that is installed as an executable.
 To use Tockloader, you need python3, a couple dependencies, and
```

### Comparing `tockloader-1.8.0/setup.py` & `tockloader-1.9.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,11 +29,12 @@
     entry_points={"console_scripts": ["tockloader = tockloader.main:main"]},
     data_files=[("bitfiles", ["static/bscan_spi_xc7a100t.bit"])],
     install_requires=[
         "argcomplete >= 1.8.2",
         "colorama >= 0.3.7",
         "crcmod >= 1.7",
         "pyserial >= 3.0.1",
-        "pytoml >= 0.1.11",
+        "toml >= 0.10.2",
         "tqdm >= 4.45.0 ",
+        "questionary >= 1.10.0",
     ],
 )
```

### Comparing `tockloader-1.8.0/static/bscan_spi_xc7a100t.bit` & `tockloader-1.9.0/static/bscan_spi_xc7a100t.bit`

 * *Files identical despite different names*

### Comparing `tockloader-1.8.0/tockloader/app_installed.py` & `tockloader-1.9.0/tockloader/app_installed.py`

 * *Files 2% similar despite different names*

```diff
@@ -278,9 +278,22 @@
         out += "Total Size in Flash:   {} bytes\n".format(self.get_size())
 
         if verbose:
             out += "Address in Flash:      {:#x}\n".format(offset)
             out += textwrap.indent(str(self.tbfh), "  ")
         return out
 
+    def object(self):
+        """
+        Return a dict object containing the information about this app.
+        """
+        return {
+            "name": self.get_name(),
+            "enabled": self.tbfh.is_enabled(),
+            "sticky": self.tbfh.is_sticky(),
+            "size": self.get_size(),
+            "address": self.address,
+            "header": self.tbfh.object(),
+        }
+
     def __str__(self):
         return self.get_name()
```

### Comparing `tockloader-1.8.0/tockloader/app_padding.py` & `tockloader-1.9.0/tockloader/app_padding.py`

 * *Files identical despite different names*

### Comparing `tockloader-1.8.0/tockloader/app_tab.py` & `tockloader-1.9.0/tockloader/app_tab.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,19 @@
     App object, and the correct one for the board will be used later.
     """
 
     def __init__(self, tbfs):
         """
         Create a `TabApp` from a list of TabTbfs.
         """
+        if len(tbfs) == 0:
+            raise TockLoaderException(
+                "There must be at least one TBF to create a TabApp"
+            )
+
         self.tbfs = tbfs  # A list of TabTbfs.
 
     def get_name(self):
         """
         Return the app name.
         """
         app_names = set([tbf.tbfh.get_app_name() for tbf in self.tbfs])
```

### Comparing `tockloader-1.8.0/tockloader/board_interface.py` & `tockloader-1.9.0/tockloader/board_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,22 +142,34 @@
                 # Set to the maximum RAM size, as the LiteX bootloader will
                 # update the flash image into RAM.
                 "max_size": 0x10000000,
             },
         },
         "litex_sim": {
             "description": "LiteX SoC running on Verilated simulation",
-            "arch": "rv32i",
+            "arch": "rv32imc",
             "no_attribute_table": True,
             "flash_file": {
                 # This corresponds to the --integrated-rom-size when starting
                 # the `litex_sim` Verilated simulation.
                 "max_size": 0x00100000,
             },
         },
+        "qemu_rv32_virt": {
+            "description": "QEMU RISC-V 32 bit virt Platform",
+            "arch": "rv32imac",
+            # The QEMU-provided binary will be loaded at address 0x80000000
+            "address_translator": lambda addr: addr - 0x80000000,
+            "no_attribute_table": True,
+            "flash_file": {
+                # Size of the ROM and PROG region combined, where the resulting
+                # binary will be loaded into by QEMU:
+                "max_size": 0x00200000,
+            },
+        },
         "stm32f3discovery": {
             "description": "STM32F3-based Discovery Boards",
             "arch": "cortex-m4",
             "page_size": 2048,
             "no_attribute_table": True,
             "openocd": {
                 "prefix": 'interface hla; \
@@ -246,14 +258,25 @@
             "page_size": 4096,
             "no_attribute_table": True,
             "openocd": {
                 "prefix": "source [find interface/raspberrypi-swd.cfg]; \
                            source [find target/rp2040.cfg];",
             },
         },
+        "sma_q3": {
+            "description": "SMA Q3 smart watch (Bangle.js 2, Jazda)",
+            "arch": "cortex-m4",
+            "page_size": 4096,
+            "no_attribute_table": True,
+            "openocd": {
+                "prefix": "source [find interface/stlink.cfg]; \
+                           interface hla; \
+                           source [find target/nrf52.cfg];",
+            },
+        },
     }
 
     def __init__(self, args):
         self.args = args
 
         # These settings allow tockloader to correctly communicate with and
         # program the attached hardware platform. They can be set through the
```

### Comparing `tockloader-1.8.0/tockloader/bootloader_serial.py` & `tockloader-1.9.0/tockloader/bootloader_serial.py`

 * *Files identical despite different names*

### Comparing `tockloader-1.8.0/tockloader/flash_file.py` & `tockloader-1.9.0/tockloader/flash_file.py`

 * *Files identical despite different names*

### Comparing `tockloader-1.8.0/tockloader/helpers.py` & `tockloader-1.9.0/tockloader/helpers.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 users in a nice way.
 """
 
 import argparse
 import sys
 
 import colorama
+import questionary
 
 
 def set_terminal_title(title):
     if sys.stdout.isatty():
         sys.stdout.write(colorama.ansi.set_title(title))
         sys.stdout.flush()
 
@@ -23,15 +24,15 @@
     if info.manufacturer and info.manufacturer != "n/a":
         extras.append(info.manufacturer)
     if info.name and info.name != "n/a":
         extras.append(info.name)
     if info.description and info.description != "n/a":
         extras.append(info.description)
     # if info.hwid and info.hwid != 'n/a':
-    # 	extras.append(info.hwid)
+    #  extras.append(info.hwid)
     if info.product and info.product != "n/a":
         if info.product != info.description:
             extras.append(info.product)
     title = " : ".join(extras)
 
     set_terminal_title(title)
 
@@ -39,14 +40,50 @@
 def set_terminal_title_from_port(port):
     """
     Set the title of the user's terminal for Tockloader.
     """
     set_terminal_title("Tockloader : {}".format(port))
 
 
+def menu_new(options, *, return_type, default_index=None, prompt="", title=""):
+    """
+    Present an interactive menu of choices to a user.
+
+    `options` should be a like-list object whose iterated objects can be coerced
+    into strings.
+
+    `return_type` must be set to one of:
+      - "index" - for the index into the options array
+      - "value" - for the option value chosen
+
+    `default_index` is the index to present as the default value (what happens
+    if the user simply presses enter). Passing `None` disables default
+    selection.
+    """
+
+    prompt_to_show = prompt
+    if len(title) > len(prompt_to_show):
+        prompt_to_show = title
+
+    default = None
+    if default_index:
+        default = options[default_index]
+
+    response = questionary.select(
+        prompt_to_show, choices=options, default=default, qmark=""
+    ).ask()
+
+    if return_type == "index":
+        return options.index(response)
+    elif return_type == "value":
+        return response
+    else:
+        raise NotImplementedError("Menu caller asked for bad return_type")
+
+
 def menu(options, *, return_type, default_index=0, prompt="Which option? ", title=""):
     """
     Present a menu of choices to a user
 
     `options` should be a like-list object whose iterated objects can be coerced
     into strings.
```

### Comparing `tockloader-1.8.0/tockloader/jlinkexe.py` & `tockloader-1.9.0/tockloader/jlinkexe.py`

 * *Files identical despite different names*

### Comparing `tockloader-1.8.0/tockloader/main.py` & `tockloader-1.9.0/tockloader/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -323,15 +323,15 @@
     for tab in tabs:
         # Print the basic information that is true about the TAB and all
         # contained TBF binaries.
         print(tab)
 
         # Ask the user if they want to see more detail about a certain TBF.
         tbf_names = tab.get_tbf_names()
-        index = helpers.menu(
+        index = helpers.menu_new(
             tbf_names + ["None"],
             return_type="index",
             title="Which TBF to inspect further?",
         )
         if index < len(tbf_names):
             print("")
             print("{}:".format(tbf_names[index]))
@@ -563,14 +563,24 @@
     )
     parent_channel.add_argument(
         "--no-bootloader-entry",
         action="store_true",
         help="Tell Tockloader to assume the bootloader is already active.",
     )
 
+    # Parser for all output formatting related flags shared by multiple
+    # commands.
+    parent_format = argparse.ArgumentParser(add_help=False)
+    parent_format.add_argument(
+        "--output-format",
+        help="Address where apps are located",
+        choices=["terminal", "json"],
+        default="terminal",
+    )
+
     # Support multiple commands for this tool
     subparser = parser.add_subparsers(title="Commands", metavar="")
 
     # Command Groups
     #
     # Python argparse doesn't support grouping commands in subparsers as of
     # January 2021 :(. The best we can do now is order them logically.
@@ -595,14 +605,20 @@
     listen.add_argument("--rtt", action="store_true", help="Use Segger RTT to listen.")
     listen.add_argument(
         "--board",
         default=None,
         help="Specify the board that is being read from. Only used with --rtt.",
     )
     listen.add_argument(
+        "--jlink", action="store_true", help="Use JLinkExe. Only used with --rtt."
+    )
+    listen.add_argument(
+        "--openocd", action="store_true", help="Use OpenOCD. Only used with --rtt."
+    )
+    listen.add_argument(
         "--jlink-cmd", help="The JLinkExe binary to invoke. Only used with --rtt."
     )
     listen.add_argument(
         "--jlink-rtt-cmd",
         help="The JLinkRTTClient binary to invoke. Only used with --rtt.",
     )
     listen.add_argument(
@@ -616,14 +632,37 @@
         help="The JLink speed to pass to JLinkExe. Only used with --rtt.",
     )
     listen.add_argument(
         "--jlink-if",
         default="swd",
         help="The interface type to pass to JLinkExe. Only used with --rtt.",
     )
+    listen.add_argument(
+        "--openocd-board",
+        help="The cfg file in OpenOCD `board` folder. Only used with --rtt.",
+    )
+    listen.add_argument(
+        "--openocd-cmd",
+        default="openocd",
+        help="The openocd binary to invoke. Only used with --rtt.",
+    )
+    listen.add_argument(
+        "--openocd-options",
+        default=[],
+        help="Tockloader-specific flags to direct how Tockloader uses OpenOCD. Only used with --rtt.",
+        nargs="*",
+    )
+    listen.add_argument(
+        "--openocd-commands",
+        default={},
+        type=lambda kv: kv.split("=", 1),
+        action=helpers.ListToDictAction,
+        help='Directly specify which OpenOCD commands to use for "program", "read", or "erase" actions. Example: "program=flash write_image erase {{binary}} {address:#x};verify_image {{binary}} {address:#x};" Only used with --rtt.',
+        nargs="*",
+    )
     listen.set_defaults(func=command_listen)
 
     install = subparser.add_parser(
         "install",
         parents=[parent, parent_apps, parent_channel],
         help="Install apps on the board",
     )
@@ -660,15 +699,15 @@
         help="Remove an already flashed app",
     )
     uninstall.set_defaults(func=command_uninstall)
     uninstall.add_argument("name", help="The name of the app(s) to remove", nargs="*")
 
     listcmd = subparser.add_parser(
         "list",
-        parents=[parent, parent_apps, parent_channel],
+        parents=[parent, parent_apps, parent_channel, parent_format],
         help="List the apps installed on the board",
     )
     listcmd.set_defaults(func=command_list)
     listcmd.add_argument(
         "--verbose", "-v", help="Print more information", action="store_true"
     )
     listcmd.add_argument(
@@ -676,15 +715,15 @@
         "-q",
         help="Print just a list of application names",
         action="store_true",
     )
 
     info = subparser.add_parser(
         "info",
-        parents=[parent, parent_apps, parent_channel],
+        parents=[parent, parent_apps, parent_channel, parent_format],
         help="Verbose information about the connected board",
     )
     info.set_defaults(func=command_info)
 
     eraseapps = subparser.add_parser(
         "erase-apps",
         parents=[parent, parent_apps, parent_channel],
@@ -791,15 +830,15 @@
     dump_flash_page.set_defaults(func=command_dump_flash_page)
     dump_flash_page.add_argument(
         "page", help="The number of the page to read", type=lambda x: int(x, 0)
     )
 
     listattributes = subparser.add_parser(
         "list-attributes",
-        parents=[parent, parent_channel],
+        parents=[parent, parent_channel, parent_format],
         help="List attributes stored on the board",
     )
     listattributes.set_defaults(func=command_list_attributes)
 
     setattribute = subparser.add_parser(
         "set-attribute",
         parents=[parent, parent_channel],
```

### Comparing `tockloader-1.8.0/tockloader/openocd.py` & `tockloader-1.9.0/tockloader/openocd.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,16 +7,18 @@
 way. Note, I just made up the string (flag) names; they are not passed to
 OpenOCD directly.
 """
 
 import logging
 import platform
 import shlex
+import socket
 import subprocess
 import tempfile
+import time
 
 from .board_interface import BoardInterface
 from .exceptions import TockLoaderException
 
 # global static variable for collecting temp files for Windows
 collect_temp_files = []
 
@@ -84,21 +86,22 @@
             self._configure_from_known_boards()
 
         if self.openocd_board == None:
             raise TockLoaderException(
                 "Unknown OpenOCD board name. You must pass --openocd-board."
             )
 
-    def _run_openocd_commands(self, commands, binary, write=True):
+    def _gather_openocd_cmdline(self, commands, binary, write=True, exit=True):
         """
-        - `commands`: String of openocd commands. Use {binary} for where the name
+        - `commands`: List of openocd commands. Use {binary} for where the name
           of the binary file should be substituted.
         - `binary`: A bytes() object that will be used to write to the board.
         - `write`: Set to true if the command writes binaries to the board. Set
           to false if the command will read bits from the board.
+        - `exit`: When `True`, openocd will exit after executing commands.
         """
 
         # in Windows, you can't mark delete bc they delete too fast
         delete = platform.system() != "Windows"
         if self.args.debug:
             delete = False
 
@@ -114,16 +117,18 @@
             if platform.system() == "Windows":
                 # For Windows, forward slashes need to be escaped
                 temp_bin.name = temp_bin.name.replace("\\", "\\\\\\")
                 # For Windows, files need to be manually deleted
                 global collect_temp_files
                 collect_temp_files += [temp_bin.name]
 
-            # Update the command with the name of the binary file
-            commands = commands.format(binary=temp_bin.name)
+            # Update the commands with the name of the binary file
+            commands = [command.format(binary=temp_bin.name) for command in commands]
+        else:
+            temp_bin = None
 
         # Create the actual openocd command and run it. All of this can be
         # customized if needed for an unusual board.
 
         # Defaults.
         prefix = ""
         source = "source [find board/{board}];".format(board=self.openocd_board)
@@ -139,24 +144,38 @@
             source = ""
         if "noreset" in self.openocd_options:
             cmd_prefix = "init; halt;"
         if "nocmdprefix" in self.openocd_options:
             cmd_prefix = ""
         if "resume" in self.openocd_options:
             cmd_suffix = "soft_reset_halt; resume;"
+        if exit:
+            cmd_suffix += "exit"
 
-        openocd_command = '{openocd_cmd} -c "{prefix} {source} {cmd_prefix} {cmd} {cmd_suffix} exit" --debug'.format(
-            openocd_cmd=self.openocd_cmd,
+        command_param = "{prefix} {source} {cmd_prefix} {cmd} {cmd_suffix}".format(
             prefix=prefix,
             source=source,
             cmd_prefix=cmd_prefix,
-            cmd=commands,
+            cmd="; ".join(commands),
             cmd_suffix=cmd_suffix,
         )
 
+        return (
+            "{openocd_cmd} -c {cmd} --debug".format(
+                openocd_cmd=self.openocd_cmd,
+                cmd=shlex.quote(command_param),
+            ),
+            temp_bin,
+        )
+
+    def _run_openocd_commands(self, commands, binary, write=True):
+        openocd_command, temp_bin = self._gather_openocd_cmdline(
+            [commands], binary, write
+        )
+
         logging.debug('Running "{}".'.format(openocd_command.replace("$", "\$")))
 
         def print_output(subp):
             response = ""
             if subp.stdout:
                 response += subp.stdout.decode("utf-8")
             if subp.stderr:
@@ -355,7 +374,79 @@
             or self.arch == None
             or self.openocd_board == "cortex-m0"
             or self.page_size == 0
         ):
             raise TockLoaderException(
                 "Could not determine the current board or arch or openocd board name"
             )
+
+    def run_terminal(self):
+        self.open_link_to_board()
+        logging.status("Starting OpenOCD RTT connection.")
+        openocd_command, _ = self._gather_openocd_cmdline(
+            [
+                'rtt setup 0x20000000 65536 "SEGGER RTT"',
+                "init",
+                "rtt start",
+                "rtt server start 9999 0",
+                "reset run",
+            ],
+            None,
+            exit=False,
+        )
+
+        logging.debug('Running "{}".'.format(openocd_command.replace("$", "\$")))
+
+        cleanup = []
+        try:
+            # This won't print messages from OpenOCD,
+            # to avoid interfering with the console.
+            ocd_p = subprocess.Popen(
+                shlex.split(openocd_command),
+                stdout=subprocess.DEVNULL,
+                stderr=subprocess.DEVNULL,
+            )
+            cleanup.append(ocd_p.wait)
+            cleanup.append(ocd_p.kill)
+
+            listener = socket.socket()
+            MAX_TRIES = 3
+            for i in range(MAX_TRIES):
+                # Delay to give the connection time to start before running
+                # the RTT listener.
+                time.sleep(1)
+                if ocd_p.poll():
+                    return
+                try:
+                    listener.connect(("127.0.0.1", 9999))
+                    logging.debug("Connecting to OpenOCD, attempt {}.".format(i))
+                    break
+                except ConnectionRefusedError:
+                    if i == MAX_TRIES - 1:
+                        raise
+
+            cleanup.append(listener.close)
+            logging.status("Listening for messages.")
+
+            out = listener.makefile(mode="rb")
+            cleanup.append(out.close)
+            for out_line in iter(out.readline, ""):
+                l = out_line.decode("utf-8", errors="replace")
+                if not l.startswith("###RTT Client: *"):
+                    print(l, end="")
+        finally:
+            logging.status("Stopping")
+            for f in reversed(cleanup):
+                f()
+
+            openocd_command, _ = self._gather_openocd_cmdline(
+                [
+                    "init",
+                    "reset halt",
+                ],
+                None,
+            )
+            subprocess.run(
+                shlex.split(openocd_command),
+                stdout=subprocess.DEVNULL,
+                stderr=subprocess.DEVNULL,
+            )
```

### Comparing `tockloader-1.8.0/tockloader/tab.py` & `tockloader-1.9.0/tockloader/tab.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import shutil
 import struct
 import tarfile
 import tempfile
 import textwrap
 import urllib.request
 
-import pytoml
+import toml
 
 from .app_tab import TabApp
 from .app_tab import TabTbf
 from .exceptions import TockLoaderException
 from .tbfh import TBFHeader
 
 
@@ -49,15 +49,16 @@
                     logging.error("  - A temporary file could not be created.")
                     logging.error("  - Untarring the TAB failed.")
                     logging.error("Exception: {}".format(e))
                 raise TockLoaderException("Could not download .tab file.")
 
     def extract_app(self, arch):
         """
-        Return a `TabApp` object from this TAB. You must specify the desired MCU
+        Return a `TabApp` object from this TAB, or `None` if the requested
+        architecture is not present in the TAB. You must specify the desired MCU
         architecture so the correct App object can be retrieved. Note that an
         architecture may have multiple TBF files if the app is compiled for a
         fixed address, and multiple fixed address versions are included in the
         TAB.
         """
         # Find all filenames that start with the architecture name.
         matching_tbf_filenames = []
@@ -65,14 +66,18 @@
         # A TBF name is in the format: <architecture>.<anything>.tbf
         for contained_file in contained_files:
             name_pieces = contained_file.split(".")
             if len(name_pieces) >= 2 and name_pieces[-1] == "tbf":
                 if name_pieces[0] == arch:
                     matching_tbf_filenames.append(contained_file)
 
+        if len(matching_tbf_filenames) == 0:
+            # No match for this architecture! Just return None.
+            return None
+
         # Get all of the TBF headers and app binaries to create a TabApp.
         tbfs = []
         for tbf_filename in matching_tbf_filenames:
             binary_tarinfo = self.tab.getmember(tbf_filename)
             binary = self.tab.extractfile(binary_tarinfo).read()
 
             # First get the TBF header from the correct binary in the TAB
@@ -258,15 +263,15 @@
         # Use cached value.
         if hasattr(self, "metadata"):
             return self.metadata
 
         # Otherwise parse f.toml file.
         metadata_tarinfo = self.tab.getmember("metadata.toml")
         metadata_str = self.tab.extractfile(metadata_tarinfo).read().decode("utf-8")
-        self.metadata = pytoml.loads(metadata_str)
+        self.metadata = toml.loads(metadata_str)
         return self.metadata
 
     def _get_metadata_key(self, key):
         """
         Return the value for a specific key from the metadata file.
         """
         metadata = self._parse_metadata()
```

### Comparing `tockloader-1.8.0/tockloader/tbfh.py` & `tockloader-1.9.0/tockloader/tbfh.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,14 +62,23 @@
             "protected_size", self.protected_size, self.protected_size
         )
         out += "  {:<20}: {:>10} {:>#12x}\n".format(
             "minimum_ram_size", self.minimum_ram_size, self.minimum_ram_size
         )
         return out
 
+    def object(self):
+        return {
+            "type": "main",
+            "id": self.TLVID,
+            "init_fn_offset": self.init_fn_offset,
+            "protected_size": self.protected_size,
+            "minimum_ram_size": self.minimum_ram_size,
+        }
+
 
 class TBFTLVWriteableFlashRegions(TBFTLV):
     TLVID = 0x02
 
     def __init__(self, buffer):
         self.valid = False
 
@@ -93,14 +102,25 @@
         )
         for i, wfr in enumerate(self.writeable_flash_regions):
             out += "  writeable flash region {}\n".format(i)
             out += "    {:<18}: {:>8} {:>#12x}\n".format("offset", wfr[0], wfr[0])
             out += "    {:<18}: {:>8} {:>#12x}\n".format("length", wfr[1], wfr[1])
         return out
 
+    def object(self):
+        out = {
+            "type": "writeable_flash_regions",
+            "id": self.HEADER_TYPE_WRITEABLE_FLASH_REGIONS,
+            "wfrs": [],
+        }
+
+        for wfr in self.writeable_flash_regions:
+            out["wfrs"].append({"offset": wfr[0], "length": wfr[1]})
+        return out
+
 
 class TBFTLVPackageName(TBFTLV):
     TLVID = 0x03
 
     def __init__(self, buffer):
         self.package_name = buffer.decode("utf-8")
         self.valid = True
@@ -116,14 +136,21 @@
         return out
 
     def __str__(self):
         out = "TLV: Package Name ({})\n".format(self.TLVID)
         out += "  {:<20}: {}\n".format("package_name", self.package_name)
         return out
 
+    def object(self):
+        return {
+            "type": "name",
+            "id": self.TLVID,
+            "package_name": self.package_name,
+        }
+
 
 class TBFTLVPicOption1(TBFTLV):
     TLVID = 0x04
 
     def __init__(self, buffer):
         self.valid = False
 
@@ -160,14 +187,30 @@
         )
 
     def __str__(self):
         out = "TLV: PIC Option 1 ({})\n".format(self.TLVID)
         out += "  {:<20}: {}\n".format("PIC", "C Style")
         return out
 
+    def object(self):
+        return {
+            "type": "pic_option_1",
+            "id": self.TLVID,
+            "text_offset": self.text_offset,
+            "data_offset": self.data_offset,
+            "data_size": self.data_size,
+            "bss_memory_offset": self.bss_memory_offset,
+            "bss_size": self.bss_size,
+            "relocation_data_offset": self.relocation_data_offset,
+            "relocation_data_size": self.relocation_data_size,
+            "got_offset": self.got_offset,
+            "got_size": self.got_size,
+            "minimum_stack_length": self.minimum_stack_length,
+        }
+
 
 class TBFTLVFixedAddress(TBFTLV):
     TLVID = 0x05
 
     def __init__(self, buffer):
         self.valid = False
 
@@ -188,14 +231,22 @@
             "fixed_address_ram", self.fixed_address_ram, self.fixed_address_ram
         )
         out += "  {:<20}: {:>10} {:>#12x}\n".format(
             "fixed_address_flash", self.fixed_address_flash, self.fixed_address_flash
         )
         return out
 
+    def object(self):
+        return {
+            "type": "fixed_addresses",
+            "id": self.TLVID,
+            "fixed_address_ram": self.fixed_address_ram,
+            "fixed_address_flash": self.fixed_address_flash,
+        }
+
 
 class TBFTLVKernelVersion(TBFTLV):
     TLVID = 0x08
 
     def __init__(self, buffer):
         self.valid = False
 
@@ -213,14 +264,22 @@
         out += "  {:<20}: {}\n".format("kernel_major", self.kernel_major)
         out += "  {:<20}: {}\n".format("kernel_minor", self.kernel_minor)
         out += "  {:<20}: ^{}.{}\n".format(
             "kernel version", self.kernel_major, self.kernel_minor
         )
         return out
 
+    def object(self):
+        return {
+            "type": "kernel_version",
+            "id": self.TLVID,
+            "kernel_major": self.kernel_major,
+            "kernel_minor": self.kernel_minor,
+        }
+
 
 class TBFHeader:
     """
     Tock Binary Format header class. This can parse TBF encoded headers and
     return various properties of the application.
     """
 
@@ -765,14 +824,35 @@
         )
 
         for tlv in self.tlvs:
             out += str(tlv)
 
         return out
 
+    def object(self):
+        out = {"version": self.version}
+
+        # Special case version 1. However, at this point (May 2020), I would be
+        # shocked if this ever gets run on a version 1 TBFH.
+        if self.version == 1:
+            for k, v in sorted(self.fields.items()):
+                out[k] = v
+            return out
+
+        out["header_size"] = self.fields["header_size"]
+        out["total_size"] = self.fields["total_size"]
+        out["checksum"] = self.fields["checksum"]
+        out["flags"] = self.fields["flags"]
+
+        out["tlvs"] = []
+        for tlv in self.tlvs:
+            out["tlvs"].append(tlv.object())
+
+        return out
+
 
 class TBFHeaderPadding(TBFHeader):
     """
     TBF Header that is only padding between apps. Since apps are packed as
     linked-list, this allows apps to be pushed to later addresses while
     preserving the linked-list structure.
     """
```

### Comparing `tockloader-1.8.0/tockloader/tockloader.py` & `tockloader-1.9.0/tockloader/tockloader.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 import os
 import platform
 import string
 import textwrap
 import time
 
 from . import helpers
+from . import display
 from .app_installed import InstalledApp
 from .app_padding import PaddingApp
 from .app_padding import InstalledPaddingApp
 from .app_tab import TabApp
 from .board_interface import BoardInterface
 from .bootloader_serial import BootloaderSerial
 from .exceptions import TockLoaderException
@@ -103,14 +104,15 @@
             },
             "hifive1": {"start_address": 0x20430000},
             "hifive1b": {"start_address": 0x20040000},
             "litex_arty": {"start_address": 0x41000000},
             "litex_sim": {"start_address": 0x00080000},
             "nucleof4": {"start_address": 0x08040000},
             "microbit_v2": {"start_address": 0x00040000},
+            "qemu_rv32_virt": {"start_address": 0x80100000},
             "stm32f3discovery": {"start_address": 0x08020000},
             "stm32f4discovery": {"start_address": 0x08040000},
             "raspberry_pi_pico": {"start_address": 0x10020000},
         },
     }
 
     def __init__(self, args):
@@ -245,15 +247,21 @@
         """
         # Enter bootloader mode to get things started
         with self._start_communication_with_board():
 
             # Get all apps based on their header
             apps = self._extract_all_app_headers(verbose)
 
-            self._print_apps(apps, verbose, quiet)
+            if self.args.output_format == "json":
+                displayer = display.JSONDisplay()
+            else:
+                displayer = display.HumanReadableDisplay()
+
+            displayer.list_apps(apps, verbose, quiet)
+            print(displayer.get())
 
     def install(self, tabs, replace="yes", erase=False, sticky=False):
         """
         Add or update TABs on the board.
 
         - `replace` can be "yes", "no", or "only"
         - `erase` if true means erase all other apps before installing
@@ -522,15 +530,23 @@
         with self._start_communication_with_board():
 
             if not self._bootloader_is_present():
                 raise TockLoaderException(
                     "No bootloader found! That means there is nowhere for attributes to go."
                 )
 
-            self._print_attributes(self.channel.get_all_attributes())
+            attributes = self.channel.get_all_attributes()
+
+            if self.args.output_format == "json":
+                displayer = display.JSONDisplay()
+            else:
+                displayer = display.HumanReadableDisplay()
+
+            displayer.list_attributes(attributes)
+            print(displayer.get())
 
     def set_attribute(self, key, value):
         """
         Change an attribute stored on the board.
         """
 
         # Enter bootloader mode to get things started
@@ -591,33 +607,35 @@
     def info(self):
         """
         Print all info about this board.
         """
         # Enter bootloader mode to get things started
         with self._start_communication_with_board():
 
+            if self.args.output_format == "json":
+                displayer = display.JSONDisplay()
+            else:
+                displayer = display.HumanReadableDisplay(show_headers=True)
+
             # Print all apps
-            print("Apps:")
             apps = self._extract_all_app_headers()
-            self._print_apps(apps, True, False)
+            displayer.list_apps(apps, True, False)
 
             if self._bootloader_is_present():
                 # Print all attributes
-                print("Attributes:")
                 attributes = self.channel.get_all_attributes()
-                self._print_attributes(attributes)
-                print("")
+                displayer.list_attributes(attributes)
 
                 # Show bootloader version
                 version = self.channel.get_bootloader_version()
                 if version == None:
                     version = "unknown"
-                print("Bootloader version: {}".format(version))
-            else:
-                print("No bootloader.")
+                displayer.bootloader_version(version)
+
+            print(displayer.get())
 
     def dump_flash_page(self, page_num):
         """
         Print one page of flash contents.
         """
         with self._start_communication_with_board():
             page_size = self.channel.get_page_size()
@@ -654,15 +672,19 @@
         to have been called at this point.
         """
         # By default, we use the serial connection and serial terminal. However,
         # tockloader supports other terminals, and we choose the correct one
         # here. There is no need to save the channel, since
         # `channel.run_terminal()` never returns.
         if self.args.rtt:
-            channel = JLinkExe(self.args)
+            if self.args.openocd:
+                channel = OpenOCD(self.args)
+            else:
+                channel = JLinkExe(self.args)
+
         else:
             channel = BootloaderSerial(self.args)
             channel.open_link_to_board(listen=True)
 
         channel.run_terminal()
 
     def print_known_boards(self):
@@ -916,25 +938,38 @@
         # solution. An interested contributor could probably find many
         # improvements and optimizations.
         #
 
         # Get where the apps live in flash.
         address = self._get_apps_start_address()
 
-        # First, we are going to split the work into two cases: do we have any
-        # app that is compiled for a fixed address, or not? Likely, there won't
-        # be platforms that have mixed fixed address apps and PIC apps. This
-        # split simplifies things, but a better algorithm would not have this
-        # split.
-        is_fixed_address_app = False
-        for app in apps:
-            if app.has_fixed_addresses():
-                is_fixed_address_app = True
+        # First, we are going to split the work into three cases:
+        #
+        # 1. All apps are fixed address, meaning they have to be loaded at very
+        #    specific addresses.
+        # 2. All apps are position independent, and can be put at any address.
+        # 3. There is a mix of fixed address and position independent apps.
+        #
+        # Then we can handle organizing the apps in each case separately.
+
+        # Default to mixed, and only if all are one type be specific.
+        app_position_scenario = "mixed"
+        if all(map(lambda x: x.has_fixed_addresses(), apps)):
+            app_position_scenario = "fixed"
+        elif all(map(lambda x: not x.has_fixed_addresses(), apps)):
+            app_position_scenario = "independent"
+
+        if app_position_scenario == "mixed":
+            # Currently unsupported. This could (should?) be added in the
+            # future.
+            raise TockLoaderException(
+                "Mixing fixed address and position-independent apps is currently unsupported."
+            )
 
-        if is_fixed_address_app:
+        if app_position_scenario == "fixed":
             #
             # This is the fixed addresses case
             #
 
             def brad_sort(slices):
                 """
                 Get an ordering of apps where the fixed start addresses are
@@ -1270,14 +1305,20 @@
                     )
                 )
                 continue
 
             # This app is good to install, continue the process.
 
             app = tab.extract_app(arch)
+            if app == None:
+                raise TockLoaderException(
+                    "Unable to locate a valid application binary matching the target architecture ({})".format(
+                        arch
+                    )
+                )
 
             # Enforce other sizing constraints here.
             app.set_size_constraint(self.app_settings["size_constraint"])
 
             apps.append(app)
 
         if len(apps) == 0:
@@ -1365,21 +1406,7 @@
 
             if len(apps) == 0:
                 logging.info("No found apps.")
 
         else:
             # In quiet mode just show the names.
             print(" ".join([app.get_name() for app in apps]))
-
-    def _print_attributes(self, attributes):
-        """
-        Print the list of attributes in the bootloader.
-        """
-        for index, attribute in enumerate(attributes):
-            if attribute:
-                print(
-                    "{:02d}: {:>8} = {}".format(
-                        index, attribute["key"], attribute["value"]
-                    )
-                )
-            else:
-                print("{:02d}:".format(index))
```

### Comparing `tockloader-1.8.0/tockloader.egg-info/SOURCES.txt` & `tockloader-1.9.0/tockloader.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 tockloader/__init__.py
 tockloader/_version.py
 tockloader/app_installed.py
 tockloader/app_padding.py
 tockloader/app_tab.py
 tockloader/board_interface.py
 tockloader/bootloader_serial.py
+tockloader/display.py
 tockloader/exceptions.py
 tockloader/flash_file.py
 tockloader/helpers.py
 tockloader/jlinkexe.py
 tockloader/main.py
 tockloader/openocd.py
 tockloader/tab.py
```

