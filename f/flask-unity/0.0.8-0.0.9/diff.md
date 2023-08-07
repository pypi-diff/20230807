# Comparing `tmp/flask_unity-0.0.8.tar.gz` & `tmp/flask_unity-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_unity-0.0.8.tar", last modified: Sun Aug  6 23:08:35 2023, max compression
+gzip compressed data, was "flask_unity-0.0.9.tar", last modified: Sun Aug  6 23:10:36 2023, max compression
```

## Comparing `flask_unity-0.0.8.tar` & `flask_unity-0.0.9.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-08-06 23:08:35.942905 flask_unity-0.0.8/
--rw-rw-r--   0 usman     (1000) usman     (1000)     1279 2023-08-06 23:08:30.000000 flask_unity-0.0.8/CHANGELOG
--rw-rw-r--   0 usman     (1000) usman     (1000)     1077 2023-08-05 06:53:20.000000 flask_unity-0.0.8/LICENSE
--rw-rw-r--   0 usman     (1000) usman     (1000)       82 2023-08-06 06:39:07.000000 flask_unity-0.0.8/MANIFEST.in
--rw-rw-r--   0 usman     (1000) usman     (1000)     5941 2023-08-06 23:08:35.942905 flask_unity-0.0.8/PKG-INFO
--rw-rw-r--   0 usman     (1000) usman     (1000)     3494 2023-08-06 23:08:30.000000 flask_unity-0.0.8/README.md
-drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-08-06 23:08:35.882917 flask_unity-0.0.8/flask_unity/
--rw-rw-r--   0 usman     (1000) usman     (1000)      879 2023-08-06 23:08:30.000000 flask_unity-0.0.8/flask_unity/__init__.py
--rw-rw-r--   0 usman     (1000) usman     (1000)      489 2023-08-06 23:08:30.000000 flask_unity-0.0.8/flask_unity/api.py
-drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-08-06 23:08:35.898913 flask_unity-0.0.8/flask_unity/auth/
--rw-rw-r--   0 usman     (1000) usman     (1000)       46 2023-08-06 23:08:30.000000 flask_unity-0.0.8/flask_unity/auth/__init__.py
--rw-rw-r--   0 usman     (1000) usman     (1000)     1298 2023-08-06 23:08:30.000000 flask_unity-0.0.8/flask_unity/auth/admin.py
--rw-rw-r--   0 usman     (1000) usman     (1000)     1643 2023-08-06 23:08:30.000000 flask_unity-0.0.8/flask_unity/auth/forms.py
--rw-rw-r--   0 usman     (1000) usman     (1000)     1285 2023-08-06 23:08:30.000000 flask_unity-0.0.8/flask_unity/auth/models.py
--rw-rw-r--   0 usman     (1000) usman     (1000)     6089 2023-08-06 23:08:30.000000 flask_unity-0.0.8/flask_unity/auth/routes.py
--rw-rw-r--   0 usman     (1000) usman     (1000)    21240 2023-08-06 23:08:30.000000 flask_unity-0.0.8/flask_unity/base.py
--rw-rw-r--   0 usman     (1000) usman     (1000)     4721 2023-08-06 23:08:30.000000 flask_unity-0.0.8/flask_unity/blueprint.py
-drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-08-06 23:08:35.898913 flask_unity-0.0.8/flask_unity/contrib/
--rw-rw-r--   0 usman     (1000) usman     (1000)      619 2023-08-06 23:08:30.000000 flask_unity-0.0.8/flask_unity/contrib/__init__.py
--rw-rw-r--   0 usman     (1000) usman     (1000)      437 2023-08-06 23:08:30.000000 flask_unity-0.0.8/flask_unity/database.py
-drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-08-06 23:08:35.902912 flask_unity-0.0.8/flask_unity/mute/
--rw-rw-r--   0 usman     (1000) usman     (1000)      601 2023-08-06 23:08:30.000000 flask_unity-0.0.8/flask_unity/mute/__init__.py
--rw-rw-r--   0 usman     (1000) usman     (1000)     1532 2023-08-06 23:08:30.000000 flask_unity-0.0.8/flask_unity/mute/app.py
--rw-rw-r--   0 usman     (1000) usman     (1000)     2899 2023-08-06 23:08:30.000000 flask_unity-0.0.8/flask_unity/mute/page.py
--rw-rw-r--   0 usman     (1000) usman     (1000)     3430 2023-08-06 23:08:30.000000 flask_unity-0.0.8/flask_unity/mute/project.py
-drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-08-06 23:08:35.906912 flask_unity-0.0.8/flask_unity/static/
-drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-08-06 23:08:35.858921 flask_unity-0.0.8/flask_unity/static/default_style/
-drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-08-06 23:08:35.906912 flask_unity-0.0.8/flask_unity/static/default_style/css/
--rw-rw-r--   0 usman     (1000) usman     (1000)     6831 2023-08-06 21:05:40.000000 flask_unity-0.0.8/flask_unity/static/default_style/css/style.css
-drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-08-06 23:08:35.910911 flask_unity-0.0.8/flask_unity/static/default_style/js/
--rw-rw-r--   0 usman     (1000) usman     (1000)      132 2023-08-06 23:07:01.000000 flask_unity-0.0.8/flask_unity/static/default_style/js/index.js
-drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-08-06 23:08:35.914910 flask_unity-0.0.8/flask_unity/static/default_style/media/
--rw-rw-r--   0 usman     (1000) usman     (1000)     3767 2023-08-06 21:05:40.000000 flask_unity-0.0.8/flask_unity/static/default_style/media/alert.png
--rw-rw-r--   0 usman     (1000) usman     (1000)     1460 2023-08-06 21:05:40.000000 flask_unity-0.0.8/flask_unity/static/default_style/media/default_img.png
--rw-rw-r--   0 usman     (1000) usman     (1000)     3767 2023-08-06 21:05:40.000000 flask_unity-0.0.8/flask_unity/static/default_style/media/favicon.ico
--rw-rw-r--   0 usman     (1000) usman     (1000)        0 2023-08-06 21:05:40.000000 flask_unity-0.0.8/flask_unity/static/do_nothing.txt
-drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-08-06 23:08:35.862920 flask_unity-0.0.8/flask_unity/templates/
-drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-08-06 23:08:35.930907 flask_unity-0.0.8/flask_unity/templates/default_errors/
--rw-rw-r--   0 usman     (1000) usman     (1000)      141 2023-08-06 23:08:30.000000 flask_unity-0.0.8/flask_unity/templates/default_errors/400.html
--rw-rw-r--   0 usman     (1000) usman     (1000)      142 2023-08-06 23:08:30.000000 flask_unity-0.0.8/flask_unity/templates/default_errors/401.html
--rw-rw-r--   0 usman     (1000) usman     (1000)      139 2023-08-06 23:08:30.000000 flask_unity-0.0.8/flask_unity/templates/default_errors/403.html
--rw-rw-r--   0 usman     (1000) usman     (1000)      139 2023-08-06 23:08:30.000000 flask_unity-0.0.8/flask_unity/templates/default_errors/404.html
--rw-rw-r--   0 usman     (1000) usman     (1000)      144 2023-08-06 23:08:30.000000 flask_unity-0.0.8/flask_unity/templates/default_errors/406.html
--rw-rw-r--   0 usman     (1000) usman     (1000)      152 2023-08-06 23:08:30.000000 flask_unity-0.0.8/flask_unity/templates/default_errors/415.html
--rw-rw-r--   0 usman     (1000) usman     (1000)      147 2023-08-06 23:08:30.000000 flask_unity-0.0.8/flask_unity/templates/default_errors/429.html
--rw-rw-r--   0 usman     (1000) usman     (1000)      151 2023-08-06 23:08:30.000000 flask_unity-0.0.8/flask_unity/templates/default_errors/500.html
--rw-rw-r--   0 usman     (1000) usman     (1000)      146 2023-08-06 23:08:30.000000 flask_unity-0.0.8/flask_unity/templates/default_errors/501.html
--rw-rw-r--   0 usman     (1000) usman     (1000)      142 2023-08-06 23:08:30.000000 flask_unity-0.0.8/flask_unity/templates/default_errors/502.html
--rw-rw-r--   0 usman     (1000) usman     (1000)      150 2023-08-06 23:08:30.000000 flask_unity-0.0.8/flask_unity/templates/default_errors/503.html
--rw-rw-r--   0 usman     (1000) usman     (1000)      146 2023-08-06 23:08:30.000000 flask_unity-0.0.8/flask_unity/templates/default_errors/504.html
-drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-08-06 23:08:35.938905 flask_unity-0.0.8/flask_unity/templates/default_page/
--rw-rw-r--   0 usman     (1000) usman     (1000)     3092 2023-08-06 23:08:30.000000 flask_unity-0.0.8/flask_unity/templates/default_page/admin_change_password.html
--rw-rw-r--   0 usman     (1000) usman     (1000)      622 2023-08-06 23:08:30.000000 flask_unity-0.0.8/flask_unity/templates/default_page/admin_change_profile_image.html
--rw-rw-r--   0 usman     (1000) usman     (1000)     2262 2023-08-06 23:08:30.000000 flask_unity-0.0.8/flask_unity/templates/default_page/admin_login.html
--rw-rw-r--   0 usman     (1000) usman     (1000)     3150 2023-08-06 23:08:30.000000 flask_unity-0.0.8/flask_unity/templates/default_page/admin_register.html
--rw-rw-r--   0 usman     (1000) usman     (1000)     4196 2023-08-06 23:08:30.000000 flask_unity-0.0.8/flask_unity/templates/default_page/default.html
--rw-rw-r--   0 usman     (1000) usman     (1000)     1025 2023-08-06 23:08:30.000000 flask_unity-0.0.8/flask_unity/templates/default_page/default_base.html
--rw-rw-r--   0 usman     (1000) usman     (1000)      523 2023-08-06 23:08:30.000000 flask_unity-0.0.8/flask_unity/templates/default_page/default_index.html
--rw-rw-r--   0 usman     (1000) usman     (1000)     8740 2023-08-06 23:08:30.000000 flask_unity-0.0.8/flask_unity/utils.py
-drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-08-06 23:08:35.890915 flask_unity-0.0.8/flask_unity.egg-info/
--rw-rw-r--   0 usman     (1000) usman     (1000)     5941 2023-08-06 23:08:34.000000 flask_unity-0.0.8/flask_unity.egg-info/PKG-INFO
--rw-rw-r--   0 usman     (1000) usman     (1000)     1904 2023-08-06 23:08:35.000000 flask_unity-0.0.8/flask_unity.egg-info/SOURCES.txt
--rw-rw-r--   0 usman     (1000) usman     (1000)        1 2023-08-06 23:08:34.000000 flask_unity-0.0.8/flask_unity.egg-info/dependency_links.txt
--rw-rw-r--   0 usman     (1000) usman     (1000)      398 2023-08-06 23:08:34.000000 flask_unity-0.0.8/flask_unity.egg-info/requires.txt
--rw-rw-r--   0 usman     (1000) usman     (1000)       12 2023-08-06 23:08:34.000000 flask_unity-0.0.8/flask_unity.egg-info/top_level.txt
-drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-08-06 23:08:35.938905 flask_unity-0.0.8/media/
--rw-rw-r--   0 usman     (1000) usman     (1000)    30662 2023-08-06 23:08:30.000000 flask_unity-0.0.8/media/flask_unity_default_page.png
--rw-rw-r--   0 usman     (1000) usman     (1000)      417 2023-08-06 23:08:30.000000 flask_unity-0.0.8/requirements.txt
--rw-rw-r--   0 usman     (1000) usman     (1000)       38 2023-08-06 23:08:35.942905 flask_unity-0.0.8/setup.cfg
--rw-rw-r--   0 usman     (1000) usman     (1000)     2608 2023-08-06 23:08:30.000000 flask_unity-0.0.8/setup.py
+drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-08-06 23:10:35.962923 flask_unity-0.0.9/
+-rw-rw-r--   0 usman     (1000) usman     (1000)     1382 2023-08-06 23:10:30.000000 flask_unity-0.0.9/CHANGELOG
+-rw-rw-r--   0 usman     (1000) usman     (1000)     1077 2023-08-05 06:53:20.000000 flask_unity-0.0.9/LICENSE
+-rw-rw-r--   0 usman     (1000) usman     (1000)       82 2023-08-06 06:39:07.000000 flask_unity-0.0.9/MANIFEST.in
+-rw-rw-r--   0 usman     (1000) usman     (1000)     5867 2023-08-06 23:10:35.958923 flask_unity-0.0.9/PKG-INFO
+-rw-rw-r--   0 usman     (1000) usman     (1000)     3317 2023-08-06 23:10:30.000000 flask_unity-0.0.9/README.md
+drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-08-06 23:10:35.854944 flask_unity-0.0.9/flask_unity/
+-rw-rw-r--   0 usman     (1000) usman     (1000)      879 2023-08-06 23:10:30.000000 flask_unity-0.0.9/flask_unity/__init__.py
+-rw-rw-r--   0 usman     (1000) usman     (1000)     1280 2023-08-06 23:10:30.000000 flask_unity-0.0.9/flask_unity/api.py
+drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-08-06 23:10:35.886938 flask_unity-0.0.9/flask_unity/auth/
+-rw-rw-r--   0 usman     (1000) usman     (1000)       46 2023-08-06 23:08:30.000000 flask_unity-0.0.9/flask_unity/auth/__init__.py
+-rw-rw-r--   0 usman     (1000) usman     (1000)     1298 2023-08-06 23:08:30.000000 flask_unity-0.0.9/flask_unity/auth/admin.py
+-rw-rw-r--   0 usman     (1000) usman     (1000)     1643 2023-08-06 23:08:30.000000 flask_unity-0.0.9/flask_unity/auth/forms.py
+-rw-rw-r--   0 usman     (1000) usman     (1000)     1285 2023-08-06 23:08:30.000000 flask_unity-0.0.9/flask_unity/auth/models.py
+-rw-rw-r--   0 usman     (1000) usman     (1000)     6089 2023-08-06 23:08:30.000000 flask_unity-0.0.9/flask_unity/auth/routes.py
+-rw-rw-r--   0 usman     (1000) usman     (1000)    22696 2023-08-06 23:10:30.000000 flask_unity-0.0.9/flask_unity/base.py
+-rw-rw-r--   0 usman     (1000) usman     (1000)     4721 2023-08-06 23:08:30.000000 flask_unity-0.0.9/flask_unity/blueprint.py
+drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-08-06 23:10:35.890937 flask_unity-0.0.9/flask_unity/contrib/
+-rw-rw-r--   0 usman     (1000) usman     (1000)      619 2023-08-06 23:08:30.000000 flask_unity-0.0.9/flask_unity/contrib/__init__.py
+-rw-rw-r--   0 usman     (1000) usman     (1000)      437 2023-08-06 23:08:30.000000 flask_unity-0.0.9/flask_unity/database.py
+drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-08-06 23:10:35.902935 flask_unity-0.0.9/flask_unity/mute/
+-rw-rw-r--   0 usman     (1000) usman     (1000)      601 2023-08-06 23:08:30.000000 flask_unity-0.0.9/flask_unity/mute/__init__.py
+-rw-rw-r--   0 usman     (1000) usman     (1000)     1532 2023-08-06 23:08:30.000000 flask_unity-0.0.9/flask_unity/mute/app.py
+-rw-rw-r--   0 usman     (1000) usman     (1000)     2899 2023-08-06 23:08:30.000000 flask_unity-0.0.9/flask_unity/mute/page.py
+-rw-rw-r--   0 usman     (1000) usman     (1000)     3458 2023-08-06 23:10:30.000000 flask_unity-0.0.9/flask_unity/mute/project.py
+drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-08-06 23:10:35.902935 flask_unity-0.0.9/flask_unity/static/
+drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-08-06 23:10:35.802955 flask_unity-0.0.9/flask_unity/static/default_style/
+drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-08-06 23:10:35.906934 flask_unity-0.0.9/flask_unity/static/default_style/css/
+-rw-rw-r--   0 usman     (1000) usman     (1000)     6831 2023-08-06 21:05:40.000000 flask_unity-0.0.9/flask_unity/static/default_style/css/style.css
+drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-08-06 23:10:35.910933 flask_unity-0.0.9/flask_unity/static/default_style/js/
+-rw-rw-r--   0 usman     (1000) usman     (1000)      132 2023-08-06 23:07:01.000000 flask_unity-0.0.9/flask_unity/static/default_style/js/index.js
+drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-08-06 23:10:35.922931 flask_unity-0.0.9/flask_unity/static/default_style/media/
+-rw-rw-r--   0 usman     (1000) usman     (1000)     3767 2023-08-06 21:05:40.000000 flask_unity-0.0.9/flask_unity/static/default_style/media/alert.png
+-rw-rw-r--   0 usman     (1000) usman     (1000)     1460 2023-08-06 21:05:40.000000 flask_unity-0.0.9/flask_unity/static/default_style/media/default_img.png
+-rw-rw-r--   0 usman     (1000) usman     (1000)     3767 2023-08-06 21:05:40.000000 flask_unity-0.0.9/flask_unity/static/default_style/media/favicon.ico
+-rw-rw-r--   0 usman     (1000) usman     (1000)        0 2023-08-06 21:05:40.000000 flask_unity-0.0.9/flask_unity/static/do_nothing.txt
+drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-08-06 23:10:35.810953 flask_unity-0.0.9/flask_unity/templates/
+drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-08-06 23:10:35.942927 flask_unity-0.0.9/flask_unity/templates/default_errors/
+-rw-rw-r--   0 usman     (1000) usman     (1000)      141 2023-08-06 23:08:30.000000 flask_unity-0.0.9/flask_unity/templates/default_errors/400.html
+-rw-rw-r--   0 usman     (1000) usman     (1000)      142 2023-08-06 23:08:30.000000 flask_unity-0.0.9/flask_unity/templates/default_errors/401.html
+-rw-rw-r--   0 usman     (1000) usman     (1000)      139 2023-08-06 23:08:30.000000 flask_unity-0.0.9/flask_unity/templates/default_errors/403.html
+-rw-rw-r--   0 usman     (1000) usman     (1000)      139 2023-08-06 23:08:30.000000 flask_unity-0.0.9/flask_unity/templates/default_errors/404.html
+-rw-rw-r--   0 usman     (1000) usman     (1000)      144 2023-08-06 23:08:30.000000 flask_unity-0.0.9/flask_unity/templates/default_errors/406.html
+-rw-rw-r--   0 usman     (1000) usman     (1000)      152 2023-08-06 23:08:30.000000 flask_unity-0.0.9/flask_unity/templates/default_errors/415.html
+-rw-rw-r--   0 usman     (1000) usman     (1000)      147 2023-08-06 23:08:30.000000 flask_unity-0.0.9/flask_unity/templates/default_errors/429.html
+-rw-rw-r--   0 usman     (1000) usman     (1000)      151 2023-08-06 23:08:30.000000 flask_unity-0.0.9/flask_unity/templates/default_errors/500.html
+-rw-rw-r--   0 usman     (1000) usman     (1000)      146 2023-08-06 23:08:30.000000 flask_unity-0.0.9/flask_unity/templates/default_errors/501.html
+-rw-rw-r--   0 usman     (1000) usman     (1000)      142 2023-08-06 23:08:30.000000 flask_unity-0.0.9/flask_unity/templates/default_errors/502.html
+-rw-rw-r--   0 usman     (1000) usman     (1000)      150 2023-08-06 23:08:30.000000 flask_unity-0.0.9/flask_unity/templates/default_errors/503.html
+-rw-rw-r--   0 usman     (1000) usman     (1000)      146 2023-08-06 23:08:30.000000 flask_unity-0.0.9/flask_unity/templates/default_errors/504.html
+drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-08-06 23:10:35.958923 flask_unity-0.0.9/flask_unity/templates/default_page/
+-rw-rw-r--   0 usman     (1000) usman     (1000)     3092 2023-08-06 23:08:30.000000 flask_unity-0.0.9/flask_unity/templates/default_page/admin_change_password.html
+-rw-rw-r--   0 usman     (1000) usman     (1000)      622 2023-08-06 23:08:30.000000 flask_unity-0.0.9/flask_unity/templates/default_page/admin_change_profile_image.html
+-rw-rw-r--   0 usman     (1000) usman     (1000)     2262 2023-08-06 23:08:30.000000 flask_unity-0.0.9/flask_unity/templates/default_page/admin_login.html
+-rw-rw-r--   0 usman     (1000) usman     (1000)     3150 2023-08-06 23:08:30.000000 flask_unity-0.0.9/flask_unity/templates/default_page/admin_register.html
+-rw-rw-r--   0 usman     (1000) usman     (1000)     4196 2023-08-06 23:08:30.000000 flask_unity-0.0.9/flask_unity/templates/default_page/default.html
+-rw-rw-r--   0 usman     (1000) usman     (1000)     1025 2023-08-06 23:08:30.000000 flask_unity-0.0.9/flask_unity/templates/default_page/default_base.html
+-rw-rw-r--   0 usman     (1000) usman     (1000)      519 2023-08-06 23:10:30.000000 flask_unity-0.0.9/flask_unity/templates/default_page/default_index.html
+-rw-rw-r--   0 usman     (1000) usman     (1000)     8740 2023-08-06 23:10:30.000000 flask_unity-0.0.9/flask_unity/utils.py
+drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-08-06 23:10:35.870941 flask_unity-0.0.9/flask_unity.egg-info/
+-rw-rw-r--   0 usman     (1000) usman     (1000)     5867 2023-08-06 23:10:34.000000 flask_unity-0.0.9/flask_unity.egg-info/PKG-INFO
+-rw-rw-r--   0 usman     (1000) usman     (1000)     1904 2023-08-06 23:10:35.000000 flask_unity-0.0.9/flask_unity.egg-info/SOURCES.txt
+-rw-rw-r--   0 usman     (1000) usman     (1000)        1 2023-08-06 23:10:34.000000 flask_unity-0.0.9/flask_unity.egg-info/dependency_links.txt
+-rw-rw-r--   0 usman     (1000) usman     (1000)      398 2023-08-06 23:10:34.000000 flask_unity-0.0.9/flask_unity.egg-info/requires.txt
+-rw-rw-r--   0 usman     (1000) usman     (1000)       12 2023-08-06 23:10:34.000000 flask_unity-0.0.9/flask_unity.egg-info/top_level.txt
+drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-08-06 23:10:35.958923 flask_unity-0.0.9/media/
+-rw-rw-r--   0 usman     (1000) usman     (1000)    30636 2023-08-06 23:10:30.000000 flask_unity-0.0.9/media/flask_unity_default_page.png
+-rw-rw-r--   0 usman     (1000) usman     (1000)      417 2023-08-06 23:10:30.000000 flask_unity-0.0.9/requirements.txt
+-rw-rw-r--   0 usman     (1000) usman     (1000)       38 2023-08-06 23:10:35.986918 flask_unity-0.0.9/setup.cfg
+-rw-rw-r--   0 usman     (1000) usman     (1000)     2613 2023-08-06 23:10:30.000000 flask_unity-0.0.9/setup.py
```

### Comparing `flask_unity-0.0.8/CHANGELOG` & `flask_unity-0.0.9/CHANGELOG`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 # Change Log
 
-## 0.0.8 (07/august/2023)
+## 0.0.9 (07/august/2023)
+
+- Nineth Release
+
+Fixing bugs
+
+Fixing v0.0.8 bugs for OS compatibility, and also tested on windows OS
 
 - Eight Release
 
 OS compatibility
 
 Making flask_unity to be compatible with windows OS as well as other OS
```

### Comparing `flask_unity-0.0.8/LICENSE` & `flask_unity-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_unity-0.0.8/PKG-INFO` & `flask_unity-0.0.9/flask_unity.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: flask_unity
-Version: 0.0.8
+Name: flask-unity
+Version: 0.0.9
 Summary: An extension of flask web framework that erase the complexity of structuring flask project blueprint, packages, and other annoying stuffs
 Home-page: https://flask-unity.readthedocs.io
 Download-URL: https://pypi.org/project/flask-unity
 Author: Usman Musa
 Author-email: usmanmusa1920@gmail.com
 License: MIT
 Project-URL: Documentation, https://flask-unity.readthedocs.io
@@ -28,15 +28,15 @@
 
 # Flask-unity
 
 An extension of flask web framework that erase the complexity of structuring flask project blueprint, packages, and other annoying stuffs.
 
 ## Installation
 
-Install and update the latest release from <a href="https://pypi.org/project/flask-unity">pypi</a>. Basically the library was uploaded using `sdist` (Source Distribution) and this software (library) it might not be compatible with `windows operating system` but it works on other `OS` such as `linux` and `macOS`, but very soon the version that will be compatible with **windows operating system** will be release, stay tuned.
+Install and update the latest release from <a href="https://pypi.org/project/flask-unity">pypi</a>. Basically the library was uploaded using `sdist` (Source Distribution) and this software (library) as from `v0.0.9` it is now compatible and also tested with `windows OS` and others as well, such as `linux`, `macOS` and possibly some others too!.
 
 ```
 pip install --upgrade flask_unity
 ```
 
 ## Create flask project using flask_unity
 
@@ -100,35 +100,37 @@
 
 visit `http://127.0.0.1:5000/admin` this will take you to admin page. From there you are ready to go.
 
 See more documentations <a href="https://flask-unity.readthedocs.io">here!</a>
 
 ### Flask-unity default page
 
-![Flask-unity default page](./media/flask_unity_default_page.png)
-
-### Flask-unity default page
-
 <!-- ![Flask-unity default page](./media/flask_unity_default_page.png) -->
 
-[![Flask-unity default page](https://raw.githubusercontent.com/usmanmusa1920/flask_unity/v0.0.8/media/flask_unity_default_page.png)](https://flask-unity.readthedocs.io)
+[![Flask-unity default page](https://raw.githubusercontent.com/usmanmusa1920/flask_unity/v0.0.9/media/flask_unity_default_page.png)](https://flask-unity.readthedocs.io)
 
 ## Useful links
 
 - Documentation: https://flask-unity.readthedocs.io
 - Repository: https://github.com/usmanmusa1920/flask-unity
 <!-- - PYPI Release: https://pypi.org/project/flask-unity -->
 - Docker example: https://github.com/usmanmusa1920/flask-unity/tree/master/example/flask_unity-docker
 
 Pull requests are welcome
 
 
 # Change Log
 
-## 0.0.8 (07/august/2023)
+## 0.0.9 (07/august/2023)
+
+- Nineth Release
+
+Fixing bugs
+
+Fixing v0.0.8 bugs for OS compatibility, and also tested on windows OS
 
 - Eight Release
 
 OS compatibility
 
 Making flask_unity to be compatible with windows OS as well as other OS
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flask_unity Version: 0.0.8 Summary: An extension of
+Metadata-Version: 2.1 Name: flask-unity Version: 0.0.9 Summary: An extension of
 flask web framework that erase the complexity of structuring flask project
 blueprint, packages, and other annoying stuffs Home-page: https://flask-
 unity.readthedocs.io Download-URL: https://pypi.org/project/flask-unity Author:
 Usman Musa Author-email: usmanmusa1920@gmail.com License: MIT Project-URL:
 Documentation, https://flask-unity.readthedocs.io Project-URL: Source, https://
 github.com/usmanmusa1920/flask-unity Keywords: flask_unity Platform: any
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
@@ -13,61 +13,59 @@
 Language :: Python Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.10 Requires-Python: >=3.6 Description-Content-Type: text/markdown
 License-File: LICENSE # Flask-unity An extension of flask web framework that
 erase the complexity of structuring flask project blueprint, packages, and
 other annoying stuffs. ## Installation Install and update the latest release
 from pypi. Basically the library was uploaded using `sdist` (Source
-Distribution) and this software (library) it might not be compatible with
-`windows operating system` but it works on other `OS` such as `linux` and
-`macOS`, but very soon the version that will be compatible with **windows
-operating system** will be release, stay tuned. ``` pip install --upgrade
-flask_unity ``` ## Create flask project using flask_unity After the
-installation paste the following command on your termianl ``` python -c "from
-flask_unity import project; project('schoolsite')" ``` This will create a
-project called `schoolsite` now cd into the `schoolsite` directory, if you do
-`ls` within the directory you just enter you will see a module called
-`thunder.py` and some directories (some in the form of package) `media`,
-`static`, `templates` and a directory with the same name of your base directory
-name, in our case it is `schoolsite`. Boot up the flask server by running the
-below command ``` python thunder.py boot ``` Now visit the local url `http://
-127.0.0.1:5000` this will show you index page of your project ## Create flask
-app within your project (schoolsite) For you to start an app within your
-project `schoolsite` shutdown the flask development server by pressing ( CTRL+C
-) and then run the following command, by giving the name you want your app to
-be, in our case we will call our app `exam` ``` python thunder.py create_app -
-a exam ``` this will create an app (a new package called `exam`) within your
-project `(schoolsite)` ## Register an app Once the app is created open a file
-`schoolsite/routes.py` and import your `exam` blueprint which is in (`exam/
-views.py`), default name given to an app blueprint, is the app name so our
-`exam` app blueprint name is `exam`, after importing it, append (register) the
-app blueprint in a list called `reg_blueprints` in that same file of
-`schoolsite/routes.py` importing blueprint ```py from exam.views import exam
-``` registering blueprint ```py reg_blueprints = [ blueprint.default,
-blueprint.errors, blueprint.auth, base, exam, ] ``` once you register the app,
-boot up the flask webserver again by ``` python thunder.py boot ``` visit
-`http://127.0.0.1:5000` which is your project landing page visit `http://
-127.0.0.1:5000/exam` this will take you to your app landing page (exam) visit
-`http://127.0.0.1:5000/admin` this will take you to admin page. From there you
-are ready to go. See more documentations here! ### Flask-unity default page !
-[Flask-unity default page](./media/flask_unity_default_page.png) ### Flask-
-unity default page  [![Flask-unity default page](https://
-raw.githubusercontent.com/usmanmusa1920/flask_unity/v0.0.8/media/
+Distribution) and this software (library) as from `v0.0.9` it is now compatible
+and also tested with `windows OS` and others as well, such as `linux`, `macOS`
+and possibly some others too!. ``` pip install --upgrade flask_unity ``` ##
+Create flask project using flask_unity After the installation paste the
+following command on your termianl ``` python -c "from flask_unity import
+project; project('schoolsite')" ``` This will create a project called
+`schoolsite` now cd into the `schoolsite` directory, if you do `ls` within the
+directory you just enter you will see a module called `thunder.py` and some
+directories (some in the form of package) `media`, `static`, `templates` and a
+directory with the same name of your base directory name, in our case it is
+`schoolsite`. Boot up the flask server by running the below command ``` python
+thunder.py boot ``` Now visit the local url `http://127.0.0.1:5000` this will
+show you index page of your project ## Create flask app within your project
+(schoolsite) For you to start an app within your project `schoolsite` shutdown
+the flask development server by pressing ( CTRL+C ) and then run the following
+command, by giving the name you want your app to be, in our case we will call
+our app `exam` ``` python thunder.py create_app -a exam ``` this will create an
+app (a new package called `exam`) within your project `(schoolsite)` ##
+Register an app Once the app is created open a file `schoolsite/routes.py` and
+import your `exam` blueprint which is in (`exam/views.py`), default name given
+to an app blueprint, is the app name so our `exam` app blueprint name is
+`exam`, after importing it, append (register) the app blueprint in a list
+called `reg_blueprints` in that same file of `schoolsite/routes.py` importing
+blueprint ```py from exam.views import exam ``` registering blueprint ```py
+reg_blueprints = [ blueprint.default, blueprint.errors, blueprint.auth, base,
+exam, ] ``` once you register the app, boot up the flask webserver again by ```
+python thunder.py boot ``` visit `http://127.0.0.1:5000` which is your project
+landing page visit `http://127.0.0.1:5000/exam` this will take you to your app
+landing page (exam) visit `http://127.0.0.1:5000/admin` this will take you to
+admin page. From there you are ready to go. See more documentations here! ###
+Flask-unity default page  [![Flask-unity default page](https://
+raw.githubusercontent.com/usmanmusa1920/flask_unity/v0.0.9/media/
 flask_unity_default_page.png)](https://flask-unity.readthedocs.io) ## Useful
 links - Documentation: https://flask-unity.readthedocs.io - Repository: https:/
 /github.com/usmanmusa1920/flask-unity  - Docker example: https://github.com/
 usmanmusa1920/flask-unity/tree/master/example/flask_unity-docker Pull requests
-are welcome # Change Log ## 0.0.8 (07/august/2023) - Eight Release OS
-compatibility Making flask_unity to be compatible with windows OS as well as
-other OS ## 0.0.7 (07/august/2023) - Seventh Release This release mostly is for
-adding more docs and examples. - Sixth Release Alembic is included as
-dependency (in the require module list). - Fifth Release In fifith release, we
-handle how default user file system tricks is, things like when user change his
-profile picture. - Fourth Release In this release we handle how we can
-customise the admin html page by inheriting (extends) it in our project
+are welcome # Change Log ## 0.0.9 (07/august/2023) - Nineth Release Fixing bugs
+Fixing v0.0.8 bugs for OS compatibility, and also tested on windows OS - Eight
+Release OS compatibility Making flask_unity to be compatible with windows OS as
+well as other OS ## 0.0.7 (07/august/2023) - Seventh Release This release
+mostly is for adding more docs and examples. - Sixth Release Alembic is
+included as dependency (in the require module list). - Fifth Release In fifith
+release, we handle how default user file system tricks is, things like when
+user change his profile picture. - Fourth Release In this release we handle how
+we can customise the admin html page by inheriting (extends) it in our project
 templates/admin directory, and the admin page on how to bind models in the
 admin. Also I refactor other libraries that this package needs with their
 corresponding versions in the setup.py and requirements.txt files. In this
 release good documentations is well packed. Database migration is added using
 `alembic` Some error pages, default page were added but still you can customise
 it in your project sub folder (the package with the same name of your project
 in your project directory) in a file called `route.py`. Also an admin directory
```

### Comparing `flask_unity-0.0.8/README.md` & `flask_unity-0.0.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Flask-unity
 
 An extension of flask web framework that erase the complexity of structuring flask project blueprint, packages, and other annoying stuffs.
 
 ## Installation
 
-Install and update the latest release from <a href="https://pypi.org/project/flask-unity">pypi</a>. Basically the library was uploaded using `sdist` (Source Distribution) and this software (library) it might not be compatible with `windows operating system` but it works on other `OS` such as `linux` and `macOS`, but very soon the version that will be compatible with **windows operating system** will be release, stay tuned.
+Install and update the latest release from <a href="https://pypi.org/project/flask-unity">pypi</a>. Basically the library was uploaded using `sdist` (Source Distribution) and this software (library) as from `v0.0.9` it is now compatible and also tested with `windows OS` and others as well, such as `linux`, `macOS` and possibly some others too!.
 
 ```
 pip install --upgrade flask_unity
 ```
 
 ## Create flask project using flask_unity
 
@@ -72,21 +72,17 @@
 
 visit `http://127.0.0.1:5000/admin` this will take you to admin page. From there you are ready to go.
 
 See more documentations <a href="https://flask-unity.readthedocs.io">here!</a>
 
 ### Flask-unity default page
 
-![Flask-unity default page](./media/flask_unity_default_page.png)
-
-### Flask-unity default page
-
 <!-- ![Flask-unity default page](./media/flask_unity_default_page.png) -->
 
-[![Flask-unity default page](https://raw.githubusercontent.com/usmanmusa1920/flask_unity/v0.0.8/media/flask_unity_default_page.png)](https://flask-unity.readthedocs.io)
+[![Flask-unity default page](https://raw.githubusercontent.com/usmanmusa1920/flask_unity/v0.0.9/media/flask_unity_default_page.png)](https://flask-unity.readthedocs.io)
 
 ## Useful links
 
 - Documentation: https://flask-unity.readthedocs.io
 - Repository: https://github.com/usmanmusa1920/flask-unity
 <!-- - PYPI Release: https://pypi.org/project/flask-unity -->
 - Docker example: https://github.com/usmanmusa1920/flask-unity/tree/master/example/flask_unity-docker
```

#### html2text {}

```diff
@@ -1,15 +1,14 @@
 # Flask-unity An extension of flask web framework that erase the complexity of
 structuring flask project blueprint, packages, and other annoying stuffs. ##
 Installation Install and update the latest release from pypi. Basically the
 library was uploaded using `sdist` (Source Distribution) and this software
-(library) it might not be compatible with `windows operating system` but it
-works on other `OS` such as `linux` and `macOS`, but very soon the version that
-will be compatible with **windows operating system** will be release, stay
-tuned. ``` pip install --upgrade flask_unity ``` ## Create flask project using
+(library) as from `v0.0.9` it is now compatible and also tested with `windows
+OS` and others as well, such as `linux`, `macOS` and possibly some others too!.
+``` pip install --upgrade flask_unity ``` ## Create flask project using
 flask_unity After the installation paste the following command on your termianl
 ``` python -c "from flask_unity import project; project('schoolsite')" ``` This
 will create a project called `schoolsite` now cd into the `schoolsite`
 directory, if you do `ls` within the directory you just enter you will see a
 module called `thunder.py` and some directories (some in the form of package)
 `media`, `static`, `templates` and a directory with the same name of your base
 directory name, in our case it is `schoolsite`. Boot up the flask server by
@@ -28,16 +27,14 @@
 file of `schoolsite/routes.py` importing blueprint ```py from exam.views import
 exam ``` registering blueprint ```py reg_blueprints = [ blueprint.default,
 blueprint.errors, blueprint.auth, base, exam, ] ``` once you register the app,
 boot up the flask webserver again by ``` python thunder.py boot ``` visit
 `http://127.0.0.1:5000` which is your project landing page visit `http://
 127.0.0.1:5000/exam` this will take you to your app landing page (exam) visit
 `http://127.0.0.1:5000/admin` this will take you to admin page. From there you
-are ready to go. See more documentations here! ### Flask-unity default page !
-[Flask-unity default page](./media/flask_unity_default_page.png) ### Flask-
-unity default page  [![Flask-unity default page](https://
-raw.githubusercontent.com/usmanmusa1920/flask_unity/v0.0.8/media/
-flask_unity_default_page.png)](https://flask-unity.readthedocs.io) ## Useful
-links - Documentation: https://flask-unity.readthedocs.io - Repository: https:/
-/github.com/usmanmusa1920/flask-unity  - Docker example: https://github.com/
-usmanmusa1920/flask-unity/tree/master/example/flask_unity-docker Pull requests
-are welcome
+are ready to go. See more documentations here! ### Flask-unity default page  [!
+[Flask-unity default page](https://raw.githubusercontent.com/usmanmusa1920/
+flask_unity/v0.0.9/media/flask_unity_default_page.png)](https://flask-
+unity.readthedocs.io) ## Useful links - Documentation: https://flask-
+unity.readthedocs.io - Repository: https://github.com/usmanmusa1920/flask-unity
+- Docker example: https://github.com/usmanmusa1920/flask-unity/tree/master/
+example/flask_unity-docker Pull requests are welcome
```

### Comparing `flask_unity-0.0.8/flask_unity/__init__.py` & `flask_unity-0.0.9/flask_unity/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     /    /___ /  | /_/ /  |     /__/ /  |/ __/__   /     /
   
   An extension of flask web framework that erase the complexity of structuring flask project blueprint, packages, and other annoying stuffs
 """
 
 
 __title__ = 'flask_unity'
-__version__ = '0.0.8'
+__version__ = '0.0.9'
 __author__ = 'Usman Musa'
 __author_email__ = 'usmanmusa1920@gmail.com'
 __author_website__ = 'https://usmanmusa1920.github.io'
 __repository__ = 'https://github.com/usmanmusa1920/flask-unity'
 __url__ = 'https://flask-unity.readthedocs.io'
 __copyright__ = 'Copyright (C) 2022 - 2023 Usman Musa'
```

### Comparing `flask_unity-0.0.8/flask_unity/auth/admin.py` & `flask_unity-0.0.9/flask_unity/auth/admin.py`

 * *Files identical despite different names*

### Comparing `flask_unity-0.0.8/flask_unity/auth/forms.py` & `flask_unity-0.0.9/flask_unity/auth/forms.py`

 * *Files identical despite different names*

### Comparing `flask_unity-0.0.8/flask_unity/auth/models.py` & `flask_unity-0.0.9/flask_unity/auth/models.py`

 * *Files identical despite different names*

### Comparing `flask_unity-0.0.8/flask_unity/auth/routes.py` & `flask_unity-0.0.9/flask_unity/auth/routes.py`

 * *Files identical despite different names*

### Comparing `flask_unity-0.0.8/flask_unity/base.py` & `flask_unity-0.0.9/flask_unity/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,31 +33,51 @@
   DEBUG     ---  10
   INFO      ---  20
   WARNING   ---  30  (default)
   ERROR     ---  40
   CRITICAL  ---  50
 """
 
-formatter = '[+] [%(asctime)s] [%(levelname)s] %(message)s'
-logging.basicConfig(format = formatter)
+FORMATTER = '[+] [%(asctime)s] [%(levelname)s] %(message)s'
+logging.basicConfig(format = FORMATTER)
 LOGGER = logging.getLogger(__name__)
 LOGGER.setLevel(logging.DEBUG)
 
 # used for relative path to default image to copy for a project (only)
 ORIGIN = Path(__file__).resolve().parent
 OS_SEP = os.path.sep # platform-specific path separator (for linux `/`, for windows `\\`)
 
 
 class BaseStructure:
   """base structure class"""
 
   def __init__(self, is_software=True):
     """base structure class initializer"""
     self.is_software = is_software
-    self.fls_cmd = 'touch'
+
+    # we can use any of the below three variables to make our code compatible with
+    # many OS, but we go with the first one which is `self.os_name`
+    self.os_name = os.name # nt or posix
+    self.platform_name_1 = sys.platform # win32 or linux or darwin or android
+    self.platform_name_2 = platform.system() # Windows, Darwin, Linux, etc.
+
+    if self.os_name == 'nt':
+    # if self.platform_name_1 == 'win32':
+    # if self.platform_name_2 == 'Windows':
+      self.fls_cmd = 'echo >'
+    elif self.os_name == 'posix':
+    # elif self.platform_name_1 == 'linux' or self.platform_name_1 == 'darwin' or self.platform_name_1 == 'android':
+    # elif self.platform_name_2 == 'Linux' or self.platform_name_2 == 'Darwin':
+      self.fls_cmd = 'touch'
+    else:
+      err_compt = f'{__title__.capitalize()} v{__version__} is not compatible with your OS'
+      print()
+      LOGGER.error(err_compt)
+      print()
+      exit()
     self._exs_first = ['index', 'style']
     self._exs_last = ['.html', '.css', '.js']
     
 
   def append_exs_to_file(self, fls_name=False, _exs_='.py', name=None):
     """
     append .py extension for files if _exs_ value is '.py' or type is str, else if _exs_ type is list, make list of static files `['index.html', 'index.js', 'style.css']`
@@ -105,30 +125,20 @@
       img_write.write(img_read_data)
       
 
   def file_opt(self, _dir, tree=True, _here=False, _where=False):
     """
     make dir tree if `tree=True` and get into it, if `_here` or `_where` is equal to True
     """
-
-    # we can use any of the below three variables to make our code compatible with many OS
-    os_name = os.name # nt or posix
-    platform_name_1 = sys.platform # win32 or linux or darwin or android
-    platform_name_2 = platform.system() # Windows, Darwin, Linux, etc.
-
     if tree:
-      if os_name == 'nt':
-      # if platform_name_1 == 'win32':
-      # if platform_name_2 == 'Windows':
+      if self.os_name == 'nt':
         os.makedirs(_dir, exist_ok=True)
         # The exist_ok=True argument ensures that the function
         # does not raise an exception if the directory already exists.
-      elif os_name == 'posix':
-      # elif platform_name_1 == 'linux' or platform_name_1 == 'darwin' or platform_name_1 == 'android':
-      # elif platform_name_2 == 'Linux' or platform_name_2 == 'Darwin':
+      elif self.os_name == 'posix':
         sp.run(['mkdir', '-p', _dir])
       else:
         err_compt = f'{__title__.capitalize()} v{__version__} is not compatible with your OS'
         print()
         LOGGER.error(err_compt)
         print()
         exit()
@@ -159,15 +169,24 @@
     is_app: if it is True, that mean it will do operation of making app files,
     else it will make for the entire project
     """
     
     if is_app:
       for _fls in fls:
         app_name = os.getcwd().split(OS_SEP)[-1]
-        sp.run(shlex.split(f'{fls_cmd} {_fls}'))
+        if self.os_name == 'nt':
+          sp.run(shlex.split(f'{fls_cmd} {_fls}'), shell=True)
+        elif self.os_name == 'posix':
+          sp.run(shlex.split(f'{fls_cmd} {_fls}'))
+        else:
+          err_compt = f'{__title__.capitalize()} v{__version__} is not compatible with your OS'
+          print()
+          LOGGER.error(err_compt)
+          print()
+          exit()
         if is_static_file:
           # building app default files (html, css, js)
           self.file_content(file_name=_fls, content=f'{app_default_dummy}', route_go=False)
         else:
           # building app default files (__init__.py, admin.py, forms.py, models.py, views.py)
           if _fls == '__init__.py':
             self.file_content(file_name=_fls, content=f'# from {__title__} software, your app ({app_name}) {_fls} file\n{app_init_dummy()}', route_go=False)
@@ -178,15 +197,24 @@
           elif _fls == 'models.py':
             self.file_content(file_name=_fls, content=f'# from {__title__} software, your app ({app_name}) {_fls} file\n{app_models_dummy()}', route_go=False)
           elif _fls == 'views.py':
             self.file_content(file_name=_fls, content=f'# from {__title__} software, your app ({app_name}) {_fls} file\n{app_views_dummy(app_name)}', route_go=False)
     else:
       for _fls in fls:
         if _fls[:-3] == file:
-          sp.run(shlex.split(f'{fls_cmd} {_fls}'))
+          if self.os_name == 'nt':
+            sp.run(shlex.split(f'{fls_cmd} {_fls}'), shell=True)
+          elif self.os_name == 'posix':
+            sp.run(shlex.split(f'{fls_cmd} {_fls}'))
+          else:
+            err_compt = f'{__title__.capitalize()} v{__version__} is not compatible with your OS'
+            print()
+            LOGGER.error(err_compt)
+            print()
+            exit()
           self.file_content(
             file_name=_fls,content=f'# Your project {_fls} file\n{thunder_dummy(proj_nm)}', route_go=False
             ) # building the run module `thunder.py`
             
 
   def dir_tree(self, proj_name=None):
     """
@@ -209,15 +237,24 @@
       # making directories trees and their default files in the loop
       for _dir in dirs:
         if _dir == dirs[0] + OS_SEP + dirs[0]:
           self.file_opt(_dir, _here=_here)
           # create default modules inside project sub dir
           for _fls in fls:
             if _fls[:-3] != 'thunder':
-              sp.run(shlex.split(f'{self.fls_cmd} {_fls}'))
+              if self.os_name == 'nt':
+                sp.run(shlex.split(f'{self.fls_cmd} {_fls}'), shell=True)
+              elif self.os_name == 'posix':
+                sp.run(shlex.split(f'{self.fls_cmd} {_fls}'))
+              else:
+                err_compt = f'{__title__.capitalize()} v{__version__} is not compatible with your OS'
+                print()
+                LOGGER.error(err_compt)
+                print()
+                exit()
               # building project default files (__init__.py, config.py, routes.py, secret.py)
               if _fls == '__init__.py':
                 self.file_content(file_name=_fls, content=f'# from {__title__} software, your ({proj_name}) project {_fls} file\n{pro_init_dummy()}', route_go=False)
               elif _fls == 'config.py':
                 self.file_content(file_name=_fls, content=f'# from {__title__} software, your ({proj_name}) project {_fls} file\n{pro_config_dummy(proj_name)}', route_go=False)
               elif _fls == 'routes.py':
                 self.file_content(file_name=_fls, content=f'# from {__title__} software, your ({proj_name}) project {_fls} file\n{pro_routes_dummy(proj_name)}', route_go=False)
```

### Comparing `flask_unity-0.0.8/flask_unity/blueprint.py` & `flask_unity-0.0.9/flask_unity/blueprint.py`

 * *Files identical despite different names*

### Comparing `flask_unity-0.0.8/flask_unity/contrib/__init__.py` & `flask_unity-0.0.9/flask_unity/contrib/__init__.py`

 * *Files identical despite different names*

### Comparing `flask_unity-0.0.8/flask_unity/mute/__init__.py` & `flask_unity-0.0.9/flask_unity/mute/__init__.py`

 * *Files identical despite different names*

### Comparing `flask_unity-0.0.8/flask_unity/mute/app.py` & `flask_unity-0.0.9/flask_unity/mute/app.py`

 * *Files identical despite different names*

### Comparing `flask_unity-0.0.8/flask_unity/mute/page.py` & `flask_unity-0.0.9/flask_unity/mute/page.py`

 * *Files identical despite different names*

### Comparing `flask_unity-0.0.8/flask_unity/mute/project.py` & `flask_unity-0.0.9/flask_unity/mute/project.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 ORIGIN_PATH = Path(__file__).resolve().parent.parent
 OS_SEP = os.path.sep # platform-specific path separator (for linux `/`, for windows `\\`)
 
 
 class Config:
   SECRET_KEY = '{secure_app}'
   # The `SQLALCHEMY_DATABASE_URI` might not be compatible with windows OS,
-  # change it to your windows drive like: 'C:\path\to\your\default.db'
+  # change it to your windows drive like: 'C:\path\to\your\default.db' (if you encounter an error)
   SQLALCHEMY_DATABASE_URI = 'sqlite:///'+str(ORIGIN_PATH)+OS_SEP+'default.db'
   # set optional bootswatch theme
   FLASK_ADMIN_SWATCH = 'cerulean'
   UPLOAD_FOLDER = os.path.join(ORIGIN_PATH, 'media')
   ALLOWED_EXTENSIONS = ('png', 'jpg', 'jpeg')
   MAX_CONTENT_LENGTH = 16 * 1024 * 1024
```

### Comparing `flask_unity-0.0.8/flask_unity/static/default_style/css/style.css` & `flask_unity-0.0.9/flask_unity/static/default_style/css/style.css`

 * *Files identical despite different names*

### Comparing `flask_unity-0.0.8/flask_unity/static/default_style/media/alert.png` & `flask_unity-0.0.9/flask_unity/static/default_style/media/alert.png`

 * *Files identical despite different names*

### Comparing `flask_unity-0.0.8/flask_unity/static/default_style/media/default_img.png` & `flask_unity-0.0.9/flask_unity/static/default_style/media/default_img.png`

 * *Files identical despite different names*

### Comparing `flask_unity-0.0.8/flask_unity/static/default_style/media/favicon.ico` & `flask_unity-0.0.9/flask_unity/static/default_style/media/favicon.ico`

 * *Files identical despite different names*

### Comparing `flask_unity-0.0.8/flask_unity/templates/default_page/admin_change_password.html` & `flask_unity-0.0.9/flask_unity/templates/default_page/admin_change_password.html`

 * *Files identical despite different names*

### Comparing `flask_unity-0.0.8/flask_unity/templates/default_page/admin_change_profile_image.html` & `flask_unity-0.0.9/flask_unity/templates/default_page/admin_change_profile_image.html`

 * *Files identical despite different names*

### Comparing `flask_unity-0.0.8/flask_unity/templates/default_page/admin_login.html` & `flask_unity-0.0.9/flask_unity/templates/default_page/admin_login.html`

 * *Files identical despite different names*

### Comparing `flask_unity-0.0.8/flask_unity/templates/default_page/admin_register.html` & `flask_unity-0.0.9/flask_unity/templates/default_page/admin_register.html`

 * *Files identical despite different names*

### Comparing `flask_unity-0.0.8/flask_unity/templates/default_page/default.html` & `flask_unity-0.0.9/flask_unity/templates/default_page/default.html`

 * *Files identical despite different names*

### Comparing `flask_unity-0.0.8/flask_unity/templates/default_page/default_base.html` & `flask_unity-0.0.9/flask_unity/templates/default_page/default_base.html`

 * *Files identical despite different names*

### Comparing `flask_unity-0.0.8/flask_unity/templates/default_page/default_index.html` & `flask_unity-0.0.9/flask_unity/templates/default_page/default_index.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 <!-- default index page for your project and app (they `app and project` will inherite it) -->
 {% extends 'default.html' %}
 
 {% block logo %}
   <div class="mini">
     <div class="mini_column">
       <p><pre>  ...........................
-               _____ ______
+           _____ ______
    /  / /|  /   /     /    |/
   /  / / | /   /     /     /
  /__/ /  |/ __/__   /     /
 .............................
 
 </pre></p>
       {% block short_info %}
```

### Comparing `flask_unity-0.0.8/flask_unity/utils.py` & `flask_unity-0.0.9/flask_unity/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
   desc_center = desc.center(len(desc) + 6)
   border = '=' * len(desc_center)
   return [desc_center, border]
   
   
 # Style for flask_unity default pages:
     # ============================
-    #  @ flask_unity software - v0.0.8 
+    #  @ flask_unity software - v0.0.9 
     # ============================
 footer_style = stylePage(__title__, version=__version__)
 
 
 def rem_blueprint(lst_blue=None, rem_blue=None):
   # these are blueprint that we don't want to show on the
   # default page so we are removing them from the list
```

### Comparing `flask_unity-0.0.8/flask_unity.egg-info/PKG-INFO` & `flask_unity-0.0.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: flask-unity
-Version: 0.0.8
+Name: flask_unity
+Version: 0.0.9
 Summary: An extension of flask web framework that erase the complexity of structuring flask project blueprint, packages, and other annoying stuffs
 Home-page: https://flask-unity.readthedocs.io
 Download-URL: https://pypi.org/project/flask-unity
 Author: Usman Musa
 Author-email: usmanmusa1920@gmail.com
 License: MIT
 Project-URL: Documentation, https://flask-unity.readthedocs.io
@@ -28,15 +28,15 @@
 
 # Flask-unity
 
 An extension of flask web framework that erase the complexity of structuring flask project blueprint, packages, and other annoying stuffs.
 
 ## Installation
 
-Install and update the latest release from <a href="https://pypi.org/project/flask-unity">pypi</a>. Basically the library was uploaded using `sdist` (Source Distribution) and this software (library) it might not be compatible with `windows operating system` but it works on other `OS` such as `linux` and `macOS`, but very soon the version that will be compatible with **windows operating system** will be release, stay tuned.
+Install and update the latest release from <a href="https://pypi.org/project/flask-unity">pypi</a>. Basically the library was uploaded using `sdist` (Source Distribution) and this software (library) as from `v0.0.9` it is now compatible and also tested with `windows OS` and others as well, such as `linux`, `macOS` and possibly some others too!.
 
 ```
 pip install --upgrade flask_unity
 ```
 
 ## Create flask project using flask_unity
 
@@ -100,35 +100,37 @@
 
 visit `http://127.0.0.1:5000/admin` this will take you to admin page. From there you are ready to go.
 
 See more documentations <a href="https://flask-unity.readthedocs.io">here!</a>
 
 ### Flask-unity default page
 
-![Flask-unity default page](./media/flask_unity_default_page.png)
-
-### Flask-unity default page
-
 <!-- ![Flask-unity default page](./media/flask_unity_default_page.png) -->
 
-[![Flask-unity default page](https://raw.githubusercontent.com/usmanmusa1920/flask_unity/v0.0.8/media/flask_unity_default_page.png)](https://flask-unity.readthedocs.io)
+[![Flask-unity default page](https://raw.githubusercontent.com/usmanmusa1920/flask_unity/v0.0.9/media/flask_unity_default_page.png)](https://flask-unity.readthedocs.io)
 
 ## Useful links
 
 - Documentation: https://flask-unity.readthedocs.io
 - Repository: https://github.com/usmanmusa1920/flask-unity
 <!-- - PYPI Release: https://pypi.org/project/flask-unity -->
 - Docker example: https://github.com/usmanmusa1920/flask-unity/tree/master/example/flask_unity-docker
 
 Pull requests are welcome
 
 
 # Change Log
 
-## 0.0.8 (07/august/2023)
+## 0.0.9 (07/august/2023)
+
+- Nineth Release
+
+Fixing bugs
+
+Fixing v0.0.8 bugs for OS compatibility, and also tested on windows OS
 
 - Eight Release
 
 OS compatibility
 
 Making flask_unity to be compatible with windows OS as well as other OS
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flask-unity Version: 0.0.8 Summary: An extension of
+Metadata-Version: 2.1 Name: flask_unity Version: 0.0.9 Summary: An extension of
 flask web framework that erase the complexity of structuring flask project
 blueprint, packages, and other annoying stuffs Home-page: https://flask-
 unity.readthedocs.io Download-URL: https://pypi.org/project/flask-unity Author:
 Usman Musa Author-email: usmanmusa1920@gmail.com License: MIT Project-URL:
 Documentation, https://flask-unity.readthedocs.io Project-URL: Source, https://
 github.com/usmanmusa1920/flask-unity Keywords: flask_unity Platform: any
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
@@ -13,61 +13,59 @@
 Language :: Python Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.10 Requires-Python: >=3.6 Description-Content-Type: text/markdown
 License-File: LICENSE # Flask-unity An extension of flask web framework that
 erase the complexity of structuring flask project blueprint, packages, and
 other annoying stuffs. ## Installation Install and update the latest release
 from pypi. Basically the library was uploaded using `sdist` (Source
-Distribution) and this software (library) it might not be compatible with
-`windows operating system` but it works on other `OS` such as `linux` and
-`macOS`, but very soon the version that will be compatible with **windows
-operating system** will be release, stay tuned. ``` pip install --upgrade
-flask_unity ``` ## Create flask project using flask_unity After the
-installation paste the following command on your termianl ``` python -c "from
-flask_unity import project; project('schoolsite')" ``` This will create a
-project called `schoolsite` now cd into the `schoolsite` directory, if you do
-`ls` within the directory you just enter you will see a module called
-`thunder.py` and some directories (some in the form of package) `media`,
-`static`, `templates` and a directory with the same name of your base directory
-name, in our case it is `schoolsite`. Boot up the flask server by running the
-below command ``` python thunder.py boot ``` Now visit the local url `http://
-127.0.0.1:5000` this will show you index page of your project ## Create flask
-app within your project (schoolsite) For you to start an app within your
-project `schoolsite` shutdown the flask development server by pressing ( CTRL+C
-) and then run the following command, by giving the name you want your app to
-be, in our case we will call our app `exam` ``` python thunder.py create_app -
-a exam ``` this will create an app (a new package called `exam`) within your
-project `(schoolsite)` ## Register an app Once the app is created open a file
-`schoolsite/routes.py` and import your `exam` blueprint which is in (`exam/
-views.py`), default name given to an app blueprint, is the app name so our
-`exam` app blueprint name is `exam`, after importing it, append (register) the
-app blueprint in a list called `reg_blueprints` in that same file of
-`schoolsite/routes.py` importing blueprint ```py from exam.views import exam
-``` registering blueprint ```py reg_blueprints = [ blueprint.default,
-blueprint.errors, blueprint.auth, base, exam, ] ``` once you register the app,
-boot up the flask webserver again by ``` python thunder.py boot ``` visit
-`http://127.0.0.1:5000` which is your project landing page visit `http://
-127.0.0.1:5000/exam` this will take you to your app landing page (exam) visit
-`http://127.0.0.1:5000/admin` this will take you to admin page. From there you
-are ready to go. See more documentations here! ### Flask-unity default page !
-[Flask-unity default page](./media/flask_unity_default_page.png) ### Flask-
-unity default page  [![Flask-unity default page](https://
-raw.githubusercontent.com/usmanmusa1920/flask_unity/v0.0.8/media/
+Distribution) and this software (library) as from `v0.0.9` it is now compatible
+and also tested with `windows OS` and others as well, such as `linux`, `macOS`
+and possibly some others too!. ``` pip install --upgrade flask_unity ``` ##
+Create flask project using flask_unity After the installation paste the
+following command on your termianl ``` python -c "from flask_unity import
+project; project('schoolsite')" ``` This will create a project called
+`schoolsite` now cd into the `schoolsite` directory, if you do `ls` within the
+directory you just enter you will see a module called `thunder.py` and some
+directories (some in the form of package) `media`, `static`, `templates` and a
+directory with the same name of your base directory name, in our case it is
+`schoolsite`. Boot up the flask server by running the below command ``` python
+thunder.py boot ``` Now visit the local url `http://127.0.0.1:5000` this will
+show you index page of your project ## Create flask app within your project
+(schoolsite) For you to start an app within your project `schoolsite` shutdown
+the flask development server by pressing ( CTRL+C ) and then run the following
+command, by giving the name you want your app to be, in our case we will call
+our app `exam` ``` python thunder.py create_app -a exam ``` this will create an
+app (a new package called `exam`) within your project `(schoolsite)` ##
+Register an app Once the app is created open a file `schoolsite/routes.py` and
+import your `exam` blueprint which is in (`exam/views.py`), default name given
+to an app blueprint, is the app name so our `exam` app blueprint name is
+`exam`, after importing it, append (register) the app blueprint in a list
+called `reg_blueprints` in that same file of `schoolsite/routes.py` importing
+blueprint ```py from exam.views import exam ``` registering blueprint ```py
+reg_blueprints = [ blueprint.default, blueprint.errors, blueprint.auth, base,
+exam, ] ``` once you register the app, boot up the flask webserver again by ```
+python thunder.py boot ``` visit `http://127.0.0.1:5000` which is your project
+landing page visit `http://127.0.0.1:5000/exam` this will take you to your app
+landing page (exam) visit `http://127.0.0.1:5000/admin` this will take you to
+admin page. From there you are ready to go. See more documentations here! ###
+Flask-unity default page  [![Flask-unity default page](https://
+raw.githubusercontent.com/usmanmusa1920/flask_unity/v0.0.9/media/
 flask_unity_default_page.png)](https://flask-unity.readthedocs.io) ## Useful
 links - Documentation: https://flask-unity.readthedocs.io - Repository: https:/
 /github.com/usmanmusa1920/flask-unity  - Docker example: https://github.com/
 usmanmusa1920/flask-unity/tree/master/example/flask_unity-docker Pull requests
-are welcome # Change Log ## 0.0.8 (07/august/2023) - Eight Release OS
-compatibility Making flask_unity to be compatible with windows OS as well as
-other OS ## 0.0.7 (07/august/2023) - Seventh Release This release mostly is for
-adding more docs and examples. - Sixth Release Alembic is included as
-dependency (in the require module list). - Fifth Release In fifith release, we
-handle how default user file system tricks is, things like when user change his
-profile picture. - Fourth Release In this release we handle how we can
-customise the admin html page by inheriting (extends) it in our project
+are welcome # Change Log ## 0.0.9 (07/august/2023) - Nineth Release Fixing bugs
+Fixing v0.0.8 bugs for OS compatibility, and also tested on windows OS - Eight
+Release OS compatibility Making flask_unity to be compatible with windows OS as
+well as other OS ## 0.0.7 (07/august/2023) - Seventh Release This release
+mostly is for adding more docs and examples. - Sixth Release Alembic is
+included as dependency (in the require module list). - Fifth Release In fifith
+release, we handle how default user file system tricks is, things like when
+user change his profile picture. - Fourth Release In this release we handle how
+we can customise the admin html page by inheriting (extends) it in our project
 templates/admin directory, and the admin page on how to bind models in the
 admin. Also I refactor other libraries that this package needs with their
 corresponding versions in the setup.py and requirements.txt files. In this
 release good documentations is well packed. Database migration is added using
 `alembic` Some error pages, default page were added but still you can customise
 it in your project sub folder (the package with the same name of your project
 in your project directory) in a file called `route.py`. Also an admin directory
```

### Comparing `flask_unity-0.0.8/flask_unity.egg-info/SOURCES.txt` & `flask_unity-0.0.9/flask_unity.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flask_unity-0.0.8/setup.py` & `flask_unity-0.0.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
 
 from setuptools import setup
 from setuptools import find_packages
 
 
 setup(
-  name = 'flask_unity', # name of the main package (base folder i.e flask_unity)
-  version = '0.0.8',
+  name = 'flask_unity', # name of the main package (base folderflask_unitylask_unity)
+  version = '0.0.9',
   description = 'An extension of flask web framework that erase the complexity of structuring flask project blueprint, packages, and other annoying stuffs',
   long_description = open('README.md').read() + '\n\n' + open('CHANGELOG').read(),
   long_description_content_type='text/markdown',
   python_requires = '>=3.6',
   platforms='any',
   
   url = 'https://flask-unity.readthedocs.io',
```

