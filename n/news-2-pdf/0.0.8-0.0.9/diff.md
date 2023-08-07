# Comparing `tmp/news_2_pdf-0.0.8.tar.gz` & `tmp/news_2_pdf-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/news_2_pdf-0.0.8.tar", last modified: Tue Jan  7 22:03:40 2020, max compression
+gzip compressed data, was "dist/news_2_pdf-0.0.9.tar", last modified: Thu Jan  9 19:17:50 2020, max compression
```

## Comparing `news_2_pdf-0.0.8.tar` & `news_2_pdf-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 yunzhi   (672583) primarygroup (89939)        0 2020-01-07 22:03:40.000000 news_2_pdf-0.0.8/
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      867 2020-01-07 22:03:40.000000 news_2_pdf-0.0.8/PKG-INFO
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      294 2019-12-31 22:15:32.000000 news_2_pdf-0.0.8/README.md
-drwxr-xr-x   0 yunzhi   (672583) primarygroup (89939)        0 2020-01-07 22:03:40.000000 news_2_pdf-0.0.8/news_2_pdf/
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)     1160 2019-12-31 22:50:25.000000 news_2_pdf-0.0.8/news_2_pdf/__init__.py
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      710 2019-12-31 22:15:32.000000 news_2_pdf-0.0.8/news_2_pdf/article.py
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)     1247 2019-12-31 22:45:55.000000 news_2_pdf-0.0.8/news_2_pdf/find_links.py
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      735 2020-01-07 22:03:10.000000 news_2_pdf-0.0.8/news_2_pdf/index.py
-drwxr-xr-x   0 yunzhi   (672583) primarygroup (89939)        0 2020-01-07 22:03:40.000000 news_2_pdf-0.0.8/news_2_pdf.egg-info/
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      867 2020-01-07 22:03:39.000000 news_2_pdf-0.0.8/news_2_pdf.egg-info/PKG-INFO
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      277 2020-01-07 22:03:39.000000 news_2_pdf-0.0.8/news_2_pdf.egg-info/SOURCES.txt
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)        1 2020-01-07 22:03:39.000000 news_2_pdf-0.0.8/news_2_pdf.egg-info/dependency_links.txt
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)       66 2020-01-07 22:03:39.000000 news_2_pdf-0.0.8/news_2_pdf.egg-info/requires.txt
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)       11 2020-01-07 22:03:39.000000 news_2_pdf-0.0.8/news_2_pdf.egg-info/top_level.txt
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)       38 2020-01-07 22:03:40.000000 news_2_pdf-0.0.8/setup.cfg
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      800 2020-01-07 21:59:47.000000 news_2_pdf-0.0.8/setup.py
+drwxr-xr-x   0 yunzhi   (672583) primarygroup (89939)        0 2020-01-09 19:17:50.000000 news_2_pdf-0.0.9/
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      867 2020-01-09 19:17:50.000000 news_2_pdf-0.0.9/PKG-INFO
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      294 2019-12-31 22:15:32.000000 news_2_pdf-0.0.9/README.md
+drwxr-xr-x   0 yunzhi   (672583) primarygroup (89939)        0 2020-01-09 19:17:50.000000 news_2_pdf-0.0.9/news_2_pdf/
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)     1176 2020-01-09 19:16:00.000000 news_2_pdf-0.0.9/news_2_pdf/__init__.py
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      793 2020-01-09 19:10:18.000000 news_2_pdf-0.0.9/news_2_pdf/article.py
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)     1938 2020-01-09 18:57:47.000000 news_2_pdf-0.0.9/news_2_pdf/find_links.py
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      818 2020-01-09 19:15:29.000000 news_2_pdf-0.0.9/news_2_pdf/index.py
+drwxr-xr-x   0 yunzhi   (672583) primarygroup (89939)        0 2020-01-09 19:17:50.000000 news_2_pdf-0.0.9/news_2_pdf.egg-info/
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      867 2020-01-09 19:17:50.000000 news_2_pdf-0.0.9/news_2_pdf.egg-info/PKG-INFO
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      277 2020-01-09 19:17:50.000000 news_2_pdf-0.0.9/news_2_pdf.egg-info/SOURCES.txt
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)        1 2020-01-09 19:17:50.000000 news_2_pdf-0.0.9/news_2_pdf.egg-info/dependency_links.txt
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)       66 2020-01-09 19:17:50.000000 news_2_pdf-0.0.9/news_2_pdf.egg-info/requires.txt
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)       11 2020-01-09 19:17:50.000000 news_2_pdf-0.0.9/news_2_pdf.egg-info/top_level.txt
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)       38 2020-01-09 19:17:50.000000 news_2_pdf-0.0.9/setup.cfg
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      800 2020-01-09 17:07:34.000000 news_2_pdf-0.0.9/setup.py
```

### Comparing `news_2_pdf-0.0.8/PKG-INFO` & `news_2_pdf-0.0.9/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: news_2_pdf
-Version: 0.0.8
+Version: 0.0.9
 Summary: Generate international news in pdf.
 Home-page: https://github.com/gaoyunzhi/news_2_pdf
 Author: Yunzhi Gao
 Author-email: gaoyunzhi@gmail.com
 License: UNKNOWN
 Description: # news_2_pdf
```

### Comparing `news_2_pdf-0.0.8/news_2_pdf/__init__.py` & `news_2_pdf-0.0.9/news_2_pdf/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,33 +2,33 @@
 # -*- coding: utf-8 -*-
 
 name = 'news_2_pdf'
 
 import os
 from .find_links import findLinks
 from .article import getArticleHtml
-from .index import getIndexHtml
+from .index import getIndexHtml, cleanName
 from datetime import date
 
 if os.name == 'posix':
 	ebook_convert_app = '/Applications/calibre.app/Contents/MacOS/ebook-convert'
 else:
 	ebook_convert_app = 'ebook-convert'
 
 def gen(news_source='bbc', ebook_convert_app=ebook_convert_app):
 	links = findLinks(news_source)
-	filename = '今日新闻%s%s' % (news_source, date.today().strftime("%y%m%d"))
+	filename = '%s%s' % (date.today().strftime("%m%d"), news_source.upper())
 
 	os.system('rm -rf html_result')	
 	os.system('mkdir html_result > /dev/null 2>&1')
 
 	for name, link in links.copy().items():
 		html = getArticleHtml(name, link, filename + '.html')
 		if html:
-			with open('html_result/%s.html' % name, 'w') as f:
+			with open('html_result/%s.html' % cleanName(name), 'w') as f:
 				f.write(html)
 		else:
 			del links[name]
 
 	index_html_name = 'html_result/%s.html' % filename
 	with open(index_html_name, 'w') as f:
 		f.write(getIndexHtml(news_source, links))
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `news_2_pdf-0.0.8/news_2_pdf.egg-info/PKG-INFO` & `news_2_pdf-0.0.9/news_2_pdf.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: news-2-pdf
-Version: 0.0.8
+Version: 0.0.9
 Summary: Generate international news in pdf.
 Home-page: https://github.com/gaoyunzhi/news_2_pdf
 Author: Yunzhi Gao
 Author-email: gaoyunzhi@gmail.com
 License: UNKNOWN
 Description: # news_2_pdf
```

### Comparing `news_2_pdf-0.0.8/setup.py` & `news_2_pdf-0.0.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="news_2_pdf",
-    version="0.0.8",
+    version="0.0.9",
     author="Yunzhi Gao",
     author_email="gaoyunzhi@gmail.com",
     description="Generate international news in pdf.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/gaoyunzhi/news_2_pdf",
     packages=setuptools.find_packages(),
```

