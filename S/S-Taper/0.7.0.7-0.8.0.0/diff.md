# Comparing `tmp/S_Taper-0.7.0.7.tar.gz` & `tmp/S_Taper-0.8.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "S_Taper-0.7.0.7.tar", last modified: Tue Dec 13 17:52:33 2022, max compression
+gzip compressed data, was "S_Taper-0.8.0.0.tar", last modified: Mon Aug  7 07:25:46 2023, max compression
```

## Comparing `S_Taper-0.7.0.7.tar` & `S_Taper-0.8.0.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2022-12-13 17:52:33.719799 S_Taper-0.7.0.7/
--rw-rw-rw-   0        0        0      662 2022-12-13 17:52:33.719799 S_Taper-0.7.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      215 2022-10-24 14:26:34.000000 S_Taper-0.7.0.7/README.md
-drwxrwxrwx   0        0        0        0 2022-12-13 17:52:33.713797 S_Taper-0.7.0.7/S_Taper.egg-info/
--rw-rw-rw-   0        0        0      662 2022-12-13 17:52:33.000000 S_Taper-0.7.0.7/S_Taper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2022-12-13 17:52:33.000000 S_Taper-0.7.0.7/S_Taper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-13 17:52:33.000000 S_Taper-0.7.0.7/S_Taper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2022-12-13 17:52:33.000000 S_Taper-0.7.0.7/S_Taper.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-12-13 17:52:33.717798 S_Taper-0.7.0.7/s_taper/
--rw-rw-rw-   0        0        0     3146 2022-12-13 17:52:20.000000 S_Taper-0.7.0.7/s_taper/__init__.py
--rw-rw-rw-   0        0        0       82 2022-12-13 17:52:20.000000 S_Taper-0.7.0.7/s_taper/consts.py
--rw-rw-rw-   0        0        0       42 2022-12-13 17:52:33.720799 S_Taper-0.7.0.7/setup.cfg
--rw-rw-rw-   0        0        0      655 2022-12-13 17:52:20.000000 S_Taper-0.7.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 07:25:46.768957 S_Taper-0.8.0.0/
+-rw-rw-rw-   0        0        0      662 2023-08-07 07:25:46.768957 S_Taper-0.8.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      215 2022-10-24 14:26:34.000000 S_Taper-0.8.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-08-07 07:25:46.764368 S_Taper-0.8.0.0/S_Taper.egg-info/
+-rw-rw-rw-   0        0        0      662 2023-08-07 07:25:46.000000 S_Taper-0.8.0.0/S_Taper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      205 2023-08-07 07:25:46.000000 S_Taper-0.8.0.0/S_Taper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 07:25:46.000000 S_Taper-0.8.0.0/S_Taper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-08-07 07:25:46.000000 S_Taper-0.8.0.0/S_Taper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-07 07:25:46.767394 S_Taper-0.8.0.0/s_taper/
+-rw-rw-rw-   0        0        0     3659 2023-08-07 07:23:55.000000 S_Taper-0.8.0.0/s_taper/__init__.py
+-rw-rw-rw-   0        0        0     4146 2023-08-07 07:23:55.000000 S_Taper-0.8.0.0/s_taper/aio.py
+-rw-rw-rw-   0        0        0       82 2022-12-13 17:52:20.000000 S_Taper-0.8.0.0/s_taper/consts.py
+-rw-rw-rw-   0        0        0       42 2023-08-07 07:25:46.769959 S_Taper-0.8.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      655 2023-08-07 07:23:55.000000 S_Taper-0.8.0.0/setup.py
```

### Comparing `S_Taper-0.7.0.7/PKG-INFO` & `S_Taper-0.8.0.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: S_Taper
-Version: 0.7.0.7
+Version: 0.8.0.0
 Summary: Simple write-read add-on to SQLite3
 Home-page: https://github.com/TheYoungEngineers/SulfTaper
 Author: Nikita_Khalitov
 Author-email: nik1020031.nik@gmail.com
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `S_Taper-0.7.0.7/S_Taper.egg-info/PKG-INFO` & `S_Taper-0.8.0.0/S_Taper.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: S-Taper
-Version: 0.7.0.7
+Version: 0.8.0.0
 Summary: Simple write-read add-on to SQLite3
 Home-page: https://github.com/TheYoungEngineers/SulfTaper
 Author: Nikita_Khalitov
 Author-email: nik1020031.nik@gmail.com
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `S_Taper-0.7.0.7/s_taper/__init__.py` & `S_Taper-0.8.0.0/s_taper/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 import sqlite3
 import s_taper.consts
+import s_taper.aio
 
 
 class Taper:
     """
         Main class. Its instances correspond to a single table in the database.
         Use:
         table1 = Taper("table_name", "file.db")
     """
+    class _Value:
+        def __init__(self):
+            pass
 
     def __init__(self, table_name: str, file_name: str):
         self._table_name: str = table_name
         self._file_name: str = file_name
+        self.obj = self._Value()
+        self._columns = {}
 
-    def write(self, table_name: str = None, values: list | tuple = None):
+    def write(self, values: list | tuple = None, table_name: str = None,):
         if table_name is None:
             table_name = self._table_name
         conn = sqlite3.connect(self._file_name)
         cur = conn.cursor()
         questions = "?"
         for x in range(len(values) - 1):
             questions += ", ?"
@@ -82,17 +88,34 @@
             if n != len(table):
                 task += ", "
             else:
                 task += ");"
         cur.execute(task)
         conn.commit()
         conn.close()
-        return Taper(table_name, self._file_name)
+
+        temp = Taper(table_name, self._file_name)
+        temp._columns = table
+        temp.__create_obj__()
+        return temp
 
     def pop_table(self, table_name: str = None):
         if not table_name:
             table_name = self._table_name
         conn = sqlite3.connect(self._file_name)
         cur = conn.cursor()
         cur.execute(f"DROP TABLE {table_name}")
         conn.commit()
         conn.close()
+
+    def __create_obj__(self):
+        for key in self._columns:
+            self.obj.__setattr__(key, None)
+
+    def execute(self, sql: str):
+        conn = sqlite3.connect(self._file_name)
+        cur = conn.cursor()
+        cur.execute(sql)
+        conn.commit()
+        conn.close()
+
+
```

### Comparing `S_Taper-0.7.0.7/setup.py` & `S_Taper-0.8.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
 	long_description = fh.read()
 
 setuptools.setup(
 	name='S_Taper',
-	version="0.7.0.7",
+	version="0.8.0.0",
 	author="Nikita_Khalitov",
 	author_email="nik1020031.nik@gmail.com",
 	description="Simple write-read add-on to SQLite3",
 	long_description=long_description,
 	long_description_content_type="text/markdown",
 	url="https://github.com/TheYoungEngineers/SulfTaper",
 	packages=setuptools.find_packages(),
```

