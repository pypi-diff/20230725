# Comparing `tmp/rapo-0.4.3.tar.gz` & `tmp/rapo-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapo-0.4.3.tar", last modified: Sat Jul  8 17:51:31 2023, max compression
+gzip compressed data, was "rapo-0.4.4.tar", last modified: Tue Jul 25 21:44:08 2023, max compression
```

## Comparing `rapo-0.4.3.tar` & `rapo-0.4.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 timur      (501) staff       (20)        0 2023-07-08 17:51:31.145784 rapo-0.4.3/
--rw-r--r--   0 timur      (501) staff       (20)     1074 2023-04-11 10:47:36.000000 rapo-0.4.3/LICENSE
--rw-r--r--   0 timur      (501) staff       (20)     3704 2023-07-08 17:51:31.145570 rapo-0.4.3/PKG-INFO
--rw-r--r--   0 timur      (501) staff       (20)     3199 2023-07-08 17:44:30.000000 rapo-0.4.3/README.md
-drwxr-xr-x   0 timur      (501) staff       (20)        0 2023-07-08 17:51:31.142525 rapo-0.4.3/rapo/
--rw-r--r--   0 timur      (501) staff       (20)      469 2023-07-08 17:44:30.000000 rapo-0.4.3/rapo/__init__.py
--rw-r--r--   0 timur      (501) staff       (20)     3028 2023-07-08 17:44:30.000000 rapo-0.4.3/rapo/config.py
--rw-r--r--   0 timur      (501) staff       (20)     8367 2023-07-08 17:44:30.000000 rapo-0.4.3/rapo/database.py
--rw-r--r--   0 timur      (501) staff       (20)      290 2023-07-08 17:44:30.000000 rapo-0.4.3/rapo/logger.py
-drwxr-xr-x   0 timur      (501) staff       (20)        0 2023-07-08 17:51:31.144007 rapo-0.4.3/rapo/main/
--rw-r--r--   0 timur      (501) staff       (20)      155 2023-04-11 10:47:36.000000 rapo-0.4.3/rapo/main/__init__.py
--rw-r--r--   0 timur      (501) staff       (20)      166 2023-07-08 17:44:30.000000 rapo-0.4.3/rapo/main/case.py
--rw-r--r--   0 timur      (501) staff       (20)    77165 2023-07-08 17:44:30.000000 rapo-0.4.3/rapo/main/control.py
--rw-r--r--   0 timur      (501) staff       (20)      799 2023-07-08 17:44:30.000000 rapo-0.4.3/rapo/main/fields.py
--rw-r--r--   0 timur      (501) staff       (20)    14060 2023-07-08 17:44:30.000000 rapo-0.4.3/rapo/main/scheduler.py
--rw-r--r--   0 timur      (501) staff       (20)     3523 2023-07-08 17:44:30.000000 rapo-0.4.3/rapo/reader.py
--rw-r--r--   0 timur      (501) staff       (20)     2848 2023-07-08 17:44:30.000000 rapo-0.4.3/rapo/utils.py
-drwxr-xr-x   0 timur      (501) staff       (20)        0 2023-07-08 17:51:31.144150 rapo-0.4.3/rapo/web/
--rw-r--r--   0 timur      (501) staff       (20)     4525 2023-07-08 17:44:30.000000 rapo-0.4.3/rapo/web/__init__.py
-drwxr-xr-x   0 timur      (501) staff       (20)        0 2023-07-08 17:51:31.144634 rapo-0.4.3/rapo/web/api/
--rw-r--r--   0 timur      (501) staff       (20)       48 2023-04-11 10:47:36.000000 rapo-0.4.3/rapo/web/api/__init__.py
--rw-r--r--   0 timur      (501) staff       (20)     3025 2023-07-08 17:44:30.000000 rapo-0.4.3/rapo/web/api/app.py
--rw-r--r--   0 timur      (501) staff       (20)      249 2023-04-11 10:47:36.000000 rapo-0.4.3/rapo/web/api/auth.py
--rw-r--r--   0 timur      (501) staff       (20)      170 2023-04-11 10:47:36.000000 rapo-0.4.3/rapo/web/api/response.py
-drwxr-xr-x   0 timur      (501) staff       (20)        0 2023-07-08 17:51:31.144773 rapo-0.4.3/rapo/web/api/templates/
--rw-r--r--   0 timur      (501) staff       (20)      279 2023-04-11 10:47:36.000000 rapo-0.4.3/rapo/web/api/templates/help.html
-drwxr-xr-x   0 timur      (501) staff       (20)        0 2023-07-08 17:51:31.143241 rapo-0.4.3/rapo.egg-info/
--rw-r--r--   0 timur      (501) staff       (20)     3704 2023-07-08 17:51:31.000000 rapo-0.4.3/rapo.egg-info/PKG-INFO
--rw-r--r--   0 timur      (501) staff       (20)      507 2023-07-08 17:51:31.000000 rapo-0.4.3/rapo.egg-info/SOURCES.txt
--rw-r--r--   0 timur      (501) staff       (20)        1 2023-07-08 17:51:31.000000 rapo-0.4.3/rapo.egg-info/dependency_links.txt
--rw-r--r--   0 timur      (501) staff       (20)      134 2023-07-08 17:51:31.000000 rapo-0.4.3/rapo.egg-info/requires.txt
--rw-r--r--   0 timur      (501) staff       (20)        5 2023-07-08 17:51:31.000000 rapo-0.4.3/rapo.egg-info/top_level.txt
--rw-r--r--   0 timur      (501) staff       (20)       38 2023-07-08 17:51:31.145837 rapo-0.4.3/setup.cfg
--rw-r--r--   0 timur      (501) staff       (20)     1363 2023-07-08 17:44:30.000000 rapo-0.4.3/setup.py
+drwxr-xr-x   0 timur      (501) staff       (20)        0 2023-07-25 21:44:08.789082 rapo-0.4.4/
+-rw-r--r--   0 timur      (501) staff       (20)     1074 2023-04-11 10:47:36.000000 rapo-0.4.4/LICENSE
+-rw-r--r--   0 timur      (501) staff       (20)     3704 2023-07-25 21:44:08.788933 rapo-0.4.4/PKG-INFO
+-rw-r--r--   0 timur      (501) staff       (20)     3199 2023-07-10 14:37:03.000000 rapo-0.4.4/README.md
+drwxr-xr-x   0 timur      (501) staff       (20)        0 2023-07-25 21:44:08.786003 rapo-0.4.4/rapo/
+-rw-r--r--   0 timur      (501) staff       (20)      469 2023-07-25 21:41:20.000000 rapo-0.4.4/rapo/__init__.py
+-rw-r--r--   0 timur      (501) staff       (20)     3028 2023-07-08 17:44:30.000000 rapo-0.4.4/rapo/config.py
+-rw-r--r--   0 timur      (501) staff       (20)     8367 2023-07-08 17:44:30.000000 rapo-0.4.4/rapo/database.py
+-rw-r--r--   0 timur      (501) staff       (20)      290 2023-07-08 17:44:30.000000 rapo-0.4.4/rapo/logger.py
+drwxr-xr-x   0 timur      (501) staff       (20)        0 2023-07-25 21:44:08.787665 rapo-0.4.4/rapo/main/
+-rw-r--r--   0 timur      (501) staff       (20)      155 2023-04-11 10:47:36.000000 rapo-0.4.4/rapo/main/__init__.py
+-rw-r--r--   0 timur      (501) staff       (20)      166 2023-07-08 17:44:30.000000 rapo-0.4.4/rapo/main/case.py
+-rw-r--r--   0 timur      (501) staff       (20)    77187 2023-07-25 21:31:39.000000 rapo-0.4.4/rapo/main/control.py
+-rw-r--r--   0 timur      (501) staff       (20)      799 2023-07-08 17:44:30.000000 rapo-0.4.4/rapo/main/fields.py
+-rw-r--r--   0 timur      (501) staff       (20)    14060 2023-07-08 17:44:30.000000 rapo-0.4.4/rapo/main/scheduler.py
+-rw-r--r--   0 timur      (501) staff       (20)     3523 2023-07-08 17:44:30.000000 rapo-0.4.4/rapo/reader.py
+-rw-r--r--   0 timur      (501) staff       (20)     2848 2023-07-08 17:44:30.000000 rapo-0.4.4/rapo/utils.py
+drwxr-xr-x   0 timur      (501) staff       (20)        0 2023-07-25 21:44:08.787830 rapo-0.4.4/rapo/web/
+-rw-r--r--   0 timur      (501) staff       (20)     4627 2023-07-25 21:01:43.000000 rapo-0.4.4/rapo/web/__init__.py
+drwxr-xr-x   0 timur      (501) staff       (20)        0 2023-07-25 21:44:08.788398 rapo-0.4.4/rapo/web/api/
+-rw-r--r--   0 timur      (501) staff       (20)       48 2023-04-11 10:47:36.000000 rapo-0.4.4/rapo/web/api/__init__.py
+-rw-r--r--   0 timur      (501) staff       (20)     3025 2023-07-08 17:44:30.000000 rapo-0.4.4/rapo/web/api/app.py
+-rw-r--r--   0 timur      (501) staff       (20)      249 2023-04-11 10:47:36.000000 rapo-0.4.4/rapo/web/api/auth.py
+-rw-r--r--   0 timur      (501) staff       (20)      170 2023-04-11 10:47:36.000000 rapo-0.4.4/rapo/web/api/response.py
+drwxr-xr-x   0 timur      (501) staff       (20)        0 2023-07-25 21:44:08.788538 rapo-0.4.4/rapo/web/api/templates/
+-rw-r--r--   0 timur      (501) staff       (20)      279 2023-04-11 10:47:36.000000 rapo-0.4.4/rapo/web/api/templates/help.html
+drwxr-xr-x   0 timur      (501) staff       (20)        0 2023-07-25 21:44:08.786909 rapo-0.4.4/rapo.egg-info/
+-rw-r--r--   0 timur      (501) staff       (20)     3704 2023-07-25 21:44:08.000000 rapo-0.4.4/rapo.egg-info/PKG-INFO
+-rw-r--r--   0 timur      (501) staff       (20)      507 2023-07-25 21:44:08.000000 rapo-0.4.4/rapo.egg-info/SOURCES.txt
+-rw-r--r--   0 timur      (501) staff       (20)        1 2023-07-25 21:44:08.000000 rapo-0.4.4/rapo.egg-info/dependency_links.txt
+-rw-r--r--   0 timur      (501) staff       (20)      134 2023-07-25 21:44:08.000000 rapo-0.4.4/rapo.egg-info/requires.txt
+-rw-r--r--   0 timur      (501) staff       (20)        5 2023-07-25 21:44:08.000000 rapo-0.4.4/rapo.egg-info/top_level.txt
+-rw-r--r--   0 timur      (501) staff       (20)       38 2023-07-25 21:44:08.789130 rapo-0.4.4/setup.cfg
+-rw-r--r--   0 timur      (501) staff       (20)     1363 2023-07-08 17:44:30.000000 rapo-0.4.4/setup.py
```

### Comparing `rapo-0.4.3/LICENSE` & `rapo-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rapo-0.4.3/PKG-INFO` & `rapo-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapo
-Version: 0.4.3
+Version: 0.4.4
 Summary: Python Revenue Assurance Process Optimizer.
 Home-page: https://github.com/t3eHawk/rapo
 Author: Timur Faradzhov
 Author-email: timurfaradzhov@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `rapo-0.4.3/README.md` & `rapo-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `rapo-0.4.3/rapo/config.py` & `rapo-0.4.4/rapo/config.py`

 * *Files identical despite different names*

### Comparing `rapo-0.4.3/rapo/database.py` & `rapo-0.4.4/rapo/database.py`

 * *Files identical despite different names*

### Comparing `rapo-0.4.3/rapo/main/control.py` & `rapo-0.4.4/rapo/main/control.py`

 * *Files 0% similar despite different names*

```diff
@@ -1438,14 +1438,15 @@
             clause = sa.or_(result_type.in_(target_types),
                             result_type.is_(None))
             statement = db.compile(clause)
             expression = statement.string
             return expression
         else:
             logger.debug(f'{self.c} Error SQL not found')
+            return ''
 
     def parse_reconciliation_rule_config(self):
         """Get control rule configuration.
 
         Returns
         -------
         config : list
```

### Comparing `rapo-0.4.3/rapo/main/fields.py` & `rapo-0.4.4/rapo/main/fields.py`

 * *Files identical despite different names*

### Comparing `rapo-0.4.3/rapo/main/scheduler.py` & `rapo-0.4.4/rapo/main/scheduler.py`

 * *Files identical despite different names*

### Comparing `rapo-0.4.3/rapo/reader.py` & `rapo-0.4.4/rapo/reader.py`

 * *Files identical despite different names*

### Comparing `rapo-0.4.3/rapo/utils.py` & `rapo-0.4.4/rapo/utils.py`

 * *Files identical despite different names*

### Comparing `rapo-0.4.3/rapo/web/__init__.py` & `rapo-0.4.4/rapo/web/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,19 +52,21 @@
 
     def start(self):
         """Start web API server."""
         if self.status is True and self.pid and psutil.pid_exists(self.pid):
             message = f'web API already running at PID {self.pid}'
             raise Exception(message)
         app = f'{self.app.name}:app'
+        exe = sys.executable
+        dir = os.path.dirname(exe)
         env = os.environ.copy()
         self.start_date = dt.datetime.now()
         self.status = True
         if self.dev is True:
-            script = ['flask', 'run']
+            script = [os.path.join(dir, 'flask'), 'run']
             args = ['--host', self.host, '--port', str(self.port)]
             cmd = [arg for arg in [*script, *args] if arg is not None]
             env['FLASK_APP'] = app
             env['FLASK_ENV'] = 'development'
             try:
                 proc = sp.Popen(cmd, env=env)
                 self.pid = proc.pid
@@ -83,15 +85,15 @@
                 self.stop_date = dt.datetime.now()
                 update = (self.table.update()
                                     .values(stop_date=self.stop_date,
                                             status='N'))
                 db.execute(update)
                 proc.terminate()
         else:
-            script = 'waitress-serve'
+            script = os.path.join(dir, 'waitress-serve')
             args = ['--host', self.host, '--port', str(self.port), app]
             cmd = [arg for arg in [script, *args] if arg is not None]
             proc = sp.Popen(cmd, env=env, stdout=sp.DEVNULL, stderr=sp.DEVNULL)
             self.pid = proc.pid
             update = self.table.update().values(server=self.server,
                                                 username=self.username,
                                                 pid=self.pid,
```

### Comparing `rapo-0.4.3/rapo/web/api/app.py` & `rapo-0.4.4/rapo/web/api/app.py`

 * *Files identical despite different names*

### Comparing `rapo-0.4.3/rapo.egg-info/PKG-INFO` & `rapo-0.4.4/rapo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapo
-Version: 0.4.3
+Version: 0.4.4
 Summary: Python Revenue Assurance Process Optimizer.
 Home-page: https://github.com/t3eHawk/rapo
 Author: Timur Faradzhov
 Author-email: timurfaradzhov@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `rapo-0.4.3/setup.py` & `rapo-0.4.4/setup.py`

 * *Files identical despite different names*

