# Comparing `tmp/cval-lib-0.0.2.8.tar.gz` & `tmp/cval-lib-0.0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cval-lib-0.0.2.8.tar", last modified: Fri Jul  7 10:26:12 2023, max compression
+gzip compressed data, was "cval-lib-0.0.2.9.tar", last modified: Wed Jul 12 05:26:10 2023, max compression
```

## Comparing `cval-lib-0.0.2.8.tar` & `cval-lib-0.0.2.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-07 10:26:12.927762 cval-lib-0.0.2.8/
--rw-rw-r--   0 localhost  (1000) localhost  (1000)    11357 2023-06-29 09:48:08.000000 cval-lib-0.0.2.8/LICENSE
--rw-rw-r--   0 localhost  (1000) localhost  (1000)      204 2023-07-07 10:26:12.927762 cval-lib-0.0.2.8/PKG-INFO
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     6568 2023-07-07 09:13:46.000000 cval-lib-0.0.2.8/README.md
-drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-07 10:26:12.927762 cval-lib-0.0.2.8/cval_lib/
--rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-07-02 18:05:48.000000 cval-lib-0.0.2.8/cval_lib/__init__.py
-drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-07 10:26:12.927762 cval-lib-0.0.2.8/cval_lib/configs/
--rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.2.8/cval_lib/configs/__init__.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)      137 2023-07-02 13:22:21.000000 cval-lib-0.0.2.8/cval_lib/configs/main_config.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     1428 2023-06-29 09:48:08.000000 cval-lib-0.0.2.8/cval_lib/connection.py
-drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-07 10:26:12.927762 cval-lib-0.0.2.8/cval_lib/examples/
--rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.2.8/cval_lib/examples/__init__.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     1637 2023-07-07 09:09:28.000000 cval-lib-0.0.2.8/cval_lib/examples/dataset.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     1829 2023-07-07 09:09:28.000000 cval-lib-0.0.2.8/cval_lib/examples/embeddings.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     1258 2023-07-07 09:09:28.000000 cval-lib-0.0.2.8/cval_lib/examples/monkey_patch.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     2022 2023-07-07 09:09:28.000000 cval-lib-0.0.2.8/cval_lib/examples/on_pemise.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     2367 2023-07-07 09:09:28.000000 cval-lib-0.0.2.8/cval_lib/examples/polling.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     1383 2023-07-07 10:26:10.000000 cval-lib-0.0.2.8/cval_lib/examples/result.py
-drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-07 10:26:12.927762 cval-lib-0.0.2.8/cval_lib/handlers/
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     1260 2023-06-29 09:48:08.000000 cval-lib-0.0.2.8/cval_lib/handlers/__async.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.2.8/cval_lib/handlers/__init__.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     2750 2023-07-07 09:09:28.000000 cval-lib-0.0.2.8/cval_lib/handlers/_abstract_handler.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     5076 2023-07-06 06:28:17.000000 cval-lib-0.0.2.8/cval_lib/handlers/dataset.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     1984 2023-07-07 10:26:10.000000 cval-lib-0.0.2.8/cval_lib/handlers/detection.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     5250 2023-07-02 18:30:35.000000 cval-lib-0.0.2.8/cval_lib/handlers/embedding.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)      950 2023-07-07 09:09:28.000000 cval-lib-0.0.2.8/cval_lib/handlers/frame.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)      710 2023-07-07 09:09:28.000000 cval-lib-0.0.2.8/cval_lib/handlers/frames.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     2449 2023-07-07 10:26:10.000000 cval-lib-0.0.2.8/cval_lib/handlers/result.py
-drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-07 10:26:12.927762 cval-lib-0.0.2.8/cval_lib/models/
--rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.2.8/cval_lib/models/__init__.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     1914 2023-06-29 09:48:08.000000 cval-lib-0.0.2.8/cval_lib/models/dataset.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     3014 2023-07-06 15:53:23.000000 cval-lib-0.0.2.8/cval_lib/models/detection.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     1404 2023-07-02 18:41:52.000000 cval-lib-0.0.2.8/cval_lib/models/embedding.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     2210 2023-07-07 10:26:10.000000 cval-lib-0.0.2.8/cval_lib/models/result.py
-drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-07 10:26:12.927762 cval-lib-0.0.2.8/cval_lib/patterns/
--rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.2.8/cval_lib/patterns/__init__.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)      240 2023-06-29 09:48:08.000000 cval-lib-0.0.2.8/cval_lib/patterns/singleton.py
-drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-07 10:26:12.927762 cval-lib-0.0.2.8/cval_lib.egg-info/
--rw-rw-r--   0 localhost  (1000) localhost  (1000)      204 2023-07-07 10:26:12.000000 cval-lib-0.0.2.8/cval_lib.egg-info/PKG-INFO
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     1083 2023-07-07 10:26:12.000000 cval-lib-0.0.2.8/cval_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 localhost  (1000) localhost  (1000)        1 2023-07-07 10:26:12.000000 cval-lib-0.0.2.8/cval_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 localhost  (1000) localhost  (1000)       18 2023-07-07 10:26:12.000000 cval-lib-0.0.2.8/cval_lib.egg-info/requires.txt
--rw-rw-r--   0 localhost  (1000) localhost  (1000)        9 2023-07-07 10:26:12.000000 cval-lib-0.0.2.8/cval_lib.egg-info/top_level.txt
--rw-rw-r--   0 localhost  (1000) localhost  (1000)       38 2023-07-07 10:26:12.927762 cval-lib-0.0.2.8/setup.cfg
--rw-rw-r--   0 localhost  (1000) localhost  (1000)      448 2023-07-07 10:26:10.000000 cval-lib-0.0.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 05:26:10.791409 cval-lib-0.0.2.9/
+-rw-rw-rw-   0        0        0    11558 2023-07-12 05:13:55.000000 cval-lib-0.0.2.9/LICENSE
+-rw-rw-rw-   0        0        0      212 2023-07-12 05:26:10.791409 cval-lib-0.0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0     6795 2023-07-12 05:13:55.000000 cval-lib-0.0.2.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 05:26:10.748410 cval-lib-0.0.2.9/cval_lib/
+-rw-rw-rw-   0        0        0        0 2023-07-12 05:13:55.000000 cval-lib-0.0.2.9/cval_lib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 05:26:10.749409 cval-lib-0.0.2.9/cval_lib/configs/
+-rw-rw-rw-   0        0        0        0 2023-07-12 05:13:55.000000 cval-lib-0.0.2.9/cval_lib/configs/__init__.py
+-rw-rw-rw-   0        0        0      142 2023-07-12 05:13:55.000000 cval-lib-0.0.2.9/cval_lib/configs/main_config.py
+-rw-rw-rw-   0        0        0     1474 2023-07-12 05:13:55.000000 cval-lib-0.0.2.9/cval_lib/connection.py
+drwxrwxrwx   0        0        0        0 2023-07-12 05:26:10.753410 cval-lib-0.0.2.9/cval_lib/examples/
+-rw-rw-rw-   0        0        0        0 2023-07-12 05:13:55.000000 cval-lib-0.0.2.9/cval_lib/examples/__init__.py
+-rw-rw-rw-   0        0        0     1678 2023-07-12 05:13:55.000000 cval-lib-0.0.2.9/cval_lib/examples/dataset.py
+-rw-rw-rw-   0        0        0     1870 2023-07-12 05:13:55.000000 cval-lib-0.0.2.9/cval_lib/examples/embeddings.py
+-rw-rw-rw-   0        0        0     1283 2023-07-12 05:13:55.000000 cval-lib-0.0.2.9/cval_lib/examples/monkey_patch.py
+-rw-rw-rw-   0        0        0     2069 2023-07-12 05:13:55.000000 cval-lib-0.0.2.9/cval_lib/examples/on_pemise.py
+-rw-rw-rw-   0        0        0     2426 2023-07-12 05:13:55.000000 cval-lib-0.0.2.9/cval_lib/examples/polling.py
+-rw-rw-rw-   0        0        0     1409 2023-07-12 05:13:55.000000 cval-lib-0.0.2.9/cval_lib/examples/result.py
+drwxrwxrwx   0        0        0        0 2023-07-12 05:26:10.758409 cval-lib-0.0.2.9/cval_lib/handlers/
+-rw-rw-rw-   0        0        0     1286 2023-07-12 05:13:55.000000 cval-lib-0.0.2.9/cval_lib/handlers/__async.py
+-rw-rw-rw-   0        0        0        0 2023-07-12 05:13:55.000000 cval-lib-0.0.2.9/cval_lib/handlers/__init__.py
+-rw-rw-rw-   0        0        0     2826 2023-07-12 05:13:55.000000 cval-lib-0.0.2.9/cval_lib/handlers/_abstract_handler.py
+-rw-rw-rw-   0        0        0     5207 2023-07-12 05:21:20.000000 cval-lib-0.0.2.9/cval_lib/handlers/dataset.py
+-rw-rw-rw-   0        0        0     2035 2023-07-12 05:13:55.000000 cval-lib-0.0.2.9/cval_lib/handlers/detection.py
+-rw-rw-rw-   0        0        0     5371 2023-07-12 05:21:20.000000 cval-lib-0.0.2.9/cval_lib/handlers/embedding.py
+-rw-rw-rw-   0        0        0      988 2023-07-12 05:13:55.000000 cval-lib-0.0.2.9/cval_lib/handlers/frame.py
+-rw-rw-rw-   0        0        0      735 2023-07-12 05:13:55.000000 cval-lib-0.0.2.9/cval_lib/handlers/frames.py
+-rw-rw-rw-   0        0        0     2511 2023-07-12 05:13:55.000000 cval-lib-0.0.2.9/cval_lib/handlers/result.py
+drwxrwxrwx   0        0        0        0 2023-07-12 05:26:10.761411 cval-lib-0.0.2.9/cval_lib/models/
+-rw-rw-rw-   0        0        0        0 2023-07-12 05:13:55.000000 cval-lib-0.0.2.9/cval_lib/models/__init__.py
+-rw-rw-rw-   0        0        0     1994 2023-07-12 05:21:20.000000 cval-lib-0.0.2.9/cval_lib/models/dataset.py
+-rw-rw-rw-   0        0        0     3091 2023-07-12 05:13:55.000000 cval-lib-0.0.2.9/cval_lib/models/detection.py
+-rw-rw-rw-   0        0        0     1437 2023-07-12 05:13:55.000000 cval-lib-0.0.2.9/cval_lib/models/embedding.py
+-rw-rw-rw-   0        0        0     2290 2023-07-12 05:21:20.000000 cval-lib-0.0.2.9/cval_lib/models/result.py
+drwxrwxrwx   0        0        0        0 2023-07-12 05:26:10.762410 cval-lib-0.0.2.9/cval_lib/patterns/
+-rw-rw-rw-   0        0        0        0 2023-07-12 05:13:55.000000 cval-lib-0.0.2.9/cval_lib/patterns/__init__.py
+-rw-rw-rw-   0        0        0      248 2023-07-12 05:13:55.000000 cval-lib-0.0.2.9/cval_lib/patterns/singleton.py
+drwxrwxrwx   0        0        0        0 2023-07-12 05:26:10.787410 cval-lib-0.0.2.9/cval_lib.egg-info/
+-rw-rw-rw-   0        0        0      212 2023-07-12 05:26:10.000000 cval-lib-0.0.2.9/cval_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1829 2023-07-12 05:26:10.000000 cval-lib-0.0.2.9/cval_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 05:26:10.000000 cval-lib-0.0.2.9/cval_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-07-12 05:26:10.000000 cval-lib-0.0.2.9/cval_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-12 05:26:10.000000 cval-lib-0.0.2.9/cval_lib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 05:26:10.797415 cval-lib-0.0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0      467 2023-07-12 05:25:19.000000 cval-lib-0.0.2.9/setup.py
```

### Comparing `cval-lib-0.0.2.8/LICENSE` & `cval-lib-0.0.2.9/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `cval-lib-0.0.2.8/README.md` & `cval-lib-0.0.2.9/README.md`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,227 +1,227 @@
-<!-- TOP OF README ANCHOR -->
-<a name="top"></a>
-<!-- PROJECT LOGO -->
-<br />
-<div align="center">
-  <p>
-    <img src="https://github.com/fangorntreabeard/cval-lib/blob/main/logo/logo.jpg?raw=true" alt="Cval logo" width="155" height="155">
-  </p>
-<h3 align="center">CVAL REST API LIBRARY</h3>
-  <p align="center">
-    A library designed to interact with the REST-API cval.ai
-    <br/>
-    <b>
-      <a href="https://cval.ai">REST API docs</a>
-      ·
-      <a href="https://github.com/fangorntreabeard/cval-lib/issues">Report Bug</a>
-      ·
-      <a href="https://colab.research.google.com/drive/1f93b-aCv4MacngujLVUcQBJ9T1mJZBKH?usp=sharing"> Google Colaboratory Demo </a>
-    </b>
-  </p>
-</div>
-
-# About
-
-With CVAL, you can iteratively **improve your models** by following our active learning loop.
-
-* **First**, manually or semi-automatically annotate a random set of images.
-
-* **Next**, train your model and use uncertainty and diversity methods to score the remaining images for annotation.
-
-* **Then**, manually or semi-automatically annotate the images marked as more confident to increase the accuracy of the model.
-
-Repeat this process until you achieve an acceptable quality of the model.
-
-# Getting started
-
-To start using the CVAL Rest API, you need to **obtain** a **client/user API key**. 
-Once you have your API key, you can use it to authenticate your requests and interact with the CVAL Rest API endpoints. 
-Refer to our API documentation for detailed information on available endpoints, request formats, and response structures.
-
-## Installation
-
-#### Unix and Mac
-```shell
-python3 -m pip install cval-lib
-```
-or downloaded:
-
-```shell
-python3 -m pip install cval-lib.tar
-```
-
-#### Windows
-```powershell
-python -m pip install cval-lib
-```
-or downloaded:
-```shell
-python3 -m pip install cval-lib.tar
-```
-
-#### Submodule
-```shell
-git submodule add https://github.com/fangorntreabeard/cval-lib.git cval
-```
-## Architecture
-The library architecture consists of **three layers**:
-1. _A layer of protocols and abstract handlers_. Responsible for the use of a particular library. If an error is found, it is enough to simply change one method.
-2. _A layer of handlers._ These are all the methods that are present in the API. Are based on abstract
-3. _Model layer._ If the data structure changes, only this layer changes.
-
-## Examples
-
-##### Set your user_api_key
-
-```python3
-from cval_lib.connection import CVALConnection
-USER_API_KEY = 'awesome_api_key'
-cval = CVALConnection(USER_API_KEY)
-```
-
-> The same actions are available with the rest of the entities, but there are some nuances, for example, somewhere there is the use of models, and somewhere only parameters. But anyway, these examples well reflect possible scenarios when working with cval. The most typical api scenario is a dataset, so let's start with it.
-
-### Dataset
- > Within the framework of the created system, datasets are spaces in which data for machine learning is stored.
- Creating a dataset is similar to creating a folder.
-##### Create dataset
-```python3
-# :NOTE: To avoid incomprehensibility of errors, it is recommended to use  CVALConnection
-ds_id = cval.dataset().create(name='on-premise-scheme-ds', description='')
-print(ds_id)
-```
-
-##### Update dataset
-```python3
-ds = cval.dataset()
-print(ds.update(ds_id, description='any string data'))
-# :NOTE: the dataset can store the state (ds_id)
-ds.update(name='sample name')
-```
-
-##### Get dataset
-```python3
-print(ds.get())
-```
-
-> A further example of using the library concerns embedding. Since embedding is a large data object and the method of its creation is completely defined by the user, the embedding method works through query schemes (models).
-
-### Embeddings
-
-> Embeddings are vector representations of images obtained using pytorch or any other library
-
-##### Create embeddings
-
-```python3
-from random import random
-import uuid
-from cval_lib.models.embedding import ImageEmbeddingModel
-
-img_id_1 = str(uuid.uuid4().hex)
-img_id_2 = str(uuid.uuid4().hex)
-
-
-embeddings = [
- ImageEmbeddingModel(id=img_id_1, image_embedding=list(map(lambda x:random(), range(1000)))),
- ImageEmbeddingModel(id=img_id_2, image_embedding=list(map(lambda x: random(), range(1000)))),
-]
-
-print(embeddings)
-```
-
-
-##### Upload & check embeddings
-
-```python3
-emb = cval.embedding(ds_id, 'training')
-emb.upload_many(embeddings)
-print(emb.get_many())
-```
-
-> The following example is used to invoke active learning
- 
-### Active learning
-
-##### Get predictions data
-
-```python3
-from random import random
-import uuid
-from cval_lib.models.detection import BBoxScores, FramePrediction
-
-# :NOTE: example only
-frames_predictions = list(
-    map(
-        lambda x: FramePrediction(
-            frame_id=str(uuid.uuid4().hex),
-            predictions=list(
-                map(lambda x: BBoxScores(category_id=str(uuid.uuid4()), score=random()), range(100)))
-        ),
-        range(10)
-    )
-)
-print(frames_predictions)
-
-```
-
-##### Construct config
-
-```python3
-from cval_lib.models.detection import DetectionSamplingOnPremise
-request = DetectionSamplingOnPremise(
- num_of_samples=200, 
- bbox_selection_policy='min', 
- selection_strategy='margin', 
- sort_strategy='ascending',
- frames=frames_predictions,
-)
-```
-
-##### Run active learning
-```python3
-emb = cval.detection()
-print(emb.on_premise_sampling(request))
-```
-> The following method is most relevant when we are dealing with long-term tasks and, accordingly, with asynchronous interaction.
-##### Polling
-> refers to actively sampling the status of an external device by a client program as a synchronous activity.
-
-```python3
-import uuid
-from random import random
-from time import sleep
-
-from cval_lib.connection import CVALConnection
-from cval_lib.models.detection import DetectionSamplingOnPremise, FramePrediction, BBoxScores
-
-frames_predictions = list(
-        map(
-            lambda x: FramePrediction(
-                frame_id=str(uuid.uuid4().hex),
-                predictions=list(map(lambda _: BBoxScores(category_id=str(uuid.uuid4()), score=random()), range(100)))
-            ),
-            range(1000)
-        )
-    )
-
-request = DetectionSamplingOnPremise(
-        num_of_samples=200,
-        bbox_selection_policy='min',
-        selection_strategy='margin',
-        sort_strategy='ascending',
-        frames=frames_predictions,
-    )
-emb = cval.detection()
-print(emb.on_premise_sampling(request))
-
-result = None
-sleep_sec = 1
-while result is None:
-    result = emb.result.get().result
-    print(f'Polling... {sleep_sec} s')
-    sleep(sleep_sec)
-    sleep_sec *= 2
-
-print(result)
-
-```
+<!-- TOP OF README ANCHOR -->
+<a name="top"></a>
+<!-- PROJECT LOGO -->
+<br />
+<div align="center">
+  <p>
+    <img src="https://github.com/fangorntreabeard/cval-lib/blob/main/logo/logo.jpg?raw=true" alt="Cval logo" width="155" height="155">
+  </p>
+<h3 align="center">CVAL REST API LIBRARY</h3>
+  <p align="center">
+    A library designed to interact with the REST-API cval.ai
+    <br/>
+    <b>
+      <a href="https://cval.ai">REST API docs</a>
+      ·
+      <a href="https://github.com/fangorntreabeard/cval-lib/issues">Report Bug</a>
+      ·
+      <a href="https://colab.research.google.com/drive/1f93b-aCv4MacngujLVUcQBJ9T1mJZBKH?usp=sharing"> Google Colaboratory Demo </a>
+    </b>
+  </p>
+</div>
+
+# About
+
+With CVAL, you can iteratively **improve your models** by following our active learning loop.
+
+* **First**, manually or semi-automatically annotate a random set of images.
+
+* **Next**, train your model and use uncertainty and diversity methods to score the remaining images for annotation.
+
+* **Then**, manually or semi-automatically annotate the images marked as more confident to increase the accuracy of the model.
+
+Repeat this process until you achieve an acceptable quality of the model.
+
+# Getting started
+
+To start using the CVAL Rest API, you need to **obtain** a **client/user API key**. 
+Once you have your API key, you can use it to authenticate your requests and interact with the CVAL Rest API endpoints. 
+Refer to our API documentation for detailed information on available endpoints, request formats, and response structures.
+
+## Installation
+
+#### Unix and Mac
+```shell
+python3 -m pip install cval-lib
+```
+or downloaded:
+
+```shell
+python3 -m pip install cval-lib.tar
+```
+
+#### Windows
+```powershell
+python -m pip install cval-lib
+```
+or downloaded:
+```shell
+python3 -m pip install cval-lib.tar
+```
+
+#### Submodule
+```shell
+git submodule add https://github.com/fangorntreabeard/cval-lib.git cval
+```
+## Architecture
+The library architecture consists of **three layers**:
+1. _A layer of protocols and abstract handlers_. Responsible for the use of a particular library. If an error is found, it is enough to simply change one method.
+2. _A layer of handlers._ These are all the methods that are present in the API. Are based on abstract
+3. _Model layer._ If the data structure changes, only this layer changes.
+
+## Examples
+
+##### Set your user_api_key
+
+```python3
+from cval_lib.connection import CVALConnection
+USER_API_KEY = 'awesome_api_key'
+cval = CVALConnection(USER_API_KEY)
+```
+
+> The same actions are available with the rest of the entities, but there are some nuances, for example, somewhere there is the use of models, and somewhere only parameters. But anyway, these examples well reflect possible scenarios when working with cval. The most typical api scenario is a dataset, so let's start with it.
+
+### Dataset
+ > Within the framework of the created system, datasets are spaces in which data for machine learning is stored.
+ Creating a dataset is similar to creating a folder.
+##### Create dataset
+```python3
+# :NOTE: To avoid incomprehensibility of errors, it is recommended to use  CVALConnection
+ds_id = cval.dataset().create(name='on-premise-scheme-ds', description='')
+print(ds_id)
+```
+
+##### Update dataset
+```python3
+ds = cval.dataset()
+print(ds.update(ds_id, description='any string data'))
+# :NOTE: the dataset can store the state (ds_id)
+ds.update(name='sample name')
+```
+
+##### Get dataset
+```python3
+print(ds.get())
+```
+
+> A further example of using the library concerns embedding. Since embedding is a large data object and the method of its creation is completely defined by the user, the embedding method works through query schemes (models).
+
+### Embeddings
+
+> Embeddings are vector representations of images obtained using pytorch or any other library
+
+##### Create embeddings
+
+```python3
+from random import random
+import uuid
+from cval_lib.models.embedding import ImageEmbeddingModel
+
+img_id_1 = str(uuid.uuid4().hex)
+img_id_2 = str(uuid.uuid4().hex)
+
+
+embeddings = [
+ ImageEmbeddingModel(id=img_id_1, image_embedding=list(map(lambda x:random(), range(1000)))),
+ ImageEmbeddingModel(id=img_id_2, image_embedding=list(map(lambda x: random(), range(1000)))),
+]
+
+print(embeddings)
+```
+
+
+##### Upload & check embeddings
+
+```python3
+emb = cval.embedding(ds_id, 'training')
+emb.upload_many(embeddings)
+print(emb.get_many())
+```
+
+> The following example is used to invoke active learning
+ 
+### Active learning
+
+##### Get predictions data
+
+```python3
+from random import random
+import uuid
+from cval_lib.models.detection import BBoxScores, FramePrediction
+
+# :NOTE: example only
+frames_predictions = list(
+    map(
+        lambda x: FramePrediction(
+            frame_id=str(uuid.uuid4().hex),
+            predictions=list(
+                map(lambda x: BBoxScores(category_id=str(uuid.uuid4()), score=random()), range(100)))
+        ),
+        range(10)
+    )
+)
+print(frames_predictions)
+
+```
+
+##### Construct config
+
+```python3
+from cval_lib.models.detection import DetectionSamplingOnPremise
+request = DetectionSamplingOnPremise(
+ num_of_samples=200, 
+ bbox_selection_policy='min', 
+ selection_strategy='margin', 
+ sort_strategy='ascending',
+ frames=frames_predictions,
+)
+```
+
+##### Run active learning
+```python3
+emb = cval.detection()
+print(emb.on_premise_sampling(request))
+```
+> The following method is most relevant when we are dealing with long-term tasks and, accordingly, with asynchronous interaction.
+##### Polling
+> refers to actively sampling the status of an external device by a client program as a synchronous activity.
+
+```python3
+import uuid
+from random import random
+from time import sleep
+
+from cval_lib.connection import CVALConnection
+from cval_lib.models.detection import DetectionSamplingOnPremise, FramePrediction, BBoxScores
+
+frames_predictions = list(
+        map(
+            lambda x: FramePrediction(
+                frame_id=str(uuid.uuid4().hex),
+                predictions=list(map(lambda _: BBoxScores(category_id=str(uuid.uuid4()), score=random()), range(100)))
+            ),
+            range(1000)
+        )
+    )
+
+request = DetectionSamplingOnPremise(
+        num_of_samples=200,
+        bbox_selection_policy='min',
+        selection_strategy='margin',
+        sort_strategy='ascending',
+        frames=frames_predictions,
+    )
+emb = cval.detection()
+print(emb.on_premise_sampling(request))
+
+result = None
+sleep_sec = 1
+while result is None:
+    result = emb.result.get().result
+    print(f'Polling... {sleep_sec} s')
+    sleep(sleep_sec)
+    sleep_sec *= 2
+
+print(result)
+
+```
```

### Comparing `cval-lib-0.0.2.8/cval_lib/connection.py` & `cval-lib-0.0.2.9/cval_lib/connection.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-from requests import Session
-
-from cval_lib.handlers.dataset import Dataset
-from cval_lib.handlers.embedding import Embedding
-from cval_lib.handlers.detection import Detection
-from cval_lib.handlers.result import Result
-
-
-class CVALConnection:
-    def __init__(self, user_api_key: str):
-        self._session = Session()
-        self._session.headers = {'user_api_key': user_api_key}
-
-    def dataset(self):
-        """
-        actions with dataset: : create, get, delete, update by ID or all (with some limits)
-        :return: Dataset
-        """
-        return Dataset(session=self._session)
-
-    def embedding(self, dataset_id: str, type_of_dataset: str):
-        """
-        actions with embedding: create, get, delete, update by ID or all (with some limits)
-        :param dataset_id: id of dataset
-        :param type_of_dataset: type of dataset (training, test, validation)
-        :return: Embedding
-        """
-        return Embedding(self._session, dataset_id=dataset_id, type_of_dataset=type_of_dataset)
-
-    def detection(self, ):
-        """
-        This method can be used to call a detection sampling or test
-        :return: Detection
-        """
-        return Detection(self._session)
-
-    def result(self):
-        """
-        This method can be used for polling
-        :return: Result
-        """
-        return Result(self._session)
-
-    def __del__(self):
-        self._session.close()
-        del self
+from requests import Session
+
+from cval_lib.handlers.dataset import Dataset
+from cval_lib.handlers.embedding import Embedding
+from cval_lib.handlers.detection import Detection
+from cval_lib.handlers.result import Result
+
+
+class CVALConnection:
+    def __init__(self, user_api_key: str):
+        self._session = Session()
+        self._session.headers = {'user_api_key': user_api_key}
+
+    def dataset(self):
+        """
+        actions with dataset: : create, get, delete, update by ID or all (with some limits)
+        :return: Dataset
+        """
+        return Dataset(session=self._session)
+
+    def embedding(self, dataset_id: str, type_of_dataset: str):
+        """
+        actions with embedding: create, get, delete, update by ID or all (with some limits)
+        :param dataset_id: id of dataset
+        :param type_of_dataset: type of dataset (training, test, validation)
+        :return: Embedding
+        """
+        return Embedding(self._session, dataset_id=dataset_id, type_of_dataset=type_of_dataset)
+
+    def detection(self, ):
+        """
+        This method can be used to call a detection sampling or test
+        :return: Detection
+        """
+        return Detection(self._session)
+
+    def result(self):
+        """
+        This method can be used for polling
+        :return: Result
+        """
+        return Result(self._session)
+
+    def __del__(self):
+        self._session.close()
+        del self
```

### Comparing `cval-lib-0.0.2.8/cval_lib/examples/dataset.py` & `cval-lib-0.0.2.9/cval_lib/examples/dataset.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-"""
-Introducing CVAL Rest API, a powerful tool for AI developers in the computer vision field.
-Our service combines the concepts of human-in-the-loop and active learning to improve the quality of
-your models and minimize annotation costs for classification, detection, and segmentation cases.
-
-With CVAL, you can iteratively improve your models by following our active learning loop.
-First, manually or semi-automatically annotate a random set of images.
-Next, train your model and use uncertainty and diversity methods to score the remaining images for annotation.
-Then, manually or semi-automatically annotate the images marked as more confident to increase the accuracy of the model.
-Repeat this process until you achieve an acceptable quality of the model.
-
-Our service makes it easy to implement this workflow and improve your models quickly and efficiently.
-Try our demo notebook to see how CVAL can revolutionize your computer vision projects.
-
-To obtain a client_api_key, please send a request to k.suhorukov@digital-quarters.com
-"""
-
-
-if __name__ == '__main__':
-    from cval_lib.connection import CVALConnection
-
-    # set up your user_api_key
-    user_api_key = 'USER_API_KEY'
-    # set up session
-    cval = CVALConnection(user_api_key)
-    # choose strategy
-    ds = cval.dataset()
-    # create your dataset
-    ds_id = ds.create()
-    print(ds_id)
-    # update your dataset
-    update = ds.update(name='any')
-    print('', update)
-    # watch changes
-    get = ds.get()
-    print(get)
-    # also you can use dataset_id for watch changes
-    get = ds.get(ds_id)
-    print(get)
-    # get all datasets
-    print(ds.get_all())
+"""
+Introducing CVAL Rest API, a powerful tool for AI developers in the computer vision field.
+Our service combines the concepts of human-in-the-loop and active learning to improve the quality of
+your models and minimize annotation costs for classification, detection, and segmentation cases.
+
+With CVAL, you can iteratively improve your models by following our active learning loop.
+First, manually or semi-automatically annotate a random set of images.
+Next, train your model and use uncertainty and diversity methods to score the remaining images for annotation.
+Then, manually or semi-automatically annotate the images marked as more confident to increase the accuracy of the model.
+Repeat this process until you achieve an acceptable quality of the model.
+
+Our service makes it easy to implement this workflow and improve your models quickly and efficiently.
+Try our demo notebook to see how CVAL can revolutionize your computer vision projects.
+
+To obtain a client_api_key, please send a request to k.suhorukov@digital-quarters.com
+"""
+
+
+if __name__ == '__main__':
+    from cval_lib.connection import CVALConnection
+
+    # set up your user_api_key
+    user_api_key = 'USER_API_KEY'
+    # set up session
+    cval = CVALConnection(user_api_key)
+    # choose strategy
+    ds = cval.dataset()
+    # create your dataset
+    ds_id = ds.create()
+    print(ds_id)
+    # update your dataset
+    update = ds.update(name='any')
+    print('', update)
+    # watch changes
+    get = ds.get()
+    print(get)
+    # also you can use dataset_id for watch changes
+    get = ds.get(ds_id)
+    print(get)
+    # get all datasets
+    print(ds.get_all())
```

### Comparing `cval-lib-0.0.2.8/cval_lib/examples/embeddings.py` & `cval-lib-0.0.2.9/cval_lib/examples/embeddings.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-"""
-Introducing CVAL Rest API, a powerful tool for AI developers in the computer vision field.
-Our service combines the concepts of human-in-the-loop and active learning to improve the quality of
-your models and minimize annotation costs for classification, detection, and segmentation cases.
-
-With CVAL, you can iteratively improve your models by following our active learning loop.
-First, manually or semi-automatically annotate a random set of images.
-Next, train your model and use uncertainty and diversity methods to score the remaining images for annotation.
-Then, manually or semi-automatically annotate the images marked as more confident to increase the accuracy of the model.
-Repeat this process until you achieve an acceptable quality of the model.
-
-Our service makes it easy to implement this workflow and improve your models quickly and efficiently.
-Try our demo notebook to see how CVAL can revolutionize your computer vision projects.
-
-To obtain a client_api_key, please send a request to k.suhorukov@digital-quarters.com
-"""
-
-if __name__ == '__main__':
-    from random import random
-    import uuid
-
-    from cval_lib.connection import CVALConnection
-    from cval_lib.models.embedding import ImageEmbeddingModel
-
-    img_id_1 = str(uuid.uuid4().hex)
-    img_id_2 = str(uuid.uuid4().hex)
-
-    embeddings = [
-        ImageEmbeddingModel(id=img_id_1, image_embedding=list(map(lambda x: random(), range(1000)))),
-        ImageEmbeddingModel(id=img_id_2, image_embedding=list(map(lambda x: random(), range(1000)))),
-    ]
-
-    print(embeddings)
-    user_api_key = 'USER_API_KEY'
-    cval = CVALConnection(user_api_key)
-    ds = cval.dataset()
-    ds.create()
-    emb = cval.embedding("ID", 'training')
-    emb.upload_many(embeddings)
-    ds.embedding(type_of_dataset='training').get_many()
-    print(emb.get_many())
+"""
+Introducing CVAL Rest API, a powerful tool for AI developers in the computer vision field.
+Our service combines the concepts of human-in-the-loop and active learning to improve the quality of
+your models and minimize annotation costs for classification, detection, and segmentation cases.
+
+With CVAL, you can iteratively improve your models by following our active learning loop.
+First, manually or semi-automatically annotate a random set of images.
+Next, train your model and use uncertainty and diversity methods to score the remaining images for annotation.
+Then, manually or semi-automatically annotate the images marked as more confident to increase the accuracy of the model.
+Repeat this process until you achieve an acceptable quality of the model.
+
+Our service makes it easy to implement this workflow and improve your models quickly and efficiently.
+Try our demo notebook to see how CVAL can revolutionize your computer vision projects.
+
+To obtain a client_api_key, please send a request to k.suhorukov@digital-quarters.com
+"""
+
+if __name__ == '__main__':
+    from random import random
+    import uuid
+
+    from cval_lib.connection import CVALConnection
+    from cval_lib.models.embedding import ImageEmbeddingModel
+
+    img_id_1 = str(uuid.uuid4().hex)
+    img_id_2 = str(uuid.uuid4().hex)
+
+    embeddings = [
+        ImageEmbeddingModel(id=img_id_1, image_embedding=list(map(lambda x: random(), range(1000)))),
+        ImageEmbeddingModel(id=img_id_2, image_embedding=list(map(lambda x: random(), range(1000)))),
+    ]
+
+    print(embeddings)
+    user_api_key = 'USER_API_KEY'
+    cval = CVALConnection(user_api_key)
+    ds = cval.dataset()
+    ds.create()
+    emb = cval.embedding("ID", 'training')
+    emb.upload_many(embeddings)
+    ds.embedding(type_of_dataset='training').get_many()
+    print(emb.get_many())
```

### Comparing `cval-lib-0.0.2.8/cval_lib/examples/monkey_patch.py` & `cval-lib-0.0.2.9/cval_lib/examples/result.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,24 @@
-"""
-Introducing CVAL Rest API, a powerful tool for AI developers in the computer vision field.
-Our service combines the concepts of human-in-the-loop and active learning to improve the quality of
-your models and minimize annotation costs for classification, detection, and segmentation cases.
-
-With CVAL, you can iteratively improve your models by following our active learning loop.
-First, manually or semi-automatically annotate a random set of images.
-Next, train your model and use uncertainty and diversity methods to score the remaining images for annotation.
-Then, manually or semi-automatically annotate the images marked as more confident to increase the accuracy of the model.
-Repeat this process until you achieve an acceptable quality of the model.
-
-Our service makes it easy to implement this workflow and improve your models quickly and efficiently.
-Try our demo notebook to see how CVAL can revolutionize your computer vision projects.
-
-To obtain a client_api_key, please send a request to k.suhorukov@digital-quarters.com
-"""
-
-
-if __name__ == '__main__':
-    from cval_lib.connection import CVALConnection
-    api_key = 'USER_API_KEY'
-    cval = CVALConnection(api_key)
-    ds = cval.dataset()
-    ds.create()
-    print(ds.result.get_many())
+"""
+Introducing CVAL Rest API, a powerful tool for AI developers in the computer vision field.
+Our service combines the concepts of human-in-the-loop and active learning to improve the quality of
+your models and minimize annotation costs for classification, detection, and segmentation cases.
+
+With CVAL, you can iteratively improve your models by following our active learning loop.
+First, manually or semi-automatically annotate a random set of images.
+Next, train your model and use uncertainty and diversity methods to score the remaining images for annotation.
+Then, manually or semi-automatically annotate the images marked as more confident to increase the accuracy of the model.
+Repeat this process until you achieve an acceptable quality of the model.
+
+Our service makes it easy to implement this workflow and improve your models quickly and efficiently.
+Try our demo notebook to see how CVAL can revolutionize your computer vision projects.
+
+To obtain a client_api_key, please send a request to k.suhorukov@digital-quarters.com
+"""
+
+
+if __name__ == '__main__':
+    from cval_lib.connection import CVALConnection
+    user_api_key = '11a6006a98793bb5086bbf6f6808dd6bd9a706a38ddb36c58a484991263e8535'
+    cval = CVALConnection(user_api_key)
+    print(cval.result().get('ecb8a52b-9bc0-4e56-a496-e69ce74cc0ec'))
+    print(cval.result().get(cval.result().get_many()[0].result_id))
```

### Comparing `cval-lib-0.0.2.8/cval_lib/examples/on_pemise.py` & `cval-lib-0.0.2.9/cval_lib/examples/on_pemise.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-"""
-Introducing CVAL Rest API, a powerful tool for AI developers in the computer vision field.
-Our service combines the concepts of human-in-the-loop and active learning to improve the quality of
-your models and minimize annotation costs for classification, detection, and segmentation cases.
-
-With CVAL, you can iteratively improve your models by following our active learning loop.
-First, manually or semi-automatically annotate a random set of images.
-Next, train your model and use uncertainty and diversity methods to score the remaining images for annotation.
-Then, manually or semi-automatically annotate the images marked as more confident to increase the accuracy of the model.
-Repeat this process until you achieve an acceptable quality of the model.
-
-Our service makes it easy to implement this workflow and improve your models quickly and efficiently.
-Try our demo notebook to see how CVAL can revolutionize your computer vision projects.
-
-To obtain a client_api_key, please send a request to k.suhorukov@digital-quarters.com
-"""
-
-if __name__ == '__main__':
-    import uuid
-    from random import random
-
-    from cval_lib.connection import CVALConnection
-    from cval_lib.models.detection import DetectionSamplingOnPremise, FramePrediction, BBoxScores
-
-    frames_predictions = list(
-        map(
-            lambda x: FramePrediction(
-                frame_id=str(uuid.uuid4().hex),
-                predictions=list(map(lambda _: BBoxScores(category_id=str(uuid.uuid4()), score=random()), range(100)))
-            ),
-            range(100)
-        )
-    )
-
-    print(frames_predictions)
-
-    request = DetectionSamplingOnPremise(
-        num_of_samples=200,
-        bbox_selection_policy='min',
-        selection_strategy='margin',
-        sort_strategy='ascending',
-        frames=frames_predictions,
-    )
-    api_key = '11a6006a98793bb5086bbf6f6808dd6bd9a706a38ddb36c58a484991263e8535'
-    cval = CVALConnection(api_key)
-    detection = cval.detection()
-    print(detection.on_premise_sampling(request))
+"""
+Introducing CVAL Rest API, a powerful tool for AI developers in the computer vision field.
+Our service combines the concepts of human-in-the-loop and active learning to improve the quality of
+your models and minimize annotation costs for classification, detection, and segmentation cases.
+
+With CVAL, you can iteratively improve your models by following our active learning loop.
+First, manually or semi-automatically annotate a random set of images.
+Next, train your model and use uncertainty and diversity methods to score the remaining images for annotation.
+Then, manually or semi-automatically annotate the images marked as more confident to increase the accuracy of the model.
+Repeat this process until you achieve an acceptable quality of the model.
+
+Our service makes it easy to implement this workflow and improve your models quickly and efficiently.
+Try our demo notebook to see how CVAL can revolutionize your computer vision projects.
+
+To obtain a client_api_key, please send a request to k.suhorukov@digital-quarters.com
+"""
+
+if __name__ == '__main__':
+    import uuid
+    from random import random
+
+    from cval_lib.connection import CVALConnection
+    from cval_lib.models.detection import DetectionSamplingOnPremise, FramePrediction, BBoxScores
+
+    frames_predictions = list(
+        map(
+            lambda x: FramePrediction(
+                frame_id=str(uuid.uuid4().hex),
+                predictions=list(map(lambda _: BBoxScores(category_id=str(uuid.uuid4()), score=random()), range(100)))
+            ),
+            range(100)
+        )
+    )
+
+    print(frames_predictions)
+
+    request = DetectionSamplingOnPremise(
+        num_of_samples=200,
+        bbox_selection_policy='min',
+        selection_strategy='margin',
+        sort_strategy='ascending',
+        frames=frames_predictions,
+    )
+    api_key = '11a6006a98793bb5086bbf6f6808dd6bd9a706a38ddb36c58a484991263e8535'
+    cval = CVALConnection(api_key)
+    detection = cval.detection()
+    print(detection.on_premise_sampling(request))
```

### Comparing `cval-lib-0.0.2.8/cval_lib/examples/polling.py` & `cval-lib-0.0.2.9/cval_lib/examples/polling.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-"""
-Introducing CVAL Rest API, a powerful tool for AI developers in the computer vision field.
-Our service combines the concepts of human-in-the-loop and active learning to improve the quality of
-your models and minimize annotation costs for classification, detection, and segmentation cases.
-
-With CVAL, you can iteratively improve your models by following our active learning loop.
-First, manually or semi-automatically annotate a random set of images.
-Next, train your model and use uncertainty and diversity methods to score the remaining images for annotation.
-Then, manually or semi-automatically annotate the images marked as more confident to increase the accuracy of the model.
-Repeat this process until you achieve an acceptable quality of the model.
-
-Our service makes it easy to implement this workflow and improve your models quickly and efficiently.
-Try our demo notebook to see how CVAL can revolutionize your computer vision projects.
-
-To obtain a client_api_key, please send a request to k.suhorukov@digital-quarters.com
-"""
-
-if __name__ == '__main__':
-    import uuid
-    from random import random
-    from time import sleep
-
-    from cval_lib.connection import CVALConnection
-    from cval_lib.models.detection import DetectionSamplingOnPremise, FramePrediction, BBoxScores
-
-    frames_predictions = list(
-            map(
-                lambda x: FramePrediction(
-                    frame_id=str(uuid.uuid4().hex),
-                    predictions=list(
-                        map(
-                            lambda _: BBoxScores(category_id=str(uuid.uuid4()), score=random()),
-                            range(10000)
-                        ),
-                    )
-                ),
-                range(10000)
-            )
-        )
-
-    request = DetectionSamplingOnPremise(
-            num_of_samples=200,
-            bbox_selection_policy='min',
-            selection_strategy='margin',
-            sort_strategy='ascending',
-            frames=frames_predictions,
-        )
-    user_api_key = '11a6006a98793bb5086bbf6f6808dd6bd9a706a38ddb36c58a484991263e8535'
-    cval = CVALConnection(user_api_key)
-    emb = cval.detection()
-    result = None
-    sleep_sec = 1
-
-    while result is None:
-        result = emb.result.get()
-        print(f'Polling... {sleep_sec} s')
-        sleep(sleep_sec)
-        sleep_sec *= 2
-    print(result)
+"""
+Introducing CVAL Rest API, a powerful tool for AI developers in the computer vision field.
+Our service combines the concepts of human-in-the-loop and active learning to improve the quality of
+your models and minimize annotation costs for classification, detection, and segmentation cases.
+
+With CVAL, you can iteratively improve your models by following our active learning loop.
+First, manually or semi-automatically annotate a random set of images.
+Next, train your model and use uncertainty and diversity methods to score the remaining images for annotation.
+Then, manually or semi-automatically annotate the images marked as more confident to increase the accuracy of the model.
+Repeat this process until you achieve an acceptable quality of the model.
+
+Our service makes it easy to implement this workflow and improve your models quickly and efficiently.
+Try our demo notebook to see how CVAL can revolutionize your computer vision projects.
+
+To obtain a client_api_key, please send a request to k.suhorukov@digital-quarters.com
+"""
+
+if __name__ == '__main__':
+    import uuid
+    from random import random
+    from time import sleep
+
+    from cval_lib.connection import CVALConnection
+    from cval_lib.models.detection import DetectionSamplingOnPremise, FramePrediction, BBoxScores
+
+    frames_predictions = list(
+            map(
+                lambda x: FramePrediction(
+                    frame_id=str(uuid.uuid4().hex),
+                    predictions=list(
+                        map(
+                            lambda _: BBoxScores(category_id=str(uuid.uuid4()), score=random()),
+                            range(10000)
+                        ),
+                    )
+                ),
+                range(10000)
+            )
+        )
+
+    request = DetectionSamplingOnPremise(
+            num_of_samples=200,
+            bbox_selection_policy='min',
+            selection_strategy='margin',
+            sort_strategy='ascending',
+            frames=frames_predictions,
+        )
+    user_api_key = '11a6006a98793bb5086bbf6f6808dd6bd9a706a38ddb36c58a484991263e8535'
+    cval = CVALConnection(user_api_key)
+    emb = cval.detection()
+    result = None
+    sleep_sec = 1
+
+    while result is None:
+        result = emb.result.get()
+        print(f'Polling... {sleep_sec} s')
+        sleep(sleep_sec)
+        sleep_sec *= 2
+    print(result)
```

### Comparing `cval-lib-0.0.2.8/cval_lib/examples/result.py` & `cval-lib-0.0.2.9/cval_lib/examples/monkey_patch.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,25 @@
-"""
-Introducing CVAL Rest API, a powerful tool for AI developers in the computer vision field.
-Our service combines the concepts of human-in-the-loop and active learning to improve the quality of
-your models and minimize annotation costs for classification, detection, and segmentation cases.
-
-With CVAL, you can iteratively improve your models by following our active learning loop.
-First, manually or semi-automatically annotate a random set of images.
-Next, train your model and use uncertainty and diversity methods to score the remaining images for annotation.
-Then, manually or semi-automatically annotate the images marked as more confident to increase the accuracy of the model.
-Repeat this process until you achieve an acceptable quality of the model.
-
-Our service makes it easy to implement this workflow and improve your models quickly and efficiently.
-Try our demo notebook to see how CVAL can revolutionize your computer vision projects.
-
-To obtain a client_api_key, please send a request to k.suhorukov@digital-quarters.com
-"""
-
-
-if __name__ == '__main__':
-    from cval_lib.connection import CVALConnection
-    user_api_key = '11a6006a98793bb5086bbf6f6808dd6bd9a706a38ddb36c58a484991263e8535'
-    cval = CVALConnection(user_api_key)
-    print(cval.result().get('ecb8a52b-9bc0-4e56-a496-e69ce74cc0ec'))
-    print(cval.result().get(cval.result().get_many()[0].task_id))
+"""
+Introducing CVAL Rest API, a powerful tool for AI developers in the computer vision field.
+Our service combines the concepts of human-in-the-loop and active learning to improve the quality of
+your models and minimize annotation costs for classification, detection, and segmentation cases.
+
+With CVAL, you can iteratively improve your models by following our active learning loop.
+First, manually or semi-automatically annotate a random set of images.
+Next, train your model and use uncertainty and diversity methods to score the remaining images for annotation.
+Then, manually or semi-automatically annotate the images marked as more confident to increase the accuracy of the model.
+Repeat this process until you achieve an acceptable quality of the model.
+
+Our service makes it easy to implement this workflow and improve your models quickly and efficiently.
+Try our demo notebook to see how CVAL can revolutionize your computer vision projects.
+
+To obtain a client_api_key, please send a request to k.suhorukov@digital-quarters.com
+"""
+
+
+if __name__ == '__main__':
+    from cval_lib.connection import CVALConnection
+    api_key = 'USER_API_KEY'
+    cval = CVALConnection(api_key)
+    ds = cval.dataset()
+    ds.create()
+    print(ds.result.get_many())
```

### Comparing `cval-lib-0.0.2.8/cval_lib/handlers/__async.py` & `cval-lib-0.0.2.9/cval_lib/handlers/__async.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-"""
-Introducing CVAL Rest API, a powerful tool for AI developers in the computer vision field.
-Our service combines the concepts of human-in-the-loop and active learning to improve the quality of
-your models and minimize annotation costs for classification, detection, and segmentation cases.
-
-With CVAL, you can iteratively improve your models by following our active learning loop.
-First, manually or semi-automatically annotate a random set of images.
-Next, train your model and use uncertainty and diversity methods to score the remaining images for annotation.
-Then, manually or semi-automatically annotate the images marked as more confident to increase the accuracy of the model.
-Repeat this process until you achieve an acceptable quality of the model.
-
-Our service makes it easy to implement this workflow and improve your models quickly and efficiently.
-Try our demo notebook to see how CVAL can revolutionize your computer vision projects.
-
-To obtain a client_api_key, please send a request to k.suhorukov@digital-quarters.com
-"""
-
-import asyncio
-
-
-def asyncio_runner(func, *args, **kwargs):
-    loop = asyncio.new_event_loop()
-    asyncio.set_event_loop(loop)
-    res = loop.run_until_complete(func(*args, *kwargs))
-    loop.close()
-    return res
+"""
+Introducing CVAL Rest API, a powerful tool for AI developers in the computer vision field.
+Our service combines the concepts of human-in-the-loop and active learning to improve the quality of
+your models and minimize annotation costs for classification, detection, and segmentation cases.
+
+With CVAL, you can iteratively improve your models by following our active learning loop.
+First, manually or semi-automatically annotate a random set of images.
+Next, train your model and use uncertainty and diversity methods to score the remaining images for annotation.
+Then, manually or semi-automatically annotate the images marked as more confident to increase the accuracy of the model.
+Repeat this process until you achieve an acceptable quality of the model.
+
+Our service makes it easy to implement this workflow and improve your models quickly and efficiently.
+Try our demo notebook to see how CVAL can revolutionize your computer vision projects.
+
+To obtain a client_api_key, please send a request to k.suhorukov@digital-quarters.com
+"""
+
+import asyncio
+
+
+def asyncio_runner(func, *args, **kwargs):
+    loop = asyncio.new_event_loop()
+    asyncio.set_event_loop(loop)
+    res = loop.run_until_complete(func(*args, *kwargs))
+    loop.close()
+    return res
```

### Comparing `cval-lib-0.0.2.8/cval_lib/handlers/dataset.py` & `cval-lib-0.0.2.9/cval_lib/handlers/dataset.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,127 +1,127 @@
-"""
-Introducing CVAL Rest API, a powerful tool for AI developers in the computer vision field.
-Our service combines the concepts of human-in-the-loop and active learning to improve the quality of
-your models and minimize annotation costs for classification, detection, and segmentation cases.
-
-With CVAL, you can iteratively improve your models by following our active learning loop.
-First, manually or semi-automatically annotate a random set of images.
-Next, train your model and use uncertainty and diversity methods to score the remaining images for annotation.
-Then, manually or semi-automatically annotate the images marked as more confident to increase the accuracy of the model.
-Repeat this process until you achieve an acceptable quality of the model.
-
-Our service makes it easy to implement this workflow and improve your models quickly and efficiently.
-Try our demo notebook to see how CVAL can revolutionize your computer vision projects.
-
-To obtain a client_api_key, please send a request to k.suhorukov@digital-quarters.com
-"""
-
-from typing import List
-
-from requests import Session
-
-from cval_lib.configs.main_config import MainConfig
-from cval_lib.handlers._abstract_handler import AbstractHandler
-from cval_lib.handlers.detection import Detection
-from cval_lib.handlers.embedding import Embedding
-from cval_lib.handlers.result import Result
-from cval_lib.models.dataset import DatasetModel, DatasetResponse
-
-
-class Dataset(AbstractHandler):
-    """
-    Within the framework of the created system,
-    datasets are spaces in which data for machine learning is stored.
-    Creating a dataset is similar to creating a folder.
-    """
-    def __init__(self, session: Session):
-        self.dataset_request = DatasetModel()
-        self.route = f'{MainConfig().main_url}/dataset'
-        self.dataset_id = None
-        self.result = Result(session)
-        self._embedding = Embedding(session, _is_not_second=False)
-        self.embedding = self._embedding.monkey_patch_url
-        self.detection = Detection(session)
-        super().__init__(session)
-
-    def __repr__(self):
-        return f'<dataset {self.dataset_id}>'
-
-    def _construct_request(self, name: str, description: str):
-        self.dataset_request = DatasetModel()
-        if name is not None:
-            self.dataset_request.dataset_name = name
-        if description is not None:
-            self.dataset_request.dataset_description = description
-
-    def create(
-            self,
-            name: str = None,
-            description: str = None,
-    ) -> str:
-        """
-        this method creates a dataset
-        :param name: the name of dataset
-        :param description: the name of dataset
-        :return: id of dataset (dataset_id)
-        """
-        self._construct_request(name, description)
-        self._post(url=self.route, json=self.dataset_request.dict())
-        self.dataset_id = self.send().json().get('dataset_id')
-        self._embedding.dataset_id = self.dataset_id
-        return self.dataset_id
-
-    def update(
-            self,
-            dataset_id: str = None,
-            name: str = None,
-            description: str = None,
-    ) -> DatasetModel:
-        """
-        this method updates a dataset
-        :param dataset_id: id of dataset
-        :param name: the name of dataset
-        :param description: the description of dataset
-        :return: DatasetResponse model with updates
-        """
-        dataset_id = self.set_dataset_id(dataset_id)
-        self._construct_request(name, description)
-        self._put(url=self.route+f'/{dataset_id}', json=self.dataset_request.dict(), )
-        self.dataset_request = self.send().json()
-        return self.dataset_request
-
-    def set_dataset_id(self, dataset_id: str = None):
-        if dataset_id is None:
-            dataset_id = self.dataset_id
-        self.dataset_id = dataset_id
-        if self.dataset_id is None:
-            raise ValueError('dataset_id cannot be None')
-        self._embedding.dataset_id = dataset_id
-        return self.dataset_id
-
-    def get(
-            self,
-            dataset_id: str = None,
-    ) -> DatasetModel:
-        """
-        this method returns a dataset name and description by dataset_id
-        :param dataset_id: id of dataset
-        :return: DatasetResponse model with updates
-        """
-        dataset_id = self.set_dataset_id(dataset_id)
-        self._get(url=self.route+f'/{dataset_id}')
-        return DatasetModel.parse_obj(self.send().json())
-
-    def get_all(
-            self,
-            name: str = None,
-            description: str = None,
-    ) -> List[DatasetResponse]:
-        """
-        this method returns a dataset name and description by dataset_id
-        :param name: the name of dataset. regexp
-        :param description: the description of dataset. regexp
-        :return: DatasetResponse model with updates
-        """
-        self._construct_request(name, description)
-        self._get(url=self.route+'s/all', params=self.dataset_request.dict())
-        return [DatasetResponse.parse_obj(i) for i in self.send().json()]
+"""
+Introducing CVAL Rest API, a powerful tool for AI developers in the computer vision field.
+Our service combines the concepts of human-in-the-loop and active learning to improve the quality of
+your models and minimize annotation costs for classification, detection, and segmentation cases.
+
+With CVAL, you can iteratively improve your models by following our active learning loop.
+First, manually or semi-automatically annotate a random set of images.
+Next, train your model and use uncertainty and diversity methods to score the remaining images for annotation.
+Then, manually or semi-automatically annotate the images marked as more confident to increase the accuracy of the model.
+Repeat this process until you achieve an acceptable quality of the model.
+
+Our service makes it easy to implement this workflow and improve your models quickly and efficiently.
+Try our demo notebook to see how CVAL can revolutionize your computer vision projects.
+
+To obtain a client_api_key, please send a request to k.suhorukov@digital-quarters.com
+"""
+
+from typing import List
+
+from requests import Session
+
+from cval_lib.configs.main_config import MainConfig
+from cval_lib.handlers._abstract_handler import AbstractHandler
+from cval_lib.handlers.detection import Detection
+from cval_lib.handlers.embedding import Embedding
+from cval_lib.handlers.result import Result
+from cval_lib.models.dataset import DatasetModel, DatasetResponse
+
+
+class Dataset(AbstractHandler):
+    """
+    Within the framework of the created system,
+    datasets are spaces in which data for machine learning is stored.
+    Creating a dataset is similar to creating a folder.
+    """
+    def __init__(self, session: Session):
+        self.dataset_request = DatasetModel()
+        self.route = f'{MainConfig().main_url}/dataset'
+        self.dataset_id = None
+        self.result = Result(session)
+        self._embedding = Embedding(session, _is_not_second=False)
+        self.embedding = self._embedding.monkey_patch_url
+        self.detection = Detection(session)
+        super().__init__(session)
+
+    def __repr__(self):
+        return f'<dataset {self.dataset_id}>'
+
+    def _construct_request(self, name: str, description: str):
+        self.dataset_request = DatasetModel()
+        if name is not None:
+            self.dataset_request.dataset_name = name
+        if description is not None:
+            self.dataset_request.dataset_description = description
+
+    def create(
+            self,
+            name: str = None,
+            description: str = None,
+    ) -> str:
+        """
+        this method creates a dataset
+        :param name: the name of dataset
+        :param description: the name of dataset
+        :return: id of dataset (dataset_id)
+        """
+        self._construct_request(name, description)
+        self._post(url=self.route, json=self.dataset_request.dict())
+        self.dataset_id = self.send().json().get('dataset_id')
+        self._embedding.dataset_id = self.dataset_id
+        return self.dataset_id
+
+    def update(
+            self,
+            dataset_id: str = None,
+            name: str = None,
+            description: str = None,
+    ) -> DatasetModel:
+        """
+        this method updates a dataset
+        :param dataset_id: id of dataset
+        :param name: the name of dataset
+        :param description: the description of dataset
+        :return: DatasetResponse model with updates
+        """
+        dataset_id = self.set_dataset_id(dataset_id)
+        self._construct_request(name, description)
+        self._put(url=self.route+f'/{dataset_id}', json=self.dataset_request.dict(), )
+        self.dataset_request = self.send().json()
+        return self.dataset_request
+
+    def set_dataset_id(self, dataset_id: str = None):
+        if dataset_id is None:
+            dataset_id = self.dataset_id
+        self.dataset_id = dataset_id
+        if self.dataset_id is None:
+            raise ValueError('dataset_id cannot be None')
+        self._embedding.dataset_id = dataset_id
+        return self.dataset_id
+
+    def get(
+            self,
+            dataset_id: str = None,
+    ) -> 'DatasetModel':
+        """
+        this method returns a dataset name and description by dataset_id
+        :param dataset_id: id of dataset
+        :return: DatasetResponse model with updates
+        """
+        dataset_id = self.set_dataset_id(dataset_id)
+        self._get(url=self.route+f'/{dataset_id}')
+        return DatasetModel.parse_obj(self.send().json())
+
+    def get_all(
+            self,
+            name: str = None,
+            description: str = None,
+    ) -> List['DatasetResponse']:
+        """
+        this method returns a dataset name and description by dataset_id
+        :param name: the name of dataset. regexp
+        :param description: the description of dataset. regexp
+        :return: DatasetResponse model with updates
+        """
+        self._construct_request(name, description)
+        self._get(url=self.route+'s/all', params=self.dataset_request.dict())
+        return [DatasetResponse.parse_obj(i) for i in self.send().json()]
```

### Comparing `cval-lib-0.0.2.8/cval_lib/handlers/embedding.py` & `cval-lib-0.0.2.9/cval_lib/handlers/embedding.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,115 +1,115 @@
-"""
-Introducing CVAL Rest API, a powerful tool for AI developers in the computer vision field.
-Our service combines the concepts of human-in-the-loop and active learning to improve the quality of
-your models and minimize annotation costs for classification, detection, and segmentation cases.
-
-With CVAL, you can iteratively improve your models by following our active learning loop.
-First, manually or semi-automatically annotate a random set of images.
-Next, train your model and use uncertainty and diversity methods to score the remaining images for annotation.
-Then, manually or semi-automatically annotate the images marked as more confident to increase the accuracy of the model.
-Repeat this process until you achieve an acceptable quality of the model.
-
-Our service makes it easy to implement this workflow and improve your models quickly and efficiently.
-Try our demo notebook to see how CVAL can revolutionize your computer vision projects.
-
-To obtain a client_api_key, please send a request to k.suhorukov@digital-quarters.com
-"""
-
-from typing import List
-from requests import Session, Response
-
-from cval_lib.configs.main_config import MainConfig
-from cval_lib.handlers._abstract_handler import AbstractHandler
-from cval_lib.models.embedding import ImageEmbeddingModel
-
-
-class Embedding(AbstractHandler):
-    """
-    Embeddings are vector representations of images
-    obtained using pytorch or any other library
-    """
-    def __init__(
-            self,
-            session: Session,
-            dataset_id: str = None,
-            type_of_dataset: str = None,
-            _is_not_second=True
-    ):
-        if _is_not_second and dataset_id is None:
-            raise ValueError('dataset_id must be not None')
-        if _is_not_second and type_of_dataset is None:
-            raise ValueError('type_of_dataset must be not None')
-        self.dataset_id = dataset_id
-        self.type_of_dataset = type_of_dataset
-        self.route = f'{MainConfig().main_url}/dataset/{dataset_id}/{type_of_dataset}/'
-        super().__init__(session)
-
-    def monkey_patch_url(self, type_of_dataset: str, ) -> None:
-        self.route = f'{MainConfig().main_url}/dataset/{self.dataset_id}/{type_of_dataset}/'
-        return self
-
-    def get_many(self, start_limit: int = 0, stop_limit: int = 1000) -> List[ImageEmbeddingModel]:
-        """
-        :param start_limit: upper limit of items
-        :param stop_limit: lower limit of items
-        :return: List[ImageEmbeddingModel]
-        """
-        self._get(f'{MainConfig.main_url}/dataset/{self.dataset_id}/{self.type_of_dataset}/embeddings', params={'start_limit': start_limit, 'stop_limit': stop_limit})
-        return [ImageEmbeddingModel.parse_obj(i) for i in self.send().json()]
-
-    def get_by_id(self, embedding_id: str, ) -> [ImageEmbeddingModel]:
-        """
-        :param embedding_id: id of embedding
-        :return: ImageEmbeddingModel
-        """
-        self._get(self.route + f'embedding/{embedding_id}')
-        return ImageEmbeddingModel.parse_obj(self.send().json())
-
-    def upload_many(self, embeddings: List[ImageEmbeddingModel]) -> Response:
-        """
-        :param embeddings: List[ImageEmbeddingModel]
-        :return: Response, This method does not return anything useful to use, but performs an action
-        """
-        self._post(f'{MainConfig.main_url}/dataset/{self.dataset_id}/{self.type_of_dataset}/embeddings', json=[i.dict() for i in embeddings])
-        return self.send()
-
-    def upload_by_id(self, embedding_id: str, embedding: ImageEmbeddingModel) -> Response:
-        """
-        :param embedding: List[ImageEmbeddingModel]
-        :param embedding_id: id of embedding
-        :return: Response, This method does not return anything useful to use, but performs an action
-        """
-        self._post(self.route + f'/embedding/{embedding_id}', json=embedding.dict())
-        return self.send()
-
-    def update_many(self, embeddings: List[ImageEmbeddingModel]) -> Response:
-        """
-        :param embeddings: List[ImageEmbeddingModel]
-        :return: Response, This method does not return anything useful to use, but performs an action
-        """
-        self._put(self.route + f'embeddings', json=[i.dict() for i in embeddings])
-        return self.send()
-
-    def update_by_id(self, embedding_id: str, embedding: ImageEmbeddingModel) -> Response:
-        """
-        :param embedding: List[ImageEmbeddingModel]
-        :param embedding_id: id of embedding
-        :return: Response, This method does not return anything useful to use, but performs an action
-        """
-        self._put(self.route + f'embedding/{embedding_id}', json=embedding.dict())
-        return self.send()
-
-    def delete_all(self) -> Response:
-        """
-        :return: Response, This method does not return anything useful to use, but performs an action
-        """
-        self._delete(self.route + f'embeddings')
-        return self.send()
-
-    def delete_by_id(self, embedding_id: str) -> Response:
-        """
-        :param embedding_id: id of embedding
-        :return: Response, This method does not return anything useful to use, but performs an action
-        """
-        self._delete(self.route + f'embedding/{embedding_id}')
-        return self.send()
+"""
+Introducing CVAL Rest API, a powerful tool for AI developers in the computer vision field.
+Our service combines the concepts of human-in-the-loop and active learning to improve the quality of
+your models and minimize annotation costs for classification, detection, and segmentation cases.
+
+With CVAL, you can iteratively improve your models by following our active learning loop.
+First, manually or semi-automatically annotate a random set of images.
+Next, train your model and use uncertainty and diversity methods to score the remaining images for annotation.
+Then, manually or semi-automatically annotate the images marked as more confident to increase the accuracy of the model.
+Repeat this process until you achieve an acceptable quality of the model.
+
+Our service makes it easy to implement this workflow and improve your models quickly and efficiently.
+Try our demo notebook to see how CVAL can revolutionize your computer vision projects.
+
+To obtain a client_api_key, please send a request to k.suhorukov@digital-quarters.com
+"""
+
+from typing import List
+from requests import Session, Response
+
+from cval_lib.configs.main_config import MainConfig
+from cval_lib.handlers._abstract_handler import AbstractHandler
+from cval_lib.models.embedding import ImageEmbeddingModel
+
+
+class Embedding(AbstractHandler):
+    """
+    Embeddings are vector representations of images
+    obtained using pytorch or any other library
+    """
+    def __init__(
+            self,
+            session: Session,
+            dataset_id: str = None,
+            type_of_dataset: str = None,
+            _is_not_second=True
+    ):
+        if _is_not_second and dataset_id is None:
+            raise ValueError('dataset_id must be not None')
+        if _is_not_second and type_of_dataset is None:
+            raise ValueError('type_of_dataset must be not None')
+        self.dataset_id = dataset_id
+        self.type_of_dataset = type_of_dataset
+        self.route = f'{MainConfig().main_url}/dataset/{dataset_id}/{type_of_dataset}/'
+        super().__init__(session)
+
+    def monkey_patch_url(self, type_of_dataset: str, ) -> 'None':
+        self.route = f'{MainConfig().main_url}/dataset/{self.dataset_id}/{type_of_dataset}/'
+        return self
+
+    def get_many(self, start_limit: int = 0, stop_limit: int = 1000) -> List['ImageEmbeddingModel']:
+        """
+        :param start_limit: upper limit of items
+        :param stop_limit: lower limit of items
+        :return: List[ImageEmbeddingModel]
+        """
+        self._get(f'{MainConfig.main_url}/dataset/{self.dataset_id}/{self.type_of_dataset}/embeddings', params={'start_limit': start_limit, 'stop_limit': stop_limit})
+        return [ImageEmbeddingModel.parse_obj(i) for i in self.send().json()]
+
+    def get_by_id(self, embedding_id: str, ) -> 'ImageEmbeddingModel':
+        """
+        :param embedding_id: id of embedding
+        :return: ImageEmbeddingModel
+        """
+        self._get(self.route + f'embedding/{embedding_id}')
+        return ImageEmbeddingModel.parse_obj(self.send().json())
+
+    def upload_many(self, embeddings: List[ImageEmbeddingModel]) -> Response:
+        """
+        :param embeddings: List[ImageEmbeddingModel]
+        :return: Response, This method does not return anything useful to use, but performs an action
+        """
+        self._post(f'{MainConfig.main_url}/dataset/{self.dataset_id}/{self.type_of_dataset}/embeddings', json=[i.dict() for i in embeddings])
+        return self.send()
+
+    def upload_by_id(self, embedding_id: str, embedding: ImageEmbeddingModel) -> Response:
+        """
+        :param embedding: List[ImageEmbeddingModel]
+        :param embedding_id: id of embedding
+        :return: Response, This method does not return anything useful to use, but performs an action
+        """
+        self._post(self.route + f'/embedding/{embedding_id}', json=embedding.dict())
+        return self.send()
+
+    def update_many(self, embeddings: List['ImageEmbeddingModel']) -> Response:
+        """
+        :param embeddings: List[ImageEmbeddingModel]
+        :return: Response, This method does not return anything useful to use, but performs an action
+        """
+        self._put(self.route + f'embeddings', json=[i.dict() for i in embeddings])
+        return self.send()
+
+    def update_by_id(self, embedding_id: str, embedding: ImageEmbeddingModel) -> Response:
+        """
+        :param embedding: List[ImageEmbeddingModel]
+        :param embedding_id: id of embedding
+        :return: Response, This method does not return anything useful to use, but performs an action
+        """
+        self._put(self.route + f'embedding/{embedding_id}', json=embedding.dict())
+        return self.send()
+
+    def delete_all(self) -> Response:
+        """
+        :return: Response, This method does not return anything useful to use, but performs an action
+        """
+        self._delete(self.route + f'embeddings')
+        return self.send()
+
+    def delete_by_id(self, embedding_id: str) -> Response:
+        """
+        :param embedding_id: id of embedding
+        :return: Response, This method does not return anything useful to use, but performs an action
+        """
+        self._delete(self.route + f'embedding/{embedding_id}')
+        return self.send()
```

### Comparing `cval-lib-0.0.2.8/cval_lib/handlers/frames.py` & `cval-lib-0.0.2.9/cval_lib/handlers/frames.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-from typing import List
-
-from requests import Session
-
-from cval_lib.configs.main_config import MainConfig
-from cval_lib.handlers._abstract_handler import AbstractHandler
-
-
-class Frames(AbstractHandler):
-    def __init__(
-        self,
-        session: Session,
-        dataset_id: str = None,
-    ):
-        self.route = f'{MainConfig.main_url}/dataset/{dataset_id}/'
-        super().__init__(session)
-
-    def read_meta(self, type_of_dataset: str):
-        self._get(self.route + f'/{type_of_dataset}/frames/meta', stream=True)
-        return self.send()
-
-    @AbstractHandler.pos_val
-    def create_fb(self, *args, files: List[bytes]):
-        self._post(self.route, files=files)
-        return self.send()
+from typing import List
+
+from requests import Session
+
+from cval_lib.configs.main_config import MainConfig
+from cval_lib.handlers._abstract_handler import AbstractHandler
+
+
+class Frames(AbstractHandler):
+    def __init__(
+        self,
+        session: Session,
+        dataset_id: str = None,
+    ):
+        self.route = f'{MainConfig.main_url}/dataset/{dataset_id}/'
+        super().__init__(session)
+
+    def read_meta(self, type_of_dataset: str):
+        self._get(self.route + f'/{type_of_dataset}/frames/meta', stream=True)
+        return self.send()
+
+    @AbstractHandler.pos_val
+    def create_fb(self, *args, files: List[bytes]):
+        self._post(self.route, files=files)
+        return self.send()
```

### Comparing `cval-lib-0.0.2.8/cval_lib/handlers/result.py` & `cval-lib-0.0.2.9/cval_lib/handlers/result.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-"""
-Introducing CVAL Rest API, a powerful tool for AI developers in the computer vision field.
-Our service combines the concepts of human-in-the-loop and active learning to improve the quality of
-your models and minimize annotation costs for classification, detection, and segmentation cases.
-
-With CVAL, you can iteratively improve your models by following our active learning loop.
-First, manually or semi-automatically annotate a random set of images.
-Next, train your model and use uncertainty and diversity methods to score the remaining images for annotation.
-Then, manually or semi-automatically annotate the images marked as more confident to increase the accuracy of the model.
-Repeat this process until you achieve an acceptable quality of the model.
-
-Our service makes it easy to implement this workflow and improve your models quickly and efficiently.
-Try our demo notebook to see how CVAL can revolutionize your computer vision projects.
-
-To obtain a client_api_key, please send a request to k.suhorukov@digital-quarters.com
-"""
-
-from requests import Session
-
-from cval_lib.configs.main_config import MainConfig
-from cval_lib.handlers._abstract_handler import AbstractHandler
-from cval_lib.models.result import ResultResponse
-
-
-class Result(AbstractHandler):
-    """
-    The result is the entity in which the processing data is stored
-    """
-    def __init__(
-            self,
-            session: Session,
-    ):
-        self.route = f'{MainConfig.main_url}/result'
-        self.result_id = None
-        super().__init__(session)
-
-    def _set_result_id(self, result_id: str = None):
-        if result_id is None:
-            result_id = self.result_id
-        if result_id is None:
-            raise ValueError('task_id cannot be None')
-        self.result_id = result_id
-
-    def get(self, result_id: str = None) -> ResultResponse:
-        """
-        :param result_id: id of result
-        :return: ResultResponse
-        """
-        self._set_result_id(result_id)
-        self._get(self.route + f'/{self.result_id}')
-        return ResultResponse.parse_obj(self.send().json())
-
-    def get_many(self, dataset_id: str = None, limit=100, ):
-        """
-        :param dataset_id: id of dataset
-        :param limit: limit of returned objects
-        :return:
-        """
-        self._get(self.route + 's', params={'limit': limit, 'dataset_id': dataset_id})
-        return [ResultResponse.parse_obj(i) for i in self.send().json()]
+"""
+Introducing CVAL Rest API, a powerful tool for AI developers in the computer vision field.
+Our service combines the concepts of human-in-the-loop and active learning to improve the quality of
+your models and minimize annotation costs for classification, detection, and segmentation cases.
+
+With CVAL, you can iteratively improve your models by following our active learning loop.
+First, manually or semi-automatically annotate a random set of images.
+Next, train your model and use uncertainty and diversity methods to score the remaining images for annotation.
+Then, manually or semi-automatically annotate the images marked as more confident to increase the accuracy of the model.
+Repeat this process until you achieve an acceptable quality of the model.
+
+Our service makes it easy to implement this workflow and improve your models quickly and efficiently.
+Try our demo notebook to see how CVAL can revolutionize your computer vision projects.
+
+To obtain a client_api_key, please send a request to k.suhorukov@digital-quarters.com
+"""
+
+from requests import Session
+
+from cval_lib.configs.main_config import MainConfig
+from cval_lib.handlers._abstract_handler import AbstractHandler
+from cval_lib.models.result import ResultResponse
+
+
+class Result(AbstractHandler):
+    """
+    The result is the entity in which the processing data is stored
+    """
+    def __init__(
+            self,
+            session: Session,
+    ):
+        self.route = f'{MainConfig.main_url}/result'
+        self.result_id = None
+        super().__init__(session)
+
+    def _set_result_id(self, result_id: str = None):
+        if result_id is None:
+            result_id = self.result_id
+        if result_id is None:
+            raise ValueError('result_id cannot be None')
+        self.result_id = result_id
+
+    def get(self, result_id: str = None) -> ResultResponse:
+        """
+        :param result_id: id of result
+        :return: ResultResponse
+        """
+        self._set_result_id(result_id)
+        self._get(self.route + f'/{self.result_id}')
+        return ResultResponse.parse_obj(self.send().json())
+
+    def get_many(self, dataset_id: str = None, limit=100, ):
+        """
+        :param dataset_id: id of dataset
+        :param limit: limit of returned objects
+        :return:
+        """
+        self._get(self.route + 's', params={'limit': limit, 'dataset_id': dataset_id})
+        return [ResultResponse.parse_obj(i) for i in self.send().json()]
```

### Comparing `cval-lib-0.0.2.8/cval_lib/models/detection.py` & `cval-lib-0.0.2.9/cval_lib/models/detection.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,77 +1,77 @@
-"""
-Introducing CVAL Rest API, a powerful tool for AI developers in the computer vision field.
-Our service combines the concepts of human-in-the-loop and active learning to improve the quality of
-your models and minimize annotation costs for classification, detection, and segmentation cases.
-
-With CVAL, you can iteratively improve your models by following our active learning loop.
-First, manually or semi-automatically annotate a random set of images.
-Next, train your model and use uncertainty and diversity methods to score the remaining images for annotation.
-Then, manually or semi-automatically annotate the images marked as more confident to increase the accuracy of the model.
-Repeat this process until you achieve an acceptable quality of the model.
-
-Our service makes it easy to implement this workflow and improve your models quickly and efficiently.
-Try our demo notebook to see how CVAL can revolutionize your computer vision projects.
-
-To obtain a client_api_key, please send a request to k.suhorukov@digital-quarters.com
-"""
-from typing import List
-from pydantic import validator
-
-from pydantic import BaseModel, Field
-
-
-class BBoxScores(BaseModel):
-    """
-    :param category_id: id of the category in FramePrediction namespace
-    :param score: prediction of model on that bbox
-    """
-    category_id: str
-    score: float
-
-
-class FramePrediction(BaseModel):
-    """
-    :param frame_id: id of the frame
-    :param predictions: bbox scores
-    """
-    frame_id: str = Field(max_length=32)
-    predictions: List[BBoxScores]
-
-
-class DetectionSamplingOnPremise(BaseModel):
-    """
-    :param num_of_samples: absolute number of samples to select
-    :param bbox_selection_policy:
-    Which bounding box to select when there are multiple boxes on an image,
-    according to their confidence. Currently supports: min, max, mean
-    :selection_strategy: Currently supports: margin, least, ratio, entropy
-    :param frames: prediction for th picture and the bbox
-    :type frames: List[FramePrediction]
-    :raises ValueError if value not in allowed
-    """
-    num_of_samples: int
-    bbox_selection_policy: str
-    selection_strategy: str
-    sort_strategy: str
-    frames: List[FramePrediction]
-
-    @validator('bbox_selection_policy')
-    def validate_bbox_selection_policy(cls, value):
-        allowed = ['min', 'max', 'sum', 'mean']
-        if value not in allowed:
-            raise ValueError(f"allowed bbox_selection_policy = {allowed}")
-        return value
-
-    @validator('selection_strategy')
-    def validate_selection_strategy(cls, value):
-        allowed = 'margin,least,ratio,entropy,probability'.split(',')
-        if value not in allowed:
-            raise ValueError(f"allowed selection_strategy = {allowed}")
-        return value
-
-    @validator('sort_strategy')
-    def validate_sort_strategy(cls, value):
-        allowed = 'ascending,descending'.split(',')
-        if value not in allowed:
-            raise ValueError(f"allowed sort_strategy = {allowed}")
-        return value
+"""
+Introducing CVAL Rest API, a powerful tool for AI developers in the computer vision field.
+Our service combines the concepts of human-in-the-loop and active learning to improve the quality of
+your models and minimize annotation costs for classification, detection, and segmentation cases.
+
+With CVAL, you can iteratively improve your models by following our active learning loop.
+First, manually or semi-automatically annotate a random set of images.
+Next, train your model and use uncertainty and diversity methods to score the remaining images for annotation.
+Then, manually or semi-automatically annotate the images marked as more confident to increase the accuracy of the model.
+Repeat this process until you achieve an acceptable quality of the model.
+
+Our service makes it easy to implement this workflow and improve your models quickly and efficiently.
+Try our demo notebook to see how CVAL can revolutionize your computer vision projects.
+
+To obtain a client_api_key, please send a request to k.suhorukov@digital-quarters.com
+"""
+from typing import List
+from pydantic import validator
+
+from pydantic import BaseModel, Field
+
+
+class BBoxScores(BaseModel):
+    """
+    :param category_id: id of the category in FramePrediction namespace
+    :param score: prediction of model on that bbox
+    """
+    category_id: str
+    score: float
+
+
+class FramePrediction(BaseModel):
+    """
+    :param frame_id: id of the frame
+    :param predictions: bbox scores
+    """
+    frame_id: str = Field(max_length=32)
+    predictions: List[BBoxScores]
+
+
+class DetectionSamplingOnPremise(BaseModel):
+    """
+    :param num_of_samples: absolute number of samples to select
+    :param bbox_selection_policy:
+    Which bounding box to select when there are multiple boxes on an image,
+    according to their confidence. Currently supports: min, max, mean
+    :selection_strategy: Currently supports: margin, least, ratio, entropy
+    :param frames: prediction for th picture and the bbox
+    :type frames: List[FramePrediction]
+    :raises ValueError if value not in allowed
+    """
+    num_of_samples: int
+    bbox_selection_policy: str
+    selection_strategy: str
+    sort_strategy: str
+    frames: List[FramePrediction]
+
+    @validator('bbox_selection_policy')
+    def validate_bbox_selection_policy(cls, value):
+        allowed = ['min', 'max', 'sum', 'mean']
+        if value not in allowed:
+            raise ValueError(f"allowed bbox_selection_policy = {allowed}")
+        return value
+
+    @validator('selection_strategy')
+    def validate_selection_strategy(cls, value):
+        allowed = 'margin,least,ratio,entropy,probability'.split(',')
+        if value not in allowed:
+            raise ValueError(f"allowed selection_strategy = {allowed}")
+        return value
+
+    @validator('sort_strategy')
+    def validate_sort_strategy(cls, value):
+        allowed = 'ascending,descending'.split(',')
+        if value not in allowed:
+            raise ValueError(f"allowed sort_strategy = {allowed}")
+        return value
```

### Comparing `cval-lib-0.0.2.8/cval_lib/models/embedding.py` & `cval-lib-0.0.2.9/cval_lib/models/embedding.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-"""
-Introducing CVAL Rest API, a powerful tool for AI developers in the computer vision field.
-Our service combines the concepts of human-in-the-loop and active learning to improve the quality of
-your models and minimize annotation costs for classification, detection, and segmentation cases.
-
-With CVAL, you can iteratively improve your models by following our active learning loop.
-First, manually or semi-automatically annotate a random set of images.
-Next, train your model and use uncertainty and diversity methods to score the remaining images for annotation.
-Then, manually or semi-automatically annotate the images marked as more confident to increase the accuracy of the model.
-Repeat this process until you achieve an acceptable quality of the model.
-
-Our service makes it easy to implement this workflow and improve your models quickly and efficiently.
-Try our demo notebook to see how CVAL can revolutionize your computer vision projects.
-
-To obtain a client_api_key, please send a request to k.suhorukov@digital-quarters.com
-"""
-
-from typing import List
-
-from pydantic import BaseModel, Field
-
-
-class ImageEmbeddingModel(BaseModel):
-    """
-    Describes the embedding model
-    :param id: id of embedding
-    :type id: str
-    :param image_embedding: image embedding vector
-    :type image_embedding: List[float]
-    """
-    id: str = Field(max_length=32)
-    image_embedding: List[float]
-
+"""
+Introducing CVAL Rest API, a powerful tool for AI developers in the computer vision field.
+Our service combines the concepts of human-in-the-loop and active learning to improve the quality of
+your models and minimize annotation costs for classification, detection, and segmentation cases.
+
+With CVAL, you can iteratively improve your models by following our active learning loop.
+First, manually or semi-automatically annotate a random set of images.
+Next, train your model and use uncertainty and diversity methods to score the remaining images for annotation.
+Then, manually or semi-automatically annotate the images marked as more confident to increase the accuracy of the model.
+Repeat this process until you achieve an acceptable quality of the model.
+
+Our service makes it easy to implement this workflow and improve your models quickly and efficiently.
+Try our demo notebook to see how CVAL can revolutionize your computer vision projects.
+
+To obtain a client_api_key, please send a request to k.suhorukov@digital-quarters.com
+"""
+
+from typing import List
+
+from pydantic import BaseModel, Field
+
+
+class ImageEmbeddingModel(BaseModel):
+    """
+    Describes the embedding model
+    :param id: id of embedding
+    :type id: str
+    :param image_embedding: image embedding vector
+    :type image_embedding: List[float]
+    """
+    id: str = Field(max_length=32)
+    image_embedding: List[float]
+
```

### Comparing `cval-lib-0.0.2.8/cval_lib.egg-info/SOURCES.txt` & `cval-lib-0.0.2.9/cval_lib.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -31,8 +31,33 @@
 ./cval_lib/patterns/singleton.py
 cval_lib/__init__.py
 cval_lib/connection.py
 cval_lib.egg-info/PKG-INFO
 cval_lib.egg-info/SOURCES.txt
 cval_lib.egg-info/dependency_links.txt
 cval_lib.egg-info/requires.txt
-cval_lib.egg-info/top_level.txt
+cval_lib.egg-info/top_level.txt
+cval_lib/configs/__init__.py
+cval_lib/configs/main_config.py
+cval_lib/examples/__init__.py
+cval_lib/examples/dataset.py
+cval_lib/examples/embeddings.py
+cval_lib/examples/monkey_patch.py
+cval_lib/examples/on_pemise.py
+cval_lib/examples/polling.py
+cval_lib/examples/result.py
+cval_lib/handlers/__async.py
+cval_lib/handlers/__init__.py
+cval_lib/handlers/_abstract_handler.py
+cval_lib/handlers/dataset.py
+cval_lib/handlers/detection.py
+cval_lib/handlers/embedding.py
+cval_lib/handlers/frame.py
+cval_lib/handlers/frames.py
+cval_lib/handlers/result.py
+cval_lib/models/__init__.py
+cval_lib/models/dataset.py
+cval_lib/models/detection.py
+cval_lib/models/embedding.py
+cval_lib/models/result.py
+cval_lib/patterns/__init__.py
+cval_lib/patterns/singleton.py
```

