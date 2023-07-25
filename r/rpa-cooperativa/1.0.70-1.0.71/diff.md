# Comparing `tmp/rpa_cooperativa-1.0.70.tar.gz` & `tmp/rpa_cooperativa-1.0.71.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpa_cooperativa-1.0.70.tar", last modified: Fri Jul 21 19:52:08 2023, max compression
+gzip compressed data, was "rpa_cooperativa-1.0.71.tar", last modified: Tue Jul 25 11:34:03 2023, max compression
```

## Comparing `rpa_cooperativa-1.0.70.tar` & `rpa_cooperativa-1.0.71.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 19:52:08.836005 rpa_cooperativa-1.0.70/
--rw-rw-rw-   0        0        0     1115 2023-03-09 01:05:15.000000 rpa_cooperativa-1.0.70/LICENSE
--rw-rw-rw-   0        0        0     6969 2023-07-21 19:52:08.832936 rpa_cooperativa-1.0.70/PKG-INFO
--rw-rw-rw-   0        0        0     5824 2023-07-13 15:55:54.000000 rpa_cooperativa-1.0.70/README.md
-drwxrwxrwx   0        0        0        0 2023-07-21 19:52:08.677143 rpa_cooperativa-1.0.70/rpa_coop/
--rw-rw-rw-   0        0        0      613 2023-07-21 18:26:52.000000 rpa_cooperativa-1.0.70/rpa_coop/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 19:52:08.774132 rpa_cooperativa-1.0.70/rpa_coop/img/
--rw-rw-rw-   0        0        0      140 2023-03-16 01:30:18.000000 rpa_cooperativa-1.0.70/rpa_coop/img/hash
--rw-rw-rw-   0        0        0     2980 2023-03-09 16:48:20.000000 rpa_cooperativa-1.0.70/rpa_coop/img/relatorios_azul.PNG
--rw-rw-rw-   0        0        0     3576 2023-03-09 16:47:53.000000 rpa_cooperativa-1.0.70/rpa_coop/img/relatorios_verde.PNG
--rw-rw-rw-   0        0        0      379 2023-05-19 19:03:26.000000 rpa_cooperativa-1.0.70/rpa_coop/img/sacg_branco.PNG
--rw-rw-rw-   0        0        0      463 2023-06-01 13:04:34.000000 rpa_cooperativa-1.0.70/rpa_coop/img/sagc_verde.PNG
--rw-rw-rw-   0        0        0      384 2023-02-28 19:53:19.000000 rpa_cooperativa-1.0.70/rpa_coop/img/siac_amarelo.PNG
--rw-rw-rw-   0        0        0      370 2023-04-17 14:08:47.000000 rpa_cooperativa-1.0.70/rpa_coop/img/siac_branco.PNG
--rw-rw-rw-   0        0        0      364 2023-04-17 14:10:18.000000 rpa_cooperativa-1.0.70/rpa_coop/img/siat_amarelo.PNG
--rw-rw-rw-   0        0        0      349 2023-02-28 19:53:39.000000 rpa_cooperativa-1.0.70/rpa_coop/img/siat_branco.PNG
--rw-rw-rw-   0        0        0     6079 2023-03-09 16:47:31.000000 rpa_cooperativa-1.0.70/rpa_coop/img/transacional_azul.PNG
--rw-rw-rw-   0        0        0     6652 2023-03-09 16:46:38.000000 rpa_cooperativa-1.0.70/rpa_coop/img/transacional_verde.PNG
--rw-rw-rw-   0        0        0   104247 2023-07-21 19:51:34.000000 rpa_cooperativa-1.0.70/rpa_coop/rpa_coop.py
-drwxrwxrwx   0        0        0        0 2023-07-21 19:52:08.824759 rpa_cooperativa-1.0.70/rpa_cooperativa.egg-info/
--rw-rw-rw-   0        0        0     6969 2023-07-21 19:52:08.000000 rpa_cooperativa-1.0.70/rpa_cooperativa.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      631 2023-07-21 19:52:08.000000 rpa_cooperativa-1.0.70/rpa_cooperativa.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 19:52:08.000000 rpa_cooperativa-1.0.70/rpa_cooperativa.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-21 19:52:08.000000 rpa_cooperativa-1.0.70/rpa_cooperativa.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      581 2023-07-21 19:52:08.000000 rpa_cooperativa-1.0.70/rpa_cooperativa.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-21 19:52:08.000000 rpa_cooperativa-1.0.70/rpa_cooperativa.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-21 19:52:08.837016 rpa_cooperativa-1.0.70/setup.cfg
--rw-rw-rw-   0        0        0     2350 2023-07-21 19:51:09.000000 rpa_cooperativa-1.0.70/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 11:34:03.391317 rpa_cooperativa-1.0.71/
+-rw-rw-rw-   0        0        0     1115 2023-03-09 01:05:15.000000 rpa_cooperativa-1.0.71/LICENSE
+-rw-rw-rw-   0        0        0     6969 2023-07-25 11:34:03.388395 rpa_cooperativa-1.0.71/PKG-INFO
+-rw-rw-rw-   0        0        0     5824 2023-07-13 15:55:54.000000 rpa_cooperativa-1.0.71/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 11:34:03.271074 rpa_cooperativa-1.0.71/rpa_coop/
+-rw-rw-rw-   0        0        0      613 2023-07-21 18:26:52.000000 rpa_cooperativa-1.0.71/rpa_coop/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 11:34:03.353936 rpa_cooperativa-1.0.71/rpa_coop/img/
+-rw-rw-rw-   0        0        0      140 2023-03-16 01:30:18.000000 rpa_cooperativa-1.0.71/rpa_coop/img/hash
+-rw-rw-rw-   0        0        0     2980 2023-03-09 16:48:20.000000 rpa_cooperativa-1.0.71/rpa_coop/img/relatorios_azul.PNG
+-rw-rw-rw-   0        0        0     3576 2023-03-09 16:47:53.000000 rpa_cooperativa-1.0.71/rpa_coop/img/relatorios_verde.PNG
+-rw-rw-rw-   0        0        0      379 2023-05-19 19:03:26.000000 rpa_cooperativa-1.0.71/rpa_coop/img/sacg_branco.PNG
+-rw-rw-rw-   0        0        0      463 2023-06-01 13:04:34.000000 rpa_cooperativa-1.0.71/rpa_coop/img/sagc_verde.PNG
+-rw-rw-rw-   0        0        0      384 2023-02-28 19:53:19.000000 rpa_cooperativa-1.0.71/rpa_coop/img/siac_amarelo.PNG
+-rw-rw-rw-   0        0        0      370 2023-04-17 14:08:47.000000 rpa_cooperativa-1.0.71/rpa_coop/img/siac_branco.PNG
+-rw-rw-rw-   0        0        0      364 2023-04-17 14:10:18.000000 rpa_cooperativa-1.0.71/rpa_coop/img/siat_amarelo.PNG
+-rw-rw-rw-   0        0        0      349 2023-02-28 19:53:39.000000 rpa_cooperativa-1.0.71/rpa_coop/img/siat_branco.PNG
+-rw-rw-rw-   0        0        0     6079 2023-03-09 16:47:31.000000 rpa_cooperativa-1.0.71/rpa_coop/img/transacional_azul.PNG
+-rw-rw-rw-   0        0        0     6652 2023-03-09 16:46:38.000000 rpa_cooperativa-1.0.71/rpa_coop/img/transacional_verde.PNG
+-rw-rw-rw-   0        0        0   104249 2023-07-25 11:32:18.000000 rpa_cooperativa-1.0.71/rpa_coop/rpa_coop.py
+drwxrwxrwx   0        0        0        0 2023-07-25 11:34:03.383319 rpa_cooperativa-1.0.71/rpa_cooperativa.egg-info/
+-rw-rw-rw-   0        0        0     6969 2023-07-25 11:34:02.000000 rpa_cooperativa-1.0.71/rpa_cooperativa.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      631 2023-07-25 11:34:03.000000 rpa_cooperativa-1.0.71/rpa_cooperativa.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 11:34:02.000000 rpa_cooperativa-1.0.71/rpa_cooperativa.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-25 11:34:02.000000 rpa_cooperativa-1.0.71/rpa_cooperativa.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      581 2023-07-25 11:34:02.000000 rpa_cooperativa-1.0.71/rpa_cooperativa.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-25 11:34:02.000000 rpa_cooperativa-1.0.71/rpa_cooperativa.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-25 11:34:03.391317 rpa_cooperativa-1.0.71/setup.cfg
+-rw-rw-rw-   0        0        0     2350 2023-07-25 11:33:12.000000 rpa_cooperativa-1.0.71/setup.py
```

### Comparing `rpa_cooperativa-1.0.70/LICENSE` & `rpa_cooperativa-1.0.71/LICENSE`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.70/PKG-INFO` & `rpa_cooperativa-1.0.71/rpa_cooperativa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: rpa_cooperativa
-Version: 1.0.70
+Name: rpa-cooperativa
+Version: 1.0.71
 Summary: Classes referente automação com python para... api fluid, api whatsapp, api sms, sql, acc
 Home-page: https://github.com/edenilsonsantos/rpa_cooperativa
 Author: Edenilson Fernandes dos Santos
 Author-email: santoeen@gmail.com
 License: MIT License
 Project-URL: repository, https://github.com/edenilsonsantos/rpa_cooperativa
 Keywords: rpa cooperativa fluid api automação sql sqlalchemy
```

### Comparing `rpa_cooperativa-1.0.70/README.md` & `rpa_cooperativa-1.0.71/README.md`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.70/rpa_coop/__init__.py` & `rpa_cooperativa-1.0.71/rpa_coop/__init__.py`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.70/rpa_coop/img/relatorios_azul.PNG` & `rpa_cooperativa-1.0.71/rpa_coop/img/relatorios_azul.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.70/rpa_coop/img/relatorios_verde.PNG` & `rpa_cooperativa-1.0.71/rpa_coop/img/relatorios_verde.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.70/rpa_coop/img/transacional_azul.PNG` & `rpa_cooperativa-1.0.71/rpa_coop/img/transacional_azul.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.70/rpa_coop/img/transacional_verde.PNG` & `rpa_cooperativa-1.0.71/rpa_coop/img/transacional_verde.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.70/rpa_coop/rpa_coop.py` & `rpa_cooperativa-1.0.71/rpa_coop/rpa_coop.py`

 * *Files 1% similar despite different names*

```diff
@@ -2258,19 +2258,19 @@
     def __init__(self):
         pass
     
     def pegar_erro(self) -> str:
         '''usar dentro do except do try, captura informações do erro'''
         str_traceback = self.traceback.format_exc().replace('Traceback (most recent call last):', '').replace('^','').replace('~','').replace('File ','').replace('"','').replace("'","")
         try:
-            dica1 = str(self.re.findall('line\s\d+', str_traceback)[0]).replace('line', 'linha') + ' em ' + str(self.re.findall('c:.+py', str_traceback)[0]).split('\\')[-1]
+            dica1 = str(self.re.findall('line\s\d+', str_traceback)[0]).replace('line', 'linha') + ' em ' + str(self.re.findall('\D:.+py', str_traceback)[0]).split('\\')[-1]
         except:
             dica1 = ''
         try:
-            dica2 = str(self.re.findall('line\s\d+', str_traceback)[1]).replace('line', 'linha') + ' em ' + str(self.re.findall('c:.+py', str_traceback)[1]).split('\\')[-1]
+            dica2 = str(self.re.findall('line\s\d+', str_traceback)[1]).replace('line', 'linha') + ' em ' + str(self.re.findall('\D:.+py', str_traceback)[1]).split('\\')[-1]
         except:
             dica2 = ''
         try:
             list_traceback = str_traceback.splitlines()
             erro = str(list_traceback[-3]).strip() + ' : ' + str(list_traceback[-1]).strip()
             msg_log = f'{dica1} --> {str(list_traceback[2]).strip()} \n{dica2} --> {erro}'
         except:
```

### Comparing `rpa_cooperativa-1.0.70/rpa_cooperativa.egg-info/PKG-INFO` & `rpa_cooperativa-1.0.71/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: rpa-cooperativa
-Version: 1.0.70
+Name: rpa_cooperativa
+Version: 1.0.71
 Summary: Classes referente automação com python para... api fluid, api whatsapp, api sms, sql, acc
 Home-page: https://github.com/edenilsonsantos/rpa_cooperativa
 Author: Edenilson Fernandes dos Santos
 Author-email: santoeen@gmail.com
 License: MIT License
 Project-URL: repository, https://github.com/edenilsonsantos/rpa_cooperativa
 Keywords: rpa cooperativa fluid api automação sql sqlalchemy
```

### Comparing `rpa_cooperativa-1.0.70/rpa_cooperativa.egg-info/SOURCES.txt` & `rpa_cooperativa-1.0.71/rpa_cooperativa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.70/rpa_cooperativa.egg-info/requires.txt` & `rpa_cooperativa-1.0.71/rpa_cooperativa.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.70/setup.py` & `rpa_cooperativa-1.0.71/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r") as arq:
     readme = arq.read()
 
 
 setup(
     name="rpa_cooperativa",
-    version="1.0.70",
+    version="1.0.71",
     license='MIT License',
     author="Edenilson Fernandes dos Santos",
     author_email='santoeen@gmail.com',
     description="Classes referente automação com python para... api fluid, api whatsapp, api sms, sql, acc",
     long_description=readme,
     long_description_content_type="text/markdown",
     keywords='rpa cooperativa fluid api automação sql sqlalchemy',
```

