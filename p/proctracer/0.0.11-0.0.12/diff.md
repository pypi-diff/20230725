# Comparing `tmp/proctracer-0.0.11.tar.gz` & `tmp/proctracer-0.0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proctracer-0.0.11.tar", last modified: Tue Jul 25 08:20:11 2023, max compression
+gzip compressed data, was "proctracer-0.0.12.tar", last modified: Tue Jul 25 08:41:29 2023, max compression
```

## Comparing `proctracer-0.0.11.tar` & `proctracer-0.0.12.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:20:11.310341 proctracer-0.0.11/
--rw-r--r--   0 root         (0) root         (0)     1498 2023-07-25 07:18:11.000000 proctracer-0.0.11/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-25 07:18:11.000000 proctracer-0.0.11/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2747 2023-07-25 08:20:11.310341 proctracer-0.0.11/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1631 2023-07-25 07:18:11.000000 proctracer-0.0.11/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:20:11.310341 proctracer-0.0.11/proctracer/
--rw-r--r--   0 root         (0) root         (0)      113 2023-07-25 08:19:59.000000 proctracer-0.0.11/proctracer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:20:11.310341 proctracer-0.0.11/proctracer/plugins/
--rw-r--r--   0 root         (0) root         (0)      589 2023-07-25 07:18:11.000000 proctracer-0.0.11/proctracer/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3731 2023-07-25 07:18:11.000000 proctracer-0.0.11/proctracer/plugins/net_dev.plugin.py
--rw-r--r--   0 root         (0) root         (0)     3324 2023-07-25 08:08:27.000000 proctracer-0.0.11/proctracer/plugins/net_snmp_udp.plugin.py
--rw-r--r--   0 root         (0) root         (0)     6412 2023-07-25 07:18:11.000000 proctracer-0.0.11/proctracer/plugins/net_udpX.plugin.py
--rw-r--r--   0 root         (0) root         (0)     5625 2023-07-25 07:18:11.000000 proctracer-0.0.11/proctracer/plugins/pid_stat.plugin.py
--rw-r--r--   0 root         (0) root         (0)     3285 2023-07-25 07:18:11.000000 proctracer-0.0.11/proctracer/plugins/plugin_base.py
--rw-r--r--   0 root         (0) root         (0)     4434 2023-07-25 07:18:11.000000 proctracer-0.0.11/proctracer/plugins/plugin_proc_tracer_base.py
--rw-r--r--   0 root         (0) root         (0)     2876 2023-07-25 07:18:11.000000 proctracer-0.0.11/proctracer/plugins/pressure_X.plugin.py
--rw-r--r--   0 root         (0) root         (0)     2489 2023-07-25 07:18:11.000000 proctracer-0.0.11/proctracer/plugins/stat.plugin.py
--rw-r--r--   0 root         (0) root         (0)     2277 2023-07-25 07:18:11.000000 proctracer-0.0.11/proctracer/plugins/text_pipe.plugin.py
--rwxr-xr-x   0 root         (0) root         (0)     4706 2023-07-25 07:18:11.000000 proctracer-0.0.11/proctracer/proctracer.py
--rw-r--r--   0 root         (0) root         (0)       87 2023-07-25 07:18:11.000000 proctracer-0.0.11/proctracer/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:20:11.310341 proctracer-0.0.11/proctracer.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2747 2023-07-25 08:20:11.000000 proctracer-0.0.11/proctracer.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      712 2023-07-25 08:20:11.000000 proctracer-0.0.11/proctracer.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 08:20:11.000000 proctracer-0.0.11/proctracer.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       59 2023-07-25 08:20:11.000000 proctracer-0.0.11/proctracer.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       85 2023-07-25 08:20:11.000000 proctracer-0.0.11/proctracer.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-07-25 08:20:11.000000 proctracer-0.0.11/proctracer.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      101 2023-07-25 08:20:11.310341 proctracer-0.0.11/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     4836 2023-07-25 07:18:11.000000 proctracer-0.0.11/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:41:29.372778 proctracer-0.0.12/
+-rw-r--r--   0 root         (0) root         (0)     1498 2023-07-25 07:18:11.000000 proctracer-0.0.12/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-25 07:18:11.000000 proctracer-0.0.12/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2747 2023-07-25 08:41:29.372778 proctracer-0.0.12/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1631 2023-07-25 07:18:11.000000 proctracer-0.0.12/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:41:29.368778 proctracer-0.0.12/proctracer/
+-rw-r--r--   0 root         (0) root         (0)      113 2023-07-25 08:41:19.000000 proctracer-0.0.12/proctracer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:41:29.372778 proctracer-0.0.12/proctracer/plugins/
+-rw-r--r--   0 root         (0) root         (0)      589 2023-07-25 07:18:11.000000 proctracer-0.0.12/proctracer/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3731 2023-07-25 07:18:11.000000 proctracer-0.0.12/proctracer/plugins/net_dev.plugin.py
+-rw-r--r--   0 root         (0) root         (0)     3323 2023-07-25 08:41:02.000000 proctracer-0.0.12/proctracer/plugins/net_snmp_udp.plugin.py
+-rw-r--r--   0 root         (0) root         (0)     6412 2023-07-25 07:18:11.000000 proctracer-0.0.12/proctracer/plugins/net_udpX.plugin.py
+-rw-r--r--   0 root         (0) root         (0)     5625 2023-07-25 07:18:11.000000 proctracer-0.0.12/proctracer/plugins/pid_stat.plugin.py
+-rw-r--r--   0 root         (0) root         (0)     3285 2023-07-25 07:18:11.000000 proctracer-0.0.12/proctracer/plugins/plugin_base.py
+-rw-r--r--   0 root         (0) root         (0)     4434 2023-07-25 07:18:11.000000 proctracer-0.0.12/proctracer/plugins/plugin_proc_tracer_base.py
+-rw-r--r--   0 root         (0) root         (0)     2876 2023-07-25 07:18:11.000000 proctracer-0.0.12/proctracer/plugins/pressure_X.plugin.py
+-rw-r--r--   0 root         (0) root         (0)     2489 2023-07-25 07:18:11.000000 proctracer-0.0.12/proctracer/plugins/stat.plugin.py
+-rw-r--r--   0 root         (0) root         (0)     2277 2023-07-25 07:18:11.000000 proctracer-0.0.12/proctracer/plugins/text_pipe.plugin.py
+-rwxr-xr-x   0 root         (0) root         (0)     4706 2023-07-25 07:18:11.000000 proctracer-0.0.12/proctracer/proctracer.py
+-rw-r--r--   0 root         (0) root         (0)       87 2023-07-25 07:18:11.000000 proctracer-0.0.12/proctracer/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:41:29.372778 proctracer-0.0.12/proctracer.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2747 2023-07-25 08:41:29.000000 proctracer-0.0.12/proctracer.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      712 2023-07-25 08:41:29.000000 proctracer-0.0.12/proctracer.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 08:41:29.000000 proctracer-0.0.12/proctracer.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       59 2023-07-25 08:41:29.000000 proctracer-0.0.12/proctracer.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       85 2023-07-25 08:41:29.000000 proctracer-0.0.12/proctracer.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-07-25 08:41:29.000000 proctracer-0.0.12/proctracer.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      101 2023-07-25 08:41:29.372778 proctracer-0.0.12/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     4836 2023-07-25 07:18:11.000000 proctracer-0.0.12/setup.py
```

### Comparing `proctracer-0.0.11/LICENSE.md` & `proctracer-0.0.12/LICENSE.md`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.11/PKG-INFO` & `proctracer-0.0.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proctracer
-Version: 0.0.11
+Version: 0.0.12
 Summary: /proc Tracer
 Home-page: https://proctracer.io
 Author: David Kracht
 Author-email: dave.kracht@gmail.com
 License: BSD-3
 Project-URL: Documentation, https://github.com/david-kracht/proctracer
 Project-URL: Source, https://github.com/david-kracht/proctracer.git
```

### Comparing `proctracer-0.0.11/README.md` & `proctracer-0.0.12/README.md`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.11/proctracer/plugins/__init__.py` & `proctracer-0.0.12/proctracer/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.11/proctracer/plugins/net_dev.plugin.py` & `proctracer-0.0.12/proctracer/plugins/net_dev.plugin.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.11/proctracer/plugins/net_snmp_udp.plugin.py` & `proctracer-0.0.12/proctracer/plugins/net_snmp_udp.plugin.py`

 * *Files 11% similar despite different names*

```diff
@@ -59,32 +59,32 @@
 
             axs[1].plot( x *100.0, label= "InErrorRate")
             axs[1].legend()
                 
             axs[1].set_ylabel('Ratio [%]')
             axs[1].grid()
             axs[1].set_xlim(0,maxT)
-            #axs[1].set_ylim(0,None)
+            axs[1].set_ylim(0,105.0)
 
             ######### Ratio 2
             x=self.data_frame[["SndbufErrors"]].div(self.data_frame.OutDatagrams, axis=0) # relative count wrt. start time
 
             axs[2].plot( x *100.0 , label= "SndbufErrors")
             axs[2].legend()
                 
             axs[2].set_ylabel('Ratio [%]')
             axs[2].grid()
             axs[2].set_xlim(0,maxT)
-            #axs[2].set_ylim(0,None)
+            axs[2].set_ylim(0,105.0)
 
             ######### Counts
             self.data_frame -= self.data_frame.iloc[0].values.squeeze() # relative count wrt. start time
             
             axs[0].plot( self.data_frame , label= self.data_frame.columns)
             axs[0].legend()
                 
             axs[0].set_ylabel('Datagrams [count]')
             axs[0].grid()
             axs[0].set_xlim(0,maxT)
-            #axs[0].set_ylim(0,None)
+            axs[0].set_ylim(0,None)
 
         pdf.savefig(fig)
```

### Comparing `proctracer-0.0.11/proctracer/plugins/net_udpX.plugin.py` & `proctracer-0.0.12/proctracer/plugins/net_udpX.plugin.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.11/proctracer/plugins/pid_stat.plugin.py` & `proctracer-0.0.12/proctracer/plugins/pid_stat.plugin.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.11/proctracer/plugins/plugin_base.py` & `proctracer-0.0.12/proctracer/plugins/plugin_base.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.11/proctracer/plugins/plugin_proc_tracer_base.py` & `proctracer-0.0.12/proctracer/plugins/plugin_proc_tracer_base.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.11/proctracer/plugins/pressure_X.plugin.py` & `proctracer-0.0.12/proctracer/plugins/pressure_X.plugin.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.11/proctracer/plugins/stat.plugin.py` & `proctracer-0.0.12/proctracer/plugins/stat.plugin.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.11/proctracer/plugins/text_pipe.plugin.py` & `proctracer-0.0.12/proctracer/plugins/text_pipe.plugin.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.11/proctracer/proctracer.py` & `proctracer-0.0.12/proctracer/proctracer.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.11/proctracer.egg-info/PKG-INFO` & `proctracer-0.0.12/proctracer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proctracer
-Version: 0.0.11
+Version: 0.0.12
 Summary: /proc Tracer
 Home-page: https://proctracer.io
 Author: David Kracht
 Author-email: dave.kracht@gmail.com
 License: BSD-3
 Project-URL: Documentation, https://github.com/david-kracht/proctracer
 Project-URL: Source, https://github.com/david-kracht/proctracer.git
```

### Comparing `proctracer-0.0.11/proctracer.egg-info/SOURCES.txt` & `proctracer-0.0.12/proctracer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.11/setup.py` & `proctracer-0.0.12/setup.py`

 * *Files identical despite different names*

