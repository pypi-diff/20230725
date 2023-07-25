# Comparing `tmp/polypacket-1.0.8.tar.gz` & `tmp/polypacket-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/polypacket-1.0.8.tar", last modified: Wed Sep 18 18:31:08 2019, max compression
+gzip compressed data, was "dist/polypacket-1.0.9.tar", last modified: Wed Sep 18 19:09:53 2019, max compression
```

## Comparing `polypacket-1.0.8.tar` & `polypacket-1.0.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0 jason     (1000) jason     (1000)        0 2019-09-18 18:31:08.000000 polypacket-1.0.8/
--rwxrwxrwx   0 jason     (1000) jason     (1000)    17276 2019-09-18 18:31:08.000000 polypacket-1.0.8/PKG-INFO
-drwxrwxrwx   0 jason     (1000) jason     (1000)        0 2019-09-18 18:31:07.000000 polypacket-1.0.8/polypacket/
-drwxrwxrwx   0 jason     (1000) jason     (1000)        0 2019-09-18 18:31:07.000000 polypacket-1.0.8/polypacket/examples/
--rwxrwxrwx   0 jason     (1000) jason     (1000)     1802 2019-09-05 18:31:47.000000 polypacket-1.0.8/polypacket/examples/sample_protocol.xml
--rwxrwxrwx   0 jason     (1000) jason     (1000)     3022 2019-09-18 13:42:35.000000 polypacket-1.0.8/polypacket/examples/sample_protocol.yml
--rwxrwxrwx   0 jason     (1000) jason     (1000)     6639 2019-09-18 13:42:35.000000 polypacket-1.0.8/polypacket/poly-make
--rwxrwxrwx   0 jason     (1000) jason     (1000)     6636 2019-09-18 17:54:02.000000 polypacket-1.0.8/polypacket/poly-packet
--rwxrwxrwx   0 jason     (1000) jason     (1000)    11764 2019-09-18 18:28:24.000000 polypacket-1.0.8/polypacket/polyservice.py
--rwxrwxrwx   0 jason     (1000) jason     (1000)    23833 2019-09-18 18:26:02.000000 polypacket-1.0.8/polypacket/protocol.py
-drwxrwxrwx   0 jason     (1000) jason     (1000)        0 2019-09-18 18:31:08.000000 polypacket-1.0.8/polypacket/templates/
--rwxrwxrwx   0 jason     (1000) jason     (1000)     5296 2019-09-05 16:53:44.000000 polypacket-1.0.8/polypacket/templates/app_template.c
--rwxrwxrwx   0 jason     (1000) jason     (1000)      727 2019-08-23 16:18:54.000000 polypacket-1.0.8/polypacket/templates/app_template.h
--rwxrwxrwx   0 jason     (1000) jason     (1000)      895 2019-09-05 14:51:06.000000 polypacket-1.0.8/polypacket/templates/cmake_template.txt
--rwxrwxrwx   0 jason     (1000) jason     (1000)     9746 2019-09-05 16:48:06.000000 polypacket-1.0.8/polypacket/templates/c_header_template.h
--rwxrwxrwx   0 jason     (1000) jason     (1000)    16762 2019-09-18 13:42:35.000000 polypacket-1.0.8/polypacket/templates/c_source_template.c
--rwxrwxrwx   0 jason     (1000) jason     (1000)     4626 2019-09-13 14:48:31.000000 polypacket-1.0.8/polypacket/templates/doc_template.html
--rwxrwxrwx   0 jason     (1000) jason     (1000)     4935 2019-08-22 14:37:24.000000 polypacket-1.0.8/polypacket/templates/doc_template.md
--rwxrwxrwx   0 jason     (1000) jason     (1000)     1699 2019-08-22 14:37:24.000000 polypacket-1.0.8/polypacket/templates/javascript_template.js
--rwxrwxrwx   0 jason     (1000) jason     (1000)      179 2019-08-22 19:08:49.000000 polypacket-1.0.8/polypacket/templates/readme_template.md
--rwxrwxrwx   0 jason     (1000) jason     (1000)     5357 2019-09-17 14:47:42.000000 polypacket-1.0.8/polypacket/templates/util_main_template.c
--rwxrwxrwx   0 jason     (1000) jason     (1000)       73 2019-09-18 13:42:35.000000 polypacket-1.0.8/polypacket/__init__.py
-drwxrwxrwx   0 jason     (1000) jason     (1000)        0 2019-09-18 18:31:07.000000 polypacket-1.0.8/polypacket.egg-info/
--rwxrwxrwx   0 jason     (1000) jason     (1000)        1 2019-09-18 18:31:07.000000 polypacket-1.0.8/polypacket.egg-info/dependency_links.txt
--rwxrwxrwx   0 jason     (1000) jason     (1000)    17276 2019-09-18 18:31:07.000000 polypacket-1.0.8/polypacket.egg-info/PKG-INFO
--rwxrwxrwx   0 jason     (1000) jason     (1000)       41 2019-09-18 18:31:07.000000 polypacket-1.0.8/polypacket.egg-info/requires.txt
--rwxrwxrwx   0 jason     (1000) jason     (1000)      779 2019-09-18 18:31:07.000000 polypacket-1.0.8/polypacket.egg-info/SOURCES.txt
--rwxrwxrwx   0 jason     (1000) jason     (1000)       11 2019-09-18 18:31:07.000000 polypacket-1.0.8/polypacket.egg-info/top_level.txt
--rwxrwxrwx   0 jason     (1000) jason     (1000)    13588 2019-09-18 13:42:35.000000 polypacket-1.0.8/README.md
--rwxrwxrwx   0 jason     (1000) jason     (1000)       38 2019-09-18 18:31:08.000000 polypacket-1.0.8/setup.cfg
--rwxrwxrwx   0 jason     (1000) jason     (1000)      951 2019-09-18 18:30:31.000000 polypacket-1.0.8/setup.py
+drwxrwxrwx   0 jason     (1000) jason     (1000)        0 2019-09-18 19:09:53.000000 polypacket-1.0.9/
+-rwxrwxrwx   0 jason     (1000) jason     (1000)    17321 2019-09-18 19:09:53.000000 polypacket-1.0.9/PKG-INFO
+drwxrwxrwx   0 jason     (1000) jason     (1000)        0 2019-09-18 19:09:53.000000 polypacket-1.0.9/polypacket/
+drwxrwxrwx   0 jason     (1000) jason     (1000)        0 2019-09-18 19:09:53.000000 polypacket-1.0.9/polypacket/examples/
+-rwxrwxrwx   0 jason     (1000) jason     (1000)     1802 2019-09-05 18:31:47.000000 polypacket-1.0.9/polypacket/examples/sample_protocol.xml
+-rwxrwxrwx   0 jason     (1000) jason     (1000)     3022 2019-09-18 13:42:35.000000 polypacket-1.0.9/polypacket/examples/sample_protocol.yml
+-rwxrwxrwx   0 jason     (1000) jason     (1000)     6642 2019-09-18 19:08:46.000000 polypacket-1.0.9/polypacket/poly-make
+-rwxrwxrwx   0 jason     (1000) jason     (1000)     7330 2019-09-18 19:08:42.000000 polypacket-1.0.9/polypacket/poly-packet
+-rwxrwxrwx   0 jason     (1000) jason     (1000)    11764 2019-09-18 18:28:24.000000 polypacket-1.0.9/polypacket/polyservice.py
+-rwxrwxrwx   0 jason     (1000) jason     (1000)    23833 2019-09-18 18:32:16.000000 polypacket-1.0.9/polypacket/protocol.py
+drwxrwxrwx   0 jason     (1000) jason     (1000)        0 2019-09-18 19:09:53.000000 polypacket-1.0.9/polypacket/templates/
+-rwxrwxrwx   0 jason     (1000) jason     (1000)     5296 2019-09-05 16:53:44.000000 polypacket-1.0.9/polypacket/templates/app_template.c
+-rwxrwxrwx   0 jason     (1000) jason     (1000)      727 2019-08-23 16:18:54.000000 polypacket-1.0.9/polypacket/templates/app_template.h
+-rwxrwxrwx   0 jason     (1000) jason     (1000)      895 2019-09-05 14:51:06.000000 polypacket-1.0.9/polypacket/templates/cmake_template.txt
+-rwxrwxrwx   0 jason     (1000) jason     (1000)     9746 2019-09-05 16:48:06.000000 polypacket-1.0.9/polypacket/templates/c_header_template.h
+-rwxrwxrwx   0 jason     (1000) jason     (1000)    16762 2019-09-18 13:42:35.000000 polypacket-1.0.9/polypacket/templates/c_source_template.c
+-rwxrwxrwx   0 jason     (1000) jason     (1000)     4626 2019-09-13 14:48:31.000000 polypacket-1.0.9/polypacket/templates/doc_template.html
+-rwxrwxrwx   0 jason     (1000) jason     (1000)     4935 2019-08-22 14:37:24.000000 polypacket-1.0.9/polypacket/templates/doc_template.md
+-rwxrwxrwx   0 jason     (1000) jason     (1000)     1699 2019-08-22 14:37:24.000000 polypacket-1.0.9/polypacket/templates/javascript_template.js
+-rwxrwxrwx   0 jason     (1000) jason     (1000)      179 2019-08-22 19:08:49.000000 polypacket-1.0.9/polypacket/templates/readme_template.md
+-rwxrwxrwx   0 jason     (1000) jason     (1000)     5357 2019-09-17 14:47:42.000000 polypacket-1.0.9/polypacket/templates/util_main_template.c
+-rwxrwxrwx   0 jason     (1000) jason     (1000)       73 2019-09-18 13:42:35.000000 polypacket-1.0.9/polypacket/__init__.py
+drwxrwxrwx   0 jason     (1000) jason     (1000)        0 2019-09-18 19:09:53.000000 polypacket-1.0.9/polypacket.egg-info/
+-rwxrwxrwx   0 jason     (1000) jason     (1000)        1 2019-09-18 19:09:53.000000 polypacket-1.0.9/polypacket.egg-info/dependency_links.txt
+-rwxrwxrwx   0 jason     (1000) jason     (1000)    17321 2019-09-18 19:09:53.000000 polypacket-1.0.9/polypacket.egg-info/PKG-INFO
+-rwxrwxrwx   0 jason     (1000) jason     (1000)       41 2019-09-18 19:09:53.000000 polypacket-1.0.9/polypacket.egg-info/requires.txt
+-rwxrwxrwx   0 jason     (1000) jason     (1000)      779 2019-09-18 19:09:53.000000 polypacket-1.0.9/polypacket.egg-info/SOURCES.txt
+-rwxrwxrwx   0 jason     (1000) jason     (1000)       11 2019-09-18 19:09:53.000000 polypacket-1.0.9/polypacket.egg-info/top_level.txt
+-rwxrwxrwx   0 jason     (1000) jason     (1000)    13633 2019-09-18 18:34:04.000000 polypacket-1.0.9/README.md
+-rwxrwxrwx   0 jason     (1000) jason     (1000)       38 2019-09-18 19:09:53.000000 polypacket-1.0.9/setup.cfg
+-rwxrwxrwx   0 jason     (1000) jason     (1000)      951 2019-09-18 19:07:52.000000 polypacket-1.0.9/setup.py
```

### Comparing `polypacket-1.0.8/PKG-INFO` & `polypacket-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polypacket
-Version: 1.0.8
+Version: 1.0.9
 Summary: A tool for building protocol services
 Home-page: http://www.up-rev.com/
 Author: Jason Berger
 Author-email: JBerger@up-rev.com
 License: UNKNOWN
 Description: # PolyPacket
         
@@ -223,24 +223,24 @@
         ### poly-packet
         
         the poly-packet tool can be used to test a protocol, or just as a utility for existing devices. The tool features auto-complete and you can get a list of options with 'tab'
         
         terminal 1:
         int the first terminal open the tool and then connect to port 8000
         ```bash
-        poly-packet -i sample_protocol.yml
-        connect udp:8000
+        poly-packet -i sample_protocol.yml -c connect udp:8000
         ```
         
         terminal 2:
-        on the second, open port 8001 and connect to 8000
-        to send a packet, type the name of the packet and then fill in the fields (make sure to use seperating commas)
+        on the second, open port 8001 and connect to 8000.
+        To send a packet, type the name of the packet and then fill in the fields (make sure to use separating commas)
         ```bash
-        poly-packet -i sample_protocol.yml
-        connect udp:8001:8000
+        poly-packet -i sample_protocol.yml -c connect udp:8001:8000
+        
+        #then from the poly-packet terminal:
         Data sensorA: 89 , sensorB: 87 , sensorName: test name  
         ```
         
         
         ### poly-make
         
         poly-make is the tool that will turn the yaml description into c code for projects.
```

### Comparing `polypacket-1.0.8/polypacket/examples/sample_protocol.xml` & `polypacket-1.0.9/polypacket/examples/sample_protocol.xml`

 * *Files identical despite different names*

### Comparing `polypacket-1.0.8/polypacket/examples/sample_protocol.yml` & `polypacket-1.0.9/polypacket/examples/sample_protocol.yml`

 * *Files identical despite different names*

### Comparing `polypacket-1.0.8/polypacket/poly-make` & `polypacket-1.0.9/polypacket/poly-make`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/python3
+#!/usr/bin/env python
 #
 #@file make_protocol.py
 #@brief python script to generate code for PolyPacket
 #@author Jason Berger
 #@date 02/19/2019
 #
```

### Comparing `polypacket-1.0.8/polypacket/poly-packet` & `polypacket-1.0.9/polypacket/poly-packet`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/python3
+#!/usr/bin/env python
 """
 An example of a BufferControl in a full screen layout that offers auto
 completion.
 Important is to make sure that there is a `CompletionsMenu` in the layout,
 otherwise the completions won't be visible.
 """
 from prompt_toolkit.application import Application
@@ -39,17 +39,18 @@
     'connect', 'send'], ignore_case=True)
 
 connect_completer = WordCompleter(['serial:','udp:'],ignore_case=True)
 
 packet_completer = ''
 
 
-outputField = TextArea(style='class:output-win',height=20,multiline=True)
+outputField = TextArea(style='class:output-win',multiline=True)
 outputField.text = "Ctrl-C to quit"
 
+
 # Style.
 style = Style([
     ('output-win', 'bg:#000000 #00ff00'),
     ('input-win', 'bg:#000000 #ffffff'),
     ('line',        '#004400'),
     ('status', 'bg:#004400 #ffffff')
 ])
@@ -74,15 +75,15 @@
                 buff.completer = WordCompleter(fields,ignore_case=True )
 
 # The layout
 inputBuffer = Buffer(completer=command_completer, complete_while_typing=False, multiline=False, on_text_changed=onInputChange)
 #inputBuffer.text = 'SendCmd src: 45, dst: 32, cmd: 4'
 
 #outputWin = Window(BufferControl(buffer=outputField,focusable=False), height=20, style='class:output-win')
-inputWin = Window(BufferControl(buffer=inputBuffer),style='class:input-win')
+inputWin = Window(BufferControl(buffer=inputBuffer), height=4, style='class:input-win')
 body = FloatContainer(
     content=HSplit([
         #outputWin,
         outputField,
         Window(height=1, char='-', style='class:line'),
         inputWin,
     ]),
@@ -217,20 +218,32 @@
 
     packetNames.append('connect')
 
     packet_completer = WordCompleter(packetNames,ignore_case=True)
 
     inputBuffer.completer = packet_completer
 
+    outputField.text = "" #"Ctrl-C to quit"
+    outputField.text += "______     _      ______          _        _   \n"
+    outputField.text += "| ___ \   | |     | ___ \        | |      | |  \n"
+    outputField.text += "| |_/ /__ | |_   _| |_/ /_ _  ___| | _____| |_ \n"
+    outputField.text += "|  __/ _ \| | | | |  __/ _` |/ __| |/ / _ \ __|\n"
+    outputField.text += "| | | (_) | | |_| | | | (_| | (__|   <  __/ |_ \n"
+    outputField.text += "\_|  \___/|_|\__, \_|  \__,_|\___|_|\_\___|\__|    ["+ PROTOCOL.name+ " protocol]\n"
+    outputField.text += "              __/ |                            \n"
+    outputField.text += "             |___/                             \n"
+
     if not args.command == '':
         commands = ' '.join(args.command)
         commands = commands.split(';')
         for com in commands:
             parseCommand(com)
 
+
+
     application.run()
 
 
 def testService(service):
 
     service.addIface("")
     newPacket = service.newPacket('Data')
```

### Comparing `polypacket-1.0.8/polypacket/polyservice.py` & `polypacket-1.0.9/polypacket/polyservice.py`

 * *Files identical despite different names*

### Comparing `polypacket-1.0.8/polypacket/protocol.py` & `polypacket-1.0.9/polypacket/protocol.py`

 * *Files identical despite different names*

### Comparing `polypacket-1.0.8/polypacket/templates/app_template.c` & `polypacket-1.0.9/polypacket/templates/app_template.c`

 * *Files identical despite different names*

### Comparing `polypacket-1.0.8/polypacket/templates/app_template.h` & `polypacket-1.0.9/polypacket/templates/app_template.h`

 * *Files identical despite different names*

### Comparing `polypacket-1.0.8/polypacket/templates/cmake_template.txt` & `polypacket-1.0.9/polypacket/templates/cmake_template.txt`

 * *Files identical despite different names*

### Comparing `polypacket-1.0.8/polypacket/templates/c_header_template.h` & `polypacket-1.0.9/polypacket/templates/c_header_template.h`

 * *Files identical despite different names*

### Comparing `polypacket-1.0.8/polypacket/templates/c_source_template.c` & `polypacket-1.0.9/polypacket/templates/c_source_template.c`

 * *Files identical despite different names*

### Comparing `polypacket-1.0.8/polypacket/templates/doc_template.html` & `polypacket-1.0.9/polypacket/templates/doc_template.html`

 * *Files identical despite different names*

### Comparing `polypacket-1.0.8/polypacket/templates/doc_template.md` & `polypacket-1.0.9/polypacket/templates/doc_template.md`

 * *Files identical despite different names*

### Comparing `polypacket-1.0.8/polypacket/templates/javascript_template.js` & `polypacket-1.0.9/polypacket/templates/javascript_template.js`

 * *Files identical despite different names*

### Comparing `polypacket-1.0.8/polypacket/templates/util_main_template.c` & `polypacket-1.0.9/polypacket/templates/util_main_template.c`

 * *Files identical despite different names*

### Comparing `polypacket-1.0.8/polypacket.egg-info/PKG-INFO` & `polypacket-1.0.9/polypacket.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polypacket
-Version: 1.0.8
+Version: 1.0.9
 Summary: A tool for building protocol services
 Home-page: http://www.up-rev.com/
 Author: Jason Berger
 Author-email: JBerger@up-rev.com
 License: UNKNOWN
 Description: # PolyPacket
         
@@ -223,24 +223,24 @@
         ### poly-packet
         
         the poly-packet tool can be used to test a protocol, or just as a utility for existing devices. The tool features auto-complete and you can get a list of options with 'tab'
         
         terminal 1:
         int the first terminal open the tool and then connect to port 8000
         ```bash
-        poly-packet -i sample_protocol.yml
-        connect udp:8000
+        poly-packet -i sample_protocol.yml -c connect udp:8000
         ```
         
         terminal 2:
-        on the second, open port 8001 and connect to 8000
-        to send a packet, type the name of the packet and then fill in the fields (make sure to use seperating commas)
+        on the second, open port 8001 and connect to 8000.
+        To send a packet, type the name of the packet and then fill in the fields (make sure to use separating commas)
         ```bash
-        poly-packet -i sample_protocol.yml
-        connect udp:8001:8000
+        poly-packet -i sample_protocol.yml -c connect udp:8001:8000
+        
+        #then from the poly-packet terminal:
         Data sensorA: 89 , sensorB: 87 , sensorName: test name  
         ```
         
         
         ### poly-make
         
         poly-make is the tool that will turn the yaml description into c code for projects.
```

### Comparing `polypacket-1.0.8/polypacket.egg-info/SOURCES.txt` & `polypacket-1.0.9/polypacket.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `polypacket-1.0.8/README.md` & `polypacket-1.0.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -215,24 +215,24 @@
 ### poly-packet
 
 the poly-packet tool can be used to test a protocol, or just as a utility for existing devices. The tool features auto-complete and you can get a list of options with 'tab'
 
 terminal 1:
 int the first terminal open the tool and then connect to port 8000
 ```bash
-poly-packet -i sample_protocol.yml
-connect udp:8000
+poly-packet -i sample_protocol.yml -c connect udp:8000
 ```
 
 terminal 2:
-on the second, open port 8001 and connect to 8000
-to send a packet, type the name of the packet and then fill in the fields (make sure to use seperating commas)
+on the second, open port 8001 and connect to 8000.
+To send a packet, type the name of the packet and then fill in the fields (make sure to use separating commas)
 ```bash
-poly-packet -i sample_protocol.yml
-connect udp:8001:8000
+poly-packet -i sample_protocol.yml -c connect udp:8001:8000
+
+#then from the poly-packet terminal:
 Data sensorA: 89 , sensorB: 87 , sensorName: test name  
 ```
 
 
 ### poly-make
 
 poly-make is the tool that will turn the yaml description into c code for projects.
```

### Comparing `polypacket-1.0.8/setup.py` & `polypacket-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
      name='polypacket',
-     version='1.0.08',
+     version='1.0.09',
      author="Jason Berger",
      author_email="JBerger@up-rev.com",
      description="A tool for building protocol services",
      long_description=long_description,
      scripts=['polypacket/poly-packet','polypacket/poly-make'],
      long_description_content_type="text/markdown",
      url="http://www.up-rev.com/",
```

