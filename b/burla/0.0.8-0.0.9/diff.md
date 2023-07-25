# Comparing `tmp/burla-0.0.8.tar.gz` & `tmp/burla-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "burla-0.0.8.tar", max compression
+gzip compressed data, was "burla-0.0.9.tar", max compression
```

## Comparing `burla-0.0.8.tar` & `burla-0.0.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      503 2023-07-17 19:06:21.951421 burla-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      175 2023-07-13 18:25:13.491110 burla-0.0.8/src/burla/__init__.py
--rw-r--r--   0        0        0     1352 2023-07-12 19:34:52.816658 burla-0.0.8/src/burla/_logstream.py
--rw-r--r--   0        0        0      907 2023-07-13 18:24:57.649392 burla-0.0.8/src/burla/config.py
--rw-r--r--   0        0        0     4148 2023-07-17 19:06:03.804535 burla-0.0.8/src/burla/remote_parallel_map.py
--rw-r--r--   0        0        0      616 1970-01-01 00:00:00.000000 burla-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      503 2023-07-18 23:01:39.157499 burla-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      175 2023-07-13 18:25:13.491110 burla-0.0.9/src/burla/__init__.py
+-rw-r--r--   0        0        0     1352 2023-07-12 19:34:52.816658 burla-0.0.9/src/burla/_logstream.py
+-rw-r--r--   0        0        0      907 2023-07-13 18:24:57.649392 burla-0.0.9/src/burla/config.py
+-rw-r--r--   0        0        0     4407 2023-07-18 23:02:00.574713 burla-0.0.9/src/burla/remote_parallel_map.py
+-rw-r--r--   0        0        0      616 1970-01-01 00:00:00.000000 burla-0.0.9/PKG-INFO
```

### Comparing `burla-0.0.8/src/burla/_logstream.py` & `burla-0.0.9/src/burla/_logstream.py`

 * *Files identical despite different names*

### Comparing `burla-0.0.8/src/burla/config.py` & `burla-0.0.9/src/burla/config.py`

 * *Files identical despite different names*

### Comparing `burla-0.0.8/src/burla/remote_parallel_map.py` & `burla-0.0.9/src/burla/remote_parallel_map.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,44 +12,44 @@
 from tblib import pickling_support
 
 from burla._logstream import print_logs_from_queue
 from burla.config import load_api_key_from_local_config
 
 pickling_support.install()
 
-BURLA_SERVICE_URL = "https://burla-webservice-production-gxc7eo4ala-uc.a.run.app"
+BURLA_SERVICE_URL = "https://burla-webservice-prod-0-0-9-gxc7eo4ala-uc.a.run.app"
 # BURLA_SERVICE_URL = "https://burla-webservice-gxc7eo4ala-uc.a.run.app"
 # BURLA_SERVICE_URL = "https://127.0.0.1:5000"
 
 JOB_ENV_REPO = "us-east4-docker.pkg.dev/burla-389321/burla-job-environments"
 
 JOB_STATUS_POLL_RATE_SEC = 6  # how often to check for job completion
 TIMEOUT_MIN = 60 * 12  # max time a Burla job can run for
 
 
 class JobTimeoutError(Exception):
     def __init__(self, job_id, timeout):
         super().__init__(f"Burla job with id: '{job_id}' timed out after {timeout} seconds.")
 
 
-def _get_job_info(job_id: str, epoch: int, attempt=0):
+def _get_job_info(job_id: str, epoch: int, headers: dict, attempt=0):
     try:
-        response = requests.get(f"{BURLA_SERVICE_URL}/v1/jobs/{job_id}/{epoch}")
+        response = requests.get(f"{BURLA_SERVICE_URL}/v1/jobs/{job_id}/{epoch}", headers=headers)
         response.raise_for_status()
         return response.json()
     except requests.exceptions.HTTPError as e:
         if str(response.status_code).startswith("5") and attempt != 3:
             warnings.warn(
                 (
                     f"Received {response.status_code} response from server checking status of job: "
                     f"{job_id} Retrying..."
                 )
             )
             sleep(2)
-            return _get_job_info(job_id, epoch, attempt=attempt + 1)
+            return _get_job_info(job_id, epoch, headers, attempt=attempt + 1)
         else:
             raise e
 
 
 def remote_parallel_map(
     function_: Callable,
     inputs: list,
@@ -59,31 +59,34 @@
 ):
     if not function_.__annotations__.get("return") is str:
         raise AttributeError("Please add the return type annotation 'str' to your input function.")
 
     if cpus > 100:
         raise AttributeError("Currently unable to satisfy requests for > 100 computers")
 
-    api_key = api_key or load_api_key_from_local_config()
-    response = requests.post(f"{BURLA_SERVICE_URL}/v1/jobs/", json={"key": api_key})
+    # https://www.rfc-editor.org/rfc/rfc7235 <- specifies "correct" api key location
+    headers = {"Authorization": f"Bearer {api_key or load_api_key_from_local_config()}"}
+
+    response = requests.post(f"{BURLA_SERVICE_URL}/v1/jobs/", json={}, headers=headers)
     response.raise_for_status()
     job_id = response.json()["job_id"]
 
     user_python_version = f"{sys.version_info.major}.{sys.version_info.minor}"
     default_docker_image = f"{JOB_ENV_REPO}/python{user_python_version}/burla_job_env:latest"
 
     data = {
-        "key": api_key,
         "function_pkl_hex": dill.dumps(function_.__code__).hex(),
         "inputs": inputs,
         "image": image or default_docker_image,
         "num_computers": cpus,
     }
     job_started_at_epoch = int(time())
-    response = requests.post(f"{BURLA_SERVICE_URL}/v1/jobs/{job_id}", json=data)
+
+    # TODO: start this on separate thread so we can print logs before all subjobs are running.
+    response = requests.post(f"{BURLA_SERVICE_URL}/v1/jobs/{job_id}", json=data, headers=headers)
     response.raise_for_status()
 
     last_epoch = job_started_at_epoch
     epoch = last_epoch
     job_is_running = True
     job_timed_out = False
 
@@ -95,15 +98,15 @@
 
     # loop until job finishes, or times out
     while job_is_running and (not job_timed_out):
         # TODO: record and subtract time so this loop always takes exactly JOB_STATUS_POLL_RATE_SEC
         # sec to run? This might fix late logs?
         sleep(JOB_STATUS_POLL_RATE_SEC)
 
-        job = _get_job_info(job_id, last_epoch)
+        job = _get_job_info(job_id, last_epoch, headers)
 
         # add all logs to print queue
         for epoch, log_message in job["logs"]:
             print_queue.put((epoch, log_message))
 
         last_epoch = epoch
         job_is_running = job["job_is_done"] == False
```

### Comparing `burla-0.0.8/PKG-INFO` & `burla-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: burla
-Version: 0.0.8
+Version: 0.0.9
 Summary: Make your python script 100x faster
 Author: Jake Zuliani
 Author-email: jake@burla.dev
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

