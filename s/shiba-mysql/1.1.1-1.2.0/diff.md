# Comparing `tmp/shiba_mysql-1.1.1.tar.gz` & `tmp/shiba_mysql-1.2.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shiba_mysql-1.1.1.tar", last modified: Sun Jul 16 01:31:00 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

