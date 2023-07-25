# Comparing `tmp/flywheel_bids-1.2.3-py3-none-any.whl.zip` & `tmp/flywheel_bids-1.2.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 106019 bytes, number of entries: 54
+Zip file size: 106036 bytes, number of entries: 54
 -rw-r--r--  2.0 unx        5 b- defN 80-Jan-01 00:00 flywheel_bids/__init__.py
 -rw-r--r--  2.0 unx    23112 b- defN 80-Jan-01 00:00 flywheel_bids/curate_bids.py
 -rw-r--r--  2.0 unx    23741 b- defN 80-Jan-01 00:00 flywheel_bids/export_bids.py
 -rw-r--r--  2.0 unx       76 b- defN 80-Jan-01 00:00 flywheel_bids/results/__init__.py
 -rw-r--r--  2.0 unx     2361 b- defN 80-Jan-01 00:00 flywheel_bids/results/zip_htmls.py
 -rw-r--r--  2.0 unx     5147 b- defN 80-Jan-01 00:00 flywheel_bids/results/zip_intermediate.py
 -rw-r--r--  2.0 unx        5 b- defN 80-Jan-01 00:00 flywheel_bids/supporting_files/__init__.py
 -rw-r--r--  2.0 unx    10537 b- defN 80-Jan-01 00:00 flywheel_bids/supporting_files/bidsify_flywheel.py
 -rw-r--r--  2.0 unx     4353 b- defN 80-Jan-01 00:00 flywheel_bids/supporting_files/classifications.py
 -rw-r--r--  2.0 unx     1234 b- defN 80-Jan-01 00:00 flywheel_bids/supporting_files/errors.py
 -rw-r--r--  2.0 unx     6607 b- defN 80-Jan-01 00:00 flywheel_bids/supporting_files/file_funcs.py
 -rw-r--r--  2.0 unx     7311 b- defN 80-Jan-01 00:00 flywheel_bids/supporting_files/project_tree.py
--rw-r--r--  2.0 unx     6252 b- defN 80-Jan-01 00:00 flywheel_bids/supporting_files/resolver.py
+-rw-r--r--  2.0 unx     6305 b- defN 80-Jan-01 00:00 flywheel_bids/supporting_files/resolver.py
 -rw-r--r--  2.0 unx    23538 b- defN 80-Jan-01 00:00 flywheel_bids/supporting_files/templates.py
 -rw-r--r--  2.0 unx    10872 b- defN 80-Jan-01 00:00 flywheel_bids/supporting_files/utils.py
 -rw-r--r--  2.0 unx      175 b- defN 80-Jan-01 00:00 flywheel_bids/templates/README.md
 -rw-r--r--  2.0 unx    27899 b- defN 80-Jan-01 00:00 flywheel_bids/templates/bids-v1.json
 -rw-r--r--  2.0 unx    53901 b- defN 80-Jan-01 00:00 flywheel_bids/templates/default.json
 -rw-r--r--  2.0 unx     1536 b- defN 80-Jan-01 00:00 flywheel_bids/templates/flywheel_curated/README.md
 -rw-r--r--  2.0 unx      271 b- defN 80-Jan-01 00:00 flywheel_bids/templates/flywheel_curated/bridge-bdlong-project-template-attributes.txt
@@ -45,12 +45,12 @@
 -rw-r--r--  2.0 unx    44997 b- defN 80-Jan-01 00:00 flywheel_bids/templates/reproin.json
 -rw-r--r--  2.0 unx    63150 b- defN 80-Jan-01 00:00 flywheel_bids/upload_bids.py
 -rw-r--r--  2.0 unx    13998 b- defN 80-Jan-01 00:00 flywheel_bids/utils/download_run_level.py
 -rw-r--r--  2.0 unx     2026 b- defN 80-Jan-01 00:00 flywheel_bids/utils/performance.py
 -rw-r--r--  2.0 unx     1816 b- defN 80-Jan-01 00:00 flywheel_bids/utils/run_level.py
 -rw-r--r--  2.0 unx     2522 b- defN 80-Jan-01 00:00 flywheel_bids/utils/tree.py
 -rw-r--r--  2.0 unx     5898 b- defN 80-Jan-01 00:00 flywheel_bids/utils/validate.py
--rw-r--r--  2.0 unx     5627 b- defN 80-Jan-01 00:00 flywheel_bids-1.2.3.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 flywheel_bids-1.2.3.dist-info/WHEEL
--rw-r--r--  2.0 unx     1066 b- defN 80-Jan-01 00:00 flywheel_bids-1.2.3.dist-info/LICENSE
-?rw-r--r--  2.0 unx     6263 b- defN 16-Jan-01 00:00 flywheel_bids-1.2.3.dist-info/RECORD
-54 files, 548063 bytes uncompressed, 95397 bytes compressed:  82.6%
+-rw-r--r--  2.0 unx     5627 b- defN 80-Jan-01 00:00 flywheel_bids-1.2.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 flywheel_bids-1.2.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx     1066 b- defN 80-Jan-01 00:00 flywheel_bids-1.2.4.dist-info/LICENSE
+?rw-r--r--  2.0 unx     6263 b- defN 16-Jan-01 00:00 flywheel_bids-1.2.4.dist-info/RECORD
+54 files, 548116 bytes uncompressed, 95414 bytes compressed:  82.6%
```

## zipnote {}

```diff
@@ -144,20 +144,20 @@
 
 Filename: flywheel_bids/utils/tree.py
 Comment: 
 
 Filename: flywheel_bids/utils/validate.py
 Comment: 
 
-Filename: flywheel_bids-1.2.3.dist-info/METADATA
+Filename: flywheel_bids-1.2.4.dist-info/METADATA
 Comment: 
 
-Filename: flywheel_bids-1.2.3.dist-info/WHEEL
+Filename: flywheel_bids-1.2.4.dist-info/WHEEL
 Comment: 
 
-Filename: flywheel_bids-1.2.3.dist-info/LICENSE
+Filename: flywheel_bids-1.2.4.dist-info/LICENSE
 Comment: 
 
-Filename: flywheel_bids-1.2.3.dist-info/RECORD
+Filename: flywheel_bids-1.2.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## flywheel_bids/supporting_files/resolver.py

```diff
@@ -144,20 +144,20 @@
     Args:
         fw (Flywheel Client): to be able to access the file
         acquisition_id (str): The acquisition that the NIfTI and json files are in
         nifti_name (str): Name of the NIfTI file that matches the sidecar file name
         field_name (str): The key at the top level of the json file where the results should go, e.g. Intendedfor
         results (object): the value to assign to the key, e.g. a list of strings (BIDS paths)
     """
-    if fw == None:
-        print("Client is None.  Cannot update sidecar")
-    else:
+    if isinstance(fw, flywheel.client.Client):
         sidecar_name = nifti_name[:-7] + ".json"
         acquisition = fw.get_acquisition(acquisition_id)
         sidecar_contents = acquisition.read_file(sidecar_name)
         if not sidecar_contents:
             print(f"Unable to load {sidecar_name}")
         sidecar_json = json.loads(sidecar_contents)
         sidecar_json[field_name] = results
         json_str = json.dumps(sidecar_json, indent=4)
         file_spec = flywheel.FileSpec(sidecar_name, json_str, "text/plain")
         acquisition.upload_file(file_spec)
+    else:  # must be a test
+        print(f"Client is {type(fw)}.  Cannot update sidecar")
```

## Comparing `flywheel_bids-1.2.3.dist-info/METADATA` & `flywheel_bids-1.2.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flywheel-bids
-Version: 1.2.3
+Version: 1.2.4
 Summary: Flywheel BIDS Client
 Home-page: https://gitlab.com/flywheel-io/public/bids-client
 License: MIT
 Keywords: Flywheel,flywheel,BIDS,SDK
 Author: Flywheel
 Author-email: support@flywheel.io
 Requires-Python: >=3.8,<4.0
```

## Comparing `flywheel_bids-1.2.3.dist-info/LICENSE` & `flywheel_bids-1.2.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `flywheel_bids-1.2.3.dist-info/RECORD` & `flywheel_bids-1.2.4.dist-info/RECORD`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 flywheel_bids/results/zip_intermediate.py,sha256=DZmSBnkj_YdpRKfZC13MimwjGjwclWDXF06uv3uMS9c,5147
 flywheel_bids/supporting_files/__init__.py,sha256=Y4xogqvLXa5sAUBRzU_qrcOE145CqsQhbeTjpwPmX1E,5
 flywheel_bids/supporting_files/bidsify_flywheel.py,sha256=_JAy7mZOM5BrMl-TMvSs7gnr-lrkfCzI33yo8EvMoH4,10537
 flywheel_bids/supporting_files/classifications.py,sha256=uisUcFW-36Zq4uXFnd-sI1Q93E9E6zgeBqipeF0AdtA,4353
 flywheel_bids/supporting_files/errors.py,sha256=6oi6hA2EM7b-7RiOjCUL0lnVLxOuEclzfoyEvtuaR3o,1234
 flywheel_bids/supporting_files/file_funcs.py,sha256=0ZP4w7Ey5uc8MpeEOgOUjZVNOum05C9Ha-V-17XOt1I,6607
 flywheel_bids/supporting_files/project_tree.py,sha256=081OxA5UgL4l1D0rCa1xQWxuu5Bxsepcdha2ir96E7E,7311
-flywheel_bids/supporting_files/resolver.py,sha256=Omd1sH9R6HD3oG1C2IzT-C9oVH5rOj6I4Ev-IEJnFWY,6252
+flywheel_bids/supporting_files/resolver.py,sha256=fxPNPj9p4g2U4pQU7ib2wkKZICNhWyvU1U7M4uwpv8k,6305
 flywheel_bids/supporting_files/templates.py,sha256=7MW7Y41Q1fBaATkcK2Sl8bC_9zracyzFjgn4EjzOW-g,23538
 flywheel_bids/supporting_files/utils.py,sha256=apYF0J9yp7vqWmsnMCPZb59m2oPOEld_YbKjYDjRoQM,10872
 flywheel_bids/templates/README.md,sha256=W2b6jw4TIpoSxEUqdC8AKjFUWLiTX4Q2kDDCOKK1vaw,175
 flywheel_bids/templates/bids-v1.json,sha256=nxiQHfvfN5tEMTn0USoijkFqixnBGhHPpItiUoJ0qt8,27899
 flywheel_bids/templates/default.json,sha256=dLcG0wzXyL33cOnFT3d6m-OVgo8XCQLXDBmpy8KDTTo,53901
 flywheel_bids/templates/flywheel_curated/README.md,sha256=k290CuURkHP3w847_qKcVwaqVKTKSZv_r8onr2_peDc,1536
 flywheel_bids/templates/flywheel_curated/bridge-bdlong-project-template-attributes.txt,sha256=PsL48bjRmfcVKQR_rU6b9pshg_qnPNpUL7Ls5zIFH8o,271
@@ -44,11 +44,11 @@
 flywheel_bids/templates/reproin.json,sha256=j9FxrVe3k6wqF4Kgice7FPnMDzdoDnVhkVD3FV0ylgU,44997
 flywheel_bids/upload_bids.py,sha256=Z8NkWpmTtOYGJkXx2gCWvvmkJ51X8DPnMIpIjgnodQ0,63150
 flywheel_bids/utils/download_run_level.py,sha256=NssyGcOzVURfagXgzryQHLA9YZFA3PzwI7EyuQUyVLU,13998
 flywheel_bids/utils/performance.py,sha256=rcC3DyvpdJO1k18vyFlK93OhazPctBwABb6qA4kNEMo,2026
 flywheel_bids/utils/run_level.py,sha256=FL_ChyzCECoUS7HrdRjWCEnE6e78wIA5ePKjQ4PiT2c,1816
 flywheel_bids/utils/tree.py,sha256=6bfQmkp1iqwk9RrIXxrMHMldwe9ALbvL81RA5NIqXn0,2522
 flywheel_bids/utils/validate.py,sha256=noMFXBD7_k8wioxhSIiw7JNzExiyPcS3DyBbpWUiaww,5898
-flywheel_bids-1.2.3.dist-info/METADATA,sha256=VK2lida9Sg12dyBzDhEtKJpRqrTCFaj_XxaUOnwadG8,5627
-flywheel_bids-1.2.3.dist-info/WHEEL,sha256=vVCvjcmxuUltf8cYhJ0sJMRDLr1XsPuxEId8YDzbyCY,88
-flywheel_bids-1.2.3.dist-info/LICENSE,sha256=dqr2l_pCmH5B2MnrF0BMMugS_MmWV4bPLqF9aHWn4Tk,1066
-flywheel_bids-1.2.3.dist-info/RECORD,,
+flywheel_bids-1.2.4.dist-info/METADATA,sha256=TVc2uOBEcDVC0ygoI7aN2uOWtz1lEicrS4MGyZ2NsAo,5627
+flywheel_bids-1.2.4.dist-info/WHEEL,sha256=vVCvjcmxuUltf8cYhJ0sJMRDLr1XsPuxEId8YDzbyCY,88
+flywheel_bids-1.2.4.dist-info/LICENSE,sha256=dqr2l_pCmH5B2MnrF0BMMugS_MmWV4bPLqF9aHWn4Tk,1066
+flywheel_bids-1.2.4.dist-info/RECORD,,
```

