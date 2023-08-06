# Comparing `tmp/canned-views-0.1.7.tar.gz` & `tmp/canned-views-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "canned-views-0.1.7.tar", last modified: Wed Aug 10 12:12:13 2022, max compression
+gzip compressed data, was "canned-views-0.1.8.tar", last modified: Sun Aug  6 22:56:43 2023, max compression
```

## Comparing `canned-views-0.1.7.tar` & `canned-views-0.1.8.tar`

### file list

```diff
@@ -1,76 +1,83 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-10 12:12:13.885326 canned-views-0.1.7/
--rw-r--r--   0 erikvw     (501) staff       (20)       96 2022-06-16 12:00:21.000000 canned-views-0.1.7/.coveragerc
--rw-r--r--   0 erikvw     (501) staff       (20)      436 2022-06-16 12:00:21.000000 canned-views-0.1.7/.editorconfig
--rw-r--r--   0 erikvw     (501) staff       (20)     1843 2022-06-16 12:00:21.000000 canned-views-0.1.7/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-16 12:00:21.000000 canned-views-0.1.7/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-16 12:00:21.000000 canned-views-0.1.7/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35149 2022-06-09 17:03:14.000000 canned-views-0.1.7/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-06-16 12:00:21.000000 canned-views-0.1.7/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)     1798 2022-08-10 12:12:13.885454 canned-views-0.1.7/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)      939 2022-06-26 09:28:45.000000 canned-views-0.1.7/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-08-10 12:12:05.000000 canned-views-0.1.7/VERSION
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-10 12:12:13.878602 canned-views-0.1.7/canned_views/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-16 12:00:21.000000 canned-views-0.1.7/canned_views/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2496 2022-08-10 12:12:05.000000 canned-views-0.1.7/canned_views/admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      169 2022-06-16 12:00:21.000000 canned-views-0.1.7/canned_views/admin_site.py
--rw-r--r--   0 erikvw     (501) staff       (20)      282 2022-06-16 12:00:21.000000 canned-views-0.1.7/canned_views/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)      960 2022-06-26 09:28:45.000000 canned-views-0.1.7/canned_views/auth_objects.py
--rw-r--r--   0 erikvw     (501) staff       (20)      509 2022-06-26 09:28:45.000000 canned-views-0.1.7/canned_views/auths.py
--rw-r--r--   0 erikvw     (501) staff       (20)       36 2022-06-16 12:00:21.000000 canned-views-0.1.7/canned_views/constants.py
--rw-r--r--   0 erikvw     (501) staff       (20)      796 2022-06-26 09:28:45.000000 canned-views-0.1.7/canned_views/forms.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-10 12:12:13.882020 canned-views-0.1.7/canned_views/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)     6831 2022-06-16 12:00:21.000000 canned-views-0.1.7/canned_views/migrations/0001_initial.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1761 2022-06-17 01:59:24.000000 canned-views-0.1.7/canned_views/migrations/0002_cannedviews_columns_cannedviews_order_by_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)      943 2022-06-17 01:59:24.000000 canned-views-0.1.7/canned_views/migrations/0003_remove_cannedviews_columns_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1504 2022-06-17 21:05:12.000000 canned-views-0.1.7/canned_views/migrations/0004_auto_20220617_2306.py
--rw-r--r--   0 erikvw     (501) staff       (20)      565 2022-06-17 21:05:12.000000 canned-views-0.1.7/canned_views/migrations/0005_auto_20220617_2344.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2486 2022-06-26 09:28:45.000000 canned-views-0.1.7/canned_views/migrations/0006_cannedviews_filter_by_current_site_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4905 2022-06-26 09:28:45.000000 canned-views-0.1.7/canned_views/migrations/0007_cannedviews_linked_column_name_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)      646 2022-06-26 09:28:45.000000 canned-views-0.1.7/canned_views/migrations/0008_rename_cannedviews_cannedview_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)      814 2022-07-04 15:46:45.000000 canned-views-0.1.7/canned_views/migrations/0009_auto_20220704_1841.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-16 12:00:21.000000 canned-views-0.1.7/canned_views/migrations/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2598 2022-06-26 09:28:45.000000 canned-views-0.1.7/canned_views/models.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-10 12:12:13.871749 canned-views-0.1.7/canned_views/templates/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-10 12:12:13.882826 canned-views-0.1.7/canned_views/templates/canned_views/
--rw-r--r--   0 erikvw     (501) staff       (20)     5530 2022-07-18 18:08:14.000000 canned-views-0.1.7/canned_views/templates/canned_views/base.html
--rw-r--r--   0 erikvw     (501) staff       (20)     1419 2022-06-17 21:05:12.000000 canned-views-0.1.7/canned_views/templates/canned_views/base_dj3.html
--rw-r--r--   0 erikvw     (501) staff       (20)      222 2022-06-16 12:00:21.000000 canned-views-0.1.7/canned_views/templates/canned_views/button.html
--rw-r--r--   0 erikvw     (501) staff       (20)     1806 2022-06-26 09:28:45.000000 canned-views-0.1.7/canned_views/templates/canned_views/canned_view.html
--rw-r--r--   0 erikvw     (501) staff       (20)      994 2022-06-26 09:28:45.000000 canned-views-0.1.7/canned_views/templates/canned_views/home.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-10 12:12:13.883045 canned-views-0.1.7/canned_views/templatetags/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-16 12:00:21.000000 canned-views-0.1.7/canned_views/templatetags/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1758 2022-06-26 09:28:45.000000 canned-views-0.1.7/canned_views/templatetags/canned_extras.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-10 12:12:13.883193 canned-views-0.1.7/canned_views/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-17 21:05:12.000000 canned-views-0.1.7/canned_views/tests/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-10 12:12:13.883273 canned-views-0.1.7/canned_views/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-17 21:05:12.000000 canned-views-0.1.7/canned_views/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      323 2022-06-17 21:05:12.000000 canned-views-0.1.7/canned_views/urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)     6977 2022-06-26 09:28:45.000000 canned-views-0.1.7/canned_views/utils.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-10 12:12:13.883603 canned-views-0.1.7/canned_views/views/
--rw-r--r--   0 erikvw     (501) staff       (20)       66 2022-06-17 01:59:24.000000 canned-views-0.1.7/canned_views/views/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2079 2022-06-26 09:28:45.000000 canned-views-0.1.7/canned_views/views/basic_view.py
--rw-r--r--   0 erikvw     (501) staff       (20)      961 2022-06-26 09:28:45.000000 canned-views-0.1.7/canned_views/views/home_view.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-10 12:12:13.879377 canned-views-0.1.7/canned_views.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)     1798 2022-08-10 12:12:13.000000 canned-views-0.1.7/canned_views.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     2035 2022-08-10 12:12:13.000000 canned-views-0.1.7/canned_views.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-08-10 12:12:13.000000 canned-views-0.1.7/canned_views.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-06-16 11:55:19.000000 canned-views-0.1.7/canned_views.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)       13 2022-08-10 12:12:13.000000 canned-views-0.1.7/canned_views.egg-info/requires.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       30 2022-08-10 12:12:13.000000 canned-views-0.1.7/canned_views.egg-info/top_level.txt
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-10 12:12:13.884836 canned-views-0.1.7/canned_views_app/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-16 12:00:21.000000 canned-views-0.1.7/canned_views_app/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      250 2022-06-16 12:00:21.000000 canned-views-0.1.7/canned_views_app/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)      382 2022-06-16 12:00:21.000000 canned-views-0.1.7/canned_views_app/asgi.py
--rwxr-xr-x   0 erikvw     (501) staff       (20)      672 2022-06-17 01:59:24.000000 canned-views-0.1.7/canned_views_app/manage.py
--rw-r--r--   0 erikvw     (501) staff       (20)      249 2022-06-17 01:59:24.000000 canned-views-0.1.7/canned_views_app/navbars.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4900 2022-06-16 12:00:21.000000 canned-views-0.1.7/canned_views_app/settings.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-10 12:12:13.872127 canned-views-0.1.7/canned_views_app/templates/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-10 12:12:13.885094 canned-views-0.1.7/canned_views_app/templates/canned_views_app/
--rw-r--r--   0 erikvw     (501) staff       (20)      109 2022-06-16 12:00:21.000000 canned-views-0.1.7/canned_views_app/templates/canned_views_app/base.html
--rw-r--r--   0 erikvw     (501) staff       (20)     1200 2022-06-16 19:47:16.000000 canned-views-0.1.7/canned_views_app/templates/canned_views_app/home.html
--rw-r--r--   0 erikvw     (501) staff       (20)     1114 2022-06-16 12:00:21.000000 canned-views-0.1.7/canned_views_app/urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)      356 2022-06-16 12:00:21.000000 canned-views-0.1.7/canned_views_app/views.py
--rw-r--r--   0 erikvw     (501) staff       (20)      382 2022-06-16 12:00:21.000000 canned-views-0.1.7/canned_views_app/wsgi.py
--rw-r--r--   0 erikvw     (501) staff       (20)      164 2022-06-16 12:00:21.000000 canned-views-0.1.7/codecov.yml
--rw-r--r--   0 erikvw     (501) staff       (20)     1585 2022-06-16 12:00:21.000000 canned-views-0.1.7/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)     1188 2022-08-10 12:12:13.885808 canned-views-0.1.7/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-06 22:56:43.811105 canned-views-0.1.8/
+-rw-r--r--   0 erikvw     (501) staff       (20)       96 2022-06-16 12:00:21.000000 canned-views-0.1.8/.coveragerc
+-rw-r--r--   0 erikvw     (501) staff       (20)      436 2022-06-16 12:00:21.000000 canned-views-0.1.8/.editorconfig
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-06 22:56:43.799358 canned-views-0.1.8/.github/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-06 22:56:43.802936 canned-views-0.1.8/.github/workflows/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1935 2023-08-06 22:56:36.000000 canned-views-0.1.8/.github/workflows/build.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1843 2022-06-16 12:00:21.000000 canned-views-0.1.8/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1077 2023-08-06 22:56:36.000000 canned-views-0.1.8/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2023-08-06 22:56:36.000000 canned-views-0.1.8/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-16 12:00:21.000000 canned-views-0.1.8/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-16 12:00:21.000000 canned-views-0.1.8/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35149 2022-06-09 17:03:14.000000 canned-views-0.1.8/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-06-16 12:00:21.000000 canned-views-0.1.8/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)     1750 2023-08-06 22:56:43.811200 canned-views-0.1.8/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)      939 2022-06-26 09:28:45.000000 canned-views-0.1.8/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-08-10 12:12:05.000000 canned-views-0.1.8/VERSION
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-06 22:56:43.804725 canned-views-0.1.8/canned_views/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-16 12:00:21.000000 canned-views-0.1.8/canned_views/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2582 2023-08-06 22:56:36.000000 canned-views-0.1.8/canned_views/admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      169 2022-06-16 12:00:21.000000 canned-views-0.1.8/canned_views/admin_site.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      282 2022-06-16 12:00:21.000000 canned-views-0.1.8/canned_views/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      960 2022-06-26 09:28:45.000000 canned-views-0.1.8/canned_views/auth_objects.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      509 2022-06-26 09:28:45.000000 canned-views-0.1.8/canned_views/auths.py
+-rw-r--r--   0 erikvw     (501) staff       (20)       36 2022-06-16 12:00:21.000000 canned-views-0.1.8/canned_views/constants.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      796 2022-06-26 09:28:45.000000 canned-views-0.1.8/canned_views/forms.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-06 22:56:43.807162 canned-views-0.1.8/canned_views/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)    11107 2023-08-06 22:56:36.000000 canned-views-0.1.8/canned_views/migrations/0001_initial.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2074 2023-08-06 22:56:36.000000 canned-views-0.1.8/canned_views/migrations/0002_cannedviews_columns_cannedviews_order_by_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      942 2023-08-06 22:56:36.000000 canned-views-0.1.8/canned_views/migrations/0003_remove_cannedviews_columns_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1787 2023-08-06 22:56:36.000000 canned-views-0.1.8/canned_views/migrations/0004_auto_20220617_2306.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      564 2023-08-06 22:56:36.000000 canned-views-0.1.8/canned_views/migrations/0005_auto_20220617_2344.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2703 2023-08-06 22:56:36.000000 canned-views-0.1.8/canned_views/migrations/0006_cannedviews_filter_by_current_site_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5720 2023-08-06 22:56:36.000000 canned-views-0.1.8/canned_views/migrations/0007_cannedviews_linked_column_name_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      645 2023-08-06 22:56:36.000000 canned-views-0.1.8/canned_views/migrations/0008_rename_cannedviews_cannedview_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      814 2022-07-04 15:46:45.000000 canned-views-0.1.8/canned_views/migrations/0009_auto_20220704_1841.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      604 2023-08-06 22:56:36.000000 canned-views-0.1.8/canned_views/migrations/0010_alter_cannedview_managers.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      841 2023-08-06 22:56:36.000000 canned-views-0.1.8/canned_views/migrations/0011_alter_cannedview_options.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-16 12:00:21.000000 canned-views-0.1.8/canned_views/migrations/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2598 2022-06-26 09:28:45.000000 canned-views-0.1.8/canned_views/models.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-06 22:56:43.799681 canned-views-0.1.8/canned_views/templates/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-06 22:56:43.807991 canned-views-0.1.8/canned_views/templates/canned_views/
+-rw-r--r--   0 erikvw     (501) staff       (20)     5530 2022-07-18 18:08:14.000000 canned-views-0.1.8/canned_views/templates/canned_views/base.html
+-rw-r--r--   0 erikvw     (501) staff       (20)     1419 2022-06-17 21:05:12.000000 canned-views-0.1.8/canned_views/templates/canned_views/base_dj3.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      222 2022-06-16 12:00:21.000000 canned-views-0.1.8/canned_views/templates/canned_views/button.html
+-rw-r--r--   0 erikvw     (501) staff       (20)     1806 2022-06-26 09:28:45.000000 canned-views-0.1.8/canned_views/templates/canned_views/canned_view.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      994 2022-06-26 09:28:45.000000 canned-views-0.1.8/canned_views/templates/canned_views/home.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-06 22:56:43.808240 canned-views-0.1.8/canned_views/templatetags/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-16 12:00:21.000000 canned-views-0.1.8/canned_views/templatetags/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1758 2022-06-26 09:28:45.000000 canned-views-0.1.8/canned_views/templatetags/canned_extras.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-06 22:56:43.808393 canned-views-0.1.8/canned_views/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-17 21:05:12.000000 canned-views-0.1.8/canned_views/tests/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-06 22:56:43.808482 canned-views-0.1.8/canned_views/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-17 21:05:12.000000 canned-views-0.1.8/canned_views/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      323 2022-06-17 21:05:12.000000 canned-views-0.1.8/canned_views/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     7012 2023-08-06 22:56:36.000000 canned-views-0.1.8/canned_views/utils.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-06 22:56:43.809046 canned-views-0.1.8/canned_views/views/
+-rw-r--r--   0 erikvw     (501) staff       (20)       66 2022-06-17 01:59:24.000000 canned-views-0.1.8/canned_views/views/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2079 2022-06-26 09:28:45.000000 canned-views-0.1.8/canned_views/views/basic_view.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      961 2022-06-26 09:28:45.000000 canned-views-0.1.8/canned_views/views/home_view.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-06 22:56:43.805594 canned-views-0.1.8/canned_views.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1750 2023-08-06 22:56:43.000000 canned-views-0.1.8/canned_views.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     2212 2023-08-06 22:56:43.000000 canned-views-0.1.8/canned_views.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-08-06 22:56:43.000000 canned-views-0.1.8/canned_views.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-06-16 11:55:19.000000 canned-views-0.1.8/canned_views.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)       13 2023-08-06 22:56:43.000000 canned-views-0.1.8/canned_views.egg-info/requires.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       30 2023-08-06 22:56:43.000000 canned-views-0.1.8/canned_views.egg-info/top_level.txt
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-06 22:56:43.810474 canned-views-0.1.8/canned_views_app/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-16 12:00:21.000000 canned-views-0.1.8/canned_views_app/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      250 2022-06-16 12:00:21.000000 canned-views-0.1.8/canned_views_app/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      382 2022-06-16 12:00:21.000000 canned-views-0.1.8/canned_views_app/asgi.py
+-rwxr-xr-x   0 erikvw     (501) staff       (20)      672 2022-06-17 01:59:24.000000 canned-views-0.1.8/canned_views_app/manage.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      249 2022-06-17 01:59:24.000000 canned-views-0.1.8/canned_views_app/navbars.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4232 2023-08-06 22:56:36.000000 canned-views-0.1.8/canned_views_app/settings.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-06 22:56:43.800122 canned-views-0.1.8/canned_views_app/templates/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-06 22:56:43.810835 canned-views-0.1.8/canned_views_app/templates/canned_views_app/
+-rw-r--r--   0 erikvw     (501) staff       (20)      109 2022-06-16 12:00:21.000000 canned-views-0.1.8/canned_views_app/templates/canned_views_app/base.html
+-rw-r--r--   0 erikvw     (501) staff       (20)     1200 2022-06-16 19:47:16.000000 canned-views-0.1.8/canned_views_app/templates/canned_views_app/home.html
+-rw-r--r--   0 erikvw     (501) staff       (20)     1114 2022-06-16 12:00:21.000000 canned-views-0.1.8/canned_views_app/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      356 2022-06-16 12:00:21.000000 canned-views-0.1.8/canned_views_app/views.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      382 2022-06-16 12:00:21.000000 canned-views-0.1.8/canned_views_app/wsgi.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      168 2023-08-06 22:56:36.000000 canned-views-0.1.8/codecov.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1642 2023-08-06 22:56:36.000000 canned-views-0.1.8/pyproject.toml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1153 2023-08-06 22:56:43.811511 canned-views-0.1.8/setup.cfg
```

### Comparing `canned-views-0.1.7/.gitignore` & `canned-views-0.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `canned-views-0.1.7/LICENSE` & `canned-views-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `canned-views-0.1.7/PKG-INFO` & `canned-views-0.1.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: canned-views
-Version: 0.1.7
+Version: 0.1.8
 Summary: SQL views presented as simple Django ListView reports
 Home-page: https://github.com/erikvw/canned-views
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django sql view ListView,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.1
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Requires-Python: >=3.9
+Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
 
 Canned Views
 ------------
```

### Comparing `canned-views-0.1.7/README.rst` & `canned-views-0.1.8/README.rst`

 * *Files identical despite different names*

### Comparing `canned-views-0.1.7/canned_views/admin.py` & `canned-views-0.1.8/canned_views/admin.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,21 @@
+from typing import Tuple
+
 from django.contrib import admin
 from django.template.loader import render_to_string
 from django.urls import reverse
 
 from .admin_site import canned_views_admin
 from .auth_objects import CANNED_VIEW_SUPER_ROLE
 from .forms import CannedViewsForm
 from .models import CannedView
 
 
 @admin.register(CannedView, site=canned_views_admin)
 class CannedViewAdmin(admin.ModelAdmin):
-
     form = CannedViewsForm
 
     fieldsets = (
         (
             None,
             (
                 {
@@ -42,26 +43,26 @@
                         "reverse_url_args",
                     )
                 }
             ),
         ),
     )
 
-    list_display = [
+    list_display: Tuple[str, ...] = (
         "display_name",
         "list_view",
         "description",
         "sql_view_name",
-    ]
+    )
 
-    search_fields = ("name", "display_name", "sql_view_name")
+    search_fields: Tuple[str, ...] = ("name", "display_name", "sql_view_name")
 
-    readonly_fields = ("sql_view_name", "sql_select_columns")
+    readonly_fields: Tuple[str, ...] = ("sql_view_name", "sql_select_columns")
 
-    def get_readonly_fields(self, request, obj=None) -> tuple:
+    def get_readonly_fields(self, request, obj=None) -> Tuple[str, ...]:
         readonly_fields = super().get_readonly_fields(request, obj=obj) or ()
         try:
             roles = request.user.userprofile.roles.all()
         except AttributeError:
             pass
         else:
             role_names = tuple(role.name for role in roles)
```

### Comparing `canned-views-0.1.7/canned_views/auth_objects.py` & `canned-views-0.1.8/canned_views/auth_objects.py`

 * *Files identical despite different names*

### Comparing `canned-views-0.1.7/canned_views/forms.py` & `canned-views-0.1.8/canned_views/forms.py`

 * *Files identical despite different names*

### Comparing `canned-views-0.1.7/canned_views/migrations/0003_remove_cannedviews_columns_and_more.py` & `canned-views-0.1.8/canned_views/migrations/0003_remove_cannedviews_columns_and_more.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 # Generated by Django 4.0.5 on 2022-06-16 16:17
 
 from django.db import migrations
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
-        ('canned_views', '0002_cannedviews_columns_cannedviews_order_by_and_more'),
+        ("canned_views", "0002_cannedviews_columns_cannedviews_order_by_and_more"),
     ]
 
     operations = [
         migrations.RemoveField(
-            model_name='cannedviews',
-            name='columns',
+            model_name="cannedviews",
+            name="columns",
         ),
         migrations.RemoveField(
-            model_name='cannedviews',
-            name='order_by',
+            model_name="cannedviews",
+            name="order_by",
         ),
         migrations.RemoveField(
-            model_name='cannedviews',
-            name='where',
+            model_name="cannedviews",
+            name="where",
         ),
         migrations.RemoveField(
-            model_name='historicalcannedviews',
-            name='columns',
+            model_name="historicalcannedviews",
+            name="columns",
         ),
         migrations.RemoveField(
-            model_name='historicalcannedviews',
-            name='order_by',
+            model_name="historicalcannedviews",
+            name="order_by",
         ),
         migrations.RemoveField(
-            model_name='historicalcannedviews',
-            name='where',
+            model_name="historicalcannedviews",
+            name="where",
         ),
     ]
```

### Comparing `canned-views-0.1.7/canned_views/migrations/0004_auto_20220617_2306.py` & `canned-views-0.1.8/canned_views/migrations/0004_auto_20220617_2306.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,51 @@
 # Generated by Django 3.2.13 on 2022-06-17 20:06
 
 import django.core.validators
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
-        ('canned_views', '0003_remove_cannedviews_columns_and_more'),
+        ("canned_views", "0003_remove_cannedviews_columns_and_more"),
     ]
 
     operations = [
         migrations.AddField(
-            model_name='cannedviews',
-            name='sql_select_columns',
-            field=models.TextField(blank=True, help_text='Comma separated list of field names for the SQL SELECT. All lowercase, no spaces', null=True, validators=[django.core.validators.RegexValidator(regex='^([a-z0-9_,])+$')]),
+            model_name="cannedviews",
+            name="sql_select_columns",
+            field=models.TextField(
+                blank=True,
+                help_text="Comma separated list of field names for the SQL SELECT. All lowercase, no spaces",
+                null=True,
+                validators=[django.core.validators.RegexValidator(regex="^([a-z0-9_,])+$")],
+            ),
         ),
         migrations.AddField(
-            model_name='historicalcannedviews',
-            name='sql_select_columns',
-            field=models.TextField(blank=True, help_text='Comma separated list of field names for the SQL SELECT. All lowercase, no spaces', null=True, validators=[django.core.validators.RegexValidator(regex='^([a-z0-9_,])+$')]),
+            model_name="historicalcannedviews",
+            name="sql_select_columns",
+            field=models.TextField(
+                blank=True,
+                help_text="Comma separated list of field names for the SQL SELECT. All lowercase, no spaces",
+                null=True,
+                validators=[django.core.validators.RegexValidator(regex="^([a-z0-9_,])+$")],
+            ),
         ),
         migrations.AlterField(
-            model_name='cannedviews',
-            name='sql_view_name',
-            field=models.CharField(max_length=50, null=True, validators=[django.core.validators.RegexValidator(regex='^([a-z0-9_])+$')]),
+            model_name="cannedviews",
+            name="sql_view_name",
+            field=models.CharField(
+                max_length=50,
+                null=True,
+                validators=[django.core.validators.RegexValidator(regex="^([a-z0-9_])+$")],
+            ),
         ),
         migrations.AlterField(
-            model_name='historicalcannedviews',
-            name='sql_view_name',
-            field=models.CharField(max_length=50, null=True, validators=[django.core.validators.RegexValidator(regex='^([a-z0-9_])+$')]),
+            model_name="historicalcannedviews",
+            name="sql_view_name",
+            field=models.CharField(
+                max_length=50,
+                null=True,
+                validators=[django.core.validators.RegexValidator(regex="^([a-z0-9_])+$")],
+            ),
         ),
     ]
```

### Comparing `canned-views-0.1.7/canned_views/migrations/0005_auto_20220617_2344.py` & `canned-views-0.1.8/canned_views/migrations/0005_auto_20220617_2344.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 # Generated by Django 3.2.13 on 2022-06-17 20:44
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
-        ('canned_views', '0004_auto_20220617_2306'),
+        ("canned_views", "0004_auto_20220617_2306"),
     ]
 
     operations = [
         migrations.AddField(
-            model_name='cannedviews',
-            name='instructions',
+            model_name="cannedviews",
+            name="instructions",
             field=models.TextField(null=True),
         ),
         migrations.AddField(
-            model_name='historicalcannedviews',
-            name='instructions',
+            model_name="historicalcannedviews",
+            name="instructions",
             field=models.TextField(null=True),
         ),
     ]
```

### Comparing `canned-views-0.1.7/canned_views/migrations/0006_cannedviews_filter_by_current_site_and_more.py` & `canned-views-0.1.8/canned_views/migrations/0006_cannedviews_filter_by_current_site_and_more.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,64 +1,77 @@
 # Generated by Django 4.0.5 on 2022-06-25 18:48
 
 import django.core.validators
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
-        ('canned_views', '0005_auto_20220617_2344'),
+        ("canned_views", "0005_auto_20220617_2344"),
     ]
 
     operations = [
         migrations.AddField(
-            model_name='cannedviews',
-            name='filter_by_current_site',
-            field=models.CharField(choices=[('Yes', 'Yes'), ('No', 'No')], default='No', max_length=10),
+            model_name="cannedviews",
+            name="filter_by_current_site",
+            field=models.CharField(
+                choices=[("Yes", "Yes"), ("No", "No")], default="No", max_length=10
+            ),
         ),
         migrations.AddField(
-            model_name='historicalcannedviews',
-            name='filter_by_current_site',
-            field=models.CharField(choices=[('Yes', 'Yes'), ('No', 'No')], default='No', max_length=10),
+            model_name="historicalcannedviews",
+            name="filter_by_current_site",
+            field=models.CharField(
+                choices=[("Yes", "Yes"), ("No", "No")], default="No", max_length=10
+            ),
         ),
         migrations.AlterField(
-            model_name='cannedviews',
-            name='description',
+            model_name="cannedviews",
+            name="description",
             field=models.TextField(blank=True, null=True),
         ),
         migrations.AlterField(
-            model_name='cannedviews',
-            name='display_name',
+            model_name="cannedviews",
+            name="display_name",
             field=models.CharField(blank=True, max_length=30),
         ),
         migrations.AlterField(
-            model_name='cannedviews',
-            name='instructions',
+            model_name="cannedviews",
+            name="instructions",
             field=models.TextField(blank=True, null=True),
         ),
         migrations.AlterField(
-            model_name='cannedviews',
-            name='sql_select_columns',
-            field=models.TextField(blank=True, help_text='Comma separated list of field names for the SQL SELECT. All lowercase', null=True, validators=[django.core.validators.RegexValidator(regex='^([a-z0-9_, ])+$')]),
+            model_name="cannedviews",
+            name="sql_select_columns",
+            field=models.TextField(
+                blank=True,
+                help_text="Comma separated list of field names for the SQL SELECT. All lowercase",
+                null=True,
+                validators=[django.core.validators.RegexValidator(regex="^([a-z0-9_, ])+$")],
+            ),
         ),
         migrations.AlterField(
-            model_name='historicalcannedviews',
-            name='description',
+            model_name="historicalcannedviews",
+            name="description",
             field=models.TextField(blank=True, null=True),
         ),
         migrations.AlterField(
-            model_name='historicalcannedviews',
-            name='display_name',
+            model_name="historicalcannedviews",
+            name="display_name",
             field=models.CharField(blank=True, max_length=30),
         ),
         migrations.AlterField(
-            model_name='historicalcannedviews',
-            name='instructions',
+            model_name="historicalcannedviews",
+            name="instructions",
             field=models.TextField(blank=True, null=True),
         ),
         migrations.AlterField(
-            model_name='historicalcannedviews',
-            name='sql_select_columns',
-            field=models.TextField(blank=True, help_text='Comma separated list of field names for the SQL SELECT. All lowercase', null=True, validators=[django.core.validators.RegexValidator(regex='^([a-z0-9_, ])+$')]),
+            model_name="historicalcannedviews",
+            name="sql_select_columns",
+            field=models.TextField(
+                blank=True,
+                help_text="Comma separated list of field names for the SQL SELECT. All lowercase",
+                null=True,
+                validators=[django.core.validators.RegexValidator(regex="^([a-z0-9_, ])+$")],
+            ),
         ),
     ]
```

### Comparing `canned-views-0.1.7/canned_views/migrations/0007_cannedviews_linked_column_name_and_more.py` & `canned-views-0.1.8/canned_views/migrations/0007_cannedviews_linked_column_name_and_more.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,104 +1,155 @@
 # Generated by Django 4.0.5 on 2022-06-26 07:50
 
 import django.core.validators
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
-        ('canned_views', '0006_cannedviews_filter_by_current_site_and_more'),
+        ("canned_views", "0006_cannedviews_filter_by_current_site_and_more"),
     ]
 
     operations = [
         migrations.AddField(
-            model_name='cannedviews',
-            name='linked_column_name',
-            field=models.CharField(default='subject_identifier', max_length=50),
+            model_name="cannedviews",
+            name="linked_column_name",
+            field=models.CharField(default="subject_identifier", max_length=50),
         ),
         migrations.AddField(
-            model_name='cannedviews',
-            name='reverse_url',
-            field=models.CharField(choices=[('Yes', 'Yes'), ('No', 'No')], default='No', max_length=10),
+            model_name="cannedviews",
+            name="reverse_url",
+            field=models.CharField(
+                choices=[("Yes", "Yes"), ("No", "No")], default="No", max_length=10
+            ),
         ),
         migrations.AddField(
-            model_name='cannedviews',
-            name='reverse_url_args',
-            field=models.CharField(help_text='column names separated by comma. For example, subject_identifier,visit_code,visit_code_sequence,visit_schedule_name,schedule_name.', max_length=500, null=True),
+            model_name="cannedviews",
+            name="reverse_url_args",
+            field=models.CharField(
+                help_text="column names separated by comma. For example, subject_identifier,visit_code,visit_code_sequence,visit_schedule_name,schedule_name.",
+                max_length=500,
+                null=True,
+            ),
         ),
         migrations.AddField(
-            model_name='cannedviews',
-            name='reverse_url_name',
-            field=models.CharField(help_text='a valid url name as a `key` for the `value` stored in the `url_names` dictionary. For example, `subject_dashboard_url`.', max_length=50, null=True),
+            model_name="cannedviews",
+            name="reverse_url_name",
+            field=models.CharField(
+                help_text="a valid url name as a `key` for the `value` stored in the `url_names` dictionary. For example, `subject_dashboard_url`.",
+                max_length=50,
+                null=True,
+            ),
         ),
         migrations.AddField(
-            model_name='historicalcannedviews',
-            name='linked_column_name',
-            field=models.CharField(default='subject_identifier', max_length=50),
+            model_name="historicalcannedviews",
+            name="linked_column_name",
+            field=models.CharField(default="subject_identifier", max_length=50),
         ),
         migrations.AddField(
-            model_name='historicalcannedviews',
-            name='reverse_url',
-            field=models.CharField(choices=[('Yes', 'Yes'), ('No', 'No')], default='No', max_length=10),
+            model_name="historicalcannedviews",
+            name="reverse_url",
+            field=models.CharField(
+                choices=[("Yes", "Yes"), ("No", "No")], default="No", max_length=10
+            ),
         ),
         migrations.AddField(
-            model_name='historicalcannedviews',
-            name='reverse_url_args',
-            field=models.CharField(help_text='column names separated by comma. For example, subject_identifier,visit_code,visit_code_sequence,visit_schedule_name,schedule_name.', max_length=500, null=True),
+            model_name="historicalcannedviews",
+            name="reverse_url_args",
+            field=models.CharField(
+                help_text="column names separated by comma. For example, subject_identifier,visit_code,visit_code_sequence,visit_schedule_name,schedule_name.",
+                max_length=500,
+                null=True,
+            ),
         ),
         migrations.AddField(
-            model_name='historicalcannedviews',
-            name='reverse_url_name',
-            field=models.CharField(help_text='a valid url name as a `key` for the `value` stored in the `url_names` dictionary. For example, `subject_dashboard_url`.', max_length=50, null=True),
+            model_name="historicalcannedviews",
+            name="reverse_url_name",
+            field=models.CharField(
+                help_text="a valid url name as a `key` for the `value` stored in the `url_names` dictionary. For example, `subject_dashboard_url`.",
+                max_length=50,
+                null=True,
+            ),
         ),
         migrations.AlterField(
-            model_name='cannedviews',
-            name='description',
-            field=models.TextField(blank=True, help_text='Appears in the report header. A clear descrtiption of the report and its intended use.', null=True),
+            model_name="cannedviews",
+            name="description",
+            field=models.TextField(
+                blank=True,
+                help_text="Appears in the report header. A clear descrtiption of the report and its intended use.",
+                null=True,
+            ),
         ),
         migrations.AlterField(
-            model_name='cannedviews',
-            name='display_name',
+            model_name="cannedviews",
+            name="display_name",
             field=models.CharField(blank=True, max_length=50),
         ),
         migrations.AlterField(
-            model_name='cannedviews',
-            name='filter_by_current_site',
-            field=models.CharField(choices=[('Yes', 'Yes'), ('No', 'No')], default='No', help_text='If yes, the column `site_id` is expected', max_length=10),
-        ),
-        migrations.AlterField(
-            model_name='cannedviews',
-            name='instructions',
-            field=models.TextField(blank=True, help_text='Appears in the report header. Instructions for the user of the report', null=True),
+            model_name="cannedviews",
+            name="filter_by_current_site",
+            field=models.CharField(
+                choices=[("Yes", "Yes"), ("No", "No")],
+                default="No",
+                help_text="If yes, the column `site_id` is expected",
+                max_length=10,
+            ),
+        ),
+        migrations.AlterField(
+            model_name="cannedviews",
+            name="instructions",
+            field=models.TextField(
+                blank=True,
+                help_text="Appears in the report header. Instructions for the user of the report",
+                null=True,
+            ),
+        ),
+        migrations.AlterField(
+            model_name="cannedviews",
+            name="name",
+            field=models.CharField(
+                max_length=30,
+                validators=[django.core.validators.RegexValidator(regex="^([a-z0-9_])+$")],
+            ),
+        ),
+        migrations.AlterField(
+            model_name="historicalcannedviews",
+            name="description",
+            field=models.TextField(
+                blank=True,
+                help_text="Appears in the report header. A clear descrtiption of the report and its intended use.",
+                null=True,
+            ),
         ),
         migrations.AlterField(
-            model_name='cannedviews',
-            name='name',
-            field=models.CharField(max_length=30, validators=[django.core.validators.RegexValidator(regex='^([a-z0-9_])+$')]),
-        ),
-        migrations.AlterField(
-            model_name='historicalcannedviews',
-            name='description',
-            field=models.TextField(blank=True, help_text='Appears in the report header. A clear descrtiption of the report and its intended use.', null=True),
-        ),
-        migrations.AlterField(
-            model_name='historicalcannedviews',
-            name='display_name',
+            model_name="historicalcannedviews",
+            name="display_name",
             field=models.CharField(blank=True, max_length=50),
         ),
         migrations.AlterField(
-            model_name='historicalcannedviews',
-            name='filter_by_current_site',
-            field=models.CharField(choices=[('Yes', 'Yes'), ('No', 'No')], default='No', help_text='If yes, the column `site_id` is expected', max_length=10),
-        ),
-        migrations.AlterField(
-            model_name='historicalcannedviews',
-            name='instructions',
-            field=models.TextField(blank=True, help_text='Appears in the report header. Instructions for the user of the report', null=True),
-        ),
-        migrations.AlterField(
-            model_name='historicalcannedviews',
-            name='name',
-            field=models.CharField(max_length=30, validators=[django.core.validators.RegexValidator(regex='^([a-z0-9_])+$')]),
+            model_name="historicalcannedviews",
+            name="filter_by_current_site",
+            field=models.CharField(
+                choices=[("Yes", "Yes"), ("No", "No")],
+                default="No",
+                help_text="If yes, the column `site_id` is expected",
+                max_length=10,
+            ),
+        ),
+        migrations.AlterField(
+            model_name="historicalcannedviews",
+            name="instructions",
+            field=models.TextField(
+                blank=True,
+                help_text="Appears in the report header. Instructions for the user of the report",
+                null=True,
+            ),
+        ),
+        migrations.AlterField(
+            model_name="historicalcannedviews",
+            name="name",
+            field=models.CharField(
+                max_length=30,
+                validators=[django.core.validators.RegexValidator(regex="^([a-z0-9_])+$")],
+            ),
         ),
     ]
```

### Comparing `canned-views-0.1.7/canned_views/migrations/0009_auto_20220704_1841.py` & `canned-views-0.1.8/canned_views/migrations/0009_auto_20220704_1841.py`

 * *Files identical despite different names*

### Comparing `canned-views-0.1.7/canned_views/models.py` & `canned-views-0.1.8/canned_views/models.py`

 * *Files identical despite different names*

### Comparing `canned-views-0.1.7/canned_views/templates/canned_views/base.html` & `canned-views-0.1.8/canned_views/templates/canned_views/base.html`

 * *Files identical despite different names*

### Comparing `canned-views-0.1.7/canned_views/templates/canned_views/base_dj3.html` & `canned-views-0.1.8/canned_views/templates/canned_views/base_dj3.html`

 * *Files identical despite different names*

### Comparing `canned-views-0.1.7/canned_views/templates/canned_views/canned_view.html` & `canned-views-0.1.8/canned_views/templates/canned_views/canned_view.html`

 * *Files identical despite different names*

### Comparing `canned-views-0.1.7/canned_views/templates/canned_views/home.html` & `canned-views-0.1.8/canned_views/templates/canned_views/home.html`

 * *Files identical despite different names*

### Comparing `canned-views-0.1.7/canned_views/templatetags/canned_extras.py` & `canned-views-0.1.8/canned_views/templatetags/canned_extras.py`

 * *Files identical despite different names*

### Comparing `canned-views-0.1.7/canned_views/utils.py` & `canned-views-0.1.8/canned_views/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import re
 from typing import Any, List, Optional
 
 import sqlvalidator
 from django import forms
 from django.conf import settings
 from django.db import OperationalError, connection, models
 
@@ -70,54 +71,60 @@
             raise DynamicModelError("Invalid report name")
         if sql_view_name != sql_view_name.replace(" ", "").lower().strip(BAD_CHARS):
             raise DynamicModelError("Invalid sql_view_name")
         if not sql_view_name.startswith(get_sql_view_name_prefix()):
             raise DynamicModelError(
                 f"Invalid sql_view_name. Must start with `{get_sql_view_name_prefix()}`"
             )
-        self.sql_view_name = sql_view_name
+        if not re.match(r"^([a-z_])+$", sql_view_name):
+            raise DynamicModelError("Invalid sql view name")
+        self.sql_view_name: str = sql_view_name
         self.read_from_cursor()
         model_name = f"TemporaryView{name.replace('_', '').lower().title()}"
         # create class
         self.model_cls = type(model_name, (models.Model,), self.model_attrs)
         # unregister from all_models
         try:
             del self.model_cls._meta.apps.all_models[settings.APP_NAME][  # noqa
                 model_name.lower()
             ]
         except KeyError:
             pass
 
-    def get_sql(self, cols: Optional[str] = None):
-        cols = cols.replace(" ", "").split(",") if cols else []
+    def get_sql(self, cols: str = None):
+        cols = cols.replace(" ", "")
+        if not re.match(r"^([a-z,])+$", cols):
+            raise DynamicModelError("Invalid columns string.")
+        cols = cols.split(",") if cols else []
         for col in cols:
             if col not in self.sql_select_columns:
                 raise DynamicModelError(f"Invalid column specified. Got `{col}`.")
         sql_select_columns = cols or self.sql_select_columns
-        # if self.reverse_url == YES:
-        #     args = tuple() if self.reverse_url_args is None else
-        #     url_name = url_names.get(self.reverse_url_name)
-        #     sql_select_columns.append(f"'{url_name}' as url")
-        # if "subject_identifier" in sql_select_columns and "url" not in sql_select_columns:
-        #     url_name = url_names.get("subject_dashboard_url")
-        #     sql_select_columns.append(f"'{url_name}' as url")
         if "id" not in sql_select_columns:
-            sql = f"select {','.join(sql_select_columns)}, 0 AS id from {self.sql_view_name}"
+            sql = "select {','.join(sql_select_columns)}, 0 AS id from {self.sql_view_name}"
         else:
-            sql = f"select {','.join(sql_select_columns)} from {self.sql_view_name}"
+            sql = (
+                f"select {','.join(sql_select_columns)} "  # nosec B608
+                f"from {self.sql_view_name}"
+            )
         return sql
 
     def read_from_cursor(self):
         """Determine server type and update select command and column names."""
         with connection.cursor() as cursor:
             try:
                 cursor.execute(f"describe {self.sql_view_name}")
             except OperationalError:
-                cursor.execute(f"select * from pragma_table_info('{self.sql_view_name}')")
-                self.sql_describe = f"select * from pragma_table_info('{self.sql_view_name}')"
+                cursor.execute(
+                    "select * from pragma_table_info('%(sql_view_name)s')",  # nosec B608
+                    params=dict(sql_view_name=self.sql_view_name),
+                )
+                self.sql_describe = (
+                    f"select * from pragma_table_info('{self.sql_view_name}')"  # nosec B608
+                )
                 self.dialect = Dialects.get("sqlite")
             else:
                 self.sql_describe = f"describe {self.sql_view_name}"
                 self.dialect = Dialects.get("mysql")
             self.columns = [col[0] for col in cursor.description]
 
     @property
```

### Comparing `canned-views-0.1.7/canned_views/views/basic_view.py` & `canned-views-0.1.8/canned_views/views/basic_view.py`

 * *Files identical despite different names*

### Comparing `canned-views-0.1.7/canned_views/views/home_view.py` & `canned-views-0.1.8/canned_views/views/home_view.py`

 * *Files identical despite different names*

### Comparing `canned-views-0.1.7/canned_views.egg-info/PKG-INFO` & `canned-views-0.1.8/canned_views.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: canned-views
-Version: 0.1.7
+Version: 0.1.8
 Summary: SQL views presented as simple Django ListView reports
 Home-page: https://github.com/erikvw/canned-views
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django sql view ListView,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.1
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Requires-Python: >=3.9
+Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
 
 Canned Views
 ------------
```

### Comparing `canned-views-0.1.7/canned_views.egg-info/SOURCES.txt` & `canned-views-0.1.8/canned_views.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 .coveragerc
 .editorconfig
 .gitignore
+.pre-commit-config.yaml
+.yamllint
 AUTHORS
 CHANGES
 LICENSE
 MANIFEST.in
 README.rst
 VERSION
 codecov.yml
 pyproject.toml
 setup.cfg
+.github/workflows/build.yml
 canned_views/__init__.py
 canned_views/admin.py
 canned_views/admin_site.py
 canned_views/apps.py
 canned_views/auth_objects.py
 canned_views/auths.py
 canned_views/constants.py
@@ -32,14 +35,16 @@
 canned_views/migrations/0003_remove_cannedviews_columns_and_more.py
 canned_views/migrations/0004_auto_20220617_2306.py
 canned_views/migrations/0005_auto_20220617_2344.py
 canned_views/migrations/0006_cannedviews_filter_by_current_site_and_more.py
 canned_views/migrations/0007_cannedviews_linked_column_name_and_more.py
 canned_views/migrations/0008_rename_cannedviews_cannedview_and_more.py
 canned_views/migrations/0009_auto_20220704_1841.py
+canned_views/migrations/0010_alter_cannedview_managers.py
+canned_views/migrations/0011_alter_cannedview_options.py
 canned_views/migrations/__init__.py
 canned_views/templates/canned_views/base.html
 canned_views/templates/canned_views/base_dj3.html
 canned_views/templates/canned_views/button.html
 canned_views/templates/canned_views/canned_view.html
 canned_views/templates/canned_views/home.html
 canned_views/templatetags/__init__.py
```

### Comparing `canned-views-0.1.7/canned_views_app/manage.py` & `canned-views-0.1.8/canned_views_app/manage.py`

 * *Files identical despite different names*

### Comparing `canned-views-0.1.7/canned_views_app/settings.py` & `canned-views-0.1.8/canned_views_app/settings.py`

 * *Files 14% similar despite different names*

```diff
@@ -33,18 +33,16 @@
 SITE_ID = 1
 EDC_NAVBAR_DEFAULT = "canned_views_app"
 EDC_PROTOCOL_PROJECT_NAME = "Reports"
 PROJECT_NAME = "Reports"
 # Quick-start development settings - unsuitable for production
 # See https://docs.djangoproject.com/en/4.0/howto/deployment/checklist/
 
-# SECURITY WARNING: keep the secret key used in production secret!
-SECRET_KEY = "django-insecure-68zb@3bs^yev0--y_254d=@6&0cme3o7(9+6%#ga00)0(6)0x%"
+SECRET_KEY = "django-insecure-68zb@3bs^yev0--y_254d=@6&0cme3o7(9+6%#ga00)0(6)0x%"  # nosec B105
 
-# SECURITY WARNING: don't run with debug turned on in production!
 DEBUG = True
 
 ALLOWED_HOSTS = []
 
 
 # Application definition
 
@@ -103,42 +101,19 @@
         },
     },
 ]
 
 WSGI_APPLICATION = "canned_views_app.wsgi.application"
 
 
-# Database
-# https://docs.djangoproject.com/en/4.0/ref/settings/#databases
-
-# DATABASES = {
-#     "default": {
-#         "ENGINE": "django.db.backends.sqlite3",
-#         "NAME": BASE_DIR / "db.sqlite3",
-#     }
-# }
-
 DATABASES = {"default": env.db()}
+
 # be secure and clear DATABASE_URL since it is no longer needed.
 DATABASE_URL = None
 
-# DATABASES = {
-#     "default": {
-#         "ENGINE": "django.db.backends.mysql",
-#         "NAME": "canned_views",
-#         "USER": "",
-#         "PASSWORD": "",
-#         "HOST": "localhost",
-#         "PORT": "",
-#     }
-# }
-
-# Password validation
-# https://docs.djangoproject.com/en/4.0/ref/settings/#auth-password-validators
-
 AUTH_PASSWORD_VALIDATORS = [
     {
         "NAME": "django.contrib.auth.password_validation.UserAttributeSimilarityValidator",
     },
     {
         "NAME": "django.contrib.auth.password_validation.MinimumLengthValidator",
     },
```

### Comparing `canned-views-0.1.7/canned_views_app/templates/canned_views_app/home.html` & `canned-views-0.1.8/canned_views_app/templates/canned_views_app/home.html`

 * *Files identical despite different names*

### Comparing `canned-views-0.1.7/canned_views_app/urls.py` & `canned-views-0.1.8/canned_views_app/urls.py`

 * *Files identical despite different names*

### Comparing `canned-views-0.1.7/pyproject.toml` & `canned-views-0.1.8/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -28,39 +28,43 @@
 skip_covered = true
 omit = ["requirements.txt"]
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 envlist =
-    py{39}-dj{32,dev},
+    py{311}-dj{41,42,dev},
     lint
+
 isolated_build = true
 
 [gh-actions]
 python =
-    3.9: py39, lint
+    3.11: py311, lint
 
 [gh-actions:env]
 DJANGO =
-    3.2: dj32, lint
+    4.1: dj41
+    4.2: dj42
     dev: djdev
 
 [testenv]
 deps =
     -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/tox.txt
     -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/test_utils.txt
     -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/edc.txt
     -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/third_party_dev.txt
-    dj32: Django>=3.2,<3.3
+    dj41: Django>=4.1,<4.2
+    dj42: Django>=4.2,<5.0
     djdev: https://github.com/django/django/tarball/main
 
 commands =
     pip install -U pip
     pip --version
+    pip freeze
     coverage run -a runtests.py
     coverage report
 
 [testenv:lint]
 deps = -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/lint.txt
 commands =
     isort --profile=black --check --diff .
```

### Comparing `canned-views-0.1.7/setup.cfg` & `canned-views-0.1.8/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -8,24 +8,23 @@
 description = SQL views presented as simple Django ListView reports
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 keywords = django sql view ListView, clinicedc, clinical trials
 classifiers = 
 	Environment :: Web Environment
 	Framework :: Django
-	Framework :: Django :: 3.2
+	Framework :: Django :: 4.1
 	Intended Audience :: Developers
 	Intended Audience :: Science/Research
 	Operating System :: OS Independent
-	Programming Language :: Python :: 3.8
-	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.11
 	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 
 [options]
-python_requires = >=3.9
+python_requires = >=3.11
 zip_safe = False
 include_package_data = True
 packages = find:
 install_requires = 
 	sqlvalidator
 
 [options.packages.find]
@@ -36,14 +35,14 @@
 	bin*
 	canned_views.tests*
 
 [flake8]
 ignore = E226,W503,E203
 max-line-length = 95
 max-complexity = 10
-exclude = */migrations,.tox,.git,__pycache__,build,dist,.eggs
+exclude = */migrations/*,.tox,.git,__pycache__,build,dist,.eggs
 per-file-ignores = __init__.py: F401
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

