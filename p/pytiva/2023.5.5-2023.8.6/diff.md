# Comparing `tmp/pytiva-2023.5.5.tar.gz` & `tmp/pytiva-2023.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytiva-2023.5.5.tar", last modified: Wed May  3 21:31:26 2023, max compression
+gzip compressed data, was "pytiva-2023.8.6.tar", last modified: Mon Aug  7 01:22:25 2023, max compression
```

## Comparing `pytiva-2023.5.5.tar` & `pytiva-2023.8.6.tar`

### file list

```diff
@@ -1,58 +1,64 @@
-drwxrwxr-x   0 tj        (1000) tj        (1000)        0 2023-05-03 21:31:26.957147 pytiva-2023.5.5/
--rw-rw-r--   0 tj        (1000) tj        (1000)    35149 2022-11-20 20:53:47.000000 pytiva-2023.5.5/LICENSE
--rw-rw-r--   0 tj        (1000) tj        (1000)      866 2023-05-03 21:31:26.957147 pytiva-2023.5.5/PKG-INFO
--rw-rw-r--   0 tj        (1000) tj        (1000)      292 2023-04-30 15:42:01.000000 pytiva-2023.5.5/README.md
--rw-rw-r--   0 tj        (1000) tj        (1000)      934 2023-05-03 21:30:57.000000 pytiva-2023.5.5/pyproject.toml
-drwxrwxr-x   0 tj        (1000) tj        (1000)        0 2023-05-03 21:31:26.913145 pytiva-2023.5.5/pytiva/
--rw-rw-r--   0 tj        (1000) tj        (1000)      148 2023-04-21 18:01:43.000000 pytiva-2023.5.5/pytiva/__init__.py
-drwxrwxr-x   0 tj        (1000) tj        (1000)        0 2023-05-03 21:31:26.913145 pytiva-2023.5.5/pytiva/activity/
--rw-rw-r--   0 tj        (1000) tj        (1000)    11122 2023-04-21 19:12:18.000000 pytiva-2023.5.5/pytiva/activity/ActivityDataSet.py
--rw-rw-r--   0 tj        (1000) tj        (1000)      102 2022-11-11 19:52:47.000000 pytiva-2023.5.5/pytiva/activity/__init__.py
--rw-rw-r--   0 tj        (1000) tj        (1000)     1801 2023-04-08 15:20:20.000000 pytiva-2023.5.5/pytiva/activity/utils.py
-drwxrwxr-x   0 tj        (1000) tj        (1000)        0 2023-05-03 21:31:26.925146 pytiva-2023.5.5/pytiva/anesthesia/
--rw-rw-r--   0 tj        (1000) tj        (1000)     3045 2023-04-24 20:11:34.000000 pytiva-2023.5.5/pytiva/anesthesia/AnesthesiaCaseDataSet.py
--rw-rw-r--   0 tj        (1000) tj        (1000)     1988 2023-03-29 01:52:22.000000 pytiva-2023.5.5/pytiva/anesthesia/AnesthesiaCaseEventsDataSet.py
--rw-rw-r--   0 tj        (1000) tj        (1000)     4555 2023-02-14 16:40:11.000000 pytiva-2023.5.5/pytiva/anesthesia/AnesthesiaCaseMedicationsDataSet.py
--rw-rw-r--   0 tj        (1000) tj        (1000)      370 2023-04-01 21:59:08.000000 pytiva-2023.5.5/pytiva/anesthesia/AnesthesiaCaseStaffingDataSet.py
--rw-rw-r--   0 tj        (1000) tj        (1000)      882 2023-04-01 22:53:53.000000 pytiva-2023.5.5/pytiva/anesthesia/AnesthesiaDataSet.py
--rw-rw-r--   0 tj        (1000) tj        (1000)    13292 2023-04-24 20:09:40.000000 pytiva-2023.5.5/pytiva/anesthesia/AnesthesiaStudy.py
--rw-rw-r--   0 tj        (1000) tj        (1000)     2816 2023-04-30 15:32:20.000000 pytiva-2023.5.5/pytiva/anesthesia/EventActivityDefinition.py
--rw-rw-r--   0 tj        (1000) tj        (1000)      465 2023-02-14 22:04:16.000000 pytiva-2023.5.5/pytiva/anesthesia/__init__.py
--rw-rw-r--   0 tj        (1000) tj        (1000)     1571 2023-02-05 18:43:13.000000 pytiva-2023.5.5/pytiva/anesthesia/utils.py
-drwxrwxr-x   0 tj        (1000) tj        (1000)        0 2023-05-03 21:31:26.925146 pytiva-2023.5.5/pytiva/dataset/
--rw-rw-r--   0 tj        (1000) tj        (1000)     5720 2023-04-30 15:37:19.000000 pytiva-2023.5.5/pytiva/dataset/DataSet.py
--rw-rw-r--   0 tj        (1000) tj        (1000)      950 2023-04-09 22:37:45.000000 pytiva-2023.5.5/pytiva/dataset/TimeSeriesDataSet.py
--rw-rw-r--   0 tj        (1000) tj        (1000)       78 2023-04-08 14:19:31.000000 pytiva-2023.5.5/pytiva/dataset/__init__.py
--rw-rw-r--   0 tj        (1000) tj        (1000)       59 2023-05-03 19:02:04.000000 pytiva-2023.5.5/pytiva/requirements.txt
-drwxrwxr-x   0 tj        (1000) tj        (1000)        0 2023-05-03 21:31:26.929146 pytiva-2023.5.5/pytiva/staffing/
--rw-rw-r--   0 tj        (1000) tj        (1000)      273 2023-04-08 15:01:52.000000 pytiva-2023.5.5/pytiva/staffing/CapacityTSDS.py
--rw-rw-r--   0 tj        (1000) tj        (1000)     3042 2022-11-04 18:22:16.000000 pytiva-2023.5.5/pytiva/staffing/ProviderShift.py
--rw-rw-r--   0 tj        (1000) tj        (1000)     3401 2023-04-09 22:37:51.000000 pytiva-2023.5.5/pytiva/staffing/ResourceAssignmentDataSet.py
--rw-rw-r--   0 tj        (1000) tj        (1000)      242 2023-04-01 22:25:45.000000 pytiva-2023.5.5/pytiva/staffing/StaffingDataSet.py
--rw-rw-r--   0 tj        (1000) tj        (1000)      293 2023-04-08 15:02:09.000000 pytiva-2023.5.5/pytiva/staffing/__init__.py
--rw-rw-r--   0 tj        (1000) tj        (1000)     4987 2023-04-07 21:12:34.000000 pytiva-2023.5.5/pytiva/staffing/utils.py
-drwxrwxr-x   0 tj        (1000) tj        (1000)        0 2023-05-03 21:31:26.933146 pytiva-2023.5.5/pytiva/utils/
--rw-rw-r--   0 tj        (1000) tj        (1000)       21 2023-02-01 23:16:37.000000 pytiva-2023.5.5/pytiva/utils/__init__.py
--rw-rw-r--   0 tj        (1000) tj        (1000)     4094 2023-03-28 16:03:27.000000 pytiva-2023.5.5/pytiva/utils/utils.py
-drwxrwxr-x   0 tj        (1000) tj        (1000)        0 2023-05-03 21:31:26.937146 pytiva-2023.5.5/pytiva/viz/
--rw-rw-r--   0 tj        (1000) tj        (1000)       59 2023-04-21 19:08:41.000000 pytiva-2023.5.5/pytiva/viz/__init__.py
--rw-rw-r--   0 tj        (1000) tj        (1000)     2536 2023-04-23 00:26:25.000000 pytiva-2023.5.5/pytiva/viz/gantt.py
-drwxrwxr-x   0 tj        (1000) tj        (1000)        0 2023-05-03 21:31:26.913145 pytiva-2023.5.5/pytiva.egg-info/
--rw-rw-r--   0 tj        (1000) tj        (1000)      866 2023-05-03 21:31:26.000000 pytiva-2023.5.5/pytiva.egg-info/PKG-INFO
--rw-rw-r--   0 tj        (1000) tj        (1000)     1388 2023-05-03 21:31:26.000000 pytiva-2023.5.5/pytiva.egg-info/SOURCES.txt
--rw-rw-r--   0 tj        (1000) tj        (1000)        1 2023-05-03 21:31:26.000000 pytiva-2023.5.5/pytiva.egg-info/dependency_links.txt
--rw-rw-r--   0 tj        (1000) tj        (1000)       59 2023-05-03 21:31:26.000000 pytiva-2023.5.5/pytiva.egg-info/requires.txt
--rw-rw-r--   0 tj        (1000) tj        (1000)        7 2023-05-03 21:31:26.000000 pytiva-2023.5.5/pytiva.egg-info/top_level.txt
--rw-rw-r--   0 tj        (1000) tj        (1000)       38 2023-05-03 21:31:26.957147 pytiva-2023.5.5/setup.cfg
-drwxrwxr-x   0 tj        (1000) tj        (1000)        0 2023-05-03 21:31:26.957147 pytiva-2023.5.5/tests/
--rw-rw-r--   0 tj        (1000) tj        (1000)     1342 2023-05-03 15:27:47.000000 pytiva-2023.5.5/tests/test_ProviderShift.py
--rw-rw-r--   0 tj        (1000) tj        (1000)     3293 2023-05-03 15:27:47.000000 pytiva-2023.5.5/tests/test_ResourceAssignmentDataSet.py
--rw-rw-r--   0 tj        (1000) tj        (1000)      963 2023-05-03 15:27:47.000000 pytiva-2023.5.5/tests/test_activity.py
--rw-rw-r--   0 tj        (1000) tj        (1000)     1676 2023-05-03 15:27:47.000000 pytiva-2023.5.5/tests/test_activity_unduplication_with_meds.py
--rw-rw-r--   0 tj        (1000) tj        (1000)      982 2023-05-03 15:27:47.000000 pytiva-2023.5.5/tests/test_anesthesia.py
--rw-rw-r--   0 tj        (1000) tj        (1000)     1371 2023-05-03 15:27:47.000000 pytiva-2023.5.5/tests/test_anesthesia_case_events_dataset.py
--rw-rw-r--   0 tj        (1000) tj        (1000)     1849 2023-05-03 15:27:47.000000 pytiva-2023.5.5/tests/test_anesthesia_study.py
--rw-rw-r--   0 tj        (1000) tj        (1000)     2590 2023-05-03 15:27:47.000000 pytiva-2023.5.5/tests/test_dataset.py
--rw-rw-r--   0 tj        (1000) tj        (1000)     3532 2023-05-03 15:27:47.000000 pytiva-2023.5.5/tests/test_gantt.py
--rw-rw-r--   0 tj        (1000) tj        (1000)      192 2023-04-09 20:16:13.000000 pytiva-2023.5.5/tests/test_staffing.py
--rw-rw-r--   0 tj        (1000) tj        (1000)     3983 2023-04-23 01:25:52.000000 pytiva-2023.5.5/tests/testconfig.py
+drwxrwxr-x   0 tj        (1000) tj        (1000)        0 2023-08-07 01:22:24.997656 pytiva-2023.8.6/
+-rw-rw-r--   0 tj        (1000) tj        (1000)    35149 2022-11-20 20:53:47.000000 pytiva-2023.8.6/LICENSE
+-rw-rw-r--   0 tj        (1000) tj        (1000)     2503 2023-08-07 01:22:24.997656 pytiva-2023.8.6/PKG-INFO
+-rw-rw-r--   0 tj        (1000) tj        (1000)     1929 2023-05-04 14:56:11.000000 pytiva-2023.8.6/README.md
+-rw-rw-r--   0 tj        (1000) tj        (1000)      954 2023-08-07 01:20:40.000000 pytiva-2023.8.6/pyproject.toml
+drwxrwxr-x   0 tj        (1000) tj        (1000)        0 2023-08-07 01:22:24.949655 pytiva-2023.8.6/pytiva/
+-rw-rw-r--   0 tj        (1000) tj        (1000)      168 2023-08-04 21:44:39.000000 pytiva-2023.8.6/pytiva/__init__.py
+drwxrwxr-x   0 tj        (1000) tj        (1000)        0 2023-08-07 01:22:24.957655 pytiva-2023.8.6/pytiva/activity/
+-rw-rw-r--   0 tj        (1000) tj        (1000)    11122 2023-04-21 19:12:18.000000 pytiva-2023.8.6/pytiva/activity/ActivityDataSet.py
+-rw-rw-r--   0 tj        (1000) tj        (1000)      102 2022-11-11 19:52:47.000000 pytiva-2023.8.6/pytiva/activity/__init__.py
+-rw-rw-r--   0 tj        (1000) tj        (1000)     1785 2023-05-30 15:06:27.000000 pytiva-2023.8.6/pytiva/activity/utils.py
+drwxrwxr-x   0 tj        (1000) tj        (1000)        0 2023-08-07 01:22:24.965655 pytiva-2023.8.6/pytiva/anesthesia/
+-rw-rw-r--   0 tj        (1000) tj        (1000)     3045 2023-04-24 20:11:34.000000 pytiva-2023.8.6/pytiva/anesthesia/AnesthesiaCaseDataSet.py
+-rw-rw-r--   0 tj        (1000) tj        (1000)     1988 2023-03-29 01:52:22.000000 pytiva-2023.8.6/pytiva/anesthesia/AnesthesiaCaseEventsDataSet.py
+-rw-rw-r--   0 tj        (1000) tj        (1000)     4555 2023-02-14 16:40:11.000000 pytiva-2023.8.6/pytiva/anesthesia/AnesthesiaCaseMedicationsDataSet.py
+-rw-rw-r--   0 tj        (1000) tj        (1000)      370 2023-04-01 21:59:08.000000 pytiva-2023.8.6/pytiva/anesthesia/AnesthesiaCaseStaffingDataSet.py
+-rw-rw-r--   0 tj        (1000) tj        (1000)      882 2023-04-01 22:53:53.000000 pytiva-2023.8.6/pytiva/anesthesia/AnesthesiaDataSet.py
+-rw-rw-r--   0 tj        (1000) tj        (1000)    13373 2023-08-04 18:37:12.000000 pytiva-2023.8.6/pytiva/anesthesia/AnesthesiaStudy.py
+-rw-rw-r--   0 tj        (1000) tj        (1000)     2816 2023-04-30 15:32:20.000000 pytiva-2023.8.6/pytiva/anesthesia/EventActivityDefinition.py
+-rw-rw-r--   0 tj        (1000) tj        (1000)      465 2023-02-14 22:04:16.000000 pytiva-2023.8.6/pytiva/anesthesia/__init__.py
+-rw-rw-r--   0 tj        (1000) tj        (1000)     1571 2023-02-05 18:43:13.000000 pytiva-2023.8.6/pytiva/anesthesia/utils.py
+drwxrwxr-x   0 tj        (1000) tj        (1000)        0 2023-08-07 01:22:24.969655 pytiva-2023.8.6/pytiva/dataset/
+-rw-rw-r--   0 tj        (1000) tj        (1000)     6187 2023-07-19 22:01:01.000000 pytiva-2023.8.6/pytiva/dataset/DataSet.py
+-rw-rw-r--   0 tj        (1000) tj        (1000)      950 2023-04-09 22:37:45.000000 pytiva-2023.8.6/pytiva/dataset/TimeSeriesDataSet.py
+-rw-rw-r--   0 tj        (1000) tj        (1000)       78 2023-04-08 14:19:31.000000 pytiva-2023.8.6/pytiva/dataset/__init__.py
+-rw-rw-r--   0 tj        (1000) tj        (1000)       68 2023-05-05 21:20:58.000000 pytiva-2023.8.6/pytiva/requirements.txt
+drwxrwxr-x   0 tj        (1000) tj        (1000)        0 2023-08-07 01:22:24.977656 pytiva-2023.8.6/pytiva/staffing/
+-rw-rw-r--   0 tj        (1000) tj        (1000)      273 2023-04-08 15:01:52.000000 pytiva-2023.8.6/pytiva/staffing/CapacityTSDS.py
+-rw-rw-r--   0 tj        (1000) tj        (1000)     3042 2022-11-04 18:22:16.000000 pytiva-2023.8.6/pytiva/staffing/ProviderShift.py
+-rw-rw-r--   0 tj        (1000) tj        (1000)     3401 2023-04-09 22:37:51.000000 pytiva-2023.8.6/pytiva/staffing/ResourceAssignmentDataSet.py
+-rw-rw-r--   0 tj        (1000) tj        (1000)      242 2023-04-01 22:25:45.000000 pytiva-2023.8.6/pytiva/staffing/StaffingDataSet.py
+-rw-rw-r--   0 tj        (1000) tj        (1000)      293 2023-04-08 15:02:09.000000 pytiva-2023.8.6/pytiva/staffing/__init__.py
+-rw-rw-r--   0 tj        (1000) tj        (1000)     4987 2023-04-07 21:12:34.000000 pytiva-2023.8.6/pytiva/staffing/utils.py
+drwxrwxr-x   0 tj        (1000) tj        (1000)        0 2023-08-07 01:22:24.977656 pytiva-2023.8.6/pytiva/stats/
+-rw-rw-r--   0 tj        (1000) tj        (1000)       67 2023-08-04 18:38:09.000000 pytiva-2023.8.6/pytiva/stats/__init__.py
+-rw-rw-r--   0 tj        (1000) tj        (1000)     5537 2023-08-06 23:48:41.000000 pytiva-2023.8.6/pytiva/stats/utils.py
+drwxrwxr-x   0 tj        (1000) tj        (1000)        0 2023-08-07 01:22:24.981655 pytiva-2023.8.6/pytiva/utils/
+-rw-rw-r--   0 tj        (1000) tj        (1000)       21 2023-02-01 23:16:37.000000 pytiva-2023.8.6/pytiva/utils/__init__.py
+-rw-rw-r--   0 tj        (1000) tj        (1000)     4094 2023-03-28 16:03:27.000000 pytiva-2023.8.6/pytiva/utils/utils.py
+drwxrwxr-x   0 tj        (1000) tj        (1000)        0 2023-08-07 01:22:24.985656 pytiva-2023.8.6/pytiva/viz/
+-rw-rw-r--   0 tj        (1000) tj        (1000)      143 2023-08-04 21:38:18.000000 pytiva-2023.8.6/pytiva/viz/__init__.py
+-rw-rw-r--   0 tj        (1000) tj        (1000)     2536 2023-04-23 00:26:25.000000 pytiva-2023.8.6/pytiva/viz/gantt.py
+-rw-rw-r--   0 tj        (1000) tj        (1000)     3442 2023-08-04 22:57:46.000000 pytiva-2023.8.6/pytiva/viz/lineplots.py
+drwxrwxr-x   0 tj        (1000) tj        (1000)        0 2023-08-07 01:22:24.949655 pytiva-2023.8.6/pytiva.egg-info/
+-rw-rw-r--   0 tj        (1000) tj        (1000)     2503 2023-08-07 01:22:24.000000 pytiva-2023.8.6/pytiva.egg-info/PKG-INFO
+-rw-rw-r--   0 tj        (1000) tj        (1000)     1497 2023-08-07 01:22:24.000000 pytiva-2023.8.6/pytiva.egg-info/SOURCES.txt
+-rw-rw-r--   0 tj        (1000) tj        (1000)        1 2023-08-07 01:22:24.000000 pytiva-2023.8.6/pytiva.egg-info/dependency_links.txt
+-rw-rw-r--   0 tj        (1000) tj        (1000)       68 2023-08-07 01:22:24.000000 pytiva-2023.8.6/pytiva.egg-info/requires.txt
+-rw-rw-r--   0 tj        (1000) tj        (1000)        7 2023-08-07 01:22:24.000000 pytiva-2023.8.6/pytiva.egg-info/top_level.txt
+-rw-rw-r--   0 tj        (1000) tj        (1000)       38 2023-08-07 01:22:24.997656 pytiva-2023.8.6/setup.cfg
+drwxrwxr-x   0 tj        (1000) tj        (1000)        0 2023-08-07 01:22:24.997656 pytiva-2023.8.6/tests/
+-rw-rw-r--   0 tj        (1000) tj        (1000)     1342 2023-05-03 15:27:47.000000 pytiva-2023.8.6/tests/test_ProviderShift.py
+-rw-rw-r--   0 tj        (1000) tj        (1000)     3293 2023-05-03 15:27:47.000000 pytiva-2023.8.6/tests/test_ResourceAssignmentDataSet.py
+-rw-rw-r--   0 tj        (1000) tj        (1000)      963 2023-05-03 15:27:47.000000 pytiva-2023.8.6/tests/test_activity.py
+-rw-rw-r--   0 tj        (1000) tj        (1000)     1676 2023-05-03 15:27:47.000000 pytiva-2023.8.6/tests/test_activity_unduplication_with_meds.py
+-rw-rw-r--   0 tj        (1000) tj        (1000)      982 2023-05-03 15:27:47.000000 pytiva-2023.8.6/tests/test_anesthesia.py
+-rw-rw-r--   0 tj        (1000) tj        (1000)     1371 2023-05-03 15:27:47.000000 pytiva-2023.8.6/tests/test_anesthesia_case_events_dataset.py
+-rw-rw-r--   0 tj        (1000) tj        (1000)     1849 2023-05-03 15:27:47.000000 pytiva-2023.8.6/tests/test_anesthesia_study.py
+-rw-rw-r--   0 tj        (1000) tj        (1000)     2559 2023-08-07 00:03:42.000000 pytiva-2023.8.6/tests/test_dataset.py
+-rw-rw-r--   0 tj        (1000) tj        (1000)     3532 2023-05-03 15:27:47.000000 pytiva-2023.8.6/tests/test_gantt.py
+-rw-rw-r--   0 tj        (1000) tj        (1000)      192 2023-04-09 20:16:13.000000 pytiva-2023.8.6/tests/test_staffing.py
+-rw-rw-r--   0 tj        (1000) tj        (1000)     1611 2023-08-07 00:06:52.000000 pytiva-2023.8.6/tests/test_stats.py
+-rw-rw-r--   0 tj        (1000) tj        (1000)     2290 2023-08-07 01:06:58.000000 pytiva-2023.8.6/tests/test_viz.py
+-rw-rw-r--   0 tj        (1000) tj        (1000)     4325 2023-08-07 00:54:41.000000 pytiva-2023.8.6/tests/testconfig.py
```

### Comparing `pytiva-2023.5.5/LICENSE` & `pytiva-2023.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pytiva-2023.5.5/pyproject.toml` & `pytiva-2023.8.6/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pytiva"
-version = "2023.5.5"
+version = "2023.8.6"
 authors = [
     { name="TJ Biel", email="tjbiel85@gmail.com" },
 ]
 description = "Python Tools for Investigation and Visualziing Activity within anesthesia records"
 readme = "README.md"
 requires-python = ">=3.10.4"
 classifiers = [
@@ -24,14 +24,15 @@
 [tool.setuptools]
 packages = [
     "pytiva",
     "pytiva.activity",
     "pytiva.anesthesia",
     "pytiva.dataset",
     "pytiva.staffing",
+    "pytiva.stats",
     "pytiva.utils",
     "pytiva.viz"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/tjbiel85/pytiva"
 "Bug Tracker" = "https://github.com/tjbiel85/pytiva/issues"
```

### Comparing `pytiva-2023.5.5/pytiva/activity/ActivityDataSet.py` & `pytiva-2023.8.6/pytiva/activity/ActivityDataSet.py`

 * *Files identical despite different names*

### Comparing `pytiva-2023.5.5/pytiva/activity/utils.py` & `pytiva-2023.8.6/pytiva/activity/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import itertools
 import operator
+
 ORDERED_WEEKLY_DAY_NAME = ['Sunday', 'Monday', 'Tuesday', 'Wednesday', 'Thursday', 'Friday', 'Saturday']
 
 
 def value_between_row_values(
         row,
         value,
         column_left='activity_start',
```

### Comparing `pytiva-2023.5.5/pytiva/anesthesia/AnesthesiaCaseDataSet.py` & `pytiva-2023.8.6/pytiva/anesthesia/AnesthesiaCaseDataSet.py`

 * *Files identical despite different names*

### Comparing `pytiva-2023.5.5/pytiva/anesthesia/AnesthesiaCaseEventsDataSet.py` & `pytiva-2023.8.6/pytiva/anesthesia/AnesthesiaCaseEventsDataSet.py`

 * *Files identical despite different names*

### Comparing `pytiva-2023.5.5/pytiva/anesthesia/AnesthesiaCaseMedicationsDataSet.py` & `pytiva-2023.8.6/pytiva/anesthesia/AnesthesiaCaseMedicationsDataSet.py`

 * *Files identical despite different names*

### Comparing `pytiva-2023.5.5/pytiva/anesthesia/AnesthesiaDataSet.py` & `pytiva-2023.8.6/pytiva/anesthesia/AnesthesiaDataSet.py`

 * *Files identical despite different names*

### Comparing `pytiva-2023.5.5/pytiva/anesthesia/AnesthesiaStudy.py` & `pytiva-2023.8.6/pytiva/anesthesia/AnesthesiaStudy.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,15 +125,16 @@
 
     @property
     def _member_ds_and_counts(self):
         # in which case, unittests will need to be updated to support them
         # (json casts tuples to list, which is how the data are stored for comparison)
         return [[k, len(v._df)] for k, v in self._case_dataset_member_dict.items()]
 
-    def summarize(self, verbose=True, activity_count_freq='M', extra_quantiles=[.90, .95, .98]):
+    def summarize(self, verbose=True, activity_count_freq='M', extra_quantiles=[.90, .95, .98], include_ci=0.95):
+        #TODO: update this to incorporate stats.describe_plus()
         lines = [f"### AnesthesiaStudy object ###"]
 
         # case summary info
         lines.append(f'* Case data *')
 
         start_min, start_max = self._anesthesia_start_range
         lines.append(f"ds_cases['anesthesia_start'] range: {start_min} to {start_max}")
```

### Comparing `pytiva-2023.5.5/pytiva/anesthesia/EventActivityDefinition.py` & `pytiva-2023.8.6/pytiva/anesthesia/EventActivityDefinition.py`

 * *Files identical despite different names*

### Comparing `pytiva-2023.5.5/pytiva/anesthesia/utils.py` & `pytiva-2023.8.6/pytiva/anesthesia/utils.py`

 * *Files identical despite different names*

### Comparing `pytiva-2023.5.5/pytiva/dataset/DataSet.py` & `pytiva-2023.8.6/pytiva/dataset/DataSet.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pandas as pd
+from ..stats import test_group_means as st_test_group_means
 
 
 class DataSet(object):
     """
     A base class for building objects based mostly on pandas.DataFrame
     objects, but with extra functionality one might want to pass forward.
 
@@ -148,7 +149,14 @@
         :param lst_items: allowable items; will be used in DataFrame[col].isin()
         :return: excluded items, in an object of the same type as self
         """
         mask = self._df[col].isin(lst_items)
         excluded = self._df.loc[ ~mask ]
         self._df = self._df.loc[ mask ]
         return type(self)(excluded)
+
+    def test_group_means(self, category_label, data_label, anova_alpha=0.05, hsd_confidence_level=0.95,
+                         *args, **kwargs):
+        df = self._df
+        categories = df[category_label].unique()
+        samples = [df[df[category_label] == s][data_label] for s in categories]
+        return st_test_group_means(samples, categories, anova_alpha, hsd_confidence_level, *args, **kwargs)
```

### Comparing `pytiva-2023.5.5/pytiva/dataset/TimeSeriesDataSet.py` & `pytiva-2023.8.6/pytiva/dataset/TimeSeriesDataSet.py`

 * *Files identical despite different names*

### Comparing `pytiva-2023.5.5/pytiva/staffing/ProviderShift.py` & `pytiva-2023.8.6/pytiva/staffing/ProviderShift.py`

 * *Files identical despite different names*

### Comparing `pytiva-2023.5.5/pytiva/staffing/ResourceAssignmentDataSet.py` & `pytiva-2023.8.6/pytiva/staffing/ResourceAssignmentDataSet.py`

 * *Files identical despite different names*

### Comparing `pytiva-2023.5.5/pytiva/staffing/utils.py` & `pytiva-2023.8.6/pytiva/staffing/utils.py`

 * *Files identical despite different names*

### Comparing `pytiva-2023.5.5/pytiva/utils/utils.py` & `pytiva-2023.8.6/pytiva/utils/utils.py`

 * *Files identical despite different names*

### Comparing `pytiva-2023.5.5/pytiva/viz/gantt.py` & `pytiva-2023.8.6/pytiva/viz/gantt.py`

 * *Files identical despite different names*

### Comparing `pytiva-2023.5.5/pytiva.egg-info/SOURCES.txt` & `pytiva-2023.8.6/pytiva.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -25,22 +25,27 @@
 pytiva/dataset/__init__.py
 pytiva/staffing/CapacityTSDS.py
 pytiva/staffing/ProviderShift.py
 pytiva/staffing/ResourceAssignmentDataSet.py
 pytiva/staffing/StaffingDataSet.py
 pytiva/staffing/__init__.py
 pytiva/staffing/utils.py
+pytiva/stats/__init__.py
+pytiva/stats/utils.py
 pytiva/utils/__init__.py
 pytiva/utils/utils.py
 pytiva/viz/__init__.py
 pytiva/viz/gantt.py
+pytiva/viz/lineplots.py
 tests/test_ProviderShift.py
 tests/test_ResourceAssignmentDataSet.py
 tests/test_activity.py
 tests/test_activity_unduplication_with_meds.py
 tests/test_anesthesia.py
 tests/test_anesthesia_case_events_dataset.py
 tests/test_anesthesia_study.py
 tests/test_dataset.py
 tests/test_gantt.py
 tests/test_staffing.py
+tests/test_stats.py
+tests/test_viz.py
 tests/testconfig.py
```

### Comparing `pytiva-2023.5.5/tests/test_ProviderShift.py` & `pytiva-2023.8.6/tests/test_ProviderShift.py`

 * *Files identical despite different names*

### Comparing `pytiva-2023.5.5/tests/test_ResourceAssignmentDataSet.py` & `pytiva-2023.8.6/tests/test_ResourceAssignmentDataSet.py`

 * *Files identical despite different names*

### Comparing `pytiva-2023.5.5/tests/test_activity.py` & `pytiva-2023.8.6/tests/test_activity.py`

 * *Files identical despite different names*

### Comparing `pytiva-2023.5.5/tests/test_activity_unduplication_with_meds.py` & `pytiva-2023.8.6/tests/test_activity_unduplication_with_meds.py`

 * *Files identical despite different names*

### Comparing `pytiva-2023.5.5/tests/test_anesthesia.py` & `pytiva-2023.8.6/tests/test_anesthesia.py`

 * *Files identical despite different names*

### Comparing `pytiva-2023.5.5/tests/test_anesthesia_case_events_dataset.py` & `pytiva-2023.8.6/tests/test_anesthesia_case_events_dataset.py`

 * *Files identical despite different names*

### Comparing `pytiva-2023.5.5/tests/test_anesthesia_study.py` & `pytiva-2023.8.6/tests/test_anesthesia_study.py`

 * *Files identical despite different names*

### Comparing `pytiva-2023.5.5/tests/test_dataset.py` & `pytiva-2023.8.6/tests/test_dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 # local test config
 import testconfig
 
 
 class TestDataSet(unittest.TestCase):
     def setUp(self):
         self.df_ref = pd.read_csv(
-            os.path.join(testconfig.WD, testconfig.TESTDATA['DS_ACTIVITY'])# ACTIVITY_TEST_DATA_FILENAME),
-            #parse_dates=['activity_start', 'activity_end']
+            os.path.join(testconfig.WD, testconfig.TESTDATA['DS_ACTIVITY']),
+            parse_dates=['activity_start', 'activity_end']
         )
 
     def test_none_data_throws_exception(self):
         # None is usually allowed by pandas.DataFrame
         # but not for a DataSet
         with self.assertRaises(Exception):
             ds = DataSet(None)
```

### Comparing `pytiva-2023.5.5/tests/test_gantt.py` & `pytiva-2023.8.6/tests/test_gantt.py`

 * *Files identical despite different names*

### Comparing `pytiva-2023.5.5/tests/testconfig.py` & `pytiva-2023.8.6/tests/testconfig.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,19 @@
     'ONE_CASE_GANTT': 'testdata-expected_one_case_gantt.csv',
     'ONE_CASE_GANTT_PNG': 'comparison_gantt_one_case.png',
     #'ONE_CASE_GANTT_PNG_SAMPLE_SHA512_HEXDIGEST': '9e0c9a152bd912ce6b1bc6d0e0f1f1ed075d6e99dda4268d70a7496c380bd0dd89378f645f943ade972d1615152b7ccf1189d3b8953ac83290291e7c7b1e2144',
     'DS_STAFFING_ACTIVITY': 'testdata-ds_staffing_activity.csv',
     'DS_RESOURCES_LIMITED_BY_PS_DICT': 'testdata-ds_resources_limited_by_ps_dict.csv',
     'DS_RESOURCES_LIMITED_BY_DATE_LIST': 'testdata-ds_resources_limited_by_date_list.csv',
     'DS_RESOURCES_LIMITED_BY_DATE_LIST_AND_PS_DICT': 'testdata-ds_resources_limited_by_date_list_and_ps_dict.csv',
-    'ADS_GENERATE_RESOURCE_ACTIVITY_W_PS_DICT': 'testdata-ads_generate_resource_activity_w_ps_dict.csv'
+    'ADS_GENERATE_RESOURCE_ACTIVITY_W_PS_DICT': 'testdata-ads_generate_resource_activity_w_ps_dict.csv',
+    'EXPECTED_TUKEY_HSD_DF': 'testdata-expected_tukey_hsd_df.csv',
+    'EXPECTED_ANOVA_DICT': {'f_statistic': 5352.653462676786, 'p_value': 0.0, 'alpha': 0.05, 'reject_h0': True},
+    'DF_MEAN_RATE_BY_CATEGORY': 'testdata-df_mean_rate_by_category.csv',
+    'DF_MEAN_RATE_BY_CATEGORY_WITH_CI': 'testdata-df_mean_rate_by_category_with_ci.csv'
 }
 
 TESTDATA_CSV_DICT_FOR_DATASETS = {
     'ds_cases': {'FILEPATH': os.path.join(WD, TESTDATA['DS_CASES'])},
     'ds_case_meds': {'FILEPATH': os.path.join(WD, TESTDATA['DS_CASE_MEDS'])},
     'ds_case_events': {'FILEPATH': os.path.join(WD, TESTDATA['DS_CASE_EVENTS'])}
 }
```

