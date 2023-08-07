# Comparing `tmp/fastapi-listing-0.0.8.tar.gz` & `tmp/fastapi-listing-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-listing-0.0.8.tar", last modified: Sat May 13 08:12:49 2023, max compression
+gzip compressed data, was "fastapi-listing-0.2.1.tar", last modified: Sat Jul 29 07:58:09 2023, max compression
```

## Comparing `fastapi-listing-0.0.8.tar` & `fastapi-listing-0.2.1.tar`

### file list

```diff
@@ -1,62 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 08:12:49.481732 fastapi-listing-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-13 08:12:39.000000 fastapi-listing-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21709 2023-05-13 08:12:49.481732 fastapi-listing-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20760 2023-05-13 08:12:39.000000 fastapi-listing-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 08:12:49.477732 fastapi-listing-0.0.8/fastapi_listing/
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-13 08:12:39.000000 fastapi-listing-0.0.8/fastapi_listing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 08:12:49.477732 fastapi-listing-0.0.8/fastapi_listing/abstracts/
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-13 08:12:39.000000 fastapi-listing-0.0.8/fastapi_listing/abstracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-13 08:12:39.000000 fastapi-listing-0.0.8/fastapi_listing/abstracts/base_query.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-13 08:12:39.000000 fastapi-listing-0.0.8/fastapi_listing/abstracts/dao.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-13 08:12:39.000000 fastapi-listing-0.0.8/fastapi_listing/abstracts/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-05-13 08:12:39.000000 fastapi-listing-0.0.8/fastapi_listing/abstracts/listing.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-13 08:12:39.000000 fastapi-listing-0.0.8/fastapi_listing/abstracts/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-13 08:12:39.000000 fastapi-listing-0.0.8/fastapi_listing/abstracts/sorter.py
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-13 08:12:39.000000 fastapi-listing-0.0.8/fastapi_listing/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 08:12:49.477732 fastapi-listing-0.0.8/fastapi_listing/dao/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-13 08:12:39.000000 fastapi-listing-0.0.8/fastapi_listing/dao/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-05-13 08:12:39.000000 fastapi-listing-0.0.8/fastapi_listing/dao/generic_dao.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-13 08:12:39.000000 fastapi-listing-0.0.8/fastapi_listing/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 08:12:49.477732 fastapi-listing-0.0.8/fastapi_listing/factory/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-13 08:12:39.000000 fastapi-listing-0.0.8/fastapi_listing/factory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-13 08:12:39.000000 fastapi-listing-0.0.8/fastapi_listing/factory/_generic_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-13 08:12:39.000000 fastapi-listing-0.0.8/fastapi_listing/factory/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-13 08:12:39.000000 fastapi-listing-0.0.8/fastapi_listing/factory/strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 08:12:49.477732 fastapi-listing-0.0.8/fastapi_listing/filters/
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-13 08:12:39.000000 fastapi-listing-0.0.8/fastapi_listing/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5274 2023-05-13 08:12:39.000000 fastapi-listing-0.0.8/fastapi_listing/filters/generic_filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 08:12:49.481732 fastapi-listing-0.0.8/fastapi_listing/interface/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 08:12:39.000000 fastapi-listing-0.0.8/fastapi_listing/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-13 08:12:39.000000 fastapi-listing-0.0.8/fastapi_listing/interface/listing_meta_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-13 08:12:39.000000 fastapi-listing-0.0.8/fastapi_listing/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 08:12:49.481732 fastapi-listing-0.0.8/fastapi_listing/mechanics/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-13 08:12:39.000000 fastapi-listing-0.0.8/fastapi_listing/mechanics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-13 08:12:39.000000 fastapi-listing-0.0.8/fastapi_listing/mechanics/iterative_filter_mechanics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-05-13 08:12:39.000000 fastapi-listing-0.0.8/fastapi_listing/mechanics/singleton_sorter_mechanics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 08:12:49.481732 fastapi-listing-0.0.8/fastapi_listing/paginator/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-13 08:12:39.000000 fastapi-listing-0.0.8/fastapi_listing/paginator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-13 08:12:39.000000 fastapi-listing-0.0.8/fastapi_listing/paginator/naive_page_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-13 08:12:39.000000 fastapi-listing-0.0.8/fastapi_listing/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 08:12:49.481732 fastapi-listing-0.0.8/fastapi_listing/service/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-13 08:12:39.000000 fastapi-listing-0.0.8/fastapi_listing/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14811 2023-05-13 08:12:39.000000 fastapi-listing-0.0.8/fastapi_listing/service/listing_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 08:12:49.481732 fastapi-listing-0.0.8/fastapi_listing/sorter/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-13 08:12:39.000000 fastapi-listing-0.0.8/fastapi_listing/sorter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-13 08:12:39.000000 fastapi-listing-0.0.8/fastapi_listing/sorter/naive_page_sorter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 08:12:49.481732 fastapi-listing-0.0.8/fastapi_listing/strategies/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-13 08:12:39.000000 fastapi-listing-0.0.8/fastapi_listing/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-05-13 08:12:39.000000 fastapi-listing-0.0.8/fastapi_listing/strategies/query_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-05-13 08:12:39.000000 fastapi-listing-0.0.8/fastapi_listing/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-13 08:12:39.000000 fastapi-listing-0.0.8/fastapi_listing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 08:12:49.477732 fastapi-listing-0.0.8/fastapi_listing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21709 2023-05-13 08:12:49.000000 fastapi-listing-0.0.8/fastapi_listing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-05-13 08:12:49.000000 fastapi-listing-0.0.8/fastapi_listing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 08:12:49.000000 fastapi-listing-0.0.8/fastapi_listing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-13 08:12:49.000000 fastapi-listing-0.0.8/fastapi_listing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-13 08:12:49.000000 fastapi-listing-0.0.8/fastapi_listing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-13 08:12:49.481732 fastapi-listing-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-05-13 08:12:39.000000 fastapi-listing-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 08:12:49.481732 fastapi-listing-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 08:12:39.000000 fastapi-listing-0.0.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-05-13 08:12:39.000000 fastapi-listing-0.0.8/tests/fake_listing_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-05-13 08:12:39.000000 fastapi-listing-0.0.8/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:58:09.639585 fastapi-listing-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-29 07:57:59.000000 fastapi-listing-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-07-29 07:58:09.639585 fastapi-listing-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-07-29 07:57:59.000000 fastapi-listing-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:58:09.631585 fastapi-listing-0.2.1/fastapi_listing/
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-29 07:57:59.000000 fastapi-listing-0.2.1/fastapi_listing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:58:09.635585 fastapi-listing-0.2.1/fastapi_listing/abstracts/
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-29 07:57:59.000000 fastapi-listing-0.2.1/fastapi_listing/abstracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-29 07:57:59.000000 fastapi-listing-0.2.1/fastapi_listing/abstracts/base_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-29 07:57:59.000000 fastapi-listing-0.2.1/fastapi_listing/abstracts/dao.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-29 07:57:59.000000 fastapi-listing-0.2.1/fastapi_listing/abstracts/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-29 07:57:59.000000 fastapi-listing-0.2.1/fastapi_listing/abstracts/interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-07-29 07:57:59.000000 fastapi-listing-0.2.1/fastapi_listing/abstracts/listing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-29 07:57:59.000000 fastapi-listing-0.2.1/fastapi_listing/abstracts/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-29 07:57:59.000000 fastapi-listing-0.2.1/fastapi_listing/abstracts/sorter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-29 07:57:59.000000 fastapi-listing-0.2.1/fastapi_listing/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-29 07:57:59.000000 fastapi-listing-0.2.1/fastapi_listing/ctyping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:58:09.635585 fastapi-listing-0.2.1/fastapi_listing/dao/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-29 07:57:59.000000 fastapi-listing-0.2.1/fastapi_listing/dao/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-07-29 07:57:59.000000 fastapi-listing-0.2.1/fastapi_listing/dao/dao_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-07-29 07:57:59.000000 fastapi-listing-0.2.1/fastapi_listing/dao/generic_dao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-29 07:57:59.000000 fastapi-listing-0.2.1/fastapi_listing/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:58:09.635585 fastapi-listing-0.2.1/fastapi_listing/factory/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-29 07:57:59.000000 fastapi-listing-0.2.1/fastapi_listing/factory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-07-29 07:57:59.000000 fastapi-listing-0.2.1/fastapi_listing/factory/_generic_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-07-29 07:57:59.000000 fastapi-listing-0.2.1/fastapi_listing/factory/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-29 07:57:59.000000 fastapi-listing-0.2.1/fastapi_listing/factory/interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-29 07:57:59.000000 fastapi-listing-0.2.1/fastapi_listing/factory/strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:58:09.635585 fastapi-listing-0.2.1/fastapi_listing/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-29 07:57:59.000000 fastapi-listing-0.2.1/fastapi_listing/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-07-29 07:57:59.000000 fastapi-listing-0.2.1/fastapi_listing/filters/generic_filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:58:09.639585 fastapi-listing-0.2.1/fastapi_listing/interceptors/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-29 07:57:59.000000 fastapi-listing-0.2.1/fastapi_listing/interceptors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-07-29 07:57:59.000000 fastapi-listing-0.2.1/fastapi_listing/interceptors/individual_sorter_interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-29 07:57:59.000000 fastapi-listing-0.2.1/fastapi_listing/interceptors/iterative_filter_interceptor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:58:09.639585 fastapi-listing-0.2.1/fastapi_listing/interface/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 07:57:59.000000 fastapi-listing-0.2.1/fastapi_listing/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-29 07:57:59.000000 fastapi-listing-0.2.1/fastapi_listing/interface/client_site_params_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-07-29 07:57:59.000000 fastapi-listing-0.2.1/fastapi_listing/interface/listing_meta_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3745 2023-07-29 07:57:59.000000 fastapi-listing-0.2.1/fastapi_listing/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-07-29 07:57:59.000000 fastapi-listing-0.2.1/fastapi_listing/middlewares.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:58:09.639585 fastapi-listing-0.2.1/fastapi_listing/paginator/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-29 07:57:59.000000 fastapi-listing-0.2.1/fastapi_listing/paginator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-07-29 07:57:59.000000 fastapi-listing-0.2.1/fastapi_listing/paginator/page_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-29 07:57:59.000000 fastapi-listing-0.2.1/fastapi_listing/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:58:09.639585 fastapi-listing-0.2.1/fastapi_listing/service/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-29 07:57:59.000000 fastapi-listing-0.2.1/fastapi_listing/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-07-29 07:57:59.000000 fastapi-listing-0.2.1/fastapi_listing/service/_core_listing_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-29 07:57:59.000000 fastapi-listing-0.2.1/fastapi_listing/service/adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-07-29 07:58:00.000000 fastapi-listing-0.2.1/fastapi_listing/service/listing_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:58:09.639585 fastapi-listing-0.2.1/fastapi_listing/sorter/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-29 07:58:00.000000 fastapi-listing-0.2.1/fastapi_listing/sorter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-29 07:58:00.000000 fastapi-listing-0.2.1/fastapi_listing/sorter/page_sorter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:58:09.639585 fastapi-listing-0.2.1/fastapi_listing/strategies/
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-29 07:58:00.000000 fastapi-listing-0.2.1/fastapi_listing/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-07-29 07:58:00.000000 fastapi-listing-0.2.1/fastapi_listing/strategies/query_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-29 07:58:00.000000 fastapi-listing-0.2.1/fastapi_listing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:58:09.635585 fastapi-listing-0.2.1/fastapi_listing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-07-29 07:58:09.000000 fastapi-listing-0.2.1/fastapi_listing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-07-29 07:58:09.000000 fastapi-listing-0.2.1/fastapi_listing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 07:58:09.000000 fastapi-listing-0.2.1/fastapi_listing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-29 07:58:09.000000 fastapi-listing-0.2.1/fastapi_listing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-29 07:58:09.000000 fastapi-listing-0.2.1/fastapi_listing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 07:58:09.639585 fastapi-listing-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-07-29 07:58:00.000000 fastapi-listing-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:58:09.639585 fastapi-listing-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 07:58:00.000000 fastapi-listing-0.2.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-07-29 07:58:00.000000 fastapi-listing-0.2.1/tests/dao_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8267 2023-07-29 07:58:00.000000 fastapi-listing-0.2.1/tests/fake_listing_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7561 2023-07-29 07:58:00.000000 fastapi-listing-0.2.1/tests/original_responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-07-29 07:58:00.000000 fastapi-listing-0.2.1/tests/pydantic_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-07-29 07:58:00.000000 fastapi-listing-0.2.1/tests/service_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-07-29 07:58:00.000000 fastapi-listing-0.2.1/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18692 2023-07-29 07:58:00.000000 fastapi-listing-0.2.1/tests/test_main_v2.py
```

### Comparing `fastapi-listing-0.0.8/LICENSE` & `fastapi-listing-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi-listing-0.0.8/fastapi_listing/abstracts/dao.py` & `fastapi-listing-0.2.1/fastapi_listing/abstracts/dao.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 from abc import ABCMeta, abstractmethod
 from typing import Union, Dict, List
-from fastapi_listing.typing import SqlAlchemyModel
+from fastapi_listing.ctyping import SqlAlchemyModel
 
 
 class DaoAbstract(metaclass=ABCMeta):
 
     @property
     @abstractmethod
     def model(self):
         pass
 
+    @property
+    @abstractmethod
+    def name(self):
+        pass
+
     @abstractmethod
     def create(self, values: Dict[str, Union[str, int]]) -> SqlAlchemyModel:
         pass
 
     @abstractmethod
     def update(self, identifier: Dict[str, Union[str, int, list]], values: dict) -> bool:
         pass
```

### Comparing `fastapi-listing-0.0.8/fastapi_listing/dao/generic_dao.py` & `fastapi-listing-0.2.1/fastapi_listing/dao/generic_dao.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from fastapi_listing.abstracts import DaoAbstract
 from sqlalchemy.orm import Session
 from typing import Union, Dict, List
 
-from fastapi_listing.typing import SqlAlchemyModel
+from fastapi_listing.ctyping import SqlAlchemyModel
 
 
 class GenericDao(DaoAbstract):  # type:ignore # noqa
     """
     Dao stands for data access object.
     This layers encapsulates all logic that a user may write
     in order to interact with databases.
@@ -28,14 +28,15 @@
     but one dao object can talk to multiple models with having first primary model.
 
     Note - no data validation should happen at this layer. That should be prior to pushing
     at this layer.
     """
 
     # model: SqlAlchemyModel = None to be defined at model dao level
+    # name: str = "DaoName"
 
     def __init__(self, read_db=None, write_db=None):
         # considering that we are dealing with separate read and write dbs.
         # we must have two sessions one for read replica and one for master or write replica
         # we should define our reusable attributes here that we will use in each dao method definition
         # even if we are using single db still having two references for the same session won't hurt
         # for future expansion once we decide to move on to read/write replica architecure
@@ -80,9 +81,9 @@
     def read(self, identifier: Dict[str, Union[str, int, list]],
              fields: Union[list, str] = "__all__") -> SqlAlchemyModel:
         raise NotImplementedError
 
     def delete(self, ids: List[int]) -> bool:
         raise NotImplementedError
 
-    def get_naive_read(self, fields_to_read: list):
+    def get_default_read(self, fields_to_read: list):
         return self._read_db.query(*fields_to_read)
```

### Comparing `fastapi-listing-0.0.8/fastapi_listing/factory/strategy.py` & `fastapi-listing-0.2.1/fastapi_listing/factory/strategy.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,20 +4,23 @@
     def __init__(self):
         self._strategy = {}
 
     def register_strategy(self, key: str, builder: type):
         if key is None or not key:
             raise ValueError(f"Invalid type key!")
         if key in self._strategy:
-            raise ValueError(f"strategy name already in use with {self._strategy[key].__name__}!")
+            raise ValueError(f"strategy name: {key}, already in use with {self._strategy[key].__name__}!")
         if not isinstance(builder, object):
             raise ValueError(f"builder is not a valid callable!")
         self._strategy[key] = builder
 
     def create(self, key: str, *args, **kwargs) -> object:
         strategy_ = self._strategy.get(key)
         if not strategy_:
             raise ValueError(key)
         return strategy_(*args, **kwargs)
 
+    def aware_of(self, key: str) -> bool:
+        return key in self._strategy
+
 
 strategy_factory = StrategyObjectFactory()
```

### Comparing `fastapi-listing-0.0.8/fastapi_listing/filters/__init__.py` & `fastapi-listing-0.2.1/fastapi_listing/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi-listing-0.0.8/fastapi_listing/filters/generic_filters.py` & `fastapi-listing-0.2.1/fastapi_listing/filters/generic_filters.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,29 @@
+from typing import Callable
 from datetime import datetime
 
 from fastapi_listing.abstracts import FilterAbstract
-from fastapi_listing.typing import SqlAlchemyQuery, AnySqlAlchemyColumn
+from fastapi_listing.ctyping import SqlAlchemyQuery, AnySqlAlchemyColumn
 
 
 class CommonFilterImpl(FilterAbstract):
 
-    def __init__(self, dao=None, request=None, extra_context=None):
+    def __init__(self, dao=None, request=None, *, extra_context=None,
+                 field_extract_fn: Callable[[str], AnySqlAlchemyColumn] = None):
+        # lambda x: getattr(Model, x)
         self.dao = dao
         self.request = request
         self.extra_context = extra_context
+        self.custom_field_extractor = field_extract_fn
 
     def extract_field(self, field: str) -> AnySqlAlchemyColumn:
-        return getattr(self.dao.model, field.split(".")[-1])
+        field = field.split(".")[-1]
+        if self.custom_field_extractor:
+            return self.custom_field_extractor(field)
+        return getattr(self.dao.model, field)
 
     def filter(self, *, field: str = None, value: dict = None, query=None) -> SqlAlchemyQuery:
         raise NotImplementedError("To be implemented in child class!")
 
 
 class EqualityFilter(CommonFilterImpl):
 
@@ -148,7 +155,16 @@
     def filter(self, *, field: str = None, value: dict = None, query=None) -> SqlAlchemyQuery:
         inst_field = self.extract_field(field)
         if value.get("search"):
             query = query.filter(inst_field.is_not(None))
         else:
             query = query.filter(inst_field.is_(None))
         return query
+
+
+class MySqlNativeDateFormateRangeFilter(CommonFilterImpl):
+
+    def filter(self, *, field: str = None, value: dict = None, query=None) -> SqlAlchemyQuery:
+        inst_field = self.extract_field(field)
+        if value:
+            query = query.filter(inst_field.between(value.get("start"), value.get("end")))
+        return query
```

### Comparing `fastapi-listing-0.0.8/fastapi_listing/sorter/naive_page_sorter.py` & `fastapi-listing-0.2.1/fastapi_listing/sorter/page_sorter.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,16 @@
-from typing import Dict
-from fastapi_listing.abstracts import TableDataSortingStrategy
-from fastapi_listing.typing import SqlAlchemyModel, FastapiRequest, SqlAlchemyQuery, AnySqlAlchemyColumn
+from typing import Dict, Callable
+from fastapi_listing.abstracts import AbsSortingStrategy
+from fastapi_listing.ctyping import SqlAlchemyModel, FastapiRequest, SqlAlchemyQuery, AnySqlAlchemyColumn
+from fastapi_listing.factory import _generic_factory
 
 
-class SortingOrderStrategy(TableDataSortingStrategy):
+class SortingOrderStrategy(AbsSortingStrategy):
+
+    name = "default_sorter"
 
     def __init__(self, model: SqlAlchemyModel = None, request: FastapiRequest = None):
         self.model = model
         self.request = request
 
     @staticmethod
     def sort_asc_util(query: SqlAlchemyQuery, inst_field: AnySqlAlchemyColumn) -> SqlAlchemyQuery:
@@ -17,27 +20,28 @@
     @staticmethod
     def sort_dsc_util(query: SqlAlchemyQuery, inst_field: AnySqlAlchemyColumn) -> SqlAlchemyQuery:
         query = query.order_by(inst_field.desc())
         return query
 
     def sort(self, *, query: SqlAlchemyQuery = None, value: Dict[str, str] = None,
              extra_context: dict = None) -> SqlAlchemyQuery:
-        if value is None:
-            raise ValueError("sort expects value with structure [type, field], none provided")
         assert value["type"] in ["asc", "dsc"], "invalid sorting style!"
         inst_field: AnySqlAlchemyColumn = self.validate_srt_field(self.model, value["field"])
         if value["type"] == "asc":
             query = self.sort_asc_util(query, inst_field)
         else:
             query = self.sort_dsc_util(query, inst_field)
         return query
 
-    @staticmethod
-    def validate_srt_field(model: SqlAlchemyModel, sort_field: str):
-        try:
-            inst_field = getattr(model, sort_field)
-        except AttributeError:
-            inst_field = None
-        if inst_field is None:
-            raise ValueError(
-                f"Provided sort field is not an attribute of {model}")  # todo improve this by custom exception
+    def validate_srt_field(self, model: SqlAlchemyModel, sort_field: str):
+        field = sort_field.split(".")[-1]
+        if sort_field in _generic_factory.object_creation_collector:
+            inst_field = _generic_factory.create(sort_field, field)
+        else:
+            try:
+                inst_field = getattr(model, field)
+            except AttributeError:
+                inst_field = None
+            if inst_field is None:
+                raise ValueError(
+                    f"Provided sort field is not an attribute of {model.__name__}")  # todo improve this by custom exception
         return inst_field
```

### Comparing `fastapi-listing-0.0.8/fastapi_listing/strategies/__init__.py` & `fastapi-listing-0.2.1/fastapi_listing/strategies/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from fastapi_listing.strategies.query_strategy import NaiveQueryStrategy
-from fastapi_listing.paginator import NaivePaginationStrategy
+from fastapi_listing.strategies.query_strategy import QueryStrategy
+from fastapi_listing.paginator import PaginationStrategy
 from fastapi_listing.sorter import SortingOrderStrategy
 
 
 class ModuleInterface:
     """
     Represents a strategy interface. A strategy should have a constant NAME
     This module must be registered by strategy factory
```

### Comparing `fastapi-listing-0.0.8/fastapi_listing/strategies/query_strategy.py` & `fastapi-listing-0.2.1/fastapi_listing/strategies/query_strategy.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-from fastapi_listing.abstracts import QueryStrategy
+from fastapi_listing.abstracts import AbsQueryStrategy
 from fastapi_listing.dao import GenericDao
-from fastapi_listing.typing import SqlAlchemyQuery, FastapiRequest
+from fastapi_listing.ctyping import SqlAlchemyQuery, FastapiRequest
 
 
-class NaiveQueryStrategy(QueryStrategy):
+class QueryStrategy(AbsQueryStrategy):
+
+    name = "default_query"
 
     def get_inst_attr_to_read(self, custom_fields: bool, field_list: list, dao: GenericDao):
         inst_fields = []
 
         if custom_fields:
             # ("BYPASS CUSTOM PYDANTIC FIELDS ALLOWED.")
             # when serializer contains fields that get filled via validators or at runtime
@@ -21,9 +23,10 @@
             inst_fields = [getattr(dao.model, field) for field in field_list]
         return inst_fields
 
     def get_query(self, *, request: FastapiRequest = None, dao: GenericDao = None,
                   extra_context: dict = None) -> SqlAlchemyQuery:
         inst_fields = self.get_inst_attr_to_read(extra_context.get("custom_fields"), extra_context.get("field_list"),
                                                  dao)
-        query = dao.get_naive_read(inst_fields)
+        query = dao.get_default_read(inst_fields)
+        print(query.statement)
         return query
```

### Comparing `fastapi-listing-0.0.8/fastapi_listing/typing.py` & `fastapi-listing-0.2.1/fastapi_listing/ctyping.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,20 +14,21 @@
     DeclarativeMeta = None
     Query = None
     Session = None
     Column = None
 
 
 class ListingResponseType(TypedDict):
-    data: List[Dict[str, Union[int, str, list, dict]]]
-    currentPageNumber: int
-    currentPageSize: int
-    totalCount: int
     hasNext: bool
+    totalCount: int
+    currentPageSize: int
+    currentPageNumber: int
+    data: List[Dict[str, Union[int, str, list, dict]]]
 
 
 SqlAlchemyQuery = TypeVar("SqlAlchemyQuery", bound=Query)
 SqlAlchemySession = TypeVar("SqlAlchemySession", bound=Session)
 FastapiRequest = TypeVar("FastapiRequest", bound=Request)
 AnySqlAlchemyColumn = TypeVar("AnySqlAlchemyColumn", bound=Column)
 SqlAlchemyModel = TypeVar("SqlAlchemyModel", bound=DeclarativeMeta)
 
+
```

### Comparing `fastapi-listing-0.0.8/fastapi_listing.egg-info/SOURCES.txt` & `fastapi-listing-0.2.1/fastapi_listing.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,46 +1,58 @@
 LICENSE
 README.md
 setup.py
 fastapi_listing/__init__.py
 fastapi_listing/constants.py
+fastapi_listing/ctyping.py
 fastapi_listing/errors.py
 fastapi_listing/loader.py
+fastapi_listing/middlewares.py
 fastapi_listing/py.typed
-fastapi_listing/typing.py
 fastapi_listing/utils.py
 fastapi_listing.egg-info/PKG-INFO
 fastapi_listing.egg-info/SOURCES.txt
 fastapi_listing.egg-info/dependency_links.txt
 fastapi_listing.egg-info/requires.txt
 fastapi_listing.egg-info/top_level.txt
 fastapi_listing/abstracts/__init__.py
 fastapi_listing/abstracts/base_query.py
 fastapi_listing/abstracts/dao.py
 fastapi_listing/abstracts/filter.py
+fastapi_listing/abstracts/interceptor.py
 fastapi_listing/abstracts/listing.py
 fastapi_listing/abstracts/paginator.py
 fastapi_listing/abstracts/sorter.py
 fastapi_listing/dao/__init__.py
+fastapi_listing/dao/dao_registry.py
 fastapi_listing/dao/generic_dao.py
 fastapi_listing/factory/__init__.py
 fastapi_listing/factory/_generic_factory.py
 fastapi_listing/factory/filter.py
+fastapi_listing/factory/interceptor.py
 fastapi_listing/factory/strategy.py
 fastapi_listing/filters/__init__.py
 fastapi_listing/filters/generic_filters.py
+fastapi_listing/interceptors/__init__.py
+fastapi_listing/interceptors/individual_sorter_interceptor.py
+fastapi_listing/interceptors/iterative_filter_interceptor.py
 fastapi_listing/interface/__init__.py
+fastapi_listing/interface/client_site_params_adapter.py
 fastapi_listing/interface/listing_meta_info.py
-fastapi_listing/mechanics/__init__.py
-fastapi_listing/mechanics/iterative_filter_mechanics.py
-fastapi_listing/mechanics/singleton_sorter_mechanics.py
 fastapi_listing/paginator/__init__.py
-fastapi_listing/paginator/naive_page_builder.py
+fastapi_listing/paginator/page_builder.py
 fastapi_listing/service/__init__.py
+fastapi_listing/service/_core_listing_service.py
+fastapi_listing/service/adapters.py
 fastapi_listing/service/listing_main.py
 fastapi_listing/sorter/__init__.py
-fastapi_listing/sorter/naive_page_sorter.py
+fastapi_listing/sorter/page_sorter.py
 fastapi_listing/strategies/__init__.py
 fastapi_listing/strategies/query_strategy.py
 tests/__init__.py
+tests/dao_setup.py
 tests/fake_listing_setup.py
-tests/test_main.py
+tests/original_responses.py
+tests/pydantic_setup.py
+tests/service_setup.py
+tests/test_main.py
+tests/test_main_v2.py
```

### Comparing `fastapi-listing-0.0.8/setup.py` & `fastapi-listing-0.2.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,19 +49,21 @@
         "test": [
             "requests",
             "pytest>=6.2.4",
             "mypy>=0.971",
             "pytest-env>=0.6.2",
             "flake8>=3.9.2",
             "isort>=5.10.1",
-            "pydantic>=1.5.0",
+            "pydantic==1.10.7",
             "starlette>=0.21.0",
             "sqlalchemy>=2.0.7",
             "starlite>=1.38.0",
             "httpx>=0.23.0",
             "pytest-mock>=3.6.1",
             "fastapi>=0.92.0",
             "mypy>=0.971",
             "pytest-mypy>=0.9.1",
+            "mysqlclient",
+            "pytest-cov==4.1.0"
         ],
     },
 )
```

### Comparing `fastapi-listing-0.0.8/tests/fake_listing_setup.py` & `fastapi-listing-0.2.1/tests/fake_listing_setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,284 +1,249 @@
 from typing import Optional
 from fastapi_listing import FastapiListing, ListingService
-from fastapi_listing.strategies import NaiveQueryStrategy, NaivePaginationStrategy, SortingOrderStrategy
+from fastapi_listing.strategies import QueryStrategy, PaginationStrategy, SortingOrderStrategy
 from fastapi_listing.factory import strategy_factory, filter_factory
 from fastapi_listing.filters import generic_filters
 from fastapi_listing.dao import GenericDao
 from pydantic import BaseModel, Field, root_validator
 from fastapi_listing import utils
 from sqlalchemy.orm import declarative_base
 from sqlalchemy import Column, String, Integer
 from sqlalchemy.dialects.mysql import BIT
 from typing import List, Dict
+from tests import dao_setup
 
 Base = declarative_base()
 
-fake_db = [
-    {
-        "id": 1,
-        "product_name": "Hyundai Verna",
-        "is_active": 1
-    },
-    {
-        "id": 2,
-        "product_name": "Hyundai Centro",
-        "is_active": 0
-    },
-]
-
-fake_resp_aliased = [
-    {
-        "id": 1,
-        "pn": "Hyundai Verna",
-        "ia": 1
-    },
-    {
-        "id": 2,
-        "pn": "Hyundai Centro",
-        "ia": 0
-    }
-]
-
-fake_custom_column_resp_aliased = [
-    {
-        "id": 1,
-        "pn": "Hyundai Verna",
-        "ia": 1,
-        "cd": "1-HV"
-    },
-    {
-        "id": 2,
-        "pn": "Hyundai Centro",
-        "ia": 0,
-        "cd": "2-HC"
-    }
-]
-
-fake_resp_aliased_size_1 = [
-    {
-        "id": 1,
-        "pn": "Hyundai Verna",
-        "ia": 1
-    },
-]
-fake_db_query1 = "select * from fake_db"
-
-fake_db_response = {
-    "data": fake_resp_aliased,
-    "totalCount": len(fake_db),
-    "currentPageSize": 10,
-    "currentPageNumber": 0,
-    "hasNext": False
-}
-
-fake_db_response_with_custom_column = {
-    "data": fake_custom_column_resp_aliased,
-    "totalCount": len(fake_db),
-    "currentPageSize": 10,
-    "currentPageNumber": 0,
-    "hasNext": False
-}
-
-fake_db_response_page_size_1 = {
-    "data": fake_resp_aliased_size_1,
-    "totalCount": len(fake_resp_aliased_size_1),
-    "currentPageSize": 1,
-    "currentPageNumber": 0,
-    "hasNext": False
-}
-
-
-class ProductDetail(BaseModel):
-    id: int
-    product_name: str = Field(alias="pn")
-    is_active: bool = Field(alias="ia")
-
-    class Config:
-        allow_population_by_field_name = True
-
-
-class ProductPage(BaseModel):
-    data: List[ProductDetail] = []
-    currentPageSize: int
-    currentPageNumber: int
-    hasNext: bool
-    totalCount: int
-
-    class Config:
-        orm_mode = True
-        allow_population_by_field_name = True
-
-
-class ProductDetailWithCustomFields(BaseModel):
-    id: int
-    product_name: str = Field(alias="pn")
-    is_active: bool = Field(alias="ia")
-    code: Optional[str] = Field(alias="cd")
-
-    @root_validator
-    def generate_product_code(cls, values):
-        pnm = values["product_name"]
-        pnm = pnm.split()
-        cd = []
-        for nm in pnm:
-            cd.append(nm[:1])
-        values["code"] = f"{values['id']}-{''.join(cd)}"
-        return values
-
-    class Config:
-        allow_population_by_field_name = True
-
-
-class ProductPageWithCustomColumns(BaseModel):
-    data: List[ProductDetailWithCustomFields] = []
-    currentPageSize: int
-    currentPageNumber: int
-    hasNext: bool
-    totalCount: int
-
-    class Config:
-        orm_mode = True
-        allow_population_by_field_name = True
-
-
-class Product(Base):
-    __tablename__ = 'fake_product'
-    id = Column(Integer, primary_key=True)
-    product_name = Column(String(500, 'utf8mb4_unicode_520_ci'), index=True)
-    is_active = Column(BIT(1), nullable=False, index=True)
-
-
-class FakeProductDao(GenericDao):  # noqa
-    model = Product
-
-
-class FakeQueryStrategyV1(NaiveQueryStrategy):
-
-    def get_query(self, *, request=None, dao=None,
-                  extra_context: dict = None):
-
-        assert dao.model == Product
-        assert isinstance(dao, FakeProductDao) == True
-        if not extra_context.get("custom_fields"):
-            assert extra_context.get("field_list") == list(ProductDetail.__fields__.keys())
-            assert [Product.id, Product.product_name, Product.is_active] == \
-                   self.get_inst_attr_to_read(custom_fields=False, field_list=extra_context.get("field_list"), dao=dao)
-        else:
-            assert [Product.id, Product.product_name, Product.is_active] == \
-                   self.get_inst_attr_to_read(custom_fields=True, field_list=extra_context.get("field_list"), dao=dao)
-        return fake_db_query1
-
-
-class FakeSortingStrategy(SortingOrderStrategy):
-
-    def sort(self, *, query=None, value: Dict[str, str] = None,
-             extra_context: dict = None):
-        assert value["type"] in ["asc", "dsc"]
-        assert query == fake_db_query1
-        return query
+# fake_db = [
+#     {
+#         "id": 1,
+#         "product_name": "Hyundai Verna",
+#         "is_active": 1
+#     },
+#     {
+#         "id": 2,
+#         "product_name": "Hyundai Centro",
+#         "is_active": 0
+#     },
+# ]
+#
+# fake_resp_aliased = [
+#     {
+#         "id": 1,
+#         "pn": "Hyundai Verna",
+#         "ia": 1
+#     },
+#     {
+#         "id": 2,
+#         "pn": "Hyundai Centro",
+#         "ia": 0
+#     }
+# ]
+#
+# fake_custom_column_resp_aliased = [
+#     {
+#         "id": 1,
+#         "pn": "Hyundai Verna",
+#         "ia": 1,
+#         "cd": "1-HV"
+#     },
+#     {
+#         "id": 2,
+#         "pn": "Hyundai Centro",
+#         "ia": 0,
+#         "cd": "2-HC"
+#     }
+# ]
+#
+# fake_resp_aliased_size_1 = [
+#     {
+#         "id": 1,
+#         "pn": "Hyundai Verna",
+#         "ia": 1
+#     },
+# ]
+# fake_db_query1 = "select * from fake_db"
+#
+# fake_db_response = {
+#     "data": fake_resp_aliased,
+#     "totalCount": len(fake_db),
+#     "currentPageSize": 10,
+#     "currentPageNumber": 0,
+#     "hasNext": False
+# }
+#
+# fake_db_response_with_custom_column = {
+#     "data": fake_custom_column_resp_aliased,
+#     "totalCount": len(fake_db),
+#     "currentPageSize": 10,
+#     "currentPageNumber": 0,
+#     "hasNext": False
+# }
+#
+# fake_db_response_page_size_1 = {
+#     "data": fake_resp_aliased_size_1,
+#     "totalCount": len(fake_resp_aliased_size_1),
+#     "currentPageSize": 1,
+#     "currentPageNumber": 0,
+#     "hasNext": False
+# }
+#
+#
+# class ProductDetail(BaseModel):
+#     id: int
+#     product_name: str = Field(alias="pn")
+#     is_active: bool = Field(alias="ia")
+#
+#     class Config:
+#         allow_population_by_field_name = True
+#
+#
+# class ProductPage(BaseModel):
+#     data: List[ProductDetail] = []
+#     currentPageSize: int
+#     currentPageNumber: int
+#     hasNext: bool
+#     totalCount: int
+#
+#     class Config:
+#         orm_mode = True
+#         allow_population_by_field_name = True
+#
+#
+# class ProductDetailWithCustomFields(BaseModel):
+#     id: int
+#     product_name: str = Field(alias="pn")
+#     is_active: bool = Field(alias="ia")
+#     code: Optional[str] = Field(alias="cd")
+#
+#     @root_validator
+#     def generate_product_code(cls, values):
+#         pnm = values["product_name"]
+#         pnm = pnm.split()
+#         cd = []
+#         for nm in pnm:
+#             cd.append(nm[:1])
+#         values["code"] = f"{values['id']}-{''.join(cd)}"
+#         return values
+#
+#     class Config:
+#         allow_population_by_field_name = True
+#
+#
+# class ProductPageWithCustomColumns(BaseModel):
+#     data: List[ProductDetailWithCustomFields] = []
+#     currentPageSize: int
+#     currentPageNumber: int
+#     hasNext: bool
+#     totalCount: int
+#
+#     class Config:
+#         orm_mode = True
+#         allow_population_by_field_name = True
+#
+#
+# class Product(Base):
+#     __tablename__ = 'fake_product'
+#     id = Column(Integer, primary_key=True)
+#     product_name = Column(String(500, 'utf8mb4_unicode_520_ci'), index=True)
+#     is_active = Column(BIT(1), nullable=False, index=True)
+#
+#
+# class FakeProductDao(GenericDao):  # noqa
+#     model = Product
+#
+#
+# class FakeQueryStrategyV1(QueryStrategy):
+#
+#     def get_query(self, *, request=None, dao=None,
+#                   extra_context: dict = None):
+#
+#         assert dao.model == Product
+#         assert isinstance(dao, FakeProductDao) == True
+#         if not extra_context.get("custom_fields"):
+#             assert extra_context.get("field_list") == list(ProductDetail.__fields__.keys())
+#             assert [Product.id, Product.product_name, Product.is_active] == \
+#                    self.get_inst_attr_to_read(custom_fields=False, field_list=extra_context.get("field_list"), dao=dao)
+#         else:
+#             assert [Product.id, Product.product_name, Product.is_active] == \
+#                    self.get_inst_attr_to_read(custom_fields=True, field_list=extra_context.get("field_list"), dao=dao)
+#         return fake_db_query1
+#
+#
+# class FakeSortingStrategy(SortingOrderStrategy):
+#
+#     def sort(self, *, query=None, value: Dict[str, str] = None,
+#              extra_context: dict = None):
+#         assert value["type"] in ["asc", "dsc"]
+#         assert query == fake_db_query1
+#         return query
+#
+#
+# class FakePaginationStrategyV1(PaginationStrategy):
+#
+#     def paginate(self, query, request, extra_context: dict):
+#         pagination_params = utils.dictify_query_params(request.query_params.get("pagination"))
+#         assert pagination_params == self.default_pagination_params
+#         assert query == fake_db_query1
+#         return {
+#             "data": fake_db,
+#             "totalCount": len(fake_db),
+#             "currentPageSize": pagination_params.get("pageSize"),
+#             "currentPageNumber": pagination_params.get("page"),
+#             "hasNext": False
+#         }
+#
+#
+# strategy_factory.register_strategy("fake_query_strategy", FakeQueryStrategyV1)
+# strategy_factory.register_strategy("fake_sorting_strategy", FakeSortingStrategy)
+# strategy_factory.register_strategy("fake_paginator_strategy", FakePaginationStrategyV1)
+#
+#
+# class TestListingServiceDefaultFlow(ListingService):
+#     default_srt_on = "id"
+#     dao_kls = FakeProductDao
+#     query_strategy = "fake_query_strategy"
+#     sorting_strategy = "fake_sorting_strategy"
+#     paginate_strategy = "fake_paginator_strategy"
+#
+#     def get_listing(self):
+#         return FastapiListing(self.request, self.dao, ProductDetail).get_response(self.MetaInfo(self))
+#
+#
+# class TestListingServiceDefaultFlowWithCustomColumns(ListingService):
+#     default_srt_on = "id"
+#     dao_kls = FakeProductDao
+#     query_strategy = "fake_query_strategy"
+#     sorting_strategy = "fake_sorting_strategy"
+#     paginate_strategy = "fake_paginator_strategy"
+#
+#     def get_listing(self):
+#         return FastapiListing(self.request, self.dao, ProductDetailWithCustomFields, custom_fields=True).get_response(self.MetaInfo(self))
 
 
-class FakePaginationStrategyV1(NaivePaginationStrategy):
+class FakePaginationStrategyV2(PaginationStrategy):
 
     def paginate(self, query, request, extra_context: dict):
-        pagination_params = utils.jsonify_query_params(request.query_params.get("pagination"))
-        assert pagination_params == self.default_pagination_params
-        assert query == fake_db_query1
-        return {
-            "data": fake_db,
-            "totalCount": len(fake_db),
-            "currentPageSize": pagination_params.get("pageSize"),
-            "currentPageNumber": pagination_params.get("page"),
-            "hasNext": False
-        }
-
-
-strategy_factory.register_strategy("fake_query_strategy", FakeQueryStrategyV1)
-strategy_factory.register_strategy("fake_sorting_strategy", FakeSortingStrategy)
-strategy_factory.register_strategy("fake_paginator_strategy", FakePaginationStrategyV1)
-
-
-class TestListingServiceDefaultFlow(ListingService):
-    DEFAULT_SRT_ON = "id"
-    dao_kls = FakeProductDao
-    QUERY_STRATEGY = "fake_query_strategy"
-    SORTING_STRATEGY = "fake_sorting_strategy"
-    PAGINATE_STRATEGY = "fake_paginator_strategy"
-
-    def get_listing(self):
-        return FastapiListing(self.request, self.dao, ProductDetail).get_response(self.MetaInfo(self))
-
-
-class TestListingServiceDefaultFlowWithCustomColumns(ListingService):
-    DEFAULT_SRT_ON = "id"
-    dao_kls = FakeProductDao
-    QUERY_STRATEGY = "fake_query_strategy"
-    SORTING_STRATEGY = "fake_sorting_strategy"
-    PAGINATE_STRATEGY = "fake_paginator_strategy"
-
-    def get_listing(self):
-        return FastapiListing(self.request, self.dao, ProductDetailWithCustomFields, custom_fields=True).get_response(self.MetaInfo(self))
-
-
-class FakePaginationStrategyV2(NaivePaginationStrategy):
-
-    def paginate(self, query, request, extra_context: dict):
-        pagination_params = utils.jsonify_query_params(request.query_params.get("pagination"))
-        assert pagination_params == {"pageSize": 1, "page": 0}
-        assert query == fake_db_query1
-        return {
-            "data": fake_db[:1],
-            "totalCount": len(fake_db[:1]),
-            "currentPageSize": pagination_params.get("pageSize"),
-            "currentPageNumber": pagination_params.get("page"),
-            "hasNext": False
-        }
+        ...
+        # pagination_params = utils.dictify_query_params(request.query_params.get("pagination"))
+        # assert pagination_params == {"pageSize": 1, "page": 0}
+        # assert query == fake_db_query1
+        # return {
+        #     "data": fake_db[:1],
+        #     "totalCount": len(fake_db[:1]),
+        #     "currentPageSize": pagination_params.get("pageSize"),
+        #     "currentPageNumber": pagination_params.get("page"),
+        #     "hasNext": False
+        # }
 
 
 strategy_factory.register_strategy("fake_paginator_strategy_v2", FakePaginationStrategyV2)
 
 
-class TestListingServiceVariablePageFlow(ListingService):
-    DEFAULT_SRT_ON = "id"
-    dao_kls = FakeProductDao
-    QUERY_STRATEGY = "fake_query_strategy"
-    SORTING_STRATEGY = "fake_sorting_strategy"
-    PAGINATE_STRATEGY = "fake_paginator_strategy_v2"
-
-    def get_listing(self):
-        return FastapiListing(self.request, self.dao, ProductDetail).get_response(self.MetaInfo(self))
-
-
-class FakeSortingStrategyV2(SortingOrderStrategy):
-
-    def sort(self, *, query=None, value: Dict[str, str] = None,
-             extra_context: dict = None):
-        assert value["type"] in ["asc", "dsc"], "invalid sorting style!"
-        assert query == fake_db_query1
-
-        return query
-
-
-strategy_factory.register_strategy("fake_sorting_strategy_v2", FakeSortingStrategyV2)
-
-
-class TestListingServiceSortFlow(ListingService):
-    DEFAULT_SRT_ON = "id"
-    dao_kls = FakeProductDao
-    QUERY_STRATEGY = "fake_query_strategy"
-    SORTING_STRATEGY = "fake_sorting_strategy_v2"
-    PAGINATE_STRATEGY = "fake_paginator_strategy_v2"
-
-    sort_mapper = {
-        "id": "Product.product_id"
-    }
-
-    def get_listing(self):
-        return FastapiListing(self.request, self.dao, ProductDetail).get_response(self.MetaInfo(self))
 
 
 def spawn_valueerror_for_strategy_registry(strategy1, strategy2):
     strategy_factory.register_strategy(strategy1, FakePaginationStrategyV2)
     strategy_factory.register_strategy(strategy2, FakePaginationStrategyV2)
 
 
@@ -288,10 +253,8 @@
 
 
 def invalid_type_factory_keys(factory, key):
     if factory == "filter":
         filter_factory.register_filter(key, generic_filters.EqualityFilter)
     elif factory == "strategy":
         strategy_factory.register_strategy(key, FakePaginationStrategyV2)
-    else:
-        raise ValueError("Invalid factory selection!")
```

### Comparing `fastapi-listing-0.0.8/tests/test_main.py` & `fastapi-listing-0.2.1/tests/test_main.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,112 +1,110 @@
 from fastapi import Request
 from fastapi import FastAPI
 import pytest
 from fastapi.testclient import TestClient
-from .fake_listing_setup import ProductPage, TestListingServiceDefaultFlow, fake_db_response, \
-    fake_db_response_page_size_1, TestListingServiceVariablePageFlow, TestListingServiceSortFlow, \
-    spawn_valueerror_for_strategy_registry, spawn_valueerror_for_filter_factory, invalid_type_factory_keys, ProductPageWithCustomColumns, TestListingServiceDefaultFlowWithCustomColumns, fake_db_response_with_custom_column
-from fastapi_listing.errors import ListingFilterError
+from .fake_listing_setup import  \
+    spawn_valueerror_for_strategy_registry, spawn_valueerror_for_filter_factory, invalid_type_factory_keys
 
 app = FastAPI()
 
-
-@app.get("/", response_model=ProductPage)
-def read_main(request: Request):
-    resp = TestListingServiceDefaultFlow(request, read_db="read_db_session", write_db="write_db_session").get_listing()
-    return resp
-
-
-@app.get("/custom-columns", response_model=ProductPageWithCustomColumns)
-def read_main_with_custom_fields(request: Request):
-    resp = TestListingServiceDefaultFlowWithCustomColumns(request, read_db="read_db_session", write_db="write_db_session").get_listing()
-    return resp
-
-
-@app.get("/var-page", response_model=ProductPage)
-def read_limit_1_page(request: Request):
-    resp = TestListingServiceVariablePageFlow(request, read_db="read_db_session",
-                                               write_db="write_db_session").get_listing()
-    return resp
-
-
-@app.get("/sort", response_model=ProductPage)
-def sort_test(reqeust: Request):
-    resp = TestListingServiceSortFlow(reqeust).get_listing()
-    return resp
+# @app.get("/", response_model=ProductPage)
+# def read_main(request: Request):
+#     resp = TestListingServiceDefaultFlow(request, read_db="read_db_session", write_db="write_db_session").get_listing()
+#     return resp
+#
+#
+# @app.get("/custom-columns", response_model=ProductPageWithCustomColumns)
+# def read_main_with_custom_fields(request: Request):
+#     resp = TestListingServiceDefaultFlowWithCustomColumns(request, read_db="read_db_session",
+#                                                           write_db="write_db_session").get_listing()
+#     return resp
+#
+#
+# @app.get("/var-page", response_model=ProductPage)
+# def read_limit_1_page(request: Request):
+#     resp = TestListingServiceVariablePageFlow(request, read_db="read_db_session",
+#                                               write_db="write_db_session").get_listing()
+#     return resp
+#
+#
+# @app.get("/sort", response_model=ProductPage)
+# def sort_test(reqeust: Request):
+#     resp = TestListingServiceSortFlow(reqeust).get_listing()
+#     return resp
 
 
 client = TestClient(app)
 
 
-def test_call_default():
-    response = client.get("/", params={"pagination": "%7B%22pageSize%22%3A10%2C%20%22page%22%3A0%7D"})
-    assert response.status_code == 200
-    assert response.json() == fake_db_response
-
-
-def test_call_default_flow_with_custom_columns():
-    response = client.get("/custom-columns", params={"pagination": "%7B%22pageSize%22%3A10%2C%20%22page%22%3A0%7D"})
-    assert response.status_code == 200
-    assert response.json() == fake_db_response_with_custom_column
-
-
-def test_call_variable_page():
-    response = client.get("/var-page", params={"pagination": "%7B%22pageSize%22%3A1%2C%20%22page%22%3A0%7D"})
-    assert response.status_code == 200
-    assert response.json() == fake_db_response_page_size_1
-
-
-def test_call_filter_not_registered():
-    # filter = [{"field":"abc", "value":{"search":"something"}}]
-    # with pytest.raises(Exception) as exc_info:
-    response = client.get("/var-page", params={"pagination": "%7B%22pageSize%22%3A1%2C%20%22page%22%3A0%7D",
-                                               "filter": "%5B%7B%22field%22%3A%22abc%22%2C%20%22value%22%3A%7B%22search%22%3A%22something%22%7D%7D%5D"})
-
-    assert response.status_code == 409
-    assert response.json().get("detail") == "Filter'(s) not registered with listing: {'abc'}, Did you forget to do it?"
-
-
-def test_call_sort_not_registered():
-    # sort =[{"field":"abc", "type":"asc"}]
-    response = client.get("/var-page", params={"pagination": "%7B%22pageSize%22%3A1%2C%20%22page%22%3A0%7D",
-                                               "sort": "%5B%7B%22field%22%3A%22abc%22%2C%20%22type%22%3A%22asc%22%7D%5D"})
-
-    assert response.status_code == 409
-    assert response.json().get("detail") == "Sorter'(s) not registered with listing: {'abc'}, Did you forget to do it?"
-
-
-def test_defective_sorter_semantic():
-    response = client.get("/var-page", params={"pagination": "%7B%22pageSize%22%3A1%2C%20%22page%22%3A0%7D",
-                                               "sort": "%5B%7B%22field%22%3Aabc%22%2C%20%22type%22%22asc%22%7D%5D"})
-
-    assert response.status_code == 422
-    assert response.json().get("detail") == "sorter param is not a valid json!"
-
-
-def test_defective_filter_semantic():
-    response = client.get("/var-page", params={"pagination": "%7B%22pageSize%22%3A1%2C%20%22page%22%3A0%7D",
-                                               "filter": "%5B%7B%22field%22%3A%22abc%22%2C%20%22value%22%7B%22searsomething%22%7D%5D"})
-
-    assert response.status_code == 422
-    assert response.json().get("detail") == "filter param is not a valid json!"
-
-
-def test_unknown_sorting_style():
-    with pytest.raises(AssertionError) as e:
-        response = client.get("/sort", params={"pagination": "%7B%22pageSize%22%3A1%2C%20%22page%22%3A0%7D",
-                                               "sort": "%5B%7B%22field%22%3A%22id%22%2C%20%22type%22%3A%22somethingse%22%7D%5D"})
-
-    assert e.value.args[0] == "invalid sorting style!"
-
-
+# def test_call_default():
+#     response = client.get("/", params={"pagination": "%7B%22pageSize%22%3A10%2C%20%22page%22%3A0%7D"})
+#     assert response.status_code == 200
+#     assert response.json() == fake_db_response
+#
+#
+# def test_call_default_flow_with_custom_columns():
+#     response = client.get("/custom-columns", params={"pagination": "%7B%22pageSize%22%3A10%2C%20%22page%22%3A0%7D"})
+#     assert response.status_code == 200
+#     assert response.json() == fake_db_response_with_custom_column
+#
+#
+# def test_call_variable_page():
+#     response = client.get("/var-page", params={"pagination": "%7B%22pageSize%22%3A1%2C%20%22page%22%3A0%7D"})
+#     assert response.status_code == 200
+#     assert response.json() == fake_db_response_page_size_1
+#
+#
+# def test_call_filter_not_registered():
+#     # filter = [{"field":"abc", "value":{"search":"something"}}]
+#     # with pytest.raises(Exception) as exc_info:
+#     response = client.get("/var-page", params={"pagination": "%7B%22pageSize%22%3A1%2C%20%22page%22%3A0%7D",
+#                                                "filter": "%5B%7B%22field%22%3A%22abc%22%2C%20%22value%22%3A%7B%22search%22%3A%22something%22%7D%7D%5D"})
+#
+#     assert response.status_code == 409
+#     assert response.json().get("detail") == "Filter'(s) not registered with listing: {'abc'}, Did you forget to do it?"
+#
+#
+# def test_call_sort_not_registered():
+#     # sort =[{"field":"abc", "type":"asc"}]
+#     response = client.get("/var-page", params={"pagination": "%7B%22pageSize%22%3A1%2C%20%22page%22%3A0%7D",
+#                                                "sort": "%5B%7B%22field%22%3A%22abc%22%2C%20%22type%22%3A%22asc%22%7D%5D"})
+#
+#     assert response.status_code == 409
+#     assert response.json().get("detail") == "Sorter'(s) not registered with listing: {'abc'}, Did you forget to do it?"
+#
+#
+# def test_defective_sorter_semantic():
+#     response = client.get("/var-page", params={"pagination": "%7B%22pageSize%22%3A1%2C%20%22page%22%3A0%7D",
+#                                                "sort": "%5B%7B%22field%22%3Aabc%22%2C%20%22type%22%22asc%22%7D%5D"})
+#
+#     assert response.status_code == 422
+#     assert response.json().get("detail") == "sorter param is not a valid json!"
+#
+#
+# def test_defective_filter_semantic():
+#     response = client.get("/var-page", params={"pagination": "%7B%22pageSize%22%3A1%2C%20%22page%22%3A0%7D",
+#                                                "filter": "%5B%7B%22field%22%3A%22abc%22%2C%20%22value%22%7B%22searsomething%22%7D%5D"})
+#
+#     assert response.status_code == 422
+#     assert response.json().get("detail") == "filter param is not a valid json!"
+#
+#
+# def test_unknown_sorting_style():
+#     with pytest.raises(AssertionError) as e:
+#         response = client.get("/sort", params={"pagination": "%7B%22pageSize%22%3A1%2C%20%22page%22%3A0%7D",
+#                                                "sort": "%5B%7B%22field%22%3A%22id%22%2C%20%22type%22%3A%22somethingse%22%7D%5D"})
+#
+#     assert e.value.args[0] == "invalid sorting style!"
+#
+#
 def test_strategy_factory_unique_strategy_register():
     with pytest.raises(ValueError) as e:
         spawn_valueerror_for_strategy_registry("same_strategy_key", "same_strategy_key")
-    assert e.value.args[0] == "strategy name already in use with FakePaginationStrategyV2!"
+    assert e.value.args[0] == "strategy name: same_strategy_key, already in use with FakePaginationStrategyV2!"
 
 
 def test_filter_factory_unique_strategy_register():
     with pytest.raises(ValueError) as e:
         spawn_valueerror_for_filter_factory("same_field_name", "same_field_name")
     assert e.value.args[0] == "filter name already in use with EqualityFilter!"
 
@@ -123,7 +121,22 @@
     with pytest.raises(ValueError) as e:
         invalid_type_factory_keys("strategy", None)
     assert e.value.args[0] == "Invalid type key!"
 
     with pytest.raises(ValueError) as e:
         invalid_type_factory_keys("strategy", "")
     assert e.value.args[0] == "Invalid type key!"
+
+
+def test_dao_factory():
+    from fastapi_listing.dao import dao_factory
+    from .dao_setup import TitleDao
+    with pytest.raises(ValueError) as e:
+        dao_factory.register_dao(None, None)
+    assert e.value.args[0] == "Invalid type key, expected str type got <class 'NoneType'>!"
+    dao_factory.register_dao("titlepre", TitleDao)
+    with pytest.raises(ValueError) as e:
+        dao_factory.register_dao("titlepre", None)
+    assert e.value.args[0] == "Dao name titlepre already in use with TitleDao!"
+    with pytest.raises(ValueError) as e:
+        dao_factory.create(None)
+    assert e.value.args[0] == None
```

