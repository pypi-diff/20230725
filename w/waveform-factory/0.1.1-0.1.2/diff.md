# Comparing `tmp/waveform_factory-0.1.1.tar.gz` & `tmp/waveform_factory-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waveform_factory-0.1.1.tar", last modified: Mon Jul 24 21:48:25 2023, max compression
+gzip compressed data, was "waveform_factory-0.1.2.tar", last modified: Mon Jul 24 22:36:35 2023, max compression
```

## Comparing `waveform_factory-0.1.1.tar` & `waveform_factory-0.1.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 paulbennett   (501) staff       (20)        0 2023-07-24 21:48:25.607610 waveform_factory-0.1.1/
--rw-r--r--   0 paulbennett   (501) staff       (20)     1069 2023-07-24 19:12:11.000000 waveform_factory-0.1.1/LICENSE
--rw-r--r--   0 paulbennett   (501) staff       (20)      264 2023-07-24 21:48:25.607453 waveform_factory-0.1.1/PKG-INFO
--rw-r--r--   0 paulbennett   (501) staff       (20)      696 2023-07-24 19:12:11.000000 waveform_factory-0.1.1/README.md
--rw-r--r--   0 paulbennett   (501) staff       (20)       38 2023-07-24 21:48:25.607651 waveform_factory-0.1.1/setup.cfg
--rw-r--r--   0 paulbennett   (501) staff       (20)      717 2023-07-24 21:48:14.000000 waveform_factory-0.1.1/setup.py
-drwxr-xr-x   0 paulbennett   (501) staff       (20)        0 2023-07-24 21:48:25.603199 waveform_factory-0.1.1/tests/
--rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform_factory-0.1.1/tests/__init__.py
-drwxr-xr-x   0 paulbennett   (501) staff       (20)        0 2023-07-24 21:48:25.604864 waveform_factory-0.1.1/tests/patterns/
--rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform_factory-0.1.1/tests/patterns/__init__.py
--rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform_factory-0.1.1/tests/patterns/test_arches.py
--rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform_factory-0.1.1/tests/patterns/test_autoregressive.py
--rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform_factory-0.1.1/tests/patterns/test_cosine.py
--rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform_factory-0.1.1/tests/patterns/test_decay.py
--rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform_factory-0.1.1/tests/patterns/test_exponential.py
--rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform_factory-0.1.1/tests/patterns/test_gaussian_noise.py
--rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform_factory-0.1.1/tests/patterns/test_morlet.py
--rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform_factory-0.1.1/tests/patterns/test_rate.py
--rw-r--r--   0 paulbennett   (501) staff       (20)     4786 2023-07-24 21:46:24.000000 waveform_factory-0.1.1/tests/patterns/test_sawtooth.py
--rw-r--r--   0 paulbennett   (501) staff       (20)     4122 2023-07-24 21:46:24.000000 waveform_factory-0.1.1/tests/patterns/test_sine.py
--rw-r--r--   0 paulbennett   (501) staff       (20)     3111 2023-07-24 21:46:24.000000 waveform_factory-0.1.1/tests/patterns/test_square.py
--rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform_factory-0.1.1/tests/patterns/test_step.py
--rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform_factory-0.1.1/tests/patterns/test_triangle.py
--rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform_factory-0.1.1/tests/test_pattern_generator.py
-drwxr-xr-x   0 paulbennett   (501) staff       (20)        0 2023-07-24 21:48:25.605044 waveform_factory-0.1.1/waveform_factory/
--rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-24 21:46:11.000000 waveform_factory-0.1.1/waveform_factory/__init__.py
--rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform_factory-0.1.1/waveform_factory/pattern_generator.py
-drwxr-xr-x   0 paulbennett   (501) staff       (20)        0 2023-07-24 21:48:25.607124 waveform_factory-0.1.1/waveform_factory/patterns/
--rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform_factory-0.1.1/waveform_factory/patterns/__init__.py
--rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform_factory-0.1.1/waveform_factory/patterns/arches.py
--rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform_factory-0.1.1/waveform_factory/patterns/autoregressive.py
--rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform_factory-0.1.1/waveform_factory/patterns/cosine.py
--rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform_factory-0.1.1/waveform_factory/patterns/decay.py
--rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform_factory-0.1.1/waveform_factory/patterns/exponential.py
--rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform_factory-0.1.1/waveform_factory/patterns/gaussian_noise.py
--rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform_factory-0.1.1/waveform_factory/patterns/morlet.py
--rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform_factory-0.1.1/waveform_factory/patterns/rate.py
--rw-r--r--   0 paulbennett   (501) staff       (20)     1387 2023-07-13 16:23:36.000000 waveform_factory-0.1.1/waveform_factory/patterns/sawtooth.py
--rw-r--r--   0 paulbennett   (501) staff       (20)     1073 2023-07-13 16:28:42.000000 waveform_factory-0.1.1/waveform_factory/patterns/sine.py
--rw-r--r--   0 paulbennett   (501) staff       (20)     1186 2023-07-24 19:34:39.000000 waveform_factory-0.1.1/waveform_factory/patterns/square.py
--rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform_factory-0.1.1/waveform_factory/patterns/step.py
--rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform_factory-0.1.1/waveform_factory/patterns/triangle.py
-drwxr-xr-x   0 paulbennett   (501) staff       (20)        0 2023-07-24 21:48:25.607297 waveform_factory-0.1.1/waveform_factory/utils/
--rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform_factory-0.1.1/waveform_factory/utils/__init__.py
--rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform_factory-0.1.1/waveform_factory/utils/helpers.py
-drwxr-xr-x   0 paulbennett   (501) staff       (20)        0 2023-07-24 21:48:25.605564 waveform_factory-0.1.1/waveform_factory.egg-info/
--rw-r--r--   0 paulbennett   (501) staff       (20)      264 2023-07-24 21:48:25.000000 waveform_factory-0.1.1/waveform_factory.egg-info/PKG-INFO
--rw-r--r--   0 paulbennett   (501) staff       (20)     1370 2023-07-24 21:48:25.000000 waveform_factory-0.1.1/waveform_factory.egg-info/SOURCES.txt
--rw-r--r--   0 paulbennett   (501) staff       (20)        1 2023-07-24 21:48:25.000000 waveform_factory-0.1.1/waveform_factory.egg-info/dependency_links.txt
--rw-r--r--   0 paulbennett   (501) staff       (20)       17 2023-07-24 21:48:25.000000 waveform_factory-0.1.1/waveform_factory.egg-info/requires.txt
--rw-r--r--   0 paulbennett   (501) staff       (20)       17 2023-07-24 21:48:25.000000 waveform_factory-0.1.1/waveform_factory.egg-info/top_level.txt
+drwxr-xr-x   0 paulbennett   (501) staff       (20)        0 2023-07-24 22:36:35.768289 waveform_factory-0.1.2/
+-rw-r--r--   0 paulbennett   (501) staff       (20)     1069 2023-07-24 22:13:23.000000 waveform_factory-0.1.2/LICENSE
+-rw-r--r--   0 paulbennett   (501) staff       (20)      498 2023-07-24 22:36:35.768173 waveform_factory-0.1.2/PKG-INFO
+-rw-r--r--   0 paulbennett   (501) staff       (20)      760 2023-07-24 22:32:47.000000 waveform_factory-0.1.2/README.md
+-rw-r--r--   0 paulbennett   (501) staff       (20)       38 2023-07-24 22:36:35.768326 waveform_factory-0.1.2/setup.cfg
+-rw-r--r--   0 paulbennett   (501) staff       (20)      753 2023-07-24 22:36:17.000000 waveform_factory-0.1.2/setup.py
+drwxr-xr-x   0 paulbennett   (501) staff       (20)        0 2023-07-24 22:36:35.763958 waveform_factory-0.1.2/tests/
+-rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform_factory-0.1.2/tests/__init__.py
+drwxr-xr-x   0 paulbennett   (501) staff       (20)        0 2023-07-24 22:36:35.765866 waveform_factory-0.1.2/tests/patterns/
+-rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform_factory-0.1.2/tests/patterns/__init__.py
+-rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform_factory-0.1.2/tests/patterns/test_arches.py
+-rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform_factory-0.1.2/tests/patterns/test_autoregressive.py
+-rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform_factory-0.1.2/tests/patterns/test_cosine.py
+-rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform_factory-0.1.2/tests/patterns/test_decay.py
+-rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform_factory-0.1.2/tests/patterns/test_exponential.py
+-rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform_factory-0.1.2/tests/patterns/test_gaussian_noise.py
+-rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform_factory-0.1.2/tests/patterns/test_morlet.py
+-rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform_factory-0.1.2/tests/patterns/test_rate.py
+-rw-r--r--   0 paulbennett   (501) staff       (20)     4786 2023-07-24 22:32:47.000000 waveform_factory-0.1.2/tests/patterns/test_sawtooth.py
+-rw-r--r--   0 paulbennett   (501) staff       (20)     4122 2023-07-24 22:32:47.000000 waveform_factory-0.1.2/tests/patterns/test_sine.py
+-rw-r--r--   0 paulbennett   (501) staff       (20)     3111 2023-07-24 22:34:15.000000 waveform_factory-0.1.2/tests/patterns/test_square.py
+-rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform_factory-0.1.2/tests/patterns/test_step.py
+-rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform_factory-0.1.2/tests/patterns/test_triangle.py
+-rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-13 15:37:49.000000 waveform_factory-0.1.2/tests/test_pattern_generator.py
+drwxr-xr-x   0 paulbennett   (501) staff       (20)        0 2023-07-24 22:36:35.766041 waveform_factory-0.1.2/waveform_factory/
+-rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-24 22:32:47.000000 waveform_factory-0.1.2/waveform_factory/__init__.py
+-rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-24 22:32:47.000000 waveform_factory-0.1.2/waveform_factory/pattern_generator.py
+drwxr-xr-x   0 paulbennett   (501) staff       (20)        0 2023-07-24 22:36:35.767869 waveform_factory-0.1.2/waveform_factory/patterns/
+-rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-24 22:32:47.000000 waveform_factory-0.1.2/waveform_factory/patterns/__init__.py
+-rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-24 22:32:47.000000 waveform_factory-0.1.2/waveform_factory/patterns/arches.py
+-rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-24 22:32:47.000000 waveform_factory-0.1.2/waveform_factory/patterns/autoregressive.py
+-rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-24 22:32:47.000000 waveform_factory-0.1.2/waveform_factory/patterns/cosine.py
+-rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-24 22:32:47.000000 waveform_factory-0.1.2/waveform_factory/patterns/decay.py
+-rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-24 22:32:47.000000 waveform_factory-0.1.2/waveform_factory/patterns/exponential.py
+-rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-24 22:32:47.000000 waveform_factory-0.1.2/waveform_factory/patterns/gaussian_noise.py
+-rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-24 22:32:47.000000 waveform_factory-0.1.2/waveform_factory/patterns/morlet.py
+-rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-24 22:32:47.000000 waveform_factory-0.1.2/waveform_factory/patterns/rate.py
+-rw-r--r--   0 paulbennett   (501) staff       (20)     1387 2023-07-24 22:32:47.000000 waveform_factory-0.1.2/waveform_factory/patterns/sawtooth.py
+-rw-r--r--   0 paulbennett   (501) staff       (20)     1073 2023-07-24 22:32:47.000000 waveform_factory-0.1.2/waveform_factory/patterns/sine.py
+-rw-r--r--   0 paulbennett   (501) staff       (20)     1190 2023-07-24 22:32:47.000000 waveform_factory-0.1.2/waveform_factory/patterns/square.py
+-rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-24 22:32:47.000000 waveform_factory-0.1.2/waveform_factory/patterns/step.py
+-rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-24 22:32:47.000000 waveform_factory-0.1.2/waveform_factory/patterns/triangle.py
+drwxr-xr-x   0 paulbennett   (501) staff       (20)        0 2023-07-24 22:36:35.768032 waveform_factory-0.1.2/waveform_factory/utils/
+-rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-24 22:32:47.000000 waveform_factory-0.1.2/waveform_factory/utils/__init__.py
+-rw-r--r--   0 paulbennett   (501) staff       (20)        0 2023-07-24 22:32:47.000000 waveform_factory-0.1.2/waveform_factory/utils/helpers.py
+drwxr-xr-x   0 paulbennett   (501) staff       (20)        0 2023-07-24 22:36:35.766568 waveform_factory-0.1.2/waveform_factory.egg-info/
+-rw-r--r--   0 paulbennett   (501) staff       (20)      498 2023-07-24 22:36:35.000000 waveform_factory-0.1.2/waveform_factory.egg-info/PKG-INFO
+-rw-r--r--   0 paulbennett   (501) staff       (20)     1370 2023-07-24 22:36:35.000000 waveform_factory-0.1.2/waveform_factory.egg-info/SOURCES.txt
+-rw-r--r--   0 paulbennett   (501) staff       (20)        1 2023-07-24 22:36:35.000000 waveform_factory-0.1.2/waveform_factory.egg-info/dependency_links.txt
+-rw-r--r--   0 paulbennett   (501) staff       (20)       46 2023-07-24 22:36:35.000000 waveform_factory-0.1.2/waveform_factory.egg-info/requires.txt
+-rw-r--r--   0 paulbennett   (501) staff       (20)       17 2023-07-24 22:36:35.000000 waveform_factory-0.1.2/waveform_factory.egg-info/top_level.txt
```

### Comparing `waveform_factory-0.1.1/LICENSE` & `waveform_factory-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `waveform_factory-0.1.1/README.md` & `waveform_factory-0.1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -12,7 +12,9 @@
 
 ## Installation
 
 To install Waveform Factory, you can use pip:
 
 ```bash
 pip install waveformfactory
+```
+![PyPI](https://img.shields.io/pypi/v/waveform-factory.svg)
```

### Comparing `waveform_factory-0.1.1/setup.py` & `waveform_factory-0.1.2/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from setuptools import setup, find_packages
 
+with open('requirements.txt') as f:
+    required = f.read().splitlines()
+
 setup(
     name='waveform_factory',
-    version='0.1.1',
+    version='0.1.2',
     url='https://github.com/MrB-Can/waveform-factory',
     author='Paul Bennett',
     author_email='paul@lgis.ca',
     description='Wave form data generator',
-    lonmg_description='Waveform Factory is a python library that generates various types of waveform patterns. It is '
+    long_description='Waveform Factory is a python library that generates various types of waveform patterns. It is '
                 'designed to aid in the creation, manipulation, and analysis of waveform data for various '
                 'applications including music, signal processing, and more.',
     packages=find_packages(include=['waveform_factory', 'waveform_factory.*']),
-    install_requires=[
-        'numpy',
-        'matplotlib',
-    ],
+    install_requires=required,
 )
+
```

### Comparing `waveform_factory-0.1.1/tests/patterns/test_sawtooth.py` & `waveform_factory-0.1.2/tests/patterns/test_sawtooth.py`

 * *Files identical despite different names*

### Comparing `waveform_factory-0.1.1/tests/patterns/test_sine.py` & `waveform_factory-0.1.2/tests/patterns/test_sine.py`

 * *Files identical despite different names*

### Comparing `waveform_factory-0.1.1/tests/patterns/test_square.py` & `waveform_factory-0.1.2/tests/patterns/test_square.py`

 * *Files identical despite different names*

### Comparing `waveform_factory-0.1.1/waveform_factory/patterns/sawtooth.py` & `waveform_factory-0.1.2/waveform_factory/patterns/sawtooth.py`

 * *Files identical despite different names*

### Comparing `waveform_factory-0.1.1/waveform_factory/patterns/sine.py` & `waveform_factory-0.1.2/waveform_factory/patterns/sine.py`

 * *Files identical despite different names*

### Comparing `waveform_factory-0.1.1/waveform_factory/patterns/square.py` & `waveform_factory-0.1.2/waveform_factory/patterns/square.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import numpy as np
-from scipy.signal import square
+from scipy.signal import square as sqr
 
 
 def generate_square_wave(frequency: float, amplitude: float, length: float, sample_rate: int = 44100,
                          phase_shift: float = 0.0, offset: float = 0.0, invert: bool = False) -> np.ndarray:
     """
     Generates a square wave.
 
@@ -14,15 +14,15 @@
     :param phase_shift: The phase shift of the square wave in radians. Default is 0.0.
     :param offset: The DC offset of the square wave. Default is 0.0.
     :param invert: A boolean indicating whether the square wave should be inverted or not. Default is False.
     :return: A numpy array representing the generated square wave.
     """
 
     t = np.linspace(0, length, int(sample_rate * length), False)  # time variable
-    waveform = square(2 * np.pi * frequency * t + phase_shift)
+    waveform = sqr(2 * np.pi * frequency * t + phase_shift)
 
     if invert:
         waveform *= -1
 
     waveform = amplitude * waveform + offset
 
     return waveform
```

### Comparing `waveform_factory-0.1.1/waveform_factory.egg-info/SOURCES.txt` & `waveform_factory-0.1.2/waveform_factory.egg-info/SOURCES.txt`

 * *Files identical despite different names*

