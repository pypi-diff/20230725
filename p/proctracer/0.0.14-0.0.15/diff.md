# Comparing `tmp/proctracer-0.0.14.tar.gz` & `tmp/proctracer-0.0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proctracer-0.0.14.tar", last modified: Tue Jul 25 10:17:00 2023, max compression
+gzip compressed data, was "proctracer-0.0.15.tar", last modified: Tue Jul 25 10:45:21 2023, max compression
```

## Comparing `proctracer-0.0.14.tar` & `proctracer-0.0.15.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 10:17:00.687907 proctracer-0.0.14/
--rw-r--r--   0 root         (0) root         (0)     1498 2023-07-25 07:18:11.000000 proctracer-0.0.14/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-25 07:18:11.000000 proctracer-0.0.14/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2747 2023-07-25 10:17:00.687907 proctracer-0.0.14/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1631 2023-07-25 07:18:11.000000 proctracer-0.0.14/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 10:17:00.687907 proctracer-0.0.14/proctracer/
--rw-r--r--   0 root         (0) root         (0)      113 2023-07-25 10:16:42.000000 proctracer-0.0.14/proctracer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 10:17:00.687907 proctracer-0.0.14/proctracer/plugins/
--rw-r--r--   0 root         (0) root         (0)      589 2023-07-25 07:18:11.000000 proctracer-0.0.14/proctracer/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3731 2023-07-25 07:18:11.000000 proctracer-0.0.14/proctracer/plugins/net_dev.plugin.py
--rw-r--r--   0 root         (0) root         (0)     3310 2023-07-25 09:54:45.000000 proctracer-0.0.14/proctracer/plugins/net_snmp_udp.plugin.py
--rw-r--r--   0 root         (0) root         (0)     6412 2023-07-25 07:18:11.000000 proctracer-0.0.14/proctracer/plugins/net_udpX.plugin.py
--rw-r--r--   0 root         (0) root         (0)     5625 2023-07-25 07:18:11.000000 proctracer-0.0.14/proctracer/plugins/pid_stat.plugin.py
--rw-r--r--   0 root         (0) root         (0)     3285 2023-07-25 07:18:11.000000 proctracer-0.0.14/proctracer/plugins/plugin_base.py
--rw-r--r--   0 root         (0) root         (0)     4973 2023-07-25 10:14:56.000000 proctracer-0.0.14/proctracer/plugins/plugin_proc_tracer_base.py
--rw-r--r--   0 root         (0) root         (0)     2876 2023-07-25 07:18:11.000000 proctracer-0.0.14/proctracer/plugins/pressure_X.plugin.py
--rw-r--r--   0 root         (0) root         (0)     2489 2023-07-25 07:18:11.000000 proctracer-0.0.14/proctracer/plugins/stat.plugin.py
--rw-r--r--   0 root         (0) root         (0)     2277 2023-07-25 07:18:11.000000 proctracer-0.0.14/proctracer/plugins/text_pipe.plugin.py
--rwxr-xr-x   0 root         (0) root         (0)     4706 2023-07-25 07:18:11.000000 proctracer-0.0.14/proctracer/proctracer.py
--rw-r--r--   0 root         (0) root         (0)       87 2023-07-25 07:18:11.000000 proctracer-0.0.14/proctracer/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 10:17:00.687907 proctracer-0.0.14/proctracer.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2747 2023-07-25 10:17:00.000000 proctracer-0.0.14/proctracer.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      712 2023-07-25 10:17:00.000000 proctracer-0.0.14/proctracer.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 10:17:00.000000 proctracer-0.0.14/proctracer.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       59 2023-07-25 10:17:00.000000 proctracer-0.0.14/proctracer.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       85 2023-07-25 10:17:00.000000 proctracer-0.0.14/proctracer.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-07-25 10:17:00.000000 proctracer-0.0.14/proctracer.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      101 2023-07-25 10:17:00.687907 proctracer-0.0.14/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     4836 2023-07-25 07:18:11.000000 proctracer-0.0.14/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 10:45:21.025752 proctracer-0.0.15/
+-rw-r--r--   0 root         (0) root         (0)     1498 2023-07-25 07:18:11.000000 proctracer-0.0.15/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-25 07:18:11.000000 proctracer-0.0.15/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2747 2023-07-25 10:45:21.025752 proctracer-0.0.15/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1631 2023-07-25 07:18:11.000000 proctracer-0.0.15/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 10:45:21.021752 proctracer-0.0.15/proctracer/
+-rw-r--r--   0 root         (0) root         (0)      113 2023-07-25 10:45:19.000000 proctracer-0.0.15/proctracer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 10:45:21.025752 proctracer-0.0.15/proctracer/plugins/
+-rw-r--r--   0 root         (0) root         (0)      589 2023-07-25 07:18:11.000000 proctracer-0.0.15/proctracer/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3731 2023-07-25 07:18:11.000000 proctracer-0.0.15/proctracer/plugins/net_dev.plugin.py
+-rw-r--r--   0 root         (0) root         (0)     3310 2023-07-25 09:54:45.000000 proctracer-0.0.15/proctracer/plugins/net_snmp_udp.plugin.py
+-rw-r--r--   0 root         (0) root         (0)     6412 2023-07-25 07:18:11.000000 proctracer-0.0.15/proctracer/plugins/net_udpX.plugin.py
+-rw-r--r--   0 root         (0) root         (0)     5625 2023-07-25 07:18:11.000000 proctracer-0.0.15/proctracer/plugins/pid_stat.plugin.py
+-rw-r--r--   0 root         (0) root         (0)     3285 2023-07-25 07:18:11.000000 proctracer-0.0.15/proctracer/plugins/plugin_base.py
+-rw-r--r--   0 root         (0) root         (0)     4977 2023-07-25 10:45:01.000000 proctracer-0.0.15/proctracer/plugins/plugin_proc_tracer_base.py
+-rw-r--r--   0 root         (0) root         (0)     2876 2023-07-25 07:18:11.000000 proctracer-0.0.15/proctracer/plugins/pressure_X.plugin.py
+-rw-r--r--   0 root         (0) root         (0)     2489 2023-07-25 07:18:11.000000 proctracer-0.0.15/proctracer/plugins/stat.plugin.py
+-rw-r--r--   0 root         (0) root         (0)     2277 2023-07-25 07:18:11.000000 proctracer-0.0.15/proctracer/plugins/text_pipe.plugin.py
+-rwxr-xr-x   0 root         (0) root         (0)     4706 2023-07-25 07:18:11.000000 proctracer-0.0.15/proctracer/proctracer.py
+-rw-r--r--   0 root         (0) root         (0)       87 2023-07-25 07:18:11.000000 proctracer-0.0.15/proctracer/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 10:45:21.025752 proctracer-0.0.15/proctracer.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2747 2023-07-25 10:45:20.000000 proctracer-0.0.15/proctracer.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      712 2023-07-25 10:45:21.000000 proctracer-0.0.15/proctracer.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 10:45:20.000000 proctracer-0.0.15/proctracer.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       59 2023-07-25 10:45:20.000000 proctracer-0.0.15/proctracer.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       85 2023-07-25 10:45:20.000000 proctracer-0.0.15/proctracer.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-07-25 10:45:20.000000 proctracer-0.0.15/proctracer.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      101 2023-07-25 10:45:21.025752 proctracer-0.0.15/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     4836 2023-07-25 07:18:11.000000 proctracer-0.0.15/setup.py
```

### Comparing `proctracer-0.0.14/LICENSE.md` & `proctracer-0.0.15/LICENSE.md`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.14/PKG-INFO` & `proctracer-0.0.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proctracer
-Version: 0.0.14
+Version: 0.0.15
 Summary: /proc Tracer
 Home-page: https://proctracer.io
 Author: David Kracht
 Author-email: dave.kracht@gmail.com
 License: BSD-3
 Project-URL: Documentation, https://github.com/david-kracht/proctracer
 Project-URL: Source, https://github.com/david-kracht/proctracer.git
```

### Comparing `proctracer-0.0.14/README.md` & `proctracer-0.0.15/README.md`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.14/proctracer/plugins/__init__.py` & `proctracer-0.0.15/proctracer/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.14/proctracer/plugins/net_dev.plugin.py` & `proctracer-0.0.15/proctracer/plugins/net_dev.plugin.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.14/proctracer/plugins/net_snmp_udp.plugin.py` & `proctracer-0.0.15/proctracer/plugins/net_snmp_udp.plugin.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.14/proctracer/plugins/net_udpX.plugin.py` & `proctracer-0.0.15/proctracer/plugins/net_udpX.plugin.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.14/proctracer/plugins/pid_stat.plugin.py` & `proctracer-0.0.15/proctracer/plugins/pid_stat.plugin.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.14/proctracer/plugins/plugin_base.py` & `proctracer-0.0.15/proctracer/plugins/plugin_base.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.14/proctracer/plugins/plugin_proc_tracer_base.py` & `proctracer-0.0.15/proctracer/plugins/plugin_proc_tracer_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -89,23 +89,23 @@
         proc_data = self.proc_reader(file)
 
         if proc_data:
 
             for line in proc_data.splitlines()[self.first_line:self.last_line]:
                 
                 #blacklist
-                to_be_rejected = ( len(self.anti_patterns) != 0 )
-                if not to_be_rejected:
+                if ( len(self.anti_patterns) != 0 ):
+                    to_be_collected=True
                     for pattern in self.anti_patterns:
                         if pattern in line:
-                            to_be_rejected = True
+                            to_be_collected = False
                             break
                 
-                if to_be_rejected:
-                    continue
+                    if not to_be_collected:
+                        continue
                 
                 #whitelist
                 to_be_collected = ( len(self.patterns) == 0 )
 
                 if not to_be_collected:
                     for pattern in self.patterns:
                         if pattern in line:
```

### Comparing `proctracer-0.0.14/proctracer/plugins/pressure_X.plugin.py` & `proctracer-0.0.15/proctracer/plugins/pressure_X.plugin.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.14/proctracer/plugins/stat.plugin.py` & `proctracer-0.0.15/proctracer/plugins/stat.plugin.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.14/proctracer/plugins/text_pipe.plugin.py` & `proctracer-0.0.15/proctracer/plugins/text_pipe.plugin.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.14/proctracer/proctracer.py` & `proctracer-0.0.15/proctracer/proctracer.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.14/proctracer.egg-info/PKG-INFO` & `proctracer-0.0.15/proctracer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proctracer
-Version: 0.0.14
+Version: 0.0.15
 Summary: /proc Tracer
 Home-page: https://proctracer.io
 Author: David Kracht
 Author-email: dave.kracht@gmail.com
 License: BSD-3
 Project-URL: Documentation, https://github.com/david-kracht/proctracer
 Project-URL: Source, https://github.com/david-kracht/proctracer.git
```

### Comparing `proctracer-0.0.14/proctracer.egg-info/SOURCES.txt` & `proctracer-0.0.15/proctracer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.14/setup.py` & `proctracer-0.0.15/setup.py`

 * *Files identical despite different names*

