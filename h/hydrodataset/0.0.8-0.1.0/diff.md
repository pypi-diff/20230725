# Comparing `tmp/hydrodataset-0.0.8.tar.gz` & `tmp/hydrodataset-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydrodataset-0.0.8.tar", last modified: Sat Oct  8 06:28:28 2022, max compression
+gzip compressed data, was "hydrodataset-0.1.0.tar", last modified: Tue Jul 25 08:13:52 2023, max compression
```

## Comparing `hydrodataset-0.0.8.tar` & `hydrodataset-0.1.0.tar`

### file list

```diff
@@ -1,25 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-08 06:28:28.895756 hydrodataset-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)      161 2022-10-08 06:28:20.000000 hydrodataset-0.0.8/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-10-08 06:28:20.000000 hydrodataset-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      122 2022-10-08 06:28:20.000000 hydrodataset-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     7387 2022-10-08 06:28:28.895756 hydrodataset-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6604 2022-10-08 06:28:20.000000 hydrodataset-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-08 06:28:28.895756 hydrodataset-0.0.8/hydrodataset/
--rw-r--r--   0 runner    (1001) docker     (121)     1782 2022-10-08 06:28:20.000000 hydrodataset-0.0.8/hydrodataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    61079 2022-10-08 06:28:20.000000 hydrodataset-0.0.8/hydrodataset/camels.py
--rw-r--r--   0 runner    (1001) docker     (121)     2530 2022-10-08 06:28:20.000000 hydrodataset-0.0.8/hydrodataset/hydro_dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     2345 2022-10-08 06:28:20.000000 hydrodataset-0.0.8/hydrodataset/hydro_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    14580 2022-10-08 06:28:20.000000 hydrodataset-0.0.8/hydrodataset/lamah.py
--rw-r--r--   0 runner    (1001) docker     (121)    14059 2022-10-08 06:28:20.000000 hydrodataset-0.0.8/hydrodataset/mopex.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-08 06:28:28.895756 hydrodataset-0.0.8/hydrodataset.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7387 2022-10-08 06:28:28.000000 hydrodataset-0.0.8/hydrodataset.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      461 2022-10-08 06:28:28.000000 hydrodataset-0.0.8/hydrodataset.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-10-08 06:28:28.000000 hydrodataset-0.0.8/hydrodataset.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-08 06:28:28.000000 hydrodataset-0.0.8/hydrodataset.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-10-08 06:28:28.000000 hydrodataset-0.0.8/hydrodataset.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-10-08 06:28:28.000000 hydrodataset-0.0.8/hydrodataset.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-10-08 06:28:20.000000 hydrodataset-0.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      454 2022-10-08 06:28:28.899756 hydrodataset-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1774 2022-10-08 06:28:20.000000 hydrodataset-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-08 06:28:28.895756 hydrodataset-0.0.8/test/
--rw-r--r--   0 runner    (1001) docker     (121)     1153 2022-10-08 06:28:20.000000 hydrodataset-0.0.8/test/test_camels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:13:52.463416 hydrodataset-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-25 08:13:38.000000 hydrodataset-0.1.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-25 08:13:38.000000 hydrodataset-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-25 08:13:38.000000 hydrodataset-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8220 2023-07-25 08:13:52.463416 hydrodataset-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7437 2023-07-25 08:13:38.000000 hydrodataset-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:13:52.463416 hydrodataset-0.1.0/hydrodataset/
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-07-25 08:13:38.000000 hydrodataset-0.1.0/hydrodataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61052 2023-07-25 08:13:38.000000 hydrodataset-0.1.0/hydrodataset/camels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-07-25 08:13:38.000000 hydrodataset-0.1.0/hydrodataset/caravan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12823 2023-07-25 08:13:38.000000 hydrodataset-0.1.0/hydrodataset/grdc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-07-25 08:13:38.000000 hydrodataset-0.1.0/hydrodataset/hydro_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-07-25 08:13:38.000000 hydrodataset-0.1.0/hydrodataset/hydro_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-07-25 08:13:38.000000 hydrodataset-0.1.0/hydrodataset/hysets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14604 2023-07-25 08:13:38.000000 hydrodataset-0.1.0/hydrodataset/lamah.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13929 2023-07-25 08:13:38.000000 hydrodataset-0.1.0/hydrodataset/mopex.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39072 2023-07-25 08:13:38.000000 hydrodataset-0.1.0/hydrodataset/multi_datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:13:52.463416 hydrodataset-0.1.0/hydrodataset.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8220 2023-07-25 08:13:52.000000 hydrodataset-0.1.0/hydrodataset.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-25 08:13:52.000000 hydrodataset-0.1.0/hydrodataset.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-25 08:13:52.000000 hydrodataset-0.1.0/hydrodataset.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 08:13:52.000000 hydrodataset-0.1.0/hydrodataset.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-25 08:13:52.000000 hydrodataset-0.1.0/hydrodataset.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-25 08:13:52.000000 hydrodataset-0.1.0/hydrodataset.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-25 08:13:38.000000 hydrodataset-0.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-25 08:13:52.463416 hydrodataset-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-07-25 08:13:38.000000 hydrodataset-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:13:52.463416 hydrodataset-0.1.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-25 08:13:38.000000 hydrodataset-0.1.0/test/test_camels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-07-25 08:13:38.000000 hydrodataset-0.1.0/test/test_caravan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-07-25 08:13:38.000000 hydrodataset-0.1.0/test/test_hysets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5833 2023-07-25 08:13:38.000000 hydrodataset-0.1.0/test/test_multi_datasets.py
```

### Comparing `hydrodataset-0.0.8/LICENSE` & `hydrodataset-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hydrodataset-0.0.8/PKG-INFO` & `hydrodataset-0.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydrodataset
-Version: 0.0.8
+Version: 0.1.0
 Summary: A Python package for downloading and reading hydrological datasets
 Home-page: https://github.com/OuyangWenyu/hydrodataset
 Author: Wenyu Ouyang
 Author-email: wenyuouyang@outlook.com
 License: MIT license
 Keywords: hydrodataset
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -19,15 +19,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 <!--
  * @Author: Wenyu Ouyang
  * @Date: 2021-12-05 22:13:21
- * @LastEditTime: 2022-10-05 18:03:53
+ * @LastEditTime: 2023-07-25 15:13:52
  * @LastEditors: Wenyu Ouyang
  * @Description: README for hydrodataset
  * @FilePath: \hydrodataset\README.md
  * Copyright (c) 2021-2022 Wenyu Ouyang. All rights reserved.
 -->
 # hydrodataset
 
@@ -63,25 +63,28 @@
 pip install hydrodataset
 ```
 
 ## Usage
 
 ### 1. Download datasets
 
-There are many CAMELS datasets, including CAMELS-AUS (Australia), CAMELS-BR (Brazil), CAMELS-CL (Chile), CAMELS-GB (Great Britain), CAMELS-US (United States).
+There are many datasets similar to CAMELS(-US), including CAMELS-AUS (Australia), CAMELS-BR (Brazil), CAMELS-CL (Chile), CAMELS-GB (Great Britain), LamaH-CE, HYSETS. Recently, a new dataset named Caravan is released, which is a global dataset.
 
-Now we only support auto-downloading for CAMELS-US (later for others), but I highly recommend you to download them manually, as the downloading is not stable sometimes because of unstable web connection to the servers of these datasets all over the world.
+Now we only support auto-downloading for CAMELS-US (later for others), but I highly recommend you download them manually, as the downloading is not stable sometimes because of unstable web connections to the servers of these datasets in different places in the world.
 
 the download links:
 
 - [CAMELS-AUS (Australia)](https://doi.pangaea.de/10.1594/PANGAEA.921850)
 - [CAMELS-BR (Brazil)](https://zenodo.org/record/3964745#.YNsjKOgzbIU)
 - [CAMELS-CL (Chile)](https://doi.pangaea.de/10.1594/PANGAEA.894885)
 - [CAMELS-GB (Great Britain)](https://doi.org/10.5285/8344e4f3-d2ea-44f5-8afa-86d2987543a9)
-- [CAMELS-US (United States)](https://gdex.ucar.edu/dataset/camels)
+- [CAMELS-US (United States)](https://gdex.ucar.edu/dataset/camels.html)
+- [LamaH-CE (Central Europe)](https://doi.org/10.5281/zenodo.4525244)
+- [HYSETS (North America)](https://osf.io/rpc3w/#!)
+- [Caravan (Global)](https://zenodo.org/record/7944025)
 
 put these downloaded files in the directory organized as follows:
 
 ```dir
 camels/
 ├─ camels_aus/
 │  ├─ 01_id_name_metadata.zip
@@ -122,22 +125,33 @@
 │  ├─ 9_CAMELScl_tmax_cr2met.zip
 │  ├─ CAMELScl_catchment_boundaries.zip
 ├─ camels_gb/
 │  ├─ 8344e4f3-d2ea-44f5-8afa-86d2987543a9.zip
 ├─ camels_us/
 │  ├─ basin_set_full_res.zip
 │  ├─ basin_timeseries_v1p2_metForcing_obsFlow.zip
+│  ├─ basin_timeseries_v1p2_modelOutput_daymet.zip
+│  ├─ basin_timeseries_v1p2_modelOutput_maurer.zip
+│  ├─ basin_timeseries_v1p2_modelOutput_nldas.zip
 │  ├─ camels_attributes_v2.0.xlsx
 │  ├─ camels_clim.txt
 │  ├─ camels_geol.txt
 │  ├─ camels_hydro.txt
 │  ├─ camels_name.txt
 │  ├─ camels_soil.txt
 │  ├─ camels_topo.txt
 │  ├─ camels_vege.txt
+lamah_ce/
+├─ 2_LamaH-CE_daily
+hysets/
+├─ HYSETS_2020_QC_stations.nc
+├─ HYSETS_watershed_boundaries.zip
+├─ HYSETS_watershed_properties.txt
+caravan/
+├─ Caravan.zip
 ```
 
 ### 2. Run the code
 
 First, run the following Python code:
 
 ```Python
@@ -183,16 +197,19 @@
 HydroDataset is designed to help (1) download, (2) read, (3)format and (4) visualize some datasets through a
 core language (Python) for watershed hydrological modeling.
 
 **Note**: But now this repository is still developing and only supports quite simple functions such as downloading and reading data for watersheds.
 
 Now the dataset zoo list includes:
 
-| **Number** | **Dataset** | **Description**                                         | **Format**        |
-| ---------- | ----------- | ------------------------------------------------------- | ----------------- |
-| 1          | **CAMELS**  | CAMELS series datasets including CAMELS-AUS/BR/CL/GB/US | Dataset Directory |
+| **Number** | **Dataset** | **Description**                                         |
+| ---------- | ----------- | ------------------------------------------------------- |
+| 1          | **CAMELS**  | CAMELS series datasets including CAMELS-AUS/BR/CL/GB/US |
+| 2          | **LamaH**   | LamaH-CE dataset for Central Europe                     |
+| 3          | **HYSETS**  | HYSETS dataset for North America                        |
+| 4          | **Caravan** | Caravan dataset for global                              |
 
 ## Credits
 
 This package was created with [Cookiecutter](https://github.com/cookiecutter/cookiecutter) and the [giswqs/pypackage](https://github.com/giswqs/pypackage) project template.
 
 It was inspired by [HydroData](https://github.com/mikejohnson51/HydroData) and used some tools made by [cheginit](https://github.com/cheginit).
```

### Comparing `hydrodataset-0.0.8/README.md` & `hydrodataset-0.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <!--
  * @Author: Wenyu Ouyang
  * @Date: 2021-12-05 22:13:21
- * @LastEditTime: 2022-10-05 18:03:53
+ * @LastEditTime: 2023-07-25 15:13:52
  * @LastEditors: Wenyu Ouyang
  * @Description: README for hydrodataset
  * @FilePath: \hydrodataset\README.md
  * Copyright (c) 2021-2022 Wenyu Ouyang. All rights reserved.
 -->
 # hydrodataset
 
@@ -41,25 +41,28 @@
 pip install hydrodataset
 ```
 
 ## Usage
 
 ### 1. Download datasets
 
-There are many CAMELS datasets, including CAMELS-AUS (Australia), CAMELS-BR (Brazil), CAMELS-CL (Chile), CAMELS-GB (Great Britain), CAMELS-US (United States).
+There are many datasets similar to CAMELS(-US), including CAMELS-AUS (Australia), CAMELS-BR (Brazil), CAMELS-CL (Chile), CAMELS-GB (Great Britain), LamaH-CE, HYSETS. Recently, a new dataset named Caravan is released, which is a global dataset.
 
-Now we only support auto-downloading for CAMELS-US (later for others), but I highly recommend you to download them manually, as the downloading is not stable sometimes because of unstable web connection to the servers of these datasets all over the world.
+Now we only support auto-downloading for CAMELS-US (later for others), but I highly recommend you download them manually, as the downloading is not stable sometimes because of unstable web connections to the servers of these datasets in different places in the world.
 
 the download links:
 
 - [CAMELS-AUS (Australia)](https://doi.pangaea.de/10.1594/PANGAEA.921850)
 - [CAMELS-BR (Brazil)](https://zenodo.org/record/3964745#.YNsjKOgzbIU)
 - [CAMELS-CL (Chile)](https://doi.pangaea.de/10.1594/PANGAEA.894885)
 - [CAMELS-GB (Great Britain)](https://doi.org/10.5285/8344e4f3-d2ea-44f5-8afa-86d2987543a9)
-- [CAMELS-US (United States)](https://gdex.ucar.edu/dataset/camels)
+- [CAMELS-US (United States)](https://gdex.ucar.edu/dataset/camels.html)
+- [LamaH-CE (Central Europe)](https://doi.org/10.5281/zenodo.4525244)
+- [HYSETS (North America)](https://osf.io/rpc3w/#!)
+- [Caravan (Global)](https://zenodo.org/record/7944025)
 
 put these downloaded files in the directory organized as follows:
 
 ```dir
 camels/
 ├─ camels_aus/
 │  ├─ 01_id_name_metadata.zip
@@ -100,22 +103,33 @@
 │  ├─ 9_CAMELScl_tmax_cr2met.zip
 │  ├─ CAMELScl_catchment_boundaries.zip
 ├─ camels_gb/
 │  ├─ 8344e4f3-d2ea-44f5-8afa-86d2987543a9.zip
 ├─ camels_us/
 │  ├─ basin_set_full_res.zip
 │  ├─ basin_timeseries_v1p2_metForcing_obsFlow.zip
+│  ├─ basin_timeseries_v1p2_modelOutput_daymet.zip
+│  ├─ basin_timeseries_v1p2_modelOutput_maurer.zip
+│  ├─ basin_timeseries_v1p2_modelOutput_nldas.zip
 │  ├─ camels_attributes_v2.0.xlsx
 │  ├─ camels_clim.txt
 │  ├─ camels_geol.txt
 │  ├─ camels_hydro.txt
 │  ├─ camels_name.txt
 │  ├─ camels_soil.txt
 │  ├─ camels_topo.txt
 │  ├─ camels_vege.txt
+lamah_ce/
+├─ 2_LamaH-CE_daily
+hysets/
+├─ HYSETS_2020_QC_stations.nc
+├─ HYSETS_watershed_boundaries.zip
+├─ HYSETS_watershed_properties.txt
+caravan/
+├─ Caravan.zip
 ```
 
 ### 2. Run the code
 
 First, run the following Python code:
 
 ```Python
@@ -161,16 +175,19 @@
 HydroDataset is designed to help (1) download, (2) read, (3)format and (4) visualize some datasets through a
 core language (Python) for watershed hydrological modeling.
 
 **Note**: But now this repository is still developing and only supports quite simple functions such as downloading and reading data for watersheds.
 
 Now the dataset zoo list includes:
 
-| **Number** | **Dataset** | **Description**                                         | **Format**        |
-| ---------- | ----------- | ------------------------------------------------------- | ----------------- |
-| 1          | **CAMELS**  | CAMELS series datasets including CAMELS-AUS/BR/CL/GB/US | Dataset Directory |
+| **Number** | **Dataset** | **Description**                                         |
+| ---------- | ----------- | ------------------------------------------------------- |
+| 1          | **CAMELS**  | CAMELS series datasets including CAMELS-AUS/BR/CL/GB/US |
+| 2          | **LamaH**   | LamaH-CE dataset for Central Europe                     |
+| 3          | **HYSETS**  | HYSETS dataset for North America                        |
+| 4          | **Caravan** | Caravan dataset for global                              |
 
 ## Credits
 
 This package was created with [Cookiecutter](https://github.com/cookiecutter/cookiecutter) and the [giswqs/pypackage](https://github.com/giswqs/pypackage) project template.
 
 It was inspired by [HydroData](https://github.com/mikejohnson51/HydroData) and used some tools made by [cheginit](https://github.com/cheginit).
```

### Comparing `hydrodataset-0.0.8/hydrodataset/camels.py` & `hydrodataset-0.1.0/hydrodataset/camels.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Author: Wenyu Ouyang
 Date: 2022-01-05 18:01:11
-LastEditTime: 2022-10-07 18:37:34
+LastEditTime: 2023-07-16 16:34:22
 LastEditors: Wenyu Ouyang
 Description: Read Camels Series ("AUStralia", "BRazil", "ChiLe", "GreatBritain", "UnitedStates") datasets
 FilePath: \hydrodataset\hydrodataset\camels.py
 Copyright (c) 2021-2022 Wenyu Ouyang. All rights reserved.
 """
 import json
 import warnings
@@ -16,17 +16,16 @@
 from typing import Union
 import pandas as pd
 import numpy as np
 from pandas.core.dtypes.common import is_string_dtype, is_numeric_dtype
 from pathlib import Path
 from urllib.request import urlopen
 from tqdm import tqdm
-from hydrodataset import CACHE_DIR, hydro_utils, HydroDataset
+from hydrodataset import CACHE_DIR, hydro_utils, HydroDataset, CAMELS_REGIONS
 
-CAMELS_REGIONS = ["AUS", "BR", "CL", "GB", "US"]
 CAMELS_NO_DATASET_ERROR_LOG = (
     "We cannot read this dataset now. Please check if you choose correctly:\n"
     + str(CAMELS_REGIONS)
 )
 
 
 def time_intersect_dynamic_data(obs: np.array, date: np.array, t_range: list):
@@ -86,15 +85,15 @@
             raise NotImplementedError(
                 "Please chose one region in: " + str(CAMELS_REGIONS)
             )
         self.region = region
         self.data_source_description = self.set_data_source_describe()
         if download:
             self.download_data_source()
-        self.camels_sites = self.read_site_info()
+        self.sites = self.read_site_info()
 
     def get_name(self):
         return "CAMELS_" + self.region
 
     def set_data_source_describe(self) -> collections.OrderedDict:
         """
         the files in the dataset and their location in file system
@@ -476,15 +475,15 @@
                 data_file = os.path.join(data_folder, "camels_br_" + key + ".txt")
                 data_temp = pd.read_csv(data_file, sep="\s+")
                 var_lst_temp = list(data_temp.columns[1:])
                 var_dict[key] = var_lst_temp
                 var_lst.extend(var_lst_temp)
             return np.array(var_lst)
         elif self.region == "CL":
-            camels_cl_attr_data = self.camels_sites
+            camels_cl_attr_data = self.sites
             # exclude station id
             return camels_cl_attr_data.index.values
         elif self.region == "GB":
             var_dict = dict()
             var_lst = list()
             key_lst = self.data_source_description["CAMELS_ATTR_KEY_LST"]
             for key in key_lst:
@@ -513,30 +512,31 @@
         elif self.region == "AUS":
             forcing_types = []
             for root, dirs, files in os.walk(
                 self.data_source_description["CAMELS_FORCING_DIR"]
             ):
                 if root == self.data_source_description["CAMELS_FORCING_DIR"]:
                     continue
-                for file in files:
-                    forcing_types.append(file[:-4])
+                forcing_types.extend(
+                    file[:-4] for file in files if file != "ClimaticIndices.csv"
+                )
             return np.array(forcing_types)
         elif self.region == "BR":
             return np.array(
                 [
-                    forcing_dir.split(os.sep)[-1][13:]
+                    str(forcing_dir).split(os.sep)[-1][13:]
                     for forcing_dir in self.data_source_description[
                         "CAMELS_FORCING_DIR"
                     ]
                 ]
             )
         elif self.region == "CL":
             return np.array(
                 [
-                    "_".join(forcing_dir.split(os.sep)[-1].split("_")[2:])
+                    "_".join(str(forcing_dir).split(os.sep)[-1].split("_")[2:])
                     for forcing_dir in self.data_source_description[
                         "CAMELS_FORCING_DIR"
                     ]
                 ]
             )
         elif self.region == "GB":
             return np.array(
@@ -576,22 +576,22 @@
                     "streamflow_mmd",
                     "streamflow_QualityCodes",
                 ]
             )
         elif self.region == "BR":
             return np.array(
                 [
-                    flow_dir.split(os.sep)[-1][13:]
+                    str(flow_dir).split(os.sep)[-1][13:]
                     for flow_dir in self.data_source_description["CAMELS_FLOW_DIR"]
                 ]
             )
         elif self.region == "CL":
             return np.array(
                 [
-                    flow_dir.split(os.sep)[-1][11:]
+                    str(flow_dir).split(os.sep)[-1][11:]
                     for flow_dir in self.data_source_description["CAMELS_FLOW_DIR"]
                 ]
             )
         elif self.region == "GB":
             return np.array(["discharge_spec", "discharge_vol"])
         else:
             raise NotImplementedError(CAMELS_NO_DATASET_ERROR_LOG)
@@ -607,19 +607,19 @@
 
         Returns
         -------
         np.array
             gage/station ids
         """
         if self.region in ["BR", "GB", "US"]:
-            return self.camels_sites["gauge_id"].values
+            return self.sites["gauge_id"].values
         elif self.region == "AUS":
-            return self.camels_sites["station_id"].values
+            return self.sites["station_id"].values
         elif self.region == "CL":
-            station_ids = self.camels_sites.columns.values
+            station_ids = self.sites.columns.values
             # for 7-digit id, replace the space with 0 to get a 8-digit id
             cl_station_ids = [
                 station_id.split(" ")[-1].zfill(8) for station_id in station_ids
             ]
             return np.array(cl_station_ids)
         else:
             raise NotImplementedError(CAMELS_NO_DATASET_ERROR_LOG)
@@ -637,15 +637,15 @@
 
         Returns
         -------
         np.array
             streamflow data of one station for a given time range
         """
         logging.debug("reading %s streamflow data before 2015", usgs_id)
-        gage_id_df = self.camels_sites
+        gage_id_df = self.sites
         huc = gage_id_df[gage_id_df["gauge_id"] == usgs_id]["huc_02"].values[0]
         usgs_file = os.path.join(
             self.data_source_description["CAMELS_FLOW_DIR"],
             huc,
             usgs_id + "_streamflow_qc.txt",
         )
         data_temp = pd.read_csv(usgs_file, sep=r"\s+", header=None)
@@ -679,15 +679,15 @@
 
         Returns
         -------
         np.array
             streamflow data of one station for a given time range
         """
         logging.debug("reading %s streamflow data after 2015", usgs_id)
-        gage_id_df = self.camels_sites
+        gage_id_df = self.sites
         huc = gage_id_df[gage_id_df["gauge_id"] == usgs_id]["huc_02"].values[0]
         usgs_file = os.path.join(
             self.data_source_description["CAMELS_FLOW_AFTER2015_DIR"],
             huc,
             usgs_id + "_streamflow_qc.txt",
         )
         data_temp = pd.read_csv(usgs_file, sep=",", header=None, skiprows=1)
@@ -722,17 +722,17 @@
         Returns
         -------
         np.array
             streamflow data of one station for a given time range
         """
         logging.debug("reading %s streamflow data", gage_id)
         dir_ = [
-            flow_dir
+            str(flow_dir)
             for flow_dir in self.data_source_description["CAMELS_FLOW_DIR"]
-            if flow_type in flow_dir
+            if flow_type in str(flow_dir)
         ][0]
         if flow_type == "streamflow_mm_selected_catchments":
             flow_type = "streamflow_mm"
         elif flow_type == "streamflow_simulated":
             flow_type = "simulated_streamflow"
         gage_file = os.path.join(dir_, gage_id + "_" + flow_type + ".txt")
         data_temp = pd.read_csv(gage_file, sep=r"\s+")
@@ -958,15 +958,15 @@
         ]
         if not set(var_lst).issubset(set(model_out_put_var_lst)):
             raise RuntimeError("not in this list")
         nt = t_range_list.shape[0]
         chosen_camels_mods = np.full([len(gage_id_lst), nt, len(var_lst)], np.nan)
         count = 0
         for usgs_id in tqdm(gage_id_lst, desc="Read model output data of CAMELS-US"):
-            gage_id_df = self.camels_sites
+            gage_id_df = self.sites
             huc02_ = gage_id_df[gage_id_df["gauge_id"] == usgs_id]["huc_02"].values[0]
             file_path_dir = os.path.join(
                 self.data_source_dir,
                 "basin_timeseries_v1p2_modelOutput_" + forcing_type,
                 "model_output_" + forcing_type,
                 "model_output",
                 "flow_timeseries",
@@ -1005,15 +1005,15 @@
             chosen_camels_mods[count, ind2, :] = np.mean(result_np, axis=0)
             count = count + 1
         return chosen_camels_mods
 
     def read_forcing_gage(self, usgs_id, var_lst, t_range_list, forcing_type="daymet"):
         # data_source = daymet or maurer or nldas
         logging.debug("reading %s forcing data", usgs_id)
-        gage_id_df = self.camels_sites
+        gage_id_df = self.sites
         huc = gage_id_df[gage_id_df["gauge_id"] == usgs_id]["huc_02"].values[0]
 
         data_folder = self.data_source_description["CAMELS_FORCING_DIR"]
         if forcing_type == "daymet":
             temp_s = "cida"
         else:
             temp_s = forcing_type
@@ -1066,17 +1066,17 @@
 
         Returns
         -------
         np.array
             one type forcing data of a basin in a given time range
         """
         dir_ = [
-            _dir
+            str(_dir)
             for _dir in self.data_source_description["CAMELS_FORCING_DIR"]
-            if var_type in _dir
+            if var_type in str(_dir)
         ][0]
         if var_type in [
             "temperature_min_cpc",
             "temperature_mean_cpc",
             "temperature_max_cpc",
         ]:
             var_type = var_type[:-4]
@@ -1206,15 +1206,15 @@
     def read_attr_all(self):
         data_folder = self.data_source_description["CAMELS_ATTR_DIR"]
         key_lst = self.data_source_description["CAMELS_ATTR_KEY_LST"]
         f_dict = dict()  # factorize dict
         var_dict = dict()
         var_lst = list()
         out_lst = list()
-        gage_dict = self.camels_sites
+        gage_dict = self.sites
         if self.region == "US":
             camels_str = "camels_"
             sep_ = ";"
         elif self.region == "BR":
             camels_str = "camels_br_"
             sep_ = "\s+"
         elif self.region == "GB":
@@ -1409,15 +1409,15 @@
         In addition, we need a document to explain the meaning of all dimensions.
 
         TODO: now only support CAMELS-US
         """
         cache_npy_file = CACHE_DIR.joinpath("camels_daymet_forcing.npy")
         json_file = CACHE_DIR.joinpath("camels_daymet_forcing.json")
         variables = self.get_relevant_cols()
-        basins = self.camels_sites["gauge_id"].values
+        basins = self.sites["gauge_id"].values
         daymet_t_range = ["1980-01-01", "2015-01-01"]
         times = [
             hydro_utils.t2str(tmp)
             for tmp in hydro_utils.t_range_days(daymet_t_range).tolist()
         ]
         data_info = collections.OrderedDict(
             {
@@ -1441,15 +1441,15 @@
         Save all basins' streamflow data in a numpy array file in the cache directory
 
         TODO: now only support CAMELS-US
         """
         cache_npy_file = CACHE_DIR.joinpath("camels_streamflow.npy")
         json_file = CACHE_DIR.joinpath("camels_streamflow.json")
         variables = self.get_target_cols()
-        basins = self.camels_sites["gauge_id"].values
+        basins = self.sites["gauge_id"].values
         t_range = ["1980-01-01", "2015-01-01"]
         times = [
             hydro_utils.t2str(tmp) for tmp in hydro_utils.t_range_days(t_range).tolist()
         ]
         data_info = collections.OrderedDict(
             {
                 "dim": ["basin", "time", "variable"],
```

### Comparing `hydrodataset-0.0.8/hydrodataset/hydro_dataset.py` & `hydrodataset-0.1.0/hydrodataset/hydro_dataset.py`

 * *Files identical despite different names*

### Comparing `hydrodataset-0.0.8/hydrodataset/hydro_utils.py` & `hydrodataset-0.1.0/hydrodataset/hydro_utils.py`

 * *Files identical despite different names*

### Comparing `hydrodataset-0.0.8/hydrodataset/lamah.py` & `hydrodataset-0.1.0/hydrodataset/lamah.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Author: Wenyu Ouyang
 Date: 2022-01-05 18:01:11
-LastEditTime: 2022-09-10 10:38:49
+LastEditTime: 2023-07-16 15:03:22
 LastEditors: Wenyu Ouyang
 Description: Read Camels datasets
 FilePath: \hydrodataset\hydrodataset\lamah.py
 Copyright (c) 2021-2022 Wenyu Ouyang. All rights reserved.
 """
 import collections
 import fnmatch
@@ -13,35 +13,36 @@
 from typing import Union
 import tarfile
 import pandas as pd
 import numpy as np
 from pandas.core.dtypes.common import is_string_dtype, is_numeric_dtype
 from tqdm import tqdm
 
-from hydrodataset import hydro_utils
-from hydrodataset.hydro_dataset import HydroDataset
+from hydrodataset import hydro_utils, HydroDataset
 
 
 class Lamah(HydroDataset):
-    def __init__(self, data_path, download=False):
+    def __init__(self, data_path, download=False, region="CE"):
         """
         Initialization for LamaH-CE dataset
 
         Parameters
         ----------
         data_path
             where we put the dataset
         download
             if true, download
+        region
+            the region of LamaH-CE, now only CE
         """
         super().__init__(data_path)
         self.data_source_description = self.set_data_source_describe()
         if download:
             self.download_data_source()
-        self.camels_sites = self.read_site_info()
+        self.sites = self.read_site_info()
 
     def get_name(self):
         return "LamaH_CE"
 
     def set_data_source_describe(self) -> collections.OrderedDict:
         """
         Introduce the files in the dataset and list their location in the file system
@@ -203,15 +204,15 @@
 
         Returns
         -------
         np.array
             gage/station ids
         """
         # Not all basins have attributes, so we just chose those with attrs
-        ids = self.camels_sites["ID"].values
+        ids = self.sites["ID"].values
         attr_all_file = os.path.join(
             self.data_source_description["CAMELS_ATTR_DIR"],
             "Catchment_attributes.csv",
         )
         attr_data = pd.read_csv(attr_all_file, sep=";")
         # keep consistent with others' data type
         return np.intersect1d(ids, attr_data["ID"].values).astype(str)
```

### Comparing `hydrodataset-0.0.8/hydrodataset/mopex.py` & `hydrodataset-0.1.0/hydrodataset/mopex.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Author: Wenyu Ouyang
 Date: 2022-01-05 18:01:11
-LastEditTime: 2022-09-10 10:38:08
+LastEditTime: 2023-07-16 20:16:58
 LastEditors: Wenyu Ouyang
 Description: Read Camels datasets
 FilePath: \hydrodataset\hydrodataset\mopex.py
 Copyright (c) 2021-2022 Wenyu Ouyang. All rights reserved.
 """
 import collections
 import fnmatch
@@ -77,48 +77,46 @@
         Returns
         -------
         None
         """
         camels_config = self.data_source_description
         for f_name in os.listdir(camels_config["CAMELS_DIR"]):
             if fnmatch.fnmatch(f_name, "*.zip"):
-                unzip_dir = os.path.join(camels_config["CAMELS_DIR"], f_name[0:-4])
+                unzip_dir = os.path.join(camels_config["CAMELS_DIR"], f_name[:-4])
                 file_name = os.path.join(camels_config["CAMELS_DIR"], f_name)
                 hydro_utils.unzip_nested_zip(file_name, unzip_dir)
 
     def read_site_info(self) -> pd.DataFrame:
         """
         Read the basic information of gages in dataset
 
         Returns
         -------
         pd.DataFrame
             basic info of gages
         """
         camels_file = self.data_source_description["CAMELS_GAUGE_FILE"]
-        data = pd.read_excel(camels_file)
-        return data
+        return pd.read_excel(camels_file)
 
     def get_constant_cols(self) -> np.array:
         """
         all readable attrs
 
         Returns
         -------
         np.array
             attribute types
         """
-        data_folder = self.data_source_description["CAMELS_ATTR_DIR"]
         attr_all_file = os.path.join(
             self.data_source_description["CAMELS_DIR"],
             "HYSETS_watershed_properties.txt",
         )
         canopex_attr_indices_data = pd.read_csv(attr_all_file, sep=";")
         # exclude HYSETS watershed id
-        return canopex_attr_indices_data.columns.values[1:]
+        return canopex_attr_indices_data.columns.values[3:]
 
     def get_relevant_cols(self) -> np.array:
         """
         all readable forcing types
 
         Returns
         -------
@@ -212,15 +210,15 @@
         for k in tqdm(range(len(gage_id_lst)), desc="Read streamflow data of CANOPEX"):
             # only one streamflow type: discharge
             canopex_id = self.camels_sites[
                 self.camels_sites["STATION_ID"] == "'" + gage_id_lst[k] + "'"
             ]["CANOPEX_ID"].values[0]
             flow_file = os.path.join(
                 self.data_source_description["CAMELS_FLOW_DIR"],
-                str(canopex_id) + ".dly",
+                f"{str(canopex_id)}.dly",
             )
             read_flow_file = pd.read_csv(flow_file, header=None).values.tolist()
             flow_data = []
             flow_date = []
             for one_site in read_flow_file:
                 flow_date.append(
                     hydro_utils.t2dt(int(one_site[0][:8].replace(" ", "0")))
@@ -268,15 +266,15 @@
 
         for k in tqdm(range(len(gage_id_lst)), desc="Read forcing data of CANOPEX"):
             canopex_id = self.camels_sites[
                 self.camels_sites["STATION_ID"] == "'" + gage_id_lst[k] + "'"
             ]["CANOPEX_ID"].values[0]
             forcing_file = os.path.join(
                 self.data_source_description["CAMELS_FLOW_DIR"],
-                str(canopex_id) + ".dly",
+                f"{str(canopex_id)}.dly",
             )
             read_forcing_file = pd.read_csv(forcing_file, header=None).values.tolist()
 
             forcing_date = []
             for j in range(len(var_lst)):
                 forcing_data = []
                 for one_site in read_forcing_file:
@@ -363,18 +361,15 @@
         attr_all, var_lst_all, var_dict, f_dict = self.read_attr_all_in_one_file()
         ind_var = [var_lst_all.index(var) for var in var_lst]
         id_lst_all = self.read_object_ids()
         # Notice the sequence of station ids ! Some id_lst_all are not sorted, so don't use np.intersect1d
         ind_grid = [id_lst_all.tolist().index(tmp) for tmp in gage_id_lst]
         temp = attr_all[ind_grid, :]
         out = temp[:, ind_var]
-        if is_return_dict:
-            return out, var_dict, f_dict
-        else:
-            return out
+        return (out, var_dict, f_dict) if is_return_dict else out
 
     def read_basin_area(self, object_ids) -> np.array:
         return self.read_constant_cols(
             object_ids, ["Drainage_Area_km2"], is_return_dict=False
         )
 
     def read_mean_prep(self, object_ids) -> np.array:
@@ -382,15 +377,15 @@
         prcp_means = []
         for k in range(len(object_ids)):
             canopex_id = self.camels_sites[
                 self.camels_sites["STATION_ID"] == "'" + object_ids[k] + "'"
             ]["CANOPEX_ID"].values[0]
             forcing_file = os.path.join(
                 self.data_source_description["CAMELS_FLOW_DIR"],
-                str(canopex_id) + ".dly",
+                f"{str(canopex_id)}.dly",
             )
             read_forcing_file = pd.read_csv(forcing_file, header=None).values.tolist()
             prcp_data = []
             for one_site in read_forcing_file:
                 all_data = one_site[0].split(" ")
                 real_data = [one_data for one_data in all_data if one_data != ""]
                 prcp_data.append(float(real_data[-5]))
```

### Comparing `hydrodataset-0.0.8/hydrodataset.egg-info/PKG-INFO` & `hydrodataset-0.1.0/hydrodataset.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydrodataset
-Version: 0.0.8
+Version: 0.1.0
 Summary: A Python package for downloading and reading hydrological datasets
 Home-page: https://github.com/OuyangWenyu/hydrodataset
 Author: Wenyu Ouyang
 Author-email: wenyuouyang@outlook.com
 License: MIT license
 Keywords: hydrodataset
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -19,15 +19,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 <!--
  * @Author: Wenyu Ouyang
  * @Date: 2021-12-05 22:13:21
- * @LastEditTime: 2022-10-05 18:03:53
+ * @LastEditTime: 2023-07-25 15:13:52
  * @LastEditors: Wenyu Ouyang
  * @Description: README for hydrodataset
  * @FilePath: \hydrodataset\README.md
  * Copyright (c) 2021-2022 Wenyu Ouyang. All rights reserved.
 -->
 # hydrodataset
 
@@ -63,25 +63,28 @@
 pip install hydrodataset
 ```
 
 ## Usage
 
 ### 1. Download datasets
 
-There are many CAMELS datasets, including CAMELS-AUS (Australia), CAMELS-BR (Brazil), CAMELS-CL (Chile), CAMELS-GB (Great Britain), CAMELS-US (United States).
+There are many datasets similar to CAMELS(-US), including CAMELS-AUS (Australia), CAMELS-BR (Brazil), CAMELS-CL (Chile), CAMELS-GB (Great Britain), LamaH-CE, HYSETS. Recently, a new dataset named Caravan is released, which is a global dataset.
 
-Now we only support auto-downloading for CAMELS-US (later for others), but I highly recommend you to download them manually, as the downloading is not stable sometimes because of unstable web connection to the servers of these datasets all over the world.
+Now we only support auto-downloading for CAMELS-US (later for others), but I highly recommend you download them manually, as the downloading is not stable sometimes because of unstable web connections to the servers of these datasets in different places in the world.
 
 the download links:
 
 - [CAMELS-AUS (Australia)](https://doi.pangaea.de/10.1594/PANGAEA.921850)
 - [CAMELS-BR (Brazil)](https://zenodo.org/record/3964745#.YNsjKOgzbIU)
 - [CAMELS-CL (Chile)](https://doi.pangaea.de/10.1594/PANGAEA.894885)
 - [CAMELS-GB (Great Britain)](https://doi.org/10.5285/8344e4f3-d2ea-44f5-8afa-86d2987543a9)
-- [CAMELS-US (United States)](https://gdex.ucar.edu/dataset/camels)
+- [CAMELS-US (United States)](https://gdex.ucar.edu/dataset/camels.html)
+- [LamaH-CE (Central Europe)](https://doi.org/10.5281/zenodo.4525244)
+- [HYSETS (North America)](https://osf.io/rpc3w/#!)
+- [Caravan (Global)](https://zenodo.org/record/7944025)
 
 put these downloaded files in the directory organized as follows:
 
 ```dir
 camels/
 ├─ camels_aus/
 │  ├─ 01_id_name_metadata.zip
@@ -122,22 +125,33 @@
 │  ├─ 9_CAMELScl_tmax_cr2met.zip
 │  ├─ CAMELScl_catchment_boundaries.zip
 ├─ camels_gb/
 │  ├─ 8344e4f3-d2ea-44f5-8afa-86d2987543a9.zip
 ├─ camels_us/
 │  ├─ basin_set_full_res.zip
 │  ├─ basin_timeseries_v1p2_metForcing_obsFlow.zip
+│  ├─ basin_timeseries_v1p2_modelOutput_daymet.zip
+│  ├─ basin_timeseries_v1p2_modelOutput_maurer.zip
+│  ├─ basin_timeseries_v1p2_modelOutput_nldas.zip
 │  ├─ camels_attributes_v2.0.xlsx
 │  ├─ camels_clim.txt
 │  ├─ camels_geol.txt
 │  ├─ camels_hydro.txt
 │  ├─ camels_name.txt
 │  ├─ camels_soil.txt
 │  ├─ camels_topo.txt
 │  ├─ camels_vege.txt
+lamah_ce/
+├─ 2_LamaH-CE_daily
+hysets/
+├─ HYSETS_2020_QC_stations.nc
+├─ HYSETS_watershed_boundaries.zip
+├─ HYSETS_watershed_properties.txt
+caravan/
+├─ Caravan.zip
 ```
 
 ### 2. Run the code
 
 First, run the following Python code:
 
 ```Python
@@ -183,16 +197,19 @@
 HydroDataset is designed to help (1) download, (2) read, (3)format and (4) visualize some datasets through a
 core language (Python) for watershed hydrological modeling.
 
 **Note**: But now this repository is still developing and only supports quite simple functions such as downloading and reading data for watersheds.
 
 Now the dataset zoo list includes:
 
-| **Number** | **Dataset** | **Description**                                         | **Format**        |
-| ---------- | ----------- | ------------------------------------------------------- | ----------------- |
-| 1          | **CAMELS**  | CAMELS series datasets including CAMELS-AUS/BR/CL/GB/US | Dataset Directory |
+| **Number** | **Dataset** | **Description**                                         |
+| ---------- | ----------- | ------------------------------------------------------- |
+| 1          | **CAMELS**  | CAMELS series datasets including CAMELS-AUS/BR/CL/GB/US |
+| 2          | **LamaH**   | LamaH-CE dataset for Central Europe                     |
+| 3          | **HYSETS**  | HYSETS dataset for North America                        |
+| 4          | **Caravan** | Caravan dataset for global                              |
 
 ## Credits
 
 This package was created with [Cookiecutter](https://github.com/cookiecutter/cookiecutter) and the [giswqs/pypackage](https://github.com/giswqs/pypackage) project template.
 
 It was inspired by [HydroData](https://github.com/mikejohnson51/HydroData) and used some tools made by [cheginit](https://github.com/cheginit).
```

### Comparing `hydrodataset-0.0.8/setup.py` & `hydrodataset-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,10 +48,10 @@
     keywords='hydrodataset',
     name='hydrodataset',
     packages=find_packages(include=['hydrodataset', 'hydrodataset.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/OuyangWenyu/hydrodataset',
-    version='0.0.8',
+    version='0.1.0',
     zip_safe=False,
 )
```

### Comparing `hydrodataset-0.0.8/test/test_camels.py` & `hydrodataset-0.1.0/test/test_camels.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Author: Wenyu Ouyang
 Date: 2022-09-05 23:20:24
-LastEditTime: 2022-10-05 17:58:41
+LastEditTime: 2023-07-12 20:35:42
 LastEditors: Wenyu Ouyang
 Description: Tests for `hydrodataset` package
-FilePath: \hydrodataset\test\test_camels.py
+FilePath: /hydrodataset/test/test_camels.py
 Copyright (c) 2021-2022 Wenyu Ouyang. All rights reserved.
 """
 import io
 import sys
 import async_retriever as ar
 
 from hydrodataset import CACHE_DIR
```

