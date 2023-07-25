# Comparing `tmp/navi pro-7.1.9.tar.gz` & `tmp/navi_pro-7.2.4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/navi pro-7.1.9.tar", last modified: Mon Oct 17 18:16:44 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

