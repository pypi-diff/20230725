# Comparing `tmp/gogo_cli-0.0.7.tar.gz` & `tmp/gogo_cli-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gogo_cli-0.0.7.tar", max compression
+gzip compressed data, was "gogo_cli-0.0.8.tar", max compression
```

## Comparing `gogo_cli-0.0.7.tar` & `gogo_cli-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    35149 2023-07-25 07:42:31.896162 gogo_cli-0.0.7/LICENSE
--rw-r--r--   0        0        0        0 2023-07-25 07:42:31.896162 gogo_cli-0.0.7/gogo_cli/__init__.py
--rw-r--r--   0        0        0      114 2023-07-25 07:42:31.896162 gogo_cli-0.0.7/gogo_cli/__main__.py
--rw-r--r--   0        0        0     2805 2023-07-25 07:42:31.896162 gogo_cli-0.0.7/gogo_cli/core/__gogo_cli__.py
--rw-r--r--   0        0        0        0 2023-07-25 07:42:31.896162 gogo_cli-0.0.7/gogo_cli/core/__init__.py
--rw-r--r--   0        0        0       19 2023-07-25 07:42:31.896162 gogo_cli-0.0.7/gogo_cli/core/__version__.py
--rw-r--r--   0        0        0      251 2023-07-25 07:42:31.896162 gogo_cli-0.0.7/gogo_cli/core/utils/__cast__.py
--rw-r--r--   0        0        0      743 2023-07-25 07:42:31.896162 gogo_cli-0.0.7/gogo_cli/core/utils/__downloader__.py
--rw-r--r--   0        0        0        0 2023-07-25 07:42:31.896162 gogo_cli-0.0.7/gogo_cli/core/utils/__init__.py
--rw-r--r--   0        0        0     1445 2023-07-25 07:42:31.896162 gogo_cli-0.0.7/gogo_cli/core/utils/__menu__.py
--rw-r--r--   0        0        0     1054 2023-07-25 07:42:31.896162 gogo_cli-0.0.7/gogo_cli/core/utils/__player__.py
--rw-r--r--   0        0        0      459 2023-07-25 07:42:31.896162 gogo_cli-0.0.7/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-25 07:42:31.896162 gogo_cli-0.0.7/readme.txt
--rw-r--r--   0        0        0      504 1970-01-01 00:00:00.000000 gogo_cli-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-25 08:13:22.520051 gogo_cli-0.0.8/LICENSE
+-rw-r--r--   0        0        0        0 2023-07-25 08:13:22.524051 gogo_cli-0.0.8/gogo_cli/__init__.py
+-rw-r--r--   0        0        0      114 2023-07-25 08:13:22.524051 gogo_cli-0.0.8/gogo_cli/__main__.py
+-rw-r--r--   0        0        0     2805 2023-07-25 08:13:22.524051 gogo_cli-0.0.8/gogo_cli/core/__gogo_cli__.py
+-rw-r--r--   0        0        0        0 2023-07-25 08:13:22.524051 gogo_cli-0.0.8/gogo_cli/core/__init__.py
+-rw-r--r--   0        0        0       19 2023-07-25 08:13:22.524051 gogo_cli-0.0.8/gogo_cli/core/__version__.py
+-rw-r--r--   0        0        0      251 2023-07-25 08:13:22.524051 gogo_cli-0.0.8/gogo_cli/core/utils/__cast__.py
+-rw-r--r--   0        0        0      743 2023-07-25 08:13:22.524051 gogo_cli-0.0.8/gogo_cli/core/utils/__downloader__.py
+-rw-r--r--   0        0        0        0 2023-07-25 08:13:22.524051 gogo_cli-0.0.8/gogo_cli/core/utils/__init__.py
+-rw-r--r--   0        0        0     1445 2023-07-25 08:13:22.524051 gogo_cli-0.0.8/gogo_cli/core/utils/__menu__.py
+-rw-r--r--   0        0        0     1547 2023-07-25 08:13:22.524051 gogo_cli-0.0.8/gogo_cli/core/utils/__player__.py
+-rw-r--r--   0        0        0      459 2023-07-25 08:13:22.524051 gogo_cli-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-25 08:13:22.524051 gogo_cli-0.0.8/readme.txt
+-rw-r--r--   0        0        0      504 1970-01-01 00:00:00.000000 gogo_cli-0.0.8/PKG-INFO
```

### Comparing `gogo_cli-0.0.7/LICENSE` & `gogo_cli-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `gogo_cli-0.0.7/gogo_cli/core/__gogo_cli__.py` & `gogo_cli-0.0.8/gogo_cli/core/__gogo_cli__.py`

 * *Files identical despite different names*

### Comparing `gogo_cli-0.0.7/gogo_cli/core/utils/__downloader__.py` & `gogo_cli-0.0.8/gogo_cli/core/utils/__downloader__.py`

 * *Files identical despite different names*

### Comparing `gogo_cli-0.0.7/gogo_cli/core/utils/__menu__.py` & `gogo_cli-0.0.8/gogo_cli/core/utils/__menu__.py`

 * *Files identical despite different names*

### Comparing `gogo_cli-0.0.7/gogo_cli/core/utils/__player__.py` & `gogo_cli-0.0.8/gogo_cli/core/utils/__player__.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,29 @@
 import subprocess
 
 MPV_EXECUTABLE = "mpv"
 IINA_EXECUTABLE = "iina"
 
 def play(url, referer, anime, episode):
     try:
-        if(platform.system() == "Linux" or platform.system() == "Windows"):
+
+        output = subprocess.check_output(["uname", "-o"])
+        output_str = output.decode("utf-8").strip()
+        if output_str == "Android":
+            args = [
+                "am start", 
+                "--user 0",
+                "-a android.intent.action.VIEW",
+                f"-d \"{url}\"",
+                "-n is.xyz.mpv/.MPVActivity",
+            ]
+            mpv_android_process = subprocess.Popen(args, stdout=subprocess.DEVNULL)
+            mpv_android_process.wait()
+
+        elif(platform.system() == "Linux" or platform.system() == "Windows"):
             args = [
                 MPV_EXECUTABLE,
                 url,
                 f"--referrer={referer}",
                 f"--force-media-title=Playing {anime} Episode {episode}",
             ]
```

