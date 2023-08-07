# Comparing `tmp/readee-0.0.98.tar.gz` & `tmp/readee-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/readee-0.0.98.tar", last modified: Tue Feb 16 14:02:32 2021, max compression
+gzip compressed data, was "dist/readee-0.0.99.tar", last modified: Sun Mar 28 20:04:28 2021, max compression
```

## Comparing `readee-0.0.98.tar` & `readee-0.0.99.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 yunzhi   (672583) primarygroup (89939)        0 2021-02-16 14:02:32.025721 readee-0.0.98/
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      916 2021-02-16 14:02:32.024846 readee-0.0.98/PKG-INFO
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      314 2020-03-24 15:33:52.000000 readee-0.0.98/README.md
-drwxr-xr-x   0 yunzhi   (672583) primarygroup (89939)        0 2021-02-16 14:02:32.021252 readee-0.0.98/readee/
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      606 2020-05-12 15:12:38.000000 readee-0.0.98/readee/__init__.py
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      702 2021-01-09 02:54:08.000000 readee-0.0.98/readee/article.py
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      593 2019-12-31 21:30:59.000000 readee-0.0.98/readee/common.py
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)     1403 2021-01-09 02:56:10.000000 readee-0.0.98/readee/content.py
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      452 2020-07-27 11:23:38.000000 readee-0.0.98/readee/domain.py
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      586 2020-03-24 15:29:42.000000 readee-0.0.98/readee/final_touch.py
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)     3893 2021-02-16 13:54:56.000000 readee-0.0.98/readee/images.py
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)     3459 2021-02-16 14:01:45.000000 readee-0.0.98/readee/inner_article.py
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      456 2020-03-24 15:33:20.000000 readee-0.0.98/readee/link.py
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)     4607 2021-02-16 14:01:14.000000 readee-0.0.98/readee/offtopic.py
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)     1701 2020-11-16 16:15:35.000000 readee-0.0.98/readee/tag_replace.py
-drwxr-xr-x   0 yunzhi   (672583) primarygroup (89939)        0 2021-02-16 14:02:32.023910 readee-0.0.98/readee.egg-info/
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      916 2021-02-16 14:02:31.000000 readee-0.0.98/readee.egg-info/PKG-INFO
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      375 2021-02-16 14:02:31.000000 readee-0.0.98/readee.egg-info/SOURCES.txt
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)        1 2021-02-16 14:02:31.000000 readee-0.0.98/readee.egg-info/dependency_links.txt
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)       74 2021-02-16 14:02:31.000000 readee-0.0.98/readee.egg-info/requires.txt
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)        7 2021-02-16 14:02:31.000000 readee-0.0.98/readee.egg-info/top_level.txt
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)       38 2021-02-16 14:02:32.025981 readee-0.0.98/setup.cfg
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      814 2021-02-16 14:02:28.000000 readee-0.0.98/setup.py
+drwxr-xr-x   0 yunzhi   (672583) primarygroup (89939)        0 2021-03-28 20:04:28.120022 readee-0.0.99/
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      916 2021-03-28 20:04:28.119644 readee-0.0.99/PKG-INFO
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      314 2020-03-24 15:33:52.000000 readee-0.0.99/README.md
+drwxr-xr-x   0 yunzhi   (672583) primarygroup (89939)        0 2021-03-28 20:04:28.116667 readee-0.0.99/readee/
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      606 2020-05-12 15:12:38.000000 readee-0.0.99/readee/__init__.py
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      702 2021-01-09 02:54:08.000000 readee-0.0.99/readee/article.py
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      593 2019-12-31 21:30:59.000000 readee-0.0.99/readee/common.py
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)     1403 2021-01-09 02:56:10.000000 readee-0.0.99/readee/content.py
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      452 2020-07-27 11:23:38.000000 readee-0.0.99/readee/domain.py
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      586 2020-03-24 15:29:42.000000 readee-0.0.99/readee/final_touch.py
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)     3893 2021-02-16 13:54:56.000000 readee-0.0.99/readee/images.py
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)     3518 2021-03-28 20:04:09.000000 readee-0.0.99/readee/inner_article.py
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      456 2020-03-24 15:33:20.000000 readee-0.0.99/readee/link.py
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)     4607 2021-02-16 14:01:14.000000 readee-0.0.99/readee/offtopic.py
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)     1701 2020-11-16 16:15:35.000000 readee-0.0.99/readee/tag_replace.py
+drwxr-xr-x   0 yunzhi   (672583) primarygroup (89939)        0 2021-03-28 20:04:28.119027 readee-0.0.99/readee.egg-info/
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      916 2021-03-28 20:04:27.000000 readee-0.0.99/readee.egg-info/PKG-INFO
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      375 2021-03-28 20:04:27.000000 readee-0.0.99/readee.egg-info/SOURCES.txt
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)        1 2021-03-28 20:04:27.000000 readee-0.0.99/readee.egg-info/dependency_links.txt
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)       74 2021-03-28 20:04:27.000000 readee-0.0.99/readee.egg-info/requires.txt
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)        7 2021-03-28 20:04:27.000000 readee-0.0.99/readee.egg-info/top_level.txt
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)       38 2021-03-28 20:04:28.120155 readee-0.0.99/setup.cfg
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      814 2021-03-28 20:04:26.000000 readee-0.0.99/setup.py
```

### Comparing `readee-0.0.98/PKG-INFO` & `readee-0.0.99/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readee
-Version: 0.0.98
+Version: 0.0.99
 Summary: Library for export webpage to reader mode html.
 Home-page: https://github.com/gaoyunzhi/readee
 Author: Yunzhi Gao
 Author-email: gaoyunzhi@gmail.com
 License: UNKNOWN
 Description: # readee
```

### Comparing `readee-0.0.98/readee/__init__.py` & `readee-0.0.99/readee/__init__.py`

 * *Files identical despite different names*

### Comparing `readee-0.0.98/readee/article.py` & `readee-0.0.99/readee/article.py`

 * *Files identical despite different names*

### Comparing `readee-0.0.98/readee/common.py` & `readee-0.0.99/readee/common.py`

 * *Files identical despite different names*

### Comparing `readee-0.0.98/readee/content.py` & `readee-0.0.99/readee/content.py`

 * *Files identical despite different names*

### Comparing `readee-0.0.98/readee/final_touch.py` & `readee-0.0.99/readee/final_touch.py`

 * *Files identical despite different names*

### Comparing `readee-0.0.98/readee/images.py` & `readee-0.0.99/readee/images.py`

 * *Files identical despite different names*

### Comparing `readee-0.0.98/readee/inner_article.py` & `readee-0.0.99/readee/inner_article.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,14 +58,15 @@
 		'chinaworker.': [lambda x: x.find("div", class_ = 'pf-content'),],
 		'thesocietypages.org': [lambda x: x.find("div", class_ = 'post-content'),],
 		'chinadigitaltimes.': [lambda x: x.find("div", class_ = 'post-content'),],
 		'twreporter.org':[lambda x: x.find("div", {"id" : "article-body"}),],
 		'bbc.co.uk': [lambda x: x.find("div", {"dir": "ltr"})],
 		'bbc.com': [lambda x: x.find("article"), lambda x: x.find("main")],
 		'equalityrights.hku.hk': [lambda x: x.find("article")],
+		'biede.com': [lambda x: x.find("div", class_ = 'lay'),],
 	}
 	is_short = matchKey(soup.text, SHORT_ARTICLE)
 	text_limit = 150 if is_short else 500
 	for applicator in applicators:
 		candidate = applicator(soup)
 		if _seemsValidRawArticle(candidate, text_limit = text_limit):
 			soup = candidate
```

### Comparing `readee-0.0.98/readee/offtopic.py` & `readee-0.0.99/readee/offtopic.py`

 * *Files identical despite different names*

### Comparing `readee-0.0.98/readee/tag_replace.py` & `readee-0.0.99/readee/tag_replace.py`

 * *Files identical despite different names*

### Comparing `readee-0.0.98/readee.egg-info/PKG-INFO` & `readee-0.0.99/readee.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readee
-Version: 0.0.98
+Version: 0.0.99
 Summary: Library for export webpage to reader mode html.
 Home-page: https://github.com/gaoyunzhi/readee
 Author: Yunzhi Gao
 Author-email: gaoyunzhi@gmail.com
 License: UNKNOWN
 Description: # readee
```

### Comparing `readee-0.0.98/setup.py` & `readee-0.0.99/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="readee",
-    version="0.0.98",
+    version="0.0.99",
     author="Yunzhi Gao",
     author_email="gaoyunzhi@gmail.com",
     description="Library for export webpage to reader mode html.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/gaoyunzhi/readee",
     packages=setuptools.find_packages(),
```

