# Comparing `tmp/open-buildings-0.0.2.tar.gz` & `tmp/open-buildings-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open-buildings-0.0.2.tar", last modified: Fri Jul 21 14:48:10 2023, max compression
+gzip compressed data, was "open-buildings-0.0.4.tar", last modified: Tue Jul 25 16:23:12 2023, max compression
```

## Comparing `open-buildings-0.0.2.tar` & `open-buildings-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:48:10.796347 open-buildings-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-21 14:48:00.000000 open-buildings-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-21 14:48:00.000000 open-buildings-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11086 2023-07-21 14:48:10.796347 open-buildings-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10323 2023-07-21 14:48:00.000000 open-buildings-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:48:10.792347 open-buildings-0.0.2/open_buildings/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-21 14:48:00.000000 open-buildings-0.0.2/open_buildings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-21 14:48:00.000000 open-buildings-0.0.2/open_buildings/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-21 14:48:00.000000 open-buildings-0.0.2/open_buildings/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    19650 2023-07-21 14:48:00.000000 open-buildings-0.0.2/open_buildings/open_buildings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:48:10.792347 open-buildings-0.0.2/open_buildings.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11086 2023-07-21 14:48:10.000000 open-buildings-0.0.2/open_buildings.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-21 14:48:10.000000 open-buildings-0.0.2/open_buildings.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-21 14:48:10.000000 open-buildings-0.0.2/open_buildings.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-21 14:48:10.000000 open-buildings-0.0.2/open_buildings.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 14:48:10.000000 open-buildings-0.0.2/open_buildings.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-21 14:48:10.000000 open-buildings-0.0.2/open_buildings.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-21 14:48:10.000000 open-buildings-0.0.2/open_buildings.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-21 14:48:00.000000 open-buildings-0.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-21 14:48:10.796347 open-buildings-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-07-21 14:48:00.000000 open-buildings-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:23:12.807983 open-buildings-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-25 16:22:55.000000 open-buildings-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-25 16:22:55.000000 open-buildings-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11508 2023-07-25 16:23:12.807983 open-buildings-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10745 2023-07-25 16:22:55.000000 open-buildings-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:23:12.807983 open-buildings-0.0.4/open_buildings/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-25 16:22:55.000000 open-buildings-0.0.4/open_buildings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-07-25 16:22:55.000000 open-buildings-0.0.4/open_buildings/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-25 16:22:55.000000 open-buildings-0.0.4/open_buildings/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16811 2023-07-25 16:22:55.000000 open-buildings-0.0.4/open_buildings/open_buildings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:23:12.807983 open-buildings-0.0.4/open_buildings.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11508 2023-07-25 16:23:12.000000 open-buildings-0.0.4/open_buildings.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-25 16:23:12.000000 open-buildings-0.0.4/open_buildings.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-25 16:23:12.000000 open-buildings-0.0.4/open_buildings.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-25 16:23:12.000000 open-buildings-0.0.4/open_buildings.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 16:23:12.000000 open-buildings-0.0.4/open_buildings.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-25 16:23:12.000000 open-buildings-0.0.4/open_buildings.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-25 16:23:12.000000 open-buildings-0.0.4/open_buildings.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-25 16:22:55.000000 open-buildings-0.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-25 16:23:12.807983 open-buildings-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-07-25 16:22:55.000000 open-buildings-0.0.4/setup.py
```

### Comparing `open-buildings-0.0.2/LICENSE` & `open-buildings-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `open-buildings-0.0.2/PKG-INFO` & `open-buildings-0.0.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-buildings
-Version: 0.0.2
+Version: 0.0.4
 Summary: Tools for working with open building datasets
 Home-page: https://github.com/opengeos/open-buildings
 Author: Chris Holmes
 Author-email: homie@gmail.com
 License: Apache Software License 2.0
 Keywords: open_buildings
 Classifier: Intended Audience :: Developers
@@ -32,38 +32,41 @@
 ## Introduction
 
 This repo is intended to be a set of useful scripts for working with Google's [Open Buildings](https://sites.research.google/open-buildings/)
 dataset, specifically to help translate it into [Cloud Native Geospatial](https://cloudnativegeo.org) formats. The outputs will live
 at <https://beta.source.coop/cholmes/google-open-buildings> so most people can just make use of those directly. But these are intended to
 show the process, and then they've expanded to be a way to benchmark performance. It's an odd mix right now, if I have time I'll try to
 factor out an independent 'performance' CLI to compare processes without being specific to google open buildings and mixing in functionality
-like splitting multipolygons.
+like splitting multipolygons. The repo is now named 'open-buildings', to allow it to potentially grow to be a set of useful scripts to work with
+other open buildings datasets.
 
 This is basically my first Python project, and certainly my first open source one. It is only possible due to ChatGPT, as I'm not a python
 programmer, and not a great programmer in general (coded professionally for about 2 years, then shifted to doing lots of other stuff). So
 it's likely not great code, but it's been fun to iterate on it and seems like it might be useful to others.
 
 ## Installation
 
 Install with pip:
 
 ```bash
 pip install open-buildings
 ```
 
-Now things may sorta work? I spent close to an hour battling this and it seems to install in the local repo directory, but not
-in the venv / path for some reason. So theoretically you should be able to run `gob-tools benchmark 36b_buildings.csv test-output --format parquet`
-from anywhere and have it work. Right now it's only working for me in the repo directory. I think the safest thing is to just do
+This should add a CLI that you can then use. If it's working then:
 
 ```bash
-python google-buildings-cli.py benchmark 36b_buildings.csv test-output --format parquet
+open_buildings
 ```
 
-with the python file. Any help is more than welcome. Maybe next I'll try poetry? This python package management shit is really as bad as everyone says, even
-ChatGPT wasn't able to get me there.
+Should print out a help message. You then should be able run the CLI:
+
+
+```bash
+open_buildings benchmark 36b_buildings.csv test-output-dir --format parquet
+```
 
 The only CSV files that will work are those from Google's Open Buildings dataset.
 
 ## Functionality
 
 So far there is just one 'tool', a CLI built with click that performs two functions:
 
@@ -83,38 +86,49 @@
 │ pandas    │ 0:00:35.763740 │ 0:00:47.535597 │ 0:00:04.880124 │ 0:00:37.751942 │
 ╘═══════════╧════════════════╧════════════════╧════════════════╧════════════════╛
 ```
 
 The full options can be found with `--help` after each command, and I'll put them here for reference:
 
 ```
-Usage: gob-tools convert [OPTIONS] INPUT_PATH OUTPUT_DIRECTORY
+Usage: open_buildings convert [OPTIONS] INPUT_PATH OUTPUT_DIRECTORY
+
+  Converts a CSV or a directory of CSV's to an alternate format. Input CSV's
+  are assumed to be from Google's Open Buildings
 
 Options:
   --format [fgb|parquet|gpkg|shp]
-                                  The output format.
-  --overwrite                     Whether to overwrite existing output files.
-  --process [duckdb|pandas|ogr]   The processing method to use.
+                                  The output format. The default is FlatGeobuf (fgb)
+  --overwrite                     Whether to overwrite any existing output files.
+  --process [duckdb|pandas|ogr]   The processing method to use. The default is 
+                                  pandas.
   --skip-split-multis             Whether to keep multipolygons as they are
-                                  without splitting into their component
-                                  polygons.
+                                  without splitting into their component polygons.
   --verbose                       Whether to print detailed processing
                                   information.
   --help                          Show this message and exit.
 ```
 
 ```
-Usage: gob-tools benchmark [OPTIONS] INPUT_PATH OUTPUT_DIRECTORY
+Usage: open_buildings benchmark [OPTIONS] INPUT_PATH OUTPUT_DIRECTORY
+
+  Runs the convert function on each of the supplied processes and formats,
+  printing the timing of each as a table
 
 Options:
-  --processes TEXT      The processing methods to use.
-  --formats TEXT        The output formats.
+  --processes TEXT      The processing methods to use. One or more of duckdb,
+                        pandas or ogr, in a comma-separated list. Default is
+                        duckdb,pandas,ogr.
+  --formats TEXT        The output formats to benchmark. One or more of fgb,
+                        parquet, shp or gpkg, in a comma-separated list.
+                        Default is fgb,parquet,shp,gpkg.
   --skip-split-multis   Whether to keep multipolygons as they are without
                         splitting into their component polygons.
-  --no-gpq              Disable GPQ conversion.
+  --no-gpq              Disable GPQ conversion. Timing will be faster, but not
+                        valid GeoParquet (until DuckDB adds support)
   --verbose             Whether to print detailed processing information.
   --output-format TEXT  The format of the output. Options: ascii, csv, json.
   --help                Show this message and exit.
 ```
 
 ## Format Notes
```

### Comparing `open-buildings-0.0.2/README.md` & `open-buildings-0.0.4/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -11,38 +11,41 @@
 ## Introduction
 
 This repo is intended to be a set of useful scripts for working with Google's [Open Buildings](https://sites.research.google/open-buildings/)
 dataset, specifically to help translate it into [Cloud Native Geospatial](https://cloudnativegeo.org) formats. The outputs will live
 at <https://beta.source.coop/cholmes/google-open-buildings> so most people can just make use of those directly. But these are intended to
 show the process, and then they've expanded to be a way to benchmark performance. It's an odd mix right now, if I have time I'll try to
 factor out an independent 'performance' CLI to compare processes without being specific to google open buildings and mixing in functionality
-like splitting multipolygons.
+like splitting multipolygons. The repo is now named 'open-buildings', to allow it to potentially grow to be a set of useful scripts to work with
+other open buildings datasets.
 
 This is basically my first Python project, and certainly my first open source one. It is only possible due to ChatGPT, as I'm not a python
 programmer, and not a great programmer in general (coded professionally for about 2 years, then shifted to doing lots of other stuff). So
 it's likely not great code, but it's been fun to iterate on it and seems like it might be useful to others.
 
 ## Installation
 
 Install with pip:
 
 ```bash
 pip install open-buildings
 ```
 
-Now things may sorta work? I spent close to an hour battling this and it seems to install in the local repo directory, but not
-in the venv / path for some reason. So theoretically you should be able to run `gob-tools benchmark 36b_buildings.csv test-output --format parquet`
-from anywhere and have it work. Right now it's only working for me in the repo directory. I think the safest thing is to just do
+This should add a CLI that you can then use. If it's working then:
 
 ```bash
-python google-buildings-cli.py benchmark 36b_buildings.csv test-output --format parquet
+open_buildings
 ```
 
-with the python file. Any help is more than welcome. Maybe next I'll try poetry? This python package management shit is really as bad as everyone says, even
-ChatGPT wasn't able to get me there.
+Should print out a help message. You then should be able run the CLI:
+
+
+```bash
+open_buildings benchmark 36b_buildings.csv test-output-dir --format parquet
+```
 
 The only CSV files that will work are those from Google's Open Buildings dataset.
 
 ## Functionality
 
 So far there is just one 'tool', a CLI built with click that performs two functions:
 
@@ -62,38 +65,49 @@
 │ pandas    │ 0:00:35.763740 │ 0:00:47.535597 │ 0:00:04.880124 │ 0:00:37.751942 │
 ╘═══════════╧════════════════╧════════════════╧════════════════╧════════════════╛
 ```
 
 The full options can be found with `--help` after each command, and I'll put them here for reference:
 
 ```
-Usage: gob-tools convert [OPTIONS] INPUT_PATH OUTPUT_DIRECTORY
+Usage: open_buildings convert [OPTIONS] INPUT_PATH OUTPUT_DIRECTORY
+
+  Converts a CSV or a directory of CSV's to an alternate format. Input CSV's
+  are assumed to be from Google's Open Buildings
 
 Options:
   --format [fgb|parquet|gpkg|shp]
-                                  The output format.
-  --overwrite                     Whether to overwrite existing output files.
-  --process [duckdb|pandas|ogr]   The processing method to use.
+                                  The output format. The default is FlatGeobuf (fgb)
+  --overwrite                     Whether to overwrite any existing output files.
+  --process [duckdb|pandas|ogr]   The processing method to use. The default is 
+                                  pandas.
   --skip-split-multis             Whether to keep multipolygons as they are
-                                  without splitting into their component
-                                  polygons.
+                                  without splitting into their component polygons.
   --verbose                       Whether to print detailed processing
                                   information.
   --help                          Show this message and exit.
 ```
 
 ```
-Usage: gob-tools benchmark [OPTIONS] INPUT_PATH OUTPUT_DIRECTORY
+Usage: open_buildings benchmark [OPTIONS] INPUT_PATH OUTPUT_DIRECTORY
+
+  Runs the convert function on each of the supplied processes and formats,
+  printing the timing of each as a table
 
 Options:
-  --processes TEXT      The processing methods to use.
-  --formats TEXT        The output formats.
+  --processes TEXT      The processing methods to use. One or more of duckdb,
+                        pandas or ogr, in a comma-separated list. Default is
+                        duckdb,pandas,ogr.
+  --formats TEXT        The output formats to benchmark. One or more of fgb,
+                        parquet, shp or gpkg, in a comma-separated list.
+                        Default is fgb,parquet,shp,gpkg.
   --skip-split-multis   Whether to keep multipolygons as they are without
                         splitting into their component polygons.
-  --no-gpq              Disable GPQ conversion.
+  --no-gpq              Disable GPQ conversion. Timing will be faster, but not
+                        valid GeoParquet (until DuckDB adds support)
   --verbose             Whether to print detailed processing information.
   --output-format TEXT  The format of the output. Options: ascii, csv, json.
   --help                Show this message and exit.
 ```
 
 ## Format Notes
```

### Comparing `open-buildings-0.0.2/open_buildings/open_buildings.py` & `open-buildings-0.0.4/open_buildings/open_buildings.py`

 * *Files 10% similar despite different names*

```diff
@@ -460,112 +460,9 @@
                     'process': process,
                     'format': format,
                     'execution_time': str(timedelta(seconds=execution_time)),
                 }
             )
     return results
 
-
-def handle_comma_separated(ctx, param, value):
-    return value.split(',')
-
-
-@cli.command('convert')
-@click.argument('input_path', type=click.Path(exists=True))
-@click.argument('output_directory', type=click.Path(exists=True))
-@click.option(
-    '--format',
-    type=click.Choice(['fgb', 'parquet', 'gpkg', 'shp']),
-    default='fgb',
-    help="The output format.",
-)
-@click.option(
-    '--overwrite', is_flag=True, help="Whether to overwrite existing output files."
-)
-@click.option(
-    '--process',
-    type=click.Choice(['duckdb', 'pandas', 'ogr']),
-    default='pandas',
-    help="The processing method to use.",
-)
-@click.option(
-    '--skip-split-multis',
-    is_flag=True,
-    help="Whether to keep multipolygons as they are without splitting into their component polygons.",
-)
-@click.option(
-    '--verbose', is_flag=True, help="Whether to print detailed processing information."
-)
-def convert(
-    input_path, output_directory, format, overwrite, process, skip_split_multis, verbose
-):
-    process_geometries(
-        input_path,
-        output_directory,
-        format,
-        overwrite,
-        process,
-        not skip_split_multis,
-        verbose,
-    )
-
-
-@cli.command('benchmark')
-@click.argument('input_path', type=click.Path(exists=True))
-@click.argument('output_directory', type=click.Path(exists=True))
-@click.option(
-    '--processes',
-    callback=handle_comma_separated,
-    default='duckdb,pandas,ogr',
-    help="The processing methods to use.",
-)
-@click.option(
-    '--formats',
-    callback=handle_comma_separated,
-    default='fgb,parquet,shp,gpkg',
-    help="The output formats.",
-)
-@click.option(
-    '--skip-split-multis',
-    is_flag=True,
-    help="Whether to keep multipolygons as they are without splitting into their component polygons.",
-)
-@click.option('--no-gpq', is_flag=True, help="Disable GPQ conversion.")
-@click.option(
-    '--verbose', is_flag=True, help="Whether to print detailed processing information."
-)
-@click.option(
-    '--output-format',
-    default='ascii',
-    help="The format of the output. Options: ascii, csv, json.",
-)
-def benchmark(
-    input_path,
-    output_directory,
-    processes,
-    formats,
-    skip_split_multis,
-    no_gpq,
-    verbose,
-    output_format,
-):
-    results = process_benchmark(
-        input_path, output_directory, processes, formats, not skip_split_multis, verbose
-    )
-
-    df = pd.DataFrame(results)
-    df = df.pivot(index='process', columns='format', values='execution_time')
-
-    if output_format == 'ascii':
-        print(
-            tabulate(df, headers="keys", tablefmt="fancy_grid")
-        )  # or "grid" if you prefer
-    elif output_format == 'csv':
-        print(df.to_csv(index=False))
-    elif output_format == 'json':
-        print(df.to_json(orient='split', indent=4))
-    else:
-        raise ValueError('Invalid output format')
-
-
 if __name__ == "__main__":
     cli()
```

### Comparing `open-buildings-0.0.2/open_buildings.egg-info/PKG-INFO` & `open-buildings-0.0.4/open_buildings.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-buildings
-Version: 0.0.2
+Version: 0.0.4
 Summary: Tools for working with open building datasets
 Home-page: https://github.com/opengeos/open-buildings
 Author: Chris Holmes
 Author-email: homie@gmail.com
 License: Apache Software License 2.0
 Keywords: open_buildings
 Classifier: Intended Audience :: Developers
@@ -32,38 +32,41 @@
 ## Introduction
 
 This repo is intended to be a set of useful scripts for working with Google's [Open Buildings](https://sites.research.google/open-buildings/)
 dataset, specifically to help translate it into [Cloud Native Geospatial](https://cloudnativegeo.org) formats. The outputs will live
 at <https://beta.source.coop/cholmes/google-open-buildings> so most people can just make use of those directly. But these are intended to
 show the process, and then they've expanded to be a way to benchmark performance. It's an odd mix right now, if I have time I'll try to
 factor out an independent 'performance' CLI to compare processes without being specific to google open buildings and mixing in functionality
-like splitting multipolygons.
+like splitting multipolygons. The repo is now named 'open-buildings', to allow it to potentially grow to be a set of useful scripts to work with
+other open buildings datasets.
 
 This is basically my first Python project, and certainly my first open source one. It is only possible due to ChatGPT, as I'm not a python
 programmer, and not a great programmer in general (coded professionally for about 2 years, then shifted to doing lots of other stuff). So
 it's likely not great code, but it's been fun to iterate on it and seems like it might be useful to others.
 
 ## Installation
 
 Install with pip:
 
 ```bash
 pip install open-buildings
 ```
 
-Now things may sorta work? I spent close to an hour battling this and it seems to install in the local repo directory, but not
-in the venv / path for some reason. So theoretically you should be able to run `gob-tools benchmark 36b_buildings.csv test-output --format parquet`
-from anywhere and have it work. Right now it's only working for me in the repo directory. I think the safest thing is to just do
+This should add a CLI that you can then use. If it's working then:
 
 ```bash
-python google-buildings-cli.py benchmark 36b_buildings.csv test-output --format parquet
+open_buildings
 ```
 
-with the python file. Any help is more than welcome. Maybe next I'll try poetry? This python package management shit is really as bad as everyone says, even
-ChatGPT wasn't able to get me there.
+Should print out a help message. You then should be able run the CLI:
+
+
+```bash
+open_buildings benchmark 36b_buildings.csv test-output-dir --format parquet
+```
 
 The only CSV files that will work are those from Google's Open Buildings dataset.
 
 ## Functionality
 
 So far there is just one 'tool', a CLI built with click that performs two functions:
 
@@ -83,38 +86,49 @@
 │ pandas    │ 0:00:35.763740 │ 0:00:47.535597 │ 0:00:04.880124 │ 0:00:37.751942 │
 ╘═══════════╧════════════════╧════════════════╧════════════════╧════════════════╛
 ```
 
 The full options can be found with `--help` after each command, and I'll put them here for reference:
 
 ```
-Usage: gob-tools convert [OPTIONS] INPUT_PATH OUTPUT_DIRECTORY
+Usage: open_buildings convert [OPTIONS] INPUT_PATH OUTPUT_DIRECTORY
+
+  Converts a CSV or a directory of CSV's to an alternate format. Input CSV's
+  are assumed to be from Google's Open Buildings
 
 Options:
   --format [fgb|parquet|gpkg|shp]
-                                  The output format.
-  --overwrite                     Whether to overwrite existing output files.
-  --process [duckdb|pandas|ogr]   The processing method to use.
+                                  The output format. The default is FlatGeobuf (fgb)
+  --overwrite                     Whether to overwrite any existing output files.
+  --process [duckdb|pandas|ogr]   The processing method to use. The default is 
+                                  pandas.
   --skip-split-multis             Whether to keep multipolygons as they are
-                                  without splitting into their component
-                                  polygons.
+                                  without splitting into their component polygons.
   --verbose                       Whether to print detailed processing
                                   information.
   --help                          Show this message and exit.
 ```
 
 ```
-Usage: gob-tools benchmark [OPTIONS] INPUT_PATH OUTPUT_DIRECTORY
+Usage: open_buildings benchmark [OPTIONS] INPUT_PATH OUTPUT_DIRECTORY
+
+  Runs the convert function on each of the supplied processes and formats,
+  printing the timing of each as a table
 
 Options:
-  --processes TEXT      The processing methods to use.
-  --formats TEXT        The output formats.
+  --processes TEXT      The processing methods to use. One or more of duckdb,
+                        pandas or ogr, in a comma-separated list. Default is
+                        duckdb,pandas,ogr.
+  --formats TEXT        The output formats to benchmark. One or more of fgb,
+                        parquet, shp or gpkg, in a comma-separated list.
+                        Default is fgb,parquet,shp,gpkg.
   --skip-split-multis   Whether to keep multipolygons as they are without
                         splitting into their component polygons.
-  --no-gpq              Disable GPQ conversion.
+  --no-gpq              Disable GPQ conversion. Timing will be faster, but not
+                        valid GeoParquet (until DuckDB adds support)
   --verbose             Whether to print detailed processing information.
   --output-format TEXT  The format of the output. Options: ascii, csv, json.
   --help                Show this message and exit.
 ```
 
 ## Format Notes
```

### Comparing `open-buildings-0.0.2/setup.py` & `open-buildings-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,10 +53,10 @@
     keywords='open_buildings',
     name='open-buildings',
     packages=find_packages(include=['open_buildings', 'open_buildings.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/opengeos/open-buildings',
-    version='0.0.2',
+    version='0.0.4',
     zip_safe=False,
 )
```

