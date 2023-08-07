# Comparing `tmp/django-permagate-1.0.0.tar.gz` & `tmp/django-permagate-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-permagate-1.0.0.tar", last modified: Mon Aug  7 19:11:55 2023, max compression
+gzip compressed data, was "django-permagate-1.0.1.tar", last modified: Mon Aug  7 19:48:04 2023, max compression
```

## Comparing `django-permagate-1.0.0.tar` & `django-permagate-1.0.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 dbozh     (1000) dbozh     (1000)        0 2023-08-07 19:11:55.710601 django-permagate-1.0.0/
--rw-r--r--   0 dbozh     (1000) dbozh     (1000)     1066 2023-08-07 18:18:41.000000 django-permagate-1.0.0/LICENSE
--rw-r--r--   0 dbozh     (1000) dbozh     (1000)       83 2023-08-07 18:52:50.000000 django-permagate-1.0.0/MANIFEST.in
--rw-r--r--   0 dbozh     (1000) dbozh     (1000)     4608 2023-08-07 19:11:55.710601 django-permagate-1.0.0/PKG-INFO
--rw-r--r--   0 dbozh     (1000) dbozh     (1000)     3758 2023-08-07 18:06:09.000000 django-permagate-1.0.0/README.md
-drwxr-xr-x   0 dbozh     (1000) dbozh     (1000)        0 2023-08-07 19:11:55.710601 django-permagate-1.0.0/django_permagate.egg-info/
--rw-r--r--   0 dbozh     (1000) dbozh     (1000)     4608 2023-08-07 19:11:55.000000 django-permagate-1.0.0/django_permagate.egg-info/PKG-INFO
--rw-r--r--   0 dbozh     (1000) dbozh     (1000)      521 2023-08-07 19:11:55.000000 django-permagate-1.0.0/django_permagate.egg-info/SOURCES.txt
--rw-r--r--   0 dbozh     (1000) dbozh     (1000)        1 2023-08-07 19:11:55.000000 django-permagate-1.0.0/django_permagate.egg-info/dependency_links.txt
--rw-r--r--   0 dbozh     (1000) dbozh     (1000)       12 2023-08-07 19:11:55.000000 django-permagate-1.0.0/django_permagate.egg-info/requires.txt
--rw-r--r--   0 dbozh     (1000) dbozh     (1000)       27 2023-08-07 19:11:55.000000 django-permagate-1.0.0/django_permagate.egg-info/top_level.txt
-drwxr-xr-x   0 dbozh     (1000) dbozh     (1000)        0 2023-08-07 19:11:55.710601 django-permagate-1.0.0/permagate/
--rw-r--r--   0 dbozh     (1000) dbozh     (1000)        0 2023-08-07 17:54:26.000000 django-permagate-1.0.0/permagate/__init__.py
--rw-r--r--   0 dbozh     (1000) dbozh     (1000)       63 2023-08-03 17:00:47.000000 django-permagate-1.0.0/permagate/admin.py
--rw-r--r--   0 dbozh     (1000) dbozh     (1000)      150 2023-08-07 17:52:54.000000 django-permagate-1.0.0/permagate/apps.py
--rw-r--r--   0 dbozh     (1000) dbozh     (1000)     2876 2023-08-07 17:19:40.000000 django-permagate-1.0.0/permagate/core.py
-drwxr-xr-x   0 dbozh     (1000) dbozh     (1000)        0 2023-08-07 19:11:55.710601 django-permagate-1.0.0/permagate/migrations/
--rw-r--r--   0 dbozh     (1000) dbozh     (1000)     2628 2023-08-07 17:10:04.000000 django-permagate-1.0.0/permagate/migrations/0001_initial.py
--rw-r--r--   0 dbozh     (1000) dbozh     (1000)        0 2023-07-24 20:37:50.000000 django-permagate-1.0.0/permagate/migrations/__init__.py
--rw-r--r--   0 dbozh     (1000) dbozh     (1000)     1347 2023-08-07 17:09:15.000000 django-permagate-1.0.0/permagate/models.py
--rw-r--r--   0 dbozh     (1000) dbozh     (1000)     7307 2023-08-07 17:03:48.000000 django-permagate-1.0.0/permagate/permission.py
--rw-r--r--   0 dbozh     (1000) dbozh     (1000)      789 2023-08-07 17:42:18.000000 django-permagate-1.0.0/permagate/test_permissions.py
--rw-r--r--   0 dbozh     (1000) dbozh     (1000)     4204 2023-08-07 17:52:11.000000 django-permagate-1.0.0/permagate/tests.py
--rw-r--r--   0 dbozh     (1000) dbozh     (1000)       63 2023-07-24 20:37:50.000000 django-permagate-1.0.0/permagate/views.py
--rw-r--r--   0 dbozh     (1000) dbozh     (1000)       84 2023-08-07 18:38:18.000000 django-permagate-1.0.0/pyproject.toml
--rw-r--r--   0 dbozh     (1000) dbozh     (1000)      944 2023-08-07 19:11:55.710601 django-permagate-1.0.0/setup.cfg
--rw-r--r--   0 dbozh     (1000) dbozh     (1000)       41 2023-08-07 18:34:35.000000 django-permagate-1.0.0/setup.py
+drwxr-xr-x   0 dbozh     (1000) dbozh     (1000)        0 2023-08-07 19:48:04.770599 django-permagate-1.0.1/
+-rw-r--r--   0 dbozh     (1000) dbozh     (1000)     1066 2023-08-07 18:18:41.000000 django-permagate-1.0.1/LICENSE
+-rw-r--r--   0 dbozh     (1000) dbozh     (1000)       83 2023-08-07 18:52:50.000000 django-permagate-1.0.1/MANIFEST.in
+-rw-r--r--   0 dbozh     (1000) dbozh     (1000)     4591 2023-08-07 19:48:04.770599 django-permagate-1.0.1/PKG-INFO
+-rw-r--r--   0 dbozh     (1000) dbozh     (1000)     3741 2023-08-07 19:45:34.000000 django-permagate-1.0.1/README.md
+drwxr-xr-x   0 dbozh     (1000) dbozh     (1000)        0 2023-08-07 19:48:04.770599 django-permagate-1.0.1/django_permagate.egg-info/
+-rw-r--r--   0 dbozh     (1000) dbozh     (1000)     4591 2023-08-07 19:48:04.000000 django-permagate-1.0.1/django_permagate.egg-info/PKG-INFO
+-rw-r--r--   0 dbozh     (1000) dbozh     (1000)      521 2023-08-07 19:48:04.000000 django-permagate-1.0.1/django_permagate.egg-info/SOURCES.txt
+-rw-r--r--   0 dbozh     (1000) dbozh     (1000)        1 2023-08-07 19:48:04.000000 django-permagate-1.0.1/django_permagate.egg-info/dependency_links.txt
+-rw-r--r--   0 dbozh     (1000) dbozh     (1000)       12 2023-08-07 19:48:04.000000 django-permagate-1.0.1/django_permagate.egg-info/requires.txt
+-rw-r--r--   0 dbozh     (1000) dbozh     (1000)       27 2023-08-07 19:48:04.000000 django-permagate-1.0.1/django_permagate.egg-info/top_level.txt
+drwxr-xr-x   0 dbozh     (1000) dbozh     (1000)        0 2023-08-07 19:48:04.770599 django-permagate-1.0.1/permagate/
+-rw-r--r--   0 dbozh     (1000) dbozh     (1000)        0 2023-08-07 17:54:26.000000 django-permagate-1.0.1/permagate/__init__.py
+-rw-r--r--   0 dbozh     (1000) dbozh     (1000)       63 2023-08-03 17:00:47.000000 django-permagate-1.0.1/permagate/admin.py
+-rw-r--r--   0 dbozh     (1000) dbozh     (1000)      150 2023-08-07 17:52:54.000000 django-permagate-1.0.1/permagate/apps.py
+-rw-r--r--   0 dbozh     (1000) dbozh     (1000)     2876 2023-08-07 17:19:40.000000 django-permagate-1.0.1/permagate/core.py
+drwxr-xr-x   0 dbozh     (1000) dbozh     (1000)        0 2023-08-07 19:48:04.770599 django-permagate-1.0.1/permagate/migrations/
+-rw-r--r--   0 dbozh     (1000) dbozh     (1000)     2370 2023-08-07 19:42:04.000000 django-permagate-1.0.1/permagate/migrations/0001_initial.py
+-rw-r--r--   0 dbozh     (1000) dbozh     (1000)        0 2023-07-24 20:37:50.000000 django-permagate-1.0.1/permagate/migrations/__init__.py
+-rw-r--r--   0 dbozh     (1000) dbozh     (1000)     1120 2023-08-07 19:40:26.000000 django-permagate-1.0.1/permagate/models.py
+-rw-r--r--   0 dbozh     (1000) dbozh     (1000)     7307 2023-08-07 17:03:48.000000 django-permagate-1.0.1/permagate/permission.py
+-rw-r--r--   0 dbozh     (1000) dbozh     (1000)      789 2023-08-07 17:42:18.000000 django-permagate-1.0.1/permagate/test_permissions.py
+-rw-r--r--   0 dbozh     (1000) dbozh     (1000)     4204 2023-08-07 17:52:11.000000 django-permagate-1.0.1/permagate/tests.py
+-rw-r--r--   0 dbozh     (1000) dbozh     (1000)       63 2023-07-24 20:37:50.000000 django-permagate-1.0.1/permagate/views.py
+-rw-r--r--   0 dbozh     (1000) dbozh     (1000)       84 2023-08-07 18:38:18.000000 django-permagate-1.0.1/pyproject.toml
+-rw-r--r--   0 dbozh     (1000) dbozh     (1000)      944 2023-08-07 19:48:04.770599 django-permagate-1.0.1/setup.cfg
+-rw-r--r--   0 dbozh     (1000) dbozh     (1000)       41 2023-08-07 18:34:35.000000 django-permagate-1.0.1/setup.py
```

### Comparing `django-permagate-1.0.0/LICENSE` & `django-permagate-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-permagate-1.0.0/PKG-INFO` & `django-permagate-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-permagate
-Version: 1.0.0
+Version: 1.0.1
 Summary: A permission system for Django
 Home-page: https://github.com/davnov015/django-permagate
 Author: davnov015
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -32,19 +32,19 @@
 # Installation
 
 1. ```pip install django-permagate``` to install the package
 2. ```python 
    # Add it to the list of installed apps in Django's settings.py:
    INSTALLED_APPS = [
         ...,
-        "django-permagate",
+        "permagate",
    ]
    ```
 3. ```python manage.py migrate``` to create the permission models
-4. Set the ```PERMAGATE_PERMISSIONS``` environmental variable to the module defining the root permission (see below)
+4. Set the ```PERMAGATE_PERMISSIONS``` settings variable to the module defining the root permission (see below)
 
 # Usage
 
 ## Defining Permissions
 
 The list of permissions that may be assigned to users and groups is defined using the 
 Permission class. A root permission object is used as the starting point of the permission
@@ -75,15 +75,15 @@
 # 'test.sub2', 
 # 'test1']
 #
 # This is the list of permission strings that may be assigned to users and groups.
 
 ```
 
-The environmental variable ```PERMAGATE_PERMISSIONS``` should be set to the path of the 
+The settings variable ```PERMAGATE_PERMISSIONS``` should be set to the path of the 
 module defining the root permission variable:
 ```python
 # Assuming there's a permissions.py file in mymodule containing a variable named 'root' 
 # that contains the root permission:
 PERMAGATE_PERMISSIONS = "mymodule.permissions"
 ```
```

### Comparing `django-permagate-1.0.0/README.md` & `django-permagate-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 # Installation
 
 1. ```pip install django-permagate``` to install the package
 2. ```python 
    # Add it to the list of installed apps in Django's settings.py:
    INSTALLED_APPS = [
         ...,
-        "django-permagate",
+        "permagate",
    ]
    ```
 3. ```python manage.py migrate``` to create the permission models
-4. Set the ```PERMAGATE_PERMISSIONS``` environmental variable to the module defining the root permission (see below)
+4. Set the ```PERMAGATE_PERMISSIONS``` settings variable to the module defining the root permission (see below)
 
 # Usage
 
 ## Defining Permissions
 
 The list of permissions that may be assigned to users and groups is defined using the 
 Permission class. A root permission object is used as the starting point of the permission
@@ -49,15 +49,15 @@
 # 'test.sub2', 
 # 'test1']
 #
 # This is the list of permission strings that may be assigned to users and groups.
 
 ```
 
-The environmental variable ```PERMAGATE_PERMISSIONS``` should be set to the path of the 
+The settings variable ```PERMAGATE_PERMISSIONS``` should be set to the path of the 
 module defining the root permission variable:
 ```python
 # Assuming there's a permissions.py file in mymodule containing a variable named 'root' 
 # that contains the root permission:
 PERMAGATE_PERMISSIONS = "mymodule.permissions"
 ```
```

### Comparing `django-permagate-1.0.0/django_permagate.egg-info/PKG-INFO` & `django-permagate-1.0.1/django_permagate.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-permagate
-Version: 1.0.0
+Version: 1.0.1
 Summary: A permission system for Django
 Home-page: https://github.com/davnov015/django-permagate
 Author: davnov015
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -32,19 +32,19 @@
 # Installation
 
 1. ```pip install django-permagate``` to install the package
 2. ```python 
    # Add it to the list of installed apps in Django's settings.py:
    INSTALLED_APPS = [
         ...,
-        "django-permagate",
+        "permagate",
    ]
    ```
 3. ```python manage.py migrate``` to create the permission models
-4. Set the ```PERMAGATE_PERMISSIONS``` environmental variable to the module defining the root permission (see below)
+4. Set the ```PERMAGATE_PERMISSIONS``` settings variable to the module defining the root permission (see below)
 
 # Usage
 
 ## Defining Permissions
 
 The list of permissions that may be assigned to users and groups is defined using the 
 Permission class. A root permission object is used as the starting point of the permission
@@ -75,15 +75,15 @@
 # 'test.sub2', 
 # 'test1']
 #
 # This is the list of permission strings that may be assigned to users and groups.
 
 ```
 
-The environmental variable ```PERMAGATE_PERMISSIONS``` should be set to the path of the 
+The settings variable ```PERMAGATE_PERMISSIONS``` should be set to the path of the 
 module defining the root permission variable:
 ```python
 # Assuming there's a permissions.py file in mymodule containing a variable named 'root' 
 # that contains the root permission:
 PERMAGATE_PERMISSIONS = "mymodule.permissions"
 ```
```

### Comparing `django-permagate-1.0.0/django_permagate.egg-info/SOURCES.txt` & `django-permagate-1.0.1/django_permagate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-permagate-1.0.0/permagate/core.py` & `django-permagate-1.0.1/permagate/core.py`

 * *Files identical despite different names*

### Comparing `django-permagate-1.0.0/permagate/migrations/0001_initial.py` & `django-permagate-1.0.1/permagate/migrations/0001_initial.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-# Generated by Django 4.2.3 on 2023-08-07 17:10
+# Generated by Django 4.2.3 on 2023-08-07 19:42
 
 from django.conf import settings
 from django.db import migrations, models
 import django.db.models.deletion
 import permagate.models
 
 
 class Migration(migrations.Migration):
 
     initial = True
 
     dependencies = [
-        migrations.swappable_dependency(settings.AUTH_USER_MODEL),
         ("auth", "0012_alter_user_first_name_max_length"),
+        migrations.swappable_dependency(settings.AUTH_USER_MODEL),
     ]
 
     operations = [
         migrations.CreateModel(
             name="UserPermission",
             fields=[
                 (
@@ -37,14 +37,17 @@
                     models.ForeignKey(
                         on_delete=django.db.models.deletion.CASCADE,
                         related_name="permagate_permissions",
                         to=settings.AUTH_USER_MODEL,
                     ),
                 ),
             ],
+            options={
+                "unique_together": {("user", "permission")},
+            },
         ),
         migrations.CreateModel(
             name="GroupPermission",
             fields=[
                 (
                     "id",
                     models.BigAutoField(
@@ -63,21 +66,12 @@
                     models.ForeignKey(
                         on_delete=django.db.models.deletion.CASCADE,
                         related_name="permagate_permissions",
                         to="auth.group",
                     ),
                 ),
             ],
-        ),
-        migrations.AddConstraint(
-            model_name="userpermission",
-            constraint=models.UniqueConstraint(
-                fields=("user", "permission"), name="unique_user_permission"
-            ),
-        ),
-        migrations.AddConstraint(
-            model_name="grouppermission",
-            constraint=models.UniqueConstraint(
-                fields=("group", "permission"), name="unique_group_constraint"
-            ),
+            options={
+                "unique_together": {("group", "permission")},
+            },
         ),
     ]
```

### Comparing `django-permagate-1.0.0/permagate/models.py` & `django-permagate-1.0.1/permagate/models.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,26 +19,18 @@
 class UserPermission(models.Model):
     user = models.ForeignKey(
         User, on_delete=models.CASCADE, related_name="permagate_permissions"
     )
     permission = models.CharField(validators=[validate_permission])
 
     class Meta:
-        constraints = [
-            models.UniqueConstraint(
-                fields=["user", "permission"], name="unique_user_permission"
-            )
-        ]
+        unique_together = ["user", "permission"]
 
 
 class GroupPermission(models.Model):
     group = models.ForeignKey(
         Group, on_delete=models.CASCADE, related_name="permagate_permissions"
     )
     permission = models.CharField(validators=[validate_permission])
 
     class Meta:
-        constraints = [
-            models.UniqueConstraint(
-                fields=["group", "permission"], name="unique_group_constraint"
-            )
-        ]
+        unique_together = ["group", "permission"]
```

### Comparing `django-permagate-1.0.0/permagate/permission.py` & `django-permagate-1.0.1/permagate/permission.py`

 * *Files identical despite different names*

### Comparing `django-permagate-1.0.0/permagate/test_permissions.py` & `django-permagate-1.0.1/permagate/test_permissions.py`

 * *Files identical despite different names*

### Comparing `django-permagate-1.0.0/permagate/tests.py` & `django-permagate-1.0.1/permagate/tests.py`

 * *Files identical despite different names*

### Comparing `django-permagate-1.0.0/setup.cfg` & `django-permagate-1.0.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-permagate
-version = 1.0.0
+version = 1.0.1
 description = A permission system for Django
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/davnov015/django-permagate
 author = davnov015
 license_file = LICENSE
 classifiers =
```

