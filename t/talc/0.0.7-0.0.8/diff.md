# Comparing `tmp/talc-0.0.7.tar.gz` & `tmp/talc-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talc-0.0.7.tar", last modified: Fri Jul 21 22:22:06 2023, max compression
+gzip compressed data, was "talc-0.0.8.tar", last modified: Tue Jul 25 05:00:16 2023, max compression
```

## Comparing `talc-0.0.7.tar` & `talc-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 mkerr      (501) staff       (20)        0 2023-07-21 22:22:06.810775 talc-0.0.7/
--rw-r--r--   0 mkerr      (501) staff       (20)        0 2023-07-05 18:11:13.000000 talc-0.0.7/LICENSE
--rw-r--r--   0 mkerr      (501) staff       (20)     2065 2023-07-21 22:22:06.810666 talc-0.0.7/PKG-INFO
--rw-r--r--   0 mkerr      (501) staff       (20)     1642 2023-07-20 23:07:33.000000 talc-0.0.7/README.md
--rw-r--r--   0 mkerr      (501) staff       (20)      585 2023-07-21 22:21:50.000000 talc-0.0.7/pyproject.toml
--rw-r--r--   0 mkerr      (501) staff       (20)       38 2023-07-21 22:22:06.810805 talc-0.0.7/setup.cfg
-drwxr-xr-x   0 mkerr      (501) staff       (20)        0 2023-07-21 22:22:06.809343 talc-0.0.7/src/
-drwxr-xr-x   0 mkerr      (501) staff       (20)        0 2023-07-21 22:22:06.809848 talc-0.0.7/src/talc/
--rw-r--r--   0 mkerr      (501) staff       (20)        0 2023-07-05 18:12:06.000000 talc-0.0.7/src/talc/__init__.py
--rw-r--r--   0 mkerr      (501) staff       (20)    10653 2023-07-21 22:20:08.000000 talc-0.0.7/src/talc/talc.py
-drwxr-xr-x   0 mkerr      (501) staff       (20)        0 2023-07-21 22:22:06.810529 talc-0.0.7/src/talc.egg-info/
--rw-r--r--   0 mkerr      (501) staff       (20)     2065 2023-07-21 22:22:06.000000 talc-0.0.7/src/talc.egg-info/PKG-INFO
--rw-r--r--   0 mkerr      (501) staff       (20)      229 2023-07-21 22:22:06.000000 talc-0.0.7/src/talc.egg-info/SOURCES.txt
--rw-r--r--   0 mkerr      (501) staff       (20)        1 2023-07-21 22:22:06.000000 talc-0.0.7/src/talc.egg-info/dependency_links.txt
--rw-r--r--   0 mkerr      (501) staff       (20)       31 2023-07-21 22:22:06.000000 talc-0.0.7/src/talc.egg-info/requires.txt
--rw-r--r--   0 mkerr      (501) staff       (20)        5 2023-07-21 22:22:06.000000 talc-0.0.7/src/talc.egg-info/top_level.txt
+drwxr-xr-x   0 mkerr      (501) staff       (20)        0 2023-07-25 05:00:16.529008 talc-0.0.8/
+-rw-r--r--   0 mkerr      (501) staff       (20)        0 2023-07-05 18:11:13.000000 talc-0.0.8/LICENSE
+-rw-r--r--   0 mkerr      (501) staff       (20)     2065 2023-07-25 05:00:16.528892 talc-0.0.8/PKG-INFO
+-rw-r--r--   0 mkerr      (501) staff       (20)     1642 2023-07-20 23:07:33.000000 talc-0.0.8/README.md
+-rw-r--r--   0 mkerr      (501) staff       (20)      585 2023-07-25 04:59:13.000000 talc-0.0.8/pyproject.toml
+-rw-r--r--   0 mkerr      (501) staff       (20)       38 2023-07-25 05:00:16.529043 talc-0.0.8/setup.cfg
+drwxr-xr-x   0 mkerr      (501) staff       (20)        0 2023-07-25 05:00:16.527366 talc-0.0.8/src/
+drwxr-xr-x   0 mkerr      (501) staff       (20)        0 2023-07-25 05:00:16.527883 talc-0.0.8/src/talc/
+-rw-r--r--   0 mkerr      (501) staff       (20)        0 2023-07-05 18:12:06.000000 talc-0.0.8/src/talc/__init__.py
+-rw-r--r--   0 mkerr      (501) staff       (20)    15270 2023-07-25 04:53:42.000000 talc-0.0.8/src/talc/talc.py
+drwxr-xr-x   0 mkerr      (501) staff       (20)        0 2023-07-25 05:00:16.528736 talc-0.0.8/src/talc.egg-info/
+-rw-r--r--   0 mkerr      (501) staff       (20)     2065 2023-07-25 05:00:16.000000 talc-0.0.8/src/talc.egg-info/PKG-INFO
+-rw-r--r--   0 mkerr      (501) staff       (20)      229 2023-07-25 05:00:16.000000 talc-0.0.8/src/talc.egg-info/SOURCES.txt
+-rw-r--r--   0 mkerr      (501) staff       (20)        1 2023-07-25 05:00:16.000000 talc-0.0.8/src/talc.egg-info/dependency_links.txt
+-rw-r--r--   0 mkerr      (501) staff       (20)       31 2023-07-25 05:00:16.000000 talc-0.0.8/src/talc.egg-info/requires.txt
+-rw-r--r--   0 mkerr      (501) staff       (20)        5 2023-07-25 05:00:16.000000 talc-0.0.8/src/talc.egg-info/top_level.txt
```

### Comparing `talc-0.0.7/PKG-INFO` & `talc-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talc
-Version: 0.0.7
+Version: 0.0.8
 Summary: Logging client for Talc Debugger.
 Author-email: Max Kerr <max@talc.ai>, Matt Lee <matt@talc.ai>
 Project-URL: homepage, https://talc.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `talc-0.0.7/README.md` & `talc-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `talc-0.0.7/pyproject.toml` & `talc-0.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "talc"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Max Kerr", email="max@talc.ai" },
   { name="Matt Lee", email="matt@talc.ai" },
 ]
 description = "Logging client for Talc Debugger."
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `talc-0.0.7/src/talc/talc.py` & `talc-0.0.8/src/talc/talc.py`

 * *Files 16% similar despite different names*

```diff
@@ -143,18 +143,17 @@
     @classmethod
     def create(cls, *args, **kwargs):
         # Pop arguments that are not supported by the original create method
         agent = kwargs.pop("agent", "Default")
         session = kwargs.pop("session", None)
         stream = "stream" in kwargs and kwargs["stream"]
 
-        result = super().create(*args, **kwargs)
-
         # Handle case where we have received the full response at once.
         if not stream:
+            result = super().create(*args, **kwargs)
             try:
                 functions_available, parameters = cls.__getFunctionsAndParameters(
                     **kwargs
                 )
                 text_content, function_calls = cls.__getContent(result.choices)
                 if session and agent:
                     client.log(
@@ -259,28 +258,141 @@
                     parameters,
                 )
         except Exception as e:
             logging.warning("Error logging to talc: ", e)
 
         return final_choice
 
+    @classmethod
+    async def __streamContentAsync(cls, *args, **kwargs):
+        agent = kwargs.pop("agent", "Default")
+        session = kwargs.pop("session", None)
+
+        generator = super().acreate(*args, **kwargs)
+
+        choices = {}
+        final_choice = None
+
+        async for result in await generator:
+            contains_incomplete_option = False
+            for index, choice in enumerate(result.choices):
+                # Identify if we have at least one incomplete option still streaming
+                if choice.finish_reason is None:
+                    contains_incomplete_option = True
+
+                if index not in choices:
+                    choices[index] = []
+                choices[index].append(choice)
+            if not contains_incomplete_option:
+                final_choice = result
+                break  # We have received the full response, break before returning so we can log.
+            yield result
+
+        final_content = []
+        final_function_calls = []
+
+        # Try not to find bugs in this code, because it's going to be
+        # a pain to fix.
+        try:
+            # Accumulate all the content and function calls for each option
+            for option in choices:
+                content_accumulator = []
+                function_call_accumulator = []
+                arguments_accumulator = []
+                for chunk in choices[option]:
+                    if "delta" in chunk:
+                        if "content" in chunk.delta:
+                            content_accumulator.append(chunk.delta["content"])
+                        if "function_call" in chunk.delta:
+                            if "name" in chunk.delta["function_call"]:
+                                function_call_accumulator.append(
+                                    chunk.delta["function_call"]["name"]
+                                )
+                            if "arguments" in chunk.delta["function_call"]:
+                                arguments_accumulator.append(
+                                    chunk.delta["function_call"]["arguments"]
+                                )
+                if len(content_accumulator) > 0:
+                    final_content.append(
+                        "".join([x for x in content_accumulator if x != None])
+                    )
+                else:
+                    final_content.append(None)
+                if len(function_call_accumulator) > 0:
+                    final_function_calls.append(
+                        {
+                            "name": "".join(
+                                [x for x in function_call_accumulator if x != None]
+                            ),
+                            "arguments": "".join(
+                                [x for x in arguments_accumulator if x != None]
+                            ),
+                        }
+                    )
+                else:
+                    final_function_calls.append(None)
+            # Log the accumulated options
+            if session and agent:
+                functions_available, parameters = cls.__getFunctionsAndParameters(
+                    **kwargs
+                )
+                client.log(
+                    session,
+                    kwargs["messages"],
+                    final_content,
+                    final_function_calls,
+                    agent,
+                    functions_available,
+                    parameters,
+                )
+        except Exception as e:
+            logging.warning("Error logging to talc: ", e)
+
+        yield final_choice
+        return
+
         # print("Content ", option, ":", "".join(content_accumulator))
         # print("Function call ", option, ":", "".join(function_call_accumulator))
         # print("Arguments ", option, ":", "".join(arguments_accumulator))
         # print("=====================================")
 
     @classmethod
     async def acreate(cls, *args, **kwargs):
         # Pop arguments that are not supported by the original create method
-        agent = kwargs.pop("agent", None)
+        agent = kwargs.pop("agent", "Default")
         session = kwargs.pop("session", None)
+        stream = "stream" in kwargs and kwargs["stream"]
 
-        result = await super().acreate(*args, **kwargs)
+        # Handle case where we have received the full response at once.
+        if not stream:
+            result = await super().acreate(*args, **kwargs)
+            try:
+                functions_available, parameters = cls.__getFunctionsAndParameters(
+                    **kwargs
+                )
+                text_content, function_calls = cls.__getContent(result.choices)
+                if session and agent:
+                    client.log(
+                        session,
+                        kwargs["messages"],
+                        text_content,
+                        function_calls,
+                        agent,
+                        functions_available,
+                        parameters,
+                    )
+            except Exception as e:
+                logging.warning("Error logging to talc: ", e)
 
-        return result
+            return result
+        # Handle stream case
+        else:
+            return cls.__streamContentAsync(
+                session=session, agent=agent, *args, **kwargs
+            )
 
     @classmethod
     def __getContent(cls, choices):
         text_content = []
         function_calls = []
 
         for choice in choices:
```

### Comparing `talc-0.0.7/src/talc.egg-info/PKG-INFO` & `talc-0.0.8/src/talc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talc
-Version: 0.0.7
+Version: 0.0.8
 Summary: Logging client for Talc Debugger.
 Author-email: Max Kerr <max@talc.ai>, Matt Lee <matt@talc.ai>
 Project-URL: homepage, https://talc.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

