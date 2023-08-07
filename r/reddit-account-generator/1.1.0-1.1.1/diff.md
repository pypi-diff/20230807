# Comparing `tmp/reddit-account-generator-1.1.0.tar.gz` & `tmp/reddit-account-generator-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reddit-account-generator-1.1.0.tar", last modified: Tue Aug  1 08:59:31 2023, max compression
+gzip compressed data, was "reddit-account-generator-1.1.1.tar", last modified: Mon Aug  7 10:24:32 2023, max compression
```

## Comparing `reddit-account-generator-1.1.0.tar` & `reddit-account-generator-1.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:59:31.883876 reddit-account-generator-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-08-01 08:59:20.000000 reddit-account-generator-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-08-01 08:59:31.883876 reddit-account-generator-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-08-01 08:59:20.000000 reddit-account-generator-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:59:31.879876 reddit-account-generator-1.1.0/reddit_account_generator/
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-08-01 08:59:20.000000 reddit-account-generator-1.1.0/reddit_account_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-01 08:59:20.000000 reddit-account-generator-1.1.0/reddit_account_generator/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-08-01 08:59:20.000000 reddit-account-generator-1.1.0/reddit_account_generator/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6310 2023-08-01 08:59:20.000000 reddit-account-generator-1.1.0/reddit_account_generator/maker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-08-01 08:59:20.000000 reddit-account-generator-1.1.0/reddit_account_generator/protector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-08-01 08:59:20.000000 reddit-account-generator-1.1.0/reddit_account_generator/proxies.py
--rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-08-01 08:59:20.000000 reddit-account-generator-1.1.0/reddit_account_generator/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:59:31.883876 reddit-account-generator-1.1.0/reddit_account_generator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-08-01 08:59:31.000000 reddit-account-generator-1.1.0/reddit_account_generator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-08-01 08:59:31.000000 reddit-account-generator-1.1.0/reddit_account_generator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 08:59:31.000000 reddit-account-generator-1.1.0/reddit_account_generator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-08-01 08:59:31.000000 reddit-account-generator-1.1.0/reddit_account_generator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-01 08:59:31.000000 reddit-account-generator-1.1.0/reddit_account_generator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 08:59:31.883876 reddit-account-generator-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-08-01 08:59:20.000000 reddit-account-generator-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:24:32.504266 reddit-account-generator-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-08-07 10:24:20.000000 reddit-account-generator-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-08-07 10:24:32.504266 reddit-account-generator-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-08-07 10:24:20.000000 reddit-account-generator-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:24:32.500266 reddit-account-generator-1.1.1/reddit_account_generator/
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-08-07 10:24:20.000000 reddit-account-generator-1.1.1/reddit_account_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-07 10:24:20.000000 reddit-account-generator-1.1.1/reddit_account_generator/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-08-07 10:24:20.000000 reddit-account-generator-1.1.1/reddit_account_generator/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6310 2023-08-07 10:24:20.000000 reddit-account-generator-1.1.1/reddit_account_generator/maker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-08-07 10:24:20.000000 reddit-account-generator-1.1.1/reddit_account_generator/protector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-08-07 10:24:20.000000 reddit-account-generator-1.1.1/reddit_account_generator/proxies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-08-07 10:24:20.000000 reddit-account-generator-1.1.1/reddit_account_generator/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:24:32.500266 reddit-account-generator-1.1.1/reddit_account_generator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-08-07 10:24:32.000000 reddit-account-generator-1.1.1/reddit_account_generator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-08-07 10:24:32.000000 reddit-account-generator-1.1.1/reddit_account_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 10:24:32.000000 reddit-account-generator-1.1.1/reddit_account_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-08-07 10:24:32.000000 reddit-account-generator-1.1.1/reddit_account_generator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-07 10:24:32.000000 reddit-account-generator-1.1.1/reddit_account_generator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 10:24:32.504266 reddit-account-generator-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-08-07 10:24:20.000000 reddit-account-generator-1.1.1/setup.py
```

### Comparing `reddit-account-generator-1.1.0/LICENSE` & `reddit-account-generator-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `reddit-account-generator-1.1.0/PKG-INFO` & `reddit-account-generator-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reddit-account-generator
-Version: 1.1.0
+Version: 1.1.1
 Summary: Automatic reddit account generator on selenium.
 Home-page: https://github.com/cubicbyte/reddit-account-generator
 Author: cubicbyte
 Author-email: bmaruhnenko@gmail.com
 License: MIT
 Keywords: python reddit account-generator account-maker account-generation r-place rplace
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `reddit-account-generator-1.1.0/README.md` & `reddit-account-generator-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `reddit-account-generator-1.1.0/reddit_account_generator/__init__.py` & `reddit-account-generator-1.1.1/reddit_account_generator/__init__.py`

 * *Files identical despite different names*

### Comparing `reddit-account-generator-1.1.0/reddit_account_generator/exceptions.py` & `reddit-account-generator-1.1.1/reddit_account_generator/exceptions.py`

 * *Files identical despite different names*

### Comparing `reddit-account-generator-1.1.0/reddit_account_generator/maker.py` & `reddit-account-generator-1.1.1/reddit_account_generator/maker.py`

 * *Files identical despite different names*

### Comparing `reddit-account-generator-1.1.0/reddit_account_generator/protector.py` & `reddit-account-generator-1.1.1/reddit_account_generator/protector.py`

 * *Files identical despite different names*

### Comparing `reddit-account-generator-1.1.0/reddit_account_generator/proxies.py` & `reddit-account-generator-1.1.1/reddit_account_generator/proxies.py`

 * *Files identical despite different names*

### Comparing `reddit-account-generator-1.1.0/reddit_account_generator/utils.py` & `reddit-account-generator-1.1.1/reddit_account_generator/utils.py`

 * *Files identical despite different names*

### Comparing `reddit-account-generator-1.1.0/reddit_account_generator.egg-info/PKG-INFO` & `reddit-account-generator-1.1.1/reddit_account_generator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reddit-account-generator
-Version: 1.1.0
+Version: 1.1.1
 Summary: Automatic reddit account generator on selenium.
 Home-page: https://github.com/cubicbyte/reddit-account-generator
 Author: cubicbyte
 Author-email: bmaruhnenko@gmail.com
 License: MIT
 Keywords: python reddit account-generator account-maker account-generation r-place rplace
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `reddit-account-generator-1.1.0/reddit_account_generator.egg-info/SOURCES.txt` & `reddit-account-generator-1.1.1/reddit_account_generator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

