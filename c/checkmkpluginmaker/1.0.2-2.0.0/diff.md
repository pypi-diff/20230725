# Comparing `tmp/checkmkpluginmaker-1.0.2.tar.gz` & `tmp/checkmkpluginmaker-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "checkmkpluginmaker-1.0.2.tar", max compression
+gzip compressed data, was "checkmkpluginmaker-2.0.0.tar", max compression
```

## Comparing `checkmkpluginmaker-1.0.2.tar` & `checkmkpluginmaker-2.0.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      335 2023-07-24 06:59:59.933909 checkmkpluginmaker-1.0.2/README.md
--rw-r--r--   0        0        0      556 2023-07-24 06:59:59.933909 checkmkpluginmaker-1.0.2/pluginmaker/__init__.py
--rw-r--r--   0        0        0       24 2023-07-24 06:59:59.933909 checkmkpluginmaker-1.0.2/pluginmaker/cookiecutter_templates/__init__.py
--rw-r--r--   0        0        0      806 2023-07-24 06:59:59.933909 checkmkpluginmaker-1.0.2/pluginmaker/cookiecutter_templates/cmk_plugin/cookiecutter.json
--rw-r--r--   0        0        0     1472 2023-07-24 06:59:59.933909 checkmkpluginmaker-1.0.2/pluginmaker/cookiecutter_templates/cmk_plugin/hooks/pre_gen_project.py
--rw-r--r--   0        0        0      327 2023-07-24 06:59:59.933909 checkmkpluginmaker-1.0.2/pluginmaker/cookiecutter_templates/cmk_plugin/setup.py
--rw-r--r--   0        0        0     1811 2023-07-24 06:59:59.933909 checkmkpluginmaker-1.0.2/pluginmaker/cookiecutter_templates/cmk_plugin/{{cookiecutter.project_slug}}/Makefile
--rw-r--r--   0        0        0     1175 2023-07-24 06:59:59.933909 checkmkpluginmaker-1.0.2/pluginmaker/cookiecutter_templates/cmk_plugin/{{cookiecutter.project_slug}}/agent_invoker/agent_{{cookiecutter.agent_id}}
--rw-r--r--   0        0        0     4063 2023-07-24 06:59:59.933909 checkmkpluginmaker-1.0.2/pluginmaker/cookiecutter_templates/cmk_plugin/{{cookiecutter.project_slug}}/agent_special/agent_{{cookiecutter.agent_id}}
--rw-r--r--   0        0        0     1058 2023-07-24 06:59:59.933909 checkmkpluginmaker-1.0.2/pluginmaker/cookiecutter_templates/cmk_plugin/{{cookiecutter.project_slug}}/mkp/config
--rw-r--r--   0        0        0      848 2023-07-24 06:59:59.933909 checkmkpluginmaker-1.0.2/pluginmaker/cookiecutter_templates/cmk_plugin/{{cookiecutter.project_slug}}/plugin/service_{{cookiecutter.agent_id}}.py
--rw-r--r--   0        0        0     1888 2023-07-24 06:59:59.933909 checkmkpluginmaker-1.0.2/pluginmaker/cookiecutter_templates/cmk_plugin/{{cookiecutter.project_slug}}/wato/{{cookiecutter.agent_id}}_register.py
--rw-r--r--   0        0        0     1128 2023-07-24 06:59:59.933909 checkmkpluginmaker-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     1365 1970-01-01 00:00:00.000000 checkmkpluginmaker-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0      335 2023-07-25 00:40:18.705034 checkmkpluginmaker-2.0.0/README.md
+-rw-r--r--   0        0        0      556 2023-07-25 00:40:18.709034 checkmkpluginmaker-2.0.0/pluginmaker/__init__.py
+-rw-r--r--   0        0        0       24 2023-07-25 00:40:18.709034 checkmkpluginmaker-2.0.0/pluginmaker/cookiecutter_templates/__init__.py
+-rw-r--r--   0        0        0      806 2023-07-25 00:40:18.709034 checkmkpluginmaker-2.0.0/pluginmaker/cookiecutter_templates/cmk_plugin/cookiecutter.json
+-rw-r--r--   0        0        0     1472 2023-07-25 00:40:18.709034 checkmkpluginmaker-2.0.0/pluginmaker/cookiecutter_templates/cmk_plugin/hooks/pre_gen_project.py
+-rw-r--r--   0        0        0      327 2023-07-25 00:40:18.709034 checkmkpluginmaker-2.0.0/pluginmaker/cookiecutter_templates/cmk_plugin/setup.py
+-rw-r--r--   0        0        0     1972 2023-07-25 00:40:18.709034 checkmkpluginmaker-2.0.0/pluginmaker/cookiecutter_templates/cmk_plugin/{{cookiecutter.project_slug}}/Makefile
+-rw-r--r--   0        0        0      890 2023-07-25 00:40:18.709034 checkmkpluginmaker-2.0.0/pluginmaker/cookiecutter_templates/cmk_plugin/{{cookiecutter.project_slug}}/agent_invoker/agent_{{cookiecutter.agent_id}}
+-rw-r--r--   0        0        0     4630 2023-07-25 00:40:18.709034 checkmkpluginmaker-2.0.0/pluginmaker/cookiecutter_templates/cmk_plugin/{{cookiecutter.project_slug}}/agent_special/agent_{{cookiecutter.agent_id}}
+-rw-r--r--   0        0        0     1058 2023-07-25 00:40:18.709034 checkmkpluginmaker-2.0.0/pluginmaker/cookiecutter_templates/cmk_plugin/{{cookiecutter.project_slug}}/mkp/config
+-rw-r--r--   0        0        0     3549 2023-07-25 00:40:18.709034 checkmkpluginmaker-2.0.0/pluginmaker/cookiecutter_templates/cmk_plugin/{{cookiecutter.project_slug}}/plugin/service_{{cookiecutter.agent_id}}.py
+-rw-r--r--   0        0        0     2585 2023-07-25 00:40:18.709034 checkmkpluginmaker-2.0.0/pluginmaker/cookiecutter_templates/cmk_plugin/{{cookiecutter.project_slug}}/wato/{{cookiecutter.agent_id}}_register.py
+-rw-r--r--   0        0        0     1128 2023-07-25 00:40:18.709034 checkmkpluginmaker-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1365 1970-01-01 00:00:00.000000 checkmkpluginmaker-2.0.0/PKG-INFO
```

### Comparing `checkmkpluginmaker-1.0.2/pluginmaker/__init__.py` & `checkmkpluginmaker-2.0.0/pluginmaker/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """Entry point of my coca tools
 """
 import os
 import sys
 from cookiecutter.main import cookiecutter
 
 
-__version__ = '1.0.2'
+__version__ = '2.0.0'
 BASE_PATH = os.path.dirname(os.path.abspath(__file__))
 TEMPLATE_PATH = os.path.join(BASE_PATH, 'cookiecutter_templates')
 
 
 def welcome():
     """Say welcome to users"""
     print('I am , welcome to CheckMK Plugin Maker')
```

### Comparing `checkmkpluginmaker-1.0.2/pluginmaker/cookiecutter_templates/cmk_plugin/cookiecutter.json` & `checkmkpluginmaker-2.0.0/pluginmaker/cookiecutter_templates/cmk_plugin/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `checkmkpluginmaker-1.0.2/pluginmaker/cookiecutter_templates/cmk_plugin/hooks/pre_gen_project.py` & `checkmkpluginmaker-2.0.0/pluginmaker/cookiecutter_templates/cmk_plugin/hooks/pre_gen_project.py`

 * *Files identical despite different names*

### Comparing `checkmkpluginmaker-1.0.2/pluginmaker/cookiecutter_templates/cmk_plugin/{{cookiecutter.project_slug}}/Makefile` & `checkmkpluginmaker-2.0.0/pluginmaker/cookiecutter_templates/cmk_plugin/{{cookiecutter.project_slug}}/Makefile`

 * *Files 14% similar despite different names*

```diff
@@ -3,56 +3,63 @@
 
 AGENT_PATH=/usr/lib/check_mk_agent/plugins/
 PLUGIN_PATH=${SITE_PATH}/local/lib/check_mk/base/plugins/agent_based
 WATO_PATH=${SITE_PATH}/local/share/check_mk/web/plugins/wato
 AGENT_SPECIAL_PATH=${SITE_PATH}/local/share/check_mk/agents/special
 CHECKS_PATH=${SITE_PATH}/local/share/check_mk/checks
 
-CMK_RUN_HOST={{cookiecutter.cmk_dev_hostname}}
-
-
-# run in OMD[site]
-dev-check-agent:
-	cmk -d ${CMK_RUN_HOST}
-
-# run in OMD[site]
-dev-debug-agent:
-	cmk --debug --checks={{cookiecutter.agent_id}} -vvn ${CMK_RUN_HOST}
 
-# run in OMD[site]
-dev-detect-plugins:
-	cmk --detect-plugins={{cookiecutter.agent_id}} -vI ${CMK_RUN_HOST}
+CMK_RUN_HOST={{cookiecutter.cmk_dev_hostname}}
 
 
 PROJECT_DIR={{cookiecutter.project_slug}}
 AGENT_ID={{cookiecutter.agent_id}}
 dev-deploy-plugin:
 #	agent
-	sudo cp ./${PROJECT_DIR}/agent_special/agent_${AGENT_ID} ${AGENT_SPECIAL_PATH}/agent_${AGENT_ID}
+	sudo cp ./agent_special/agent_${AGENT_ID} ${AGENT_SPECIAL_PATH}/agent_${AGENT_ID}
 	chmod +x ${AGENT_SPECIAL_PATH}/agent_${AGENT_ID}
 #	agent invoker
-	sudo cp ./${PROJECT_DIR}/agent_invoker/agent_${AGENT_ID} ${CHECKS_PATH}/agent_${AGENT_ID}
+	sudo cp ./agent_invoker/agent_${AGENT_ID} ${CHECKS_PATH}/agent_${AGENT_ID}
 	chmod +x ${CHECKS_PATH}/agent_${AGENT_ID}
 #	wato
-	sudo cp ./${PROJECT_DIR}/wato/${AGENT_ID}_register.py ${WATO_PATH}/${AGENT_ID}_register.py
+	sudo cp ./wato/${AGENT_ID}_register.py ${WATO_PATH}/${AGENT_ID}_register.py
 #	service check
-	sudo cp ./${PROJECT_DIR}/plugin/service_${AGENT_ID}.py ${PLUGIN_PATH}/service_${AGENT_ID}.py
+	sudo cp ./plugin/service_${AGENT_ID}.py ${PLUGIN_PATH}/service_${AGENT_ID}.py
 
 	omd restart ${SITE}
 
 
 dev-undeploy-plugin:
 	rm -rf ${AGENT_SPECIAL_PATH}/agent_${AGENT_ID}
 	rm -rf ${CHECKS_PATH}/agent_${AGENT_ID}
 	rm -rf ${WATO_PATH}/${AGENT_ID}_register.py
 	rm -rf ${PLUGIN_PATH}/service_${AGENT_ID}.py
 
 
-# create MKP, run in OMD[site]
+# create MKP
 # mkp config file should be at var/check_mk/packages (in OMD[site])
 dev-create-mkp:
-	cp ./${PROJECT_DIR}/mkp/config ~/var/check_mk/packages/{{cookiecutter.agent_id}}
+	cp ./mkp/config ${SITE_PATH}/var/check_mk/packages/{{cookiecutter.agent_id}}
 
 
+# pack MKP, run in OMD[site]
+# mkp config file should be at var/check_mk/packages (in OMD[site])
 dev-pack-kmp: 
 	mkp pack {{cookiecutter.agent_id}}
 	ll | grep {{cookiecutter.agent_id}}
+
+
+dev-copy-makefile-to-site:
+	mkdir -p ${SITE_PATH}/dev/{{cookiecutter.agent_id}}
+	cp Makefile ${SITE_PATH}/dev/{{cookiecutter.agent_id}}/Makefile
+
+# run in OMD[site]
+dev-check-agent:
+	cmk -d ${CMK_RUN_HOST}
+
+# run in OMD[site]
+dev-debug-agent:
+	cmk --debug --checks={{cookiecutter.agent_id}} -vvn ${CMK_RUN_HOST}
+
+# run in OMD[site]
+dev-detect-plugins:
+	cmk --detect-plugins={{cookiecutter.agent_id}} -vI ${CMK_RUN_HOST}
```

### Comparing `checkmkpluginmaker-1.0.2/pluginmaker/cookiecutter_templates/cmk_plugin/{{cookiecutter.project_slug}}/agent_invoker/agent_{{cookiecutter.agent_id}}` & `checkmkpluginmaker-2.0.0/pluginmaker/cookiecutter_templates/cmk_plugin/{{cookiecutter.project_slug}}/agent_invoker/agent_{{cookiecutter.agent_id}}`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 #!/usr/bin/env python3
 # copy this file to local/share/check_mk/checks
 
 # -----------------------------
 # Function get params in this case is port, passed via WATO agent rule cunfiguration, hostname and ip addres of host, 
 # for which agent will be invoked 
-#
+import json
+
+
 def agent_myspecal_arguments(params, hostname, ipaddress):
     args = []
     args += ["-H", ipaddress]       # map to host in agent
-    args += ["-C", 'FPTHCM123']     # map to community in agent
-    args += ["-k", params.get('name')]      #  get from UI (wato file) then push to agent parameter name
-    args += ["--w", params['warning']]      #  get from UI (wato file) then push to agent parameter warning
-    args += ["--c", params['critical']]     #  get from UI (wato file) then push to agent parameter critical
-    args += ["--oid", params['oid']]        #  get from UI (wato file) then push to agent parameter oid
+    args += ["-C", params.get('community', 'FPTHCM123')]     # map to community in agent
+    services = params.get('services', [])
+    if services:
+        args += ['-S', json.dumps(services)]
     return args
 
 # -----------------------------
 # register invoke function for our agent
 # key value for this dictionary is name part from register datasource of our agent (name="special_agents:myspecial" remember?)
 #
 special_agent_info['{{cookiecutter.agent_id}}'] = agent_myspecal_arguments
```

### Comparing `checkmkpluginmaker-1.0.2/pluginmaker/cookiecutter_templates/cmk_plugin/{{cookiecutter.project_slug}}/mkp/config` & `checkmkpluginmaker-2.0.0/pluginmaker/cookiecutter_templates/cmk_plugin/{{cookiecutter.project_slug}}/mkp/config`

 * *Files identical despite different names*

### Comparing `checkmkpluginmaker-1.0.2/pluginmaker/cookiecutter_templates/cmk_plugin/{{cookiecutter.project_slug}}/wato/{{cookiecutter.agent_id}}_register.py` & `checkmkpluginmaker-2.0.0/pluginmaker/cookiecutter_templates/cmk_plugin/{{cookiecutter.project_slug}}/wato/{{cookiecutter.agent_id}}_register.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,44 +2,60 @@
 # to local/share/check_mk/web/plugins/wato
 
 #import required to register agent
 from cmk.gui.valuespec import (
     Dictionary,
     Integer,
     TextInput,
-    TextAscii
+    TextAscii,
+    ListOf,
+    Tuple
 )
 from cmk.gui.plugins.wato import (
     IndividualOrStoredPassword,
     RulespecGroup,
     monitoring_macro_help,
     rulespec_group_registry,
     rulespec_registry,
     HostRulespec,
 )
 #import structure where special agent will be registered
 from cmk.gui.plugins.wato.datasource_programs import RulespecGroupDatasourcePrograms
 
+
 #Some WATO form definition, to ask user for port number
 def _valuespec_special_agent_myspecial():
     return Dictionary(
         title=_("{{cookiecutter.wato_title}}"),
         help=_("{{cookiecutter.wato_description}}"),
         optional_keys=[],
         elements=[
-            ("name", TextAscii(title=_("Name displayed on Service check"), default_value="Default")),
-            ("warning", Integer(title=_("Warning threshold"), default_value=-100)),
-            ("critical", Integer(title=_("Critical threshold"), default_value=-150)),
-            (
-                "oid", 
-                TextAscii(
-                    title=_("oid value"), 
-                    default_value='1.3.6.1.4.1.3607.2.30.1.1.1.3.16395.2.10'  # default value, you could change   
+            ( 
+                "services",     # DO NOT CHANGE THIS LINE
+                ListOf(         # DO NOT CHANGE THIS LINE
+                    Dictionary(
+                        title=_("Interface"),   
+                        optional_keys = [],
+                        elements = [        # modify if you need, if bellow lines modified, change in agent code parse_input and handle_service
+                            ("card_name", TextAscii(title = _("Card name"),)),
+                            ("snmp_oid", TextAscii(title=_("SNMP Oid"), default_value="1.3.6.1.4.1.3607.2.30.1.1.1.3.16395.2.10"),),
+                            ("parameters", Tuple(
+                                elements=[
+                                    Integer(title=_("Warning threshold"), default_value=-100),
+                                    Integer(title=_("Critical threshold"), default_value=-150),
+                                    
+                                ]
+                            ))
+                            
+                        ],
+                    ),
+                    help=_("Hello check me"),
+                    title = _("Services"),
                 )
-            ),
+            ),  
         ],
         # Add or remove elements on your need
     )
 
 # -------------------------------------
 # All set, DO NOT MODIFY
 # In that piece of code we registering Special Agent
```

### Comparing `checkmkpluginmaker-1.0.2/pyproject.toml` & `checkmkpluginmaker-2.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "checkmkpluginmaker"
-version = "1.0.2"
+version = "2.0.0"
 description = ""
 authors = ["NhanDD3 <nhandd3@fpt.com>"]
 readme = "README.md"
 packages = [{include = "pluginmaker"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8"
```

### Comparing `checkmkpluginmaker-1.0.2/PKG-INFO` & `checkmkpluginmaker-2.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: checkmkpluginmaker
-Version: 1.0.2
+Version: 2.0.0
 Summary: 
 Author: NhanDD3
 Author-email: nhandd3@fpt.com
 Requires-Python: >=3.8
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

