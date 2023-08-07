# Comparing `tmp/picu-1.3.tar.gz` & `tmp/picu-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picu-1.3.tar", last modified: Thu Oct 27 03:09:54 2022, max compression
+gzip compressed data, was "picu-1.4.tar", last modified: Mon Aug  7 18:12:45 2023, max compression
```

## Comparing `picu-1.3.tar` & `picu-1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 jbernard  (1000) jbernard  (1000)        0 2022-10-27 03:09:54.075933 picu-1.3/
--rw-r--r--   0 jbernard  (1000) jbernard  (1000)      168 2022-10-27 03:09:54.075933 picu-1.3/PKG-INFO
--rw-r--r--   0 jbernard  (1000) jbernard  (1000)      966 2022-03-08 19:58:46.000000 picu-1.3/README.rst
-drwxr-xr-x   0 jbernard  (1000) jbernard  (1000)        0 2022-10-27 03:09:54.075933 picu-1.3/picu/
--rw-r--r--   0 jbernard  (1000) jbernard  (1000)       46 2022-03-08 19:58:46.000000 picu-1.3/picu/__init__.py
--rw-r--r--   0 jbernard  (1000) jbernard  (1000)     1229 2022-03-08 19:58:46.000000 picu-1.3/picu/constants.py
--rw-r--r--   0 jbernard  (1000) jbernard  (1000)      962 2022-06-02 18:08:15.000000 picu-1.3/picu/exceptions.py
--rw-r--r--   0 jbernard  (1000) jbernard  (1000)     1185 2022-03-08 19:58:46.000000 picu-1.3/picu/finalize.py
--rw-r--r--   0 jbernard  (1000) jbernard  (1000)    32916 2022-06-02 18:08:15.000000 picu-1.3/picu/loader.py
--rw-r--r--   0 jbernard  (1000) jbernard  (1000)     1120 2022-06-27 15:11:21.000000 picu-1.3/picu/utils.py
-drwxr-xr-x   0 jbernard  (1000) jbernard  (1000)        0 2022-10-27 03:09:54.075933 picu-1.3/picu.egg-info/
--rw-r--r--   0 jbernard  (1000) jbernard  (1000)      168 2022-10-27 03:09:54.000000 picu-1.3/picu.egg-info/PKG-INFO
--rw-r--r--   0 jbernard  (1000) jbernard  (1000)      231 2022-10-27 03:09:54.000000 picu-1.3/picu.egg-info/SOURCES.txt
--rw-r--r--   0 jbernard  (1000) jbernard  (1000)        1 2022-10-27 03:09:54.000000 picu-1.3/picu.egg-info/dependency_links.txt
--rw-r--r--   0 jbernard  (1000) jbernard  (1000)        5 2022-10-27 03:09:54.000000 picu-1.3/picu.egg-info/top_level.txt
--rw-r--r--   0 jbernard  (1000) jbernard  (1000)       38 2022-10-27 03:09:54.075933 picu-1.3/setup.cfg
--rwxr-xr-x   0 jbernard  (1000) jbernard  (1000)      314 2022-10-24 14:51:49.000000 picu-1.3/setup.py
+drwxr-xr-x   0 jbernard  (1000) jbernard  (1000)        0 2023-08-07 18:12:45.892705 picu-1.4/
+-rw-r--r--   0 jbernard  (1000) jbernard  (1000)      223 2023-08-07 18:12:45.892705 picu-1.4/PKG-INFO
+-rw-r--r--   0 jbernard  (1000) jbernard  (1000)      966 2022-03-08 19:58:46.000000 picu-1.4/README.rst
+drwxr-xr-x   0 jbernard  (1000) jbernard  (1000)        0 2023-08-07 18:12:45.892705 picu-1.4/picu/
+-rw-r--r--   0 jbernard  (1000) jbernard  (1000)       46 2022-03-08 19:58:46.000000 picu-1.4/picu/__init__.py
+-rw-r--r--   0 jbernard  (1000) jbernard  (1000)     1229 2022-03-08 19:58:46.000000 picu-1.4/picu/constants.py
+-rw-r--r--   0 jbernard  (1000) jbernard  (1000)      962 2022-06-02 18:08:15.000000 picu-1.4/picu/exceptions.py
+-rw-r--r--   0 jbernard  (1000) jbernard  (1000)     1185 2022-03-08 19:58:46.000000 picu-1.4/picu/finalize.py
+-rw-r--r--   0 jbernard  (1000) jbernard  (1000)    33022 2023-07-03 16:29:20.000000 picu-1.4/picu/loader.py
+-rw-r--r--   0 jbernard  (1000) jbernard  (1000)     1120 2022-06-27 15:11:21.000000 picu-1.4/picu/utils.py
+drwxr-xr-x   0 jbernard  (1000) jbernard  (1000)        0 2023-08-07 18:12:45.892705 picu-1.4/picu.egg-info/
+-rw-r--r--   0 jbernard  (1000) jbernard  (1000)      223 2023-08-07 18:12:45.000000 picu-1.4/picu.egg-info/PKG-INFO
+-rw-r--r--   0 jbernard  (1000) jbernard  (1000)      231 2023-08-07 18:12:45.000000 picu-1.4/picu.egg-info/SOURCES.txt
+-rw-r--r--   0 jbernard  (1000) jbernard  (1000)        1 2023-08-07 18:12:45.000000 picu-1.4/picu.egg-info/dependency_links.txt
+-rw-r--r--   0 jbernard  (1000) jbernard  (1000)        5 2023-08-07 18:12:45.000000 picu-1.4/picu.egg-info/top_level.txt
+-rw-r--r--   0 jbernard  (1000) jbernard  (1000)       38 2023-08-07 18:12:45.892705 picu-1.4/setup.cfg
+-rwxr-xr-x   0 jbernard  (1000) jbernard  (1000)      322 2023-08-03 15:22:11.000000 picu-1.4/setup.py
```

### Comparing `picu-1.3/README.rst` & `picu-1.4/README.rst`

 * *Files identical despite different names*

### Comparing `picu-1.3/picu/constants.py` & `picu-1.4/picu/constants.py`

 * *Files identical despite different names*

### Comparing `picu-1.3/picu/exceptions.py` & `picu-1.4/picu/exceptions.py`

 * *Files identical despite different names*

### Comparing `picu-1.3/picu/finalize.py` & `picu-1.4/picu/finalize.py`

 * *Files identical despite different names*

### Comparing `picu-1.3/picu/loader.py` & `picu-1.4/picu/loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -773,14 +773,18 @@
 
     def is_script_rtl(self, script):
         script_prop = self.property_by_name('Script')
         script_enum = self.getPropertyValueEnum(script_prop.enum, script.encode('ascii'))
 
         return self.scriptIsRightToLeft(script_enum)
 
+    def is_rtl(self, cp):
+        script = self.get_script(cp)
+        return self.is_script_rtl(script)
+
     def is_digit(self, cp):
         return self.isDigit(cp)
 
     #### IDNA ####
     @memoized_property
     def uidna_openUTS46(self):
         return self.std_icu_func(self._getfunc('uidna_openUTS46',
```

### Comparing `picu-1.3/picu/utils.py` & `picu-1.4/picu/utils.py`

 * *Files identical despite different names*

