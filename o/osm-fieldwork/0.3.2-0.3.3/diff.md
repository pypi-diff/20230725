# Comparing `tmp/osm-fieldwork-0.3.2.tar.gz` & `tmp/osm-fieldwork-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osm-fieldwork-0.3.2.tar", last modified: Tue Jun 27 10:50:24 2023, max compression
+gzip compressed data, was "osm-fieldwork-0.3.3.tar", last modified: Tue Jul 25 20:55:00 2023, max compression
```

## Comparing `osm-fieldwork-0.3.2.tar` & `osm-fieldwork-0.3.3.tar`

### file list

```diff
@@ -1,84 +1,96 @@
--rw-r--r--   0        0        0    34625 2023-06-27 10:50:14.222713 osm-fieldwork-0.3.2/LICENSE.md
--rw-r--r--   0        0        0     8656 2023-06-27 10:50:14.222713 osm-fieldwork-0.3.2/README.md
--rwxr-xr-x   0        0        0    13091 2023-06-27 10:50:14.230713 osm-fieldwork-0.3.2/osm_fieldwork/CSVDump.py
--rwxr-xr-x   0        0        0     5099 2023-06-27 10:50:14.230713 osm-fieldwork-0.3.2/osm_fieldwork/ODKDump.py
--rwxr-xr-x   0        0        0     4400 2023-06-27 10:50:14.230713 osm-fieldwork-0.3.2/osm_fieldwork/ODKForm.py
--rwxr-xr-x   0        0        0     4205 2023-06-27 10:50:14.230713 osm-fieldwork-0.3.2/osm_fieldwork/ODKInstance.py
--rwxr-xr-x   0        0        0    27428 2023-06-27 10:50:14.230713 osm-fieldwork-0.3.2/osm_fieldwork/OdkCentral.py
--rw-r--r--   0        0        0        0 2023-06-27 10:50:14.230713 osm-fieldwork-0.3.2/osm_fieldwork/__init__.py
--rw-r--r--   0        0        0       22 2023-06-27 10:50:14.230713 osm-fieldwork-0.3.2/osm_fieldwork/__version__.py
--rwxr-xr-x   0        0        0     9592 2023-06-27 10:50:14.230713 osm-fieldwork-0.3.2/osm_fieldwork/basemapper.py
--rwxr-xr-x   0        0        0     9946 2023-06-27 10:50:14.230713 osm-fieldwork-0.3.2/osm_fieldwork/convert.py
--rw-r--r--   0        0        0   683456 2023-06-27 10:50:14.234713 osm-fieldwork-0.3.2/osm_fieldwork/data_models/Impact Areas - Data Models V1.1.xlsx
--rw-r--r--   0        0        0      445 2023-06-27 10:50:14.234713 osm-fieldwork-0.3.2/osm_fieldwork/data_models/amenities.yaml
--rw-r--r--   0        0        0      226 2023-06-27 10:50:14.234713 osm-fieldwork-0.3.2/osm_fieldwork/data_models/buildings.yaml
--rw-r--r--   0        0        0      240 2023-06-27 10:50:14.234713 osm-fieldwork-0.3.2/osm_fieldwork/data_models/camping.yaml
--rw-r--r--   0        0        0      678 2023-06-27 10:50:14.234713 osm-fieldwork-0.3.2/osm_fieldwork/data_models/category.yaml
--rw-r--r--   0        0        0      119 2023-06-27 10:50:14.234713 osm-fieldwork-0.3.2/osm_fieldwork/data_models/cemeteries.yaml
--rw-r--r--   0        0        0      412 2023-06-27 10:50:14.234713 osm-fieldwork-0.3.2/osm_fieldwork/data_models/education.yaml
--rw-r--r--   0        0        0      137 2023-06-27 10:50:14.234713 osm-fieldwork-0.3.2/osm_fieldwork/data_models/emergency.yaml
--rw-r--r--   0        0        0      495 2023-06-27 10:50:14.234713 osm-fieldwork-0.3.2/osm_fieldwork/data_models/health.yaml
--rw-r--r--   0        0        0       94 2023-06-27 10:50:14.234713 osm-fieldwork-0.3.2/osm_fieldwork/data_models/landusage.yaml
--rw-r--r--   0        0        0    14028 2023-06-27 10:50:14.234713 osm-fieldwork-0.3.2/osm_fieldwork/data_models/models.yaml
--rw-r--r--   0        0        0      106 2023-06-27 10:50:14.234713 osm-fieldwork-0.3.2/osm_fieldwork/data_models/nature.yaml
--rw-r--r--   0        0        0      104 2023-06-27 10:50:14.234713 osm-fieldwork-0.3.2/osm_fieldwork/data_models/places.yaml
--rw-r--r--   0        0        0      107 2023-06-27 10:50:14.234713 osm-fieldwork-0.3.2/osm_fieldwork/data_models/religious.yaml
--rw-r--r--   0        0        0      245 2023-06-27 10:50:14.234713 osm-fieldwork-0.3.2/osm_fieldwork/data_models/toilets.yaml
--rwxr-xr-x   0        0        0     4745 2023-06-27 10:50:14.234713 osm-fieldwork-0.3.2/osm_fieldwork/data_models/validate.py
--rw-r--r--   0        0        0      348 2023-06-27 10:50:14.234713 osm-fieldwork-0.3.2/osm_fieldwork/data_models/wastedisposal.yaml
--rw-r--r--   0        0        0      170 2023-06-27 10:50:14.234713 osm-fieldwork-0.3.2/osm_fieldwork/data_models/waterpoints.yaml
--rw-r--r--   0        0        0      140 2023-06-27 10:50:14.234713 osm-fieldwork-0.3.2/osm_fieldwork/data_models/waterways.yaml
--rw-r--r--   0        0        0     1609 2023-06-27 10:50:14.234713 osm-fieldwork-0.3.2/osm_fieldwork/filter.yaml
--rwxr-xr-x   0        0        0     7378 2023-06-27 10:50:14.234713 osm-fieldwork-0.3.2/osm_fieldwork/filter_data.py
--rwxr-xr-x   0        0        0    16200 2023-06-27 10:50:14.234713 osm-fieldwork-0.3.2/osm_fieldwork/json2osm.py
--rwxr-xr-x   0        0        0    18873 2023-06-27 10:50:14.234713 osm-fieldwork-0.3.2/osm_fieldwork/make_data_extract.py
--rwxr-xr-x   0        0        0     5254 2023-06-27 10:50:14.234713 osm-fieldwork-0.3.2/osm_fieldwork/odk2csv.py
--rwxr-xr-x   0        0        0     4199 2023-06-27 10:50:14.234713 osm-fieldwork-0.3.2/osm_fieldwork/odk2geojson.py
--rwxr-xr-x   0        0        0    13649 2023-06-27 10:50:14.234713 osm-fieldwork-0.3.2/osm_fieldwork/odk_client.py
--rwxr-xr-x   0        0        0     8766 2023-06-27 10:50:14.234713 osm-fieldwork-0.3.2/osm_fieldwork/odk_merge.py
--rwxr-xr-x   0        0        0     5336 2023-06-27 10:50:14.234713 osm-fieldwork-0.3.2/osm_fieldwork/osm2favorities.py
--rwxr-xr-x   0        0        0    11547 2023-06-27 10:50:14.234713 osm-fieldwork-0.3.2/osm_fieldwork/osmfile.py
--rwxr-xr-x   0        0        0     8003 2023-06-27 10:50:14.234713 osm-fieldwork-0.3.2/osm_fieldwork/sqlite.py
--rw-r--r--   0        0        0     4474 2023-06-27 10:50:14.234713 osm-fieldwork-0.3.2/osm_fieldwork/xforms.yaml
--rw-r--r--   0        0        0     3800 2023-06-27 10:50:14.234713 osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/Makefile
--rw-r--r--   0        0        0      830 2023-06-27 10:50:14.234713 osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/__init__.py
--rw-r--r--   0        0        0  1469440 2023-06-27 10:50:14.238713 osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/amenities.xls
--rw-r--r--   0        0        0   240128 2023-06-27 10:50:14.242714 osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/buildings.xls
--rw-r--r--   0        0        0  3986944 2023-06-27 10:50:14.254714 osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/camping.xls
--rw-r--r--   0        0        0    98816 2023-06-27 10:50:14.254714 osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/cemeteries.xls
--rw-r--r--   0        0        0   111104 2023-06-27 10:50:14.254714 osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/education.xls
--rw-r--r--   0        0        0    69120 2023-06-27 10:50:14.254714 osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/health.xls
--rw-r--r--   0        0        0    22528 2023-06-27 10:50:14.254714 osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/historical.xls
--rw-r--r--   0        0        0    15872 2023-06-27 10:50:14.254714 osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/hotspring.xls
--rw-r--r--   0        0        0    59904 2023-06-27 10:50:14.254714 osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/landusage.xls
--rw-r--r--   0        0        0   129536 2023-06-27 10:50:14.258714 osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/landuse.xls
--rw-r--r--   0        0        0     1629 2023-06-27 10:50:14.258714 osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/lib/amenities.csv
--rw-r--r--   0        0        0      466 2023-06-27 10:50:14.258714 osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/lib/buildings.csv
--rw-r--r--   0        0        0       40 2023-06-27 10:50:14.258714 osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/lib/municipality.csv
--rw-r--r--   0        0        0      353 2023-06-27 10:50:14.258714 osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/lib/opening_hours.csv
--rw-r--r--   0        0        0      160 2023-06-27 10:50:14.258714 osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/lib/operational_status.csv
--rw-r--r--   0        0        0      171 2023-06-27 10:50:14.258714 osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/lib/provider.csv
--rw-r--r--   0        0        0     1737 2023-06-27 10:50:14.258714 osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/lib/towns.csv
--rw-r--r--   0        0        0       76 2023-06-27 10:50:14.258714 osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/lib/waste.csv
--rw-r--r--   0        0        0       41 2023-06-27 10:50:14.258714 osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/municipality.csv
--rw-r--r--   0        0        0    59392 2023-06-27 10:50:14.258714 osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/nature.xls
--rw-r--r--   0        0        0   126976 2023-06-27 10:50:14.258714 osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/places.xls
--rw-r--r--   0        0        0   103424 2023-06-27 10:50:14.258714 osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/religious.xls
--rw-r--r--   0        0        0   115963 2023-06-27 10:50:14.258714 osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/solidwaste.xlsx
--rw-r--r--   0        0        0   118272 2023-06-27 10:50:14.258714 osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/toilets.xls
--rw-r--r--   0        0        0      112 2023-06-27 10:50:14.258714 osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/towns.csv
--rw-r--r--   0        0        0    40448 2023-06-27 10:50:14.258714 osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/transportation.xls
--rw-r--r--   0        0        0    15186 2023-06-27 10:50:14.258714 osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/waste_collection.xlsx
--rw-r--r--   0        0        0   101888 2023-06-27 10:50:14.258714 osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/wastedisposal.xls
--rw-r--r--   0        0        0   211456 2023-06-27 10:50:14.262714 osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/waterpoints.xls
--rw-r--r--   0        0        0   269312 2023-06-27 10:50:14.262714 osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/waterways.xls
--rwxr-xr-x   0        0        0     3726 2023-06-27 10:50:14.262714 osm-fieldwork-0.3.2/osm_fieldwork/yamlfile.py
--rw-r--r--   0        0        0     1688 2023-06-27 10:50:14.262714 osm-fieldwork-0.3.2/pyproject.toml
--rw-r--r--   0        0        0       32 2023-06-27 10:50:14.262714 osm-fieldwork-0.3.2/tests/.flake8
--rw-r--r--   0        0        0      574 2023-06-27 10:50:14.262714 osm-fieldwork-0.3.2/tests/Test.yaml
--rw-r--r--   0        0        0     2713 2023-06-27 10:50:14.262714 osm-fieldwork-0.3.2/tests/test.csv
--rwxr-xr-x   0        0        0     2324 2023-06-27 10:50:14.262714 osm-fieldwork-0.3.2/tests/test_convert.py
--rwxr-xr-x   0        0        0     1889 2023-06-27 10:50:14.262714 osm-fieldwork-0.3.2/tests/test_csv.py
--rwxr-xr-x   0        0        0     3204 2023-06-27 10:50:14.262714 osm-fieldwork-0.3.2/tests/test_osm.py
--rwxr-xr-x   0        0        0     1649 2023-06-27 10:50:14.262714 osm-fieldwork-0.3.2/tests/test_yaml.py
--rw-r--r--   0        0        0     9343 1970-01-01 00:00:00.000000 osm-fieldwork-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0    34625 2023-07-25 20:54:52.845209 osm-fieldwork-0.3.3/LICENSE.md
+-rw-r--r--   0        0        0     8656 2023-07-25 20:54:52.845209 osm-fieldwork-0.3.3/README.md
+-rwxr-xr-x   0        0        0    13130 2023-07-25 20:54:52.849209 osm-fieldwork-0.3.3/osm_fieldwork/CSVDump.py
+-rwxr-xr-x   0        0        0     5099 2023-07-25 20:54:52.849209 osm-fieldwork-0.3.3/osm_fieldwork/ODKDump.py
+-rwxr-xr-x   0        0        0     4400 2023-07-25 20:54:52.849209 osm-fieldwork-0.3.3/osm_fieldwork/ODKForm.py
+-rwxr-xr-x   0        0        0     4205 2023-07-25 20:54:52.849209 osm-fieldwork-0.3.3/osm_fieldwork/ODKInstance.py
+-rwxr-xr-x   0        0        0    27539 2023-07-25 20:54:52.849209 osm-fieldwork-0.3.3/osm_fieldwork/OdkCentral.py
+-rw-r--r--   0        0        0        0 2023-07-25 20:54:52.849209 osm-fieldwork-0.3.3/osm_fieldwork/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-25 20:54:52.849209 osm-fieldwork-0.3.3/osm_fieldwork/__version__.py
+-rwxr-xr-x   0        0        0     9940 2023-07-25 20:54:52.849209 osm-fieldwork-0.3.3/osm_fieldwork/basemapper.py
+-rwxr-xr-x   0        0        0     9941 2023-07-25 20:54:52.849209 osm-fieldwork-0.3.3/osm_fieldwork/convert.py
+-rw-r--r--   0        0        0   683456 2023-07-25 20:54:52.853209 osm-fieldwork-0.3.3/osm_fieldwork/data_models/Impact Areas - Data Models V1.1.xlsx
+-rw-r--r--   0        0        0      504 2023-07-25 20:54:52.853209 osm-fieldwork-0.3.3/osm_fieldwork/data_models/amenities.yaml
+-rw-r--r--   0        0        0      349 2023-07-25 20:54:52.853209 osm-fieldwork-0.3.3/osm_fieldwork/data_models/buildings.yaml
+-rw-r--r--   0        0        0      240 2023-07-25 20:54:52.853209 osm-fieldwork-0.3.3/osm_fieldwork/data_models/camping.yaml
+-rw-r--r--   0        0        0      678 2023-07-25 20:54:52.853209 osm-fieldwork-0.3.3/osm_fieldwork/data_models/category.yaml
+-rw-r--r--   0        0        0      119 2023-07-25 20:54:52.853209 osm-fieldwork-0.3.3/osm_fieldwork/data_models/cemeteries.yaml
+-rw-r--r--   0        0        0      412 2023-07-25 20:54:52.853209 osm-fieldwork-0.3.3/osm_fieldwork/data_models/education.yaml
+-rw-r--r--   0        0        0      137 2023-07-25 20:54:52.853209 osm-fieldwork-0.3.3/osm_fieldwork/data_models/emergency.yaml
+-rw-r--r--   0        0        0      495 2023-07-25 20:54:52.853209 osm-fieldwork-0.3.3/osm_fieldwork/data_models/health.yaml
+-rw-r--r--   0        0        0       94 2023-07-25 20:54:52.853209 osm-fieldwork-0.3.3/osm_fieldwork/data_models/landusage.yaml
+-rw-r--r--   0        0        0    14028 2023-07-25 20:54:52.853209 osm-fieldwork-0.3.3/osm_fieldwork/data_models/models.yaml
+-rw-r--r--   0        0        0      106 2023-07-25 20:54:52.853209 osm-fieldwork-0.3.3/osm_fieldwork/data_models/nature.yaml
+-rw-r--r--   0        0        0      104 2023-07-25 20:54:52.853209 osm-fieldwork-0.3.3/osm_fieldwork/data_models/places.yaml
+-rw-r--r--   0        0        0      107 2023-07-25 20:54:52.853209 osm-fieldwork-0.3.3/osm_fieldwork/data_models/religious.yaml
+-rw-r--r--   0        0        0        0 2023-07-25 20:54:52.853209 osm-fieldwork-0.3.3/osm_fieldwork/data_models/taginfo-db.db
+-rw-r--r--   0        0        0      245 2023-07-25 20:54:52.853209 osm-fieldwork-0.3.3/osm_fieldwork/data_models/toilets.yaml
+-rwxr-xr-x   0        0        0     4745 2023-07-25 20:54:52.853209 osm-fieldwork-0.3.3/osm_fieldwork/data_models/validate.py
+-rw-r--r--   0        0        0      348 2023-07-25 20:54:52.853209 osm-fieldwork-0.3.3/osm_fieldwork/data_models/wastedisposal.yaml
+-rw-r--r--   0        0        0      170 2023-07-25 20:54:52.853209 osm-fieldwork-0.3.3/osm_fieldwork/data_models/waterpoints.yaml
+-rw-r--r--   0        0        0      140 2023-07-25 20:54:52.853209 osm-fieldwork-0.3.3/osm_fieldwork/data_models/waterways.yaml
+-rw-r--r--   0        0        0     1609 2023-07-25 20:54:52.853209 osm-fieldwork-0.3.3/osm_fieldwork/filter.yaml
+-rwxr-xr-x   0        0        0     7378 2023-07-25 20:54:52.853209 osm-fieldwork-0.3.3/osm_fieldwork/filter_data.py
+-rwxr-xr-x   0        0        0    16103 2023-07-25 20:54:52.853209 osm-fieldwork-0.3.3/osm_fieldwork/json2osm.py
+-rwxr-xr-x   0        0        0      442 2023-07-25 20:54:52.853209 osm-fieldwork-0.3.3/osm_fieldwork/main.py
+-rwxr-xr-x   0        0        0    21353 2023-07-25 20:54:52.853209 osm-fieldwork-0.3.3/osm_fieldwork/make_data_extract.py
+-rw-r--r--   0        0        0     3896 2023-07-25 20:54:52.853209 osm-fieldwork-0.3.3/osm_fieldwork/models.yaml
+-rwxr-xr-x   0        0        0     5284 2023-07-25 20:54:52.853209 osm-fieldwork-0.3.3/osm_fieldwork/odk2csv.py
+-rwxr-xr-x   0        0        0     4224 2023-07-25 20:54:52.853209 osm-fieldwork-0.3.3/osm_fieldwork/odk2geojson.py
+-rwxr-xr-x   0        0        0     5235 2023-07-25 20:54:52.853209 osm-fieldwork-0.3.3/osm_fieldwork/odk2osm.py
+-rwxr-xr-x   0        0        0    15611 2023-07-25 20:54:52.853209 osm-fieldwork-0.3.3/osm_fieldwork/odk_client.py
+-rwxr-xr-x   0        0        0    21645 2023-07-25 20:54:52.853209 osm-fieldwork-0.3.3/osm_fieldwork/odk_merge.py
+-rwxr-xr-x   0        0        0     5336 2023-07-25 20:54:52.853209 osm-fieldwork-0.3.3/osm_fieldwork/osm2favorities.py
+-rwxr-xr-x   0        0        0    13082 2023-07-25 20:54:52.853209 osm-fieldwork-0.3.3/osm_fieldwork/osmfile.py
+-rwxr-xr-x   0        0        0     8003 2023-07-25 20:54:52.853209 osm-fieldwork-0.3.3/osm_fieldwork/sqlite.py
+-rw-r--r--   0        0        0     3757 2023-07-25 20:54:52.853209 osm-fieldwork-0.3.3/osm_fieldwork/xforms.yaml
+-rw-r--r--   0        0        0       81 2023-07-25 20:54:52.853209 osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/.~lock.test.xls#
+-rw-r--r--   0        0        0     3795 2023-07-25 20:54:52.853209 osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/Makefile
+-rw-r--r--   0        0        0      830 2023-07-25 20:54:52.853209 osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/__init__.py
+-rw-r--r--   0        0        0  1469440 2023-07-25 20:54:52.857209 osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/amenities.xls
+-rw-r--r--   0        0        0   240128 2023-07-25 20:54:52.861209 osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/buildings.xls
+-rw-r--r--   0        0        0  3986944 2023-07-25 20:54:52.869209 osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/camping.xls
+-rw-r--r--   0        0        0    98816 2023-07-25 20:54:52.869209 osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/cemeteries.xls
+-rw-r--r--   0        0        0   111104 2023-07-25 20:54:52.869209 osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/education.xls
+-rw-r--r--   0        0        0    69120 2023-07-25 20:54:52.869209 osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/health.xls
+-rw-r--r--   0        0        0    22528 2023-07-25 20:54:52.869209 osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/historical.xls
+-rw-r--r--   0        0        0    15872 2023-07-25 20:54:52.873209 osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/hotspring.xls
+-rw-r--r--   0        0        0    59904 2023-07-25 20:54:52.873209 osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/landusage.xls
+-rw-r--r--   0        0        0   129536 2023-07-25 20:54:52.873209 osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/landuse.xls
+-rw-r--r--   0        0        0     1629 2023-07-25 20:54:52.873209 osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/lib/amenities.csv
+-rw-r--r--   0        0        0      466 2023-07-25 20:54:52.873209 osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/lib/buildings.csv
+-rw-r--r--   0        0        0       40 2023-07-25 20:54:52.873209 osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/lib/municipality.csv
+-rw-r--r--   0        0        0      353 2023-07-25 20:54:52.873209 osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/lib/opening_hours.csv
+-rw-r--r--   0        0        0      160 2023-07-25 20:54:52.873209 osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/lib/operational_status.csv
+-rw-r--r--   0        0        0      171 2023-07-25 20:54:52.873209 osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/lib/provider.csv
+-rw-r--r--   0        0        0     1737 2023-07-25 20:54:52.873209 osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/lib/towns.csv
+-rw-r--r--   0        0        0       76 2023-07-25 20:54:52.873209 osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/lib/waste.csv
+-rw-r--r--   0        0        0       41 2023-07-25 20:54:52.873209 osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/municipality.csv
+-rw-r--r--   0        0        0    59392 2023-07-25 20:54:52.873209 osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/nature.xls
+-rw-r--r--   0        0        0   126976 2023-07-25 20:54:52.873209 osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/places.xls
+-rw-r--r--   0        0        0   103424 2023-07-25 20:54:52.873209 osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/religious.xls
+-rw-r--r--   0        0        0   115963 2023-07-25 20:54:52.873209 osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/solidwaste.xlsx
+-rw-r--r--   0        0        0   265216 2023-07-25 20:54:52.873209 osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/test.xls
+-rw-r--r--   0        0        0   353280 2023-07-25 20:54:52.877209 osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/thamel.xls
+-rw-r--r--   0        0        0   118272 2023-07-25 20:54:52.877209 osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/toilets.xls
+-rw-r--r--   0        0        0      112 2023-07-25 20:54:52.877209 osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/towns.csv
+-rw-r--r--   0        0        0    40448 2023-07-25 20:54:52.877209 osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/transportation.xls
+-rw-r--r--   0        0        0    15186 2023-07-25 20:54:52.877209 osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/waste_collection.xlsx
+-rw-r--r--   0        0        0   101888 2023-07-25 20:54:52.877209 osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/wastedisposal.xls
+-rw-r--r--   0        0        0   211456 2023-07-25 20:54:52.877209 osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/waterpoints.xls
+-rw-r--r--   0        0        0   269312 2023-07-25 20:54:52.877209 osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/waterways.xls
+-rwxr-xr-x   0        0        0     3726 2023-07-25 20:54:52.877209 osm-fieldwork-0.3.3/osm_fieldwork/yamlfile.py
+-rw-r--r--   0        0        0     2106 2023-07-25 20:54:52.877209 osm-fieldwork-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0       32 2023-07-25 20:54:52.877209 osm-fieldwork-0.3.3/tests/.flake8
+-rw-r--r--   0        0        0      574 2023-07-25 20:54:52.877209 osm-fieldwork-0.3.3/tests/Test.yaml
+-rw-r--r--   0        0        0     2713 2023-07-25 20:54:52.877209 osm-fieldwork-0.3.3/tests/test.csv
+-rwxr-xr-x   0        0        0     3817 2023-07-25 20:54:52.877209 osm-fieldwork-0.3.3/tests/test_conflation.py
+-rwxr-xr-x   0        0        0     2427 2023-07-25 20:54:52.877209 osm-fieldwork-0.3.3/tests/test_convert.py
+-rwxr-xr-x   0        0        0     2076 2023-07-25 20:54:52.877209 osm-fieldwork-0.3.3/tests/test_csv.py
+-rwxr-xr-x   0        0        0     3473 2023-07-25 20:54:52.877209 osm-fieldwork-0.3.3/tests/test_osm.py
+-rwxr-xr-x   0        0        0     2992 2023-07-25 20:54:52.877209 osm-fieldwork-0.3.3/tests/test_uriparser.py
+-rwxr-xr-x   0        0        0     1697 2023-07-25 20:54:52.877209 osm-fieldwork-0.3.3/tests/test_yaml.py
+-rw-r--r--   0        0        0    12719 2023-07-25 20:54:52.877209 osm-fieldwork-0.3.3/tests/testdata/Salida.geojson
+-rw-r--r--   0        0        0     5601 2023-07-25 20:54:52.877209 osm-fieldwork-0.3.3/tests/testdata/odk_pois.osm
+-rw-r--r--   0        0        0   129410 2023-07-25 20:54:52.877209 osm-fieldwork-0.3.3/tests/testdata/osm_buildings.geojson
+-rw-r--r--   0        0        0     9343 1970-01-01 00:00:00.000000 osm-fieldwork-0.3.3/PKG-INFO
```

### Comparing `osm-fieldwork-0.3.2/LICENSE.md` & `osm-fieldwork-0.3.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.2/README.md` & `osm-fieldwork-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.2/osm_fieldwork/CSVDump.py` & `osm-fieldwork-0.3.3/osm_fieldwork/CSVDump.py`

 * *Files 0% similar despite different names*

```diff
@@ -289,23 +289,23 @@
                 feature["refs"] = refs
             if len(priv) > 0:
                 feature["private"] = priv
 
         return feature
 
 
-if __name__ == "__main__":
+def main():
     parser = argparse.ArgumentParser(
         description="convert CSV from ODK Central to OSM XML"
     )
     parser.add_argument("-v", "--verbose", action="store_true", help="verbose output")
     parser.add_argument("-y", "--yaml", help="Alternate YAML file")
     parser.add_argument("-x", "--xlsfile", help="Source XLSFile")
     parser.add_argument(
-        "-i", "--infile", help="The input file downloaded from ODK Central"
+        "-i", "--infile", required=True, help="The input file downloaded from ODK Central"
     )
     args = parser.parse_args()
     
     # if verbose, dump to the terminal.
     if args.verbose is not None:
         root = logging.getLogger()
         root.setLevel(logging.DEBUG)
@@ -346,7 +346,10 @@
             csvin.writeGeoJson(feature)
             # print("TAGS: %r" % feature['tags'])
 
     csvin.finishOSM()
     csvin.finishGeoJson()
     log.info("Wrote OSM XML file: %r" % osmoutfile)
     log.info("Wrote GeoJson file: %r" % jsonoutfile)
+
+if __name__ == "__main__":
+    main()
```

### Comparing `osm-fieldwork-0.3.2/osm_fieldwork/ODKDump.py` & `osm-fieldwork-0.3.3/osm_fieldwork/ODKDump.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.2/osm_fieldwork/ODKForm.py` & `osm-fieldwork-0.3.3/osm_fieldwork/ODKForm.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.2/osm_fieldwork/ODKInstance.py` & `osm-fieldwork-0.3.3/osm_fieldwork/ODKInstance.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.2/osm_fieldwork/OdkCentral.py` & `osm-fieldwork-0.3.3/osm_fieldwork/OdkCentral.py`

 * *Files 1% similar despite different names*

```diff
@@ -452,30 +452,34 @@
             url = f"{self.base}projects/{projectId}/forms/{xform}/draft/attachments"
         else:
             url = f"{self.base}projects/{projectId}/forms/{xform}/attachments"
         result = self.session.get(url, auth=self.auth, verify=self.verify)
         self.media = result.json()
         return self.media
 
+
     def uploadMedia(self,
                     projectId: int,
                     xform: str,
-                    filespec: str
+                    filespec: str,
+                    convert_to_draft: bool = True
                     ):
         """Upload an attachement to the ODK Central server"""
         title = os.path.basename(os.path.splitext(filespec)[0])
         datafile = f"{title}.geojson"
         xid = xform.split('_')[2]
-        url = f"{self.base}projects/{projectId}/forms/{xid}/draft"
-        result = self.session.post(url, auth=self.auth, verify=self.verify)
-        if result.status_code == 200:
-            log.debug(f"Modified {title} to draft")
-        else:
-            status = eval(result._content)
-            log.error(f"Couldn't modify {title} to draft: {status['message']}")
+
+        if convert_to_draft: 
+            url = f"{self.base}projects/{projectId}/forms/{xid}/draft"
+            result = self.session.post(url, auth=self.auth, verify=self.verify)
+            if result.status_code == 200:
+                log.debug(f"Modified {title} to draft")
+            else:
+                status = eval(result._content)
+                log.error(f"Couldn't modify {title} to draft: {status['message']}")
 
         url = f"{self.base}projects/{projectId}/forms/{xid}/draft/attachments/{datafile}"
         headers = {"Content-Type": "*/*"}
         file = open(filespec, "rb")
         media = file.read()
         file.close()
         result = self.session.post(
```

### Comparing `osm-fieldwork-0.3.2/osm_fieldwork/basemapper.py` & `osm-fieldwork-0.3.3/osm_fieldwork/basemapper.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,20 +46,27 @@
 
     # totaltime = 0.0
     logging.info(
         "Downloading %d tiles in thread %d to %s"
         % (len(tiles), threading.get_ident(), dest)
     )
     for tile in tiles:
+        bingkey = mercantile.quadkey(tile)
         filespec = f"{tile[2]}/{tile[1]}/{tile[0]}"
         for site in mirrors:
             if site["source"] != "topo":
                 filespec += "." + site["suffix"]
             url = site["url"]
-            remote = url % filespec
+            if  site["source"] == "bing":
+                remote = url % bingkey
+            elif  site["source"] == "google":
+                path = f"x={tile[0]}&s=&y={tile[1]}&z={tile[2]}"
+                remote = url % path
+            else:
+                remote = url % filespec
             print("Getting file from: %s" % remote)
             # Create the subdirectories as pySmartDL doesn't do it for us
             if os.path.isdir(dest) is False:
                 tmp = ""
                 paths = dest.split("/")
                 for i in paths[1:]:
                     tmp += "/" + i
@@ -94,19 +101,19 @@
         self.tiles = list()
         self.base = base
         # sources for imagery
         self.source = source
         self.sources = dict()
 
         # Bing hybrid imagery
-        url = "http://ecn.t0.tiles.virtualearth.net/tiles/h%s.png?g=129&mkt=en&stl=H"
+        url = "http://ecn.t0.tiles.virtualearth.net/tiles/h%s.jpg?g=129&mkt=en&stl=H"
         source = {
             "name": "Bing Maps Hybrid",
             "url": url,
-            "suffix": "png",
+            "suffix": "jpg",
             "source": "bing",
         }
         self.sources["bing"] = source
 
         # ERSI imagery
         url = "http://services.arcgisonline.com/arcgis/rest/services/World_Imagery/MapServer/tile/%s"
         source = {
@@ -124,19 +131,20 @@
             "url": url,
             "suffix": "jpg",
             "source": "topo",
         }
         self.sources["topo"] = source
 
         # Google Hybrid
-        url = "https://mt0.google.com/vt?lyrs=h&x={x}&s=&y={y}&z={z}"
+        # url = "https://mt0.google.com/vt?lyrs=s&x={x}&s=&y={y}&z={z}"
+        url = "https://mt0.google.com/vt?lyrs=s&%s"
         source = {
-            "name": "Google Hybrid",
+            "name": "Google Imagery",
             "url": url,
-            "suffix": "png",
+            "suffix": "jpg",
             "source": "google",
         }
         self.sources["google"] = source
 
         # OpenArialMap
         url = "https://tiles.openaerialmap.org/63962d0d9f665400075759be/0/63962d0d9f665400075759bf/{z}/{x}/{y}"
         source = {
```

### Comparing `osm-fieldwork-0.3.2/osm_fieldwork/convert.py` & `osm-fieldwork-0.3.3/osm_fieldwork/convert.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,19 +25,26 @@
 import argparse
 import sys
 
 # Instantiate logger
 log = logging.getLogger(__name__)
 
 
+def escape(value: str):
+    """Escape characters like embedded quotes in text fields"""
+    # tmp = value.replace(" ", "_")
+    tmp = value.replace("&", " and ")
+    return tmp.replace("'", "&apos;")
+
+
 class Convert(YamlFile):
     """A class to apply a YAML config file and convert ODK to OSM"""
 
     def __init__(self,
-                 xform: str
+                 xform: str = None
                  ):
         path = xlsforms_path.replace("xlsforms", "")
         if xform is not None:
             file = xform
         else:
             file = f"{path}/xforms.yaml"
         self.yaml = YamlFile(file)
@@ -84,21 +91,14 @@
 
     def ignoreData(self,
                    keyword: str
                    ):
         """See is a keyword is in the convert data category"""
         return keyword in self.ignore
 
-    def escape(self,
-               value: str
-               ):
-        """Escape characters like embedded quotes in text fields"""
-        tmp = value.replace(" ", "_")
-        return tmp.replace("'", "&apos;")
-
     def getKeyword(self,
                    value: str
                    ):
         """Get the value for a keyword from the yaml file"""
         key = self.yaml.yaml(value)
         if type(key) == bool:
             return value
```

### Comparing `osm-fieldwork-0.3.2/osm_fieldwork/data_models/Impact Areas - Data Models V1.1.xlsx` & `osm-fieldwork-0.3.3/osm_fieldwork/data_models/Impact Areas - Data Models V1.1.xlsx`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.2/osm_fieldwork/data_models/category.yaml` & `osm-fieldwork-0.3.3/osm_fieldwork/data_models/category.yaml`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.2/osm_fieldwork/data_models/models.yaml` & `osm-fieldwork-0.3.3/osm_fieldwork/data_models/models.yaml`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.2/osm_fieldwork/data_models/validate.py` & `osm-fieldwork-0.3.3/osm_fieldwork/data_models/validate.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.2/osm_fieldwork/filter.yaml` & `osm-fieldwork-0.3.3/osm_fieldwork/filter.yaml`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.2/osm_fieldwork/filter_data.py` & `osm-fieldwork-0.3.3/osm_fieldwork/filter_data.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.2/osm_fieldwork/json2osm.py` & `osm-fieldwork-0.3.3/osm_fieldwork/json2osm.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,23 +22,24 @@
 import csv
 import os
 import logging
 import sys
 import json
 import geojson
 from sys import argv
-from osm_fieldwork.convert import Convert
+from osm_fieldwork.convert import Convert, escape
 from osm_fieldwork.osmfile import OsmFile
 from osm_fieldwork.xlsforms import xlsforms_path
 from geojson import Point, Feature, FeatureCollection, dump
 from pathlib import Path
 #import pandas as pd
 import math
 import re
 
+
 # set log level for urlib
 log = logging.getLogger(__name__)
 
 class JsonDump(Convert):
     """A class to parse the JSON files from ODK Central or odk2geojson"""
 
     def __init__(self,
@@ -46,19 +47,14 @@
                  ):
         self.fields = dict()
         self.nodesets = dict()
         self.data = list()
         self.osm = None
         self.json = None
         self.features = list()
-        path = xlsforms_path.replace("xlsforms", "")
-        if yaml:
-            file = f"{yaml}"
-        else:
-            file = f"{path}/xforms.yaml"
         self.config = super().__init__(yaml)
 
     # def parseXLS(self, xlsfile: str):
     #     """Parse the source XLSFile if available to look for details we need"""
     #     if xlsfile is not None and len(xlsfile) > 0:
     #         entries = pd.read_excel(xlsfile, sheet_name=[0])
     #         # There will only be a single sheet
@@ -168,15 +164,15 @@
                         #             value = val
                         #         else:
                         #             self.saved[k] = value
                         #             log.debug(f"Updating last saved value for \"{k}\" with \"{value}\"")
                         if type(v) != str:
                             tags[k] = str(v)
                         else:
-                            tags[k] = v
+                            tags[k] = escape(v)
                 all_tags.update(tags)
         return all_tags
 
     def parse(self,
               filespec: str,
               data: str = None
               ):
@@ -344,24 +340,23 @@
             if len(refs) > 0:
                 feature["refs"] = refs
             if len(priv) > 0:
                 feature["private"] = priv
 
         return feature
 
-
-if __name__ == "__main__":
+def main():
     parser = argparse.ArgumentParser(
         description="convert JSON from ODK Central to OSM XML"
     )
     parser.add_argument("-v", "--verbose", action="store_true", help="verbose output")
     parser.add_argument("-y", "--yaml", help="Alternate YAML file")
     parser.add_argument("-x", "--xlsfile", help="Source XLSFile")
     parser.add_argument(
-        "-i", "--infile", help="The input file downloaded from ODK Central"
+        "-i", "--infile", required=True, help="The input file downloaded from ODK Central"
     )
     args = parser.parse_args()
     
     # if verbose, dump to the terminal.
     if args.verbose is not None:
         root = logging.getLogger()
         root.setLevel(logging.DEBUG)
@@ -410,11 +405,14 @@
                 else:
                     log.warning("Bad record! %r" % feature)
                     continue
             jsonin.writeOSM(feature)
             # This GeoJson file has all the data values
             jsonin.writeGeoJson(feature)
 
-    jsonin.finishOSM()
+    # jsonin.finishOSM()
     jsonin.finishGeoJson()
     log.info("Wrote OSM XML file: %r" % osmoutfile)
     log.info("Wrote GeoJson file: %r" % jsonoutfile)
+
+if __name__ == "__main__":
+    main()
```

### Comparing `osm-fieldwork-0.3.2/osm_fieldwork/make_data_extract.py` & `osm-fieldwork-0.3.3/osm_fieldwork/make_data_extract.py`

 * *Files 16% similar despite different names*

```diff
@@ -27,41 +27,96 @@
 import json
 from sys import argv
 from geojson import Point, Feature, FeatureCollection, dump, Polygon
 import geojson
 from osm_fieldwork.filter_data import FilterData
 from osm_fieldwork.xlsforms import xlsforms_path
 import requests
-# from requests.auth import HTTPBasicAuth
 from io import BytesIO
 import zipfile
 import time
 import psycopg2
 from shapely.geometry import shape, Polygon
 import overpy
 import shapely
 from shapely import wkt
+import logging
 
+# Instantiate logger
+log = logging.getLogger(__name__)
+
+
+def uriParser(source):
+    """Parse a URI into it's components"""
+    dbhost = None
+    dbname = None
+    dbuser = None
+    dbpass = None
+    dbport = None
+
+    # if dbhost is 'localhost' then this tries to
+    # connect to that hostname's tcp/ip port. If dbhost
+    # is None, the datbase connection is done locally
+    # through the named pipe.
+    colon = source.find(':')
+    rcolon = source.rfind(':')
+    atsign = source.find('@')
+    slash = source.find('/')
+    # If nothing but a string, then it's a local postgres database
+    # that doesn't require a user or password to login.
+    if colon < 0 and atsign < 0 and slash < 0:
+        dbname = source
+    # Get the database name, which is always after the slash
+    if slash > 0:
+        dbname = source[slash+1:]
+    # The user field is either between the beginning of the string,
+    # and either a colon or atsign as the end.
+    if colon > 0:
+        dbuser = source[:colon]
+    if colon < 0 and atsign > 0:
+        dbuser = source[:atsign]
+    # The password field is between a colon and the atsign
+    if colon > 0 and atsign > 0:
+        dbpass = source[colon+1:atsign]
+    # The hostname for the database is after an atsign, and ends
+    # either with the end of the string or a slash.
+    if atsign > 0:
+        if rcolon > 0 and rcolon > atsign:
+            dbhost = source[atsign+1:rcolon]
+        elif slash > 0:
+            dbhost = source[atsign+1:slash]
+        else:
+            dbhost = source[atsign+1:]
+    # rcolon is only above zero if there is a port number
+    if rcolon > 0 and rcolon > atsign:
+        if slash > 0:
+            dbport = source[rcolon+1:slash]
+        else:
+            dbport = source[rcolon+1:]
+            # import epdb; epdb.st()
+    if colon > 0 and atsign < 0 and slash > 0:
+        dbpass = source[colon+1:slash]
+
+        # print(f"{source}\n\tcolon={colon} rcolon={rcolon} atsign={atsign} slash={slash}")
+    db = {'dbname': dbname, 'dbhost': dbhost, 'dbuser': dbuser, 'dbpass': dbpass, 'dbport': dbport}
+
+    return db
 
 def getChoices():
     """Get the categories and associated XLSFiles fgrom the config file"""
     data = dict()
     path = xlsforms_path.replace("xlsforms", "data_models")
     if os.path.exists(f"{path}/category.yaml"):
         file = open(f"{path}/category.yaml", "r").read()
         contents = yaml.load(file, Loader=yaml.Loader)
         for entry in contents:
             [[k,v]] = entry.items()
             data[k] = v[0]
     return data
 
-# Instantiate logger
-log = logging.getLogger(__name__)
-
-
 class DatabaseAccess(object):
     def __init__(self,
                  dbhost: str = None,
                  dbname: str = None,
                  dbuser: str = None,
                  dbpass: str = None,
                  ):
@@ -73,33 +128,33 @@
             # self.auth = HTTPBasicAuth(self.user, self.passwd)
 
             # Use a persistant connect, better for multiple requests
             self.session = requests.Session()
             self.url = "https://raw-data-api0.hotosm.org/v1"
             self.headers = {"accept": "application/json", "Content-Type": "application/json"}
         else:
-            logging.info("Opening database connection to: %s" % dbhost)
+            log.info("Opening database connection to: %s" % dbhost)
             connect = "PG: dbname=" + dbname
             if dbhost is None or dbhost == "localhost":
                 connect = f"dbname={dbname}"
             else:
                 connect = f"host={dbhost} dbname={dbname}"
             if dbuser:
                 connect += f" user={dbuser}"
             if dbpass:
                 connect += f" password={dbpass}"
-            logging.debug(connect)
+            log.debug(connect)
             try:
                 self.dbshell = psycopg2.connect(connect)
                 self.dbshell.autocommit = True
                 self.dbcursor = self.dbshell.cursor()
                 if self.dbcursor.closed == 0:
-                    logging.info(f"Opened cursor in {dbname}")
+                    log.info(f"Opened cursor in {dbname}")
             except Exception as e:
-                logging.error("Couldn't connect to database: %r" % e)
+                log.error("Couldn't connect to database: %r" % e)
 
     def createJson(self,
                    category: str,
                    boundary,
                    poly: bool = False
                    ):
         path = xlsforms_path.replace("xlsforms", "data_models")
@@ -153,17 +208,17 @@
                 centroid = "geom"
             else:
                 centroid = "ST_Centroid(geom)"
             # if tags exists, then only return those fields
             if 'tags' in select:
                 for tag in select['tags']:
                     query += f" {select[tag]} AS {tag}, "
-                query += f"osm_id AS id, ST_AsEWKT({centroid} "
+                query += f"osm_id AS id, ST_AsEWKT({centroid}, version "
             else:
-                query += f"osm_id AS id, ST_AsEWKT({centroid}), tags "
+                query += f"osm_id AS id, ST_AsEWKT({centroid}), tags, version "
             query += f" FROM {table} "
             where = data['where']
             # if tags exists, then only query those fields
             if 'where' in data:
                 query += " WHERE "
                 tags = data['where']['tags'][0]
                 for tag, value in tags.items():
@@ -177,40 +232,45 @@
             sql.append(query[:-4])
         return sql
 
     def queryLocal(self,
                    query: str = None,
                    ewkt: str = None
                    ):
-        sql = f"DROP VIEW IF EXISTS ways_view;CREATE TEMP VIEW ways_view AS SELECT * FROM ways_poly WHERE ST_CONTAINS(ST_GeomFromEWKT('SRID=4326;{ewkt.wkt}'), geom)"
+        # sql = f"DROP VIEW IF EXISTS ways_view;CREATE TEMP VIEW ways_view AS SELECT * FROM ways_poly WHERE ST_CONTAINS(ST_GeomFromEWKT('SRID=4326;{ewkt.wkt}'), geom)"
+        sql = f"DROP VIEW IF EXISTS ways_view;CREATE VIEW ways_view AS SELECT * FROM ways_poly WHERE ST_CONTAINS(ST_GeomFromEWKT('SRID=4326;{ewkt.wkt}'), geom)"
         self.dbcursor.execute(sql)
-        sql = f"DROP VIEW IF EXISTS nodes_view;CREATE TEMP VIEW nodes_view AS SELECT * FROM nodes WHERE ST_CONTAINS(ST_GeomFromEWKT('SRID=4326;{ewkt.wkt}'), geom)"
+        # sql = f"DROP VIEW IF EXISTS nodes_view;CREATE TEMP VIEW nodes_view AS SELECT * FROM nodes WHERE ST_CONTAINS(ST_GeomFromEWKT('SRID=4326;{ewkt.wkt}'), geom)"
+        sql = f"DROP VIEW IF EXISTS nodes_view;CREATE VIEW nodes_view AS SELECT * FROM nodes WHERE ST_CONTAINS(ST_GeomFromEWKT('SRID=4326;{ewkt.wkt}'), geom)"
         self.dbcursor.execute(sql)
 
         sql = f"DROP VIEW IF EXISTS relations_view;CREATE TEMP VIEW relations_view AS SELECT * FROM nodes WHERE ST_CONTAINS(ST_GeomFromEWKT('SRID=4326;{ewkt.wkt}'), geom)"
         # self.dbcursor.execute(sql)
 
         if query.find(" ways_poly ") > 0:
             query = query.replace("ways_poly", "ways_view")
         elif query.find(" nodes ") > 0:
             query = query.replace("nodes", "nodes_view")
         features = list()
         log.debug(query)
         self.dbcursor.execute(query)
         result = self.dbcursor.fetchall()
-        logging.info("Query returned %d records" % len(result))
+        log.info("Query returned %d records" % len(result))
         for item in result:
+            if len(item) <= 1:
+                break
             gps = item[1][16:-1].split(" ")
             if len(gps) == 2:
                 poi = Point((float(gps[0]), float(gps[1])))
             else:
                 gps = item[1][10:]
                 poi = wkt.loads(gps)
             tags = item[2]
             tags["id"] = item[0]
+            tags['version'] = item[3]
             if "name:en" in tags:
                 tags["title"] = tags["name:en"]
                 tags["label"] = tags["name:en"]
             elif "name" in tags:
                 tags["title"] = tags["name"]
                 tags["label"] = tags["name"]
             else:
@@ -254,39 +314,38 @@
                  dbname: str = None,
                  dbuser: str = None,
                  dbpass: str = None,
                  #output: str = None
     ):
         """Initialize the postgres handler"""
         # OutputFile.__init__( self, output)
-        self.boundary = None
         super().__init__(dbhost, dbname, dbuser, dbpass)
 
     def getFeatures(self,
                     boundary,
                     filespec: str,
                     polygon: bool,
                     category: str,
-                    xlsfile: str,
+                    xlsfile: str
                     ):
         """Extract buildings from Postgres"""
-        logging.info("Extracting features from Postgres...")
+        log.info("Extracting features from Postgres...")
 
         if type(boundary) != dict:
             clip = open(boundary, "r")
             geom = geojson.load(clip)
             if 'features' in geom:
                 poly = geom['features'][0]['geometry']
             else:
                 poly = geom["geometry"]
         else:
             poly = boundary
         wkt = shape(poly)
 
-        if len(xlsfile) > 0:
+        if xlsfile and len(xlsfile) > 0:
             config = xlsfile.replace(".xls", "")
         else:
             config = category
         if self.dbshell:
             # features = list()
             sql = self.createSQL(config, polygon)
             all = list()
@@ -296,37 +355,40 @@
             collection = FeatureCollection(all)
         else:
             request = self.createJson(config, poly, polygon)
             collection = self.queryRemote(request)
         if not collection:
             return None
 
+        extract = "no"
         if len(collection['features']) == 0:
             tags = { 'title': category, 'label': category, 'id': 0}
             center = shapely.centroid(wkt)
             feature = [Feature(geometry=center, properties=tags)]
             new = FeatureCollection(feature)
             extract = "yes"
-        else:
+        elif xlsfile:
             # Process the XLSForm source file and scan it for valid tags
             # and values.
             cleaned = FilterData()
             models = xlsforms_path.replace("xlsforms", "data_models")
             if not xlsfile:
                 xlsfile = f"{category}.xls"
             file = f"{xlsforms_path}/{xlsfile}"
             if os.path.exists(file):
                 title, extract = cleaned.parse(file)
             elif os.path.exists(f"{file}x"):
                 title, extract = cleaned.parse(f"{file}x")
             # Remove anything in the data extract not in the choices sheet.
             new = cleaned.cleanData(collection)
+        else:
+            new = collection
 
         # This will be set if the XLSForm contains a select_one_from_file
-        if len(extract) > 0:
+        if len(extract) > 0 and filespec is not None:
             # filespec = f"/tmp/{outfile}"
             jsonfile = open(filespec, "w")
             dump(new, jsonfile)
             jsonfile.close()
         return new
 
 class OverpassClient(object):
@@ -340,15 +402,15 @@
     def getFeatures(self,
                     boundary,
                     filespec: str,
                     xlsfile: str,
                     category: str
                     ):
         """Extract buildings from Overpass"""
-        logging.info("Extracting features...")
+        log.info("Extracting features...")
 
         poly = ""
         if type(boundary) == str:
             clip = open(boundary, "r")
             geom = geojson.load(clip)
             if 'features' in geom:
                 aoi = geom['features'][0]['geometry']
@@ -404,29 +466,29 @@
 
     def getFeatures(self,
                     boundary,
                     infile: str,
                     outfile: str
                     ):
         """Extract buildings from a disk file"""
-        logging.info("Extracting buildings from %s..." % infile)
+        log.info("Extracting buildings from %s..." % infile)
         if boundary:
             poly = ogr.Open(boundary)
             layer = poly.GetLayer()
             ogr.Layer.Clip(osm, layer, memlayer)
         else:
             layer = poly.GetLayer()
 
         tmp = ogr.Open(infile)
         layer = tmp.GetLayer()
 
         layer.SetAttributeFilter("tags->>'building' IS NOT NULL")
 
 
-if __name__ == "__main__":
+def main():
     choices = getChoices()
     
     parser = argparse.ArgumentParser(
         description="Make GeoJson data file for ODK from OSM"
     )
     parser.add_argument("-v", "--verbose", nargs="?", const="0", help="verbose output")
     parser.add_argument(
@@ -475,45 +537,48 @@
 
     if args.geojson == "tmp.geojson":
         # The data file name is in the XML file
         regex = r"jr://file.*\.geojson"
         outfile = None
         filename = args.category + ".xml"
         if not os.path.exists(filename):
-            logging.error("Please run xls2xform or make to produce %s" % filename)
+            log.error("Please run xls2xform or make to produce %s" % filename)
             quit()
         with open(filename, "r") as f:
             txt = f.read()
             match = re.search(regex, txt)
             if match:
                 tmp = match.group().split("/")
         outfile = tmp[3]
     else:
         outfile = args.geojson.lower()
 
     xlsfile = choices[args.category]
     if args.postgres:
-        logging.info("Using a Postgres database for the data source")
-        pg = PostgresClient(args.dbhost, args.dbname, outfile)
+        log.info("Using a Postgres database for the data source")
+        pg = PostgresClient(args.dbhost, args.dbname)
         if args.geojson:
             extract = args.geojson
         else:
             infile = FilterData(xlsfile)
             extract = infile.metadata[1]
         pg.getFeatures(args.boundary, extract, args.polygon, args.category, xlsfile)
         log.info(f"Created {outfile} for {args.category}")
         # pg.cleanup(outfile)
     elif args.overpass:
-        logging.info("Using Overpass Turbo for the data source")
+        log.info("Using Overpass Turbo for the data source")
         op = OverpassClient(outfile)
         clip = open(args.boundary, "r")
         geom = geojson.load(clip)
         #op.getFeatures(args.boundary, args.geojson, args.category)
         op.getFeatures(geom, args.geojson, xlsfile, args.category)
     elif args.infile:
         f = FileClient(args.infile)
         f.getFeatures(args.boundary, args.geojson, args.category)
-        logging.info("Using file %s for the data source" % args.infile)
+        log.info("Using file %s for the data source" % args.infile)
     else:
-        logging.error("You need to supply either --overpass or --postgres")
+        log.error("You need to supply either --overpass or --postgres")
 
-        logging.info("Wrote output data file to: %s" % outfile)
+        # logging.info("Wrote output data file to: %s" % outfile)
+
+if __name__ == "__main__":
+    main()
```

### Comparing `osm-fieldwork-0.3.2/osm_fieldwork/odk2csv.py` & `osm-fieldwork-0.3.3/osm_fieldwork/odk2csv.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,21 +28,20 @@
 from pathlib import Path
 from datetime import datetime
 
 # Instantiate logger
 log = logging.getLogger(__name__)
 
 
-if __name__ == "__main__":
+def main():
     parser = argparse.ArgumentParser(
         description="Convert ODK XML instance file to CSV format"
     )
     parser.add_argument("-v", "--verbose", nargs="?", const="0", help="verbose output")
-    parser.add_argument(
-        "-i", "--instance", help="The instance file(s) from ODK Collect"
+    parser.add_argument("-i", "--instance", required=True, help="The instance file(s) from ODK Collect"
     )
     # parser.add_argument("-d","--directories", help='A local directory pato to instance files.')
     # parser.add_argument("-o","--outfile", default='tmp.csv', help='The output file for JOSM')
     args = parser.parse_args()
 
     # if verbose, dump to the termina
     if not args.verbose:
@@ -136,7 +135,10 @@
                     fields.append(key)
         csv = csv.DictWriter(csvfile, dialect="excel", fieldnames=fields)
         csv.writeheader()
         for row in rows:
             csv.writerow(row)
 
     print("Wrote: %s" % outfile)
+
+if __name__ == "__main__":
+    main()
```

### Comparing `osm-fieldwork-0.3.2/osm_fieldwork/odk2geojson.py` & `osm-fieldwork-0.3.3/osm_fieldwork/odk2geojson.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,22 +33,20 @@
 from shapely.geometry import Point
 from datetime import datetime
 
 
 # Instantiate logger
 log = logging.getLogger(__name__)
 
-if __name__ == "__main__":
+def moon():
     parser = argparse.ArgumentParser(
         description="Convert ODK XML instance file to GeoJson"
     )
     parser.add_argument("-v", "--verbose", nargs="?", const="0", help="verbose output")
-    parser.add_argument(
-        "-i", "--instance", help="The instance file(s) from ODK Collect"
-    )
+    parser.add_argument("-i", "--instance", required=True, help="The instance file(s) from ODK Collect")
     parser.add_argument("-o","--outfile", default='tmp.geojson', help='The output file for JOSM')
     args = parser.parse_args()
 
     # if verbose, dump to the termina
     if not args.verbose:
         root = logging.getLogger()
         root.setLevel(logging.DEBUG)
@@ -111,7 +109,10 @@
     now = datetime.now()
     timestamp = f"_{now.year}_{now.month}-{now.day}-{now.hour}-{now.minute}"
     outfile = args.instance.replace("*", "") + timestamp + ".geojson"
     json = open(outfile, 'w')
     dump(collection, json)
 
     print(f"Wrote output file {outfile}")
+
+if __name__ == "__main__":
+    main()
```

### Comparing `osm-fieldwork-0.3.2/osm_fieldwork/odk_client.py` & `osm-fieldwork-0.3.3/osm_fieldwork/odk_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,308 +56,318 @@
                 file = open(cache, "wb")
             file.write("projects\n")
             file.write(json.dump(data))
             file.close()
         logging.info("Wrote config file %s" % filespec)
 
 
-parser = argparse.ArgumentParser(description="command line client for ODK Central")
-parser.add_argument("-v", "--verbose", action="store_true", help="verbose output")
-# This is for server requests
-parser.add_argument(
-    "-s", "--server", choices=["projects", "users", "delete"], help="project operations"
-)
-# This is for project specific requests
-parser.add_argument(
-    "-p",
-    "--project",
-    choices=["forms", "app-users", "assignments", "delete"],
-    help="project operations",
-)
-parser.add_argument("-i", "--id", type=int, help="Project ID nunmber")
-parser.add_argument("-f", "--form", help="XForm name")
-parser.add_argument("-u", "--uuid", help="Submission UUID, needed to download the data")
-# This is for form specific requests
-parser.add_argument("-x", "--xform",
-    choices=[
-        "attachments",
-        "csv",
-        "json",
-        "submissions",
-        "upload",
-        "download",
-        "create",
-        "assignments",
-        "delete",
-        "publish",
-    ],
-    help="XForm ID for operations with data files",
-)
-parser.add_argument(
-    "-a",
-    "--appuser",
-    choices=["create", "delete", "update", "qrcode", "access"],
-    help="App-User operations",
-)
-parser.add_argument("-d", "--data", help="Data files for upload or download")
-parser.add_argument("-t", "--timestamp", help="Timestamp for submissions")
-parser.add_argument(
-    "-b", "--bulk", choices=["qrcodes", "update"], help="Bulk operations"
-)
+def main():
+    parser = argparse.ArgumentParser(description="command line client for ODK Central")
+    parser.add_argument("-v", "--verbose", action="store_true", help="verbose output")
+    # This is for server requests
+    parser.add_argument(
+        "-s", "--server", choices=["projects", "users", "delete"], help="project operations"
+    )
+    # This is for project specific requests
+    parser.add_argument(
+        "-p",
+        "--project",
+        choices=["forms", "app-users", "assignments", "delete"],
+        help="project operations",
+    )
+    parser.add_argument("-i", "--id", type=int, help="Project ID nunmber")
+    parser.add_argument("-f", "--form", help="XForm name")
+    parser.add_argument("-u", "--uuid", help="Submission UUID, needed to download the data")
+    # This is for form specific requests
+    parser.add_argument("-x", "--xform",
+                        choices=[
+                            "attachments",
+                            "csv",
+                            "json",
+                            "submissions",
+                            "upload",
+                            "download",
+                            "create",
+                            "assignments",
+                            "delete",
+                            "publish",
+                        ],
+                        help="XForm ID for operations with data files",
+                        )
+    parser.add_argument(
+        "-a",
+        "--appuser",
+        choices=["create", "delete", "update", "qrcode", "access"],
+        help="App-User operations",
+    )
+    parser.add_argument("-d", "--data", help="Data files for upload or download")
+    parser.add_argument("-t", "--timestamp", help="Timestamp for submissions")
+    parser.add_argument(
+        "-b", "--bulk", choices=["qrcodes", "update"], help="Bulk operations"
+    )
 
-# Creating a basic logger
-if __name__ == '__main__':
     logging.basicConfig(
         level=log_level,
         format=(
             "%(asctime)s.%(msecs)03d [%(levelname)s]"
             "%(name)s | %(funcName)s:%(lineno)d | %(message)s"
         ),
         datefmt="%y-%m-%d %H:%M:%S",
         stream=sys.stdout,
     )
 
-
-# Caching isn't implemented yet. That's for fancier queries that require multiple
-# requests to the ODK server. Caching allows for data like names for IDs to
-# be more user friendly.
-# parser.add_argument('-c', '--cache', action="store_true", help = 'cache data from ODK Central')
-# For now read these from the $HOME/.odkcentral config file
-# parser.add_argument('-u', '--user', help = 'ODK Central username (usually email)')
-# parser.add_argument('-pw', '--password', help = 'ODK Central password')
-
-# parser.add_argument("-d", "--download", choices=['xml', 'xlsx', 'attach', 'submit', 'zip'], help="Download files from ODK Central")
-# parser.add_argument("-u", "--upload", choices=['xml', 'xlsx', 'attach', 'submit', 'zip'], help="Upload files to ODK Central")
-
-# Any files we want to use are specified on the command line with an argument.
-# Multiple files are stored in a list.
-args, unknown = parser.parse_known_args()
-
-# Get any files for upload or download
-files = list()
-if unknown:
-    files = unknown
-
-# if verbose, dump to the terminal.
-if args.verbose is not None:
-    root = logging.getLogger()
-    root.setLevel(logging.DEBUG)
-
-    ch = logging.StreamHandler(sys.stdout)
-    ch.setLevel(logging.DEBUG)
-    formatter = logging.Formatter(
-        "%(asctime)s - %(name)s - %(levelname)s - %(message)s"
-    )
-    ch.setFormatter(formatter)
-    root.addHandler(ch)
-
-# Commands to the ODK Central server, which gets data that applies
-# to all projects on the server.
-if args.server:
-    central = OdkCentral()
-    # central.authenticate()
-    if args.server == "projects":
-        projects = central.listProjects()
-        print("There are %d projects on this ODK Central server" % len(projects))
-        ordered = sorted(projects, key=lambda item: item.get("id"))
-        for project in ordered:
-            print("\t%s: %s" % (project["id"], project["name"]))
-    elif args.server == "users":
-        users = central.listUsers()
-        logging.info("There are %d users on this ODK Central server" % len(users))
-        ordered = sorted(users, key=lambda item: item.get("id"))
-        for user in ordered:
-            print("%s: %s (%s)" % (user["id"], user["displayName"], user["email"]))
-    elif args.server == "delete":
-        central.deleteProject(args.id)
-
-# Commands to get data about a specific project on an ODK Central server.
-elif args.project:
-    project = OdkProject()
-    # project.authenticate()
-    if not args.id:
-        print('Need to specify a project ID using "--id"!')
-        print(
-            'You can use "odk_client.-py --server projects" to list all the projects!'
-        )
-        # parser.print_help()
-        quit()
-    if args.project == "forms":
-        forms = project.listForms(args.id)
-        ordered = sorted(forms, key=lambda item: item.get("xmlFormId"))
-        for form in ordered:
-            print("\t%r: %r" % (form["xmlFormId"], form["name"]))
-    # if args.project == "submissions":
-    #     submit = project.listSubmissions(args.id, args.form)
-    #     # ordered = sorted(submit, key=lambda item: item.get('xmlFormId'))
-    #     for data in submit:
-    #         print("\t%s by user %s" % (data['instanceId'], data['submitterId']))
-    if args.project == "app-users":
-        users = project.listAppUsers(args.id)
-        logging.info("There are %d app users on this ODK Central server" % len(users))
-        ordered = sorted(users, key=lambda item: item.get("id"))
-        for user in ordered:
-            print("\t%r: %s (%s)" % (user["id"], user["displayName"], user["token"]))
-    if args.project == "delete":
-        tmp = files[0].split("-")
-        if len(tmp) > 1:
-            for id in range(int(tmp[0]), int(tmp[1])):
-                project.deleteProject(id)
-        else:
-            project.deleteProject(tmp[0])
-
-        # logging.info("There are %d app users on this ODK Central server" %)
-    if args.project == "assignments":
-        assign = project.listAssignments(args.id)
-        logging.info(
-            "There are %d assignments  on this ODK Central server" % len(assign)
-        )
-        ordered = sorted(assign, key=lambda item: item.get("id"))
-        for role in ordered:
-            print("\t%r" % role)
-
-elif args.xform:
-    # This downloads files from the ODK server
-    if not args.id:
-        print('Need to specify a project ID using "--id" and an XForm id using "--"!')
-        quit()
-    if not args.form:
-        print('Need to specify a XForm id using "--form"!')
-        quit()
-
-    form = OdkForm()
-    # form.authenticate()
-    # Note that uploading and downloading is only for the attachments, usually
-    # a CSV or GeoJson file used by the Form as an external data source for
-    # survey questions
-    if args.xform == "upload":
-        for file in files:
-            logging.info("Uploading file %r for XForm %s" % (file, args.form))
-            result = form.uploadMedia(args.id, args.form, file)
-
-    elif args.xform == "download":
-        logging.info("Downloading files %r for XForm %s" % (files, args.form))
-        for file in files:
-            logging.info("Downloading %r for XForm %s" % (file, args.form))
-            data = form.getMedia(args.id, args.form, file)
-            try:
-                file = open(file, "xb")
-            except FileExistsError:
-                file = open(file, "wb")
-            file.write(data)
-            file.close()
-    elif args.xform == "assignments":
-        assign = form.listAssignments(args.id, args.form)
-        logging.info(
-            "There are %d assignments  on this ODK Central server" % len(assign)
+    # Caching isn't implemented yet. That's for fancier queries that require multiple
+    # requests to the ODK server. Caching allows for data like names for IDs to
+    # be more user friendly.
+    # parser.add_argument('-c', '--cache', action="store_true", help = 'cache data from ODK Central')
+    # For now read these from the $HOME/.odkcentral config file
+    # parser.add_argument('-u', '--user', help = 'ODK Central username (usually email)')
+    # parser.add_argument('-pw', '--password', help = 'ODK Central password')
+    # parser.add_argument("-d", "--download", choices=['xml', 'xlsx', 'attach', 'submit', 'zip'], help="Download files from ODK Central")
+    # parser.add_argument("-u", "--upload", choices=['xml', 'xlsx', 'attach', 'submit', 'zip'], help="Upload files to ODK Central")
+
+    # Any files we want to use are specified on the command line with an argument.
+    # Multiple files are stored in a list.
+    args, unknown = parser.parse_known_args()
+
+    # Get any files for upload or download
+    files = list()
+    if unknown is not None:
+        files = unknown
+
+    # if verbose, dump to the terminal.
+    if args.verbose is not None:
+        root = logging.getLogger()
+        root.setLevel(logging.DEBUG)
+
+        ch = logging.StreamHandler(sys.stdout)
+        ch.setLevel(logging.DEBUG)
+        formatter = logging.Formatter(
+            "%(asctime)s - %(name)s - %(levelname)s - %(message)s"
         )
-        # ordered = sorted(assign, key=lambda item: item.get('id'))
-        for role in assign:
-            print("\t%r" % role)
-    elif args.xform == "submissions":
-        submissions = form.listSubmissions(args.id, args.form)
-        logging.info(
-            "There are %d submissions for XForm %s" % (len(submissions), args.form)
-        )
-        for file in submissions:
-            # form.submissions.append(file)
-            print("%s: %s" % (file["instanceId"], file["createdAt"]))
-
-    elif args.xform == "csv":
-        submissions = form.getSubmissions(args.id, args.form, True, False)
-        logging.info(
-            "There are %d submissions for XForm %s" % (len(submissions), args.form)
-        )
-        for file in submissions:
-            form.submissions.append(file)
-            print("%s: %s" % (file["instanceId"], file["createdAt"]))
-
-    elif args.xform == "json":
-        submissions = form.getSubmissions(args.id, args.form, False, True, True)
-        logging.info(
-            "There are %d submissions for XForm %s" % (len(submissions), args.form)
-        )
-        for file in submissions:
-            form.submissions.append(file)
-            #print("%s: %s" % (file["instanceId"], file["createdAt"]))
-
-    elif args.xform == "attachments":
-        attachments = form.listMedia(args.id, args.form)
-        logging.info(
-            "There are %d attachments for XForm %s" % (len(attachments), args.form)
-        )
-        for file in attachments:
-            print("\t%s exists ? %s" % (file["name"], file["exists"]))
+        ch.setFormatter(formatter)
+        root.addHandler(ch)
 
-    elif args.xform == "create":
-        for file in files:
-            path = Path(file)
-            if path.suffix == ".xml":
-                logging.info("Creating XForm from %s" % file)
-                result = form.createForm(args.id, args.form, file, True)
-            elif path.suffix == ".csv":
-                logging.info("Uploading media file %r for XForm %s" % (file, file))
+    # Commands to the ODK Central server, which gets data that applies
+    # to all projects on the server.
+    if args.server:
+        central = OdkCentral()
+        # central.authenticate()
+        if args.server == "projects":
+            projects = central.listProjects()
+            print("There are %d projects on this ODK Central server" % len(projects))
+            ordered = sorted(projects, key=lambda item: item.get("id"))
+            for project in ordered:
+                print("\t%s: %s" % (project["id"], project["name"]))
+        elif args.server == "users":
+            users = central.listUsers()
+            logging.info("There are %d users on this ODK Central server" % len(users))
+            ordered = sorted(users, key=lambda item: item.get("id"))
+            for user in ordered:
+                print("%s: %s (%s)" % (user["id"], user["displayName"], user["email"]))
+        elif args.server == "delete":
+            central.deleteProject(args.id)
+
+        # Commands to get data about a specific project on an ODK Central server.
+    elif args.project:
+        project = OdkProject()
+        # project.authenticate()
+        if not args.id:
+            print('Need to specify a project ID using "--id"!')
+            print(
+                'You can use "odk_client.-py --server projects" to list all the projects!'
+            )
+            # parser.print_help()
+            quit()
+        if args.project == "forms":
+            forms = project.listForms(args.id)
+            if type(forms) == dict:
+                log.error(f"{forms['message']}, {forms['code']} ")
+                quit()
+            if type(forms) != list:
+                log.error(forms['message'])
+                quit()
+                ordered = sorted(forms, key=lambda item: item.get("xmlFormId"))
+                for form in ordered:
+                    print("\t%r: %r" % (form["xmlFormId"], form["name"]))
+                    # if args.project == "submissions":
+                    #     submit = project.listSubmissions(args.id, args.form)
+                    #     # ordered = sorted(submit, key=lambda item: item.get('xmlFormId'))
+                    #     for data in submit:
+                    #         print("\t%s by user %s" % (data['instanceId'], data['submitterId']))
+        elif args.project == "app-users":
+            users = project.listAppUsers(args.id)
+            logging.info("There are %d app users on this ODK Central server" % len(users))
+            ordered = sorted(users, key=lambda item: item.get("id"))
+            for user in ordered:
+                print("\t%r: %s (%s)" % (user["id"], user["displayName"], user["token"]))
+        elif args.project == "delete":
+            tmp = files[0].split("-")
+            if len(tmp) > 1:
+                for id in range(int(tmp[0]), int(tmp[1])):
+                    project.deleteProject(id)
+            else:
+                project.deleteProject(tmp[0])
+
+            # logging.info("There are %d app users on this ODK Central server" %)
+            if args.project == "assignments":
+                assign = project.listAssignments(args.id)
+                logging.info(
+                    "There are %d assignments  on this ODK Central server" % len(assign)
+                )
+            ordered = sorted(assign, key=lambda item: item.get("id"))
+            for role in ordered:
+                print("\t%r" % role)
+
+    elif args.xform:
+        # This downloads files from the ODK server
+        if not args.id:
+            print('Need to specify a project ID using "--id" and an XForm id using "--"!')
+            quit()
+        if not args.form:
+            print('Need to specify a XForm id using "--form"!')
+            quit()
+
+        form = OdkForm()
+        # form.authenticate()
+        # Note that uploading and downloading is only for the attachments, usually
+        # a CSV or GeoJson file used by the Form as an external data source for
+        # survey questions
+        if args.xform == "upload":
+            for file in files:
+                logging.info("Uploading file %r for XForm %s" % (file, args.form))
                 result = form.uploadMedia(args.id, args.form, file)
-        result = form.publishForm(args.id, args.form)
-
-    elif args.xform == "delete":
-        logging.info("Deleting XForm from %s" % args.form)
-        result = form.deleteForm(args.id, args.form)
-
-    elif args.xform == "publish":
-        logging.info("Publishing XForm from %s" % args.form)
-        result = form.publishForm(args.id, args.form)
-
-elif args.appuser:
-    # This handles app-users
-    print("App User ops %s" % args.appuser)
-    if not args.id:
-        print('Need to specify a project ID using "--id" and an XForm id using "--"!')
-        quit()
-    # if not args.form:
-    #     print("Need to specify a XForm id using \"--form\"!")
-    #     quit()
-
-    role = 2  # seems to be the default value
-    user = OdkAppUser()
-    if args.appuser == "create":
-        for appuser in files:
-            result = user.create(args.id, appuser)
-    elif args.appuser == "delete":
-        tmp = files[0].split("-")
-        if len(tmp) > 1:
-            for id in range(int(tmp[0]), int(tmp[1])):
-                result = user.delete(args.id, id)
-        else:
-            result = user.delete(args.id, tmp[0])
-    elif args.appuser == "update":
-        for appuser in files:
-            result = user.updateRole(args.id, args.form, role, appuser)
-    elif args.appuser == "qrcode":
-        result = user.getQRCode(args.id, args.uuid, args.form)
-    elif args.appuser == "access":
-        for appuser in files:
-            result = user.grantAccess(
-                args.id,
-                role,
-                appuser,
+        elif args.xform == "download":
+            logging.info("Downloading files %r for XForm %s" % (files, args.form))
+            for file in files:
+                logging.info("Downloading %r for XForm %s" % (file, args.form))
+                data = form.getMedia(args.id, args.form, file)
+                try:
+                    file = open(file, "xb")
+                except FileExistsError:
+                    file = open(file, "wb")
+                    file.write(data)
+                    file.close()
+        elif args.xform == "assignments":
+            assign = form.listAssignments(args.id, args.form)
+            logging.info(
+                "There are %d assignments  on this ODK Central server" % len(assign)
+            )
+            # ordered = sorted(assign, key=lambda item: item.get('id'))
+            for role in assign:
+                print("\t%r" % role)
+        elif args.xform == "submissions":
+            submissions = form.listSubmissions(args.id, args.form)
+            if not submissions:
+                submissions = list()
+            elif type(submissions) == dict:
+                log.error(f"{submissions['message']}, {submissions['code']} ")
+            else:
+                logging.info(
+                    "There are %d submissions for XForm %s" % (len(submissions), args.form)
+                )
+            for file in submissions:
+                # form.submissions.append(file)
+                print("%s: %s" % (file["instanceId"], file["createdAt"]))
+
+        elif args.xform == "csv":
+            submissions = form.getSubmissions(args.id, args.form, True, False)
+            logging.info(
+                "There are %d submissions for XForm %s" % (len(submissions), args.form)
+            )
+            for file in submissions:
+                form.submissions.append(file)
+                print("%s: %s" % (file["instanceId"], file["createdAt"]))
+
+        elif args.xform == "json":
+            submissions = form.getSubmissions(args.id, args.form, False, True, True)
+            logging.info(
+                "There are %d submissions for XForm %s" % (len(submissions), args.form)
             )
-    print(result)
+            for file in submissions:
+                form.submissions.append(file)
+                #print("%s: %s" % (file["instanceId"], file["createdAt"]))
+
+        elif args.xform == "attachments":
+            attachments = form.listMedia(args.id, args.form)
+            logging.info(
+                "There are %d attachments for XForm %s" % (len(attachments), args.form)
+            )
+            for file in attachments:
+                print("\t%s exists ? %s" % (file["name"], file["exists"]))
+
+        elif args.xform == "create":
+            for file in files:
+                path = Path(file)
+                if path.suffix == ".xml":
+                    logging.info("Creating XForm from %s" % file)
+                    result = form.createForm(args.id, args.form, file, True)
+                elif path.suffix == ".csv":
+                    logging.info("Uploading media file %r for XForm %s" % (file, file))
+                    result = form.uploadMedia(args.id, args.form, file)
+                    result = form.publishForm(args.id, args.form)
+
+        elif args.xform == "delete":
+            logging.info("Deleting XForm from %s" % args.form)
+            result = form.deleteForm(args.id, args.form)
+
+        elif args.xform == "publish":
+            logging.info("Publishing XForm from %s" % args.form)
+            result = form.publishForm(args.id, args.form)
+
+    elif args.appuser:
+        # This handles app-users
+        print("App User ops %s" % args.appuser)
+        if not args.id:
+            print('Need to specify a project ID using "--id" and an XForm id using "--"!')
+            quit()
+            # if not args.form:
+            #     print("Need to specify a XForm id using \"--form\"!")
+            #     quit()
+
+        role = 2  # seems to be the default value
+        user = OdkAppUser()
+        if args.appuser == "create":
+            for appuser in files:
+                result = user.create(args.id, appuser)
+        elif args.appuser == "delete":
+            tmp = files[0].split("-")
+            if len(tmp) > 1:
+                for id in range(int(tmp[0]), int(tmp[1])):
+                    result = user.delete(args.id, id)
+            else:
+                result = user.delete(args.id, tmp[0])
+        elif args.appuser == "update":
+            for appuser in files:
+                result = user.updateRole(args.id, args.form, role, appuser)
+        elif args.appuser == "qrcode":
+            result = user.getQRCode(args.id, args.uuid, args.form)
+        elif args.appuser == "access":
+            for appuser in files:
+                result = user.grantAccess(
+                    args.id,
+                    role,
+                    appuser,
+                )
+                print(result)
+
+        elif args.bulk:
+            central = OdkProject()
+            # project = central.getDetails(args.id)
+            appuser = OdkAppUser()
+            role = 2  # thise seems to be the default value
+            if not args.form:
+                print('Need to specify a XForm id using "--form"!')
+                quit()
+            if args.bulk == "qrcodes":
+                users = central.listAppUsers(args.id)
+                for user in users:
+                    # name = "%s-%s" % (project['name'], user['displayName'])
+                    name = "%s-%s" % (args.form, user["displayName"])
+                    result = appuser.getQRCode(args.id, user["token"], name)
+            elif args.bulk == "update":
+                users = central.listAppUsers(args.id)
+                for user in users:
+                    result = appuser.updateRole(args.id, args.form, role, user["id"])
 
-elif args.bulk:
-    central = OdkProject()
-    # project = central.getDetails(args.id)
-    appuser = OdkAppUser()
-    role = 2  # thise seems to be the default value
-    if not args.form:
-        print('Need to specify a XForm id using "--form"!')
-        quit()
-    if args.bulk == "qrcodes":
-        users = central.listAppUsers(args.id)
-        for user in users:
-            # name = "%s-%s" % (project['name'], user['displayName'])
-            name = "%s-%s" % (args.form, user["displayName"])
-            result = appuser.getQRCode(args.id, user["token"], name)
-    elif args.bulk == "update":
-        users = central.listAppUsers(args.id)
-        for user in users:
-            result = appuser.updateRole(args.id, args.form, role, user["id"])
+if __name__ == "__main__":
+    main()
```

### Comparing `osm-fieldwork-0.3.2/osm_fieldwork/osm2favorities.py` & `osm-fieldwork-0.3.3/osm_fieldwork/osm2favorities.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.2/osm_fieldwork/osmfile.py` & `osm-fieldwork-0.3.3/osm_fieldwork/osmfile.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin St, Fifth Floor, Boston, MA  02110-1301  USA
 #
 
 import logging
 from datetime import datetime
-from osm_fieldwork.convert import Convert
+from osm_fieldwork.convert import Convert, escape
 from osm_fieldwork.xlsforms import xlsforms_path
 import xmltodict
 import argparse
 from sys import argv
 import os
 import pathlib
 
@@ -30,29 +30,27 @@
 log = logging.getLogger(__name__)
 
 
 class OsmFile(object):
     """OSM File output"""
 
     def __init__(self,
-                 filespec: str,
+                 filespec: str = None,
                  options: dict = dict(),
                  outdir: str = "/tmp/"
                  ):
         self.options = options
         # Read the config file to get our OSM credentials, if we have any
         # self.config = config.config(self.options)
         self.version = 3
         self.visible = "true"
         self.osmid = -1
         # Open the OSM output file
-        if filespec is None:
-            if "outdir" in self.options:
-                self.file = self.options.get("outdir") + "foobar.osm"
-        else:
+        self.file = None
+        if filespec is not None:
             self.file = open(filespec, "w")
             # self.file = open(filespec + ".osm", 'w')
             logging.info("Opened output file: " + filespec)
         self.header()
         # logging.error("Couldn't open %s for writing!" % filespec)
 
         # This is the file that contains all the filtering data
@@ -60,33 +58,38 @@
         # self.options['convfile'] = None
         # These are for importing the CO addresses
         self.full = None
         self.addr = None
         # decrement the ID
         self.start = -1
         # path = xlsforms_path.replace("xlsforms", "")
-        self.convert = Convert("xforms.yaml")
+        self.convert = Convert()
         self.data = dict()
 
+    def __del__(self):
+        log.debug("Closing output file")
+        self.footer()
+
     def isclosed(self):
         return self.file.closed
 
     def header(self):
-        if self.file is not False:
+        if self.file is not None:
             self.file.write("<?xml version='1.0' encoding='UTF-8'?>\n")
             # self.file.write('<osm version="0.6" generator="osm-fieldowrk 0.3" timestamp="2017-03-13T21:43:02Z">\n')
             self.file.write('<osm version="0.6" generator="osm-fieldwork 0.3">\n')
             self.file.flush()
 
     def footer(self):
         # logging.debug("FIXME: %r" % self.file)
-        self.file.write("</osm>\n")
-        self.file.flush()
-        if self.file is False:
-            self.file.close()
+        if self.file is not None:
+            self.file.write("</osm>\n")
+            self.file.flush()
+            if self.file is False:
+                self.file.close()
 
     def write(self,
               data = None
               ):
         if type(data) == list:
             if data is not None:
                 for line in data:
@@ -168,26 +171,46 @@
         if "tags" in way:
             for key, value in way["tags"].items():
                 if value is None:
                     continue
                 if key == "track":
                     continue
                 if key not in attrs:
-                    newkey = self.convert.escape(key)
+                    newkey = escape(key)
                     osm += "\n    <tag k='%s' v=%r/>" % (newkey, str(value))
             if modified:
                 osm += (
-                    '\n    <tag k="fixme" v="Do not upload this without validation!"/>'
+                    '\n    <tag k="note" v="Do not upload this without validation!"/>'
                 )
             osm += "\n"
 
-        osm += "  </way>"
+        osm += "  </way>\n"
 
         return osm
 
+    def featureToNode(self,
+                     feature: dict
+                     ):
+        """Convert a GeoJson feature into the data structures used here"""
+        osm = dict()
+        ignore = ("label", "title")
+        tags = dict()
+        attrs = dict()
+        for tag, value in feature['properties'].items():
+            if tag == 'id':
+                attrs['osm_id'] = value
+            elif tag not in ignore:
+                tags[tag] = value
+        coords = feature['geometry']['coordinates']
+        attrs['lat'] = coords[1]
+        attrs['lon'] = coords[0]
+        osm['attrs'] = attrs
+        osm['tags'] = tags
+        return osm
+
     def createNode(self,
                    node: dict,
                    modified: bool = False
                    ):
         """This creates a string that is the OSM representation of a node"""
         attrs = dict()
         # Add default attributes
@@ -198,15 +221,15 @@
             attrs["id"] = int(node["attrs"]["id"])
         else:
             attrs["id"] = self.start
             self.start -= 1
         if "version" not in node["attrs"]:
             attrs["version"] = "1"
         else:
-            attrs["version"] = int(node["version"]) + 1
+            attrs["version"] = int(node['attrs']["version"]) + 1
         attrs["lat"] = node["attrs"]["lat"]
         attrs["lon"] = node["attrs"]["lon"]
         attrs["timestamp"] = datetime.now().strftime("%Y-%m-%dT%TZ")
         # If the resulting file is publicly accessible without authentication, THE GDPR applies
         # and the identifying fields should not be included
         if "uid" in node and attrs["uid"] is not None:
             attrs["uid"] = node["uid"]
@@ -225,17 +248,17 @@
             for key, value in node["tags"].items():
                 if not value:
                     continue
                 if key not in attrs:
                     osm += "\n    <tag k='%s' v=%r/>" % (key, str(value))
             if modified:
                 osm += (
-                    '\n    <tag k="fixme" v="Do not upload this without validation!"/>'
+                    '\n    <tag k="note" v="Do not upload this without validation!"/>'
                 )
-            osm += "\n  </node>"
+            osm += "\n  </node>\n"
         else:
             osm += "/>"
 
         return osm
 
     def createTag(self,
                   field: str,
@@ -254,38 +277,58 @@
             newtag = change[0]
             newval = change[1]
 
         tag[newtag] = newval
         return tag
 
     def loadFile(self,
-                 file: str
+                 osmfile: str
                  ):
         """Read a OSM XML file generated by osm_fieldwork"""
-        size = os.path.getsize(file)
-        with open(file, "rb") as file:
+        size = os.path.getsize(osmfile)
+        with open(osmfile, "r") as file:
             xml = file.read(size)  # Instances are small, read the whole file
             doc = xmltodict.parse(xml)
             if "osm" not in doc:
                 logging.warning("No data in this instance")
                 return False
             field = doc["osm"]
-        for node in field["node"]:
-            attrs = {
-                "id": node["@id"],
-                "lat": node["@lat"],
-                "lon": node["@lon"],
-                "timestamp": node["@timestamp"],
-            }
+        if type(field["node"]) == dict:
+            attrs = dict()
             tags = dict()
-            if "tag" in node:
-                for tag in node["tag"]:
-                    tags[tag["@k"]] = tag["@v"].strip()
-                node = {"attrs": attrs, "tags": tags}
-                self.data[node["attrs"]["id"]] = node
+            for k, v in field["node"].items():
+                if k[0] == '@':
+                    attrs[k[1:]] = v
+                else:
+                    for pair in field["node"]['tag']:
+                        tags[pair['@k']] = pair['@v']
+            node = {"attrs": attrs, "tags": tags}
+            self.data[node["attrs"]["id"]] = node
+        else:
+            for node in field["node"]:
+                attrs = {
+                    "id": int(node["@id"]),
+                    "lat": node["@lat"][:10],
+                    "lon": node["@lon"][:10],
+                }
+                if '@timestamp' in node:
+                    attrs["timestamp"] = node["@timestamp"]
+
+                tags = dict()
+                if "tag" in node:
+                    for tag in node["tag"]:
+                        if type(tag) == dict:
+                            tags[tag["@k"]] = tag["@v"].strip()
+                            # continue
+                        else:
+                            tags[node['tag']["@k"]] = node['tag']["@v"].strip()
+                            # continue
+                    node = {"attrs": attrs, "tags": tags}
+                    self.data[node["attrs"]["id"]] = node
+        return self.data
 
     def dump(self):
         """Dump the contents of an OSM file"""
         for id, item in self.data.items():
             for k, v in item["attrs"].items():
                 print(f"{k} = {v}")
             for k, v in item["tags"].items():
@@ -301,15 +344,15 @@
         """Extract all the tags used in this file"""
         fields = list()
         for id, item in self.data.items():
             keys = list(item["tags"].keys())
             for key in keys:
                 if key not in fields:
                     fields.append(key)
-        print(fields)
+        # print(fields)
 
 
 if __name__ == "__main__":
     # Command Line options
     parser = argparse.ArgumentParser(
         description="This program conflates ODK data with existing features from OSM."
     )
```

### Comparing `osm-fieldwork-0.3.2/osm_fieldwork/sqlite.py` & `osm-fieldwork-0.3.3/osm_fieldwork/sqlite.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/Makefile` & `osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 		"health") category="healthcare";; \
 		"nature") category="natural";; \
 		"amenities") category="amenity";; \
 	esac; \
 	sed -e "s:<data id=\"[a-zA-Z0-9_]*\":<data id=\"$${base} $${target}\":" \
 		-e "s/<h:title>[a-zA-Z0-9_]*</<h:title>$${base} $${target}</" \
 		-e "s,jr://file/[a-zA-Z0-9_]*.geojson,jr://file/$${base}_$${target}.geojson," $< > $${base}_$${target}.xml; \
-	cp -f /tmp/$${target}.geojson $${base}_$${target}.geojson
+	cp -f $${target}.geojson $${base}_$${target}.geojson
 
 # A simple naming convention is used to make it possible to automate as
 # much as possible. The basename of the XLSForm file matches the form_id
 # column in the settings sheet. The make_data_extract.py also uses the
 # same value in the category options.
 # Any associated data extract file from OSM is uploaded as well if it
 # exists. Note that when using an external geojson file, Enketo doesn't
```

### Comparing `osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/__init__.py` & `osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/__init__.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/amenities.xls` & `osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/amenities.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/buildings.xls` & `osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/buildings.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/camping.xls` & `osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/camping.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/cemeteries.xls` & `osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/cemeteries.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/education.xls` & `osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/education.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/health.xls` & `osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/health.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/historical.xls` & `osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/historical.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/hotspring.xls` & `osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/hotspring.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/landusage.xls` & `osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/landusage.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/landuse.xls` & `osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/landuse.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/lib/amenities.csv` & `osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/lib/amenities.csv`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/lib/towns.csv` & `osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/lib/towns.csv`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/nature.xls` & `osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/nature.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/places.xls` & `osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/places.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/religious.xls` & `osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/religious.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/solidwaste.xlsx` & `osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/solidwaste.xlsx`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/toilets.xls` & `osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/toilets.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/transportation.xls` & `osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/transportation.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/waste_collection.xlsx` & `osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/waste_collection.xlsx`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/wastedisposal.xls` & `osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/wastedisposal.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/waterpoints.xls` & `osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/waterpoints.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.2/osm_fieldwork/xlsforms/waterways.xls` & `osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/waterways.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.2/osm_fieldwork/yamlfile.py` & `osm-fieldwork-0.3.3/osm_fieldwork/yamlfile.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.2/tests/Test.yaml` & `osm-fieldwork-0.3.3/tests/Test.yaml`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.2/tests/test.csv` & `osm-fieldwork-0.3.3/tests/test.csv`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.2/tests/test_convert.py` & `osm-fieldwork-0.3.3/tests/test_convert.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,23 +17,25 @@
 #     You should have received a copy of the GNU General Public License
 #     along with Osm-Fieldwork.  If not, see <https:#www.gnu.org/licenses/>.
 #
 
 import os
 import sys
 import argparse
+from osm_fieldwork.xlsforms import xlsforms_path
 from osm_fieldwork.convert import Convert
 
 parser = argparse.ArgumentParser(
     description="Read and convert a CSV file from ODK Central"
 )
 parser.add_argument("--infile", default="tests/test.csv", help="The CSV input file")
 args = parser.parse_args()
 
-csv = Convert("xforms.yaml")
+path = xlsforms_path.replace("/xlsforms", "")
+csv = Convert(f"{path}/xforms.yaml")
 
 def test_get_keyword():
     """Convert a feature"""
     if "sac_scale" in csv.yaml.yaml["tags"]:
         assert 0
     else:
         assert 1
```

### Comparing `osm-fieldwork-0.3.2/tests/test_csv.py` & `osm-fieldwork-0.3.3/tests/test_csv.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,39 +16,46 @@
 #
 #     You should have received a copy of the GNU General Public License
 #     along with osm_fieldwork.  If not, see <https:#www.gnu.org/licenses/>.
 #
 
 import argparse
 import os
-import sys
 from  osm_fieldwork.CSVDump import CSVDump
 
+# find the path to the test data files
+rootdir = os.path.basename(os.getcwd())
+if rootdir == 'tests':
+    rootdir = "."
+elif rootdir == 'main':
+    rootdir = os.getcwd() + "/tests"
+
 parser = argparse.ArgumentParser(
     description="Read and parse a CSV file from ODK Central"
 )
-parser.add_argument("--infile", default="tests/test.csv", help="The CSV input file")
+parser.add_argument("--infile", default=f"{rootdir}/testdata/test.csv", help="The CSV input file")
 args = parser.parse_args()
 csv = CSVDump()
-data = csv.parse("tests/test.csv")
-# print(data)
+print(args)
+data = csv.parse(args.infile)
+print(data)
 
 
 def test_csv():
     """Make sure the CSV file got loaded and parsed"""
     assert len(data) > 0
 
 
 def test_init():
     """Make sure the YAML file got loaded"""
     assert len(csv.yaml.yaml) > 0
 
 
 def test_osm_entry():
-    csv.createOSM("tests/test.osm")
+    csv.createOSM(args.infile)
     line = {
         "timestamp": "2021-09-25T14:27:43.862Z",
         "end": "2021-09-24T17:55:26.194-06:00",
         "today": "2021-09-24",
         "features": "firepit parking caravans",
         "internet": "none",
         "lat": "38.3697403",
@@ -60,8 +67,8 @@
     csv.createEntry(line)
     # assert tmp
 
 
 if __name__ == "__main__":
     test_init()
     test_csv()
-    test_osm_entry()
+    # test_osm_entry()
```

### Comparing `osm-fieldwork-0.3.2/tests/test_osm.py` & `osm-fieldwork-0.3.3/tests/test_osm.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,46 +15,52 @@
 #     GNU General Public License for more details.
 #
 #     You should have received a copy of the GNU General Public License
 #     along with osm_fieldwork.  If not, see <https:#www.gnu.org/licenses/>.
 #
 
 import os
-import sys
-
-sys.path.append(f"{os.getcwd()}/osm_fieldwork")
+from osm_fieldwork.convert import escape
 import argparse
-from osmfile import OsmFile
+from osm_fieldwork.osmfile import OsmFile
+
+# find the path to the test data files
+rootdir = os.path.basename(os.getcwd())
+if rootdir == 'tests':
+    rootdir = "."
+elif rootdir == 'main':
+    rootdir = os.getcwd() + "/tests"
 
 parser = argparse.ArgumentParser(
     description="Read and parse a CSV file from ODK Central"
 )
-parser.add_argument("--infile", default="tests/test.csv", help="The CSV input file")
+parser.add_argument("--infile", default=f"{rootdir}/testdata/odk_pois.osm", help="The CSV input file")
+parser.add_argument("--outfile", default=f"{rootdir}/testdata/test-out.osm", help="The output OSM XML file")
 args = parser.parse_args()
 
 # Delete the test output file
-if os.path.exists("tests/test.osm"):
-    os.remove("tests/test.osm")
+if os.path.exists(args.outfile):
+    os.remove(args.outfile)
 
-osm = OsmFile("tests/test.osm")
+osm = OsmFile(args.outfile)
 
 
 def test_init():
     """Make sure the OSM file is initialized"""
-    assert os.path.exists("tests/test.osm")
+    assert os.path.exists(args.infile)
 
 
 def test_header():
     osm.header()
-    assert os.stat("tests/test.osm").st_size > 0
+    assert os.stat(args.infile).st_size > 0
 
 
 def test_footer():
     osm.footer()
-    tmp = open("tests/test.osm", "r")
+    tmp = open(args.infile, "r")
     lines = tmp.readlines()
     for line in lines:
         last = line
     assert last == "</osm>\n"
 
 
 def test_create_tag():
@@ -112,9 +118,9 @@
     test_footer()
     test_create_tag()
     test_create_node_notags()
     test_create_node_tags()
     test_create_way()
     test_create_node_modified()
     # Delete the test output file
-    if os.path.exists("tests/test.osm"):
-        os.remove("tests/test.osm")
+    if os.path.exists(args.outfile):
+        os.remove(args.outfile)
```

### Comparing `osm-fieldwork-0.3.2/tests/test_yaml.py` & `osm-fieldwork-0.3.3/tests/test_yaml.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,26 +17,26 @@
 #     You should have received a copy of the GNU General Public License
 #     along with osm_fieldwork.  If not, see <https:#www.gnu.org/licenses/>.
 #
 
 import argparse
 import sys
 import os
-
-sys.path.append(f"{os.getcwd()}/osm_fieldwork")
-from yamlfile import YamlFile
+from osm_fieldwork.xlsforms import xlsforms_path
+from osm_fieldwork.yamlfile import YamlFile
 
 parser = argparse.ArgumentParser(description="Read and parse a YAML file")
 parser.add_argument(
-    "--infile", default="osm_fieldwork/xforms.yaml", help="The YAML input file"
+    "--infile", help="The YAML input file"
 )
 args = parser.parse_args()
 
-data = YamlFile(args.infile)
-
+path = xlsforms_path.replace("/xlsforms", "")
+infile = f"{path}/xforms.yaml"
+data = YamlFile(infile)
 
 def test_validate():
     """Tests for things under validate"""
     foo = data.yaml["validate"]
     bar = foo[1]["leisure"]
     assert "firepit" in bar
```

### Comparing `osm-fieldwork-0.3.2/PKG-INFO` & `osm-fieldwork-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osm-fieldwork
-Version: 0.3.2
+Version: 0.3.3
 Summary: Convert CSV files from ODK Central to OSM format.
 License: GPL-3.0-only
 Keywords: fmtm,odk,hot,openstreetmap,opendatakit
 Author-email: Rob Savoye <rob.savoye@hotosm.org>
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

