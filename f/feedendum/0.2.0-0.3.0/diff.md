# Comparing `tmp/feedendum-0.2.0.tar.gz` & `tmp/feedendum-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feedendum-0.2.0.tar", last modified: Tue Jul  5 12:54:43 2022, max compression
+gzip compressed data, was "feedendum-0.3.0.tar", last modified: Mon Aug  7 14:04:11 2023, max compression
```

## Comparing `feedendum-0.2.0.tar` & `feedendum-0.3.0.tar`

### file list

```diff
@@ -1,20 +1,18 @@
-drwxrwxrwx   0        0        0        0 2022-07-05 12:54:43.101629 feedendum-0.2.0/
--rw-rw-rw-   0        0        0    35184 2022-06-20 08:17:55.000000 feedendum-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     1850 2022-07-05 12:54:43.100632 feedendum-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1185 2022-06-20 08:17:55.000000 feedendum-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2022-07-05 12:54:43.095723 feedendum-0.2.0/feedendum/
--rw-rw-rw-   0        0        0      711 2022-06-20 08:17:55.000000 feedendum-0.2.0/feedendum/__init__.py
--rw-rw-rw-   0        0        0       23 2022-07-05 12:36:24.000000 feedendum-0.2.0/feedendum/__version__.py
--rw-rw-rw-   0        0        0     4555 2022-07-05 12:43:01.000000 feedendum-0.2.0/feedendum/atom.py
--rw-rw-rw-   0        0        0      311 2022-06-20 08:17:55.000000 feedendum-0.2.0/feedendum/exceptions.py
--rw-rw-rw-   0        0        0     2211 2022-07-05 12:50:21.000000 feedendum-0.2.0/feedendum/feed.py
--rw-rw-rw-   0        0        0     3975 2022-07-05 12:42:46.000000 feedendum-0.2.0/feedendum/rss.py
--rw-rw-rw-   0        0        0     3535 2022-07-05 12:39:06.000000 feedendum-0.2.0/feedendum/utils.py
-drwxrwxrwx   0        0        0        0 2022-07-05 12:54:43.099633 feedendum-0.2.0/feedendum.egg-info/
--rw-rw-rw-   0        0        0     1850 2022-07-05 12:54:42.000000 feedendum-0.2.0/feedendum.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      333 2022-07-05 12:54:43.000000 feedendum-0.2.0/feedendum.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-05 12:54:42.000000 feedendum-0.2.0/feedendum.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2022-07-05 12:54:42.000000 feedendum-0.2.0/feedendum.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2022-07-05 12:54:42.000000 feedendum-0.2.0/feedendum.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-07-05 12:54:43.101629 feedendum-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     3061 2022-07-04 16:00:12.000000 feedendum-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 14:04:11.340369 feedendum-0.3.0/
+-rw-rw-rw-   0        0        0    35184 2022-06-20 08:17:55.000000 feedendum-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0    42540 2023-08-07 14:04:11.326448 feedendum-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1388 2023-08-07 13:16:35.000000 feedendum-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-08-07 14:04:11.185124 feedendum-0.3.0/feedendum/
+drwxrwxrwx   0        0        0        0 2023-08-07 14:04:11.255013 feedendum-0.3.0/feedendum/feedendum.egg-info/
+-rw-rw-rw-   0        0        0    42540 2023-08-07 14:04:11.000000 feedendum-0.3.0/feedendum/feedendum.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2023-08-07 14:04:11.000000 feedendum-0.3.0/feedendum/feedendum.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 14:04:11.000000 feedendum-0.3.0/feedendum/feedendum.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-08-07 14:04:11.000000 feedendum-0.3.0/feedendum/feedendum.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 14:04:11.000000 feedendum-0.3.0/feedendum/feedendum.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      994 2023-08-07 14:01:11.000000 feedendum-0.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-07 14:04:11.340369 feedendum-0.3.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-07 14:04:11.313281 feedendum-0.3.0/tests/
+-rw-rw-rw-   0        0        0     5042 2023-08-07 13:57:32.000000 feedendum-0.3.0/tests/test_atom.py
+-rw-rw-rw-   0        0        0     4408 2022-07-05 12:49:17.000000 feedendum-0.3.0/tests/test_feed.py
+-rw-rw-rw-   0        0        0     7114 2023-08-07 13:58:07.000000 feedendum-0.3.0/tests/test_rdf.py
+-rw-rw-rw-   0        0        0     6639 2023-08-07 13:57:41.000000 feedendum-0.3.0/tests/test_rss.py
```

### Comparing `feedendum-0.2.0/LICENSE` & `feedendum-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `feedendum-0.2.0/README.md` & `feedendum-0.3.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 # feedendum
 A python library to parse and generate RSS or atom feeds.
 
 ## Features
 
 This module can:
 
-* parse RSS text and file
-* parse Atom text and file
-* read an url if `requests` is installed
+* parse and generate RSS feeds
+* parse and generate RDF (RSS v1.0) feeds (thanks to @inigoserna)
+* parse and generate Atom feeds
 * access standard fields via `feed` class and `feed.item` list
+* preserve all data parsed, even in custom fields, when generating a RSS/Atom/RDF text
+* read an url if `requests` is installed
 * access non-standard fields via `_data` dict
 * create arbitrary feed
 * modify an existing feed
-* generate a RSS text
-* generate an Atom text
-* preserve all data parsed, even in custom fields, when generating a RSS/Atom text
 
 ## Usage
 
 ### Parsing a file
 
 For RSS:
 
     feed = feedendum.from_rss_file(file_path)
     feed = feedendum.from_rss_text(txt)
 
+For RDF (RSS v1.0): 
+
+    feed = feedendum.from_rdf_file(file_path)
+    feed = feedendum.from_rdf_text(txt)
+
 For Atom:
 
     feed = feedendum.from_atom_file(file_path)
     feed = feedendum.from_atom_text(txt)
 
 ### Accessing to parsed data
 
@@ -44,12 +48,14 @@
 
 ### Writing a file
 
 For RSS:
 
     feedendum.to_rss_string(feed)
 
-For Atom:
+For RDF (RSS v1.0):
 
-    feedendum.to_atom_string(feed)
+    feedendum.to_rdf_string(feed)
 
+For Atom:
 
+    feedendum.to_atom_string(feed)
```

