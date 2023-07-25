# Comparing `tmp/orbax-0.1.7.tar.gz` & `tmp/orbax-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orbax-0.1.7.tar", last modified: Wed Mar 29 23:15:52 2023, max compression
+gzip compressed data, was "orbax-0.1.8.tar", last modified: Tue Jul 25 21:46:19 2023, max compression
```

## Comparing `orbax-0.1.7.tar` & `orbax-0.1.8.tar`

### file list

```diff
@@ -1,31 +1,10 @@
--rw-r--r--   0        0        0    11357 2023-03-29 23:15:13.613112 orbax-0.1.7/LICENSE
--rw-r--r--   0        0        0      752 2023-03-29 23:15:13.613112 orbax-0.1.7/README.md
--rw-r--r--   0        0        0      697 2023-03-29 23:15:13.613112 orbax-0.1.7/orbax/__init__.py
--rw-r--r--   0        0        0      137 2023-03-29 23:15:13.613112 orbax-0.1.7/orbax/checkpoint/README.md
--rw-r--r--   0        0        0     2462 2023-03-29 23:15:13.613112 orbax-0.1.7/orbax/checkpoint/__init__.py
--rw-r--r--   0        0        0     2599 2023-03-29 23:15:13.613112 orbax-0.1.7/orbax/checkpoint/abstract_checkpointer.py
--rw-r--r--   0        0        0     2629 2023-03-29 23:15:13.613112 orbax-0.1.7/orbax/checkpoint/aggregate_handlers.py
--rw-r--r--   0        0        0     5348 2023-03-29 23:15:13.613112 orbax-0.1.7/orbax/checkpoint/array_checkpoint_handler.py
--rw-r--r--   0        0        0     1440 2023-03-29 23:15:13.613112 orbax-0.1.7/orbax/checkpoint/async_checkpoint_handler.py
--rw-r--r--   0        0        0     4586 2023-03-29 23:15:13.613112 orbax-0.1.7/orbax/checkpoint/async_checkpointer.py
--rw-r--r--   0        0        0     2119 2023-03-29 23:15:13.613112 orbax-0.1.7/orbax/checkpoint/checkpoint_handler.py
--rw-r--r--   0        0        0    32820 2023-03-29 23:15:13.617112 orbax-0.1.7/orbax/checkpoint/checkpoint_manager.py
--rw-r--r--   0        0        0     9920 2023-03-29 23:15:13.617112 orbax-0.1.7/orbax/checkpoint/checkpoint_utils.py
--rw-r--r--   0        0        0     7190 2023-03-29 23:15:13.617112 orbax-0.1.7/orbax/checkpoint/checkpoint_utils_test.py
--rw-r--r--   0        0        0     3866 2023-03-29 23:15:13.617112 orbax-0.1.7/orbax/checkpoint/checkpointer.py
--rw-r--r--   0        0        0     1465 2023-03-29 23:15:13.617112 orbax-0.1.7/orbax/checkpoint/future.py
--rw-r--r--   0        0        0     2103 2023-03-29 23:15:13.617112 orbax-0.1.7/orbax/checkpoint/json_checkpoint_handler.py
--rw-r--r--   0        0        0     1821 2023-03-29 23:15:13.617112 orbax-0.1.7/orbax/checkpoint/json_checkpoint_handler_test.py
--rw-r--r--   0        0        0     1872 2023-03-29 23:15:13.617112 orbax-0.1.7/orbax/checkpoint/lazy_utils.py
--rw-r--r--   0        0        0     7146 2023-03-29 23:15:13.617112 orbax-0.1.7/orbax/checkpoint/msgpack_utils.py
--rw-r--r--   0        0        0    44672 2023-03-29 23:15:13.617112 orbax-0.1.7/orbax/checkpoint/orbax_checkpoint.ipynb
--rw-r--r--   0        0        0    18683 2023-03-29 23:15:13.617112 orbax-0.1.7/orbax/checkpoint/pytree_checkpoint_handler.py
--rw-r--r--   0        0        0     5234 2023-03-29 23:15:13.617112 orbax-0.1.7/orbax/checkpoint/test_utils.py
--rw-r--r--   0        0        0     8086 2023-03-29 23:15:13.617112 orbax-0.1.7/orbax/checkpoint/transform_utils.py
--rw-r--r--   0        0        0    13678 2023-03-29 23:15:13.617112 orbax-0.1.7/orbax/checkpoint/transform_utils_test.py
--rw-r--r--   0        0        0    19429 2023-03-29 23:15:13.617112 orbax-0.1.7/orbax/checkpoint/type_handlers.py
--rw-r--r--   0        0        0    19228 2023-03-29 23:15:13.617112 orbax-0.1.7/orbax/checkpoint/utils.py
--rw-r--r--   0        0        0     5925 2023-03-29 23:15:13.617112 orbax-0.1.7/orbax/checkpoint/utils_test.py
--rw-r--r--   0        0        0      740 2023-03-29 23:15:13.617112 orbax-0.1.7/orbax/conftest.py
--rw-r--r--   0        0        0     1077 2023-03-29 23:15:13.617112 orbax-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     1852 1970-01-01 00:00:00.000000 orbax-0.1.7/PKG-INFO
+drwxrwxr-x   0 ayh      (868580) primarygroup (89939)        0 2023-07-25 21:46:19.000000 orbax-0.1.8/
+-rw-rw-r--   0 ayh      (868580) primarygroup (89939)     1137 2023-07-25 21:46:19.000000 orbax-0.1.8/PKG-INFO
+-rw-rw-r--   0 ayh      (868580) primarygroup (89939)      919 2023-07-25 21:43:19.000000 orbax-0.1.8/README.md
+drwxrwxr-x   0 ayh      (868580) primarygroup (89939)        0 2023-07-25 21:46:19.000000 orbax-0.1.8/orbax.egg-info/
+-rw-rw-r--   0 ayh      (868580) primarygroup (89939)     1137 2023-07-25 21:46:19.000000 orbax-0.1.8/orbax.egg-info/PKG-INFO
+-rw-rw-r--   0 ayh      (868580) primarygroup (89939)      134 2023-07-25 21:46:19.000000 orbax-0.1.8/orbax.egg-info/SOURCES.txt
+-rw-rw-r--   0 ayh      (868580) primarygroup (89939)        1 2023-07-25 21:46:19.000000 orbax-0.1.8/orbax.egg-info/dependency_links.txt
+-rw-rw-r--   0 ayh      (868580) primarygroup (89939)        1 2023-07-25 21:46:19.000000 orbax-0.1.8/orbax.egg-info/top_level.txt
+-rw-rw-r--   0 ayh      (868580) primarygroup (89939)       38 2023-07-25 21:46:19.000000 orbax-0.1.8/setup.cfg
+-rw-rw-r--   0 ayh      (868580) primarygroup (89939)      970 2023-07-25 21:44:29.000000 orbax-0.1.8/setup.py
```

