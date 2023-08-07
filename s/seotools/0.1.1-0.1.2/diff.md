# Comparing `tmp/seotools-0.1.1.tar.gz` & `tmp/seotools-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seotools-0.1.1.tar", last modified: Sat Aug  5 12:32:04 2023, max compression
+gzip compressed data, was "seotools-0.1.2.tar", last modified: Mon Aug  7 10:25:18 2023, max compression
```

## Comparing `seotools-0.1.1.tar` & `seotools-0.1.2.tar`

### file list

```diff
@@ -1,36 +1,38 @@
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-05 12:32:04.063716 seotools-0.1.1/
--rw-r--r--   0 james      (501) staff       (20)     3078 2023-08-03 19:33:11.000000 seotools-0.1.1/.gitignore
--rw-r--r--   0 james      (501) staff       (20)     1063 2023-08-03 19:09:09.000000 seotools-0.1.1/LICENSE
--rw-r--r--   0 james      (501) staff       (20)      865 2023-08-03 09:42:54.000000 seotools-0.1.1/Makefile
--rw-r--r--   0 james      (501) staff       (20)     3538 2023-08-05 12:32:04.063476 seotools-0.1.1/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)     3049 2023-08-05 09:35:07.000000 seotools-0.1.1/README.md
--rw-r--r--   0 james      (501) staff       (20)      638 2023-08-04 22:27:54.000000 seotools-0.1.1/api.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-05 12:32:04.058685 seotools-0.1.1/docs/
--rw-r--r--   0 james      (501) staff       (20)      159 2023-08-05 11:23:46.000000 seotools-0.1.1/docs/broken_links.md
--rw-r--r--   0 james      (501) staff       (20)        0 2023-08-03 22:02:00.000000 seotools-0.1.1/docs/changelog.md
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-05 12:32:04.059119 seotools-0.1.1/docs/helpers/
--rw-r--r--   0 james      (501) staff       (20)      392 2023-08-03 22:38:18.000000 seotools-0.1.1/docs/helpers/validate_googlebot_ips.md
--rw-r--r--   0 james      (501) staff       (20)     2591 2023-08-03 22:41:36.000000 seotools-0.1.1/docs/index.md
--rw-r--r--   0 james      (501) staff       (20)      565 2023-08-03 22:21:17.000000 seotools-0.1.1/docs/jsonld.md
--rw-r--r--   0 james      (501) staff       (20)     1049 2023-08-03 22:17:37.000000 seotools-0.1.1/docs/recommendation.md
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-05 12:32:04.059451 seotools-0.1.1/docs/reference/
--rw-r--r--   0 james      (501) staff       (20)      124 2023-08-03 22:11:54.000000 seotools-0.1.1/docs/reference/analyzer.md
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-05 12:32:04.059845 seotools-0.1.1/docs/styles/
--rw-r--r--   0 james      (501) staff       (20)       95 2023-08-03 22:03:25.000000 seotools-0.1.1/docs/styles/styles.css
--rw-r--r--   0 james      (501) staff       (20)     1050 2023-08-05 11:19:08.000000 seotools-0.1.1/mkdocs.yml
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-05 12:32:04.061292 seotools-0.1.1/seotools/
--rw-r--r--   0 james      (501) staff       (20)       22 2023-08-05 12:31:30.000000 seotools-0.1.1/seotools/__init__.py
--rw-r--r--   0 james      (501) staff       (20)    16489 2023-08-05 12:31:12.000000 seotools-0.1.1/seotools/app.py
--rw-r--r--   0 james      (501) staff       (20)      479 2023-08-05 12:31:10.000000 seotools-0.1.1/seotools/crawl_bot_validation.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-05 12:32:04.062992 seotools-0.1.1/seotools/links/
--rw-r--r--   0 james      (501) staff       (20)        0 2023-08-05 11:24:44.000000 seotools-0.1.1/seotools/links/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     1396 2023-08-05 11:24:02.000000 seotools-0.1.1/seotools/links/broken.py
--rw-r--r--   0 james      (501) staff       (20)     1162 2023-08-05 11:21:39.000000 seotools-0.1.1/seotools/topics.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-05 12:32:04.062627 seotools-0.1.1/seotools.egg-info/
--rw-r--r--   0 james      (501) staff       (20)     3538 2023-08-05 12:32:04.000000 seotools-0.1.1/seotools.egg-info/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)      544 2023-08-05 12:32:04.000000 seotools-0.1.1/seotools.egg-info/SOURCES.txt
--rw-r--r--   0 james      (501) staff       (20)        1 2023-08-05 12:32:04.000000 seotools-0.1.1/seotools.egg-info/dependency_links.txt
--rw-r--r--   0 james      (501) staff       (20)      141 2023-08-05 12:32:04.000000 seotools-0.1.1/seotools.egg-info/requires.txt
--rw-r--r--   0 james      (501) staff       (20)        9 2023-08-05 12:32:04.000000 seotools-0.1.1/seotools.egg-info/top_level.txt
--rw-r--r--   0 james      (501) staff       (20)       38 2023-08-05 12:32:04.063783 seotools-0.1.1/setup.cfg
--rw-r--r--   0 james      (501) staff       (20)     1247 2023-08-05 10:41:21.000000 seotools-0.1.1/setup.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-07 10:25:18.599868 seotools-0.1.2/
+-rw-r--r--   0 james      (501) staff       (20)     3078 2023-08-03 19:33:11.000000 seotools-0.1.2/.gitignore
+-rw-r--r--   0 james      (501) staff       (20)     1063 2023-08-03 19:09:09.000000 seotools-0.1.2/LICENSE
+-rw-r--r--   0 james      (501) staff       (20)      865 2023-08-03 09:42:54.000000 seotools-0.1.2/Makefile
+-rw-r--r--   0 james      (501) staff       (20)     3538 2023-08-07 10:25:18.599649 seotools-0.1.2/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)     3049 2023-08-05 09:35:07.000000 seotools-0.1.2/README.md
+-rw-r--r--   0 james      (501) staff       (20)      638 2023-08-04 22:27:54.000000 seotools-0.1.2/api.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-07 10:25:18.593565 seotools-0.1.2/docs/
+-rw-r--r--   0 james      (501) staff       (20)      159 2023-08-05 11:23:46.000000 seotools-0.1.2/docs/broken_links.md
+-rw-r--r--   0 james      (501) staff       (20)        0 2023-08-03 22:02:00.000000 seotools-0.1.2/docs/changelog.md
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-07 10:25:18.594102 seotools-0.1.2/docs/helpers/
+-rw-r--r--   0 james      (501) staff       (20)      392 2023-08-03 22:38:18.000000 seotools-0.1.2/docs/helpers/validate_googlebot_ips.md
+-rw-r--r--   0 james      (501) staff       (20)     2591 2023-08-03 22:41:36.000000 seotools-0.1.2/docs/index.md
+-rw-r--r--   0 james      (501) staff       (20)      565 2023-08-03 22:21:17.000000 seotools-0.1.2/docs/jsonld.md
+-rw-r--r--   0 james      (501) staff       (20)     1049 2023-08-03 22:17:37.000000 seotools-0.1.2/docs/recommendation.md
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-07 10:25:18.594493 seotools-0.1.2/docs/reference/
+-rw-r--r--   0 james      (501) staff       (20)      124 2023-08-03 22:11:54.000000 seotools-0.1.2/docs/reference/analyzer.md
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-07 10:25:18.594909 seotools-0.1.2/docs/styles/
+-rw-r--r--   0 james      (501) staff       (20)       95 2023-08-03 22:03:25.000000 seotools-0.1.2/docs/styles/styles.css
+-rw-r--r--   0 james      (501) staff       (20)     1106 2023-08-05 17:49:52.000000 seotools-0.1.2/mkdocs.yml
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-07 10:25:18.597435 seotools-0.1.2/seotools/
+-rw-r--r--   0 james      (501) staff       (20)       22 2023-08-07 10:25:07.000000 seotools-0.1.2/seotools/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)    16489 2023-08-05 12:31:12.000000 seotools-0.1.2/seotools/app.py
+-rw-r--r--   0 james      (501) staff       (20)      479 2023-08-05 12:31:10.000000 seotools-0.1.2/seotools/crawl_bot_validation.py
+-rw-r--r--   0 james      (501) staff       (20)     1480 2023-08-06 10:25:18.000000 seotools-0.1.2/seotools/forecast.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-07 10:25:18.599144 seotools-0.1.2/seotools/links/
+-rw-r--r--   0 james      (501) staff       (20)        0 2023-08-05 11:24:44.000000 seotools-0.1.2/seotools/links/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     1396 2023-08-05 11:24:02.000000 seotools-0.1.2/seotools/links/broken.py
+-rw-r--r--   0 james      (501) staff       (20)     6267 2023-08-06 10:25:48.000000 seotools-0.1.2/seotools/logs.py
+-rw-r--r--   0 james      (501) staff       (20)     1162 2023-08-05 11:21:39.000000 seotools-0.1.2/seotools/topics.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-07 10:25:18.598805 seotools-0.1.2/seotools.egg-info/
+-rw-r--r--   0 james      (501) staff       (20)     3538 2023-08-07 10:25:18.000000 seotools-0.1.2/seotools.egg-info/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)      582 2023-08-07 10:25:18.000000 seotools-0.1.2/seotools.egg-info/SOURCES.txt
+-rw-r--r--   0 james      (501) staff       (20)        1 2023-08-07 10:25:18.000000 seotools-0.1.2/seotools.egg-info/dependency_links.txt
+-rw-r--r--   0 james      (501) staff       (20)      161 2023-08-07 10:25:18.000000 seotools-0.1.2/seotools.egg-info/requires.txt
+-rw-r--r--   0 james      (501) staff       (20)        9 2023-08-07 10:25:18.000000 seotools-0.1.2/seotools.egg-info/top_level.txt
+-rw-r--r--   0 james      (501) staff       (20)       38 2023-08-07 10:25:18.599933 seotools-0.1.2/setup.cfg
+-rw-r--r--   0 james      (501) staff       (20)     1301 2023-08-06 10:25:40.000000 seotools-0.1.2/setup.py
```

### Comparing `seotools-0.1.1/.gitignore` & `seotools-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `seotools-0.1.1/LICENSE` & `seotools-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `seotools-0.1.1/Makefile` & `seotools-0.1.2/Makefile`

 * *Files identical despite different names*

### Comparing `seotools-0.1.1/PKG-INFO` & `seotools-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seotools
-Version: 0.1.1
+Version: 0.1.2
 Summary: A collection of tools for use with writing SEO-related programs in Python.
 Home-page: https://github.com/capjamesg/seotools
 Author: capjamesg
 Author-email: jamesg@jamesg.blog
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: seotools Version: 0.1.1 Summary: A collection of
+Metadata-Version: 2.1 Name: seotools Version: 0.1.2 Summary: A collection of
 tools for use with writing SEO-related programs in Python. Home-page: https://
 github.com/capjamesg/seotools Author: capjamesg Author-email:
 jamesg@jamesg.blog Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
 Provides-Extra: dev License-File: LICENSE [![version](https://badge.fury.io/py/
 seotools.svg?)](https://badge.fury.io/py/seotools) [![downloads](https://
```

### Comparing `seotools-0.1.1/README.md` & `seotools-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `seotools-0.1.1/api.py` & `seotools-0.1.2/api.py`

 * *Files identical despite different names*

### Comparing `seotools-0.1.1/docs/index.md` & `seotools-0.1.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `seotools-0.1.1/docs/jsonld.md` & `seotools-0.1.2/docs/jsonld.md`

 * *Files identical despite different names*

### Comparing `seotools-0.1.1/docs/recommendation.md` & `seotools-0.1.2/docs/recommendation.md`

 * *Files identical despite different names*

### Comparing `seotools-0.1.1/mkdocs.yml` & `seotools-0.1.2/mkdocs.yml`

 * *Files 15% similar despite different names*

```diff
@@ -15,14 +15,15 @@
   - Analyze Links: links.md
   - Identify Broken Links: broken_links.md
   - Build a Content Recommendation System: recommendation.md
   - Visualize Content Clusters: topic_clusters.md
   - Check for JSON-LD on a Page: jsonld.md
   - Reference:
     - Analyzer: reference/analyzer.md
+    - CrawlLogAnalyzer: reference/crawl_log_analyzer.md
   - Changelog: changelog.md
 
 theme:
   name: 'material'
   font:
     text: Roboto
     code: Roboto Mono
```

### Comparing `seotools-0.1.1/seotools/app.py` & `seotools-0.1.2/seotools/app.py`

 * *Files identical despite different names*

### Comparing `seotools-0.1.1/seotools/links/broken.py` & `seotools-0.1.2/seotools/links/broken.py`

 * *Files identical despite different names*

### Comparing `seotools-0.1.1/seotools/topics.py` & `seotools-0.1.2/seotools/topics.py`

 * *Files identical despite different names*

### Comparing `seotools-0.1.1/seotools.egg-info/PKG-INFO` & `seotools-0.1.2/seotools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seotools
-Version: 0.1.1
+Version: 0.1.2
 Summary: A collection of tools for use with writing SEO-related programs in Python.
 Home-page: https://github.com/capjamesg/seotools
 Author: capjamesg
 Author-email: jamesg@jamesg.blog
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: seotools Version: 0.1.1 Summary: A collection of
+Metadata-Version: 2.1 Name: seotools Version: 0.1.2 Summary: A collection of
 tools for use with writing SEO-related programs in Python. Home-page: https://
 github.com/capjamesg/seotools Author: capjamesg Author-email:
 jamesg@jamesg.blog Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
 Provides-Extra: dev License-File: LICENSE [![version](https://badge.fury.io/py/
 seotools.svg?)](https://badge.fury.io/py/seotools) [![downloads](https://
```

### Comparing `seotools-0.1.1/seotools.egg-info/SOURCES.txt` & `seotools-0.1.2/seotools.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 docs/recommendation.md
 docs/helpers/validate_googlebot_ips.md
 docs/reference/analyzer.md
 docs/styles/styles.css
 seotools/__init__.py
 seotools/app.py
 seotools/crawl_bot_validation.py
+seotools/forecast.py
+seotools/logs.py
 seotools/topics.py
 seotools.egg-info/PKG-INFO
 seotools.egg-info/SOURCES.txt
 seotools.egg-info/dependency_links.txt
 seotools.egg-info/requires.txt
 seotools.egg-info/top_level.txt
 seotools/links/__init__.py
```

### Comparing `seotools-0.1.1/setup.py` & `seotools-0.1.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,15 +22,18 @@
     install_requires=[
         "requests",
         "beautifulsoup4",
         "sentence-transformers",
         "networkx",
         "scikit-learn",
         "PyLD",
-        "indieweb-utils"
+        "indieweb-utils",
+        "prophet",
+        "pandas",
+        "tqdm",
     ],
     packages=find_packages(exclude=("tests",)),
     extras_require={
         "dev": ["flake8", "black==22.3.0", "isort", "twine", "pytest", "wheel"],
     },
     classifiers=[
         "Programming Language :: Python :: 3",
```

