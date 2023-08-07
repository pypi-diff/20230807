# Comparing `tmp/django-permagate-1.0.2.tar.gz` & `tmp/django-permagate-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-permagate-1.0.2.tar", last modified: Mon Aug  7 19:53:32 2023, max compression
+gzip compressed data, was "django-permagate-1.0.3.tar", last modified: Mon Aug  7 20:00:10 2023, max compression
```

## Comparing `django-permagate-1.0.2.tar` & `django-permagate-1.0.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 dbozh     (1000) dbozh     (1000)        0 2023-08-07 19:53:32.580596 django-permagate-1.0.2/
--rw-r--r--   0 dbozh     (1000) dbozh     (1000)     1066 2023-08-07 18:18:41.000000 django-permagate-1.0.2/LICENSE
--rw-r--r--   0 dbozh     (1000) dbozh     (1000)       83 2023-08-07 18:52:50.000000 django-permagate-1.0.2/MANIFEST.in
--rw-r--r--   0 dbozh     (1000) dbozh     (1000)     4591 2023-08-07 19:53:32.580596 django-permagate-1.0.2/PKG-INFO
--rw-r--r--   0 dbozh     (1000) dbozh     (1000)     3741 2023-08-07 19:45:34.000000 django-permagate-1.0.2/README.md
-drwxr-xr-x   0 dbozh     (1000) dbozh     (1000)        0 2023-08-07 19:53:32.570596 django-permagate-1.0.2/django_permagate.egg-info/
--rw-r--r--   0 dbozh     (1000) dbozh     (1000)     4591 2023-08-07 19:53:32.000000 django-permagate-1.0.2/django_permagate.egg-info/PKG-INFO
--rw-r--r--   0 dbozh     (1000) dbozh     (1000)      521 2023-08-07 19:53:32.000000 django-permagate-1.0.2/django_permagate.egg-info/SOURCES.txt
--rw-r--r--   0 dbozh     (1000) dbozh     (1000)        1 2023-08-07 19:53:32.000000 django-permagate-1.0.2/django_permagate.egg-info/dependency_links.txt
--rw-r--r--   0 dbozh     (1000) dbozh     (1000)       12 2023-08-07 19:53:32.000000 django-permagate-1.0.2/django_permagate.egg-info/requires.txt
--rw-r--r--   0 dbozh     (1000) dbozh     (1000)       27 2023-08-07 19:53:32.000000 django-permagate-1.0.2/django_permagate.egg-info/top_level.txt
-drwxr-xr-x   0 dbozh     (1000) dbozh     (1000)        0 2023-08-07 19:53:32.580596 django-permagate-1.0.2/permagate/
--rw-r--r--   0 dbozh     (1000) dbozh     (1000)        0 2023-08-07 17:54:26.000000 django-permagate-1.0.2/permagate/__init__.py
--rw-r--r--   0 dbozh     (1000) dbozh     (1000)       63 2023-08-03 17:00:47.000000 django-permagate-1.0.2/permagate/admin.py
--rw-r--r--   0 dbozh     (1000) dbozh     (1000)      150 2023-08-07 17:52:54.000000 django-permagate-1.0.2/permagate/apps.py
--rw-r--r--   0 dbozh     (1000) dbozh     (1000)     2876 2023-08-07 17:19:40.000000 django-permagate-1.0.2/permagate/core.py
-drwxr-xr-x   0 dbozh     (1000) dbozh     (1000)        0 2023-08-07 19:53:32.580596 django-permagate-1.0.2/permagate/migrations/
--rw-r--r--   0 dbozh     (1000) dbozh     (1000)     2544 2023-08-07 19:53:03.000000 django-permagate-1.0.2/permagate/migrations/0001_initial.py
--rw-r--r--   0 dbozh     (1000) dbozh     (1000)        0 2023-07-24 20:37:50.000000 django-permagate-1.0.2/permagate/migrations/__init__.py
--rw-r--r--   0 dbozh     (1000) dbozh     (1000)     1152 2023-08-07 19:52:04.000000 django-permagate-1.0.2/permagate/models.py
--rw-r--r--   0 dbozh     (1000) dbozh     (1000)     7307 2023-08-07 17:03:48.000000 django-permagate-1.0.2/permagate/permission.py
--rw-r--r--   0 dbozh     (1000) dbozh     (1000)      789 2023-08-07 17:42:18.000000 django-permagate-1.0.2/permagate/test_permissions.py
--rw-r--r--   0 dbozh     (1000) dbozh     (1000)     4204 2023-08-07 17:52:11.000000 django-permagate-1.0.2/permagate/tests.py
--rw-r--r--   0 dbozh     (1000) dbozh     (1000)       63 2023-07-24 20:37:50.000000 django-permagate-1.0.2/permagate/views.py
--rw-r--r--   0 dbozh     (1000) dbozh     (1000)       84 2023-08-07 18:38:18.000000 django-permagate-1.0.2/pyproject.toml
--rw-r--r--   0 dbozh     (1000) dbozh     (1000)      944 2023-08-07 19:53:32.580596 django-permagate-1.0.2/setup.cfg
--rw-r--r--   0 dbozh     (1000) dbozh     (1000)       41 2023-08-07 18:34:35.000000 django-permagate-1.0.2/setup.py
+drwxr-xr-x   0 dbozh     (1000) dbozh     (1000)        0 2023-08-07 20:00:10.020600 django-permagate-1.0.3/
+-rw-r--r--   0 dbozh     (1000) dbozh     (1000)     1066 2023-08-07 18:18:41.000000 django-permagate-1.0.3/LICENSE
+-rw-r--r--   0 dbozh     (1000) dbozh     (1000)       83 2023-08-07 18:52:50.000000 django-permagate-1.0.3/MANIFEST.in
+-rw-r--r--   0 dbozh     (1000) dbozh     (1000)     4591 2023-08-07 20:00:10.020600 django-permagate-1.0.3/PKG-INFO
+-rw-r--r--   0 dbozh     (1000) dbozh     (1000)     3741 2023-08-07 19:45:34.000000 django-permagate-1.0.3/README.md
+drwxr-xr-x   0 dbozh     (1000) dbozh     (1000)        0 2023-08-07 20:00:10.010600 django-permagate-1.0.3/django_permagate.egg-info/
+-rw-r--r--   0 dbozh     (1000) dbozh     (1000)     4591 2023-08-07 20:00:10.000000 django-permagate-1.0.3/django_permagate.egg-info/PKG-INFO
+-rw-r--r--   0 dbozh     (1000) dbozh     (1000)      521 2023-08-07 20:00:10.000000 django-permagate-1.0.3/django_permagate.egg-info/SOURCES.txt
+-rw-r--r--   0 dbozh     (1000) dbozh     (1000)        1 2023-08-07 20:00:10.000000 django-permagate-1.0.3/django_permagate.egg-info/dependency_links.txt
+-rw-r--r--   0 dbozh     (1000) dbozh     (1000)       12 2023-08-07 20:00:10.000000 django-permagate-1.0.3/django_permagate.egg-info/requires.txt
+-rw-r--r--   0 dbozh     (1000) dbozh     (1000)       27 2023-08-07 20:00:10.000000 django-permagate-1.0.3/django_permagate.egg-info/top_level.txt
+drwxr-xr-x   0 dbozh     (1000) dbozh     (1000)        0 2023-08-07 20:00:10.010600 django-permagate-1.0.3/permagate/
+-rw-r--r--   0 dbozh     (1000) dbozh     (1000)        0 2023-08-07 17:54:26.000000 django-permagate-1.0.3/permagate/__init__.py
+-rw-r--r--   0 dbozh     (1000) dbozh     (1000)       63 2023-08-03 17:00:47.000000 django-permagate-1.0.3/permagate/admin.py
+-rw-r--r--   0 dbozh     (1000) dbozh     (1000)      150 2023-08-07 17:52:54.000000 django-permagate-1.0.3/permagate/apps.py
+-rw-r--r--   0 dbozh     (1000) dbozh     (1000)     2876 2023-08-07 17:19:40.000000 django-permagate-1.0.3/permagate/core.py
+drwxr-xr-x   0 dbozh     (1000) dbozh     (1000)        0 2023-08-07 20:00:10.020600 django-permagate-1.0.3/permagate/migrations/
+-rw-r--r--   0 dbozh     (1000) dbozh     (1000)     2543 2023-08-07 19:58:16.000000 django-permagate-1.0.3/permagate/migrations/0001_initial.py
+-rw-r--r--   0 dbozh     (1000) dbozh     (1000)        0 2023-07-24 20:37:50.000000 django-permagate-1.0.3/permagate/migrations/__init__.py
+-rw-r--r--   0 dbozh     (1000) dbozh     (1000)     1152 2023-08-07 19:52:04.000000 django-permagate-1.0.3/permagate/models.py
+-rw-r--r--   0 dbozh     (1000) dbozh     (1000)     7307 2023-08-07 17:03:48.000000 django-permagate-1.0.3/permagate/permission.py
+-rw-r--r--   0 dbozh     (1000) dbozh     (1000)      789 2023-08-07 17:42:18.000000 django-permagate-1.0.3/permagate/test_permissions.py
+-rw-r--r--   0 dbozh     (1000) dbozh     (1000)     4204 2023-08-07 17:52:11.000000 django-permagate-1.0.3/permagate/tests.py
+-rw-r--r--   0 dbozh     (1000) dbozh     (1000)       63 2023-07-24 20:37:50.000000 django-permagate-1.0.3/permagate/views.py
+-rw-r--r--   0 dbozh     (1000) dbozh     (1000)       84 2023-08-07 18:38:18.000000 django-permagate-1.0.3/pyproject.toml
+-rw-r--r--   0 dbozh     (1000) dbozh     (1000)      944 2023-08-07 20:00:10.020600 django-permagate-1.0.3/setup.cfg
+-rw-r--r--   0 dbozh     (1000) dbozh     (1000)       41 2023-08-07 18:34:35.000000 django-permagate-1.0.3/setup.py
```

### Comparing `django-permagate-1.0.2/LICENSE` & `django-permagate-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-permagate-1.0.2/PKG-INFO` & `django-permagate-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-permagate
-Version: 1.0.2
+Version: 1.0.3
 Summary: A permission system for Django
 Home-page: https://github.com/davnov015/django-permagate
 Author: davnov015
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-permagate-1.0.2/README.md` & `django-permagate-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `django-permagate-1.0.2/django_permagate.egg-info/PKG-INFO` & `django-permagate-1.0.3/django_permagate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-permagate
-Version: 1.0.2
+Version: 1.0.3
 Summary: A permission system for Django
 Home-page: https://github.com/davnov015/django-permagate
 Author: davnov015
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-permagate-1.0.2/django_permagate.egg-info/SOURCES.txt` & `django-permagate-1.0.3/django_permagate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-permagate-1.0.2/permagate/core.py` & `django-permagate-1.0.3/permagate/core.py`

 * *Files identical despite different names*

### Comparing `django-permagate-1.0.2/permagate/migrations/0001_initial.py` & `django-permagate-1.0.3/permagate/migrations/0001_initial.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 class Migration(migrations.Migration):
 
     initial = True
 
     dependencies = [
         migrations.swappable_dependency(settings.AUTH_USER_MODEL),
-        ("auth", "0012_alter_user_first_name_max_length"),
+        ("auth", "0009_alter_user_last_name_max_length"),
     ]
 
     operations = [
         migrations.CreateModel(
             name="UserPermission",
             fields=[
                 (
```

### Comparing `django-permagate-1.0.2/permagate/models.py` & `django-permagate-1.0.3/permagate/models.py`

 * *Files identical despite different names*

### Comparing `django-permagate-1.0.2/permagate/permission.py` & `django-permagate-1.0.3/permagate/permission.py`

 * *Files identical despite different names*

### Comparing `django-permagate-1.0.2/permagate/test_permissions.py` & `django-permagate-1.0.3/permagate/test_permissions.py`

 * *Files identical despite different names*

### Comparing `django-permagate-1.0.2/permagate/tests.py` & `django-permagate-1.0.3/permagate/tests.py`

 * *Files identical despite different names*

### Comparing `django-permagate-1.0.2/setup.cfg` & `django-permagate-1.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-permagate
-version = 1.0.2
+version = 1.0.3
 description = A permission system for Django
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/davnov015/django-permagate
 author = davnov015
 license_file = LICENSE
 classifiers =
```

