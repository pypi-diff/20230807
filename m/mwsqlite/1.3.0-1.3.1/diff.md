# Comparing `tmp/mwsqlite-1.3.0.tar.gz` & `tmp/mwsqlite-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mwsqlite-1.3.0.tar", last modified: Mon Jul 24 08:45:01 2023, max compression
+gzip compressed data, was "dist\mwsqlite-1.3.1.tar", last modified: Mon Aug  7 07:48:47 2023, max compression
```

## Comparing `mwsqlite-1.3.0.tar` & `mwsqlite-1.3.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 08:45:01.933732 mwsqlite-1.3.0/
--rw-rw-rw-   0        0        0     1088 2022-10-20 18:54:22.000000 mwsqlite-1.3.0/LICENSE
--rw-rw-rw-   0        0        0     3172 2023-07-24 08:45:01.934733 mwsqlite-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     2075 2022-12-19 15:39:05.000000 mwsqlite-1.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-24 08:45:01.911728 mwsqlite-1.3.0/mwsqlite/
--rw-rw-rw-   0        0        0      209 2023-07-24 07:45:57.000000 mwsqlite-1.3.0/mwsqlite/__init__.py
--rw-rw-rw-   0        0        0     2405 2023-07-24 07:30:17.000000 mwsqlite-1.3.0/mwsqlite/_types.py
--rw-rw-rw-   0        0        0    14212 2023-07-24 07:45:25.000000 mwsqlite-1.3.0/mwsqlite/mw_sql.py
--rw-rw-rw-   0        0        0     3388 2022-12-23 15:06:08.000000 mwsqlite-1.3.0/mwsqlite/sql_compile.py
--rw-rw-rw-   0        0        0      551 2022-12-23 17:48:26.000000 mwsqlite-1.3.0/mwsqlite/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-24 08:45:01.932732 mwsqlite-1.3.0/mwsqlite.egg-info/
--rw-rw-rw-   0        0        0     3172 2023-07-24 08:45:01.000000 mwsqlite-1.3.0/mwsqlite.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      296 2023-07-24 08:45:01.000000 mwsqlite-1.3.0/mwsqlite.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 08:45:01.000000 mwsqlite-1.3.0/mwsqlite.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-24 08:45:01.000000 mwsqlite-1.3.0/mwsqlite.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        9 2023-07-24 08:45:01.000000 mwsqlite-1.3.0/mwsqlite.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-24 08:45:01.939734 mwsqlite-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1666 2023-07-24 07:46:27.000000 mwsqlite-1.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 07:48:47.161738 mwsqlite-1.3.1/
+-rw-rw-rw-   0        0        0     1088 2022-10-20 18:54:22.000000 mwsqlite-1.3.1/LICENSE
+-rw-rw-rw-   0        0        0     3172 2023-08-07 07:48:47.162738 mwsqlite-1.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2075 2022-12-19 15:39:05.000000 mwsqlite-1.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-08-07 07:48:47.145946 mwsqlite-1.3.1/mwsqlite/
+-rw-rw-rw-   0        0        0      209 2023-07-24 07:45:57.000000 mwsqlite-1.3.1/mwsqlite/__init__.py
+-rw-rw-rw-   0        0        0     2405 2023-07-24 07:30:17.000000 mwsqlite-1.3.1/mwsqlite/_types.py
+-rw-rw-rw-   0        0        0    14205 2023-08-07 07:41:02.000000 mwsqlite-1.3.1/mwsqlite/mw_sql.py
+-rw-rw-rw-   0        0        0     3610 2023-08-07 07:44:18.000000 mwsqlite-1.3.1/mwsqlite/sql_compile.py
+-rw-rw-rw-   0        0        0      551 2022-12-23 17:48:26.000000 mwsqlite-1.3.1/mwsqlite/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-07 07:48:47.160738 mwsqlite-1.3.1/mwsqlite.egg-info/
+-rw-rw-rw-   0        0        0     3172 2023-08-07 07:48:46.000000 mwsqlite-1.3.1/mwsqlite.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      296 2023-08-07 07:48:47.000000 mwsqlite-1.3.1/mwsqlite.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 07:48:46.000000 mwsqlite-1.3.1/mwsqlite.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-08-07 07:48:46.000000 mwsqlite-1.3.1/mwsqlite.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        9 2023-08-07 07:48:46.000000 mwsqlite-1.3.1/mwsqlite.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-07 07:48:47.164274 mwsqlite-1.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1666 2023-08-07 07:48:24.000000 mwsqlite-1.3.1/setup.py
```

### Comparing `mwsqlite-1.3.0/LICENSE` & `mwsqlite-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mwsqlite-1.3.0/PKG-INFO` & `mwsqlite-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: mwsqlite
-Version: 1.3.0
+Version: 1.3.1
 Summary: Simply python library for interact with (EOSIO) WAX blockchain
 Home-page: https://github.com/makarworld/mwsqlite.git
-Download-URL: https://github.com/makarworld/mwsqlite/archive/refs/tags/v1.3.0.zip
+Download-URL: https://github.com/makarworld/mwsqlite/archive/refs/tags/v1.3.1.zip
 Author: abuztrade
 Author-email: abuztrade.work@gmail.com
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Communications :: Email
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mwsqlite-1.3.0/README.md` & `mwsqlite-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `mwsqlite-1.3.0/mwsqlite/_types.py` & `mwsqlite-1.3.1/mwsqlite/_types.py`

 * *Files identical despite different names*

### Comparing `mwsqlite-1.3.0/mwsqlite/mw_sql.py` & `mwsqlite-1.3.1/mwsqlite/mw_sql.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         self.tables = tables
         self.ensure_connection = ensure_connection
 
         for table in self.tables:
             if "id" in self.tables[table].keys():
                 raise Exception("You can't use 'id' as column name")
 
-            cmd = SQLCompile.create(table, self.tables[table].keys())
+            cmd = SQLCompile.create(table, self.tables[table])
             cursor.execute(cmd)
 
             self.__setattr__(table, Table(table, self.tables[table], self))
 
     def table(self, table: str) -> Table:
         """
         Get table object.
```

### Comparing `mwsqlite-1.3.0/mwsqlite/sql_compile.py` & `mwsqlite-1.3.1/mwsqlite/sql_compile.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,21 +30,30 @@
             table=table, fields=fields, where=where)
     
     @staticmethod
     def delete(table, where):
         return SQLRequest.DELETE.format(
             table=table, where=where)
 
+types_dict = {
+    str: 'TEXT',
+    int: 'INTEGER',
+    float: 'REAL',
+    bool: 'TEXT',
+    list: 'TEXT',
+    dict: 'TEXT',
+}
+
 class SQLCompile:
     @staticmethod
-    def create(table: str, fields: list):
-        # fields = ["name", "age", ...]
+    def create(table: str, fields: dict):
+        # fields = {"name": str, "age": int, ...}
         cmd = SQLRequest.create(
             table = table, 
-            fields = ' TEXT, '.join(fields) + ' TEXT'
+            fields = ', '.join([f"{k} {types_dict.get(v, 'TEXT')}" for k, v in fields.items()])#' TEXT, '.join(fields) + ' TEXT'
         )
 
         return cmd
 
     @staticmethod
     def insert(table: str, fields: list):
         cmd = SQLRequest.insert(
```

### Comparing `mwsqlite-1.3.0/mwsqlite/utils.py` & `mwsqlite-1.3.1/mwsqlite/utils.py`

 * *Files identical despite different names*

### Comparing `mwsqlite-1.3.0/mwsqlite.egg-info/PKG-INFO` & `mwsqlite-1.3.1/mwsqlite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: mwsqlite
-Version: 1.3.0
+Version: 1.3.1
 Summary: Simply python library for interact with (EOSIO) WAX blockchain
 Home-page: https://github.com/makarworld/mwsqlite.git
-Download-URL: https://github.com/makarworld/mwsqlite/archive/refs/tags/v1.3.0.zip
+Download-URL: https://github.com/makarworld/mwsqlite/archive/refs/tags/v1.3.1.zip
 Author: abuztrade
 Author-email: abuztrade.work@gmail.com
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Communications :: Email
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mwsqlite-1.3.0/setup.py` & `mwsqlite-1.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 :author: abuztrade
 :license: MIT License, see LICENSE file.
 :copyright: (c) 2022 by abuztrade.
 """
 
 
-version = '1.3.0'
+version = '1.3.1'
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="mwsqlite",
     version=version,
```

