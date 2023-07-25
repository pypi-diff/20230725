# Comparing `tmp/trycortex-1.0.7.tar.gz` & `tmp/trycortex-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trycortex-1.0.7.tar", max compression
+gzip compressed data, was "trycortex-1.0.8.tar", max compression
```

## Comparing `trycortex-1.0.7.tar` & `trycortex-1.0.8.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       57 2023-07-13 22:45:36.236046 trycortex-1.0.7/README.md
--rw-r--r--   0        0        0      489 2023-07-24 19:09:04.145004 trycortex-1.0.7/pyproject.toml
--rw-r--r--   0        0        0       90 2023-07-13 21:47:58.631841 trycortex-1.0.7/trycortex/__init__.py
--rw-r--r--   0        0        0    12976 2023-07-19 20:20:29.647945 trycortex-1.0.7/trycortex/api.py
--rw-r--r--   0        0        0        0 2023-07-13 23:06:56.199856 trycortex-1.0.7/trycortex/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-07-14 22:58:20.969482 trycortex-1.0.7/trycortex/cli/callable/__init__.py
--rw-r--r--   0        0        0     1600 2023-07-17 18:57:14.549510 trycortex-1.0.7/trycortex/cli/callable/callable_config.py
--rw-r--r--   0        0        0     6858 2023-07-24 18:49:55.816281 trycortex-1.0.7/trycortex/cli/callable/commands.py
--rw-r--r--   0        0        0      308 2023-07-13 23:09:13.654204 trycortex-1.0.7/trycortex/cli/cli.py
--rw-r--r--   0        0        0     1522 2023-07-15 00:34:23.304330 trycortex-1.0.7/trycortex/cli/utils.py
--rw-r--r--   0        0        0      855 1970-01-01 00:00:00.000000 trycortex-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0       57 2023-07-13 22:45:36.236046 trycortex-1.0.8/README.md
+-rw-r--r--   0        0        0      489 2023-07-25 21:49:43.355138 trycortex-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0       90 2023-07-13 21:47:58.631841 trycortex-1.0.8/trycortex/__init__.py
+-rw-r--r--   0        0        0    12976 2023-07-19 20:20:29.647945 trycortex-1.0.8/trycortex/api.py
+-rw-r--r--   0        0        0        0 2023-07-13 23:06:56.199856 trycortex-1.0.8/trycortex/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-14 22:58:20.969482 trycortex-1.0.8/trycortex/cli/callable/__init__.py
+-rw-r--r--   0        0        0     1600 2023-07-25 19:54:37.293457 trycortex-1.0.8/trycortex/cli/callable/callable_config.py
+-rw-r--r--   0        0        0     6869 2023-07-25 21:48:58.385594 trycortex-1.0.8/trycortex/cli/callable/commands.py
+-rw-r--r--   0        0        0      308 2023-07-25 19:54:52.811386 trycortex-1.0.8/trycortex/cli/cli.py
+-rw-r--r--   0        0        0     1522 2023-07-15 00:34:23.304330 trycortex-1.0.8/trycortex/cli/utils.py
+-rw-r--r--   0        0        0      855 1970-01-01 00:00:00.000000 trycortex-1.0.8/PKG-INFO
```

### Comparing `trycortex-1.0.7/trycortex/api.py` & `trycortex-1.0.8/trycortex/api.py`

 * *Files identical despite different names*

### Comparing `trycortex-1.0.7/trycortex/cli/callable/callable_config.py` & `trycortex-1.0.8/trycortex/cli/callable/callable_config.py`

 * *Files identical despite different names*

### Comparing `trycortex-1.0.7/trycortex/cli/callable/commands.py` & `trycortex-1.0.8/trycortex/cli/callable/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,38 +38,38 @@
     s = re.sub(r"[\s_-]+", "-", s)
     s = s.strip("-")
     return s
 
 def _update_callable_requirements(
     existing_requirements: List[str], new_requirements: List[str]
 ) -> List[str]:
-    """Returns an updated list of agent requirements to go in requirements.txt."""
+    """Returns an updated list of callable requirements to go in requirements.txt."""
 
-    # If the user specified a fixieai requirement, use that.
-    fixie_requirement = next(
+    # If the user specified a trycortex requirement, use that.
+    cortex_requirement = next(
         filter(
             functools.partial(re.match, CORTEX_REQUIREMENT_PATTERN), new_requirements
         ),
         CURRENT_CORTEX_REQUIREMENT,
     )
 
-    # Ensure that a compatible version of the Fixie SDK is present.
+    # Ensure that a compatible version of the Cortex SDK is present.
     resolved_requirements: List[str] = []
 
     for existing_requirement in existing_requirements:
         if (
             re.match(CORTEX_REQUIREMENT_PATTERN, existing_requirement)
-            and existing_requirement != fixie_requirement
+            and existing_requirement != cortex_requirement
         ):
-            # Ignore any existing (but different) fixieai requirements.
+            # Ignore any existing (but different) cortex requirements.
             continue
 
         resolved_requirements.append(existing_requirement)
 
-    for new_requirement in [fixie_requirement] + new_requirements:
+    for new_requirement in [cortex_requirement] + new_requirements:
         if new_requirement not in resolved_requirements:
             resolved_requirements.append(new_requirement)
 
     return resolved_requirements
 
 @callable.command("init", help="Creates an callable.yaml file.")
 @click.option("--name", help="Name of the callable.")
@@ -145,15 +145,15 @@
         with open(path / REQUIREMENTS_TXT, "rt") as requirements_txt:
             existing_requirements = list(
                 r.strip() for r in requirements_txt.readlines()
             )
     except FileNotFoundError:
         existing_requirements = []
 
-    resolved_requirements = _update_agent_requirements(
+    resolved_requirements = _update_callable_requirements(
         existing_requirements, list(requirement)
     )
     if not existing_requirements:
         write_requirements = True
     else:
         new_requirements = [
             r for r in resolved_requirements if r not in existing_requirements
```

### Comparing `trycortex-1.0.7/trycortex/cli/utils.py` & `trycortex-1.0.8/trycortex/cli/utils.py`

 * *Files identical despite different names*

### Comparing `trycortex-1.0.7/PKG-INFO` & `trycortex-1.0.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trycortex
-Version: 1.0.7
+Version: 1.0.8
 Summary: Python library for Cortex
 Author: Charles
 Author-email: charlespun6@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

