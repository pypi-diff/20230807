# Comparing `tmp/sqlite-s3-query-0.0.8.tar.gz` & `tmp/sqlite-s3-query-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/dituser/dev/sqlite-s3-query/dist/tmpdtf4xgdz/sqlite-s3-query-0.0.8.tar", last modified: Sat Aug 28 09:45:51 2021, max compression
+gzip compressed data, was "/Users/dituser/dev/sqlite-s3-query/dist/tmp0jiotzj4/sqlite-s3-query-0.0.9.tar", last modified: Sat Aug 28 14:52:18 2021, max compression
```

## Comparing `sqlite-s3-query-0.0.8.tar` & `sqlite-s3-query-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 dituser    (501) staff       (20)        0 2021-08-28 09:45:51.325960 sqlite-s3-query-0.0.8/
--rw-r--r--   0 dituser    (501) staff       (20)     1072 2021-08-14 05:30:31.000000 sqlite-s3-query-0.0.8/LICENSE
--rw-r--r--   0 dituser    (501) staff       (20)     4241 2021-08-28 09:45:51.325594 sqlite-s3-query-0.0.8/PKG-INFO
--rw-r--r--   0 dituser    (501) staff       (20)     3747 2021-08-28 07:08:48.000000 sqlite-s3-query-0.0.8/README.md
--rw-r--r--   0 dituser    (501) staff       (20)       38 2021-08-28 09:45:51.326082 sqlite-s3-query-0.0.8/setup.cfg
--rw-r--r--   0 dituser    (501) staff       (20)      766 2021-08-28 09:45:11.000000 sqlite-s3-query-0.0.8/setup.py
-drwxr-xr-x   0 dituser    (501) staff       (20)        0 2021-08-28 09:45:51.325096 sqlite-s3-query-0.0.8/sqlite_s3_query.egg-info/
--rw-r--r--   0 dituser    (501) staff       (20)     4241 2021-08-28 09:45:51.000000 sqlite-s3-query-0.0.8/sqlite_s3_query.egg-info/PKG-INFO
--rw-r--r--   0 dituser    (501) staff       (20)      239 2021-08-28 09:45:51.000000 sqlite-s3-query-0.0.8/sqlite_s3_query.egg-info/SOURCES.txt
--rw-r--r--   0 dituser    (501) staff       (20)        1 2021-08-28 09:45:51.000000 sqlite-s3-query-0.0.8/sqlite_s3_query.egg-info/dependency_links.txt
--rw-r--r--   0 dituser    (501) staff       (20)       14 2021-08-28 09:45:51.000000 sqlite-s3-query-0.0.8/sqlite_s3_query.egg-info/requires.txt
--rw-r--r--   0 dituser    (501) staff       (20)       16 2021-08-28 09:45:51.000000 sqlite-s3-query-0.0.8/sqlite_s3_query.egg-info/top_level.txt
--rw-r--r--   0 dituser    (501) staff       (20)     5682 2021-08-28 09:41:14.000000 sqlite-s3-query-0.0.8/sqlite_s3_query.py
+drwxr-xr-x   0 dituser    (501) staff       (20)        0 2021-08-28 14:52:18.129946 sqlite-s3-query-0.0.9/
+-rw-r--r--   0 dituser    (501) staff       (20)     1072 2021-08-14 05:30:31.000000 sqlite-s3-query-0.0.9/LICENSE
+-rw-r--r--   0 dituser    (501) staff       (20)     4537 2021-08-28 14:52:18.129495 sqlite-s3-query-0.0.9/PKG-INFO
+-rw-r--r--   0 dituser    (501) staff       (20)     4043 2021-08-28 14:48:31.000000 sqlite-s3-query-0.0.9/README.md
+-rw-r--r--   0 dituser    (501) staff       (20)       38 2021-08-28 14:52:18.130068 sqlite-s3-query-0.0.9/setup.cfg
+-rw-r--r--   0 dituser    (501) staff       (20)      766 2021-08-28 14:50:42.000000 sqlite-s3-query-0.0.9/setup.py
+drwxr-xr-x   0 dituser    (501) staff       (20)        0 2021-08-28 14:52:18.128988 sqlite-s3-query-0.0.9/sqlite_s3_query.egg-info/
+-rw-r--r--   0 dituser    (501) staff       (20)     4537 2021-08-28 14:52:18.000000 sqlite-s3-query-0.0.9/sqlite_s3_query.egg-info/PKG-INFO
+-rw-r--r--   0 dituser    (501) staff       (20)      239 2021-08-28 14:52:18.000000 sqlite-s3-query-0.0.9/sqlite_s3_query.egg-info/SOURCES.txt
+-rw-r--r--   0 dituser    (501) staff       (20)        1 2021-08-28 14:52:18.000000 sqlite-s3-query-0.0.9/sqlite_s3_query.egg-info/dependency_links.txt
+-rw-r--r--   0 dituser    (501) staff       (20)       14 2021-08-28 14:52:18.000000 sqlite-s3-query-0.0.9/sqlite_s3_query.egg-info/requires.txt
+-rw-r--r--   0 dituser    (501) staff       (20)       16 2021-08-28 14:52:18.000000 sqlite-s3-query-0.0.9/sqlite_s3_query.egg-info/top_level.txt
+-rw-r--r--   0 dituser    (501) staff       (20)    12116 2021-08-28 14:33:44.000000 sqlite-s3-query-0.0.9/sqlite_s3_query.py
```

### Comparing `sqlite-s3-query-0.0.8/LICENSE` & `sqlite-s3-query-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlite-s3-query-0.0.8/PKG-INFO` & `sqlite-s3-query-0.0.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlite-s3-query
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python context manager to query a SQLite file stored on S3
 Home-page: https://github.com/michalc/sqlite-s3-query
 Author: Michal Charemza
 Author-email: michal@charemza.name
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -24,21 +24,20 @@
 SQL statements that write to the database are not supported.
 
 Inspired by [phiresky's sql.js-httpvfs](https://github.com/phiresky/sql.js-httpvfs), and [dacort's Stack Overflow answer](https://stackoverflow.com/a/59434097/1319998).
 
 
 ## Installation
 
-sqlite-s3-query depends on [APSW](https://github.com/rogerbinns/apsw), which is not available on PyPI, but can be installed directly from GitHub.
-
 ```bash
 pip install sqlite_s3_query
-pip install https://github.com/rogerbinns/apsw/releases/download/3.36.0-r1/apsw-3.36.0-r1.zip --global-option=fetch --global-option=--version --global-option=3.36.0 --global-option=--all --global-option=build --global-option=--enable-all-extensions
 ```
 
+The libsqlite3 binary library is also required, but this is typically already installed on most systems.
+
 
 ## Usage
 
 ```python
 from sqlite_s3_query import sqlite_s3_query
 
 with sqlite_s3_query(url='https://my-bucket.s3.eu-west-2.amazonaws.com/my-db.sqlite') as query:
@@ -100,7 +99,26 @@
 )
 
 with query_my_db() as query:
     for row in query_my_db('SELECT * FROM my_table WHERE my_col = ?', params=('my-value',)):
         print(row)
 ```
 
+The location of the libsqlite3 can be changed by overriding the `get_libsqlite3` parameter.
+
+```python
+from functools import partial
+from sys import playform
+import httpx
+from sqlite_s3_query import sqlite_s3_query
+
+query_my_db = partial(sqlite_s3_query,
+    url='https://my-bucket.s3.eu-west-2.amazonaws.com/my-db.sqlite',
+    get_libsqlite3=lambda: cdll.LoadLibrary({'linux': 'libsqlite3.so', 'darwin': 'libsqlite3.dylib'}[platform])
+)
+
+with query_my_db() as query:
+    for row in query_my_db('SELECT * FROM my_table WHERE my_col = ?', params=('my-value',)):
+        print(row)
+```
+
+
```

### Comparing `sqlite-s3-query-0.0.8/README.md` & `sqlite-s3-query-0.0.9/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -8,21 +8,20 @@
 SQL statements that write to the database are not supported.
 
 Inspired by [phiresky's sql.js-httpvfs](https://github.com/phiresky/sql.js-httpvfs), and [dacort's Stack Overflow answer](https://stackoverflow.com/a/59434097/1319998).
 
 
 ## Installation
 
-sqlite-s3-query depends on [APSW](https://github.com/rogerbinns/apsw), which is not available on PyPI, but can be installed directly from GitHub.
-
 ```bash
 pip install sqlite_s3_query
-pip install https://github.com/rogerbinns/apsw/releases/download/3.36.0-r1/apsw-3.36.0-r1.zip --global-option=fetch --global-option=--version --global-option=3.36.0 --global-option=--all --global-option=build --global-option=--enable-all-extensions
 ```
 
+The libsqlite3 binary library is also required, but this is typically already installed on most systems.
+
 
 ## Usage
 
 ```python
 from sqlite_s3_query import sqlite_s3_query
 
 with sqlite_s3_query(url='https://my-bucket.s3.eu-west-2.amazonaws.com/my-db.sqlite') as query:
@@ -82,8 +81,26 @@
     url='https://my-bucket.s3.eu-west-2.amazonaws.com/my-db.sqlite',
     get_http_client=lambda: httpx.Client(),
 )
 
 with query_my_db() as query:
     for row in query_my_db('SELECT * FROM my_table WHERE my_col = ?', params=('my-value',)):
         print(row)
-```
+```
+
+The location of the libsqlite3 can be changed by overriding the `get_libsqlite3` parameter.
+
+```python
+from functools import partial
+from sys import playform
+import httpx
+from sqlite_s3_query import sqlite_s3_query
+
+query_my_db = partial(sqlite_s3_query,
+    url='https://my-bucket.s3.eu-west-2.amazonaws.com/my-db.sqlite',
+    get_libsqlite3=lambda: cdll.LoadLibrary({'linux': 'libsqlite3.so', 'darwin': 'libsqlite3.dylib'}[platform])
+)
+
+with query_my_db() as query:
+    for row in query_my_db('SELECT * FROM my_table WHERE my_col = ?', params=('my-value',)):
+        print(row)
+```
```

### Comparing `sqlite-s3-query-0.0.8/setup.py` & `sqlite-s3-query-0.0.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def long_description():
     with open('README.md', 'r') as file:
         return file.read()
 
 
 setuptools.setup(
     name='sqlite-s3-query',
-    version='0.0.8',
+    version='0.0.9',
     author='Michal Charemza',
     author_email='michal@charemza.name',
     description='Python context manager to query a SQLite file stored on S3',
     long_description=long_description(),
     long_description_content_type='text/markdown',
     url='https://github.com/michalc/sqlite-s3-query',
     classifiers=[
```

### Comparing `sqlite-s3-query-0.0.8/sqlite_s3_query.egg-info/PKG-INFO` & `sqlite-s3-query-0.0.9/sqlite_s3_query.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlite-s3-query
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python context manager to query a SQLite file stored on S3
 Home-page: https://github.com/michalc/sqlite-s3-query
 Author: Michal Charemza
 Author-email: michal@charemza.name
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -24,21 +24,20 @@
 SQL statements that write to the database are not supported.
 
 Inspired by [phiresky's sql.js-httpvfs](https://github.com/phiresky/sql.js-httpvfs), and [dacort's Stack Overflow answer](https://stackoverflow.com/a/59434097/1319998).
 
 
 ## Installation
 
-sqlite-s3-query depends on [APSW](https://github.com/rogerbinns/apsw), which is not available on PyPI, but can be installed directly from GitHub.
-
 ```bash
 pip install sqlite_s3_query
-pip install https://github.com/rogerbinns/apsw/releases/download/3.36.0-r1/apsw-3.36.0-r1.zip --global-option=fetch --global-option=--version --global-option=3.36.0 --global-option=--all --global-option=build --global-option=--enable-all-extensions
 ```
 
+The libsqlite3 binary library is also required, but this is typically already installed on most systems.
+
 
 ## Usage
 
 ```python
 from sqlite_s3_query import sqlite_s3_query
 
 with sqlite_s3_query(url='https://my-bucket.s3.eu-west-2.amazonaws.com/my-db.sqlite') as query:
@@ -100,7 +99,26 @@
 )
 
 with query_my_db() as query:
     for row in query_my_db('SELECT * FROM my_table WHERE my_col = ?', params=('my-value',)):
         print(row)
 ```
 
+The location of the libsqlite3 can be changed by overriding the `get_libsqlite3` parameter.
+
+```python
+from functools import partial
+from sys import playform
+import httpx
+from sqlite_s3_query import sqlite_s3_query
+
+query_my_db = partial(sqlite_s3_query,
+    url='https://my-bucket.s3.eu-west-2.amazonaws.com/my-db.sqlite',
+    get_libsqlite3=lambda: cdll.LoadLibrary({'linux': 'libsqlite3.so', 'darwin': 'libsqlite3.dylib'}[platform])
+)
+
+with query_my_db() as query:
+    for row in query_my_db('SELECT * FROM my_table WHERE my_col = ?', params=('my-value',)):
+        print(row)
+```
+
+
```

