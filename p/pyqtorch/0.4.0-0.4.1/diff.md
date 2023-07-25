# Comparing `tmp/pyqtorch-0.4.0.tar.gz` & `tmp/pyqtorch-0.4.1.tar.gz`

## Comparing `pyqtorch-0.4.0.tar` & `pyqtorch-0.4.1.tar`

### file list

```diff
@@ -1,64 +1,63 @@
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/CONTRIBUTING.md
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/README.md
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/mkdocs.yml
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/publish.sh
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/readthedocs.yml
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/setup.py
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/.github/workflows/run-tests-and-mypy.yml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/docs/CODE_OF_CONDUCT.md -> ../CODE_OF_CONDUCT.md
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/docs/CONTRIBUTING.md -> ../CONTRIBUTING.md
--rw-r--r--   0        0        0    57645 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/docs/QAOA.ipynb
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/docs/circuit.md
--rw-r--r--   0        0        0     6493 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/docs/essentials.ipynb
--rw-r--r--   0        0        0   154246 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/docs/fit_function.ipynb
--rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/docs/gate_composition.ipynb
--rw-r--r--   0        0        0     4634 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/docs/hamevo.md
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/docs/index.md
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/docs/matrices.md
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/docs/parametric.md
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/docs/primitive.md
--rw-r--r--   0        0        0    46162 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/docs/deprecated/QAOA.ipynb
--rw-r--r--   0        0        0    19339 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/docs/deprecated/bench.py
--rw-r--r--   0        0        0    74042 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/docs/deprecated/fit_function.ipynb
--rw-r--r--   0        0        0    74062 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/docs/deprecated/getting_started.ipynb
--rw-r--r--   0        0        0   121176 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/docs/deprecated/ham_evol_comparison.ipynb
--rw-r--r--   0        0        0     6459 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/docs/deprecated/state_evolution.ipynb
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/pyqtorch/__init__.py
--rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/pyqtorch/ansatz.py
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/pyqtorch/embedding.py
--rw-r--r--   0        0        0     4939 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/pyqtorch/matrices.py
--rw-r--r--   0        0        0     6255 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/pyqtorch/matrices_sparse.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/pyqtorch/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/pyqtorch/converters/__init__.py
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/pyqtorch/converters/store_ops.py
--rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/pyqtorch/converters/to_qiskit.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/pyqtorch/core/__init__.py
--rw-r--r--   0        0        0    24532 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/pyqtorch/core/batched_operation.py
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/pyqtorch/core/circuit.py
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/pyqtorch/core/measurement.py
--rw-r--r--   0        0        0    23548 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/pyqtorch/core/operation.py
--rw-r--r--   0        0        0     6499 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/pyqtorch/core/utils.py
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/pyqtorch/modules/__init__.py
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/pyqtorch/modules/abstract.py
--rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/pyqtorch/modules/apply.py
--rw-r--r--   0        0        0     6904 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/pyqtorch/modules/circuit.py
--rw-r--r--   0        0        0    12217 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/pyqtorch/modules/hamevo.py
--rw-r--r--   0        0        0    14141 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/pyqtorch/modules/parametric.py
--rw-r--r--   0        0        0    13235 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/pyqtorch/modules/primitive.py
--rw-r--r--   0        0        0     5393 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/pyqtorch/modules/utils.py
--rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/tests/conftest.py
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/tests/test_batched_operations.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/tests/test_circ_matrices.py
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/tests/test_converters.py
--rw-r--r--   0        0        0     8146 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/tests/test_module_hamevo.py
--rw-r--r--   0        0        0    10001 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/tests/test_modules.py
--rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/tests/test_notebooks.py
--rw-r--r--   0        0        0     6034 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/tests/test_operations.py
--rw-r--r--   0        0        0     6496 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/tests/test_operations_hamevo.py
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/tests/test_sparse_modules.py
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/LICENSE
--rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 pyqtorch-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/README.md
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/mkdocs.yml
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/readthedocs.yml
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/setup.py
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/.github/workflows/run-tests-and-mypy.yml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/docs/CODE_OF_CONDUCT.md -> ../CODE_OF_CONDUCT.md
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/docs/CONTRIBUTING.md -> ../CONTRIBUTING.md
+-rw-r--r--   0        0        0    57645 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/docs/QAOA.ipynb
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/docs/circuit.md
+-rw-r--r--   0        0        0     6493 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/docs/essentials.ipynb
+-rw-r--r--   0        0        0   154246 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/docs/fit_function.ipynb
+-rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/docs/gate_composition.ipynb
+-rw-r--r--   0        0        0     4634 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/docs/hamevo.md
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/docs/index.md
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/docs/matrices.md
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/docs/parametric.md
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/docs/primitive.md
+-rw-r--r--   0        0        0    46162 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/docs/deprecated/QAOA.ipynb
+-rw-r--r--   0        0        0    19339 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/docs/deprecated/bench.py
+-rw-r--r--   0        0        0    74042 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/docs/deprecated/fit_function.ipynb
+-rw-r--r--   0        0        0    74062 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/docs/deprecated/getting_started.ipynb
+-rw-r--r--   0        0        0   121176 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/docs/deprecated/ham_evol_comparison.ipynb
+-rw-r--r--   0        0        0     6459 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/docs/deprecated/state_evolution.ipynb
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/pyqtorch/__init__.py
+-rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/pyqtorch/ansatz.py
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/pyqtorch/embedding.py
+-rw-r--r--   0        0        0     4939 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/pyqtorch/matrices.py
+-rw-r--r--   0        0        0     6255 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/pyqtorch/matrices_sparse.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/pyqtorch/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/pyqtorch/converters/__init__.py
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/pyqtorch/converters/store_ops.py
+-rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/pyqtorch/converters/to_qiskit.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/pyqtorch/core/__init__.py
+-rw-r--r--   0        0        0    24532 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/pyqtorch/core/batched_operation.py
+-rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/pyqtorch/core/circuit.py
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/pyqtorch/core/measurement.py
+-rw-r--r--   0        0        0    23548 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/pyqtorch/core/operation.py
+-rw-r--r--   0        0        0     6499 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/pyqtorch/core/utils.py
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/pyqtorch/modules/__init__.py
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/pyqtorch/modules/abstract.py
+-rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/pyqtorch/modules/apply.py
+-rw-r--r--   0        0        0     6904 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/pyqtorch/modules/circuit.py
+-rw-r--r--   0        0        0    12217 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/pyqtorch/modules/hamevo.py
+-rw-r--r--   0        0        0    15727 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/pyqtorch/modules/parametric.py
+-rw-r--r--   0        0        0    13235 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/pyqtorch/modules/primitive.py
+-rw-r--r--   0        0        0     5393 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/pyqtorch/modules/utils.py
+-rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/tests/conftest.py
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/tests/test_batched_operations.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/tests/test_circ_matrices.py
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/tests/test_converters.py
+-rw-r--r--   0        0        0     8146 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/tests/test_module_hamevo.py
+-rw-r--r--   0        0        0    11404 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/tests/test_modules.py
+-rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/tests/test_notebooks.py
+-rw-r--r--   0        0        0     6034 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/tests/test_operations.py
+-rw-r--r--   0        0        0     6496 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/tests/test_operations_hamevo.py
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/tests/test_sparse_modules.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/LICENSE
+-rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 pyqtorch-0.4.1/PKG-INFO
```

### Comparing `pyqtorch-0.4.0/.pre-commit-config.yaml` & `pyqtorch-0.4.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.0/CODE_OF_CONDUCT.md` & `pyqtorch-0.4.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.0/CONTRIBUTING.md` & `pyqtorch-0.4.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.0/mkdocs.yml` & `pyqtorch-0.4.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.0/.github/workflows/run-tests-and-mypy.yml` & `pyqtorch-0.4.1/.github/workflows/run-tests-and-mypy.yml`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.0/docs/QAOA.ipynb` & `pyqtorch-0.4.1/docs/QAOA.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.0/docs/essentials.ipynb` & `pyqtorch-0.4.1/docs/essentials.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.0/docs/fit_function.ipynb` & `pyqtorch-0.4.1/docs/fit_function.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.0/docs/gate_composition.ipynb` & `pyqtorch-0.4.1/docs/gate_composition.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.0/docs/hamevo.md` & `pyqtorch-0.4.1/docs/hamevo.md`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.0/docs/deprecated/QAOA.ipynb` & `pyqtorch-0.4.1/docs/deprecated/QAOA.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.0/docs/deprecated/bench.py` & `pyqtorch-0.4.1/docs/deprecated/bench.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.0/docs/deprecated/fit_function.ipynb` & `pyqtorch-0.4.1/docs/deprecated/fit_function.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.0/docs/deprecated/getting_started.ipynb` & `pyqtorch-0.4.1/docs/deprecated/getting_started.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.0/docs/deprecated/ham_evol_comparison.ipynb` & `pyqtorch-0.4.1/docs/deprecated/ham_evol_comparison.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.0/docs/deprecated/state_evolution.ipynb` & `pyqtorch-0.4.1/docs/deprecated/state_evolution.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.0/pyqtorch/__init__.py` & `pyqtorch-0.4.1/pyqtorch/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.0/pyqtorch/ansatz.py` & `pyqtorch-0.4.1/pyqtorch/ansatz.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.0/pyqtorch/embedding.py` & `pyqtorch-0.4.1/pyqtorch/embedding.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.0/pyqtorch/matrices.py` & `pyqtorch-0.4.1/pyqtorch/matrices.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.0/pyqtorch/matrices_sparse.py` & `pyqtorch-0.4.1/pyqtorch/matrices_sparse.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.0/pyqtorch/converters/store_ops.py` & `pyqtorch-0.4.1/pyqtorch/converters/store_ops.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.0/pyqtorch/converters/to_qiskit.py` & `pyqtorch-0.4.1/pyqtorch/converters/to_qiskit.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.0/pyqtorch/core/__init__.py` & `pyqtorch-0.4.1/pyqtorch/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.0/pyqtorch/core/batched_operation.py` & `pyqtorch-0.4.1/pyqtorch/core/batched_operation.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.0/pyqtorch/core/circuit.py` & `pyqtorch-0.4.1/pyqtorch/core/circuit.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.0/pyqtorch/core/measurement.py` & `pyqtorch-0.4.1/pyqtorch/core/measurement.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.0/pyqtorch/core/operation.py` & `pyqtorch-0.4.1/pyqtorch/core/operation.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.0/pyqtorch/core/utils.py` & `pyqtorch-0.4.1/pyqtorch/core/utils.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.0/pyqtorch/modules/__init__.py` & `pyqtorch-0.4.1/pyqtorch/modules/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pyqtorch.modules.circuit import (
     EntanglingLayer,
     FeaturemapLayer,
     QuantumCircuit,
     VariationalLayer,
 )
 from pyqtorch.modules.hamevo import HamEvo, HamEvoEig, HamEvoExp, HamEvoType, HamiltonianEvolution
-from pyqtorch.modules.parametric import CPHASE, CRX, CRY, CRZ, RX, RY, RZ, U
+from pyqtorch.modules.parametric import CPHASE, CRX, CRY, CRZ, PHASE, RX, RY, RZ, U
 from pyqtorch.modules.primitive import CNOT, CSWAP, CY, CZ, SWAP, H, I, S, Sdagger, T, X, Y, Z
 from pyqtorch.modules.utils import (
     is_normalized,
     normalize,
     overlap,
     random_state,
     uniform_state,
```

### Comparing `pyqtorch-0.4.0/pyqtorch/modules/abstract.py` & `pyqtorch-0.4.1/pyqtorch/modules/abstract.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.0/pyqtorch/modules/apply.py` & `pyqtorch-0.4.1/pyqtorch/modules/apply.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.0/pyqtorch/modules/circuit.py` & `pyqtorch-0.4.1/pyqtorch/modules/circuit.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.0/pyqtorch/modules/hamevo.py` & `pyqtorch-0.4.1/pyqtorch/modules/hamevo.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.0/pyqtorch/modules/parametric.py` & `pyqtorch-0.4.1/pyqtorch/modules/parametric.py`

 * *Files 2% similar despite different names*

```diff
@@ -225,14 +225,59 @@
         result = rz_gate(z_state, theta)
         print(result)
         ```
         """
         super().__init__("Z", qubits, n_qubits)
 
 
+class PHASE(RotationGate):
+    def __init__(self, qubits: ArrayLike, n_qubits: int):
+        """
+        Represents a PHASE rotation gate in a quantum circuit.
+
+        Arguments:
+            qubits (ArrayLike): The qubit index or list of qubit indices.
+            n_qubits (int): The total number of qubits in the circuit.
+
+        Examples:
+        ```python exec="on" source="above" result="json"
+        import torch
+        import pyqtorch.modules as pyq
+
+        # Create an PHASE gate
+        gate = pyq.PHASE(qubits=[0], n_qubits=1)
+
+        # Create a zero state
+        z_state = pyq.zero_state(n_qubits=1)
+
+        # Create a random theta angle
+        theta = torch.rand(1)
+
+        # Apply the PHASE gate to the zero state with the random theta angle
+        result = gate(z_state, theta)
+        print(result)
+        ```
+        """
+        super().__init__("I", qubits, n_qubits)
+
+    def apply(self, matrices: torch.Tensor, state: torch.Tensor) -> torch.Tensor:
+        batch_size = matrices.size(-1)
+        return _apply_batch_gate(state, matrices, self.qubits, self.n_qubits, batch_size)
+
+    def forward(self, state: torch.Tensor, thetas: torch.Tensor) -> torch.Tensor:
+        mats = self.matrices(thetas)
+        return self.apply(mats, state)
+
+    def matrices(self, thetas: torch.Tensor) -> torch.Tensor:
+        theta = thetas.squeeze(0) if thetas.ndim == 2 else thetas
+        batch_mat = self.imat.unsqueeze(2).repeat(1, 1, len(theta))
+        batch_mat[1, 1, :] = torch.exp(torch.tensor(1.0j * thetas)).unsqueeze(0).unsqueeze(1)
+        return batch_mat
+
+
 class CRX(ControlledRotationGate):
     def __init__(self, qubits: ArrayLike, n_qubits: int):
         """
         Represents a controlled-X-axis rotation (CRX) gate in a quantum circuit.
         The CRX gate class creates a controlled RX gate, applying the RX according
         to the control qubit state.
```

### Comparing `pyqtorch-0.4.0/pyqtorch/modules/primitive.py` & `pyqtorch-0.4.1/pyqtorch/modules/primitive.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.0/pyqtorch/modules/utils.py` & `pyqtorch-0.4.1/pyqtorch/modules/utils.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.0/tests/conftest.py` & `pyqtorch-0.4.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.0/tests/test_batched_operations.py` & `pyqtorch-0.4.1/tests/test_batched_operations.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.0/tests/test_circ_matrices.py` & `pyqtorch-0.4.1/tests/test_circ_matrices.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.0/tests/test_converters.py` & `pyqtorch-0.4.1/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.0/tests/test_module_hamevo.py` & `pyqtorch-0.4.1/tests/test_module_hamevo.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.0/tests/test_modules.py` & `pyqtorch-0.4.1/tests/test_modules.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import Callable
 
 import pytest
 import torch
 
 import pyqtorch.core as func_pyq
 import pyqtorch.modules as pyq
+from pyqtorch.core.utils import OPERATIONS_DICT
 from pyqtorch.modules.abstract import AbstractGate
 
 DEVICE = "cuda" if torch.cuda.is_available() else "cpu"
 DTYPE = torch.cdouble
 
 state_000 = pyq.zero_state(3, device=DEVICE, dtype=DTYPE)
 state_001 = pyq.X(qubits=[2], n_qubits=3)(state_000)
@@ -265,7 +266,32 @@
 @pytest.mark.parametrize("batch_size", [i for i in range(1, 8)])
 def test_overlap_states_batch_nqubits(state_fn: Callable, n_qubits: int, batch_size: int) -> None:
     state = state_fn(n_qubits, batch_size, device=DEVICE, dtype=DTYPE)
     assert torch.allclose(
         pyq.overlap(state, state),
         torch.ones(batch_size),
     )
+
+
+@pytest.mark.parametrize("state_fn", [pyq.random_state, pyq.zero_state, pyq.uniform_state])
+@pytest.mark.parametrize("batch_size", [i for i in range(1, 2, 10)])
+@pytest.mark.parametrize("n_qubits", [i for i in range(1, 6)])
+def test_parametrized_phase_gate(state_fn: Callable, batch_size: int, n_qubits: int) -> None:
+    qubits = [torch.randint(low=0, high=n_qubits, size=(1,)).item()]
+    state = state_fn(n_qubits, batch_size=batch_size, device=DEVICE, dtype=DTYPE)
+    phi = torch.tensor([torch.pi / 2], dtype=torch.cdouble)
+    phase = pyq.PHASE(qubits, n_qubits).to(device=DEVICE, dtype=DTYPE)
+    constant_phase = pyq.S(qubits, n_qubits).to(device=DEVICE, dtype=DTYPE)
+    assert torch.allclose(phase(state, phi), constant_phase(state, phi))
+
+
+@pytest.mark.parametrize("state_fn", [pyq.random_state, pyq.zero_state, pyq.uniform_state])
+def test_parametric_phase_hamevo(
+    state_fn: Callable, batch_size: int = 1, n_qubits: int = 1
+) -> None:
+    qubits = [0]
+    state = state_fn(n_qubits, batch_size=batch_size, device=DEVICE, dtype=DTYPE)
+    phi = torch.rand(1, dtype=torch.cdouble)
+    H = (OPERATIONS_DICT["Z"] - OPERATIONS_DICT["I"]) / 2
+    hamevo = pyq.HamEvoExp(H, phi, qubits=qubits, n_qubits=n_qubits)
+    phase = pyq.PHASE(qubits, n_qubits).to(device=DEVICE, dtype=DTYPE)
+    assert torch.allclose(phase(state, phi), hamevo(state))
```

### Comparing `pyqtorch-0.4.0/tests/test_notebooks.py` & `pyqtorch-0.4.1/tests/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.0/tests/test_operations.py` & `pyqtorch-0.4.1/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.0/tests/test_operations_hamevo.py` & `pyqtorch-0.4.1/tests/test_operations_hamevo.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.0/tests/test_sparse_modules.py` & `pyqtorch-0.4.1/tests/test_sparse_modules.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.0/.gitignore` & `pyqtorch-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.0/LICENSE` & `pyqtorch-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.4.0/pyproject.toml` & `pyqtorch-0.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     { name = "Aleksander Wennersteen", email = "aleksander.wennersteen@pasqal.com" },
     { name = "Mario Dagrada", email = "mario.dagrada@pasqal.com" },
     { name = "Dominik Seitz", email = "dominik.seitz@pasqal.com" },
     { name = "Niklas Heim", email = "niklas.heim@pasqal.com" },
 ]
 requires-python = ">=3.8,<3.12"
 license = {text = "Proprietary"}
-version = "0.4.0"
+version = "0.4.1"
 classifiers=[
     "License :: Other/Proprietary License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
```

### Comparing `pyqtorch-0.4.0/PKG-INFO` & `pyqtorch-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqtorch
-Version: 0.4.0
+Version: 0.4.1
 Summary: An efficient, large-scale emulator designed for quantum machine learning, seamlessly integrated with a PyTorch backend. Please refer to https://pyqtorch.readthedocs.io/en/latest/ for setup and usage info, along with the full documentation.
 Author-email: Slimane Thabet <slimane.thabet@pasqal.com>, Aleksander Wennersteen <aleksander.wennersteen@pasqal.com>, Mario Dagrada <mario.dagrada@pasqal.com>, Dominik Seitz <dominik.seitz@pasqal.com>, Niklas Heim <niklas.heim@pasqal.com>
 License: Proprietary
 License-File: LICENSE
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

