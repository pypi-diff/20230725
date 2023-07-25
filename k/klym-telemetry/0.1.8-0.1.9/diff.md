# Comparing `tmp/klym-telemetry-0.1.8.tar.gz` & `tmp/klym-telemetry-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klym-telemetry-0.1.8.tar", last modified: Mon May  8 17:26:51 2023, max compression
+gzip compressed data, was "klym-telemetry-0.1.9.tar", last modified: Mon May  8 17:39:59 2023, max compression
```

## Comparing `klym-telemetry-0.1.8.tar` & `klym-telemetry-0.1.9.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 17:26:51.531158 klym-telemetry-0.1.8/
--rw-rw-rw-   0        0        0     4076 2023-05-08 17:26:51.530103 klym-telemetry-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     3148 2023-05-01 21:12:52.000000 klym-telemetry-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-05-08 17:26:51.494086 klym-telemetry-0.1.8/klym_telemetry/
--rw-rw-rw-   0        0        0        0 2023-04-22 00:00:44.000000 klym-telemetry-0.1.8/klym_telemetry/__init__.py
--rw-rw-rw-   0        0        0     2612 2023-04-23 22:09:56.000000 klym-telemetry-0.1.8/klym_telemetry/helpers.py
-drwxrwxrwx   0        0        0        0 2023-05-08 17:26:51.527063 klym-telemetry-0.1.8/klym_telemetry/instrumenters/
--rw-rw-rw-   0        0        0     1175 2023-05-08 16:52:38.000000 klym-telemetry-0.1.8/klym_telemetry/instrumenters/__init__.py
--rw-rw-rw-   0        0        0      878 2023-05-08 16:59:10.000000 klym-telemetry-0.1.8/klym_telemetry/instrumenters/airflow.py
--rw-rw-rw-   0        0        0     2131 2023-04-25 19:42:07.000000 klym-telemetry-0.1.8/klym_telemetry/instrumenters/base.py
--rw-rw-rw-   0        0        0      507 2023-05-03 15:19:21.000000 klym-telemetry-0.1.8/klym_telemetry/instrumenters/celery.py
--rw-rw-rw-   0        0        0      507 2023-05-03 15:18:48.000000 klym-telemetry-0.1.8/klym_telemetry/instrumenters/django.py
--rw-rw-rw-   0        0        0      874 2023-05-08 13:47:20.000000 klym-telemetry-0.1.8/klym_telemetry/instrumenters/fastapi.py
--rw-rw-rw-   0        0        0      636 2023-05-08 16:52:38.000000 klym-telemetry-0.1.8/klym_telemetry/instrumenters/module_import.py
--rw-rw-rw-   0        0        0      515 2023-05-01 21:09:25.000000 klym-telemetry-0.1.8/klym_telemetry/instrumenters/psycopg2.py
--rw-rw-rw-   0        0        0      515 2023-05-03 15:19:21.000000 klym-telemetry-0.1.8/klym_telemetry/instrumenters/requests.py
--rw-rw-rw-   0        0        0     5693 2023-04-23 22:09:56.000000 klym-telemetry-0.1.8/klym_telemetry/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-08 17:26:51.503060 klym-telemetry-0.1.8/klym_telemetry.egg-info/
--rw-rw-rw-   0        0        0     4076 2023-05-08 17:26:51.000000 klym-telemetry-0.1.8/klym_telemetry.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      648 2023-05-08 17:26:51.000000 klym-telemetry-0.1.8/klym_telemetry.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 17:26:51.000000 klym-telemetry-0.1.8/klym_telemetry.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      406 2023-05-08 17:26:51.000000 klym-telemetry-0.1.8/klym_telemetry.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-08 17:26:51.000000 klym-telemetry-0.1.8/klym_telemetry.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-08 17:26:51.531158 klym-telemetry-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1795 2023-05-08 17:20:26.000000 klym-telemetry-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 17:39:59.355332 klym-telemetry-0.1.9/
+-rw-rw-rw-   0        0        0     4076 2023-05-08 17:39:59.354342 klym-telemetry-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3148 2023-05-01 21:12:52.000000 klym-telemetry-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-05-08 17:39:59.326260 klym-telemetry-0.1.9/klym_telemetry/
+-rw-rw-rw-   0        0        0        0 2023-04-22 00:00:44.000000 klym-telemetry-0.1.9/klym_telemetry/__init__.py
+-rw-rw-rw-   0        0        0     2612 2023-04-23 22:09:56.000000 klym-telemetry-0.1.9/klym_telemetry/helpers.py
+drwxrwxrwx   0        0        0        0 2023-05-08 17:39:59.352339 klym-telemetry-0.1.9/klym_telemetry/instrumenters/
+-rw-rw-rw-   0        0        0     1267 2023-05-08 17:39:18.000000 klym-telemetry-0.1.9/klym_telemetry/instrumenters/__init__.py
+-rw-rw-rw-   0        0        0      536 2023-05-08 17:39:18.000000 klym-telemetry-0.1.9/klym_telemetry/instrumenters/aiohttp.py
+-rw-rw-rw-   0        0        0      878 2023-05-08 16:59:10.000000 klym-telemetry-0.1.9/klym_telemetry/instrumenters/airflow.py
+-rw-rw-rw-   0        0        0     2131 2023-04-25 19:42:07.000000 klym-telemetry-0.1.9/klym_telemetry/instrumenters/base.py
+-rw-rw-rw-   0        0        0      507 2023-05-03 15:19:21.000000 klym-telemetry-0.1.9/klym_telemetry/instrumenters/celery.py
+-rw-rw-rw-   0        0        0      507 2023-05-03 15:18:48.000000 klym-telemetry-0.1.9/klym_telemetry/instrumenters/django.py
+-rw-rw-rw-   0        0        0      874 2023-05-08 13:47:20.000000 klym-telemetry-0.1.9/klym_telemetry/instrumenters/fastapi.py
+-rw-rw-rw-   0        0        0      636 2023-05-08 16:52:38.000000 klym-telemetry-0.1.9/klym_telemetry/instrumenters/module_import.py
+-rw-rw-rw-   0        0        0      515 2023-05-01 21:09:25.000000 klym-telemetry-0.1.9/klym_telemetry/instrumenters/psycopg2.py
+-rw-rw-rw-   0        0        0      515 2023-05-03 15:19:21.000000 klym-telemetry-0.1.9/klym_telemetry/instrumenters/requests.py
+-rw-rw-rw-   0        0        0     5693 2023-04-23 22:09:56.000000 klym-telemetry-0.1.9/klym_telemetry/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-08 17:39:59.335291 klym-telemetry-0.1.9/klym_telemetry.egg-info/
+-rw-rw-rw-   0        0        0     4076 2023-05-08 17:39:59.000000 klym-telemetry-0.1.9/klym_telemetry.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      688 2023-05-08 17:39:59.000000 klym-telemetry-0.1.9/klym_telemetry.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 17:39:59.000000 klym-telemetry-0.1.9/klym_telemetry.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      459 2023-05-08 17:39:59.000000 klym-telemetry-0.1.9/klym_telemetry.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-08 17:39:59.000000 klym-telemetry-0.1.9/klym_telemetry.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-08 17:39:59.355332 klym-telemetry-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1860 2023-05-08 17:39:18.000000 klym-telemetry-0.1.9/setup.py
```

### Comparing `klym-telemetry-0.1.8/PKG-INFO` & `klym-telemetry-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: klym-telemetry
-Version: 0.1.8
+Version: 0.1.9
 Summary: Scaffold library
 Home-page: https://dummy.readthedocs.io/
 Author: Klym Telemetry
 Author-email: example@email.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `klym-telemetry-0.1.8/README.md` & `klym-telemetry-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `klym-telemetry-0.1.8/klym_telemetry/helpers.py` & `klym-telemetry-0.1.9/klym_telemetry/helpers.py`

 * *Files identical despite different names*

### Comparing `klym-telemetry-0.1.8/klym_telemetry/instrumenters/__init__.py` & `klym-telemetry-0.1.9/klym_telemetry/instrumenters/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     INSTRUMENTERS = {
         "fastapi": ("klym_telemetry.instrumenters.fastapi", "_FastAPIInstrumentor"),
         "airflow": ("klym_telemetry.instrumenters.airflow", "_AirflowInstrumentor"),
         "django": ("klym_telemetry.instrumenters.django", "_DjangoInstrumentor"),
         "celery": ("klym_telemetry.instrumenters.celery", "_CeleryInstrumentor"),
         "psycopg2": ("klym_telemetry.instrumenters.psycopg2", "_Psycopg2Instrumentor"),
         "requests": ("klym_telemetry.instrumenters.requests", "_RequestsInstrumentor"),
+        "aiohttp": ("klym_telemetry.instrumenters.aiohttp", "_AioHttpClientInstrumentor"),
     }
 
 def instrument_app(app_type: str, **kwargs):
     try:
         package = SupportedInstrumenters.INSTRUMENTERS.value.get(app_type)[0]
         classname = SupportedInstrumenters.INSTRUMENTERS.value.get(app_type)[1]
         return importer.import_module(package, classname)(**kwargs).instrument()
```

### Comparing `klym-telemetry-0.1.8/klym_telemetry/instrumenters/airflow.py` & `klym-telemetry-0.1.9/klym_telemetry/instrumenters/airflow.py`

 * *Files identical despite different names*

### Comparing `klym-telemetry-0.1.8/klym_telemetry/instrumenters/base.py` & `klym-telemetry-0.1.9/klym_telemetry/instrumenters/base.py`

 * *Files identical despite different names*

### Comparing `klym-telemetry-0.1.8/klym_telemetry/instrumenters/fastapi.py` & `klym-telemetry-0.1.9/klym_telemetry/instrumenters/fastapi.py`

 * *Files identical despite different names*

### Comparing `klym-telemetry-0.1.8/klym_telemetry/instrumenters/module_import.py` & `klym-telemetry-0.1.9/klym_telemetry/instrumenters/module_import.py`

 * *Files identical despite different names*

### Comparing `klym-telemetry-0.1.8/klym_telemetry/instrumenters/psycopg2.py` & `klym-telemetry-0.1.9/klym_telemetry/instrumenters/psycopg2.py`

 * *Files identical despite different names*

### Comparing `klym-telemetry-0.1.8/klym_telemetry/instrumenters/requests.py` & `klym-telemetry-0.1.9/klym_telemetry/instrumenters/requests.py`

 * *Files identical despite different names*

### Comparing `klym-telemetry-0.1.8/klym_telemetry/utils.py` & `klym-telemetry-0.1.9/klym_telemetry/utils.py`

 * *Files identical despite different names*

### Comparing `klym-telemetry-0.1.8/klym_telemetry.egg-info/PKG-INFO` & `klym-telemetry-0.1.9/klym_telemetry.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: klym-telemetry
-Version: 0.1.8
+Version: 0.1.9
 Summary: Scaffold library
 Home-page: https://dummy.readthedocs.io/
 Author: Klym Telemetry
 Author-email: example@email.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `klym-telemetry-0.1.8/klym_telemetry.egg-info/SOURCES.txt` & `klym-telemetry-0.1.9/klym_telemetry.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 klym_telemetry/utils.py
 klym_telemetry.egg-info/PKG-INFO
 klym_telemetry.egg-info/SOURCES.txt
 klym_telemetry.egg-info/dependency_links.txt
 klym_telemetry.egg-info/requires.txt
 klym_telemetry.egg-info/top_level.txt
 klym_telemetry/instrumenters/__init__.py
+klym_telemetry/instrumenters/aiohttp.py
 klym_telemetry/instrumenters/airflow.py
 klym_telemetry/instrumenters/base.py
 klym_telemetry/instrumenters/celery.py
 klym_telemetry/instrumenters/django.py
 klym_telemetry/instrumenters/fastapi.py
 klym_telemetry/instrumenters/module_import.py
 klym_telemetry/instrumenters/psycopg2.py
```

### Comparing `klym-telemetry-0.1.8/setup.py` & `klym-telemetry-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 HERE = path.abspath(path.dirname(__file__))
 
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="klym-telemetry",
-    version="0.1.8",
+    version="0.1.9",
     description="Scaffold library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://dummy.readthedocs.io/",
     author="Klym Telemetry",
     author_email="example@email.com",
     license="MIT",
@@ -36,13 +36,14 @@
     install_requires=[
         'opentelemetry-instrumentation-django~=0.38b0',
         'opentelemetry-instrumentation-fastapi~=0.38b0',
         'opentelemetry-instrumentation-requests~=0.38b0',
         'opentelemetry-instrumentation-sqlalchemy~=0.38b0',
         'opentelemetry-instrumentation-psycopg2~=0.38b0',
         'opentelemetry-instrumentation-celery~=0.38b0',
+        'opentelemetry-instrumentation-aiohttp-client~=0.38b0',
         'opentelemetry-exporter-otlp-proto-grpc~=1.17.0',
         'opentelemetry-propagator-aws-xray~=1.0.1',
         'opentelemetry-sdk-extension-aws~=2.0.1'
     ],
     python_requires='>=3.6',
 )
```

