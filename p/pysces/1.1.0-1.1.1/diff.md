# Comparing `tmp/pysces-1.1.0.tar.gz` & `tmp/pysces-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysces-1.1.0.tar", last modified: Wed Apr 19 11:19:30 2023, max compression
+gzip compressed data, was "pysces-1.1.1.tar", last modified: Tue Jul 25 18:11:52 2023, max compression
```

## Comparing `pysces-1.1.0.tar` & `pysces-1.1.1.tar`

### file list

```diff
@@ -1,138 +1,138 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:19:30.458885 pysces-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-19 11:19:27.000000 pysces-1.1.0/ADDITIONAL_LICENCES.md
--rw-r--r--   0 runner    (1001) docker     (123)     9978 2023-04-19 11:19:27.000000 pysces-1.1.0/CHANGES.md
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-19 11:19:27.000000 pysces-1.1.0/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-19 11:19:27.000000 pysces-1.1.0/CONTRIBUTORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-04-19 11:19:27.000000 pysces-1.1.0/INSTALL.md
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-19 11:19:27.000000 pysces-1.1.0/LATEST.md
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-04-19 11:19:27.000000 pysces-1.1.0/LICENCE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-04-19 11:19:27.000000 pysces-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-19 11:19:27.000000 pysces-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-04-19 11:19:30.458885 pysces-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-04-19 11:19:27.000000 pysces-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-19 11:19:27.000000 pysces-1.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:19:30.450885 pysces-1.1.0/pysces/
--rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/PyscesConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/PyscesContrib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/PyscesContribUser.py
--rw-r--r--   0 runner    (1001) docker     (123)     9360 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/PyscesInterfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    32019 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/PyscesJWSParse.py
--rw-r--r--   0 runner    (1001) docker     (123)    53189 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/PyscesLink.py
--rw-r--r--   0 runner    (1001) docker     (123)    19980 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/PyscesMiniModel.py
--rw-r--r--   0 runner    (1001) docker     (123)   349989 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/PyscesModel.py
--rw-r--r--   0 runner    (1001) docker     (123)    12084 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/PyscesModelMap.py
--rw-r--r--   0 runner    (1001) docker     (123)    13017 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/PyscesParScan.py
--rw-r--r--   0 runner    (1001) docker     (123)    57192 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/PyscesParse.py
--rw-r--r--   0 runner    (1001) docker     (123)    31204 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/PyscesPlot.py
--rw-r--r--   0 runner    (1001) docker     (123)    53012 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/PyscesPlot2.py
--rw-r--r--   0 runner    (1001) docker     (123)    32648 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/PyscesRandom.py
--rw-r--r--   0 runner    (1001) docker     (123)    30871 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/PyscesSBML.py
--rw-r--r--   0 runner    (1001) docker     (123)    18256 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/PyscesSED.py
--rw-r--r--   0 runner    (1001) docker     (123)    20294 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/PyscesScan.py
--rw-r--r--   0 runner    (1001) docker     (123)    56341 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/PyscesStoich.py
--rw-r--r--   0 runner    (1001) docker     (123)    34243 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/PyscesTest.py
--rw-r--r--   0 runner    (1001) docker     (123)    12587 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/PyscesUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14492 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/PyscesWeb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)    57145 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/RateChar.py
--rw-r--r--   0 runner    (1001) docker     (123)    18277 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/_multicorescan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:19:30.450885 pysces-1.1.0/pysces/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/contrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:19:30.450885 pysces-1.1.0/pysces/contrib/demo/
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/contrib/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/contrib/demo/demotest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:19:30.450885 pysces-1.1.0/pysces/core2/
--rw-r--r--   0 runner    (1001) docker     (123)    18572 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/core2/InfixParser.py
--rw-r--r--   0 runner    (1001) docker     (123)    55235 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/core2/PyscesCore2.py
--rw-r--r--   0 runner    (1001) docker     (123)    81721 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/core2/PyscesCore2Interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    24562 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/core2/PyscesCore2Modules.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/core2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42905 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/core2/lex.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/core2/version.py
--rw-r--r--   0 runner    (1001) docker     (123)   137736 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/core2/yacc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:19:30.450885 pysces-1.1.0/pysces/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/docs/DOCS.txt
--rw-r--r--   0 runner    (1001) docker     (123)    26145 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/docs/HISTORY.txt
--rw-r--r--   0 runner    (1001) docker     (123)   488229 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/docs/userguide.pdf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:19:30.454885 pysces-1.1.0/pysces/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/examples/benchmark.ipy
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/examples/parallelscan.ipy
--rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/examples/pysces_stochpy.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/examples/testRunScatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/examples/testinvalidstate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/examples/testparscanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/examples/testratechar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:19:30.454885 pysces-1.1.0/pysces/kraken/
--rw-r--r--   0 runner    (1001) docker     (123)    15458 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/kraken/Kraken.py
--rw-r--r--   0 runner    (1001) docker     (123)     6758 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/kraken/KrakenDataTools.py
--rw-r--r--   0 runner    (1001) docker     (123)    14998 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/kraken/KrakenNET.py
--rw-r--r--   0 runner    (1001) docker     (123)    11029 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/kraken/KrakenServer.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/kraken/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:19:30.454885 pysces-1.1.0/pysces/kraken/controllers/
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/kraken/controllers/kill_tentacles.py
--rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/kraken/controllers/kraken_continuation.py
--rw-r--r--   0 runner    (1001) docker     (123)    11564 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/kraken/controllers/kraken_continuation_eigen.py
--rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/kraken/controllers/kraken_continuation_eigen2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/kraken/controllers/kraken_intersect.py
--rw-r--r--   0 runner    (1001) docker     (123)    13710 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/kraken/controllers/kraken_scanner2.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/kraken/server_list
--rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/kraken/startup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:19:30.454885 pysces-1.1.0/pysces/lib/
--rw-r--r--   0 runner    (1001) docker     (123)     9861 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/lib/FirstDerivatives.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42905 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/lib/lex.py
--rw-r--r--   0 runner    (1001) docker     (123)   124351 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/lib/miriamids.py
--rw-r--r--   0 runner    (1001) docker     (123)   151642 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/lib/pyparsing.py
--rw-r--r--   0 runner    (1001) docker     (123)   137736 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/lib/yacc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:19:30.454885 pysces-1.1.0/pysces/metatool/
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/metatool/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:19:30.458885 pysces-1.1.0/pysces/nleq2/
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/nleq2/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/nleq2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18561 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/nleq2/linalg_nleq2.f
--rw-r--r--   0 runner    (1001) docker     (123)    55672 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/nleq2/nleq2-4.3.tar.gz
--rw-r--r--   0 runner    (1001) docker     (123)   127885 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/nleq2/nleq2.f
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/nleq2/nleq2.pyf
--rw-r--r--   0 runner    (1001) docker     (123)     5594 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/nleq2/nleq2_readme.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5594 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/nleq2/readme
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/nleq2/readme.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/nleq2/wnorm.f
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/nleq2/zibconst.f
--rw-r--r--   0 runner    (1001) docker     (123)    10975 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/nleq2/zibmon.f
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/nleq2/zibsec.f
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:19:30.458885 pysces-1.1.0/pysces/pitcon/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/pitcon/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/pitcon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   132416 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/pitcon/dpcon61.f
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/pitcon/dpcon61w.f
--rw-r--r--   0 runner    (1001) docker     (123)    30665 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/pitcon/pcon61subd.f
--rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/pitcon/pitcon.pyf
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/pitcon/readme.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:19:30.458885 pysces-1.1.0/pysces/pscmodels/
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/pscmodels/Burstmodel.psc
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/pscmodels/isola2a.psc
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/pscmodels/lin5_hill.psc
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/pscmodels/noisy_lin4.psc.txt
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/pscmodels/pysces_test_branch1.psc
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/pscmodels/pysces_test_linear1.psc
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/pscmodels/pysces_test_moiety1.psc
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/pscmodels/pysces_test_pitcon.psc
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-19 11:19:30.000000 pysces-1.1.0/pysces/pyscfg.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:19:30.458885 pysces-1.1.0/pysces/sandbox/
--rw-r--r--   0 runner    (1001) docker     (123)    12084 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/sandbox/Intersect.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/sandbox/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:19:30.458885 pysces-1.1.0/pysces/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/version.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:19:30.450885 pysces-1.1.0/pysces.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-04-19 11:19:30.000000 pysces-1.1.0/pysces.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-04-19 11:19:30.000000 pysces-1.1.0/pysces.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 11:19:30.000000 pysces-1.1.0/pysces.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 11:19:30.000000 pysces-1.1.0/pysces.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-19 11:19:30.000000 pysces-1.1.0/pysces.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-19 11:19:30.000000 pysces-1.1.0/pysces.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-19 11:19:27.000000 pysces-1.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 11:19:30.458885 pysces-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     8182 2023-04-19 11:19:27.000000 pysces-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:11:52.844620 pysces-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-25 18:11:43.000000 pysces-1.1.1/ADDITIONAL_LICENCES.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9978 2023-07-25 18:11:43.000000 pysces-1.1.1/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-25 18:11:43.000000 pysces-1.1.1/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-25 18:11:43.000000 pysces-1.1.1/CONTRIBUTORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-07-25 18:11:43.000000 pysces-1.1.1/INSTALL.md
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-25 18:11:43.000000 pysces-1.1.1/LATEST.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-25 18:11:43.000000 pysces-1.1.1/LICENCE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-07-25 18:11:43.000000 pysces-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-25 18:11:43.000000 pysces-1.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-07-25 18:11:52.844620 pysces-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-07-25 18:11:43.000000 pysces-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-25 18:11:43.000000 pysces-1.1.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:11:52.824620 pysces-1.1.1/pysces/
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/PyscesConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/PyscesContrib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/PyscesContribUser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9394 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/PyscesInterfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32019 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/PyscesJWSParse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53189 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/PyscesLink.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19980 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/PyscesMiniModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)   352475 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/PyscesModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12084 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/PyscesModelMap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13017 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/PyscesParScan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57192 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/PyscesParse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31204 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/PyscesPlot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53254 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/PyscesPlot2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32648 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/PyscesRandom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30871 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/PyscesSBML.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18256 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/PyscesSED.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20424 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/PyscesScan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56341 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/PyscesStoich.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34243 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/PyscesTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12593 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/PyscesUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14492 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/PyscesWeb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    57145 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/RateChar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18704 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/_multicorescan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:11:52.828620 pysces-1.1.1/pysces/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:11:52.828620 pysces-1.1.1/pysces/contrib/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/contrib/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/contrib/demo/demotest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:11:52.828620 pysces-1.1.1/pysces/core2/
+-rw-r--r--   0 runner    (1001) docker     (123)    18572 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/core2/InfixParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55235 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/core2/PyscesCore2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82319 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/core2/PyscesCore2Interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24562 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/core2/PyscesCore2Modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/core2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42905 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/core2/lex.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/core2/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)   137736 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/core2/yacc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:11:52.832620 pysces-1.1.1/pysces/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/docs/DOCS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    26145 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/docs/HISTORY.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   488229 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/docs/userguide.pdf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:11:52.832620 pysces-1.1.1/pysces/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/examples/benchmark.ipy
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/examples/parallelscan.ipy
+-rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/examples/pysces_stochpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/examples/testRunScatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/examples/testinvalidstate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/examples/testparscanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/examples/testratechar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:11:52.836620 pysces-1.1.1/pysces/kraken/
+-rw-r--r--   0 runner    (1001) docker     (123)    15458 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/kraken/Kraken.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6758 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/kraken/KrakenDataTools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14998 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/kraken/KrakenNET.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11029 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/kraken/KrakenServer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/kraken/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:11:52.836620 pysces-1.1.1/pysces/kraken/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/kraken/controllers/kill_tentacles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/kraken/controllers/kraken_continuation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11564 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/kraken/controllers/kraken_continuation_eigen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/kraken/controllers/kraken_continuation_eigen2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/kraken/controllers/kraken_intersect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13710 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/kraken/controllers/kraken_scanner2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/kraken/server_list
+-rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/kraken/startup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:11:52.836620 pysces-1.1.1/pysces/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     9861 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/lib/FirstDerivatives.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42905 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/lib/lex.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124351 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/lib/miriamids.py
+-rw-r--r--   0 runner    (1001) docker     (123)   151642 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/lib/pyparsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)   137736 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/lib/yacc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:11:52.836620 pysces-1.1.1/pysces/metatool/
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/metatool/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:11:52.840620 pysces-1.1.1/pysces/nleq2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/nleq2/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/nleq2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18561 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/nleq2/linalg_nleq2.f
+-rw-r--r--   0 runner    (1001) docker     (123)    55672 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/nleq2/nleq2-4.3.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (123)   127885 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/nleq2/nleq2.f
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/nleq2/nleq2.pyf
+-rw-r--r--   0 runner    (1001) docker     (123)     5594 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/nleq2/nleq2_readme.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5594 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/nleq2/readme
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/nleq2/readme.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/nleq2/wnorm.f
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/nleq2/zibconst.f
+-rw-r--r--   0 runner    (1001) docker     (123)    10975 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/nleq2/zibmon.f
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/nleq2/zibsec.f
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:11:52.840620 pysces-1.1.1/pysces/pitcon/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/pitcon/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/pitcon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   132416 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/pitcon/dpcon61.f
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/pitcon/dpcon61w.f
+-rw-r--r--   0 runner    (1001) docker     (123)    30665 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/pitcon/pcon61subd.f
+-rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/pitcon/pitcon.pyf
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/pitcon/readme.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:11:52.844620 pysces-1.1.1/pysces/pscmodels/
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/pscmodels/Burstmodel.psc
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/pscmodels/isola2a.psc
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/pscmodels/lin5_hill.psc
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/pscmodels/noisy_lin4.psc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/pscmodels/pysces_test_branch1.psc
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/pscmodels/pysces_test_linear1.psc
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/pscmodels/pysces_test_moiety1.psc
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/pscmodels/pysces_test_pitcon.psc
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-25 18:11:52.000000 pysces-1.1.1/pysces/pyscfg.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:11:52.844620 pysces-1.1.1/pysces/sandbox/
+-rw-r--r--   0 runner    (1001) docker     (123)    12084 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/sandbox/Intersect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/sandbox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:11:52.844620 pysces-1.1.1/pysces/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-25 18:11:43.000000 pysces-1.1.1/pysces/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:11:52.828620 pysces-1.1.1/pysces.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-07-25 18:11:52.000000 pysces-1.1.1/pysces.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-07-25 18:11:52.000000 pysces-1.1.1/pysces.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 18:11:52.000000 pysces-1.1.1/pysces.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 18:11:52.000000 pysces-1.1.1/pysces.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-25 18:11:52.000000 pysces-1.1.1/pysces.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-25 18:11:52.000000 pysces-1.1.1/pysces.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-25 18:11:43.000000 pysces-1.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 18:11:52.844620 pysces-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7177 2023-07-25 18:11:43.000000 pysces-1.1.1/setup.py
```

### Comparing `pysces-1.1.0/ADDITIONAL_LICENCES.md` & `pysces-1.1.1/ADDITIONAL_LICENCES.md`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/CHANGES.md` & `pysces-1.1.1/CHANGES.md`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/CONTRIBUTORS.md` & `pysces-1.1.1/CONTRIBUTORS.md`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/INSTALL.md` & `pysces-1.1.1/INSTALL.md`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/LATEST.md` & `pysces-1.1.1/LATEST.md`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/LICENCE.txt` & `pysces-1.1.1/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/LICENSE` & `pysces-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/MANIFEST.in` & `pysces-1.1.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/PKG-INFO` & `pysces-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysces
-Version: 1.1.0
+Version: 1.1.1
 Summary: The Python Simulator for Cellular Systems - simulation and analysis tools for modelling biological systems
 Home-page: http://pysces.sourceforge.net
 Download-URL: https://pypi.org/project/pysces/#files
 Author: Brett G. Olivier and Johann M. Rohwer
 Author-email: pysces@googlegroups.com
 Maintainer: Brett G. Olivier and Johann M. Rohwer
 Maintainer-email: pysces@googlegroups.com
```

### Comparing `pysces-1.1.0/README.md` & `pysces-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/PyscesContrib.py` & `pysces-1.1.1/pysces/PyscesContrib.py`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/PyscesContribUser.py` & `pysces-1.1.1/pysces/PyscesContribUser.py`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/PyscesInterfaces.py` & `pysces-1.1.1/pysces/PyscesInterfaces.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,28 +115,29 @@
         self,
         mod,
         filename=None,
         directory=None,
         iValues=True,
         getdocument=False,
         getstrbuf=False,
+        debug=False,
     ):
         """
         Writes a PySCeS model object to an SBML file.
 
         - *filename*: writes <filename>.xml or <model_name>.xml if None
         - *directory*: (optional) an output directory
         - *iValues*: if True then the models initial values are used (or the current values if False).
         - *getdocument*: if True an SBML document object is returned instead of writing to disk or
         - *getstrbuf*: if True a StringIO buffer is returned instead of writing to disk
         """
         self.core = NewCore(mod, iValues=iValues)
         ##  assert os.sys.platform != 'win32', '\nSBML translation currently only supported on Linux (Mac?)'
         assert self.core != None, "\nPlease set a PySCeS model or Core2 object"
-        self.core2sbml = CoreToSBML(self.core)
+        self.core2sbml = CoreToSBML(self.core, debug=debug)
         self.core2sbml.level = self.sbml_level
         self.core2sbml.version = self.sbml_version
         assert self.core2sbml.SBML != None, "\nProblems loading SBML/Python interface"
         self.__buildSbmlComponents__()
         if filename == None:
             filename = self.core.name
         if filename[-4:] != '.xml':
```

### Comparing `pysces-1.1.0/pysces/PyscesJWSParse.py` & `pysces-1.1.1/pysces/PyscesJWSParse.py`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/PyscesLink.py` & `pysces-1.1.1/pysces/PyscesLink.py`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/PyscesMiniModel.py` & `pysces-1.1.1/pysces/PyscesMiniModel.py`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/PyscesModel.py` & `pysces-1.1.1/pysces/PyscesModel.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,17 +28,16 @@
             PyscesModel
             -----------
 
             This module contains the core PySCeS classes which
             create the model and associated data objects
 
             '''
-import os, copy, gc, time
-import math, operator, re
-import pprint, pickle, io
+import os, copy, time
+import pickle
 import warnings
 try:
     input = raw_input  # Py2 compatibility
 except NameError:
     pass
 import numpy
 import scipy
@@ -76,15 +75,17 @@
     pitcon,
     plt,
     gplt,
     PyscesStoich,
     PyscesParse,
     __SILENT_START__,
     __CHGDIR_ON_START__,
+    __CUSTOM_DATATYPE__,
     SED,
+    _checkPandas,
 )
 
 if __CHGDIR_ON_START__:
     CWD = OUTPUT_DIR
 else:
     CWD = os.getcwd()
 
@@ -100,20 +101,19 @@
 del random.SystemRandom, random.WichmannHill, random.triangular
 # used by functions random.NV_MAGICCONST, random.SG_MAGICCONST, random.BPF, random.RECIP_BPF
 
 
 # Scipy version check
 if (
     int(scipy.__version__.split('.')[0]) < 1
-    and int(scipy.__version__.split('.')[1]) < 6
 ):
     print(
         '\nINFO: Your version of SciPy ('
         + scipy.version.version
-        + ') might be too old\n\tVersion 0.6.x or newer is strongly recommended\n'
+        + ') might be too old\n\tVersion 1.0.x or newer is strongly recommended\n'
     )
 else:
     if not __SILENT_START__:
         print(
             'You are using NumPy ({}) with SciPy ({})'.format(
                 numpy.__version__, scipy.__version__
             )
@@ -168,43 +168,46 @@
             sequence = self.setSequence(event_list)
             for ev in sequence:
                 if ev._assign_now:
                     print('executing', ev.name)
                     for ass in ev.assignments:
                         ass.evaluateAssignment()
                         if ass.variable in self.mod.L0matrix.getLabels()[1] or (
-                            self.mod.mode_integrate_all_odes
-                            and ass.variable in self.mod.__species__
+                            self.mod.mode_integrate_all_odes and ass.variable in self.mod.__species__
                         ):
                             assVal = ass.getValue()
                             assIdx = self.mod.__species__.index(ass.variable)
-                            if self.mod.__KeyWords__["Species_In_Conc"]:
+                            if self.mod.__KeyWords__['Species_In_Conc']:
                                 solver.y[assIdx] = assVal * getattr(
                                     self.mod, self.mod.__CsizeAllIdx__[assIdx]
                                 )
-                                setattr(self.mod, ass.variable, assVal * getattr(
-                                    self.mod, self.mod.__CsizeAllIdx__[assIdx]))
+                                setattr(
+                                    self.mod,
+                                    ass.variable,
+                                    assVal * getattr(self.mod, self.mod.__CsizeAllIdx__[assIdx]),
+                                )
                             else:
                                 solver.y[assIdx] = assVal
                                 setattr(self.mod, ass.variable, assVal)
                         elif (
                             not self.mod.mode_integrate_all_odes
                             and ass.variable in self.mod.L0matrix.getLabels()[0]
                         ):
                             print(
-                                'Event assignment to dependent species consider setting "mod.mode_integrate_all_odes = True"'
+                                'Event assignment to dependent species!\nConsider setting "mod.mode_integrate_all_odes = True"'
                             )
                             setattr(self.mod, ass.variable, ass.value)
-                        elif (
-                            self.mod.__HAS_RATE_RULES__ and ass.variable in self.mod.__rate_rules__
-                        ):
+                        elif self.mod.__HAS_RATE_RULES__ and ass.variable in self.mod.__rate_rules__:
+                            assert (
+                                self.mod.mode_integrate_all_odes
+                            ), 'Assigning events to RateRules requires integrating all ODEs.\n Set "mod.mode_integrate_all_odes = True"'
                             assVal = ass.getValue()
                             rrIdx = self.mod.__rate_rules__.index(ass.variable)
                             self.mod.__rrule__[rrIdx] = assVal
-                            solver.y[self.mod.L0matrix.shape[1] + rrIdx] = assVal
+                            solver.y[self.mod.Nmatrix.shape[0] + rrIdx] = assVal
                             setattr(self.mod, ass.variable, assVal)
                         else:
                             ass()
                             setattr(self.mod, ass.variable, ass.value)
                 # track any parameter changes
                 self.parvals.append([getattr(self.mod, p) for p in self.mod.parameters])
 
@@ -1465,24 +1468,59 @@
             self.LoadFromString(File, fString)
         else:
             self.LoadFromFile(File, dir)
         # stuff that needs to be done before initmodel
         self.__settings__['mode_substitute_assignment_rules'] = False
         self.__settings__['cvode_track_assignment_rules'] = True
         self.__settings__['display_compartment_warnings'] = False
+        self.__settings__['custom_datatype'] = __CUSTOM_DATATYPE__
         self._TIME_ = 0.0  # this will be the built-in time
         self.piecewise_functions = []
         self.__piecewises__ = {}
         self.__HAS_PIECEWISE__ = False
+
         if autoload:
             self.ModelLoad()
             self.__PSC_auto_load = True
         else:
             self.__PSC_auto_load = False
 
+        # autoload a custom datatype ... currently pandas
+        if __CUSTOM_DATATYPE__ == 'pandas':
+            if _checkPandas():
+                self.enableDataPandas(True)
+            else:
+                self.enableDataPandas(False)
+
+    def enableDataPandas(self, var=True):
+        """
+        Toggle custom data type for `mod.sim` and `mod.scan` objects.
+
+        - *var* if True, return pandas DataFrame, else numpy recarray
+        """
+        if var:
+            try:
+                import pandas
+                self.__pandas = pandas
+                self.__settings__['custom_datatype'] = 'pandas'
+                print('Pandas output enabled.')
+            except ModuleNotFoundError:
+                print(
+                    '''
+        Pandas is not installed. Install with:
+            pip install pandas        or
+            conda install pandas
+        Unsetting custom datatype!
+                    '''
+                )
+                self.__settings__['custom_datatype'] = None
+        else:
+            self.__settings__['custom_datatype'] = None
+            print('Pandas output disabled.')
+
     def ModelLoad(self, stoich_load=0):
         """
         Load and instantiate a PySCeS model so that it can be used for further analyses. This function
         replaces the pre-0.7.1 doLoad() method.
 
         - *stoich_load* try to load a structural analysis saved with Stoichiometry_Save_Serial() (default=0)
 
@@ -3942,18 +3980,24 @@
                 for x in range(sim_res.shape[0]):
                     sim_res[x] = self._SpeciesAmountToConc(sim_res[x])
             if self.__HAS_RATE_RULES__:
                 sim_res = numpy.concatenate([sim_res, rrules], axis=1)
 
         if self.__settings__['cvode_return_event_timepoints']:
             self.sim_time = t
+            self._ev_idx = idx
         else:
-            tidx = [numpy.where(t==i)[0][0] for i in self.sim_time]
+            tidx = [numpy.where(t == i)[0][0] for i in self.sim_time]
             sim_res = sim_res[tidx]
             rates = rates[tidx]
+            self._ev_idx = (
+                [0]
+                + [numpy.min(numpy.where(self.sim_time >= i)) for i in problem.event_times]
+                + [len(t)]
+            )
 
         return sim_res, rates, True
 
     def CVODE_VPYTHON(self, s):
         """Future VPython hook for CVODE"""
         pass
 
@@ -4741,44 +4785,60 @@
             self.data_sim.setRules(rrules, self.__rate_rules__)
         if self._CVODE_XOUT:
             self._CVODE_xdata = numpy.zeros((len(self.sim_time), len(self._CVODE_extra_output)))
             # get assignment rules
             r = self.__rules__
             ars = {name: r[name] for name in r if r[name]['type'] == 'assignment'}
             # loop through extra output and evaluate from simulation data
-            for i in range(len(self._CVODE_extra_output)):
-                name = self._CVODE_extra_output[i]
+            # set parameters for each event in case they changed
+            for k in range(len(self._CVODE_extra_output)):
+                name = self._CVODE_extra_output[k]
                 self._update_assignment_rule_code(ars[name])
-                self._CVODE_xdata[:, i] = eval(ars[name]['data_sim_string'])
+                for i in range(len(self._ev_idx) - 1):
+                    for j in range(len(self.parameters)):
+                        setattr(self, self.parameters[j], self._problem.parvals[i][j])
+                    p = self._ev_idx[i]
+                    q = self._ev_idx[i + 1]
+                    self._CVODE_xdata[p:q, k] = eval(ars[name]['data_sim_string'])
                 self.data_sim.setXData(self._CVODE_xdata, lbls=self._CVODE_extra_output)
             self._CVODE_xdata = None
+
         if not simOK:
             print('Simulation failure')
         del sim_res
 
     def _update_assignment_rule_code(self, rule):
         replacements = []
         rule['data_sim_string'] = rule['code_string']
         for s in rule['symbols']:
-            if s in self.__reactions__ or s in self.__rules__ or s in self.__species__:
+            if (
+                s in self.__reactions__
+                or s in self.__rules__
+                or s in self.__species__
+            ):
                 # catch any _init so it doesn't get replaced
                 replacements.append((s + '_init', '_zzzz_'))
                 # replace symbol to get sim data
-                replacements.append(('self.' + s, 'self.data_sim.getSimData("' + s + '")[:,1]'))
+                replacements.append(
+                    ('self.' + s, 'self.data_sim.getSimData("' + s + '")[p:q,1]')
+                )
                 # revert the _init
                 replacements.append(('_zzzz_', s + '_init'))
 
         for old, new in replacements:
             rule['data_sim_string'] = rule['data_sim_string'].replace(old, new)
 
     @property
     def sim(self):
         if self._sim is None and self.data_sim is not None:
             data = self.data_sim.getAllSimData(lbls=True)
-            self._sim = numpy.rec.fromrecords(data[0], names=data[1])
+            if self.__settings__['custom_datatype'] == 'pandas':
+                self._sim = self.__pandas.DataFrame(data[0], columns=data[1])
+            else:
+                self._sim = numpy.rec.fromrecords(data[0], names=data[1])
         return self._sim
 
     def State(self):
         """
         State()
 
         PySCeS non-linear solver driver routine. Solve for a steady state using HYBRD/NLEQ2/FINTSLV
@@ -8944,17 +9004,22 @@
             self.scan_res = numpy.zeros((len(range1), len(self.scan_out) + 1))
         else:
             self.scan_res = numpy.array(result)
 
     @property
     def scan(self):
         if self._scan is None and self.scan_res is not None:
-            self._scan = numpy.rec.fromrecords(
-                self.scan_res, names=[self.scan_in] + self.scan_out
-            )
+            if self.__settings__['custom_datatype'] == 'pandas':
+                self._scan = self.__pandas.DataFrame(
+                    self.scan_res, columns=[self.scan_in] + self.scan_out
+                )
+            else:
+                self._scan = numpy.rec.fromrecords(
+                    self.scan_res, names=[self.scan_in] + self.scan_out
+                )
         return self._scan
 
     def Scan1Plot(self, plot=[], title=None, log=None, format='lines', filename=None):
         """
         Plot the results of a parameter scan generated with **Scan1()**
 
         - *plot* if empty mod.scan_out is used, otherwise any subset of mod.scan_out (default=[])
```

### Comparing `pysces-1.1.0/pysces/PyscesModelMap.py` & `pysces-1.1.1/pysces/PyscesModelMap.py`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/PyscesParScan.py` & `pysces-1.1.1/pysces/PyscesParScan.py`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/PyscesParse.py` & `pysces-1.1.1/pysces/PyscesParse.py`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/PyscesPlot.py` & `pysces-1.1.1/pysces/PyscesPlot.py`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/PyscesPlot2.py` & `pysces-1.1.1/pysces/PyscesPlot2.py`

 * *Files 0% similar despite different names*

```diff
@@ -779,14 +779,15 @@
         'qt4agg',
         'tkagg',
         'wx',
         'wxagg',
         'cocoaagg',
         'agg',
         'nbagg',
+        'module://ipympl.backend_nbagg',
         'cairo',
         'emf',
         'gdk',
         'pdf',
         'ps',
         'svg',
         'template',
@@ -801,14 +802,15 @@
         'qtagg',
         'qt4agg',
         'tkagg',
         'wx',
         'wxagg',
         'cocoaagg',
         'nbagg',
+        'module://ipympl.backend_nbagg',
     ]
 
     __NON_INTERACTIVE_BACKENDS__ = [
         'agg',
         'pdf',
         'ps',
         'svg',
@@ -821,17 +823,21 @@
             self.__WORK_DIR__ = work_dir
         else:
             self.__WORK_DIR__ = os.getcwd()
         try:
             import matplotlib
 
             if self.isnotebook():
-                backend = 'nbAgg'
+                try:
+                    import ipympl       # for jupyterlab
+                    backend = 'module://ipympl.backend_nbagg'
+                except ModuleNotFoundError:
+                    backend = 'nbAgg'   # for notebook if ipympl not installed
                 import pysces
-                pysces.__MATPLOTLIB_BACKEND__ = 'nbAgg'
+                pysces.__MATPLOTLIB_BACKEND__ = backend
 
             if backend.lower() in self.__INTERACTIVE_BACKENDS__:
                 matplotlib.use(backend)
                 self.__BACKEND__ = backend
                 if not __SILENT_START__:
                     print(('Matplotlib backend set to: \"{}\"'.format(backend)))
             elif backend.lower() in self.__NON_INTERACTIVE_BACKENDS__:
@@ -870,18 +876,16 @@
                 print(ex)
                 print(
                     "\nPySCeS defaults to matplotlib's TKagg backend if not specified \
                          in the user configuration file, set \"matplotlib_backend = <backend>\" "
                 )
 
         from matplotlib import pyplot
-        from matplotlib import pylab
 
-        ##  self.pyplot = pyplot
-        self.pyplot = pylab
+        self.pyplot = pyplot
         if self.__MODE_INTERACTIVE__:
             self.pyplot.ion()
         self._setNewFigureGenerator(self.MAX_OPEN_WINDOWS)
 
     def isnotebook(self):
         try:
             shell = get_ipython().__class__.__name__
```

### Comparing `pysces-1.1.0/pysces/PyscesRandom.py` & `pysces-1.1.1/pysces/PyscesRandom.py`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/PyscesSBML.py` & `pysces-1.1.1/pysces/PyscesSBML.py`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/PyscesSED.py` & `pysces-1.1.1/pysces/PyscesSED.py`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/PyscesScan.py` & `pysces-1.1.1/pysces/PyscesScan.py`

 * *Files 1% similar despite different names*

```diff
@@ -349,16 +349,14 @@
 
         - *stst* add steady-state data to output array
         - *lbls* return a tuple of (array, column_header_list)
 
         If *stst* is True output has dimensions [scan_parameters]+[state_species+state_flux]+[Useroutput]
         otherwise [scan_parameters]+[Useroutput].
         """
-        output_array = None
-        labels = []
         if stst:
             if self.HAS_USER_OUTPUT:
                 output_array = scipy.hstack(
                     [self.ScanSpace, self.SteadyStateResults, self.UserOutputResults]
                 )
                 labels = (
                     self.GenOrder
@@ -373,16 +371,18 @@
                 )
         else:
             output_array = scipy.hstack([self.ScanSpace, self.UserOutputResults])
             labels = self.GenOrder + self.UserOutputList
         if lbls:
             return output_array, labels
         else:
-            return output_array
-
+            if self.mod.__settings__['custom_datatype'] == 'pandas':
+                return self.mod._PysMod__pandas.DataFrame(output_array, columns=labels)
+            else:
+                return output_array
 
 class PITCONScanUtils(object):
     """
     Static Bifurcation Scanning utilities using PITCON, call with loaded model object.
     Hopefully nobody else was trying to use the older class as it was horrible. This new
     one is is leaner, meaner and pretty cool ;-)
     """
```

### Comparing `pysces-1.1.0/pysces/PyscesStoich.py` & `pysces-1.1.1/pysces/PyscesStoich.py`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/PyscesTest.py` & `pysces-1.1.1/pysces/PyscesTest.py`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/PyscesUtils.py` & `pysces-1.1.1/pysces/PyscesUtils.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 def str2bool(s):
     """
     Tries to convert a string to a Python boolean
 
     - *s* True if 'True', 'true' or'1' else False
 
     """
-    if s in ['True', 'true', '1']:
+    if s in ['True', 'true', '1', True]:
         return True
     else:
         return False
 
 
 class TimerBox:
     """
```

### Comparing `pysces-1.1.0/pysces/PyscesWeb.py` & `pysces-1.1.1/pysces/PyscesWeb.py`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/README.txt` & `pysces-1.1.1/pysces/README.txt`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/RateChar.py` & `pysces-1.1.1/pysces/RateChar.py`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/__init__.py` & `pysces-1.1.1/pysces/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,25 +39,25 @@
             terms of the PySceS (BSD style) license. See LICENSE.txt that came with
             this distribution for specifics.
 
             NO WARRANTY IS EXPRESSED OR IMPLIED.  USE AT YOUR OWN RISK.
             Copyright (C) 2004-2023 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
             """
 
-import os, time
-from pkg_resources import get_build_platform
+import os
+import time
 from . import PyscesConfig
 from . import PyscesParse
 from . import PyscesLink as link
 from . import PyscesSED as SED
 
 from .PyscesUtils import str2bool
 from .PyscesModelMap import ModelMap
+from .version import current_version_tuple
 
-# TODO get rid unused imports
 from .PyscesWeb import PyscesHTML
 
 html = PyscesHTML()
 
 DEBUG = False
 
 inipath = None
@@ -74,53 +74,46 @@
 
 extra_dll_dir = os.path.join(os.path.dirname(__file__), '.libs')
 if os.sys.platform == 'win32' and os.path.isdir(extra_dll_dir):
     os.environ["PATH"] += os.pathsep + extra_dll_dir
     if hasattr(os, 'add_dll_directory'):
         os.add_dll_directory(extra_dll_dir)
 
-if os.sys.platform == 'win32':
-    __PyscesConfigDefault = PyscesConfig.__DefaultWin
-else:
-    __PyscesConfigDefault = PyscesConfig.__DefaultPosix
+__PyscesConfigDefault = PyscesConfig.__DefaultConfig
 
 if DEBUG:
     print(time.strftime('1-%H:%M:%S'))
 
-eggdir = 'pysces-%s-py%s.%s-%s.egg' % (
-    __version__,
-    os.sys.version_info[0],
-    os.sys.version_info[1],
-    get_build_platform(),
-)
 for path in os.sys.path:
     chkPath = path.split(os.path.sep)[-1]
     if chkPath == 'pysces' and path != os.getcwd():
+        # for in-place development with setup.py develop (legacy)
         if os.path.isdir(os.path.join(path, 'pysces')):
-            # for in-place development with setup.py develop
             install_dir = os.path.join(path, 'pysces')
         else:
             install_dir = path
         inipath = os.path.join(install_dir, 'pyscfg.ini')
         break
-    elif chkPath == eggdir:
-        install_dir = os.path.join(path, 'pysces')
+    # for in-place development with setup.py develop (new)
+    elif '__editable__.pysces' in path:
+        MAJOR, MINOR, MICRO = current_version_tuple()
+        exec(
+            'import __editable___pysces_{}_{}_{}_finder as finder'.format(
+                MAJOR, MINOR, MICRO
+            )
+        )
+        install_dir = finder.MAPPING['pysces']
         inipath = os.path.join(install_dir, 'pyscfg.ini')
         break
 if inipath == None:
     for k in os.sys.path_importer_cache:
         if k.split(os.path.sep)[-1] == 'pysces':
             install_dir = k
             inipath = os.path.join(install_dir, 'pyscfg.ini')
             break
-        elif k.split(os.path.sep)[-1] == eggdir:
-            install_dir = os.path.join(k, 'pysces')
-            inipath = os.path.join(install_dir, 'pyscfg.ini')
-            break
-del eggdir
 if DEBUG:
     print(time.strftime('2-%H:%M:%S'))
 
 try:
     __config_dict = PyscesConfig.ReadConfig(inipath, config=__PyscesConfigDefault)
 except Exception as ex:
     if DEBUG:
@@ -146,69 +139,55 @@
         GNUPLOT_DIR = __config_dict[key]
         if GNUPLOT_DIR == 'None':
             GNUPLOT_DIR = None
     elif key == 'silentstart':
         __SILENT_START__ = str2bool(__config_dict[key])
     elif key == 'change_dir_on_start':
         __CHGDIR_ON_START__ = str2bool(__config_dict[key])
+    elif key == 'custom_datatype':
+        __CUSTOM_DATATYPE__ = __config_dict[key]
+        if __CUSTOM_DATATYPE__ == 'None':
+            __CUSTOM_DATATYPE__ = None
 assert inipath != None, '\nNo configuration file found'
 
 if DEBUG:
     print(time.strftime('3-%H:%M:%S'))
 
 __userdict = None
-if os.sys.platform != 'win32':
+# search for legacy Windows Pysces directory location
+if os.sys.platform == 'win32' and os.path.exists(
+    os.path.join(os.getenv('HOMEDRIVE') + os.path.sep, 'Pysces', '.pys_usercfg.ini')
+):
+    __userdict = PyscesConfig.ReadConfig(
+        os.path.join(
+            os.getenv('HOMEDRIVE') + os.path.sep, 'Pysces', '.pys_usercfg.ini'
+        ),
+        PyscesConfig.__DefaultConfigUsr,
+    )
+else:
     if os.path.exists(
         os.path.join(os.path.expanduser('~'), 'Pysces', '.pys_usercfg.ini')
     ):
         __userdict = PyscesConfig.ReadConfig(
             os.path.join(os.path.expanduser('~'), 'Pysces', '.pys_usercfg.ini'),
-            PyscesConfig.__DefaultPosixUsr,
+            PyscesConfig.__DefaultConfigUsr,
         )
     else:
         if not os.path.exists(os.path.join(os.path.expanduser('~'), 'Pysces')):
             os.makedirs(os.path.join(os.path.expanduser('~'), 'Pysces'))
         PyscesConfig.WriteConfig(
             os.path.join(os.path.expanduser('~'), 'Pysces', '.pys_usercfg.ini'),
-            config=PyscesConfig.__DefaultPosixUsr,
+            config=PyscesConfig.__DefaultConfigUsr,
             section='Pysces',
         )
         __userdict = PyscesConfig.ReadConfig(
             os.path.join(os.path.expanduser('~'), 'Pysces', '.pys_usercfg.ini'),
-            PyscesConfig.__DefaultPosixUsr,
-        )
-else:
-    if os.path.exists(
-        os.path.join(os.getenv('HOMEDRIVE') + os.path.sep, 'Pysces', '.pys_usercfg.ini')
-    ):
-        __userdict = PyscesConfig.ReadConfig(
-            os.path.join(
-                os.getenv('HOMEDRIVE') + os.path.sep, 'Pysces', '.pys_usercfg.ini'
-            ),
-            PyscesConfig.__DefaultWinUsr,
-        )
-    elif os.path.exists(
-        os.path.join(os.getenv('USERPROFILE'), 'Pysces', '.pys_usercfg.ini')
-    ):
-        __userdict = PyscesConfig.ReadConfig(
-            os.path.join(os.getenv('USERPROFILE'), 'Pysces', '.pys_usercfg.ini'),
-            PyscesConfig.__DefaultWinUsr,
-        )
-    else:
-        if not os.path.exists(os.path.join(os.getenv('USERPROFILE'), 'Pysces')):
-            os.makedirs(os.path.join(os.getenv('USERPROFILE'), 'Pysces'))
-        PyscesConfig.WriteConfig(
-            os.path.join(os.getenv('USERPROFILE'), 'Pysces', '.pys_usercfg.ini'),
-            config=PyscesConfig.__DefaultWinUsr,
-            section='Pysces',
-        )
-        __userdict = PyscesConfig.ReadConfig(
-            os.path.join(os.getenv('USERPROFILE'), 'Pysces', '.pys_usercfg.ini'),
-            PyscesConfig.__DefaultWinUsr,
+            PyscesConfig.__DefaultConfigUsr,
         )
+
 for key in __userdict:
     if key == 'output_dir':
         output_dir = __userdict[key]
         if not os.path.exists(__userdict[key]):
             os.makedirs(__userdict[key])
     elif key == 'model_dir':
         model_dir = __userdict[key]
@@ -224,14 +203,18 @@
         GNUPLOT_DIR = __userdict[key]
         if GNUPLOT_DIR == 'None':
             GNUPLOT_DIR = None
     elif key == 'silentstart':
         __SILENT_START__ = str2bool(__userdict[key])
     elif key == 'change_dir_on_start':
         __CHGDIR_ON_START__ = str2bool(__userdict[key])
+    elif key == 'custom_datatype':
+        __CUSTOM_DATATYPE__ = __userdict[key]
+        if __CUSTOM_DATATYPE__ == 'None':
+            __CUSTOM_DATATYPE__ = None
 assert output_dir != None, '\nNo output directory defined'
 assert model_dir != None, '\nNo model directory defined'
 
 # following is to get the full path when .pys_usercfg.ini specifies CWD as follows:
 # output_dir = ./
 backup_dir = os.getcwd()
 os.chdir(output_dir)
@@ -454,15 +437,52 @@
 except ImportError as ex:
     SBML = None
     if DEBUG:
         print(ex)
     if not __SILENT_START__:
         print("INFO: libSBML not installed, SBML support not available.")
 
+# custom datatype for mod.sim and mod.scan
+if __CUSTOM_DATATYPE__:
+    assert (
+        __CUSTOM_DATATYPE__ == 'pandas'
+    ), f'Custom datatype {__CUSTOM_DATATYPE__} not supported, only pandas is supported.'
+    if not __SILENT_START__:
+        print('INFO: Custom datatype set to pandas.')
+
+def _checkPandas():
+    try:
+        import pandas
+        return True
+    except ModuleNotFoundError:
+        print(
+            """
+Custom datatype set in configuration but pandas not installed. Install with:
+    pip install pandas        or
+    conda install pandas
+Unsetting custom datatype!
+            """
+        )
+        return False
+
+def enablePandas(var=True):
+    """
+    Enable pandas data type globally per session for `mod.sim` and `mod.scan` objects.
+
+    - *var* if True, return pandas DataFrame, else numpy recarray
+    """
+    if var and _checkPandas():
+        PyscesModel.__CUSTOM_DATATYPE__ = 'pandas'
+        print('Enabling pandas globally...')
+    else:
+        PyscesModel.__CUSTOM_DATATYPE__ = None
+        print('Disabling pandas globally...')
+
 # This has to come at the end
+from . import PyscesModel
 from .PyscesModel import PysMod as model
 from .PyscesModel import ScanDataObj as ScanDataObj
 
 PyscesModel.interface = interface
 from .PyscesTest import PyscesTest as test
 
 write = None
```

### Comparing `pysces-1.1.0/pysces/_multicorescan.py` & `pysces-1.1.1/pysces/_multicorescan.py`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/contrib/__init__.py` & `pysces-1.1.1/pysces/contrib/__init__.py`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/contrib/demo/demotest.py` & `pysces-1.1.1/pysces/contrib/demo/demotest.py`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/core2/InfixParser.py` & `pysces-1.1.1/pysces/core2/InfixParser.py`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/core2/PyscesCore2.py` & `pysces-1.1.1/pysces/core2/PyscesCore2.py`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/core2/PyscesCore2Interfaces.py` & `pysces-1.1.1/pysces/core2/PyscesCore2Interfaces.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 Brett G. Olivier
 """
 from __future__ import division, print_function
 from __future__ import absolute_import
 from __future__ import unicode_literals
 
 from .version import __version__
+from .PyscesCore2 import AssignmentRule
 
 import os, copy, re, time
 from getpass import getuser
 from xml.etree import ElementTree
 import io
 import itertools
 import numpy
@@ -602,15 +603,14 @@
     SBML = None
     level = 3
     version = 2
     model = None
     document = None
     time = None
     __events__ = None
-    __DEBUG__ = False
     UNINIT_DEFAULT = 1e-3
 
     NumpyToMathML = {
         'numpy.greater_equal': 'geq',
         'numpy.greater': 'gt',
         'numpy.less_equal': 'leq',
         'numpy.less': 'lt',
@@ -624,29 +624,28 @@
         'numpy.arctan': 'arctan',
         'numpy.sinh': 'sinh',
         'numpy.cosh': 'cosh',
         'numpy.tanh': 'tanh',
         'numpy.sin': 'sin',
         'numpy.cos': 'cos',
         'numpy.tan': 'tan',
+        'numpy.pi': 'pi',
         'math.log10': 'log',
         'math.log': 'ln',
         'numpy.floor': 'floor',
         'numpy.ceil': 'ceil',
         'numpy.sqrt': 'sqrt',
         'math.sqrt': 'sqrt',
         'math.exp': 'exp',
         'operator.eq': 'eq',
         'operator.ne': 'neq',
         'operator.gt': 'gt',
         'operator.ge': 'geq',
         'operator.lt': 'lt',
         'operator.le': 'leq',
-        'operator.eq': 'equal',
-        'operator.ne': 'neq',
         'self._piecewise_': 'piecewise',
         '_piecewise_': 'piecewise',
         'operator.not_': 'not',
         ' and ' : ' && ',
         ' or ' : ' || ',
 
     }
@@ -666,37 +665,37 @@
         'numpy.arctan',
         'numpy.sinh',
         'numpy.cosh',
         'numpy.tanh',
         'numpy.sin',
         'numpy.cos',
         'numpy.tan',
+        'numpy.pi',
         'math.log10',
         'math.log',
         'numpy.floor',
         'numpy.ceil',
         'numpy.sqrt',
         'math.sqrt',
         'math.exp',
         'operator.eq',
         'operator.ne',
         'operator.gt',
         'operator.ge',
         'operator.lt',
         'operator.le',
-        'operator.eq',
-        'operator.ne',
         'self._piecewise_',
         '_piecewise_',
         'operator.not_',
         ' and ',
         ' or ',
     ]
 
-    def __init__(self, core):
+    def __init__(self, core, debug):
+        self.__DEBUG__ = debug
         self.core = core
         self.name = self.core.getName().replace('.psc', '').replace('.xml', '')
         try:
             import libsbml as SBML
 
             self.SBML = SBML
         except Exception as e:
@@ -813,14 +812,16 @@
 
     def setSpecies(self):
         """
         Add the species definitions to the SBML model object:
 
         """
         for spe in self.core.species:
+            if self.__DEBUG__:
+                print('Adding species: %s' % spe.name)
             s = self.model.createSpecies()
             s.setId(spe.name)
             s.setName(spe.name)
             if not spe.hasCompartment() and len(self.core.compartments) == 1:
                 print(
                     'Warning: species %s does not have a compartment locating it in \"%s\"'
                     % (spe.getName(), self.core.compartments[0].getName())
@@ -861,36 +862,41 @@
             p.setId(par.name)
             p.setName(par.name)
 
             # check for None value with no value and assign a default
             #print('PAR', par.name, par())
             # TODO: sort out this ZeroDivision and parameter initialisation error in a more sophisticated way, for example, evaluation assignment rules on export.
             try:
-                if par() is None:
-                    print(
-                        'INFO: parameter \"{}\" not been defined setting to {}'.format(par.getName(), self.UNINIT_DEFAULT)
-                    )
-                    if par.name in self.core.__InitDict__ and self.core.__InitDict__[par.name] is None:
-                        self.core.__InitDict__[par.name] = self.UNINIT_DEFAULT
-                    par.value = par.value_initial = self.core.__InitDict__[par.name]
-                # check for uninitialise parameters that have a value
-                elif par.name in self.core.__InitDict__:
-                    print(
-                        'INFO: parameter \"{}\" not initialised setting to ({})'.format(par.name, par())
-                    )
-                    self.core.__InitDict__[par.name] = par()
-                    par.value = par.value_initial = self.core.__InitDict__[par.name]
+                if not isinstance(par, AssignmentRule):
+                    if self.__DEBUG__:
+                        print('Adding parameter: %s' % par.name)
+                    if par() is None:
+                        print(
+                            'INFO: parameter \"{}\" not been defined setting to {}'.format(par.getName(), self.UNINIT_DEFAULT)
+                        )
+                        if par.name in self.core.__InitDict__ and self.core.__InitDict__[par.name] is None:
+                            self.core.__InitDict__[par.name] = self.UNINIT_DEFAULT
+                        par.value = par.value_initial = self.core.__InitDict__[par.name]
+                    # check for uninitialise parameters that have a value
+                    elif par.name in self.core.__InitDict__:
+                        print(
+                            'INFO: parameter \"{}\" not initialised setting to ({})'.format(par.name, par())
+                        )
+                        self.core.__InitDict__[par.name] = par()
+                        par.value = par.value_initial = self.core.__InitDict__[par.name]
             except ZeroDivisionError:
                 print('INFO: parameter \"{}\"initialisation error setting to 0.0'.format(par.name))
                 par.value = par.value_initial = self.core.__InitDict__[par.name] = 0.0
 
 
 
             # first attempt, check for a formula ... could be done with introspection
             if hasattr(par, 'formula'):
+                if self.__DEBUG__:
+                    print('Adding assignment rule: %s' % par.name)
                 p.setConstant(False)
                 r = self.model.createAssignmentRule()
                 r.setVariable(par.name)
                 formula = (
                     par.code_string.split('=')[1].replace('self.', '').replace('()', '')
                 )
                 #print('LOOKATME PARSE ASSIGNMENT RULE line 861')
@@ -951,14 +957,16 @@
         strBuf.seek(0)
         mathMLout = strBuf.read()
         return self.SBML.readMathMLFromString(mathMLout)
 
     def setRules(self):
         """Set rate rules"""
         for rule in self.core.rate_rules:
+            if self.__DEBUG__:
+                print('Adding rate rule: %s' % rule.getName())
             RR = self.model.createRateRule()
             RR.setVariable(rule.getName())
             # replace PySCeS infix with libSBML infix
             form = rule.code_string.split('=')[1].replace('self.', '').replace('()', '')
             form = self.infixPSC2SBML(form)
             req_replacements = {}
             for symb in rule._names:
@@ -993,15 +1001,16 @@
             if rpar == None:
                 rpar = self.model.getSpecies(rule.getName())
             if rpar != None:
                 rpar.setConstant(False)
 
     def setFunctions(self):
         for func in self.core.functions:
-            #print(func)
+            if self.__DEBUG__:
+                print('Adding function: %s' % func.getName())
             FNC = self.model.createFunctionDefinition()
             FNC.setName(func.getName())
             FNC.setId(func.getName())
             form = func.code_string.split('=')[1].replace('self.', '').replace('()', '')
             #print(form)
             form = self.infixPSC2SBML(form)
             #print(form)
@@ -1078,15 +1087,16 @@
                 ASTnodeD = self.astSetCSymbolTime(ASTnodeD)
                 D = self.SBML.Delay(self.level, self.version)
                 D.setMath(ASTnodeD)
                 EV.setDelay(D)
 
     def setReactions(self):
         for rxn in self.core.reactions:
-            # print 'Adding reaction:', rxn.name
+            if self.__DEBUG__:
+                print('Adding reaction: %s' % rxn.name)
             SBML_R = self.model.createReaction()
             SBML_R.setId(rxn.name)
             SBML_R.setName(rxn.name)
             for s in rxn.substrates:
                 ##  print '\t' + rxn.name +' has substrate: ' + s.name + ' (%s)' % abs(rxn.stoichiometry[s.name])
                 if self.SBML.getLibSBMLVersion() < 40000:
                     sref = self.SBML.SpeciesReference(
```

### Comparing `pysces-1.1.0/pysces/core2/PyscesCore2Modules.py` & `pysces-1.1.1/pysces/core2/PyscesCore2Modules.py`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/core2/__init__.py` & `pysces-1.1.1/pysces/core2/__init__.py`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/core2/lex.py` & `pysces-1.1.1/pysces/core2/lex.py`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/core2/yacc.py` & `pysces-1.1.1/pysces/core2/yacc.py`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/docs/HISTORY.txt` & `pysces-1.1.1/pysces/docs/HISTORY.txt`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/docs/userguide.pdf` & `pysces-1.1.1/pysces/docs/userguide.pdf`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/examples/benchmark.ipy` & `pysces-1.1.1/pysces/examples/benchmark.ipy`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/examples/parallelscan.ipy` & `pysces-1.1.1/pysces/examples/parallelscan.ipy`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/examples/pysces_stochpy.py` & `pysces-1.1.1/pysces/examples/pysces_stochpy.py`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/examples/testRunScatter.py` & `pysces-1.1.1/pysces/examples/testRunScatter.py`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/examples/testinvalidstate.py` & `pysces-1.1.1/pysces/examples/testinvalidstate.py`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/examples/testparscanner.py` & `pysces-1.1.1/pysces/examples/testparscanner.py`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/examples/testratechar.py` & `pysces-1.1.1/pysces/examples/testratechar.py`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/kraken/Kraken.py` & `pysces-1.1.1/pysces/kraken/Kraken.py`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/kraken/KrakenDataTools.py` & `pysces-1.1.1/pysces/kraken/KrakenDataTools.py`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/kraken/KrakenNET.py` & `pysces-1.1.1/pysces/kraken/KrakenNET.py`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/kraken/KrakenServer.py` & `pysces-1.1.1/pysces/kraken/KrakenServer.py`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/kraken/__init__.py` & `pysces-1.1.1/pysces/kraken/__init__.py`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/kraken/controllers/kraken_continuation.py` & `pysces-1.1.1/pysces/kraken/controllers/kraken_continuation.py`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/kraken/controllers/kraken_continuation_eigen.py` & `pysces-1.1.1/pysces/kraken/controllers/kraken_continuation_eigen.py`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/kraken/controllers/kraken_continuation_eigen2.py` & `pysces-1.1.1/pysces/kraken/controllers/kraken_continuation_eigen2.py`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/kraken/controllers/kraken_intersect.py` & `pysces-1.1.1/pysces/kraken/controllers/kraken_intersect.py`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/kraken/controllers/kraken_scanner2.py` & `pysces-1.1.1/pysces/kraken/controllers/kraken_scanner2.py`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/kraken/startup.py` & `pysces-1.1.1/pysces/kraken/startup.py`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/lib/FirstDerivatives.py` & `pysces-1.1.1/pysces/lib/FirstDerivatives.py`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/lib/__init__.py` & `pysces-1.1.1/pysces/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/lib/lex.py` & `pysces-1.1.1/pysces/lib/lex.py`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/lib/miriamids.py` & `pysces-1.1.1/pysces/lib/miriamids.py`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/lib/pyparsing.py` & `pysces-1.1.1/pysces/lib/pyparsing.py`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/lib/yacc.py` & `pysces-1.1.1/pysces/lib/yacc.py`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/metatool/__init__.py` & `pysces-1.1.1/pysces/metatool/__init__.py`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/nleq2/CMakeLists.txt` & `pysces-1.1.1/pysces/nleq2/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/nleq2/__init__.py` & `pysces-1.1.1/pysces/nleq2/__init__.py`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/nleq2/linalg_nleq2.f` & `pysces-1.1.1/pysces/nleq2/linalg_nleq2.f`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/nleq2/nleq2-4.3.tar.gz` & `pysces-1.1.1/pysces/nleq2/nleq2-4.3.tar.gz`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/nleq2/nleq2.f` & `pysces-1.1.1/pysces/nleq2/nleq2.f`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/nleq2/nleq2.pyf` & `pysces-1.1.1/pysces/nleq2/nleq2.pyf`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/nleq2/nleq2_readme.txt` & `pysces-1.1.1/pysces/nleq2/nleq2_readme.txt`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/nleq2/readme` & `pysces-1.1.1/pysces/nleq2/readme`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/nleq2/readme.txt` & `pysces-1.1.1/pysces/nleq2/readme.txt`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/nleq2/wnorm.f` & `pysces-1.1.1/pysces/nleq2/wnorm.f`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/nleq2/zibconst.f` & `pysces-1.1.1/pysces/nleq2/zibconst.f`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/nleq2/zibmon.f` & `pysces-1.1.1/pysces/nleq2/zibmon.f`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/nleq2/zibsec.f` & `pysces-1.1.1/pysces/nleq2/zibsec.f`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/pitcon/CMakeLists.txt` & `pysces-1.1.1/pysces/pitcon/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/pitcon/dpcon61.f` & `pysces-1.1.1/pysces/pitcon/dpcon61.f`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/pitcon/dpcon61w.f` & `pysces-1.1.1/pysces/pitcon/dpcon61w.f`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/pitcon/pcon61subd.f` & `pysces-1.1.1/pysces/pitcon/pcon61subd.f`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/pitcon/pitcon.pyf` & `pysces-1.1.1/pysces/pitcon/pitcon.pyf`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/pitcon/readme.txt` & `pysces-1.1.1/pysces/pitcon/readme.txt`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/pscmodels/Burstmodel.psc` & `pysces-1.1.1/pysces/pscmodels/Burstmodel.psc`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/pscmodels/isola2a.psc` & `pysces-1.1.1/pysces/pscmodels/isola2a.psc`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/pscmodels/lin5_hill.psc` & `pysces-1.1.1/pysces/pscmodels/lin5_hill.psc`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/pscmodels/pysces_test_branch1.psc` & `pysces-1.1.1/pysces/pscmodels/pysces_test_branch1.psc`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/pscmodels/pysces_test_moiety1.psc` & `pysces-1.1.1/pysces/pscmodels/pysces_test_moiety1.psc`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/pscmodels/pysces_test_pitcon.psc` & `pysces-1.1.1/pysces/pscmodels/pysces_test_pitcon.psc`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/sandbox/Intersect.py` & `pysces-1.1.1/pysces/sandbox/Intersect.py`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces/tests/__init__.py` & `pysces-1.1.1/pysces/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/pysces.egg-info/PKG-INFO` & `pysces-1.1.1/pysces.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysces
-Version: 1.1.0
+Version: 1.1.1
 Summary: The Python Simulator for Cellular Systems - simulation and analysis tools for modelling biological systems
 Home-page: http://pysces.sourceforge.net
 Download-URL: https://pypi.org/project/pysces/#files
 Author: Brett G. Olivier and Johann M. Rohwer
 Author-email: pysces@googlegroups.com
 Maintainer: Brett G. Olivier and Johann M. Rohwer
 Maintainer-email: pysces@googlegroups.com
```

### Comparing `pysces-1.1.0/pysces.egg-info/SOURCES.txt` & `pysces-1.1.1/pysces.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pysces-1.1.0/setup.py` & `pysces-1.1.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,27 +25,24 @@
 with open('pysces/version.txt') as f:
     __version__ = f.read().strip()
 
 # avoid duplication
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
-import os, re
+import os
+import re
+import sysconfig
 
 try:
     import configparser  # Py 3
 except ImportError:
     import ConfigParser as configparser  # Py 2
 
 try:
-    print('Building an egg? %s.' % FRYING_EGGS)
-except:
-    FRYING_EGGS = False
-
-try:
     import setuptools
 
     print('setuptools is available.')
 except Exception as ex:
     print('setuptools not available.')
 
 try:
@@ -96,55 +93,26 @@
 
 mypackage_data = {}
 
 # add some model files into pscmodels
 mypackage_data['pysces.pscmodels'] = ['*.psc']
 
 # Default configurations for the pyscfg.ini files
-if os.sys.platform == 'win32':
-    if FRYING_EGGS:
-        eggdir = 'pysces-%s-py%s.%s-%s.egg' % (
-            __version__,
-            os.sys.version_info[0],
-            os.sys.version_info[1],
-            os.sys.platform,
-        )
-        installdir = os.path.join(
-            os.sys.prefix, 'lib', 'site-packages', eggdir, 'pysces'
-        )
-    else:
-        installdir = os.path.join(os.sys.prefix, 'lib', 'site-packages', 'pysces')
-    config = {
-        "install_dir": installdir,
-        "model_dir": os.path.join(os.getenv('USERPROFILE'), 'Pysces', 'psc'),
-        "output_dir": os.path.join(os.getenv('USERPROFILE'), 'Pysces'),
-        "gnuplot_dir": None,
-        "silentstart": False,
-        "change_dir_on_start": False,
-    }
-else:
-    if hasattr(os.sys, 'lib'):
-        lib = os.sys.lib
-    else:
-        lib = 'lib'
-    config = {
-        "install_dir": os.path.join(
-            os.sys.prefix,
-            lib,
-            "python%d.%d" % tuple(os.sys.version_info[:2]),
-            'site-packages',
-            'pysces',
-        ),
-        "model_dir": os.path.join(os.path.expanduser('~'), 'Pysces', 'psc'),
-        "output_dir": os.path.join(os.path.expanduser('~'), 'Pysces'),
-        "gnuplot_dir": None,
-        "silentstart": False,
-        "change_dir_on_start": False,
-    }
-
+config = {
+    "install_dir": os.path.join(
+        sysconfig.get_path('platlib'),
+        'pysces',
+    ),
+    "model_dir": os.path.join(os.path.expanduser('~'), 'Pysces', 'psc'),
+    "output_dir": os.path.join(os.path.expanduser('~'), 'Pysces'),
+    "gnuplot_dir": None,
+    "silentstart": False,
+    "change_dir_on_start": False,
+    "custom_datatype": None,
+}
 
 def writeConfig(local_path, config={}):
     cfgfile = open(os.path.join(local_path, 'pysces', 'pyscfg.ini'), 'w')
     cp = configparser.ConfigParser()
     # PySCeS internal setup
     cp.add_section('Pysces')
     for key in config:
```

