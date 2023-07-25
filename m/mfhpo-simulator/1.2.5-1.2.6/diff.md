# Comparing `tmp/mfhpo_simulator-1.2.5-py3-none-any.whl.zip` & `tmp/mfhpo_simulator-1.2.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,21 @@
-Zip file size: 30249 bytes, number of entries: 15
--rw-rw-r--  2.0 unx      560 b- defN 23-Jul-25 08:25 benchmark_simulator/__init__.py
+Zip file size: 35324 bytes, number of entries: 19
+-rw-rw-r--  2.0 unx      560 b- defN 23-Jul-25 08:31 benchmark_simulator/__init__.py
 -rw-rw-r--  2.0 unx     7761 b- defN 23-Jul-19 11:36 benchmark_simulator/_constants.py
 -rw-rw-r--  2.0 unx    12622 b- defN 23-Jul-19 07:25 benchmark_simulator/_secure_proc.py
 -rw-rw-r--  2.0 unx     5116 b- defN 23-Jul-06 23:36 benchmark_simulator/_utils.py
 -rw-rw-r--  2.0 unx    28910 b- defN 23-Jul-19 11:36 benchmark_simulator/simulator.py
 -rw-rw-r--  2.0 unx     2582 b- defN 23-Jul-06 18:41 benchmark_simulator/_simulator/_base_wrapper.py
 -rw-rw-r--  2.0 unx     3335 b- defN 23-Jul-19 11:36 benchmark_simulator/_simulator/_utils.py
 -rw-rw-r--  2.0 unx    13196 b- defN 23-Jul-19 11:36 benchmark_simulator/_simulator/_worker.py
 -rw-rw-r--  2.0 unx     3767 b- defN 23-Jul-18 21:06 benchmark_simulator/_simulator/_worker_manager.py
 -rw-rw-r--  2.0 unx     9134 b- defN 23-Jul-18 21:22 benchmark_simulator/_simulator/_worker_manager_for_ask_and_tell.py
--rw-rw-r--  2.0 unx    10760 b- defN 23-Jul-25 08:25 mfhpo_simulator-1.2.5.dist-info/LICENSE
--rw-rw-r--  2.0 unx      307 b- defN 23-Jul-25 08:25 mfhpo_simulator-1.2.5.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-25 08:25 mfhpo_simulator-1.2.5.dist-info/WHEEL
--rw-rw-r--  2.0 unx       51 b- defN 23-Jul-25 08:25 mfhpo_simulator-1.2.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1401 b- defN 23-Jul-25 08:25 mfhpo_simulator-1.2.5.dist-info/RECORD
-15 files, 99594 bytes uncompressed, 27883 bytes compressed:  72.0%
+-rw-rw-r--  2.0 unx     2181 b- defN 23-Jul-06 18:55 benchmark_simulator/_trackers/_config_tracker.py
+-rw-rw-r--  2.0 unx     5012 b- defN 23-Jul-06 23:14 benchmark_simulator/_trackers/_state_tracker.py
+-rw-rw-r--  2.0 unx      284 b- defN 23-Jul-10 08:56 benchmark_simulator/utils/__init__.py
+-rw-rw-r--  2.0 unx     8990 b- defN 23-Jul-11 10:13 benchmark_simulator/utils/_performance_over_time.py
+-rw-rw-r--  2.0 unx    10760 b- defN 23-Jul-25 08:32 mfhpo_simulator-1.2.6.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      307 b- defN 23-Jul-25 08:32 mfhpo_simulator-1.2.6.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-25 08:32 mfhpo_simulator-1.2.6.dist-info/WHEEL
+-rw-rw-r--  2.0 unx      107 b- defN 23-Jul-25 08:32 mfhpo_simulator-1.2.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1812 b- defN 23-Jul-25 08:32 mfhpo_simulator-1.2.6.dist-info/RECORD
+19 files, 116528 bytes uncompressed, 32288 bytes compressed:  72.3%
```

## zipnote {}

```diff
@@ -24,23 +24,35 @@
 
 Filename: benchmark_simulator/_simulator/_worker_manager.py
 Comment: 
 
 Filename: benchmark_simulator/_simulator/_worker_manager_for_ask_and_tell.py
 Comment: 
 
-Filename: mfhpo_simulator-1.2.5.dist-info/LICENSE
+Filename: benchmark_simulator/_trackers/_config_tracker.py
 Comment: 
 
-Filename: mfhpo_simulator-1.2.5.dist-info/METADATA
+Filename: benchmark_simulator/_trackers/_state_tracker.py
 Comment: 
 
-Filename: mfhpo_simulator-1.2.5.dist-info/WHEEL
+Filename: benchmark_simulator/utils/__init__.py
 Comment: 
 
-Filename: mfhpo_simulator-1.2.5.dist-info/top_level.txt
+Filename: benchmark_simulator/utils/_performance_over_time.py
 Comment: 
 
-Filename: mfhpo_simulator-1.2.5.dist-info/RECORD
+Filename: mfhpo_simulator-1.2.6.dist-info/LICENSE
+Comment: 
+
+Filename: mfhpo_simulator-1.2.6.dist-info/METADATA
+Comment: 
+
+Filename: mfhpo_simulator-1.2.6.dist-info/WHEEL
+Comment: 
+
+Filename: mfhpo_simulator-1.2.6.dist-info/top_level.txt
+Comment: 
+
+Filename: mfhpo_simulator-1.2.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## benchmark_simulator/__init__.py

```diff
@@ -1,12 +1,12 @@
 from benchmark_simulator._constants import AbstractAskTellOptimizer, ObjectiveFuncType
 from benchmark_simulator.simulator import ObjectiveFuncWrapper, get_multiple_wrappers
 
 
-__version__ = "1.2.5"
+__version__ = "1.2.6"
 __copyright__ = "Copyright (C) 2023 Shuhei Watanabe"
 __licence__ = "Apache-2.0 License"
 __author__ = "Shuhei Watanabe"
 __author_email__ = "shuhei.watanabe.utokyo@gmail.com"
 __url__ = "https://github.com/nabenabe0928/mfhpo-simulator"
```

## Comparing `mfhpo_simulator-1.2.5.dist-info/LICENSE` & `mfhpo_simulator-1.2.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mfhpo_simulator-1.2.5.dist-info/RECORD` & `mfhpo_simulator-1.2.6.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,19 @@
-benchmark_simulator/__init__.py,sha256=H9QemnTzx17HGLzuxY4WhEHQ3mRoHgbgtmc2HEtUQuQ,560
+benchmark_simulator/__init__.py,sha256=A80Q8uXYuFqZkRmxJD12ULnPDjkiH3rtAteDZmclVgg,560
 benchmark_simulator/_constants.py,sha256=j23rkYb3d9d2Mrqc8fs_nOk8GYWgC3Mw_JVa0pZxU-c,7761
 benchmark_simulator/_secure_proc.py,sha256=NfvcOGg8-SUW8FNaPTn6ShKayTjOfwTbZOQmCibEToM,12622
 benchmark_simulator/_utils.py,sha256=ZA8l51dZMxpjhMZCUExO-Mg8r5ilJWdvR2P3RFipzk4,5116
 benchmark_simulator/simulator.py,sha256=xdBLgBwmG3ZDNCdyjGZPvO6IJSD4u1Mwo_VqR3UpdKc,28910
 benchmark_simulator/_simulator/_base_wrapper.py,sha256=HvK4Iq1vjCuD1HEcphY-hl4Wo_vo1d-N_FA9PFkYukA,2582
 benchmark_simulator/_simulator/_utils.py,sha256=5vqU_iT-2TdTwyAXSscJsqEuSOp-SMKGMk1K_qVmy1g,3335
 benchmark_simulator/_simulator/_worker.py,sha256=y0hOLlAcSlS8yNIF3TUIiYvkbgTygvAV2Xzi0v8il9w,13196
 benchmark_simulator/_simulator/_worker_manager.py,sha256=wwdsMDeuVLjdFKqbZ3sJ7C5Ep8G2fFDT0jyYw-RkGGc,3767
 benchmark_simulator/_simulator/_worker_manager_for_ask_and_tell.py,sha256=UxuQI4--_uExrhweE3i4I5_z-cVz-mPOcJb_1RX4G3c,9134
-mfhpo_simulator-1.2.5.dist-info/LICENSE,sha256=auQsw_aAlfeXmKRQ_tmNBjUD2-wJojtRJPslgGyGqK4,10760
-mfhpo_simulator-1.2.5.dist-info/METADATA,sha256=Zo1Hr7EMiu24McBaiRSH7eWuYD94PPFDshthdLupkOE,307
-mfhpo_simulator-1.2.5.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-mfhpo_simulator-1.2.5.dist-info/top_level.txt,sha256=dkUhIqI2xJvV1NOS7bvMDWMNDJ1GGBwTnOBedLuz3OA,51
-mfhpo_simulator-1.2.5.dist-info/RECORD,,
+benchmark_simulator/_trackers/_config_tracker.py,sha256=-tKF_13VtOnAmCm0uzENpUg_ePyd7o_PvG9mkxzXjzQ,2181
+benchmark_simulator/_trackers/_state_tracker.py,sha256=EyeOuoFPf7c8yUgmhrDe54d0wc0Jowxo-6Vs7aUBZ5I,5012
+benchmark_simulator/utils/__init__.py,sha256=PWSU9sL4fLNRLkwm3mElZ7D_wLCWDdyCZa39RqcTYoQ,284
+benchmark_simulator/utils/_performance_over_time.py,sha256=gGUMahKBBZbL0deYYnvF1qzyJ-MH2dRf39IigWGGnek,8990
+mfhpo_simulator-1.2.6.dist-info/LICENSE,sha256=auQsw_aAlfeXmKRQ_tmNBjUD2-wJojtRJPslgGyGqK4,10760
+mfhpo_simulator-1.2.6.dist-info/METADATA,sha256=nJ233eTJiAvdGb1SJnig0nxLV70jlZiGdhqjJNSYt6A,307
+mfhpo_simulator-1.2.6.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+mfhpo_simulator-1.2.6.dist-info/top_level.txt,sha256=uJovuRlKQlk3_JQI_pIvLjq9bJ7D1LdHBYxgRvtIzFk,107
+mfhpo_simulator-1.2.6.dist-info/RECORD,,
```

