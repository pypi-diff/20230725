# Comparing `tmp/spelunker-0.5.5.tar.gz` & `tmp/spelunker-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spelunker-0.5.5.tar", last modified: Thu Jul 20 14:48:33 2023, max compression
+gzip compressed data, was "spelunker-1.0.0.tar", last modified: Mon Jul 24 23:48:17 2023, max compression
```

## Comparing `spelunker-0.5.5.tar` & `spelunker-1.0.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 ddeal     (5761) STSCI\science  (1031)        0 2023-07-20 14:48:33.457543 spelunker-0.5.5/
--rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)     1085 2023-07-19 23:46:23.000000 spelunker-0.5.5/LICENSE
--rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)     4213 2023-07-20 14:48:33.457916 spelunker-0.5.5/PKG-INFO
--rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)     3673 2023-07-20 14:27:18.000000 spelunker-0.5.5/README.md
--rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)      160 2023-07-20 14:48:33.459364 spelunker-0.5.5/setup.cfg
--rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)     1047 2023-07-20 14:43:56.000000 spelunker-0.5.5/setup.py
-drwxr-xr-x   0 ddeal     (5761) STSCI\science  (1031)        0 2023-07-20 14:48:33.453137 spelunker-0.5.5/spelunker.egg-info/
--rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)     4213 2023-07-20 14:48:33.000000 spelunker-0.5.5/spelunker.egg-info/PKG-INFO
--rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)      298 2023-07-20 14:48:33.000000 spelunker-0.5.5/spelunker.egg-info/SOURCES.txt
--rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)        1 2023-07-20 14:48:33.000000 spelunker-0.5.5/spelunker.egg-info/dependency_links.txt
--rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)        1 2023-07-20 14:48:33.000000 spelunker-0.5.5/spelunker.egg-info/not-zip-safe
--rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)       74 2023-07-20 14:48:33.000000 spelunker-0.5.5/spelunker.egg-info/requires.txt
--rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)       10 2023-07-20 14:48:33.000000 spelunker-0.5.5/spelunker.egg-info/top_level.txt
-drwxr-xr-x   0 ddeal     (5761) STSCI\science  (1031)        0 2023-07-20 14:48:33.456449 spelunker-0.5.5/src/
--rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)      121 2023-07-19 19:56:38.000000 spelunker-0.5.5/src/__init__.py
--rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)       21 2023-07-20 14:46:06.000000 spelunker-0.5.5/src/_version.py
--rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)      420 2023-07-20 03:46:26.000000 spelunker-0.5.5/src/dashboard.py
--rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)    42777 2023-07-20 03:38:07.000000 spelunker-0.5.5/src/spelunker.py
+drwxr-xr-x   0 ddeal     (5761) STSCI\science  (1031)        0 2023-07-24 23:48:17.179870 spelunker-1.0.0/
+-rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)     1085 2023-07-19 23:46:23.000000 spelunker-1.0.0/LICENSE
+-rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)     4561 2023-07-24 23:48:17.180246 spelunker-1.0.0/PKG-INFO
+-rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)     4022 2023-07-21 13:51:03.000000 spelunker-1.0.0/README.md
+-rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)      160 2023-07-24 23:48:17.181407 spelunker-1.0.0/setup.cfg
+-rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)     1047 2023-07-20 15:20:44.000000 spelunker-1.0.0/setup.py
+drwxr-xr-x   0 ddeal     (5761) STSCI\science  (1031)        0 2023-07-24 23:48:17.174606 spelunker-1.0.0/spelunker.egg-info/
+-rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)     4561 2023-07-24 23:48:16.000000 spelunker-1.0.0/spelunker.egg-info/PKG-INFO
+-rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)      298 2023-07-24 23:48:17.000000 spelunker-1.0.0/spelunker.egg-info/SOURCES.txt
+-rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)        1 2023-07-24 23:48:16.000000 spelunker-1.0.0/spelunker.egg-info/dependency_links.txt
+-rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)        1 2023-07-24 23:48:16.000000 spelunker-1.0.0/spelunker.egg-info/not-zip-safe
+-rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)       74 2023-07-24 23:48:16.000000 spelunker-1.0.0/spelunker.egg-info/requires.txt
+-rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)       10 2023-07-24 23:48:16.000000 spelunker-1.0.0/spelunker.egg-info/top_level.txt
+drwxr-xr-x   0 ddeal     (5761) STSCI\science  (1031)        0 2023-07-24 23:48:17.178588 spelunker-1.0.0/src/
+-rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)      121 2023-07-19 19:56:38.000000 spelunker-1.0.0/src/__init__.py
+-rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)       21 2023-07-24 23:47:02.000000 spelunker-1.0.0/src/_version.py
+-rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)      420 2023-07-20 15:20:44.000000 spelunker-1.0.0/src/dashboard.py
+-rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)    50750 2023-07-24 23:47:30.000000 spelunker-1.0.0/src/spelunker.py
```

### Comparing `spelunker-0.5.5/LICENSE` & `spelunker-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spelunker-0.5.5/PKG-INFO` & `spelunker-1.0.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spelunker
-Version: 0.5.5
+Version: 1.0.0
 Summary: spelunker: a library to extract guidestar data and observe technical and stellar events
 Home-page: https://github.com/GalagaBits/JWST-FGS-Spelunker
 Author: Derod Deal
 Author-email: dealderod@ufl.edu
 License: MIT
 Keywords: guidestars
 Requires: numpy
@@ -22,21 +22,21 @@
 
 # Spelunker — NIRISS FGS quicklook pipeline 
 
 ![](https://github.com/GalagaBits/JWST-FGS-Spelunker/blob/main/spelunker.png)
 
 -------------------------------------------------------------------------------------
 
-`spelunker` is a package that assists and finds technical anomalies and stellar properties from guidestars. 
+`spelunker` is a package that assists on studying JWST FGS/NIRISS guidestar data.
 
 **Authors:** Derod Deal (dealderod@ufl.edu), Néstor Espinoza (nespinoza@stsci.edu)
 
 ## Statement of need
 
-Every time JWST observes an object, it simultaneously observes a nearby star --- a so-called "guide star" --- with the NIRISS Fine Guidance Sensor (FGS) that is used to keep the telescope locked on the target of interest. While researchers typically focus on their science targets, the guide star data can be extremely interesting on its own right. On the one hand, telescope-level anomalies could be detected (and, in principle, corrected) using this guide star data. On the other, this data also provides a "free" sky survey in the infrared (0.6 to 5 microns), on which short (~hours to days) time series of stars are recorded --- which one could "mine" if a pipeline existed for it to search for, e.g., stellar variability or even exoplanet transits: a true treasure chest. Here we present a first version of an automated, public quick-look time-series data processing pipeline for NIRISS FGS data. The pipeline is able to generate time-series for several metrics of the FGS data in an automated fashion, including fluxes and PSF variations, along with derived products from those such as periodograms that can aid on their analysis given only a JWST program ID number.
+Every time JWST observes an object, it simultaneously observes a nearby star --- a so-called "guide star" --- with the NIRISS Fine Guidance Sensor (FGS) that is used to keep the telescope locked on the target of interest. While researchers typically focus on their science targets, the guide star data can be extremely interesting on its own right both to detect anomalies on science data, as well as to explore time-series data of guidestars themselves. `spelunker` provides an easy-to-access ("plug-and-play") library to access this guide star data. The library is able to generate time-series for several metrics of the FGS data in an automated fashion, including fluxes and PSF variations, along with derived products from those such as periodograms that can aid on their analysis given only a JWST program ID number.
 
 ## Installation
 
 To install `spelunker`, use `pip install`.
 
 ```bash
 pip install spelunker
@@ -45,26 +45,43 @@
 ## Using the library
 
 Get started with `spelunker` with only two lines of code.
 
 ```python
 import spelunker
 
-spk = spelunker.load('/Users/ddeal/JWST-Treasure-Chest/', pid=1534)
+spk = spelunker.load(pid=1534)
 ```
-With our object `spk`, we can start interpeting data from guidestars, such as making a plot of the tracked guidestars within a Program ID.
+This will download guidestar data for Program ID 1534; the `spk` object itself can then be used to explore this guidestar data! For example, let's make a plot of the guidestar time-series for the first minutes of this PID:
+
+```python
+import matplotlib.pyplot as plt
+
+# Convert times from MJD to minutes:
+plt.plot( ( spk.fg_time - spk.fg_time[0] ) * 24 * 60, spk.fg_flux )
+
+plt.xlim(0,10)
+plt.xlabel('Time from start (minutes)')
+plt.ylabel('Counts')
+
+```
+<p align='center'>
+    <img src="plots/timeseries.png"  width=100% height=80%>
+</p>
+
+(See below on more information that can be extracted, including fitting 2D gaussians to each FGS integration!). We can even make a plot of the tracked guidestars within this Program ID:
 
 ```python
 spk.guidestar_plot()
 ```
 <p align='center'>
     <img src="https://github.com/GalagaBits/JWST-FGS-Spelunker/blob/main/plots/guidestar_positions.png"  width=80% height=80%>
 </p>
 
-We can also plot the timeseries of fitted gaussian parameters (use `spk.gauss2d_fit` to apply gaussian fitting to all guidestar frames) or the flux timeseries. Mnemonics from JWST technical events can be overplotted on any timeseries, such as high-gain antenna (HGA) movement or when the FGS tracks a new guidestar.
+Mnemonics from JWST technical events can be overplotted on any timeseries, such as high-gain antenna (HGA) movement or to identify if the FGS tracks a new guidestar [if the `jwstuser` package is also installed](https://github.com/spacetelescope/jwstuser/):
 
 ```python
 import matplotlib.pyplot as plt
 
 spk.mast_api_token = 'insert a token from auth.MAST here'
 
 fig, ax = plt.subplots(figsize=(12,4),dpi=200)
@@ -83,7 +100,11 @@
 - [Guidestar Targets](https://github.com/GalagaBits/JWST-FGS-Spelunker/blob/main/notebooks/examples/guidestar_targets.ipynb)
 - [Pixel centroid changes and mnemonics](https://github.com/GalagaBits/JWST-FGS-Spelunker/blob/main/notebooks/examples/pixel_centroid_mnemonics.ipynb)
 
 
 ## Licence and attribution
 
 This project is under the MIT License, which can be viewed [here](https://github.com/GalagaBits/JWST-FGS-Spelunker/blob/main/LICENSE).
+
+## Acknowledgments
+
+DD and NE would like to thank the STScI's Space Astronomy Summer Program (SASP) as well as the National Astronomy Consortium (NAC) program which made it possible for them to work together on this fantastic project!
```

### Comparing `spelunker-0.5.5/README.md` & `spelunker-1.0.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # Spelunker — NIRISS FGS quicklook pipeline 
 
 ![](https://github.com/GalagaBits/JWST-FGS-Spelunker/blob/main/spelunker.png)
 
 -------------------------------------------------------------------------------------
 
-`spelunker` is a package that assists and finds technical anomalies and stellar properties from guidestars. 
+`spelunker` is a package that assists on studying JWST FGS/NIRISS guidestar data.
 
 **Authors:** Derod Deal (dealderod@ufl.edu), Néstor Espinoza (nespinoza@stsci.edu)
 
 ## Statement of need
 
-Every time JWST observes an object, it simultaneously observes a nearby star --- a so-called "guide star" --- with the NIRISS Fine Guidance Sensor (FGS) that is used to keep the telescope locked on the target of interest. While researchers typically focus on their science targets, the guide star data can be extremely interesting on its own right. On the one hand, telescope-level anomalies could be detected (and, in principle, corrected) using this guide star data. On the other, this data also provides a "free" sky survey in the infrared (0.6 to 5 microns), on which short (~hours to days) time series of stars are recorded --- which one could "mine" if a pipeline existed for it to search for, e.g., stellar variability or even exoplanet transits: a true treasure chest. Here we present a first version of an automated, public quick-look time-series data processing pipeline for NIRISS FGS data. The pipeline is able to generate time-series for several metrics of the FGS data in an automated fashion, including fluxes and PSF variations, along with derived products from those such as periodograms that can aid on their analysis given only a JWST program ID number.
+Every time JWST observes an object, it simultaneously observes a nearby star --- a so-called "guide star" --- with the NIRISS Fine Guidance Sensor (FGS) that is used to keep the telescope locked on the target of interest. While researchers typically focus on their science targets, the guide star data can be extremely interesting on its own right both to detect anomalies on science data, as well as to explore time-series data of guidestars themselves. `spelunker` provides an easy-to-access ("plug-and-play") library to access this guide star data. The library is able to generate time-series for several metrics of the FGS data in an automated fashion, including fluxes and PSF variations, along with derived products from those such as periodograms that can aid on their analysis given only a JWST program ID number.
 
 ## Installation
 
 To install `spelunker`, use `pip install`.
 
 ```bash
 pip install spelunker
@@ -23,26 +23,43 @@
 ## Using the library
 
 Get started with `spelunker` with only two lines of code.
 
 ```python
 import spelunker
 
-spk = spelunker.load('/Users/ddeal/JWST-Treasure-Chest/', pid=1534)
+spk = spelunker.load(pid=1534)
 ```
-With our object `spk`, we can start interpeting data from guidestars, such as making a plot of the tracked guidestars within a Program ID.
+This will download guidestar data for Program ID 1534; the `spk` object itself can then be used to explore this guidestar data! For example, let's make a plot of the guidestar time-series for the first minutes of this PID:
+
+```python
+import matplotlib.pyplot as plt
+
+# Convert times from MJD to minutes:
+plt.plot( ( spk.fg_time - spk.fg_time[0] ) * 24 * 60, spk.fg_flux )
+
+plt.xlim(0,10)
+plt.xlabel('Time from start (minutes)')
+plt.ylabel('Counts')
+
+```
+<p align='center'>
+    <img src="plots/timeseries.png"  width=100% height=80%>
+</p>
+
+(See below on more information that can be extracted, including fitting 2D gaussians to each FGS integration!). We can even make a plot of the tracked guidestars within this Program ID:
 
 ```python
 spk.guidestar_plot()
 ```
 <p align='center'>
     <img src="https://github.com/GalagaBits/JWST-FGS-Spelunker/blob/main/plots/guidestar_positions.png"  width=80% height=80%>
 </p>
 
-We can also plot the timeseries of fitted gaussian parameters (use `spk.gauss2d_fit` to apply gaussian fitting to all guidestar frames) or the flux timeseries. Mnemonics from JWST technical events can be overplotted on any timeseries, such as high-gain antenna (HGA) movement or when the FGS tracks a new guidestar.
+Mnemonics from JWST technical events can be overplotted on any timeseries, such as high-gain antenna (HGA) movement or to identify if the FGS tracks a new guidestar [if the `jwstuser` package is also installed](https://github.com/spacetelescope/jwstuser/):
 
 ```python
 import matplotlib.pyplot as plt
 
 spk.mast_api_token = 'insert a token from auth.MAST here'
 
 fig, ax = plt.subplots(figsize=(12,4),dpi=200)
@@ -60,8 +77,12 @@
 
 - [Guidestar Targets](https://github.com/GalagaBits/JWST-FGS-Spelunker/blob/main/notebooks/examples/guidestar_targets.ipynb)
 - [Pixel centroid changes and mnemonics](https://github.com/GalagaBits/JWST-FGS-Spelunker/blob/main/notebooks/examples/pixel_centroid_mnemonics.ipynb)
 
 
 ## Licence and attribution
 
-This project is under the MIT License, which can be viewed [here](https://github.com/GalagaBits/JWST-FGS-Spelunker/blob/main/LICENSE).
+This project is under the MIT License, which can be viewed [here](https://github.com/GalagaBits/JWST-FGS-Spelunker/blob/main/LICENSE).
+
+## Acknowledgments
+
+DD and NE would like to thank the STScI's Space Astronomy Summer Program (SASP) as well as the National Astronomy Consortium (NAC) program which made it possible for them to work together on this fantastic project!
```

### Comparing `spelunker-0.5.5/setup.py` & `spelunker-1.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `spelunker-0.5.5/spelunker.egg-info/PKG-INFO` & `spelunker-1.0.0/spelunker.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spelunker
-Version: 0.5.5
+Version: 1.0.0
 Summary: spelunker: a library to extract guidestar data and observe technical and stellar events
 Home-page: https://github.com/GalagaBits/JWST-FGS-Spelunker
 Author: Derod Deal
 Author-email: dealderod@ufl.edu
 License: MIT
 Keywords: guidestars
 Requires: numpy
@@ -22,21 +22,21 @@
 
 # Spelunker — NIRISS FGS quicklook pipeline 
 
 ![](https://github.com/GalagaBits/JWST-FGS-Spelunker/blob/main/spelunker.png)
 
 -------------------------------------------------------------------------------------
 
-`spelunker` is a package that assists and finds technical anomalies and stellar properties from guidestars. 
+`spelunker` is a package that assists on studying JWST FGS/NIRISS guidestar data.
 
 **Authors:** Derod Deal (dealderod@ufl.edu), Néstor Espinoza (nespinoza@stsci.edu)
 
 ## Statement of need
 
-Every time JWST observes an object, it simultaneously observes a nearby star --- a so-called "guide star" --- with the NIRISS Fine Guidance Sensor (FGS) that is used to keep the telescope locked on the target of interest. While researchers typically focus on their science targets, the guide star data can be extremely interesting on its own right. On the one hand, telescope-level anomalies could be detected (and, in principle, corrected) using this guide star data. On the other, this data also provides a "free" sky survey in the infrared (0.6 to 5 microns), on which short (~hours to days) time series of stars are recorded --- which one could "mine" if a pipeline existed for it to search for, e.g., stellar variability or even exoplanet transits: a true treasure chest. Here we present a first version of an automated, public quick-look time-series data processing pipeline for NIRISS FGS data. The pipeline is able to generate time-series for several metrics of the FGS data in an automated fashion, including fluxes and PSF variations, along with derived products from those such as periodograms that can aid on their analysis given only a JWST program ID number.
+Every time JWST observes an object, it simultaneously observes a nearby star --- a so-called "guide star" --- with the NIRISS Fine Guidance Sensor (FGS) that is used to keep the telescope locked on the target of interest. While researchers typically focus on their science targets, the guide star data can be extremely interesting on its own right both to detect anomalies on science data, as well as to explore time-series data of guidestars themselves. `spelunker` provides an easy-to-access ("plug-and-play") library to access this guide star data. The library is able to generate time-series for several metrics of the FGS data in an automated fashion, including fluxes and PSF variations, along with derived products from those such as periodograms that can aid on their analysis given only a JWST program ID number.
 
 ## Installation
 
 To install `spelunker`, use `pip install`.
 
 ```bash
 pip install spelunker
@@ -45,26 +45,43 @@
 ## Using the library
 
 Get started with `spelunker` with only two lines of code.
 
 ```python
 import spelunker
 
-spk = spelunker.load('/Users/ddeal/JWST-Treasure-Chest/', pid=1534)
+spk = spelunker.load(pid=1534)
 ```
-With our object `spk`, we can start interpeting data from guidestars, such as making a plot of the tracked guidestars within a Program ID.
+This will download guidestar data for Program ID 1534; the `spk` object itself can then be used to explore this guidestar data! For example, let's make a plot of the guidestar time-series for the first minutes of this PID:
+
+```python
+import matplotlib.pyplot as plt
+
+# Convert times from MJD to minutes:
+plt.plot( ( spk.fg_time - spk.fg_time[0] ) * 24 * 60, spk.fg_flux )
+
+plt.xlim(0,10)
+plt.xlabel('Time from start (minutes)')
+plt.ylabel('Counts')
+
+```
+<p align='center'>
+    <img src="plots/timeseries.png"  width=100% height=80%>
+</p>
+
+(See below on more information that can be extracted, including fitting 2D gaussians to each FGS integration!). We can even make a plot of the tracked guidestars within this Program ID:
 
 ```python
 spk.guidestar_plot()
 ```
 <p align='center'>
     <img src="https://github.com/GalagaBits/JWST-FGS-Spelunker/blob/main/plots/guidestar_positions.png"  width=80% height=80%>
 </p>
 
-We can also plot the timeseries of fitted gaussian parameters (use `spk.gauss2d_fit` to apply gaussian fitting to all guidestar frames) or the flux timeseries. Mnemonics from JWST technical events can be overplotted on any timeseries, such as high-gain antenna (HGA) movement or when the FGS tracks a new guidestar.
+Mnemonics from JWST technical events can be overplotted on any timeseries, such as high-gain antenna (HGA) movement or to identify if the FGS tracks a new guidestar [if the `jwstuser` package is also installed](https://github.com/spacetelescope/jwstuser/):
 
 ```python
 import matplotlib.pyplot as plt
 
 spk.mast_api_token = 'insert a token from auth.MAST here'
 
 fig, ax = plt.subplots(figsize=(12,4),dpi=200)
@@ -83,7 +100,11 @@
 - [Guidestar Targets](https://github.com/GalagaBits/JWST-FGS-Spelunker/blob/main/notebooks/examples/guidestar_targets.ipynb)
 - [Pixel centroid changes and mnemonics](https://github.com/GalagaBits/JWST-FGS-Spelunker/blob/main/notebooks/examples/pixel_centroid_mnemonics.ipynb)
 
 
 ## Licence and attribution
 
 This project is under the MIT License, which can be viewed [here](https://github.com/GalagaBits/JWST-FGS-Spelunker/blob/main/LICENSE).
+
+## Acknowledgments
+
+DD and NE would like to thank the STScI's Space Astronomy Summer Program (SASP) as well as the National Astronomy Consortium (NAC) program which made it possible for them to work together on this fantastic project!
```

### Comparing `spelunker-0.5.5/src/spelunker.py` & `spelunker-1.0.0/src/spelunker.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-# fgs_spelunker_ver5003
-
 import numpy as np
 import scipy.optimize as opt
 import pandas as pd
 import datetime
 
 from jwst import datamodels
 
 from astroquery.mast import Observations
 
-from astropy.table import Table, hstack
+from astropy.table import Table, hstack, vstack
 from astropy.time import Time
 from astropy import units as u
 from astropy.timeseries import LombScargle
 
 from astroplan.plots import plot_finder_image
 from astropy import coordinates
 from astropy.coordinates import SkyCoord
@@ -27,31 +25,52 @@
 import matplotlib.transforms as transforms
 
 import ray
 import glob
 import os
 
 
-
 try:
     from jwstuser import engdb
     jwstuser_installed = True
 
 except ImportError:
     jwstuser_installed = False
     print('jwstuser is not installed. mnemonics() will not work.')
 
 
-
 class load:
 
-    def __init__(self, directory, pid='None', obs_num='None',  visit='None', visit_group='None', parallel_sequnence_id='None', 
-                 activity_number='None', exposure_number='None', dir_seg='None', guider='None', calib_level=2):
-        self.directory = directory
-        os.chdir(self.directory)
+    init_dir = os.getcwd()
+
+    def __init__(self, dir='None', pid='None', obs_num='None',  visit='None', visit_group='None', parallel_sequnence_id='None', 
+                 activity_number='None', exposure_number='None', dir_seg='None', guider='None', calib_level=2, save=False):
+        
+        os.chdir(self.init_dir)
+
+        created_dir = "spelunker_outputs"
+        current_dir = self.init_dir
+
+        if dir != 'None':
+            os.chdir(dir)
+            if not os.path.exists(dir+'/'+created_dir):  #https://www.geeksforgeeks.org/how-to-create-directory-if-it-does-not-exist-using-python/
+                os.makedirs(created_dir)
+                temp_dirc = created_dir
+            else:
+                temp_dirc = created_dir
+
+        else:
+            if not os.path.exists(current_dir+'/'+created_dir):
+                os.makedirs(created_dir)
+                temp_dirc = created_dir
+            else:
+                temp_dirc = created_dir
+
+        self.directory = os.getcwd()+'/'+temp_dirc
+        print('Current working directory for spelunker: '+self.directory+'\n')
 
         self.mast_api_token = None
         self.fg_table = None
 
         self.fg_array = None
         self.fg_time = None
         self.fg_flux = None
@@ -61,16 +80,15 @@
 
         self.object_properties = None
 
         self.fontsize = 14
         
         if pid != 'None':
             self.download(pid, obs_num=obs_num, visit=visit, visit_group=visit_group, parallel_sequnence_id=parallel_sequnence_id,
-                          activity_number=activity_number, exposure_number=exposure_number, dir_seg=dir_seg, guider=guider, calib_level=calib_level)
-
+                          activity_number=activity_number, exposure_number=exposure_number, dir_seg=dir_seg, guider=guider, calib_level=calib_level, save=save)
 
     def stitcher(self, fg_timeseries):
         '''
         Stitches multiple projectids with respect to epoch in one single array.
         '''
         fg_cube = []
         for data in fg_timeseries:
@@ -111,25 +129,22 @@
 
         return fg_array, fg_time, fg_flux
     
     def normalization_flux_preprocessing(self,):
         '''
         Normalize star flux by star metadata.
         '''
-        os.chdir('mastDownload/JWST/')
 
         norm_array = []
         for data in self.fg_timeseries:
             norm_array.append(data.data/np.nanmedian(data.data))
 
         norm_array = np.vstack(norm_array)
         norm_flux = np.nansum(norm_array, axis=(1,2))
 
-        os.chdir(self.directory)
-
         return norm_array, norm_flux
 
     def time_sort_preprocessing(self, fg_array, fg_time, fg_flux):
         '''
         Sorts the three arrays by time, regardless of filename or file order.
         '''
 
@@ -165,34 +180,37 @@
             else:
                 duplicates_mask.append(False)
         
         return products[duplicates_mask]
 
 
     def download(self, pid, obs_num='None',  visit='None', visit_group='None', parallel_sequnence_id='None', 
-                 activity_number='None', exposure_number='None', dir_seg='None', guider='None', calib_level=2):
+                 activity_number='None', exposure_number='None', dir_seg='None', guider='None', calib_level=2, save=False):
         '''
         Downloads the data from the projectid website. Turns the projectid into a manageable
         fits file. Downloads the files onto a local directory.
         '''
 
         self.pid = pid
 
         os.chdir(self.directory)
-        
+
         if obs_num == 'None' and visit != 'None':
             raise ValueError('When a visit is identified, the obs_num needs to be identified.')
 
+        print("Connecting with astroquery...")
+        
         if obs_num != 'None' and visit != 'None':
             matched_obs = Observations.query_criteria(
                 obs_collection = 'JWST',
                 proposal_id=str(pid),
             )
             
-            data_products = Observations.get_product_list(matched_obs)
+            data_products = [Observations.get_product_list(obs) for obs in matched_obs]
+            data_products = vstack(data_products)
 
             products = Observations.filter_products(data_products,
                         productType=["AUXILIARY",],
                         extension="fits",
                         productSubGroupDescription = "GS-FG",
                         dataproduct_type='image'
             )
@@ -219,15 +237,17 @@
 
         elif obs_num != 'None':
             matched_obs = Observations.query_criteria(
                 obs_collection = 'JWST',
                 proposal_id=str(pid),
             )
 
-            data_products = Observations.get_product_list(matched_obs)
+            data_products = [Observations.get_product_list(obs) for obs in matched_obs]
+            data_products = vstack(data_products)
+
             products = Observations.filter_products(data_products,
                         productType=["AUXILIARY",],
                         extension="fits",
                         productSubGroupDescription = "GS-FG",
                         dataproduct_type='image'
             )
 
@@ -247,15 +267,17 @@
 
         else:
             matched_obs = Observations.query_criteria(
                 obs_collection = 'JWST',
                 proposal_id=str(pid),
                 )
 
-            data_products = Observations.get_product_list(matched_obs)
+            data_products = [Observations.get_product_list(obs) for obs in matched_obs]
+            data_products = vstack(data_products)
+
             products = Observations.filter_products(data_products,
                                     productType=["AUXILIARY",],
                                     extension="fits",
                                     productSubGroupDescription = "GS-FG",
                                     dataproduct_type='image'
                                     )
         
@@ -263,15 +285,15 @@
             mask = products['calib_level'] == int(calib_level)
             productsx = products[mask]
 
         productsx = self.duplicate_rm(productsx)
 
         manifest = Observations.download_products(productsx,)
 
-        os.chdir(self.directory+'mastDownload/JWST/')
+        os.chdir(self.directory+'/mastDownload/JWST/')
         fg_raw = sorted(glob.glob('**/jw0'+str(pid)+'**_gs-fg_**_cal.fits'))
 
         fg = []
         sliced_directory = []
 
         for i in fg_raw:
                 fg.append(i.rsplit('/')[-1])
@@ -383,16 +405,14 @@
         sort_table = fg_table.sort(['guidestar_time'])
 
         self.fg_datamodel = list(fg_table['object_fg'])
         self.fg_table = fg_table
 
         self.fg_timeseries = [fn for fn in self.fg_datamodel]
 
-        os.chdir(self.directory)
-
         all_times = []
         all_fluxes = []
         
         for i in self.fg_datamodel:
             all_times.append( np.linspace( i.meta.guidestar.data_start, 
                                i.meta.guidestar.data_end, 
                                i.data.shape[0])
@@ -415,17 +435,30 @@
 
             norm_array, norm_flux = self.normalization_flux_preprocessing()
 
             fg_time = self.stitcher(all_times)
 
             fg_array, fg_time, fg_flux = self.negative_flux_preprocessing(norm_array, fg_time, norm_flux)
 
-        np.save(self.directory+str(pid)+'fg_array', fg_array)
-        np.save(self.directory+str(pid)+'fg_flux', fg_flux)
-        np.save(self.directory+str(pid)+'fg_time', fg_time)
+
+        # Saving numpy arrays
+
+        os.chdir(self.directory)
+
+        if save:
+            data_arrays_dir = 'data_arrays'
+            if not os.path.exists(data_arrays_dir):
+                os.makedirs(data_arrays_dir)
+
+            os.chdir(self.directory+'/'+data_arrays_dir)
+            np.save('pid_'+str(pid)+'_fg_array', fg_array)
+            np.save('pid_'+str(pid)+'_fg_time', fg_time)
+            np.save('pid_'+str(pid)+'_fg_flux', fg_flux)
+
+            os.chdir(self.directory)
 
         self.fg_array = fg_array
         self.fg_time = fg_time
         self.fg_flux = fg_flux
 
         self.fg_table = self.table()
         self.object_properties = self.object_properties_func()
@@ -509,28 +542,27 @@
         self.fg_array = fg_array
         self.fg_time = fg_time
         self.fg_flux = fg_flux
         self.fg_datamodel = fg2
         self.fg_table = None
         self.object_properties = None
 
-    def time_array_sec(self, fg_time):
+    def time_to_sec(self, fg_time):
         '''
         Creates an time array using from fg_time. Outputs elasped time and epoch time in mjd.
         '''
         return (fg_time - fg_time[0]) * 24 * 3600.
 
 
     '''
     FITTING TOOLS
     ------------------------------------------------------------------------------------------------------
     '''
 
-
-    def gauss2d_fit(self, fg_array='None', ncpus=4):
+    def gauss2d_fit(self, fg_array='None', ncpus=4, save=False):
         '''
         Applies a spatial gaussian fit to a data array for guide star data. The gaussian parameters
         include amplitude, centriods, stddev, and theta. Uses ray. Outputs an astopy table.
         '''
         if type(fg_array) == str:
             if fg_array == 'None':
                 fg_array = self.fg_array
@@ -547,20 +579,25 @@
             c = (np.sin(theta)**2)/(2*sigma_x**2) + (np.cos(theta)**2)/(2*sigma_y**2)
             g = amplitude*np.exp( - (a*((x-xo)**2) + 2*b*(x-xo)*(y-yo) 
                                     + c*((y-yo)**2))) + offset
             return g.ravel()
         
         ray.shutdown()
 
-        @ray.remote(num_cpus=ncpus,)
+        @ray.remote(num_cpus=ncpus, max_retries=3)
         def ray_curve_fit(gaussian_2d, xx, yy, datar, initial_guess):
-            popt, pcov = opt.curve_fit(gaussian_2d, (xx, yy), datar, p0=initial_guess, maxfev = 500000)
-            return popt
+            try:
+                popt, pcov = opt.curve_fit(gaussian_2d, (xx, yy), datar, p0=initial_guess, maxfev = 2000)
+                return popt
+            
+            except RuntimeError:
+                popt = [np.nan]*7
+                return popt
     
-        ray.init(ignore_reinit_error=True)
+        ray.init(ignore_reinit_error=True, num_cpus = ncpus)
         
         x = np.linspace(0, 7, 8)
         y = np.linspace(0, 7, 8)
         xx, yy = np.meshgrid(x, y)
 
         if len(fg_array.shape) == 3 and fg_array.shape[0] != 1:
 
@@ -572,42 +609,40 @@
 
                 initial_guess = np.array([datar.max(), int(coords[1]), int(coords[0]), 1, 1, 0, zodical_light])
 
                 popt = ray_curve_fit.remote(gaussian_2d, xx, yy, datar, initial_guess)
                 initial_guess_main_obj.append(popt)
 
             initial_guess_main = []
+
             for i in initial_guess_main_obj:
                 popt2 = ray.get(i)
                 initial_guess_main.append([popt2[0], popt2[1],popt2[2],popt2[3],popt2[4],popt2[5],popt2[6]])
 
             guess = Table(rows=initial_guess_main, names=['amplitude','x_mean', 'y_mean', 'x_stddev', 'y_stddev', 'theta', 'offset'])
 
             initial_guess = np.array([np.nanmedian(guess['amplitude']),np.nanmedian(guess['x_mean']),np.nanmedian(guess['y_mean']),
                                         np.nanmedian(guess['x_stddev']),np.nanmedian(guess['y_stddev']),np.nanmedian(guess['theta']),np.nanmedian(guess['offset'])])
             
             rows5_obj = []
             for idx, data in enumerate(fg_array):
                 datar = data.ravel()
                 zodical_light = np.nanmedian(data[0:3,5:8])
+                coords = np.where(data==datar.max())
 
                 initial_guess[6] = zodical_light
+                initial_guess[1], initial_guess[2] = int(coords[1]), int(coords[0])
 
                 popt = ray_curve_fit.remote(gaussian_2d, xx, yy, datar, initial_guess)
                 rows5_obj.append(popt)
 
             rows5 = []
-            for i in rows5_obj:
-                try:
-                    popt3 = ray.get(i)
-                    rows5.append([popt3[0], popt3[1],popt3[2],popt3[3],popt3[4],popt3[5],popt3[6]])
-
-                except RuntimeError:
-                    print('A runtime error has occured with fitting. Logging nan.')
-                    rows5.append([np.nan]*7)
+            for idx, i in enumerate(rows5_obj):
+                popt3 = ray.get(i)
+                rows5.append([popt3[0], popt3[1],popt3[2],popt3[3],popt3[4],popt3[5],popt3[6]])                
 
         elif len(fg_array.shape) == 2 and (fg_array.shape[0] & fg_array.shape[1]) == 8:
             
             data = np.copy(fg_array)
             datar = data.ravel()
             zodical_light = np.nanmedian(data[0:3, 5:8])
             coords = np.where(data==datar.max())
@@ -619,18 +654,23 @@
 
         ray.shutdown()
 
         table = Table(rows=rows5, names=['amplitude','x_mean', 'y_mean', 'x_stddev', 'y_stddev', 'theta', 'offset'])
 
         self.gaussfit_results = table
         
+        if save:
+            gaussfits_array_dir = 'gaussfits'
+            if not os.path.exists(gaussfits_array_dir):
+                os.makedirs(gaussfits_array_dir)
+            table.write(str(self.pid)+'_'+gaussfits_array_dir+'.dat', format='ascii', overwrite=True)
 
         return table
     
-    def quick_fit(self, fg_array):
+    def quick_fit(self, fg_array='None', save=False):
         '''
         Performs a quick fit to an array of fg data. Outputs an astropy table
         '''
         if type(fg_array) == str:
             if fg_array == 'None':
                 fg_array = self.fg_array
 
@@ -675,14 +715,20 @@
         quick_fit_table['y_mean'] = np.nan_to_num(cen_y)
         quick_fit_table['x_stddev'] = np.nan_to_num(std_x)
         quick_fit_table['y_stddev'] = np.nan_to_num(std_y)
         quick_fit_table['theta'] = 0
         quick_fit_table['offset'] = 0
 
         self.quickfit_results = quick_fit_table
+        
+        if save:
+            quickfits_array_dir = 'quickfits'
+            if not os.path.exists(quickfits_array_dir):
+                os.makedirs(quickfits_array_dir)
+            quick_fit_table.write(str(self.pid)+'_'+quickfits_array_dir+'.dat', format='ascii', overwrite=True)
 
         return quick_fit_table
 
 
     '''
     POSTPROCESSING METHODS 
     ------------------------------------------------------------------------------------------------------
@@ -704,15 +750,41 @@
         return min, max
 
 
     '''
     ANALYTICAL TOOLS 
     ------------------------------------------------------------------------------------------------------
     '''
-
+    def timescale(self, fg_time, fg_time_sec,):
+        '''
+        '''
+        if fg_time_sec[-1] > 172800:
+            # in mjd
+            #ax2.plot(short_fg_time, short_fg_flux)
+            xlabel = 'Time (mjd)'
+            time = fg_time
+            return xlabel, time
+        elif fg_time_sec[-1] > 10800:
+            # in hours
+            #ax2.plot(short_fg_time_sec /60 /60, short_fg_flux)
+            xlabel = 'Time (hours)'
+            time = fg_time_sec /60 /60
+            return xlabel, time
+        elif fg_time_sec[-1] > 300:
+            # in minutes
+            #ax2.plot(short_fg_time_sec /60, short_fg_flux)
+            xlabel = 'Time (mins)'
+            time = fg_time_sec /60
+            return xlabel, time
+        else:
+            # in secs
+            #ax2.plot(short_fg_time_sec, short_fg_flux)
+            xlabel = 'Time (sec)'
+            time = fg_time_sec
+            return xlabel, time
 
     def bin_data(self, time, y, n_bin):
     
         # Stolen from juliet: https://github.com/nespinoza/juliet/blob/master/juliet/utils.py
         time_bins = []
         y_bins = []
         y_err_bins = []
@@ -721,105 +793,115 @@
             y_bins.append(np.median(y[i:i + n_bin - 1]))
             y_err_bins.append(
                 np.sqrt(np.var(y[i:i + n_bin - 1])) /
                 np.sqrt(len(y[i:i + n_bin - 1])))
             
         return np.array(time_bins), np.array(y_bins), np.array(y_err_bins)
     
-    def timeseries_binned_plot(self, fg_time='None', fg_flux='None'):
+    def timeseries_binned_plot(self, fg_time='None', fg_flux='None', start_time='None', end_time='None'):
 
         if type(fg_flux) and type(fg_time) == str:
             if fg_time and fg_flux == 'None':
                 fg_time = self.fg_time
                 fg_flux = self.fg_flux
 
+        if start_time and end_time != 'None':
+            start_time_idx = np.abs(fg_time - start_time).argmin() # https://www.geeksforgeeks.org/find-the-nearest-value-and-the-index-of-numpy-array/
+            end_time_idx = np.abs(fg_time - end_time).argmin()
+
+            fg_time = fg_time[start_time_idx:end_time_idx]
+            fg_flux = fg_flux[start_time_idx:end_time_idx]
+            
+        fg_time_sec = self.time_to_sec(fg_time)
+        xlabel, time_scaled = self.timescale(fg_time, fg_time_sec)
+
         ax = plt.subplot()
 
-        tbin, ybin, ybinerr = self.bin_data(fg_time, fg_flux / np.nanmedian(fg_flux), n_bin = 314)
+        norm_flux = fg_flux/ np.nanmedian(fg_flux)
 
-        ax.plot(fg_time, fg_flux/ np.nanmedian(fg_flux), color = 'black', alpha = 0.1)
+        tbin, ybin, ybinerr = self.bin_data(time_scaled, norm_flux, n_bin = 96)
+        ax.plot(time_scaled, norm_flux, color = 'black', alpha = 0.1)
         ax.errorbar(tbin, ybin, ybinerr, fmt = 'o', 
              mfc = 'white', mec = 'black', ecolor = 'black', elinewidth = 1, alpha=0.8)
         
         ax.set_ylabel('Relative flux', fontsize = self.fontsize)
-        ax.set_xlabel('Time (mjd)')
-        ax.set_ylim(0.4, 1.6)
+        ax.set_xlabel(xlabel)
+        ax.set_ylim(np.nanmean(norm_flux) - 2*np.nanstd(norm_flux), np.nanmean(norm_flux) + 2*np.nanstd(norm_flux))
 
         return ax
     
     def timeseries_list_plot(self, table='None', fg_time='None', start_time='None', end_time='None'):
 
         if type(fg_time) and type(table) == str:
             if table and fg_time == 'None':
                 table = self.gaussfit_results
                 fg_time = self.fg_time
 
+        if start_time and end_time != 'None':
+            start_time_idx = np.abs(fg_time - start_time).argmin()
+            end_time_idx = np.abs(fg_time - end_time).argmin()
+            fg_time = fg_time[start_time_idx:end_time_idx]
+
+        fg_time_sec = self.time_to_sec(fg_time)
+        xlabel, time_scaled = self.timescale(fg_time, fg_time_sec)
+
         fig, ax = plt.subplots(4,2, figsize = (12,21), dpi = 200)
 
         #ax[].plot(fg_time, cen_x, color = 'black', alpha = .4)
         ax[0,0].set_title('Centroid_x')
-        ax[0,0].plot(fg_time, table['x_mean'])
-        ax[0,0].set_xlabel('Time (mjd)')
+        ax[0,0].plot(time_scaled, table['x_mean'])
+        ax[0,0].set_xlabel(xlabel)
         ax[0,0].set_ylabel('Pixel')
-        ax[0,0].set_ylim(np.mean(table['x_mean']) - 5*np.nanstd(table['x_mean']), 
-                         np.mean(table['x_mean']) + 5*np.nanstd(table['x_mean']))
+        ax[0,0].set_ylim(np.nanmean(table['x_mean']) - 5*np.nanstd(table['x_mean']), 
+                         np.nanmean(table['x_mean']) + 5*np.nanstd(table['x_mean']))
 
         ax[1,0].set_title('stddev_x')
-        ax[1,0].plot(fg_time, table['x_stddev'])
-        ax[1,0].set_ylim(np.mean(table['x_stddev']) - 1*np.nanstd(table['x_stddev']), 
-                         np.mean(table['x_stddev']) + 5*np.nanstd(table['x_stddev']))
-        ax[1,0].set_xlabel('Time (mjd)')
+        ax[1,0].plot(time_scaled, table['x_stddev'])
+        ax[1,0].set_ylim(np.nanmean(table['x_stddev']) - 1*np.nanstd(table['x_stddev']), 
+                         np.nanmean(table['x_stddev']) + 5*np.nanstd(table['x_stddev']))
+        ax[1,0].set_xlabel(xlabel)
         ax[1,0].set_ylabel('Pixel')
 
         ax[0,1].set_title('Centroid_y')
-        ax[0,1].plot(fg_time,table['y_mean'], color='orange')
-        ax[0,1].set_ylim(np.mean(table['y_mean']) - 5*np.nanstd(table['y_mean']), 
-                         np.mean(table['y_mean']) + 5*np.nanstd(table['y_mean']))
-        ax[0,1].set_xlabel('Time (mjd)')
+        ax[0,1].plot(time_scaled,table['y_mean'], color='orange')
+        ax[0,1].set_ylim(np.nanmean(table['y_mean']) - 5*np.nanstd(table['y_mean']), 
+                         np.nanmean(table['y_mean']) + 5*np.nanstd(table['y_mean']))
+        ax[0,1].set_xlabel(xlabel)
         ax[0,1].set_ylabel('Pixel')
         
         ax[1,1].set_title('stddev_y')
-        ax[1,1].plot(fg_time,table['y_stddev'], color='orange')
-        ax[1,1].set_ylim(np.mean(table['y_stddev']) - 1*np.nanstd(table['y_stddev']), 
-                         np.mean(table['y_stddev']) + 5*np.nanstd(table['y_stddev']))
-        ax[1,1].set_xlabel('Time (mjd)')
+        ax[1,1].plot(time_scaled,table['y_stddev'], color='orange')
+        ax[1,1].set_ylim(np.nanmean(table['y_stddev']) - 1*np.nanstd(table['y_stddev']), 
+                         np.nanmean(table['y_stddev']) + 5*np.nanstd(table['y_stddev']))
+        ax[1,1].set_xlabel(xlabel)
         ax[1,1].set_ylabel('Pixel')
 
         ax[2,0].set_title('amplitude')
-        ax[2,0].plot(fg_time,table['amplitude'], color='blue')
-        ax[2,0].set_ylim(np.mean(table['amplitude']) - 3*np.nanstd(table['amplitude']), 
-                         np.mean(table['amplitude']) + 3*np.nanstd(table['amplitude']))
-        ax[2,0].set_xlabel('Time (mjd)')
+        ax[2,0].plot(time_scaled,table['amplitude'], color='blue')
+        ax[2,0].set_ylim(np.nanmean(table['amplitude']) - 3*np.nanstd(table['amplitude']), 
+                         np.nanmean(table['amplitude']) + 3*np.nanstd(table['amplitude']))
+        ax[2,0].set_xlabel(xlabel)
         ax[2,0].set_ylabel('Counts')
 
         ax[2,1].set_title('theta')
-        ax[2,1].plot(fg_time,table['theta'], color='red')
-        ax[2,1].set_ylim(np.mean(table['theta']) - 3*np.nanstd(table['theta']), 
-                         np.mean(table['theta']) + 3*np.nanstd(table['theta']))
-        ax[2,1].set_xlabel('Time (mjd)')
+        ax[2,1].plot(time_scaled,table['theta'], color='red')
+        ax[2,1].set_ylim(np.nanmean(table['theta']) - 3*np.nanstd(table['theta']), 
+                         np.nanmean(table['theta']) + 3*np.nanstd(table['theta']))
+        ax[2,1].set_xlabel(xlabel)
         ax[2,1].set_ylabel('Radians')
 
         ax[3,0].set_title('offset')
-        ax[3,0].plot(fg_time,table['offset'], color='lightblue')
-        ax[3,0].set_ylim(np.mean(table['offset']) - 3*np.nanstd(table['offset']), 
-                         np.mean(table['offset']) + 3*np.nanstd(table['offset']))
+        ax[3,0].plot(time_scaled,table['offset'], color='lightblue')
+        ax[3,0].set_ylim(np.nanmean(table['offset']) - 3*np.nanstd(table['offset']), 
+                         np.nanmean(table['offset']) + 3*np.nanstd(table['offset']))
         ax[3,0].set_xlabel('Time (mjd)')
         ax[3,0].set_ylabel('Counts')
 
         ax[3,1].set_visible(False)
 
-        if start_time and end_time != 'None':
-            ax[0,0].set_xlim(start_time,end_time)
-            ax[0,1].set_xlim(start_time,end_time)
-            ax[1,0].set_xlim(start_time,end_time)
-            ax[1,1].set_xlim(start_time,end_time)
-            ax[2,0].set_xlim(start_time,end_time)
-            ax[2,1].set_xlim(start_time,end_time)
-            ax[3,0].set_xlim(start_time,end_time)
-
         return ax
    
     def guidestar_plot(self,):
         '''
         '''
         coords = SkyCoord(self.object_properties['ra'], self.object_properties['dec'], unit='deg')
         target = SkyCoord(np.mean(coords.ra),np.mean(coords.dec),unit='deg')
@@ -895,16 +977,14 @@
                 ax = plt.subplot()
 
                 for x_time, y_time in pairwise(event_time):
                     ax.axvspan(x_time, y_time, alpha=0.3)
                     ax.axvline(x_time,color='g',)
                     ax.axvline(y_time, color='r',)
 
-                print(event_time)
-
                 ax.axvline(x_time, color='g', label='hga_start')
                 ax.axvline(y_time, color='r', label='hga_stop')
 
                 return ax
             elif event_time == []:
                 print('No HGA events found. Returning a blank plot.')
                 ax = plt.subplot()
@@ -978,29 +1058,29 @@
                 ax.text(x, 0.75, s=str(' '+y[0:20]),transform=trans, clip_on=True, rotation=5, wrap=True)
                 ax.text(x, 0.7, s=str(' '+y[20:42]),transform=trans, clip_on=True, rotation=5, wrap=True)
 
             ax.axvline(self.filename_mnemonics[0][0], color='brown', label='filename')
                 
             return ax
 
-    def periodogram(self, table='None', time='None'):
+    def periodogram(self, table='None', time='None', save=False):
         '''
         Creates a periodogram plot for all parameters.
         '''
         if type(time) and type(table) == str:
             if table and time == 'None':
                 table = self.gaussfit_results
                 time = self.fg_time
 
         time_t, gs_xmean, gs_ymean = time, table['x_mean'].value, table['y_mean'].value
         gs_xstddev, gs_ystddev = table['x_stddev'].value, table['y_stddev'].value
         gs_theta, gs_amplitude = table['theta'].value, table['amplitude'].value
         gs_offset = table['offset'].value
 
-        time_t = self.time_array_sec(time_t)
+        time_t = self.time_to_sec(time_t)
 
         frequency_sub0, power_sub0 = LombScargle(time_t, gs_amplitude).autopower(samples_per_peak=5)
         frequency_sub1, power_sub1 = LombScargle(time_t, gs_xmean).autopower(samples_per_peak=5)
         frequency_sub2, power_sub2 = LombScargle(time_t, gs_ymean).autopower(samples_per_peak=5)
         frequency_sub3, power_sub3 = LombScargle(time_t, gs_xstddev).autopower(samples_per_peak=5)
         frequency_sub4, power_sub4 = LombScargle(time_t, gs_ystddev).autopower(samples_per_peak=5)
         frequency_sub5, power_sub5 = LombScargle(time_t, gs_theta).autopower(samples_per_peak=5)
@@ -1045,18 +1125,23 @@
         self.pgram_x_mean = pgram_table['frequency_x_mean'], pgram_table['power_x_mean']
         self.pgram_y_mean = pgram_table['frequency_y_mean'], pgram_table['power_y_mean']
         self.pgram_x_stddev = pgram_table['frequency_x_stddev'], pgram_table['power_x_stddev']
         self.pgram_y_stddev = pgram_table['frequency_y_stddev'], pgram_table['power_y_stddev']
         self.pgram_theta = pgram_table['frequency_theta'], pgram_table['power_theta']
         self.pgram_offset = pgram_table['frequency_offset'], pgram_table['power_offset']
 
+        if save:
+            periodogram_dir = 'periodograms'
+            if not os.path.exists(periodogram_dir):
+                os.makedirs(periodogram_dir)
+            table.write(str(self.pid)+'_'+periodogram_dir+'.dat', format='ascii', overwrite=True)
+        
         return ax
 
 
-
     '''
     ANIMATIONS 
     ------------------------------------------------------------------------------------------------------
     '''
 
 
     def timelapse_animation(self,fg_array='None', start = 0, stop = -1, interval=100, filename='movie.gif'):
@@ -1077,63 +1162,147 @@
         # From matplotlib https://matplotlib.org/stable/gallery/animation/dynamic_image.html
         ims = []
 
         min, max = self.minmax_gaussian_postprocessing(fg_array)
 
         for i in range(len(short_fg_array)):
             im = ax.imshow(short_fg_array[i], animated=True)
+            im.set_clim(vmin=min, vmax=max)
             if i == 0:
                 ax.imshow(short_fg_array[i])
             ims.append([im])
 
         fig.suptitle('Guidestar spatial timeseries animation')
         fig.colorbar(im, label='Counts', ax = ax)
         fig.tight_layout()
 
         ani = animation.ArtistAnimation(fig, ims, interval=interval, blit=True,
                                         repeat_delay=1000)
         ani.save(filename)
 
-    def flux_spatial_timelapse_animation(self,fg_array='None', fg_flux='None', start = 0, stop = -1, interval=100, filename='movie.mp4',):
+    def flux_spatial_timelapse_animation(self,fg_array='None', fg_time='None', fg_flux='None', start = 0, stop = 100, interval=100, filename='movie.gif',):
         '''
         Creates an animation of a timeseries for a fg_array. Inputs array, start frame and stop frame
         '''
-        if type(fg_flux) and type(fg_array) == str:
+        if type(fg_flux) and type(fg_array) and type(fg_time) == str:
             if fg_array and fg_flux == 'None':
                 fg_array = self.fg_array
                 fg_flux = self.fg_flux
+                fg_time = self.fg_time
 
         fig = plt.figure(figsize=(14,6), dpi=200)
 
         ax1 = fig.add_subplot(1,2,2)
         ax2 = fig.add_subplot(1,2,1)
 
         ax1.get_xaxis().set_visible(False)
         ax1.get_yaxis().set_visible(False)
 
         ax2.set_ylabel('Counts')
-        ax2.get_xaxis().set_visible(False)
+        ax2.get_xaxis().set_visible(True)
         
         short_fg_array = fg_array[start:stop]
         short_fg_flux = fg_flux[start:stop]
+        short_fg_time = fg_time[start:stop]
+
+        short_fg_time_sec = self.time_to_sec(short_fg_time)
+
+        xlabel, short_fg_time_animated = self.timescale(short_fg_time, short_fg_time_sec)
 
+        ax2.set_xlabel(xlabel)
+            
         ims = []
 
         min, max = self.minmax_gaussian_postprocessing(fg_array)
 
-        for i in range(len(short_fg_array)):
-            im = ax1.imshow(short_fg_array[i], animated=True)
-            im.set_clim(min, max)
+        im2, = ax2.plot(short_fg_time_animated, short_fg_flux, animated=True, color='black', alpha=0.5)
+        for idx, i in enumerate(short_fg_time_animated):
+            
+            im = ax1.imshow(short_fg_array[idx], animated=True)
+            im.set_clim(vmin=min, vmax=max)
 
-            im2, = ax2.plot(short_fg_flux, animated=True, color='black', alpha=0.5)
             im3 = ax2.vlines(i, np.min(short_fg_flux), np.max(short_fg_flux),  animated=True, color='red')
-
             ims.append([im, im2, im3])
 
         fig.suptitle('Guidestar spatial timeseries animation')
         fig.colorbar(im, label='Counts', ax = ax1)
         fig.tight_layout()
 
         ani = animation.ArtistAnimation(fig, ims, interval=interval, blit=True,
                                         repeat_delay=1000)
         
-        ani.save(filename,writer='ffmpeg')
+        ani.save(filename,writer='ffmpeg')
+
+
+    '''  
+    UTILITY FUNCTIONS 
+    ------------------------------------------------------------------------------------------------------
+    '''
+
+    def save(self, suffix = None):
+        '''
+        This function saves all the time-series information available from the guidestar in an easy-to-read format. Right now works only for 
+        the case on which one has a single guidestar:
+
+        Inputs:
+        -------
+
+        :param suffix: (optional, string)
+        String that will be added in front of the output filename.
+
+        Outputs:
+        -------
+        This function saves outputs to a .txt file.
+
+
+        '''
+
+        header = '# spelunker guidestar outputs\n'+\
+                 '# ---------------------------\n#\n' 
+
+        for i in range( len(self.object_properties['guidestar_catalog_id']) ):
+
+            base_fname = self.object_properties['guidestar_catalog_id'][i] +\
+                         '_'+str(self.object_properties['int_start'][0]) + '.txt'
+
+            header += '# Guidestar ID: {0:} | RA: {1:.6f}, DEC: {2:.6f}\n'.format(self.object_properties['guidestar_catalog_id'][i], \
+                                                                                 self.object_properties['ra'][i], \
+                                                                                 self.object_properties['dec'][i])
+            if suffix is not None:
+
+                base_fname = suffix + '_' +  base_fname
+
+            header += '# Column 0: Time (JD-2400000.5)\n'
+            header += '# Column 1: Total flux (Counts)\n'
+            
+            if self.gaussfit_results is not None:
+
+                header += '# Column 2: Gaussian Amplitude (counts) \n'
+                header += '# Column 3: Gaussian X location (pix) \n'
+                header += '# Column 4: Gaussian Y location (pix) \n'
+                header += '# Column 5: Gaussian stdev X (pix) \n'
+                header += '# Column 6: Gaussian stdev Y (pix) \n'
+                header += '# Column 7: Gaussian theta (degs)\n'
+                header += '# Column 8: Background counts \n'
+
+            fout = open(self.directory+'/'+base_fname, 'w')
+            fout.write(header)
+
+            for j in range( len(self.fg_time) ):
+
+                if self.gaussfit_results is None:
+
+                    fout.write('{0:.12f} {1:.5f}\n'.format(self.fg_time[j], self.fg_flux[j]))
+
+                else:
+
+                    fout.write('{0:.12f} {1:.5f} {2:.12f} {3:.12f} {4:.12f} {5:.12f} {6:.12f} {7:.12f} {8:.12f}\n'.format(self.fg_time[j], self.fg_flux[j], 
+                                                                                                                   self.gaussfit_results['amplitude'].value[j],
+                                                                                                                   self.gaussfit_results['x_mean'].value[j],
+                                                                                                                   self.gaussfit_results['y_mean'].value[j],
+                                                                                                                   self.gaussfit_results['x_stddev'].value[j],
+                                                                                                                   self.gaussfit_results['y_stddev'].value[j],
+                                                                                                                   self.gaussfit_results['theta'].value[j],
+                                                                                                                   self.gaussfit_results['offset'].value[j]
+                                                                                                                   ))
+
+            fout.close()
```

