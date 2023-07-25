# Comparing `tmp/proctracer-0.0.16.tar.gz` & `tmp/proctracer-0.0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proctracer-0.0.16.tar", last modified: Tue Jul 25 11:32:57 2023, max compression
+gzip compressed data, was "proctracer-0.0.17.tar", last modified: Tue Jul 25 11:38:31 2023, max compression
```

## Comparing `proctracer-0.0.16.tar` & `proctracer-0.0.17.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 11:32:57.431050 proctracer-0.0.16/
--rw-r--r--   0 root         (0) root         (0)     1498 2023-07-25 07:18:11.000000 proctracer-0.0.16/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-25 07:18:11.000000 proctracer-0.0.16/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2747 2023-07-25 11:32:57.431050 proctracer-0.0.16/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1631 2023-07-25 07:18:11.000000 proctracer-0.0.16/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 11:32:57.431050 proctracer-0.0.16/proctracer/
--rw-r--r--   0 root         (0) root         (0)      113 2023-07-25 11:32:54.000000 proctracer-0.0.16/proctracer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 11:32:57.431050 proctracer-0.0.16/proctracer/plugins/
--rw-r--r--   0 root         (0) root         (0)      589 2023-07-25 07:18:11.000000 proctracer-0.0.16/proctracer/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3731 2023-07-25 07:18:11.000000 proctracer-0.0.16/proctracer/plugins/net_dev.plugin.py
--rw-r--r--   0 root         (0) root         (0)     6460 2023-07-25 11:32:41.000000 proctracer-0.0.16/proctracer/plugins/net_snmp_udp.plugin.py
--rw-r--r--   0 root         (0) root         (0)     6412 2023-07-25 07:18:11.000000 proctracer-0.0.16/proctracer/plugins/net_udpX.plugin.py
--rw-r--r--   0 root         (0) root         (0)     5625 2023-07-25 07:18:11.000000 proctracer-0.0.16/proctracer/plugins/pid_stat.plugin.py
--rw-r--r--   0 root         (0) root         (0)     3285 2023-07-25 07:18:11.000000 proctracer-0.0.16/proctracer/plugins/plugin_base.py
--rw-r--r--   0 root         (0) root         (0)     4977 2023-07-25 10:45:01.000000 proctracer-0.0.16/proctracer/plugins/plugin_proc_tracer_base.py
--rw-r--r--   0 root         (0) root         (0)     2876 2023-07-25 07:18:11.000000 proctracer-0.0.16/proctracer/plugins/pressure_X.plugin.py
--rw-r--r--   0 root         (0) root         (0)     2489 2023-07-25 07:18:11.000000 proctracer-0.0.16/proctracer/plugins/stat.plugin.py
--rw-r--r--   0 root         (0) root         (0)     2277 2023-07-25 07:18:11.000000 proctracer-0.0.16/proctracer/plugins/text_pipe.plugin.py
--rwxr-xr-x   0 root         (0) root         (0)     4706 2023-07-25 07:18:11.000000 proctracer-0.0.16/proctracer/proctracer.py
--rw-r--r--   0 root         (0) root         (0)       87 2023-07-25 07:18:11.000000 proctracer-0.0.16/proctracer/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 11:32:57.431050 proctracer-0.0.16/proctracer.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2747 2023-07-25 11:32:57.000000 proctracer-0.0.16/proctracer.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      712 2023-07-25 11:32:57.000000 proctracer-0.0.16/proctracer.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 11:32:57.000000 proctracer-0.0.16/proctracer.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       59 2023-07-25 11:32:57.000000 proctracer-0.0.16/proctracer.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       85 2023-07-25 11:32:57.000000 proctracer-0.0.16/proctracer.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-07-25 11:32:57.000000 proctracer-0.0.16/proctracer.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      101 2023-07-25 11:32:57.431050 proctracer-0.0.16/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     4836 2023-07-25 07:18:11.000000 proctracer-0.0.16/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 11:38:31.943454 proctracer-0.0.17/
+-rw-r--r--   0 root         (0) root         (0)     1498 2023-07-25 07:18:11.000000 proctracer-0.0.17/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-25 07:18:11.000000 proctracer-0.0.17/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2747 2023-07-25 11:38:31.943454 proctracer-0.0.17/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1631 2023-07-25 07:18:11.000000 proctracer-0.0.17/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 11:38:31.939454 proctracer-0.0.17/proctracer/
+-rw-r--r--   0 root         (0) root         (0)      113 2023-07-25 11:37:04.000000 proctracer-0.0.17/proctracer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 11:38:31.943454 proctracer-0.0.17/proctracer/plugins/
+-rw-r--r--   0 root         (0) root         (0)      589 2023-07-25 07:18:11.000000 proctracer-0.0.17/proctracer/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3731 2023-07-25 07:18:11.000000 proctracer-0.0.17/proctracer/plugins/net_dev.plugin.py
+-rw-r--r--   0 root         (0) root         (0)     3310 2023-07-25 11:37:39.000000 proctracer-0.0.17/proctracer/plugins/net_snmp_udp.plugin.py
+-rw-r--r--   0 root         (0) root         (0)     6459 2023-07-25 11:38:03.000000 proctracer-0.0.17/proctracer/plugins/net_udpX.plugin.py
+-rw-r--r--   0 root         (0) root         (0)     5625 2023-07-25 07:18:11.000000 proctracer-0.0.17/proctracer/plugins/pid_stat.plugin.py
+-rw-r--r--   0 root         (0) root         (0)     3285 2023-07-25 07:18:11.000000 proctracer-0.0.17/proctracer/plugins/plugin_base.py
+-rw-r--r--   0 root         (0) root         (0)     4977 2023-07-25 10:45:01.000000 proctracer-0.0.17/proctracer/plugins/plugin_proc_tracer_base.py
+-rw-r--r--   0 root         (0) root         (0)     2876 2023-07-25 07:18:11.000000 proctracer-0.0.17/proctracer/plugins/pressure_X.plugin.py
+-rw-r--r--   0 root         (0) root         (0)     2489 2023-07-25 07:18:11.000000 proctracer-0.0.17/proctracer/plugins/stat.plugin.py
+-rw-r--r--   0 root         (0) root         (0)     2277 2023-07-25 07:18:11.000000 proctracer-0.0.17/proctracer/plugins/text_pipe.plugin.py
+-rwxr-xr-x   0 root         (0) root         (0)     4706 2023-07-25 07:18:11.000000 proctracer-0.0.17/proctracer/proctracer.py
+-rw-r--r--   0 root         (0) root         (0)       87 2023-07-25 07:18:11.000000 proctracer-0.0.17/proctracer/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 11:38:31.939454 proctracer-0.0.17/proctracer.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2747 2023-07-25 11:38:31.000000 proctracer-0.0.17/proctracer.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      712 2023-07-25 11:38:31.000000 proctracer-0.0.17/proctracer.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 11:38:31.000000 proctracer-0.0.17/proctracer.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       59 2023-07-25 11:38:31.000000 proctracer-0.0.17/proctracer.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       85 2023-07-25 11:38:31.000000 proctracer-0.0.17/proctracer.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-07-25 11:38:31.000000 proctracer-0.0.17/proctracer.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      101 2023-07-25 11:38:31.943454 proctracer-0.0.17/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     4836 2023-07-25 07:18:11.000000 proctracer-0.0.17/setup.py
```

### Comparing `proctracer-0.0.16/LICENSE.md` & `proctracer-0.0.17/LICENSE.md`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.16/PKG-INFO` & `proctracer-0.0.17/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proctracer
-Version: 0.0.16
+Version: 0.0.17
 Summary: /proc Tracer
 Home-page: https://proctracer.io
 Author: David Kracht
 Author-email: dave.kracht@gmail.com
 License: BSD-3
 Project-URL: Documentation, https://github.com/david-kracht/proctracer
 Project-URL: Source, https://github.com/david-kracht/proctracer.git
```

### Comparing `proctracer-0.0.16/README.md` & `proctracer-0.0.17/README.md`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.16/proctracer/plugins/__init__.py` & `proctracer-0.0.17/proctracer/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.16/proctracer/plugins/net_dev.plugin.py` & `proctracer-0.0.17/proctracer/plugins/net_dev.plugin.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.16/proctracer/plugins/net_snmp_udp.plugin.py` & `proctracer-0.0.17/proctracer/plugins/net_udpX.plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,15 @@
                 
             if not pivot_table.columns.empty:
                 axs[0].legend(fontsize='xx-small', loc= 'upper right')
                  
             axs[0].set_ylabel('Size of tx/rx Queues')
             axs[0].grid()
             axs[0].set_xlim(0,maxT)
-            #axs[0].set_ylim(0,maxV*1.05+0.01)
+            axs[0].set_ylim(0,maxV*1.05+0.01)
 
             ######### Drops
             maxV=0
             for value in ['drops']:
                 pivot_table = self.data_frame.pivot_table(index='time', columns=['socket'], values=value)
                 #pivot_table -= pivot_table.iloc[0].values.squeeze() # relative count wrt. start time
                 pivot_table = pivot_table.loc[:, (pivot_table > 0).any()]
```

### Comparing `proctracer-0.0.16/proctracer/plugins/pid_stat.plugin.py` & `proctracer-0.0.17/proctracer/plugins/pid_stat.plugin.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.16/proctracer/plugins/plugin_base.py` & `proctracer-0.0.17/proctracer/plugins/plugin_base.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.16/proctracer/plugins/plugin_proc_tracer_base.py` & `proctracer-0.0.17/proctracer/plugins/plugin_proc_tracer_base.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.16/proctracer/plugins/pressure_X.plugin.py` & `proctracer-0.0.17/proctracer/plugins/pressure_X.plugin.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.16/proctracer/plugins/stat.plugin.py` & `proctracer-0.0.17/proctracer/plugins/stat.plugin.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.16/proctracer/plugins/text_pipe.plugin.py` & `proctracer-0.0.17/proctracer/plugins/text_pipe.plugin.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.16/proctracer/proctracer.py` & `proctracer-0.0.17/proctracer/proctracer.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.16/proctracer.egg-info/PKG-INFO` & `proctracer-0.0.17/proctracer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proctracer
-Version: 0.0.16
+Version: 0.0.17
 Summary: /proc Tracer
 Home-page: https://proctracer.io
 Author: David Kracht
 Author-email: dave.kracht@gmail.com
 License: BSD-3
 Project-URL: Documentation, https://github.com/david-kracht/proctracer
 Project-URL: Source, https://github.com/david-kracht/proctracer.git
```

### Comparing `proctracer-0.0.16/proctracer.egg-info/SOURCES.txt` & `proctracer-0.0.17/proctracer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.16/setup.py` & `proctracer-0.0.17/setup.py`

 * *Files identical despite different names*

