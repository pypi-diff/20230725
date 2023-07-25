# Comparing `tmp/crepex_pyutil-0.7.0.tar.gz` & `tmp/crepex_pyutil-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crepex_pyutil-0.7.0.tar", max compression
+gzip compressed data, was "crepex_pyutil-0.8.0.tar", max compression
```

## Comparing `crepex_pyutil-0.7.0.tar` & `crepex_pyutil-0.8.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      791 2023-04-12 09:41:55.227358 crepex_pyutil-0.7.0/README.md
--rw-r--r--   0        0        0      413 2023-07-25 02:22:02.525119 crepex_pyutil-0.7.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-12 06:42:39.752853 crepex_pyutil-0.7.0/src/crepex_pyutil/__init__.py
--rw-r--r--   0        0        0     1263 2023-07-25 01:32:47.149766 crepex_pyutil-0.7.0/src/crepex_pyutil/collections.py
--rwxr-xr-x   0        0        0     3246 2023-07-01 09:13:24.096916 crepex_pyutil-0.7.0/src/crepex_pyutil/dates.py
--rw-r--r--   0        0        0      713 2023-07-25 02:20:50.521194 crepex_pyutil-0.7.0/src/crepex_pyutil/exceptions.py
--rw-r--r--   0        0        0      266 2023-07-25 02:15:01.661489 crepex_pyutil-0.7.0/src/crepex_pyutil/math.py
--rw-r--r--   0        0        0       81 2023-05-15 08:44:18.527777 crepex_pyutil-0.7.0/src/crepex_pyutil/requests/__init__.py
--rw-r--r--   0        0        0     2107 2023-04-12 06:02:06.720570 crepex_pyutil-0.7.0/src/crepex_pyutil/requests/helper.py
--rw-r--r--   0        0        0     2197 2023-05-15 08:45:17.992026 crepex_pyutil-0.7.0/src/crepex_pyutil/requests/slack.py
--rwxr-xr-x   0        0        0     1726 2023-04-27 01:58:48.842662 crepex_pyutil-0.7.0/src/crepex_pyutil/string.py
--rw-r--r--   0        0        0     1303 1970-01-01 00:00:00.000000 crepex_pyutil-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0      791 2023-04-12 09:41:55.227358 crepex_pyutil-0.8.0/README.md
+-rw-r--r--   0        0        0      413 2023-07-25 04:37:10.279538 crepex_pyutil-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-12 06:42:39.752853 crepex_pyutil-0.8.0/src/crepex_pyutil/__init__.py
+-rw-r--r--   0        0        0     1789 2023-07-25 04:36:44.867030 crepex_pyutil-0.8.0/src/crepex_pyutil/collections.py
+-rwxr-xr-x   0        0        0     3246 2023-07-01 09:13:24.096916 crepex_pyutil-0.8.0/src/crepex_pyutil/dates.py
+-rw-r--r--   0        0        0      713 2023-07-25 02:20:50.521194 crepex_pyutil-0.8.0/src/crepex_pyutil/exceptions.py
+-rw-r--r--   0        0        0      266 2023-07-25 02:15:01.661489 crepex_pyutil-0.8.0/src/crepex_pyutil/math.py
+-rw-r--r--   0        0        0       81 2023-05-15 08:44:18.527777 crepex_pyutil-0.8.0/src/crepex_pyutil/requests/__init__.py
+-rw-r--r--   0        0        0     2107 2023-04-12 06:02:06.720570 crepex_pyutil-0.8.0/src/crepex_pyutil/requests/helper.py
+-rw-r--r--   0        0        0     2197 2023-05-15 08:45:17.992026 crepex_pyutil-0.8.0/src/crepex_pyutil/requests/slack.py
+-rwxr-xr-x   0        0        0     1726 2023-04-27 01:58:48.842662 crepex_pyutil-0.8.0/src/crepex_pyutil/string.py
+-rw-r--r--   0        0        0     1303 1970-01-01 00:00:00.000000 crepex_pyutil-0.8.0/PKG-INFO
```

### Comparing `crepex_pyutil-0.7.0/README.md` & `crepex_pyutil-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `crepex_pyutil-0.7.0/src/crepex_pyutil/collections.py` & `crepex_pyutil-0.8.0/src/crepex_pyutil/collections.py`

 * *Files 23% similar despite different names*

```diff
@@ -32,7 +32,27 @@
     """
     dict list를 dict 요소의 주어진 키에 대한 값을 기준으로 dict map으로 전환
     :param key: dict 내부의 키
     :param values: 대상값
     :return: 변환된 dict
     """
     return {obj[key]: obj for obj in values}
+
+
+def omit(dictionary: dict, keys: list):
+    """
+    dict 에서 특정한 키를 제외하고 반환
+    :param dictionary: 대상
+    :param keys: 제외할 key
+    :return: dict
+    """
+    return {key: dictionary[key] for key in dictionary if key not in keys}
+
+
+def pick(dictionary: dict, keys: list):
+    """
+    dict 에서 특정한 키만 선택하여 반환
+    :param dictionary: 대상
+    :param keys: 선택할 key
+    :return: dict
+    """
+    return {key: dictionary[key] for key in dictionary if key in keys}
```

### Comparing `crepex_pyutil-0.7.0/src/crepex_pyutil/dates.py` & `crepex_pyutil-0.8.0/src/crepex_pyutil/dates.py`

 * *Files identical despite different names*

### Comparing `crepex_pyutil-0.7.0/src/crepex_pyutil/exceptions.py` & `crepex_pyutil-0.8.0/src/crepex_pyutil/exceptions.py`

 * *Files identical despite different names*

### Comparing `crepex_pyutil-0.7.0/src/crepex_pyutil/requests/helper.py` & `crepex_pyutil-0.8.0/src/crepex_pyutil/requests/helper.py`

 * *Files identical despite different names*

### Comparing `crepex_pyutil-0.7.0/src/crepex_pyutil/requests/slack.py` & `crepex_pyutil-0.8.0/src/crepex_pyutil/requests/slack.py`

 * *Files identical despite different names*

### Comparing `crepex_pyutil-0.7.0/src/crepex_pyutil/string.py` & `crepex_pyutil-0.8.0/src/crepex_pyutil/string.py`

 * *Files identical despite different names*

### Comparing `crepex_pyutil-0.7.0/PKG-INFO` & `crepex_pyutil-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crepex-pyutil
-Version: 0.7.0
+Version: 0.8.0
 Summary: CrepeX python utilities
 Author: Hyunwoo Shim
 Author-email: hyunwoo.shim@crepe-x.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

