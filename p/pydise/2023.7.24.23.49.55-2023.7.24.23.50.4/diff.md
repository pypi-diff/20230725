# Comparing `tmp/pydise-2023.7.24.23.49.55.tar.gz` & `tmp/pydise-2023.7.24.23.50.4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydise-2023.7.24.23.49.55.tar", last modified: Mon Jul 24 23:49:55 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

