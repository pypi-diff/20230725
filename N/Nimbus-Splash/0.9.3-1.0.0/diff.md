# Comparing `tmp/Nimbus Splash-0.9.3.tar.gz` & `tmp/Nimbus_Splash-1.0.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Nimbus Splash-0.9.3.tar", last modified: Mon Mar 20 12:05:04 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

