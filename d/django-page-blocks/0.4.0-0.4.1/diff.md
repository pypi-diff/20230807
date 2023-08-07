# Comparing `tmp/django-page-blocks-0.4.0.tar.gz` & `tmp/django-page-blocks-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-page-blocks-0.4.0.tar", last modified: Sun May 21 15:17:59 2023, max compression
+gzip compressed data, was "django-page-blocks-0.4.1.tar", last modified: Mon Aug  7 19:10:56 2023, max compression
```

## Comparing `django-page-blocks-0.4.0.tar` & `django-page-blocks-0.4.1.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-05-21 15:17:59.185837 django-page-blocks-0.4.0/
--rw-rw-r--   0 mark      (1000) mark      (1000)     1101 2021-11-10 18:41:53.000000 django-page-blocks-0.4.0/LICENSE
--rw-rw-r--   0 mark      (1000) mark      (1000)      215 2021-11-10 18:53:22.000000 django-page-blocks-0.4.0/MANIFEST.in
--rw-rw-r--   0 mark      (1000) mark      (1000)     6035 2023-05-21 15:17:59.185837 django-page-blocks-0.4.0/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)     5013 2023-05-21 15:17:06.000000 django-page-blocks-0.4.0/README.md
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-05-21 15:17:59.105835 django-page-blocks-0.4.0/django_page_blocks.egg-info/
--rw-rw-r--   0 mark      (1000) mark      (1000)     6035 2023-05-21 15:17:59.000000 django-page-blocks-0.4.0/django_page_blocks.egg-info/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)     2240 2023-05-21 15:17:59.000000 django-page-blocks-0.4.0/django_page_blocks.egg-info/SOURCES.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        1 2023-05-21 15:17:59.000000 django-page-blocks-0.4.0/django_page_blocks.egg-info/dependency_links.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       11 2023-05-21 15:17:59.000000 django-page-blocks-0.4.0/django_page_blocks.egg-info/top_level.txt
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-05-21 15:17:59.109835 django-page-blocks-0.4.0/pageblocks/
--rw-rw-r--   0 mark      (1000) mark      (1000)      146 2022-05-12 17:17:14.000000 django-page-blocks-0.4.0/pageblocks/__init__.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      394 2023-05-20 14:55:38.000000 django-page-blocks-0.4.0/pageblocks/admin.py
--rw-rw-r--   0 mark      (1000) mark      (1000)    13250 2023-05-20 18:20:00.000000 django-page-blocks-0.4.0/pageblocks/blocks.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     3648 2023-05-20 18:20:00.000000 django-page-blocks-0.4.0/pageblocks/forms.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-05-21 15:17:59.109835 django-page-blocks-0.4.0/pageblocks/migrations/
--rw-r--r--   0 mark      (1000) mark      (1000)     1217 2021-10-12 16:50:46.000000 django-page-blocks-0.4.0/pageblocks/migrations/0001_initial.py
--rw-r--r--   0 mark      (1000) mark      (1000)      483 2021-10-12 16:54:28.000000 django-page-blocks-0.4.0/pageblocks/migrations/0002_auto_20211012_1854.py
--rw-r--r--   0 mark      (1000) mark      (1000)      653 2021-11-07 17:04:20.000000 django-page-blocks-0.4.0/pageblocks/migrations/0003_auto_20211107_1804.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      546 2022-05-12 17:17:14.000000 django-page-blocks-0.4.0/pageblocks/migrations/0004_image.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      487 2023-05-20 18:20:00.000000 django-page-blocks-0.4.0/pageblocks/migrations/0005_remove_pageblock_language_pageblock_i18n_data.py
--rw-r--r--   0 mark      (1000) mark      (1000)        0 2021-10-12 16:50:46.000000 django-page-blocks-0.4.0/pageblocks/migrations/__init__.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-05-21 15:17:59.161837 django-page-blocks-0.4.0/pageblocks/migrations/__pycache__/
--rw-r--r--   0 mark      (1000) mark      (1000)     1125 2023-01-23 12:01:11.000000 django-page-blocks-0.4.0/pageblocks/migrations/__pycache__/0001_initial.cpython-310.pyc
--rw-r--r--   0 mark      (1000) mark      (1000)     1122 2021-10-12 16:50:47.000000 django-page-blocks-0.4.0/pageblocks/migrations/__pycache__/0001_initial.cpython-39.pyc
--rw-r--r--   0 mark      (1000) mark      (1000)      615 2023-01-23 12:01:11.000000 django-page-blocks-0.4.0/pageblocks/migrations/__pycache__/0002_auto_20211012_1854.cpython-310.pyc
--rw-r--r--   0 mark      (1000) mark      (1000)      612 2021-10-12 16:54:30.000000 django-page-blocks-0.4.0/pageblocks/migrations/__pycache__/0002_auto_20211012_1854.cpython-39.pyc
--rw-r--r--   0 mark      (1000) mark      (1000)      773 2021-11-07 16:51:24.000000 django-page-blocks-0.4.0/pageblocks/migrations/__pycache__/0003_auto_20211107_1751.cpython-39.pyc
--rw-r--r--   0 mark      (1000) mark      (1000)      802 2023-01-23 12:01:11.000000 django-page-blocks-0.4.0/pageblocks/migrations/__pycache__/0003_auto_20211107_1804.cpython-310.pyc
--rw-r--r--   0 mark      (1000) mark      (1000)      799 2021-11-07 17:04:22.000000 django-page-blocks-0.4.0/pageblocks/migrations/__pycache__/0003_auto_20211107_1804.cpython-39.pyc
--rw-r--r--   0 mark      (1000) mark      (1000)      685 2023-01-23 12:01:11.000000 django-page-blocks-0.4.0/pageblocks/migrations/__pycache__/0004_image.cpython-310.pyc
--rw-r--r--   0 mark      (1000) mark      (1000)      682 2022-03-16 11:50:13.000000 django-page-blocks-0.4.0/pageblocks/migrations/__pycache__/0004_image.cpython-39.pyc
--rw-r--r--   0 mark      (1000) mark      (1000)      647 2023-05-20 15:08:04.000000 django-page-blocks-0.4.0/pageblocks/migrations/__pycache__/0005_remove_pageblock_language_pageblock_i18n_data.cpython-310.pyc
--rw-r--r--   0 mark      (1000) mark      (1000)      131 2023-01-23 12:01:11.000000 django-page-blocks-0.4.0/pageblocks/migrations/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 mark      (1000) mark      (1000)      130 2021-10-12 16:50:46.000000 django-page-blocks-0.4.0/pageblocks/migrations/__pycache__/__init__.cpython-39.pyc
--rw-rw-r--   0 mark      (1000) mark      (1000)     2449 2023-05-20 18:20:00.000000 django-page-blocks-0.4.0/pageblocks/models.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-05-21 15:17:59.101835 django-page-blocks-0.4.0/pageblocks/static/
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-05-21 15:17:59.101835 django-page-blocks-0.4.0/pageblocks/static/admin/
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-05-21 15:17:59.101835 django-page-blocks-0.4.0/pageblocks/static/admin/pageblocks/
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-05-21 15:17:59.161837 django-page-blocks-0.4.0/pageblocks/static/admin/pageblocks/css/
--rw-rw-r--   0 mark      (1000) mark      (1000)     2320 2023-05-20 18:20:00.000000 django-page-blocks-0.4.0/pageblocks/static/admin/pageblocks/css/change_form.css
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-05-21 15:17:59.165837 django-page-blocks-0.4.0/pageblocks/static/admin/pageblocks/js/
--rw-rw-r--   0 mark      (1000) mark      (1000)    15461 2023-05-20 18:20:00.000000 django-page-blocks-0.4.0/pageblocks/static/admin/pageblocks/js/change_form.js
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-05-21 15:17:59.101835 django-page-blocks-0.4.0/pageblocks/templates/
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-05-21 15:17:59.101835 django-page-blocks-0.4.0/pageblocks/templates/admin/
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-05-21 15:17:59.165837 django-page-blocks-0.4.0/pageblocks/templates/admin/pageblocks/
--rw-rw-r--   0 mark      (1000) mark      (1000)      382 2023-05-20 18:20:00.000000 django-page-blocks-0.4.0/pageblocks/templates/admin/pageblocks/block_editor.html
--rw-rw-r--   0 mark      (1000) mark      (1000)      983 2022-05-12 17:17:14.000000 django-page-blocks-0.4.0/pageblocks/templates/admin/pageblocks/change_form.html
--rw-rw-r--   0 mark      (1000) mark      (1000)      239 2021-08-18 19:18:02.000000 django-page-blocks-0.4.0/pageblocks/templates/admin/pageblocks/multi_language_input.html
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-05-21 15:17:59.101835 django-page-blocks-0.4.0/pageblocks/templates/pageblocks/
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-05-21 15:17:59.165837 django-page-blocks-0.4.0/pageblocks/templates/pageblocks/blocks/
--rw-rw-r--   0 mark      (1000) mark      (1000)       77 2021-11-09 23:08:53.000000 django-page-blocks-0.4.0/pageblocks/templates/pageblocks/blocks/container.html
--rw-rw-r--   0 mark      (1000) mark      (1000)       21 2021-11-09 23:01:34.000000 django-page-blocks-0.4.0/pageblocks/templates/pageblocks/blocks/html.html
--rw-rw-r--   0 mark      (1000) mark      (1000)      139 2022-05-12 17:17:14.000000 django-page-blocks-0.4.0/pageblocks/templates/pageblocks/blocks/image.html
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-05-21 15:17:59.169837 django-page-blocks-0.4.0/pageblocks/templatetags/
--rw-rw-r--   0 mark      (1000) mark      (1000)        0 2021-11-09 22:25:12.000000 django-page-blocks-0.4.0/pageblocks/templatetags/__init__.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-05-21 15:17:59.185837 django-page-blocks-0.4.0/pageblocks/templatetags/__pycache__/
--rw-r--r--   0 mark      (1000) mark      (1000)      133 2023-01-23 12:01:11.000000 django-page-blocks-0.4.0/pageblocks/templatetags/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 mark      (1000) mark      (1000)      132 2021-11-09 22:26:41.000000 django-page-blocks-0.4.0/pageblocks/templatetags/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 mark      (1000) mark      (1000)     1527 2023-05-20 18:04:38.000000 django-page-blocks-0.4.0/pageblocks/templatetags/__pycache__/pageblocks.cpython-310.pyc
--rw-r--r--   0 mark      (1000) mark      (1000)     1671 2022-05-12 17:13:20.000000 django-page-blocks-0.4.0/pageblocks/templatetags/__pycache__/pageblocks.cpython-39.pyc
--rw-rw-r--   0 mark      (1000) mark      (1000)     1066 2023-05-20 18:20:00.000000 django-page-blocks-0.4.0/pageblocks/templatetags/pageblocks.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     7638 2023-05-20 18:20:00.000000 django-page-blocks-0.4.0/pageblocks/tests.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      163 2021-08-18 19:49:24.000000 django-page-blocks-0.4.0/pageblocks/utils.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     1002 2022-03-15 22:06:20.000000 django-page-blocks-0.4.0/pageblocks/views.py
--rw-rw-r--   0 mark      (1000) mark      (1000)       38 2023-05-21 15:17:59.185837 django-page-blocks-0.4.0/setup.cfg
--rw-rw-r--   0 mark      (1000) mark      (1000)     1357 2023-05-20 18:20:00.000000 django-page-blocks-0.4.0/setup.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-08-07 19:10:56.188969 django-page-blocks-0.4.1/
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1101 2021-11-10 18:41:53.000000 django-page-blocks-0.4.1/LICENSE
+-rw-rw-r--   0 mark      (1000) mark      (1000)      215 2021-11-10 18:53:22.000000 django-page-blocks-0.4.1/MANIFEST.in
+-rw-rw-r--   0 mark      (1000) mark      (1000)     6035 2023-08-07 19:10:56.188969 django-page-blocks-0.4.1/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)     5013 2023-05-21 15:17:06.000000 django-page-blocks-0.4.1/README.md
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-08-07 19:10:56.168968 django-page-blocks-0.4.1/django_page_blocks.egg-info/
+-rw-rw-r--   0 mark      (1000) mark      (1000)     6035 2023-08-07 19:10:56.000000 django-page-blocks-0.4.1/django_page_blocks.egg-info/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)     2240 2023-08-07 19:10:56.000000 django-page-blocks-0.4.1/django_page_blocks.egg-info/SOURCES.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        1 2023-08-07 19:10:56.000000 django-page-blocks-0.4.1/django_page_blocks.egg-info/dependency_links.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       11 2023-08-07 19:10:56.000000 django-page-blocks-0.4.1/django_page_blocks.egg-info/top_level.txt
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-08-07 19:10:56.172968 django-page-blocks-0.4.1/pageblocks/
+-rw-rw-r--   0 mark      (1000) mark      (1000)      146 2022-05-12 17:17:14.000000 django-page-blocks-0.4.1/pageblocks/__init__.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      394 2023-05-20 14:55:38.000000 django-page-blocks-0.4.1/pageblocks/admin.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)    13710 2023-08-07 19:05:36.000000 django-page-blocks-0.4.1/pageblocks/blocks.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     3648 2023-05-20 18:20:00.000000 django-page-blocks-0.4.1/pageblocks/forms.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-08-07 19:10:56.176969 django-page-blocks-0.4.1/pageblocks/migrations/
+-rw-r--r--   0 mark      (1000) mark      (1000)     1217 2021-10-12 16:50:46.000000 django-page-blocks-0.4.1/pageblocks/migrations/0001_initial.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      483 2021-10-12 16:54:28.000000 django-page-blocks-0.4.1/pageblocks/migrations/0002_auto_20211012_1854.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      653 2021-11-07 17:04:20.000000 django-page-blocks-0.4.1/pageblocks/migrations/0003_auto_20211107_1804.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      546 2022-05-12 17:17:14.000000 django-page-blocks-0.4.1/pageblocks/migrations/0004_image.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      487 2023-05-20 18:20:00.000000 django-page-blocks-0.4.1/pageblocks/migrations/0005_remove_pageblock_language_pageblock_i18n_data.py
+-rw-r--r--   0 mark      (1000) mark      (1000)        0 2021-10-12 16:50:46.000000 django-page-blocks-0.4.1/pageblocks/migrations/__init__.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-08-07 19:10:56.180969 django-page-blocks-0.4.1/pageblocks/migrations/__pycache__/
+-rw-r--r--   0 mark      (1000) mark      (1000)     1125 2023-01-23 12:01:11.000000 django-page-blocks-0.4.1/pageblocks/migrations/__pycache__/0001_initial.cpython-310.pyc
+-rw-r--r--   0 mark      (1000) mark      (1000)     1122 2021-10-12 16:50:47.000000 django-page-blocks-0.4.1/pageblocks/migrations/__pycache__/0001_initial.cpython-39.pyc
+-rw-r--r--   0 mark      (1000) mark      (1000)      615 2023-01-23 12:01:11.000000 django-page-blocks-0.4.1/pageblocks/migrations/__pycache__/0002_auto_20211012_1854.cpython-310.pyc
+-rw-r--r--   0 mark      (1000) mark      (1000)      612 2021-10-12 16:54:30.000000 django-page-blocks-0.4.1/pageblocks/migrations/__pycache__/0002_auto_20211012_1854.cpython-39.pyc
+-rw-r--r--   0 mark      (1000) mark      (1000)      773 2021-11-07 16:51:24.000000 django-page-blocks-0.4.1/pageblocks/migrations/__pycache__/0003_auto_20211107_1751.cpython-39.pyc
+-rw-r--r--   0 mark      (1000) mark      (1000)      802 2023-01-23 12:01:11.000000 django-page-blocks-0.4.1/pageblocks/migrations/__pycache__/0003_auto_20211107_1804.cpython-310.pyc
+-rw-r--r--   0 mark      (1000) mark      (1000)      799 2021-11-07 17:04:22.000000 django-page-blocks-0.4.1/pageblocks/migrations/__pycache__/0003_auto_20211107_1804.cpython-39.pyc
+-rw-r--r--   0 mark      (1000) mark      (1000)      685 2023-01-23 12:01:11.000000 django-page-blocks-0.4.1/pageblocks/migrations/__pycache__/0004_image.cpython-310.pyc
+-rw-r--r--   0 mark      (1000) mark      (1000)      682 2022-03-16 11:50:13.000000 django-page-blocks-0.4.1/pageblocks/migrations/__pycache__/0004_image.cpython-39.pyc
+-rw-r--r--   0 mark      (1000) mark      (1000)      647 2023-08-07 18:52:33.000000 django-page-blocks-0.4.1/pageblocks/migrations/__pycache__/0005_remove_pageblock_language_pageblock_i18n_data.cpython-310.pyc
+-rw-r--r--   0 mark      (1000) mark      (1000)      131 2023-01-23 12:01:11.000000 django-page-blocks-0.4.1/pageblocks/migrations/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 mark      (1000) mark      (1000)      130 2021-10-12 16:50:46.000000 django-page-blocks-0.4.1/pageblocks/migrations/__pycache__/__init__.cpython-39.pyc
+-rw-rw-r--   0 mark      (1000) mark      (1000)     2449 2023-05-20 18:20:00.000000 django-page-blocks-0.4.1/pageblocks/models.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-08-07 19:10:56.164968 django-page-blocks-0.4.1/pageblocks/static/
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-08-07 19:10:56.164968 django-page-blocks-0.4.1/pageblocks/static/admin/
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-08-07 19:10:56.164968 django-page-blocks-0.4.1/pageblocks/static/admin/pageblocks/
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-08-07 19:10:56.180969 django-page-blocks-0.4.1/pageblocks/static/admin/pageblocks/css/
+-rw-rw-r--   0 mark      (1000) mark      (1000)     2320 2023-05-20 18:20:00.000000 django-page-blocks-0.4.1/pageblocks/static/admin/pageblocks/css/change_form.css
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-08-07 19:10:56.180969 django-page-blocks-0.4.1/pageblocks/static/admin/pageblocks/js/
+-rw-rw-r--   0 mark      (1000) mark      (1000)    15924 2023-08-07 19:08:34.000000 django-page-blocks-0.4.1/pageblocks/static/admin/pageblocks/js/change_form.js
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-08-07 19:10:56.164968 django-page-blocks-0.4.1/pageblocks/templates/
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-08-07 19:10:56.164968 django-page-blocks-0.4.1/pageblocks/templates/admin/
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-08-07 19:10:56.184969 django-page-blocks-0.4.1/pageblocks/templates/admin/pageblocks/
+-rw-rw-r--   0 mark      (1000) mark      (1000)      382 2023-05-20 18:20:00.000000 django-page-blocks-0.4.1/pageblocks/templates/admin/pageblocks/block_editor.html
+-rw-rw-r--   0 mark      (1000) mark      (1000)      983 2022-05-12 17:17:14.000000 django-page-blocks-0.4.1/pageblocks/templates/admin/pageblocks/change_form.html
+-rw-rw-r--   0 mark      (1000) mark      (1000)      239 2021-08-18 19:18:02.000000 django-page-blocks-0.4.1/pageblocks/templates/admin/pageblocks/multi_language_input.html
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-08-07 19:10:56.164968 django-page-blocks-0.4.1/pageblocks/templates/pageblocks/
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-08-07 19:10:56.184969 django-page-blocks-0.4.1/pageblocks/templates/pageblocks/blocks/
+-rw-rw-r--   0 mark      (1000) mark      (1000)       77 2021-11-09 23:08:53.000000 django-page-blocks-0.4.1/pageblocks/templates/pageblocks/blocks/container.html
+-rw-rw-r--   0 mark      (1000) mark      (1000)       21 2021-11-09 23:01:34.000000 django-page-blocks-0.4.1/pageblocks/templates/pageblocks/blocks/html.html
+-rw-rw-r--   0 mark      (1000) mark      (1000)      139 2022-05-12 17:17:14.000000 django-page-blocks-0.4.1/pageblocks/templates/pageblocks/blocks/image.html
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-08-07 19:10:56.184969 django-page-blocks-0.4.1/pageblocks/templatetags/
+-rw-rw-r--   0 mark      (1000) mark      (1000)        0 2021-11-09 22:25:12.000000 django-page-blocks-0.4.1/pageblocks/templatetags/__init__.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-08-07 19:10:56.188969 django-page-blocks-0.4.1/pageblocks/templatetags/__pycache__/
+-rw-r--r--   0 mark      (1000) mark      (1000)      133 2023-01-23 12:01:11.000000 django-page-blocks-0.4.1/pageblocks/templatetags/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 mark      (1000) mark      (1000)      132 2021-11-09 22:26:41.000000 django-page-blocks-0.4.1/pageblocks/templatetags/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 mark      (1000) mark      (1000)     1527 2023-08-07 18:52:32.000000 django-page-blocks-0.4.1/pageblocks/templatetags/__pycache__/pageblocks.cpython-310.pyc
+-rw-r--r--   0 mark      (1000) mark      (1000)     1671 2022-05-12 17:13:20.000000 django-page-blocks-0.4.1/pageblocks/templatetags/__pycache__/pageblocks.cpython-39.pyc
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1066 2023-05-20 18:20:00.000000 django-page-blocks-0.4.1/pageblocks/templatetags/pageblocks.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     7638 2023-05-20 18:20:00.000000 django-page-blocks-0.4.1/pageblocks/tests.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      163 2021-08-18 19:49:24.000000 django-page-blocks-0.4.1/pageblocks/utils.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1002 2022-03-15 22:06:20.000000 django-page-blocks-0.4.1/pageblocks/views.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)       38 2023-08-07 19:10:56.188969 django-page-blocks-0.4.1/setup.cfg
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1357 2023-08-07 19:10:14.000000 django-page-blocks-0.4.1/setup.py
```

### Comparing `django-page-blocks-0.4.0/LICENSE` & `django-page-blocks-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-page-blocks-0.4.0/PKG-INFO` & `django-page-blocks-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-page-blocks
-Version: 0.4.0
+Version: 0.4.1
 Summary: A simple, Wagtail CMS inspired multi language content block engine for Django.  Intended to give slightly more control than regular flatpages.
 Home-page: https://github.com/bravasoftware/django-page-blocks
 Author: Mark Skelton
 Author-email: studio@bravasoftware.com
 License: MIT License
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `django-page-blocks-0.4.0/README.md` & `django-page-blocks-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `django-page-blocks-0.4.0/django_page_blocks.egg-info/PKG-INFO` & `django-page-blocks-0.4.1/django_page_blocks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-page-blocks
-Version: 0.4.0
+Version: 0.4.1
 Summary: A simple, Wagtail CMS inspired multi language content block engine for Django.  Intended to give slightly more control than regular flatpages.
 Home-page: https://github.com/bravasoftware/django-page-blocks
 Author: Mark Skelton
 Author-email: studio@bravasoftware.com
 License: MIT License
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `django-page-blocks-0.4.0/django_page_blocks.egg-info/SOURCES.txt` & `django-page-blocks-0.4.1/django_page_blocks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-page-blocks-0.4.0/pageblocks/blocks.py` & `django-page-blocks-0.4.1/pageblocks/blocks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import logging
 import base64
 import copy
 import imghdr
 import re
 import uuid
 
 from django.conf import settings
@@ -51,18 +52,30 @@
 
 class ImageField(BaseField):
     input_type = 'image'
     multi_lingual = False
 
 class BlockStreamField(BaseField):
     input_type = 'blockstream'
+    block_types = None
+
+    def __init__(self, block_types=None, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        if block_types:
+            self.block_types = block_types
 
     def serialize_field_definition(self, id):
         fd = super().serialize_field_definition(id)
         fd['initial'] = []
+        fd['block_types'] = []
+        for t in self.block_types if self.block_types else []:
+            try:
+                fd['block_types'].append(t.__module__ + '.' + t.__name__)
+            except Exception as e:
+                logging.error(e)
         return fd
 
 
 class BlockValidationError(Exception):
     def __init__(self, msg, field_id):
         super().__init__(msg)
         self.field_id = field_id
```

### Comparing `django-page-blocks-0.4.0/pageblocks/forms.py` & `django-page-blocks-0.4.1/pageblocks/forms.py`

 * *Files identical despite different names*

### Comparing `django-page-blocks-0.4.0/pageblocks/migrations/0001_initial.py` & `django-page-blocks-0.4.1/pageblocks/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-page-blocks-0.4.0/pageblocks/migrations/0003_auto_20211107_1804.py` & `django-page-blocks-0.4.1/pageblocks/migrations/0003_auto_20211107_1804.py`

 * *Files identical despite different names*

### Comparing `django-page-blocks-0.4.0/pageblocks/migrations/0004_image.py` & `django-page-blocks-0.4.1/pageblocks/migrations/0004_image.py`

 * *Files identical despite different names*

### Comparing `django-page-blocks-0.4.0/pageblocks/migrations/__pycache__/0001_initial.cpython-310.pyc` & `django-page-blocks-0.4.1/pageblocks/migrations/__pycache__/0001_initial.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-page-blocks-0.4.0/pageblocks/migrations/__pycache__/0001_initial.cpython-39.pyc` & `django-page-blocks-0.4.1/pageblocks/migrations/__pycache__/0001_initial.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-page-blocks-0.4.0/pageblocks/migrations/__pycache__/0002_auto_20211012_1854.cpython-310.pyc` & `django-page-blocks-0.4.1/pageblocks/migrations/__pycache__/0002_auto_20211012_1854.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-page-blocks-0.4.0/pageblocks/migrations/__pycache__/0002_auto_20211012_1854.cpython-39.pyc` & `django-page-blocks-0.4.1/pageblocks/migrations/__pycache__/0002_auto_20211012_1854.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-page-blocks-0.4.0/pageblocks/migrations/__pycache__/0003_auto_20211107_1751.cpython-39.pyc` & `django-page-blocks-0.4.1/pageblocks/migrations/__pycache__/0003_auto_20211107_1751.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-page-blocks-0.4.0/pageblocks/migrations/__pycache__/0003_auto_20211107_1804.cpython-310.pyc` & `django-page-blocks-0.4.1/pageblocks/migrations/__pycache__/0003_auto_20211107_1804.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-page-blocks-0.4.0/pageblocks/migrations/__pycache__/0003_auto_20211107_1804.cpython-39.pyc` & `django-page-blocks-0.4.1/pageblocks/migrations/__pycache__/0003_auto_20211107_1804.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-page-blocks-0.4.0/pageblocks/migrations/__pycache__/0004_image.cpython-310.pyc` & `django-page-blocks-0.4.1/pageblocks/migrations/__pycache__/0004_image.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-page-blocks-0.4.0/pageblocks/migrations/__pycache__/0004_image.cpython-39.pyc` & `django-page-blocks-0.4.1/pageblocks/migrations/__pycache__/0004_image.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-page-blocks-0.4.0/pageblocks/migrations/__pycache__/0005_remove_pageblock_language_pageblock_i18n_data.cpython-310.pyc` & `django-page-blocks-0.4.1/pageblocks/migrations/__pycache__/0005_remove_pageblock_language_pageblock_i18n_data.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat May 20 15:08:01 2023 UTC, .py size: 487 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-00000000: 6f0d 0d0a 0000 0000 51e2 6864 e701 0000  o.......Q.hd....
+00000000: 6f0d 0d0a 0000 0000 500f 6964 e701 0000  o.......P.id....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2600 0000 6400  .....@...s&...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 4700  d.l.m.Z.m.Z...G.
 00000040: 6402 6403 8400 6403 6501 6a03 8303 5a03  d.d...d.e.j...Z.
 00000050: 6404 5300 2905 e900 0000 0029 02da 0a6d  d.S.)......)...m
 00000060: 6967 7261 7469 6f6e 73da 066d 6f64 656c  igrations..model
 00000070: 7363 0000 0000 0000 0000 0000 0000 0000  sc..............
 00000080: 0000 0700 0000 4000 0000 7338 0000 0065  ......@...s8...e
 00000090: 005a 0164 005a 0264 0167 015a 0365 046a  .Z.d.Z.d.g.Z.e.j
 000000a0: 0564 0264 0364 048d 0265 046a 0664 0264  .d.d.d...e.j.d.d
 000000b0: 0565 076a 0865 0964 068d 0164 078d 0367  .e.j.e.d...d...g
 000000c0: 025a 0a64 0853 0029 09da 094d 6967 7261  .Z.d.S.)...Migra
 000000d0: 7469 6f6e 2902 da0a 7061 6765 626c 6f63  tion)...pagebloc
-000000e0: 6b73 5a0a 3030 3034 5f69 6d61 6765 da09  ksZ.0004_image..
+000000e0: 6b73 da0a 3030 3034 5f69 6d61 6765 5a09  ks..0004_imageZ.
 000000f0: 7061 6765 626c 6f63 6bda 086c 616e 6775  pageblock..langu
 00000100: 6167 6529 02da 0a6d 6f64 656c 5f6e 616d  age)...model_nam
 00000110: 65da 046e 616d 65da 0969 3138 6e5f 6461  e..name..i18n_da
 00000120: 7461 2901 da07 6465 6661 756c 7429 0372  ta)...default).r
 00000130: 0800 0000 7209 0000 00da 0566 6965 6c64  ....r......field
 00000140: 4e29 0bda 085f 5f6e 616d 655f 5fda 0a5f  N)...__name__.._
 00000150: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
```

### Comparing `django-page-blocks-0.4.0/pageblocks/models.py` & `django-page-blocks-0.4.1/pageblocks/models.py`

 * *Files identical despite different names*

### Comparing `django-page-blocks-0.4.0/pageblocks/static/admin/pageblocks/css/change_form.css` & `django-page-blocks-0.4.1/pageblocks/static/admin/pageblocks/css/change_form.css`

 * *Files identical despite different names*

### Comparing `django-page-blocks-0.4.0/pageblocks/static/admin/pageblocks/js/change_form.js` & `django-page-blocks-0.4.1/pageblocks/static/admin/pageblocks/js/change_form.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -116,15 +116,15 @@
         {{ field.label }}<span class="small" v-if="field.required">*</span>
       </label>
       <textarea v-if="field.input_type === 'textarea'" :required="field.required" :class="field.class" v-model="value" v-on:change="onValueChanged()"></textarea>
       <input v-if="field.input_type === 'text'" :type='field.input_type' :required="field.required" :class="field.class" v-model="value" v-on:change="onValueChanged()" />
       <block-editor
         v-if="field.input_type === 'blockstream'"
         v-model="value"
-        :available-blocks="availableBlocks"
+        :available-blocks="filterAvailableBlocks(field)"
         v-on:change="onValueChanged()"
         :block-index="blockIndex"
         :input-name="inputName"
         :languages="languages"
         :default-language="defaultLanguage"></block-editor>
       <image-uploader
         v-if="field.input_type === 'image'"
@@ -152,14 +152,26 @@
                     for (const err of this.$root.blockEditorErrors[this.inputName]) {
                         if (err[1] === this.blockIndex.join(',') && err[2] == this.fieldId) {
                             return err[err.length - 1];
                         }
                     }
                 }
                 return null;
+            },
+            filterAvailableBlocks: function(field) {
+                if (!field.block_types || field.block_types.length === 0) {
+                    return this.availableBlocks;
+                }
+                const filteredBlocks = {};
+                for (const blockType of field.block_types) {
+                    if (this.availableBlocks[blockType] !== undefined) {
+                        filteredBlocks[blockType] = this.availableBlocks[blockType];
+                    }
+                }
+                return filteredBlocks;
             }
         },
     });
 
     Vue.component('block-editor', {
         template: `
     <div class="block-editor">
```

### Comparing `django-page-blocks-0.4.0/pageblocks/templates/admin/pageblocks/change_form.html` & `django-page-blocks-0.4.1/pageblocks/templates/admin/pageblocks/change_form.html`

 * *Files identical despite different names*

### Comparing `django-page-blocks-0.4.0/pageblocks/templatetags/__pycache__/pageblocks.cpython-310.pyc` & `django-page-blocks-0.4.1/pageblocks/templatetags/__pycache__/pageblocks.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat May 20 18:04:37 2023 UTC, .py size: 1066 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b50b 6964 2a04 0000  o.........id*...
+00000000: 6f0d 0d0a 0000 0000 500f 6964 2a04 0000  o.......P.id*...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 b200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 0100 6405  ..d.d.l.m.Z...d.
 00000060: 6406 6c08 6d09 5a09 0100 6501 a00a a100  d.l.m.Z...e.....
 00000070: 5a0b 650b 6a0c 6407 6408 8400 8301 5a0d  Z.e.j.d.d.....Z.
```

### Comparing `django-page-blocks-0.4.0/pageblocks/templatetags/__pycache__/pageblocks.cpython-39.pyc` & `django-page-blocks-0.4.1/pageblocks/templatetags/__pycache__/pageblocks.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-page-blocks-0.4.0/pageblocks/templatetags/pageblocks.py` & `django-page-blocks-0.4.1/pageblocks/templatetags/pageblocks.py`

 * *Files identical despite different names*

### Comparing `django-page-blocks-0.4.0/pageblocks/tests.py` & `django-page-blocks-0.4.1/pageblocks/tests.py`

 * *Files identical despite different names*

### Comparing `django-page-blocks-0.4.0/pageblocks/views.py` & `django-page-blocks-0.4.1/pageblocks/views.py`

 * *Files identical despite different names*

### Comparing `django-page-blocks-0.4.0/setup.py` & `django-page-blocks-0.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 with open(os.path.join(os.path.dirname(__file__), 'README.md')) as readme:
     README = readme.read()
 
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='django-page-blocks',
-    version='0.4.0',
+    version='0.4.1',
     packages=find_packages(),
     include_package_data=True,
     license='MIT License',
     description='A simple, Wagtail CMS inspired multi language content block engine for Django.  Intended to give slightly more control than regular flatpages.',
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://github.com/bravasoftware/django-page-blocks',
```

