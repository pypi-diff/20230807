# Comparing `tmp/munidata-2.2.0.tar.gz` & `tmp/munidata-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "munidata-2.2.0.tar", last modified: Thu Oct 27 03:21:39 2022, max compression
+gzip compressed data, was "munidata-2.3.0.tar", last modified: Mon Aug  7 18:21:06 2023, max compression
```

## Comparing `munidata-2.2.0.tar` & `munidata-2.3.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 jbernard  (1000) jbernard  (1000)        0 2022-10-27 03:21:39.226170 munidata-2.2.0/
--rw-r--r--   0 jbernard  (1000) jbernard  (1000)     1539 2022-03-08 19:58:50.000000 munidata-2.2.0/LICENSE
--rw-r--r--   0 jbernard  (1000) jbernard  (1000)       82 2022-03-08 19:58:50.000000 munidata-2.2.0/MANIFEST.in
--rw-r--r--   0 jbernard  (1000) jbernard  (1000)     4438 2022-10-27 03:21:39.226170 munidata-2.2.0/PKG-INFO
--rw-r--r--   0 jbernard  (1000) jbernard  (1000)     3758 2022-10-27 03:19:07.000000 munidata-2.2.0/README.md
-drwxr-xr-x   0 jbernard  (1000) jbernard  (1000)        0 2022-10-27 03:21:39.226170 munidata-2.2.0/munidata/
--rw-r--r--   0 jbernard  (1000) jbernard  (1000)      112 2022-03-08 19:58:50.000000 munidata-2.2.0/munidata/__init__.py
--rw-r--r--   0 jbernard  (1000) jbernard  (1000)     6993 2022-03-08 19:58:50.000000 munidata-2.2.0/munidata/database.py
-drwxr-xr-x   0 jbernard  (1000) jbernard  (1000)        0 2022-10-27 03:21:39.226170 munidata-2.2.0/munidata/idna/
--rw-r--r--   0 jbernard  (1000) jbernard  (1000)        0 2022-03-08 19:58:50.000000 munidata-2.2.0/munidata/idna/__init__.py
--rw-r--r--   0 jbernard  (1000) jbernard  (1000)    51975 2022-03-08 19:58:50.000000 munidata-2.2.0/munidata/idna/idna_tables_1000.py
--rw-r--r--   0 jbernard  (1000) jbernard  (1000)    52856 2022-06-30 17:15:00.000000 munidata-2.2.0/munidata/idna/idna_tables_1100.py
--rw-r--r--   0 jbernard  (1000) jbernard  (1000)    53519 2022-06-30 15:49:51.000000 munidata-2.2.0/munidata/idna/idna_tables_1200.py
--rw-r--r--   0 jbernard  (1000) jbernard  (1000)    42396 2022-03-08 19:58:50.000000 munidata-2.2.0/munidata/idna/idna_tables_520.py
--rw-r--r--   0 jbernard  (1000) jbernard  (1000)    43708 2022-03-08 19:58:50.000000 munidata-2.2.0/munidata/idna/idna_tables_600.py
--rw-r--r--   0 jbernard  (1000) jbernard  (1000)    45247 2022-03-08 19:58:50.000000 munidata-2.2.0/munidata/idna/idna_tables_610.py
--rw-r--r--   0 jbernard  (1000) jbernard  (1000)    45247 2022-03-08 19:58:50.000000 munidata-2.2.0/munidata/idna/idna_tables_620.py
--rw-r--r--   0 jbernard  (1000) jbernard  (1000)    45264 2022-03-08 19:58:50.000000 munidata-2.2.0/munidata/idna/idna_tables_630.py
--rw-r--r--   0 jbernard  (1000) jbernard  (1000)    48877 2022-03-08 19:58:50.000000 munidata-2.2.0/munidata/idna/idna_tables_700.py
--rw-r--r--   0 jbernard  (1000) jbernard  (1000)    50161 2022-03-08 19:58:50.000000 munidata-2.2.0/munidata/idna/idna_tables_800.py
--rw-r--r--   0 jbernard  (1000) jbernard  (1000)    51411 2022-03-08 19:58:50.000000 munidata-2.2.0/munidata/idna/idna_tables_900.py
--rw-r--r--   0 jbernard  (1000) jbernard  (1000)     2050 2022-06-30 18:14:31.000000 munidata-2.2.0/munidata/idna/idnatables.py
--rw-r--r--   0 jbernard  (1000) jbernard  (1000)     1616 2022-03-08 19:58:50.000000 munidata-2.2.0/munidata/manager.py
-drwxr-xr-x   0 jbernard  (1000) jbernard  (1000)        0 2022-10-27 03:21:39.226170 munidata-2.2.0/munidata.egg-info/
--rw-r--r--   0 jbernard  (1000) jbernard  (1000)     4438 2022-10-27 03:21:38.000000 munidata-2.2.0/munidata.egg-info/PKG-INFO
--rw-r--r--   0 jbernard  (1000) jbernard  (1000)      754 2022-10-27 03:21:39.000000 munidata-2.2.0/munidata.egg-info/SOURCES.txt
--rw-r--r--   0 jbernard  (1000) jbernard  (1000)        1 2022-10-27 03:21:38.000000 munidata-2.2.0/munidata.egg-info/dependency_links.txt
--rw-r--r--   0 jbernard  (1000) jbernard  (1000)        5 2022-10-27 03:21:39.000000 munidata-2.2.0/munidata.egg-info/requires.txt
--rw-r--r--   0 jbernard  (1000) jbernard  (1000)        9 2022-10-27 03:21:39.000000 munidata-2.2.0/munidata.egg-info/top_level.txt
--rwxr-xr-x   0 jbernard  (1000) jbernard  (1000)     2463 2022-03-08 19:58:50.000000 munidata-2.2.0/picu_multi.py
--rw-r--r--   0 jbernard  (1000) jbernard  (1000)       10 2022-03-08 19:58:50.000000 munidata-2.2.0/requirements.txt
--rw-r--r--   0 jbernard  (1000) jbernard  (1000)       38 2022-10-27 03:21:39.226170 munidata-2.2.0/setup.cfg
--rwxr-xr-x   0 jbernard  (1000) jbernard  (1000)      967 2022-10-27 03:21:27.000000 munidata-2.2.0/setup.py
--rwxr-xr-x   0 jbernard  (1000) jbernard  (1000)     1905 2022-03-08 19:58:50.000000 munidata-2.2.0/test_munidata.py
-drwxr-xr-x   0 jbernard  (1000) jbernard  (1000)        0 2022-10-27 03:21:39.226170 munidata-2.2.0/tools/
--rwxr-xr-x   0 jbernard  (1000) jbernard  (1000)     4325 2022-07-01 14:24:19.000000 munidata-2.2.0/tools/parse_idna_tables.py
+drwxr-xr-x   0 jbernard  (1000) jbernard  (1000)        0 2023-08-07 18:21:06.001068 munidata-2.3.0/
+-rw-r--r--   0 jbernard  (1000) jbernard  (1000)     1539 2022-03-08 19:58:50.000000 munidata-2.3.0/LICENSE
+-rw-r--r--   0 jbernard  (1000) jbernard  (1000)       82 2022-03-08 19:58:50.000000 munidata-2.3.0/MANIFEST.in
+-rw-r--r--   0 jbernard  (1000) jbernard  (1000)     4615 2023-08-07 18:21:06.001068 munidata-2.3.0/PKG-INFO
+-rw-r--r--   0 jbernard  (1000) jbernard  (1000)     3758 2022-10-27 03:19:07.000000 munidata-2.3.0/README.md
+drwxr-xr-x   0 jbernard  (1000) jbernard  (1000)        0 2023-08-07 18:21:05.997735 munidata-2.3.0/munidata/
+-rw-r--r--   0 jbernard  (1000) jbernard  (1000)      112 2022-03-08 19:58:50.000000 munidata-2.3.0/munidata/__init__.py
+-rw-r--r--   0 jbernard  (1000) jbernard  (1000)     7303 2023-07-03 16:22:52.000000 munidata-2.3.0/munidata/database.py
+drwxr-xr-x   0 jbernard  (1000) jbernard  (1000)        0 2023-08-07 18:21:06.001068 munidata-2.3.0/munidata/idna/
+-rw-r--r--   0 jbernard  (1000) jbernard  (1000)        0 2022-03-08 19:58:50.000000 munidata-2.3.0/munidata/idna/__init__.py
+-rw-r--r--   0 jbernard  (1000) jbernard  (1000)    51975 2022-03-08 19:58:50.000000 munidata-2.3.0/munidata/idna/idna_tables_1000.py
+-rw-r--r--   0 jbernard  (1000) jbernard  (1000)    52856 2022-06-30 17:15:00.000000 munidata-2.3.0/munidata/idna/idna_tables_1100.py
+-rw-r--r--   0 jbernard  (1000) jbernard  (1000)    53519 2022-06-30 15:49:51.000000 munidata-2.3.0/munidata/idna/idna_tables_1200.py
+-rw-r--r--   0 jbernard  (1000) jbernard  (1000)    42396 2022-03-08 19:58:50.000000 munidata-2.3.0/munidata/idna/idna_tables_520.py
+-rw-r--r--   0 jbernard  (1000) jbernard  (1000)    43708 2022-03-08 19:58:50.000000 munidata-2.3.0/munidata/idna/idna_tables_600.py
+-rw-r--r--   0 jbernard  (1000) jbernard  (1000)    45247 2022-03-08 19:58:50.000000 munidata-2.3.0/munidata/idna/idna_tables_610.py
+-rw-r--r--   0 jbernard  (1000) jbernard  (1000)    45247 2022-03-08 19:58:50.000000 munidata-2.3.0/munidata/idna/idna_tables_620.py
+-rw-r--r--   0 jbernard  (1000) jbernard  (1000)    45264 2022-03-08 19:58:50.000000 munidata-2.3.0/munidata/idna/idna_tables_630.py
+-rw-r--r--   0 jbernard  (1000) jbernard  (1000)    48877 2022-03-08 19:58:50.000000 munidata-2.3.0/munidata/idna/idna_tables_700.py
+-rw-r--r--   0 jbernard  (1000) jbernard  (1000)    50161 2022-03-08 19:58:50.000000 munidata-2.3.0/munidata/idna/idna_tables_800.py
+-rw-r--r--   0 jbernard  (1000) jbernard  (1000)    51411 2022-03-08 19:58:50.000000 munidata-2.3.0/munidata/idna/idna_tables_900.py
+-rw-r--r--   0 jbernard  (1000) jbernard  (1000)     2050 2022-06-30 18:14:31.000000 munidata-2.3.0/munidata/idna/idnatables.py
+-rw-r--r--   0 jbernard  (1000) jbernard  (1000)     1616 2022-03-08 19:58:50.000000 munidata-2.3.0/munidata/manager.py
+drwxr-xr-x   0 jbernard  (1000) jbernard  (1000)        0 2023-08-07 18:21:05.997735 munidata-2.3.0/munidata.egg-info/
+-rw-r--r--   0 jbernard  (1000) jbernard  (1000)     4615 2023-08-07 18:21:05.000000 munidata-2.3.0/munidata.egg-info/PKG-INFO
+-rw-r--r--   0 jbernard  (1000) jbernard  (1000)      754 2023-08-07 18:21:05.000000 munidata-2.3.0/munidata.egg-info/SOURCES.txt
+-rw-r--r--   0 jbernard  (1000) jbernard  (1000)        1 2023-08-07 18:21:05.000000 munidata-2.3.0/munidata.egg-info/dependency_links.txt
+-rw-r--r--   0 jbernard  (1000) jbernard  (1000)        5 2023-08-07 18:21:05.000000 munidata-2.3.0/munidata.egg-info/requires.txt
+-rw-r--r--   0 jbernard  (1000) jbernard  (1000)        9 2023-08-07 18:21:05.000000 munidata-2.3.0/munidata.egg-info/top_level.txt
+-rwxr-xr-x   0 jbernard  (1000) jbernard  (1000)     2463 2022-03-08 19:58:50.000000 munidata-2.3.0/picu_multi.py
+-rw-r--r--   0 jbernard  (1000) jbernard  (1000)       10 2023-08-03 15:26:37.000000 munidata-2.3.0/requirements.txt
+-rw-r--r--   0 jbernard  (1000) jbernard  (1000)       38 2023-08-07 18:21:06.001068 munidata-2.3.0/setup.cfg
+-rwxr-xr-x   0 jbernard  (1000) jbernard  (1000)     1122 2023-08-03 16:31:19.000000 munidata-2.3.0/setup.py
+-rwxr-xr-x   0 jbernard  (1000) jbernard  (1000)     1905 2022-03-08 19:58:50.000000 munidata-2.3.0/test_munidata.py
+drwxr-xr-x   0 jbernard  (1000) jbernard  (1000)        0 2023-08-07 18:21:06.001068 munidata-2.3.0/tools/
+-rwxr-xr-x   0 jbernard  (1000) jbernard  (1000)     4325 2022-07-01 14:24:19.000000 munidata-2.3.0/tools/parse_idna_tables.py
```

### Comparing `munidata-2.2.0/LICENSE` & `munidata-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `munidata-2.2.0/PKG-INFO` & `munidata-2.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 Metadata-Version: 2.1
 Name: munidata
-Version: 2.2.0
+Version: 2.3.0
 Summary: Provides an API for accessing multiple instances of Unicode data
-Author: Viagenie and Wil Tan
-Author-email: support@viagenie.ca
-License: TBD
+Home-page: UNKNOWN
+Author: Cofomo, Viagenie and Wil Tan
+Author-email: int-eng@cofomo.com
+License: BSD
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Munidata
 
 munidata is an API for accessing multiple instances of Unicode data.
```

### Comparing `munidata-2.2.0/README.md` & `munidata-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `munidata-2.2.0/munidata/database.py` & `munidata-2.3.0/munidata/database.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,14 +56,23 @@
         Check if character is a digit.
 
         :param cp: Codepoint.
         :return:  Whether the character is a digit.
         """
         raise NotImplementedError
 
+    def is_rtl(self, cp):
+        """
+        Check is character is from a Right To Left script.
+
+        :param cp: Codepoint.
+        :return:  Whether the character is from a Right To Left script.
+        """
+        raise NotImplementedError
+
     def is_script_rtl(self, script):
         """
         Check is a script is Right To Left.
 
         :param script: Script.
         :return: Whether the script is Right To Left.
         """
@@ -180,14 +189,17 @@
 
     def is_combining_mark(self, cp):
         return self._icu.is_combining_mark(cp)
 
     def is_digit(self, cp):
         return self._icu.is_digit(cp)
 
+    def is_rtl(self, cp):
+        return self._icu.is_rtl(cp)
+
     def is_script_rtl(self, script):
         return self._icu.is_script_rtl(script)
 
     def get_script_extensions(self, cp, alpha4=False):
         if alpha4:
             prop_type = U_SHORT_PROPERTY_NAME
         else:
```

### Comparing `munidata-2.2.0/munidata/idna/idna_tables_1000.py` & `munidata-2.3.0/munidata/idna/idna_tables_1000.py`

 * *Files identical despite different names*

### Comparing `munidata-2.2.0/munidata/idna/idna_tables_1100.py` & `munidata-2.3.0/munidata/idna/idna_tables_1100.py`

 * *Files identical despite different names*

### Comparing `munidata-2.2.0/munidata/idna/idna_tables_1200.py` & `munidata-2.3.0/munidata/idna/idna_tables_1200.py`

 * *Files identical despite different names*

### Comparing `munidata-2.2.0/munidata/idna/idna_tables_520.py` & `munidata-2.3.0/munidata/idna/idna_tables_520.py`

 * *Files identical despite different names*

### Comparing `munidata-2.2.0/munidata/idna/idna_tables_600.py` & `munidata-2.3.0/munidata/idna/idna_tables_600.py`

 * *Files identical despite different names*

### Comparing `munidata-2.2.0/munidata/idna/idna_tables_610.py` & `munidata-2.3.0/munidata/idna/idna_tables_610.py`

 * *Files identical despite different names*

### Comparing `munidata-2.2.0/munidata/idna/idna_tables_620.py` & `munidata-2.3.0/munidata/idna/idna_tables_620.py`

 * *Files identical despite different names*

### Comparing `munidata-2.2.0/munidata/idna/idna_tables_630.py` & `munidata-2.3.0/munidata/idna/idna_tables_630.py`

 * *Files identical despite different names*

### Comparing `munidata-2.2.0/munidata/idna/idna_tables_700.py` & `munidata-2.3.0/munidata/idna/idna_tables_700.py`

 * *Files identical despite different names*

### Comparing `munidata-2.2.0/munidata/idna/idna_tables_800.py` & `munidata-2.3.0/munidata/idna/idna_tables_800.py`

 * *Files identical despite different names*

### Comparing `munidata-2.2.0/munidata/idna/idna_tables_900.py` & `munidata-2.3.0/munidata/idna/idna_tables_900.py`

 * *Files identical despite different names*

### Comparing `munidata-2.2.0/munidata/idna/idnatables.py` & `munidata-2.3.0/munidata/idna/idnatables.py`

 * *Files identical despite different names*

### Comparing `munidata-2.2.0/munidata/manager.py` & `munidata-2.3.0/munidata/manager.py`

 * *Files identical despite different names*

### Comparing `munidata-2.2.0/munidata.egg-info/PKG-INFO` & `munidata-2.3.0/munidata.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 Metadata-Version: 2.1
 Name: munidata
-Version: 2.2.0
+Version: 2.3.0
 Summary: Provides an API for accessing multiple instances of Unicode data
-Author: Viagenie and Wil Tan
-Author-email: support@viagenie.ca
-License: TBD
+Home-page: UNKNOWN
+Author: Cofomo, Viagenie and Wil Tan
+Author-email: int-eng@cofomo.com
+License: BSD
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Munidata
 
 munidata is an API for accessing multiple instances of Unicode data.
```

### Comparing `munidata-2.2.0/munidata.egg-info/SOURCES.txt` & `munidata-2.3.0/munidata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `munidata-2.2.0/picu_multi.py` & `munidata-2.3.0/picu_multi.py`

 * *Files identical despite different names*

### Comparing `munidata-2.2.0/test_munidata.py` & `munidata-2.3.0/test_munidata.py`

 * *Files identical despite different names*

### Comparing `munidata-2.2.0/tools/parse_idna_tables.py` & `munidata-2.3.0/tools/parse_idna_tables.py`

 * *Files identical despite different names*

