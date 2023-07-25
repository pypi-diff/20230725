# Comparing `tmp/sysnet-pyutils-1.0.2.tar.gz` & `tmp/sysnet-pyutils-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sysnet-pyutils-1.0.2.tar", last modified: Fri May 19 13:26:14 2023, max compression
+gzip compressed data, was "sysnet-pyutils-1.0.3.tar", last modified: Tue Jul 25 15:03:49 2023, max compression
```

## Comparing `sysnet-pyutils-1.0.2.tar` & `sysnet-pyutils-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 13:26:14.504728 sysnet-pyutils-1.0.2/
--rw-rw-rw-   0        0        0    35184 2023-03-27 14:59:40.000000 sysnet-pyutils-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     9052 2023-05-19 13:26:14.503729 sysnet-pyutils-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     8430 2023-05-19 13:25:22.000000 sysnet-pyutils-1.0.2/README.md
--rw-rw-rw-   0        0        0      862 2023-05-19 13:25:22.000000 sysnet-pyutils-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       47 2023-03-27 16:22:12.000000 sysnet-pyutils-1.0.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-19 13:26:14.504728 sysnet-pyutils-1.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-19 13:26:14.493862 sysnet-pyutils-1.0.2/sysnet_pyutils/
--rw-rw-rw-   0        0        0        0 2023-03-27 15:02:04.000000 sysnet-pyutils-1.0.2/sysnet_pyutils/__init__.py
--rw-rw-rw-   0        0        0     2622 2023-04-06 08:45:17.000000 sysnet-pyutils-1.0.2/sysnet_pyutils/barcode.py
--rw-rw-rw-   0        0        0     2763 2023-04-06 10:52:47.000000 sysnet-pyutils-1.0.2/sysnet_pyutils/ident.py
--rw-rw-rw-   0        0        0    14941 2023-05-19 13:25:22.000000 sysnet-pyutils-1.0.2/sysnet_pyutils/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-19 13:26:14.502729 sysnet-pyutils-1.0.2/sysnet_pyutils.egg-info/
--rw-rw-rw-   0        0        0     9052 2023-05-19 13:26:14.000000 sysnet-pyutils-1.0.2/sysnet_pyutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      339 2023-05-19 13:26:14.000000 sysnet-pyutils-1.0.2/sysnet_pyutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 13:26:14.000000 sysnet-pyutils-1.0.2/sysnet_pyutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-05-19 13:26:14.000000 sysnet-pyutils-1.0.2/sysnet_pyutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-19 13:26:14.000000 sysnet-pyutils-1.0.2/sysnet_pyutils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-25 15:03:49.258327 sysnet-pyutils-1.0.3/
+-rw-rw-rw-   0        0        0    35184 2023-03-27 14:59:40.000000 sysnet-pyutils-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0    10913 2023-07-25 15:03:49.257328 sysnet-pyutils-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0    10291 2023-07-25 15:03:27.000000 sysnet-pyutils-1.0.3/README.md
+-rw-rw-rw-   0        0        0      862 2023-07-25 15:03:27.000000 sysnet-pyutils-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       68 2023-07-25 15:00:57.000000 sysnet-pyutils-1.0.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-25 15:03:49.258327 sysnet-pyutils-1.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-25 15:03:49.245330 sysnet-pyutils-1.0.3/sysnet_pyutils/
+-rw-rw-rw-   0        0        0        0 2023-03-27 15:02:04.000000 sysnet-pyutils-1.0.3/sysnet_pyutils/__init__.py
+-rw-rw-rw-   0        0        0     2622 2023-04-06 08:45:17.000000 sysnet-pyutils-1.0.3/sysnet_pyutils/barcode.py
+-rw-rw-rw-   0        0        0     2763 2023-04-06 10:52:47.000000 sysnet-pyutils-1.0.3/sysnet_pyutils/ident.py
+-rw-rw-rw-   0        0        0    16002 2023-07-25 15:00:57.000000 sysnet-pyutils-1.0.3/sysnet_pyutils/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-25 15:03:49.255332 sysnet-pyutils-1.0.3/sysnet_pyutils.egg-info/
+-rw-rw-rw-   0        0        0    10913 2023-07-25 15:03:49.000000 sysnet-pyutils-1.0.3/sysnet_pyutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      339 2023-07-25 15:03:49.000000 sysnet-pyutils-1.0.3/sysnet_pyutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 15:03:49.000000 sysnet-pyutils-1.0.3/sysnet_pyutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2023-07-25 15:03:49.000000 sysnet-pyutils-1.0.3/sysnet_pyutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-25 15:03:49.000000 sysnet-pyutils-1.0.3/sysnet_pyutils.egg-info/top_level.txt
```

### Comparing `sysnet-pyutils-1.0.2/LICENSE` & `sysnet-pyutils-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sysnet-pyutils-1.0.2/PKG-INFO` & `sysnet-pyutils-1.0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: sysnet-pyutils
-Version: 1.0.2
-Summary: Python Utilities
-Author-email: Data Developer <info@sysnet.cz>
-Project-URL: Homepage, https://github.com/SYSNET-CZ/pyutils
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Programming Language :: Python :: 3
-Classifier: Intended Audience :: Developers
-Classifier: License :: Free For Home Use
-Classifier: Natural Language :: Czech
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # sysnet-pyutils
 
 SYSNET Python Utilities
 
 Knihovna obsahuje záklaní, v aplikacích hojně používané, utility.
 
 ## sysnet-pyutils.utils
@@ -217,14 +200,47 @@
 * param uuid_type: Lze použít pouze typ 1 nebo 4
 * return: uuid
 --------------------------------------------------------------------------------------------------------------------------------
 #### who_am_i():
 Vrátí název aktuální funkce
 * return: název funkce, odkud je voláno  
 * například:   `__name__ = who_am_i()`  
+--------------------------------------------------------------------------------------------------------------------------------
+### Vereze 1.0.3
+#### to_camel(s):
+Převede text z hadí_notace do VelbloudíNotace
+* param s: text v hadí notaci
+* return: text ve velbloudí notaci  
+--------------------------------------------------------------------------------------------------------------------------------
+#### to_snake(s):
+Převede text z VelbloudíNotace do hadí_notace 
+* param s: text ve velbloudí notaci
+* return: text v hadí notaci  
+--------------------------------------------------------------------------------------------------------------------------------
+#### to_camel_dict(d):
+Rekurzivně převede klíče ve slovníku z hadí_notace do VelbloudíNotace
+* param d: dictionary s klíči v hadí notaci
+* return: dictionary s klíči ve velbloudí notaci  
+--------------------------------------------------------------------------------------------------------------------------------
+#### to_snake_dict(d):
+Rekurzivně převede klíče ve slovníku z VelbloudíNotace do hadí_notace 
+* param d: dictionary s klíči ve velbloudí notaci
+* return: dictionary s klíči v hadí notaci  
+--------------------------------------------------------------------------------------------------------------------------------
+#### xml_to_dict(xml_text):
+Parsuje XML string do XML dictionary 
+podle pravidel viz https://github.com/martinblech/xmltodict
+* param xml_text:    XML text
+* return:    XML dictionary
+--------------------------------------------------------------------------------------------------------------------------------
+#### dict_to_xml(xml_dict):
+Parsuje XML dict do XML textu podle 
+pravidel viz https://github.com/martinblech/xmltodict
+* param xml_dict:    XML dictionary
+* return:    XML text
 
 
 ## Systémové proměnné
 
 * **TZ**: Časová zóna. Implicitně 'Europe/Prague'
 * **DEBUG**: Debug mode. Implictně `True`
 * **LOG_FORMAT**: Formát logování. Implicitně `'%(asctime)s - %(levelname)s in %(module)s: %(message)s'`
```

### Comparing `sysnet-pyutils-1.0.2/README.md` & `sysnet-pyutils-1.0.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: sysnet-pyutils
+Version: 1.0.3
+Summary: Python Utilities
+Author-email: Data Developer <info@sysnet.cz>
+Project-URL: Homepage, https://github.com/SYSNET-CZ/pyutils
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Programming Language :: Python :: 3
+Classifier: Intended Audience :: Developers
+Classifier: License :: Free For Home Use
+Classifier: Natural Language :: Czech
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Software Development :: Libraries
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # sysnet-pyutils
 
 SYSNET Python Utilities
 
 Knihovna obsahuje záklaní, v aplikacích hojně používané, utility.
 
 ## sysnet-pyutils.utils
@@ -200,14 +217,47 @@
 * param uuid_type: Lze použít pouze typ 1 nebo 4
 * return: uuid
 --------------------------------------------------------------------------------------------------------------------------------
 #### who_am_i():
 Vrátí název aktuální funkce
 * return: název funkce, odkud je voláno  
 * například:   `__name__ = who_am_i()`  
+--------------------------------------------------------------------------------------------------------------------------------
+### Vereze 1.0.3
+#### to_camel(s):
+Převede text z hadí_notace do VelbloudíNotace
+* param s: text v hadí notaci
+* return: text ve velbloudí notaci  
+--------------------------------------------------------------------------------------------------------------------------------
+#### to_snake(s):
+Převede text z VelbloudíNotace do hadí_notace 
+* param s: text ve velbloudí notaci
+* return: text v hadí notaci  
+--------------------------------------------------------------------------------------------------------------------------------
+#### to_camel_dict(d):
+Rekurzivně převede klíče ve slovníku z hadí_notace do VelbloudíNotace
+* param d: dictionary s klíči v hadí notaci
+* return: dictionary s klíči ve velbloudí notaci  
+--------------------------------------------------------------------------------------------------------------------------------
+#### to_snake_dict(d):
+Rekurzivně převede klíče ve slovníku z VelbloudíNotace do hadí_notace 
+* param d: dictionary s klíči ve velbloudí notaci
+* return: dictionary s klíči v hadí notaci  
+--------------------------------------------------------------------------------------------------------------------------------
+#### xml_to_dict(xml_text):
+Parsuje XML string do XML dictionary 
+podle pravidel viz https://github.com/martinblech/xmltodict
+* param xml_text:    XML text
+* return:    XML dictionary
+--------------------------------------------------------------------------------------------------------------------------------
+#### dict_to_xml(xml_dict):
+Parsuje XML dict do XML textu podle 
+pravidel viz https://github.com/martinblech/xmltodict
+* param xml_dict:    XML dictionary
+* return:    XML text
 
 
 ## Systémové proměnné
 
 * **TZ**: Časová zóna. Implicitně 'Europe/Prague'
 * **DEBUG**: Debug mode. Implictně `True`
 * **LOG_FORMAT**: Formát logování. Implicitně `'%(asctime)s - %(levelname)s in %(module)s: %(message)s'`
```

### Comparing `sysnet-pyutils-1.0.2/pyproject.toml` & `sysnet-pyutils-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sysnet-pyutils"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
   { name="Data Developer", email="info@sysnet.cz" },
 ]
 description = "Python Utilities"
 readme = "README.md"
 license = { file="LICENSE.md" }
 requires-python = ">=3.9"
```

### Comparing `sysnet-pyutils-1.0.2/sysnet_pyutils/barcode.py` & `sysnet-pyutils-1.0.3/sysnet_pyutils/barcode.py`

 * *Files identical despite different names*

### Comparing `sysnet-pyutils-1.0.2/sysnet_pyutils/ident.py` & `sysnet-pyutils-1.0.3/sysnet_pyutils/ident.py`

 * *Files identical despite different names*

### Comparing `sysnet-pyutils-1.0.2/sysnet_pyutils/utils.py` & `sysnet-pyutils-1.0.3/sysnet_pyutils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import uuid
 import re
 from datetime import datetime, timedelta
 from urllib.parse import quote
 
 import dateutil.parser
 import pytz
+import xmltodict
 import yaml
 
 from sysnet_pyutils.ident import generate_pid, check_pid, correct_pid, generate_id12
 
 TZ = os.getenv('TZ', 'Europe/Prague')
 DEBUG = os.getenv("DEBUG", 'True').lower() in ('true', '1', 't')
 LOG_FORMAT = os.getenv('LOG_FORMAT', '%(asctime)s - %(levelname)s in %(module)s: %(message)s')
@@ -603,7 +604,48 @@
         Nastaví externí logger (například z Djanga nebo Flask)
 
         :param ext_logger: Esterní logger
         :return:
         """
         if ext_logger is not None:
             self.logger = ext_logger
+
+
+def to_camel(s):
+    temp = re.split('_+', s)
+    out = temp[0] + ''.join(map(lambda x: x.title(), temp[1:]))
+    return out
+
+
+def to_snake(s):
+    return re.sub('([A-Z]\w+$)', '_\\1', s).lower()
+
+
+def to_snake_dict(d):
+    if isinstance(d, list):
+        return [to_snake_dict(i) if isinstance(i, (dict, list)) else i for i in d]
+    return {to_snake(a): to_snake_dict(b) if isinstance(b, (dict, list)) else b for a, b in d.items()}
+
+
+def to_camel_dict(d):
+    if isinstance(d, list):
+        return [to_camel_dict(i) if isinstance(i, (dict, list)) else i for i in d]
+    return {to_camel(a): to_camel_dict(b) if isinstance(b, (dict, list)) else b for a, b in d.items()}
+
+
+def xml_to_dict(xml_text):
+    """
+    Parsuje XML string do XML dictionary
+    :param xml_text:    XML text
+    :return:    XML dictionary
+    """
+    return xmltodict.parse(xml_text)
+
+
+def dict_to_xml(xml_dict):
+    """
+    Parsuje XML dict do XML textu
+
+    :param xml_dict:    XML dictionary
+    :return:    XML text
+    """
+    return xmltodict.unparse(xml_dict)
```

### Comparing `sysnet-pyutils-1.0.2/sysnet_pyutils.egg-info/PKG-INFO` & `sysnet-pyutils-1.0.3/sysnet_pyutils.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sysnet-pyutils
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python Utilities
 Author-email: Data Developer <info@sysnet.cz>
 Project-URL: Homepage, https://github.com/SYSNET-CZ/pyutils
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: License :: Free For Home Use
@@ -217,14 +217,47 @@
 * param uuid_type: Lze použít pouze typ 1 nebo 4
 * return: uuid
 --------------------------------------------------------------------------------------------------------------------------------
 #### who_am_i():
 Vrátí název aktuální funkce
 * return: název funkce, odkud je voláno  
 * například:   `__name__ = who_am_i()`  
+--------------------------------------------------------------------------------------------------------------------------------
+### Vereze 1.0.3
+#### to_camel(s):
+Převede text z hadí_notace do VelbloudíNotace
+* param s: text v hadí notaci
+* return: text ve velbloudí notaci  
+--------------------------------------------------------------------------------------------------------------------------------
+#### to_snake(s):
+Převede text z VelbloudíNotace do hadí_notace 
+* param s: text ve velbloudí notaci
+* return: text v hadí notaci  
+--------------------------------------------------------------------------------------------------------------------------------
+#### to_camel_dict(d):
+Rekurzivně převede klíče ve slovníku z hadí_notace do VelbloudíNotace
+* param d: dictionary s klíči v hadí notaci
+* return: dictionary s klíči ve velbloudí notaci  
+--------------------------------------------------------------------------------------------------------------------------------
+#### to_snake_dict(d):
+Rekurzivně převede klíče ve slovníku z VelbloudíNotace do hadí_notace 
+* param d: dictionary s klíči ve velbloudí notaci
+* return: dictionary s klíči v hadí notaci  
+--------------------------------------------------------------------------------------------------------------------------------
+#### xml_to_dict(xml_text):
+Parsuje XML string do XML dictionary 
+podle pravidel viz https://github.com/martinblech/xmltodict
+* param xml_text:    XML text
+* return:    XML dictionary
+--------------------------------------------------------------------------------------------------------------------------------
+#### dict_to_xml(xml_dict):
+Parsuje XML dict do XML textu podle 
+pravidel viz https://github.com/martinblech/xmltodict
+* param xml_dict:    XML dictionary
+* return:    XML text
 
 
 ## Systémové proměnné
 
 * **TZ**: Časová zóna. Implicitně 'Europe/Prague'
 * **DEBUG**: Debug mode. Implictně `True`
 * **LOG_FORMAT**: Formát logování. Implicitně `'%(asctime)s - %(levelname)s in %(module)s: %(message)s'`
```

