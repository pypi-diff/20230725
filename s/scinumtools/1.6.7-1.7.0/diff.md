# Comparing `tmp/scinumtools-1.6.7.tar.gz` & `tmp/scinumtools-1.7.0.tar.gz`

## Comparing `scinumtools-1.6.7.tar` & `scinumtools-1.7.0.tar`

### file list

```diff
@@ -1,89 +1,89 @@
--rwxr-xr-x   0        0        0      188 2020-02-02 00:00:00.000000 scinumtools-1.6.7/build_doc.sh
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 scinumtools-1.6.7/requirements.txt
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 scinumtools-1.6.7/.github/workflows/pytest.yml
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 scinumtools-1.6.7/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 scinumtools-1.6.7/.github/workflows/static.yml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 scinumtools-1.6.7/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 scinumtools-1.6.7/docs/make.bat
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 scinumtools-1.6.7/docs/source/conf.py
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 scinumtools-1.6.7/docs/source/data.rst
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 scinumtools-1.6.7/docs/source/index.rst
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 scinumtools-1.6.7/docs/source/introduction.rst
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 scinumtools-1.6.7/docs/source/math.rst
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 scinumtools-1.6.7/docs/source/phys.rst
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 scinumtools-1.6.7/docs/source/stats.rst
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 scinumtools-1.6.7/docs/source/structs.rst
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 scinumtools-1.6.7/docs/source/api/modules.rst
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 scinumtools-1.6.7/docs/source/api/scinumtools.data.rst
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 scinumtools-1.6.7/docs/source/api/scinumtools.math.rst
--rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 scinumtools-1.6.7/docs/source/api/scinumtools.math.solver.rst
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 scinumtools-1.6.7/docs/source/api/scinumtools.phys.rst
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 scinumtools-1.6.7/docs/source/api/scinumtools.phys.units.rst
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 scinumtools-1.6.7/docs/source/api/scinumtools.rst
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 scinumtools-1.6.7/docs/source/api/scinumtools.stats.rst
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 scinumtools-1.6.7/docs/source/api/scinumtools.structs.rst
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 scinumtools-1.6.7/src/scinumtools/__init__.py
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 scinumtools-1.6.7/src/scinumtools/data/CachingClass.py
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 scinumtools-1.6.7/src/scinumtools/data/ImageClass.py
--rw-r--r--   0        0        0     6086 2020-02-02 00:00:00.000000 scinumtools-1.6.7/src/scinumtools/data/PlottingClass.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 scinumtools-1.6.7/src/scinumtools/data/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scinumtools-1.6.7/src/scinumtools/math/__init__.py
--rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 scinumtools-1.6.7/src/scinumtools/math/solver/AtomClass.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 scinumtools-1.6.7/src/scinumtools/math/solver/ExpressionClass.py
--rw-r--r--   0        0        0     7525 2020-02-02 00:00:00.000000 scinumtools-1.6.7/src/scinumtools/math/solver/OperatorClass.py
--rw-r--r--   0        0        0     3803 2020-02-02 00:00:00.000000 scinumtools-1.6.7/src/scinumtools/math/solver/SolverClass.py
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 scinumtools-1.6.7/src/scinumtools/math/solver/TokensClass.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 scinumtools-1.6.7/src/scinumtools/math/solver/__init__.py
--rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 scinumtools-1.6.7/src/scinumtools/phys/ConstantsClass.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 scinumtools-1.6.7/src/scinumtools/phys/__init__.py
--rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 scinumtools-1.6.7/src/scinumtools/phys/units/BaseUnitsClass.py
--rw-r--r--   0        0        0     3332 2020-02-02 00:00:00.000000 scinumtools-1.6.7/src/scinumtools/phys/units/DimensionsClass.py
--rw-r--r--   0        0        0     3403 2020-02-02 00:00:00.000000 scinumtools-1.6.7/src/scinumtools/phys/units/FractionClass.py
--rw-r--r--   0        0        0    13259 2020-02-02 00:00:00.000000 scinumtools-1.6.7/src/scinumtools/phys/units/QuantityClass.py
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 scinumtools-1.6.7/src/scinumtools/phys/units/UnitClass.py
--rw-r--r--   0        0        0     2538 2020-02-02 00:00:00.000000 scinumtools-1.6.7/src/scinumtools/phys/units/UnitConverters.py
--rw-r--r--   0        0        0    10710 2020-02-02 00:00:00.000000 scinumtools-1.6.7/src/scinumtools/phys/units/UnitList.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 scinumtools-1.6.7/src/scinumtools/phys/units/__init__.py
--rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 scinumtools-1.6.7/src/scinumtools/stats/StopwatchClass.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 scinumtools-1.6.7/src/scinumtools/stats/__init__.py
--rw-r--r--   0        0        0     5509 2020-02-02 00:00:00.000000 scinumtools-1.6.7/src/scinumtools/structs/CollectorClass.py
--rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 scinumtools-1.6.7/src/scinumtools/structs/ParameterClass.py
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 scinumtools-1.6.7/src/scinumtools/structs/ProgressBar.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 scinumtools-1.6.7/src/scinumtools/structs/__init__.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 scinumtools-1.6.7/tests/README.md
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 scinumtools-1.6.7/tests/cached_data.npy
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 scinumtools-1.6.7/tests/pyproject.toml
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scinumtools-1.6.7/tests/requirements.txt
--rw-r--r--   0        0        0     6537 2020-02-02 00:00:00.000000 scinumtools-1.6.7/tests/test_data.py
--rw-r--r--   0        0        0     4225 2020-02-02 00:00:00.000000 scinumtools-1.6.7/tests/test_math.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 scinumtools-1.6.7/tests/test_physics.py
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 scinumtools-1.6.7/tests/test_stats.py
--rw-r--r--   0        0        0     4184 2020-02-02 00:00:00.000000 scinumtools-1.6.7/tests/test_struct.py
--rw-r--r--   0        0        0    12551 2020-02-02 00:00:00.000000 scinumtools-1.6.7/tests/test_units.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 scinumtools-1.6.7/tests/src/scinumtools/__init__.py
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 scinumtools-1.6.7/tests/src/scinumtools/data/CachingClass.py
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 scinumtools-1.6.7/tests/src/scinumtools/data/ImageClass.py
--rw-r--r--   0        0        0     4741 2020-02-02 00:00:00.000000 scinumtools-1.6.7/tests/src/scinumtools/data/PlottingClass.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 scinumtools-1.6.7/tests/src/scinumtools/data/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scinumtools-1.6.7/tests/src/scinumtools/math/__init__.py
--rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 scinumtools-1.6.7/tests/src/scinumtools/math/solver/AtomClass.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 scinumtools-1.6.7/tests/src/scinumtools/math/solver/ExpressionClass.py
--rw-r--r--   0        0        0     7525 2020-02-02 00:00:00.000000 scinumtools-1.6.7/tests/src/scinumtools/math/solver/OperatorClass.py
--rw-r--r--   0        0        0     3803 2020-02-02 00:00:00.000000 scinumtools-1.6.7/tests/src/scinumtools/math/solver/SolverClass.py
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 scinumtools-1.6.7/tests/src/scinumtools/math/solver/TokensClass.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 scinumtools-1.6.7/tests/src/scinumtools/math/solver/__init__.py
--rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 scinumtools-1.6.7/tests/src/scinumtools/phys/ConstantsClass.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 scinumtools-1.6.7/tests/src/scinumtools/phys/__init__.py
--rw-r--r--   0        0        0     9181 2020-02-02 00:00:00.000000 scinumtools-1.6.7/tests/src/scinumtools/phys/units/QuantityClass.py
--rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 scinumtools-1.6.7/tests/src/scinumtools/phys/units/UnitConverters.py
--rw-r--r--   0        0        0    10140 2020-02-02 00:00:00.000000 scinumtools-1.6.7/tests/src/scinumtools/phys/units/UnitList.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scinumtools-1.6.7/tests/src/scinumtools/phys/units/__init__.py
--rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 scinumtools-1.6.7/tests/src/scinumtools/stats/StopwatchClass.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 scinumtools-1.6.7/tests/src/scinumtools/stats/__init__.py
--rw-r--r--   0        0        0     5397 2020-02-02 00:00:00.000000 scinumtools-1.6.7/tests/src/scinumtools/structs/CollectorClass.py
--rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 scinumtools-1.6.7/tests/src/scinumtools/structs/ParameterClass.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 scinumtools-1.6.7/tests/src/scinumtools/structs/__init__.py
--rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 scinumtools-1.6.7/.gitignore
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 scinumtools-1.6.7/README.md
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 scinumtools-1.6.7/pyproject.toml
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 scinumtools-1.6.7/PKG-INFO
+-rwxr-xr-x   0        0        0      246 2020-02-02 00:00:00.000000 scinumtools-1.7.0/build_doc.sh
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 scinumtools-1.7.0/requirements.txt
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 scinumtools-1.7.0/.github/workflows/pytest.yml
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 scinumtools-1.7.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 scinumtools-1.7.0/.github/workflows/static.yml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 scinumtools-1.7.0/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 scinumtools-1.7.0/docs/make.bat
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 scinumtools-1.7.0/docs/source/conf.py
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 scinumtools-1.7.0/docs/source/data.rst
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 scinumtools-1.7.0/docs/source/index.rst
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 scinumtools-1.7.0/docs/source/introduction.rst
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 scinumtools-1.7.0/docs/source/math.rst
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 scinumtools-1.7.0/docs/source/phys.rst
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 scinumtools-1.7.0/docs/source/stats.rst
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 scinumtools-1.7.0/docs/source/structs.rst
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 scinumtools-1.7.0/docs/source/api/modules.rst
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 scinumtools-1.7.0/docs/source/api/scinumtools.data.rst
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 scinumtools-1.7.0/docs/source/api/scinumtools.math.rst
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 scinumtools-1.7.0/docs/source/api/scinumtools.math.solver.rst
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 scinumtools-1.7.0/docs/source/api/scinumtools.phys.rst
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 scinumtools-1.7.0/docs/source/api/scinumtools.phys.units.rst
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 scinumtools-1.7.0/docs/source/api/scinumtools.rst
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 scinumtools-1.7.0/docs/source/api/scinumtools.stats.rst
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 scinumtools-1.7.0/docs/source/api/scinumtools.structs.rst
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 scinumtools-1.7.0/src/scinumtools/__init__.py
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 scinumtools-1.7.0/src/scinumtools/data/CachingClass.py
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 scinumtools-1.7.0/src/scinumtools/data/ImageClass.py
+-rw-r--r--   0        0        0     4617 2020-02-02 00:00:00.000000 scinumtools-1.7.0/src/scinumtools/data/PlottingClass.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 scinumtools-1.7.0/src/scinumtools/data/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scinumtools-1.7.0/src/scinumtools/math/__init__.py
+-rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 scinumtools-1.7.0/src/scinumtools/math/solver/AtomClass.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 scinumtools-1.7.0/src/scinumtools/math/solver/ExpressionClass.py
+-rw-r--r--   0        0        0     7525 2020-02-02 00:00:00.000000 scinumtools-1.7.0/src/scinumtools/math/solver/OperatorClass.py
+-rw-r--r--   0        0        0     3803 2020-02-02 00:00:00.000000 scinumtools-1.7.0/src/scinumtools/math/solver/SolverClass.py
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 scinumtools-1.7.0/src/scinumtools/math/solver/TokensClass.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 scinumtools-1.7.0/src/scinumtools/math/solver/__init__.py
+-rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 scinumtools-1.7.0/src/scinumtools/phys/ConstantsClass.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 scinumtools-1.7.0/src/scinumtools/phys/__init__.py
+-rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 scinumtools-1.7.0/src/scinumtools/phys/units/BaseUnitsClass.py
+-rw-r--r--   0        0        0     3332 2020-02-02 00:00:00.000000 scinumtools-1.7.0/src/scinumtools/phys/units/DimensionsClass.py
+-rw-r--r--   0        0        0     3403 2020-02-02 00:00:00.000000 scinumtools-1.7.0/src/scinumtools/phys/units/FractionClass.py
+-rw-r--r--   0        0        0    13259 2020-02-02 00:00:00.000000 scinumtools-1.7.0/src/scinumtools/phys/units/QuantityClass.py
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 scinumtools-1.7.0/src/scinumtools/phys/units/UnitClass.py
+-rw-r--r--   0        0        0     2538 2020-02-02 00:00:00.000000 scinumtools-1.7.0/src/scinumtools/phys/units/UnitConverters.py
+-rw-r--r--   0        0        0    10710 2020-02-02 00:00:00.000000 scinumtools-1.7.0/src/scinumtools/phys/units/UnitList.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 scinumtools-1.7.0/src/scinumtools/phys/units/__init__.py
+-rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 scinumtools-1.7.0/src/scinumtools/stats/StopwatchClass.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 scinumtools-1.7.0/src/scinumtools/stats/__init__.py
+-rw-r--r--   0        0        0     5905 2020-02-02 00:00:00.000000 scinumtools-1.7.0/src/scinumtools/structs/CollectorClass.py
+-rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 scinumtools-1.7.0/src/scinumtools/structs/ParameterClass.py
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 scinumtools-1.7.0/src/scinumtools/structs/ProgressBar.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 scinumtools-1.7.0/src/scinumtools/structs/__init__.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 scinumtools-1.7.0/tests/README.md
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 scinumtools-1.7.0/tests/cached_data.npy
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 scinumtools-1.7.0/tests/pyproject.toml
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scinumtools-1.7.0/tests/requirements.txt
+-rw-r--r--   0        0        0     6016 2020-02-02 00:00:00.000000 scinumtools-1.7.0/tests/test_data.py
+-rw-r--r--   0        0        0     4225 2020-02-02 00:00:00.000000 scinumtools-1.7.0/tests/test_math.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 scinumtools-1.7.0/tests/test_physics.py
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 scinumtools-1.7.0/tests/test_stats.py
+-rw-r--r--   0        0        0     4432 2020-02-02 00:00:00.000000 scinumtools-1.7.0/tests/test_struct.py
+-rw-r--r--   0        0        0    12551 2020-02-02 00:00:00.000000 scinumtools-1.7.0/tests/test_units.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 scinumtools-1.7.0/tests/src/scinumtools/__init__.py
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 scinumtools-1.7.0/tests/src/scinumtools/data/CachingClass.py
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 scinumtools-1.7.0/tests/src/scinumtools/data/ImageClass.py
+-rw-r--r--   0        0        0     4741 2020-02-02 00:00:00.000000 scinumtools-1.7.0/tests/src/scinumtools/data/PlottingClass.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 scinumtools-1.7.0/tests/src/scinumtools/data/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scinumtools-1.7.0/tests/src/scinumtools/math/__init__.py
+-rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 scinumtools-1.7.0/tests/src/scinumtools/math/solver/AtomClass.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 scinumtools-1.7.0/tests/src/scinumtools/math/solver/ExpressionClass.py
+-rw-r--r--   0        0        0     7525 2020-02-02 00:00:00.000000 scinumtools-1.7.0/tests/src/scinumtools/math/solver/OperatorClass.py
+-rw-r--r--   0        0        0     3803 2020-02-02 00:00:00.000000 scinumtools-1.7.0/tests/src/scinumtools/math/solver/SolverClass.py
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 scinumtools-1.7.0/tests/src/scinumtools/math/solver/TokensClass.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 scinumtools-1.7.0/tests/src/scinumtools/math/solver/__init__.py
+-rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 scinumtools-1.7.0/tests/src/scinumtools/phys/ConstantsClass.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 scinumtools-1.7.0/tests/src/scinumtools/phys/__init__.py
+-rw-r--r--   0        0        0     9181 2020-02-02 00:00:00.000000 scinumtools-1.7.0/tests/src/scinumtools/phys/units/QuantityClass.py
+-rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 scinumtools-1.7.0/tests/src/scinumtools/phys/units/UnitConverters.py
+-rw-r--r--   0        0        0    10140 2020-02-02 00:00:00.000000 scinumtools-1.7.0/tests/src/scinumtools/phys/units/UnitList.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scinumtools-1.7.0/tests/src/scinumtools/phys/units/__init__.py
+-rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 scinumtools-1.7.0/tests/src/scinumtools/stats/StopwatchClass.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 scinumtools-1.7.0/tests/src/scinumtools/stats/__init__.py
+-rw-r--r--   0        0        0     5397 2020-02-02 00:00:00.000000 scinumtools-1.7.0/tests/src/scinumtools/structs/CollectorClass.py
+-rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 scinumtools-1.7.0/tests/src/scinumtools/structs/ParameterClass.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 scinumtools-1.7.0/tests/src/scinumtools/structs/__init__.py
+-rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 scinumtools-1.7.0/.gitignore
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 scinumtools-1.7.0/README.md
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 scinumtools-1.7.0/pyproject.toml
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 scinumtools-1.7.0/PKG-INFO
```

### Comparing `scinumtools-1.6.7/.github/workflows/python-publish.yml` & `scinumtools-1.7.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.7/.github/workflows/static.yml` & `scinumtools-1.7.0/.github/workflows/static.yml`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.7/docs/Makefile` & `scinumtools-1.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.7/docs/make.bat` & `scinumtools-1.7.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.7/docs/source/conf.py` & `scinumtools-1.7.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.7/docs/source/index.rst` & `scinumtools-1.7.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.7/docs/source/api/scinumtools.data.rst` & `scinumtools-1.7.0/docs/source/api/scinumtools.data.rst`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.7/docs/source/api/scinumtools.math.solver.rst` & `scinumtools-1.7.0/docs/source/api/scinumtools.math.solver.rst`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.7/docs/source/api/scinumtools.phys.units.rst` & `scinumtools-1.7.0/docs/source/api/scinumtools.phys.units.rst`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.7/docs/source/api/scinumtools.structs.rst` & `scinumtools-1.7.0/docs/source/api/scinumtools.structs.rst`

 * *Files 21% similar despite different names*

```diff
@@ -16,14 +16,22 @@
 -----------------------------------------
 
 .. automodule:: scinumtools.structs.ParameterClass
    :members:
    :undoc-members:
    :show-inheritance:
 
+scinumtools.structs.ProgressBar module
+--------------------------------------
+
+.. automodule:: scinumtools.structs.ProgressBar
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 Module contents
 ---------------
 
 .. automodule:: scinumtools.structs
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `scinumtools-1.6.7/src/scinumtools/data/CachingClass.py` & `scinumtools-1.7.0/src/scinumtools/data/CachingClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.7/src/scinumtools/data/ImageClass.py` & `scinumtools-1.7.0/src/scinumtools/data/ImageClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.7/src/scinumtools/data/PlottingClass.py` & `scinumtools-1.7.0/tests/src/scinumtools/data/PlottingClass.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from matplotlib.colors import Normalize, LogNorm
 from dataclasses import dataclass
 import numpy as np
-from typing import Union
 
 from ..structs import ArrayCollector
 
 @dataclass
 class Ranges:
     """ Dataclass that contains data ranges
     """
@@ -102,49 +101,14 @@
         """ Return logarithmic norm from ranges
         """
         return LogNorm(
             vmin=np.log10(np.nanmin(self._collector.zminpos)), 
             vmax=np.log10(np.nanmax(self._collector.zmax))
         )
 
-class DataPlotGrid:
-    data: Union[list,dict]
-    ndata: int
-    ncols: int
-    nrows: int
-    figsize: tuple
-
-    def __init__(self, data, ncols=2, axsize=(4,2)):
-        self.data = data
-        self.ndata = len(data)
-        self.ncols = ncols
-        self.nrows = int(np.ceil(self.ndata/self.ncols))
-        self.figsize = (self.ncols*axsize[0], self.nrows*axsize[1])
-
-    def items(self, missing=None, transpose=False):
-        if missing:
-            for i in range(self.ndata, self.ncols*self.nrows):
-                if transpose:
-                    yield (i,int(i%self.nrows),int(i/self.nrows))
-                else:
-                    yield (i,int(i/self.ncols),int(i%self.ncols))
-        else:
-            if isinstance(self.data, list):
-                for i,d in enumerate(self.data):
-                    if transpose:
-                        yield (i,int(i%self.nrows),int(i/self.nrows),d)
-                    else:
-                        yield (i,int(i/self.ncols),int(i%self.ncols),d)
-            elif isinstance(self.data, dict):
-                for i,(k,v) in enumerate(self.data.items()):
-                    if transpose:
-                        yield (i,int(i%self.nrows),int(i/self.nrows),k,v)
-                    else:
-                        yield (i,int(i/self.ncols),int(i%self.ncols),k,v)
-
 def ListToGrid(data, ncols, missing=None, transpose=False):
     """
     Enumerate given data with an index and row/column number specified by number of columns
 
     :param list data: Any iterable data, e.g. list, array
     :param int ncols: Number of grid columns
     :param bool missing: List only missing grid points
```

### Comparing `scinumtools-1.6.7/src/scinumtools/math/solver/AtomClass.py` & `scinumtools-1.7.0/src/scinumtools/math/solver/AtomClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.7/src/scinumtools/math/solver/ExpressionClass.py` & `scinumtools-1.7.0/src/scinumtools/math/solver/ExpressionClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.7/src/scinumtools/math/solver/OperatorClass.py` & `scinumtools-1.7.0/src/scinumtools/math/solver/OperatorClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.7/src/scinumtools/math/solver/SolverClass.py` & `scinumtools-1.7.0/src/scinumtools/math/solver/SolverClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.7/src/scinumtools/math/solver/TokensClass.py` & `scinumtools-1.7.0/src/scinumtools/math/solver/TokensClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.7/src/scinumtools/phys/ConstantsClass.py` & `scinumtools-1.7.0/src/scinumtools/phys/ConstantsClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.7/src/scinumtools/phys/units/BaseUnitsClass.py` & `scinumtools-1.7.0/src/scinumtools/phys/units/BaseUnitsClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.7/src/scinumtools/phys/units/DimensionsClass.py` & `scinumtools-1.7.0/src/scinumtools/phys/units/DimensionsClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.7/src/scinumtools/phys/units/FractionClass.py` & `scinumtools-1.7.0/src/scinumtools/phys/units/FractionClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.7/src/scinumtools/phys/units/QuantityClass.py` & `scinumtools-1.7.0/src/scinumtools/phys/units/QuantityClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.7/src/scinumtools/phys/units/UnitClass.py` & `scinumtools-1.7.0/src/scinumtools/phys/units/UnitClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.7/src/scinumtools/phys/units/UnitConverters.py` & `scinumtools-1.7.0/src/scinumtools/phys/units/UnitConverters.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.7/src/scinumtools/phys/units/UnitList.py` & `scinumtools-1.7.0/src/scinumtools/phys/units/UnitList.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.7/src/scinumtools/stats/StopwatchClass.py` & `scinumtools-1.7.0/src/scinumtools/stats/StopwatchClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.7/src/scinumtools/structs/CollectorClass.py` & `scinumtools-1.7.0/tests/src/scinumtools/structs/CollectorClass.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,17 +29,14 @@
         pass
     
     def __init__(self, columns: list):
         self._columns = []
         for column in columns:
             setattr(self,column,[])
             self._columns.append(column)
-
-    def __str__(self):
-        return self.to_text()
         
     def append(self, values: list):
         """ Append a single row
 
         :param values: List of values for each column
         """
         for n, name in enumerate(self._columns):
@@ -115,17 +112,14 @@
                 setattr(self,column,np.array([],**kwargs))
                 self._columns.append(column)
         else:
             for column in columns:
                 setattr(self,column,np.array([]))
                 self._columns.append(column)
 
-    def __str__(self):
-        return self.to_text()
-    
     def append(self, values: list):
         """ Append a single row
 
         :param values: List of values for each column
         """
         for n, name in enumerate(self._columns):
             data = getattr(self,name)
```

### Comparing `scinumtools-1.6.7/src/scinumtools/structs/ParameterClass.py` & `scinumtools-1.7.0/src/scinumtools/structs/ParameterClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.7/src/scinumtools/structs/ProgressBar.py` & `scinumtools-1.7.0/src/scinumtools/structs/ProgressBar.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.7/tests/cached_data.npy` & `scinumtools-1.7.0/tests/cached_data.npy`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.7/tests/pyproject.toml` & `scinumtools-1.7.0/tests/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.7/tests/test_data.py` & `scinumtools-1.7.0/tests/test_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -87,109 +87,84 @@
 
     assert xranges.minpos == 0.11111111111111116
     assert xranges.min == -9
     assert xranges.max == 9
     assert yranges.minpos == 0.10526315789473673
     assert yranges.min == -18
     assert yranges.max == 18
-    
-def test_list_to_grid():
 
-    data = range(5)
-    ncols = 2
-    
-    # List all defined grid points
+def test_data_plot_grid():
+    # test lists
     grid = [
         (0, 0, 0, 0),
         (1, 0, 1, 1),
         (2, 1, 0, 2),
         (3, 1, 1, 3),
         (4, 2, 0, 4),
     ]
-    for r,row in enumerate(ListToGrid(data,ncols)):
-        assert grid[r] == row
-
-    # List all missing grid points
-    for r,row in enumerate(ListToGrid(data,ncols,missing=True)):
-        assert (5, 2, 1) == row
-
-    # List transposed grid points
+    dpg = DataPlotGrid(list(range(5)), 2)
+    for i, m, n, v in dpg.items():
+        assert grid[i] == (i, m, n, v)
+    for i, m, n in dpg.items(missing=True):
+        assert (i, m, n) == (5, 2, 1)
     grid = [
         (0, 0, 0, 0),
         (1, 1, 0, 1),
         (2, 2, 0, 2),
         (3, 0, 1, 3),
         (4, 1, 1, 4),
     ]
-    for r,row in enumerate(ListToGrid(data,ncols,transpose=True)):
-        assert grid[r] == row
+    for i, m, n, v in dpg.items(transpose=True):
+        assert grid[i] == (i, m, n, v)
+    for i, m, n in dpg.items(transpose=True, missing=True):
+        assert (i, m, n) == (5, 2, 1)
         
-    # List all missing transposed grid points
-    for r,row in enumerate(ListToGrid(data,ncols,transpose=True,missing=True)):
-        assert (5, 2, 1) == row
-        
-def test_dict_to_grid():
-
-    data = dict(
+    # test dictionaries
+    dpg = DataPlotGrid(dict(
         a = 0,
         b = 1,
         c = 2,
         d = 3,
         e = 4
-    )
-    ncols = 2
-    
-    # List all defined grid points
+    ), 2)
     grid = [
         (0, 0, 0, 'a', 0),
         (1, 0, 1, 'b', 1),
         (2, 1, 0, 'c', 2),
         (3, 1, 1, 'd', 3),
         (4, 2, 0, 'e', 4),
     ]
-    for r,row in enumerate(DictToGrid(data,ncols)):
-        assert grid[r] == row
-
-    # List all missing grid points
-    grid = [
-        (5, 2, 1)
-    ]
-    for r,row in enumerate(DictToGrid(data,ncols,missing=True)):
-        assert grid[r] == row
-        
-    # List all transposed grid points
+    for i,m,n,k,v in dpg.items():
+        assert grid[i] == (i,m,n,k,v)
+    for i,m,n in dpg.items(missing=True):
+        assert (5, 2, 1) == (i,m,n)
     grid = [
         (0, 0, 0, 'a', 0),
         (1, 1, 0, 'b', 1),
         (2, 2, 0, 'c', 2),
         (3, 0, 1, 'd', 3),
         (4, 1, 1, 'e', 4),
     ]
-    for r,row in enumerate(DictToGrid(data,ncols,transpose=True)):
-        assert grid[r] == row
-
-    # List all missing transposed grid points
-    grid = [
-        (5, 2, 1)
-    ]
-    for r,row in enumerate(DictToGrid(data,ncols,transpose=True,missing=True)):
-        assert grid[r] == row
+    for i,m,n,k,v in dpg.items(transpose=True):
+        assert grid[i] == (i,m,n,k,v)
+    for i,m,n in dpg.items(transpose=True,missing=True):
+        assert (5, 2, 1) == (i,m,n)
         
 def test_thumbnail():
 
     # Test grayscale case
     nx, ny = 300, 200
     data = np.zeros((nx,ny))
     for i in range(nx):
         for j in range(ny):
             data[i,j] = (i-nx/2)**2 + (j-ny/2)**2
-            imold = ThumbnailImage(
-                extent = (-30,30,-20,20),
-                data = data
-            )
+    imold = ThumbnailImage(
+        extent = (-30,30,-20,20),
+        data = data
+    )
     np.testing.assert_equal(np.asarray(imold.im), data)
 
     # Test grayscale resizing
     data_resized = [
         [9.6480850e+03, 1.1210736e+04, 9.5458672e+03, 1.1227712e+04, 9.3136709e+03],
         [1.0238771e+04, 9.7449180e+03, 6.8944453e+03, 9.7642842e+03, 9.8572793e+03],
         [5.1896011e+03, 2.6150837e+03, 1.7226636e-03, 2.6263579e+03, 4.9675088e+03],
```

### Comparing `scinumtools-1.6.7/tests/test_math.py` & `scinumtools-1.7.0/tests/test_math.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.7/tests/test_stats.py` & `scinumtools-1.7.0/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.7/tests/test_struct.py` & `scinumtools-1.7.0/tests/test_struct.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 def test_row_collector_list():
     
     columns = ['col1','col2','col3']
     with ListCollector(columns) as lc:
         lc.append([1,2,3])
         lc.append([4,5,6])
         lc.append([7,8,9])
+        assert lc.size() == 3
         assert lc.col1 == [1,4,7]
         assert lc.col2 == [2,5,8]
         assert lc.col3 == [3,6,9]
         assert lc.to_dict() == dict(
             col1 = [1,4,7],
             col2 = [2,5,8],
             col3 = [3,6,9],
@@ -40,14 +41,15 @@
         
 def test_row_collector_array():
     
     with ArrayCollector(['col1','col2','col3']) as ac:
         ac.append([1,2,3])
         ac.append([4,5,6])
         ac.append([7,8,0])
+        assert ac.size() == 3
         np.testing.assert_equal(ac.col1, [1,4,7])
         np.testing.assert_equal(ac.col2, [2,5,8])
         np.testing.assert_equal(ac.col3, [3,6,0])
         np.testing.assert_equal(ac.to_dict(), dict(
             col1 = [1,4,7], 
             col2 = [2,5,8],
             col3 = [3,6,0],
@@ -134,7 +136,18 @@
         test(params)
     # direct value insertion
     params = ParameterDict(['a','b','c'],{
         'd': [1, 2, 3],
         'e': [4, 5, 6]
     })
     test(params)
+
+def test_progressbar():
+
+    nsteps = 200
+    pb = ProgressBar(nsteps)
+    for i in range(nsteps):
+        pb.step()
+    pb.close()
+
+    with ProgressBar(nsteps) as pb:
+        pb.step()
```

### Comparing `scinumtools-1.6.7/tests/test_units.py` & `scinumtools-1.7.0/tests/test_units.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.7/tests/src/scinumtools/data/ImageClass.py` & `scinumtools-1.7.0/tests/src/scinumtools/data/ImageClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.7/tests/src/scinumtools/data/PlottingClass.py` & `scinumtools-1.7.0/src/scinumtools/data/PlottingClass.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from matplotlib.colors import Normalize, LogNorm
 from dataclasses import dataclass
 import numpy as np
+from typing import Union
 
 from ..structs import ArrayCollector
 
 @dataclass
 class Ranges:
     """ Dataclass that contains data ranges
     """
@@ -101,43 +102,43 @@
         """ Return logarithmic norm from ranges
         """
         return LogNorm(
             vmin=np.log10(np.nanmin(self._collector.zminpos)), 
             vmax=np.log10(np.nanmax(self._collector.zmax))
         )
 
-def ListToGrid(data, ncols, missing=None, transpose=False):
-    """
-    Enumerate given data with an index and row/column number specified by number of columns
-
-    :param list data: Any iterable data, e.g. list, array
-    :param int ncols: Number of grid columns
-    :param bool missing: List only missing grid points
-    :param bool transpose: Transpose grid layout from horizontal to vertical arrangement
-    """
-    ndata = len(data)
-    nrows = int(np.ceil(ndata/ncols))
-    if missing:
-        for i in range(ndata, ncols*nrows):
-            yield (i,int(i%nrows),int(i/nrows)) if transpose else (i,int(i/ncols),int(i%ncols))
-    else:
-        for i,d in enumerate(data):
-            yield (i,int(i%nrows),int(i/nrows),d) if transpose else (i,int(i/ncols),int(i%ncols),d)
-    
-def DictToGrid(data, ncols, missing=None, transpose=False):
-    """
-    Enumerate given data with an index and row/column number specified by number of columns
-
-    :param dict data: A Python dictionary with keys and values
-    :param int ncols: Number of grid columns
-    :param bool missing: List only missing grid points
-    :param bool transpose: Transpose grid layout from horizontal to vertical arrangement
-    """
-    ndata = len(data)
-    nrows = int(np.ceil(ndata/ncols))
-    if missing:
-        for i in range(ndata, ncols*nrows):
-            yield (i,int(i%nrows),int(i/nrows)) if transpose else (i,int(i/ncols),int(i%ncols))
-    else:
-        for i,(k,v) in enumerate(data.items()):
-            yield (i,int(i%nrows),int(i/nrows),k,v) if transpose else (i,int(i/ncols),int(i%ncols),k,v)
-    
+class DataPlotGrid:
+    data: Union[list,dict]
+    ndata: int
+    ncols: int
+    nrows: int
+    figsize: tuple
+
+    def __init__(self, data: Union[list,dict], ncols:int=2, axsize:tuple=(4,2)):
+        self.data = data
+        self.ndata = len(data)
+        self.ncols = ncols
+        self.nrows = int(np.ceil(self.ndata/self.ncols))
+        self.figsize = (self.ncols*axsize[0], self.nrows*axsize[1])
+
+    def items(self, missing:bool=None, transpose:bool=False):
+        if missing:
+            for i in range(self.ndata, self.ncols*self.nrows):
+                if transpose:
+                    yield (i,int(i%self.nrows),int(i/self.nrows))
+                else:
+                    yield (i,int(i/self.ncols),int(i%self.ncols))
+        else:
+            if isinstance(self.data, list):
+                for i,d in enumerate(self.data):
+                    if transpose:
+                        yield (i,int(i%self.nrows),int(i/self.nrows),d)
+                    else:
+                        yield (i,int(i/self.ncols),int(i%self.ncols),d)
+            elif isinstance(self.data, dict):
+                for i,(k,v) in enumerate(self.data.items()):
+                    if transpose:
+                        yield (i,int(i%self.nrows),int(i/self.nrows),k,v)
+                    else:
+                        yield (i,int(i/self.ncols),int(i%self.ncols),k,v)
+            else:
+                raise Exception('Wrong data type:', self.data)
```

### Comparing `scinumtools-1.6.7/tests/src/scinumtools/math/solver/AtomClass.py` & `scinumtools-1.7.0/tests/src/scinumtools/math/solver/AtomClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.7/tests/src/scinumtools/math/solver/ExpressionClass.py` & `scinumtools-1.7.0/tests/src/scinumtools/math/solver/ExpressionClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.7/tests/src/scinumtools/math/solver/OperatorClass.py` & `scinumtools-1.7.0/tests/src/scinumtools/math/solver/OperatorClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.7/tests/src/scinumtools/math/solver/SolverClass.py` & `scinumtools-1.7.0/tests/src/scinumtools/math/solver/SolverClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.7/tests/src/scinumtools/math/solver/TokensClass.py` & `scinumtools-1.7.0/tests/src/scinumtools/math/solver/TokensClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.7/tests/src/scinumtools/phys/ConstantsClass.py` & `scinumtools-1.7.0/tests/src/scinumtools/phys/ConstantsClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.7/tests/src/scinumtools/phys/units/QuantityClass.py` & `scinumtools-1.7.0/tests/src/scinumtools/phys/units/QuantityClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.7/tests/src/scinumtools/phys/units/UnitConverters.py` & `scinumtools-1.7.0/tests/src/scinumtools/phys/units/UnitConverters.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.7/tests/src/scinumtools/phys/units/UnitList.py` & `scinumtools-1.7.0/tests/src/scinumtools/phys/units/UnitList.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.7/tests/src/scinumtools/stats/StopwatchClass.py` & `scinumtools-1.7.0/tests/src/scinumtools/stats/StopwatchClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.7/tests/src/scinumtools/structs/CollectorClass.py` & `scinumtools-1.7.0/src/scinumtools/structs/CollectorClass.py`

 * *Files 16% similar despite different names*

```diff
@@ -29,14 +29,17 @@
         pass
     
     def __init__(self, columns: list):
         self._columns = []
         for column in columns:
             setattr(self,column,[])
             self._columns.append(column)
+
+    def __str__(self):
+        return self.to_text()
         
     def append(self, values: list):
         """ Append a single row
 
         :param values: List of values for each column
         """
         for n, name in enumerate(self._columns):
@@ -48,14 +51,22 @@
         :param str name: name of the sorting column
         :param bool reverse: reverse order
         """
         ids = np.argsort(getattr(self, name))
         if reverse: ids = ids[::-1]
         for n, name in enumerate(self._columns):
             setattr(self,name,list(np.array(getattr(self, name))[ids]))
+
+    def size(self):
+        """ Get number of items in columns
+        """
+        if self._columns:
+            return len(getattr(self, self._columns[0]))
+        else:
+            return 0
             
     def to_dict(self):
         """ Convert class data to a dictionary of lists/arrays
         """
         data = {}
         for name in self._columns:
             data[name] = getattr(self,name)
@@ -86,15 +97,15 @@
 
     Example of use:
 
     ..code-block::
     
         import scinumtools as snt
         
-        with snt.structs.RowCollector(['col1','col2','col3']) as rc:
+        with snt.structs.ArrayCollector(['col1','col2','col3']) as rc:
              rc.append([1,2,3])
              rc.append([4,5,6])
              data = rc.to_dict()
     
     :param columns: This can be either a list of column names or a dictionary with column array settings
     """
     _columns: list
@@ -112,14 +123,17 @@
                 setattr(self,column,np.array([],**kwargs))
                 self._columns.append(column)
         else:
             for column in columns:
                 setattr(self,column,np.array([]))
                 self._columns.append(column)
 
+    def __str__(self):
+        return self.to_text()
+    
     def append(self, values: list):
         """ Append a single row
 
         :param values: List of values for each column
         """
         for n, name in enumerate(self._columns):
             data = getattr(self,name)
@@ -132,14 +146,22 @@
         :param str name: name of the sorting column
         """
         ids = np.argsort(getattr(self, name))
         if reverse: ids = ids[::-1]
         for n, name in enumerate(self._columns):
             setattr(self,name,getattr(self, name)[ids])
             
+    def size(self):
+        """ Get number of items in columns
+        """
+        if self._columns:
+            return len(getattr(self, self._columns[0]))
+        else:
+            return 0
+        
     def to_dict(self):
         """ Convert class data to a dictionary of lists/arrays
         """
         data = {}
         for name in self._columns:
             data[name] = getattr(self,name)
         return data
```

### Comparing `scinumtools-1.6.7/tests/src/scinumtools/structs/ParameterClass.py` & `scinumtools-1.7.0/tests/src/scinumtools/structs/ParameterClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.7/.gitignore` & `scinumtools-1.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `scinumtools-1.6.7/pyproject.toml` & `scinumtools-1.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "scinumtools"
-version = "1.6.7"
+version = "1.7.0"
 authors = [
   { name="Ondrej Pego Jaura", email="vrtulka23@pm.me" },
 ]
 description = "Set of most frequently used tools for a rapid numerical code development in Python."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `scinumtools-1.6.7/PKG-INFO` & `scinumtools-1.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scinumtools
-Version: 1.6.7
+Version: 1.7.0
 Summary: Set of most frequently used tools for a rapid numerical code development in Python.
 Project-URL: Homepage, https://github.com/vrtulka23/scinumtools
 Project-URL: Bug Tracker, https://github.com/vrtulka23/scinumtools/issues
 Author-email: Ondrej Pego Jaura <vrtulka23@pm.me>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

