# Comparing `tmp/stravavis-0.1.0.tar.gz` & `tmp/stravavis-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stravavis-0.1.0.tar", last modified: Fri Dec 30 12:32:54 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `stravavis-0.1.0.tar` & `stravavis-0.2.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 huvankem (692055019) wheel        (0)        0 2022-12-30 12:32:54.244670 stravavis-0.1.0/
--rw-r--r--   0 huvankem (692055019) wheel        (0)     1068 2022-12-30 12:07:30.000000 stravavis-0.1.0/LICENSE
--rw-r--r--   0 huvankem (692055019) wheel        (0)     5433 2022-12-30 12:32:54.244742 stravavis-0.1.0/PKG-INFO
--rw-r--r--   0 huvankem (692055019) wheel        (0)     4403 2022-12-30 12:07:30.000000 stravavis-0.1.0/README.md
--rw-r--r--   0 huvankem (692055019) wheel        (0)     1262 2022-12-30 12:32:54.245453 stravavis-0.1.0/setup.cfg
--rw-r--r--   0 huvankem (692055019) wheel        (0)       38 2022-12-30 12:07:30.000000 stravavis-0.1.0/setup.py
-drwxr-xr-x   0 huvankem (692055019) wheel        (0)        0 2022-12-30 12:32:54.230055 stravavis-0.1.0/src/
-drwxr-xr-x   0 huvankem (692055019) wheel        (0)        0 2022-12-30 12:32:54.240432 stravavis-0.1.0/src/stravavis/
--rw-r--r--   0 huvankem (692055019) wheel        (0)        0 2022-12-30 12:07:30.000000 stravavis-0.1.0/src/stravavis/__init__.py
--rw-r--r--   0 huvankem (692055019) wheel        (0)       69 2022-12-30 12:07:30.000000 stravavis-0.1.0/src/stravavis/__main__.py
--rw-r--r--   0 huvankem (692055019) wheel        (0)     4677 2022-12-30 12:07:30.000000 stravavis-0.1.0/src/stravavis/cli.py
--rw-r--r--   0 huvankem (692055019) wheel        (0)      992 2022-12-30 12:07:30.000000 stravavis-0.1.0/src/stravavis/plot_calendar.py
--rw-r--r--   0 huvankem (692055019) wheel        (0)     2803 2022-12-30 12:07:30.000000 stravavis-0.1.0/src/stravavis/plot_dumbbell.py
--rw-r--r--   0 huvankem (692055019) wheel        (0)     1074 2022-12-30 12:07:30.000000 stravavis-0.1.0/src/stravavis/plot_elevations.py
--rw-r--r--   0 huvankem (692055019) wheel        (0)     1068 2022-12-30 12:07:30.000000 stravavis-0.1.0/src/stravavis/plot_facets.py
--rw-r--r--   0 huvankem (692055019) wheel        (0)     1169 2022-12-30 12:07:30.000000 stravavis-0.1.0/src/stravavis/plot_landscape.py
--rw-r--r--   0 huvankem (692055019) wheel        (0)     1690 2022-12-30 12:07:30.000000 stravavis-0.1.0/src/stravavis/plot_map.py
--rw-r--r--   0 huvankem (692055019) wheel        (0)      231 2022-12-30 12:07:30.000000 stravavis-0.1.0/src/stravavis/process_activities.py
--rw-r--r--   0 huvankem (692055019) wheel        (0)     3170 2022-12-30 12:07:30.000000 stravavis-0.1.0/src/stravavis/process_data.py
-drwxr-xr-x   0 huvankem (692055019) wheel        (0)        0 2022-12-30 12:32:54.244563 stravavis-0.1.0/src/stravavis.egg-info/
--rw-r--r--   0 huvankem (692055019) wheel        (0)     5433 2022-12-30 12:32:54.000000 stravavis-0.1.0/src/stravavis.egg-info/PKG-INFO
--rw-r--r--   0 huvankem (692055019) wheel        (0)      613 2022-12-30 12:32:54.000000 stravavis-0.1.0/src/stravavis.egg-info/SOURCES.txt
--rw-r--r--   0 huvankem (692055019) wheel        (0)        1 2022-12-30 12:32:54.000000 stravavis-0.1.0/src/stravavis.egg-info/dependency_links.txt
--rw-r--r--   0 huvankem (692055019) wheel        (0)       49 2022-12-30 12:32:54.000000 stravavis-0.1.0/src/stravavis.egg-info/entry_points.txt
--rw-r--r--   0 huvankem (692055019) wheel        (0)       61 2022-12-30 12:32:54.000000 stravavis-0.1.0/src/stravavis.egg-info/requires.txt
--rw-r--r--   0 huvankem (692055019) wheel        (0)       10 2022-12-30 12:32:54.000000 stravavis-0.1.0/src/stravavis.egg-info/top_level.txt
--rw-r--r--   0 huvankem (692055019) wheel        (0)        1 2022-12-30 12:31:15.000000 stravavis-0.1.0/src/stravavis.egg-info/zip-safe
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 stravavis-0.2.0/.flake8
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 stravavis-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 stravavis-0.2.0/RELEASING.md
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 stravavis-0.2.0/tox.ini
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 stravavis-0.2.0/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 stravavis-0.2.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stravavis-0.2.0/src/stravavis/__init__.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 stravavis-0.2.0/src/stravavis/__main__.py
+-rw-r--r--   0        0        0     4858 2020-02-02 00:00:00.000000 stravavis-0.2.0/src/stravavis/cli.py
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 stravavis-0.2.0/src/stravavis/plot_calendar.py
+-rw-r--r--   0        0        0     2837 2020-02-02 00:00:00.000000 stravavis-0.2.0/src/stravavis/plot_dumbbell.py
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 stravavis-0.2.0/src/stravavis/plot_elevations.py
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 stravavis-0.2.0/src/stravavis/plot_facets.py
+-rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 stravavis-0.2.0/src/stravavis/plot_landscape.py
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 stravavis-0.2.0/src/stravavis/plot_map.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 stravavis-0.2.0/src/stravavis/process_activities.py
+-rw-r--r--   0        0        0     3187 2020-02-02 00:00:00.000000 stravavis-0.2.0/src/stravavis/process_data.py
+-rw-r--r--   0        0        0     5471 2020-02-02 00:00:00.000000 stravavis-0.2.0/tests/csv/activities.csv
+-rw-r--r--   0        0        0   457385 2020-02-02 00:00:00.000000 stravavis-0.2.0/tests/gpx/activity_7348460494.gpx
+-rw-r--r--   0        0        0  1456905 2020-02-02 00:00:00.000000 stravavis-0.2.0/tests/gpx/activity_7397878357.gpx
+-rw-r--r--   0        0        0   324000 2020-02-02 00:00:00.000000 stravavis-0.2.0/tests/gpx/activity_7448910422.gpx
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 stravavis-0.2.0/tests/gpx/invalid-lon-lat-missing.gpx
+-rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 stravavis-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 stravavis-0.2.0/LICENSE
+-rw-r--r--   0        0        0     4348 2020-02-02 00:00:00.000000 stravavis-0.2.0/README.md
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 stravavis-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5505 2020-02-02 00:00:00.000000 stravavis-0.2.0/PKG-INFO
```

### Comparing `stravavis-0.1.0/LICENSE` & `stravavis-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stravavis-0.1.0/PKG-INFO` & `stravavis-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,45 @@
 Metadata-Version: 2.1
 Name: stravavis
-Version: 0.1.0
+Version: 0.2.0
 Summary: Create artistic visualisations with your exercise data
-Home-page: https://github.com/marcusvolz/strava_py
+Project-URL: Homepage, https://github.com/marcusvolz/strava_py
+Project-URL: Source, https://github.com/marcusvolz/strava_py
 Author: Marcus Volz
+Maintainer: Hugo van Kemenade
 License: MIT
-Project-URL: Source, https://github.com/marcusvolz/strava_py
-Keywords: strava,artistic visualisations,artistic,visualisation,exercise data,exercise
+License-File: LICENSE
+Keywords: artistic,artistic visualisations,exercise,exercise data,strava,visualisation
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Artistic Software
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Topic :: Scientific/Engineering :: Visualization
-Requires-Python: >=3.7
+Requires-Python: >=3.8
+Requires-Dist: calmap
+Requires-Dist: fit2gpx
+Requires-Dist: gpxpy
+Requires-Dist: matplotlib
+Requires-Dist: pandas<2
+Requires-Dist: plotnine
+Requires-Dist: rich
+Requires-Dist: seaborn
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # strava_py
+
 Create artistic visualisations with your exercise data (Python version).
 
-This is a port of the [R strava package](https://github.com/marcusvolz/strava) to Python.
+This is a port of the [R strava package](https://github.com/marcusvolz/strava) to
+Python.
 
 ## Installation
 
 Install via pip:
 
 ```sh
 python3 -m pip install stravavis
@@ -50,15 +59,16 @@
 stravavis --help
 ```
 
 ## Examples
 
 ### Facets
 
-A plot of activities as small multiples. The concept behind this plot was originally inspired by [Sisu](https://twitter.com/madewithsisu).
+A plot of activities as small multiples. The concept behind this plot was originally
+inspired by [Sisu](https://twitter.com/madewithsisu).
 
 ![facets](https://raw.githubusercontent.com/marcusvolz/strava_py/main/plots/facets001.png "Facets, showing activity outlines")
 
 ### Map
 
 A map of activities viewed in plan.
 
@@ -74,47 +84,64 @@
 
 Elevation profiles superimposed.
 
 ![map](https://raw.githubusercontent.com/marcusvolz/strava_py/main/plots/landscape001.png "Elevation profiles superimposed")
 
 ### Calendar
 
-Calendar heatmap showing daily activity distance, using the [calmap](https://pythonhosted.org/calmap/) package. Requires "activities.csv" from the bulk Strava export.
+Calendar heatmap showing daily activity distance, using the
+[calmap](https://pythonhosted.org/calmap/) package. Requires "activities.csv" from the
+bulk Strava export.
 
 ![map](https://raw.githubusercontent.com/marcusvolz/strava_py/main/plots/calendar001.png "Calendar heatmap")
 
 ### Dumbbell plot
 
-Activities shown as horizontal lines by time of day and day of year, facetted by year. Requires "activities.csv" from the bulk Strava export.
+Activities shown as horizontal lines by time of day and day of year, facetted by year.
+Requires "activities.csv" from the bulk Strava export.
 
 ![map](https://raw.githubusercontent.com/marcusvolz/strava_py/main/plots/dumbbell001.png "Dumbbell plot")
 
 ## How to use
 
 ### Bulk export from Strava
-The process for downloading data is described on the Strava website here: [https://support.strava.com/hc/en-us/articles/216918437-Exporting-your-Data-and-Bulk-Export#Bulk], but in essence, do the following:
-                                                                           
+
+The process for downloading data is described on the Strava website here:
+[https://support.strava.com/hc/en-us/articles/216918437-Exporting-your-Data-and-Bulk-Export#Bulk],
+but in essence, do the following:
+
 1. Log in to [Strava](https://www.strava.com/)
-2. Select "[Settings](https://www.strava.com/settings/profile)" from the main drop-down menu at top right of the screen
-3. Select "[My Account](https://www.strava.com/account)" from the navigation menu to the left of the screen.
-4. Under the "[Download or Delete Your Account](https://www.strava.com/athlete/delete_your_account)" heading, click the "Get Started" button.
-5. Under the "Download Request", heading, click the "Request Your Archive" button. ***Don't click anything else on that page, i.e. particularly not the "Request Account Deletion" button.***
+2. Select "[Settings](https://www.strava.com/settings/profile)" from the main drop-down
+   menu at top right of the screen
+3. Select "[My Account](https://www.strava.com/account)" from the navigation menu to the
+   left of the screen.
+4. Under the
+   "[Download or Delete Your Account](https://www.strava.com/athlete/delete_your_account)"
+   heading, click the "Get Started" button.
+5. Under the "Download Request", heading, click the "Request Your Archive" button.
+   **_Don't click anything else on that page, i.e. particularly not the "Request Account
+   Deletion" button._**
 6. Wait for an email to be sent
 7. Click the link in email to download zipped folder containing activities
 8. Unzip files
 
 ### Process the data
 
-The main function for importing and processing activity files expects a path to a directory of unzipped GPX and / or FIT files. If required, the [fit2gpx](https://github.com/dodo-saba/fit2gpx) package provides useful tools for pre-processing bulk files exported from Strava, e.g. unzipping activity files (see Use Case 3: Strava Bulk Export Tools).
+The main function for importing and processing activity files expects a path to a
+directory of unzipped GPX and / or FIT files. If required, the
+[fit2gpx](https://github.com/dodo-saba/fit2gpx) package provides useful tools for
+pre-processing bulk files exported from Strava, e.g. unzipping activity files (see Use
+Case 3: Strava Bulk Export Tools).
 
 ```python
 df = process_data("<path to folder with GPX and / or FIT files>")
 ```
 
-Some plots use the "activities.csv" file from the Strava bulk export zip. For those plots, create an "activities" dataframe using the following function:
+Some plots use the "activities.csv" file from the Strava bulk export zip. For those
+plots, create an "activities" dataframe using the following function:
 
 ```python
 activities = process_activities("<path to activities.csv file>")
 ```
 
 ### Plot activities as small multiples
```

### Comparing `stravavis-0.1.0/README.md` & `stravavis-0.2.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # strava_py
+
 Create artistic visualisations with your exercise data (Python version).
 
-This is a port of the [R strava package](https://github.com/marcusvolz/strava) to Python.
+This is a port of the [R strava package](https://github.com/marcusvolz/strava) to
+Python.
 
 ## Installation
 
 Install via pip:
 
 ```sh
 python3 -m pip install stravavis
@@ -25,15 +27,16 @@
 stravavis --help
 ```
 
 ## Examples
 
 ### Facets
 
-A plot of activities as small multiples. The concept behind this plot was originally inspired by [Sisu](https://twitter.com/madewithsisu).
+A plot of activities as small multiples. The concept behind this plot was originally
+inspired by [Sisu](https://twitter.com/madewithsisu).
 
 ![facets](https://raw.githubusercontent.com/marcusvolz/strava_py/main/plots/facets001.png "Facets, showing activity outlines")
 
 ### Map
 
 A map of activities viewed in plan.
 
@@ -49,47 +52,64 @@
 
 Elevation profiles superimposed.
 
 ![map](https://raw.githubusercontent.com/marcusvolz/strava_py/main/plots/landscape001.png "Elevation profiles superimposed")
 
 ### Calendar
 
-Calendar heatmap showing daily activity distance, using the [calmap](https://pythonhosted.org/calmap/) package. Requires "activities.csv" from the bulk Strava export.
+Calendar heatmap showing daily activity distance, using the
+[calmap](https://pythonhosted.org/calmap/) package. Requires "activities.csv" from the
+bulk Strava export.
 
 ![map](https://raw.githubusercontent.com/marcusvolz/strava_py/main/plots/calendar001.png "Calendar heatmap")
 
 ### Dumbbell plot
 
-Activities shown as horizontal lines by time of day and day of year, facetted by year. Requires "activities.csv" from the bulk Strava export.
+Activities shown as horizontal lines by time of day and day of year, facetted by year.
+Requires "activities.csv" from the bulk Strava export.
 
 ![map](https://raw.githubusercontent.com/marcusvolz/strava_py/main/plots/dumbbell001.png "Dumbbell plot")
 
 ## How to use
 
 ### Bulk export from Strava
-The process for downloading data is described on the Strava website here: [https://support.strava.com/hc/en-us/articles/216918437-Exporting-your-Data-and-Bulk-Export#Bulk], but in essence, do the following:
-                                                                           
+
+The process for downloading data is described on the Strava website here:
+[https://support.strava.com/hc/en-us/articles/216918437-Exporting-your-Data-and-Bulk-Export#Bulk],
+but in essence, do the following:
+
 1. Log in to [Strava](https://www.strava.com/)
-2. Select "[Settings](https://www.strava.com/settings/profile)" from the main drop-down menu at top right of the screen
-3. Select "[My Account](https://www.strava.com/account)" from the navigation menu to the left of the screen.
-4. Under the "[Download or Delete Your Account](https://www.strava.com/athlete/delete_your_account)" heading, click the "Get Started" button.
-5. Under the "Download Request", heading, click the "Request Your Archive" button. ***Don't click anything else on that page, i.e. particularly not the "Request Account Deletion" button.***
+2. Select "[Settings](https://www.strava.com/settings/profile)" from the main drop-down
+   menu at top right of the screen
+3. Select "[My Account](https://www.strava.com/account)" from the navigation menu to the
+   left of the screen.
+4. Under the
+   "[Download or Delete Your Account](https://www.strava.com/athlete/delete_your_account)"
+   heading, click the "Get Started" button.
+5. Under the "Download Request", heading, click the "Request Your Archive" button.
+   **_Don't click anything else on that page, i.e. particularly not the "Request Account
+   Deletion" button._**
 6. Wait for an email to be sent
 7. Click the link in email to download zipped folder containing activities
 8. Unzip files
 
 ### Process the data
 
-The main function for importing and processing activity files expects a path to a directory of unzipped GPX and / or FIT files. If required, the [fit2gpx](https://github.com/dodo-saba/fit2gpx) package provides useful tools for pre-processing bulk files exported from Strava, e.g. unzipping activity files (see Use Case 3: Strava Bulk Export Tools).
+The main function for importing and processing activity files expects a path to a
+directory of unzipped GPX and / or FIT files. If required, the
+[fit2gpx](https://github.com/dodo-saba/fit2gpx) package provides useful tools for
+pre-processing bulk files exported from Strava, e.g. unzipping activity files (see Use
+Case 3: Strava Bulk Export Tools).
 
 ```python
 df = process_data("<path to folder with GPX and / or FIT files>")
 ```
 
-Some plots use the "activities.csv" file from the Strava bulk export zip. For those plots, create an "activities" dataframe using the following function:
+Some plots use the "activities.csv" file from the Strava bulk export zip. For those
+plots, create an "activities" dataframe using the following function:
 
 ```python
 activities = process_activities("<path to activities.csv file>")
 ```
 
 ### Plot activities as small multiples
```

### Comparing `stravavis-0.1.0/src/stravavis/cli.py` & `stravavis-0.2.0/src/stravavis/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,43 +11,65 @@
     )
     parser.add_argument(
         "-o", "--output_prefix", default="strava", help="Prefix for output PNG files"
     )
     parser.add_argument(
         "--lon_min",
         type=float,
-        help="Minimum longitude for plot_map (values less than this are removed from the data)",
+        help="Minimum longitude for plot_map "
+        "(values less than this are removed from the data)",
     )
     parser.add_argument(
         "--lon_max",
         type=float,
-        help="Maximum longitude for plot_map (values greater than this are removed from the data)",
+        help="Maximum longitude for plot_map "
+        "(values greater than this are removed from the data)",
     )
     parser.add_argument(
         "--lat_min",
         type=float,
-        help="Minimum latitude for plot_map (values less than this are removed from the data)",
+        help="Minimum latitude for plot_map "
+        "(values less than this are removed from the data)",
     )
     parser.add_argument(
         "--lat_max",
         type=float,
-        help="Maximum latitude for plot_map (values greater than this are removed from the data)",
+        help="Maximum latitude for plot_map "
+        "(values greater than this are removed from the data)",
     )
     parser.add_argument(
         "--bbox", help="Shortcut for comma-separated LON_MIN,LAT_MIN,LON_MAX,LAT_MAX"
     )
-    parser.add_argument("--alpha", default=0.4, help="Line transparency. 0 = Fully transparent, 1 = No transparency")
+    parser.add_argument(
+        "--alpha",
+        default=0.4,
+        help="Line transparency. 0 = Fully transparent, 1 = No transparency",
+    )
     parser.add_argument("--linewidth", default=0.4, help="Line width")
-    parser.add_argument("--activities_path", help="Path to activities.csv from Strava bulk export zip")
-    parser.add_argument("--year_min", help="The minimum year to use for the calendar heatmap.")
-    parser.add_argument("--year_max", help="The maximum year to use for the calendar heatmap.")
-    parser.add_argument("--max_dist", help="Maximum daily distance for the calendar heatmap; values above this will be capped.")
+    parser.add_argument(
+        "--activities_path", help="Path to activities.csv from Strava bulk export zip"
+    )
+    parser.add_argument(
+        "--year_min", help="The minimum year to use for the calendar heatmap."
+    )
+    parser.add_argument(
+        "--year_max", help="The maximum year to use for the calendar heatmap."
+    )
+    parser.add_argument(
+        "--max_dist",
+        help="Maximum daily distance for the calendar heatmap; "
+        "values above this will be capped.",
+    )
     parser.add_argument("--fig_height", help="Figure height for the calendar heatmap.")
     parser.add_argument("--fig_width", help="Figure width for the calendar heatmap.")
-    parser.add_argument("--local_timezone", help="Timezone for determining local times for activities. See pytz.all_timezones for a list of all timezones.")
+    parser.add_argument(
+        "--local_timezone",
+        help="Timezone for determining local times for activities. "
+        "See pytz.all_timezones for a list of all timezones.",
+    )
     args = parser.parse_args()
 
     # Expand "~" or "~user"
     args.path = os.path.expanduser(args.path)
 
     if os.path.isdir(args.path):
         args.path = os.path.join(args.path, "*")
@@ -110,15 +132,15 @@
     print(f"Saved to {outfile}")
 
     if activities is not None:
         print("Plotting calendar...")
         outfile = f"{args.output_prefix}-calendar.png"
         plot_calendar(activities, output_file=outfile)
         print(f"Saved to {outfile}")
-    
+
         print("Plotting dumbbell...")
         outfile = f"{args.output_prefix}-dumbbell.png"
         plot_dumbbell(activities, output_file=outfile)
         print(f"Saved to {outfile}")
 
 
 if __name__ == "__main__":
```

### Comparing `stravavis-0.1.0/src/stravavis/plot_landscape.py` & `stravavis-0.2.0/src/stravavis/plot_landscape.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 import matplotlib.pyplot as plt
 import pandas as pd
 from rich.progress import track
 
 
-def plot_landscape(df, output_file = 'landscape.png'):
-
+def plot_landscape(df, output_file="landscape.png"):
     # Create a new figure
     plt.figure()
 
     # Convert ele to numeric
-    df['ele'] = pd.to_numeric(df['ele'])
-    
+    df["ele"] = pd.to_numeric(df["ele"])
+
     # Create a list of activity names
-    activities = df['name'].unique()
+    activities = df["name"].unique()
 
     # Normalize dist
     processed = []
 
     for activity in track(activities, "Processing tracks"):
-        df_i = df[df['name'] == activity]
-        df_i["dist_norm"] = (df_i["dist"] - df_i["dist"].min()) / (df_i["dist"].max() - df_i["dist"].min())
+        df_i = df[df["name"] == activity]
+        df_i["dist_norm"] = (df_i["dist"] - df_i["dist"].min()) / (
+            df_i["dist"].max() - df_i["dist"].min()
+        )
         processed.append(df_i)
 
     df = pd.concat(processed)
 
     # Plot activities one by one
     for activity in track(activities, "Plotting activities"):
-        x = df[df['name'] == activity]['dist_norm']
-        y = df[df['name'] == activity]['ele']
-        plt.fill_between(x, y, color='black', alpha=0.03, linewidth=0)
-        plt.plot(x, y, color='black', alpha=0.125, linewidth=0.25)
+        x = df[df["name"] == activity]["dist_norm"]
+        y = df[df["name"] == activity]["ele"]
+        plt.fill_between(x, y, color="black", alpha=0.03, linewidth=0)
+        plt.plot(x, y, color="black", alpha=0.125, linewidth=0.25)
 
     # Update plot aesthetics
-    plt.axis('off')
+    plt.axis("off")
     plt.margins(0)
-    plt.subplots_adjust(left = 0.05, right = 0.95, bottom = 0.05, top = 0.95)
-    plt.savefig(output_file, dpi = 600)
+    plt.subplots_adjust(left=0.05, right=0.95, bottom=0.05, top=0.95)
+    plt.savefig(output_file, dpi=600)
```

### Comparing `stravavis-0.1.0/src/stravavis/plot_map.py` & `stravavis-0.2.0/src/stravavis/plot_map.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,46 +20,53 @@
 
     # Get y value
     mercator_n = log(tan((pi / 4) + (lat_rad / 2)))
     y = (MAP_HEIGHT / 2) + (MAP_WIDTH * mercator_n / (2 * pi))
     return y
 
 
-def plot_map(df, lon_min=None, lon_max= None, lat_min=None, lat_max=None,
-             alpha=0.3, linewidth=0.3, output_file="map.png"):
-
+def plot_map(
+    df,
+    lon_min=None,
+    lon_max=None,
+    lat_min=None,
+    lat_max=None,
+    alpha=0.3,
+    linewidth=0.3,
+    output_file="map.png",
+):
     # Create a new figure
     plt.figure()
 
     # Remove data outside the input ranges for lon / lat
     if lon_min is not None:
-        df = df[df['lon'] >= lon_min]
-    
+        df = df[df["lon"] >= lon_min]
+
     if lon_max is not None:
-        df = df[df['lon'] <= lon_max]
-    
+        df = df[df["lon"] <= lon_max]
+
     if lat_min is not None:
-        df = df[df['lat'] >= lat_min]
-    
+        df = df[df["lat"] >= lat_min]
+
     if lat_max is not None:
-        df = df[df['lat'] <= lat_max]
+        df = df[df["lat"] <= lat_max]
 
     # Create a list of activity names
-    activities = df['name'].unique()
+    activities = df["name"].unique()
 
     # Plot activities one by one
     for activity in track(activities, "Plotting activities"):
-        x = df[df['name'] == activity]['lon']
-        y = df[df['name'] == activity]['lat']
+        x = df[df["name"] == activity]["lon"]
+        y = df[df["name"] == activity]["lat"]
 
         # Transform to Mercator projection so maps aren't squashed away from equator
         x = x.transform(convert_x)
         y = y.transform(convert_y)
 
-        plt.plot(x, y, color='black', alpha=alpha, linewidth=linewidth)
+        plt.plot(x, y, color="black", alpha=alpha, linewidth=linewidth)
 
     # Update plot aesthetics
-    plt.axis('off')
-    plt.axis('equal')
+    plt.axis("off")
+    plt.axis("equal")
     plt.margins(0)
-    plt.subplots_adjust(left = 0.05, right = 0.95, bottom = 0.05, top = 0.95)
-    plt.savefig(output_file, dpi = 600)
+    plt.subplots_adjust(left=0.05, right=0.95, bottom=0.05, top=0.95)
+    plt.savefig(output_file, dpi=600)
```

### Comparing `stravavis-0.1.0/src/stravavis/process_data.py` & `stravavis-0.2.0/src/stravavis/process_data.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,16 +28,16 @@
     lon = []
     lat = []
     ele = []
     time = []
     name = []
     dist = []
 
-    for track in activity.tracks:
-        for segment in track.segments:
+    for activity_track in activity.tracks:
+        for segment in activity_track.segments:
             x0 = activity.tracks[0].segments[0].points[0].longitude
             y0 = activity.tracks[0].segments[0].points[0].latitude
             d0 = 0
             for point in segment.points:
                 x = point.longitude
                 y = point.latitude
                 z = point.elevation
@@ -98,15 +98,14 @@
     )
 
     return df
 
 
 # Function for processing (unzipped) GPX and FIT files in a directory (path)
 def process_data(path):
-
     # Process all files (GPX or FIT)
     filenames = glob.glob(path)
 
     with Pool() as pool:
         try:
             it = pool.imap_unordered(process_file, filenames)
             it = track(it, total=len(filenames), description="Processing")
```

