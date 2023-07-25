# Comparing `tmp/deciphon-0.8.1.tar.gz` & `tmp/deciphon-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deciphon-0.8.1.tar", max compression
+gzip compressed data, was "deciphon-0.9.0.tar", max compression
```

## Comparing `deciphon-0.8.1.tar` & `deciphon-0.9.0.tar`

### file list

```diff
@@ -1,30 +1,16 @@
--rw-r--r--   0        0        0     1063 2023-02-05 23:42:00.945231 deciphon-0.8.1/LICENSE
--rw-r--r--   0        0        0     2996 2023-02-08 11:19:00.538561 deciphon-0.8.1/README.md
--rw-r--r--   0        0        0        0 2023-02-05 23:50:26.348804 deciphon-0.8.1/deciphon/__init__.py
--rw-r--r--   0        0        0        0 2023-03-05 16:53:57.996737 deciphon-0.8.1/deciphon/api/__init__.py
--rw-r--r--   0        0        0     4356 2023-03-06 10:42:06.208901 deciphon-0.8.1/deciphon/api/api.py
--rw-r--r--   0        0        0     2215 2023-03-06 09:47:45.810524 deciphon-0.8.1/deciphon/api/cli.py
--rw-r--r--   0        0        0     2783 2023-05-11 11:29:23.733899 deciphon-0.8.1/deciphon/cli.py
--rw-r--r--   0        0        0      501 2023-02-10 13:02:37.810954 deciphon-0.8.1/deciphon/config.py
--rw-r--r--   0        0        0        0 2023-03-06 10:22:22.559435 deciphon-0.8.1/deciphon/daemon/__init__.py
--rw-r--r--   0        0        0      622 2023-03-06 10:24:39.743329 deciphon-0.8.1/deciphon/daemon/cli.py
--rw-r--r--   0        0        0     1691 2023-03-06 10:42:28.436070 deciphon-0.8.1/deciphon/daemon/pressd.py
--rw-r--r--   0        0        0     2718 2023-03-06 10:42:22.221451 deciphon-0.8.1/deciphon/daemon/scand.py
--rw-r--r--   0        0        0       72 2023-03-06 09:58:29.086811 deciphon-0.8.1/deciphon/dbfile.py
--rw-r--r--   0        0        0       84 2023-03-01 11:03:34.003201 deciphon-0.8.1/deciphon/errors.py
--rw-r--r--   0        0        0       91 2023-03-01 15:13:24.333208 deciphon-0.8.1/deciphon/filepath.py
--rw-r--r--   0        0        0      483 2023-03-01 11:08:40.980239 deciphon-0.8.1/deciphon/filetype.py
--rw-r--r--   0        0        0      157 2023-02-08 14:33:19.553381 deciphon-0.8.1/deciphon/fire_and_forget.py
--rw-r--r--   0        0        0      595 2023-04-30 03:27:38.496088 deciphon-0.8.1/deciphon/h3daemon.py
--rw-r--r--   0        0        0      196 2023-03-06 10:12:59.866043 deciphon-0.8.1/deciphon/hmmer_press.py
--rw-r--r--   0        0        0       76 2023-03-06 09:53:17.004469 deciphon-0.8.1/deciphon/hmmfile.py
--rw-r--r--   0        0        0      775 2023-02-13 10:15:16.068006 deciphon-0.8.1/deciphon/models.py
--rw-r--r--   0        0        0      522 2023-02-08 14:44:07.024041 deciphon-0.8.1/deciphon/percent.py
--rw-r--r--   0        0        0       69 2023-03-06 10:02:25.754663 deciphon-0.8.1/deciphon/press.py
--rw-r--r--   0        0        0      321 2023-03-06 10:33:28.705124 deciphon-0.8.1/deciphon/scan.py
--rw-r--r--   0        0        0     1929 2023-03-08 14:07:58.009142 deciphon-0.8.1/deciphon/seqfile.py
--rw-r--r--   0        0        0      670 2023-03-04 10:38:17.846292 deciphon-0.8.1/deciphon/service_exit.py
--rw-r--r--   0        0        0      157 2023-03-06 10:32:56.579299 deciphon-0.8.1/deciphon/snapfile.py
--rw-r--r--   0        0        0      556 2023-02-14 10:18:24.072041 deciphon-0.8.1/deciphon/storage.py
--rw-r--r--   0        0        0      720 2023-05-12 15:13:31.601084 deciphon-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     3761 1970-01-01 00:00:00.000000 deciphon-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-07-25 12:32:17.169247 deciphon-0.9.0/LICENSE
+-rw-r--r--   0        0        0     2996 2023-07-25 12:32:17.169247 deciphon-0.9.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-25 12:32:17.169247 deciphon-0.9.0/deciphon/__init__.py
+-rw-r--r--   0        0        0      483 2023-07-25 12:32:17.169247 deciphon-0.9.0/deciphon/catch_validation.py
+-rw-r--r--   0        0        0     4853 2023-07-25 12:32:17.169247 deciphon-0.9.0/deciphon/cli.py
+-rw-r--r--   0        0        0      430 2023-07-25 12:32:17.169247 deciphon-0.9.0/deciphon/filetype.py
+-rw-r--r--   0        0        0      248 2023-07-25 12:32:17.169247 deciphon-0.9.0/deciphon/gencode.py
+-rw-r--r--   0        0        0      680 2023-07-25 12:32:17.169247 deciphon-0.9.0/deciphon/h3daemon.py
+-rw-r--r--   0        0        0      213 2023-07-25 12:32:17.169247 deciphon-0.9.0/deciphon/hmmer_press.py
+-rw-r--r--   0        0        0      775 2023-07-25 12:32:17.169247 deciphon-0.9.0/deciphon/models.py
+-rw-r--r--   0        0        0       72 2023-07-25 12:32:17.169247 deciphon-0.9.0/deciphon/path_like.py
+-rw-r--r--   0        0        0      522 2023-07-25 12:32:17.169247 deciphon-0.9.0/deciphon/percent.py
+-rw-r--r--   0        0        0     1414 2023-07-25 12:32:17.169247 deciphon-0.9.0/deciphon/seq_file.py
+-rw-r--r--   0        0        0      670 2023-07-25 12:32:17.169247 deciphon-0.9.0/deciphon/service_exit.py
+-rw-r--r--   0        0        0      742 2023-07-25 12:32:17.169247 deciphon-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     3866 1970-01-01 00:00:00.000000 deciphon-0.9.0/PKG-INFO
```

### Comparing `deciphon-0.8.1/LICENSE` & `deciphon-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deciphon-0.8.1/README.md` & `deciphon-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `deciphon-0.8.1/deciphon/h3daemon.py` & `deciphon-0.9.0/deciphon/h3daemon.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from h3daemon.hmmfile import HMMFile as H3File
 from h3daemon.sched import SchedContext
 
-from deciphon.hmmfile import HMMFile
+from deciphon_core.hmmfile import HMMFile
 
 __all__ = ["H3Daemon"]
 
 
 class H3Daemon:
-    def __init__(self, hmmfile: HMMFile) -> None:
+    def __init__(self, hmmfile: HMMFile, stdout=None, stderr=None) -> None:
         self._hmmfile = hmmfile
-        self._sched_ctx = SchedContext(H3File(hmmfile.path))
+        h3file = H3File(hmmfile.path)
+        self._sched_ctx = SchedContext(h3file, stdout=stdout, stderr=stderr)
         self._port: int = -1
 
     @property
     def port(self):
         return self._port
 
     def __enter__(self):
```

### Comparing `deciphon-0.8.1/deciphon/models.py` & `deciphon-0.9.0/deciphon/models.py`

 * *Files identical despite different names*

### Comparing `deciphon-0.8.1/deciphon/percent.py` & `deciphon-0.9.0/deciphon/percent.py`

 * *Files identical despite different names*

### Comparing `deciphon-0.8.1/deciphon/service_exit.py` & `deciphon-0.9.0/deciphon/service_exit.py`

 * *Files identical despite different names*

### Comparing `deciphon-0.8.1/PKG-INFO` & `deciphon-0.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: deciphon
-Version: 0.8.1
+Version: 0.9.0
 Summary: Individually annotate long, error-prone nucleotide sequences into proteins
 License: MIT
 Author: Danilo Horta
-Author-email: danilo.horta@pm.me
-Requires-Python: >=3.10,<4.0
+Author-email: horta@ebi.ac.uk
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: blx
-Requires-Dist: cffi
-Requires-Dist: deciphon-core
-Requires-Dist: fasta-reader
-Requires-Dist: gmqtt
-Requires-Dist: h3daemon (>=0.13.3)
-Requires-Dist: hmmer
-Requires-Dist: ijson
-Requires-Dist: pydantic
-Requires-Dist: requests
-Requires-Dist: typer[all]
-Requires-Dist: uvloop
+Requires-Dist: cffi (>=1.15.1)
+Requires-Dist: deciphon-core (>=0.13.1)
+Requires-Dist: deciphon-snap (>=0.5.0)
+Requires-Dist: fasta-reader (>=3.0.1)
+Requires-Dist: h3daemon (>=0.13.4)
+Requires-Dist: hmmer (>=0.2.4)
+Requires-Dist: ijson (>=3.2.1)
+Requires-Dist: pydantic (>=2.0.3)
+Requires-Dist: tabulate (>=0.9.0)
+Requires-Dist: typer[all] (>=0.9.0)
 Description-Content-Type: text/markdown
 
 # Welcome to deciphon 👋
 
 > Individually annotate long, error-prone nucleotide sequences into proteins
 
 ### 🏠 [Homepage](https://github.com/EBI-Metagenomics/deciphon-py)
```

