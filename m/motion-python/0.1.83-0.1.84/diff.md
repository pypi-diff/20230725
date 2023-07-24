# Comparing `tmp/motion_python-0.1.83.tar.gz` & `tmp/motion_python-0.1.84.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motion_python-0.1.83.tar", max compression
+gzip compressed data, was "motion_python-0.1.84.tar", max compression
```

## Comparing `motion_python-0.1.83.tar` & `motion_python-0.1.84.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     3344 2023-07-22 00:03:38.019174 motion_python-0.1.83/README.md
--rw-r--r--   0        0        0      344 2023-07-22 00:03:38.019174 motion_python-0.1.83/motion/__init__.py
--rw-r--r--   0        0        0     3867 2023-07-22 00:03:38.019174 motion_python-0.1.83/motion/cli.py
--rw-r--r--   0        0        0    24251 2023-07-22 00:03:38.019174 motion_python-0.1.83/motion/component.py
--rw-r--r--   0        0        0     4623 2023-07-22 00:03:38.019174 motion_python-0.1.83/motion/dicts.py
--rw-r--r--   0        0        0    17243 2023-07-22 00:03:38.019174 motion_python-0.1.83/motion/execute.py
--rw-r--r--   0        0        0    13682 2023-07-22 00:03:38.019174 motion_python-0.1.83/motion/instance.py
--rw-r--r--   0        0        0     4897 2023-07-22 00:03:38.019174 motion_python-0.1.83/motion/migrate.py
--rw-r--r--   0        0        0    13660 2023-07-22 00:03:38.019174 motion_python-0.1.83/motion/res/eff_short_wordlist_1.txt
--rw-r--r--   0        0        0     1153 2023-07-22 00:03:38.019174 motion_python-0.1.83/motion/route.py
--rw-r--r--   0        0        0     4545 2023-07-22 00:03:38.019174 motion_python-0.1.83/motion/server/update_task.py
--rw-r--r--   0        0        0     9966 2023-07-22 00:03:38.019174 motion_python-0.1.83/motion/utils.py
--rw-r--r--   0        0        0     1782 2023-07-22 00:03:58.623507 motion_python-0.1.83/pyproject.toml
--rw-r--r--   0        0        0     4128 1970-01-01 00:00:00.000000 motion_python-0.1.83/PKG-INFO
+-rw-r--r--   0        0        0     3344 2023-07-24 22:06:42.644584 motion_python-0.1.84/README.md
+-rw-r--r--   0        0        0      344 2023-07-24 22:06:42.644584 motion_python-0.1.84/motion/__init__.py
+-rw-r--r--   0        0        0     3867 2023-07-24 22:06:42.644584 motion_python-0.1.84/motion/cli.py
+-rw-r--r--   0        0        0    24251 2023-07-24 22:06:42.644584 motion_python-0.1.84/motion/component.py
+-rw-r--r--   0        0        0     4623 2023-07-24 22:06:42.644584 motion_python-0.1.84/motion/dicts.py
+-rw-r--r--   0        0        0    17268 2023-07-24 22:06:42.644584 motion_python-0.1.84/motion/execute.py
+-rw-r--r--   0        0        0    13682 2023-07-24 22:06:42.644584 motion_python-0.1.84/motion/instance.py
+-rw-r--r--   0        0        0     4897 2023-07-24 22:06:42.644584 motion_python-0.1.84/motion/migrate.py
+-rw-r--r--   0        0        0    13660 2023-07-24 22:06:42.644584 motion_python-0.1.84/motion/res/eff_short_wordlist_1.txt
+-rw-r--r--   0        0        0     1153 2023-07-24 22:06:42.644584 motion_python-0.1.84/motion/route.py
+-rw-r--r--   0        0        0     4574 2023-07-24 22:06:42.644584 motion_python-0.1.84/motion/server/update_task.py
+-rw-r--r--   0        0        0    10019 2023-07-24 22:06:42.644584 motion_python-0.1.84/motion/utils.py
+-rw-r--r--   0        0        0     1782 2023-07-24 22:07:05.928714 motion_python-0.1.84/pyproject.toml
+-rw-r--r--   0        0        0     4128 1970-01-01 00:00:00.000000 motion_python-0.1.84/PKG-INFO
```

### Comparing `motion_python-0.1.83/README.md` & `motion_python-0.1.84/README.md`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.83/motion/cli.py` & `motion_python-0.1.84/motion/cli.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.83/motion/component.py` & `motion_python-0.1.84/motion/component.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.83/motion/dicts.py` & `motion_python-0.1.84/motion/dicts.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.83/motion/execute.py` & `motion_python-0.1.84/motion/execute.py`

 * *Files 0% similar despite different names*

```diff
@@ -226,16 +226,16 @@
     def _updateState(self, new_state: Dict[str, Any]) -> None:
         if not new_state:
             return
 
         if not isinstance(new_state, dict):
             raise TypeError("State should be a dict.")
 
-        with self._redis_con.lock(self._instance_name):
-            # Get latest state
+        # Get latest state
+        with self._redis_con.lock(f"MOTION_LOCK:{self._instance_name}", timeout=30):
             self._state = self._loadState()
             self._state.update(new_state)
 
             # Save state to redis
             saveState(
                 self._state,
                 self._redis_con,
```

### Comparing `motion_python-0.1.83/motion/instance.py` & `motion_python-0.1.84/motion/instance.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.83/motion/migrate.py` & `motion_python-0.1.84/motion/migrate.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.83/motion/res/eff_short_wordlist_1.txt` & `motion_python-0.1.84/motion/res/eff_short_wordlist_1.txt`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.83/motion/route.py` & `motion_python-0.1.84/motion/route.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.83/motion/server/update_task.py` & `motion_python-0.1.84/motion/server/update_task.py`

 * *Files 4% similar despite different names*

```diff
@@ -91,15 +91,15 @@
                         }
                     ),
                 )
                 continue
 
             # Run update op
             try:
-                with redis_con.lock(self.instance_name):
+                with redis_con.lock(f"MOTION_LOCK:{self.instance_name}", timeout=30):
                     old_state = loadState(
                         redis_con,
                         self.instance_name,
                         self.load_state_func,
                     )
                     state_update = self.routes[queue_name].run(
                         state=old_state,
```

### Comparing `motion_python-0.1.83/motion/utils.py` & `motion_python-0.1.84/motion/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,14 +121,15 @@
     # Check if the instance exists
     if not redis_con.exists(f"MOTION_VERSION:{instance_name}"):
         return False
 
     # Delete the instance state, version, and cached results
     redis_con.delete(f"MOTION_STATE:{instance_name}")
     redis_con.delete(f"MOTION_VERSION:{instance_name}")
+    redis_con.delete(f"MOTION_LOCK:{instance_name}")
 
     results_to_delete = redis_con.keys(f"MOTION_RESULT:{instance_name}/*")
     queues_to_delete = redis_con.keys(f"MOTION_QUEUE:{instance_name}/*")
     pipeline = redis_con.pipeline()
     for result in results_to_delete:
         pipeline.delete(result)
     for queue in queues_to_delete:
```

### Comparing `motion_python-0.1.83/pyproject.toml` & `motion_python-0.1.84/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "motion-python"
-version = "0.1.83"
+version = "0.1.84"
 description = "A trigger-based framework for creating and executing ML pipelines."
 authors = ["Shreya Shankar <shreyashankar@berkeley.edu>"]
 readme = "README.md"
 packages = [{include = "motion"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `motion_python-0.1.83/PKG-INFO` & `motion_python-0.1.84/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motion-python
-Version: 0.1.83
+Version: 0.1.84
 Summary: A trigger-based framework for creating and executing ML pipelines.
 Author: Shreya Shankar
 Author-email: shreyashankar@berkeley.edu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

