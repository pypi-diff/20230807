# Comparing `tmp/wagtail-favicon-0.2.0.tar.gz` & `tmp/wagtail_favicon-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-favicon-0.2.0.tar", max compression
+gzip compressed data, was "wagtail_favicon-0.3.0.tar", max compression
```

## Comparing `wagtail-favicon-0.2.0.tar` & `wagtail_favicon-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rw-r--r--   0        0        0     1515 2021-09-06 03:44:43.548150 wagtail-favicon-0.2.0/README.md
--rw-r--r--   0        0        0      408 2021-09-06 23:39:50.762071 wagtail-favicon-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2021-09-06 23:39:50.762071 wagtail-favicon-0.2.0/wagtail_favicon/__init__.py
--rw-r--r--   0        0        0      104 2021-09-06 03:44:43.548150 wagtail-favicon-0.2.0/wagtail_favicon/apps.py
--rw-r--r--   0        0        0     1646 2021-09-06 03:44:43.548150 wagtail-favicon-0.2.0/wagtail_favicon/migrations/0001_initial.py
--rw-r--r--   0        0        0      573 2021-09-06 03:44:43.548150 wagtail-favicon-0.2.0/wagtail_favicon/migrations/0002_remove_social_sharing_image_setting.py
--rw-r--r--   0        0        0        0 2021-09-06 03:44:43.548150 wagtail-favicon-0.2.0/wagtail_favicon/migrations/__init__.py
--rw-r--r--   0        0        0     2220 2021-09-06 03:44:43.551483 wagtail-favicon-0.2.0/wagtail_favicon/models.py
--rw-r--r--   0        0        0      363 2021-09-06 03:44:43.551483 wagtail-favicon-0.2.0/wagtail_favicon/templates/browser-config.xml
--rw-r--r--   0        0        0      672 2021-09-06 03:44:43.551483 wagtail-favicon-0.2.0/wagtail_favicon/templates/tags/favicon_meta.html
--rw-r--r--   0        0        0      726 2021-09-06 03:44:43.551483 wagtail-favicon-0.2.0/wagtail_favicon/templatetags/favicon_tags.py
--rw-r--r--   0        0        0      180 2021-09-06 03:44:43.551483 wagtail-favicon-0.2.0/wagtail_favicon/urls.py
--rw-r--r--   0        0        0      275 2021-09-06 03:44:43.551483 wagtail-favicon-0.2.0/wagtail_favicon/validators.py
--rw-r--r--   0        0        0     2341 2021-09-06 03:44:43.551483 wagtail-favicon-0.2.0/wagtail_favicon/views.py
--rw-r--r--   0        0        0     2257 2021-09-15 01:26:43.216977 wagtail-favicon-0.2.0/setup.py
--rw-r--r--   0        0        0     2283 2021-09-15 01:26:43.217242 wagtail-favicon-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1489 2023-08-07 02:37:28.543722 wagtail_favicon-0.3.0/README.md
+-rw-r--r--   0        0        0      412 2023-08-07 02:37:28.543722 wagtail_favicon-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-07 00:57:51.783200 wagtail_favicon-0.3.0/wagtail_favicon/__init__.py
+-rw-r--r--   0        0        0      104 2023-08-07 00:57:51.783200 wagtail_favicon-0.3.0/wagtail_favicon/apps.py
+-rw-r--r--   0        0        0     1646 2023-08-07 00:57:51.787200 wagtail_favicon-0.3.0/wagtail_favicon/migrations/0001_initial.py
+-rw-r--r--   0        0        0      573 2023-08-07 00:57:51.787200 wagtail_favicon-0.3.0/wagtail_favicon/migrations/0002_remove_social_sharing_image_setting.py
+-rw-r--r--   0        0        0        0 2023-08-07 00:57:51.787200 wagtail_favicon-0.3.0/wagtail_favicon/migrations/__init__.py
+-rw-r--r--   0        0        0     2155 2023-08-07 02:37:28.543722 wagtail_favicon-0.3.0/wagtail_favicon/models.py
+-rw-r--r--   0        0        0      363 2023-08-07 00:57:51.787200 wagtail_favicon-0.3.0/wagtail_favicon/templates/browser-config.xml
+-rw-r--r--   0        0        0      672 2023-08-07 00:57:51.787200 wagtail_favicon-0.3.0/wagtail_favicon/templates/tags/favicon_meta.html
+-rw-r--r--   0        0        0      723 2023-08-07 02:37:28.543722 wagtail_favicon-0.3.0/wagtail_favicon/templatetags/favicon_tags.py
+-rw-r--r--   0        0        0      182 2023-08-07 02:37:28.543722 wagtail_favicon-0.3.0/wagtail_favicon/urls.py
+-rw-r--r--   0        0        0      276 2023-08-07 02:37:28.543722 wagtail_favicon-0.3.0/wagtail_favicon/validators.py
+-rw-r--r--   0        0        0     2336 2023-08-07 02:37:28.543722 wagtail_favicon-0.3.0/wagtail_favicon/views.py
+-rw-r--r--   0        0        0     2363 1970-01-01 00:00:00.000000 wagtail_favicon-0.3.0/PKG-INFO
```

### Comparing `wagtail-favicon-0.2.0/README.md` & `wagtail_favicon-0.3.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # Wagtail Favicon
 
 Easily add shortcut icons to any wagtail site. Upload a .png image from a wagtail settings page and wagtail-favicon will resize it and add provide markup to your pages via a template tag.
 
+Version 0.3.0 is for Wagtail versions 3+.
+
 ---
 
 ### Installation & Setup
 
 #### Install with pip
 
 ```
@@ -28,22 +30,20 @@
 
 #### Add routes to app.urls
 
 ```
 from wagtail_favicon.urls import urls as favicon_urls
 
 urlpatterns += [
-    url(r'^documents/', include(wagtaildocs_urls)),
-    url(r'^search/$', search, name='search'),
-    url(r'', include(wagtail_urls)),
+    path('documents/', include(wagtaildocs_urls)),
+    path('search/', search, name='search'),
+    path('', include(wagtail_urls)),
 
-    url(r'', include(favicon_urls)),  # <------ add urls to existing urls
+    path('', include(favicon_urls)),  # <------ add urls to existing urls
 ]
-
-# note: newer versions of django may use `path` instead of `url`
 ```
 
 Once you've completed setup you will now be able to access the folloing urls:
 
 - https://example.com/manifest.json
 - https://example.com/browser-config.xml
```

### Comparing `wagtail-favicon-0.2.0/wagtail_favicon/migrations/0001_initial.py` & `wagtail_favicon-0.3.0/wagtail_favicon/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail-favicon-0.2.0/wagtail_favicon/migrations/0002_remove_social_sharing_image_setting.py` & `wagtail_favicon-0.3.0/wagtail_favicon/migrations/0002_remove_social_sharing_image_setting.py`

 * *Files identical despite different names*

### Comparing `wagtail-favicon-0.2.0/wagtail_favicon/models.py` & `wagtail_favicon-0.3.0/wagtail_favicon/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from django.db import models
 from django.utils.functional import cached_property
 
-from wagtail.admin.edit_handlers import MultiFieldPanel, FieldPanel
-from wagtail.contrib.settings.models import BaseSetting, register_setting
+from wagtail.admin.panels import MultiFieldPanel, FieldPanel
+from wagtail.contrib.settings.models import BaseSiteSetting, register_setting
 from wagtail.images import get_image_model_string
-from wagtail.images.edit_handlers import ImageChooserPanel
 
 from .validators import validate_hex
 
 
 class FaviconRenditions:
     icon_sizes = [
         '192x192',
@@ -51,15 +50,15 @@
 
     @cached_property
     def apple_icons(self):
         return self.make_renditions(self.apple_icon_sizes)
 
 
 @register_setting
-class FaviconSettings(BaseSetting, FaviconRenditions):
+class FaviconSettings(BaseSiteSetting, FaviconRenditions):
     base_favicon_image = models.ForeignKey(
         get_image_model_string(),
         null=True,
         blank=True,
         on_delete=models.SET_NULL,
         related_name='+'
     )
@@ -78,15 +77,15 @@
     )
 
     panels = [
         MultiFieldPanel(
             [
                 FieldPanel('app_name'),
                 FieldPanel('app_theme_color'),
-                ImageChooserPanel('base_favicon_image'),
+                FieldPanel('base_favicon_image'),
             ],
             heading="Favicon Settings",
             classname="collapsible"
         ),
     ]
 
     class Meta:
```

### Comparing `wagtail-favicon-0.2.0/wagtail_favicon/templates/tags/favicon_meta.html` & `wagtail_favicon-0.3.0/wagtail_favicon/templates/tags/favicon_meta.html`

 * *Files identical despite different names*

### Comparing `wagtail-favicon-0.2.0/wagtail_favicon/templatetags/favicon_tags.py` & `wagtail_favicon-0.3.0/wagtail_favicon/templatetags/favicon_tags.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from django import template
-from wagtail.core.models import Site
+
+from wagtail.models import Site
 
 from wagtail_favicon.models import FaviconSettings
 
+
 register = template.Library()
 
 
 @register.inclusion_tag('tags/favicon_meta.html', takes_context=True)
 def favicon_meta(context):
     site = Site.find_for_request(context.get('request'))
     favicon_settings = FaviconSettings.for_site(site)
```

### Comparing `wagtail-favicon-0.2.0/wagtail_favicon/views.py` & `wagtail_favicon-0.3.0/wagtail_favicon/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from django.template.response import TemplateResponse
 from django.http import JsonResponse, Http404
-from wagtail.core.models import Site
+from django.template.response import TemplateResponse
+
+from wagtail.models import Site
 
 from .models import FaviconSettings
 
 
 def browser_config(request):
     settings = FaviconSettings.for_site(Site.find_for_request(request))
     image = settings.base_favicon_image
@@ -72,8 +73,7 @@
     if settings.app_name:
         content['name'] = settings.app_name
 
     if settings.app_theme_color:
         content['theme_color'] = settings.app_theme_color
 
     return JsonResponse(content)
-
```

### Comparing `wagtail-favicon-0.2.0/setup.py` & `wagtail_favicon-0.3.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,94 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: wagtail-favicon
+Version: 0.3.0
+Summary: Easily add shortcut icons to any wagtail site.
+Home-page: https://github.com/octavenz/wagtail-favicon
+License: BSD
+Author: Pat Horsley
+Author-email: support@octave.nz
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 2
+Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
 
-packages = \
-['wagtail_favicon',
- 'wagtail_favicon.migrations',
- 'wagtail_favicon.templatetags']
-
-package_data = \
-{'': ['*'], 'wagtail_favicon': ['templates/*', 'templates/tags/*']}
-
-setup_kwargs = {
-    'name': 'wagtail-favicon',
-    'version': '0.2.0',
-    'description': 'Easily add shortcut icons to any wagtail site.',
-    'long_description': "# Wagtail Favicon\n\nEasily add shortcut icons to any wagtail site. Upload a .png image from a wagtail settings page and wagtail-favicon will resize it and add provide markup to your pages via a template tag.\n\n---\n\n### Installation & Setup\n\n#### Install with pip\n\n```\npip install wagtail-favicon\n\nor\n\npoetry add wagtail-favicon\n```\n\n#### Add to Django installed apps\n\n```\nINSTALLED_APPS = [\n    #...\n    'wagtail.contrib.settings'  # <-- ensure you have wagtail settings loaded \n    'wagtail_favicon',\n]\n```\n\n#### Add routes to app.urls\n\n```\nfrom wagtail_favicon.urls import urls as favicon_urls\n\nurlpatterns += [\n    url(r'^documents/', include(wagtaildocs_urls)),\n    url(r'^search/$', search, name='search'),\n    url(r'', include(wagtail_urls)),\n\n    url(r'', include(favicon_urls)),  # <------ add urls to existing urls\n]\n\n# note: newer versions of django may use `path` instead of `url`\n```\n\nOnce you've completed setup you will now be able to access the folloing urls:\n\n- https://example.com/manifest.json\n- https://example.com/browser-config.xml\n\n\n#### Add template tag to <head> tag in templates/base.html\n\n```\n{% load favicon_tags %}\n  <html>\n    <head>\n        {% favicon_meta %}\n    </head>\n```\n\n#### Edit Settings\n\nGo to `Wagtail Admin >> Settings >> Favicon`  \n\nConfigure settings  \n\nFor best results use a transparent png at 1024 x 1024.  \nIdeally pre optimised with a tool like [tinypng.com](https://tinypng.com).\n\n![Screenshot](https://github.com/octavenz/wagtail-favicon/blob/master/screenshot.jpg)\n\n",
-    'author': 'Pat Horsley',
-    'author_email': 'pat@octave.nz',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/octavenz/wagtail-favicon',
-    'packages': packages,
-    'package_data': package_data,
-}
+# Wagtail Favicon
+
+Easily add shortcut icons to any wagtail site. Upload a .png image from a wagtail settings page and wagtail-favicon will resize it and add provide markup to your pages via a template tag.
+
+Version 0.3.0 is for Wagtail versions 3+.
+
+---
+
+### Installation & Setup
+
+#### Install with pip
+
+```
+pip install wagtail-favicon
+
+or
+
+poetry add wagtail-favicon
+```
+
+#### Add to Django installed apps
+
+```
+INSTALLED_APPS = [
+    #...
+    'wagtail.contrib.settings'  # <-- ensure you have wagtail settings loaded 
+    'wagtail_favicon',
+]
+```
+
+#### Add routes to app.urls
+
+```
+from wagtail_favicon.urls import urls as favicon_urls
+
+urlpatterns += [
+    path('documents/', include(wagtaildocs_urls)),
+    path('search/', search, name='search'),
+    path('', include(wagtail_urls)),
+
+    path('', include(favicon_urls)),  # <------ add urls to existing urls
+]
+```
+
+Once you've completed setup you will now be able to access the folloing urls:
+
+- https://example.com/manifest.json
+- https://example.com/browser-config.xml
+
+
+#### Add template tag to <head> tag in templates/base.html
+
+```
+{% load favicon_tags %}
+  <html>
+    <head>
+        {% favicon_meta %}
+    </head>
+```
+
+#### Edit Settings
+
+Go to `Wagtail Admin >> Settings >> Favicon`  
+
+Configure settings  
+
+For best results use a transparent png at 1024 x 1024.  
+Ideally pre optimised with a tool like [tinypng.com](https://tinypng.com).
+
+![Screenshot](https://github.com/octavenz/wagtail-favicon/blob/master/screenshot.jpg)
 
 
-setup(**setup_kwargs)
```

