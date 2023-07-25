# Comparing `tmp/seismic-rna-0.4.1.tar.gz` & `tmp/seismic-rna-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seismic-rna-0.4.1.tar", last modified: Fri Jul 21 02:50:00 2023, max compression
+gzip compressed data, was "seismic-rna-0.5.0.tar", last modified: Tue Jul 25 02:02:28 2023, max compression
```

## Comparing `seismic-rna-0.4.1.tar` & `seismic-rna-0.5.0.tar`

### file list

```diff
@@ -1,118 +1,124 @@
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-21 02:50:00.061316 seismic-rna-0.4.1/
--rw-r--r--   0 mfa        (503) staff       (20)    35150 2023-06-29 02:33:57.000000 seismic-rna-0.4.1/LICENSE
--rw-r--r--   0 mfa        (503) staff       (20)     1910 2023-07-21 02:50:00.060911 seismic-rna-0.4.1/PKG-INFO
--rw-r--r--   0 mfa        (503) staff       (20)     1347 2023-07-19 21:38:18.000000 seismic-rna-0.4.1/README.md
--rw-r--r--   0 mfa        (503) staff       (20)     1037 2023-07-21 02:49:16.000000 seismic-rna-0.4.1/pyproject.toml
--rw-r--r--   0 mfa        (503) staff       (20)       38 2023-07-21 02:50:00.061411 seismic-rna-0.4.1/setup.cfg
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-21 02:49:59.934843 seismic-rna-0.4.1/src/
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-21 02:49:59.946192 seismic-rna-0.4.1/src/seismic_rna.egg-info/
--rw-r--r--   0 mfa        (503) staff       (20)     1910 2023-07-21 02:49:59.000000 seismic-rna-0.4.1/src/seismic_rna.egg-info/PKG-INFO
--rw-r--r--   0 mfa        (503) staff       (20)     3039 2023-07-21 02:49:59.000000 seismic-rna-0.4.1/src/seismic_rna.egg-info/SOURCES.txt
--rw-r--r--   0 mfa        (503) staff       (20)        1 2023-07-21 02:49:59.000000 seismic-rna-0.4.1/src/seismic_rna.egg-info/dependency_links.txt
--rw-r--r--   0 mfa        (503) staff       (20)       53 2023-07-21 02:49:59.000000 seismic-rna-0.4.1/src/seismic_rna.egg-info/entry_points.txt
--rw-r--r--   0 mfa        (503) staff       (20)      176 2023-07-21 02:49:59.000000 seismic-rna-0.4.1/src/seismic_rna.egg-info/requires.txt
--rw-r--r--   0 mfa        (503) staff       (20)       11 2023-07-21 02:49:59.000000 seismic-rna-0.4.1/src/seismic_rna.egg-info/top_level.txt
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-21 02:49:59.948989 seismic-rna-0.4.1/src/seismicrna/
--rw-r--r--   0 mfa        (503) staff       (20)      201 2023-07-16 01:27:23.000000 seismic-rna-0.4.1/src/seismicrna/__init__.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-21 02:49:59.955338 seismic-rna-0.4.1/src/seismicrna/align/
--rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.4.1/src/seismicrna/align/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)    22758 2023-07-05 00:01:54.000000 seismic-rna-0.4.1/src/seismicrna/align/fq2bam.py
--rwxr-xr-x   0 mfa        (503) staff       (20)    20020 2023-07-09 17:46:17.000000 seismic-rna-0.4.1/src/seismicrna/align/fqutil.py
--rw-r--r--   0 mfa        (503) staff       (20)     7600 2023-07-20 02:53:44.000000 seismic-rna-0.4.1/src/seismicrna/align/main.py
--rwxr-xr-x   0 mfa        (503) staff       (20)     9115 2023-06-29 02:17:49.000000 seismic-rna-0.4.1/src/seismicrna/align/strandedness.py
--rw-r--r--   0 mfa        (503) staff       (20)        0 2023-06-29 02:17:49.000000 seismic-rna-0.4.1/src/seismicrna/align/test.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-21 02:49:59.962752 seismic-rna-0.4.1/src/seismicrna/cluster/
--rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.4.1/src/seismicrna/cluster/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)    13197 2023-07-15 21:12:26.000000 seismic-rna-0.4.1/src/seismicrna/cluster/compare.py
--rw-r--r--   0 mfa        (503) staff       (20)    18681 2023-06-29 02:17:49.000000 seismic-rna-0.4.1/src/seismicrna/cluster/em.py
--rw-r--r--   0 mfa        (503) staff       (20)     6262 2023-06-29 02:17:49.000000 seismic-rna-0.4.1/src/seismicrna/cluster/krun.py
--rw-r--r--   0 mfa        (503) staff       (20)     4209 2023-06-29 02:17:49.000000 seismic-rna-0.4.1/src/seismicrna/cluster/load.py
--rw-r--r--   0 mfa        (503) staff       (20)     2464 2023-07-16 00:26:28.000000 seismic-rna-0.4.1/src/seismicrna/cluster/main.py
--rw-r--r--   0 mfa        (503) staff       (20)     1264 2023-07-15 00:22:05.000000 seismic-rna-0.4.1/src/seismicrna/cluster/names.py
--rw-r--r--   0 mfa        (503) staff       (20)     2862 2023-06-29 02:17:49.000000 seismic-rna-0.4.1/src/seismicrna/cluster/report.py
--rw-r--r--   0 mfa        (503) staff       (20)     4981 2023-06-29 02:17:49.000000 seismic-rna-0.4.1/src/seismicrna/cluster/write.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-21 02:49:59.994103 seismic-rna-0.4.1/src/seismicrna/core/
--rw-r--r--   0 mfa        (503) staff       (20)        0 2023-06-29 02:17:49.000000 seismic-rna-0.4.1/src/seismicrna/core/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)    15704 2023-06-29 18:01:10.000000 seismic-rna-0.4.1/src/seismicrna/core/bitcall.py
--rw-r--r--   0 mfa        (503) staff       (20)    19264 2023-07-07 22:07:51.000000 seismic-rna-0.4.1/src/seismicrna/core/bitvect.py
--rw-r--r--   0 mfa        (503) staff       (20)    18165 2023-07-19 23:10:51.000000 seismic-rna-0.4.1/src/seismicrna/core/cli.py
--rw-r--r--   0 mfa        (503) staff       (20)     1120 2023-06-29 21:48:51.000000 seismic-rna-0.4.1/src/seismicrna/core/depend.py
--rw-r--r--   0 mfa        (503) staff       (20)     6844 2023-06-29 02:17:49.000000 seismic-rna-0.4.1/src/seismicrna/core/docdef.py
--rw-r--r--   0 mfa        (503) staff       (20)     2201 2023-06-29 02:17:49.000000 seismic-rna-0.4.1/src/seismicrna/core/docstring.py
--rw-r--r--   0 mfa        (503) staff       (20)     1972 2023-06-29 02:17:49.000000 seismic-rna-0.4.1/src/seismicrna/core/dump.py
--rw-r--r--   0 mfa        (503) staff       (20)      628 2023-06-29 02:17:49.000000 seismic-rna-0.4.1/src/seismicrna/core/files.py
--rw-r--r--   0 mfa        (503) staff       (20)     7933 2023-07-07 22:47:51.000000 seismic-rna-0.4.1/src/seismicrna/core/load.py
--rw-r--r--   0 mfa        (503) staff       (20)     2837 2023-07-07 02:37:13.000000 seismic-rna-0.4.1/src/seismicrna/core/logs.py
--rw-r--r--   0 mfa        (503) staff       (20)    14124 2023-06-29 02:17:49.000000 seismic-rna-0.4.1/src/seismicrna/core/mu.py
--rw-r--r--   0 mfa        (503) staff       (20)    10537 2023-06-30 18:53:43.000000 seismic-rna-0.4.1/src/seismicrna/core/mu_test.py
--rw-r--r--   0 mfa        (503) staff       (20)    14509 2023-07-12 20:28:15.000000 seismic-rna-0.4.1/src/seismicrna/core/parallel.py
--rw-r--r--   0 mfa        (503) staff       (20)    23511 2023-07-07 00:11:58.000000 seismic-rna-0.4.1/src/seismicrna/core/path.py
--rw-r--r--   0 mfa        (503) staff       (20)    29387 2023-07-14 20:09:45.000000 seismic-rna-0.4.1/src/seismicrna/core/rel.py
--rw-r--r--   0 mfa        (503) staff       (20)    45953 2023-06-30 18:58:01.000000 seismic-rna-0.4.1/src/seismicrna/core/rel_test.py
--rw-r--r--   0 mfa        (503) staff       (20)    29740 2023-07-12 04:26:52.000000 seismic-rna-0.4.1/src/seismicrna/core/report.py
--rw-r--r--   0 mfa        (503) staff       (20)     9169 2023-06-29 02:17:49.000000 seismic-rna-0.4.1/src/seismicrna/core/rna.py
--rw-r--r--   0 mfa        (503) staff       (20)    27329 2023-07-09 16:52:06.000000 seismic-rna-0.4.1/src/seismicrna/core/sect.py
--rw-r--r--   0 mfa        (503) staff       (20)     7101 2023-07-06 00:49:26.000000 seismic-rna-0.4.1/src/seismicrna/core/sect_test.py
--rw-r--r--   0 mfa        (503) staff       (20)     9798 2023-06-30 03:50:29.000000 seismic-rna-0.4.1/src/seismicrna/core/seq.py
--rw-r--r--   0 mfa        (503) staff       (20)     6634 2023-06-30 14:56:23.000000 seismic-rna-0.4.1/src/seismicrna/core/seq_test.py
--rw-r--r--   0 mfa        (503) staff       (20)     2799 2023-06-29 21:49:14.000000 seismic-rna-0.4.1/src/seismicrna/core/shell.py
--rw-r--r--   0 mfa        (503) staff       (20)     1054 2023-06-29 19:54:35.000000 seismic-rna-0.4.1/src/seismicrna/core/sim.py
--rw-r--r--   0 mfa        (503) staff       (20)      769 2023-07-06 00:49:45.000000 seismic-rna-0.4.1/src/seismicrna/core/sim_test.py
--rw-r--r--   0 mfa        (503) staff       (20)      758 2023-06-29 02:17:49.000000 seismic-rna-0.4.1/src/seismicrna/core/types.py
--rwxr-xr-x   0 mfa        (503) staff       (20)    14291 2023-06-30 03:36:23.000000 seismic-rna-0.4.1/src/seismicrna/core/xam.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-21 02:49:59.998782 seismic-rna-0.4.1/src/seismicrna/demult/
--rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.4.1/src/seismicrna/demult/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)    42624 2023-07-19 22:35:50.000000 seismic-rna-0.4.1/src/seismicrna/demult/demultiplex.py
--rw-r--r--   0 mfa        (503) staff       (20)     2103 2023-07-19 22:35:50.000000 seismic-rna-0.4.1/src/seismicrna/demult/main.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-21 02:50:00.009013 seismic-rna-0.4.1/src/seismicrna/draw/
--rw-r--r--   0 mfa        (503) staff       (20)      256 2023-06-29 19:38:33.000000 seismic-rna-0.4.1/src/seismicrna/draw/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)      225 2023-06-29 02:17:49.000000 seismic-rna-0.4.1/src/seismicrna/draw/load_dataset.py
--rw-r--r--   0 mfa        (503) staff       (20)     6013 2023-06-29 02:17:49.000000 seismic-rna-0.4.1/src/seismicrna/draw/main.py
--rw-r--r--   0 mfa        (503) staff       (20)     6656 2023-06-29 02:17:49.000000 seismic-rna-0.4.1/src/seismicrna/draw/manipulator.py
--rw-r--r--   0 mfa        (503) staff       (20)    17447 2023-06-29 19:43:29.000000 seismic-rna-0.4.1/src/seismicrna/draw/plotter.py
--rw-r--r--   0 mfa        (503) staff       (20)    15931 2023-06-29 02:17:49.000000 seismic-rna-0.4.1/src/seismicrna/draw/study.py
--rw-r--r--   0 mfa        (503) staff       (20)    11285 2023-06-29 02:17:49.000000 seismic-rna-0.4.1/src/seismicrna/draw/util.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-21 02:50:00.021994 seismic-rna-0.4.1/src/seismicrna/graph/
--rw-r--r--   0 mfa        (503) staff       (20)       22 2023-06-29 02:17:49.000000 seismic-rna-0.4.1/src/seismicrna/graph/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)     8731 2023-07-14 21:02:58.000000 seismic-rna-0.4.1/src/seismicrna/graph/base.py
--rw-r--r--   0 mfa        (503) staff       (20)     3539 2023-07-15 02:04:52.000000 seismic-rna-0.4.1/src/seismicrna/graph/color.py
--rw-r--r--   0 mfa        (503) staff       (20)     2701 2023-07-12 18:10:50.000000 seismic-rna-0.4.1/src/seismicrna/graph/default.py
--rw-r--r--   0 mfa        (503) staff       (20)     7493 2023-07-16 00:28:27.000000 seismic-rna-0.4.1/src/seismicrna/graph/hist.py
--rw-r--r--   0 mfa        (503) staff       (20)      337 2023-06-29 02:17:49.000000 seismic-rna-0.4.1/src/seismicrna/graph/main.py
--rw-r--r--   0 mfa        (503) staff       (20)    13371 2023-07-16 00:27:55.000000 seismic-rna-0.4.1/src/seismicrna/graph/seq.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-21 02:50:00.027781 seismic-rna-0.4.1/src/seismicrna/image/
--rw-r--r--   0 mfa        (503) staff       (20)        0 2023-07-09 20:01:37.000000 seismic-rna-0.4.1/src/seismicrna/image/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)     3492 2023-07-12 02:42:12.000000 seismic-rna-0.4.1/src/seismicrna/image/logo.py
--rw-r--r--   0 mfa        (503) staff       (20)     9616 2023-07-16 01:27:58.000000 seismic-rna-0.4.1/src/seismicrna/main.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-21 02:50:00.035121 seismic-rna-0.4.1/src/seismicrna/mask/
--rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.4.1/src/seismicrna/mask/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)     4074 2023-07-08 00:07:16.000000 seismic-rna-0.4.1/src/seismicrna/mask/load.py
--rw-r--r--   0 mfa        (503) staff       (20)     4447 2023-07-16 00:26:07.000000 seismic-rna-0.4.1/src/seismicrna/mask/main.py
--rw-r--r--   0 mfa        (503) staff       (20)     1315 2023-06-29 02:17:49.000000 seismic-rna-0.4.1/src/seismicrna/mask/report.py
--rw-r--r--   0 mfa        (503) staff       (20)    14222 2023-07-15 22:36:16.000000 seismic-rna-0.4.1/src/seismicrna/mask/write.py
--rw-r--r--   0 mfa        (503) staff       (20)      164 2023-07-16 01:29:14.000000 seismic-rna-0.4.1/src/seismicrna/meta.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-21 02:50:00.048107 seismic-rna-0.4.1/src/seismicrna/relate/
--rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.4.1/src/seismicrna/relate/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)     1413 2023-06-29 02:17:49.000000 seismic-rna-0.4.1/src/seismicrna/relate/export.py
--rw-r--r--   0 mfa        (503) staff       (20)     3241 2023-06-29 02:17:49.000000 seismic-rna-0.4.1/src/seismicrna/relate/load.py
--rw-r--r--   0 mfa        (503) staff       (20)     3096 2023-07-20 02:49:54.000000 seismic-rna-0.4.1/src/seismicrna/relate/main.py
--rw-r--r--   0 mfa        (503) staff       (20)    28055 2023-06-29 02:17:49.000000 seismic-rna-0.4.1/src/seismicrna/relate/relate.py
--rw-r--r--   0 mfa        (503) staff       (20)     1509 2023-06-29 02:17:49.000000 seismic-rna-0.4.1/src/seismicrna/relate/report.py
--rw-r--r--   0 mfa        (503) staff       (20)    10170 2023-06-30 02:27:38.000000 seismic-rna-0.4.1/src/seismicrna/relate/sam.py
--rw-r--r--   0 mfa        (503) staff       (20)     2984 2023-06-29 02:17:49.000000 seismic-rna-0.4.1/src/seismicrna/relate/seqpos.py
--rw-r--r--   0 mfa        (503) staff       (20)     3066 2023-06-29 02:17:49.000000 seismic-rna-0.4.1/src/seismicrna/relate/test.py
--rw-r--r--   0 mfa        (503) staff       (20)    15085 2023-07-10 03:02:51.000000 seismic-rna-0.4.1/src/seismicrna/relate/write.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-21 02:50:00.051917 seismic-rna-0.4.1/src/seismicrna/struct/
--rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.4.1/src/seismicrna/struct/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)     3827 2023-07-19 23:10:12.000000 seismic-rna-0.4.1/src/seismicrna/struct/main.py
--rw-r--r--   0 mfa        (503) staff       (20)     1850 2023-07-09 19:43:33.000000 seismic-rna-0.4.1/src/seismicrna/struct/rnastructure.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-21 02:50:00.058045 seismic-rna-0.4.1/src/seismicrna/table/
--rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.4.1/src/seismicrna/table/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)     9380 2023-07-20 23:21:09.000000 seismic-rna-0.4.1/src/seismicrna/table/base.py
--rw-r--r--   0 mfa        (503) staff       (20)     7236 2023-07-15 00:22:19.000000 seismic-rna-0.4.1/src/seismicrna/table/load.py
--rw-r--r--   0 mfa        (503) staff       (20)     1724 2023-07-16 00:27:03.000000 seismic-rna-0.4.1/src/seismicrna/table/main.py
--rw-r--r--   0 mfa        (503) staff       (20)    15792 2023-07-21 02:45:00.000000 seismic-rna-0.4.1/src/seismicrna/table/tabulate.py
--rw-r--r--   0 mfa        (503) staff       (20)     4684 2023-07-15 00:02:34.000000 seismic-rna-0.4.1/src/seismicrna/table/write.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-21 02:50:00.060093 seismic-rna-0.4.1/src/seismicrna/test/
--rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.4.1/src/seismicrna/test/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)      971 2023-07-06 00:56:02.000000 seismic-rna-0.4.1/src/seismicrna/test/main.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-25 02:02:28.312890 seismic-rna-0.5.0/
+-rw-r--r--   0 mfa        (503) staff       (20)    35150 2023-06-29 02:33:57.000000 seismic-rna-0.5.0/LICENSE
+-rw-r--r--   0 mfa        (503) staff       (20)     1910 2023-07-25 02:02:28.312286 seismic-rna-0.5.0/PKG-INFO
+-rw-r--r--   0 mfa        (503) staff       (20)     1347 2023-07-19 21:38:18.000000 seismic-rna-0.5.0/README.md
+-rw-r--r--   0 mfa        (503) staff       (20)     1037 2023-07-24 19:17:05.000000 seismic-rna-0.5.0/pyproject.toml
+-rw-r--r--   0 mfa        (503) staff       (20)       38 2023-07-25 02:02:28.313073 seismic-rna-0.5.0/setup.cfg
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-25 02:02:28.087771 seismic-rna-0.5.0/src/
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-25 02:02:28.099147 seismic-rna-0.5.0/src/seismic_rna.egg-info/
+-rw-r--r--   0 mfa        (503) staff       (20)     1910 2023-07-25 02:02:28.000000 seismic-rna-0.5.0/src/seismic_rna.egg-info/PKG-INFO
+-rw-r--r--   0 mfa        (503) staff       (20)     3226 2023-07-25 02:02:28.000000 seismic-rna-0.5.0/src/seismic_rna.egg-info/SOURCES.txt
+-rw-r--r--   0 mfa        (503) staff       (20)        1 2023-07-25 02:02:28.000000 seismic-rna-0.5.0/src/seismic_rna.egg-info/dependency_links.txt
+-rw-r--r--   0 mfa        (503) staff       (20)       53 2023-07-25 02:02:28.000000 seismic-rna-0.5.0/src/seismic_rna.egg-info/entry_points.txt
+-rw-r--r--   0 mfa        (503) staff       (20)      176 2023-07-25 02:02:28.000000 seismic-rna-0.5.0/src/seismic_rna.egg-info/requires.txt
+-rw-r--r--   0 mfa        (503) staff       (20)       11 2023-07-25 02:02:28.000000 seismic-rna-0.5.0/src/seismic_rna.egg-info/top_level.txt
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-25 02:02:28.101507 seismic-rna-0.5.0/src/seismicrna/
+-rw-r--r--   0 mfa        (503) staff       (20)      201 2023-07-16 01:27:23.000000 seismic-rna-0.5.0/src/seismicrna/__init__.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-25 02:02:28.109597 seismic-rna-0.5.0/src/seismicrna/align/
+-rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.5.0/src/seismicrna/align/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)    22758 2023-07-05 00:01:54.000000 seismic-rna-0.5.0/src/seismicrna/align/fq2bam.py
+-rwxr-xr-x   0 mfa        (503) staff       (20)    20020 2023-07-09 17:46:17.000000 seismic-rna-0.5.0/src/seismicrna/align/fqutil.py
+-rw-r--r--   0 mfa        (503) staff       (20)     7600 2023-07-20 02:53:44.000000 seismic-rna-0.5.0/src/seismicrna/align/main.py
+-rwxr-xr-x   0 mfa        (503) staff       (20)     9115 2023-06-29 02:17:49.000000 seismic-rna-0.5.0/src/seismicrna/align/strandedness.py
+-rw-r--r--   0 mfa        (503) staff       (20)        0 2023-06-29 02:17:49.000000 seismic-rna-0.5.0/src/seismicrna/align/test.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-25 02:02:28.134606 seismic-rna-0.5.0/src/seismicrna/cluster/
+-rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.5.0/src/seismicrna/cluster/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)    13197 2023-07-15 21:12:26.000000 seismic-rna-0.5.0/src/seismicrna/cluster/compare.py
+-rw-r--r--   0 mfa        (503) staff       (20)    18681 2023-06-29 02:17:49.000000 seismic-rna-0.5.0/src/seismicrna/cluster/em.py
+-rw-r--r--   0 mfa        (503) staff       (20)     6262 2023-06-29 02:17:49.000000 seismic-rna-0.5.0/src/seismicrna/cluster/krun.py
+-rw-r--r--   0 mfa        (503) staff       (20)     4209 2023-06-29 02:17:49.000000 seismic-rna-0.5.0/src/seismicrna/cluster/load.py
+-rw-r--r--   0 mfa        (503) staff       (20)     2464 2023-07-16 00:26:28.000000 seismic-rna-0.5.0/src/seismicrna/cluster/main.py
+-rw-r--r--   0 mfa        (503) staff       (20)     1334 2023-07-24 16:13:21.000000 seismic-rna-0.5.0/src/seismicrna/cluster/names.py
+-rw-r--r--   0 mfa        (503) staff       (20)     2862 2023-06-29 02:17:49.000000 seismic-rna-0.5.0/src/seismicrna/cluster/report.py
+-rw-r--r--   0 mfa        (503) staff       (20)     4981 2023-06-29 02:17:49.000000 seismic-rna-0.5.0/src/seismicrna/cluster/write.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-25 02:02:28.205889 seismic-rna-0.5.0/src/seismicrna/core/
+-rw-r--r--   0 mfa        (503) staff       (20)        0 2023-06-29 02:17:49.000000 seismic-rna-0.5.0/src/seismicrna/core/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)    15704 2023-06-29 18:01:10.000000 seismic-rna-0.5.0/src/seismicrna/core/bitcall.py
+-rw-r--r--   0 mfa        (503) staff       (20)    19264 2023-07-07 22:07:51.000000 seismic-rna-0.5.0/src/seismicrna/core/bitvect.py
+-rw-r--r--   0 mfa        (503) staff       (20)    18140 2023-07-24 20:58:36.000000 seismic-rna-0.5.0/src/seismicrna/core/cli.py
+-rw-r--r--   0 mfa        (503) staff       (20)     1120 2023-06-29 21:48:51.000000 seismic-rna-0.5.0/src/seismicrna/core/depend.py
+-rw-r--r--   0 mfa        (503) staff       (20)     6847 2023-07-23 22:22:45.000000 seismic-rna-0.5.0/src/seismicrna/core/docdef.py
+-rw-r--r--   0 mfa        (503) staff       (20)     2201 2023-06-29 02:17:49.000000 seismic-rna-0.5.0/src/seismicrna/core/docstring.py
+-rw-r--r--   0 mfa        (503) staff       (20)     1972 2023-06-29 02:17:49.000000 seismic-rna-0.5.0/src/seismicrna/core/dump.py
+-rw-r--r--   0 mfa        (503) staff       (20)      628 2023-06-29 02:17:49.000000 seismic-rna-0.5.0/src/seismicrna/core/files.py
+-rw-r--r--   0 mfa        (503) staff       (20)     7933 2023-07-07 22:47:51.000000 seismic-rna-0.5.0/src/seismicrna/core/load.py
+-rw-r--r--   0 mfa        (503) staff       (20)     2837 2023-07-07 02:37:13.000000 seismic-rna-0.5.0/src/seismicrna/core/logs.py
+-rw-r--r--   0 mfa        (503) staff       (20)    14781 2023-07-24 20:58:00.000000 seismic-rna-0.5.0/src/seismicrna/core/mu.py
+-rw-r--r--   0 mfa        (503) staff       (20)    10537 2023-06-30 18:53:43.000000 seismic-rna-0.5.0/src/seismicrna/core/mu_test.py
+-rw-r--r--   0 mfa        (503) staff       (20)    14509 2023-07-12 20:28:15.000000 seismic-rna-0.5.0/src/seismicrna/core/parallel.py
+-rw-r--r--   0 mfa        (503) staff       (20)    23511 2023-07-07 00:11:58.000000 seismic-rna-0.5.0/src/seismicrna/core/path.py
+-rw-r--r--   0 mfa        (503) staff       (20)    29387 2023-07-14 20:09:45.000000 seismic-rna-0.5.0/src/seismicrna/core/rel.py
+-rw-r--r--   0 mfa        (503) staff       (20)    45953 2023-06-30 18:58:01.000000 seismic-rna-0.5.0/src/seismicrna/core/rel_test.py
+-rw-r--r--   0 mfa        (503) staff       (20)    29740 2023-07-12 04:26:52.000000 seismic-rna-0.5.0/src/seismicrna/core/report.py
+-rw-r--r--   0 mfa        (503) staff       (20)     8525 2023-07-24 21:00:21.000000 seismic-rna-0.5.0/src/seismicrna/core/rna.py
+-rw-r--r--   0 mfa        (503) staff       (20)    27329 2023-07-09 16:52:06.000000 seismic-rna-0.5.0/src/seismicrna/core/sect.py
+-rw-r--r--   0 mfa        (503) staff       (20)     7101 2023-07-06 00:49:26.000000 seismic-rna-0.5.0/src/seismicrna/core/sect_test.py
+-rw-r--r--   0 mfa        (503) staff       (20)     9798 2023-06-30 03:50:29.000000 seismic-rna-0.5.0/src/seismicrna/core/seq.py
+-rw-r--r--   0 mfa        (503) staff       (20)     6634 2023-06-30 14:56:23.000000 seismic-rna-0.5.0/src/seismicrna/core/seq_test.py
+-rw-r--r--   0 mfa        (503) staff       (20)     2799 2023-06-29 21:49:14.000000 seismic-rna-0.5.0/src/seismicrna/core/shell.py
+-rw-r--r--   0 mfa        (503) staff       (20)     1054 2023-06-29 19:54:35.000000 seismic-rna-0.5.0/src/seismicrna/core/sim.py
+-rw-r--r--   0 mfa        (503) staff       (20)      769 2023-07-06 00:49:45.000000 seismic-rna-0.5.0/src/seismicrna/core/sim_test.py
+-rw-r--r--   0 mfa        (503) staff       (20)      758 2023-06-29 02:17:49.000000 seismic-rna-0.5.0/src/seismicrna/core/types.py
+-rwxr-xr-x   0 mfa        (503) staff       (20)    14291 2023-06-30 03:36:23.000000 seismic-rna-0.5.0/src/seismicrna/core/xam.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-25 02:02:28.210162 seismic-rna-0.5.0/src/seismicrna/demult/
+-rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.5.0/src/seismicrna/demult/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)    42624 2023-07-19 22:35:50.000000 seismic-rna-0.5.0/src/seismicrna/demult/demultiplex.py
+-rw-r--r--   0 mfa        (503) staff       (20)     2103 2023-07-19 22:35:50.000000 seismic-rna-0.5.0/src/seismicrna/demult/main.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-25 02:02:28.240786 seismic-rna-0.5.0/src/seismicrna/draw/
+-rw-r--r--   0 mfa        (503) staff       (20)      256 2023-06-29 19:38:33.000000 seismic-rna-0.5.0/src/seismicrna/draw/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)      225 2023-06-29 02:17:49.000000 seismic-rna-0.5.0/src/seismicrna/draw/load_dataset.py
+-rw-r--r--   0 mfa        (503) staff       (20)     6013 2023-06-29 02:17:49.000000 seismic-rna-0.5.0/src/seismicrna/draw/main.py
+-rw-r--r--   0 mfa        (503) staff       (20)     6656 2023-06-29 02:17:49.000000 seismic-rna-0.5.0/src/seismicrna/draw/manipulator.py
+-rw-r--r--   0 mfa        (503) staff       (20)    17447 2023-06-29 19:43:29.000000 seismic-rna-0.5.0/src/seismicrna/draw/plotter.py
+-rw-r--r--   0 mfa        (503) staff       (20)    15931 2023-06-29 02:17:49.000000 seismic-rna-0.5.0/src/seismicrna/draw/study.py
+-rw-r--r--   0 mfa        (503) staff       (20)    11285 2023-06-29 02:17:49.000000 seismic-rna-0.5.0/src/seismicrna/draw/util.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-25 02:02:28.254752 seismic-rna-0.5.0/src/seismicrna/graph/
+-rw-r--r--   0 mfa        (503) staff       (20)       22 2023-06-29 02:17:49.000000 seismic-rna-0.5.0/src/seismicrna/graph/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)    11178 2023-07-25 01:42:36.000000 seismic-rna-0.5.0/src/seismicrna/graph/base.py
+-rw-r--r--   0 mfa        (503) staff       (20)     3539 2023-07-15 02:04:52.000000 seismic-rna-0.5.0/src/seismicrna/graph/color.py
+-rw-r--r--   0 mfa        (503) staff       (20)     2720 2023-07-24 17:02:36.000000 seismic-rna-0.5.0/src/seismicrna/graph/default.py
+-rw-r--r--   0 mfa        (503) staff       (20)     3310 2023-07-25 01:26:46.000000 seismic-rna-0.5.0/src/seismicrna/graph/delbar.py
+-rw-r--r--   0 mfa        (503) staff       (20)     7513 2023-07-24 17:02:36.000000 seismic-rna-0.5.0/src/seismicrna/graph/hist.py
+-rw-r--r--   0 mfa        (503) staff       (20)      399 2023-07-24 23:03:17.000000 seismic-rna-0.5.0/src/seismicrna/graph/main.py
+-rw-r--r--   0 mfa        (503) staff       (20)     3203 2023-07-25 01:25:16.000000 seismic-rna-0.5.0/src/seismicrna/graph/scatter.py
+-rw-r--r--   0 mfa        (503) staff       (20)     1572 2023-07-24 21:45:48.000000 seismic-rna-0.5.0/src/seismicrna/graph/seq.py
+-rw-r--r--   0 mfa        (503) staff       (20)     9998 2023-07-25 01:32:37.000000 seismic-rna-0.5.0/src/seismicrna/graph/seqbar.py
+-rw-r--r--   0 mfa        (503) staff       (20)     9126 2023-07-25 01:43:16.000000 seismic-rna-0.5.0/src/seismicrna/graph/seqpair.py
+-rw-r--r--   0 mfa        (503) staff       (20)     3821 2023-07-24 23:10:58.000000 seismic-rna-0.5.0/src/seismicrna/graph/traces.py
+-rw-r--r--   0 mfa        (503) staff       (20)     2697 2023-07-24 17:02:36.000000 seismic-rna-0.5.0/src/seismicrna/graph/write.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-25 02:02:28.257260 seismic-rna-0.5.0/src/seismicrna/image/
+-rw-r--r--   0 mfa        (503) staff       (20)        0 2023-07-09 20:01:37.000000 seismic-rna-0.5.0/src/seismicrna/image/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)     3492 2023-07-12 02:42:12.000000 seismic-rna-0.5.0/src/seismicrna/image/logo.py
+-rw-r--r--   0 mfa        (503) staff       (20)     9628 2023-07-24 01:05:01.000000 seismic-rna-0.5.0/src/seismicrna/main.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-25 02:02:28.266434 seismic-rna-0.5.0/src/seismicrna/mask/
+-rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.5.0/src/seismicrna/mask/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)     4074 2023-07-08 00:07:16.000000 seismic-rna-0.5.0/src/seismicrna/mask/load.py
+-rw-r--r--   0 mfa        (503) staff       (20)     4447 2023-07-16 00:26:07.000000 seismic-rna-0.5.0/src/seismicrna/mask/main.py
+-rw-r--r--   0 mfa        (503) staff       (20)     1315 2023-06-29 02:17:49.000000 seismic-rna-0.5.0/src/seismicrna/mask/report.py
+-rw-r--r--   0 mfa        (503) staff       (20)    14222 2023-07-15 22:36:16.000000 seismic-rna-0.5.0/src/seismicrna/mask/write.py
+-rw-r--r--   0 mfa        (503) staff       (20)      164 2023-07-16 01:29:14.000000 seismic-rna-0.5.0/src/seismicrna/meta.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-25 02:02:28.297763 seismic-rna-0.5.0/src/seismicrna/relate/
+-rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.5.0/src/seismicrna/relate/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)     1413 2023-06-29 02:17:49.000000 seismic-rna-0.5.0/src/seismicrna/relate/export.py
+-rw-r--r--   0 mfa        (503) staff       (20)     3241 2023-06-29 02:17:49.000000 seismic-rna-0.5.0/src/seismicrna/relate/load.py
+-rw-r--r--   0 mfa        (503) staff       (20)     3096 2023-07-20 02:49:54.000000 seismic-rna-0.5.0/src/seismicrna/relate/main.py
+-rw-r--r--   0 mfa        (503) staff       (20)    28055 2023-06-29 02:17:49.000000 seismic-rna-0.5.0/src/seismicrna/relate/relate.py
+-rw-r--r--   0 mfa        (503) staff       (20)     1509 2023-06-29 02:17:49.000000 seismic-rna-0.5.0/src/seismicrna/relate/report.py
+-rw-r--r--   0 mfa        (503) staff       (20)    10170 2023-06-30 02:27:38.000000 seismic-rna-0.5.0/src/seismicrna/relate/sam.py
+-rw-r--r--   0 mfa        (503) staff       (20)     2984 2023-06-29 02:17:49.000000 seismic-rna-0.5.0/src/seismicrna/relate/seqpos.py
+-rw-r--r--   0 mfa        (503) staff       (20)     3066 2023-06-29 02:17:49.000000 seismic-rna-0.5.0/src/seismicrna/relate/test.py
+-rw-r--r--   0 mfa        (503) staff       (20)    15085 2023-07-10 03:02:51.000000 seismic-rna-0.5.0/src/seismicrna/relate/write.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-25 02:02:28.300561 seismic-rna-0.5.0/src/seismicrna/struct/
+-rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.5.0/src/seismicrna/struct/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)     3847 2023-07-24 20:59:53.000000 seismic-rna-0.5.0/src/seismicrna/struct/main.py
+-rw-r--r--   0 mfa        (503) staff       (20)     1807 2023-07-24 21:02:55.000000 seismic-rna-0.5.0/src/seismicrna/struct/rnastructure.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-25 02:02:28.307288 seismic-rna-0.5.0/src/seismicrna/table/
+-rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.5.0/src/seismicrna/table/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)     8983 2023-07-24 21:08:00.000000 seismic-rna-0.5.0/src/seismicrna/table/base.py
+-rw-r--r--   0 mfa        (503) staff       (20)     8287 2023-07-24 22:13:11.000000 seismic-rna-0.5.0/src/seismicrna/table/load.py
+-rw-r--r--   0 mfa        (503) staff       (20)     2138 2023-07-24 01:11:31.000000 seismic-rna-0.5.0/src/seismicrna/table/main.py
+-rw-r--r--   0 mfa        (503) staff       (20)    15792 2023-07-21 02:45:00.000000 seismic-rna-0.5.0/src/seismicrna/table/tabulate.py
+-rw-r--r--   0 mfa        (503) staff       (20)     4684 2023-07-15 00:02:34.000000 seismic-rna-0.5.0/src/seismicrna/table/write.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-25 02:02:28.311179 seismic-rna-0.5.0/src/seismicrna/test/
+-rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.5.0/src/seismicrna/test/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)      971 2023-07-06 00:56:02.000000 seismic-rna-0.5.0/src/seismicrna/test/main.py
```

### Comparing `seismic-rna-0.4.1/LICENSE` & `seismic-rna-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.1/PKG-INFO` & `seismic-rna-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seismic-rna
-Version: 0.4.1
+Version: 0.5.0
 Summary: RNA Structure Ensemble Inference via Sequencing, Mutation Identification, and Clustering
 Author: Matty Allan, Yves Martin, Scott Grote, Alberic de Lajarte
 License: GPL-3.0-only
 Project-URL: Homepage, https://github.com/rouskinlab/seismic-rna
 Project-URL: Bug Tracker, https://github.com/rouskinlab/seismic-rna/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `seismic-rna-0.4.1/README.md` & `seismic-rna-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.1/pyproject.toml` & `seismic-rna-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "seismic-rna"
-version = "0.4.1"
+version = "0.5.0"
 authors = [
     {name="Matty Allan"},
     {name="Yves Martin"},
     {name="Scott Grote"},
     {name="Alberic de Lajarte"},
 ]
 description = "RNA Structure Ensemble Inference via Sequencing, Mutation Identification, and Clustering"
```

### Comparing `seismic-rna-0.4.1/src/seismic_rna.egg-info/PKG-INFO` & `seismic-rna-0.5.0/src/seismic_rna.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seismic-rna
-Version: 0.4.1
+Version: 0.5.0
 Summary: RNA Structure Ensemble Inference via Sequencing, Mutation Identification, and Clustering
 Author: Matty Allan, Yves Martin, Scott Grote, Alberic de Lajarte
 License: GPL-3.0-only
 Project-URL: Homepage, https://github.com/rouskinlab/seismic-rna
 Project-URL: Bug Tracker, https://github.com/rouskinlab/seismic-rna/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `seismic-rna-0.4.1/src/seismic_rna.egg-info/SOURCES.txt` & `seismic-rna-0.5.0/src/seismic_rna.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -63,17 +63,23 @@
 src/seismicrna/draw/plotter.py
 src/seismicrna/draw/study.py
 src/seismicrna/draw/util.py
 src/seismicrna/graph/__init__.py
 src/seismicrna/graph/base.py
 src/seismicrna/graph/color.py
 src/seismicrna/graph/default.py
+src/seismicrna/graph/delbar.py
 src/seismicrna/graph/hist.py
 src/seismicrna/graph/main.py
+src/seismicrna/graph/scatter.py
 src/seismicrna/graph/seq.py
+src/seismicrna/graph/seqbar.py
+src/seismicrna/graph/seqpair.py
+src/seismicrna/graph/traces.py
+src/seismicrna/graph/write.py
 src/seismicrna/image/__init__.py
 src/seismicrna/image/logo.py
 src/seismicrna/mask/__init__.py
 src/seismicrna/mask/load.py
 src/seismicrna/mask/main.py
 src/seismicrna/mask/report.py
 src/seismicrna/mask/write.py
```

### Comparing `seismic-rna-0.4.1/src/seismicrna/align/fq2bam.py` & `seismic-rna-0.5.0/src/seismicrna/align/fq2bam.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.1/src/seismicrna/align/fqutil.py` & `seismic-rna-0.5.0/src/seismicrna/align/fqutil.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.1/src/seismicrna/align/main.py` & `seismic-rna-0.5.0/src/seismicrna/align/main.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.1/src/seismicrna/align/strandedness.py` & `seismic-rna-0.5.0/src/seismicrna/align/strandedness.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.1/src/seismicrna/cluster/compare.py` & `seismic-rna-0.5.0/src/seismicrna/cluster/compare.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.1/src/seismicrna/cluster/em.py` & `seismic-rna-0.5.0/src/seismicrna/cluster/em.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.1/src/seismicrna/cluster/krun.py` & `seismic-rna-0.5.0/src/seismicrna/cluster/krun.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.1/src/seismicrna/cluster/load.py` & `seismic-rna-0.5.0/src/seismicrna/cluster/load.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.1/src/seismicrna/cluster/main.py` & `seismic-rna-0.5.0/src/seismicrna/cluster/main.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.1/src/seismicrna/cluster/names.py` & `seismic-rna-0.5.0/src/seismicrna/cluster/names.py`

 * *Files 9% similar despite different names*

```diff
@@ -33,10 +33,10 @@
         raise ValueError(f"order must be {ineq} 0, but got {order}")
     if cluster < 0 or (cluster == 0 and not allow_zero):
         raise ValueError(f"cluster must be {ineq} 0, but got {cluster}")
     if cluster > order:
         raise ValueError(f"cluster ({cluster}) must be ≤ order ({order})")
 
 
-def fmt_clust_name(order: int, cluster: int):
-    validate_order_cluster(order, cluster)
-    return f"Cluster {order}-{cluster}"
+def fmt_clust_name(order: int, cluster: int, allow_zero: bool = False):
+    validate_order_cluster(order, cluster, allow_zero)
+    return f"Cluster {order}-{cluster}" if order > 0 else ENSEMBLE_NAME
```

### Comparing `seismic-rna-0.4.1/src/seismicrna/cluster/report.py` & `seismic-rna-0.5.0/src/seismicrna/cluster/report.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.1/src/seismicrna/cluster/write.py` & `seismic-rna-0.5.0/src/seismicrna/cluster/write.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.1/src/seismicrna/core/bitcall.py` & `seismic-rna-0.5.0/src/seismicrna/core/bitcall.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.1/src/seismicrna/core/bitvect.py` & `seismic-rna-0.5.0/src/seismicrna/core/bitvect.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.1/src/seismicrna/core/cli.py` & `seismic-rna-0.5.0/src/seismicrna/core/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -590,40 +590,36 @@
          "likelihood value has increased by less than this "
          "threshold between two consecutive iterations.")
 
 # Tables
 
 opt_rels = Option(
     ("--rels", "-r"),
-    default="",
     type=str,
+    multiple=True,
+    default=("m",),
     help="Output these relationships between the read and the reference")
 
 # RNA structure prediction
 
 opt_fold = Option(
     ("--fold/--no-fold",),
     type=bool,
     default=False,
     help="Whether to predict the RNA structure using Fold")
 
 opt_quantile = Option(
     ("--quantile", "-q"),
     type=float,
-    default=0.9,
-    help="Quantile of reactivities for normalization")
+    default=-1.,
+    help="Quantile of mutation rates for normalization and winsorization "
+         "(-1 to disable both). Must be -1 or in [0, 1].")
 
 # Graphing
 
-opt_stack = Option(
-    ("--stack/--no-stack",),
-    type=bool,
-    default=False,
-    help="Whether to stack relationships")
-
 opt_arrange = Option(
     ("--arrange",),
     type=Choice(CLUST_ARRANGE_OPTIONS),
     default=CLUST_ORDER,
     help="Whether to graph each INDIVidual cluster in its own file, "
          "graph each ORDER of clusters in its own file, "
          "or UNITE all clusters in one file containing all orders.")
```

### Comparing `seismic-rna-0.4.1/src/seismicrna/core/depend.py` & `seismic-rna-0.5.0/src/seismicrna/core/depend.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.1/src/seismicrna/core/docdef.py` & `seismic-rna-0.5.0/src/seismicrna/core/docdef.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,16 +166,16 @@
     return decorator
 
 
 def autodoc(extra_docs: dict[str, str] | None = None, return_doc: str = ""):
     """ Call `paramdoc` and automatically infer descriptions and
     type annotations about all parameters from the CLI and API.
     Documentation of any extra parameters may also be given. """
-    return paramdoc(cli_docs if extra_docs is None
-                    else {**cli_docs, **extra_docs},
+    return paramdoc((cli_docs if extra_docs is None
+                     else {**cli_docs, **extra_docs}),
                     return_doc)
 
 
 def auto(*,
          extra_defs: dict[str, Any] | None = None,
          exclude_defs: tuple[str, ...] = (),
          extra_docs: dict[str, str] | None = None,
```

### Comparing `seismic-rna-0.4.1/src/seismicrna/core/docstring.py` & `seismic-rna-0.5.0/src/seismicrna/core/docstring.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.1/src/seismicrna/core/dump.py` & `seismic-rna-0.5.0/src/seismicrna/core/dump.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.1/src/seismicrna/core/files.py` & `seismic-rna-0.5.0/src/seismicrna/core/files.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.1/src/seismicrna/core/load.py` & `seismic-rna-0.5.0/src/seismicrna/core/load.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.1/src/seismicrna/core/logs.py` & `seismic-rna-0.5.0/src/seismicrna/core/logs.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.1/src/seismicrna/core/mu.py` & `seismic-rna-0.5.0/src/seismicrna/core/mu.py`

 * *Files 6% similar despite different names*

```diff
@@ -305,7 +305,26 @@
         Must be ≥ 0.
     """
     return pd.DataFrame(calc_mu_adj(mu_obs.reindex(index=section.range,
                                                    fill_value=0.).values,
                                     min_gap),
                         index=section.range,
                         columns=mu_obs.columns).loc[mu_obs.index]
+
+
+def get_mu_quantile(mus: pd.Series, quantile: float) -> float:
+    """ Compute the mutation rate at a quantile. """
+    return np.nanquantile(mus.values, quantile)
+
+
+def normalize(mus: pd.Series, quantile: float):
+    """ Normalize the mutation rates to a quantile. """
+    if quantile == -1.:
+        # Do not normalize the mutation rates if quantile == -1.
+        return mus.copy()
+    return mus / get_mu_quantile(mus, quantile)
+
+
+def winsorize(mus: pd.Series, quantile: float):
+    """ Normalize and winsorize the mutation rates to a quantile. """
+    return pd.Series(np.clip(normalize(mus, quantile), 0., 1.),
+                     index=mus.index)
```

### Comparing `seismic-rna-0.4.1/src/seismicrna/core/mu_test.py` & `seismic-rna-0.5.0/src/seismicrna/core/mu_test.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.1/src/seismicrna/core/parallel.py` & `seismic-rna-0.5.0/src/seismicrna/core/parallel.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.1/src/seismicrna/core/path.py` & `seismic-rna-0.5.0/src/seismicrna/core/path.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.1/src/seismicrna/core/rel.py` & `seismic-rna-0.5.0/src/seismicrna/core/rel.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.1/src/seismicrna/core/rel_test.py` & `seismic-rna-0.5.0/src/seismicrna/core/rel_test.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.1/src/seismicrna/core/report.py` & `seismic-rna-0.5.0/src/seismicrna/core/report.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.1/src/seismicrna/core/rna.py` & `seismic-rna-0.5.0/src/seismicrna/core/rna.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from pathlib import Path
 from typing import Iterable
 
 import numpy as np
 import pandas as pd
 
 from . import path
+from .mu import winsorize
 from .sect import Section
 from .seq import write_fasta
 
 logger = getLogger(__name__)
 
 
 class RnaSection(object):
@@ -26,15 +27,15 @@
 
     @property
     def sect(self):
         return self.section.name
 
     @cached_property
     def seq(self):
-        """ Sequence in RNA format. """
+        """ Sequence as RNA. """
         return self.section.seq.tr()
 
     @property
     def seq_record(self):
         return self.section.ref_sect, self.seq
 
 
@@ -46,30 +47,14 @@
         super().__init__(title, section)
         self.sample = sample
         self.dms_sect = data_sect
         if np.any(reacts < 0.) or np.any(reacts > 1.):
             raise ValueError(f"Got reactivities outside [0, 1]: {reacts}")
         self.reacts = reacts.reindex(self.section.range)
 
-    def get_ceiling(self, quantile: float) -> float:
-        """ Compute the maximum reactivity given a quantile. """
-        if not 0. < quantile <= 1.:
-            raise ValueError("Quantile for reactivity ceiling must be in "
-                             f"(0, 1], but got {quantile}")
-        return np.nanquantile(self.reacts.values, quantile)
-
-    def normalize(self, quantile: float):
-        """ Normalize the reactivities to a given quantile. """
-        return self.reacts / self.get_ceiling(quantile)
-
-    def winsorize(self, quantile: float):
-        """ Normalize and winsorize the reactivities. """
-        return pd.Series(np.clip(self.normalize(quantile), 0., 1.),
-                         index=self.reacts.index)
-
     @cache
     def get_dir(self, out_dir: Path):
         """ Get the directory in which this RNA's files will go. """
         return path.builddir(path.ModSeg, path.SampSeg, path.RefSeg,
                              path.SectSeg, path.FoldSectSeg,
                              top=out_dir, module=path.MOD_STRUCT,
                              sample=self.sample, ref=self.ref,
@@ -96,15 +81,15 @@
                              struct=self.title, ext=path.DOT_EXTS[0])
 
     def dms_file(self, out_dir: Path):
         """ Get the path to the DMS data file of the RNA. """
         return self.get_file(out_dir, path.DmsReactsSeg,
                              reacts=self.title, ext=path.DMS_EXT)
 
-    def varnac_file(self, out_dir: Path):
+    def varna_color_file(self, out_dir: Path):
         """ Get the path to the VARNA color file of the RNA. """
         return self.get_file(out_dir, path.VarnaColorSeg,
                              reacts=self.title, ext=path.TXT_EXT)
 
     def to_fasta(self, out_dir: Path):
         """ Write the RNA sequence to a FASTA file. """
         fasta = self.get_fasta(out_dir)
@@ -112,42 +97,42 @@
         return fasta
 
     def to_dms(self, out_dir: Path, quantile: float):
         """ Write the DMS reactivities to a DMS file. """
         # The DMS reactivities must be numbered starting from 1 at the
         # beginning of the section, even if the section does not start
         # at 1. Renumber the section from 1.
-        dms = pd.Series(self.winsorize(quantile).values,
+        dms = pd.Series(winsorize(self.reacts, quantile).values,
                         index=self.section.range_int_one)
         # Drop bases with missing data to make RNAstructure ignore them.
         dms.dropna(inplace=True)
         # Write the DMS reactivities to the DMS file.
         dms_file = self.dms_file(out_dir)
         dms.to_csv(dms_file, sep="\t", header=False)
         return dms_file
 
-    def to_varnac(self, out_dir: Path, quantile: float):
+    def to_varna_color_file(self, out_dir: Path, quantile: float):
         """ Write the VARNA colors to a file. """
         # Normalize and winsorize the DMS reactivities.
-        varnac = self.winsorize(quantile)
+        varna_color = winsorize(self.reacts, quantile)
         # Fill missing values with -1, to signify no data.
-        varnac.fillna(-1., inplace=True)
+        varna_color.fillna(-1., inplace=True)
         # Write the values to the VARNA color file.
-        varnac_file = self.varnac_file(out_dir)
-        varnac.to_csv(varnac_file, header=False, index=False)
-        return varnac_file
+        varna_color_file = self.varna_color_file(out_dir)
+        varna_color.to_csv(varna_color_file, header=False, index=False)
+        return varna_color_file
 
 
 class Rna2dStructure(RnaSection):
     """ RNA secondary structure. """
 
-    IDX_FIELD = "n"
+    IDX_FIELD = "Index"
     BASE_FIELD = "Base"
-    PRIOR_FIELD = "n-1"
-    NEXT_FIELD = "n+1"
+    PREV_FIELD = "Prev"
+    NEXT_FIELD = "Next"
     PAIR_FIELD = "Pair"
     POS_FIELD = "Position"
 
     def __init__(self,
                  title: str,
                  section: Section,
                  pairs: Iterable[tuple[int, int]]):
@@ -192,26 +177,26 @@
         return partners
 
     @property
     def ct_data(self):
         """ Return the connectivity table as a DataFrame. """
         # Make an index the same length as the section and starting
         # from 1 (CT files must start at index 1).
-        index = pd.RangeIndex(1, self.section.length + 1, name=self.IDX_FIELD)
+        index = pd.Index(self.section.range_int_one, name=self.IDX_FIELD)
         # Adjust the numbers of the paired bases (i.e. pairs > 0) such
         # that they also index from 1.
         pairs = self.partners.values.copy()
         pairs[pairs > 0] -= self.section.end5 - 1
         # Generate the data for the connectivity table.
         data = {
             self.BASE_FIELD: self.seq.to_str_array(),
-            self.PRIOR_FIELD: index.values - 1,
+            self.PREV_FIELD: index.values - 1,
             self.NEXT_FIELD: index.values + 1,
             self.PAIR_FIELD: pairs,
-            self.POS_FIELD: self.section.range,
+            self.POS_FIELD: self.section.range_int,
         }
         # Assemble the data into a DataFrame.
         return pd.DataFrame.from_dict({field: pd.Series(values, index=index)
                                        for field, values in data.items()})
 
     @property
     def ct_text(self):
```

### Comparing `seismic-rna-0.4.1/src/seismicrna/core/sect.py` & `seismic-rna-0.5.0/src/seismicrna/core/sect.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.1/src/seismicrna/core/sect_test.py` & `seismic-rna-0.5.0/src/seismicrna/core/sect_test.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.1/src/seismicrna/core/seq.py` & `seismic-rna-0.5.0/src/seismicrna/core/seq.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.1/src/seismicrna/core/seq_test.py` & `seismic-rna-0.5.0/src/seismicrna/core/seq_test.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.1/src/seismicrna/core/shell.py` & `seismic-rna-0.5.0/src/seismicrna/core/shell.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.1/src/seismicrna/core/sim.py` & `seismic-rna-0.5.0/src/seismicrna/core/sim.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.1/src/seismicrna/core/sim_test.py` & `seismic-rna-0.5.0/src/seismicrna/core/sim_test.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.1/src/seismicrna/core/types.py` & `seismic-rna-0.5.0/src/seismicrna/core/types.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.1/src/seismicrna/core/xam.py` & `seismic-rna-0.5.0/src/seismicrna/core/xam.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.1/src/seismicrna/demult/demultiplex.py` & `seismic-rna-0.5.0/src/seismicrna/demult/demultiplex.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.1/src/seismicrna/demult/main.py` & `seismic-rna-0.5.0/src/seismicrna/demult/main.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.1/src/seismicrna/draw/main.py` & `seismic-rna-0.5.0/src/seismicrna/draw/main.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.1/src/seismicrna/draw/manipulator.py` & `seismic-rna-0.5.0/src/seismicrna/draw/manipulator.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.1/src/seismicrna/draw/plotter.py` & `seismic-rna-0.5.0/src/seismicrna/draw/plotter.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.1/src/seismicrna/draw/study.py` & `seismic-rna-0.5.0/src/seismicrna/draw/study.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.1/src/seismicrna/draw/util.py` & `seismic-rna-0.5.0/src/seismicrna/draw/util.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.1/src/seismicrna/graph/base.py` & `seismic-rna-0.5.0/src/seismicrna/graph/base.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,28 @@
 from abc import ABC, abstractmethod
-from logging import getLogger
 from functools import cache, cached_property
+from logging import getLogger
 from pathlib import Path
 from typing import Any, Iterable
 
 from plotly import graph_objects as go
 from plotly.subplots import make_subplots
 
 from .color import ColorMap, get_cmap
 from ..core import path
 from ..core.seq import DNA
 from ..table.base import Table
-from ..table.load import load, TableLoader, PosTableLoader
+from ..table.load import TableLoader, PosTableLoader
 
 logger = getLogger(__name__)
 
-
 # Number of digits behind the decimal point to be kept.
 PRECISION = 6
 
 
-def find_tables(tables: tuple[str, ...]):
-    """ Return a file for each given file/directory of a table. """
-    return path.find_files_chain(map(Path, tables), [path.MutTabSeg])
-
-
 class GraphBase(ABC):
 
     def __init__(self, cmap: str | None = None):
         self._cmap_name = cmap
 
     @cached_property
     @abstractmethod
@@ -88,39 +82,48 @@
 
     @property
     @abstractmethod
     def ncols(self) -> int:
         """ Number of columns of subplots. """
 
     @property
-    @abstractmethod
-    def subplot_titles(self):
+    def row_titles(self) -> list[str] | None:
+        """ Title of each row. """
+        return None
+
+    @property
+    def col_titles(self) -> list[str] | None:
+        """ Title of each column. """
+        return None
+
+    @property
+    def subplot_titles(self) -> list[str] | None:
         """ Titles of the subplots. """
+        return None
+
+    def _get_subplots_params(self):
+        return dict(rows=self.nrows,
+                    cols=self.ncols,
+                    row_titles=self.row_titles,
+                    column_titles=self.col_titles)
 
     def _figure_init(self):
         """ Initialize the figure. """
-        return make_subplots(rows=self.nrows, cols=self.ncols)
+        return make_subplots(**self._get_subplots_params())
 
     def _figure_data(self, fig: go.Figure):
         """ Add data to the figure. """
         for (row, col), trace in self.get_traces():
             fig.add_trace(trace, row=row, col=col)
 
     def _figure_layout(self, fig: go.Figure):
         """ Update the figure's layout. """
         fig.update_layout(title=self.title,
                           plot_bgcolor="#ffffff",
                           paper_bgcolor="#ffffff")
-        fig.update_xaxes(linewidth=1,
-                         linecolor="#000000",
-                         autorange=True)
-        fig.update_yaxes(gridcolor="#d0d0d0",
-                         linewidth=1,
-                         linecolor="#000000",
-                         autorange=True)
 
     @cache
     def get_figure(self):
         """ Figure object. """
         fig = self._figure_init()
         self._figure_data(fig)
         self._figure_layout(fig)
@@ -161,16 +164,16 @@
         if html:
             files.append(self.write_html())
         if pdf:
             files.append(self.write_pdf())
         return files
 
 
-class OneSampGraph(GraphBase, ABC):
-    """ Graph of one sample. """
+class SampleGraph(GraphBase, ABC):
+    """ Graph of one or more samples. """
 
     @property
     @abstractmethod
     def sample(self):
         """ Name of the sample. """
         return ""
 
@@ -179,14 +182,38 @@
         """ Path segments. """
         return super().get_path_segs() + (path.SampSeg,)
 
     def get_path_fields(self):
         return {**super().get_path_fields(), path.SAMP: self.sample}
 
 
+class OneSampleGraph(SampleGraph, ABC):
+    """ Graph of one sample. """
+
+
+class TwoSampleGraph(SampleGraph, ABC):
+    """ Graph of two samples. """
+
+    @property
+    @abstractmethod
+    def sample1(self):
+        """ Name of the first sample. """
+        return ""
+
+    @property
+    @abstractmethod
+    def sample2(self):
+        """ Name of the second sample. """
+        return ""
+
+    @property
+    def sample(self):
+        return f"{self.sample1}_vs_{self.sample2}"
+
+
 class OneRefGraph(GraphBase, ABC):
     """ Graph of one reference.  """
 
     @property
     @abstractmethod
     def ref(self):
         """ Name of the reference sequence. """
@@ -215,42 +242,36 @@
     @property
     @abstractmethod
     def seq(self):
         """ Reference sequence as a DNA object. """
         return DNA(b"")
 
 
-class OneTableGraph(OneSampGraph, OneRefGraph, ABC):
+class OneTableGraph(OneSampleGraph, OneRefGraph, ABC):
     """ Graph of data from one TableLoader. """
 
-    def __init__(self):
-        super().__init__()
-        self._table = None
+    def __init__(self, *args, table: TableLoader, **kwargs):
+        super().__init__(*args, **kwargs)
+        if not isinstance(table, self.get_table_type()):
+            raise TypeError(f"{self.__class__.__name__} expected table "
+                            f"of type '{self.get_table_type().__name__}', "
+                            f"but got type '{type(table).__name__}'")
+        self._table = table
 
     @classmethod
     @abstractmethod
     def get_table_type(cls):
         """ Type of TableLoader for this graph. """
         return TableLoader
 
     @property
     def table(self) -> (TableLoader | PosTableLoader | Table):
         """ Table of data. """
-        if self._table is None:
-            raise TypeError("table not set")
         return self._table
 
-    @table.setter
-    def table(self, table: TableLoader):
-        if not isinstance(table, self.get_table_type()):
-            raise TypeError(f"{self.__class__.__name__} expected table "
-                            f"of type '{self.get_table_type().__name__}', "
-                            f"but got type '{type(table).__name__}'")
-        self._table = table
-
     @property
     def out_dir(self):
         return self.table.out_dir
 
     @property
     def sample(self):
         return self.table.sample
@@ -260,61 +281,133 @@
         return self.table.ref
 
     @property
     def sect(self):
         return self.table.sect
 
 
+class TwoTableGraph(TwoSampleGraph, OneRefGraph, ABC):
+
+    def __init__(self, *args, table1: TableLoader, table2: TableLoader,
+                 **kwargs):
+        super().__init__(*args, **kwargs)
+        for table, table_type in zip([table1,
+                                      table2],
+                                     [self.get_table1_type(),
+                                      self.get_table2_type()]):
+            if not isinstance(table, table_type):
+                raise TypeError(f"{self.__class__.__name__} expected table "
+                                f"of type '{table_type.__name__}', "
+                                f"but got type '{type(table).__name__}'")
+        self._table1 = table1
+        self._table2 = table2
+
+    @classmethod
+    @abstractmethod
+    def get_table1_type(cls):
+        """ Type of the first TableLoader for this graph. """
+        return TableLoader
+
+    @classmethod
+    @abstractmethod
+    def get_table2_type(cls):
+        """ Type of the second TableLoader for this graph. """
+        return TableLoader
+
+    @property
+    def table1(self) -> (TableLoader | PosTableLoader | Table):
+        """ First table of data. """
+        return self._table1
+
+    @property
+    def table2(self) -> (TableLoader | PosTableLoader | Table):
+        """ Second table of data. """
+        return self._table2
+
+    def _get_common_attribute(self, name: str):
+        """ Get the common attribute for tables 1 and 2. """
+        attr1 = self.table1.__getattribute__(name)
+        attr2 = self.table2.__getattribute__(name)
+        if attr1 != attr2:
+            raise ValueError(f"Attribute '{name}' differs between tables 1 "
+                             f"({repr(attr1)}) and 2 ({repr(attr2)})")
+        return attr1
+
+    @property
+    def out_dir(self):
+        return self._get_common_attribute("out_dir")
+
+    @property
+    def ref(self):
+        return self._get_common_attribute("ref")
+
+    @property
+    def sect(self):
+        return self._get_common_attribute("sect")
+
+    @property
+    def sample1(self):
+        return self.table1.sample
+
+    @property
+    def sample2(self):
+        return self.table2.sample
+
+    @property
+    def sample(self):
+        if self.sample1 == self.sample2:
+            return self.sample1
+        return f"{self.sample1}__and__{self.sample2}"
+
+
 class OneTableSeqGraph(OneTableGraph, OneSeqGraph, ABC):
 
     @classmethod
     def get_table_type(cls):
         return PosTableLoader
 
     @property
     def seq(self):
         return self.table.seq
 
 
+class TwoTableSeqGraph(TwoTableGraph, OneSeqGraph, ABC):
+
+    @classmethod
+    def get_table1_type(cls):
+        return PosTableLoader
+
+    @classmethod
+    def get_table2_type(cls):
+        return PosTableLoader
+
+    @property
+    def seq(self):
+        return self._get_common_attribute("seq")
+
+
 class CartesianGraph(GraphBase, ABC):
     """ Graph with one pair of x and y axes. """
 
     @property
     @abstractmethod
     def x_title(self) -> str:
         """ Title of the x-axis. """
 
     @property
     @abstractmethod
     def y_title(self) -> str:
         """ Title of the y-axis. """
 
-    def _figure_init(self):
-        return make_subplots(rows=self.nrows, cols=self.ncols,
-                             shared_xaxes="all", shared_yaxes="all",
-                             x_title=self.x_title, y_title=self.y_title,
-                             subplot_titles=self.subplot_titles)
-
-
-class GraphWriter(ABC):
-    """ Write the proper types of graphs for a given table. """
-
-    def __init__(self, table_file: Path):
-        self.table_file = table_file
+    def _figure_layout(self, fig: go.Figure):
+        super()._figure_layout(fig)
+        fig.update_xaxes(linewidth=1,
+                         linecolor="#000000",
+                         autorange=True)
+        fig.update_yaxes(linewidth=1,
+                         linecolor="#000000",
+                         autorange=True)
 
-    @cached_property
-    def table(self):
-        """ The table providing the data for the graph(s). """
-        return load(self.table_file)
-
-    @abstractmethod
-    def iter(self, *args, **kwargs):
-        """ Yield every graph for the table. """
-        yield GraphBase()
-
-    def write(self, *args, csv: bool, html: bool, pdf: bool, **kwargs):
-        """ Generate and write every graph for the table. """
-        # Get the paths for every graph.
-        paths = list()
-        for graph in self.iter(*args, **kwargs):
-            paths.extend(graph.write(csv=csv, html=html, pdf=pdf))
-        return paths
+    def _get_subplots_params(self):
+        return {**super()._get_subplots_params(),
+                **dict(shared_xaxes="all", shared_yaxes="all",
+                       x_title=self.x_title, y_title=self.y_title)}
```

### Comparing `seismic-rna-0.4.1/src/seismicrna/graph/color.py` & `seismic-rna-0.5.0/src/seismicrna/graph/color.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.1/src/seismicrna/graph/default.py` & `seismic-rna-0.5.0/src/seismicrna/graph/default.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from pathlib import Path
 
 from click import command
 
-from .base import find_tables, GraphWriter
-from .seq import run as run_pos
+from .base import find_tables, OneTableGraphWriter
+from .seqbar import run as run_pos
 from ..core import docdef, path
 from ..core.cli import (opt_table, opt_csv, opt_html, opt_pdf,
                         opt_max_procs, opt_parallel)
 
 
 params = [
     opt_table,
@@ -34,15 +34,15 @@
         max_procs: int,
         parallel: bool) -> list[Path]:
     """ Create the canonical set of graphs. """
     # Positional graphs.
     run_pos()
 
 
-class CanonicalGraphWriter(GraphWriter):
+class CanonicalGraphWriter(OneTableGraphWriter):
 
     def iter(self, fields: str, count: bool, stack: bool):
         if isinstance(self.table, RelPosTableLoader):
             if stack:
                 if count:
                     yield RelCountStackedPosBarGraph(table=self.table,
                                                      codes=fields)
```

### Comparing `seismic-rna-0.4.1/src/seismicrna/graph/hist.py` & `seismic-rna-0.5.0/src/seismicrna/graph/hist.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from pathlib import Path
 
 import numpy as np
 import pandas as pd
 from click import command
 from plotly import graph_objects as go
 
-from .base import (find_tables, GraphWriter, CartesianGraph, OneTableGraph,
-                   OneSampGraph)
+from .base import (find_tables, OneTableGraphWriter, CartesianGraph, OneTableGraph,
+                   OneSampleGraph)
 from .color import RelColorMap
 from ..core import docdef
 from ..core.cli import (arg_input_file, opt_rels,
                         opt_y_ratio, opt_hist_bins,
                         opt_csv, opt_html, opt_pdf,
                         opt_max_procs, opt_parallel)
 from ..core.parallel import dispatch
@@ -59,15 +59,15 @@
     return list(chain(*dispatch([writer.write for writer in writers],
                                 max_procs, parallel, pass_n_procs=False,
                                 kwargs=dict(fields=fields, count=y_ratio,
                                             group=group, bins=hist_bins,
                                             csv=csv, html=html, pdf=pdf))))
 
 
-class ReadHistogramWriter(GraphWriter):
+class ReadHistogramWriter(OneTableGraphWriter):
 
     def iter(self, fields: str, bins: int, count: bool, group: bool):
         if isinstance(self.table, RelReadTableLoader):
             if group:
                 yield RelReadHist(table=self.table, codes=fields,
                                   x_ratio=bins, y_ratio=count)
             else:
@@ -80,15 +80,15 @@
                                    x_ratio=bins, y_ratio=count)
             else:
                 for field in fields:
                     yield MaskReadHist(table=self.table, codes=field,
                                        x_ratio=bins, y_ratio=count)
 
 
-class ReadHistogram(CartesianGraph, OneTableGraph, OneSampGraph, ABC):
+class ReadHistogram(CartesianGraph, OneTableGraph, OneSampleGraph, ABC):
     """ Histogram of an attribute of reads. """
 
     def __init__(self, *args,
                  table: (Table | RelReadTableLoader
                          | MaskReadTableLoader | ClustReadTableLoader),
                  **kwargs):
         super().__init__(*args, **kwargs)
```

### Comparing `seismic-rna-0.4.1/src/seismicrna/image/logo.py` & `seismic-rna-0.5.0/src/seismicrna/image/logo.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.1/src/seismicrna/main.py` & `seismic-rna-0.5.0/src/seismicrna/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,15 +122,15 @@
         # Cluster options
         max_clusters: int,
         em_runs: int,
         min_em_iter: int,
         max_em_iter: int,
         em_thresh: float,
         # Table options
-        rels: str,
+        rels: tuple[str, ...],
         # Fold options
         fold: bool,
         quantile: float):
     """ Run entire pipeline. """
     # Demultiplexing
     if demult_on:
         for dms, dmi, dmm in demultiplex_mod.run(
```

### Comparing `seismic-rna-0.4.1/src/seismicrna/mask/load.py` & `seismic-rna-0.5.0/src/seismicrna/mask/load.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.1/src/seismicrna/mask/main.py` & `seismic-rna-0.5.0/src/seismicrna/mask/main.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.1/src/seismicrna/mask/report.py` & `seismic-rna-0.5.0/src/seismicrna/mask/report.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.1/src/seismicrna/mask/write.py` & `seismic-rna-0.5.0/src/seismicrna/mask/write.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.1/src/seismicrna/relate/export.py` & `seismic-rna-0.5.0/src/seismicrna/relate/export.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.1/src/seismicrna/relate/load.py` & `seismic-rna-0.5.0/src/seismicrna/relate/load.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.1/src/seismicrna/relate/main.py` & `seismic-rna-0.5.0/src/seismicrna/relate/main.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.1/src/seismicrna/relate/relate.py` & `seismic-rna-0.5.0/src/seismicrna/relate/relate.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.1/src/seismicrna/relate/report.py` & `seismic-rna-0.5.0/src/seismicrna/relate/report.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.1/src/seismicrna/relate/sam.py` & `seismic-rna-0.5.0/src/seismicrna/relate/sam.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.1/src/seismicrna/relate/seqpos.py` & `seismic-rna-0.5.0/src/seismicrna/relate/seqpos.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.1/src/seismicrna/relate/test.py` & `seismic-rna-0.5.0/src/seismicrna/relate/test.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.1/src/seismicrna/relate/write.py` & `seismic-rna-0.5.0/src/seismicrna/relate/write.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.1/src/seismicrna/struct/main.py` & `seismic-rna-0.5.0/src/seismicrna/struct/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -96,9 +96,9 @@
                     pass_n_procs=False)
 
 
 def fold_profile(rna: RnaProfile, out_dir: Path, quantile: float, **kwargs):
     """ Fold a section of an RNA from one mutational profile. """
     ct_file = fold(rna, out_dir=out_dir, quantile=quantile, **kwargs)
     dot_file = ct2dot(ct_file)
-    varnac_file = rna.to_varnac(out_dir, quantile)
-    return ct_file, dot_file, varnac_file
+    varna_color_file = rna.to_varna_color_file(out_dir, quantile)
+    return ct_file, dot_file, varna_color_file
```

### Comparing `seismic-rna-0.4.1/src/seismicrna/struct/rnastructure.py` & `seismic-rna-0.5.0/src/seismicrna/struct/rnastructure.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,23 +13,21 @@
 from ..core.shell import run_cmd, RNASTRUCTURE_FOLD_CMD
 
 logger = getLogger(__name__)
 
 
 def fold(rna: RnaProfile, *,
          out_dir: Path, temp_dir: Path, save_temp: bool,
-         quantile: float,
-         rerun: bool):
+         quantile: float, rerun: bool):
     """ Run the 'Fold' program of RNAstructure. """
     ct_file = rna.ct_file(out_dir)
     if rerun or not ct_file.is_file():
         cmd = [RNASTRUCTURE_FOLD_CMD]
-        if quantile > 0.:
-            # Write the DMS reactivities file for the RNA.
-            cmd.extend(["--DMS", rna.to_dms(temp_dir, quantile)])
+        # Write the DMS reactivities file for the RNA.
+        cmd.extend(["--DMS", rna.to_dms(temp_dir, quantile)])
         # Write a temporary FASTA file for the RNA.
         cmd.append(fasta := rna.to_fasta(temp_dir))
         try:
             # Get the path of the output CT file.
             cmd.append(ct_file)
             # Run the command.
             run_cmd(cmd, check_is_after=[ct_file])
```

### Comparing `seismic-rna-0.4.1/src/seismicrna/table/base.py` & `seismic-rna-0.5.0/src/seismicrna/table/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from pathlib import Path
 from typing import Any
 
 import pandas as pd
 
 from ..cluster.names import CLS_NAME, ORD_NAME
 from ..core import path
+from ..core.mu import winsorize
 from ..core.sect import index_to_pos, index_to_seq
 
 # General fields
 READ_TITLE = "Read Name"
 R_OBS_TITLE = "Reads Observed"
 R_ADJ_TITLE = "Reads Adjusted"
 REL_NAME = "Relationship"
@@ -142,40 +143,29 @@
     def _switch_rel(self, column: tuple, new_rel: str):
         """ Switch the relationship in a column label. """
         return new_rel,
 
     @cache
     def _count_col(self, column: tuple):
         """ Count the bits for a column. """
-        # Determine the relationship to count.
-        if column[self._rel_level_index] == INFOR_REL:
-            # Sum the matched and mutated bits.
-            match_col = self._switch_rel(column, MATCH_REL)
-            mutat_col = self._switch_rel(column, MUTAT_REL)
-            return self._count_col(match_col) + self._count_col(mutat_col)
-        try:
-            # The relationship should appear in the table, so return it
-            # as a Series.
-            return self.data.loc[:, column].squeeze()
-        except KeyError:
-            # Suppress exception chaining.
-            pass
-        raise ValueError(f"{self} was not built with column {column}")
+        return self.data.loc[:, column].squeeze()
 
     @cache
-    def _ratio_col(self, column: tuple, precision: int | None = None):
+    def _ratio_col(self, column: tuple, quantile: float, precision: int | None):
         """ Compute the ratio for a column. """
         # Determine the relationship to use as the numerator.
         numer_rel = column[self._rel_level_index]
         # Determine the relationship to use as the denominator.
         denom_rel = COVER_REL if numer_rel == INFOR_REL else INFOR_REL
         # Determine the column to use as the denominator.
         denom_col = self._switch_rel(column, denom_rel)
         # Compute the ratio of the numerator and the denominator.
         ratio = self._count_col(column) / self._count_col(denom_col)
+        # If a quantile was given, then winsorize to it.
+        ratio = winsorize(ratio, quantile)
         # Round the ratio to the desired precision.
         if precision is not None:
             ratio = ratio.round(precision)
         return ratio
 
     @staticmethod
     def _format_selection(**kwargs) -> dict[str, list]:
@@ -190,24 +180,27 @@
                 pass
         return selection
 
     def _get_indexer(self, selection: dict[str, list]):
         """ Format a column selection into a column indexer. """
         return selection.get(REL_NAME, slice(None))
 
-    def select(self, ratio: bool, precision: int | None = None, **kwargs: list):
+    def select(self, ratio: bool,
+               quantile: float = -1.,
+               precision: int | None = None,
+               **kwargs: list):
         """ Output selected data from the table as a DataFrame. """
         # Instantiate an empty DataFrame with the index and columns.
         indexer = self._get_indexer(self._format_selection(**kwargs))
         columns = self.data.loc[:, indexer].columns
         data = pd.DataFrame(index=self.data.index, columns=columns, dtype=float)
         # Fill in the DataFrame one column at a time.
         for column in columns:
-            data.loc[:, column] = (self._ratio_col(column, precision) if ratio
-                                   else self._count_col(column))
+            data.loc[:, column] = (self._ratio_col(column, quantile, precision)
+                                   if ratio else self._count_col(column))
         return data
 
 
 # Table by Source (relate/mask/cluster) ################################
 
 class RelTable(RelTypeTable, ABC):
     pass
```

### Comparing `seismic-rna-0.4.1/src/seismicrna/table/load.py` & `seismic-rna-0.5.0/src/seismicrna/table/load.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 import pandas as pd
 
 from .base import (MUTAT_REL, CLUST_INDEX_NAMES, REL_NAME,
                    Table, RelTypeTable, PosTable, ReadTable,
                    RelPosTable, RelReadTable,
                    MaskPosTable, MaskReadTable,
                    ClustPosTable, ClustReadTable, ClustFreqTable)
-from ..cluster.names import ENSEMBLE_NAME, ORD_CLS_NAME, fmt_clust_name
+from ..cluster.names import (ENSEMBLE_NAME, ORD_NAME, CLS_NAME, ORD_CLS_NAME,
+                             fmt_clust_name)
 from ..core import path
 from ..core.rna import RnaProfile
 from ..core.sect import Section, INDEX_NAMES
 
 
 # Table Loader Base Classes ############################################
 
@@ -67,29 +68,29 @@
 
 class RelTypeTableLoader(TableLoader, RelTypeTable, ABC):
     """ Load a table of relationship types. """
 
 
 # Load by Index (position/read/frequency) ##############################
 
-class PosTableLoader(TableLoader, PosTable, ABC):
+class PosTableLoader(RelTypeTableLoader, PosTable, ABC):
     """ Load data indexed by position. """
 
     @classmethod
     def index_col(cls):
         return list(range(len(INDEX_NAMES)))
 
     @abstractmethod
     def iter_profiles(self, sections: Iterable[Section]):
         """ Yield RNA mutational profiles from the table. """
         for section in sections:
             yield RnaProfile("", section, "", "", pd.Series())
 
 
-class ReadTableLoader(TableLoader, ReadTable, ABC):
+class ReadTableLoader(RelTypeTableLoader, ReadTable, ABC):
     """ Load data indexed by read. """
 
     @classmethod
     def index_col(cls):
         return 0
 
 
@@ -201,14 +202,19 @@
         # Reformat the index of clusters.
         data.index = reformat_cluster_index(data.index)
         return data
 
 
 # Helper Functions #####################################################
 
+def find_tables(tables: tuple[str, ...]):
+    """ Return a file for each given file/directory of a table. """
+    return path.find_files_chain(map(Path, tables), [path.MutTabSeg])
+
+
 def load(table_file: Path):
     """ Helper function to load a TableLoader from a table file. """
     for loader_type in (RelPosTableLoader, RelReadTableLoader,
                         MaskPosTableLoader, MaskReadTableLoader,
                         ClustPosTableLoader, ClustReadTableLoader,
                         ClustFreqTableLoader):
         try:
@@ -225,7 +231,24 @@
     """ Ensure that the columns are a MultiIndex and that the order and
     cluster numbers are integers, not strings. """
     return pd.MultiIndex.from_arrays(
         [index.get_level_values(n).astype(int if n in ORD_CLS_NAME else str)
          for n in index.names],
         names=index.names
     )
+
+
+def get_clusters(columns: pd.Index | pd.MultiIndex, allow_zero: bool = False):
+    """ Return a MultiIndex of non-redundant orders and cluster numbers
+    from columns with order and cluster numbers as levels. """
+    try:
+        return pd.MultiIndex.from_arrays([columns.get_level_values(level)
+                                          for level in ORD_CLS_NAME],
+                                         names=ORD_CLS_NAME).drop_duplicates()
+    except KeyError:
+        # The index did not contain levels named "order" and "cluster".
+        if allow_zero:
+            # Default to an index of zero for each level.
+            return pd.MultiIndex.from_tuples([(0,) * len(ORD_CLS_NAME)],
+                                             names=ORD_CLS_NAME)
+        # Re-raise the error.
+        raise
```

### Comparing `seismic-rna-0.4.1/src/seismicrna/table/main.py` & `seismic-rna-0.5.0/src/seismicrna/table/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+from collections import Counter
 from itertools import chain
 from logging import getLogger
 from pathlib import Path
+from typing import Iterable
 
 from click import command
 
 from .write import write
 from ..core import docdef, path
 from ..core.cli import (arg_input_file, opt_rels,
                         opt_max_procs, opt_parallel, opt_rerun)
@@ -19,28 +21,37 @@
 def cli(*args, **kwargs):
     """ Tabulate per-base and per-read mutation counts from 'relate' and
     'mask', and mutation rates and read memberships from 'cluster'. """
     return run(*args, **kwargs)
 
 
 @docdef.auto()
-def run(input_file: tuple[str, ...], rels: str,
+def run(input_file: tuple[str, ...], rels: tuple[str, ...],
         max_procs: int, parallel: bool, **kwargs):
     """
     Run the table module.
     """
     report_files = list(map(Path, input_file))
     relate_reports = path.find_files_chain(report_files, [path.RelateRepSeg])
     if relate_reports:
         logger.debug(f"Found relate report files: {relate_reports}")
     mask_reports = path.find_files_chain(report_files, [path.MaskRepSeg])
     if mask_reports:
         logger.debug(f"Found mask report files: {mask_reports}")
     clust_reports = path.find_files_chain(report_files, [path.ClustRepSeg])
     if clust_reports:
         logger.debug(f"Found cluster report files: {clust_reports}")
-    tasks = [(file, rels) for file in chain(relate_reports,
-                                            mask_reports,
-                                            clust_reports)]
+    rels_str = join_rels(rels)
+    tasks = [(file, rels_str) for file in chain(relate_reports,
+                                                mask_reports,
+                                                clust_reports)]
     return list(chain(*dispatch(write, max_procs, parallel,
                                 args=tasks, kwargs=kwargs,
                                 pass_n_procs=False)))
+
+
+def join_rels(rels: Iterable[str]):
+    """ Join relationships into one string. """
+    counts = Counter(r for rel in rels for r in rel)
+    if dups := [item for item, count in counts.items() if count > 1]:
+        logger.warning(f"Got duplicate relationships: {dups}")
+    return "".join(counts)
```

### Comparing `seismic-rna-0.4.1/src/seismicrna/table/tabulate.py` & `seismic-rna-0.5.0/src/seismicrna/table/tabulate.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.1/src/seismicrna/table/write.py` & `seismic-rna-0.5.0/src/seismicrna/table/write.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.1/src/seismicrna/test/main.py` & `seismic-rna-0.5.0/src/seismicrna/test/main.py`

 * *Files identical despite different names*

