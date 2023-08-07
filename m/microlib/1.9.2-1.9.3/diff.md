# Comparing `tmp/microlib-1.9.2.tar.gz` & `tmp/microlib-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microlib-1.9.2.tar", max compression
+gzip compressed data, was "microlib-1.9.3.tar", max compression
```

## Comparing `microlib-1.9.2.tar` & `microlib-1.9.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    35147 2022-08-03 05:23:10.040213 microlib-1.9.2/LICENSE
--rw-r--r--   0        0        0     1463 2022-08-03 05:23:10.040213 microlib-1.9.2/README.rst
--rw-r--r--   0        0        0     1354 2022-08-03 05:23:10.040213 microlib-1.9.2/microlib/__init__.py
--rw-r--r--   0        0        0     5687 2021-02-26 06:43:10.068487 microlib-1.9.2/microlib/configfile.py
--rw-r--r--   0        0        0        2 2021-02-16 13:49:32.838687 microlib-1.9.2/microlib/data/empty_default_config.json
--rw-r--r--   0        0        0        0 2021-02-16 13:47:24.891334 microlib-1.9.2/microlib/data/empty_default_config.toml
--rw-r--r--   0        0        0     1804 2022-08-03 05:23:10.040213 microlib-1.9.2/microlib/data/pyproject.toml
--rw-r--r--   0        0        0    14410 2021-08-27 12:54:07.844812 microlib-1.9.2/microlib/database.py
--rw-r--r--   0        0        0     4044 2022-08-03 05:23:10.040213 microlib-1.9.2/microlib/deprecation.py
--rw-r--r--   0        0        0      869 2020-11-12 17:28:53.484313 microlib-1.9.2/microlib/prefs.py
--rw-r--r--   0        0        0     7092 2021-08-31 04:56:57.961335 microlib-1.9.2/microlib/terminal.py
--rw-r--r--   0        0        0     2163 2022-08-03 05:23:10.040213 microlib-1.9.2/microlib/tools.py
--rw-r--r--   0        0        0     2377 2020-11-12 21:12:28.338575 microlib-1.9.2/microlib/xdict.py
--rw-r--r--   0        0        0     1812 2022-08-11 20:20:10.029349 microlib-1.9.2/pyproject.toml
--rw-r--r--   0        0        0     2414 2022-08-11 20:20:16.660411 microlib-1.9.2/setup.py
--rw-r--r--   0        0        0     2902 2022-08-11 20:20:16.660720 microlib-1.9.2/PKG-INFO
+-rw-r--r--   0        0        0     2066 2023-08-07 18:57:14.828127 microlib-1.9.3/CHANGELOG.rst
+-rw-r--r--   0        0        0    35147 2022-08-03 05:23:10.040213 microlib-1.9.3/LICENSE
+-rw-r--r--   0        0        0     1463 2022-08-03 05:23:10.040213 microlib-1.9.3/README.rst
+-rw-r--r--   0        0        0     1354 2022-08-03 05:23:10.040213 microlib-1.9.3/microlib/__init__.py
+-rw-r--r--   0        0        0     5687 2021-02-26 06:43:10.068487 microlib-1.9.3/microlib/configfile.py
+-rw-r--r--   0        0        0        2 2021-02-16 13:49:32.838687 microlib-1.9.3/microlib/data/empty_default_config.json
+-rw-r--r--   0        0        0        0 2021-02-16 13:47:24.891334 microlib-1.9.3/microlib/data/empty_default_config.toml
+-rw-r--r--   0        0        0     1804 2022-08-03 05:23:10.040213 microlib-1.9.3/microlib/data/pyproject.toml
+-rw-r--r--   0        0        0    14507 2023-08-07 18:44:48.131996 microlib-1.9.3/microlib/database.py
+-rw-r--r--   0        0        0     4044 2022-08-03 05:23:10.040213 microlib-1.9.3/microlib/deprecation.py
+-rw-r--r--   0        0        0      869 2020-11-12 17:28:53.484313 microlib-1.9.3/microlib/prefs.py
+-rw-r--r--   0        0        0     7092 2021-08-31 04:56:57.961335 microlib-1.9.3/microlib/terminal.py
+-rw-r--r--   0        0        0     2163 2022-08-03 05:23:10.040213 microlib-1.9.3/microlib/tools.py
+-rw-r--r--   0        0        0     2377 2020-11-12 21:12:28.338575 microlib-1.9.3/microlib/xdict.py
+-rw-r--r--   0        0        0     1812 2023-08-07 18:57:05.428177 microlib-1.9.3/pyproject.toml
+-rw-r--r--   0        0        0     2950 1970-01-01 00:00:00.000000 microlib-1.9.3/PKG-INFO
```

### Comparing `microlib-1.9.2/LICENSE` & `microlib-1.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `microlib-1.9.2/README.rst` & `microlib-1.9.3/README.rst`

 * *Files identical despite different names*

### Comparing `microlib-1.9.2/microlib/__init__.py` & `microlib-1.9.3/microlib/__init__.py`

 * *Files identical despite different names*

### Comparing `microlib-1.9.2/microlib/configfile.py` & `microlib-1.9.3/microlib/configfile.py`

 * *Files identical despite different names*

### Comparing `microlib-1.9.2/microlib/data/pyproject.toml` & `microlib-1.9.3/microlib/data/pyproject.toml`

 * *Files identical despite different names*

### Comparing `microlib-1.9.2/microlib/database.py` & `microlib-1.9.3/microlib/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,14 +68,15 @@
         return self.cursor
 
     def __exit__(self, exc_class, exc, traceback):
         if self.testing:
             self.conn.execute('ROLLBACK TO SAVEPOINT starttest;')
         else:
             self.conn.commit()
+        self.cursor.close()
         self.conn.close()
 
 
 class Operator:
     """
     A collection of shortcuts to execute commands on a sqlite3 db.
 
@@ -240,27 +241,28 @@
         return (titles, qmarks)
 
     def _content(self, rows):
         return rows
 
     def insert_rows(self, table_name, rows, col_titles=None):
         """Insert rows to the table."""
-        if col_titles is None:
-            col_titles = self.get_cols(table_name)
-        for row in rows:
-            if len(col_titles) != len(row):
-                data = [f"'{item}'" for item in row]
-                data = ', '.join(data)
-                raise ValueError(f'In database, {data} requires {len(row)} '
-                                 f'columns, but table {table_name} has only '
-                                 f'{len(col_titles)} columns.')
-        titles, qmarks = self._titles_and_qmarks(col_titles)
-        cmd = f'INSERT INTO {table_name}({titles}) VALUES({qmarks})'
-        content = self._content(rows)
-        self.cursor.executemany(cmd, content)
+        if rows:
+            if col_titles is None:
+                col_titles = self.get_cols(table_name)
+            for row in rows:
+                if len(col_titles) != len(row):
+                    data = [f"'{item}'" for item in row]
+                    data = ', '.join(data)
+                    raise ValueError(f'In database, {data} requires {len(row)}'
+                                     f' columns, but table {table_name} has '
+                                     f'only {len(col_titles)} columns.')
+            titles, qmarks = self._titles_and_qmarks(col_titles)
+            cmd = f'INSERT INTO {table_name}({titles}) VALUES({qmarks})'
+            content = self._content(rows)
+            self.cursor.executemany(cmd, content)
 
     def merge_tables(self, name1, name2):
         """Insert rows of table name1 table into name2."""
         if len(self.get_cols(name1)) != len(self.get_cols(name2)):
             raise ValueError(f'In database, cannot merge table {name1} into '
                              f'table {name2} because they have different '
                              f'numbers of columns ({self.get_cols(name1)} and '
```

### Comparing `microlib-1.9.2/microlib/deprecation.py` & `microlib-1.9.3/microlib/deprecation.py`

 * *Files identical despite different names*

### Comparing `microlib-1.9.2/microlib/prefs.py` & `microlib-1.9.3/microlib/prefs.py`

 * *Files identical despite different names*

### Comparing `microlib-1.9.2/microlib/terminal.py` & `microlib-1.9.3/microlib/terminal.py`

 * *Files identical despite different names*

### Comparing `microlib-1.9.2/microlib/tools.py` & `microlib-1.9.3/microlib/tools.py`

 * *Files identical despite different names*

### Comparing `microlib-1.9.2/microlib/xdict.py` & `microlib-1.9.3/microlib/xdict.py`

 * *Files identical despite different names*

### Comparing `microlib-1.9.2/pyproject.toml` & `microlib-1.9.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "microlib"
-version = "1.9.2"
+version = "1.9.3"
 description = "Collection of various useful tools."
 license = 'GPL-3.0-or-later'
 authors = ["Nicolas Hainaux <nh.techn@posteo.net>"]
 readme = 'README.rst'
 repository = 'https://gitlab.com/nicolas.hainaux/microlib'
 classifiers = ['Development Status :: 5 - Production/Stable',
                'Natural Language :: English',
```

### Comparing `microlib-1.9.2/PKG-INFO` & `microlib-1.9.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microlib
-Version: 1.9.2
+Version: 1.9.3
 Summary: Collection of various useful tools.
 Home-page: https://gitlab.com/nicolas.hainaux/microlib
 License: GPL-3.0-or-later
 Author: Nicolas Hainaux
 Author-email: nh.techn@posteo.net
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,23 +13,24 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: BSD :: FreeBSD
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
 Requires-Dist: blessed (>=1.18.1,<2.0.0)
 Requires-Dist: click (>=8.0.1,<9.0.0)
-Requires-Dist: importlib-metadata (>=3.1,<5.0); python_full_version >= "3.7.0" and python_full_version < "3.8.0"
+Requires-Dist: importlib-metadata (>=3.1,<5.0) ; python_version >= "3.7.dev0" and python_version < "3.8.dev0"
 Requires-Dist: intspan (>=1.6.1,<2.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Project-URL: Repository, https://gitlab.com/nicolas.hainaux/microlib
 Description-Content-Type: text/x-rst
 
 |coveralls|
```

