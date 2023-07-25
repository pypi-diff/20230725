# Comparing `tmp/opensr-test-0.0.2.tar.gz` & `tmp/opensr-test-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opensr-test-0.0.2.tar", last modified: Thu Jul 13 09:46:17 2023, max compression
+gzip compressed data, was "opensr-test-0.0.3.tar", last modified: Tue Jul 25 11:42:40 2023, max compression
```

## Comparing `opensr-test-0.0.2.tar` & `opensr-test-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 csaybar   (1000) csaybar   (1000)        0 2023-07-13 09:46:17.397294 opensr-test-0.0.2/
--rw-rw-r--   0 csaybar   (1000) csaybar   (1000)     1077 2023-07-12 18:42:54.000000 opensr-test-0.0.2/LICENSE
--rw-rw-r--   0 csaybar   (1000) csaybar   (1000)    14757 2023-07-13 09:46:17.397294 opensr-test-0.0.2/PKG-INFO
--rw-rw-r--   0 csaybar   (1000) csaybar   (1000)    14135 2023-07-12 19:05:04.000000 opensr-test-0.0.2/README.md
-drwxrwxr-x   0 csaybar   (1000) csaybar   (1000)        0 2023-07-13 09:46:17.397294 opensr-test-0.0.2/opensr_test.egg-info/
--rw-rw-r--   0 csaybar   (1000) csaybar   (1000)    14757 2023-07-13 09:46:17.000000 opensr-test-0.0.2/opensr_test.egg-info/PKG-INFO
--rw-rw-r--   0 csaybar   (1000) csaybar   (1000)      200 2023-07-13 09:46:17.000000 opensr-test-0.0.2/opensr_test.egg-info/SOURCES.txt
--rw-rw-r--   0 csaybar   (1000) csaybar   (1000)        1 2023-07-13 09:46:17.000000 opensr-test-0.0.2/opensr_test.egg-info/dependency_links.txt
--rw-rw-r--   0 csaybar   (1000) csaybar   (1000)       61 2023-07-13 09:46:17.000000 opensr-test-0.0.2/opensr_test.egg-info/requires.txt
--rw-rw-r--   0 csaybar   (1000) csaybar   (1000)        1 2023-07-13 09:46:17.000000 opensr-test-0.0.2/opensr_test.egg-info/top_level.txt
--rw-rw-r--   0 csaybar   (1000) csaybar   (1000)       38 2023-07-13 09:46:17.397294 opensr-test-0.0.2/setup.cfg
--rw-rw-r--   0 csaybar   (1000) csaybar   (1000)     1295 2023-07-13 09:46:07.000000 opensr-test-0.0.2/setup.py
+drwxrwxr-x   0 csaybar   (1000) csaybar   (1000)        0 2023-07-25 11:42:40.057461 opensr-test-0.0.3/
+-rw-rw-r--   0 csaybar   (1000) csaybar   (1000)     1077 2023-07-12 18:42:54.000000 opensr-test-0.0.3/LICENSE
+-rw-rw-r--   0 csaybar   (1000) csaybar   (1000)    16839 2023-07-25 11:42:40.057461 opensr-test-0.0.3/PKG-INFO
+-rw-rw-r--   0 csaybar   (1000) csaybar   (1000)    16168 2023-07-21 06:35:39.000000 opensr-test-0.0.3/README.md
+drwxrwxr-x   0 csaybar   (1000) csaybar   (1000)        0 2023-07-25 11:42:40.057461 opensr-test-0.0.3/opensr_test.egg-info/
+-rw-rw-r--   0 csaybar   (1000) csaybar   (1000)    16839 2023-07-25 11:42:39.000000 opensr-test-0.0.3/opensr_test.egg-info/PKG-INFO
+-rw-rw-r--   0 csaybar   (1000) csaybar   (1000)      200 2023-07-25 11:42:40.000000 opensr-test-0.0.3/opensr_test.egg-info/SOURCES.txt
+-rw-rw-r--   0 csaybar   (1000) csaybar   (1000)        1 2023-07-25 11:42:39.000000 opensr-test-0.0.3/opensr_test.egg-info/dependency_links.txt
+-rw-rw-r--   0 csaybar   (1000) csaybar   (1000)       30 2023-07-25 11:42:39.000000 opensr-test-0.0.3/opensr_test.egg-info/requires.txt
+-rw-rw-r--   0 csaybar   (1000) csaybar   (1000)        1 2023-07-25 11:42:39.000000 opensr-test-0.0.3/opensr_test.egg-info/top_level.txt
+-rw-rw-r--   0 csaybar   (1000) csaybar   (1000)       38 2023-07-25 11:42:40.057461 opensr-test-0.0.3/setup.cfg
+-rw-rw-r--   0 csaybar   (1000) csaybar   (1000)     1270 2023-07-25 11:42:30.000000 opensr-test-0.0.3/setup.py
```

### Comparing `opensr-test-0.0.2/LICENSE` & `opensr-test-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `opensr-test-0.0.2/PKG-INFO` & `opensr-test-0.0.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,28 @@
-Metadata-Version: 2.1
-Name: opensr-test
-Version: 0.0.2
-Summary: A comprehensive benchmark for real-world Sentinel-2 imagery super-resolution
-Home-page: https://github.com/ESAOpenSR/opensr-test
-Author: Cesar Aybar Camacho
-Author-email: csaybar@gmail.com
-License: MIT
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <p align="center">
-  <a href="https://github.com/ESAOpenSR/opensr-test"><img src="https://user-images.githubusercontent.com/16768318/213960001-66bb7d18-13d8-41d4-9de3-1e8a77f73787.png" alt="header" width="55%"></a>
-</p>[Title](https://github.com/ESAOpenSR/opensr-check)
+  <a href="https://github.com/ESAOpenSR/opensr-test"><img src="https://github.com/ESAOpenSR/opensr-test/assets/16768318/15661226-f4c4-4d55-8dd1-d73a228e36da" alt="header" width="55%"></a>
+</p>
+
+
+
 
 <p align="center">
     <em>A comprehensive benchmark for real-world Sentinel-2 imagery super-resolution</em>
 </p>
 
 <p align="center">
 <a href='https://pypi.python.org/pypi/opensr-test'>
     <img src='https://img.shields.io/pypi/v/opensr-test.svg' alt='PyPI' />
 </a>
 
 <a href="https://opensource.org/licenses/MIT" target="_blank">
     <img src="https://img.shields.io/badge/License-MIT-blue.svg" alt="License">
 </a>
-<a href='https://opensr-test.readthedocs.io/en/latest/?badge=latest'>
-    <img src='https://readthedocs.org/projects/opensr-test/badge/?version=latest' alt='Documentation Status' />
+<a href='https://opensr-test.readthedocs.io/en/latest/?badge=main'>
+    <img src='https://readthedocs.org/projects/opensr-test/badge/?version=main' alt='Documentation Status' />
 </a>
 <a href="https://github.com/psf/black" target="_blank">
     <img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="Black">
 </a>
 <a href="https://pycqa.github.io/isort/" target="_blank">
     <img src="https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336" alt="isort">
 </a>
@@ -52,80 +38,115 @@
 
 **Paper**: Coming soon!
 
 ---
 
 ## Overview
 
-In remote sensing, image super-resolution (ISR) is a technique used to create high-resolution (HR) images from low-resolution (R) satellite images, giving a more detailed view of the Earth's surface. However, with the constant development and introduction of new ISR algorithms, it can be challenging to stay updated on the latest advancements and to evaluate their performance objectively. To address this issue, we introduce SRcheck, a Python package that provides an easy-to-use interface for comparing and benchmarking various ISR methods. SRcheck includes a range of datasets that consist of high-resolution and low-resolution image pairs, as well as a set of quantitative metrics for evaluating the performance of SISR algorithms.
+In the domain of remote sensing, image super-resolution (ISR) goal is augmenting the ground sampling distance, also known as spatial resolution. Over recent years, numerous research papers have been proposed addressing ISR; however, they invariably suffer from two main issues. Firstly, the majority of these proposed models are tested on synthetic data. As a result, their applicability and performance in real-world scenarios remain unverified. Secondly, the frequently utilized evaluation metrics for these models, such as LPIPS and SSIM, are inherently designed for perceptual image analysis, not specifically for super-resolution.
+
+In response to these challenges, **'opensr-test'** has been introduced as a Python package, designed to provide users with three meticulously curated test datasets. These datasets are tailored to minimize spatial distortions between Low Resolution (LR) and High Resolution (HR) images, while calibrating differences in the spectral domain. Moreover, the **'opensr-test'** package offers five distinct types of metrics aimed at accurately evaluating the performance of ISR algorithms, thus addressing the aforementioned shortcomings of conventional evaluation techniques.
+
+## Datasets
+
+The utilization of *synthetic data* in benchmarking could potentially introduce biased conclusions, as there are no guarantees that a degradation method could not inadvertently incorporate some form of bias, i.e. the degradation does not match the real-world ground sampling distance of the LR image. Therefore, to avoid *synthetic data* potential errors, the datasets utilized in **opensr-test** are meticulously created following a *cross-sensor approach* that means that HR and LR comes from different sensor but they are aligned as closely as possible, i.e. harmonized. Due to the limited availability of open HR resolution data that correspond with Sentinel-2, we propose using three HR sensors: SPOT, VENµS, and NAIP.
+
+
+| Dataset        | Scale | # Scenes | HRsize | HR Reference                                                                               |
+|----------------|-------|----------|--------|--------------------------------------------------------------------------------------------|
+| NAIP-19        | x4    | 200      | 512    | USDA Farm Production and Conservation - Business Center, Geospatial Enterprise Operations. |
+| SPOTPAN-10     | x4    | 200      | 512    | European Space Agency, 2017, SPOT 1-5 ESA                                                  |
+| Mini-SEN2VENµS | x2    | 200      | 512    | Vegetation and Environment monitoring on a New Micro-Satellite (SEN2VENμS).                |
+
+
+
+
+## Metrics
+
+We propose that evaluating the ISR process with a single metric is not adequate, and therefore, we suggest the use of five metrics, which will be detailed below.
+
+<details>
+    <summary><b>Spectral consistency</b></summary>
+    Measured based on the comparison of LR and SR images. The reflectance values are then compared using spectral angle distance metrics. The LR and degraded SR values should not be identical but rather similar.
+</details>
+
+<details>
+    <summary><b>Spatial consistency</b></summary>
+    Measured again from the comparison of the LR and SR images, ground control points are obtained using LightGlue + DISK. The difference between the reference points and a first-order polynomial is then calculated.
+</details>
+
+<details>
+    <summary><b>High-frequency</b></summary>
+    Measured from the comparison of LR and SR images, we calculate the MTF between the LR-SR pairs to assess the improvement in ground sampling distance. The MTF curve represents the system's response in different spatial frequencies. A higher MTF value at a specific frequency indicates a better resolution and sharper image details. The reported metric is the comparison of the area under the MTF curve between the LR and SR images, from the Nyquist frequency of Sentinel2 to the super-resolved image.
+</details>
+
+<details>
+    <summary><b>Omission</b></summary>
+    Error related to the inability to represent the actual high-frequency information from the landscape. The systematic error must be first removed.
+</details>
+
+<details>
+    <summary><b>Hallucinations</b></summary>
+    Hallucinations refer to errors that are solely related to high-frequency information inducted by the super-resolution model, with no correlation to the real continuous space. 
+</details>
+
+
+<img src="https://github.com/ESAOpenSR/opensr-test/assets/16768318/473865e5-5661-4b6a-b941-ae170ffd6d0e" alt="isort"  width="55%">
+
 
 ## Installation
 
 Install the latest version from PyPI:
 
 ```
-pip install srcheck
+pip install opensr-test
 ```
 
-Upgrade `srcheck` by running:
+Upgrade `opensr-test` by running:
 
 ```
-pip install -U srcheck
+pip install -U opensr-test
 ```
 
 Install the latest version from conda-forge:
 
 ```
-conda install -c conda-forge srcheck
+conda install -c conda-forge opensr-test
 ```
 
 Install the latest dev version from GitHub by running:
 
 ```
-pip install git+https://github.com/csaybar/srcheck
+pip install git+https://github.com/ESAOpenSR/opensr-test
 ```
 
 ## How does it work?
 
+opensr-test needs either a PyTorch (torch.nn.Module, torch.jit.trace or  torch.jit.script) or TensorFlow model. The following example shows 
+how to run the benchmarks:
+
 <center>
-    <img src="https://user-images.githubusercontent.com/16768318/213967913-3c665d59-5053-43a7-a450-859b7442b345.png" alt="header" width="70%">
+    <img src="https://github.com/ESAOpenSR/opensr-test/assets/16768318/60a34d0a-f7ab-4c52-b68c-978e51898733" alt="header" width="70%">
 </center>
 
-**srcheck** needs either a `torch.nn.Module` class or a compiled model via `torch.jit.trace` or `torch.jit.script`. The following example shows how to run the benchmarks:
+The following example shows how to run the benchmarks:
 
 ```python
 import torch
-import srcheck
+import opensr_test
 
+# Load your model
 model = torch.jit.load('/content/quantSRmodel.pt', map_location='cpu')
-srcheck.benchmark(model, dataset='SPOT-50', metrics=['PSNR', 'SSIM'], type= "NoSRI")
-```
-
-srcheck supports two group types of metrics: (a) Surface Reflectance Integrity (SRI) and (b) No Surface Reflectance Integrity (NoSRI). This difference is due to the fact that depending on the application, developers will be interested in optimizing the "image quality" or the "image fidelity". *Image fidelity* refers to how closely the LR image represents the real source distribution (HR). Optimizing fidelity is crucial for applications that require preserving surface reflectance as close as possible to the original values. On the other hand, *image quality* refers to how pleasant the image is for the human eye. Optimizing image quality is important for creating HR image satellite base maps. The image below shows the natural trade-off that exists between these two group types of metrics.
 
+# Check if the model works
+dataset = opensr_test.naip
 
-<center>
-    <img src="https://user-images.githubusercontent.com/16768318/213970463-5c2a8012-4e76-48ce-bb13-4d51590d359c.png" alt="header" width="60%">
-</center>
-
-But what happens if my ISR algorithm increases the image by a factor of 8, but the datasets available in srcheck do not support 8X? In that case, *srcheck* will automatically convert the results to the native resolution of the datasets. For example, if your algorithm increases the image by 2X, and you want to test it on SPOT-50 whose images are 10m in LR and 6m in HR, *srcheck* will upscale the results from 5 meters to 6m using the bilinear interpolation algorithm. Similarly, in the MUS2-50 dataset, *srcheck* will downscale the results from 5m to 2m. This is done in order the results can be compared with the datasets available.
-
-<center>
-    <img src="https://user-images.githubusercontent.com/16768318/213971771-04b193e7-83e8-436a-b4a1-0c317cc7b756.png" alt="header" width="75%">
-</center>
-
-## Datasets
-
-[**https://zenodo.org/record/7562334**](https://zenodo.org/record/7562334)
-
-More datasets are coming soon!
-
-## Metrics
-
-Metrics documentation is coming soon!
+opensr_test.check(model, dataset)
+# { 'Spectral': 0.08, 'Spatial': 2.34, 'High-frequency': 1.32, 'Hallucination': 0.90, 'Omission': 1.03}
+```
 
 ## Pre-trained Models
 Pre-trained models are available at various scales and hosted at the awesome [`huggingface_hub`](https://huggingface.co/models?filter=super-image). By default the models were pretrained on [DIV2K](https://huggingface.co/datasets/eugenesiow/Div2k), a dataset of 800 high-quality (2K resolution) images for training, augmented to 4000 images and uses a dev set of 100 validation images (images numbered 801 to 900). 
 
 The leaderboard below shows the 
 [PSNR](https://en.wikipedia.org/wiki/Peak_signal-to-noise_ratio#Quality_estimation_with_PSNR) / [SSIM](https://en.wikipedia.org/wiki/Structural_similarity#Algorithm) 
 metrics for each model at various scales on various test sets ([Set5](https://huggingface.co/datasets/eugenesiow/Set5),
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,70 +1,81 @@
-Metadata-Version: 2.1 Name: opensr-test Version: 0.0.2 Summary: A comprehensive
-benchmark for real-world Sentinel-2 imagery super-resolution Home-page: https:/
-/github.com/ESAOpenSR/opensr-test Author: Cesar Aybar Camacho Author-email:
-csaybar@gmail.com License: MIT Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: License :: OSI Approved :: MIT License Classifier: Programming
-Language :: Python Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Description-Content-Type: text/markdown License-File:
-LICENSE
                                    [header]
-[Title](https://github.com/ESAOpenSR/opensr-check)
  A comprehensive benchmark for real-world Sentinel-2 imagery super-resolution
             [PyPI] [License] [Documentation_Status] [Black] [isort]
 --- **GitHub**: [https://github.com/ESAOpenSR/opensr-test](https://github.com/
 ESAOpenSR/opensr-test) **Documentation**: [https://opensr-test.readthedocs.io/]
 (https://opensr-test.readthedocs.io/) **PyPI**: [https://pypi.org/project/
 opensr-test/](https://pypi.org/project/opensr-test/) **Paper**: Coming soon! --
-- ## Overview In remote sensing, image super-resolution (ISR) is a technique
-used to create high-resolution (HR) images from low-resolution (R) satellite
-images, giving a more detailed view of the Earth's surface. However, with the
-constant development and introduction of new ISR algorithms, it can be
-challenging to stay updated on the latest advancements and to evaluate their
-performance objectively. To address this issue, we introduce SRcheck, a Python
-package that provides an easy-to-use interface for comparing and benchmarking
-various ISR methods. SRcheck includes a range of datasets that consist of high-
-resolution and low-resolution image pairs, as well as a set of quantitative
-metrics for evaluating the performance of SISR algorithms. ## Installation
-Install the latest version from PyPI: ``` pip install srcheck ``` Upgrade
-`srcheck` by running: ``` pip install -U srcheck ``` Install the latest version
-from conda-forge: ``` conda install -c conda-forge srcheck ``` Install the
-latest dev version from GitHub by running: ``` pip install git+https://
-github.com/csaybar/srcheck ``` ## How does it work?
+- ## Overview In the domain of remote sensing, image super-resolution (ISR)
+goal is augmenting the ground sampling distance, also known as spatial
+resolution. Over recent years, numerous research papers have been proposed
+addressing ISR; however, they invariably suffer from two main issues. Firstly,
+the majority of these proposed models are tested on synthetic data. As a
+result, their applicability and performance in real-world scenarios remain
+unverified. Secondly, the frequently utilized evaluation metrics for these
+models, such as LPIPS and SSIM, are inherently designed for perceptual image
+analysis, not specifically for super-resolution. In response to these
+challenges, **'opensr-test'** has been introduced as a Python package, designed
+to provide users with three meticulously curated test datasets. These datasets
+are tailored to minimize spatial distortions between Low Resolution (LR) and
+High Resolution (HR) images, while calibrating differences in the spectral
+domain. Moreover, the **'opensr-test'** package offers five distinct types of
+metrics aimed at accurately evaluating the performance of ISR algorithms, thus
+addressing the aforementioned shortcomings of conventional evaluation
+techniques. ## Datasets The utilization of *synthetic data* in benchmarking
+could potentially introduce biased conclusions, as there are no guarantees that
+a degradation method could not inadvertently incorporate some form of bias,
+i.e. the degradation does not match the real-world ground sampling distance of
+the LR image. Therefore, to avoid *synthetic data* potential errors, the
+datasets utilized in **opensr-test** are meticulously created following a
+*cross-sensor approach* that means that HR and LR comes from different sensor
+but they are aligned as closely as possible, i.e. harmonized. Due to the
+limited availability of open HR resolution data that correspond with Sentinel-
+2, we propose using three HR sensors: SPOT, VENÂµS, and NAIP. | Dataset | Scale
+| # Scenes | HRsize | HR Reference | |----------------|-------|----------|-----
+---|---------------------------------------------------------------------------
+-----------------| | NAIP-19 | x4 | 200 | 512 | USDA Farm Production and
+Conservation - Business Center, Geospatial Enterprise Operations. | | SPOTPAN-
+10 | x4 | 200 | 512 | European Space Agency, 2017, SPOT 1-5 ESA | | Mini-
+SEN2VENÂµS | x2 | 200 | 512 | Vegetation and Environment monitoring on a New
+Micro-Satellite (SEN2VENÎ¼S). | ## Metrics We propose that evaluating the ISR
+process with a single metric is not adequate, and therefore, we suggest the use
+of five metrics, which will be detailed below.  Spectral consistency Measured
+based on the comparison of LR and SR images. The reflectance values are then
+compared using spectral angle distance metrics. The LR and degraded SR values
+should not be identical but rather similar.   Spatial consistency Measured
+again from the comparison of the LR and SR images, ground control points are
+obtained using LightGlue + DISK. The difference between the reference points
+and a first-order polynomial is then calculated.   High-frequency Measured from
+the comparison of LR and SR images, we calculate the MTF between the LR-SR
+pairs to assess the improvement in ground sampling distance. The MTF curve
+represents the system's response in different spatial frequencies. A higher MTF
+value at a specific frequency indicates a better resolution and sharper image
+details. The reported metric is the comparison of the area under the MTF curve
+between the LR and SR images, from the Nyquist frequency of Sentinel2 to the
+super-resolved image.   Omission Error related to the inability to represent
+the actual high-frequency information from the landscape. The systematic error
+must be first removed.   Hallucinations Hallucinations refer to errors that are
+solely related to high-frequency information inducted by the super-resolution
+model, with no correlation to the real continuous space.  [isort] ##
+Installation Install the latest version from PyPI: ``` pip install opensr-test
+``` Upgrade `opensr-test` by running: ``` pip install -U opensr-test ```
+Install the latest version from conda-forge: ``` conda install -c conda-forge
+opensr-test ``` Install the latest dev version from GitHub by running: ``` pip
+install git+https://github.com/ESAOpenSR/opensr-test ``` ## How does it work?
+opensr-test needs either a PyTorch (torch.nn.Module, torch.jit.trace or
+torch.jit.script) or TensorFlow model. The following example shows how to run
+the benchmarks:
                                    [header]
-**srcheck** needs either a `torch.nn.Module` class or a compiled model via
-`torch.jit.trace` or `torch.jit.script`. The following example shows how to run
-the benchmarks: ```python import torch import srcheck model = torch.jit.load('/
-content/quantSRmodel.pt', map_location='cpu') srcheck.benchmark(model,
-dataset='SPOT-50', metrics=['PSNR', 'SSIM'], type= "NoSRI") ``` srcheck
-supports two group types of metrics: (a) Surface Reflectance Integrity (SRI)
-and (b) No Surface Reflectance Integrity (NoSRI). This difference is due to the
-fact that depending on the application, developers will be interested in
-optimizing the "image quality" or the "image fidelity". *Image fidelity* refers
-to how closely the LR image represents the real source distribution (HR).
-Optimizing fidelity is crucial for applications that require preserving surface
-reflectance as close as possible to the original values. On the other hand,
-*image quality* refers to how pleasant the image is for the human eye.
-Optimizing image quality is important for creating HR image satellite base
-maps. The image below shows the natural trade-off that exists between these two
-group types of metrics.
-                                   [header]
-But what happens if my ISR algorithm increases the image by a factor of 8, but
-the datasets available in srcheck do not support 8X? In that case, *srcheck*
-will automatically convert the results to the native resolution of the
-datasets. For example, if your algorithm increases the image by 2X, and you
-want to test it on SPOT-50 whose images are 10m in LR and 6m in HR, *srcheck*
-will upscale the results from 5 meters to 6m using the bilinear interpolation
-algorithm. Similarly, in the MUS2-50 dataset, *srcheck* will downscale the
-results from 5m to 2m. This is done in order the results can be compared with
-the datasets available.
-                                   [header]
-## Datasets [**https://zenodo.org/record/7562334**](https://zenodo.org/record/
-7562334) More datasets are coming soon! ## Metrics Metrics documentation is
-coming soon! ## Pre-trained Models Pre-trained models are available at various
+The following example shows how to run the benchmarks: ```python import torch
+import opensr_test # Load your model model = torch.jit.load('/content/
+quantSRmodel.pt', map_location='cpu') # Check if the model works dataset =
+opensr_test.naip opensr_test.check(model, dataset) # { 'Spectral': 0.08,
+'Spatial': 2.34, 'High-frequency': 1.32, 'Hallucination': 0.90, 'Omission':
+1.03} ``` ## Pre-trained Models Pre-trained models are available at various
 scales and hosted at the awesome [`huggingface_hub`](https://huggingface.co/
 models?filter=super-image). By default the models were pretrained on [DIV2K]
 (https://huggingface.co/datasets/eugenesiow/Div2k), a dataset of 800 high-
 quality (2K resolution) images for training, augmented to 4000 images and uses
 a dev set of 100 validation images (images numbered 801 to 900). The
 leaderboard below shows the [PSNR](https://en.wikipedia.org/wiki/Peak_signal-
 to-noise_ratio#Quality_estimation_with_PSNR) / [SSIM](https://en.wikipedia.org/
```

### Comparing `opensr-test-0.0.2/opensr_test.egg-info/PKG-INFO` & `opensr-test-0.0.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,46 @@
 Metadata-Version: 2.1
 Name: opensr-test
-Version: 0.0.2
+Version: 0.0.3
 Summary: A comprehensive benchmark for real-world Sentinel-2 imagery super-resolution
 Home-page: https://github.com/ESAOpenSR/opensr-test
 Author: Cesar Aybar Camacho
 Author-email: csaybar@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
-  <a href="https://github.com/ESAOpenSR/opensr-test"><img src="https://user-images.githubusercontent.com/16768318/213960001-66bb7d18-13d8-41d4-9de3-1e8a77f73787.png" alt="header" width="55%"></a>
-</p>[Title](https://github.com/ESAOpenSR/opensr-check)
+  <a href="https://github.com/ESAOpenSR/opensr-test"><img src="https://github.com/ESAOpenSR/opensr-test/assets/16768318/15661226-f4c4-4d55-8dd1-d73a228e36da" alt="header" width="55%"></a>
+</p>
+
+
+
 
 <p align="center">
     <em>A comprehensive benchmark for real-world Sentinel-2 imagery super-resolution</em>
 </p>
 
 <p align="center">
 <a href='https://pypi.python.org/pypi/opensr-test'>
     <img src='https://img.shields.io/pypi/v/opensr-test.svg' alt='PyPI' />
 </a>
 
 <a href="https://opensource.org/licenses/MIT" target="_blank">
     <img src="https://img.shields.io/badge/License-MIT-blue.svg" alt="License">
 </a>
-<a href='https://opensr-test.readthedocs.io/en/latest/?badge=latest'>
-    <img src='https://readthedocs.org/projects/opensr-test/badge/?version=latest' alt='Documentation Status' />
+<a href='https://opensr-test.readthedocs.io/en/latest/?badge=main'>
+    <img src='https://readthedocs.org/projects/opensr-test/badge/?version=main' alt='Documentation Status' />
 </a>
 <a href="https://github.com/psf/black" target="_blank">
     <img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="Black">
 </a>
 <a href="https://pycqa.github.io/isort/" target="_blank">
     <img src="https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336" alt="isort">
 </a>
@@ -52,80 +56,115 @@
 
 **Paper**: Coming soon!
 
 ---
 
 ## Overview
 
-In remote sensing, image super-resolution (ISR) is a technique used to create high-resolution (HR) images from low-resolution (R) satellite images, giving a more detailed view of the Earth's surface. However, with the constant development and introduction of new ISR algorithms, it can be challenging to stay updated on the latest advancements and to evaluate their performance objectively. To address this issue, we introduce SRcheck, a Python package that provides an easy-to-use interface for comparing and benchmarking various ISR methods. SRcheck includes a range of datasets that consist of high-resolution and low-resolution image pairs, as well as a set of quantitative metrics for evaluating the performance of SISR algorithms.
+In the domain of remote sensing, image super-resolution (ISR) goal is augmenting the ground sampling distance, also known as spatial resolution. Over recent years, numerous research papers have been proposed addressing ISR; however, they invariably suffer from two main issues. Firstly, the majority of these proposed models are tested on synthetic data. As a result, their applicability and performance in real-world scenarios remain unverified. Secondly, the frequently utilized evaluation metrics for these models, such as LPIPS and SSIM, are inherently designed for perceptual image analysis, not specifically for super-resolution.
+
+In response to these challenges, **'opensr-test'** has been introduced as a Python package, designed to provide users with three meticulously curated test datasets. These datasets are tailored to minimize spatial distortions between Low Resolution (LR) and High Resolution (HR) images, while calibrating differences in the spectral domain. Moreover, the **'opensr-test'** package offers five distinct types of metrics aimed at accurately evaluating the performance of ISR algorithms, thus addressing the aforementioned shortcomings of conventional evaluation techniques.
+
+## Datasets
+
+The utilization of *synthetic data* in benchmarking could potentially introduce biased conclusions, as there are no guarantees that a degradation method could not inadvertently incorporate some form of bias, i.e. the degradation does not match the real-world ground sampling distance of the LR image. Therefore, to avoid *synthetic data* potential errors, the datasets utilized in **opensr-test** are meticulously created following a *cross-sensor approach* that means that HR and LR comes from different sensor but they are aligned as closely as possible, i.e. harmonized. Due to the limited availability of open HR resolution data that correspond with Sentinel-2, we propose using three HR sensors: SPOT, VENµS, and NAIP.
+
+
+| Dataset        | Scale | # Scenes | HRsize | HR Reference                                                                               |
+|----------------|-------|----------|--------|--------------------------------------------------------------------------------------------|
+| NAIP-19        | x4    | 200      | 512    | USDA Farm Production and Conservation - Business Center, Geospatial Enterprise Operations. |
+| SPOTPAN-10     | x4    | 200      | 512    | European Space Agency, 2017, SPOT 1-5 ESA                                                  |
+| Mini-SEN2VENµS | x2    | 200      | 512    | Vegetation and Environment monitoring on a New Micro-Satellite (SEN2VENμS).                |
+
+
+
+
+## Metrics
+
+We propose that evaluating the ISR process with a single metric is not adequate, and therefore, we suggest the use of five metrics, which will be detailed below.
+
+<details>
+    <summary><b>Spectral consistency</b></summary>
+    Measured based on the comparison of LR and SR images. The reflectance values are then compared using spectral angle distance metrics. The LR and degraded SR values should not be identical but rather similar.
+</details>
+
+<details>
+    <summary><b>Spatial consistency</b></summary>
+    Measured again from the comparison of the LR and SR images, ground control points are obtained using LightGlue + DISK. The difference between the reference points and a first-order polynomial is then calculated.
+</details>
+
+<details>
+    <summary><b>High-frequency</b></summary>
+    Measured from the comparison of LR and SR images, we calculate the MTF between the LR-SR pairs to assess the improvement in ground sampling distance. The MTF curve represents the system's response in different spatial frequencies. A higher MTF value at a specific frequency indicates a better resolution and sharper image details. The reported metric is the comparison of the area under the MTF curve between the LR and SR images, from the Nyquist frequency of Sentinel2 to the super-resolved image.
+</details>
+
+<details>
+    <summary><b>Omission</b></summary>
+    Error related to the inability to represent the actual high-frequency information from the landscape. The systematic error must be first removed.
+</details>
+
+<details>
+    <summary><b>Hallucinations</b></summary>
+    Hallucinations refer to errors that are solely related to high-frequency information inducted by the super-resolution model, with no correlation to the real continuous space. 
+</details>
+
+
+<img src="https://github.com/ESAOpenSR/opensr-test/assets/16768318/473865e5-5661-4b6a-b941-ae170ffd6d0e" alt="isort"  width="55%">
+
 
 ## Installation
 
 Install the latest version from PyPI:
 
 ```
-pip install srcheck
+pip install opensr-test
 ```
 
-Upgrade `srcheck` by running:
+Upgrade `opensr-test` by running:
 
 ```
-pip install -U srcheck
+pip install -U opensr-test
 ```
 
 Install the latest version from conda-forge:
 
 ```
-conda install -c conda-forge srcheck
+conda install -c conda-forge opensr-test
 ```
 
 Install the latest dev version from GitHub by running:
 
 ```
-pip install git+https://github.com/csaybar/srcheck
+pip install git+https://github.com/ESAOpenSR/opensr-test
 ```
 
 ## How does it work?
 
+opensr-test needs either a PyTorch (torch.nn.Module, torch.jit.trace or  torch.jit.script) or TensorFlow model. The following example shows 
+how to run the benchmarks:
+
 <center>
-    <img src="https://user-images.githubusercontent.com/16768318/213967913-3c665d59-5053-43a7-a450-859b7442b345.png" alt="header" width="70%">
+    <img src="https://github.com/ESAOpenSR/opensr-test/assets/16768318/60a34d0a-f7ab-4c52-b68c-978e51898733" alt="header" width="70%">
 </center>
 
-**srcheck** needs either a `torch.nn.Module` class or a compiled model via `torch.jit.trace` or `torch.jit.script`. The following example shows how to run the benchmarks:
+The following example shows how to run the benchmarks:
 
 ```python
 import torch
-import srcheck
+import opensr_test
 
+# Load your model
 model = torch.jit.load('/content/quantSRmodel.pt', map_location='cpu')
-srcheck.benchmark(model, dataset='SPOT-50', metrics=['PSNR', 'SSIM'], type= "NoSRI")
-```
-
-srcheck supports two group types of metrics: (a) Surface Reflectance Integrity (SRI) and (b) No Surface Reflectance Integrity (NoSRI). This difference is due to the fact that depending on the application, developers will be interested in optimizing the "image quality" or the "image fidelity". *Image fidelity* refers to how closely the LR image represents the real source distribution (HR). Optimizing fidelity is crucial for applications that require preserving surface reflectance as close as possible to the original values. On the other hand, *image quality* refers to how pleasant the image is for the human eye. Optimizing image quality is important for creating HR image satellite base maps. The image below shows the natural trade-off that exists between these two group types of metrics.
-
-
-<center>
-    <img src="https://user-images.githubusercontent.com/16768318/213970463-5c2a8012-4e76-48ce-bb13-4d51590d359c.png" alt="header" width="60%">
-</center>
-
-But what happens if my ISR algorithm increases the image by a factor of 8, but the datasets available in srcheck do not support 8X? In that case, *srcheck* will automatically convert the results to the native resolution of the datasets. For example, if your algorithm increases the image by 2X, and you want to test it on SPOT-50 whose images are 10m in LR and 6m in HR, *srcheck* will upscale the results from 5 meters to 6m using the bilinear interpolation algorithm. Similarly, in the MUS2-50 dataset, *srcheck* will downscale the results from 5m to 2m. This is done in order the results can be compared with the datasets available.
 
-<center>
-    <img src="https://user-images.githubusercontent.com/16768318/213971771-04b193e7-83e8-436a-b4a1-0c317cc7b756.png" alt="header" width="75%">
-</center>
-
-## Datasets
-
-[**https://zenodo.org/record/7562334**](https://zenodo.org/record/7562334)
+# Check if the model works
+dataset = opensr_test.naip
 
-More datasets are coming soon!
-
-## Metrics
-
-Metrics documentation is coming soon!
+opensr_test.check(model, dataset)
+# { 'Spectral': 0.08, 'Spatial': 2.34, 'High-frequency': 1.32, 'Hallucination': 0.90, 'Omission': 1.03}
+```
 
 ## Pre-trained Models
 Pre-trained models are available at various scales and hosted at the awesome [`huggingface_hub`](https://huggingface.co/models?filter=super-image). By default the models were pretrained on [DIV2K](https://huggingface.co/datasets/eugenesiow/Div2k), a dataset of 800 high-quality (2K resolution) images for training, augmented to 4000 images and uses a dev set of 100 validation images (images numbered 801 to 900). 
 
 The leaderboard below shows the 
 [PSNR](https://en.wikipedia.org/wiki/Peak_signal-to-noise_ratio#Quality_estimation_with_PSNR) / [SSIM](https://en.wikipedia.org/wiki/Structural_similarity#Algorithm) 
 metrics for each model at various scales on various test sets ([Set5](https://huggingface.co/datasets/eugenesiow/Set5),
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,70 +1,90 @@
-Metadata-Version: 2.1 Name: opensr-test Version: 0.0.2 Summary: A comprehensive
+Metadata-Version: 2.1 Name: opensr-test Version: 0.0.3 Summary: A comprehensive
 benchmark for real-world Sentinel-2 imagery super-resolution Home-page: https:/
 /github.com/ESAOpenSR/opensr-test Author: Cesar Aybar Camacho Author-email:
 csaybar@gmail.com License: MIT Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Description-Content-Type: text/markdown License-File:
-LICENSE
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Description-Content-Type: text/markdown License-File: LICENSE
                                    [header]
-[Title](https://github.com/ESAOpenSR/opensr-check)
  A comprehensive benchmark for real-world Sentinel-2 imagery super-resolution
             [PyPI] [License] [Documentation_Status] [Black] [isort]
 --- **GitHub**: [https://github.com/ESAOpenSR/opensr-test](https://github.com/
 ESAOpenSR/opensr-test) **Documentation**: [https://opensr-test.readthedocs.io/]
 (https://opensr-test.readthedocs.io/) **PyPI**: [https://pypi.org/project/
 opensr-test/](https://pypi.org/project/opensr-test/) **Paper**: Coming soon! --
-- ## Overview In remote sensing, image super-resolution (ISR) is a technique
-used to create high-resolution (HR) images from low-resolution (R) satellite
-images, giving a more detailed view of the Earth's surface. However, with the
-constant development and introduction of new ISR algorithms, it can be
-challenging to stay updated on the latest advancements and to evaluate their
-performance objectively. To address this issue, we introduce SRcheck, a Python
-package that provides an easy-to-use interface for comparing and benchmarking
-various ISR methods. SRcheck includes a range of datasets that consist of high-
-resolution and low-resolution image pairs, as well as a set of quantitative
-metrics for evaluating the performance of SISR algorithms. ## Installation
-Install the latest version from PyPI: ``` pip install srcheck ``` Upgrade
-`srcheck` by running: ``` pip install -U srcheck ``` Install the latest version
-from conda-forge: ``` conda install -c conda-forge srcheck ``` Install the
-latest dev version from GitHub by running: ``` pip install git+https://
-github.com/csaybar/srcheck ``` ## How does it work?
+- ## Overview In the domain of remote sensing, image super-resolution (ISR)
+goal is augmenting the ground sampling distance, also known as spatial
+resolution. Over recent years, numerous research papers have been proposed
+addressing ISR; however, they invariably suffer from two main issues. Firstly,
+the majority of these proposed models are tested on synthetic data. As a
+result, their applicability and performance in real-world scenarios remain
+unverified. Secondly, the frequently utilized evaluation metrics for these
+models, such as LPIPS and SSIM, are inherently designed for perceptual image
+analysis, not specifically for super-resolution. In response to these
+challenges, **'opensr-test'** has been introduced as a Python package, designed
+to provide users with three meticulously curated test datasets. These datasets
+are tailored to minimize spatial distortions between Low Resolution (LR) and
+High Resolution (HR) images, while calibrating differences in the spectral
+domain. Moreover, the **'opensr-test'** package offers five distinct types of
+metrics aimed at accurately evaluating the performance of ISR algorithms, thus
+addressing the aforementioned shortcomings of conventional evaluation
+techniques. ## Datasets The utilization of *synthetic data* in benchmarking
+could potentially introduce biased conclusions, as there are no guarantees that
+a degradation method could not inadvertently incorporate some form of bias,
+i.e. the degradation does not match the real-world ground sampling distance of
+the LR image. Therefore, to avoid *synthetic data* potential errors, the
+datasets utilized in **opensr-test** are meticulously created following a
+*cross-sensor approach* that means that HR and LR comes from different sensor
+but they are aligned as closely as possible, i.e. harmonized. Due to the
+limited availability of open HR resolution data that correspond with Sentinel-
+2, we propose using three HR sensors: SPOT, VENÂµS, and NAIP. | Dataset | Scale
+| # Scenes | HRsize | HR Reference | |----------------|-------|----------|-----
+---|---------------------------------------------------------------------------
+-----------------| | NAIP-19 | x4 | 200 | 512 | USDA Farm Production and
+Conservation - Business Center, Geospatial Enterprise Operations. | | SPOTPAN-
+10 | x4 | 200 | 512 | European Space Agency, 2017, SPOT 1-5 ESA | | Mini-
+SEN2VENÂµS | x2 | 200 | 512 | Vegetation and Environment monitoring on a New
+Micro-Satellite (SEN2VENÎ¼S). | ## Metrics We propose that evaluating the ISR
+process with a single metric is not adequate, and therefore, we suggest the use
+of five metrics, which will be detailed below.  Spectral consistency Measured
+based on the comparison of LR and SR images. The reflectance values are then
+compared using spectral angle distance metrics. The LR and degraded SR values
+should not be identical but rather similar.   Spatial consistency Measured
+again from the comparison of the LR and SR images, ground control points are
+obtained using LightGlue + DISK. The difference between the reference points
+and a first-order polynomial is then calculated.   High-frequency Measured from
+the comparison of LR and SR images, we calculate the MTF between the LR-SR
+pairs to assess the improvement in ground sampling distance. The MTF curve
+represents the system's response in different spatial frequencies. A higher MTF
+value at a specific frequency indicates a better resolution and sharper image
+details. The reported metric is the comparison of the area under the MTF curve
+between the LR and SR images, from the Nyquist frequency of Sentinel2 to the
+super-resolved image.   Omission Error related to the inability to represent
+the actual high-frequency information from the landscape. The systematic error
+must be first removed.   Hallucinations Hallucinations refer to errors that are
+solely related to high-frequency information inducted by the super-resolution
+model, with no correlation to the real continuous space.  [isort] ##
+Installation Install the latest version from PyPI: ``` pip install opensr-test
+``` Upgrade `opensr-test` by running: ``` pip install -U opensr-test ```
+Install the latest version from conda-forge: ``` conda install -c conda-forge
+opensr-test ``` Install the latest dev version from GitHub by running: ``` pip
+install git+https://github.com/ESAOpenSR/opensr-test ``` ## How does it work?
+opensr-test needs either a PyTorch (torch.nn.Module, torch.jit.trace or
+torch.jit.script) or TensorFlow model. The following example shows how to run
+the benchmarks:
                                    [header]
-**srcheck** needs either a `torch.nn.Module` class or a compiled model via
-`torch.jit.trace` or `torch.jit.script`. The following example shows how to run
-the benchmarks: ```python import torch import srcheck model = torch.jit.load('/
-content/quantSRmodel.pt', map_location='cpu') srcheck.benchmark(model,
-dataset='SPOT-50', metrics=['PSNR', 'SSIM'], type= "NoSRI") ``` srcheck
-supports two group types of metrics: (a) Surface Reflectance Integrity (SRI)
-and (b) No Surface Reflectance Integrity (NoSRI). This difference is due to the
-fact that depending on the application, developers will be interested in
-optimizing the "image quality" or the "image fidelity". *Image fidelity* refers
-to how closely the LR image represents the real source distribution (HR).
-Optimizing fidelity is crucial for applications that require preserving surface
-reflectance as close as possible to the original values. On the other hand,
-*image quality* refers to how pleasant the image is for the human eye.
-Optimizing image quality is important for creating HR image satellite base
-maps. The image below shows the natural trade-off that exists between these two
-group types of metrics.
-                                   [header]
-But what happens if my ISR algorithm increases the image by a factor of 8, but
-the datasets available in srcheck do not support 8X? In that case, *srcheck*
-will automatically convert the results to the native resolution of the
-datasets. For example, if your algorithm increases the image by 2X, and you
-want to test it on SPOT-50 whose images are 10m in LR and 6m in HR, *srcheck*
-will upscale the results from 5 meters to 6m using the bilinear interpolation
-algorithm. Similarly, in the MUS2-50 dataset, *srcheck* will downscale the
-results from 5m to 2m. This is done in order the results can be compared with
-the datasets available.
-                                   [header]
-## Datasets [**https://zenodo.org/record/7562334**](https://zenodo.org/record/
-7562334) More datasets are coming soon! ## Metrics Metrics documentation is
-coming soon! ## Pre-trained Models Pre-trained models are available at various
+The following example shows how to run the benchmarks: ```python import torch
+import opensr_test # Load your model model = torch.jit.load('/content/
+quantSRmodel.pt', map_location='cpu') # Check if the model works dataset =
+opensr_test.naip opensr_test.check(model, dataset) # { 'Spectral': 0.08,
+'Spatial': 2.34, 'High-frequency': 1.32, 'Hallucination': 0.90, 'Omission':
+1.03} ``` ## Pre-trained Models Pre-trained models are available at various
 scales and hosted at the awesome [`huggingface_hub`](https://huggingface.co/
 models?filter=super-image). By default the models were pretrained on [DIV2K]
 (https://huggingface.co/datasets/eugenesiow/Div2k), a dataset of 800 high-
 quality (2K resolution) images for training, augmented to 4000 images and uses
 a dev set of 100 validation images (images numbered 801 to 900). The
 leaderboard below shows the [PSNR](https://en.wikipedia.org/wiki/Peak_signal-
 to-noise_ratio#Quality_estimation_with_PSNR) / [SSIM](https://en.wikipedia.org/
```

### Comparing `opensr-test-0.0.2/setup.py` & `opensr-test-0.0.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,34 +10,31 @@
     text_type = type("")
     with io.open(filename, mode="r", encoding="utf-8") as fd:
         return re.sub(text_type(r":[a-z]+:`~?(.*?)`"), text_type(r"``\1``"), fd.read())
 
 
 setup(
     name="opensr-test",
-    version="0.0.2",
+    version="0.0.3",
     url="https://github.com/ESAOpenSR/opensr-test",
     license="MIT",
     author="Cesar Aybar Camacho",
     author_email="csaybar@gmail.com",
     description="A comprehensive benchmark for real-world Sentinel-2 imagery super-resolution",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     packages=find_packages(exclude=("tests",), include=["opensr-test", "opensr-test.*"]),    
     install_requires=[
-        "numpy",
         "pydantic",
         "alive_progress",
-        "orjson",
-        "timm",
-        "torchvision",
-        "pandas",
+        "numpy",
     ],
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8"
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
     ],
 )
```

