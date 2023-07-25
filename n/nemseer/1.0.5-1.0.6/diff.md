# Comparing `tmp/nemseer-1.0.5.tar.gz` & `tmp/nemseer-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nemseer-1.0.5.tar", max compression
+gzip compressed data, was "nemseer-1.0.6.tar", max compression
```

## Comparing `nemseer-1.0.5.tar` & `nemseer-1.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rwxr-xr-x   0        0        0    35150 2023-07-05 04:40:24.529006 nemseer-1.0.5/LICENSE
--rw-r--r--   0        0        0     7930 2023-07-05 04:40:24.529006 nemseer-1.0.5/README.md
--rw-r--r--   0        0        0     2886 2023-07-05 04:40:25.133010 nemseer-1.0.5/pyproject.toml
--rw-r--r--   0        0        0      912 2023-07-05 04:40:25.137010 nemseer-1.0.5/src/nemseer/__init__.py
--rw-r--r--   0        0        0     4706 2023-07-05 04:40:25.137010 nemseer-1.0.5/src/nemseer/data.py
--rw-r--r--   0        0        0    15759 2023-07-05 04:40:25.137010 nemseer-1.0.5/src/nemseer/data_compilers.py
--rw-r--r--   0        0        0     9135 2023-07-05 04:40:25.137010 nemseer-1.0.5/src/nemseer/data_handlers.py
--rw-r--r--   0        0        0    17937 2023-07-05 04:40:25.137010 nemseer-1.0.5/src/nemseer/downloader.py
--rw-r--r--   0        0        0        0 2023-07-05 04:40:25.137010 nemseer-1.0.5/src/nemseer/forecast_type/__init__.py
--rw-r--r--   0        0        0     9275 2023-07-05 04:40:25.137010 nemseer-1.0.5/src/nemseer/forecast_type/run_time_generators.py
--rw-r--r--   0        0        0    13135 2023-07-05 04:40:25.137010 nemseer-1.0.5/src/nemseer/forecast_type/validators.py
--rw-r--r--   0        0        0     7810 2023-07-05 04:40:25.137010 nemseer-1.0.5/src/nemseer/nemseer.py
--rw-r--r--   0        0        0        0 2023-07-05 04:40:25.137010 nemseer-1.0.5/src/nemseer/py.typed
--rw-r--r--   0        0        0    14181 2023-07-05 04:40:25.137010 nemseer-1.0.5/src/nemseer/query.py
--rw-r--r--   0        0        0     8994 1970-01-01 00:00:00.000000 nemseer-1.0.5/PKG-INFO
+-rwxr-xr-x   0        0        0    35150 2023-07-25 06:26:02.221516 nemseer-1.0.6/LICENSE
+-rw-r--r--   0        0        0     7930 2023-07-25 06:26:02.221516 nemseer-1.0.6/README.md
+-rw-r--r--   0        0        0     2813 2023-07-25 06:26:02.853527 nemseer-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0      912 2023-07-25 06:26:02.853527 nemseer-1.0.6/src/nemseer/__init__.py
+-rw-r--r--   0        0        0     4706 2023-07-25 06:26:02.853527 nemseer-1.0.6/src/nemseer/data.py
+-rw-r--r--   0        0        0    15617 2023-07-25 06:26:02.853527 nemseer-1.0.6/src/nemseer/data_compilers.py
+-rw-r--r--   0        0        0     9143 2023-07-25 06:26:02.853527 nemseer-1.0.6/src/nemseer/data_handlers.py
+-rw-r--r--   0        0        0    17937 2023-07-25 06:26:02.853527 nemseer-1.0.6/src/nemseer/downloader.py
+-rw-r--r--   0        0        0        0 2023-07-25 06:26:02.853527 nemseer-1.0.6/src/nemseer/forecast_type/__init__.py
+-rw-r--r--   0        0        0     9275 2023-07-25 06:26:02.853527 nemseer-1.0.6/src/nemseer/forecast_type/run_time_generators.py
+-rw-r--r--   0        0        0    13135 2023-07-25 06:26:02.853527 nemseer-1.0.6/src/nemseer/forecast_type/validators.py
+-rw-r--r--   0        0        0     7810 2023-07-25 06:26:02.853527 nemseer-1.0.6/src/nemseer/nemseer.py
+-rw-r--r--   0        0        0        0 2023-07-25 06:26:02.853527 nemseer-1.0.6/src/nemseer/py.typed
+-rw-r--r--   0        0        0    14181 2023-07-25 06:26:02.853527 nemseer-1.0.6/src/nemseer/query.py
+-rw-r--r--   0        0        0     8906 1970-01-01 00:00:00.000000 nemseer-1.0.6/PKG-INFO
```

### Comparing `nemseer-1.0.5/LICENSE` & `nemseer-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nemseer-1.0.5/README.md` & `nemseer-1.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -25,19 +25,19 @@
 
 Whereas PASA processes are primarily used to assess resource adequacy based on technical inputs and assumptions for resources in the market (i.e. used to answer questions such as *"can operational demand be met in the forecast horizon with a sufficient safety (reserve) margin?"*), pre-dispatch processes incorporate the latest set of market participant offers and thus produce regional prices forecasts for energy and frequency control ancillary services [(FCAS)](https://aemo.com.au/-/media/files/electricity/nem/security_and_reliability/ancillary_services/guide-to-ancillary-services-in-the-national-electricity-market.pdf). Overviews of the various pre-dispatch and PASA processes can be found in the [glossary](https://nemseer.readthedocs.io/en/latest/glossary.html).
 
 [^1]: We use the term *"forecast"* loosely, especially given that these *"forecasts"* change once participants update offer information (e.g. through rebidding) or submit revised resource availabilities and energy constraints. Both of these are intended outcomes of these *"ahead processes"*, which are run to provide system and market information to participants to inform their decision-making. However, to avoid confusion and to ensure consistency with the language used by AEMO, we use the terms *"forecast"* (or outputs) and *"forecast types"* (or ahead processes) in `nemseer`.
 
 `nemseer` enables you to download and work with data for the following forecast types. Where available, AEMO process and table descriptions are linked:
 
-1. 5-minute pre-dispatch (`P5MIN`: [Table descriptions](https://nemweb.com.au/Reports/Current/MMSDataModelReport/Electricity/MMS%20Data%20Model%20Report_files/MMS_222.htm#1))
-2. [Pre-dispatch](https://www.aemo.com.au/-/media/files/electricity/nem/security_and_reliability/power_system_ops/procedures/so_op_3704-predispatch.pdf?la=en) (`PREDISPATCH`: [Table descriptions](https://nemweb.com.au/Reports/Current/MMSDataModelReport/Electricity/MMS%20Data%20Model%20Report_files/MMS_260.htm#1))
-3. Pre-dispatch Projected Assessment of System Adequacy (`PDPASA`: [Tables and Descriptions](https://nemweb.com.au/Reports/Current/MMSDataModelReport/Electricity/MMS%20Data%20Model%20Report_files/MMS_467.htm#1))
-4. [Short Term Projected Assessment of System Adequacy](https://wa.aemo.com.au/-/media/files/electricity/nem/planning_and_forecasting/pasa/stpasa-process-description.pdf) (`STPASA`: [Table descriptions](https://nemweb.com.au/Reports/Current/MMSDataModelReport/Electricity/MMS%20Data%20Model%20Report_files/MMS_335.htm#1))
-5. [Medium Term Projected Assessment of System Adequacy](https://wa.aemo.com.au/-/media/files/electricity/nem/planning_and_forecasting/pasa/mt-pasa-process-description-v62.pdf?la=en) (`MTPASA`: [Table descriptions](https://nemweb.com.au/Reports/Current/MMSDataModelReport/Electricity/MMS%20Data%20Model%20Report_files/MMS_210.htm#1))
+1. 5-minute pre-dispatch (`P5MIN`: [Table descriptions](https://nemweb.com.au/Reports/Current/MMSDataModelReport/Electricity/MMS%20Data%20Model%20Report_files/MMS_231.htm#1))
+2. [Pre-dispatch](https://www.aemo.com.au/-/media/files/electricity/nem/security_and_reliability/power_system_ops/procedures/so_op_3704-predispatch.pdf?la=en) (`PREDISPATCH`: [Table descriptions](https://nemweb.com.au/Reports/Current/MMSDataModelReport/Electricity/MMS%20Data%20Model%20Report_files/MMS_272.htm#1))
+3. Pre-dispatch Projected Assessment of System Adequacy (`PDPASA`: [Tables and Descriptions](https://nemweb.com.au/Reports/Current/MMSDataModelReport/Electricity/MMS%20Data%20Model%20Report_files/MMS_481.htm#1))
+4. [Short Term Projected Assessment of System Adequacy](https://wa.aemo.com.au/-/media/files/electricity/nem/planning_and_forecasting/pasa/stpasa-process-description.pdf) (`STPASA`: [Table descriptions](https://nemweb.com.au/Reports/Current/MMSDataModelReport/Electricity/MMS%20Data%20Model%20Report_files/MMS_349.htm#1))
+5. [Medium Term Projected Assessment of System Adequacy](https://wa.aemo.com.au/-/media/files/electricity/nem/planning_and_forecasting/pasa/mt-pasa-process-description-v62.pdf?la=en) (`MTPASA`: [Table descriptions](https://nemweb.com.au/Reports/Current/MMSDataModelReport/Electricity/MMS%20Data%20Model%20Report_files/MMS_219.htm#1))
 
 Another helpful reference for PASA information is AEMO's [Reliability Standard Implementation Guidelines](https://www.aemo.com.au/-/media/files/electricity/nem/planning_and_forecasting/rsig/reliability-standard-implementation-guidelines.pdf?la=en).
 
 ### ST PASA Replacement Project
 
 Note that the methodologies for PD PASA and ST PASA are being reviewed by AEMO. In particular, the ST PASA Replacement project will combine PD PASA and ST PASA into ST PASA. For more detail, refer to the [final determination of the rule change](https://www.aemc.gov.au/sites/default/files/2022-05/ERC0332%20-%20Updating%20Short%20Term%20PASA%20-%20Final%20determination.pdf) and the [AEMO ST PASA Replacement Project home page](https://aemo.com.au/en/initiatives/trials-and-initiatives/st-pasa-replacement-project).
```

### Comparing `nemseer-1.0.5/pyproject.toml` & `nemseer-1.0.6/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 [tool.poetry]
 name = "nemseer"
-version = "1.0.5"
+version = "1.0.6"
 description = "A package for downloading and handling forecasts for the National Electricity Market (NEM) from the Australian Energy Market Operator (AEMO)."
 authors = ["Abhijith Prakash"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 
 # Main dependencies for the package via poetry. Package users will need these dependencies.
 [tool.poetry.dependencies]
-python = ">= 3.8,<3.12"
-attrs = "^21.3.0"
-beautifulsoup4 = "^4"
-netCDF4 = "^1.6.0"
-numpy = "^1.23.0"
+python = ">=3.8,<3.12"
+attrs = "^21"
+beautifulsoup4 = "*"
+netCDF4 = "^1"
+numpy = "*"
 packaging = "^21.3"
-pandas = "^1.2"
-psutil = "^5.9.1"
+pandas = "*"
+psutil = "^5"
 pyarrow = "*"
 requests = "^2"
-tqdm = "^4.64.0"
-xarray = "^2022"
+tqdm = "^4"
+xarray = "*"
 
 # Packages for developers for creating documentation
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 # MyST parser for Sphinx documentation with furo theme
-Sphinx = "^5.0.2"
-furo = "^2022.6.21"
-myst-parser = "^0.18.0"
-sphinx-copybutton = "^0.5.0"
+Sphinx = "^5"
+furo = "*"
+myst-parser = "*"
+sphinx-copybutton = "*"
 # The packages below are required for compiling example notebooks
 jupyter = "^1.0.0"
 notebook = "^6.4.12"
 myst-nb = "^0.16.0"
-matplotlib = "^3.5.3"
-plotly = "^5.10.0"
-kaleido = "0.2.1"
-hvplot = "^0.8.1"
-nemosis = "^3.2.0"
+matplotlib = "^3"
+plotly = "^5"
+kaleido = "0.2"
+hvplot = "^0.8"
+nemosis = "^3"
 
 
 # Packages for developers for debugging
 [tool.poetry.group.debug]
 optional = true
 
 [tool.poetry.group.debug.dependencies]
@@ -73,15 +73,15 @@
 # Packages for developers for testing
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
 # pytest and pytest-cov for coverage
 pytest = "^7"
-pytest-cov = "^3"
+pytest-cov = "^4"
 grequests = "^0.6.0"
 pytest-mock = "^3.8.2"
 
 # Config for pytest and pytest-cov
 [tool.pytest.ini_options]
 # path to tests for pytest
 testpaths = ["tests"]
```

### Comparing `nemseer-1.0.5/src/nemseer/__init__.py` & `nemseer-1.0.6/src/nemseer/__init__.py`

 * *Files identical despite different names*

### Comparing `nemseer-1.0.5/src/nemseer/data.py` & `nemseer-1.0.6/src/nemseer/data.py`

 * *Files identical despite different names*

### Comparing `nemseer-1.0.5/src/nemseer/data_compilers.py` & `nemseer-1.0.6/src/nemseer/data_compilers.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,25 +147,25 @@
             raw_tables = tables
         for ftype in ENUMERATED_TABLES:
             if query.forecast_type == ftype:
                 for table, enumerate_to in ENUMERATED_TABLES[ftype]:
                     if table in raw_tables:
                         tables = _enumerate_tables(tables, table, enumerate_to)
         return cls(
-            run_start=query.run_start,
-            run_end=query.run_end,
-            forecasted_start=query.forecasted_start,
-            forecasted_end=query.forecasted_end,
-            forecast_type=query.forecast_type,
-            metadata=query.metadata,
-            raw_cache=query.raw_cache,
-            processed_cache=query.processed_cache,
-            processed_queries=query.processed_queries,
-            raw_tables=raw_tables,
-            compiled_data=None,
+            query.run_start,
+            query.run_end,
+            query.forecasted_start,
+            query.forecasted_end,
+            query.forecast_type,
+            query.metadata,
+            query.raw_cache,
+            query.processed_cache,
+            query.processed_queries,
+            raw_tables,
+            None,
         )
 
     def invalid_or_corrupted_files(self) -> List[str]:
         """A list of invalid/corrupted files as per files in `.invalid_aemo_files.txt`.
         Returns an empty list if the stubfile does not exist.
         """
         invalid_or_corrupted_stubfile = self.raw_cache / Path(INVALID_STUBS_FILE)
```

### Comparing `nemseer-1.0.5/src/nemseer/data_handlers.py` & `nemseer-1.0.6/src/nemseer/data_handlers.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         :class:`pandas.DataFrame` with datetime columns converted according to standard
         AEMO
         format
     """
     dt_cols = DATETIME_COLS
     dt_cols_present = dt_cols.intersection(set(df.columns.tolist()))
     for col in dt_cols_present:
-        df.loc[:, col] = pd.to_datetime(df[col], format=DATETIME_FORMAT)
+        df.loc[:, col] = pd.to_datetime(df[col], format=DATETIME_FORMAT + ":%S")
     return df
 
 
 def _parse_id_cols(df: pd.DataFrame) -> pd.DataFrame:
     """Finds relevant ID columns in the DataFrame and converts them to categories
 
     Args:
```

### Comparing `nemseer-1.0.5/src/nemseer/downloader.py` & `nemseer-1.0.6/src/nemseer/downloader.py`

 * *Files identical despite different names*

### Comparing `nemseer-1.0.5/src/nemseer/forecast_type/run_time_generators.py` & `nemseer-1.0.6/src/nemseer/forecast_type/run_time_generators.py`

 * *Files identical despite different names*

### Comparing `nemseer-1.0.5/src/nemseer/forecast_type/validators.py` & `nemseer-1.0.6/src/nemseer/forecast_type/validators.py`

 * *Files identical despite different names*

### Comparing `nemseer-1.0.5/src/nemseer/nemseer.py` & `nemseer-1.0.6/src/nemseer/nemseer.py`

 * *Files identical despite different names*

### Comparing `nemseer-1.0.5/src/nemseer/query.py` & `nemseer-1.0.6/src/nemseer/query.py`

 * *Files identical despite different names*

### Comparing `nemseer-1.0.5/PKG-INFO` & `nemseer-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: nemseer
-Version: 1.0.5
+Version: 1.0.6
 Summary: A package for downloading and handling forecasts for the National Electricity Market (NEM) from the Australian Energy Market Operator (AEMO).
 License: GPL-3.0-or-later
 Author: Abhijith Prakash
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: attrs (>=21.3.0,<22.0.0)
-Requires-Dist: beautifulsoup4 (>=4,<5)
-Requires-Dist: netCDF4 (>=1.6.0,<2.0.0)
-Requires-Dist: numpy (>=1.23.0,<2.0.0)
+Requires-Dist: attrs (>=21,<22)
+Requires-Dist: beautifulsoup4
+Requires-Dist: netCDF4 (>=1,<2)
+Requires-Dist: numpy
 Requires-Dist: packaging (>=21.3,<22.0)
-Requires-Dist: pandas (>=1.2,<2.0)
-Requires-Dist: psutil (>=5.9.1,<6.0.0)
+Requires-Dist: pandas
+Requires-Dist: psutil (>=5,<6)
 Requires-Dist: pyarrow
 Requires-Dist: requests (>=2,<3)
-Requires-Dist: tqdm (>=4.64.0,<5.0.0)
-Requires-Dist: xarray (>=2022,<2023)
+Requires-Dist: tqdm (>=4,<5)
+Requires-Dist: xarray
 Description-Content-Type: text/markdown
 
 # nemseer
 
 [![PyPI version](https://badge.fury.io/py/nemseer.svg)](https://badge.fury.io/py/nemseer)
 [![Continuous Integration and Deployment](https://github.com/UNSW-CEEM/NEMSEER/actions/workflows/cicd.yml/badge.svg)](https://github.com/UNSW-CEEM/NEMSEER/actions/workflows/cicd.yml)
 [![Documentation Status](https://readthedocs.org/projects/nemseer/badge/?version=latest)](https://nemseer.readthedocs.io/en/latest/?badge=latest)
@@ -51,19 +51,19 @@
 
 Whereas PASA processes are primarily used to assess resource adequacy based on technical inputs and assumptions for resources in the market (i.e. used to answer questions such as *"can operational demand be met in the forecast horizon with a sufficient safety (reserve) margin?"*), pre-dispatch processes incorporate the latest set of market participant offers and thus produce regional prices forecasts for energy and frequency control ancillary services [(FCAS)](https://aemo.com.au/-/media/files/electricity/nem/security_and_reliability/ancillary_services/guide-to-ancillary-services-in-the-national-electricity-market.pdf). Overviews of the various pre-dispatch and PASA processes can be found in the [glossary](https://nemseer.readthedocs.io/en/latest/glossary.html).
 
 [^1]: We use the term *"forecast"* loosely, especially given that these *"forecasts"* change once participants update offer information (e.g. through rebidding) or submit revised resource availabilities and energy constraints. Both of these are intended outcomes of these *"ahead processes"*, which are run to provide system and market information to participants to inform their decision-making. However, to avoid confusion and to ensure consistency with the language used by AEMO, we use the terms *"forecast"* (or outputs) and *"forecast types"* (or ahead processes) in `nemseer`.
 
 `nemseer` enables you to download and work with data for the following forecast types. Where available, AEMO process and table descriptions are linked:
 
-1. 5-minute pre-dispatch (`P5MIN`: [Table descriptions](https://nemweb.com.au/Reports/Current/MMSDataModelReport/Electricity/MMS%20Data%20Model%20Report_files/MMS_222.htm#1))
-2. [Pre-dispatch](https://www.aemo.com.au/-/media/files/electricity/nem/security_and_reliability/power_system_ops/procedures/so_op_3704-predispatch.pdf?la=en) (`PREDISPATCH`: [Table descriptions](https://nemweb.com.au/Reports/Current/MMSDataModelReport/Electricity/MMS%20Data%20Model%20Report_files/MMS_260.htm#1))
-3. Pre-dispatch Projected Assessment of System Adequacy (`PDPASA`: [Tables and Descriptions](https://nemweb.com.au/Reports/Current/MMSDataModelReport/Electricity/MMS%20Data%20Model%20Report_files/MMS_467.htm#1))
-4. [Short Term Projected Assessment of System Adequacy](https://wa.aemo.com.au/-/media/files/electricity/nem/planning_and_forecasting/pasa/stpasa-process-description.pdf) (`STPASA`: [Table descriptions](https://nemweb.com.au/Reports/Current/MMSDataModelReport/Electricity/MMS%20Data%20Model%20Report_files/MMS_335.htm#1))
-5. [Medium Term Projected Assessment of System Adequacy](https://wa.aemo.com.au/-/media/files/electricity/nem/planning_and_forecasting/pasa/mt-pasa-process-description-v62.pdf?la=en) (`MTPASA`: [Table descriptions](https://nemweb.com.au/Reports/Current/MMSDataModelReport/Electricity/MMS%20Data%20Model%20Report_files/MMS_210.htm#1))
+1. 5-minute pre-dispatch (`P5MIN`: [Table descriptions](https://nemweb.com.au/Reports/Current/MMSDataModelReport/Electricity/MMS%20Data%20Model%20Report_files/MMS_231.htm#1))
+2. [Pre-dispatch](https://www.aemo.com.au/-/media/files/electricity/nem/security_and_reliability/power_system_ops/procedures/so_op_3704-predispatch.pdf?la=en) (`PREDISPATCH`: [Table descriptions](https://nemweb.com.au/Reports/Current/MMSDataModelReport/Electricity/MMS%20Data%20Model%20Report_files/MMS_272.htm#1))
+3. Pre-dispatch Projected Assessment of System Adequacy (`PDPASA`: [Tables and Descriptions](https://nemweb.com.au/Reports/Current/MMSDataModelReport/Electricity/MMS%20Data%20Model%20Report_files/MMS_481.htm#1))
+4. [Short Term Projected Assessment of System Adequacy](https://wa.aemo.com.au/-/media/files/electricity/nem/planning_and_forecasting/pasa/stpasa-process-description.pdf) (`STPASA`: [Table descriptions](https://nemweb.com.au/Reports/Current/MMSDataModelReport/Electricity/MMS%20Data%20Model%20Report_files/MMS_349.htm#1))
+5. [Medium Term Projected Assessment of System Adequacy](https://wa.aemo.com.au/-/media/files/electricity/nem/planning_and_forecasting/pasa/mt-pasa-process-description-v62.pdf?la=en) (`MTPASA`: [Table descriptions](https://nemweb.com.au/Reports/Current/MMSDataModelReport/Electricity/MMS%20Data%20Model%20Report_files/MMS_219.htm#1))
 
 Another helpful reference for PASA information is AEMO's [Reliability Standard Implementation Guidelines](https://www.aemo.com.au/-/media/files/electricity/nem/planning_and_forecasting/rsig/reliability-standard-implementation-guidelines.pdf?la=en).
 
 ### ST PASA Replacement Project
 
 Note that the methodologies for PD PASA and ST PASA are being reviewed by AEMO. In particular, the ST PASA Replacement project will combine PD PASA and ST PASA into ST PASA. For more detail, refer to the [final determination of the rule change](https://www.aemc.gov.au/sites/default/files/2022-05/ERC0332%20-%20Updating%20Short%20Term%20PASA%20-%20Final%20determination.pdf) and the [AEMO ST PASA Replacement Project home page](https://aemo.com.au/en/initiatives/trials-and-initiatives/st-pasa-replacement-project).
```

