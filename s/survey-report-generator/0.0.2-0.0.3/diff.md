# Comparing `tmp/survey_report_generator-0.0.2.tar.gz` & `tmp/survey_report_generator-0.0.3.tar.gz`

## Comparing `survey_report_generator-0.0.2.tar` & `survey_report_generator-0.0.3.tar`

### file list

```diff
@@ -1,28 +1,26 @@
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 survey_report_generator-0.0.2/requirements.txt
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 survey_report_generator-0.0.2/src/.DS_Store
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 survey_report_generator-0.0.2/src/__init__.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 survey_report_generator-0.0.2/src/setup.py
--rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 survey_report_generator-0.0.2/src/report_generation/.DS_Store
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 survey_report_generator-0.0.2/src/report_generation/__init__.py
--rw-r--r--   0        0        0    10539 2020-02-02 00:00:00.000000 survey_report_generator-0.0.2/src/report_generation/databases.py
--rw-r--r--   0        0        0    12246 2020-02-02 00:00:00.000000 survey_report_generator-0.0.2/src/report_generation/databases_summary.py
--rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 survey_report_generator-0.0.2/src/report_generation/date_time.py
--rw-r--r--   0        0        0     4858 2020-02-02 00:00:00.000000 survey_report_generator-0.0.2/src/report_generation/download_files.py
--rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 survey_report_generator-0.0.2/src/report_generation/fesm.py
--rw-r--r--   0        0        0     7154 2020-02-02 00:00:00.000000 survey_report_generator-0.0.2/src/report_generation/figures_utils.py
--rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 survey_report_generator-0.0.2/src/report_generation/filter_utils.py
--rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 survey_report_generator-0.0.2/src/report_generation/filter_utils_summary.py
--rw-r--r--   0        0        0     3305 2020-02-02 00:00:00.000000 survey_report_generator-0.0.2/src/report_generation/g_drive_utils.py
--rw-r--r--   0        0        0     8248 2020-02-02 00:00:00.000000 survey_report_generator-0.0.2/src/report_generation/generate_report.py
--rw-r--r--   0        0        0     3827 2020-02-02 00:00:00.000000 survey_report_generator-0.0.2/src/report_generation/koala_habitat.py
--rw-r--r--   0        0        0     2769 2020-02-02 00:00:00.000000 survey_report_generator-0.0.2/src/report_generation/pct.py
--rw-r--r--   0        0        0  1246571 2020-02-02 00:00:00.000000 survey_report_generator-0.0.2/src/report_generation/report-template.docx
--rw-r--r--   0        0        0     6550 2020-02-02 00:00:00.000000 survey_report_generator-0.0.2/src/report_generation/report.py
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 survey_report_generator-0.0.2/src/report_generation/storage.json
--rw-r--r--   0        0        0     2614 2020-02-02 00:00:00.000000 survey_report_generator-0.0.2/src/report_generation/summary.py
--rw-r--r--   0        0        0    11370 2020-02-02 00:00:00.000000 survey_report_generator-0.0.2/src/report_generation/tables.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 survey_report_generator-0.0.2/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 survey_report_generator-0.0.2/LICENSE
--rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 survey_report_generator-0.0.2/README.md
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 survey_report_generator-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3183 2020-02-02 00:00:00.000000 survey_report_generator-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 survey_report_generator-0.0.3/requirements.txt
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 survey_report_generator-0.0.3/setup.py
+-rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 survey_report_generator-0.0.3/survey_report_generator/.DS_Store
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 survey_report_generator-0.0.3/survey_report_generator/__init__.py
+-rw-r--r--   0        0        0    10539 2020-02-02 00:00:00.000000 survey_report_generator-0.0.3/survey_report_generator/databases.py
+-rw-r--r--   0        0        0    12224 2020-02-02 00:00:00.000000 survey_report_generator-0.0.3/survey_report_generator/databases_summary.py
+-rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 survey_report_generator-0.0.3/survey_report_generator/date_time.py
+-rw-r--r--   0        0        0     4858 2020-02-02 00:00:00.000000 survey_report_generator-0.0.3/survey_report_generator/download_files.py
+-rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 survey_report_generator-0.0.3/survey_report_generator/fesm.py
+-rw-r--r--   0        0        0     7154 2020-02-02 00:00:00.000000 survey_report_generator-0.0.3/survey_report_generator/figures_utils.py
+-rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 survey_report_generator-0.0.3/survey_report_generator/filter_utils.py
+-rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 survey_report_generator-0.0.3/survey_report_generator/filter_utils_summary.py
+-rw-r--r--   0        0        0     3305 2020-02-02 00:00:00.000000 survey_report_generator-0.0.3/survey_report_generator/g_drive_utils.py
+-rw-r--r--   0        0        0     8248 2020-02-02 00:00:00.000000 survey_report_generator-0.0.3/survey_report_generator/generate_report.py
+-rw-r--r--   0        0        0     3827 2020-02-02 00:00:00.000000 survey_report_generator-0.0.3/survey_report_generator/koala_habitat.py
+-rw-r--r--   0        0        0     2769 2020-02-02 00:00:00.000000 survey_report_generator-0.0.3/survey_report_generator/pct.py
+-rw-r--r--   0        0        0  1246571 2020-02-02 00:00:00.000000 survey_report_generator-0.0.3/survey_report_generator/report-template.docx
+-rw-r--r--   0        0        0     6554 2020-02-02 00:00:00.000000 survey_report_generator-0.0.3/survey_report_generator/report.py
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 survey_report_generator-0.0.3/survey_report_generator/storage.json
+-rw-r--r--   0        0        0     2614 2020-02-02 00:00:00.000000 survey_report_generator-0.0.3/survey_report_generator/summary.py
+-rw-r--r--   0        0        0    11370 2020-02-02 00:00:00.000000 survey_report_generator-0.0.3/survey_report_generator/tables.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 survey_report_generator-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 survey_report_generator-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 survey_report_generator-0.0.3/README.md
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 survey_report_generator-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3183 2020-02-02 00:00:00.000000 survey_report_generator-0.0.3/PKG-INFO
```

### Comparing `survey_report_generator-0.0.2/src/report_generation/.DS_Store` & `survey_report_generator-0.0.3/survey_report_generator/.DS_Store`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.2/src/report_generation/databases.py` & `survey_report_generator-0.0.3/survey_report_generator/databases.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.2/src/report_generation/databases_summary.py` & `survey_report_generator-0.0.3/survey_report_generator/databases_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pandas as pd
 from shapely.geometry import Polygon
 import numpy as np
 import os
 
 import download_files
-from filter_utils_summary import filter_location, filter_datetime, filter_species_names
+from filter_utils_summary import filter_location, filter_datetime
 
 pd.options.mode.chained_assignment = None  # default='warn'
 
 
 def generate_databases(location_filter, database_location, download_databases, summary=False):
     if download_databases:
         download_files.download_databases(database_location)
```

### Comparing `survey_report_generator-0.0.2/src/report_generation/date_time.py` & `survey_report_generator-0.0.3/survey_report_generator/date_time.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.2/src/report_generation/download_files.py` & `survey_report_generator-0.0.3/survey_report_generator/download_files.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.2/src/report_generation/fesm.py` & `survey_report_generator-0.0.3/survey_report_generator/fesm.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.2/src/report_generation/figures_utils.py` & `survey_report_generator-0.0.3/survey_report_generator/figures_utils.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.2/src/report_generation/filter_utils.py` & `survey_report_generator-0.0.3/survey_report_generator/filter_utils.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.2/src/report_generation/filter_utils_summary.py` & `survey_report_generator-0.0.3/survey_report_generator/filter_utils_summary.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.2/src/report_generation/g_drive_utils.py` & `survey_report_generator-0.0.3/survey_report_generator/g_drive_utils.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.2/src/report_generation/generate_report.py` & `survey_report_generator-0.0.3/survey_report_generator/generate_report.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.2/src/report_generation/koala_habitat.py` & `survey_report_generator-0.0.3/survey_report_generator/koala_habitat.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.2/src/report_generation/pct.py` & `survey_report_generator-0.0.3/survey_report_generator/pct.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.2/src/report_generation/report-template.docx` & `survey_report_generator-0.0.3/survey_report_generator/report-template.docx`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.2/src/report_generation/report.py` & `survey_report_generator-0.0.3/survey_report_generator/report.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 
 import pandas as pd
 
-from src.report_generation import download_files
-from src.report_generation.databases import generate_survey_database, generate_detections_database, \
+from survey_report_generator import download_files
+from survey_report_generator.databases import generate_survey_database, generate_detections_database, \
     generate_airdata_database, generate_kml_database
 
 
 class Report:
     """
     This class represents a report object and includes all variables necessary to extract relevant data to build a
     report.
```

### Comparing `survey_report_generator-0.0.2/src/report_generation/storage.json` & `survey_report_generator-0.0.3/survey_report_generator/storage.json`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.2/src/report_generation/summary.py` & `survey_report_generator-0.0.3/survey_report_generator/summary.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.2/src/report_generation/tables.py` & `survey_report_generator-0.0.3/survey_report_generator/tables.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.2/LICENSE` & `survey_report_generator-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.2/README.md` & `survey_report_generator-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.2/pyproject.toml` & `survey_report_generator-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "survey-report-generator"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
     { name="Oliver Hahn", email="oliver.a.hahn@gmail.com" },
 ]
 description = "A tool to generate survey reports from collected data"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `survey_report_generator-0.0.2/PKG-INFO` & `survey_report_generator-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: survey-report-generator
-Version: 0.0.2
+Version: 0.0.3
 Summary: A tool to generate survey reports from collected data
 Project-URL: Homepage, https://github.com/nsw-wildlife-drone-hub/report-generator
 Author-email: Oliver Hahn <oliver.a.hahn@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

