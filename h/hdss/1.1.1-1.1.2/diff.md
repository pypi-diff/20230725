# Comparing `tmp/hdss-1.1.1.tar.gz` & `tmp/hdss-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hdss-1.1.1.tar", max compression
+gzip compressed data, was "hdss-1.1.2.tar", max compression
```

## Comparing `hdss-1.1.1.tar` & `hdss-1.1.2.tar`

### file list

```diff
@@ -1,6 +1,14 @@
--rw-r--r--   0        0        0      718 2022-07-05 12:54:13.781427 hdss-1.1.1/README.md
--rw-r--r--   0        0        0     6148 2023-07-06 10:37:54.977432 hdss-1.1.1/hdss/.DS_Store
--rw-r--r--   0        0        0       48 2022-06-25 08:10:40.407522 hdss-1.1.1/hdss/__init__.py
--rw-r--r--   0        0        0     8559 2023-07-06 09:49:51.021515 hdss-1.1.1/hdss/code.py
--rw-r--r--   0        0        0      363 2023-07-06 10:43:24.726448 hdss-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     1322 1970-01-01 00:00:00.000000 hdss-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0      718 2022-07-05 12:54:13.781427 hdss-1.1.2/README.md
+-rw-r--r--   0        0        0     6148 2023-07-25 20:14:08.078317 hdss-1.1.2/hdss/.DS_Store
+-rw-r--r--   0        0        0      112 2023-07-25 15:45:17.944019 hdss-1.1.2/hdss/__init__.py
+-rw-r--r--   0        0        0     6148 2023-07-25 20:08:11.422470 hdss-1.1.2/hdss/src/.DS_Store
+-rw-r--r--   0        0        0      655 2023-07-25 20:06:56.997145 hdss-1.1.2/hdss/src/bezier_image.py
+-rw-r--r--   0        0        0     1578 2023-07-25 20:06:56.969142 hdss-1.1.2/hdss/src/bezier_utils.py
+-rw-r--r--   0        0        0     2479 2023-07-25 20:06:56.988154 hdss-1.1.2/hdss/src/create_shapes.py
+-rw-r--r--   0        0        0      523 2023-07-25 20:06:56.965520 hdss-1.1.2/hdss/src/glbl.py
+-rw-r--r--   0        0        0      428 2023-07-25 20:06:57.000198 hdss-1.1.2/hdss/src/set_params.py
+-rw-r--r--   0        0        0     4469 2023-07-25 20:06:57.010021 hdss-1.1.2/hdss/src/set_persp_transform.py
+-rw-r--r--   0        0        0      172 2023-07-25 20:06:56.993205 hdss-1.1.2/hdss/src/set_random_noise.py
+-rw-r--r--   0        0        0      389 2023-07-25 20:06:57.006518 hdss-1.1.2/hdss/src/utils.py
+-rw-r--r--   0        0        0      364 2023-07-25 20:24:06.846388 hdss-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1223 1970-01-01 00:00:00.000000 hdss-1.1.2/PKG-INFO
```

### Comparing `hdss-1.1.1/README.md` & `hdss-1.1.2/README.md`

 * *Files identical despite different names*

