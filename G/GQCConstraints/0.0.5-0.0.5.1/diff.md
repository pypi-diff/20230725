# Comparing `tmp/GQCConstraints-0.0.5.tar.gz` & `tmp/GQCConstraints-0.0.5.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GQCConstraints-0.0.5.tar", last modified: Tue Jul 25 12:40:25 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

