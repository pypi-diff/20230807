# Comparing `tmp/metapensiero.sphinx.patchdb-4.0.dev8.tar.gz` & `tmp/metapensiero.sphinx.patchdb-4.0.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metapensiero.sphinx.patchdb-4.0.dev8.tar", last modified: Thu Jul 27 16:34:16 2023, max compression
+gzip compressed data, was "metapensiero.sphinx.patchdb-4.0.dev9.tar", last modified: Fri Jul 28 08:20:21 2023, max compression
```

## Comparing `metapensiero.sphinx.patchdb-4.0.dev8.tar` & `metapensiero.sphinx.patchdb-4.0.dev9.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     4109 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/CHANGES.rst
--rw-r--r--   0        0        0      589 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/Makefile
--rw-r--r--   0        0        0    10656 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/OLDERCHANGES.rst
--rw-r--r--   0        0        0    31089 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/README.rst
--rw-r--r--   0        0        0     2006 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/flake.lock
--rw-r--r--   0        0        0     3760 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/flake.nix
--rw-r--r--   0        0        0     1745 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/pyproject.toml
--rw-r--r--   0        0        0      697 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/src/metapensiero/sphinx/patchdb/__init__.py
--rw-r--r--   0        0        0     7496 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/src/metapensiero/sphinx/patchdb/contexts/__init__.py
--rw-r--r--   0        0        0     3545 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/src/metapensiero/sphinx/patchdb/contexts/firebird.py
--rw-r--r--   0        0        0     4692 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/src/metapensiero/sphinx/patchdb/contexts/mysql.py
--rw-r--r--   0        0        0     4289 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/src/metapensiero/sphinx/patchdb/contexts/postgres.py
--rw-r--r--   0        0        0     1505 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/src/metapensiero/sphinx/patchdb/contexts/python.py
--rw-r--r--   0        0        0    17964 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/src/metapensiero/sphinx/patchdb/contexts/sql.py
--rw-r--r--   0        0        0     3858 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/src/metapensiero/sphinx/patchdb/contexts/sqlite.py
--rw-r--r--   0        0        0     1546 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/src/metapensiero/sphinx/patchdb/locale/__init__.py
--rw-r--r--   0        0        0    13092 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/src/metapensiero/sphinx/patchdb/locale/it/LC_MESSAGES/metapensiero-sphinx-patchdb.po
--rw-r--r--   0        0        0      285 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/src/metapensiero/sphinx/patchdb/locale/mapping.cfg
--rw-r--r--   0        0        0     8935 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/src/metapensiero/sphinx/patchdb/locale/metapensiero-sphinx-patchdb.pot
--rw-r--r--   0        0        0     4673 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/src/metapensiero/sphinx/patchdb/manager.py
--rw-r--r--   0        0        0    14064 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/src/metapensiero/sphinx/patchdb/patch.py
--rw-r--r--   0        0        0     9282 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/src/metapensiero/sphinx/patchdb/planner.py
--rw-r--r--   0        0        0     9175 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/src/metapensiero/sphinx/patchdb/pup.py
--rw-r--r--   0        0        0    24367 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/src/metapensiero/sphinx/patchdb/script.py
--rw-r--r--   0        0        0     7312 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/src/metapensiero/sphinx/patchdb/states.py
--rw-r--r--   0        0        0     8148 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/tests/fixtures.py
--rwxr-xr-x   0        0        0     1633 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/tests/postgresql
--rw-r--r--   0        0        0     7111 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/tests/test_bad.py
--rw-r--r--   0        0        0     4430 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/tests/test_drops.py
--rw-r--r--   0        0        0     1182 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/tests/test_external_file.py
--rw-r--r--   0        0        0     3557 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/tests/test_helpers.py
--rw-r--r--   0        0        0     1862 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/tests/test_manager.py
--rw-r--r--   0        0        0     2284 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/tests/test_modular.py
--rw-r--r--   0        0        0     3555 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/tests/test_patch.py
--rw-r--r--   0        0        0     8226 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/tests/test_planner.py
--rw-r--r--   0        0        0     2766 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/tests/test_python.py
--rw-r--r--   0        0        0     7007 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/tests/test_revisions.py
--rw-r--r--   0        0        0     4632 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/tests/test_sql.py
--rw-r--r--   0        0        0     2291 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/tests/test_sql_fb.py
--rw-r--r--   0        0        0     4328 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/tests/test_sql_ms.py
--rw-r--r--   0        0        0     7639 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/tests/test_sql_pg.py
--rw-r--r--   0        0        0     2835 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/tests/test_states.py
--rw-r--r--   0        0        0     2094 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/tests/test_variables.py
--rw-r--r--   0        0        0    32184 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/PKG-INFO
+-rw-r--r--   0        0        0     4222 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev9/CHANGES.rst
+-rw-r--r--   0        0        0      589 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev9/Makefile
+-rw-r--r--   0        0        0    10656 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev9/OLDERCHANGES.rst
+-rw-r--r--   0        0        0    31089 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev9/README.rst
+-rw-r--r--   0        0        0     2006 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev9/flake.lock
+-rw-r--r--   0        0        0     3760 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev9/flake.nix
+-rw-r--r--   0        0        0     1745 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev9/pyproject.toml
+-rw-r--r--   0        0        0      697 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev9/src/metapensiero/sphinx/patchdb/__init__.py
+-rw-r--r--   0        0        0     7496 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev9/src/metapensiero/sphinx/patchdb/contexts/__init__.py
+-rw-r--r--   0        0        0     3545 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev9/src/metapensiero/sphinx/patchdb/contexts/firebird.py
+-rw-r--r--   0        0        0     4692 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev9/src/metapensiero/sphinx/patchdb/contexts/mysql.py
+-rw-r--r--   0        0        0     4289 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev9/src/metapensiero/sphinx/patchdb/contexts/postgres.py
+-rw-r--r--   0        0        0     1505 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev9/src/metapensiero/sphinx/patchdb/contexts/python.py
+-rw-r--r--   0        0        0    17964 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev9/src/metapensiero/sphinx/patchdb/contexts/sql.py
+-rw-r--r--   0        0        0     3858 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev9/src/metapensiero/sphinx/patchdb/contexts/sqlite.py
+-rw-r--r--   0        0        0     1546 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev9/src/metapensiero/sphinx/patchdb/locale/__init__.py
+-rw-r--r--   0        0        0    13092 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev9/src/metapensiero/sphinx/patchdb/locale/it/LC_MESSAGES/metapensiero-sphinx-patchdb.po
+-rw-r--r--   0        0        0      285 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev9/src/metapensiero/sphinx/patchdb/locale/mapping.cfg
+-rw-r--r--   0        0        0     8935 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev9/src/metapensiero/sphinx/patchdb/locale/metapensiero-sphinx-patchdb.pot
+-rw-r--r--   0        0        0     4673 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev9/src/metapensiero/sphinx/patchdb/manager.py
+-rw-r--r--   0        0        0    14448 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev9/src/metapensiero/sphinx/patchdb/patch.py
+-rw-r--r--   0        0        0     9282 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev9/src/metapensiero/sphinx/patchdb/planner.py
+-rw-r--r--   0        0        0     9175 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev9/src/metapensiero/sphinx/patchdb/pup.py
+-rw-r--r--   0        0        0    24367 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev9/src/metapensiero/sphinx/patchdb/script.py
+-rw-r--r--   0        0        0     7312 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev9/src/metapensiero/sphinx/patchdb/states.py
+-rw-r--r--   0        0        0     8148 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev9/tests/fixtures.py
+-rwxr-xr-x   0        0        0     1633 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev9/tests/postgresql
+-rw-r--r--   0        0        0     7111 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev9/tests/test_bad.py
+-rw-r--r--   0        0        0     4430 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev9/tests/test_drops.py
+-rw-r--r--   0        0        0     1182 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev9/tests/test_external_file.py
+-rw-r--r--   0        0        0     3557 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev9/tests/test_helpers.py
+-rw-r--r--   0        0        0     1862 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev9/tests/test_manager.py
+-rw-r--r--   0        0        0     2284 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev9/tests/test_modular.py
+-rw-r--r--   0        0        0     3555 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev9/tests/test_patch.py
+-rw-r--r--   0        0        0     8226 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev9/tests/test_planner.py
+-rw-r--r--   0        0        0     2766 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev9/tests/test_python.py
+-rw-r--r--   0        0        0     7007 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev9/tests/test_revisions.py
+-rw-r--r--   0        0        0     4632 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev9/tests/test_sql.py
+-rw-r--r--   0        0        0     2291 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev9/tests/test_sql_fb.py
+-rw-r--r--   0        0        0     4328 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev9/tests/test_sql_ms.py
+-rw-r--r--   0        0        0     7639 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev9/tests/test_sql_pg.py
+-rw-r--r--   0        0        0     2835 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev9/tests/test_states.py
+-rw-r--r--   0        0        0     2094 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev9/tests/test_variables.py
+-rw-r--r--   0        0        0    32184 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev9/PKG-INFO
```

### Comparing `metapensiero.sphinx.patchdb-4.0.dev8/CHANGES.rst` & `metapensiero.sphinx.patchdb-4.0.dev9/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Changes\ [#]_
 -------------
 
+4.0.dev9 (2023-07-28)
+~~~~~~~~~~~~~~~~~~~~~
+
+* Adjust unspecified revisions also in the new `replaces` entries
+
+
 4.0.dev8 (2023-07-27)
 ~~~~~~~~~~~~~~~~~~~~~
 
 * Various fixes to the new ``Planner`` machinery
 
 * Add a new `replaces` option on the patches, as a better alternative to the kludge introduced
   in version 4.0.dev3.
```

### Comparing `metapensiero.sphinx.patchdb-4.0.dev8/Makefile` & `metapensiero.sphinx.patchdb-4.0.dev9/Makefile`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev8/OLDERCHANGES.rst` & `metapensiero.sphinx.patchdb-4.0.dev9/OLDERCHANGES.rst`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev8/README.rst` & `metapensiero.sphinx.patchdb-4.0.dev9/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -183,15 +183,18 @@
      :depends: Some function@1
      :brings: Some function@2
 
      DROP FUNCTION some_function(int, OUT int)
      ;;
      ;;INCLUDE: some_function.sql
 
-A particular case is when you actually need to *replace* something with something else, for example instead of upgrading the function above you want to replace it entirely. This is when the ``replaces`` option comes handy: it is almost equivalent to the ``depends`` option, except that it is not an error when an item specified with the former does not exist::
+A particular case is when you actually need to *replace* something with something else, for
+example instead of upgrading the function above you want to replace it entirely. This is when
+the ``replaces`` option comes handy: it is almost equivalent to the ``depends`` option, except
+that it is not an error when an item specified with the former does not exist::
 
   .. patchdb:script:: Some other function
      :file: some_other_function.sql
 
   .. patchdb:script:: Replace some function with a different one
      :replaces: Some function@1
      :brings: Some other function@1
```

### Comparing `metapensiero.sphinx.patchdb-4.0.dev8/flake.lock` & `metapensiero.sphinx.patchdb-4.0.dev9/flake.lock`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev8/flake.nix` & `metapensiero.sphinx.patchdb-4.0.dev9/flake.nix`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev8/pyproject.toml` & `metapensiero.sphinx.patchdb-4.0.dev9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "metapensiero.sphinx.patchdb"
 description = "Extract scripts from a reST document and apply them in order."
-version = "4.0.dev8"
+version = "4.0.dev9"
 authors = [
     { name = "Lele Gaifax", email = "lele@metapensiero.it" },
 ]
 readme = "README.rst"
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `metapensiero.sphinx.patchdb-4.0.dev8/src/metapensiero/sphinx/patchdb/__init__.py` & `metapensiero.sphinx.patchdb-4.0.dev9/src/metapensiero/sphinx/patchdb/__init__.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev8/src/metapensiero/sphinx/patchdb/contexts/__init__.py` & `metapensiero.sphinx.patchdb-4.0.dev9/src/metapensiero/sphinx/patchdb/contexts/__init__.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev8/src/metapensiero/sphinx/patchdb/contexts/firebird.py` & `metapensiero.sphinx.patchdb-4.0.dev9/src/metapensiero/sphinx/patchdb/contexts/firebird.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev8/src/metapensiero/sphinx/patchdb/contexts/mysql.py` & `metapensiero.sphinx.patchdb-4.0.dev9/src/metapensiero/sphinx/patchdb/contexts/mysql.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev8/src/metapensiero/sphinx/patchdb/contexts/postgres.py` & `metapensiero.sphinx.patchdb-4.0.dev9/src/metapensiero/sphinx/patchdb/contexts/postgres.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev8/src/metapensiero/sphinx/patchdb/contexts/python.py` & `metapensiero.sphinx.patchdb-4.0.dev9/src/metapensiero/sphinx/patchdb/contexts/python.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev8/src/metapensiero/sphinx/patchdb/contexts/sql.py` & `metapensiero.sphinx.patchdb-4.0.dev9/src/metapensiero/sphinx/patchdb/contexts/sql.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev8/src/metapensiero/sphinx/patchdb/contexts/sqlite.py` & `metapensiero.sphinx.patchdb-4.0.dev9/src/metapensiero/sphinx/patchdb/contexts/sqlite.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev8/src/metapensiero/sphinx/patchdb/locale/__init__.py` & `metapensiero.sphinx.patchdb-4.0.dev9/src/metapensiero/sphinx/patchdb/locale/__init__.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev8/src/metapensiero/sphinx/patchdb/locale/it/LC_MESSAGES/metapensiero-sphinx-patchdb.po` & `metapensiero.sphinx.patchdb-4.0.dev9/src/metapensiero/sphinx/patchdb/locale/it/LC_MESSAGES/metapensiero-sphinx-patchdb.po`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (C) 2016, 2017, 2019, 2021, 2022, 2023 Lele Gaifax
 # This file is distributed under the same license as the
 # metapensiero.sphinx.patchdb project.
 # Lele Gaifax <lele@metapensiero.it>, 2016.
 #
 msgid ""
 msgstr ""
-"Project-Id-Version: metapensiero.sphinx.patchdb 4.0.dev8\n"
+"Project-Id-Version: metapensiero.sphinx.patchdb 4.0.dev9\n"
 "Report-Msgid-Bugs-To: lele@metapensiero.it\n"
 "POT-Creation-Date: 2023-07-27 18:30+0200\n"
 "PO-Revision-Date: 2023-07-27 18:31+0200\n"
 "Last-Translator: Lele Gaifax <lele@metapensiero.it>\n"
 "Language: it\n"
 "Language-Team: it <lele@metapensiero.it>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `metapensiero.sphinx.patchdb-4.0.dev8/src/metapensiero/sphinx/patchdb/locale/metapensiero-sphinx-patchdb.pot` & `metapensiero.sphinx.patchdb-4.0.dev9/src/metapensiero/sphinx/patchdb/locale/metapensiero-sphinx-patchdb.pot`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the
 # metapensiero.sphinx.patchdb project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2023.
 #
 #, fuzzy
 msgid ""
 msgstr ""
-"Project-Id-Version: metapensiero.sphinx.patchdb 4.0.dev8\n"
+"Project-Id-Version: metapensiero.sphinx.patchdb 4.0.dev9\n"
 "Report-Msgid-Bugs-To: lele@metapensiero.it\n"
 "POT-Creation-Date: 2023-07-27 18:30+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `metapensiero.sphinx.patchdb-4.0.dev8/src/metapensiero/sphinx/patchdb/manager.py` & `metapensiero.sphinx.patchdb-4.0.dev9/src/metapensiero/sphinx/patchdb/manager.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev8/src/metapensiero/sphinx/patchdb/patch.py` & `metapensiero.sphinx.patchdb-4.0.dev9/src/metapensiero/sphinx/patchdb/patch.py`

 * *Files 3% similar despite different names*

```diff
@@ -189,15 +189,14 @@
         :returns: a `(bool, str)` tuple,, ``True`` when the patch must be retained, ``False``
                   to discard it and the reason
 
         Perform also some sanity checks: all `depends`, `brings` and `preceeds` must exist at
         this point.
         """
 
-        retain_reason = ''
         for i, (pid, rev) in enumerate(self.depends):
             p = pm[pid]
             if p is None:
                 reason = (f'defined in {self.source} at line {self.line}'
                           f' depends on non existing "{pid}@{rev}"')
                 if self.is_migration:
                     return False, reason
@@ -207,14 +206,19 @@
             elif rev == '*':
                 current_rev = context[pid]
                 if current_rev is None:
                     self.depends[i] = (pid, p.revision)
                 else:
                     self.depends[i] = (pid, current_rev)
 
+        for i, (pid, rev) in enumerate(self.replaces):
+            if rev is None or rev == '*':
+                rev = context[pid]
+                self.replaces[i] = (pid, rev)
+
         for i, (pid, rev) in enumerate(self.brings):
             p = pm[pid]
             if p is None:
                 reason = (f'defined in {self.source} at line {self.line},'
                           f' brings to non existing "{pid}@{rev}"')
                 return False, reason
             if rev is None:
@@ -225,17 +229,23 @@
             if p is None:
                 reason = (f'defined in {self.source} at line {self.line}'
                           f' preceeds on non existing "{pid}@{rev}"')
                 if self.is_migration:
                     return False, reason
                 raise DependencyError(f'{self} {reason}')
             if rev is None:
-                self.preceeds[i] = (pid, pm[pid].revision)
+                self.preceeds[i] = (pid, p.revision)
+            elif rev == '*':
+                current_rev = context[pid]
+                if current_rev is None:
+                    self.preceeds[i] = (pid, p.revision)
+                else:
+                    self.preceeds[i] = (pid, current_rev)
 
-        return True, retain_reason
+        return True, ''
 
     def beautify(self):
         "Compute a beautified and highlighted HTML version of the script."
 
         from pygments import highlight
         from pygments.lexers import get_lexer_by_name, get_lexer_for_mimetype
         from pygments.formatters import get_formatter_by_name
```

### Comparing `metapensiero.sphinx.patchdb-4.0.dev8/src/metapensiero/sphinx/patchdb/planner.py` & `metapensiero.sphinx.patchdb-4.0.dev9/src/metapensiero/sphinx/patchdb/planner.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev8/src/metapensiero/sphinx/patchdb/pup.py` & `metapensiero.sphinx.patchdb-4.0.dev9/src/metapensiero/sphinx/patchdb/pup.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev8/src/metapensiero/sphinx/patchdb/script.py` & `metapensiero.sphinx.patchdb-4.0.dev9/src/metapensiero/sphinx/patchdb/script.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev8/src/metapensiero/sphinx/patchdb/states.py` & `metapensiero.sphinx.patchdb-4.0.dev9/src/metapensiero/sphinx/patchdb/states.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev8/tests/fixtures.py` & `metapensiero.sphinx.patchdb-4.0.dev9/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev8/tests/postgresql` & `metapensiero.sphinx.patchdb-4.0.dev9/tests/postgresql`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev8/tests/test_bad.py` & `metapensiero.sphinx.patchdb-4.0.dev9/tests/test_bad.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev8/tests/test_drops.py` & `metapensiero.sphinx.patchdb-4.0.dev9/tests/test_drops.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev8/tests/test_external_file.py` & `metapensiero.sphinx.patchdb-4.0.dev9/tests/test_external_file.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev8/tests/test_helpers.py` & `metapensiero.sphinx.patchdb-4.0.dev9/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev8/tests/test_manager.py` & `metapensiero.sphinx.patchdb-4.0.dev9/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev8/tests/test_modular.py` & `metapensiero.sphinx.patchdb-4.0.dev9/tests/test_modular.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev8/tests/test_patch.py` & `metapensiero.sphinx.patchdb-4.0.dev9/tests/test_patch.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev8/tests/test_planner.py` & `metapensiero.sphinx.patchdb-4.0.dev9/tests/test_planner.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev8/tests/test_python.py` & `metapensiero.sphinx.patchdb-4.0.dev9/tests/test_python.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev8/tests/test_revisions.py` & `metapensiero.sphinx.patchdb-4.0.dev9/tests/test_revisions.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev8/tests/test_sql.py` & `metapensiero.sphinx.patchdb-4.0.dev9/tests/test_sql.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev8/tests/test_sql_fb.py` & `metapensiero.sphinx.patchdb-4.0.dev9/tests/test_sql_fb.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev8/tests/test_sql_ms.py` & `metapensiero.sphinx.patchdb-4.0.dev9/tests/test_sql_ms.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev8/tests/test_sql_pg.py` & `metapensiero.sphinx.patchdb-4.0.dev9/tests/test_sql_pg.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev8/tests/test_states.py` & `metapensiero.sphinx.patchdb-4.0.dev9/tests/test_states.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev8/tests/test_variables.py` & `metapensiero.sphinx.patchdb-4.0.dev9/tests/test_variables.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev8/PKG-INFO` & `metapensiero.sphinx.patchdb-4.0.dev9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metapensiero.sphinx.patchdb
-Version: 4.0.dev8
+Version: 4.0.dev9
 Summary: Extract scripts from a reST document and apply them in order.
 License: GPL-3.0-or-later
 Author-email: Lele Gaifax <lele@metapensiero.it>
 Requires-Python: >=3.10
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Framework :: Sphinx :: Extension
@@ -208,15 +208,18 @@
      :depends: Some function@1
      :brings: Some function@2
 
      DROP FUNCTION some_function(int, OUT int)
      ;;
      ;;INCLUDE: some_function.sql
 
-A particular case is when you actually need to *replace* something with something else, for example instead of upgrading the function above you want to replace it entirely. This is when the ``replaces`` option comes handy: it is almost equivalent to the ``depends`` option, except that it is not an error when an item specified with the former does not exist::
+A particular case is when you actually need to *replace* something with something else, for
+example instead of upgrading the function above you want to replace it entirely. This is when
+the ``replaces`` option comes handy: it is almost equivalent to the ``depends`` option, except
+that it is not an error when an item specified with the former does not exist::
 
   .. patchdb:script:: Some other function
      :file: some_other_function.sql
 
   .. patchdb:script:: Replace some function with a different one
      :replaces: Some function@1
      :brings: Some other function@1
```

