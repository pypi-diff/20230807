# Comparing `tmp/django-permagate-1.0.1.tar.gz` & `tmp/django-permagate-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-permagate-1.0.1.tar", last modified: Mon Aug  7 19:48:04 2023, max compression
+gzip compressed data, was "django-permagate-1.0.2.tar", last modified: Mon Aug  7 19:53:32 2023, max compression
```

## Comparing `django-permagate-1.0.1.tar` & `django-permagate-1.0.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 dbozh     (1000) dbozh     (1000)        0 2023-08-07 19:48:04.770599 django-permagate-1.0.1/
--rw-r--r--   0 dbozh     (1000) dbozh     (1000)     1066 2023-08-07 18:18:41.000000 django-permagate-1.0.1/LICENSE
--rw-r--r--   0 dbozh     (1000) dbozh     (1000)       83 2023-08-07 18:52:50.000000 django-permagate-1.0.1/MANIFEST.in
--rw-r--r--   0 dbozh     (1000) dbozh     (1000)     4591 2023-08-07 19:48:04.770599 django-permagate-1.0.1/PKG-INFO
--rw-r--r--   0 dbozh     (1000) dbozh     (1000)     3741 2023-08-07 19:45:34.000000 django-permagate-1.0.1/README.md
-drwxr-xr-x   0 dbozh     (1000) dbozh     (1000)        0 2023-08-07 19:48:04.770599 django-permagate-1.0.1/django_permagate.egg-info/
--rw-r--r--   0 dbozh     (1000) dbozh     (1000)     4591 2023-08-07 19:48:04.000000 django-permagate-1.0.1/django_permagate.egg-info/PKG-INFO
--rw-r--r--   0 dbozh     (1000) dbozh     (1000)      521 2023-08-07 19:48:04.000000 django-permagate-1.0.1/django_permagate.egg-info/SOURCES.txt
--rw-r--r--   0 dbozh     (1000) dbozh     (1000)        1 2023-08-07 19:48:04.000000 django-permagate-1.0.1/django_permagate.egg-info/dependency_links.txt
--rw-r--r--   0 dbozh     (1000) dbozh     (1000)       12 2023-08-07 19:48:04.000000 django-permagate-1.0.1/django_permagate.egg-info/requires.txt
--rw-r--r--   0 dbozh     (1000) dbozh     (1000)       27 2023-08-07 19:48:04.000000 django-permagate-1.0.1/django_permagate.egg-info/top_level.txt
-drwxr-xr-x   0 dbozh     (1000) dbozh     (1000)        0 2023-08-07 19:48:04.770599 django-permagate-1.0.1/permagate/
--rw-r--r--   0 dbozh     (1000) dbozh     (1000)        0 2023-08-07 17:54:26.000000 django-permagate-1.0.1/permagate/__init__.py
--rw-r--r--   0 dbozh     (1000) dbozh     (1000)       63 2023-08-03 17:00:47.000000 django-permagate-1.0.1/permagate/admin.py
--rw-r--r--   0 dbozh     (1000) dbozh     (1000)      150 2023-08-07 17:52:54.000000 django-permagate-1.0.1/permagate/apps.py
--rw-r--r--   0 dbozh     (1000) dbozh     (1000)     2876 2023-08-07 17:19:40.000000 django-permagate-1.0.1/permagate/core.py
-drwxr-xr-x   0 dbozh     (1000) dbozh     (1000)        0 2023-08-07 19:48:04.770599 django-permagate-1.0.1/permagate/migrations/
--rw-r--r--   0 dbozh     (1000) dbozh     (1000)     2370 2023-08-07 19:42:04.000000 django-permagate-1.0.1/permagate/migrations/0001_initial.py
--rw-r--r--   0 dbozh     (1000) dbozh     (1000)        0 2023-07-24 20:37:50.000000 django-permagate-1.0.1/permagate/migrations/__init__.py
--rw-r--r--   0 dbozh     (1000) dbozh     (1000)     1120 2023-08-07 19:40:26.000000 django-permagate-1.0.1/permagate/models.py
--rw-r--r--   0 dbozh     (1000) dbozh     (1000)     7307 2023-08-07 17:03:48.000000 django-permagate-1.0.1/permagate/permission.py
--rw-r--r--   0 dbozh     (1000) dbozh     (1000)      789 2023-08-07 17:42:18.000000 django-permagate-1.0.1/permagate/test_permissions.py
--rw-r--r--   0 dbozh     (1000) dbozh     (1000)     4204 2023-08-07 17:52:11.000000 django-permagate-1.0.1/permagate/tests.py
--rw-r--r--   0 dbozh     (1000) dbozh     (1000)       63 2023-07-24 20:37:50.000000 django-permagate-1.0.1/permagate/views.py
--rw-r--r--   0 dbozh     (1000) dbozh     (1000)       84 2023-08-07 18:38:18.000000 django-permagate-1.0.1/pyproject.toml
--rw-r--r--   0 dbozh     (1000) dbozh     (1000)      944 2023-08-07 19:48:04.770599 django-permagate-1.0.1/setup.cfg
--rw-r--r--   0 dbozh     (1000) dbozh     (1000)       41 2023-08-07 18:34:35.000000 django-permagate-1.0.1/setup.py
+drwxr-xr-x   0 dbozh     (1000) dbozh     (1000)        0 2023-08-07 19:53:32.580596 django-permagate-1.0.2/
+-rw-r--r--   0 dbozh     (1000) dbozh     (1000)     1066 2023-08-07 18:18:41.000000 django-permagate-1.0.2/LICENSE
+-rw-r--r--   0 dbozh     (1000) dbozh     (1000)       83 2023-08-07 18:52:50.000000 django-permagate-1.0.2/MANIFEST.in
+-rw-r--r--   0 dbozh     (1000) dbozh     (1000)     4591 2023-08-07 19:53:32.580596 django-permagate-1.0.2/PKG-INFO
+-rw-r--r--   0 dbozh     (1000) dbozh     (1000)     3741 2023-08-07 19:45:34.000000 django-permagate-1.0.2/README.md
+drwxr-xr-x   0 dbozh     (1000) dbozh     (1000)        0 2023-08-07 19:53:32.570596 django-permagate-1.0.2/django_permagate.egg-info/
+-rw-r--r--   0 dbozh     (1000) dbozh     (1000)     4591 2023-08-07 19:53:32.000000 django-permagate-1.0.2/django_permagate.egg-info/PKG-INFO
+-rw-r--r--   0 dbozh     (1000) dbozh     (1000)      521 2023-08-07 19:53:32.000000 django-permagate-1.0.2/django_permagate.egg-info/SOURCES.txt
+-rw-r--r--   0 dbozh     (1000) dbozh     (1000)        1 2023-08-07 19:53:32.000000 django-permagate-1.0.2/django_permagate.egg-info/dependency_links.txt
+-rw-r--r--   0 dbozh     (1000) dbozh     (1000)       12 2023-08-07 19:53:32.000000 django-permagate-1.0.2/django_permagate.egg-info/requires.txt
+-rw-r--r--   0 dbozh     (1000) dbozh     (1000)       27 2023-08-07 19:53:32.000000 django-permagate-1.0.2/django_permagate.egg-info/top_level.txt
+drwxr-xr-x   0 dbozh     (1000) dbozh     (1000)        0 2023-08-07 19:53:32.580596 django-permagate-1.0.2/permagate/
+-rw-r--r--   0 dbozh     (1000) dbozh     (1000)        0 2023-08-07 17:54:26.000000 django-permagate-1.0.2/permagate/__init__.py
+-rw-r--r--   0 dbozh     (1000) dbozh     (1000)       63 2023-08-03 17:00:47.000000 django-permagate-1.0.2/permagate/admin.py
+-rw-r--r--   0 dbozh     (1000) dbozh     (1000)      150 2023-08-07 17:52:54.000000 django-permagate-1.0.2/permagate/apps.py
+-rw-r--r--   0 dbozh     (1000) dbozh     (1000)     2876 2023-08-07 17:19:40.000000 django-permagate-1.0.2/permagate/core.py
+drwxr-xr-x   0 dbozh     (1000) dbozh     (1000)        0 2023-08-07 19:53:32.580596 django-permagate-1.0.2/permagate/migrations/
+-rw-r--r--   0 dbozh     (1000) dbozh     (1000)     2544 2023-08-07 19:53:03.000000 django-permagate-1.0.2/permagate/migrations/0001_initial.py
+-rw-r--r--   0 dbozh     (1000) dbozh     (1000)        0 2023-07-24 20:37:50.000000 django-permagate-1.0.2/permagate/migrations/__init__.py
+-rw-r--r--   0 dbozh     (1000) dbozh     (1000)     1152 2023-08-07 19:52:04.000000 django-permagate-1.0.2/permagate/models.py
+-rw-r--r--   0 dbozh     (1000) dbozh     (1000)     7307 2023-08-07 17:03:48.000000 django-permagate-1.0.2/permagate/permission.py
+-rw-r--r--   0 dbozh     (1000) dbozh     (1000)      789 2023-08-07 17:42:18.000000 django-permagate-1.0.2/permagate/test_permissions.py
+-rw-r--r--   0 dbozh     (1000) dbozh     (1000)     4204 2023-08-07 17:52:11.000000 django-permagate-1.0.2/permagate/tests.py
+-rw-r--r--   0 dbozh     (1000) dbozh     (1000)       63 2023-07-24 20:37:50.000000 django-permagate-1.0.2/permagate/views.py
+-rw-r--r--   0 dbozh     (1000) dbozh     (1000)       84 2023-08-07 18:38:18.000000 django-permagate-1.0.2/pyproject.toml
+-rw-r--r--   0 dbozh     (1000) dbozh     (1000)      944 2023-08-07 19:53:32.580596 django-permagate-1.0.2/setup.cfg
+-rw-r--r--   0 dbozh     (1000) dbozh     (1000)       41 2023-08-07 18:34:35.000000 django-permagate-1.0.2/setup.py
```

### Comparing `django-permagate-1.0.1/LICENSE` & `django-permagate-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-permagate-1.0.1/PKG-INFO` & `django-permagate-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-permagate
-Version: 1.0.1
+Version: 1.0.2
 Summary: A permission system for Django
 Home-page: https://github.com/davnov015/django-permagate
 Author: davnov015
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-permagate-1.0.1/README.md` & `django-permagate-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `django-permagate-1.0.1/django_permagate.egg-info/PKG-INFO` & `django-permagate-1.0.2/django_permagate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-permagate
-Version: 1.0.1
+Version: 1.0.2
 Summary: A permission system for Django
 Home-page: https://github.com/davnov015/django-permagate
 Author: davnov015
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-permagate-1.0.1/django_permagate.egg-info/SOURCES.txt` & `django-permagate-1.0.2/django_permagate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-permagate-1.0.1/permagate/core.py` & `django-permagate-1.0.2/permagate/core.py`

 * *Files identical despite different names*

### Comparing `django-permagate-1.0.1/permagate/migrations/0001_initial.py` & `django-permagate-1.0.2/permagate/migrations/0001_initial.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-# Generated by Django 4.2.3 on 2023-08-07 19:42
+# Generated by Django 4.2.3 on 2023-08-07 19:53
 
 from django.conf import settings
 from django.db import migrations, models
 import django.db.models.deletion
 import permagate.models
 
 
 class Migration(migrations.Migration):
 
     initial = True
 
     dependencies = [
-        ("auth", "0012_alter_user_first_name_max_length"),
         migrations.swappable_dependency(settings.AUTH_USER_MODEL),
+        ("auth", "0012_alter_user_first_name_max_length"),
     ]
 
     operations = [
         migrations.CreateModel(
             name="UserPermission",
             fields=[
                 (
@@ -26,15 +26,18 @@
                         primary_key=True,
                         serialize=False,
                         verbose_name="ID",
                     ),
                 ),
                 (
                     "permission",
-                    models.CharField(validators=[permagate.models.validate_permission]),
+                    models.CharField(
+                        max_length=255,
+                        validators=[permagate.models.validate_permission],
+                    ),
                 ),
                 (
                     "user",
                     models.ForeignKey(
                         on_delete=django.db.models.deletion.CASCADE,
                         related_name="permagate_permissions",
                         to=settings.AUTH_USER_MODEL,
@@ -55,15 +58,18 @@
                         primary_key=True,
                         serialize=False,
                         verbose_name="ID",
                     ),
                 ),
                 (
                     "permission",
-                    models.CharField(validators=[permagate.models.validate_permission]),
+                    models.CharField(
+                        max_length=255,
+                        validators=[permagate.models.validate_permission],
+                    ),
                 ),
                 (
                     "group",
                     models.ForeignKey(
                         on_delete=django.db.models.deletion.CASCADE,
                         related_name="permagate_permissions",
                         to="auth.group",
```

### Comparing `django-permagate-1.0.1/permagate/models.py` & `django-permagate-1.0.2/permagate/models.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,21 +16,21 @@
         )
 
 
 class UserPermission(models.Model):
     user = models.ForeignKey(
         User, on_delete=models.CASCADE, related_name="permagate_permissions"
     )
-    permission = models.CharField(validators=[validate_permission])
+    permission = models.CharField(validators=[validate_permission], max_length=255)
 
     class Meta:
         unique_together = ["user", "permission"]
 
 
 class GroupPermission(models.Model):
     group = models.ForeignKey(
         Group, on_delete=models.CASCADE, related_name="permagate_permissions"
     )
-    permission = models.CharField(validators=[validate_permission])
+    permission = models.CharField(validators=[validate_permission], max_length=255)
 
     class Meta:
         unique_together = ["group", "permission"]
```

### Comparing `django-permagate-1.0.1/permagate/permission.py` & `django-permagate-1.0.2/permagate/permission.py`

 * *Files identical despite different names*

### Comparing `django-permagate-1.0.1/permagate/test_permissions.py` & `django-permagate-1.0.2/permagate/test_permissions.py`

 * *Files identical despite different names*

### Comparing `django-permagate-1.0.1/permagate/tests.py` & `django-permagate-1.0.2/permagate/tests.py`

 * *Files identical despite different names*

### Comparing `django-permagate-1.0.1/setup.cfg` & `django-permagate-1.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-permagate
-version = 1.0.1
+version = 1.0.2
 description = A permission system for Django
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/davnov015/django-permagate
 author = davnov015
 license_file = LICENSE
 classifiers =
```

