# Comparing `tmp/robin_stocks-3.0.5.tar.gz` & `tmp/robin_stocks-3.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robin_stocks-3.0.5.tar", last modified: Thu Jul  6 03:30:33 2023, max compression
+gzip compressed data, was "robin_stocks-3.0.6.tar", last modified: Mon Aug  7 02:53:30 2023, max compression
```

## Comparing `robin_stocks-3.0.5.tar` & `robin_stocks-3.0.6.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-07-06 03:30:33.808555 robin_stocks-3.0.5/
--rw-r--r--   0 josh       (501) staff       (20)     1062 2018-10-17 16:32:18.000000 robin_stocks-3.0.5/LICENSE.txt
--rw-r--r--   0 josh       (501) staff       (20)       88 2018-09-27 04:22:53.000000 robin_stocks-3.0.5/MANIFEST.in
--rw-r--r--   0 josh       (501) staff       (20)     5087 2023-07-06 03:30:33.808074 robin_stocks-3.0.5/PKG-INFO
--rw-r--r--   0 josh       (501) staff       (20)     4629 2021-02-20 06:32:12.000000 robin_stocks-3.0.5/README.rst
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-07-06 03:30:33.787011 robin_stocks-3.0.5/robin_stocks/
--rw-r--r--   0 josh       (501) staff       (20)       47 2021-02-20 06:32:12.000000 robin_stocks-3.0.5/robin_stocks/__init__.py
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-07-06 03:30:33.793959 robin_stocks-3.0.5/robin_stocks/gemini/
--rw-r--r--   0 josh       (501) staff       (20)      789 2021-02-20 06:32:12.000000 robin_stocks-3.0.5/robin_stocks/gemini/__init__.py
--rw-r--r--   0 josh       (501) staff       (20)    12995 2021-02-20 06:32:12.000000 robin_stocks-3.0.5/robin_stocks/gemini/account.py
--rw-r--r--   0 josh       (501) staff       (20)     2499 2021-02-20 06:32:12.000000 robin_stocks-3.0.5/robin_stocks/gemini/authentication.py
--rw-r--r--   0 josh       (501) staff       (20)    10801 2021-02-20 06:32:12.000000 robin_stocks-3.0.5/robin_stocks/gemini/crypto.py
--rw-r--r--   0 josh       (501) staff       (20)      585 2021-02-20 06:32:12.000000 robin_stocks-3.0.5/robin_stocks/gemini/globals.py
--rw-r--r--   0 josh       (501) staff       (20)     6140 2021-02-20 06:32:12.000000 robin_stocks-3.0.5/robin_stocks/gemini/helper.py
--rw-r--r--   0 josh       (501) staff       (20)    18993 2021-02-20 06:32:12.000000 robin_stocks-3.0.5/robin_stocks/gemini/orders.py
--rw-r--r--   0 josh       (501) staff       (20)     3859 2021-02-20 06:32:12.000000 robin_stocks-3.0.5/robin_stocks/gemini/urls.py
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-07-06 03:30:33.800479 robin_stocks-3.0.5/robin_stocks/robinhood/
--rw-r--r--   0 josh       (501) staff       (20)     5064 2023-06-17 04:58:36.000000 robin_stocks-3.0.5/robin_stocks/robinhood/__init__.py
--rw-r--r--   0 josh       (501) staff       (20)    30664 2023-06-17 05:10:20.000000 robin_stocks-3.0.5/robin_stocks/robinhood/account.py
--rw-r--r--   0 josh       (501) staff       (20)     8596 2021-10-20 03:38:49.000000 robin_stocks-3.0.5/robin_stocks/robinhood/authentication.py
--rw-r--r--   0 josh       (501) staff       (20)     9715 2021-05-12 02:09:12.000000 robin_stocks-3.0.5/robin_stocks/robinhood/crypto.py
--rw-r--r--   0 josh       (501) staff       (20)     6602 2023-05-22 00:46:39.000000 robin_stocks-3.0.5/robin_stocks/robinhood/export.py
--rw-r--r--   0 josh       (501) staff       (20)      902 2021-02-20 06:32:12.000000 robin_stocks-3.0.5/robin_stocks/robinhood/globals.py
--rw-r--r--   0 josh       (501) staff       (20)    13321 2023-07-06 02:38:32.000000 robin_stocks-3.0.5/robin_stocks/robinhood/helper.py
--rw-r--r--   0 josh       (501) staff       (20)    11649 2021-02-27 17:30:21.000000 robin_stocks-3.0.5/robin_stocks/robinhood/markets.py
--rw-r--r--   0 josh       (501) staff       (20)    20412 2023-06-17 04:58:36.000000 robin_stocks-3.0.5/robin_stocks/robinhood/options.py
--rw-r--r--   0 josh       (501) staff       (20)    65728 2023-07-06 02:38:32.000000 robin_stocks-3.0.5/robin_stocks/robinhood/orders.py
--rw-r--r--   0 josh       (501) staff       (20)     9622 2023-05-22 00:46:39.000000 robin_stocks-3.0.5/robin_stocks/robinhood/profiles.py
--rw-r--r--   0 josh       (501) staff       (20)    25274 2023-07-06 02:38:32.000000 robin_stocks-3.0.5/robin_stocks/robinhood/stocks.py
--rw-r--r--   0 josh       (501) staff       (20)     7682 2023-07-06 02:38:32.000000 robin_stocks-3.0.5/robin_stocks/robinhood/urls.py
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-07-06 03:30:33.804880 robin_stocks-3.0.5/robin_stocks/tda/
--rw-r--r--   0 josh       (501) staff       (20)      713 2021-02-20 06:32:12.000000 robin_stocks-3.0.5/robin_stocks/tda/__init__.py
--rw-r--r--   0 josh       (501) staff       (20)     4761 2021-02-20 06:32:12.000000 robin_stocks-3.0.5/robin_stocks/tda/accounts.py
--rw-r--r--   0 josh       (501) staff       (20)     6608 2021-02-20 06:32:12.000000 robin_stocks-3.0.5/robin_stocks/tda/authentication.py
--rw-r--r--   0 josh       (501) staff       (20)      753 2021-02-20 06:32:12.000000 robin_stocks-3.0.5/robin_stocks/tda/globals.py
--rw-r--r--   0 josh       (501) staff       (20)     9765 2021-02-20 06:32:12.000000 robin_stocks-3.0.5/robin_stocks/tda/helper.py
--rw-r--r--   0 josh       (501) staff       (20)     3433 2021-02-20 06:32:12.000000 robin_stocks-3.0.5/robin_stocks/tda/markets.py
--rw-r--r--   0 josh       (501) staff       (20)     4714 2021-02-20 06:32:12.000000 robin_stocks-3.0.5/robin_stocks/tda/orders.py
--rw-r--r--   0 josh       (501) staff       (20)    12030 2021-02-20 06:33:23.000000 robin_stocks-3.0.5/robin_stocks/tda/stocks.py
--rw-r--r--   0 josh       (501) staff       (20)     3161 2021-02-20 06:32:12.000000 robin_stocks-3.0.5/robin_stocks/tda/urls.py
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-07-06 03:30:33.789833 robin_stocks-3.0.5/robin_stocks.egg-info/
--rw-r--r--   0 josh       (501) staff       (20)     5087 2023-07-06 03:30:33.000000 robin_stocks-3.0.5/robin_stocks.egg-info/PKG-INFO
--rw-r--r--   0 josh       (501) staff       (20)     1330 2023-07-06 03:30:33.000000 robin_stocks-3.0.5/robin_stocks.egg-info/SOURCES.txt
--rw-r--r--   0 josh       (501) staff       (20)        1 2023-07-06 03:30:33.000000 robin_stocks-3.0.5/robin_stocks.egg-info/dependency_links.txt
--rw-r--r--   0 josh       (501) staff       (20)        1 2018-02-23 03:52:33.000000 robin_stocks-3.0.5/robin_stocks.egg-info/not-zip-safe
--rw-r--r--   0 josh       (501) staff       (20)       42 2023-07-06 03:30:33.000000 robin_stocks-3.0.5/robin_stocks.egg-info/requires.txt
--rw-r--r--   0 josh       (501) staff       (20)       19 2023-07-06 03:30:33.000000 robin_stocks-3.0.5/robin_stocks.egg-info/top_level.txt
--rw-r--r--   0 josh       (501) staff       (20)       38 2023-07-06 03:30:33.808706 robin_stocks-3.0.5/setup.cfg
--rw-r--r--   0 josh       (501) staff       (20)      931 2023-07-06 02:38:52.000000 robin_stocks-3.0.5/setup.py
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-07-06 03:30:33.807455 robin_stocks-3.0.5/tests/
--rw-r--r--   0 josh       (501) staff       (20)        0 2020-06-15 04:00:04.000000 robin_stocks-3.0.5/tests/__init__.py
--rw-r--r--   0 josh       (501) staff       (20)     9843 2023-05-22 02:31:15.000000 robin_stocks-3.0.5/tests/app_tests.py
--rw-r--r--   0 josh       (501) staff       (20)     2157 2021-02-20 06:32:12.000000 robin_stocks-3.0.5/tests/test_gemini.py
--rw-r--r--   0 josh       (501) staff       (20)    32945 2023-07-06 02:51:59.000000 robin_stocks-3.0.5/tests/test_robinhood.py
--rw-r--r--   0 josh       (501) staff       (20)      571 2021-02-20 06:32:12.000000 robin_stocks-3.0.5/tests/test_tda.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-08-07 02:53:30.754207 robin_stocks-3.0.6/
+-rw-r--r--   0 josh       (501) staff       (20)     1062 2018-10-17 16:32:18.000000 robin_stocks-3.0.6/LICENSE.txt
+-rw-r--r--   0 josh       (501) staff       (20)       88 2018-09-27 04:22:53.000000 robin_stocks-3.0.6/MANIFEST.in
+-rw-r--r--   0 josh       (501) staff       (20)     5087 2023-08-07 02:53:30.753597 robin_stocks-3.0.6/PKG-INFO
+-rw-r--r--   0 josh       (501) staff       (20)     4629 2021-02-20 06:32:12.000000 robin_stocks-3.0.6/README.rst
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-08-07 02:53:30.713166 robin_stocks-3.0.6/robin_stocks/
+-rw-r--r--   0 josh       (501) staff       (20)       47 2021-02-20 06:32:12.000000 robin_stocks-3.0.6/robin_stocks/__init__.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-08-07 02:53:30.724437 robin_stocks-3.0.6/robin_stocks/gemini/
+-rw-r--r--   0 josh       (501) staff       (20)      789 2021-02-20 06:32:12.000000 robin_stocks-3.0.6/robin_stocks/gemini/__init__.py
+-rw-r--r--   0 josh       (501) staff       (20)    12995 2021-02-20 06:32:12.000000 robin_stocks-3.0.6/robin_stocks/gemini/account.py
+-rw-r--r--   0 josh       (501) staff       (20)     2499 2021-02-20 06:32:12.000000 robin_stocks-3.0.6/robin_stocks/gemini/authentication.py
+-rw-r--r--   0 josh       (501) staff       (20)    10801 2021-02-20 06:32:12.000000 robin_stocks-3.0.6/robin_stocks/gemini/crypto.py
+-rw-r--r--   0 josh       (501) staff       (20)      585 2021-02-20 06:32:12.000000 robin_stocks-3.0.6/robin_stocks/gemini/globals.py
+-rw-r--r--   0 josh       (501) staff       (20)     6140 2021-02-20 06:32:12.000000 robin_stocks-3.0.6/robin_stocks/gemini/helper.py
+-rw-r--r--   0 josh       (501) staff       (20)    18993 2021-02-20 06:32:12.000000 robin_stocks-3.0.6/robin_stocks/gemini/orders.py
+-rw-r--r--   0 josh       (501) staff       (20)     3859 2021-02-20 06:32:12.000000 robin_stocks-3.0.6/robin_stocks/gemini/urls.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-08-07 02:53:30.735188 robin_stocks-3.0.6/robin_stocks/robinhood/
+-rw-r--r--   0 josh       (501) staff       (20)     5064 2023-06-17 04:58:36.000000 robin_stocks-3.0.6/robin_stocks/robinhood/__init__.py
+-rw-r--r--   0 josh       (501) staff       (20)    30664 2023-06-17 05:10:20.000000 robin_stocks-3.0.6/robin_stocks/robinhood/account.py
+-rw-r--r--   0 josh       (501) staff       (20)     8596 2021-10-20 03:38:49.000000 robin_stocks-3.0.6/robin_stocks/robinhood/authentication.py
+-rw-r--r--   0 josh       (501) staff       (20)     9715 2021-05-12 02:09:12.000000 robin_stocks-3.0.6/robin_stocks/robinhood/crypto.py
+-rw-r--r--   0 josh       (501) staff       (20)     6602 2023-05-22 00:46:39.000000 robin_stocks-3.0.6/robin_stocks/robinhood/export.py
+-rw-r--r--   0 josh       (501) staff       (20)      902 2021-02-20 06:32:12.000000 robin_stocks-3.0.6/robin_stocks/robinhood/globals.py
+-rw-r--r--   0 josh       (501) staff       (20)    13293 2023-08-07 02:51:23.000000 robin_stocks-3.0.6/robin_stocks/robinhood/helper.py
+-rw-r--r--   0 josh       (501) staff       (20)    11649 2021-02-27 17:30:21.000000 robin_stocks-3.0.6/robin_stocks/robinhood/markets.py
+-rw-r--r--   0 josh       (501) staff       (20)    20412 2023-06-17 04:58:36.000000 robin_stocks-3.0.6/robin_stocks/robinhood/options.py
+-rw-r--r--   0 josh       (501) staff       (20)    65728 2023-08-07 02:51:23.000000 robin_stocks-3.0.6/robin_stocks/robinhood/orders.py
+-rw-r--r--   0 josh       (501) staff       (20)     9622 2023-05-22 00:46:39.000000 robin_stocks-3.0.6/robin_stocks/robinhood/profiles.py
+-rw-r--r--   0 josh       (501) staff       (20)    25274 2023-07-06 02:38:32.000000 robin_stocks-3.0.6/robin_stocks/robinhood/stocks.py
+-rw-r--r--   0 josh       (501) staff       (20)     7682 2023-07-06 02:38:32.000000 robin_stocks-3.0.6/robin_stocks/robinhood/urls.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-08-07 02:53:30.746057 robin_stocks-3.0.6/robin_stocks/tda/
+-rw-r--r--   0 josh       (501) staff       (20)      713 2021-02-20 06:32:12.000000 robin_stocks-3.0.6/robin_stocks/tda/__init__.py
+-rw-r--r--   0 josh       (501) staff       (20)     4761 2021-02-20 06:32:12.000000 robin_stocks-3.0.6/robin_stocks/tda/accounts.py
+-rw-r--r--   0 josh       (501) staff       (20)     6608 2021-02-20 06:32:12.000000 robin_stocks-3.0.6/robin_stocks/tda/authentication.py
+-rw-r--r--   0 josh       (501) staff       (20)      753 2021-02-20 06:32:12.000000 robin_stocks-3.0.6/robin_stocks/tda/globals.py
+-rw-r--r--   0 josh       (501) staff       (20)     9765 2021-02-20 06:32:12.000000 robin_stocks-3.0.6/robin_stocks/tda/helper.py
+-rw-r--r--   0 josh       (501) staff       (20)     3433 2021-02-20 06:32:12.000000 robin_stocks-3.0.6/robin_stocks/tda/markets.py
+-rw-r--r--   0 josh       (501) staff       (20)     4714 2021-02-20 06:32:12.000000 robin_stocks-3.0.6/robin_stocks/tda/orders.py
+-rw-r--r--   0 josh       (501) staff       (20)    12030 2021-02-20 06:33:23.000000 robin_stocks-3.0.6/robin_stocks/tda/stocks.py
+-rw-r--r--   0 josh       (501) staff       (20)     3161 2021-02-20 06:32:12.000000 robin_stocks-3.0.6/robin_stocks/tda/urls.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-08-07 02:53:30.718209 robin_stocks-3.0.6/robin_stocks.egg-info/
+-rw-r--r--   0 josh       (501) staff       (20)     5087 2023-08-07 02:53:30.000000 robin_stocks-3.0.6/robin_stocks.egg-info/PKG-INFO
+-rw-r--r--   0 josh       (501) staff       (20)     1330 2023-08-07 02:53:30.000000 robin_stocks-3.0.6/robin_stocks.egg-info/SOURCES.txt
+-rw-r--r--   0 josh       (501) staff       (20)        1 2023-08-07 02:53:30.000000 robin_stocks-3.0.6/robin_stocks.egg-info/dependency_links.txt
+-rw-r--r--   0 josh       (501) staff       (20)        1 2018-02-23 03:52:33.000000 robin_stocks-3.0.6/robin_stocks.egg-info/not-zip-safe
+-rw-r--r--   0 josh       (501) staff       (20)       42 2023-08-07 02:53:30.000000 robin_stocks-3.0.6/robin_stocks.egg-info/requires.txt
+-rw-r--r--   0 josh       (501) staff       (20)       19 2023-08-07 02:53:30.000000 robin_stocks-3.0.6/robin_stocks.egg-info/top_level.txt
+-rw-r--r--   0 josh       (501) staff       (20)       38 2023-08-07 02:53:30.754360 robin_stocks-3.0.6/setup.cfg
+-rw-r--r--   0 josh       (501) staff       (20)      931 2023-08-07 02:52:29.000000 robin_stocks-3.0.6/setup.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-08-07 02:53:30.752811 robin_stocks-3.0.6/tests/
+-rw-r--r--   0 josh       (501) staff       (20)        0 2020-06-15 04:00:04.000000 robin_stocks-3.0.6/tests/__init__.py
+-rw-r--r--   0 josh       (501) staff       (20)     9843 2023-05-22 02:31:15.000000 robin_stocks-3.0.6/tests/app_tests.py
+-rw-r--r--   0 josh       (501) staff       (20)     2157 2021-02-20 06:32:12.000000 robin_stocks-3.0.6/tests/test_gemini.py
+-rw-r--r--   0 josh       (501) staff       (20)    32945 2023-07-06 02:51:59.000000 robin_stocks-3.0.6/tests/test_robinhood.py
+-rw-r--r--   0 josh       (501) staff       (20)      571 2021-02-20 06:32:12.000000 robin_stocks-3.0.6/tests/test_tda.py
```

### Comparing `robin_stocks-3.0.5/LICENSE.txt` & `robin_stocks-3.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.5/PKG-INFO` & `robin_stocks-3.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robin_stocks
-Version: 3.0.5
+Version: 3.0.6
 Summary: A Python wrapper around the Robinhood API
 Home-page: https://github.com/jmfernandes/robin_stocks
 Author: Josh Fernandes
 Author-email: joshfernandes@mac.com
 License: MIT
 Keywords: robinhood,robin stocks,finance app,stocks,options,trading,investing
 Requires: requests
```

### Comparing `robin_stocks-3.0.5/README.rst` & `robin_stocks-3.0.6/README.rst`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.5/robin_stocks/gemini/__init__.py` & `robin_stocks-3.0.6/robin_stocks/gemini/__init__.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.5/robin_stocks/gemini/account.py` & `robin_stocks-3.0.6/robin_stocks/gemini/account.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.5/robin_stocks/gemini/authentication.py` & `robin_stocks-3.0.6/robin_stocks/gemini/authentication.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.5/robin_stocks/gemini/crypto.py` & `robin_stocks-3.0.6/robin_stocks/gemini/crypto.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.5/robin_stocks/gemini/globals.py` & `robin_stocks-3.0.6/robin_stocks/gemini/globals.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.5/robin_stocks/gemini/helper.py` & `robin_stocks-3.0.6/robin_stocks/gemini/helper.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.5/robin_stocks/gemini/orders.py` & `robin_stocks-3.0.6/robin_stocks/gemini/orders.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.5/robin_stocks/gemini/urls.py` & `robin_stocks-3.0.6/robin_stocks/gemini/urls.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.5/robin_stocks/robinhood/__init__.py` & `robin_stocks-3.0.6/robin_stocks/robinhood/__init__.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.5/robin_stocks/robinhood/account.py` & `robin_stocks-3.0.6/robin_stocks/robinhood/account.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.5/robin_stocks/robinhood/authentication.py` & `robin_stocks-3.0.6/robin_stocks/robinhood/authentication.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.5/robin_stocks/robinhood/crypto.py` & `robin_stocks-3.0.6/robin_stocks/robinhood/crypto.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.5/robin_stocks/robinhood/export.py` & `robin_stocks-3.0.6/robin_stocks/robinhood/export.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.5/robin_stocks/robinhood/globals.py` & `robin_stocks-3.0.6/robin_stocks/robinhood/globals.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.5/robin_stocks/robinhood/helper.py` & `robin_stocks-3.0.6/robin_stocks/robinhood/helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -345,20 +345,19 @@
         if json:
             update_session('Content-Type', 'application/json')
             res = SESSION.post(url, json=payload, timeout=timeout)
             update_session(
                 'Content-Type', 'application/x-www-form-urlencoded; charset=utf-8')
         else:
             res = SESSION.post(url, data=payload, timeout=timeout)
-        if res.status_code in [500,400]:
+        if res.status_code not in [200, 201, 202, 204, 301, 302, 303, 304, 307, 400, 401, 402, 403]:
             raise Exception("Received "+ str(res.status_code))
         data = res.json()
     except Exception as message:
         print("Error in request_post: {0}".format(message), file=get_output())
-    # Either return response <200,401,etc.> or the data that is returned from requests.
     if jsonify_data:
         return(data)
     else:
         return(res)
 
 
 def request_delete(url):
```

### Comparing `robin_stocks-3.0.5/robin_stocks/robinhood/markets.py` & `robin_stocks-3.0.6/robin_stocks/robinhood/markets.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.5/robin_stocks/robinhood/options.py` & `robin_stocks-3.0.6/robin_stocks/robinhood/options.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.5/robin_stocks/robinhood/orders.py` & `robin_stocks-3.0.6/robin_stocks/robinhood/orders.py`

 * *Files 0% similar despite different names*

```diff
@@ -897,15 +897,15 @@
     :type account_number: Optional[str]
     :param jsonify: If set to False, function will return the request object which contains status code and headers.
     :type jsonify: Optional[str]
     :returns: Dictionary that contains information regarding the trading of options, \
     such as the order id, the state of order (queued, confired, filled, failed, canceled, etc.), \
     the price, and the quantity.
     """
-    return(order_option_spread("credit", price, symbol, quantity, spread, timeInForce, account_number, jsonify))
+    return(order_option_spread("credit", price, symbol, quantity, spread, account_number, timeInForce, jsonify))
 
 
 @login_required
 def order_option_debit_spread(price, symbol, quantity, spread, timeInForce='gtc', account_number=None, jsonify=True):
     """Submits a limit order for an option debit spread.
 
     :param price: The limit price to trigger a sell of the option.
@@ -929,15 +929,15 @@
     :type account_number: Optional[str]
     :param jsonify: If set to False, function will return the request object which contains status code and headers.
     :type jsonify: Optional[str]
     :returns: Dictionary that contains information regarding the trading of options, \
     such as the order id, the state of order (queued, confired, filled, failed, canceled, etc.), \
     the price, and the quantity.
     """
-    return(order_option_spread("debit", price, symbol, quantity, spread, timeInForce, account_number, jsonify))
+    return(order_option_spread("debit", price, symbol, quantity, spread, account_number, timeInForce, jsonify))
 
 
 @login_required
 def order_option_spread(direction, price, symbol, quantity, spread, account_number=None, timeInForce='gtc', jsonify=True):
     """Submits a limit order for an option spread. i.e. place a debit / credit spread
 
     :param direction: Can be "credit" or "debit".
```

### Comparing `robin_stocks-3.0.5/robin_stocks/robinhood/profiles.py` & `robin_stocks-3.0.6/robin_stocks/robinhood/profiles.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.5/robin_stocks/robinhood/stocks.py` & `robin_stocks-3.0.6/robin_stocks/robinhood/stocks.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.5/robin_stocks/robinhood/urls.py` & `robin_stocks-3.0.6/robin_stocks/robinhood/urls.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.5/robin_stocks/tda/__init__.py` & `robin_stocks-3.0.6/robin_stocks/tda/__init__.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.5/robin_stocks/tda/accounts.py` & `robin_stocks-3.0.6/robin_stocks/tda/accounts.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.5/robin_stocks/tda/authentication.py` & `robin_stocks-3.0.6/robin_stocks/tda/authentication.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.5/robin_stocks/tda/globals.py` & `robin_stocks-3.0.6/robin_stocks/tda/globals.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.5/robin_stocks/tda/helper.py` & `robin_stocks-3.0.6/robin_stocks/tda/helper.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.5/robin_stocks/tda/markets.py` & `robin_stocks-3.0.6/robin_stocks/tda/markets.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.5/robin_stocks/tda/orders.py` & `robin_stocks-3.0.6/robin_stocks/tda/orders.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.5/robin_stocks/tda/stocks.py` & `robin_stocks-3.0.6/robin_stocks/tda/stocks.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.5/robin_stocks/tda/urls.py` & `robin_stocks-3.0.6/robin_stocks/tda/urls.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.5/robin_stocks.egg-info/PKG-INFO` & `robin_stocks-3.0.6/robin_stocks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robin-stocks
-Version: 3.0.5
+Version: 3.0.6
 Summary: A Python wrapper around the Robinhood API
 Home-page: https://github.com/jmfernandes/robin_stocks
 Author: Josh Fernandes
 Author-email: joshfernandes@mac.com
 License: MIT
 Keywords: robinhood,robin stocks,finance app,stocks,options,trading,investing
 Requires: requests
```

### Comparing `robin_stocks-3.0.5/robin_stocks.egg-info/SOURCES.txt` & `robin_stocks-3.0.6/robin_stocks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.5/setup.py` & `robin_stocks-3.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='robin_stocks',
-      version='3.0.5',
+      version='3.0.6',
       description='A Python wrapper around the Robinhood API',
       long_description=long_description,
       long_description_content_type='text/x-rst',
       url='https://github.com/jmfernandes/robin_stocks',
       author='Josh Fernandes',
       author_email='joshfernandes@mac.com',
       keywords=['robinhood','robin stocks','finance app','stocks','options','trading','investing'],
```

### Comparing `robin_stocks-3.0.5/tests/app_tests.py` & `robin_stocks-3.0.6/tests/app_tests.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.5/tests/test_gemini.py` & `robin_stocks-3.0.6/tests/test_gemini.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.5/tests/test_robinhood.py` & `robin_stocks-3.0.6/tests/test_robinhood.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.5/tests/test_tda.py` & `robin_stocks-3.0.6/tests/test_tda.py`

 * *Files identical despite different names*

