# Comparing `tmp/pkgNipun-1.1.0.tar.gz` & `tmp/pkgNipun-1.1.6.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkgNipun-1.1.0.tar", last modified: Tue Jul 18 15:58:46 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

