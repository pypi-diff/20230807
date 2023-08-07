# Comparing `tmp/forecastmanager-0.1.4.tar.gz` & `tmp/forecastmanager-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forecastmanager-0.1.4.tar", last modified: Mon Jul 31 11:19:16 2023, max compression
+gzip compressed data, was "forecastmanager-0.1.5.tar", last modified: Mon Aug  7 09:55:17 2023, max compression
```

## Comparing `forecastmanager-0.1.4.tar` & `forecastmanager-0.1.5.tar`

### file list

```diff
@@ -1,112 +1,114 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:19:16.743251 forecastmanager-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-31 11:19:16.743251 forecastmanager-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:19:16.731251 forecastmanager-0.1.4/forecastmanager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/forecastmanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/forecastmanager/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/forecastmanager/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/forecastmanager/blocks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:19:16.727250 forecastmanager-0.1.4/forecastmanager/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:19:16.727250 forecastmanager-0.1.4/forecastmanager/locale/am/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:19:16.731251 forecastmanager-0.1.4/forecastmanager/locale/am/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    10121 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/forecastmanager/locale/am/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    15641 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/forecastmanager/locale/am/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:19:16.727250 forecastmanager-0.1.4/forecastmanager/locale/ar/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:19:16.735251 forecastmanager-0.1.4/forecastmanager/locale/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     9613 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/forecastmanager/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    15149 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/forecastmanager/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:19:16.727250 forecastmanager-0.1.4/forecastmanager/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:19:16.735251 forecastmanager-0.1.4/forecastmanager/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     8096 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/forecastmanager/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    13635 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/forecastmanager/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:19:16.727250 forecastmanager-0.1.4/forecastmanager/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:19:16.735251 forecastmanager-0.1.4/forecastmanager/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     8721 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/forecastmanager/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    14260 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/forecastmanager/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:19:16.727250 forecastmanager-0.1.4/forecastmanager/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:19:16.735251 forecastmanager-0.1.4/forecastmanager/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     8921 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/forecastmanager/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    14463 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/forecastmanager/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:19:16.727250 forecastmanager-0.1.4/forecastmanager/locale/sw/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:19:16.735251 forecastmanager-0.1.4/forecastmanager/locale/sw/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     8396 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/forecastmanager/locale/sw/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    13932 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/forecastmanager/locale/sw/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:19:16.735251 forecastmanager-0.1.4/forecastmanager/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/forecastmanager/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:19:16.735251 forecastmanager-0.1.4/forecastmanager/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/forecastmanager/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/forecastmanager/management/commands/generate_forecast.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:19:16.735251 forecastmanager-0.1.4/forecastmanager/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/forecastmanager/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/forecastmanager/migrations/0002_remove_forecast_max_temp_remove_forecast_min_temp_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/forecastmanager/migrations/0003_alter_forecast_unique_together.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/forecastmanager/migrations/0004_forecastdataparameters_parameter_type_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/forecastmanager/migrations/0005_alter_forecastdataparameters_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/forecastmanager/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/forecastmanager/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/forecastmanager/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/forecastmanager/site_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:19:16.731251 forecastmanager-0.1.4/forecastmanager/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:19:16.731251 forecastmanager-0.1.4/forecastmanager/static/forecastmanager/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:19:16.743251 forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/clearsky.png
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/cloudy.png
--rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/fair.png
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/fog.png
--rw-r--r--   0 runner    (1001) docker     (123)     7110 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/heavyrain.png
--rw-r--r--   0 runner    (1001) docker     (123)     7775 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/heavyrainandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)    10436 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/heavyrainshowers.png
--rw-r--r--   0 runner    (1001) docker     (123)    11254 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/heavyrainshowersandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)     7441 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/heavysleet.png
--rw-r--r--   0 runner    (1001) docker     (123)     8197 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/heavysleetandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)    11065 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/heavysleetshowers.png
--rw-r--r--   0 runner    (1001) docker     (123)    11822 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/heavysleetshowersandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)     7075 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/heavysnow.png
--rw-r--r--   0 runner    (1001) docker     (123)     7853 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/heavysnowandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)    10344 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/heavysnowshowers.png
--rw-r--r--   0 runner    (1001) docker     (123)    11258 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/heavysnowshowersandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)     6757 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/lightrain.png
--rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/lightrainandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)     9867 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/lightrainshowers.png
--rw-r--r--   0 runner    (1001) docker     (123)     6993 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/lightsleet.png
--rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/lightsleetandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)    10097 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/lightsleetshowers.png
--rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/lightsnow.png
--rw-r--r--   0 runner    (1001) docker     (123)     7705 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/lightsnowandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/lightsnowshowers.png
--rw-r--r--   0 runner    (1001) docker     (123)    11113 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/lightssleetshowersandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)    11046 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/lightssnowshowersandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)     8879 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/partlycloudy.png
--rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/rain.png
--rw-r--r--   0 runner    (1001) docker     (123)     7645 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/rainandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)    10027 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/rainshowers.png
--rw-r--r--   0 runner    (1001) docker     (123)    10986 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/rainshowersandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)     7325 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/sleet.png
--rw-r--r--   0 runner    (1001) docker     (123)     7959 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/sleetandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)    10521 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/sleetshowers.png
--rw-r--r--   0 runner    (1001) docker     (123)    11328 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/sleetshowersandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)     7040 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/snow.png
--rw-r--r--   0 runner    (1001) docker     (123)     7754 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/snowandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)    10208 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/snowshowers.png
--rw-r--r--   0 runner    (1001) docker     (123)    11183 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/snowshowersandthunder.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:19:16.743251 forecastmanager-0.1.4/forecastmanager/static/forecastmanager/js/
--rw-r--r--   0 runner    (1001) docker     (123)    38899 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/forecastmanager/static/forecastmanager/js/forecast_basemap.js
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/forecastmanager/static/forecastmanager/js/helpers.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:19:16.731251 forecastmanager-0.1.4/forecastmanager/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:19:16.743251 forecastmanager-0.1.4/forecastmanager/templates/forecastmanager/
--rw-r--r--   0 runner    (1001) docker     (123)    20746 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/forecastmanager/templates/forecastmanager/create_forecast.html
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/forecastmanager/templates/forecastmanager/forecast_base.html
--rw-r--r--   0 runner    (1001) docker     (123)    11365 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/forecastmanager/templates/forecastmanager/view_forecast.html
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/forecastmanager/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/forecastmanager/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     6845 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/forecastmanager/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/forecastmanager/wagtail_hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:19:16.731251 forecastmanager-0.1.4/forecastmanager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-31 11:19:16.000000 forecastmanager-0.1.4/forecastmanager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-07-31 11:19:16.000000 forecastmanager-0.1.4/forecastmanager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 11:19:16.000000 forecastmanager-0.1.4/forecastmanager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-31 11:19:16.000000 forecastmanager-0.1.4/forecastmanager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-31 11:19:16.000000 forecastmanager-0.1.4/forecastmanager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-31 11:18:58.000000 forecastmanager-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-31 11:19:16.743251 forecastmanager-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:55:17.089048 forecastmanager-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-08-07 09:55:17.089048 forecastmanager-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:55:17.057047 forecastmanager-0.1.5/forecastmanager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/blocks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:55:17.049046 forecastmanager-0.1.5/forecastmanager/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:55:17.049046 forecastmanager-0.1.5/forecastmanager/locale/am/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:55:17.061047 forecastmanager-0.1.5/forecastmanager/locale/am/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    10121 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/locale/am/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    15641 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/locale/am/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:55:17.049046 forecastmanager-0.1.5/forecastmanager/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:55:17.061047 forecastmanager-0.1.5/forecastmanager/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     9613 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    15149 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:55:17.049046 forecastmanager-0.1.5/forecastmanager/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:55:17.065047 forecastmanager-0.1.5/forecastmanager/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     8096 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    13635 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:55:17.049046 forecastmanager-0.1.5/forecastmanager/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:55:17.065047 forecastmanager-0.1.5/forecastmanager/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     8721 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    14260 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:55:17.049046 forecastmanager-0.1.5/forecastmanager/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:55:17.065047 forecastmanager-0.1.5/forecastmanager/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     8921 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    14463 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:55:17.049046 forecastmanager-0.1.5/forecastmanager/locale/sw/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:55:17.065047 forecastmanager-0.1.5/forecastmanager/locale/sw/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     8396 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/locale/sw/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    13932 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/locale/sw/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:55:17.065047 forecastmanager-0.1.5/forecastmanager/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:55:17.065047 forecastmanager-0.1.5/forecastmanager/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/management/commands/generate_forecast.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:55:17.069047 forecastmanager-0.1.5/forecastmanager/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/migrations/0002_remove_forecast_max_temp_remove_forecast_min_temp_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/migrations/0003_alter_forecast_unique_together.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/migrations/0004_forecastdataparameters_parameter_type_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/migrations/0005_alter_forecastdataparameters_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/migrations/0006_alter_forecastsetting_enable_auto_forecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/site_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:55:17.053047 forecastmanager-0.1.5/forecastmanager/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:55:17.053047 forecastmanager-0.1.5/forecastmanager/static/forecastmanager/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:55:17.085048 forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/clearsky.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/cloudy.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/fair.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/fog.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7110 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/heavyrain.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7775 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/heavyrainandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10436 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/heavyrainshowers.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11254 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/heavyrainshowersandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7441 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/heavysleet.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8197 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/heavysleetandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11065 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/heavysleetshowers.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11822 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/heavysleetshowersandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7075 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/heavysnow.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7853 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/heavysnowandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10344 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/heavysnowshowers.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11258 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/heavysnowshowersandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6757 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/lightrain.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/lightrainandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9867 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/lightrainshowers.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6993 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/lightsleet.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/lightsleetandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10097 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/lightsleetshowers.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/lightsnow.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7705 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/lightsnowandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/lightsnowshowers.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11113 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/lightssleetshowersandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11046 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/lightssnowshowersandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8879 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/partlycloudy.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/rain.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7645 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/rainandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10027 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/rainshowers.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10986 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/rainshowersandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7325 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/sleet.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7959 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/sleetandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10521 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/sleetshowers.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11328 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/sleetshowersandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7040 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/snow.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7754 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/snowandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10208 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/snowshowers.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11183 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/snowshowersandthunder.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:55:17.085048 forecastmanager-0.1.5/forecastmanager/static/forecastmanager/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    38899 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/static/forecastmanager/js/forecast_basemap.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/static/forecastmanager/js/helpers.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:55:17.053047 forecastmanager-0.1.5/forecastmanager/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:55:17.089048 forecastmanager-0.1.5/forecastmanager/templates/forecastmanager/
+-rw-r--r--   0 runner    (1001) docker     (123)    20746 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/templates/forecastmanager/create_forecast.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/templates/forecastmanager/forecast_base.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11365 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/templates/forecastmanager/view_forecast.html
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6845 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/forecastmanager/wagtail_hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:55:17.061047 forecastmanager-0.1.5/forecastmanager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-08-07 09:55:17.000000 forecastmanager-0.1.5/forecastmanager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-08-07 09:55:17.000000 forecastmanager-0.1.5/forecastmanager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 09:55:17.000000 forecastmanager-0.1.5/forecastmanager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-07 09:55:17.000000 forecastmanager-0.1.5/forecastmanager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-07 09:55:17.000000 forecastmanager-0.1.5/forecastmanager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-07 09:54:55.000000 forecastmanager-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-08-07 09:55:17.089048 forecastmanager-0.1.5/setup.cfg
```

### Comparing `forecastmanager-0.1.4/PKG-INFO` & `forecastmanager-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forecastmanager
-Version: 0.1.4
+Version: 0.1.5
 Summary: Integration of Weather City Forecasts Manager in Wagtail Projects.
 Home-page: https://github.com/wmo-raf/forecastmanager
 Author: Grace Amondi
 Author-email: miswa.grace@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `forecastmanager-0.1.4/forecastmanager/blocks.py` & `forecastmanager-0.1.5/forecastmanager/blocks.py`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.4/forecastmanager/locale/am/LC_MESSAGES/django.mo` & `forecastmanager-0.1.5/forecastmanager/locale/am/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.4/forecastmanager/locale/am/LC_MESSAGES/django.po` & `forecastmanager-0.1.5/forecastmanager/locale/am/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.4/forecastmanager/locale/ar/LC_MESSAGES/django.mo` & `forecastmanager-0.1.5/forecastmanager/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.4/forecastmanager/locale/ar/LC_MESSAGES/django.po` & `forecastmanager-0.1.5/forecastmanager/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.4/forecastmanager/locale/en/LC_MESSAGES/django.mo` & `forecastmanager-0.1.5/forecastmanager/locale/en/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.4/forecastmanager/locale/en/LC_MESSAGES/django.po` & `forecastmanager-0.1.5/forecastmanager/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.4/forecastmanager/locale/es/LC_MESSAGES/django.mo` & `forecastmanager-0.1.5/forecastmanager/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.4/forecastmanager/locale/es/LC_MESSAGES/django.po` & `forecastmanager-0.1.5/forecastmanager/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.4/forecastmanager/locale/fr/LC_MESSAGES/django.mo` & `forecastmanager-0.1.5/forecastmanager/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.4/forecastmanager/locale/fr/LC_MESSAGES/django.po` & `forecastmanager-0.1.5/forecastmanager/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.4/forecastmanager/locale/sw/LC_MESSAGES/django.mo` & `forecastmanager-0.1.5/forecastmanager/locale/sw/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.4/forecastmanager/locale/sw/LC_MESSAGES/django.po` & `forecastmanager-0.1.5/forecastmanager/locale/sw/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.4/forecastmanager/management/commands/generate_forecast.py` & `forecastmanager-0.1.5/forecastmanager/management/commands/generate_forecast.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 import pandas as pd
 import numpy as np
 import requests
 
 from wagtailgeowidget.helpers import geosgeometry_str_to_struct
 from forecastmanager.models import City,Forecast
 from forecastmanager.site_settings import ForecastSetting,ForecastPeriod
-
+from forecastmanager.tasks import generate_forecasts
+from datetime import timedelta
 
 # Define the base URL for the Met Norway API
 BASE_URL = "https://api.met.no/weatherapi/locationforecast/2.0/complete"
 headers = {
   'User-Agent':'Mozilla/5.0 (Linux; Android 6.0; Nexus 5 Build/MRA58N) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Mobile Safari/537.36'
 }
 
@@ -24,14 +25,17 @@
 
 class Command(BaseCommand):
     help = ('autotranslate all the message files that have been generated '
             'using the `makemessages` command.')
 
     def handle(self, *args, **options):
 
+        # generate_forecasts(repeat=timedelta(hours=3).seconds, verbose_name="generate_forecasts")
+
+        # self.stdout.write(self.style.SUCCESS("Successfully submitted City Forecasts download task"))
         print("ATTEMPTING TO AUTOGENERATE 7 DAY FORECAST...")
            
         cities_ls = list(City.objects.all().values())
 
         forecast_setting = ForecastSetting.objects.all().first()
         parameters = forecast_setting.data_parameter_values
```

### Comparing `forecastmanager-0.1.4/forecastmanager/migrations/0001_initial.py` & `forecastmanager-0.1.5/forecastmanager/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.4/forecastmanager/migrations/0002_remove_forecast_max_temp_remove_forecast_min_temp_and_more.py` & `forecastmanager-0.1.5/forecastmanager/migrations/0002_remove_forecast_max_temp_remove_forecast_min_temp_and_more.py`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.4/forecastmanager/migrations/0004_forecastdataparameters_parameter_type_and_more.py` & `forecastmanager-0.1.5/forecastmanager/migrations/0004_forecastdataparameters_parameter_type_and_more.py`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.4/forecastmanager/migrations/0005_alter_forecastdataparameters_parameter.py` & `forecastmanager-0.1.5/forecastmanager/migrations/0005_alter_forecastdataparameters_parameter.py`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.4/forecastmanager/models.py` & `forecastmanager-0.1.5/forecastmanager/models.py`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.4/forecastmanager/serializers.py` & `forecastmanager-0.1.5/forecastmanager/serializers.py`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.4/forecastmanager/site_settings.py` & `forecastmanager-0.1.5/forecastmanager/site_settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from wagtail.contrib.settings.registry import register_setting
 from wagtail.models import Orderable
 
 
 @register_setting
 class ForecastSetting(ClusterableModel, BaseSiteSetting):
     enable_auto_forecast = models.BooleanField(
-        default=True,
+        default=False,
         verbose_name=_('Enable automated forecasts')
     )
 
     TEMPERATURE_UNITS = (
         ("celsius", "°C"),
         ("fareinheit", "°F"),
         ("kelvin", "K")
```

### Comparing `forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/clearsky.png` & `forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/clearsky.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/cloudy.png` & `forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/cloudy.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/fair.png` & `forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/fair.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/fog.png` & `forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/fog.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/heavyrain.png` & `forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/heavyrain.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/heavyrainandthunder.png` & `forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/heavyrainandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/heavyrainshowers.png` & `forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/heavyrainshowers.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/heavyrainshowersandthunder.png` & `forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/heavyrainshowersandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/heavysleet.png` & `forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/heavysleet.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/heavysleetandthunder.png` & `forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/heavysleetandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/heavysleetshowers.png` & `forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/heavysleetshowers.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/heavysleetshowersandthunder.png` & `forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/heavysleetshowersandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/heavysnow.png` & `forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/heavysnow.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/heavysnowandthunder.png` & `forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/heavysnowandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/heavysnowshowers.png` & `forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/heavysnowshowers.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/heavysnowshowersandthunder.png` & `forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/heavysnowshowersandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/lightrain.png` & `forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/lightrain.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/lightrainandthunder.png` & `forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/lightrainandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/lightrainshowers.png` & `forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/lightrainshowers.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/lightsleet.png` & `forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/lightsleet.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/lightsleetandthunder.png` & `forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/lightsleetandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/lightsleetshowers.png` & `forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/lightsleetshowers.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/lightsnow.png` & `forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/lightsnow.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/lightsnowandthunder.png` & `forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/lightsnowandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/lightsnowshowers.png` & `forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/lightsnowshowers.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/lightssleetshowersandthunder.png` & `forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/lightssleetshowersandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/lightssnowshowersandthunder.png` & `forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/lightssnowshowersandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/partlycloudy.png` & `forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/partlycloudy.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/rain.png` & `forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/rain.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/rainandthunder.png` & `forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/rainandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/rainshowers.png` & `forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/rainshowers.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/rainshowersandthunder.png` & `forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/rainshowersandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/sleet.png` & `forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/sleet.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/sleetandthunder.png` & `forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/sleetandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/sleetshowers.png` & `forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/sleetshowers.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/sleetshowersandthunder.png` & `forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/sleetshowersandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/snow.png` & `forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/snow.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/snowandthunder.png` & `forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/snowandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/snowshowers.png` & `forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/snowshowers.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.4/forecastmanager/static/forecastmanager/img/snowshowersandthunder.png` & `forecastmanager-0.1.5/forecastmanager/static/forecastmanager/img/snowshowersandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.4/forecastmanager/static/forecastmanager/js/forecast_basemap.js` & `forecastmanager-0.1.5/forecastmanager/static/forecastmanager/js/forecast_basemap.js`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.4/forecastmanager/static/forecastmanager/js/helpers.js` & `forecastmanager-0.1.5/forecastmanager/static/forecastmanager/js/helpers.js`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.4/forecastmanager/templates/forecastmanager/create_forecast.html` & `forecastmanager-0.1.5/forecastmanager/templates/forecastmanager/create_forecast.html`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.4/forecastmanager/templates/forecastmanager/forecast_base.html` & `forecastmanager-0.1.5/forecastmanager/templates/forecastmanager/forecast_base.html`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.4/forecastmanager/templates/forecastmanager/view_forecast.html` & `forecastmanager-0.1.5/forecastmanager/templates/forecastmanager/view_forecast.html`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.4/forecastmanager/views.py` & `forecastmanager-0.1.5/forecastmanager/views.py`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.4/forecastmanager/wagtail_hooks.py` & `forecastmanager-0.1.5/forecastmanager/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.4/forecastmanager.egg-info/PKG-INFO` & `forecastmanager-0.1.5/forecastmanager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forecastmanager
-Version: 0.1.4
+Version: 0.1.5
 Summary: Integration of Weather City Forecasts Manager in Wagtail Projects.
 Home-page: https://github.com/wmo-raf/forecastmanager
 Author: Grace Amondi
 Author-email: miswa.grace@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `forecastmanager-0.1.4/forecastmanager.egg-info/SOURCES.txt` & `forecastmanager-0.1.5/forecastmanager.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 forecastmanager/__init__.py
 forecastmanager/admin.py
 forecastmanager/apps.py
 forecastmanager/blocks.py
 forecastmanager/models.py
 forecastmanager/serializers.py
 forecastmanager/site_settings.py
+forecastmanager/tasks.py
 forecastmanager/tests.py
 forecastmanager/urls.py
 forecastmanager/views.py
 forecastmanager/wagtail_hooks.py
 forecastmanager.egg-info/PKG-INFO
 forecastmanager.egg-info/SOURCES.txt
 forecastmanager.egg-info/dependency_links.txt
@@ -34,14 +35,15 @@
 forecastmanager/management/commands/__init__.py
 forecastmanager/management/commands/generate_forecast.py
 forecastmanager/migrations/0001_initial.py
 forecastmanager/migrations/0002_remove_forecast_max_temp_remove_forecast_min_temp_and_more.py
 forecastmanager/migrations/0003_alter_forecast_unique_together.py
 forecastmanager/migrations/0004_forecastdataparameters_parameter_type_and_more.py
 forecastmanager/migrations/0005_alter_forecastdataparameters_parameter.py
+forecastmanager/migrations/0006_alter_forecastsetting_enable_auto_forecast.py
 forecastmanager/migrations/__init__.py
 forecastmanager/static/forecastmanager/img/clearsky.png
 forecastmanager/static/forecastmanager/img/cloudy.png
 forecastmanager/static/forecastmanager/img/fair.png
 forecastmanager/static/forecastmanager/img/fog.png
 forecastmanager/static/forecastmanager/img/heavyrain.png
 forecastmanager/static/forecastmanager/img/heavyrainandthunder.png
```

### Comparing `forecastmanager-0.1.4/setup.cfg` & `forecastmanager-0.1.5/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = forecastmanager
-version = 0.1.4
+version = 0.1.5
 description = Integration of Weather City Forecasts Manager in Wagtail Projects.
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/wmo-raf/forecastmanager
 author = Grace Amondi
 author_email = miswa.grace@gmail.com
 license = MIT
```

