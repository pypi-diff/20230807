# Comparing `tmp/panoptes-ui-0.2.2.tar.gz` & `tmp/panoptes-ui-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panoptes-ui-0.2.2.tar", last modified: Thu Aug  3 14:12:10 2023, max compression
+gzip compressed data, was "panoptes-ui-0.2.3.tar", last modified: Mon Aug  7 15:45:24 2023, max compression
```

## Comparing `panoptes-ui-0.2.2.tar` & `panoptes-ui-0.2.3.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:12:10.329707 panoptes-ui-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-08-03 14:12:10.329707 panoptes-ui-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:12:10.301707 panoptes-ui-0.2.2/panoptes/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/panoptes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:12:10.301707 panoptes-ui-0.2.2/panoptes/routes/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/routes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/routes/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/schema_forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:12:10.305707 panoptes-ui-0.2.2/panoptes/server_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/server_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/server_utilities/db_queries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:12:10.305707 panoptes-ui-0.2.2/panoptes/static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:12:10.305707 panoptes-ui-0.2.2/panoptes/static/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/404.html
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/about.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:12:10.309707 panoptes-ui-0.2.2/panoptes/static/src/css/
--rw-r--r--   0 runner    (1001) docker     (123)   336236 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/css/style.css
--rw-r--r--   0 runner    (1001) docker     (123)   773634 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/css/style.css.map
--rw-r--r--   0 runner    (1001) docker     (123)   276087 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/css/style.min.css
--rw-r--r--   0 runner    (1001) docker     (123)  1044838 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/css/style.min.css.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:12:10.309707 panoptes-ui-0.2.2/panoptes/static/src/img/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:12:10.313707 panoptes-ui-0.2.2/panoptes/static/src/img/avatars/
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/img/avatars/1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/img/avatars/2.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/img/avatars/3.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/img/avatars/4.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    19058 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/img/avatars/5.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/img/avatars/6.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/img/avatars/7.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    20466 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/img/avatars/8.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:12:10.317707 panoptes-ui-0.2.2/panoptes/static/src/img/brand/
--rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/img/brand/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/img/brand/panoptes.png
--rw-r--r--   0 runner    (1001) docker     (123)  1201622 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/img/brand/panoptes.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/img/brand/panoptes_eye.png
--rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/img/brand/panoptes_logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/img/brand/sygnet.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/img/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    10610 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/job.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:12:10.321707 panoptes-ui-0.2.2/panoptes/static/src/js/
--rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/js/charts.js
--rw-r--r--   0 runner    (1001) docker     (123)     9421 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/js/charts.js.map
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/js/colors.js
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/js/colors.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/js/main.js
--rw-r--r--   0 runner    (1001) docker     (123)    20520 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/js/main.js.map
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/js/popovers.js
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/js/popovers.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:12:10.321707 panoptes-ui-0.2.2/panoptes/static/src/js/src/
--rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/js/src/charts.js
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/js/src/colors.js
--rw-r--r--   0 runner    (1001) docker     (123)     9344 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/js/src/init.js
--rw-r--r--   0 runner    (1001) docker     (123)     8755 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/js/src/main.js
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/js/src/popovers.js
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/js/src/tooltips.js
--rw-r--r--   0 runner    (1001) docker     (123)    11320 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/js/src/widgets.js
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/js/tooltips.js
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/js/tooltips.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    11143 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/js/widgets.js
--rw-r--r--   0 runner    (1001) docker     (123)    27173 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/js/widgets.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:12:10.321707 panoptes-ui-0.2.2/panoptes/static/src/notifications/
--rw-r--r--   0 runner    (1001) docker     (123)    36471 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/notifications/alerts.html
--rw-r--r--   0 runner    (1001) docker     (123)    35530 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/notifications/badge.html
--rw-r--r--   0 runner    (1001) docker     (123)    41078 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/notifications/modals.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:12:10.325707 panoptes-ui-0.2.2/panoptes/static/src/scss/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/scss/_custom.scss
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/scss/_variables.scss
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/scss/style.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:12:10.325707 panoptes-ui-0.2.2/panoptes/static/src/scss/vendors/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/scss/vendors/_variables.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:12:10.325707 panoptes-ui-0.2.2/panoptes/static/src/scss/vendors/pace-progress/
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/scss/vendors/pace-progress/pace.scss
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/searchResults.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:12:10.297707 panoptes-ui-0.2.2/panoptes/static/src/vendors/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:12:10.297707 panoptes-ui-0.2.2/panoptes/static/src/vendors/pace-progress/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:12:10.325707 panoptes-ui-0.2.2/panoptes/static/src/vendors/pace-progress/css/
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/vendors/pace-progress/css/pace.css
--rw-r--r--   0 runner    (1001) docker     (123)   117500 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/vendors/pace-progress/css/pace.css.map
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/vendors/pace-progress/css/pace.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   117477 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/vendors/pace-progress/css/pace.min.css.map
--rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/workflow.html
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/static/src/workflows.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:12:10.325707 panoptes-ui-0.2.2/panoptes/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7469 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/tests/api_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/panoptes/tests/api_test_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:12:10.329707 panoptes-ui-0.2.2/panoptes_ui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-08-03 14:12:10.000000 panoptes-ui-0.2.2/panoptes_ui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-08-03 14:12:10.000000 panoptes-ui-0.2.2/panoptes_ui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 14:12:10.000000 panoptes-ui-0.2.2/panoptes_ui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-03 14:12:10.000000 panoptes-ui-0.2.2/panoptes_ui.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-03 14:12:10.000000 panoptes-ui-0.2.2/panoptes_ui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-03 14:12:10.000000 panoptes-ui-0.2.2/panoptes_ui.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 14:12:10.329707 panoptes-ui-0.2.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1147 2023-08-03 14:11:59.000000 panoptes-ui-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:45:24.259642 panoptes-ui-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-08-07 15:45:10.000000 panoptes-ui-0.2.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-07 15:45:10.000000 panoptes-ui-0.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-08-07 15:45:24.259642 panoptes-ui-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-08-07 15:45:10.000000 panoptes-ui-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:45:24.243642 panoptes-ui-0.2.3/panoptes/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-07 15:45:10.000000 panoptes-ui-0.2.3/panoptes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-08-07 15:45:10.000000 panoptes-ui-0.2.3/panoptes/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-08-07 15:45:10.000000 panoptes-ui-0.2.3/panoptes/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-08-07 15:45:10.000000 panoptes-ui-0.2.3/panoptes/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-08-07 15:45:10.000000 panoptes-ui-0.2.3/panoptes/panoptes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:45:24.243642 panoptes-ui-0.2.3/panoptes/routes/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-08-07 15:45:10.000000 panoptes-ui-0.2.3/panoptes/routes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-08-07 15:45:10.000000 panoptes-ui-0.2.3/panoptes/routes/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-08-07 15:45:10.000000 panoptes-ui-0.2.3/panoptes/schema_forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:45:24.243642 panoptes-ui-0.2.3/panoptes/server_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 15:45:10.000000 panoptes-ui-0.2.3/panoptes/server_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-08-07 15:45:10.000000 panoptes-ui-0.2.3/panoptes/server_utilities/db_queries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:45:24.243642 panoptes-ui-0.2.3/panoptes/static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 15:45:10.000000 panoptes-ui-0.2.3/panoptes/static/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:45:24.243642 panoptes-ui-0.2.3/panoptes/static/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-08-07 15:45:10.000000 panoptes-ui-0.2.3/panoptes/static/src/404.html
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 15:45:10.000000 panoptes-ui-0.2.3/panoptes/static/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-08-07 15:45:10.000000 panoptes-ui-0.2.3/panoptes/static/src/about.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:45:24.247642 panoptes-ui-0.2.3/panoptes/static/src/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   336236 2023-08-07 15:45:10.000000 panoptes-ui-0.2.3/panoptes/static/src/css/style.css
+-rw-r--r--   0 runner    (1001) docker     (123)   773634 2023-08-07 15:45:10.000000 panoptes-ui-0.2.3/panoptes/static/src/css/style.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)   276087 2023-08-07 15:45:10.000000 panoptes-ui-0.2.3/panoptes/static/src/css/style.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)  1044838 2023-08-07 15:45:10.000000 panoptes-ui-0.2.3/panoptes/static/src/css/style.min.css.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:45:24.247642 panoptes-ui-0.2.3/panoptes/static/src/img/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:45:24.247642 panoptes-ui-0.2.3/panoptes/static/src/img/avatars/
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-08-07 15:45:10.000000 panoptes-ui-0.2.3/panoptes/static/src/img/avatars/1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-08-07 15:45:10.000000 panoptes-ui-0.2.3/panoptes/static/src/img/avatars/2.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-08-07 15:45:10.000000 panoptes-ui-0.2.3/panoptes/static/src/img/avatars/3.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-08-07 15:45:10.000000 panoptes-ui-0.2.3/panoptes/static/src/img/avatars/4.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    19058 2023-08-07 15:45:10.000000 panoptes-ui-0.2.3/panoptes/static/src/img/avatars/5.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-08-07 15:45:10.000000 panoptes-ui-0.2.3/panoptes/static/src/img/avatars/6.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-08-07 15:45:10.000000 panoptes-ui-0.2.3/panoptes/static/src/img/avatars/7.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    20466 2023-08-07 15:45:10.000000 panoptes-ui-0.2.3/panoptes/static/src/img/avatars/8.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:45:24.251642 panoptes-ui-0.2.3/panoptes/static/src/img/brand/
+-rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-08-07 15:45:10.000000 panoptes-ui-0.2.3/panoptes/static/src/img/brand/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-08-07 15:45:10.000000 panoptes-ui-0.2.3/panoptes/static/src/img/brand/panoptes.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1201622 2023-08-07 15:45:10.000000 panoptes-ui-0.2.3/panoptes/static/src/img/brand/panoptes.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-08-07 15:45:10.000000 panoptes-ui-0.2.3/panoptes/static/src/img/brand/panoptes_eye.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-08-07 15:45:10.000000 panoptes-ui-0.2.3/panoptes/static/src/img/brand/panoptes_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-08-07 15:45:10.000000 panoptes-ui-0.2.3/panoptes/static/src/img/brand/sygnet.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-08-07 15:45:10.000000 panoptes-ui-0.2.3/panoptes/static/src/img/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    10610 2023-08-07 15:45:10.000000 panoptes-ui-0.2.3/panoptes/static/src/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-08-07 15:45:10.000000 panoptes-ui-0.2.3/panoptes/static/src/job.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:45:24.255642 panoptes-ui-0.2.3/panoptes/static/src/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-08-07 15:45:10.000000 panoptes-ui-0.2.3/panoptes/static/src/js/charts.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9421 2023-08-07 15:45:10.000000 panoptes-ui-0.2.3/panoptes/static/src/js/charts.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-08-07 15:45:10.000000 panoptes-ui-0.2.3/panoptes/static/src/js/colors.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-08-07 15:45:10.000000 panoptes-ui-0.2.3/panoptes/static/src/js/colors.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-08-07 15:45:10.000000 panoptes-ui-0.2.3/panoptes/static/src/js/main.js
+-rw-r--r--   0 runner    (1001) docker     (123)    20520 2023-08-07 15:45:10.000000 panoptes-ui-0.2.3/panoptes/static/src/js/main.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-08-07 15:45:10.000000 panoptes-ui-0.2.3/panoptes/static/src/js/popovers.js
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-08-07 15:45:10.000000 panoptes-ui-0.2.3/panoptes/static/src/js/popovers.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:45:24.255642 panoptes-ui-0.2.3/panoptes/static/src/js/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-08-07 15:45:10.000000 panoptes-ui-0.2.3/panoptes/static/src/js/src/charts.js
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-08-07 15:45:10.000000 panoptes-ui-0.2.3/panoptes/static/src/js/src/colors.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9344 2023-08-07 15:45:10.000000 panoptes-ui-0.2.3/panoptes/static/src/js/src/init.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8755 2023-08-07 15:45:10.000000 panoptes-ui-0.2.3/panoptes/static/src/js/src/main.js
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-08-07 15:45:10.000000 panoptes-ui-0.2.3/panoptes/static/src/js/src/popovers.js
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-08-07 15:45:10.000000 panoptes-ui-0.2.3/panoptes/static/src/js/src/tooltips.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11320 2023-08-07 15:45:10.000000 panoptes-ui-0.2.3/panoptes/static/src/js/src/widgets.js
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-08-07 15:45:10.000000 panoptes-ui-0.2.3/panoptes/static/src/js/tooltips.js
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-08-07 15:45:10.000000 panoptes-ui-0.2.3/panoptes/static/src/js/tooltips.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    11143 2023-08-07 15:45:10.000000 panoptes-ui-0.2.3/panoptes/static/src/js/widgets.js
+-rw-r--r--   0 runner    (1001) docker     (123)    27173 2023-08-07 15:45:10.000000 panoptes-ui-0.2.3/panoptes/static/src/js/widgets.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:45:24.255642 panoptes-ui-0.2.3/panoptes/static/src/notifications/
+-rw-r--r--   0 runner    (1001) docker     (123)    36471 2023-08-07 15:45:10.000000 panoptes-ui-0.2.3/panoptes/static/src/notifications/alerts.html
+-rw-r--r--   0 runner    (1001) docker     (123)    35530 2023-08-07 15:45:10.000000 panoptes-ui-0.2.3/panoptes/static/src/notifications/badge.html
+-rw-r--r--   0 runner    (1001) docker     (123)    41078 2023-08-07 15:45:10.000000 panoptes-ui-0.2.3/panoptes/static/src/notifications/modals.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:45:24.255642 panoptes-ui-0.2.3/panoptes/static/src/scss/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-07 15:45:10.000000 panoptes-ui-0.2.3/panoptes/static/src/scss/_custom.scss
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-07 15:45:10.000000 panoptes-ui-0.2.3/panoptes/static/src/scss/_variables.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-08-07 15:45:10.000000 panoptes-ui-0.2.3/panoptes/static/src/scss/style.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:45:24.255642 panoptes-ui-0.2.3/panoptes/static/src/scss/vendors/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-08-07 15:45:10.000000 panoptes-ui-0.2.3/panoptes/static/src/scss/vendors/_variables.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:45:24.255642 panoptes-ui-0.2.3/panoptes/static/src/scss/vendors/pace-progress/
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-08-07 15:45:10.000000 panoptes-ui-0.2.3/panoptes/static/src/scss/vendors/pace-progress/pace.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-08-07 15:45:10.000000 panoptes-ui-0.2.3/panoptes/static/src/searchResults.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:45:24.239642 panoptes-ui-0.2.3/panoptes/static/src/vendors/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:45:24.239642 panoptes-ui-0.2.3/panoptes/static/src/vendors/pace-progress/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:45:24.259642 panoptes-ui-0.2.3/panoptes/static/src/vendors/pace-progress/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-08-07 15:45:10.000000 panoptes-ui-0.2.3/panoptes/static/src/vendors/pace-progress/css/pace.css
+-rw-r--r--   0 runner    (1001) docker     (123)   117500 2023-08-07 15:45:10.000000 panoptes-ui-0.2.3/panoptes/static/src/vendors/pace-progress/css/pace.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-08-07 15:45:10.000000 panoptes-ui-0.2.3/panoptes/static/src/vendors/pace-progress/css/pace.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   117477 2023-08-07 15:45:10.000000 panoptes-ui-0.2.3/panoptes/static/src/vendors/pace-progress/css/pace.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-08-07 15:45:10.000000 panoptes-ui-0.2.3/panoptes/static/src/workflow.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-08-07 15:45:10.000000 panoptes-ui-0.2.3/panoptes/static/src/workflows.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:45:24.259642 panoptes-ui-0.2.3/panoptes/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 15:45:10.000000 panoptes-ui-0.2.3/panoptes/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7469 2023-08-07 15:45:10.000000 panoptes-ui-0.2.3/panoptes/tests/api_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-08-07 15:45:10.000000 panoptes-ui-0.2.3/panoptes/tests/api_test_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:45:24.259642 panoptes-ui-0.2.3/panoptes_ui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-08-07 15:45:24.000000 panoptes-ui-0.2.3/panoptes_ui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-08-07 15:45:24.000000 panoptes-ui-0.2.3/panoptes_ui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 15:45:24.000000 panoptes-ui-0.2.3/panoptes_ui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-07 15:45:24.000000 panoptes-ui-0.2.3/panoptes_ui.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-07 15:45:24.000000 panoptes-ui-0.2.3/panoptes_ui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-07 15:45:24.000000 panoptes-ui-0.2.3/panoptes_ui.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 15:45:24.259642 panoptes-ui-0.2.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1147 2023-08-07 15:45:10.000000 panoptes-ui-0.2.3/setup.py
```

### Comparing `panoptes-ui-0.2.2/LICENSE.md` & `panoptes-ui-0.2.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.2/PKG-INFO` & `panoptes-ui-0.2.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panoptes-ui
-Version: 0.2.2
+Version: 0.2.3
 Summary: panoptes: monitor computational workflows in real time
 Home-page: https://github.com/panoptes-organization/panoptes
 Author: panoptes-organization
 Author-email: georgekostoulas@gmail.com, agardelakos@gmail.com, fgypas@gmail.com, gntalaperas@gmail.com, dimitris.afe@gmail.com, rekoumisd@gmail.com, vsochat@stanford.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `panoptes-ui-0.2.2/README.md` & `panoptes-ui-0.2.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -8,23 +8,20 @@
 - Administrations that want to monitor their servers
 - Web developers that want to integrate the service in bigger web applications
 
 **Note:** panoptes is in early development stage and the first proof of concept server will support only workflows written in [snakemake](https://snakemake.readthedocs.io/en/stable/).
 
 # Installation
 
-## Basic installation process
-
-### Requirements
-
+Requirements:
 - Python>=3.6
 - virtualenv
 - [sqlite3](https://www.sqlite.org/download.html)
 
-### Option 1: Install via pypi and run server
+## Install from pypi and run server
 
 Create virtual environment
 ```bash
 virtualenv -p `which python3` venv
 ```
 
 Activate virtual environment
@@ -40,39 +37,35 @@
 ```bash
 panoptes
 ```
 Server should run on: 127.0.0.1:5000
 
 By default it should generate an sqlite database: .panoptes.db
 
-### Option 2: Install via conda and run server
+## Install from conda and run server
 
 Create conda environment
 ```bash
-conda create --name panoptes
+conda create --name panoptes -c conda-forge -c bioconda panoptes-ui
 ```
 
 Activate conda environment
 ```bash
 conda activate panoptes
 ```
 
-Install via pypi OR conda
-```bash
-conda install -c panoptes-organization panoptes-ui
-```
 Run server
 ```bash
 panoptes
 ```
 Server should run on: 127.0.0.1:5000
 
 By default it should generate an sqlite database: .panoptes.db
 
-### Option 3: Install from source code and run server
+## Install from source code and run server
 
 Clone repo
 ```bash
 git clone https://github.com/panoptes-organization/panoptes.git
 ```
 
 Enter repo
@@ -99,23 +92,38 @@
 ```bash
 panoptes
 ```
 Server should run on: 127.0.0.1:5000
 
 By default it should generate an sqlite database: .panoptes.db 
 
-## Docker installation
+## Docker execution
+
+Requirements:
+- docker
+
+Pull image that is automatically built from bioconda. You can find the latest tag in the following url: https://quay.io/repository/biocontainers/panoptes-ui?tab=tags. For example:
+```
+docker pull quay.io/biocontainers/panoptes-ui:0.2.2--pyh7cba7a3_0
+```
+
+Then run the container with:
 
-### Requirements
+```bash
+docker run -p 5000:5000 -it "image id" panoptes
+```
 
+> Note: In this case the database is stored within the docker image, so every time you restart the server the database will be empty. You would need to mount the volumes to make the database persistent.
+
+## Docker compose execution
+
+Requirements:
 - docker
 - docker-compose
 
-### Build and run with docker-compose
-
 Build
 ```bash
 docker-compose build
 ```
 
 Run
 ```bash
@@ -125,23 +133,36 @@
 Server should run on: http://127.0.0.1:8000
 
 Stop
 ```bash
 docker-compose down
 ```
 
-### Run an example workflow
+## Singularity execution
+
+You can also deploy the server with singularity. To do so pull the image with singularity. For example:
+
+```bash
+singularity pull docker://quay.io/biocontainers/panoptes-ui:0.2.2--pyh7cba7a3_0
+```
+
+And then we can start the server by running:
+```bash
+singularity exec panoptes-ui:0.2.2--pyh7cba7a3_0
+```
+
+# Run an example workflow
 
 In order to run an example workflow please follow the instructions [here](https://github.com/panoptes-organization/snakemake_example_workflow)
 
-### panoptes in action
+## panoptes in action
 
 [![Watch the video](https://img.youtube.com/vi/de-YSJmq_5s/hqdefault.jpg)](https://www.youtube.com/watch?v=de-YSJmq_5s)
 
-### panoptes API
+## panoptes API
 
 Panoptes provides the following API endpoints:
 
 Endpoint | Method | Description 
 -- | -- | --
 `/api/service-info` | `GET` | Server status
 `/api/workflows` | `GET` | Get all workflows
@@ -162,12 +183,12 @@
 
 # Contribute
 
 Please see the [Contributing instructions](CONTRIBUTING.md).
 
 ## CI server
 
-Changes in develop or master trigger a [Travis](https://travis-ci.com/panoptes-organization/panoptes) build (and runs tests)
+Changes in develop or master trigger a [GitHub Actions](https://github.com/panoptes-organization/panoptes/actions) build (and runs tests)
 
 # Contact
 
 In case the [issues section](https://github.com/panoptes-organization/panoptes/issues) is not enough for you, you can also contact us via [discord](https://discord.gg/vMcZCVZ)
```

### Comparing `panoptes-ui-0.2.2/panoptes/app.py` & `panoptes-ui-0.2.3/panoptes/app.py`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.2/panoptes/database.py` & `panoptes-ui-0.2.3/panoptes/database.py`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.2/panoptes/models.py` & `panoptes-ui-0.2.3/panoptes/models.py`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.2/panoptes/panoptes.py` & `panoptes-ui-0.2.3/panoptes/panoptes.py`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.2/panoptes/routes/api.py` & `panoptes-ui-0.2.3/panoptes/routes/api.py`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.2/panoptes/schema_forms.py` & `panoptes-ui-0.2.3/panoptes/schema_forms.py`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.2/panoptes/server_utilities/db_queries.py` & `panoptes-ui-0.2.3/panoptes/server_utilities/db_queries.py`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.2/panoptes/static/src/404.html` & `panoptes-ui-0.2.3/panoptes/static/src/404.html`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.2/panoptes/static/src/about.html` & `panoptes-ui-0.2.3/panoptes/static/src/about.html`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.2/panoptes/static/src/css/style.css` & `panoptes-ui-0.2.3/panoptes/static/src/css/style.css`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.2/panoptes/static/src/css/style.css.map` & `panoptes-ui-0.2.3/panoptes/static/src/css/style.css.map`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.2/panoptes/static/src/css/style.min.css` & `panoptes-ui-0.2.3/panoptes/static/src/css/style.min.css`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.2/panoptes/static/src/css/style.min.css.map` & `panoptes-ui-0.2.3/panoptes/static/src/css/style.min.css.map`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.2/panoptes/static/src/img/avatars/1.jpg` & `panoptes-ui-0.2.3/panoptes/static/src/img/avatars/1.jpg`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.2/panoptes/static/src/img/avatars/2.jpg` & `panoptes-ui-0.2.3/panoptes/static/src/img/avatars/2.jpg`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.2/panoptes/static/src/img/avatars/3.jpg` & `panoptes-ui-0.2.3/panoptes/static/src/img/avatars/3.jpg`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.2/panoptes/static/src/img/avatars/4.jpg` & `panoptes-ui-0.2.3/panoptes/static/src/img/avatars/4.jpg`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.2/panoptes/static/src/img/avatars/5.jpg` & `panoptes-ui-0.2.3/panoptes/static/src/img/avatars/5.jpg`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.2/panoptes/static/src/img/avatars/6.jpg` & `panoptes-ui-0.2.3/panoptes/static/src/img/avatars/6.jpg`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.2/panoptes/static/src/img/avatars/7.jpg` & `panoptes-ui-0.2.3/panoptes/static/src/img/avatars/7.jpg`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.2/panoptes/static/src/img/avatars/8.jpg` & `panoptes-ui-0.2.3/panoptes/static/src/img/avatars/8.jpg`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.2/panoptes/static/src/img/brand/logo.svg` & `panoptes-ui-0.2.3/panoptes/static/src/img/brand/logo.svg`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.2/panoptes/static/src/img/brand/panoptes.png` & `panoptes-ui-0.2.3/panoptes/static/src/img/brand/panoptes.png`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.2/panoptes/static/src/img/brand/panoptes.svg` & `panoptes-ui-0.2.3/panoptes/static/src/img/brand/panoptes.svg`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.2/panoptes/static/src/img/brand/panoptes_eye.png` & `panoptes-ui-0.2.3/panoptes/static/src/img/brand/panoptes_eye.png`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.2/panoptes/static/src/img/brand/panoptes_logo.svg` & `panoptes-ui-0.2.3/panoptes/static/src/img/brand/panoptes_logo.svg`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.2/panoptes/static/src/img/brand/sygnet.svg` & `panoptes-ui-0.2.3/panoptes/static/src/img/brand/sygnet.svg`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.2/panoptes/static/src/img/favicon.ico` & `panoptes-ui-0.2.3/panoptes/static/src/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.2/panoptes/static/src/index.html` & `panoptes-ui-0.2.3/panoptes/static/src/index.html`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.2/panoptes/static/src/job.html` & `panoptes-ui-0.2.3/panoptes/static/src/job.html`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.2/panoptes/static/src/js/charts.js` & `panoptes-ui-0.2.3/panoptes/static/src/js/charts.js`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.2/panoptes/static/src/js/charts.js.map` & `panoptes-ui-0.2.3/panoptes/static/src/js/charts.js.map`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.2/panoptes/static/src/js/colors.js` & `panoptes-ui-0.2.3/panoptes/static/src/js/colors.js`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.2/panoptes/static/src/js/colors.js.map` & `panoptes-ui-0.2.3/panoptes/static/src/js/colors.js.map`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.2/panoptes/static/src/js/main.js` & `panoptes-ui-0.2.3/panoptes/static/src/js/main.js`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.2/panoptes/static/src/js/main.js.map` & `panoptes-ui-0.2.3/panoptes/static/src/js/main.js.map`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.2/panoptes/static/src/js/popovers.js.map` & `panoptes-ui-0.2.3/panoptes/static/src/js/popovers.js.map`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.2/panoptes/static/src/js/src/charts.js` & `panoptes-ui-0.2.3/panoptes/static/src/js/src/charts.js`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.2/panoptes/static/src/js/src/colors.js` & `panoptes-ui-0.2.3/panoptes/static/src/js/src/colors.js`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.2/panoptes/static/src/js/src/init.js` & `panoptes-ui-0.2.3/panoptes/static/src/js/src/init.js`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.2/panoptes/static/src/js/src/main.js` & `panoptes-ui-0.2.3/panoptes/static/src/js/src/main.js`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.2/panoptes/static/src/js/src/widgets.js` & `panoptes-ui-0.2.3/panoptes/static/src/js/src/widgets.js`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.2/panoptes/static/src/js/tooltips.js.map` & `panoptes-ui-0.2.3/panoptes/static/src/js/tooltips.js.map`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.2/panoptes/static/src/js/widgets.js` & `panoptes-ui-0.2.3/panoptes/static/src/js/widgets.js`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.2/panoptes/static/src/js/widgets.js.map` & `panoptes-ui-0.2.3/panoptes/static/src/js/widgets.js.map`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.2/panoptes/static/src/notifications/alerts.html` & `panoptes-ui-0.2.3/panoptes/static/src/notifications/alerts.html`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.2/panoptes/static/src/notifications/badge.html` & `panoptes-ui-0.2.3/panoptes/static/src/notifications/badge.html`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.2/panoptes/static/src/notifications/modals.html` & `panoptes-ui-0.2.3/panoptes/static/src/notifications/modals.html`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.2/panoptes/static/src/scss/vendors/pace-progress/pace.scss` & `panoptes-ui-0.2.3/panoptes/static/src/scss/vendors/pace-progress/pace.scss`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.2/panoptes/static/src/searchResults.html` & `panoptes-ui-0.2.3/panoptes/static/src/searchResults.html`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.2/panoptes/static/src/vendors/pace-progress/css/pace.css` & `panoptes-ui-0.2.3/panoptes/static/src/vendors/pace-progress/css/pace.css`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.2/panoptes/static/src/vendors/pace-progress/css/pace.css.map` & `panoptes-ui-0.2.3/panoptes/static/src/vendors/pace-progress/css/pace.css.map`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.2/panoptes/static/src/vendors/pace-progress/css/pace.min.css` & `panoptes-ui-0.2.3/panoptes/static/src/vendors/pace-progress/css/pace.min.css`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.2/panoptes/static/src/vendors/pace-progress/css/pace.min.css.map` & `panoptes-ui-0.2.3/panoptes/static/src/vendors/pace-progress/css/pace.min.css.map`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.2/panoptes/static/src/workflow.html` & `panoptes-ui-0.2.3/panoptes/static/src/workflow.html`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.2/panoptes/static/src/workflows.html` & `panoptes-ui-0.2.3/panoptes/static/src/workflows.html`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.2/panoptes/tests/api_test.py` & `panoptes-ui-0.2.3/panoptes/tests/api_test.py`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.2/panoptes/tests/api_test_helper.py` & `panoptes-ui-0.2.3/panoptes/tests/api_test_helper.py`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.2/panoptes_ui.egg-info/PKG-INFO` & `panoptes-ui-0.2.3/panoptes_ui.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panoptes-ui
-Version: 0.2.2
+Version: 0.2.3
 Summary: panoptes: monitor computational workflows in real time
 Home-page: https://github.com/panoptes-organization/panoptes
 Author: panoptes-organization
 Author-email: georgekostoulas@gmail.com, agardelakos@gmail.com, fgypas@gmail.com, gntalaperas@gmail.com, dimitris.afe@gmail.com, rekoumisd@gmail.com, vsochat@stanford.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `panoptes-ui-0.2.2/panoptes_ui.egg-info/SOURCES.txt` & `panoptes-ui-0.2.3/panoptes_ui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `panoptes-ui-0.2.2/setup.py` & `panoptes-ui-0.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 if sys.version_info < (3, 6):
     sys.exit('Sorry, panoptes requires Python >= 3.6')
 
 setup(
     name='panoptes-ui',
-    version='0.2.2',
+    version='0.2.3',
     url='https://github.com/panoptes-organization/panoptes',
     license='MIT',
     author='panoptes-organization',
     author_email='georgekostoulas@gmail.com, agardelakos@gmail.com, fgypas@gmail.com, gntalaperas@gmail.com, dimitris.afe@gmail.com, rekoumisd@gmail.com, vsochat@stanford.edu',
     description="panoptes: monitor computational workflows in real time",
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
```

