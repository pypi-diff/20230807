# Comparing `tmp/bw_matchbox-1.0.0.tar.gz` & `tmp/bw_matchbox-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bw_matchbox-1.0.0.tar", last modified: Mon Aug  7 06:04:52 2023, max compression
+gzip compressed data, was "bw_matchbox-1.0.1.tar", last modified: Mon Aug  7 13:45:04 2023, max compression
```

## Comparing `bw_matchbox-1.0.0.tar` & `bw_matchbox-1.0.1.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-07 06:04:52.858772 bw_matchbox-1.0.0/
--rw-r--r--   0 chrismutel   (501) staff       (20)     1067 2023-06-20 12:26:53.000000 bw_matchbox-1.0.0/LICENSE
--rw-r--r--   0 chrismutel   (501) staff       (20)      226 2023-08-02 21:05:25.000000 bw_matchbox-1.0.0/MANIFEST.in
--rw-r--r--   0 chrismutel   (501) staff       (20)     6361 2023-08-07 06:04:52.858838 bw_matchbox-1.0.0/PKG-INFO
--rw-r--r--   0 chrismutel   (501) staff       (20)     5337 2023-08-05 17:26:08.000000 bw_matchbox-1.0.0/README.md
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-07 06:04:52.842398 bw_matchbox-1.0.0/bw_matchbox/
--rw-r--r--   0 chrismutel   (501) staff       (20)        6 2023-08-07 06:04:24.000000 bw_matchbox-1.0.0/bw_matchbox/VERSION
--rw-r--r--   0 chrismutel   (501) staff       (20)      215 2023-08-01 17:17:21.000000 bw_matchbox-1.0.0/bw_matchbox/__init__.py
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-07 06:04:52.840606 bw_matchbox-1.0.0/bw_matchbox/assets/
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-07 06:04:52.844980 bw_matchbox-1.0.0/bw_matchbox/assets/css/
--rw-r--r--   0 chrismutel   (501) staff       (20)     3297 2023-08-06 18:22:10.000000 bw_matchbox-1.0.0/bw_matchbox/assets/css/common-modal.css
--rw-r--r--   0 chrismutel   (501) staff       (20)     1922 2023-08-06 18:22:10.000000 bw_matchbox-1.0.0/bw_matchbox/assets/css/common.css
--rw-r--r--   0 chrismutel   (501) staff       (20)     4256 2023-08-06 18:22:10.000000 bw_matchbox-1.0.0/bw_matchbox/assets/css/compare.css
--rw-r--r--   0 chrismutel   (501) staff       (20)      640 2023-08-03 20:45:26.000000 bw_matchbox-1.0.0/bw_matchbox/assets/css/customizations.css
--rw-r--r--   0 chrismutel   (501) staff       (20)     1392 2023-08-04 13:00:53.000000 bw_matchbox-1.0.0/bw_matchbox/assets/css/fixed-table.css
--rw-r--r--   0 chrismutel   (501) staff       (20)     7618 2023-08-01 07:10:26.000000 bw_matchbox-1.0.0/bw_matchbox/assets/css/normalize.css
--rw-r--r--   0 chrismutel   (501) staff       (20)     4315 2023-08-06 18:22:10.000000 bw_matchbox-1.0.0/bw_matchbox/assets/css/processes-list.css
--rw-r--r--   0 chrismutel   (501) staff       (20)    11556 2023-08-01 07:10:26.000000 bw_matchbox-1.0.0/bw_matchbox/assets/css/skeleton.css
--rw-r--r--   0 chrismutel   (501) staff       (20)      916 2023-08-01 07:10:26.000000 bw_matchbox-1.0.0/bw_matchbox/assets/css/tooltip.css
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-07 06:04:52.845203 bw_matchbox-1.0.0/bw_matchbox/assets/images/
--rw-r--r--   0 chrismutel   (501) staff       (20)    32038 2023-06-20 12:27:44.000000 bw_matchbox-1.0.0/bw_matchbox/assets/images/favicon.ico
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-07 06:04:52.840500 bw_matchbox-1.0.0/bw_matchbox/assets/js/
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-07 06:04:52.847488 bw_matchbox-1.0.0/bw_matchbox/assets/js/Compare/
--rw-r--r--   0 chrismutel   (501) staff       (20)    20394 2023-08-06 20:10:31.000000 bw_matchbox-1.0.0/bw_matchbox/assets/js/Compare/CompareCore.js
--rw-r--r--   0 chrismutel   (501) staff       (20)     6194 2023-08-06 18:22:10.000000 bw_matchbox-1.0.0/bw_matchbox/assets/js/Compare/CompareProxyDialogModal.js
--rw-r--r--   0 chrismutel   (501) staff       (20)     1272 2023-08-04 16:42:28.000000 bw_matchbox-1.0.0/bw_matchbox/assets/js/Compare/CompareRowClick.js
--rw-r--r--   0 chrismutel   (501) staff       (20)    12879 2023-08-06 18:22:10.000000 bw_matchbox-1.0.0/bw_matchbox/assets/js/Compare/CompareRowsHelpers.js
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-07 06:04:52.848937 bw_matchbox-1.0.0/bw_matchbox/assets/js/ProcessesList/
--rw-r--r--   0 chrismutel   (501) staff       (20)     4388 2023-08-06 18:22:10.000000 bw_matchbox-1.0.0/bw_matchbox/assets/js/ProcessesList/ProcessesList.js
--rw-r--r--   0 chrismutel   (501) staff       (20)      885 2023-08-06 18:22:10.000000 bw_matchbox-1.0.0/bw_matchbox/assets/js/ProcessesList/ProcessesListConstants.js
--rw-r--r--   0 chrismutel   (501) staff       (20)     1452 2023-08-06 18:22:10.000000 bw_matchbox-1.0.0/bw_matchbox/assets/js/ProcessesList/ProcessesListData.js
--rw-r--r--   0 chrismutel   (501) staff       (20)     5632 2023-08-06 18:22:10.000000 bw_matchbox-1.0.0/bw_matchbox/assets/js/ProcessesList/ProcessesListDataLoad.js
--rw-r--r--   0 chrismutel   (501) staff       (20)     3447 2023-08-06 18:22:10.000000 bw_matchbox-1.0.0/bw_matchbox/assets/js/ProcessesList/ProcessesListDataRender.js
--rw-r--r--   0 chrismutel   (501) staff       (20)     1081 2023-08-06 18:22:10.000000 bw_matchbox-1.0.0/bw_matchbox/assets/js/ProcessesList/ProcessesListNodes.js
--rw-r--r--   0 chrismutel   (501) staff       (20)     4862 2023-08-06 18:22:10.000000 bw_matchbox-1.0.0/bw_matchbox/assets/js/ProcessesList/ProcessesListPagination.UNUSED.js
--rw-r--r--   0 chrismutel   (501) staff       (20)     3321 2023-08-06 18:22:10.000000 bw_matchbox-1.0.0/bw_matchbox/assets/js/ProcessesList/ProcessesListSearch.js
--rw-r--r--   0 chrismutel   (501) staff       (20)     9995 2023-08-06 18:22:10.000000 bw_matchbox-1.0.0/bw_matchbox/assets/js/ProcessesList/ProcessesListStates.js
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-07 06:04:52.849279 bw_matchbox-1.0.0/bw_matchbox/assets/js/common/
--rw-r--r--   0 chrismutel   (501) staff       (20)     5634 2023-08-04 13:00:53.000000 bw_matchbox-1.0.0/bw_matchbox/assets/js/common/CommonHelpers.js
--rw-r--r--   0 chrismutel   (501) staff       (20)     5781 2023-08-06 18:22:10.000000 bw_matchbox-1.0.0/bw_matchbox/assets/js/common/CommonModal.js
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-07 06:04:52.840545 bw_matchbox-1.0.0/bw_matchbox/assets/js/libs/
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-07 06:04:52.849627 bw_matchbox-1.0.0/bw_matchbox/assets/js/libs/ym/
--rw-r--r--   0 chrismutel   (501) staff       (20)    13286 2023-08-03 20:45:26.000000 bw_matchbox-1.0.0/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.js
--rw-r--r--   0 chrismutel   (501) staff       (20)     6018 2023-08-03 20:45:26.000000 bw_matchbox-1.0.0/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.min.js
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-07 06:04:52.853096 bw_matchbox-1.0.0/bw_matchbox/assets/templates/
--rw-r--r--   0 chrismutel   (501) staff       (20)      756 2023-08-04 13:00:53.000000 bw_matchbox-1.0.0/bw_matchbox/assets/templates/common-modal.html
--rw-r--r--   0 chrismutel   (501) staff       (20)     3880 2023-08-06 18:22:10.000000 bw_matchbox-1.0.0/bw_matchbox/assets/templates/compare.html
--rw-r--r--   0 chrismutel   (501) staff       (20)     2681 2023-08-05 17:26:08.000000 bw_matchbox-1.0.0/bw_matchbox/assets/templates/databases.html
--rw-r--r--   0 chrismutel   (501) staff       (20)      461 2023-07-23 15:09:13.000000 bw_matchbox-1.0.0/bw_matchbox/assets/templates/expand.html
--rw-r--r--   0 chrismutel   (501) staff       (20)       16 2023-06-20 12:27:44.000000 bw_matchbox-1.0.0/bw_matchbox/assets/templates/footer.html
--rw-r--r--   0 chrismutel   (501) staff       (20)     2666 2023-08-04 13:00:53.000000 bw_matchbox-1.0.0/bw_matchbox/assets/templates/header.html
--rw-r--r--   0 chrismutel   (501) staff       (20)     6969 2023-08-06 18:22:10.000000 bw_matchbox-1.0.0/bw_matchbox/assets/templates/index.html
--rw-r--r--   0 chrismutel   (501) staff       (20)      733 2023-06-21 04:56:26.000000 bw_matchbox-1.0.0/bw_matchbox/assets/templates/match-status.html
--rw-r--r--   0 chrismutel   (501) staff       (20)     1721 2023-08-03 20:45:26.000000 bw_matchbox-1.0.0/bw_matchbox/assets/templates/match.html
--rw-r--r--   0 chrismutel   (501) staff       (20)      734 2023-08-05 17:26:08.000000 bw_matchbox-1.0.0/bw_matchbox/assets/templates/navigation.html
--rw-r--r--   0 chrismutel   (501) staff       (20)     5932 2023-08-06 18:58:22.000000 bw_matchbox-1.0.0/bw_matchbox/assets/templates/process_detail.html
--rw-r--r--   0 chrismutel   (501) staff       (20)      599 2023-07-22 21:06:00.000000 bw_matchbox-1.0.0/bw_matchbox/assets/templates/project.html
--rw-r--r--   0 chrismutel   (501) staff       (20)      412 2023-08-01 07:10:26.000000 bw_matchbox-1.0.0/bw_matchbox/assets/templates/search-embedded.html
--rw-r--r--   0 chrismutel   (501) staff       (20)      850 2023-06-20 12:27:44.000000 bw_matchbox-1.0.0/bw_matchbox/assets/templates/search.html
--rw-r--r--   0 chrismutel   (501) staff       (20)      947 2023-06-20 12:27:44.000000 bw_matchbox-1.0.0/bw_matchbox/assets/templates/search_result.html
--rw-r--r--   0 chrismutel   (501) staff       (20)     1243 2023-07-23 08:33:52.000000 bw_matchbox-1.0.0/bw_matchbox/assets/templates/select_files.html
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-07 06:04:52.853478 bw_matchbox-1.0.0/bw_matchbox/bin/
--rw-r--r--   0 chrismutel   (501) staff       (20)        0 2023-06-20 12:27:44.000000 bw_matchbox-1.0.0/bw_matchbox/bin/__init__.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     2692 2023-08-05 17:26:08.000000 bw_matchbox-1.0.0/bw_matchbox/bin/matchbox.py
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-07 06:04:52.856237 bw_matchbox-1.0.0/bw_matchbox/data/
--rw-r--r--   0 chrismutel   (501) staff       (20)   123246 2023-08-01 17:17:21.000000 bw_matchbox-1.0.0/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-mining.json
--rw-r--r--   0 chrismutel   (501) staff       (20)    93862 2023-07-23 09:30:53.000000 bw_matchbox-1.0.0/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-string-matching.json
--rw-r--r--   0 chrismutel   (501) staff       (20)   116072 2023-08-01 17:17:21.000000 bw_matchbox-1.0.0/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-transport.json
--rw-r--r--   0 chrismutel   (501) staff       (20)      603 2023-07-23 09:34:59.000000 bw_matchbox-1.0.0/bw_matchbox/data/dare.json
--rw-r--r--   0 chrismutel   (501) staff       (20)     2155 2023-08-06 18:22:10.000000 bw_matchbox-1.0.0/bw_matchbox/utils.py
--rw-r--r--   0 chrismutel   (501) staff       (20)    22926 2023-08-06 19:01:25.000000 bw_matchbox-1.0.0/bw_matchbox/webapp.py
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-07 06:04:52.857562 bw_matchbox-1.0.0/bw_matchbox.egg-info/
--rw-r--r--   0 chrismutel   (501) staff       (20)     6361 2023-08-07 06:04:52.000000 bw_matchbox-1.0.0/bw_matchbox.egg-info/PKG-INFO
--rw-r--r--   0 chrismutel   (501) staff       (20)     5090 2023-08-07 06:04:52.000000 bw_matchbox-1.0.0/bw_matchbox.egg-info/SOURCES.txt
--rw-r--r--   0 chrismutel   (501) staff       (20)        1 2023-08-07 06:04:52.000000 bw_matchbox-1.0.0/bw_matchbox.egg-info/dependency_links.txt
--rw-r--r--   0 chrismutel   (501) staff       (20)       59 2023-08-07 06:04:52.000000 bw_matchbox-1.0.0/bw_matchbox.egg-info/entry_points.txt
--rw-r--r--   0 chrismutel   (501) staff       (20)        1 2023-07-23 07:30:31.000000 bw_matchbox-1.0.0/bw_matchbox.egg-info/not-zip-safe
--rw-r--r--   0 chrismutel   (501) staff       (20)      167 2023-08-07 06:04:52.000000 bw_matchbox-1.0.0/bw_matchbox.egg-info/requires.txt
--rw-r--r--   0 chrismutel   (501) staff       (20)       12 2023-08-07 06:04:52.000000 bw_matchbox-1.0.0/bw_matchbox.egg-info/top_level.txt
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-07 06:04:52.856488 bw_matchbox-1.0.0/docs/
--rw-r--r--   0 chrismutel   (501) staff       (20)     1145 2023-07-23 07:23:19.000000 bw_matchbox-1.0.0/docs/conf.py
--rw-r--r--   0 chrismutel   (501) staff       (20)       87 2023-06-20 12:26:53.000000 bw_matchbox-1.0.0/pyproject.toml
--rw-r--r--   0 chrismutel   (501) staff       (20)     1900 2023-08-07 06:04:52.859219 bw_matchbox-1.0.0/setup.cfg
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-07 13:45:04.167070 bw_matchbox-1.0.1/
+-rw-r--r--   0 cmutel     (501) staff       (20)     1067 2023-07-24 11:16:50.000000 bw_matchbox-1.0.1/LICENSE
+-rw-r--r--   0 cmutel     (501) staff       (20)      226 2023-08-03 14:06:22.000000 bw_matchbox-1.0.1/MANIFEST.in
+-rw-r--r--   0 cmutel     (501) staff       (20)     6361 2023-08-07 13:45:04.167162 bw_matchbox-1.0.1/PKG-INFO
+-rw-r--r--   0 cmutel     (501) staff       (20)     5337 2023-08-05 07:08:03.000000 bw_matchbox-1.0.1/README.md
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-07 13:45:04.152833 bw_matchbox-1.0.1/bw_matchbox/
+-rw-r--r--   0 cmutel     (501) staff       (20)        6 2023-08-07 13:44:20.000000 bw_matchbox-1.0.1/bw_matchbox/VERSION
+-rw-r--r--   0 cmutel     (501) staff       (20)      215 2023-08-03 14:06:22.000000 bw_matchbox-1.0.1/bw_matchbox/__init__.py
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-07 13:45:04.150853 bw_matchbox-1.0.1/bw_matchbox/assets/
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-07 13:45:04.155127 bw_matchbox-1.0.1/bw_matchbox/assets/css/
+-rw-r--r--   0 cmutel     (501) staff       (20)     3297 2023-08-07 06:34:48.000000 bw_matchbox-1.0.1/bw_matchbox/assets/css/common-modal.css
+-rw-r--r--   0 cmutel     (501) staff       (20)     1922 2023-08-07 06:34:48.000000 bw_matchbox-1.0.1/bw_matchbox/assets/css/common.css
+-rw-r--r--   0 cmutel     (501) staff       (20)     4256 2023-08-07 06:34:48.000000 bw_matchbox-1.0.1/bw_matchbox/assets/css/compare.css
+-rw-r--r--   0 cmutel     (501) staff       (20)      640 2023-08-05 06:10:27.000000 bw_matchbox-1.0.1/bw_matchbox/assets/css/customizations.css
+-rw-r--r--   0 cmutel     (501) staff       (20)     1392 2023-08-05 06:10:27.000000 bw_matchbox-1.0.1/bw_matchbox/assets/css/fixed-table.css
+-rw-r--r--   0 cmutel     (501) staff       (20)     7618 2023-08-01 11:28:52.000000 bw_matchbox-1.0.1/bw_matchbox/assets/css/normalize.css
+-rw-r--r--   0 cmutel     (501) staff       (20)     4315 2023-08-06 09:58:28.000000 bw_matchbox-1.0.1/bw_matchbox/assets/css/processes-list.css
+-rw-r--r--   0 cmutel     (501) staff       (20)    11556 2023-08-01 11:28:52.000000 bw_matchbox-1.0.1/bw_matchbox/assets/css/skeleton.css
+-rw-r--r--   0 cmutel     (501) staff       (20)      916 2023-08-01 11:28:52.000000 bw_matchbox-1.0.1/bw_matchbox/assets/css/tooltip.css
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-07 13:45:04.155381 bw_matchbox-1.0.1/bw_matchbox/assets/images/
+-rw-r--r--   0 cmutel     (501) staff       (20)    32038 2023-07-24 11:16:50.000000 bw_matchbox-1.0.1/bw_matchbox/assets/images/favicon.ico
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-07 13:45:04.150746 bw_matchbox-1.0.1/bw_matchbox/assets/js/
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-07 13:45:04.156309 bw_matchbox-1.0.1/bw_matchbox/assets/js/Compare/
+-rw-r--r--   0 cmutel     (501) staff       (20)    20293 2023-08-07 06:34:48.000000 bw_matchbox-1.0.1/bw_matchbox/assets/js/Compare/CompareCore.js
+-rw-r--r--   0 cmutel     (501) staff       (20)     6194 2023-08-07 06:34:48.000000 bw_matchbox-1.0.1/bw_matchbox/assets/js/Compare/CompareProxyDialogModal.js
+-rw-r--r--   0 cmutel     (501) staff       (20)     1272 2023-08-05 06:10:27.000000 bw_matchbox-1.0.1/bw_matchbox/assets/js/Compare/CompareRowClick.js
+-rw-r--r--   0 cmutel     (501) staff       (20)    12879 2023-08-07 06:34:48.000000 bw_matchbox-1.0.1/bw_matchbox/assets/js/Compare/CompareRowsHelpers.js
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-07 13:45:04.158335 bw_matchbox-1.0.1/bw_matchbox/assets/js/ProcessesList/
+-rw-r--r--   0 cmutel     (501) staff       (20)     4388 2023-08-06 09:58:28.000000 bw_matchbox-1.0.1/bw_matchbox/assets/js/ProcessesList/ProcessesList.js
+-rw-r--r--   0 cmutel     (501) staff       (20)      885 2023-08-06 09:58:28.000000 bw_matchbox-1.0.1/bw_matchbox/assets/js/ProcessesList/ProcessesListConstants.js
+-rw-r--r--   0 cmutel     (501) staff       (20)     1452 2023-08-06 09:58:28.000000 bw_matchbox-1.0.1/bw_matchbox/assets/js/ProcessesList/ProcessesListData.js
+-rw-r--r--   0 cmutel     (501) staff       (20)     5632 2023-08-06 09:58:28.000000 bw_matchbox-1.0.1/bw_matchbox/assets/js/ProcessesList/ProcessesListDataLoad.js
+-rw-r--r--   0 cmutel     (501) staff       (20)     3447 2023-08-06 09:58:28.000000 bw_matchbox-1.0.1/bw_matchbox/assets/js/ProcessesList/ProcessesListDataRender.js
+-rw-r--r--   0 cmutel     (501) staff       (20)     1081 2023-08-06 09:58:28.000000 bw_matchbox-1.0.1/bw_matchbox/assets/js/ProcessesList/ProcessesListNodes.js
+-rw-r--r--   0 cmutel     (501) staff       (20)     4862 2023-08-06 09:58:28.000000 bw_matchbox-1.0.1/bw_matchbox/assets/js/ProcessesList/ProcessesListPagination.UNUSED.js
+-rw-r--r--   0 cmutel     (501) staff       (20)     3321 2023-08-06 09:58:28.000000 bw_matchbox-1.0.1/bw_matchbox/assets/js/ProcessesList/ProcessesListSearch.js
+-rw-r--r--   0 cmutel     (501) staff       (20)     9995 2023-08-06 09:58:28.000000 bw_matchbox-1.0.1/bw_matchbox/assets/js/ProcessesList/ProcessesListStates.js
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-07 13:45:04.158711 bw_matchbox-1.0.1/bw_matchbox/assets/js/common/
+-rw-r--r--   0 cmutel     (501) staff       (20)     5634 2023-08-05 06:10:27.000000 bw_matchbox-1.0.1/bw_matchbox/assets/js/common/CommonHelpers.js
+-rw-r--r--   0 cmutel     (501) staff       (20)     5781 2023-08-06 13:56:54.000000 bw_matchbox-1.0.1/bw_matchbox/assets/js/common/CommonModal.js
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-07 13:45:04.150792 bw_matchbox-1.0.1/bw_matchbox/assets/js/libs/
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-07 13:45:04.159306 bw_matchbox-1.0.1/bw_matchbox/assets/js/libs/ym/
+-rw-r--r--   0 cmutel     (501) staff       (20)    13286 2023-08-03 14:06:22.000000 bw_matchbox-1.0.1/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.js
+-rw-r--r--   0 cmutel     (501) staff       (20)     6018 2023-08-03 14:06:22.000000 bw_matchbox-1.0.1/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.min.js
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-07 13:45:04.162797 bw_matchbox-1.0.1/bw_matchbox/assets/templates/
+-rw-r--r--   0 cmutel     (501) staff       (20)      756 2023-08-05 06:10:27.000000 bw_matchbox-1.0.1/bw_matchbox/assets/templates/common-modal.html
+-rw-r--r--   0 cmutel     (501) staff       (20)     3880 2023-08-07 06:34:48.000000 bw_matchbox-1.0.1/bw_matchbox/assets/templates/compare.html
+-rw-r--r--   0 cmutel     (501) staff       (20)     2681 2023-08-05 07:08:03.000000 bw_matchbox-1.0.1/bw_matchbox/assets/templates/databases.html
+-rw-r--r--   0 cmutel     (501) staff       (20)      461 2023-07-24 11:16:50.000000 bw_matchbox-1.0.1/bw_matchbox/assets/templates/expand.html
+-rw-r--r--   0 cmutel     (501) staff       (20)       16 2023-07-24 11:16:50.000000 bw_matchbox-1.0.1/bw_matchbox/assets/templates/footer.html
+-rw-r--r--   0 cmutel     (501) staff       (20)     2666 2023-08-05 06:10:27.000000 bw_matchbox-1.0.1/bw_matchbox/assets/templates/header.html
+-rw-r--r--   0 cmutel     (501) staff       (20)     6969 2023-08-06 09:58:28.000000 bw_matchbox-1.0.1/bw_matchbox/assets/templates/index.html
+-rw-r--r--   0 cmutel     (501) staff       (20)      733 2023-07-24 11:16:50.000000 bw_matchbox-1.0.1/bw_matchbox/assets/templates/match-status.html
+-rw-r--r--   0 cmutel     (501) staff       (20)     1713 2023-08-07 13:23:46.000000 bw_matchbox-1.0.1/bw_matchbox/assets/templates/match.html
+-rw-r--r--   0 cmutel     (501) staff       (20)      734 2023-08-05 07:08:03.000000 bw_matchbox-1.0.1/bw_matchbox/assets/templates/navigation.html
+-rw-r--r--   0 cmutel     (501) staff       (20)     5830 2023-08-07 13:43:30.000000 bw_matchbox-1.0.1/bw_matchbox/assets/templates/process_detail.html
+-rw-r--r--   0 cmutel     (501) staff       (20)      599 2023-07-24 11:16:50.000000 bw_matchbox-1.0.1/bw_matchbox/assets/templates/project.html
+-rw-r--r--   0 cmutel     (501) staff       (20)      412 2023-08-01 11:28:52.000000 bw_matchbox-1.0.1/bw_matchbox/assets/templates/search-embedded.html
+-rw-r--r--   0 cmutel     (501) staff       (20)      850 2023-07-24 11:16:50.000000 bw_matchbox-1.0.1/bw_matchbox/assets/templates/search.html
+-rw-r--r--   0 cmutel     (501) staff       (20)      947 2023-07-24 11:16:50.000000 bw_matchbox-1.0.1/bw_matchbox/assets/templates/search_result.html
+-rw-r--r--   0 cmutel     (501) staff       (20)     1243 2023-07-24 11:16:50.000000 bw_matchbox-1.0.1/bw_matchbox/assets/templates/select_files.html
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-07 13:45:04.163043 bw_matchbox-1.0.1/bw_matchbox/bin/
+-rw-r--r--   0 cmutel     (501) staff       (20)        0 2023-07-24 11:16:50.000000 bw_matchbox-1.0.1/bw_matchbox/bin/__init__.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     2692 2023-08-05 18:47:38.000000 bw_matchbox-1.0.1/bw_matchbox/bin/matchbox.py
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-07 13:45:04.164508 bw_matchbox-1.0.1/bw_matchbox/data/
+-rw-r--r--   0 cmutel     (501) staff       (20)   123246 2023-08-03 14:06:22.000000 bw_matchbox-1.0.1/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-mining.json
+-rw-r--r--   0 cmutel     (501) staff       (20)    93862 2023-07-24 11:16:50.000000 bw_matchbox-1.0.1/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-string-matching.json
+-rw-r--r--   0 cmutel     (501) staff       (20)   116072 2023-08-03 14:06:22.000000 bw_matchbox-1.0.1/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-transport.json
+-rw-r--r--   0 cmutel     (501) staff       (20)      603 2023-07-24 11:16:50.000000 bw_matchbox-1.0.1/bw_matchbox/data/dare.json
+-rw-r--r--   0 cmutel     (501) staff       (20)     2204 2023-08-07 13:25:08.000000 bw_matchbox-1.0.1/bw_matchbox/utils.py
+-rw-r--r--   0 cmutel     (501) staff       (20)    22989 2023-08-07 13:42:11.000000 bw_matchbox-1.0.1/bw_matchbox/webapp.py
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-07 13:45:04.165585 bw_matchbox-1.0.1/bw_matchbox.egg-info/
+-rw-r--r--   0 cmutel     (501) staff       (20)     6361 2023-08-07 13:45:04.000000 bw_matchbox-1.0.1/bw_matchbox.egg-info/PKG-INFO
+-rw-r--r--   0 cmutel     (501) staff       (20)     5090 2023-08-07 13:45:04.000000 bw_matchbox-1.0.1/bw_matchbox.egg-info/SOURCES.txt
+-rw-r--r--   0 cmutel     (501) staff       (20)        1 2023-08-07 13:45:04.000000 bw_matchbox-1.0.1/bw_matchbox.egg-info/dependency_links.txt
+-rw-r--r--   0 cmutel     (501) staff       (20)       59 2023-08-07 13:45:04.000000 bw_matchbox-1.0.1/bw_matchbox.egg-info/entry_points.txt
+-rw-r--r--   0 cmutel     (501) staff       (20)        1 2023-07-24 11:26:00.000000 bw_matchbox-1.0.1/bw_matchbox.egg-info/not-zip-safe
+-rw-r--r--   0 cmutel     (501) staff       (20)      167 2023-08-07 13:45:04.000000 bw_matchbox-1.0.1/bw_matchbox.egg-info/requires.txt
+-rw-r--r--   0 cmutel     (501) staff       (20)       12 2023-08-07 13:45:04.000000 bw_matchbox-1.0.1/bw_matchbox.egg-info/top_level.txt
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-07 13:45:04.164644 bw_matchbox-1.0.1/docs/
+-rw-r--r--   0 cmutel     (501) staff       (20)     1145 2023-07-24 11:16:50.000000 bw_matchbox-1.0.1/docs/conf.py
+-rw-r--r--   0 cmutel     (501) staff       (20)       87 2023-07-24 11:16:50.000000 bw_matchbox-1.0.1/pyproject.toml
+-rw-r--r--   0 cmutel     (501) staff       (20)     1900 2023-08-07 13:45:04.167573 bw_matchbox-1.0.1/setup.cfg
```

### Comparing `bw_matchbox-1.0.0/LICENSE` & `bw_matchbox-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.0/PKG-INFO` & `bw_matchbox-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bw_matchbox
-Version: 1.0.0
+Version: 1.0.1
 Summary: Browser to match Brightway databases
 Home-page: https://github.com/cauldron/bw_matchbox
 Author: Chris Mutel
 Author-email: <cmutel@gmail.com>
 Maintainer: Chris Mutel
 Maintainer-email: <cmutel@gmail.com>
 License: MIT
```

### Comparing `bw_matchbox-1.0.0/README.md` & `bw_matchbox-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.0/bw_matchbox/assets/css/common-modal.css` & `bw_matchbox-1.0.1/bw_matchbox/assets/css/common-modal.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.0/bw_matchbox/assets/css/common.css` & `bw_matchbox-1.0.1/bw_matchbox/assets/css/common.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.0/bw_matchbox/assets/css/compare.css` & `bw_matchbox-1.0.1/bw_matchbox/assets/css/compare.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.0/bw_matchbox/assets/css/customizations.css` & `bw_matchbox-1.0.1/bw_matchbox/assets/css/customizations.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.0/bw_matchbox/assets/css/fixed-table.css` & `bw_matchbox-1.0.1/bw_matchbox/assets/css/fixed-table.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.0/bw_matchbox/assets/css/normalize.css` & `bw_matchbox-1.0.1/bw_matchbox/assets/css/normalize.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.0/bw_matchbox/assets/css/processes-list.css` & `bw_matchbox-1.0.1/bw_matchbox/assets/css/processes-list.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.0/bw_matchbox/assets/css/skeleton.css` & `bw_matchbox-1.0.1/bw_matchbox/assets/css/skeleton.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.0/bw_matchbox/assets/css/tooltip.css` & `bw_matchbox-1.0.1/bw_matchbox/assets/css/tooltip.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.0/bw_matchbox/assets/images/favicon.ico` & `bw_matchbox-1.0.1/bw_matchbox/assets/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.0/bw_matchbox/assets/js/Compare/CompareCore.js` & `bw_matchbox-1.0.1/bw_matchbox/assets/js/Compare/CompareCore.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -248,26 +248,23 @@
 
             removeRowHandler(element) {
                 CompareRowClick.disableRowClickHandler();
                 const rowId = element.closest('td').getAttribute('row_id');
                 const {
                     target_data
                 } = this.sharedData;
-
-                function removeValue(obj, index, arr) {
-                    console.log(this.CompareCore.sharedData);
+                document.getElementById('replace-with-target-arrow').style.display = 'none';
+                target_data.filter((obj, index, arr) => {
                     if (obj.row_id == rowId) {
-                        this.CompareCore.sharedData.comment += `* Removed exchange of ${obj.amount} ${obj.unit} ${obj.name} from ${obj.location}.\n`;
+                        this.sharedData.comment += `* Removed exchange of ${obj.amount} ${obj.unit} ${obj.name} from ${obj.location}.\n`;
                         arr.splice(index, 1);
                         return true;
                     }
                     return false;
-                }
-                document.getElementById('replace-with-target-arrow').style.display = 'none';
-                target_data.filter(removeValue);
+                });
                 this.buildTable('target-table', target_data, true);
             },
 
             expandRowHandler(element) {
                 const {
                     target_data
                 } = this.sharedData;
```

### Comparing `bw_matchbox-1.0.0/bw_matchbox/assets/js/Compare/CompareProxyDialogModal.js` & `bw_matchbox-1.0.1/bw_matchbox/assets/js/Compare/CompareProxyDialogModal.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.0/bw_matchbox/assets/js/Compare/CompareRowClick.js` & `bw_matchbox-1.0.1/bw_matchbox/assets/js/Compare/CompareRowClick.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.0/bw_matchbox/assets/js/Compare/CompareRowsHelpers.js` & `bw_matchbox-1.0.1/bw_matchbox/assets/js/Compare/CompareRowsHelpers.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.0/bw_matchbox/assets/js/ProcessesList/ProcessesList.js` & `bw_matchbox-1.0.1/bw_matchbox/assets/js/ProcessesList/ProcessesList.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.0/bw_matchbox/assets/js/ProcessesList/ProcessesListConstants.js` & `bw_matchbox-1.0.1/bw_matchbox/assets/js/ProcessesList/ProcessesListConstants.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.0/bw_matchbox/assets/js/ProcessesList/ProcessesListData.js` & `bw_matchbox-1.0.1/bw_matchbox/assets/js/ProcessesList/ProcessesListData.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.0/bw_matchbox/assets/js/ProcessesList/ProcessesListDataLoad.js` & `bw_matchbox-1.0.1/bw_matchbox/assets/js/ProcessesList/ProcessesListDataLoad.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.0/bw_matchbox/assets/js/ProcessesList/ProcessesListDataRender.js` & `bw_matchbox-1.0.1/bw_matchbox/assets/js/ProcessesList/ProcessesListDataRender.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.0/bw_matchbox/assets/js/ProcessesList/ProcessesListNodes.js` & `bw_matchbox-1.0.1/bw_matchbox/assets/js/ProcessesList/ProcessesListNodes.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.0/bw_matchbox/assets/js/ProcessesList/ProcessesListPagination.UNUSED.js` & `bw_matchbox-1.0.1/bw_matchbox/assets/js/ProcessesList/ProcessesListPagination.UNUSED.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.0/bw_matchbox/assets/js/ProcessesList/ProcessesListSearch.js` & `bw_matchbox-1.0.1/bw_matchbox/assets/js/ProcessesList/ProcessesListSearch.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.0/bw_matchbox/assets/js/ProcessesList/ProcessesListStates.js` & `bw_matchbox-1.0.1/bw_matchbox/assets/js/ProcessesList/ProcessesListStates.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.0/bw_matchbox/assets/js/common/CommonHelpers.js` & `bw_matchbox-1.0.1/bw_matchbox/assets/js/common/CommonHelpers.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.0/bw_matchbox/assets/js/common/CommonModal.js` & `bw_matchbox-1.0.1/bw_matchbox/assets/js/common/CommonModal.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.0/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.js` & `bw_matchbox-1.0.1/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.0/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.min.js` & `bw_matchbox-1.0.1/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.min.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.0/bw_matchbox/assets/templates/common-modal.html` & `bw_matchbox-1.0.1/bw_matchbox/assets/templates/common-modal.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.0/bw_matchbox/assets/templates/compare.html` & `bw_matchbox-1.0.1/bw_matchbox/assets/templates/compare.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.0/bw_matchbox/assets/templates/databases.html` & `bw_matchbox-1.0.1/bw_matchbox/assets/templates/databases.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.0/bw_matchbox/assets/templates/header.html` & `bw_matchbox-1.0.1/bw_matchbox/assets/templates/header.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.0/bw_matchbox/assets/templates/index.html` & `bw_matchbox-1.0.1/bw_matchbox/assets/templates/index.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.0/bw_matchbox/assets/templates/match-status.html` & `bw_matchbox-1.0.1/bw_matchbox/assets/templates/match-status.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.0/bw_matchbox/assets/templates/match.html` & `bw_matchbox-1.0.1/bw_matchbox/assets/templates/match.html`

 * *Files 6% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 }
 
 var doSearch = function () {
   var qs = encodeURIComponent(searchBar.value);
   if (qs) {
     const req = new XMLHttpRequest();
     req.addEventListener('load', search_result_updater);
-    req.open('GET', '{{ url_for('search') }}?e=1&source={{ ds.id }}&database=ecoinvent-3.9-cutoff&q=' + qs);
+    req.open('GET', '{{ url_for('search') }}?e=1&source={{ ds.id }}&database={{ target }}&q=' + qs);
     req.send();
   };
 };
 
 searchBar.addEventListener('focusout', doSearch);
 searchBar.addEventListener('keypress', function(event) {
   if (event.key === 'Enter') {
```

### Comparing `bw_matchbox-1.0.0/bw_matchbox/assets/templates/navigation.html` & `bw_matchbox-1.0.1/bw_matchbox/assets/templates/navigation.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.0/bw_matchbox/assets/templates/process_detail.html` & `bw_matchbox-1.0.1/bw_matchbox/assets/templates/process_detail.html`

 * *Files 12% similar despite different names*

```diff
@@ -37,42 +37,23 @@
       <h2>Technosphere Inputs</h2>
       <table width="100%">
         <tr>
           <th>Amount</th>
           <th>Name</th>
           <th>Location</th>
           <th>Unit</th>
-          {% if show_matching %}
-            <th>Matched</th>
-            <th>Action</th>
-          {% endif %}
+          <th>Matched</th>
         </tr>
         {% for row in technosphere %}
         <tr>
           <td>{{row.amount}}</td>
           <td><a href="{{ url_for('process_detail', id=row.input.id) }}">{{row.input.name}}</a></td>
           <td>{{row.input.location}}</td>
           <td>{{row.input.unit}}</td>
-          {% if show_matching %}
-            <td>{% if row.matched %}<i class="fa-solid fa-check"></i>{% else %}<i class="fa-solid fa-circle-xmark"></i>{% endif %}</td>
-            <td>
-              {% if row.matched %}
-                <div class="tooltip">
-                    <a class="button button-primary" href="{{ url_for('compare', source=row.input.id, target=row.match.id)}}">Compare</a>
-                    <div class="left">
-                        <p>{{ row.match.name }}</p>
-                        <p>{{ row.match.unit }}</p>
-                        <p>{{ row.match.location }}</p>
-                    </div>
-                </div>
-              {%  else %}
-                <a class="button button-primary" target="_blank" href="{{ url_for('match', source=row.input.id) }}">Match</a>
-              {% endif %}
-            </td>
-          {% endif %}
+          <td>{% if row.matched %}<i class="fa-solid fa-check"></i>{% else %}<i class="fa-solid fa-circle-xmark"></i>{% endif %}</td>
         </tr>
         {% endfor %}
       </table>
       <h2>Biosphere Inputs</h2>
       {% if biosphere|length > 50 or not biosphere|length %}
       <p>{{ biosphere|length }} biosphere exchanges</p>
       {% else %}
@@ -89,14 +70,38 @@
             <td>{{ exc.input.name }}</td>
             <td>{{ exc.input.categories|join("|") }}</td>
             <td>{{ exc.input.unit }}</td>
           </tr>
         {% endfor %}
       {% endif %}
       </table>
+      <h2>Consuming processes ({{ total_consumers }})</h2>
+      {% if not total_consumers %}
+      <p>No consuming processes</p>
+      {% elif total_consumers > 50 %}
+      <p>Showing 50 of {{ total_consumers }}</p>
+      {% endif %}
+      {% if total_consumers %}
+      <table width="100%">
+        <tr>
+          <th>Amount</th>
+          <th>Name</th>
+          <th>Location</th>
+          <th>Unit</th>
+        </tr>
+        {% for exc in consumers %}
+          <tr>
+            <td>{{ exc.amount }}</td>
+            <td>{{ exc.output.name }}</td>
+            <td>{{ exc.output.location }}</td>
+            <td>{{ exc.output.unit }}</td>
+          </tr>
+        {% endfor %}
+      {% endif %}
+      </table>
     </div>
   </div>
 </div>
 
 <script type="text/javascript">
 function markWaitlist (button) {
   var url = "{{ url_for('add_attribute', id=ds.id, attr='waitlist', value='1')|safe }}";
```

#### html2text {}

```diff
@@ -21,31 +21,33 @@
     * Proxy: {{_proxy_node_}}
     * {% endif %} {% if reference_node %}
     * Proxy for: {{_reference_node_}}
     * {% endif %} {% if match_type %}
     * Match type: {{ match_type }}
     * {% endif %}
 ***** Technosphere Inputs *****
-Amount        Name              Location              Unit              Matched     Action
-                                                                                    {% if row.matched
-                                                                                    %}
-                                                                                    Compare
-                                                                                    {{ row.match.name
-                                                                        {% if       }}
-{             {                 {                     {                 row.matched {{ row.match.unit
-{row.amount}} {row.input.name}} {row.input.location}} {row.input.unit}} %}{% else   }}
-                                                                        %}{% endif  {
-                                                                        %}          {
-                                                                                    row.match.location
-                                                                                    }}
-                                                                                    {% else %} Match
-                                                                                    {% endif %}
+Amount        Name              Location              Unit              Matched
+                                                                        {% if
+{             {                 {                     {                 row.matched
+{row.amount}} {row.input.name}} {row.input.location}} {row.input.unit}} %}{% else
+                                                                        %}{% endif
+                                                                        %}
 ***** Biosphere Inputs *****
 {% if biosphere|length > 50 or not biosphere|length %}
 {{ biosphere|length }} biosphere exchanges
 {% else %}
 Amount           Name              Categories                Unit
                                    {
 {{ exc.amount }} {{ exc.input.name {                         {{ exc.input.unit
                  }}                exc.input.categories|join }}
                                    ("|") }}
+***** Consuming processes ({{ total_consumers }}) *****
+{% if not total_consumers %}
+No consuming processes
+{% elif total_consumers > 50 %}
+Showing 50 of {{ total_consumers }}
+{% endif %} {% if total_consumers %}
+Amount           Name               Location              Unit
+                 {{ exc.output.name {
+{{ exc.amount }} }}                 { exc.output.location {{ exc.output.unit }}
+                                    }}
  {% include 'footer.html' %}
```

### Comparing `bw_matchbox-1.0.0/bw_matchbox/assets/templates/project.html` & `bw_matchbox-1.0.1/bw_matchbox/assets/templates/project.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.0/bw_matchbox/assets/templates/search.html` & `bw_matchbox-1.0.1/bw_matchbox/assets/templates/search.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.0/bw_matchbox/assets/templates/search_result.html` & `bw_matchbox-1.0.1/bw_matchbox/assets/templates/search_result.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.0/bw_matchbox/assets/templates/select_files.html` & `bw_matchbox-1.0.1/bw_matchbox/assets/templates/select_files.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.0/bw_matchbox/bin/matchbox.py` & `bw_matchbox-1.0.1/bw_matchbox/bin/matchbox.py`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.0/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-mining.json` & `bw_matchbox-1.0.1/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-mining.json`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.0/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-string-matching.json` & `bw_matchbox-1.0.1/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-string-matching.json`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.0/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-transport.json` & `bw_matchbox-1.0.1/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-transport.json`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.0/bw_matchbox/data/dare.json` & `bw_matchbox-1.0.1/bw_matchbox/data/dare.json`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.0/bw_matchbox/utils.py` & `bw_matchbox-1.0.1/bw_matchbox/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import json
 import importlib.metadata
+import json
 from pathlib import Path
 from typing import Optional, Union
 
 from Levenshtein import distance
 
 
 def get_version_tuple() -> tuple:
@@ -62,14 +62,15 @@
     "1": "No direct match available",
     "2": "Direct match with near-identical data",
     "3": "Match with updated data",
     "4": "Match with updated data and adding source transport",
     "5": "Match with market and replace or remove transport",
     "6": "Match with market and replace or remove transport and loss factor",
     "7": "Equivalent datasets after modification",
+    "8": "Replace aggregated with unit process",
 }
 
 
 def get_match_types(output_dir: Path) -> dict:
     match_types_file = output_dir / "match_types.json"
     try:
         return json.load(open(match_types_file))
```

### Comparing `bw_matchbox-1.0.0/bw_matchbox/webapp.py` & `bw_matchbox-1.0.1/bw_matchbox/webapp.py`

 * *Files 2% similar despite different names*

```diff
@@ -510,16 +510,17 @@
         target=t,
         file_number=sum(1 for obj in files if obj["enabled"]),
         user=auth.current_user(),
         same_name_count=same_name_count,
         same_name=same_name,
         technosphere=technosphere,
         biosphere=biosphere,
-        show_matching=False,
         match_type=matchbox_app.config["mb_match_types"].get(node.get("match_type")),
+        total_consumers=len(node.upstream()),
+        consumers=list(node.upstream())[:50],
     )
 
 
 @matchbox_app.route("/multi-match/<id>", methods=["GET"])
 @auth.login_required
 def multi_match(id):
     context = get_context()
```

### Comparing `bw_matchbox-1.0.0/bw_matchbox.egg-info/PKG-INFO` & `bw_matchbox-1.0.1/bw_matchbox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bw-matchbox
-Version: 1.0.0
+Version: 1.0.1
 Summary: Browser to match Brightway databases
 Home-page: https://github.com/cauldron/bw_matchbox
 Author: Chris Mutel
 Author-email: <cmutel@gmail.com>
 Maintainer: Chris Mutel
 Maintainer-email: <cmutel@gmail.com>
 License: MIT
```

### Comparing `bw_matchbox-1.0.0/bw_matchbox.egg-info/SOURCES.txt` & `bw_matchbox-1.0.1/bw_matchbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.0/docs/conf.py` & `bw_matchbox-1.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.0/setup.cfg` & `bw_matchbox-1.0.1/setup.cfg`

 * *Files identical despite different names*

