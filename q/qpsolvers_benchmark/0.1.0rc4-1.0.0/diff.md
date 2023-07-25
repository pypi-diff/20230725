# Comparing `tmp/qpsolvers_benchmark-0.1.0rc4.tar.gz` & `tmp/qpsolvers_benchmark-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qpsolvers_benchmark-0.1.0rc4.tar", last modified: Thu Jan 26 14:52:35 2023, max compression
+gzip compressed data, was "qpsolvers_benchmark-1.0.0.tar", last modified: Tue Jul 25 12:13:25 2023, max compression
```

## Comparing `qpsolvers_benchmark-0.1.0rc4.tar` & `qpsolvers_benchmark-1.0.0.tar`

### file list

```diff
@@ -1,38 +1,25 @@
--rw-r--r--   0        0        0     1162 2022-12-13 11:20:59.949355 qpsolvers_benchmark-0.1.0rc4/.github/ISSUE_TEMPLATE/new_problem.md
--rw-r--r--   0        0        0      271 2022-12-13 12:15:08.854346 qpsolvers_benchmark-0.1.0rc4/.github/ISSUE_TEMPLATE/software_issue.md
--rw-r--r--   0        0        0      700 2023-01-26 14:49:40.293437 qpsolvers_benchmark-0.1.0rc4/.github/workflows/CI.yml
--rw-r--r--   0        0        0       92 2022-11-07 08:16:29.729744 qpsolvers_benchmark-0.1.0rc4/.gitignore
--rw-r--r--   0        0        0     1052 2023-01-26 14:51:53.527478 qpsolvers_benchmark-0.1.0rc4/CHANGELOG.md
--rw-r--r--   0        0        0      629 2022-12-24 09:50:28.416923 qpsolvers_benchmark-0.1.0rc4/CONTRIBUTING.md
--rw-r--r--   0        0        0    11357 2022-12-24 09:50:28.416923 qpsolvers_benchmark-0.1.0rc4/LICENSE
--rw-r--r--   0        0        0     6912 2023-01-26 14:49:40.293437 qpsolvers_benchmark-0.1.0rc4/README.md
--rwxr-xr-x   0        0        0     7065 2023-01-11 09:15:12.911314 qpsolvers_benchmark-0.1.0rc4/benchmark.py
--rw-r--r--   0        0        0      398 2023-01-17 18:10:04.288812 qpsolvers_benchmark-0.1.0rc4/environment.yaml
--rw-r--r--   0        0        0     1794 2023-01-17 18:10:04.288812 qpsolvers_benchmark-0.1.0rc4/pyproject.toml
--rw-r--r--   0        0        0      985 2023-01-04 16:59:29.754068 qpsolvers_benchmark-0.1.0rc4/qpsolvers_benchmark/__init__.py
--rw-r--r--   0        0        0      883 2023-01-11 09:15:12.911314 qpsolvers_benchmark-0.1.0rc4/qpsolvers_benchmark/exceptions.py
--rw-r--r--   0        0        0     2526 2023-01-11 09:15:12.911314 qpsolvers_benchmark-0.1.0rc4/qpsolvers_benchmark/plots.py
--rw-r--r--   0        0        0     3806 2023-01-04 16:59:29.754068 qpsolvers_benchmark-0.1.0rc4/qpsolvers_benchmark/problem.py
--rw-r--r--   0        0        0    17628 2023-01-17 16:21:12.363585 qpsolvers_benchmark-0.1.0rc4/qpsolvers_benchmark/report.py
--rw-r--r--   0        0        0    11132 2023-01-11 09:15:12.911314 qpsolvers_benchmark-0.1.0rc4/qpsolvers_benchmark/results.py
--rw-r--r--   0        0        0     4943 2023-01-04 16:59:29.754068 qpsolvers_benchmark-0.1.0rc4/qpsolvers_benchmark/run.py
--rw-r--r--   0        0        0     1734 2023-01-04 16:59:29.754068 qpsolvers_benchmark-0.1.0rc4/qpsolvers_benchmark/shgeom.py
--rw-r--r--   0        0        0     5180 2023-01-26 14:49:40.293437 qpsolvers_benchmark-0.1.0rc4/qpsolvers_benchmark/solver_issues.py
--rw-r--r--   0        0        0     5965 2023-01-17 16:25:22.511769 qpsolvers_benchmark-0.1.0rc4/qpsolvers_benchmark/solver_settings.py
--rw-r--r--   0        0        0     2030 2022-12-24 09:50:28.420924 qpsolvers_benchmark-0.1.0rc4/qpsolvers_benchmark/spdlog.py
--rw-r--r--   0        0        0     5503 2023-01-26 14:49:40.293437 qpsolvers_benchmark-0.1.0rc4/qpsolvers_benchmark/test_set.py
--rw-r--r--   0        0        0      665 2023-01-04 16:59:29.754068 qpsolvers_benchmark-0.1.0rc4/qpsolvers_benchmark/test_sets/__init__.py
--rw-r--r--   0        0        0     2936 2023-01-04 16:59:29.754068 qpsolvers_benchmark-0.1.0rc4/qpsolvers_benchmark/test_sets/github_ffa.py
--rw-r--r--   0        0        0     1030 2023-01-04 16:59:29.754068 qpsolvers_benchmark-0.1.0rc4/qpsolvers_benchmark/test_sets/github_ffa_problems/__init__.py
--rw-r--r--   0        0        0     1415 2023-01-04 16:59:29.754068 qpsolvers_benchmark-0.1.0rc4/qpsolvers_benchmark/test_sets/github_ffa_problems/ghffa01.py
--rw-r--r--   0        0        0     1344 2023-01-04 16:59:29.754068 qpsolvers_benchmark-0.1.0rc4/qpsolvers_benchmark/test_sets/github_ffa_problems/ghffa02.py
--rw-r--r--   0        0        0     1339 2023-01-04 16:59:29.758068 qpsolvers_benchmark-0.1.0rc4/qpsolvers_benchmark/test_sets/github_ffa_problems/ghffa03.py
--rw-r--r--   0        0        0     6338 2023-01-04 16:59:29.758068 qpsolvers_benchmark-0.1.0rc4/qpsolvers_benchmark/test_sets/maros_meszaros.py
--rw-r--r--   0        0        0     2169 2023-01-04 16:59:29.758068 qpsolvers_benchmark-0.1.0rc4/qpsolvers_benchmark/test_sets/maros_meszaros_dense.py
--rw-r--r--   0        0        0      744 2022-12-24 09:50:28.420924 qpsolvers_benchmark-0.1.0rc4/qpsolvers_benchmark/test_sets/problem.py
--rw-r--r--   0        0        0     1588 2023-01-11 09:15:12.911314 qpsolvers_benchmark-0.1.0rc4/qpsolvers_benchmark/tolerance.py
--rw-r--r--   0        0        0     3757 2023-01-17 16:21:12.363585 qpsolvers_benchmark-0.1.0rc4/qpsolvers_benchmark/utils.py
--rw-r--r--   0        0        0      761 2023-01-26 14:35:19.038969 qpsolvers_benchmark-0.1.0rc4/qpsolvers_benchmark/version.py
--rw-r--r--   0        0        0     1155 2023-01-04 16:59:29.762068 qpsolvers_benchmark-0.1.0rc4/tox.ini
--rw-r--r--   0        0        0     1256 1970-01-01 00:00:00.000000 qpsolvers_benchmark-0.1.0rc4/setup.py
--rw-r--r--   0        0        0     8881 1970-01-01 00:00:00.000000 qpsolvers_benchmark-0.1.0rc4/PKG-INFO
+-rw-r--r--   0        0        0     1471 2023-07-25 11:49:30.311879 qpsolvers_benchmark-1.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0      629 2022-12-24 09:50:28.416923 qpsolvers_benchmark-1.0.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0    11357 2022-12-24 09:50:28.416923 qpsolvers_benchmark-1.0.0/LICENSE
+-rw-r--r--   0        0        0     8711 2023-07-25 12:11:27.283642 qpsolvers_benchmark-1.0.0/README.md
+-rw-r--r--   0        0        0      398 2023-04-18 14:45:51.689956 qpsolvers_benchmark-1.0.0/environment.yaml
+-rw-r--r--   0        0        0     2358 2023-07-25 11:54:36.087824 qpsolvers_benchmark-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      983 2023-02-07 14:30:22.354053 qpsolvers_benchmark-1.0.0/qpsolvers_benchmark/__init__.py
+-rw-r--r--   0        0        0     9048 2023-07-17 13:36:28.541158 qpsolvers_benchmark-1.0.0/qpsolvers_benchmark/benchmark.py
+-rw-r--r--   0        0        0      859 2023-02-07 14:30:22.354053 qpsolvers_benchmark-1.0.0/qpsolvers_benchmark/exceptions.py
+-rw-r--r--   0        0        0     3051 2023-04-10 15:49:43.848558 qpsolvers_benchmark-1.0.0/qpsolvers_benchmark/plot_metric.py
+-rw-r--r--   0        0        0     3783 2023-05-06 08:56:41.273999 qpsolvers_benchmark-1.0.0/qpsolvers_benchmark/problem.py
+-rw-r--r--   0        0        0    18163 2023-02-28 15:07:18.081635 qpsolvers_benchmark-1.0.0/qpsolvers_benchmark/report.py
+-rw-r--r--   0        0        0    11027 2023-02-28 15:34:18.149817 qpsolvers_benchmark-1.0.0/qpsolvers_benchmark/results.py
+-rw-r--r--   0        0        0     4936 2023-02-07 14:30:22.358053 qpsolvers_benchmark-1.0.0/qpsolvers_benchmark/run.py
+-rw-r--r--   0        0        0     1727 2023-02-07 14:30:22.358053 qpsolvers_benchmark-1.0.0/qpsolvers_benchmark/shgeom.py
+-rw-r--r--   0        0        0     5168 2023-02-07 14:30:22.358053 qpsolvers_benchmark-1.0.0/qpsolvers_benchmark/solver_issues.py
+-rw-r--r--   0        0        0     6370 2023-07-17 13:36:28.541158 qpsolvers_benchmark-1.0.0/qpsolvers_benchmark/solver_settings.py
+-rw-r--r--   0        0        0     2167 2023-02-07 14:30:22.358053 qpsolvers_benchmark-1.0.0/qpsolvers_benchmark/spdlog.py
+-rw-r--r--   0        0        0     5882 2023-04-10 15:49:43.848558 qpsolvers_benchmark-1.0.0/qpsolvers_benchmark/test_set.py
+-rw-r--r--   0        0        0     1772 2023-02-03 21:11:17.751369 qpsolvers_benchmark-1.0.0/qpsolvers_benchmark/tolerance.py
+-rw-r--r--   0        0        0     4064 2023-04-10 16:07:49.082853 qpsolvers_benchmark-1.0.0/qpsolvers_benchmark/utils.py
+-rw-r--r--   0        0        0      746 2023-07-25 11:49:41.411877 qpsolvers_benchmark-1.0.0/qpsolvers_benchmark/version.py
+-rw-r--r--   0        0        0     1040 2023-02-07 14:30:22.358053 qpsolvers_benchmark-1.0.0/tox.ini
+-rw-r--r--   0        0        0     1442 1970-01-01 00:00:00.000000 qpsolvers_benchmark-1.0.0/setup.py
+-rw-r--r--   0        0        0    10743 1970-01-01 00:00:00.000000 qpsolvers_benchmark-1.0.0/PKG-INFO
```

### Comparing `qpsolvers_benchmark-0.1.0rc4/CHANGELOG.md` & `qpsolvers_benchmark-1.0.0/CHANGELOG.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,28 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
+## [1.0.0] - 2023/07/25
+
+### Added
+
+* Allow non-lowercase solver names in the command line (thanks to @ottapav)
+* Command-line tool and standalone test sets (thanks to @ZAKIAkram)
+
+### Changed
+
+* Plot: trim solutions that don't fulfill tolerance requirements
+* Rename ``hist`` command to ``plot``
+* Update to qpsolvers v3.4.0
+
+### Fixed
+
+* Plot whiskers on solutions beyond tolerance requirements (thanks to @ottapav)
+
 ## [0.1.0-beta] - 2022/01/26
 
 ### Added
 
 * Check dual residual
 * Check duality gap
 * Document all benchmark functions
```

### Comparing `qpsolvers_benchmark-0.1.0rc4/CONTRIBUTING.md` & `qpsolvers_benchmark-1.0.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `qpsolvers_benchmark-0.1.0rc4/LICENSE` & `qpsolvers_benchmark-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qpsolvers_benchmark-0.1.0rc4/README.md` & `qpsolvers_benchmark-1.0.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,61 @@
 # QP solvers benchmark
 
-[![Build](https://img.shields.io/github/actions/workflow/status/stephane-caron/qpsolvers_benchmark/CI.yml?branch=main)](https://github.com/stephane-caron/qpsolvers_benchmark/actions)
+[![Build](https://img.shields.io/github/actions/workflow/status/stephane-caron/qpsolvers_benchmark/ci.yml?branch=main)](https://github.com/stephane-caron/qpsolvers_benchmark/actions)
 [![PyPI version](https://img.shields.io/pypi/v/qpsolvers_benchmark)](https://pypi.org/project/qpsolvers_benchmark/)
 [![Contributing](https://img.shields.io/badge/PRs-welcome-green.svg)](https://github.com/stephane-caron/qpsolvers_benchmark/tree/master/CONTRIBUTING.md)
 
 Benchmark for quadratic programming (QP) solvers available in Python.
 
-The goal of this benchmark is to help us compare and select QP solvers. Its methodology is open to [discussions](https://github.com/stephane-caron/qpsolvers_benchmark/discussions). New test sets are [also welcome](CONTRIBUTING.md). Feel free to add one that better represents the kind of problems you are working on.
+The goal of this benchmark is to help users compare and select QP solvers. Its methodology is open to [discussions](https://github.com/stephane-caron/qpsolvers_benchmark/discussions). The benchmark ships standard and community [test sets](#test-sets), as well as a ``qpsolvers_benchmark`` command-line tool to run any test set directly on your machine. For instance:
+
+```console
+qpsolvers_benchmark maros_meszaros/maros_meszaros.py run
+```
+
+The outcome from running a test set is a standardized report evaluating all [metrics](#metrics) of the benchmark across all available QP solvers. This repository also distributes [results](#results) from running the benchmark on all test sets using the same computer.
+
+New test sets are [welcome](CONTRIBUTING.md). The benchmark is designed so that each test-set directory is standalone, so that the ``qpsolvers_benchmark`` command can be run on test sets from other repositories. Feel free to create ones that better represent the kind of problems you are working on.
 
 ## Solvers
 
 | Solver | Keyword | Algorithm | Matrices | License |
 | ------ | ------- | --------- | -------- | ------- |
+| [Clarabel](https://github.com/oxfordcontrol/Clarabel.rs) | ``clarabel`` | Interior point | Sparse | Apache-2.0 |
 | [CVXOPT](http://cvxopt.org/) | ``cvxopt`` | Interior point | Dense | GPL-3.0 |
+| [DAQP](https://github.com/darnstrom/daqp) | ``daqp`` | Active set | Dense | MIT |
 | [ECOS](https://web.stanford.edu/~boyd/papers/ecos.html) | ``ecos`` | Interior point | Sparse | GPL-3.0 |
 | [Gurobi](https://www.gurobi.com/) | ``gurobi`` | Interior point | Sparse | Commercial |
 | [HiGHS](https://highs.dev/) | ``highs`` | Active set | Sparse | MIT |
 | [MOSEK](https://mosek.com/) | ``mosek`` | Interior point | Sparse | Commercial |
+| NPPro | ``nppro`` | Active set | Dense | Commercial |
 | [OSQP](https://osqp.org/) | ``osqp`` | Douglas–Rachford | Sparse | Apache-2.0 |
 | [ProxQP](https://github.com/Simple-Robotics/proxsuite) | ``proxqp`` | Augmented Lagrangian | Dense & Sparse | BSD-2-Clause |
 | [qpOASES](https://github.com/coin-or/qpOASES) | ``qpoases`` | Active set | Dense | LGPL-2.1 |
 | [qpSWIFT](https://qpswift.github.io/) | ``qpswift`` | Interior point | Sparse | GPL-3.0 |
 | [quadprog](https://pypi.python.org/pypi/quadprog/) | ``quadprog`` | Goldfarb-Idnani | Dense | GPL-2.0 |
 | [SCS](https://www.cvxgrp.org/scs/) | ``scs`` | Douglas–Rachford | Sparse | MIT |
 
-## Test sets and results
+## Test sets
 
-The benchmark has different test sets that represent different use cases for QP solvers. Click on a test set to check out its report.
+The benchmark comes with standard and community test sets to represent different use cases for QP solvers:
 
 | Test set | Keyword | Description |
 | -------- | ------- | ----------- |
-| [GitHub free-for-all](results/github_ffa.md) | ``github_ffa`` | Test set built by the community on GitHub, new problems [are welcome](https://github.com/stephane-caron/qpsolvers_benchmark/issues/new?assignees=&labels=&template=new_problem.md&title=)! |
-| [Maros-Meszaros](results/maros_meszaros.md) | ``maros_meszaros`` | Standard set of problems designed to be difficult. |
-| [Maros-Meszaros dense](results/maros_meszaros_dense.md) | ``maros_meszaros_dense`` | Subset of the Maros-Meszaros test set restricted to smaller dense problems. |
+| **GitHub free-for-all** | ``github_ffa`` | Test set built by the community on GitHub, new problems [are welcome](https://github.com/stephane-caron/qpsolvers_benchmark/issues/new?assignees=&labels=&template=new_problem.md&title=)! |
+| **Maros-Meszaros** | ``maros_meszaros`` | Standard set of problems designed to be difficult. |
+| **Maros-Meszaros dense** | ``maros_meszaros_dense`` | Subset of the Maros-Meszaros test set restricted to smaller dense problems. |
+
+## Results
+
+The outcome from running a test set is a standardized report. Here are the results obtained from running all test sets in this repository with the same computer:
+
+* [GitHub free-for-all](github_ffa/results/github_ffa.md)
+* [Maros-Meszaros](maros_meszaros/results/maros_meszaros.md)
+* [Maros-Meszaros dense](maros_meszaros/results/maros_meszaros_dense.md)
 
 ## Metrics
 
 We evaluate QP solvers based on the following metrics:
 
 - **Success rate:** percentage of problems a solver is able to solve on a given test set.
 - **Computation time:** time a solver takes to solve a given problem.
@@ -78,27 +97,39 @@
 pip install qpsolvers_benchmark
 ```
 
 By default, the benchmark will run all supported solvers it finds.
 
 ## Running the benchmark
 
-Pick up the keyword corresponding to the desired [test set](#test-sets), for instance ``maros_meszaros``, and pass it to the ``run`` command:
+Once the benchmark is installed, you will be able to run the ``qpsolvers_benchmark`` command. Provide it with the script corresponding to the [test set](#test-sets) you want to run, followed by a benchmark command such as "run". For instance, let's run the "dense" subset of the Maros-Meszaros test set:
 
 ```console
-python benchmark.py maros_meszaros run
+qpsolvers_benchmark maros_meszaros/maros_meszaros_dense.py run
 ```
 
 You can also run a specific solver, problem or set of solver settings:
 
 ```console
-python benchmark.py maros_meszaros_dense run --solver proxqp --settings default
+qpsolvers_benchmark maros_meszaros/maros_meszaros_dense.py run --solver proxqp --settings default
 ```
 
-Check out ``python benchmark.py --help`` for all available commands and arguments.
+Check out ``qpsolvers_benchmark --help`` for a list of available commands and arguments.
+
+## Plots
+
+The command line ships a ``plot`` command to compare solver performances over a test set for a specific metric. For instance, run:
+
+```console
+qpsolvers_benchmark maros_meszaros/maros_meszaros_dense.py plot runtime high_accuracy
+```
+
+To generate the following plot:
+
+![image](https://user-images.githubusercontent.com/1189580/220150365-530cd685-fc90-49b5-90e0-0b243fa602d9.png)
 
 ## Contributing
 
 Contributions to improving this benchmark are welcome. You can for instance propose new problems, or share the runtimes you obtain on your machine. Check out the [contribution guidelines](CONTRIBUTING.md) for details.
 
 ## See also
```

### Comparing `qpsolvers_benchmark-0.1.0rc4/benchmark.py` & `qpsolvers_benchmark-1.0.0/qpsolvers_benchmark/benchmark.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,45 +11,43 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""This is the main script for the 'qpsolvers_benchmark' package.
+
+It provides tools to benchmark different Quadratic Programming (QP) solvers.
+"""
+
 import argparse
 import os
+import sys
 from importlib import import_module  # type: ignore
 
-from qpsolvers_benchmark import Report, Results, TestSet, logging, run
-from qpsolvers_benchmark.plots import hist
+from .plot_metric import plot_metric
+from .report import Report
+from .results import Results
+from .run import run
+from .spdlog import logging
+from .test_set import TestSet
 
-TEST_SETS = [
-    "github_ffa",
-    "maros_meszaros",
-    "maros_meszaros_dense",
-]
-
-TEST_ARGS = {
-    "maros_meszaros": {
-        "data_dir": os.path.join(os.path.dirname(__file__), "data"),
-    },
-    "maros_meszaros_dense": {
-        "data_dir": os.path.join(os.path.dirname(__file__), "data"),
-    },
-}
 
+def parse_command_line_arguments() -> argparse.Namespace:
+    """Extracts and interprets command line arguments passed to the script.
 
-def parse_command_line_arguments():
+    Returns:
+        args: arguments of the command line.
+    """
     parser = argparse.ArgumentParser(
         description="Benchmark quadratic programming solvers"
     )
     parser.add_argument(
-        "test_set",
-        choices=TEST_SETS,
-        help="test set from the benchmark to consider",
+        "test_set_path", help="path to the test set python file"
     )
     parser.add_argument(
         "-v",
         "--verbose",
         default=False,
         action="store_true",
         help="verbose mode",
@@ -74,37 +72,48 @@
         help="evaluate test set results interactively",
     )
     parser_check_results.add_argument(
         "--results-file",
         help="path to the results CSV file",
     )
 
-    # hist
-    parser_hist = subparsers.add_parser(
-        "hist",
+    # plot
+    parser_plot = subparsers.add_parser(
+        "plot",
         help="compare how solvers performed on a given metric",
     )
-    parser_hist.add_argument(
+    parser_plot.add_argument(
         "metric",
         help='name of the metric to evaluate (e.g. "duality_gap")',
     )
-    parser_hist.add_argument(
+    parser_plot.add_argument(
         "settings",
         help='settings to compare solvers on (e.g. "high_accuracy")',
     )
-    parser_hist.add_argument(
+    parser_plot.add_argument(
+        "--results-file", help="path to the CSV file where results are stored"
+    )
+    parser_plot.add_argument(
+        "--linewidth",
+        help="width of plotted lines in px",
+        type=int,
+        default=3,
+    )
+    parser_plot.add_argument(
+        "--savefig",
+        help="path to a file to save the plot to (rather than displaying it)",
+    )
+    parser_plot.add_argument(
         "--solvers",
         help="solvers to limit the histogram to",
         nargs="+",
     )
-    parser_hist.add_argument(
-        "--bins",
-        help="number of bins in the resulting histogram",
-        type=int,
-        default=10,
+    parser_plot.add_argument(
+        "--title",
+        help='plot title (set to "" to disable)',
     )
 
     # report
     parser_report = subparsers.add_parser(
         "report",
         help="write report from test set results",
     )
@@ -119,14 +128,17 @@
 
     # run
     parser_run = subparsers.add_parser(
         "run",
         help="run all tests from the test set",
     )
     parser_run.add_argument(
+        "--results-path", help="write results in a specific directory"
+    )
+    parser_run.add_argument(
         "--include-timeouts",
         default=False,
         action="store_true",
         help="include timeouts when --rerunning the test set",
     )
     parser_run.add_argument(
         "--problem",
@@ -147,103 +159,145 @@
         help="limit run to a specific solver",
     )
     parser_run.add_argument(
         "--author",
         help="author field in the post-run report",
     )
 
-    return parser.parse_args()
+    args = parser.parse_args()
+    if "settings" in args and args.settings is not None:
+        args.settings = args.settings.lower()
+    if "solver" in args and args.solver is not None:
+        args.solver = args.solver.lower()
+    if "solvers" in args and args.solvers is not None:
+        lowercase_solvers = [name.lower() for name in args.solvers]
+        args.solvers = lowercase_solvers
+    return args
+
 
+def find_results_file(args: argparse.Namespace) -> str:
+    """Find the path to the results file.
 
-def find_results_file(args):
-    if args.command in ["check_results", "report"]:
+    Args:
+        args: The arguments passed in the command line.
+
+    Raises:
+        FileNotFoundError: If the file was not found.
+
+    Returns:
+        str: The path to the results file.
+    """
+    if args.command in ["check_results", "report", "plot"]:
         results_file = (
-            args.results_file
+            os.path.abspath(args.results_file)
             if args.results_file
-            else f"results/{args.test_set}.csv"
+            else os.path.join(
+                os.path.dirname(os.path.abspath(args.test_set_path)),
+                "results",
+                os.path.split(args.test_set_path)[1].replace(".py", ".csv"),
+            )
         )
         if not os.path.exists(results_file):
             raise FileNotFoundError(f"results file '{results_file}' not found")
     else:
-        results_dir = os.path.join(os.path.dirname(__file__), "results")
-        results_file = os.path.join(results_dir, f"{args.test_set}.csv")
+        if args.command == "run" and args.results_path:
+            results_dir = os.path.abspath(args.results_path)
+        else:
+            testset_dir = os.path.dirname(args.test_set_path)
+            results_dir = os.path.join(testset_dir, "results")
+        if not os.path.exists(results_dir):
+            os.mkdir(results_dir)
+        results_file = os.path.join(
+            results_dir,
+            os.path.split(args.test_set_path)[1].replace(".py", ".csv"),
+        )
     return results_file
 
 
-def load_test_set(name: str) -> TestSet:
-    """
-    Load a test set.
+def load_test_set(path: str) -> TestSet:
+    """Load a test set.
 
     Args:
-        name: Name of the test set.
+        path: path to the .py file containing the class definition
+                of the TestSet
 
     Returns:
-        Test set.
+        Test set
     """
-    module = import_module(f"qpsolvers_benchmark.test_sets.{name}")
+    dir_path, full_name = os.path.split(path)
+    name = full_name.replace(".py", "")
+    sys.path.append(
+        dir_path
+    )  # Add directory path to system path so import_module can find the module
+    module = import_module(name)
     class_name = name.title().replace("_", "")
     TestClass = getattr(module, class_name)
-    kwargs = TEST_ARGS.get(name, {})
-    return TestClass(**kwargs)
+    return TestClass()
 
 
-if __name__ == "__main__":
+def main():
+    """Main function of the script."""
     args = parse_command_line_arguments()
     if args.verbose:
         logging.getLogger().setLevel(logging.DEBUG)
-
-    test_set = load_test_set(args.test_set)
+    test_set = load_test_set(os.path.abspath(args.test_set_path))
     results = Results(find_results_file(args), test_set)
 
     if args.command == "run":
-        args.solver = args.solver.lower() if args.solver else None
-        args.settings = args.settings.lower() if args.settings else None
         run(
             test_set,
             results,
             only_problem=args.problem,
             only_settings=args.settings,
             only_solver=args.solver,
             rerun=args.rerun,
             include_timeouts=args.include_timeouts,
         )
 
     if args.command == "check_problem":
         problem = test_set.get_problem(args.problem)
+        _ = problem  # dummy variable, to pass ruff linting
         logging.info(f"Check out `problem` for the {args.problem} problem")
 
     if args.command == "check_results":
         logging.info("Check out `results` for the full results data")
         df = results.df
+        _ = df  # dummy variable, to pass ruff linting
         logging.info("Check out `df` for results as a pandas DataFrame")
 
     if args.command in ["check_problem", "check_results"]:
         try:
             import IPython
 
             if not IPython.get_ipython():
                 IPython.embed()
         except ImportError:
             logging.error(
                 "IPython not found, run this script in interactive mode"
             )
 
-    if args.command == "hist":
-        hist(
+    if args.command == "plot":
+        plot_metric(
             args.metric,
             results.df,
             args.settings,
             test_set,
             solvers=args.solvers,
-            nb_bins=args.bins,
+            linewidth=args.linewidth,
+            savefig=args.savefig,
+            title=args.title,
         )
 
     if args.command in ["report", "run"]:
         logging.info("Writing the overall report...")
         author = (
             args.author
             if args.author
             else input("GitHub username to write in the report? ")
         )
         report = Report(author, results)
         md_path = results.csv_path.replace(".csv", ".md")
         report.write(md_path)
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `qpsolvers_benchmark-0.1.0rc4/qpsolvers_benchmark/__init__.py` & `qpsolvers_benchmark-1.0.0/qpsolvers_benchmark/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,17 +11,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""
-Benchmark for quadratic programming solvers available in Python.
-"""
+"""Benchmark for quadratic programming solvers available in Python."""
 
 from .report import Report
 from .results import Results
 from .run import run
 from .spdlog import logging
 from .test_set import TestSet
 from .version import get_version
```

### Comparing `qpsolvers_benchmark-0.1.0rc4/qpsolvers_benchmark/exceptions.py` & `qpsolvers_benchmark-1.0.0/qpsolvers_benchmark/exceptions.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,24 +11,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""
-Benchmark exceptions.
-"""
+"""Benchmark exceptions."""
 
 
 class BenchmarkError(Exception):
-
-    """
-    Base class for benchmark exceptions.
-    """
+    """Base class for benchmark exceptions."""
 
 
 class ProblemNotFound(BenchmarkError):
-
-    """
-    Exception raised when a requested problem is not part of a test set.
-    """
+    """Exception raised when a requested problem is not part of a test set."""
```

### Comparing `qpsolvers_benchmark-0.1.0rc4/qpsolvers_benchmark/plots.py` & `qpsolvers_benchmark-1.0.0/qpsolvers_benchmark/plot_metric.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,72 +11,78 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""
-Plots for analysis of test set results.
-"""
+"""Plots for analysis of test set results."""
 
 from typing import List, Optional
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas
 
 from .test_set import TestSet
 
 
-def hist(
+def plot_metric(
     metric: str,
     df: pandas.DataFrame,
     settings: str,
     test_set: TestSet,
     solvers: Optional[List[str]] = None,
-    nb_bins: int = 10,
-    alpha: float = 0.5,
+    linewidth: float = 3.0,
+    savefig: Optional[str] = None,
+    title: Optional[str] = None,
 ) -> None:
-    """
-    Histogram comparing solvers on a given metric.
+    """Plot comparing solvers on a given metric.
 
     Args:
         metric: Metric to compare solvers on.
         df: Test set results data frame.
         settings: Settings to compare solvers on.
         test_set: Test set.
         solvers: Names of solvers to compare (default: all).
-        nb_bins: Number of bins in the histogram.
-        alpha: Histogram transparency.
+        linewidth: Width of output lines, in px.
+        savefig: If set, save plot to this path rather than displaying it.
+        title: Plot title, set to "" to disable.
     """
     assert issubclass(df[metric].dtype.type, np.floating)
+    nb_problems = test_set.count_problems()
     settings_df = df[df["settings"] == settings]
     metric_tol = test_set.tolerances[settings].from_metric(metric)
-    hist_df = settings_df.assign(
-        **{
-            metric: settings_df[metric].mask(
-                ~settings_df["found"],
-                metric_tol,
-            ),
-        }
-    )
+    found_df = settings_df[settings_df["found"]]
+    solved_df = found_df[found_df[metric] <= metric_tol]
     plot_solvers: List[str] = (
-        solvers if solvers is not None else list(set(hist_df.solver))
+        solvers if solvers is not None else list(set(solved_df.solver))
     )
     for solver in plot_solvers:
-        values = hist_df[hist_df["solver"] == solver][metric].values
-        _, bins = np.histogram(values, bins=nb_bins)
-        logmin = np.log10(max(bins[0], 1e-20))
-        logmax = np.log10(max(bins[-1], 1e-20))
-        logbins = np.logspace(logmin, logmax, len(bins))
-        plt.hist(values, bins=logbins, cumulative=True, alpha=alpha)
+        values = solved_df[solved_df["solver"] == solver][metric].values
+        nb_solved = len(values)
+        if nb_solved < 1:
+            plt.step([0.0, metric_tol], [0.0, 0.0], linewidth=linewidth)
+            continue
+        sorted_values = np.sort(values)
+        y = np.arange(1, 1 + nb_solved)
+        last_value = max(metric_tol, sorted_values[-1])
+        padded_values = np.hstack([sorted_values, [last_value]])
+        padded_y = np.hstack([y, [nb_solved]])
+        plt.step(padded_values, padded_y, linewidth=linewidth)
     plt.legend(plot_solvers)
-    plt.title(
-        f"Comparing {metric} on {test_set.title} with {settings} settings"
-    )
+    if title is None:
+        plt.title(
+            f"Comparing {metric} on {test_set.title} with {settings} settings"
+        )
+    elif title != "":
+        plt.title(title)
     plt.xlabel(metric)
     plt.xscale("log")
-    plt.axvline(x=metric_tol, color="r")
+    plt.axhline(y=nb_problems, color="gray", linestyle=":")
+    plt.axvline(x=metric_tol, color="gray", linestyle=":")
     plt.ylabel("# problems solved")
     plt.grid(True)
-    plt.show(block=True)
+    if savefig:
+        plt.savefig(fname=savefig)
+    else:  # display figure
+        plt.show(block=True)
```

### Comparing `qpsolvers_benchmark-0.1.0rc4/qpsolvers_benchmark/problem.py` & `qpsolvers_benchmark-1.0.0/qpsolvers_benchmark/problem.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,29 +11,25 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""
-Matrix-vector representation of a quadratic program.
-"""
+"""Matrix-vector representation of a quadratic program."""
 
 from typing import Optional, Union
 
 import numpy as np
 import qpsolvers
 import scipy.sparse as spa
 
 
 class Problem(qpsolvers.Problem):
-
-    """
-    Quadratic program.
+    """Quadratic program.
 
     Attributes:
         cost_offset: Cost offset, used to compare solution cost to a known
             optimal one. Defaults to zero.
         name: Name of the problem, for reporting.
         optimal_cost: If known, cost at the optimum of the problem.
     """
@@ -52,25 +48,22 @@
         b: Optional[np.ndarray],
         lb: Optional[np.ndarray],
         ub: Optional[np.ndarray],
         name: str,
         optimal_cost: Optional[float] = None,
         cost_offset: float = 0.0,
     ):
-        """
-        Quadratic program in qpsolvers format.
-        """
+        """Quadratic program in qpsolvers format."""
         super().__init__(P, q, G, h, A, b, lb, ub)
         self.cost_offset = cost_offset
         self.name = name
         self.optimal_cost = optimal_cost
 
     def to_dense(self):
-        """
-        Return dense version.
+        """Return dense version.
 
         Returns:
             Dense version of the present problem.
         """
         return Problem(
             self.P.toarray().astype(float),
             self.q,
@@ -82,16 +75,15 @@
             self.ub,
             name=self.name,
             optimal_cost=self.optimal_cost,
             cost_offset=self.cost_offset,
         )
 
     def to_sparse(self):
-        """
-        Return sparse version.
+        """Return sparse version.
 
         Returns:
             Sparse version of the present problem.
         """
         P, G, A = self.P, self.G, self.A
         return Problem(
             spa.csc_matrix(P) if isinstance(P, np.ndarray) else P,
@@ -104,26 +96,25 @@
             self.ub,
             name=self.name,
             optimal_cost=self.optimal_cost,
             cost_offset=self.cost_offset,
         )
 
     def cost_error(self, solution: qpsolvers.Solution) -> Optional[float]:
-        """
-        Compute difference between found cost and the optimal one.
+        """Compute difference between found cost and the optimal one.
 
         Args:
-            x: Primal solution.
+            solution: Problem solution.
 
         Returns:
             Cost error, i.e. deviation from the (known) optimal cost.
 
         Note:
             Cost errors can be negative when the primal residual is large. We
             count that as errors as well using absolute values.
         """
         x = solution.x
-        if x is None or self.optimal_cost is None:
+        if not solution.found or x is None or self.optimal_cost is None:
             return None
         P, q = self.P, self.q
         cost = 0.5 * x.dot(P.dot(x)) + q.dot(x) + self.cost_offset
         return abs(cost - self.optimal_cost)
```

### Comparing `qpsolvers_benchmark-0.1.0rc4/qpsolvers_benchmark/report.py` & `qpsolvers_benchmark-1.0.0/qpsolvers_benchmark/report.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,17 +11,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""
-Report written from test set results.
-"""
+"""Report written from test set results."""
 
 import datetime
 import io
 from importlib import metadata
 from typing import Dict
 
 import pandas
@@ -31,17 +29,15 @@
 from .spdlog import logging
 from .test_set import TestSet
 from .utils import capitalize_settings, get_cpu_info, get_solver_versions
 from .version import get_version
 
 
 class Report:
-
-    """
-    Report generated from benchmark results.
+    """Report generated from benchmark results.
 
     Attributes:
         author: GitHub username of the person who generated the report.
         results: Results from which the report should be generated.
         solver_settings: Dictionary of solver parameters for each settings.
         test_set: Test set from which results were generated.
     """
@@ -58,16 +54,15 @@
     __success_rate_df: pandas.DataFrame
     author: str
     results: Results
     solver_settings: Dict[str, SolverSettings]
     test_set: TestSet
 
     def __init__(self, author: str, results: Results):
-        """
-        Initialize report.
+        """Initialize report.
 
         Args:
             author: GitHub username of the person who generated the report.
             results: Results from which the report should be generated.
         """
         self.__correct_rate_df = pandas.DataFrame()
         self.__cost_df = pandas.DataFrame()
@@ -78,16 +73,15 @@
         self.__success_rate_df = pandas.DataFrame()
         self.author = author
         self.results = results
         self.solver_settings = results.test_set.solver_settings
         self.test_set = results.test_set
 
     def get_tolerances_table(self) -> str:
-        """
-        Get tolerances Markdown table.
+        """Get tolerances Markdown table.
 
         Returns:
             Tolerances Markdown table.
         """
         names = list(self.test_set.tolerances.keys())
         df = pandas.DataFrame(
             [],
@@ -111,16 +105,15 @@
                 ],
                 ignore_index=True,
             )
         df = df.sort_values(by="tolerance")
         return df.to_markdown(index=False)
 
     def get_solver_settings_table(self) -> str:
-        """
-        Get Markdown table for solver settings.
+        """Get Markdown table for solver settings.
 
         Returns:
             Solver settings Markdown table.
         """
         solver_settings = self.test_set.solver_settings
         names = list(solver_settings.keys())
         df = pandas.DataFrame(
@@ -155,16 +148,15 @@
                 ],
                 ignore_index=True,
             )
         df = df.sort_values(by=["solver", "parameter"])
         return df.to_markdown(index=False)
 
     def get_solver_versions_table(self):
-        """
-        Get Markdown table for solver versions.
+        """Get Markdown table for solver versions.
 
         Returns:
             Solver versions Markdown table.
         """
         versions = get_solver_versions(self.test_set.solvers)
         versions_df = pandas.DataFrame(
             {
@@ -174,17 +166,15 @@
         )
         versions_df = versions_df.set_index("solver")
         versions_df = versions_df.sort_index()
         versions_table = versions_df.to_markdown(index=True)
         return versions_table
 
     def __compute_dataframes(self) -> None:
-        """
-        Compute dataframes used in the report.
-        """
+        """Compute dataframes used in the report."""
         primal_tolerances = {
             name: tolerance.primal
             for name, tolerance in self.test_set.tolerances.items()
         }
         dual_tolerances = {
             name: tolerance.dual
             for name, tolerance in self.test_set.tolerances.items()
@@ -236,16 +226,15 @@
         self.__cost_df = self.results.build_shifted_geometric_mean_df(
             column="cost_error",
             shift=10.0,
             not_found_values=cost_tolerances,
         )
 
     def write(self, path: str) -> None:
-        """
-        Write report to a given path.
+        """Write report to a given path.
 
         Args:
             path: Path to the Markdown file to write the report to.
 
         Note:
             We make sure each table in the report is preceded by a single line
             title, for instance "Precentage of problems each solver is able to
@@ -256,21 +245,21 @@
         self.__compute_dataframes()
         with open(path, "w", encoding="UTF-8") as fh:
             self.__write_header(fh)
             self.__write_toc(fh)
             self.__write_description(fh)
             self.__write_solvers_section(fh)
             self.__write_settings_section(fh)
+            self.__write_limitations_section(fh)
             self.__write_results_by_settings(fh)
             self.__write_results_by_metric(fh)
         logging.info(f"Wrote report to {path}")
 
     def __write_header(self, fh: io.TextIOWrapper) -> None:
-        """
-        Write report header.
+        """Write report header.
 
         Args:
             fh: Output file handle.
         """
         benchmark_version = get_version()
         cpu_info = get_cpu_info()
         date = str(datetime.datetime.now(datetime.timezone.utc))
@@ -283,26 +272,26 @@
 | CPU     | {cpu_info} |
 | Run by  | [@{self.author}](https://github.com/{self.author}/) |
 
 """
         )
 
     def __write_toc(self, fh: io.TextIOWrapper) -> None:
-        """
-        Write table of contents.
+        """Write table of contents.
 
         Args:
             fh: Output file handle.
         """
         fh.write("## Contents\n\n")
         if self.test_set.description is not None:
             fh.write("* [Description](#description)\n")
         fh.write(
             """* [Solvers](#solvers)
 * [Settings](#settings)
+* [Known limitations](#known-limitations)
 * [Results by settings](#results-by-settings)\n"""
         )
         for name in self.solver_settings:
             link = name.replace("_", "-")
             fh.write(f"    * [{capitalize_settings(name)}](#{link})\n")
         fh.write(
             """* [Results by metric](#results-by-metric)
@@ -312,26 +301,24 @@
         * [Primal residual](#primal-residual)
         * [Dual residual](#dual-residual)
         * [Duality gap](#duality-gap)
     * [Cost error](#cost-error)\n\n"""
         )
 
     def __write_description(self, fh: io.TextIOWrapper) -> None:
-        """
-        Write optional Description section.
+        """Write optional Description section.
 
         Args:
             fh: Output file handle.
         """
         if self.test_set.description is not None:
             fh.write(f"## Description\n\n{self.test_set.description}\n\n")
 
     def __write_solvers_section(self, fh: io.TextIOWrapper) -> None:
-        """
-        Write Solvers section.
+        """Write Solvers section.
 
         Args:
             fh: Output file handle.
         """
         qpsolvers_version = metadata.version("qpsolvers")
         fh.write(
             f"""## Solvers
@@ -340,16 +327,15 @@
 
 All solvers were called via
 [qpsolvers](https://github.com/stephane-caron/qpsolvers)
 v{qpsolvers_version}.\n\n"""
         )
 
     def __write_settings_section(self, fh: io.TextIOWrapper) -> None:
-        """
-        Write Settings section.
+        """Write Settings section.
 
         Args:
             fh: Output file handle.
         """
         italics_settings = [f"*{x}*" for x in self.solver_settings]
         fh.write(
             f"""## Settings
@@ -361,17 +347,33 @@
 {self.get_tolerances_table()}
 
 Solvers for each settings are configured as follows:
 
 {self.get_solver_settings_table()}\n\n"""
         )
 
-    def __write_results_by_settings(self, fh: io.TextIOWrapper) -> None:
+    def __write_limitations_section(self, fh: io.TextIOWrapper) -> None:
+        """Write Known limitations section.
+
+        Args:
+            fh: Output file handle.
         """
-        Write Results by settings.
+        fh.write(
+            """## Known limitations
+
+The following [issues](https://github.com/qpsolvers/qpsolvers_benchmark/issues)
+have been identified as impacting the fairness of this benchmark. Keep them in
+mind when drawing conclusions from the results.
+
+- [#60](https://github.com/qpsolvers/qpsolvers_benchmark/issues/60):
+  Conversion to SOCP limits performance of ECOS\n\n"""
+        )
+
+    def __write_results_by_settings(self, fh: io.TextIOWrapper) -> None:
+        """Write Results by settings.
 
         Args:
             fh: Output file handle.
         """
         fh.write("""## Results by settings\n\n""")
         for settings in self.solver_settings:
             cols = {
@@ -397,16 +399,15 @@
 Solvers are compared over the whole test set by [shifted geometric
 mean](../README.md#shifted-geometric-mean) (shm). Lower is better.
 
 {df.to_markdown(index=True, floatfmt=".1f")}\n\n"""
             )
 
     def __write_results_by_metric(self, fh: io.TextIOWrapper) -> None:
-        """
-        Write Results by metric.
+        """Write Results by metric.
 
         Args:
             fh: Output file handle.
         """
         fh.write(
             f"""## Results by metric
```

### Comparing `qpsolvers_benchmark-0.1.0rc4/qpsolvers_benchmark/results.py` & `qpsolvers_benchmark-1.0.0/qpsolvers_benchmark/results.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,17 +11,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""
-Test case results.
-"""
+"""Test case results."""
 
 import os.path
 from typing import Dict, Tuple
 
 import numpy as np
 import pandas
 import qpsolvers
@@ -29,31 +27,28 @@
 from .problem import Problem
 from .shgeom import shgeom
 from .spdlog import logging
 from .test_set import TestSet
 
 
 class Results:
-
-    """
-    Test set results.
+    """Test set results.
 
     Attributes:
         csv_path: Path to the results CSV file.
         df: Data frame storing the results.
         test_set: Test set from which results were produced.
     """
 
     csv_path: str
     df: pandas.DataFrame
     test_set: TestSet
 
     def __init__(self, csv_path: str, test_set: TestSet):
-        """
-        Initialize results.
+        """Initialize results.
 
         Args:
             csv_path: Path to the results CSV file.
             test_set: Test set from which results were produced.
         """
         df = pandas.DataFrame(
             [],
@@ -85,24 +80,21 @@
             logging.info(f"Loading existing results from {csv_path}")
             df = pandas.concat([df, pandas.read_csv(csv_path)])
         self.csv_path = csv_path
         self.df = df
         self.test_set = test_set
 
     def write(self) -> None:
-        """
-        Write results to their CSV file for persistence.
-        """
+        """Write results to their CSV file for persistence."""
         logging.debug(f"Test set results written to {self.csv_path}")
         self.df = self.df.sort_values(by=["problem", "solver", "settings"])
         self.df.to_csv(self.csv_path, index=False)
 
     def has(self, problem: Problem, solver: str, settings: str) -> bool:
-        """
-        Check if results contain a given run of a solver on a problem.
+        """Check if results contain a given run of a solver on a problem.
 
         Args:
             problem: Test set problem.
             solver: Name of the QP solver.
             settings: Name of the corresponding solver settings.
 
         Returns:
@@ -113,17 +105,15 @@
             & (self.df["solver"] == solver)
             & (self.df["settings"] == settings)
         ).any()
 
     def is_timeout(
         self, problem: Problem, solver: str, settings: str, time_limit: float
     ) -> bool:
-        """
-        Check whether a particular result was a timeout.
-        """
+        """Check whether a particular result was a timeout."""
         runtime = self.df[
             (self.df["problem"] == problem.name)
             & (self.df["solver"] == solver)
             & (self.df["settings"] == settings)
         ]["runtime"].iat[0]
         return runtime > 0.99 * time_limit
 
@@ -131,16 +121,15 @@
         self,
         problem: Problem,
         solver: str,
         settings: str,
         solution: qpsolvers.Solution,
         runtime: float,
     ) -> None:
-        """
-        Update entry for a given (problem, solver) pair.
+        """Update entry for a given (problem, solver) pair.
 
         Args:
             problem: Problem solved.
             solver: Solver name.
             settings: Solver settings.
             solution: Solution found by the solver.
             runtime: Duration the solver took, in seconds.
@@ -157,15 +146,15 @@
                 self.df,
                 pandas.DataFrame(
                     {
                         "problem": [problem.name],
                         "solver": [solver],
                         "settings": [settings],
                         "runtime": [runtime],
-                        "found": [not solution.is_empty],
+                        "found": [solution.found],
                         "primal_residual": [solution.primal_residual()],
                         "dual_residual": [solution.dual_residual()],
                         "duality_gap": [solution.duality_gap()],
                         "cost_error": [problem.cost_error(solution)],
                     }
                 ),
             ],
@@ -175,16 +164,15 @@
     def build_success_rate_df(
         self,
         primal_tolerances: Dict[str, float],
         dual_tolerances: Dict[str, float],
         gap_tolerances: Dict[str, float],
         cost_tolerances: Dict[str, float],
     ) -> Tuple[pandas.DataFrame, pandas.DataFrame]:
-        """
-        Build the success-rate data frame.
+        """Build the success-rate data frame.
 
         Args:
             primal_tolerances: Primal-residual tolerance for each settings.
             dual_tolerances: Dual-residual tolerance for each settings.
             gap_tolerances: Duality-gap tolerance for each settings.
             cost_tolerances: Cost tolerance for each settings.
 
@@ -226,16 +214,15 @@
     def build_correct_rate_df(
         self,
         primal_tolerances: Dict[str, float],
         dual_tolerances: Dict[str, float],
         gap_tolerances: Dict[str, float],
         cost_tolerances: Dict[str, float],
     ) -> Tuple[pandas.DataFrame, pandas.DataFrame]:
-        """
-        Build the correctness-rate data frame.
+        """Build the correctness-rate data frame.
 
         Args:
             primal_tolerances: Primal-residual tolerance for each settings.
             dual_tolerances: Dual-residual tolerance for each settings.
             gap_tolerances: Duality-gap tolerance for each settings.
             cost_tolerances: Cost tolerance for each settings.
 
@@ -279,16 +266,15 @@
             .sort_index()
         )
         return correctness_rate_df
 
     def build_shifted_geometric_mean_df(
         self, column: str, shift: float, not_found_values: Dict[str, float]
     ) -> pandas.DataFrame:
-        """
-        Compute the shifted geometric mean of a results column.
+        """Compute the shifted geometric mean of a results column.
 
         Args:
             column: Name of the column to average.
             shift: Shift of the shifted geometric mean.
             not_found_values: Values to apply when a solver has not found a
                 solution (one per settings). For instance, time limits are used
                 for the runtime of a solver that fails to solve a problem.
```

### Comparing `qpsolvers_benchmark-0.1.0rc4/qpsolvers_benchmark/run.py` & `qpsolvers_benchmark-1.0.0/qpsolvers_benchmark/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,17 +11,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""
-Main function of the benchmark.
-"""
+"""Main function of the benchmark."""
 
 from time import perf_counter
 from typing import Optional
 
 import qpsolvers
 from qpsolvers.exceptions import SolverNotFound
 
@@ -37,16 +35,15 @@
     results: Results,
     only_problem: Optional[str] = None,
     only_settings: Optional[str] = None,
     only_solver: Optional[str] = None,
     rerun: bool = False,
     include_timeouts: bool = False,
 ) -> None:
-    """
-    Run a given test set and store results.
+    """Run a given test set and store results.
 
     Args:
         test_set: Test set to run.
         results: Results instance to write to.
         only_problem: If set, only run that specific problem in the set.
         only_settings: If set, only run with these solver settings.
         only_solver: If set, only run that specific solver.
```

### Comparing `qpsolvers_benchmark-0.1.0rc4/qpsolvers_benchmark/shgeom.py` & `qpsolvers_benchmark-1.0.0/qpsolvers_benchmark/shgeom.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,24 +11,21 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""
-Shifted geometric mean.
-"""
+"""Shifted geometric mean."""
 
 import numpy as np
 
 
 def shgeom(v: np.ndarray, sh: float) -> float:
-    """
-    `Shifted geometric mean <http://plato.asu.edu/ftp/shgeom.html>`_.
+    """`Shifted geometric mean <http://plato.asu.edu/ftp/shgeom.html>`_.
 
     Args:
         v: Nonnegative values.
         sh: Shift parameter.
 
     Note:
         The mean is computed as exponential of sum of logs to avoid memory
```

### Comparing `qpsolvers_benchmark-0.1.0rc4/qpsolvers_benchmark/solver_issues.py` & `qpsolvers_benchmark-1.0.0/qpsolvers_benchmark/solver_issues.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,27 +11,24 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""
-Some solvers fail on some problems. Make sure we handle and report those.
-"""
+"""Some solvers fail on some problems. Make sure we handle and report those."""
 
 from typing import Dict, Tuple
 
 from .problem import Problem
 from .spdlog import logging
 
 
 def skip_solver_issue(problem: Problem, solver: str) -> bool:
-    """
-    Check whether a solver is known to fail at solving a given problem.
+    """Check whether a solver is known to fail at solving a given problem.
 
     Args:
         problem: Problem to solve.
         solver: QP solver.
 
     Returns:
         True if solver is known to fail at solving the problem.
@@ -44,16 +41,15 @@
         return True
     return False
 
 
 def skip_solver_timeout(
     time_limit: float, problem: Problem, solver: str, settings: str
 ) -> bool:
-    """
-    Skip known solver timeouts.
+    """Skip known solver timeouts.
 
     Args:
         time_limit: Time limit in seconds.
         problem: Problem to solve.
         solver: QP solver.
         settings: QP solver settings.
```

### Comparing `qpsolvers_benchmark-0.1.0rc4/qpsolvers_benchmark/solver_settings.py` & `qpsolvers_benchmark-1.0.0/qpsolvers_benchmark/solver_settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,174 +11,168 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""
-Solver settings.
-"""
+"""Solver settings."""
 
 from typing import Any, Dict, Iterator, Set
 
 import numpy as np
 
 
 class SolverSettings:
-
-    """
-    Settings for multiple solvers.
-    """
+    """Settings for multiple solvers."""
 
     IMPLEMENTED_SOLVERS: Set[str] = set(
         [
+            "clarabel",
             "cvxopt",
+            "daqp",
             "ecos",
             "gurobi",
             "highs",
+            "nppro",
             "osqp",
             "proxqp",
             "qpoases",
             "qpswift",
             "quadprog",
             "scs",
         ]
     )
 
     @classmethod
     def is_implemented(cls, solver: str):
-        """
-        Check whether a solver is implemented by this class.
-        """
+        """Check whether a solver is implemented by this class."""
         return solver in cls.IMPLEMENTED_SOLVERS
 
     def __init__(self) -> None:
-        """
-        Initialize settings.
-        """
+        """Initialize settings."""
         self.__settings: Dict[str, Dict[str, Any]] = {
             solver: {} for solver in self.IMPLEMENTED_SOLVERS
         }
 
     def __getitem__(self, solver: str) -> Dict[str, Any]:
-        """
-        Get settings dictionary of a given solver.
+        """Get settings dictionary of a given solver.
 
         Args:
             solver: Name of the QP solver.
 
         Returns:
             Dictionary of custom solver settings.
         """
         return self.__settings[solver]
 
     def set_eps_abs(self, eps_abs: float) -> None:
-        """
-        Set absolute primal, dual and duality-gap tolerances for solvers that
-        support it.
+        r"""Set absolute tolerances for solvers that support it.
 
         Args:
             eps_abs: Absolute primal, dual and duality-gap tolerance.
 
         Notes:
-            When we set an absolute tolerance :math:`\\epsilon_{abs}` on
+            When we set an absolute tolerance :math:`\epsilon_{abs}` on
             residuals, we ask the solver to find an approximation of the
             optimum such that the primal residual, dual residual and duality
-            gap are below :math:`\\epsilon_{abs}`, that is:
+            gap are below :math:`\epsilon_{abs}`, that is:
 
             .. math::
 
-                \\begin{align}
-                r_p := \\max(\\| A x - b \\|_\\infty, [G x - h]^+, [lb - x]^+,
-                [x - ub]^+) & \\leq \\epsilon_{abs} \\\\
-                r_d := \\| P x + q + A^T y + G^T z + z_{box} \\|_\\infty &
-                \\leq \\epsilon_{abs} \\\\
+                \begin{align}
+                r_p := \max(\| A x - b \|_\infty, [G x - h]^+, [lb - x]^+,
+                [x - ub]^+) & \leq \epsilon_{abs} \\
+                r_d := \| P x + q + A^T y + G^T z + z_{box} \|_\infty &
+                \leq \epsilon_{abs} \\
                 r_g := | x^T P x + q^T x + b^T y + h^T z + lb^T z_{box}^- +
-                ub^T z_{box}^+ | & \\leq \\epsilon_{abs}
-                \\end{align}
+                ub^T z_{box}^+ | & \leq \epsilon_{abs}
+                \end{align}
 
-            were :math:`v^- = \\min(v, 0)` and :math:`v^+ = \\max(v, 0)`. The
+            were :math:`v^- = \min(v, 0)` and :math:`v^+ = \max(v, 0)`. The
             tolerance on the primal residual is called "feasibility tolerance"
             by some solvers, for instance CVXOPT and ECOS. See `this note
             <https://scaron.info/blog/optimality-conditions-and-numerical-tolerances-in-qp-solvers.html>`__
             for more details.
         """
+        self.__settings["clarabel"]["tol_feas"] = eps_abs
         self.__settings["cvxopt"]["feastol"] = eps_abs
+        self.__settings["daqp"]["dual_tol"] = eps_abs
+        self.__settings["daqp"]["primal_tol"] = eps_abs
         self.__settings["ecos"]["feastol"] = eps_abs
         self.__settings["gurobi"]["FeasibilityTol"] = eps_abs  # primal
         self.__settings["gurobi"]["OptimalityTol"] = eps_abs  # dual
         self.__settings["highs"]["dual_feasibility_tolerance"] = eps_abs
+
+        # Note on primal feasibility with HiGHS: "Primal feasibility is
+        # maintained rather than achieved (in contrast to IPM or ADMM based
+        # solvers) [...] changing the primal feasibility tolerance setting
+        # doesn't have any effect on QPs at the moment".
+        # https://github.com/ERGO-Code/HiGHS/issues/996#issuecomment-1561890995
         self.__settings["highs"]["primal_feasibility_tolerance"] = eps_abs
+
         self.__settings["osqp"]["eps_abs"] = eps_abs
         self.__settings["proxqp"]["eps_abs"] = eps_abs
         self.__settings["qpswift"]["RELTOL"] = eps_abs * np.sqrt(3.0)
         self.__settings["scs"]["eps_abs"] = eps_abs
 
     def set_eps_rel(self, eps_rel: float) -> None:
-        """
-        Set relative primal, dual and duality-gap tolerances for solvers that
-        support it.
+        """Set relative tolerances for solvers that support it.
 
         Args:
             eps_rel: Relative primal feasibility tolerance.
         """
         self.__settings["osqp"]["eps_rel"] = eps_rel
         self.__settings["proxqp"]["eps_rel"] = eps_rel
         self.__settings["scs"]["eps_rel"] = eps_rel
 
     def set_time_limit(self, time_limit: float) -> None:
-        """
-        Apply time limits to all solvers that support it.
+        """Apply time limits to all solvers that support it.
 
         Args:
             time_limit: Time limit in seconds.
         """
         self.__settings["gurobi"]["TimeLimit"] = time_limit
         self.__settings["highs"]["time_limit"] = time_limit
         self.__settings["osqp"]["time_limit"] = time_limit
         self.__settings["qpoases"]["time_limit"] = time_limit
         self.__settings["scs"]["time_limit_secs"] = time_limit
 
     def set_verbosity(self, verbose: bool) -> None:
-        """
-        Apply verbosity settings to all solvers.
+        """Apply verbosity settings to all solvers.
 
         Args:
             verbose: Verbosity boolean.
         """
         for solver in self.IMPLEMENTED_SOLVERS:
             self.__settings[solver]["verbose"] = verbose
 
     @property
     def solvers(self) -> Iterator[str]:
-        """
-        List solvers configured in these settings.
-        """
+        """List solvers configured in these settings."""
         for solver in self.__settings:
             yield solver
 
     def get_param(self, solver: str, param: str, default: str) -> Any:
-        """
-        Get solver parameter in these settings.
+        """Get solver parameter in these settings.
 
         Args:
             solver: QP solver.
             param: Parameter name.
             default: Value to return if the parameter is not configured.
 
         Returns:
             Corresponding solver parameter, or default value.
         """
         if solver not in self.__settings:
             return default
         return self.__settings[solver].get(param, default)
 
     def set_param(self, solver: str, param: str, value: Any) -> None:
-        """
-        Set solver parameter.
+        """Set solver parameter.
 
         Args:
             solver: QP solver.
             param: Parameter name.
+            value: Parameter value.
         """
         self.__settings[solver][param] = value
```

### Comparing `qpsolvers_benchmark-0.1.0rc4/qpsolvers_benchmark/spdlog.py` & `qpsolvers_benchmark-1.0.0/qpsolvers_benchmark/spdlog.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,28 +11,26 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""
+"""Logging with formatting similar to spdlog.
+
 Import ``logging`` from this module to use logging from Python standard library
 with formatting similar to spdlog.
 """
 
 import logging
 from typing import Any, Dict
 
 
 class SpdlogFormatter(logging.Formatter):
-
-    """
-    Custom logging formatter visually consistent with spdlog.
-    """
+    """Custom logging formatter visually consistent with spdlog."""
 
     BOLD_RED: str = "\033[31;1m"
     BOLD_WHITE: str = "\033[37;1m"
     BOLD_YELLOW: str = "\033[33;1m"
     GREEN: str = "\033[32m"
     MAGENTA: str = "\033[35m"
     ON_RED: str = "\033[41m"
@@ -43,14 +41,19 @@
         logging.DEBUG: f"[{MAGENTA}debug{RESET}]",
         logging.ERROR: f"[{BOLD_RED}error{RESET}]",
         logging.INFO: f"[{GREEN}info{RESET}]",
         logging.WARNING: f"[{BOLD_YELLOW}warning{RESET}]",
     }
 
     def format(self, record):
+        """Format for a logging record.
+
+        Args:
+            record: Record to format.
+        """
         custom_format = (
             "[%(asctime)s] "
             + self.LEVEL_FORMAT.get(record.levelno, "[???]")
             + " %(message)s (%(filename)s:%(lineno)d)"
         )
         formatter = logging.Formatter(custom_format)
         return formatter.format(record)
```

### Comparing `qpsolvers_benchmark-0.1.0rc4/qpsolvers_benchmark/test_set.py` & `qpsolvers_benchmark-1.0.0/qpsolvers_benchmark/test_set.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,83 +11,76 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""
-Base class for test sets.
-"""
+"""Base class for test sets."""
 
 import abc
 from typing import Dict, Iterator, Optional
 
 import qpsolvers
 
 from .exceptions import ProblemNotFound
 from .problem import Problem
 from .solver_settings import SolverSettings
 from .spdlog import logging
 from .tolerance import Tolerance
 
 
 class TestSet(abc.ABC):
+    """Abstract base class for a test set.
 
-    """
-    Abstract base class for a test test, i.e. a collection of problems with
-    solver settings.
+    A test set is a collection of problems with solver settings.
 
     Attributes:
         solver_settings: Dictionary of solver parameters for each settings.
         tolerances: Validation tolerances.
     """
 
     solver_settings: Dict[str, SolverSettings]
     tolerances: Dict[str, Tolerance]
 
     @abc.abstractmethod
     def __iter__(self) -> Iterator[Problem]:
-        """
-        Yield test problems one by one.
-        """
+        """Yield test problems one by one."""
 
     @property
     @abc.abstractmethod
     def description(self) -> str:
-        """
-        Test set description.
-        """
+        """Test set description."""
 
     @abc.abstractmethod
     def define_tolerances(self) -> None:
-        """
-        Define validation tolerances.
-        """
+        """Define validation tolerances."""
 
     def define_solver_settings(self) -> None:
-        """
-        Define solver settings.
-        """
+        """Define solver settings."""
         default = SolverSettings()
         default.set_param("qpoases", "predefined_options", "default")
         default.set_time_limit(self.tolerances["default"].runtime)
 
         high_accuracy = SolverSettings()
         high_accuracy.set_eps_abs(1e-9)
         high_accuracy.set_eps_rel(0.0)
+        high_accuracy.set_param("clarabel", "tol_gap_abs", 1e-9)
+        high_accuracy.set_param("clarabel", "tol_gap_rel", 0.0)
         high_accuracy.set_param("proxqp", "check_duality_gap", True)
         high_accuracy.set_param("proxqp", "eps_duality_gap_abs", 1e-9)
         high_accuracy.set_param("proxqp", "eps_duality_gap_rel", 0.0)
         high_accuracy.set_param("qpoases", "predefined_options", "reliable")
         high_accuracy.set_time_limit(self.tolerances["high_accuracy"].runtime)
 
         low_accuracy = SolverSettings()
         low_accuracy.set_eps_abs(1e-3)
         low_accuracy.set_eps_rel(0.0)
+        low_accuracy.set_param("clarabel", "tol_gap_abs", 1e-3)
+        low_accuracy.set_param("clarabel", "tol_gap_rel", 0.0)
         low_accuracy.set_param("proxqp", "check_duality_gap", True)
         low_accuracy.set_param("proxqp", "eps_duality_gap_abs", 1e-3)
         low_accuracy.set_param("proxqp", "eps_duality_gap_rel", 0.0)
         low_accuracy.set_param("qpoases", "predefined_options", "fast")
         low_accuracy.set_time_limit(self.tolerances["low_accuracy"].runtime)
 
         self.solver_settings = {
@@ -95,29 +88,23 @@
             "high_accuracy": high_accuracy,
             "low_accuracy": low_accuracy,
         }
 
     @property
     @abc.abstractmethod
     def sparse_only(self) -> bool:
-        """
-        If True, test set is restricted to solvers with a sparse matrix API.
-        """
+        """If True, restrict test set to solvers with a sparse matrix API."""
 
     @property
     @abc.abstractmethod
     def title(self) -> str:
-        """
-        Report title.
-        """
+        """Report title."""
 
     def __init__(self):
-        """
-        Initialize test set.
-        """
+        """Initialize test set."""
         candidate_solvers = set(
             qpsolvers.sparse_solvers
             if self.sparse_only
             else qpsolvers.available_solvers
         )
         solvers = set(
             solver
@@ -134,31 +121,40 @@
         self.tolerances = {}
         #
         self.define_tolerances()
         self.define_solver_settings()
         self.check_definitions()
 
     def check_definitions(self):
-        """
-        Check that settings and tolerance definitions are consistent.
+        """Check that settings and tolerance definitions are consistent.
 
         Raises:
             ValueError: in case of inconsistency.
         """
         tolerances = set(self.tolerances.keys())
         settings = set(self.solver_settings.keys())
         if tolerances != settings:
             logging.error("Settings are not consistent with tolerances")
             logging.info(f"Settings: {settings}")
             logging.info(f"Tolerances: {tolerances}")
             raise ValueError("Settings are not consistent with tolerances")
 
-    def get_problem(self, name: str) -> Optional[Problem]:
+    def count_problems(self) -> int:
+        """Count the number of problems in the set.
+
+        Returns:
+            Number of problems in the test set.
         """
-        Get a specific test set problem.
+        nb_problems = 0
+        for _ in self:
+            nb_problems += 1
+        return nb_problems
+
+    def get_problem(self, name: str) -> Optional[Problem]:
+        """Get a specific test set problem.
 
         Args:
             name: Problem name.
 
         Returns:
             Problem if found, None otherwise.
         """
```

### Comparing `qpsolvers_benchmark-0.1.0rc4/qpsolvers_benchmark/test_sets/__init__.py` & `qpsolvers_benchmark-1.0.0/qpsolvers_benchmark/version.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,10 +11,13 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""
-Test sets of the benchmark.
-"""
+"""Benchmark version."""
+
+
+def get_version() -> str:
+    """Get benchmark version as a string."""
+    return "1.0.0"
```

### Comparing `qpsolvers_benchmark-0.1.0rc4/qpsolvers_benchmark/tolerance.py` & `qpsolvers_benchmark-1.0.0/qpsolvers_benchmark/tolerance.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,28 +11,24 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""
-Tolerances on solver solution validation.
-"""
+"""Tolerances on solver solution validation."""
 
 from dataclasses import dataclass
 
 from .exceptions import BenchmarkError
 
 
 @dataclass
 class Tolerance:
-
-    """
-    Tolerances on solver solution validation.
+    """Tolerances on solver solution validation.
 
     Attributes:
         cost: Cost tolerance.
         primal: Tolerance on primal residuals.
         dual: Tolerance on dual residuals.
         gap: Tolerance on duality gaps.
         runtime: Time limit in seconds.
@@ -41,14 +37,22 @@
     cost: float
     primal: float
     dual: float
     gap: float
     runtime: float
 
     def from_metric(self, metric: str) -> float:
+        """Get tolerance corresponding to a given metric.
+
+        Args:
+            metric: Metric to get the tolerance of.
+
+        Returns:
+            Corresponding tolerance.
+        """
         if metric == "primal_residual":
             return self.primal
         if metric == "dual_residual":
             return self.dual
         if metric == "duality_gap":
             return self.gap
         if metric == "runtime":
```

### Comparing `qpsolvers_benchmark-0.1.0rc4/qpsolvers_benchmark/utils.py` & `qpsolvers_benchmark-1.0.0/qpsolvers_benchmark/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,23 +11,22 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""
-Utility functions.
-"""
+"""Utility functions."""
 
 import platform
 from importlib import import_module, metadata
 from time import perf_counter
 from typing import Set, Tuple
 
+import numpy as np
 import qpsolvers
 
 from .problem import Problem
 from .spdlog import logging
 
 try:
     import cpuinfo
@@ -35,43 +34,40 @@
     cpuinfo = None
     logging.warning(
         "Run ``pip install py-cpuinfo`` for more accurate CPU info"
     )
 
 
 def capitalize_settings(name: str) -> str:
-    """
-    Capitalize settings name.
+    """Capitalize settings name.
 
     Args:
         name: Settings name, e.g. "low_accuracy".
 
     Returns:
         Capitalized settings name to use as column title, e.g. "Low accuracy".
     """
     return name.replace("_", " ").capitalize()
 
 
 def get_cpu_info() -> str:
-    """
-    Get CPU information.
+    """Get CPU information.
 
     Returns:
         CPU information.
     """
     return (
         platform.processor()
         if cpuinfo is None
         else cpuinfo.get_cpu_info()["brand_raw"]
     )
 
 
 def get_solver_versions(solvers: Set[str]):
-    """
-    Get version numbers for a given set of solvers.
+    """Get version numbers for a given set of solvers.
 
     Args:
         solvers: Names of solvers to get the version of.
 
     Returns:
         Dictionary mapping solver names to their versions.
     """
@@ -105,31 +101,43 @@
         versions["gurobi"] += " (size-limited)"
     return versions
 
 
 def time_solve_problem(
     problem: Problem, solver: str, **kwargs
 ) -> Tuple[qpsolvers.Solution, float]:
-    """
-    Solve quadratic program.
+    """Solve quadratic program.
 
     Args:
         problem: Quadratic program to solve.
         solver: Name of the backend QP solver to call.
+        kwargs: Keyword arguments forwarded to underlying solver.
 
     Returns:
         Solution to the quadratic program, along with the time the solver took
         to compute it.
     """
     # Don't time matrix conversions for solvers that require sparse inputs
-    if solver in ["highs", "osqp", "scs"]:
+    if (
+        solver in qpsolvers.sparse_solvers
+        and solver not in qpsolvers.dense_solvers
+    ):
         problem = problem.to_sparse()
     start_time = perf_counter()
     try:
         solution = qpsolvers.solve_problem(problem, solver=solver, **kwargs)
     except Exception as e:  # pylint: disable=W0703
         # TODO(scaron): wait for qpsolvers update regarding exceptions
         # See https://github.com/stephane-caron/qpsolvers/pull/139
         logging.warning(f"Caught solver {type(e).__name__} exception: {e}")
         solution = qpsolvers.Solution(problem)
     runtime = perf_counter() - start_time
     return solution, runtime
+
+
+def is_posdef(M: np.ndarray) -> bool:
+    """Test whether a matrix is positive-definite.
+
+    Args:
+        M: Matrix to test.
+    """
+    return all(np.linalg.eigvals(M) > 0)
```

### Comparing `qpsolvers_benchmark-0.1.0rc4/setup.py` & `qpsolvers_benchmark-1.0.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,52 @@
 #!/usr/bin/env python
 # setup.py generated by flit for tools that don't yet use PEP 517
 
 from distutils.core import setup
 
 packages = \
-['qpsolvers_benchmark',
- 'qpsolvers_benchmark.test_sets',
- 'qpsolvers_benchmark.test_sets.github_ffa_problems']
+['qpsolvers_benchmark']
 
 package_data = \
-{'': ['*']}
+{'': ['*'],
+ 'qpsolvers_benchmark': ['test_sets/*', 'test_sets/github_ffa_problems/*']}
 
 install_requires = \
-['cvxopt >=1.2.6',
+['clarabel >=0.4.1',
+ 'cvxopt >=1.2.6',
  'ecos >=2.0.8',
  'highspy >=1.1.2.dev3',
+ 'matplotlib >=3.6.2',
  'osqp >=0.6.2',
  'pandas >=1.4.3',
  'proxsuite >=0.3.0',
- 'qpsolvers >=2.7.2',
+ 'qpsolvers >=3.4.0',
  'quadprog >=0.1.11',
  'scs >=3.2.0',
  'tabulate >=0.9.0']
 
 extras_require = \
 {'open_source_solvers': ['cvxopt >= 1.3.0',
                          'ecos >= 2.0.10',
                          'highspy >= 1.1.2',
                          'osqp >= 0.6.2',
                          'proxsuite >= 0.3.0',
                          'quadprog >= 0.1.11',
                          'scs >= 3.2.2']}
 
+entry_points = \
+{'console_scripts': ['qpsolvers_benchmark = '
+                     'qpsolvers_benchmark.benchmark:main']}
+
 setup(name='qpsolvers_benchmark',
-      version='0.1.0rc4',
+      version='1.0.0',
       description='Benchmark for quadratic programming solvers available in Python.',
       author=None,
       author_email='Stéphane Caron <stephane.caron@normalesup.org>',
       url=None,
       packages=packages,
       package_data=package_data,
       install_requires=install_requires,
       extras_require=extras_require,
+      entry_points=entry_points,
       python_requires='>=3.7',
      )
```

### Comparing `qpsolvers_benchmark-0.1.0rc4/PKG-INFO` & `qpsolvers_benchmark-1.0.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qpsolvers_benchmark
-Version: 0.1.0rc4
+Version: 1.0.0
 Summary: Benchmark for quadratic programming solvers available in Python.
 Keywords: quadratic programming,benchmark,solvers,numerical optimization
 Author-email: Stéphane Caron <stephane.caron@normalesup.org>
 Maintainer-email: Stéphane Caron <stephane.caron@normalesup.org>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
@@ -13,21 +13,23 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Mathematics
+Requires-Dist: clarabel >=0.4.1
 Requires-Dist: cvxopt >=1.2.6
 Requires-Dist: ecos >=2.0.8
 Requires-Dist: highspy >=1.1.2.dev3
+Requires-Dist: matplotlib >=3.6.2
 Requires-Dist: osqp >=0.6.2
 Requires-Dist: pandas >=1.4.3
 Requires-Dist: proxsuite >=0.3.0
-Requires-Dist: qpsolvers >=2.7.2
+Requires-Dist: qpsolvers >=3.4.0
 Requires-Dist: quadprog >=0.1.11
 Requires-Dist: scs >=3.2.0
 Requires-Dist: tabulate >=0.9.0
 Requires-Dist: cvxopt >= 1.3.0 ; extra == "open_source_solvers"
 Requires-Dist: ecos >= 2.0.10 ; extra == "open_source_solvers"
 Requires-Dist: highspy >= 1.1.2 ; extra == "open_source_solvers"
 Requires-Dist: osqp >= 0.6.2 ; extra == "open_source_solvers"
@@ -37,47 +39,66 @@
 Project-URL: Changelog, https://github.com/stephane-caron/qpsolvers_benchmark/blob/master/CHANGELOG.md
 Project-URL: Source, https://github.com/stephane-caron/qpsolvers_benchmark
 Project-URL: Tracker, https://github.com/stephane-caron/qpsolvers_benchmark/issues
 Provides-Extra: open_source_solvers
 
 # QP solvers benchmark
 
-[![Build](https://img.shields.io/github/actions/workflow/status/stephane-caron/qpsolvers_benchmark/CI.yml?branch=main)](https://github.com/stephane-caron/qpsolvers_benchmark/actions)
+[![Build](https://img.shields.io/github/actions/workflow/status/stephane-caron/qpsolvers_benchmark/ci.yml?branch=main)](https://github.com/stephane-caron/qpsolvers_benchmark/actions)
 [![PyPI version](https://img.shields.io/pypi/v/qpsolvers_benchmark)](https://pypi.org/project/qpsolvers_benchmark/)
 [![Contributing](https://img.shields.io/badge/PRs-welcome-green.svg)](https://github.com/stephane-caron/qpsolvers_benchmark/tree/master/CONTRIBUTING.md)
 
 Benchmark for quadratic programming (QP) solvers available in Python.
 
-The goal of this benchmark is to help us compare and select QP solvers. Its methodology is open to [discussions](https://github.com/stephane-caron/qpsolvers_benchmark/discussions). New test sets are [also welcome](CONTRIBUTING.md). Feel free to add one that better represents the kind of problems you are working on.
+The goal of this benchmark is to help users compare and select QP solvers. Its methodology is open to [discussions](https://github.com/stephane-caron/qpsolvers_benchmark/discussions). The benchmark ships standard and community [test sets](#test-sets), as well as a ``qpsolvers_benchmark`` command-line tool to run any test set directly on your machine. For instance:
+
+```console
+qpsolvers_benchmark maros_meszaros/maros_meszaros.py run
+```
+
+The outcome from running a test set is a standardized report evaluating all [metrics](#metrics) of the benchmark across all available QP solvers. This repository also distributes [results](#results) from running the benchmark on all test sets using the same computer.
+
+New test sets are [welcome](CONTRIBUTING.md). The benchmark is designed so that each test-set directory is standalone, so that the ``qpsolvers_benchmark`` command can be run on test sets from other repositories. Feel free to create ones that better represent the kind of problems you are working on.
 
 ## Solvers
 
 | Solver | Keyword | Algorithm | Matrices | License |
 | ------ | ------- | --------- | -------- | ------- |
+| [Clarabel](https://github.com/oxfordcontrol/Clarabel.rs) | ``clarabel`` | Interior point | Sparse | Apache-2.0 |
 | [CVXOPT](http://cvxopt.org/) | ``cvxopt`` | Interior point | Dense | GPL-3.0 |
+| [DAQP](https://github.com/darnstrom/daqp) | ``daqp`` | Active set | Dense | MIT |
 | [ECOS](https://web.stanford.edu/~boyd/papers/ecos.html) | ``ecos`` | Interior point | Sparse | GPL-3.0 |
 | [Gurobi](https://www.gurobi.com/) | ``gurobi`` | Interior point | Sparse | Commercial |
 | [HiGHS](https://highs.dev/) | ``highs`` | Active set | Sparse | MIT |
 | [MOSEK](https://mosek.com/) | ``mosek`` | Interior point | Sparse | Commercial |
+| NPPro | ``nppro`` | Active set | Dense | Commercial |
 | [OSQP](https://osqp.org/) | ``osqp`` | Douglas–Rachford | Sparse | Apache-2.0 |
 | [ProxQP](https://github.com/Simple-Robotics/proxsuite) | ``proxqp`` | Augmented Lagrangian | Dense & Sparse | BSD-2-Clause |
 | [qpOASES](https://github.com/coin-or/qpOASES) | ``qpoases`` | Active set | Dense | LGPL-2.1 |
 | [qpSWIFT](https://qpswift.github.io/) | ``qpswift`` | Interior point | Sparse | GPL-3.0 |
 | [quadprog](https://pypi.python.org/pypi/quadprog/) | ``quadprog`` | Goldfarb-Idnani | Dense | GPL-2.0 |
 | [SCS](https://www.cvxgrp.org/scs/) | ``scs`` | Douglas–Rachford | Sparse | MIT |
 
-## Test sets and results
+## Test sets
 
-The benchmark has different test sets that represent different use cases for QP solvers. Click on a test set to check out its report.
+The benchmark comes with standard and community test sets to represent different use cases for QP solvers:
 
 | Test set | Keyword | Description |
 | -------- | ------- | ----------- |
-| [GitHub free-for-all](results/github_ffa.md) | ``github_ffa`` | Test set built by the community on GitHub, new problems [are welcome](https://github.com/stephane-caron/qpsolvers_benchmark/issues/new?assignees=&labels=&template=new_problem.md&title=)! |
-| [Maros-Meszaros](results/maros_meszaros.md) | ``maros_meszaros`` | Standard set of problems designed to be difficult. |
-| [Maros-Meszaros dense](results/maros_meszaros_dense.md) | ``maros_meszaros_dense`` | Subset of the Maros-Meszaros test set restricted to smaller dense problems. |
+| **GitHub free-for-all** | ``github_ffa`` | Test set built by the community on GitHub, new problems [are welcome](https://github.com/stephane-caron/qpsolvers_benchmark/issues/new?assignees=&labels=&template=new_problem.md&title=)! |
+| **Maros-Meszaros** | ``maros_meszaros`` | Standard set of problems designed to be difficult. |
+| **Maros-Meszaros dense** | ``maros_meszaros_dense`` | Subset of the Maros-Meszaros test set restricted to smaller dense problems. |
+
+## Results
+
+The outcome from running a test set is a standardized report. Here are the results obtained from running all test sets in this repository with the same computer:
+
+* [GitHub free-for-all](github_ffa/results/github_ffa.md)
+* [Maros-Meszaros](maros_meszaros/results/maros_meszaros.md)
+* [Maros-Meszaros dense](maros_meszaros/results/maros_meszaros_dense.md)
 
 ## Metrics
 
 We evaluate QP solvers based on the following metrics:
 
 - **Success rate:** percentage of problems a solver is able to solve on a given test set.
 - **Computation time:** time a solver takes to solve a given problem.
@@ -119,27 +140,39 @@
 pip install qpsolvers_benchmark
 ```
 
 By default, the benchmark will run all supported solvers it finds.
 
 ## Running the benchmark
 
-Pick up the keyword corresponding to the desired [test set](#test-sets), for instance ``maros_meszaros``, and pass it to the ``run`` command:
+Once the benchmark is installed, you will be able to run the ``qpsolvers_benchmark`` command. Provide it with the script corresponding to the [test set](#test-sets) you want to run, followed by a benchmark command such as "run". For instance, let's run the "dense" subset of the Maros-Meszaros test set:
 
 ```console
-python benchmark.py maros_meszaros run
+qpsolvers_benchmark maros_meszaros/maros_meszaros_dense.py run
 ```
 
 You can also run a specific solver, problem or set of solver settings:
 
 ```console
-python benchmark.py maros_meszaros_dense run --solver proxqp --settings default
+qpsolvers_benchmark maros_meszaros/maros_meszaros_dense.py run --solver proxqp --settings default
 ```
 
-Check out ``python benchmark.py --help`` for all available commands and arguments.
+Check out ``qpsolvers_benchmark --help`` for a list of available commands and arguments.
+
+## Plots
+
+The command line ships a ``plot`` command to compare solver performances over a test set for a specific metric. For instance, run:
+
+```console
+qpsolvers_benchmark maros_meszaros/maros_meszaros_dense.py plot runtime high_accuracy
+```
+
+To generate the following plot:
+
+![image](https://user-images.githubusercontent.com/1189580/220150365-530cd685-fc90-49b5-90e0-0b243fa602d9.png)
 
 ## Contributing
 
 Contributions to improving this benchmark are welcome. You can for instance propose new problems, or share the runtimes you obtain on your machine. Check out the [contribution guidelines](CONTRIBUTING.md) for details.
 
 ## See also
```

