# Comparing `tmp/gpt_automation-0.1.1.tar.gz` & `tmp/gpt_automation-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt_automation-0.1.1.tar", last modified: Mon Jul 24 23:50:08 2023, max compression
+gzip compressed data, was "gpt_automation-0.1.2.tar", last modified: Tue Jul 25 00:12:31 2023, max compression
```

## Comparing `gpt_automation-0.1.1.tar` & `gpt_automation-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 23:50:08.450670 gpt_automation-0.1.1/
--rw-rw-rw-   0        0        0    11560 2023-07-24 23:26:12.000000 gpt_automation-0.1.1/LICENSE
--rw-rw-rw-   0        0        0       50 2023-07-24 23:26:12.000000 gpt_automation-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0    16303 2023-07-24 23:50:08.450670 gpt_automation-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2785 2023-07-24 23:26:12.000000 gpt_automation-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-24 23:50:08.435117 gpt_automation-0.1.1/gpt_automation.egg-info/
--rw-rw-rw-   0        0        0    16303 2023-07-24 23:50:08.000000 gpt_automation-0.1.1/gpt_automation.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      359 2023-07-24 23:50:08.000000 gpt_automation-0.1.1/gpt_automation.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 23:50:08.000000 gpt_automation-0.1.1/gpt_automation.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-07-24 23:50:08.000000 gpt_automation-0.1.1/gpt_automation.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       56 2023-07-24 23:50:08.000000 gpt_automation-0.1.1/gpt_automation.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 23:50:08.000000 gpt_automation-0.1.1/gpt_automation.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      516 2023-07-24 23:49:48.000000 gpt_automation-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0      421 2023-07-24 23:50:08.450670 gpt_automation-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      247 2023-07-24 23:49:11.000000 gpt_automation-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-24 23:50:08.419433 gpt_automation-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-24 23:50:08.450670 gpt_automation-0.1.1/src/sample_config/
--rw-rw-rw-   0        0        0      159 2023-07-24 23:26:12.000000 gpt_automation-0.1.1/src/sample_config/black_list.txt
--rw-rw-rw-   0        0        0       36 2023-07-24 23:26:12.000000 gpt_automation-0.1.1/src/sample_config/white_list.txt
+drwxrwxrwx   0        0        0        0 2023-07-25 00:12:31.357181 gpt_automation-0.1.2/
+-rw-rw-rw-   0        0        0    11560 2023-07-24 23:26:12.000000 gpt_automation-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0       61 2023-07-25 00:04:10.000000 gpt_automation-0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0    16303 2023-07-25 00:12:31.357181 gpt_automation-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2785 2023-07-24 23:26:12.000000 gpt_automation-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 00:12:31.328940 gpt_automation-0.1.2/gpt_automation/
+-rw-rw-rw-   0        0        0        0 2023-07-25 00:01:46.000000 gpt_automation-0.1.2/gpt_automation/__init__.py
+-rw-rw-rw-   0        0        0     1608 2023-07-24 23:26:12.000000 gpt_automation-0.1.2/gpt_automation/ignore_walk.py
+-rw-rw-rw-   0        0        0     3556 2023-07-25 00:05:17.000000 gpt_automation-0.1.2/gpt_automation/main.py
+-rw-rw-rw-   0        0        0     1613 2023-07-25 00:05:54.000000 gpt_automation-0.1.2/gpt_automation/project_info.py
+drwxrwxrwx   0        0        0        0 2023-07-25 00:12:31.357181 gpt_automation-0.1.2/gpt_automation/sample_config/
+-rw-rw-rw-   0        0        0      123 2023-07-25 00:12:11.000000 gpt_automation-0.1.2/gpt_automation/sample_config/black_list.txt
+-rw-rw-rw-   0        0        0     1123 2023-07-25 00:10:12.000000 gpt_automation-0.1.2/gpt_automation/sample_config/white_list.txt
+drwxrwxrwx   0        0        0        0 2023-07-25 00:12:31.357181 gpt_automation-0.1.2/gpt_automation.egg-info/
+-rw-rw-rw-   0        0        0    16303 2023-07-25 00:12:31.000000 gpt_automation-0.1.2/gpt_automation.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      492 2023-07-25 00:12:31.000000 gpt_automation-0.1.2/gpt_automation.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 00:12:31.000000 gpt_automation-0.1.2/gpt_automation.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-07-25 00:12:31.000000 gpt_automation-0.1.2/gpt_automation.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       21 2023-07-25 00:12:31.000000 gpt_automation-0.1.2/gpt_automation.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-25 00:12:31.000000 gpt_automation-0.1.2/gpt_automation.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      452 2023-07-25 00:04:10.000000 gpt_automation-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0      432 2023-07-25 00:12:31.357181 gpt_automation-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      258 2023-07-25 00:03:46.000000 gpt_automation-0.1.2/setup.py
```

### Comparing `gpt_automation-0.1.1/LICENSE` & `gpt_automation-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt_automation-0.1.1/PKG-INFO` & `gpt_automation-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt_automation
-Version: 0.1.1
+Version: 0.1.2
 Summary: GPT directory structure and file contents prompt generator
 Home-page: https://github.com/vrocky/gpt-automation/
 Author: Vinit
 Author-email: Vinit <author@example.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
```

### Comparing `gpt_automation-0.1.1/README.md` & `gpt_automation-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `gpt_automation-0.1.1/gpt_automation.egg-info/PKG-INFO` & `gpt_automation-0.1.2/gpt_automation.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-automation
-Version: 0.1.1
+Version: 0.1.2
 Summary: GPT directory structure and file contents prompt generator
 Home-page: https://github.com/vrocky/gpt-automation/
 Author: Vinit
 Author-email: Vinit <author@example.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
```

