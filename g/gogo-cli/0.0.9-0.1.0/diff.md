# Comparing `tmp/gogo_cli-0.0.9.tar.gz` & `tmp/gogo_cli-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gogo_cli-0.0.9.tar", max compression
+gzip compressed data, was "gogo_cli-0.1.0.tar", max compression
```

## Comparing `gogo_cli-0.0.9.tar` & `gogo_cli-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    35149 2023-07-25 08:17:52.678632 gogo_cli-0.0.9/LICENSE
--rw-r--r--   0        0        0        0 2023-07-25 08:17:52.678632 gogo_cli-0.0.9/gogo_cli/__init__.py
--rw-r--r--   0        0        0      114 2023-07-25 08:17:52.678632 gogo_cli-0.0.9/gogo_cli/__main__.py
--rw-r--r--   0        0        0     2805 2023-07-25 08:17:52.678632 gogo_cli-0.0.9/gogo_cli/core/__gogo_cli__.py
--rw-r--r--   0        0        0        0 2023-07-25 08:17:52.678632 gogo_cli-0.0.9/gogo_cli/core/__init__.py
--rw-r--r--   0        0        0       19 2023-07-25 08:17:52.678632 gogo_cli-0.0.9/gogo_cli/core/__version__.py
--rw-r--r--   0        0        0      251 2023-07-25 08:17:52.678632 gogo_cli-0.0.9/gogo_cli/core/utils/__cast__.py
--rw-r--r--   0        0        0      743 2023-07-25 08:17:52.678632 gogo_cli-0.0.9/gogo_cli/core/utils/__downloader__.py
--rw-r--r--   0        0        0        0 2023-07-25 08:17:52.678632 gogo_cli-0.0.9/gogo_cli/core/utils/__init__.py
--rw-r--r--   0        0        0     1445 2023-07-25 08:17:52.678632 gogo_cli-0.0.9/gogo_cli/core/utils/__menu__.py
--rw-r--r--   0        0        0     1667 2023-07-25 08:17:52.678632 gogo_cli-0.0.9/gogo_cli/core/utils/__player__.py
--rw-r--r--   0        0        0      459 2023-07-25 08:17:52.678632 gogo_cli-0.0.9/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-25 08:17:52.678632 gogo_cli-0.0.9/readme.txt
--rw-r--r--   0        0        0      504 1970-01-01 00:00:00.000000 gogo_cli-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-25 08:21:04.233283 gogo_cli-0.1.0/LICENSE
+-rw-r--r--   0        0        0        0 2023-07-25 08:21:04.233283 gogo_cli-0.1.0/gogo_cli/__init__.py
+-rw-r--r--   0        0        0      114 2023-07-25 08:21:04.233283 gogo_cli-0.1.0/gogo_cli/__main__.py
+-rw-r--r--   0        0        0     2805 2023-07-25 08:21:04.233283 gogo_cli-0.1.0/gogo_cli/core/__gogo_cli__.py
+-rw-r--r--   0        0        0        0 2023-07-25 08:21:04.233283 gogo_cli-0.1.0/gogo_cli/core/__init__.py
+-rw-r--r--   0        0        0       19 2023-07-25 08:21:04.233283 gogo_cli-0.1.0/gogo_cli/core/__version__.py
+-rw-r--r--   0        0        0      251 2023-07-25 08:21:04.233283 gogo_cli-0.1.0/gogo_cli/core/utils/__cast__.py
+-rw-r--r--   0        0        0      743 2023-07-25 08:21:04.233283 gogo_cli-0.1.0/gogo_cli/core/utils/__downloader__.py
+-rw-r--r--   0        0        0        0 2023-07-25 08:21:04.233283 gogo_cli-0.1.0/gogo_cli/core/utils/__init__.py
+-rw-r--r--   0        0        0     1445 2023-07-25 08:21:04.233283 gogo_cli-0.1.0/gogo_cli/core/utils/__menu__.py
+-rw-r--r--   0        0        0     1665 2023-07-25 08:21:04.233283 gogo_cli-0.1.0/gogo_cli/core/utils/__player__.py
+-rw-r--r--   0        0        0      459 2023-07-25 08:21:04.233283 gogo_cli-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-25 08:21:04.233283 gogo_cli-0.1.0/readme.txt
+-rw-r--r--   0        0        0      504 1970-01-01 00:00:00.000000 gogo_cli-0.1.0/PKG-INFO
```

### Comparing `gogo_cli-0.0.9/LICENSE` & `gogo_cli-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gogo_cli-0.0.9/gogo_cli/core/__gogo_cli__.py` & `gogo_cli-0.1.0/gogo_cli/core/__gogo_cli__.py`

 * *Files identical despite different names*

### Comparing `gogo_cli-0.0.9/gogo_cli/core/utils/__downloader__.py` & `gogo_cli-0.1.0/gogo_cli/core/utils/__downloader__.py`

 * *Files identical despite different names*

### Comparing `gogo_cli-0.0.9/gogo_cli/core/utils/__menu__.py` & `gogo_cli-0.1.0/gogo_cli/core/utils/__menu__.py`

 * *Files identical despite different names*

### Comparing `gogo_cli-0.0.9/gogo_cli/core/utils/__player__.py` & `gogo_cli-0.1.0/gogo_cli/core/utils/__player__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
                 "am",
                 "start", 
                 "--user",
                 "0",
                 "-a",
                 "android.intent.action.VIEW",
                 "-d".
-                f"\"{url}\"",
+                f'"{url}"',
                 "-n",
                 "is.xyz.mpv/.MPVActivity",
             ]
             mpv_android_process = subprocess.Popen(args, stdout=subprocess.DEVNULL)
             mpv_android_process.wait()
 
         elif(platform.system() == "Linux" or platform.system() == "Windows"):
```

