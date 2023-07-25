# Comparing `tmp/modelwhaleutils-0.5.2.0.tar.gz` & `tmp/modelwhaleutils-0.5.2.1-py3.7.egg`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/modelwhaleutils-0.5.2.0.tar", last modified: Mon Jul 10 04:04:37 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

