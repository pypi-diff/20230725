# Comparing `tmp/ryo-iso-0.1.6.tar.gz` & `tmp/ryo_iso-0.1.7-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ryo-iso-0.1.6.tar", last modified: Sat Nov 19 03:09:06 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

