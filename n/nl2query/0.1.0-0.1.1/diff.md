# Comparing `tmp/nl2query-0.1.0.tar.gz` & `tmp/nl2query-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nl2query-0.1.0.tar", max compression
+gzip compressed data, was "nl2query-0.1.1.tar", max compression
```

## Comparing `nl2query-0.1.0.tar` & `nl2query-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rwxr-xr-x   0        0        0     1073 2023-06-25 23:12:59.048784 nl2query-0.1.0/LICENSE
--rwxr-xr-x   0        0        0        0 2023-06-25 23:13:00.170417 nl2query-0.1.0/README.md
--rwxr-xr-x   0        0        0      261 2023-08-06 23:25:17.006176 nl2query-0.1.0/nl2query/__init__.py
--rwxr-xr-x   0        0        0     1717 2023-08-06 23:25:17.009173 nl2query-0.1.0/nl2query/base.py
--rwxr-xr-x   0        0        0     4936 2023-08-06 23:25:17.012172 nl2query-0.1.0/nl2query/cypherquery.py
--rwxr-xr-x   0        0        0     3294 2023-08-06 23:25:17.015174 nl2query-0.1.0/nl2query/kustoquery.py
--rwxr-xr-x   0        0        0     3713 2023-08-06 23:25:17.018178 nl2query-0.1.0/nl2query/mongoquery.py
--rwxr-xr-x   0        0        0     3291 2023-08-06 23:25:17.021174 nl2query-0.1.0/nl2query/pandasquery.py
--rwxr-xr-x   0        0        0      386 2023-08-06 23:31:57.427275 nl2query-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      448 1970-01-01 00:00:00.000000 nl2query-0.1.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1073 2023-06-25 23:12:59.048784 nl2query-0.1.1/LICENSE
+-rwxr-xr-x   0        0        0        0 2023-06-25 23:13:00.170417 nl2query-0.1.1/README.md
+-rwxr-xr-x   0        0        0      261 2023-08-06 23:25:17.006176 nl2query-0.1.1/nl2query/__init__.py
+-rwxr-xr-x   0        0        0     1717 2023-08-06 23:25:17.009173 nl2query-0.1.1/nl2query/base.py
+-rwxr-xr-x   0        0        0     4936 2023-08-06 23:25:17.012172 nl2query-0.1.1/nl2query/cypherquery.py
+-rwxr-xr-x   0        0        0     3294 2023-08-06 23:25:17.015174 nl2query-0.1.1/nl2query/kustoquery.py
+-rwxr-xr-x   0        0        0     3713 2023-08-06 23:25:17.018178 nl2query-0.1.1/nl2query/mongoquery.py
+-rwxr-xr-x   0        0        0     3291 2023-08-06 23:25:17.021174 nl2query-0.1.1/nl2query/pandasquery.py
+-rwxr-xr-x   0        0        0      499 2023-08-07 02:01:33.044614 nl2query-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      601 1970-01-01 00:00:00.000000 nl2query-0.1.1/PKG-INFO
```

### Comparing `nl2query-0.1.0/LICENSE` & `nl2query-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nl2query-0.1.0/nl2query/base.py` & `nl2query-0.1.1/nl2query/base.py`

 * *Files identical despite different names*

### Comparing `nl2query-0.1.0/nl2query/cypherquery.py` & `nl2query-0.1.1/nl2query/cypherquery.py`

 * *Files identical despite different names*

### Comparing `nl2query-0.1.0/nl2query/kustoquery.py` & `nl2query-0.1.1/nl2query/kustoquery.py`

 * *Files identical despite different names*

### Comparing `nl2query-0.1.0/nl2query/mongoquery.py` & `nl2query-0.1.1/nl2query/mongoquery.py`

 * *Files identical despite different names*

### Comparing `nl2query-0.1.0/nl2query/pandasquery.py` & `nl2query-0.1.1/nl2query/pandasquery.py`

 * *Files identical despite different names*

