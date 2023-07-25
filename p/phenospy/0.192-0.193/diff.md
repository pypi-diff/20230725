# Comparing `tmp/phenospy-0.192.tar.gz` & `tmp/phenospy-0.193.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phenospy-0.192.tar", last modified: Tue Jul 25 13:40:16 2023, max compression
+gzip compressed data, was "phenospy-0.193.tar", last modified: Tue Jul 25 13:55:58 2023, max compression
```

## Comparing `phenospy-0.192.tar` & `phenospy-0.193.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 taravser (1128288419) ATKK\hyad-all (984178727)        0 2023-07-25 13:40:16.641677 phenospy-0.192/
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     1080 2023-03-13 19:55:04.000000 phenospy-0.192/LICENSE.txt
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)       31 2023-03-13 20:40:28.000000 phenospy-0.192/MANIFEST.in
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     3385 2023-07-25 13:40:16.641443 phenospy-0.192/PKG-INFO
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     2539 2023-04-18 19:03:17.000000 phenospy-0.192/README.md
-drwxr-xr-x   0 taravser (1128288419) ATKK\hyad-all (984178727)        0 2023-07-25 13:40:16.634366 phenospy-0.192/phenospy/
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)      370 2023-04-03 16:35:02.000000 phenospy-0.192/phenospy/__init__.py
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)    19565 2023-07-25 13:39:11.000000 phenospy-0.192/phenospy/nl_fun.py
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     1109 2023-04-03 16:31:49.000000 phenospy-0.192/phenospy/nl_owlToMd.py
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     2258 2023-04-03 16:50:14.000000 phenospy-0.192/phenospy/nl_owlToMd_fun.py
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     2403 2023-03-28 14:23:07.000000 phenospy-0.192/phenospy/owl_make_phsOntology.py
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)      631 2023-03-28 17:14:38.000000 phenospy-0.192/phenospy/owl_owlready_config.py
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     4013 2023-03-28 18:24:24.000000 phenospy-0.192/phenospy/owl_xml2owl_fun.py
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)    16941 2023-07-25 12:23:12.000000 phenospy-0.192/phenospy/owl_xmlToOwl.py
-drwxr-xr-x   0 taravser (1128288419) ATKK\hyad-all (984178727)        0 2023-07-25 13:40:16.641001 phenospy-0.192/phenospy/package-data/
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     6148 2023-03-28 19:11:16.000000 phenospy-0.192/phenospy/package-data/.DS_Store
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)      591 2023-03-27 19:35:46.000000 phenospy-0.192/phenospy/package-data/phenoscript.obda
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)    18495 2023-03-27 19:35:46.000000 phenospy-0.192/phenospy/package-data/phenoscript.owl
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)      127 2023-03-27 19:35:46.000000 phenospy-0.192/phenospy/package-data/phenoscript.properties
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     3224 2023-04-19 08:58:27.000000 phenospy-0.192/phenospy/package-data/phs-config.yaml
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     7502 2023-03-27 17:52:38.000000 phenospy-0.192/phenospy/package-data/snippets-default.json
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     1065 2023-03-15 14:43:16.000000 phenospy-0.192/phenospy/phs_addXmlMeta.py
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     5390 2023-03-28 18:02:16.000000 phenospy-0.192/phenospy/phs_grammar.py
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     2232 2023-03-28 18:15:48.000000 phenospy-0.192/phenospy/phs_mainConvert.py
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     3898 2023-03-28 18:28:37.000000 phenospy-0.192/phenospy/phs_parser_fun.py
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     3153 2023-03-28 18:28:31.000000 phenospy-0.192/phenospy/phs_various_fun.py
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)    14872 2023-03-28 18:12:47.000000 phenospy-0.192/phenospy/phs_xml.py
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     6508 2023-03-28 18:13:03.000000 phenospy-0.192/phenospy/phs_xmlTranslateTerms.py
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     7009 2023-03-28 17:14:38.000000 phenospy-0.192/phenospy/snips_fun.py
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)    10953 2023-04-19 14:00:48.000000 phenospy-0.192/phenospy/snips_makeFromYaml.py
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     5312 2023-04-19 15:37:02.000000 phenospy-0.192/phenospy/snips_readFromJSON.py
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     2366 2023-04-17 06:49:33.000000 phenospy-0.192/phenospy/xml_recodeThis.py
-drwxr-xr-x   0 taravser (1128288419) ATKK\hyad-all (984178727)        0 2023-07-25 13:40:16.637821 phenospy-0.192/phenospy.egg-info/
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     3385 2023-07-25 13:40:16.000000 phenospy-0.192/phenospy.egg-info/PKG-INFO
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)      944 2023-07-25 13:40:16.000000 phenospy-0.192/phenospy.egg-info/SOURCES.txt
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)        1 2023-07-25 13:40:16.000000 phenospy-0.192/phenospy.egg-info/dependency_links.txt
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)       43 2023-07-25 13:40:16.000000 phenospy-0.192/phenospy.egg-info/requires.txt
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)        9 2023-07-25 13:40:16.000000 phenospy-0.192/phenospy.egg-info/top_level.txt
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)       38 2023-07-25 13:40:16.641742 phenospy-0.192/setup.cfg
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     1239 2023-07-25 13:39:15.000000 phenospy-0.192/setup.py
+drwxr-xr-x   0 taravser (1128288419) ATKK\hyad-all (984178727)        0 2023-07-25 13:55:58.095028 phenospy-0.193/
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     1080 2023-03-13 19:55:04.000000 phenospy-0.193/LICENSE.txt
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)       31 2023-03-13 20:40:28.000000 phenospy-0.193/MANIFEST.in
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     3385 2023-07-25 13:55:58.094844 phenospy-0.193/PKG-INFO
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     2539 2023-04-18 19:03:17.000000 phenospy-0.193/README.md
+drwxr-xr-x   0 taravser (1128288419) ATKK\hyad-all (984178727)        0 2023-07-25 13:55:58.090191 phenospy-0.193/phenospy/
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)      370 2023-04-03 16:35:02.000000 phenospy-0.193/phenospy/__init__.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)    19831 2023-07-25 13:55:55.000000 phenospy-0.193/phenospy/nl_fun.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     1109 2023-04-03 16:31:49.000000 phenospy-0.193/phenospy/nl_owlToMd.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     2258 2023-04-03 16:50:14.000000 phenospy-0.193/phenospy/nl_owlToMd_fun.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     2403 2023-03-28 14:23:07.000000 phenospy-0.193/phenospy/owl_make_phsOntology.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)      631 2023-03-28 17:14:38.000000 phenospy-0.193/phenospy/owl_owlready_config.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     4013 2023-03-28 18:24:24.000000 phenospy-0.193/phenospy/owl_xml2owl_fun.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)    16941 2023-07-25 12:23:12.000000 phenospy-0.193/phenospy/owl_xmlToOwl.py
+drwxr-xr-x   0 taravser (1128288419) ATKK\hyad-all (984178727)        0 2023-07-25 13:55:58.094454 phenospy-0.193/phenospy/package-data/
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     6148 2023-03-28 19:11:16.000000 phenospy-0.193/phenospy/package-data/.DS_Store
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)      591 2023-03-27 19:35:46.000000 phenospy-0.193/phenospy/package-data/phenoscript.obda
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)    18495 2023-03-27 19:35:46.000000 phenospy-0.193/phenospy/package-data/phenoscript.owl
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)      127 2023-03-27 19:35:46.000000 phenospy-0.193/phenospy/package-data/phenoscript.properties
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     3224 2023-04-19 08:58:27.000000 phenospy-0.193/phenospy/package-data/phs-config.yaml
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     7502 2023-03-27 17:52:38.000000 phenospy-0.193/phenospy/package-data/snippets-default.json
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     1065 2023-03-15 14:43:16.000000 phenospy-0.193/phenospy/phs_addXmlMeta.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     5390 2023-03-28 18:02:16.000000 phenospy-0.193/phenospy/phs_grammar.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     2232 2023-03-28 18:15:48.000000 phenospy-0.193/phenospy/phs_mainConvert.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     3898 2023-03-28 18:28:37.000000 phenospy-0.193/phenospy/phs_parser_fun.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     3153 2023-03-28 18:28:31.000000 phenospy-0.193/phenospy/phs_various_fun.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)    14872 2023-03-28 18:12:47.000000 phenospy-0.193/phenospy/phs_xml.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     6508 2023-03-28 18:13:03.000000 phenospy-0.193/phenospy/phs_xmlTranslateTerms.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     7009 2023-03-28 17:14:38.000000 phenospy-0.193/phenospy/snips_fun.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)    10953 2023-04-19 14:00:48.000000 phenospy-0.193/phenospy/snips_makeFromYaml.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     5312 2023-04-19 15:37:02.000000 phenospy-0.193/phenospy/snips_readFromJSON.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     2366 2023-04-17 06:49:33.000000 phenospy-0.193/phenospy/xml_recodeThis.py
+drwxr-xr-x   0 taravser (1128288419) ATKK\hyad-all (984178727)        0 2023-07-25 13:55:58.091613 phenospy-0.193/phenospy.egg-info/
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     3385 2023-07-25 13:55:58.000000 phenospy-0.193/phenospy.egg-info/PKG-INFO
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)      944 2023-07-25 13:55:58.000000 phenospy-0.193/phenospy.egg-info/SOURCES.txt
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)        1 2023-07-25 13:55:58.000000 phenospy-0.193/phenospy.egg-info/dependency_links.txt
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)       43 2023-07-25 13:55:58.000000 phenospy-0.193/phenospy.egg-info/requires.txt
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)        9 2023-07-25 13:55:58.000000 phenospy-0.193/phenospy.egg-info/top_level.txt
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)       38 2023-07-25 13:55:58.095139 phenospy-0.193/setup.cfg
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     1239 2023-07-25 13:55:45.000000 phenospy-0.193/setup.py
```

### Comparing `phenospy-0.192/LICENSE.txt` & `phenospy-0.193/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `phenospy-0.192/PKG-INFO` & `phenospy-0.193/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phenospy
-Version: 0.192
+Version: 0.193
 Summary: Tools for making and processing computable phenotype descriptions
 Home-page: https://github.com/sergeitarasov/PhenoScript
 Author: Sergei Tarasov
 Author-email: sergei.tarasov@helsinki.fi
 License: MIT
 Project-URL: Project Logo, https://raw.githubusercontent.com/sergeitarasov/PhenoScript/main/Phenoscript_logo.png
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `phenospy-0.192/README.md` & `phenospy-0.193/README.md`

 * *Files identical despite different names*

### Comparing `phenospy-0.192/phenospy/nl_fun.py` & `phenospy-0.193/phenospy/nl_fun.py`

 * *Files 1% similar despite different names*

```diff
@@ -419,14 +419,19 @@
                 # txt = txt + traverseOntoMark_Overleaf(value, tabs=tabs+"\t", visited_nodes=visited_nodes)
                 txt = txt + traverseGraphForNL(onto, value, tabs=tabs+tab_char, tab_char = tab_char, visited_nodes=visited_nodes)
         return txt
     if len(triples) == 0:
         # print('TRIPR len=0')
         return ";"
 
+def check_string_pattern_complete(s):
+    if (s.startswith(',') or s.startswith(':')) and not s.endswith(';'):
+        return True
+    return False
+
 # -----------------------------------------
 # Render NL when traversing graph
 # -----------------------------------------
 # obo.RO_0015007 increased_in_magnitude_relative_to http://purl.obolibrary.org/obo/RO_0015007
 # obo.RO_0015008 decreased in magnitude relative to http://purl.obolibrary.org/obo/RO_0015008
 def renderNL(x, onto):
     obo = onto.get_namespace("http://purl.obolibrary.org/obo/")
@@ -445,15 +450,19 @@
             return " [%s](%s)" % (x.label.first(), x.iri)
     elif issubclass(x, owl.AnnotationProperty):
         return ""
     elif isinstance(x, (int, float)):
         return " %s;" % str(x)
     elif isinstance(x, str):
         #return x
-        return "%s" % x
+        #return "%s" % x
+        if check_string_pattern_complete(x):
+           return "%s" % x
+        else:
+            return  " %s" % x
 
 
 # -----------------------------------------
 # Make NL desciptions in Md format
 # -----------------------------------------
 # ind0 = onto.search(label = 'org_Grebennikovius_basilewskyi')[0]
 # def makeMarkdown(onto, ind0, file_save=None, verbose=False):
```

### Comparing `phenospy-0.192/phenospy/nl_owlToMd.py` & `phenospy-0.193/phenospy/nl_owlToMd.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.192/phenospy/nl_owlToMd_fun.py` & `phenospy-0.193/phenospy/nl_owlToMd_fun.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.192/phenospy/owl_make_phsOntology.py` & `phenospy-0.193/phenospy/owl_make_phsOntology.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.192/phenospy/owl_owlready_config.py` & `phenospy-0.193/phenospy/owl_owlready_config.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.192/phenospy/owl_xml2owl_fun.py` & `phenospy-0.193/phenospy/owl_xml2owl_fun.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.192/phenospy/owl_xmlToOwl.py` & `phenospy-0.193/phenospy/owl_xmlToOwl.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.192/phenospy/package-data/.DS_Store` & `phenospy-0.193/phenospy/package-data/.DS_Store`

 * *Files identical despite different names*

### Comparing `phenospy-0.192/phenospy/package-data/phenoscript.obda` & `phenospy-0.193/phenospy/package-data/phenoscript.obda`

 * *Files identical despite different names*

### Comparing `phenospy-0.192/phenospy/package-data/phenoscript.owl` & `phenospy-0.193/phenospy/package-data/phenoscript.owl`

 * *Files identical despite different names*

### Comparing `phenospy-0.192/phenospy/package-data/phs-config.yaml` & `phenospy-0.193/phenospy/package-data/phs-config.yaml`

 * *Files identical despite different names*

### Comparing `phenospy-0.192/phenospy/package-data/snippets-default.json` & `phenospy-0.193/phenospy/package-data/snippets-default.json`

 * *Files identical despite different names*

### Comparing `phenospy-0.192/phenospy/phs_addXmlMeta.py` & `phenospy-0.193/phenospy/phs_addXmlMeta.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.192/phenospy/phs_grammar.py` & `phenospy-0.193/phenospy/phs_grammar.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.192/phenospy/phs_mainConvert.py` & `phenospy-0.193/phenospy/phs_mainConvert.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.192/phenospy/phs_parser_fun.py` & `phenospy-0.193/phenospy/phs_parser_fun.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.192/phenospy/phs_various_fun.py` & `phenospy-0.193/phenospy/phs_various_fun.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.192/phenospy/phs_xml.py` & `phenospy-0.193/phenospy/phs_xml.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.192/phenospy/phs_xmlTranslateTerms.py` & `phenospy-0.193/phenospy/phs_xmlTranslateTerms.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.192/phenospy/snips_fun.py` & `phenospy-0.193/phenospy/snips_fun.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.192/phenospy/snips_makeFromYaml.py` & `phenospy-0.193/phenospy/snips_makeFromYaml.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.192/phenospy/snips_readFromJSON.py` & `phenospy-0.193/phenospy/snips_readFromJSON.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.192/phenospy/xml_recodeThis.py` & `phenospy-0.193/phenospy/xml_recodeThis.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.192/phenospy.egg-info/PKG-INFO` & `phenospy-0.193/phenospy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phenospy
-Version: 0.192
+Version: 0.193
 Summary: Tools for making and processing computable phenotype descriptions
 Home-page: https://github.com/sergeitarasov/PhenoScript
 Author: Sergei Tarasov
 Author-email: sergei.tarasov@helsinki.fi
 License: MIT
 Project-URL: Project Logo, https://raw.githubusercontent.com/sergeitarasov/PhenoScript/main/Phenoscript_logo.png
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `phenospy-0.192/phenospy.egg-info/SOURCES.txt` & `phenospy-0.193/phenospy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phenospy-0.192/setup.py` & `phenospy-0.193/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='phenospy',
-    version='0.192',
+    version='0.193',
     packages=find_packages(exclude=['tests*', 'devel*', 'build*']),
     license='MIT',
     description='Tools for making and processing computable phenotype descriptions',
     long_description_content_type="text/markdown",
     long_description=open('README.md').read(),
     install_requires=['Owlready2',
                       'PyYAML',
```

