# Comparing `tmp/bSuite-python-1.1.3.tar.gz` & `tmp/bSuite-python-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bSuite-python-1.1.3.tar", last modified: Fri Jul  7 21:12:42 2023, max compression
+gzip compressed data, was "bSuite-python-2.0.0.tar", last modified: Mon Aug  7 17:15:39 2023, max compression
```

## Comparing `bSuite-python-1.1.3.tar` & `bSuite-python-2.0.0.tar`

### file list

```diff
@@ -1,31 +1,71 @@
-drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-07-07 21:12:42.783470 bSuite-python-1.1.3/
--rw-r--r--   0 birdwell   (501) staff       (20)    35148 2023-07-05 15:31:16.000000 bSuite-python-1.1.3/LICENSE
--rw-r--r--   0 birdwell   (501) staff       (20)    40984 2023-07-07 21:12:42.783277 bSuite-python-1.1.3/PKG-INFO
--rw-r--r--   0 birdwell   (501) staff       (20)       16 2023-07-05 15:45:08.000000 bSuite-python-1.1.3/README.md
-drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-07-07 21:12:42.775058 bSuite-python-1.1.3/bSuite_configure/
--rw-r--r--   0 birdwell   (501) staff       (20)    35148 2023-07-05 15:31:16.000000 bSuite-python-1.1.3/bSuite_configure/LICENSE
--rw-r--r--   0 birdwell   (501) staff       (20)      372 2023-07-05 02:23:50.000000 bSuite-python-1.1.3/bSuite_configure/pyproject.toml
-drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-07-07 21:12:42.773492 bSuite-python-1.1.3/bSuite_configure/src/
-drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-07-07 21:12:42.773534 bSuite-python-1.1.3/bSuite_configure/src/bSuite/
-drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-07-07 21:12:42.775768 bSuite-python-1.1.3/bSuite_configure/src/bSuite/configure/
--rw-r--r--   0 birdwell   (501) staff       (20)       52 2023-07-05 01:59:36.000000 bSuite-python-1.1.3/bSuite_configure/src/bSuite/configure/__init__.py
--rw-r--r--   0 birdwell   (501) staff       (20)     1233 2023-07-05 01:05:11.000000 bSuite-python-1.1.3/bSuite_configure/src/bSuite/configure/configure.py
-drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-07-07 21:12:42.776261 bSuite-python-1.1.3/bSuite_database/
--rw-r--r--   0 birdwell   (501) staff       (20)    35148 2023-07-05 15:31:16.000000 bSuite-python-1.1.3/bSuite_database/LICENSE
--rw-r--r--   0 birdwell   (501) staff       (20)      490 2023-07-05 02:26:14.000000 bSuite-python-1.1.3/bSuite_database/pyproject.toml
-drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-07-07 21:12:42.773698 bSuite-python-1.1.3/bSuite_database/src/
-drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-07-07 21:12:42.773740 bSuite-python-1.1.3/bSuite_database/src/bSuite/
-drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-07-07 21:12:42.777390 bSuite-python-1.1.3/bSuite_database/src/bSuite/database/
--rw-r--r--   0 birdwell   (501) staff       (20)      112 2023-07-04 23:38:47.000000 bSuite-python-1.1.3/bSuite_database/src/bSuite/database/__init__.py
--rw-r--r--   0 birdwell   (501) staff       (20)     8010 2023-07-07 21:11:43.000000 bSuite-python-1.1.3/bSuite_database/src/bSuite/database/base.py
--rw-r--r--   0 birdwell   (501) staff       (20)     2851 2023-07-06 00:12:17.000000 bSuite-python-1.1.3/bSuite_database/src/bSuite/database/crypto.py
--rw-r--r--   0 birdwell   (501) staff       (20)     2629 2023-07-07 20:26:55.000000 bSuite-python-1.1.3/bSuite_database/src/bSuite/database/mapped.py
-drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-07-07 21:12:42.782967 bSuite-python-1.1.3/bSuite_python.egg-info/
--rw-r--r--   0 birdwell   (501) staff       (20)    40984 2023-07-07 21:12:42.000000 bSuite-python-1.1.3/bSuite_python.egg-info/PKG-INFO
--rw-r--r--   0 birdwell   (501) staff       (20)      622 2023-07-07 21:12:42.000000 bSuite-python-1.1.3/bSuite_python.egg-info/SOURCES.txt
--rw-r--r--   0 birdwell   (501) staff       (20)        1 2023-07-07 21:12:42.000000 bSuite-python-1.1.3/bSuite_python.egg-info/dependency_links.txt
--rw-r--r--   0 birdwell   (501) staff       (20)       39 2023-07-07 21:12:42.000000 bSuite-python-1.1.3/bSuite_python.egg-info/requires.txt
--rw-r--r--   0 birdwell   (501) staff       (20)        7 2023-07-07 21:12:42.000000 bSuite-python-1.1.3/bSuite_python.egg-info/top_level.txt
--rw-r--r--   0 birdwell   (501) staff       (20)      788 2023-07-07 21:12:34.000000 bSuite-python-1.1.3/pyproject.toml
--rw-r--r--   0 birdwell   (501) staff       (20)       38 2023-07-07 21:12:42.783510 bSuite-python-1.1.3/setup.cfg
--rw-r--r--   0 birdwell   (501) staff       (20)       39 2023-07-05 00:44:00.000000 bSuite-python-1.1.3/setup.py
+drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-08-07 17:15:39.780163 bSuite-python-2.0.0/
+-rw-r--r--   0 birdwell   (501) staff       (20)    35148 2023-07-05 15:31:16.000000 bSuite-python-2.0.0/LICENSE
+-rw-r--r--   0 birdwell   (501) staff       (20)    40971 2023-08-07 17:15:39.779961 bSuite-python-2.0.0/PKG-INFO
+-rw-r--r--   0 birdwell   (501) staff       (20)       16 2023-07-05 15:45:08.000000 bSuite-python-2.0.0/README.md
+drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-08-07 17:15:39.765891 bSuite-python-2.0.0/bSuite_auth/
+-rw-r--r--   0 birdwell   (501) staff       (20)    35148 2023-07-05 15:31:16.000000 bSuite-python-2.0.0/bSuite_auth/LICENSE
+-rw-r--r--   0 birdwell   (501) staff       (20)      369 2023-07-26 15:54:33.000000 bSuite-python-2.0.0/bSuite_auth/README.md
+-rw-r--r--   0 birdwell   (501) staff       (20)      909 2023-07-26 22:24:37.000000 bSuite-python-2.0.0/bSuite_auth/pyproject.toml
+drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-08-07 17:15:39.763064 bSuite-python-2.0.0/bSuite_auth/src/
+drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-08-07 17:15:39.763121 bSuite-python-2.0.0/bSuite_auth/src/bSuite/
+drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-08-07 17:15:39.766955 bSuite-python-2.0.0/bSuite_auth/src/bSuite/auth/
+-rw-r--r--   0 birdwell   (501) staff       (20)      137 2023-07-26 22:24:37.000000 bSuite-python-2.0.0/bSuite_auth/src/bSuite/auth/__init__.py
+-rw-r--r--   0 birdwell   (501) staff       (20)     6497 2023-07-31 19:06:13.000000 bSuite-python-2.0.0/bSuite_auth/src/bSuite/auth/client.py
+-rw-r--r--   0 birdwell   (501) staff       (20)      527 2023-07-26 16:06:12.000000 bSuite-python-2.0.0/bSuite_auth/src/bSuite/auth/etc.py
+-rw-r--r--   0 birdwell   (501) staff       (20)     3720 2023-07-26 22:24:02.000000 bSuite-python-2.0.0/bSuite_auth/src/bSuite/auth/middleware.py
+drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-08-07 17:15:39.767662 bSuite-python-2.0.0/bSuite_configure/
+-rw-r--r--   0 birdwell   (501) staff       (20)    35148 2023-07-05 15:31:16.000000 bSuite-python-2.0.0/bSuite_configure/LICENSE
+-rw-r--r--   0 birdwell   (501) staff       (20)      372 2023-07-05 02:23:50.000000 bSuite-python-2.0.0/bSuite_configure/pyproject.toml
+drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-08-07 17:15:39.763316 bSuite-python-2.0.0/bSuite_configure/src/
+drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-08-07 17:15:39.763368 bSuite-python-2.0.0/bSuite_configure/src/bSuite/
+drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-08-07 17:15:39.768367 bSuite-python-2.0.0/bSuite_configure/src/bSuite/configure/
+-rw-r--r--   0 birdwell   (501) staff       (20)       52 2023-07-05 01:59:36.000000 bSuite-python-2.0.0/bSuite_configure/src/bSuite/configure/__init__.py
+-rw-r--r--   0 birdwell   (501) staff       (20)     1233 2023-07-05 01:05:11.000000 bSuite-python-2.0.0/bSuite_configure/src/bSuite/configure/configure.py
+drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-08-07 17:15:39.773892 bSuite-python-2.0.0/bSuite_database/
+-rw-r--r--   0 birdwell   (501) staff       (20)    35148 2023-07-05 15:31:16.000000 bSuite-python-2.0.0/bSuite_database/LICENSE
+-rw-r--r--   0 birdwell   (501) staff       (20)       41 2023-08-05 18:47:08.000000 bSuite-python-2.0.0/bSuite_database/README.md
+-rw-r--r--   0 birdwell   (501) staff       (20)      937 2023-08-05 18:45:55.000000 bSuite-python-2.0.0/bSuite_database/pyproject.toml
+drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-08-07 17:15:39.763533 bSuite-python-2.0.0/bSuite_database/src/
+drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-08-07 17:15:39.763577 bSuite-python-2.0.0/bSuite_database/src/bSuite/
+drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-08-07 17:15:39.775472 bSuite-python-2.0.0/bSuite_database/src/bSuite/database/
+-rw-r--r--   0 birdwell   (501) staff       (20)      134 2023-08-05 18:42:02.000000 bSuite-python-2.0.0/bSuite_database/src/bSuite/database/__init__.py
+-rw-r--r--   0 birdwell   (501) staff       (20)     8010 2023-08-05 18:59:29.000000 bSuite-python-2.0.0/bSuite_database/src/bSuite/database/base.py
+-rw-r--r--   0 birdwell   (501) staff       (20)     2851 2023-07-25 14:48:38.000000 bSuite-python-2.0.0/bSuite_database/src/bSuite/database/crypto.py
+-rw-r--r--   0 birdwell   (501) staff       (20)     2629 2023-07-25 14:48:38.000000 bSuite-python-2.0.0/bSuite_database/src/bSuite/database/mapped.py
+-rw-r--r--   0 birdwell   (501) staff       (20)      482 2023-08-05 19:00:22.000000 bSuite-python-2.0.0/bSuite_database/src/bSuite/database/models.py
+drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-08-07 17:15:39.776279 bSuite-python-2.0.0/bSuite_python.egg-info/
+-rw-r--r--   0 birdwell   (501) staff       (20)    40971 2023-08-07 17:15:39.000000 bSuite-python-2.0.0/bSuite_python.egg-info/PKG-INFO
+-rw-r--r--   0 birdwell   (501) staff       (20)     1618 2023-08-07 17:15:39.000000 bSuite-python-2.0.0/bSuite_python.egg-info/SOURCES.txt
+-rw-r--r--   0 birdwell   (501) staff       (20)        1 2023-08-07 17:15:39.000000 bSuite-python-2.0.0/bSuite_python.egg-info/dependency_links.txt
+-rw-r--r--   0 birdwell   (501) staff       (20)       85 2023-08-07 17:15:39.000000 bSuite-python-2.0.0/bSuite_python.egg-info/requires.txt
+-rw-r--r--   0 birdwell   (501) staff       (20)        7 2023-08-07 17:15:39.000000 bSuite-python-2.0.0/bSuite_python.egg-info/top_level.txt
+drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-08-07 17:15:39.776588 bSuite-python-2.0.0/bSuite_spotify/
+-rw-r--r--   0 birdwell   (501) staff       (20)    35148 2023-07-25 14:48:38.000000 bSuite-python-2.0.0/bSuite_spotify/LICENSE
+-rw-r--r--   0 birdwell   (501) staff       (20)      439 2023-07-25 14:48:38.000000 bSuite-python-2.0.0/bSuite_spotify/pyproject.toml
+drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-08-07 17:15:39.763810 bSuite-python-2.0.0/bSuite_spotify/src/
+drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-08-07 17:15:39.763864 bSuite-python-2.0.0/bSuite_spotify/src/bSuite/
+drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-08-07 17:15:39.777002 bSuite-python-2.0.0/bSuite_spotify/src/bSuite/spotify/
+-rw-r--r--   0 birdwell   (501) staff       (20)      152 2023-07-25 14:48:38.000000 bSuite-python-2.0.0/bSuite_spotify/src/bSuite/spotify/__init__.py
+drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-08-07 17:15:39.777521 bSuite-python-2.0.0/bSuite_spotify/src/bSuite/spotify/tk/
+-rw-r--r--   0 birdwell   (501) staff       (20)       49 2023-07-25 14:48:38.000000 bSuite-python-2.0.0/bSuite_spotify/src/bSuite/spotify/tk/__init__.py
+-rw-r--r--   0 birdwell   (501) staff       (20)     2153 2023-07-25 14:48:38.000000 bSuite-python-2.0.0/bSuite_spotify/src/bSuite/spotify/tk/enhanced.py
+-rw-r--r--   0 birdwell   (501) staff       (20)      209 2023-08-01 14:26:01.000000 bSuite-python-2.0.0/bSuite_spotify/src/bSuite/spotify/utilities.py
+drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-08-07 17:15:39.778269 bSuite-python-2.0.0/bSuite_spotify/src/bSuite/spotify/web/
+-rw-r--r--   0 birdwell   (501) staff       (20)      112 2023-07-25 14:48:38.000000 bSuite-python-2.0.0/bSuite_spotify/src/bSuite/spotify/web/__init__.py
+-rw-r--r--   0 birdwell   (501) staff       (20)      164 2023-07-25 14:48:38.000000 bSuite-python-2.0.0/bSuite_spotify/src/bSuite/spotify/web/exceptions.py
+-rw-r--r--   0 birdwell   (501) staff       (20)     4147 2023-07-25 14:48:38.000000 bSuite-python-2.0.0/bSuite_spotify/src/bSuite/spotify/web/functional.py
+-rw-r--r--   0 birdwell   (501) staff       (20)     4263 2023-07-25 14:48:38.000000 bSuite-python-2.0.0/bSuite_spotify/src/bSuite/spotify/web/oop.py
+-rw-r--r--   0 birdwell   (501) staff       (20)      349 2023-07-25 14:48:38.000000 bSuite-python-2.0.0/bSuite_spotify/src/bSuite/spotify/web/temp.py
+drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-08-07 17:15:39.778620 bSuite-python-2.0.0/bSuite_utils/
+-rw-r--r--   0 birdwell   (501) staff       (20)    35148 2023-07-25 14:48:38.000000 bSuite-python-2.0.0/bSuite_utils/LICENSE
+-rw-r--r--   0 birdwell   (501) staff       (20)      837 2023-08-07 17:12:08.000000 bSuite-python-2.0.0/bSuite_utils/pyproject.toml
+drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-08-07 17:15:39.764163 bSuite-python-2.0.0/bSuite_utils/src/
+drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-08-07 17:15:39.764214 bSuite-python-2.0.0/bSuite_utils/src/bSuite/
+drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-08-07 17:15:39.779495 bSuite-python-2.0.0/bSuite_utils/src/bSuite/utils/
+-rw-r--r--   0 birdwell   (501) staff       (20)       23 2023-08-07 17:12:08.000000 bSuite-python-2.0.0/bSuite_utils/src/bSuite/utils/__init__.py
+-rw-r--r--   0 birdwell   (501) staff       (20)      834 2023-08-07 17:08:16.000000 bSuite-python-2.0.0/bSuite_utils/src/bSuite/utils/spotify.py
+-rw-r--r--   0 birdwell   (501) staff       (20)      594 2023-08-07 16:51:11.000000 bSuite-python-2.0.0/bSuite_utils/src/bSuite/utils/strings.py
+-rw-r--r--   0 birdwell   (501) staff       (20)       60 2023-08-01 14:26:01.000000 bSuite-python-2.0.0/bSuite_utils/src/bSuite/utils/time.py
+-rw-r--r--   0 birdwell   (501) staff       (20)     1238 2023-08-07 17:15:25.000000 bSuite-python-2.0.0/pyproject.toml
+-rw-r--r--   0 birdwell   (501) staff       (20)       38 2023-08-07 17:15:39.780211 bSuite-python-2.0.0/setup.cfg
+-rw-r--r--   0 birdwell   (501) staff       (20)       39 2023-07-05 00:44:00.000000 bSuite-python-2.0.0/setup.py
```

### Comparing `bSuite-python-1.1.3/LICENSE` & `bSuite-python-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bSuite-python-1.1.3/PKG-INFO` & `bSuite-python-2.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bSuite-python
-Version: 1.1.3
+Version: 2.0.0
 Summary: advanced helper modules. python edition
 Author-email: John Birdwell <j.c.birdwell@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -674,15 +674,14 @@
           The GNU General Public License does not permit incorporating your program
         into proprietary programs.  If your program is a subroutine library, you
         may consider it more useful to permit linking proprietary applications with
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
 Project-URL: Repository, https://github.com/jcbirdwell/bSuite
-Keywords: helpers,utilities,database,postgres,.ini
+Keywords: configs,utilities,database,postgres,authentication
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
-Provides-Extra: CRYPTO
 License-File: LICENSE
 
 Utility library
```

### Comparing `bSuite-python-1.1.3/bSuite_configure/LICENSE` & `bSuite-python-2.0.0/bSuite_auth/LICENSE`

 * *Files identical despite different names*

### Comparing `bSuite-python-1.1.3/bSuite_configure/src/bSuite/configure/configure.py` & `bSuite-python-2.0.0/bSuite_configure/src/bSuite/configure/configure.py`

 * *Files identical despite different names*

### Comparing `bSuite-python-1.1.3/bSuite_database/LICENSE` & `bSuite-python-2.0.0/bSuite_configure/LICENSE`

 * *Files identical despite different names*

### Comparing `bSuite-python-1.1.3/bSuite_database/src/bSuite/database/base.py` & `bSuite-python-2.0.0/bSuite_database/src/bSuite/database/base.py`

 * *Files identical despite different names*

### Comparing `bSuite-python-1.1.3/bSuite_database/src/bSuite/database/crypto.py` & `bSuite-python-2.0.0/bSuite_database/src/bSuite/database/crypto.py`

 * *Files identical despite different names*

### Comparing `bSuite-python-1.1.3/bSuite_database/src/bSuite/database/mapped.py` & `bSuite-python-2.0.0/bSuite_database/src/bSuite/database/mapped.py`

 * *Files identical despite different names*

### Comparing `bSuite-python-1.1.3/bSuite_python.egg-info/PKG-INFO` & `bSuite-python-2.0.0/bSuite_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bSuite-python
-Version: 1.1.3
+Version: 2.0.0
 Summary: advanced helper modules. python edition
 Author-email: John Birdwell <j.c.birdwell@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -674,15 +674,14 @@
           The GNU General Public License does not permit incorporating your program
         into proprietary programs.  If your program is a subroutine library, you
         may consider it more useful to permit linking proprietary applications with
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
 Project-URL: Repository, https://github.com/jcbirdwell/bSuite
-Keywords: helpers,utilities,database,postgres,.ini
+Keywords: configs,utilities,database,postgres,authentication
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
-Provides-Extra: CRYPTO
 License-File: LICENSE
 
 Utility library
```

