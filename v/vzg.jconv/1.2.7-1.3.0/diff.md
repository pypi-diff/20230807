# Comparing `tmp/vzg.jconv-1.2.7.tar.gz` & `tmp/vzg.jconv-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vzg.jconv-1.2.7.tar", last modified: Wed Aug  2 12:08:41 2023, max compression
+gzip compressed data, was "vzg.jconv-1.3.0.tar", last modified: Mon Aug  7 14:51:18 2023, max compression
```

## Comparing `vzg.jconv-1.2.7.tar` & `vzg.jconv-1.3.0.tar`

### file list

```diff
@@ -1,57 +1,61 @@
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-02 12:08:41.243723 vzg.jconv-1.2.7/
--rw-rw-r--   0 teg       (1000) teg       (1000)    34520 2020-02-07 11:02:19.000000 vzg.jconv-1.2.7/LICENSE.txt
--rw-rw-r--   0 teg       (1000) teg       (1000)      149 2020-02-08 11:53:49.000000 vzg.jconv-1.2.7/MANIFEST.in
--rw-rw-r--   0 teg       (1000) teg       (1000)     1339 2023-08-02 12:08:41.243723 vzg.jconv-1.2.7/PKG-INFO
--rw-rw-r--   0 teg       (1000) teg       (1000)      463 2023-02-16 10:38:51.000000 vzg.jconv-1.2.7/README.md
--rw-rw-r--   0 teg       (1000) teg       (1000)        6 2023-08-02 12:07:14.000000 vzg.jconv-1.2.7/VERSION.txt
--rw-rw-r--   0 teg       (1000) teg       (1000)       38 2023-08-02 12:08:41.243723 vzg.jconv-1.2.7/setup.cfg
--rw-rw-r--   0 teg       (1000) teg       (1000)     1868 2023-08-02 11:54:02.000000 vzg.jconv-1.2.7/setup.py
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-02 12:08:41.243723 vzg.jconv-1.2.7/src/
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-02 12:08:41.243723 vzg.jconv-1.2.7/src/vzg/
--rw-rw-r--   0 teg       (1000) teg       (1000)       80 2020-11-05 11:14:17.000000 vzg.jconv-1.2.7/src/vzg/__init__.py
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-02 12:08:41.243723 vzg.jconv-1.2.7/src/vzg/jconv/
--rw-rw-r--   0 teg       (1000) teg       (1000)      275 2020-02-07 09:30:55.000000 vzg.jconv-1.2.7/src/vzg/jconv/__init__.py
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-02 12:08:41.243723 vzg.jconv-1.2.7/src/vzg/jconv/converter/
--rw-rw-r--   0 teg       (1000) teg       (1000)      378 2020-02-07 13:03:16.000000 vzg.jconv-1.2.7/src/vzg/jconv/converter/__init__.py
--rw-rw-r--   0 teg       (1000) teg       (1000)    15052 2023-08-02 11:31:38.000000 vzg.jconv-1.2.7/src/vzg/jconv/converter/jats.py
--rw-rw-r--   0 teg       (1000) teg       (1000)      450 2020-07-07 11:26:12.000000 vzg.jconv-1.2.7/src/vzg/jconv/errors.py
--rw-rw-r--   0 teg       (1000) teg       (1000)     4136 2023-08-01 08:59:23.000000 vzg.jconv-1.2.7/src/vzg/jconv/gapi.py
--rw-rw-r--   0 teg       (1000) teg       (1000)     1112 2023-07-31 15:01:19.000000 vzg.jconv-1.2.7/src/vzg/jconv/interfaces.py
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-02 12:08:41.243723 vzg.jconv-1.2.7/src/vzg/jconv/journal/
--rw-rw-r--   0 teg       (1000) teg       (1000)     6603 2023-07-31 15:28:18.000000 vzg.jconv-1.2.7/src/vzg/jconv/journal/__init__.py
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-02 12:08:41.243723 vzg.jconv-1.2.7/src/vzg/jconv/langcode/
--rw-rw-r--   0 teg       (1000) teg       (1000)     1156 2020-02-07 12:48:06.000000 vzg.jconv-1.2.7/src/vzg/jconv/langcode/__init__.py
--rw-rw-r--   0 teg       (1000) teg       (1000)    11245 2020-02-07 12:11:08.000000 vzg.jconv-1.2.7/src/vzg/jconv/langcode/language-codes.json
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-02 12:08:41.243723 vzg.jconv-1.2.7/src/vzg/jconv/person/
--rw-rw-r--   0 teg       (1000) teg       (1000)     5949 2023-07-21 15:51:03.000000 vzg.jconv-1.2.7/src/vzg/jconv/person/__init__.py
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-02 12:08:41.243723 vzg.jconv-1.2.7/src/vzg/jconv/publisher/
--rw-rw-r--   0 teg       (1000) teg       (1000)     1314 2023-07-28 13:58:32.000000 vzg.jconv-1.2.7/src/vzg/jconv/publisher/__init__.py
--rw-rw-r--   0 teg       (1000) teg       (1000)      263 2020-07-02 08:39:22.000000 vzg.jconv-1.2.7/src/vzg/jconv/publisher/publisher-codes.json
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-02 12:08:41.243723 vzg.jconv-1.2.7/src/vzg/jconv/schema/
--rw-rw-r--   0 teg       (1000) teg       (1000)    17321 2022-01-14 16:28:18.000000 vzg.jconv-1.2.7/src/vzg/jconv/schema/article_schema.json
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-02 12:08:41.243723 vzg.jconv-1.2.7/src/vzg/jconv/test/
--rw-rw-r--   0 teg       (1000) teg       (1000)      960 2020-02-11 12:04:12.000000 vzg.jconv-1.2.7/src/vzg/jconv/test/__init__.py
--rw-rw-r--   0 teg       (1000) teg       (1000)     1218 2023-07-21 15:51:03.000000 vzg.jconv-1.2.7/src/vzg/jconv/test/conftest.py
--rw-rw-r--   0 teg       (1000) teg       (1000)     6068 2023-07-21 15:51:03.000000 vzg.jconv-1.2.7/src/vzg/jconv/test/test_jats_article.py
--rw-rw-r--   0 teg       (1000) teg       (1000)     3627 2023-08-01 07:25:20.000000 vzg.jconv-1.2.7/src/vzg/jconv/test/test_jats_converter.py
--rw-rw-r--   0 teg       (1000) teg       (1000)     7302 2023-08-01 07:22:39.000000 vzg.jconv-1.2.7/src/vzg/jconv/test/test_jats_degruyter.py
--rw-rw-r--   0 teg       (1000) teg       (1000)     2406 2023-08-01 09:54:23.000000 vzg.jconv-1.2.7/src/vzg/jconv/test/test_jatsdate.py
--rw-rw-r--   0 teg       (1000) teg       (1000)     4008 2023-07-31 15:20:44.000000 vzg.jconv-1.2.7/src/vzg/jconv/test/test_journal.py
--rw-rw-r--   0 teg       (1000) teg       (1000)     1038 2020-02-11 12:04:12.000000 vzg.jconv-1.2.7/src/vzg/jconv/test/test_langcode.py
--rw-rw-r--   0 teg       (1000) teg       (1000)     2803 2023-02-16 12:17:30.000000 vzg.jconv-1.2.7/src/vzg/jconv/test/test_person.py
--rw-rw-r--   0 teg       (1000) teg       (1000)     1029 2020-07-02 09:05:29.000000 vzg.jconv-1.2.7/src/vzg/jconv/test/test_publisher.py
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-02 12:08:41.243723 vzg.jconv-1.2.7/src/vzg/jconv/tools/
--rw-rw-r--   0 teg       (1000) teg       (1000)      378 2020-02-12 10:22:25.000000 vzg.jconv-1.2.7/src/vzg/jconv/tools/__init__.py
--rw-rw-r--   0 teg       (1000) teg       (1000)     6790 2023-07-21 15:51:03.000000 vzg.jconv-1.2.7/src/vzg/jconv/tools/simple_conv.py
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-02 12:08:41.243723 vzg.jconv-1.2.7/src/vzg/jconv/utils/
--rw-rw-r--   0 teg       (1000) teg       (1000)     2932 2023-07-24 11:56:32.000000 vzg.jconv-1.2.7/src/vzg/jconv/utils/__init__.py
--rw-rw-r--   0 teg       (1000) teg       (1000)     1989 2023-08-01 09:44:49.000000 vzg.jconv-1.2.7/src/vzg/jconv/utils/date.py
-drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-02 12:08:41.243723 vzg.jconv-1.2.7/src/vzg.jconv.egg-info/
--rw-rw-r--   0 teg       (1000) teg       (1000)     1339 2023-08-02 12:08:41.000000 vzg.jconv-1.2.7/src/vzg.jconv.egg-info/PKG-INFO
--rw-rw-r--   0 teg       (1000) teg       (1000)     1316 2023-08-02 12:08:41.000000 vzg.jconv-1.2.7/src/vzg.jconv.egg-info/SOURCES.txt
--rw-rw-r--   0 teg       (1000) teg       (1000)        1 2023-08-02 12:08:41.000000 vzg.jconv-1.2.7/src/vzg.jconv.egg-info/dependency_links.txt
--rw-rw-r--   0 teg       (1000) teg       (1000)       65 2023-08-02 12:08:41.000000 vzg.jconv-1.2.7/src/vzg.jconv.egg-info/entry_points.txt
--rw-rw-r--   0 teg       (1000) teg       (1000)        4 2023-08-02 12:08:41.000000 vzg.jconv-1.2.7/src/vzg.jconv.egg-info/namespace_packages.txt
--rw-rw-r--   0 teg       (1000) teg       (1000)        1 2020-02-07 10:31:14.000000 vzg.jconv-1.2.7/src/vzg.jconv.egg-info/not-zip-safe
--rw-rw-r--   0 teg       (1000) teg       (1000)       48 2023-08-02 12:08:41.000000 vzg.jconv-1.2.7/src/vzg.jconv.egg-info/requires.txt
--rw-rw-r--   0 teg       (1000) teg       (1000)        4 2023-08-02 12:08:41.000000 vzg.jconv-1.2.7/src/vzg.jconv.egg-info/top_level.txt
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-07 14:51:18.894899 vzg.jconv-1.3.0/
+-rw-rw-r--   0 teg       (1000) teg       (1000)    34520 2020-02-07 11:02:19.000000 vzg.jconv-1.3.0/LICENSE.txt
+-rw-rw-r--   0 teg       (1000) teg       (1000)      149 2020-02-08 11:53:49.000000 vzg.jconv-1.3.0/MANIFEST.in
+-rw-rw-r--   0 teg       (1000) teg       (1000)     1339 2023-08-07 14:51:18.894899 vzg.jconv-1.3.0/PKG-INFO
+-rw-rw-r--   0 teg       (1000) teg       (1000)      463 2023-02-16 10:38:51.000000 vzg.jconv-1.3.0/README.md
+-rw-rw-r--   0 teg       (1000) teg       (1000)        6 2023-08-07 14:50:50.000000 vzg.jconv-1.3.0/VERSION.txt
+-rw-rw-r--   0 teg       (1000) teg       (1000)       38 2023-08-07 14:51:18.894899 vzg.jconv-1.3.0/setup.cfg
+-rw-rw-r--   0 teg       (1000) teg       (1000)     1868 2023-08-02 11:54:02.000000 vzg.jconv-1.3.0/setup.py
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-07 14:51:18.890899 vzg.jconv-1.3.0/src/
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-07 14:51:18.894899 vzg.jconv-1.3.0/src/vzg/
+-rw-rw-r--   0 teg       (1000) teg       (1000)       80 2020-11-05 11:14:17.000000 vzg.jconv-1.3.0/src/vzg/__init__.py
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-07 14:51:18.894899 vzg.jconv-1.3.0/src/vzg/jconv/
+-rw-rw-r--   0 teg       (1000) teg       (1000)      275 2020-02-07 09:30:55.000000 vzg.jconv-1.3.0/src/vzg/jconv/__init__.py
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-07 14:51:18.894899 vzg.jconv-1.3.0/src/vzg/jconv/archives/
+-rw-rw-r--   0 teg       (1000) teg       (1000)      361 2023-08-07 14:48:59.000000 vzg.jconv-1.3.0/src/vzg/jconv/archives/__init__.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     2323 2023-08-07 14:48:59.000000 vzg.jconv-1.3.0/src/vzg/jconv/archives/springer.py
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-07 14:51:18.894899 vzg.jconv-1.3.0/src/vzg/jconv/converter/
+-rw-rw-r--   0 teg       (1000) teg       (1000)      378 2020-02-07 13:03:16.000000 vzg.jconv-1.3.0/src/vzg/jconv/converter/__init__.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)    15363 2023-08-07 14:48:59.000000 vzg.jconv-1.3.0/src/vzg/jconv/converter/jats.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)      450 2020-07-07 11:26:12.000000 vzg.jconv-1.3.0/src/vzg/jconv/errors.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     4136 2023-08-01 08:59:23.000000 vzg.jconv-1.3.0/src/vzg/jconv/gapi.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     1285 2023-08-07 14:48:59.000000 vzg.jconv-1.3.0/src/vzg/jconv/interfaces.py
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-07 14:51:18.894899 vzg.jconv-1.3.0/src/vzg/jconv/journal/
+-rw-rw-r--   0 teg       (1000) teg       (1000)     6629 2023-08-07 14:48:59.000000 vzg.jconv-1.3.0/src/vzg/jconv/journal/__init__.py
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-07 14:51:18.894899 vzg.jconv-1.3.0/src/vzg/jconv/langcode/
+-rw-rw-r--   0 teg       (1000) teg       (1000)     1156 2020-02-07 12:48:06.000000 vzg.jconv-1.3.0/src/vzg/jconv/langcode/__init__.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)    11245 2020-02-07 12:11:08.000000 vzg.jconv-1.3.0/src/vzg/jconv/langcode/language-codes.json
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-07 14:51:18.894899 vzg.jconv-1.3.0/src/vzg/jconv/person/
+-rw-rw-r--   0 teg       (1000) teg       (1000)     5949 2023-07-21 15:51:03.000000 vzg.jconv-1.3.0/src/vzg/jconv/person/__init__.py
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-07 14:51:18.894899 vzg.jconv-1.3.0/src/vzg/jconv/publisher/
+-rw-rw-r--   0 teg       (1000) teg       (1000)     1314 2023-07-28 13:58:32.000000 vzg.jconv-1.3.0/src/vzg/jconv/publisher/__init__.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)      263 2020-07-02 08:39:22.000000 vzg.jconv-1.3.0/src/vzg/jconv/publisher/publisher-codes.json
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-07 14:51:18.894899 vzg.jconv-1.3.0/src/vzg/jconv/schema/
+-rw-rw-r--   0 teg       (1000) teg       (1000)    17321 2022-01-14 16:28:18.000000 vzg.jconv-1.3.0/src/vzg/jconv/schema/article_schema.json
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-07 14:51:18.894899 vzg.jconv-1.3.0/src/vzg/jconv/test/
+-rw-rw-r--   0 teg       (1000) teg       (1000)      960 2020-02-11 12:04:12.000000 vzg.jconv-1.3.0/src/vzg/jconv/test/__init__.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     1218 2023-07-21 15:51:03.000000 vzg.jconv-1.3.0/src/vzg/jconv/test/conftest.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     1819 2023-08-07 14:48:59.000000 vzg.jconv-1.3.0/src/vzg/jconv/test/test_archives.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     6068 2023-07-21 15:51:03.000000 vzg.jconv-1.3.0/src/vzg/jconv/test/test_jats_article.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     3627 2023-08-01 07:25:20.000000 vzg.jconv-1.3.0/src/vzg/jconv/test/test_jats_converter.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     7302 2023-08-01 07:22:39.000000 vzg.jconv-1.3.0/src/vzg/jconv/test/test_jats_degruyter.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     2406 2023-08-01 09:54:23.000000 vzg.jconv-1.3.0/src/vzg/jconv/test/test_jatsdate.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     4008 2023-07-31 15:20:44.000000 vzg.jconv-1.3.0/src/vzg/jconv/test/test_journal.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     1038 2020-02-11 12:04:12.000000 vzg.jconv-1.3.0/src/vzg/jconv/test/test_langcode.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     2803 2023-02-16 12:17:30.000000 vzg.jconv-1.3.0/src/vzg/jconv/test/test_person.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     1029 2020-07-02 09:05:29.000000 vzg.jconv-1.3.0/src/vzg/jconv/test/test_publisher.py
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-07 14:51:18.894899 vzg.jconv-1.3.0/src/vzg/jconv/tools/
+-rw-rw-r--   0 teg       (1000) teg       (1000)      378 2020-02-12 10:22:25.000000 vzg.jconv-1.3.0/src/vzg/jconv/tools/__init__.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     6200 2023-08-07 14:48:59.000000 vzg.jconv-1.3.0/src/vzg/jconv/tools/simple_conv.py
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-07 14:51:18.894899 vzg.jconv-1.3.0/src/vzg/jconv/utils/
+-rw-rw-r--   0 teg       (1000) teg       (1000)     2932 2023-07-24 11:56:32.000000 vzg.jconv-1.3.0/src/vzg/jconv/utils/__init__.py
+-rw-rw-r--   0 teg       (1000) teg       (1000)     1989 2023-08-01 09:44:49.000000 vzg.jconv-1.3.0/src/vzg/jconv/utils/date.py
+drwxrwxr-x   0 teg       (1000) teg       (1000)        0 2023-08-07 14:51:18.894899 vzg.jconv-1.3.0/src/vzg.jconv.egg-info/
+-rw-rw-r--   0 teg       (1000) teg       (1000)     1339 2023-08-07 14:51:18.000000 vzg.jconv-1.3.0/src/vzg.jconv.egg-info/PKG-INFO
+-rw-rw-r--   0 teg       (1000) teg       (1000)     1422 2023-08-07 14:51:18.000000 vzg.jconv-1.3.0/src/vzg.jconv.egg-info/SOURCES.txt
+-rw-rw-r--   0 teg       (1000) teg       (1000)        1 2023-08-07 14:51:18.000000 vzg.jconv-1.3.0/src/vzg.jconv.egg-info/dependency_links.txt
+-rw-rw-r--   0 teg       (1000) teg       (1000)       65 2023-08-07 14:51:18.000000 vzg.jconv-1.3.0/src/vzg.jconv.egg-info/entry_points.txt
+-rw-rw-r--   0 teg       (1000) teg       (1000)        4 2023-08-07 14:51:18.000000 vzg.jconv-1.3.0/src/vzg.jconv.egg-info/namespace_packages.txt
+-rw-rw-r--   0 teg       (1000) teg       (1000)        1 2020-02-07 10:31:14.000000 vzg.jconv-1.3.0/src/vzg.jconv.egg-info/not-zip-safe
+-rw-rw-r--   0 teg       (1000) teg       (1000)       48 2023-08-07 14:51:18.000000 vzg.jconv-1.3.0/src/vzg.jconv.egg-info/requires.txt
+-rw-rw-r--   0 teg       (1000) teg       (1000)        4 2023-08-07 14:51:18.000000 vzg.jconv-1.3.0/src/vzg.jconv.egg-info/top_level.txt
```

### Comparing `vzg.jconv-1.2.7/LICENSE.txt` & `vzg.jconv-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.2.7/PKG-INFO` & `vzg.jconv-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vzg.jconv
-Version: 1.2.7
+Version: 1.3.0
 Summary: Python library to create JSON Data
 Home-page: https://github.com/gbv/vzg.jconv
 Author: Marc-J. Tegethoff
 Author-email: tegethoff@gbv.de
 License: GNU Affero General Public License v3
 Project-URL: PyPI, https://pypi.python.org/pypi/vzg.jconv
 Project-URL: Source, https://github.com/gbv/vzg.jconv
```

### Comparing `vzg.jconv-1.2.7/setup.py` & `vzg.jconv-1.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.2.7/src/vzg/jconv/converter/jats.py` & `vzg.jconv-1.3.0/src/vzg/jconv/converter/jats.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 # Copyright (c) 2020-2023 Verbundzentrale des GBV.
 # All Rights Reserved.
 #
 ##############################################################################
 """
 
 # Imports
+from pathlib import Path
 from zope.interface import implementer
 from vzg.jconv.interfaces import IArticle
 from vzg.jconv.interfaces import IConverter
 from vzg.jconv.gapi import NAMESPACES
 from vzg.jconv.gapi import JSON_SCHEMA
 from vzg.jconv.gapi import JATS_SPRINGER_PUBTYPE
 from vzg.jconv.gapi import JATS_XPATHS
@@ -141,15 +142,16 @@
         nodes = self.dom.xpath(expression, namespaces=NAMESPACES)
 
         if len(nodes) > 0:
             expression = JATS_XPATHS["pub-date-format"].format(
                 pubtype=self.pubtype.name
             )
         else:
-            expression = JATS_XPATHS["pub-date"].format(pubtype=self.pubtype.value)
+            expression = JATS_XPATHS["pub-date"].format(
+                pubtype=self.pubtype.value)
 
         node = self.xpath(expression)
 
         if len(node) == 0:
             return None
 
         dateOfProduction = JatsDate(node[0])
@@ -427,14 +429,18 @@
     iso639 : vzg.jconv.langcode.ISO_639
 
     publisher : string
         Set or override the publisher entry
 
     validate : bool
         Validate each IArticle
+
+    name : str
+        optionnal filename
+
     Returns
     -------
     None
 
     Raises
     ------
     OSError
@@ -447,17 +453,23 @@
 
     >>> conv = JatsConverter(xpath)
     >>> conv.run()
     >>> conv.articles
     []
     """
 
-    def __init__(self, jatspath, iso639=None, publisher=None, validate=False):
+    def __init__(self,
+                 jatspath: Path,
+                 iso639: ISO_639 = None,
+                 publisher: str = None,
+                 validate: bool = False,
+                 name: str = ""):
         self.jatspath = jatspath
         self.articles = []
+        self.name = name
         self.publisher = publisher
         self.pubtype_source = PUBTYPE_SOURCES.basic
 
         if not self.jatspath.is_file():
             raise OSError
 
         with open(self.jatspath, "rb") as fh:
@@ -492,21 +504,23 @@
             nodes = self.dom.xpath(expression, namespaces=NAMESPACES)
             if len(nodes) > 0:
                 self.pubtype_source = PUBTYPE_SOURCES.degruyter
 
         for entry in JATS_SPRINGER_PUBTYPE:
             if self.pubtype_source == PUBTYPE_SOURCES.springer:
                 logger.debug("new pub")
-                expression = JATS_XPATHS["pub-date-format"].format(pubtype=entry.name)
+                expression = JATS_XPATHS["pub-date-format"].format(
+                    pubtype=entry.name)
             elif self.pubtype_source == PUBTYPE_SOURCES.degruyter:
                 expression = JATS_XPATHS["pub-date-pubtype-val"].format(
                     pubtype=entry.value
                 )
             else:
-                expression = JATS_XPATHS["pub-date"].format(pubtype=entry.value)
+                expression = JATS_XPATHS["pub-date"].format(
+                    pubtype=entry.value)
 
             nodes = self.dom.xpath(expression, namespaces=NAMESPACES)
 
             if len(nodes) > 0:
                 pubtypes.append(entry)
 
         logger.debug(pubtypes)
@@ -523,15 +537,16 @@
         for pubtype in self.pubtypes:
             article = JatsArticle(
                 self.dom, pubtype, self.iso639, self.publisher, self.pubtype_source
             )
 
             if self.validate:
                 try:
-                    jsonschema.validate(instance=article.jdict, schema=JSON_SCHEMA)
+                    jsonschema.validate(
+                        instance=article.jdict, schema=JSON_SCHEMA)
                     self.articles.append(article)
                 except jsonschema.ValidationError as Exc:
                     logger.info(Exc, exc_info=False)
                     self.validation_failed = True
 
                 continue
```

### Comparing `vzg.jconv-1.2.7/src/vzg/jconv/gapi.py` & `vzg.jconv-1.3.0/src/vzg/jconv/gapi.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.2.7/src/vzg/jconv/interfaces.py` & `vzg.jconv-1.3.0/src/vzg/jconv/interfaces.py`

 * *Files 23% similar despite different names*

```diff
@@ -21,18 +21,25 @@
     journal = Attribute("Journal")
     json = Attribute("Article as JSON object")
     lang_code = Attribute("Language Code")
     primary_id = Attribute("Primäre ID des Datensatzes in der Datenquelle")
     title = Attribute("Article Title")
 
 
+class IArchive(Interface):
+    """Exchange Container"""
+
+    converters = Attribute("List of IConverter objects")
+
+
 class IConverter(Interface):
     """Converter"""
 
     articles = Attribute("List of IArticle objects")
+    name = Attribute("Optional name of the source file")
 
     def run(self):
         """Start the conversion"""
 
 
 class IJournal(Interface):
     """Journal"""
```

### Comparing `vzg.jconv-1.2.7/src/vzg/jconv/journal/__init__.py` & `vzg.jconv-1.3.0/src/vzg/jconv/journal/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 # Imports
 import logging
 from zope.interface import implementer
 from vzg.jconv.interfaces import IJournal
 from vzg.jconv.gapi import NAMESPACES
 from vzg.jconv.gapi import JATS_SPRINGER_PUBTYPE
 from vzg.jconv.gapi import PUBTYPE_SOURCES
-from vzg.jconv.gapi import JATS_SPRINGER_PUBTYPE, PUBTYPE_SOURCES
 from vzg.jconv.gapi import JATS_SPRINGER_JOURNALTYPE
 from vzg.jconv.gapi import JATS_XPATHS
 from vzg.jconv.utils.date import JatsDate
 from vzg.jconv.utils import get_pubtype_suffix
 from lxml import etree
 
 __author__ = """Marc-J. Tegethoff <tegethoff@gbv.de>"""
@@ -68,21 +67,23 @@
     @property
     def date(self) -> JatsDate:
         """Look for the earliest date"""
         date_node = None
 
         for pubtype in JATS_SPRINGER_PUBTYPE:
             if self.article.pubtype_source == PUBTYPE_SOURCES.springer:
-                expression = JATS_XPATHS["pub-date-format"].format(pubtype=pubtype.name)
+                expression = JATS_XPATHS["pub-date-format"].format(
+                    pubtype=pubtype.name)
             elif self.article.pubtype_source == PUBTYPE_SOURCES.degruyter:
                 expression = JATS_XPATHS["pub-date-pubtype-val"].format(
                     pubtype=pubtype.value
                 )
             else:
-                expression = JATS_XPATHS["pub-date"].format(pubtype=pubtype.value)
+                expression = JATS_XPATHS["pub-date"].format(
+                    pubtype=pubtype.value)
 
             node = self.xpath(expression)
 
             if len(node) > 0:
                 dnode = JatsDate(node[0])
 
                 if isinstance(date_node, JatsDate):
@@ -96,15 +97,16 @@
     @property
     def jids(self) -> dict:
         jids = {
             "emerald": [JATS_XPATHS["journal-id"].format(journaltype="publisher")],
             "basic": [JATS_XPATHS["journal-id"].format(journaltype="publisher-id")],
             "doi": [JATS_XPATHS["journal-id"].format(journaltype="doi")],
             self.article.pubtype.value: [
-                JATS_XPATHS["journal-issn"].format(pubtype=self.article.pubtype.value),
+                JATS_XPATHS["journal-issn"].format(
+                    pubtype=self.article.pubtype.value),
                 JATS_XPATHS["journal-issn-pformat"].format(
                     pubtype=self.article.pubtype.name
                 ),
             ],
         }
 
         if self.article.pubtype_source == PUBTYPE_SOURCES.degruyter:
@@ -145,15 +147,16 @@
 
                 jid = {"type": jtype, "id": node[0]}
 
                 if jtype == "basic":
                     jid["type"] = "springer"
                     if self.article.pubtype_source == PUBTYPE_SOURCES.degruyter:
                         jid["type"] = "degruyter"
-                        jid["id"] += get_pubtype_suffix(self.article.pubtype.value)
+                        jid["id"] += get_pubtype_suffix(
+                            self.article.pubtype.value)
 
                 if jid["type"] in JATS_SPRINGER_JOURNALTYPE.__members__:
                     jid["type"] = JATS_SPRINGER_JOURNALTYPE[jid["type"]].value
 
                 _ids.append(jid)
 
                 done.append(jtype)
```

### Comparing `vzg.jconv-1.2.7/src/vzg/jconv/langcode/__init__.py` & `vzg.jconv-1.3.0/src/vzg/jconv/langcode/__init__.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.2.7/src/vzg/jconv/langcode/language-codes.json` & `vzg.jconv-1.3.0/src/vzg/jconv/langcode/language-codes.json`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.2.7/src/vzg/jconv/person/__init__.py` & `vzg.jconv-1.3.0/src/vzg/jconv/person/__init__.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.2.7/src/vzg/jconv/publisher/__init__.py` & `vzg.jconv-1.3.0/src/vzg/jconv/publisher/__init__.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.2.7/src/vzg/jconv/schema/article_schema.json` & `vzg.jconv-1.3.0/src/vzg/jconv/schema/article_schema.json`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.2.7/src/vzg/jconv/test/__init__.py` & `vzg.jconv-1.3.0/src/vzg/jconv/test/__init__.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.2.7/src/vzg/jconv/test/conftest.py` & `vzg.jconv-1.3.0/src/vzg/jconv/test/conftest.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.2.7/src/vzg/jconv/test/test_jats_article.py` & `vzg.jconv-1.3.0/src/vzg/jconv/test/test_jats_article.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.2.7/src/vzg/jconv/test/test_jats_converter.py` & `vzg.jconv-1.3.0/src/vzg/jconv/test/test_jats_converter.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.2.7/src/vzg/jconv/test/test_jats_degruyter.py` & `vzg.jconv-1.3.0/src/vzg/jconv/test/test_jats_degruyter.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.2.7/src/vzg/jconv/test/test_jatsdate.py` & `vzg.jconv-1.3.0/src/vzg/jconv/test/test_jatsdate.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.2.7/src/vzg/jconv/test/test_journal.py` & `vzg.jconv-1.3.0/src/vzg/jconv/test/test_journal.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.2.7/src/vzg/jconv/test/test_langcode.py` & `vzg.jconv-1.3.0/src/vzg/jconv/test/test_langcode.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.2.7/src/vzg/jconv/test/test_person.py` & `vzg.jconv-1.3.0/src/vzg/jconv/test/test_person.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.2.7/src/vzg/jconv/test/test_publisher.py` & `vzg.jconv-1.3.0/src/vzg/jconv/test/test_publisher.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.2.7/src/vzg/jconv/tools/simple_conv.py` & `vzg.jconv-1.3.0/src/vzg/jconv/tools/simple_conv.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 # -*- coding: UTF-8 -*-
 """Beschreibung
 
 ##############################################################################
 #
-# Copyright (c) 2020 Verbundzentrale des GBV.
+# Copyright (c) 2020-2023 Verbundzentrale des GBV.
 # All Rights Reserved.
 #
 ##############################################################################
 """
 
 # Imports
 import logging
 from pathlib import Path
 import zipfile
 import tempfile
+from vzg.jconv.archives.springer import ArchiveSpringer
 from vzg.jconv.converter.jats import JatsConverter
 
 __author__ = """Marc-J. Tegethoff <marc.tegethoff@gbv.de>"""
 __docformat__ = "plaintext"
 
 
 def fromarchive(options):
@@ -83,58 +84,44 @@
     dst = opath / jpath.name
     deliverysignature = uuid.uuid4()
 
     if not opath.exists():
         opath.mkdir(0o755, parents=True)
 
     with zipfile.ZipFile(dst, "w") as jsonarchive:
-        with zipfile.ZipFile(jpath) as xmlarchive:
-            num_xml = 0
-            for name in xmlarchive.namelist():
-                num_xml += 1
-
-            num_xml = float(num_xml)
-
-            for i, zipinfo in enumerate(xmlarchive.infolist()):
-                with tempfile.NamedTemporaryFile("w+b") as tmpfh:
-                    tmpfh.write(xmlarchive.read(zipinfo))
-                    tmpfh.flush()
-
-                    jatspath = Path(tmpfh.name)
-
-                    xpercent = i / num_xml * 100
-                    msg = f"{zipinfo.filename} ({xpercent:.2f}%)"
-                    logger.info(msg)
-
-                    if options.publisher == "":
-                        jconv = JatsConverter(jatspath, validate=options.validate)
-                    else:
-                        jconv = JatsConverter(
-                            jatspath,
-                            publisher=options.publisher,
-                            validate=options.validate,
-                        )
-                    jconv.run()
-
-                    anum = len(jconv.articles)
-                    msg = f"\t{anum} article(s)"
-                    logger.info(msg)
-
-                    if options.dry_run is False:
-                        for j, article in enumerate(jconv.articles):
-                            aname = f"{deliverysignature}-{i}-{j}.json"
-                            logger.info(aname)
-                            jsonarchive.writestr(
-                                aname, article.json, compress_type=zipfile.ZIP_DEFLATED
-                            )
-
-                    if options.stop and jconv.validation_failed:
-                        msg = "Validation problem"
-                        logger.info(msg)
-                        break
+        converter_kwargs = {"validate": options.validate}
+        if options.publisher != "":
+            converter_kwargs["publisher"] = options.publisher
+
+        xmlarchive = ArchiveSpringer(jpath, converter_kwargs=converter_kwargs)
+        num_xml = float(xmlarchive.num_files)
+
+        for i, jconv in enumerate(xmlarchive.converters):
+            xpercent = i / num_xml * 100
+            msg = f"{jconv.name} ({xpercent:.2f}%)"
+            logger.info(msg)
+
+            jconv.run()
+
+            anum = len(jconv.articles)
+            msg = f"\t{anum} article(s)"
+            logger.info(msg)
+
+            if options.dry_run is False:
+                for j, article in enumerate(jconv.articles):
+                    aname = f"{deliverysignature}-{i}-{j}.json"
+                    logger.info(aname)
+                    jsonarchive.writestr(
+                        aname, article.json, compress_type=zipfile.ZIP_DEFLATED
+                    )
+
+            if options.stop and jconv.validation_failed:
+                msg = "Validation problem"
+                logger.info(msg)
+                break
 
 
 def run():
     """Start the application"""
     from argparse import ArgumentParser
 
     description = "Simple conversion tool."
```

### Comparing `vzg.jconv-1.2.7/src/vzg/jconv/utils/__init__.py` & `vzg.jconv-1.3.0/src/vzg/jconv/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.2.7/src/vzg/jconv/utils/date.py` & `vzg.jconv-1.3.0/src/vzg/jconv/utils/date.py`

 * *Files identical despite different names*

### Comparing `vzg.jconv-1.2.7/src/vzg.jconv.egg-info/PKG-INFO` & `vzg.jconv-1.3.0/src/vzg.jconv.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vzg.jconv
-Version: 1.2.7
+Version: 1.3.0
 Summary: Python library to create JSON Data
 Home-page: https://github.com/gbv/vzg.jconv
 Author: Marc-J. Tegethoff
 Author-email: tegethoff@gbv.de
 License: GNU Affero General Public License v3
 Project-URL: PyPI, https://pypi.python.org/pypi/vzg.jconv
 Project-URL: Source, https://github.com/gbv/vzg.jconv
```

### Comparing `vzg.jconv-1.2.7/src/vzg.jconv.egg-info/SOURCES.txt` & `vzg.jconv-1.3.0/src/vzg.jconv.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -13,25 +13,28 @@
 src/vzg.jconv.egg-info/not-zip-safe
 src/vzg.jconv.egg-info/requires.txt
 src/vzg.jconv.egg-info/top_level.txt
 src/vzg/jconv/__init__.py
 src/vzg/jconv/errors.py
 src/vzg/jconv/gapi.py
 src/vzg/jconv/interfaces.py
+src/vzg/jconv/archives/__init__.py
+src/vzg/jconv/archives/springer.py
 src/vzg/jconv/converter/__init__.py
 src/vzg/jconv/converter/jats.py
 src/vzg/jconv/journal/__init__.py
 src/vzg/jconv/langcode/__init__.py
 src/vzg/jconv/langcode/language-codes.json
 src/vzg/jconv/person/__init__.py
 src/vzg/jconv/publisher/__init__.py
 src/vzg/jconv/publisher/publisher-codes.json
 src/vzg/jconv/schema/article_schema.json
 src/vzg/jconv/test/__init__.py
 src/vzg/jconv/test/conftest.py
+src/vzg/jconv/test/test_archives.py
 src/vzg/jconv/test/test_jats_article.py
 src/vzg/jconv/test/test_jats_converter.py
 src/vzg/jconv/test/test_jats_degruyter.py
 src/vzg/jconv/test/test_jatsdate.py
 src/vzg/jconv/test/test_journal.py
 src/vzg/jconv/test/test_langcode.py
 src/vzg/jconv/test/test_person.py
```

