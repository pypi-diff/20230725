# Comparing `tmp/proctracer-0.0.12.tar.gz` & `tmp/proctracer-0.0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proctracer-0.0.12.tar", last modified: Tue Jul 25 08:41:29 2023, max compression
+gzip compressed data, was "proctracer-0.0.13.tar", last modified: Tue Jul 25 09:52:40 2023, max compression
```

## Comparing `proctracer-0.0.12.tar` & `proctracer-0.0.13.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:41:29.372778 proctracer-0.0.12/
--rw-r--r--   0 root         (0) root         (0)     1498 2023-07-25 07:18:11.000000 proctracer-0.0.12/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-25 07:18:11.000000 proctracer-0.0.12/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2747 2023-07-25 08:41:29.372778 proctracer-0.0.12/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1631 2023-07-25 07:18:11.000000 proctracer-0.0.12/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:41:29.368778 proctracer-0.0.12/proctracer/
--rw-r--r--   0 root         (0) root         (0)      113 2023-07-25 08:41:19.000000 proctracer-0.0.12/proctracer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:41:29.372778 proctracer-0.0.12/proctracer/plugins/
--rw-r--r--   0 root         (0) root         (0)      589 2023-07-25 07:18:11.000000 proctracer-0.0.12/proctracer/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3731 2023-07-25 07:18:11.000000 proctracer-0.0.12/proctracer/plugins/net_dev.plugin.py
--rw-r--r--   0 root         (0) root         (0)     3323 2023-07-25 08:41:02.000000 proctracer-0.0.12/proctracer/plugins/net_snmp_udp.plugin.py
--rw-r--r--   0 root         (0) root         (0)     6412 2023-07-25 07:18:11.000000 proctracer-0.0.12/proctracer/plugins/net_udpX.plugin.py
--rw-r--r--   0 root         (0) root         (0)     5625 2023-07-25 07:18:11.000000 proctracer-0.0.12/proctracer/plugins/pid_stat.plugin.py
--rw-r--r--   0 root         (0) root         (0)     3285 2023-07-25 07:18:11.000000 proctracer-0.0.12/proctracer/plugins/plugin_base.py
--rw-r--r--   0 root         (0) root         (0)     4434 2023-07-25 07:18:11.000000 proctracer-0.0.12/proctracer/plugins/plugin_proc_tracer_base.py
--rw-r--r--   0 root         (0) root         (0)     2876 2023-07-25 07:18:11.000000 proctracer-0.0.12/proctracer/plugins/pressure_X.plugin.py
--rw-r--r--   0 root         (0) root         (0)     2489 2023-07-25 07:18:11.000000 proctracer-0.0.12/proctracer/plugins/stat.plugin.py
--rw-r--r--   0 root         (0) root         (0)     2277 2023-07-25 07:18:11.000000 proctracer-0.0.12/proctracer/plugins/text_pipe.plugin.py
--rwxr-xr-x   0 root         (0) root         (0)     4706 2023-07-25 07:18:11.000000 proctracer-0.0.12/proctracer/proctracer.py
--rw-r--r--   0 root         (0) root         (0)       87 2023-07-25 07:18:11.000000 proctracer-0.0.12/proctracer/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:41:29.372778 proctracer-0.0.12/proctracer.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2747 2023-07-25 08:41:29.000000 proctracer-0.0.12/proctracer.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      712 2023-07-25 08:41:29.000000 proctracer-0.0.12/proctracer.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 08:41:29.000000 proctracer-0.0.12/proctracer.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       59 2023-07-25 08:41:29.000000 proctracer-0.0.12/proctracer.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       85 2023-07-25 08:41:29.000000 proctracer-0.0.12/proctracer.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-07-25 08:41:29.000000 proctracer-0.0.12/proctracer.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      101 2023-07-25 08:41:29.372778 proctracer-0.0.12/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     4836 2023-07-25 07:18:11.000000 proctracer-0.0.12/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:52:40.951536 proctracer-0.0.13/
+-rw-r--r--   0 root         (0) root         (0)     1498 2023-07-25 07:18:11.000000 proctracer-0.0.13/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-25 07:18:11.000000 proctracer-0.0.13/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2747 2023-07-25 09:52:40.951536 proctracer-0.0.13/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1631 2023-07-25 07:18:11.000000 proctracer-0.0.13/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:52:40.951536 proctracer-0.0.13/proctracer/
+-rw-r--r--   0 root         (0) root         (0)      113 2023-07-25 09:52:27.000000 proctracer-0.0.13/proctracer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:52:40.951536 proctracer-0.0.13/proctracer/plugins/
+-rw-r--r--   0 root         (0) root         (0)      589 2023-07-25 07:18:11.000000 proctracer-0.0.13/proctracer/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3731 2023-07-25 07:18:11.000000 proctracer-0.0.13/proctracer/plugins/net_dev.plugin.py
+-rw-r--r--   0 root         (0) root         (0)     3312 2023-07-25 09:51:03.000000 proctracer-0.0.13/proctracer/plugins/net_snmp_udp.plugin.py
+-rw-r--r--   0 root         (0) root         (0)     6412 2023-07-25 07:18:11.000000 proctracer-0.0.13/proctracer/plugins/net_udpX.plugin.py
+-rw-r--r--   0 root         (0) root         (0)     5625 2023-07-25 07:18:11.000000 proctracer-0.0.13/proctracer/plugins/pid_stat.plugin.py
+-rw-r--r--   0 root         (0) root         (0)     3285 2023-07-25 07:18:11.000000 proctracer-0.0.13/proctracer/plugins/plugin_base.py
+-rw-r--r--   0 root         (0) root         (0)     4990 2023-07-25 09:51:13.000000 proctracer-0.0.13/proctracer/plugins/plugin_proc_tracer_base.py
+-rw-r--r--   0 root         (0) root         (0)     2876 2023-07-25 07:18:11.000000 proctracer-0.0.13/proctracer/plugins/pressure_X.plugin.py
+-rw-r--r--   0 root         (0) root         (0)     2489 2023-07-25 07:18:11.000000 proctracer-0.0.13/proctracer/plugins/stat.plugin.py
+-rw-r--r--   0 root         (0) root         (0)     2277 2023-07-25 07:18:11.000000 proctracer-0.0.13/proctracer/plugins/text_pipe.plugin.py
+-rwxr-xr-x   0 root         (0) root         (0)     4706 2023-07-25 07:18:11.000000 proctracer-0.0.13/proctracer/proctracer.py
+-rw-r--r--   0 root         (0) root         (0)       87 2023-07-25 07:18:11.000000 proctracer-0.0.13/proctracer/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:52:40.951536 proctracer-0.0.13/proctracer.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2747 2023-07-25 09:52:40.000000 proctracer-0.0.13/proctracer.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      712 2023-07-25 09:52:40.000000 proctracer-0.0.13/proctracer.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 09:52:40.000000 proctracer-0.0.13/proctracer.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       59 2023-07-25 09:52:40.000000 proctracer-0.0.13/proctracer.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       85 2023-07-25 09:52:40.000000 proctracer-0.0.13/proctracer.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-07-25 09:52:40.000000 proctracer-0.0.13/proctracer.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      101 2023-07-25 09:52:40.951536 proctracer-0.0.13/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     4836 2023-07-25 07:18:11.000000 proctracer-0.0.13/setup.py
```

### Comparing `proctracer-0.0.12/LICENSE.md` & `proctracer-0.0.13/LICENSE.md`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.12/PKG-INFO` & `proctracer-0.0.13/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proctracer
-Version: 0.0.12
+Version: 0.0.13
 Summary: /proc Tracer
 Home-page: https://proctracer.io
 Author: David Kracht
 Author-email: dave.kracht@gmail.com
 License: BSD-3
 Project-URL: Documentation, https://github.com/david-kracht/proctracer
 Project-URL: Source, https://github.com/david-kracht/proctracer.git
```

### Comparing `proctracer-0.0.12/README.md` & `proctracer-0.0.13/README.md`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.12/proctracer/plugins/__init__.py` & `proctracer-0.0.13/proctracer/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.12/proctracer/plugins/net_dev.plugin.py` & `proctracer-0.0.13/proctracer/plugins/net_dev.plugin.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.12/proctracer/plugins/net_snmp_udp.plugin.py` & `proctracer-0.0.13/proctracer/plugins/net_snmp_udp.plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,17 +6,16 @@
 
     def __init__(self, config_yaml):
         super().__init__(
             config_yaml=config_yaml,
             file='/proc/net/snmp',
             key='Protocol',
             header_in='Protocol InDatagrams NoPorts InErrors OutDatagrams RcvbufErrors SndbufErrors InCsumErrors IgnoredMulti MemErrors',
-            first_line=9,
-            last_line=10,
-            patterns='Udp:'
+            patterns='Udp:',
+            anti_patterns='InDatagrams'
             )
 
     def mapper(self, sample):
         new_sample={}
         for k,entry in sample.items():
             new_sample[k] = {
                 self.key : k,
```

### Comparing `proctracer-0.0.12/proctracer/plugins/net_udpX.plugin.py` & `proctracer-0.0.13/proctracer/plugins/net_udpX.plugin.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.12/proctracer/plugins/pid_stat.plugin.py` & `proctracer-0.0.13/proctracer/plugins/pid_stat.plugin.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.12/proctracer/plugins/plugin_base.py` & `proctracer-0.0.13/proctracer/plugins/plugin_base.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.12/proctracer/plugins/plugin_proc_tracer_base.py` & `proctracer-0.0.13/proctracer/plugins/plugin_proc_tracer_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,22 +23,23 @@
 
         t=cls.t()
 
         with PdfPages("%s/%s.pdf" % (cls.config_yaml['report_output_path'], cls.config_yaml['report_name']) ) as pdf:
             for p in cls.instances:
                 cls.instances[p].add_diagrams(pdf, t)
 
-    def __init__(self, config_yaml, file, key, header_in, first_line=0, last_line=None, patterns=''):
+    def __init__(self, config_yaml, file, key, header_in, first_line=0, last_line=None, patterns='', anti_patterns=''):
         super().__init__(config_yaml)
         self.file=file
         self.key=key
         self.header_in = header_in
         self.first_line=first_line
         self.last_line=last_line
         self.patterns=patterns.split()
+        self.anti_patterns=anti_patterns.split()
         self.header_in = self.header_in.split()
         self.diff_on = ''
         self.proc_fds={}
         self.sample_old={}
         self.data_frame = pd.DataFrame()
         self.retry_read_counter = 5
 
@@ -86,23 +87,36 @@
 
         t= self.t()
         proc_data = self.proc_reader(file)
 
         if proc_data:
 
             for line in proc_data.splitlines()[self.first_line:self.last_line]:
-
+                
+                #blacklist
+                to_be_rejected = ( len(self.anti_patterns) == 0 )
+                if not to_be_rejected:
+                    for pattern in self.anti_patterns:
+                        if pattern in line:
+                            to_be_rejected = True
+                            break
+                
+                
+                if to_be_rejected:
+                    continue
+                
+                #whitelist
                 to_be_collected = ( len(self.patterns) == 0 )
 
                 if not to_be_collected:
                     for pattern in self.patterns:
                         if pattern in line:
                             to_be_collected = True
                             break
-
+                
                 if to_be_collected:
                     line=self.pre_parsing_step(line)
                     
                     entry = { k: v for k, v in zip(self.header_in, line.split() ) }
                     entry['time']= t
                     sample[entry[self.key]] = entry
```

### Comparing `proctracer-0.0.12/proctracer/plugins/pressure_X.plugin.py` & `proctracer-0.0.13/proctracer/plugins/pressure_X.plugin.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.12/proctracer/plugins/stat.plugin.py` & `proctracer-0.0.13/proctracer/plugins/stat.plugin.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.12/proctracer/plugins/text_pipe.plugin.py` & `proctracer-0.0.13/proctracer/plugins/text_pipe.plugin.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.12/proctracer/proctracer.py` & `proctracer-0.0.13/proctracer/proctracer.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.12/proctracer.egg-info/PKG-INFO` & `proctracer-0.0.13/proctracer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proctracer
-Version: 0.0.12
+Version: 0.0.13
 Summary: /proc Tracer
 Home-page: https://proctracer.io
 Author: David Kracht
 Author-email: dave.kracht@gmail.com
 License: BSD-3
 Project-URL: Documentation, https://github.com/david-kracht/proctracer
 Project-URL: Source, https://github.com/david-kracht/proctracer.git
```

### Comparing `proctracer-0.0.12/proctracer.egg-info/SOURCES.txt` & `proctracer-0.0.13/proctracer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.12/setup.py` & `proctracer-0.0.13/setup.py`

 * *Files identical despite different names*

