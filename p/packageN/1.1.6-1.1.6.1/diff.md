# Comparing `tmp/packageN-1.1.6.tar.gz` & `tmp/packageN-1.1.6.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "packageN-1.1.6.tar", last modified: Tue Jul 25 06:22:12 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

