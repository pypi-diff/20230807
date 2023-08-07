# Comparing `tmp/survey_report_generator-0.0.4.tar.gz` & `tmp/survey_report_generator-0.0.5.tar.gz`

## Comparing `survey_report_generator-0.0.4.tar` & `survey_report_generator-0.0.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 survey_report_generator-0.0.4/.DS_Store
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 survey_report_generator-0.0.4/requirements.txt
--rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 survey_report_generator-0.0.4/survey_report_generator/.DS_Store
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 survey_report_generator-0.0.4/survey_report_generator/__init__.py
--rw-r--r--   0        0        0    10617 2020-02-02 00:00:00.000000 survey_report_generator-0.0.4/survey_report_generator/databases.py
--rw-r--r--   0        0        0    12225 2020-02-02 00:00:00.000000 survey_report_generator-0.0.4/survey_report_generator/databases_summary.py
--rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 survey_report_generator-0.0.4/survey_report_generator/date_time.py
--rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 survey_report_generator-0.0.4/survey_report_generator/download_files.py
--rw-r--r--   0        0        0     2646 2020-02-02 00:00:00.000000 survey_report_generator-0.0.4/survey_report_generator/fesm.py
--rw-r--r--   0        0        0     7154 2020-02-02 00:00:00.000000 survey_report_generator-0.0.4/survey_report_generator/figures_utils.py
--rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 survey_report_generator-0.0.4/survey_report_generator/filter_utils.py
--rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 survey_report_generator-0.0.4/survey_report_generator/filter_utils_summary.py
--rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 survey_report_generator-0.0.4/survey_report_generator/g_drive_utils.py
--rw-r--r--   0        0        0     8582 2020-02-02 00:00:00.000000 survey_report_generator-0.0.4/survey_report_generator/generate_report.py
--rw-r--r--   0        0        0     3828 2020-02-02 00:00:00.000000 survey_report_generator-0.0.4/survey_report_generator/koala_habitat.py
--rw-r--r--   0        0        0     2770 2020-02-02 00:00:00.000000 survey_report_generator-0.0.4/survey_report_generator/pct.py
--rw-r--r--   0        0        0  1246571 2020-02-02 00:00:00.000000 survey_report_generator-0.0.4/survey_report_generator/report-template.docx
--rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 survey_report_generator-0.0.4/survey_report_generator/report.py
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 survey_report_generator-0.0.4/survey_report_generator/storage.json
--rw-r--r--   0        0        0     2614 2020-02-02 00:00:00.000000 survey_report_generator-0.0.4/survey_report_generator/summary.py
--rw-r--r--   0        0        0    11371 2020-02-02 00:00:00.000000 survey_report_generator-0.0.4/survey_report_generator/tables.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 survey_report_generator-0.0.4/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 survey_report_generator-0.0.4/LICENSE
--rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 survey_report_generator-0.0.4/README.md
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 survey_report_generator-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     3330 2020-02-02 00:00:00.000000 survey_report_generator-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 survey_report_generator-0.0.5/.DS_Store
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 survey_report_generator-0.0.5/requirements.txt
+-rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 survey_report_generator-0.0.5/survey_report_generator/.DS_Store
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 survey_report_generator-0.0.5/survey_report_generator/__init__.py
+-rw-r--r--   0        0        0    10617 2020-02-02 00:00:00.000000 survey_report_generator-0.0.5/survey_report_generator/databases.py
+-rw-r--r--   0        0        0    12225 2020-02-02 00:00:00.000000 survey_report_generator-0.0.5/survey_report_generator/databases_summary.py
+-rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 survey_report_generator-0.0.5/survey_report_generator/date_time.py
+-rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 survey_report_generator-0.0.5/survey_report_generator/download_files.py
+-rw-r--r--   0        0        0     2646 2020-02-02 00:00:00.000000 survey_report_generator-0.0.5/survey_report_generator/fesm.py
+-rw-r--r--   0        0        0     7154 2020-02-02 00:00:00.000000 survey_report_generator-0.0.5/survey_report_generator/figures_utils.py
+-rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 survey_report_generator-0.0.5/survey_report_generator/filter_utils.py
+-rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 survey_report_generator-0.0.5/survey_report_generator/filter_utils_summary.py
+-rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 survey_report_generator-0.0.5/survey_report_generator/g_drive_utils.py
+-rw-r--r--   0        0        0     8582 2020-02-02 00:00:00.000000 survey_report_generator-0.0.5/survey_report_generator/generate_report.py
+-rw-r--r--   0        0        0     3828 2020-02-02 00:00:00.000000 survey_report_generator-0.0.5/survey_report_generator/koala_habitat.py
+-rw-r--r--   0        0        0     2770 2020-02-02 00:00:00.000000 survey_report_generator-0.0.5/survey_report_generator/pct.py
+-rw-r--r--   0        0        0  1246571 2020-02-02 00:00:00.000000 survey_report_generator-0.0.5/survey_report_generator/report-template.docx
+-rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 survey_report_generator-0.0.5/survey_report_generator/report.py
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 survey_report_generator-0.0.5/survey_report_generator/storage.json
+-rw-r--r--   0        0        0     2614 2020-02-02 00:00:00.000000 survey_report_generator-0.0.5/survey_report_generator/summary.py
+-rw-r--r--   0        0        0    11371 2020-02-02 00:00:00.000000 survey_report_generator-0.0.5/survey_report_generator/tables.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 survey_report_generator-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 survey_report_generator-0.0.5/LICENSE
+-rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 survey_report_generator-0.0.5/README.md
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 survey_report_generator-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3330 2020-02-02 00:00:00.000000 survey_report_generator-0.0.5/PKG-INFO
```

### Comparing `survey_report_generator-0.0.4/.DS_Store` & `survey_report_generator-0.0.5/.DS_Store`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.4/survey_report_generator/.DS_Store` & `survey_report_generator-0.0.5/survey_report_generator/.DS_Store`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.4/survey_report_generator/__init__.py` & `survey_report_generator-0.0.5/survey_report_generator/__init__.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.4/survey_report_generator/databases.py` & `survey_report_generator-0.0.5/survey_report_generator/databases.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.4/survey_report_generator/databases_summary.py` & `survey_report_generator-0.0.5/survey_report_generator/databases_summary.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.4/survey_report_generator/date_time.py` & `survey_report_generator-0.0.5/survey_report_generator/date_time.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.4/survey_report_generator/download_files.py` & `survey_report_generator-0.0.5/survey_report_generator/download_files.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.4/survey_report_generator/fesm.py` & `survey_report_generator-0.0.5/survey_report_generator/fesm.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.4/survey_report_generator/figures_utils.py` & `survey_report_generator-0.0.5/survey_report_generator/figures_utils.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.4/survey_report_generator/filter_utils.py` & `survey_report_generator-0.0.5/survey_report_generator/filter_utils.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.4/survey_report_generator/filter_utils_summary.py` & `survey_report_generator-0.0.5/survey_report_generator/filter_utils_summary.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.4/survey_report_generator/g_drive_utils.py` & `survey_report_generator-0.0.5/survey_report_generator/g_drive_utils.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.4/survey_report_generator/generate_report.py` & `survey_report_generator-0.0.5/survey_report_generator/generate_report.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.4/survey_report_generator/koala_habitat.py` & `survey_report_generator-0.0.5/survey_report_generator/koala_habitat.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.4/survey_report_generator/pct.py` & `survey_report_generator-0.0.5/survey_report_generator/pct.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.4/survey_report_generator/report-template.docx` & `survey_report_generator-0.0.5/survey_report_generator/report-template.docx`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.4/survey_report_generator/report.py` & `survey_report_generator-0.0.5/survey_report_generator/report.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.4/survey_report_generator/storage.json` & `survey_report_generator-0.0.5/survey_report_generator/storage.json`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.4/survey_report_generator/summary.py` & `survey_report_generator-0.0.5/survey_report_generator/summary.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.4/survey_report_generator/tables.py` & `survey_report_generator-0.0.5/survey_report_generator/tables.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.4/.gitignore` & `survey_report_generator-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.4/LICENSE` & `survey_report_generator-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.4/README.md` & `survey_report_generator-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.4/pyproject.toml` & `survey_report_generator-0.0.5/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,34 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "survey-report-generator"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
     { name="Oliver Hahn", email="oliver.a.hahn@gmail.com" },
 ]
 description = "A tool to generate survey reports from collected data"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/nsw-wildlife-drone-hub/report-generator"
+"Homepage" = "https://github.com/nsw-wildlife-drone-hub/report-generator"
+
+[tool.poetry.dependencies]
+gdown = "^4.7.1"
+oauth2client = "^4.1.3"
+httplib2 = "^0.22.0"
+pandas = "^2.0.1"
+docxtpl = "^0.11.5"
+numpy = "^1.24.3"
+geopandas = "^0.9.0"
+contextily = "^1.3.0"
+shapely = "^2.0.1"
+google-api-python-client = "^2.86.0"
+fiona = "*"
```

### Comparing `survey_report_generator-0.0.4/PKG-INFO` & `survey_report_generator-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: survey-report-generator
-Version: 0.0.4
+Version: 0.0.5
 Summary: A tool to generate survey reports from collected data
 Project-URL: Homepage, https://github.com/nsw-wildlife-drone-hub/report-generator
 Author-email: Oliver Hahn <oliver.a.hahn@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

