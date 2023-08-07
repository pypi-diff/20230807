# Comparing `tmp/SQLAlchemyExample-0.1.5.tar.gz` & `tmp/SQLAlchemyExample-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SQLAlchemyExample-0.1.5.tar", last modified: Sat Aug  5 23:02:22 2023, max compression
+gzip compressed data, was "SQLAlchemyExample-0.1.6.tar", last modified: Mon Aug  7 21:42:03 2023, max compression
```

## Comparing `SQLAlchemyExample-0.1.5.tar` & `SQLAlchemyExample-0.1.6.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 23:02:22.034472 SQLAlchemyExample-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-08-05 23:02:12.000000 SQLAlchemyExample-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-08-05 23:02:12.000000 SQLAlchemyExample-0.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-08-05 23:02:22.034472 SQLAlchemyExample-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-08-05 23:02:12.000000 SQLAlchemyExample-0.1.5/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-08-05 23:02:12.000000 SQLAlchemyExample-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-08-05 23:02:12.000000 SQLAlchemyExample-0.1.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-08-05 23:02:22.034472 SQLAlchemyExample-0.1.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 23:02:22.034472 SQLAlchemyExample-0.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 23:02:22.034472 SQLAlchemyExample-0.1.5/src/SQLAlchemyExample.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-08-05 23:02:22.000000 SQLAlchemyExample-0.1.5/src/SQLAlchemyExample.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-08-05 23:02:22.000000 SQLAlchemyExample-0.1.5/src/SQLAlchemyExample.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 23:02:22.000000 SQLAlchemyExample-0.1.5/src/SQLAlchemyExample.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-05 23:02:22.000000 SQLAlchemyExample-0.1.5/src/SQLAlchemyExample.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 23:02:22.000000 SQLAlchemyExample-0.1.5/src/SQLAlchemyExample.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 23:02:22.034472 SQLAlchemyExample-0.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-08-05 23:02:12.000000 SQLAlchemyExample-0.1.5/tests/test_ex01_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-08-05 23:02:12.000000 SQLAlchemyExample-0.1.5/tests/test_ex02_otm_bi_single_table_inherit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-08-05 23:02:12.000000 SQLAlchemyExample-0.1.5/tests/test_ex03_otm_uni_single_table_inherit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:42:03.123328 SQLAlchemyExample-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-08-07 21:41:52.000000 SQLAlchemyExample-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-08-07 21:41:52.000000 SQLAlchemyExample-0.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-08-07 21:42:03.123328 SQLAlchemyExample-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-08-07 21:41:52.000000 SQLAlchemyExample-0.1.6/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-08-07 21:41:52.000000 SQLAlchemyExample-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-08-07 21:41:52.000000 SQLAlchemyExample-0.1.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-08-07 21:42:03.123328 SQLAlchemyExample-0.1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:42:03.119328 SQLAlchemyExample-0.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:42:03.123328 SQLAlchemyExample-0.1.6/src/SQLAlchemyExample.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-08-07 21:42:03.000000 SQLAlchemyExample-0.1.6/src/SQLAlchemyExample.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-08-07 21:42:03.000000 SQLAlchemyExample-0.1.6/src/SQLAlchemyExample.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 21:42:03.000000 SQLAlchemyExample-0.1.6/src/SQLAlchemyExample.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-07 21:42:03.000000 SQLAlchemyExample-0.1.6/src/SQLAlchemyExample.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 21:42:03.000000 SQLAlchemyExample-0.1.6/src/SQLAlchemyExample.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:42:03.123328 SQLAlchemyExample-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6868 2023-08-07 21:41:52.000000 SQLAlchemyExample-0.1.6/tests/test_otm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-08-07 21:41:52.000000 SQLAlchemyExample-0.1.6/tests/test_otm_sti.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-08-07 21:41:52.000000 SQLAlchemyExample-0.1.6/tests/test_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-08-07 21:41:52.000000 SQLAlchemyExample-0.1.6/tests/test_sti.py
```

### Comparing `SQLAlchemyExample-0.1.5/LICENSE` & `SQLAlchemyExample-0.1.6/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 MIT License
 
 Copyright (c) [year] [fullname]
 
-Permission is hereby granted, free of charge, to any person obtaining a copy
+Permission is hereby granted, free of charge, to any Student obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
+copies of the Software, and to permit Students to whom the Software is
 furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all
 copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
```

### Comparing `SQLAlchemyExample-0.1.5/PKG-INFO` & `SQLAlchemyExample-0.1.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SQLAlchemyExample
-Version: 0.1.5
+Version: 0.1.6
 Summary: Exploring SQLAlchemy
 Author: Hendrik du Toit
 Author-email: hendrik@brightedge.co.za
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: Topic :: Database
@@ -135,7 +135,15 @@
 :Status: Work In Progress
 
 .. Information about the project's license.
 
 Contact
 -------
 :Status: Work In Progress
+
+
+ToDo
+----
+
+1. Documentation - Add naming conventions
+    1. Tables
+    2. Table module definitions
```

### Comparing `SQLAlchemyExample-0.1.5/README.rst` & `SQLAlchemyExample-0.1.6/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -117,7 +117,15 @@
 :Status: Work In Progress
 
 .. Information about the project's license.
 
 Contact
 -------
 :Status: Work In Progress
+
+
+ToDo
+----
+
+1. Documentation - Add naming conventions
+    1. Tables
+    2. Table module definitions
```

### Comparing `SQLAlchemyExample-0.1.5/pyproject.toml` & `SQLAlchemyExample-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,14 @@
 
 [tool.black]
 skip-string-normalization = true
 extend-exclude = "/templates"
 
 
 [tool.pytest.ini_options]
-#addopts = ["--import-mode=importlib", '-v', '--ignore-glob=*\Archive', '--cov-report=html']
-addopts = ["--import-mode=importlib", '-v', '--cov=./', '--ignore-glob=*\Archive', '--cov-report=html']
+addopts = ["--import-mode=importlib", '-v', '--ignore-glob=*\Archive', '--cov-report=html']
+#addopts = ["--import-mode=importlib", '-v', '--cov=./', '--ignore-glob=*\Archive', '--cov-report=html']
 #pythonpath = ["src", "tests" ]
 markers = [
     'select: Run a selection of tests',
     'otmuni: One-To-Manu Uni-direction'
 ]
```

### Comparing `SQLAlchemyExample-0.1.5/requirements.txt` & `SQLAlchemyExample-0.1.6/requirements.txt`

 * *Files identical despite different names*

### Comparing `SQLAlchemyExample-0.1.5/setup.cfg` & `SQLAlchemyExample-0.1.6/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = SQLAlchemyExample
-version = 0.1.5
+version = 0.1.6
 author = Hendrik du Toit
 author_email = hendrik@brightedge.co.za
 description = Exploring SQLAlchemy
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 classifiers = 
 	Development Status :: 4 - Beta
@@ -30,13 +30,13 @@
 [options.packages.find]
 where = src
 
 [flake8]
 exclude = __init__.py, VersionArchive/, Archive/
 max-line-length = 88
 select = C,E,F,W,B,B950
-extend-ignore = E203, E501
+extend-ignore = E203, E501, W503
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `SQLAlchemyExample-0.1.5/src/SQLAlchemyExample.egg-info/PKG-INFO` & `SQLAlchemyExample-0.1.6/src/SQLAlchemyExample.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SQLAlchemyExample
-Version: 0.1.5
+Version: 0.1.6
 Summary: Exploring SQLAlchemy
 Author: Hendrik du Toit
 Author-email: hendrik@brightedge.co.za
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: Topic :: Database
@@ -135,7 +135,15 @@
 :Status: Work In Progress
 
 .. Information about the project's license.
 
 Contact
 -------
 :Status: Work In Progress
+
+
+ToDo
+----
+
+1. Documentation - Add naming conventions
+    1. Tables
+    2. Table module definitions
```

### Comparing `SQLAlchemyExample-0.1.5/tests/test_ex01_simple.py` & `SQLAlchemyExample-0.1.6/tests/test_simple.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,57 +4,57 @@
 
 
 class TestSimple:
     def test_table_exist(self, setup_db_simple):
         engine, session, base = setup_db_simple
         inspector = inspect(engine)
 
-        assert 'person' in inspector.get_table_names()
+        assert 'Student' in inspector.get_table_names()
         pass
 
-    def test_person_table_deletion(self, setup_db_simple):
+    def test_Student_table_deletion(self, setup_db_simple):
         engine, session, base = setup_db_simple
-        base.metadata.tables[f'{environ.get("MYSQL_DB_NAME")}.person'].drop()
+        base.metadata.tables[f'{environ.get("MYSQL_DB_NAME")}.Student'].drop()
         inspector = inspect(engine)
 
-        assert 'person' not in inspector.get_table_names()
+        assert 'Student' not in inspector.get_table_names()
         pass
 
     @pytest.mark.select
-    def test_person_assign_data(self, setup_db_simple):
+    def test_Student_assign_data(self, setup_db_simple):
         engine, session, base = setup_db_simple
-        import ex01_00_simple as tab_cfg
+        import simple as tab_cfg
 
-        person_list = [
-            tab_cfg.Person(name='John Doe'),
-            tab_cfg.Person(name='Jane Smith'),
+        Student_list = [
+            tab_cfg.Student(name='Ford Prefect'),
+            tab_cfg.Student(name='Arthur Dent'),
         ]
-        session.add_all(person_list)
+        session.add_all(Student_list)
         session.commit()
 
-        qry = session.query(tab_cfg.Person).all()
+        qry = session.query(tab_cfg.Student).all()
         assert len(qry) > 0
         for i, x in enumerate(qry):
-            assert x.name == person_list[i].name
+            assert x.name == Student_list[i].name
             pass
         pass
 
     @pytest.mark.select
-    def test_person_table_dunder_repr_ok(self, setup_db_simple):
+    def test_Student_table_dunder_repr_ok(self, setup_db_simple):
         engine, session, base = setup_db_simple
-        import ex01_00_simple as tab_cfg
+        import simple as tab_cfg
 
-        person = tab_cfg.Person(name='John')
-        session.add_all([person])
+        Student = tab_cfg.Student(name='John')
+        session.add_all([Student])
         session.commit()
 
-        assert repr(person) == '<Person(id=1 name=John)>'
+        assert repr(Student) == '<Student(id=1 name=John)>'
         pass
 
     @pytest.mark.select
-    def test_person_table_dunder_str_ok(self, setup_db_simple):
-        import ex01_00_simple as tab_cfg
+    def test_Student_table_dunder_str_ok(self, setup_db_simple):
+        import simple as tab_cfg
 
-        person = tab_cfg.Person(name='John')
+        Student = tab_cfg.Student(name='John')
 
-        assert str(person) == 'John'
+        assert str(Student) == 'John'
         pass
```

