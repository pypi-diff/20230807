# Comparing `tmp/bw_matchbox-0.7.0.tar.gz` & `tmp/bw_matchbox-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bw_matchbox-0.7.0.tar", last modified: Sun Aug  6 19:19:27 2023, max compression
+gzip compressed data, was "bw_matchbox-0.7.1.tar", last modified: Sun Aug  6 20:15:29 2023, max compression
```

## Comparing `bw_matchbox-0.7.0.tar` & `bw_matchbox-0.7.1.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-06 19:19:27.326846 bw_matchbox-0.7.0/
--rw-r--r--   0 chrismutel   (501) staff       (20)     1067 2023-06-20 12:26:53.000000 bw_matchbox-0.7.0/LICENSE
--rw-r--r--   0 chrismutel   (501) staff       (20)      226 2023-08-02 21:05:25.000000 bw_matchbox-0.7.0/MANIFEST.in
--rw-r--r--   0 chrismutel   (501) staff       (20)     6361 2023-08-06 19:19:27.326906 bw_matchbox-0.7.0/PKG-INFO
--rw-r--r--   0 chrismutel   (501) staff       (20)     5337 2023-08-05 17:26:08.000000 bw_matchbox-0.7.0/README.md
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-06 19:19:27.312123 bw_matchbox-0.7.0/bw_matchbox/
--rw-r--r--   0 chrismutel   (501) staff       (20)        6 2023-08-06 19:19:05.000000 bw_matchbox-0.7.0/bw_matchbox/VERSION
--rw-r--r--   0 chrismutel   (501) staff       (20)      215 2023-08-01 17:17:21.000000 bw_matchbox-0.7.0/bw_matchbox/__init__.py
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-06 19:19:27.310431 bw_matchbox-0.7.0/bw_matchbox/assets/
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-06 19:19:27.314892 bw_matchbox-0.7.0/bw_matchbox/assets/css/
--rw-r--r--   0 chrismutel   (501) staff       (20)     3297 2023-08-06 18:22:10.000000 bw_matchbox-0.7.0/bw_matchbox/assets/css/common-modal.css
--rw-r--r--   0 chrismutel   (501) staff       (20)     1922 2023-08-06 18:22:10.000000 bw_matchbox-0.7.0/bw_matchbox/assets/css/common.css
--rw-r--r--   0 chrismutel   (501) staff       (20)     4256 2023-08-06 18:22:10.000000 bw_matchbox-0.7.0/bw_matchbox/assets/css/compare.css
--rw-r--r--   0 chrismutel   (501) staff       (20)      640 2023-08-03 20:45:26.000000 bw_matchbox-0.7.0/bw_matchbox/assets/css/customizations.css
--rw-r--r--   0 chrismutel   (501) staff       (20)     1392 2023-08-04 13:00:53.000000 bw_matchbox-0.7.0/bw_matchbox/assets/css/fixed-table.css
--rw-r--r--   0 chrismutel   (501) staff       (20)     7618 2023-08-01 07:10:26.000000 bw_matchbox-0.7.0/bw_matchbox/assets/css/normalize.css
--rw-r--r--   0 chrismutel   (501) staff       (20)     4315 2023-08-06 18:22:10.000000 bw_matchbox-0.7.0/bw_matchbox/assets/css/processes-list.css
--rw-r--r--   0 chrismutel   (501) staff       (20)    11556 2023-08-01 07:10:26.000000 bw_matchbox-0.7.0/bw_matchbox/assets/css/skeleton.css
--rw-r--r--   0 chrismutel   (501) staff       (20)      916 2023-08-01 07:10:26.000000 bw_matchbox-0.7.0/bw_matchbox/assets/css/tooltip.css
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-06 19:19:27.315126 bw_matchbox-0.7.0/bw_matchbox/assets/images/
--rw-r--r--   0 chrismutel   (501) staff       (20)    32038 2023-06-20 12:27:44.000000 bw_matchbox-0.7.0/bw_matchbox/assets/images/favicon.ico
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-06 19:19:27.310326 bw_matchbox-0.7.0/bw_matchbox/assets/js/
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-06 19:19:27.316336 bw_matchbox-0.7.0/bw_matchbox/assets/js/Compare/
--rw-r--r--   0 chrismutel   (501) staff       (20)    20330 2023-08-06 19:03:10.000000 bw_matchbox-0.7.0/bw_matchbox/assets/js/Compare/CompareCore.js
--rw-r--r--   0 chrismutel   (501) staff       (20)     6194 2023-08-06 18:22:10.000000 bw_matchbox-0.7.0/bw_matchbox/assets/js/Compare/CompareProxyDialogModal.js
--rw-r--r--   0 chrismutel   (501) staff       (20)     1272 2023-08-04 16:42:28.000000 bw_matchbox-0.7.0/bw_matchbox/assets/js/Compare/CompareRowClick.js
--rw-r--r--   0 chrismutel   (501) staff       (20)    12879 2023-08-06 18:22:10.000000 bw_matchbox-0.7.0/bw_matchbox/assets/js/Compare/CompareRowsHelpers.js
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-06 19:19:27.317723 bw_matchbox-0.7.0/bw_matchbox/assets/js/ProcessesList/
--rw-r--r--   0 chrismutel   (501) staff       (20)     4388 2023-08-06 18:22:10.000000 bw_matchbox-0.7.0/bw_matchbox/assets/js/ProcessesList/ProcessesList.js
--rw-r--r--   0 chrismutel   (501) staff       (20)      885 2023-08-06 18:22:10.000000 bw_matchbox-0.7.0/bw_matchbox/assets/js/ProcessesList/ProcessesListConstants.js
--rw-r--r--   0 chrismutel   (501) staff       (20)     1452 2023-08-06 18:22:10.000000 bw_matchbox-0.7.0/bw_matchbox/assets/js/ProcessesList/ProcessesListData.js
--rw-r--r--   0 chrismutel   (501) staff       (20)     5632 2023-08-06 18:22:10.000000 bw_matchbox-0.7.0/bw_matchbox/assets/js/ProcessesList/ProcessesListDataLoad.js
--rw-r--r--   0 chrismutel   (501) staff       (20)     3447 2023-08-06 18:22:10.000000 bw_matchbox-0.7.0/bw_matchbox/assets/js/ProcessesList/ProcessesListDataRender.js
--rw-r--r--   0 chrismutel   (501) staff       (20)     1081 2023-08-06 18:22:10.000000 bw_matchbox-0.7.0/bw_matchbox/assets/js/ProcessesList/ProcessesListNodes.js
--rw-r--r--   0 chrismutel   (501) staff       (20)     4862 2023-08-06 18:22:10.000000 bw_matchbox-0.7.0/bw_matchbox/assets/js/ProcessesList/ProcessesListPagination.UNUSED.js
--rw-r--r--   0 chrismutel   (501) staff       (20)     3321 2023-08-06 18:22:10.000000 bw_matchbox-0.7.0/bw_matchbox/assets/js/ProcessesList/ProcessesListSearch.js
--rw-r--r--   0 chrismutel   (501) staff       (20)     9995 2023-08-06 18:22:10.000000 bw_matchbox-0.7.0/bw_matchbox/assets/js/ProcessesList/ProcessesListStates.js
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-06 19:19:27.318071 bw_matchbox-0.7.0/bw_matchbox/assets/js/common/
--rw-r--r--   0 chrismutel   (501) staff       (20)     5634 2023-08-04 13:00:53.000000 bw_matchbox-0.7.0/bw_matchbox/assets/js/common/CommonHelpers.js
--rw-r--r--   0 chrismutel   (501) staff       (20)     5781 2023-08-06 18:22:10.000000 bw_matchbox-0.7.0/bw_matchbox/assets/js/common/CommonModal.js
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-06 19:19:27.310372 bw_matchbox-0.7.0/bw_matchbox/assets/js/libs/
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-06 19:19:27.318408 bw_matchbox-0.7.0/bw_matchbox/assets/js/libs/ym/
--rw-r--r--   0 chrismutel   (501) staff       (20)    13286 2023-08-03 20:45:26.000000 bw_matchbox-0.7.0/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.js
--rw-r--r--   0 chrismutel   (501) staff       (20)     6018 2023-08-03 20:45:26.000000 bw_matchbox-0.7.0/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.min.js
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-06 19:19:27.321997 bw_matchbox-0.7.0/bw_matchbox/assets/templates/
--rw-r--r--   0 chrismutel   (501) staff       (20)      756 2023-08-04 13:00:53.000000 bw_matchbox-0.7.0/bw_matchbox/assets/templates/common-modal.html
--rw-r--r--   0 chrismutel   (501) staff       (20)     3880 2023-08-06 18:22:10.000000 bw_matchbox-0.7.0/bw_matchbox/assets/templates/compare.html
--rw-r--r--   0 chrismutel   (501) staff       (20)     2681 2023-08-05 17:26:08.000000 bw_matchbox-0.7.0/bw_matchbox/assets/templates/databases.html
--rw-r--r--   0 chrismutel   (501) staff       (20)      461 2023-07-23 15:09:13.000000 bw_matchbox-0.7.0/bw_matchbox/assets/templates/expand.html
--rw-r--r--   0 chrismutel   (501) staff       (20)       16 2023-06-20 12:27:44.000000 bw_matchbox-0.7.0/bw_matchbox/assets/templates/footer.html
--rw-r--r--   0 chrismutel   (501) staff       (20)     2666 2023-08-04 13:00:53.000000 bw_matchbox-0.7.0/bw_matchbox/assets/templates/header.html
--rw-r--r--   0 chrismutel   (501) staff       (20)     6969 2023-08-06 18:22:10.000000 bw_matchbox-0.7.0/bw_matchbox/assets/templates/index.html
--rw-r--r--   0 chrismutel   (501) staff       (20)      733 2023-06-21 04:56:26.000000 bw_matchbox-0.7.0/bw_matchbox/assets/templates/match-status.html
--rw-r--r--   0 chrismutel   (501) staff       (20)     1721 2023-08-03 20:45:26.000000 bw_matchbox-0.7.0/bw_matchbox/assets/templates/match.html
--rw-r--r--   0 chrismutel   (501) staff       (20)      734 2023-08-05 17:26:08.000000 bw_matchbox-0.7.0/bw_matchbox/assets/templates/navigation.html
--rw-r--r--   0 chrismutel   (501) staff       (20)     5932 2023-08-06 18:58:22.000000 bw_matchbox-0.7.0/bw_matchbox/assets/templates/process_detail.html
--rw-r--r--   0 chrismutel   (501) staff       (20)      599 2023-07-22 21:06:00.000000 bw_matchbox-0.7.0/bw_matchbox/assets/templates/project.html
--rw-r--r--   0 chrismutel   (501) staff       (20)      412 2023-08-01 07:10:26.000000 bw_matchbox-0.7.0/bw_matchbox/assets/templates/search-embedded.html
--rw-r--r--   0 chrismutel   (501) staff       (20)      850 2023-06-20 12:27:44.000000 bw_matchbox-0.7.0/bw_matchbox/assets/templates/search.html
--rw-r--r--   0 chrismutel   (501) staff       (20)      947 2023-06-20 12:27:44.000000 bw_matchbox-0.7.0/bw_matchbox/assets/templates/search_result.html
--rw-r--r--   0 chrismutel   (501) staff       (20)     1243 2023-07-23 08:33:52.000000 bw_matchbox-0.7.0/bw_matchbox/assets/templates/select_files.html
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-06 19:19:27.322398 bw_matchbox-0.7.0/bw_matchbox/bin/
--rw-r--r--   0 chrismutel   (501) staff       (20)        0 2023-06-20 12:27:44.000000 bw_matchbox-0.7.0/bw_matchbox/bin/__init__.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     2692 2023-08-05 17:26:08.000000 bw_matchbox-0.7.0/bw_matchbox/bin/matchbox.py
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-06 19:19:27.324551 bw_matchbox-0.7.0/bw_matchbox/data/
--rw-r--r--   0 chrismutel   (501) staff       (20)   123246 2023-08-01 17:17:21.000000 bw_matchbox-0.7.0/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-mining.json
--rw-r--r--   0 chrismutel   (501) staff       (20)    93862 2023-07-23 09:30:53.000000 bw_matchbox-0.7.0/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-string-matching.json
--rw-r--r--   0 chrismutel   (501) staff       (20)   116072 2023-08-01 17:17:21.000000 bw_matchbox-0.7.0/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-transport.json
--rw-r--r--   0 chrismutel   (501) staff       (20)      603 2023-07-23 09:34:59.000000 bw_matchbox-0.7.0/bw_matchbox/data/dare.json
--rw-r--r--   0 chrismutel   (501) staff       (20)     2155 2023-08-06 18:22:10.000000 bw_matchbox-0.7.0/bw_matchbox/utils.py
--rw-r--r--   0 chrismutel   (501) staff       (20)    22926 2023-08-06 19:01:25.000000 bw_matchbox-0.7.0/bw_matchbox/webapp.py
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-06 19:19:27.325754 bw_matchbox-0.7.0/bw_matchbox.egg-info/
--rw-r--r--   0 chrismutel   (501) staff       (20)     6361 2023-08-06 19:19:27.000000 bw_matchbox-0.7.0/bw_matchbox.egg-info/PKG-INFO
--rw-r--r--   0 chrismutel   (501) staff       (20)     5090 2023-08-06 19:19:27.000000 bw_matchbox-0.7.0/bw_matchbox.egg-info/SOURCES.txt
--rw-r--r--   0 chrismutel   (501) staff       (20)        1 2023-08-06 19:19:27.000000 bw_matchbox-0.7.0/bw_matchbox.egg-info/dependency_links.txt
--rw-r--r--   0 chrismutel   (501) staff       (20)       59 2023-08-06 19:19:27.000000 bw_matchbox-0.7.0/bw_matchbox.egg-info/entry_points.txt
--rw-r--r--   0 chrismutel   (501) staff       (20)        1 2023-07-23 07:30:31.000000 bw_matchbox-0.7.0/bw_matchbox.egg-info/not-zip-safe
--rw-r--r--   0 chrismutel   (501) staff       (20)      167 2023-08-06 19:19:27.000000 bw_matchbox-0.7.0/bw_matchbox.egg-info/requires.txt
--rw-r--r--   0 chrismutel   (501) staff       (20)       12 2023-08-06 19:19:27.000000 bw_matchbox-0.7.0/bw_matchbox.egg-info/top_level.txt
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-06 19:19:27.324798 bw_matchbox-0.7.0/docs/
--rw-r--r--   0 chrismutel   (501) staff       (20)     1145 2023-07-23 07:23:19.000000 bw_matchbox-0.7.0/docs/conf.py
--rw-r--r--   0 chrismutel   (501) staff       (20)       87 2023-06-20 12:26:53.000000 bw_matchbox-0.7.0/pyproject.toml
--rw-r--r--   0 chrismutel   (501) staff       (20)     1900 2023-08-06 19:19:27.327275 bw_matchbox-0.7.0/setup.cfg
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-06 20:15:29.989277 bw_matchbox-0.7.1/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1067 2023-06-20 12:26:53.000000 bw_matchbox-0.7.1/LICENSE
+-rw-r--r--   0 chrismutel   (501) staff       (20)      226 2023-08-02 21:05:25.000000 bw_matchbox-0.7.1/MANIFEST.in
+-rw-r--r--   0 chrismutel   (501) staff       (20)     6361 2023-08-06 20:15:29.989342 bw_matchbox-0.7.1/PKG-INFO
+-rw-r--r--   0 chrismutel   (501) staff       (20)     5337 2023-08-05 17:26:08.000000 bw_matchbox-0.7.1/README.md
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-06 20:15:29.973949 bw_matchbox-0.7.1/bw_matchbox/
+-rw-r--r--   0 chrismutel   (501) staff       (20)        6 2023-08-06 20:15:09.000000 bw_matchbox-0.7.1/bw_matchbox/VERSION
+-rw-r--r--   0 chrismutel   (501) staff       (20)      215 2023-08-01 17:17:21.000000 bw_matchbox-0.7.1/bw_matchbox/__init__.py
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-06 20:15:29.972210 bw_matchbox-0.7.1/bw_matchbox/assets/
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-06 20:15:29.976582 bw_matchbox-0.7.1/bw_matchbox/assets/css/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     3297 2023-08-06 18:22:10.000000 bw_matchbox-0.7.1/bw_matchbox/assets/css/common-modal.css
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1922 2023-08-06 18:22:10.000000 bw_matchbox-0.7.1/bw_matchbox/assets/css/common.css
+-rw-r--r--   0 chrismutel   (501) staff       (20)     4256 2023-08-06 18:22:10.000000 bw_matchbox-0.7.1/bw_matchbox/assets/css/compare.css
+-rw-r--r--   0 chrismutel   (501) staff       (20)      640 2023-08-03 20:45:26.000000 bw_matchbox-0.7.1/bw_matchbox/assets/css/customizations.css
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1392 2023-08-04 13:00:53.000000 bw_matchbox-0.7.1/bw_matchbox/assets/css/fixed-table.css
+-rw-r--r--   0 chrismutel   (501) staff       (20)     7618 2023-08-01 07:10:26.000000 bw_matchbox-0.7.1/bw_matchbox/assets/css/normalize.css
+-rw-r--r--   0 chrismutel   (501) staff       (20)     4315 2023-08-06 18:22:10.000000 bw_matchbox-0.7.1/bw_matchbox/assets/css/processes-list.css
+-rw-r--r--   0 chrismutel   (501) staff       (20)    11556 2023-08-01 07:10:26.000000 bw_matchbox-0.7.1/bw_matchbox/assets/css/skeleton.css
+-rw-r--r--   0 chrismutel   (501) staff       (20)      916 2023-08-01 07:10:26.000000 bw_matchbox-0.7.1/bw_matchbox/assets/css/tooltip.css
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-06 20:15:29.976817 bw_matchbox-0.7.1/bw_matchbox/assets/images/
+-rw-r--r--   0 chrismutel   (501) staff       (20)    32038 2023-06-20 12:27:44.000000 bw_matchbox-0.7.1/bw_matchbox/assets/images/favicon.ico
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-06 20:15:29.972106 bw_matchbox-0.7.1/bw_matchbox/assets/js/
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-06 20:15:29.978132 bw_matchbox-0.7.1/bw_matchbox/assets/js/Compare/
+-rw-r--r--   0 chrismutel   (501) staff       (20)    20394 2023-08-06 20:10:31.000000 bw_matchbox-0.7.1/bw_matchbox/assets/js/Compare/CompareCore.js
+-rw-r--r--   0 chrismutel   (501) staff       (20)     6194 2023-08-06 18:22:10.000000 bw_matchbox-0.7.1/bw_matchbox/assets/js/Compare/CompareProxyDialogModal.js
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1272 2023-08-04 16:42:28.000000 bw_matchbox-0.7.1/bw_matchbox/assets/js/Compare/CompareRowClick.js
+-rw-r--r--   0 chrismutel   (501) staff       (20)    12879 2023-08-06 18:22:10.000000 bw_matchbox-0.7.1/bw_matchbox/assets/js/Compare/CompareRowsHelpers.js
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-06 20:15:29.979534 bw_matchbox-0.7.1/bw_matchbox/assets/js/ProcessesList/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     4388 2023-08-06 18:22:10.000000 bw_matchbox-0.7.1/bw_matchbox/assets/js/ProcessesList/ProcessesList.js
+-rw-r--r--   0 chrismutel   (501) staff       (20)      885 2023-08-06 18:22:10.000000 bw_matchbox-0.7.1/bw_matchbox/assets/js/ProcessesList/ProcessesListConstants.js
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1452 2023-08-06 18:22:10.000000 bw_matchbox-0.7.1/bw_matchbox/assets/js/ProcessesList/ProcessesListData.js
+-rw-r--r--   0 chrismutel   (501) staff       (20)     5632 2023-08-06 18:22:10.000000 bw_matchbox-0.7.1/bw_matchbox/assets/js/ProcessesList/ProcessesListDataLoad.js
+-rw-r--r--   0 chrismutel   (501) staff       (20)     3447 2023-08-06 18:22:10.000000 bw_matchbox-0.7.1/bw_matchbox/assets/js/ProcessesList/ProcessesListDataRender.js
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1081 2023-08-06 18:22:10.000000 bw_matchbox-0.7.1/bw_matchbox/assets/js/ProcessesList/ProcessesListNodes.js
+-rw-r--r--   0 chrismutel   (501) staff       (20)     4862 2023-08-06 18:22:10.000000 bw_matchbox-0.7.1/bw_matchbox/assets/js/ProcessesList/ProcessesListPagination.UNUSED.js
+-rw-r--r--   0 chrismutel   (501) staff       (20)     3321 2023-08-06 18:22:10.000000 bw_matchbox-0.7.1/bw_matchbox/assets/js/ProcessesList/ProcessesListSearch.js
+-rw-r--r--   0 chrismutel   (501) staff       (20)     9995 2023-08-06 18:22:10.000000 bw_matchbox-0.7.1/bw_matchbox/assets/js/ProcessesList/ProcessesListStates.js
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-06 20:15:29.979916 bw_matchbox-0.7.1/bw_matchbox/assets/js/common/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     5634 2023-08-04 13:00:53.000000 bw_matchbox-0.7.1/bw_matchbox/assets/js/common/CommonHelpers.js
+-rw-r--r--   0 chrismutel   (501) staff       (20)     5781 2023-08-06 18:22:10.000000 bw_matchbox-0.7.1/bw_matchbox/assets/js/common/CommonModal.js
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-06 20:15:29.972148 bw_matchbox-0.7.1/bw_matchbox/assets/js/libs/
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-06 20:15:29.980349 bw_matchbox-0.7.1/bw_matchbox/assets/js/libs/ym/
+-rw-r--r--   0 chrismutel   (501) staff       (20)    13286 2023-08-03 20:45:26.000000 bw_matchbox-0.7.1/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.js
+-rw-r--r--   0 chrismutel   (501) staff       (20)     6018 2023-08-03 20:45:26.000000 bw_matchbox-0.7.1/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.min.js
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-06 20:15:29.984062 bw_matchbox-0.7.1/bw_matchbox/assets/templates/
+-rw-r--r--   0 chrismutel   (501) staff       (20)      756 2023-08-04 13:00:53.000000 bw_matchbox-0.7.1/bw_matchbox/assets/templates/common-modal.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)     3880 2023-08-06 18:22:10.000000 bw_matchbox-0.7.1/bw_matchbox/assets/templates/compare.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2681 2023-08-05 17:26:08.000000 bw_matchbox-0.7.1/bw_matchbox/assets/templates/databases.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)      461 2023-07-23 15:09:13.000000 bw_matchbox-0.7.1/bw_matchbox/assets/templates/expand.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)       16 2023-06-20 12:27:44.000000 bw_matchbox-0.7.1/bw_matchbox/assets/templates/footer.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2666 2023-08-04 13:00:53.000000 bw_matchbox-0.7.1/bw_matchbox/assets/templates/header.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)     6969 2023-08-06 18:22:10.000000 bw_matchbox-0.7.1/bw_matchbox/assets/templates/index.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)      733 2023-06-21 04:56:26.000000 bw_matchbox-0.7.1/bw_matchbox/assets/templates/match-status.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1721 2023-08-03 20:45:26.000000 bw_matchbox-0.7.1/bw_matchbox/assets/templates/match.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)      734 2023-08-05 17:26:08.000000 bw_matchbox-0.7.1/bw_matchbox/assets/templates/navigation.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)     5932 2023-08-06 18:58:22.000000 bw_matchbox-0.7.1/bw_matchbox/assets/templates/process_detail.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)      599 2023-07-22 21:06:00.000000 bw_matchbox-0.7.1/bw_matchbox/assets/templates/project.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)      412 2023-08-01 07:10:26.000000 bw_matchbox-0.7.1/bw_matchbox/assets/templates/search-embedded.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)      850 2023-06-20 12:27:44.000000 bw_matchbox-0.7.1/bw_matchbox/assets/templates/search.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)      947 2023-06-20 12:27:44.000000 bw_matchbox-0.7.1/bw_matchbox/assets/templates/search_result.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1243 2023-07-23 08:33:52.000000 bw_matchbox-0.7.1/bw_matchbox/assets/templates/select_files.html
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-06 20:15:29.984471 bw_matchbox-0.7.1/bw_matchbox/bin/
+-rw-r--r--   0 chrismutel   (501) staff       (20)        0 2023-06-20 12:27:44.000000 bw_matchbox-0.7.1/bw_matchbox/bin/__init__.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2692 2023-08-05 17:26:08.000000 bw_matchbox-0.7.1/bw_matchbox/bin/matchbox.py
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-06 20:15:29.986428 bw_matchbox-0.7.1/bw_matchbox/data/
+-rw-r--r--   0 chrismutel   (501) staff       (20)   123246 2023-08-01 17:17:21.000000 bw_matchbox-0.7.1/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-mining.json
+-rw-r--r--   0 chrismutel   (501) staff       (20)    93862 2023-07-23 09:30:53.000000 bw_matchbox-0.7.1/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-string-matching.json
+-rw-r--r--   0 chrismutel   (501) staff       (20)   116072 2023-08-01 17:17:21.000000 bw_matchbox-0.7.1/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-transport.json
+-rw-r--r--   0 chrismutel   (501) staff       (20)      603 2023-07-23 09:34:59.000000 bw_matchbox-0.7.1/bw_matchbox/data/dare.json
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2155 2023-08-06 18:22:10.000000 bw_matchbox-0.7.1/bw_matchbox/utils.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)    22926 2023-08-06 19:01:25.000000 bw_matchbox-0.7.1/bw_matchbox/webapp.py
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-06 20:15:29.987797 bw_matchbox-0.7.1/bw_matchbox.egg-info/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     6361 2023-08-06 20:15:29.000000 bw_matchbox-0.7.1/bw_matchbox.egg-info/PKG-INFO
+-rw-r--r--   0 chrismutel   (501) staff       (20)     5090 2023-08-06 20:15:29.000000 bw_matchbox-0.7.1/bw_matchbox.egg-info/SOURCES.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)        1 2023-08-06 20:15:29.000000 bw_matchbox-0.7.1/bw_matchbox.egg-info/dependency_links.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)       59 2023-08-06 20:15:29.000000 bw_matchbox-0.7.1/bw_matchbox.egg-info/entry_points.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)        1 2023-07-23 07:30:31.000000 bw_matchbox-0.7.1/bw_matchbox.egg-info/not-zip-safe
+-rw-r--r--   0 chrismutel   (501) staff       (20)      167 2023-08-06 20:15:29.000000 bw_matchbox-0.7.1/bw_matchbox.egg-info/requires.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)       12 2023-08-06 20:15:29.000000 bw_matchbox-0.7.1/bw_matchbox.egg-info/top_level.txt
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-06 20:15:29.986670 bw_matchbox-0.7.1/docs/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1145 2023-07-23 07:23:19.000000 bw_matchbox-0.7.1/docs/conf.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)       87 2023-06-20 12:26:53.000000 bw_matchbox-0.7.1/pyproject.toml
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1900 2023-08-06 20:15:29.989808 bw_matchbox-0.7.1/setup.cfg
```

### Comparing `bw_matchbox-0.7.0/LICENSE` & `bw_matchbox-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.7.0/PKG-INFO` & `bw_matchbox-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bw_matchbox
-Version: 0.7.0
+Version: 0.7.1
 Summary: Browser to match Brightway databases
 Home-page: https://github.com/cauldron/bw_matchbox
 Author: Chris Mutel
 Author-email: <cmutel@gmail.com>
 Maintainer: Chris Mutel
 Maintainer-email: <cmutel@gmail.com>
 License: MIT
```

### Comparing `bw_matchbox-0.7.0/README.md` & `bw_matchbox-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.7.0/bw_matchbox/assets/css/common-modal.css` & `bw_matchbox-0.7.1/bw_matchbox/assets/css/common-modal.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.7.0/bw_matchbox/assets/css/common.css` & `bw_matchbox-0.7.1/bw_matchbox/assets/css/common.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.7.0/bw_matchbox/assets/css/compare.css` & `bw_matchbox-0.7.1/bw_matchbox/assets/css/compare.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.7.0/bw_matchbox/assets/css/customizations.css` & `bw_matchbox-0.7.1/bw_matchbox/assets/css/customizations.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.7.0/bw_matchbox/assets/css/fixed-table.css` & `bw_matchbox-0.7.1/bw_matchbox/assets/css/fixed-table.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.7.0/bw_matchbox/assets/css/normalize.css` & `bw_matchbox-0.7.1/bw_matchbox/assets/css/normalize.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.7.0/bw_matchbox/assets/css/processes-list.css` & `bw_matchbox-0.7.1/bw_matchbox/assets/css/processes-list.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.7.0/bw_matchbox/assets/css/skeleton.css` & `bw_matchbox-0.7.1/bw_matchbox/assets/css/skeleton.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.7.0/bw_matchbox/assets/css/tooltip.css` & `bw_matchbox-0.7.1/bw_matchbox/assets/css/tooltip.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.7.0/bw_matchbox/assets/images/favicon.ico` & `bw_matchbox-0.7.1/bw_matchbox/assets/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.7.0/bw_matchbox/assets/js/Compare/CompareCore.js` & `bw_matchbox-0.7.1/bw_matchbox/assets/js/Compare/CompareCore.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -250,16 +250,17 @@
                 CompareRowClick.disableRowClickHandler();
                 const rowId = element.closest('td').getAttribute('row_id');
                 const {
                     target_data
                 } = this.sharedData;
 
                 function removeValue(obj, index, arr) {
+                    console.log(this.CompareCore.sharedData);
                     if (obj.row_id == rowId) {
-                        this.sharedData.comment += `* Removed exchange of ${obj.amount} ${obj.unit} ${obj.name} from ${obj.location}.\n`;
+                        this.CompareCore.sharedData.comment += `* Removed exchange of ${obj.amount} ${obj.unit} ${obj.name} from ${obj.location}.\n`;
                         arr.splice(index, 1);
                         return true;
                     }
                     return false;
                 }
                 document.getElementById('replace-with-target-arrow').style.display = 'none';
                 target_data.filter(removeValue);
```

### Comparing `bw_matchbox-0.7.0/bw_matchbox/assets/js/Compare/CompareProxyDialogModal.js` & `bw_matchbox-0.7.1/bw_matchbox/assets/js/Compare/CompareProxyDialogModal.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.7.0/bw_matchbox/assets/js/Compare/CompareRowClick.js` & `bw_matchbox-0.7.1/bw_matchbox/assets/js/Compare/CompareRowClick.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.7.0/bw_matchbox/assets/js/Compare/CompareRowsHelpers.js` & `bw_matchbox-0.7.1/bw_matchbox/assets/js/Compare/CompareRowsHelpers.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.7.0/bw_matchbox/assets/js/ProcessesList/ProcessesList.js` & `bw_matchbox-0.7.1/bw_matchbox/assets/js/ProcessesList/ProcessesList.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.7.0/bw_matchbox/assets/js/ProcessesList/ProcessesListConstants.js` & `bw_matchbox-0.7.1/bw_matchbox/assets/js/ProcessesList/ProcessesListConstants.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.7.0/bw_matchbox/assets/js/ProcessesList/ProcessesListData.js` & `bw_matchbox-0.7.1/bw_matchbox/assets/js/ProcessesList/ProcessesListData.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.7.0/bw_matchbox/assets/js/ProcessesList/ProcessesListDataLoad.js` & `bw_matchbox-0.7.1/bw_matchbox/assets/js/ProcessesList/ProcessesListDataLoad.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.7.0/bw_matchbox/assets/js/ProcessesList/ProcessesListDataRender.js` & `bw_matchbox-0.7.1/bw_matchbox/assets/js/ProcessesList/ProcessesListDataRender.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.7.0/bw_matchbox/assets/js/ProcessesList/ProcessesListNodes.js` & `bw_matchbox-0.7.1/bw_matchbox/assets/js/ProcessesList/ProcessesListNodes.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.7.0/bw_matchbox/assets/js/ProcessesList/ProcessesListPagination.UNUSED.js` & `bw_matchbox-0.7.1/bw_matchbox/assets/js/ProcessesList/ProcessesListPagination.UNUSED.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.7.0/bw_matchbox/assets/js/ProcessesList/ProcessesListSearch.js` & `bw_matchbox-0.7.1/bw_matchbox/assets/js/ProcessesList/ProcessesListSearch.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.7.0/bw_matchbox/assets/js/ProcessesList/ProcessesListStates.js` & `bw_matchbox-0.7.1/bw_matchbox/assets/js/ProcessesList/ProcessesListStates.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.7.0/bw_matchbox/assets/js/common/CommonHelpers.js` & `bw_matchbox-0.7.1/bw_matchbox/assets/js/common/CommonHelpers.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.7.0/bw_matchbox/assets/js/common/CommonModal.js` & `bw_matchbox-0.7.1/bw_matchbox/assets/js/common/CommonModal.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.7.0/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.js` & `bw_matchbox-0.7.1/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.7.0/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.min.js` & `bw_matchbox-0.7.1/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.min.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.7.0/bw_matchbox/assets/templates/common-modal.html` & `bw_matchbox-0.7.1/bw_matchbox/assets/templates/common-modal.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.7.0/bw_matchbox/assets/templates/compare.html` & `bw_matchbox-0.7.1/bw_matchbox/assets/templates/compare.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.7.0/bw_matchbox/assets/templates/databases.html` & `bw_matchbox-0.7.1/bw_matchbox/assets/templates/databases.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.7.0/bw_matchbox/assets/templates/header.html` & `bw_matchbox-0.7.1/bw_matchbox/assets/templates/header.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.7.0/bw_matchbox/assets/templates/index.html` & `bw_matchbox-0.7.1/bw_matchbox/assets/templates/index.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.7.0/bw_matchbox/assets/templates/match-status.html` & `bw_matchbox-0.7.1/bw_matchbox/assets/templates/match-status.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.7.0/bw_matchbox/assets/templates/match.html` & `bw_matchbox-0.7.1/bw_matchbox/assets/templates/match.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.7.0/bw_matchbox/assets/templates/navigation.html` & `bw_matchbox-0.7.1/bw_matchbox/assets/templates/navigation.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.7.0/bw_matchbox/assets/templates/process_detail.html` & `bw_matchbox-0.7.1/bw_matchbox/assets/templates/process_detail.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.7.0/bw_matchbox/assets/templates/project.html` & `bw_matchbox-0.7.1/bw_matchbox/assets/templates/project.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.7.0/bw_matchbox/assets/templates/search.html` & `bw_matchbox-0.7.1/bw_matchbox/assets/templates/search.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.7.0/bw_matchbox/assets/templates/search_result.html` & `bw_matchbox-0.7.1/bw_matchbox/assets/templates/search_result.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.7.0/bw_matchbox/assets/templates/select_files.html` & `bw_matchbox-0.7.1/bw_matchbox/assets/templates/select_files.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.7.0/bw_matchbox/bin/matchbox.py` & `bw_matchbox-0.7.1/bw_matchbox/bin/matchbox.py`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.7.0/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-mining.json` & `bw_matchbox-0.7.1/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-mining.json`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.7.0/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-string-matching.json` & `bw_matchbox-0.7.1/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-string-matching.json`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.7.0/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-transport.json` & `bw_matchbox-0.7.1/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-transport.json`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.7.0/bw_matchbox/data/dare.json` & `bw_matchbox-0.7.1/bw_matchbox/data/dare.json`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.7.0/bw_matchbox/utils.py` & `bw_matchbox-0.7.1/bw_matchbox/utils.py`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.7.0/bw_matchbox/webapp.py` & `bw_matchbox-0.7.1/bw_matchbox/webapp.py`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.7.0/bw_matchbox.egg-info/PKG-INFO` & `bw_matchbox-0.7.1/bw_matchbox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bw-matchbox
-Version: 0.7.0
+Version: 0.7.1
 Summary: Browser to match Brightway databases
 Home-page: https://github.com/cauldron/bw_matchbox
 Author: Chris Mutel
 Author-email: <cmutel@gmail.com>
 Maintainer: Chris Mutel
 Maintainer-email: <cmutel@gmail.com>
 License: MIT
```

### Comparing `bw_matchbox-0.7.0/bw_matchbox.egg-info/SOURCES.txt` & `bw_matchbox-0.7.1/bw_matchbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.7.0/docs/conf.py` & `bw_matchbox-0.7.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.7.0/setup.cfg` & `bw_matchbox-0.7.1/setup.cfg`

 * *Files identical despite different names*

