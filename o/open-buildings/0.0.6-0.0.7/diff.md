# Comparing `tmp/open-buildings-0.0.6.tar.gz` & `tmp/open-buildings-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open-buildings-0.0.6.tar", last modified: Wed Jul 26 03:00:04 2023, max compression
+gzip compressed data, was "open-buildings-0.0.7.tar", last modified: Mon Aug  7 13:12:40 2023, max compression
```

## Comparing `open-buildings-0.0.6.tar` & `open-buildings-0.0.7.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 03:00:04.089462 open-buildings-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-26 02:59:53.000000 open-buildings-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-26 02:59:53.000000 open-buildings-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11508 2023-07-26 03:00:04.089462 open-buildings-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10745 2023-07-26 02:59:53.000000 open-buildings-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 03:00:04.089462 open-buildings-0.0.6/open_buildings/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-26 02:59:53.000000 open-buildings-0.0.6/open_buildings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-07-26 02:59:53.000000 open-buildings-0.0.6/open_buildings/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-26 02:59:53.000000 open-buildings-0.0.6/open_buildings/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    16781 2023-07-26 02:59:53.000000 open-buildings-0.0.6/open_buildings/open_buildings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 03:00:04.089462 open-buildings-0.0.6/open_buildings.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11508 2023-07-26 03:00:04.000000 open-buildings-0.0.6/open_buildings.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-26 03:00:04.000000 open-buildings-0.0.6/open_buildings.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-26 03:00:04.000000 open-buildings-0.0.6/open_buildings.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-26 03:00:04.000000 open-buildings-0.0.6/open_buildings.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 03:00:04.000000 open-buildings-0.0.6/open_buildings.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-26 03:00:04.000000 open-buildings-0.0.6/open_buildings.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-26 03:00:04.000000 open-buildings-0.0.6/open_buildings.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-26 02:59:53.000000 open-buildings-0.0.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-26 03:00:04.089462 open-buildings-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-07-26 02:59:53.000000 open-buildings-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:12:40.561011 open-buildings-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-08-07 13:12:28.000000 open-buildings-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-08-07 13:12:28.000000 open-buildings-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11780 2023-08-07 13:12:40.561011 open-buildings-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11017 2023-08-07 13:12:28.000000 open-buildings-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:12:40.561011 open-buildings-0.0.7/open_buildings/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-07 13:12:28.000000 open-buildings-0.0.7/open_buildings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-08-07 13:12:28.000000 open-buildings-0.0.7/open_buildings/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-08-07 13:12:28.000000 open-buildings-0.0.7/open_buildings/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17400 2023-08-07 13:12:28.000000 open-buildings-0.0.7/open_buildings/open_buildings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-08-07 13:12:28.000000 open-buildings-0.0.7/open_buildings/overture-buildings-by-country.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-08-07 13:12:28.000000 open-buildings-0.0.7/open_buildings/overture-buildings-parquet-add-columns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:12:40.561011 open-buildings-0.0.7/open_buildings.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11780 2023-08-07 13:12:40.000000 open-buildings-0.0.7/open_buildings.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-08-07 13:12:40.000000 open-buildings-0.0.7/open_buildings.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-07 13:12:40.000000 open-buildings-0.0.7/open_buildings.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-07 13:12:40.000000 open-buildings-0.0.7/open_buildings.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 13:12:40.000000 open-buildings-0.0.7/open_buildings.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-07 13:12:40.000000 open-buildings-0.0.7/open_buildings.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-07 13:12:40.000000 open-buildings-0.0.7/open_buildings.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-07 13:12:28.000000 open-buildings-0.0.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-08-07 13:12:40.561011 open-buildings-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-08-07 13:12:28.000000 open-buildings-0.0.7/setup.py
```

### Comparing `open-buildings-0.0.6/LICENSE` & `open-buildings-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `open-buildings-0.0.6/PKG-INFO` & `open-buildings-0.0.7/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: open-buildings
-Version: 0.0.6
-Summary: Tools for working with open building datasets
-Home-page: https://github.com/opengeos/open-buildings
-Author: Chris Holmes
-Author-email: homie@gmail.com
-License: Apache Software License 2.0
-Keywords: open_buildings
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # open-buildings
 
 [![image](https://img.shields.io/pypi/v/open_buildings.svg)](https://pypi.python.org/pypi/open_buildings)
 
 **Tools for working with open building datasets**
 
 -   Free software: Apache Software License 2.0
@@ -69,26 +48,27 @@
 ## Functionality
 
 So far there is just one 'tool', a CLI built with click that performs two functions:
 
 -   `convert` takes as input either a single CSV file or a directory of CSV files, downloaded locally from the Google Buildings dataset. It can write out as GeoParquet, FlatGeobuf, GeoPackage and Shapefile, and can process the data using DuckDB, GeoPandas or OGR.
 -   `benchmark` runs the convert command against one or more different formats, and one or more different processes, and reports out how long each took.
 
-A sample output for `benchmark`, run on 36b_buildings.csv, a 130 mb CSV file is:
+A sample output for `benchmark`, run on 219_buildings.csv, a 101 mb CSV file is:
 
 ```
-╒═══════════╤════════════════╤════════════════╤════════════════╤════════════════╕
-│ process   │ fgb            │ gpkg           │ parquet        │ shp            │
-╞═══════════╪════════════════╪════════════════╪════════════════╪════════════════╡
-│ duckdb    │ 0:00:04.287083 │ 0:01:52.222495 │ 0:00:02.880891 │ 0:00:05.404221 │
-├───────────┼────────────────┼────────────────┼────────────────┼────────────────┤
-│ ogr       │ 0:00:03.620750 │ 0:00:08.528865 │ 0:00:02.319576 │ 0:00:03.609031 │
-├───────────┼────────────────┼────────────────┼────────────────┼────────────────┤
-│ pandas    │ 0:00:35.763740 │ 0:00:47.535597 │ 0:00:04.880124 │ 0:00:37.751942 │
-╘═══════════╧════════════════╧════════════════╧════════════════╧════════════════╛
+Table for file: 219_buildings.csv
+╒═══════════╤═══════════╤═══════════╤═══════════╤═══════════╕
+│ process   │ fgb       │ gpkg      │ parquet   │ shp       │
+╞═══════════╪═══════════╪═══════════╪═══════════╪═══════════╡
+│ duckdb    │ 00:02.330 │ 00:00.000 │ 00:01.866 │ 00:03.119 │
+├───────────┼───────────┼───────────┼───────────┼───────────┤
+│ ogr       │ 00:02.034 │ 00:07.456 │ 00:01.423 │ 00:02.491 │
+├───────────┼───────────┼───────────┼───────────┼───────────┤
+│ pandas    │ 00:18.184 │ 00:24.096 │ 00:02.710 │ 00:20.032 │
+╘═══════════╧═══════════╧═══════════╧═══════════╧═══════════╛
 ```
 
 The full options can be found with `--help` after each command, and I'll put them here for reference:
 
 ```
 Usage: open_buildings convert [OPTIONS] INPUT_PATH OUTPUT_DIRECTORY
 
@@ -122,42 +102,45 @@
                         parquet, shp or gpkg, in a comma-separated list.
                         Default is fgb,parquet,shp,gpkg.
   --skip-split-multis   Whether to keep multipolygons as they are without
                         splitting into their component polygons.
   --no-gpq              Disable GPQ conversion. Timing will be faster, but not
                         valid GeoParquet (until DuckDB adds support)
   --verbose             Whether to print detailed processing information.
-  --output-format TEXT  The format of the output. Options: ascii, csv, json.
+  --output-format TEXT  The format of the output. Options: ascii, csv, json,
+                        chart.
   --help                Show this message and exit.
 ```
 
+**Warning** - note that `--no-gpq` doesn't actually work right now, see https://github.com/opengeos/open-buildings/issues/4 to track. It is just always set to true, so DuckDB times with Parquet will be inflated (you can change it in the Python code in a global variables). Note also that the `ogr` process does not work with `--skip-split-multis`, but will just report very minimal times since it skips doing anything, see https://github.com/opengeos/open-buildings/issues/5 to track.
+
 ## Format Notes
 
 I'm mostly focused on GeoParquet and FlatGeobuf, as good cloud-native geo formats. I included GeoPackage and Shapefile mostly for benchmarking purposes. GeoPackage I think is a good option for Esri and other more legacy software that is slow to adopt new formats. Shapefile is total crap for this use case - it fails on files bigger than 4 gigabytes, and lots of the source S2 Google Building CSV's are bigger, so it's not useful for translating. The truncation of field names is also annoying, since the CSV file didn't try to make short names (nor should it, the limit is silly).
 
 GeoPackage is particularly slow with DuckDB, it's likely got a bit of a bug in it. But it works well with Pandas and OGR.
 
 ## Process Notes
 
 When I was processing V2 of the Google Building's dataset I did most of the initial work with GeoPandas, which was awesome, and has the best GeoParquet implementation. But the size of the data made its all in memory processing untenable. I ended up using PostGIS a decent but, but near the end of that process I discovered DuckDB, and was blown away by it's speed and ability to manage memory well. So for this tool I was mostly focused on those two.
 
-Note that GeoParquet from DuckDB by default runs [gpq](https://github.com/planetlabs/gpq) on the DuckDB Parquet output, which adds a good chunk of processing time. This makes it so the DuckDB processing output is slower than it would be if DuckDB natively wrote GeoParquet metadata, which I believe is on their roadmap. So that will likely emerge as the fastest benchmark time. In the code you can set RUN_GPQ_CONVERSION to false if you want to get a sense of it. In the above benchmark running the Parquet with DuckDB without GPQ conversion at the end resulted in a time of 0:00:01.845316
-
 Note also that currently DuckDB fgb, gpkg and shp output don't include projection information, so if you want to use the output then you'd need to run ogr2ogr on the output. It sounds like that may get fixed pretty soon, so I'm not going to add a step that includes the ogr conversion.
 
 OGR was added later, and as of yet does not yet do the key step of splitting multi-polygons, since it's just using ogr2ogr as a sub-process and I've yet to find a way to do that from the CLI (though knowing GDAL/OGR there probably is one - please let me know). To run the benchmark with it you need to do --skip-split-multis or else the times on it will be 0 (except for Shapefile, since it doesn't differentiate between multipolygons and regular polygons). I hope to add that functionality and get it on par, which may mean using Fiona. But it seems like that may affect performance, since Fiona doesn't use the [GDAL/OGR column-oriented API](https://gdal.org/development/rfc/rfc86_column_oriented_api.html).
 
+### Code customizations
+
+There are 3 options that you can set as global variables in the Python code, but are not yet CLI options. These are:
+
+* `RUN_GPQ_CONVERSION` - whether GeoParquet from DuckDB by default runs [gpq](https://github.com/planetlabs/gpq) on the DuckDB Parquet output, which adds a good chunk of processing time. This makes it so the DuckDB processing output is slower than it would be if DuckDB natively wrote GeoParquet metadata, which I believe is on their roadmap. So that will likely emerge as the fastest benchmark time. In the code you can set `RUN_GPQ_CONVERSION` in the python code to false if you want to get a sense of it. In the above benchmark running the Parquet with DuckDB without GPQ conversion at the end resulted in a time of .76 seconds. 
+* `PARQUET_COMPRESSION` - which compression to use for Parquet encoding. Note that not all processes support all compression options, and also the OGR converter currently ignores this option.
+* `SKIP_DUCK_GPKG` - whether to skip the GeoPackage conversion option on DuckDB, since it takes a long time to run.
+
+
 ## Roadmap
 
 The next tool to write is to add country and admin level 1 attributes from GeoBoundaries. This was the trickiest step in processing v2 buildings.
 This will be an interesting to benchmark, with the options being more like DuckDB and PostGIS (pandas could try but may not work on the biggest ones), and potentially even big query. The next functionality to add after that will be do spatial partitioning, and perhaps after that add Iceberg and Delta Lake and compare those two (I didn't get to that step with the v2 buildings). And perhaps I'll also add a tool to easily grab any data from the partitioned geoparquet on source.coop and get it in the format you want.
 
-## Ideas
-
-I'll try to turn these into tickets, but just wanted to jot down some ways I've thought about evolving the script.
+## Contributing
 
--   Make GPQ a flag to pass in, not hardcoded.
--   Make parquet compression options a flag to pass in and raise appropriate errors about which one can be used.
--   Add the splitting of multipolygons to the ogr process. This may need to make use of Fiona, but that may lose the speed of the [column-oriented API](https://gdal.org/development/rfc/rfc86_column_oriented_api.html) - so may be interesting to have both options to benchmark.
--   Include ability to get the source CSV's directly from the cloud, unzip them and process them.
--   Print out the file sizes of the resulting formats in the benchmark.
--   Add GeoJSON? It seems like crap for this goal of working with huge files, but could be interesting to show performance and size characteristics. I do love GeoJSON, it's one of the best formats, but this is not the use case for it.
+All contributions are welcome, I love running open source projects. I'm clearly just learning to code Python, so there's no judgement about crappy code. And I'm super happy to learn from others about better code. Feel free to sound in on [the issues](https://github.com/opengeos/open-buildings/issues), make new ones, grab one, or make a PR. There's lots of low hanging fruit of things to add. And if you're just starting out programming don't hesitate to ask even basic things in the [discussions](https://github.com/opengeos/open-buildings/discussions).
```

### Comparing `open-buildings-0.0.6/README.md` & `open-buildings-0.0.7/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,28 @@
+Metadata-Version: 2.1
+Name: open-buildings
+Version: 0.0.7
+Summary: Tools for working with open building datasets
+Home-page: https://github.com/opengeos/open-buildings
+Author: Chris Holmes
+Author-email: homie@gmail.com
+License: Apache Software License 2.0
+Keywords: open_buildings
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # open-buildings
 
 [![image](https://img.shields.io/pypi/v/open_buildings.svg)](https://pypi.python.org/pypi/open_buildings)
 
 **Tools for working with open building datasets**
 
 -   Free software: Apache Software License 2.0
@@ -48,26 +69,27 @@
 ## Functionality
 
 So far there is just one 'tool', a CLI built with click that performs two functions:
 
 -   `convert` takes as input either a single CSV file or a directory of CSV files, downloaded locally from the Google Buildings dataset. It can write out as GeoParquet, FlatGeobuf, GeoPackage and Shapefile, and can process the data using DuckDB, GeoPandas or OGR.
 -   `benchmark` runs the convert command against one or more different formats, and one or more different processes, and reports out how long each took.
 
-A sample output for `benchmark`, run on 36b_buildings.csv, a 130 mb CSV file is:
+A sample output for `benchmark`, run on 219_buildings.csv, a 101 mb CSV file is:
 
 ```
-╒═══════════╤════════════════╤════════════════╤════════════════╤════════════════╕
-│ process   │ fgb            │ gpkg           │ parquet        │ shp            │
-╞═══════════╪════════════════╪════════════════╪════════════════╪════════════════╡
-│ duckdb    │ 0:00:04.287083 │ 0:01:52.222495 │ 0:00:02.880891 │ 0:00:05.404221 │
-├───────────┼────────────────┼────────────────┼────────────────┼────────────────┤
-│ ogr       │ 0:00:03.620750 │ 0:00:08.528865 │ 0:00:02.319576 │ 0:00:03.609031 │
-├───────────┼────────────────┼────────────────┼────────────────┼────────────────┤
-│ pandas    │ 0:00:35.763740 │ 0:00:47.535597 │ 0:00:04.880124 │ 0:00:37.751942 │
-╘═══════════╧════════════════╧════════════════╧════════════════╧════════════════╛
+Table for file: 219_buildings.csv
+╒═══════════╤═══════════╤═══════════╤═══════════╤═══════════╕
+│ process   │ fgb       │ gpkg      │ parquet   │ shp       │
+╞═══════════╪═══════════╪═══════════╪═══════════╪═══════════╡
+│ duckdb    │ 00:02.330 │ 00:00.000 │ 00:01.866 │ 00:03.119 │
+├───────────┼───────────┼───────────┼───────────┼───────────┤
+│ ogr       │ 00:02.034 │ 00:07.456 │ 00:01.423 │ 00:02.491 │
+├───────────┼───────────┼───────────┼───────────┼───────────┤
+│ pandas    │ 00:18.184 │ 00:24.096 │ 00:02.710 │ 00:20.032 │
+╘═══════════╧═══════════╧═══════════╧═══════════╧═══════════╛
 ```
 
 The full options can be found with `--help` after each command, and I'll put them here for reference:
 
 ```
 Usage: open_buildings convert [OPTIONS] INPUT_PATH OUTPUT_DIRECTORY
 
@@ -101,42 +123,45 @@
                         parquet, shp or gpkg, in a comma-separated list.
                         Default is fgb,parquet,shp,gpkg.
   --skip-split-multis   Whether to keep multipolygons as they are without
                         splitting into their component polygons.
   --no-gpq              Disable GPQ conversion. Timing will be faster, but not
                         valid GeoParquet (until DuckDB adds support)
   --verbose             Whether to print detailed processing information.
-  --output-format TEXT  The format of the output. Options: ascii, csv, json.
+  --output-format TEXT  The format of the output. Options: ascii, csv, json,
+                        chart.
   --help                Show this message and exit.
 ```
 
+**Warning** - note that `--no-gpq` doesn't actually work right now, see https://github.com/opengeos/open-buildings/issues/4 to track. It is just always set to true, so DuckDB times with Parquet will be inflated (you can change it in the Python code in a global variables). Note also that the `ogr` process does not work with `--skip-split-multis`, but will just report very minimal times since it skips doing anything, see https://github.com/opengeos/open-buildings/issues/5 to track.
+
 ## Format Notes
 
 I'm mostly focused on GeoParquet and FlatGeobuf, as good cloud-native geo formats. I included GeoPackage and Shapefile mostly for benchmarking purposes. GeoPackage I think is a good option for Esri and other more legacy software that is slow to adopt new formats. Shapefile is total crap for this use case - it fails on files bigger than 4 gigabytes, and lots of the source S2 Google Building CSV's are bigger, so it's not useful for translating. The truncation of field names is also annoying, since the CSV file didn't try to make short names (nor should it, the limit is silly).
 
 GeoPackage is particularly slow with DuckDB, it's likely got a bit of a bug in it. But it works well with Pandas and OGR.
 
 ## Process Notes
 
 When I was processing V2 of the Google Building's dataset I did most of the initial work with GeoPandas, which was awesome, and has the best GeoParquet implementation. But the size of the data made its all in memory processing untenable. I ended up using PostGIS a decent but, but near the end of that process I discovered DuckDB, and was blown away by it's speed and ability to manage memory well. So for this tool I was mostly focused on those two.
 
-Note that GeoParquet from DuckDB by default runs [gpq](https://github.com/planetlabs/gpq) on the DuckDB Parquet output, which adds a good chunk of processing time. This makes it so the DuckDB processing output is slower than it would be if DuckDB natively wrote GeoParquet metadata, which I believe is on their roadmap. So that will likely emerge as the fastest benchmark time. In the code you can set RUN_GPQ_CONVERSION to false if you want to get a sense of it. In the above benchmark running the Parquet with DuckDB without GPQ conversion at the end resulted in a time of 0:00:01.845316
-
 Note also that currently DuckDB fgb, gpkg and shp output don't include projection information, so if you want to use the output then you'd need to run ogr2ogr on the output. It sounds like that may get fixed pretty soon, so I'm not going to add a step that includes the ogr conversion.
 
 OGR was added later, and as of yet does not yet do the key step of splitting multi-polygons, since it's just using ogr2ogr as a sub-process and I've yet to find a way to do that from the CLI (though knowing GDAL/OGR there probably is one - please let me know). To run the benchmark with it you need to do --skip-split-multis or else the times on it will be 0 (except for Shapefile, since it doesn't differentiate between multipolygons and regular polygons). I hope to add that functionality and get it on par, which may mean using Fiona. But it seems like that may affect performance, since Fiona doesn't use the [GDAL/OGR column-oriented API](https://gdal.org/development/rfc/rfc86_column_oriented_api.html).
 
+### Code customizations
+
+There are 3 options that you can set as global variables in the Python code, but are not yet CLI options. These are:
+
+* `RUN_GPQ_CONVERSION` - whether GeoParquet from DuckDB by default runs [gpq](https://github.com/planetlabs/gpq) on the DuckDB Parquet output, which adds a good chunk of processing time. This makes it so the DuckDB processing output is slower than it would be if DuckDB natively wrote GeoParquet metadata, which I believe is on their roadmap. So that will likely emerge as the fastest benchmark time. In the code you can set `RUN_GPQ_CONVERSION` in the python code to false if you want to get a sense of it. In the above benchmark running the Parquet with DuckDB without GPQ conversion at the end resulted in a time of .76 seconds. 
+* `PARQUET_COMPRESSION` - which compression to use for Parquet encoding. Note that not all processes support all compression options, and also the OGR converter currently ignores this option.
+* `SKIP_DUCK_GPKG` - whether to skip the GeoPackage conversion option on DuckDB, since it takes a long time to run.
+
+
 ## Roadmap
 
 The next tool to write is to add country and admin level 1 attributes from GeoBoundaries. This was the trickiest step in processing v2 buildings.
 This will be an interesting to benchmark, with the options being more like DuckDB and PostGIS (pandas could try but may not work on the biggest ones), and potentially even big query. The next functionality to add after that will be do spatial partitioning, and perhaps after that add Iceberg and Delta Lake and compare those two (I didn't get to that step with the v2 buildings). And perhaps I'll also add a tool to easily grab any data from the partitioned geoparquet on source.coop and get it in the format you want.
 
-## Ideas
-
-I'll try to turn these into tickets, but just wanted to jot down some ways I've thought about evolving the script.
+## Contributing
 
--   Make GPQ a flag to pass in, not hardcoded.
--   Make parquet compression options a flag to pass in and raise appropriate errors about which one can be used.
--   Add the splitting of multipolygons to the ogr process. This may need to make use of Fiona, but that may lose the speed of the [column-oriented API](https://gdal.org/development/rfc/rfc86_column_oriented_api.html) - so may be interesting to have both options to benchmark.
--   Include ability to get the source CSV's directly from the cloud, unzip them and process them.
--   Print out the file sizes of the resulting formats in the benchmark.
--   Add GeoJSON? It seems like crap for this goal of working with huge files, but could be interesting to show performance and size characteristics. I do love GeoJSON, it's one of the best formats, but this is not the use case for it.
+All contributions are welcome, I love running open source projects. I'm clearly just learning to code Python, so there's no judgement about crappy code. And I'm super happy to learn from others about better code. Feel free to sound in on [the issues](https://github.com/opengeos/open-buildings/issues), make new ones, grab one, or make a PR. There's lots of low hanging fruit of things to add. And if you're just starting out programming don't hesitate to ask even basic things in the [discussions](https://github.com/opengeos/open-buildings/discussions).
```

### Comparing `open-buildings-0.0.6/open_buildings/cli.py` & `open-buildings-0.0.7/open_buildings/cli.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-"""CLI to convert Google Open Building CSV files to alternate formats."""
 import sys
+import os
 import click
 import pandas as pd
+import matplotlib.pyplot as plt
 from open_buildings import process_benchmark, process_geometries
+from datetime import datetime, timedelta
 from tabulate import tabulate
 
 
 @click.group()
 def main():
     """CLI to convert Google Open Building CSV files to alternate formats."""
     pass
@@ -36,16 +38,17 @@
 )
 @click.option('--no-gpq', is_flag=True, help="Disable GPQ conversion. Timing will be faster, but not valid GeoParquet (until DuckDB adds support)")
 @click.option(
     '--verbose', is_flag=True, help="Whether to print detailed processing information."
 )
 @click.option(
     '--output-format',
+    callback=handle_comma_separated,
     default='ascii',
-    help="The format of the output. Options: ascii, csv, json.",
+    help="The format of the output. Options: ascii, csv, json, chart.",
 )
 def benchmark(
     input_path,
     output_directory,
     processes,
     formats,
     skip_split_multis,
@@ -57,24 +60,42 @@
     results = process_benchmark(
         input_path, output_directory, processes, formats, not skip_split_multis, verbose
     )
 
     df = pd.DataFrame(results)
     df = df.pivot(index='process', columns='format', values='execution_time')
 
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
+    base_name = os.path.basename(input_path)
+    file_name, file_ext = os.path.splitext(base_name)
+
+    for format in output_format:
+        if format == 'csv':
+            df.to_csv(f"{output_directory}/{file_name}_benchmark.csv", index=False)
+        elif format == 'json':
+            df.to_json(f"{output_directory}/{file_name}_benchmark.json", orient='split', indent=4)
+        elif format == 'chart':
+            df.plot(kind='bar', rot=0)
+            plt.title(f'Benchmark for file: {base_name}')
+            plt.xlabel('Process')
+            plt.ylabel('Execution Time (in seconds)')
+            plt.tight_layout()
+            plt.savefig(f"{output_directory}/{file_name}_benchmark.png")
+            plt.clf()
+        elif format == 'ascii':
+            # Format execution in the data frame from seconds into a string time with
+            # minutes and seconds str(timedelta(seconds=execution_time))
+            df_formatted = df.copy()
+            for column in df_formatted.columns:
+                df_formatted[column] = df_formatted[column].apply(lambda x: (datetime.min + timedelta(seconds=x)).strftime('%M:%S.%f')[:-3])
+
+            print(f"\nTable for file: {base_name}")
+            print(tabulate(df_formatted, headers="keys", tablefmt="fancy_grid"))
+
+        else:
+            raise ValueError('Invalid output format')
 
 @main.command('convert')
 @click.argument('input_path', type=click.Path(exists=True))
 @click.argument('output_directory', type=click.Path(exists=True))
 @click.option(
     '--format',
     type=click.Choice(['fgb', 'parquet', 'gpkg', 'shp']),
```

### Comparing `open-buildings-0.0.6/open_buildings/open_buildings.py` & `open-buildings-0.0.7/open_buildings/open_buildings.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,24 +13,27 @@
 from shapely.geometry import mapping
 from openlocationcode import openlocationcode as olc
 
 # Global variable, that runs GPQ (https://github.com/planetlabs/gpq) after DuckDB writes the Parquet file.
 # This is necessary because DuckDB does not write the GeoParquet metadata (yet). Once DuckDB implements
 # this feature can be removed. Setting it to false will give a sense of how fast DuckDB will be, but
 # if you want to actually use the output GeoParquet files, set it to True.
-RUN_GPQ_CONVERSION = False
+RUN_GPQ_CONVERSION = True
 
 # Global variable, that sets the compression type for the Parquet files. The two options that
 # will work for both DuckDB and pandas are 'snappy' and 'gzip'. 'snappy' is the default. You can
 # try out brotli with pandas, it seems to give the most compression. DuckDB additional supports
 # zstd, but pandas does not. Note that GPQ conversion on DuckDB output likely keeps the same
 # compression, but I have not tested this. GPQ conversion from Parquet does not yet support
 # the other GPQ compression options.
 PARQUET_COMPRESSION = 'snappy'
 
+# Don't run the DuckDB GPKG conversion if set to true, as it takes a long time, likely due to a bug.
+# It means longer runs and puts one big time on the graphs.
+SKIP_DUCK_GPKG = True
 
 @click.group()
 def cli():
     pass
 
 
 def define_output_paths(input_file_path, output_directory, format):
@@ -181,18 +184,23 @@
             gpq_elapsed_time = gpq_end_time - gpq_start_time
             print(f"Time taken to run gpq: {gpq_elapsed_time:.2f} seconds")
         else:
             print(
                 f"Skipping gpq convert on {output_file_path}. This means the output will be WKB, but it will need to be converted to GeoParquet."
             )
     elif format == 'gpkg':
-        c.execute(
-            f"COPY (SELECT * EXCLUDE geometry, ST_AsWKB(ST_GeomFromText(geometry)) AS geometry from buildings) \
-                TO '{output_file_path}' WITH  (FORMAT GDAL, DRIVER 'GPKG');"
-        )
+        if SKIP_DUCK_GPKG:
+            print(
+                f"Skipping duckdb-gpkg conversion on {output_file_path}, since SKIP_DUCK_GPKG is set to True. There is likely a bug, since it takes way longer and skews the graphs"
+            )
+        else:
+            c.execute(
+                f"COPY (SELECT * EXCLUDE geometry, ST_AsWKB(ST_GeomFromText(geometry)) AS geometry from buildings) \
+                    TO '{output_file_path}' WITH  (FORMAT GDAL, DRIVER 'GPKG');"
+            )
     elif format == 'shp':
         c.execute(
             f"COPY (SELECT * EXCLUDE geometry, ST_AsWKB(ST_GeomFromText(geometry)) AS geometry from buildings) \
                 TO '{output_file_path}' WITH  (FORMAT GDAL, DRIVER 'ESRI Shapefile');"
         )
 
     conn.close()
@@ -450,18 +458,21 @@
                 format,
                 True,
                 process,
                 split_multipolygons,
                 verbose,
             )
             execution_time = time.time() - start_time
+            if process == 'duckdb' and format == 'gpkg' and SKIP_DUCK_GPKG:
+                execution_time = 0
             results.append(
                 {
                     'process': process,
                     'format': format,
-                    'execution_time': str(timedelta(seconds=execution_time)),
+                    #'execution_time': str(timedelta(seconds=execution_time)),
+                    'execution_time': execution_time,
                 }
             )
     return results
 
 if __name__ == "__main__":
     cli()
```

### Comparing `open-buildings-0.0.6/open_buildings.egg-info/PKG-INFO` & `open-buildings-0.0.7/open_buildings.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-buildings
-Version: 0.0.6
+Version: 0.0.7
 Summary: Tools for working with open building datasets
 Home-page: https://github.com/opengeos/open-buildings
 Author: Chris Holmes
 Author-email: homie@gmail.com
 License: Apache Software License 2.0
 Keywords: open_buildings
 Classifier: Intended Audience :: Developers
@@ -69,26 +69,27 @@
 ## Functionality
 
 So far there is just one 'tool', a CLI built with click that performs two functions:
 
 -   `convert` takes as input either a single CSV file or a directory of CSV files, downloaded locally from the Google Buildings dataset. It can write out as GeoParquet, FlatGeobuf, GeoPackage and Shapefile, and can process the data using DuckDB, GeoPandas or OGR.
 -   `benchmark` runs the convert command against one or more different formats, and one or more different processes, and reports out how long each took.
 
-A sample output for `benchmark`, run on 36b_buildings.csv, a 130 mb CSV file is:
+A sample output for `benchmark`, run on 219_buildings.csv, a 101 mb CSV file is:
 
 ```
-╒═══════════╤════════════════╤════════════════╤════════════════╤════════════════╕
-│ process   │ fgb            │ gpkg           │ parquet        │ shp            │
-╞═══════════╪════════════════╪════════════════╪════════════════╪════════════════╡
-│ duckdb    │ 0:00:04.287083 │ 0:01:52.222495 │ 0:00:02.880891 │ 0:00:05.404221 │
-├───────────┼────────────────┼────────────────┼────────────────┼────────────────┤
-│ ogr       │ 0:00:03.620750 │ 0:00:08.528865 │ 0:00:02.319576 │ 0:00:03.609031 │
-├───────────┼────────────────┼────────────────┼────────────────┼────────────────┤
-│ pandas    │ 0:00:35.763740 │ 0:00:47.535597 │ 0:00:04.880124 │ 0:00:37.751942 │
-╘═══════════╧════════════════╧════════════════╧════════════════╧════════════════╛
+Table for file: 219_buildings.csv
+╒═══════════╤═══════════╤═══════════╤═══════════╤═══════════╕
+│ process   │ fgb       │ gpkg      │ parquet   │ shp       │
+╞═══════════╪═══════════╪═══════════╪═══════════╪═══════════╡
+│ duckdb    │ 00:02.330 │ 00:00.000 │ 00:01.866 │ 00:03.119 │
+├───────────┼───────────┼───────────┼───────────┼───────────┤
+│ ogr       │ 00:02.034 │ 00:07.456 │ 00:01.423 │ 00:02.491 │
+├───────────┼───────────┼───────────┼───────────┼───────────┤
+│ pandas    │ 00:18.184 │ 00:24.096 │ 00:02.710 │ 00:20.032 │
+╘═══════════╧═══════════╧═══════════╧═══════════╧═══════════╛
 ```
 
 The full options can be found with `--help` after each command, and I'll put them here for reference:
 
 ```
 Usage: open_buildings convert [OPTIONS] INPUT_PATH OUTPUT_DIRECTORY
 
@@ -122,42 +123,45 @@
                         parquet, shp or gpkg, in a comma-separated list.
                         Default is fgb,parquet,shp,gpkg.
   --skip-split-multis   Whether to keep multipolygons as they are without
                         splitting into their component polygons.
   --no-gpq              Disable GPQ conversion. Timing will be faster, but not
                         valid GeoParquet (until DuckDB adds support)
   --verbose             Whether to print detailed processing information.
-  --output-format TEXT  The format of the output. Options: ascii, csv, json.
+  --output-format TEXT  The format of the output. Options: ascii, csv, json,
+                        chart.
   --help                Show this message and exit.
 ```
 
+**Warning** - note that `--no-gpq` doesn't actually work right now, see https://github.com/opengeos/open-buildings/issues/4 to track. It is just always set to true, so DuckDB times with Parquet will be inflated (you can change it in the Python code in a global variables). Note also that the `ogr` process does not work with `--skip-split-multis`, but will just report very minimal times since it skips doing anything, see https://github.com/opengeos/open-buildings/issues/5 to track.
+
 ## Format Notes
 
 I'm mostly focused on GeoParquet and FlatGeobuf, as good cloud-native geo formats. I included GeoPackage and Shapefile mostly for benchmarking purposes. GeoPackage I think is a good option for Esri and other more legacy software that is slow to adopt new formats. Shapefile is total crap for this use case - it fails on files bigger than 4 gigabytes, and lots of the source S2 Google Building CSV's are bigger, so it's not useful for translating. The truncation of field names is also annoying, since the CSV file didn't try to make short names (nor should it, the limit is silly).
 
 GeoPackage is particularly slow with DuckDB, it's likely got a bit of a bug in it. But it works well with Pandas and OGR.
 
 ## Process Notes
 
 When I was processing V2 of the Google Building's dataset I did most of the initial work with GeoPandas, which was awesome, and has the best GeoParquet implementation. But the size of the data made its all in memory processing untenable. I ended up using PostGIS a decent but, but near the end of that process I discovered DuckDB, and was blown away by it's speed and ability to manage memory well. So for this tool I was mostly focused on those two.
 
-Note that GeoParquet from DuckDB by default runs [gpq](https://github.com/planetlabs/gpq) on the DuckDB Parquet output, which adds a good chunk of processing time. This makes it so the DuckDB processing output is slower than it would be if DuckDB natively wrote GeoParquet metadata, which I believe is on their roadmap. So that will likely emerge as the fastest benchmark time. In the code you can set RUN_GPQ_CONVERSION to false if you want to get a sense of it. In the above benchmark running the Parquet with DuckDB without GPQ conversion at the end resulted in a time of 0:00:01.845316
-
 Note also that currently DuckDB fgb, gpkg and shp output don't include projection information, so if you want to use the output then you'd need to run ogr2ogr on the output. It sounds like that may get fixed pretty soon, so I'm not going to add a step that includes the ogr conversion.
 
 OGR was added later, and as of yet does not yet do the key step of splitting multi-polygons, since it's just using ogr2ogr as a sub-process and I've yet to find a way to do that from the CLI (though knowing GDAL/OGR there probably is one - please let me know). To run the benchmark with it you need to do --skip-split-multis or else the times on it will be 0 (except for Shapefile, since it doesn't differentiate between multipolygons and regular polygons). I hope to add that functionality and get it on par, which may mean using Fiona. But it seems like that may affect performance, since Fiona doesn't use the [GDAL/OGR column-oriented API](https://gdal.org/development/rfc/rfc86_column_oriented_api.html).
 
+### Code customizations
+
+There are 3 options that you can set as global variables in the Python code, but are not yet CLI options. These are:
+
+* `RUN_GPQ_CONVERSION` - whether GeoParquet from DuckDB by default runs [gpq](https://github.com/planetlabs/gpq) on the DuckDB Parquet output, which adds a good chunk of processing time. This makes it so the DuckDB processing output is slower than it would be if DuckDB natively wrote GeoParquet metadata, which I believe is on their roadmap. So that will likely emerge as the fastest benchmark time. In the code you can set `RUN_GPQ_CONVERSION` in the python code to false if you want to get a sense of it. In the above benchmark running the Parquet with DuckDB without GPQ conversion at the end resulted in a time of .76 seconds. 
+* `PARQUET_COMPRESSION` - which compression to use for Parquet encoding. Note that not all processes support all compression options, and also the OGR converter currently ignores this option.
+* `SKIP_DUCK_GPKG` - whether to skip the GeoPackage conversion option on DuckDB, since it takes a long time to run.
+
+
 ## Roadmap
 
 The next tool to write is to add country and admin level 1 attributes from GeoBoundaries. This was the trickiest step in processing v2 buildings.
 This will be an interesting to benchmark, with the options being more like DuckDB and PostGIS (pandas could try but may not work on the biggest ones), and potentially even big query. The next functionality to add after that will be do spatial partitioning, and perhaps after that add Iceberg and Delta Lake and compare those two (I didn't get to that step with the v2 buildings). And perhaps I'll also add a tool to easily grab any data from the partitioned geoparquet on source.coop and get it in the format you want.
 
-## Ideas
-
-I'll try to turn these into tickets, but just wanted to jot down some ways I've thought about evolving the script.
+## Contributing
 
--   Make GPQ a flag to pass in, not hardcoded.
--   Make parquet compression options a flag to pass in and raise appropriate errors about which one can be used.
--   Add the splitting of multipolygons to the ogr process. This may need to make use of Fiona, but that may lose the speed of the [column-oriented API](https://gdal.org/development/rfc/rfc86_column_oriented_api.html) - so may be interesting to have both options to benchmark.
--   Include ability to get the source CSV's directly from the cloud, unzip them and process them.
--   Print out the file sizes of the resulting formats in the benchmark.
--   Add GeoJSON? It seems like crap for this goal of working with huge files, but could be interesting to show performance and size characteristics. I do love GeoJSON, it's one of the best formats, but this is not the use case for it.
+All contributions are welcome, I love running open source projects. I'm clearly just learning to code Python, so there's no judgement about crappy code. And I'm super happy to learn from others about better code. Feel free to sound in on [the issues](https://github.com/opengeos/open-buildings/issues), make new ones, grab one, or make a PR. There's lots of low hanging fruit of things to add. And if you're just starting out programming don't hesitate to ask even basic things in the [discussions](https://github.com/opengeos/open-buildings/discussions).
```

### Comparing `open-buildings-0.0.6/setup.py` & `open-buildings-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,10 +53,10 @@
     keywords='open_buildings',
     name='open-buildings',
     packages=find_packages(include=['open_buildings', 'open_buildings.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/opengeos/open-buildings',
-    version='0.0.6',
+    version='0.0.7',
     zip_safe=False,
 )
```

