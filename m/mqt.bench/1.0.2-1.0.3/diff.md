# Comparing `tmp/mqt.bench-1.0.2.tar.gz` & `tmp/mqt.bench-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mqt.bench-1.0.2.tar", last modified: Sun Jul 23 19:21:22 2023, max compression
+gzip compressed data, was "mqt.bench-1.0.3.tar", last modified: Tue Jul 25 07:37:07 2023, max compression
```

## Comparing `mqt.bench-1.0.2.tar` & `mqt.bench-1.0.3.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:21:22.098525 mqt.bench-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:21:22.066524 mqt.bench-1.0.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/.github/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:21:22.066524 mqt.bench-1.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/.github/workflows/coverage.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/.github/workflows/mypy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/.github/workflows/release-drafter.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    16437 2023-07-23 19:21:22.098525 mqt.bench-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13781 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/config.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:21:22.070525 mqt.bench-1.0.2/img/
--rw-r--r--   0 runner    (1001) docker     (123)    21005 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/img/arch.png
--rw-r--r--   0 runner    (1001) docker     (123)    86005 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/img/level_1.png
--rw-r--r--   0 runner    (1001) docker     (123)    84500 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/img/level_2.png
--rw-r--r--   0 runner    (1001) docker     (123)    76051 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/img/level_3.png
--rw-r--r--   0 runner    (1001) docker     (123)   112485 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/img/level_4.png
--rw-r--r--   0 runner    (1001) docker     (123)    61137 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/img/mqt_dark.png
--rw-r--r--   0 runner    (1001) docker     (123)    57266 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/img/mqt_light.png
--rw-r--r--   0 runner    (1001) docker     (123)   196044 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/img/mqtbench.png
--rw-r--r--   0 runner    (1001) docker     (123)     4529 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-23 19:21:22.098525 mqt.bench-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:21:22.062524 mqt.bench-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:21:22.062524 mqt.bench-1.0.2/src/mqt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:21:22.074524 mqt.bench-1.0.2/src/mqt/bench/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/src/mqt/bench/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17832 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/src/mqt/bench/benchmark_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:21:22.074524 mqt.bench-1.0.2/src/mqt/bench/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/src/mqt/bench/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/src/mqt/bench/benchmarks/ae.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/src/mqt/bench/benchmarks/dj.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/src/mqt/bench/benchmarks/ghz.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/src/mqt/bench/benchmarks/graphstate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/src/mqt/bench/benchmarks/grover.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/src/mqt/bench/benchmarks/qaoa.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/src/mqt/bench/benchmarks/qft.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/src/mqt/bench/benchmarks/qftentangled.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:21:22.078524 mqt.bench-1.0.2/src/mqt/bench/benchmarks/qiskit_application_finance/
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/src/mqt/bench/benchmarks/qiskit_application_finance/portfolioqaoa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/src/mqt/bench/benchmarks/qiskit_application_finance/portfoliovqe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/src/mqt/bench/benchmarks/qiskit_application_finance/pricingcall.py
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/src/mqt/bench/benchmarks/qiskit_application_finance/pricingput.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:21:22.078524 mqt.bench-1.0.2/src/mqt/bench/benchmarks/qiskit_application_ml/
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/src/mqt/bench/benchmarks/qiskit_application_ml/qnn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:21:22.078524 mqt.bench-1.0.2/src/mqt/bench/benchmarks/qiskit_application_nature/
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/src/mqt/bench/benchmarks/qiskit_application_nature/groundstate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:21:22.078524 mqt.bench-1.0.2/src/mqt/bench/benchmarks/qiskit_application_optimization/
--rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/src/mqt/bench/benchmarks/qiskit_application_optimization/routing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/src/mqt/bench/benchmarks/qiskit_application_optimization/tsp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/src/mqt/bench/benchmarks/qpeexact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/src/mqt/bench/benchmarks/qpeinexact.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/src/mqt/bench/benchmarks/qwalk.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/src/mqt/bench/benchmarks/random.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/src/mqt/bench/benchmarks/realamprandom.py
--rw-r--r--   0 runner    (1001) docker     (123)     8807 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/src/mqt/bench/benchmarks/shor.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/src/mqt/bench/benchmarks/su2random.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/src/mqt/bench/benchmarks/twolocalrandom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/src/mqt/bench/benchmarks/vqe.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/src/mqt/bench/benchmarks/wstate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:21:22.094525 mqt.bench-1.0.2/src/mqt/bench/evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/src/mqt/bench/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/src/mqt/bench/evaluation/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123) 15925096 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/src/mqt/bench/evaluation/evaluation_data.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     8133 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/src/mqt/bench/evaluation/evaluation_visualization.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:21:22.094525 mqt.bench-1.0.2/src/mqt/bench/evaluation/results/
--rw-r--r--   0 runner    (1001) docker     (123)    16461 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/src/mqt/bench/evaluation/results/pie.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    19421 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/src/mqt/bench/evaluation/results/qubit_dist.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    24774 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/src/mqt/bench/evaluation/results/violins.pdf
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/src/mqt/bench/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8149 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/src/mqt/bench/qiskit_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    11132 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/src/mqt/bench/tket_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    12928 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/src/mqt/bench/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:21:22.094525 mqt.bench-1.0.2/src/mqt/benchviewer/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/src/mqt/benchviewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26632 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/src/mqt/benchviewer/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/src/mqt/benchviewer/main.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/src/mqt/benchviewer/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:21:22.098525 mqt.bench-1.0.2/src/mqt/benchviewer/static/
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/src/mqt/benchviewer/static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:21:22.098525 mqt.bench-1.0.2/src/mqt/benchviewer/static/files/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/src/mqt/benchviewer/static/files/MQTBench_all.zip
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:21:22.098525 mqt.bench-1.0.2/src/mqt/benchviewer/static/files/qasm_output/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/src/mqt/benchviewer/static/files/qasm_output/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    61137 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/src/mqt/benchviewer/static/mqt_dark.png
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/src/mqt/benchviewer/static/tum_logo.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:21:22.098525 mqt.bench-1.0.2/src/mqt/benchviewer/templates/
--rw-r--r--   0 runner    (1001) docker     (123)    16436 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/src/mqt/benchviewer/templates/benchmark_description.html
--rw-r--r--   0 runner    (1001) docker     (123)     7441 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/src/mqt/benchviewer/templates/description.html
--rw-r--r--   0 runner    (1001) docker     (123)    28150 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/src/mqt/benchviewer/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     7693 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/src/mqt/benchviewer/templates/legal.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:21:22.070525 mqt.bench-1.0.2/src/mqt.bench.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16437 2023-07-23 19:21:21.000000 mqt.bench-1.0.2/src/mqt.bench.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-07-23 19:21:22.000000 mqt.bench-1.0.2/src/mqt.bench.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 19:21:21.000000 mqt.bench-1.0.2/src/mqt.bench.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-23 19:21:21.000000 mqt.bench-1.0.2/src/mqt.bench.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-23 19:21:21.000000 mqt.bench-1.0.2/src/mqt.bench.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-23 19:21:21.000000 mqt.bench-1.0.2/src/mqt.bench.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:21:22.098525 mqt.bench-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    27066 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/tests/test_bench.py
--rw-r--r--   0 runner    (1001) docker     (123)    15180 2023-07-23 19:21:12.000000 mqt.bench-1.0.2/tests/test_benchviewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:37:07.855824 mqt.bench-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:37:07.819824 mqt.bench-1.0.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/.github/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:37:07.819824 mqt.bench-1.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/.github/workflows/coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/.github/workflows/mypy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/.github/workflows/release-drafter.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    16437 2023-07-25 07:37:07.855824 mqt.bench-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13781 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/config.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:37:07.819824 mqt.bench-1.0.3/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    21005 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/img/arch.png
+-rw-r--r--   0 runner    (1001) docker     (123)    86005 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/img/level_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)    84500 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/img/level_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)    76051 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/img/level_3.png
+-rw-r--r--   0 runner    (1001) docker     (123)   112485 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/img/level_4.png
+-rw-r--r--   0 runner    (1001) docker     (123)    61137 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/img/mqt_dark.png
+-rw-r--r--   0 runner    (1001) docker     (123)    57266 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/img/mqt_light.png
+-rw-r--r--   0 runner    (1001) docker     (123)   196044 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/img/mqtbench.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4529 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 07:37:07.855824 mqt.bench-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:37:07.815824 mqt.bench-1.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:37:07.815824 mqt.bench-1.0.3/src/mqt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:37:07.823824 mqt.bench-1.0.3/src/mqt/bench/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/src/mqt/bench/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17733 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/src/mqt/bench/benchmark_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:37:07.827824 mqt.bench-1.0.3/src/mqt/bench/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/src/mqt/bench/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/src/mqt/bench/benchmarks/ae.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/src/mqt/bench/benchmarks/dj.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/src/mqt/bench/benchmarks/ghz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/src/mqt/bench/benchmarks/graphstate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/src/mqt/bench/benchmarks/grover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/src/mqt/bench/benchmarks/qaoa.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/src/mqt/bench/benchmarks/qft.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/src/mqt/bench/benchmarks/qftentangled.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:37:07.827824 mqt.bench-1.0.3/src/mqt/bench/benchmarks/qiskit_application_finance/
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/src/mqt/bench/benchmarks/qiskit_application_finance/portfolioqaoa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/src/mqt/bench/benchmarks/qiskit_application_finance/portfoliovqe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/src/mqt/bench/benchmarks/qiskit_application_finance/pricingcall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/src/mqt/bench/benchmarks/qiskit_application_finance/pricingput.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:37:07.827824 mqt.bench-1.0.3/src/mqt/bench/benchmarks/qiskit_application_ml/
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/src/mqt/bench/benchmarks/qiskit_application_ml/qnn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:37:07.827824 mqt.bench-1.0.3/src/mqt/bench/benchmarks/qiskit_application_nature/
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/src/mqt/bench/benchmarks/qiskit_application_nature/groundstate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:37:07.827824 mqt.bench-1.0.3/src/mqt/bench/benchmarks/qiskit_application_optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/src/mqt/bench/benchmarks/qiskit_application_optimization/routing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/src/mqt/bench/benchmarks/qiskit_application_optimization/tsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/src/mqt/bench/benchmarks/qpeexact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/src/mqt/bench/benchmarks/qpeinexact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/src/mqt/bench/benchmarks/qwalk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/src/mqt/bench/benchmarks/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/src/mqt/bench/benchmarks/realamprandom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8807 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/src/mqt/bench/benchmarks/shor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/src/mqt/bench/benchmarks/su2random.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/src/mqt/bench/benchmarks/twolocalrandom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/src/mqt/bench/benchmarks/vqe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/src/mqt/bench/benchmarks/wstate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:37:07.851824 mqt.bench-1.0.3/src/mqt/bench/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/src/mqt/bench/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/src/mqt/bench/evaluation/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123) 15925096 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/src/mqt/bench/evaluation/evaluation_data.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     8133 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/src/mqt/bench/evaluation/evaluation_visualization.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:37:07.851824 mqt.bench-1.0.3/src/mqt/bench/evaluation/results/
+-rw-r--r--   0 runner    (1001) docker     (123)    16461 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/src/mqt/bench/evaluation/results/pie.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    19421 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/src/mqt/bench/evaluation/results/qubit_dist.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    24774 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/src/mqt/bench/evaluation/results/violins.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/src/mqt/bench/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8149 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/src/mqt/bench/qiskit_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11132 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/src/mqt/bench/tket_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12888 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/src/mqt/bench/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:37:07.851824 mqt.bench-1.0.3/src/mqt/benchviewer/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/src/mqt/benchviewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26632 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/src/mqt/benchviewer/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/src/mqt/benchviewer/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/src/mqt/benchviewer/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:37:07.855824 mqt.bench-1.0.3/src/mqt/benchviewer/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/src/mqt/benchviewer/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:37:07.855824 mqt.bench-1.0.3/src/mqt/benchviewer/static/files/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/src/mqt/benchviewer/static/files/MQTBench_all.zip
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:37:07.855824 mqt.bench-1.0.3/src/mqt/benchviewer/static/files/qasm_output/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/src/mqt/benchviewer/static/files/qasm_output/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    61137 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/src/mqt/benchviewer/static/mqt_dark.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/src/mqt/benchviewer/static/tum_logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:37:07.855824 mqt.bench-1.0.3/src/mqt/benchviewer/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    16436 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/src/mqt/benchviewer/templates/benchmark_description.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7441 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/src/mqt/benchviewer/templates/description.html
+-rw-r--r--   0 runner    (1001) docker     (123)    28153 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/src/mqt/benchviewer/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7693 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/src/mqt/benchviewer/templates/legal.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:37:07.823824 mqt.bench-1.0.3/src/mqt.bench.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16437 2023-07-25 07:37:07.000000 mqt.bench-1.0.3/src/mqt.bench.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-07-25 07:37:07.000000 mqt.bench-1.0.3/src/mqt.bench.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 07:37:07.000000 mqt.bench-1.0.3/src/mqt.bench.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-25 07:37:07.000000 mqt.bench-1.0.3/src/mqt.bench.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-25 07:37:07.000000 mqt.bench-1.0.3/src/mqt.bench.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-25 07:37:07.000000 mqt.bench-1.0.3/src/mqt.bench.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:37:07.855824 mqt.bench-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    27066 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/tests/test_bench.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15180 2023-07-25 07:36:57.000000 mqt.bench-1.0.3/tests/test_benchviewer.py
```

### Comparing `mqt.bench-1.0.2/.github/dependabot.yml` & `mqt.bench-1.0.3/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.2/.github/release-drafter.yml` & `mqt.bench-1.0.3/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.2/.github/workflows/codeql.yml` & `mqt.bench-1.0.3/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.2/.github/workflows/coverage.yml` & `mqt.bench-1.0.3/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.2/.github/workflows/deploy.yml` & `mqt.bench-1.0.3/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.2/.gitignore` & `mqt.bench-1.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.2/.pre-commit-config.yaml` & `mqt.bench-1.0.3/.pre-commit-config.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -66,15 +66,15 @@
   - repo: https://github.com/pre-commit/mirrors-prettier
     rev: "v3.0.0"
     hooks:
       - id: prettier
         types_or: [yaml, markdown, html, css, javascript, json]
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.0.278
+    rev: v0.0.280
     hooks:
       - id: ruff
         args: ["--fix"]
 
   - repo: https://github.com/pre-commit/mirrors-mypy
     rev: v1.4.1
     hooks:
```

### Comparing `mqt.bench-1.0.2/LICENSE` & `mqt.bench-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.2/PKG-INFO` & `mqt.bench-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mqt.bench
-Version: 1.0.2
+Version: 1.0.3
 Summary: MQT Bench - A MQT tool for Benchmarking Quantum Software Tools
 Author-email: Nils Quetschlich <nils.quetschlich@tum.de>, Lukas Burgholzer <lukas.burgholzer@jku.at>
 License: MIT License
         
         Copyright (c) 2022 Nils Quetschlich, Lukas Burgholzer, and Robert Wille
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `mqt.bench-1.0.2/README.md` & `mqt.bench-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.2/config.json` & `mqt.bench-1.0.3/config.json`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.2/img/arch.png` & `mqt.bench-1.0.3/img/arch.png`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.2/img/level_1.png` & `mqt.bench-1.0.3/img/level_1.png`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.2/img/level_2.png` & `mqt.bench-1.0.3/img/level_2.png`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.2/img/level_3.png` & `mqt.bench-1.0.3/img/level_3.png`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.2/img/level_4.png` & `mqt.bench-1.0.3/img/level_4.png`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.2/img/mqt_dark.png` & `mqt.bench-1.0.3/img/mqt_dark.png`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.2/img/mqt_light.png` & `mqt.bench-1.0.3/img/mqt_light.png`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.2/img/mqtbench.png` & `mqt.bench-1.0.3/img/mqtbench.png`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.2/pyproject.toml` & `mqt.bench-1.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.2/src/mqt/bench/benchmark_generator.py` & `mqt.bench-1.0.3/src/mqt/bench/benchmark_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,36 +78,36 @@
         return True
 
     def define_benchmark_instances(self, benchmark: Benchmark) -> None:
         lib = utils.get_module_for_benchmark(benchmark["name"])
         file_precheck = benchmark["precheck_possible"]
         instances: list[tuple[int, str]] | list[int] | list[str] | range
         if benchmark["include"]:
-            if benchmark["name"] == "grover" or benchmark["name"] == "qwalk":
+            if benchmark["name"] in ("grover", "qwalk"):
                 instances_without_anc_mode = range(
                     benchmark["min_qubits"],
                     benchmark["max_qubits"],
                     benchmark["stepsize"],
                 )
                 instances = [
                     (instance, anc_mode)
                     for instance in instances_without_anc_mode
                     for anc_mode in benchmark["ancillary_mode"]
                 ]
 
             elif benchmark["name"] == "shor":
                 instances = [lib.get_instance(choice) for choice in benchmark["instances"]]
 
-            elif benchmark["name"] == "routing" or benchmark["name"] == "tsp":
+            elif benchmark["name"] in ("routing", "tsp"):
                 instances = range(benchmark["min_nodes"], benchmark["max_nodes"])
 
             elif benchmark["name"] == "groundstate":
                 instances = benchmark["instances"]
 
-            elif benchmark["name"] == "pricingcall" or benchmark["name"] == "pricingput":
+            elif benchmark["name"] in ("pricingcall", "pricingput"):
                 instances = range(benchmark["min_uncertainty"], benchmark["max_uncertainty"])
 
             else:
                 instances = range(benchmark["min_qubits"], benchmark["max_qubits"], benchmark["stepsize"])
 
             self.generate_all_benchmarks(lib, instances, file_precheck)
 
@@ -326,15 +326,15 @@
 
     elif benchmark_name == "groundstate":
         qc = lib.create_circuit(benchmark_instance_name)
 
     else:
         qc = lib.create_circuit(circuit_size)
 
-    if level == "alg" or level == 0:
+    if level in ("alg", 0):
         return qc
 
     if compiler is None:
         msg = "Compiler must be specified for non-algorithmic levels."
         raise ValueError(msg)
 
     compiler = compiler.lower()
@@ -344,32 +344,32 @@
         raise ValueError(msg)
 
     if compiler_settings is None:
         compiler_settings = CompilerSettings(QiskitSettings(), TKETSettings())
     assert (compiler_settings.tket is not None) or (compiler_settings.qiskit is not None)
 
     independent_level = 1
-    if level == "indep" or level == independent_level:
+    if level in ("indep", independent_level):
         if compiler == "qiskit":
             return qiskit_helper.get_indep_level(qc, circuit_size, False, True)
         if compiler == "tket":
             return tket_helper.get_indep_level(qc, circuit_size, False, True)
 
     native_gates_level = 2
-    if level == "nativegates" or level == native_gates_level:
+    if level in ("nativegates", native_gates_level):
         assert gate_set_name is not None
         if compiler == "qiskit":
             assert compiler_settings.qiskit is not None
             opt_level = compiler_settings.qiskit.optimization_level
             return qiskit_helper.get_native_gates_level(qc, gate_set_name, circuit_size, opt_level, False, True)
         if compiler == "tket":
             return tket_helper.get_native_gates_level(qc, gate_set_name, circuit_size, False, True)
 
     mapped_level = 3
-    if level == "mapped" or level == mapped_level:
+    if level in ("mapped", mapped_level):
         assert gate_set_name is not None
         assert device_name is not None
         if compiler == "qiskit":
             assert compiler_settings.qiskit is not None
             opt_level = compiler_settings.qiskit.optimization_level
             assert isinstance(opt_level, int)
             return qiskit_helper.get_mapped_level(
```

### Comparing `mqt.bench-1.0.2/src/mqt/bench/benchmarks/ae.py` & `mqt.bench-1.0.3/src/mqt/bench/benchmarks/ae.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.2/src/mqt/bench/benchmarks/dj.py` & `mqt.bench-1.0.3/src/mqt/bench/benchmarks/dj.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.2/src/mqt/bench/benchmarks/ghz.py` & `mqt.bench-1.0.3/src/mqt/bench/benchmarks/ghz.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.2/src/mqt/bench/benchmarks/graphstate.py` & `mqt.bench-1.0.3/src/mqt/bench/benchmarks/graphstate.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.2/src/mqt/bench/benchmarks/grover.py` & `mqt.bench-1.0.3/src/mqt/bench/benchmarks/grover.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.2/src/mqt/bench/benchmarks/qaoa.py` & `mqt.bench-1.0.3/src/mqt/bench/benchmarks/qaoa.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.2/src/mqt/bench/benchmarks/qft.py` & `mqt.bench-1.0.3/src/mqt/bench/benchmarks/qft.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.2/src/mqt/bench/benchmarks/qftentangled.py` & `mqt.bench-1.0.3/src/mqt/bench/benchmarks/qftentangled.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.2/src/mqt/bench/benchmarks/qiskit_application_finance/portfolioqaoa.py` & `mqt.bench-1.0.3/src/mqt/bench/benchmarks/qiskit_application_finance/portfolioqaoa.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.2/src/mqt/bench/benchmarks/qiskit_application_finance/portfoliovqe.py` & `mqt.bench-1.0.3/src/mqt/bench/benchmarks/qiskit_application_finance/portfoliovqe.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.2/src/mqt/bench/benchmarks/qiskit_application_finance/pricingcall.py` & `mqt.bench-1.0.3/src/mqt/bench/benchmarks/qiskit_application_finance/pricingcall.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.2/src/mqt/bench/benchmarks/qiskit_application_finance/pricingput.py` & `mqt.bench-1.0.3/src/mqt/bench/benchmarks/qiskit_application_finance/pricingput.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.2/src/mqt/bench/benchmarks/qiskit_application_ml/qnn.py` & `mqt.bench-1.0.3/src/mqt/bench/benchmarks/qiskit_application_ml/qnn.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.2/src/mqt/bench/benchmarks/qiskit_application_nature/groundstate.py` & `mqt.bench-1.0.3/src/mqt/bench/benchmarks/qiskit_application_nature/groundstate.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.2/src/mqt/bench/benchmarks/qiskit_application_optimization/routing.py` & `mqt.bench-1.0.3/src/mqt/bench/benchmarks/qiskit_application_optimization/routing.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.2/src/mqt/bench/benchmarks/qiskit_application_optimization/tsp.py` & `mqt.bench-1.0.3/src/mqt/bench/benchmarks/qiskit_application_optimization/tsp.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.2/src/mqt/bench/benchmarks/qpeexact.py` & `mqt.bench-1.0.3/src/mqt/bench/benchmarks/qpeexact.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.2/src/mqt/bench/benchmarks/qpeinexact.py` & `mqt.bench-1.0.3/src/mqt/bench/benchmarks/qpeinexact.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.2/src/mqt/bench/benchmarks/qwalk.py` & `mqt.bench-1.0.3/src/mqt/bench/benchmarks/qwalk.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     node = QuantumRegister(n, "node")
 
     n_anc = 0
     ancillary_cutoff_recursion = 3
     if ancillary_mode == "recursion" and n > ancillary_cutoff_recursion:
         n_anc = 1
     ancillary_cutoff_vchain = 2
-    if (ancillary_mode == "v-chain" or ancillary_mode == "v-chain-dirty") and n > ancillary_cutoff_vchain:
+    if (ancillary_mode in ("v-chain", "v-chain-dirty")) and n > ancillary_cutoff_vchain:
         n_anc = n - 2
 
     if n_anc == 0:
         qc = QuantumCircuit(node, coin, name="qwalk")
 
         # coin state preparation
         if coin_state_preparation is not None:
```

### Comparing `mqt.bench-1.0.2/src/mqt/bench/benchmarks/random.py` & `mqt.bench-1.0.3/src/mqt/bench/benchmarks/random.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.2/src/mqt/bench/benchmarks/realamprandom.py` & `mqt.bench-1.0.3/src/mqt/bench/benchmarks/realamprandom.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.2/src/mqt/bench/benchmarks/shor.py` & `mqt.bench-1.0.3/src/mqt/bench/benchmarks/shor.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.2/src/mqt/bench/benchmarks/su2random.py` & `mqt.bench-1.0.3/src/mqt/bench/benchmarks/su2random.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.2/src/mqt/bench/benchmarks/twolocalrandom.py` & `mqt.bench-1.0.3/src/mqt/bench/benchmarks/twolocalrandom.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.2/src/mqt/bench/benchmarks/vqe.py` & `mqt.bench-1.0.3/src/mqt/bench/benchmarks/vqe.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.2/src/mqt/bench/benchmarks/wstate.py` & `mqt.bench-1.0.3/src/mqt/bench/benchmarks/wstate.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.2/src/mqt/bench/evaluation/evaluation.py` & `mqt.bench-1.0.3/src/mqt/bench/evaluation/evaluation.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.2/src/mqt/bench/evaluation/evaluation_data.pkl` & `mqt.bench-1.0.3/src/mqt/bench/evaluation/evaluation_data.pkl`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.2/src/mqt/bench/evaluation/evaluation_visualization.ipynb` & `mqt.bench-1.0.3/src/mqt/bench/evaluation/evaluation_visualization.ipynb`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.2/src/mqt/bench/evaluation/results/pie.pdf` & `mqt.bench-1.0.3/src/mqt/bench/evaluation/results/pie.pdf`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.2/src/mqt/bench/evaluation/results/qubit_dist.pdf` & `mqt.bench-1.0.3/src/mqt/bench/evaluation/results/qubit_dist.pdf`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.2/src/mqt/bench/evaluation/results/violins.pdf` & `mqt.bench-1.0.3/src/mqt/bench/evaluation/results/violins.pdf`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.2/src/mqt/bench/qiskit_helper.py` & `mqt.bench-1.0.3/src/mqt/bench/qiskit_helper.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.2/src/mqt/bench/tket_helper.py` & `mqt.bench-1.0.3/src/mqt/bench/tket_helper.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.2/src/mqt/bench/utils.py` & `mqt.bench-1.0.3/src/mqt/bench/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -269,15 +269,15 @@
         "oqc_lucy": get_cmap_oqc_lucy,
         "ionq_harmony": get_fully_connected_cmap,
         "ionq_aria1": get_fully_connected_cmap,
         "quantinuum_h2": get_fully_connected_cmap,
     }
 
     if device in c_map_functions:
-        if device == "ibm_washington" or device == "ibm_montreal":
+        if device in ("ibm_washington", "ibm_montreal"):
             cmap = c_map_functions[device]().configuration().coupling_map
         elif device == "ionq_harmony":
             cmap = c_map_functions[device](11)
         elif device == "ionq_aria1":
             cmap = c_map_functions[device](25)
         elif device == "quantinuum_h2":
             cmap = c_map_functions[device](32)
@@ -320,15 +320,15 @@
 ) -> SupermarqFeatures:
     connectivity_collection: list[list[int]] = []
     liveness_A_matrix = 0
     for _ in range(qc.num_qubits):
         connectivity_collection.append([])
 
     for instruction, qargs, _ in qc.data:
-        if instruction.name == "barrier" or instruction.name == "measure":
+        if instruction.name in ("barrier", "measure"):
             continue
         liveness_A_matrix += len(qargs)
         first_qubit = calc_qubit_index(qargs, qc.qregs, 0)
         all_indices = [first_qubit]
         if len(qargs) == 2:
             second_qubit = calc_qubit_index(qargs, qc.qregs, 1)
             all_indices.append(second_qubit)
@@ -345,15 +345,15 @@
     num_gates = sum(count_ops.values())
     # before subtracting the measure and barrier gates, check whether it is in the dict
     if "measure" in count_ops:
         num_gates -= count_ops.get("measure")
     if "barrier" in count_ops:
         num_gates -= count_ops.get("barrier")
     num_multiple_qubit_gates = qc.num_nonlocal_gates()
-    depth = qc.depth(lambda x: x[0].name != "barrier" and x[0].name != "measure")
+    depth = qc.depth(lambda x: x[0].name not in ("barrier", "measure"))
     program_communication = np.sum(connectivity) / (qc.num_qubits * (qc.num_qubits - 1))
 
     if num_multiple_qubit_gates == 0:
         critical_depth = 0.0
     else:
         critical_depth = (
             qc.depth(filter_function=lambda x: len(x[1]) > 1 and x[0].name != "barrier") / num_multiple_qubit_gates
```

### Comparing `mqt.bench-1.0.2/src/mqt/benchviewer/backend.py` & `mqt.bench-1.0.3/src/mqt/benchviewer/backend.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.2/src/mqt/benchviewer/main.py` & `mqt.bench-1.0.3/src/mqt/benchviewer/main.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.2/src/mqt/benchviewer/static/favicon.ico` & `mqt.bench-1.0.3/src/mqt/benchviewer/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.2/src/mqt/benchviewer/static/mqt_dark.png` & `mqt.bench-1.0.3/src/mqt/benchviewer/static/mqt_dark.png`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.2/src/mqt/benchviewer/static/tum_logo.svg` & `mqt.bench-1.0.3/src/mqt/benchviewer/static/tum_logo.svg`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.2/src/mqt/benchviewer/templates/benchmark_description.html` & `mqt.bench-1.0.3/src/mqt/benchviewer/templates/benchmark_description.html`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.2/src/mqt/benchviewer/templates/description.html` & `mqt.bench-1.0.3/src/mqt/benchviewer/templates/description.html`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.2/src/mqt/benchviewer/templates/index.html` & `mqt.bench-1.0.3/src/mqt/benchviewer/templates/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -633,15 +633,15 @@
         <strong
           >In case you are using MQT Bench in your work, we would be thankful if
           you referred to it by citing the following publication:</strong
         >
       </p>
 
       <p>
-        @misc{quetschlich2023mqtbench, <br />
+        @article{quetschlich2023mqtbench, <br />
         &nbsp; title=&#123;&#123;&#123;MQT Bench}}: Benchmarking Software and
         Design Automation Tools for Quantum Computing},<br />
         &nbsp; shorttitle = &#123;&#123;MQT Bench}},<br />
         &nbsp; journal = &#123;&#123;Quantum}},<br />
         &nbsp; author={Quetschlich, Nils and Burgholzer, Lukas and Wille,
         Robert},<br />
         &nbsp; year={2023},<br />
```

#### html2text {}

```diff
@@ -87,15 +87,15 @@
  Download selected Benchmarks
 *** Reference ***
 For a more detailed description of MQT Bench, we are referring to the
 corresponding paper "MQT_Bench:_Benchmarking_Software_and_Design_Automation
 Tools_for_Quantum_Computing". Our implementation is available on Github. In
 case you are using MQT Bench in your work, we would be thankful if you referred
 to it by citing the following publication:
-@misc{quetschlich2023mqtbench,
+@article{quetschlich2023mqtbench,
   title={{{MQT Bench}}: Benchmarking Software and Design Automation Tools for
 Quantum Computing},
   shorttitle = {{MQT Bench}},
   journal = {{Quantum}},
   author={Quetschlich, Nils and Burgholzer, Lukas and Wille, Robert},
   year={2023},
   note={{{MQT Bench}} is available at \url{https://www.cda.cit.tum.de/mqtbench/
```

### Comparing `mqt.bench-1.0.2/src/mqt/benchviewer/templates/legal.html` & `mqt.bench-1.0.3/src/mqt/benchviewer/templates/legal.html`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.2/src/mqt.bench.egg-info/PKG-INFO` & `mqt.bench-1.0.3/src/mqt.bench.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mqt.bench
-Version: 1.0.2
+Version: 1.0.3
 Summary: MQT Bench - A MQT tool for Benchmarking Quantum Software Tools
 Author-email: Nils Quetschlich <nils.quetschlich@tum.de>, Lukas Burgholzer <lukas.burgholzer@jku.at>
 License: MIT License
         
         Copyright (c) 2022 Nils Quetschlich, Lukas Burgholzer, and Robert Wille
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `mqt.bench-1.0.2/src/mqt.bench.egg-info/SOURCES.txt` & `mqt.bench-1.0.3/src/mqt.bench.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.2/tests/test_bench.py` & `mqt.bench-1.0.3/tests/test_bench.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.0.2/tests/test_benchviewer.py` & `mqt.bench-1.0.3/tests/test_benchviewer.py`

 * *Files identical despite different names*

