# Comparing `tmp/survey_report_generator-0.0.5.tar.gz` & `tmp/survey_report_generator-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "survey_report_generator-0.0.6.tar", max compression
```

## Comparing `survey_report_generator-0.0.5.tar` & `survey_report_generator-0.0.6.tar`

### file list

```diff
@@ -1,26 +1,22 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 survey_report_generator-0.0.5/.DS_Store
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 survey_report_generator-0.0.5/requirements.txt
--rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 survey_report_generator-0.0.5/survey_report_generator/.DS_Store
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 survey_report_generator-0.0.5/survey_report_generator/__init__.py
--rw-r--r--   0        0        0    10617 2020-02-02 00:00:00.000000 survey_report_generator-0.0.5/survey_report_generator/databases.py
--rw-r--r--   0        0        0    12225 2020-02-02 00:00:00.000000 survey_report_generator-0.0.5/survey_report_generator/databases_summary.py
--rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 survey_report_generator-0.0.5/survey_report_generator/date_time.py
--rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 survey_report_generator-0.0.5/survey_report_generator/download_files.py
--rw-r--r--   0        0        0     2646 2020-02-02 00:00:00.000000 survey_report_generator-0.0.5/survey_report_generator/fesm.py
--rw-r--r--   0        0        0     7154 2020-02-02 00:00:00.000000 survey_report_generator-0.0.5/survey_report_generator/figures_utils.py
--rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 survey_report_generator-0.0.5/survey_report_generator/filter_utils.py
--rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 survey_report_generator-0.0.5/survey_report_generator/filter_utils_summary.py
--rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 survey_report_generator-0.0.5/survey_report_generator/g_drive_utils.py
--rw-r--r--   0        0        0     8582 2020-02-02 00:00:00.000000 survey_report_generator-0.0.5/survey_report_generator/generate_report.py
--rw-r--r--   0        0        0     3828 2020-02-02 00:00:00.000000 survey_report_generator-0.0.5/survey_report_generator/koala_habitat.py
--rw-r--r--   0        0        0     2770 2020-02-02 00:00:00.000000 survey_report_generator-0.0.5/survey_report_generator/pct.py
--rw-r--r--   0        0        0  1246571 2020-02-02 00:00:00.000000 survey_report_generator-0.0.5/survey_report_generator/report-template.docx
--rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 survey_report_generator-0.0.5/survey_report_generator/report.py
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 survey_report_generator-0.0.5/survey_report_generator/storage.json
--rw-r--r--   0        0        0     2614 2020-02-02 00:00:00.000000 survey_report_generator-0.0.5/survey_report_generator/summary.py
--rw-r--r--   0        0        0    11371 2020-02-02 00:00:00.000000 survey_report_generator-0.0.5/survey_report_generator/tables.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 survey_report_generator-0.0.5/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 survey_report_generator-0.0.5/LICENSE
--rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 survey_report_generator-0.0.5/README.md
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 survey_report_generator-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     3330 2020-02-02 00:00:00.000000 survey_report_generator-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-05 05:33:37.736436 survey_report_generator-0.0.6/LICENSE
+-rw-r--r--   0        0        0     2834 2023-08-07 10:46:30.714865 survey_report_generator-0.0.6/README.md
+-rw-r--r--   0        0        0      871 2023-08-07 11:25:18.453379 survey_report_generator-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      839 2023-08-07 09:58:08.296356 survey_report_generator-0.0.6/survey_report_generator/__init__.py
+-rw-r--r--   0        0        0    10617 2023-08-07 09:38:48.380575 survey_report_generator-0.0.6/survey_report_generator/databases.py
+-rw-r--r--   0        0        0    12225 2023-08-07 09:38:48.371683 survey_report_generator-0.0.6/survey_report_generator/databases_summary.py
+-rw-r--r--   0        0        0     2965 2023-06-29 03:08:24.254071 survey_report_generator-0.0.6/survey_report_generator/date_time.py
+-rw-r--r--   0        0        0     4665 2023-08-07 10:42:12.482586 survey_report_generator-0.0.6/survey_report_generator/download_files.py
+-rw-r--r--   0        0        0     2646 2023-08-07 09:38:48.352733 survey_report_generator-0.0.6/survey_report_generator/fesm.py
+-rw-r--r--   0        0        0     7154 2023-08-02 01:31:26.062606 survey_report_generator-0.0.6/survey_report_generator/figures_utils.py
+-rw-r--r--   0        0        0     2925 2023-07-12 23:25:21.640034 survey_report_generator-0.0.6/survey_report_generator/filter_utils.py
+-rw-r--r--   0        0        0     3143 2023-06-28 11:49:29.042738 survey_report_generator-0.0.6/survey_report_generator/filter_utils_summary.py
+-rw-r--r--   0        0        0     3353 2023-08-07 09:49:11.581585 survey_report_generator-0.0.6/survey_report_generator/g_drive_utils.py
+-rw-r--r--   0        0        0     8582 2023-08-07 09:54:53.358761 survey_report_generator-0.0.6/survey_report_generator/generate_report.py
+-rw-r--r--   0        0        0     3828 2023-08-07 09:38:48.360972 survey_report_generator-0.0.6/survey_report_generator/koala_habitat.py
+-rw-r--r--   0        0        0     2770 2023-08-07 09:38:48.357342 survey_report_generator-0.0.6/survey_report_generator/pct.py
+-rw-r--r--   0        0        0  1246571 2023-07-25 04:03:13.364594 survey_report_generator-0.0.6/survey_report_generator/report-template.docx
+-rw-r--r--   0        0        0     6630 2023-08-07 09:40:31.415655 survey_report_generator-0.0.6/survey_report_generator/report.py
+-rw-r--r--   0        0        0     1275 2023-08-07 09:49:18.984969 survey_report_generator-0.0.6/survey_report_generator/storage.json
+-rw-r--r--   0        0        0     2614 2023-06-29 02:22:00.019734 survey_report_generator-0.0.6/survey_report_generator/summary.py
+-rw-r--r--   0        0        0    11371 2023-08-07 09:38:48.384945 survey_report_generator-0.0.6/survey_report_generator/tables.py
+-rw-r--r--   0        0        0     4019 1970-01-01 00:00:00.000000 survey_report_generator-0.0.6/PKG-INFO
```

### Comparing `survey_report_generator-0.0.5/survey_report_generator/__init__.py` & `survey_report_generator-0.0.6/survey_report_generator/__init__.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.5/survey_report_generator/databases.py` & `survey_report_generator-0.0.6/survey_report_generator/databases.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.5/survey_report_generator/databases_summary.py` & `survey_report_generator-0.0.6/survey_report_generator/databases_summary.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.5/survey_report_generator/date_time.py` & `survey_report_generator-0.0.6/survey_report_generator/date_time.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.5/survey_report_generator/download_files.py` & `survey_report_generator-0.0.6/survey_report_generator/download_files.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.5/survey_report_generator/fesm.py` & `survey_report_generator-0.0.6/survey_report_generator/fesm.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.5/survey_report_generator/figures_utils.py` & `survey_report_generator-0.0.6/survey_report_generator/figures_utils.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.5/survey_report_generator/filter_utils.py` & `survey_report_generator-0.0.6/survey_report_generator/filter_utils.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.5/survey_report_generator/filter_utils_summary.py` & `survey_report_generator-0.0.6/survey_report_generator/filter_utils_summary.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.5/survey_report_generator/g_drive_utils.py` & `survey_report_generator-0.0.6/survey_report_generator/g_drive_utils.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.5/survey_report_generator/generate_report.py` & `survey_report_generator-0.0.6/survey_report_generator/generate_report.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.5/survey_report_generator/koala_habitat.py` & `survey_report_generator-0.0.6/survey_report_generator/koala_habitat.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.5/survey_report_generator/pct.py` & `survey_report_generator-0.0.6/survey_report_generator/pct.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.5/survey_report_generator/report-template.docx` & `survey_report_generator-0.0.6/survey_report_generator/report-template.docx`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.5/survey_report_generator/report.py` & `survey_report_generator-0.0.6/survey_report_generator/report.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.5/survey_report_generator/storage.json` & `survey_report_generator-0.0.6/survey_report_generator/storage.json`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.5/survey_report_generator/summary.py` & `survey_report_generator-0.0.6/survey_report_generator/summary.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.5/survey_report_generator/tables.py` & `survey_report_generator-0.0.6/survey_report_generator/tables.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.5/LICENSE` & `survey_report_generator-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.5/README.md` & `survey_report_generator-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.5/pyproject.toml` & `survey_report_generator-0.0.6/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 [build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
 
-[project]
+[tool.poetry]
 name = "survey-report-generator"
-version = "0.0.5"
-authors = [
-    { name="Oliver Hahn", email="oliver.a.hahn@gmail.com" },
-]
+version = "0.0.6"
 description = "A tool to generate survey reports from collected data"
+authors = ["Oliver Hahn <oliver.a.hahn@gmail.com>"]
+license = "MIT"  # Assuming your project is MIT licensed based on the classifiers
 readme = "README.md"
-requires-python = ">=3.7"
+homepage = "https://github.com/nsw-wildlife-drone-hub/report-generator"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
-[project.urls]
-"Homepage" = "https://github.com/nsw-wildlife-drone-hub/report-generator"
-
 [tool.poetry.dependencies]
+python = ">=3.7"
 gdown = "^4.7.1"
 oauth2client = "^4.1.3"
 httplib2 = "^0.22.0"
 pandas = "^2.0.1"
 docxtpl = "^0.11.5"
 numpy = "^1.24.3"
 geopandas = "^0.9.0"
 contextily = "^1.3.0"
 shapely = "^2.0.1"
 google-api-python-client = "^2.86.0"
 fiona = "*"
+
```

### Comparing `survey_report_generator-0.0.5/PKG-INFO` & `survey_report_generator-0.0.6/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,35 @@
 Metadata-Version: 2.1
 Name: survey-report-generator
-Version: 0.0.5
+Version: 0.0.6
 Summary: A tool to generate survey reports from collected data
-Project-URL: Homepage, https://github.com/nsw-wildlife-drone-hub/report-generator
-Author-email: Oliver Hahn <oliver.a.hahn@gmail.com>
-License-File: LICENSE
+Home-page: https://github.com/nsw-wildlife-drone-hub/report-generator
+License: MIT
+Author: Oliver Hahn
+Author-email: oliver.a.hahn@gmail.com
+Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: contextily (>=1.3.0,<2.0.0)
+Requires-Dist: docxtpl (>=0.11.5,<0.12.0)
+Requires-Dist: fiona
+Requires-Dist: gdown (>=4.7.1,<5.0.0)
+Requires-Dist: geopandas (>=0.9.0,<0.10.0)
+Requires-Dist: google-api-python-client (>=2.86.0,<3.0.0)
+Requires-Dist: httplib2 (>=0.22.0,<0.23.0)
+Requires-Dist: numpy (>=1.24.3,<2.0.0)
+Requires-Dist: oauth2client (>=4.1.3,<5.0.0)
+Requires-Dist: pandas (>=2.0.1,<3.0.0)
+Requires-Dist: shapely (>=2.0.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Survey Report Generator
 
 [![PyPI version](https://badge.fury.io/py/survey-report-generator.svg)](https://badge.fury.io/py/survey-report-generator)
 
 Report Generator is a Python package used to generate reports for drone surveys. 
@@ -62,7 +79,8 @@
 ```
 
 This will generate folders with databases and figures along with the report itself as a Word document.
 
 ## License
 
 Report Generator is released under the [MIT License](LICENSE).
+
```

