# Comparing `tmp/logassistant-0.1.1.tar.gz` & `tmp/logassistant-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logassistant-0.1.1.tar", last modified: Mon Jul 24 21:58:41 2023, max compression
+gzip compressed data, was "logassistant-0.1.2.tar", last modified: Mon Jul 24 22:22:14 2023, max compression
```

## Comparing `logassistant-0.1.1.tar` & `logassistant-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:58:41.385785 logassistant-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-24 21:58:27.000000 logassistant-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-24 21:58:41.385785 logassistant-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-07-24 21:58:27.000000 logassistant-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 21:58:41.385785 logassistant-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-24 21:58:27.000000 logassistant-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:58:41.385785 logassistant-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:58:41.385785 logassistant-0.1.1/src/logassistant/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-24 21:58:27.000000 logassistant-0.1.1/src/logassistant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4314 2023-07-24 21:58:27.000000 logassistant-0.1.1/src/logassistant/logassistant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:58:41.385785 logassistant-0.1.1/src/logassistant.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-24 21:58:41.000000 logassistant-0.1.1/src/logassistant.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-24 21:58:41.000000 logassistant-0.1.1/src/logassistant.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 21:58:41.000000 logassistant-0.1.1/src/logassistant.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-24 21:58:41.000000 logassistant-0.1.1/src/logassistant.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-24 21:58:41.000000 logassistant-0.1.1/src/logassistant.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-24 21:58:41.000000 logassistant-0.1.1/src/logassistant.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:22:14.177022 logassistant-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-24 22:22:00.000000 logassistant-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-24 22:22:14.177022 logassistant-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-07-24 22:22:00.000000 logassistant-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 22:22:14.177022 logassistant-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-24 22:22:00.000000 logassistant-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:22:14.177022 logassistant-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:22:14.177022 logassistant-0.1.2/src/logassistant/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-24 22:22:00.000000 logassistant-0.1.2/src/logassistant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-07-24 22:22:00.000000 logassistant-0.1.2/src/logassistant/logassistant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:22:14.177022 logassistant-0.1.2/src/logassistant.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-24 22:22:14.000000 logassistant-0.1.2/src/logassistant.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-24 22:22:14.000000 logassistant-0.1.2/src/logassistant.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 22:22:14.000000 logassistant-0.1.2/src/logassistant.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-24 22:22:14.000000 logassistant-0.1.2/src/logassistant.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-24 22:22:14.000000 logassistant-0.1.2/src/logassistant.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-24 22:22:14.000000 logassistant-0.1.2/src/logassistant.egg-info/top_level.txt
```

### Comparing `logassistant-0.1.1/LICENSE` & `logassistant-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `logassistant-0.1.1/README.md` & `logassistant-0.1.2/README.md`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -50,8 +50,8 @@
 - requests
 - openai
 
 # License
 This project is licensed under the MIT License. See the LICENSE file for more details.
 
 # Contributing
-Contributions to the Log Assistant are welcome! If you encounter any issues or have ideas for improvements, please feel free to open an issue or submit a pull request on our GitHub repository.
+Contributions to the Log Assistant are welcome! If you encounter any issues or have ideas for improvements, please feel free to open an issue or submit a pull request on our GitHub repository.
```

### Comparing `logassistant-0.1.1/setup.py` & `logassistant-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Function to read the requirements from requirements.txt
 def parse_requirements(filename):
     with open(filename) as f:
         return [line.strip() for line in f if line.strip()]
 
 setuptools.setup(
     name='logassistant',
-    version='0.1.1',
+    version='0.1.2',
     package_dir={'': 'src'},
     packages=setuptools.find_packages(where='src'),
     install_requires=parse_requirements('requirements.txt'),  # Read from requirements.txt
     entry_points={
         'console_scripts': [
             'log_assist_script = main:main',
         ],
```

### Comparing `logassistant-0.1.1/src/logassistant/logassistant.py` & `logassistant-0.1.2/src/logassistant/logassistant.py`

 * *Files 6% similar despite different names*

```diff
@@ -96,26 +96,27 @@
 
             # Convert the function arguments to a string representation
             arguments_str = ", ".join(f"{key}={value}" for key, value in function_arguments.items())
 
             # Execute the function with the provided arguments
             result = func(*args, **kwargs)
 
-            # Prepare the log message
-            request_content = f"""Analyze this function call as if it was executed and create a log message that a programmer would write as a sentence, don't write any prefixes: 
+            # Prepare the prompt
+            prompt = f"""Analyze this function call as if it was executed and create a log message that 
+                a programmer would write as a sentence, don't write any prefixes. Try to summarize what the function does in short. 
                 The function is: {source_code} with parameters: {arguments_str}. The result was {result}"""
 
             print(
                 f"Analyzing {function_name} call with parameters: {arguments_str} ...",
                 end="",
                 flush=True,
             )
 
             # Send the log message to ChatGPT
-            response = self.send_request(request_content)
+            response = self.send_request(prompt)
 
             print(
                 "\r" + " " * (shutil.get_terminal_size().columns - 1), end="\r"
             )  # Delete the loading message
             print(f"{self.function_call_count}.\t{response}")
             self.print_horizontal_line()
```

