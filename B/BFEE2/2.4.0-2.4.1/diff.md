# Comparing `tmp/BFEE2-2.4.0.tar.gz` & `tmp/BFEE2-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BFEE2-2.4.0.tar", last modified: Mon Jun  5 06:32:34 2023, max compression
+gzip compressed data, was "BFEE2-2.4.1.tar", last modified: Tue Jul 25 01:39:32 2023, max compression
```

## Comparing `BFEE2-2.4.0.tar` & `BFEE2-2.4.1.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxrwxr-x   0 chinfo    (1000) chinfo    (1000)        0 2023-06-05 06:32:34.181026 BFEE2-2.4.0/
-drwxrwxr-x   0 chinfo    (1000) chinfo    (1000)        0 2023-06-05 06:32:34.173025 BFEE2-2.4.0/BFEE2/
--rw-rw-r--   0 chinfo    (1000) chinfo    (1000)        0 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/__init__.py
-drwxrwxr-x   0 chinfo    (1000) chinfo    (1000)        0 2023-06-05 06:32:34.173025 BFEE2-2.4.0/BFEE2/commonTools/
--rw-rw-r--   0 chinfo    (1000) chinfo    (1000)        0 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/commonTools/__init__.py
--rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     1450 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/commonTools/commonSlots.py
--rw-rw-r--   0 chinfo    (1000) chinfo    (1000)    11005 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/commonTools/fileParser.py
--rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     5677 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/commonTools/ploter.py
-drwxrwxr-x   0 chinfo    (1000) chinfo    (1000)        0 2023-06-05 06:32:34.173025 BFEE2-2.4.0/BFEE2/doc/
--rw-rw-r--   0 chinfo    (1000) chinfo    (1000)   143522 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/doc/Doc.pdf
--rw-rw-r--   0 chinfo    (1000) chinfo    (1000)        1 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/doc/__init__.py
--rw-rw-r--   0 chinfo    (1000) chinfo    (1000)    99397 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/gui.py
--rw-rw-r--   0 chinfo    (1000) chinfo    (1000)   130682 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/inputGenerator.py
--rw-rw-r--   0 chinfo    (1000) chinfo    (1000)    20408 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/postTreatment.py
-drwxrwxr-x   0 chinfo    (1000) chinfo    (1000)        0 2023-06-05 06:32:34.177026 BFEE2-2.4.0/BFEE2/templates_gromacs/
--rw-rw-r--   0 chinfo    (1000) chinfo    (1000)      654 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_gromacs/000.colvars.template
--rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     1124 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_gromacs/000.generate_tpr_sh.template
--rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     1516 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_gromacs/000.mdp.template
--rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     1595 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_gromacs/001.colvars.template
--rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     1124 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_gromacs/001.generate_tpr_sh.template
--rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     1516 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_gromacs/001.mdp.template
--rw-rw-r--   0 chinfo    (1000) chinfo    (1000)        2 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_gromacs/001.readme.template
--rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     2169 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_gromacs/002.colvars.template
--rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     1124 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_gromacs/002.generate_tpr_sh.template
--rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     1516 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_gromacs/002.mdp.template
--rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     2708 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_gromacs/003.colvars.template
--rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     1397 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_gromacs/003.generate_tpr_sh.template
--rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     1516 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_gromacs/003.mdp.template
--rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     3300 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_gromacs/004.colvars.template
--rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     1525 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_gromacs/004.generate_tpr_sh.template
--rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     1516 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_gromacs/004.mdp.template
--rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     3809 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_gromacs/005.colvars.template
--rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     1653 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_gromacs/005.generate_tpr_sh.template
--rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     1516 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_gromacs/005.mdp.template
--rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     4260 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_gromacs/006.colvars.template
--rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     1781 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_gromacs/006.generate_tpr_sh.template
--rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     1516 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_gromacs/006.mdp.template
--rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     4512 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_gromacs/007.colvars.template
--rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     1909 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_gromacs/007.generate_tpr_sh.template
--rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     1497 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_gromacs/007.mdp.template
--rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     3584 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_gromacs/007_eq.colvars.template
--rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     3118 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_gromacs/007_eq.generate_tpr_sh.template
--rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     1181 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_gromacs/007_min.mdp.template
--rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     1044 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_gromacs/008.colvars.template
--rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     1124 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_gromacs/008.generate_tpr_sh.template
--rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     1516 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_gromacs/008.mdp.template
--rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     1079 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_gromacs/008_eq.generate_tpr_sh.template
--rw-rw-r--   0 chinfo    (1000) chinfo    (1000)    74395 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_gromacs/BFEEGromacs.py
--rw-rw-r--   0 chinfo    (1000) chinfo    (1000)        0 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_gromacs/__init__.py
--rw-rw-r--   0 chinfo    (1000) chinfo    (1000)      394 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_gromacs/find_min_max.awk
-drwxrwxr-x   0 chinfo    (1000) chinfo    (1000)        0 2023-06-05 06:32:34.177026 BFEE2-2.4.0/BFEE2/templates_namd/
--rw-rw-r--   0 chinfo    (1000) chinfo    (1000)        0 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_namd/__init__.py
--rw-rw-r--   0 chinfo    (1000) chinfo    (1000)    44797 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_namd/configTemplate.py
--rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     8601 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_namd/fep.tcl
--rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     4809 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_namd/scriptTemplate.py
--rw-rw-r--   0 chinfo    (1000) chinfo    (1000)      302 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_namd/solvate.tcl
--rw-rw-r--   0 chinfo    (1000) chinfo    (1000)      298 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_namd/solvate_mem.tcl
--rw-rw-r--   0 chinfo    (1000) chinfo    (1000)    10591 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_namd/updateCenters.py
-drwxrwxr-x   0 chinfo    (1000) chinfo    (1000)        0 2023-06-05 06:32:34.181026 BFEE2-2.4.0/BFEE2/templates_readme/
--rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     1027 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_readme/Readme_Gromacs_Geometrical.txt
--rw-rw-r--   0 chinfo    (1000) chinfo    (1000)      879 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_readme/Readme_NAMD_Alchemical.txt
--rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     1492 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_readme/Readme_NAMD_Geometrical.txt
--rw-rw-r--   0 chinfo    (1000) chinfo    (1000)        1 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/templates_readme/__init__.py
-drwxrwxr-x   0 chinfo    (1000) chinfo    (1000)        0 2023-06-05 06:32:34.181026 BFEE2-2.4.0/BFEE2/third_party/
--rw-rw-r--   0 chinfo    (1000) chinfo    (1000)        0 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/third_party/__init__.py
--rw-rw-r--   0 chinfo    (1000) chinfo    (1000)    14923 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/third_party/py_bar.py
--rw-rw-r--   0 chinfo    (1000) chinfo    (1000)       49 2023-06-05 06:17:23.000000 BFEE2-2.4.0/BFEE2/version.py
-drwxrwxr-x   0 chinfo    (1000) chinfo    (1000)        0 2023-06-05 06:32:34.173025 BFEE2-2.4.0/BFEE2.egg-info/
--rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     5059 2023-06-05 06:32:33.000000 BFEE2-2.4.0/BFEE2.egg-info/PKG-INFO
--rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     2581 2023-06-05 06:32:33.000000 BFEE2-2.4.0/BFEE2.egg-info/SOURCES.txt
--rw-rw-r--   0 chinfo    (1000) chinfo    (1000)        1 2023-06-05 06:32:33.000000 BFEE2-2.4.0/BFEE2.egg-info/dependency_links.txt
--rw-rw-r--   0 chinfo    (1000) chinfo    (1000)       68 2023-06-05 06:32:33.000000 BFEE2-2.4.0/BFEE2.egg-info/requires.txt
--rw-rw-r--   0 chinfo    (1000) chinfo    (1000)        6 2023-06-05 06:32:33.000000 BFEE2-2.4.0/BFEE2.egg-info/top_level.txt
--rw-rw-r--   0 chinfo    (1000) chinfo    (1000)    35349 2023-06-05 06:17:23.000000 BFEE2-2.4.0/LICENSE
--rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     5059 2023-06-05 06:32:34.181026 BFEE2-2.4.0/PKG-INFO
--rw-rw-r--   0 chinfo    (1000) chinfo    (1000)     4659 2023-06-05 06:17:23.000000 BFEE2-2.4.0/README.md
-drwxrwxr-x   0 chinfo    (1000) chinfo    (1000)        0 2023-06-05 06:32:34.181026 BFEE2-2.4.0/bin/
--rwxr-xr-x   0 chinfo    (1000) chinfo    (1000)      468 2023-06-05 06:17:23.000000 BFEE2-2.4.0/bin/BFEE2Gui.py
--rw-rw-r--   0 chinfo    (1000) chinfo    (1000)      104 2023-06-05 06:17:23.000000 BFEE2-2.4.0/pyproject.toml
--rw-rw-r--   0 chinfo    (1000) chinfo    (1000)      683 2023-06-05 06:32:34.181026 BFEE2-2.4.0/setup.cfg
--rw-rw-r--   0 chinfo    (1000) chinfo    (1000)      247 2023-06-05 06:17:23.000000 BFEE2-2.4.0/setup.py
+drwxrwxr-x   0 chinfo    (1001) chinfo    (1001)        0 2023-07-25 01:39:32.097076 BFEE2-2.4.1/
+drwxrwxr-x   0 chinfo    (1001) chinfo    (1001)        0 2023-07-25 01:39:32.093076 BFEE2-2.4.1/BFEE2/
+-rw-rw-r--   0 chinfo    (1001) chinfo    (1001)        0 2023-07-24 14:48:15.000000 BFEE2-2.4.1/BFEE2/__init__.py
+drwxrwxr-x   0 chinfo    (1001) chinfo    (1001)        0 2023-07-25 01:39:32.093076 BFEE2-2.4.1/BFEE2/commonTools/
+-rw-rw-r--   0 chinfo    (1001) chinfo    (1001)        0 2023-07-24 14:48:15.000000 BFEE2-2.4.1/BFEE2/commonTools/__init__.py
+-rw-rw-r--   0 chinfo    (1001) chinfo    (1001)     1450 2023-07-24 14:48:15.000000 BFEE2-2.4.1/BFEE2/commonTools/commonSlots.py
+-rw-rw-r--   0 chinfo    (1001) chinfo    (1001)    11005 2023-07-24 14:48:15.000000 BFEE2-2.4.1/BFEE2/commonTools/fileParser.py
+-rw-rw-r--   0 chinfo    (1001) chinfo    (1001)     5677 2023-07-24 14:48:15.000000 BFEE2-2.4.1/BFEE2/commonTools/ploter.py
+drwxrwxr-x   0 chinfo    (1001) chinfo    (1001)        0 2023-07-25 01:39:32.093076 BFEE2-2.4.1/BFEE2/doc/
+-rw-rw-r--   0 chinfo    (1001) chinfo    (1001)   143522 2023-07-24 14:48:15.000000 BFEE2-2.4.1/BFEE2/doc/Doc.pdf
+-rw-rw-r--   0 chinfo    (1001) chinfo    (1001)        1 2023-07-24 14:48:15.000000 BFEE2-2.4.1/BFEE2/doc/__init__.py
+-rw-rw-r--   0 chinfo    (1001) chinfo    (1001)    99397 2023-07-24 14:48:15.000000 BFEE2-2.4.1/BFEE2/gui.py
+-rw-rw-r--   0 chinfo    (1001) chinfo    (1001)   130682 2023-07-24 14:48:15.000000 BFEE2-2.4.1/BFEE2/inputGenerator.py
+-rw-rw-r--   0 chinfo    (1001) chinfo    (1001)    20408 2023-07-24 14:48:15.000000 BFEE2-2.4.1/BFEE2/postTreatment.py
+drwxrwxr-x   0 chinfo    (1001) chinfo    (1001)        0 2023-07-25 01:39:32.097076 BFEE2-2.4.1/BFEE2/templates_gromacs/
+-rw-rw-r--   0 chinfo    (1001) chinfo    (1001)      654 2023-07-24 14:48:15.000000 BFEE2-2.4.1/BFEE2/templates_gromacs/000.colvars.template
+-rw-rw-r--   0 chinfo    (1001) chinfo    (1001)     1124 2023-07-24 14:48:15.000000 BFEE2-2.4.1/BFEE2/templates_gromacs/000.generate_tpr_sh.template
+-rw-rw-r--   0 chinfo    (1001) chinfo    (1001)     1516 2023-07-24 14:48:15.000000 BFEE2-2.4.1/BFEE2/templates_gromacs/000.mdp.template
+-rw-rw-r--   0 chinfo    (1001) chinfo    (1001)     1595 2023-07-24 14:48:15.000000 BFEE2-2.4.1/BFEE2/templates_gromacs/001.colvars.template
+-rw-rw-r--   0 chinfo    (1001) chinfo    (1001)     1124 2023-07-24 14:48:15.000000 BFEE2-2.4.1/BFEE2/templates_gromacs/001.generate_tpr_sh.template
+-rw-rw-r--   0 chinfo    (1001) chinfo    (1001)     1516 2023-07-24 14:48:15.000000 BFEE2-2.4.1/BFEE2/templates_gromacs/001.mdp.template
+-rw-rw-r--   0 chinfo    (1001) chinfo    (1001)        2 2023-07-24 14:48:15.000000 BFEE2-2.4.1/BFEE2/templates_gromacs/001.readme.template
+-rw-rw-r--   0 chinfo    (1001) chinfo    (1001)     2169 2023-07-24 14:48:15.000000 BFEE2-2.4.1/BFEE2/templates_gromacs/002.colvars.template
+-rw-rw-r--   0 chinfo    (1001) chinfo    (1001)     1124 2023-07-24 14:48:15.000000 BFEE2-2.4.1/BFEE2/templates_gromacs/002.generate_tpr_sh.template
+-rw-rw-r--   0 chinfo    (1001) chinfo    (1001)     1516 2023-07-24 14:48:15.000000 BFEE2-2.4.1/BFEE2/templates_gromacs/002.mdp.template
+-rw-rw-r--   0 chinfo    (1001) chinfo    (1001)     2708 2023-07-24 14:48:15.000000 BFEE2-2.4.1/BFEE2/templates_gromacs/003.colvars.template
+-rw-rw-r--   0 chinfo    (1001) chinfo    (1001)     1397 2023-07-24 14:48:15.000000 BFEE2-2.4.1/BFEE2/templates_gromacs/003.generate_tpr_sh.template
+-rw-rw-r--   0 chinfo    (1001) chinfo    (1001)     1516 2023-07-24 14:48:15.000000 BFEE2-2.4.1/BFEE2/templates_gromacs/003.mdp.template
+-rw-rw-r--   0 chinfo    (1001) chinfo    (1001)     3300 2023-07-24 14:48:15.000000 BFEE2-2.4.1/BFEE2/templates_gromacs/004.colvars.template
+-rw-rw-r--   0 chinfo    (1001) chinfo    (1001)     1525 2023-07-24 14:48:15.000000 BFEE2-2.4.1/BFEE2/templates_gromacs/004.generate_tpr_sh.template
+-rw-rw-r--   0 chinfo    (1001) chinfo    (1001)     1516 2023-07-24 14:48:15.000000 BFEE2-2.4.1/BFEE2/templates_gromacs/004.mdp.template
+-rw-rw-r--   0 chinfo    (1001) chinfo    (1001)     3809 2023-07-24 14:48:15.000000 BFEE2-2.4.1/BFEE2/templates_gromacs/005.colvars.template
+-rw-rw-r--   0 chinfo    (1001) chinfo    (1001)     1653 2023-07-24 14:48:15.000000 BFEE2-2.4.1/BFEE2/templates_gromacs/005.generate_tpr_sh.template
+-rw-rw-r--   0 chinfo    (1001) chinfo    (1001)     1516 2023-07-24 14:48:15.000000 BFEE2-2.4.1/BFEE2/templates_gromacs/005.mdp.template
+-rw-rw-r--   0 chinfo    (1001) chinfo    (1001)     4260 2023-07-24 14:48:15.000000 BFEE2-2.4.1/BFEE2/templates_gromacs/006.colvars.template
+-rw-rw-r--   0 chinfo    (1001) chinfo    (1001)     1781 2023-07-24 14:48:15.000000 BFEE2-2.4.1/BFEE2/templates_gromacs/006.generate_tpr_sh.template
+-rw-rw-r--   0 chinfo    (1001) chinfo    (1001)     1516 2023-07-24 14:48:15.000000 BFEE2-2.4.1/BFEE2/templates_gromacs/006.mdp.template
+-rw-rw-r--   0 chinfo    (1001) chinfo    (1001)     4512 2023-07-24 14:48:15.000000 BFEE2-2.4.1/BFEE2/templates_gromacs/007.colvars.template
+-rw-rw-r--   0 chinfo    (1001) chinfo    (1001)     1909 2023-07-24 14:48:15.000000 BFEE2-2.4.1/BFEE2/templates_gromacs/007.generate_tpr_sh.template
+-rw-rw-r--   0 chinfo    (1001) chinfo    (1001)     1497 2023-07-24 14:48:15.000000 BFEE2-2.4.1/BFEE2/templates_gromacs/007.mdp.template
+-rw-rw-r--   0 chinfo    (1001) chinfo    (1001)     3584 2023-07-24 14:48:15.000000 BFEE2-2.4.1/BFEE2/templates_gromacs/007_eq.colvars.template
+-rw-rw-r--   0 chinfo    (1001) chinfo    (1001)     3118 2023-07-24 14:48:15.000000 BFEE2-2.4.1/BFEE2/templates_gromacs/007_eq.generate_tpr_sh.template
+-rw-rw-r--   0 chinfo    (1001) chinfo    (1001)     1181 2023-07-24 14:48:15.000000 BFEE2-2.4.1/BFEE2/templates_gromacs/007_min.mdp.template
+-rw-rw-r--   0 chinfo    (1001) chinfo    (1001)     1044 2023-07-24 14:48:15.000000 BFEE2-2.4.1/BFEE2/templates_gromacs/008.colvars.template
+-rw-rw-r--   0 chinfo    (1001) chinfo    (1001)     1124 2023-07-24 14:48:15.000000 BFEE2-2.4.1/BFEE2/templates_gromacs/008.generate_tpr_sh.template
+-rw-rw-r--   0 chinfo    (1001) chinfo    (1001)     1516 2023-07-24 14:48:15.000000 BFEE2-2.4.1/BFEE2/templates_gromacs/008.mdp.template
+-rw-rw-r--   0 chinfo    (1001) chinfo    (1001)     1079 2023-07-24 14:48:15.000000 BFEE2-2.4.1/BFEE2/templates_gromacs/008_eq.generate_tpr_sh.template
+-rw-rw-r--   0 chinfo    (1001) chinfo    (1001)    74395 2023-07-24 14:48:15.000000 BFEE2-2.4.1/BFEE2/templates_gromacs/BFEEGromacs.py
+-rw-rw-r--   0 chinfo    (1001) chinfo    (1001)        0 2023-07-24 14:48:15.000000 BFEE2-2.4.1/BFEE2/templates_gromacs/__init__.py
+-rw-rw-r--   0 chinfo    (1001) chinfo    (1001)      394 2023-07-24 14:48:15.000000 BFEE2-2.4.1/BFEE2/templates_gromacs/find_min_max.awk
+drwxrwxr-x   0 chinfo    (1001) chinfo    (1001)        0 2023-07-25 01:39:32.097076 BFEE2-2.4.1/BFEE2/templates_namd/
+-rw-rw-r--   0 chinfo    (1001) chinfo    (1001)        0 2023-07-24 14:48:15.000000 BFEE2-2.4.1/BFEE2/templates_namd/__init__.py
+-rw-rw-r--   0 chinfo    (1001) chinfo    (1001)    44835 2023-07-24 14:48:15.000000 BFEE2-2.4.1/BFEE2/templates_namd/configTemplate.py
+-rw-rw-r--   0 chinfo    (1001) chinfo    (1001)     8601 2023-07-24 14:48:15.000000 BFEE2-2.4.1/BFEE2/templates_namd/fep.tcl
+-rw-rw-r--   0 chinfo    (1001) chinfo    (1001)     4809 2023-07-24 14:48:15.000000 BFEE2-2.4.1/BFEE2/templates_namd/scriptTemplate.py
+-rw-rw-r--   0 chinfo    (1001) chinfo    (1001)      302 2023-07-24 14:48:15.000000 BFEE2-2.4.1/BFEE2/templates_namd/solvate.tcl
+-rw-rw-r--   0 chinfo    (1001) chinfo    (1001)      298 2023-07-24 14:48:15.000000 BFEE2-2.4.1/BFEE2/templates_namd/solvate_mem.tcl
+-rw-rw-r--   0 chinfo    (1001) chinfo    (1001)    10591 2023-07-24 14:48:15.000000 BFEE2-2.4.1/BFEE2/templates_namd/updateCenters.py
+drwxrwxr-x   0 chinfo    (1001) chinfo    (1001)        0 2023-07-25 01:39:32.097076 BFEE2-2.4.1/BFEE2/templates_readme/
+-rw-rw-r--   0 chinfo    (1001) chinfo    (1001)     1027 2023-07-24 14:48:15.000000 BFEE2-2.4.1/BFEE2/templates_readme/Readme_Gromacs_Geometrical.txt
+-rw-rw-r--   0 chinfo    (1001) chinfo    (1001)      879 2023-07-24 14:48:15.000000 BFEE2-2.4.1/BFEE2/templates_readme/Readme_NAMD_Alchemical.txt
+-rw-rw-r--   0 chinfo    (1001) chinfo    (1001)     1492 2023-07-24 14:48:15.000000 BFEE2-2.4.1/BFEE2/templates_readme/Readme_NAMD_Geometrical.txt
+-rw-rw-r--   0 chinfo    (1001) chinfo    (1001)        1 2023-07-24 14:48:15.000000 BFEE2-2.4.1/BFEE2/templates_readme/__init__.py
+drwxrwxr-x   0 chinfo    (1001) chinfo    (1001)        0 2023-07-25 01:39:32.097076 BFEE2-2.4.1/BFEE2/third_party/
+-rw-rw-r--   0 chinfo    (1001) chinfo    (1001)        0 2023-07-24 14:48:15.000000 BFEE2-2.4.1/BFEE2/third_party/__init__.py
+-rw-rw-r--   0 chinfo    (1001) chinfo    (1001)    14923 2023-07-24 14:48:15.000000 BFEE2-2.4.1/BFEE2/third_party/py_bar.py
+-rw-rw-r--   0 chinfo    (1001) chinfo    (1001)       49 2023-07-24 14:48:15.000000 BFEE2-2.4.1/BFEE2/version.py
+drwxrwxr-x   0 chinfo    (1001) chinfo    (1001)        0 2023-07-25 01:39:32.093076 BFEE2-2.4.1/BFEE2.egg-info/
+-rw-rw-r--   0 chinfo    (1001) chinfo    (1001)     5059 2023-07-25 01:39:32.000000 BFEE2-2.4.1/BFEE2.egg-info/PKG-INFO
+-rw-rw-r--   0 chinfo    (1001) chinfo    (1001)     2581 2023-07-25 01:39:32.000000 BFEE2-2.4.1/BFEE2.egg-info/SOURCES.txt
+-rw-rw-r--   0 chinfo    (1001) chinfo    (1001)        1 2023-07-25 01:39:32.000000 BFEE2-2.4.1/BFEE2.egg-info/dependency_links.txt
+-rw-rw-r--   0 chinfo    (1001) chinfo    (1001)       68 2023-07-25 01:39:32.000000 BFEE2-2.4.1/BFEE2.egg-info/requires.txt
+-rw-rw-r--   0 chinfo    (1001) chinfo    (1001)        6 2023-07-25 01:39:32.000000 BFEE2-2.4.1/BFEE2.egg-info/top_level.txt
+-rw-rw-r--   0 chinfo    (1001) chinfo    (1001)    35349 2023-07-24 14:48:15.000000 BFEE2-2.4.1/LICENSE
+-rw-rw-r--   0 chinfo    (1001) chinfo    (1001)     5059 2023-07-25 01:39:32.097076 BFEE2-2.4.1/PKG-INFO
+-rw-rw-r--   0 chinfo    (1001) chinfo    (1001)     4659 2023-07-24 14:48:15.000000 BFEE2-2.4.1/README.md
+drwxrwxr-x   0 chinfo    (1001) chinfo    (1001)        0 2023-07-25 01:39:32.097076 BFEE2-2.4.1/bin/
+-rwxr-xr-x   0 chinfo    (1001) chinfo    (1001)      468 2023-07-24 14:48:15.000000 BFEE2-2.4.1/bin/BFEE2Gui.py
+-rw-rw-r--   0 chinfo    (1001) chinfo    (1001)      104 2023-07-24 14:48:15.000000 BFEE2-2.4.1/pyproject.toml
+-rw-rw-r--   0 chinfo    (1001) chinfo    (1001)      683 2023-07-25 01:39:32.101076 BFEE2-2.4.1/setup.cfg
+-rw-rw-r--   0 chinfo    (1001) chinfo    (1001)      247 2023-07-24 14:48:15.000000 BFEE2-2.4.1/setup.py
```

### Comparing `BFEE2-2.4.0/BFEE2/commonTools/commonSlots.py` & `BFEE2-2.4.1/BFEE2/commonTools/commonSlots.py`

 * *Files identical despite different names*

### Comparing `BFEE2-2.4.0/BFEE2/commonTools/fileParser.py` & `BFEE2-2.4.1/BFEE2/commonTools/fileParser.py`

 * *Files identical despite different names*

### Comparing `BFEE2-2.4.0/BFEE2/commonTools/ploter.py` & `BFEE2-2.4.1/BFEE2/commonTools/ploter.py`

 * *Files identical despite different names*

### Comparing `BFEE2-2.4.0/BFEE2/doc/Doc.pdf` & `BFEE2-2.4.1/BFEE2/doc/Doc.pdf`

 * *Files identical despite different names*

### Comparing `BFEE2-2.4.0/BFEE2/gui.py` & `BFEE2-2.4.1/BFEE2/gui.py`

 * *Files identical despite different names*

### Comparing `BFEE2-2.4.0/BFEE2/inputGenerator.py` & `BFEE2-2.4.1/BFEE2/inputGenerator.py`

 * *Files identical despite different names*

### Comparing `BFEE2-2.4.0/BFEE2/postTreatment.py` & `BFEE2-2.4.1/BFEE2/postTreatment.py`

 * *Files identical despite different names*

### Comparing `BFEE2-2.4.0/BFEE2/templates_gromacs/000.colvars.template` & `BFEE2-2.4.1/BFEE2/templates_gromacs/000.colvars.template`

 * *Files identical despite different names*

### Comparing `BFEE2-2.4.0/BFEE2/templates_gromacs/000.generate_tpr_sh.template` & `BFEE2-2.4.1/BFEE2/templates_gromacs/000.generate_tpr_sh.template`

 * *Files identical despite different names*

### Comparing `BFEE2-2.4.0/BFEE2/templates_gromacs/000.mdp.template` & `BFEE2-2.4.1/BFEE2/templates_gromacs/000.mdp.template`

 * *Files identical despite different names*

### Comparing `BFEE2-2.4.0/BFEE2/templates_gromacs/001.colvars.template` & `BFEE2-2.4.1/BFEE2/templates_gromacs/001.colvars.template`

 * *Files identical despite different names*

### Comparing `BFEE2-2.4.0/BFEE2/templates_gromacs/001.generate_tpr_sh.template` & `BFEE2-2.4.1/BFEE2/templates_gromacs/001.generate_tpr_sh.template`

 * *Files identical despite different names*

### Comparing `BFEE2-2.4.0/BFEE2/templates_gromacs/001.mdp.template` & `BFEE2-2.4.1/BFEE2/templates_gromacs/001.mdp.template`

 * *Files identical despite different names*

### Comparing `BFEE2-2.4.0/BFEE2/templates_gromacs/002.colvars.template` & `BFEE2-2.4.1/BFEE2/templates_gromacs/002.colvars.template`

 * *Files identical despite different names*

### Comparing `BFEE2-2.4.0/BFEE2/templates_gromacs/002.generate_tpr_sh.template` & `BFEE2-2.4.1/BFEE2/templates_gromacs/002.generate_tpr_sh.template`

 * *Files identical despite different names*

### Comparing `BFEE2-2.4.0/BFEE2/templates_gromacs/002.mdp.template` & `BFEE2-2.4.1/BFEE2/templates_gromacs/002.mdp.template`

 * *Files identical despite different names*

### Comparing `BFEE2-2.4.0/BFEE2/templates_gromacs/003.colvars.template` & `BFEE2-2.4.1/BFEE2/templates_gromacs/003.colvars.template`

 * *Files identical despite different names*

### Comparing `BFEE2-2.4.0/BFEE2/templates_gromacs/003.generate_tpr_sh.template` & `BFEE2-2.4.1/BFEE2/templates_gromacs/003.generate_tpr_sh.template`

 * *Files identical despite different names*

### Comparing `BFEE2-2.4.0/BFEE2/templates_gromacs/003.mdp.template` & `BFEE2-2.4.1/BFEE2/templates_gromacs/003.mdp.template`

 * *Files identical despite different names*

### Comparing `BFEE2-2.4.0/BFEE2/templates_gromacs/004.colvars.template` & `BFEE2-2.4.1/BFEE2/templates_gromacs/004.colvars.template`

 * *Files identical despite different names*

### Comparing `BFEE2-2.4.0/BFEE2/templates_gromacs/004.generate_tpr_sh.template` & `BFEE2-2.4.1/BFEE2/templates_gromacs/004.generate_tpr_sh.template`

 * *Files identical despite different names*

### Comparing `BFEE2-2.4.0/BFEE2/templates_gromacs/004.mdp.template` & `BFEE2-2.4.1/BFEE2/templates_gromacs/004.mdp.template`

 * *Files identical despite different names*

### Comparing `BFEE2-2.4.0/BFEE2/templates_gromacs/005.colvars.template` & `BFEE2-2.4.1/BFEE2/templates_gromacs/005.colvars.template`

 * *Files identical despite different names*

### Comparing `BFEE2-2.4.0/BFEE2/templates_gromacs/005.generate_tpr_sh.template` & `BFEE2-2.4.1/BFEE2/templates_gromacs/005.generate_tpr_sh.template`

 * *Files identical despite different names*

### Comparing `BFEE2-2.4.0/BFEE2/templates_gromacs/005.mdp.template` & `BFEE2-2.4.1/BFEE2/templates_gromacs/005.mdp.template`

 * *Files identical despite different names*

### Comparing `BFEE2-2.4.0/BFEE2/templates_gromacs/006.colvars.template` & `BFEE2-2.4.1/BFEE2/templates_gromacs/006.colvars.template`

 * *Files identical despite different names*

### Comparing `BFEE2-2.4.0/BFEE2/templates_gromacs/006.generate_tpr_sh.template` & `BFEE2-2.4.1/BFEE2/templates_gromacs/006.generate_tpr_sh.template`

 * *Files identical despite different names*

### Comparing `BFEE2-2.4.0/BFEE2/templates_gromacs/006.mdp.template` & `BFEE2-2.4.1/BFEE2/templates_gromacs/006.mdp.template`

 * *Files identical despite different names*

### Comparing `BFEE2-2.4.0/BFEE2/templates_gromacs/007.colvars.template` & `BFEE2-2.4.1/BFEE2/templates_gromacs/007.colvars.template`

 * *Files identical despite different names*

### Comparing `BFEE2-2.4.0/BFEE2/templates_gromacs/007.generate_tpr_sh.template` & `BFEE2-2.4.1/BFEE2/templates_gromacs/007.generate_tpr_sh.template`

 * *Files identical despite different names*

### Comparing `BFEE2-2.4.0/BFEE2/templates_gromacs/007.mdp.template` & `BFEE2-2.4.1/BFEE2/templates_gromacs/007.mdp.template`

 * *Files identical despite different names*

### Comparing `BFEE2-2.4.0/BFEE2/templates_gromacs/007_eq.colvars.template` & `BFEE2-2.4.1/BFEE2/templates_gromacs/007_eq.colvars.template`

 * *Files identical despite different names*

### Comparing `BFEE2-2.4.0/BFEE2/templates_gromacs/007_eq.generate_tpr_sh.template` & `BFEE2-2.4.1/BFEE2/templates_gromacs/007_eq.generate_tpr_sh.template`

 * *Files identical despite different names*

### Comparing `BFEE2-2.4.0/BFEE2/templates_gromacs/007_min.mdp.template` & `BFEE2-2.4.1/BFEE2/templates_gromacs/007_min.mdp.template`

 * *Files identical despite different names*

### Comparing `BFEE2-2.4.0/BFEE2/templates_gromacs/008.colvars.template` & `BFEE2-2.4.1/BFEE2/templates_gromacs/008.colvars.template`

 * *Files identical despite different names*

### Comparing `BFEE2-2.4.0/BFEE2/templates_gromacs/008.generate_tpr_sh.template` & `BFEE2-2.4.1/BFEE2/templates_gromacs/008.generate_tpr_sh.template`

 * *Files identical despite different names*

### Comparing `BFEE2-2.4.0/BFEE2/templates_gromacs/008.mdp.template` & `BFEE2-2.4.1/BFEE2/templates_gromacs/008.mdp.template`

 * *Files identical despite different names*

### Comparing `BFEE2-2.4.0/BFEE2/templates_gromacs/008_eq.generate_tpr_sh.template` & `BFEE2-2.4.1/BFEE2/templates_gromacs/008_eq.generate_tpr_sh.template`

 * *Files identical despite different names*

### Comparing `BFEE2-2.4.0/BFEE2/templates_gromacs/BFEEGromacs.py` & `BFEE2-2.4.1/BFEE2/templates_gromacs/BFEEGromacs.py`

 * *Files identical despite different names*

### Comparing `BFEE2-2.4.0/BFEE2/templates_namd/configTemplate.py` & `BFEE2-2.4.1/BFEE2/templates_namd/configTemplate.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # generate NAMD/Gromacs/Colvars config files
 
+import numpy as np
+
 class configTemplate:
     ''' generate NAMD/Gromacs/Colvars config files
         In the Colvars config file, ndx and xyz files are used to indicate the group of atoms
         The non-hydrogen atoms of protein are labeled as 'protein' in complex.ndx
         The non-hydrogen atoms of ligand are labeled as 'ligand' in complex.ndx
         The non-hydrogen atoms of user-defined reference are labeled as 'reference' in complex.ndx '''
 
@@ -110,15 +112,15 @@
             return ''
         
         # OPLS mixing rule
         if OPLSMixingRule:
             configString += f'\
 vdwGeometricSigma    yes               \n'
 
-        if NAMDRestartCoor == '' and NAMDRestartVel == '' and NAMDRestartXsc == '' and PBCCondition != '':
+        if NAMDRestartCoor == '' and NAMDRestartVel == '' and NAMDRestartXsc == '' and isinstance(PBCCondition, np.ndarray):
             # set temperature
             configString += f'\
 temperature    {temperature}                      \n\
 cellBasisVector1    {PBCCondition[0][0]} 0 0         \n\
 cellBasisVector2    0 {PBCCondition[0][1]} 0         \n\
 cellBasisVector3    0 0 {PBCCondition[0][2]}         \n\
 cellOrigin    {PBCCondition[1][0]} {PBCCondition[1][1]} {PBCCondition[1][2]}  \n'
```

### Comparing `BFEE2-2.4.0/BFEE2/templates_namd/fep.tcl` & `BFEE2-2.4.1/BFEE2/templates_namd/fep.tcl`

 * *Files identical despite different names*

### Comparing `BFEE2-2.4.0/BFEE2/templates_namd/scriptTemplate.py` & `BFEE2-2.4.1/BFEE2/templates_namd/scriptTemplate.py`

 * *Files identical despite different names*

### Comparing `BFEE2-2.4.0/BFEE2/templates_namd/updateCenters.py` & `BFEE2-2.4.1/BFEE2/templates_namd/updateCenters.py`

 * *Files identical despite different names*

### Comparing `BFEE2-2.4.0/BFEE2/templates_readme/Readme_Gromacs_Geometrical.txt` & `BFEE2-2.4.1/BFEE2/templates_readme/Readme_Gromacs_Geometrical.txt`

 * *Files identical despite different names*

### Comparing `BFEE2-2.4.0/BFEE2/templates_readme/Readme_NAMD_Alchemical.txt` & `BFEE2-2.4.1/BFEE2/templates_readme/Readme_NAMD_Alchemical.txt`

 * *Files identical despite different names*

### Comparing `BFEE2-2.4.0/BFEE2/templates_readme/Readme_NAMD_Geometrical.txt` & `BFEE2-2.4.1/BFEE2/templates_readme/Readme_NAMD_Geometrical.txt`

 * *Files identical despite different names*

### Comparing `BFEE2-2.4.0/BFEE2/third_party/py_bar.py` & `BFEE2-2.4.1/BFEE2/third_party/py_bar.py`

 * *Files identical despite different names*

### Comparing `BFEE2-2.4.0/BFEE2.egg-info/PKG-INFO` & `BFEE2-2.4.1/BFEE2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BFEE2
-Version: 2.4.0
+Version: 2.4.1
 Summary: Binding Free Energy Estimator 2
 Home-page: https://github.com/fhh2626/BFEE2
 Author: Haohao Fu, Haochuan Chen, Wensheng Cai and Chris Chipot
 Author-email: wscai@nankai.edu.cn
 Maintainer: Haohao Fu
 Maintainer-email: fhh2626@mail.nankai.edu.cn
 License: GPLv3
```

### Comparing `BFEE2-2.4.0/BFEE2.egg-info/SOURCES.txt` & `BFEE2-2.4.1/BFEE2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `BFEE2-2.4.0/LICENSE` & `BFEE2-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `BFEE2-2.4.0/PKG-INFO` & `BFEE2-2.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BFEE2
-Version: 2.4.0
+Version: 2.4.1
 Summary: Binding Free Energy Estimator 2
 Home-page: https://github.com/fhh2626/BFEE2
 Author: Haohao Fu, Haochuan Chen, Wensheng Cai and Chris Chipot
 Author-email: wscai@nankai.edu.cn
 Maintainer: Haohao Fu
 Maintainer-email: fhh2626@mail.nankai.edu.cn
 License: GPLv3
```

### Comparing `BFEE2-2.4.0/README.md` & `BFEE2-2.4.1/README.md`

 * *Files identical despite different names*

### Comparing `BFEE2-2.4.0/setup.cfg` & `BFEE2-2.4.1/setup.cfg`

 * *Files identical despite different names*

