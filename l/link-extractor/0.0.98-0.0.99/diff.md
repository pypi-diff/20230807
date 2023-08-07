# Comparing `tmp/link_extractor-0.0.98.tar.gz` & `tmp/link_extractor-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/link_extractor-0.0.98.tar", last modified: Mon Feb 15 11:56:31 2021, max compression
+gzip compressed data, was "dist/link_extractor-0.0.99.tar", last modified: Tue Feb 16 15:42:02 2021, max compression
```

## Comparing `link_extractor-0.0.98.tar` & `link_extractor-0.0.99.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 yunzhi   (672583) primarygroup (89939)        0 2021-02-15 11:56:31.936779 link_extractor-0.0.98/
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      784 2021-02-15 11:56:31.936403 link_extractor-0.0.98/PKG-INFO
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      192 2020-07-13 23:56:47.000000 link_extractor-0.0.98/README.md
-drwxr-xr-x   0 yunzhi   (672583) primarygroup (89939)        0 2021-02-15 11:56:31.933098 link_extractor-0.0.98/link_extractor/
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)     3410 2020-12-22 17:44:08.000000 link_extractor-0.0.98/link_extractor/__init__.py
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)     1456 2021-02-15 11:56:26.000000 link_extractor-0.0.98/link_extractor/config.yaml
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      794 2020-12-18 19:23:59.000000 link_extractor-0.0.98/link_extractor/douban.py
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      503 2021-01-13 02:04:25.000000 link_extractor-0.0.98/link_extractor/get_soup.py
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      371 2020-08-14 23:01:34.000000 link_extractor-0.0.98/link_extractor/util.py
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      349 2020-08-14 21:36:08.000000 link_extractor-0.0.98/link_extractor/vocus.py
-drwxr-xr-x   0 yunzhi   (672583) primarygroup (89939)        0 2021-02-15 11:56:31.935818 link_extractor-0.0.98/link_extractor.egg-info/
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      784 2021-02-15 11:56:31.000000 link_extractor-0.0.98/link_extractor.egg-info/PKG-INFO
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      360 2021-02-15 11:56:31.000000 link_extractor-0.0.98/link_extractor.egg-info/SOURCES.txt
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)        1 2021-02-15 11:56:31.000000 link_extractor-0.0.98/link_extractor.egg-info/dependency_links.txt
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)       36 2021-02-15 11:56:31.000000 link_extractor-0.0.98/link_extractor.egg-info/requires.txt
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)       15 2021-02-15 11:56:31.000000 link_extractor-0.0.98/link_extractor.egg-info/top_level.txt
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)       38 2021-02-15 11:56:31.936891 link_extractor-0.0.98/setup.cfg
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      841 2021-02-15 11:56:29.000000 link_extractor-0.0.98/setup.py
+drwxr-xr-x   0 yunzhi   (672583) primarygroup (89939)        0 2021-02-16 15:42:02.378310 link_extractor-0.0.99/
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      784 2021-02-16 15:42:02.378045 link_extractor-0.0.99/PKG-INFO
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      192 2020-07-13 23:56:47.000000 link_extractor-0.0.99/README.md
+drwxr-xr-x   0 yunzhi   (672583) primarygroup (89939)        0 2021-02-16 15:42:02.375507 link_extractor-0.0.99/link_extractor/
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)     3410 2020-12-22 17:44:08.000000 link_extractor-0.0.99/link_extractor/__init__.py
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)     1536 2021-02-16 15:41:51.000000 link_extractor-0.0.99/link_extractor/config.yaml
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      794 2020-12-18 19:23:59.000000 link_extractor-0.0.99/link_extractor/douban.py
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      503 2021-01-13 02:04:25.000000 link_extractor-0.0.99/link_extractor/get_soup.py
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      371 2020-08-14 23:01:34.000000 link_extractor-0.0.99/link_extractor/util.py
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      349 2020-08-14 21:36:08.000000 link_extractor-0.0.99/link_extractor/vocus.py
+drwxr-xr-x   0 yunzhi   (672583) primarygroup (89939)        0 2021-02-16 15:42:02.377590 link_extractor-0.0.99/link_extractor.egg-info/
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      784 2021-02-16 15:42:02.000000 link_extractor-0.0.99/link_extractor.egg-info/PKG-INFO
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      360 2021-02-16 15:42:02.000000 link_extractor-0.0.99/link_extractor.egg-info/SOURCES.txt
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)        1 2021-02-16 15:42:02.000000 link_extractor-0.0.99/link_extractor.egg-info/dependency_links.txt
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)       36 2021-02-16 15:42:02.000000 link_extractor-0.0.99/link_extractor.egg-info/requires.txt
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)       15 2021-02-16 15:42:02.000000 link_extractor-0.0.99/link_extractor.egg-info/top_level.txt
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)       38 2021-02-16 15:42:02.378393 link_extractor-0.0.99/setup.cfg
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      841 2021-02-16 15:42:00.000000 link_extractor-0.0.99/setup.py
```

### Comparing `link_extractor-0.0.98/PKG-INFO` & `link_extractor-0.0.99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: link_extractor
-Version: 0.0.98
+Version: 0.0.99
 Summary: Extract Links from news source, ranked by importance.
 Home-page: https://github.com/gaoyunzhi/link_extractor
 Author: Yunzhi Gao
 Author-email: gaoyunzhi@gmail.com
 License: UNKNOWN
 Description: # link_extractor
```

### Comparing `link_extractor-0.0.98/link_extractor/__init__.py` & `link_extractor-0.0.99/link_extractor/__init__.py`

 * *Files identical despite different names*

### Comparing `link_extractor-0.0.98/link_extractor/config.yaml` & `link_extractor-0.0.99/link_extractor/config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -76,12 +76,16 @@
   must_contain_part: features
   sig_len: 
     - 7
 www.biede.com:
   not_contain:
     - name/
     - tag/
+equalityrights.hku.hk:
+  not_contain:
+    - Projects/
+  must_contain_part: post
 thenewslen:
   must_contain_part: article
 serviceworkercn.com:
   not_contain:
     - bulletin
```

### Comparing `link_extractor-0.0.98/link_extractor/douban.py` & `link_extractor-0.0.99/link_extractor/douban.py`

 * *Files identical despite different names*

### Comparing `link_extractor-0.0.98/link_extractor.egg-info/PKG-INFO` & `link_extractor-0.0.99/link_extractor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: link-extractor
-Version: 0.0.98
+Version: 0.0.99
 Summary: Extract Links from news source, ranked by importance.
 Home-page: https://github.com/gaoyunzhi/link_extractor
 Author: Yunzhi Gao
 Author-email: gaoyunzhi@gmail.com
 License: UNKNOWN
 Description: # link_extractor
```

### Comparing `link_extractor-0.0.98/setup.py` & `link_extractor-0.0.99/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="link_extractor",
-    version="0.0.98",
+    version="0.0.99",
     author="Yunzhi Gao",
     author_email="gaoyunzhi@gmail.com",
     description="Extract Links from news source, ranked by importance.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/gaoyunzhi/link_extractor",
     packages=setuptools.find_packages(),
```

