# Comparing `tmp/discotime-0.0.4.tar.gz` & `tmp/discotime-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discotime-0.0.4.tar", last modified: Thu Jul 20 11:11:23 2023, max compression
+gzip compressed data, was "discotime-0.1.0.tar", last modified: Tue Jul 25 09:08:31 2023, max compression
```

## Comparing `discotime-0.0.4.tar` & `discotime-0.1.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:11:23.944746 discotime-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-20 11:11:08.000000 discotime-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-20 11:11:08.000000 discotime-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-07-20 11:11:23.944746 discotime-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-20 11:11:08.000000 discotime-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-20 11:11:08.000000 discotime-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-07-20 11:11:23.944746 discotime-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:11:23.940746 discotime-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:11:23.940746 discotime-0.0.4/src/discotime/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-20 11:11:08.000000 discotime-0.0.4/src/discotime/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:11:23.944746 discotime-0.0.4/src/discotime/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-20 11:11:08.000000 discotime-0.0.4/src/discotime/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-07-20 11:11:08.000000 discotime-0.0.4/src/discotime/datasets/from_rstats.py
--rw-r--r--   0 runner    (1001) docker     (123)    11771 2023-07-20 11:11:08.000000 discotime-0.0.4/src/discotime/datasets/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:11:23.944746 discotime-0.0.4/src/discotime/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-20 11:11:08.000000 discotime-0.0.4/src/discotime/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-07-20 11:11:08.000000 discotime-0.0.4/src/discotime/metrics/brier_score.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:11:23.944746 discotime-0.0.4/src/discotime/models/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-20 11:11:08.000000 discotime-0.0.4/src/discotime/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-07-20 11:11:08.000000 discotime-0.0.4/src/discotime/models/components.py
--rw-r--r--   0 runner    (1001) docker     (123)    10737 2023-07-20 11:11:08.000000 discotime-0.0.4/src/discotime/models/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:11:23.944746 discotime-0.0.4/src/discotime/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-20 11:11:08.000000 discotime-0.0.4/src/discotime/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9317 2023-07-20 11:11:08.000000 discotime-0.0.4/src/discotime/utils/estimators.py
--rw-r--r--   0 runner    (1001) docker     (123)     6566 2023-07-20 11:11:08.000000 discotime-0.0.4/src/discotime/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-20 11:11:08.000000 discotime-0.0.4/src/discotime/utils/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:11:23.944746 discotime-0.0.4/src/discotime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-07-20 11:11:23.000000 discotime-0.0.4/src/discotime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-20 11:11:23.000000 discotime-0.0.4/src/discotime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 11:11:23.000000 discotime-0.0.4/src/discotime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-20 11:11:23.000000 discotime-0.0.4/src/discotime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-20 11:11:23.000000 discotime-0.0.4/src/discotime.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:11:23.944746 discotime-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-20 11:11:08.000000 discotime-0.0.4/tests/test_lightning_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     5706 2023-07-20 11:11:08.000000 discotime-0.0.4/tests/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-07-20 11:11:08.000000 discotime-0.0.4/tests/test_mgus2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-07-20 11:11:08.000000 discotime-0.0.4/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-20 11:11:08.000000 discotime-0.0.4/tests/test_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-07-20 11:11:08.000000 discotime-0.0.4/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:08:31.359848 discotime-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-25 09:08:22.000000 discotime-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-25 09:08:22.000000 discotime-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-07-25 09:08:31.359848 discotime-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-25 09:08:22.000000 discotime-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-25 09:08:22.000000 discotime-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-07-25 09:08:31.359848 discotime-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:08:31.355848 discotime-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:08:31.355848 discotime-0.1.0/src/discotime/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-25 09:08:22.000000 discotime-0.1.0/src/discotime/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:08:31.355848 discotime-0.1.0/src/discotime/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-25 09:08:22.000000 discotime-0.1.0/src/discotime/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-07-25 09:08:22.000000 discotime-0.1.0/src/discotime/datasets/from_rstats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11771 2023-07-25 09:08:22.000000 discotime-0.1.0/src/discotime/datasets/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:08:31.355848 discotime-0.1.0/src/discotime/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-25 09:08:22.000000 discotime-0.1.0/src/discotime/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6083 2023-07-25 09:08:22.000000 discotime-0.1.0/src/discotime/metrics/brier_score.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:08:31.355848 discotime-0.1.0/src/discotime/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-25 09:08:22.000000 discotime-0.1.0/src/discotime/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-07-25 09:08:22.000000 discotime-0.1.0/src/discotime/models/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10499 2023-07-25 09:08:22.000000 discotime-0.1.0/src/discotime/models/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:08:31.359848 discotime-0.1.0/src/discotime/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-25 09:08:22.000000 discotime-0.1.0/src/discotime/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9330 2023-07-25 09:08:22.000000 discotime-0.1.0/src/discotime/utils/estimators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6566 2023-07-25 09:08:22.000000 discotime-0.1.0/src/discotime/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-25 09:08:22.000000 discotime-0.1.0/src/discotime/utils/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:08:31.355848 discotime-0.1.0/src/discotime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-07-25 09:08:31.000000 discotime-0.1.0/src/discotime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-25 09:08:31.000000 discotime-0.1.0/src/discotime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 09:08:31.000000 discotime-0.1.0/src/discotime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-25 09:08:31.000000 discotime-0.1.0/src/discotime.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-25 09:08:31.000000 discotime-0.1.0/src/discotime.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:08:31.359848 discotime-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-25 09:08:22.000000 discotime-0.1.0/tests/test_lightning_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6680 2023-07-25 09:08:22.000000 discotime-0.1.0/tests/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-07-25 09:08:22.000000 discotime-0.1.0/tests/test_mgus2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-07-25 09:08:22.000000 discotime-0.1.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-25 09:08:22.000000 discotime-0.1.0/tests/test_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-07-25 09:08:22.000000 discotime-0.1.0/tests/test_utils.py
```

### Comparing `discotime-0.0.4/LICENSE` & `discotime-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `discotime-0.0.4/PKG-INFO` & `discotime-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discotime
-Version: 0.0.4
+Version: 0.1.0
 Summary: Discrete-time competing risk analysis with neural networks
 Home-page: https://github.com/peterchristofferholm/discotime
 Author: Peter Holm
 Author-email: "Peter Holm" <petchdk@gmail.com>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.10
```

### Comparing `discotime-0.0.4/README.md` & `discotime-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `discotime-0.0.4/setup.cfg` & `discotime-0.1.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = discotime
-version = 0.0.4
+version = 0.1.0
 url = https://github.com/peterchristofferholm/discotime
 author = Peter Holm
 author_email = "Peter Holm" <petchdk@gmail.com>
 description = Discrete-time competing risk analysis with neural networks
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
```

### Comparing `discotime-0.0.4/src/discotime/datasets/from_rstats.py` & `discotime-0.1.0/src/discotime/datasets/from_rstats.py`

 * *Files identical despite different names*

### Comparing `discotime-0.0.4/src/discotime/datasets/utils.py` & `discotime-0.1.0/src/discotime/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `discotime-0.0.4/src/discotime/metrics/brier_score.py` & `discotime-0.1.0/src/discotime/metrics/brier_score.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,15 +155,15 @@
         n_causes = phi_test.shape[-1]
         tau = self.eval_grid
 
         futime, status = survival_test
         futime = torch.as_tensor(futime).squeeze()
         status = torch.as_tensor(status).squeeze()
 
-        cic = 1 - AalenJohansen(futime, status, n_causes)(tau)
+        cic = AalenJohansen(futime, status, n_causes)(tau)
         phi_null = cic.unsqueeze(0).expand_as(phi_test)
 
         bs_test = self.brier_score(phi_test, tau, survival_test)
         bs_null = self.brier_score(phi_null, tau, survival_test)
 
         if self.integrate:
             bs_null = torch.trapezoid(bs_null, tau.view(-1, 1), dim=0)
```

### Comparing `discotime-0.0.4/src/discotime/models/components.py` & `discotime-0.1.0/src/discotime/models/components.py`

 * *Files identical despite different names*

### Comparing `discotime-0.0.4/src/discotime/models/models.py` & `discotime-0.1.0/src/discotime/models/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional, Any, Callable, Dict
+from typing import Optional, Any, Callable, Dict, Sequence
 from dataclasses import dataclass
 import warnings
 
 import torch
 from torch.nn import functional as F
 from torch import nn
 from lightning import pytorch as pl
@@ -21,58 +21,56 @@
     activation functions in the ``torch.nn`` module.
     """
 
     n_sequential_blocks: int = 2
     """Number of neural-network layer blocks.
 
     Each block is modelled after a ResNet skip-block and contains the following
-    key elements: 
-    
+    key elements:
+
     .. code-block ::
 
         Sequential(
             (0): LazyBatchNorm1d()
             (1): LazyLinear()
             (2): DropOut()
             (3): SiLU()
             (4): LazyLinear()
             (5): DropOut()
         )
 
     Per default the output of the model is ``self.act_fn(x + self.net(x))``
-    but the skip part can be removed by setting :attr:`use_skip_connections` to 
-    ``False``. :attr:`n_hidden_units` controls the size of the linear layers in 
-    each block. See :class:`.components.Block` for more details 
+    but the skip part can be removed by setting :attr:`use_skip_connections` to
+    ``False``. :attr:`n_hidden_units` controls the size of the linear layers in
+    each block. See :class:`.components.Block` for more details
     on the actual implementation.
     """
     n_hidden_units: int = 20
     """Number of neurons in each of the hidden layers.
-    
+
     For ease of of use, the size of each hidden layer have been constrained to
     to be the exact same size as all the others. Default is 20.
     """
     dropout_rate: Optional[float] = None
     """Should ``nn.Dropout()`` be used in each block, and if so what is the
     rate of dropout? If ``None`` then dropout is not used. Default is None.
     """
     batch_normalization: bool = True
     """Use batch normalization in each block? Default is True."""
     use_skip_connections: bool = False
     """Toggle the use of skip-connections in the model blocks."""
 
-    evaluation_grid_size: int = 50
-    """Either the length of (int) or the specific grid (seq of floats) at which
-    model metrics are calculated. If an integer `n` is passed, then `n` evenly
+    evaluation_grid_size: Optional[int] = 50
+    """An integer `n`, then `n` evenly
     distributed timepoint are chosen from the range of the data.
     """
-    evaluation_grid_cuts: Optional[int] = None
-    """Either the length of (int) or the specific grid (seq of floats) at which
-    model metrics are calculated. If an integer `n` is passed, then `n` evenly
-    distributed timepoint are chosen from the range of the data.
+    evaluation_grid_cuts: Optional[Sequence[float]] = None
+    """Specify the grid (seq of floats) at which model metrics are calculated.
     """
+
     n_time_bins: Optional[int] = None
     """Number of time bins in discretization grid.
 
     If ``None``, which is the default, then we try to get the information from
     the attached datamodule during setup.
     """
     n_risks: Optional[int] = None
@@ -246,15 +244,15 @@
         self._test_step_outputs.append(
             (self._predict_estimates(x, self.eval_grid), ct, ce)
         )
         return test_loss
 
     def on_test_epoch_end(self) -> None:
         estimates, ct, ce = map(
-            lambda x: torch.cat(x), zip(*self._test_step_outputs)
+            lambda x: torch.cat(x).cpu(), zip(*self._test_step_outputs)
         )
         self._test_step_outputs.clear()  # empty list
         for metric, metric_fn in self._metrics.items():
             values = metric_fn(estimates, (ct, ce))
             for cause, value in enumerate(values, start=1):
                 self.log(f"test_{metric}_cause{cause}", value)
```

### Comparing `discotime-0.0.4/src/discotime/utils/estimators.py` & `discotime-0.1.0/src/discotime/utils/estimators.py`

 * *Files 0% similar despite different names*

```diff
@@ -203,15 +203,15 @@
         sj = torch.cumprod((nj - mj) / nj, dim=0).roll(1)
         sj[0] = 1
 
         n_risks = n_causes if n_causes else torch.max(_event).item()
         assert isinstance(n_risks, int)  # type narrowing
 
         # cause-specific incidences
-        ci = torch.zeros((len(tj), n_risks)).to(tj)
+        ci = torch.zeros((len(tj), n_risks), dtype=torch.double)
         for e in range(1, n_risks + 1):
             te = _time[_event == e]
             mcj = torch.bincount(torch.searchsorted(tj, te), minlength=len(tj))
             ci[:, e - 1] = torch.cumsum(sj * (mcj / nj), dim=0)
 
         self._tj = tj
         self._sj = sj
```

### Comparing `discotime-0.0.4/src/discotime/utils/misc.py` & `discotime-0.1.0/src/discotime/utils/misc.py`

 * *Files identical despite different names*

### Comparing `discotime-0.0.4/src/discotime/utils/typing.py` & `discotime-0.1.0/src/discotime/utils/typing.py`

 * *Files identical despite different names*

### Comparing `discotime-0.0.4/src/discotime.egg-info/PKG-INFO` & `discotime-0.1.0/src/discotime.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discotime
-Version: 0.0.4
+Version: 0.1.0
 Summary: Discrete-time competing risk analysis with neural networks
 Home-page: https://github.com/peterchristofferholm/discotime
 Author: Peter Holm
 Author-email: "Peter Holm" <petchdk@gmail.com>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.10
```

### Comparing `discotime-0.0.4/src/discotime.egg-info/SOURCES.txt` & `discotime-0.1.0/src/discotime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `discotime-0.0.4/tests/test_lightning_module.py` & `discotime-0.1.0/tests/test_lightning_module.py`

 * *Files identical despite different names*

### Comparing `discotime-0.0.4/tests/test_metrics.py` & `discotime-0.1.0/tests/test_metrics.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from itertools import pairwise, count, islice
+
 import torch
 import pytest
 from hypothesis import given, example
 from hypothesis import strategies as st
 
 from discotime.metrics import BrierScore, BrierScoreScaled
 from discotime.utils import AalenJohansen, IPCW
@@ -170,7 +172,39 @@
     expected_ndim = 1 if integrate else 2
     assert bss.ndim == expected_ndim
 
     expected_shape = (2,) if integrate else (len(tau), 2)
     assert bss.shape == expected_shape
 
     assert torch.all(bss <= 1)
+
+
+def test_brier_score_scaled_2(default_mgus2_model):
+    model = default_mgus2_model
+    data = [*map(torch.as_tensor, model.datamodule.dset_fit[:])]
+
+    tau = torch.linspace(10, 365, 50)
+    bss = BrierScoreScaled((data[3], data[4]), tau, True)
+
+    def training_loop():
+        optim = model.configure_optimizers()
+
+        for i in count():
+            model.train()
+            for batch_idx, batch in enumerate(
+                model.datamodule.train_dataloader()
+            ):
+                optim.zero_grad()
+                loss = model.training_step(batch, batch_idx)
+                model.backward(loss)
+                optim.step()
+
+            model.eval()
+            est = model._predict_estimates(data[0], tau)
+
+            if i % 5 == 0:
+                yield bss(est, (data[3], data[4]))
+
+    assert all(
+        torch.all(a <= (b + 0.01))
+        for (a, b) in pairwise(islice(training_loop(), 20))
+    )
```

### Comparing `discotime-0.0.4/tests/test_mgus2.py` & `discotime-0.1.0/tests/test_mgus2.py`

 * *Files identical despite different names*

### Comparing `discotime-0.0.4/tests/test_models.py` & `discotime-0.1.0/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `discotime-0.0.4/tests/test_preprocessing.py` & `discotime-0.1.0/tests/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `discotime-0.0.4/tests/test_utils.py` & `discotime-0.1.0/tests/test_utils.py`

 * *Files identical despite different names*

