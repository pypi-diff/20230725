# Comparing `tmp/work-1.0.0.tar.gz` & `tmp/work-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "work-1.0.0.tar", max compression
+gzip compressed data, was "work-1.0.1.tar", max compression
```

## Comparing `work-1.0.0.tar` & `work-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1033 2022-08-29 19:21:01.200221 work-1.0.0/README.md
--rw-r--r--   0        0        0      592 2023-07-21 15:26:51.039899 work-1.0.0/pyproject.toml
--rw-r--r--   0        0        0    88905 2023-07-21 14:03:58.320482 work-1.0.0/src/work.py
--rw-r--r--   0        0        0        0 2021-02-24 12:12:04.352563 work-1.0.0/src/work_components/__init__.py
--rw-r--r--   0        0        0    24173 2023-07-20 13:19:00.050197 work-1.0.0/src/work_components/arguments.py
--rw-r--r--   0        0        0     2045 2023-07-21 15:26:51.039899 work-1.0.0/src/work_components/consts.py
--rw-r--r--   0        0        0    22034 2023-07-18 16:04:16.421220 work-1.0.0/src/work_components/container.py
--rw-r--r--   0        0        0        0 2022-08-23 18:01:16.135701 work-1.0.0/src/work_components/dao/__init__.py
--rw-r--r--   0        0        0    15926 2023-07-05 14:46:26.049963 work-1.0.0/src/work_components/dao/core.py
--rw-r--r--   0        0        0     1523 2023-07-05 14:05:08.910489 work-1.0.0/src/work_components/dao/flags.py
--rw-r--r--   0        0        0    11530 2023-07-05 13:33:23.043915 work-1.0.0/src/work_components/dao/rc.py
--rw-r--r--   0        0        0    11011 2023-07-19 09:32:06.070610 work-1.0.0/src/work_components/dao/recess.py
--rw-r--r--   0        0        0     6209 2023-07-05 17:58:05.483335 work-1.0.0/src/work_components/dt_parse.py
--rw-r--r--   0        0        0     4400 2023-07-21 14:03:58.320482 work-1.0.0/src/work_components/migrate.py
--rw-r--r--   0        0        0      344 2023-07-05 13:32:05.419111 work-1.0.0/src/work_components/protocols.py
--rw-r--r--   0        0        0      471 2023-06-20 12:46:12.229256 work-1.0.0/src/work_components/timestamps.py
--rw-r--r--   0        0        0     8067 2023-07-11 18:36:01.409614 work-1.0.0/src/work_components/util.py
--rw-r--r--   0        0        0     1561 1970-01-01 00:00:00.000000 work-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1033 2022-08-29 19:21:01.200221 work-1.0.1/README.md
+-rw-r--r--   0        0        0      592 2023-07-25 18:13:04.321615 work-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0    88787 2023-07-25 18:11:55.336963 work-1.0.1/src/work.py
+-rw-r--r--   0        0        0        0 2021-02-24 12:12:04.352563 work-1.0.1/src/work_components/__init__.py
+-rw-r--r--   0        0        0    24173 2023-07-20 13:19:00.050197 work-1.0.1/src/work_components/arguments.py
+-rw-r--r--   0        0        0     2045 2023-07-25 18:13:09.261661 work-1.0.1/src/work_components/consts.py
+-rw-r--r--   0        0        0    22034 2023-07-18 16:04:16.421220 work-1.0.1/src/work_components/container.py
+-rw-r--r--   0        0        0        0 2022-08-23 18:01:16.135701 work-1.0.1/src/work_components/dao/__init__.py
+-rw-r--r--   0        0        0    15926 2023-07-05 14:46:26.049963 work-1.0.1/src/work_components/dao/core.py
+-rw-r--r--   0        0        0     1523 2023-07-05 14:05:08.910489 work-1.0.1/src/work_components/dao/flags.py
+-rw-r--r--   0        0        0    11530 2023-07-05 13:33:23.043915 work-1.0.1/src/work_components/dao/rc.py
+-rw-r--r--   0        0        0    11011 2023-07-19 09:32:06.070610 work-1.0.1/src/work_components/dao/recess.py
+-rw-r--r--   0        0        0     6209 2023-07-05 17:58:05.483335 work-1.0.1/src/work_components/dt_parse.py
+-rw-r--r--   0        0        0     4470 2023-07-25 18:11:55.340963 work-1.0.1/src/work_components/migrate.py
+-rw-r--r--   0        0        0      344 2023-07-05 13:32:05.419111 work-1.0.1/src/work_components/protocols.py
+-rw-r--r--   0        0        0      471 2023-06-20 12:46:12.229256 work-1.0.1/src/work_components/timestamps.py
+-rw-r--r--   0        0        0     8067 2023-07-11 18:36:01.409614 work-1.0.1/src/work_components/util.py
+-rw-r--r--   0        0        0     1561 1970-01-01 00:00:00.000000 work-1.0.1/PKG-INFO
```

### Comparing `work-1.0.0/README.md` & `work-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `work-1.0.0/pyproject.toml` & `work-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "work"
-version = "1.0.0"
+version = "1.0.1"
 description = "Manual time tracking via a CLI that works similarly to git."
 authors = ["vauhochzett <vauhoch@zett.cc>"]
 readme = "README.md"
 homepage = "https://vauhoch.zett.cc/work/"
 packages = [
     { include = "work.py", from = "src" },
     { include = "work_components", from = "src" },
```

### Comparing `work-1.0.0/src/work.py` & `work-1.0.1/src/work.py`

 * *Files 1% similar despite different names*

```diff
@@ -389,28 +389,28 @@
         start_time: Optional[dt.datetime] = self.dao.get_start_time()
 
         if start_time is None:
             raise InvalidOperationWarning.cant(
                 "stop work", "no run is currently active"
             )
 
+        if end_time == start_time:
+            self.dao.cancel_run()
+            raise InvalidOperationWarning(
+                "End time is identical to start time – run cancelled."
+            )
+
         self._can_i_add_this(
             start_time=start_time, end_time=end_time, operation="stop work"
         )
 
-        if end_time == start_time:
-            self.dao.cancel_run()
-            print("End time is identical to start time – run cancelled.")
-            return 0.0
-
         # Preconditions met: Run can be stopped.
         if not dry_run:
             self.dao.stop_run(end_time=end_time, category=category, message=message)
-            return Record(start=start_time, end=end_time).get_minutes()
-        return 0.0
+        return util.minutes_difference(start=start_time, end=end_time)
 
     # add #
 
     def add(self, args) -> None:
         """Add a protocol entry consisting of start time, end time and optional date flag."""
 
         start_time: dt.datetime
@@ -421,18 +421,14 @@
         self._can_i_add_this(
             start_time=start_time,
             end_time=end_time,
             operation="add entry",
             force=args.force,
         )
 
-        if end_time == start_time:
-            print("End time is identical to start time – did nothing.")
-            return
-
         if not args.dry_run:
             self.dao.add_protocol_entry(
                 start_time=start_time,
                 end_time=end_time,
                 category=args.category,
                 message=args.message,
                 force=args.force,
```

### Comparing `work-1.0.0/src/work_components/arguments.py` & `work-1.0.1/src/work_components/arguments.py`

 * *Files identical despite different names*

### Comparing `work-1.0.0/src/work_components/consts.py` & `work-1.0.1/src/work_components/consts.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 """ Shared constants """
 
 import os
 import pathlib
 from typing import List, Tuple
 
-VERSION: str = "1.0.0"
+VERSION: str = "1.0.1"
 RECORDS_VERSION: int = 3
 
 # Directories
 PARENT_DIR: pathlib.Path = pathlib.Path("~", ".local", "share").expanduser()
 DIRECTORY: pathlib.Path = PARENT_DIR.joinpath("work")
 DIRECTORY_DEBUG: pathlib.Path = PARENT_DIR.joinpath("debug", "work")
```

### Comparing `work-1.0.0/src/work_components/container.py` & `work-1.0.1/src/work_components/container.py`

 * *Files identical despite different names*

### Comparing `work-1.0.0/src/work_components/dao/core.py` & `work-1.0.1/src/work_components/dao/core.py`

 * *Files identical despite different names*

### Comparing `work-1.0.0/src/work_components/dao/flags.py` & `work-1.0.1/src/work_components/dao/flags.py`

 * *Files identical despite different names*

### Comparing `work-1.0.0/src/work_components/dao/rc.py` & `work-1.0.1/src/work_components/dao/rc.py`

 * *Files identical despite different names*

### Comparing `work-1.0.0/src/work_components/dao/recess.py` & `work-1.0.1/src/work_components/dao/recess.py`

 * *Files identical despite different names*

### Comparing `work-1.0.0/src/work_components/dt_parse.py` & `work-1.0.1/src/work_components/dt_parse.py`

 * *Files identical despite different names*

### Comparing `work-1.0.0/src/work_components/migrate.py` & `work-1.0.1/src/work_components/migrate.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,19 +115,22 @@
     """Print 'what's new' message for given version."""
     whatsnew_messages: Dict[str, Dict[str, str]] = {
         "0": {
             "100": """Configurable aliases and macros
 Configuration file location moved to match XDG Base Directory Specification
 Force rounding with arguments "now+", "now-", or prevent with "now!"
 Improved listing of free days in "free-days --list" """,
-            "101": """Skip interactive selection (edit, remove) with --all or --last
+        },
+        "1": {
+            "0": """New name on PyPI: work-time-log is now work!
+Skip interactive selection (edit, remove) with --all or --last
 Filtering applies smart case
 Day names and dates can be used interchangeably
 Flags --date and -D are deprecated""",
-        }
+        },
     }
 
     major, minor, *_ = version.split(".")
     if major not in whatsnew_messages or minor not in whatsnew_messages[major]:
         return
 
     message_shown_flag: str = f"whatsnew:{major}.{minor}"
```

### Comparing `work-1.0.0/src/work_components/util.py` & `work-1.0.1/src/work_components/util.py`

 * *Files identical despite different names*

### Comparing `work-1.0.0/PKG-INFO` & `work-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: work
-Version: 1.0.0
+Version: 1.0.1
 Summary: Manual time tracking via a CLI that works similarly to git.
 Home-page: https://vauhoch.zett.cc/work/
 Author: vauhochzett
 Author-email: vauhoch@zett.cc
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

