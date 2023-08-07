# Comparing `tmp/bw_matchbox-1.0.3.tar.gz` & `tmp/bw_matchbox-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bw_matchbox-1.0.3.tar", last modified: Mon Aug  7 18:25:46 2023, max compression
+gzip compressed data, was "bw_matchbox-1.0.4.tar", last modified: Mon Aug  7 21:45:58 2023, max compression
```

## Comparing `bw_matchbox-1.0.3.tar` & `bw_matchbox-1.0.4.tar`

### file list

```diff
@@ -1,86 +1,84 @@
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-07 18:25:46.966080 bw_matchbox-1.0.3/
--rw-r--r--   0 chrismutel   (501) staff       (20)     1067 2023-06-20 12:26:53.000000 bw_matchbox-1.0.3/LICENSE
--rw-r--r--   0 chrismutel   (501) staff       (20)      226 2023-08-02 21:05:25.000000 bw_matchbox-1.0.3/MANIFEST.in
--rw-r--r--   0 chrismutel   (501) staff       (20)     6361 2023-08-07 18:25:46.966174 bw_matchbox-1.0.3/PKG-INFO
--rw-r--r--   0 chrismutel   (501) staff       (20)     5337 2023-08-05 17:26:08.000000 bw_matchbox-1.0.3/README.md
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-07 18:25:46.856857 bw_matchbox-1.0.3/bw_matchbox/
--rw-r--r--   0 chrismutel   (501) staff       (20)        6 2023-08-07 18:25:11.000000 bw_matchbox-1.0.3/bw_matchbox/VERSION
--rw-r--r--   0 chrismutel   (501) staff       (20)      215 2023-08-01 17:17:21.000000 bw_matchbox-1.0.3/bw_matchbox/__init__.py
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-07 18:25:46.846595 bw_matchbox-1.0.3/bw_matchbox/assets/
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-07 18:25:46.883003 bw_matchbox-1.0.3/bw_matchbox/assets/css/
--rw-r--r--   0 chrismutel   (501) staff       (20)     4266 2023-08-07 17:38:14.000000 bw_matchbox-1.0.3/bw_matchbox/assets/css/common-modal.css
--rw-r--r--   0 chrismutel   (501) staff       (20)     1922 2023-08-06 18:22:10.000000 bw_matchbox-1.0.3/bw_matchbox/assets/css/common.css
--rw-r--r--   0 chrismutel   (501) staff       (20)     4256 2023-08-07 17:38:14.000000 bw_matchbox-1.0.3/bw_matchbox/assets/css/compare.css
--rw-r--r--   0 chrismutel   (501) staff       (20)      640 2023-08-03 20:45:26.000000 bw_matchbox-1.0.3/bw_matchbox/assets/css/customizations.css
--rw-r--r--   0 chrismutel   (501) staff       (20)     1392 2023-08-04 13:00:53.000000 bw_matchbox-1.0.3/bw_matchbox/assets/css/fixed-table.css
--rw-r--r--   0 chrismutel   (501) staff       (20)     7618 2023-08-01 07:10:26.000000 bw_matchbox-1.0.3/bw_matchbox/assets/css/normalize.css
--rw-r--r--   0 chrismutel   (501) staff       (20)       99 2023-08-07 17:38:14.000000 bw_matchbox-1.0.3/bw_matchbox/assets/css/process-detail.css
--rw-r--r--   0 chrismutel   (501) staff       (20)     4315 2023-08-06 18:22:10.000000 bw_matchbox-1.0.3/bw_matchbox/assets/css/processes-list.css
--rw-r--r--   0 chrismutel   (501) staff       (20)    11556 2023-08-01 07:10:26.000000 bw_matchbox-1.0.3/bw_matchbox/assets/css/skeleton.css
--rw-r--r--   0 chrismutel   (501) staff       (20)      916 2023-08-01 07:10:26.000000 bw_matchbox-1.0.3/bw_matchbox/assets/css/tooltip.css
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-07 18:25:46.884824 bw_matchbox-1.0.3/bw_matchbox/assets/images/
--rw-r--r--   0 chrismutel   (501) staff       (20)    32038 2023-06-20 12:27:44.000000 bw_matchbox-1.0.3/bw_matchbox/assets/images/favicon.ico
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-07 18:25:46.846492 bw_matchbox-1.0.3/bw_matchbox/assets/js/
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-07 18:25:46.897383 bw_matchbox-1.0.3/bw_matchbox/assets/js/Compare/
--rw-r--r--   0 chrismutel   (501) staff       (20)    20293 2023-08-07 07:57:13.000000 bw_matchbox-1.0.3/bw_matchbox/assets/js/Compare/CompareCore.js
--rw-r--r--   0 chrismutel   (501) staff       (20)     6250 2023-08-07 17:38:14.000000 bw_matchbox-1.0.3/bw_matchbox/assets/js/Compare/CompareProxyDialogModal.js
--rw-r--r--   0 chrismutel   (501) staff       (20)     1272 2023-08-04 16:42:28.000000 bw_matchbox-1.0.3/bw_matchbox/assets/js/Compare/CompareRowClick.js
--rw-r--r--   0 chrismutel   (501) staff       (20)    12879 2023-08-06 18:22:10.000000 bw_matchbox-1.0.3/bw_matchbox/assets/js/Compare/CompareRowsHelpers.js
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-07 18:25:46.900251 bw_matchbox-1.0.3/bw_matchbox/assets/js/ProcessDetail/
--rw-r--r--   0 chrismutel   (501) staff       (20)     7506 2023-08-07 17:41:58.000000 bw_matchbox-1.0.3/bw_matchbox/assets/js/ProcessDetail/ProcessDetail.js
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-07 18:25:46.919399 bw_matchbox-1.0.3/bw_matchbox/assets/js/ProcessesList/
--rw-r--r--   0 chrismutel   (501) staff       (20)     4388 2023-08-06 18:22:10.000000 bw_matchbox-1.0.3/bw_matchbox/assets/js/ProcessesList/ProcessesList.js
--rw-r--r--   0 chrismutel   (501) staff       (20)      885 2023-08-06 18:22:10.000000 bw_matchbox-1.0.3/bw_matchbox/assets/js/ProcessesList/ProcessesListConstants.js
--rw-r--r--   0 chrismutel   (501) staff       (20)     1452 2023-08-06 18:22:10.000000 bw_matchbox-1.0.3/bw_matchbox/assets/js/ProcessesList/ProcessesListData.js
--rw-r--r--   0 chrismutel   (501) staff       (20)     5068 2023-08-07 17:38:14.000000 bw_matchbox-1.0.3/bw_matchbox/assets/js/ProcessesList/ProcessesListDataLoad.js
--rw-r--r--   0 chrismutel   (501) staff       (20)     3447 2023-08-06 18:22:10.000000 bw_matchbox-1.0.3/bw_matchbox/assets/js/ProcessesList/ProcessesListDataRender.js
--rw-r--r--   0 chrismutel   (501) staff       (20)     1081 2023-08-06 18:22:10.000000 bw_matchbox-1.0.3/bw_matchbox/assets/js/ProcessesList/ProcessesListNodes.js
--rw-r--r--   0 chrismutel   (501) staff       (20)     4862 2023-08-06 18:22:10.000000 bw_matchbox-1.0.3/bw_matchbox/assets/js/ProcessesList/ProcessesListPagination.UNUSED.js
--rw-r--r--   0 chrismutel   (501) staff       (20)     3321 2023-08-06 18:22:10.000000 bw_matchbox-1.0.3/bw_matchbox/assets/js/ProcessesList/ProcessesListSearch.js
--rw-r--r--   0 chrismutel   (501) staff       (20)     9995 2023-08-06 18:22:10.000000 bw_matchbox-1.0.3/bw_matchbox/assets/js/ProcessesList/ProcessesListStates.js
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-07 18:25:46.922878 bw_matchbox-1.0.3/bw_matchbox/assets/js/common/
--rw-r--r--   0 chrismutel   (501) staff       (20)     5634 2023-08-04 13:00:53.000000 bw_matchbox-1.0.3/bw_matchbox/assets/js/common/CommonHelpers.js
--rw-r--r--   0 chrismutel   (501) staff       (20)     8875 2023-08-07 17:38:14.000000 bw_matchbox-1.0.3/bw_matchbox/assets/js/common/CommonModal.js
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-07 18:25:46.846536 bw_matchbox-1.0.3/bw_matchbox/assets/js/libs/
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-07 18:25:46.928526 bw_matchbox-1.0.3/bw_matchbox/assets/js/libs/ym/
--rw-r--r--   0 chrismutel   (501) staff       (20)    13286 2023-08-03 20:45:26.000000 bw_matchbox-1.0.3/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.js
--rw-r--r--   0 chrismutel   (501) staff       (20)     6018 2023-08-03 20:45:26.000000 bw_matchbox-1.0.3/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.min.js
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-07 18:25:46.960842 bw_matchbox-1.0.3/bw_matchbox/assets/templates/
--rw-r--r--   0 chrismutel   (501) staff       (20)      756 2023-08-04 13:00:53.000000 bw_matchbox-1.0.3/bw_matchbox/assets/templates/common-modal.html
--rw-r--r--   0 chrismutel   (501) staff       (20)     3916 2023-08-07 17:38:14.000000 bw_matchbox-1.0.3/bw_matchbox/assets/templates/compare.html
--rw-r--r--   0 chrismutel   (501) staff       (20)     2681 2023-08-05 17:26:08.000000 bw_matchbox-1.0.3/bw_matchbox/assets/templates/databases.html
--rw-r--r--   0 chrismutel   (501) staff       (20)      461 2023-07-23 15:09:13.000000 bw_matchbox-1.0.3/bw_matchbox/assets/templates/expand.html
--rw-r--r--   0 chrismutel   (501) staff       (20)       16 2023-06-20 12:27:44.000000 bw_matchbox-1.0.3/bw_matchbox/assets/templates/footer.html
--rw-r--r--   0 chrismutel   (501) staff       (20)     2666 2023-08-04 13:00:53.000000 bw_matchbox-1.0.3/bw_matchbox/assets/templates/header.html
--rw-r--r--   0 chrismutel   (501) staff       (20)     6983 2023-08-07 17:38:14.000000 bw_matchbox-1.0.3/bw_matchbox/assets/templates/index.html
--rw-r--r--   0 chrismutel   (501) staff       (20)      733 2023-06-21 04:56:26.000000 bw_matchbox-1.0.3/bw_matchbox/assets/templates/match-status.html
--rw-r--r--   0 chrismutel   (501) staff       (20)     1713 2023-08-07 17:38:14.000000 bw_matchbox-1.0.3/bw_matchbox/assets/templates/match.html
--rw-r--r--   0 chrismutel   (501) staff       (20)      734 2023-08-05 17:26:08.000000 bw_matchbox-1.0.3/bw_matchbox/assets/templates/navigation.html
--rw-r--r--   0 chrismutel   (501) staff       (20)     5890 2023-08-07 18:24:38.000000 bw_matchbox-1.0.3/bw_matchbox/assets/templates/process_detail.html
--rw-r--r--   0 chrismutel   (501) staff       (20)      599 2023-07-22 21:06:00.000000 bw_matchbox-1.0.3/bw_matchbox/assets/templates/project.html
--rw-r--r--   0 chrismutel   (501) staff       (20)      412 2023-08-01 07:10:26.000000 bw_matchbox-1.0.3/bw_matchbox/assets/templates/search-embedded.html
--rw-r--r--   0 chrismutel   (501) staff       (20)      850 2023-06-20 12:27:44.000000 bw_matchbox-1.0.3/bw_matchbox/assets/templates/search.html
--rw-r--r--   0 chrismutel   (501) staff       (20)      947 2023-06-20 12:27:44.000000 bw_matchbox-1.0.3/bw_matchbox/assets/templates/search_result.html
--rw-r--r--   0 chrismutel   (501) staff       (20)     1243 2023-07-23 08:33:52.000000 bw_matchbox-1.0.3/bw_matchbox/assets/templates/select_files.html
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-07 18:25:46.961355 bw_matchbox-1.0.3/bw_matchbox/bin/
--rw-r--r--   0 chrismutel   (501) staff       (20)        0 2023-06-20 12:27:44.000000 bw_matchbox-1.0.3/bw_matchbox/bin/__init__.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     2692 2023-08-05 17:26:08.000000 bw_matchbox-1.0.3/bw_matchbox/bin/matchbox.py
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-07 18:25:46.963455 bw_matchbox-1.0.3/bw_matchbox/data/
--rw-r--r--   0 chrismutel   (501) staff       (20)   123246 2023-08-01 17:17:21.000000 bw_matchbox-1.0.3/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-mining.json
--rw-r--r--   0 chrismutel   (501) staff       (20)    93862 2023-07-23 09:30:53.000000 bw_matchbox-1.0.3/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-string-matching.json
--rw-r--r--   0 chrismutel   (501) staff       (20)   116072 2023-08-01 17:17:21.000000 bw_matchbox-1.0.3/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-transport.json
--rw-r--r--   0 chrismutel   (501) staff       (20)      603 2023-07-23 09:34:59.000000 bw_matchbox-1.0.3/bw_matchbox/data/dare.json
--rw-r--r--   0 chrismutel   (501) staff       (20)     2204 2023-08-07 09:06:12.000000 bw_matchbox-1.0.3/bw_matchbox/utils.py
--rw-r--r--   0 chrismutel   (501) staff       (20)    22989 2023-08-07 17:38:14.000000 bw_matchbox-1.0.3/bw_matchbox/webapp.py
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-07 18:25:46.964876 bw_matchbox-1.0.3/bw_matchbox.egg-info/
--rw-r--r--   0 chrismutel   (501) staff       (20)     6361 2023-08-07 18:25:46.000000 bw_matchbox-1.0.3/bw_matchbox.egg-info/PKG-INFO
--rw-r--r--   0 chrismutel   (501) staff       (20)     5284 2023-08-07 18:25:46.000000 bw_matchbox-1.0.3/bw_matchbox.egg-info/SOURCES.txt
--rw-r--r--   0 chrismutel   (501) staff       (20)        1 2023-08-07 18:25:46.000000 bw_matchbox-1.0.3/bw_matchbox.egg-info/dependency_links.txt
--rw-r--r--   0 chrismutel   (501) staff       (20)       59 2023-08-07 18:25:46.000000 bw_matchbox-1.0.3/bw_matchbox.egg-info/entry_points.txt
--rw-r--r--   0 chrismutel   (501) staff       (20)        1 2023-07-23 07:30:31.000000 bw_matchbox-1.0.3/bw_matchbox.egg-info/not-zip-safe
--rw-r--r--   0 chrismutel   (501) staff       (20)      167 2023-08-07 18:25:46.000000 bw_matchbox-1.0.3/bw_matchbox.egg-info/requires.txt
--rw-r--r--   0 chrismutel   (501) staff       (20)       12 2023-08-07 18:25:46.000000 bw_matchbox-1.0.3/bw_matchbox.egg-info/top_level.txt
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-07 18:25:46.963702 bw_matchbox-1.0.3/docs/
--rw-r--r--   0 chrismutel   (501) staff       (20)     1145 2023-07-23 07:23:19.000000 bw_matchbox-1.0.3/docs/conf.py
--rw-r--r--   0 chrismutel   (501) staff       (20)       87 2023-06-20 12:26:53.000000 bw_matchbox-1.0.3/pyproject.toml
--rw-r--r--   0 chrismutel   (501) staff       (20)     1900 2023-08-07 18:25:46.966558 bw_matchbox-1.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:45:58.858666 bw_matchbox-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-08-07 21:45:42.000000 bw_matchbox-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-08-07 21:45:42.000000 bw_matchbox-1.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-08-07 21:45:58.858666 bw_matchbox-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5337 2023-08-07 21:45:42.000000 bw_matchbox-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:45:58.842666 bw_matchbox-1.0.4/bw_matchbox/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-07 21:45:42.000000 bw_matchbox-1.0.4/bw_matchbox/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-08-07 21:45:42.000000 bw_matchbox-1.0.4/bw_matchbox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:45:58.842666 bw_matchbox-1.0.4/bw_matchbox/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:45:58.846666 bw_matchbox-1.0.4/bw_matchbox/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-08-07 21:45:42.000000 bw_matchbox-1.0.4/bw_matchbox/assets/css/common-modal.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-08-07 21:45:42.000000 bw_matchbox-1.0.4/bw_matchbox/assets/css/common.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-08-07 21:45:42.000000 bw_matchbox-1.0.4/bw_matchbox/assets/css/compare.css
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-08-07 21:45:42.000000 bw_matchbox-1.0.4/bw_matchbox/assets/css/customizations.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-08-07 21:45:42.000000 bw_matchbox-1.0.4/bw_matchbox/assets/css/fixed-table.css
+-rw-r--r--   0 runner    (1001) docker     (123)     7618 2023-08-07 21:45:42.000000 bw_matchbox-1.0.4/bw_matchbox/assets/css/normalize.css
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-08-07 21:45:42.000000 bw_matchbox-1.0.4/bw_matchbox/assets/css/process-detail.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-08-07 21:45:42.000000 bw_matchbox-1.0.4/bw_matchbox/assets/css/processes-list.css
+-rw-r--r--   0 runner    (1001) docker     (123)    11556 2023-08-07 21:45:42.000000 bw_matchbox-1.0.4/bw_matchbox/assets/css/skeleton.css
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-07 21:45:42.000000 bw_matchbox-1.0.4/bw_matchbox/assets/css/tooltip.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:45:58.846666 bw_matchbox-1.0.4/bw_matchbox/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    32038 2023-08-07 21:45:42.000000 bw_matchbox-1.0.4/bw_matchbox/assets/images/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:45:58.842666 bw_matchbox-1.0.4/bw_matchbox/assets/js/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:45:58.846666 bw_matchbox-1.0.4/bw_matchbox/assets/js/Compare/
+-rw-r--r--   0 runner    (1001) docker     (123)    20293 2023-08-07 21:45:42.000000 bw_matchbox-1.0.4/bw_matchbox/assets/js/Compare/CompareCore.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-08-07 21:45:42.000000 bw_matchbox-1.0.4/bw_matchbox/assets/js/Compare/CompareProxyDialogModal.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-08-07 21:45:42.000000 bw_matchbox-1.0.4/bw_matchbox/assets/js/Compare/CompareRowClick.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12879 2023-08-07 21:45:42.000000 bw_matchbox-1.0.4/bw_matchbox/assets/js/Compare/CompareRowsHelpers.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:45:58.846666 bw_matchbox-1.0.4/bw_matchbox/assets/js/ProcessDetail/
+-rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-08-07 21:45:42.000000 bw_matchbox-1.0.4/bw_matchbox/assets/js/ProcessDetail/ProcessDetail.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:45:58.850666 bw_matchbox-1.0.4/bw_matchbox/assets/js/ProcessesList/
+-rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-08-07 21:45:42.000000 bw_matchbox-1.0.4/bw_matchbox/assets/js/ProcessesList/ProcessesList.js
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-08-07 21:45:42.000000 bw_matchbox-1.0.4/bw_matchbox/assets/js/ProcessesList/ProcessesListConstants.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-08-07 21:45:42.000000 bw_matchbox-1.0.4/bw_matchbox/assets/js/ProcessesList/ProcessesListData.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-08-07 21:45:42.000000 bw_matchbox-1.0.4/bw_matchbox/assets/js/ProcessesList/ProcessesListDataLoad.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-08-07 21:45:42.000000 bw_matchbox-1.0.4/bw_matchbox/assets/js/ProcessesList/ProcessesListDataRender.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-08-07 21:45:42.000000 bw_matchbox-1.0.4/bw_matchbox/assets/js/ProcessesList/ProcessesListNodes.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4862 2023-08-07 21:45:42.000000 bw_matchbox-1.0.4/bw_matchbox/assets/js/ProcessesList/ProcessesListPagination.UNUSED.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-08-07 21:45:42.000000 bw_matchbox-1.0.4/bw_matchbox/assets/js/ProcessesList/ProcessesListSearch.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9995 2023-08-07 21:45:42.000000 bw_matchbox-1.0.4/bw_matchbox/assets/js/ProcessesList/ProcessesListStates.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:45:58.850666 bw_matchbox-1.0.4/bw_matchbox/assets/js/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-08-07 21:45:42.000000 bw_matchbox-1.0.4/bw_matchbox/assets/js/common/CommonHelpers.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8875 2023-08-07 21:45:42.000000 bw_matchbox-1.0.4/bw_matchbox/assets/js/common/CommonModal.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:45:58.842666 bw_matchbox-1.0.4/bw_matchbox/assets/js/libs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:45:58.850666 bw_matchbox-1.0.4/bw_matchbox/assets/js/libs/ym/
+-rw-r--r--   0 runner    (1001) docker     (123)    13286 2023-08-07 21:45:42.000000 bw_matchbox-1.0.4/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-08-07 21:45:42.000000 bw_matchbox-1.0.4/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:45:58.854666 bw_matchbox-1.0.4/bw_matchbox/assets/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-08-07 21:45:42.000000 bw_matchbox-1.0.4/bw_matchbox/assets/templates/common-modal.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-08-07 21:45:42.000000 bw_matchbox-1.0.4/bw_matchbox/assets/templates/compare.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-08-07 21:45:42.000000 bw_matchbox-1.0.4/bw_matchbox/assets/templates/databases.html
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-08-07 21:45:42.000000 bw_matchbox-1.0.4/bw_matchbox/assets/templates/expand.html
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-07 21:45:42.000000 bw_matchbox-1.0.4/bw_matchbox/assets/templates/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-08-07 21:45:42.000000 bw_matchbox-1.0.4/bw_matchbox/assets/templates/header.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6983 2023-08-07 21:45:42.000000 bw_matchbox-1.0.4/bw_matchbox/assets/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-08-07 21:45:42.000000 bw_matchbox-1.0.4/bw_matchbox/assets/templates/match-status.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-08-07 21:45:42.000000 bw_matchbox-1.0.4/bw_matchbox/assets/templates/match.html
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-08-07 21:45:42.000000 bw_matchbox-1.0.4/bw_matchbox/assets/templates/navigation.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-08-07 21:45:42.000000 bw_matchbox-1.0.4/bw_matchbox/assets/templates/process_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-08-07 21:45:42.000000 bw_matchbox-1.0.4/bw_matchbox/assets/templates/project.html
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-08-07 21:45:42.000000 bw_matchbox-1.0.4/bw_matchbox/assets/templates/search-embedded.html
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-08-07 21:45:42.000000 bw_matchbox-1.0.4/bw_matchbox/assets/templates/search.html
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-07 21:45:42.000000 bw_matchbox-1.0.4/bw_matchbox/assets/templates/search_result.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-08-07 21:45:42.000000 bw_matchbox-1.0.4/bw_matchbox/assets/templates/select_files.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:45:58.854666 bw_matchbox-1.0.4/bw_matchbox/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 21:45:42.000000 bw_matchbox-1.0.4/bw_matchbox/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-08-07 21:45:42.000000 bw_matchbox-1.0.4/bw_matchbox/bin/matchbox.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:45:58.854666 bw_matchbox-1.0.4/bw_matchbox/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   123246 2023-08-07 21:45:42.000000 bw_matchbox-1.0.4/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-mining.json
+-rw-r--r--   0 runner    (1001) docker     (123)    93862 2023-08-07 21:45:42.000000 bw_matchbox-1.0.4/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-string-matching.json
+-rw-r--r--   0 runner    (1001) docker     (123)   116072 2023-08-07 21:45:42.000000 bw_matchbox-1.0.4/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-transport.json
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-08-07 21:45:42.000000 bw_matchbox-1.0.4/bw_matchbox/data/dare.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-08-07 21:45:42.000000 bw_matchbox-1.0.4/bw_matchbox/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24465 2023-08-07 21:45:42.000000 bw_matchbox-1.0.4/bw_matchbox/webapp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:45:58.858666 bw_matchbox-1.0.4/bw_matchbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-08-07 21:45:58.000000 bw_matchbox-1.0.4/bw_matchbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-08-07 21:45:58.000000 bw_matchbox-1.0.4/bw_matchbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 21:45:58.000000 bw_matchbox-1.0.4/bw_matchbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-07 21:45:58.000000 bw_matchbox-1.0.4/bw_matchbox.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 21:45:58.000000 bw_matchbox-1.0.4/bw_matchbox.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-08-07 21:45:58.000000 bw_matchbox-1.0.4/bw_matchbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-07 21:45:58.000000 bw_matchbox-1.0.4/bw_matchbox.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-07 21:45:42.000000 bw_matchbox-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-08-07 21:45:58.858666 bw_matchbox-1.0.4/setup.cfg
```

### Comparing `bw_matchbox-1.0.3/LICENSE` & `bw_matchbox-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.3/PKG-INFO` & `bw_matchbox-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bw_matchbox
-Version: 1.0.3
+Version: 1.0.4
 Summary: Browser to match Brightway databases
 Home-page: https://github.com/cauldron/bw_matchbox
 Author: Chris Mutel
 Author-email: <cmutel@gmail.com>
 Maintainer: Chris Mutel
 Maintainer-email: <cmutel@gmail.com>
 License: MIT
```

### Comparing `bw_matchbox-1.0.3/README.md` & `bw_matchbox-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.3/bw_matchbox/assets/css/common-modal.css` & `bw_matchbox-1.0.4/bw_matchbox/assets/css/common-modal.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.3/bw_matchbox/assets/css/common.css` & `bw_matchbox-1.0.4/bw_matchbox/assets/css/common.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.3/bw_matchbox/assets/css/compare.css` & `bw_matchbox-1.0.4/bw_matchbox/assets/css/compare.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.3/bw_matchbox/assets/css/customizations.css` & `bw_matchbox-1.0.4/bw_matchbox/assets/css/customizations.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.3/bw_matchbox/assets/css/fixed-table.css` & `bw_matchbox-1.0.4/bw_matchbox/assets/css/fixed-table.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.3/bw_matchbox/assets/css/normalize.css` & `bw_matchbox-1.0.4/bw_matchbox/assets/css/normalize.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.3/bw_matchbox/assets/css/processes-list.css` & `bw_matchbox-1.0.4/bw_matchbox/assets/css/processes-list.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.3/bw_matchbox/assets/css/skeleton.css` & `bw_matchbox-1.0.4/bw_matchbox/assets/css/skeleton.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.3/bw_matchbox/assets/css/tooltip.css` & `bw_matchbox-1.0.4/bw_matchbox/assets/css/tooltip.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.3/bw_matchbox/assets/images/favicon.ico` & `bw_matchbox-1.0.4/bw_matchbox/assets/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.3/bw_matchbox/assets/js/Compare/CompareCore.js` & `bw_matchbox-1.0.4/bw_matchbox/assets/js/Compare/CompareCore.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.3/bw_matchbox/assets/js/Compare/CompareProxyDialogModal.js` & `bw_matchbox-1.0.4/bw_matchbox/assets/js/Compare/CompareProxyDialogModal.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.3/bw_matchbox/assets/js/Compare/CompareRowClick.js` & `bw_matchbox-1.0.4/bw_matchbox/assets/js/Compare/CompareRowClick.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.3/bw_matchbox/assets/js/Compare/CompareRowsHelpers.js` & `bw_matchbox-1.0.4/bw_matchbox/assets/js/Compare/CompareRowsHelpers.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.3/bw_matchbox/assets/js/ProcessDetail/ProcessDetail.js` & `bw_matchbox-1.0.4/bw_matchbox/assets/js/ProcessDetail/ProcessDetail.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.3/bw_matchbox/assets/js/ProcessesList/ProcessesList.js` & `bw_matchbox-1.0.4/bw_matchbox/assets/js/ProcessesList/ProcessesList.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.3/bw_matchbox/assets/js/ProcessesList/ProcessesListConstants.js` & `bw_matchbox-1.0.4/bw_matchbox/assets/js/ProcessesList/ProcessesListConstants.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.3/bw_matchbox/assets/js/ProcessesList/ProcessesListData.js` & `bw_matchbox-1.0.4/bw_matchbox/assets/js/ProcessesList/ProcessesListData.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.3/bw_matchbox/assets/js/ProcessesList/ProcessesListDataLoad.js` & `bw_matchbox-1.0.4/bw_matchbox/assets/js/ProcessesList/ProcessesListDataLoad.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.3/bw_matchbox/assets/js/ProcessesList/ProcessesListDataRender.js` & `bw_matchbox-1.0.4/bw_matchbox/assets/js/ProcessesList/ProcessesListDataRender.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -27,14 +27,15 @@
                 const {
                     id, // 726 (required!)
                     name, // 'Electronic capacitors, resistors, coils, transformers, connectors and other components (except  semiconductors and printed circuit assemblies); at manufacturer'
                     location, // 'United States'
                     unit, // ''
                     // details_url, // '/process/726'
                     // match_url, // '/match/726'
+                    match_type, // 'No direct match available'
                     matched, // false
                 } = rowData;
                 /* console.log('[ProcessesListDataRender:renderDataRow]: start', {
                  *   details_url, // '/process/726'
                  *   id, // 726
                  *   location, // 'United States'
                  *   match_url, // '/match/726'
@@ -42,15 +43,15 @@
                  *   name, // 'Electronic capacitors, resistors, coils, transformers, connectors and other components (except  semiconductors and printed circuit assemblies); at manufacturer'
                  *   unit, // ''
                  *   rowData,
                  * });
                  */
                 const matchUrl = '/match/' + id;
                 const matchButton = matched ?
-                    `<a class="button" href="${matchUrl || ''}"><i class="fa-solid fa-check"></i> EDIT</a>` :
+                    `<a class="button" href="${matchUrl || ''}"><i class="fa-solid fa-check"></i> ${match_type || 'EDIT'}</a>` :
                     `<a class="button button-primary" href="${
               matchUrl || ''
             }"><i class="fa-solid fa-circle-xmark"></i> ADD</a>`;
                 const content = `
           <tr>
             <td><div><a href="/process/${id || ''}">${name || ''}</a></div></td>
             <td><div>${location || ''}</div></td>
```

### Comparing `bw_matchbox-1.0.3/bw_matchbox/assets/js/ProcessesList/ProcessesListNodes.js` & `bw_matchbox-1.0.4/bw_matchbox/assets/js/ProcessesList/ProcessesListNodes.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.3/bw_matchbox/assets/js/ProcessesList/ProcessesListPagination.UNUSED.js` & `bw_matchbox-1.0.4/bw_matchbox/assets/js/ProcessesList/ProcessesListPagination.UNUSED.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.3/bw_matchbox/assets/js/ProcessesList/ProcessesListSearch.js` & `bw_matchbox-1.0.4/bw_matchbox/assets/js/ProcessesList/ProcessesListSearch.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.3/bw_matchbox/assets/js/ProcessesList/ProcessesListStates.js` & `bw_matchbox-1.0.4/bw_matchbox/assets/js/ProcessesList/ProcessesListStates.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.3/bw_matchbox/assets/js/common/CommonHelpers.js` & `bw_matchbox-1.0.4/bw_matchbox/assets/js/common/CommonHelpers.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.3/bw_matchbox/assets/js/common/CommonModal.js` & `bw_matchbox-1.0.4/bw_matchbox/assets/js/common/CommonModal.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.3/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.js` & `bw_matchbox-1.0.4/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.3/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.min.js` & `bw_matchbox-1.0.4/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.min.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.3/bw_matchbox/assets/templates/common-modal.html` & `bw_matchbox-1.0.4/bw_matchbox/assets/templates/common-modal.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.3/bw_matchbox/assets/templates/compare.html` & `bw_matchbox-1.0.4/bw_matchbox/assets/templates/compare.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.3/bw_matchbox/assets/templates/databases.html` & `bw_matchbox-1.0.4/bw_matchbox/assets/templates/databases.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.3/bw_matchbox/assets/templates/header.html` & `bw_matchbox-1.0.4/bw_matchbox/assets/templates/header.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.3/bw_matchbox/assets/templates/index.html` & `bw_matchbox-1.0.4/bw_matchbox/assets/templates/index.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.3/bw_matchbox/assets/templates/match-status.html` & `bw_matchbox-1.0.4/bw_matchbox/assets/templates/match-status.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.3/bw_matchbox/assets/templates/match.html` & `bw_matchbox-1.0.4/bw_matchbox/assets/templates/match.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.3/bw_matchbox/assets/templates/navigation.html` & `bw_matchbox-1.0.4/bw_matchbox/assets/templates/navigation.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.3/bw_matchbox/assets/templates/process_detail.html` & `bw_matchbox-1.0.4/bw_matchbox/assets/templates/process_detail.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.3/bw_matchbox/assets/templates/project.html` & `bw_matchbox-1.0.4/bw_matchbox/assets/templates/project.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.3/bw_matchbox/assets/templates/search.html` & `bw_matchbox-1.0.4/bw_matchbox/assets/templates/search.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.3/bw_matchbox/assets/templates/search_result.html` & `bw_matchbox-1.0.4/bw_matchbox/assets/templates/search_result.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.3/bw_matchbox/assets/templates/select_files.html` & `bw_matchbox-1.0.4/bw_matchbox/assets/templates/select_files.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.3/bw_matchbox/bin/matchbox.py` & `bw_matchbox-1.0.4/bw_matchbox/bin/matchbox.py`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.3/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-mining.json` & `bw_matchbox-1.0.4/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-mining.json`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.3/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-string-matching.json` & `bw_matchbox-1.0.4/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-string-matching.json`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.3/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-transport.json` & `bw_matchbox-1.0.4/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-transport.json`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.3/bw_matchbox/data/dare.json` & `bw_matchbox-1.0.4/bw_matchbox/data/dare.json`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.3/bw_matchbox/utils.py` & `bw_matchbox-1.0.4/bw_matchbox/utils.py`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.3/bw_matchbox/webapp.py` & `bw_matchbox-1.0.4/bw_matchbox/webapp.py`

 * *Files 4% similar despite different names*

```diff
@@ -341,33 +341,72 @@
             if limit:
                 qs = qs.limit(limit)
         else:
             qs = apply_filter_to_qs(qs, filter_arg)
             total_records = len(qs)
             qs = apply_limit_offset(qs, limit, offset)
 
+    for obj in qs:
+        print("match_type", obj.data.get("match_type"))
+        print("data:", obj.data)
+
     payload = {
         "total_records": total_records,
         "data": [
             {
                 "details_url": flask.url_for("process_detail", id=obj.id),
                 "match_url": flask.url_for("match", source=obj.id),
                 "matched": bool(obj.data.get("matched")),
+                "match_type": get_match_type_for_source_process(obj),
                 "waitlist": bool(obj.data.get("waitlist")),
                 "id": obj.id,
                 "name": obj.name,
                 "location": obj.location,
                 "unit": obj.data["unit"],
             }
             for obj in qs
         ],
     }
     return flask.jsonify(payload)
 
 
+mwmarortalf = "Match with market and replace or remove transport and loss factor"
+
+MATCH_TYPE_ABBREVIATIONS = {
+    "No direct match available": "No direct match",
+    "Direct match with near-identical data": "Near-identical data",
+    "Match with updated data": "Updated data",
+    "Match with updated data and adding source transport": "Updated data w/ src trans",
+    "Match with market and replace or remove transport": "Market w/ diff trans",
+    mwmarortalf: "Market w/ diff trans loss",
+    "Equivalent datasets after modification": "Modifications",
+    "Replace aggregated with unit process": "Replace aggregated",
+    "Unknown": "Unknown",
+}
+
+
+def get_match_type_for_source_process(node):
+    if hasattr(node, "data"):
+        if node.data.get("proxy_id"):
+            mt = bd.get_node(id=node.data["proxy_id"]).get("match_type")
+            return MATCH_TYPE_ABBREVIATIONS[
+                matchbox_app.config["mb_match_types"].get(mt, "Unknown")
+            ]
+        else:
+            return "Unknown"
+    else:
+        mt = bd.get_node(id=node["proxy_id"]).get("match_type")
+        if not mt or mt == "0":
+            return "Unknown"
+        else:
+            return MATCH_TYPE_ABBREVIATIONS[
+                matchbox_app.config["mb_match_types"].get(mt, "Unknown")
+            ]
+
+
 # @matchbox_app.route("/match-status", methods=["GET"])
 # @auth.login_required
 # def match_status():
 #     crud = {}
 #     status = {}
 #     failed = []
```

### Comparing `bw_matchbox-1.0.3/bw_matchbox.egg-info/PKG-INFO` & `bw_matchbox-1.0.4/bw_matchbox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bw-matchbox
-Version: 1.0.3
+Version: 1.0.4
 Summary: Browser to match Brightway databases
 Home-page: https://github.com/cauldron/bw_matchbox
 Author: Chris Mutel
 Author-email: <cmutel@gmail.com>
 Maintainer: Chris Mutel
 Maintainer-email: <cmutel@gmail.com>
 License: MIT
```

### Comparing `bw_matchbox-1.0.3/bw_matchbox.egg-info/SOURCES.txt` & `bw_matchbox-1.0.4/bw_matchbox.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,14 @@
 ./bw_matchbox/assets/templates/select_files.html
 ./bw_matchbox/bin/__init__.py
 ./bw_matchbox/bin/matchbox.py
 ./bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-mining.json
 ./bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-string-matching.json
 ./bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-transport.json
 ./bw_matchbox/data/dare.json
-./docs/conf.py
 bw_matchbox/VERSION
 bw_matchbox.egg-info/PKG-INFO
 bw_matchbox.egg-info/SOURCES.txt
 bw_matchbox.egg-info/dependency_links.txt
 bw_matchbox.egg-info/entry_points.txt
 bw_matchbox.egg-info/not-zip-safe
 bw_matchbox.egg-info/requires.txt
```

### Comparing `bw_matchbox-1.0.3/setup.cfg` & `bw_matchbox-1.0.4/setup.cfg`

 * *Files identical despite different names*

