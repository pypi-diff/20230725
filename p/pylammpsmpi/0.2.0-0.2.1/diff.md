# Comparing `tmp/pylammpsmpi-0.2.0.tar.gz` & `tmp/pylammpsmpi-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylammpsmpi-0.2.0.tar", last modified: Mon Jul 17 21:17:25 2023, max compression
+gzip compressed data, was "pylammpsmpi-0.2.1.tar", last modified: Mon Jul 24 23:50:23 2023, max compression
```

## Comparing `pylammpsmpi-0.2.0.tar` & `pylammpsmpi-0.2.1.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:17:25.476988 pylammpsmpi-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-07-17 21:17:22.000000 pylammpsmpi-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-17 21:17:22.000000 pylammpsmpi-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-17 21:17:25.476988 pylammpsmpi-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-07-17 21:17:22.000000 pylammpsmpi-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:17:25.476988 pylammpsmpi-0.2.0/pylammpsmpi/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-17 21:17:22.000000 pylammpsmpi-0.2.0/pylammpsmpi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-17 21:17:25.476988 pylammpsmpi-0.2.0/pylammpsmpi/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:17:25.476988 pylammpsmpi-0.2.0/pylammpsmpi/mpi/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 21:17:22.000000 pylammpsmpi-0.2.0/pylammpsmpi/mpi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13805 2023-07-17 21:17:22.000000 pylammpsmpi-0.2.0/pylammpsmpi/mpi/lmpmpi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:17:25.476988 pylammpsmpi-0.2.0/pylammpsmpi/wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 21:17:22.000000 pylammpsmpi-0.2.0/pylammpsmpi/wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14979 2023-07-17 21:17:22.000000 pylammpsmpi-0.2.0/pylammpsmpi/wrapper/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    20729 2023-07-17 21:17:22.000000 pylammpsmpi-0.2.0/pylammpsmpi/wrapper/concurrent.py
--rw-r--r--   0 runner    (1001) docker     (123)     6038 2023-07-17 21:17:22.000000 pylammpsmpi-0.2.0/pylammpsmpi/wrapper/extended.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:17:25.476988 pylammpsmpi-0.2.0/pylammpsmpi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-17 21:17:25.000000 pylammpsmpi-0.2.0/pylammpsmpi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-17 21:17:25.000000 pylammpsmpi-0.2.0/pylammpsmpi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 21:17:25.000000 pylammpsmpi-0.2.0/pylammpsmpi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-17 21:17:25.000000 pylammpsmpi-0.2.0/pylammpsmpi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-17 21:17:25.000000 pylammpsmpi-0.2.0/pylammpsmpi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-17 21:17:25.476988 pylammpsmpi-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-17 21:17:25.000000 pylammpsmpi-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:17:25.476988 pylammpsmpi-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-07-17 21:17:22.000000 pylammpsmpi-0.2.0/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-07-17 21:17:22.000000 pylammpsmpi-0.2.0/tests/test_concurrent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-07-17 21:17:22.000000 pylammpsmpi-0.2.0/tests/test_pylammpsmpi_local.py
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-07-17 21:17:22.000000 pylammpsmpi-0.2.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 23:50:23.133724 pylammpsmpi-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-07-24 23:50:19.000000 pylammpsmpi-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-24 23:50:19.000000 pylammpsmpi-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-24 23:50:23.133724 pylammpsmpi-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-07-24 23:50:19.000000 pylammpsmpi-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 23:50:23.133724 pylammpsmpi-0.2.1/pylammpsmpi/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-24 23:50:19.000000 pylammpsmpi-0.2.1/pylammpsmpi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-24 23:50:23.133724 pylammpsmpi-0.2.1/pylammpsmpi/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 23:50:23.129724 pylammpsmpi-0.2.1/pylammpsmpi/mpi/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 23:50:19.000000 pylammpsmpi-0.2.1/pylammpsmpi/mpi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13805 2023-07-24 23:50:19.000000 pylammpsmpi-0.2.1/pylammpsmpi/mpi/lmpmpi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 23:50:23.129724 pylammpsmpi-0.2.1/pylammpsmpi/wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 23:50:19.000000 pylammpsmpi-0.2.1/pylammpsmpi/wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26684 2023-07-24 23:50:19.000000 pylammpsmpi-0.2.1/pylammpsmpi/wrapper/ase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14979 2023-07-24 23:50:19.000000 pylammpsmpi-0.2.1/pylammpsmpi/wrapper/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20753 2023-07-24 23:50:19.000000 pylammpsmpi-0.2.1/pylammpsmpi/wrapper/concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-07-24 23:50:19.000000 pylammpsmpi-0.2.1/pylammpsmpi/wrapper/extended.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 23:50:23.129724 pylammpsmpi-0.2.1/pylammpsmpi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-24 23:50:23.000000 pylammpsmpi-0.2.1/pylammpsmpi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-24 23:50:23.000000 pylammpsmpi-0.2.1/pylammpsmpi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 23:50:23.000000 pylammpsmpi-0.2.1/pylammpsmpi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-24 23:50:23.000000 pylammpsmpi-0.2.1/pylammpsmpi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-24 23:50:23.000000 pylammpsmpi-0.2.1/pylammpsmpi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-24 23:50:23.133724 pylammpsmpi-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-24 23:50:22.000000 pylammpsmpi-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 23:50:23.133724 pylammpsmpi-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-07-24 23:50:19.000000 pylammpsmpi-0.2.1/tests/test_ase_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-07-24 23:50:19.000000 pylammpsmpi-0.2.1/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-07-24 23:50:19.000000 pylammpsmpi-0.2.1/tests/test_concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-07-24 23:50:19.000000 pylammpsmpi-0.2.1/tests/test_pylammpsmpi_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-07-24 23:50:19.000000 pylammpsmpi-0.2.1/versioneer.py
```

### Comparing `pylammpsmpi-0.2.0/LICENSE` & `pylammpsmpi-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pylammpsmpi-0.2.0/PKG-INFO` & `pylammpsmpi-0.2.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylammpsmpi
-Version: 0.2.0
+Version: 0.2.1
 Summary: Parallel Lammps Python interface
 Home-page: https://github.com/pyiron/pylammpsmpi
 Author: Jan Janssen
 Author-email: janssen@mpie.de
 License: BSD
 Keywords: lammps,mpi4py
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,10 +13,11 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: ase
 License-File: LICENSE
 
 PylammpsMPI couples a serial python process to an MPI parallel LAMMPS libary.
```

### Comparing `pylammpsmpi-0.2.0/pylammpsmpi/mpi/lmpmpi.py` & `pylammpsmpi-0.2.1/pylammpsmpi/mpi/lmpmpi.py`

 * *Files identical despite different names*

### Comparing `pylammpsmpi-0.2.0/pylammpsmpi/wrapper/base.py` & `pylammpsmpi-0.2.1/pylammpsmpi/wrapper/base.py`

 * *Files identical despite different names*

### Comparing `pylammpsmpi-0.2.0/pylammpsmpi/wrapper/concurrent.py` & `pylammpsmpi-0.2.1/pylammpsmpi/wrapper/concurrent.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 
 import os
 import socket
 from concurrent.futures import Future
 from queue import Queue
-from threading import Thread
-from pympipool import SocketInterface, cancel_items_in_queue
+from pympipool import RaisingThread, SocketInterface, cancel_items_in_queue
 
 
 __author__ = "Sarath Menon, Jan Janssen"
 __copyright__ = (
     "Copyright 2020, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
@@ -101,17 +100,18 @@
         self._future_queue = Queue()
         self._process = None
         self._oversubscribe = oversubscribe
         self._enable_flux_backend = enable_flux_backend
         self._cmdargs = cmdargs
         self._queue_adapter = queue_adapter
         self._queue_adapter_kwargs = queue_adapter_kwargs
+        self._start_process()
 
-    def start_process(self):
-        self._process = Thread(
+    def _start_process(self):
+        self._process = RaisingThread(
             target=execute_async,
             kwargs={
                 "future_queue": self._future_queue,
                 "cmdargs": self._cmdargs,
                 "cores": self.cores,
                 "oversubscribe": self._oversubscribe,
                 "enable_flux_backend": self._enable_flux_backend,
```

### Comparing `pylammpsmpi-0.2.0/pylammpsmpi/wrapper/extended.py` & `pylammpsmpi-0.2.1/pylammpsmpi/wrapper/extended.py`

 * *Files 1% similar despite different names*

```diff
@@ -263,15 +263,14 @@
             oversubscribe=self.oversubscribe,
             enable_flux_backend=self.enable_flux_backend,
             working_directory=self.working_directory,
             cmdargs=cmdargs,
             queue_adapter=queue_adapter,
             queue_adapter_kwargs=queue_adapter_kwargs,
         )
-        self.lmp.start_process()
 
     def __getattr__(self, name):
         """
         Try to run input as a lammps command
         """
         if name in func_list:
```

### Comparing `pylammpsmpi-0.2.0/pylammpsmpi.egg-info/PKG-INFO` & `pylammpsmpi-0.2.1/pylammpsmpi.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylammpsmpi
-Version: 0.2.0
+Version: 0.2.1
 Summary: Parallel Lammps Python interface
 Home-page: https://github.com/pyiron/pylammpsmpi
 Author: Jan Janssen
 Author-email: janssen@mpie.de
 License: BSD
 Keywords: lammps,mpi4py
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,10 +13,11 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: ase
 License-File: LICENSE
 
 PylammpsMPI couples a serial python process to an MPI parallel LAMMPS libary.
```

### Comparing `pylammpsmpi-0.2.0/setup.py` & `pylammpsmpi-0.2.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,26 +7,30 @@
     description="Parallel Lammps Python interface",
     long_description="PylammpsMPI couples a serial python process to an MPI parallel LAMMPS libary.",
     url='https://github.com/pyiron/pylammpsmpi',
     author='Jan Janssen',
     author_email='janssen@mpie.de',
     license='BSD',
 
-    classifiers=['Development Status :: 5 - Production/Stable',
-                 'Topic :: Scientific/Engineering :: Physics',
-                 'License :: OSI Approved :: BSD License',
-                 'Intended Audience :: Science/Research',
-                 'Operating System :: OS Independent',
-                 'Programming Language :: Python :: 3.7',
-                 'Programming Language :: Python :: 3.8',
-                 'Programming Language :: Python :: 3.9',
-                 'Programming Language :: Python :: 3.10',
-                 'Programming Language :: Python :: 3.11'
-                ],
+    classifiers=[
+        'Development Status :: 5 - Production/Stable',
+         'Topic :: Scientific/Engineering :: Physics',
+         'License :: OSI Approved :: BSD License',
+         'Intended Audience :: Science/Research',
+         'Operating System :: OS Independent',
+         'Programming Language :: Python :: 3.7',
+         'Programming Language :: Python :: 3.8',
+         'Programming Language :: Python :: 3.9',
+         'Programming Language :: Python :: 3.10',
+         'Programming Language :: Python :: 3.11',
+    ],
 
     keywords='lammps, mpi4py',
     packages=find_packages(exclude=["*tests*"]),
     install_requires=[
-        "mpi4py>=3.1.4", "pympipool>=0.5.4", "numpy>=1.23.5"
+        "mpi4py>=3.1.4", "pympipool>=0.5.6", "numpy>=1.23.5"
     ],
+    extras_require={
+        "ase": ["ase>=3.22.1", "scipy>=1.10.1"],
+    },
     cmdclass=versioneer.get_cmdclass(),
 )
```

### Comparing `pylammpsmpi-0.2.0/tests/test_base.py` & `pylammpsmpi-0.2.1/tests/test_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,14 @@
         cls.lmp = LammpsBase(
             cores=1,
             oversubscribe=False,
             enable_flux_backend=False,
             working_directory=".",
             cmdargs=["-cite", cls.citation_file]
         )
-        cls.lmp.start_process()
         cls.lmp.file(cls.lammps_file)
 
     @classmethod
     def tearDownClass(cls):
         cls.lmp.close()
 
     def test_extract_atom(self):
```

### Comparing `pylammpsmpi-0.2.0/tests/test_concurrent.py` & `pylammpsmpi-0.2.1/tests/test_concurrent.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,14 @@
         cls.lmp = LammpsConcurrent(
             cores=1,
             oversubscribe=False,
             enable_flux_backend=False,
             working_directory=".",
             cmdargs=["-cite", cls.citation_file]
         )
-        cls.lmp.start_process()
         cls.lmp.file(cls.lammps_file).result()
 
     @classmethod
     def tearDownClass(cls):
         cls.lmp.close()
 
     def test_extract_atom(self):
```

### Comparing `pylammpsmpi-0.2.0/tests/test_pylammpsmpi_local.py` & `pylammpsmpi-0.2.1/tests/test_pylammpsmpi_local.py`

 * *Files identical despite different names*

### Comparing `pylammpsmpi-0.2.0/versioneer.py` & `pylammpsmpi-0.2.1/versioneer.py`

 * *Files identical despite different names*

