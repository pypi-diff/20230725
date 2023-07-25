# Comparing `tmp/nobuco-0.6.1.tar.gz` & `tmp/nobuco-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nobuco-0.6.1.tar", last modified: Mon Jul 24 13:34:25 2023, max compression
+gzip compressed data, was "nobuco-0.6.2.tar", last modified: Tue Jul 25 20:59:44 2023, max compression
```

## Comparing `nobuco-0.6.1.tar` & `nobuco-0.6.2.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-24 13:34:25.301624 nobuco-0.6.1/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2023-04-25 18:07:04.000000 nobuco-0.6.1/LICENSE
--rw-rw-r--   0 alex      (1000) alex      (1000)    24897 2023-07-24 13:34:25.301624 nobuco-0.6.1/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)    24311 2023-07-01 11:16:21.000000 nobuco-0.6.1/README.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-24 13:34:25.297624 nobuco-0.6.1/nobuco/
--rw-rw-r--   0 alex      (1000) alex      (1000)      533 2023-06-23 09:29:01.000000 nobuco-0.6.1/nobuco/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1270 2023-07-01 10:07:17.000000 nobuco-0.6.1/nobuco/commons.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)    13988 2023-07-20 10:12:52.000000 nobuco-0.6.1/nobuco/convert.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-24 13:34:25.297624 nobuco-0.6.1/nobuco/converters/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.6.1/nobuco/converters/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2397 2023-07-01 10:07:17.000000 nobuco-0.6.1/nobuco/converters/channel_ordering.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     1761 2023-07-01 10:07:17.000000 nobuco-0.6.1/nobuco/converters/node_converter.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2256 2023-06-19 20:03:57.000000 nobuco-0.6.1/nobuco/converters/tensor.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1358 2023-07-24 13:27:30.000000 nobuco-0.6.1/nobuco/converters/type_cast.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     4274 2023-07-24 13:14:20.000000 nobuco-0.6.1/nobuco/converters/validation.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-24 13:34:25.297624 nobuco-0.6.1/nobuco/entity/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.6.1/nobuco/entity/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      739 2023-04-25 18:07:04.000000 nobuco-0.6.1/nobuco/entity/keras.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    14874 2023-07-01 10:07:17.000000 nobuco-0.6.1/nobuco/entity/pytorch.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1316 2023-07-01 10:07:17.000000 nobuco-0.6.1/nobuco/funcs.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-24 13:34:25.301624 nobuco-0.6.1/nobuco/layers/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.6.1/nobuco/layers/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4419 2023-07-24 13:29:19.000000 nobuco-0.6.1/nobuco/layers/channel_order.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4524 2023-04-25 18:07:04.000000 nobuco-0.6.1/nobuco/layers/container.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      313 2023-04-25 18:07:04.000000 nobuco-0.6.1/nobuco/layers/stub.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1113 2023-07-20 18:19:12.000000 nobuco-0.6.1/nobuco/layers/weight.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-24 13:34:25.301624 nobuco-0.6.1/nobuco/locate/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.6.1/nobuco/locate/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      785 2023-04-25 18:07:04.000000 nobuco-0.6.1/nobuco/locate/link.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      599 2023-04-25 18:07:04.000000 nobuco-0.6.1/nobuco/locate/locate.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-24 13:34:25.301624 nobuco-0.6.1/nobuco/node_converters/
--rw-rw-r--   0 alex      (1000) alex      (1000)      210 2023-04-25 18:07:04.000000 nobuco-0.6.1/nobuco/node_converters/__init__.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     6967 2023-07-01 10:07:17.000000 nobuco-0.6.1/nobuco/node_converters/activation.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2225 2023-07-01 10:07:17.000000 nobuco-0.6.1/nobuco/node_converters/attention.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1169 2023-07-01 10:07:17.000000 nobuco-0.6.1/nobuco/node_converters/boolean.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     1165 2023-07-01 10:07:17.000000 nobuco-0.6.1/nobuco/node_converters/boolean_mask.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     3504 2023-07-01 10:07:17.000000 nobuco-0.6.1/nobuco/node_converters/comparison.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)    20101 2023-07-01 10:07:17.000000 nobuco-0.6.1/nobuco/node_converters/convolution.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)      754 2023-07-01 10:07:17.000000 nobuco-0.6.1/nobuco/node_converters/dropout.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1790 2023-07-01 10:07:17.000000 nobuco-0.6.1/nobuco/node_converters/interpolation.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     5152 2023-07-01 10:07:17.000000 nobuco-0.6.1/nobuco/node_converters/linear.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    16532 2023-07-24 13:27:30.000000 nobuco-0.6.1/nobuco/node_converters/math.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     1814 2023-07-01 10:07:17.000000 nobuco-0.6.1/nobuco/node_converters/misc.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     2213 2023-07-01 10:07:17.000000 nobuco-0.6.1/nobuco/node_converters/normalization.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1261 2023-07-01 10:07:17.000000 nobuco-0.6.1/nobuco/node_converters/padding.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     2934 2023-07-01 10:07:17.000000 nobuco-0.6.1/nobuco/node_converters/pooling.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     3332 2023-07-01 10:07:17.000000 nobuco-0.6.1/nobuco/node_converters/recurrent.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9538 2023-07-11 12:35:48.000000 nobuco-0.6.1/nobuco/node_converters/slice.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4029 2023-07-23 08:12:26.000000 nobuco-0.6.1/nobuco/node_converters/tensor_cast.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6726 2023-07-23 08:18:17.000000 nobuco-0.6.1/nobuco/node_converters/tensor_creation.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11559 2023-07-23 08:26:17.000000 nobuco-0.6.1/nobuco/node_converters/tensor_manipulation.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      369 2023-07-01 10:07:17.000000 nobuco-0.6.1/nobuco/node_converters/tensor_shape.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      452 2023-07-01 10:07:17.000000 nobuco-0.6.1/nobuco/node_converters/torchvision.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-24 13:34:25.301624 nobuco-0.6.1/nobuco/trace/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.6.1/nobuco/trace/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1378 2023-07-01 10:07:17.000000 nobuco-0.6.1/nobuco/trace/tensor_storage.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10069 2023-07-23 20:33:27.000000 nobuco-0.6.1/nobuco/trace/trace.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2776 2023-04-25 18:07:04.000000 nobuco-0.6.1/nobuco/util.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-24 13:34:25.301624 nobuco-0.6.1/nobuco/vis/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.6.1/nobuco/vis/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1934 2023-04-25 18:07:04.000000 nobuco-0.6.1/nobuco/vis/console_stylizer.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3158 2023-04-25 18:07:04.000000 nobuco-0.6.1/nobuco/vis/html_stylizer.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-24 13:34:25.297624 nobuco-0.6.1/nobuco.egg-info/
--rw-rw-r--   0 alex      (1000) alex      (1000)    24897 2023-07-24 13:34:25.000000 nobuco-0.6.1/nobuco.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     1702 2023-07-24 13:34:25.000000 nobuco-0.6.1/nobuco.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-07-24 13:34:25.000000 nobuco-0.6.1/nobuco.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       17 2023-07-24 13:34:25.000000 nobuco-0.6.1/nobuco.egg-info/requires.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        7 2023-07-24 13:34:25.000000 nobuco-0.6.1/nobuco.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)      735 2023-07-24 13:33:26.000000 nobuco-0.6.1/pyproject.toml
--rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-07-24 13:34:25.301624 nobuco-0.6.1/setup.cfg
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-25 20:59:44.343300 nobuco-0.6.2/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2023-04-25 18:07:04.000000 nobuco-0.6.2/LICENSE
+-rw-rw-r--   0 alex      (1000) alex      (1000)    24897 2023-07-25 20:59:44.343300 nobuco-0.6.2/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)    24311 2023-07-01 11:16:21.000000 nobuco-0.6.2/README.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-25 20:59:44.339300 nobuco-0.6.2/nobuco/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      581 2023-07-25 20:58:16.000000 nobuco-0.6.2/nobuco/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1270 2023-07-01 10:07:17.000000 nobuco-0.6.2/nobuco/commons.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)    13988 2023-07-20 10:12:52.000000 nobuco-0.6.2/nobuco/convert.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-25 20:59:44.339300 nobuco-0.6.2/nobuco/converters/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.6.2/nobuco/converters/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2397 2023-07-01 10:07:17.000000 nobuco-0.6.2/nobuco/converters/channel_ordering.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     1761 2023-07-25 20:57:18.000000 nobuco-0.6.2/nobuco/converters/node_converter.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2256 2023-06-19 20:03:57.000000 nobuco-0.6.2/nobuco/converters/tensor.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1358 2023-07-24 13:27:30.000000 nobuco-0.6.2/nobuco/converters/type_cast.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     4274 2023-07-24 13:14:20.000000 nobuco-0.6.2/nobuco/converters/validation.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-25 20:59:44.339300 nobuco-0.6.2/nobuco/entity/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.6.2/nobuco/entity/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      739 2023-04-25 18:07:04.000000 nobuco-0.6.2/nobuco/entity/keras.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    14874 2023-07-01 10:07:17.000000 nobuco-0.6.2/nobuco/entity/pytorch.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1316 2023-07-01 10:07:17.000000 nobuco-0.6.2/nobuco/funcs.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-25 20:59:44.339300 nobuco-0.6.2/nobuco/layers/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.6.2/nobuco/layers/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4419 2023-07-24 13:29:19.000000 nobuco-0.6.2/nobuco/layers/channel_order.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4524 2023-04-25 18:07:04.000000 nobuco-0.6.2/nobuco/layers/container.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      313 2023-04-25 18:07:04.000000 nobuco-0.6.2/nobuco/layers/stub.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1113 2023-07-20 18:19:12.000000 nobuco-0.6.2/nobuco/layers/weight.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-25 20:59:44.339300 nobuco-0.6.2/nobuco/locate/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.6.2/nobuco/locate/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      785 2023-04-25 18:07:04.000000 nobuco-0.6.2/nobuco/locate/link.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      599 2023-04-25 18:07:04.000000 nobuco-0.6.2/nobuco/locate/locate.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-25 20:59:44.343300 nobuco-0.6.2/nobuco/node_converters/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      210 2023-04-25 18:07:04.000000 nobuco-0.6.2/nobuco/node_converters/__init__.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     6967 2023-07-01 10:07:17.000000 nobuco-0.6.2/nobuco/node_converters/activation.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2225 2023-07-01 10:07:17.000000 nobuco-0.6.2/nobuco/node_converters/attention.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1169 2023-07-01 10:07:17.000000 nobuco-0.6.2/nobuco/node_converters/boolean.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     1165 2023-07-01 10:07:17.000000 nobuco-0.6.2/nobuco/node_converters/boolean_mask.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     3504 2023-07-01 10:07:17.000000 nobuco-0.6.2/nobuco/node_converters/comparison.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)    11813 2023-07-25 20:54:47.000000 nobuco-0.6.2/nobuco/node_converters/convolution.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)      754 2023-07-01 10:07:17.000000 nobuco-0.6.2/nobuco/node_converters/dropout.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1790 2023-07-01 10:07:17.000000 nobuco-0.6.2/nobuco/node_converters/interpolation.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     5152 2023-07-01 10:07:17.000000 nobuco-0.6.2/nobuco/node_converters/linear.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    16532 2023-07-24 13:27:30.000000 nobuco-0.6.2/nobuco/node_converters/math.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     1814 2023-07-01 10:07:17.000000 nobuco-0.6.2/nobuco/node_converters/misc.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     2213 2023-07-01 10:07:17.000000 nobuco-0.6.2/nobuco/node_converters/normalization.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1261 2023-07-01 10:07:17.000000 nobuco-0.6.2/nobuco/node_converters/padding.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     2934 2023-07-01 10:07:17.000000 nobuco-0.6.2/nobuco/node_converters/pooling.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     3332 2023-07-01 10:07:17.000000 nobuco-0.6.2/nobuco/node_converters/recurrent.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9538 2023-07-11 12:35:48.000000 nobuco-0.6.2/nobuco/node_converters/slice.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4029 2023-07-23 08:12:26.000000 nobuco-0.6.2/nobuco/node_converters/tensor_cast.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6726 2023-07-23 08:18:17.000000 nobuco-0.6.2/nobuco/node_converters/tensor_creation.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11559 2023-07-23 08:26:17.000000 nobuco-0.6.2/nobuco/node_converters/tensor_manipulation.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      369 2023-07-01 10:07:17.000000 nobuco-0.6.2/nobuco/node_converters/tensor_shape.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      452 2023-07-01 10:07:17.000000 nobuco-0.6.2/nobuco/node_converters/torchvision.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-25 20:59:44.343300 nobuco-0.6.2/nobuco/trace/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.6.2/nobuco/trace/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1378 2023-07-01 10:07:17.000000 nobuco-0.6.2/nobuco/trace/tensor_storage.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10069 2023-07-23 20:33:27.000000 nobuco-0.6.2/nobuco/trace/trace.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2776 2023-04-25 18:07:04.000000 nobuco-0.6.2/nobuco/util.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-25 20:59:44.343300 nobuco-0.6.2/nobuco/vis/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.6.2/nobuco/vis/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1934 2023-04-25 18:07:04.000000 nobuco-0.6.2/nobuco/vis/console_stylizer.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3158 2023-04-25 18:07:04.000000 nobuco-0.6.2/nobuco/vis/html_stylizer.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-25 20:59:44.339300 nobuco-0.6.2/nobuco.egg-info/
+-rw-rw-r--   0 alex      (1000) alex      (1000)    24897 2023-07-25 20:59:44.000000 nobuco-0.6.2/nobuco.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1702 2023-07-25 20:59:44.000000 nobuco-0.6.2/nobuco.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-07-25 20:59:44.000000 nobuco-0.6.2/nobuco.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       17 2023-07-25 20:59:44.000000 nobuco-0.6.2/nobuco.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        7 2023-07-25 20:59:44.000000 nobuco-0.6.2/nobuco.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)      735 2023-07-25 20:59:07.000000 nobuco-0.6.2/pyproject.toml
+-rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-07-25 20:59:44.343300 nobuco-0.6.2/setup.cfg
```

### Comparing `nobuco-0.6.1/LICENSE` & `nobuco-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.1/PKG-INFO` & `nobuco-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nobuco
-Version: 0.6.1
+Version: 0.6.2
 Summary: Pytorch to Tensorflow conversion made intuitive
 Author-email: Alexander Lutsenko <lex.lutsenko@gmail.com>
 Project-URL: Homepage, https://github.com/AlexanderLutsenko/nobuco
 Project-URL: Bug Tracker, https://github.com/AlexanderLutsenko/nobuco/issues
 Keywords: pytorch,tensorflow,keras,converter
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `nobuco-0.6.1/README.md` & `nobuco-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.1/nobuco/__init__.py` & `nobuco-0.6.2/nobuco/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from nobuco.funcs import force_tensorflow_order, force_pytorch_order, shape
 from nobuco.locate.locate import locate_converter
 from nobuco.trace.trace import traceable
 
-from nobuco.converters.node_converter import converter
+from nobuco.converters.node_converter import converter, unregister_converter
 from nobuco.convert import pytorch_to_keras
 from nobuco.commons import ChannelOrder, ChannelOrderingStrategy
 
 
 __all__ = [
     pytorch_to_keras,
     converter,
+    unregister_converter,
     traceable,
     ChannelOrder,
     ChannelOrderingStrategy,
     force_tensorflow_order,
     force_pytorch_order,
     shape,
     locate_converter
```

### Comparing `nobuco-0.6.1/nobuco/commons.py` & `nobuco-0.6.2/nobuco/commons.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.1/nobuco/convert.py` & `nobuco-0.6.2/nobuco/convert.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.1/nobuco/converters/channel_ordering.py` & `nobuco-0.6.2/nobuco/converters/channel_ordering.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.1/nobuco/converters/node_converter.py` & `nobuco-0.6.2/nobuco/converters/node_converter.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,11 +33,11 @@
         for op in ops:
             op = Tracer.op_unwrap(op)
             CONVERTER_DICT[op] = node_converter
         return node_converter
     return inner
 
 
-def converter_unregister(op):
+def unregister_converter(op):
     op = Tracer.op_unwrap(op)
     if op in CONVERTER_DICT:
         del CONVERTER_DICT[op]
```

### Comparing `nobuco-0.6.1/nobuco/converters/tensor.py` & `nobuco-0.6.2/nobuco/converters/tensor.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.1/nobuco/converters/type_cast.py` & `nobuco-0.6.2/nobuco/converters/type_cast.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.1/nobuco/converters/validation.py` & `nobuco-0.6.2/nobuco/converters/validation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.1/nobuco/entity/keras.py` & `nobuco-0.6.2/nobuco/entity/keras.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.1/nobuco/entity/pytorch.py` & `nobuco-0.6.2/nobuco/entity/pytorch.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.1/nobuco/funcs.py` & `nobuco-0.6.2/nobuco/funcs.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.1/nobuco/layers/channel_order.py` & `nobuco-0.6.2/nobuco/layers/channel_order.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.1/nobuco/layers/container.py` & `nobuco-0.6.2/nobuco/layers/container.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.1/nobuco/layers/weight.py` & `nobuco-0.6.2/nobuco/layers/weight.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.1/nobuco/locate/link.py` & `nobuco-0.6.2/nobuco/locate/link.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.1/nobuco/locate/locate.py` & `nobuco-0.6.2/nobuco/locate/locate.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.1/nobuco/node_converters/activation.py` & `nobuco-0.6.2/nobuco/node_converters/activation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.1/nobuco/node_converters/attention.py` & `nobuco-0.6.2/nobuco/node_converters/attention.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.1/nobuco/node_converters/boolean.py` & `nobuco-0.6.2/nobuco/node_converters/boolean.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.1/nobuco/node_converters/boolean_mask.py` & `nobuco-0.6.2/nobuco/node_converters/boolean_mask.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.1/nobuco/node_converters/comparison.py` & `nobuco-0.6.2/nobuco/node_converters/comparison.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.1/nobuco/node_converters/dropout.py` & `nobuco-0.6.2/nobuco/node_converters/dropout.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.1/nobuco/node_converters/interpolation.py` & `nobuco-0.6.2/nobuco/node_converters/interpolation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.1/nobuco/node_converters/linear.py` & `nobuco-0.6.2/nobuco/node_converters/linear.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.1/nobuco/node_converters/math.py` & `nobuco-0.6.2/nobuco/node_converters/math.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.1/nobuco/node_converters/misc.py` & `nobuco-0.6.2/nobuco/node_converters/misc.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.1/nobuco/node_converters/normalization.py` & `nobuco-0.6.2/nobuco/node_converters/normalization.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.1/nobuco/node_converters/padding.py` & `nobuco-0.6.2/nobuco/node_converters/padding.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.1/nobuco/node_converters/pooling.py` & `nobuco-0.6.2/nobuco/node_converters/pooling.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.1/nobuco/node_converters/recurrent.py` & `nobuco-0.6.2/nobuco/node_converters/recurrent.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.1/nobuco/node_converters/slice.py` & `nobuco-0.6.2/nobuco/node_converters/slice.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.1/nobuco/node_converters/tensor_cast.py` & `nobuco-0.6.2/nobuco/node_converters/tensor_cast.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.1/nobuco/node_converters/tensor_creation.py` & `nobuco-0.6.2/nobuco/node_converters/tensor_creation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.1/nobuco/node_converters/tensor_manipulation.py` & `nobuco-0.6.2/nobuco/node_converters/tensor_manipulation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.1/nobuco/trace/tensor_storage.py` & `nobuco-0.6.2/nobuco/trace/tensor_storage.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.1/nobuco/trace/trace.py` & `nobuco-0.6.2/nobuco/trace/trace.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.1/nobuco/util.py` & `nobuco-0.6.2/nobuco/util.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.1/nobuco/vis/console_stylizer.py` & `nobuco-0.6.2/nobuco/vis/console_stylizer.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.1/nobuco/vis/html_stylizer.py` & `nobuco-0.6.2/nobuco/vis/html_stylizer.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.1/nobuco.egg-info/PKG-INFO` & `nobuco-0.6.2/nobuco.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nobuco
-Version: 0.6.1
+Version: 0.6.2
 Summary: Pytorch to Tensorflow conversion made intuitive
 Author-email: Alexander Lutsenko <lex.lutsenko@gmail.com>
 Project-URL: Homepage, https://github.com/AlexanderLutsenko/nobuco
 Project-URL: Bug Tracker, https://github.com/AlexanderLutsenko/nobuco/issues
 Keywords: pytorch,tensorflow,keras,converter
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `nobuco-0.6.1/nobuco.egg-info/SOURCES.txt` & `nobuco-0.6.2/nobuco.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.1/pyproject.toml` & `nobuco-0.6.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nobuco"
-version = "0.6.1"
+version = "0.6.2"
 description = "Pytorch to Tensorflow conversion made intuitive"
 readme = "README.md"
 authors = [
   { name="Alexander Lutsenko", email="lex.lutsenko@gmail.com" },
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
```

