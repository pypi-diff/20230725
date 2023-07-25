# Comparing `tmp/modflow-setup-0.2.0.tar.gz` & `tmp/modflow-setup-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modflow-setup-0.2.0.tar", last modified: Mon Feb  6 20:52:13 2023, max compression
+gzip compressed data, was "modflow-setup-0.3.0.tar", last modified: Tue Jul 25 15:13:04 2023, max compression
```

## Comparing `modflow-setup-0.2.0.tar` & `modflow-setup-0.3.0.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 20:52:13.777305 modflow-setup-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/AUTHORS.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     1650 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-02-06 20:52:13.777305 modflow-setup-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 20:52:13.757305 modflow-setup-0.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 20:52:13.761305 modflow-setup-0.2.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 20:52:13.765305 modflow-setup-0.2.0/docs/source/api/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/docs/source/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/docs/source/api/mfsetup.discretization.rst
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/docs/source/api/mfsetup.fileio.rst
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/docs/source/api/mfsetup.grid.rst
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/docs/source/api/mfsetup.interpolate.rst
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/docs/source/api/mfsetup.mf6model.rst
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/docs/source/api/mfsetup.mfmodel.rst
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/docs/source/api/mfsetup.mfnwtmodel.rst
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/docs/source/api/mfsetup.tdis.rst
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/docs/source/api/mfsetup.tmr.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 20:52:13.765305 modflow-setup-0.2.0/docs/source/concepts/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/docs/source/concepts/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/docs/source/concepts/perimeter-bcs.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7699 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/docs/source/config-file-defaults.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/docs/source/config-file-gallery.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9083 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/docs/source/config-file.rst
--rw-r--r--   0 runner    (1001) docker     (123)    16081 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/docs/source/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/docs/source/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 20:52:13.765305 modflow-setup-0.2.0/docs/source/input/
--rw-r--r--   0 runner    (1001) docker     (123)    19963 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/docs/source/input/basic-stress.rst
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/docs/source/input/dis.rst
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/docs/source/input/ic.rst
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/docs/source/input/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/docs/source/input/lak.rst
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/docs/source/input/obs.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/docs/source/input/oc.rst
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/docs/source/input/props.rst
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/docs/source/input/sfr.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13711 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/docs/source/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/docs/source/philosophy.rst
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/docs/source/pleasant-example.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/docs/source/references.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/docs/source/release-history.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/docs/source/structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/docs/source/troubleshooting.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 20:52:13.781305 modflow-setup-0.2.0/mfsetup/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/mfsetup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-02-06 20:52:13.781305 modflow-setup-0.2.0/mfsetup/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    19934 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/mfsetup/bcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/mfsetup/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/mfsetup/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    28607 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/mfsetup/discretization.py
--rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/mfsetup/equality.py
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/mfsetup/evaporation.py
--rw-r--r--   0 runner    (1001) docker     (123)    49324 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/mfsetup/fileio.py
--rw-r--r--   0 runner    (1001) docker     (123)    42623 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/mfsetup/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/mfsetup/ic.py
--rw-r--r--   0 runner    (1001) docker     (123)    14982 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/mfsetup/interpolate.py
--rw-r--r--   0 runner    (1001) docker     (123)    32147 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/mfsetup/lakes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/mfsetup/mf5to6.py
--rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/mfsetup/mf6_defaults.yml
--rw-r--r--   0 runner    (1001) docker     (123)    40471 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/mfsetup/mf6model.py
--rw-r--r--   0 runner    (1001) docker     (123)    83401 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/mfsetup/mfmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/mfsetup/mfnwt_defaults.yml
--rw-r--r--   0 runner    (1001) docker     (123)    36572 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/mfsetup/mfnwtmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)    17151 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/mfsetup/model_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/mfsetup/mover.py
--rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/mfsetup/obs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5978 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/mfsetup/oc.py
--rw-r--r--   0 runner    (1001) docker     (123)    67974 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/mfsetup/sourcedata.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/mfsetup/sourcemodel.py
--rw-r--r--   0 runner    (1001) docker     (123)    32132 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/mfsetup/tdis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/mfsetup/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 20:52:13.777305 modflow-setup-0.2.0/mfsetup/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/mfsetup/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11037 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/mfsetup/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 20:52:13.777305 modflow-setup-0.2.0/mfsetup/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)    17384 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/mfsetup/tests/data/shellmound.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/mfsetup/tests/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/mfsetup/tests/test_bcs.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/mfsetup/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    14148 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/mfsetup/tests/test_discretization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/mfsetup/tests/test_equality.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/mfsetup/tests/test_evaporation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/mfsetup/tests/test_fileio.py
--rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/mfsetup/tests/test_get_data_from_parent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/mfsetup/tests/test_get_model_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    12709 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/mfsetup/tests/test_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/mfsetup/tests/test_interpolation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7719 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/mfsetup/tests/test_lakes.py
--rw-r--r--   0 runner    (1001) docker     (123)    10887 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/mfsetup/tests/test_lgr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/mfsetup/tests/test_mf5to6.py
--rw-r--r--   0 runner    (1001) docker     (123)    40641 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/mfsetup/tests/test_mf6_shellmound.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/mfsetup/tests/test_mf6_shellmound_mixed_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/mfsetup/tests/test_mf6_shellmound_rot_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    15587 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/mfsetup/tests/test_mf6_tmr_shellmound.py
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/mfsetup/tests/test_notebooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/mfsetup/tests/test_obs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/mfsetup/tests/test_oc.py
--rw-r--r--   0 runner    (1001) docker     (123)    27440 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/mfsetup/tests/test_pfl_mfnwt_inset.py
--rw-r--r--   0 runner    (1001) docker     (123)    32058 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/mfsetup/tests/test_pleasant_mf6_inset.py
--rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/mfsetup/tests/test_pleasant_mfnwt_inset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/mfsetup/tests/test_solver_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    16542 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/mfsetup/tests/test_sourcedata.py
--rw-r--r--   0 runner    (1001) docker     (123)    17797 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/mfsetup/tests/test_tdis.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/mfsetup/tests/test_testing.py
--rw-r--r--   0 runner    (1001) docker     (123)    42687 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/mfsetup/tests/test_tmr.py
--rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/mfsetup/tests/test_units.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/mfsetup/tests/test_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/mfsetup/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7480 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/mfsetup/tests/test_wateruse.py
--rw-r--r--   0 runner    (1001) docker     (123)     8847 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/mfsetup/tests/test_wells.py
--rw-r--r--   0 runner    (1001) docker     (123)    49159 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/mfsetup/tmr.py
--rw-r--r--   0 runner    (1001) docker     (123)     9793 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/mfsetup/units.py
--rw-r--r--   0 runner    (1001) docker     (123)     4285 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/mfsetup/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    18539 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/mfsetup/wateruse.py
--rw-r--r--   0 runner    (1001) docker     (123)    31340 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/mfsetup/wells.py
--rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/mfsetup/zbud.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 20:52:13.777305 modflow-setup-0.2.0/modflow_setup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-02-06 20:52:13.000000 modflow-setup-0.2.0/modflow_setup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-02-06 20:52:13.000000 modflow-setup-0.2.0/modflow_setup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-06 20:52:13.000000 modflow-setup-0.2.0/modflow_setup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-02-06 20:52:13.000000 modflow-setup-0.2.0/modflow_setup.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-06 20:52:13.000000 modflow-setup-0.2.0/modflow_setup.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-02-06 20:52:13.777305 modflow-setup-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    68613 2023-02-06 20:51:58.000000 modflow-setup-0.2.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:13:04.239083 modflow-setup-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-25 15:12:43.000000 modflow-setup-0.3.0/AUTHORS.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1650 2023-07-25 15:12:43.000000 modflow-setup-0.3.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-25 15:12:43.000000 modflow-setup-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-07-25 15:13:04.239083 modflow-setup-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-07-25 15:12:43.000000 modflow-setup-0.3.0/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:13:04.231083 modflow-setup-0.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-25 15:12:43.000000 modflow-setup-0.3.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-07-25 15:12:43.000000 modflow-setup-0.3.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:13:04.231083 modflow-setup-0.3.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:13:04.231083 modflow-setup-0.3.0/docs/source/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-25 15:12:43.000000 modflow-setup-0.3.0/docs/source/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-25 15:12:43.000000 modflow-setup-0.3.0/docs/source/api/mfsetup.discretization.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-25 15:12:43.000000 modflow-setup-0.3.0/docs/source/api/mfsetup.fileio.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-25 15:12:43.000000 modflow-setup-0.3.0/docs/source/api/mfsetup.grid.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-25 15:12:43.000000 modflow-setup-0.3.0/docs/source/api/mfsetup.interpolate.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-25 15:12:43.000000 modflow-setup-0.3.0/docs/source/api/mfsetup.mf6model.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-25 15:12:43.000000 modflow-setup-0.3.0/docs/source/api/mfsetup.mfmodel.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-25 15:12:43.000000 modflow-setup-0.3.0/docs/source/api/mfsetup.mfnwtmodel.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-25 15:12:43.000000 modflow-setup-0.3.0/docs/source/api/mfsetup.tdis.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-25 15:12:43.000000 modflow-setup-0.3.0/docs/source/api/mfsetup.tmr.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:13:04.231083 modflow-setup-0.3.0/docs/source/concepts/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-25 15:12:43.000000 modflow-setup-0.3.0/docs/source/concepts/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-07-25 15:12:43.000000 modflow-setup-0.3.0/docs/source/concepts/perimeter-bcs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7699 2023-07-25 15:12:43.000000 modflow-setup-0.3.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-25 15:12:43.000000 modflow-setup-0.3.0/docs/source/config-file-defaults.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-07-25 15:12:43.000000 modflow-setup-0.3.0/docs/source/config-file-gallery.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9083 2023-07-25 15:12:43.000000 modflow-setup-0.3.0/docs/source/config-file.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    16081 2023-07-25 15:12:43.000000 modflow-setup-0.3.0/docs/source/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-25 15:12:43.000000 modflow-setup-0.3.0/docs/source/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-25 15:12:43.000000 modflow-setup-0.3.0/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:13:04.235083 modflow-setup-0.3.0/docs/source/input/
+-rw-r--r--   0 runner    (1001) docker     (123)    23389 2023-07-25 15:12:43.000000 modflow-setup-0.3.0/docs/source/input/basic-stress.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-25 15:12:43.000000 modflow-setup-0.3.0/docs/source/input/dis.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-25 15:12:43.000000 modflow-setup-0.3.0/docs/source/input/ic.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-25 15:12:43.000000 modflow-setup-0.3.0/docs/source/input/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-25 15:12:43.000000 modflow-setup-0.3.0/docs/source/input/lak.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-25 15:12:43.000000 modflow-setup-0.3.0/docs/source/input/obs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-07-25 15:12:43.000000 modflow-setup-0.3.0/docs/source/input/oc.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-25 15:12:43.000000 modflow-setup-0.3.0/docs/source/input/props.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-25 15:12:43.000000 modflow-setup-0.3.0/docs/source/input/sfr.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    19142 2023-07-25 15:12:43.000000 modflow-setup-0.3.0/docs/source/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-07-25 15:12:43.000000 modflow-setup-0.3.0/docs/source/philosophy.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-25 15:12:43.000000 modflow-setup-0.3.0/docs/source/pleasant-example.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-07-25 15:12:43.000000 modflow-setup-0.3.0/docs/source/references.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-07-25 15:12:43.000000 modflow-setup-0.3.0/docs/source/release-history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-07-25 15:12:43.000000 modflow-setup-0.3.0/docs/source/structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-07-25 15:12:43.000000 modflow-setup-0.3.0/docs/source/troubleshooting.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:13:04.243083 modflow-setup-0.3.0/mfsetup/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-25 15:12:43.000000 modflow-setup-0.3.0/mfsetup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-25 15:13:04.243083 modflow-setup-0.3.0/mfsetup/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23731 2023-07-25 15:12:43.000000 modflow-setup-0.3.0/mfsetup/bcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-07-25 15:12:43.000000 modflow-setup-0.3.0/mfsetup/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-25 15:12:43.000000 modflow-setup-0.3.0/mfsetup/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29102 2023-07-25 15:12:43.000000 modflow-setup-0.3.0/mfsetup/discretization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-07-25 15:12:43.000000 modflow-setup-0.3.0/mfsetup/equality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-07-25 15:12:43.000000 modflow-setup-0.3.0/mfsetup/evaporation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49338 2023-07-25 15:12:43.000000 modflow-setup-0.3.0/mfsetup/fileio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43130 2023-07-25 15:12:43.000000 modflow-setup-0.3.0/mfsetup/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-07-25 15:12:43.000000 modflow-setup-0.3.0/mfsetup/ic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14982 2023-07-25 15:12:43.000000 modflow-setup-0.3.0/mfsetup/interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32168 2023-07-25 15:12:43.000000 modflow-setup-0.3.0/mfsetup/lakes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-07-25 15:12:43.000000 modflow-setup-0.3.0/mfsetup/mf5to6.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7139 2023-07-25 15:12:43.000000 modflow-setup-0.3.0/mfsetup/mf6_defaults.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    44255 2023-07-25 15:12:43.000000 modflow-setup-0.3.0/mfsetup/mf6model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81026 2023-07-25 15:12:43.000000 modflow-setup-0.3.0/mfsetup/mfmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5896 2023-07-25 15:12:43.000000 modflow-setup-0.3.0/mfsetup/mfnwt_defaults.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    39667 2023-07-25 15:12:43.000000 modflow-setup-0.3.0/mfsetup/mfnwtmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17181 2023-07-25 15:12:43.000000 modflow-setup-0.3.0/mfsetup/model_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-07-25 15:12:43.000000 modflow-setup-0.3.0/mfsetup/mover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8836 2023-07-25 15:12:43.000000 modflow-setup-0.3.0/mfsetup/obs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6022 2023-07-25 15:12:43.000000 modflow-setup-0.3.0/mfsetup/oc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70768 2023-07-25 15:12:43.000000 modflow-setup-0.3.0/mfsetup/sourcedata.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 15:12:43.000000 modflow-setup-0.3.0/mfsetup/sourcemodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38489 2023-07-25 15:12:43.000000 modflow-setup-0.3.0/mfsetup/tdis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-07-25 15:12:43.000000 modflow-setup-0.3.0/mfsetup/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:13:04.239083 modflow-setup-0.3.0/mfsetup/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 15:12:43.000000 modflow-setup-0.3.0/mfsetup/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11037 2023-07-25 15:12:43.000000 modflow-setup-0.3.0/mfsetup/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:13:04.239083 modflow-setup-0.3.0/mfsetup/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    18617 2023-07-25 15:12:44.000000 modflow-setup-0.3.0/mfsetup/tests/data/shellmound.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-07-25 15:12:44.000000 modflow-setup-0.3.0/mfsetup/tests/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-07-25 15:12:44.000000 modflow-setup-0.3.0/mfsetup/tests/test_bcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-25 15:12:44.000000 modflow-setup-0.3.0/mfsetup/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14148 2023-07-25 15:12:44.000000 modflow-setup-0.3.0/mfsetup/tests/test_discretization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-25 15:12:44.000000 modflow-setup-0.3.0/mfsetup/tests/test_equality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-07-25 15:12:44.000000 modflow-setup-0.3.0/mfsetup/tests/test_evaporation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-07-25 15:12:44.000000 modflow-setup-0.3.0/mfsetup/tests/test_fileio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7782 2023-07-25 15:12:44.000000 modflow-setup-0.3.0/mfsetup/tests/test_get_data_from_parent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-07-25 15:12:44.000000 modflow-setup-0.3.0/mfsetup/tests/test_get_model_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12709 2023-07-25 15:12:44.000000 modflow-setup-0.3.0/mfsetup/tests/test_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-07-25 15:12:44.000000 modflow-setup-0.3.0/mfsetup/tests/test_interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7719 2023-07-25 15:12:44.000000 modflow-setup-0.3.0/mfsetup/tests/test_lakes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10887 2023-07-25 15:12:44.000000 modflow-setup-0.3.0/mfsetup/tests/test_lgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-07-25 15:12:44.000000 modflow-setup-0.3.0/mfsetup/tests/test_mf5to6.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42467 2023-07-25 15:12:44.000000 modflow-setup-0.3.0/mfsetup/tests/test_mf6_shellmound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-25 15:12:44.000000 modflow-setup-0.3.0/mfsetup/tests/test_mf6_shellmound_mixed_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-07-25 15:12:44.000000 modflow-setup-0.3.0/mfsetup/tests/test_mf6_shellmound_rot_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15623 2023-07-25 15:12:44.000000 modflow-setup-0.3.0/mfsetup/tests/test_mf6_tmr_shellmound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-07-25 15:12:44.000000 modflow-setup-0.3.0/mfsetup/tests/test_notebooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-25 15:12:44.000000 modflow-setup-0.3.0/mfsetup/tests/test_obs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-07-25 15:12:44.000000 modflow-setup-0.3.0/mfsetup/tests/test_oc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27454 2023-07-25 15:12:44.000000 modflow-setup-0.3.0/mfsetup/tests/test_pfl_mfnwt_inset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32077 2023-07-25 15:12:44.000000 modflow-setup-0.3.0/mfsetup/tests/test_pleasant_mf6_inset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-07-25 15:12:44.000000 modflow-setup-0.3.0/mfsetup/tests/test_pleasant_mfnwt_inset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-25 15:12:44.000000 modflow-setup-0.3.0/mfsetup/tests/test_solver_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21744 2023-07-25 15:12:44.000000 modflow-setup-0.3.0/mfsetup/tests/test_sourcedata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18120 2023-07-25 15:12:44.000000 modflow-setup-0.3.0/mfsetup/tests/test_tdis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-25 15:12:44.000000 modflow-setup-0.3.0/mfsetup/tests/test_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42687 2023-07-25 15:12:44.000000 modflow-setup-0.3.0/mfsetup/tests/test_tmr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-07-25 15:12:44.000000 modflow-setup-0.3.0/mfsetup/tests/test_units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-25 15:12:44.000000 modflow-setup-0.3.0/mfsetup/tests/test_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-25 15:12:44.000000 modflow-setup-0.3.0/mfsetup/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7507 2023-07-25 15:12:44.000000 modflow-setup-0.3.0/mfsetup/tests/test_wateruse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8847 2023-07-25 15:12:44.000000 modflow-setup-0.3.0/mfsetup/tests/test_wells.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49159 2023-07-25 15:12:44.000000 modflow-setup-0.3.0/mfsetup/tmr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9793 2023-07-25 15:12:44.000000 modflow-setup-0.3.0/mfsetup/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4285 2023-07-25 15:12:44.000000 modflow-setup-0.3.0/mfsetup/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18573 2023-07-25 15:12:44.000000 modflow-setup-0.3.0/mfsetup/wateruse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31411 2023-07-25 15:12:44.000000 modflow-setup-0.3.0/mfsetup/wells.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-07-25 15:12:44.000000 modflow-setup-0.3.0/mfsetup/zbud.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:13:04.239083 modflow-setup-0.3.0/modflow_setup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-07-25 15:13:04.000000 modflow-setup-0.3.0/modflow_setup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-07-25 15:13:04.000000 modflow-setup-0.3.0/modflow_setup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 15:13:04.000000 modflow-setup-0.3.0/modflow_setup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-25 15:13:04.000000 modflow-setup-0.3.0/modflow_setup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-25 15:13:04.000000 modflow-setup-0.3.0/modflow_setup.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-25 15:12:44.000000 modflow-setup-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-25 15:12:44.000000 modflow-setup-0.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-25 15:13:04.243083 modflow-setup-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-07-25 15:12:44.000000 modflow-setup-0.3.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68613 2023-07-25 15:12:44.000000 modflow-setup-0.3.0/versioneer.py
```

### Comparing `modflow-setup-0.2.0/LICENSE.md` & `modflow-setup-0.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `modflow-setup-0.2.0/PKG-INFO` & `modflow-setup-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: modflow-setup
-Version: 0.2.0
-Summary: Package to facilitate setup of a MODFLOW-6 groundwater flow model with the SFR package.
+Version: 0.3.0
+Summary: Robust automation of MODFLOW model construction.
 Home-page: https://github.com/aleaf/modflow-setup
 Author: USGS MAP Project
 Author-email: aleaf@usgs.gov
 License: BSD (3-clause)
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
@@ -16,19 +16,19 @@
 
 
 Modflow-setup
 -----------------------------------------------
 Modflow-setup is a Python package for automating the setup of MODFLOW groundwater models from grid-independent source data including shapefiles, rasters, and other MODFLOW models that are geo-located. Input data and model construction options are summarized in a single configuration file. Source data are read from their native formats and mapped to a regular finite difference grid specified in the configuration file. An external array-based [Flopy](https://github.com/modflowpy/flopy) model instance with the desired packages is created from the sampled source data and configuration settings. MODFLOW input can then be written from the flopy model instance.
 
 
-### Version 0.1
-![Tests](https://github.com/usgs/modflow-setup/workflows/Tests/badge.svg)
-[![codecov](https://codecov.io/gh/usgs/modflow-setup/branch/develop/graph/badge.svg?token=aWN47DYeIv)](https://codecov.io/gh/usgs/modflow-setup)
+### Version 0.2
+![Tests](https://github.com/aleaf/modflow-setup/workflows/Tests/badge.svg)
+[![codecov](https://codecov.io/gh/aleaf/modflow-setup/branch/develop/graph/badge.svg?token=aWN47DYeIv)](https://codecov.io/gh/aleaf/modflow-setup)
 [![PyPI version](https://badge.fury.io/py/modflow-setup.svg)](https://badge.fury.io/py/modflow-setup)
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/usgs/modflow-setup/develop?urlpath=lab/tree/examples)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/doi-usgs/modflow-setup/develop?urlpath=lab/tree/examples)
 [![Project Status: Active – The project has reached a stable, usable state and is being actively developed.](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active)
 
 
 
 
 
 Getting Started
```

### Comparing `modflow-setup-0.2.0/Readme.md` & `modflow-setup-0.3.0/Readme.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 
 Modflow-setup
 -----------------------------------------------
 Modflow-setup is a Python package for automating the setup of MODFLOW groundwater models from grid-independent source data including shapefiles, rasters, and other MODFLOW models that are geo-located. Input data and model construction options are summarized in a single configuration file. Source data are read from their native formats and mapped to a regular finite difference grid specified in the configuration file. An external array-based [Flopy](https://github.com/modflowpy/flopy) model instance with the desired packages is created from the sampled source data and configuration settings. MODFLOW input can then be written from the flopy model instance.
 
 
-### Version 0.1
-![Tests](https://github.com/usgs/modflow-setup/workflows/Tests/badge.svg)
-[![codecov](https://codecov.io/gh/usgs/modflow-setup/branch/develop/graph/badge.svg?token=aWN47DYeIv)](https://codecov.io/gh/usgs/modflow-setup)
+### Version 0.2
+![Tests](https://github.com/aleaf/modflow-setup/workflows/Tests/badge.svg)
+[![codecov](https://codecov.io/gh/aleaf/modflow-setup/branch/develop/graph/badge.svg?token=aWN47DYeIv)](https://codecov.io/gh/aleaf/modflow-setup)
 [![PyPI version](https://badge.fury.io/py/modflow-setup.svg)](https://badge.fury.io/py/modflow-setup)
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/usgs/modflow-setup/develop?urlpath=lab/tree/examples)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/doi-usgs/modflow-setup/develop?urlpath=lab/tree/examples)
 [![Project Status: Active – The project has reached a stable, usable state and is being actively developed.](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active)
 
 
 
 
 
 Getting Started
```

### Comparing `modflow-setup-0.2.0/docs/Makefile` & `modflow-setup-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `modflow-setup-0.2.0/docs/make.bat` & `modflow-setup-0.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `modflow-setup-0.2.0/docs/source/concepts/perimeter-bcs.rst` & `modflow-setup-0.3.0/docs/source/concepts/perimeter-bcs.rst`

 * *Files identical despite different names*

### Comparing `modflow-setup-0.2.0/docs/source/conf.py` & `modflow-setup-0.3.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `modflow-setup-0.2.0/docs/source/config-file-defaults.rst` & `modflow-setup-0.3.0/docs/source/config-file-defaults.rst`

 * *Files identical despite different names*

### Comparing `modflow-setup-0.2.0/docs/source/config-file-gallery.rst` & `modflow-setup-0.3.0/docs/source/config-file-gallery.rst`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 Shellmound TMR inset test case
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 * 13 layer MODFLOW-6 Telescopic Mesh Refinement (TMR) model with a MODFLOW-6 parent model
 * 1:1 layer mapping between parent and TMR inset (default)
 * parent model grid defined with a SpatialReference subblock (which overrides information in MODFLOW Namefile)
 * DIS package top and bottom elevations copied from parent model
 * IC, NPF, STO, RCH, and WEL packages copied from parent model (default if not specified in config file)
-* `default OC configuration <#MODFLOW-6 configuration defaults>`_
+* :ref:`default OC configuration <MODFLOW-6 configuration defaults>`
 * variable time discretization
 * model grid aligned with the `National Hydrologic Grid`_
 * SFR network created from custom hydrography
 
 
 .. literalinclude:: ../../mfsetup/tests/data/shellmound_tmr_inset.yml
     :language: yaml
```

### Comparing `modflow-setup-0.2.0/docs/source/config-file.rst` & `modflow-setup-0.3.0/docs/source/config-file.rst`

 * *Files identical despite different names*

### Comparing `modflow-setup-0.2.0/docs/source/contributing.rst` & `modflow-setup-0.3.0/docs/source/contributing.rst`

 * *Files identical despite different names*

### Comparing `modflow-setup-0.2.0/docs/source/index.rst` & `modflow-setup-0.3.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `modflow-setup-0.2.0/docs/source/input/basic-stress.rst` & `modflow-setup-0.3.0/docs/source/input/basic-stress.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 =======================================================================================
 Specifying boundary conditions with the 'basic' MODFLOW stress packages
 =======================================================================================
 
-.. note::
-   This page is a work in progress and needs some more work.
-
 This page describes configuration file input for the basic MODFLOW stress packages, including
 the CHD, DRN, GHB, RCH, RIV and WEL packages. The EVT package is not currently supported by Modflow-setup. The supported packages can be broadly placed into two categories. Feature or list-based packages such as CHD, DRN, GHB, RIV and WEL often represent discrete phenomena such as surface water features, pumping wells, or even lines that denote a perimeter boundary. Input to  these packages in MODFLOW is tabular, consisting of a table for each stress period, with rows specifying stresses at individual grid cells representing the boundary features. In contrast, continuous or grid-based packages represent a stress field that applies to a large area, such as areal recharge. In past versions of MODFLOW, input to these packages was array-based, with values specified for all model cells, at each stress period. In MODFLOW 6, input to these packages can be array or list-based. The Recharge (RCH) Package is currently the only grid-based stress package supported by Modflow-setup. In keeping with the current structured grid-based paradigm of Modflow-setup, Modflow 6 recharge input is generated for the array-based recharge package (Langevin and others, 2017).
 
 
 
 List-based basic stress packages
 -------------------------------------
@@ -23,42 +20,72 @@
         * A ``shapefile:`` block for specifying shapefile input that maps the boundary condition features in space. Items in the shapefile block include
 
             * ``filename:`` path to the shapefile
             * ``boundname_col:`` column in shapefile with feature names to be applied as `boundnames` in Modflow 6 input
             * ``all_touched:`` argument to :func:`rasterio.features.rasterize` that specifies whether all intersected grid cells should be included, or just the grid cells with centers inside the feature.
             * One or more variable columns: Optionally the shapefile can also supply steady-state variable values by feature in attribute columns named for the variables (e.g. ``'head'``, ``'bhead'``, etc.)
 
-        * **(Not implemented yet)** A ``csvfile:`` block for specifying point feature locations or time-varying values for the variables. Items in the shapefile block include
+            Example:
+
+            .. literalinclude:: ../../../mfsetup/tests/data/shellmound.yml
+                :language: yaml
+                :start-at: shapefile:
+                :end-before: csvfile:
+
+        * A ``csvfile:`` block for specifying point feature locations or time-varying values for the variables. Items in the shapefile block include
 
             * ``filename:`` or `filenames:` path(s) to the csv file(s)
             * ``id_column``: unique identifier associated with each feature
             * ``datetime_column:`` date-time associated with each stress value
             * ``end_datetime_column:`` date-time associated with the end of stress value (optional; for rates that extend across more than one model stress period. If this is specified, ``datetime_column:`` is assumed to indicate the date-time associated with the start of each stress value.
             * ``x_col:`` feature x-coordinate (WEL package only; default ``'x'``)
             * ``y_col:`` feature y-coordinate (WEL package only; default ``'y'``)
             * ``length_units:`` length units associated with the stress value (optional; if omitted no conversion is performed)
             * ``time_units:`` time units associated with the stress value (WEL package only; optional; if omitted no conversion is performed)
             * ``volume_units:`` value-units associated with the stress value (e.g. `gallons`) in lieu of length-based volume units (e.g., `cubic feet`) (WEL package only; optional; if omitted volumes are assumed to be in model units of L\ :sup:`3` and no conversion is performed)
             * ``boundname_col:`` column in shapefile with feature names to be applied as `boundnames` in Modflow 6 input
+            * one or more columns for the package variables, specified in the format of ``<variable>_col``, where ``<variable>`` is an input variable for the package; for example ``head_col`` for the Constant Head Package, or ``cond_col`` for the Drain or GHB packages.
             * ``period_stats:`` a sub-block that is used to specify mapping of the input data to the model temporal discretization. Items within period stats are numbered by stress period, with the entry for each item specifying the temporal aggregation. Currently, two options are supported:
                 * aggregation of measurements falling within a stress period. For example, assigning the mean value of all input data points within the stress period. In this case, the aggregration method is simply specified as a string. While ``mean`` is typical, any of the standard numpy aggregators can be use (``min``, ``max``, etc.)
                 * aggregation of measurements from an arbitrary time window. For example, applying a long-term mean to a steady-state stress period, or transient period representing a different time window. In this case three items are specified-- the aggregation method, the start date, and end date (e.g. ``[mean, 2000-01-01, 2017-12-31]``)
 
+            Example:
+
+            .. literalinclude:: ../../../mfsetup/tests/data/shellmound.yml
+                :language: yaml
+                :start-at: csvfile:
+                :end-before: # Drain Package
+
+
+        * Additional sub-blocks or items for specifying values for each variable
+            * In general, these sub-blocks are named for the variable (e.g. ``bhead:``).
+            * Scalar values (items) can be specified in model units, and are applied globally to the variable.
+
                 Example:
 
                 .. literalinclude:: ../../../mfsetup/tests/data/shellmound.yml
                     :language: yaml
-                    :lines: 219-224
+                    :start-at: cond:
+                    :end-at: cond:
+
+            * Rasters can be used to specify steady-state values that vary in space; values supplied with a raster are mapped to the model grid using zonal statistics. If the raster contains projection information (GeoTIFFs are preferred in part because of this), reprojection to the model coorindate reference system (CRS) will be performed automatically as needed. Otherwise, the raster is assumed to be in the model projection. Units can optionally be specified and automatically converted; otherwise, the raster values are assumed to be in the model units. Items in the raster block include:
+
+                * ``filename:`` or `filenames:` path(s) to the raster
+                * ``length_units:`` (or ``elevation_units``; optional): length units of the raster values
+                * ``time_units:`` (optional): time units of the raster values (``cond`` variable only)
+                * ``stat:`` (optional): zonal statistic to use in sampling the raster (defaults are listed for each variable in the :ref:`Configuration defaults`)
 
+                Example:
+
+                .. literalinclude:: ../../../mfsetup/tests/data/shellmound.yml
+                    :language: yaml
+                    :start-at: stage:
+                    :end-before: mfsetup_options:
 
-        * additional sub-blocks or items for specifying values for each variable
-            * in general, these sub-blocks are named for the variable (e.g. ``bhead:``)
-            * scalar values (items) are applied globally to the variable
-            * rasters can be used to specify steady-state values that vary in space; values supplied with a raster are mapped to the model grid using zonal statistics. If the raster contains projection information (GeoTIFFs are preferred in part because of this), any reprojection to the model coorindate reference system (CRS) will be performed automatically as needed. Otherwise, the raster is assumed to be in the model projection.
-            * (Not implemented yet) NetCDF input for gridded values that vary in time and space. Due to the lack of standardization in NetCDF coordinate reference information, automatic reprojection is currently not supported for NetCDF files; the data are assumed to be in the model CRS.
+            * **Not implemented yet:** NetCDF input for gridded values that vary in time and space. Due to the lack of standardization in NetCDF coordinate reference information, automatic reprojection is currently not supported for NetCDF files; the data are assumed to be in the model CRS.
     * ``mfsetup_options:`` Configuration options for Modflow-setup. General options that apply to all basic stress packages include:
             * ``external_files:`` Whether to write the package input as external text arrays or tables (i.e., with ``open/close`` statements). By default ``True`` except in the case of list-based or tabular files for MODFLOW-NWT models, which are not supported. Adding support for this may require changes to Flopy, which handles external list-based files differently for MODFLOW-2005 style models.
             * ``external_filename_fmt:`` Python string format for external file names. By default, ``"<package or variable abbreviation>_{:03d}.dat"``. which results in filenames such as ``wel_000.dat``, ``wel_001.dat``, ``wel_002.dat``... for stress periods 0, 1, and 2, for example.
 
             Other Modflow-setup options specific to individual packages are described below.
 
 Constant Head (CHD) Package
@@ -77,21 +104,27 @@
     * raster to specify steady state elevations by cell (for supplied shapefile)
     * shapefile or csv to specify steady elevations by feature
     * csv to specify transient elevation by feature (needs to be referenced to features in shapefile)
 
     **Examples**
     (also see the :ref:`Configuration File Gallery`)
 
-    .. literalinclude:: ../../../mfsetup/tests/data/shellmound_tmr_inset.yml
+    Setting up a Constant Head package with perimeter fluxes from a parent model (Note: an additional ``source_data`` block can be added to represent other features inside of the model perimeter, as below):
+
+    .. literalinclude:: ../../../mfsetup/tests/data/pfl_nwt_test.yml
         :language: yaml
-        :lines: 120-123
+        :start-at: chd:
+
+    Setting up a Constant Head package from features specified in a shapefile,
+    and time-varing heads specified in a csvfile:
 
     .. literalinclude:: ../../../mfsetup/tests/data/shellmound.yml
         :language: yaml
-        :lines: 285-298
+        :start-after: # Constant Head Package
+        :end-before: # Drain Package
 
 
 Drain DRN Package
 ++++++++++++++++++
 Input consists of elevations and conductances that may vary in time or space.
 
     **Required input**
@@ -108,15 +141,16 @@
     * csv to specify transient elevation by feature (needs to be referenced to features in shapefile)
 
     **Examples**
     (also see the :ref:`Configuration File Gallery`)
 
     .. literalinclude:: ../../../mfsetup/tests/data/shellmound.yml
         :language: yaml
-        :lines: 299-313
+        :start-after: # Drain Package
+        :end-before: # General Head Boundary Package
 
 General Head Boundary (GHB) Package
 +++++++++++++++++++++++++++++++++++++
 Input consists of head elevations and conductances that may vary in time or space.
 
     **Required input**
 
@@ -132,15 +166,16 @@
     * csv to specify transient elevations or conductances by feature (needs to be referenced to features in shapefile)
 
     **Examples**
     (also see the :ref:`Configuration File Gallery`)
 
     .. literalinclude:: ../../../mfsetup/tests/data/shellmound.yml
         :language: yaml
-        :lines: 316-337
+        :start-after: # General Head Boundary Package
+        :end-before: # River Package
 
 River (RIV) package
 ++++++++++++++++++++
 Input consists of stages, river bottom elevations and conductances,
  that may vary in time or space.
 
     **Required input**
@@ -158,21 +193,23 @@
     * csv to specify transient heads, conductances and rbots by feature (needs to be referenced to features in shapefile)
 
     **Examples**
     (also see the :ref:`Configuration File Gallery`)
 
     .. literalinclude:: ../../../mfsetup/tests/data/shellmound.yml
         :language: yaml
-        :lines: 338-358
+        :start-after: # River Package
+        :end-before: # Well Package
 
     Example of setting up the RIV package using SFRmaker (via the ``sfr:`` block):
 
     .. literalinclude:: ../../../mfsetup/tests/data/shellmound_tmr_inset.yml
         :language: yaml
-        :lines: 99-118
+        :start-at: sfr:
+        :end-at: to_riv:
 
 
 Well (WEL) Package
 ++++++++++++++++++++
 Input consists of flux rates that may vary in time or space.
 
     **Required input**
@@ -202,15 +239,25 @@
         * input for column names and units is the same for the general ``csvfile:`` block described above
         * temporal discretization is specified using a ``period_stats:`` sub-block
         * spatial discretization for open intervals spanning multiple layers is specified using a ``vertical_flux_distribution:`` sub-block
         * Examples:
 
             .. literalinclude:: ../../../mfsetup/tests/data/shellmound.yml
                 :language: yaml
-                :lines: 359-388
+                :start-after: # Well Package
+                :end-before: # Output Control Package
+
+    * Perimeter boundary fluxes from a parent model solution:
+
+            .. literalinclude:: ../../../mfsetup/tests/data/shellmound_tmr_inset.yml
+                :language: yaml
+                :start-at: wel:
+
+
+        Similar to the Constant Head Package, a ``perimeter_boundary`` block can be mixed with the other input blocks described here to simulate pumping or injection inside of the model perimeter.
 
     * ``wdnr_dataset`` block
         .. note::
             This is a custom option from early versions of Modflow-setup, and is likely to be generalized into a combined shapefile (or CSV site information file) and CSV timeseries input option similar to the other basic stress packages.
 
         * site information is specified in a shapefile formatted like ``csls_sources_wu_pts.shp`` below
         * pumping rates are specified by month in a CSV file formatted like ``master_wu.csv`` below
@@ -260,15 +307,15 @@
 In the above example, ``0.01`` would be also be applied to all subsequent stress periods.
 
 Grid-independent input
 @@@@@@@@@@@@@@@@@@@@@@@@@@@
 Modflow-setup currently supports three methods for entering spatially-referenced recharge input not mapped to the model grid.
 
     * Recharge translated from a parent model RCH package
-        * this input option is very simple. A parent model with a recharge package is needed, and ``default_source_data: True`` must be specified in the ``parent:`` block. Then, fluxes from the parent model are simply mapped to the inset model grid, based on the parent model cell centers, and the stress period mappings specified in the ``parent:`` block. Recharge package options can still be specified in a ``rch:`` block.
+        * This input option is very simple. A parent model with a recharge package is needed, and ``default_source_data: True`` must be specified in the ``parent:`` block. Then, fluxes from the parent model are simply mapped to the inset model grid, based on the parent model cell centers, and the stress period mappings specified in the ``parent:`` block. Recharge package options can still be specified in a ``rch:`` block.
 
     * Raster input by stress period
         * A raster of spatially varying recharge values can be supplied for one or more model stress periods. Similar to the direct input, specified recharge will be applied to subsequent periods were recharge is not specified.
         * If the raster contains projection information (GeoTIFFs are preferred in part because of this), any reprojection to the model coorindate reference system (CRS) will be performed automatically as needed. Otherwise, the raster is assumed to be in the model projection.
         * Input items include:
             * ``length_units:`` input recharge length units (optional; if omitted no conversion is performed)
             * ``time_units:`` input recharge time units (optional; if omitted no conversion is performed)
@@ -279,21 +326,26 @@
 
             .. literalinclude:: ../../../mfsetup/tests/data/pfl_nwt_test.yml
                 :language: yaml
                 :lines: 99-106
 
     * NetCDF input
         * NetCDF input can be supplied for gridded values that vary in time and space.
-        * Due to the lack of standardization in NetCDF coordinate reference information, automatic reprojection is currently not supported for NetCDF files; the data are assumed to be in the model CRS.
+        * Automatic reprojection is supported for Climate Forecast (CF) 1.8-compliant netcdf files (that work with the :py:meth:`pyproj.CRS.from_cf() <pyproj.crs.CRS.from_cf>` constructor), or files that have a `'crs_wkt'` or `'proj4_string'` grid mapping variable (the latter includes many or most Soil Water Balance Code models).
+        * Otherwise, coordinate reference information can be supplied via the ``crs:`` item (using any valid input to :py:class:`pyproj.crs.CRS`), and the data will be reprojected to the model coordinate reference system.
+
         * Input items include:
+            * ``variable:`` name of variable in NetCDF file containing the recharge values.
             * ``length_units:`` input recharge length units (optional; if omitted no conversion is performed)
             * ``time_units:`` input recharge time units (optional; if omitted no conversion is performed)
+            * ``crs``: coordinate reference system (CRS) of the netcdf file (optional; only needed if the NetCDF file is in a different CRS than the model *and* automatic reprojection from the internal `grid mapping <http://cfconventions.org/cf-conventions/cf-conventions.html#grid-mappings-and-projections>`_ isn't working.
             * ``resample_method:`` method for resampling the data from the source grid to model grid. (optional; by default, ``'nearest'``)
             * ``period_stats:`` a sub-block that is used to specify mapping of the input data to the model temporal discretization. Items within period stats are numbered by stress period, with the entry for each item specifying the temporal aggregation. Currently, two options are supported:
                 * aggregation of measurements falling within a stress period. For example, assigning the mean value of all input data points within the stress period. In this case, the aggregration method is simply specified as a string. While ``mean`` is typical, any of the standard numpy aggregators can be use (``min``, ``max``, etc.)
                 * aggregation of measurements from an arbitrary time window. For example, applying a long-term mean to a steady-state stress period, or transient period representing a different time window. In this case three items are specified-- the aggregation method, the start date, and end date (e.g. ``[mean, 2000-01-01, 2017-12-31]``; see below for an example)
 
         * Examples:
 
             .. literalinclude:: ../../../mfsetup/tests/data/shellmound.yml
                 :language: yaml
-                :lines: 205-224
+                :start-after: # Recharge Package
+                :end-before: # Streamflow Routing Package
```

### Comparing `modflow-setup-0.2.0/docs/source/input/index.rst` & `modflow-setup-0.3.0/docs/source/input/index.rst`

 * *Files identical despite different names*

### Comparing `modflow-setup-0.2.0/docs/source/input/oc.rst` & `modflow-setup-0.3.0/docs/source/input/oc.rst`

 * *Files identical despite different names*

### Comparing `modflow-setup-0.2.0/docs/source/installation.rst` & `modflow-setup-0.3.0/docs/source/installation.rst`

 * *Files 19% similar despite different names*

```diff
@@ -3,20 +3,25 @@
 ============
 
 Installing python dependencies with Conda
 -----------------------------------------
 ``Modflow-setup`` depends on a number of python packages, many of which have external C library dependencies. The easiest way to install most of these is through a  `Conda environment`_, using `Mamba`_ as the package manager. A few packages are not available via Conda, and must be installed with `pip`_. If you are on the USGS internal network, see the `Considerations for USGS Users`_ section below first.
 
 
-Download and install the 64-bit `Anaconda python distribution`_ or `Miniconda <https://docs.conda.io/en/latest/miniconda.html>`_
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+Download and install a python distribution and Conda-like package installer
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+There are many ways to do this:
 
-  * Anaconda comes with a larger selection of popular data science and scientific packages, making it ideal for those who use python frequently for scientific computing.
-  * Miniconda is a minimal installer with a much smaller footprint, making it ideal for those who only want to use ``Modflow-setup``.
-  * **Make sure to install Anaconda or Miniconda to your username** (not at the system level). More often than not, installing at the system level (for all users) seems to result in issues with library dependencies (for example, import of ``fiona`` or ``rasterio`` failing because gdal isn't found). It is also good practice to periodically do a `clean uninstall`_ of Anaconda, which at the system level requires admin. privileges.
+    * The `Anaconda python distribution`_ comes with a large selection of popular data science and scientific packages pre-installed.
+
+    * `Miniconda <https://docs.conda.io/en/latest/miniconda.html>`_ is a minimal installer with a much smaller footprint, making it ideal for creating python environments dedicated to specific tasks (a recommended practice).
+
+    * `Mambaforge <https://github.com/conda-forge/miniforge#mambaforge>`_ is like Miniconda, but pre-configured to use the `Mamba`_ installer, and only the `conda-forge <https://conda-forge.org/docs/user/introduction.html>`_ channel for getting packages (more below). If the above two options don't work (for example, the Conda installer fails or gets stuck on the "solve" step), this may be your best option.
+
+**Make sure to install Anaconda or Miniconda to your username** (not at the system level). More often than not, installing at the system level (for all users) seems to result in issues with library dependencies (for example, import of ``fiona`` or ``rasterio`` failing because gdal isn't found). It is also good practice to periodically do a `clean uninstall`_ of Anaconda, which at the system level requires admin. privileges.
 
     * In the installer, at the “Destination Select” step, select “Install for me only.” It should say something about how the software will be installed to your home folder.
     * If your installer skips the “Destination Select” step, when you get to "Installation Type", click “Change Install Location” and then “Install for me only.”
 
 
 Download an environment file
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
@@ -30,17 +35,26 @@
   * Alternatively, clone (`using git`_) or `download`_ the ``modflow-setup`` repository, which includes the two environment files at the root level.
   * Note that both of these environment files contain a ``pip`` section of packages that will be installed with pip, after the ``Conda`` packages are installed.
 
 Creating a `Conda environment`_ using `Mamba`_
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 If you are on the USGS internal network, see the `Considerations for USGS Users`_ section below first.
 
-While Conda can of course be used to create a Conda environment, the Mamba package solver is generally faster and more robust, especially for larger, more complex environments like the included ``requirements.yml``. Mamba is a reimplementation of the conda package manager in C++.
+Before using Mamba, you will need to `install it first <https://mamba.readthedocs.io/en/latest/installation.html>`_.
+
+Python packages are available from conda via channels. Conda comes preconfigured to install packages from the default channel, which is maintained by Anaconda, Inc. In general, you may have better luck exclusively using the `conda-forge <https://conda-forge.org/docs/user/introduction.html>`_ channel instead, which is community-based and intended to provide a single location to get any package, with a minimum of hassle. In general, it is bad practice to mix package channels within a single environment. You can read more `here <https://conda-forge.org/docs/user/introduction.html>`__, but to set conda-forge as the default:
+
+.. code-block:: bash
+
+    conda config --add channels conda-forge
+
+.. note::
+    If you are having trouble installing Mamba (for example, the conda package solver fails when you try to install it, or takes an excessively long time), you may have better luck uninstalling `Anaconda completely <clean uninstall>`_ and installing `Mambaforge <https://github.com/conda-forge/miniforge#mambaforge>`_ instead, as directed in the Mamba install instructions. Mambaforge solves both of the above problems by providing a minimal python distribution and conda-style package installer that is preconfigured to use both `conda-forge <https://conda-forge.org/docs/user/introduction.html>`_ and `Mamba`_.
 
-To get started, open an Anaconda Command Prompt on Windows or a terminal window on OSX and point it to the location of ``requirements.yml`` or ``gis.yml`` and enter:
+Once you have a python distribution and mamba installed, to create the conda environment, open a new Anaconda Command Prompt on Windows or a new terminal window on OSX and point it to the location of ``requirements.yml`` or ``gis.yml`` and enter:
 
 .. code-block:: bash
 
     mamba env create -f requirements.yml
 
 Building the environment will probably take a while. If the build fails because of an SSL error, fix the problem (see `Considerations for USGS Users`_ below) and either:
 
@@ -58,37 +72,67 @@
         .. code-block:: bash
 
             mamba env remove -n mfsetup
             mamba env create -f requirements.yml
 
 Keeping the Conda environment up to date
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-The python packages and other open source software libraries that Modflow-setup depends on are continually changing. Modflow-setup aims to mostly follow the `Numpy guidelines for package support <https://numpy.org/neps/nep-0029-deprecation_policy.html>`_, which effectively means that the two latest minor versions of Python (e.g. 3.8 and 3.7) and their associated Numpy versions will be supported. However, occasionally backwards compatability with a particular package may be broken in a shorter timeframe, in which case the minimum required version of that package will be specified in the ``requirements.yml`` file. All of this to say that your Conda environment will eventually get out of date. The `Conda documentation <https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html>`_ has instructions for updating packages within a Conda environment, but at some point (perhaps a few times a year) it is good practice to simply delete the environment and rebuild it from the `.yml` file. Every so often, you may also want to reinstall Anaconda after a `clean uninstall`_.
+The python packages and other open source software libraries that Modflow-setup depends on are continually changing. Modflow-setup aims to mostly follow the `Numpy guidelines for package support <https://numpy.org/neps/nep-0029-deprecation_policy.html>`_, which effectively means that the two latest minor versions of Python (e.g. 3.11 and 3.10) and their associated Numpy versions will be supported. However, occasionally backwards compatability with a particular package may be broken in a shorter timeframe, in which case the minimum required version of that package will be specified in the ``requirements.yml`` file. All of this to say that your Conda environment will eventually get out of date. The `Conda documentation <https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html>`_ has instructions for updating packages within a Conda environment, but at some point (perhaps a few times a year) it is good practice to simply delete the environment and rebuild it from the `.yml` file. Every so often, you may also want to reinstall Anaconda after a `clean uninstall`_.
 
 Installing Modflow-setup
 -----------------------------
 There are several ways to install Modflow-setup. Regardless of the method, the installation must be performed in a python
 environment with the required dependencies. In the case of the Conda environment created above, the environment must be activated, so that right version of python is called when ``python`` is entered at the command line:
 
 .. code-block:: bash
 
     conda activate mfsetup
 
 (note that even with Mamba, ``conda activate/deactivate`` are still used)
 
 
+Installing and updating Modflow-setup from `PyPI <https://pypi.org/>`_
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+Once a suitable conda environment (that contains ALL of the dependencies) is made and activated, the simplest way to install Modflow-setup is from the Python Package Index using pip.
+
+.. code-block:: bash
+
+    pip install modflow-setup
+
+Subsequent releases of Modflow-setup to PyPI can then be installed with
+
+.. code-block:: bash
+
+    pip install --upgrade modflow-setup
+
+
+Note that in some situations you may have to ``pip uninstall modflow-setup`` and then ``pip install modflow-setup``. You can always check
+what version of Modflow-setup you have within a python session with
+
+.. code-block:: python
+
+    import mfsetup
+    mfsetup.__version__
+
+Or if you are using Conda, at the command line with
+
+.. code-block:: bash
+
+    conda list
+
 Installing the latest develop version of Modflow-setup
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-Pip can be used to fetch Modflow-setup directly from GitHub:
+In some situations you may want the bleeding-edge version of Modflow-setup that is being actively developed on GitHub. For example,
+to incorporate a bug fix that was made after the latest release. Pip can also be used to fetch Modflow-setup directly from GitHub:
 
 .. code-block:: bash
 
     pip install git+https://github.com/aleaf/modflow-setup@develop
 
-Subsequent updates can then be made with
+(for the develop branch). Subsequent updates can then be made with
 
 .. code-block:: bash
 
     pip uninstall modflow-setup
     pip install git+https://github.com/aleaf/modflow-setup@develop
 
 Installing the Modflow-setup source code in-place
@@ -113,14 +157,37 @@
 .. note::
     If you are making local changes to Modflow-setup that you want to contribute, the workflow is slightly different. See the :ref:`Contributing to Modflow-setup` page for more details.
 
 
 The advantage of installing the source code in-place is that any changes you make are automatically incorporated into your python environment, without any additional install commands. When debugging in an interactive development environment (IDE) such as Pycharm or VS Code, error tracebacks and inspection features go to the actual source code, not the version installed in the ``site-packages`` folder. Additionally, since this install is done through pip, ``pip uninstall``
 will work to remove the package, and the current version of the package (including the latest commit information) will be visible with ``conda list``.
 
+Installing the IPython kernel to use Modflow-setup in Jupyter Notebooks
+------------------------------------------------------------------------------------------------
+This step may not be needed if you already have an existing Python environment with the packages required by Modflow-setup *and* Jupyter Notebook installed. However, if you'd like to use Modflow-setup in a Jupyter Notebook with the included ``mfsetup`` environment (specified in ``requirements.yml``), you'll most likely need to install the IPython kernel in that environment. You can do this at the command line or terminal window (with ``mfsetup`` activated):
+
+.. code-block:: bash
+
+    python -m ipykernel install --user --name mfsetup --display-name "mfsetup"
+
+
+The first instance of ``mfsetup`` in this command is the environment to install the kernel to, and the second instance (in quotes) is the name that will appear in the ``Kernel`` menu within Jupyter Notebook. To use the kernel, simply select it from the ``Kernel > Change kernel`` menu within  Jupyter Notebook.
+
+Best practices
+------------------------
+
+* Install the \*conda distribution of your choice to your user account, NOT at the system level. Installing to your user means you have rights to delete and reinstall Anaconda as-needed, as well as to edit any configuration files for pip, Conda, etc. Installing at the system level also just seems to lead to more confusing problems with dependencies, at least in the USGS.
+* Periodically (maybe a few times a year?) fully remove your \*conda distribution and reinstall it. If you just can't get things to work (packages won't import or produce DLL errors on import, adding or upgrading a package takes a very long time or results in excessive upgrades or downgrades of other packages, etc.), fully removing and reinstalling \*conda just may resolve your issues.
+* Don't use your base environment; create and delete environments as needed. Conda is generally pretty good about managing packages between environments without wasting a lot of disk space.
+* Use an environment file (as above) to create a conda environment, instead of installing packages ad-hoc.
+* Use Mamba instead of Conda; it just works better for environments with a lot of packages.
+* After setting up the above conda environment, scan the screen output to make sure that everything installed correctly, especially the packages installed through pip.
+* Avoid mixing package channels within a Conda environment. Strictly sticking to conda-forge may yield the best results.
+* Use `conda-pack`_, rather than an overly-detailed environment file, to guarantee reproducibility.
+
 
 _`Considerations for USGS Users`
 --------------------------------
 Using conda or pip on the USGS network requires SSL verification, which can cause a number of issues.
 If you are encountering persistant issues with creating the conda environment,
 you may have better luck trying the install off of the USGS network (e.g. at home).
 See `here <https://tst.usgs.gov/applications/application-and-script-signing/>`_ for more information
@@ -212,14 +279,15 @@
 
 
 .. _Anaconda python distribution: https://www.anaconda.com/distribution/
 .. _clean uninstall: https://docs.anaconda.com/anaconda/install/uninstall/
 .. _Conda: https://docs.conda.io/en/latest/
 .. _Mamba: https://mamba.readthedocs.io/en/latest/
 .. _Conda environment: https://docs.conda.io/projects/conda/en/latest/user-guide/concepts/environments.html
+.. _conda-pack: https://conda.github.io/conda-pack/
 .. _condarc: https://docs.conda.io/projects/conda/en/latest/user-guide/configuration/use-condarc.html
 .. _download: https://github.com/aleaf/modflow-setup/archive/master.zip
 .. _gis.yml: https://raw.githubusercontent.com/aleaf/modflow-setup/master/gis.yml
 .. _Download the DOI SSL certificate: https://tst.usgs.gov/applications/application-and-script-signing/
 .. _pip: https://packaging.python.org/tutorials/installing-packages/#use-pip-for-installing
 .. _Readme file: https://github.com/aleaf/modflow-setup/blob/master/Readme.md
 .. _requirements.yml: https://raw.githubusercontent.com/aleaf/modflow-setup/master/requirements.yml
```

### Comparing `modflow-setup-0.2.0/docs/source/philosophy.rst` & `modflow-setup-0.3.0/docs/source/philosophy.rst`

 * *Files identical despite different names*

### Comparing `modflow-setup-0.2.0/docs/source/pleasant-example.rst` & `modflow-setup-0.3.0/docs/source/pleasant-example.rst`

 * *Files identical despite different names*

### Comparing `modflow-setup-0.2.0/docs/source/references.rst` & `modflow-setup-0.3.0/docs/source/references.rst`

 * *Files identical despite different names*

### Comparing `modflow-setup-0.2.0/docs/source/release-history.rst` & `modflow-setup-0.3.0/docs/source/release-history.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,46 @@
 ===============
 Release History
 ===============
 
+
+Version 0.3.0 (2023-07-25)
+----------------------------------------
+
+* Transient input to basic stress packages can now be supplied via a ``csvfile:`` block. Transient
+  values for the package variables are associated with the shapefile feature extents via an
+  ``id_column`` of values that match values in the shapefile id_column. Input can be mixed between
+  transient ``csvfile:`` input and static input supplied via rasters (that varies spatially)
+  or uniform global values. See the Basic stress packages section in the documentation for more details.
+* add automatic reprojection of NetCDF source data files
+* most Soil Water Balance code models should be work as-is
+* added ``crs:`` configuration file item to specify the coordinate reference system for NetCDF files
+  where coordinate reference information can't be parsed.
+* add support for inner and outer CSV file output in MODFLOW 6 IMS options (remap input to work with Flopy)
+* refactor ``grid.rasterize()`` function to work with standard Flopy ``StructuredGrid`` (s)
+* refactor MODFLOW 6 head observations setup
+* add ``allow_obs_in_bc_cells`` option to allow observations in boundary condition cells (previously not allowed).
+* put modflow-setup specific options in an ``mfsetup_options:`` sub-block, consistent with other packages
+* fixes to adapted to breaking changes with pandas 2.0 and revised flopy modelgrid/crs interface
+* fix ``AttributeError`` issue with model name not getting passed to flopy
+* some fixes to model version reporting in MODFLOW input file headers
+
 Version 0.2.0 (2023-02-06)
 ----------------------------------------
 * add minimal support for MODFLOW-2000 parent models and variably-spaced structured grids
     * relax requirement that inset cells align with parent cells
     * add package translations between mf6 and mf2k
 * remove all basic stress package bcs from inactive cells prior to write
 * fix to allow for no epsg input argument to setup_grid (crs is now favored)
 * add support for virtual raster (`*.vrt` file) input
 * add support for parent MODFLOW model Name files with blank lines
 * other fixes to adapt to breaking changes in numpy 1.24, pandas, inspect, collections and SFRmaker
 
 Version 0.1.0 Initial release (2022-09-30)
-----------------------------------------
+-----------------------------------------------
 * support for constructing MODFLOW-NWT or MODFLOW-6 models from scratch
 * supported source dataset formats include GeoTiff, Arc-Ascii grids, shapefiles, NetCDF, and CSV files
 * automatic reprojection of source datasets that have CRS information (GeoTiffs, shapefiles, etc.)
 * supported MODFLOW-NWT packages: DIS, BAS6, OC, UPW, RCH, GHB, SFR2, LAK, WEL, MNW2, HYD, GAGE, NWT, CHD, DRN, GHB, RIV
 * supported MODFLOW-6 packages: DIS, IC, OC, NPF, RCHA, SFR, LAK, WEL, OBS, IMS, TDIS, CHD, DRN, GHB, RIV
 * Lake observations are set up automatically (one output file per lake); basic stress package observations are also setup up automatically
 * SFR observations can be set up via an ``observations`` block in the SFR package ``source_data``
```

### Comparing `modflow-setup-0.2.0/docs/source/structure.rst` & `modflow-setup-0.3.0/docs/source/structure.rst`

 * *Files identical despite different names*

### Comparing `modflow-setup-0.2.0/docs/source/troubleshooting.rst` & `modflow-setup-0.3.0/docs/source/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `modflow-setup-0.2.0/mfsetup/bcs.py` & `modflow-setup-0.3.0/mfsetup/bcs.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,82 +1,140 @@
 """
 Functions for simple MODFLOW boundary conditions such as ghb, drain, etc.
 """
 import numbers
 import shutil
 
 import flopy
+import geopandas as gpd
 import numpy as np
 import pandas as pd
 
 fm = flopy.modflow
 import pyproj
 import rasterio
 from gisutils import project
 from rasterstats import zonal_stats
 from shapely.geometry import Polygon
 
-from mfsetup.discretization import cellids_to_kij, get_layer
+from mfsetup.discretization import cellids_to_kij, get_highest_active_layer, get_layer
 from mfsetup.grid import rasterize
-from mfsetup.units import convert_length_units
+from mfsetup.sourcedata import TransientTabularSourceData
+from mfsetup.units import convert_length_units, convert_time_units
+
+
+def is_number(s):
+    try:
+        float(s)
+        return True
+    except ValueError:
+        return False
 
 
 def setup_basic_stress_data(model, shapefile=None, csvfile=None,
                             head=None, elev=None, bhead=None, stage=None,
                             cond=None, rbot=None, default_rbot_thickness=1,
                             all_touched=True,
                             **kwargs):
 
     m = model
 
+    # basic stress package variables
+    variables = {'head': head, 'elev': elev, 'bhead': bhead,
+                 'stage': stage, 'cond': cond, 'rbot': rbot}
+
     # get the BC cells
     # todo: generalize more of the GHB setup code and move it somewhere else
     bc_cells = None
     if shapefile is not None:
         shapefile = shapefile.copy()
         key = [k for k in shapefile.keys() if 'filename' in k.lower()]
         if key:
             shapefile_name = shapefile.pop(key[0])
             if 'all_touched' in shapefile:
                 all_touched = shapefile['all_touched']
                 if 'boundname_col' in shapefile:
                     shapefile['names_column'] = shapefile.pop('boundname_col')
             bc_cells = rasterize(shapefile_name, m.modelgrid, **shapefile)
+            bc_cell_id_kwargs = shapefile.copy()
+            bc_cell_id_kwargs['names_column'] = shapefile['id_column']
+            bc_cell_ids = rasterize(shapefile_name, m.modelgrid, **bc_cell_id_kwargs)
+            # fill unnamed feature names with id numbers (as strings)
+            unnamed = bc_cells == 'nan'
+            bc_cells[unnamed] = bc_cell_ids[unnamed]
+
+    csv_input = None
     if csvfile is not None:
-        raise NotImplementedError('Time-varying (CSV) file input not yet supported for this package.')
+        csv_kwargs = csvfile.copy()
+        csv_kwargs['filenames'] = [csv_kwargs.pop('filename')]
+        data_columns = {v: k.split('_')[0] for k, v in csv_kwargs.items()
+                                  if k.split('_')[0] in variables.keys()}
+        csv_kwargs['data_columns'] = list(data_columns.keys())
+        sd = TransientTabularSourceData(
+                dest_model=m, **csv_kwargs)
+        csv_input = sd.get_data()
+        csv_input.index = csv_input[csv_kwargs['id_column']].astype(str)
+        # rename the input data columns to their MODFLOW variable names
+        csv_input.rename(columns=data_columns, inplace=True)
+
+        #raise NotImplementedError('Time-varying (CSV) file input not yet supported for this package.')
     if bc_cells is None:
         return
 
     # create polygons of model grid cells
     if bc_cells.dtype == object:
         cells_with_bc = bc_cells.flat != ''
     else:
         cells_with_bc = bc_cells.flat > 0
+
     vertices = np.array(m.modelgrid.vertices)[cells_with_bc, :, :]
     polygons = [Polygon(vrts) for vrts in vertices]
 
     # setup DataFrame for MODFLOW input
     i, j = np.indices((m.nrow, m.ncol))
-    df = pd.DataFrame({'per': 0,
+    # start with stress period 0 as a template
+    df_0 = pd.DataFrame({'per': 0,
                        'k': 0,
                        'i': i.flat,
                        'j': j.flat})
     # add the boundnames
     if bc_cells.dtype == object:
-        df['boundname'] = bc_cells.flat
-        nan_boundnames = df.boundname.isna() | df.boundname.isin({'', 'nan'})
-        df.loc[nan_boundnames, 'boundname'] = 'unnamed'
+        df_0['boundname'] = bc_cells.flat
+        nan_boundnames = df_0.boundname.isna() | df_0.boundname.isin({'', 'nan'})
+        df_0.loc[nan_boundnames, 'boundname'] = 'unnamed'
+        # convert any numeric boundnames to strings
+        # (otherwise MODFLOW 6 will mistake them for cell IDs)
+        df_0['boundname'] = [f"feature-{bname}" if is_number(bname)
+                             else bname for bname in df_0['boundname']]
+    # add the feature ids
+    # (for associating transient input with cells)
+    df_0['feature_id'] = bc_cell_ids.flat
+    df_0.index = df_0['feature_id']
+
     # cull to just the cells with bcs
-    df = df.loc[cells_with_bc].copy()
+    df_0 = df_0.loc[cells_with_bc].copy()
+    df = gpd.GeoDataFrame(df_0, geometry=polygons, crs=model.modelgrid.crs)
 
-    variables = {'head': head, 'elev': elev, 'bhead': bhead,
-                 'stage': stage, 'cond': cond, 'rbot': rbot}
+    # collect input that may be mixed
+    # between transient input supplied via csvfiles
+    # and static input supplied via rasters or global values
     for var, entry in variables.items():
-        if entry is not None:
-            # Raster of variable values supplied
+        # check for transient csv input for the variable
+        if csv_input is not None and var in csv_input:
+            df_0 = df.copy()
+            dfs = []
+            for per in csv_input['per'].unique():
+                df_per = df_0.copy()
+                df_per['per'] = per
+                df_per[var] = csv_input.loc[csv_input['per'] == per, var]
+                dfs.append(df_per)
+            df = pd.concat(dfs, axis=0)
+        # otherwise, check for static input
+        elif entry is not None:
+            # Raster of spatially varying values supplied
             if isinstance(entry, dict):
                 filename_entries = [k for k in entry.keys() if 'filename' in k.lower()]
                 if not any(filename_entries):
                     continue
                 filename = entry[filename_entries[0]]
                 with rasterio.open(filename) as src:
                     meta = src.meta
@@ -84,15 +142,17 @@
                 # reproject the polygons to the dem crs if needed
                 try:
                     from gisutils import get_authority_crs
                     raster_crs = get_authority_crs(src.crs)
                 except:
                     raster_crs = pyproj.crs.CRS.from_user_input(src.crs)
                 if raster_crs != m.modelgrid.crs:
-                    polygons = project(polygons, m.modelgrid.crs, raster_crs)
+                    polygons = project(df.geometry.tolist(), m.modelgrid.crs, raster_crs)
+                else:
+                    polygons = df.geometry.tolist()
 
                 # all_touched arg for rasterstats.zonal_stats
                 all_touched = False
                 if meta['transform'][0] > m.modelgrid.delr[0]:
                     all_touched = True
                 stat = entry['stat']
                 results = zonal_stats(polygons, filename, stats=stat,
@@ -101,19 +161,24 @@
                 #values[cells_with_bc] = np.array([r[stat] for r in results])
                 values = np.array([r[stat] for r in results])
                 # cull to polygon statistics within model area
                 valid = values != None
                 values = values[valid]
                 df = df.loc[valid].copy()
 
-                units_key = [k for k in entry if 'units' in k]
-                if len(units_key) > 0:
-                    values *= convert_length_units(entry[units_key[0]],
+                # Convert units if they are specified
+                # Note: this only works because the variables considered here
+                # all have length in the numerator
+                # and cond has time in the denominator
+                if 'length_units' in entry:
+                    values *= convert_length_units(entry['length_units'],
                                                     model.length_units)
-                #values = np.reshape(values, (m.nrow, m.ncol))
+                if var == 'cond' and 'time_units' in entry:
+                    values /= convert_time_units(entry['time_units'],
+                                                    model.time_units)
 
                 # add the layer and the values to the Modflow input DataFrame
                 # assign layers so that the elevation is above the cell bottoms
                 if var in ['head', 'elev', 'bhead']:
                     df['k'] = get_layer(model.dis.botm.array, df.i, df.j, values)
                 df[var] = values
             # single global value specified
@@ -127,37 +192,59 @@
 
     # drop cells that don't include this boundary condition
     df.dropna(axis=0, inplace=True)
 
     # special handling of rbot for RIV package
     if 'stage' in df.columns and 'rbot' not in df.columns:
         df['rbot'] = df['stage'] - default_rbot_thickness
-        df['k'] = get_layer(model.dis.botm.array, df.i, df.j, df['rbot'])
+
+    # exclude inactive cells
+    #k, i, j = df.k, df.i, df.j
+    if model.version == 'mf6':
+        idomain = model.idomain
+    else:
+        idomain = model.ibound
 
     # remove BC cells from places where the specified head is below the model
+    # set the layer according to the variable
     for var in ['head', 'elev', 'bhead', 'rbot']:
         if var in df.columns:
             below_bottom_of_model = df[var] < model.dis.botm.array[-1, df.i, df.j] + 0.01
             df = df.loc[~below_bottom_of_model].copy()
+            df['k'] = get_layer(model.dis.botm.array,
+                                df['i'], df['j'], df[var])
+            # move any variable elevations in inactive cells
+            # to the highest active layer below
+            df['idomain'] = idomain[df['k'], df['i'], df['j']]
+            if any(df['idomain'] < 1):
+                idomain_slice = idomain[:, df['i'], df['j']]
+                is_above = model.dis.botm.array[:, df['i'], df['j']] > \
+                    [df[var].tolist()] * idomain.shape[0]
+                idomain_slice[is_above] = 0
+                highest_active_below = np.argmax(idomain_slice, axis=0)
+                df.loc[df['idomain'] < 1, 'k'] = highest_active_below[df['idomain'] < 1]
+
+    #active_cells = idomain[k, i, j] >= 1
+    #df = df.loc[active_cells]
+
+    # set layer to the highest active
+    #highest_active = get_highest_active_layer(idomain)
+    #df['k'] = highest_active[df['i'], df['j']]
 
-    # exclude inactive cells
-    k, i, j = df.k, df.i, df.j
-    if model.version == 'mf6':
-        active_cells = model.idomain[k, i, j] >= 1
-    else:
-        active_cells = model.ibound[k, i, j] >= 1
-    df = df.loc[active_cells]
+    # drop locations that are completely inactive
+    df = df.loc[df['k'].isin(range(idomain.shape[0]))]
 
     # sort the columns
     col_order = ['per', 'k', 'i', 'j', 'head', 'elev', 'bhead', 'stage',
                  'cond', 'rbot', 'boundname']
     cols = [c for c in col_order if c in df.columns]
     df = df[cols].copy()
     return df
 
+
 def get_bc_package_cells(package, exclude_horizontal=True):
     """
 
     Parameters
     ----------
     package : flopy package instance for boundary condition
 
@@ -221,18 +308,14 @@
     # monkey patch the mf6 version to behave like the mf2005 version
     #if isinstance(mftransientlist, flopy.mf6.data.mfdatalist.MFTransientList):
     #    mftransientlist.data = {per: ra for per, ra in enumerate(mftransientlist.array)}
 
     # find relevant variable names
     # may have to iterate over the first stress period
     #for per in range(data.model.nper):
-    try:
-        data.data
-    except:
-        j=2
     for per, spd in data.data.items():
         if spd is not None and hasattr(spd, 'dtype'):
             varnames = list([n for n in spd.dtype.names
                              if n not in ['k', 'i', 'j', 'cellid', 'boundname']])
             break
 
     # create list of dataframes for each stress period
```

### Comparing `modflow-setup-0.2.0/mfsetup/checks.py` & `modflow-setup-0.3.0/mfsetup/checks.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,15 +15,16 @@
     time discretization
     (https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.date_range.html)
     """
     perlen = data.get('perlen') is not None
     steady = data.get('steady', False)
     if isinstance(steady, dict):
         steady = steady.get(0)
-    if not steady:
+    # if there's at least one transient stress period
+    if not np.all(steady):
         included = [k for k in ['nper', 'start_date_time', 'end_date_time', 'freq']
                     if data.get(k) is not None]
         has3 = len(included) >= 3
         return perlen or has3
     else:
         nper = data.get('nper') is not None
         return nper or perlen
```

### Comparing `modflow-setup-0.2.0/mfsetup/config.py` & `modflow-setup-0.3.0/mfsetup/config.py`

 * *Files identical despite different names*

### Comparing `modflow-setup-0.2.0/mfsetup/discretization.py` & `modflow-setup-0.3.0/mfsetup/discretization.py`

 * *Files 2% similar despite different names*

```diff
@@ -452,29 +452,39 @@
         #min_layer_thickness = minimum_layer_thickness
         #isthin = np.diff(all_layers, axis=0) * -1 < min_layer_thickness + tol
         #criteria = criteria | isthin
     idomain = np.abs(~criteria).astype(int)
     return idomain
 
 
+def get_highest_active_layer(idomain, null_value=-9999):
+    """Get the highest active model layer at each
+    i, j location, accounting for inactive and
+    vertical pass-through cells."""
+    idm = idomain.copy()
+    # reset all inactive/passthrough values to large positive value
+    # for min calc
+    idm[idm < 1] = 9999
+    highest_active_layer = np.argmin(idm, axis=0)
+    # set locations with all inactive cells to null values
+    highest_active_layer[(idm == 9999).all(axis=0)] = null_value
+    return highest_active_layer
+
+
 def make_irch(idomain):
-    # make the irch array
-    # copy idomain
-    idm_lay = idomain.copy()
-    for i,cl in enumerate(idm_lay):
-        # set both inactive and pass through cells to -1
-        cl[cl<=0] = -1
-        # set active cells to current layer
-        cl[cl>0] = i
-    # now reset all the inactive/passthrough values to large positive to not mess up min calc
-    idm_lay[idm_lay==-1] = 9999
-    # find min active layer
-    irch = np.min(idm_lay, axis=0)
-    # set all inactive and pass through back to -1
-    irch[irch==9999] = 0
+    """Make an irch array for the MODFLOW 6 Recharge Package,
+    which specifies the highest active model layer at each
+    i, j location, accounting for inactive and
+    vertical pass-through cells. Set all i, j locations
+    with no active layers to 1 (MODFLOW 6 only allows
+    valid layer numbers in the irch array).
+    """
+    irch = get_highest_active_layer(idomain, null_value=-9999)
+    # set locations where all layers are inactive back to 0
+    irch[irch == -9999] = 0
     irch += 1 # set to one-based
     return irch
 
 
 def get_layer_thicknesses(top, botm, idomain=None):
     """For each i, j location in the grid, get thicknesses
     between pairs of subsequent valid elevation values. Make
```

### Comparing `modflow-setup-0.2.0/mfsetup/equality.py` & `modflow-setup-0.3.0/mfsetup/equality.py`

 * *Files identical despite different names*

### Comparing `modflow-setup-0.2.0/mfsetup/evaporation.py` & `modflow-setup-0.3.0/mfsetup/evaporation.py`

 * *Files identical despite different names*

### Comparing `modflow-setup-0.2.0/mfsetup/fileio.py` & `modflow-setup-0.3.0/mfsetup/fileio.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,15 +146,15 @@
 
 def append_csv(filename, df, **kwargs):
     """Read data from filename,
     append to dataframe, and write appended dataframe
     back to filename."""
     if os.path.exists(filename):
         written = pd.read_csv(filename)
-        df = df.append(written)
+        df = pd.concat([df, written], axis=0)
     df.to_csv(filename, **kwargs)
 
 
 def load_cfg(cfgfile, verbose=False, default_file=None):
     """This method loads a YAML or JSON configuration file,
     applies configuration defaults from a default_file if specified,
     adds the absolute file path of the configuration file
```

### Comparing `modflow-setup-0.2.0/mfsetup/grid.py` & `modflow-setup-0.3.0/mfsetup/grid.py`

 * *Files 2% similar despite different names*

```diff
@@ -200,17 +200,15 @@
             return self.nrow * self.ncol
         return self.nlay * self.nrow * self.ncol
 
     @property
     def transform(self):
         """Rasterio Affine object (same as transform attribute of rasters).
         """
-        return Affine(self.delr[0], 0., self.xul,
-                      0., -self.delc[0], self.yul) * \
-               Affine.rotation(-self.angrot)
+        return get_transform(self)
 
     @property
     def crs(self):
         """pyproj.crs.CRS instance describing the coordinate reference system
         for the model grid.
         """
         return self._crs
@@ -237,19 +235,14 @@
               - An object with a `to_wkt` method.
               - A :class:`pyproj.crs.CRS` class
         """
         crs = get_crs(crs=crs)
         self._crs = crs
 
     @property
-    def epsg(self):
-        if self.crs is not None:
-            return self.crs.to_epsg()
-
-    @property
     def proj_str(self):
         if self.crs is not None:
             return self.crs.to_proj4()
 
     @property
     def wkt(self):
         if self.crs is not None:
@@ -695,15 +688,15 @@
 
     if crs is not None:
         if version.parse(gisutils.__version__) < version.parse('0.2.0'):
             raise ValueError("The rasterize function requires gisutils >= 0.2")
         from gisutils import get_authority_crs
         crs = get_authority_crs(crs)
 
-    trans = grid.transform
+    trans = get_transform(grid)
 
     if isinstance(feature, str) or isinstance(feature, Path):
         df = gpd.read_file(feature)
     elif isinstance(feature, pd.DataFrame):
         df = feature.copy()
         df = gpd.GeoDataFrame(df, crs=crs)
     elif isinstance(feature, collections.abc.Iterable):
@@ -725,15 +718,18 @@
 
     # reproject to grid crs
     if df.crs is not None:
         orig_crs = df.crs
         df.to_crs(grid.crs, inplace=True)
         if not df['geometry'].is_valid.all():
             df['geometry'] = [g.buffer(0) for g in df.geometry]
-        if not df['geometry'].is_valid.all():
+        geoms_are_valid = df['geometry'].is_valid.all() & \
+            (not df.geometry.is_empty.any()) & \
+                np.isfinite(df.geometry.bounds.sum().sum())
+        if not geoms_are_valid:
             raise ValueError('Something went wrong with reprojecting '
                              f'the input features from\n{orig_crs}\nto\n{grid.crs}\n'
                              'Check the input feature and model grid projections'
                              'If you are on a network that requires special '
                              'SSL authentication, try running this operation '
                              'again off-network.'
                              )
@@ -1134,7 +1130,22 @@
     k, i, j = get_kij_from_node3d(df['n'].values, nrow, ncol)
     df['kn'], df['in'], df['jn'] = k, i, j
     k, i, j = get_kij_from_node3d(df['m'].values, nrow, ncol)
     df['km'], df['im'], df['jm'] = k, i, j
     df.reset_index()
     print(f"Getting intercell connections took {time.time() - ta:.2f}s\n")
     return df
+
+
+def get_transform(modelgrid):
+    """Get a rasterio Affine object from a Flopy modelgrid
+    (same as transform attribute of rasters).
+    """
+    if not isinstance(modelgrid, StructuredGrid):
+        raise ValueError(
+            f"{type(modelgrid)}: Input needs to be a flopy.discretization.StructuredGrid")
+    x0 = modelgrid.xyedges[0][0]
+    y0 = modelgrid.xyedges[1][0]
+    xul, yul = modelgrid.get_coords(x0, y0)
+    return Affine(modelgrid.delr[0], 0., xul,
+                    0., -modelgrid.delc[0], yul) * \
+            Affine.rotation(-modelgrid.angrot)
```

### Comparing `modflow-setup-0.2.0/mfsetup/ic.py` & `modflow-setup-0.3.0/mfsetup/ic.py`

 * *Files identical despite different names*

### Comparing `modflow-setup-0.2.0/mfsetup/interpolate.py` & `modflow-setup-0.3.0/mfsetup/interpolate.py`

 * *Files identical despite different names*

### Comparing `modflow-setup-0.2.0/mfsetup/lakes.py` & `modflow-setup-0.3.0/mfsetup/lakes.py`

 * *Files 1% similar despite different names*

```diff
@@ -397,15 +397,15 @@
             inactive = model.idomain[k, i, j] < 1
             horizontal_connections = horizontal_connections.loc[~inactive].copy()
             horizontal_connections['lakeno'] = lake_id
             k, i, j = horizontal_connections[['k', 'i', 'j']].T.values
             horizontal_connections['zone'] = littoral_profundal_zones[i, j]
             horizontal_connections['cellid'] = list(zip(k, i, j))
             horizontal_connections.drop(['k', 'i', 'j'], axis=1, inplace=True)
-            df = df.append(horizontal_connections)
+            df = pd.concat([df, horizontal_connections], axis=0)
     # assign iconn (connection number) values for each lake
     dfs = []
     for lakeno, group in df.groupby('lakeno'):
         group = group.copy()
         group['iconn'] = list(range(len(group)))
         dfs.append(group)
     df = pd.concat(dfs)
@@ -479,15 +479,15 @@
     lakeperioddata = {}
     periods = lake_fluxes.groupby('per')
     for per, group in periods:
         group = group.replace('ACTIVE', np.nan)
         group.rename(columns={'precipitation': 'rainfall'}, inplace=True)
         group.index = group.lak_id.values
         datacols = {'rainfall', 'evaporation', 'withdrawal', 'runoff', 'stage'}
-        datacols = datacols.intersection(group.columns)
+        datacols = [c for c in group.columns if c in datacols]
         group = group.loc[:, datacols]
         data = group.stack().reset_index()
         data.rename(columns={'level_0': 'lakeno',
                              0: 'value'}, inplace=True)
         # data['laksetting'] = ['{} {}'.format(variable, value)
         #                      for variable, value in zip(data['level_1'], data['value'])]
         data['lakeno'] -= 1
```

### Comparing `modflow-setup-0.2.0/mfsetup/mf5to6.py` & `modflow-setup-0.3.0/mfsetup/mf5to6.py`

 * *Files identical despite different names*

### Comparing `modflow-setup-0.2.0/mfsetup/mf6_defaults.yml` & `modflow-setup-0.3.0/mfsetup/mf6_defaults.yml`

 * *Files 2% similar despite different names*

```diff
@@ -170,14 +170,16 @@
     save_flows: True
     boundnames: True
   source_data:
     shapefile:
       all_touched: True
     elev:
       stat: 'min'
+    cond:
+      stat: 'mean'
   mfsetup_options:
     external_files: True  # option to write stress_period_data to external files
     external_filename_fmt: "drn_{:03d}.dat"
 
 ghb:
   options:
     print_input: False
@@ -185,14 +187,16 @@
     save_flows: True
     boundnames: True
   source_data:
     shapefile:
       all_touched: True
     bhead:
       stat: 'min'
+    cond:
+      stat: 'mean'
   mfsetup_options:
     external_files: True  # option to write stress_period_data to external files
     external_filename_fmt: "ghb_{:03d}.dat"
 
 riv:
   options:
     print_input: True
@@ -200,14 +204,16 @@
     save_flows: True
     boundnames: True
   source_data:
     shapefile:
       all_touched: True
     stage:
       stat: 'min'
+    cond:
+      stat: 'mean'
   output_files:
     rivdata_file: '{}_rivdata.csv' # table with auxillary information on river reaches (routing, source hydrography IDs, etc.)
   mfsetup_options:
     default_rbot_thickness: 1.
     external_files: True  # option to write stress_period_data to external files
     external_filename_fmt: "riv_{:03d}.dat"
 
@@ -238,23 +244,25 @@
 obs:
   options:
     digits: 10
     print_input: True
   source_data:
     column_mappings:
       hydlbl: ['obsprefix', 'obsnme', 'common_name']
-  default_columns:
     x_location_col: 'x' # x coordinates in wtm
     y_location_col: 'y' # y coordinates in wtm
-  filename_fmt: '{}.head.obs'  # only head obs supported at this point
+  mfsetup_options:
+    allow_obs_in_bc_cells: False
+    obsname_character_limit: 40  # modflow 6 limit
+    filename_fmt: '{}.head.obs'  # only head obs supported at this point
 
 ims:
   options:
     print_option: 'all'
-    'csv_output fileout': '{}_solver_out.csv'
+    csv_outer_output: 'solver_outer_out.csv'
   nonlinear:
     outer_dvclose: 1.e-1
     outer_maximum: 200
     under_relaxation:  'dbd'
     under_relaxation_theta: 0.7
     under_relaxation_kappa: 0.1
     under_relaxation_gamma: 0.0
```

### Comparing `modflow-setup-0.2.0/mfsetup/mf6model.py` & `modflow-setup-0.3.0/mfsetup/mf6model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import copy
 import os
 import shutil
 import time
 
 import flopy
 import numpy as np
 import pandas as pd
@@ -33,26 +34,26 @@
     setup_lake_tablefiles,
     setup_mf6_lake_obs,
 )
 from mfsetup.mfmodel import MFsetupMixin
 from mfsetup.mover import get_mover_sfr_package_input
 from mfsetup.obs import setup_head_observations
 from mfsetup.oc import parse_oc_period_input
-from mfsetup.tdis import add_date_comments_to_tdis
+from mfsetup.tdis import add_date_comments_to_tdis, setup_perioddata
 from mfsetup.units import convert_time_units
 from mfsetup.utils import flatten, get_input_arguments
 
 
 class MF6model(MFsetupMixin, mf6.ModflowGwf):
     """Class representing a MODFLOW-6 model.
     """
     default_file = '/mf6_defaults.yml'
 
-    def __init__(self, simulation=None, parent=None, cfg=None,
-                 modelname='model', exe_name='mf6', load=False,
+    def __init__(self, simulation=None, modelname='model', parent=None, cfg=None,
+                 exe_name='mf6', load=False,
                  version='mf6', lgr=False, **kwargs):
         defaults = {'simulation': simulation,
                     'parent': parent,
                     'modelname': modelname,
                     'exe_name': exe_name,
                     'version': version,
                     'lgr': lgr}
@@ -116,14 +117,71 @@
     def length_units(self):
         return self.cfg['dis']['options']['length_units']
 
     @property
     def time_units(self):
         return self.cfg['tdis']['options']['time_units']
 
+
+    @property
+    def perioddata(self):
+        """DataFrame summarizing stress period information.
+        Columns:
+        ============== =========================================
+        start_datetime Start date of each model stress period
+        end_datetime   End date of each model stress period
+        time           MODFLOW elapsed time, in days*
+        per            Model stress period number
+        perlen         Stress period length (days)
+        nstp           Number of timesteps in stress period
+        tsmult         Timestep multiplier
+        steady         Steady-state or transient
+        oc             Output control setting for MODFLOW
+        parent_sp      Corresponding parent model stress period
+        ============== =========================================
+        """
+        if self._perioddata is None:
+            # check first for already loaded time discretization info
+            try:
+                tdis_perioddata_config = {col: getattr(self.modeltime, col)
+                                          for col in ['perlen', 'nstp', 'tsmult']}
+                nper = self.modeltime.nper
+                steady = self.modeltime.steady_state
+                default_start_datetime = self.modeltime.start_datetime
+            except:
+                tdis_perioddata_config = self.cfg['tdis']['perioddata']
+                default_start_datetime = self.cfg['tdis']['options'].get('start_date_time',
+                                                                         '1970-01-01')
+                #tdis_dimensions_config = self.cfg['tdis']['dimensions']
+                nper = self.cfg['tdis']['dimensions'].get('nper')
+                # steady can be input in either the tdis or sto input blocks
+                steady = self.cfg['tdis'].get('steady')
+                if steady is None:
+                    steady = self.cfg['sto'].get('steady')
+
+            parent_stress_periods = self.cfg.get('parent').get('copy_stress_periods')
+            perioddata = setup_perioddata(
+                    self,
+                    tdis_perioddata_config=tdis_perioddata_config,
+                    default_start_datetime=default_start_datetime,
+                    nper=nper, steady=steady,
+                    time_units=self.time_units,
+                    parent_model=self.parent,
+                    parent_stress_periods=parent_stress_periods,
+                    )
+            self._perioddata = perioddata
+            # reset nper property so that it will reference perioddata table
+            self._nper = None
+            self._perioddata.to_csv(f'{self._tables_path}/stress_period_data.csv', index=False)
+            # update the model configuration
+            if 'parent_sp' in perioddata.columns:
+                self.cfg['parent']['copy_stress_periods'] = perioddata['parent_sp'].tolist()
+
+        return self._perioddata
+
     @property
     def idomain(self):
         """3D array indicating which cells will be included in the simulation.
         Made a property so that it can be easily updated when any packages
         it depends on change.
         """
         if self._idomain is None and 'DIS' in self.get_package_list():
@@ -403,17 +461,14 @@
             if v not in kwargs:
                 kwargs[v] = kwargs.pop(k)
         kwargs['length_units'] = self.length_units
         # get the arguments for the flopy version of ModflowGwfdis
         # but instantiate with modflow-setup subclass of ModflowGwfdis
         kwargs = get_input_arguments(kwargs, mf6.ModflowGwfdis)
         dis = ModflowGwfdis(model=self, **kwargs)
-        self._perioddata = None  # reset perioddata
-        #if not isinstance(self._modelgrid, MFsetupGrid):
-        #    self._modelgrid = None  # override DIS package grid setup
         self._mg_resync = False
         self._reset_bc_arrays()
         self._set_idomain()
         print("finished in {:.2f}s\n".format(time.time() - t0))
         return dis
 
     def setup_tdis(self):
@@ -681,22 +736,34 @@
         """
         Sets up the OBS utility.
         """
         package = 'obs'
         print('\nSetting up {} package...'.format(package.upper()))
         t0 = time.time()
 
+        iobs_domain = None
+        if not kwargs['mfsetup_options']['allow_obs_in_bc_cells']:
+            # for now, discard any head observations in same (i, j) column of cells
+            # as a non-well boundary condition
+            # including lake package lakes and non lake, non well BCs
+            # (high-K lakes are excluded, since we may want head obs at those locations,
+            #  to serve as pseudo lake stage observations)
+            iobs_domain = ~((self.isbc == 1) | np.any(self.isbc > 2))
+
         # munge the observation data
         df = setup_head_observations(self,
-                                     format=package,
-                                     obsname_column='obsname')
+                                     obs_package=package,
+                                     obsname_column='obsname',
+                                     iobs_domain=iobs_domain,
+                                     **kwargs['source_data'],
+                                     **kwargs['mfsetup_options'])
 
         # reformat to flopy input format
         obsdata = df[['obsname', 'obstype', 'id']].to_records(index=False)
-        filename = self.cfg[package]['filename_fmt'].format(self.name)
+        filename = self.cfg[package]['mfsetup_options']['filename_fmt'].format(self.name)
         obsdata = {filename: obsdata}
 
         kwargs = self.cfg[package].copy()
         kwargs.update(self.cfg[package]['options'])
         kwargs['continuous'] = obsdata
         kwargs = get_input_arguments(kwargs, mf6.ModflowUtlobs)
         obs = mf6.ModflowUtlobs(self,  **kwargs)
@@ -726,14 +793,21 @@
         """
         Sets up the IMS package.
         """
         package = 'ims'
         print('\nSetting up {} package...'.format(package.upper()))
         t0 = time.time()
         kwargs = flatten(self.cfg[package])
+        # renames to cover difference between mf6: flopy input
+        renames = {'csv_outer_output': 'csv_outer_output_filerecord',
+                   'csv_inner_output': 'csv_outer_inner_filerecord'
+                   }
+        for k, v in renames.items():
+            if k in kwargs:
+                kwargs[v] = kwargs[k]
         kwargs = get_input_arguments(kwargs, mf6.ModflowIms)
         ims = mf6.ModflowIms(self.simulation, **kwargs)
         #self.simulation.register_ims_package(ims, [self.name])
         print("finished in {:.2f}s\n".format(time.time() - t0))
         return ims
 
     def setup_simulation_mover(self):
```

### Comparing `modflow-setup-0.2.0/mfsetup/mfmodel.py` & `modflow-setup-0.3.0/mfsetup/mfmodel.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,15 @@
     get_model_length_units,
     get_model_time_units,
     get_package_name,
 )
 from mfsetup.model_version import get_versions
 from mfsetup.sourcedata import TransientTabularSourceData, setup_array
 from mfsetup.tdis import (
+    concat_periodata_groups,
     get_parent_stress_periods,
     parse_perioddata_groups,
     setup_perioddata,
     setup_perioddata_group,
 )
 from mfsetup.tmr import Tmr
 from mfsetup.units import convert_length_units, lenuni_text, lenuni_values
@@ -238,35 +239,35 @@
 
     @property
     def bbox(self):
         if self._bbox is None and self.modelgrid is not None:
             self._bbox = self.modelgrid.bbox
         return self._bbox
 
-    @property
-    def perioddata(self):
-        """DataFrame summarizing stress period information.
-
-        Columns:
-
-          start_date_time : pandas datetimes; start date/time of each stress period
-          (does not include steady-state periods)
-          end_date_time : pandas datetimes; end date/time of each stress period
-          (does not include steady-state periods)
-          time : float; cumulative MODFLOW time (includes steady-state periods)
-          per : zero-based stress period
-          perlen : stress period length in model time units
-          nstp : number of timesteps in the stress period
-          tsmult : timestep multiplier for stress period
-          steady : True=steady-state, False=Transient
-          oc : MODFLOW-6 output control options
-        """
-        if self._perioddata is None:
-            self._set_perioddata()
-        return self._perioddata
+    #@property
+    #def perioddata(self):
+    #    """DataFrame summarizing stress period information.
+#
+    #    Columns:
+#
+    #      start_date_time : pandas datetimes; start date/time of each stress period
+    #      (does not include steady-state periods)
+    #      end_date_time : pandas datetimes; end date/time of each stress period
+    #      (does not include steady-state periods)
+    #      time : float; cumulative MODFLOW time (includes steady-state periods)
+    #      per : zero-based stress period
+    #      perlen : stress period length in model time units
+    #      nstp : number of timesteps in the stress period
+    #      tsmult : timestep multiplier for stress period
+    #      steady : True=steady-state, False=Transient
+    #      oc : MODFLOW-6 output control options
+    #    """
+    #    if self._perioddata is None:
+    #        perioddata = setup_perioddata(self)
+    #    return self._perioddata
 
     @property
     def parent(self):
         return self._parent
 
     @property
     def parent_layers(self):
@@ -355,15 +356,15 @@
         References
         ----------
         https://github.com/warner/python-versioneer
         https://github.com/warner/python-versioneer/blob/master/details.md
         """
         if self._model_version is None:
             self._model_version = get_versions(path=self.model_ws,
-                                   start_version=self.cfg['metadata']['start_version'])
+                                   start_version=str(self.cfg['metadata']['start_version']))
         return self._model_version
 
     @property
     def longname(self):
         if self._longname is None:
             longname = self.cfg['metadata'].get('longname')
             if longname is None:
@@ -994,34 +995,46 @@
 
         if mg_kwargs is not None:
             kwargs = mg_kwargs.copy()
         else:
             kwargs = {'xoff': self.parent.modelgrid.xoffset,
                       'yoff': self.parent.modelgrid.yoffset,
                       'angrot': self.parent.modelgrid.angrot,
+                      'crs': self.parent.modelgrid.crs,
                       'epsg': self.parent.modelgrid.epsg,
-                      'proj4': self.parent.modelgrid.proj4,
+                      #'proj4': self.parent.modelgrid.proj4,
                       }
         parent_units = get_model_length_units(self.parent)
         if 'lenuni' in self.cfg['parent']:
             parent_units = lenuni_text[self.cfg['parent']['lenuni']]
         elif 'length_units' in self.cfg['parent']:
             parent_units = self.cfg['parent']['length_units']
 
         if self.version == 'mf6':
             self.parent.dis.length_units = parent_units
         else:
             self.parent.dis.lenuni = lenuni_values[parent_units]
 
         # make sure crs is populated, then get CRS units for the grid
-        if kwargs.get('epsg') is not None:
-            kwargs['crs'] = pyproj.crs.CRS.from_epsg(kwargs['epsg'])
-        elif kwargs['crs'] is not None:
-            from gisutils import get_authority_crs
+        from gisutils import get_authority_crs
+        if kwargs.get('crs') is not None:
             kwargs['crs'] = get_authority_crs(kwargs['crs'])
+        elif kwargs.get('epsg') is not None:
+            kwargs['crs'] = get_authority_crs(kwargs['epsg'])
+        # no parent CRS info, assume the parent model is in the same CRS
+        elif self.cfg['setup_grid'].get('crs') is not None:
+            kwargs['crs'] = get_authority_crs(self.cfg['setup_grid']['crs'])
+        # no parent CRS info, assume the parent model is in the same CRS
+        elif self.cfg['setup_grid'].get('epsg') is not None:
+            kwargs['crs'] = get_authority_crs(self.cfg['setup_grid']['epsg'])
+        else:
+            raise ValueError('No coordinate reference input in setup_grid: or parent: '
+                             'SpatialReference: blocks of configuration file. Supply '
+                             'at least coordinate reference information to '
+                             'setup_grid: crs: item.')
 
         parent_grid_units = kwargs['crs'].axis_info[0].unit_name
 
         if 'foot' in parent_grid_units.lower() or 'feet' in parent_grid_units.lower():
             parent_grid_units = 'feet'
         elif 'metre' in parent_grid_units.lower() or 'meter' in parent_grid_units.lower():
             parent_grid_units = 'meters'
@@ -1110,28 +1123,32 @@
             # set the parent model grid from mg_kwargs if not None
             # otherwise, convert parent model grid to MFsetupGrid
             mg_kwargs = self.cfg['parent'].get('SpatialReference',
                                           self.cfg['parent'].get('modelgrid', None))
             self._set_parent_modelgrid(mg_kwargs)
 
             # setup parent model perioddata table
-            if not hasattr(self.parent, 'perioddata'):
+            if getattr(self.parent, 'perioddata', None) is None:
                 kwargs = self.cfg['parent'].copy()
-                kwargs['nper'] = self.parent.nper
                 kwargs['model_time_units'] = self.cfg['parent']['time_units']
-                if self.version == 'mf6':
+                if self.parent.version == 'mf6':
                     for var in ['perlen', 'nstp', 'tsmult']:
                         kwargs[var] = getattr(self.parent.modeltime, var)
                     kwargs['steady'] = self.parent.modeltime.steady_state
+                    kwargs['nper'] = self.parent.simulation.tdis.nper.array
                 else:
                     for var in ['perlen', 'steady', 'nstp', 'tsmult']:
                         kwargs[var] = self.parent.dis.__dict__[var].array
+                    kwargs['nper'] = self.parent.dis.nper
                 kwargs = get_input_arguments(kwargs, setup_perioddata_group)
                 kwargs['oc_saverecord'] = {}
-                self._parent.perioddata = setup_perioddata_group(**kwargs)
+                if hasattr(self.parent, '_perioddata'):
+                    self._parent._perioddata = setup_perioddata_group(**kwargs)
+                else:
+                    self._parent.perioddata = setup_perioddata_group(**kwargs)
 
             # default_source_data, where omitted configuration input is
             # obtained from parent model by default
             # Set default_source_data to True by default if it isn't specified
             if self.cfg['parent'].get('default_source_data') is None:
                 self.cfg['parent']['default_source_data'] = True
             if self.cfg['parent'].get('default_source_data'):
@@ -1188,80 +1205,14 @@
                                 if self.cfg['sto'].get('steady') is None:
                                     self.cfg['sto']['steady'] = self.parent.modeltime.steady_state[parent_periods]
                         else:
                             for var in ['perlen', 'nstp', 'tsmult', 'steady']:
                                 if self.cfg['dis'].get(var) is None:
                                     self.cfg['dis'][var] = self.parent.dis.__dict__[var].array[parent_periods]
 
-    def _set_perioddata(self):
-        """Sets up the perioddata DataFrame.
-
-        Needs some work to be more general.
-        """
-
-        if self.version == 'mf6':
-            default_start_datetime = self.cfg['tdis']['options'].get('start_date_time', '1970-01-01')
-            tdis_dimensions_config = self.cfg['tdis']['dimensions']
-            tdis_perioddata_config = self.cfg['tdis']['perioddata']
-            nper = self.cfg['tdis']['dimensions'].get('nper')
-            # steady can be input in either the tdis or sto input blocks
-            steady = self.cfg['tdis'].get('steady')
-            if steady is None:
-                steady = self.cfg['sto'].get('steady')
-        else:
-            default_start_datetime = self.cfg['dis'].get('start_date_time', '1970-01-01')
-            tdis_dimensions_config = self.cfg['dis']
-            tdis_perioddata_config = self.cfg['dis']
-            nper = self.cfg['dis'].get('nper')
-            steady = self.cfg['dis'].get('steady')
-
-        # get start_date_time from parent if available and start_date_time wasn't specified
-        if tdis_perioddata_config.get('start_date_time', '1970-01-01') == '1970-01-01' and \
-                default_start_datetime != '1970-01-01':
-            tdis_perioddata_config['start_date_time'] = default_start_datetime
-
-        # cast steady array to boolean
-        if steady is not None and not isinstance(steady, dict):
-            tdis_perioddata_config['steady'] = np.array(tdis_perioddata_config['steady']).astype(bool).tolist()
-
-        # get period data groups
-        # if no groups are specified, make a group from general stress period input
-        cfg = self.cfg
-        defaults = {'start_date_time': default_start_datetime,
-                    'nper': nper,
-                    'steady': steady,
-                    'oc_saverecord': cfg['oc'].get('saverecord', {0: ['save head last',
-                                                                      'save budget last']})
-                    }
-        perioddata_groups = parse_perioddata_groups(tdis_perioddata_config, defaults)
-
-        # set up the perioddata table from the groups
-        self._perioddata = setup_perioddata(perioddata_groups, self.time_units)
-
-        # assign parent model stress periods to each inset model stress period
-        parent_stress_periods = self.cfg.get('parent', {}).get('copy_stress_periods')
-        parent_sp = None
-        if self.parent is not None:
-            if parent_stress_periods is not None:
-                # parent_sp has parent model stress period corresponding
-                # to each inset model stress period (len=nper)
-                # the same parent stress period can be specified for multiple inset model periods
-                parent_sp = get_parent_stress_periods(self.parent, nper=self.nper,
-                                                      parent_stress_periods=parent_stress_periods)
-                self.cfg['parent']['copy_stress_periods'] = parent_sp
-            elif self._is_lgr:
-                parent_sp = self._perioddata['per'].values
-
-        # add corresponding stress periods in parent model if there are any
-        self._perioddata['parent_sp'] = parent_sp
-        assert np.array_equal(self._perioddata['per'].values, np.arange(len(self._perioddata)))
-        # reset nper property so that it will reference perioddata table
-        self._nper = None
-        self._perioddata.to_csv('{}/stress_period_data.csv'.format(self._tables_path), index=False)
-
     def _setup_array(self, package, var, vmin=-1e30, vmax=1e30,
                       source_model=None, source_package=None,
                       **kwargs):
         return setup_array(self, package, var, vmin=vmin, vmax=vmax,
                            source_model=source_model, source_package=source_package,
                            **kwargs)
```

### Comparing `modflow-setup-0.2.0/mfsetup/mfnwt_defaults.yml` & `modflow-setup-0.3.0/mfsetup/mfnwt_defaults.yml`

 * *Files 8% similar despite different names*

```diff
@@ -112,35 +112,41 @@
 drn:
   options:
   source_data:
     shapefile:
       all_touched: True
     elev:
       stat: 'min'
+    cond:
+      stat: 'mean'
   mfsetup_options:
     external_files: True  # option to write stress_period_data to external files
     external_filename_fmt: "drn_{:03d}.dat"
 
 ghb:
   options:
   source_data:
     shapefile:
       all_touched: True
     bhead:
       stat: 'min'
+    cond:
+      stat: 'mean'
   mfsetup_options:
     external_files: False  # option to write stress_period_data to external files
     external_filename_fmt: "ghb_{:03d}.dat"
 
 riv:
   source_data:
     shapefile:
       all_touched: True
     stage:
       stat: 'min'
+    cond:
+      stat: 'mean'
   output_files:
     rivdata_file: '{}_rivdata.csv' # table with auxillary information on river reaches (routing, source hydrography IDs, etc.)
   mfsetup_options:
     default_rbot_thickness: 1.
     external_files: True  # option to write stress_period_data to external files
     external_filename_fmt: "riv_{:03d}.dat"
 
@@ -167,20 +173,22 @@
   budget_fileout_fmt: '{}.cbc'
   period_options: {0: ['save head last',
                        'save budget last']
   }
 
 hyd:
   hydnoh: -999
-  default_columns:
-    x_location_col: 'x_utm' # x coordinates in wtm
-    y_location_col: 'y_utm' # y coordinates in wtm
   source_data:
     column_mappings:
       hydlbl: ['obsprefix', 'obsnme', 'common_name']
+    x_location_col: 'x' # x coordinates in wtm
+    y_location_col: 'y' # y coordinates in wtm
+  mfsetup_options:
+    allow_obs_in_bc_cells: False
+    obsname_character_limit: 14  # hydmod limit
 
 gag:
   starting_unit_number: 250
   lak_outtype: 1 # see gage package documentation for Data Set 2a outtype
   sfr_outtype: 0 # see gage package documentation for Data Set 2b outtype
   column_mappings:
     x_location_col: ['x_utm', 'X']
```

### Comparing `modflow-setup-0.2.0/mfsetup/mfnwtmodel.py` & `modflow-setup-0.3.0/mfsetup/mfnwtmodel.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,19 @@
     setup_lake_fluxes,
     setup_lake_info,
     setup_lake_tablefiles,
 )
 from mfsetup.mfmodel import MFsetupMixin
 from mfsetup.obs import setup_head_observations
 from mfsetup.oc import parse_oc_period_input
-from mfsetup.tdis import get_parent_stress_periods, setup_perioddata_group
+from mfsetup.tdis import (
+    get_parent_stress_periods,
+    setup_perioddata,
+    setup_perioddata_group,
+)
 from mfsetup.units import convert_length_units, itmuni_text, lenuni_text
 from mfsetup.utils import get_input_arguments, get_packages
 
 
 class MFnwtModel(MFsetupMixin, Modflow):
     """Class representing a MODFLOW-NWT model"""
     default_file = '/mfnwt_defaults.yml'
@@ -106,14 +110,61 @@
         return lenuni_text[self.cfg['dis']['lenuni']]
 
     @property
     def time_units(self):
         return itmuni_text[self.cfg['dis']['itmuni']]
 
     @property
+    def perioddata(self):
+        """DataFrame summarizing stress period information.
+        Columns:
+        ============== =========================================
+        start_datetime Start date of each model stress period
+        end_datetime   End date of each model stress period
+        time           MODFLOW elapsed time, in days*
+        per            Model stress period number
+        perlen         Stress period length (days)
+        nstp           Number of timesteps in stress period
+        tsmult         Timestep multiplier
+        steady         Steady-state or transient
+        oc             Output control setting for MODFLOW
+        parent_sp      Corresponding parent model stress period
+        ============== =========================================
+
+        TODO: the code here might still need to be adapted to
+        parallel the code in MF6model.perioddata, to work with
+        parent models that are already loaded but have no configuration.
+        """
+        if self._perioddata is None:
+            default_start_datetime = self.cfg['dis'].get('start_date_time', '1970-01-01')
+            tdis_perioddata_config = self.cfg['dis']
+            nper = self.cfg['dis'].get('nper')
+            steady = self.cfg['dis'].get('steady')
+            parent_stress_periods=None
+            if self.parent is not None:
+                parent_stress_periods = self.cfg['parent'].get('copy_stress_periods')
+            perioddata = setup_perioddata(
+                    self,
+                    tdis_perioddata_config=tdis_perioddata_config,
+                    default_start_datetime=default_start_datetime,
+                    nper=nper, steady=steady, time_units=self.time_units,
+                    parent_model=self.parent,
+                    parent_stress_periods=parent_stress_periods,
+                    )
+            self._perioddata = perioddata
+            # reset nper property so that it will reference perioddata table
+            self._nper = None
+            self._perioddata.to_csv(f'{self._tables_path}/stress_period_data.csv', index=False)
+            # update the model configuration
+            if 'parent_sp' in perioddata.columns:
+                self.cfg['parent']['copy_stress_periods'] = perioddata['parent_sp'].tolist()
+
+        return self._perioddata
+
+    @property
     def ipakcb(self):
         """By default write everything to one cell budget file."""
         return self.cfg['upw'].get('ipakcb', 53)
 
     @property
     def ibound(self):
         """3D array indicating which cells will be included in the simulation.
@@ -289,15 +340,15 @@
         print("finished in {:.2f}s\n".format(time.time() - t0))
         return dis
 
     def setup_tdis(self, **kwargs):
         """Calls the _set_perioddata, to establish time discretization. Only purpose
         is to conform to same syntax as mf6 for MFsetupMixin.setup_from_yaml()
         """
-        self._set_perioddata()
+        self.perioddata
 
     def setup_bas6(self, **kwargs):
         """"""
         package = 'bas6'
         print('\nSetting up {} package...'.format(package.upper()))
         t0 = time.time()
 
@@ -659,17 +710,30 @@
 
     def setup_hyd(self, **kwargs):
         """TODO: generalize hydmod setup with specific input requirements"""
         package = 'hyd'
         print('setting up HYDMOD package...')
         t0 = time.time()
 
-        # munge the head observation data
-        df = setup_head_observations(self, format=package,
-                                     obsname_column='hydlbl')
+        iobs_domain = None
+        if not kwargs['mfsetup_options']['allow_obs_in_bc_cells']:
+            # for now, discard any head observations in same (i, j) column of cells
+            # as a non-well boundary condition
+            # including lake package lakes and non lake, non well BCs
+            # (high-K lakes are excluded, since we may want head obs at those locations,
+            #  to serve as pseudo lake stage observations)
+            iobs_domain = (self.isbc == 1) | np.any(self.isbc > 2)
+
+        # munge the observation data
+        df = setup_head_observations(self,
+                                     obs_package=package,
+                                     obsname_column='hydlbl',
+                                     iobs_domain=iobs_domain,
+                                     **kwargs['source_data'],
+                                     **kwargs['mfsetup_options'])
 
         # create observation data recarray
         obsdata = fm.ModflowHyd.get_empty(len(df))
         for c in obsdata.dtype.names:
             assert c in df.columns, "Missing observation data field: {}".format(c)
             obsdata[c] = df[c]
         nhyd = len(df)
```

### Comparing `modflow-setup-0.2.0/mfsetup/model_version.py` & `modflow-setup-0.3.0/mfsetup/model_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     The ".dev0" means dirty. Note that .dev0 sorts backwards
     (a dirty tree will appear "older" than the corresponding clean one),
     but you shouldn't be releasing software with -dirty anyways.
 
     Exceptions:
     1: no tags. 0.postDISTANCE[.dev0]
     """
-    if pieces["closest-tag"]:
+    if pieces["closest-tag"] and str(start_version) == '0':
         rendered = pieces["closest-tag"]
         if pieces["distance"] or pieces["dirty"]:
             rendered += ".post%d" % pieces["distance"]
             if pieces["dirty"]:
                 rendered += ".dev0"
             rendered += plus_or_dot(pieces)
             rendered += "g%s" % pieces["short"]
```

### Comparing `modflow-setup-0.2.0/mfsetup/mover.py` & `modflow-setup-0.3.0/mfsetup/mover.py`

 * *Files identical despite different names*

### Comparing `modflow-setup-0.2.0/mfsetup/obs.py` & `modflow-setup-0.3.0/mfsetup/obs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 import pandas as pd
-from shapely.geometry import Point
+from shapely.geometry import Point, box
 
 from mfsetup.fileio import check_source_files
 from mfsetup.grid import get_ij
 
 
 def read_observation_data(f=None, column_info=None,
                           column_mappings=None):
@@ -46,49 +46,52 @@
     obsname_cols = ['obsname', 'hydlbl']
     for c in obsname_cols:
         if c in df.columns:
             df[c] = df[c].astype(str)
     return df
 
 
-def setup_head_observations(model, obs_info_files=None,
-                            format='hyd',
-                            obsname_column='obsname'):
-
-    self = model
-    package = format
-    source_data_config = self.cfg[package]['source_data']
+def setup_head_observations(model, filenames=None,
+                            obs_package='hyd', column_mappings=None,
+                            obsname_column='obsname',
+                            x_location_col='x',
+                            y_location_col='y',
+                            obsname_character_limit=40,
+                            drop_observations=None, iobs_domain=None,
+                            **kwargs):
 
     # set a 14 character obsname limit for the hydmod package
     # https://water.usgs.gov/ogw/modflow-nwt/MODFLOW-NWT-Guide/index.html?hyd.htm
     # 40 character limit for MODFLOW-6 (see IO doc)
-    obsname_character_limit = 40
-    if format == 'hyd':
-        obsname_character_limit = 14
+
 
     # TODO: read head observation data using TabularSourceData instead
-    if obs_info_files is None:
-        for key in 'filename', 'filenames':
-            if key in source_data_config:
-                obs_info_files = source_data_config[key]
-        if obs_info_files is None:
+    if filenames is None:
+        filenames = kwargs.get('filename')
+        if filenames is None:
             print("No data for the Observation (OBS) utility.")
             return
+    obs_info_files = filenames
 
     # get obs_info_files into dictionary format
     # filename: dict of column names mappings
+    default_inputs = {
+            'x_location_col': x_location_col,
+            'y_location_col': y_location_col,
+        }
+
     if isinstance(obs_info_files, str):
         obs_info_files = [obs_info_files]
     if isinstance(obs_info_files, list):
-        obs_info_files = {f: self.cfg[package]['default_columns']
+        obs_info_files = {f: default_inputs
                           for f in obs_info_files}
     elif isinstance(obs_info_files, dict):
         for k, v in obs_info_files.items():
             if v is None:
-                obs_info_files[k] = self.cfg[package]['default_columns']
+                obs_info_files[k] = default_inputs
 
     check_source_files(obs_info_files.keys())
     # dictionaries mapping from obstypes to hydmod input
     pckg = {'LK': 'BAS',  # head package for high-K lakes; lake package lakes get dropped
             'GW': 'BAS',
             'head': 'BAS',
             'lake': 'BAS',
@@ -100,15 +103,14 @@
            'ST': 'SO',
            'flux': 'SO'
            }
     print('Reading observation files...')
     dfs = []
     for f, column_info in obs_info_files.items():
         print(f)
-        column_mappings = self.cfg[package]['source_data'].get('column_mappings')
         df = read_observation_data(f, column_info,
                                    column_mappings=column_mappings)
         if 'obs_type' in df.columns and 'pckg' not in df.columns:
             df['pckg'] = [pckg.get(s, 'BAS') for s in df['obs_type']]
         elif 'pckg' not in df.columns:
             df['pckg'] = 'BAS'  # default to getting heads
         if 'obs_type' in df.columns and 'intyp' not in df.columns:
@@ -119,39 +121,19 @@
         df[obsname_column] = df[obsname_column].astype(str).str.lower()
 
         dfs.append(df[['pckg', 'arr', 'intyp', 'x', 'y', obsname_column, 'file']])
     df = pd.concat(dfs, axis=0)
 
     print('\nCulling observations to model area...')
     df['geometry'] = [Point(x, y) for x, y in zip(df.x, df.y)]
-    within = [g.within(self.bbox) for g in df.geometry]
+    l, r, t, b = model.modelgrid.extent
+    bbox = box(l, b, r, t)
+    within = [g.within(bbox) for g in df.geometry]
     df = df.loc[within].copy()
 
-    print('Dropping head observations that coincide with boundary conditions...')
-    i, j = get_ij(self.modelgrid, df.x.values, df.y.values)
-    df['i'], df['j'] = i, j
-
-    #islak = self.lakarr[0, i, j] != 0
-    # for now, discard any head observations in same (i, j) column of cells
-    # as a non-well boundary condition
-    # lake package lakes
-    has_lak = np.any(self.isbc[:, i, j] == 1, axis=0)
-    # non lake, non well BCs
-    # (high-K lakes are excluded, since we may want head obs at those locations,
-    #  to serve as pseudo lake stage observations)
-    has_bc = has_lak | np.any(self.isbc[:, i, j] > 2, axis=0)
-    if any(has_bc):
-        print(f'dropped {np.sum(has_bc)} of {len(df)} observations in cells with bcs.')
-    df = df.loc[~has_bc].copy()
-
-    drop_obs = self.cfg[package].get('drop_observations', [])
-    if len(drop_obs) > 0:
-        print('Dropping head observations specified in {}...'.format(self.cfg.get('filename', 'config file')))
-        df = df.loc[~df[obsname_column].astype(str).isin(drop_obs)]
-
     # make unique observation names for each model layer; applying the character limit
     # preserve end of obsname, truncating initial characters as needed
     # (for observations based on lat-lon coordinates such as usgs, or other naming schemes
     #  where names share leading characters)
     prefix_character_limit = obsname_character_limit  # - 2
     df[obsname_column] = [obsname[-prefix_character_limit:] for obsname in df[obsname_column]]
     duplicated = df[obsname_column].duplicated(keep=False)
@@ -162,35 +144,50 @@
         print(df.loc[duplicated, [obsname_column, 'file']])
 
     # make sure every head observation is in each layer
     non_heads = df.loc[df.arr != 'HD'].copy()
     heads = df.loc[df.arr == 'HD'].copy()
     heads0 = heads.groupby(obsname_column).first().reset_index()
     heads0[obsname_column] = heads0[obsname_column].astype(str)
-    heads_all_layers = pd.concat([heads0] * self.nlay).sort_values(by=obsname_column)
-    heads_all_layers['klay'] = list(range(self.nlay)) * len(heads0)
+    heads_all_layers = pd.concat([heads0] * model.modelgrid.nlay).sort_values(by=obsname_column)
+    heads_all_layers['klay'] = list(range(model.modelgrid.nlay)) * len(heads0)
     heads_all_layers[obsname_column] = ['{}'.format(obsname)  # _{:.0f}'.format(obsname, k)
                                         for obsname, k in zip(heads_all_layers[obsname_column],
                                                               heads_all_layers['klay'])]
     df = pd.concat([heads_all_layers, non_heads], axis=0)
 
     # dtypes
     assert df[obsname_column].dtype == object
     df['klay'] = df.klay.astype(int)
 
-    if format == 'hyd':
+    print('Culling observations to cells allowed by iobs_domain...')
+    i, j = get_ij(model.modelgrid, df.x.values, df.y.values)
+    df['i'], df['j'] = i, j
+
+    keep = np.array([True] * len(df))
+    if iobs_domain is not None:
+        keep = np.ravel(iobs_domain[df['klay'].values, i, j] > 0)
+    if np.any(~keep):
+        print(f'dropped {np.sum(~keep)} of {len(df)} observations in cells with bcs.')
+        df = df.loc[keep].copy()
+
+    if drop_observations is not None:
+        print('Dropping head observations specified in drop_observations...')
+        df = df.loc[~df[obsname_column].astype(str).isin(drop_observations)]
+
+    if obs_package == 'hyd':
         # get model locations
-        xl, yl = self.modelgrid.get_local_coords(df.x.values, df.y.values)
+        xl, yl = model.modelgrid.get_local_coords(df.x.values, df.y.values)
         df['xl'] = xl
         df['yl'] = yl
         # drop observations located in inactive cels
         ibdn = model.bas6.ibound.array[df.klay.values, df.i.values, df.j.values]
         active = ibdn >= 1
         df.drop(['i', 'j'], axis=1, inplace=True)
-    elif format == 'obs':  # mf6 observation utility
+    elif obs_package == 'obs':  # mf6 observation utility
         obstype = {'BAS': 'HEAD'}
         renames = {'pckg': 'obstype'}
         df.pckg.replace(obstype, inplace=True)
         df.rename(columns=renames, inplace=True)
         df['id'] = list(zip(df.klay, df.i, df.j))
         # drop observations located in inactive cels
         idm = model.idomain[df.klay.values, df.i.values, df.j.values]
```

### Comparing `modflow-setup-0.2.0/mfsetup/oc.py` & `modflow-setup-0.3.0/mfsetup/oc.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     -------
     flopy_input : dict
         Input to the flopy output control package constructor.
 
     Examples
     --------
     >>> period_input = {'saverecord': {0: {'head': 'last', 'budget': 'last'}}
+    >>> parse_oc_period_input(period_input)
     {0: [('head', 'last'), ('budget', 'last')]}
     """
     if nstp is not None:
         nstp = list(nstp)
         nper = len(nstp)
 
     flopy_input = {}
```

### Comparing `modflow-setup-0.2.0/mfsetup/sourcedata.py` & `modflow-setup-0.3.0/mfsetup/sourcedata.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 import os
 import shutil
 import warnings
 from pathlib import Path
 
 import numpy as np
 import pandas as pd
+import pyproj
 from flopy.utils import binaryfile as bf
-from gisutils import get_values_at_points, shp2df
+from gisutils import get_values_at_points, project, shp2df
 from scipy.interpolate import griddata
 from shapely.geometry import Point
 
 import xarray as xr
 from mfsetup.discretization import (
     fill_cells_vertically,
     fill_empty_layers,
@@ -37,14 +38,15 @@
 )
 from mfsetup.units import convert_length_units, convert_time_units, convert_volume_units
 from mfsetup.utils import get_input_arguments
 
 renames = {'mult': 'multiplier',
            'elevation_units': 'length_units',
            'from_parent': 'from_source_model_layers',
+           'data_column': 'data_columns'
            }
 
 
 class SourceData:
     """Class for handling source_data specified in config file.
 
     Parameters
@@ -613,15 +615,15 @@
             results[inset_kper] = period_mean2d
         self.data = results
         return results
 
 
 class NetCDFSourceData(ArraySourceData, TransientSourceDataMixin):
     def __init__(self, filenames, variable, period_stats,
-                 length_units='unknown', time_units='days',
+                 length_units='unknown', time_units='days', crs=None,
                  dest_model=None, source_modelgrid=None,
                  from_source_model_layers=None, datatype='transient2d',
                  resample_method='nearest', vmin=-1e30, vmax=1e30
                  ):
 
         ArraySourceData.__init__(self, variable=None,
                                  length_units=length_units, time_units=time_units,
@@ -640,33 +642,78 @@
         else:
             self.filename = filenames
         self.variable = variable
         self.resample_method = resample_method
         self.dest_model = dest_model
         self.time_col = 'time'
 
+        self._crs = None
+        self._specified_crs = crs
+
         # set xy value arrays for source and dest. grids
         with xr.open_dataset(self.filename) as ds:
             x1, y1 = np.meshgrid(ds.x.values, ds.y.values)
             x1 = x1.ravel()
             y1 = y1.ravel()
+            # reproject the netcdf coords
+            # to the model CRS
+            if self.crs is not None:
+                if self.crs != self.dest_model.modelgrid.crs:
+                    x1, y1 = project((x1, y1),
+                                     self.crs,
+                                     self.dest_model.modelgrid.crs)
             self.source_grid_xy = np.array([x1, y1]).transpose()
         x2 = self.dest_model.modelgrid.xcellcenters.ravel()
         y2 = self.dest_model.modelgrid.ycellcenters.ravel()
         self.dest_grid_xy = np.array([x2, y2]).transpose()
 
     @property
     def interp_weights(self):
         """For a given parent, only calculate interpolation weights
         once to speed up re-gridding of arrays to pfl_nwt."""
         if self._interp_weights is None:
             self._interp_weights = interp_weights(self.source_grid_xy,
                                                   self.dest_grid_xy)
         return self._interp_weights
 
+    @property
+    def crs(self):
+        """Try to make a valid pyproj.CRS instance from
+        coordinate reference system information in the
+        NetCDF file. Assumes that CF-like grid_mapping
+        information is stored in a 'crs' variable.
+
+        """
+        specified_crs = None
+        ncfile_crs = None
+        if self._specified_crs is not None:
+            specified_crs = pyproj.CRS(self._specified_crs)
+            self._specified_crs = specified_crs
+        if self._crs is None:
+            with xr.open_dataset(self.filename) as ds:
+                crs_da = getattr(ds, 'crs', None)
+            if crs_da is not None:
+                grid_mapping = crs_da.attrs
+                ncfile_crs = self.get_crs_from_grid_mapping(grid_mapping)
+            if specified_crs is None:
+                if ncfile_crs is None:
+                    print('Could not create valid pyproj.CRS object'
+                         f'from grid mapping infromation in {self.filename} '
+                         f'Input in {self.filename} will be assumed to be in the '
+                          'model coordinate reference system.')
+                else:
+                    self._crs = ncfile_crs
+            elif (ncfile_crs is None) or (specified_crs == ncfile_crs):
+                self._crs = specified_crs
+            else:
+                raise ValueError(f'Specified CRS is different than CRS in NetCDF file; check for consistency.\n'
+                                 '{specified_crs}\n!=\n{ncfile_crs}')
+
+        return self._crs
+
     def regrid_from_source(self, source_array,
                            method='linear'):
         """Interpolate values in source array onto
         the destination model grid, using SpatialReference instances
         attached to the source and destination models.
 
         Parameters
@@ -696,26 +743,47 @@
 
         # sample values to model stress periods
         results = {}
         for kper, period_stat in self.period_stats.items():
             if period_stat is None:
                 continue
             aggregated = aggregate_xarray_to_stress_period(data,
-                                                           datetime_column=self.time_col,
+                                                           datetime_coords_name=self.time_col,
                                                            **period_stat)
             # sample the data onto the model grid
             resampled = self.regrid_from_source(aggregated,
                                                 method=self.resample_method)
             # reshape results to model grid
             period_mean2d = resampled.reshape(self.dest_model.nrow,
                                               self.dest_model.ncol)
             results[kper] = period_mean2d * self.unit_conversion
         self.data = results
         return results
 
+    @staticmethod
+    def get_crs_from_grid_mapping(grid_mapping):
+        crs = None
+        try:
+            crs = pyproj.CRS.from_cf(grid_mapping)
+        except:
+            pass
+        if 'crs_wkt' in grid_mapping:
+            try:
+                crs = pyproj.CRS(grid_mapping['crs_wkt'])
+            except:
+                pass
+        # Soil Water Balance Code output
+        # usually has a "proj4_string" entry
+        if 'proj4_string' in grid_mapping:
+            try:
+                crs = pyproj.CRS(grid_mapping['proj4_string'])
+            except:
+                pass
+        # could add more crazy try/excepts here
+        return crs
 
 class MFBinaryArraySourceData(ArraySourceData):
     """Subclass for handling MODFLOW binary array data
     that may come from another model."""
     def __init__(self, variable, filename=None,
                  length_units='unknown', time_units='unknown',
                  dest_model=None, source_modelgrid=None,
@@ -968,26 +1036,27 @@
         return df.reset_index(drop=True)
 
 
 class TransientTabularSourceData(SourceData, TransientSourceDataMixin):
     """Subclass for handling tabular source data that
     represents a time series."""
 
-    def __init__(self, filenames, data_column, datetime_column, id_column,
+    def __init__(self, filenames, data_columns, datetime_column, id_column,
                  x_col='x', y_col='y', end_datetime_column=None, period_stats={0: 'mean'},
                  length_units='unknown', time_units='unknown', volume_units=None,
                  column_mappings=None, category_column=None,
-                 dest_model=None, resolve_duplicates_with='raise error'):
+                 dest_model=None, resolve_duplicates_with='raise error', **kwargs):
         SourceData.__init__(self, filenames=filenames,
                             length_units=length_units, time_units=time_units,
                             volume_units=volume_units,
                             dest_model=dest_model)
         TransientSourceDataMixin.__init__(self, period_stats=period_stats, dest_model=dest_model)
-
-        self.data_column = data_column
+        if isinstance(data_columns, str):
+            data_columns = [data_columns]
+        self.data_columns = data_columns
         self.datetime_column = datetime_column
         self.end_datetime_column = end_datetime_column
         self.id_column = id_column
         self.column_mappings = column_mappings
         self.category_column = category_column
         self.time_col = datetime_column
         self.x_col = x_col
@@ -1042,24 +1111,25 @@
         period_data = []
         for kper, period_stat in self.period_stats.items():
             if period_stat is None:
                 continue
             aggregated = aggregate_dataframe_to_stress_period(df, id_column=self.id_column,
                                                               datetime_column=self.datetime_column,
                                                               end_datetime_column=self.end_datetime_column,
-                                                              data_column=self.data_column,
+                                                              data_column=self.data_columns,
                                                               category_column=self.category_column,
                                                               resolve_duplicates_with=self.resolve_duplicates_with,
                                                               **period_stat)
             aggregated['per'] = kper
             period_data.append(aggregated)
         dfm = pd.concat(period_data)
 
-        if self.data_column is not None:
-            dfm[self.data_column] *= self.unit_conversion
+        if self.data_columns is not None:
+            for col in self.data_columns:
+                dfm[col] *= self.unit_conversion
         dfm.sort_values(by=['per', self.id_column], inplace=True)
 
         # drop any extra unnamed columns from accidental saving of the index on to_csv
         drop_columns = [c for c in dfm.columns if 'unnamed' in c]
         dfm.drop(drop_columns, axis=1, inplace=True)
 
         # map x, y locations to modelgrid
```

### Comparing `modflow-setup-0.2.0/mfsetup/tdis.py` & `modflow-setup-0.3.0/mfsetup/tdis.py`

 * *Files 11% similar despite different names*

```diff
@@ -77,20 +77,24 @@
         parent_sp = [0]
         for i in range(nper - 1):
             parent_sp.append(parent_sp[-1])
     assert len(parent_sp) == nper
     return parent_sp
 
 
-def parse_perioddata_groups(perioddata_dict, defaults={}):
+def parse_perioddata_groups(perioddata_dict,
+                            **kwargs):
     """Reorganize input in perioddata dict into
     a list of groups (dicts).
     """
-    #perioddata = perioddata_dict.copy()
     perioddata_groups = []
+    defaults = {
+        'start_date_time': '1970-01-01'
+    }
+    defaults.update(kwargs)
     group0 = defaults.copy()
 
     valid_txt = "if transient: perlen specified or 3 of start_date_time, " \
                 "end_date_time, nper or freq;\n" \
                 "if steady: nper or perlen specified. Default perlen " \
                 "for steady-state periods is 1."
     for k, v in perioddata_dict.items():
@@ -101,27 +105,27 @@
                 data = get_input_arguments(data, setup_perioddata_group)
                 perioddata_groups.append(data)
             else:
                 print_item(k, data)
                 prefix = "perioddata input for {} must have".format(k)
                 raise Exception(prefix + valid_txt)
         elif 'perioddata' in k.lower():
-            perioddata_groups += parse_perioddata_groups(perioddata_dict[k], defaults=defaults)
+            perioddata_groups += parse_perioddata_groups(perioddata_dict[k], **defaults)
         else:
             group0[k] = v
     if len(perioddata_groups) == 0:
         if not is_valid_perioddata(group0):
             print_item('perioddata:', group0)
             prefix = "perioddata input must have"
             raise Exception(prefix + valid_txt)
         data = get_input_arguments(group0, setup_perioddata_group)
         perioddata_groups = [data]
     for group in perioddata_groups:
         if 'steady' in group:
-            if np.isscalar(group['steady']):
+            if np.isscalar(group['steady']) or group['steady'] is None:
                 group['steady'] = {0: group['steady']}
             elif not isinstance(group['steady'], dict):
                 group['steady'] = {i: s for i, s in enumerate(group['steady'])}
     return perioddata_groups
 
 
 def setup_perioddata_group(start_date_time, end_date_time=None,
@@ -365,56 +369,159 @@
 
     # specify steady-state or transient for each period, filling empty
     # periods with previous state (same logic as MF6 input)
     issteady = [steady[0]]
     for i in range(len(perioddata)):
         issteady.append(steady.get(i, issteady[i]))
     perioddata['steady'] = issteady[1:]
+    perioddata['steady'] = perioddata['steady'].astype(bool)
 
     # set up output control, using previous value to fill empty periods
     # (same as MF6)
     oclist = [None]
     for i in range(len(perioddata)):
         oclist.append(oc.get(i, oclist[i]))
     perioddata['oc'] = oclist[1:]
 
     # correct nstp and tsmult to be 1 for steady-state periods
-    perioddata.loc[perioddata.steady, 'nstp'] = 1
-    perioddata.loc[perioddata.steady, 'tsmult'] = 1
+    perioddata.loc[perioddata.steady.values, 'nstp'] = 1
+    perioddata.loc[perioddata.steady.values, 'tsmult'] = 1
     return perioddata
 
 
-def setup_perioddata(perioddata_groups, time_units='days'):
+def concat_periodata_groups(perioddata_groups, time_units='days'):
+    """Concatenate multiple perioddata DataFrames, but sort
+    result on (absolute) datetimes and increment model time and stress period
+    numbers accordingly."""
 
     # update any missing variables in the groups with global variables
     group_dfs = []
     for i, group in enumerate(perioddata_groups):
         group.update({'model_time_units': time_units,
                       })
         df = setup_perioddata_group(**group)
         group_dfs.append(df)
 
-    # concatenate groups into single dataframe of perioddata
-    perioddata = concat_periodata_groups(group_dfs)
-    return perioddata
-
-
-def concat_periodata_groups(groups):
-    """Concatenate multiple perioddata DataFrames, but sort
-    result on (absolute) datetimes and increment model time and stress period
-    numbers accordingly."""
-    df = pd.concat(groups).sort_values(by=['end_datetime'])
+    df = pd.concat(group_dfs).sort_values(by=['end_datetime'])
     perlen = np.ones(len(df))
     perlen[~df.steady.values] = df.loc[~df.steady.values, 'perlen']
     df['time'] = np.cumsum(perlen)
     df['per'] = range(len(df))
     df.index = range(len(df))
     return df
 
 
+def setup_perioddata(model,
+                     tdis_perioddata_config,
+                     default_start_datetime=None,
+                     nper=None,
+                     steady=None, time_units='days',
+                     oc_saverecord=None, parent_model=None,
+                     parent_stress_periods=None,
+                     ):
+    """Sets up the perioddata DataFrame that is used to reference model
+    stress period start and end times to real date time.
+
+    Parameters
+    ----------
+    model : _type_
+        _description_
+    tdis_perioddata_config : dict
+        ``perioddata:``, ``tdis:`` (MODFLOW 6 models) or ``dis:`` (MODFLOW-2005 models)
+        block from the Modflow-setup configuration file.
+    default_start_datetime : str, optional
+        Start date for model from the tdis: options: block in the configuration file,
+        or ``model.modeltime.start_datetime`` Flopy attribute. Only used
+        where start_datetime information is missing, for example if a group
+        for an initial steady-state period in ``tdis_perioddata_config``
+        doesn't have a start_datetime: entry. By default, None, in which case
+        the default start_datetime of 1970-01-01 may be applied by
+        py:func:`setup_perioddata_group`.
+    nper : int, optional
+        Number of stress periods. Only used if nper is specified in the
+        tdis: dimensions: block of the configuration file and
+        not in a perioddata group.
+    steady : bool, sequence or dict
+        Whether each period is steady-state or transient. Only used
+        if steady is specified in the tdis: or sto: configuration file
+        blocks (MODFLOW 6 models) or the dis: block (MODFLOW-2005 models),
+        and not in perioddata groups.
+    time_units : str, optional
+        Model time units, by default 'days'.
+    oc_saverecord : dict, optional
+        Output control settings, keyed by stress period. Only
+        used to record this information in the stress period data table.
+    parent_model : flopy model instance, optional
+        Parent model, if model is an inset.
+    parent_stress_periods : list of ints, optional
+        Parent model stress periods to apply to the inset model
+        (read from the parent: copy_stress_periods: item in the
+        configuration file).
+
+    Returns
+    -------
+    perioddata : DataFrame
+        Table of stress period information with columns:
+
+        ============== =========================================
+        start_datetime Start date of each model stress period
+        end_datetime   End date of each model stress period
+        time           MODFLOW elapsed time, in days [#f1]_
+        per            Model stress period number
+        perlen         Stress period length (days)
+        nstp           Number of timesteps in stress period
+        tsmult         Timestep multiplier
+        steady         Steady-state or transient
+        oc             Output control setting for MODFLOW
+        parent_sp      Corresponding parent model stress period
+        ============== =========================================
+
+    Notes
+    -----
+    perioddata is also saved to stress_period_data.csv in the tables folder
+    (usually `/tables`).
+
+    .. rubric:: Footnotes
+
+    .. [#f1] Modflow elapsed time includes the time lengths specified for
+        any steady-state periods (at least 1 day). Therefore if the model
+        has an initial steady-state period with a ``perlen`` of one day,
+        the elapsed time at the model start date will already be 1 day.
+    """
+    # get start_date_time from parent if available and start_date_time wasn't specified
+    # only apply to tdis_perioddata_config if it wasn't specified there
+    if tdis_perioddata_config.get('start_datetime', '1970-01-01') == '1970-01-01' and \
+            default_start_datetime != '1970-01-01':
+        tdis_perioddata_config['start_date_time'] = default_start_datetime
+
+    perioddata_groups = parse_perioddata_groups(tdis_perioddata_config,
+                                                nper=nper, steady=steady,
+                                                start_date_time=default_start_datetime)
+
+    # set up the perioddata table from the groups
+    perioddata = concat_periodata_groups(perioddata_groups, time_units)
+
+    # assign parent model stress periods to each inset model stress period
+    parent_sp = None
+    if parent_model is not None:
+        if parent_stress_periods is not None:
+            # parent_sp has parent model stress period corresponding
+            # to each inset model stress period (len=nper)
+            # the same parent stress period can be specified for multiple inset model periods
+            parent_sp = get_parent_stress_periods(parent_model, nper=len(perioddata),
+                                                    parent_stress_periods=parent_stress_periods)
+        elif model._is_lgr:
+            parent_sp = perioddata['per'].values
+
+        # add corresponding stress periods in parent model if there are any
+        perioddata['parent_sp'] = parent_sp
+    assert np.array_equal(perioddata['per'].values, np.arange(len(perioddata)))
+    return perioddata
+
+
 def aggregate_dataframe_to_stress_period(data, id_column, data_column, datetime_column='datetime',
                                          end_datetime_column=None, category_column=None,
                                          start_datetime=None, end_datetime=None, period_stat='mean',
                                          resolve_duplicates_with='raise error'):
     """Aggregate time-series data in a DataFrame to a single value representing
     a period defined by a start and end date.
 
@@ -570,27 +677,29 @@
     # ensure that ids are unique in each time period
     # by summing multiple id instances by period
     # (only sum the data column)
     # check for duplicates with same time, id, and category (measured vs estimated)
     duplicated = pd.Series(list(zip(period_data[datetime_column],
                                     period_data[id_column],
                                     period_data[category_column]))).duplicated()
-    # if len(period_data) > 0:
-    if any(duplicated):
-        if resolve_duplicates_with == 'raise error':
-            duplicate_info = period_data.loc[duplicated.values]
-            msg = 'The following locations are duplicates which need to be resolved:\n'.format(duplicate_info.__str__())
-            raise ValueError(msg)
-        period_data.index.name = None
-        by_period = period_data.groupby([id_column, datetime_column]).first().reset_index()
-        by_period[data_column] = getattr(period_data.groupby([id_column, datetime_column]),
-                                            resolve_duplicates_with)()[data_column].values
-        period_data = by_period
     aggregated = period_data.groupby(id_column).first()
-    aggregated[data_column] = getattr(period_data.groupby(id_column), stat)()[data_column].values
+    for data_column in data_columns:
+        if any(duplicated):
+            if resolve_duplicates_with == 'raise error':
+                duplicate_info = period_data.loc[duplicated.values]
+                msg = 'The following locations are duplicates which need to be resolved:\n'.format(duplicate_info.__str__())
+                raise ValueError(msg)
+            period_data.index.name = None
+            by_period = period_data.groupby([id_column, datetime_column]).first().reset_index()
+            agg_groupedby = getattr(period_data.groupby([id_column, datetime_column]),
+                                    resolve_duplicates_with)(numeric_only=True)
+            by_period[data_column] = agg_groupedby[data_column].values
+            period_data = by_period
+        agg_groupedby = getattr(period_data.groupby(id_column), stat)(numeric_only=True)
+        aggregated[data_column] = agg_groupedby[data_column].values
     # if category column was argued, get counts of measured vs estimated
     # for each measurement location, for current stress period
     if categories:
         counts = period_data.groupby([id_column, category_column]).size().unstack(fill_value=0)
         for col in 'measured', 'estimated':
             if col not in counts.columns:
                 counts[col] = 0
@@ -604,16 +713,17 @@
     drop_cols = [datetime_column]
     if not categories:  # drop category column if it was created
         drop_cols.append(category_column)
     aggregated.drop(drop_cols, axis=1, inplace=True)
     return aggregated
 
 
-def aggregate_xarray_to_stress_period(data, start_datetime, end_datetime,
-                                      period_stat, datetime_column):
+def aggregate_xarray_to_stress_period(data, datetime_coords_name='time',
+                                      start_datetime=None, end_datetime=None,
+                                      period_stat='mean'):
 
     if isinstance(start_datetime, pd.Timestamp):
         start_datetime = start_datetime.strftime('%Y-%m-%d')
     if isinstance(end_datetime, pd.Timestamp):
         end_datetime = end_datetime.strftime('%Y-%m-%d')
     if isinstance(period_stat, str):
         period_stat = [period_stat]
@@ -629,31 +739,49 @@
             arr = data.loc[start:end].values
 
         # stat specified by single item
         elif len(period_stat) == 1:
             period = period_stat.pop()
             # stat for a specified month
             if period in months.keys() or period in months.values():
-                arr = data.loc[data[datetime_column].dt.month == months.get(period, period)].values
+                arr = data.loc[data[datetime_coords_name].dt.month == months.get(period, period)].values
 
             # stat for a period specified by single string (e.g. '2014', '2014-01', etc.)
             else:
                 arr = data.loc[period].values
 
         # no period specified; use start/end of current period
         elif len(period_stat) == 0:
+
+            assert datetime_coords_name in data.coords, \
+                "datetime_column needed for " \
+                "resampling irregular data to model stress periods"
+            # not sure if this is needed for xarray
+            if data[datetime_coords_name].dtype == object:
+                data[datetime_coords_name] = pd.to_datetime(data[datetime_coords_name])
+            # default to aggregating whole dataset
+            # if start_ and end_datetime not provided
+            if start_datetime is None:
+                start_datetime = data[datetime_coords_name].values[0]
+            if end_datetime is None:
+                end_datetime = data[datetime_coords_name].values[-1]
+            # >= includes the start datetime
+            # for now, in comparison to aggregate_dataframe_to_stress_period() fn
+            # for tabular data (pandas)
+            # assume that xarray data does not have an end_datetime column
+            # (infer the end datetimes)
             arr = data.loc[start_datetime:end_datetime].values
 
         else:
             raise Exception("")
 
     # compute statistic on data
-    period_stat = getattr(arr, stat)(axis=0)
+    aggregated = getattr(arr, stat)(axis=0)
 
-    return period_stat
+    return aggregated
 
 
 def add_date_comments_to_tdis(tdis_file, start_dates, end_dates=None):
     """Add stress period start and end dates to a tdis file as comments;
     add modflow-setup version info to tdis file header.
     """
     tempfile = tdis_file + '.temp'
```

### Comparing `modflow-setup-0.2.0/mfsetup/testing.py` & `modflow-setup-0.3.0/mfsetup/testing.py`

 * *Files identical despite different names*

### Comparing `modflow-setup-0.2.0/mfsetup/tests/conftest.py` & `modflow-setup-0.3.0/mfsetup/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `modflow-setup-0.2.0/mfsetup/tests/data/shellmound.yml` & `modflow-setup-0.3.0/mfsetup/tests/data/shellmound.yml`

 * *Files 4% similar despite different names*

```diff
@@ -197,28 +197,29 @@
     save_flows: True
   griddata:
     iconvert: 1  # convertible layers
     # initial global values for storage
     sy: 0.25
     ss: 1.e-6
 
-# recharge package
+# Recharge Package
 rch:
   options:
     print_input: True
     print_flows: False
     save_flows: True
     readasarrays: True
   source_data:
     # resample recharge from NetCDF file with time-series of grids
     recharge:
       filename: 'shellmound/net_infiltration__2000-01-01_to_2017-12-31__414_by_394.nc'
       variable: 'net_infiltration'
       length_units: 'inches'
       time_units: 'days'
+      crs: 5070
       resample_method: 'linear'
       period_stats:
         # for the first two stress periods
         # apply mean recharge rates for dates below
         0: ['mean', '2000-01-01', '2017-12-31']
         1: ['mean', '2000-01-01', '2017-12-31']
         2: 'mean'  # for periods 2 on, use the mean recharge for that period
@@ -288,17 +289,29 @@
     save_flows: True
   source_data:
     shapefile:
       filename: '../../../mfsetup/tests/data/shellmound/shps/waterbodies.shp'
       id_column: 'COMID' # shapefile attribute field with include_ids:
       include_ids: [18046162] # features used to form the boundary
       boundname_col: 'GNIS_NAME'
-    head:
-      filename: 'shellmound/rasters/meras_100m_dem.tif'
-      elevation_units: 'feet'
+    csvfile:
+      filename: 'shellmound/tables/chd_heads.csv'
+      id_column: 'comid'
+      datetime_column: 'start_datetime'
+      end_datetime_column: 'end_datetime'
+      head_column: 'head'
+      length_units: 'feet'
+      # how heads will be aggregated to the model stress periods
+      period_stats:
+          # apply the mean heads across a specified time period
+          # for the initial steady state
+          # (default of 'mean' uses all times in input data)
+          0: ['mean', '2000-01-01', '2017-12-31']
+          1: mean  # apply the mean heads for the time period of s.p. 1
+          #  the last statistic specified (mean) will also be applied to subsequent periods
 
 # Drain Package
 drn:
   options:
     save_flows: True
   source_data:
     shapefile:
@@ -326,18 +339,34 @@
       include_ids: [18046230]
       # argument to rasterio.features.rasterize
       # if true, all grid cells touching the feature(s)
       # in the shapefile will be assigned BCs, if False
       # only the cells with centers inside the polygon
       # will be included
       all_touched: True
-    bhead:
-      filename: 'shellmound/rasters/meras_100m_dem.tif'
-      elevation_units: 'feet'
-    cond: 1.e+3
+    # Example of mixed boundary condition input, where
+    # a shapefile defines the feature extents
+    # a csvfile defines transient head values
+    # a raster defines static but spatially varying conductance
+    csvfile:
+      filename: 'shellmound/tables/chd_heads.csv'
+      id_column: 'comid'
+      datetime_column: 'start_datetime'
+      end_datetime_column: 'end_datetime'
+      bhead_column: 'head'
+      length_units: 'feet'
+      # with no period_stats: block, aggregation defaults
+      # to 'mean' for each stress period
+    cond:
+      # note: a single global value could also be specified here,
+      # as for the Drain Package
+      filename: shellmound/rasters/k330.tif
+      length_units: meters
+      time_units: days
+
 
 # River Package
 riv:
   options:
     save_flows: True
   source_data:
     shapefile:
```

### Comparing `modflow-setup-0.2.0/mfsetup/tests/plot.py` & `modflow-setup-0.3.0/mfsetup/tests/plot.py`

 * *Files identical despite different names*

### Comparing `modflow-setup-0.2.0/mfsetup/tests/test_bcs.py` & `modflow-setup-0.3.0/mfsetup/tests/test_bcs.py`

 * *Files identical despite different names*

### Comparing `modflow-setup-0.2.0/mfsetup/tests/test_discretization.py` & `modflow-setup-0.3.0/mfsetup/tests/test_discretization.py`

 * *Files identical despite different names*

### Comparing `modflow-setup-0.2.0/mfsetup/tests/test_equality.py` & `modflow-setup-0.3.0/mfsetup/tests/test_equality.py`

 * *Files identical despite different names*

### Comparing `modflow-setup-0.2.0/mfsetup/tests/test_evaporation.py` & `modflow-setup-0.3.0/mfsetup/tests/test_evaporation.py`

 * *Files identical despite different names*

### Comparing `modflow-setup-0.2.0/mfsetup/tests/test_fileio.py` & `modflow-setup-0.3.0/mfsetup/tests/test_fileio.py`

 * *Files identical despite different names*

### Comparing `modflow-setup-0.2.0/mfsetup/tests/test_get_data_from_parent.py` & `modflow-setup-0.3.0/mfsetup/tests/test_get_data_from_parent.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,36 +4,38 @@
 import pytest
 
 
 def get_model(basic_model_instance, parent_stress_period_input):
     m = basic_model_instance
     m.setup_dis()
     m.cfg['parent']['copy_stress_periods'] = parent_stress_period_input
-    m._set_perioddata()
+    #m._set_perioddata()
+    m.perioddata
     # test how parent stress periods are used in package setup
     if m.version != 'mf6':
         m.setup_bas6()
     m.setup_tdis()
     return m
 
 
-@pytest.mark.parametrize('input',
+@pytest.mark.parametrize('copy_parent_sp',
            ('all',
             [0],  # repeat parent stress period 0
             [2],  # repeat parent stress period 2
             [1, 2]  # include parent stress periods 1 and 2, repeating 2
             ))
-def test_get_perimeter_heads_from_parent(input, basic_model_instance, request, project_root_path):
+def test_get_perimeter_heads_from_parent(copy_parent_sp,
+                                         basic_model_instance, request, project_root_path):
     # change the working dir to the current model_ws
     # (wd gets set to model_ws for each model handled in basic_model
     os.chdir(basic_model_instance._abs_model_ws)
     test_name = request.node.name.split('[')[1].strip(']')
-    if basic_model_instance.name == 'pfl' and input not in ('all', [0]):
+    if basic_model_instance.name == 'pfl' and copy_parent_sp not in ('all', [0]):
         return
-    m = get_model(basic_model_instance, input)
+    m = get_model(basic_model_instance, copy_parent_sp)
 
     # perimeter heads
     # kind of cheesy because it doesn't test the actual values, only differences
     if m.version == 'mf6':
         m.cfg['chd']['mfsetup_options']['external_files'] = False
     chd = m.setup_chd(**m.cfg['chd'], **m.cfg['chd']['mfsetup_options'])
     data = chd.stress_period_data.data
@@ -48,23 +50,23 @@
     # actually got two heads that were the same for the pleasant_nwt test case,
     # even though time series appeared to be correctly sampled from parent model
     # so for the purpose of the test, allow for two heads to match
     all_heads_are_different = len(np.unique(np.array(mean_heads))) >= len(mean_heads) - 1
     first_value_different = np.array_equal(np.diff(np.round(mean_heads, 4)) == 0,
                                            [False] + [True] * (len(mean_heads) - 2))
     expected = {'pfl_nwt-all': same_head_as_start,  # one parent model stress period, 'all' input
-                'pfl_nwt-input1': same_head_as_start,  # one parent model stress period, input=[0]
+                'pfl_nwt-copy_parent_sp1': same_head_as_start,  # one parent model stress period, input=[0]
                 'pleasant_nwt-all': all_heads_are_different,  # many parent model stress periods, input='all'
-                'pleasant_nwt-input1': same_head_as_start,  # many parent model stress periods, input=[0]
-                'pleasant_nwt-input2': same_head_as_start,  # many parent model stress periods, input=[2]
-                'pleasant_nwt-input3': first_value_different,  # many parent model stress periods, input=[1, 2]
+                'pleasant_nwt-copy_parent_sp1': same_head_as_start,  # many parent model stress periods, input=[0]
+                'pleasant_nwt-copy_parent_sp2': same_head_as_start,  # many parent model stress periods, input=[2]
+                'pleasant_nwt-copy_parent_sp3': first_value_different,  # many parent model stress periods, input=[1, 2]
                 'get_pleasant_mf6-all': all_heads_are_different,
-                'get_pleasant_mf6-input1': same_head_as_start,
-                'get_pleasant_mf6-input2': same_head_as_start,
-                'get_pleasant_mf6-input3': first_value_different,
+                'get_pleasant_mf6-copy_parent_sp1': same_head_as_start,
+                'get_pleasant_mf6-copy_parent_sp2': same_head_as_start,
+                'get_pleasant_mf6-copy_parent_sp3': first_value_different,
                 }
     assert expected[test_name]
     # reset the working directory
     os.chdir(project_root_path)
 
 
 @pytest.mark.parametrize('input', ('all',
```

### Comparing `modflow-setup-0.2.0/mfsetup/tests/test_get_model_version.py` & `modflow-setup-0.3.0/mfsetup/tests/test_get_model_version.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,25 +3,28 @@
 import pytest
 
 from mfsetup import __version__
 from mfsetup.model_version import get_versions
 from mfsetup.tests.conftest import basic_model_instance
 
 
-@pytest.mark.parametrize('start_version', ('0',
-                                           '3.0.0',
-                                           '3.0',
-                                           '3'
+@pytest.mark.parametrize('start_version', (
+    #'0' start_version=0 is the default, and
+    # only produces result below if there are no tags
+    '3.0.0',
+    '3.0',
+    '3'
                                            )
                          )
 def test_get_versions(start_version):
     rest = get_versions(path='.',
                         start_version='')
     result = get_versions(path='.',
                           start_version=start_version)
+    #
     assert result['version'] == start_version + rest['version']
 
 
 def test_get_version_without_git(project_root_path):
     path = os.path.join(project_root_path, '..')
     result = get_versions(path=path,
                           start_version='0')
```

### Comparing `modflow-setup-0.2.0/mfsetup/tests/test_grid.py` & `modflow-setup-0.3.0/mfsetup/tests/test_grid.py`

 * *Files identical despite different names*

### Comparing `modflow-setup-0.2.0/mfsetup/tests/test_interpolation.py` & `modflow-setup-0.3.0/mfsetup/tests/test_interpolation.py`

 * *Files identical despite different names*

### Comparing `modflow-setup-0.2.0/mfsetup/tests/test_lakes.py` & `modflow-setup-0.3.0/mfsetup/tests/test_lakes.py`

 * *Files identical despite different names*

### Comparing `modflow-setup-0.2.0/mfsetup/tests/test_lgr.py` & `modflow-setup-0.3.0/mfsetup/tests/test_lgr.py`

 * *Files identical despite different names*

### Comparing `modflow-setup-0.2.0/mfsetup/tests/test_mf5to6.py` & `modflow-setup-0.3.0/mfsetup/tests/test_mf5to6.py`

 * *Files identical despite different names*

### Comparing `modflow-setup-0.2.0/mfsetup/tests/test_mf6_shellmound.py` & `modflow-setup-0.3.0/mfsetup/tests/test_mf6_shellmound.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from mfsetup import testing
 from mfsetup.checks import check_external_files_for_nans
 from mfsetup.discretization import (
     cellids_to_kij,
     find_remove_isolated_cells,
     get_layer_thicknesses,
 )
-from mfsetup.fileio import exe_exists, load_array, load_cfg, read_mf6_block
+from mfsetup.fileio import exe_exists, load, load_array, load_cfg, read_mf6_block
 from mfsetup.grid import rasterize
 from mfsetup.mf6model import MF6model
 from mfsetup.units import convert_length_units
 from mfsetup.utils import get_input_arguments
 
 
 @pytest.fixture(scope="module", autouse=True)
@@ -179,14 +179,24 @@
     expected_listfile_name = model.cfg['model']['list_filename_fmt'].format(model.name)
     with open(model.namefile) as src:
         for line in src:
             if 'LIST' in line:
                 assert line.strip().split()[-1] == expected_listfile_name
 
 
+def test_ims_setup(shellmound_model):
+    model = shellmound_model
+    ims = model.setup_ims()
+
+    assert ims.csv_outer_output_filerecord is not None
+
+    assert ims.csv_outer_output_filerecord.array[0][0] == \
+        'solver_outer_out.csv'
+
+
 def test_snap_to_NHG(shellmound_cfg, shellmound_simulation):
     cfg = deepcopy(shellmound_cfg)
     #simulation = deepcopy(simulation)
     cfg['model']['simulation'] = shellmound_simulation
     cfg['setup_grid']['snap_to_NHG'] = True
 
     cfg = MF6model._parse_model_kwargs(cfg)
@@ -464,39 +474,30 @@
                                           'column_mappings':
                                               {'obsname': ['obsprefix'],
                                                'x': 'x_5070',
                                                'y': 'y_5070'}
                                           },
                                      },
                                     ])
-def test_obs_setup(shellmound_model_with_dis, config):
+def test_obs_setup(shellmound_model_with_dis, config, project_root_path):
     m = shellmound_model_with_dis  # deepcopy(model)
-    defaults = {'default_columns':
-                    {'x_location_col': 'x', # x coordinates in wtm
-                     'y_location_col': 'y' # y coordinates in wtm
-                     },
-                'filename_fmt': '{}.head.obs',  # only head obs supported at this point
-                'options':
-                    {'digits': 10,
-                     'print_input': True}
-                }
-    defaults.update(config)
-    m.cfg['obs'] = defaults
-    obs = m.setup_obs()
+    default_mf6_cfg = load(Path(project_root_path) / 'mfsetup/mf6_defaults.yml')
+    kwargs = default_mf6_cfg['obs'].copy()
+    kwargs.update(config)
+    obs = m.setup_obs(**kwargs)
     obs.write()
     obsfile = os.path.join(m.model_ws, obs.filename)
     assert os.path.exists(obsfile)
     assert isinstance(obs, mf6.ModflowUtlobs)
     with open(obsfile) as obsdata:
         for line in obsdata:
             if 'fileout' in line.lower():
                 _, _, _, fname = line.strip().split()
-                assert fname == m.cfg['obs']['filename_fmt'].format(m.name)
+                assert fname == m.cfg['obs']['mfsetup_options']['filename_fmt'].format(m.name)
                 break
-    j=2
 
 
 @pytest.mark.parametrize('input', [
     # flopy-style input
     {'saverecord': {0: {'head': 'last', 'budget': 'last'}}},
     # MODFLOW 6-style input
     {'period_options': {0: ['save head last', 'save budget last']}},
@@ -615,16 +616,47 @@
     assert len(df) > 0
     k, i, j = zip(*df['cellid'])
     cell_bottoms = m.dis.botm.array[k, i, j]
     for var in head_variables:
         assert np.all(df[var] > cell_bottoms)
     if pckg_abbrv == 'riv':
         assert np.all(df['stage'] > df['rbot'])
-    if pckg_abbrv != 'chd':
+    if pckg_abbrv not in {'chd', 'ghb'}:
         assert np.all(df['cond'] == m.cfg[pckg_abbrv]['source_data']['cond'])
+    # checks for basic transient csv input case
+    if pckg_abbrv == 'chd':
+        include_ids = m.cfg['chd']['source_data']['shapefile']['include_ids']
+        in_df = pd.read_csv(m.cfg['chd']['source_data']['csvfile']['filename'])
+        in_df = in_df.loc[in_df['comid'].isin(include_ids)]
+        spd_heads = np.array(
+            [ra[0][1] for per, ra in m.chd.stress_period_data.data.items()])
+        # every stress period should have input
+        assert len(m.chd.stress_period_data.data.keys()) == m.nper
+        # heads in CHD package should match the CSV input,
+        # after conversion to meters
+        assert np.allclose(in_df['head'].values, spd_heads[1:]/.3048)
+    # more advanced transient input case with csv
+    # and conductance values specified via a raster
+    if pckg_abbrv == 'ghb':
+        in_df = pd.read_csv(m.cfg['ghb']['source_data']['csvfile']['filename'])
+        spd_heads = np.array(
+            [ra[0][1] for per, ra in m.ghb.stress_period_data.data.items()])
+        # every stress period should have input
+        assert len(m.ghb.stress_period_data.data.keys()) == m.nper
+        # heads in CHD package should match the CSV input,
+        # after conversion to meters
+        assert np.allclose(in_df['head'].values[-1], spd_heads[1:]/.3048)
+
+        in_raster = m.cfg['ghb']['source_data']['cond']['filename']
+        with rasterio.open(in_raster) as src:
+            data = src.read(1)
+            raster_cond = np.unique(data[data > 0])[0]
+        spd_conds = np.array(
+            [ra[0][2] for per, ra in m.ghb.stress_period_data.data.items()])
+        assert np.allclose(spd_conds, raster_cond)
     if boundnames:
         assert 'boundname_col' in m.cfg[pckg_abbrv]['source_data']['shapefile']
         assert not set(df['boundname']).symmetric_difference(boundnames)
 
 
 def test_wel_setup(shellmound_model_with_dis):
     m = shellmound_model_with_dis  # deepcopy(model)
@@ -688,16 +720,15 @@
     sums = np.array(sums)
     sums2 = np.array(sums2)
     # if this doesn't match
     # may be due to wells with invalid open intervals getting removed
     assert np.allclose(sums, sums2, rtol=0.01)
 
 
-def test_sfr_setup(model_with_sfr
-                   ):
+def test_sfr_setup(model_with_sfr, project_root_path):
     m = model_with_sfr
     m.sfr.write()
     assert os.path.exists(os.path.join(m.model_ws, m.sfr.filename))
     assert isinstance(m.sfr, mf6.ModflowGwfsfr)
     output_path = m._shapefiles_path
     shapefiles = ['{}/{}_sfr_cells.shp'.format(output_path, m.name),
                   '{}/{}_sfr_outlets.shp'.format(output_path, m.name),
@@ -728,15 +759,15 @@
 
     # check that adding runoff works
     runoff_period_data = m.sfrdata.period_data.dropna(subset=['runoff'], axis=0)
     # only compare periods 2-7 (2007-04-01 to 2010-04-01)
     runoff_period_data = runoff_period_data.loc[2:].copy()
     runoff_period_data['line_id_in_model'] = runoff_period_data['line_id_in_model'].astype(int)
     # sum runoff by line id for each period
-    runoff_period_comid_sums = runoff_period_data.groupby(['per', 'line_id_in_model']).sum()
+    runoff_period_comid_sums = runoff_period_data.groupby(['per', 'line_id_in_model']).sum(numeric_only=True)
     # then take the mean for each line id across periods
     mean_period_data_runoff_by_comid = runoff_period_comid_sums.groupby('line_id_in_model').mean()
     # read in the input values
     df = pd.read_csv('../../data/shellmound/tables/swb_runoff_by_nhdplus_comid_m3d.csv')
     df['time'] = pd.to_datetime(df['time'])
     df = df.loc['2007-04-01':]
     mean_input_runoff_by_comid = df.groupby('comid').mean()
@@ -772,15 +803,18 @@
     # that is in the model. So any catchment in the model that is not a headwater in NHDPlus
     # will have runoff greater than the input data.
 
     # check minimum slope
     assert np.allclose(np.round(m.sfr.packagedata.array['rgrd'].min(), 6), \
                        np.round(m.cfg['sfr']['sfrmaker_options']['minimum_slope'], 6))
     # check that no observations were placed in cells with SFR
-    m.setup_obs()
+    #default_mf6_cfg = load(Path(project_root_path) / 'mfsetup/mf6_defaults.yml')
+    #kwargs = default_mf6_cfg['obs'].copy()
+    #kwargs.update(config)
+    obs = m.setup_obs(**m.cfg['obs'])
     sfr_cells = set(m.sfr.packagedata.array['cellid'])
     obs_cells = set(m.obs[1].continuous.data['shellmound.head.obs']['id'])
     assert not any(obs_cells.intersection(sfr_cells))
 
 
 def test_sfr_inflows_from_csv(model_with_sfr):
     m = model_with_sfr
```

### Comparing `modflow-setup-0.2.0/mfsetup/tests/test_mf6_shellmound_mixed_layers.py` & `modflow-setup-0.3.0/mfsetup/tests/test_mf6_shellmound_mixed_layers.py`

 * *Files identical despite different names*

### Comparing `modflow-setup-0.2.0/mfsetup/tests/test_mf6_shellmound_rot_grid.py` & `modflow-setup-0.3.0/mfsetup/tests/test_mf6_shellmound_rot_grid.py`

 * *Files identical despite different names*

### Comparing `modflow-setup-0.2.0/mfsetup/tests/test_mf6_tmr_shellmound.py` & `modflow-setup-0.3.0/mfsetup/tests/test_mf6_tmr_shellmound.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,15 +166,16 @@
 
 
 @pytest.mark.parametrize('from_binary', (False, True))
 def test_ic_setup(shellmound_tmr_model_with_dis, from_binary):
     """Test starting heads setup from model top or parent model head solution
     (MODFLOW binary output)."""
     m = copy.deepcopy(shellmound_tmr_model_with_dis)
-    binaryfile = str(Path(m.parent.model_ws) / f'{m.parent.name}.hds')
+    parent_ws = Path(m.cfg['parent']['model_ws'])
+    binaryfile = str(parent_ws / f'{m.parent.name}.hds')
     if from_binary:
         config = {'strt': {'from_parent': {'binaryfile': binaryfile,
                                            'period': 0
                                            }}}
         m.cfg['ic']['source_data'] = config
     ic = m.setup_ic()
     ic.write()
```

### Comparing `modflow-setup-0.2.0/mfsetup/tests/test_notebooks.py` & `modflow-setup-0.3.0/mfsetup/tests/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `modflow-setup-0.2.0/mfsetup/tests/test_obs.py` & `modflow-setup-0.3.0/mfsetup/tests/test_obs.py`

 * *Files identical despite different names*

### Comparing `modflow-setup-0.2.0/mfsetup/tests/test_oc.py` & `modflow-setup-0.3.0/mfsetup/tests/test_oc.py`

 * *Files identical despite different names*

### Comparing `modflow-setup-0.2.0/mfsetup/tests/test_pfl_mfnwt_inset.py` & `modflow-setup-0.3.0/mfsetup/tests/test_pfl_mfnwt_inset.py`

 * *Files 0% similar despite different names*

```diff
@@ -544,15 +544,15 @@
 
     # TODO: add datetime comments to OC file
 
 
 def test_hyd_setup(pfl_nwt_with_dis_bas6):
 
     m = pfl_nwt_with_dis_bas6  #deepcopy(pfl_nwt_with_dis)
-    hyd = m.setup_hyd()
+    hyd = m.setup_hyd(**m.cfg['hyd'])
     hyd.write_file()
     # verify that each head observation is in each layer
     df = pd.DataFrame(hyd.obsdata)
     heads = df.loc[df.arr == b'HD']
     nobs = len(set(heads.hydlbl))
     assert sorted(heads.klay.tolist()) == sorted(list(range(m.nlay)) * nobs)
     #m.cfg['hyd'][]
```

### Comparing `modflow-setup-0.2.0/mfsetup/tests/test_pleasant_mf6_inset.py` & `modflow-setup-0.3.0/mfsetup/tests/test_pleasant_mf6_inset.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,17 +132,17 @@
     package_list = [s.lower() for s in m.parent.get_package_list()]
     for package in m.cfg['parent']['skip_load']:
         assert package.lower() not in package_list
 
 
 def test_perioddata(get_pleasant_mf6, pleasant_nwt):
     nwt = pleasant_nwt
-    nwt._set_perioddata()
+    nwt.perioddata
     m = get_pleasant_mf6
-    m._set_perioddata()
+    m.perioddata
     assert m.perioddata['start_datetime'][0] == pd.Timestamp(m.cfg['tdis']['options']['start_date_time'])
     pd.testing.assert_frame_equal(m.perioddata, nwt.perioddata, check_dtype=False)
 
 
 def test_tdis_setup(get_pleasant_mf6):
 
     m = get_pleasant_mf6 #deepcopy(model)
@@ -303,24 +303,24 @@
         assert np.any(m._isbc2d == 2)
         assert npf.k.array.max() == m.cfg['high_k_lakes']['high_k_value']
         # for now, k33 not adjusted in setting high-k lakes
 
 
 def test_obs_setup(get_pleasant_mf6_with_dis):
     m = get_pleasant_mf6_with_dis  # deepcopy(model)
-    obs = m.setup_obs()
+    obs = m.setup_obs(**m.cfg['obs'])
     obs.write()
     obsfile = os.path.join(m.model_ws, obs.filename)
     assert os.path.exists(obsfile)
     assert isinstance(obs, mf6.ModflowUtlobs)
     with open(obsfile) as obsdata:
         for line in obsdata:
             if 'fileout' in line.lower():
                 _, _, _, fname = line.strip().split()
-                assert fname == m.cfg['obs']['filename_fmt'].format(m.name)
+                assert fname == m.cfg['obs']['mfsetup_options']['filename_fmt'].format(m.name)
                 break
 
 
 def test_oc_setup(get_pleasant_mf6_with_dis):
     m = get_pleasant_mf6_with_dis  # deepcopy(model)
     oc = m.setup_oc()
     oc.write()
```

### Comparing `modflow-setup-0.2.0/mfsetup/tests/test_pleasant_mfnwt_inset.py` & `modflow-setup-0.3.0/mfsetup/tests/test_pleasant_mfnwt_inset.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from mfsetup.discretization import find_remove_isolated_cells
 from mfsetup.fileio import load_array
 from mfsetup.tests.test_lakes import get_prism_data
 
 
 def test_perioddata(get_pleasant_nwt):
     m = get_pleasant_nwt
-    m._set_perioddata()
+    m.perioddata
     assert m.perioddata['start_datetime'][0] == pd.Timestamp(m.cfg['dis']['start_date_time'])
 
 
 def test_ibound(pleasant_nwt_with_dis):
     m = pleasant_nwt_with_dis
     # use pleasant lake extent as ibound
     is_pleasant_lake = m.lakarr[0]
```

### Comparing `modflow-setup-0.2.0/mfsetup/tests/test_solver_setup.py` & `modflow-setup-0.3.0/mfsetup/tests/test_solver_setup.py`

 * *Files identical despite different names*

### Comparing `modflow-setup-0.2.0/mfsetup/tests/test_sourcedata.py` & `modflow-setup-0.3.0/mfsetup/tests/test_sourcedata.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 import os
+from pathlib import Path
 
+import gisutils
 import numpy as np
 import pandas as pd
+import pyproj
 import pytest
 from shapely.geometry import Point
 
 import xarray as xr
 from mfsetup.discretization import weighted_average_between_layers
 from mfsetup.fileio import _parse_file_path_keys_from_source_data
 from mfsetup.sourcedata import (
     ArraySourceData,
     MFArrayData,
     MFBinaryArraySourceData,
+    NetCDFSourceData,
     TabularSourceData,
     TransientArraySourceData,
     TransientTabularSourceData,
     transient2d_to_xarray,
 )
 from mfsetup.units import convert_length_units, convert_time_units
 
@@ -349,15 +353,15 @@
     input_csv = os.path.join(tmpdir, 'csv_cap_cols.csv')
     df = pd.read_csv(csvfile)
     df.columns = [c.capitalize() for c in df.columns]
     # create a geometry column of wkt strings, as would result if the csv were written by geopandas.to_csv
     df['geometry'] = [str(Point(x, y)) for x, y in zip(df.X, df.Y)]
     df.to_csv(input_csv, index=False)
 
-    sd = TransientTabularSourceData(filenames=input_csv, data_column='Flux_m3',
+    sd = TransientTabularSourceData(filenames=input_csv, data_columns='Flux_m3',
                                     datetime_column='Start_datetime', id_column='Node',
                                     x_col='X', y_col='Y',
                                     period_stats={0: 'mean', 1: None, 2: 'none', 3: 'mean'},
                                     length_units='unknown', time_units='unknown', volume_units=None,
                                     column_mappings=None, resolve_duplicates_with='sum',
                                     dest_model=m)
     # expected period stats
@@ -381,7 +385,109 @@
     filenames = None
     sd = TransientArraySourceData(filenames, 'rech', period_stats=None,
                  length_units='unknown', time_units='days',
                  dest_model=None, source_modelgrid=None, source_array=None,
                  from_source_model_layers=None, datatype=None,
                  resample_method='nearest', vmin=-1e30, vmax=1e30
                  )
+
+@pytest.mark.parametrize('crs', (
+    None,
+    5070,
+    pytest.param(4269, marks=pytest.mark.xfail(reason='inconsistent CRS'))
+    ))
+def test_netcdf_source_data(test_data_path, tmpdir, crs,
+                            shellmound_model_with_dis):
+
+    # netcdf input in same projection as the model
+    ncfile = test_data_path / \
+        'shellmound/net_infiltration__2000-01-01_to_2017-12-31__414_by_394.nc'
+    m = shellmound_model_with_dis
+
+    sd = NetCDFSourceData(ncfile, 'net_infiltration', period_stats={0: 'mean'},
+                 length_units='inches', time_units='days',
+                 dest_model=m, crs=crs
+                 )
+    results1 = sd.get_data()
+
+    # only run the next part of the test,
+    # which looks at reproject, once
+    if crs is None:
+        # make a new netcdf on a different CRS
+        ds = xr.open_dataset(ncfile)
+
+        orig_grid_mapping = ds.crs.attrs.copy()
+        std_parallel = (orig_grid_mapping.pop('latitude_of_first_standard_parallel'),
+                        orig_grid_mapping.pop('latitude_of_second_standard_parallel'))
+        orig_grid_mapping['standard_parallel'] = std_parallel
+        orig_crs = pyproj.CRS.from_cf(orig_grid_mapping)
+
+        # reference the second netcdf to UTM zone 15 north
+        dest_epsg = 26915
+        dest_crs = pyproj.CRS(dest_epsg)
+        x, y = np.meshgrid(ds.x, ds.y)
+        X_utm, Y_utm = gisutils.project((x, y), orig_crs, dest_crs)
+        dx = ds.x.diff(dim='x').values[0]
+        dy = ds.y.diff(dim='y').values[0]
+        # new x and y vectors
+        x_utm = np.add.accumulate([0] + np.ones(len(ds.x)).tolist()[:-1]) * dx + X_utm[0, 0]
+        y_utm = np.add.accumulate([0] + np.ones(len(ds.y)).tolist()[:-1]) * dy + Y_utm[0, 0]
+        # represenations of new x and y locations in old crs
+        x2, y2 = gisutils.project(tuple(np.meshgrid(x_utm, y_utm)), dest_crs, orig_crs)
+
+        interped = ds['net_infiltration'].interp(x=(['x', 'y'], x2),
+                                                y=(['x', 'y'], y2),
+                                                method='linear')
+        ds2 = xr.Dataset({
+            'net_infiltration': (('time', 'y', 'x'), interped.values),
+            'crs': ds['crs'].values
+            },
+                    #dims=['time', 'y', 'x'],
+                    coords={'x': x_utm, 'y': y_utm, 'time': interped.time}
+                    )
+        ds2['crs'].attrs = dest_crs.to_cf()
+        # write out netcdf
+        reprojected_ncfile = Path(tmpdir) / f'net_inf_{dest_epsg}.nc'
+        ds2.to_netcdf(reprojected_ncfile, format='netcdf4', engine='netcdf4', #engine='h5netcdf',
+                        encoding={'net_infiltration': {'zlib': True, 'complevel': 4,
+                                                        'dtype': 'float32', #'scale_factor': 0.01,
+                                                        '_FillValue': -9999,
+                                                        }})
+        sd2 = NetCDFSourceData(reprojected_ncfile, 'net_infiltration', period_stats={0: 'mean'},
+                    length_units='inches', time_units='days',
+                    dest_model=m, #resample_method='linear'
+                    )
+        results2 = sd2.get_data()
+        # the reprojected results won't match the original results
+        # especially well, because of the coarse grid size
+        # and interpolation involved in resampling
+        # the orignal onto another rectilinear grid
+        # in a different orientation (the non-model crs)
+        # both nearest and linear resampling result in
+        # error between 1 and 5%
+        for per in results1.keys():
+            assert np.allclose(results1[per].mean(),
+                            results2[per].mean(), rtol=0.05)
+        # write another netcdf with no CRS information
+        del ds2['crs']
+        reprojected_ncfile = Path(tmpdir) / f'net_inf_no-crs.nc'
+        ds2.to_netcdf(reprojected_ncfile, format='netcdf4', engine='netcdf4', #engine='h5netcdf',
+                        encoding={'net_infiltration': {'zlib': True, 'complevel': 4,
+                                                        'dtype': 'float32', #'scale_factor': 0.01,
+                                                        '_FillValue': -9999,
+                                                        }})
+        sd3 = NetCDFSourceData(reprojected_ncfile, 'net_infiltration', period_stats={0: 'mean'},
+                    length_units='inches', time_units='days', crs=dest_epsg,
+                    dest_model=m, #resample_method='linear'
+                    )
+        results3 = sd3.get_data()
+        # the reprojected results won't match the original results
+        # especially well, because of the coarse grid size
+        # and interpolation involved in resampling
+        # the orignal onto another rectilinear grid
+        # in a different orientation (the non-model crs)
+        # both nearest and linear resampling result in
+        # error between 1 and 5%
+        for per in results1.keys():
+            assert np.allclose(results1[per].mean(),
+                            results3[per].mean(), rtol=0.05)
+        j=2
```

### Comparing `modflow-setup-0.2.0/mfsetup/tests/test_tdis.py` & `modflow-setup-0.3.0/mfsetup/tests/test_tdis.py`

 * *Files 2% similar despite different names*

```diff
@@ -227,15 +227,16 @@
     # test adding parent stress periods to perioddata table
     m.cfg['parent']['copy_stress_periods'] = copy_periods
     if m.version != 'mf6':
         m.cfg['dis']['nper'] = nper
         for var in ['perlen', 'nstp', 'tsmult', 'steady']:
             del m.cfg['dis'][var]
     m._set_parent()
-    m._set_perioddata()
+    m._perioddata = None
+    m.perioddata
     assert np.array_equal(m.perioddata['parent_sp'], np.array(expected[test_name]))
 
 
 @pytest.mark.parametrize('dates', [('2007-04-01', '2007-03-31'),
                                    ('2008-04-01', '2008-09-30'),
                                    ('2008-10-01', '2009-03-31')])
 @pytest.mark.parametrize('sourcefile', ['tables/sp69_pumping_from_meras21_m3.csv',
@@ -270,15 +271,15 @@
     start, end = dates
     welldata = pd.read_csv(os.path.join(shellmound_datapath, sourcefile
                                         ))
 
     welldata['start_datetime'] = pd.to_datetime(welldata.start_datetime)
     welldata['end_datetime'] = pd.to_datetime(welldata.end_datetime)
     duplicate_well = welldata.groupby('node').get_group(welldata.node.values[0])
-    welldata = welldata.append(duplicate_well)
+    welldata = pd.concat([welldata, duplicate_well], axis=0)
     start_datetime = pd.Timestamp(start)
     end_datetime = pd.Timestamp(end)  # pandas convention of including last day
     result = aggregate_dataframe_to_stress_period(welldata, id_column='node', data_column='flux_m3',
                                                   datetime_column='start_datetime', end_datetime_column='end_datetime',
                                                   start_datetime=start_datetime, end_datetime=end_datetime,
                                                   period_stat='mean', resolve_duplicates_with='sum')
     overlap = (welldata.start_datetime < end_datetime) & \
@@ -289,15 +290,16 @@
 
     # for each location (id), take the mean across source data time periods
     if end_datetime < start_datetime:
         assert result['flux_m3'].sum() == 0
     if not any(overlap):
         assert len(result) == 0
     if any(overlap):
-        agg = welldata.loc[overlap].copy().groupby(['start_datetime', 'node']).sum().reset_index()
+        groupbedby = welldata.loc[overlap].copy().groupby(['start_datetime', 'node'])
+        agg = groupbedby.sum(numeric_only=True).reset_index()
         agg = agg.groupby('node').mean().reset_index()
         expected_sum = agg['flux_m3'].sum()
         if duplicate_well.node.values[0] in agg.index:
             dw_overlaps = (duplicate_well.start_datetime < end_datetime) & \
                     (duplicate_well.end_datetime > start_datetime)
             expected_sum += duplicate_well.loc[dw_overlaps, 'flux_m3'].mean()
         assert np.allclose(result['flux_m3'].sum(), expected_sum)
@@ -370,24 +372,28 @@
                           'perlen': perlen,
                           'steady': False})
     return times
 
 
 @pytest.mark.parametrize('category_col', (None, 'comment'))
 def test_aggregate_values_with_categories(obsdata, times, category_col, dest_model, tmpdir):
-    file = os.path.join(tmpdir, 'obsdata.csv')
-    obsdata.to_csv(file, index=False)
+    csvfile = os.path.join(tmpdir, 'obsdata.csv')
+    obsdata['flow_ft3d'] = obsdata['flow_m3d']/(.3048**3)
+    obsdata.to_csv(csvfile, index=False)
     dest_model._perioddata = times
-    sd = TransientTabularSourceData(file, data_column='flow_m3d', datetime_column='datetime', id_column='line_id',
+    sd = TransientTabularSourceData(csvfile, data_columns=['flow_m3d', 'flow_ft3d'], datetime_column='datetime', id_column='line_id',
                                     x_col='x', y_col='y', end_datetime_column=None, period_stats={0: 'mean'},
                                     length_units='unknown', time_units='unknown', volume_units=None,
                                     column_mappings=None, category_column=category_col,
                                     resolve_duplicates_with='raise error',
                                     dest_model=dest_model)
     results = sd.get_data()
+    # check that multiple data_columns get passed through
+    # and treated the same
+    assert np.allclose(results['flow_m3d']/results['flow_ft3d'],.3048**3)
     results.sort_values(by=['per', 'site_no'], inplace=True)
     assert np.array_equal(results.site_no.values,
                           np.array([2000, 2001, 2000, 2002]))
     assert np.array_equal(results['flow_m3d'].values,
                           np.array([1.000000,  # 2000 value in per 0
                                     0.500000,  # 2001 average for per 0
                                     2.000000,  # 2000 value in per 1
```

### Comparing `modflow-setup-0.2.0/mfsetup/tests/test_testing.py` & `modflow-setup-0.3.0/mfsetup/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `modflow-setup-0.2.0/mfsetup/tests/test_tmr.py` & `modflow-setup-0.3.0/mfsetup/tests/test_tmr.py`

 * *Files identical despite different names*

### Comparing `modflow-setup-0.2.0/mfsetup/tests/test_units.py` & `modflow-setup-0.3.0/mfsetup/tests/test_units.py`

 * *Files identical despite different names*

### Comparing `modflow-setup-0.2.0/mfsetup/tests/test_usage.py` & `modflow-setup-0.3.0/mfsetup/tests/test_usage.py`

 * *Files identical despite different names*

### Comparing `modflow-setup-0.2.0/mfsetup/tests/test_utils.py` & `modflow-setup-0.3.0/mfsetup/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `modflow-setup-0.2.0/mfsetup/tests/test_wateruse.py` & `modflow-setup-0.3.0/mfsetup/tests/test_wateruse.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,16 +52,16 @@
     monthlyQ_cols = [col_fmt.format(calendar.month_abbr[i]).lower()
                      for i in range(1, 13)]
     wu['annual_total_calc'] = wu[monthlyQ_cols].sum(axis=1)
 
     # verify that the monthly values match the annual totals
     assert np.allclose(wu['annual_wdrl_total_gallons'], wu['annual_total_calc'])
 
-    sums = wu.dropna(subset=['annual_wdrl_total_gallons'], axis=0).groupby('site_no').sum()
-    means = wu.dropna(subset=['annual_wdrl_total_gallons'], axis=0).groupby('site_no').mean()
+    sums = wu.dropna(subset=['annual_wdrl_total_gallons'], axis=0).groupby('site_no').sum(numeric_only=True)
+    means = wu.dropna(subset=['annual_wdrl_total_gallons'], axis=0).groupby('site_no').mean(numeric_only=True)
     means['Q_m3d'] = sums['annual_wdrl_total_gallons'] / sums['days'] / conversions[2]
 
     sites = [int(s.strip('site')) for s in df.boundname]
     means = means.loc[sites]
     compare = pd.DataFrame({'site_no': df.index,
                             'Q1': df['q'],  # wel package flux computed by get_mean_pumping_rates
                             'Q2': -means['Q_m3d']})  # expected wel package flux
@@ -114,15 +114,15 @@
     perlen = list(m.cfg['dis']['perlen'])
     m.cfg['dis']['nper'] = nper + 1
     m.cfg['dis']['steady'] = [True] + [False] * nper
     m.cfg['dis']['perlen'] = [1] + perlen
     m.cfg['dis']['nstp'] = [1] + [5] * nper
     m.cfg['dis']['tsmult'] = [1] + [1.2] * nper
 
-    m._set_perioddata()
+    m.perioddata
     m.perioddata['parent_sp'] = [0] + list(range(nper))
     assert m.perioddata.steady[0]
     assert m.perioddata.perlen[0] == 1
 
     # test with transient first stress period
     m.setup_wel(**m.cfg['wel'], **m.cfg['wel']['mfsetup_options'])
     df = m.wel.stress_period_data.get_dataframe()
```

### Comparing `modflow-setup-0.2.0/mfsetup/tests/test_wells.py` & `modflow-setup-0.3.0/mfsetup/tests/test_wells.py`

 * *Files identical despite different names*

### Comparing `modflow-setup-0.2.0/mfsetup/tmr.py` & `modflow-setup-0.3.0/mfsetup/tmr.py`

 * *Files identical despite different names*

### Comparing `modflow-setup-0.2.0/mfsetup/units.py` & `modflow-setup-0.3.0/mfsetup/units.py`

 * *Files identical despite different names*

### Comparing `modflow-setup-0.2.0/mfsetup/utils.py` & `modflow-setup-0.3.0/mfsetup/utils.py`

 * *Files identical despite different names*

### Comparing `modflow-setup-0.2.0/mfsetup/wateruse.py` & `modflow-setup-0.3.0/mfsetup/wateruse.py`

 * *Files 0% similar despite different names*

```diff
@@ -263,16 +263,16 @@
             period_data = inperiod.copy()
         # mean for given month (e.g. august mean)
         elif stat in months.keys() or stat in months.values():
             period_data = inperiod.loc[inperiod.month == months.get(stat, stat)].copy()
         else:
             raise ValueError('Unrecognized input for stat: {}'.format(stat))
 
-        site_means = period_data.groupby('site_no').mean()
-        site_sums = period_data.groupby('site_no').sum()
+        site_means = period_data.groupby('site_no').mean(numeric_only=True)
+        site_sums = period_data.groupby('site_no').sum(numeric_only=True)
         site_means['gal_d'] = site_sums['gallons'] / site_sums['days']
         # conversion to model units is based on lenuni variable in DIS package
         gal_to_model_units = convert_volume_units('gal', get_model_length_units(model))
         site_means['q'] = site_means.gal_d * gal_to_model_units
         site_means['per'] = per
 
         wel_data.append(well_info[['k', 'i', 'j']].join(site_means[['q', 'per']], how='inner'))
```

### Comparing `modflow-setup-0.2.0/mfsetup/wells.py` & `modflow-setup-0.3.0/mfsetup/wells.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from shapely.geometry import Point
 
 from mfsetup.fileio import append_csv, check_source_files
 from mfsetup.grid import get_ij
 from mfsetup.sourcedata import TransientTabularSourceData
 from mfsetup.wateruse import get_mean_pumping_rates, resample_pumping_rates
 
+
 def setup_wel_data(model, source_data=None, #for_external_files=True,
                    dropped_wells_file='dropped_wells.csv'):
     """Performs the part of well package setup that is independent of
     MODFLOW version. Returns a DataFrame with the information
     needed to set up stress_period_data.
     """
     # default options for distributing fluxes vertically
@@ -80,15 +81,15 @@
         spd['i'] = i
         spd['j'] = j
 
         # map wells to inset model layers if different from parent
         to_inset_layers = {v:k for k, v in model.parent_layers.items()}
         spd['k'] = [to_inset_layers[k] for k in spd['k']]
 
-        df = df.append(spd)
+        df = pd.concat([df, spd], axis=0)
 
 
     # read source data and map onto model space and time discretization
     # multiple types of source data can be submitted
     elif datasets is not None:
         for k, v in datasets.items():
 
@@ -107,15 +108,15 @@
                         vfd = vfd_defaults.copy()
                         vfd.update(v.get('vertical_flux_distribution', {}))
                         csvdata = assign_layers_from_screen_top_botm(csvdata,
                                                                      model,
                                                                      **vfd)
                     else:
                         csvdata['k'] = 0
-                df = df.append(csvdata[columns])
+                df = pd.concat([df, csvdata[columns]], axis=0)
 
             elif k.lower() == 'wells':  # generic dict
                 added_wells = {k: v for k, v in v.items() if v is not None}
                 if len(added_wells) > 0:
                     aw = pd.DataFrame(added_wells).T
                     aw['boundname'] = aw.index
                 else:
@@ -123,15 +124,15 @@
                 if aw is not None:
                     if 'x' in aw.columns and 'y' in aw.columns:
                         aw['i'], aw['j'] = get_ij(model.modelgrid,
                                                   aw['x'].values,
                                                   aw['y'].values)
                     aw['per'] = aw['per'].astype(int)
                     aw['k'] = aw['k'].astype(int)
-                    df = df.append(aw)
+                    df = pd.concat([df, aw], axis=0)
 
             elif k.lower() == 'wdnr_dataset':  # custom input format for WI DNR
                 # Get steady-state pumping rates
                 check_source_files([v['water_use'],
                                     v['water_use_points']])
 
                 # fill out period stats
@@ -148,22 +149,22 @@
 
                 if len(periods_with_dataset_means) > 0:
                     wu_means = get_mean_pumping_rates(v['water_use'],
                                                       v['water_use_points'],
                                                       period_stats=periods_with_dataset_means,
                                                       drop_ids=v.get('drop_ids'),
                                                       model=model)
-                    df = df.append(wu_means)
+                    df = pd.concat([df, wu_means], axis=0)
                 if len(resampled_periods) > 0:
                     wu_resampled = resample_pumping_rates(v['water_use'],
                                                           v['water_use_points'],
                                                           drop_ids=v.get('drop_ids'),
                                                           exclude_steady_state=True,
                                                           model=model)
-                    df = df.append(wu_resampled)
+                    df = pd.concat([df, wu_resampled], axis=0)
 
     for col in ['per', 'k', 'i', 'j']:
         df[col] = df[col].astype(int)
 
     # drop any k, i, j locations that are inactive
     if model.version == 'mf6':
         inactive = model.dis.idomain.array[df.k.values,
```

### Comparing `modflow-setup-0.2.0/mfsetup/zbud.py` & `modflow-setup-0.3.0/mfsetup/zbud.py`

 * *Files identical despite different names*

### Comparing `modflow-setup-0.2.0/modflow_setup.egg-info/PKG-INFO` & `modflow-setup-0.3.0/modflow_setup.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: modflow-setup
-Version: 0.2.0
-Summary: Package to facilitate setup of a MODFLOW-6 groundwater flow model with the SFR package.
+Version: 0.3.0
+Summary: Robust automation of MODFLOW model construction.
 Home-page: https://github.com/aleaf/modflow-setup
 Author: USGS MAP Project
 Author-email: aleaf@usgs.gov
 License: BSD (3-clause)
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
@@ -16,19 +16,19 @@
 
 
 Modflow-setup
 -----------------------------------------------
 Modflow-setup is a Python package for automating the setup of MODFLOW groundwater models from grid-independent source data including shapefiles, rasters, and other MODFLOW models that are geo-located. Input data and model construction options are summarized in a single configuration file. Source data are read from their native formats and mapped to a regular finite difference grid specified in the configuration file. An external array-based [Flopy](https://github.com/modflowpy/flopy) model instance with the desired packages is created from the sampled source data and configuration settings. MODFLOW input can then be written from the flopy model instance.
 
 
-### Version 0.1
-![Tests](https://github.com/usgs/modflow-setup/workflows/Tests/badge.svg)
-[![codecov](https://codecov.io/gh/usgs/modflow-setup/branch/develop/graph/badge.svg?token=aWN47DYeIv)](https://codecov.io/gh/usgs/modflow-setup)
+### Version 0.2
+![Tests](https://github.com/aleaf/modflow-setup/workflows/Tests/badge.svg)
+[![codecov](https://codecov.io/gh/aleaf/modflow-setup/branch/develop/graph/badge.svg?token=aWN47DYeIv)](https://codecov.io/gh/aleaf/modflow-setup)
 [![PyPI version](https://badge.fury.io/py/modflow-setup.svg)](https://badge.fury.io/py/modflow-setup)
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/usgs/modflow-setup/develop?urlpath=lab/tree/examples)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/doi-usgs/modflow-setup/develop?urlpath=lab/tree/examples)
 [![Project Status: Active – The project has reached a stable, usable state and is being actively developed.](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active)
 
 
 
 
 
 Getting Started
```

### Comparing `modflow-setup-0.2.0/modflow_setup.egg-info/SOURCES.txt` & `modflow-setup-0.3.0/modflow_setup.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `modflow-setup-0.2.0/setup.py` & `modflow-setup-0.3.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,15 @@
                     if not line.startswith('#')]
 
 
 setup(
     name='modflow-setup',
     version=versioneer.get_version(),
     cmdclass=versioneer.get_cmdclass(),
-    description="Package to facilitate setup of a MODFLOW-6 groundwater flow model with the SFR package.",
+    description="Robust automation of MODFLOW model construction.",
     long_description=readme,
     long_description_content_type='text/markdown',
     author="USGS MAP Project",
     author_email='aleaf@usgs.gov',
     url='https://github.com/aleaf/modflow-setup',
     python_requires='>={}'.format('.'.join(str(n) for n in min_version)),
     packages=find_packages(exclude=['docs', 'tests']),
```

### Comparing `modflow-setup-0.2.0/versioneer.py` & `modflow-setup-0.3.0/versioneer.py`

 * *Files identical despite different names*

