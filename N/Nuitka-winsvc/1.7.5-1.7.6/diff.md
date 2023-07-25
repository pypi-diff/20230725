# Comparing `tmp/Nuitka-winsvc-1.7.5.tar.gz` & `tmp/Nuitka-winsvc-1.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Nuitka-winsvc-1.7.5.tar", last modified: Tue Jul 18 02:58:18 2023, max compression
+gzip compressed data, was "Nuitka-winsvc-1.7.6.tar", last modified: Tue Jul 25 02:27:12 2023, max compression
```

## Comparing `Nuitka-winsvc-1.7.5.tar` & `Nuitka-winsvc-1.7.6.tar`

### file list

```diff
@@ -1,1802 +1,1803 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.507221 Nuitka-winsvc-1.7.5/
--rw-rw-rw-   0        0        0   843525 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/Changelog.rst
--rw-rw-rw-   0        0        0   152515 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/Developer_Manual.rst
--rw-rw-rw-   0        0        0    11348 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.5/LICENSE.txt
--rw-rw-rw-   0        0        0     1733 2023-07-18 02:14:59.000000 Nuitka-winsvc-1.7.5/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:16.372813 Nuitka-winsvc-1.7.5/Nuitka_winsvc.egg-info/
--rw-rw-rw-   0        0        0     4626 2023-07-18 02:58:15.000000 Nuitka-winsvc-1.7.5/Nuitka_winsvc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    76718 2023-07-18 02:58:16.000000 Nuitka-winsvc-1.7.5/Nuitka_winsvc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 02:58:15.000000 Nuitka-winsvc-1.7.5/Nuitka_winsvc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      308 2023-07-18 02:58:15.000000 Nuitka-winsvc-1.7.5/Nuitka_winsvc.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-03-28 09:21:19.000000 Nuitka-winsvc-1.7.5/Nuitka_winsvc.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       35 2023-07-18 02:58:15.000000 Nuitka-winsvc-1.7.5/Nuitka_winsvc.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-18 02:58:15.000000 Nuitka-winsvc-1.7.5/Nuitka_winsvc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4626 2023-07-18 02:58:18.506240 Nuitka-winsvc-1.7.5/PKG-INFO
--rw-rw-rw-   0        0        0     2651 2023-07-18 02:14:59.000000 Nuitka-winsvc-1.7.5/README.md
--rw-rw-rw-   0        0        0    76929 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:16.385507 Nuitka-winsvc-1.7.5/bin/
--rw-rw-rw-   0        0        0     1135 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/bin/autoformat-nuitka-source
--rw-rw-rw-   0        0        0     1134 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/bin/check-nuitka-with-pylint
--rw-rw-rw-   0        0        0     1150 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/bin/compare_with_cpython
--rw-rw-rw-   0        0        0     3079 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/bin/compare_with_xml
--rw-rw-rw-   0        0        0     1163 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/bin/measure-construct-performance
--rw-rw-rw-   0        0        0     1685 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/bin/nuitka
--rw-rw-rw-   0        0        0     1685 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/bin/nuitka-run
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:16.242936 Nuitka-winsvc-1.7.5/doc/
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:16.389412 Nuitka-winsvc-1.7.5/doc/Logo/
--rw-rw-rw-   0        0        0     7321 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.5/doc/Logo/Nuitka-Logo-Horizontal.svg
--rw-rw-rw-   0        0        0     7401 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.5/doc/Logo/Nuitka-Logo-Symbol.svg
--rw-rw-rw-   0        0        0    17917 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.5/doc/Logo/Nuitka-Logo-Vertical.svg
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:16.398203 Nuitka-winsvc-1.7.5/doc/images/
--rw-rw-rw-   0        0        0     7585 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.5/doc/images/Nuitka-Logo-Horizontal.png
--rw-rw-rw-   0        0        0     4452 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.5/doc/images/Nuitka-Logo-Symbol.png
--rw-rw-rw-   0        0        0     9828 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.5/doc/images/Nuitka-Logo-Vertical.png
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:16.402110 Nuitka-winsvc-1.7.5/lib/
--rw-rw-rw-   0        0        0     4250 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/lib/hints.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:16.406992 Nuitka-winsvc-1.7.5/misc/
--rwxrwxrwx   0        0        0      901 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/misc/nuitka-run.bat
--rwxrwxrwx   0        0        0     1038 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/misc/nuitka.bat
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:16.439215 Nuitka-winsvc-1.7.5/nuitka/
--rw-rw-rw-   0        0        0     7529 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/nuitka/Builtins.py
--rw-rw-rw-   0        0        0     5437 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/BytecodeCaching.py
--rw-rw-rw-   0        0        0     3440 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/Bytecodes.py
--rw-rw-rw-   0        0        0     1884 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/CacheCleanup.py
--rw-rw-rw-   0        0        0    11148 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/Constants.py
--rw-rw-rw-   0        0        0     2447 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/Errors.py
--rw-rw-rw-   0        0        0    37438 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/nuitka/MainControl.py
--rw-rw-rw-   0        0        0     8064 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/ModuleRegistry.py
--rw-rw-rw-   0        0        0    57181 2023-07-18 02:14:59.000000 Nuitka-winsvc-1.7.5/nuitka/OptionParsing.py
--rw-rw-rw-   0        0        0    66375 2023-07-18 02:15:00.000000 Nuitka-winsvc-1.7.5/nuitka/Options.py
--rw-rw-rw-   0        0        0     5022 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/OutputDirectories.py
--rw-rw-rw-   0        0        0    14550 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/PostProcessing.py
--rw-rw-rw-   0        0        0     5770 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/Progress.py
--rw-rw-rw-   0        0        0     7472 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/PythonFlavors.py
--rw-rw-rw-   0        0        0     4061 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/PythonOperators.py
--rw-rw-rw-   0        0        0    12179 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/PythonVersions.py
--rw-rw-rw-   0        0        0     9062 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/nuitka/Serialization.py
--rw-rw-rw-   0        0        0     4670 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/SourceCodeReferences.py
--rw-rw-rw-   0        0        0    11235 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/Tracing.py
--rw-rw-rw-   0        0        0     3395 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/TreeXML.py
--rw-rw-rw-   0        0        0    15235 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/Variables.py
--rw-rw-rw-   0        0        0     2055 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/nuitka/Version.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/__init__.py
--rw-rw-rw-   0        0        0     5615 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/__main__.py
--rw-rw-rw-   0        0        0     5295 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/__past__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:16.455548 Nuitka-winsvc-1.7.5/nuitka/build/
--rw-rw-rw-   0        0        0    34131 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/nuitka/build/Backend.scons
--rw-rw-rw-   0        0        0     8300 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/nuitka/build/CCompilerVersion.scons
--rw-rw-rw-   0        0        0     2716 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/nuitka/build/DataComposerInterface.py
--rw-rw-rw-   0        0        0    18793 2023-07-18 02:15:00.000000 Nuitka-winsvc-1.7.5/nuitka/build/Onefile.scons
--rw-rw-rw-   0        0        0    15698 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/nuitka/build/SconsCaching.py
--rw-rw-rw-   0        0        0    31022 2023-07-18 02:15:00.000000 Nuitka-winsvc-1.7.5/nuitka/build/SconsCompilerSettings.py
--rw-rw-rw-   0        0        0     5527 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/SconsHacks.py
--rw-rw-rw-   0        0        0    15827 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/nuitka/build/SconsInterface.py
--rw-rw-rw-   0        0        0     2671 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/nuitka/build/SconsProgress.py
--rw-rw-rw-   0        0        0    12022 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/nuitka/build/SconsSpawn.py
--rw-rw-rw-   0        0        0    24338 2023-06-16 02:35:34.000000 Nuitka-winsvc-1.7.5/nuitka/build/SconsUtils.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:16.245864 Nuitka-winsvc-1.7.5/nuitka/build/include/
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:16.489725 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/
--rw-rw-rw-   0        0        0     7972 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/allocator.h
--rw-rw-rw-   0        0        0     3470 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/builtins.h
--rw-rw-rw-   0        0        0     4604 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/calling.h
--rw-rw-rw-   0        0        0     1977 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/checkers.h
--rw-rw-rw-   0        0        0     1261 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/checksum_tools.h
--rw-rw-rw-   0        0        0     9571 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/compiled_asyncgen.h
--rw-rw-rw-   0        0        0     2002 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/compiled_cell.h
--rw-rw-rw-   0        0        0     9325 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/compiled_coroutine.h
--rw-rw-rw-   0        0        0    16949 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/compiled_frame.h
--rw-rw-rw-   0        0        0     5972 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/compiled_function.h
--rw-rw-rw-   0        0        0     9136 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/compiled_generator.h
--rw-rw-rw-   0        0        0     1838 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/compiled_method.h
--rw-rw-rw-   0        0        0     7408 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/constants.h
--rw-rw-rw-   0        0        0     1293 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/constants_blob.h
--rw-rw-rw-   0        0        0    34083 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/exceptions.h
--rw-rw-rw-   0        0        0     3473 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/filesystem_paths.h
--rw-rw-rw-   0        0        0     6253 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/freelists.h
--rw-rw-rw-   0        0        0    86326 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/hedley.h
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:16.587379 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/
--rw-rw-rw-   0        0        0     3393 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/attributes.h
--rw-rw-rw-   0        0        0     2663 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/boolean.h
--rw-rw-rw-   0        0        0     1181 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/bytearrays.h
--rw-rw-rw-   0        0        0     1135 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/bytes.h
--rw-rw-rw-   0        0        0     9335 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/calling_generated.h
--rw-rw-rw-   0        0        0    13140 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/comparisons_eq.h
--rw-rw-rw-   0        0        0    10616 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/comparisons_ge.h
--rw-rw-rw-   0        0        0    10615 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/comparisons_gt.h
--rw-rw-rw-   0        0        0    13140 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/comparisons_le.h
--rw-rw-rw-   0        0        0    13139 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/comparisons_lt.h
--rw-rw-rw-   0        0        0    10616 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/comparisons_ne.h
--rw-rw-rw-   0        0        0     1743 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/complex.h
--rw-rw-rw-   0        0        0    13109 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/dictionaries.h
--rw-rw-rw-   0        0        0     1206 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/floats.h
--rw-rw-rw-   0        0        0     3897 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/import_hard.h
--rw-rw-rw-   0        0        0     1798 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/indexes.h
--rw-rw-rw-   0        0        0     2941 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/ints.h
--rw-rw-rw-   0        0        0     9992 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/iterators.h
--rw-rw-rw-   0        0        0     3411 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/lists.h
--rw-rw-rw-   0        0        0     1633 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/lists_generated.h
--rw-rw-rw-   0        0        0     1328 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/mappings.h
--rw-rw-rw-   0        0        0     4573 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/operations.h
--rw-rw-rw-   0        0        0    12685 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/operations_binary_add.h
--rw-rw-rw-   0        0        0     5663 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/operations_binary_bitand.h
--rw-rw-rw-   0        0        0     5641 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/operations_binary_bitor.h
--rw-rw-rw-   0        0        0     5663 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/operations_binary_bitxor.h
--rw-rw-rw-   0        0        0     5422 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/operations_binary_divmod.h
--rw-rw-rw-   0        0        0     5460 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/operations_binary_floordiv.h
--rw-rw-rw-   0        0        0     5115 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/operations_binary_lshift.h
--rw-rw-rw-   0        0        0     2799 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/operations_binary_matmult.h
--rw-rw-rw-   0        0        0    15778 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/operations_binary_mod.h
--rw-rw-rw-   0        0        0    13210 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/operations_binary_mult.h
--rw-rw-rw-   0        0        0     5791 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/operations_binary_olddiv.h
--rw-rw-rw-   0        0        0     4714 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/operations_binary_pow.h
--rw-rw-rw-   0        0        0     5115 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/operations_binary_rshift.h
--rw-rw-rw-   0        0        0     5824 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/operations_binary_sub.h
--rw-rw-rw-   0        0        0     5438 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/operations_binary_truediv.h
--rw-rw-rw-   0        0        0    15100 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/operations_builtin_types.h
--rw-rw-rw-   0        0        0     8670 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/operations_inplace_add.h
--rw-rw-rw-   0        0        0     3767 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/operations_inplace_bitand.h
--rw-rw-rw-   0        0        0     3753 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/operations_inplace_bitor.h
--rw-rw-rw-   0        0        0     3767 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/operations_inplace_bitxor.h
--rw-rw-rw-   0        0        0     4846 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/operations_inplace_floordiv.h
--rw-rw-rw-   0        0        0     3011 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/operations_inplace_lshift.h
--rw-rw-rw-   0        0        0     2727 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/operations_inplace_matmult.h
--rw-rw-rw-   0        0        0    10626 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/operations_inplace_mod.h
--rw-rw-rw-   0        0        0     9201 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/operations_inplace_mult.h
--rw-rw-rw-   0        0        0     5147 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/operations_inplace_olddiv.h
--rw-rw-rw-   0        0        0     4349 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/operations_inplace_pow.h
--rw-rw-rw-   0        0        0     3011 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/operations_inplace_rshift.h
--rw-rw-rw-   0        0        0     4975 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/operations_inplace_sub.h
--rw-rw-rw-   0        0        0     4826 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/operations_inplace_truediv.h
--rw-rw-rw-   0        0        0     3297 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/raising.h
--rw-rw-rw-   0        0        0     2178 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/rangeobjects.h
--rw-rw-rw-   0        0        0     1146 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/richcomparisons.h
--rw-rw-rw-   0        0        0     1112 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/sequences.h
--rw-rw-rw-   0        0        0     1025 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/sets.h
--rw-rw-rw-   0        0        0     8419 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/slices.h
--rw-rw-rw-   0        0        0     1242 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/strings.h
--rw-rw-rw-   0        0        0    17575 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/subscripts.h
--rw-rw-rw-   0        0        0     5720 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/tuples.h
--rw-rw-rw-   0        0        0    14411 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helpers.h
--rw-rw-rw-   0        0        0     5375 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/importing.h
--rw-rw-rw-   0        0        0    12979 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/incbin.h
--rw-rw-rw-   0        0        0    14427 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/prelude.h
--rw-rw-rw-   0        0        0     2870 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/printing.h
--rw-rw-rw-   0        0        0     1761 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/python_pgo.h
--rw-rw-rw-   0        0        0     2243 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/safe_string_ops.h
--rw-rw-rw-   0        0        0     3840 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/threading.h
--rw-rw-rw-   0        0        0     3144 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/tracing.h
--rw-rw-rw-   0        0        0     2936 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/unfreezing.h
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:16.274184 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:16.590307 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/appdirs/
--rw-rw-rw-   0        0        0     1097 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/appdirs/LICENSE.txt
--rw-rw-rw-   0        0        0    24824 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/appdirs/appdirs.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:16.592260 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/atomicwrites/
--rw-rw-rw-   0        0        0     1069 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/atomicwrites/LICENSE
--rw-rw-rw-   0        0        0     6794 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/atomicwrites/atomicwrites.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:16.594213 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/bin/
--rw-rw-rw-   0        0        0     1331 2023-04-13 07:04:12.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/bin/scons.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:16.249777 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/clcache/
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:16.597143 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/clcache/clcache/
--rw-rw-rw-   0        0        0     1585 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/clcache/clcache/LICENSE
--rw-rw-rw-   0        0        0       93 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/clcache/clcache/__init__.py
--rw-rw-rw-   0        0        0    65424 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/clcache/clcache/caching.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:16.598120 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/colorama/
--rw-rw-rw-   0        0        0     1491 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/colorama/LICENSE.txt
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:16.606909 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/colorama/colorama/
--rw-rw-rw-   0        0        0      243 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/colorama/colorama/__init__.py
--rw-rw-rw-   0        0        0     2522 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/colorama/colorama/ansi.py
--rw-rw-rw-   0        0        0    10517 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/colorama/colorama/ansitowin32.py
--rw-rw-rw-   0        0        0     1915 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/colorama/colorama/initialise.py
--rw-rw-rw-   0        0        0     5404 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/colorama/colorama/win32.py
--rw-rw-rw-   0        0        0     6438 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/colorama/colorama/winterm.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:16.607884 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/glob2/
--rw-rw-rw-   0        0        0     1359 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/glob2/LICENSE
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:16.612767 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/glob2/glob2/
--rw-rw-rw-   0        0        0       82 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/glob2/glob2/__init__.py
--rw-rw-rw-   0        0        0     6859 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/glob2/glob2/compat.py
--rw-rw-rw-   0        0        0     4463 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/glob2/glob2/fnmatch.py
--rw-rw-rw-   0        0        0     8304 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/glob2/glob2/impl.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:16.614720 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2/
--rw-rw-rw-   0        0        0     1467 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2/LICENSE.rst
--rw-rw-rw-   0        0        0       85 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:16.645968 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2/jinja2/
--rw-rw-rw-   0        0        0     2423 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2/jinja2/__init__.py
--rw-rw-rw-   0        0        0     2685 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2/jinja2/_compat.py
--rw-rw-rw-   0        0        0     1726 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2/jinja2/_identifier.py
--rw-rw-rw-   0        0        0    12719 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2/jinja2/bccache.py
--rw-rw-rw-   0        0        0    65386 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2/jinja2/compiler.py
--rw-rw-rw-   0        0        0     1626 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2/jinja2/constants.py
--rw-rw-rw-   0        0        0    12281 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2/jinja2/debug.py
--rw-rw-rw-   0        0        0     1400 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2/jinja2/defaults.py
--rw-rw-rw-   0        0        0    50849 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2/jinja2/environment.py
--rw-rw-rw-   0        0        0     4428 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2/jinja2/exceptions.py
--rw-rw-rw-   0        0        0    24500 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2/jinja2/ext.py
--rw-rw-rw-   0        0        0    36528 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2/jinja2/filters.py
--rw-rw-rw-   0        0        0     9197 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2/jinja2/idtracking.py
--rw-rw-rw-   0        0        0    28559 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2/jinja2/lexer.py
--rw-rw-rw-   0        0        0    17473 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2/jinja2/loaders.py
--rw-rw-rw-   0        0        0     4340 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2/jinja2/meta.py
--rw-rw-rw-   0        0        0     7308 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2/jinja2/nativetypes.py
--rw-rw-rw-   0        0        0    30853 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2/jinja2/nodes.py
--rw-rw-rw-   0        0        0     1722 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2/jinja2/optimizer.py
--rw-rw-rw-   0        0        0    35875 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2/jinja2/parser.py
--rw-rw-rw-   0        0        0    27644 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2/jinja2/runtime.py
--rw-rw-rw-   0        0        0    17080 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2/jinja2/sandbox.py
--rw-rw-rw-   0        0        0     4214 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2/jinja2/tests.py
--rw-rw-rw-   0        0        0    20501 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2/jinja2/utils.py
--rw-rw-rw-   0        0        0     3316 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2/jinja2/visitor.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:16.647921 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2_35/
--rw-rw-rw-   0        0        0     1466 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2_35/LICENSE.rst
--rw-rw-rw-   0        0        0       84 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2_35/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:16.677216 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2_35/jinja2/
--rw-rw-rw-   0        0        0     2616 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2_35/jinja2/__init__.py
--rw-rw-rw-   0        0        0     2685 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2_35/jinja2/_compat.py
--rw-rw-rw-   0        0        0     1726 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2_35/jinja2/_identifier.py
--rw-rw-rw-   0        0        0    12719 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2_35/jinja2/bccache.py
--rw-rw-rw-   0        0        0    65386 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2_35/jinja2/compiler.py
--rw-rw-rw-   0        0        0     1626 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2_35/jinja2/constants.py
--rw-rw-rw-   0        0        0    12281 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2_35/jinja2/debug.py
--rw-rw-rw-   0        0        0     1400 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2_35/jinja2/defaults.py
--rw-rw-rw-   0        0        0    50849 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2_35/jinja2/environment.py
--rw-rw-rw-   0        0        0     4428 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2_35/jinja2/exceptions.py
--rw-rw-rw-   0        0        0    24500 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2_35/jinja2/ext.py
--rw-rw-rw-   0        0        0    36528 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2_35/jinja2/filters.py
--rw-rw-rw-   0        0        0     9197 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2_35/jinja2/idtracking.py
--rw-rw-rw-   0        0        0    28559 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2_35/jinja2/lexer.py
--rw-rw-rw-   0        0        0    17474 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2_35/jinja2/loaders.py
--rw-rw-rw-   0        0        0     4340 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2_35/jinja2/meta.py
--rw-rw-rw-   0        0        0     7308 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2_35/jinja2/nativetypes.py
--rw-rw-rw-   0        0        0    30853 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2_35/jinja2/nodes.py
--rw-rw-rw-   0        0        0     1722 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2_35/jinja2/optimizer.py
--rw-rw-rw-   0        0        0    35875 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2_35/jinja2/parser.py
--rw-rw-rw-   0        0        0    27644 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2_35/jinja2/runtime.py
--rw-rw-rw-   0        0        0    17080 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2_35/jinja2/sandbox.py
--rw-rw-rw-   0        0        0     4214 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2_35/jinja2/tests.py
--rw-rw-rw-   0        0        0    20501 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2_35/jinja2/utils.py
--rw-rw-rw-   0        0        0     3316 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2_35/jinja2/visitor.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:16.264438 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:16.254655 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:16.704558 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/
--rw-rw-rw-   0        0        0    47844 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Action.py
--rw-rw-rw-   0        0        0    33996 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Builder.py
--rw-rw-rw-   0        0        0     8083 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/CacheDir.py
--rw-rw-rw-   0        0        0    27693 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Conftest.py
--rw-rw-rw-   0        0        0     6938 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Debug.py
--rw-rw-rw-   0        0        0    17622 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Defaults.py
--rw-rw-rw-   0        0        0    96183 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Environment.py
--rw-rw-rw-   0        0        0     7358 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Errors.py
--rw-rw-rw-   0        0        0    21540 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Executor.py
--rw-rw-rw-   0        0        0    16000 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Job.py
--rw-rw-rw-   0        0        0     9589 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Memoize.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:16.707487 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/
--rw-rw-rw-   0        0        0     4197 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Alias.py
--rw-rw-rw-   0        0        0   121420 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/FS.py
--rw-rw-rw-   0        0        0     4164 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Python.py
--rw-rw-rw-   0        0        0    49503 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:16.713347 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/
--rw-rw-rw-   0        0        0     1950 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/BoolOption.py
--rw-rw-rw-   0        0        0     1950 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/EnumOption.py
--rw-rw-rw-   0        0        0     1950 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/ListOption.py
--rw-rw-rw-   0        0        0     1965 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PackageOption.py
--rw-rw-rw-   0        0        0     2736 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PathOption.py
--rw-rw-rw-   0        0        0     2614 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/__init__.py
--rw-rw-rw-   0        0        0     8467 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/PathList.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:16.726042 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/
--rw-rw-rw-   0        0        0     9314 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/__init__.py
--rw-rw-rw-   0        0        0     3131 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/aix.py
--rw-rw-rw-   0        0        0     1989 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/cygwin.py
--rw-rw-rw-   0        0        0     2483 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/darwin.py
--rw-rw-rw-   0        0        0     1718 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/hpux.py
--rw-rw-rw-   0        0        0     1605 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/irix.py
--rw-rw-rw-   0        0        0     2170 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/os2.py
--rw-rw-rw-   0        0        0     4179 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/posix.py
--rw-rw-rw-   0        0        0     1882 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/sunos.py
--rw-rw-rw-   0        0        0    14948 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/win32.py
--rw-rw-rw-   0        0        0    39700 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConf.py
--rw-rw-rw-   0        0        0    12950 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConsign.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:16.730924 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/
--rw-rw-rw-   0        0        0     4810 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/C.py
--rw-rw-rw-   0        0        0     3751 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Dir.py
--rw-rw-rw-   0        0        0     3233 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Prog.py
--rw-rw-rw-   0        0        0     2011 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/RC.py
--rw-rw-rw-   0        0        0    14663 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:16.737760 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/
--rw-rw-rw-   0        0        0    14029 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Interactive.py
--rw-rw-rw-   0        0        0    52665 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Main.py
--rw-rw-rw-   0        0        0    40719 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConsOptions.py
--rw-rw-rw-   0        0        0    24133 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConscript.py
--rw-rw-rw-   0        0        0    14053 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/__init__.py
--rw-rw-rw-   0        0        0     2305 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Sig.py
--rw-rw-rw-   0        0        0    34903 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Subst.py
--rw-rw-rw-   0        0        0    40510 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Taskmaster.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:16.824670 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/
--rw-rw-rw-   0        0        0     2166 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/386asm.py
--rw-rw-rw-   0        0        0     2433 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/BitKeeper.py
--rw-rw-rw-   0        0        0     2859 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/CVS.py
--rw-rw-rw-   0        0        0    18084 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/GettextCommon.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:16.831509 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/
--rw-rw-rw-   0        0        0     2078 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/__init__.py
--rw-rw-rw-   0        0        0     2004 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/arch.py
--rw-rw-rw-   0        0        0     9248 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/common.py
--rw-rw-rw-   0        0        0     2784 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/netframework.py
--rw-rw-rw-   0        0        0    14869 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/sdk.py
--rw-rw-rw-   0        0        0    19499 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vc.py
--rw-rw-rw-   0        0        0    20832 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vs.py
--rw-rw-rw-   0        0        0     3763 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Perforce.py
--rw-rw-rw-   0        0        0     5149 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/PharLapCommon.py
--rw-rw-rw-   0        0        0     2290 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/RCS.py
--rw-rw-rw-   0        0        0     2328 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/SCCS.py
--rw-rw-rw-   0        0        0     2657 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Subversion.py
--rw-rw-rw-   0        0        0    31283 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/__init__.py
--rw-rw-rw-   0        0        0     2379 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixc++.py
--rw-rw-rw-   0        0        0     2267 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixcc.py
--rw-rw-rw-   0        0        0     2681 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixf77.py
--rw-rw-rw-   0        0        0     2720 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixlink.py
--rw-rw-rw-   0        0        0     2796 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/applelink.py
--rw-rw-rw-   0        0        0     2147 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ar.py
--rw-rw-rw-   0        0        0     2936 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/as.py
--rw-rw-rw-   0        0        0     2935 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/bcc32.py
--rw-rw-rw-   0        0        0     3432 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/c++.py
--rw-rw-rw-   0        0        0     3785 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cc.py
--rw-rw-rw-   0        0        0     2777 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cyglink.py
--rw-rw-rw-   0        0        0     1711 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/default.py
--rw-rw-rw-   0        0        0      142 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/dmd.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:16.833460 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/docbook/
--rw-rw-rw-   0        0        0    29618 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/docbook/__init__.py
--rw-rw-rw-   0        0        0     3428 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/filesystem.py
--rw-rw-rw-   0        0        0     2681 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g++.py
--rw-rw-rw-   0        0        0     2433 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g77.py
--rw-rw-rw-   0        0        0     1844 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gas.py
--rw-rw-rw-   0        0        0     3472 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gcc.py
--rw-rw-rw-   0        0        0     4782 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gdc.py
--rw-rw-rw-   0        0        0     2025 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gettext.py
--rw-rw-rw-   0        0        0     2256 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gfortran.py
--rw-rw-rw-   0        0        0     2460 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gnulink.py
--rw-rw-rw-   0        0        0     2639 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpc++.py
--rw-rw-rw-   0        0        0     1810 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpcc.py
--rw-rw-rw-   0        0        0     2333 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hplink.py
--rw-rw-rw-   0        0        0     2140 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icc.py
--rw-rw-rw-   0        0        0     1902 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icl.py
--rw-rw-rw-   0        0        0     2077 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink.py
--rw-rw-rw-   0        0        0     2043 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink32.py
--rw-rw-rw-   0        0        0    18600 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/install.py
--rw-rw-rw-   0        0        0    25816 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/intelc.py
--rw-rw-rw-   0        0        0     3328 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/lex.py
--rw-rw-rw-   0        0        0     8394 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/link.py
--rw-rw-rw-   0        0        0     3953 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/linkloc.py
--rw-rw-rw-   0        0        0     2309 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/m4.py
--rw-rw-rw-   0        0        0     2945 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/masm.py
--rw-rw-rw-   0        0        0     6919 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mingw.py
--rw-rw-rw-   0        0        0     4381 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgfmt.py
--rw-rw-rw-   0        0        0     4658 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msginit.py
--rw-rw-rw-   0        0        0     4224 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgmerge.py
--rw-rw-rw-   0        0        0     2168 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslib.py
--rw-rw-rw-   0        0        0    13881 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslink.py
--rw-rw-rw-   0        0        0     1804 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mssdk.py
--rw-rw-rw-   0        0        0    11380 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvc.py
--rw-rw-rw-   0        0        0    72761 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvs.py
--rw-rw-rw-   0        0        0     6841 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwcc.py
--rw-rw-rw-   0        0        0     3579 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwld.py
--rw-rw-rw-   0        0        0     2618 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/nasm.py
--rw-rw-rw-   0        0        0     4375 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rmic.py
--rw-rw-rw-   0        0        0     2827 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rpcgen.py
--rw-rw-rw-   0        0        0     2513 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgiar.py
--rw-rw-rw-   0        0        0     1991 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgic++.py
--rw-rw-rw-   0        0        0     1819 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgicc.py
--rw-rw-rw-   0        0        0     2123 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgilink.py
--rw-rw-rw-   0        0        0     2502 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunar.py
--rw-rw-rw-   0        0        0     4695 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunc++.py
--rw-rw-rw-   0        0        0     1927 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/suncc.py
--rw-rw-rw-   0        0        0     2349 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunlink.py
--rw-rw-rw-   0        0        0     2473 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tar.py
--rw-rw-rw-   0        0        0     5992 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/textfile.py
--rw-rw-rw-   0        0        0     1831 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tlib.py
--rw-rw-rw-   0        0        0     3730 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/wix.py
--rw-rw-rw-   0        0        0    13016 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/xgettext.py
--rw-rw-rw-   0        0        0     3415 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/zip.py
--rw-rw-rw-   0        0        0    48938 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Util.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:16.842247 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/
--rw-rw-rw-   0        0        0     3007 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/BoolVariable.py
--rw-rw-rw-   0        0        0     3784 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/EnumVariable.py
--rw-rw-rw-   0        0        0     4404 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/ListVariable.py
--rw-rw-rw-   0        0        0     3557 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PackageVariable.py
--rw-rw-rw-   0        0        0     5612 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PathVariable.py
--rw-rw-rw-   0        0        0    11034 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/__init__.py
--rw-rw-rw-   0        0        0     6824 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Warnings.py
--rw-rw-rw-   0        0        0     1563 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:16.853974 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/
--rw-rw-rw-   0        0        0     8120 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/__init__.py
--rw-rw-rw-   0        0        0     3596 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_builtins.py
--rw-rw-rw-   0        0        0     1818 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_collections.py
--rw-rw-rw-   0        0        0     1742 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_dbm.py
--rw-rw-rw-   0        0        0     2465 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_hashlib.py
--rw-rw-rw-   0        0        0     1776 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_io.py
--rw-rw-rw-   0        0        0    19253 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_sets.py
--rw-rw-rw-   0        0        0    44500 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_subprocess.py
--rw-rw-rw-   0        0        0    19664 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/cpp.py
--rw-rw-rw-   0        0        0     7509 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/dblite.py
--rw-rw-rw-   0        0        0     2107 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/exitfuncs.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:16.259535 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:16.880331 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/
--rw-rw-rw-   0        0        0    53545 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Action.py
--rw-rw-rw-   0        0        0    34985 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Builder.py
--rw-rw-rw-   0        0        0    13596 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/CacheDir.py
--rw-rw-rw-   0        0        0    28403 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Conftest.py
--rw-rw-rw-   0        0        0     7533 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Debug.py
--rw-rw-rw-   0        0        0    20988 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Defaults.py
--rw-rw-rw-   0        0        0    96818 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Environment.py
--rw-rw-rw-   0        0        0     7752 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Errors.py
--rw-rw-rw-   0        0        0    22350 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Executor.py
--rw-rw-rw-   0        0        0    16068 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Job.py
--rw-rw-rw-   0        0        0     9565 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Memoize.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:16.891072 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/
--rw-rw-rw-   0        0        0     5239 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Alias.py
--rw-rw-rw-   0        0        0   135413 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/FS.py
--rw-rw-rw-   0        0        0     5758 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Python.py
--rw-rw-rw-   0        0        0    63474 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/__init__.py
--rw-rw-rw-   0        0        0     8354 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/PathList.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:16.907673 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/
--rw-rw-rw-   0        0        0    11500 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/__init__.py
--rw-rw-rw-   0        0        0     3180 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/aix.py
--rw-rw-rw-   0        0        0     2227 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/cygwin.py
--rw-rw-rw-   0        0        0     2739 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/darwin.py
--rw-rw-rw-   0        0        0     1767 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/hpux.py
--rw-rw-rw-   0        0        0     1654 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/irix.py
--rw-rw-rw-   0        0        0     1460 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/mingw.py
--rw-rw-rw-   0        0        0     2219 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/os2.py
--rw-rw-rw-   0        0        0     4476 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/posix.py
--rw-rw-rw-   0        0        0     1931 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/sunos.py
--rw-rw-rw-   0        0        0     4003 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/virtualenv.py
--rw-rw-rw-   0        0        0    16962 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/win32.py
--rw-rw-rw-   0        0        0    41186 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConf.py
--rw-rw-rw-   0        0        0    13880 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConsign.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:16.913533 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/
--rw-rw-rw-   0        0        0     4853 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/C.py
--rw-rw-rw-   0        0        0     3812 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Dir.py
--rw-rw-rw-   0        0        0     3643 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Prog.py
--rw-rw-rw-   0        0        0     2328 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/RC.py
--rw-rw-rw-   0        0        0    15053 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:16.923313 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/
--rw-rw-rw-   0        0        0    13779 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Interactive.py
--rw-rw-rw-   0        0        0    53260 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Main.py
--rw-rw-rw-   0        0        0    39394 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConsOptions.py
--rw-rw-rw-   0        0        0    26467 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConscript.py
--rw-rw-rw-   0        0        0    14489 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/__init__.py
--rw-rw-rw-   0        0        0    35863 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Subst.py
--rw-rw-rw-   0        0        0    42204 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Taskmaster.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:17.029748 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/
--rw-rw-rw-   0        0        0     2211 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/386asm.py
--rw-rw-rw-   0        0        0    18207 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/GettextCommon.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:17.044018 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/
--rw-rw-rw-   0        0        0     2152 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/__init__.py
--rw-rw-rw-   0        0        0     2057 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/arch.py
--rw-rw-rw-   0        0        0    10674 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/common.py
--rw-rw-rw-   0        0        0     2855 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/netframework.py
--rw-rw-rw-   0        0        0    15165 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/sdk.py
--rw-rw-rw-   0        0        0    33537 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vc.py
--rw-rw-rw-   0        0        0    21762 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vs.py
--rw-rw-rw-   0        0        0     4464 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/PharLapCommon.py
--rw-rw-rw-   0        0        0    50660 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/__init__.py
--rw-rw-rw-   0        0        0     1667 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixc++.py
--rw-rw-rw-   0        0        0     2316 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcc.py
--rw-rw-rw-   0        0        0     2475 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcxx.py
--rw-rw-rw-   0        0        0     2840 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixlink.py
--rw-rw-rw-   0        0        0     8618 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/applelink.py
--rw-rw-rw-   0        0        0     2226 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ar.py
--rw-rw-rw-   0        0        0     2978 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/as.py
--rw-rw-rw-   0        0        0     2977 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/bcc32.py
--rw-rw-rw-   0        0        0     1653 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/c++.py
--rw-rw-rw-   0        0        0     3827 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cc.py
--rw-rw-rw-   0        0        0     3389 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clang.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:17.045008 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangCommon/
--rw-rw-rw-   0        0        0      313 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangCommon/__init__.py
--rw-rw-rw-   0        0        0     3631 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangxx.py
--rw-rw-rw-   0        0        0     3444 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cxx.py
--rw-rw-rw-   0        0        0     8494 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cyglink.py
--rw-rw-rw-   0        0        0     1753 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/default.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:17.045972 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/docbook/
--rw-rw-rw-   0        0        0    29765 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/docbook/__init__.py
--rw-rw-rw-   0        0        0     3472 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/filesystem.py
--rw-rw-rw-   0        0        0     1630 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/g++.py
--rw-rw-rw-   0        0        0     1977 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gas.py
--rw-rw-rw-   0        0        0     3686 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gcc.py
--rw-rw-rw-   0        0        0     2580 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gettext_tool.py
--rw-rw-rw-   0        0        0     2948 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gnulink.py
--rw-rw-rw-   0        0        0     2655 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gxx.py
--rw-rw-rw-   0        0        0     1645 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpc++.py
--rw-rw-rw-   0        0        0     1859 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcc.py
--rw-rw-rw-   0        0        0     2765 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcxx.py
--rw-rw-rw-   0        0        0     2386 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hplink.py
--rw-rw-rw-   0        0        0     2189 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icc.py
--rw-rw-rw-   0        0        0     1944 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icl.py
--rw-rw-rw-   0        0        0     2123 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink.py
--rw-rw-rw-   0        0        0     2085 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink32.py
--rw-rw-rw-   0        0        0    15791 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/install.py
--rw-rw-rw-   0        0        0    26195 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/intelc.py
--rw-rw-rw-   0        0        0    13924 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/link.py
--rw-rw-rw-   0        0        0     4041 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/linkloc.py
--rw-rw-rw-   0        0        0     2351 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/m4.py
--rw-rw-rw-   0        0        0     2987 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/masm.py
--rw-rw-rw-   0        0        0     7808 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mingw.py
--rw-rw-rw-   0        0        0     4956 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgfmt.py
--rw-rw-rw-   0        0        0     5235 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msginit.py
--rw-rw-rw-   0        0        0     4808 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgmerge.py
--rw-rw-rw-   0        0        0     2475 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslib.py
--rw-rw-rw-   0        0        0    14751 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslink.py
--rw-rw-rw-   0        0        0     1847 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mssdk.py
--rw-rw-rw-   0        0        0    12588 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvc.py
--rw-rw-rw-   0        0        0    82939 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvs.py
--rw-rw-rw-   0        0        0     6883 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwcc.py
--rw-rw-rw-   0        0        0     3663 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwld.py
--rw-rw-rw-   0        0        0     2660 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/nasm.py
--rw-rw-rw-   0        0        0     4904 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rmic.py
--rw-rw-rw-   0        0        0     2877 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rpcgen.py
--rw-rw-rw-   0        0        0     2567 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgiar.py
--rw-rw-rw-   0        0        0     1652 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgic++.py
--rw-rw-rw-   0        0        0     1868 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicc.py
--rw-rw-rw-   0        0        0     2088 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicxx.py
--rw-rw-rw-   0        0        0     2176 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgilink.py
--rw-rw-rw-   0        0        0     2366 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunar.py
--rw-rw-rw-   0        0        0     1658 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunc++.py
--rw-rw-rw-   0        0        0     1976 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncc.py
--rw-rw-rw-   0        0        0     5335 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncxx.py
--rw-rw-rw-   0        0        0     2583 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunlink.py
--rw-rw-rw-   0        0        0     2515 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tar.py
--rw-rw-rw-   0        0        0     6756 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/textfile.py
--rw-rw-rw-   0        0        0     1873 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tlib.py
--rw-rw-rw-   0        0        0     3773 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/wix.py
--rw-rw-rw-   0        0        0    13982 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/xgettext.py
--rw-rw-rw-   0        0        0     3201 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/zip.py
--rw-rw-rw-   0        0        0    53803 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Util.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:17.056717 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/
--rw-rw-rw-   0        0        0     3064 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/BoolVariable.py
--rw-rw-rw-   0        0        0     3818 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/EnumVariable.py
--rw-rw-rw-   0        0        0     4459 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/ListVariable.py
--rw-rw-rw-   0        0        0     3643 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PackageVariable.py
--rw-rw-rw-   0        0        0     5579 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PathVariable.py
--rw-rw-rw-   0        0        0    11655 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/__init__.py
--rw-rw-rw-   0        0        0     6504 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Warnings.py
--rw-rw-rw-   0        0        0     1647 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:17.060633 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/
--rw-rw-rw-   0        0        0     6869 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/__init__.py
--rw-rw-rw-   0        0        0     1784 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/_scons_dbm.py
--rw-rw-rw-   0        0        0    19816 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/cpp.py
--rw-rw-rw-   0        0        0     9002 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/dblite.py
--rw-rw-rw-   0        0        0     2149 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/exitfuncs.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:16.264438 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:17.096750 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/
--rw-rw-rw-   0        0        0    56578 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Action.py
--rw-rw-rw-   0        0        0    35213 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Builder.py
--rw-rw-rw-   0        0        0    11061 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/CacheDir.py
--rw-rw-rw-   0        0        0    27408 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Conftest.py
--rw-rw-rw-   0        0        0     7884 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Debug.py
--rw-rw-rw-   0        0        0    21423 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Defaults.py
--rw-rw-rw-   0        0        0    97269 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Environment.py
--rw-rw-rw-   0        0        0     3979 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/EnvironmentValues.py
--rw-rw-rw-   0        0        0     7515 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Errors.py
--rw-rw-rw-   0        0        0    21937 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Executor.py
--rw-rw-rw-   0        0        0    16583 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Job.py
--rw-rw-rw-   0        0        0     9430 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Memoize.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:17.104572 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/
--rw-rw-rw-   0        0        0     5126 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Alias.py
--rw-rw-rw-   0        0        0   136271 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/FS.py
--rw-rw-rw-   0        0        0     6167 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Python.py
--rw-rw-rw-   0        0        0    63768 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/__init__.py
--rw-rw-rw-   0        0        0     8183 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/PathList.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:17.124096 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/
--rw-rw-rw-   0        0        0    12836 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/__init__.py
--rw-rw-rw-   0        0        0     3087 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/aix.py
--rw-rw-rw-   0        0        0     2107 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/cygwin.py
--rw-rw-rw-   0        0        0     2630 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/darwin.py
--rw-rw-rw-   0        0        0     1674 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/hpux.py
--rw-rw-rw-   0        0        0     1536 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/irix.py
--rw-rw-rw-   0        0        0     1311 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/mingw.py
--rw-rw-rw-   0        0        0     2076 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/os2.py
--rw-rw-rw-   0        0        0     4356 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/posix.py
--rw-rw-rw-   0        0        0     1805 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/sunos.py
--rw-rw-rw-   0        0        0     3860 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/virtualenv.py
--rw-rw-rw-   0        0        0    14831 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/win32.py
--rw-rw-rw-   0        0        0    41983 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConf.py
--rw-rw-rw-   0        0        0    14673 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConsign.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:17.129953 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/
--rw-rw-rw-   0        0        0     7394 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/C.py
--rw-rw-rw-   0        0        0     4357 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Dir.py
--rw-rw-rw-   0        0        0     3546 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Prog.py
--rw-rw-rw-   0        0        0     1972 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/RC.py
--rw-rw-rw-   0        0        0    15577 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:17.139727 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/
--rw-rw-rw-   0        0        0    13597 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Interactive.py
--rw-rw-rw-   0        0        0    53509 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Main.py
--rw-rw-rw-   0        0        0    42760 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConsOptions.py
--rw-rw-rw-   0        0        0    26676 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConscript.py
--rw-rw-rw-   0        0        0    14272 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/__init__.py
--rw-rw-rw-   0        0        0    36753 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Subst.py
--rw-rw-rw-   0        0        0    41191 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Taskmaster.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:17.258852 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/
--rw-rw-rw-   0        0        0     2122 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/386asm.py
--rw-rw-rw-   0        0        0    15570 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/GettextCommon.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:17.268620 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/
--rw-rw-rw-   0        0        0     2014 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/__init__.py
--rw-rw-rw-   0        0        0     1943 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/arch.py
--rw-rw-rw-   0        0        0    13182 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/common.py
--rw-rw-rw-   0        0        0     2734 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/netframework.py
--rw-rw-rw-   0        0        0    15027 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/sdk.py
--rw-rw-rw-   0        0        0    38783 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vc.py
--rw-rw-rw-   0        0        0    22570 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vs.py
--rw-rw-rw-   0        0        0     4368 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/PharLapCommon.py
--rw-rw-rw-   0        0        0    32724 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/__init__.py
--rw-rw-rw-   0        0        0     1578 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixc++.py
--rw-rw-rw-   0        0        0     2228 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcc.py
--rw-rw-rw-   0        0        0     2386 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcxx.py
--rw-rw-rw-   0        0        0     2616 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixlink.py
--rw-rw-rw-   0        0        0     7993 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/applelink.py
--rw-rw-rw-   0        0        0     2141 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ar.py
--rw-rw-rw-   0        0        0     1661 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/as.py
--rw-rw-rw-   0        0        0     2893 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/asm.py
--rw-rw-rw-   0        0        0     2889 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/bcc32.py
--rw-rw-rw-   0        0        0     1567 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/c++.py
--rw-rw-rw-   0        0        0     3742 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cc.py
--rw-rw-rw-   0        0        0     3296 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clang.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:17.270577 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangCommon/
--rw-rw-rw-   0        0        0      343 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangCommon/__init__.py
--rw-rw-rw-   0        0        0     3534 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangxx.py
--rw-rw-rw-   0        0        0     3259 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cxx.py
--rw-rw-rw-   0        0        0     7461 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cyglink.py
--rw-rw-rw-   0        0        0     1663 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/default.py
--rw-rw-rw-   0        0        0     3379 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/filesystem.py
--rw-rw-rw-   0        0        0     1544 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/g++.py
--rw-rw-rw-   0        0        0     1891 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gas.py
--rw-rw-rw-   0        0        0     3616 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gcc.py
--rw-rw-rw-   0        0        0     2377 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gettext_tool.py
--rw-rw-rw-   0        0        0     2437 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gnulink.py
--rw-rw-rw-   0        0        0     2526 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gxx.py
--rw-rw-rw-   0        0        0     1557 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpc++.py
--rw-rw-rw-   0        0        0     1772 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcc.py
--rw-rw-rw-   0        0        0     2677 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcxx.py
--rw-rw-rw-   0        0        0     2206 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hplink.py
--rw-rw-rw-   0        0        0     2096 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icc.py
--rw-rw-rw-   0        0        0     1851 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icl.py
--rw-rw-rw-   0        0        0     1954 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink.py
--rw-rw-rw-   0        0        0     1995 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink32.py
--rw-rw-rw-   0        0        0    19180 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/install.py
--rw-rw-rw-   0        0        0    25826 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/intelc.py
--rw-rw-rw-   0        0        0     2588 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/link.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:17.274475 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/
--rw-rw-rw-   0        0        0     4649 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/LoadableModule.py
--rw-rw-rw-   0        0        0     7652 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/SharedLibrary.py
--rw-rw-rw-   0        0        0     6064 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/__init__.py
--rw-rw-rw-   0        0        0     3931 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkloc.py
--rw-rw-rw-   0        0        0     2266 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/m4.py
--rw-rw-rw-   0        0        0     2900 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/masm.py
--rw-rw-rw-   0        0        0     8622 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mingw.py
--rw-rw-rw-   0        0        0     4577 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgfmt.py
--rw-rw-rw-   0        0        0     4517 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msginit.py
--rw-rw-rw-   0        0        0     4113 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgmerge.py
--rw-rw-rw-   0        0        0     2387 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslib.py
--rw-rw-rw-   0        0        0    14473 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslink.py
--rw-rw-rw-   0        0        0     1752 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mssdk.py
--rw-rw-rw-   0        0        0    12902 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvc.py
--rw-rw-rw-   0        0        0    84784 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvs.py
--rw-rw-rw-   0        0        0     6788 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwcc.py
--rw-rw-rw-   0        0        0     3576 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwld.py
--rw-rw-rw-   0        0        0     2573 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/nasm.py
--rw-rw-rw-   0        0        0     4817 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rmic.py
--rw-rw-rw-   0        0        0     2788 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rpcgen.py
--rw-rw-rw-   0        0        0     2479 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgiar.py
--rw-rw-rw-   0        0        0     1563 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgic++.py
--rw-rw-rw-   0        0        0     1780 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicc.py
--rw-rw-rw-   0        0        0     1999 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicxx.py
--rw-rw-rw-   0        0        0     2006 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgilink.py
--rw-rw-rw-   0        0        0     2271 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunar.py
--rw-rw-rw-   0        0        0     1569 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunc++.py
--rw-rw-rw-   0        0        0     1888 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncc.py
--rw-rw-rw-   0        0        0     4879 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncxx.py
--rw-rw-rw-   0        0        0     2419 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunlink.py
--rw-rw-rw-   0        0        0     2429 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tar.py
--rw-rw-rw-   0        0        0     6412 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/textfile.py
--rw-rw-rw-   0        0        0     1786 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tlib.py
--rw-rw-rw-   0        0        0     3687 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/wix.py
--rw-rw-rw-   0        0        0    12548 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/xgettext.py
--rw-rw-rw-   0        0        0     4076 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/zip.py
--rw-rw-rw-   0        0        0    71693 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Util.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:17.277404 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/
--rw-rw-rw-   0        0        0     6632 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/ConfigureCache.py
--rw-rw-rw-   0        0        0        0 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/__init__.py
--rw-rw-rw-   0        0        0    15278 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/sconsign.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:17.285231 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/
--rw-rw-rw-   0        0        0     3134 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/BoolVariable.py
--rw-rw-rw-   0        0        0     3896 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/EnumVariable.py
--rw-rw-rw-   0        0        0     4672 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/ListVariable.py
--rw-rw-rw-   0        0        0     3536 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PackageVariable.py
--rw-rw-rw-   0        0        0     5588 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PathVariable.py
--rw-rw-rw-   0        0        0    12708 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/__init__.py
--rw-rw-rw-   0        0        0     6785 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Warnings.py
--rw-rw-rw-   0        0        0      353 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:17.290099 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/
--rw-rw-rw-   0        0        0     4307 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/__init__.py
--rw-rw-rw-   0        0        0     1644 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/_scons_dbm.py
--rw-rw-rw-   0        0        0     3395 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/win32.py
--rw-rw-rw-   0        0        0    21614 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/cpp.py
--rw-rw-rw-   0        0        0     9295 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/dblite.py
--rw-rw-rw-   0        0        0     2032 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/exitfuncs.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:17.290099 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/markupsafe/
--rw-rw-rw-   0        0        0     1467 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/markupsafe/LICENSE.rst
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:17.294005 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/markupsafe/markupsafe/
--rw-rw-rw-   0        0        0    10126 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/markupsafe/markupsafe/__init__.py
--rw-rw-rw-   0        0        0      558 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/markupsafe/markupsafe/_compat.py
--rw-rw-rw-   0        0        0     4690 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/markupsafe/markupsafe/_constants.py
--rw-rw-rw-   0        0        0     1873 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/markupsafe/markupsafe/_native.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:16.271254 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/pkg_resources/
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:17.295959 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/pkg_resources/pkg_resources/
--rw-rw-rw-   0        0        0   107452 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/pkg_resources/pkg_resources/__init__.py
--rw-rw-rw-   0        0        0      538 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/pkg_resources/pkg_resources/py31compat.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:16.272230 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/tqdm/
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:17.315489 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/tqdm/tqdm/
--rw-rw-rw-   0        0        0     1591 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/tqdm/tqdm/__init__.py
--rw-rw-rw-   0        0        0      283 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/tqdm/tqdm/_main.py
--rw-rw-rw-   0        0        0     3687 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/tqdm/tqdm/_monitor.py
--rw-rw-rw-   0        0        0      283 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/tqdm/tqdm/_tqdm.py
--rw-rw-rw-   0        0        0      287 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/tqdm/tqdm/_tqdm_gui.py
--rw-rw-rw-   0        0        0      307 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/tqdm/tqdm/_tqdm_notebook.py
--rw-rw-rw-   0        0        0      888 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/tqdm/tqdm/_tqdm_pandas.py
--rw-rw-rw-   0        0        0      596 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/tqdm/tqdm/_utils.py
--rw-rw-rw-   0        0        0     1106 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/tqdm/tqdm/auto.py
--rw-rw-rw-   0        0        0      857 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/tqdm/tqdm/autonotebook.py
--rw-rw-rw-   0        0        0     1376 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/tqdm/tqdm/dask.py
--rw-rw-rw-   0        0        0     5943 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/tqdm/tqdm/gui.py
--rw-rw-rw-   0        0        0    10790 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/tqdm/tqdm/notebook.py
--rw-rw-rw-   0        0        0    57572 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/tqdm/tqdm/std.py
--rw-rw-rw-   0        0        0     6948 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/tqdm/tqdm/tk.py
--rw-rw-rw-   0        0        0     9533 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/tqdm/tqdm/utils.py
--rw-rw-rw-   0        0        0      333 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/tqdm/tqdm/version.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:17.317452 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml/
--rw-rw-rw-   0        0        0     1101 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml/LICENSE
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:17.339901 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml/yaml/
--rw-rw-rw-   0        0        0    13170 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml/yaml/__init__.py
--rw-rw-rw-   0        0        0     4883 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml/yaml/composer.py
--rw-rw-rw-   0        0        0    28639 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml/yaml/constructor.py
--rw-rw-rw-   0        0        0     3851 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml/yaml/cyaml.py
--rw-rw-rw-   0        0        0     2837 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml/yaml/dumper.py
--rw-rw-rw-   0        0        0    43006 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml/yaml/emitter.py
--rw-rw-rw-   0        0        0     2533 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml/yaml/error.py
--rw-rw-rw-   0        0        0     2445 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml/yaml/events.py
--rw-rw-rw-   0        0        0     2061 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml/yaml/loader.py
--rw-rw-rw-   0        0        0     1440 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml/yaml/nodes.py
--rw-rw-rw-   0        0        0    25495 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml/yaml/parser.py
--rw-rw-rw-   0        0        0     6794 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml/yaml/reader.py
--rw-rw-rw-   0        0        0    14184 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml/yaml/representer.py
--rw-rw-rw-   0        0        0     8999 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml/yaml/resolver.py
--rw-rw-rw-   0        0        0    51277 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml/yaml/scanner.py
--rw-rw-rw-   0        0        0     4165 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml/yaml/serializer.py
--rw-rw-rw-   0        0        0     2573 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml/yaml/tokens.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:17.340878 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml_27/
--rw-rw-rw-   0        0        0     1101 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml_27/LICENSE
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:17.362362 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml_27/yaml/
--rw-rw-rw-   0        0        0     9776 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml_27/yaml/__init__.py
--rw-rw-rw-   0        0        0     4921 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml_27/yaml/composer.py
--rw-rw-rw-   0        0        0    25145 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml_27/yaml/constructor.py
--rw-rw-rw-   0        0        0     3290 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml_27/yaml/cyaml.py
--rw-rw-rw-   0        0        0     2719 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml_27/yaml/dumper.py
--rw-rw-rw-   0        0        0    43298 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml_27/yaml/emitter.py
--rw-rw-rw-   0        0        0     2559 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml_27/yaml/error.py
--rw-rw-rw-   0        0        0     2445 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml_27/yaml/events.py
--rw-rw-rw-   0        0        0     1132 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml_27/yaml/loader.py
--rw-rw-rw-   0        0        0     1440 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml_27/yaml/nodes.py
--rw-rw-rw-   0        0        0    25542 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml_27/yaml/parser.py
--rw-rw-rw-   0        0        0     6746 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml_27/yaml/reader.py
--rw-rw-rw-   0        0        0    17711 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml_27/yaml/representer.py
--rw-rw-rw-   0        0        0     9122 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml_27/yaml/resolver.py
--rw-rw-rw-   0        0        0    52446 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml_27/yaml/scanner.py
--rw-rw-rw-   0        0        0     4171 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml_27/yaml/serializer.py
--rw-rw-rw-   0        0        0     2573 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml_27/yaml/tokens.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:17.363337 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml_35/
--rw-rw-rw-   0        0        0     1101 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml_35/LICENSE
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:17.382870 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml_35/yaml/
--rw-rw-rw-   0        0        0     9607 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml_35/yaml/__init__.py
--rw-rw-rw-   0        0        0     4881 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml_35/yaml/composer.py
--rw-rw-rw-   0        0        0    25554 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml_35/yaml/constructor.py
--rw-rw-rw-   0        0        0     3294 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml_35/yaml/cyaml.py
--rw-rw-rw-   0        0        0     2723 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml_35/yaml/dumper.py
--rw-rw-rw-   0        0        0    42954 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml_35/yaml/emitter.py
--rw-rw-rw-   0        0        0     2533 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml_35/yaml/error.py
--rw-rw-rw-   0        0        0     2445 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml_35/yaml/events.py
--rw-rw-rw-   0        0        0     1138 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml_35/yaml/loader.py
--rw-rw-rw-   0        0        0     1440 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml_35/yaml/nodes.py
--rw-rw-rw-   0        0        0    25495 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml_35/yaml/parser.py
--rw-rw-rw-   0        0        0     6854 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml_35/yaml/reader.py
--rw-rw-rw-   0        0        0    14097 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml_35/yaml/representer.py
--rw-rw-rw-   0        0        0     8970 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml_35/yaml/resolver.py
--rw-rw-rw-   0        0        0    51695 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml_35/yaml/scanner.py
--rw-rw-rw-   0        0        0     4165 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml_35/yaml/serializer.py
--rw-rw-rw-   0        0        0     2573 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml_35/yaml/tokens.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:17.386778 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/zstd/
--rw-rw-rw-   0        0        0     1530 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/zstd/LICENSE.txt
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:17.408257 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/zstd/common/
--rw-rw-rw-   0        0        0    18198 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/zstd/common/bitstream.h
--rw-rw-rw-   0        0        0    10157 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/zstd/common/compiler.h
--rw-rw-rw-   0        0        0     4455 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/zstd/common/cpu.h
--rw-rw-rw-   0        0        0     3763 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/zstd/common/debug.h
--rw-rw-rw-   0        0        0    13662 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/zstd/common/entropy_common.c
--rw-rw-rw-   0        0        0     3009 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/zstd/common/error_private.c
--rw-rw-rw-   0        0        0     2441 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/zstd/common/error_private.h
--rw-rw-rw-   0        0        0    34422 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/zstd/common/fse.h
--rw-rw-rw-   0        0        0    14748 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/zstd/common/fse_decompress.c
--rw-rw-rw-   0        0        0    20216 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/zstd/common/huf.h
--rw-rw-rw-   0        0        0    13930 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/zstd/common/mem.h
--rw-rw-rw-   0        0        0    26976 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/zstd/common/xxhash.c
--rw-rw-rw-   0        0        0    11706 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/zstd/common/xxhash.h
--rw-rw-rw-   0        0        0     2728 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/zstd/common/zstd_common.c
--rw-rw-rw-   0        0        0     2497 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/zstd/common/zstd_deps.h
--rw-rw-rw-   0        0        0     3828 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/zstd/common/zstd_errors.h
--rw-rw-rw-   0        0        0    15880 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/zstd/common/zstd_internal.h
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:17.415110 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/zstd/decompress/
--rw-rw-rw-   0        0        0    54982 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/zstd/decompress/huf_decompress.c
--rw-rw-rw-   0        0        0     9164 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.c
--rw-rw-rw-   0        0        0     1321 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.h
--rw-rw-rw-   0        0        0    80283 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/zstd/decompress/zstd_decompress.c
--rw-rw-rw-   0        0        0    66784 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.c
--rw-rw-rw-   0        0        0     2253 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.h
--rw-rw-rw-   0        0        0     7906 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_internal.h
--rw-rw-rw-   0        0        0   138334 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/zstd/zstd.h
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:17.566455 Nuitka-winsvc-1.7.5/nuitka/build/static_src/
--rw-rw-rw-   0        0        0    82114 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/CompiledAsyncgenType.c
--rw-rw-rw-   0        0        0     8250 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/CompiledCellType.c
--rw-rw-rw-   0        0        0    56307 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/CompiledCodeHelpers.c
--rw-rw-rw-   0        0        0    70973 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/CompiledCoroutineType.c
--rw-rw-rw-   0        0        0    35861 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/CompiledFrameType.c
--rw-rw-rw-   0        0        0   100376 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/CompiledFunctionType.c
--rw-rw-rw-   0        0        0    60649 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/CompiledGeneratorType.c
--rw-rw-rw-   0        0        0    48526 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/CompiledGeneratorTypeUncompiledIntegration.c
--rw-rw-rw-   0        0        0    21638 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/CompiledMethodType.c
--rw-rw-rw-   0        0        0    18993 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersAllocator.c
--rw-rw-rw-   0        0        0    37540 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersAttributes.c
--rw-rw-rw-   0        0        0    21783 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersBuiltin.c
--rw-rw-rw-   0        0        0   107641 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersBuiltinTypeMethods.c
--rw-rw-rw-   0        0        0     3033 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersBytes.c
--rw-rw-rw-   0        0        0    13057 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersCalling.c
--rw-rw-rw-   0        0        0   470655 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersCallingGenerated.c
--rw-rw-rw-   0        0        0     1617 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersChecksumTools.c
--rw-rw-rw-   0        0        0     2991 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersClasses.c
--rw-rw-rw-   0        0        0   317872 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersComparisonEq.c
--rw-rw-rw-   0        0        0     4673 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersComparisonEqUtils.c
--rw-rw-rw-   0        0        0   313003 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersComparisonGe.c
--rw-rw-rw-   0        0        0   312414 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersComparisonGt.c
--rw-rw-rw-   0        0        0   316217 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersComparisonLe.c
--rw-rw-rw-   0        0        0   315628 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersComparisonLt.c
--rw-rw-rw-   0        0        0   314618 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersComparisonNe.c
--rw-rw-rw-   0        0        0    36068 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersConstantsBlob.c
--rw-rw-rw-   0        0        0    19313 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersDeepcopy.c
--rw-rw-rw-   0        0        0    38364 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersDictionaries.c
--rw-rw-rw-   0        0        0    24295 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersDictionariesGenerated.c
--rw-rw-rw-   0        0        0     7035 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersExceptions.c
--rw-rw-rw-   0        0        0     6668 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersFiles.c
--rw-rw-rw-   0        0        0    28131 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersFilesystemPaths.c
--rw-rw-rw-   0        0        0     2426 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersFloats.c
--rw-rw-rw-   0        0        0     1774 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersHeapStorage.c
--rw-rw-rw-   0        0        0    14585 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersImport.c
--rw-rw-rw-   0        0        0    14756 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersImportHard.c
--rw-rw-rw-   0        0        0    18433 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersLists.c
--rw-rw-rw-   0        0        0    13915 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersListsGenerated.c
--rw-rw-rw-   0        0        0     1640 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersMappings.c
--rw-rw-rw-   0        0        0     3513 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersMatching.c
--rw-rw-rw-   0        0        0   181243 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersOperationBinaryAdd.c
--rw-rw-rw-   0        0        0    16700 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersOperationBinaryAddUtils.c
--rw-rw-rw-   0        0        0    77943 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersOperationBinaryBitand.c
--rw-rw-rw-   0        0        0    77782 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersOperationBinaryBitor.c
--rw-rw-rw-   0        0        0    77943 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersOperationBinaryBitxor.c
--rw-rw-rw-   0        0        0    67487 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersOperationBinaryDivmod.c
--rw-rw-rw-   0        0        0     1236 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersOperationBinaryDivmodUtils.c
--rw-rw-rw-   0        0        0    68748 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersOperationBinaryFloordiv.c
--rw-rw-rw-   0        0        0     6274 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersOperationBinaryInplaceAdd.c
--rw-rw-rw-   0        0        0    83405 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersOperationBinaryLshift.c
--rw-rw-rw-   0        0        0    13776 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersOperationBinaryMatmult.c
--rw-rw-rw-   0        0        0   183202 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersOperationBinaryMod.c
--rw-rw-rw-   0        0        0   188514 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersOperationBinaryMult.c
--rw-rw-rw-   0        0        0     3404 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersOperationBinaryMultUtils.c
--rw-rw-rw-   0        0        0    66453 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersOperationBinaryOlddiv.c
--rw-rw-rw-   0        0        0    78891 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersOperationBinaryPow.c
--rw-rw-rw-   0        0        0     1023 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersOperationBinaryPowUtils.c
--rw-rw-rw-   0        0        0    77305 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersOperationBinaryRshift.c
--rw-rw-rw-   0        0        0    70465 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersOperationBinarySub.c
--rw-rw-rw-   0        0        0    68005 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersOperationBinaryTruediv.c
--rw-rw-rw-   0        0        0   149580 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersOperationInplaceAdd.c
--rw-rw-rw-   0        0        0     4071 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersOperationInplaceAddUtils.c
--rw-rw-rw-   0        0        0    53224 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersOperationInplaceBitand.c
--rw-rw-rw-   0        0        0    53122 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersOperationInplaceBitor.c
--rw-rw-rw-   0        0        0    53224 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersOperationInplaceBitxor.c
--rw-rw-rw-   0        0        0    76512 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersOperationInplaceFloordiv.c
--rw-rw-rw-   0        0        0    47568 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersOperationInplaceLshift.c
--rw-rw-rw-   0        0        0    17742 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersOperationInplaceMatmult.c
--rw-rw-rw-   0        0        0   136100 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersOperationInplaceMod.c
--rw-rw-rw-   0        0        0   142211 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersOperationInplaceMult.c
--rw-rw-rw-   0        0        0    74142 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersOperationInplaceOlddiv.c
--rw-rw-rw-   0        0        0    82669 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersOperationInplacePow.c
--rw-rw-rw-   0        0        0    45052 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersOperationInplaceRshift.c
--rw-rw-rw-   0        0        0    82842 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersOperationInplaceSub.c
--rw-rw-rw-   0        0        0    76343 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersOperationInplaceTruediv.c
--rw-rw-rw-   0        0        0     3219 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersProfiling.c
--rw-rw-rw-   0        0        0     3805 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersPythonPgo.c
--rw-rw-rw-   0        0        0    15369 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersRaising.c
--rw-rw-rw-   0        0        0     3758 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersSafeStrings.c
--rw-rw-rw-   0        0        0     3730 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersSequences.c
--rw-rw-rw-   0        0        0     1946 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersSlices.c
--rw-rw-rw-   0        0        0    26642 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersStrings.c
--rw-rw-rw-   0        0        0     4037 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersTuples.c
--rw-rw-rw-   0        0        0     5578 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersTypes.c
--rw-rw-rw-   0        0        0    11986 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/InspectPatcher.c
--rw-rw-rw-   0        0        0    47833 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/MainProgram.c
--rw-rw-rw-   0        0        0    58634 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/MetaPathBasedLoader.c
--rw-rw-rw-   0        0        0     4537 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/MetaPathBasedLoaderImportlibMetadataDistribution.c
--rw-rw-rw-   0        0        0     6427 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/MetaPathBasedLoaderResourceReader.c
--rw-rw-rw-   0        0        0    17285 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/MetaPathBasedLoaderResourceReaderFiles.c
--rw-rw-rw-   0        0        0    36107 2023-07-18 02:50:41.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/OnefileBootstrap.c
--rw-rw-rw-   0        0        0     8021 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/nuitka/build/static_src/OnefileSplashScreen.cpp
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:17.646527 Nuitka-winsvc-1.7.5/nuitka/code_generation/
--rw-rw-rw-   0        0        0     6414 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/AsyncgenCodes.py
--rw-rw-rw-   0        0        0    10599 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/AttributeCodes.py
--rw-rw-rw-   0        0        0    21864 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/BinaryOperationHelperDefinitions.py
--rw-rw-rw-   0        0        0     2339 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/BranchCodes.py
--rw-rw-rw-   0        0        0    16009 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/BuiltinCodes.py
--rw-rw-rw-   0        0        0    35905 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/CallCodes.py
--rw-rw-rw-   0        0        0     4896 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/ClassCodes.py
--rw-rw-rw-   0        0        0    51441 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/CodeGeneration.py
--rw-rw-rw-   0        0        0     2375 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/CodeHelperSelection.py
--rw-rw-rw-   0        0        0    14392 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/CodeHelpers.py
--rw-rw-rw-   0        0        0     4879 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/CodeObjectCodes.py
--rw-rw-rw-   0        0        0    17570 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/ComparisonCodes.py
--rw-rw-rw-   0        0        0     4446 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/ComparisonHelperDefinitions.py
--rw-rw-rw-   0        0        0     7335 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/ConditionalCodes.py
--rw-rw-rw-   0        0        0     6539 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/ConstantCodes.py
--rw-rw-rw-   0        0        0    31186 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/Contexts.py
--rw-rw-rw-   0        0        0     8484 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/CoroutineCodes.py
--rw-rw-rw-   0        0        0     1574 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/CtypesCodes.py
--rw-rw-rw-   0        0        0    28478 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/DictCodes.py
--rw-rw-rw-   0        0        0     2125 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/Emission.py
--rw-rw-rw-   0        0        0     9325 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/ErrorCodes.py
--rw-rw-rw-   0        0        0    12304 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/EvalCodes.py
--rw-rw-rw-   0        0        0     8975 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/ExceptionCodes.py
--rw-rw-rw-   0        0        0     7350 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/ExpressionCTypeSelectionHelpers.py
--rw-rw-rw-   0        0        0     2093 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/ExpressionCodes.py
--rw-rw-rw-   0        0        0    17725 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/FrameCodes.py
--rw-rw-rw-   0        0        0    27968 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/FunctionCodes.py
--rw-rw-rw-   0        0        0     7690 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/GeneratorCodes.py
--rw-rw-rw-   0        0        0     5943 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/GlobalConstants.py
--rw-rw-rw-   0        0        0     6911 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/GlobalsLocalsCodes.py
--rw-rw-rw-   0        0        0     1794 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/IdCodes.py
--rw-rw-rw-   0        0        0    13318 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/ImportCodes.py
--rw-rw-rw-   0        0        0     1396 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/Indentation.py
--rw-rw-rw-   0        0        0     1506 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/IndexCodes.py
--rw-rw-rw-   0        0        0     1033 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/InjectCCodes.py
--rw-rw-rw-   0        0        0     3432 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/IntegerCodes.py
--rw-rw-rw-   0        0        0    12010 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/IteratorCodes.py
--rw-rw-rw-   0        0        0     2022 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/LabelCodes.py
--rw-rw-rw-   0        0        0     2612 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/LineNumberCodes.py
--rw-rw-rw-   0        0        0    15906 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/ListCodes.py
--rw-rw-rw-   0        0        0     6375 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/LoaderCodes.py
--rw-rw-rw-   0        0        0     9951 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/LocalsDictCodes.py
--rw-rw-rw-   0        0        0     3135 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/LoopCodes.py
--rw-rw-rw-   0        0        0     1597 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/MatchCodes.py
--rw-rw-rw-   0        0        0     6291 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/ModuleCodes.py
--rw-rw-rw-   0        0        0     8118 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/Namify.py
--rw-rw-rw-   0        0        0    12777 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/OperationCodes.py
--rw-rw-rw-   0        0        0    29459 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/PackageResourceCodes.py
--rw-rw-rw-   0        0        0     3021 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/PrintCodes.py
--rw-rw-rw-   0        0        0     5474 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/PythonAPICodes.py
--rw-rw-rw-   0        0        0    13095 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/RaisingCodes.py
--rw-rw-rw-   0        0        0     3443 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/Reports.py
--rw-rw-rw-   0        0        0     5234 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/ReturnCodes.py
--rw-rw-rw-   0        0        0     6517 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/SetCodes.py
--rw-rw-rw-   0        0        0    13949 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/SliceCodes.py
--rw-rw-rw-   0        0        0     9809 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/StringCodes.py
--rw-rw-rw-   0        0        0     8188 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/SubscriptCodes.py
--rw-rw-rw-   0        0        0    11176 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/TryCodes.py
--rw-rw-rw-   0        0        0     3786 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/TupleCodes.py
--rw-rw-rw-   0        0        0    14717 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/VariableCodes.py
--rw-rw-rw-   0        0        0     9121 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/VariableDeclarations.py
--rw-rw-rw-   0        0        0     8099 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/YieldCodes.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:17.662151 Nuitka-winsvc-1.7.5/nuitka/code_generation/c_types/
--rw-rw-rw-   0        0        0     6069 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/c_types/CTypeBases.py
--rw-rw-rw-   0        0        0     3399 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/c_types/CTypeBooleans.py
--rw-rw-rw-   0        0        0     1804 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/c_types/CTypeCFloats.py
--rw-rw-rw-   0        0        0     1378 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/c_types/CTypeCLongs.py
--rw-rw-rw-   0        0        0     3610 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/c_types/CTypeModuleDictVariables.py
--rw-rw-rw-   0        0        0     5128 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/c_types/CTypeNuitkaBooleans.py
--rw-rw-rw-   0        0        0     5211 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/c_types/CTypeNuitkaInts.py
--rw-rw-rw-   0        0        0     3955 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/c_types/CTypeNuitkaVoids.py
--rw-rw-rw-   0        0        0    19628 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/c_types/CTypePyObjectPointers.py
--rw-rw-rw-   0        0        0     2852 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/c_types/CTypeVoids.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/c_types/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:17.679729 Nuitka-winsvc-1.7.5/nuitka/code_generation/templates/
--rw-rw-rw-   0        0        0     2845 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/templates/CodeTemplatesAsyncgens.py
--rw-rw-rw-   0        0        0     5865 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/templates/CodeTemplatesConstants.py
--rw-rw-rw-   0        0        0     2921 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/templates/CodeTemplatesCoroutines.py
--rw-rw-rw-   0        0        0     2290 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/templates/CodeTemplatesExceptions.py
--rw-rw-rw-   0        0        0     6339 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/templates/CodeTemplatesFrames.py
--rw-rw-rw-   0        0        0     3321 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/templates/CodeTemplatesFunction.py
--rw-rw-rw-   0        0        0     3306 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/templates/CodeTemplatesGeneratorFunction.py
--rw-rw-rw-   0        0        0     2335 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/templates/CodeTemplatesIterators.py
--rw-rw-rw-   0        0        0     4217 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/templates/CodeTemplatesLoader.py
--rw-rw-rw-   0        0        0    21244 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/templates/CodeTemplatesModules.py
--rw-rw-rw-   0        0        0     6640 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/templates/CodeTemplatesVariables.py
--rw-rw-rw-   0        0        0     2475 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/templates/TemplateDebugWrapper.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/templates/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:17.723671 Nuitka-winsvc-1.7.5/nuitka/code_generation/templates_c/
--rw-rw-rw-   0        0        0    11231 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/templates_c/CodeTemplateCallsMethodPositional.c.j2
--rw-rw-rw-   0        0        0     5847 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/templates_c/CodeTemplateCallsMixed.c.j2
--rw-rw-rw-   0        0        0    23760 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/templates_c/CodeTemplateCallsPositional.c.j2
--rw-rw-rw-   0        0        0     5238 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/templates_c/CodeTemplateCallsPositionalMethodDescr.c.j2
--rw-rw-rw-   0        0        0     1905 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/templates_c/CodeTemplateMakeListHinted.c.j2
--rw-rw-rw-   0        0        0     1843 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/templates_c/CodeTemplateMakeListSmall.c.j2
--rw-rw-rw-   0        0        0     2817 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/templates_c/HelperBuiltinMethodOperation.c.j2
--rw-rw-rw-   0        0        0    12819 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/templates_c/HelperDictionaryCopy.c.j2
--rw-rw-rw-   0        0        0     2044 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/templates_c/HelperImportHard.c.j2
--rw-rw-rw-   0        0        0     2762 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/templates_c/HelperLongTools.c.j2
--rw-rw-rw-   0        0        0     1544 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/templates_c/HelperObjectTools.c.j2
--rw-rw-rw-   0        0        0     7197 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/templates_c/HelperOperationBinary.c.j2
--rw-rw-rw-   0        0        0    12850 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/templates_c/HelperOperationComparison.c.j2
--rw-rw-rw-   0        0        0     4288 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/templates_c/HelperOperationComparisonBytes.c.j2
--rw-rw-rw-   0        0        0     2088 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/templates_c/HelperOperationComparisonFloat.c.j2
--rw-rw-rw-   0        0        0     2118 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/templates_c/HelperOperationComparisonInt.c.j2
--rw-rw-rw-   0        0        0     3933 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/templates_c/HelperOperationComparisonList.c.j2
--rw-rw-rw-   0        0        0     7407 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/templates_c/HelperOperationComparisonLong.c.j2
--rw-rw-rw-   0        0        0     4292 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/templates_c/HelperOperationComparisonStr.c.j2
--rw-rw-rw-   0        0        0     3860 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/templates_c/HelperOperationComparisonTuple.c.j2
--rw-rw-rw-   0        0        0     4487 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/templates_c/HelperOperationComparisonUnicode.c.j2
--rw-rw-rw-   0        0        0    11579 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/templates_c/HelperOperationInplace.c.j2
--rw-rw-rw-   0        0        0    19317 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/templates_c/HelperSlotsBinary.c.j2
--rw-rw-rw-   0        0        0     2843 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/templates_c/HelperSlotsBytes.c.j2
--rw-rw-rw-   0        0        0     3635 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/templates_c/HelperSlotsCommon.c.j2
--rw-rw-rw-   0        0        0    11102 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/templates_c/HelperSlotsFloat.c.j2
--rw-rw-rw-   0        0        0    15380 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/templates_c/HelperSlotsInt.c.j2
--rw-rw-rw-   0        0        0     2979 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/templates_c/HelperSlotsList.c.j2
--rw-rw-rw-   0        0        0    10421 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/templates_c/HelperSlotsLong.c.j2
--rw-rw-rw-   0        0        0     2557 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/templates_c/HelperSlotsSet.c.j2
--rw-rw-rw-   0        0        0     3020 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/templates_c/HelperSlotsStr.c.j2
--rw-rw-rw-   0        0        0     2984 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/templates_c/HelperSlotsTuple.c.j2
--rw-rw-rw-   0        0        0     3173 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/code_generation/templates_c/HelperSlotsUnicode.c.j2
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:17.728554 Nuitka-winsvc-1.7.5/nuitka/containers/
--rw-rw-rw-   0        0        0     1435 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/containers/Namedtuples.py
--rw-rw-rw-   0        0        0     6553 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/containers/OrderedDicts.py
--rw-rw-rw-   0        0        0      554 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/containers/OrderedSets.py
--rw-rw-rw-   0        0        0     4397 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/containers/OrderedSetsFallback.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/containers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:17.731484 Nuitka-winsvc-1.7.5/nuitka/distutils/
--rw-rw-rw-   0        0        0     1964 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/distutils/Build.py
--rw-rw-rw-   0        0        0    14219 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/distutils/DistutilCommands.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/distutils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:17.735397 Nuitka-winsvc-1.7.5/nuitka/finalizations/
--rw-rw-rw-   0        0        0     1224 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/finalizations/Finalization.py
--rw-rw-rw-   0        0        0     6110 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/finalizations/FinalizeMarkups.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/finalizations/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:17.747108 Nuitka-winsvc-1.7.5/nuitka/freezer/
--rw-rw-rw-   0        0        0     7311 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/freezer/DependsExe.py
--rw-rw-rw-   0        0        0     2584 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/freezer/DllDependenciesCommon.py
--rw-rw-rw-   0        0        0    11494 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/nuitka/freezer/DllDependenciesMacOS.py
--rw-rw-rw-   0        0        0     7211 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/freezer/DllDependenciesPosix.py
--rw-rw-rw-   0        0        0     6620 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/freezer/DllDependenciesWin32.py
--rw-rw-rw-   0        0        0    17058 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/nuitka/freezer/IncludedDataFiles.py
--rw-rw-rw-   0        0        0     9492 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/freezer/IncludedEntryPoints.py
--rw-rw-rw-   0        0        0     9980 2023-07-18 02:15:00.000000 Nuitka-winsvc-1.7.5/nuitka/freezer/Onefile.py
--rw-rw-rw-   0        0        0    26319 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/freezer/Standalone.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/freezer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:17.756872 Nuitka-winsvc-1.7.5/nuitka/importing/
--rw-rw-rw-   0        0        0    11007 2023-06-25 05:57:17.000000 Nuitka-winsvc-1.7.5/nuitka/importing/IgnoreListing.py
--rw-rw-rw-   0        0        0     2899 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/importing/ImportCache.py
--rw-rw-rw-   0        0        0     6719 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/nuitka/importing/ImportResolving.py
--rw-rw-rw-   0        0        0    28463 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/importing/Importing.py
--rw-rw-rw-   0        0        0     4738 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/importing/PreloadedPackages.py
--rw-rw-rw-   0        0        0    14918 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/nuitka/importing/Recursion.py
--rw-rw-rw-   0        0        0    10981 2023-06-16 02:35:34.000000 Nuitka-winsvc-1.7.5/nuitka/importing/StandardLibrary.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/importing/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:17.861359 Nuitka-winsvc-1.7.5/nuitka/nodes/
--rw-rw-rw-   0        0        0     3637 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/AsyncgenNodes.py
--rw-rw-rw-   0        0        0     4082 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/AttributeLookupNodes.py
--rw-rw-rw-   0        0        0    13567 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/AttributeNodes.py
--rw-rw-rw-   0        0        0   378745 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/AttributeNodesGenerated.py
--rw-rw-rw-   0        0        0     3823 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/BuiltinAllNodes.py
--rw-rw-rw-   0        0        0     4098 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/BuiltinAnyNodes.py
--rw-rw-rw-   0        0        0     2496 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/BuiltinComplexNodes.py
--rw-rw-rw-   0        0        0     1698 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/BuiltinDecodingNodes.py
--rw-rw-rw-   0        0        0     2727 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/BuiltinDecoratorNodes.py
--rw-rw-rw-   0        0        0     4694 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/BuiltinDictNodes.py
--rw-rw-rw-   0        0        0     4948 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/BuiltinFormatNodes.py
--rw-rw-rw-   0        0        0     2142 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/BuiltinHashNodes.py
--rw-rw-rw-   0        0        0     5334 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/BuiltinIntegerNodes.py
--rw-rw-rw-   0        0        0    12723 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/BuiltinIteratorNodes.py
--rw-rw-rw-   0        0        0     1996 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/BuiltinLenNodes.py
--rw-rw-rw-   0        0        0     3606 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/BuiltinNextNodes.py
--rw-rw-rw-   0        0        0     3240 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/BuiltinOpenNodes.py
--rw-rw-rw-   0        0        0   245536 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/BuiltinOperationNodeBasesGenerated.py
--rw-rw-rw-   0        0        0    18589 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/BuiltinRangeNodes.py
--rw-rw-rw-   0        0        0     9067 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/BuiltinRefNodes.py
--rw-rw-rw-   0        0        0     3307 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/BuiltinSumNodes.py
--rw-rw-rw-   0        0        0    13543 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/BuiltinTypeNodes.py
--rw-rw-rw-   0        0        0     1573 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/BuiltinVarsNodes.py
--rw-rw-rw-   0        0        0    26113 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/BytesNodes.py
--rw-rw-rw-   0        0        0     6478 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/CallNodes.py
--rw-rw-rw-   0        0        0     1550 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/Checkers.py
--rw-rw-rw-   0        0        0   604445 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/ChildrenHavingMixins.py
--rw-rw-rw-   0        0        0     8448 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/ClassNodes.py
--rw-rw-rw-   0        0        0     6585 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/CodeObjectSpecs.py
--rw-rw-rw-   0        0        0    21683 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/ComparisonNodes.py
--rw-rw-rw-   0        0        0    30314 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/ConditionalNodes.py
--rw-rw-rw-   0        0        0    46536 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/ConstantRefNodes.py
--rw-rw-rw-   0        0        0    12213 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/ContainerMakingNodes.py
--rw-rw-rw-   0        0        0     2834 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/ContainerOperationNodes.py
--rw-rw-rw-   0        0        0     4581 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/CoroutineNodes.py
--rw-rw-rw-   0        0        0     1714 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/CtypesNodes.py
--rw-rw-rw-   0        0        0    51021 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/DictionaryNodes.py
--rw-rw-rw-   0        0        0     7856 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/ExceptionNodes.py
--rw-rw-rw-   0        0        0     7317 2023-06-25 05:57:17.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/ExecEvalNodes.py
--rw-rw-rw-   0        0        0    44996 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/ExpressionBases.py
--rw-rw-rw-   0        0        0    49273 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/ExpressionBasesGenerated.py
--rw-rw-rw-   0        0        0    21278 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/ExpressionShapeMixins.py
--rw-rw-rw-   0        0        0    12156 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/FrameNodes.py
--rw-rw-rw-   0        0        0     3544 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/FunctionAttributeNodes.py
--rw-rw-rw-   0        0        0    39803 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/FunctionNodes.py
--rw-rw-rw-   0        0        0     5376 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/FutureSpecs.py
--rw-rw-rw-   0        0        0     6256 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/GeneratorNodes.py
--rw-rw-rw-   0        0        0     6850 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/GlobalsLocalsNodes.py
--rw-rw-rw-   0        0        0    76798 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/HardImportNodesGenerated.py
--rw-rw-rw-   0        0        0     5508 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/ImportHardNodes.py
--rw-rw-rw-   0        0        0    45942 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/ImportNodes.py
--rw-rw-rw-   0        0        0     2733 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/IndicatorMixins.py
--rw-rw-rw-   0        0        0     1502 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/InjectCNodes.py
--rw-rw-rw-   0        0        0    11228 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/IterationHandles.py
--rw-rw-rw-   0        0        0    11002 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/KeyValuePairNodes.py
--rw-rw-rw-   0        0        0    16320 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/ListOperationNodes.py
--rw-rw-rw-   0        0        0    23094 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/LocalsDictNodes.py
--rw-rw-rw-   0        0        0    14922 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/LocalsScopes.py
--rw-rw-rw-   0        0        0    15581 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/LoopNodes.py
--rw-rw-rw-   0        0        0     1712 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/MatchNodes.py
--rw-rw-rw-   0        0        0     6534 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/ModuleAttributeNodes.py
--rw-rw-rw-   0        0        0    30972 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/ModuleNodes.py
--rw-rw-rw-   0        0        0    24899 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/NodeBases.py
--rw-rw-rw-   0        0        0    15128 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/NodeMakingHelpers.py
--rw-rw-rw-   0        0        0     5550 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/NodeMetaClasses.py
--rw-rw-rw-   0        0        0    31894 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/OperatorNodes.py
--rw-rw-rw-   0        0        0     9134 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/OperatorNodesUnary.py
--rw-rw-rw-   0        0        0     4202 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/OsSysNodes.py
--rw-rw-rw-   0        0        0    12442 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/OutlineNodes.py
--rw-rw-rw-   0        0        0    31534 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/PackageMetadataNodes.py
--rw-rw-rw-   0        0        0     7901 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/PackageResourceNodes.py
--rw-rw-rw-   0        0        0     3407 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/PrintNodes.py
--rw-rw-rw-   0        0        0     6772 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/ReturnNodes.py
--rw-rw-rw-   0        0        0     4715 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/SideEffectNodes.py
--rw-rw-rw-   0        0        0    12501 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/SliceNodes.py
--rw-rw-rw-   0        0        0    94880 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/StatementBasesGenerated.py
--rw-rw-rw-   0        0        0     9430 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/StatementNodes.py
--rw-rw-rw-   0        0        0    28658 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/StrNodes.py
--rw-rw-rw-   0        0        0     3504 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/StringConcatenationNodes.py
--rw-rw-rw-   0        0        0     8640 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/SubscriptNodes.py
--rw-rw-rw-   0        0        0    17853 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/TryNodes.py
--rw-rw-rw-   0        0        0     2405 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/TypeMatchNodes.py
--rw-rw-rw-   0        0        0    11061 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/TypeNodes.py
--rw-rw-rw-   0        0        0    39522 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/VariableAssignNodes.py
--rw-rw-rw-   0        0        0    10746 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/VariableDelNodes.py
--rw-rw-rw-   0        0        0     4574 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/VariableNameNodes.py
--rw-rw-rw-   0        0        0    30982 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/VariableRefNodes.py
--rw-rw-rw-   0        0        0     4748 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/VariableReleaseNodes.py
--rw-rw-rw-   0        0        0     3902 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/YieldNodes.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:17.866242 Nuitka-winsvc-1.7.5/nuitka/nodes/shapes/
--rw-rw-rw-   0        0        0   156243 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/shapes/BuiltinTypeShapes.py
--rw-rw-rw-   0        0        0     4387 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/shapes/ControlFlowDescriptions.py
--rw-rw-rw-   0        0        0     4567 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/shapes/ShapeMixins.py
--rw-rw-rw-   0        0        0    42374 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/shapes/StandardShapes.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/nodes/shapes/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:17.877961 Nuitka-winsvc-1.7.5/nuitka/optimizations/
--rw-rw-rw-   0        0        0     3279 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/optimizations/BytecodeDemotion.py
--rw-rw-rw-   0        0        0     3920 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/optimizations/FunctionInlining.py
--rw-rw-rw-   0        0        0     2144 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/optimizations/Graphs.py
--rw-rw-rw-   0        0        0    10762 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/optimizations/Optimization.py
--rw-rw-rw-   0        0        0    52058 2023-06-25 05:57:17.000000 Nuitka-winsvc-1.7.5/nuitka/optimizations/OptimizeBuiltinCalls.py
--rw-rw-rw-   0        0        0     2272 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/optimizations/Tags.py
--rw-rw-rw-   0        0        0    40896 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/optimizations/TraceCollections.py
--rw-rw-rw-   0        0        0    23977 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/optimizations/ValueTraces.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/optimizations/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:17.878937 Nuitka-winsvc-1.7.5/nuitka/pgo/
--rw-rw-rw-   0        0        0     4663 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/pgo/PGO.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/pgo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:17.881867 Nuitka-winsvc-1.7.5/nuitka/plugins/
--rw-rw-rw-   0        0        0    40838 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/nuitka/plugins/PluginBase.py
--rw-rw-rw-   0        0        0    57611 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/nuitka/plugins/Plugins.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/plugins/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:17.923856 Nuitka-winsvc-1.7.5/nuitka/plugins/standard/
--rw-rw-rw-   0        0        0    22510 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/nuitka/plugins/standard/AntiBloatPlugin.py
--rw-rw-rw-   0        0        0     3460 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/plugins/standard/ConsiderPyLintAnnotationsPlugin.py
--rw-rw-rw-   0        0        0    10383 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/nuitka/plugins/standard/DataFilesPlugin.py
--rw-rw-rw-   0        0        0     4404 2023-06-16 02:35:34.000000 Nuitka-winsvc-1.7.5/nuitka/plugins/standard/DelvewheelPlugin.py
--rw-rw-rw-   0        0        0     5675 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/plugins/standard/DillPlugin.py
--rw-rw-rw-   0        0        0    13744 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/nuitka/plugins/standard/DllFilesPlugin.py
--rw-rw-rw-   0        0        0     2062 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/plugins/standard/EnumPlugin.py
--rw-rw-rw-   0        0        0     1905 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/plugins/standard/EventletPlugin.py
--rw-rw-rw-   0        0        0     1880 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/plugins/standard/GeventPlugin.py
--rw-rw-rw-   0        0        0     3482 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/plugins/standard/GiPlugin.py
--rw-rw-rw-   0        0        0     5027 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/plugins/standard/GlfwPlugin.py
--rw-rw-rw-   0        0        0    18335 2023-06-16 02:35:34.000000 Nuitka-winsvc-1.7.5/nuitka/plugins/standard/ImplicitImports.py
--rw-rw-rw-   0        0        0     4948 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/plugins/standard/KivyPlugin.py
--rw-rw-rw-   0        0        0     7239 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/nuitka/plugins/standard/MatplotlibPlugin.py
--rw-rw-rw-   0        0        0     6352 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/nuitka/plugins/standard/MultiprocessingPlugin.py
--rw-rw-rw-   0        0        0     1187 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/plugins/standard/NumpyPlugin.py
--rw-rw-rw-   0        0        0     6595 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/nuitka/plugins/standard/OptionsNannyPlugin.py
--rw-rw-rw-   0        0        0     1917 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/plugins/standard/PbrPlugin.py
--rw-rw-rw-   0        0        0     4665 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/plugins/standard/PkgResourcesPlugin.py
--rw-rw-rw-   0        0        0     6992 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/plugins/standard/PmwPlugin.py
--rw-rw-rw-   0        0        0    50293 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/nuitka/plugins/standard/PySidePyQtPlugin.py
--rw-rw-rw-   0        0        0     2986 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/nuitka/plugins/standard/PywebViewPlugin.py
--rw-rw-rw-   0        0        0     1160 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/plugins/standard/TensorflowPlugin.py
--rw-rw-rw-   0        0        0    12242 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/nuitka/plugins/standard/TkinterPlugin.py
--rw-rw-rw-   0        0        0     1140 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/plugins/standard/TorchPlugin.py
--rw-rw-rw-   0        0        0    10191 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/nuitka/plugins/standard/TransformersPlugin.py
--rw-rw-rw-   0        0        0     1073 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/nuitka/plugins/standard/TrioPlugin.py
--rw-rw-rw-   0        0        0     5640 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/plugins/standard/UpxPlugin.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/plugins/standard/__init__.py
--rw-rw-rw-   0        0        0   164577 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/nuitka/plugins/standard/standard.nuitka-package.config.yml
--rw-rw-rw-   0        0        0     2221 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/nuitka/plugins/standard/stdlib2.nuitka-package.config.yml
--rw-rw-rw-   0        0        0     9940 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/nuitka/plugins/standard/stdlib3.nuitka-package.config.yml
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:17.926786 Nuitka-winsvc-1.7.5/nuitka/reports/
--rw-rw-rw-   0        0        0     2209 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/reports/LicenseReport.rst.j2
--rw-rw-rw-   0        0        0    17538 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/reports/Reports.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/reports/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:17.939480 Nuitka-winsvc-1.7.5/nuitka/specs/
--rw-rw-rw-   0        0        0     5911 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/specs/BuiltinBytesOperationSpecs.py
--rw-rw-rw-   0        0        0     2786 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/specs/BuiltinDictOperationSpecs.py
--rw-rw-rw-   0        0        0     2541 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/specs/BuiltinListOperationSpecs.py
--rw-rw-rw-   0        0        0    26455 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/specs/BuiltinParameterSpecs.py
--rw-rw-rw-   0        0        0     6065 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/specs/BuiltinStrOperationSpecs.py
--rw-rw-rw-   0        0        0     1159 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/specs/BuiltinTypeOperationSpecs.py
--rw-rw-rw-   0        0        0     4802 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/specs/BuiltinUnicodeOperationSpecs.py
--rw-rw-rw-   0        0        0     5263 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/nuitka/specs/HardImportSpecs.py
--rw-rw-rw-   0        0        0    18740 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/specs/ParameterSpecs.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/specs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:17.941433 Nuitka-winsvc-1.7.5/nuitka/tools/
--rw-rw-rw-   0        0        0     1603 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/tools/Basics.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:17.942410 Nuitka-winsvc-1.7.5/nuitka/tools/commercial/
--rw-rw-rw-   0        0        0      815 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/tools/commercial/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:17.945340 Nuitka-winsvc-1.7.5/nuitka/tools/data_composer/
--rw-rw-rw-   0        0        0    14250 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/nuitka/tools/data_composer/DataComposer.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/tools/data_composer/__init__.py
--rw-rw-rw-   0        0        0     1306 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/tools/data_composer/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:17.948271 Nuitka-winsvc-1.7.5/nuitka/tools/environments/
--rw-rw-rw-   0        0        0     2449 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/tools/environments/CreateEnvironment.py
--rw-rw-rw-   0        0        0     3735 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/tools/environments/Virtualenv.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/tools/environments/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:17.949246 Nuitka-winsvc-1.7.5/nuitka/tools/general/
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/tools/general/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:17.953155 Nuitka-winsvc-1.7.5/nuitka/tools/general/dll_report/
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/tools/general/dll_report/__init__.py
--rw-rw-rw-   0        0        0     2366 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/tools/general/dll_report/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:17.955107 Nuitka-winsvc-1.7.5/nuitka/tools/general/find_module/
--rw-rw-rw-   0        0        0     3920 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/nuitka/tools/general/find_module/FindModuleCode.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/tools/general/find_module/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:17.959012 Nuitka-winsvc-1.7.5/nuitka/tools/onefile_compressor/
--rw-rw-rw-   0        0        0    10194 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/tools/onefile_compressor/OnefileCompressor.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/tools/onefile_compressor/__init__.py
--rw-rw-rw-   0        0        0     1311 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/tools/onefile_compressor/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:17.961940 Nuitka-winsvc-1.7.5/nuitka/tools/podman/
--rw-rw-rw-   0        0        0     1872 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/nuitka/tools/podman/Podman.py
--rw-rw-rw-   0        0        0      833 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/nuitka/tools/podman/__init__.py
--rw-rw-rw-   0        0        0     6685 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/nuitka/tools/podman/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:17.963893 Nuitka-winsvc-1.7.5/nuitka/tools/profiler/
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/tools/profiler/__init__.py
--rw-rw-rw-   0        0        0     2529 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/tools/profiler/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:17.966823 Nuitka-winsvc-1.7.5/nuitka/tools/scanning/
--rw-rw-rw-   0        0        0     3344 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/tools/scanning/DisplayPackageDLLs.py
--rw-rw-rw-   0        0        0     2095 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/tools/scanning/DisplayPackageData.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/tools/scanning/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:17.973658 Nuitka-winsvc-1.7.5/nuitka/tools/specialize/
--rw-rw-rw-   0        0        0    51143 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/tools/specialize/CTypeDescriptions.py
--rw-rw-rw-   0        0        0     7685 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/tools/specialize/Common.py
--rw-rw-rw-   0        0        0    39625 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/tools/specialize/SpecializeC.py
--rw-rw-rw-   0        0        0    34664 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/nuitka/tools/specialize/SpecializePython.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.5/nuitka/tools/specialize/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:17.982448 Nuitka-winsvc-1.7.5/nuitka/tools/testing/
--rw-rw-rw-   0        0        0    55396 2023-06-16 02:35:34.000000 Nuitka-winsvc-1.7.5/nuitka/tools/testing/Common.py
--rw-rw-rw-   0        0        0     1483 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/nuitka/tools/testing/Constructs.py
--rw-rw-rw-   0        0        0     8940 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/nuitka/tools/testing/OutputComparison.py
--rw-rw-rw-   0        0        0     1278 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/nuitka/tools/testing/Pythons.py
--rw-rw-rw-   0        0        0     8024 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/nuitka/tools/testing/RuntimeTracing.py
--rw-rw-rw-   0        0        0     5371 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/nuitka/tools/testing/SearchModes.py
--rw-rw-rw-   0        0        0     3375 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/nuitka/tools/testing/Valgrind.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/nuitka/tools/testing/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:17.987335 Nuitka-winsvc-1.7.5/nuitka/tools/testing/check_reference_counts/
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/nuitka/tools/testing/check_reference_counts/__init__.py
--rw-rw-rw-   0        0        0     3064 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/nuitka/tools/testing/check_reference_counts/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:17.989283 Nuitka-winsvc-1.7.5/nuitka/tools/testing/compare_with_cpython/
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/nuitka/tools/testing/compare_with_cpython/__init__.py
--rw-rw-rw-   0        0        0    29429 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/nuitka/tools/testing/compare_with_cpython/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:17.991236 Nuitka-winsvc-1.7.5/nuitka/tools/testing/find_sxs_modules/
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/nuitka/tools/testing/find_sxs_modules/__init__.py
--rw-rw-rw-   0        0        0     1949 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/nuitka/tools/testing/find_sxs_modules/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:17.993190 Nuitka-winsvc-1.7.5/nuitka/tools/testing/measure_construct_performance/
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/nuitka/tools/testing/measure_construct_performance/__init__.py
--rw-rw-rw-   0        0        0     8755 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/nuitka/tools/testing/measure_construct_performance/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:17.995145 Nuitka-winsvc-1.7.5/nuitka/tools/testing/run_nuitka_tests/
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/nuitka/tools/testing/run_nuitka_tests/__init__.py
--rw-rw-rw-   0        0        0    36321 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/nuitka/tools/testing/run_nuitka_tests/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:17.997095 Nuitka-winsvc-1.7.5/nuitka/tools/watch/
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/nuitka/tools/watch/__init__.py
--rw-rw-rw-   0        0        0     9503 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/nuitka/tools/watch/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.046286 Nuitka-winsvc-1.7.5/nuitka/tree/
--rw-rw-rw-   0        0        0    47135 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/nuitka/tree/Building.py
--rw-rw-rw-   0        0        0    74608 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/nuitka/tree/ComplexCallHelperFunctions.py
--rw-rw-rw-   0        0        0     1700 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/nuitka/tree/Extractions.py
--rw-rw-rw-   0        0        0     2572 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/nuitka/tree/InternalModule.py
--rw-rw-rw-   0        0        0     1511 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/nuitka/tree/Operations.py
--rw-rw-rw-   0        0        0     2807 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/nuitka/tree/ReformulationAssertStatements.py
--rw-rw-rw-   0        0        0    42768 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/nuitka/tree/ReformulationAssignmentStatements.py
--rw-rw-rw-   0        0        0     2948 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/nuitka/tree/ReformulationBooleanExpressions.py
--rw-rw-rw-   0        0        0    11693 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/nuitka/tree/ReformulationCallExpressions.py
--rw-rw-rw-   0        0        0    15072 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/nuitka/tree/ReformulationClasses.py
--rw-rw-rw-   0        0        0    37638 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/nuitka/tree/ReformulationClasses3.py
--rw-rw-rw-   0        0        0     6430 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/nuitka/tree/ReformulationComparisonExpressions.py
--rw-rw-rw-   0        0        0    22111 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/nuitka/tree/ReformulationContractionExpressions.py
--rw-rw-rw-   0        0        0    11061 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/nuitka/tree/ReformulationDictionaryCreation.py
--rw-rw-rw-   0        0        0    14607 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/nuitka/tree/ReformulationExecStatements.py
--rw-rw-rw-   0        0        0     7782 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/nuitka/tree/ReformulationForLoopStatements.py
--rw-rw-rw-   0        0        0    30544 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/nuitka/tree/ReformulationFunctionStatements.py
--rw-rw-rw-   0        0        0    13437 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/nuitka/tree/ReformulationImportStatements.py
--rw-rw-rw-   0        0        0     6577 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/nuitka/tree/ReformulationLambdaExpressions.py
--rw-rw-rw-   0        0        0    20962 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/nuitka/tree/ReformulationMatchStatements.py
--rw-rw-rw-   0        0        0     2409 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/nuitka/tree/ReformulationMultidist.py
--rw-rw-rw-   0        0        0     8194 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/nuitka/tree/ReformulationNamespacePackages.py
--rw-rw-rw-   0        0        0     4658 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/nuitka/tree/ReformulationPrintStatements.py
--rw-rw-rw-   0        0        0    15371 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/nuitka/tree/ReformulationSequenceCreation.py
--rw-rw-rw-   0        0        0     4824 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/nuitka/tree/ReformulationSubscriptExpressions.py
--rw-rw-rw-   0        0        0    14615 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/nuitka/tree/ReformulationTryExceptStatements.py
--rw-rw-rw-   0        0        0     6982 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/nuitka/tree/ReformulationTryFinallyStatements.py
--rw-rw-rw-   0        0        0     5674 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/nuitka/tree/ReformulationWhileLoopStatements.py
--rw-rw-rw-   0        0        0    14341 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/nuitka/tree/ReformulationWithStatements.py
--rw-rw-rw-   0        0        0     3088 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/nuitka/tree/ReformulationYieldExpressions.py
--rw-rw-rw-   0        0        0    12746 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/nuitka/tree/SourceHandling.py
--rw-rw-rw-   0        0        0     3757 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/nuitka/tree/SyntaxErrors.py
--rw-rw-rw-   0        0        0    22973 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/nuitka/tree/TreeHelpers.py
--rw-rw-rw-   0        0        0    20012 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/nuitka/tree/VariableClosure.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/nuitka/tree/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.113691 Nuitka-winsvc-1.7.5/nuitka/utils/
--rw-rw-rw-   0        0        0     2655 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/nuitka/utils/AppDirs.py
--rw-rw-rw-   0        0        0     3248 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/nuitka/utils/CStrings.py
--rw-rw-rw-   0        0        0     3653 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/nuitka/utils/CommandLineOptions.py
--rw-rw-rw-   0        0        0     4297 2023-06-16 02:35:34.000000 Nuitka-winsvc-1.7.5/nuitka/utils/Distributions.py
--rw-rw-rw-   0        0        0     5794 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/nuitka/utils/Download.py
--rw-rw-rw-   0        0        0    12645 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/nuitka/utils/Execution.py
--rw-rw-rw-   0        0        0    36129 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/nuitka/utils/FileOperations.py
--rw-rw-rw-   0        0        0     2885 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/nuitka/utils/Hashing.py
--rw-rw-rw-   0        0        0     2362 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/nuitka/utils/Images.py
--rw-rw-rw-   0        0        0     6816 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/nuitka/utils/Importing.py
--rw-rw-rw-   0        0        0     8149 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/nuitka/utils/InstalledPythons.py
--rw-rw-rw-   0        0        0     2224 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/nuitka/utils/InstanceCounters.py
--rw-rw-rw-   0        0        0     4336 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/nuitka/utils/Jinja2.py
--rw-rw-rw-   0        0        0     1238 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/nuitka/utils/Json.py
--rw-rw-rw-   0        0        0     4304 2023-06-16 02:35:34.000000 Nuitka-winsvc-1.7.5/nuitka/utils/MacOSApp.py
--rw-rw-rw-   0        0        0     5040 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/nuitka/utils/MemoryUsage.py
--rw-rw-rw-   0        0        0     9062 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/nuitka/utils/ModuleNames.py
--rw-rw-rw-   0        0        0     4309 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/nuitka/utils/ReExecute.py
--rw-rw-rw-   0        0        0     3815 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/nuitka/utils/Rest.py
--rw-rw-rw-   0        0        0    22701 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/nuitka/utils/SharedLibraries.py
--rw-rw-rw-   0        0        0     3664 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/nuitka/utils/Shebang.py
--rw-rw-rw-   0        0        0     2591 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/nuitka/utils/Signing.py
--rw-rw-rw-   0        0        0     6207 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/nuitka/utils/StaticLibraries.py
--rw-rw-rw-   0        0        0     2602 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/nuitka/utils/ThreadedExecutor.py
--rw-rw-rw-   0        0        0     2772 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/nuitka/utils/Timing.py
--rw-rw-rw-   0        0        0    10826 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/nuitka/utils/Utils.py
--rw-rw-rw-   0        0        0    10574 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/nuitka/utils/WindowsFileUsage.py
--rw-rw-rw-   0        0        0    19540 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/nuitka/utils/WindowsResources.py
--rw-rw-rw-   0        0        0     6108 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/nuitka/utils/Yaml.py
--rw-rw-rw-   0        0        0      833 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/nuitka/utils/__init__.py
--rw-rw-rw-   0        0        0      834 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-18 02:58:18.507221 Nuitka-winsvc-1.7.5/setup.cfg
--rw-rw-rw-   0        0        0    15297 2023-07-18 02:15:00.000000 Nuitka-winsvc-1.7.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.115648 Nuitka-winsvc-1.7.5/tests/
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.223053 Nuitka-winsvc-1.7.5/tests/basics/
--rw-rw-rw-   0        0        0     1766 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/basics/AssertsTest.py
--rw-rw-rw-   0        0        0     5934 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/basics/AssignmentsTest.py
--rw-rw-rw-   0        0        0     5866 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/basics/AssignmentsTest32.py
--rw-rw-rw-   0        0        0     4055 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/basics/BranchingTest.py
--rw-rw-rw-   0        0        0     1104 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/basics/BuiltinOverload.py
--rw-rw-rw-   0        0        0     3749 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/basics/BuiltinSuperTest.py
--rw-rw-rw-   0        0        0    17080 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/basics/BuiltinsTest.py
--rw-rw-rw-   0        0        0      866 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/basics/ClassMinimalTest.py
--rw-rw-rw-   0        0        0     4764 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/basics/ClassesTest.py
--rw-rw-rw-   0        0        0     3414 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/basics/ClassesTest32.py
--rw-rw-rw-   0        0        0     1406 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/basics/ClassesTest34.py
--rw-rw-rw-   0        0        0     4698 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/basics/ComparisonChainsTest.py
--rw-rw-rw-   0        0        0     4639 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/basics/ConstantsTest.py
--rw-rw-rw-   0        0        0      995 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/basics/ConstantsTest27.py
--rw-rw-rw-   0        0        0     1628 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/basics/DecoratorsTest.py
--rw-rw-rw-   0        0        0     2317 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/basics/DefaultParametersTest.py
--rw-rw-rw-   0        0        0     1127 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/basics/DoubleDeletionsTest.py
--rw-rw-rw-   0        0        0      806 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/basics/EmptyModuleTest.py
--rw-rw-rw-   0        0        0    14387 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/basics/ExceptionRaisingTest.py
--rw-rw-rw-   0        0        0      961 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/basics/ExceptionRaisingTest32.py
--rw-rw-rw-   0        0        0     1458 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/basics/ExceptionRaisingTest33.py
--rw-rw-rw-   0        0        0     6747 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/basics/ExecEvalTest.py
--rw-rw-rw-   0        0        0     1417 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/basics/ExtremeClosureTest.py
--rw-rw-rw-   0        0        0     1658 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/basics/FunctionObjectsTest.py
--rw-rw-rw-   0        0        0    12335 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/basics/FunctionsTest.py
--rw-rw-rw-   0        0        0     3603 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/basics/FunctionsTest32.py
--rw-rw-rw-   0        0        0     2627 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/basics/FunctionsTest_2.py
--rw-rw-rw-   0        0        0      890 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/basics/FutureTest32.py
--rw-rw-rw-   0        0        0     5809 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/basics/GeneratorExpressionsTest.py
--rw-rw-rw-   0        0        0     1041 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/basics/GeneratorExpressionsTest_37.py
--rw-rw-rw-   0        0        0     3824 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/basics/GlobalStatementTest.py
--rw-rw-rw-   0        0        0     1286 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/basics/HelloWorldTest_2.py
--rw-rw-rw-   0        0        0     2469 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/basics/ImportingTest.py
--rw-rw-rw-   0        0        0     1296 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/basics/InplaceOperationsTest.py
--rw-rw-rw-   0        0        0     4227 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/basics/InspectionTest.py
--rw-rw-rw-   0        0        0     1504 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/basics/InspectionTest_35.py
--rw-rw-rw-   0        0        0     1618 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/basics/InspectionTest_36.py
--rw-rw-rw-   0        0        0     1671 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/basics/LambdasTest.py
--rw-rw-rw-   0        0        0     2731 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/basics/LateClosureAssignmentTest.py
--rw-rw-rw-   0        0        0     2923 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/basics/ListContractionsTest.py
--rw-rw-rw-   0        0        0     3329 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/basics/LoopingTest.py
--rw-rw-rw-   0        0        0     1536 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/basics/MainProgramsTest.py
--rw-rw-rw-   0        0        0     1925 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/basics/ModuleAttributesTest.py
--rw-rw-rw-   0        0        0     1988 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/basics/OperatorsTest.py
--rw-rw-rw-   0        0        0    14903 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/basics/OrderChecksTest.py
--rw-rw-rw-   0        0        0     1827 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/basics/OrderChecksTest27.py
--rw-rw-rw-   0        0        0     1452 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/basics/OverflowFunctionsTest_2.py
--rw-rw-rw-   0        0        0     5853 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/basics/ParameterErrorsTest.py
--rw-rw-rw-   0        0        0     1899 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/basics/ParameterErrorsTest32.py
--rw-rw-rw-   0        0        0      863 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/basics/PrintFutureTest.py
--rw-rw-rw-   0        0        0     1413 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/basics/PrintingTest_2.py
--rw-rw-rw-   0        0        0      878 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/basics/RecursionTest.py
--rw-rw-rw-   0        0        0    23840 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/basics/ReferencingTest.py
--rw-rw-rw-   0        0        0     2076 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/basics/ReferencingTest27.py
--rw-rw-rw-   0        0        0     7819 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/basics/ReferencingTest33.py
--rw-rw-rw-   0        0        0     4902 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/basics/ReferencingTest35.py
--rw-rw-rw-   0        0        0     5092 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/basics/ReferencingTest36.py
--rw-rw-rw-   0        0        0     2899 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/basics/ReferencingTest_2.py
--rw-rw-rw-   0        0        0     1630 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/basics/SlotsTest.py
--rw-rw-rw-   0        0        0     1159 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/basics/ThreadedGeneratorsTest.py
--rw-rw-rw-   0        0        0    22966 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/basics/TrickAssignmentsTest32.py
--rw-rw-rw-   0        0        0     1541 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/basics/TrickAssignmentsTest35.py
--rw-rw-rw-   0        0        0     1788 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/basics/TrickAssignmentsTest_2.py
--rw-rw-rw-   0        0        0     2086 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/basics/TryContinueFinallyTest.py
--rw-rw-rw-   0        0        0     2212 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/basics/TryExceptContinueTest.py
--rw-rw-rw-   0        0        0     2275 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/basics/TryExceptFinallyTest.py
--rw-rw-rw-   0        0        0     2304 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/basics/TryExceptFramesTest.py
--rw-rw-rw-   0        0        0     2842 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/basics/TryReturnFinallyTest.py
--rw-rw-rw-   0        0        0     2328 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/basics/TryYieldFinallyTest.py
--rw-rw-rw-   0        0        0     1093 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/basics/UnicodeTest.py
--rw-rw-rw-   0        0        0     1877 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/basics/UnpackingTest35.py
--rw-rw-rw-   0        0        0     2095 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/basics/VarargsTest.py
--rw-rw-rw-   0        0        0     4879 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/basics/WithStatementsTest.py
--rw-rw-rw-   0        0        0     3070 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/basics/YieldFromTest33.py
--rw-rw-rw-   0        0        0     3821 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/basics/run_all.py
--rw-rw-rw-   0        0        0     2271 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/basics/run_xml.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.225983 Nuitka-winsvc-1.7.5/tests/onefile/
--rw-rw-rw-   0        0        0     1213 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/onefile/HelloWorldTest.py
--rw-rw-rw-   0        0        0     1307 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/onefile/KeyboardInterruptTest.py
--rw-rw-rw-   0        0        0     5816 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/onefile/run_all.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.241605 Nuitka-winsvc-1.7.5/tests/optimizations/
--rw-rw-rw-   0        0        0      958 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/optimizations/ArgumentTypes.py
--rw-rw-rw-   0        0        0     1055 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/optimizations/Attributes.py
--rw-rw-rw-   0        0        0     1021 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/optimizations/Calls.py
--rw-rw-rw-   0        0        0      921 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/optimizations/Conditions.py
--rw-rw-rw-   0        0        0      909 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/optimizations/DecodingOperations.py
--rw-rw-rw-   0        0        0     1212 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/optimizations/FormatStrings36.py
--rw-rw-rw-   0        0        0     1150 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/optimizations/HardImports.py
--rw-rw-rw-   0        0        0      974 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/optimizations/HardImports_2.py
--rw-rw-rw-   0        0        0      918 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/optimizations/Iterations.py
--rw-rw-rw-   0        0        0     1260 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/optimizations/Len.py
--rw-rw-rw-   0        0        0     2262 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/optimizations/Operations.py
--rw-rw-rw-   0        0        0     1333 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/optimizations/Subscripts.py
--rw-rw-rw-   0        0        0     8736 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/optimizations/run_all.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.242583 Nuitka-winsvc-1.7.5/tests/packages/
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.243560 Nuitka-winsvc-1.7.5/tests/packages/package_import_success_after_failure/
--rw-rw-rw-   0        0        0     2382 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/packages/package_import_success_after_failure/PackageImportSuccessAfterFailure.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.245514 Nuitka-winsvc-1.7.5/tests/packages/package_import_success_after_failure/variable_package/
--rw-rw-rw-   0        0        0      942 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/packages/package_import_success_after_failure/variable_package/SomeModule.py
--rw-rw-rw-   0        0        0     1168 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/packages/package_import_success_after_failure/variable_package/__init__.py
--rw-rw-rw-   0        0        0     3671 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/packages/run_all.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:16.296643 Nuitka-winsvc-1.7.5/tests/packages/sub_package/
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.248444 Nuitka-winsvc-1.7.5/tests/packages/sub_package/kitty/
--rw-rw-rw-   0        0        0     1230 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/packages/sub_package/kitty/__init__.py
--rw-rw-rw-   0        0        0      908 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/packages/sub_package/kitty/bigkitty.py
--rw-rw-rw-   0        0        0      910 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/packages/sub_package/kitty/smallkitty.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.254306 Nuitka-winsvc-1.7.5/tests/packages/sub_package/kitty/speak/
--rw-rw-rw-   0        0        0      929 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/packages/sub_package/kitty/speak/__init__.py
--rw-rw-rw-   0        0        0     1053 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/packages/sub_package/kitty/speak/hello.py
--rw-rw-rw-   0        0        0      966 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/packages/sub_package/kitty/speak/miau.py
--rw-rw-rw-   0        0        0      968 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/packages/sub_package/kitty/speak/purr.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:16.297620 Nuitka-winsvc-1.7.5/tests/packages/top_level_attributes_3/
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.257230 Nuitka-winsvc-1.7.5/tests/packages/top_level_attributes_3/some_package/
--rw-rw-rw-   0        0        0     2336 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/packages/top_level_attributes_3/some_package/__init__.py
--rw-rw-rw-   0        0        0      907 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/packages/top_level_attributes_3/some_package/some_module.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.258208 Nuitka-winsvc-1.7.5/tests/plugins/
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.259184 Nuitka-winsvc-1.7.5/tests/plugins/code_signing/
--rw-rw-rw-   0        0        0     1170 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/plugins/code_signing/CodeSigningMain.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.262114 Nuitka-winsvc-1.7.5/tests/plugins/data_files/
--rw-rw-rw-   0        0        0     1332 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/plugins/data_files/DataFilesMain.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.264070 Nuitka-winsvc-1.7.5/tests/plugins/data_files/data_files_package/
--rw-rw-rw-   0        0        0      924 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/plugins/data_files/data_files_package/__init__.py
--rw-rw-rw-   0        0        0        0 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/tests/plugins/data_files/data_files_package/lala.txt
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.265045 Nuitka-winsvc-1.7.5/tests/plugins/data_files/data_files_package/sub_dir/
--rw-rw-rw-   0        0        0        0 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/tests/plugins/data_files/data_files_package/sub_dir/lulu.txt
--rw-rw-rw-   0        0        0      255 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/tests/plugins/data_files/test_case.nuitka-package.config.yml
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.266997 Nuitka-winsvc-1.7.5/tests/plugins/parameters/
--rw-rw-rw-   0        0        0     1019 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/plugins/parameters/ParametersMain.py
--rw-rw-rw-   0        0        0     2168 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/plugins/parameters/parameter-using-plugin.py
--rw-rw-rw-   0        0        0     3861 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/plugins/run_all.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.267978 Nuitka-winsvc-1.7.5/tests/programs/
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.270906 Nuitka-winsvc-1.7.5/tests/programs/absolute_import/
--rw-rw-rw-   0        0        0      867 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/absolute_import/AbsoluteImportMain.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.274809 Nuitka-winsvc-1.7.5/tests/programs/absolute_import/foobar/
--rw-rw-rw-   0        0        0      796 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/absolute_import/foobar/__init__.py
--rw-rw-rw-   0        0        0     1043 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/absolute_import/foobar/foobar.py
--rw-rw-rw-   0        0        0      879 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/absolute_import/foobar/local.py
--rw-rw-rw-   0        0        0      860 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/absolute_import/foobar/util.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.275785 Nuitka-winsvc-1.7.5/tests/programs/case_imports1/
--rw-rw-rw-   0        0        0      808 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/case_imports1/CasedImportingMain.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.276762 Nuitka-winsvc-1.7.5/tests/programs/case_imports1/path1/
--rw-rw-rw-   0        0        0      798 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/case_imports1/path1/Some_Module.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.277738 Nuitka-winsvc-1.7.5/tests/programs/case_imports1/path1/Some_Package/
--rw-rw-rw-   0        0        0      799 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/case_imports1/path1/Some_Package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.278716 Nuitka-winsvc-1.7.5/tests/programs/case_imports1/path2/
--rw-rw-rw-   0        0        0      798 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/case_imports1/path2/some_module.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.279693 Nuitka-winsvc-1.7.5/tests/programs/case_imports1/path2/some_package/
--rw-rw-rw-   0        0        0      799 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/case_imports1/path2/some_package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.280666 Nuitka-winsvc-1.7.5/tests/programs/case_imports2/
--rw-rw-rw-   0        0        0      808 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/case_imports2/CasedImportingMain.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.282620 Nuitka-winsvc-1.7.5/tests/programs/case_imports2/path1/
--rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/case_imports2/path1/some_module.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.283596 Nuitka-winsvc-1.7.5/tests/programs/case_imports2/path1/some_package/
--rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/case_imports2/path1/some_package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.285553 Nuitka-winsvc-1.7.5/tests/programs/case_imports2/path2/
--rw-rw-rw-   0        0        0      798 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/case_imports2/path2/Some_Module.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.287502 Nuitka-winsvc-1.7.5/tests/programs/case_imports2/path2/Some_Package/
--rw-rw-rw-   0        0        0      799 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/case_imports2/path2/Some_Package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.288481 Nuitka-winsvc-1.7.5/tests/programs/case_imports3/
--rw-rw-rw-   0        0        0     1075 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/case_imports3/CasedImportingMain.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.289456 Nuitka-winsvc-1.7.5/tests/programs/case_imports3/path1/
--rw-rw-rw-   0        0        0      809 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/case_imports3/path1/Some_Module.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.291409 Nuitka-winsvc-1.7.5/tests/programs/case_imports3/path1/Some_Package/
--rw-rw-rw-   0        0        0      810 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/case_imports3/path1/Some_Package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.292390 Nuitka-winsvc-1.7.5/tests/programs/case_imports3/path2/
--rw-rw-rw-   0        0        0      809 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/case_imports3/path2/Some_Module.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.293364 Nuitka-winsvc-1.7.5/tests/programs/case_imports3/path2/Some_Package/
--rw-rw-rw-   0        0        0      810 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/case_imports3/path2/Some_Package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.295317 Nuitka-winsvc-1.7.5/tests/programs/cyclic_imports/
--rw-rw-rw-   0        0        0      801 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/cyclic_imports/CyclicImportsMain.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.299265 Nuitka-winsvc-1.7.5/tests/programs/cyclic_imports/cyclic_importing_package/
--rw-rw-rw-   0        0        0      875 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/cyclic_imports/cyclic_importing_package/Child1.py
--rw-rw-rw-   0        0        0      875 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/cyclic_imports/cyclic_importing_package/Child2.py
--rw-rw-rw-   0        0        0      842 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/cyclic_imports/cyclic_importing_package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.304111 Nuitka-winsvc-1.7.5/tests/programs/dash_import/
--rw-rw-rw-   0        0        0      888 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/dash_import/DashImportMain.py
--rw-rw-rw-   0        0        0      817 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/dash_import/dash-module.py
--rw-rw-rw-   0        0        0      817 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/dash_import/plus+module.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.306056 Nuitka-winsvc-1.7.5/tests/programs/dash_main/
--rw-rw-rw-   0        0        0      809 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/dash_main/Dash-Main.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.307033 Nuitka-winsvc-1.7.5/tests/programs/deep/
--rw-rw-rw-   0        0        0      898 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/deep/DeepProgramMain.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.310939 Nuitka-winsvc-1.7.5/tests/programs/deep/some_package/
--rw-rw-rw-   0        0        0      980 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/deep/some_package/DeepBrother.py
--rw-rw-rw-   0        0        0      909 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/deep/some_package/DeepChild.py
--rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/deep/some_package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.312893 Nuitka-winsvc-1.7.5/tests/programs/deep/some_package/deep_package/
--rw-rw-rw-   0        0        0      876 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/deep/some_package/deep_package/DeepDeepChild.py
--rw-rw-rw-   0        0        0      952 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/deep/some_package/deep_package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.313868 Nuitka-winsvc-1.7.5/tests/programs/dunderinit_imports/
--rw-rw-rw-   0        0        0      794 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/dunderinit_imports/DunderInitImportsMain.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.316798 Nuitka-winsvc-1.7.5/tests/programs/dunderinit_imports/package/
--rw-rw-rw-   0        0        0      797 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/dunderinit_imports/package/SubModule.py
--rw-rw-rw-   0        0        0      857 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/dunderinit_imports/package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.319744 Nuitka-winsvc-1.7.5/tests/programs/import_variants/
--rw-rw-rw-   0        0        0     1005 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/import_variants/ImportVariationsMain.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.325587 Nuitka-winsvc-1.7.5/tests/programs/import_variants/some_package/
--rw-rw-rw-   0        0        0      946 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/import_variants/some_package/Child1.py
--rw-rw-rw-   0        0        0     1098 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/import_variants/some_package/Child2.py
--rw-rw-rw-   0        0        0      822 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/import_variants/some_package/Child3.py
--rw-rw-rw-   0        0        0      994 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/import_variants/some_package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.327539 Nuitka-winsvc-1.7.5/tests/programs/main_raises/
--rw-rw-rw-   0        0        0      911 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/main_raises/ErrorMain.py
--rw-rw-rw-   0        0        0      808 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/main_raises/ErrorRaising.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.330469 Nuitka-winsvc-1.7.5/tests/programs/main_raises2/
--rw-rw-rw-   0        0        0     1080 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/main_raises2/ErrorInFunctionMain.py
--rw-rw-rw-   0        0        0      808 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/main_raises2/ErrorRaising.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.331446 Nuitka-winsvc-1.7.5/tests/programs/module_attributes/
--rw-rw-rw-   0        0        0     1529 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/module_attributes/ModuleAttributesMain.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.333398 Nuitka-winsvc-1.7.5/tests/programs/module_attributes/package_level1/
--rw-rw-rw-   0        0        0     1744 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/module_attributes/package_level1/Nearby1.py
--rw-rw-rw-   0        0        0     1611 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/module_attributes/package_level1/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.337306 Nuitka-winsvc-1.7.5/tests/programs/module_attributes/package_level1/package_level2/
--rw-rw-rw-   0        0        0     1744 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/module_attributes/package_level1/package_level2/Nearby2.py
--rw-rw-rw-   0        0        0     1611 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/module_attributes/package_level1/package_level2/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.340234 Nuitka-winsvc-1.7.5/tests/programs/module_attributes/package_level1/package_level2/package_level3/
--rw-rw-rw-   0        0        0     1744 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/module_attributes/package_level1/package_level2/package_level3/Nearby3.py
--rw-rw-rw-   0        0        0     1611 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/module_attributes/package_level1/package_level2/package_level3/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.342187 Nuitka-winsvc-1.7.5/tests/programs/module_exits/
--rw-rw-rw-   0        0        0      869 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/module_exits/ErrorExitingModule.py
--rw-rw-rw-   0        0        0      867 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/module_exits/Main.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.344139 Nuitka-winsvc-1.7.5/tests/programs/module_object_replacing/
--rw-rw-rw-   0        0        0     1078 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/module_object_replacing/ModuleObjectReplacingMain.py
--rw-rw-rw-   0        0        0     1359 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/module_object_replacing/SelfReplacingModule.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.345116 Nuitka-winsvc-1.7.5/tests/programs/multiprocessing_using/
--rw-rw-rw-   0        0        0      990 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/multiprocessing_using/MultiprocessingUsingMain.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.348045 Nuitka-winsvc-1.7.5/tests/programs/multiprocessing_using/foo/
--rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/multiprocessing_using/foo/__init__.py
--rw-rw-rw-   0        0        0      836 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/multiprocessing_using/foo/__main__.py
--rw-rw-rw-   0        0        0     1758 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/multiprocessing_using/foo/entry.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.349022 Nuitka-winsvc-1.7.5/tests/programs/named_imports/
--rw-rw-rw-   0        0        0      846 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/named_imports/NamedImportsMain.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.350978 Nuitka-winsvc-1.7.5/tests/programs/named_imports/some_package/
--rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/named_imports/some_package/SomeModule.py
--rw-rw-rw-   0        0        0      824 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/named_imports/some_package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.353908 Nuitka-winsvc-1.7.5/tests/programs/named_imports/some_package/sub_package/
--rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/named_imports/some_package/sub_package/SomeModule.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.354883 Nuitka-winsvc-1.7.5/tests/programs/package_code/
--rw-rw-rw-   0        0        0      800 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/package_code/PackageInitCodeMain.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.356835 Nuitka-winsvc-1.7.5/tests/programs/package_code/some_package/
--rw-rw-rw-   0        0        0      810 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/package_code/some_package/SomeModule.py
--rw-rw-rw-   0        0        0      809 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/package_code/some_package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.359765 Nuitka-winsvc-1.7.5/tests/programs/package_contains_main/
--rw-rw-rw-   0        0        0      789 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/package_contains_main/PackageContainsMain.py
--rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/package_contains_main/__init__.py
--rw-rw-rw-   0        0        0      801 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/package_contains_main/local.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.360742 Nuitka-winsvc-1.7.5/tests/programs/package_init_import/
--rw-rw-rw-   0        0        0      823 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/package_init_import/PackageInitImportMain.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.362694 Nuitka-winsvc-1.7.5/tests/programs/package_init_import/some_package/
--rw-rw-rw-   0        0        0     1008 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/package_init_import/some_package/PackageLocal.py
--rw-rw-rw-   0        0        0     1169 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/package_init_import/some_package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.363670 Nuitka-winsvc-1.7.5/tests/programs/package_init_issue/
--rw-rw-rw-   0        0        0      789 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/package_init_issue/PackageInitIssueMain.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.364647 Nuitka-winsvc-1.7.5/tests/programs/package_init_issue/some_package/
--rw-rw-rw-   0        0        0      798 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/package_init_issue/some_package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.366600 Nuitka-winsvc-1.7.5/tests/programs/package_init_issue/some_package/child_package/
--rw-rw-rw-   0        0        0      798 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/package_init_issue/some_package/child_package/SomeModule.py
--rw-rw-rw-   0        0        0      795 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/package_init_issue/some_package/child_package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.368567 Nuitka-winsvc-1.7.5/tests/programs/package_missing_init/
--rw-rw-rw-   0        0        0      926 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/package_missing_init/PackageMissingInitMain.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.370512 Nuitka-winsvc-1.7.5/tests/programs/package_missing_init/some_package/
--rw-rw-rw-   0        0        0      965 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/package_missing_init/some_package/some_module.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.371482 Nuitka-winsvc-1.7.5/tests/programs/package_missing_init/some_package/sub_package/
--rw-rw-rw-   0        0        0      977 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/package_missing_init/some_package/sub_package/some_sub_module.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.373435 Nuitka-winsvc-1.7.5/tests/programs/package_module_collision/
--rw-rw-rw-   0        0        0      901 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/package_module_collision/PackageAndModuleNamedSameMain.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.374412 Nuitka-winsvc-1.7.5/tests/programs/package_module_collision/Something/
--rw-rw-rw-   0        0        0      810 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/package_module_collision/Something/__init__.py
--rw-rw-rw-   0        0        0      801 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/package_module_collision/something.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.375389 Nuitka-winsvc-1.7.5/tests/programs/package_overload/
--rw-rw-rw-   0        0        0      852 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/package_overload/Main.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.378318 Nuitka-winsvc-1.7.5/tests/programs/package_overload/foo/
--rw-rw-rw-   0        0        0      799 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/package_overload/foo/__init__.py
--rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/package_overload/foo/bar.py
--rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/package_overload/foo/bar2.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.379294 Nuitka-winsvc-1.7.5/tests/programs/package_prevents_submodule/
--rw-rw-rw-   0        0        0     2972 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/package_prevents_submodule/PackagePreventsSubmoduleMain.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.381247 Nuitka-winsvc-1.7.5/tests/programs/package_prevents_submodule/some_package/
--rw-rw-rw-   0        0        0     1078 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/package_prevents_submodule/some_package/__init__.py
--rw-rw-rw-   0        0        0      800 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/package_prevents_submodule/some_package/some_module.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:16.323986 Nuitka-winsvc-1.7.5/tests/programs/package_program/
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.383201 Nuitka-winsvc-1.7.5/tests/programs/package_program/PackageAsMain/
--rw-rw-rw-   0        0        0      888 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/package_program/PackageAsMain/__init__.py
--rw-rw-rw-   0        0        0     1630 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/package_program/PackageAsMain/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.384179 Nuitka-winsvc-1.7.5/tests/programs/pkgutil_itermodules/
--rw-rw-rw-   0        0        0     1728 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/pkgutil_itermodules/PkgUtilIterModulesMain.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.387116 Nuitka-winsvc-1.7.5/tests/programs/pkgutil_itermodules/some_package/
--rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/pkgutil_itermodules/some_package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.390036 Nuitka-winsvc-1.7.5/tests/programs/pkgutil_itermodules/some_package/sub_package1/
--rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleC.py
--rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleD.py
--rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/pkgutil_itermodules/some_package/sub_package1/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.392965 Nuitka-winsvc-1.7.5/tests/programs/pkgutil_itermodules/some_package/sub_package2/
--rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleA.py
--rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleB.py
--rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/pkgutil_itermodules/some_package/sub_package2/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.393942 Nuitka-winsvc-1.7.5/tests/programs/pkgutil_usage/
--rw-rw-rw-   0        0        0     1261 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/pkgutil_usage/PkgUtilUsageMain.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.397848 Nuitka-winsvc-1.7.5/tests/programs/pkgutil_usage/package/
--rw-rw-rw-   0        0        0       13 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/tests/programs/pkgutil_usage/package/DATA_FILE.txt
--rw-rw-rw-   0        0        0       14 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/tests/programs/pkgutil_usage/package/DATA_FILE2.txt
--rw-rw-rw-   0        0        0       14 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/tests/programs/pkgutil_usage/package/DATA_FILE3.txt
--rw-rw-rw-   0        0        0     1553 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/pkgutil_usage/package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.398824 Nuitka-winsvc-1.7.5/tests/programs/plugin_import/
--rw-rw-rw-   0        0        0      859 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/plugin_import/PluginImportMain.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.400779 Nuitka-winsvc-1.7.5/tests/programs/plugin_import/some_package/
--rw-rw-rw-   0        0        0      771 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/plugin_import/some_package/__init__.py
--rw-rw-rw-   0        0        0      781 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/plugin_import/some_package/some_module.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.402749 Nuitka-winsvc-1.7.5/tests/programs/reimport_main_dynamic/
--rw-rw-rw-   0        0        0      911 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/reimport_main_dynamic/ImportItselfDynamicMain.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.404684 Nuitka-winsvc-1.7.5/tests/programs/reimport_main_static/
--rw-rw-rw-   0        0        0      898 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/reimport_main_static/ImportItselfStaticMain.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.406636 Nuitka-winsvc-1.7.5/tests/programs/relative_import/
--rw-rw-rw-   0        0        0      842 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/relative_import/RelativeImportMain.py
--rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/relative_import/dircache.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.407613 Nuitka-winsvc-1.7.5/tests/programs/resource_reader37/
--rw-rw-rw-   0        0        0     1169 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/resource_reader37/ResourceReaderMain.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.409566 Nuitka-winsvc-1.7.5/tests/programs/resource_reader37/some_package/
--rw-rw-rw-   0        0        0       13 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.5/tests/programs/resource_reader37/some_package/DATA_FILE.txt
--rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/resource_reader37/some_package/__init__.py
--rw-rw-rw-   0        0        0     6615 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/run_all.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.411519 Nuitka-winsvc-1.7.5/tests/programs/stdlib_overload/
--rw-rw-rw-   0        0        0     1171 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/stdlib_overload/StdlibOverloadMain.py
--rw-rw-rw-   0        0        0      799 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/stdlib_overload/pyexpat.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.414449 Nuitka-winsvc-1.7.5/tests/programs/stdlib_overload/some_package/
--rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/stdlib_overload/some_package/__init__.py
--rw-rw-rw-   0        0        0      909 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/stdlib_overload/some_package/normal_importing.py
--rw-rw-rw-   0        0        0      810 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/stdlib_overload/some_package/pyexpat.py
--rw-rw-rw-   0        0        0     1236 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/stdlib_overload/some_package/star_importing.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.418366 Nuitka-winsvc-1.7.5/tests/programs/syntax_errors/
--rw-rw-rw-   0        0        0      791 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/syntax_errors/IndentationErroring.py
--rw-rw-rw-   0        0        0      800 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/syntax_errors/SyntaxErroring.py
--rw-rw-rw-   0        0        0     1079 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/syntax_errors/SyntaxErrorsMain.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.422263 Nuitka-winsvc-1.7.5/tests/programs/unicode_bom/
--rw-rw-rw-   0        0        0      963 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/unicode_bom/UnicodeBomMain.py
--rw-rw-rw-   0        0        0      846 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/unicode_bom/unicode_bom.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.423237 Nuitka-winsvc-1.7.5/tests/programs/with space/
--rw-rw-rw-   0        0        0      826 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/programs/with space/Space Main.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.424215 Nuitka-winsvc-1.7.5/tests/reflected/
--rw-rw-rw-   0        0        0    14061 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/reflected/compile_itself.py
--rw-rw-rw-   0        0        0     1243 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/run-tests
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.462297 Nuitka-winsvc-1.7.5/tests/standalone/
--rw-rw-rw-   0        0        0     1058 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/standalone/BrotliUsing.py
--rw-rw-rw-   0        0        0     2554 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/standalone/CtypesUsing.py
--rw-rw-rw-   0        0        0     1136 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/standalone/FlaskUsing.py
--rw-rw-rw-   0        0        0      990 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/standalone/GlfwUsing.py
--rw-rw-rw-   0        0        0     1184 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/standalone/GtkUsing.py
--rw-rw-rw-   0        0        0     1025 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/standalone/HexEncodingTest_2.py
--rw-rw-rw-   0        0        0     1086 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/standalone/IdnaUsing.py
--rw-rw-rw-   0        0        0     1151 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/standalone/LxmlUsing.py
--rw-rw-rw-   0        0        0     1431 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/standalone/MatplotlibUsing.py
--rw-rw-rw-   0        0        0     2538 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/standalone/MetadataPackagesUsing.py
--rw-rw-rw-   0        0        0     1727 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/standalone/NumpyUsing.py
--rw-rw-rw-   0        0        0      947 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/standalone/OpenGLUsing.py
--rw-rw-rw-   0        0        0     1379 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/standalone/PandasUsing.py
--rw-rw-rw-   0        0        0     1066 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/standalone/PasslibUsing.py
--rw-rw-rw-   0        0        0     1216 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/tests/standalone/PendulumUsing.py
--rw-rw-rw-   0        0        0     2074 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/standalone/PkgResourcesRequiresUsing.py
--rw-rw-rw-   0        0        0     1067 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/standalone/PmwUsing.py
--rw-rw-rw-   0        0        0     1085 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/standalone/PyQt5Plugins.py
--rw-rw-rw-   0        0        0     1105 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/standalone/PyQt5SSLSupport.py
--rw-rw-rw-   0        0        0     2050 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/standalone/PyQt5Using.py
--rw-rw-rw-   0        0        0     1085 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/standalone/PyQt6Plugins.py
--rw-rw-rw-   0        0        0     2050 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/standalone/PyQt6Using.py
--rw-rw-rw-   0        0        0     1091 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/standalone/PySide6Plugins.py
--rw-rw-rw-   0        0        0     1757 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/standalone/PySide6Using.py
--rw-rw-rw-   0        0        0     1323 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/standalone/RsaUsing.py
--rw-rw-rw-   0        0        0      973 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/standalone/ShlibUsing.py
--rw-rw-rw-   0        0        0     1537 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.5/tests/standalone/SocketUsing.py
--rw-rw-rw-   0        0        0     1941 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/standalone/TkInterUsing.py
--rw-rw-rw-   0        0        0     3228 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/standalone/Urllib3Using.py
--rw-rw-rw-   0        0        0     1200 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/standalone/Win32ComUsing.py
--rw-rw-rw-   0        0        0     9531 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/standalone/run_all.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.463274 Nuitka-winsvc-1.7.5/tests/standalone/zip_importer/
--rw-rw-rw-   0        0        0     1264 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/standalone/zip_importer/ZipImporterMain.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:58:18.504290 Nuitka-winsvc-1.7.5/tests/syntax/
--rw-rw-rw-   0        0        0      811 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/syntax/AsyncgenReturn36.py
--rw-rw-rw-   0        0        0      868 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/syntax/BreakWithoutLoop.py
--rw-rw-rw-   0        0        0      791 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/syntax/ClassReturn.py
--rw-rw-rw-   0        0        0      970 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/syntax/ClosureDel_2.py
--rw-rw-rw-   0        0        0      849 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/syntax/ContinueWithoutLoop.py
--rw-rw-rw-   0        0        0      791 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/syntax/DuplicateArgument.py
--rw-rw-rw-   0        0        0     1111 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/syntax/ExecWithNesting_2.py
--rw-rw-rw-   0        0        0      826 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/syntax/FutureBraces.py
--rw-rw-rw-   0        0        0      805 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/syntax/FutureUnknown.py
--rw-rw-rw-   0        0        0     1041 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/syntax/GeneratorExpressions38.py
--rw-rw-rw-   0        0        0      879 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/syntax/GeneratorReturn_2.py
--rw-rw-rw-   0        0        0      792 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/syntax/GlobalForParameter.py
--rw-rw-rw-   0        0        0      995 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/syntax/Importing32.py
--rw-rw-rw-   0        0        0      799 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/syntax/IndentationError.py
--rw-rw-rw-   0        0        0      915 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/syntax/LateFutureImport.py
--rw-rw-rw-   0        0        0      841 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/syntax/MisplacedFutureImport.py
--rw-rw-rw-   0        0        0      800 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/syntax/ModuleReturn.py
--rw-rw-rw-   0        0        0      883 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/syntax/NonAsciiWithoutEncoding_2.py
--rw-rw-rw-   0        0        0      794 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/syntax/NonlocalForParameter32.py
--rw-rw-rw-   0        0        0      868 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/syntax/NonlocalNotFound32.py
--rw-rw-rw-   0        0        0      908 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/syntax/StarImportExtra.py
--rw-rw-rw-   0        0        0      869 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/syntax/SyntaxError.py
--rw-rw-rw-   0        0        0      874 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/syntax/TryExceptAllNotLast.py
--rw-rw-rw-   0        0        0      875 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/syntax/TryFinallyContinue_37.py
--rw-rw-rw-   0        0        0      776 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/syntax/UnpackNoTuple.py
--rw-rw-rw-   0        0        0      809 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/syntax/UnpackTwoStars32.py
--rw-rw-rw-   0        0        0      793 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/syntax/YieldFromInModule.py
--rw-rw-rw-   0        0        0      804 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/syntax/YieldInAsync35.py
--rw-rw-rw-   0        0        0      923 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/syntax/YieldInGenexp38.py
--rw-rw-rw-   0        0        0      781 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/syntax/YieldInModule.py
--rw-rw-rw-   0        0        0     2203 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.5/tests/syntax/run_all.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:12.029069 Nuitka-winsvc-1.7.6/
+-rw-rw-rw-   0        0        0   843525 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.6/Changelog.rst
+-rw-rw-rw-   0        0        0   152515 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/Developer_Manual.rst
+-rw-rw-rw-   0        0        0    11348 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.6/LICENSE.txt
+-rw-rw-rw-   0        0        0     1733 2023-07-25 02:26:00.000000 Nuitka-winsvc-1.7.6/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:09.848107 Nuitka-winsvc-1.7.6/Nuitka_winsvc.egg-info/
+-rw-rw-rw-   0        0        0     4575 2023-07-25 02:27:09.000000 Nuitka-winsvc-1.7.6/Nuitka_winsvc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    76752 2023-07-25 02:27:09.000000 Nuitka-winsvc-1.7.6/Nuitka_winsvc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 02:27:09.000000 Nuitka-winsvc-1.7.6/Nuitka_winsvc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      308 2023-07-25 02:27:09.000000 Nuitka-winsvc-1.7.6/Nuitka_winsvc.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-03-28 09:21:19.000000 Nuitka-winsvc-1.7.6/Nuitka_winsvc.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       35 2023-07-25 02:27:09.000000 Nuitka-winsvc-1.7.6/Nuitka_winsvc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-25 02:27:09.000000 Nuitka-winsvc-1.7.6/Nuitka_winsvc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4575 2023-07-25 02:27:12.029069 Nuitka-winsvc-1.7.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2651 2023-07-25 02:26:00.000000 Nuitka-winsvc-1.7.6/README.md
+-rw-rw-rw-   0        0        0    76929 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.6/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:09.857872 Nuitka-winsvc-1.7.6/bin/
+-rw-rw-rw-   0        0        0     1135 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/bin/autoformat-nuitka-source
+-rw-rw-rw-   0        0        0     1134 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.6/bin/check-nuitka-with-pylint
+-rw-rw-rw-   0        0        0     1150 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/bin/compare_with_cpython
+-rw-rw-rw-   0        0        0     3079 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/bin/compare_with_xml
+-rw-rw-rw-   0        0        0     1163 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/bin/measure-construct-performance
+-rw-rw-rw-   0        0        0     1685 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/bin/nuitka
+-rw-rw-rw-   0        0        0     1685 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/bin/nuitka-run
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:09.668111 Nuitka-winsvc-1.7.6/doc/
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:09.860801 Nuitka-winsvc-1.7.6/doc/Logo/
+-rw-rw-rw-   0        0        0     7321 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.6/doc/Logo/Nuitka-Logo-Horizontal.svg
+-rw-rw-rw-   0        0        0     7401 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.6/doc/Logo/Nuitka-Logo-Symbol.svg
+-rw-rw-rw-   0        0        0    17917 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.6/doc/Logo/Nuitka-Logo-Vertical.svg
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:09.864710 Nuitka-winsvc-1.7.6/doc/images/
+-rw-rw-rw-   0        0        0     7585 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.6/doc/images/Nuitka-Logo-Horizontal.png
+-rw-rw-rw-   0        0        0     4452 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.6/doc/images/Nuitka-Logo-Symbol.png
+-rw-rw-rw-   0        0        0     9828 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.6/doc/images/Nuitka-Logo-Vertical.png
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:09.867641 Nuitka-winsvc-1.7.6/lib/
+-rw-rw-rw-   0        0        0     4250 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/lib/hints.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:09.869590 Nuitka-winsvc-1.7.6/misc/
+-rwxrwxrwx   0        0        0      901 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/misc/nuitka-run.bat
+-rwxrwxrwx   0        0        0     1038 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/misc/nuitka.bat
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:09.903383 Nuitka-winsvc-1.7.6/nuitka/
+-rw-rw-rw-   0        0        0     7529 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.6/nuitka/Builtins.py
+-rw-rw-rw-   0        0        0     5437 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/BytecodeCaching.py
+-rw-rw-rw-   0        0        0     3440 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/Bytecodes.py
+-rw-rw-rw-   0        0        0     1884 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/CacheCleanup.py
+-rw-rw-rw-   0        0        0    11148 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/Constants.py
+-rw-rw-rw-   0        0        0     2447 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/Errors.py
+-rw-rw-rw-   0        0        0    37438 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.6/nuitka/MainControl.py
+-rw-rw-rw-   0        0        0     8064 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/ModuleRegistry.py
+-rw-rw-rw-   0        0        0    57179 2023-07-25 02:26:00.000000 Nuitka-winsvc-1.7.6/nuitka/OptionParsing.py
+-rw-rw-rw-   0        0        0    67763 2023-07-25 02:26:00.000000 Nuitka-winsvc-1.7.6/nuitka/Options.py
+-rw-rw-rw-   0        0        0     5022 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/OutputDirectories.py
+-rw-rw-rw-   0        0        0    14520 2023-07-25 02:10:30.000000 Nuitka-winsvc-1.7.6/nuitka/PostProcessing.py
+-rw-rw-rw-   0        0        0     5770 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/Progress.py
+-rw-rw-rw-   0        0        0     7472 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/PythonFlavors.py
+-rw-rw-rw-   0        0        0     4061 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/PythonOperators.py
+-rw-rw-rw-   0        0        0    12179 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/PythonVersions.py
+-rw-rw-rw-   0        0        0     9062 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.6/nuitka/Serialization.py
+-rw-rw-rw-   0        0        0     4670 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/SourceCodeReferences.py
+-rw-rw-rw-   0        0        0    11235 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/Tracing.py
+-rw-rw-rw-   0        0        0     3395 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/TreeXML.py
+-rw-rw-rw-   0        0        0    15235 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/Variables.py
+-rw-rw-rw-   0        0        0     2055 2023-07-25 02:10:30.000000 Nuitka-winsvc-1.7.6/nuitka/Version.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/__init__.py
+-rw-rw-rw-   0        0        0     5615 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/__main__.py
+-rw-rw-rw-   0        0        0     5295 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/__past__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:09.922914 Nuitka-winsvc-1.7.6/nuitka/build/
+-rw-rw-rw-   0        0        0    34239 2023-07-25 02:10:30.000000 Nuitka-winsvc-1.7.6/nuitka/build/Backend.scons
+-rw-rw-rw-   0        0        0     8300 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.6/nuitka/build/CCompilerVersion.scons
+-rw-rw-rw-   0        0        0     2716 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.6/nuitka/build/DataComposerInterface.py
+-rw-rw-rw-   0        0        0    18793 2023-07-25 02:26:00.000000 Nuitka-winsvc-1.7.6/nuitka/build/Onefile.scons
+-rw-rw-rw-   0        0        0    15698 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.6/nuitka/build/SconsCaching.py
+-rw-rw-rw-   0        0        0    31022 2023-07-25 02:26:00.000000 Nuitka-winsvc-1.7.6/nuitka/build/SconsCompilerSettings.py
+-rw-rw-rw-   0        0        0     5527 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/SconsHacks.py
+-rw-rw-rw-   0        0        0    15827 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.6/nuitka/build/SconsInterface.py
+-rw-rw-rw-   0        0        0     2671 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.6/nuitka/build/SconsProgress.py
+-rw-rw-rw-   0        0        0    12022 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.6/nuitka/build/SconsSpawn.py
+-rw-rw-rw-   0        0        0    24338 2023-06-16 02:35:34.000000 Nuitka-winsvc-1.7.6/nuitka/build/SconsUtils.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:09.670067 Nuitka-winsvc-1.7.6/nuitka/build/include/
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:09.958127 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/
+-rw-rw-rw-   0        0        0     7972 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/allocator.h
+-rw-rw-rw-   0        0        0     3470 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/builtins.h
+-rw-rw-rw-   0        0        0     4604 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/calling.h
+-rw-rw-rw-   0        0        0     1977 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/checkers.h
+-rw-rw-rw-   0        0        0     1261 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/checksum_tools.h
+-rw-rw-rw-   0        0        0     9571 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/compiled_asyncgen.h
+-rw-rw-rw-   0        0        0     2002 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/compiled_cell.h
+-rw-rw-rw-   0        0        0     9325 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/compiled_coroutine.h
+-rw-rw-rw-   0        0        0    16949 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/compiled_frame.h
+-rw-rw-rw-   0        0        0     5972 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/compiled_function.h
+-rw-rw-rw-   0        0        0     9136 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/compiled_generator.h
+-rw-rw-rw-   0        0        0     1838 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/compiled_method.h
+-rw-rw-rw-   0        0        0     7408 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/constants.h
+-rw-rw-rw-   0        0        0     1293 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/constants_blob.h
+-rw-rw-rw-   0        0        0    34083 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/exceptions.h
+-rw-rw-rw-   0        0        0     3473 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/filesystem_paths.h
+-rw-rw-rw-   0        0        0     6253 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/freelists.h
+-rw-rw-rw-   0        0        0    86326 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/hedley.h
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:10.026552 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/
+-rw-rw-rw-   0        0        0     3393 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/attributes.h
+-rw-rw-rw-   0        0        0     2663 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/boolean.h
+-rw-rw-rw-   0        0        0     1181 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/bytearrays.h
+-rw-rw-rw-   0        0        0     1135 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/bytes.h
+-rw-rw-rw-   0        0        0     9335 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/calling_generated.h
+-rw-rw-rw-   0        0        0    13140 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/comparisons_eq.h
+-rw-rw-rw-   0        0        0    10616 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/comparisons_ge.h
+-rw-rw-rw-   0        0        0    10615 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/comparisons_gt.h
+-rw-rw-rw-   0        0        0    13140 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/comparisons_le.h
+-rw-rw-rw-   0        0        0    13139 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/comparisons_lt.h
+-rw-rw-rw-   0        0        0    10616 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/comparisons_ne.h
+-rw-rw-rw-   0        0        0     1743 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/complex.h
+-rw-rw-rw-   0        0        0    13109 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/dictionaries.h
+-rw-rw-rw-   0        0        0     1206 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/floats.h
+-rw-rw-rw-   0        0        0     3897 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/import_hard.h
+-rw-rw-rw-   0        0        0     1798 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/indexes.h
+-rw-rw-rw-   0        0        0     2941 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/ints.h
+-rw-rw-rw-   0        0        0     9992 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/iterators.h
+-rw-rw-rw-   0        0        0     3411 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/lists.h
+-rw-rw-rw-   0        0        0     1633 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/lists_generated.h
+-rw-rw-rw-   0        0        0     1328 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/mappings.h
+-rw-rw-rw-   0        0        0     4573 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/operations.h
+-rw-rw-rw-   0        0        0    12685 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/operations_binary_add.h
+-rw-rw-rw-   0        0        0     5663 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/operations_binary_bitand.h
+-rw-rw-rw-   0        0        0     5641 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/operations_binary_bitor.h
+-rw-rw-rw-   0        0        0     5663 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/operations_binary_bitxor.h
+-rw-rw-rw-   0        0        0     5422 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/operations_binary_divmod.h
+-rw-rw-rw-   0        0        0     5460 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/operations_binary_floordiv.h
+-rw-rw-rw-   0        0        0     5115 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/operations_binary_lshift.h
+-rw-rw-rw-   0        0        0     2799 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/operations_binary_matmult.h
+-rw-rw-rw-   0        0        0    15778 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/operations_binary_mod.h
+-rw-rw-rw-   0        0        0    13210 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/operations_binary_mult.h
+-rw-rw-rw-   0        0        0     5791 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/operations_binary_olddiv.h
+-rw-rw-rw-   0        0        0     4714 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/operations_binary_pow.h
+-rw-rw-rw-   0        0        0     5115 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/operations_binary_rshift.h
+-rw-rw-rw-   0        0        0     5824 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/operations_binary_sub.h
+-rw-rw-rw-   0        0        0     5438 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/operations_binary_truediv.h
+-rw-rw-rw-   0        0        0    15100 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/operations_builtin_types.h
+-rw-rw-rw-   0        0        0     8670 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/operations_inplace_add.h
+-rw-rw-rw-   0        0        0     3767 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/operations_inplace_bitand.h
+-rw-rw-rw-   0        0        0     3753 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/operations_inplace_bitor.h
+-rw-rw-rw-   0        0        0     3767 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/operations_inplace_bitxor.h
+-rw-rw-rw-   0        0        0     4846 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/operations_inplace_floordiv.h
+-rw-rw-rw-   0        0        0     3011 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/operations_inplace_lshift.h
+-rw-rw-rw-   0        0        0     2727 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/operations_inplace_matmult.h
+-rw-rw-rw-   0        0        0    10626 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/operations_inplace_mod.h
+-rw-rw-rw-   0        0        0     9201 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/operations_inplace_mult.h
+-rw-rw-rw-   0        0        0     5147 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/operations_inplace_olddiv.h
+-rw-rw-rw-   0        0        0     4349 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/operations_inplace_pow.h
+-rw-rw-rw-   0        0        0     3011 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/operations_inplace_rshift.h
+-rw-rw-rw-   0        0        0     4975 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/operations_inplace_sub.h
+-rw-rw-rw-   0        0        0     4826 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/operations_inplace_truediv.h
+-rw-rw-rw-   0        0        0     3297 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/raising.h
+-rw-rw-rw-   0        0        0     2178 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/rangeobjects.h
+-rw-rw-rw-   0        0        0     1146 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/richcomparisons.h
+-rw-rw-rw-   0        0        0     1112 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/sequences.h
+-rw-rw-rw-   0        0        0     1025 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/sets.h
+-rw-rw-rw-   0        0        0     8419 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/slices.h
+-rw-rw-rw-   0        0        0     1242 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/strings.h
+-rw-rw-rw-   0        0        0    17575 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/subscripts.h
+-rw-rw-rw-   0        0        0     5720 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/tuples.h
+-rw-rw-rw-   0        0        0    14521 2023-07-25 02:10:30.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helpers.h
+-rw-rw-rw-   0        0        0     5375 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/importing.h
+-rw-rw-rw-   0        0        0    12979 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/incbin.h
+-rw-rw-rw-   0        0        0    14853 2023-07-25 02:10:30.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/prelude.h
+-rw-rw-rw-   0        0        0     2870 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/printing.h
+-rw-rw-rw-   0        0        0     1761 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/python_pgo.h
+-rw-rw-rw-   0        0        0     2243 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/safe_string_ops.h
+-rw-rw-rw-   0        0        0     3840 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/threading.h
+-rw-rw-rw-   0        0        0     3144 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/tracing.h
+-rw-rw-rw-   0        0        0     2936 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/unfreezing.h
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:09.749027 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:10.029480 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/appdirs/
+-rw-rw-rw-   0        0        0     1097 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/appdirs/LICENSE.txt
+-rw-rw-rw-   0        0        0    24824 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/appdirs/appdirs.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:10.032425 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/atomicwrites/
+-rw-rw-rw-   0        0        0     1069 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/atomicwrites/LICENSE
+-rw-rw-rw-   0        0        0     6794 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/atomicwrites/atomicwrites.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:10.034363 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/bin/
+-rw-rw-rw-   0        0        0     1331 2023-04-13 07:04:12.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/bin/scons.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:09.672987 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/clcache/
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:10.037293 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/clcache/clcache/
+-rw-rw-rw-   0        0        0     1585 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/clcache/clcache/LICENSE
+-rw-rw-rw-   0        0        0       93 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/clcache/clcache/__init__.py
+-rw-rw-rw-   0        0        0    65424 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/clcache/clcache/caching.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:10.038269 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/colorama/
+-rw-rw-rw-   0        0        0     1491 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/colorama/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:10.044127 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/colorama/colorama/
+-rw-rw-rw-   0        0        0      243 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/colorama/colorama/__init__.py
+-rw-rw-rw-   0        0        0     2522 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/colorama/colorama/ansi.py
+-rw-rw-rw-   0        0        0    10517 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/colorama/colorama/ansitowin32.py
+-rw-rw-rw-   0        0        0     1915 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/colorama/colorama/initialise.py
+-rw-rw-rw-   0        0        0     5404 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/colorama/colorama/win32.py
+-rw-rw-rw-   0        0        0     6438 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/colorama/colorama/winterm.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:10.045104 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/glob2/
+-rw-rw-rw-   0        0        0     1359 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/glob2/LICENSE
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:10.051489 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/glob2/glob2/
+-rw-rw-rw-   0        0        0       82 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/glob2/glob2/__init__.py
+-rw-rw-rw-   0        0        0     6859 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/glob2/glob2/compat.py
+-rw-rw-rw-   0        0        0     4463 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/glob2/glob2/fnmatch.py
+-rw-rw-rw-   0        0        0     8304 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/glob2/glob2/impl.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:10.053442 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2/
+-rw-rw-rw-   0        0        0     1467 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2/LICENSE.rst
+-rw-rw-rw-   0        0        0       85 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:10.081807 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2/jinja2/
+-rw-rw-rw-   0        0        0     2423 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2/jinja2/__init__.py
+-rw-rw-rw-   0        0        0     2685 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2/jinja2/_compat.py
+-rw-rw-rw-   0        0        0     1726 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2/jinja2/_identifier.py
+-rw-rw-rw-   0        0        0    12719 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2/jinja2/bccache.py
+-rw-rw-rw-   0        0        0    65386 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2/jinja2/compiler.py
+-rw-rw-rw-   0        0        0     1626 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2/jinja2/constants.py
+-rw-rw-rw-   0        0        0    12281 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2/jinja2/debug.py
+-rw-rw-rw-   0        0        0     1400 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2/jinja2/defaults.py
+-rw-rw-rw-   0        0        0    50849 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2/jinja2/environment.py
+-rw-rw-rw-   0        0        0     4428 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2/jinja2/exceptions.py
+-rw-rw-rw-   0        0        0    24500 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2/jinja2/ext.py
+-rw-rw-rw-   0        0        0    36528 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2/jinja2/filters.py
+-rw-rw-rw-   0        0        0     9197 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2/jinja2/idtracking.py
+-rw-rw-rw-   0        0        0    28559 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2/jinja2/lexer.py
+-rw-rw-rw-   0        0        0    17473 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2/jinja2/loaders.py
+-rw-rw-rw-   0        0        0     4340 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2/jinja2/meta.py
+-rw-rw-rw-   0        0        0     7308 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2/jinja2/nativetypes.py
+-rw-rw-rw-   0        0        0    30853 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2/jinja2/nodes.py
+-rw-rw-rw-   0        0        0     1722 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2/jinja2/optimizer.py
+-rw-rw-rw-   0        0        0    35875 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2/jinja2/parser.py
+-rw-rw-rw-   0        0        0    27644 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2/jinja2/runtime.py
+-rw-rw-rw-   0        0        0    17080 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2/jinja2/sandbox.py
+-rw-rw-rw-   0        0        0     4214 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2/jinja2/tests.py
+-rw-rw-rw-   0        0        0    20501 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2/jinja2/utils.py
+-rw-rw-rw-   0        0        0     3316 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2/jinja2/visitor.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:10.084734 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2_35/
+-rw-rw-rw-   0        0        0     1466 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2_35/LICENSE.rst
+-rw-rw-rw-   0        0        0       84 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2_35/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:10.119888 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2_35/jinja2/
+-rw-rw-rw-   0        0        0     2616 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2_35/jinja2/__init__.py
+-rw-rw-rw-   0        0        0     2685 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2_35/jinja2/_compat.py
+-rw-rw-rw-   0        0        0     1726 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2_35/jinja2/_identifier.py
+-rw-rw-rw-   0        0        0    12719 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2_35/jinja2/bccache.py
+-rw-rw-rw-   0        0        0    65386 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2_35/jinja2/compiler.py
+-rw-rw-rw-   0        0        0     1626 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2_35/jinja2/constants.py
+-rw-rw-rw-   0        0        0    12281 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2_35/jinja2/debug.py
+-rw-rw-rw-   0        0        0     1400 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2_35/jinja2/defaults.py
+-rw-rw-rw-   0        0        0    50849 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2_35/jinja2/environment.py
+-rw-rw-rw-   0        0        0     4428 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2_35/jinja2/exceptions.py
+-rw-rw-rw-   0        0        0    24500 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2_35/jinja2/ext.py
+-rw-rw-rw-   0        0        0    36528 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2_35/jinja2/filters.py
+-rw-rw-rw-   0        0        0     9197 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2_35/jinja2/idtracking.py
+-rw-rw-rw-   0        0        0    28559 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2_35/jinja2/lexer.py
+-rw-rw-rw-   0        0        0    17474 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2_35/jinja2/loaders.py
+-rw-rw-rw-   0        0        0     4340 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2_35/jinja2/meta.py
+-rw-rw-rw-   0        0        0     7308 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2_35/jinja2/nativetypes.py
+-rw-rw-rw-   0        0        0    30853 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2_35/jinja2/nodes.py
+-rw-rw-rw-   0        0        0     1722 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2_35/jinja2/optimizer.py
+-rw-rw-rw-   0        0        0    35875 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2_35/jinja2/parser.py
+-rw-rw-rw-   0        0        0    27644 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2_35/jinja2/runtime.py
+-rw-rw-rw-   0        0        0    17080 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2_35/jinja2/sandbox.py
+-rw-rw-rw-   0        0        0     4214 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2_35/jinja2/tests.py
+-rw-rw-rw-   0        0        0    20501 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2_35/jinja2/utils.py
+-rw-rw-rw-   0        0        0     3316 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2_35/jinja2/visitor.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:09.691106 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:09.677871 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:10.148268 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/
+-rw-rw-rw-   0        0        0    47844 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Action.py
+-rw-rw-rw-   0        0        0    33996 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Builder.py
+-rw-rw-rw-   0        0        0     8083 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/CacheDir.py
+-rw-rw-rw-   0        0        0    27693 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Conftest.py
+-rw-rw-rw-   0        0        0     6938 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Debug.py
+-rw-rw-rw-   0        0        0    17622 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Defaults.py
+-rw-rw-rw-   0        0        0    96183 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Environment.py
+-rw-rw-rw-   0        0        0     7358 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Errors.py
+-rw-rw-rw-   0        0        0    21540 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Executor.py
+-rw-rw-rw-   0        0        0    16000 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Job.py
+-rw-rw-rw-   0        0        0     9589 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Memoize.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:10.154124 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/
+-rw-rw-rw-   0        0        0     4197 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Alias.py
+-rw-rw-rw-   0        0        0   121420 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/FS.py
+-rw-rw-rw-   0        0        0     4164 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Python.py
+-rw-rw-rw-   0        0        0    49503 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:10.159010 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/
+-rw-rw-rw-   0        0        0     1950 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/BoolOption.py
+-rw-rw-rw-   0        0        0     1950 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/EnumOption.py
+-rw-rw-rw-   0        0        0     1950 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/ListOption.py
+-rw-rw-rw-   0        0        0     1965 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PackageOption.py
+-rw-rw-rw-   0        0        0     2736 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PathOption.py
+-rw-rw-rw-   0        0        0     2614 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/__init__.py
+-rw-rw-rw-   0        0        0     8467 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/PathList.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:10.173654 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/
+-rw-rw-rw-   0        0        0     9314 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/__init__.py
+-rw-rw-rw-   0        0        0     3131 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/aix.py
+-rw-rw-rw-   0        0        0     1989 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/cygwin.py
+-rw-rw-rw-   0        0        0     2483 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/darwin.py
+-rw-rw-rw-   0        0        0     1718 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/hpux.py
+-rw-rw-rw-   0        0        0     1605 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/irix.py
+-rw-rw-rw-   0        0        0     2170 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/os2.py
+-rw-rw-rw-   0        0        0     4179 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/posix.py
+-rw-rw-rw-   0        0        0     1882 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/sunos.py
+-rw-rw-rw-   0        0        0    14948 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/win32.py
+-rw-rw-rw-   0        0        0    39700 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConf.py
+-rw-rw-rw-   0        0        0    12950 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConsign.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:10.179515 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/
+-rw-rw-rw-   0        0        0     4810 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/C.py
+-rw-rw-rw-   0        0        0     3751 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Dir.py
+-rw-rw-rw-   0        0        0     3233 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Prog.py
+-rw-rw-rw-   0        0        0     2011 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/RC.py
+-rw-rw-rw-   0        0        0    14663 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:10.186348 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/
+-rw-rw-rw-   0        0        0    14029 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Interactive.py
+-rw-rw-rw-   0        0        0    52665 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Main.py
+-rw-rw-rw-   0        0        0    40719 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConsOptions.py
+-rw-rw-rw-   0        0        0    24133 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConscript.py
+-rw-rw-rw-   0        0        0    14053 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/__init__.py
+-rw-rw-rw-   0        0        0     2305 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Sig.py
+-rw-rw-rw-   0        0        0    34903 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Subst.py
+-rw-rw-rw-   0        0        0    40510 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Taskmaster.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:10.284524 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/
+-rw-rw-rw-   0        0        0     2166 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/386asm.py
+-rw-rw-rw-   0        0        0     2433 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/BitKeeper.py
+-rw-rw-rw-   0        0        0     2859 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/CVS.py
+-rw-rw-rw-   0        0        0    18084 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/GettextCommon.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:10.292336 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/
+-rw-rw-rw-   0        0        0     2078 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/__init__.py
+-rw-rw-rw-   0        0        0     2004 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/arch.py
+-rw-rw-rw-   0        0        0     9248 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/common.py
+-rw-rw-rw-   0        0        0     2784 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/netframework.py
+-rw-rw-rw-   0        0        0    14869 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/sdk.py
+-rw-rw-rw-   0        0        0    19499 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vc.py
+-rw-rw-rw-   0        0        0    20832 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vs.py
+-rw-rw-rw-   0        0        0     3763 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Perforce.py
+-rw-rw-rw-   0        0        0     5149 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/PharLapCommon.py
+-rw-rw-rw-   0        0        0     2290 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/RCS.py
+-rw-rw-rw-   0        0        0     2328 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/SCCS.py
+-rw-rw-rw-   0        0        0     2657 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Subversion.py
+-rw-rw-rw-   0        0        0    31283 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/__init__.py
+-rw-rw-rw-   0        0        0     2379 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixc++.py
+-rw-rw-rw-   0        0        0     2267 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixcc.py
+-rw-rw-rw-   0        0        0     2681 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixf77.py
+-rw-rw-rw-   0        0        0     2720 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixlink.py
+-rw-rw-rw-   0        0        0     2796 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/applelink.py
+-rw-rw-rw-   0        0        0     2147 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ar.py
+-rw-rw-rw-   0        0        0     2936 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/as.py
+-rw-rw-rw-   0        0        0     2935 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/bcc32.py
+-rw-rw-rw-   0        0        0     3432 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/c++.py
+-rw-rw-rw-   0        0        0     3785 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cc.py
+-rw-rw-rw-   0        0        0     2777 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cyglink.py
+-rw-rw-rw-   0        0        0     1711 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/default.py
+-rw-rw-rw-   0        0        0      142 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/dmd.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:10.292904 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/docbook/
+-rw-rw-rw-   0        0        0    29618 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/docbook/__init__.py
+-rw-rw-rw-   0        0        0     3428 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/filesystem.py
+-rw-rw-rw-   0        0        0     2681 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g++.py
+-rw-rw-rw-   0        0        0     2433 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g77.py
+-rw-rw-rw-   0        0        0     1844 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gas.py
+-rw-rw-rw-   0        0        0     3472 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gcc.py
+-rw-rw-rw-   0        0        0     4782 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gdc.py
+-rw-rw-rw-   0        0        0     2025 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gettext.py
+-rw-rw-rw-   0        0        0     2256 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gfortran.py
+-rw-rw-rw-   0        0        0     2460 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gnulink.py
+-rw-rw-rw-   0        0        0     2639 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpc++.py
+-rw-rw-rw-   0        0        0     1810 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpcc.py
+-rw-rw-rw-   0        0        0     2333 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hplink.py
+-rw-rw-rw-   0        0        0     2140 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icc.py
+-rw-rw-rw-   0        0        0     1902 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icl.py
+-rw-rw-rw-   0        0        0     2077 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink.py
+-rw-rw-rw-   0        0        0     2043 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink32.py
+-rw-rw-rw-   0        0        0    18600 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/install.py
+-rw-rw-rw-   0        0        0    25816 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/intelc.py
+-rw-rw-rw-   0        0        0     3328 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/lex.py
+-rw-rw-rw-   0        0        0     8394 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/link.py
+-rw-rw-rw-   0        0        0     3953 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/linkloc.py
+-rw-rw-rw-   0        0        0     2309 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/m4.py
+-rw-rw-rw-   0        0        0     2945 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/masm.py
+-rw-rw-rw-   0        0        0     6919 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mingw.py
+-rw-rw-rw-   0        0        0     4381 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgfmt.py
+-rw-rw-rw-   0        0        0     4658 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msginit.py
+-rw-rw-rw-   0        0        0     4224 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgmerge.py
+-rw-rw-rw-   0        0        0     2168 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslib.py
+-rw-rw-rw-   0        0        0    13881 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslink.py
+-rw-rw-rw-   0        0        0     1804 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mssdk.py
+-rw-rw-rw-   0        0        0    11380 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvc.py
+-rw-rw-rw-   0        0        0    72761 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvs.py
+-rw-rw-rw-   0        0        0     6841 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwcc.py
+-rw-rw-rw-   0        0        0     3579 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwld.py
+-rw-rw-rw-   0        0        0     2618 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/nasm.py
+-rw-rw-rw-   0        0        0     4375 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rmic.py
+-rw-rw-rw-   0        0        0     2827 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rpcgen.py
+-rw-rw-rw-   0        0        0     2513 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgiar.py
+-rw-rw-rw-   0        0        0     1991 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgic++.py
+-rw-rw-rw-   0        0        0     1819 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgicc.py
+-rw-rw-rw-   0        0        0     2123 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgilink.py
+-rw-rw-rw-   0        0        0     2502 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunar.py
+-rw-rw-rw-   0        0        0     4695 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunc++.py
+-rw-rw-rw-   0        0        0     1927 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/suncc.py
+-rw-rw-rw-   0        0        0     2349 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunlink.py
+-rw-rw-rw-   0        0        0     2473 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tar.py
+-rw-rw-rw-   0        0        0     5992 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/textfile.py
+-rw-rw-rw-   0        0        0     1831 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tlib.py
+-rw-rw-rw-   0        0        0     3730 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/wix.py
+-rw-rw-rw-   0        0        0    13016 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/xgettext.py
+-rw-rw-rw-   0        0        0     3415 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/zip.py
+-rw-rw-rw-   0        0        0    48938 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Util.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:10.302613 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/
+-rw-rw-rw-   0        0        0     3007 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/BoolVariable.py
+-rw-rw-rw-   0        0        0     3784 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/EnumVariable.py
+-rw-rw-rw-   0        0        0     4404 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/ListVariable.py
+-rw-rw-rw-   0        0        0     3557 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PackageVariable.py
+-rw-rw-rw-   0        0        0     5612 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PathVariable.py
+-rw-rw-rw-   0        0        0    11034 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/__init__.py
+-rw-rw-rw-   0        0        0     6824 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Warnings.py
+-rw-rw-rw-   0        0        0     1563 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:10.312891 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/
+-rw-rw-rw-   0        0        0     8120 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/__init__.py
+-rw-rw-rw-   0        0        0     3596 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_builtins.py
+-rw-rw-rw-   0        0        0     1818 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_collections.py
+-rw-rw-rw-   0        0        0     1742 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_dbm.py
+-rw-rw-rw-   0        0        0     2465 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_hashlib.py
+-rw-rw-rw-   0        0        0     1776 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_io.py
+-rw-rw-rw-   0        0        0    19253 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_sets.py
+-rw-rw-rw-   0        0        0    44500 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_subprocess.py
+-rw-rw-rw-   0        0        0    19664 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/cpp.py
+-rw-rw-rw-   0        0        0     7509 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/dblite.py
+-rw-rw-rw-   0        0        0     2107 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/exitfuncs.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:09.684276 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:10.344200 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/
+-rw-rw-rw-   0        0        0    53545 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Action.py
+-rw-rw-rw-   0        0        0    34985 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Builder.py
+-rw-rw-rw-   0        0        0    13596 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/CacheDir.py
+-rw-rw-rw-   0        0        0    28403 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Conftest.py
+-rw-rw-rw-   0        0        0     7533 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Debug.py
+-rw-rw-rw-   0        0        0    20988 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Defaults.py
+-rw-rw-rw-   0        0        0    96818 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Environment.py
+-rw-rw-rw-   0        0        0     7752 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Errors.py
+-rw-rw-rw-   0        0        0    22350 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Executor.py
+-rw-rw-rw-   0        0        0    16068 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Job.py
+-rw-rw-rw-   0        0        0     9565 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Memoize.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:10.351035 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/
+-rw-rw-rw-   0        0        0     5239 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Alias.py
+-rw-rw-rw-   0        0        0   135413 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/FS.py
+-rw-rw-rw-   0        0        0     5758 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Python.py
+-rw-rw-rw-   0        0        0    63474 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/__init__.py
+-rw-rw-rw-   0        0        0     8354 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/PathList.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:10.369588 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/
+-rw-rw-rw-   0        0        0    11500 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/__init__.py
+-rw-rw-rw-   0        0        0     3180 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/aix.py
+-rw-rw-rw-   0        0        0     2227 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/cygwin.py
+-rw-rw-rw-   0        0        0     2739 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/darwin.py
+-rw-rw-rw-   0        0        0     1767 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/hpux.py
+-rw-rw-rw-   0        0        0     1654 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/irix.py
+-rw-rw-rw-   0        0        0     1460 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/mingw.py
+-rw-rw-rw-   0        0        0     2219 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/os2.py
+-rw-rw-rw-   0        0        0     4476 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/posix.py
+-rw-rw-rw-   0        0        0     1931 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/sunos.py
+-rw-rw-rw-   0        0        0     4003 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/virtualenv.py
+-rw-rw-rw-   0        0        0    16962 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/win32.py
+-rw-rw-rw-   0        0        0    41186 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConf.py
+-rw-rw-rw-   0        0        0    13880 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConsign.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:10.376423 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/
+-rw-rw-rw-   0        0        0     4853 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/C.py
+-rw-rw-rw-   0        0        0     3812 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Dir.py
+-rw-rw-rw-   0        0        0     3643 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Prog.py
+-rw-rw-rw-   0        0        0     2328 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/RC.py
+-rw-rw-rw-   0        0        0    15053 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:10.384269 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/
+-rw-rw-rw-   0        0        0    13779 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Interactive.py
+-rw-rw-rw-   0        0        0    53260 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Main.py
+-rw-rw-rw-   0        0        0    39394 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConsOptions.py
+-rw-rw-rw-   0        0        0    26467 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConscript.py
+-rw-rw-rw-   0        0        0    14489 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/__init__.py
+-rw-rw-rw-   0        0        0    35863 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Subst.py
+-rw-rw-rw-   0        0        0    42204 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Taskmaster.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:10.515674 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/
+-rw-rw-rw-   0        0        0     2211 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/386asm.py
+-rw-rw-rw-   0        0        0    18207 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/GettextCommon.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:10.525439 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/
+-rw-rw-rw-   0        0        0     2152 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/__init__.py
+-rw-rw-rw-   0        0        0     2057 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/arch.py
+-rw-rw-rw-   0        0        0    10674 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/common.py
+-rw-rw-rw-   0        0        0     2855 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/netframework.py
+-rw-rw-rw-   0        0        0    15165 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/sdk.py
+-rw-rw-rw-   0        0        0    33537 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vc.py
+-rw-rw-rw-   0        0        0    21762 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vs.py
+-rw-rw-rw-   0        0        0     4464 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/PharLapCommon.py
+-rw-rw-rw-   0        0        0    50660 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/__init__.py
+-rw-rw-rw-   0        0        0     1667 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixc++.py
+-rw-rw-rw-   0        0        0     2316 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcc.py
+-rw-rw-rw-   0        0        0     2475 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcxx.py
+-rw-rw-rw-   0        0        0     2840 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixlink.py
+-rw-rw-rw-   0        0        0     8618 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/applelink.py
+-rw-rw-rw-   0        0        0     2226 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ar.py
+-rw-rw-rw-   0        0        0     2978 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/as.py
+-rw-rw-rw-   0        0        0     2977 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/bcc32.py
+-rw-rw-rw-   0        0        0     1653 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/c++.py
+-rw-rw-rw-   0        0        0     3827 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cc.py
+-rw-rw-rw-   0        0        0     3389 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clang.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:10.526415 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangCommon/
+-rw-rw-rw-   0        0        0      313 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangCommon/__init__.py
+-rw-rw-rw-   0        0        0     3631 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangxx.py
+-rw-rw-rw-   0        0        0     3444 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cxx.py
+-rw-rw-rw-   0        0        0     8494 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cyglink.py
+-rw-rw-rw-   0        0        0     1753 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/default.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:10.527392 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/docbook/
+-rw-rw-rw-   0        0        0    29765 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/docbook/__init__.py
+-rw-rw-rw-   0        0        0     3472 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/filesystem.py
+-rw-rw-rw-   0        0        0     1630 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/g++.py
+-rw-rw-rw-   0        0        0     1977 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gas.py
+-rw-rw-rw-   0        0        0     3686 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gcc.py
+-rw-rw-rw-   0        0        0     2580 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gettext_tool.py
+-rw-rw-rw-   0        0        0     2948 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gnulink.py
+-rw-rw-rw-   0        0        0     2655 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gxx.py
+-rw-rw-rw-   0        0        0     1645 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpc++.py
+-rw-rw-rw-   0        0        0     1859 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcc.py
+-rw-rw-rw-   0        0        0     2765 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcxx.py
+-rw-rw-rw-   0        0        0     2386 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hplink.py
+-rw-rw-rw-   0        0        0     2189 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icc.py
+-rw-rw-rw-   0        0        0     1944 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icl.py
+-rw-rw-rw-   0        0        0     2123 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink.py
+-rw-rw-rw-   0        0        0     2085 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink32.py
+-rw-rw-rw-   0        0        0    15791 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/install.py
+-rw-rw-rw-   0        0        0    26195 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/intelc.py
+-rw-rw-rw-   0        0        0    13924 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/link.py
+-rw-rw-rw-   0        0        0     4041 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/linkloc.py
+-rw-rw-rw-   0        0        0     2351 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/m4.py
+-rw-rw-rw-   0        0        0     2987 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/masm.py
+-rw-rw-rw-   0        0        0     7808 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mingw.py
+-rw-rw-rw-   0        0        0     4956 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgfmt.py
+-rw-rw-rw-   0        0        0     5235 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msginit.py
+-rw-rw-rw-   0        0        0     4808 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgmerge.py
+-rw-rw-rw-   0        0        0     2475 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslib.py
+-rw-rw-rw-   0        0        0    14751 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslink.py
+-rw-rw-rw-   0        0        0     1847 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mssdk.py
+-rw-rw-rw-   0        0        0    12588 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvc.py
+-rw-rw-rw-   0        0        0    82939 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvs.py
+-rw-rw-rw-   0        0        0     6883 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwcc.py
+-rw-rw-rw-   0        0        0     3663 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwld.py
+-rw-rw-rw-   0        0        0     2660 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/nasm.py
+-rw-rw-rw-   0        0        0     4904 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rmic.py
+-rw-rw-rw-   0        0        0     2877 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rpcgen.py
+-rw-rw-rw-   0        0        0     2567 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgiar.py
+-rw-rw-rw-   0        0        0     1652 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgic++.py
+-rw-rw-rw-   0        0        0     1868 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicc.py
+-rw-rw-rw-   0        0        0     2088 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicxx.py
+-rw-rw-rw-   0        0        0     2176 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgilink.py
+-rw-rw-rw-   0        0        0     2366 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunar.py
+-rw-rw-rw-   0        0        0     1658 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunc++.py
+-rw-rw-rw-   0        0        0     1976 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncc.py
+-rw-rw-rw-   0        0        0     5335 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncxx.py
+-rw-rw-rw-   0        0        0     2583 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunlink.py
+-rw-rw-rw-   0        0        0     2515 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tar.py
+-rw-rw-rw-   0        0        0     6756 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/textfile.py
+-rw-rw-rw-   0        0        0     1873 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tlib.py
+-rw-rw-rw-   0        0        0     3773 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/wix.py
+-rw-rw-rw-   0        0        0    13982 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/xgettext.py
+-rw-rw-rw-   0        0        0     3201 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/zip.py
+-rw-rw-rw-   0        0        0    53803 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Util.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:10.538134 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/
+-rw-rw-rw-   0        0        0     3064 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/BoolVariable.py
+-rw-rw-rw-   0        0        0     3818 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/EnumVariable.py
+-rw-rw-rw-   0        0        0     4459 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/ListVariable.py
+-rw-rw-rw-   0        0        0     3643 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PackageVariable.py
+-rw-rw-rw-   0        0        0     5579 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PathVariable.py
+-rw-rw-rw-   0        0        0    11655 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/__init__.py
+-rw-rw-rw-   0        0        0     6504 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Warnings.py
+-rw-rw-rw-   0        0        0     1647 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:10.541063 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/
+-rw-rw-rw-   0        0        0     6869 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/__init__.py
+-rw-rw-rw-   0        0        0     1784 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/_scons_dbm.py
+-rw-rw-rw-   0        0        0    19816 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/cpp.py
+-rw-rw-rw-   0        0        0     9002 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/dblite.py
+-rw-rw-rw-   0        0        0     2149 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/exitfuncs.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:09.692083 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:10.578225 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/
+-rw-rw-rw-   0        0        0    56578 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Action.py
+-rw-rw-rw-   0        0        0    35213 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Builder.py
+-rw-rw-rw-   0        0        0    11061 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/CacheDir.py
+-rw-rw-rw-   0        0        0    27408 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Conftest.py
+-rw-rw-rw-   0        0        0     7884 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Debug.py
+-rw-rw-rw-   0        0        0    21423 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Defaults.py
+-rw-rw-rw-   0        0        0    97269 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Environment.py
+-rw-rw-rw-   0        0        0     3979 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/EnvironmentValues.py
+-rw-rw-rw-   0        0        0     7515 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Errors.py
+-rw-rw-rw-   0        0        0    21937 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Executor.py
+-rw-rw-rw-   0        0        0    16583 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Job.py
+-rw-rw-rw-   0        0        0     9430 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Memoize.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:10.585067 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/
+-rw-rw-rw-   0        0        0     5126 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Alias.py
+-rw-rw-rw-   0        0        0   136271 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/FS.py
+-rw-rw-rw-   0        0        0     6167 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Python.py
+-rw-rw-rw-   0        0        0    63768 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/__init__.py
+-rw-rw-rw-   0        0        0     8183 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/PathList.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:10.600692 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/
+-rw-rw-rw-   0        0        0    12836 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/__init__.py
+-rw-rw-rw-   0        0        0     3087 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/aix.py
+-rw-rw-rw-   0        0        0     2107 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/cygwin.py
+-rw-rw-rw-   0        0        0     2630 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/darwin.py
+-rw-rw-rw-   0        0        0     1674 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/hpux.py
+-rw-rw-rw-   0        0        0     1536 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/irix.py
+-rw-rw-rw-   0        0        0     1311 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/mingw.py
+-rw-rw-rw-   0        0        0     2076 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/os2.py
+-rw-rw-rw-   0        0        0     4356 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/posix.py
+-rw-rw-rw-   0        0        0     1805 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/sunos.py
+-rw-rw-rw-   0        0        0     3860 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/virtualenv.py
+-rw-rw-rw-   0        0        0    14831 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/win32.py
+-rw-rw-rw-   0        0        0    41983 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConf.py
+-rw-rw-rw-   0        0        0    14673 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConsign.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:10.606544 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/
+-rw-rw-rw-   0        0        0     7394 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/C.py
+-rw-rw-rw-   0        0        0     4357 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Dir.py
+-rw-rw-rw-   0        0        0     3546 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Prog.py
+-rw-rw-rw-   0        0        0     1972 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/RC.py
+-rw-rw-rw-   0        0        0    15577 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:10.611426 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/
+-rw-rw-rw-   0        0        0    13597 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Interactive.py
+-rw-rw-rw-   0        0        0    53509 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Main.py
+-rw-rw-rw-   0        0        0    42760 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConsOptions.py
+-rw-rw-rw-   0        0        0    26676 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConscript.py
+-rw-rw-rw-   0        0        0    14272 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/__init__.py
+-rw-rw-rw-   0        0        0    36753 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Subst.py
+-rw-rw-rw-   0        0        0    41191 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Taskmaster.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:10.706813 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/
+-rw-rw-rw-   0        0        0     2122 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/386asm.py
+-rw-rw-rw-   0        0        0    15570 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/GettextCommon.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:10.716112 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/
+-rw-rw-rw-   0        0        0     2014 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/__init__.py
+-rw-rw-rw-   0        0        0     1943 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/arch.py
+-rw-rw-rw-   0        0        0    13182 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/common.py
+-rw-rw-rw-   0        0        0     2734 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/netframework.py
+-rw-rw-rw-   0        0        0    15027 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/sdk.py
+-rw-rw-rw-   0        0        0    38783 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vc.py
+-rw-rw-rw-   0        0        0    22570 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vs.py
+-rw-rw-rw-   0        0        0     4368 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/PharLapCommon.py
+-rw-rw-rw-   0        0        0    32724 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/__init__.py
+-rw-rw-rw-   0        0        0     1578 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixc++.py
+-rw-rw-rw-   0        0        0     2228 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcc.py
+-rw-rw-rw-   0        0        0     2386 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcxx.py
+-rw-rw-rw-   0        0        0     2616 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixlink.py
+-rw-rw-rw-   0        0        0     7993 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/applelink.py
+-rw-rw-rw-   0        0        0     2141 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ar.py
+-rw-rw-rw-   0        0        0     1661 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/as.py
+-rw-rw-rw-   0        0        0     2893 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/asm.py
+-rw-rw-rw-   0        0        0     2889 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/bcc32.py
+-rw-rw-rw-   0        0        0     1567 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/c++.py
+-rw-rw-rw-   0        0        0     3742 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cc.py
+-rw-rw-rw-   0        0        0     3296 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clang.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:10.718072 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangCommon/
+-rw-rw-rw-   0        0        0      343 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangCommon/__init__.py
+-rw-rw-rw-   0        0        0     3534 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangxx.py
+-rw-rw-rw-   0        0        0     3259 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cxx.py
+-rw-rw-rw-   0        0        0     7461 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cyglink.py
+-rw-rw-rw-   0        0        0     1663 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/default.py
+-rw-rw-rw-   0        0        0     3379 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/filesystem.py
+-rw-rw-rw-   0        0        0     1544 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/g++.py
+-rw-rw-rw-   0        0        0     1891 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gas.py
+-rw-rw-rw-   0        0        0     3616 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gcc.py
+-rw-rw-rw-   0        0        0     2377 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gettext_tool.py
+-rw-rw-rw-   0        0        0     2437 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gnulink.py
+-rw-rw-rw-   0        0        0     2526 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gxx.py
+-rw-rw-rw-   0        0        0     1557 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpc++.py
+-rw-rw-rw-   0        0        0     1772 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcc.py
+-rw-rw-rw-   0        0        0     2677 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcxx.py
+-rw-rw-rw-   0        0        0     2206 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hplink.py
+-rw-rw-rw-   0        0        0     2096 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icc.py
+-rw-rw-rw-   0        0        0     1851 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icl.py
+-rw-rw-rw-   0        0        0     1954 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink.py
+-rw-rw-rw-   0        0        0     1995 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink32.py
+-rw-rw-rw-   0        0        0    19180 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/install.py
+-rw-rw-rw-   0        0        0    25826 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/intelc.py
+-rw-rw-rw-   0        0        0     2588 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/link.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:10.721973 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/
+-rw-rw-rw-   0        0        0     4649 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/LoadableModule.py
+-rw-rw-rw-   0        0        0     7652 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/SharedLibrary.py
+-rw-rw-rw-   0        0        0     6064 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/__init__.py
+-rw-rw-rw-   0        0        0     3931 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkloc.py
+-rw-rw-rw-   0        0        0     2266 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/m4.py
+-rw-rw-rw-   0        0        0     2900 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/masm.py
+-rw-rw-rw-   0        0        0     8622 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mingw.py
+-rw-rw-rw-   0        0        0     4577 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgfmt.py
+-rw-rw-rw-   0        0        0     4517 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msginit.py
+-rw-rw-rw-   0        0        0     4113 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgmerge.py
+-rw-rw-rw-   0        0        0     2387 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslib.py
+-rw-rw-rw-   0        0        0    14473 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslink.py
+-rw-rw-rw-   0        0        0     1752 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mssdk.py
+-rw-rw-rw-   0        0        0    12902 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvc.py
+-rw-rw-rw-   0        0        0    84784 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvs.py
+-rw-rw-rw-   0        0        0     6788 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwcc.py
+-rw-rw-rw-   0        0        0     3576 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwld.py
+-rw-rw-rw-   0        0        0     2573 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/nasm.py
+-rw-rw-rw-   0        0        0     4817 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rmic.py
+-rw-rw-rw-   0        0        0     2788 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rpcgen.py
+-rw-rw-rw-   0        0        0     2479 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgiar.py
+-rw-rw-rw-   0        0        0     1563 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgic++.py
+-rw-rw-rw-   0        0        0     1780 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicc.py
+-rw-rw-rw-   0        0        0     1999 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicxx.py
+-rw-rw-rw-   0        0        0     2006 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgilink.py
+-rw-rw-rw-   0        0        0     2271 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunar.py
+-rw-rw-rw-   0        0        0     1569 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunc++.py
+-rw-rw-rw-   0        0        0     1888 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncc.py
+-rw-rw-rw-   0        0        0     4879 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncxx.py
+-rw-rw-rw-   0        0        0     2419 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunlink.py
+-rw-rw-rw-   0        0        0     2429 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tar.py
+-rw-rw-rw-   0        0        0     6412 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/textfile.py
+-rw-rw-rw-   0        0        0     1786 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tlib.py
+-rw-rw-rw-   0        0        0     3687 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/wix.py
+-rw-rw-rw-   0        0        0    12548 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/xgettext.py
+-rw-rw-rw-   0        0        0     4076 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/zip.py
+-rw-rw-rw-   0        0        0    71693 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Util.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:10.724902 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/
+-rw-rw-rw-   0        0        0     6632 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/ConfigureCache.py
+-rw-rw-rw-   0        0        0        0 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/__init__.py
+-rw-rw-rw-   0        0        0    15278 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/sconsign.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:10.730760 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/
+-rw-rw-rw-   0        0        0     3134 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/BoolVariable.py
+-rw-rw-rw-   0        0        0     3896 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/EnumVariable.py
+-rw-rw-rw-   0        0        0     4672 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/ListVariable.py
+-rw-rw-rw-   0        0        0     3536 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PackageVariable.py
+-rw-rw-rw-   0        0        0     5588 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PathVariable.py
+-rw-rw-rw-   0        0        0    12708 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/__init__.py
+-rw-rw-rw-   0        0        0     6785 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Warnings.py
+-rw-rw-rw-   0        0        0      353 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:10.736619 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/
+-rw-rw-rw-   0        0        0     4307 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/__init__.py
+-rw-rw-rw-   0        0        0     1644 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/_scons_dbm.py
+-rw-rw-rw-   0        0        0     3395 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/win32.py
+-rw-rw-rw-   0        0        0    21614 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/cpp.py
+-rw-rw-rw-   0        0        0     9295 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/dblite.py
+-rw-rw-rw-   0        0        0     2032 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/exitfuncs.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:10.737598 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/markupsafe/
+-rw-rw-rw-   0        0        0     1467 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/markupsafe/LICENSE.rst
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:10.742049 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/markupsafe/markupsafe/
+-rw-rw-rw-   0        0        0    10126 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/markupsafe/markupsafe/__init__.py
+-rw-rw-rw-   0        0        0      558 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/markupsafe/markupsafe/_compat.py
+-rw-rw-rw-   0        0        0     4690 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/markupsafe/markupsafe/_constants.py
+-rw-rw-rw-   0        0        0     1873 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/markupsafe/markupsafe/_native.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:09.744148 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/pkg_resources/
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:10.744969 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/pkg_resources/pkg_resources/
+-rw-rw-rw-   0        0        0   107452 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/pkg_resources/pkg_resources/__init__.py
+-rw-rw-rw-   0        0        0      538 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/pkg_resources/pkg_resources/py31compat.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:09.745131 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/tqdm/
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:10.766454 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/tqdm/tqdm/
+-rw-rw-rw-   0        0        0     1591 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/tqdm/tqdm/__init__.py
+-rw-rw-rw-   0        0        0      283 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/tqdm/tqdm/_main.py
+-rw-rw-rw-   0        0        0     3687 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/tqdm/tqdm/_monitor.py
+-rw-rw-rw-   0        0        0      283 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/tqdm/tqdm/_tqdm.py
+-rw-rw-rw-   0        0        0      287 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/tqdm/tqdm/_tqdm_gui.py
+-rw-rw-rw-   0        0        0      307 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/tqdm/tqdm/_tqdm_notebook.py
+-rw-rw-rw-   0        0        0      888 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/tqdm/tqdm/_tqdm_pandas.py
+-rw-rw-rw-   0        0        0      596 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/tqdm/tqdm/_utils.py
+-rw-rw-rw-   0        0        0     1106 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/tqdm/tqdm/auto.py
+-rw-rw-rw-   0        0        0      857 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/tqdm/tqdm/autonotebook.py
+-rw-rw-rw-   0        0        0     1376 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/tqdm/tqdm/dask.py
+-rw-rw-rw-   0        0        0     5943 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/tqdm/tqdm/gui.py
+-rw-rw-rw-   0        0        0    10790 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/tqdm/tqdm/notebook.py
+-rw-rw-rw-   0        0        0    57572 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/tqdm/tqdm/std.py
+-rw-rw-rw-   0        0        0     6948 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/tqdm/tqdm/tk.py
+-rw-rw-rw-   0        0        0     9533 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/tqdm/tqdm/utils.py
+-rw-rw-rw-   0        0        0      333 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/tqdm/tqdm/version.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:10.768408 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml/
+-rw-rw-rw-   0        0        0     1101 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml/LICENSE
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:10.789892 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml/yaml/
+-rw-rw-rw-   0        0        0    13170 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml/yaml/__init__.py
+-rw-rw-rw-   0        0        0     4883 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml/yaml/composer.py
+-rw-rw-rw-   0        0        0    28639 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml/yaml/constructor.py
+-rw-rw-rw-   0        0        0     3851 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml/yaml/cyaml.py
+-rw-rw-rw-   0        0        0     2837 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml/yaml/dumper.py
+-rw-rw-rw-   0        0        0    43006 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml/yaml/emitter.py
+-rw-rw-rw-   0        0        0     2533 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml/yaml/error.py
+-rw-rw-rw-   0        0        0     2445 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml/yaml/events.py
+-rw-rw-rw-   0        0        0     2061 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml/yaml/loader.py
+-rw-rw-rw-   0        0        0     1440 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml/yaml/nodes.py
+-rw-rw-rw-   0        0        0    25495 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml/yaml/parser.py
+-rw-rw-rw-   0        0        0     6794 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml/yaml/reader.py
+-rw-rw-rw-   0        0        0    14184 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml/yaml/representer.py
+-rw-rw-rw-   0        0        0     8999 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml/yaml/resolver.py
+-rw-rw-rw-   0        0        0    51277 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml/yaml/scanner.py
+-rw-rw-rw-   0        0        0     4165 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml/yaml/serializer.py
+-rw-rw-rw-   0        0        0     2573 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml/yaml/tokens.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:10.790866 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml_27/
+-rw-rw-rw-   0        0        0     1101 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml_27/LICENSE
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:10.811891 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml_27/yaml/
+-rw-rw-rw-   0        0        0     9776 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml_27/yaml/__init__.py
+-rw-rw-rw-   0        0        0     4921 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml_27/yaml/composer.py
+-rw-rw-rw-   0        0        0    25145 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml_27/yaml/constructor.py
+-rw-rw-rw-   0        0        0     3290 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml_27/yaml/cyaml.py
+-rw-rw-rw-   0        0        0     2719 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml_27/yaml/dumper.py
+-rw-rw-rw-   0        0        0    43298 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml_27/yaml/emitter.py
+-rw-rw-rw-   0        0        0     2559 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml_27/yaml/error.py
+-rw-rw-rw-   0        0        0     2445 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml_27/yaml/events.py
+-rw-rw-rw-   0        0        0     1132 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml_27/yaml/loader.py
+-rw-rw-rw-   0        0        0     1440 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml_27/yaml/nodes.py
+-rw-rw-rw-   0        0        0    25542 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml_27/yaml/parser.py
+-rw-rw-rw-   0        0        0     6746 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml_27/yaml/reader.py
+-rw-rw-rw-   0        0        0    17711 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml_27/yaml/representer.py
+-rw-rw-rw-   0        0        0     9122 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml_27/yaml/resolver.py
+-rw-rw-rw-   0        0        0    52446 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml_27/yaml/scanner.py
+-rw-rw-rw-   0        0        0     4171 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml_27/yaml/serializer.py
+-rw-rw-rw-   0        0        0     2573 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml_27/yaml/tokens.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:10.813726 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml_35/
+-rw-rw-rw-   0        0        0     1101 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml_35/LICENSE
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:10.858305 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml_35/yaml/
+-rw-rw-rw-   0        0        0     9607 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml_35/yaml/__init__.py
+-rw-rw-rw-   0        0        0     4881 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml_35/yaml/composer.py
+-rw-rw-rw-   0        0        0    25554 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml_35/yaml/constructor.py
+-rw-rw-rw-   0        0        0     3294 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml_35/yaml/cyaml.py
+-rw-rw-rw-   0        0        0     2723 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml_35/yaml/dumper.py
+-rw-rw-rw-   0        0        0    42954 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml_35/yaml/emitter.py
+-rw-rw-rw-   0        0        0     2533 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml_35/yaml/error.py
+-rw-rw-rw-   0        0        0     2445 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml_35/yaml/events.py
+-rw-rw-rw-   0        0        0     1138 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml_35/yaml/loader.py
+-rw-rw-rw-   0        0        0     1440 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml_35/yaml/nodes.py
+-rw-rw-rw-   0        0        0    25495 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml_35/yaml/parser.py
+-rw-rw-rw-   0        0        0     6854 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml_35/yaml/reader.py
+-rw-rw-rw-   0        0        0    14097 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml_35/yaml/representer.py
+-rw-rw-rw-   0        0        0     8970 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml_35/yaml/resolver.py
+-rw-rw-rw-   0        0        0    51695 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml_35/yaml/scanner.py
+-rw-rw-rw-   0        0        0     4165 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml_35/yaml/serializer.py
+-rw-rw-rw-   0        0        0     2573 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml_35/yaml/tokens.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:10.863185 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/zstd/
+-rw-rw-rw-   0        0        0     1530 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/zstd/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:10.898340 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/zstd/common/
+-rw-rw-rw-   0        0        0    18198 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/zstd/common/bitstream.h
+-rw-rw-rw-   0        0        0    10157 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/zstd/common/compiler.h
+-rw-rw-rw-   0        0        0     4455 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/zstd/common/cpu.h
+-rw-rw-rw-   0        0        0     3763 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/zstd/common/debug.h
+-rw-rw-rw-   0        0        0    13662 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/zstd/common/entropy_common.c
+-rw-rw-rw-   0        0        0     3009 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/zstd/common/error_private.c
+-rw-rw-rw-   0        0        0     2441 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/zstd/common/error_private.h
+-rw-rw-rw-   0        0        0    34422 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/zstd/common/fse.h
+-rw-rw-rw-   0        0        0    14748 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/zstd/common/fse_decompress.c
+-rw-rw-rw-   0        0        0    20216 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/zstd/common/huf.h
+-rw-rw-rw-   0        0        0    13930 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/zstd/common/mem.h
+-rw-rw-rw-   0        0        0    26976 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/zstd/common/xxhash.c
+-rw-rw-rw-   0        0        0    11706 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/zstd/common/xxhash.h
+-rw-rw-rw-   0        0        0     2728 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/zstd/common/zstd_common.c
+-rw-rw-rw-   0        0        0     2497 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/zstd/common/zstd_deps.h
+-rw-rw-rw-   0        0        0     3828 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/zstd/common/zstd_errors.h
+-rw-rw-rw-   0        0        0    15880 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/zstd/common/zstd_internal.h
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:10.909604 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/zstd/decompress/
+-rw-rw-rw-   0        0        0    54982 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/zstd/decompress/huf_decompress.c
+-rw-rw-rw-   0        0        0     9164 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.c
+-rw-rw-rw-   0        0        0     1321 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.h
+-rw-rw-rw-   0        0        0    80283 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/zstd/decompress/zstd_decompress.c
+-rw-rw-rw-   0        0        0    66784 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.c
+-rw-rw-rw-   0        0        0     2253 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.h
+-rw-rw-rw-   0        0        0     7906 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_internal.h
+-rw-rw-rw-   0        0        0   138334 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/zstd/zstd.h
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.040000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/
+-rw-rw-rw-   0        0        0    82393 2023-07-25 02:10:30.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/CompiledAsyncgenType.c
+-rw-rw-rw-   0        0        0     8250 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/CompiledCellType.c
+-rw-rw-rw-   0        0        0    56307 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/CompiledCodeHelpers.c
+-rw-rw-rw-   0        0        0    71532 2023-07-25 02:10:30.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/CompiledCoroutineType.c
+-rw-rw-rw-   0        0        0    35861 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/CompiledFrameType.c
+-rw-rw-rw-   0        0        0   100376 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/CompiledFunctionType.c
+-rw-rw-rw-   0        0        0    61078 2023-07-25 02:10:30.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/CompiledGeneratorType.c
+-rw-rw-rw-   0        0        0    48523 2023-07-25 02:10:30.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/CompiledGeneratorTypeUncompiledIntegration.c
+-rw-rw-rw-   0        0        0    21638 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/CompiledMethodType.c
+-rw-rw-rw-   0        0        0    18993 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersAllocator.c
+-rw-rw-rw-   0        0        0    37540 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersAttributes.c
+-rw-rw-rw-   0        0        0    22263 2023-07-25 02:10:30.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersBuiltin.c
+-rw-rw-rw-   0        0        0   107641 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersBuiltinTypeMethods.c
+-rw-rw-rw-   0        0        0     3033 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersBytes.c
+-rw-rw-rw-   0        0        0    13057 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersCalling.c
+-rw-rw-rw-   0        0        0   470655 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersCallingGenerated.c
+-rw-rw-rw-   0        0        0     1617 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersChecksumTools.c
+-rw-rw-rw-   0        0        0     2991 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersClasses.c
+-rw-rw-rw-   0        0        0   317872 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersComparisonEq.c
+-rw-rw-rw-   0        0        0     4673 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersComparisonEqUtils.c
+-rw-rw-rw-   0        0        0   313003 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersComparisonGe.c
+-rw-rw-rw-   0        0        0   312414 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersComparisonGt.c
+-rw-rw-rw-   0        0        0   316217 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersComparisonLe.c
+-rw-rw-rw-   0        0        0   315628 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersComparisonLt.c
+-rw-rw-rw-   0        0        0   314618 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersComparisonNe.c
+-rw-rw-rw-   0        0        0    36068 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersConstantsBlob.c
+-rw-rw-rw-   0        0        0    19313 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersDeepcopy.c
+-rw-rw-rw-   0        0        0    38364 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersDictionaries.c
+-rw-rw-rw-   0        0        0    24295 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersDictionariesGenerated.c
+-rw-rw-rw-   0        0        0     7035 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersExceptions.c
+-rw-rw-rw-   0        0        0     6668 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersFiles.c
+-rw-rw-rw-   0        0        0    28131 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersFilesystemPaths.c
+-rw-rw-rw-   0        0        0     2426 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersFloats.c
+-rw-rw-rw-   0        0        0     1774 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersHeapStorage.c
+-rw-rw-rw-   0        0        0    14585 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersImport.c
+-rw-rw-rw-   0        0        0    14756 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersImportHard.c
+-rw-rw-rw-   0        0        0    18431 2023-07-25 02:10:30.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersLists.c
+-rw-rw-rw-   0        0        0    13915 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersListsGenerated.c
+-rw-rw-rw-   0        0        0     1640 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersMappings.c
+-rw-rw-rw-   0        0        0     3513 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersMatching.c
+-rw-rw-rw-   0        0        0   181243 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersOperationBinaryAdd.c
+-rw-rw-rw-   0        0        0    16700 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersOperationBinaryAddUtils.c
+-rw-rw-rw-   0        0        0    77943 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersOperationBinaryBitand.c
+-rw-rw-rw-   0        0        0    77782 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersOperationBinaryBitor.c
+-rw-rw-rw-   0        0        0    77943 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersOperationBinaryBitxor.c
+-rw-rw-rw-   0        0        0    67487 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersOperationBinaryDivmod.c
+-rw-rw-rw-   0        0        0     1236 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersOperationBinaryDivmodUtils.c
+-rw-rw-rw-   0        0        0    68748 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersOperationBinaryFloordiv.c
+-rw-rw-rw-   0        0        0     6274 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersOperationBinaryInplaceAdd.c
+-rw-rw-rw-   0        0        0    83405 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersOperationBinaryLshift.c
+-rw-rw-rw-   0        0        0    13776 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersOperationBinaryMatmult.c
+-rw-rw-rw-   0        0        0   183202 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersOperationBinaryMod.c
+-rw-rw-rw-   0        0        0   188514 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersOperationBinaryMult.c
+-rw-rw-rw-   0        0        0     3404 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersOperationBinaryMultUtils.c
+-rw-rw-rw-   0        0        0    66453 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersOperationBinaryOlddiv.c
+-rw-rw-rw-   0        0        0    78891 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersOperationBinaryPow.c
+-rw-rw-rw-   0        0        0     1023 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersOperationBinaryPowUtils.c
+-rw-rw-rw-   0        0        0    77305 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersOperationBinaryRshift.c
+-rw-rw-rw-   0        0        0    70465 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersOperationBinarySub.c
+-rw-rw-rw-   0        0        0    68005 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersOperationBinaryTruediv.c
+-rw-rw-rw-   0        0        0   149580 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersOperationInplaceAdd.c
+-rw-rw-rw-   0        0        0     4071 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersOperationInplaceAddUtils.c
+-rw-rw-rw-   0        0        0    53224 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersOperationInplaceBitand.c
+-rw-rw-rw-   0        0        0    53122 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersOperationInplaceBitor.c
+-rw-rw-rw-   0        0        0    53224 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersOperationInplaceBitxor.c
+-rw-rw-rw-   0        0        0    76512 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersOperationInplaceFloordiv.c
+-rw-rw-rw-   0        0        0    47568 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersOperationInplaceLshift.c
+-rw-rw-rw-   0        0        0    17742 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersOperationInplaceMatmult.c
+-rw-rw-rw-   0        0        0   136100 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersOperationInplaceMod.c
+-rw-rw-rw-   0        0        0   142211 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersOperationInplaceMult.c
+-rw-rw-rw-   0        0        0    74142 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersOperationInplaceOlddiv.c
+-rw-rw-rw-   0        0        0    82669 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersOperationInplacePow.c
+-rw-rw-rw-   0        0        0    45052 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersOperationInplaceRshift.c
+-rw-rw-rw-   0        0        0    82842 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersOperationInplaceSub.c
+-rw-rw-rw-   0        0        0    76343 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersOperationInplaceTruediv.c
+-rw-rw-rw-   0        0        0     3219 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersProfiling.c
+-rw-rw-rw-   0        0        0     3805 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersPythonPgo.c
+-rw-rw-rw-   0        0        0    15369 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersRaising.c
+-rw-rw-rw-   0        0        0     3758 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersSafeStrings.c
+-rw-rw-rw-   0        0        0     3730 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersSequences.c
+-rw-rw-rw-   0        0        0     1946 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersSlices.c
+-rw-rw-rw-   0        0        0    26642 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersStrings.c
+-rw-rw-rw-   0        0        0     4037 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersTuples.c
+-rw-rw-rw-   0        0        0     5578 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersTypes.c
+-rw-rw-rw-   0        0        0    11986 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/InspectPatcher.c
+-rw-rw-rw-   0        0        0    47877 2023-07-25 02:10:30.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/MainProgram.c
+-rw-rw-rw-   0        0        0    58887 2023-07-25 02:10:30.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/MetaPathBasedLoader.c
+-rw-rw-rw-   0        0        0     4513 2023-07-25 02:10:30.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/MetaPathBasedLoaderImportlibMetadataDistribution.c
+-rw-rw-rw-   0        0        0     6427 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/MetaPathBasedLoaderResourceReader.c
+-rw-rw-rw-   0        0        0    17285 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/MetaPathBasedLoaderResourceReaderFiles.c
+-rw-rw-rw-   0        0        0    36107 2023-07-25 02:26:00.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/OnefileBootstrap.c
+-rw-rw-rw-   0        0        0     8021 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.6/nuitka/build/static_src/OnefileSplashScreen.cpp
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.125067 Nuitka-winsvc-1.7.6/nuitka/code_generation/
+-rw-rw-rw-   0        0        0     6414 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/AsyncgenCodes.py
+-rw-rw-rw-   0        0        0    10599 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/AttributeCodes.py
+-rw-rw-rw-   0        0        0    21864 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/BinaryOperationHelperDefinitions.py
+-rw-rw-rw-   0        0        0     2339 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/BranchCodes.py
+-rw-rw-rw-   0        0        0    16492 2023-07-25 02:10:30.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/BuiltinCodes.py
+-rw-rw-rw-   0        0        0    35905 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/CallCodes.py
+-rw-rw-rw-   0        0        0     4896 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/ClassCodes.py
+-rw-rw-rw-   0        0        0    51533 2023-07-25 02:10:30.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/CodeGeneration.py
+-rw-rw-rw-   0        0        0     2375 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/CodeHelperSelection.py
+-rw-rw-rw-   0        0        0    14392 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/CodeHelpers.py
+-rw-rw-rw-   0        0        0     4879 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/CodeObjectCodes.py
+-rw-rw-rw-   0        0        0    17570 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/ComparisonCodes.py
+-rw-rw-rw-   0        0        0     4446 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/ComparisonHelperDefinitions.py
+-rw-rw-rw-   0        0        0     7335 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/ConditionalCodes.py
+-rw-rw-rw-   0        0        0     6539 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/ConstantCodes.py
+-rw-rw-rw-   0        0        0    31186 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/Contexts.py
+-rw-rw-rw-   0        0        0     8484 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/CoroutineCodes.py
+-rw-rw-rw-   0        0        0     1574 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/CtypesCodes.py
+-rw-rw-rw-   0        0        0    28478 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/DictCodes.py
+-rw-rw-rw-   0        0        0     2125 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/Emission.py
+-rw-rw-rw-   0        0        0     9325 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/ErrorCodes.py
+-rw-rw-rw-   0        0        0    12304 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/EvalCodes.py
+-rw-rw-rw-   0        0        0     8975 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/ExceptionCodes.py
+-rw-rw-rw-   0        0        0     7350 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/ExpressionCTypeSelectionHelpers.py
+-rw-rw-rw-   0        0        0     2093 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/ExpressionCodes.py
+-rw-rw-rw-   0        0        0    17725 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/FrameCodes.py
+-rw-rw-rw-   0        0        0    27968 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/FunctionCodes.py
+-rw-rw-rw-   0        0        0     7690 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/GeneratorCodes.py
+-rw-rw-rw-   0        0        0     5943 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/GlobalConstants.py
+-rw-rw-rw-   0        0        0     6911 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/GlobalsLocalsCodes.py
+-rw-rw-rw-   0        0        0     1794 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/IdCodes.py
+-rw-rw-rw-   0        0        0    13318 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/ImportCodes.py
+-rw-rw-rw-   0        0        0     1396 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/Indentation.py
+-rw-rw-rw-   0        0        0     1506 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/IndexCodes.py
+-rw-rw-rw-   0        0        0     1033 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/InjectCCodes.py
+-rw-rw-rw-   0        0        0     3432 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/IntegerCodes.py
+-rw-rw-rw-   0        0        0    12010 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/IteratorCodes.py
+-rw-rw-rw-   0        0        0     2022 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/LabelCodes.py
+-rw-rw-rw-   0        0        0     2612 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/LineNumberCodes.py
+-rw-rw-rw-   0        0        0    15906 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/ListCodes.py
+-rw-rw-rw-   0        0        0     6375 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/LoaderCodes.py
+-rw-rw-rw-   0        0        0     9951 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/LocalsDictCodes.py
+-rw-rw-rw-   0        0        0     3135 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/LoopCodes.py
+-rw-rw-rw-   0        0        0     1597 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/MatchCodes.py
+-rw-rw-rw-   0        0        0     6291 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/ModuleCodes.py
+-rw-rw-rw-   0        0        0     8118 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/Namify.py
+-rw-rw-rw-   0        0        0    12777 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/OperationCodes.py
+-rw-rw-rw-   0        0        0    29459 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/PackageResourceCodes.py
+-rw-rw-rw-   0        0        0     3021 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/PrintCodes.py
+-rw-rw-rw-   0        0        0     5474 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/PythonAPICodes.py
+-rw-rw-rw-   0        0        0    13095 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/RaisingCodes.py
+-rw-rw-rw-   0        0        0     3443 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/Reports.py
+-rw-rw-rw-   0        0        0     5234 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/ReturnCodes.py
+-rw-rw-rw-   0        0        0     6517 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/SetCodes.py
+-rw-rw-rw-   0        0        0    13949 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/SliceCodes.py
+-rw-rw-rw-   0        0        0     9809 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/StringCodes.py
+-rw-rw-rw-   0        0        0     8188 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/SubscriptCodes.py
+-rw-rw-rw-   0        0        0    11176 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/TryCodes.py
+-rw-rw-rw-   0        0        0     3786 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/TupleCodes.py
+-rw-rw-rw-   0        0        0    14717 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/VariableCodes.py
+-rw-rw-rw-   0        0        0     9121 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/VariableDeclarations.py
+-rw-rw-rw-   0        0        0     7881 2023-07-25 02:10:30.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/YieldCodes.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.138299 Nuitka-winsvc-1.7.6/nuitka/code_generation/c_types/
+-rw-rw-rw-   0        0        0     6069 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/c_types/CTypeBases.py
+-rw-rw-rw-   0        0        0     3399 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/c_types/CTypeBooleans.py
+-rw-rw-rw-   0        0        0     1804 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/c_types/CTypeCFloats.py
+-rw-rw-rw-   0        0        0     1378 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/c_types/CTypeCLongs.py
+-rw-rw-rw-   0        0        0     3610 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/c_types/CTypeModuleDictVariables.py
+-rw-rw-rw-   0        0        0     5128 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/c_types/CTypeNuitkaBooleans.py
+-rw-rw-rw-   0        0        0     5211 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/c_types/CTypeNuitkaInts.py
+-rw-rw-rw-   0        0        0     3955 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/c_types/CTypeNuitkaVoids.py
+-rw-rw-rw-   0        0        0    19628 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/c_types/CTypePyObjectPointers.py
+-rw-rw-rw-   0        0        0     2852 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/c_types/CTypeVoids.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/c_types/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.154899 Nuitka-winsvc-1.7.6/nuitka/code_generation/templates/
+-rw-rw-rw-   0        0        0     2885 2023-07-25 02:10:30.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/templates/CodeTemplatesAsyncgens.py
+-rw-rw-rw-   0        0        0     5865 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/templates/CodeTemplatesConstants.py
+-rw-rw-rw-   0        0        0     2961 2023-07-25 02:10:30.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/templates/CodeTemplatesCoroutines.py
+-rw-rw-rw-   0        0        0     2290 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/templates/CodeTemplatesExceptions.py
+-rw-rw-rw-   0        0        0     6339 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/templates/CodeTemplatesFrames.py
+-rw-rw-rw-   0        0        0     3321 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/templates/CodeTemplatesFunction.py
+-rw-rw-rw-   0        0        0     3306 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/templates/CodeTemplatesGeneratorFunction.py
+-rw-rw-rw-   0        0        0     2335 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/templates/CodeTemplatesIterators.py
+-rw-rw-rw-   0        0        0     4217 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/templates/CodeTemplatesLoader.py
+-rw-rw-rw-   0        0        0    21244 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/templates/CodeTemplatesModules.py
+-rw-rw-rw-   0        0        0     6640 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/templates/CodeTemplatesVariables.py
+-rw-rw-rw-   0        0        0     2475 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/templates/TemplateDebugWrapper.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/templates/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.199433 Nuitka-winsvc-1.7.6/nuitka/code_generation/templates_c/
+-rw-rw-rw-   0        0        0    11231 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/templates_c/CodeTemplateCallsMethodPositional.c.j2
+-rw-rw-rw-   0        0        0     5847 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/templates_c/CodeTemplateCallsMixed.c.j2
+-rw-rw-rw-   0        0        0    23760 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/templates_c/CodeTemplateCallsPositional.c.j2
+-rw-rw-rw-   0        0        0     5238 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/templates_c/CodeTemplateCallsPositionalMethodDescr.c.j2
+-rw-rw-rw-   0        0        0     1905 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/templates_c/CodeTemplateMakeListHinted.c.j2
+-rw-rw-rw-   0        0        0     1843 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/templates_c/CodeTemplateMakeListSmall.c.j2
+-rw-rw-rw-   0        0        0     2817 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/templates_c/HelperBuiltinMethodOperation.c.j2
+-rw-rw-rw-   0        0        0    12819 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/templates_c/HelperDictionaryCopy.c.j2
+-rw-rw-rw-   0        0        0     2044 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/templates_c/HelperImportHard.c.j2
+-rw-rw-rw-   0        0        0     2762 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/templates_c/HelperLongTools.c.j2
+-rw-rw-rw-   0        0        0     1544 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/templates_c/HelperObjectTools.c.j2
+-rw-rw-rw-   0        0        0     7197 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/templates_c/HelperOperationBinary.c.j2
+-rw-rw-rw-   0        0        0    12850 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/templates_c/HelperOperationComparison.c.j2
+-rw-rw-rw-   0        0        0     4288 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/templates_c/HelperOperationComparisonBytes.c.j2
+-rw-rw-rw-   0        0        0     2088 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/templates_c/HelperOperationComparisonFloat.c.j2
+-rw-rw-rw-   0        0        0     2118 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/templates_c/HelperOperationComparisonInt.c.j2
+-rw-rw-rw-   0        0        0     3933 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/templates_c/HelperOperationComparisonList.c.j2
+-rw-rw-rw-   0        0        0     7407 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/templates_c/HelperOperationComparisonLong.c.j2
+-rw-rw-rw-   0        0        0     4292 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/templates_c/HelperOperationComparisonStr.c.j2
+-rw-rw-rw-   0        0        0     3860 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/templates_c/HelperOperationComparisonTuple.c.j2
+-rw-rw-rw-   0        0        0     4487 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/templates_c/HelperOperationComparisonUnicode.c.j2
+-rw-rw-rw-   0        0        0    11579 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/templates_c/HelperOperationInplace.c.j2
+-rw-rw-rw-   0        0        0    19317 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/templates_c/HelperSlotsBinary.c.j2
+-rw-rw-rw-   0        0        0     2843 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/templates_c/HelperSlotsBytes.c.j2
+-rw-rw-rw-   0        0        0     3635 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/templates_c/HelperSlotsCommon.c.j2
+-rw-rw-rw-   0        0        0    11102 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/templates_c/HelperSlotsFloat.c.j2
+-rw-rw-rw-   0        0        0    15380 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/templates_c/HelperSlotsInt.c.j2
+-rw-rw-rw-   0        0        0     2979 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/templates_c/HelperSlotsList.c.j2
+-rw-rw-rw-   0        0        0    10421 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/templates_c/HelperSlotsLong.c.j2
+-rw-rw-rw-   0        0        0     2557 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/templates_c/HelperSlotsSet.c.j2
+-rw-rw-rw-   0        0        0     3020 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/templates_c/HelperSlotsStr.c.j2
+-rw-rw-rw-   0        0        0     2984 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/templates_c/HelperSlotsTuple.c.j2
+-rw-rw-rw-   0        0        0     3173 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/code_generation/templates_c/HelperSlotsUnicode.c.j2
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.205285 Nuitka-winsvc-1.7.6/nuitka/containers/
+-rw-rw-rw-   0        0        0     1435 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/containers/Namedtuples.py
+-rw-rw-rw-   0        0        0     6553 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/containers/OrderedDicts.py
+-rw-rw-rw-   0        0        0      554 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/containers/OrderedSets.py
+-rw-rw-rw-   0        0        0     4397 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/containers/OrderedSetsFallback.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/containers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.209191 Nuitka-winsvc-1.7.6/nuitka/distutils/
+-rw-rw-rw-   0        0        0     1964 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/distutils/Build.py
+-rw-rw-rw-   0        0        0    14219 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/distutils/DistutilCommands.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/distutils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.212120 Nuitka-winsvc-1.7.6/nuitka/finalizations/
+-rw-rw-rw-   0        0        0     1224 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/finalizations/Finalization.py
+-rw-rw-rw-   0        0        0     6110 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/finalizations/FinalizeMarkups.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/finalizations/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.224815 Nuitka-winsvc-1.7.6/nuitka/freezer/
+-rw-rw-rw-   0        0        0     7311 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/freezer/DependsExe.py
+-rw-rw-rw-   0        0        0     2584 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/freezer/DllDependenciesCommon.py
+-rw-rw-rw-   0        0        0    11992 2023-07-25 02:10:30.000000 Nuitka-winsvc-1.7.6/nuitka/freezer/DllDependenciesMacOS.py
+-rw-rw-rw-   0        0        0     7211 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/freezer/DllDependenciesPosix.py
+-rw-rw-rw-   0        0        0     6620 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/freezer/DllDependenciesWin32.py
+-rw-rw-rw-   0        0        0    17058 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.6/nuitka/freezer/IncludedDataFiles.py
+-rw-rw-rw-   0        0        0     9492 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/freezer/IncludedEntryPoints.py
+-rw-rw-rw-   0        0        0    10269 2023-07-25 02:26:00.000000 Nuitka-winsvc-1.7.6/nuitka/freezer/Onefile.py
+-rw-rw-rw-   0        0        0    26319 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/freezer/Standalone.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/freezer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.236534 Nuitka-winsvc-1.7.6/nuitka/importing/
+-rw-rw-rw-   0        0        0    11007 2023-06-25 05:57:17.000000 Nuitka-winsvc-1.7.6/nuitka/importing/IgnoreListing.py
+-rw-rw-rw-   0        0        0     2899 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/importing/ImportCache.py
+-rw-rw-rw-   0        0        0     6719 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.6/nuitka/importing/ImportResolving.py
+-rw-rw-rw-   0        0        0    28503 2023-07-25 02:10:30.000000 Nuitka-winsvc-1.7.6/nuitka/importing/Importing.py
+-rw-rw-rw-   0        0        0     4738 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/importing/PreloadedPackages.py
+-rw-rw-rw-   0        0        0    14918 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.6/nuitka/importing/Recursion.py
+-rw-rw-rw-   0        0        0    10981 2023-06-16 02:35:34.000000 Nuitka-winsvc-1.7.6/nuitka/importing/StandardLibrary.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/importing/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.354325 Nuitka-winsvc-1.7.6/nuitka/nodes/
+-rw-rw-rw-   0        0        0     3637 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/AsyncgenNodes.py
+-rw-rw-rw-   0        0        0     4082 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/AttributeLookupNodes.py
+-rw-rw-rw-   0        0        0    13567 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/AttributeNodes.py
+-rw-rw-rw-   0        0        0   378745 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/AttributeNodesGenerated.py
+-rw-rw-rw-   0        0        0     3823 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/BuiltinAllNodes.py
+-rw-rw-rw-   0        0        0     4098 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/BuiltinAnyNodes.py
+-rw-rw-rw-   0        0        0     2496 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/BuiltinComplexNodes.py
+-rw-rw-rw-   0        0        0     1698 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/BuiltinDecodingNodes.py
+-rw-rw-rw-   0        0        0     2727 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/BuiltinDecoratorNodes.py
+-rw-rw-rw-   0        0        0     4694 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/BuiltinDictNodes.py
+-rw-rw-rw-   0        0        0     4948 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/BuiltinFormatNodes.py
+-rw-rw-rw-   0        0        0     2142 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/BuiltinHashNodes.py
+-rw-rw-rw-   0        0        0     1424 2023-07-25 02:10:30.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/BuiltinInputNodes.py
+-rw-rw-rw-   0        0        0     5334 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/BuiltinIntegerNodes.py
+-rw-rw-rw-   0        0        0    12723 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/BuiltinIteratorNodes.py
+-rw-rw-rw-   0        0        0     1996 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/BuiltinLenNodes.py
+-rw-rw-rw-   0        0        0     3606 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/BuiltinNextNodes.py
+-rw-rw-rw-   0        0        0     3240 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/BuiltinOpenNodes.py
+-rw-rw-rw-   0        0        0   245536 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/BuiltinOperationNodeBasesGenerated.py
+-rw-rw-rw-   0        0        0    18589 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/BuiltinRangeNodes.py
+-rw-rw-rw-   0        0        0     9067 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/BuiltinRefNodes.py
+-rw-rw-rw-   0        0        0     3307 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/BuiltinSumNodes.py
+-rw-rw-rw-   0        0        0    13543 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/BuiltinTypeNodes.py
+-rw-rw-rw-   0        0        0     1573 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/BuiltinVarsNodes.py
+-rw-rw-rw-   0        0        0    26113 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/BytesNodes.py
+-rw-rw-rw-   0        0        0     6478 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/CallNodes.py
+-rw-rw-rw-   0        0        0     1550 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/Checkers.py
+-rw-rw-rw-   0        0        0   604445 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/ChildrenHavingMixins.py
+-rw-rw-rw-   0        0        0     8448 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/ClassNodes.py
+-rw-rw-rw-   0        0        0     6585 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/CodeObjectSpecs.py
+-rw-rw-rw-   0        0        0    21683 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/ComparisonNodes.py
+-rw-rw-rw-   0        0        0    30314 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/ConditionalNodes.py
+-rw-rw-rw-   0        0        0    46536 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/ConstantRefNodes.py
+-rw-rw-rw-   0        0        0    12213 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/ContainerMakingNodes.py
+-rw-rw-rw-   0        0        0     2834 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/ContainerOperationNodes.py
+-rw-rw-rw-   0        0        0     4581 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/CoroutineNodes.py
+-rw-rw-rw-   0        0        0     1714 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/CtypesNodes.py
+-rw-rw-rw-   0        0        0    51021 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/DictionaryNodes.py
+-rw-rw-rw-   0        0        0     7856 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/ExceptionNodes.py
+-rw-rw-rw-   0        0        0     7317 2023-06-25 05:57:17.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/ExecEvalNodes.py
+-rw-rw-rw-   0        0        0    44996 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/ExpressionBases.py
+-rw-rw-rw-   0        0        0    52352 2023-07-25 02:10:30.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/ExpressionBasesGenerated.py
+-rw-rw-rw-   0        0        0    21278 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/ExpressionShapeMixins.py
+-rw-rw-rw-   0        0        0    12156 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/FrameNodes.py
+-rw-rw-rw-   0        0        0     3544 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/FunctionAttributeNodes.py
+-rw-rw-rw-   0        0        0    39803 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/FunctionNodes.py
+-rw-rw-rw-   0        0        0     5376 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/FutureSpecs.py
+-rw-rw-rw-   0        0        0     6256 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/GeneratorNodes.py
+-rw-rw-rw-   0        0        0     6850 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/GlobalsLocalsNodes.py
+-rw-rw-rw-   0        0        0    76798 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/HardImportNodesGenerated.py
+-rw-rw-rw-   0        0        0     5508 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/ImportHardNodes.py
+-rw-rw-rw-   0        0        0    45942 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/ImportNodes.py
+-rw-rw-rw-   0        0        0     2733 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/IndicatorMixins.py
+-rw-rw-rw-   0        0        0     1502 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/InjectCNodes.py
+-rw-rw-rw-   0        0        0    11228 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/IterationHandles.py
+-rw-rw-rw-   0        0        0    11002 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/KeyValuePairNodes.py
+-rw-rw-rw-   0        0        0    16320 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/ListOperationNodes.py
+-rw-rw-rw-   0        0        0    23094 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/LocalsDictNodes.py
+-rw-rw-rw-   0        0        0    14922 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/LocalsScopes.py
+-rw-rw-rw-   0        0        0    15581 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/LoopNodes.py
+-rw-rw-rw-   0        0        0     1712 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/MatchNodes.py
+-rw-rw-rw-   0        0        0     6534 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/ModuleAttributeNodes.py
+-rw-rw-rw-   0        0        0    30972 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/ModuleNodes.py
+-rw-rw-rw-   0        0        0    24899 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/NodeBases.py
+-rw-rw-rw-   0        0        0    15128 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/NodeMakingHelpers.py
+-rw-rw-rw-   0        0        0     5550 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/NodeMetaClasses.py
+-rw-rw-rw-   0        0        0    31894 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/OperatorNodes.py
+-rw-rw-rw-   0        0        0     9134 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/OperatorNodesUnary.py
+-rw-rw-rw-   0        0        0     4202 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/OsSysNodes.py
+-rw-rw-rw-   0        0        0    12442 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/OutlineNodes.py
+-rw-rw-rw-   0        0        0    31534 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/PackageMetadataNodes.py
+-rw-rw-rw-   0        0        0     7901 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/PackageResourceNodes.py
+-rw-rw-rw-   0        0        0     3407 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/PrintNodes.py
+-rw-rw-rw-   0        0        0     6772 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/ReturnNodes.py
+-rw-rw-rw-   0        0        0     4715 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/SideEffectNodes.py
+-rw-rw-rw-   0        0        0    12501 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/SliceNodes.py
+-rw-rw-rw-   0        0        0    94880 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/StatementBasesGenerated.py
+-rw-rw-rw-   0        0        0     9430 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/StatementNodes.py
+-rw-rw-rw-   0        0        0    28658 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/StrNodes.py
+-rw-rw-rw-   0        0        0     3504 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/StringConcatenationNodes.py
+-rw-rw-rw-   0        0        0     8640 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/SubscriptNodes.py
+-rw-rw-rw-   0        0        0    17853 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/TryNodes.py
+-rw-rw-rw-   0        0        0     2405 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/TypeMatchNodes.py
+-rw-rw-rw-   0        0        0    11061 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/TypeNodes.py
+-rw-rw-rw-   0        0        0    39522 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/VariableAssignNodes.py
+-rw-rw-rw-   0        0        0    10746 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/VariableDelNodes.py
+-rw-rw-rw-   0        0        0     4574 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/VariableNameNodes.py
+-rw-rw-rw-   0        0        0    30982 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/VariableRefNodes.py
+-rw-rw-rw-   0        0        0     4748 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/VariableReleaseNodes.py
+-rw-rw-rw-   0        0        0     3902 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/YieldNodes.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.360143 Nuitka-winsvc-1.7.6/nuitka/nodes/shapes/
+-rw-rw-rw-   0        0        0   156243 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/shapes/BuiltinTypeShapes.py
+-rw-rw-rw-   0        0        0     4387 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/shapes/ControlFlowDescriptions.py
+-rw-rw-rw-   0        0        0     4567 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/shapes/ShapeMixins.py
+-rw-rw-rw-   0        0        0    42374 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/shapes/StandardShapes.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/nodes/shapes/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.373814 Nuitka-winsvc-1.7.6/nuitka/optimizations/
+-rw-rw-rw-   0        0        0     3279 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/optimizations/BytecodeDemotion.py
+-rw-rw-rw-   0        0        0     3920 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/optimizations/FunctionInlining.py
+-rw-rw-rw-   0        0        0     2144 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/optimizations/Graphs.py
+-rw-rw-rw-   0        0        0    10762 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/optimizations/Optimization.py
+-rw-rw-rw-   0        0        0    52370 2023-07-25 02:10:30.000000 Nuitka-winsvc-1.7.6/nuitka/optimizations/OptimizeBuiltinCalls.py
+-rw-rw-rw-   0        0        0     2272 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/optimizations/Tags.py
+-rw-rw-rw-   0        0        0    40896 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/optimizations/TraceCollections.py
+-rw-rw-rw-   0        0        0    23977 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/optimizations/ValueTraces.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/optimizations/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.375767 Nuitka-winsvc-1.7.6/nuitka/pgo/
+-rw-rw-rw-   0        0        0     4663 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/pgo/PGO.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/pgo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.379673 Nuitka-winsvc-1.7.6/nuitka/plugins/
+-rw-rw-rw-   0        0        0    40887 2023-07-25 02:10:30.000000 Nuitka-winsvc-1.7.6/nuitka/plugins/PluginBase.py
+-rw-rw-rw-   0        0        0    57995 2023-07-25 02:10:30.000000 Nuitka-winsvc-1.7.6/nuitka/plugins/Plugins.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/plugins/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.424142 Nuitka-winsvc-1.7.6/nuitka/plugins/standard/
+-rw-rw-rw-   0        0        0    22510 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.6/nuitka/plugins/standard/AntiBloatPlugin.py
+-rw-rw-rw-   0        0        0     3460 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/plugins/standard/ConsiderPyLintAnnotationsPlugin.py
+-rw-rw-rw-   0        0        0    10383 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.6/nuitka/plugins/standard/DataFilesPlugin.py
+-rw-rw-rw-   0        0        0     4404 2023-06-16 02:35:34.000000 Nuitka-winsvc-1.7.6/nuitka/plugins/standard/DelvewheelPlugin.py
+-rw-rw-rw-   0        0        0     5675 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/plugins/standard/DillPlugin.py
+-rw-rw-rw-   0        0        0    13744 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.6/nuitka/plugins/standard/DllFilesPlugin.py
+-rw-rw-rw-   0        0        0     2062 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/plugins/standard/EnumPlugin.py
+-rw-rw-rw-   0        0        0     1905 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/plugins/standard/EventletPlugin.py
+-rw-rw-rw-   0        0        0     1880 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/plugins/standard/GeventPlugin.py
+-rw-rw-rw-   0        0        0     3482 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/plugins/standard/GiPlugin.py
+-rw-rw-rw-   0        0        0     5027 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/plugins/standard/GlfwPlugin.py
+-rw-rw-rw-   0        0        0    18335 2023-06-16 02:35:34.000000 Nuitka-winsvc-1.7.6/nuitka/plugins/standard/ImplicitImports.py
+-rw-rw-rw-   0        0        0     4948 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/plugins/standard/KivyPlugin.py
+-rw-rw-rw-   0        0        0     7239 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.6/nuitka/plugins/standard/MatplotlibPlugin.py
+-rw-rw-rw-   0        0        0     6352 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.6/nuitka/plugins/standard/MultiprocessingPlugin.py
+-rw-rw-rw-   0        0        0     1187 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/plugins/standard/NumpyPlugin.py
+-rw-rw-rw-   0        0        0     6691 2023-07-25 02:10:30.000000 Nuitka-winsvc-1.7.6/nuitka/plugins/standard/OptionsNannyPlugin.py
+-rw-rw-rw-   0        0        0     1917 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/plugins/standard/PbrPlugin.py
+-rw-rw-rw-   0        0        0     4665 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/plugins/standard/PkgResourcesPlugin.py
+-rw-rw-rw-   0        0        0     6992 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/plugins/standard/PmwPlugin.py
+-rw-rw-rw-   0        0        0    50584 2023-07-25 02:10:30.000000 Nuitka-winsvc-1.7.6/nuitka/plugins/standard/PySidePyQtPlugin.py
+-rw-rw-rw-   0        0        0     2986 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.6/nuitka/plugins/standard/PywebViewPlugin.py
+-rw-rw-rw-   0        0        0     1160 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/plugins/standard/TensorflowPlugin.py
+-rw-rw-rw-   0        0        0    12242 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.6/nuitka/plugins/standard/TkinterPlugin.py
+-rw-rw-rw-   0        0        0     1140 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/plugins/standard/TorchPlugin.py
+-rw-rw-rw-   0        0        0    10191 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.6/nuitka/plugins/standard/TransformersPlugin.py
+-rw-rw-rw-   0        0        0     1073 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.6/nuitka/plugins/standard/TrioPlugin.py
+-rw-rw-rw-   0        0        0     5640 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/plugins/standard/UpxPlugin.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/plugins/standard/__init__.py
+-rw-rw-rw-   0        0        0   166853 2023-07-25 02:10:30.000000 Nuitka-winsvc-1.7.6/nuitka/plugins/standard/standard.nuitka-package.config.yml
+-rw-rw-rw-   0        0        0     2221 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/nuitka/plugins/standard/stdlib2.nuitka-package.config.yml
+-rw-rw-rw-   0        0        0     9940 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.6/nuitka/plugins/standard/stdlib3.nuitka-package.config.yml
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.428049 Nuitka-winsvc-1.7.6/nuitka/reports/
+-rw-rw-rw-   0        0        0     2209 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/reports/LicenseReport.rst.j2
+-rw-rw-rw-   0        0        0    17538 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/reports/Reports.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/reports/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.441721 Nuitka-winsvc-1.7.6/nuitka/specs/
+-rw-rw-rw-   0        0        0     5911 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/specs/BuiltinBytesOperationSpecs.py
+-rw-rw-rw-   0        0        0     2786 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/specs/BuiltinDictOperationSpecs.py
+-rw-rw-rw-   0        0        0     2541 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/specs/BuiltinListOperationSpecs.py
+-rw-rw-rw-   0        0        0    26553 2023-07-25 02:10:30.000000 Nuitka-winsvc-1.7.6/nuitka/specs/BuiltinParameterSpecs.py
+-rw-rw-rw-   0        0        0     6065 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/specs/BuiltinStrOperationSpecs.py
+-rw-rw-rw-   0        0        0     1159 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/specs/BuiltinTypeOperationSpecs.py
+-rw-rw-rw-   0        0        0     4802 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/specs/BuiltinUnicodeOperationSpecs.py
+-rw-rw-rw-   0        0        0     5263 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.6/nuitka/specs/HardImportSpecs.py
+-rw-rw-rw-   0        0        0    18740 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/specs/ParameterSpecs.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/specs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.443672 Nuitka-winsvc-1.7.6/nuitka/tools/
+-rw-rw-rw-   0        0        0     1603 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/tools/Basics.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.444649 Nuitka-winsvc-1.7.6/nuitka/tools/commercial/
+-rw-rw-rw-   0        0        0      815 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/tools/commercial/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.449534 Nuitka-winsvc-1.7.6/nuitka/tools/data_composer/
+-rw-rw-rw-   0        0        0    14250 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.6/nuitka/tools/data_composer/DataComposer.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/tools/data_composer/__init__.py
+-rw-rw-rw-   0        0        0     1306 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/tools/data_composer/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.453437 Nuitka-winsvc-1.7.6/nuitka/tools/environments/
+-rw-rw-rw-   0        0        0     2449 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/tools/environments/CreateEnvironment.py
+-rw-rw-rw-   0        0        0     3735 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/tools/environments/Virtualenv.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/tools/environments/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.454414 Nuitka-winsvc-1.7.6/nuitka/tools/general/
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/tools/general/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.456366 Nuitka-winsvc-1.7.6/nuitka/tools/general/dll_report/
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/tools/general/dll_report/__init__.py
+-rw-rw-rw-   0        0        0     2366 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/tools/general/dll_report/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.458320 Nuitka-winsvc-1.7.6/nuitka/tools/general/find_module/
+-rw-rw-rw-   0        0        0     3920 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.6/nuitka/tools/general/find_module/FindModuleCode.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/tools/general/find_module/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.462226 Nuitka-winsvc-1.7.6/nuitka/tools/onefile_compressor/
+-rw-rw-rw-   0        0        0    10345 2023-07-25 02:10:30.000000 Nuitka-winsvc-1.7.6/nuitka/tools/onefile_compressor/OnefileCompressor.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/tools/onefile_compressor/__init__.py
+-rw-rw-rw-   0        0        0     1311 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/tools/onefile_compressor/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.467110 Nuitka-winsvc-1.7.6/nuitka/tools/podman/
+-rw-rw-rw-   0        0        0     1872 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.6/nuitka/tools/podman/Podman.py
+-rw-rw-rw-   0        0        0      833 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.6/nuitka/tools/podman/__init__.py
+-rw-rw-rw-   0        0        0     6685 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.6/nuitka/tools/podman/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.469062 Nuitka-winsvc-1.7.6/nuitka/tools/profiler/
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/tools/profiler/__init__.py
+-rw-rw-rw-   0        0        0     2529 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/tools/profiler/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.471991 Nuitka-winsvc-1.7.6/nuitka/tools/scanning/
+-rw-rw-rw-   0        0        0     3344 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/tools/scanning/DisplayPackageDLLs.py
+-rw-rw-rw-   0        0        0     2095 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/tools/scanning/DisplayPackageData.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/tools/scanning/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.476873 Nuitka-winsvc-1.7.6/nuitka/tools/specialize/
+-rw-rw-rw-   0        0        0    51143 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/tools/specialize/CTypeDescriptions.py
+-rw-rw-rw-   0        0        0     7685 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/tools/specialize/Common.py
+-rw-rw-rw-   0        0        0    39625 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/tools/specialize/SpecializeC.py
+-rw-rw-rw-   0        0        0    34664 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.6/nuitka/tools/specialize/SpecializePython.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:31.000000 Nuitka-winsvc-1.7.6/nuitka/tools/specialize/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.490095 Nuitka-winsvc-1.7.6/nuitka/tools/testing/
+-rw-rw-rw-   0        0        0    55424 2023-07-25 02:10:30.000000 Nuitka-winsvc-1.7.6/nuitka/tools/testing/Common.py
+-rw-rw-rw-   0        0        0     1483 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/nuitka/tools/testing/Constructs.py
+-rw-rw-rw-   0        0        0     8940 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/nuitka/tools/testing/OutputComparison.py
+-rw-rw-rw-   0        0        0     1278 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/nuitka/tools/testing/Pythons.py
+-rw-rw-rw-   0        0        0     8024 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.6/nuitka/tools/testing/RuntimeTracing.py
+-rw-rw-rw-   0        0        0     5371 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/nuitka/tools/testing/SearchModes.py
+-rw-rw-rw-   0        0        0     3375 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/nuitka/tools/testing/Valgrind.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/nuitka/tools/testing/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.492677 Nuitka-winsvc-1.7.6/nuitka/tools/testing/check_reference_counts/
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/nuitka/tools/testing/check_reference_counts/__init__.py
+-rw-rw-rw-   0        0        0     3064 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/nuitka/tools/testing/check_reference_counts/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.493999 Nuitka-winsvc-1.7.6/nuitka/tools/testing/compare_with_cpython/
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/nuitka/tools/testing/compare_with_cpython/__init__.py
+-rw-rw-rw-   0        0        0    29429 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.6/nuitka/tools/testing/compare_with_cpython/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.495952 Nuitka-winsvc-1.7.6/nuitka/tools/testing/find_sxs_modules/
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/nuitka/tools/testing/find_sxs_modules/__init__.py
+-rw-rw-rw-   0        0        0     1949 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/nuitka/tools/testing/find_sxs_modules/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.499859 Nuitka-winsvc-1.7.6/nuitka/tools/testing/measure_construct_performance/
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/nuitka/tools/testing/measure_construct_performance/__init__.py
+-rw-rw-rw-   0        0        0     8755 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.6/nuitka/tools/testing/measure_construct_performance/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.502788 Nuitka-winsvc-1.7.6/nuitka/tools/testing/run_nuitka_tests/
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/nuitka/tools/testing/run_nuitka_tests/__init__.py
+-rw-rw-rw-   0        0        0    36321 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.6/nuitka/tools/testing/run_nuitka_tests/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.504740 Nuitka-winsvc-1.7.6/nuitka/tools/watch/
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/nuitka/tools/watch/__init__.py
+-rw-rw-rw-   0        0        0     9503 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/nuitka/tools/watch/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.546289 Nuitka-winsvc-1.7.6/nuitka/tree/
+-rw-rw-rw-   0        0        0    47135 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.6/nuitka/tree/Building.py
+-rw-rw-rw-   0        0        0    74608 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/nuitka/tree/ComplexCallHelperFunctions.py
+-rw-rw-rw-   0        0        0     1700 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/nuitka/tree/Extractions.py
+-rw-rw-rw-   0        0        0     2572 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/nuitka/tree/InternalModule.py
+-rw-rw-rw-   0        0        0     1511 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/nuitka/tree/Operations.py
+-rw-rw-rw-   0        0        0     2807 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/nuitka/tree/ReformulationAssertStatements.py
+-rw-rw-rw-   0        0        0    42768 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/nuitka/tree/ReformulationAssignmentStatements.py
+-rw-rw-rw-   0        0        0     2948 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/nuitka/tree/ReformulationBooleanExpressions.py
+-rw-rw-rw-   0        0        0    11693 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/nuitka/tree/ReformulationCallExpressions.py
+-rw-rw-rw-   0        0        0    15072 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/nuitka/tree/ReformulationClasses.py
+-rw-rw-rw-   0        0        0    37638 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/nuitka/tree/ReformulationClasses3.py
+-rw-rw-rw-   0        0        0     6430 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/nuitka/tree/ReformulationComparisonExpressions.py
+-rw-rw-rw-   0        0        0    21824 2023-07-25 02:10:30.000000 Nuitka-winsvc-1.7.6/nuitka/tree/ReformulationContractionExpressions.py
+-rw-rw-rw-   0        0        0    11061 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/nuitka/tree/ReformulationDictionaryCreation.py
+-rw-rw-rw-   0        0        0    14607 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/nuitka/tree/ReformulationExecStatements.py
+-rw-rw-rw-   0        0        0     7782 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/nuitka/tree/ReformulationForLoopStatements.py
+-rw-rw-rw-   0        0        0    30544 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.6/nuitka/tree/ReformulationFunctionStatements.py
+-rw-rw-rw-   0        0        0    13437 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/nuitka/tree/ReformulationImportStatements.py
+-rw-rw-rw-   0        0        0     6577 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/nuitka/tree/ReformulationLambdaExpressions.py
+-rw-rw-rw-   0        0        0    20962 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/nuitka/tree/ReformulationMatchStatements.py
+-rw-rw-rw-   0        0        0     2409 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/nuitka/tree/ReformulationMultidist.py
+-rw-rw-rw-   0        0        0     8194 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/nuitka/tree/ReformulationNamespacePackages.py
+-rw-rw-rw-   0        0        0     4658 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/nuitka/tree/ReformulationPrintStatements.py
+-rw-rw-rw-   0        0        0    15371 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/nuitka/tree/ReformulationSequenceCreation.py
+-rw-rw-rw-   0        0        0     4824 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/nuitka/tree/ReformulationSubscriptExpressions.py
+-rw-rw-rw-   0        0        0    14615 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/nuitka/tree/ReformulationTryExceptStatements.py
+-rw-rw-rw-   0        0        0     6982 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/nuitka/tree/ReformulationTryFinallyStatements.py
+-rw-rw-rw-   0        0        0     5674 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/nuitka/tree/ReformulationWhileLoopStatements.py
+-rw-rw-rw-   0        0        0    14341 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/nuitka/tree/ReformulationWithStatements.py
+-rw-rw-rw-   0        0        0     3088 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/nuitka/tree/ReformulationYieldExpressions.py
+-rw-rw-rw-   0        0        0    12746 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/nuitka/tree/SourceHandling.py
+-rw-rw-rw-   0        0        0     3757 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/nuitka/tree/SyntaxErrors.py
+-rw-rw-rw-   0        0        0    22973 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/nuitka/tree/TreeHelpers.py
+-rw-rw-rw-   0        0        0    20012 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/nuitka/tree/VariableClosure.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/nuitka/tree/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.590839 Nuitka-winsvc-1.7.6/nuitka/utils/
+-rw-rw-rw-   0        0        0     2655 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/nuitka/utils/AppDirs.py
+-rw-rw-rw-   0        0        0     3248 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/nuitka/utils/CStrings.py
+-rw-rw-rw-   0        0        0     3653 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/nuitka/utils/CommandLineOptions.py
+-rw-rw-rw-   0        0        0     4297 2023-06-16 02:35:34.000000 Nuitka-winsvc-1.7.6/nuitka/utils/Distributions.py
+-rw-rw-rw-   0        0        0     5794 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/nuitka/utils/Download.py
+-rw-rw-rw-   0        0        0    12781 2023-07-25 02:10:31.000000 Nuitka-winsvc-1.7.6/nuitka/utils/Execution.py
+-rw-rw-rw-   0        0        0    36129 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/nuitka/utils/FileOperations.py
+-rw-rw-rw-   0        0        0     2885 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/nuitka/utils/Hashing.py
+-rw-rw-rw-   0        0        0     2362 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/nuitka/utils/Images.py
+-rw-rw-rw-   0        0        0     6985 2023-07-25 02:10:31.000000 Nuitka-winsvc-1.7.6/nuitka/utils/Importing.py
+-rw-rw-rw-   0        0        0     8149 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/nuitka/utils/InstalledPythons.py
+-rw-rw-rw-   0        0        0     2224 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/nuitka/utils/InstanceCounters.py
+-rw-rw-rw-   0        0        0     4336 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/nuitka/utils/Jinja2.py
+-rw-rw-rw-   0        0        0     1238 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/nuitka/utils/Json.py
+-rw-rw-rw-   0        0        0     4304 2023-06-16 02:35:34.000000 Nuitka-winsvc-1.7.6/nuitka/utils/MacOSApp.py
+-rw-rw-rw-   0        0        0     5040 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/nuitka/utils/MemoryUsage.py
+-rw-rw-rw-   0        0        0     9062 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.6/nuitka/utils/ModuleNames.py
+-rw-rw-rw-   0        0        0     4309 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/nuitka/utils/ReExecute.py
+-rw-rw-rw-   0        0        0     3815 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/nuitka/utils/Rest.py
+-rw-rw-rw-   0        0        0    23096 2023-07-25 02:10:31.000000 Nuitka-winsvc-1.7.6/nuitka/utils/SharedLibraries.py
+-rw-rw-rw-   0        0        0     3664 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/nuitka/utils/Shebang.py
+-rw-rw-rw-   0        0        0     2591 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/nuitka/utils/Signing.py
+-rw-rw-rw-   0        0        0     6207 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/nuitka/utils/StaticLibraries.py
+-rw-rw-rw-   0        0        0     2602 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/nuitka/utils/ThreadedExecutor.py
+-rw-rw-rw-   0        0        0     2772 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/nuitka/utils/Timing.py
+-rw-rw-rw-   0        0        0    10826 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/nuitka/utils/Utils.py
+-rw-rw-rw-   0        0        0    10574 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/nuitka/utils/WindowsFileUsage.py
+-rw-rw-rw-   0        0        0    19540 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/nuitka/utils/WindowsResources.py
+-rw-rw-rw-   0        0        0     6108 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/nuitka/utils/Yaml.py
+-rw-rw-rw-   0        0        0      833 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/nuitka/utils/__init__.py
+-rw-rw-rw-   0        0        0      834 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-25 02:27:12.029069 Nuitka-winsvc-1.7.6/setup.cfg
+-rw-rw-rw-   0        0        0    15248 2023-07-25 02:26:00.000000 Nuitka-winsvc-1.7.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.591825 Nuitka-winsvc-1.7.6/tests/
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.711078 Nuitka-winsvc-1.7.6/tests/basics/
+-rw-rw-rw-   0        0        0     1766 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/basics/AssertsTest.py
+-rw-rw-rw-   0        0        0     5934 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/basics/AssignmentsTest.py
+-rw-rw-rw-   0        0        0     5866 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/basics/AssignmentsTest32.py
+-rw-rw-rw-   0        0        0     4055 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/basics/BranchingTest.py
+-rw-rw-rw-   0        0        0     1104 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/basics/BuiltinOverload.py
+-rw-rw-rw-   0        0        0     3749 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/basics/BuiltinSuperTest.py
+-rw-rw-rw-   0        0        0    17080 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/basics/BuiltinsTest.py
+-rw-rw-rw-   0        0        0      866 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/basics/ClassMinimalTest.py
+-rw-rw-rw-   0        0        0     4764 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/basics/ClassesTest.py
+-rw-rw-rw-   0        0        0     3414 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/basics/ClassesTest32.py
+-rw-rw-rw-   0        0        0     1406 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/basics/ClassesTest34.py
+-rw-rw-rw-   0        0        0     4698 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/basics/ComparisonChainsTest.py
+-rw-rw-rw-   0        0        0     4639 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/basics/ConstantsTest.py
+-rw-rw-rw-   0        0        0      995 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/basics/ConstantsTest27.py
+-rw-rw-rw-   0        0        0     1628 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/basics/DecoratorsTest.py
+-rw-rw-rw-   0        0        0     2317 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/basics/DefaultParametersTest.py
+-rw-rw-rw-   0        0        0     1127 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/basics/DoubleDeletionsTest.py
+-rw-rw-rw-   0        0        0      806 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/basics/EmptyModuleTest.py
+-rw-rw-rw-   0        0        0    14387 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/basics/ExceptionRaisingTest.py
+-rw-rw-rw-   0        0        0      961 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/basics/ExceptionRaisingTest32.py
+-rw-rw-rw-   0        0        0     1458 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/basics/ExceptionRaisingTest33.py
+-rw-rw-rw-   0        0        0     6747 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/basics/ExecEvalTest.py
+-rw-rw-rw-   0        0        0     1417 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/basics/ExtremeClosureTest.py
+-rw-rw-rw-   0        0        0     1658 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/basics/FunctionObjectsTest.py
+-rw-rw-rw-   0        0        0    12335 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/basics/FunctionsTest.py
+-rw-rw-rw-   0        0        0     3603 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/basics/FunctionsTest32.py
+-rw-rw-rw-   0        0        0     2627 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/basics/FunctionsTest_2.py
+-rw-rw-rw-   0        0        0      890 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/basics/FutureTest32.py
+-rw-rw-rw-   0        0        0     5809 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/basics/GeneratorExpressionsTest.py
+-rw-rw-rw-   0        0        0     1041 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/basics/GeneratorExpressionsTest_37.py
+-rw-rw-rw-   0        0        0     3824 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/basics/GlobalStatementTest.py
+-rw-rw-rw-   0        0        0     1286 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/basics/HelloWorldTest_2.py
+-rw-rw-rw-   0        0        0     2469 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/basics/ImportingTest.py
+-rw-rw-rw-   0        0        0     1296 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/basics/InplaceOperationsTest.py
+-rw-rw-rw-   0        0        0     4227 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/basics/InspectionTest.py
+-rw-rw-rw-   0        0        0     1504 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/basics/InspectionTest_35.py
+-rw-rw-rw-   0        0        0     1618 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/basics/InspectionTest_36.py
+-rw-rw-rw-   0        0        0     1671 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/basics/LambdasTest.py
+-rw-rw-rw-   0        0        0     2731 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/basics/LateClosureAssignmentTest.py
+-rw-rw-rw-   0        0        0     2923 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/basics/ListContractionsTest.py
+-rw-rw-rw-   0        0        0     3329 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/basics/LoopingTest.py
+-rw-rw-rw-   0        0        0     1536 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/basics/MainProgramsTest.py
+-rw-rw-rw-   0        0        0     1925 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/basics/ModuleAttributesTest.py
+-rw-rw-rw-   0        0        0     1988 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/basics/OperatorsTest.py
+-rw-rw-rw-   0        0        0    14903 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/basics/OrderChecksTest.py
+-rw-rw-rw-   0        0        0     1827 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/basics/OrderChecksTest27.py
+-rw-rw-rw-   0        0        0     1452 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/basics/OverflowFunctionsTest_2.py
+-rw-rw-rw-   0        0        0     5853 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/basics/ParameterErrorsTest.py
+-rw-rw-rw-   0        0        0     1899 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/basics/ParameterErrorsTest32.py
+-rw-rw-rw-   0        0        0      863 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/basics/PrintFutureTest.py
+-rw-rw-rw-   0        0        0     1413 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/basics/PrintingTest_2.py
+-rw-rw-rw-   0        0        0      878 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/basics/RecursionTest.py
+-rw-rw-rw-   0        0        0    23840 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/basics/ReferencingTest.py
+-rw-rw-rw-   0        0        0     2076 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/basics/ReferencingTest27.py
+-rw-rw-rw-   0        0        0     7819 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/basics/ReferencingTest33.py
+-rw-rw-rw-   0        0        0     4904 2023-07-25 02:10:31.000000 Nuitka-winsvc-1.7.6/tests/basics/ReferencingTest35.py
+-rw-rw-rw-   0        0        0     5446 2023-07-25 02:10:31.000000 Nuitka-winsvc-1.7.6/tests/basics/ReferencingTest36.py
+-rw-rw-rw-   0        0        0     2899 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/basics/ReferencingTest_2.py
+-rw-rw-rw-   0        0        0     1630 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/basics/SlotsTest.py
+-rw-rw-rw-   0        0        0     1159 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/basics/ThreadedGeneratorsTest.py
+-rw-rw-rw-   0        0        0    22966 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/basics/TrickAssignmentsTest32.py
+-rw-rw-rw-   0        0        0     1541 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/basics/TrickAssignmentsTest35.py
+-rw-rw-rw-   0        0        0     1788 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/basics/TrickAssignmentsTest_2.py
+-rw-rw-rw-   0        0        0     2086 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/basics/TryContinueFinallyTest.py
+-rw-rw-rw-   0        0        0     2212 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/basics/TryExceptContinueTest.py
+-rw-rw-rw-   0        0        0     2275 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/basics/TryExceptFinallyTest.py
+-rw-rw-rw-   0        0        0     2304 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/basics/TryExceptFramesTest.py
+-rw-rw-rw-   0        0        0     2842 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/basics/TryReturnFinallyTest.py
+-rw-rw-rw-   0        0        0     2328 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/basics/TryYieldFinallyTest.py
+-rw-rw-rw-   0        0        0     1093 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/basics/UnicodeTest.py
+-rw-rw-rw-   0        0        0     1877 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/basics/UnpackingTest35.py
+-rw-rw-rw-   0        0        0     2095 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/basics/VarargsTest.py
+-rw-rw-rw-   0        0        0     4879 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/basics/WithStatementsTest.py
+-rw-rw-rw-   0        0        0     3070 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/basics/YieldFromTest33.py
+-rw-rw-rw-   0        0        0     3821 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/basics/run_all.py
+-rw-rw-rw-   0        0        0     2271 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/basics/run_xml.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.715963 Nuitka-winsvc-1.7.6/tests/onefile/
+-rw-rw-rw-   0        0        0     1213 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/onefile/HelloWorldTest.py
+-rw-rw-rw-   0        0        0     1307 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/onefile/KeyboardInterruptTest.py
+-rw-rw-rw-   0        0        0     5816 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/onefile/run_all.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.732562 Nuitka-winsvc-1.7.6/tests/optimizations/
+-rw-rw-rw-   0        0        0      958 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/optimizations/ArgumentTypes.py
+-rw-rw-rw-   0        0        0     1055 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/optimizations/Attributes.py
+-rw-rw-rw-   0        0        0     1021 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/optimizations/Calls.py
+-rw-rw-rw-   0        0        0      921 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/optimizations/Conditions.py
+-rw-rw-rw-   0        0        0      909 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/optimizations/DecodingOperations.py
+-rw-rw-rw-   0        0        0     1212 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/optimizations/FormatStrings36.py
+-rw-rw-rw-   0        0        0     1150 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/optimizations/HardImports.py
+-rw-rw-rw-   0        0        0      974 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/optimizations/HardImports_2.py
+-rw-rw-rw-   0        0        0      918 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/optimizations/Iterations.py
+-rw-rw-rw-   0        0        0     1260 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/optimizations/Len.py
+-rw-rw-rw-   0        0        0     2262 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/optimizations/Operations.py
+-rw-rw-rw-   0        0        0     1333 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/optimizations/Subscripts.py
+-rw-rw-rw-   0        0        0     8736 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/optimizations/run_all.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.734515 Nuitka-winsvc-1.7.6/tests/packages/
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.735491 Nuitka-winsvc-1.7.6/tests/packages/package_import_success_after_failure/
+-rw-rw-rw-   0        0        0     2382 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/packages/package_import_success_after_failure/PackageImportSuccessAfterFailure.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.738422 Nuitka-winsvc-1.7.6/tests/packages/package_import_success_after_failure/variable_package/
+-rw-rw-rw-   0        0        0      942 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/packages/package_import_success_after_failure/variable_package/SomeModule.py
+-rw-rw-rw-   0        0        0     1168 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/packages/package_import_success_after_failure/variable_package/__init__.py
+-rw-rw-rw-   0        0        0     3671 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/packages/run_all.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:09.774181 Nuitka-winsvc-1.7.6/tests/packages/sub_package/
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.741354 Nuitka-winsvc-1.7.6/tests/packages/sub_package/kitty/
+-rw-rw-rw-   0        0        0     1230 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/packages/sub_package/kitty/__init__.py
+-rw-rw-rw-   0        0        0      908 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/packages/sub_package/kitty/bigkitty.py
+-rw-rw-rw-   0        0        0      910 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/packages/sub_package/kitty/smallkitty.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.745256 Nuitka-winsvc-1.7.6/tests/packages/sub_package/kitty/speak/
+-rw-rw-rw-   0        0        0      929 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/packages/sub_package/kitty/speak/__init__.py
+-rw-rw-rw-   0        0        0     1053 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/packages/sub_package/kitty/speak/hello.py
+-rw-rw-rw-   0        0        0      966 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/packages/sub_package/kitty/speak/miau.py
+-rw-rw-rw-   0        0        0      968 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/packages/sub_package/kitty/speak/purr.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:09.775158 Nuitka-winsvc-1.7.6/tests/packages/top_level_attributes_3/
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.749164 Nuitka-winsvc-1.7.6/tests/packages/top_level_attributes_3/some_package/
+-rw-rw-rw-   0        0        0     2336 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/packages/top_level_attributes_3/some_package/__init__.py
+-rw-rw-rw-   0        0        0      907 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/packages/top_level_attributes_3/some_package/some_module.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.751118 Nuitka-winsvc-1.7.6/tests/plugins/
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.753068 Nuitka-winsvc-1.7.6/tests/plugins/code_signing/
+-rw-rw-rw-   0        0        0     1170 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/plugins/code_signing/CodeSigningMain.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.755031 Nuitka-winsvc-1.7.6/tests/plugins/data_files/
+-rw-rw-rw-   0        0        0     1332 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/plugins/data_files/DataFilesMain.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.756974 Nuitka-winsvc-1.7.6/tests/plugins/data_files/data_files_package/
+-rw-rw-rw-   0        0        0      924 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/plugins/data_files/data_files_package/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/tests/plugins/data_files/data_files_package/lala.txt
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.757951 Nuitka-winsvc-1.7.6/tests/plugins/data_files/data_files_package/sub_dir/
+-rw-rw-rw-   0        0        0        0 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/tests/plugins/data_files/data_files_package/sub_dir/lulu.txt
+-rw-rw-rw-   0        0        0      255 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/tests/plugins/data_files/test_case.nuitka-package.config.yml
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.759904 Nuitka-winsvc-1.7.6/tests/plugins/parameters/
+-rw-rw-rw-   0        0        0     1019 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/plugins/parameters/ParametersMain.py
+-rw-rw-rw-   0        0        0     2168 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/plugins/parameters/parameter-using-plugin.py
+-rw-rw-rw-   0        0        0     3861 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/plugins/run_all.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.760880 Nuitka-winsvc-1.7.6/tests/programs/
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.761857 Nuitka-winsvc-1.7.6/tests/programs/absolute_import/
+-rw-rw-rw-   0        0        0      867 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/absolute_import/AbsoluteImportMain.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.768692 Nuitka-winsvc-1.7.6/tests/programs/absolute_import/foobar/
+-rw-rw-rw-   0        0        0      796 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/absolute_import/foobar/__init__.py
+-rw-rw-rw-   0        0        0     1043 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/absolute_import/foobar/foobar.py
+-rw-rw-rw-   0        0        0      879 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/absolute_import/foobar/local.py
+-rw-rw-rw-   0        0        0      860 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/absolute_import/foobar/util.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.769669 Nuitka-winsvc-1.7.6/tests/programs/case_imports1/
+-rw-rw-rw-   0        0        0      808 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/case_imports1/CasedImportingMain.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.770645 Nuitka-winsvc-1.7.6/tests/programs/case_imports1/path1/
+-rw-rw-rw-   0        0        0      798 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/case_imports1/path1/Some_Module.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.771622 Nuitka-winsvc-1.7.6/tests/programs/case_imports1/path1/Some_Package/
+-rw-rw-rw-   0        0        0      799 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/case_imports1/path1/Some_Package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.773114 Nuitka-winsvc-1.7.6/tests/programs/case_imports1/path2/
+-rw-rw-rw-   0        0        0      798 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/case_imports1/path2/some_module.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.774090 Nuitka-winsvc-1.7.6/tests/programs/case_imports1/path2/some_package/
+-rw-rw-rw-   0        0        0      799 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/case_imports1/path2/some_package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.775067 Nuitka-winsvc-1.7.6/tests/programs/case_imports2/
+-rw-rw-rw-   0        0        0      808 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/case_imports2/CasedImportingMain.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.776044 Nuitka-winsvc-1.7.6/tests/programs/case_imports2/path1/
+-rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/case_imports2/path1/some_module.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.777020 Nuitka-winsvc-1.7.6/tests/programs/case_imports2/path1/some_package/
+-rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/case_imports2/path1/some_package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.777020 Nuitka-winsvc-1.7.6/tests/programs/case_imports2/path2/
+-rw-rw-rw-   0        0        0      798 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/case_imports2/path2/Some_Module.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.778972 Nuitka-winsvc-1.7.6/tests/programs/case_imports2/path2/Some_Package/
+-rw-rw-rw-   0        0        0      799 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/case_imports2/path2/Some_Package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.779949 Nuitka-winsvc-1.7.6/tests/programs/case_imports3/
+-rw-rw-rw-   0        0        0     1075 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/case_imports3/CasedImportingMain.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.781903 Nuitka-winsvc-1.7.6/tests/programs/case_imports3/path1/
+-rw-rw-rw-   0        0        0      809 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/case_imports3/path1/Some_Module.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.782881 Nuitka-winsvc-1.7.6/tests/programs/case_imports3/path1/Some_Package/
+-rw-rw-rw-   0        0        0      810 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/case_imports3/path1/Some_Package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.784845 Nuitka-winsvc-1.7.6/tests/programs/case_imports3/path2/
+-rw-rw-rw-   0        0        0      809 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/case_imports3/path2/Some_Module.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.785810 Nuitka-winsvc-1.7.6/tests/programs/case_imports3/path2/Some_Package/
+-rw-rw-rw-   0        0        0      810 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/case_imports3/path2/Some_Package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.786786 Nuitka-winsvc-1.7.6/tests/programs/cyclic_imports/
+-rw-rw-rw-   0        0        0      801 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/cyclic_imports/CyclicImportsMain.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.789714 Nuitka-winsvc-1.7.6/tests/programs/cyclic_imports/cyclic_importing_package/
+-rw-rw-rw-   0        0        0      875 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/cyclic_imports/cyclic_importing_package/Child1.py
+-rw-rw-rw-   0        0        0      875 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/cyclic_imports/cyclic_importing_package/Child2.py
+-rw-rw-rw-   0        0        0      842 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/cyclic_imports/cyclic_importing_package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.793162 Nuitka-winsvc-1.7.6/tests/programs/dash_import/
+-rw-rw-rw-   0        0        0      888 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/dash_import/DashImportMain.py
+-rw-rw-rw-   0        0        0      817 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/dash_import/dash-module.py
+-rw-rw-rw-   0        0        0      817 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/dash_import/plus+module.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.794134 Nuitka-winsvc-1.7.6/tests/programs/dash_main/
+-rw-rw-rw-   0        0        0      809 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/dash_main/Dash-Main.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.795111 Nuitka-winsvc-1.7.6/tests/programs/deep/
+-rw-rw-rw-   0        0        0      898 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/deep/DeepProgramMain.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.799023 Nuitka-winsvc-1.7.6/tests/programs/deep/some_package/
+-rw-rw-rw-   0        0        0      980 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/deep/some_package/DeepBrother.py
+-rw-rw-rw-   0        0        0      909 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/deep/some_package/DeepChild.py
+-rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/deep/some_package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.801947 Nuitka-winsvc-1.7.6/tests/programs/deep/some_package/deep_package/
+-rw-rw-rw-   0        0        0      876 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/deep/some_package/deep_package/DeepDeepChild.py
+-rw-rw-rw-   0        0        0      952 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/deep/some_package/deep_package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.803573 Nuitka-winsvc-1.7.6/tests/programs/dunderinit_imports/
+-rw-rw-rw-   0        0        0      794 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/dunderinit_imports/DunderInitImportsMain.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.805394 Nuitka-winsvc-1.7.6/tests/programs/dunderinit_imports/package/
+-rw-rw-rw-   0        0        0      797 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/dunderinit_imports/package/SubModule.py
+-rw-rw-rw-   0        0        0      857 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/dunderinit_imports/package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.806370 Nuitka-winsvc-1.7.6/tests/programs/import_variants/
+-rw-rw-rw-   0        0        0     1005 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/import_variants/ImportVariationsMain.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.812232 Nuitka-winsvc-1.7.6/tests/programs/import_variants/some_package/
+-rw-rw-rw-   0        0        0      946 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/import_variants/some_package/Child1.py
+-rw-rw-rw-   0        0        0     1098 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/import_variants/some_package/Child2.py
+-rw-rw-rw-   0        0        0      822 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/import_variants/some_package/Child3.py
+-rw-rw-rw-   0        0        0      994 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/import_variants/some_package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.816136 Nuitka-winsvc-1.7.6/tests/programs/main_raises/
+-rw-rw-rw-   0        0        0      911 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/main_raises/ErrorMain.py
+-rw-rw-rw-   0        0        0      808 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/main_raises/ErrorRaising.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.820041 Nuitka-winsvc-1.7.6/tests/programs/main_raises2/
+-rw-rw-rw-   0        0        0     1080 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/main_raises2/ErrorInFunctionMain.py
+-rw-rw-rw-   0        0        0      808 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/main_raises2/ErrorRaising.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.821018 Nuitka-winsvc-1.7.6/tests/programs/module_attributes/
+-rw-rw-rw-   0        0        0     1529 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/module_attributes/ModuleAttributesMain.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.823949 Nuitka-winsvc-1.7.6/tests/programs/module_attributes/package_level1/
+-rw-rw-rw-   0        0        0     1744 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/module_attributes/package_level1/Nearby1.py
+-rw-rw-rw-   0        0        0     1611 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/module_attributes/package_level1/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.825899 Nuitka-winsvc-1.7.6/tests/programs/module_attributes/package_level1/package_level2/
+-rw-rw-rw-   0        0        0     1744 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/module_attributes/package_level1/package_level2/Nearby2.py
+-rw-rw-rw-   0        0        0     1611 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/module_attributes/package_level1/package_level2/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.827854 Nuitka-winsvc-1.7.6/tests/programs/module_attributes/package_level1/package_level2/package_level3/
+-rw-rw-rw-   0        0        0     1744 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/module_attributes/package_level1/package_level2/package_level3/Nearby3.py
+-rw-rw-rw-   0        0        0     1611 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/module_attributes/package_level1/package_level2/package_level3/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.831763 Nuitka-winsvc-1.7.6/tests/programs/module_exits/
+-rw-rw-rw-   0        0        0      869 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/module_exits/ErrorExitingModule.py
+-rw-rw-rw-   0        0        0      867 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/module_exits/Main.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.835665 Nuitka-winsvc-1.7.6/tests/programs/module_object_replacing/
+-rw-rw-rw-   0        0        0     1078 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/module_object_replacing/ModuleObjectReplacingMain.py
+-rw-rw-rw-   0        0        0     1359 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/module_object_replacing/SelfReplacingModule.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.836648 Nuitka-winsvc-1.7.6/tests/programs/multiprocessing_using/
+-rw-rw-rw-   0        0        0      990 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/multiprocessing_using/MultiprocessingUsingMain.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.840550 Nuitka-winsvc-1.7.6/tests/programs/multiprocessing_using/foo/
+-rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/multiprocessing_using/foo/__init__.py
+-rw-rw-rw-   0        0        0      836 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/multiprocessing_using/foo/__main__.py
+-rw-rw-rw-   0        0        0     1758 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/multiprocessing_using/foo/entry.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.841524 Nuitka-winsvc-1.7.6/tests/programs/named_imports/
+-rw-rw-rw-   0        0        0      846 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/named_imports/NamedImportsMain.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.843477 Nuitka-winsvc-1.7.6/tests/programs/named_imports/some_package/
+-rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/named_imports/some_package/SomeModule.py
+-rw-rw-rw-   0        0        0      824 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/named_imports/some_package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.844453 Nuitka-winsvc-1.7.6/tests/programs/named_imports/some_package/sub_package/
+-rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/named_imports/some_package/sub_package/SomeModule.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.845429 Nuitka-winsvc-1.7.6/tests/programs/package_code/
+-rw-rw-rw-   0        0        0      800 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/package_code/PackageInitCodeMain.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.849337 Nuitka-winsvc-1.7.6/tests/programs/package_code/some_package/
+-rw-rw-rw-   0        0        0      810 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/package_code/some_package/SomeModule.py
+-rw-rw-rw-   0        0        0      809 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/package_code/some_package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.853243 Nuitka-winsvc-1.7.6/tests/programs/package_contains_main/
+-rw-rw-rw-   0        0        0      789 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/package_contains_main/PackageContainsMain.py
+-rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/package_contains_main/__init__.py
+-rw-rw-rw-   0        0        0      801 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/package_contains_main/local.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.854219 Nuitka-winsvc-1.7.6/tests/programs/package_init_import/
+-rw-rw-rw-   0        0        0      823 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/package_init_import/PackageInitImportMain.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.857147 Nuitka-winsvc-1.7.6/tests/programs/package_init_import/some_package/
+-rw-rw-rw-   0        0        0     1008 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/package_init_import/some_package/PackageLocal.py
+-rw-rw-rw-   0        0        0     1169 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/package_init_import/some_package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.858125 Nuitka-winsvc-1.7.6/tests/programs/package_init_issue/
+-rw-rw-rw-   0        0        0      789 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/package_init_issue/PackageInitIssueMain.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.859100 Nuitka-winsvc-1.7.6/tests/programs/package_init_issue/some_package/
+-rw-rw-rw-   0        0        0      798 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/package_init_issue/some_package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.861054 Nuitka-winsvc-1.7.6/tests/programs/package_init_issue/some_package/child_package/
+-rw-rw-rw-   0        0        0      798 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/package_init_issue/some_package/child_package/SomeModule.py
+-rw-rw-rw-   0        0        0      795 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/package_init_issue/some_package/child_package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.862030 Nuitka-winsvc-1.7.6/tests/programs/package_missing_init/
+-rw-rw-rw-   0        0        0      926 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/package_missing_init/PackageMissingInitMain.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.863007 Nuitka-winsvc-1.7.6/tests/programs/package_missing_init/some_package/
+-rw-rw-rw-   0        0        0      965 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/package_missing_init/some_package/some_module.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.864964 Nuitka-winsvc-1.7.6/tests/programs/package_missing_init/some_package/sub_package/
+-rw-rw-rw-   0        0        0      977 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/package_missing_init/some_package/sub_package/some_sub_module.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.868866 Nuitka-winsvc-1.7.6/tests/programs/package_module_collision/
+-rw-rw-rw-   0        0        0      901 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/package_module_collision/PackageAndModuleNamedSameMain.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.870821 Nuitka-winsvc-1.7.6/tests/programs/package_module_collision/Something/
+-rw-rw-rw-   0        0        0      810 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/package_module_collision/Something/__init__.py
+-rw-rw-rw-   0        0        0      801 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/package_module_collision/something.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.872314 Nuitka-winsvc-1.7.6/tests/programs/package_overload/
+-rw-rw-rw-   0        0        0      852 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/package_overload/Main.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.875237 Nuitka-winsvc-1.7.6/tests/programs/package_overload/foo/
+-rw-rw-rw-   0        0        0      799 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/package_overload/foo/__init__.py
+-rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/package_overload/foo/bar.py
+-rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/package_overload/foo/bar2.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.877190 Nuitka-winsvc-1.7.6/tests/programs/package_prevents_submodule/
+-rw-rw-rw-   0        0        0     2972 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/package_prevents_submodule/PackagePreventsSubmoduleMain.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.879142 Nuitka-winsvc-1.7.6/tests/programs/package_prevents_submodule/some_package/
+-rw-rw-rw-   0        0        0     1078 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/package_prevents_submodule/some_package/__init__.py
+-rw-rw-rw-   0        0        0      800 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/package_prevents_submodule/some_package/some_module.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:09.805142 Nuitka-winsvc-1.7.6/tests/programs/package_program/
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.884028 Nuitka-winsvc-1.7.6/tests/programs/package_program/PackageAsMain/
+-rw-rw-rw-   0        0        0      888 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/package_program/PackageAsMain/__init__.py
+-rw-rw-rw-   0        0        0     1630 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/package_program/PackageAsMain/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.885980 Nuitka-winsvc-1.7.6/tests/programs/pkgutil_itermodules/
+-rw-rw-rw-   0        0        0     1728 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/pkgutil_itermodules/PkgUtilIterModulesMain.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.886954 Nuitka-winsvc-1.7.6/tests/programs/pkgutil_itermodules/some_package/
+-rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/pkgutil_itermodules/some_package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.889885 Nuitka-winsvc-1.7.6/tests/programs/pkgutil_itermodules/some_package/sub_package1/
+-rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleC.py
+-rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleD.py
+-rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/pkgutil_itermodules/some_package/sub_package1/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.893790 Nuitka-winsvc-1.7.6/tests/programs/pkgutil_itermodules/some_package/sub_package2/
+-rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleA.py
+-rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleB.py
+-rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/pkgutil_itermodules/some_package/sub_package2/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.894767 Nuitka-winsvc-1.7.6/tests/programs/pkgutil_usage/
+-rw-rw-rw-   0        0        0     1261 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/pkgutil_usage/PkgUtilUsageMain.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.901603 Nuitka-winsvc-1.7.6/tests/programs/pkgutil_usage/package/
+-rw-rw-rw-   0        0        0       13 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/tests/programs/pkgutil_usage/package/DATA_FILE.txt
+-rw-rw-rw-   0        0        0       14 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/tests/programs/pkgutil_usage/package/DATA_FILE2.txt
+-rw-rw-rw-   0        0        0       14 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/tests/programs/pkgutil_usage/package/DATA_FILE3.txt
+-rw-rw-rw-   0        0        0     1553 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/pkgutil_usage/package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.903368 Nuitka-winsvc-1.7.6/tests/programs/plugin_import/
+-rw-rw-rw-   0        0        0      859 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/plugin_import/PluginImportMain.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.904532 Nuitka-winsvc-1.7.6/tests/programs/plugin_import/some_package/
+-rw-rw-rw-   0        0        0      771 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/plugin_import/some_package/__init__.py
+-rw-rw-rw-   0        0        0      781 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/plugin_import/some_package/some_module.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.905508 Nuitka-winsvc-1.7.6/tests/programs/reimport_main_dynamic/
+-rw-rw-rw-   0        0        0      911 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/reimport_main_dynamic/ImportItselfDynamicMain.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.906486 Nuitka-winsvc-1.7.6/tests/programs/reimport_main_static/
+-rw-rw-rw-   0        0        0      898 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/reimport_main_static/ImportItselfStaticMain.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.908439 Nuitka-winsvc-1.7.6/tests/programs/relative_import/
+-rw-rw-rw-   0        0        0      842 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/relative_import/RelativeImportMain.py
+-rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/relative_import/dircache.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.910397 Nuitka-winsvc-1.7.6/tests/programs/resource_reader37/
+-rw-rw-rw-   0        0        0     1169 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/resource_reader37/ResourceReaderMain.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.912344 Nuitka-winsvc-1.7.6/tests/programs/resource_reader37/some_package/
+-rw-rw-rw-   0        0        0       13 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.7.6/tests/programs/resource_reader37/some_package/DATA_FILE.txt
+-rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/resource_reader37/some_package/__init__.py
+-rw-rw-rw-   0        0        0     6615 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/run_all.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.916252 Nuitka-winsvc-1.7.6/tests/programs/stdlib_overload/
+-rw-rw-rw-   0        0        0     1171 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/stdlib_overload/StdlibOverloadMain.py
+-rw-rw-rw-   0        0        0      799 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/stdlib_overload/pyexpat.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.926014 Nuitka-winsvc-1.7.6/tests/programs/stdlib_overload/some_package/
+-rw-rw-rw-   0        0        0      769 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/stdlib_overload/some_package/__init__.py
+-rw-rw-rw-   0        0        0      909 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/stdlib_overload/some_package/normal_importing.py
+-rw-rw-rw-   0        0        0      810 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/stdlib_overload/some_package/pyexpat.py
+-rw-rw-rw-   0        0        0     1236 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/stdlib_overload/some_package/star_importing.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.929930 Nuitka-winsvc-1.7.6/tests/programs/syntax_errors/
+-rw-rw-rw-   0        0        0      791 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/syntax_errors/IndentationErroring.py
+-rw-rw-rw-   0        0        0      800 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/syntax_errors/SyntaxErroring.py
+-rw-rw-rw-   0        0        0     1079 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/syntax_errors/SyntaxErrorsMain.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.934362 Nuitka-winsvc-1.7.6/tests/programs/unicode_bom/
+-rw-rw-rw-   0        0        0      963 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/unicode_bom/UnicodeBomMain.py
+-rw-rw-rw-   0        0        0      846 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/unicode_bom/unicode_bom.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.937320 Nuitka-winsvc-1.7.6/tests/programs/with space/
+-rw-rw-rw-   0        0        0      826 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/programs/with space/Space Main.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.939269 Nuitka-winsvc-1.7.6/tests/reflected/
+-rw-rw-rw-   0        0        0    14061 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/reflected/compile_itself.py
+-rw-rw-rw-   0        0        0     1243 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/run-tests
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.984721 Nuitka-winsvc-1.7.6/tests/standalone/
+-rw-rw-rw-   0        0        0     1058 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/standalone/BrotliUsing.py
+-rw-rw-rw-   0        0        0     2554 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/standalone/CtypesUsing.py
+-rw-rw-rw-   0        0        0     1136 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/standalone/FlaskUsing.py
+-rw-rw-rw-   0        0        0      990 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/standalone/GlfwUsing.py
+-rw-rw-rw-   0        0        0     1184 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/standalone/GtkUsing.py
+-rw-rw-rw-   0        0        0     1025 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/standalone/HexEncodingTest_2.py
+-rw-rw-rw-   0        0        0     1086 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/standalone/IdnaUsing.py
+-rw-rw-rw-   0        0        0     1151 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/standalone/LxmlUsing.py
+-rw-rw-rw-   0        0        0     1431 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/standalone/MatplotlibUsing.py
+-rw-rw-rw-   0        0        0     2538 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/standalone/MetadataPackagesUsing.py
+-rw-rw-rw-   0        0        0     1727 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/standalone/NumpyUsing.py
+-rw-rw-rw-   0        0        0      947 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/standalone/OpenGLUsing.py
+-rw-rw-rw-   0        0        0     1379 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/standalone/PandasUsing.py
+-rw-rw-rw-   0        0        0     1066 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/standalone/PasslibUsing.py
+-rw-rw-rw-   0        0        0     1216 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.6/tests/standalone/PendulumUsing.py
+-rw-rw-rw-   0        0        0     2074 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/standalone/PkgResourcesRequiresUsing.py
+-rw-rw-rw-   0        0        0     1067 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/standalone/PmwUsing.py
+-rw-rw-rw-   0        0        0     1085 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/standalone/PyQt5Plugins.py
+-rw-rw-rw-   0        0        0     1105 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/standalone/PyQt5SSLSupport.py
+-rw-rw-rw-   0        0        0     2050 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/standalone/PyQt5Using.py
+-rw-rw-rw-   0        0        0     1085 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/standalone/PyQt6Plugins.py
+-rw-rw-rw-   0        0        0     2050 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/standalone/PyQt6Using.py
+-rw-rw-rw-   0        0        0     1091 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/standalone/PySide6Plugins.py
+-rw-rw-rw-   0        0        0     1757 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/standalone/PySide6Using.py
+-rw-rw-rw-   0        0        0     1323 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/standalone/RsaUsing.py
+-rw-rw-rw-   0        0        0      973 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/standalone/ShlibUsing.py
+-rw-rw-rw-   0        0        0     1537 2023-07-18 02:13:42.000000 Nuitka-winsvc-1.7.6/tests/standalone/SocketUsing.py
+-rw-rw-rw-   0        0        0     1941 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/standalone/TkInterUsing.py
+-rw-rw-rw-   0        0        0     3228 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/standalone/Urllib3Using.py
+-rw-rw-rw-   0        0        0     1200 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/standalone/Win32ComUsing.py
+-rw-rw-rw-   0        0        0     9531 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/standalone/run_all.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:11.985693 Nuitka-winsvc-1.7.6/tests/standalone/zip_importer/
+-rw-rw-rw-   0        0        0     1264 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/standalone/zip_importer/ZipImporterMain.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:27:12.027116 Nuitka-winsvc-1.7.6/tests/syntax/
+-rw-rw-rw-   0        0        0      811 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/syntax/AsyncgenReturn36.py
+-rw-rw-rw-   0        0        0      868 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/syntax/BreakWithoutLoop.py
+-rw-rw-rw-   0        0        0      791 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/syntax/ClassReturn.py
+-rw-rw-rw-   0        0        0      970 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/syntax/ClosureDel_2.py
+-rw-rw-rw-   0        0        0      849 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/syntax/ContinueWithoutLoop.py
+-rw-rw-rw-   0        0        0      791 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/syntax/DuplicateArgument.py
+-rw-rw-rw-   0        0        0     1111 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/syntax/ExecWithNesting_2.py
+-rw-rw-rw-   0        0        0      826 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/syntax/FutureBraces.py
+-rw-rw-rw-   0        0        0      805 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/syntax/FutureUnknown.py
+-rw-rw-rw-   0        0        0     1041 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/syntax/GeneratorExpressions38.py
+-rw-rw-rw-   0        0        0      879 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/syntax/GeneratorReturn_2.py
+-rw-rw-rw-   0        0        0      792 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/syntax/GlobalForParameter.py
+-rw-rw-rw-   0        0        0      995 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/syntax/Importing32.py
+-rw-rw-rw-   0        0        0      799 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/syntax/IndentationError.py
+-rw-rw-rw-   0        0        0      915 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/syntax/LateFutureImport.py
+-rw-rw-rw-   0        0        0      841 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/syntax/MisplacedFutureImport.py
+-rw-rw-rw-   0        0        0      800 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/syntax/ModuleReturn.py
+-rw-rw-rw-   0        0        0      883 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/syntax/NonAsciiWithoutEncoding_2.py
+-rw-rw-rw-   0        0        0      794 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/syntax/NonlocalForParameter32.py
+-rw-rw-rw-   0        0        0      868 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/syntax/NonlocalNotFound32.py
+-rw-rw-rw-   0        0        0      908 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/syntax/StarImportExtra.py
+-rw-rw-rw-   0        0        0      869 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/syntax/SyntaxError.py
+-rw-rw-rw-   0        0        0      874 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/syntax/TryExceptAllNotLast.py
+-rw-rw-rw-   0        0        0      875 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/syntax/TryFinallyContinue_37.py
+-rw-rw-rw-   0        0        0      776 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/syntax/UnpackNoTuple.py
+-rw-rw-rw-   0        0        0      809 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/syntax/UnpackTwoStars32.py
+-rw-rw-rw-   0        0        0      793 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/syntax/YieldFromInModule.py
+-rw-rw-rw-   0        0        0      804 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/syntax/YieldInAsync35.py
+-rw-rw-rw-   0        0        0      923 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/syntax/YieldInGenexp38.py
+-rw-rw-rw-   0        0        0      781 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/syntax/YieldInModule.py
+-rw-rw-rw-   0        0        0     2203 2023-05-31 01:58:32.000000 Nuitka-winsvc-1.7.6/tests/syntax/run_all.py
```

### Comparing `Nuitka-winsvc-1.7.5/Changelog.rst` & `Nuitka-winsvc-1.7.6/Changelog.rst`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/Developer_Manual.rst` & `Nuitka-winsvc-1.7.6/Developer_Manual.rst`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/LICENSE.txt` & `Nuitka-winsvc-1.7.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/MANIFEST.in` & `Nuitka-winsvc-1.7.6/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/Nuitka_winsvc.egg-info/PKG-INFO` & `Nuitka-winsvc-1.7.6/Nuitka_winsvc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Nuitka-winsvc
-Version: 1.7.5
+Version: 1.7.6
 Summary: Nuitka but support compile as Windows service
 Home-page: https://github.com/tabris17/Nuitka-winsvc
 Author: tabris17
 Author-email: tabris17.cn@gmail.com
 License: Apache License, Version 2.0
 Project-URL: Source, https://github.com/tabris17/Nuitka-winsvc
 Keywords: windows service,compiler,python,nuitka
@@ -13,15 +13,14 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Software Development :: Compilers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: System :: Software Distribution
 Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `Nuitka-winsvc-1.7.5/Nuitka_winsvc.egg-info/SOURCES.txt` & `Nuitka-winsvc-1.7.6/Nuitka_winsvc.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1009,14 +1009,15 @@
 nuitka/nodes/BuiltinAnyNodes.py
 nuitka/nodes/BuiltinComplexNodes.py
 nuitka/nodes/BuiltinDecodingNodes.py
 nuitka/nodes/BuiltinDecoratorNodes.py
 nuitka/nodes/BuiltinDictNodes.py
 nuitka/nodes/BuiltinFormatNodes.py
 nuitka/nodes/BuiltinHashNodes.py
+nuitka/nodes/BuiltinInputNodes.py
 nuitka/nodes/BuiltinIntegerNodes.py
 nuitka/nodes/BuiltinIteratorNodes.py
 nuitka/nodes/BuiltinLenNodes.py
 nuitka/nodes/BuiltinNextNodes.py
 nuitka/nodes/BuiltinOpenNodes.py
 nuitka/nodes/BuiltinOperationNodeBasesGenerated.py
 nuitka/nodes/BuiltinRangeNodes.py
```

### Comparing `Nuitka-winsvc-1.7.5/PKG-INFO` & `Nuitka-winsvc-1.7.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Nuitka-winsvc
-Version: 1.7.5
+Version: 1.7.6
 Summary: Nuitka but support compile as Windows service
 Home-page: https://github.com/tabris17/Nuitka-winsvc
 Author: tabris17
 Author-email: tabris17.cn@gmail.com
 License: Apache License, Version 2.0
 Project-URL: Source, https://github.com/tabris17/Nuitka-winsvc
 Keywords: windows service,compiler,python,nuitka
@@ -13,15 +13,14 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Software Development :: Compilers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: System :: Software Distribution
 Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `Nuitka-winsvc-1.7.5/README.md` & `Nuitka-winsvc-1.7.6/README.md`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/README.rst` & `Nuitka-winsvc-1.7.6/README.rst`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/bin/autoformat-nuitka-source` & `Nuitka-winsvc-1.7.6/bin/autoformat-nuitka-source`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/bin/check-nuitka-with-pylint` & `Nuitka-winsvc-1.7.6/bin/check-nuitka-with-pylint`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/bin/compare_with_cpython` & `Nuitka-winsvc-1.7.6/bin/compare_with_cpython`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/bin/compare_with_xml` & `Nuitka-winsvc-1.7.6/bin/compare_with_xml`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/bin/measure-construct-performance` & `Nuitka-winsvc-1.7.6/bin/measure-construct-performance`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/bin/nuitka` & `Nuitka-winsvc-1.7.6/bin/nuitka`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/bin/nuitka-run` & `Nuitka-winsvc-1.7.6/bin/nuitka-run`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/doc/Logo/Nuitka-Logo-Horizontal.svg` & `Nuitka-winsvc-1.7.6/doc/Logo/Nuitka-Logo-Horizontal.svg`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/doc/Logo/Nuitka-Logo-Symbol.svg` & `Nuitka-winsvc-1.7.6/doc/Logo/Nuitka-Logo-Symbol.svg`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/doc/Logo/Nuitka-Logo-Vertical.svg` & `Nuitka-winsvc-1.7.6/doc/Logo/Nuitka-Logo-Vertical.svg`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/doc/images/Nuitka-Logo-Horizontal.png` & `Nuitka-winsvc-1.7.6/doc/images/Nuitka-Logo-Horizontal.png`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/doc/images/Nuitka-Logo-Symbol.png` & `Nuitka-winsvc-1.7.6/doc/images/Nuitka-Logo-Symbol.png`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/doc/images/Nuitka-Logo-Vertical.png` & `Nuitka-winsvc-1.7.6/doc/images/Nuitka-Logo-Vertical.png`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/lib/hints.py` & `Nuitka-winsvc-1.7.6/lib/hints.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/misc/nuitka-run.bat` & `Nuitka-winsvc-1.7.6/misc/nuitka-run.bat`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/misc/nuitka.bat` & `Nuitka-winsvc-1.7.6/misc/nuitka.bat`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/Builtins.py` & `Nuitka-winsvc-1.7.6/nuitka/Builtins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/BytecodeCaching.py` & `Nuitka-winsvc-1.7.6/nuitka/BytecodeCaching.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/Bytecodes.py` & `Nuitka-winsvc-1.7.6/nuitka/Bytecodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/CacheCleanup.py` & `Nuitka-winsvc-1.7.6/nuitka/CacheCleanup.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/Constants.py` & `Nuitka-winsvc-1.7.6/nuitka/Constants.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/Errors.py` & `Nuitka-winsvc-1.7.6/nuitka/Errors.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/MainControl.py` & `Nuitka-winsvc-1.7.6/nuitka/MainControl.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/ModuleRegistry.py` & `Nuitka-winsvc-1.7.6/nuitka/ModuleRegistry.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/OptionParsing.py` & `Nuitka-winsvc-1.7.6/nuitka/OptionParsing.py`

 * *Files 0% similar despite different names*

```diff
@@ -324,15 +324,15 @@
 )
 
 onefile_group.add_option(
     "--onefile-child-grace-time",
     action="store",
     dest="onefile_child_grace_time",
     metavar="GRACE_TIME_MS",
-    default="5000",
+    default=None,
     help="""\
 When stopping the child, e.g. due to CTRL-C or shutdown, etc. the
 Python code gets a "KeyboardInterrupt", that it may handle e.g. to
 flush data. This is the amount of time in ms, before the child it
 killed in the hard way. Unit is ms, and default 5000.""",
 )
```

### Comparing `Nuitka-winsvc-1.7.5/nuitka/Options.py` & `Nuitka-winsvc-1.7.6/nuitka/Options.py`

 * *Files 2% similar despite different names*

```diff
@@ -363,14 +363,50 @@
     if options.is_standalone:
         options.python_flags.insert(0, "no_site")
 
     # Check onefile tempdir spec.
     if options.onefile_tempdir_spec:
         _checkOnefileTargetSpec()
 
+        if not options.is_onefile:
+            Tracing.options_logger.warning(
+                """\
+Using onefile specific option '--onefile-windows-splash-screen-image' has no effect \
+when '--onefile' is not specified."""
+            )
+
+    # Check onefile splash image
+    if options.splash_screen_image:
+        if not os.path.exists(options.splash_screen_image):
+            Tracing.options_logger.sysexit(
+                "Error, splash screen image path '%s' does not exist."
+                % options.splash_screen_image
+            )
+
+        if not options.is_onefile:
+            Tracing.options_logger.warning(
+                """\
+Using onefile specific option '--onefile-windows-splash-screen-image' has no effect \
+when '--onefile' is not specified."""
+            )
+
+    if options.onefile_child_grace_time is not None:
+        if not options.onefile_child_grace_time.isdigit():
+            Tracing.options_logger.sysexit(
+                """\
+Error, value given for '--onefile-child-grace-time' must be integer."""
+            )
+
+        if not options.is_onefile:
+            Tracing.options_logger.warning(
+                """\
+Using onefile specific option '--onefile-windows-splash-screen-image' has no effect \
+when '--onefile-child-grace-time' is not specified."""
+            )
+
     if options.force_stdout_spec:
         checkPathSpec(
             options.force_stdout_spec, "--force-stdout-spec", allow_disable=True
         )
 
     if options.force_stderr_spec:
         checkPathSpec(
@@ -1373,15 +1409,15 @@
     """:returns: bool derived from ``--show-scons``"""
     return options.show_scons
 
 
 def getJobLimit():
     """*int*, value of ``--jobs`` / "-j" or number of CPU kernels"""
     if options.jobs is None:
-        if options.low_memory:
+        if isLowMemory():
             return 1
         else:
             return getCPUCoreCount()
 
     return int(options.jobs)
 
 
@@ -1606,15 +1642,19 @@
 
     # This changes the '/' to '\' on Windows at least.
     return os.path.normpath(result)
 
 
 def getOnefileChildGraceTime():
     """*int* = ``--onefile-child-grace-time``"""
-    return int(options.onefile_child_grace_time)
+    return (
+        int(options.onefile_child_grace_time)
+        if options.onefile_child_grace_time is not None
+        else 5000
+    )
 
 
 def shallNotCompressOnefile():
     """*bool* = ``--onefile-no-compression``"""
     return options.onefile_no_compression
```

### Comparing `Nuitka-winsvc-1.7.5/nuitka/OutputDirectories.py` & `Nuitka-winsvc-1.7.6/nuitka/OutputDirectories.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/PostProcessing.py` & `Nuitka-winsvc-1.7.6/nuitka/PostProcessing.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     putTextFileContents,
     removeFileExecutablePermission,
 )
 from nuitka.utils.Images import convertImageToIconFormat
 from nuitka.utils.MacOSApp import createPlistInfoFile
 from nuitka.utils.SharedLibraries import (
     callInstallNameTool,
-    convertRPathToRunPath,
+    cleanupHeaderForAndroid,
 )
 from nuitka.utils.Utils import isAndroidBasedLinux, isMacOS, isWin32Windows
 from nuitka.utils.WindowsResources import (
     RT_GROUP_ICON,
     RT_ICON,
     RT_RCDATA,
     addResourceToFile,
@@ -373,16 +373,16 @@
             os.path.dirname(result_filename),
             "lib" + os.path.basename(result_filename)[:-4] + ".a",
         )
 
         if os.path.exists(candidate):
             os.unlink(candidate)
 
-    if isAndroidBasedLinux() and not Options.shallMakeModule():
-        convertRPathToRunPath(result_filename)
+    if isAndroidBasedLinux():
+        cleanupHeaderForAndroid(result_filename)
 
     # Might have to create a CMD file, potentially with debugger run.
     if Options.shallCreateCmdFileForExecution():
         dll_directory = getExternalUsePath(os.path.dirname(getTargetPythonDLLPath()))
 
         cmd_filename = OutputDirectories.getResultRunFilename(onefile=False)
```

### Comparing `Nuitka-winsvc-1.7.5/nuitka/Progress.py` & `Nuitka-winsvc-1.7.6/nuitka/Progress.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/PythonFlavors.py` & `Nuitka-winsvc-1.7.6/nuitka/PythonFlavors.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/PythonOperators.py` & `Nuitka-winsvc-1.7.6/nuitka/PythonOperators.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/PythonVersions.py` & `Nuitka-winsvc-1.7.6/nuitka/PythonVersions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/Serialization.py` & `Nuitka-winsvc-1.7.6/nuitka/Serialization.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/SourceCodeReferences.py` & `Nuitka-winsvc-1.7.6/nuitka/SourceCodeReferences.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/Tracing.py` & `Nuitka-winsvc-1.7.6/nuitka/Tracing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/TreeXML.py` & `Nuitka-winsvc-1.7.6/nuitka/TreeXML.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/Variables.py` & `Nuitka-winsvc-1.7.6/nuitka/Variables.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/Version.py` & `Nuitka-winsvc-1.7.6/nuitka/Version.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 #     limitations under the License.
 #
 """ Nuitka version related stuff.
 
 """
 
 version_string = """\
-Nuitka V1.7.5
+Nuitka V1.7.6
 Copyright (C) 2023 Kay Hayen."""
 
 
 def getNuitkaVersion():
     """Return Nuitka version as a string.
 
     This should not be used for >= comparisons directly.
```

### Comparing `Nuitka-winsvc-1.7.5/nuitka/__init__.py` & `Nuitka-winsvc-1.7.6/nuitka/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/__main__.py` & `Nuitka-winsvc-1.7.6/nuitka/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/__past__.py` & `Nuitka-winsvc-1.7.6/nuitka/__past__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/Backend.scons` & `Nuitka-winsvc-1.7.6/nuitka/build/Backend.scons`

 * *Files 0% similar despite different names*

```diff
@@ -956,14 +956,17 @@
 
     if main_module_name != "__main__":
         build_definitions["NUITKA_MAIN_PACKAGE_MODE"] = 1
 
     createDefinitionsFile(source_dir, "build_definitions.h", build_definitions)
 
 
+if forced_stderr_path and not forced_stdout_path:
+    env.Append(CPPDEFINES=["NUITKA_STDERR_NOT_VISIBLE"])
+
 createBuildDefinitionsFile()
 
 # The meta path based loader might want to respect that, so it does verbose traces in module
 # mode, mostly for debugging purposes only.
 if module_mode and python_sysflag_verbose:
     env.Append(CPPDEFINES=["_NUITKA_SYSFLAG_VERBOSE=1"])
```

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/CCompilerVersion.scons` & `Nuitka-winsvc-1.7.6/nuitka/build/CCompilerVersion.scons`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/DataComposerInterface.py` & `Nuitka-winsvc-1.7.6/nuitka/build/DataComposerInterface.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/Onefile.scons` & `Nuitka-winsvc-1.7.6/nuitka/build/Onefile.scons`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/SconsCaching.py` & `Nuitka-winsvc-1.7.6/nuitka/build/SconsCaching.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/SconsCompilerSettings.py` & `Nuitka-winsvc-1.7.6/nuitka/build/SconsCompilerSettings.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/SconsHacks.py` & `Nuitka-winsvc-1.7.6/nuitka/build/SconsHacks.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/SconsInterface.py` & `Nuitka-winsvc-1.7.6/nuitka/build/SconsInterface.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/SconsProgress.py` & `Nuitka-winsvc-1.7.6/nuitka/build/SconsProgress.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/SconsSpawn.py` & `Nuitka-winsvc-1.7.6/nuitka/build/SconsSpawn.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/SconsUtils.py` & `Nuitka-winsvc-1.7.6/nuitka/build/SconsUtils.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/__init__.py` & `Nuitka-winsvc-1.7.6/nuitka/build/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/allocator.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/allocator.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/builtins.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/builtins.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/calling.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/calling.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/checkers.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/checkers.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/checksum_tools.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/checksum_tools.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/compiled_asyncgen.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/compiled_asyncgen.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/compiled_cell.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/compiled_cell.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/compiled_coroutine.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/compiled_coroutine.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/compiled_frame.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/compiled_frame.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/compiled_function.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/compiled_function.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/compiled_generator.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/compiled_generator.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/compiled_method.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/compiled_method.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/constants.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/constants.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/constants_blob.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/constants_blob.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/exceptions.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/exceptions.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/filesystem_paths.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/filesystem_paths.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/freelists.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/freelists.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/hedley.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/hedley.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/attributes.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/attributes.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/boolean.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/boolean.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/bytearrays.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/bytearrays.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/bytes.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/bytes.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/calling_generated.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/calling_generated.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/comparisons_eq.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/comparisons_eq.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/comparisons_ge.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/comparisons_ge.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/comparisons_gt.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/comparisons_gt.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/comparisons_le.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/comparisons_le.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/comparisons_lt.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/comparisons_lt.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/comparisons_ne.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/comparisons_ne.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/complex.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/complex.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/dictionaries.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/dictionaries.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/floats.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/floats.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/import_hard.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/import_hard.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/indexes.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/indexes.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/ints.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/ints.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/iterators.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/iterators.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/lists.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/lists.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/lists_generated.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/lists_generated.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/mappings.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/mappings.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/operations.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/operations.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/operations_binary_add.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/operations_binary_add.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/operations_binary_bitand.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/operations_binary_bitand.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/operations_binary_bitor.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/operations_binary_bitor.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/operations_binary_bitxor.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/operations_binary_bitxor.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/operations_binary_divmod.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/operations_binary_divmod.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/operations_binary_floordiv.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/operations_binary_floordiv.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/operations_binary_lshift.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/operations_binary_lshift.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/operations_binary_matmult.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/operations_binary_matmult.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/operations_binary_mod.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/operations_binary_mod.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/operations_binary_mult.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/operations_binary_mult.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/operations_binary_olddiv.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/operations_binary_olddiv.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/operations_binary_pow.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/operations_binary_pow.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/operations_binary_rshift.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/operations_binary_rshift.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/operations_binary_sub.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/operations_binary_sub.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/operations_binary_truediv.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/operations_binary_truediv.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/operations_builtin_types.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/operations_builtin_types.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/operations_inplace_add.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/operations_inplace_add.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/operations_inplace_bitand.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/operations_inplace_bitand.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/operations_inplace_bitor.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/operations_inplace_bitor.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/operations_inplace_bitxor.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/operations_inplace_bitxor.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/operations_inplace_floordiv.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/operations_inplace_floordiv.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/operations_inplace_lshift.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/operations_inplace_lshift.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/operations_inplace_matmult.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/operations_inplace_matmult.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/operations_inplace_mod.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/operations_inplace_mod.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/operations_inplace_mult.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/operations_inplace_mult.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/operations_inplace_olddiv.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/operations_inplace_olddiv.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/operations_inplace_pow.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/operations_inplace_pow.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/operations_inplace_rshift.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/operations_inplace_rshift.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/operations_inplace_sub.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/operations_inplace_sub.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/operations_inplace_truediv.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/operations_inplace_truediv.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/raising.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/raising.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/rangeobjects.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/rangeobjects.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/richcomparisons.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/richcomparisons.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/sequences.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/sequences.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/sets.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/sets.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/slices.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/slices.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/strings.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/strings.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/subscripts.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/subscripts.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helper/tuples.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helper/tuples.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/helpers.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/helpers.h`

 * *Files 2% similar despite different names*

```diff
@@ -275,14 +275,17 @@
 
 // For built-in staticmethod() functionality.
 extern PyObject *BUILTIN_STATICMETHOD(PyObject *function);
 
 // For built-in classmethod() functionality.
 extern PyObject *BUILTIN_CLASSMETHOD(PyObject *function);
 
+// For built-in input() functionality, prompt can be NULL.
+extern PyObject *BUILTIN_INPUT(PyObject *prompt);
+
 // For built-in "int()" functionality with 2 arguments.
 extern PyObject *BUILTIN_INT2(PyObject *value, PyObject *base);
 
 #if PYTHON_VERSION < 0x300
 // For built-in "long()" functionality with 2 arguments.
 extern PyObject *BUILTIN_LONG2(PyObject *value, PyObject *base);
 #endif
```

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/importing.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/importing.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/incbin.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/incbin.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/prelude.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/prelude.h`

 * *Files 4% similar despite different names*

```diff
@@ -323,24 +323,35 @@
 #define NUITKA_CROSS_MODULE
 #define NUITKA_LOCAL_MODULE static
 
 /* Due to ABI issues, it seems that on Windows the symbols used by
  * "_PyObject_GC_TRACK" were not exported before 3.8 and we need to use a
  * function that does it instead.
  *
- * TODO: Make it work for Win32 Python <= 3.7 too.
- * TODO: The Python 3.7.0 on Linux doesn't work this way either, was a bad
- * CPython release apparently.
+ * The Python 3.7.0 release on at Linux doesn't work this way either, was
+ * a bad CPython release apparently and between 3.7.3 and 3.7.4 these have
+ * become runtime incompatible.
  */
 #if (defined(_WIN32) || defined(__MSYS__)) && PYTHON_VERSION < 0x380
 #define Nuitka_GC_Track PyObject_GC_Track
 #define Nuitka_GC_UnTrack PyObject_GC_UnTrack
+#undef _PyObject_GC_TRACK
+#undef _PyObject_GC_UNTRACK
 #elif PYTHON_VERSION == 0x370
 #define Nuitka_GC_Track PyObject_GC_Track
 #define Nuitka_GC_UnTrack PyObject_GC_UnTrack
+#undef _PyObject_GC_TRACK
+#undef _PyObject_GC_UNTRACK
+#elif defined(_NUITKA_MODULE) && PYTHON_VERSION >= 0x370 && PYTHON_VERSION < 0x380
+#define Nuitka_GC_Track PyObject_GC_Track
+#define Nuitka_GC_UnTrack PyObject_GC_UnTrack
+#undef _PyObject_GC_TRACK
+#undef _PyObject_GC_UNTRACK
+#undef PyThreadState_GET
+#define PyThreadState_GET PyThreadState_Get
 #else
 #define Nuitka_GC_Track _PyObject_GC_TRACK
 #define Nuitka_GC_UnTrack _PyObject_GC_UNTRACK
 #endif
 
 #if _NUITKA_EXPERIMENTAL_FAST_THREAD_GET && PYTHON_VERSION >= 0x300 && PYTHON_VERSION < 0x370
 // We are careful, access without locking under the assumption that we hold
```

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/printing.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/printing.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/python_pgo.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/python_pgo.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/safe_string_ops.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/safe_string_ops.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/threading.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/threading.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/tracing.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/tracing.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/include/nuitka/unfreezing.h` & `Nuitka-winsvc-1.7.6/nuitka/build/include/nuitka/unfreezing.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/appdirs/LICENSE.txt` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/appdirs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/appdirs/appdirs.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/appdirs/appdirs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/atomicwrites/LICENSE` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/atomicwrites/LICENSE`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/atomicwrites/atomicwrites.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/atomicwrites/atomicwrites.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/bin/scons.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/bin/scons.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/clcache/clcache/LICENSE` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/clcache/clcache/LICENSE`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/clcache/clcache/caching.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/clcache/clcache/caching.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/colorama/LICENSE.txt` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/colorama/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/colorama/colorama/ansi.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/colorama/colorama/ansi.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/colorama/colorama/ansitowin32.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/colorama/colorama/ansitowin32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/colorama/colorama/initialise.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/colorama/colorama/initialise.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/colorama/colorama/win32.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/colorama/colorama/win32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/colorama/colorama/winterm.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/colorama/colorama/winterm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/glob2/LICENSE` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/glob2/LICENSE`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/glob2/glob2/compat.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/glob2/glob2/compat.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/glob2/glob2/fnmatch.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/glob2/glob2/fnmatch.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/glob2/glob2/impl.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/glob2/glob2/impl.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2/LICENSE.rst` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2/jinja2/__init__.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2/jinja2/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2/jinja2/_compat.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2/jinja2/_compat.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2/jinja2/_identifier.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2/jinja2/_identifier.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2/jinja2/bccache.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2/jinja2/bccache.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2/jinja2/compiler.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2/jinja2/compiler.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2/jinja2/constants.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2/jinja2/constants.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2/jinja2/debug.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2/jinja2/debug.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2/jinja2/defaults.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2/jinja2/defaults.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2/jinja2/environment.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2/jinja2/environment.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2/jinja2/exceptions.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2/jinja2/exceptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2/jinja2/ext.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2/jinja2/ext.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2/jinja2/filters.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2/jinja2/filters.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2/jinja2/idtracking.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2/jinja2/idtracking.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2/jinja2/lexer.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2/jinja2/lexer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2/jinja2/loaders.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2/jinja2/loaders.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2/jinja2/meta.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2/jinja2/meta.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2/jinja2/nativetypes.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2/jinja2/nativetypes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2/jinja2/nodes.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2/jinja2/nodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2/jinja2/optimizer.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2/jinja2/optimizer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2/jinja2/parser.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2/jinja2/parser.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2/jinja2/runtime.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2/jinja2/runtime.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2/jinja2/sandbox.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2/jinja2/sandbox.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2/jinja2/tests.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2/jinja2/tests.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2/jinja2/utils.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2/jinja2/utils.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2/jinja2/visitor.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2/jinja2/visitor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2_35/LICENSE.rst` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2_35/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2_35/jinja2/__init__.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2_35/jinja2/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2_35/jinja2/_compat.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2_35/jinja2/_compat.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2_35/jinja2/_identifier.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2_35/jinja2/_identifier.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2_35/jinja2/bccache.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2_35/jinja2/bccache.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2_35/jinja2/compiler.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2_35/jinja2/compiler.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2_35/jinja2/constants.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2_35/jinja2/constants.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2_35/jinja2/debug.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2_35/jinja2/debug.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2_35/jinja2/defaults.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2_35/jinja2/defaults.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2_35/jinja2/environment.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2_35/jinja2/environment.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2_35/jinja2/exceptions.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2_35/jinja2/exceptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2_35/jinja2/ext.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2_35/jinja2/ext.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2_35/jinja2/filters.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2_35/jinja2/filters.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2_35/jinja2/idtracking.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2_35/jinja2/idtracking.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2_35/jinja2/lexer.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2_35/jinja2/lexer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2_35/jinja2/loaders.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2_35/jinja2/loaders.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2_35/jinja2/meta.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2_35/jinja2/meta.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2_35/jinja2/nativetypes.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2_35/jinja2/nativetypes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2_35/jinja2/nodes.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2_35/jinja2/nodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2_35/jinja2/optimizer.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2_35/jinja2/optimizer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2_35/jinja2/parser.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2_35/jinja2/parser.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2_35/jinja2/runtime.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2_35/jinja2/runtime.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2_35/jinja2/sandbox.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2_35/jinja2/sandbox.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2_35/jinja2/tests.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2_35/jinja2/tests.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2_35/jinja2/utils.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2_35/jinja2/utils.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/jinja2_35/jinja2/visitor.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/jinja2_35/jinja2/visitor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Action.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Action.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Builder.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Builder.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/CacheDir.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/CacheDir.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Conftest.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Conftest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Debug.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Debug.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Defaults.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Defaults.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Environment.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Environment.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Errors.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Errors.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Executor.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Executor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Job.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Job.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Memoize.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Memoize.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Alias.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Alias.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/FS.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/FS.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Python.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Python.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/__init__.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/BoolOption.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/BoolOption.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/EnumOption.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/EnumOption.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/ListOption.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/ListOption.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PackageOption.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PackageOption.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PathOption.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PathOption.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/__init__.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/PathList.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/PathList.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/__init__.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/aix.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/aix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/cygwin.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/cygwin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/darwin.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/darwin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/hpux.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/hpux.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/irix.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/irix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/os2.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/os2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/posix.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/posix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/sunos.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/sunos.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/win32.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/win32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConf.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConf.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConsign.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConsign.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/C.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/C.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Dir.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Dir.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Prog.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Prog.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/RC.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/RC.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/__init__.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Interactive.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Interactive.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Main.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Main.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConsOptions.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConsOptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConscript.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConscript.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/__init__.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Sig.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Sig.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Subst.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Subst.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Taskmaster.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Taskmaster.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/386asm.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/386asm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/BitKeeper.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/BitKeeper.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/CVS.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/CVS.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/GettextCommon.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/GettextCommon.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/__init__.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/arch.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/arch.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/common.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/common.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/netframework.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/netframework.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/sdk.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/sdk.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vc.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vs.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Perforce.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Perforce.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/PharLapCommon.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/PharLapCommon.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/RCS.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/RCS.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/SCCS.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/SCCS.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Subversion.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Subversion.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/__init__.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixc++.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixcc.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixf77.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixf77.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixlink.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixlink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/applelink.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/applelink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ar.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/as.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/as.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/bcc32.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/bcc32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/c++.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/c++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cc.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cyglink.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cyglink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/default.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/default.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/docbook/__init__.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/docbook/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/filesystem.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/filesystem.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g++.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g77.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g77.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gas.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gas.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gcc.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gdc.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gdc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gettext.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gettext.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gfortran.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gfortran.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gnulink.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gnulink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpc++.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpcc.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hplink.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hplink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icc.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icl.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icl.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink32.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/install.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/install.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/intelc.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/intelc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/lex.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/lex.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/link.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/link.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/linkloc.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/linkloc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/m4.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/m4.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/masm.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/masm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mingw.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mingw.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgfmt.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgfmt.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msginit.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msginit.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgmerge.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgmerge.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslib.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslib.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslink.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mssdk.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mssdk.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvc.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvs.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwcc.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwld.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwld.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/nasm.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/nasm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rmic.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rmic.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rpcgen.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rpcgen.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgiar.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgiar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgic++.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgic++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgicc.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgicc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgilink.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgilink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunar.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunc++.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/suncc.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/suncc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunlink.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunlink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tar.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/textfile.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/textfile.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tlib.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tlib.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/wix.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/wix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/xgettext.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/xgettext.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/zip.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/zip.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Util.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Util.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/BoolVariable.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/BoolVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/EnumVariable.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/EnumVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/ListVariable.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/ListVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PackageVariable.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PackageVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PathVariable.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PathVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/__init__.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Warnings.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Warnings.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/__init__.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/__init__.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_builtins.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_builtins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_collections.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_collections.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_dbm.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_dbm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_hashlib.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_hashlib.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_io.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_io.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_sets.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_sets.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_subprocess.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_subprocess.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/cpp.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/cpp.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/dblite.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/dblite.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/exitfuncs.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/exitfuncs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Action.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Action.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Builder.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Builder.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/CacheDir.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/CacheDir.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Conftest.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Conftest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Debug.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Debug.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Defaults.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Defaults.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Environment.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Environment.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Errors.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Errors.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Executor.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Executor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Job.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Job.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Memoize.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Memoize.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Alias.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Alias.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/FS.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/FS.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Python.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Python.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/__init__.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/PathList.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/PathList.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/__init__.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/aix.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/aix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/cygwin.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/cygwin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/darwin.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/darwin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/hpux.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/hpux.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/irix.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/irix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/mingw.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/mingw.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/os2.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/os2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/posix.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/posix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/sunos.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/sunos.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/virtualenv.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/virtualenv.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/win32.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/win32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConf.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConf.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConsign.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConsign.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/C.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/C.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Dir.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Dir.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Prog.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Prog.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/RC.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/RC.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/__init__.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Interactive.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Interactive.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Main.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Main.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConsOptions.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConsOptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConscript.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConscript.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/__init__.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Subst.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Subst.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Taskmaster.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Taskmaster.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/386asm.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/386asm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/GettextCommon.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/GettextCommon.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/__init__.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/arch.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/arch.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/common.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/common.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/netframework.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/netframework.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/sdk.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/sdk.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vc.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vs.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/PharLapCommon.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/PharLapCommon.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/__init__.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixc++.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcc.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcxx.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixlink.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixlink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/applelink.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/applelink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ar.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/as.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/as.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/bcc32.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/bcc32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/c++.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/c++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cc.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clang.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clang.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangxx.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cxx.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cyglink.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cyglink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/default.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/default.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/docbook/__init__.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/docbook/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/filesystem.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/filesystem.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/g++.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/g++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gas.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gas.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gcc.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gettext_tool.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gettext_tool.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gnulink.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gnulink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gxx.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpc++.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcc.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcxx.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hplink.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hplink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icc.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icl.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icl.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink32.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/install.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/install.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/intelc.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/intelc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/link.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/link.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/linkloc.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/linkloc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/m4.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/m4.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/masm.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/masm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mingw.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mingw.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgfmt.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgfmt.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msginit.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msginit.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgmerge.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgmerge.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslib.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslib.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslink.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mssdk.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mssdk.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvc.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvs.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwcc.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwld.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwld.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/nasm.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/nasm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rmic.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rmic.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rpcgen.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rpcgen.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgiar.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgiar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgic++.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgic++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicc.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicxx.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgilink.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgilink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunar.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunc++.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncc.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncxx.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunlink.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunlink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tar.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/textfile.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/textfile.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tlib.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tlib.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/wix.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/wix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/xgettext.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/xgettext.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/zip.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/zip.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Util.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Util.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/BoolVariable.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/BoolVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/EnumVariable.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/EnumVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/ListVariable.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/ListVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PackageVariable.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PackageVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PathVariable.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PathVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/__init__.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Warnings.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Warnings.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/__init__.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/__init__.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/_scons_dbm.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/_scons_dbm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/cpp.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/cpp.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/dblite.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/dblite.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/exitfuncs.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/exitfuncs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Action.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Action.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Builder.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Builder.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/CacheDir.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/CacheDir.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Conftest.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Conftest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Debug.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Debug.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Defaults.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Defaults.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Environment.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Environment.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/EnvironmentValues.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/EnvironmentValues.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Errors.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Errors.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Executor.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Executor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Job.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Job.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Memoize.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Memoize.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Alias.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Alias.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/FS.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/FS.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Python.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Python.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/__init__.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/PathList.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/PathList.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/__init__.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/aix.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/aix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/cygwin.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/cygwin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/darwin.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/darwin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/hpux.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/hpux.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/irix.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/irix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/mingw.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/mingw.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/os2.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/os2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/posix.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/posix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/sunos.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/sunos.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/virtualenv.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/virtualenv.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/win32.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/win32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConf.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConf.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConsign.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConsign.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/C.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/C.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Dir.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Dir.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Prog.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Prog.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/RC.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/RC.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/__init__.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Interactive.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Interactive.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Main.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Main.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConsOptions.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConsOptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConscript.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConscript.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/__init__.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Subst.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Subst.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Taskmaster.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Taskmaster.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/386asm.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/386asm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/GettextCommon.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/GettextCommon.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/__init__.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/arch.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/arch.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/common.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/common.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/netframework.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/netframework.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/sdk.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/sdk.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vc.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vs.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/PharLapCommon.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/PharLapCommon.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/__init__.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixc++.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcc.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcxx.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixlink.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixlink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/applelink.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/applelink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ar.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/as.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/as.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/asm.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/asm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/bcc32.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/bcc32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/c++.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/c++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cc.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clang.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clang.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangxx.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cxx.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cyglink.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cyglink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/default.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/default.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/filesystem.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/filesystem.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/g++.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/g++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gas.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gas.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gcc.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gettext_tool.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gettext_tool.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gnulink.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gnulink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gxx.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpc++.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcc.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcxx.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hplink.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hplink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icc.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icl.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icl.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink32.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/install.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/install.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/intelc.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/intelc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/link.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/link.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/LoadableModule.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/LoadableModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/SharedLibrary.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/SharedLibrary.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/__init__.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkloc.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkloc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/m4.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/m4.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/masm.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/masm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mingw.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mingw.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgfmt.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgfmt.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msginit.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msginit.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgmerge.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgmerge.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslib.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslib.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslink.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mssdk.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mssdk.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvc.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvs.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwcc.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwld.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwld.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/nasm.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/nasm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rmic.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rmic.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rpcgen.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rpcgen.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgiar.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgiar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgic++.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgic++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicc.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicxx.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgilink.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgilink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunar.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunc++.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncc.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncxx.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunlink.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunlink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tar.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/textfile.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/textfile.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tlib.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tlib.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/wix.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/wix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/xgettext.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/xgettext.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/zip.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/zip.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Util.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Util.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/ConfigureCache.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/ConfigureCache.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/sconsign.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/sconsign.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/BoolVariable.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/BoolVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/EnumVariable.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/EnumVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/ListVariable.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/ListVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PackageVariable.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PackageVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PathVariable.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PathVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/__init__.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Warnings.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Warnings.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/__init__.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/_scons_dbm.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/_scons_dbm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/win32.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/win32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/cpp.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/cpp.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/dblite.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/dblite.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/exitfuncs.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/exitfuncs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/markupsafe/LICENSE.rst` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/markupsafe/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/markupsafe/markupsafe/__init__.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/markupsafe/markupsafe/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/markupsafe/markupsafe/_compat.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/markupsafe/markupsafe/_compat.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/markupsafe/markupsafe/_constants.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/markupsafe/markupsafe/_constants.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/markupsafe/markupsafe/_native.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/markupsafe/markupsafe/_native.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/pkg_resources/pkg_resources/__init__.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/pkg_resources/pkg_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/pkg_resources/pkg_resources/py31compat.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/pkg_resources/pkg_resources/py31compat.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/tqdm/tqdm/__init__.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/tqdm/tqdm/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/tqdm/tqdm/_monitor.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/tqdm/tqdm/_monitor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/tqdm/tqdm/_tqdm_pandas.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/tqdm/tqdm/_tqdm_pandas.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/tqdm/tqdm/_utils.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/tqdm/tqdm/_utils.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/tqdm/tqdm/auto.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/tqdm/tqdm/auto.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/tqdm/tqdm/autonotebook.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/tqdm/tqdm/autonotebook.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/tqdm/tqdm/dask.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/tqdm/tqdm/dask.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/tqdm/tqdm/gui.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/tqdm/tqdm/gui.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/tqdm/tqdm/notebook.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/tqdm/tqdm/notebook.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/tqdm/tqdm/std.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/tqdm/tqdm/std.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/tqdm/tqdm/tk.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/tqdm/tqdm/tk.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/tqdm/tqdm/utils.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/tqdm/tqdm/utils.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml/LICENSE` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml/LICENSE`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml/yaml/__init__.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml/yaml/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml/yaml/composer.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml/yaml/composer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml/yaml/constructor.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml/yaml/constructor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml/yaml/cyaml.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml/yaml/cyaml.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml/yaml/dumper.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml/yaml/dumper.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml/yaml/emitter.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml/yaml/emitter.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml/yaml/error.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml/yaml/error.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml/yaml/events.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml/yaml/events.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml/yaml/loader.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml/yaml/loader.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml/yaml/nodes.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml/yaml/nodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml/yaml/parser.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml/yaml/parser.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml/yaml/reader.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml/yaml/reader.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml/yaml/representer.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml/yaml/representer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml/yaml/resolver.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml/yaml/resolver.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml/yaml/scanner.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml/yaml/scanner.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml/yaml/serializer.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml/yaml/serializer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml/yaml/tokens.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml/yaml/tokens.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml_27/LICENSE` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml_27/LICENSE`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml_27/yaml/__init__.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml_27/yaml/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml_27/yaml/composer.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml_27/yaml/composer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml_27/yaml/constructor.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml_27/yaml/constructor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml_27/yaml/cyaml.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml_27/yaml/cyaml.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml_27/yaml/dumper.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml_27/yaml/dumper.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml_27/yaml/emitter.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml_27/yaml/emitter.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml_27/yaml/error.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml_27/yaml/error.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml_27/yaml/events.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml_27/yaml/events.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml_27/yaml/loader.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml_27/yaml/loader.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml_27/yaml/nodes.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml_27/yaml/nodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml_27/yaml/parser.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml_27/yaml/parser.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml_27/yaml/reader.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml_27/yaml/reader.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml_27/yaml/representer.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml_27/yaml/representer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml_27/yaml/resolver.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml_27/yaml/resolver.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml_27/yaml/scanner.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml_27/yaml/scanner.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml_27/yaml/serializer.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml_27/yaml/serializer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml_27/yaml/tokens.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml_27/yaml/tokens.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml_35/LICENSE` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml_35/LICENSE`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml_35/yaml/__init__.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml_35/yaml/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml_35/yaml/composer.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml_35/yaml/composer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml_35/yaml/constructor.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml_35/yaml/constructor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml_35/yaml/cyaml.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml_35/yaml/cyaml.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml_35/yaml/dumper.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml_35/yaml/dumper.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml_35/yaml/emitter.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml_35/yaml/emitter.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml_35/yaml/error.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml_35/yaml/error.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml_35/yaml/events.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml_35/yaml/events.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml_35/yaml/loader.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml_35/yaml/loader.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml_35/yaml/nodes.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml_35/yaml/nodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml_35/yaml/parser.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml_35/yaml/parser.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml_35/yaml/reader.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml_35/yaml/reader.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml_35/yaml/representer.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml_35/yaml/representer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml_35/yaml/resolver.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml_35/yaml/resolver.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml_35/yaml/scanner.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml_35/yaml/scanner.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml_35/yaml/serializer.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml_35/yaml/serializer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/yaml_35/yaml/tokens.py` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/yaml_35/yaml/tokens.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/zstd/LICENSE.txt` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/zstd/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/zstd/common/bitstream.h` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/zstd/common/bitstream.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/zstd/common/compiler.h` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/zstd/common/compiler.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/zstd/common/cpu.h` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/zstd/common/cpu.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/zstd/common/debug.h` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/zstd/common/debug.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/zstd/common/entropy_common.c` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/zstd/common/entropy_common.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/zstd/common/error_private.c` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/zstd/common/error_private.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/zstd/common/error_private.h` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/zstd/common/error_private.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/zstd/common/fse.h` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/zstd/common/fse.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/zstd/common/fse_decompress.c` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/zstd/common/fse_decompress.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/zstd/common/huf.h` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/zstd/common/huf.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/zstd/common/mem.h` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/zstd/common/mem.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/zstd/common/xxhash.c` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/zstd/common/xxhash.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/zstd/common/xxhash.h` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/zstd/common/xxhash.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/zstd/common/zstd_common.c` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/zstd/common/zstd_common.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/zstd/common/zstd_deps.h` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/zstd/common/zstd_deps.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/zstd/common/zstd_errors.h` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/zstd/common/zstd_errors.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/zstd/common/zstd_internal.h` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/zstd/common/zstd_internal.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/zstd/decompress/huf_decompress.c` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/zstd/decompress/huf_decompress.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.c` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.h` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/zstd/decompress/zstd_decompress.c` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/zstd/decompress/zstd_decompress.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.c` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.h` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_internal.h` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_internal.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/inline_copy/zstd/zstd.h` & `Nuitka-winsvc-1.7.6/nuitka/build/inline_copy/zstd/zstd.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/CompiledAsyncgenType.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/CompiledAsyncgenType.c`

 * *Files 1% similar despite different names*

```diff
@@ -308,34 +308,41 @@
         assert(exception_type == NULL);
         assert(exception_value == NULL);
         assert(exception_tb == NULL);
     }
 
     if (asyncgen->m_status == status_Unused && value != NULL && value != Py_None) {
         // No exception if value is given.
+        Py_XDECREF(value);
 
         SET_CURRENT_EXCEPTION_TYPE0_STR(PyExc_TypeError, "can't send non-None value to a just-started async generator");
         return PYGEN_ERROR;
     }
 
     if (asyncgen->m_status != status_Finished) {
         if (asyncgen->m_running) {
+            Py_XDECREF(value);
+
             SET_CURRENT_EXCEPTION_TYPE0_STR(PyExc_ValueError, "async generator already executing");
             return PYGEN_ERROR;
         }
 
         PyThreadState *thread_state = PyThreadState_GET();
 
         // Put the asyncgen back on the frame stack.
         Nuitka_ThreadStateFrameType *return_frame = _Nuitka_GetThreadStateFrame(thread_state);
 
         // Consider it as running.
         if (asyncgen->m_status == status_Unused) {
             asyncgen->m_status = status_Running;
             assert(asyncgen->m_resume_frame == NULL);
+
+            // Value will not be used, can only be Py_None or NULL.
+            Py_XDECREF(value);
+            value = NULL;
         } else {
             assert(asyncgen->m_resume_frame);
             pushFrameStackGenerator(asyncgen->m_resume_frame);
 
             asyncgen->m_resume_frame = NULL;
         }
 
@@ -363,15 +370,17 @@
 #endif
 
         PyObject *yielded;
 
         if (asyncgen->m_yieldfrom == NULL) {
             yielded = ((asyncgen_code)asyncgen->m_code)(asyncgen, value);
         } else {
+            // This does not release the value if any, so we need to do it afterwards.
             yielded = Nuitka_YieldFromAsyncgenInitial(asyncgen, value);
+            Py_XDECREF(value);
         }
 
         // If the asyncgen returns with m_yieldfrom set, it wants us to yield
         // from that value from now on.
         while (yielded == NULL && asyncgen->m_yieldfrom != NULL) {
             yielded = Nuitka_YieldFromAsyncgenNext(asyncgen);
         }
@@ -454,25 +463,27 @@
                 return PYGEN_ERROR;
             }
 
             return PYGEN_ERROR;
         } else {
             // For normal yield, wrap the result value before returning.
             if (asyncgen->m_yieldfrom == NULL) {
-                // TODO: Why not transfer ownership to constructor.
+                // Transferred ownership to constructor of Nuitka_AsyncgenValueWrapper
                 PyObject *wrapped = Nuitka_AsyncgenValueWrapper_New(yielded);
                 yielded = wrapped;
 
                 assert(yielded != NULL);
             }
 
             *result = yielded;
             return PYGEN_NEXT;
         }
     } else {
+        Py_XDECREF(value);
+
         // Release exception if any, we are finished with it and will raise another.
         Py_XDECREF(exception_type);
         Py_XDECREF(exception_value);
         Py_XDECREF(exception_tb);
 
         return PYGEN_RETURN;
     }
@@ -903,20 +914,21 @@
         return NULL;
     }
 
     return Nuitka_AsyncgenAthrow_New(asyncgen, args);
 }
 
 #if PYTHON_VERSION >= 0x3a0
-static PySendResult _Nuitka_Asyncgen_amsend(struct Nuitka_AsyncgenObject *asyncgen, PyObject *arg, PyObject **result) {
+static PySendResult _Nuitka_Asyncgen_am_send(struct Nuitka_AsyncgenObject *asyncgen, PyObject *arg, PyObject **result) {
 #if _DEBUG_ASYNCGEN
     PRINT_ASYNCGEN_STATUS("Enter", asyncgen);
 #endif
 
     *result = NULL;
+    Py_INCREF(arg);
     PySendResult res = _Nuitka_Asyncgen_sendR(asyncgen, arg, false, NULL, NULL, NULL, result);
 
 #if _DEBUG_ASYNCGEN
     PRINT_ASYNCGEN_STATUS("Leave", asyncgen);
     PRINT_COROUTINE_VALUE("result", *result);
     PRINT_NEW_LINE();
 #endif
@@ -1053,15 +1065,15 @@
 
 static PyAsyncMethods Nuitka_Asyncgen_as_async = {
     0,                               // am_await
     0,                               // am_aiter (PyObject_SelfIter)
     (unaryfunc)Nuitka_Asyncgen_anext // am_anext
 #if PYTHON_VERSION >= 0x3a0
     ,
-    (sendfunc)_Nuitka_Asyncgen_amsend // am_anext
+    (sendfunc)_Nuitka_Asyncgen_am_send // am_send
 #endif
 };
 
 // TODO: Set "__doc__" automatically for method clones of compiled types from
 // the documentation of built-in original type.
 static PyGetSetDef Nuitka_Asyncgen_getsetlist[] = {
     {(char *)"__name__", (getter)Nuitka_Asyncgen_get_name, (setter)Nuitka_Asyncgen_set_name, NULL},
@@ -1279,16 +1291,15 @@
 
 // Note: This expects a reference given in value, because that is the
 // only way we use it.
 static PyObject *Nuitka_AsyncgenValueWrapper_New(PyObject *value) {
     CHECK_OBJECT(value);
 
 #if _DEBUG_REFCOUNTS
-    count_active_Nuitka_AsyncgenValueWrapper_Type -= 1;
-    count_released_Nuitka_AsyncgenValueWrapper_Type += 1;
+    count_active_Nuitka_AsyncgenValueWrapper_Type += 1;
 #endif
 
     struct Nuitka_AsyncgenWrappedValueObject *result;
 
     allocateFromFreeListFixed(free_list_asyncgen_value_wrappers, struct Nuitka_AsyncgenWrappedValueObject,
                               Nuitka_AsyncgenValueWrapper_Type);
 
@@ -1488,22 +1499,21 @@
         PRINT_NEW_LINE();
 #endif
     }
 
 #if PYTHON_VERSION >= 0x380
     asyncgen_asend->m_gen->m_running_async = true;
 #endif
-    // TODO: Who releases arg.
-    // Py_INCREF(arg);
 
 #if _DEBUG_ASYNCGEN
     PRINT_STRING("Deferring to _Nuitka_Asyncgen_send\n");
     PRINT_NEW_LINE();
 #endif
 
+    Py_INCREF(arg);
     PyObject *result = _Nuitka_Asyncgen_send(asyncgen_asend->m_gen, arg, false, NULL, NULL, NULL);
 
 #if _DEBUG_ASYNCGEN
     PRINT_STRING("Returned from _Nuitka_Asyncgen_send\n");
     PRINT_COROUTINE_VALUE("result", result);
     PRINT_CURRENT_EXCEPTION();
 #endif
```

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/CompiledCellType.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/CompiledCellType.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/CompiledCodeHelpers.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/CompiledCodeHelpers.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/CompiledCoroutineType.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/CompiledCoroutineType.c`

 * *Files 1% similar despite different names*

```diff
@@ -211,30 +211,32 @@
     if (exception_type != NULL) {
         // Exception, was thrown into us, need to send that to sub-generator.
         // We acquired ownership of the published exception and need to release it potentially.
 
         // Transfer exception owner this.
         retval = _Nuitka_YieldFromPassExceptionTo(yieldfrom, exception_type, exception_value, exception_tb);
 
+        // TODO: This wants to look at retval most definitely, send_value is going to be NULL.
         if (unlikely(send_value == NULL)) {
             PyObject *error = GET_ERROR_OCCURRED();
 
             if (error != NULL && EXCEPTION_MATCH_BOOL_SINGLE(error, PyExc_StopIteration)) {
                 *returned_value = ERROR_GET_STOP_ITERATION_VALUE();
-
                 assert(!ERROR_OCCURRED());
+
                 return NULL;
             }
         }
     } else if (PyGen_CheckExact(yieldfrom) || PyCoro_CheckExact(yieldfrom)) {
         retval = Nuitka_PyGen_Send((PyGenObject *)yieldfrom, Py_None);
     } else if (send_value == Py_None && Nuitka_CoroutineWrapper_Check(yieldfrom)) {
         struct Nuitka_CoroutineObject *yieldfrom_coroutine =
             ((struct Nuitka_CoroutineWrapperObject *)yieldfrom)->m_coroutine;
 
+        Py_INCREF(Py_None);
         retval = _Nuitka_Coroutine_send(yieldfrom_coroutine, Py_None, mode ? false : true, NULL, NULL, NULL);
     } else if (send_value == Py_None && Py_TYPE(yieldfrom)->tp_iternext != NULL) {
         retval = Py_TYPE(yieldfrom)->tp_iternext(yieldfrom);
     } else {
 #if 0
         // TODO: Add slow mode traces.
         PRINT_ITEM(yieldfrom);
@@ -253,16 +255,17 @@
             *returned_value = Py_None;
         } else if (likely(EXCEPTION_MATCH_BOOL_SINGLE(error, PyExc_StopIteration))) {
             // The sub-generator has given an exception. In case of
             // StopIteration, we need to check the value, as it is going to be
             // the expression value of this "yield from", and we are done. All
             // other errors, we need to raise.
             *returned_value = ERROR_GET_STOP_ITERATION_VALUE();
-            assert(*returned_value != NULL);
             assert(!ERROR_OCCURRED());
+
+            assert(*returned_value != NULL);
         } else {
             *returned_value = NULL;
         }
 
         return NULL;
     } else {
         assert(!ERROR_OCCURRED());
@@ -388,43 +391,50 @@
     PRINT_COROUTINE_STRING("closing", closing ? "(closing) " : "(not closing) ");
     PRINT_COROUTINE_VALUE("value", value);
     PRINT_EXCEPTION(exception_type, exception_value, exception_tb);
     PRINT_CURRENT_EXCEPTION();
     PRINT_NEW_LINE();
 #endif
 
+    // Not both a value and an exception please.
     if (value != NULL) {
         assert(exception_type == NULL);
         assert(exception_value == NULL);
         assert(exception_tb == NULL);
     }
 
     if (coroutine->m_status == status_Unused && value != NULL && value != Py_None) {
         // No exception if value is given.
+        Py_XDECREF(value);
 
         SET_CURRENT_EXCEPTION_TYPE0_STR(PyExc_TypeError, "can't send non-None value to a just-started coroutine");
         return PYGEN_ERROR;
     }
 
     if (coroutine->m_status != status_Finished) {
         if (coroutine->m_running) {
+            Py_XDECREF(value);
+
             SET_CURRENT_EXCEPTION_TYPE0_STR(PyExc_ValueError, "coroutine already executing");
             return PYGEN_ERROR;
         }
 
         PyThreadState *thread_state = PyThreadState_GET();
 
         // Put the coroutine back on the frame stack.
         Nuitka_ThreadStateFrameType *return_frame = _Nuitka_GetThreadStateFrame(thread_state);
 
         // Consider it as running.
         if (coroutine->m_status == status_Unused) {
             coroutine->m_status = status_Running;
             assert(coroutine->m_resume_frame == NULL);
 
+            // Value will not be used, can only be Py_None or NULL.
+            Py_XDECREF(value);
+            value = NULL;
         } else {
             assert(coroutine->m_resume_frame);
             pushFrameStackGenerator(coroutine->m_resume_frame);
 
             coroutine->m_resume_frame = NULL;
         }
 
@@ -448,15 +458,17 @@
 #endif
 
         PyObject *yielded;
 
         if (coroutine->m_yieldfrom == NULL) {
             yielded = ((coroutine_code)coroutine->m_code)(coroutine, value);
         } else {
+            // This does not release the value if any, so we need to do it afterwards.
             yielded = Nuitka_YieldFromCoroutineInitial(coroutine, value);
+            Py_XDECREF(value);
         }
 
         // If the coroutine returns with m_yieldfrom set, it wants us to yield
         // from that value from now on.
         while (yielded == NULL && coroutine->m_yieldfrom != NULL) {
             yielded = Nuitka_YieldFromCoroutineNext(coroutine);
         }
@@ -564,14 +576,16 @@
                 return PYGEN_ERROR;
             }
         } else {
             *result = yielded;
             return PYGEN_NEXT;
         }
     } else {
+        Py_XDECREF(value);
+
         // Release exception if any, we are finished with it and will raise another.
         Py_XDECREF(exception_type);
         Py_XDECREF(exception_value);
         Py_XDECREF(exception_tb);
 
         /* This is for status_Finished */
         assert(coroutine->m_status == status_Finished);
@@ -632,16 +646,16 @@
     }
 }
 
 static PyObject *Nuitka_Coroutine_send(struct Nuitka_CoroutineObject *coroutine, PyObject *value) {
     CHECK_OBJECT(coroutine);
     CHECK_OBJECT(value);
 
-    // TODO: Does it release value ?
-    // Py_INCREF(value);
+    // We need to transfer ownership of the sent value.
+    Py_INCREF(value);
     PyObject *result = _Nuitka_Coroutine_send(coroutine, value, false, NULL, NULL, NULL);
 
     if (result == NULL) {
         if (GET_ERROR_OCCURRED() == NULL) {
             SET_CURRENT_EXCEPTION_TYPE0(PyExc_StopIteration);
         }
     }
@@ -850,14 +864,15 @@
 
 #if _DEBUG_COROUTINE
                 PRINT_COROUTINE_STATUS("Sending return value into ourselves", coroutine);
                 PRINT_COROUTINE_VALUE("value", val);
                 PRINT_NEW_LINE();
 #endif
 
+                // The ownership of val is transferred.
                 ret = _Nuitka_Coroutine_send(coroutine, val, false, NULL, NULL, NULL);
             } else {
 #if _DEBUG_COROUTINE
                 PRINT_COROUTINE_STATUS("Sending exception value into ourselves", coroutine);
                 PRINT_CURRENT_EXCEPTION();
                 PRINT_NEW_LINE();
 #endif
@@ -1049,20 +1064,22 @@
 
     Nuitka_GC_Track(result);
 
     return (PyObject *)result;
 }
 
 #if PYTHON_VERSION >= 0x3a0
-static PySendResult _Nuitka_Coroutine_amsend(struct Nuitka_CoroutineObject *coroutine, PyObject *arg,
-                                             PyObject **result) {
+static PySendResult _Nuitka_Coroutine_am_send(struct Nuitka_CoroutineObject *coroutine, PyObject *arg,
+                                              PyObject **result) {
 #if _DEBUG_COROUTINE
     PRINT_COROUTINE_STATUS("Enter", coroutine);
 #endif
 
+    // We need to transfer ownership of the sent value.
+    Py_INCREF(arg);
     PySendResult res = _Nuitka_Coroutine_sendR(coroutine, arg, false, NULL, NULL, NULL, result);
 
 #if _DEBUG_COROUTINE
     PRINT_COROUTINE_STATUS("Leave", coroutine);
     PRINT_COROUTINE_VALUE("result", *result);
     PRINT_NEW_LINE();
 #endif
@@ -1178,20 +1195,20 @@
 #if PYTHON_VERSION >= 0x370
     {(char *)"cr_origin", T_OBJECT, offsetof(struct Nuitka_CoroutineObject, m_origin), READONLY},
 
 #endif
     {NULL}};
 
 static PyAsyncMethods Nuitka_Coroutine_as_async = {
-    (unaryfunc)Nuitka_Coroutine_await, /* am_await */
-    0,                                 /* am_aiter */
-    0                                  /* am_anext */
+    (unaryfunc)Nuitka_Coroutine_await, // am_await
+    0,                                 // am_aiter
+    0                                  // am_anext
 #if PYTHON_VERSION >= 0x3a0
     ,
-    (sendfunc)_Nuitka_Coroutine_amsend /* am_send */
+    (sendfunc)_Nuitka_Coroutine_am_send // am_send
 #endif
 
 };
 
 PyTypeObject Nuitka_Coroutine_Type = {
     PyVarObject_HEAD_INIT(NULL, 0) "compiled_coroutine",                // tp_name
     sizeof(struct Nuitka_CoroutineObject),                              // tp_basicsize
@@ -1542,27 +1559,26 @@
 
                 SET_CURRENT_EXCEPTION_TYPE0_STR(PyExc_TypeError, "__await__() returned a coroutine");
 
                 return NULL;
             }
 
             if (unlikely(!HAS_ITERNEXT(result))) {
-                PyErr_Format(PyExc_TypeError, "__await__() returned non-iterator of type '%s'",
-                             Py_TYPE(result)->tp_name);
+                SET_CURRENT_EXCEPTION_TYPE_COMPLAINT("__await__() returned non-iterator of type '%s'", result);
 
                 Py_DECREF(result);
 
                 return NULL;
             }
         }
 
         return result;
     }
 
-    PyErr_Format(PyExc_TypeError, "object %s can't be used in 'await' expression", Py_TYPE(value)->tp_name);
+    SET_CURRENT_EXCEPTION_TYPE_COMPLAINT("object %s can't be used in 'await' expression", value);
 
     return NULL;
 }
 
 #if PYTHON_VERSION >= 0x366
 static void FORMAT_AWAIT_ERROR(PyObject *value, int await_kind) {
     CHECK_OBJECT(value);
@@ -1841,16 +1857,15 @@
     unaryfunc getter = NULL;
 
     if (Py_TYPE(value)->tp_as_async) {
         getter = Py_TYPE(value)->tp_as_async->am_anext;
     }
 
     if (unlikely(getter == NULL)) {
-        PyErr_Format(PyExc_TypeError, "'async for' requires an iterator with __anext__ method, got %s",
-                     Py_TYPE(value)->tp_name);
+        SET_CURRENT_EXCEPTION_TYPE_COMPLAINT("'async for' requires an iterator with __anext__ method, got %s", value);
 
         return NULL;
     }
 
     PyObject *next_value = (*getter)(value);
 
     if (unlikely(next_value == NULL)) {
```

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/CompiledFrameType.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/CompiledFrameType.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/CompiledFunctionType.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/CompiledFunctionType.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/CompiledGeneratorType.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/CompiledGeneratorType.c`

 * *Files 1% similar despite different names*

```diff
@@ -320,21 +320,22 @@
     FETCH_ERROR_OCCURRED(&exception_type, &exception_value, &exception_tb);
 
     // Exception, was thrown into us, need to send that to sub-generator.
     if (exception_type != NULL) {
         // Passing ownership of exception fetch to it.
         retval = _Nuitka_YieldFromPassExceptionTo(yieldfrom, exception_type, exception_value, exception_tb);
 
+        // TODO: This wants to look at retval most definitely, send_value is going to be NULL.
         if (unlikely(send_value == NULL)) {
             PyObject *error = GET_ERROR_OCCURRED();
 
             if (error != NULL && EXCEPTION_MATCH_BOOL_SINGLE(error, PyExc_StopIteration)) {
                 generator->m_returned = ERROR_GET_STOP_ITERATION_VALUE();
-
                 assert(!ERROR_OCCURRED());
+
                 return NULL;
             }
         }
     } else if (PyGen_CheckExact(yieldfrom)) {
         retval = Nuitka_PyGen_Send((PyGenObject *)yieldfrom, Py_None);
     }
 #if PYTHON_VERSION >= 0x350
@@ -476,14 +477,16 @@
         assert(exception_type == NULL);
         assert(exception_value == NULL);
         assert(exception_tb == NULL);
     }
 
     if (generator->m_status != status_Finished) {
         if (generator->m_running) {
+            Py_XDECREF(value);
+
             SET_CURRENT_EXCEPTION_TYPE0_STR(PyExc_ValueError, "generator already executing");
             return NULL;
         }
 
         PyThreadState *thread_state = PyThreadState_GET();
 
 #if PYTHON_VERSION < 0x300
@@ -501,14 +504,17 @@
 #endif
 
         // Put the asyncgen back on the frame stack.
         Nuitka_ThreadStateFrameType *return_frame = _Nuitka_GetThreadStateFrame(thread_state);
 
         if (generator->m_status == status_Unused) {
             generator->m_status = status_Running;
+
+            Py_XDECREF(value);
+            value = NULL;
         } else {
             // Put the generator back on the frame stack.
             pushFrameStackGeneratorCompiledFrame(generator->m_frame);
         }
 
         // Continue the yielder function while preventing recursion.
         Nuitka_MarkGeneratorAsRunning(generator);
@@ -531,15 +537,17 @@
 
         PyObject *yielded;
 
 #if PYTHON_VERSION >= 0x300
         if (generator->m_yieldfrom == NULL) {
             yielded = ((generator_code)generator->m_code)(generator, value);
         } else {
+            // This does not release the value if any, so we need to do it afterwards.
             yielded = Nuitka_YieldFromGeneratorInitial(generator, value);
+            Py_XDECREF(value);
         }
 #else
         yielded = ((generator_code)generator->m_code)(generator, value);
 #endif
 
 #if PYTHON_VERSION >= 0x300
         // If the generator returns with m_yieldfrom set, it wants us to yield
@@ -719,32 +727,36 @@
         Nuitka_MarkGeneratorAsFinished(generator);
 #endif
 
         SET_CURRENT_EXCEPTION_TYPE0_STR(PyExc_TypeError, "can't send non-None value to a just-started generator");
         return NULL;
     }
 
+    // We need to transfer ownership of the sent value.
+    Py_INCREF(value);
     PyObject *result = _Nuitka_Generator_send(generator, value, NULL, NULL, NULL);
 
     if (result == NULL) {
         if (GET_ERROR_OCCURRED() == NULL) {
             SET_CURRENT_EXCEPTION_TYPE0(PyExc_StopIteration);
         }
     }
 
     return result;
 }
 
 static PyObject *Nuitka_Generator_tp_iternext(struct Nuitka_GeneratorObject *generator) {
+    Py_INCREF(Py_None);
     return _Nuitka_Generator_send(generator, Py_None, NULL, NULL, NULL);
 }
 
 /* Our own qiter interface, which is for quicker simple loop style iteration,
    that does not send anything in. */
 PyObject *Nuitka_Generator_qiter(struct Nuitka_GeneratorObject *generator, bool *finished) {
+    Py_INCREF(Py_None);
     PyObject *result = _Nuitka_Generator_send(generator, Py_None, NULL, NULL, NULL);
 
     if (result == NULL) {
         if (unlikely(!CHECK_AND_CLEAR_STOP_ITERATION_OCCURRED())) {
             *finished = false;
             return NULL;
         }
@@ -1431,16 +1443,16 @@
 
 // This is only used.
 #if PYTHON_VERSION >= 0x3a0
 static PyAsyncMethods Nuitka_Generator_as_async = {
     NULL, /* am_await */
     NULL, /* am_aiter */
     NULL, /* am_anext */
-    // TODO: have this too, (sendfunc)_Nuitka_Generator_amsend
-    NULL /* am_anext */
+    // TODO: have this too, (sendfunc)_Nuitka_Generator_am_send
+    NULL /* am_send */
 };
 #endif
 
 #include <structmember.h>
 
 PyTypeObject Nuitka_Generator_Type = {
     PyVarObject_HEAD_INIT(NULL, 0) "compiled_generator", // tp_name
```

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/CompiledGeneratorTypeUncompiledIntegration.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/CompiledGeneratorTypeUncompiledIntegration.c`

 * *Files 0% similar despite different names*

```diff
@@ -683,15 +683,15 @@
             f->f_back = (PyFrameObject *)Py_NewRef(back);
         }
 
         frame->previous = NULL;
     }
 
     if (!_PyObject_GC_IS_TRACKED((PyObject *)f)) {
-        _PyObject_GC_TRACK((PyObject *)f);
+        Nuitka_GC_Track((PyObject *)f);
     }
 }
 
 // Cleanup up the frame is also not exported.
 static void _Nuitka_PyFrame_Clear(_PyInterpreterFrame *frame) {
     assert(frame->owner != FRAME_OWNED_BY_GENERATOR || _PyFrame_GetGenerator(frame)->gi_frame_state == FRAME_CLEARED);
```

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/CompiledMethodType.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/CompiledMethodType.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersAllocator.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersAllocator.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersAttributes.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersAttributes.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersBuiltin.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersBuiltin.c`

 * *Files 2% similar despite different names*

```diff
@@ -239,14 +239,33 @@
     char const *arg_names[] = {"file", "mode", "buffering", "encoding", "errors", "newline", "closefd", "opener"};
 
     return CALL_BUILTIN_KW_ARGS(NUITKA_ACCESS_BUILTIN(open), args, arg_names, 8);
 }
 
 #endif
 
+NUITKA_DEFINE_BUILTIN(input);
+
+PyObject *BUILTIN_INPUT(PyObject *prompt) {
+    NUITKA_ASSIGN_BUILTIN(input);
+
+#if NUITKA_STDERR_NOT_VISIBLE && (PYTHON_VERSION >= 0x300 || !defined(_WIN32))
+    if (prompt != NULL) {
+        PRINT_ITEM(prompt);
+        prompt = NULL;
+    }
+#endif
+
+    if (prompt == NULL) {
+        return CALL_FUNCTION_NO_ARGS(NUITKA_ACCESS_BUILTIN(input));
+    } else {
+        return CALL_FUNCTION_WITH_SINGLE_ARG(NUITKA_ACCESS_BUILTIN(input), prompt);
+    }
+}
+
 /** The "staticmethod" built-in.
  *
  **/
 
 NUITKA_DEFINE_BUILTIN(staticmethod)
 
 PyObject *BUILTIN_STATICMETHOD(PyObject *value) {
```

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersBuiltinTypeMethods.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersBuiltinTypeMethods.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersBytes.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersBytes.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersCalling.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersCalling.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersCallingGenerated.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersCallingGenerated.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersChecksumTools.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersChecksumTools.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersClasses.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersClasses.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersComparisonEq.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersComparisonEq.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersComparisonEqUtils.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersComparisonEqUtils.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersComparisonGe.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersComparisonGe.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersComparisonGt.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersComparisonGt.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersComparisonLe.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersComparisonLe.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersComparisonLt.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersComparisonLt.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersComparisonNe.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersComparisonNe.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersConstantsBlob.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersConstantsBlob.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersDeepcopy.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersDeepcopy.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersDictionaries.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersDictionaries.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersDictionariesGenerated.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersDictionariesGenerated.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersExceptions.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersExceptions.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersFiles.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersFiles.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersFilesystemPaths.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersFilesystemPaths.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersFloats.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersFloats.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersHeapStorage.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersHeapStorage.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersImport.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersImport.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersImportHard.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersImportHard.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersLists.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersLists.c`

 * *Files 0% similar despite different names*

```diff
@@ -330,15 +330,15 @@
 
     return false;
 }
 #endif
 
 bool LIST_APPEND1(PyObject *target, PyObject *item) {
 #if _NUITKA_EXPERIMENTAL_DISABLE_LIST_OPT
-    int res == PyList_Append(target, item);
+    int res = PyList_Append(target, item);
     Py_DECREF(item);
     return res == 0;
 #else
     CHECK_OBJECT(target);
     assert(PyList_CheckExact(target));
 
     CHECK_OBJECT(item);
@@ -358,15 +358,15 @@
 
     return true;
 #endif
 }
 
 bool LIST_APPEND0(PyObject *target, PyObject *item) {
 #if _NUITKA_EXPERIMENTAL_DISABLE_LIST_OPT
-    int res == PyList_Append(target, item);
+    int res = PyList_Append(target, item);
     return res == 0;
 #else
     CHECK_OBJECT(target);
     assert(PyList_CheckExact(target));
 
     CHECK_OBJECT(item);
```

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersListsGenerated.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersListsGenerated.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersMappings.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersMappings.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersMatching.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersMatching.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersOperationBinaryAdd.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersOperationBinaryAdd.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersOperationBinaryAddUtils.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersOperationBinaryAddUtils.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersOperationBinaryBitand.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersOperationBinaryBitand.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersOperationBinaryBitor.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersOperationBinaryBitor.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersOperationBinaryBitxor.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersOperationBinaryBitxor.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersOperationBinaryDivmod.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersOperationBinaryDivmod.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersOperationBinaryDivmodUtils.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersOperationBinaryDivmodUtils.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersOperationBinaryFloordiv.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersOperationBinaryFloordiv.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersOperationBinaryInplaceAdd.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersOperationBinaryInplaceAdd.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersOperationBinaryLshift.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersOperationBinaryLshift.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersOperationBinaryMatmult.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersOperationBinaryMatmult.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersOperationBinaryMod.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersOperationBinaryMod.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersOperationBinaryMult.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersOperationBinaryMult.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersOperationBinaryMultUtils.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersOperationBinaryMultUtils.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersOperationBinaryOlddiv.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersOperationBinaryOlddiv.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersOperationBinaryPow.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersOperationBinaryPow.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersOperationBinaryPowUtils.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersOperationBinaryPowUtils.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersOperationBinaryRshift.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersOperationBinaryRshift.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersOperationBinarySub.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersOperationBinarySub.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersOperationBinaryTruediv.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersOperationBinaryTruediv.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersOperationInplaceAdd.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersOperationInplaceAdd.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersOperationInplaceAddUtils.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersOperationInplaceAddUtils.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersOperationInplaceBitand.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersOperationInplaceBitand.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersOperationInplaceBitor.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersOperationInplaceBitor.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersOperationInplaceBitxor.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersOperationInplaceBitxor.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersOperationInplaceFloordiv.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersOperationInplaceFloordiv.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersOperationInplaceLshift.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersOperationInplaceLshift.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersOperationInplaceMatmult.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersOperationInplaceMatmult.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersOperationInplaceMod.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersOperationInplaceMod.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersOperationInplaceMult.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersOperationInplaceMult.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersOperationInplaceOlddiv.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersOperationInplaceOlddiv.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersOperationInplacePow.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersOperationInplacePow.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersOperationInplaceRshift.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersOperationInplaceRshift.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersOperationInplaceSub.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersOperationInplaceSub.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersOperationInplaceTruediv.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersOperationInplaceTruediv.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersProfiling.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersProfiling.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersPythonPgo.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersPythonPgo.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersRaising.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersRaising.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersSafeStrings.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersSafeStrings.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersSequences.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersSequences.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersSlices.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersSlices.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersStrings.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersStrings.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersTuples.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersTuples.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/HelpersTypes.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/HelpersTypes.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/InspectPatcher.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/InspectPatcher.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/MainProgram.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/MainProgram.c`

 * *Files 0% similar despite different names*

```diff
@@ -328,15 +328,55 @@
     setlocale(LC_ALL, old_locale);
     free(old_locale);
 
     return argv_copy;
 }
 #endif
 
+#if _DEBUG_REFCOUNTS
+static void PRINT_REFCOUNTS(void) {
+    // spell-checker: ignore Asend, Athrow
+
+    PRINT_STRING("REFERENCE counts at program end:\n");
+    PRINT_STRING("active | allocated | released\n");
+#if PYTHON_VERSION >= 0x350
+    PRINT_FORMAT("Compiled Coroutines: %d | %d | %d\n", count_active_Nuitka_Coroutine_Type,
+                 count_allocated_Nuitka_Coroutine_Type, count_released_Nuitka_Coroutine_Type);
+    PRINT_FORMAT("Compiled Coroutines Wrappers: %d | %d | %d\n", count_active_Nuitka_CoroutineWrapper_Type,
+                 count_allocated_Nuitka_CoroutineWrapper_Type, count_released_Nuitka_CoroutineWrapper_Type);
+
+    PRINT_FORMAT("Compiled Coroutines AIter Wrappers: %d | %d | %d\n", count_active_Nuitka_AIterWrapper_Type,
+                 count_allocated_Nuitka_AIterWrapper_Type, count_released_Nuitka_AIterWrapper_Type);
+#endif
+#if PYTHON_VERSION >= 0x360
+    PRINT_FORMAT("Compiled Asyncgen: %d | %d | %d\n", count_active_Nuitka_Asyncgen_Type,
+                 count_allocated_Nuitka_Asyncgen_Type, count_released_Nuitka_Asyncgen_Type);
+    PRINT_FORMAT("Compiled Asyncgen Wrappers: %d | %d | %d\n", count_active_Nuitka_AsyncgenValueWrapper_Type,
+                 count_allocated_Nuitka_AsyncgenValueWrapper_Type, count_released_Nuitka_AsyncgenValueWrapper_Type);
+    PRINT_FORMAT("Compiled Asyncgen Asend: %d | %d | %d\n", count_active_Nuitka_AsyncgenAsend_Type,
+                 count_allocated_Nuitka_AsyncgenAsend_Type, count_released_Nuitka_AsyncgenAsend_Type);
+    PRINT_FORMAT("Compiled Asyncgen Athrow: %d | %d | %d\n", count_active_Nuitka_AsyncgenAthrow_Type,
+                 count_allocated_Nuitka_AsyncgenAthrow_Type, count_released_Nuitka_AsyncgenAthrow_Type);
+#endif
+
+    PRINT_FORMAT("Compiled Frames: %d | %d | %d (cache usage may occur)\n", count_active_Nuitka_Frame_Type,
+                 count_allocated_Nuitka_Frame_Type, count_released_Nuitka_Frame_Type);
+    PRINT_STRING("CACHED counts at program end:\n");
+    PRINT_STRING("active | allocated | released | hits\n");
+    PRINT_FORMAT("Cached Frames: %d | %d | %d | %d\n", count_active_frame_cache_instances,
+                 count_allocated_frame_cache_instances, count_released_frame_cache_instances,
+                 count_hit_frame_cache_instances);
+}
+#endif
+
 static int HANDLE_PROGRAM_EXIT(void) {
+#if _DEBUG_REFCOUNTS
+    PRINT_REFCOUNTS();
+#endif
+
     int exit_code;
 
     PyThreadState *thread_state = PyThreadState_GET();
 
     if (HAS_ERROR_OCCURRED(thread_state)) {
 #if PYTHON_VERSION >= 0x300
         /* Remove the frozen importlib traceback part, which would not be compatible. */
@@ -476,48 +516,14 @@
                 }
             }
 #endif
         }
     }
 }
 
-#if _DEBUG_REFCOUNTS
-static void PRINT_REFCOUNTS(void) {
-    PRINT_STRING("REFERENCE counts at program end:\n");
-    PRINT_STRING("active | allocated | released\n");
-#if PYTHON_VERSION >= 0x350
-    PRINT_FORMAT("Compiled Coroutines: %d | %d | %d\n", count_active_Nuitka_Coroutine_Type,
-                 count_allocated_Nuitka_Coroutine_Type, count_released_Nuitka_Coroutine_Type);
-    PRINT_FORMAT("Compiled Coroutines Wrappers: %d | %d | %d\n", count_active_Nuitka_CoroutineWrapper_Type,
-                 count_allocated_Nuitka_CoroutineWrapper_Type, count_released_Nuitka_CoroutineWrapper_Type);
-
-    PRINT_FORMAT("Compiled Coroutines AIter Wrappers: %d | %d | %d\n", count_active_Nuitka_AIterWrapper_Type,
-                 count_allocated_Nuitka_AIterWrapper_Type, count_released_Nuitka_AIterWrapper_Type);
-#endif
-#if PYTHON_VERSION >= 0x360
-    PRINT_FORMAT("Compiled Asyncgen: %d | %d | %d\n", count_active_Nuitka_Asyncgen_Type,
-                 count_allocated_Nuitka_Asyncgen_Type, count_released_Nuitka_Asyncgen_Type);
-    PRINT_FORMAT("Compiled Asyncgen Wrappers: %d | %d | %d\n", count_active_Nuitka_AsyncgenValueWrapper_Type,
-                 count_allocated_Nuitka_AsyncgenValueWrapper_Type, count_released_Nuitka_AsyncgenValueWrapper_Type);
-    PRINT_FORMAT("Compiled Asyncgen Asend: %d | %d | %d\n", count_active_Nuitka_AsyncgenAsend_Type,
-                 count_allocated_Nuitka_AsyncgenAsend_Type, count_released_Nuitka_AsyncgenAsend_Type);
-    PRINT_FORMAT("Compiled Asyncgen Athrow: %d | %d | %d\n", count_active_Nuitka_AsyncgenAthrow_Type,
-                 count_allocated_Nuitka_AsyncgenAthrow_Type, count_released_Nuitka_AsyncgenAthrow_Type);
-#endif
-
-    PRINT_FORMAT("Compiled Frames: %d | %d | %d (cache usage may occur)\n", count_active_Nuitka_Frame_Type,
-                 count_allocated_Nuitka_Frame_Type, count_released_Nuitka_Frame_Type);
-    PRINT_STRING("CACHED counts at program end:\n");
-    PRINT_STRING("active | allocated | released | hits\n");
-    PRINT_FORMAT("Cached Frames: %d | %d | %d | %d\n", count_active_frame_cache_instances,
-                 count_allocated_frame_cache_instances, count_released_frame_cache_instances,
-                 count_hit_frame_cache_instances);
-}
-#endif
-
 #if defined(_NUITKA_ONEFILE_MODE) && defined(_WIN32)
 
 static long onefile_ppid;
 
 DWORD WINAPI doOnefileParentMonitoring(LPVOID lpParam) {
     NUITKA_PRINT_TRACE("Onefile parent monitoring starts.");
 
@@ -1562,18 +1568,14 @@
     checkModuleConstants___main__();
 #endif
 
 #endif
 
     int exit_code = HANDLE_PROGRAM_EXIT();
 
-#if _DEBUG_REFCOUNTS
-    PRINT_REFCOUNTS();
-#endif
-
     NUITKA_PRINT_TIMING("main(): Calling Py_Exit.");
     Py_Exit(exit_code);
 
     // The "Py_Exit()" calls is not supposed to return.
     NUITKA_CANNOT_GET_HERE("Py_Exit does not return");
 }
```

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/MetaPathBasedLoader.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/MetaPathBasedLoader.c`

 * *Files 0% similar despite different names*

```diff
@@ -1375,15 +1375,21 @@
         basename = entry->name;
     } else {
         basename += 1;
     }
 
     copyStringSafe(filename_buffer, basename, sizeof(filename_buffer));
 
-    if ((entry->flags & NUITKA_PACKAGE_FLAG) != 0) {
+    if ((entry->flags & NUITKA_EXTENSION_MODULE_FLAG) != 0) {
+#if defined(_WIN32)
+        appendStringSafe(filename_buffer, ".pyd", sizeof(filename_buffer));
+#else
+        appendStringSafe(filename_buffer, ".so", sizeof(filename_buffer));
+#endif
+    } else if ((entry->flags & NUITKA_PACKAGE_FLAG) != 0) {
         appendCharSafe(filename_buffer, SEP, sizeof(filename_buffer));
         appendStringSafe(filename_buffer, "__init__.py", sizeof(filename_buffer));
     } else {
         appendStringSafe(filename_buffer, ".py", sizeof(filename_buffer));
     }
 
     PyObject *module_filename = Nuitka_String_FromString(filename_buffer);
```

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/MetaPathBasedLoaderImportlibMetadataDistribution.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/MetaPathBasedLoaderImportlibMetadataDistribution.c`

 * *Files 2% similar despite different names*

```diff
@@ -42,17 +42,17 @@
     static PyObject *importlib_metadata_distribution = NULL;
     // TODO: Use pathlib.Path for "locate_file" result should be more compatible.
 
     if (nuitka_distribution_type == NULL) {
         static char const *nuitka_distribution_code = "\n\
 import os,sys\n\
 if sys.version_info >= (3, 8):\n\
-    from importlib.metadata import Distribution,distribution,EntryPoints\n\
+    from importlib.metadata import Distribution,distribution\n\
 else:\n\
-    from importlib_metadata import Distribution,distribution,EntryPoints\n\
+    from importlib_metadata import Distribution,distribution\n\
 class nuitka_distribution(Distribution):\n\
     def __init__(self, base_path, metadata, entry_points):\n\
         self.base_path = base_path; self.metadata_data = metadata\n\
         self.entry_points_data = entry_points\n\
     def read_text(self, filename):\n\
         if filename == 'METADATA':\n\
             return self.metadata_data\n\
```

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/MetaPathBasedLoaderResourceReader.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/MetaPathBasedLoaderResourceReader.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/MetaPathBasedLoaderResourceReaderFiles.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/MetaPathBasedLoaderResourceReaderFiles.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/OnefileBootstrap.c` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/OnefileBootstrap.c`

 * *Files 0% similar despite different names*

```diff
@@ -838,15 +838,15 @@
         FORMAT_MESSAGE_FROM_SYSTEM |
         FORMAT_MESSAGE_IGNORE_INSERTS,
         NULL,
         errorCode,
         MAKELANGID(LANG_ENGLISH, SUBLANG_ENGLISH_US),
         (LPWSTR)&errorMessage,
         0, NULL);
-    wprintf(L"%LS failed (%d): %LS", fnName, errorCode, errorMessage);
+    wprintf(L"%ls failed (%d): %ls", fnName, errorCode, errorMessage);
     LocalFree(errorMessage);
     return errorCode;
 }
 
 DWORD SvcInstall(LPCWSTR cmdLine)
 {
     SC_HANDLE scManagerHandle = OpenSCManagerW(NULL, NULL, SC_MANAGER_ALL_ACCESS);
```

### Comparing `Nuitka-winsvc-1.7.5/nuitka/build/static_src/OnefileSplashScreen.cpp` & `Nuitka-winsvc-1.7.6/nuitka/build/static_src/OnefileSplashScreen.cpp`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/AsyncgenCodes.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/AsyncgenCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/AttributeCodes.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/AttributeCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/BinaryOperationHelperDefinitions.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/BinaryOperationHelperDefinitions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/BranchCodes.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/BranchCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/BuiltinCodes.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/BuiltinCodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,14 +118,28 @@
             emit=emit,
             context=context,
         )
 
         context.addCleanupTempName(value_name)
 
 
+def generateBuiltinInputCode(to_name, expression, emit, context):
+    generateCAPIObjectCode(
+        to_name=to_name,
+        capi="BUILTIN_INPUT",
+        arg_desc=(("input_arg", expression.subnode_prompt),),
+        may_raise=expression.mayRaiseExceptionOperation(),
+        conversion_check=decideConversionCheckNeeded(to_name, expression),
+        none_null=True,
+        source_ref=expression.getCompatibleSourceReference(),
+        emit=emit,
+        context=context,
+    )
+
+
 def generateBuiltinOpenCode(to_name, expression, emit, context):
     arg_desc = (
         ("open_filename", expression.subnode_filename),
         ("open_mode", expression.subnode_mode),
         ("open_buffering", expression.subnode_buffering),
     )
```

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/CallCodes.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/CallCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/ClassCodes.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/ClassCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/CodeGeneration.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/CodeGeneration.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,15 @@
     generateBuiltinBytearray1Code,
     generateBuiltinBytearray3Code,
     generateBuiltinClassmethodCode,
     generateBuiltinComplex1Code,
     generateBuiltinComplex2Code,
     generateBuiltinFloatCode,
     generateBuiltinHexCode,
+    generateBuiltinInputCode,
     generateBuiltinOctCode,
     generateBuiltinOpenCode,
     generateBuiltinRange1Code,
     generateBuiltinRange2Code,
     generateBuiltinRange3Code,
     generateBuiltinRefCode,
     generateBuiltinStaticmethodCode,
@@ -662,14 +663,15 @@
         "EXPRESSION_MATCH_TYPE_CHECK_SEQUENCE": generateMatchTypeCheckSequenceCode,
         "EXPRESSION_MATCH_TYPE_CHECK_MAPPING": generateMatchTypeCheckMappingCode,
         "EXPRESSION_BUILTIN_DIR1": generateBuiltinDir1Code,
         "EXPRESSION_BUILTIN_VARS": generateBuiltinVarsCode,
         "EXPRESSION_BUILTIN_HASATTR": generateBuiltinHasattrCode,
         "EXPRESSION_BUILTIN_GETATTR": generateBuiltinGetattrCode,
         "EXPRESSION_BUILTIN_SETATTR": generateBuiltinSetattrCode,
+        "EXPRESSION_BUILTIN_INPUT": generateBuiltinInputCode,
         "EXPRESSION_BUILTIN_OPEN_P2": generateBuiltinOpenCode,
         "EXPRESSION_BUILTIN_OPEN_P3": generateBuiltinOpenCode,
         "EXPRESSION_BUILTIN_STATICMETHOD": generateBuiltinStaticmethodCode,
         "EXPRESSION_BUILTIN_CLASSMETHOD": generateBuiltinClassmethodCode,
         "EXPRESSION_BUILTIN_RANGE1": generateBuiltinRange1Code,
         "EXPRESSION_BUILTIN_RANGE2": generateBuiltinRange2Code,
         "EXPRESSION_BUILTIN_RANGE3": generateBuiltinRange3Code,
```

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/CodeHelperSelection.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/CodeHelperSelection.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/CodeHelpers.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/CodeHelpers.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/CodeObjectCodes.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/CodeObjectCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/ComparisonCodes.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/ComparisonCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/ComparisonHelperDefinitions.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/ComparisonHelperDefinitions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/ConditionalCodes.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/ConditionalCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/ConstantCodes.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/ConstantCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/Contexts.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/Contexts.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/CoroutineCodes.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/CoroutineCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/CtypesCodes.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/CtypesCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/DictCodes.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/DictCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/Emission.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/Emission.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/ErrorCodes.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/ErrorCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/EvalCodes.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/EvalCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/ExceptionCodes.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/ExceptionCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/ExpressionCTypeSelectionHelpers.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/ExpressionCTypeSelectionHelpers.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/ExpressionCodes.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/ExpressionCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/FrameCodes.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/FrameCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/FunctionCodes.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/FunctionCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/GeneratorCodes.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/GeneratorCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/GlobalConstants.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/GlobalConstants.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/GlobalsLocalsCodes.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/GlobalsLocalsCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/IdCodes.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/IdCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/ImportCodes.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/ImportCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/Indentation.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/Indentation.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/IndexCodes.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/IndexCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/InjectCCodes.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/InjectCCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/IntegerCodes.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/IntegerCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/IteratorCodes.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/IteratorCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/LabelCodes.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/LabelCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/LineNumberCodes.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/LineNumberCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/ListCodes.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/ListCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/LoaderCodes.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/LoaderCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/LocalsDictCodes.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/LocalsDictCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/LoopCodes.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/LoopCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/MatchCodes.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/MatchCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/ModuleCodes.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/ModuleCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/Namify.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/Namify.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/OperationCodes.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/OperationCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/PackageResourceCodes.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/PackageResourceCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/PrintCodes.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/PrintCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/PythonAPICodes.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/PythonAPICodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/RaisingCodes.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/RaisingCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/Reports.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/Reports.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/ReturnCodes.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/ReturnCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/SetCodes.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/SetCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/SliceCodes.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/SliceCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/StringCodes.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/StringCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/SubscriptCodes.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/SubscriptCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/TryCodes.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/TryCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/TupleCodes.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/TupleCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/VariableCodes.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/VariableCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/VariableDeclarations.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/VariableDeclarations.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/YieldCodes.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/YieldCodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,16 +115,17 @@
 
     yield_return_name = VariableDeclaration(
         "PyObject *", "yield_return_value", None, None
     )
 
     getErrorExitCode(check_name=yield_return_name, emit=emit, context=context)
 
-    # Called with object
+    # Called with object, so we can simply do this.
     emit("%s = %s;" % (to_name, yield_return_name))
+    context.addCleanupTempName(to_name)
 
 
 def generateYieldCode(to_name, expression, emit, context):
     (value_name,) = generateChildExpressionsCode(
         expression=expression, emit=emit, context=context
     )
 
@@ -189,16 +190,14 @@
             yield_code=yield_code,
             resume_code=None,
             preserve_exception=preserve_exception,
             emit=emit,
             context=context,
         )
 
-        context.addCleanupTempName(result_name)
-
 
 def generateYieldFromWaitableCode(to_name, expression, emit, context):
 
     # In handlers, we must preserve/restore the exception.
     preserve_exception = expression.isExceptionPreserving()
 
     (awaited_name,) = generateChildExpressionsCode(
@@ -233,20 +232,14 @@
             yield_code=yield_code,
             resume_code=resume_code,
             preserve_exception=preserve_exception,
             emit=emit,
             context=context,
         )
 
-        # TODO: Seems to be redundant with and _getYieldPreserveCode doing
-        # it and could be removed
-        getErrorExitCode(check_name=result_name, emit=emit, context=context)
-
-        context.addCleanupTempName(result_name)
-
 
 def getYieldReturnDispatchCode(context):
     function_dispatch = [
         "case %(index)d: goto yield_return_%(index)d;" % {"index": yield_index}
         for yield_index in range(context.getLabelCount("yield_return"), 0, -1)
     ]
```

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/__init__.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/c_types/CTypeBases.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/c_types/CTypeBases.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/c_types/CTypeBooleans.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/c_types/CTypeBooleans.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/c_types/CTypeCFloats.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/c_types/CTypeCFloats.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/c_types/CTypeCLongs.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/c_types/CTypeCLongs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/c_types/CTypeModuleDictVariables.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/c_types/CTypeModuleDictVariables.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/c_types/CTypeNuitkaBooleans.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/c_types/CTypeNuitkaBooleans.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/c_types/CTypeNuitkaInts.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/c_types/CTypeNuitkaInts.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/c_types/CTypeNuitkaVoids.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/c_types/CTypeNuitkaVoids.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/c_types/CTypePyObjectPointers.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/c_types/CTypePyObjectPointers.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/c_types/CTypeVoids.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/c_types/CTypeVoids.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/c_types/__init__.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/c_types/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/templates/CodeTemplatesAsyncgens.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/templates/CodeTemplatesAsyncgens.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 %(function_local_types)s
 };
 #endif
 
 static PyObject *%(function_identifier)s_context(struct Nuitka_AsyncgenObject *asyncgen, PyObject *yield_return_value) {
     CHECK_OBJECT(asyncgen);
     assert(Nuitka_Asyncgen_Check((PyObject *)asyncgen));
+    CHECK_OBJECT_X(yield_return_value);
 
 #if %(has_heap_declaration)s
     // Heap access.
 %(heap_declaration)s
 #endif
 
     // Dispatch to yield based on return label index:
```

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/templates/CodeTemplatesConstants.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/templates/CodeTemplatesConstants.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/templates/CodeTemplatesCoroutines.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/templates/CodeTemplatesCoroutines.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 %(function_local_types)s
 };
 #endif
 
 static PyObject *%(function_identifier)s_context(struct Nuitka_CoroutineObject *coroutine, PyObject *yield_return_value) {
     CHECK_OBJECT(coroutine);
     assert(Nuitka_Coroutine_Check((PyObject *)coroutine));
+    CHECK_OBJECT_X(yield_return_value);
 
 #if %(has_heap_declaration)s
     // Heap access.
 %(heap_declaration)s
 #endif
 
     // Dispatch to yield based on return label index:
```

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/templates/CodeTemplatesExceptions.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/templates/CodeTemplatesExceptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/templates/CodeTemplatesFrames.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/templates/CodeTemplatesFrames.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/templates/CodeTemplatesFunction.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/templates/CodeTemplatesFunction.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/templates/CodeTemplatesGeneratorFunction.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/templates/CodeTemplatesGeneratorFunction.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/templates/CodeTemplatesIterators.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/templates/CodeTemplatesIterators.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/templates/CodeTemplatesLoader.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/templates/CodeTemplatesLoader.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/templates/CodeTemplatesModules.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/templates/CodeTemplatesModules.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/templates/CodeTemplatesVariables.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/templates/CodeTemplatesVariables.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/templates/TemplateDebugWrapper.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/templates/TemplateDebugWrapper.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/templates/__init__.py` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/templates_c/CodeTemplateCallsMethodPositional.c.j2` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/templates_c/CodeTemplateCallsMethodPositional.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/templates_c/CodeTemplateCallsMixed.c.j2` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/templates_c/CodeTemplateCallsMixed.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/templates_c/CodeTemplateCallsPositional.c.j2` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/templates_c/CodeTemplateCallsPositional.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/templates_c/CodeTemplateCallsPositionalMethodDescr.c.j2` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/templates_c/CodeTemplateCallsPositionalMethodDescr.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/templates_c/CodeTemplateMakeListHinted.c.j2` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/templates_c/CodeTemplateMakeListHinted.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/templates_c/CodeTemplateMakeListSmall.c.j2` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/templates_c/CodeTemplateMakeListSmall.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/templates_c/HelperBuiltinMethodOperation.c.j2` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/templates_c/HelperBuiltinMethodOperation.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/templates_c/HelperDictionaryCopy.c.j2` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/templates_c/HelperDictionaryCopy.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/templates_c/HelperImportHard.c.j2` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/templates_c/HelperImportHard.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/templates_c/HelperLongTools.c.j2` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/templates_c/HelperLongTools.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/templates_c/HelperObjectTools.c.j2` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/templates_c/HelperObjectTools.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/templates_c/HelperOperationBinary.c.j2` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/templates_c/HelperOperationBinary.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/templates_c/HelperOperationComparison.c.j2` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/templates_c/HelperOperationComparison.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/templates_c/HelperOperationComparisonBytes.c.j2` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/templates_c/HelperOperationComparisonBytes.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/templates_c/HelperOperationComparisonFloat.c.j2` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/templates_c/HelperOperationComparisonFloat.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/templates_c/HelperOperationComparisonInt.c.j2` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/templates_c/HelperOperationComparisonInt.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/templates_c/HelperOperationComparisonList.c.j2` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/templates_c/HelperOperationComparisonList.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/templates_c/HelperOperationComparisonLong.c.j2` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/templates_c/HelperOperationComparisonLong.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/templates_c/HelperOperationComparisonStr.c.j2` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/templates_c/HelperOperationComparisonStr.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/templates_c/HelperOperationComparisonTuple.c.j2` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/templates_c/HelperOperationComparisonTuple.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/templates_c/HelperOperationComparisonUnicode.c.j2` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/templates_c/HelperOperationComparisonUnicode.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/templates_c/HelperOperationInplace.c.j2` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/templates_c/HelperOperationInplace.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/templates_c/HelperSlotsBinary.c.j2` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/templates_c/HelperSlotsBinary.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/templates_c/HelperSlotsBytes.c.j2` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/templates_c/HelperSlotsBytes.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/templates_c/HelperSlotsCommon.c.j2` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/templates_c/HelperSlotsCommon.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/templates_c/HelperSlotsFloat.c.j2` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/templates_c/HelperSlotsFloat.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/templates_c/HelperSlotsInt.c.j2` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/templates_c/HelperSlotsInt.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/templates_c/HelperSlotsList.c.j2` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/templates_c/HelperSlotsList.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/templates_c/HelperSlotsLong.c.j2` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/templates_c/HelperSlotsLong.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/templates_c/HelperSlotsSet.c.j2` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/templates_c/HelperSlotsSet.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/templates_c/HelperSlotsStr.c.j2` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/templates_c/HelperSlotsStr.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/templates_c/HelperSlotsTuple.c.j2` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/templates_c/HelperSlotsTuple.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/code_generation/templates_c/HelperSlotsUnicode.c.j2` & `Nuitka-winsvc-1.7.6/nuitka/code_generation/templates_c/HelperSlotsUnicode.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/containers/Namedtuples.py` & `Nuitka-winsvc-1.7.6/nuitka/containers/Namedtuples.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/containers/OrderedDicts.py` & `Nuitka-winsvc-1.7.6/nuitka/containers/OrderedDicts.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/containers/OrderedSets.py` & `Nuitka-winsvc-1.7.6/nuitka/containers/OrderedSets.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/containers/OrderedSetsFallback.py` & `Nuitka-winsvc-1.7.6/nuitka/containers/OrderedSetsFallback.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/containers/__init__.py` & `Nuitka-winsvc-1.7.6/nuitka/containers/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/distutils/Build.py` & `Nuitka-winsvc-1.7.6/nuitka/distutils/Build.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/distutils/DistutilCommands.py` & `Nuitka-winsvc-1.7.6/nuitka/distutils/DistutilCommands.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/distutils/__init__.py` & `Nuitka-winsvc-1.7.6/nuitka/distutils/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/finalizations/Finalization.py` & `Nuitka-winsvc-1.7.6/nuitka/finalizations/Finalization.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/finalizations/FinalizeMarkups.py` & `Nuitka-winsvc-1.7.6/nuitka/finalizations/FinalizeMarkups.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/finalizations/__init__.py` & `Nuitka-winsvc-1.7.6/nuitka/finalizations/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/freezer/DependsExe.py` & `Nuitka-winsvc-1.7.6/nuitka/freezer/DependsExe.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/freezer/DllDependenciesCommon.py` & `Nuitka-winsvc-1.7.6/nuitka/freezer/DllDependenciesCommon.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/freezer/DllDependenciesMacOS.py` & `Nuitka-winsvc-1.7.6/nuitka/freezer/DllDependenciesMacOS.py`

 * *Files 3% similar despite different names*

```diff
@@ -183,14 +183,25 @@
                 candidate = os.path.join(library_dir, path)
                 if os.path.exists(candidate):
                     resolved_path = os.path.normpath(candidate)
                     break
         else:
             resolved_path = path
 
+        # Some extension modules seem to reference themselves a wrong name,
+        # duplicating their module name into the filename, but that does
+        # not exist.
+        if not os.path.exists(resolved_path) and package_name is not None:
+            parts = os.path.basename(resolved_path).split(".")
+
+            if parts[0] == package_name.asString():
+                resolved_path = os.path.join(
+                    os.path.dirname(resolved_path), ".".join(parts[1:])
+                )
+
         # Some extension modules seem to reference themselves by a different
         # extension module name, so use that if it exists.
         if not os.path.exists(resolved_path) and python_version >= 0x300:
             so_suffixes = getSharedLibrarySuffixes()[:-1]
 
             specific_suffix = so_suffixes[0]
             abi_suffix = so_suffixes[1]
```

### Comparing `Nuitka-winsvc-1.7.5/nuitka/freezer/DllDependenciesPosix.py` & `Nuitka-winsvc-1.7.6/nuitka/freezer/DllDependenciesPosix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/freezer/DllDependenciesWin32.py` & `Nuitka-winsvc-1.7.6/nuitka/freezer/DllDependenciesWin32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/freezer/IncludedDataFiles.py` & `Nuitka-winsvc-1.7.6/nuitka/freezer/IncludedDataFiles.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/freezer/IncludedEntryPoints.py` & `Nuitka-winsvc-1.7.6/nuitka/freezer/IncludedEntryPoints.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/freezer/Onefile.py` & `Nuitka-winsvc-1.7.6/nuitka/freezer/Onefile.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,16 +44,22 @@
 from nuitka.utils.FileOperations import (
     areSamePaths,
     getExternalUsePath,
     getFileContents,
     removeDirectory,
 )
 from nuitka.utils.InstalledPythons import findInstalledPython
+from nuitka.utils.SharedLibraries import cleanupHeaderForAndroid
 from nuitka.utils.Signing import addMacOSCodeSignature
-from nuitka.utils.Utils import isMacOS, isWin32OrPosixWindows, isWin32Windows
+from nuitka.utils.Utils import (
+    isAndroidBasedLinux,
+    isMacOS,
+    isWin32OrPosixWindows,
+    isWin32Windows,
+)
 from nuitka.utils.WindowsResources import RT_RCDATA, addResourceToFile
 
 
 def packDistFolderToOnefile(dist_dir):
     """Pack distribution to onefile, i.e. a single file that is directly executable."""
 
     onefile_output_filename = getResultFullpath(onefile=True)
@@ -167,14 +173,15 @@
         attachOnefilePayload(
             dist_dir=dist_dir,
             onefile_output_filename=onefile_output_filename,
             start_binary=start_binary,
             expect_compression=compressor_python is not None,
             file_checksums=file_checksums,
             win_path_sep=win_path_sep,
+            low_memory=Options.isLowMemory(),
         )
     else:
         onefile_compressor_path = os.path.normpath(
             os.path.join(os.path.dirname(__file__), "..", "tools", "onefile_compressor")
         )
 
         mapping = {
@@ -196,14 +203,15 @@
                     compressor_python.getPythonExe(),
                     onefile_compressor_path,
                     dist_dir,
                     getExternalUsePath(onefile_output_filename, only_dirname=True),
                     start_binary,
                     str(file_checksums),
                     str(win_path_sep),
+                    str(Options.isLowMemory()),
                 ],
                 shell=False,
             )
 
 
 def packDistFolderToOnefileBootstrap(onefile_output_filename, dist_dir):
     postprocessing_logger.info(
@@ -238,14 +246,17 @@
     _runOnefileScons(
         onefile_compression=compressor_python is not None,
     )
 
     if isWin32Windows():
         executePostProcessingResources(manifest=None, onefile=True)
 
+    if isAndroidBasedLinux():
+        cleanupHeaderForAndroid(onefile_output_filename)
+
     Plugins.onBootstrapBinary(onefile_output_filename)
 
     if isMacOS():
         addMacOSCodeSignature(filenames=[onefile_output_filename])
 
     if not payload_used_in_build:
         runOnefileCompressor(
```

### Comparing `Nuitka-winsvc-1.7.5/nuitka/freezer/Standalone.py` & `Nuitka-winsvc-1.7.6/nuitka/freezer/Standalone.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/freezer/__init__.py` & `Nuitka-winsvc-1.7.6/nuitka/freezer/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/importing/IgnoreListing.py` & `Nuitka-winsvc-1.7.6/nuitka/importing/IgnoreListing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/importing/ImportCache.py` & `Nuitka-winsvc-1.7.6/nuitka/importing/ImportCache.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/importing/ImportResolving.py` & `Nuitka-winsvc-1.7.6/nuitka/importing/ImportResolving.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/importing/Importing.py` & `Nuitka-winsvc-1.7.6/nuitka/importing/Importing.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,18 @@
 from nuitka.plugins.Plugins import Plugins
 from nuitka.PythonFlavors import isNuitkaPython
 from nuitka.PythonVersions import python_version
 from nuitka.Tracing import my_print, recursion_logger
 from nuitka.tree.ReformulationMultidist import locateMultidistModule
 from nuitka.utils.AppDirs import getCacheDir
 from nuitka.utils.FileOperations import listDir, removeDirectory
-from nuitka.utils.Importing import getSharedLibrarySuffixes
+from nuitka.utils.Importing import (
+    getSharedLibrarySuffixes,
+    isBuiltinModuleName,
+)
 from nuitka.utils.ModuleNames import ModuleName
 from nuitka.utils.SharedLibraries import (
     hasUniversalOrMatchingMacOSArchitecture,
 )
 from nuitka.utils.Utils import isMacOS, isWin32OrPosixWindows
 
 from .IgnoreListing import isIgnoreListedNotExistingModule
@@ -658,16 +661,16 @@
     # and on some systems, that fails.
     if package_name is None and module_name == "site":
         candidate = os.environ.get("NUITKA_SITE_FILENAME", "")
 
         if candidate:
             return candidate, "py"
 
-    # Free pass for built-in modules, the need not exist.
-    if package_name is None and imp.is_builtin(module_name):
+    # Free pass for built-in modules, they need not exist.
+    if package_name is None and isBuiltinModuleName(module_name):
         return None
 
     search_path = getPackageSearchPath(package_name)
 
     if _debug_module_finding:
         my_print(
             "_findModuleInPath: Using search path", search_path, "for", package_name
```

### Comparing `Nuitka-winsvc-1.7.5/nuitka/importing/PreloadedPackages.py` & `Nuitka-winsvc-1.7.6/nuitka/importing/PreloadedPackages.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/importing/Recursion.py` & `Nuitka-winsvc-1.7.6/nuitka/importing/Recursion.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/importing/StandardLibrary.py` & `Nuitka-winsvc-1.7.6/nuitka/importing/StandardLibrary.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/importing/__init__.py` & `Nuitka-winsvc-1.7.6/nuitka/importing/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/AsyncgenNodes.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/AsyncgenNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/AttributeLookupNodes.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/AttributeLookupNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/AttributeNodes.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/AttributeNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/AttributeNodesGenerated.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/AttributeNodesGenerated.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/BuiltinAllNodes.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/BuiltinAllNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/BuiltinAnyNodes.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/BuiltinAnyNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/BuiltinComplexNodes.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/BuiltinComplexNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/BuiltinDecodingNodes.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/BuiltinDecodingNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/BuiltinDecoratorNodes.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/BuiltinDecoratorNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/BuiltinDictNodes.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/BuiltinDictNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/BuiltinFormatNodes.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/BuiltinFormatNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/BuiltinHashNodes.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/BuiltinHashNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/BuiltinIntegerNodes.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/BuiltinIntegerNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/BuiltinIteratorNodes.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/BuiltinIteratorNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/BuiltinLenNodes.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/BuiltinLenNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/BuiltinNextNodes.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/BuiltinNextNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/BuiltinOpenNodes.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/BuiltinOpenNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/BuiltinOperationNodeBasesGenerated.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/BuiltinOperationNodeBasesGenerated.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/BuiltinRangeNodes.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/BuiltinRangeNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/BuiltinRefNodes.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/BuiltinRefNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/BuiltinSumNodes.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/BuiltinSumNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/BuiltinTypeNodes.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/BuiltinTypeNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/BuiltinVarsNodes.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/BuiltinVarsNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/BytesNodes.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/BytesNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/CallNodes.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/CallNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/Checkers.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/Checkers.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/ChildrenHavingMixins.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/ChildrenHavingMixins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/ClassNodes.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/ClassNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/CodeObjectSpecs.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/CodeObjectSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/ComparisonNodes.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/ComparisonNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/ConditionalNodes.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/ConditionalNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/ConstantRefNodes.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/ConstantRefNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/ContainerMakingNodes.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/ContainerMakingNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/ContainerOperationNodes.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/ContainerOperationNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/CoroutineNodes.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/CoroutineNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/CtypesNodes.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/CtypesNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/DictionaryNodes.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/DictionaryNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/ExceptionNodes.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/ExceptionNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/ExecEvalNodes.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/ExecEvalNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/ExpressionBases.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/ExpressionBases.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/ExpressionBasesGenerated.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/ExpressionBasesGenerated.py`

 * *Files 1% similar despite different names*

```diff
@@ -1500,14 +1500,120 @@
     ChildHavingPairsTupleFinalNoRaiseMixin
 )
 ExpressionImportlibMetadataSelectableGroupsValueRefBase = (
     ChildHavingPairsTupleFinalNoRaiseMixin
 )
 
 
+class ChildHavingPromptOptionalFinalMixin(ExpressionBase):
+    # Mixins are not allowed to specify slots, pylint: disable=assigning-non-slot
+    __slots__ = ()
+
+    # This is generated for use in
+    #   ExpressionBuiltinInput
+
+    def __init__(self, prompt, source_ref):
+        if prompt is not None:
+            prompt.parent = self
+
+        self.subnode_prompt = prompt
+
+        ExpressionBase.__init__(self, source_ref)
+
+    def getVisitableNodes(self):
+        """The visitable nodes, with tuple values flattened."""
+
+        value = self.subnode_prompt
+
+        if value is None:
+            return ()
+        else:
+            return (value,)
+
+    def getVisitableNodesNamed(self):
+        """Named children dictionary.
+
+        For use in cloning nodes, debugging and XML output.
+        """
+
+        return (("prompt", self.subnode_prompt),)
+
+    def replaceChild(self, old_node, new_node):
+        value = self.subnode_prompt
+        if old_node is value:
+            if new_node is not None:
+                new_node.parent = self
+
+            self.subnode_prompt = new_node
+
+            return
+
+        raise AssertionError("Didn't find child", old_node, "in", self)
+
+    def getCloneArgs(self):
+        """Get clones of all children to pass for a new node.
+
+        Needs to make clones of child nodes too.
+        """
+
+        values = {
+            "prompt": self.subnode_prompt.makeClone()
+            if self.subnode_prompt is not None
+            else None,
+        }
+
+        values.update(self.getDetails())
+
+        return values
+
+    def finalize(self):
+        del self.parent
+
+        if self.subnode_prompt is not None:
+            self.subnode_prompt.finalize()
+        del self.subnode_prompt
+
+    def computeExpressionRaw(self, trace_collection):
+        """Compute an expression.
+
+        Default behavior is to just visit the child expressions first, and
+        then the node "computeExpression". For a few cases this needs to
+        be overloaded, e.g. conditional expressions.
+        """
+
+        # First apply the sub-expression, as they it's evaluated before.
+        expression = self.subnode_prompt
+
+        if expression is not None:
+            expression = trace_collection.onExpression(expression)
+
+            if expression.willRaiseAnyException():
+                return (
+                    expression,
+                    "new_raise",
+                    lambda: "For '%s' the child expression '%s' will raise."
+                    % (self.getChildNameNice(), expression.getChildNameNice()),
+                )
+
+        trace_collection.onExceptionRaiseExit(BaseException)
+        return self, None, None
+
+    def collectVariableAccesses(self, emit_read, emit_write):
+        """Collect variable reads and writes of child nodes."""
+
+        subnode_prompt = self.subnode_prompt
+
+        if subnode_prompt is not None:
+            self.subnode_prompt.collectVariableAccesses(emit_read, emit_write)
+
+
+# Assign the names that are easier to import with a stable name.
+ExpressionBuiltinInputBase = ChildHavingPromptOptionalFinalMixin
+
+
 class ChildHavingValueFinalNoRaiseMixin(ExpressionBase):
     # Mixins are not allowed to specify slots, pylint: disable=assigning-non-slot
     __slots__ = ()
 
     # This is generated for use in
     #   ExpressionBuiltinClassmethod
     #   ExpressionBuiltinStaticmethod
```

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/ExpressionShapeMixins.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/ExpressionShapeMixins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/FrameNodes.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/FrameNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/FunctionAttributeNodes.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/FunctionAttributeNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/FunctionNodes.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/FunctionNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/FutureSpecs.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/FutureSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/GeneratorNodes.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/GeneratorNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/GlobalsLocalsNodes.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/GlobalsLocalsNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/HardImportNodesGenerated.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/HardImportNodesGenerated.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/ImportHardNodes.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/ImportHardNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/ImportNodes.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/ImportNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/IndicatorMixins.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/IndicatorMixins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/InjectCNodes.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/InjectCNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/IterationHandles.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/IterationHandles.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/KeyValuePairNodes.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/KeyValuePairNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/ListOperationNodes.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/ListOperationNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/LocalsDictNodes.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/LocalsDictNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/LocalsScopes.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/LocalsScopes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/LoopNodes.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/LoopNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/MatchNodes.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/MatchNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/ModuleAttributeNodes.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/ModuleAttributeNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/ModuleNodes.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/ModuleNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/NodeBases.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/NodeBases.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/NodeMakingHelpers.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/NodeMakingHelpers.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/NodeMetaClasses.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/NodeMetaClasses.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/OperatorNodes.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/OperatorNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/OperatorNodesUnary.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/OperatorNodesUnary.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/OsSysNodes.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/OsSysNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/OutlineNodes.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/OutlineNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/PackageMetadataNodes.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/PackageMetadataNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/PackageResourceNodes.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/PackageResourceNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/PrintNodes.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/PrintNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/ReturnNodes.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/ReturnNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/SideEffectNodes.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/SideEffectNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/SliceNodes.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/SliceNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/StatementBasesGenerated.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/StatementBasesGenerated.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/StatementNodes.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/StatementNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/StrNodes.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/StrNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/StringConcatenationNodes.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/StringConcatenationNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/SubscriptNodes.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/SubscriptNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/TryNodes.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/TryNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/TypeMatchNodes.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/TypeMatchNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/TypeNodes.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/TypeNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/VariableAssignNodes.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/VariableAssignNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/VariableDelNodes.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/VariableDelNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/VariableNameNodes.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/VariableNameNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/VariableRefNodes.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/VariableRefNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/VariableReleaseNodes.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/VariableReleaseNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/YieldNodes.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/YieldNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/__init__.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/shapes/BuiltinTypeShapes.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/shapes/BuiltinTypeShapes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/shapes/ControlFlowDescriptions.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/shapes/ControlFlowDescriptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/shapes/ShapeMixins.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/shapes/ShapeMixins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/shapes/StandardShapes.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/shapes/StandardShapes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/nodes/shapes/__init__.py` & `Nuitka-winsvc-1.7.6/nuitka/nodes/shapes/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/optimizations/BytecodeDemotion.py` & `Nuitka-winsvc-1.7.6/nuitka/optimizations/BytecodeDemotion.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/optimizations/FunctionInlining.py` & `Nuitka-winsvc-1.7.6/nuitka/optimizations/FunctionInlining.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/optimizations/Graphs.py` & `Nuitka-winsvc-1.7.6/nuitka/optimizations/Graphs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/optimizations/Optimization.py` & `Nuitka-winsvc-1.7.6/nuitka/optimizations/Optimization.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/optimizations/OptimizeBuiltinCalls.py` & `Nuitka-winsvc-1.7.6/nuitka/optimizations/OptimizeBuiltinCalls.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,14 +49,15 @@
     ExpressionBuiltinBin,
     ExpressionBuiltinFormat,
     ExpressionBuiltinHex,
     ExpressionBuiltinId,
     ExpressionBuiltinOct,
 )
 from nuitka.nodes.BuiltinHashNodes import ExpressionBuiltinHash
+from nuitka.nodes.BuiltinInputNodes import ExpressionBuiltinInput
 from nuitka.nodes.BuiltinIntegerNodes import (
     ExpressionBuiltinInt1,
     ExpressionBuiltinInt2,
 )
 from nuitka.nodes.BuiltinIteratorNodes import (
     ExpressionBuiltinIter1,
     ExpressionBuiltinIter2,
@@ -1322,14 +1323,22 @@
     return BuiltinParameterSpecs.extractBuiltinArgs(
         node=node,
         builtin_class=ExpressionBuiltinHash,
         builtin_spec=BuiltinParameterSpecs.builtin_hash_spec,
     )
 
 
+def input_extractor(node):
+    return BuiltinParameterSpecs.extractBuiltinArgs(
+        node=node,
+        builtin_class=ExpressionBuiltinInput,
+        builtin_spec=BuiltinParameterSpecs.builtin_input_spec,
+    )
+
+
 def format_extractor(node):
     def makeFormat0(source_ref):
         # pylint: disable=unused-argument
 
         return makeRaiseExceptionReplacementExpressionFromInstance(
             expression=node,
             exception=TypeError("format() takes at least 1 argument (0 given)"),
@@ -1428,14 +1437,15 @@
     "slice": slice_extractor,
     "hash": hash_extractor,
     "format": format_extractor,
     "open": open_extractor,
     "staticmethod": staticmethod_extractor,
     "classmethod": classmethod_extractor,
     "divmod": divmod_extractor,
+    "input": input_extractor,
 }
 
 if python_version < 0x300:
     # These are not in Python3
     _dispatch_dict["long"] = long_extractor
     _dispatch_dict["unicode"] = unicode_extractor
     _dispatch_dict["execfile"] = execfile_extractor
```

### Comparing `Nuitka-winsvc-1.7.5/nuitka/optimizations/Tags.py` & `Nuitka-winsvc-1.7.6/nuitka/optimizations/Tags.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/optimizations/TraceCollections.py` & `Nuitka-winsvc-1.7.6/nuitka/optimizations/TraceCollections.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/optimizations/ValueTraces.py` & `Nuitka-winsvc-1.7.6/nuitka/optimizations/ValueTraces.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/optimizations/__init__.py` & `Nuitka-winsvc-1.7.6/nuitka/optimizations/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/pgo/PGO.py` & `Nuitka-winsvc-1.7.6/nuitka/pgo/PGO.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/pgo/__init__.py` & `Nuitka-winsvc-1.7.6/nuitka/pgo/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/plugins/PluginBase.py` & `Nuitka-winsvc-1.7.6/nuitka/plugins/PluginBase.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 
 The base class will serve as documentation. And it will point to examples of
 it being used.
 """
 
 import ast
 import functools
-import imp
 import inspect
 import os
 import sys
 
 from nuitka import Options
 from nuitka.__past__ import getMetaClassBase
 from nuitka.containers.Namedtuples import makeNamedtupleClass
@@ -66,14 +65,15 @@
 from nuitka.PythonVersions import (
     getTestExecutionPythonVersions,
     python_version,
 )
 from nuitka.Tracing import plugins_logger
 from nuitka.utils.Distributions import isDistributionCondaPackage
 from nuitka.utils.Execution import NuitkaCalledProcessError, check_output
+from nuitka.utils.Importing import isBuiltinModuleName
 from nuitka.utils.ModuleNames import (
     ModuleName,
     makeTriggerModuleName,
     post_module_load_trigger_name,
     pre_module_load_trigger_name,
 )
 from nuitka.utils.SharedLibraries import locateDLL, locateDLLsInDirectory
@@ -1141,15 +1141,15 @@
                 # Querying package versions.
                 "version": _getPackageVersion,
                 "plugin": _isPluginActive,
                 "no_asserts": hasPythonFlagNoAsserts(),
                 "no_docstrings": hasPythonFlagNoDocStrings(),
                 "no_annotations": hasPythonFlagNoAnnotations(),
                 # Querying package properties
-                "has_builtin_module": imp.is_builtin,
+                "has_builtin_module": isBuiltinModuleName,
             }
         )
 
         if isWin32Windows():
             context.update(
                 {
                     "arch_x86": getArchitecture() == "x86",
```

### Comparing `Nuitka-winsvc-1.7.5/nuitka/plugins/Plugins.py` & `Nuitka-winsvc-1.7.6/nuitka/plugins/Plugins.py`

 * *Files 0% similar despite different names*

```diff
@@ -203,14 +203,25 @@
     return ("tk-inter",)
 
 
 def getGuiPluginNames():
     return getQtPluginNames() + getOtherGuiPluginNames()
 
 
+def hasActiveGuiPluginForBinding(binding_name):
+    if binding_name in ("tkinter", "Tkinter"):
+        return hasActivePlugin("tk-inter")
+    elif binding_name in getQtBindingNames():
+        return hasActivePlugin(binding_name.lower())
+    else:
+        # For wx, we do not have a plugin right now, it just works, but
+        # also means it cannot be picked.
+        return False
+
+
 def hasActivePlugin(plugin_name):
     """Decide if a plugin is active.
 
     Args:
         plugin_name - name of the plugin
 
     Notes:
```

### Comparing `Nuitka-winsvc-1.7.5/nuitka/plugins/__init__.py` & `Nuitka-winsvc-1.7.6/nuitka/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/plugins/standard/AntiBloatPlugin.py` & `Nuitka-winsvc-1.7.6/nuitka/plugins/standard/AntiBloatPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/plugins/standard/ConsiderPyLintAnnotationsPlugin.py` & `Nuitka-winsvc-1.7.6/nuitka/plugins/standard/ConsiderPyLintAnnotationsPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/plugins/standard/DataFilesPlugin.py` & `Nuitka-winsvc-1.7.6/nuitka/plugins/standard/DataFilesPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/plugins/standard/DelvewheelPlugin.py` & `Nuitka-winsvc-1.7.6/nuitka/plugins/standard/DelvewheelPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/plugins/standard/DillPlugin.py` & `Nuitka-winsvc-1.7.6/nuitka/plugins/standard/DillPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/plugins/standard/DllFilesPlugin.py` & `Nuitka-winsvc-1.7.6/nuitka/plugins/standard/DllFilesPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/plugins/standard/EnumPlugin.py` & `Nuitka-winsvc-1.7.6/nuitka/plugins/standard/EnumPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/plugins/standard/EventletPlugin.py` & `Nuitka-winsvc-1.7.6/nuitka/plugins/standard/EventletPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/plugins/standard/GeventPlugin.py` & `Nuitka-winsvc-1.7.6/nuitka/plugins/standard/GeventPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/plugins/standard/GiPlugin.py` & `Nuitka-winsvc-1.7.6/nuitka/plugins/standard/GiPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/plugins/standard/GlfwPlugin.py` & `Nuitka-winsvc-1.7.6/nuitka/plugins/standard/GlfwPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/plugins/standard/ImplicitImports.py` & `Nuitka-winsvc-1.7.6/nuitka/plugins/standard/ImplicitImports.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/plugins/standard/KivyPlugin.py` & `Nuitka-winsvc-1.7.6/nuitka/plugins/standard/KivyPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/plugins/standard/MatplotlibPlugin.py` & `Nuitka-winsvc-1.7.6/nuitka/plugins/standard/MatplotlibPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/plugins/standard/MultiprocessingPlugin.py` & `Nuitka-winsvc-1.7.6/nuitka/plugins/standard/MultiprocessingPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/plugins/standard/NumpyPlugin.py` & `Nuitka-winsvc-1.7.6/nuitka/plugins/standard/NumpyPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/plugins/standard/OptionsNannyPlugin.py` & `Nuitka-winsvc-1.7.6/nuitka/plugins/standard/OptionsNannyPlugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,15 +93,17 @@
                 else:
                     downside_message = """\
 Otherwise a terminal window will open"""
 
                 self.info(
                     """\
 Note, when using '%s', consider using '--disable-console' option. %s. However for \
-debugging, terminal output is the easiest way to see informative traceback information."""
+debugging, terminal output is the easiest way to see informative traceback \
+and error information, so delay this until your program working and remove \
+once you find it non-working."""
                     % (full_name, downside_message)
                 )
 
         else:
             self.sysexitIllegalOptionValue(full_name, "console", console)
 
     def _checkMacOSBundleMode(self, full_name, macos_bundle):
```

### Comparing `Nuitka-winsvc-1.7.5/nuitka/plugins/standard/PbrPlugin.py` & `Nuitka-winsvc-1.7.6/nuitka/plugins/standard/PbrPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/plugins/standard/PkgResourcesPlugin.py` & `Nuitka-winsvc-1.7.6/nuitka/plugins/standard/PkgResourcesPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/plugins/standard/PmwPlugin.py` & `Nuitka-winsvc-1.7.6/nuitka/plugins/standard/PmwPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/plugins/standard/PySidePyQtPlugin.py` & `Nuitka-winsvc-1.7.6/nuitka/plugins/standard/PySidePyQtPlugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,32 +28,31 @@
     isOnefileMode,
     isStandaloneMode,
     shallCreateAppBundle,
 )
 from nuitka.plugins.PluginBase import NuitkaPluginBase
 from nuitka.plugins.Plugins import (
     getActiveQtPlugin,
+    getOtherGUIBindingNames,
     getQtBindingNames,
     getQtPluginNames,
+    hasActiveGuiPluginForBinding,
 )
 from nuitka.PythonFlavors import isAnacondaPython
 from nuitka.PythonVersions import python_version
 from nuitka.utils.FileOperations import getFileList, listDir
 from nuitka.utils.ModuleNames import ModuleName
 from nuitka.utils.Utils import (
     getArchitecture,
     isDebianBasedLinux,
     isLinux,
     isMacOS,
     isWin32Windows,
 )
 
-# Use to detect the Qt plugin that is active and check for conflicts.
-_qt_binding_names = getQtBindingNames()
-
 
 class NuitkaPluginQtBindingsPluginBase(NuitkaPluginBase):
     # Automatically suppress detectors for any other toolkit
     plugin_gui_toolkit = True
 
     # For overload in the derived bindings plugin.
     binding_name = None
@@ -76,15 +75,15 @@
         self.binding_package_name = ModuleName(self.binding_name)
 
         # Allow to specify none.
         if self.qt_plugins == set(["none"]):
             self.qt_plugins = set()
 
         # Prevent the list of binding names from being incomplete, it's used for conflicts.
-        assert self.binding_name in _qt_binding_names, self.binding_name
+        assert self.binding_name in getQtBindingNames(), self.binding_name
 
         # Also lets have consistency in naming.
         assert self.plugin_name in getQtPluginNames()
 
         active_qt_plugin_name = getActiveQtPlugin()
 
         if active_qt_plugin_name is not None:
@@ -105,15 +104,15 @@
 by default only the sensible ones are included, but you can also put
 "all" or list them individually. If you specify something that does
 not exist, a list of all available will be given.""",
         )
 
         group.add_option(
             "--noinclude-qt-translations",
-            action="store",
+            action="store_true",
             dest="no_qt_translations",
             default=False,
             help="""\
 Include Qt translations with QtWebEngine if used. These can be a lot
 of files that you may not want to be included.""",
         )
 
@@ -1060,15 +1059,15 @@
     def onModuleEncounter(
         self, using_module_name, module_name, module_filename, module_kind
     ):
         top_package_name = module_name.getTopLevelPackageName()
 
         if isStandaloneMode():
             if (
-                top_package_name in _qt_binding_names
+                top_package_name in getQtBindingNames()
                 and top_package_name != self.binding_name
             ):
                 if top_package_name not in self.warned_about:
                     self.info(
                         """\
 Unwanted import of '%(unwanted)s' that conflicts with '%(binding_name)s' \
 encountered, preventing its inclusion. As a result an "ImportError" might \
@@ -1084,14 +1083,23 @@
 
                 return (
                     False,
                     "Not included due to potentially conflicting Qt versions with selected Qt binding '%s'."
                     % self.binding_name,
                 )
 
+            if (
+                top_package_name in getOtherGUIBindingNames()
+                and not hasActiveGuiPluginForBinding(top_package_name)
+            ):
+                return (
+                    False,
+                    "Not included due to its plugin not being active, but a Qt plugin is.",
+                )
+
     def onModuleCompleteSet(self, module_set):
         self.onModuleCompleteSetGUI(
             module_set=module_set, plugin_binding_name=self.binding_name
         )
 
     def onModuleSourceCode(self, module_name, source_code):
         """Third party packages that make binding selections."""
@@ -1417,15 +1425,15 @@
 
     def onModuleEncounter(
         self, using_module_name, module_name, module_filename, module_kind
     ):
         top_package_name = module_name.getTopLevelPackageName()
 
         if isStandaloneMode():
-            if top_package_name in _qt_binding_names:
+            if top_package_name in getQtBindingNames():
                 if top_package_name not in self.warned_about:
                     self.info(
                         """\
 Unwanted import of '%(unwanted)s' that is forbidden encountered, preventing
 its use. As a result an "ImportError" might be given at run time. Uninstall
 it for full compatible behavior with the uncompiled code to debug it."""
                         % {
```

### Comparing `Nuitka-winsvc-1.7.5/nuitka/plugins/standard/PywebViewPlugin.py` & `Nuitka-winsvc-1.7.6/nuitka/plugins/standard/PywebViewPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/plugins/standard/TensorflowPlugin.py` & `Nuitka-winsvc-1.7.6/nuitka/plugins/standard/TensorflowPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/plugins/standard/TkinterPlugin.py` & `Nuitka-winsvc-1.7.6/nuitka/plugins/standard/TkinterPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/plugins/standard/TorchPlugin.py` & `Nuitka-winsvc-1.7.6/nuitka/plugins/standard/TorchPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/plugins/standard/TransformersPlugin.py` & `Nuitka-winsvc-1.7.6/nuitka/plugins/standard/TransformersPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/plugins/standard/TrioPlugin.py` & `Nuitka-winsvc-1.7.6/nuitka/plugins/standard/TrioPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/plugins/standard/UpxPlugin.py` & `Nuitka-winsvc-1.7.6/nuitka/plugins/standard/UpxPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/plugins/standard/__init__.py` & `Nuitka-winsvc-1.7.6/nuitka/plugins/standard/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/plugins/standard/standard.nuitka-package.config.yml` & `Nuitka-winsvc-1.7.6/nuitka/plugins/standard/standard.nuitka-package.config.yml`

 * *Files 0% similar despite different names*

```diff
@@ -1149,14 +1149,27 @@
 - module-name: 'keras.utils.vis_utils'
   anti-bloat:
     - description: 'remove IPython reference'
       replacements_plain:
         'from IPython import display': 'raise ImportError'
       when: 'not use_ipython'
 
+- module-name: 'keyring'
+  data-files:
+    include-metadata:
+      - 'keyring'
+  implicit-imports:
+    - depends:
+        - 'keyring.backends.*'
+
+- module-name: 'keyring.backends.Windows'
+  implicit-imports:
+    - depends:
+        - 'win32timezone'
+
 - module-name: 'kivy'
   data-files:
     dirs:
       - 'data'
 
 - module-name: 'kivy._clock'
   implicit-imports:
@@ -1666,30 +1679,30 @@
           if not val:
               try:
                   smsg = msg()
               except TypeError:
                   smsg = msg
               raise AssertionError(smsg)
 
-        def assert_equal(actual, desired, err_msg='', verbose=True):
+        def assert_equal(*args, **kwargs):
           pass
 
-        def assert_approx_equal(actual, desired, significant=7, err_msg='', verbose=True):
+        def assert_approx_equal(*args, **kwargs):
           pass
 
-        def assert_almost_equal(actual, desired, decimal=7, err_msg='', verbose=True):
+        def assert_almost_equal(*args, **kwargs):
           pass
 
-        def assert_array_equal(x, y, err_msg='', verbose=True, *, strict=False):
+        def assert_array_equal(*args, **kwargs):
           pass
 
-        def assert_array_less(x, y, err_msg='', verbose=True):
+        def assert_array_less(*args, **kwargs):
           pass
 
-        def assert_array_almost_equal(x, y, decimal=6, err_msg='', verbose=True):
+        def assert_array_almost_equal(*args, **kwargs):
           pass
 
 - module-name: 'numpy.testing._private.pytesttester'
   anti-bloat:
     - description: 'remove numpy testing framework'
       module_code: |
         class PytestTester:
@@ -1751,14 +1764,27 @@
 
 - module-name: 'opentele.utils'
   anti-bloat:
     - description: 'workaround compiled function decorator issues'
       replacements_plain:
         'bases = func.__class__.__bases__': 'bases = func.__class__.__bases__ if func.__class__.__bases__ != (FunctionType,) else (object,)'
 
+- module-name: 'opentelemetry.exporter.jaeger.thrift'
+  import-hacks:
+    - global-sys-path:
+        # This package forces itself into "sys.path" and expects absolute
+        # imports like "jaeger" to be available.
+        - 'gen'
+
+- module-name: 'opentelemetry.exporter.jaeger.thrift.gen'
+  anti-bloat:
+    - description: 'remove "sys.path" hack'
+      replacements_plain:
+        'sys.path.append': ''
+
 - module-name: 'opentelemetry.propagate'
   data-files:
     include-metadata:
       - 'opentelemetry-api'
 
   implicit-imports:
     - depends:
@@ -5043,21 +5069,44 @@
     - description: 'compatibility workaround'
       replacements_plain:
         ? "\ndef _dp_init_subclass"
         : |-
           @classmethod
           def _dp_init_subclass
 
+- module-name: 'torch_scatter'
+  anti-bloat:
+    - description: 'workaround finding DLLs as modules by wrong names'
+      replacements_plain:
+        "f'{library}_cuda', [osp.dirname(__file__)]": "f'torch_scatter.{library}_cuda'"
+        "f'{library}_cpu', [osp.dirname(__file__)]": "f'torch_scatter.{library}_cpu'"
+        'importlib.machinery.PathFinder()': 'importlib.util'
+  implicit-imports:
+    - depends:
+        - '._version_cpu'
+        - '._scatter_cpu'
+        - '._segment_csr_cpu'
+        - '._segment_coo_cpu'
+        - '._version_cuda'
+        - '._scatter_cuda'
+        - '._segment_csr_cuda'
+        - '._segment_coo_cuda'
+
 - module-name: 'torchaudio'
   import-hacks:
     - find-dlls-near-module:
         - 'torch'
     - acceptable-missing-dlls:
         - '_torchaudio_ffmpeg'
 
+- module-name: 'torchaudio.lib._torchaudio'
+  implicit-imports:
+    - depends:
+        - 'torchaudio.lib.libtorchaudio'
+
 - module-name: 'torchmetrics.utilities.checks'
   anti-bloat:
     - description: 'remove unittest reference'
       replacements_plain:
         'from unittest.mock import Mock': ''
         'isinstance(instance_attr, Mock)': 'False'
 
@@ -5153,14 +5202,20 @@
 - module-name: 'transformers.models.yoso.modeling_yoso'
   anti-bloat:
     - description: 'remove setuptools usage'
       change_function:
         'load_cuda_kernels': "'(lambda : False)'"
       when: 'not use_setuptools'
 
+- module-name: 'transformers.processing_utils'
+  anti-bloat:
+    - description: 'workaround manual import issue'
+      replacements_plain:
+        'transformers_module = direct_transformers_import(Path(__file__).parent)': 'import transformers as transformers_module'
+
 - module-name: 'transformers.trainer'
   anti-bloat:
     - description: 'remove IPython reference'
       replacements_plain:
         'is_in_notebook()': 'False'
       when: 'not use_ipython'
 
@@ -5481,14 +5536,29 @@
 
 - module-name: 'webview'
   data-files:
     dirs:
       - 'lib'
   dlls:
     - from_filenames:
+        relative_path: 'lib/runtimes/win-x86/native'
+        prefixes:
+          - 'WebView2Loader'
+      when: 'win32 and arch_x86'
+    - from_filenames:
+        relative_path: 'lib/runtimes/win-x64/native'
+        prefixes:
+          - 'WebView2Loader'
+      when: 'win32 and arch_amd64'
+    - from_filenames:
+        relative_path: 'lib/runtimes/win-arm64/native'
+        prefixes:
+          - 'WebView2Loader'
+      when: 'win32 and arch_arm64'
+    - from_filenames:
         relative_path: 'lib/x86'
         prefixes:
           - 'WebView2Loader'
       when: 'win32 and arch_x86'
     - from_filenames:
         relative_path: 'lib/x64'
         prefixes:
@@ -5517,14 +5587,20 @@
 
 - module-name: 'webview.platforms.edgechromium'
   anti-bloat:
     - description: 'workaround unused platform DLL checks'
       replacements_plain:
         "';' + interop_dll_path(platform)": "';' + os.path.abspath(os.path.join(os.path.dirname(__file__), '..', 'lib', platform))"
 
+- module-name: 'werkzeug.serving'
+  anti-bloat:
+    - description: 'remove ability to run with reloader'
+      replacements_plain:
+        'if use_reloader:': 'if False:'
+
 - module-name: 'win32com'
   import-hacks:
     # This package adds another directory to the search path of itself,
     # which we will not find packages in unless added.
     - package-dirs:
         - 'win32comext'
       when: 'win32'
@@ -5543,14 +5619,21 @@
       - description: 'wx will crash in console mode during startup'
         console: 'yes'
         when: 'macos'
       - description: 'wx requires program to be in bundle form'
         macos_bundle: 'yes'
         when: 'macos'
 
+- module-name: 'wx.html2'
+  dlls:
+    - from_filenames:
+        prefixes:
+          - 'WebView2Loader'
+      when: 'win32'
+
 - module-name: 'xarray'
   data-files:
     dirs:
       - 'static'
 
 - module-name: 'xarray.backends.locks'
   anti-bloat:
```

### Comparing `Nuitka-winsvc-1.7.5/nuitka/plugins/standard/stdlib2.nuitka-package.config.yml` & `Nuitka-winsvc-1.7.6/nuitka/plugins/standard/stdlib2.nuitka-package.config.yml`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/plugins/standard/stdlib3.nuitka-package.config.yml` & `Nuitka-winsvc-1.7.6/nuitka/plugins/standard/stdlib3.nuitka-package.config.yml`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/reports/LicenseReport.rst.j2` & `Nuitka-winsvc-1.7.6/nuitka/reports/LicenseReport.rst.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/reports/Reports.py` & `Nuitka-winsvc-1.7.6/nuitka/reports/Reports.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/reports/__init__.py` & `Nuitka-winsvc-1.7.6/nuitka/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/specs/BuiltinBytesOperationSpecs.py` & `Nuitka-winsvc-1.7.6/nuitka/specs/BuiltinBytesOperationSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/specs/BuiltinDictOperationSpecs.py` & `Nuitka-winsvc-1.7.6/nuitka/specs/BuiltinDictOperationSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/specs/BuiltinListOperationSpecs.py` & `Nuitka-winsvc-1.7.6/nuitka/specs/BuiltinListOperationSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/specs/BuiltinParameterSpecs.py` & `Nuitka-winsvc-1.7.6/nuitka/specs/BuiltinParameterSpecs.py`

 * *Files 0% similar despite different names*

```diff
@@ -487,14 +487,18 @@
 # Beware: One argument version defines "stop", not "start".
 builtin_slice_spec = BuiltinParameterSpecNoKeywords(
     "slice", ("start", "stop", "step"), default_count=2
 )
 
 builtin_hash_spec = BuiltinParameterSpecNoKeywords("hash", ("object",), default_count=0)
 
+builtin_input_spec = BuiltinParameterSpecNoKeywords(
+    "input", ("prompt",), default_count=1
+)
+
 builtin_format_spec = BuiltinParameterSpecNoKeywords(
     "format", ("value", "format_spec"), default_count=1
 )
 
 if python_version < 0x380:
     builtin_sum_spec = BuiltinParameterSpecNoKeywords(
         "sum", ("sequence", "start"), default_count=1
```

### Comparing `Nuitka-winsvc-1.7.5/nuitka/specs/BuiltinStrOperationSpecs.py` & `Nuitka-winsvc-1.7.6/nuitka/specs/BuiltinStrOperationSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/specs/BuiltinTypeOperationSpecs.py` & `Nuitka-winsvc-1.7.6/nuitka/specs/BuiltinTypeOperationSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/specs/BuiltinUnicodeOperationSpecs.py` & `Nuitka-winsvc-1.7.6/nuitka/specs/BuiltinUnicodeOperationSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/specs/HardImportSpecs.py` & `Nuitka-winsvc-1.7.6/nuitka/specs/HardImportSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/specs/ParameterSpecs.py` & `Nuitka-winsvc-1.7.6/nuitka/specs/ParameterSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/specs/__init__.py` & `Nuitka-winsvc-1.7.6/nuitka/specs/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tools/Basics.py` & `Nuitka-winsvc-1.7.6/nuitka/tools/Basics.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tools/__init__.py` & `Nuitka-winsvc-1.7.6/nuitka/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tools/commercial/__init__.py` & `Nuitka-winsvc-1.7.6/nuitka/tools/commercial/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tools/data_composer/DataComposer.py` & `Nuitka-winsvc-1.7.6/nuitka/tools/data_composer/DataComposer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tools/data_composer/__init__.py` & `Nuitka-winsvc-1.7.6/nuitka/tools/data_composer/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tools/data_composer/__main__.py` & `Nuitka-winsvc-1.7.6/nuitka/tools/data_composer/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tools/environments/CreateEnvironment.py` & `Nuitka-winsvc-1.7.6/nuitka/tools/environments/CreateEnvironment.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tools/environments/Virtualenv.py` & `Nuitka-winsvc-1.7.6/nuitka/tools/environments/Virtualenv.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tools/environments/__init__.py` & `Nuitka-winsvc-1.7.6/nuitka/tools/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tools/general/__init__.py` & `Nuitka-winsvc-1.7.6/nuitka/tools/general/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tools/general/dll_report/__init__.py` & `Nuitka-winsvc-1.7.6/nuitka/tools/general/dll_report/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tools/general/dll_report/__main__.py` & `Nuitka-winsvc-1.7.6/nuitka/tools/general/dll_report/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tools/general/find_module/FindModuleCode.py` & `Nuitka-winsvc-1.7.6/nuitka/tools/general/find_module/FindModuleCode.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tools/general/find_module/__init__.py` & `Nuitka-winsvc-1.7.6/nuitka/tools/general/find_module/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tools/onefile_compressor/OnefileCompressor.py` & `Nuitka-winsvc-1.7.6/nuitka/tools/onefile_compressor/OnefileCompressor.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,21 +40,21 @@
     decoratorRetries,
     isPosixWindows,
     isWin32OrPosixWindows,
     isWin32Windows,
 )
 
 
-def getCompressorFunction(expect_compression):
+def getCompressorFunction(expect_compression, low_memory):
     # spell-checker: ignore zstd, closefd
 
     if expect_compression:
         from zstandard import ZstdCompressor  # pylint: disable=I0021,import-error
 
-        compressor_context = ZstdCompressor(level=22)
+        compressor_context = ZstdCompressor(level=3 if low_memory else 22)
 
         @contextmanager
         def useCompressedFile(output_file):
             with compressor_context.stream_writer(
                 output_file, closefd=False
             ) as compressed_file:
                 yield compressed_file
@@ -117,18 +117,20 @@
 def attachOnefilePayload(
     dist_dir,
     onefile_output_filename,
     start_binary,
     expect_compression,
     file_checksums,
     win_path_sep,
+    low_memory,
 ):
     # Somewhat detail rich, pylint: disable=too-many-statements
     compression_indicator, compressor = getCompressorFunction(
-        expect_compression=expect_compression
+        expect_compression=expect_compression,
+        low_memory=low_memory,
     )
 
     def _attachOnefilePayloadFile(
         compressed_file, filename_full, dist_dir, filename_encoding
     ):
         payload_item_size = 0
 
@@ -283,22 +285,24 @@
     # Internal tool, most simple command line handling. This is the build directory
     # where main Nuitka put the .const files.
     dist_dir = sys.argv[1]
     onefile_output_filename = sys.argv[2]
     start_binary = os.path.normpath(sys.argv[3])  # Might switch from MSYS2 to CPython
     file_checksums = sys.argv[4] == "True"
     win_path_sep = sys.argv[5] == "True"
+    low_memory = sys.argv[6] == "True"
 
     if os.environ.get("NUITKA_PROGRESS_BAR") == "1":
         enableProgressBar()
 
     attachOnefilePayload(
         dist_dir=dist_dir,
         onefile_output_filename=onefile_output_filename,
         start_binary=start_binary,
         # We wouldn't be here, if that was not the case.
         expect_compression=True,
         file_checksums=file_checksums,
         win_path_sep=win_path_sep,
+        low_memory=low_memory,
     )
 
     sys.exit(0)
```

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tools/onefile_compressor/__init__.py` & `Nuitka-winsvc-1.7.6/nuitka/tools/onefile_compressor/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tools/onefile_compressor/__main__.py` & `Nuitka-winsvc-1.7.6/nuitka/tools/onefile_compressor/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tools/podman/Podman.py` & `Nuitka-winsvc-1.7.6/nuitka/tools/podman/Podman.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tools/podman/__init__.py` & `Nuitka-winsvc-1.7.6/nuitka/tools/podman/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tools/podman/__main__.py` & `Nuitka-winsvc-1.7.6/nuitka/tools/podman/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tools/profiler/__init__.py` & `Nuitka-winsvc-1.7.6/nuitka/tools/profiler/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tools/profiler/__main__.py` & `Nuitka-winsvc-1.7.6/nuitka/tools/profiler/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tools/scanning/DisplayPackageDLLs.py` & `Nuitka-winsvc-1.7.6/nuitka/tools/scanning/DisplayPackageDLLs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tools/scanning/DisplayPackageData.py` & `Nuitka-winsvc-1.7.6/nuitka/tools/scanning/DisplayPackageData.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tools/scanning/__init__.py` & `Nuitka-winsvc-1.7.6/nuitka/tools/scanning/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tools/specialize/CTypeDescriptions.py` & `Nuitka-winsvc-1.7.6/nuitka/tools/specialize/CTypeDescriptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tools/specialize/Common.py` & `Nuitka-winsvc-1.7.6/nuitka/tools/specialize/Common.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tools/specialize/SpecializeC.py` & `Nuitka-winsvc-1.7.6/nuitka/tools/specialize/SpecializeC.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tools/specialize/SpecializePython.py` & `Nuitka-winsvc-1.7.6/nuitka/tools/specialize/SpecializePython.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tools/specialize/__init__.py` & `Nuitka-winsvc-1.7.6/nuitka/tools/specialize/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tools/testing/Common.py` & `Nuitka-winsvc-1.7.6/nuitka/tools/testing/Common.py`

 * *Files 0% similar despite different names*

```diff
@@ -586,15 +586,15 @@
         elif type(x) is dict:
             if "__builtins__" in x:
                 k = "<module dict %s>" % x["__name__"]
             elif "__spec__" in x and "__name__" in x:
                 k = "<module dict %s>" % x["__name__"]
             else:
                 k = str(x)
-        elif x.__class__.__name__ == "compiled_frame":
+        elif hasattr(x, "__class__") and x.__class__.__name__ == "compiled_frame":
             k = "<compiled_frame at xxx, line %d code %s" % (x.f_lineno, x.f_code)
         else:
             k = str(x)
 
         c = sys.getrefcount(x)
 
         if k in m:
```

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tools/testing/Constructs.py` & `Nuitka-winsvc-1.7.6/nuitka/tools/testing/Constructs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tools/testing/OutputComparison.py` & `Nuitka-winsvc-1.7.6/nuitka/tools/testing/OutputComparison.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tools/testing/Pythons.py` & `Nuitka-winsvc-1.7.6/nuitka/tools/testing/Pythons.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tools/testing/RuntimeTracing.py` & `Nuitka-winsvc-1.7.6/nuitka/tools/testing/RuntimeTracing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tools/testing/SearchModes.py` & `Nuitka-winsvc-1.7.6/nuitka/tools/testing/SearchModes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tools/testing/Valgrind.py` & `Nuitka-winsvc-1.7.6/nuitka/tools/testing/Valgrind.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tools/testing/__init__.py` & `Nuitka-winsvc-1.7.6/nuitka/tools/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tools/testing/check_reference_counts/__init__.py` & `Nuitka-winsvc-1.7.6/nuitka/tools/testing/check_reference_counts/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tools/testing/check_reference_counts/__main__.py` & `Nuitka-winsvc-1.7.6/nuitka/tools/testing/check_reference_counts/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tools/testing/compare_with_cpython/__init__.py` & `Nuitka-winsvc-1.7.6/nuitka/tools/testing/compare_with_cpython/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tools/testing/compare_with_cpython/__main__.py` & `Nuitka-winsvc-1.7.6/nuitka/tools/testing/compare_with_cpython/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tools/testing/find_sxs_modules/__init__.py` & `Nuitka-winsvc-1.7.6/nuitka/tools/testing/find_sxs_modules/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tools/testing/find_sxs_modules/__main__.py` & `Nuitka-winsvc-1.7.6/nuitka/tools/testing/find_sxs_modules/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tools/testing/measure_construct_performance/__init__.py` & `Nuitka-winsvc-1.7.6/nuitka/tools/testing/measure_construct_performance/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tools/testing/measure_construct_performance/__main__.py` & `Nuitka-winsvc-1.7.6/nuitka/tools/testing/measure_construct_performance/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tools/testing/run_nuitka_tests/__init__.py` & `Nuitka-winsvc-1.7.6/nuitka/tools/testing/run_nuitka_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tools/testing/run_nuitka_tests/__main__.py` & `Nuitka-winsvc-1.7.6/nuitka/tools/testing/run_nuitka_tests/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tools/watch/__init__.py` & `Nuitka-winsvc-1.7.6/nuitka/tools/watch/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tools/watch/__main__.py` & `Nuitka-winsvc-1.7.6/nuitka/tools/watch/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tree/Building.py` & `Nuitka-winsvc-1.7.6/nuitka/tree/Building.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tree/ComplexCallHelperFunctions.py` & `Nuitka-winsvc-1.7.6/nuitka/tree/ComplexCallHelperFunctions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tree/Extractions.py` & `Nuitka-winsvc-1.7.6/nuitka/tree/Extractions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tree/InternalModule.py` & `Nuitka-winsvc-1.7.6/nuitka/tree/InternalModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tree/Operations.py` & `Nuitka-winsvc-1.7.6/nuitka/tree/Operations.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tree/ReformulationAssertStatements.py` & `Nuitka-winsvc-1.7.6/nuitka/tree/ReformulationAssertStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tree/ReformulationAssignmentStatements.py` & `Nuitka-winsvc-1.7.6/nuitka/tree/ReformulationAssignmentStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tree/ReformulationBooleanExpressions.py` & `Nuitka-winsvc-1.7.6/nuitka/tree/ReformulationBooleanExpressions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tree/ReformulationCallExpressions.py` & `Nuitka-winsvc-1.7.6/nuitka/tree/ReformulationCallExpressions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tree/ReformulationClasses.py` & `Nuitka-winsvc-1.7.6/nuitka/tree/ReformulationClasses.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tree/ReformulationClasses3.py` & `Nuitka-winsvc-1.7.6/nuitka/tree/ReformulationClasses3.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tree/ReformulationComparisonExpressions.py` & `Nuitka-winsvc-1.7.6/nuitka/tree/ReformulationComparisonExpressions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tree/ReformulationContractionExpressions.py` & `Nuitka-winsvc-1.7.6/nuitka/tree/ReformulationContractionExpressions.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,14 @@
 )
 from nuitka.nodes.DictionaryNodes import (
     StatementDictOperationSet,
     StatementDictOperationSetKeyValue,
 )
 from nuitka.nodes.FrameNodes import (
     StatementsFrameAsyncgen,
-    StatementsFrameFunction,
     StatementsFrameGenerator,
 )
 from nuitka.nodes.FunctionNodes import ExpressionFunctionRef
 from nuitka.nodes.GeneratorNodes import (
     ExpressionGeneratorObjectBody,
     ExpressionMakeGeneratorObject,
     StatementGeneratorReturnNone,
@@ -399,25 +398,14 @@
                     for_asyncgen=False,
                     source_ref=source_ref,
                 ),
                 source_ref=source_ref.atInternal(),
             )
         )
 
-    if for_asyncgen and python_version >= 0x370 and node.generators[0].is_async:
-        statements.append(
-            makeStatementAssignmentVariable(
-                variable=iter_tmp,
-                source=ExpressionTempVariableRef(
-                    variable=iter_tmp, source_ref=source_ref
-                ),
-                source_ref=source_ref,
-            )
-        )
-
     if start_value is not None:
         statements.append(
             makeStatementAssignmentVariable(
                 variable=container_tmp,
                 source=makeConstantRefNode(constant=start_value, source_ref=source_ref),
                 source_ref=source_ref.atInternal(),
             )
@@ -436,15 +424,19 @@
                 ),
                 source_ref=source_ref,
             )
         else:
             assert emit_class is ExpressionYield
 
             current_body = emit_class(
-                buildNode(provider=function_body, node=node.elt, source_ref=source_ref),
+                buildNode(
+                    provider=function_body,
+                    node=node.elt,
+                    source_ref=source_ref,
+                ),
                 source_ref=source_ref,
             )
     else:
         current_body = emit_class(
             dict_arg=ExpressionTempVariableRef(
                 variable=container_tmp, source_ref=source_ref
             ),
@@ -586,15 +578,16 @@
 
     return statements, release_statements
 
 
 def _buildContractionNode(provider, node, name, emit_class, start_value, source_ref):
     # The contraction nodes are reformulated to function bodies, with loops as
     # described in the Developer Manual. They use a lot of temporary names,
-    # nested blocks, etc. and so a lot of variable names, pylint:disable=too-many-locals
+    # nested blocks, etc. and so a lot of variable names.
+    # pylint: disable=too-many-locals
 
     function_body = ExpressionOutlineFunction(
         provider=provider, name=intern(name[1:-1]), source_ref=source_ref
     )
 
     iter_tmp = function_body.allocateTempVariable(temp_scope=None, name=".0")
 
@@ -639,15 +632,15 @@
             provider=function_body,
             tried=mergeStatements((statements, return_statement)),
             final=release_statements,
             source_ref=source_ref.atInternal(),
         ),
     )
 
-    if python_version < 0x300:
+    if python_version < 0x300 or emit_class is not ExpressionYield:
         body = makeStatementsSequenceFromStatements(assign_iter_statement, statements)
     else:
         parent_module = provider.getParentModule()
 
         code_object = CodeObjectSpec(
             co_name=name,
             co_qualname=provider.getChildQualname(name),
@@ -662,15 +655,15 @@
             co_filename=parent_module.getRunTimeFilename(),
             co_lineno=source_ref.getLineNumber(),
             future_spec=parent_module.getFutureSpec(),
         )
 
         body = makeStatementsSequenceFromStatements(
             assign_iter_statement,
-            StatementsFrameFunction(
+            StatementsFrameGenerator(
                 statements=mergeStatements(statements, False),
                 code_object=code_object,
                 source_ref=source_ref,
             ),
         )
 
     function_body.setChildBody(body)
```

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tree/ReformulationDictionaryCreation.py` & `Nuitka-winsvc-1.7.6/nuitka/tree/ReformulationDictionaryCreation.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tree/ReformulationExecStatements.py` & `Nuitka-winsvc-1.7.6/nuitka/tree/ReformulationExecStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tree/ReformulationForLoopStatements.py` & `Nuitka-winsvc-1.7.6/nuitka/tree/ReformulationForLoopStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tree/ReformulationFunctionStatements.py` & `Nuitka-winsvc-1.7.6/nuitka/tree/ReformulationFunctionStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tree/ReformulationImportStatements.py` & `Nuitka-winsvc-1.7.6/nuitka/tree/ReformulationImportStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tree/ReformulationLambdaExpressions.py` & `Nuitka-winsvc-1.7.6/nuitka/tree/ReformulationLambdaExpressions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tree/ReformulationMatchStatements.py` & `Nuitka-winsvc-1.7.6/nuitka/tree/ReformulationMatchStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tree/ReformulationMultidist.py` & `Nuitka-winsvc-1.7.6/nuitka/tree/ReformulationMultidist.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tree/ReformulationNamespacePackages.py` & `Nuitka-winsvc-1.7.6/nuitka/tree/ReformulationNamespacePackages.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tree/ReformulationPrintStatements.py` & `Nuitka-winsvc-1.7.6/nuitka/tree/ReformulationPrintStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tree/ReformulationSequenceCreation.py` & `Nuitka-winsvc-1.7.6/nuitka/tree/ReformulationSequenceCreation.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tree/ReformulationSubscriptExpressions.py` & `Nuitka-winsvc-1.7.6/nuitka/tree/ReformulationSubscriptExpressions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tree/ReformulationTryExceptStatements.py` & `Nuitka-winsvc-1.7.6/nuitka/tree/ReformulationTryExceptStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tree/ReformulationTryFinallyStatements.py` & `Nuitka-winsvc-1.7.6/nuitka/tree/ReformulationTryFinallyStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tree/ReformulationWhileLoopStatements.py` & `Nuitka-winsvc-1.7.6/nuitka/tree/ReformulationWhileLoopStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tree/ReformulationWithStatements.py` & `Nuitka-winsvc-1.7.6/nuitka/tree/ReformulationWithStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tree/ReformulationYieldExpressions.py` & `Nuitka-winsvc-1.7.6/nuitka/tree/ReformulationYieldExpressions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tree/SourceHandling.py` & `Nuitka-winsvc-1.7.6/nuitka/tree/SourceHandling.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tree/SyntaxErrors.py` & `Nuitka-winsvc-1.7.6/nuitka/tree/SyntaxErrors.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tree/TreeHelpers.py` & `Nuitka-winsvc-1.7.6/nuitka/tree/TreeHelpers.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tree/VariableClosure.py` & `Nuitka-winsvc-1.7.6/nuitka/tree/VariableClosure.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/tree/__init__.py` & `Nuitka-winsvc-1.7.6/nuitka/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/utils/AppDirs.py` & `Nuitka-winsvc-1.7.6/nuitka/utils/AppDirs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/utils/CStrings.py` & `Nuitka-winsvc-1.7.6/nuitka/utils/CStrings.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/utils/CommandLineOptions.py` & `Nuitka-winsvc-1.7.6/nuitka/utils/CommandLineOptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/utils/Distributions.py` & `Nuitka-winsvc-1.7.6/nuitka/utils/Distributions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/utils/Download.py` & `Nuitka-winsvc-1.7.6/nuitka/utils/Download.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/utils/Execution.py` & `Nuitka-winsvc-1.7.6/nuitka/utils/Execution.py`

 * *Files 2% similar despite different names*

```diff
@@ -329,22 +329,28 @@
         return subprocess.NULLDEV
     except AttributeError:
         # File is supposed to stay open, pylint: disable=consider-using-with
         subprocess.NULLDEV = open(os.devnull, "rb")
         return subprocess.NULLDEV
 
 
-def executeToolChecked(logger, command, absence_message, stderr_filter=None):
+def executeToolChecked(
+    logger, command, absence_message, stderr_filter=None, optional=False
+):
     """Execute external tool, checking for success and no error outputs, returning result."""
 
     command = list(command)
     tool = command[0]
 
     if not isExecutableCommand(tool):
-        logger.sysexit(absence_message)
+        if optional:
+            logger.warning(absence_message)
+            return 0, b"", b""
+        else:
+            logger.sysexit(absence_message)
 
     # Allow to avoid repeated scans in PATH for the tool.
     command[0] = getExecutablePath(tool)
 
     process = subprocess.Popen(
         command,
         stdin=getNullInput(),
```

### Comparing `Nuitka-winsvc-1.7.5/nuitka/utils/FileOperations.py` & `Nuitka-winsvc-1.7.6/nuitka/utils/FileOperations.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/utils/Hashing.py` & `Nuitka-winsvc-1.7.6/nuitka/utils/Hashing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/utils/Images.py` & `Nuitka-winsvc-1.7.6/nuitka/utils/Images.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/utils/Importing.py` & `Nuitka-winsvc-1.7.6/nuitka/utils/Importing.py`

 * *Files 1% similar despite different names*

```diff
@@ -212,7 +212,16 @@
                 _compile_time_modules[module_name] = sys.modules[module_name]
 
     # Some code should only use this, after knowing it will be found. Complain if
     # that is not the case.
     assert _compile_time_modules[module_name] or not must_exist
 
     return _compile_time_modules[module_name] or None
+
+
+def isBuiltinModuleName(module_name):
+    if python_version < 0x300:
+        import imp as _imp
+    else:
+        import _imp
+
+    return _imp.is_builtin(module_name)
```

### Comparing `Nuitka-winsvc-1.7.5/nuitka/utils/InstalledPythons.py` & `Nuitka-winsvc-1.7.6/nuitka/utils/InstalledPythons.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/utils/InstanceCounters.py` & `Nuitka-winsvc-1.7.6/nuitka/utils/InstanceCounters.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/utils/Jinja2.py` & `Nuitka-winsvc-1.7.6/nuitka/utils/Jinja2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/utils/Json.py` & `Nuitka-winsvc-1.7.6/nuitka/utils/Json.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/utils/MacOSApp.py` & `Nuitka-winsvc-1.7.6/nuitka/utils/MacOSApp.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/utils/MemoryUsage.py` & `Nuitka-winsvc-1.7.6/nuitka/utils/MemoryUsage.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/utils/ModuleNames.py` & `Nuitka-winsvc-1.7.6/nuitka/utils/ModuleNames.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/utils/ReExecute.py` & `Nuitka-winsvc-1.7.6/nuitka/utils/ReExecute.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/utils/Rest.py` & `Nuitka-winsvc-1.7.6/nuitka/utils/Rest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/utils/SharedLibraries.py` & `Nuitka-winsvc-1.7.6/nuitka/utils/SharedLibraries.py`

 * *Files 2% similar despite different names*

```diff
@@ -737,27 +737,40 @@
             continue
 
         result[os.path.basename(filename)] = filename
 
     return result
 
 
-def convertRPathToRunPath(filename):
+# spell-checker: ignore termux DT_RUNPATH
+_termux_elf_cleaner_usage = (
+    "Needs 'termux-elf-cleaner' to clean up created files. Install it for best results."
+)
+
+
+def cleanupHeaderForAndroid(filename):
     """Change a DT_RPATH to DT_RUNPATH
 
     On Android this seems required, because the linker doesn't support the one
     created by default.
     """
 
     with withEnvironmentVarOverridden("LANG", "C"):
         executeToolChecked(
             logger=postprocessing_logger,
             command=("patchelf", "--shrink-rpath", filename),
-            stderr_filter=_filterPatchelfErrorOutput,
             absence_message=_patchelf_usage,
+            stderr_filter=_filterPatchelfErrorOutput,
+        )
+
+        executeToolChecked(
+            logger=postprocessing_logger,
+            command=("termux-elf-cleaner", "--quiet", filename),
+            absence_message=_termux_elf_cleaner_usage,
+            optional=True,
         )
 
 
 _nm_usage = """\
 Error, needs 'nm' on your system, to detect exported DLL symbols."""
```

### Comparing `Nuitka-winsvc-1.7.5/nuitka/utils/Shebang.py` & `Nuitka-winsvc-1.7.6/nuitka/utils/Shebang.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/utils/Signing.py` & `Nuitka-winsvc-1.7.6/nuitka/utils/Signing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/utils/StaticLibraries.py` & `Nuitka-winsvc-1.7.6/nuitka/utils/StaticLibraries.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/utils/ThreadedExecutor.py` & `Nuitka-winsvc-1.7.6/nuitka/utils/ThreadedExecutor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/utils/Timing.py` & `Nuitka-winsvc-1.7.6/nuitka/utils/Timing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/utils/Utils.py` & `Nuitka-winsvc-1.7.6/nuitka/utils/Utils.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/utils/WindowsFileUsage.py` & `Nuitka-winsvc-1.7.6/nuitka/utils/WindowsFileUsage.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/utils/WindowsResources.py` & `Nuitka-winsvc-1.7.6/nuitka/utils/WindowsResources.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/utils/Yaml.py` & `Nuitka-winsvc-1.7.6/nuitka/utils/Yaml.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/nuitka/utils/__init__.py` & `Nuitka-winsvc-1.7.6/nuitka/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/pyproject.toml` & `Nuitka-winsvc-1.7.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/setup.py` & `Nuitka-winsvc-1.7.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -385,15 +385,14 @@
         "Topic :: Software Development :: Quality Assurance",
         # Nuitka standalone mode aims at distribution
         "Topic :: System :: Software Distribution",
         # Python2 supported versions.
         "Programming Language :: Python :: 2.6",
         "Programming Language :: Python :: 2.7",
         # Python3 supported versions.
-        "Programming Language :: Python :: 3.3",
         "Programming Language :: Python :: 3.4",
         "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
```

### Comparing `Nuitka-winsvc-1.7.5/tests/basics/AssertsTest.py` & `Nuitka-winsvc-1.7.6/tests/basics/AssertsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/basics/AssignmentsTest.py` & `Nuitka-winsvc-1.7.6/tests/basics/AssignmentsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/basics/AssignmentsTest32.py` & `Nuitka-winsvc-1.7.6/tests/basics/AssignmentsTest32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/basics/BranchingTest.py` & `Nuitka-winsvc-1.7.6/tests/basics/BranchingTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/basics/BuiltinOverload.py` & `Nuitka-winsvc-1.7.6/tests/basics/BuiltinOverload.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/basics/BuiltinSuperTest.py` & `Nuitka-winsvc-1.7.6/tests/basics/BuiltinSuperTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/basics/BuiltinsTest.py` & `Nuitka-winsvc-1.7.6/tests/basics/BuiltinsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/basics/ClassMinimalTest.py` & `Nuitka-winsvc-1.7.6/tests/basics/ClassMinimalTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/basics/ClassesTest.py` & `Nuitka-winsvc-1.7.6/tests/basics/ClassesTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/basics/ClassesTest32.py` & `Nuitka-winsvc-1.7.6/tests/basics/ClassesTest32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/basics/ClassesTest34.py` & `Nuitka-winsvc-1.7.6/tests/basics/ClassesTest34.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/basics/ComparisonChainsTest.py` & `Nuitka-winsvc-1.7.6/tests/basics/ComparisonChainsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/basics/ConstantsTest.py` & `Nuitka-winsvc-1.7.6/tests/basics/ConstantsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/basics/ConstantsTest27.py` & `Nuitka-winsvc-1.7.6/tests/basics/ConstantsTest27.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/basics/DecoratorsTest.py` & `Nuitka-winsvc-1.7.6/tests/basics/DecoratorsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/basics/DefaultParametersTest.py` & `Nuitka-winsvc-1.7.6/tests/basics/DefaultParametersTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/basics/DoubleDeletionsTest.py` & `Nuitka-winsvc-1.7.6/tests/basics/DoubleDeletionsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/basics/EmptyModuleTest.py` & `Nuitka-winsvc-1.7.6/tests/basics/EmptyModuleTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/basics/ExceptionRaisingTest.py` & `Nuitka-winsvc-1.7.6/tests/basics/ExceptionRaisingTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/basics/ExceptionRaisingTest32.py` & `Nuitka-winsvc-1.7.6/tests/basics/ExceptionRaisingTest32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/basics/ExceptionRaisingTest33.py` & `Nuitka-winsvc-1.7.6/tests/basics/ExceptionRaisingTest33.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/basics/ExecEvalTest.py` & `Nuitka-winsvc-1.7.6/tests/basics/ExecEvalTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/basics/ExtremeClosureTest.py` & `Nuitka-winsvc-1.7.6/tests/basics/ExtremeClosureTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/basics/FunctionObjectsTest.py` & `Nuitka-winsvc-1.7.6/tests/basics/FunctionObjectsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/basics/FunctionsTest.py` & `Nuitka-winsvc-1.7.6/tests/basics/FunctionsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/basics/FunctionsTest32.py` & `Nuitka-winsvc-1.7.6/tests/basics/FunctionsTest32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/basics/FunctionsTest_2.py` & `Nuitka-winsvc-1.7.6/tests/basics/FunctionsTest_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/basics/FutureTest32.py` & `Nuitka-winsvc-1.7.6/tests/basics/FutureTest32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/basics/GeneratorExpressionsTest.py` & `Nuitka-winsvc-1.7.6/tests/basics/GeneratorExpressionsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/basics/GeneratorExpressionsTest_37.py` & `Nuitka-winsvc-1.7.6/tests/basics/GeneratorExpressionsTest_37.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/basics/GlobalStatementTest.py` & `Nuitka-winsvc-1.7.6/tests/basics/GlobalStatementTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/basics/HelloWorldTest_2.py` & `Nuitka-winsvc-1.7.6/tests/basics/HelloWorldTest_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/basics/ImportingTest.py` & `Nuitka-winsvc-1.7.6/tests/basics/ImportingTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/basics/InplaceOperationsTest.py` & `Nuitka-winsvc-1.7.6/tests/basics/InplaceOperationsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/basics/InspectionTest.py` & `Nuitka-winsvc-1.7.6/tests/basics/InspectionTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/basics/InspectionTest_35.py` & `Nuitka-winsvc-1.7.6/tests/basics/InspectionTest_35.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/basics/InspectionTest_36.py` & `Nuitka-winsvc-1.7.6/tests/basics/InspectionTest_36.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/basics/LambdasTest.py` & `Nuitka-winsvc-1.7.6/tests/basics/LambdasTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/basics/LateClosureAssignmentTest.py` & `Nuitka-winsvc-1.7.6/tests/basics/LateClosureAssignmentTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/basics/ListContractionsTest.py` & `Nuitka-winsvc-1.7.6/tests/basics/ListContractionsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/basics/LoopingTest.py` & `Nuitka-winsvc-1.7.6/tests/basics/LoopingTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/basics/MainProgramsTest.py` & `Nuitka-winsvc-1.7.6/tests/basics/MainProgramsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/basics/ModuleAttributesTest.py` & `Nuitka-winsvc-1.7.6/tests/basics/ModuleAttributesTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/basics/OperatorsTest.py` & `Nuitka-winsvc-1.7.6/tests/basics/OperatorsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/basics/OrderChecksTest.py` & `Nuitka-winsvc-1.7.6/tests/basics/OrderChecksTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/basics/OrderChecksTest27.py` & `Nuitka-winsvc-1.7.6/tests/basics/OrderChecksTest27.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/basics/OverflowFunctionsTest_2.py` & `Nuitka-winsvc-1.7.6/tests/basics/OverflowFunctionsTest_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/basics/ParameterErrorsTest.py` & `Nuitka-winsvc-1.7.6/tests/basics/ParameterErrorsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/basics/ParameterErrorsTest32.py` & `Nuitka-winsvc-1.7.6/tests/basics/ParameterErrorsTest32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/basics/PrintFutureTest.py` & `Nuitka-winsvc-1.7.6/tests/basics/PrintFutureTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/basics/PrintingTest_2.py` & `Nuitka-winsvc-1.7.6/tests/basics/PrintingTest_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/basics/RecursionTest.py` & `Nuitka-winsvc-1.7.6/tests/basics/RecursionTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/basics/ReferencingTest.py` & `Nuitka-winsvc-1.7.6/tests/basics/ReferencingTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/basics/ReferencingTest27.py` & `Nuitka-winsvc-1.7.6/tests/basics/ReferencingTest27.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/basics/ReferencingTest33.py` & `Nuitka-winsvc-1.7.6/tests/basics/ReferencingTest33.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/basics/ReferencingTest35.py` & `Nuitka-winsvc-1.7.6/tests/basics/ReferencingTest35.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,15 @@
         return value
 
 
 def simpleFunction3():
     async def f():
         result = []
 
-        # Python 3.5 before 3.2 won't allow this.
+        # Python 3.5 before 3.5.2 won't allow this.
         try:
             async for letter in AsyncIteratorWrapper("abcdefg"):
                 result.append(letter)
         except TypeError:
             assert sys.version_info < (3, 5, 2)
 
         return result
```

### Comparing `Nuitka-winsvc-1.7.5/tests/basics/ReferencingTest36.py` & `Nuitka-winsvc-1.7.6/tests/basics/ReferencingTest36.py`

 * *Files 6% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         try:
             if exc:
                 exc = False
                 fut = coro.throw(AwaitException)
             else:
                 fut = coro.send(None)
         except StopIteration as ex:
-            return ex.args[0]
+            return ex.args[0] if ex.args else None
 
         if fut == ("throw",):
             exc = True
 
 
 def simpleFunction1():
     async def gen1():
@@ -77,15 +77,15 @@
             yield
         except:  # pylint: disable=bare-except
             pass
 
     async def run():
         g = gen1()
         await g.asend(None)
-        await g.asend(None)
+        await g.asend(2772)
 
     try:
         run_async(run())
     except StopAsyncIteration:
         pass
 
 
@@ -172,17 +172,39 @@
         rawdata = b"The quick brown fox jumps over the lazy dog.\r\n"
         # Be slow so we don't depend on other modules
         rawdata += bytes(range(256))
 
     return C()
 
 
+async def funcTrace1():
+    return [await awaitable() for _i in range(50)]
+
+
+def simpleFunction6():
+    run_async(funcTrace1())
+
+
+async def funcTrace2():
+    result = []
+
+    for _i in range(50):
+        value = await awaitable()
+        result.append(value)
+
+    return result
+
+
+def simpleFunction7():
+    run_async(funcTrace2())
+
+
 # This refleaks big time, but the construct is rare enough to not bother
 # as this proves hard to find.
-def disabled_simpleFunction6():
+def disabled_simpleFunction8():
     loop = asyncio.new_event_loop()
     asyncio.set_event_loop(None)
 
     async def waiter(timeout):
         await asyncio.sleep(timeout)
         yield 1
```

### Comparing `Nuitka-winsvc-1.7.5/tests/basics/ReferencingTest_2.py` & `Nuitka-winsvc-1.7.6/tests/basics/ReferencingTest_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/basics/SlotsTest.py` & `Nuitka-winsvc-1.7.6/tests/basics/SlotsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/basics/ThreadedGeneratorsTest.py` & `Nuitka-winsvc-1.7.6/tests/basics/ThreadedGeneratorsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/basics/TrickAssignmentsTest32.py` & `Nuitka-winsvc-1.7.6/tests/basics/TrickAssignmentsTest32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/basics/TrickAssignmentsTest35.py` & `Nuitka-winsvc-1.7.6/tests/basics/TrickAssignmentsTest35.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/basics/TrickAssignmentsTest_2.py` & `Nuitka-winsvc-1.7.6/tests/basics/TrickAssignmentsTest_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/basics/TryContinueFinallyTest.py` & `Nuitka-winsvc-1.7.6/tests/basics/TryContinueFinallyTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/basics/TryExceptContinueTest.py` & `Nuitka-winsvc-1.7.6/tests/basics/TryExceptContinueTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/basics/TryExceptFinallyTest.py` & `Nuitka-winsvc-1.7.6/tests/basics/TryExceptFinallyTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/basics/TryExceptFramesTest.py` & `Nuitka-winsvc-1.7.6/tests/basics/TryExceptFramesTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/basics/TryReturnFinallyTest.py` & `Nuitka-winsvc-1.7.6/tests/basics/TryReturnFinallyTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/basics/TryYieldFinallyTest.py` & `Nuitka-winsvc-1.7.6/tests/basics/TryYieldFinallyTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/basics/UnicodeTest.py` & `Nuitka-winsvc-1.7.6/tests/basics/UnicodeTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/basics/UnpackingTest35.py` & `Nuitka-winsvc-1.7.6/tests/basics/UnpackingTest35.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/basics/VarargsTest.py` & `Nuitka-winsvc-1.7.6/tests/basics/VarargsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/basics/WithStatementsTest.py` & `Nuitka-winsvc-1.7.6/tests/basics/WithStatementsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/basics/YieldFromTest33.py` & `Nuitka-winsvc-1.7.6/tests/basics/YieldFromTest33.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/basics/run_all.py` & `Nuitka-winsvc-1.7.6/tests/basics/run_all.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/basics/run_xml.py` & `Nuitka-winsvc-1.7.6/tests/basics/run_xml.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/onefile/HelloWorldTest.py` & `Nuitka-winsvc-1.7.6/tests/onefile/HelloWorldTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/onefile/KeyboardInterruptTest.py` & `Nuitka-winsvc-1.7.6/tests/onefile/KeyboardInterruptTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/onefile/run_all.py` & `Nuitka-winsvc-1.7.6/tests/onefile/run_all.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/optimizations/ArgumentTypes.py` & `Nuitka-winsvc-1.7.6/tests/optimizations/ArgumentTypes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/optimizations/Attributes.py` & `Nuitka-winsvc-1.7.6/tests/optimizations/Attributes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/optimizations/Calls.py` & `Nuitka-winsvc-1.7.6/tests/optimizations/Calls.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/optimizations/Conditions.py` & `Nuitka-winsvc-1.7.6/tests/optimizations/Conditions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/optimizations/DecodingOperations.py` & `Nuitka-winsvc-1.7.6/tests/optimizations/DecodingOperations.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/optimizations/FormatStrings36.py` & `Nuitka-winsvc-1.7.6/tests/optimizations/FormatStrings36.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/optimizations/HardImports.py` & `Nuitka-winsvc-1.7.6/tests/optimizations/HardImports.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/optimizations/HardImports_2.py` & `Nuitka-winsvc-1.7.6/tests/optimizations/HardImports_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/optimizations/Iterations.py` & `Nuitka-winsvc-1.7.6/tests/optimizations/Iterations.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/optimizations/Len.py` & `Nuitka-winsvc-1.7.6/tests/optimizations/Len.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/optimizations/Operations.py` & `Nuitka-winsvc-1.7.6/tests/optimizations/Operations.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/optimizations/Subscripts.py` & `Nuitka-winsvc-1.7.6/tests/optimizations/Subscripts.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/optimizations/run_all.py` & `Nuitka-winsvc-1.7.6/tests/optimizations/run_all.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/packages/package_import_success_after_failure/PackageImportSuccessAfterFailure.py` & `Nuitka-winsvc-1.7.6/tests/packages/package_import_success_after_failure/PackageImportSuccessAfterFailure.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/packages/package_import_success_after_failure/variable_package/SomeModule.py` & `Nuitka-winsvc-1.7.6/tests/packages/package_import_success_after_failure/variable_package/SomeModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/packages/package_import_success_after_failure/variable_package/__init__.py` & `Nuitka-winsvc-1.7.6/tests/packages/package_import_success_after_failure/variable_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/packages/run_all.py` & `Nuitka-winsvc-1.7.6/tests/packages/run_all.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/packages/sub_package/kitty/__init__.py` & `Nuitka-winsvc-1.7.6/tests/packages/sub_package/kitty/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/packages/sub_package/kitty/bigkitty.py` & `Nuitka-winsvc-1.7.6/tests/packages/sub_package/kitty/bigkitty.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/packages/sub_package/kitty/smallkitty.py` & `Nuitka-winsvc-1.7.6/tests/packages/sub_package/kitty/smallkitty.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/packages/sub_package/kitty/speak/__init__.py` & `Nuitka-winsvc-1.7.6/tests/packages/sub_package/kitty/speak/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/packages/sub_package/kitty/speak/hello.py` & `Nuitka-winsvc-1.7.6/tests/packages/sub_package/kitty/speak/hello.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/packages/sub_package/kitty/speak/miau.py` & `Nuitka-winsvc-1.7.6/tests/packages/sub_package/kitty/speak/miau.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/packages/sub_package/kitty/speak/purr.py` & `Nuitka-winsvc-1.7.6/tests/packages/sub_package/kitty/speak/purr.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/packages/top_level_attributes_3/some_package/__init__.py` & `Nuitka-winsvc-1.7.6/tests/packages/top_level_attributes_3/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/packages/top_level_attributes_3/some_package/some_module.py` & `Nuitka-winsvc-1.7.6/tests/packages/top_level_attributes_3/some_package/some_module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/plugins/code_signing/CodeSigningMain.py` & `Nuitka-winsvc-1.7.6/tests/plugins/code_signing/CodeSigningMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/plugins/data_files/DataFilesMain.py` & `Nuitka-winsvc-1.7.6/tests/plugins/data_files/DataFilesMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/plugins/data_files/data_files_package/__init__.py` & `Nuitka-winsvc-1.7.6/tests/plugins/data_files/data_files_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/plugins/parameters/ParametersMain.py` & `Nuitka-winsvc-1.7.6/tests/plugins/parameters/ParametersMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/plugins/parameters/parameter-using-plugin.py` & `Nuitka-winsvc-1.7.6/tests/plugins/parameters/parameter-using-plugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/plugins/run_all.py` & `Nuitka-winsvc-1.7.6/tests/plugins/run_all.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/absolute_import/AbsoluteImportMain.py` & `Nuitka-winsvc-1.7.6/tests/programs/absolute_import/AbsoluteImportMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/absolute_import/foobar/__init__.py` & `Nuitka-winsvc-1.7.6/tests/programs/absolute_import/foobar/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/absolute_import/foobar/foobar.py` & `Nuitka-winsvc-1.7.6/tests/programs/absolute_import/foobar/foobar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/absolute_import/foobar/local.py` & `Nuitka-winsvc-1.7.6/tests/programs/absolute_import/foobar/local.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/absolute_import/foobar/util.py` & `Nuitka-winsvc-1.7.6/tests/programs/absolute_import/foobar/util.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/case_imports1/CasedImportingMain.py` & `Nuitka-winsvc-1.7.6/tests/programs/case_imports1/CasedImportingMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/case_imports1/path1/Some_Module.py` & `Nuitka-winsvc-1.7.6/tests/programs/case_imports1/path1/Some_Module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/case_imports1/path1/Some_Package/__init__.py` & `Nuitka-winsvc-1.7.6/tests/programs/case_imports1/path1/Some_Package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/case_imports1/path2/some_module.py` & `Nuitka-winsvc-1.7.6/tests/programs/case_imports1/path2/some_module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/case_imports1/path2/some_package/__init__.py` & `Nuitka-winsvc-1.7.6/tests/programs/case_imports1/path2/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/case_imports2/CasedImportingMain.py` & `Nuitka-winsvc-1.7.6/tests/programs/case_imports2/CasedImportingMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/case_imports2/path1/some_module.py` & `Nuitka-winsvc-1.7.6/tests/programs/case_imports2/path1/some_module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/case_imports2/path1/some_package/__init__.py` & `Nuitka-winsvc-1.7.6/tests/programs/case_imports2/path1/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/case_imports2/path2/Some_Module.py` & `Nuitka-winsvc-1.7.6/tests/programs/case_imports2/path2/Some_Module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/case_imports2/path2/Some_Package/__init__.py` & `Nuitka-winsvc-1.7.6/tests/programs/case_imports2/path2/Some_Package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/case_imports3/CasedImportingMain.py` & `Nuitka-winsvc-1.7.6/tests/programs/case_imports3/CasedImportingMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/case_imports3/path1/Some_Module.py` & `Nuitka-winsvc-1.7.6/tests/programs/case_imports3/path1/Some_Module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/case_imports3/path1/Some_Package/__init__.py` & `Nuitka-winsvc-1.7.6/tests/programs/case_imports3/path1/Some_Package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/case_imports3/path2/Some_Module.py` & `Nuitka-winsvc-1.7.6/tests/programs/case_imports3/path2/Some_Module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/case_imports3/path2/Some_Package/__init__.py` & `Nuitka-winsvc-1.7.6/tests/programs/case_imports3/path2/Some_Package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/cyclic_imports/CyclicImportsMain.py` & `Nuitka-winsvc-1.7.6/tests/programs/cyclic_imports/CyclicImportsMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/cyclic_imports/cyclic_importing_package/Child1.py` & `Nuitka-winsvc-1.7.6/tests/programs/cyclic_imports/cyclic_importing_package/Child1.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/cyclic_imports/cyclic_importing_package/Child2.py` & `Nuitka-winsvc-1.7.6/tests/programs/cyclic_imports/cyclic_importing_package/Child2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/cyclic_imports/cyclic_importing_package/__init__.py` & `Nuitka-winsvc-1.7.6/tests/programs/cyclic_imports/cyclic_importing_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/dash_import/DashImportMain.py` & `Nuitka-winsvc-1.7.6/tests/programs/dash_import/DashImportMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/dash_import/dash-module.py` & `Nuitka-winsvc-1.7.6/tests/programs/dash_import/dash-module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/dash_import/plus+module.py` & `Nuitka-winsvc-1.7.6/tests/programs/dash_import/plus+module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/dash_main/Dash-Main.py` & `Nuitka-winsvc-1.7.6/tests/programs/dash_main/Dash-Main.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/deep/DeepProgramMain.py` & `Nuitka-winsvc-1.7.6/tests/programs/deep/DeepProgramMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/deep/some_package/DeepBrother.py` & `Nuitka-winsvc-1.7.6/tests/programs/deep/some_package/DeepBrother.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/deep/some_package/DeepChild.py` & `Nuitka-winsvc-1.7.6/tests/programs/deep/some_package/DeepChild.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/deep/some_package/__init__.py` & `Nuitka-winsvc-1.7.6/tests/programs/deep/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/deep/some_package/deep_package/DeepDeepChild.py` & `Nuitka-winsvc-1.7.6/tests/programs/deep/some_package/deep_package/DeepDeepChild.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/deep/some_package/deep_package/__init__.py` & `Nuitka-winsvc-1.7.6/tests/programs/deep/some_package/deep_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/dunderinit_imports/DunderInitImportsMain.py` & `Nuitka-winsvc-1.7.6/tests/programs/dunderinit_imports/DunderInitImportsMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/dunderinit_imports/package/SubModule.py` & `Nuitka-winsvc-1.7.6/tests/programs/dunderinit_imports/package/SubModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/dunderinit_imports/package/__init__.py` & `Nuitka-winsvc-1.7.6/tests/programs/dunderinit_imports/package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/import_variants/ImportVariationsMain.py` & `Nuitka-winsvc-1.7.6/tests/programs/import_variants/ImportVariationsMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/import_variants/some_package/Child1.py` & `Nuitka-winsvc-1.7.6/tests/programs/import_variants/some_package/Child1.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/import_variants/some_package/Child2.py` & `Nuitka-winsvc-1.7.6/tests/programs/import_variants/some_package/Child2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/import_variants/some_package/Child3.py` & `Nuitka-winsvc-1.7.6/tests/programs/import_variants/some_package/Child3.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/import_variants/some_package/__init__.py` & `Nuitka-winsvc-1.7.6/tests/programs/import_variants/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/main_raises/ErrorMain.py` & `Nuitka-winsvc-1.7.6/tests/programs/main_raises/ErrorMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/main_raises/ErrorRaising.py` & `Nuitka-winsvc-1.7.6/tests/programs/main_raises/ErrorRaising.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/main_raises2/ErrorInFunctionMain.py` & `Nuitka-winsvc-1.7.6/tests/programs/main_raises2/ErrorInFunctionMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/main_raises2/ErrorRaising.py` & `Nuitka-winsvc-1.7.6/tests/programs/main_raises2/ErrorRaising.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/module_attributes/ModuleAttributesMain.py` & `Nuitka-winsvc-1.7.6/tests/programs/module_attributes/ModuleAttributesMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/module_attributes/package_level1/Nearby1.py` & `Nuitka-winsvc-1.7.6/tests/programs/module_attributes/package_level1/Nearby1.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/module_attributes/package_level1/__init__.py` & `Nuitka-winsvc-1.7.6/tests/programs/module_attributes/package_level1/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/module_attributes/package_level1/package_level2/Nearby2.py` & `Nuitka-winsvc-1.7.6/tests/programs/module_attributes/package_level1/package_level2/Nearby2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/module_attributes/package_level1/package_level2/__init__.py` & `Nuitka-winsvc-1.7.6/tests/programs/module_attributes/package_level1/package_level2/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/module_attributes/package_level1/package_level2/package_level3/Nearby3.py` & `Nuitka-winsvc-1.7.6/tests/programs/module_attributes/package_level1/package_level2/package_level3/Nearby3.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/module_attributes/package_level1/package_level2/package_level3/__init__.py` & `Nuitka-winsvc-1.7.6/tests/programs/module_attributes/package_level1/package_level2/package_level3/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/module_exits/ErrorExitingModule.py` & `Nuitka-winsvc-1.7.6/tests/programs/module_exits/ErrorExitingModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/module_exits/Main.py` & `Nuitka-winsvc-1.7.6/tests/programs/module_exits/Main.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/module_object_replacing/ModuleObjectReplacingMain.py` & `Nuitka-winsvc-1.7.6/tests/programs/module_object_replacing/ModuleObjectReplacingMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/module_object_replacing/SelfReplacingModule.py` & `Nuitka-winsvc-1.7.6/tests/programs/module_object_replacing/SelfReplacingModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/multiprocessing_using/MultiprocessingUsingMain.py` & `Nuitka-winsvc-1.7.6/tests/programs/multiprocessing_using/MultiprocessingUsingMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/multiprocessing_using/foo/__init__.py` & `Nuitka-winsvc-1.7.6/tests/programs/multiprocessing_using/foo/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/multiprocessing_using/foo/__main__.py` & `Nuitka-winsvc-1.7.6/tests/programs/multiprocessing_using/foo/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/multiprocessing_using/foo/entry.py` & `Nuitka-winsvc-1.7.6/tests/programs/multiprocessing_using/foo/entry.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/named_imports/NamedImportsMain.py` & `Nuitka-winsvc-1.7.6/tests/programs/named_imports/NamedImportsMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/named_imports/some_package/SomeModule.py` & `Nuitka-winsvc-1.7.6/tests/programs/named_imports/some_package/SomeModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/named_imports/some_package/__init__.py` & `Nuitka-winsvc-1.7.6/tests/programs/named_imports/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/named_imports/some_package/sub_package/SomeModule.py` & `Nuitka-winsvc-1.7.6/tests/programs/named_imports/some_package/sub_package/SomeModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/package_code/PackageInitCodeMain.py` & `Nuitka-winsvc-1.7.6/tests/programs/package_code/PackageInitCodeMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/package_code/some_package/SomeModule.py` & `Nuitka-winsvc-1.7.6/tests/programs/package_code/some_package/SomeModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/package_code/some_package/__init__.py` & `Nuitka-winsvc-1.7.6/tests/programs/package_code/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/package_contains_main/PackageContainsMain.py` & `Nuitka-winsvc-1.7.6/tests/programs/package_contains_main/PackageContainsMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/package_contains_main/__init__.py` & `Nuitka-winsvc-1.7.6/tests/programs/package_contains_main/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/package_contains_main/local.py` & `Nuitka-winsvc-1.7.6/tests/programs/package_contains_main/local.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/package_init_import/PackageInitImportMain.py` & `Nuitka-winsvc-1.7.6/tests/programs/package_init_import/PackageInitImportMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/package_init_import/some_package/PackageLocal.py` & `Nuitka-winsvc-1.7.6/tests/programs/package_init_import/some_package/PackageLocal.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/package_init_import/some_package/__init__.py` & `Nuitka-winsvc-1.7.6/tests/programs/package_init_import/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/package_init_issue/PackageInitIssueMain.py` & `Nuitka-winsvc-1.7.6/tests/programs/package_init_issue/PackageInitIssueMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/package_init_issue/some_package/__init__.py` & `Nuitka-winsvc-1.7.6/tests/programs/package_init_issue/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/package_init_issue/some_package/child_package/SomeModule.py` & `Nuitka-winsvc-1.7.6/tests/programs/package_init_issue/some_package/child_package/SomeModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/package_init_issue/some_package/child_package/__init__.py` & `Nuitka-winsvc-1.7.6/tests/programs/package_init_issue/some_package/child_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/package_missing_init/PackageMissingInitMain.py` & `Nuitka-winsvc-1.7.6/tests/programs/package_missing_init/PackageMissingInitMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/package_missing_init/some_package/some_module.py` & `Nuitka-winsvc-1.7.6/tests/programs/package_missing_init/some_package/some_module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/package_missing_init/some_package/sub_package/some_sub_module.py` & `Nuitka-winsvc-1.7.6/tests/programs/package_missing_init/some_package/sub_package/some_sub_module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/package_module_collision/PackageAndModuleNamedSameMain.py` & `Nuitka-winsvc-1.7.6/tests/programs/package_module_collision/PackageAndModuleNamedSameMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/package_module_collision/Something/__init__.py` & `Nuitka-winsvc-1.7.6/tests/programs/package_module_collision/Something/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/package_module_collision/something.py` & `Nuitka-winsvc-1.7.6/tests/programs/package_module_collision/something.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/package_overload/Main.py` & `Nuitka-winsvc-1.7.6/tests/programs/package_overload/Main.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/package_overload/foo/__init__.py` & `Nuitka-winsvc-1.7.6/tests/programs/package_overload/foo/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/package_overload/foo/bar.py` & `Nuitka-winsvc-1.7.6/tests/programs/package_overload/foo/bar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/package_overload/foo/bar2.py` & `Nuitka-winsvc-1.7.6/tests/programs/package_overload/foo/bar2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/package_prevents_submodule/PackagePreventsSubmoduleMain.py` & `Nuitka-winsvc-1.7.6/tests/programs/package_prevents_submodule/PackagePreventsSubmoduleMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/package_prevents_submodule/some_package/__init__.py` & `Nuitka-winsvc-1.7.6/tests/programs/package_prevents_submodule/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/package_prevents_submodule/some_package/some_module.py` & `Nuitka-winsvc-1.7.6/tests/programs/package_prevents_submodule/some_package/some_module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/package_program/PackageAsMain/__init__.py` & `Nuitka-winsvc-1.7.6/tests/programs/package_program/PackageAsMain/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/package_program/PackageAsMain/__main__.py` & `Nuitka-winsvc-1.7.6/tests/programs/package_program/PackageAsMain/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/pkgutil_itermodules/PkgUtilIterModulesMain.py` & `Nuitka-winsvc-1.7.6/tests/programs/pkgutil_itermodules/PkgUtilIterModulesMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/pkgutil_itermodules/some_package/__init__.py` & `Nuitka-winsvc-1.7.6/tests/programs/pkgutil_itermodules/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleC.py` & `Nuitka-winsvc-1.7.6/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleC.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleD.py` & `Nuitka-winsvc-1.7.6/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleD.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/pkgutil_itermodules/some_package/sub_package1/__init__.py` & `Nuitka-winsvc-1.7.6/tests/programs/pkgutil_itermodules/some_package/sub_package1/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleA.py` & `Nuitka-winsvc-1.7.6/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleA.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleB.py` & `Nuitka-winsvc-1.7.6/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleB.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/pkgutil_itermodules/some_package/sub_package2/__init__.py` & `Nuitka-winsvc-1.7.6/tests/programs/pkgutil_itermodules/some_package/sub_package2/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/pkgutil_usage/PkgUtilUsageMain.py` & `Nuitka-winsvc-1.7.6/tests/programs/pkgutil_usage/PkgUtilUsageMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/pkgutil_usage/package/__init__.py` & `Nuitka-winsvc-1.7.6/tests/programs/pkgutil_usage/package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/plugin_import/PluginImportMain.py` & `Nuitka-winsvc-1.7.6/tests/programs/plugin_import/PluginImportMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/plugin_import/some_package/__init__.py` & `Nuitka-winsvc-1.7.6/tests/programs/plugin_import/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/plugin_import/some_package/some_module.py` & `Nuitka-winsvc-1.7.6/tests/programs/plugin_import/some_package/some_module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/reimport_main_dynamic/ImportItselfDynamicMain.py` & `Nuitka-winsvc-1.7.6/tests/programs/reimport_main_dynamic/ImportItselfDynamicMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/reimport_main_static/ImportItselfStaticMain.py` & `Nuitka-winsvc-1.7.6/tests/programs/reimport_main_static/ImportItselfStaticMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/relative_import/RelativeImportMain.py` & `Nuitka-winsvc-1.7.6/tests/programs/relative_import/RelativeImportMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/relative_import/dircache.py` & `Nuitka-winsvc-1.7.6/tests/programs/relative_import/dircache.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/resource_reader37/ResourceReaderMain.py` & `Nuitka-winsvc-1.7.6/tests/programs/resource_reader37/ResourceReaderMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/resource_reader37/some_package/__init__.py` & `Nuitka-winsvc-1.7.6/tests/programs/resource_reader37/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/run_all.py` & `Nuitka-winsvc-1.7.6/tests/programs/run_all.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/stdlib_overload/StdlibOverloadMain.py` & `Nuitka-winsvc-1.7.6/tests/programs/stdlib_overload/StdlibOverloadMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/stdlib_overload/pyexpat.py` & `Nuitka-winsvc-1.7.6/tests/programs/stdlib_overload/pyexpat.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/stdlib_overload/some_package/__init__.py` & `Nuitka-winsvc-1.7.6/tests/programs/stdlib_overload/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/stdlib_overload/some_package/normal_importing.py` & `Nuitka-winsvc-1.7.6/tests/programs/stdlib_overload/some_package/normal_importing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/stdlib_overload/some_package/pyexpat.py` & `Nuitka-winsvc-1.7.6/tests/programs/stdlib_overload/some_package/pyexpat.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/stdlib_overload/some_package/star_importing.py` & `Nuitka-winsvc-1.7.6/tests/programs/stdlib_overload/some_package/star_importing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/syntax_errors/IndentationErroring.py` & `Nuitka-winsvc-1.7.6/tests/programs/syntax_errors/IndentationErroring.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/syntax_errors/SyntaxErroring.py` & `Nuitka-winsvc-1.7.6/tests/programs/syntax_errors/SyntaxErroring.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/syntax_errors/SyntaxErrorsMain.py` & `Nuitka-winsvc-1.7.6/tests/programs/syntax_errors/SyntaxErrorsMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/unicode_bom/UnicodeBomMain.py` & `Nuitka-winsvc-1.7.6/tests/programs/unicode_bom/UnicodeBomMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/unicode_bom/unicode_bom.py` & `Nuitka-winsvc-1.7.6/tests/programs/unicode_bom/unicode_bom.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/programs/with space/Space Main.py` & `Nuitka-winsvc-1.7.6/tests/programs/with space/Space Main.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/reflected/compile_itself.py` & `Nuitka-winsvc-1.7.6/tests/reflected/compile_itself.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/run-tests` & `Nuitka-winsvc-1.7.6/tests/run-tests`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/standalone/BrotliUsing.py` & `Nuitka-winsvc-1.7.6/tests/standalone/BrotliUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/standalone/CtypesUsing.py` & `Nuitka-winsvc-1.7.6/tests/standalone/CtypesUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/standalone/FlaskUsing.py` & `Nuitka-winsvc-1.7.6/tests/standalone/FlaskUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/standalone/GlfwUsing.py` & `Nuitka-winsvc-1.7.6/tests/standalone/GlfwUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/standalone/GtkUsing.py` & `Nuitka-winsvc-1.7.6/tests/standalone/GtkUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/standalone/HexEncodingTest_2.py` & `Nuitka-winsvc-1.7.6/tests/standalone/HexEncodingTest_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/standalone/IdnaUsing.py` & `Nuitka-winsvc-1.7.6/tests/standalone/IdnaUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/standalone/LxmlUsing.py` & `Nuitka-winsvc-1.7.6/tests/standalone/LxmlUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/standalone/MatplotlibUsing.py` & `Nuitka-winsvc-1.7.6/tests/standalone/MatplotlibUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/standalone/MetadataPackagesUsing.py` & `Nuitka-winsvc-1.7.6/tests/standalone/MetadataPackagesUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/standalone/NumpyUsing.py` & `Nuitka-winsvc-1.7.6/tests/standalone/NumpyUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/standalone/OpenGLUsing.py` & `Nuitka-winsvc-1.7.6/tests/standalone/OpenGLUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/standalone/PandasUsing.py` & `Nuitka-winsvc-1.7.6/tests/standalone/PandasUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/standalone/PasslibUsing.py` & `Nuitka-winsvc-1.7.6/tests/standalone/PasslibUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/standalone/PendulumUsing.py` & `Nuitka-winsvc-1.7.6/tests/standalone/PendulumUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/standalone/PkgResourcesRequiresUsing.py` & `Nuitka-winsvc-1.7.6/tests/standalone/PkgResourcesRequiresUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/standalone/PmwUsing.py` & `Nuitka-winsvc-1.7.6/tests/standalone/PmwUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/standalone/PyQt5Plugins.py` & `Nuitka-winsvc-1.7.6/tests/standalone/PyQt5Plugins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/standalone/PyQt5SSLSupport.py` & `Nuitka-winsvc-1.7.6/tests/standalone/PyQt5SSLSupport.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/standalone/PyQt5Using.py` & `Nuitka-winsvc-1.7.6/tests/standalone/PyQt5Using.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/standalone/PyQt6Plugins.py` & `Nuitka-winsvc-1.7.6/tests/standalone/PyQt6Plugins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/standalone/PyQt6Using.py` & `Nuitka-winsvc-1.7.6/tests/standalone/PyQt6Using.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/standalone/PySide6Plugins.py` & `Nuitka-winsvc-1.7.6/tests/standalone/PySide6Plugins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/standalone/PySide6Using.py` & `Nuitka-winsvc-1.7.6/tests/standalone/PySide6Using.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/standalone/RsaUsing.py` & `Nuitka-winsvc-1.7.6/tests/standalone/RsaUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/standalone/ShlibUsing.py` & `Nuitka-winsvc-1.7.6/tests/standalone/ShlibUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/standalone/SocketUsing.py` & `Nuitka-winsvc-1.7.6/tests/standalone/SocketUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/standalone/TkInterUsing.py` & `Nuitka-winsvc-1.7.6/tests/standalone/TkInterUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/standalone/Urllib3Using.py` & `Nuitka-winsvc-1.7.6/tests/standalone/Urllib3Using.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/standalone/Win32ComUsing.py` & `Nuitka-winsvc-1.7.6/tests/standalone/Win32ComUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/standalone/run_all.py` & `Nuitka-winsvc-1.7.6/tests/standalone/run_all.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/standalone/zip_importer/ZipImporterMain.py` & `Nuitka-winsvc-1.7.6/tests/standalone/zip_importer/ZipImporterMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/syntax/AsyncgenReturn36.py` & `Nuitka-winsvc-1.7.6/tests/syntax/AsyncgenReturn36.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/syntax/BreakWithoutLoop.py` & `Nuitka-winsvc-1.7.6/tests/syntax/BreakWithoutLoop.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/syntax/ClassReturn.py` & `Nuitka-winsvc-1.7.6/tests/syntax/ClassReturn.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/syntax/ClosureDel_2.py` & `Nuitka-winsvc-1.7.6/tests/syntax/ClosureDel_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/syntax/ContinueWithoutLoop.py` & `Nuitka-winsvc-1.7.6/tests/syntax/ContinueWithoutLoop.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/syntax/DuplicateArgument.py` & `Nuitka-winsvc-1.7.6/tests/syntax/DuplicateArgument.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/syntax/ExecWithNesting_2.py` & `Nuitka-winsvc-1.7.6/tests/syntax/ExecWithNesting_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/syntax/FutureBraces.py` & `Nuitka-winsvc-1.7.6/tests/syntax/FutureBraces.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/syntax/FutureUnknown.py` & `Nuitka-winsvc-1.7.6/tests/syntax/FutureUnknown.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/syntax/GeneratorExpressions38.py` & `Nuitka-winsvc-1.7.6/tests/syntax/GeneratorExpressions38.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/syntax/GeneratorReturn_2.py` & `Nuitka-winsvc-1.7.6/tests/syntax/GeneratorReturn_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/syntax/GlobalForParameter.py` & `Nuitka-winsvc-1.7.6/tests/syntax/GlobalForParameter.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/syntax/Importing32.py` & `Nuitka-winsvc-1.7.6/tests/syntax/Importing32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/syntax/IndentationError.py` & `Nuitka-winsvc-1.7.6/tests/syntax/IndentationError.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/syntax/LateFutureImport.py` & `Nuitka-winsvc-1.7.6/tests/syntax/LateFutureImport.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/syntax/MisplacedFutureImport.py` & `Nuitka-winsvc-1.7.6/tests/syntax/MisplacedFutureImport.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/syntax/ModuleReturn.py` & `Nuitka-winsvc-1.7.6/tests/syntax/ModuleReturn.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/syntax/NonAsciiWithoutEncoding_2.py` & `Nuitka-winsvc-1.7.6/tests/syntax/NonAsciiWithoutEncoding_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/syntax/NonlocalForParameter32.py` & `Nuitka-winsvc-1.7.6/tests/syntax/NonlocalForParameter32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/syntax/NonlocalNotFound32.py` & `Nuitka-winsvc-1.7.6/tests/syntax/NonlocalNotFound32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/syntax/StarImportExtra.py` & `Nuitka-winsvc-1.7.6/tests/syntax/StarImportExtra.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/syntax/SyntaxError.py` & `Nuitka-winsvc-1.7.6/tests/syntax/SyntaxError.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/syntax/TryExceptAllNotLast.py` & `Nuitka-winsvc-1.7.6/tests/syntax/TryExceptAllNotLast.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/syntax/TryFinallyContinue_37.py` & `Nuitka-winsvc-1.7.6/tests/syntax/TryFinallyContinue_37.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/syntax/UnpackNoTuple.py` & `Nuitka-winsvc-1.7.6/tests/syntax/UnpackNoTuple.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/syntax/UnpackTwoStars32.py` & `Nuitka-winsvc-1.7.6/tests/syntax/UnpackTwoStars32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/syntax/YieldFromInModule.py` & `Nuitka-winsvc-1.7.6/tests/syntax/YieldFromInModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/syntax/YieldInAsync35.py` & `Nuitka-winsvc-1.7.6/tests/syntax/YieldInAsync35.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/syntax/YieldInGenexp38.py` & `Nuitka-winsvc-1.7.6/tests/syntax/YieldInGenexp38.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/syntax/YieldInModule.py` & `Nuitka-winsvc-1.7.6/tests/syntax/YieldInModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.7.5/tests/syntax/run_all.py` & `Nuitka-winsvc-1.7.6/tests/syntax/run_all.py`

 * *Files identical despite different names*

