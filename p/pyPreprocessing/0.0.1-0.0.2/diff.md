# Comparing `tmp/pyPreprocessing-0.0.1.tar.gz` & `tmp/pyPreprocessing-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/almami/Alexander/Python_Skripte/00_packages/pyPreprocessing/dist/tmp31tfs18u/pyPreprocessing-0.0.1.tar", last modified: Wed Dec  1 18:42:13 2021, max compression
+gzip compressed data, was "pyPreprocessing-0.0.2.tar", last modified: Tue Jul 25 11:03:34 2023, max compression
```

## Comparing `pyPreprocessing-0.0.1.tar` & `pyPreprocessing-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,31 @@
-drwxrwxr-x   0 almami    (1000) almami    (1000)        0 2021-12-01 18:42:13.000000 pyPreprocessing-0.0.1/
--rw-rw-r--   0 almami    (1000) almami    (1000)     1074 2021-10-17 22:09:06.000000 pyPreprocessing-0.0.1/LICENSE
--rw-rw-r--   0 almami    (1000) almami    (1000)     1713 2021-12-01 18:42:13.000000 pyPreprocessing-0.0.1/PKG-INFO
--rw-rw-r--   0 almami    (1000) almami    (1000)     1099 2021-11-06 19:02:34.000000 pyPreprocessing-0.0.1/README.md
--rw-rw-r--   0 almami    (1000) almami    (1000)      702 2021-12-01 18:42:13.000000 pyPreprocessing-0.0.1/setup.cfg
--rw-rw-r--   0 almami    (1000) almami    (1000)      317 2021-10-18 17:44:12.000000 pyPreprocessing-0.0.1/setup.py
-drwxrwxr-x   0 almami    (1000) almami    (1000)        0 2021-12-01 18:42:13.000000 pyPreprocessing-0.0.1/src/
-drwxrwxr-x   0 almami    (1000) almami    (1000)        0 2021-12-01 18:42:13.000000 pyPreprocessing-0.0.1/src/pyPreprocessing/
--rw-rw-r--   0 almami    (1000) almami    (1000)       16 2021-10-18 17:44:12.000000 pyPreprocessing-0.0.1/src/pyPreprocessing/__init__.py
--rw-rw-r--   0 almami    (1000) almami    (1000)    19896 2021-10-18 22:14:45.000000 pyPreprocessing-0.0.1/src/pyPreprocessing/baseline_correction.py
--rw-rw-r--   0 almami    (1000) almami    (1000)    15563 2021-10-18 17:44:12.000000 pyPreprocessing-0.0.1/src/pyPreprocessing/smoothing.py
--rw-rw-r--   0 almami    (1000) almami    (1000)     3250 2021-10-18 17:44:12.000000 pyPreprocessing-0.0.1/src/pyPreprocessing/transform.py
-drwxrwxr-x   0 almami    (1000) almami    (1000)        0 2021-12-01 18:42:13.000000 pyPreprocessing-0.0.1/src/pyPreprocessing.egg-info/
--rw-rw-r--   0 almami    (1000) almami    (1000)     1713 2021-12-01 18:42:13.000000 pyPreprocessing-0.0.1/src/pyPreprocessing.egg-info/PKG-INFO
--rw-rw-r--   0 almami    (1000) almami    (1000)      391 2021-12-01 18:42:13.000000 pyPreprocessing-0.0.1/src/pyPreprocessing.egg-info/SOURCES.txt
--rw-rw-r--   0 almami    (1000) almami    (1000)       59 2021-12-01 18:42:13.000000 pyPreprocessing-0.0.1/src/pyPreprocessing.egg-info/dependency_links.txt
--rw-rw-r--   0 almami    (1000) almami    (1000)       48 2021-12-01 18:42:13.000000 pyPreprocessing-0.0.1/src/pyPreprocessing.egg-info/requires.txt
--rw-rw-r--   0 almami    (1000) almami    (1000)       16 2021-12-01 18:42:13.000000 pyPreprocessing-0.0.1/src/pyPreprocessing.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-25 11:03:34.348642 pyPreprocessing-0.0.2/
+drwxrwxrwx   0        0        0        0 2023-07-25 11:03:34.268642 pyPreprocessing-0.0.2/.github/
+drwxrwxrwx   0        0        0        0 2023-07-25 11:03:34.312642 pyPreprocessing-0.0.2/.github/workflows/
+-rw-rw-rw-   0        0        0     1238 2023-01-17 12:22:04.000000 pyPreprocessing-0.0.2/.github/workflows/main.yml
+-rw-rw-rw-   0        0        0       58 2023-01-17 12:22:04.000000 pyPreprocessing-0.0.2/.gitignore
+-rw-rw-rw-   0        0        0     1095 2023-01-17 12:22:04.000000 pyPreprocessing-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1709 2023-07-25 11:03:34.975911 pyPreprocessing-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1117 2023-01-17 12:22:04.000000 pyPreprocessing-0.0.2/README.md
+-rw-rw-rw-   0        0        0      179 2023-07-21 12:17:16.000000 pyPreprocessing-0.0.2/environment.yml
+drwxrwxrwx   0        0        0        0 2023-07-25 11:03:34.340642 pyPreprocessing-0.0.2/examples/
+-rw-rw-rw-   0        0        0     5776 2023-07-21 12:28:51.000000 pyPreprocessing-0.0.2/examples/baseline_correction_examples.py
+-rw-rw-rw-   0        0        0       85 2023-07-21 12:17:02.000000 pyPreprocessing-0.0.2/requirements.txt
+-rw-rw-rw-   0        0        0      731 2023-07-25 11:03:34.987467 pyPreprocessing-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      326 2023-07-25 10:56:41.000000 pyPreprocessing-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 11:03:34.380642 pyPreprocessing-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-25 11:03:34.380642 pyPreprocessing-0.0.2/src/pyPreprocessing/
+-rw-rw-rw-   0        0        0       17 2023-01-17 12:22:04.000000 pyPreprocessing-0.0.2/src/pyPreprocessing/__init__.py
+-rw-rw-rw-   0        0        0    20381 2023-01-17 12:22:04.000000 pyPreprocessing-0.0.2/src/pyPreprocessing/baseline_correction.py
+-rw-rw-rw-   0        0        0    16248 2023-01-17 12:22:04.000000 pyPreprocessing-0.0.2/src/pyPreprocessing/smoothing.py
+-rw-rw-rw-   0        0        0     5487 2023-07-21 12:15:14.000000 pyPreprocessing-0.0.2/src/pyPreprocessing/transform.py
+drwxrwxrwx   0        0        0        0 2023-07-25 11:03:34.388642 pyPreprocessing-0.0.2/src/pyPreprocessing.egg-info/
+-rw-rw-rw-   0        0        0     1709 2023-07-25 11:03:34.000000 pyPreprocessing-0.0.2/src/pyPreprocessing.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      603 2023-07-25 11:03:34.000000 pyPreprocessing-0.0.2/src/pyPreprocessing.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       59 2023-07-25 11:03:34.000000 pyPreprocessing-0.0.2/src/pyPreprocessing.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-07-25 11:03:34.000000 pyPreprocessing-0.0.2/src/pyPreprocessing.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-25 11:03:34.000000 pyPreprocessing-0.0.2/src/pyPreprocessing.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-25 11:03:34.392642 pyPreprocessing-0.0.2/tests/
+-rw-rw-rw-   0        0        0        2 2023-01-17 12:22:04.000000 pyPreprocessing-0.0.2/tests/__init__.py
+-rw-rw-rw-   0        0        0     4122 2023-01-17 12:22:04.000000 pyPreprocessing-0.0.2/tests/test_baseline_correction.py
+-rw-rw-rw-   0        0        0     4814 2023-01-17 12:22:04.000000 pyPreprocessing-0.0.2/tests/test_smoothing.py
+-rw-rw-rw-   0        0        0     1579 2023-01-17 12:22:04.000000 pyPreprocessing-0.0.2/tests/test_transform.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyPreprocessing-0.0.1/LICENSE` & `pyPreprocessing-0.0.2/LICENSE`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2021 Alexander Southan
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2021 Alexander Southan
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `pyPreprocessing-0.0.1/PKG-INFO` & `pyPreprocessing-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,32 @@
-Metadata-Version: 2.1
-Name: pyPreprocessing
-Version: 0.0.1
-Summary: package preprocessing of datasets, especially from spectroscopy
-Home-page: https://github.com/AlexanderSouthan/pyPreprocessing
-Author: Alexander Southan
-Author-email: alexander.southan@web.de
-License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/AlexanderSouthan/pyPreprocessing/issues
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
-[![build workflow](https://github.com/AlexanderSouthan/pyPreprocessing/actions/workflows/main.yml/badge.svg)](https://github.com/AlexanderSouthan/pyPreprocessing/actions/workflows/main.yml)
-[![codecov](https://codecov.io/gh/AlexanderSouthan/pyPreprocessing/branch/master/graph/badge.svg?token=7GN1K2MVJ3)](https://codecov.io/gh/AlexanderSouthan/pyPreprocessing)
-
-# pyPreprocessing
-## General information
-For preprocessing of datasets like Raman spectra, infrared spectra, UV/Vis
-spectra, but also HPLC data and many other types of data, currently via
-baseline correction, smoothing, filtering, transformation, normalization and
-derivative. It relies on numpy, pandas, scipy, tqdm and scikit-learn, but also
-on https://github.com/AlexanderSouthan/pyRegression for the introduction of
-equality constraints into the polynomial baseline estimation methods, and
-https://github.com/AlexanderSouthan/little_helpers.
-
-## Documentation
-Please visit:
-https://alexandersouthan.github.io/pyPreprocessing/
-
-
+Metadata-Version: 2.1
+Name: pyPreprocessing
+Version: 0.0.2
+Summary: package preprocessing of datasets, especially from spectroscopy
+Home-page: https://github.com/AlexanderSouthan/pyPreprocessing
+Author: Alexander Southan
+Author-email: alexander.southan@web.de
+Project-URL: Bug Tracker, https://github.com/AlexanderSouthan/pyPreprocessing/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
+[![build workflow](https://github.com/AlexanderSouthan/pyPreprocessing/actions/workflows/main.yml/badge.svg)](https://github.com/AlexanderSouthan/pyPreprocessing/actions/workflows/main.yml)
+[![codecov](https://codecov.io/gh/AlexanderSouthan/pyPreprocessing/branch/master/graph/badge.svg?token=7GN1K2MVJ3)](https://codecov.io/gh/AlexanderSouthan/pyPreprocessing)
+
+# pyPreprocessing
+## General information
+For preprocessing of datasets like Raman spectra, infrared spectra, UV/Vis
+spectra, but also HPLC data and many other types of data, currently via
+baseline correction, smoothing, filtering, transformation, normalization and
+derivative. It relies on numpy, pandas, scipy, tqdm and scikit-learn, but also
+on https://github.com/AlexanderSouthan/pyDataFitting for the introduction of
+equality constraints into the polynomial baseline estimation methods, and
+https://github.com/AlexanderSouthan/little_helpers.
+
+## Documentation
+Please visit:
+https://alexandersouthan.github.io/pyPreprocessing/
```

### Comparing `pyPreprocessing-0.0.1/README.md` & `pyPreprocessing-0.0.2/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
-[![build workflow](https://github.com/AlexanderSouthan/pyPreprocessing/actions/workflows/main.yml/badge.svg)](https://github.com/AlexanderSouthan/pyPreprocessing/actions/workflows/main.yml)
-[![codecov](https://codecov.io/gh/AlexanderSouthan/pyPreprocessing/branch/master/graph/badge.svg?token=7GN1K2MVJ3)](https://codecov.io/gh/AlexanderSouthan/pyPreprocessing)
-
-# pyPreprocessing
-## General information
-For preprocessing of datasets like Raman spectra, infrared spectra, UV/Vis
-spectra, but also HPLC data and many other types of data, currently via
-baseline correction, smoothing, filtering, transformation, normalization and
-derivative. It relies on numpy, pandas, scipy, tqdm and scikit-learn, but also
-on https://github.com/AlexanderSouthan/pyRegression for the introduction of
-equality constraints into the polynomial baseline estimation methods, and
-https://github.com/AlexanderSouthan/little_helpers.
-
-## Documentation
-Please visit:
-https://alexandersouthan.github.io/pyPreprocessing/
+[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
+[![build workflow](https://github.com/AlexanderSouthan/pyPreprocessing/actions/workflows/main.yml/badge.svg)](https://github.com/AlexanderSouthan/pyPreprocessing/actions/workflows/main.yml)
+[![codecov](https://codecov.io/gh/AlexanderSouthan/pyPreprocessing/branch/master/graph/badge.svg?token=7GN1K2MVJ3)](https://codecov.io/gh/AlexanderSouthan/pyPreprocessing)
+
+# pyPreprocessing
+## General information
+For preprocessing of datasets like Raman spectra, infrared spectra, UV/Vis
+spectra, but also HPLC data and many other types of data, currently via
+baseline correction, smoothing, filtering, transformation, normalization and
+derivative. It relies on numpy, pandas, scipy, tqdm and scikit-learn, but also
+on https://github.com/AlexanderSouthan/pyDataFitting for the introduction of
+equality constraints into the polynomial baseline estimation methods, and
+https://github.com/AlexanderSouthan/little_helpers.
+
+## Documentation
+Please visit:
+https://alexandersouthan.github.io/pyPreprocessing/
```

### Comparing `pyPreprocessing-0.0.1/src/pyPreprocessing/baseline_correction.py` & `pyPreprocessing-0.0.2/src/pyPreprocessing/baseline_correction.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,485 +1,485 @@
-﻿# -*- coding: utf-8 -*-
-"""
-Provides functions correct_baseline and generate_baseline which can be used for
-baseline preprocessing of spectral data. See function docstrings for more
-detail.
-"""
-
-import numpy as np
-from tqdm import tqdm
-from scipy.sparse import diags
-from scipy.sparse.linalg import spsolve
-from scipy.spatial import ConvexHull
-
-from pyDataFitting.polynomial_regression import (polynomial_fit,
-                                                 piecewise_polynomial_fit)
-from little_helpers.math_functions import piecewise_polynomial
-from .transform import transform as transform_spectra
-from .smoothing import smoothing as smooth_spectra
-from little_helpers.array_tools import y_at_x
-
-
-def correct_baseline(raw_data, mode, smoothing=True, transform=False,
-                     **kwargs):
-    """
-    Calculate baseline data for raw_data with generate_baseline(...).
-
-    Takes the same arguments like generate_baseline, for details see
-    docstring of generate_baseline.
-    """
-    return raw_data - generate_baseline(raw_data, mode, smoothing=smoothing,
-                                        transform=transform, **kwargs)
-
-
-def generate_baseline(raw_data, mode, smoothing=True, transform=False,
-                      **kwargs):
-    """
-    Calculate baseline data on input datasets with different algorithms.
-
-    Input data:
-    -----------
-    raw_data: ndarray
-        Numpy 2D array of shape (N, M) with N datasets and M data points per
-        dataset. If only one dataset is given, it has to have the shape (1, M).
-    mode: str
-        Algorithm for baseline calculation. Allowed values:
-        'convex_hull', 'ALSS', 'iALSS', 'drPLS', 'SNIP', 'ModPoly', 'IModPoly',
-        'PPF'.
-    smoothing: bool
-        True if datasets should be smoothed before calculation (recommended),
-        otherwise False.
-    transform: bool
-        True if datasets should be transformed before calculation,
-        otherwise False.
-
-    kwargs for smoothing == True
-    ---------------------------
-    savgol_window: int
-        window size for Savitzky-Golay window, default=19.
-    savgol_order: int
-        polynomial order for Savitzky-Golay filter, default=2.
-
-    kwargs for transform == True
-    ---------------------------
-    currently none, but will to be added in future versions.
-
-    kwargs for different baseline modes:
-    ------------------------------------
-    convex_hull:
-        wavenumbers: ndarray
-            Numpy array containing wavenumbers or wavelengths of datasets.
-            Must have M elements and must be sorted. default=np.arange(M)
-    ALSS:
-        lam: float
-            default=10000
-        p: float
-            default=0.001
-        n_iter: int
-            default=10
-        conv_crit: float
-            default=0.001
-    iALSS:
-        lam: float
-            default=2000
-        lam_1: float
-            default=0.01
-        p: float
-            default=0.01
-        n_iter: int
-            default=10
-        conv_crit: float
-            default=0.001
-        wavenumbers: ndarray
-            Numpy array containing wavenumbers or wavelengths of datasets.
-            Must have M elements. default=np.arange(M)
-    drPLS:
-        lam: float
-            default=1000000
-        eta: float
-            default=0.5
-        n_iter: int
-            default=100
-        conv_crit: float
-            default=0.001
-    SNIP:
-        n_iter: int
-            default=100
-    ModPoly, IModPoly:
-        wavenumbers: ndarray
-            Numpy array containing wavenumbers or wavelengths of datasets.
-            Must have M elements and must be sorted. default=np.arange(M)
-        n_iter: int
-            default=100
-        poly_order: int
-            default=5
-        fixed_points: list of tuples, optional
-            Contains constraints for points that the baseline must
-            pass through. Each point is given by a tuple of two numbers,
-            the wavenumber and the intensity of the point. If no point
-            constraints are to be applied, this must be None. The
-            default is None.
-        fixed_slopes: list of tuples, optional
-            Contains constraints for slopes that the fit functions must
-            have at specific wavenumbers. Each slope is given by a tuple of
-            two numbers, the wavenumber and the slope. If no slope
-            constraints are to be applied, this must be None. The
-            default is None.
-    PPF:
-        wavenumbers: ndarray, optional
-            Numpy array containing wavenumbers or wavelengths of datasets.
-            Must have M elements and must be sorted. default=np.arange(M).
-        n_iter: int, optional
-            default=100
-        segment_borders : list of int or float, optional
-            The values with respect to wavenumbers at which the data is divided
-            into segments. An arbitrary number of segment borders may be given,
-            but it is recommended to provide a sorted list in order to avoid
-            confusion. If the list is not sorted, it will be sorted. The
-            default is [wavenumbers[len(wavenumbers)//2]], resulting in a
-            segmentation in the middle of the data.
-        poly_orders : list of int, optional
-            A list containing the polynomial orders used for the baseline fit.
-            Must contain one more element than segment_borders. Default is
-            [3, 3].
-        fit_method: str, optional
-            Defines if the polynomial baseline fit of the segments is
-            performed by the ModPoly ('ModPoly') or IModPoly ('IModPoly')
-            algorithm. Default is 'ModPoly'.
-        y_at_borders : None, or list of float or None, or 'int_at_borders', 
-        optional
-            May contain dependent variable values used as equality constraints
-            at the segment borders. The fits of both touching segments are
-            forced through the point given by the pair (segment border,
-            y_at_border). The list entries may also be None to state that at a
-            certain segment border, no constraint is to be applied. The default
-            is 'int_at_borders' which is the intensity value at the
-            segment_borders.
-    """
-    # Optionally, spectrum data is smoothed before beaseline calculation. This
-    # makes sense especially for baseline generation methods that have problems
-    # with noise. Currently Savitzky-Golay only.
-    if smoothing:
-        savgol_window = kwargs.get('savgol_window', 9)
-        savgol_order = kwargs.get('savol_order', 2)
-        raw_data = smooth_spectra(raw_data, 'sav_gol',
-                                  savgol_points=savgol_window,
-                                  poly_order=savgol_order)
-
-    # Transformation makes sense for spectra that cover a broad range of peak
-    # intensities. Otherwise, small peaks may be more or less ignored during
-    # baseline calculation. Currently LLS transformation only.
-    if transform:
-        spectra_minimum_value = raw_data.min()
-        raw_data = transform_spectra(raw_data, 'log_log_sqrt')
-
-    # wavenumbers are used for convex_hull, ModPoly, IModPoly, PPF, iALSS
-    if 'wavenumbers' in kwargs:
-        wavenumbers = kwargs.get('wavenumbers')
-        ascending_wn = (wavenumbers[1]-wavenumbers[0]) > 0
-    else:
-        wavenumbers = np.arange(raw_data.shape[1])
-        ascending_wn = True
-
-    baseline_data = np.zeros_like(raw_data)
-    baseline_modes = ['convex_hull', 'ALSS', 'iALSS', 'drPLS', 'SNIP',
-                      'ModPoly', 'IModPoly', 'PPF']
-
-    if mode == baseline_modes[0]:  # convex_hull
-        # based on (but improved a bit)
-        # https://dsp.stackexchange.com/questions/2725/
-        # how-to-perform-a-rubberband-correction-on-spectroscopic-data
-
-        if ascending_wn:
-            raw_data = np.flip(raw_data, axis=1)
-            wavenumbers = np.flip(wavenumbers)
-
-        for ii, current_spectrum in enumerate(tqdm(raw_data)):
-            hull_vertices = ConvexHull(
-                np.array(list(zip(wavenumbers, current_spectrum)))).vertices
-
-            # Rotate convex hull vertices until they start from the lowest one
-            hull_vertices = np.roll(hull_vertices, -np.argmin(hull_vertices))
-
-            # split vertices into upper and lower part
-            hull_vertices_section_1 = hull_vertices[:np.argmax(hull_vertices)
-                                                    + 1]
-            hull_vertices_section_2 = np.sort(
-                np.insert(hull_vertices[np.argmax(hull_vertices):], 0,
-                          hull_vertices[0]))
-
-            # calculate spectrum mean intensities of upper and lower vertices
-            raw_mean_1 = np.mean(current_spectrum[hull_vertices_section_1])
-            raw_mean_2 = np.mean(current_spectrum[hull_vertices_section_2])
-
-            # Select lower vertices as baseline vertices
-            if raw_mean_1 > raw_mean_2:
-                baseline_vertices = hull_vertices_section_2
-            else:
-                baseline_vertices = hull_vertices_section_1
-
-            # Create baseline using linear interpolation between vertices
-            baseline_data[ii, :] = np.interp(
-                wavenumbers, np.flip(wavenumbers[baseline_vertices]),
-                np.flip(current_spectrum[baseline_vertices]))
-
-        if ascending_wn:
-            baseline_data = np.flip(baseline_data, axis=1)
-
-    elif mode == baseline_modes[1]:  # ALSS
-        # according to
-        # "Baseline Correction with Asymmetric Least Squares Smoothing"
-        # by P. Eilers and H. Boelens.
-        # https://zanran_storage.s3.amazonaws.com/www.science.uva.nl/
-        # ContentPages/443199618.pdf
-
-        # set mode specific parameters
-        lam = kwargs.get('lam', 10000)
-        p = kwargs.get('p', 0.001)
-        n_iter = kwargs.get('n_iter', 10)
-        conv_crit = kwargs.get('conv_crit', 0.001)
-        #############################
-
-        L = raw_data.shape[1]
-        D = diags([1, -2, 1], [0, -1, -2], shape=(L, L-2), format='csr')
-        D = D.dot(D.transpose())
-
-        for ii, current_spectrum in enumerate(tqdm(raw_data)):
-
-            # this is the code for the fitting procedure
-            w = np.ones(L)
-            W = diags(w, format='csr')
-            z = w
-
-            for jj in range(int(n_iter)):
-                W.setdiag(w)
-                Z = W + lam * D
-                z_prev = z
-                z = spsolve(Z, w*current_spectrum, permc_spec='NATURAL')
-                if np.linalg.norm(z - z_prev) > conv_crit:
-                    w = p * (current_spectrum > z) + (1-p) * (
-                        current_spectrum < z)
-                else:
-                    break
-            # end of fitting procedure
-
-            baseline_data[ii, :] = z
-
-    elif mode == baseline_modes[2]:  # iALSS
-        # according to "Anal. Methods, 2014, 6, 4402–4407."
-
-        # set mode specific parameters
-        lam = kwargs.get('lam', 2000)
-        lam_1 = kwargs.get('lam_1', 0.01)
-        p = kwargs.get('p', 0.01)
-        n_iter = kwargs.get('n_iter', 10)
-        conv_crit = kwargs.get('conv_crit', 0.001)
-        #############################
-
-        L = raw_data.shape[1]
-        fit_coeffs = np.polynomial.polynomial.polyfit(wavenumbers,
-                                                      raw_data.T, 2)
-        w_start_all = np.polynomial.polynomial.polyval(wavenumbers, fit_coeffs)
-
-        D = diags([1, -2, 1], [0, -1, -2], shape=(L, L-2), format='csr')
-        D = D.dot(D.transpose())
-        D_1 = diags([-1, 1], [0, -1], shape=(L, L-1), format='csr')
-        D_1 = D_1.dot(D_1.transpose())
-
-        for ii, current_spectrum in enumerate(tqdm(raw_data)):
-
-            # this is the code for the fitting procedure
-            w = w_start_all[ii, :]
-            z = w
-            W = diags(w, format='csr')
-            w = p * (current_spectrum > z) + (1-p) * (current_spectrum < z)
-
-            for jj in range(int(n_iter)):
-                W.setdiag(w)
-                W = W.dot(W.transpose())
-                Z = W + lam_1 * D_1 + lam * D
-                R = (W + lam_1 * D_1) * current_spectrum
-                z_prev = z
-                z = spsolve(Z, R, permc_spec='NATURAL')
-                if np.linalg.norm(z - z_prev) > conv_crit:
-                    w = p * (current_spectrum > z) + (1-p) * (
-                        current_spectrum < z)
-                else:
-                    break
-            # end of fitting procedure
-
-            baseline_data[ii, :] = z
-
-    elif mode == baseline_modes[3]:  # drPLS
-        # according to "Applied Optics, 2019, 58, 3913-3920."
-
-        # set mode specific parameters
-        lam = kwargs.get('lam', 1000000)
-        eta = kwargs.get('eta', 0.5)
-        n_iter = kwargs.get('n_iter', 100)
-        conv_crit = kwargs.get('conv_crit', 0.001)
-        #############################
-
-        L = raw_data.shape[1]
-
-        D = diags([1, -2, 1], [0, -1, -2], shape=(L, L-2), format='csr')
-        D = D.dot(D.transpose())
-        D_1 = diags([-1, 1], [0, -1], shape=(L, L-1), format='csr')
-        D_1 = D_1.dot(D_1.transpose())
-
-        w_0 = np.ones(L)
-        I_n = diags(w_0, format='csr')
-
-        for ii, current_spectrum in enumerate(tqdm(raw_data)):
-
-            # this is the code for the fitting procedure
-            w = w_0
-            W = diags(w, format='csr')
-            Z = w_0
-
-            for jj in range(int(n_iter)):
-                W.setdiag(w)
-                Z_prev = Z
-                Z = spsolve(W + D_1 + lam * (I_n - eta*W) *
-                            D, W*current_spectrum, permc_spec='NATURAL')
-                if np.linalg.norm(Z - Z_prev) > conv_crit:
-                    d = current_spectrum - Z
-                    d_negative = d[d < 0]
-                    sigma_negative = np.std(d_negative)
-                    mean_negative = np.mean(d_negative)
-                    w = 0.5 * (1 - np.exp(jj) * (d - (
-                        -mean_negative + 2*sigma_negative))/sigma_negative / (
-                            1 + np.abs(np.exp(jj) * (d - (
-                                - mean_negative + 2 * sigma_negative)) /
-                                sigma_negative)))
-                else:
-                    break
-            # end of fitting procedure
-
-            baseline_data[ii, :] = Z
-
-    elif mode == baseline_modes[4]:  # SNIP
-        # according to "Nuclear Instruments and Methods in Physics Research
-        # 934 (1988) 396-402."
-        # and Nuclear Instruments and Methods in Physics Research Section A:
-        # Accelerators, Spectrometers, Detectors and Associated Equipment 1997,
-        # 401 (1), 113-132
-
-        # set mode specific parameters
-        n_iter = kwargs.get('n_iter', 100)
-        #############################
-
-        spectrum_points = raw_data.shape[1]
-        working_spectra = np.zeros_like(raw_data)
-
-        for pp in tqdm(np.arange(1, n_iter+1)):
-            r1 = raw_data[:, pp:spectrum_points-pp]
-            r2 = (np.roll(raw_data, -pp, axis=1)[:, pp:spectrum_points-pp] +
-                  np.roll(raw_data, pp, axis=1)[:, pp:spectrum_points-pp])/2
-            working_spectra = np.minimum(r1, r2)
-            raw_data[:, pp:spectrum_points-pp] = working_spectra
-
-        baseline_data = raw_data
-
-    elif mode in baseline_modes[5:8]:  # ModPoly, IModPoly, PPF
-        # according to Applied Spectroscopy, 2007, 61 (11), 1225-1232.
-        # without dev: Chemometrics and Intelligent Laboratory Systems 82
-        #              (2006) 59– 65.
-        #              Maybe also ModPoly from first source?
-
-        # set mode specific parameters
-        n_iter = kwargs.get('n_iter', 100)
-        if mode in baseline_modes[5:7]:  # ModPoly, IModPoly
-            poly_order = kwargs.get('poly_order', 5)
-            fixed_points = kwargs.get('fixed_points', None)
-            fixed_slopes = kwargs.get('fixed_slopes', None)
-        if mode == baseline_modes[7]:  # PPF
-            segment_borders = kwargs.get(
-                'segment_borders', [wavenumbers[len(wavenumbers)//2]])
-
-            poly_orders = kwargs.get('poly_orders', [3, 3])
-            y_at_borders = kwargs.get('y_at_borders', 'int_at_borders')
-            fit_method = kwargs.get('fit_method', 'ModPoly')
-        #############################
-
-        if not ascending_wn:
-            raw_data = np.flip(raw_data, axis=1)
-            wavenumbers = np.flip(wavenumbers)
-
-        wavenumbers_start = wavenumbers
-        # previous_dev = 0
-
-        for ii, current_spectrum in enumerate(tqdm(raw_data)):
-            wavenumbers = wavenumbers_start
-
-            if mode == baseline_modes[7]:  # 'PPF'
-                if y_at_borders == 'int_at_borders':
-                    y_at_borders_values = y_at_x(
-                        segment_borders, wavenumbers, current_spectrum)
-                else:
-                    y_at_borders_values = y_at_borders
-
-            for jj in range(int(n_iter)):
-                if mode in baseline_modes[5:7]:  # ModPoly, IModPoly
-                    # The polynomial_fit method from pyRegression is only used
-                    # if constraints are to be considered because the numpy
-                    # polyfit method is faster.
-                    if (fixed_points is not None) or (
-                            fixed_slopes is not None):
-                        fit_data, fit_coeffs = polynomial_fit(
-                            wavenumbers, current_spectrum, poly_order,
-                            fixed_points=fixed_points,
-                            fixed_slopes=fixed_slopes)
-                    else:
-                        fit_coeffs = np.polynomial.polynomial.polyfit(
-                            wavenumbers, current_spectrum, poly_order)
-                        fit_data = np.polynomial.polynomial.polyval(
-                            wavenumbers, fit_coeffs)
-                else:  # PPF
-                    fit_data, fit_coeffs = piecewise_polynomial_fit(
-                        wavenumbers, current_spectrum, segment_borders,
-                        poly_orders, y_at_borders=y_at_borders_values,
-                        slope_at_borders=None)
-
-                # ModPoly or PPF with ModPoly
-                if (mode == baseline_modes[5]) or (
-                        (mode == baseline_modes[7]) and (fit_method=='ModPoly')
-                        ):
-                    dev = 0
-                # IModPoly or PPF with IModPoly
-                else:
-                    residual = current_spectrum - fit_data
-                    dev = residual.std()
-                    # if abs((dev - previous_dev)/dev) < 0.01:
-                    #    break
-
-                if jj == 0:
-                    mask = (current_spectrum <= fit_data + dev)
-                    wavenumbers = wavenumbers[mask]
-                    current_spectrum = current_spectrum[mask]
-                    fit_data = fit_data[mask]
-                np.copyto(current_spectrum, fit_data + dev,
-                          where=(current_spectrum >= (fit_data+dev)))
-                # previous_dev = dev
-
-            if mode in baseline_modes[5:7]:  # ModPoly, IModPoly
-                baseline_data[ii, :] = np.polynomial.polynomial.polyval(
-                    wavenumbers_start, fit_coeffs)
-            else:  # PPF
-                baseline_data[ii, :] = piecewise_polynomial(
-                    wavenumbers_start, fit_coeffs,
-                    segment_borders=segment_borders)
-
-        if not ascending_wn:
-            baseline_data = np.flip(baseline_data, axis=1)
-            # raw_data = np.flip(raw_data, axis=1)
-
-    else:
-        raise ValueError('No valid baseline mode entered. Allowed modes are '
-                         '{0}'.format(baseline_modes))
-
-    if transform:
-        baseline_data = transform_spectra(
-            baseline_data, 'log_log_sqrt', direction='inverse',
-            min_value=spectra_minimum_value)
-
-    return np.around(baseline_data, decimals=6)
+﻿# -*- coding: utf-8 -*-
+"""
+Provides functions correct_baseline and generate_baseline which can be used for
+baseline preprocessing of spectral data. See function docstrings for more
+detail.
+"""
+
+import numpy as np
+from tqdm import tqdm
+from scipy.sparse import diags
+from scipy.sparse.linalg import spsolve
+from scipy.spatial import ConvexHull
+
+from pyDataFitting.polynomial_regression import (polynomial_fit,
+                                                 piecewise_polynomial_fit)
+from little_helpers.math_functions import piecewise_polynomial
+from .transform import transform as transform_spectra
+from .smoothing import smoothing as smooth_spectra
+from little_helpers.array_tools import y_at_x
+
+
+def correct_baseline(raw_data, mode, smoothing=True, transform=False,
+                     **kwargs):
+    """
+    Calculate baseline data for raw_data with generate_baseline(...).
+
+    Takes the same arguments like generate_baseline, for details see
+    docstring of generate_baseline.
+    """
+    return raw_data - generate_baseline(raw_data, mode, smoothing=smoothing,
+                                        transform=transform, **kwargs)
+
+
+def generate_baseline(raw_data, mode, smoothing=True, transform=False,
+                      **kwargs):
+    """
+    Calculate baseline data on input datasets with different algorithms.
+
+    Input data:
+    -----------
+    raw_data: ndarray
+        Numpy 2D array of shape (N, M) with N datasets and M data points per
+        dataset. If only one dataset is given, it has to have the shape (1, M).
+    mode: str
+        Algorithm for baseline calculation. Allowed values:
+        'convex_hull', 'ALSS', 'iALSS', 'drPLS', 'SNIP', 'ModPoly', 'IModPoly',
+        'PPF'.
+    smoothing: bool
+        True if datasets should be smoothed before calculation (recommended),
+        otherwise False.
+    transform: bool
+        True if datasets should be transformed before calculation,
+        otherwise False.
+
+    kwargs for smoothing == True
+    ---------------------------
+    savgol_window: int
+        window size for Savitzky-Golay window, default=19.
+    savgol_order: int
+        polynomial order for Savitzky-Golay filter, default=2.
+
+    kwargs for transform == True
+    ---------------------------
+    currently none, but will to be added in future versions.
+
+    kwargs for different baseline modes:
+    ------------------------------------
+    convex_hull:
+        wavenumbers: ndarray
+            Numpy array containing wavenumbers or wavelengths of datasets.
+            Must have M elements and must be sorted. default=np.arange(M)
+    ALSS:
+        lam: float
+            default=10000
+        p: float
+            default=0.001
+        n_iter: int
+            default=10
+        conv_crit: float
+            default=0.001
+    iALSS:
+        lam: float
+            default=2000
+        lam_1: float
+            default=0.01
+        p: float
+            default=0.01
+        n_iter: int
+            default=10
+        conv_crit: float
+            default=0.001
+        wavenumbers: ndarray
+            Numpy array containing wavenumbers or wavelengths of datasets.
+            Must have M elements. default=np.arange(M)
+    drPLS:
+        lam: float
+            default=1000000
+        eta: float
+            default=0.5
+        n_iter: int
+            default=100
+        conv_crit: float
+            default=0.001
+    SNIP:
+        n_iter: int
+            default=100
+    ModPoly, IModPoly:
+        wavenumbers: ndarray
+            Numpy array containing wavenumbers or wavelengths of datasets.
+            Must have M elements and must be sorted. default=np.arange(M)
+        n_iter: int
+            default=100
+        poly_order: int
+            default=5
+        fixed_points: list of tuples, optional
+            Contains constraints for points that the baseline must
+            pass through. Each point is given by a tuple of two numbers,
+            the wavenumber and the intensity of the point. If no point
+            constraints are to be applied, this must be None. The
+            default is None.
+        fixed_slopes: list of tuples, optional
+            Contains constraints for slopes that the fit functions must
+            have at specific wavenumbers. Each slope is given by a tuple of
+            two numbers, the wavenumber and the slope. If no slope
+            constraints are to be applied, this must be None. The
+            default is None.
+    PPF:
+        wavenumbers: ndarray, optional
+            Numpy array containing wavenumbers or wavelengths of datasets.
+            Must have M elements and must be sorted. default=np.arange(M).
+        n_iter: int, optional
+            default=100
+        segment_borders : list of int or float, optional
+            The values with respect to wavenumbers at which the data is divided
+            into segments. An arbitrary number of segment borders may be given,
+            but it is recommended to provide a sorted list in order to avoid
+            confusion. If the list is not sorted, it will be sorted. The
+            default is [wavenumbers[len(wavenumbers)//2]], resulting in a
+            segmentation in the middle of the data.
+        poly_orders : list of int, optional
+            A list containing the polynomial orders used for the baseline fit.
+            Must contain one more element than segment_borders. Default is
+            [3, 3].
+        fit_method: str, optional
+            Defines if the polynomial baseline fit of the segments is
+            performed by the ModPoly ('ModPoly') or IModPoly ('IModPoly')
+            algorithm. Default is 'ModPoly'.
+        y_at_borders : None, or list of float or None, or 'int_at_borders', 
+        optional
+            May contain dependent variable values used as equality constraints
+            at the segment borders. The fits of both touching segments are
+            forced through the point given by the pair (segment border,
+            y_at_border). The list entries may also be None to state that at a
+            certain segment border, no constraint is to be applied. The default
+            is 'int_at_borders' which is the intensity value at the
+            segment_borders.
+    """
+    # Optionally, spectrum data is smoothed before beaseline calculation. This
+    # makes sense especially for baseline generation methods that have problems
+    # with noise. Currently Savitzky-Golay only.
+    if smoothing:
+        savgol_window = kwargs.get('savgol_window', 9)
+        savgol_order = kwargs.get('savol_order', 2)
+        raw_data = smooth_spectra(raw_data, 'sav_gol',
+                                  savgol_points=savgol_window,
+                                  poly_order=savgol_order)
+
+    # Transformation makes sense for spectra that cover a broad range of peak
+    # intensities. Otherwise, small peaks may be more or less ignored during
+    # baseline calculation. Currently LLS transformation only.
+    if transform:
+        spectra_minimum_value = raw_data.min()
+        raw_data = transform_spectra(raw_data, 'log_log_sqrt')
+
+    # wavenumbers are used for convex_hull, ModPoly, IModPoly, PPF, iALSS
+    if 'wavenumbers' in kwargs:
+        wavenumbers = kwargs.get('wavenumbers')
+        ascending_wn = (wavenumbers[1]-wavenumbers[0]) > 0
+    else:
+        wavenumbers = np.arange(raw_data.shape[1])
+        ascending_wn = True
+
+    baseline_data = np.zeros_like(raw_data)
+    baseline_modes = ['convex_hull', 'ALSS', 'iALSS', 'drPLS', 'SNIP',
+                      'ModPoly', 'IModPoly', 'PPF']
+
+    if mode == baseline_modes[0]:  # convex_hull
+        # based on (but improved a bit)
+        # https://dsp.stackexchange.com/questions/2725/
+        # how-to-perform-a-rubberband-correction-on-spectroscopic-data
+
+        if ascending_wn:
+            raw_data = np.flip(raw_data, axis=1)
+            wavenumbers = np.flip(wavenumbers)
+
+        for ii, current_spectrum in enumerate(tqdm(raw_data)):
+            hull_vertices = ConvexHull(
+                np.array(list(zip(wavenumbers, current_spectrum)))).vertices
+
+            # Rotate convex hull vertices until they start from the lowest one
+            hull_vertices = np.roll(hull_vertices, -np.argmin(hull_vertices))
+
+            # split vertices into upper and lower part
+            hull_vertices_section_1 = hull_vertices[:np.argmax(hull_vertices)
+                                                    + 1]
+            hull_vertices_section_2 = np.sort(
+                np.insert(hull_vertices[np.argmax(hull_vertices):], 0,
+                          hull_vertices[0]))
+
+            # calculate spectrum mean intensities of upper and lower vertices
+            raw_mean_1 = np.mean(current_spectrum[hull_vertices_section_1])
+            raw_mean_2 = np.mean(current_spectrum[hull_vertices_section_2])
+
+            # Select lower vertices as baseline vertices
+            if raw_mean_1 > raw_mean_2:
+                baseline_vertices = hull_vertices_section_2
+            else:
+                baseline_vertices = hull_vertices_section_1
+
+            # Create baseline using linear interpolation between vertices
+            baseline_data[ii, :] = np.interp(
+                wavenumbers, np.flip(wavenumbers[baseline_vertices]),
+                np.flip(current_spectrum[baseline_vertices]))
+
+        if ascending_wn:
+            baseline_data = np.flip(baseline_data, axis=1)
+
+    elif mode == baseline_modes[1]:  # ALSS
+        # according to
+        # "Baseline Correction with Asymmetric Least Squares Smoothing"
+        # by P. Eilers and H. Boelens.
+        # https://zanran_storage.s3.amazonaws.com/www.science.uva.nl/
+        # ContentPages/443199618.pdf
+
+        # set mode specific parameters
+        lam = kwargs.get('lam', 10000)
+        p = kwargs.get('p', 0.001)
+        n_iter = kwargs.get('n_iter', 10)
+        conv_crit = kwargs.get('conv_crit', 0.001)
+        #############################
+
+        L = raw_data.shape[1]
+        D = diags([1, -2, 1], [0, -1, -2], shape=(L, L-2), format='csr')
+        D = D.dot(D.transpose())
+
+        for ii, current_spectrum in enumerate(tqdm(raw_data)):
+
+            # this is the code for the fitting procedure
+            w = np.ones(L)
+            W = diags(w, format='csr')
+            z = w
+
+            for jj in range(int(n_iter)):
+                W.setdiag(w)
+                Z = W + lam * D
+                z_prev = z
+                z = spsolve(Z, w*current_spectrum, permc_spec='NATURAL')
+                if np.linalg.norm(z - z_prev) > conv_crit:
+                    w = p * (current_spectrum > z) + (1-p) * (
+                        current_spectrum < z)
+                else:
+                    break
+            # end of fitting procedure
+
+            baseline_data[ii, :] = z
+
+    elif mode == baseline_modes[2]:  # iALSS
+        # according to "Anal. Methods, 2014, 6, 4402–4407."
+
+        # set mode specific parameters
+        lam = kwargs.get('lam', 2000)
+        lam_1 = kwargs.get('lam_1', 0.01)
+        p = kwargs.get('p', 0.01)
+        n_iter = kwargs.get('n_iter', 10)
+        conv_crit = kwargs.get('conv_crit', 0.001)
+        #############################
+
+        L = raw_data.shape[1]
+        fit_coeffs = np.polynomial.polynomial.polyfit(wavenumbers,
+                                                      raw_data.T, 2)
+        w_start_all = np.polynomial.polynomial.polyval(wavenumbers, fit_coeffs)
+
+        D = diags([1, -2, 1], [0, -1, -2], shape=(L, L-2), format='csr')
+        D = D.dot(D.transpose())
+        D_1 = diags([-1, 1], [0, -1], shape=(L, L-1), format='csr')
+        D_1 = D_1.dot(D_1.transpose())
+
+        for ii, current_spectrum in enumerate(tqdm(raw_data)):
+
+            # this is the code for the fitting procedure
+            w = w_start_all[ii, :]
+            z = w
+            W = diags(w, format='csr')
+            w = p * (current_spectrum > z) + (1-p) * (current_spectrum < z)
+
+            for jj in range(int(n_iter)):
+                W.setdiag(w)
+                W = W.dot(W.transpose())
+                Z = W + lam_1 * D_1 + lam * D
+                R = (W + lam_1 * D_1) * current_spectrum
+                z_prev = z
+                z = spsolve(Z, R, permc_spec='NATURAL')
+                if np.linalg.norm(z - z_prev) > conv_crit:
+                    w = p * (current_spectrum > z) + (1-p) * (
+                        current_spectrum < z)
+                else:
+                    break
+            # end of fitting procedure
+
+            baseline_data[ii, :] = z
+
+    elif mode == baseline_modes[3]:  # drPLS
+        # according to "Applied Optics, 2019, 58, 3913-3920."
+
+        # set mode specific parameters
+        lam = kwargs.get('lam', 1000000)
+        eta = kwargs.get('eta', 0.5)
+        n_iter = kwargs.get('n_iter', 100)
+        conv_crit = kwargs.get('conv_crit', 0.001)
+        #############################
+
+        L = raw_data.shape[1]
+
+        D = diags([1, -2, 1], [0, -1, -2], shape=(L, L-2), format='csr')
+        D = D.dot(D.transpose())
+        D_1 = diags([-1, 1], [0, -1], shape=(L, L-1), format='csr')
+        D_1 = D_1.dot(D_1.transpose())
+
+        w_0 = np.ones(L)
+        I_n = diags(w_0, format='csr')
+
+        for ii, current_spectrum in enumerate(tqdm(raw_data)):
+
+            # this is the code for the fitting procedure
+            w = w_0
+            W = diags(w, format='csr')
+            Z = w_0
+
+            for jj in range(int(n_iter)):
+                W.setdiag(w)
+                Z_prev = Z
+                Z = spsolve(W + D_1 + lam * (I_n - eta*W) *
+                            D, W*current_spectrum, permc_spec='NATURAL')
+                if np.linalg.norm(Z - Z_prev) > conv_crit:
+                    d = current_spectrum - Z
+                    d_negative = d[d < 0]
+                    sigma_negative = np.std(d_negative)
+                    mean_negative = np.mean(d_negative)
+                    w = 0.5 * (1 - np.exp(jj) * (d - (
+                        -mean_negative + 2*sigma_negative))/sigma_negative / (
+                            1 + np.abs(np.exp(jj) * (d - (
+                                - mean_negative + 2 * sigma_negative)) /
+                                sigma_negative)))
+                else:
+                    break
+            # end of fitting procedure
+
+            baseline_data[ii, :] = Z
+
+    elif mode == baseline_modes[4]:  # SNIP
+        # according to "Nuclear Instruments and Methods in Physics Research
+        # 934 (1988) 396-402."
+        # and Nuclear Instruments and Methods in Physics Research Section A:
+        # Accelerators, Spectrometers, Detectors and Associated Equipment 1997,
+        # 401 (1), 113-132
+
+        # set mode specific parameters
+        n_iter = kwargs.get('n_iter', 100)
+        #############################
+
+        spectrum_points = raw_data.shape[1]
+        working_spectra = np.zeros_like(raw_data)
+
+        for pp in tqdm(np.arange(1, n_iter+1)):
+            r1 = raw_data[:, pp:spectrum_points-pp]
+            r2 = (np.roll(raw_data, -pp, axis=1)[:, pp:spectrum_points-pp] +
+                  np.roll(raw_data, pp, axis=1)[:, pp:spectrum_points-pp])/2
+            working_spectra = np.minimum(r1, r2)
+            raw_data[:, pp:spectrum_points-pp] = working_spectra
+
+        baseline_data = raw_data
+
+    elif mode in baseline_modes[5:8]:  # ModPoly, IModPoly, PPF
+        # according to Applied Spectroscopy, 2007, 61 (11), 1225-1232.
+        # without dev: Chemometrics and Intelligent Laboratory Systems 82
+        #              (2006) 59– 65.
+        #              Maybe also ModPoly from first source?
+
+        # set mode specific parameters
+        n_iter = kwargs.get('n_iter', 100)
+        if mode in baseline_modes[5:7]:  # ModPoly, IModPoly
+            poly_order = kwargs.get('poly_order', 5)
+            fixed_points = kwargs.get('fixed_points', None)
+            fixed_slopes = kwargs.get('fixed_slopes', None)
+        if mode == baseline_modes[7]:  # PPF
+            segment_borders = kwargs.get(
+                'segment_borders', [wavenumbers[len(wavenumbers)//2]])
+
+            poly_orders = kwargs.get('poly_orders', [3, 3])
+            y_at_borders = kwargs.get('y_at_borders', 'int_at_borders')
+            fit_method = kwargs.get('fit_method', 'ModPoly')
+        #############################
+
+        if not ascending_wn:
+            raw_data = np.flip(raw_data, axis=1)
+            wavenumbers = np.flip(wavenumbers)
+
+        wavenumbers_start = wavenumbers
+        # previous_dev = 0
+
+        for ii, current_spectrum in enumerate(tqdm(raw_data)):
+            wavenumbers = wavenumbers_start
+
+            if mode == baseline_modes[7]:  # 'PPF'
+                if y_at_borders == 'int_at_borders':
+                    y_at_borders_values = y_at_x(
+                        segment_borders, wavenumbers, current_spectrum)
+                else:
+                    y_at_borders_values = y_at_borders
+
+            for jj in range(int(n_iter)):
+                if mode in baseline_modes[5:7]:  # ModPoly, IModPoly
+                    # The polynomial_fit method from pyRegression is only used
+                    # if constraints are to be considered because the numpy
+                    # polyfit method is faster.
+                    if (fixed_points is not None) or (
+                            fixed_slopes is not None):
+                        fit_data, fit_coeffs = polynomial_fit(
+                            wavenumbers, current_spectrum, poly_order,
+                            fixed_points=fixed_points,
+                            fixed_slopes=fixed_slopes)
+                    else:
+                        fit_coeffs = np.polynomial.polynomial.polyfit(
+                            wavenumbers, current_spectrum, poly_order)
+                        fit_data = np.polynomial.polynomial.polyval(
+                            wavenumbers, fit_coeffs)
+                else:  # PPF
+                    fit_data, fit_coeffs = piecewise_polynomial_fit(
+                        wavenumbers, current_spectrum, segment_borders,
+                        poly_orders, y_at_borders=y_at_borders_values,
+                        slope_at_borders=None)
+
+                # ModPoly or PPF with ModPoly
+                if (mode == baseline_modes[5]) or (
+                        (mode == baseline_modes[7]) and (fit_method=='ModPoly')
+                        ):
+                    dev = 0
+                # IModPoly or PPF with IModPoly
+                else:
+                    residual = current_spectrum - fit_data
+                    dev = residual.std()
+                    # if abs((dev - previous_dev)/dev) < 0.01:
+                    #    break
+
+                if jj == 0:
+                    mask = (current_spectrum <= fit_data + dev)
+                    wavenumbers = wavenumbers[mask]
+                    current_spectrum = current_spectrum[mask]
+                    fit_data = fit_data[mask]
+                np.copyto(current_spectrum, fit_data + dev,
+                          where=(current_spectrum >= (fit_data+dev)))
+                # previous_dev = dev
+
+            if mode in baseline_modes[5:7]:  # ModPoly, IModPoly
+                baseline_data[ii, :] = np.polynomial.polynomial.polyval(
+                    wavenumbers_start, fit_coeffs)
+            else:  # PPF
+                baseline_data[ii, :] = piecewise_polynomial(
+                    wavenumbers_start, fit_coeffs,
+                    segment_borders=segment_borders)
+
+        if not ascending_wn:
+            baseline_data = np.flip(baseline_data, axis=1)
+            # raw_data = np.flip(raw_data, axis=1)
+
+    else:
+        raise ValueError('No valid baseline mode entered. Allowed modes are '
+                         '{0}'.format(baseline_modes))
+
+    if transform:
+        baseline_data = transform_spectra(
+            baseline_data, 'log_log_sqrt', direction='inverse',
+            min_value=spectra_minimum_value)
+
+    return np.around(baseline_data, decimals=6)
```

### Comparing `pyPreprocessing-0.0.1/src/pyPreprocessing/smoothing.py` & `pyPreprocessing-0.0.2/src/pyPreprocessing/smoothing.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,356 +1,362 @@
-# -*- coding: utf-8 -*-
-"""
-Provides functions for smoothing and filtering of data rows oganized in 2D
-numpy arrays.
-"""
-
-import numpy as np
-import pandas as pd
-from scipy.signal import savgol_filter
-from scipy.interpolate import interp1d
-from sklearn.decomposition import PCA
-
-
-def smoothing(raw_data, mode, interpolate=False, point_mirror=True, **kwargs):
-    """
-    Smoothes data rows with different algorithms.
-
-    Parameters
-    ----------
-    raw_data : ndarray
-        2D numpy array with the shape (N,M) containing N data rows to be
-        smoothed. Each data row is represented by row in numpy array and
-        contains M values. If only one data row is present, raw_data has the
-        shape (1,M).
-    mode : str
-        Algorithm used for smoothing. Allowed modes are 'sav_gol' for Savitzky-
-        Golay, 'rolling_median' for a median filter, 'pca' for smoothing based
-        on principal component analysis, 'weighted_moving_average' for a
-        moving average that uses weights, so e.g. can decide if values in the
-        window are used for or excluded from averaging.
-    interpolate : boolean
-        False if x coordinate is evenly spaced. True if x coordinate is not
-        evenly spaced, then raw_data is interpolated to an evenly spaced
-        x coordinate. Default is False
-    point_mirror : boolean
-        Dataset is point reflected at both end points before smoothing to
-        reduce artifacts at the data edges.
-    **kwargs for interpolate=True
-        x_coordinate : ndarray
-            1D numpy array with shape (M,) used for interpolation.
-        data_points : int, optional
-            number of data points returned after interpolation. Default is one
-            order of magnitude more than M.
-        return_type : string, optional
-            Defines if the interpolated dataset with a number of data_points
-            is returned ('interp') or if the returned dataset has the same
-            dimensions and x_coordinates like the original dataset ('orig').
-            Default is 'interp'.
-    **kwargs for different smoothing modes
-        sav_gol:
-            deriv : int
-                Derivative order to be calculated. Default is 0 (no
-                derivative).
-            savgol_points : int
-                Number of point defining one side of the Savitzky-Golay window.
-                Total window is 2*savgol_points+1. Default is 9.
-            poly_order : int
-                Polynomial order used for polynomial fitting of the Savitzky-
-                Golay window. Default is 2.
-            savgol_mode : str
-                Must be ‘mirror’, ‘constant’, ‘nearest’, ‘wrap’ or ‘interp’.
-                See documentation of scipy.signal.savgol_filter.
-        rolling_median:
-            window: int
-                Data points included in rolling window used for median
-                calculations. Default is 5.
-        pca:
-            pca_components : int
-                Number of principal components used to reconstruct the original
-                data. Default is 5.
-        weighted_moving_average:
-            weights : list of float
-                The number of entries decide the window length used for
-                smoothing. A value > 0 means that the value is used with the
-                specified weight, a value of 0 means the value is excluded,
-                e.g. [1, 0, 1] is a window of size 3 in which the center point
-                is exluded from the calculations. Default is [1, 1, 0, 1, 1].
-
-    Returns
-    -------
-    ndarray or tuple of ndarrays
-        2D numpy array containing the smoothed data in the same shape as
-        raw_data if interpolate is false. Else tuple containing interpolated
-        x coordinates and 2D numpy array in the shape of
-        (N,10**np.ceil(np.log10(len(x_coordinate)))). In case of mode is
-        weighted_moving_average, the corresponding standard deviations are
-        also calulated and a tuple with the smoothed data and the standard
-        deviations is returned.
-
-    """
-    # copy of raw_data for later restoration of data edges
-    raw_old = pd.DataFrame(raw_data.copy())
-    # Preprocessing of input data for unevenly spaced x coordinate
-    if interpolate:
-        x_coordinate = kwargs.get('x_coordinate', np.linspace(
-            0, 1000, raw_data.shape[1]))
-        data_points = kwargs.get('data_points',
-                                 int(10**np.ceil(np.log10(len(x_coordinate)))))
-
-        itp = interp1d(x_coordinate, raw_data, kind='linear')
-        x_interpolated = np.linspace(x_coordinate[0], x_coordinate[-1],
-                                     data_points)
-        raw_data = itp(x_interpolated)
-
-    # Optional extension of smoothed data by point mirrored raw data.
-    if point_mirror:
-        raw_data = np.concatenate(
-            ((-np.flip(raw_data, axis=1)+2*raw_data[:, 0, np.newaxis])[:, :-1],
-             raw_data, (-np.flip(raw_data, axis=1) +
-                        2*raw_data[:, -1, np.newaxis])[:, 1:]), axis=1)
-        #raw_data = np.concatenate((-np.squeeze(raw_data.T)[::-1]+2*np.squeeze(raw_data.T)[0],np.squeeze(raw_data.T),-np.squeeze(raw_data.T)[::-1]+2*np.squeeze(raw_data.T)[-1]))[np.newaxis]
-
-    smoothing_modes = ['sav_gol', 'rolling_median', 'pca',
-                       'weighted_moving_average']
-
-    if mode == smoothing_modes[0]:  # sav_gol
-        deriv = kwargs.get('deriv', 0)
-        savgol_points = kwargs.get('savgol_points', 9)
-        poly_order = kwargs.get('poly_order', 2)
-        savgol_mode = kwargs.get('savgol_mode', 'nearest')
-
-        smoothed_data = savgol_filter(raw_data, 1+2*savgol_points, poly_order,
-                                      deriv=deriv, axis=1, mode=savgol_mode)
-
-    elif mode == smoothing_modes[1]:  # rolling_median
-        window = kwargs.get('window', 5)
-        # next line due to pandas rolling window, look for numpy solution
-        raw_data = pd.DataFrame(raw_data)
-
-        edge_value_count = int((window-1)/2)
-        smoothed_data = raw_data.rolling(
-                window, axis=1, center=True).median().iloc[
-                :, edge_value_count:-edge_value_count]
-
-        # On the data edges, the original data is used, so the edges are not
-        # smoothed (only relevant if point_mirror is False).
-        smoothed_data = pd.concat(
-            [raw_old.iloc[:, 0:edge_value_count], smoothed_data,
-             raw_old.iloc[:, -1-edge_value_count:]], axis=1).values
-
-    elif mode == smoothing_modes[2]:  # pca
-        pca_components = kwargs.get('pca_components', 5)
-
-        pca = PCA(n_components=pca_components)
-        scores = pca.fit_transform(raw_data)
-        loadings = pca.components_
-
-        smoothed_data = (
-            np.dot(scores, loadings) + np.mean(raw_data, axis=0))
-
-    elif mode == smoothing_modes[3]:  # weighted_moving_average
-        weights = kwargs.get('weights', [1, 1, 0, 1, 1])
-
-        window_size = len(weights)
-        value_count = raw_data.shape[1]
-        edge_value_count = int((window_size-1)/2)
-        remaining_values = value_count-window_size+1
-
-        column_indices = np.repeat(
-            np.arange(window_size)[np.newaxis], remaining_values, axis=0
-            ) + np.arange(remaining_values)[:, np.newaxis]
-        # column_indices = column_indices[:, weights]
-
-        # the following step multiplies the total value number with
-        # window_size, so might be problematic for large datasets
-        value_array = np.squeeze(raw_data[np.newaxis][:, :, column_indices])
-        if len(value_array.shape) == 2:
-            value_array = value_array[np.newaxis]
-        smoothed_data, selective_std = weighted_mean_std(value_array, weights)
-        smoothed_data = pd.DataFrame(smoothed_data)
-
-        # selective_std = np.std(value_array, axis=2)
-        # On the edges, the std is calculated from the reduced number of edge
-        # data points (only relevant if point_mirror is False).
-        selective_std = np.concatenate((
-            np.repeat(np.std(raw_old.values[:, 0:edge_value_count], axis=1),
-                      edge_value_count).reshape(-1, edge_value_count),
-            selective_std,
-            np.repeat(np.std(raw_old.values[:, -edge_value_count:], axis=1),
-                      edge_value_count).reshape(-1, edge_value_count)
-            ), axis=1)
-
-        # On the data edges, the original data is used, so the edges are not
-        # smoothed (only relevant if point_mirror is False).
-        raw_data = pd.DataFrame(raw_data)
-        smoothed_data = pd.concat(
-            [raw_old.iloc[:, 0:edge_value_count], smoothed_data,
-             raw_old.iloc[:, -edge_value_count:]], axis=1).values
-
-    else:
-        raise ValueError('No valid smoothing mode entered. Allowed modes are '
-                         '{0}'.format(smoothing_modes))
-
-    # Removal of previously added point mirrored data.
-    if point_mirror:
-        smoothed_data = smoothed_data[
-            :, int(np.ceil(smoothed_data.shape[1]/3)-1):
-                int(2*np.ceil(smoothed_data.shape[1]/3)-1)]
-        if mode == smoothing_modes[3]:  # weighted_moving_average
-            selective_std = selective_std[
-                :, int(np.ceil(selective_std.shape[1]/3)-1):
-                    int(2*np.ceil(selective_std.shape[1]/3)-1)]
-
-    if interpolate:
-        return_type = kwargs.get('return_type', 'interp')
-        if return_type == 'interp':
-            return (x_interpolated, smoothed_data)
-        elif return_type == 'orig':
-            f = interp1d(x_interpolated, smoothed_data, kind='linear')
-            return (x_coordinate, f(x_coordinate))
-        else:
-            raise ValueError('No valid return_type given.')
-    elif mode == smoothing_modes[3]:  # weighted_moving_average
-        return (smoothed_data, selective_std)
-    else:
-        return smoothed_data
-
-
-def weighted_mean_std(values, weights, std=True):
-    """
-    Calculate the weighted mean and (biased) standard deviation of values.
-
-    Parameters
-    ----------
-    values : ndarray
-        An n-dimensional array in the shape (..., M) with data rows with M
-        elements. Calculations are performed for each data row in the last
-        dimension of values.
-    weights : list of float
-        A list containing the weights used in the calculations. Must contain
-        M elements.
-    std : bool, optional
-        Decides if the weighted standard deviation is also calculated, default
-        is True.
-
-    Returns
-    -------
-    weighted_mean : ndarray
-        An (n-1)-dimensional array containing the weighted means for the data
-        rows, so has the shape of values without the last dimension.
-    weighted_std : ndarray
-        An (n-1)-dimensional array containing the weighted standard deviations
-        for the data rows, so has the shape of values without the last
-        dimension. Only in case of std=True.
-
-    """
-    weighted_mean = np.average(values, weights=weights, axis=-1)
-    if std:
-        weighted_std = np.sqrt(
-            np.average((values-weighted_mean[..., np.newaxis])**2,
-                       weights=weights, axis=-1))
-        return (weighted_mean, weighted_std)
-    else:
-        return weighted_mean
-
-
-def filtering(raw_data, mode, fill='NaN', **kwargs):
-    """
-    Filter data rows with different algorithms.
-
-    Filtered values are replaced by np.nan.
-
-    Parameters
-    ----------
-    raw_data : ndarray
-        2D numpy array with the shape (N,M) containing N data rows to be
-        filtered. Each data row is represented by row in numpy array and
-        contains M values. If only one data row is present, raw_data has the
-        shape (1, M).
-    mode : str
-        Algorithm used for filtering. Allowed modes are 'spike_filter' for
-        sharp peaks, 'max_thresh' for removal of values above or equal to a
-        maximum threshold, 'min_thresh' for removal of values below or equal to
-        a minumum threshold.
-    fill : str, optional
-        Decides the way filtered points are replaced. Currently 'NaN'
-        where values are replaced by np.nan, 'zeros' where values are
-        replaced by zeros, or 'mov_avg' (only for mode=='spike_filter') where
-        values are replaced by the weighted moving average.
-    **kwargs for different filter modes
-        spike_filter:
-            weights : list of float, optional
-                The number of entries decide the window length used for
-                smoothing. A value > 0 means that the value is used with the
-                specified weight, a value of 0 means the value is excluded,
-                e.g. [1, 0, 1] is a window of size 3 in which the center point
-                is exluded from the calculations. Default is [1, 1, 0, 1, 1].
-            std_factor : float, optional
-                The number of standard deviations a value is allowed to be away
-                from the moving average before it is removed by the filter.
-                Mean and standard deviation are calculated in a rolling fashion
-                so that only sharp peaks are found. Default is 2.
-            point_mirror : bool, optional
-                Decides if the data edges are point mirrored before rolling
-                average. If True, estimates of mean and standard deviation also
-                at the edges are obtained. If False, data at the edges are kept
-                like in the original. Default is False.
-            interpolate : boolean, optional
-                False if x coordinate is evenly spaced. True if x coordinate is
-                not evenly spaced, then raw_data is interpolated to an evenly
-                spaced x coordinate. Default is False
-        max_thresh
-            max:_thresh : float, optional
-                The maximum threshold. Default is 1000.
-        min_thresh
-            min_thresh : float, optional
-                The minimum threshold. Default is 0.
-
-    Returns
-    -------
-    ndarray
-        Returns an ndarray with dimensions like raw_data. Filtered points are
-        changed according to the fill selected.
-
-    """
-    filter_modes = ['spike_filter', 'max_thresh', 'min_thresh']
-    if fill == 'NaN':
-        fill_value = np.nan
-    elif fill == 'zeros':
-        fill_value = 0
-
-    if mode == filter_modes[0]:  # spike_filter
-        weights = kwargs.get('weights', [1, 1, 0, 1, 1])
-        window_size = len(weights)
-        std_factor = kwargs.get('std_factor', 2)
-        point_mirror = kwargs.get('point_mirror', False)
-        interpolate = kwargs.get('interpolate', False)
-
-        mov_avg, mov_std = smoothing(
-            raw_data, 'weighted_moving_average', point_mirror=point_mirror,
-            interpolate=interpolate, weights=weights)
-
-        diffs = np.absolute(raw_data - mov_avg)
-
-        if fill == 'mov_avg':
-            fill_value = mov_avg[diffs > std_factor*mov_std]
-        raw_data[diffs > std_factor*mov_std] = fill_value
-        filtered_data = raw_data
-
-    elif mode == filter_modes[1]:  # max_thresh
-        maximum_threshold = kwargs.get('max_thresh', 1000)
-        raw_data = raw_data.astype(float)
-        raw_data[raw_data > maximum_threshold] = fill_value
-        filtered_data = raw_data
-
-    elif mode == filter_modes[2]:  # min_thresh
-        minimum_threshold = kwargs.get('min_thresh', 0)
-        raw_data = raw_data.astype(float)
-        raw_data[raw_data < minimum_threshold] = fill_value
-        filtered_data = raw_data
-
-    else:
-        raise ValueError('No valid filter mode entered. Allowed modes are '
-                         '{0}'.format(filter_modes))
-        
-    return filtered_data
+# -*- coding: utf-8 -*-
+"""
+Provides functions for smoothing and filtering of data rows oganized in 2D
+numpy arrays.
+"""
+
+import numpy as np
+import pandas as pd
+from scipy.signal import savgol_filter
+from scipy.interpolate import interp1d
+from sklearn.decomposition import PCA
+
+
+def smoothing(raw_data, mode, interpolate=False, point_mirror=True, **kwargs):
+    """
+    Smoothes data rows with different algorithms.
+
+    Parameters
+    ----------
+    raw_data : ndarray
+        2D numpy array with the shape (N,M) containing N data rows to be
+        smoothed. Each data row is represented by row in numpy array and
+        contains M values. If only one data row is present, raw_data has the
+        shape (1,M).
+    mode : str
+        Algorithm used for smoothing. Allowed modes are 'sav_gol' for Savitzky-
+        Golay, 'rolling_median' for a median filter, 'pca' for smoothing based
+        on principal component analysis, 'weighted_moving_average' for a
+        moving average that uses weights, so e.g. can decide if values in the
+        window are used for or excluded from averaging.
+    interpolate : boolean
+        False if x coordinate is evenly spaced. True if x coordinate is not
+        evenly spaced, then raw_data is interpolated to an evenly spaced
+        x coordinate. Default is False
+    point_mirror : boolean
+        Dataset is point reflected at both end points before smoothing to
+        reduce artifacts at the data edges.
+    **kwargs for interpolate=True
+        x_coordinate : ndarray
+            1D numpy array with shape (M,) used for interpolation.
+        data_points : int, optional
+            number of data points returned after interpolation. Default is one
+            order of magnitude more than M.
+        return_type : string, optional
+            Defines if the interpolated dataset with a number of data_points
+            is returned ('interp') or if the returned dataset has the same
+            dimensions and x_coordinates like the original dataset ('orig').
+            Default is 'interp'.
+    **kwargs for different smoothing modes
+        sav_gol:
+            deriv : int
+                Derivative order to be calculated. Default is 0 (no
+                derivative).
+            savgol_points : int
+                Number of point defining one side of the Savitzky-Golay window.
+                Total window is 2*savgol_points+1. Default is 9.
+            poly_order : int
+                Polynomial order used for polynomial fitting of the Savitzky-
+                Golay window. Default is 2.
+            savgol_mode : str
+                Must be ‘mirror’, ‘constant’, ‘nearest’, ‘wrap’ or ‘interp’.
+                See documentation of scipy.signal.savgol_filter.
+        rolling_median:
+            window: int
+                Data points included in rolling window used for median
+                calculations. Default is 5.
+        pca:
+            pca_components : int
+                Number of principal components used to reconstruct the original
+                data. Default is 5.
+        weighted_moving_average:
+            weights : list of float
+                The number of entries decide the window length used for
+                smoothing. A value > 0 means that the value is used with the
+                specified weight, a value of 0 means the value is excluded,
+                e.g. [1, 0, 1] is a window of size 3 in which the center point
+                is exluded from the calculations. Default is [1, 1, 0, 1, 1].
+
+    Returns
+    -------
+    ndarray or tuple of ndarrays
+        2D numpy array containing the smoothed data in the same shape as
+        raw_data if interpolate is false. Else tuple containing interpolated
+        x coordinates and 2D numpy array in the shape of
+        (N,10**np.ceil(np.log10(len(x_coordinate)))). In case of mode is
+        weighted_moving_average, the corresponding standard deviations are
+        also calulated and a tuple with the smoothed data and the standard
+        deviations is returned.
+
+    """
+    # copy of raw_data for later restoration of data edges
+    raw_old = pd.DataFrame(raw_data.copy())
+    # Preprocessing of input data for unevenly spaced x coordinate
+    if interpolate:
+        x_coordinate = kwargs.get('x_coordinate', np.linspace(
+            0, 1000, raw_data.shape[1]))
+        data_points = kwargs.get('data_points',
+                                 int(10**np.ceil(np.log10(len(x_coordinate)))))
+
+        itp = interp1d(x_coordinate, raw_data, kind='linear')
+        x_interpolated = np.linspace(x_coordinate[0], x_coordinate[-1],
+                                     data_points)
+        raw_data = itp(x_interpolated)
+
+    # Optional extension of smoothed data by point mirrored raw data.
+    if point_mirror:
+        raw_data = np.concatenate(
+            ((-np.flip(raw_data, axis=1)+2*raw_data[:, 0, np.newaxis])[:, :-1],
+             raw_data, (-np.flip(raw_data, axis=1) +
+                        2*raw_data[:, -1, np.newaxis])[:, 1:]), axis=1)
+        #raw_data = np.concatenate((-np.squeeze(raw_data.T)[::-1]+2*np.squeeze(raw_data.T)[0],np.squeeze(raw_data.T),-np.squeeze(raw_data.T)[::-1]+2*np.squeeze(raw_data.T)[-1]))[np.newaxis]
+
+    smoothing_modes = ['sav_gol', 'rolling_median', 'pca',
+                       'weighted_moving_average']
+
+    if mode == smoothing_modes[0]:  # sav_gol
+        deriv = kwargs.get('deriv', 0)
+        savgol_points = kwargs.get('savgol_points', 9)
+        poly_order = kwargs.get('poly_order', 2)
+        savgol_mode = kwargs.get('savgol_mode', 'nearest')
+
+        smoothed_data = savgol_filter(raw_data, 1+2*savgol_points, poly_order,
+                                      deriv=deriv, axis=1, mode=savgol_mode)
+
+    elif mode == smoothing_modes[1]:  # rolling_median
+        window = kwargs.get('window', 5)
+        # next line due to pandas rolling window, look for numpy solution
+        raw_data = pd.DataFrame(raw_data)
+
+        edge_value_count = int((window-1)/2)
+        smoothed_data = raw_data.rolling(
+                window, axis=1, center=True).median().iloc[
+                :, edge_value_count:-edge_value_count]
+
+        # On the data edges, the original data is used, so the edges are not
+        # smoothed (only relevant if point_mirror is False).
+        smoothed_data = pd.concat(
+            [raw_old.iloc[:, 0:edge_value_count], smoothed_data,
+             raw_old.iloc[:, -1-edge_value_count:]], axis=1).values
+
+    elif mode == smoothing_modes[2]:  # pca
+        pca_components = kwargs.get('pca_components', 5)
+
+        pca = PCA(n_components=pca_components)
+        scores = pca.fit_transform(raw_data)
+        loadings = pca.components_
+
+        smoothed_data = (
+            np.dot(scores, loadings) + np.mean(raw_data, axis=0))
+
+    elif mode == smoothing_modes[3]:  # weighted_moving_average
+        weights = kwargs.get('weights', [1, 1, 0, 1, 1])
+
+        window_size = len(weights)
+        value_count = raw_data.shape[1]
+        edge_value_count = int((window_size-1)/2)
+        remaining_values = value_count-window_size+1
+
+        column_indices = np.repeat(
+            np.arange(window_size)[np.newaxis], remaining_values, axis=0
+            ) + np.arange(remaining_values)[:, np.newaxis]
+        # column_indices = column_indices[:, weights]
+
+        # the following step multiplies the total value number with
+        # window_size, so might be problematic for large datasets
+        value_array = np.squeeze(raw_data[np.newaxis][:, :, column_indices])
+        if len(value_array.shape) == 2:
+            value_array = value_array[np.newaxis]
+        smoothed_data, selective_std = weighted_mean_std(value_array, weights)
+        smoothed_data = pd.DataFrame(smoothed_data)
+
+        # selective_std = np.std(value_array, axis=2)
+        # On the edges, the std is calculated from the reduced number of edge
+        # data points (only relevant if point_mirror is False).
+        selective_std = np.concatenate((
+            np.repeat(np.std(raw_old.values[:, 0:edge_value_count], axis=1),
+                      edge_value_count).reshape(-1, edge_value_count),
+            selective_std,
+            np.repeat(np.std(raw_old.values[:, -edge_value_count:], axis=1),
+                      edge_value_count).reshape(-1, edge_value_count)
+            ), axis=1)
+
+        # On the data edges, the original data is used, so the edges are not
+        # smoothed (only relevant if point_mirror is False).
+        raw_data = pd.DataFrame(raw_data)
+        smoothed_data = pd.concat(
+            [raw_old.iloc[:, 0:edge_value_count], smoothed_data,
+             raw_old.iloc[:, -edge_value_count:]], axis=1).values
+
+    else:
+        raise ValueError('No valid smoothing mode entered. Allowed modes are '
+                         '{0}'.format(smoothing_modes))
+
+    # Removal of previously added point mirrored data.
+    if point_mirror:
+        smoothed_data = smoothed_data[
+            :, int(np.ceil(smoothed_data.shape[1]/3)-1):
+                int(2*np.ceil(smoothed_data.shape[1]/3)-1)]
+        if mode == smoothing_modes[3]:  # weighted_moving_average
+            selective_std = selective_std[
+                :, int(np.ceil(selective_std.shape[1]/3)-1):
+                    int(2*np.ceil(selective_std.shape[1]/3)-1)]
+
+    if interpolate:
+        return_type = kwargs.get('return_type', 'interp')
+        if return_type == 'interp':
+            return (x_interpolated, smoothed_data)
+        elif return_type == 'orig':
+            f = interp1d(x_interpolated, smoothed_data, kind='linear')
+            return (x_coordinate, f(x_coordinate))
+        else:
+            raise ValueError('No valid return_type given.')
+    elif mode == smoothing_modes[3]:  # weighted_moving_average
+        return (smoothed_data, selective_std)
+    else:
+        return smoothed_data
+
+
+def weighted_mean_std(values, weights, std=True):
+    """
+    Calculate the weighted mean and (biased) standard deviation of values.
+
+    Parameters
+    ----------
+    values : ndarray
+        An n-dimensional array in the shape (..., M) with data rows with M
+        elements. Calculations are performed for each data row in the last
+        dimension of values.
+    weights : list of float
+        A list containing the weights used in the calculations. Must contain
+        M elements.
+    std : bool, optional
+        Decides if the weighted standard deviation is also calculated, default
+        is True.
+
+    Returns
+    -------
+    weighted_mean : ndarray
+        An (n-1)-dimensional array containing the weighted means for the data
+        rows, so has the shape of values without the last dimension.
+    weighted_std : ndarray
+        An (n-1)-dimensional array containing the weighted standard deviations
+        for the data rows, so has the shape of values without the last
+        dimension. Only in case of std=True.
+
+    """
+    weighted_mean = np.average(values, weights=weights, axis=-1)
+    if std:
+        weighted_std = np.sqrt(
+            np.average((values-weighted_mean[..., np.newaxis])**2,
+                       weights=weights, axis=-1))
+        return (weighted_mean, weighted_std)
+    else:
+        return weighted_mean
+
+
+def filtering(raw_data, mode, fill='NaN', **kwargs):
+    """
+    Filter data rows with different algorithms.
+
+    Filtered values are replaced by np.nan.
+
+    Parameters
+    ----------
+    raw_data : ndarray
+        2D numpy array with the shape (N,M) containing N data rows to be
+        filtered. Each data row is represented by row in numpy array and
+        contains M values. If only one data row is present, raw_data has the
+        shape (1, M).
+    mode : str
+        Algorithm used for filtering. Allowed modes are 'spike_filter' for
+        sharp peaks, 'max_thresh' for removal of values above or equal to a
+        maximum threshold, 'min_thresh' for removal of values below or equal to
+        a minumum threshold.
+    fill : str, optional
+        Decides the way filtered points are replaced. Currently 'NaN'
+        where values are replaced by np.nan, 'zeros' where values are
+        replaced by zeros, or 'mov_avg' (only for mode=='spike_filter') where
+        values are replaced by the weighted moving average.
+    **kwargs for different filter modes
+        spike_filter:
+            weights : list of float, optional
+                The number of entries decide the window length used for
+                smoothing. A value > 0 means that the value is used with the
+                specified weight, a value of 0 means the value is excluded,
+                e.g. [1, 0, 1] is a window of size 3 in which the center point
+                is exluded from the calculations. Default is [1, 1, 0, 1, 1].
+            std_factor : float, optional
+                The number of standard deviations a value is allowed to be away
+                from the moving average before it is removed by the filter.
+                Mean and standard deviation are calculated in a rolling fashion
+                so that only sharp peaks are found. Default is 2.
+            point_mirror : bool, optional
+                Decides if the data edges are point mirrored before rolling
+                average. If True, estimates of mean and standard deviation also
+                at the edges are obtained. If False, data at the edges are kept
+                like in the original. Default is False.
+            interpolate : boolean, optional
+                False if x coordinate is evenly spaced. True if x coordinate is
+                not evenly spaced, then raw_data is interpolated to an evenly
+                spaced x coordinate. Default is False
+        max_thresh
+            max:_thresh : float, optional
+                The maximum threshold. Default is 1000.
+        min_thresh
+            min_thresh : float, optional
+                The minimum threshold. Default is 0.
+
+    Returns
+    -------
+    ndarray
+        Returns an ndarray with dimensions like raw_data. Filtered points are
+        changed according to the fill selected.
+
+    """
+    filter_modes = ['spike_filter', 'max_thresh', 'min_thresh']
+    fill_values = ['NaN', 'zeros', 'mov_avg']
+    if fill == 'NaN':
+        fill_value = np.nan
+    elif fill == 'zeros':
+        fill_value = 0
+    elif ((fill not in fill_values) or
+          (fill == 'mov_avg' and mode != filter_modes[0])):
+        raise ValueError('No valid fill value given for this mode.')
+
+    if mode == filter_modes[0]:  # spike_filter
+        weights = kwargs.get('weights', [1, 1, 0, 1, 1])
+        window_size = len(weights)
+        std_factor = kwargs.get('std_factor', 2)
+        point_mirror = kwargs.get('point_mirror', False)
+        interpolate = kwargs.get('interpolate', False)
+
+        filtered_data = raw_data.copy()
+        mov_avg, mov_std = smoothing(
+            filtered_data, 'weighted_moving_average',
+            point_mirror=point_mirror, interpolate=interpolate,
+            weights=weights)
+
+        diffs = np.absolute(filtered_data - mov_avg)
+
+        if fill == 'mov_avg':
+            fill_value = mov_avg[diffs > std_factor*mov_std]
+        filtered_data[diffs > std_factor*mov_std] = fill_value
+        # filtered_data = raw_data
+
+    elif mode == filter_modes[1]:  # max_thresh
+        maximum_threshold = kwargs.get('max_thresh', 1000)
+        filtered_data = raw_data.copy().astype(float)
+        filtered_data[filtered_data > maximum_threshold] = fill_value
+        # filtered_data = raw_data
+
+    elif mode == filter_modes[2]:  # min_thresh
+        minimum_threshold = kwargs.get('min_thresh', 0)
+        filtered_data = raw_data.copy().astype(float)
+        filtered_data[filtered_data < minimum_threshold] = fill_value
+        # filtered_data = raw_data
+
+    else:
+        raise ValueError('No valid filter mode entered. Allowed modes are '
+                         '{0}'.format(filter_modes))
+
+    return filtered_data
```

### Comparing `pyPreprocessing-0.0.1/src/pyPreprocessing.egg-info/PKG-INFO` & `pyPreprocessing-0.0.2/src/pyPreprocessing.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,32 @@
-Metadata-Version: 2.1
-Name: pyPreprocessing
-Version: 0.0.1
-Summary: package preprocessing of datasets, especially from spectroscopy
-Home-page: https://github.com/AlexanderSouthan/pyPreprocessing
-Author: Alexander Southan
-Author-email: alexander.southan@web.de
-License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/AlexanderSouthan/pyPreprocessing/issues
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
-[![build workflow](https://github.com/AlexanderSouthan/pyPreprocessing/actions/workflows/main.yml/badge.svg)](https://github.com/AlexanderSouthan/pyPreprocessing/actions/workflows/main.yml)
-[![codecov](https://codecov.io/gh/AlexanderSouthan/pyPreprocessing/branch/master/graph/badge.svg?token=7GN1K2MVJ3)](https://codecov.io/gh/AlexanderSouthan/pyPreprocessing)
-
-# pyPreprocessing
-## General information
-For preprocessing of datasets like Raman spectra, infrared spectra, UV/Vis
-spectra, but also HPLC data and many other types of data, currently via
-baseline correction, smoothing, filtering, transformation, normalization and
-derivative. It relies on numpy, pandas, scipy, tqdm and scikit-learn, but also
-on https://github.com/AlexanderSouthan/pyRegression for the introduction of
-equality constraints into the polynomial baseline estimation methods, and
-https://github.com/AlexanderSouthan/little_helpers.
-
-## Documentation
-Please visit:
-https://alexandersouthan.github.io/pyPreprocessing/
-
-
+Metadata-Version: 2.1
+Name: pyPreprocessing
+Version: 0.0.2
+Summary: package preprocessing of datasets, especially from spectroscopy
+Home-page: https://github.com/AlexanderSouthan/pyPreprocessing
+Author: Alexander Southan
+Author-email: alexander.southan@web.de
+Project-URL: Bug Tracker, https://github.com/AlexanderSouthan/pyPreprocessing/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
+[![build workflow](https://github.com/AlexanderSouthan/pyPreprocessing/actions/workflows/main.yml/badge.svg)](https://github.com/AlexanderSouthan/pyPreprocessing/actions/workflows/main.yml)
+[![codecov](https://codecov.io/gh/AlexanderSouthan/pyPreprocessing/branch/master/graph/badge.svg?token=7GN1K2MVJ3)](https://codecov.io/gh/AlexanderSouthan/pyPreprocessing)
+
+# pyPreprocessing
+## General information
+For preprocessing of datasets like Raman spectra, infrared spectra, UV/Vis
+spectra, but also HPLC data and many other types of data, currently via
+baseline correction, smoothing, filtering, transformation, normalization and
+derivative. It relies on numpy, pandas, scipy, tqdm and scikit-learn, but also
+on https://github.com/AlexanderSouthan/pyDataFitting for the introduction of
+equality constraints into the polynomial baseline estimation methods, and
+https://github.com/AlexanderSouthan/little_helpers.
+
+## Documentation
+Please visit:
+https://alexandersouthan.github.io/pyPreprocessing/
```

