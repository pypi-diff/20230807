# Comparing `tmp/filter-data-options-0.0.1.tar.gz` & `tmp/filter-data-options-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filter-data-options-0.0.1.tar", last modified: Mon Aug  7 02:55:11 2023, max compression
+gzip compressed data, was "filter-data-options-0.0.2.tar", last modified: Mon Aug  7 03:09:46 2023, max compression
```

## Comparing `filter-data-options-0.0.1.tar` & `filter-data-options-0.0.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-08-07 02:55:11.350799 filter-data-options-0.0.1/
--rw-rw-rw-   0        0        0     1082 2023-08-06 12:03:52.000000 filter-data-options-0.0.1/LICENSE
--rw-rw-rw-   0        0        0       56 2023-08-07 02:52:32.000000 filter-data-options-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      600 2023-08-07 02:55:11.347796 filter-data-options-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      314 2023-08-06 12:03:52.000000 filter-data-options-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-08-07 02:55:10.713807 filter-data-options-0.0.1/filter_data_options/
--rw-rw-rw-   0        0        0     2537 2023-08-07 02:51:08.000000 filter-data-options-0.0.1/filter_data_options/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-07 02:55:10.639792 filter-data-options-0.0.1/filter_data_options/frontend/
-drwxrwxrwx   0        0        0        0 2023-08-07 02:55:10.938791 filter-data-options-0.0.1/filter_data_options/frontend/build/
--rw-rw-rw-   0        0        0      374 2023-08-07 02:50:34.000000 filter-data-options-0.0.1/filter_data_options/frontend/build/asset-manifest.json
--rw-rw-rw-   0        0        0   206960 2023-08-06 12:03:52.000000 filter-data-options-0.0.1/filter_data_options/frontend/build/bootstrap.min.css
--rw-rw-rw-   0        0        0      553 2023-08-07 02:50:34.000000 filter-data-options-0.0.1/filter_data_options/frontend/build/index.html
-drwxrwxrwx   0        0        0        0 2023-08-07 02:55:10.644791 filter-data-options-0.0.1/filter_data_options/frontend/build/static/
-drwxrwxrwx   0        0        0        0 2023-08-07 02:55:11.023808 filter-data-options-0.0.1/filter_data_options/frontend/build/static/css/
--rw-rw-rw-   0        0        0     1726 2023-08-07 02:50:34.000000 filter-data-options-0.0.1/filter_data_options/frontend/build/static/css/main.b628d786.css
--rw-rw-rw-   0        0        0     3692 2023-08-07 02:50:34.000000 filter-data-options-0.0.1/filter_data_options/frontend/build/static/css/main.b628d786.css.map
-drwxrwxrwx   0        0        0        0 2023-08-07 02:55:11.325794 filter-data-options-0.0.1/filter_data_options/frontend/build/static/js/
--rw-rw-rw-   0        0        0   478358 2023-08-07 02:50:34.000000 filter-data-options-0.0.1/filter_data_options/frontend/build/static/js/main.4958325e.js
--rw-rw-rw-   0        0        0     1609 2023-08-07 02:50:34.000000 filter-data-options-0.0.1/filter_data_options/frontend/build/static/js/main.4958325e.js.LICENSE.txt
--rw-rw-rw-   0        0        0  1834993 2023-08-07 02:50:34.000000 filter-data-options-0.0.1/filter_data_options/frontend/build/static/js/main.4958325e.js.map
-drwxrwxrwx   0        0        0        0 2023-08-07 02:55:10.826794 filter-data-options-0.0.1/filter_data_options.egg-info/
--rw-rw-rw-   0        0        0      600 2023-08-07 02:55:09.000000 filter-data-options-0.0.1/filter_data_options.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      772 2023-08-07 02:55:10.000000 filter-data-options-0.0.1/filter_data_options.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-07 02:55:09.000000 filter-data-options-0.0.1/filter_data_options.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-08-07 02:55:09.000000 filter-data-options-0.0.1/filter_data_options.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-08-07 02:55:10.000000 filter-data-options-0.0.1/filter_data_options.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-07 02:55:11.351795 filter-data-options-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      814 2023-08-07 02:38:21.000000 filter-data-options-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 03:09:46.952149 filter-data-options-0.0.2/
+-rw-rw-rw-   0        0        0     1082 2023-08-06 12:03:52.000000 filter-data-options-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0       56 2023-08-07 02:52:32.000000 filter-data-options-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      958 2023-08-07 03:09:46.948158 filter-data-options-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      672 2023-08-07 03:08:47.000000 filter-data-options-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-08-07 03:09:46.751141 filter-data-options-0.0.2/filter_data_options/
+-rw-rw-rw-   0        0        0     2537 2023-08-07 02:51:08.000000 filter-data-options-0.0.2/filter_data_options/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-07 03:09:46.688146 filter-data-options-0.0.2/filter_data_options/frontend/
+drwxrwxrwx   0        0        0        0 2023-08-07 03:09:46.856142 filter-data-options-0.0.2/filter_data_options/frontend/build/
+-rw-rw-rw-   0        0        0      374 2023-08-07 02:50:34.000000 filter-data-options-0.0.2/filter_data_options/frontend/build/asset-manifest.json
+-rw-rw-rw-   0        0        0   206960 2023-08-06 12:03:52.000000 filter-data-options-0.0.2/filter_data_options/frontend/build/bootstrap.min.css
+-rw-rw-rw-   0        0        0      553 2023-08-07 02:50:34.000000 filter-data-options-0.0.2/filter_data_options/frontend/build/index.html
+drwxrwxrwx   0        0        0        0 2023-08-07 03:09:46.708146 filter-data-options-0.0.2/filter_data_options/frontend/build/static/
+drwxrwxrwx   0        0        0        0 2023-08-07 03:09:46.877143 filter-data-options-0.0.2/filter_data_options/frontend/build/static/css/
+-rw-rw-rw-   0        0        0     1726 2023-08-07 02:50:34.000000 filter-data-options-0.0.2/filter_data_options/frontend/build/static/css/main.b628d786.css
+-rw-rw-rw-   0        0        0     3692 2023-08-07 02:50:34.000000 filter-data-options-0.0.2/filter_data_options/frontend/build/static/css/main.b628d786.css.map
+drwxrwxrwx   0        0        0        0 2023-08-07 03:09:46.922149 filter-data-options-0.0.2/filter_data_options/frontend/build/static/js/
+-rw-rw-rw-   0        0        0   478358 2023-08-07 02:50:34.000000 filter-data-options-0.0.2/filter_data_options/frontend/build/static/js/main.4958325e.js
+-rw-rw-rw-   0        0        0     1609 2023-08-07 02:50:34.000000 filter-data-options-0.0.2/filter_data_options/frontend/build/static/js/main.4958325e.js.LICENSE.txt
+-rw-rw-rw-   0        0        0  1834993 2023-08-07 02:50:34.000000 filter-data-options-0.0.2/filter_data_options/frontend/build/static/js/main.4958325e.js.map
+drwxrwxrwx   0        0        0        0 2023-08-07 03:09:46.827146 filter-data-options-0.0.2/filter_data_options.egg-info/
+-rw-rw-rw-   0        0        0      958 2023-08-07 03:09:45.000000 filter-data-options-0.0.2/filter_data_options.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      772 2023-08-07 03:09:46.000000 filter-data-options-0.0.2/filter_data_options.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 03:09:45.000000 filter-data-options-0.0.2/filter_data_options.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-08-07 03:09:45.000000 filter-data-options-0.0.2/filter_data_options.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-08-07 03:09:45.000000 filter-data-options-0.0.2/filter_data_options.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-07 03:09:46.953145 filter-data-options-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      814 2023-08-07 03:08:38.000000 filter-data-options-0.0.2/setup.py
```

### Comparing `filter-data-options-0.0.1/LICENSE` & `filter-data-options-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `filter-data-options-0.0.1/filter_data_options/__init__.py` & `filter-data-options-0.0.2/filter_data_options/__init__.py`

 * *Files identical despite different names*

### Comparing `filter-data-options-0.0.1/filter_data_options/frontend/build/bootstrap.min.css` & `filter-data-options-0.0.2/filter_data_options/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `filter-data-options-0.0.1/filter_data_options/frontend/build/index.html` & `filter-data-options-0.0.2/filter_data_options/frontend/build/index.html`

 * *Files identical despite different names*

### Comparing `filter-data-options-0.0.1/filter_data_options/frontend/build/static/css/main.b628d786.css` & `filter-data-options-0.0.2/filter_data_options/frontend/build/static/css/main.b628d786.css`

 * *Files identical despite different names*

### Comparing `filter-data-options-0.0.1/filter_data_options/frontend/build/static/css/main.b628d786.css.map` & `filter-data-options-0.0.2/filter_data_options/frontend/build/static/css/main.b628d786.css.map`

 * *Files identical despite different names*

### Comparing `filter-data-options-0.0.1/filter_data_options/frontend/build/static/js/main.4958325e.js` & `filter-data-options-0.0.2/filter_data_options/frontend/build/static/js/main.4958325e.js`

 * *Files identical despite different names*

### Comparing `filter-data-options-0.0.1/filter_data_options/frontend/build/static/js/main.4958325e.js.LICENSE.txt` & `filter-data-options-0.0.2/filter_data_options/frontend/build/static/js/main.4958325e.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `filter-data-options-0.0.1/filter_data_options/frontend/build/static/js/main.4958325e.js.map` & `filter-data-options-0.0.2/filter_data_options/frontend/build/static/js/main.4958325e.js.map`

 * *Files identical despite different names*

### Comparing `filter-data-options-0.0.1/filter_data_options.egg-info/SOURCES.txt` & `filter-data-options-0.0.2/filter_data_options.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `filter-data-options-0.0.1/setup.py` & `filter-data-options-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="filter-data-options",
-    version="0.0.1",
+    version="0.0.2",
     author="",
     author_email="",
     description="Streamlit component that allows you to display or not particular data selected",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

