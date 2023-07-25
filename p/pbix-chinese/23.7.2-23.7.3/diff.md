# Comparing `tmp/pbix_chinese-23.7.2.tar.gz` & `tmp/pbix_chinese-23.7.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pbix_chinese-23.7.2.tar", last modified: Thu Jul 20 03:43:22 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

