# Comparing `tmp/tidychef-0.1.0.tar.gz` & `tmp/tidychef-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tidychef-0.1.0.tar", max compression
+gzip compressed data, was "tidychef-0.1.1.tar", max compression
```

## Comparing `tidychef-0.1.0.tar` & `tidychef-0.1.1.tar`

### file list

```diff
@@ -1,87 +1,88 @@
--rw-r--r--   0        0        0     1127 2023-07-24 18:12:06.786912 tidychef-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      245 2023-07-25 07:54:18.333658 tidychef-0.1.0/tidychef/__init__.py
--rw-r--r--   0        0        0      110 2023-07-05 08:30:04.083380 tidychef-0.1.0/tidychef/acquire/__init__.py
--rw-r--r--   0        0        0      520 2023-07-24 18:04:58.226769 tidychef-0.1.0/tidychef/acquire/base.py
--rw-r--r--   0        0        0      133 2023-06-28 13:56:49.387210 tidychef-0.1.0/tidychef/acquire/csv/__init__.py
--rw-r--r--   0        0        0     3402 2023-07-25 07:42:58.792065 tidychef-0.1.0/tidychef/acquire/csv/http_implemented.py
--rw-r--r--   0        0        0     3036 2023-07-25 07:43:33.075028 tidychef-0.1.0/tidychef/acquire/csv/local_implemented.py
--rw-r--r--   0        0        0     2455 2023-07-25 07:45:41.458935 tidychef-0.1.0/tidychef/acquire/main.py
--rw-r--r--   0        0        0      163 2023-07-23 15:42:10.265499 tidychef-0.1.0/tidychef/acquire/python/__init__.py
--rw-r--r--   0        0        0     2467 2023-07-25 07:43:28.624238 tidychef-0.1.0/tidychef/acquire/python/listoflists_implemented.py
--rw-r--r--   0        0        0     2851 2023-07-25 07:44:03.424136 tidychef-0.1.0/tidychef/acquire/python/pipetable_implemented.py
--rw-r--r--   0        0        0      133 2023-06-28 14:19:41.973466 tidychef-0.1.0/tidychef/acquire/xls/__init__.py
--rw-r--r--   0        0        0     4258 2023-07-25 07:44:26.721737 tidychef-0.1.0/tidychef/acquire/xls/http_implemented.py
--rw-r--r--   0        0        0     3345 2023-07-25 07:44:39.053004 tidychef-0.1.0/tidychef/acquire/xls/local_implemented.py
--rw-r--r--   0        0        0      134 2023-06-28 13:56:49.375947 tidychef-0.1.0/tidychef/acquire/xlsx/__init__.py
--rw-r--r--   0        0        0     4372 2023-07-25 07:44:56.396637 tidychef-0.1.0/tidychef/acquire/xlsx/http_implemented.py
--rw-r--r--   0        0        0     3662 2023-07-25 07:45:08.699028 tidychef-0.1.0/tidychef/acquire/xlsx/local_implemented.py
--rw-r--r--   0        0        0      149 2023-07-23 17:11:06.781553 tidychef-0.1.0/tidychef/against/__init__.py
--rw-r--r--   0        0        0        0 2023-07-11 20:08:08.429121 tidychef-0.1.0/tidychef/against/implementations/__init__.py
--rw-r--r--   0        0        0      638 2023-07-25 07:23:52.963306 tidychef-0.1.0/tidychef/against/implementations/base.py
--rw-r--r--   0        0        0     1163 2023-07-25 07:25:47.995142 tidychef-0.1.0/tidychef/against/implementations/items.py
--rw-r--r--   0        0        0     2401 2023-07-25 07:25:53.424611 tidychef-0.1.0/tidychef/against/implementations/length.py
--rw-r--r--   0        0        0     3572 2023-07-25 07:25:36.472780 tidychef-0.1.0/tidychef/against/implementations/numeric.py
--rw-r--r--   0        0        0     1120 2023-07-25 07:26:23.342013 tidychef-0.1.0/tidychef/against/implementations/regex.py
--rw-r--r--   0        0        0     1766 2023-07-25 07:47:12.734570 tidychef-0.1.0/tidychef/against/wrapper.py
--rw-r--r--   0        0        0       48 2023-05-28 22:18:13.690464 tidychef-0.1.0/tidychef/column/__init__.py
--rw-r--r--   0        0        0     2970 2023-07-25 07:46:59.116780 tidychef-0.1.0/tidychef/column/base.py
--rw-r--r--   0        0        0     4995 2023-07-25 07:47:30.656866 tidychef-0.1.0/tidychef/column/column.py
--rw-r--r--   0        0        0      527 2023-06-27 16:25:09.098617 tidychef-0.1.0/tidychef/datafuncs/README.md
--rw-r--r--   0        0        0     1075 2023-07-23 17:11:06.809528 tidychef-0.1.0/tidychef/datafuncs/__init__.py
--rw-r--r--   0        0        0     8878 2023-07-24 18:03:57.415174 tidychef-0.1.0/tidychef/datafuncs/common.py
--rw-r--r--   0        0        0     5639 2023-07-24 18:03:55.736608 tidychef-0.1.0/tidychef/datafuncs/excel.py
--rw-r--r--   0        0        0     6119 2023-07-24 18:03:54.264597 tidychef-0.1.0/tidychef/datafuncs/ordering.py
--rw-r--r--   0        0        0      453 2023-05-24 09:26:45.996492 tidychef-0.1.0/tidychef/direction/README.md
--rw-r--r--   0        0        0       60 2023-07-12 10:33:30.217649 tidychef-0.1.0/tidychef/direction/__init__.py
--rw-r--r--   0        0        0     4803 2023-07-24 18:03:49.931406 tidychef-0.1.0/tidychef/direction/directions.py
--rw-r--r--   0        0        0      885 2023-07-23 17:11:06.805910 tidychef-0.1.0/tidychef/exceptions/__init__.py
--rw-r--r--   0        0        0     2150 2023-07-23 13:37:16.866495 tidychef-0.1.0/tidychef/exceptions/badparams.py
--rw-r--r--   0        0        0      777 2023-07-23 17:10:30.841539 tidychef-0.1.0/tidychef/exceptions/cells.py
--rw-r--r--   0        0        0     3408 2023-07-23 17:10:20.538378 tidychef-0.1.0/tidychef/exceptions/common.py
--rw-r--r--   0        0        0      652 2023-07-12 12:23:20.039435 tidychef-0.1.0/tidychef/exceptions/lookups.py
--rw-r--r--   0        0        0        0 2023-07-12 13:26:57.378906 tidychef-0.1.0/tidychef/lookup/__init__.py
--rw-r--r--   0        0        0      447 2023-07-24 18:03:47.784091 tidychef-0.1.0/tidychef/lookup/base.py
--rw-r--r--   0        0        0        0 2023-05-26 13:52:55.388417 tidychef-0.1.0/tidychef/lookup/engines/README.md
--rw-r--r--   0        0        0        0 2023-06-14 15:18:13.870543 tidychef-0.1.0/tidychef/lookup/engines/__init__.py
--rw-r--r--   0        0        0    13681 2023-07-25 07:48:25.203597 tidychef-0.1.0/tidychef/lookup/engines/closest.py
--rw-r--r--   0        0        0      957 2023-07-24 18:03:44.342917 tidychef-0.1.0/tidychef/lookup/engines/constant.py
--rw-r--r--   0        0        0     6129 2023-07-25 07:48:38.777076 tidychef-0.1.0/tidychef/lookup/engines/direct.py
--rw-r--r--   0        0        0     4049 2023-07-25 07:48:47.404609 tidychef-0.1.0/tidychef/lookup/engines/horizontal_condition.py
--rw-r--r--   0        0        0    10700 2023-07-25 07:49:00.642629 tidychef-0.1.0/tidychef/lookup/engines/within.py
--rw-r--r--   0        0        0       21 2023-05-24 09:26:45.998537 tidychef-0.1.0/tidychef/models/__init__.py
--rw-r--r--   0        0        0        0 2023-05-24 09:26:46.000263 tidychef-0.1.0/tidychef/models/source/__init__.py
--rw-r--r--   0        0        0     6999 2023-07-25 07:49:30.892006 tidychef-0.1.0/tidychef/models/source/cell.py
--rw-r--r--   0        0        0       77 2023-05-24 09:26:46.000543 tidychef-0.1.0/tidychef/models/source/cellformat.py
--rw-r--r--   0        0        0     7762 2023-07-25 07:49:40.728144 tidychef-0.1.0/tidychef/models/source/table.py
--rw-r--r--   0        0        0       39 2023-06-20 17:35:02.406176 tidychef-0.1.0/tidychef/notebook/__init__.py
--rw-r--r--   0        0        0      465 2023-07-16 10:09:55.515709 tidychef-0.1.0/tidychef/notebook/ipython.py
--rw-r--r--   0        0        0        0 2023-06-17 11:41:28.459219 tidychef-0.1.0/tidychef/notebook/preview/__init__.py
--rw-r--r--   0        0        0     3778 2023-07-25 07:51:24.701683 tidychef-0.1.0/tidychef/notebook/preview/boundary.py
--rw-r--r--   0        0        0     2910 2023-07-25 07:50:26.281679 tidychef-0.1.0/tidychef/notebook/preview/html/components.py
--rw-r--r--   0        0        0      651 2023-07-14 22:09:11.515526 tidychef-0.1.0/tidychef/notebook/preview/html/constants.py
--rw-r--r--   0        0        0     2616 2023-07-25 07:50:37.866855 tidychef-0.1.0/tidychef/notebook/preview/html/main.py
--rw-r--r--   0        0        0     4869 2023-07-25 07:50:58.627598 tidychef-0.1.0/tidychef/notebook/preview/html/table.py
--rw-r--r--   0        0        0      926 2023-07-16 14:00:02.838338 tidychef-0.1.0/tidychef/notebook/preview/html/tidy_data.py
--rw-r--r--   0        0        0       59 2023-07-12 10:33:30.001045 tidychef-0.1.0/tidychef/output/__init__.py
--rw-r--r--   0        0        0      561 2023-06-16 19:33:30.841073 tidychef-0.1.0/tidychef/output/base.py
--rw-r--r--   0        0        0    14254 2023-07-25 07:52:00.465984 tidychef-0.1.0/tidychef/output/tidydata.py
--rw-r--r--   0        0        0      459 2023-06-27 16:24:57.036542 tidychef-0.1.0/tidychef/selection/README.md
--rw-r--r--   0        0        0      143 2023-07-12 10:33:30.114915 tidychef-0.1.0/tidychef/selection/__init__.py
--rw-r--r--   0        0        0      153 2023-07-24 18:06:08.468256 tidychef-0.1.0/tidychef/selection/csv/csv.py
--rw-r--r--   0        0        0     2022 2023-06-27 16:25:30.891041 tidychef-0.1.0/tidychef/selection/filters/README.md
--rw-r--r--   0        0        0      196 2023-07-17 15:19:20.512477 tidychef-0.1.0/tidychef/selection/filters/__init__.py
--rw-r--r--   0        0        0     1388 2023-07-24 18:06:42.658006 tidychef-0.1.0/tidychef/selection/filters/common.py
--rw-r--r--   0        0        0    28752 2023-07-25 07:58:50.258318 tidychef-0.1.0/tidychef/selection/selectable.py
--rw-r--r--   0        0        0      132 2023-06-28 16:12:18.376303 tidychef-0.1.0/tidychef/selection/xls/xls.py
--rw-r--r--   0        0        0      134 2023-06-28 16:11:52.808553 tidychef-0.1.0/tidychef/selection/xlsx/xlsx.py
--rw-r--r--   0        0        0       41 2023-06-28 13:17:51.552905 tidychef-0.1.0/tidychef/utils/__init__.py
--rw-r--r--   0        0        0       72 2023-05-24 09:26:46.004839 tidychef-0.1.0/tidychef/utils/cellutils/__init__.py
--rw-r--r--   0        0        0     1556 2023-05-24 09:26:46.005013 tidychef-0.1.0/tidychef/utils/cellutils/excel.py
--rw-r--r--   0        0        0       76 2023-05-24 09:26:46.005163 tidychef-0.1.0/tidychef/utils/decorators/README.md
--rw-r--r--   0        0        0       94 2023-07-18 07:19:23.361670 tidychef-0.1.0/tidychef/utils/decorators/__init__.py
--rw-r--r--   0        0        0      572 2023-05-28 22:18:13.736328 tidychef-0.1.0/tidychef/utils/decorators/dontmutate.py
--rw-r--r--   0        0        0       40 2023-06-16 20:07:44.113463 tidychef-0.1.0/tidychef/utils/fileutils/__init__.py
--rw-r--r--   0        0        0      809 2023-07-24 18:06:46.898985 tidychef-0.1.0/tidychef/utils/fileutils/paths.py
--rw-r--r--   0        0        0      494 2023-06-28 13:56:51.241240 tidychef-0.1.0/tidychef/utils/http/caching.py
--rw-r--r--   0        0        0     1605 1970-01-01 00:00:00.000000 tidychef-0.1.0/setup.py
--rw-r--r--   0        0        0      921 1970-01-01 00:00:00.000000 tidychef-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1950 2023-07-25 07:42:17.130890 tidychef-0.1.1/README.md
+-rw-r--r--   0        0        0     1223 2023-07-25 09:27:36.529144 tidychef-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      245 2023-07-25 07:54:18.333658 tidychef-0.1.1/tidychef/__init__.py
+-rw-r--r--   0        0        0      110 2023-07-05 08:30:04.083380 tidychef-0.1.1/tidychef/acquire/__init__.py
+-rw-r--r--   0        0        0      520 2023-07-24 18:04:58.226769 tidychef-0.1.1/tidychef/acquire/base.py
+-rw-r--r--   0        0        0      133 2023-06-28 13:56:49.387210 tidychef-0.1.1/tidychef/acquire/csv/__init__.py
+-rw-r--r--   0        0        0     3402 2023-07-25 07:42:58.792065 tidychef-0.1.1/tidychef/acquire/csv/http_implemented.py
+-rw-r--r--   0        0        0     3036 2023-07-25 07:43:33.075028 tidychef-0.1.1/tidychef/acquire/csv/local_implemented.py
+-rw-r--r--   0        0        0     2455 2023-07-25 07:45:41.458935 tidychef-0.1.1/tidychef/acquire/main.py
+-rw-r--r--   0        0        0      163 2023-07-23 15:42:10.265499 tidychef-0.1.1/tidychef/acquire/python/__init__.py
+-rw-r--r--   0        0        0     2467 2023-07-25 07:43:28.624238 tidychef-0.1.1/tidychef/acquire/python/listoflists_implemented.py
+-rw-r--r--   0        0        0     2851 2023-07-25 07:44:03.424136 tidychef-0.1.1/tidychef/acquire/python/pipetable_implemented.py
+-rw-r--r--   0        0        0      133 2023-06-28 14:19:41.973466 tidychef-0.1.1/tidychef/acquire/xls/__init__.py
+-rw-r--r--   0        0        0     4258 2023-07-25 07:44:26.721737 tidychef-0.1.1/tidychef/acquire/xls/http_implemented.py
+-rw-r--r--   0        0        0     3345 2023-07-25 07:44:39.053004 tidychef-0.1.1/tidychef/acquire/xls/local_implemented.py
+-rw-r--r--   0        0        0      134 2023-06-28 13:56:49.375947 tidychef-0.1.1/tidychef/acquire/xlsx/__init__.py
+-rw-r--r--   0        0        0     4372 2023-07-25 07:44:56.396637 tidychef-0.1.1/tidychef/acquire/xlsx/http_implemented.py
+-rw-r--r--   0        0        0     3662 2023-07-25 07:45:08.699028 tidychef-0.1.1/tidychef/acquire/xlsx/local_implemented.py
+-rw-r--r--   0        0        0      149 2023-07-23 17:11:06.781553 tidychef-0.1.1/tidychef/against/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-11 20:08:08.429121 tidychef-0.1.1/tidychef/against/implementations/__init__.py
+-rw-r--r--   0        0        0      638 2023-07-25 07:23:52.963306 tidychef-0.1.1/tidychef/against/implementations/base.py
+-rw-r--r--   0        0        0     1163 2023-07-25 07:25:47.995142 tidychef-0.1.1/tidychef/against/implementations/items.py
+-rw-r--r--   0        0        0     2401 2023-07-25 07:25:53.424611 tidychef-0.1.1/tidychef/against/implementations/length.py
+-rw-r--r--   0        0        0     3572 2023-07-25 07:25:36.472780 tidychef-0.1.1/tidychef/against/implementations/numeric.py
+-rw-r--r--   0        0        0     1120 2023-07-25 07:26:23.342013 tidychef-0.1.1/tidychef/against/implementations/regex.py
+-rw-r--r--   0        0        0     1766 2023-07-25 07:47:12.734570 tidychef-0.1.1/tidychef/against/wrapper.py
+-rw-r--r--   0        0        0       48 2023-05-28 22:18:13.690464 tidychef-0.1.1/tidychef/column/__init__.py
+-rw-r--r--   0        0        0     2970 2023-07-25 07:46:59.116780 tidychef-0.1.1/tidychef/column/base.py
+-rw-r--r--   0        0        0     4995 2023-07-25 07:47:30.656866 tidychef-0.1.1/tidychef/column/column.py
+-rw-r--r--   0        0        0      527 2023-06-27 16:25:09.098617 tidychef-0.1.1/tidychef/datafuncs/README.md
+-rw-r--r--   0        0        0     1075 2023-07-23 17:11:06.809528 tidychef-0.1.1/tidychef/datafuncs/__init__.py
+-rw-r--r--   0        0        0     8878 2023-07-24 18:03:57.415174 tidychef-0.1.1/tidychef/datafuncs/common.py
+-rw-r--r--   0        0        0     5639 2023-07-24 18:03:55.736608 tidychef-0.1.1/tidychef/datafuncs/excel.py
+-rw-r--r--   0        0        0     6119 2023-07-24 18:03:54.264597 tidychef-0.1.1/tidychef/datafuncs/ordering.py
+-rw-r--r--   0        0        0      453 2023-05-24 09:26:45.996492 tidychef-0.1.1/tidychef/direction/README.md
+-rw-r--r--   0        0        0       60 2023-07-12 10:33:30.217649 tidychef-0.1.1/tidychef/direction/__init__.py
+-rw-r--r--   0        0        0     4803 2023-07-24 18:03:49.931406 tidychef-0.1.1/tidychef/direction/directions.py
+-rw-r--r--   0        0        0      885 2023-07-23 17:11:06.805910 tidychef-0.1.1/tidychef/exceptions/__init__.py
+-rw-r--r--   0        0        0     2150 2023-07-23 13:37:16.866495 tidychef-0.1.1/tidychef/exceptions/badparams.py
+-rw-r--r--   0        0        0      777 2023-07-23 17:10:30.841539 tidychef-0.1.1/tidychef/exceptions/cells.py
+-rw-r--r--   0        0        0     3408 2023-07-23 17:10:20.538378 tidychef-0.1.1/tidychef/exceptions/common.py
+-rw-r--r--   0        0        0      652 2023-07-12 12:23:20.039435 tidychef-0.1.1/tidychef/exceptions/lookups.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:26:57.378906 tidychef-0.1.1/tidychef/lookup/__init__.py
+-rw-r--r--   0        0        0      447 2023-07-24 18:03:47.784091 tidychef-0.1.1/tidychef/lookup/base.py
+-rw-r--r--   0        0        0        0 2023-05-26 13:52:55.388417 tidychef-0.1.1/tidychef/lookup/engines/README.md
+-rw-r--r--   0        0        0        0 2023-06-14 15:18:13.870543 tidychef-0.1.1/tidychef/lookup/engines/__init__.py
+-rw-r--r--   0        0        0    13681 2023-07-25 07:48:25.203597 tidychef-0.1.1/tidychef/lookup/engines/closest.py
+-rw-r--r--   0        0        0      957 2023-07-24 18:03:44.342917 tidychef-0.1.1/tidychef/lookup/engines/constant.py
+-rw-r--r--   0        0        0     6129 2023-07-25 07:48:38.777076 tidychef-0.1.1/tidychef/lookup/engines/direct.py
+-rw-r--r--   0        0        0     4049 2023-07-25 07:48:47.404609 tidychef-0.1.1/tidychef/lookup/engines/horizontal_condition.py
+-rw-r--r--   0        0        0    10700 2023-07-25 07:49:00.642629 tidychef-0.1.1/tidychef/lookup/engines/within.py
+-rw-r--r--   0        0        0       21 2023-05-24 09:26:45.998537 tidychef-0.1.1/tidychef/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 09:26:46.000263 tidychef-0.1.1/tidychef/models/source/__init__.py
+-rw-r--r--   0        0        0     6999 2023-07-25 07:49:30.892006 tidychef-0.1.1/tidychef/models/source/cell.py
+-rw-r--r--   0        0        0       77 2023-05-24 09:26:46.000543 tidychef-0.1.1/tidychef/models/source/cellformat.py
+-rw-r--r--   0        0        0     7762 2023-07-25 07:49:40.728144 tidychef-0.1.1/tidychef/models/source/table.py
+-rw-r--r--   0        0        0       39 2023-06-20 17:35:02.406176 tidychef-0.1.1/tidychef/notebook/__init__.py
+-rw-r--r--   0        0        0      465 2023-07-16 10:09:55.515709 tidychef-0.1.1/tidychef/notebook/ipython.py
+-rw-r--r--   0        0        0        0 2023-06-17 11:41:28.459219 tidychef-0.1.1/tidychef/notebook/preview/__init__.py
+-rw-r--r--   0        0        0     3778 2023-07-25 07:51:24.701683 tidychef-0.1.1/tidychef/notebook/preview/boundary.py
+-rw-r--r--   0        0        0     2910 2023-07-25 07:50:26.281679 tidychef-0.1.1/tidychef/notebook/preview/html/components.py
+-rw-r--r--   0        0        0      651 2023-07-14 22:09:11.515526 tidychef-0.1.1/tidychef/notebook/preview/html/constants.py
+-rw-r--r--   0        0        0     2616 2023-07-25 07:50:37.866855 tidychef-0.1.1/tidychef/notebook/preview/html/main.py
+-rw-r--r--   0        0        0     4869 2023-07-25 07:50:58.627598 tidychef-0.1.1/tidychef/notebook/preview/html/table.py
+-rw-r--r--   0        0        0      926 2023-07-16 14:00:02.838338 tidychef-0.1.1/tidychef/notebook/preview/html/tidy_data.py
+-rw-r--r--   0        0        0       59 2023-07-12 10:33:30.001045 tidychef-0.1.1/tidychef/output/__init__.py
+-rw-r--r--   0        0        0      561 2023-06-16 19:33:30.841073 tidychef-0.1.1/tidychef/output/base.py
+-rw-r--r--   0        0        0    14254 2023-07-25 07:52:00.465984 tidychef-0.1.1/tidychef/output/tidydata.py
+-rw-r--r--   0        0        0      459 2023-06-27 16:24:57.036542 tidychef-0.1.1/tidychef/selection/README.md
+-rw-r--r--   0        0        0      143 2023-07-12 10:33:30.114915 tidychef-0.1.1/tidychef/selection/__init__.py
+-rw-r--r--   0        0        0      153 2023-07-24 18:06:08.468256 tidychef-0.1.1/tidychef/selection/csv/csv.py
+-rw-r--r--   0        0        0     2022 2023-06-27 16:25:30.891041 tidychef-0.1.1/tidychef/selection/filters/README.md
+-rw-r--r--   0        0        0      196 2023-07-17 15:19:20.512477 tidychef-0.1.1/tidychef/selection/filters/__init__.py
+-rw-r--r--   0        0        0     1388 2023-07-24 18:06:42.658006 tidychef-0.1.1/tidychef/selection/filters/common.py
+-rw-r--r--   0        0        0    28752 2023-07-25 07:58:50.258318 tidychef-0.1.1/tidychef/selection/selectable.py
+-rw-r--r--   0        0        0      132 2023-06-28 16:12:18.376303 tidychef-0.1.1/tidychef/selection/xls/xls.py
+-rw-r--r--   0        0        0      134 2023-06-28 16:11:52.808553 tidychef-0.1.1/tidychef/selection/xlsx/xlsx.py
+-rw-r--r--   0        0        0       41 2023-06-28 13:17:51.552905 tidychef-0.1.1/tidychef/utils/__init__.py
+-rw-r--r--   0        0        0       72 2023-05-24 09:26:46.004839 tidychef-0.1.1/tidychef/utils/cellutils/__init__.py
+-rw-r--r--   0        0        0     1556 2023-05-24 09:26:46.005013 tidychef-0.1.1/tidychef/utils/cellutils/excel.py
+-rw-r--r--   0        0        0       76 2023-05-24 09:26:46.005163 tidychef-0.1.1/tidychef/utils/decorators/README.md
+-rw-r--r--   0        0        0       94 2023-07-18 07:19:23.361670 tidychef-0.1.1/tidychef/utils/decorators/__init__.py
+-rw-r--r--   0        0        0      572 2023-05-28 22:18:13.736328 tidychef-0.1.1/tidychef/utils/decorators/dontmutate.py
+-rw-r--r--   0        0        0       40 2023-06-16 20:07:44.113463 tidychef-0.1.1/tidychef/utils/fileutils/__init__.py
+-rw-r--r--   0        0        0      809 2023-07-24 18:06:46.898985 tidychef-0.1.1/tidychef/utils/fileutils/paths.py
+-rw-r--r--   0        0        0      494 2023-06-28 13:56:51.241240 tidychef-0.1.1/tidychef/utils/http/caching.py
+-rw-r--r--   0        0        0     3637 1970-01-01 00:00:00.000000 tidychef-0.1.1/setup.py
+-rw-r--r--   0        0        0     3048 1970-01-01 00:00:00.000000 tidychef-0.1.1/PKG-INFO
```

### Comparing `tidychef-0.1.0/pyproject.toml` & `tidychef-0.1.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 [tool.poetry]
 name = "tidychef"
-version = "0.1.0"
-description = "Python package for transforming human readable tables into tidy data"
+version = "0.1.1"
+description = "Python framework for transforming tabulated data with visual relationships into tidy data"
 authors = ["mikeAdamss <mikelovesbooks@gmail.com>"]
 packages = [
   {include = "tidychef"},
 ]
 license = "Apache 2.0"
+readme = "README.md"
+repository = "https://github.com/mikeAdamss/tidychef"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 tabulate = "^0.9.0"
 requests = "^2.31.0"
 validators = "^0.20.0"
 openpyxl = "^3.1.2"
```

### Comparing `tidychef-0.1.0/tidychef/acquire/base.py` & `tidychef-0.1.1/tidychef/acquire/base.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.0/tidychef/acquire/csv/http_implemented.py` & `tidychef-0.1.1/tidychef/acquire/csv/http_implemented.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.0/tidychef/acquire/csv/local_implemented.py` & `tidychef-0.1.1/tidychef/acquire/csv/local_implemented.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.0/tidychef/acquire/main.py` & `tidychef-0.1.1/tidychef/acquire/main.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.0/tidychef/acquire/python/listoflists_implemented.py` & `tidychef-0.1.1/tidychef/acquire/python/listoflists_implemented.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.0/tidychef/acquire/python/pipetable_implemented.py` & `tidychef-0.1.1/tidychef/acquire/python/pipetable_implemented.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.0/tidychef/acquire/xls/http_implemented.py` & `tidychef-0.1.1/tidychef/acquire/xls/http_implemented.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.0/tidychef/acquire/xls/local_implemented.py` & `tidychef-0.1.1/tidychef/acquire/xls/local_implemented.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.0/tidychef/acquire/xlsx/http_implemented.py` & `tidychef-0.1.1/tidychef/acquire/xlsx/http_implemented.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.0/tidychef/acquire/xlsx/local_implemented.py` & `tidychef-0.1.1/tidychef/acquire/xlsx/local_implemented.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.0/tidychef/against/implementations/base.py` & `tidychef-0.1.1/tidychef/against/implementations/base.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.0/tidychef/against/implementations/items.py` & `tidychef-0.1.1/tidychef/against/implementations/items.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.0/tidychef/against/implementations/length.py` & `tidychef-0.1.1/tidychef/against/implementations/length.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.0/tidychef/against/implementations/numeric.py` & `tidychef-0.1.1/tidychef/against/implementations/numeric.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.0/tidychef/against/implementations/regex.py` & `tidychef-0.1.1/tidychef/against/implementations/regex.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.0/tidychef/against/wrapper.py` & `tidychef-0.1.1/tidychef/against/wrapper.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.0/tidychef/column/base.py` & `tidychef-0.1.1/tidychef/column/base.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.0/tidychef/column/column.py` & `tidychef-0.1.1/tidychef/column/column.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.0/tidychef/datafuncs/README.md` & `tidychef-0.1.1/tidychef/datafuncs/README.md`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.0/tidychef/datafuncs/__init__.py` & `tidychef-0.1.1/tidychef/datafuncs/__init__.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.0/tidychef/datafuncs/common.py` & `tidychef-0.1.1/tidychef/datafuncs/common.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.0/tidychef/datafuncs/excel.py` & `tidychef-0.1.1/tidychef/datafuncs/excel.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.0/tidychef/datafuncs/ordering.py` & `tidychef-0.1.1/tidychef/datafuncs/ordering.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.0/tidychef/direction/directions.py` & `tidychef-0.1.1/tidychef/direction/directions.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.0/tidychef/exceptions/__init__.py` & `tidychef-0.1.1/tidychef/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.0/tidychef/exceptions/badparams.py` & `tidychef-0.1.1/tidychef/exceptions/badparams.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.0/tidychef/exceptions/cells.py` & `tidychef-0.1.1/tidychef/exceptions/cells.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.0/tidychef/exceptions/common.py` & `tidychef-0.1.1/tidychef/exceptions/common.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.0/tidychef/exceptions/lookups.py` & `tidychef-0.1.1/tidychef/exceptions/lookups.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.0/tidychef/lookup/engines/closest.py` & `tidychef-0.1.1/tidychef/lookup/engines/closest.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.0/tidychef/lookup/engines/constant.py` & `tidychef-0.1.1/tidychef/lookup/engines/constant.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.0/tidychef/lookup/engines/direct.py` & `tidychef-0.1.1/tidychef/lookup/engines/direct.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.0/tidychef/lookup/engines/horizontal_condition.py` & `tidychef-0.1.1/tidychef/lookup/engines/horizontal_condition.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.0/tidychef/lookup/engines/within.py` & `tidychef-0.1.1/tidychef/lookup/engines/within.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.0/tidychef/models/source/cell.py` & `tidychef-0.1.1/tidychef/models/source/cell.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.0/tidychef/models/source/table.py` & `tidychef-0.1.1/tidychef/models/source/table.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.0/tidychef/notebook/preview/boundary.py` & `tidychef-0.1.1/tidychef/notebook/preview/boundary.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.0/tidychef/notebook/preview/html/components.py` & `tidychef-0.1.1/tidychef/notebook/preview/html/components.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.0/tidychef/notebook/preview/html/constants.py` & `tidychef-0.1.1/tidychef/notebook/preview/html/constants.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.0/tidychef/notebook/preview/html/main.py` & `tidychef-0.1.1/tidychef/notebook/preview/html/main.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.0/tidychef/notebook/preview/html/table.py` & `tidychef-0.1.1/tidychef/notebook/preview/html/table.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.0/tidychef/notebook/preview/html/tidy_data.py` & `tidychef-0.1.1/tidychef/notebook/preview/html/tidy_data.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.0/tidychef/output/base.py` & `tidychef-0.1.1/tidychef/output/base.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.0/tidychef/output/tidydata.py` & `tidychef-0.1.1/tidychef/output/tidydata.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.0/tidychef/selection/filters/README.md` & `tidychef-0.1.1/tidychef/selection/filters/README.md`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.0/tidychef/selection/filters/common.py` & `tidychef-0.1.1/tidychef/selection/filters/common.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.0/tidychef/selection/selectable.py` & `tidychef-0.1.1/tidychef/selection/selectable.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.0/tidychef/utils/cellutils/excel.py` & `tidychef-0.1.1/tidychef/utils/cellutils/excel.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.0/tidychef/utils/decorators/dontmutate.py` & `tidychef-0.1.1/tidychef/utils/decorators/dontmutate.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.0/tidychef/utils/fileutils/paths.py` & `tidychef-0.1.1/tidychef/utils/fileutils/paths.py`

 * *Files identical despite different names*

