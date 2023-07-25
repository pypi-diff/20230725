# Comparing `tmp/Hive_ML-1.0a0.tar.gz` & `tmp/Hive_ML-1.0a0.post1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Hive_ML-1.0a0.tar", last modified: Fri Jul 21 10:34:21 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

