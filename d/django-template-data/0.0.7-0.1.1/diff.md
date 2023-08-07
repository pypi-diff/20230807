# Comparing `tmp/django-template-data-0.0.7.tar.gz` & `tmp/django-template-data-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-template-data-0.0.7.tar", last modified: Thu May 12 02:37:57 2022, max compression
+gzip compressed data, was "django-template-data-0.1.1.tar", last modified: Mon Aug  7 18:14:51 2023, max compression
```

## Comparing `django-template-data-0.0.7.tar` & `django-template-data-0.1.1.tar`

### file list

```diff
@@ -1,30 +1,29 @@
-drwxrwxr-x   0 jefcolbi  (1000) jefcolbi  (1000)        0 2022-05-12 02:37:57.000000 django-template-data-0.0.7/
-drwxrwxr-x   0 jefcolbi  (1000) jefcolbi  (1000)        0 2022-05-12 02:37:57.000000 django-template-data-0.0.7/django_template_data.egg-info/
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)       32 2022-05-12 02:37:57.000000 django-template-data-0.0.7/django_template_data.egg-info/requires.txt
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)        1 2022-05-12 02:37:57.000000 django-template-data-0.0.7/django_template_data.egg-info/dependency_links.txt
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)     4312 2022-05-12 02:37:57.000000 django-template-data-0.0.7/django_template_data.egg-info/PKG-INFO
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)      830 2022-05-12 02:37:57.000000 django-template-data-0.0.7/django_template_data.egg-info/SOURCES.txt
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)       14 2022-05-12 02:37:57.000000 django-template-data-0.0.7/django_template_data.egg-info/top_level.txt
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)     4312 2022-05-12 02:37:57.000000 django-template-data-0.0.7/PKG-INFO
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)       38 2022-05-12 02:37:57.000000 django-template-data-0.0.7/setup.cfg
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)     2795 2020-10-05 03:01:08.000000 django-template-data-0.0.7/README.md
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)     3890 2022-05-12 02:37:18.000000 django-template-data-0.0.7/setup.py
-drwxrwxr-x   0 jefcolbi  (1000) jefcolbi  (1000)        0 2022-05-12 02:37:57.000000 django-template-data-0.0.7/template_data/
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)        1 2020-06-03 02:31:19.000000 django-template-data-0.0.7/template_data/__init__.py
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)     1644 2022-04-18 22:39:28.000000 django-template-data-0.0.7/template_data/admin.py
-drwxrwxr-x   0 jefcolbi  (1000) jefcolbi  (1000)        0 2022-05-12 02:37:57.000000 django-template-data-0.0.7/template_data/management/
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)        0 2022-05-03 20:41:02.000000 django-template-data-0.0.7/template_data/management/__init__.py
-drwxrwxr-x   0 jefcolbi  (1000) jefcolbi  (1000)        0 2022-05-12 02:37:57.000000 django-template-data-0.0.7/template_data/management/commands/
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)        0 2022-05-03 20:41:10.000000 django-template-data-0.0.7/template_data/management/commands/__init__.py
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)     1256 2022-05-11 23:08:59.000000 django-template-data-0.0.7/template_data/management/commands/save_data.py
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)     1085 2022-05-11 23:21:15.000000 django-template-data-0.0.7/template_data/management/commands/restore_data.py
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)     2336 2022-05-04 15:53:11.000000 django-template-data-0.0.7/template_data/management/commands/add_data.py
-drwxrwxr-x   0 jefcolbi  (1000) jefcolbi  (1000)        0 2022-05-12 02:37:57.000000 django-template-data-0.0.7/template_data/migrations/
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)        1 2020-10-05 01:33:48.000000 django-template-data-0.0.7/template_data/migrations/__init__.py
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)      470 2022-05-04 15:53:36.000000 django-template-data-0.0.7/template_data/migrations/0003_alter_templatedata_lang.py
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)     1233 2020-10-05 01:37:43.000000 django-template-data-0.0.7/template_data/migrations/0001_initial.py
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)      664 2022-04-18 22:28:07.000000 django-template-data-0.0.7/template_data/migrations/0002_auto_20220418_2228.py
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)      473 2022-05-12 00:01:24.000000 django-template-data-0.0.7/template_data/migrations/0004_alter_templatedata_lang.py
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)      128 2022-04-18 20:01:36.000000 django-template-data-0.0.7/template_data/apps.py
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)     1599 2022-05-03 20:41:15.000000 django-template-data-0.0.7/template_data/models.py
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)     2711 2022-05-03 20:41:15.000000 django-template-data-0.0.7/template_data/processors.py
+drwxrwxr-x   0 jefcolbi  (1000) jefcolbi  (1000)        0 2023-08-07 18:14:51.780547 django-template-data-0.1.1/
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)     7494 2023-08-07 18:14:51.780547 django-template-data-0.1.1/PKG-INFO
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)     5265 2023-08-07 17:51:02.000000 django-template-data-0.1.1/README.md
+drwxrwxr-x   0 jefcolbi  (1000) jefcolbi  (1000)        0 2023-08-07 18:14:51.780547 django-template-data-0.1.1/django_template_data.egg-info/
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)     7494 2023-08-07 18:14:51.000000 django-template-data-0.1.1/django_template_data.egg-info/PKG-INFO
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)      791 2023-08-07 18:14:51.000000 django-template-data-0.1.1/django_template_data.egg-info/SOURCES.txt
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)        1 2023-08-07 18:14:51.000000 django-template-data-0.1.1/django_template_data.egg-info/dependency_links.txt
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)       50 2023-08-07 18:14:51.000000 django-template-data-0.1.1/django_template_data.egg-info/requires.txt
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)       14 2023-08-07 18:14:51.000000 django-template-data-0.1.1/django_template_data.egg-info/top_level.txt
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)       38 2023-08-07 18:14:51.780547 django-template-data-0.1.1/setup.cfg
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)     3922 2023-08-07 18:13:35.000000 django-template-data-0.1.1/setup.py
+drwxrwxr-x   0 jefcolbi  (1000) jefcolbi  (1000)        0 2023-08-07 18:14:51.780547 django-template-data-0.1.1/template_data/
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)        1 2023-05-17 16:46:06.000000 django-template-data-0.1.1/template_data/__init__.py
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)     1644 2023-05-17 16:46:06.000000 django-template-data-0.1.1/template_data/admin.py
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)      128 2023-05-17 16:46:06.000000 django-template-data-0.1.1/template_data/apps.py
+drwxrwxr-x   0 jefcolbi  (1000) jefcolbi  (1000)        0 2023-08-07 18:14:51.780547 django-template-data-0.1.1/template_data/management/
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)        0 2023-05-17 16:46:06.000000 django-template-data-0.1.1/template_data/management/__init__.py
+drwxrwxr-x   0 jefcolbi  (1000) jefcolbi  (1000)        0 2023-08-07 18:14:51.780547 django-template-data-0.1.1/template_data/management/commands/
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)        0 2023-05-17 16:46:06.000000 django-template-data-0.1.1/template_data/management/commands/__init__.py
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)     2336 2023-05-17 16:46:06.000000 django-template-data-0.1.1/template_data/management/commands/add_data.py
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)     1085 2023-05-17 16:46:06.000000 django-template-data-0.1.1/template_data/management/commands/restore_data.py
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)     7137 2023-08-07 17:20:28.000000 django-template-data-0.1.1/template_data/management/commands/rewrite_template.py
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)     1256 2023-05-17 16:46:06.000000 django-template-data-0.1.1/template_data/management/commands/save_data.py
+drwxrwxr-x   0 jefcolbi  (1000) jefcolbi  (1000)        0 2023-08-07 18:14:51.780547 django-template-data-0.1.1/template_data/migrations/
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)     1233 2023-05-17 16:46:06.000000 django-template-data-0.1.1/template_data/migrations/0001_initial.py
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)     2727 2023-08-07 17:09:40.000000 django-template-data-0.1.1/template_data/migrations/0002_templatedata_lang_alter_templatedata_id.py
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)        1 2023-05-17 16:46:06.000000 django-template-data-0.1.1/template_data/migrations/__init__.py
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)     1599 2023-05-17 16:46:06.000000 django-template-data-0.1.1/template_data/models.py
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)     2711 2023-05-17 16:46:06.000000 django-template-data-0.1.1/template_data/processors.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-template-data-0.0.7/django_template_data.egg-info/SOURCES.txt` & `django-template-data-0.1.1/django_template_data.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -10,13 +10,12 @@
 template_data/apps.py
 template_data/models.py
 template_data/processors.py
 template_data/management/__init__.py
 template_data/management/commands/__init__.py
 template_data/management/commands/add_data.py
 template_data/management/commands/restore_data.py
+template_data/management/commands/rewrite_template.py
 template_data/management/commands/save_data.py
 template_data/migrations/0001_initial.py
-template_data/migrations/0002_auto_20220418_2228.py
-template_data/migrations/0003_alter_templatedata_lang.py
-template_data/migrations/0004_alter_templatedata_lang.py
+template_data/migrations/0002_templatedata_lang_alter_templatedata_id.py
 template_data/migrations/__init__.py
```

### Comparing `django-template-data-0.0.7/setup.py` & `django-template-data-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,19 +14,21 @@
 # Package meta-data.
 NAME = 'django-template-data'
 DESCRIPTION = 'A library to load data from database to template'
 URL = 'https://github.com/jefcolbi/django-template-data'
 EMAIL = 'jefcolbi@gmail.com'
 AUTHOR = 'jefcolbi'
 REQUIRES_PYTHON = '>=3.5'
-VERSION = '0.0.7'
+VERSION = '0.1.1'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
-    "django>=3.0"
+    "django>=3.0",
+    "lxml",
+    "html5-parser"
 ]
 
 # What packages are optional?
 EXTRAS = {
     'meta': ['django-meta'],
 }
```

### Comparing `django-template-data-0.0.7/template_data/admin.py` & `django-template-data-0.1.1/template_data/admin.py`

 * *Files identical despite different names*

### Comparing `django-template-data-0.0.7/template_data/management/commands/save_data.py` & `django-template-data-0.1.1/template_data/management/commands/save_data.py`

 * *Files identical despite different names*

### Comparing `django-template-data-0.0.7/template_data/management/commands/restore_data.py` & `django-template-data-0.1.1/template_data/management/commands/restore_data.py`

 * *Files identical despite different names*

### Comparing `django-template-data-0.0.7/template_data/management/commands/add_data.py` & `django-template-data-0.1.1/template_data/management/commands/add_data.py`

 * *Files identical despite different names*

### Comparing `django-template-data-0.0.7/template_data/migrations/0001_initial.py` & `django-template-data-0.1.1/template_data/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-template-data-0.0.7/template_data/models.py` & `django-template-data-0.1.1/template_data/models.py`

 * *Files identical despite different names*

### Comparing `django-template-data-0.0.7/template_data/processors.py` & `django-template-data-0.1.1/template_data/processors.py`

 * *Files identical despite different names*

