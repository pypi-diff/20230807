# Comparing `tmp/bw_matchbox-1.0.1.tar.gz` & `tmp/bw_matchbox-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bw_matchbox-1.0.1.tar", last modified: Mon Aug  7 13:45:04 2023, max compression
+gzip compressed data, was "bw_matchbox-1.0.2.tar", last modified: Mon Aug  7 17:25:20 2023, max compression
```

## Comparing `bw_matchbox-1.0.1.tar` & `bw_matchbox-1.0.2.tar`

### file list

```diff
@@ -1,83 +1,86 @@
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-07 13:45:04.167070 bw_matchbox-1.0.1/
--rw-r--r--   0 cmutel     (501) staff       (20)     1067 2023-07-24 11:16:50.000000 bw_matchbox-1.0.1/LICENSE
--rw-r--r--   0 cmutel     (501) staff       (20)      226 2023-08-03 14:06:22.000000 bw_matchbox-1.0.1/MANIFEST.in
--rw-r--r--   0 cmutel     (501) staff       (20)     6361 2023-08-07 13:45:04.167162 bw_matchbox-1.0.1/PKG-INFO
--rw-r--r--   0 cmutel     (501) staff       (20)     5337 2023-08-05 07:08:03.000000 bw_matchbox-1.0.1/README.md
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-07 13:45:04.152833 bw_matchbox-1.0.1/bw_matchbox/
--rw-r--r--   0 cmutel     (501) staff       (20)        6 2023-08-07 13:44:20.000000 bw_matchbox-1.0.1/bw_matchbox/VERSION
--rw-r--r--   0 cmutel     (501) staff       (20)      215 2023-08-03 14:06:22.000000 bw_matchbox-1.0.1/bw_matchbox/__init__.py
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-07 13:45:04.150853 bw_matchbox-1.0.1/bw_matchbox/assets/
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-07 13:45:04.155127 bw_matchbox-1.0.1/bw_matchbox/assets/css/
--rw-r--r--   0 cmutel     (501) staff       (20)     3297 2023-08-07 06:34:48.000000 bw_matchbox-1.0.1/bw_matchbox/assets/css/common-modal.css
--rw-r--r--   0 cmutel     (501) staff       (20)     1922 2023-08-07 06:34:48.000000 bw_matchbox-1.0.1/bw_matchbox/assets/css/common.css
--rw-r--r--   0 cmutel     (501) staff       (20)     4256 2023-08-07 06:34:48.000000 bw_matchbox-1.0.1/bw_matchbox/assets/css/compare.css
--rw-r--r--   0 cmutel     (501) staff       (20)      640 2023-08-05 06:10:27.000000 bw_matchbox-1.0.1/bw_matchbox/assets/css/customizations.css
--rw-r--r--   0 cmutel     (501) staff       (20)     1392 2023-08-05 06:10:27.000000 bw_matchbox-1.0.1/bw_matchbox/assets/css/fixed-table.css
--rw-r--r--   0 cmutel     (501) staff       (20)     7618 2023-08-01 11:28:52.000000 bw_matchbox-1.0.1/bw_matchbox/assets/css/normalize.css
--rw-r--r--   0 cmutel     (501) staff       (20)     4315 2023-08-06 09:58:28.000000 bw_matchbox-1.0.1/bw_matchbox/assets/css/processes-list.css
--rw-r--r--   0 cmutel     (501) staff       (20)    11556 2023-08-01 11:28:52.000000 bw_matchbox-1.0.1/bw_matchbox/assets/css/skeleton.css
--rw-r--r--   0 cmutel     (501) staff       (20)      916 2023-08-01 11:28:52.000000 bw_matchbox-1.0.1/bw_matchbox/assets/css/tooltip.css
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-07 13:45:04.155381 bw_matchbox-1.0.1/bw_matchbox/assets/images/
--rw-r--r--   0 cmutel     (501) staff       (20)    32038 2023-07-24 11:16:50.000000 bw_matchbox-1.0.1/bw_matchbox/assets/images/favicon.ico
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-07 13:45:04.150746 bw_matchbox-1.0.1/bw_matchbox/assets/js/
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-07 13:45:04.156309 bw_matchbox-1.0.1/bw_matchbox/assets/js/Compare/
--rw-r--r--   0 cmutel     (501) staff       (20)    20293 2023-08-07 06:34:48.000000 bw_matchbox-1.0.1/bw_matchbox/assets/js/Compare/CompareCore.js
--rw-r--r--   0 cmutel     (501) staff       (20)     6194 2023-08-07 06:34:48.000000 bw_matchbox-1.0.1/bw_matchbox/assets/js/Compare/CompareProxyDialogModal.js
--rw-r--r--   0 cmutel     (501) staff       (20)     1272 2023-08-05 06:10:27.000000 bw_matchbox-1.0.1/bw_matchbox/assets/js/Compare/CompareRowClick.js
--rw-r--r--   0 cmutel     (501) staff       (20)    12879 2023-08-07 06:34:48.000000 bw_matchbox-1.0.1/bw_matchbox/assets/js/Compare/CompareRowsHelpers.js
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-07 13:45:04.158335 bw_matchbox-1.0.1/bw_matchbox/assets/js/ProcessesList/
--rw-r--r--   0 cmutel     (501) staff       (20)     4388 2023-08-06 09:58:28.000000 bw_matchbox-1.0.1/bw_matchbox/assets/js/ProcessesList/ProcessesList.js
--rw-r--r--   0 cmutel     (501) staff       (20)      885 2023-08-06 09:58:28.000000 bw_matchbox-1.0.1/bw_matchbox/assets/js/ProcessesList/ProcessesListConstants.js
--rw-r--r--   0 cmutel     (501) staff       (20)     1452 2023-08-06 09:58:28.000000 bw_matchbox-1.0.1/bw_matchbox/assets/js/ProcessesList/ProcessesListData.js
--rw-r--r--   0 cmutel     (501) staff       (20)     5632 2023-08-06 09:58:28.000000 bw_matchbox-1.0.1/bw_matchbox/assets/js/ProcessesList/ProcessesListDataLoad.js
--rw-r--r--   0 cmutel     (501) staff       (20)     3447 2023-08-06 09:58:28.000000 bw_matchbox-1.0.1/bw_matchbox/assets/js/ProcessesList/ProcessesListDataRender.js
--rw-r--r--   0 cmutel     (501) staff       (20)     1081 2023-08-06 09:58:28.000000 bw_matchbox-1.0.1/bw_matchbox/assets/js/ProcessesList/ProcessesListNodes.js
--rw-r--r--   0 cmutel     (501) staff       (20)     4862 2023-08-06 09:58:28.000000 bw_matchbox-1.0.1/bw_matchbox/assets/js/ProcessesList/ProcessesListPagination.UNUSED.js
--rw-r--r--   0 cmutel     (501) staff       (20)     3321 2023-08-06 09:58:28.000000 bw_matchbox-1.0.1/bw_matchbox/assets/js/ProcessesList/ProcessesListSearch.js
--rw-r--r--   0 cmutel     (501) staff       (20)     9995 2023-08-06 09:58:28.000000 bw_matchbox-1.0.1/bw_matchbox/assets/js/ProcessesList/ProcessesListStates.js
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-07 13:45:04.158711 bw_matchbox-1.0.1/bw_matchbox/assets/js/common/
--rw-r--r--   0 cmutel     (501) staff       (20)     5634 2023-08-05 06:10:27.000000 bw_matchbox-1.0.1/bw_matchbox/assets/js/common/CommonHelpers.js
--rw-r--r--   0 cmutel     (501) staff       (20)     5781 2023-08-06 13:56:54.000000 bw_matchbox-1.0.1/bw_matchbox/assets/js/common/CommonModal.js
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-07 13:45:04.150792 bw_matchbox-1.0.1/bw_matchbox/assets/js/libs/
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-07 13:45:04.159306 bw_matchbox-1.0.1/bw_matchbox/assets/js/libs/ym/
--rw-r--r--   0 cmutel     (501) staff       (20)    13286 2023-08-03 14:06:22.000000 bw_matchbox-1.0.1/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.js
--rw-r--r--   0 cmutel     (501) staff       (20)     6018 2023-08-03 14:06:22.000000 bw_matchbox-1.0.1/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.min.js
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-07 13:45:04.162797 bw_matchbox-1.0.1/bw_matchbox/assets/templates/
--rw-r--r--   0 cmutel     (501) staff       (20)      756 2023-08-05 06:10:27.000000 bw_matchbox-1.0.1/bw_matchbox/assets/templates/common-modal.html
--rw-r--r--   0 cmutel     (501) staff       (20)     3880 2023-08-07 06:34:48.000000 bw_matchbox-1.0.1/bw_matchbox/assets/templates/compare.html
--rw-r--r--   0 cmutel     (501) staff       (20)     2681 2023-08-05 07:08:03.000000 bw_matchbox-1.0.1/bw_matchbox/assets/templates/databases.html
--rw-r--r--   0 cmutel     (501) staff       (20)      461 2023-07-24 11:16:50.000000 bw_matchbox-1.0.1/bw_matchbox/assets/templates/expand.html
--rw-r--r--   0 cmutel     (501) staff       (20)       16 2023-07-24 11:16:50.000000 bw_matchbox-1.0.1/bw_matchbox/assets/templates/footer.html
--rw-r--r--   0 cmutel     (501) staff       (20)     2666 2023-08-05 06:10:27.000000 bw_matchbox-1.0.1/bw_matchbox/assets/templates/header.html
--rw-r--r--   0 cmutel     (501) staff       (20)     6969 2023-08-06 09:58:28.000000 bw_matchbox-1.0.1/bw_matchbox/assets/templates/index.html
--rw-r--r--   0 cmutel     (501) staff       (20)      733 2023-07-24 11:16:50.000000 bw_matchbox-1.0.1/bw_matchbox/assets/templates/match-status.html
--rw-r--r--   0 cmutel     (501) staff       (20)     1713 2023-08-07 13:23:46.000000 bw_matchbox-1.0.1/bw_matchbox/assets/templates/match.html
--rw-r--r--   0 cmutel     (501) staff       (20)      734 2023-08-05 07:08:03.000000 bw_matchbox-1.0.1/bw_matchbox/assets/templates/navigation.html
--rw-r--r--   0 cmutel     (501) staff       (20)     5830 2023-08-07 13:43:30.000000 bw_matchbox-1.0.1/bw_matchbox/assets/templates/process_detail.html
--rw-r--r--   0 cmutel     (501) staff       (20)      599 2023-07-24 11:16:50.000000 bw_matchbox-1.0.1/bw_matchbox/assets/templates/project.html
--rw-r--r--   0 cmutel     (501) staff       (20)      412 2023-08-01 11:28:52.000000 bw_matchbox-1.0.1/bw_matchbox/assets/templates/search-embedded.html
--rw-r--r--   0 cmutel     (501) staff       (20)      850 2023-07-24 11:16:50.000000 bw_matchbox-1.0.1/bw_matchbox/assets/templates/search.html
--rw-r--r--   0 cmutel     (501) staff       (20)      947 2023-07-24 11:16:50.000000 bw_matchbox-1.0.1/bw_matchbox/assets/templates/search_result.html
--rw-r--r--   0 cmutel     (501) staff       (20)     1243 2023-07-24 11:16:50.000000 bw_matchbox-1.0.1/bw_matchbox/assets/templates/select_files.html
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-07 13:45:04.163043 bw_matchbox-1.0.1/bw_matchbox/bin/
--rw-r--r--   0 cmutel     (501) staff       (20)        0 2023-07-24 11:16:50.000000 bw_matchbox-1.0.1/bw_matchbox/bin/__init__.py
--rw-r--r--   0 cmutel     (501) staff       (20)     2692 2023-08-05 18:47:38.000000 bw_matchbox-1.0.1/bw_matchbox/bin/matchbox.py
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-07 13:45:04.164508 bw_matchbox-1.0.1/bw_matchbox/data/
--rw-r--r--   0 cmutel     (501) staff       (20)   123246 2023-08-03 14:06:22.000000 bw_matchbox-1.0.1/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-mining.json
--rw-r--r--   0 cmutel     (501) staff       (20)    93862 2023-07-24 11:16:50.000000 bw_matchbox-1.0.1/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-string-matching.json
--rw-r--r--   0 cmutel     (501) staff       (20)   116072 2023-08-03 14:06:22.000000 bw_matchbox-1.0.1/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-transport.json
--rw-r--r--   0 cmutel     (501) staff       (20)      603 2023-07-24 11:16:50.000000 bw_matchbox-1.0.1/bw_matchbox/data/dare.json
--rw-r--r--   0 cmutel     (501) staff       (20)     2204 2023-08-07 13:25:08.000000 bw_matchbox-1.0.1/bw_matchbox/utils.py
--rw-r--r--   0 cmutel     (501) staff       (20)    22989 2023-08-07 13:42:11.000000 bw_matchbox-1.0.1/bw_matchbox/webapp.py
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-07 13:45:04.165585 bw_matchbox-1.0.1/bw_matchbox.egg-info/
--rw-r--r--   0 cmutel     (501) staff       (20)     6361 2023-08-07 13:45:04.000000 bw_matchbox-1.0.1/bw_matchbox.egg-info/PKG-INFO
--rw-r--r--   0 cmutel     (501) staff       (20)     5090 2023-08-07 13:45:04.000000 bw_matchbox-1.0.1/bw_matchbox.egg-info/SOURCES.txt
--rw-r--r--   0 cmutel     (501) staff       (20)        1 2023-08-07 13:45:04.000000 bw_matchbox-1.0.1/bw_matchbox.egg-info/dependency_links.txt
--rw-r--r--   0 cmutel     (501) staff       (20)       59 2023-08-07 13:45:04.000000 bw_matchbox-1.0.1/bw_matchbox.egg-info/entry_points.txt
--rw-r--r--   0 cmutel     (501) staff       (20)        1 2023-07-24 11:26:00.000000 bw_matchbox-1.0.1/bw_matchbox.egg-info/not-zip-safe
--rw-r--r--   0 cmutel     (501) staff       (20)      167 2023-08-07 13:45:04.000000 bw_matchbox-1.0.1/bw_matchbox.egg-info/requires.txt
--rw-r--r--   0 cmutel     (501) staff       (20)       12 2023-08-07 13:45:04.000000 bw_matchbox-1.0.1/bw_matchbox.egg-info/top_level.txt
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-07 13:45:04.164644 bw_matchbox-1.0.1/docs/
--rw-r--r--   0 cmutel     (501) staff       (20)     1145 2023-07-24 11:16:50.000000 bw_matchbox-1.0.1/docs/conf.py
--rw-r--r--   0 cmutel     (501) staff       (20)       87 2023-07-24 11:16:50.000000 bw_matchbox-1.0.1/pyproject.toml
--rw-r--r--   0 cmutel     (501) staff       (20)     1900 2023-08-07 13:45:04.167573 bw_matchbox-1.0.1/setup.cfg
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-07 17:25:20.878497 bw_matchbox-1.0.2/
+-rw-r--r--   0 cmutel     (501) staff       (20)     1067 2023-07-24 11:16:50.000000 bw_matchbox-1.0.2/LICENSE
+-rw-r--r--   0 cmutel     (501) staff       (20)      226 2023-08-03 14:06:22.000000 bw_matchbox-1.0.2/MANIFEST.in
+-rw-r--r--   0 cmutel     (501) staff       (20)     6361 2023-08-07 17:25:20.878569 bw_matchbox-1.0.2/PKG-INFO
+-rw-r--r--   0 cmutel     (501) staff       (20)     5337 2023-08-05 07:08:03.000000 bw_matchbox-1.0.2/README.md
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-07 17:25:20.864828 bw_matchbox-1.0.2/bw_matchbox/
+-rw-r--r--   0 cmutel     (501) staff       (20)        6 2023-08-07 17:24:53.000000 bw_matchbox-1.0.2/bw_matchbox/VERSION
+-rw-r--r--   0 cmutel     (501) staff       (20)      215 2023-08-03 14:06:22.000000 bw_matchbox-1.0.2/bw_matchbox/__init__.py
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-07 17:25:20.862976 bw_matchbox-1.0.2/bw_matchbox/assets/
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-07 17:25:20.867238 bw_matchbox-1.0.2/bw_matchbox/assets/css/
+-rw-r--r--   0 cmutel     (501) staff       (20)     4266 2023-08-07 17:24:49.000000 bw_matchbox-1.0.2/bw_matchbox/assets/css/common-modal.css
+-rw-r--r--   0 cmutel     (501) staff       (20)     1922 2023-08-07 06:34:48.000000 bw_matchbox-1.0.2/bw_matchbox/assets/css/common.css
+-rw-r--r--   0 cmutel     (501) staff       (20)     4256 2023-08-07 13:49:10.000000 bw_matchbox-1.0.2/bw_matchbox/assets/css/compare.css
+-rw-r--r--   0 cmutel     (501) staff       (20)      640 2023-08-05 06:10:27.000000 bw_matchbox-1.0.2/bw_matchbox/assets/css/customizations.css
+-rw-r--r--   0 cmutel     (501) staff       (20)     1392 2023-08-05 06:10:27.000000 bw_matchbox-1.0.2/bw_matchbox/assets/css/fixed-table.css
+-rw-r--r--   0 cmutel     (501) staff       (20)     7618 2023-08-01 11:28:52.000000 bw_matchbox-1.0.2/bw_matchbox/assets/css/normalize.css
+-rw-r--r--   0 cmutel     (501) staff       (20)       99 2023-08-07 17:24:49.000000 bw_matchbox-1.0.2/bw_matchbox/assets/css/process-detail.css
+-rw-r--r--   0 cmutel     (501) staff       (20)     4315 2023-08-06 09:58:28.000000 bw_matchbox-1.0.2/bw_matchbox/assets/css/processes-list.css
+-rw-r--r--   0 cmutel     (501) staff       (20)    11556 2023-08-01 11:28:52.000000 bw_matchbox-1.0.2/bw_matchbox/assets/css/skeleton.css
+-rw-r--r--   0 cmutel     (501) staff       (20)      916 2023-08-01 11:28:52.000000 bw_matchbox-1.0.2/bw_matchbox/assets/css/tooltip.css
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-07 17:25:20.867458 bw_matchbox-1.0.2/bw_matchbox/assets/images/
+-rw-r--r--   0 cmutel     (501) staff       (20)    32038 2023-07-24 11:16:50.000000 bw_matchbox-1.0.2/bw_matchbox/assets/images/favicon.ico
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-07 17:25:20.862867 bw_matchbox-1.0.2/bw_matchbox/assets/js/
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-07 17:25:20.868512 bw_matchbox-1.0.2/bw_matchbox/assets/js/Compare/
+-rw-r--r--   0 cmutel     (501) staff       (20)    20293 2023-08-07 06:34:48.000000 bw_matchbox-1.0.2/bw_matchbox/assets/js/Compare/CompareCore.js
+-rw-r--r--   0 cmutel     (501) staff       (20)     6250 2023-08-07 17:24:49.000000 bw_matchbox-1.0.2/bw_matchbox/assets/js/Compare/CompareProxyDialogModal.js
+-rw-r--r--   0 cmutel     (501) staff       (20)     1272 2023-08-05 06:10:27.000000 bw_matchbox-1.0.2/bw_matchbox/assets/js/Compare/CompareRowClick.js
+-rw-r--r--   0 cmutel     (501) staff       (20)    12879 2023-08-07 06:34:48.000000 bw_matchbox-1.0.2/bw_matchbox/assets/js/Compare/CompareRowsHelpers.js
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-07 17:25:20.868672 bw_matchbox-1.0.2/bw_matchbox/assets/js/ProcessDetail/
+-rw-r--r--   0 cmutel     (501) staff       (20)     7467 2023-08-07 17:24:49.000000 bw_matchbox-1.0.2/bw_matchbox/assets/js/ProcessDetail/ProcessDetail.js
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-07 17:25:20.870494 bw_matchbox-1.0.2/bw_matchbox/assets/js/ProcessesList/
+-rw-r--r--   0 cmutel     (501) staff       (20)     4388 2023-08-06 09:58:28.000000 bw_matchbox-1.0.2/bw_matchbox/assets/js/ProcessesList/ProcessesList.js
+-rw-r--r--   0 cmutel     (501) staff       (20)      885 2023-08-06 09:58:28.000000 bw_matchbox-1.0.2/bw_matchbox/assets/js/ProcessesList/ProcessesListConstants.js
+-rw-r--r--   0 cmutel     (501) staff       (20)     1452 2023-08-06 09:58:28.000000 bw_matchbox-1.0.2/bw_matchbox/assets/js/ProcessesList/ProcessesListData.js
+-rw-r--r--   0 cmutel     (501) staff       (20)     5068 2023-08-07 17:24:49.000000 bw_matchbox-1.0.2/bw_matchbox/assets/js/ProcessesList/ProcessesListDataLoad.js
+-rw-r--r--   0 cmutel     (501) staff       (20)     3447 2023-08-06 09:58:28.000000 bw_matchbox-1.0.2/bw_matchbox/assets/js/ProcessesList/ProcessesListDataRender.js
+-rw-r--r--   0 cmutel     (501) staff       (20)     1081 2023-08-06 09:58:28.000000 bw_matchbox-1.0.2/bw_matchbox/assets/js/ProcessesList/ProcessesListNodes.js
+-rw-r--r--   0 cmutel     (501) staff       (20)     4862 2023-08-06 09:58:28.000000 bw_matchbox-1.0.2/bw_matchbox/assets/js/ProcessesList/ProcessesListPagination.UNUSED.js
+-rw-r--r--   0 cmutel     (501) staff       (20)     3321 2023-08-06 09:58:28.000000 bw_matchbox-1.0.2/bw_matchbox/assets/js/ProcessesList/ProcessesListSearch.js
+-rw-r--r--   0 cmutel     (501) staff       (20)     9995 2023-08-06 09:58:28.000000 bw_matchbox-1.0.2/bw_matchbox/assets/js/ProcessesList/ProcessesListStates.js
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-07 17:25:20.871003 bw_matchbox-1.0.2/bw_matchbox/assets/js/common/
+-rw-r--r--   0 cmutel     (501) staff       (20)     5634 2023-08-05 06:10:27.000000 bw_matchbox-1.0.2/bw_matchbox/assets/js/common/CommonHelpers.js
+-rw-r--r--   0 cmutel     (501) staff       (20)     8875 2023-08-07 17:24:49.000000 bw_matchbox-1.0.2/bw_matchbox/assets/js/common/CommonModal.js
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-07 17:25:20.862913 bw_matchbox-1.0.2/bw_matchbox/assets/js/libs/
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-07 17:25:20.871447 bw_matchbox-1.0.2/bw_matchbox/assets/js/libs/ym/
+-rw-r--r--   0 cmutel     (501) staff       (20)    13286 2023-08-03 14:06:22.000000 bw_matchbox-1.0.2/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.js
+-rw-r--r--   0 cmutel     (501) staff       (20)     6018 2023-08-03 14:06:22.000000 bw_matchbox-1.0.2/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.min.js
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-07 17:25:20.874397 bw_matchbox-1.0.2/bw_matchbox/assets/templates/
+-rw-r--r--   0 cmutel     (501) staff       (20)      756 2023-08-05 06:10:27.000000 bw_matchbox-1.0.2/bw_matchbox/assets/templates/common-modal.html
+-rw-r--r--   0 cmutel     (501) staff       (20)     3916 2023-08-07 17:24:49.000000 bw_matchbox-1.0.2/bw_matchbox/assets/templates/compare.html
+-rw-r--r--   0 cmutel     (501) staff       (20)     2681 2023-08-05 07:08:03.000000 bw_matchbox-1.0.2/bw_matchbox/assets/templates/databases.html
+-rw-r--r--   0 cmutel     (501) staff       (20)      461 2023-07-24 11:16:50.000000 bw_matchbox-1.0.2/bw_matchbox/assets/templates/expand.html
+-rw-r--r--   0 cmutel     (501) staff       (20)       16 2023-07-24 11:16:50.000000 bw_matchbox-1.0.2/bw_matchbox/assets/templates/footer.html
+-rw-r--r--   0 cmutel     (501) staff       (20)     2666 2023-08-05 06:10:27.000000 bw_matchbox-1.0.2/bw_matchbox/assets/templates/header.html
+-rw-r--r--   0 cmutel     (501) staff       (20)     6983 2023-08-07 17:24:49.000000 bw_matchbox-1.0.2/bw_matchbox/assets/templates/index.html
+-rw-r--r--   0 cmutel     (501) staff       (20)      733 2023-07-24 11:16:50.000000 bw_matchbox-1.0.2/bw_matchbox/assets/templates/match-status.html
+-rw-r--r--   0 cmutel     (501) staff       (20)     1713 2023-08-07 13:23:46.000000 bw_matchbox-1.0.2/bw_matchbox/assets/templates/match.html
+-rw-r--r--   0 cmutel     (501) staff       (20)      734 2023-08-05 07:08:03.000000 bw_matchbox-1.0.2/bw_matchbox/assets/templates/navigation.html
+-rw-r--r--   0 cmutel     (501) staff       (20)     5826 2023-08-07 17:24:49.000000 bw_matchbox-1.0.2/bw_matchbox/assets/templates/process_detail.html
+-rw-r--r--   0 cmutel     (501) staff       (20)      599 2023-07-24 11:16:50.000000 bw_matchbox-1.0.2/bw_matchbox/assets/templates/project.html
+-rw-r--r--   0 cmutel     (501) staff       (20)      412 2023-08-01 11:28:52.000000 bw_matchbox-1.0.2/bw_matchbox/assets/templates/search-embedded.html
+-rw-r--r--   0 cmutel     (501) staff       (20)      850 2023-07-24 11:16:50.000000 bw_matchbox-1.0.2/bw_matchbox/assets/templates/search.html
+-rw-r--r--   0 cmutel     (501) staff       (20)      947 2023-07-24 11:16:50.000000 bw_matchbox-1.0.2/bw_matchbox/assets/templates/search_result.html
+-rw-r--r--   0 cmutel     (501) staff       (20)     1243 2023-07-24 11:16:50.000000 bw_matchbox-1.0.2/bw_matchbox/assets/templates/select_files.html
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-07 17:25:20.874678 bw_matchbox-1.0.2/bw_matchbox/bin/
+-rw-r--r--   0 cmutel     (501) staff       (20)        0 2023-07-24 11:16:50.000000 bw_matchbox-1.0.2/bw_matchbox/bin/__init__.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     2692 2023-08-05 18:47:38.000000 bw_matchbox-1.0.2/bw_matchbox/bin/matchbox.py
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-07 17:25:20.876158 bw_matchbox-1.0.2/bw_matchbox/data/
+-rw-r--r--   0 cmutel     (501) staff       (20)   123246 2023-08-03 14:06:22.000000 bw_matchbox-1.0.2/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-mining.json
+-rw-r--r--   0 cmutel     (501) staff       (20)    93862 2023-07-24 11:16:50.000000 bw_matchbox-1.0.2/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-string-matching.json
+-rw-r--r--   0 cmutel     (501) staff       (20)   116072 2023-08-03 14:06:22.000000 bw_matchbox-1.0.2/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-transport.json
+-rw-r--r--   0 cmutel     (501) staff       (20)      603 2023-07-24 11:16:50.000000 bw_matchbox-1.0.2/bw_matchbox/data/dare.json
+-rw-r--r--   0 cmutel     (501) staff       (20)     2204 2023-08-07 13:25:08.000000 bw_matchbox-1.0.2/bw_matchbox/utils.py
+-rw-r--r--   0 cmutel     (501) staff       (20)    22989 2023-08-07 13:42:11.000000 bw_matchbox-1.0.2/bw_matchbox/webapp.py
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-07 17:25:20.877160 bw_matchbox-1.0.2/bw_matchbox.egg-info/
+-rw-r--r--   0 cmutel     (501) staff       (20)     6361 2023-08-07 17:25:20.000000 bw_matchbox-1.0.2/bw_matchbox.egg-info/PKG-INFO
+-rw-r--r--   0 cmutel     (501) staff       (20)     5284 2023-08-07 17:25:20.000000 bw_matchbox-1.0.2/bw_matchbox.egg-info/SOURCES.txt
+-rw-r--r--   0 cmutel     (501) staff       (20)        1 2023-08-07 17:25:20.000000 bw_matchbox-1.0.2/bw_matchbox.egg-info/dependency_links.txt
+-rw-r--r--   0 cmutel     (501) staff       (20)       59 2023-08-07 17:25:20.000000 bw_matchbox-1.0.2/bw_matchbox.egg-info/entry_points.txt
+-rw-r--r--   0 cmutel     (501) staff       (20)        1 2023-07-24 11:26:00.000000 bw_matchbox-1.0.2/bw_matchbox.egg-info/not-zip-safe
+-rw-r--r--   0 cmutel     (501) staff       (20)      167 2023-08-07 17:25:20.000000 bw_matchbox-1.0.2/bw_matchbox.egg-info/requires.txt
+-rw-r--r--   0 cmutel     (501) staff       (20)       12 2023-08-07 17:25:20.000000 bw_matchbox-1.0.2/bw_matchbox.egg-info/top_level.txt
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-07 17:25:20.876287 bw_matchbox-1.0.2/docs/
+-rw-r--r--   0 cmutel     (501) staff       (20)     1145 2023-07-24 11:16:50.000000 bw_matchbox-1.0.2/docs/conf.py
+-rw-r--r--   0 cmutel     (501) staff       (20)       87 2023-07-24 11:16:50.000000 bw_matchbox-1.0.2/pyproject.toml
+-rw-r--r--   0 cmutel     (501) staff       (20)     1900 2023-08-07 17:25:20.878966 bw_matchbox-1.0.2/setup.cfg
```

### Comparing `bw_matchbox-1.0.1/LICENSE` & `bw_matchbox-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.1/PKG-INFO` & `bw_matchbox-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bw_matchbox
-Version: 1.0.1
+Version: 1.0.2
 Summary: Browser to match Brightway databases
 Home-page: https://github.com/cauldron/bw_matchbox
 Author: Chris Mutel
 Author-email: <cmutel@gmail.com>
 Maintainer: Chris Mutel
 Maintainer-email: <cmutel@gmail.com>
 License: MIT
```

### Comparing `bw_matchbox-1.0.1/README.md` & `bw_matchbox-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.1/bw_matchbox/assets/css/common-modal.css` & `bw_matchbox-1.0.2/bw_matchbox/assets/css/common-modal.css`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+/* stylelint-disable selector-class-pattern */
+
 body.has-modal {
   /* Hide scrollbars when active modals are exist. */
   overflow: hidden;
 }
 
 .common-modal-wrapper .common-modal {
   z-index: 1; /* Sit on top */
@@ -49,22 +51,58 @@
 }
 /* Window geometry... */
 .common-modal-wrapper .common-modal-window {
   /* Default, narrow-screen: show in a full-screen mode */
   width: 100%;
   height: 100%;
 }
+/* Full width and height... */
+.common-modal-wrapper .common-modal-content-wrapper {
+  /* Make full window width default */
+  width: 100%;
+}
+/*
+.common-modal-wrapper .common-modal-window.fullWindowWidth .common-modal-content-wrapper {
+  width: 100%;
+}
+.common-modal-wrapper .common-modal-window.fullWindowHeight .common-modal-content-wrapper {
+  height: 100%;
+}
+*/
 @media (width >= 600px) and (height >= 400px) {
   .common-modal-wrapper .common-modal-window {
     /* Wide-screen: show as a window */
     border-radius: 8px;
     width: 80%;
     height: 80%;
     max-width: 1200px;
   }
+  /* Auto width and height... */
+  .common-modal-wrapper .common-modal-window.autoWidth {
+    width: auto;
+  }
+  .common-modal-wrapper .common-modal-window.autoHeight {
+    height: auto;
+  }
+}
+/* Adjust custom window sizes (sm, md, lg) */
+@media (width >= 600px) {
+  .common-modal-wrapper .common-modal-window.width-sm {
+    width: 400px;
+  }
+}
+@media (width >= 800px) {
+  .common-modal-wrapper .common-modal-window.width-md {
+    width: 700px;
+  }
+}
+@media (width >= 1120px) {
+  .common-modal-wrapper .common-modal-window.width-lg {
+    width: 900px;
+  }
 }
 
 /* Modal Content/Box */
 .common-modal-wrapper .common-modal-content {
   margin: auto; /* 15% from the top and centered */
   flex: 1;
   overflow: hidden;
```

### Comparing `bw_matchbox-1.0.1/bw_matchbox/assets/css/common.css` & `bw_matchbox-1.0.2/bw_matchbox/assets/css/common.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.1/bw_matchbox/assets/css/compare.css` & `bw_matchbox-1.0.2/bw_matchbox/assets/css/compare.css`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
   width: 50%;
   white-space: wrap;
 }
 .compare-table .cell-location {
   width: 30%;
 }
 .compare-table .cell-unit {
-  width: 2em;
+  width: 8em;
 }
 
 /* Action cell icons */
 .compare-table td.cell-actions {
   color: #e5e5e5;
 }
 .compare-table td.cell-actions a {
```

### Comparing `bw_matchbox-1.0.1/bw_matchbox/assets/css/customizations.css` & `bw_matchbox-1.0.2/bw_matchbox/assets/css/customizations.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.1/bw_matchbox/assets/css/fixed-table.css` & `bw_matchbox-1.0.2/bw_matchbox/assets/css/fixed-table.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.1/bw_matchbox/assets/css/normalize.css` & `bw_matchbox-1.0.2/bw_matchbox/assets/css/normalize.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.1/bw_matchbox/assets/css/processes-list.css` & `bw_matchbox-1.0.2/bw_matchbox/assets/css/processes-list.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.1/bw_matchbox/assets/css/skeleton.css` & `bw_matchbox-1.0.2/bw_matchbox/assets/css/skeleton.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.1/bw_matchbox/assets/css/tooltip.css` & `bw_matchbox-1.0.2/bw_matchbox/assets/css/tooltip.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.1/bw_matchbox/assets/images/favicon.ico` & `bw_matchbox-1.0.2/bw_matchbox/assets/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.1/bw_matchbox/assets/js/Compare/CompareCore.js` & `bw_matchbox-1.0.2/bw_matchbox/assets/js/Compare/CompareCore.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.1/bw_matchbox/assets/js/Compare/CompareProxyDialogModal.js` & `bw_matchbox-1.0.2/bw_matchbox/assets/js/Compare/CompareProxyDialogModal.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -154,22 +154,24 @@
                     exchanges: target_data,
                     source: source_id,
                     match_type,
                     comment,
                     name,
                 };
                 const url = '/create-proxy/';
-                console.log('[CompareProxyDialogModal:onSubmitButtonClick]', {
-                    target_data,
-                    source_id,
-                    match_type,
-                    comment,
-                    name,
-                    submissionData,
-                });
+                /* // DEBUG
+                 * console.log('[CompareProxyDialogModal:onSubmitButtonClick]', {
+                 *   target_data,
+                 *   source_id,
+                 *   match_type,
+                 *   comment,
+                 *   name,
+                 *   submissionData,
+                 * });
+                 */
                 fetch(url, {
                     method: 'POST',
                     redirect: 'follow',
                     headers: {
                         'Content-Type': 'application/json'
                     },
                     body: JSON.stringify(submissionData),
```

### Comparing `bw_matchbox-1.0.1/bw_matchbox/assets/js/Compare/CompareRowClick.js` & `bw_matchbox-1.0.2/bw_matchbox/assets/js/Compare/CompareRowClick.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.1/bw_matchbox/assets/js/Compare/CompareRowsHelpers.js` & `bw_matchbox-1.0.2/bw_matchbox/assets/js/Compare/CompareRowsHelpers.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.1/bw_matchbox/assets/js/ProcessesList/ProcessesList.js` & `bw_matchbox-1.0.2/bw_matchbox/assets/js/ProcessesList/ProcessesList.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.1/bw_matchbox/assets/js/ProcessesList/ProcessesListConstants.js` & `bw_matchbox-1.0.2/bw_matchbox/assets/js/ProcessesList/ProcessesListConstants.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.1/bw_matchbox/assets/js/ProcessesList/ProcessesListData.js` & `bw_matchbox-1.0.2/bw_matchbox/assets/js/ProcessesList/ProcessesListData.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.1/bw_matchbox/assets/js/ProcessesList/ProcessesListDataLoad.js` & `bw_matchbox-1.0.2/bw_matchbox/assets/js/ProcessesList/ProcessesListDataLoad.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -38,56 +38,54 @@
                     userDb,
                     searchValue,
                     sharedParams,
                     hasSearch
                 } =
                 ProcessesListData;
                 const {
-                    databases,
-                    // database, // UNUSED: #41: Using `databases` and `userDb`.
+                    databases
                 } = sharedParams;
                 const {
                     pageSize,
                     processesApiUrl: urlBase,
-                    useDebug,
                     defaultOrderBy,
                     defaultFilterBy,
                 } = ProcessesListConstants;
                 const userDbValue = databases[userDb]; // Could it be empty? Eg, to use: `|| database`
                 const offset = currentPage * pageSize; // TODO!
                 const params = {
-                    search: searchValue, // TODO: Should the `order_by` parameter be disabled if the `search` parameter has used?
-                    database: userDbValue, // useDebug ? database : userDb || defaultUserDb,
+                    search: searchValue,
+                    database: userDbValue,
+                    // The `order_by` parameter should be disabled if the `search` parameter has used...
                     order_by: !hasSearch && orderBy !== defaultOrderBy ? orderBy : '',
                     filter: filterBy !== defaultFilterBy ? filterBy : '',
                     offset,
                     limit: pageSize,
                 };
                 const urlQuery = CommonHelpers.makeQuery(params, {
                     addQuestionSymbol: true
                 });
                 const url = urlBase + urlQuery;
-                // DEBUG: Using temporarily while working with requests (issues #41, #45, etc)...
-                console.log('[ProcessesListDataLoad:loadData]: start', {
-                    searchValue,
-                    databases,
-                    userDbValue,
-                    useDebug,
-                    userDb,
-                    // database, // UNUSED: #41: Using `databases` and `userDb`.
-                    url,
-                    params,
-                    urlQuery,
-                    urlBase,
-                    currentPage,
-                    pageSize,
-                    offset,
-                    orderBy,
-                    filterBy,
-                });
+                /* // DEBUG: Using temporarily while working with requests (issues #41, #45, etc)...
+                 * console.log('[ProcessesListDataLoad:loadData]: start', {
+                 *   searchValue,
+                 *   databases,
+                 *   userDbValue,
+                 *   userDb,
+                 *   url,
+                 *   params,
+                 *   urlQuery,
+                 *   urlBase,
+                 *   currentPage,
+                 *   pageSize,
+                 *   offset,
+                 *   orderBy,
+                 *   filterBy,
+                 * });
+                 */
                 ProcessesListStates.setLoading(true);
                 fetch(url)
                     .then((res) => {
                         const {
                             ok,
                             status,
                             statusText
@@ -119,29 +117,18 @@
                             total_records: totalRecords
                         } = json;
                         const hasData = Array.isArray(data) && !!data.length;
                         const loadedRecords = hasData ? data.length : 0;
                         const currentRecords = offset + loadedRecords;
                         const hasMoreData = hasData && currentRecords < totalRecords;
                         const availableCount = hasMoreData ? totalRecords - currentRecords : 0;
-                        /* console.log('[ProcessesListDataLoad:loadData]: success', {
-                         *   availableCount,
-                         *   totalRecords,
-                         *   hasData,
-                         *   loadedRecords,
-                         *   currentRecords,
-                         *   hasMoreData,
-                         *   data,
-                         * });
-                         */
                         // Update total records number...
-                        // ProcessesListData.totalRecords = totalRecords;
                         ProcessesListStates.setTotalRecordsCount(totalRecords);
                         // Append data to current table...
-                        // TODO: Use `opts.update` to update (replace rows) last loaded data set.
+                        // TODO: Use `opts.update` to update (replace rows) last loaded data set?
                         ProcessesListDataRender.renderTableData(data, {
                             append: true
                         });
                         ProcessesListStates.setError(undefined); // Clear the error: all is ok
                         ProcessesListStates.setHasData(ProcessesListData.hasData || hasData); // Update 'has data' flag
                         ProcessesListStates.setHasMoreData(hasMoreData); // Update 'has more data' flag
                         ProcessesListStates.updateAvailableRecordsInfo(availableCount);
```

### Comparing `bw_matchbox-1.0.1/bw_matchbox/assets/js/ProcessesList/ProcessesListDataRender.js` & `bw_matchbox-1.0.2/bw_matchbox/assets/js/ProcessesList/ProcessesListDataRender.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.1/bw_matchbox/assets/js/ProcessesList/ProcessesListNodes.js` & `bw_matchbox-1.0.2/bw_matchbox/assets/js/ProcessesList/ProcessesListNodes.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.1/bw_matchbox/assets/js/ProcessesList/ProcessesListPagination.UNUSED.js` & `bw_matchbox-1.0.2/bw_matchbox/assets/js/ProcessesList/ProcessesListPagination.UNUSED.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.1/bw_matchbox/assets/js/ProcessesList/ProcessesListSearch.js` & `bw_matchbox-1.0.2/bw_matchbox/assets/js/ProcessesList/ProcessesListSearch.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.1/bw_matchbox/assets/js/ProcessesList/ProcessesListStates.js` & `bw_matchbox-1.0.2/bw_matchbox/assets/js/ProcessesList/ProcessesListStates.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.1/bw_matchbox/assets/js/common/CommonHelpers.js` & `bw_matchbox-1.0.2/bw_matchbox/assets/js/common/CommonHelpers.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.1/bw_matchbox/assets/js/common/CommonModal.js` & `bw_matchbox-1.0.2/bw_matchbox/assets/js/common/CommonModal.js`

 * *Files 26% similar despite different names*

#### js-beautify {}

```diff
@@ -11,14 +11,57 @@
     ) {
         // Define module...
 
         const CommonModal = {
             /** Initialized flag (see `inited` method) */
             inited: false,
 
+            onHideHandlers: [],
+
+            onHide(cb) {
+                if (cb && typeof cb === 'function') {
+                    this.onHideHandlers.push(cb);
+                }
+                return this;
+            },
+
+            clearOnHideHandlers() {
+                // Clear handlers list...
+                if (this.onHideHandlers.length) {
+                    this.onHideHandlers.length = 0; //  = [];
+                }
+                return this;
+            },
+
+            invokeOnHideHandlers() {
+                if (this.onHideHandlers.length) {
+                    // Invoke all the hide handlers and empty the list...
+                    let cb;
+                    while ((cb = this.onHideHandlers.shift()) != undefined) {
+                        if (cb && typeof cb === 'function') {
+                            try {
+                                cb();
+                                /* // Alternate option: Delayed start...
+                                 * setTimeout(cb, 0);
+                                 */
+                            } catch (error) {
+                                // eslint-disable-next-line no-console
+                                console.error('[CommonModal:invokeOnHideHandlers]: error (catched)', {
+                                    error,
+                                    cb,
+                                });
+                                // eslint-disable-next-line no-debugger
+                                debugger;
+                            }
+                        }
+                    }
+                }
+                return this;
+            },
+
             /** getModalNode -- Get root modal node
              * @return {HTMLElement|undefined}
              */
             getModalNode() {
                 const modal = document.getElementById('common-modal');
                 // TODO: Cache?
                 return modal;
@@ -63,14 +106,39 @@
              */
             setModalContentOption(optionName, optionValue) {
                 const contentEl = this.getModalNodeElementByClass('common-modal-content');
                 contentEl.classList.toggle(optionName, !!optionValue);
                 return this;
             },
 
+            /** setModalWindowOption -- Set one (boolean) modal content option.
+             * @param {string} optionName
+             * @param {boolean} [optionValue]
+             */
+            setModalWindowOption(optionName, optionValue) {
+                const literalOptions = {
+                    width: ['sm', 'md', 'lg'],
+                };
+                const contentEl = this.getModalNodeElementByClass('common-modal-window');
+                const literals = literalOptions[optionName];
+                if (literals) {
+                    // Literal option...
+                    literals.forEach((val) => {
+                        // Remove all the other and set current option...
+                        const isOn = val === optionValue;
+                        const name = optionName + '-' + val;
+                        contentEl.classList.toggle(name, isOn);
+                    });
+                } else {
+                    // Boolean option...
+                    contentEl.classList.toggle(optionName, !!optionValue);
+                }
+                return this;
+            },
+
             /** setModalContentScrollable -- Enable/disable scrollable mode for modal content.
              * @param {boolean} [scrollable]
              */
             setModalContentScrollable(scrollable) {
                 this.setModalContentOption('scrollable', scrollable);
                 return this;
             },
@@ -90,14 +158,30 @@
                 const names = Object.keys(options);
                 names.forEach((name) => {
                     this.setModalContentOption(name, options[name]);
                 });
                 return this;
             },
 
+            /** setModalWindowOptions -- Set one (boolean) modal content option.
+             * @param {<Record<string, [boolean]>>}} options - Options (`width`, `autoWidth`, `autoHeight`, `fullWindowHeight`, `fullWindowHeightt`)
+             * @param {string} [options.width] - Custom window size (sm, md, lg)
+             * @param {boolean} [options.autoWidth]
+             * @param {boolean} [options.autoHeight]
+             * @param {boolean} [options.fullWindowWidth] (UNUSED)
+             * @param {boolean} [options.fullWindowHeight] (UNUSED)
+             */
+            setModalWindowOptions(options) {
+                const names = Object.keys(options);
+                names.forEach((name) => {
+                    this.setModalWindowOption(name, options[name]);
+                });
+                return this;
+            },
+
             /** setModalContentId -- Set one (boolean) modal content option.
              * @param {string} id
              */
             setModalContentId(id) {
                 const contentEl = this.getModalNodeElementByClass('common-modal-content');
                 contentEl.setAttribute('id', id);
                 return this;
@@ -124,23 +208,31 @@
                 if (title) {
                     this.setTitle(title);
                 }
                 this.activateEvents();
                 return this;
             },
 
-            /** Hide modal window */
-            hideModal() {
+            /** Hide modal window
+             * @param {object} [opts] - Options.
+             * @param {boolean} [opts.dontNotify] - Options.
+             */
+            hideModal(opts = {}) {
                 this.deactivateEvents();
                 const modal = this.getModalNode();
                 if (!modal.classList.contains('show')) {
                     throw new Error('Trying to hide already hidden modal');
                 }
                 modal.classList.toggle('show', false);
                 document.body.classList.toggle('has-modal', false);
+                if (opts.dontNotify) {
+                    this.clearOnHideHandlers();
+                } else {
+                    this.invokeOnHideHandlers();
+                }
                 return this;
             },
 
             // Active events...
 
             onActiveKeyPress(event) {
                 if (event.key === 'Escape') {
```

### Comparing `bw_matchbox-1.0.1/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.js` & `bw_matchbox-1.0.2/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.1/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.min.js` & `bw_matchbox-1.0.2/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.min.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.1/bw_matchbox/assets/templates/common-modal.html` & `bw_matchbox-1.0.2/bw_matchbox/assets/templates/common-modal.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.1/bw_matchbox/assets/templates/compare.html` & `bw_matchbox-1.0.2/bw_matchbox/assets/templates/compare.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 {% include 'header.html' %}
 
 {# Common dependencies... #}
 
+{# Modal windows are used #}
 {% include 'common-modal.html' %}
 
 {# Module-specific dependencies... #}
 
 <link rel="stylesheet" href="{{ url_for('static', filename='css/compare.css') }}">
 
 <script src="{{ url_for('static', filename='js/Compare/CompareRowsHelpers.js') }}"></script>
 <script src="{{ url_for('static', filename='js/Compare/CompareProxyDialogModal.js') }}"></script>
 <script src="{{ url_for('static', filename='js/Compare/CompareRowClick.js') }}"></script>
 <script src="{{ url_for('static', filename='js/Compare/CompareCore.js') }}"></script>
 
 {# Core js module:
-  - `CompareCore` (from `bw_matchbox/assets/js/compare-core.js`)
+  - `CompareCore` (from `bw_matchbox/assets/js/Compare/CompareCore.js`)
 #}
 
 <div id="compare-root" class="container compare">
   {% include 'navigation.html' %}
   <div class="row">
     <div class="four columns">
       <h4>Location: {% if source_node.location == target_node.location %}Same{% else %}{{ source_node.location }}
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-{% include 'header.html' %} {# Common dependencies... #} {% include 'common-
-modal.html' %} {# Module-specific dependencies... #}
- {# Core js module: - `CompareCore` (from `bw_matchbox/assets/js/compare-
-core.js`) #}
+{% include 'header.html' %} {# Common dependencies... #} {# Modal windows are
+used #} {% include 'common-modal.html' %} {# Module-specific dependencies... #}
+ {# Core js module: - `CompareCore` (from `bw_matchbox/assets/js/Compare/
+CompareCore.js`) #}
 {% include 'navigation.html' %}
 *** Location: {% if source_node.location == target_node.location %}Same{% else
 %}{{ source_node.location }} | {{ target_node.location }}{% endif %} ***
 *** Unit: {% if source_node.unit == target_node.unit %}Same{% else %}{
 { source_node.unit }} | {{ target_node.unit }}{% endif %} ***
 {% if proxy and proxy != "None" %}Create Proxy 1-to-1 Proxy{% else %}Save{%
 endif %}
```

### Comparing `bw_matchbox-1.0.1/bw_matchbox/assets/templates/databases.html` & `bw_matchbox-1.0.2/bw_matchbox/assets/templates/databases.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.1/bw_matchbox/assets/templates/header.html` & `bw_matchbox-1.0.2/bw_matchbox/assets/templates/header.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.1/bw_matchbox/assets/templates/index.html` & `bw_matchbox-1.0.2/bw_matchbox/assets/templates/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 <script src="{{ url_for('static', filename='js/ProcessesList/ProcessesListStates.js') }}"></script>
 <script src="{{ url_for('static', filename='js/ProcessesList/ProcessesList.js') }}"></script>
 {# UNUSED ProcessesListPagination -- Using incremental data loading
 <script src="{{ url_for('static', filename='js/ProcessesList/ProcessesListPagination.js') }}"></script>
 #}
 
 {# Core module:
-  - `ProcessesList` (from `bw_matchbox/assets/js/ProcessesList.js`)
+  - `ProcessesList` (from `bw_matchbox/assets/js/ProcessesList/ProcessesList.js`)
 #}
 
 <div id="processes-list-root" class="container processes-list empty loading">
   {% include 'navigation.html' %}
   <div class="page-search">
     <p><input type="text" class="u-full-width" placeholder="Enter value to search" value="{{ query_string }}" id="query_string" /></p>
   </div>
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 {% include 'header.html' %} {# Module-specific dependencies... #}
  {# UNUSED ProcessesListPagination -- Using incremental data loading
  #} {# Core module: - `ProcessesList` (from `bw_matchbox/assets/js/
-ProcessesList.js`) #}
+ProcessesList/ProcessesList.js`) #}
 {% include 'navigation.html' %}
 [{{ query_string }}  ]
  {# Controls for `order_by` parameter (name, location, product; default is
 (empty) i.e. random (see `order-random` for `.processes-list` root node. #}
 Order by:   o Random   o Name   o Location   o Product    {# Controls for
 `filter` parameter: `matched`, `unmatched`, or `waitlist`. #}  Filter by:   o
 None   o Matched   o Unmatched   o Waitlist    {# Controls for `database`
```

### Comparing `bw_matchbox-1.0.1/bw_matchbox/assets/templates/match-status.html` & `bw_matchbox-1.0.2/bw_matchbox/assets/templates/match-status.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.1/bw_matchbox/assets/templates/match.html` & `bw_matchbox-1.0.2/bw_matchbox/assets/templates/match.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.1/bw_matchbox/assets/templates/navigation.html` & `bw_matchbox-1.0.2/bw_matchbox/assets/templates/navigation.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.1/bw_matchbox/assets/templates/process_detail.html` & `bw_matchbox-1.0.2/bw_matchbox/assets/templates/process_detail.html`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,33 @@
 {% include 'header.html' %}
-<div class="container">
+
+{# Common dependencies... #}
+
+{# Modal windows are used #}
+{% include 'common-modal.html' %}
+
+{# Module-specific dependencies... #}
+
+<link rel="stylesheet" href="{{ url_for('static', filename='css/process-detail.css') }}">
+
+<script src="{{ url_for('static', filename='js/ProcessDetail/ProcessDetail.js') }}"></script>
+
+{# Core js module:
+  - `ProcessDetail` (from `bw_matchbox/assets/js/ProcessDetail/ProcessDetail.js`)
+#}
+
+<div class="process-detail container">
   {% include 'navigation.html' %}
   <div class="row">
     <div class="column">
       <h1>{{ ds.name }}
         {% if ds.database == source %}
-          <button onclick="markWaitlist(this)" style="vertical-align: middle" class="button-primary" id="mark-waitlist">Waitlist</button>
-          {% if not ds.matched %}<button onclick="markMatched(this)" style="vertical-align: middle" class="button-primary" id="manual-match">No match needed</button>
-          {% if same_name_count %}<button onclick="markAllMatched(this)" style="vertical-align: middle" class="button-primary" id="manual-multi-match">Mark all matched</button>{% endif %}
+          <button onClick="ProcessDetail.markWaitlist(this)" style="vertical-align: middle" class="button-primary" id="mark-waitlist">Waitlist</button>
+          {% if not ds.matched %}<button onClick="ProcessDetail.markMatched(this)" style="vertical-align: middle" class="button-primary" id="manual-match">No match needed</button>
+          {% if same_name_count %}<button onClick="ProcessDetail.markAllMatched(this)" style="vertical-align: middle" class="button-primary" id="manual-multi-match">Mark all matched</button>{% endif %}
           <a style="vertical-align: middle" id="match-button" class="button button-primary" href="{{ url_for('match', source=ds.id)}}">Match</a>{% elif ds.match_type == "1" %}<button id="match-button" style="vertical-align: middle">No match needed</button>{% else %}<button id="match-button" style="vertical-align: middle">Matched</button>{% endif %}
         {% endif %}
       </h1>
       <ul>
           <li>Database: {{ ds.database }}</li>
           <li>Location: {{ ds.location }}</li>
           <li>Unit: {{ ds.unit }}</li>
@@ -99,49 +115,29 @@
       {% endif %}
       </table>
     </div>
   </div>
 </div>
 
 <script type="text/javascript">
-function markWaitlist (button) {
-  var url = "{{ url_for('add_attribute', id=ds.id, attr='waitlist', value='1')|safe }}";
-  fetch(url).then((response) => {
-    if (!response.ok) {
-        throw new Error(`HTTP error ${response.status}`);
-    };
-    button.innerText = "Waitlisted";
-    button.classList.remove("button-primary");
+modules.require('ProcessDetail', function requireProcessDetail(ProcessDetail) {
+  // Global variables for compare tables feature (via global variable `sharedData`)...
+  const sharedData = {
+    addAttributeUrl: "{{ url_for('add_attribute', id=ds.id)|safe }}",
+    // markWaitlistUrl: "{{ url_for('add_attribute', id=ds.id, attr='waitlist', value='1')|safe }}",
+    markMatchTypeUrl: "{{ url_for('add_attribute', id=ds.id, attr='match_type', value='1')|safe }}",
+    markMatchedUrl: "{{ url_for('add_attribute', id=ds.id, attr='matched', value='1')|safe }}",
+    markAllMatchedUrl: "{{ url_for('multi_match', id=ds.id)|safe }}",
+    multimatch: "{{ multimatch or '' }}", // TODO: What type of variable is here? Is it string or boolean?
+  };
+  console.log('[process_detail:requireProcessDetail]', {
+    sharedData,
   });
-};
 
-function markMatched (button) {
-  fetch("{{ url_for('add_attribute', id=ds.id, attr='match_type', value='1')|safe }}");
-  var url = "{{ url_for('add_attribute', id=ds.id, attr='matched', value='1')|safe }}";
-  fetch(url).then((response) => {
-    if (!response.ok) {
-        throw new Error(`HTTP error ${response.status}`);
-    };
-    button.innerText = "Matched";
-    button.classList.remove("button-primary");
-    document.getElementById('match-button').style.display = 'none';
-    document.getElementById('manual-multi-match').style.display = 'none';
-    {% if multimatch %}document.getElementById('manual-multi-match').style.display = 'none';{% endif %}
-  });
-};
+  // Export to global scope (to access from generated html code handlers).
+  window.ProcessDetail = ProcessDetail;
 
-{% if same_name_count %}
-function markAllMatched (button) {
-  var url = "{{ url_for('multi_match', id=ds.id)|safe }}";
-  fetch(url).then((response) => {
-    if (!response.ok) {
-        throw new Error(`HTTP error ${response.status}`);
-    };
-    button.innerText = "Matched";
-    button.classList.remove("button-primary");
-    document.getElementById('manual-match').style.display = 'none';
-    document.getElementById('match-button').style.display = 'none';
-  });
-};
-{% endif %}
+  // Start core module...
+  ProcessDetail.start(sharedData);
+});
 </script>
 {% include 'footer.html' %}
```

#### html2text {}

```diff
@@ -1,8 +1,11 @@
-{% include 'header.html' %}
+{% include 'header.html' %} {# Common dependencies... #} {# Modal windows are
+used #} {% include 'common-modal.html' %} {# Module-specific dependencies... #}
+ {# Core js module: - `ProcessDetail` (from `bw_matchbox/assets/js/
+ProcessDetail/ProcessDetail.js`) #}
 {% include 'navigation.html' %}
 ****** {{ ds.name }} {% if ds.database == source %} Waitlist {% if not
 ds.matched %}No match needed {% if same_name_count %}Mark all matched{% endif
 %} Match{% elif ds.match_type == "1" %}No match needed{% else %}Matched{% endif
 %} {% endif %} ******
     * Database: {{ ds.database }}
     * Location: {{ ds.location }}
```

### Comparing `bw_matchbox-1.0.1/bw_matchbox/assets/templates/project.html` & `bw_matchbox-1.0.2/bw_matchbox/assets/templates/project.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.1/bw_matchbox/assets/templates/search.html` & `bw_matchbox-1.0.2/bw_matchbox/assets/templates/search.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.1/bw_matchbox/assets/templates/search_result.html` & `bw_matchbox-1.0.2/bw_matchbox/assets/templates/search_result.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.1/bw_matchbox/assets/templates/select_files.html` & `bw_matchbox-1.0.2/bw_matchbox/assets/templates/select_files.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.1/bw_matchbox/bin/matchbox.py` & `bw_matchbox-1.0.2/bw_matchbox/bin/matchbox.py`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.1/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-mining.json` & `bw_matchbox-1.0.2/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-mining.json`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.1/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-string-matching.json` & `bw_matchbox-1.0.2/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-string-matching.json`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.1/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-transport.json` & `bw_matchbox-1.0.2/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-transport.json`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.1/bw_matchbox/data/dare.json` & `bw_matchbox-1.0.2/bw_matchbox/data/dare.json`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.1/bw_matchbox/utils.py` & `bw_matchbox-1.0.2/bw_matchbox/utils.py`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.1/bw_matchbox/webapp.py` & `bw_matchbox-1.0.2/bw_matchbox/webapp.py`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.1/bw_matchbox.egg-info/PKG-INFO` & `bw_matchbox-1.0.2/bw_matchbox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bw-matchbox
-Version: 1.0.1
+Version: 1.0.2
 Summary: Browser to match Brightway databases
 Home-page: https://github.com/cauldron/bw_matchbox
 Author: Chris Mutel
 Author-email: <cmutel@gmail.com>
 Maintainer: Chris Mutel
 Maintainer-email: <cmutel@gmail.com>
 License: MIT
```

### Comparing `bw_matchbox-1.0.1/bw_matchbox.egg-info/SOURCES.txt` & `bw_matchbox-1.0.2/bw_matchbox.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -9,22 +9,24 @@
 ./bw_matchbox/webapp.py
 ./bw_matchbox/assets/css/common-modal.css
 ./bw_matchbox/assets/css/common.css
 ./bw_matchbox/assets/css/compare.css
 ./bw_matchbox/assets/css/customizations.css
 ./bw_matchbox/assets/css/fixed-table.css
 ./bw_matchbox/assets/css/normalize.css
+./bw_matchbox/assets/css/process-detail.css
 ./bw_matchbox/assets/css/processes-list.css
 ./bw_matchbox/assets/css/skeleton.css
 ./bw_matchbox/assets/css/tooltip.css
 ./bw_matchbox/assets/images/favicon.ico
 ./bw_matchbox/assets/js/Compare/CompareCore.js
 ./bw_matchbox/assets/js/Compare/CompareProxyDialogModal.js
 ./bw_matchbox/assets/js/Compare/CompareRowClick.js
 ./bw_matchbox/assets/js/Compare/CompareRowsHelpers.js
+./bw_matchbox/assets/js/ProcessDetail/ProcessDetail.js
 ./bw_matchbox/assets/js/ProcessesList/ProcessesList.js
 ./bw_matchbox/assets/js/ProcessesList/ProcessesListConstants.js
 ./bw_matchbox/assets/js/ProcessesList/ProcessesListData.js
 ./bw_matchbox/assets/js/ProcessesList/ProcessesListDataLoad.js
 ./bw_matchbox/assets/js/ProcessesList/ProcessesListDataRender.js
 ./bw_matchbox/assets/js/ProcessesList/ProcessesListNodes.js
 ./bw_matchbox/assets/js/ProcessesList/ProcessesListPagination.UNUSED.js
@@ -67,22 +69,24 @@
 bw_matchbox.egg-info/top_level.txt
 bw_matchbox/assets/css/common-modal.css
 bw_matchbox/assets/css/common.css
 bw_matchbox/assets/css/compare.css
 bw_matchbox/assets/css/customizations.css
 bw_matchbox/assets/css/fixed-table.css
 bw_matchbox/assets/css/normalize.css
+bw_matchbox/assets/css/process-detail.css
 bw_matchbox/assets/css/processes-list.css
 bw_matchbox/assets/css/skeleton.css
 bw_matchbox/assets/css/tooltip.css
 bw_matchbox/assets/images/favicon.ico
 bw_matchbox/assets/js/Compare/CompareCore.js
 bw_matchbox/assets/js/Compare/CompareProxyDialogModal.js
 bw_matchbox/assets/js/Compare/CompareRowClick.js
 bw_matchbox/assets/js/Compare/CompareRowsHelpers.js
+bw_matchbox/assets/js/ProcessDetail/ProcessDetail.js
 bw_matchbox/assets/js/ProcessesList/ProcessesList.js
 bw_matchbox/assets/js/ProcessesList/ProcessesListConstants.js
 bw_matchbox/assets/js/ProcessesList/ProcessesListData.js
 bw_matchbox/assets/js/ProcessesList/ProcessesListDataLoad.js
 bw_matchbox/assets/js/ProcessesList/ProcessesListDataRender.js
 bw_matchbox/assets/js/ProcessesList/ProcessesListNodes.js
 bw_matchbox/assets/js/ProcessesList/ProcessesListPagination.UNUSED.js
```

### Comparing `bw_matchbox-1.0.1/docs/conf.py` & `bw_matchbox-1.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.1/setup.cfg` & `bw_matchbox-1.0.2/setup.cfg`

 * *Files identical despite different names*

