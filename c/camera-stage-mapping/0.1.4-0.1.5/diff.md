# Comparing `tmp/camera-stage-mapping-0.1.4.tar.gz` & `tmp/camera_stage_mapping-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "camera-stage-mapping-0.1.4.tar", last modified: Fri Sep  4 15:58:08 2020, max compression
+gzip compressed data, was "camera_stage_mapping-0.1.5.tar", max compression
```

## Comparing `camera-stage-mapping-0.1.4.tar` & `camera_stage_mapping-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rw-r--r--   0        0        0    35141 2020-09-04 15:57:04.881617 camera-stage-mapping-0.1.4/LICENSE
--rw-r--r--   0        0        0     2418 2020-09-04 15:57:04.881617 camera-stage-mapping-0.1.4/README.md
--rw-r--r--   0        0        0      900 2020-09-04 15:57:04.881617 camera-stage-mapping-0.1.4/camera_stage_mapping/__init__.py
--rw-r--r--   0        0        0     5205 2020-09-04 15:57:04.881617 camera-stage-mapping-0.1.4/camera_stage_mapping/array_with_attrs.py
--rw-r--r--   0        0        0    13758 2020-09-04 15:57:04.881617 camera-stage-mapping-0.1.4/camera_stage_mapping/camera_stage_calibration_1d.py
--rw-r--r--   0        0        0     6245 2020-09-04 15:57:04.881617 camera-stage-mapping-0.1.4/camera_stage_mapping/camera_stage_calibration_2d.py
--rw-r--r--   0        0        0    19625 2020-09-04 15:57:04.881617 camera-stage-mapping-0.1.4/camera_stage_mapping/camera_stage_tracker.py
--rw-r--r--   0        0        0    20728 2020-09-04 15:57:04.881617 camera-stage-mapping-0.1.4/camera_stage_mapping/camera_with_location.py.disabled
--rw-r--r--   0        0        0     4807 2020-09-04 15:57:04.881617 camera-stage-mapping-0.1.4/camera_stage_mapping/closed_loop_move.py
--rw-r--r--   0        0        0     5092 2020-09-04 15:57:04.881617 camera-stage-mapping-0.1.4/camera_stage_mapping/correlation_image_tracking.py
--rw-r--r--   0        0        0     7905 2020-09-04 15:57:04.881617 camera-stage-mapping-0.1.4/camera_stage_mapping/fft_image_tracking.py
--rw-r--r--   0        0        0    12056 2020-09-04 15:57:04.881617 camera-stage-mapping-0.1.4/camera_stage_mapping/ofm_extension.py
--rw-r--r--   0        0        0     3655 2020-09-04 15:57:04.881617 camera-stage-mapping-0.1.4/camera_stage_mapping/scan_coords_times.py
--rw-r--r--   0        0        0     1253 2020-09-04 15:57:04.889617 camera-stage-mapping-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     3392 2020-09-04 15:58:08.604821 camera-stage-mapping-0.1.4/setup.py
--rw-r--r--   0        0        0     3409 2020-09-04 15:58:08.605316 camera-stage-mapping-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    35141 2023-07-24 22:15:45.645677 camera_stage_mapping-0.1.5/LICENSE
+-rw-r--r--   0        0        0     2418 2023-07-24 22:15:45.645677 camera_stage_mapping-0.1.5/README.md
+-rw-r--r--   0        0        0      900 2023-07-24 22:15:45.645677 camera_stage_mapping-0.1.5/camera_stage_mapping/__init__.py
+-rw-r--r--   0        0        0     5205 2023-07-24 22:15:45.646677 camera_stage_mapping-0.1.5/camera_stage_mapping/array_with_attrs.py
+-rw-r--r--   0        0        0    13752 2023-07-24 22:15:45.646677 camera_stage_mapping-0.1.5/camera_stage_mapping/camera_stage_calibration_1d.py
+-rw-r--r--   0        0        0     6242 2023-07-24 22:15:45.646677 camera_stage_mapping-0.1.5/camera_stage_mapping/camera_stage_calibration_2d.py
+-rw-r--r--   0        0        0    19625 2023-07-24 22:15:45.646677 camera_stage_mapping-0.1.5/camera_stage_mapping/camera_stage_tracker.py
+-rw-r--r--   0        0        0    20725 2023-07-24 22:15:45.646677 camera_stage_mapping-0.1.5/camera_stage_mapping/camera_with_location.py.disabled
+-rw-r--r--   0        0        0     4807 2023-07-24 22:15:45.646677 camera_stage_mapping-0.1.5/camera_stage_mapping/closed_loop_move.py
+-rw-r--r--   0        0        0     5092 2023-07-24 22:15:45.646677 camera_stage_mapping-0.1.5/camera_stage_mapping/correlation_image_tracking.py
+-rw-r--r--   0        0        0     7896 2023-07-24 22:15:45.646677 camera_stage_mapping-0.1.5/camera_stage_mapping/fft_image_tracking.py
+-rw-r--r--   0        0        0    12056 2023-07-24 22:15:45.647677 camera_stage_mapping-0.1.5/camera_stage_mapping/ofm_extension.py
+-rw-r--r--   0        0        0     3655 2023-07-24 22:15:45.647677 camera_stage_mapping-0.1.5/camera_stage_mapping/scan_coords_times.py
+-rw-r--r--   0        0        0     1295 2023-07-24 22:15:45.653677 camera_stage_mapping-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3413 1970-01-01 00:00:00.000000 camera_stage_mapping-0.1.5/PKG-INFO
```

### Comparing `camera-stage-mapping-0.1.4/LICENSE` & `camera_stage_mapping-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `camera-stage-mapping-0.1.4/README.md` & `camera_stage_mapping-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `camera-stage-mapping-0.1.4/camera_stage_mapping/__init__.py` & `camera_stage_mapping-0.1.5/camera_stage_mapping/__init__.py`

 * *Files identical despite different names*

### Comparing `camera-stage-mapping-0.1.4/camera_stage_mapping/array_with_attrs.py` & `camera_stage_mapping-0.1.5/camera_stage_mapping/array_with_attrs.py`

 * *Files identical despite different names*

### Comparing `camera-stage-mapping-0.1.4/camera_stage_mapping/camera_stage_calibration_1d.py` & `camera_stage_mapping-0.1.5/camera_stage_mapping/camera_stage_calibration_1d.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 def direction_from_points(points):
     """Figure out the axis of motion from an Nx2 array of points.
     
     The return value is a normalised vector that points along the
     direction with the most motion.  This is the first *principal
     component* of the points.
     """
-    points = points.astype(np.float)
+    points = points.astype(float)
     points -= np.mean(points, axis=0)[np.newaxis, :]
     eigenvalues, eigenvectors = np.linalg.eig(np.cov(points.T))
     return eigenvectors[:,np.argmax(eigenvalues)]
 
 def apply_backlash(x, backlash=0, start_unwound=True):
     """Apply a basic model of backlash to a set of coordinates.
 
@@ -270,15 +270,15 @@
         stage_1d = np.sum(stage_pos * stage_direction[np.newaxis, :], axis=1)
         image_1d = np.sum(image_pos * image_direction[np.newaxis, :], axis=1)
         return stage_1d, image_1d
 
     ax[1].plot(*convert_moves(results["exponential_moves"]), 'o-')
     
     stage_pos, image_pos = convert_moves(results["linear_moves"])
-    model = apply_backlash(stage_pos, results["backlash"]).astype(np.float)
+    model = apply_backlash(stage_pos, results["backlash"]).astype(float)
     model *= results["pixels_per_step"]
     model += np.mean(image_pos) - np.mean(model)
     ax[1].plot(stage_pos, model, '-')
     ax[1].plot(stage_pos, image_pos, 'o')
     if results["backlash_corrected_moves"] is not None:
         ax[1].plot(*convert_moves(results["backlash_corrected_moves"]), '+')
```

### Comparing `camera-stage-mapping-0.1.4/camera_stage_mapping/camera_stage_calibration_2d.py` & `camera_stage_mapping-0.1.5/camera_stage_mapping/camera_stage_calibration_2d.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,15 @@
     finally:
         move(starting_position)
     # We then use least-squares to fit the XY part of the matrix relating 
     # pixels to distance
     # stage_positions should be the stage positions, with a zero mean.
     # image_positions should be the same, but calculated from the images
     stage_positions, image_positions, _ = tracker.history
-    stage_positions = stage_positions.astype(np.float)
+    stage_positions = stage_positions.astype(float)
     stage_positions -= np.mean(stage_positions, axis=0)
     stage_positions = stage_positions[:,:2] # ensure it's 2d
     image_positions -= np.mean(image_positions, axis=0)
     #image_positions *= -1 # To get the matrix right, we want the position of each
                         # image relative to the template, rather than the other way around
     A, res, rank, s = np.linalg.lstsq(image_positions, stage_positions) # we solve pixel_shifts*A = location_shifts
```

### Comparing `camera-stage-mapping-0.1.4/camera_stage_mapping/camera_stage_tracker.py` & `camera_stage_mapping-0.1.5/camera_stage_mapping/camera_stage_tracker.py`

 * *Files identical despite different names*

### Comparing `camera-stage-mapping-0.1.4/camera_stage_mapping/camera_with_location.py.disabled` & `camera_stage_mapping-0.1.5/camera_stage_mapping/camera_with_location.py.disabled`

 * *Files 0% similar despite different names*

```diff
@@ -360,15 +360,15 @@
                     tracker.append_point()
         finally:
             move(starting_position)
         # We then use least-squares to fit the XY part of the matrix relating pixels to distance
         # stage_positions should be the stage positions, with a zero mean.
         # image_positions also has zero mean for x and y, but is calculated from cross-correlation.
         stage_positions, image_positions = tracker.history
-        stage_positions = stage_positions.astype(np.float)
+        stage_positions = stage_positions.astype(float)
         stage_positions -= np.mean(stage_positions, axis=0)
         stage_positions = stage_positions[:,:2] # ensure it's 2d
         image_positions -= np.mean(image_positions, axis=0)
         image_positions *= -1 # To get the matrix right, we want the position of each
                             # image relative to the template, rather than the other way around
         print(f"The image, stage position arrays are {image_positions.shape},{stage_positions.shape}")
         A, res, rank, s = np.linalg.lstsq(image_positions, stage_positions) # we solve pixel_shifts*A = location_shifts
```

### Comparing `camera-stage-mapping-0.1.4/camera_stage_mapping/closed_loop_move.py` & `camera_stage_mapping-0.1.5/camera_stage_mapping/closed_loop_move.py`

 * *Files identical despite different names*

### Comparing `camera-stage-mapping-0.1.4/camera_stage_mapping/correlation_image_tracking.py` & `camera_stage_mapping-0.1.5/camera_stage_mapping/correlation_image_tracking.py`

 * *Files identical despite different names*

### Comparing `camera-stage-mapping-0.1.4/camera_stage_mapping/fft_image_tracking.py` & `camera_stage_mapping-0.1.5/camera_stage_mapping/fft_image_tracking.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     Returns:
         image, fft_shape
     """
     if len(image.shape) == 3:
         image = np.mean(image, axis=2)
     fft_shape = np.array(image.shape)
     if pad:
-        image = image.astype(np.float) - np.mean(image)
+        image = image.astype(float) - np.mean(image)
         fft_shape *= 2
     return image, fft_shape
 
 def high_pass_fourier_mask(shape, s, rfft=True):
     """Generate a mask performing a high pass filter
     
     The return value is a 2D array, which can be multiplied
@@ -48,15 +48,15 @@
         shape: tuple of 2 integers
             The shape of the output array
         s: float
             The standard deviation of the Gaussian in real
             space, in pixels
     """
     high_pass_filter = np.ones(shape)
-    x, y = (np.arange(n, dtype=np.float) for n in shape)
+    x, y = (np.arange(n, dtype=float) for n in shape)
     # Beyond the halfway point of the array, frequencies are negative
     x[x.shape[0]//2:x.shape[0]] -= x.shape[0]
     if not rfft: # If it's a real fft, the last axis is halved so we can skip this.
         y[y.shape[0]//2:y.shape[0]] -= y.shape[0]
     x /= np.max(np.abs(x)) * 2  # Normalise so highest frequency is 1/2
     y /= np.max(np.abs(y)) * 2  # Normalise so highest frequency is 1/2
     r2 = x[:, np.newaxis]**2 + y[np.newaxis, :]**2
@@ -106,15 +106,15 @@
             Set this to true if we are working on the output of
             a Fourier transform.  This will adjust the coordinates
             such that we effectively perform quadrant swapping, to
             place the DC component in the centre of the image, and
             make the coordinate (0,0) correspond to that point, with
             positive and negative coordinates either side.
     """
-    assert corr.dtype == np.float, "The image must be floating point"
+    assert corr.dtype == float, "The image must be floating point"
     background = np.max(corr) - fractional_threshold * (np.max(corr) - np.min(corr))
     background_subtracted = corr - background
     background_subtracted[background_subtracted < 0] = 0
     xs, ys = (np.arange(n) for n in corr.shape) # This is equivalent to meshgrid, more or less...
     if quadrant_swap:
         xs[len(xs)//2:] -= len(xs)
         ys[len(ys)//2:] -= len(ys)
```

### Comparing `camera-stage-mapping-0.1.4/camera_stage_mapping/ofm_extension.py` & `camera_stage_mapping-0.1.5/camera_stage_mapping/ofm_extension.py`

 * *Files identical despite different names*

### Comparing `camera-stage-mapping-0.1.4/camera_stage_mapping/scan_coords_times.py` & `camera_stage_mapping-0.1.5/camera_stage_mapping/scan_coords_times.py`

 * *Files identical despite different names*

### Comparing `camera-stage-mapping-0.1.4/pyproject.toml` & `camera_stage_mapping-0.1.5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
 
 [tool.poetry]
 name = "camera-stage-mapping"
-version = "0.1.4"
+version = "0.1.5"
 license = "LGPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://gitlab.com/openflexure/microscope-extensions/camera-stage-mapping/"
 description = "Calibration and mapping between stage and camera coordinates in a microscope"
 authors = ["Richard Bowman <richard.bowman@cantab.net>"]
 
 [tool.poetry.dependencies]
-python = "^3.6"
-numpy = "^1.17"
+python = "^3.9"
+numpy = "^1.20"
 opencv-python-headless = {version = "^4.1", optional = true} # This is critical for Raspberry Pi.  Could remove entirely with a direct crosscorrelation function...
 scipy = {version = "^1.4", optional = true}
 
 [tool.poetry.dev-dependencies]
-pytest = "^5.4"
-openflexure-microscope-client = {version = "0.1.2", optional = true}
-ipykernel = {version = "^5.2", optional = true}
+pytest = "^7.4"
+openflexure-microscope-client = {version = ">=0.1.8", optional = true}
+ipykernel = {version = ">=5.2", optional = true}
 matplotlib = {version = "^3.2", optional = true}
-sphinx = "^3.1"
-sphinx-rtd-theme = "0.5.0"
-sphinx-autoapi = {version = "^1.4.0"}
+sphinx = "^6.0" # rtd-theme may have issues with sphinx 7
+sphinx-rtd-theme = "^1.0"
+sphinx-autoapi = {version = "^2.1"}
 
 [tool.poetry.extras]
 correlation = ["opencv-python-headless", "scipy"]
 ofmclient = ["openflexure-microscope-client"]
 ipython = ["ipykernel", "matplotlib"]
 all = ["opencv-python-headless", "scipy", "openflexure-microscope-client", "ipykernel", "matplotlib"]
```

### Comparing `camera-stage-mapping-0.1.4/setup.py` & `camera_stage_mapping-0.1.5/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,35 +1,43 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: camera-stage-mapping
+Version: 0.1.5
+Summary: Calibration and mapping between stage and camera coordinates in a microscope
+Home-page: https://gitlab.com/openflexure/microscope-extensions/camera-stage-mapping/
+License: LGPL-3.0-or-later
+Author: Richard Bowman
+Author-email: richard.bowman@cantab.net
+Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: all
+Provides-Extra: correlation
+Provides-Extra: ipython
+Provides-Extra: ofmclient
+Requires-Dist: numpy (>=1.20,<2.0)
+Requires-Dist: opencv-python-headless (>=4.1,<5.0) ; extra == "correlation" or extra == "all"
+Requires-Dist: scipy (>=1.4,<2.0) ; extra == "correlation" or extra == "all"
+Description-Content-Type: text/markdown
+
+# Camera Stage Mapping calibration
+
+This Python module allows you to calibrate a microscope's stage against the camera.  By moving the sample a known number of steps, and tracking how far the image translates, it is possible to recover the number of steps per pixel.  This code goes a step further, and recovers a 2x2 affine transformation matrix, so it will cope with rotation, flipping, and non-uniform scaling of the X and Y axes.  The calibration routines are designed to be relatively robust and minimally parameterised, so they start by determining a sensible step size automatically.
+
+As part of the calibration, you can use either FFT-based or directly calculated cross correlation to track motion of the sample.  This code is probably useful on its own, and is found in the ``fft_image_tracking`` and ``correlation_image_tracking`` submodules.  The underlying mechanism of tracking stage and camera coordinates simultaneously is handled by the ``CameraStageTracker`` class, in ``camera_stage_tracker``.  The main calibration function is ``camera_stage_calibration_1d.calibrate_backlash_1d``.  For 2D calibration, I recommend running this once for X and once for Y, then using ``camera_stage_calibration_1d.image_to_stage_displacement_from_1d`` to combine the two calibrations.  This is more robust than the 2D grid calibration method.
+
+## Hardware interface
+Rather than tie these functions to a specific class interface, as found in many lab control frameworks, the calibration routines simply require functions to be passed in as arguments.  This is done for maximum flexibility, and to impose the fewest necessary constraints on the hardware we are controlling.  In the future, we may define a class interface to use, and would welcome input on how to do this without forcing a particular taxonomy of laboratory instruments upon everyone using the library.
+
+## Installing
+```
+pip install camera-stage-mapping
+```
+This package is published on PyPI and can be installed using ``pip``.  It's managed using ``poetry`` and can be installed by cloning the repository and running ``poetry install``.  For details of how to set up a development environment, please see [CONTRIBUTING].
 
-packages = \
-['camera_stage_mapping']
+## Documentation
+The functions all have fairly extensive docstrings and the module is documented on [readthedocs].
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['numpy>=1.17,<2.0']
-
-extras_require = \
-{'all': ['opencv-python-headless>=4.1,<5.0', 'scipy>=1.4,<2.0'],
- 'correlation': ['opencv-python-headless>=4.1,<5.0', 'scipy>=1.4,<2.0']}
-
-setup_kwargs = {
-    'name': 'camera-stage-mapping',
-    'version': '0.1.4',
-    'description': 'Calibration and mapping between stage and camera coordinates in a microscope',
-    'long_description': "# Camera Stage Mapping calibration\n\nThis Python module allows you to calibrate a microscope's stage against the camera.  By moving the sample a known number of steps, and tracking how far the image translates, it is possible to recover the number of steps per pixel.  This code goes a step further, and recovers a 2x2 affine transformation matrix, so it will cope with rotation, flipping, and non-uniform scaling of the X and Y axes.  The calibration routines are designed to be relatively robust and minimally parameterised, so they start by determining a sensible step size automatically.\n\nAs part of the calibration, you can use either FFT-based or directly calculated cross correlation to track motion of the sample.  This code is probably useful on its own, and is found in the ``fft_image_tracking`` and ``correlation_image_tracking`` submodules.  The underlying mechanism of tracking stage and camera coordinates simultaneously is handled by the ``CameraStageTracker`` class, in ``camera_stage_tracker``.  The main calibration function is ``camera_stage_calibration_1d.calibrate_backlash_1d``.  For 2D calibration, I recommend running this once for X and once for Y, then using ``camera_stage_calibration_1d.image_to_stage_displacement_from_1d`` to combine the two calibrations.  This is more robust than the 2D grid calibration method.\n\n## Hardware interface\nRather than tie these functions to a specific class interface, as found in many lab control frameworks, the calibration routines simply require functions to be passed in as arguments.  This is done for maximum flexibility, and to impose the fewest necessary constraints on the hardware we are controlling.  In the future, we may define a class interface to use, and would welcome input on how to do this without forcing a particular taxonomy of laboratory instruments upon everyone using the library.\n\n## Installing\n```\npip install camera-stage-mapping\n```\nThis package is published on PyPI and can be installed using ``pip``.  It's managed using ``poetry`` and can be installed by cloning the repository and running ``poetry install``.  For details of how to set up a development environment, please see [CONTRIBUTING].\n\n## Documentation\nThe functions all have fairly extensive docstrings and the module is documented on [readthedocs].\n\n[readthedocs]: https://camera-stage-mapping.readthedocs.io/en/latest/index.html\n[CONTRIBUTING]: ./CONTRIBUTING.md",
-    'author': 'Richard Bowman',
-    'author_email': 'richard.bowman@cantab.net',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://gitlab.com/openflexure/microscope-extensions/camera-stage-mapping/',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.6,<4.0',
-}
-
-
-setup(**setup_kwargs)
+[readthedocs]: https://camera-stage-mapping.readthedocs.io/en/latest/index.html
+[CONTRIBUTING]: ./CONTRIBUTING.md
```

