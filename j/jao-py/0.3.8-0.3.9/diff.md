# Comparing `tmp/jao-py-0.3.8.tar.gz` & `tmp/jao-py-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jao-py-0.3.8.tar", last modified: Thu Jun  1 07:53:46 2023, max compression
+gzip compressed data, was "jao-py-0.3.9.tar", last modified: Mon Aug  7 08:41:06 2023, max compression
```

## Comparing `jao-py-0.3.8.tar` & `jao-py-0.3.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:53:46.144340 jao-py-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-01 07:53:35.000000 jao-py-0.3.8/LICENSE.MD
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-06-01 07:53:46.144340 jao-py-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-01 07:53:35.000000 jao-py-0.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:53:46.140340 jao-py-0.3.8/jao/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:53:46.144340 jao-py-0.3.8/jao/CWE/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-01 07:53:35.000000 jao-py-0.3.8/jao/CWE/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-01 07:53:35.000000 jao-py-0.3.8/jao/CWE/definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-01 07:53:35.000000 jao-py-0.3.8/jao/CWE/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    14485 2023-06-01 07:53:35.000000 jao-py-0.3.8/jao/CWE/jao.py
--rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-06-01 07:53:35.000000 jao-py-0.3.8/jao/CWE/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-01 07:53:35.000000 jao-py-0.3.8/jao/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:53:46.144340 jao-py-0.3.8/jao/beta/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-01 07:53:35.000000 jao-py-0.3.8/jao/beta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-06-01 07:53:35.000000 jao-py-0.3.8/jao/beta/jao.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-01 07:53:35.000000 jao-py-0.3.8/jao/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7961 2023-06-01 07:53:35.000000 jao-py-0.3.8/jao/jao.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 07:53:35.000000 jao-py-0.3.8/jao/mappings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-06-01 07:53:35.000000 jao-py-0.3.8/jao/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-01 07:53:35.000000 jao-py-0.3.8/jao/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-06-01 07:53:35.000000 jao-py-0.3.8/jao/webservice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:53:46.144340 jao-py-0.3.8/jao_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-06-01 07:53:46.000000 jao-py-0.3.8/jao_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-01 07:53:46.000000 jao-py-0.3.8/jao_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 07:53:46.000000 jao-py-0.3.8/jao_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-01 07:53:46.000000 jao-py-0.3.8/jao_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-01 07:53:46.000000 jao-py-0.3.8/jao_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-01 07:53:46.144340 jao-py-0.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-06-01 07:53:35.000000 jao-py-0.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 08:41:06.906421 jao-py-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-07 08:40:58.000000 jao-py-0.3.9/LICENSE.MD
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-08-07 08:41:06.906421 jao-py-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-08-07 08:40:58.000000 jao-py-0.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 08:41:06.906421 jao-py-0.3.9/jao/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 08:41:06.906421 jao-py-0.3.9/jao/CWE/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-07 08:40:58.000000 jao-py-0.3.9/jao/CWE/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-08-07 08:40:58.000000 jao-py-0.3.9/jao/CWE/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-08-07 08:40:58.000000 jao-py-0.3.9/jao/CWE/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14485 2023-08-07 08:40:58.000000 jao-py-0.3.9/jao/CWE/jao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-08-07 08:40:58.000000 jao-py-0.3.9/jao/CWE/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-08-07 08:40:58.000000 jao-py-0.3.9/jao/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 08:41:06.906421 jao-py-0.3.9/jao/beta/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-07 08:40:58.000000 jao-py-0.3.9/jao/beta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-08-07 08:40:58.000000 jao-py-0.3.9/jao/beta/jao.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-07 08:40:58.000000 jao-py-0.3.9/jao/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8287 2023-08-07 08:40:58.000000 jao-py-0.3.9/jao/jao.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 08:40:58.000000 jao-py-0.3.9/jao/mappings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-08-07 08:40:58.000000 jao-py-0.3.9/jao/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-07 08:40:58.000000 jao-py-0.3.9/jao/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-08-07 08:40:58.000000 jao-py-0.3.9/jao/webservice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 08:41:06.906421 jao-py-0.3.9/jao_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-08-07 08:41:06.000000 jao-py-0.3.9/jao_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-08-07 08:41:06.000000 jao-py-0.3.9/jao_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 08:41:06.000000 jao-py-0.3.9/jao_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-07 08:41:06.000000 jao-py-0.3.9/jao_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-08-07 08:41:06.000000 jao-py-0.3.9/jao_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-07 08:41:06.906421 jao-py-0.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-08-07 08:40:58.000000 jao-py-0.3.9/setup.py
```

### Comparing `jao-py-0.3.8/LICENSE.MD` & `jao-py-0.3.9/LICENSE.MD`

 * *Files identical despite different names*

### Comparing `jao-py-0.3.8/PKG-INFO` & `jao-py-0.3.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jao-py
-Version: 0.3.8
+Version: 0.3.9
 Summary: A python API wrapper for JAO.eu
 Home-page: https://github.com/fboerman/jao-py
 Author: Frank Boerman
 Author-email: frank@fboerman.nl
 License: MIT
 Keywords: JAO data api energy
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `jao-py-0.3.8/README.md` & `jao-py-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `jao-py-0.3.8/jao/CWE/jao.py` & `jao-py-0.3.9/jao/CWE/jao.py`

 * *Files identical despite different names*

### Comparing `jao-py-0.3.8/jao/CWE/parsers.py` & `jao-py-0.3.9/jao/CWE/parsers.py`

 * *Files identical despite different names*

### Comparing `jao-py-0.3.8/jao/beta/jao.py` & `jao-py-0.3.9/jao/beta/jao.py`

 * *Files identical despite different names*

### Comparing `jao-py-0.3.8/jao/jao.py` & `jao-py-0.3.9/jao/jao.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import itertools
 from .exceptions import NoMatchingDataError
 from .parsers import parse_final_domain, parse_base_output
 from typing import List, Dict
 from .util import to_snake_case
 
 __title__ = "jao-py"
-__version__ = "0.3.8"
+__version__ = "0.3.9"
 __author__ = "Frank Boerman"
 __license__ = "MIT"
 
 
 class JaoPublicationToolClient:
     BASEURL = "https://publicationtool.jao.eu/core/api/core/"
     BASEURL2 = "https://publicationtool.jao.eu/core/api/data/"
@@ -121,14 +121,17 @@
             r.raise_for_status()
             data += r.json()['data']
         if len(data) == 0:
             raise NoMatchingDataError
 
         return data
 
+    def query_lta(self, d_from: pd.Timestamp, d_to: pd.Timestamp) -> List[Dict]:
+        return self._query_base_fromto(d_from, d_to, 'lta')
+
     def query_validations(self, d_from: pd.Timestamp, d_to: pd.Timestamp) -> List[Dict]:
         return self._query_base_fromto(d_from, d_to, 'validationReductions')
 
     def query_maxbex(self, day: pd.Timestamp) -> List[Dict]:
         return self._query_base(day, 'maxExchanges')
 
     def query_minmax_np(self, day: pd.Timestamp) -> List[Dict]:
@@ -180,14 +183,19 @@
         return df
 
     def query_minmax_np(self, day: pd.Timestamp) -> pd.DataFrame:
         return parse_base_output(
             super().query_minmax_np(day=day)
         )
 
+    def query_lta(self, d_from: pd.Timestamp, d_to: pd.Timestamp) -> pd.DataFrame:
+        return parse_base_output(
+            super().query_lta(d_from=d_from, d_to=d_to)
+        )
+
     def query_validations(self, d_from: pd.Timestamp, d_to: pd.Timestamp) -> pd.DataFrame:
         df = parse_base_output(
             super().query_validations(d_from=d_from, d_to=d_to)
         ).rename(columns=to_snake_case)
         df['last_modified_on'] = pd.to_datetime(df['last_modified_on'], utc=True).dt.tz_convert('europe/amsterdam')
 
         return df
```

### Comparing `jao-py-0.3.8/jao/parsers.py` & `jao-py-0.3.9/jao/parsers.py`

 * *Files identical despite different names*

### Comparing `jao-py-0.3.8/jao/webservice.py` & `jao-py-0.3.9/jao/webservice.py`

 * *Files identical despite different names*

### Comparing `jao-py-0.3.8/jao_py.egg-info/PKG-INFO` & `jao-py-0.3.9/jao_py.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jao-py
-Version: 0.3.8
+Version: 0.3.9
 Summary: A python API wrapper for JAO.eu
 Home-page: https://github.com/fboerman/jao-py
 Author: Frank Boerman
 Author-email: frank@fboerman.nl
 License: MIT
 Keywords: JAO data api energy
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `jao-py-0.3.8/setup.py` & `jao-py-0.3.9/setup.py`

 * *Files identical despite different names*

