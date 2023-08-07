# Comparing `tmp/precursorupdater-0.1.3.tar.gz` & `tmp/precursorupdater-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "precursorupdater-0.1.3.tar", last modified: Thu Mar  9 15:31:48 2023, max compression
+gzip compressed data, was "precursorupdater-0.1.4.tar", last modified: Mon Aug  7 16:22:07 2023, max compression
```

## Comparing `precursorupdater-0.1.3.tar` & `precursorupdater-0.1.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 bunnie    (1000) bunnie    (1000)        0 2023-03-09 15:31:48.128944 precursorupdater-0.1.3/
--rw-r--r--   0 bunnie    (1000) bunnie    (1000)    11358 2022-10-14 08:49:25.000000 precursorupdater-0.1.3/LICENSE
--rw-r--r--   0 bunnie    (1000) bunnie    (1000)     2268 2023-03-09 15:31:48.127943 precursorupdater-0.1.3/PKG-INFO
--rw-r--r--   0 bunnie    (1000) bunnie    (1000)     1228 2023-03-08 20:07:15.000000 precursorupdater-0.1.3/README.md
-drwxr-xr-x   0 bunnie    (1000) bunnie    (1000)        0 2023-03-09 15:31:48.112944 precursorupdater-0.1.3/precursorupdater/
--rw-r--r--   0 bunnie    (1000) bunnie    (1000)       35 2022-10-14 08:49:25.000000 precursorupdater-0.1.3/precursorupdater/__init__.py
--rw-r--r--   0 bunnie    (1000) bunnie    (1000)       49 2022-10-14 08:49:25.000000 precursorupdater-0.1.3/precursorupdater/__main__.py
--rwxr-xr-x   0 bunnie    (1000) bunnie    (1000)    45556 2023-03-09 14:46:12.000000 precursorupdater-0.1.3/precursorupdater/precursorupdater.py
-drwxr-xr-x   0 bunnie    (1000) bunnie    (1000)        0 2023-03-09 15:31:48.124945 precursorupdater-0.1.3/precursorupdater/precursorusb/
--rw-r--r--   0 bunnie    (1000) bunnie    (1000)       39 2022-10-14 08:49:25.000000 precursorupdater-0.1.3/precursorupdater/precursorusb/__init__.py
--rw-r--r--   0 bunnie    (1000) bunnie    (1000)    16063 2023-03-09 14:48:35.000000 precursorupdater-0.1.3/precursorupdater/precursorusb/precursorusb.py
-drwxr-xr-x   0 bunnie    (1000) bunnie    (1000)        0 2023-03-09 15:31:48.120945 precursorupdater-0.1.3/precursorupdater.egg-info/
--rw-r--r--   0 bunnie    (1000) bunnie    (1000)     2268 2023-03-09 15:31:47.000000 precursorupdater-0.1.3/precursorupdater.egg-info/PKG-INFO
--rw-r--r--   0 bunnie    (1000) bunnie    (1000)      451 2023-03-09 15:31:48.000000 precursorupdater-0.1.3/precursorupdater.egg-info/SOURCES.txt
--rw-r--r--   0 bunnie    (1000) bunnie    (1000)        1 2023-03-09 15:31:47.000000 precursorupdater-0.1.3/precursorupdater.egg-info/dependency_links.txt
--rw-r--r--   0 bunnie    (1000) bunnie    (1000)       78 2023-03-09 15:31:47.000000 precursorupdater-0.1.3/precursorupdater.egg-info/entry_points.txt
--rw-r--r--   0 bunnie    (1000) bunnie    (1000)       53 2023-03-09 15:31:47.000000 precursorupdater-0.1.3/precursorupdater.egg-info/requires.txt
--rw-r--r--   0 bunnie    (1000) bunnie    (1000)       17 2023-03-09 15:31:47.000000 precursorupdater-0.1.3/precursorupdater.egg-info/top_level.txt
--rw-r--r--   0 bunnie    (1000) bunnie    (1000)       38 2023-03-09 15:31:48.128944 precursorupdater-0.1.3/setup.cfg
--rw-r--r--   0 bunnie    (1000) bunnie    (1000)     1396 2023-03-09 15:31:33.000000 precursorupdater-0.1.3/setup.py
+drwxr-xr-x   0 bunnie    (1000) bunnie    (1000)        0 2023-08-07 16:22:07.003176 precursorupdater-0.1.4/
+-rw-r--r--   0 bunnie    (1000) bunnie    (1000)    11358 2022-10-14 08:49:25.000000 precursorupdater-0.1.4/LICENSE
+-rw-r--r--   0 bunnie    (1000) bunnie    (1000)     2268 2023-08-07 16:22:07.002177 precursorupdater-0.1.4/PKG-INFO
+-rw-r--r--   0 bunnie    (1000) bunnie    (1000)     1228 2023-03-20 19:01:38.000000 precursorupdater-0.1.4/README.md
+drwxr-xr-x   0 bunnie    (1000) bunnie    (1000)        0 2023-08-07 16:22:06.982171 precursorupdater-0.1.4/precursorupdater/
+-rw-r--r--   0 bunnie    (1000) bunnie    (1000)       35 2022-10-14 08:49:25.000000 precursorupdater-0.1.4/precursorupdater/__init__.py
+-rw-r--r--   0 bunnie    (1000) bunnie    (1000)       49 2022-10-14 08:49:25.000000 precursorupdater-0.1.4/precursorupdater/__main__.py
+-rwxr-xr-x   0 bunnie    (1000) bunnie    (1000)    45639 2023-08-07 16:15:20.000000 precursorupdater-0.1.4/precursorupdater/precursorupdater.py
+drwxr-xr-x   0 bunnie    (1000) bunnie    (1000)        0 2023-08-07 16:22:06.995170 precursorupdater-0.1.4/precursorupdater/precursorusb/
+-rw-r--r--   0 bunnie    (1000) bunnie    (1000)       39 2022-10-14 08:49:25.000000 precursorupdater-0.1.4/precursorupdater/precursorusb/__init__.py
+-rw-r--r--   0 bunnie    (1000) bunnie    (1000)    16063 2023-03-20 19:01:38.000000 precursorupdater-0.1.4/precursorupdater/precursorusb/precursorusb.py
+drwxr-xr-x   0 bunnie    (1000) bunnie    (1000)        0 2023-08-07 16:22:06.993170 precursorupdater-0.1.4/precursorupdater.egg-info/
+-rw-r--r--   0 bunnie    (1000) bunnie    (1000)     2268 2023-08-07 16:22:06.000000 precursorupdater-0.1.4/precursorupdater.egg-info/PKG-INFO
+-rw-r--r--   0 bunnie    (1000) bunnie    (1000)      451 2023-08-07 16:22:06.000000 precursorupdater-0.1.4/precursorupdater.egg-info/SOURCES.txt
+-rw-r--r--   0 bunnie    (1000) bunnie    (1000)        1 2023-08-07 16:22:06.000000 precursorupdater-0.1.4/precursorupdater.egg-info/dependency_links.txt
+-rw-r--r--   0 bunnie    (1000) bunnie    (1000)       78 2023-08-07 16:22:06.000000 precursorupdater-0.1.4/precursorupdater.egg-info/entry_points.txt
+-rw-r--r--   0 bunnie    (1000) bunnie    (1000)       53 2023-08-07 16:22:06.000000 precursorupdater-0.1.4/precursorupdater.egg-info/requires.txt
+-rw-r--r--   0 bunnie    (1000) bunnie    (1000)       17 2023-08-07 16:22:06.000000 precursorupdater-0.1.4/precursorupdater.egg-info/top_level.txt
+-rw-r--r--   0 bunnie    (1000) bunnie    (1000)       38 2023-08-07 16:22:07.003176 precursorupdater-0.1.4/setup.cfg
+-rw-r--r--   0 bunnie    (1000) bunnie    (1000)     1396 2023-08-07 16:21:56.000000 precursorupdater-0.1.4/setup.py
```

### Comparing `precursorupdater-0.1.3/LICENSE` & `precursorupdater-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `precursorupdater-0.1.3/PKG-INFO` & `precursorupdater-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: precursorupdater
-Version: 0.1.3
+Version: 0.1.4
 Summary: Precursor USB Updater
 Home-page: https://github.com/betrusted-io/betrusted-wiki/wiki/Updating-Your-Device
 Author: bunnie
 License: Apache2.0
 Project-URL: Bug Tracker, https://github.com/betrusted-io/xous-core/issues
 Project-URL: Documentation, https://github.com/betrusted-io/betrusted-wiki/wiki/Updating-Your-Device
 Project-URL: Source Code, https://github.com/betrusted-io/xous-core/tree/main/tools/updater
```

### Comparing `precursorupdater-0.1.3/README.md` & `precursorupdater-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `precursorupdater-0.1.3/precursorupdater/precursorupdater.py` & `precursorupdater-0.1.4/precursorupdater/precursorupdater.py`

 * *Files 0% similar despite different names*

```diff
@@ -658,14 +658,18 @@
     # initial check to see if the Precursor device is there
     try:
         (locs, pc_usb) = get_usb_interface(args.config, args.peek, args.override_csr, args.force)
     except ValueError:
         print("Precursor device not found. Please check the USB cable and ensure that `usb debug` was run in Shellchat")
         exit(1)
 
+    if args.config:
+        print("--config selected, quitting.")
+        exit(0)
+
     # now try to download all the artifacts and check their versions
     # this list should visit kernels in order from newest to oldest.
     URL_STABLE = 'https://ci.betrusted.io/releases/latest/'
     URL_BLEEDING = 'https://ci.betrusted.io/latest-ci/'
     print("Phase 1: Download the update")
     if args.bleeding_edge:
         print("Bleeding edge CI build selected")
```

### Comparing `precursorupdater-0.1.3/precursorupdater/precursorusb/precursorusb.py` & `precursorupdater-0.1.4/precursorupdater/precursorusb/precursorusb.py`

 * *Files identical despite different names*

### Comparing `precursorupdater-0.1.3/precursorupdater.egg-info/PKG-INFO` & `precursorupdater-0.1.4/precursorupdater.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: precursorupdater
-Version: 0.1.3
+Version: 0.1.4
 Summary: Precursor USB Updater
 Home-page: https://github.com/betrusted-io/betrusted-wiki/wiki/Updating-Your-Device
 Author: bunnie
 License: Apache2.0
 Project-URL: Bug Tracker, https://github.com/betrusted-io/xous-core/issues
 Project-URL: Documentation, https://github.com/betrusted-io/betrusted-wiki/wiki/Updating-Your-Device
 Project-URL: Source Code, https://github.com/betrusted-io/xous-core/tree/main/tools/updater
```

### Comparing `precursorupdater-0.1.3/setup.py` & `precursorupdater-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from setuptools import setup, find_packages
 with open('README.md') as f:
     long_description = f.read()
 
 setup(
     name="precursorupdater",
-    version="0.1.3",
+    version="0.1.4",
     author="bunnie",
     description="Precursor USB Updater",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/betrusted-io/betrusted-wiki/wiki/Updating-Your-Device",
     project_urls={
         "Bug Tracker": "https://github.com/betrusted-io/xous-core/issues",
```

