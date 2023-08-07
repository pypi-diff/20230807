# Comparing `tmp/streamlit-highcharts-0.1.5.tar.gz` & `tmp/streamlit-highcharts-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-highcharts-0.1.5.tar", last modified: Wed Oct 26 13:52:05 2022, max compression
+gzip compressed data, was "streamlit-highcharts-0.1.6.tar", last modified: Mon Aug  7 09:32:07 2023, max compression
```

## Comparing `streamlit-highcharts-0.1.5.tar` & `streamlit-highcharts-0.1.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 13:52:05.957112 streamlit-highcharts-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (121)     1075 2022-10-26 13:51:46.000000 streamlit-highcharts-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-10-26 13:51:46.000000 streamlit-highcharts-0.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1977 2022-10-26 13:52:05.953112 streamlit-highcharts-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1720 2022-10-26 13:51:46.000000 streamlit-highcharts-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-26 13:52:05.957112 streamlit-highcharts-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      652 2022-10-26 13:51:46.000000 streamlit-highcharts-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 13:52:05.953112 streamlit-highcharts-0.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 13:52:05.953112 streamlit-highcharts-0.1.5/src/streamlit_highcharts/
--rw-r--r--   0 runner    (1001) docker     (121)    60843 2022-10-26 13:51:46.000000 streamlit-highcharts-0.1.5/src/streamlit_highcharts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 13:52:05.953112 streamlit-highcharts-0.1.5/src/streamlit_highcharts/frontend/
--rw-r--r--   0 runner    (1001) docker     (121)     1655 2022-10-26 13:51:46.000000 streamlit-highcharts-0.1.5/src/streamlit_highcharts/frontend/index.html
--rw-r--r--   0 runner    (1001) docker     (121)      451 2022-10-26 13:51:46.000000 streamlit-highcharts-0.1.5/src/streamlit_highcharts/frontend/main.js
--rw-r--r--   0 runner    (1001) docker     (121)     1121 2022-10-26 13:51:46.000000 streamlit-highcharts-0.1.5/src/streamlit_highcharts/frontend/streamlit-component-lib.js
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-26 13:51:46.000000 streamlit-highcharts-0.1.5/src/streamlit_highcharts/frontend/style.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 13:52:05.953112 streamlit-highcharts-0.1.5/src/streamlit_highcharts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1977 2022-10-26 13:52:05.000000 streamlit-highcharts-0.1.5/src/streamlit_highcharts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      506 2022-10-26 13:52:05.000000 streamlit-highcharts-0.1.5/src/streamlit_highcharts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-26 13:52:05.000000 streamlit-highcharts-0.1.5/src/streamlit_highcharts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-10-26 13:52:05.000000 streamlit-highcharts-0.1.5/src/streamlit_highcharts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-10-26 13:52:05.000000 streamlit-highcharts-0.1.5/src/streamlit_highcharts.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:32:07.676696 streamlit-highcharts-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-08-07 09:31:58.000000 streamlit-highcharts-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-08-07 09:31:58.000000 streamlit-highcharts-0.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-08-07 09:32:07.676696 streamlit-highcharts-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-08-07 09:31:58.000000 streamlit-highcharts-0.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 09:32:07.676696 streamlit-highcharts-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-08-07 09:31:58.000000 streamlit-highcharts-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:32:07.668696 streamlit-highcharts-0.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:32:07.672696 streamlit-highcharts-0.1.6/src/streamlit_highcharts/
+-rw-r--r--   0 runner    (1001) docker     (123)    60843 2023-08-07 09:31:58.000000 streamlit-highcharts-0.1.6/src/streamlit_highcharts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:32:07.676696 streamlit-highcharts-0.1.6/src/streamlit_highcharts/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-08-07 09:31:58.000000 streamlit-highcharts-0.1.6/src/streamlit_highcharts/frontend/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-08-07 09:31:58.000000 streamlit-highcharts-0.1.6/src/streamlit_highcharts/frontend/main.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-08-07 09:31:58.000000 streamlit-highcharts-0.1.6/src/streamlit_highcharts/frontend/streamlit-component-lib.js
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-07 09:31:58.000000 streamlit-highcharts-0.1.6/src/streamlit_highcharts/frontend/style.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:32:07.672696 streamlit-highcharts-0.1.6/src/streamlit_highcharts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-08-07 09:32:07.000000 streamlit-highcharts-0.1.6/src/streamlit_highcharts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-08-07 09:32:07.000000 streamlit-highcharts-0.1.6/src/streamlit_highcharts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 09:32:07.000000 streamlit-highcharts-0.1.6/src/streamlit_highcharts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-07 09:32:07.000000 streamlit-highcharts-0.1.6/src/streamlit_highcharts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-07 09:32:07.000000 streamlit-highcharts-0.1.6/src/streamlit_highcharts.egg-info/top_level.txt
```

### Comparing `streamlit-highcharts-0.1.5/LICENSE` & `streamlit-highcharts-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-highcharts-0.1.5/PKG-INFO` & `streamlit-highcharts-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-highcharts
-Version: 0.1.5
+Version: 0.1.6
 Summary: Simple wrapper for Highcharts JS libs
 Author: Anthony Alteirac
 Author-email: anthony@alteirac.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `streamlit-highcharts-0.1.5/README.md` & `streamlit-highcharts-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `streamlit-highcharts-0.1.5/setup.py` & `streamlit-highcharts-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="streamlit-highcharts",
-    version="0.1.5",
+    version="0.1.6",
     author="Anthony Alteirac",
     author_email="anthony@alteirac.com",
     description="Simple wrapper for Highcharts JS libs",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(where="src"),
     package_dir={"": "src"},
```

### Comparing `streamlit-highcharts-0.1.5/src/streamlit_highcharts/__init__.py` & `streamlit-highcharts-0.1.6/src/streamlit_highcharts/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-highcharts-0.1.5/src/streamlit_highcharts/frontend/index.html` & `streamlit-highcharts-0.1.6/src/streamlit_highcharts/frontend/index.html`

 * *Files identical despite different names*

### Comparing `streamlit-highcharts-0.1.5/src/streamlit_highcharts/frontend/streamlit-component-lib.js` & `streamlit-highcharts-0.1.6/src/streamlit_highcharts/frontend/streamlit-component-lib.js`

 * *Files identical despite different names*

### Comparing `streamlit-highcharts-0.1.5/src/streamlit_highcharts.egg-info/PKG-INFO` & `streamlit-highcharts-0.1.6/src/streamlit_highcharts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-highcharts
-Version: 0.1.5
+Version: 0.1.6
 Summary: Simple wrapper for Highcharts JS libs
 Author: Anthony Alteirac
 Author-email: anthony@alteirac.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

