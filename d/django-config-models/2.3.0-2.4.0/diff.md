# Comparing `tmp/django-config-models-2.3.0.tar.gz` & `tmp/django-config-models-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-config-models-2.3.0.tar", last modified: Thu Jan 20 10:47:05 2022, max compression
+gzip compressed data, was "django-config-models-2.4.0.tar", last modified: Mon Jul 24 07:38:04 2023, max compression
```

## Comparing `django-config-models-2.3.0.tar` & `django-config-models-2.4.0.tar`

### file list

```diff
@@ -1,37 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-20 10:47:05.441147 django-config-models-2.3.0/
--rw-r--r--   0 runner    (1001) docker     (121)      428 2022-01-20 10:47:02.000000 django-config-models-2.3.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (121)     4160 2022-01-20 10:47:02.000000 django-config-models-2.3.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)    35119 2022-01-20 10:47:02.000000 django-config-models-2.3.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      249 2022-01-20 10:47:02.000000 django-config-models-2.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     8521 2022-01-20 10:47:05.445147 django-config-models-2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3579 2022-01-20 10:47:02.000000 django-config-models-2.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-20 10:47:05.441147 django-config-models-2.3.0/config_models/
--rw-r--r--   0 runner    (1001) docker     (121)      199 2022-01-20 10:47:02.000000 django-config-models-2.3.0/config_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8007 2022-01-20 10:47:02.000000 django-config-models-2.3.0/config_models/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)      235 2022-01-20 10:47:02.000000 django-config-models-2.3.0/config_models/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)      918 2022-01-20 10:47:02.000000 django-config-models-2.3.0/config_models/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-20 10:47:05.441147 django-config-models-2.3.0/config_models/management/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-20 10:47:02.000000 django-config-models-2.3.0/config_models/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-20 10:47:05.441147 django-config-models-2.3.0/config_models/management/commands/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-20 10:47:02.000000 django-config-models-2.3.0/config_models/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2456 2022-01-20 10:47:02.000000 django-config-models-2.3.0/config_models/management/commands/populate_model.py
--rw-r--r--   0 runner    (1001) docker     (121)    10393 2022-01-20 10:47:02.000000 django-config-models-2.3.0/config_models/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-20 10:47:05.441147 django-config-models-2.3.0/config_models/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-20 10:47:05.441147 django-config-models-2.3.0/config_models/templates/config_models/
--rw-r--r--   0 runner    (1001) docker     (121)      662 2022-01-20 10:47:02.000000 django-config-models-2.3.0/config_models/templates/config_models/base.html
--rw-r--r--   0 runner    (1001) docker     (121)      980 2022-01-20 10:47:02.000000 django-config-models-2.3.0/config_models/templatetags.py
--rw-r--r--   0 runner    (1001) docker     (121)      209 2022-01-20 10:47:02.000000 django-config-models-2.3.0/config_models/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)     2583 2022-01-20 10:47:02.000000 django-config-models-2.3.0/config_models/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2612 2022-01-20 10:47:02.000000 django-config-models-2.3.0/config_models/views.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-20 10:47:05.441147 django-config-models-2.3.0/django_config_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8521 2022-01-20 10:47:05.000000 django-config-models-2.3.0/django_config_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      791 2022-01-20 10:47:05.000000 django-config-models-2.3.0/django_config_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-20 10:47:05.000000 django-config-models-2.3.0/django_config_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-20 10:47:05.000000 django-config-models-2.3.0/django_config_models.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-01-20 10:47:05.000000 django-config-models-2.3.0/django_config_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-01-20 10:47:05.000000 django-config-models-2.3.0/django_config_models.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-20 10:47:05.441147 django-config-models-2.3.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (121)      165 2022-01-20 10:47:02.000000 django-config-models-2.3.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (121)      561 2022-01-20 10:47:02.000000 django-config-models-2.3.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-01-20 10:47:05.445147 django-config-models-2.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     5188 2022-01-20 10:47:02.000000 django-config-models-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 07:38:04.564940 django-config-models-2.4.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      428 2023-07-24 07:37:58.000000 django-config-models-2.4.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (122)     4258 2023-07-24 07:37:58.000000 django-config-models-2.4.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    35119 2023-07-24 07:37:58.000000 django-config-models-2.4.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      249 2023-07-24 07:37:58.000000 django-config-models-2.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    10884 2023-07-24 07:38:04.564940 django-config-models-2.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5860 2023-07-24 07:37:58.000000 django-config-models-2.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 07:38:04.564940 django-config-models-2.4.0/config_models/
+-rw-r--r--   0 runner    (1001) docker     (122)      105 2023-07-24 07:37:58.000000 django-config-models-2.4.0/config_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7978 2023-07-24 07:37:58.000000 django-config-models-2.4.0/config_models/admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)      235 2023-07-24 07:37:58.000000 django-config-models-2.4.0/config_models/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)      918 2023-07-24 07:37:58.000000 django-config-models-2.4.0/config_models/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 07:38:04.564940 django-config-models-2.4.0/config_models/management/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-24 07:37:58.000000 django-config-models-2.4.0/config_models/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 07:38:04.564940 django-config-models-2.4.0/config_models/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-24 07:37:58.000000 django-config-models-2.4.0/config_models/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2456 2023-07-24 07:37:58.000000 django-config-models-2.4.0/config_models/management/commands/populate_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10391 2023-07-24 07:37:58.000000 django-config-models-2.4.0/config_models/models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 07:38:04.560940 django-config-models-2.4.0/config_models/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 07:38:04.564940 django-config-models-2.4.0/config_models/templates/config_models/
+-rw-r--r--   0 runner    (1001) docker     (122)      662 2023-07-24 07:37:58.000000 django-config-models-2.4.0/config_models/templates/config_models/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)      980 2023-07-24 07:37:58.000000 django-config-models-2.4.0/config_models/templatetags.py
+-rw-r--r--   0 runner    (1001) docker     (122)      209 2023-07-24 07:37:58.000000 django-config-models-2.4.0/config_models/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2583 2023-07-24 07:37:58.000000 django-config-models-2.4.0/config_models/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2612 2023-07-24 07:37:58.000000 django-config-models-2.4.0/config_models/views.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 07:38:04.564940 django-config-models-2.4.0/django_config_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    10884 2023-07-24 07:38:04.000000 django-config-models-2.4.0/django_config_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      900 2023-07-24 07:38:04.000000 django-config-models-2.4.0/django_config_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-24 07:38:04.000000 django-config-models-2.4.0/django_config_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-24 07:38:04.000000 django-config-models-2.4.0/django_config_models.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       49 2023-07-24 07:38:04.000000 django-config-models-2.4.0/django_config_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       14 2023-07-24 07:38:04.000000 django-config-models-2.4.0/django_config_models.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 07:38:04.564940 django-config-models-2.4.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      165 2023-07-24 07:37:58.000000 django-config-models-2.4.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      561 2023-07-24 07:37:58.000000 django-config-models-2.4.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-24 07:38:04.568940 django-config-models-2.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     5192 2023-07-24 07:37:58.000000 django-config-models-2.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 07:38:04.564940 django-config-models-2.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     2904 2023-07-24 07:37:58.000000 django-config-models-2.4.0/tests/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17700 2023-07-24 07:37:58.000000 django-config-models-2.4.0/tests/test_config_models.py
+-rw-r--r--   0 runner    (1001) docker     (122)      899 2023-07-24 07:37:58.000000 django-config-models-2.4.0/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7989 2023-07-24 07:37:58.000000 django-config-models-2.4.0/tests/test_model_deserialization.py
```

### Comparing `django-config-models-2.3.0/CHANGELOG.rst` & `django-config-models-2.4.0/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,17 @@
    This project adheres to Semantic Versioning (http://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
 
+* Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
+  deprecated
+
 [2.3.0] - 2022-01-19
 ~~~~~~~~~~~~~~~~~~~~
 * Added Support for Django40 in CI
 * Dropped Support for Django22, 30, 31
 
 [2.2.2] - 2021-20-12
 ~~~~~~~~~~~~~~~~~~~~
@@ -57,15 +60,15 @@
 ~~~~~~~~~~~~~~~~~~~~
 * Dropping support for Python 2.7
 * Switch to using edx-django-utils TieredCache (a two-layer cache that uses both
   Django's cache and an internal request-level cache) to reduce the number of
   memcached roundtrips. This was a major performance issue that accounted for
   10-20% of transaction time for certain courseware views in edx-platform.
 * It is now REQUIRED to add `RequestCacheMiddleware` `to middleware
-  <https://github.com/edx/edx-django-utils/tree/master/edx_django_utils/cache#tieredcachemiddleware>`_
+  <https://github.com/openedx/edx-django-utils/tree/master/edx_django_utils/cache#tieredcachemiddleware>`_
   to use ConfigModels.
 * Remove usage of the "configuration" cache setting. ConfigModels now always use
   the default Django cache.
 * Django Rest Framework 3.7 and 3.8 are no longer supported.
 
 [1.0.1] - 2019-04-23
 ~~~~~~~~~~~~~~~~~~~~
```

### Comparing `django-config-models-2.3.0/LICENSE.txt` & `django-config-models-2.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-config-models-2.3.0/config_models/admin.py` & `django-config-models-2.4.0/config_models/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,18 +193,19 @@
                     if request.POST.get(clear_checkbox_name) != 'on':
                         request.FILES.setdefault(field_name, field_value)
                 get[field_name] = field_value
             request.GET = get
         # Call our grandparent's add_view, skipping the parent code
         # because the parent code has a different way to prepopulate new configuration entries
         # with the value of the latest config, which doesn't make sense for keyed models.
-        # pylint: disable=bad-super-call
         return super(ConfigurationModelAdmin, self).add_view(request, form_url, extra_context)
 
+    @admin.display(
+        description=_('Update')
+    )
     def edit_link(self, inst):
         """ Edit link for the change view """
         if not inst.is_active:
             return '--'
         update_url = reverse(f'admin:{self.model._meta.app_label}_{self.model._meta.model_name}_add')
         update_url += f"?source={inst.pk}"
         return format_html('<a href="{}">{}</a>', update_url, _('Update'))
-    edit_link.short_description = _('Update')
```

### Comparing `django-config-models-2.3.0/config_models/decorators.py` & `django-config-models-2.4.0/config_models/decorators.py`

 * *Files identical despite different names*

### Comparing `django-config-models-2.3.0/config_models/management/commands/populate_model.py` & `django-config-models-2.4.0/config_models/management/commands/populate_model.py`

 * *Files identical despite different names*

### Comparing `django-config-models-2.3.0/config_models/models.py` & `django-config-models-2.4.0/config_models/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
         TieredCache.delete_all_tiers(self.cache_key_name(*[getattr(self, key) for key in self.KEY_FIELDS]))
         if self.KEY_FIELDS:
             TieredCache.delete_all_tiers(self.key_values_cache_key_name())
 
     @classmethod
     def cache_key_name(cls, *args):
         """Return the name of the key to use to cache the current configuration"""
-        if cls.KEY_FIELDS != ():    # pylint: disable=use-implicit-booleaness-not-comparison
+        if cls.KEY_FIELDS != ():  # pylint: disable=use-implicit-booleaness-not-comparison
             if len(args) != len(cls.KEY_FIELDS):
                 raise TypeError(
                     f"cache_key_name() takes exactly {len(cls.KEY_FIELDS)} arguments ({len(args)} given)"
                 )
             return f"configuration/{cls.__name__}/current/{','.join(str(arg) for arg in args)}"
         else:
             return f'configuration/{cls.__name__}/current'
```

### Comparing `django-config-models-2.3.0/config_models/templates/config_models/base.html` & `django-config-models-2.4.0/config_models/templates/config_models/base.html`

 * *Files identical despite different names*

### Comparing `django-config-models-2.3.0/config_models/templatetags.py` & `django-config-models-2.4.0/config_models/templatetags.py`

 * *Files identical despite different names*

### Comparing `django-config-models-2.3.0/config_models/utils.py` & `django-config-models-2.4.0/config_models/utils.py`

 * *Files identical despite different names*

### Comparing `django-config-models-2.3.0/config_models/views.py` & `django-config-models-2.4.0/config_models/views.py`

 * *Files identical despite different names*

### Comparing `django-config-models-2.3.0/requirements/constraints.txt` & `django-config-models-2.4.0/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `django-config-models-2.3.0/setup.py` & `django-config-models-2.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,28 +101,28 @@
 setup(
     name='django-config-models',
     version=VERSION,
     description="""Configuration models for Django allowing config management with auditing.""",
     long_description=README + '\n\n' + CHANGELOG,
     author='edX',
     author_email='oscm@edx.org',
-    url='https://github.com/edx/django-config-models',
+    url='https://github.com/openedx/django-config-models',
     packages=[
         'config_models',
     ],
     include_package_data=True,
     install_requires=load_requirements('requirements/base.in'),
     license="AGPL 3.0",
     zip_safe=False,
     keywords='Django edx',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Framework :: Django',
         'Framework :: Django :: 3.2',
-        'Framework :: Django :: 4.0',
+        'Framework :: Django :: 4.2',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
     ],
 )
```

