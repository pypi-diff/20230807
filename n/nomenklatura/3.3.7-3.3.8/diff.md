# Comparing `tmp/nomenklatura-3.3.7.tar.gz` & `tmp/nomenklatura-3.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nomenklatura-3.3.7.tar", last modified: Thu Aug  3 07:53:47 2023, max compression
+gzip compressed data, was "nomenklatura-3.3.8.tar", last modified: Mon Aug  7 16:22:38 2023, max compression
```

## Comparing `nomenklatura-3.3.7.tar` & `nomenklatura-3.3.8.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:53:47.405739 nomenklatura-3.3.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-08-03 07:53:47.405739 nomenklatura-3.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:53:47.389739 nomenklatura-3.3.7/nomenklatura/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:53:47.393739 nomenklatura-3.3.7/nomenklatura/data/
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/data/regression-v1.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/data/regression-v2.pkl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:53:47.393739 nomenklatura-3.3.7/nomenklatura/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/dataset/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/dataset/coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/dataset/publisher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/dataset/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/dataset/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:53:47.393739 nomenklatura-3.3.7/nomenklatura/enrich/
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/enrich/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/enrich/aleph.py
--rw-r--r--   0 runner    (1001) docker     (123)     5544 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/enrich/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/enrich/nominatim.py
--rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/enrich/opencorporates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:53:47.397739 nomenklatura-3.3.7/nomenklatura/enrich/wikidata/
--rw-r--r--   0 runner    (1001) docker     (123)     9872 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/enrich/wikidata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/enrich/wikidata/lang.py
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/enrich/wikidata/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/enrich/wikidata/props.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/enrich/wikidata/qualified.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/enrich/wikidata/value.py
--rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/enrich/yente.py
--rw-r--r--   0 runner    (1001) docker     (123)    15265 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:53:47.397739 nomenklatura-3.3.7/nomenklatura/index/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/index/entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/index/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/index/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/judgement.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:53:47.397739 nomenklatura-3.3.7/nomenklatura/matching/
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/matching/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:53:47.397739 nomenklatura-3.3.7/nomenklatura/matching/heuristic/
--rw-r--r--   0 runner    (1001) docker     (123)     5942 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/matching/heuristic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/matching/heuristic/logic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/matching/pairs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/matching/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/matching/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:53:47.401739 nomenklatura-3.3.7/nomenklatura/matching/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/matching/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/matching/v1/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/matching/v1/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/matching/v1/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/matching/v1/names.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/matching/v1/train.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/matching/v1/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:53:47.401739 nomenklatura-3.3.7/nomenklatura/matching/v2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/matching/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/matching/v2/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/matching/v2/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/matching/v2/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/matching/v2/names.py
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/matching/v2/train.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/matching/v2/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:53:47.401739 nomenklatura-3.3.7/nomenklatura/publish/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/publish/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/publish/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/publish/edges.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/publish/names.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:53:47.401739 nomenklatura-3.3.7/nomenklatura/resolver/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/resolver/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/resolver/edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/resolver/identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    12955 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/resolver/resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/senzing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:53:47.405739 nomenklatura-3.3.7/nomenklatura/statement/
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/statement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/statement/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     6283 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/statement/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     7897 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/statement/statement.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:53:47.405739 nomenklatura-3.3.7/nomenklatura/store/
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/store/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/store/level.py
--rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/store/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/store/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/stream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:53:47.405739 nomenklatura-3.3.7/nomenklatura/tui/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/tui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/tui/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/tui/comparison.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/tui/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/nomenklatura/xref.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:53:47.393739 nomenklatura-3.3.7/nomenklatura.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-08-03 07:53:47.000000 nomenklatura-3.3.7/nomenklatura.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-08-03 07:53:47.000000 nomenklatura-3.3.7/nomenklatura.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 07:53:47.000000 nomenklatura-3.3.7/nomenklatura.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-03 07:53:47.000000 nomenklatura-3.3.7/nomenklatura.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 07:53:47.000000 nomenklatura-3.3.7/nomenklatura.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 07:52:45.000000 nomenklatura-3.3.7/nomenklatura.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-08-03 07:53:47.000000 nomenklatura-3.3.7/nomenklatura.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-03 07:53:47.000000 nomenklatura-3.3.7/nomenklatura.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 07:53:47.405739 nomenklatura-3.3.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-08-03 07:51:04.000000 nomenklatura-3.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:22:38.701370 nomenklatura-3.3.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-08-07 16:22:38.697370 nomenklatura-3.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:22:38.693370 nomenklatura-3.3.8/nomenklatura/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:22:38.693370 nomenklatura-3.3.8/nomenklatura/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/data/regression-v1.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/data/regression-v2.pkl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:22:38.693370 nomenklatura-3.3.8/nomenklatura/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/dataset/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/dataset/coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5292 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/dataset/publisher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/dataset/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/dataset/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:22:38.693370 nomenklatura-3.3.8/nomenklatura/enrich/
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/enrich/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/enrich/aleph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5544 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/enrich/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/enrich/nominatim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/enrich/opencorporates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:22:38.697370 nomenklatura-3.3.8/nomenklatura/enrich/wikidata/
+-rw-r--r--   0 runner    (1001) docker     (123)     9872 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/enrich/wikidata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/enrich/wikidata/lang.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/enrich/wikidata/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/enrich/wikidata/props.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/enrich/wikidata/qualified.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/enrich/wikidata/value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/enrich/yente.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15265 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:22:38.697370 nomenklatura-3.3.8/nomenklatura/index/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/index/entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/index/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/index/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/judgement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:22:38.697370 nomenklatura-3.3.8/nomenklatura/matching/
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/matching/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:22:38.697370 nomenklatura-3.3.8/nomenklatura/matching/heuristic/
+-rw-r--r--   0 runner    (1001) docker     (123)     5942 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/matching/heuristic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/matching/heuristic/logic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/matching/pairs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/matching/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/matching/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:22:38.697370 nomenklatura-3.3.8/nomenklatura/matching/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/matching/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/matching/v1/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/matching/v1/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/matching/v1/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/matching/v1/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/matching/v1/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/matching/v1/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:22:38.697370 nomenklatura-3.3.8/nomenklatura/matching/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/matching/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/matching/v2/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/matching/v2/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/matching/v2/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/matching/v2/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/matching/v2/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/matching/v2/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:22:38.697370 nomenklatura-3.3.8/nomenklatura/publish/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/publish/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/publish/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/publish/edges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/publish/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:22:38.697370 nomenklatura-3.3.8/nomenklatura/resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/resolver/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/resolver/edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/resolver/identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12955 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/resolver/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/senzing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:22:38.697370 nomenklatura-3.3.8/nomenklatura/statement/
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/statement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/statement/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6283 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/statement/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7897 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/statement/statement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:22:38.697370 nomenklatura-3.3.8/nomenklatura/store/
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/store/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/store/level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/store/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/store/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/stream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:22:38.697370 nomenklatura-3.3.8/nomenklatura/tui/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/tui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/tui/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/tui/comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/tui/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/nomenklatura/xref.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:22:38.693370 nomenklatura-3.3.8/nomenklatura.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-08-07 16:22:38.000000 nomenklatura-3.3.8/nomenklatura.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-08-07 16:22:38.000000 nomenklatura-3.3.8/nomenklatura.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 16:22:38.000000 nomenklatura-3.3.8/nomenklatura.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-07 16:22:38.000000 nomenklatura-3.3.8/nomenklatura.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 16:22:38.000000 nomenklatura-3.3.8/nomenklatura.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 16:21:35.000000 nomenklatura-3.3.8/nomenklatura.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-08-07 16:22:38.000000 nomenklatura-3.3.8/nomenklatura.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-07 16:22:38.000000 nomenklatura-3.3.8/nomenklatura.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 16:22:38.701370 nomenklatura-3.3.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-08-07 16:20:05.000000 nomenklatura-3.3.8/setup.py
```

### Comparing `nomenklatura-3.3.7/LICENSE` & `nomenklatura-3.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.7/PKG-INFO` & `nomenklatura-3.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nomenklatura
-Version: 3.3.7
+Version: 3.3.8
 Summary: Make record linkages in followthemoney data.
 Home-page: https://github.com/opensanctions/nomenklatura
 Author: Friedrich Lindenberg
 Author-email: friedrich@pudo.org
 License: MIT
 Keywords: data mapping identity followthemoney linkage record
 Description-Content-Type: text/markdown
```

### Comparing `nomenklatura-3.3.7/README.md` & `nomenklatura-3.3.8/README.md`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.7/nomenklatura/cache.py` & `nomenklatura-3.3.8/nomenklatura/cache.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.7/nomenklatura/cli.py` & `nomenklatura-3.3.8/nomenklatura/cli.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.7/nomenklatura/data/regression-v1.pkl` & `nomenklatura-3.3.8/nomenklatura/data/regression-v1.pkl`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.7/nomenklatura/data/regression-v2.pkl` & `nomenklatura-3.3.8/nomenklatura/data/regression-v2.pkl`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.7/nomenklatura/dataset/catalog.py` & `nomenklatura-3.3.8/nomenklatura/dataset/catalog.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.7/nomenklatura/dataset/coverage.py` & `nomenklatura-3.3.8/nomenklatura/dataset/coverage.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 class DataCoverage(object):
     """Details on the temporal and geographic scope of a dataset."""
 
     # Derived from Aleph
     FREQUENCIES = (
         "unknown",
         "never",
+        "hourly",
         "daily",
         "weekly",
         "monthly",
         "annual",
     )
 
     def __init__(self, data: Dict[str, Any]) -> None:
```

### Comparing `nomenklatura-3.3.7/nomenklatura/dataset/dataset.py` & `nomenklatura-3.3.8/nomenklatura/dataset/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
+import yaml
+import logging
 from functools import cached_property
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Set, Type, TypeVar
-
-import yaml
 from followthemoney.types import registry
 
 from nomenklatura.dataset.coverage import DataCoverage
 from nomenklatura.dataset.publisher import DataPublisher
 from nomenklatura.dataset.resource import DataResource
 from nomenklatura.dataset.util import (
     Named,
@@ -16,14 +16,15 @@
 )
 from nomenklatura.util import PathLike, iso_to_version
 
 if TYPE_CHECKING:
     from nomenklatura.dataset.catalog import DataCatalog
 
 DS = TypeVar("DS", bound="Dataset")
+log = logging.getLogger(__name__)
 
 
 class Dataset(Named):
     """A unit of entities. A dataset is a set of data, sez W3C."""
 
     def __init__(self, catalog: "DataCatalog[DS]", data: Dict[str, Any]) -> None:
         self.catalog = catalog
@@ -54,22 +55,26 @@
         self._children.update(string_list(data.get("datasets", [])))
         self._children.update(string_list(data.get("scopes", [])))
 
     @cached_property
     def children(self: DS) -> Set[DS]:
         children: Set[DS] = set()
         for child_name in self._children:
-            children.add(self.catalog.require(child_name))
-        if self in children:
-            children.remove(self)
+            child = self.catalog.get(child_name)
+            if child is None:
+                log.error("Missing child dataset %r (in %r)", self.name, child_name)
+                continue
+            if child == self:
+                continue
+            children.add(child)
         return children
 
     @cached_property
     def is_collection(self: DS) -> bool:
-        return len(self.children) > 0
+        return len(self._children) > 0
 
     @property
     def datasets(self: DS) -> Set[DS]:
         current: Set[DS] = set([self])
         for child in self.children:
             current.update(child.datasets)
         return current
@@ -99,15 +104,15 @@
             "description": self.description,
             "url": self.url,
             "version": self.version,
             "updated_at": self.updated_at,
             "category": self.category,
             "resources": [r.to_dict() for r in self.resources],
         }
-        children = [c.name for c in self.children if c != self]
+        children = [c for c in self._children if c != self.name]
         if len(children):
             data["children"] = children
         datasets = [c.name for c in self.datasets if c != self]
         if len(datasets):
             data["datasets"] = datasets
         if self.coverage is not None:
             data["coverage"] = self.coverage.to_dict()
```

### Comparing `nomenklatura-3.3.7/nomenklatura/dataset/publisher.py` & `nomenklatura-3.3.8/nomenklatura/dataset/publisher.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.7/nomenklatura/dataset/resource.py` & `nomenklatura-3.3.8/nomenklatura/dataset/resource.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.7/nomenklatura/dataset/util.py` & `nomenklatura-3.3.8/nomenklatura/dataset/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.7/nomenklatura/db.py` & `nomenklatura-3.3.8/nomenklatura/db.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.7/nomenklatura/enrich/__init__.py` & `nomenklatura-3.3.8/nomenklatura/enrich/__init__.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.7/nomenklatura/enrich/aleph.py` & `nomenklatura-3.3.8/nomenklatura/enrich/aleph.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.7/nomenklatura/enrich/common.py` & `nomenklatura-3.3.8/nomenklatura/enrich/common.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.7/nomenklatura/enrich/nominatim.py` & `nomenklatura-3.3.8/nomenklatura/enrich/nominatim.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.7/nomenklatura/enrich/opencorporates.py` & `nomenklatura-3.3.8/nomenklatura/enrich/opencorporates.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.7/nomenklatura/enrich/wikidata/__init__.py` & `nomenklatura-3.3.8/nomenklatura/enrich/wikidata/__init__.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.7/nomenklatura/enrich/wikidata/lang.py` & `nomenklatura-3.3.8/nomenklatura/enrich/wikidata/lang.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.7/nomenklatura/enrich/wikidata/model.py` & `nomenklatura-3.3.8/nomenklatura/enrich/wikidata/model.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.7/nomenklatura/enrich/wikidata/props.py` & `nomenklatura-3.3.8/nomenklatura/enrich/wikidata/props.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.7/nomenklatura/enrich/wikidata/qualified.py` & `nomenklatura-3.3.8/nomenklatura/enrich/wikidata/qualified.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.7/nomenklatura/enrich/wikidata/value.py` & `nomenklatura-3.3.8/nomenklatura/enrich/wikidata/value.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.7/nomenklatura/enrich/yente.py` & `nomenklatura-3.3.8/nomenklatura/enrich/yente.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.7/nomenklatura/entity.py` & `nomenklatura-3.3.8/nomenklatura/entity.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.7/nomenklatura/index/entry.py` & `nomenklatura-3.3.8/nomenklatura/index/entry.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.7/nomenklatura/index/index.py` & `nomenklatura-3.3.8/nomenklatura/index/index.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.7/nomenklatura/index/tokenizer.py` & `nomenklatura-3.3.8/nomenklatura/index/tokenizer.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.7/nomenklatura/judgement.py` & `nomenklatura-3.3.8/nomenklatura/judgement.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.7/nomenklatura/matching/__init__.py` & `nomenklatura-3.3.8/nomenklatura/matching/__init__.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.7/nomenklatura/matching/heuristic/__init__.py` & `nomenklatura-3.3.8/nomenklatura/matching/heuristic/__init__.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.7/nomenklatura/matching/heuristic/logic.py` & `nomenklatura-3.3.8/nomenklatura/matching/heuristic/logic.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.7/nomenklatura/matching/pairs.py` & `nomenklatura-3.3.8/nomenklatura/matching/pairs.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.7/nomenklatura/matching/types.py` & `nomenklatura-3.3.8/nomenklatura/matching/types.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.7/nomenklatura/matching/util.py` & `nomenklatura-3.3.8/nomenklatura/matching/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.7/nomenklatura/matching/v1/dates.py` & `nomenklatura-3.3.8/nomenklatura/matching/v1/dates.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.7/nomenklatura/matching/v1/misc.py` & `nomenklatura-3.3.8/nomenklatura/matching/v1/misc.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.7/nomenklatura/matching/v1/model.py` & `nomenklatura-3.3.8/nomenklatura/matching/v1/model.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.7/nomenklatura/matching/v1/names.py` & `nomenklatura-3.3.8/nomenklatura/matching/v1/names.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.7/nomenklatura/matching/v1/train.py` & `nomenklatura-3.3.8/nomenklatura/matching/v1/train.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.7/nomenklatura/matching/v1/util.py` & `nomenklatura-3.3.8/nomenklatura/matching/v1/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.7/nomenklatura/matching/v2/dates.py` & `nomenklatura-3.3.8/nomenklatura/matching/v2/dates.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.7/nomenklatura/matching/v2/misc.py` & `nomenklatura-3.3.8/nomenklatura/matching/v2/misc.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.7/nomenklatura/matching/v2/model.py` & `nomenklatura-3.3.8/nomenklatura/matching/v2/model.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.7/nomenklatura/matching/v2/names.py` & `nomenklatura-3.3.8/nomenklatura/matching/v2/names.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.7/nomenklatura/matching/v2/train.py` & `nomenklatura-3.3.8/nomenklatura/matching/v2/train.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.7/nomenklatura/matching/v2/util.py` & `nomenklatura-3.3.8/nomenklatura/matching/v2/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.7/nomenklatura/publish/dates.py` & `nomenklatura-3.3.8/nomenklatura/publish/dates.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.7/nomenklatura/publish/edges.py` & `nomenklatura-3.3.8/nomenklatura/publish/edges.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.7/nomenklatura/publish/names.py` & `nomenklatura-3.3.8/nomenklatura/publish/names.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.7/nomenklatura/resolver/edge.py` & `nomenklatura-3.3.8/nomenklatura/resolver/edge.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.7/nomenklatura/resolver/identifier.py` & `nomenklatura-3.3.8/nomenklatura/resolver/identifier.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.7/nomenklatura/resolver/resolver.py` & `nomenklatura-3.3.8/nomenklatura/resolver/resolver.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.7/nomenklatura/senzing.py` & `nomenklatura-3.3.8/nomenklatura/senzing.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.7/nomenklatura/statement/__init__.py` & `nomenklatura-3.3.8/nomenklatura/statement/__init__.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.7/nomenklatura/statement/db.py` & `nomenklatura-3.3.8/nomenklatura/statement/db.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.7/nomenklatura/statement/serialize.py` & `nomenklatura-3.3.8/nomenklatura/statement/serialize.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.7/nomenklatura/statement/statement.py` & `nomenklatura-3.3.8/nomenklatura/statement/statement.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.7/nomenklatura/store/__init__.py` & `nomenklatura-3.3.8/nomenklatura/store/__init__.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.7/nomenklatura/store/base.py` & `nomenklatura-3.3.8/nomenklatura/store/base.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.7/nomenklatura/store/level.py` & `nomenklatura-3.3.8/nomenklatura/store/level.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.7/nomenklatura/store/memory.py` & `nomenklatura-3.3.8/nomenklatura/store/memory.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.7/nomenklatura/store/util.py` & `nomenklatura-3.3.8/nomenklatura/store/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.7/nomenklatura/stream.py` & `nomenklatura-3.3.8/nomenklatura/stream.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,35 +23,38 @@
         super().__init__(model, data, key_prefix=key_prefix, cleaned=cleaned)
         self._caption: Optional[str] = data.get("caption")
         self.datasets: Set[str] = set(data.get("datasets", []))
         self.referents: Set[str] = set(data.get("referents", []))
         self.first_seen: Optional[str] = data.get("first_seen")
         self.last_seen: Optional[str] = data.get("last_seen")
         self.last_change: Optional[str] = data.get("last_change")
+        self.target: Optional[bool] = data.get("target", False)
         self.context = {}
 
     def merge(self: "StreamEntity", other: "StreamEntity") -> "StreamEntity":
         merged = super().merge(other)
         merged._caption = pick_name(_defined(self._caption, other._caption))
         merged.referents.update(other.referents)
         merged.datasets.update(other.datasets)
         self.first_seen = min(_defined(self.first_seen, other.first_seen), default=None)
         self.last_seen = max(_defined(self.last_seen, other.last_seen), default=None)
+        self.target = self.target or other.target
         changed = _defined(self.last_change, other.last_change)
         self.last_change = max(changed, default=None)
         return merged
 
     def to_dict(self) -> Dict[str, Any]:
         data: Dict[str, Any] = {
             "id": self.id,
             "caption": self._caption or self.caption,
             "schema": self.schema.name,
             "properties": self.properties,
             "referents": list(self.referents),
             "datasets": list(self.datasets),
+            "target": self.target,
         }
         if self.first_seen is not None:
             data["first_seen"] = self.first_seen
         if self.last_seen is not None:
             data["last_seen"] = self.last_seen
         if self.last_change is not None:
             data["last_change"] = self.last_change
```

### Comparing `nomenklatura-3.3.7/nomenklatura/tui/app.py` & `nomenklatura-3.3.8/nomenklatura/tui/app.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.7/nomenklatura/tui/comparison.py` & `nomenklatura-3.3.8/nomenklatura/tui/comparison.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.7/nomenklatura/tui/util.py` & `nomenklatura-3.3.8/nomenklatura/tui/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.7/nomenklatura/util.py` & `nomenklatura-3.3.8/nomenklatura/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.7/nomenklatura/xref.py` & `nomenklatura-3.3.8/nomenklatura/xref.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.7/nomenklatura.egg-info/PKG-INFO` & `nomenklatura-3.3.8/nomenklatura.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nomenklatura
-Version: 3.3.7
+Version: 3.3.8
 Summary: Make record linkages in followthemoney data.
 Home-page: https://github.com/opensanctions/nomenklatura
 Author: Friedrich Lindenberg
 Author-email: friedrich@pudo.org
 License: MIT
 Keywords: data mapping identity followthemoney linkage record
 Description-Content-Type: text/markdown
```

### Comparing `nomenklatura-3.3.7/nomenklatura.egg-info/SOURCES.txt` & `nomenklatura-3.3.8/nomenklatura.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.7/setup.py` & `nomenklatura-3.3.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md") as f:
     long_description = f.read()
 
 
 setup(
     name="nomenklatura",
-    version="3.3.7",
+    version="3.3.8",
     description="Make record linkages in followthemoney data.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="data mapping identity followthemoney linkage record",
     author="Friedrich Lindenberg",
     author_email="friedrich@pudo.org",
     url="https://github.com/opensanctions/nomenklatura",
```

