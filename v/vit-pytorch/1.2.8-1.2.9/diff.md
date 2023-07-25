# Comparing `tmp/vit-pytorch-1.2.8.tar.gz` & `tmp/vit-pytorch-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vit-pytorch-1.2.8.tar", last modified: Mon Jul 24 21:31:06 2023, max compression
+gzip compressed data, was "vit-pytorch-1.2.9.tar", last modified: Tue Jul 25 17:39:30 2023, max compression
```

## Comparing `vit-pytorch-1.2.8.tar` & `vit-pytorch-1.2.9.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:31:06.749235 vit-pytorch-1.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-24 21:31:06.749235 vit-pytorch-1.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    62662 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 21:31:06.749235 vit-pytorch-1.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:31:06.741234 vit-pytorch-1.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/tests/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:31:06.745235 vit-pytorch-1.2.8/vit_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10258 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/ats_vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/cait.py
--rw-r--r--   0 runner    (1001) docker     (123)    12001 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/cct.py
--rw-r--r--   0 runner    (1001) docker     (123)    12186 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/cct_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     9194 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/cross_vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     8347 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/crossformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/cvt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/deepvit.py
--rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/dino.py
--rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/distill.py
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/efficient.py
--rw-r--r--   0 runner    (1001) docker     (123)    12657 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/es_vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/learnable_memory_vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     6474 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/levit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/local_vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/mae.py
--rw-r--r--   0 runner    (1001) docker     (123)     8305 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/max_vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     7897 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/mobile_vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/mp3.py
--rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/mpp.py
--rw-r--r--   0 runner    (1001) docker     (123)    10850 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/na_vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     6003 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/nest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/parallel_vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/pit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/recorder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9055 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/regionvit.py
--rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/rvt.py
--rw-r--r--   0 runner    (1001) docker     (123)     9690 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/scalable_vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     8998 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/sep_vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/simmim.py
--rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/simple_flash_attn_vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/simple_vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3715 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/simple_vit_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/simple_vit_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/simple_vit_with_patch_dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/t2t.py
--rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/twins_svt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/vit_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/vit_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/vit_for_small_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/vit_with_patch_dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/vit_with_patch_merger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-07-24 21:30:49.000000 vit-pytorch-1.2.8/vit_pytorch/vivit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:31:06.745235 vit-pytorch-1.2.8/vit_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-24 21:31:06.000000 vit-pytorch-1.2.8/vit_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-07-24 21:31:06.000000 vit-pytorch-1.2.8/vit_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 21:31:06.000000 vit-pytorch-1.2.8/vit_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 21:31:06.000000 vit-pytorch-1.2.8/vit_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-24 21:31:06.000000 vit-pytorch-1.2.8/vit_pytorch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:39:30.929937 vit-pytorch-1.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-25 17:39:16.000000 vit-pytorch-1.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-25 17:39:16.000000 vit-pytorch-1.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-25 17:39:30.929937 vit-pytorch-1.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    63066 2023-07-25 17:39:16.000000 vit-pytorch-1.2.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 17:39:30.929937 vit-pytorch-1.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-25 17:39:16.000000 vit-pytorch-1.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:39:30.925937 vit-pytorch-1.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-25 17:39:16.000000 vit-pytorch-1.2.9/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:39:30.929937 vit-pytorch-1.2.9/vit_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-25 17:39:16.000000 vit-pytorch-1.2.9/vit_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10258 2023-07-25 17:39:16.000000 vit-pytorch-1.2.9/vit_pytorch/ats_vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-07-25 17:39:16.000000 vit-pytorch-1.2.9/vit_pytorch/cait.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12001 2023-07-25 17:39:16.000000 vit-pytorch-1.2.9/vit_pytorch/cct.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12186 2023-07-25 17:39:16.000000 vit-pytorch-1.2.9/vit_pytorch/cct_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9194 2023-07-25 17:39:16.000000 vit-pytorch-1.2.9/vit_pytorch/cross_vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8347 2023-07-25 17:39:16.000000 vit-pytorch-1.2.9/vit_pytorch/crossformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-07-25 17:39:16.000000 vit-pytorch-1.2.9/vit_pytorch/cvt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-07-25 17:39:16.000000 vit-pytorch-1.2.9/vit_pytorch/deepvit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-07-25 17:39:16.000000 vit-pytorch-1.2.9/vit_pytorch/dino.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-07-25 17:39:16.000000 vit-pytorch-1.2.9/vit_pytorch/distill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-07-25 17:39:16.000000 vit-pytorch-1.2.9/vit_pytorch/efficient.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12657 2023-07-25 17:39:16.000000 vit-pytorch-1.2.9/vit_pytorch/es_vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-07-25 17:39:16.000000 vit-pytorch-1.2.9/vit_pytorch/extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-07-25 17:39:16.000000 vit-pytorch-1.2.9/vit_pytorch/learnable_memory_vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6474 2023-07-25 17:39:16.000000 vit-pytorch-1.2.9/vit_pytorch/levit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-07-25 17:39:16.000000 vit-pytorch-1.2.9/vit_pytorch/local_vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-07-25 17:39:16.000000 vit-pytorch-1.2.9/vit_pytorch/mae.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8305 2023-07-25 17:39:16.000000 vit-pytorch-1.2.9/vit_pytorch/max_vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7897 2023-07-25 17:39:16.000000 vit-pytorch-1.2.9/vit_pytorch/mobile_vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-07-25 17:39:16.000000 vit-pytorch-1.2.9/vit_pytorch/mp3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-07-25 17:39:16.000000 vit-pytorch-1.2.9/vit_pytorch/mpp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12364 2023-07-25 17:39:16.000000 vit-pytorch-1.2.9/vit_pytorch/na_vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6003 2023-07-25 17:39:16.000000 vit-pytorch-1.2.9/vit_pytorch/nest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-07-25 17:39:16.000000 vit-pytorch-1.2.9/vit_pytorch/parallel_vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-07-25 17:39:16.000000 vit-pytorch-1.2.9/vit_pytorch/pit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-07-25 17:39:16.000000 vit-pytorch-1.2.9/vit_pytorch/recorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9055 2023-07-25 17:39:16.000000 vit-pytorch-1.2.9/vit_pytorch/regionvit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-07-25 17:39:16.000000 vit-pytorch-1.2.9/vit_pytorch/rvt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9690 2023-07-25 17:39:16.000000 vit-pytorch-1.2.9/vit_pytorch/scalable_vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8998 2023-07-25 17:39:16.000000 vit-pytorch-1.2.9/vit_pytorch/sep_vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-07-25 17:39:16.000000 vit-pytorch-1.2.9/vit_pytorch/simmim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-07-25 17:39:16.000000 vit-pytorch-1.2.9/vit_pytorch/simple_flash_attn_vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-07-25 17:39:16.000000 vit-pytorch-1.2.9/vit_pytorch/simple_vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3715 2023-07-25 17:39:16.000000 vit-pytorch-1.2.9/vit_pytorch/simple_vit_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-07-25 17:39:16.000000 vit-pytorch-1.2.9/vit_pytorch/simple_vit_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-07-25 17:39:16.000000 vit-pytorch-1.2.9/vit_pytorch/simple_vit_with_patch_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-07-25 17:39:16.000000 vit-pytorch-1.2.9/vit_pytorch/t2t.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-07-25 17:39:16.000000 vit-pytorch-1.2.9/vit_pytorch/twins_svt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-07-25 17:39:16.000000 vit-pytorch-1.2.9/vit_pytorch/vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-07-25 17:39:16.000000 vit-pytorch-1.2.9/vit_pytorch/vit_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-07-25 17:39:16.000000 vit-pytorch-1.2.9/vit_pytorch/vit_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-07-25 17:39:16.000000 vit-pytorch-1.2.9/vit_pytorch/vit_for_small_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-07-25 17:39:16.000000 vit-pytorch-1.2.9/vit_pytorch/vit_with_patch_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-07-25 17:39:16.000000 vit-pytorch-1.2.9/vit_pytorch/vit_with_patch_merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-07-25 17:39:16.000000 vit-pytorch-1.2.9/vit_pytorch/vivit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:39:30.929937 vit-pytorch-1.2.9/vit_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-25 17:39:30.000000 vit-pytorch-1.2.9/vit_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-07-25 17:39:30.000000 vit-pytorch-1.2.9/vit_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 17:39:30.000000 vit-pytorch-1.2.9/vit_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 17:39:30.000000 vit-pytorch-1.2.9/vit_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-25 17:39:30.000000 vit-pytorch-1.2.9/vit_pytorch.egg-info/top_level.txt
```

### Comparing `vit-pytorch-1.2.8/LICENSE` & `vit-pytorch-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.8/PKG-INFO` & `vit-pytorch-1.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vit-pytorch
-Version: 1.2.8
+Version: 1.2.9
 Summary: Vision Transformer (ViT) - Pytorch
 Home-page: https://github.com/lucidrains/vit-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,image recognition
 Classifier: Development Status :: 4 - Beta
```

### Comparing `vit-pytorch-1.2.8/README.md` & `vit-pytorch-1.2.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -175,14 +175,32 @@
     [torch.randn(3, 64, 256)]
 ]
 
 preds = v(images) # (5, 1000) - 5, because 5 images of different resolution above
 
 ```
 
+Or if you would rather that the framework auto group the images into variable lengthed sequences that do not exceed a certain max length
+
+```python
+images = [
+    torch.randn(3, 256, 256),
+    torch.randn(3, 128, 128),
+    torch.randn(3, 128, 256),
+    torch.randn(3, 256, 128),
+    torch.randn(3, 64, 256)
+]
+
+preds = v(
+    images,
+    group_images = True,
+    group_max_seq_len = 64
+) # (5, 1000)
+```
+
 ## Distillation
 
 <img src="./images/distill.png" width="300px"></img>
 
 A recent <a href="https://arxiv.org/abs/2012.12877">paper</a> has shown that use of a distillation token for distilling knowledge from convolutional nets to vision transformer can yield small and efficient vision transformers. This repository offers the means to do distillation easily.
 
 ex. distilling from Resnet50 (or any teacher) to a vision transformer
```

#### html2text {}

```diff
@@ -63,21 +63,26 @@
 = 2048, dropout = 0.1, emb_dropout = 0.1, token_dropout_prob = 0.1 # token
 dropout of 10% (keep 90% of tokens) ) # 5 images of different resolutions -
 List[List[Tensor]] # for now, you'll have to correctly place images in same
 batch element as to not exceed maximum allowed sequence length for self-
 attention w/ masking images = [ [torch.randn(3, 256, 256), torch.randn(3, 128,
 128)], [torch.randn(3, 128, 256), torch.randn(3, 256, 128)], [torch.randn(3,
 64, 256)] ] preds = v(images) # (5, 1000) - 5, because 5 images of different
-resolution above ``` ## Distillation [./images/distill.png] A recent paper has
-shown that use of a distillation token for distilling knowledge from
-convolutional nets to vision transformer can yield small and efficient vision
-transformers. This repository offers the means to do distillation easily. ex.
-distilling from Resnet50 (or any teacher) to a vision transformer ```python
-import torch from torchvision.models import resnet50 from vit_pytorch.distill
-import DistillableViT, DistillWrapper teacher = resnet50(pretrained = True) v =
+resolution above ``` Or if you would rather that the framework auto group the
+images into variable lengthed sequences that do not exceed a certain max length
+```python images = [ torch.randn(3, 256, 256), torch.randn(3, 128, 128),
+torch.randn(3, 128, 256), torch.randn(3, 256, 128), torch.randn(3, 64, 256) ]
+preds = v( images, group_images = True, group_max_seq_len = 64 ) # (5, 1000)
+``` ## Distillation [./images/distill.png] A recent paper has shown that use of
+a distillation token for distilling knowledge from convolutional nets to vision
+transformer can yield small and efficient vision transformers. This repository
+offers the means to do distillation easily. ex. distilling from Resnet50 (or
+any teacher) to a vision transformer ```python import torch from
+torchvision.models import resnet50 from vit_pytorch.distill import
+DistillableViT, DistillWrapper teacher = resnet50(pretrained = True) v =
 DistillableViT( image_size = 256, patch_size = 32, num_classes = 1000, dim =
 1024, depth = 6, heads = 8, mlp_dim = 2048, dropout = 0.1, emb_dropout = 0.1 )
 distiller = DistillWrapper( student = v, teacher = teacher, temperature = 3, #
 temperature of distillation alpha = 0.5, # trade between main loss and
 distillation loss hard = False # whether to use soft or hard distillation ) img
 = torch.randn(2, 3, 256, 256) labels = torch.randint(0, 1000, (2,)) loss =
 distiller(img, labels) loss.backward() # after lots of training above ... pred
```

### Comparing `vit-pytorch-1.2.8/setup.py` & `vit-pytorch-1.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'vit-pytorch',
   packages = find_packages(exclude=['examples']),
-  version = '1.2.8',
+  version = '1.2.9',
   license='MIT',
   description = 'Vision Transformer (ViT) - Pytorch',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/vit-pytorch',
   keywords = [
```

### Comparing `vit-pytorch-1.2.8/vit_pytorch/ats_vit.py` & `vit-pytorch-1.2.9/vit_pytorch/ats_vit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.8/vit_pytorch/cait.py` & `vit-pytorch-1.2.9/vit_pytorch/cait.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.8/vit_pytorch/cct.py` & `vit-pytorch-1.2.9/vit_pytorch/cct.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.8/vit_pytorch/cct_3d.py` & `vit-pytorch-1.2.9/vit_pytorch/cct_3d.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.8/vit_pytorch/cross_vit.py` & `vit-pytorch-1.2.9/vit_pytorch/cross_vit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.8/vit_pytorch/crossformer.py` & `vit-pytorch-1.2.9/vit_pytorch/crossformer.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.8/vit_pytorch/cvt.py` & `vit-pytorch-1.2.9/vit_pytorch/cvt.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.8/vit_pytorch/deepvit.py` & `vit-pytorch-1.2.9/vit_pytorch/deepvit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.8/vit_pytorch/dino.py` & `vit-pytorch-1.2.9/vit_pytorch/dino.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.8/vit_pytorch/distill.py` & `vit-pytorch-1.2.9/vit_pytorch/distill.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.8/vit_pytorch/efficient.py` & `vit-pytorch-1.2.9/vit_pytorch/efficient.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.8/vit_pytorch/es_vit.py` & `vit-pytorch-1.2.9/vit_pytorch/es_vit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.8/vit_pytorch/extractor.py` & `vit-pytorch-1.2.9/vit_pytorch/extractor.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.8/vit_pytorch/learnable_memory_vit.py` & `vit-pytorch-1.2.9/vit_pytorch/learnable_memory_vit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.8/vit_pytorch/levit.py` & `vit-pytorch-1.2.9/vit_pytorch/levit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.8/vit_pytorch/local_vit.py` & `vit-pytorch-1.2.9/vit_pytorch/local_vit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.8/vit_pytorch/mae.py` & `vit-pytorch-1.2.9/vit_pytorch/mae.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.8/vit_pytorch/max_vit.py` & `vit-pytorch-1.2.9/vit_pytorch/max_vit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.8/vit_pytorch/mobile_vit.py` & `vit-pytorch-1.2.9/vit_pytorch/mobile_vit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.8/vit_pytorch/mp3.py` & `vit-pytorch-1.2.9/vit_pytorch/mp3.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.8/vit_pytorch/mpp.py` & `vit-pytorch-1.2.9/vit_pytorch/mpp.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.8/vit_pytorch/na_vit.py` & `vit-pytorch-1.2.9/vit_pytorch/na_vit.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from functools import partial
-from typing import List
+from typing import List, Union
 
 import torch
 import torch.nn.functional as F
 from torch import nn, Tensor
 from torch.nn.utils.rnn import pad_sequence as orig_pad_sequence
 
 from einops import rearrange, repeat
@@ -13,20 +13,66 @@
 
 def exists(val):
     return val is not None
 
 def default(val, d):
     return val if exists(val) else d
 
+def always(val):
+    return lambda *args: val
+
 def pair(t):
     return t if isinstance(t, tuple) else (t, t)
 
 def divisible_by(numer, denom):
     return (numer % denom) == 0
 
+# auto grouping images
+
+def group_images_by_max_seq_len(
+    images: List[Tensor],
+    patch_size: int,
+    calc_token_dropout = None,
+    max_seq_len = 2048
+
+) -> List[List[Tensor]]:
+
+    calc_token_dropout = default(calc_token_dropout, always(0.))
+
+    groups = []
+    group = []
+    seq_len = 0
+
+    if isinstance(calc_token_dropout, (float, int)):
+        calc_token_dropout = always(calc_token_dropout)
+
+    for image in images:
+        assert isinstance(image, Tensor)
+
+        image_dims = image.shape[-2:]
+        ph, pw = map(lambda t: t // patch_size, image_dims)
+
+        image_seq_len = (ph * pw)
+        image_seq_len = int(image_seq_len * (1 - calc_token_dropout(*image_dims)))
+
+        assert image_seq_len <= max_seq_len, f'image with dimensions {image_dims} exceeds maximum sequence length'
+
+        if (seq_len + image_seq_len) > max_seq_len:
+            groups.append(group)
+            group = []
+            seq_len = 0
+
+        group.append(image)
+        seq_len += image_seq_len
+
+    if len(group) > 0:
+        groups.append(group)
+
+    return groups
+
 # normalization
 # they use layernorm without bias, something that pytorch does not offer
 
 class LayerNorm(nn.Module):
     def __init__(self, dim):
         super().__init__()
         self.gamma = nn.Parameter(torch.ones(dim))
@@ -142,15 +188,15 @@
         super().__init__()
         image_height, image_width = pair(image_size)
 
         # what percent of tokens to dropout
         # if int or float given, then assume constant dropout prob
         # otherwise accept a callback that in turn calculates dropout prob from height and width
 
-        self.calc_token_dropout = calc_token_dropout = None
+        self.calc_token_dropout = None
 
         if callable(token_dropout_prob):
             self.calc_token_dropout = token_dropout_prob
 
         elif isinstance(token_dropout_prob, (float, int)):
             assert 0. < token_dropout_prob < 1.
             token_dropout_prob = float(token_dropout_prob)
@@ -195,21 +241,33 @@
 
     @property
     def device(self):
         return next(self.parameters()).device
 
     def forward(
         self,
-        batched_images: List[List[Tensor]] # assume different resolution images already grouped correctly
+        batched_images: Union[List[Tensor], List[List[Tensor]]], # assume different resolution images already grouped correctly
+        group_images = False,
+        group_max_seq_len = 2048
     ):
         p, c, device, has_token_dropout = self.patch_size, self.channels, self.device, exists(self.calc_token_dropout)
 
         arange = partial(torch.arange, device = device)
         pad_sequence = partial(orig_pad_sequence, batch_first = True)
 
+        # auto pack if specified
+
+        if group_images:
+            batched_images = group_images_by_max_seq_len(
+                batched_images,
+                patch_size = self.patch_size,
+                calc_token_dropout = self.calc_token_dropout,
+                max_seq_len = group_max_seq_len
+            )
+
         # process images into variable lengthed sequences with attention mask
 
         num_images = []
         batched_sequences = []
         batched_positions = []
         batched_image_ids = []
```

### Comparing `vit-pytorch-1.2.8/vit_pytorch/nest.py` & `vit-pytorch-1.2.9/vit_pytorch/nest.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.8/vit_pytorch/parallel_vit.py` & `vit-pytorch-1.2.9/vit_pytorch/parallel_vit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.8/vit_pytorch/pit.py` & `vit-pytorch-1.2.9/vit_pytorch/pit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.8/vit_pytorch/recorder.py` & `vit-pytorch-1.2.9/vit_pytorch/recorder.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.8/vit_pytorch/regionvit.py` & `vit-pytorch-1.2.9/vit_pytorch/regionvit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.8/vit_pytorch/rvt.py` & `vit-pytorch-1.2.9/vit_pytorch/rvt.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.8/vit_pytorch/scalable_vit.py` & `vit-pytorch-1.2.9/vit_pytorch/scalable_vit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.8/vit_pytorch/sep_vit.py` & `vit-pytorch-1.2.9/vit_pytorch/sep_vit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.8/vit_pytorch/simmim.py` & `vit-pytorch-1.2.9/vit_pytorch/simmim.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.8/vit_pytorch/simple_flash_attn_vit.py` & `vit-pytorch-1.2.9/vit_pytorch/simple_flash_attn_vit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.8/vit_pytorch/simple_vit.py` & `vit-pytorch-1.2.9/vit_pytorch/simple_vit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.8/vit_pytorch/simple_vit_1d.py` & `vit-pytorch-1.2.9/vit_pytorch/simple_vit_1d.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.8/vit_pytorch/simple_vit_3d.py` & `vit-pytorch-1.2.9/vit_pytorch/simple_vit_3d.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.8/vit_pytorch/simple_vit_with_patch_dropout.py` & `vit-pytorch-1.2.9/vit_pytorch/simple_vit_with_patch_dropout.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.8/vit_pytorch/t2t.py` & `vit-pytorch-1.2.9/vit_pytorch/t2t.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.8/vit_pytorch/twins_svt.py` & `vit-pytorch-1.2.9/vit_pytorch/twins_svt.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.8/vit_pytorch/vit.py` & `vit-pytorch-1.2.9/vit_pytorch/vit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.8/vit_pytorch/vit_1d.py` & `vit-pytorch-1.2.9/vit_pytorch/vit_1d.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.8/vit_pytorch/vit_3d.py` & `vit-pytorch-1.2.9/vit_pytorch/vit_3d.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.8/vit_pytorch/vit_for_small_dataset.py` & `vit-pytorch-1.2.9/vit_pytorch/vit_for_small_dataset.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.8/vit_pytorch/vit_with_patch_dropout.py` & `vit-pytorch-1.2.9/vit_pytorch/vit_with_patch_dropout.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.8/vit_pytorch/vit_with_patch_merger.py` & `vit-pytorch-1.2.9/vit_pytorch/vit_with_patch_merger.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.8/vit_pytorch/vivit.py` & `vit-pytorch-1.2.9/vit_pytorch/vivit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.2.8/vit_pytorch.egg-info/PKG-INFO` & `vit-pytorch-1.2.9/vit_pytorch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vit-pytorch
-Version: 1.2.8
+Version: 1.2.9
 Summary: Vision Transformer (ViT) - Pytorch
 Home-page: https://github.com/lucidrains/vit-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,image recognition
 Classifier: Development Status :: 4 - Beta
```

### Comparing `vit-pytorch-1.2.8/vit_pytorch.egg-info/SOURCES.txt` & `vit-pytorch-1.2.9/vit_pytorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

