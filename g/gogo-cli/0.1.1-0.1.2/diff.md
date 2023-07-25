# Comparing `tmp/gogo_cli-0.1.1.tar.gz` & `tmp/gogo_cli-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gogo_cli-0.1.1.tar", max compression
+gzip compressed data, was "gogo_cli-0.1.2.tar", max compression
```

## Comparing `gogo_cli-0.1.1.tar` & `gogo_cli-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    35149 2023-07-25 08:23:31.347442 gogo_cli-0.1.1/LICENSE
--rw-r--r--   0        0        0        0 2023-07-25 08:23:31.347442 gogo_cli-0.1.1/gogo_cli/__init__.py
--rw-r--r--   0        0        0      114 2023-07-25 08:23:31.347442 gogo_cli-0.1.1/gogo_cli/__main__.py
--rw-r--r--   0        0        0     2805 2023-07-25 08:23:31.347442 gogo_cli-0.1.1/gogo_cli/core/__gogo_cli__.py
--rw-r--r--   0        0        0        0 2023-07-25 08:23:31.347442 gogo_cli-0.1.1/gogo_cli/core/__init__.py
--rw-r--r--   0        0        0       19 2023-07-25 08:23:31.347442 gogo_cli-0.1.1/gogo_cli/core/__version__.py
--rw-r--r--   0        0        0      251 2023-07-25 08:23:31.347442 gogo_cli-0.1.1/gogo_cli/core/utils/__cast__.py
--rw-r--r--   0        0        0      743 2023-07-25 08:23:31.347442 gogo_cli-0.1.1/gogo_cli/core/utils/__downloader__.py
--rw-r--r--   0        0        0        0 2023-07-25 08:23:31.347442 gogo_cli-0.1.1/gogo_cli/core/utils/__init__.py
--rw-r--r--   0        0        0     1445 2023-07-25 08:23:31.347442 gogo_cli-0.1.1/gogo_cli/core/utils/__menu__.py
--rw-r--r--   0        0        0     1658 2023-07-25 08:23:31.347442 gogo_cli-0.1.1/gogo_cli/core/utils/__player__.py
--rw-r--r--   0        0        0      459 2023-07-25 08:23:31.347442 gogo_cli-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-25 08:23:31.347442 gogo_cli-0.1.1/readme.txt
--rw-r--r--   0        0        0      504 1970-01-01 00:00:00.000000 gogo_cli-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-25 08:28:43.940696 gogo_cli-0.1.2/LICENSE
+-rw-r--r--   0        0        0        0 2023-07-25 08:28:43.940696 gogo_cli-0.1.2/gogo_cli/__init__.py
+-rw-r--r--   0        0        0      114 2023-07-25 08:28:43.940696 gogo_cli-0.1.2/gogo_cli/__main__.py
+-rw-r--r--   0        0        0     2805 2023-07-25 08:28:43.940696 gogo_cli-0.1.2/gogo_cli/core/__gogo_cli__.py
+-rw-r--r--   0        0        0        0 2023-07-25 08:28:43.940696 gogo_cli-0.1.2/gogo_cli/core/__init__.py
+-rw-r--r--   0        0        0       19 2023-07-25 08:28:43.940696 gogo_cli-0.1.2/gogo_cli/core/__version__.py
+-rw-r--r--   0        0        0      251 2023-07-25 08:28:43.940696 gogo_cli-0.1.2/gogo_cli/core/utils/__cast__.py
+-rw-r--r--   0        0        0      743 2023-07-25 08:28:43.940696 gogo_cli-0.1.2/gogo_cli/core/utils/__downloader__.py
+-rw-r--r--   0        0        0        0 2023-07-25 08:28:43.940696 gogo_cli-0.1.2/gogo_cli/core/utils/__init__.py
+-rw-r--r--   0        0        0     1445 2023-07-25 08:28:43.940696 gogo_cli-0.1.2/gogo_cli/core/utils/__menu__.py
+-rw-r--r--   0        0        0     1342 2023-07-25 08:28:43.940696 gogo_cli-0.1.2/gogo_cli/core/utils/__player__.py
+-rw-r--r--   0        0        0      459 2023-07-25 08:28:43.940696 gogo_cli-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-25 08:28:43.940696 gogo_cli-0.1.2/readme.txt
+-rw-r--r--   0        0        0      504 1970-01-01 00:00:00.000000 gogo_cli-0.1.2/PKG-INFO
```

### Comparing `gogo_cli-0.1.1/LICENSE` & `gogo_cli-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gogo_cli-0.1.1/gogo_cli/core/__gogo_cli__.py` & `gogo_cli-0.1.2/gogo_cli/core/__gogo_cli__.py`

 * *Files identical despite different names*

### Comparing `gogo_cli-0.1.1/gogo_cli/core/utils/__downloader__.py` & `gogo_cli-0.1.2/gogo_cli/core/utils/__downloader__.py`

 * *Files identical despite different names*

### Comparing `gogo_cli-0.1.1/gogo_cli/core/utils/__menu__.py` & `gogo_cli-0.1.2/gogo_cli/core/utils/__menu__.py`

 * *Files identical despite different names*

### Comparing `gogo_cli-0.1.1/gogo_cli/core/utils/__player__.py` & `gogo_cli-0.1.2/gogo_cli/core/utils/__player__.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,29 +6,15 @@
 
 def play(url, referer, anime, episode):
     try:
 
         output = subprocess.check_output(["uname", "-o"])
         output_str = output.decode("utf-8").strip()
         if output_str == "Android":
-            args = [
-                "nohup",
-                "am",
-                "start", 
-                "--user",
-                "0",
-                "-a",
-                "android.intent.action.VIEW",
-                "-d".
-                url,
-                "-n",
-                "is.xyz.mpv/.MPVActivity",
-            ]
-            mpv_android_process = subprocess.Popen(args, stdout=subprocess.DEVNULL)
-            mpv_android_process.wait()
+            subprocess.call(f"nohup am start --user 0 -a android.intent.action.VIEW -d \"{url}\" -n is.xyz.mpv/.MPVActivity", shell=True)
 
         elif(platform.system() == "Linux" or platform.system() == "Windows"):
             args = [
                 MPV_EXECUTABLE,
                 url,
                 f"--referrer={referer}",
                 f"--force-media-title=Playing {anime} Episode {episode}",
```

