# Comparing `tmp/Joule-0.9.8.tar.gz` & `tmp/Joule-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Joule-0.9.8.tar", last modified: Mon Nov 18 21:08:01 2019, max compression
+gzip compressed data, was "dist/Joule-0.9.9.tar", last modified: Thu Nov 21 20:50:45 2019, max compression
```

## Comparing `Joule-0.9.8.tar` & `Joule-0.9.9.tar`

### file list

```diff
@@ -1,210 +1,210 @@
-drwxr-xr-x   0 jdonnal    (501) staff       (20)        0 2019-11-18 21:08:01.000000 Joule-0.9.8/
-drwxr-xr-x   0 jdonnal    (501) staff       (20)        0 2019-11-18 21:08:01.000000 Joule-0.9.8/Joule.egg-info/
--rw-r--r--   0 jdonnal    (501) staff       (20)     3738 2019-11-18 21:08:01.000000 Joule-0.9.8/Joule.egg-info/PKG-INFO
--rw-r--r--   0 jdonnal    (501) staff       (20)     5576 2019-11-18 21:08:01.000000 Joule-0.9.8/Joule.egg-info/SOURCES.txt
--rw-r--r--   0 jdonnal    (501) staff       (20)        1 2019-11-18 21:08:01.000000 Joule-0.9.8/Joule.egg-info/dependency_links.txt
--rw-r--r--   0 jdonnal    (501) staff       (20)      377 2019-11-18 21:08:01.000000 Joule-0.9.8/Joule.egg-info/entry_points.txt
--rw-r--r--   0 jdonnal    (501) staff       (20)        1 2019-11-18 21:08:01.000000 Joule-0.9.8/Joule.egg-info/namespace_packages.txt
--rw-r--r--   0 jdonnal    (501) staff       (20)        1 2018-10-06 23:40:12.000000 Joule-0.9.8/Joule.egg-info/not-zip-safe
--rw-r--r--   0 jdonnal    (501) staff       (20)      184 2019-11-18 21:08:01.000000 Joule-0.9.8/Joule.egg-info/requires.txt
--rw-r--r--   0 jdonnal    (501) staff       (20)       12 2019-11-18 21:08:01.000000 Joule-0.9.8/Joule.egg-info/top_level.txt
--rw-r--r--   0 jdonnal    (501) staff       (20)      248 2019-07-26 18:42:54.000000 Joule-0.9.8/MANIFEST.in
--rw-r--r--   0 jdonnal    (501) staff       (20)     3738 2019-11-18 21:08:01.000000 Joule-0.9.8/PKG-INFO
--rw-r--r--   0 jdonnal    (501) staff       (20)     2664 2019-07-03 18:08:20.000000 Joule-0.9.8/README.rst
-drwxr-xr-x   0 jdonnal    (501) staff       (20)        0 2019-11-18 21:08:01.000000 Joule-0.9.8/joule/
--rw-r--r--   0 jdonnal    (501) staff       (20)      453 2019-01-12 01:45:31.000000 Joule-0.9.8/joule/__init__.py
--rw-r--r--   0 jdonnal    (501) staff       (20)      497 2019-11-18 21:08:01.000000 Joule-0.9.8/joule/_version.py
-drwxr-xr-x   0 jdonnal    (501) staff       (20)        0 2019-11-18 21:08:01.000000 Joule-0.9.8/joule/api/
--rw-r--r--   0 jdonnal    (501) staff       (20)      392 2019-07-30 18:18:45.000000 Joule-0.9.8/joule/api/__init__.py
--rw-r--r--   0 jdonnal    (501) staff       (20)     3639 2019-07-30 18:38:53.000000 Joule-0.9.8/joule/api/annotation.py
--rw-r--r--   0 jdonnal    (501) staff       (20)    10155 2019-05-09 14:20:06.000000 Joule-0.9.8/joule/api/data.py
--rw-r--r--   0 jdonnal    (501) staff       (20)      654 2019-07-25 14:38:07.000000 Joule-0.9.8/joule/api/db.py
--rw-r--r--   0 jdonnal    (501) staff       (20)     2875 2019-05-09 14:20:06.000000 Joule-0.9.8/joule/api/folder.py
--rw-r--r--   0 jdonnal    (501) staff       (20)     1738 2019-03-05 19:38:44.000000 Joule-0.9.8/joule/api/folder_type.py
--rw-r--r--   0 jdonnal    (501) staff       (20)     7204 2019-05-09 14:20:06.000000 Joule-0.9.8/joule/api/helpers.py
--rw-r--r--   0 jdonnal    (501) staff       (20)     1503 2019-05-10 21:28:44.000000 Joule-0.9.8/joule/api/master.py
--rw-r--r--   0 jdonnal    (501) staff       (20)     4473 2019-05-15 21:39:02.000000 Joule-0.9.8/joule/api/module.py
-drwxr-xr-x   0 jdonnal    (501) staff       (20)        0 2019-11-18 21:08:01.000000 Joule-0.9.8/joule/api/node/
--rw-r--r--   0 jdonnal    (501) staff       (20)       94 2019-05-09 14:20:06.000000 Joule-0.9.8/joule/api/node/__init__.py
--rw-r--r--   0 jdonnal    (501) staff       (20)     8886 2019-07-25 00:25:11.000000 Joule-0.9.8/joule/api/node/base_node.py
--rw-r--r--   0 jdonnal    (501) staff       (20)      268 2019-05-09 14:20:06.000000 Joule-0.9.8/joule/api/node/node_config.py
--rw-r--r--   0 jdonnal    (501) staff       (20)      122 2019-05-09 14:20:06.000000 Joule-0.9.8/joule/api/node/node_info.py
--rw-r--r--   0 jdonnal    (501) staff       (20)      988 2019-05-09 14:20:06.000000 Joule-0.9.8/joule/api/node/tcp_node.py
--rw-r--r--   0 jdonnal    (501) staff       (20)      877 2019-05-09 14:20:06.000000 Joule-0.9.8/joule/api/node/unix_node.py
--rw-r--r--   0 jdonnal    (501) staff       (20)     1427 2019-09-11 15:34:37.000000 Joule-0.9.8/joule/api/proxy.py
-drwxr-xr-x   0 jdonnal    (501) staff       (20)        0 2019-11-18 21:08:01.000000 Joule-0.9.8/joule/api/session/
--rw-r--r--   0 jdonnal    (501) staff       (20)      112 2019-05-09 14:20:06.000000 Joule-0.9.8/joule/api/session/__init__.py
--rw-r--r--   0 jdonnal    (501) staff       (20)     1018 2019-05-09 14:20:06.000000 Joule-0.9.8/joule/api/session/base_session.py
--rw-r--r--   0 jdonnal    (501) staff       (20)     2709 2019-05-09 14:20:06.000000 Joule-0.9.8/joule/api/session/tcp_session.py
--rw-r--r--   0 jdonnal    (501) staff       (20)     1759 2019-07-25 00:12:27.000000 Joule-0.9.8/joule/api/session/unix_session.py
--rw-r--r--   0 jdonnal    (501) staff       (20)    11565 2019-06-28 19:38:12.000000 Joule-0.9.8/joule/api/stream.py
-drwxr-xr-x   0 jdonnal    (501) staff       (20)        0 2019-11-18 21:08:01.000000 Joule-0.9.8/joule/cli/
--rw-r--r--   0 jdonnal    (501) staff       (20)      894 2019-05-09 14:20:06.000000 Joule-0.9.8/joule/cli/__init__.py
-drwxr-xr-x   0 jdonnal    (501) staff       (20)        0 2019-11-18 21:08:01.000000 Joule-0.9.8/joule/cli/admin/
--rw-r--r--   0 jdonnal    (501) staff       (20)      429 2019-07-26 18:44:59.000000 Joule-0.9.8/joule/cli/admin/__init__.py
--rw-r--r--   0 jdonnal    (501) staff       (20)     3101 2019-09-11 15:34:37.000000 Joule-0.9.8/joule/cli/admin/authorize.py
--rw-r--r--   0 jdonnal    (501) staff       (20)     3175 2019-09-11 15:34:37.000000 Joule-0.9.8/joule/cli/admin/backup.py
--rw-r--r--   0 jdonnal    (501) staff       (20)     3260 2019-09-11 15:34:37.000000 Joule-0.9.8/joule/cli/admin/erase.py
--rw-r--r--   0 jdonnal    (501) staff       (20)    17428 2019-09-11 15:34:37.000000 Joule-0.9.8/joule/cli/admin/ingest.py
--rw-r--r--   0 jdonnal    (501) staff       (20)     6032 2019-11-13 01:07:36.000000 Joule-0.9.8/joule/cli/admin/initialize.py
-drwxr-xr-x   0 jdonnal    (501) staff       (20)        0 2019-11-18 21:08:01.000000 Joule-0.9.8/joule/cli/admin/local_postgres_templates/
--rw-r--r--   0 jdonnal    (501) staff       (20)       68 2019-07-24 01:06:55.000000 Joule-0.9.8/joule/cli/admin/local_postgres_templates/pg_hba.conf.jinja2
--rw-r--r--   0 jdonnal    (501) staff       (20)        0 2019-07-18 00:42:32.000000 Joule-0.9.8/joule/cli/admin/local_postgres_templates/pg_ident.conf.jinja2
--rw-r--r--   0 jdonnal    (501) staff       (20)     1874 2019-07-26 17:58:05.000000 Joule-0.9.8/joule/cli/admin/local_postgres_templates/postgresql.conf.jinja2
--rw-r--r--   0 jdonnal    (501) staff       (20)      110 2019-07-20 21:13:28.000000 Joule-0.9.8/joule/cli/admin/local_postgres_templates/recovery.conf.jinja2
--rw-r--r--   0 jdonnal    (501) staff       (20)      725 2019-06-28 19:28:13.000000 Joule-0.9.8/joule/cli/config.py
-drwxr-xr-x   0 jdonnal    (501) staff       (20)        0 2019-11-18 21:08:01.000000 Joule-0.9.8/joule/cli/data/
--rw-r--r--   0 jdonnal    (501) staff       (20)      354 2019-05-09 14:20:06.000000 Joule-0.9.8/joule/cli/data/__init__.py
--rw-r--r--   0 jdonnal    (501) staff       (20)    14859 2019-09-11 15:34:37.000000 Joule-0.9.8/joule/cli/data/copy.py
--rw-r--r--   0 jdonnal    (501) staff       (20)     1529 2019-05-29 14:04:54.000000 Joule-0.9.8/joule/cli/data/intervals.py
--rw-r--r--   0 jdonnal    (501) staff       (20)     3077 2019-05-29 14:04:54.000000 Joule-0.9.8/joule/cli/data/read.py
--rw-r--r--   0 jdonnal    (501) staff       (20)     1561 2019-05-29 14:04:54.000000 Joule-0.9.8/joule/cli/data/remove.py
--rw-r--r--   0 jdonnal    (501) staff       (20)     1257 2019-05-29 14:04:54.000000 Joule-0.9.8/joule/cli/folder.py
-drwxr-xr-x   0 jdonnal    (501) staff       (20)        0 2019-11-18 21:08:01.000000 Joule-0.9.8/joule/cli/follower/
--rw-r--r--   0 jdonnal    (501) staff       (20)      224 2019-05-09 14:20:06.000000 Joule-0.9.8/joule/cli/follower/__init__.py
--rw-r--r--   0 jdonnal    (501) staff       (20)      576 2019-05-29 14:04:54.000000 Joule-0.9.8/joule/cli/follower/delete.py
--rw-r--r--   0 jdonnal    (501) staff       (20)      781 2019-05-29 14:04:54.000000 Joule-0.9.8/joule/cli/follower/list.py
--rw-r--r--   0 jdonnal    (501) staff       (20)       86 2019-05-09 14:20:06.000000 Joule-0.9.8/joule/cli/helpers.py
-drwxr-xr-x   0 jdonnal    (501) staff       (20)        0 2019-11-18 21:08:01.000000 Joule-0.9.8/joule/cli/master/
--rw-r--r--   0 jdonnal    (501) staff       (20)      259 2019-05-09 14:20:06.000000 Joule-0.9.8/joule/cli/master/__init__.py
--rw-r--r--   0 jdonnal    (501) staff       (20)     2940 2019-10-04 20:14:05.000000 Joule-0.9.8/joule/cli/master/add.py
--rw-r--r--   0 jdonnal    (501) staff       (20)      757 2019-05-29 14:04:54.000000 Joule-0.9.8/joule/cli/master/delete.py
--rw-r--r--   0 jdonnal    (501) staff       (20)     1315 2019-05-29 14:04:54.000000 Joule-0.9.8/joule/cli/master/list.py
-drwxr-xr-x   0 jdonnal    (501) staff       (20)        0 2019-11-18 21:08:01.000000 Joule-0.9.8/joule/cli/module/
--rw-r--r--   0 jdonnal    (501) staff       (20)      256 2019-01-12 01:46:25.000000 Joule-0.9.8/joule/cli/module/__init__.py
--rw-r--r--   0 jdonnal    (501) staff       (20)     1647 2019-05-29 14:04:54.000000 Joule-0.9.8/joule/cli/module/info.py
--rw-r--r--   0 jdonnal    (501) staff       (20)     1621 2019-05-29 14:03:46.000000 Joule-0.9.8/joule/cli/module/list.py
--rw-r--r--   0 jdonnal    (501) staff       (20)      645 2019-05-29 14:04:54.000000 Joule-0.9.8/joule/cli/module/logs.py
-drwxr-xr-x   0 jdonnal    (501) staff       (20)        0 2019-11-18 21:08:01.000000 Joule-0.9.8/joule/cli/node/
--rw-r--r--   0 jdonnal    (501) staff       (20)      376 2019-05-09 14:20:06.000000 Joule-0.9.8/joule/cli/node/__init__.py
--rw-r--r--   0 jdonnal    (501) staff       (20)      972 2019-08-03 18:52:44.000000 Joule-0.9.8/joule/cli/node/add.py
--rw-r--r--   0 jdonnal    (501) staff       (20)      351 2019-05-09 14:20:06.000000 Joule-0.9.8/joule/cli/node/default.py
--rw-r--r--   0 jdonnal    (501) staff       (20)      365 2019-05-09 14:20:06.000000 Joule-0.9.8/joule/cli/node/delete.py
--rw-r--r--   0 jdonnal    (501) staff       (20)      592 2019-05-29 14:04:54.000000 Joule-0.9.8/joule/cli/node/info.py
--rw-r--r--   0 jdonnal    (501) staff       (20)      836 2019-05-09 14:20:06.000000 Joule-0.9.8/joule/cli/node/list.py
-drwxr-xr-x   0 jdonnal    (501) staff       (20)        0 2019-11-18 21:08:01.000000 Joule-0.9.8/joule/cli/proxy/
--rw-r--r--   0 jdonnal    (501) staff       (20)      202 2019-05-09 14:20:06.000000 Joule-0.9.8/joule/cli/proxy/__init__.py
--rw-r--r--   0 jdonnal    (501) staff       (20)      920 2019-05-29 14:04:54.000000 Joule-0.9.8/joule/cli/proxy/info.py
--rw-r--r--   0 jdonnal    (501) staff       (20)      909 2019-09-11 15:34:37.000000 Joule-0.9.8/joule/cli/proxy/list.py
-drwxr-xr-x   0 jdonnal    (501) staff       (20)        0 2019-11-18 21:08:01.000000 Joule-0.9.8/joule/cli/stream/
--rw-r--r--   0 jdonnal    (501) staff       (20)      436 2019-06-28 18:41:11.000000 Joule-0.9.8/joule/cli/stream/__init__.py
--rw-r--r--   0 jdonnal    (501) staff       (20)     2413 2019-06-28 19:42:12.000000 Joule-0.9.8/joule/cli/stream/annotation.py
--rw-r--r--   0 jdonnal    (501) staff       (20)      674 2019-05-29 14:04:54.000000 Joule-0.9.8/joule/cli/stream/destroy.py
--rw-r--r--   0 jdonnal    (501) staff       (20)     3301 2019-05-29 14:04:54.000000 Joule-0.9.8/joule/cli/stream/info.py
--rw-r--r--   0 jdonnal    (501) staff       (20)     2309 2019-07-26 18:40:00.000000 Joule-0.9.8/joule/cli/stream/list.py
--rw-r--r--   0 jdonnal    (501) staff       (20)      635 2019-05-29 14:04:54.000000 Joule-0.9.8/joule/cli/stream/move.py
--rw-r--r--   0 jdonnal    (501) staff       (20)        0 2019-01-12 01:46:25.000000 Joule-0.9.8/joule/cli.py
-drwxr-xr-x   0 jdonnal    (501) staff       (20)        0 2019-11-18 21:08:01.000000 Joule-0.9.8/joule/client/
--rw-r--r--   0 jdonnal    (501) staff       (20)      269 2019-01-12 01:45:31.000000 Joule-0.9.8/joule/client/__init__.py
--rw-r--r--   0 jdonnal    (501) staff       (20)    12997 2019-10-04 01:41:32.000000 Joule-0.9.8/joule/client/base_module.py
-drwxr-xr-x   0 jdonnal    (501) staff       (20)        0 2019-11-18 21:08:01.000000 Joule-0.9.8/joule/client/builtins/
--rw-r--r--   0 jdonnal    (501) staff       (20)        0 2018-10-06 23:32:02.000000 Joule-0.9.8/joule/client/builtins/__init__.py
-drwxr-xr-x   0 jdonnal    (501) staff       (20)        0 2019-11-18 21:08:01.000000 Joule-0.9.8/joule/client/builtins/__pycache__/
--rw-r--r--   0 jdonnal    (501) staff       (20)      127 2019-05-16 13:38:27.000000 Joule-0.9.8/joule/client/builtins/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0 jdonnal    (501) staff       (20)     2746 2019-07-24 20:23:35.000000 Joule-0.9.8/joule/client/builtins/__pycache__/file_reader.cpython-36.pyc
--rw-r--r--   0 jdonnal    (501) staff       (20)     2383 2019-05-16 13:38:28.000000 Joule-0.9.8/joule/client/builtins/__pycache__/mean_filter.cpython-36.pyc
--rw-r--r--   0 jdonnal    (501) staff       (20)     2926 2019-05-16 13:38:28.000000 Joule-0.9.8/joule/client/builtins/__pycache__/median_filter.cpython-36.pyc
--rw-r--r--   0 jdonnal    (501) staff       (20)     2912 2019-05-16 13:38:28.000000 Joule-0.9.8/joule/client/builtins/__pycache__/random_reader.cpython-36.pyc
--rw-r--r--   0 jdonnal    (501) staff       (20)     4706 2019-08-16 19:15:44.000000 Joule-0.9.8/joule/client/builtins/__pycache__/visualizer.cpython-36.pyc
-drwxr-xr-x   0 jdonnal    (501) staff       (20)        0 2019-11-18 21:08:01.000000 Joule-0.9.8/joule/client/builtins/assets/
-drwxr-xr-x   0 jdonnal    (501) staff       (20)        0 2019-11-18 21:08:01.000000 Joule-0.9.8/joule/client/builtins/assets/css/
--rw-r--r--   0 jdonnal    (501) staff       (20)   140936 2019-01-12 01:45:31.000000 Joule-0.9.8/joule/client/builtins/assets/css/bootstrap.min.css
--rw-r--r--   0 jdonnal    (501) staff       (20)   562427 2019-01-12 01:45:31.000000 Joule-0.9.8/joule/client/builtins/assets/css/bootstrap.min.css.map
--rw-r--r--   0 jdonnal    (501) staff       (20)      646 2019-01-12 01:45:31.000000 Joule-0.9.8/joule/client/builtins/assets/css/index.css
-drwxr-xr-x   0 jdonnal    (501) staff       (20)        0 2019-11-18 21:08:01.000000 Joule-0.9.8/joule/client/builtins/assets/js/
--rw-r--r--   0 jdonnal    (501) staff       (20)    70966 2019-01-12 01:45:31.000000 Joule-0.9.8/joule/client/builtins/assets/js/bootstrap.bundle.min.js
--rw-r--r--   0 jdonnal    (501) staff       (20)   294126 2019-01-12 01:45:31.000000 Joule-0.9.8/joule/client/builtins/assets/js/bootstrap.bundle.min.js.map
--rw-r--r--   0 jdonnal    (501) staff       (20)     1871 2019-08-27 13:06:55.000000 Joule-0.9.8/joule/client/builtins/assets/js/index.js
--rw-r--r--   0 jdonnal    (501) staff       (20)    86927 2019-01-12 01:45:31.000000 Joule-0.9.8/joule/client/builtins/assets/js/jquery-3.3.1.min.js
--rw-r--r--   0 jdonnal    (501) staff       (20)   132382 2019-01-12 01:45:31.000000 Joule-0.9.8/joule/client/builtins/assets/js/jquery-3.3.1.min.map
--rw-r--r--   0 jdonnal    (501) staff       (20)    19188 2019-01-12 01:45:31.000000 Joule-0.9.8/joule/client/builtins/assets/js/popper.min.js
--rw-r--r--   0 jdonnal    (501) staff       (20)   112587 2019-01-12 01:45:31.000000 Joule-0.9.8/joule/client/builtins/assets/js/popper.min.js.map
-drwxr-xr-x   0 jdonnal    (501) staff       (20)        0 2019-11-18 21:08:01.000000 Joule-0.9.8/joule/client/builtins/assets/templates/
--rw-r--r--   0 jdonnal    (501) staff       (20)      737 2019-09-11 15:34:37.000000 Joule-0.9.8/joule/client/builtins/assets/templates/base.jinja2
--rw-r--r--   0 jdonnal    (501) staff       (20)     3274 2019-08-16 19:06:21.000000 Joule-0.9.8/joule/client/builtins/assets/templates/index.jinja2
--rw-r--r--   0 jdonnal    (501) staff       (20)     2556 2019-07-16 18:08:37.000000 Joule-0.9.8/joule/client/builtins/file_reader.py
--rw-r--r--   0 jdonnal    (501) staff       (20)     2041 2019-01-12 01:45:31.000000 Joule-0.9.8/joule/client/builtins/mean_filter.py
--rw-r--r--   0 jdonnal    (501) staff       (20)     3458 2019-02-06 03:28:37.000000 Joule-0.9.8/joule/client/builtins/median_filter.py
--rw-r--r--   0 jdonnal    (501) staff       (20)     3187 2019-01-12 01:45:31.000000 Joule-0.9.8/joule/client/builtins/random_reader.py
--rw-r--r--   0 jdonnal    (501) staff       (20)     4728 2019-09-11 15:34:37.000000 Joule-0.9.8/joule/client/builtins/visualizer.py
--rw-r--r--   0 jdonnal    (501) staff       (20)     1414 2019-09-11 15:34:37.000000 Joule-0.9.8/joule/client/composite_module.py
--rw-r--r--   0 jdonnal    (501) staff       (20)     1992 2019-09-11 15:34:37.000000 Joule-0.9.8/joule/client/filter_module.py
--rw-r--r--   0 jdonnal    (501) staff       (20)     2335 2019-02-06 02:58:41.000000 Joule-0.9.8/joule/client/fir_filter_module.py
-drwxr-xr-x   0 jdonnal    (501) staff       (20)        0 2019-11-18 21:08:01.000000 Joule-0.9.8/joule/client/helpers/
--rw-r--r--   0 jdonnal    (501) staff       (20)      409 2019-10-02 01:19:37.000000 Joule-0.9.8/joule/client/helpers/__init__.py
--rw-r--r--   0 jdonnal    (501) staff       (20)     3452 2019-10-04 01:32:21.000000 Joule-0.9.8/joule/client/helpers/args.py
--rw-r--r--   0 jdonnal    (501) staff       (20)     7094 2019-10-04 18:22:25.000000 Joule-0.9.8/joule/client/helpers/pipes.py
--rw-r--r--   0 jdonnal    (501) staff       (20)     2853 2019-10-01 00:50:09.000000 Joule-0.9.8/joule/client/reader_module.py
-drwxr-xr-x   0 jdonnal    (501) staff       (20)        0 2019-11-18 21:08:01.000000 Joule-0.9.8/joule/controllers/
--rw-r--r--   0 jdonnal    (501) staff       (20)     2724 2019-09-11 15:34:37.000000 Joule-0.9.8/joule/controllers/__init__.py
--rw-r--r--   0 jdonnal    (501) staff       (20)     5262 2019-07-03 00:41:10.000000 Joule-0.9.8/joule/controllers/annotation_controller.py
--rw-r--r--   0 jdonnal    (501) staff       (20)     1455 2019-09-11 15:34:37.000000 Joule-0.9.8/joule/controllers/app_controller.py
--rw-r--r--   0 jdonnal    (501) staff       (20)     9933 2019-03-01 01:35:57.000000 Joule-0.9.8/joule/controllers/data_controller.py
--rw-r--r--   0 jdonnal    (501) staff       (20)     6075 2019-07-03 17:48:25.000000 Joule-0.9.8/joule/controllers/folder_controller.py
--rw-r--r--   0 jdonnal    (501) staff       (20)     2626 2019-11-07 02:16:36.000000 Joule-0.9.8/joule/controllers/follower_controller.py
--rw-r--r--   0 jdonnal    (501) staff       (20)     7873 2019-10-04 20:16:58.000000 Joule-0.9.8/joule/controllers/master_controller.py
--rw-r--r--   0 jdonnal    (501) staff       (20)     2480 2019-05-15 21:39:02.000000 Joule-0.9.8/joule/controllers/module_controller.py
--rw-r--r--   0 jdonnal    (501) staff       (20)     1055 2019-05-09 14:20:06.000000 Joule-0.9.8/joule/controllers/proxy_controller.py
--rw-r--r--   0 jdonnal    (501) staff       (20)      772 2019-07-25 00:07:43.000000 Joule-0.9.8/joule/controllers/root_controller.py
--rw-r--r--   0 jdonnal    (501) staff       (20)     7042 2019-07-24 01:30:48.000000 Joule-0.9.8/joule/controllers/stream_controller.py
--rw-r--r--   0 jdonnal    (501) staff       (20)    13427 2019-10-17 17:01:17.000000 Joule-0.9.8/joule/daemon.py
--rw-r--r--   0 jdonnal    (501) staff       (20)      851 2019-08-13 00:05:57.000000 Joule-0.9.8/joule/errors.py
--rw-r--r--   0 jdonnal    (501) staff       (20)     2458 2019-11-18 21:06:53.000000 Joule-0.9.8/joule/middleware.py
-drwxr-xr-x   0 jdonnal    (501) staff       (20)        0 2019-11-18 21:08:01.000000 Joule-0.9.8/joule/models/
--rw-r--r--   0 jdonnal    (501) staff       (20)      714 2019-06-20 18:24:19.000000 Joule-0.9.8/joule/models/__init__.py
--rw-r--r--   0 jdonnal    (501) staff       (20)     2288 2019-07-03 00:20:56.000000 Joule-0.9.8/joule/models/annotation.py
--rw-r--r--   0 jdonnal    (501) staff       (20)     1891 2019-09-11 15:34:37.000000 Joule-0.9.8/joule/models/config.py
-drwxr-xr-x   0 jdonnal    (501) staff       (20)        0 2019-11-18 21:08:01.000000 Joule-0.9.8/joule/models/data_store/
--rw-r--r--   0 jdonnal    (501) staff       (20)      167 2019-01-12 01:45:31.000000 Joule-0.9.8/joule/models/data_store/__init__.py
--rw-r--r--   0 jdonnal    (501) staff       (20)     2863 2019-01-25 02:08:22.000000 Joule-0.9.8/joule/models/data_store/data_store.py
--rw-r--r--   0 jdonnal    (501) staff       (20)       94 2019-01-12 01:45:31.000000 Joule-0.9.8/joule/models/data_store/errors.py
--rw-r--r--   0 jdonnal    (501) staff       (20)    14472 2019-09-16 18:17:46.000000 Joule-0.9.8/joule/models/data_store/nilmdb.py
--rw-r--r--   0 jdonnal    (501) staff       (20)     1054 2019-01-25 02:08:22.000000 Joule-0.9.8/joule/models/data_store/nilmdb_helpers.py
--rw-r--r--   0 jdonnal    (501) staff       (20)    12945 2019-01-12 01:45:31.000000 Joule-0.9.8/joule/models/data_store/nilmdb_inserter.py
--rw-r--r--   0 jdonnal    (501) staff       (20)    11610 2019-07-30 01:05:34.000000 Joule-0.9.8/joule/models/data_store/psql_helpers.py
-drwxr-xr-x   0 jdonnal    (501) staff       (20)        0 2019-11-18 21:08:01.000000 Joule-0.9.8/joule/models/data_store/sql/
--rw-r--r--   0 jdonnal    (501) staff       (20)     1473 2019-01-12 01:45:31.000000 Joule-0.9.8/joule/models/data_store/sql/info.sql
--rw-r--r--   0 jdonnal    (501) staff       (20)     1374 2019-09-16 18:10:00.000000 Joule-0.9.8/joule/models/data_store/sql/row_count.sql
--rw-r--r--   0 jdonnal    (501) staff       (20)    11847 2019-10-04 00:27:20.000000 Joule-0.9.8/joule/models/data_store/timescale.py
--rw-r--r--   0 jdonnal    (501) staff       (20)     8032 2019-10-04 00:29:49.000000 Joule-0.9.8/joule/models/data_store/timescale_inserter.py
--rw-r--r--   0 jdonnal    (501) staff       (20)     7683 2019-07-03 01:34:14.000000 Joule-0.9.8/joule/models/element.py
--rw-r--r--   0 jdonnal    (501) staff       (20)     4912 2019-05-09 14:20:06.000000 Joule-0.9.8/joule/models/folder.py
--rw-r--r--   0 jdonnal    (501) staff       (20)      979 2019-05-09 14:20:06.000000 Joule-0.9.8/joule/models/follower.py
--rw-r--r--   0 jdonnal    (501) staff       (20)     1290 2019-05-09 14:20:06.000000 Joule-0.9.8/joule/models/master.py
--rw-r--r--   0 jdonnal    (501) staff       (20)       83 2019-01-12 01:45:31.000000 Joule-0.9.8/joule/models/meta.py
--rw-r--r--   0 jdonnal    (501) staff       (20)     2946 2019-05-15 21:39:02.000000 Joule-0.9.8/joule/models/module.py
-drwxr-xr-x   0 jdonnal    (501) staff       (20)        0 2019-11-18 21:08:01.000000 Joule-0.9.8/joule/models/pipes/
--rw-r--r--   0 jdonnal    (501) staff       (20)      382 2019-01-12 01:45:31.000000 Joule-0.9.8/joule/models/pipes/__init__.py
--rw-r--r--   0 jdonnal    (501) staff       (20)      219 2019-08-13 00:07:39.000000 Joule-0.9.8/joule/models/pipes/errors.py
--rw-r--r--   0 jdonnal    (501) staff       (20)      875 2019-01-12 01:45:31.000000 Joule-0.9.8/joule/models/pipes/factories.py
--rw-r--r--   0 jdonnal    (501) staff       (20)     5251 2019-03-02 18:35:49.000000 Joule-0.9.8/joule/models/pipes/input_pipe.py
--rw-r--r--   0 jdonnal    (501) staff       (20)     8719 2019-07-24 20:08:18.000000 Joule-0.9.8/joule/models/pipes/local_pipe.py
--rw-r--r--   0 jdonnal    (501) staff       (20)     3597 2019-11-07 02:16:36.000000 Joule-0.9.8/joule/models/pipes/output_pipe.py
--rw-r--r--   0 jdonnal    (501) staff       (20)     9313 2019-02-26 02:09:04.000000 Joule-0.9.8/joule/models/pipes/pipe.py
--rw-r--r--   0 jdonnal    (501) staff       (20)      283 2019-05-09 14:20:06.000000 Joule-0.9.8/joule/models/proxy.py
--rw-r--r--   0 jdonnal    (501) staff       (20)    11826 2019-07-03 01:31:42.000000 Joule-0.9.8/joule/models/stream.py
--rw-r--r--   0 jdonnal    (501) staff       (20)     7440 2019-09-11 15:34:37.000000 Joule-0.9.8/joule/models/supervisor.py
--rw-r--r--   0 jdonnal    (501) staff       (20)    16440 2019-10-03 20:43:18.000000 Joule-0.9.8/joule/models/worker.py
-drwxr-xr-x   0 jdonnal    (501) staff       (20)        0 2019-11-18 21:08:01.000000 Joule-0.9.8/joule/resources/
--rw-r--r--   0 jdonnal    (501) staff       (20)      267 2019-05-09 14:20:06.000000 Joule-0.9.8/joule/resources/joule.service
-drwxr-xr-x   0 jdonnal    (501) staff       (20)        0 2019-11-18 21:08:01.000000 Joule-0.9.8/joule/resources/templates/
--rw-r--r--   0 jdonnal    (501) staff       (20)     1766 2019-11-13 01:04:01.000000 Joule-0.9.8/joule/resources/templates/main.conf.jinja2
--rw-r--r--   0 jdonnal    (501) staff       (20)      740 2019-02-20 14:21:11.000000 Joule-0.9.8/joule/resources/templates/module.example
--rw-r--r--   0 jdonnal    (501) staff       (20)     1013 2019-02-20 13:10:26.000000 Joule-0.9.8/joule/resources/templates/stream.example
-drwxr-xr-x   0 jdonnal    (501) staff       (20)        0 2019-11-18 21:08:01.000000 Joule-0.9.8/joule/services/
--rw-r--r--   0 jdonnal    (501) staff       (20)        0 2019-01-12 01:45:31.000000 Joule-0.9.8/joule/services/__init__.py
--rw-r--r--   0 jdonnal    (501) staff       (20)      804 2019-01-12 01:45:31.000000 Joule-0.9.8/joule/services/helpers.py
--rw-r--r--   0 jdonnal    (501) staff       (20)     6468 2019-09-11 21:04:01.000000 Joule-0.9.8/joule/services/load_config.py
--rw-r--r--   0 jdonnal    (501) staff       (20)     3142 2019-01-12 01:45:31.000000 Joule-0.9.8/joule/services/load_modules.py
--rw-r--r--   0 jdonnal    (501) staff       (20)     2436 2019-01-12 01:45:31.000000 Joule-0.9.8/joule/services/load_streams.py
--rw-r--r--   0 jdonnal    (501) staff       (20)     5056 2019-10-17 01:09:02.000000 Joule-0.9.8/joule/services/parse_pipe_config.py
-drwxr-xr-x   0 jdonnal    (501) staff       (20)        0 2019-11-18 21:08:01.000000 Joule-0.9.8/joule/utilities/
--rw-r--r--   0 jdonnal    (501) staff       (20)      422 2019-07-24 23:58:30.000000 Joule-0.9.8/joule/utilities/__init__.py
--rw-r--r--   0 jdonnal    (501) staff       (20)     1755 2019-08-07 18:44:38.000000 Joule-0.9.8/joule/utilities/connection_info.py
--rw-r--r--   0 jdonnal    (501) staff       (20)     2578 2019-01-12 01:45:31.000000 Joule-0.9.8/joule/utilities/interval_tools.py
--rw-r--r--   0 jdonnal    (501) staff       (20)     1547 2019-07-03 16:23:28.000000 Joule-0.9.8/joule/utilities/misc.py
--rw-r--r--   0 jdonnal    (501) staff       (20)      426 2019-01-25 02:08:22.000000 Joule-0.9.8/joule/utilities/stream.py
--rw-r--r--   0 jdonnal    (501) staff       (20)     1985 2019-06-20 20:40:11.000000 Joule-0.9.8/joule/utilities/time.py
--rw-r--r--   0 jdonnal    (501) staff       (20)      200 2019-11-18 21:08:01.000000 Joule-0.9.8/setup.cfg
--rw-r--r--   0 jdonnal    (501) staff       (20)     2439 2019-07-09 01:21:43.000000 Joule-0.9.8/setup.py
--rw-r--r--   0 jdonnal    (501) staff       (20)    68611 2019-01-12 01:45:31.000000 Joule-0.9.8/versioneer.py
+drwxr-xr-x   0 jdonnal    (501) staff       (20)        0 2019-11-21 20:50:45.000000 Joule-0.9.9/
+drwxr-xr-x   0 jdonnal    (501) staff       (20)        0 2019-11-21 20:50:45.000000 Joule-0.9.9/Joule.egg-info/
+-rw-r--r--   0 jdonnal    (501) staff       (20)     3738 2019-11-21 20:50:45.000000 Joule-0.9.9/Joule.egg-info/PKG-INFO
+-rw-r--r--   0 jdonnal    (501) staff       (20)     5576 2019-11-21 20:50:45.000000 Joule-0.9.9/Joule.egg-info/SOURCES.txt
+-rw-r--r--   0 jdonnal    (501) staff       (20)        1 2019-11-21 20:50:45.000000 Joule-0.9.9/Joule.egg-info/dependency_links.txt
+-rw-r--r--   0 jdonnal    (501) staff       (20)      377 2019-11-21 20:50:45.000000 Joule-0.9.9/Joule.egg-info/entry_points.txt
+-rw-r--r--   0 jdonnal    (501) staff       (20)        1 2019-11-21 20:50:45.000000 Joule-0.9.9/Joule.egg-info/namespace_packages.txt
+-rw-r--r--   0 jdonnal    (501) staff       (20)        1 2018-10-06 23:40:12.000000 Joule-0.9.9/Joule.egg-info/not-zip-safe
+-rw-r--r--   0 jdonnal    (501) staff       (20)      184 2019-11-21 20:50:45.000000 Joule-0.9.9/Joule.egg-info/requires.txt
+-rw-r--r--   0 jdonnal    (501) staff       (20)       12 2019-11-21 20:50:45.000000 Joule-0.9.9/Joule.egg-info/top_level.txt
+-rw-r--r--   0 jdonnal    (501) staff       (20)      248 2019-07-26 18:42:54.000000 Joule-0.9.9/MANIFEST.in
+-rw-r--r--   0 jdonnal    (501) staff       (20)     3738 2019-11-21 20:50:45.000000 Joule-0.9.9/PKG-INFO
+-rw-r--r--   0 jdonnal    (501) staff       (20)     2664 2019-07-03 18:08:20.000000 Joule-0.9.9/README.rst
+drwxr-xr-x   0 jdonnal    (501) staff       (20)        0 2019-11-21 20:50:45.000000 Joule-0.9.9/joule/
+-rw-r--r--   0 jdonnal    (501) staff       (20)      453 2019-01-12 01:45:31.000000 Joule-0.9.9/joule/__init__.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)      497 2019-11-21 20:50:45.000000 Joule-0.9.9/joule/_version.py
+drwxr-xr-x   0 jdonnal    (501) staff       (20)        0 2019-11-21 20:50:45.000000 Joule-0.9.9/joule/api/
+-rw-r--r--   0 jdonnal    (501) staff       (20)      392 2019-07-30 18:18:45.000000 Joule-0.9.9/joule/api/__init__.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)     3639 2019-07-30 18:38:53.000000 Joule-0.9.9/joule/api/annotation.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)    10155 2019-05-09 14:20:06.000000 Joule-0.9.9/joule/api/data.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)      654 2019-07-25 14:38:07.000000 Joule-0.9.9/joule/api/db.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)     2875 2019-05-09 14:20:06.000000 Joule-0.9.9/joule/api/folder.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)     1738 2019-03-05 19:38:44.000000 Joule-0.9.9/joule/api/folder_type.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)     7204 2019-05-09 14:20:06.000000 Joule-0.9.9/joule/api/helpers.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)     1503 2019-05-10 21:28:44.000000 Joule-0.9.9/joule/api/master.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)     4473 2019-05-15 21:39:02.000000 Joule-0.9.9/joule/api/module.py
+drwxr-xr-x   0 jdonnal    (501) staff       (20)        0 2019-11-21 20:50:45.000000 Joule-0.9.9/joule/api/node/
+-rw-r--r--   0 jdonnal    (501) staff       (20)       94 2019-05-09 14:20:06.000000 Joule-0.9.9/joule/api/node/__init__.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)     8886 2019-07-25 00:25:11.000000 Joule-0.9.9/joule/api/node/base_node.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)      268 2019-05-09 14:20:06.000000 Joule-0.9.9/joule/api/node/node_config.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)      122 2019-05-09 14:20:06.000000 Joule-0.9.9/joule/api/node/node_info.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)      988 2019-05-09 14:20:06.000000 Joule-0.9.9/joule/api/node/tcp_node.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)      877 2019-05-09 14:20:06.000000 Joule-0.9.9/joule/api/node/unix_node.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)     1427 2019-09-11 15:34:37.000000 Joule-0.9.9/joule/api/proxy.py
+drwxr-xr-x   0 jdonnal    (501) staff       (20)        0 2019-11-21 20:50:45.000000 Joule-0.9.9/joule/api/session/
+-rw-r--r--   0 jdonnal    (501) staff       (20)      112 2019-05-09 14:20:06.000000 Joule-0.9.9/joule/api/session/__init__.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)     1018 2019-05-09 14:20:06.000000 Joule-0.9.9/joule/api/session/base_session.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)     2709 2019-05-09 14:20:06.000000 Joule-0.9.9/joule/api/session/tcp_session.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)     1759 2019-07-25 00:12:27.000000 Joule-0.9.9/joule/api/session/unix_session.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)    11565 2019-06-28 19:38:12.000000 Joule-0.9.9/joule/api/stream.py
+drwxr-xr-x   0 jdonnal    (501) staff       (20)        0 2019-11-21 20:50:45.000000 Joule-0.9.9/joule/cli/
+-rw-r--r--   0 jdonnal    (501) staff       (20)      894 2019-05-09 14:20:06.000000 Joule-0.9.9/joule/cli/__init__.py
+drwxr-xr-x   0 jdonnal    (501) staff       (20)        0 2019-11-21 20:50:45.000000 Joule-0.9.9/joule/cli/admin/
+-rw-r--r--   0 jdonnal    (501) staff       (20)      429 2019-07-26 18:44:59.000000 Joule-0.9.9/joule/cli/admin/__init__.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)     3101 2019-09-11 15:34:37.000000 Joule-0.9.9/joule/cli/admin/authorize.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)     3175 2019-09-11 15:34:37.000000 Joule-0.9.9/joule/cli/admin/backup.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)     3260 2019-09-11 15:34:37.000000 Joule-0.9.9/joule/cli/admin/erase.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)    17428 2019-09-11 15:34:37.000000 Joule-0.9.9/joule/cli/admin/ingest.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)     6032 2019-11-13 01:07:36.000000 Joule-0.9.9/joule/cli/admin/initialize.py
+drwxr-xr-x   0 jdonnal    (501) staff       (20)        0 2019-11-21 20:50:45.000000 Joule-0.9.9/joule/cli/admin/local_postgres_templates/
+-rw-r--r--   0 jdonnal    (501) staff       (20)       68 2019-07-24 01:06:55.000000 Joule-0.9.9/joule/cli/admin/local_postgres_templates/pg_hba.conf.jinja2
+-rw-r--r--   0 jdonnal    (501) staff       (20)        0 2019-07-18 00:42:32.000000 Joule-0.9.9/joule/cli/admin/local_postgres_templates/pg_ident.conf.jinja2
+-rw-r--r--   0 jdonnal    (501) staff       (20)     1874 2019-07-26 17:58:05.000000 Joule-0.9.9/joule/cli/admin/local_postgres_templates/postgresql.conf.jinja2
+-rw-r--r--   0 jdonnal    (501) staff       (20)      110 2019-07-20 21:13:28.000000 Joule-0.9.9/joule/cli/admin/local_postgres_templates/recovery.conf.jinja2
+-rw-r--r--   0 jdonnal    (501) staff       (20)      725 2019-06-28 19:28:13.000000 Joule-0.9.9/joule/cli/config.py
+drwxr-xr-x   0 jdonnal    (501) staff       (20)        0 2019-11-21 20:50:45.000000 Joule-0.9.9/joule/cli/data/
+-rw-r--r--   0 jdonnal    (501) staff       (20)      354 2019-05-09 14:20:06.000000 Joule-0.9.9/joule/cli/data/__init__.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)    14859 2019-09-11 15:34:37.000000 Joule-0.9.9/joule/cli/data/copy.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)     1529 2019-05-29 14:04:54.000000 Joule-0.9.9/joule/cli/data/intervals.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)     3077 2019-05-29 14:04:54.000000 Joule-0.9.9/joule/cli/data/read.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)     1561 2019-05-29 14:04:54.000000 Joule-0.9.9/joule/cli/data/remove.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)     1257 2019-05-29 14:04:54.000000 Joule-0.9.9/joule/cli/folder.py
+drwxr-xr-x   0 jdonnal    (501) staff       (20)        0 2019-11-21 20:50:45.000000 Joule-0.9.9/joule/cli/follower/
+-rw-r--r--   0 jdonnal    (501) staff       (20)      224 2019-05-09 14:20:06.000000 Joule-0.9.9/joule/cli/follower/__init__.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)      576 2019-05-29 14:04:54.000000 Joule-0.9.9/joule/cli/follower/delete.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)      781 2019-05-29 14:04:54.000000 Joule-0.9.9/joule/cli/follower/list.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)       86 2019-05-09 14:20:06.000000 Joule-0.9.9/joule/cli/helpers.py
+drwxr-xr-x   0 jdonnal    (501) staff       (20)        0 2019-11-21 20:50:45.000000 Joule-0.9.9/joule/cli/master/
+-rw-r--r--   0 jdonnal    (501) staff       (20)      259 2019-05-09 14:20:06.000000 Joule-0.9.9/joule/cli/master/__init__.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)     2940 2019-10-04 20:14:05.000000 Joule-0.9.9/joule/cli/master/add.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)      757 2019-05-29 14:04:54.000000 Joule-0.9.9/joule/cli/master/delete.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)     1315 2019-05-29 14:04:54.000000 Joule-0.9.9/joule/cli/master/list.py
+drwxr-xr-x   0 jdonnal    (501) staff       (20)        0 2019-11-21 20:50:45.000000 Joule-0.9.9/joule/cli/module/
+-rw-r--r--   0 jdonnal    (501) staff       (20)      256 2019-01-12 01:46:25.000000 Joule-0.9.9/joule/cli/module/__init__.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)     1647 2019-05-29 14:04:54.000000 Joule-0.9.9/joule/cli/module/info.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)     1621 2019-05-29 14:03:46.000000 Joule-0.9.9/joule/cli/module/list.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)      645 2019-05-29 14:04:54.000000 Joule-0.9.9/joule/cli/module/logs.py
+drwxr-xr-x   0 jdonnal    (501) staff       (20)        0 2019-11-21 20:50:45.000000 Joule-0.9.9/joule/cli/node/
+-rw-r--r--   0 jdonnal    (501) staff       (20)      376 2019-05-09 14:20:06.000000 Joule-0.9.9/joule/cli/node/__init__.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)      972 2019-08-03 18:52:44.000000 Joule-0.9.9/joule/cli/node/add.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)      351 2019-05-09 14:20:06.000000 Joule-0.9.9/joule/cli/node/default.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)      365 2019-05-09 14:20:06.000000 Joule-0.9.9/joule/cli/node/delete.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)      592 2019-05-29 14:04:54.000000 Joule-0.9.9/joule/cli/node/info.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)      836 2019-05-09 14:20:06.000000 Joule-0.9.9/joule/cli/node/list.py
+drwxr-xr-x   0 jdonnal    (501) staff       (20)        0 2019-11-21 20:50:45.000000 Joule-0.9.9/joule/cli/proxy/
+-rw-r--r--   0 jdonnal    (501) staff       (20)      202 2019-05-09 14:20:06.000000 Joule-0.9.9/joule/cli/proxy/__init__.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)      920 2019-05-29 14:04:54.000000 Joule-0.9.9/joule/cli/proxy/info.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)      909 2019-09-11 15:34:37.000000 Joule-0.9.9/joule/cli/proxy/list.py
+drwxr-xr-x   0 jdonnal    (501) staff       (20)        0 2019-11-21 20:50:45.000000 Joule-0.9.9/joule/cli/stream/
+-rw-r--r--   0 jdonnal    (501) staff       (20)      436 2019-06-28 18:41:11.000000 Joule-0.9.9/joule/cli/stream/__init__.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)     2413 2019-06-28 19:42:12.000000 Joule-0.9.9/joule/cli/stream/annotation.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)      674 2019-05-29 14:04:54.000000 Joule-0.9.9/joule/cli/stream/destroy.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)     3301 2019-05-29 14:04:54.000000 Joule-0.9.9/joule/cli/stream/info.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)     2309 2019-07-26 18:40:00.000000 Joule-0.9.9/joule/cli/stream/list.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)      635 2019-05-29 14:04:54.000000 Joule-0.9.9/joule/cli/stream/move.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)        0 2019-01-12 01:46:25.000000 Joule-0.9.9/joule/cli.py
+drwxr-xr-x   0 jdonnal    (501) staff       (20)        0 2019-11-21 20:50:45.000000 Joule-0.9.9/joule/client/
+-rw-r--r--   0 jdonnal    (501) staff       (20)      269 2019-01-12 01:45:31.000000 Joule-0.9.9/joule/client/__init__.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)    12998 2019-11-21 18:16:53.000000 Joule-0.9.9/joule/client/base_module.py
+drwxr-xr-x   0 jdonnal    (501) staff       (20)        0 2019-11-21 20:50:45.000000 Joule-0.9.9/joule/client/builtins/
+-rw-r--r--   0 jdonnal    (501) staff       (20)        0 2018-10-06 23:32:02.000000 Joule-0.9.9/joule/client/builtins/__init__.py
+drwxr-xr-x   0 jdonnal    (501) staff       (20)        0 2019-11-21 20:50:45.000000 Joule-0.9.9/joule/client/builtins/__pycache__/
+-rw-r--r--   0 jdonnal    (501) staff       (20)      127 2019-05-16 13:38:27.000000 Joule-0.9.9/joule/client/builtins/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0 jdonnal    (501) staff       (20)     2746 2019-07-24 20:23:35.000000 Joule-0.9.9/joule/client/builtins/__pycache__/file_reader.cpython-36.pyc
+-rw-r--r--   0 jdonnal    (501) staff       (20)     2383 2019-05-16 13:38:28.000000 Joule-0.9.9/joule/client/builtins/__pycache__/mean_filter.cpython-36.pyc
+-rw-r--r--   0 jdonnal    (501) staff       (20)     2926 2019-05-16 13:38:28.000000 Joule-0.9.9/joule/client/builtins/__pycache__/median_filter.cpython-36.pyc
+-rw-r--r--   0 jdonnal    (501) staff       (20)     2912 2019-05-16 13:38:28.000000 Joule-0.9.9/joule/client/builtins/__pycache__/random_reader.cpython-36.pyc
+-rw-r--r--   0 jdonnal    (501) staff       (20)     4706 2019-08-16 19:15:44.000000 Joule-0.9.9/joule/client/builtins/__pycache__/visualizer.cpython-36.pyc
+drwxr-xr-x   0 jdonnal    (501) staff       (20)        0 2019-11-21 20:50:45.000000 Joule-0.9.9/joule/client/builtins/assets/
+drwxr-xr-x   0 jdonnal    (501) staff       (20)        0 2019-11-21 20:50:45.000000 Joule-0.9.9/joule/client/builtins/assets/css/
+-rw-r--r--   0 jdonnal    (501) staff       (20)   140936 2019-01-12 01:45:31.000000 Joule-0.9.9/joule/client/builtins/assets/css/bootstrap.min.css
+-rw-r--r--   0 jdonnal    (501) staff       (20)   562427 2019-01-12 01:45:31.000000 Joule-0.9.9/joule/client/builtins/assets/css/bootstrap.min.css.map
+-rw-r--r--   0 jdonnal    (501) staff       (20)      646 2019-01-12 01:45:31.000000 Joule-0.9.9/joule/client/builtins/assets/css/index.css
+drwxr-xr-x   0 jdonnal    (501) staff       (20)        0 2019-11-21 20:50:45.000000 Joule-0.9.9/joule/client/builtins/assets/js/
+-rw-r--r--   0 jdonnal    (501) staff       (20)    70966 2019-01-12 01:45:31.000000 Joule-0.9.9/joule/client/builtins/assets/js/bootstrap.bundle.min.js
+-rw-r--r--   0 jdonnal    (501) staff       (20)   294126 2019-01-12 01:45:31.000000 Joule-0.9.9/joule/client/builtins/assets/js/bootstrap.bundle.min.js.map
+-rw-r--r--   0 jdonnal    (501) staff       (20)     1871 2019-08-27 13:06:55.000000 Joule-0.9.9/joule/client/builtins/assets/js/index.js
+-rw-r--r--   0 jdonnal    (501) staff       (20)    86927 2019-01-12 01:45:31.000000 Joule-0.9.9/joule/client/builtins/assets/js/jquery-3.3.1.min.js
+-rw-r--r--   0 jdonnal    (501) staff       (20)   132382 2019-01-12 01:45:31.000000 Joule-0.9.9/joule/client/builtins/assets/js/jquery-3.3.1.min.map
+-rw-r--r--   0 jdonnal    (501) staff       (20)    19188 2019-01-12 01:45:31.000000 Joule-0.9.9/joule/client/builtins/assets/js/popper.min.js
+-rw-r--r--   0 jdonnal    (501) staff       (20)   112587 2019-01-12 01:45:31.000000 Joule-0.9.9/joule/client/builtins/assets/js/popper.min.js.map
+drwxr-xr-x   0 jdonnal    (501) staff       (20)        0 2019-11-21 20:50:45.000000 Joule-0.9.9/joule/client/builtins/assets/templates/
+-rw-r--r--   0 jdonnal    (501) staff       (20)      737 2019-09-11 15:34:37.000000 Joule-0.9.9/joule/client/builtins/assets/templates/base.jinja2
+-rw-r--r--   0 jdonnal    (501) staff       (20)     3274 2019-08-16 19:06:21.000000 Joule-0.9.9/joule/client/builtins/assets/templates/index.jinja2
+-rw-r--r--   0 jdonnal    (501) staff       (20)     2556 2019-07-16 18:08:37.000000 Joule-0.9.9/joule/client/builtins/file_reader.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)     2041 2019-01-12 01:45:31.000000 Joule-0.9.9/joule/client/builtins/mean_filter.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)     3458 2019-02-06 03:28:37.000000 Joule-0.9.9/joule/client/builtins/median_filter.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)     3187 2019-01-12 01:45:31.000000 Joule-0.9.9/joule/client/builtins/random_reader.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)     4728 2019-09-11 15:34:37.000000 Joule-0.9.9/joule/client/builtins/visualizer.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)     1414 2019-09-11 15:34:37.000000 Joule-0.9.9/joule/client/composite_module.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)     1992 2019-09-11 15:34:37.000000 Joule-0.9.9/joule/client/filter_module.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)     2335 2019-02-06 02:58:41.000000 Joule-0.9.9/joule/client/fir_filter_module.py
+drwxr-xr-x   0 jdonnal    (501) staff       (20)        0 2019-11-21 20:50:45.000000 Joule-0.9.9/joule/client/helpers/
+-rw-r--r--   0 jdonnal    (501) staff       (20)      409 2019-10-02 01:19:37.000000 Joule-0.9.9/joule/client/helpers/__init__.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)     3452 2019-10-04 01:32:21.000000 Joule-0.9.9/joule/client/helpers/args.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)     7094 2019-10-04 18:22:25.000000 Joule-0.9.9/joule/client/helpers/pipes.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)     2853 2019-10-01 00:50:09.000000 Joule-0.9.9/joule/client/reader_module.py
+drwxr-xr-x   0 jdonnal    (501) staff       (20)        0 2019-11-21 20:50:45.000000 Joule-0.9.9/joule/controllers/
+-rw-r--r--   0 jdonnal    (501) staff       (20)     2724 2019-09-11 15:34:37.000000 Joule-0.9.9/joule/controllers/__init__.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)     5262 2019-07-03 00:41:10.000000 Joule-0.9.9/joule/controllers/annotation_controller.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)     1455 2019-09-11 15:34:37.000000 Joule-0.9.9/joule/controllers/app_controller.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)     9933 2019-03-01 01:35:57.000000 Joule-0.9.9/joule/controllers/data_controller.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)     6075 2019-07-03 17:48:25.000000 Joule-0.9.9/joule/controllers/folder_controller.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)     2626 2019-11-07 02:16:36.000000 Joule-0.9.9/joule/controllers/follower_controller.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)     7873 2019-10-04 20:16:58.000000 Joule-0.9.9/joule/controllers/master_controller.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)     2480 2019-05-15 21:39:02.000000 Joule-0.9.9/joule/controllers/module_controller.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)     1055 2019-05-09 14:20:06.000000 Joule-0.9.9/joule/controllers/proxy_controller.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)      772 2019-07-25 00:07:43.000000 Joule-0.9.9/joule/controllers/root_controller.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)     7042 2019-07-24 01:30:48.000000 Joule-0.9.9/joule/controllers/stream_controller.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)    13428 2019-11-21 18:07:31.000000 Joule-0.9.9/joule/daemon.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)      851 2019-08-13 00:05:57.000000 Joule-0.9.9/joule/errors.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)     2458 2019-11-18 21:06:53.000000 Joule-0.9.9/joule/middleware.py
+drwxr-xr-x   0 jdonnal    (501) staff       (20)        0 2019-11-21 20:50:45.000000 Joule-0.9.9/joule/models/
+-rw-r--r--   0 jdonnal    (501) staff       (20)      714 2019-06-20 18:24:19.000000 Joule-0.9.9/joule/models/__init__.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)     2288 2019-07-03 00:20:56.000000 Joule-0.9.9/joule/models/annotation.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)     1891 2019-09-11 15:34:37.000000 Joule-0.9.9/joule/models/config.py
+drwxr-xr-x   0 jdonnal    (501) staff       (20)        0 2019-11-21 20:50:45.000000 Joule-0.9.9/joule/models/data_store/
+-rw-r--r--   0 jdonnal    (501) staff       (20)      167 2019-01-12 01:45:31.000000 Joule-0.9.9/joule/models/data_store/__init__.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)     2863 2019-01-25 02:08:22.000000 Joule-0.9.9/joule/models/data_store/data_store.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)       94 2019-01-12 01:45:31.000000 Joule-0.9.9/joule/models/data_store/errors.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)    14472 2019-09-16 18:17:46.000000 Joule-0.9.9/joule/models/data_store/nilmdb.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)     1054 2019-01-25 02:08:22.000000 Joule-0.9.9/joule/models/data_store/nilmdb_helpers.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)    12945 2019-01-12 01:45:31.000000 Joule-0.9.9/joule/models/data_store/nilmdb_inserter.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)    11610 2019-07-30 01:05:34.000000 Joule-0.9.9/joule/models/data_store/psql_helpers.py
+drwxr-xr-x   0 jdonnal    (501) staff       (20)        0 2019-11-21 20:50:45.000000 Joule-0.9.9/joule/models/data_store/sql/
+-rw-r--r--   0 jdonnal    (501) staff       (20)     1473 2019-01-12 01:45:31.000000 Joule-0.9.9/joule/models/data_store/sql/info.sql
+-rw-r--r--   0 jdonnal    (501) staff       (20)     1374 2019-09-16 18:10:00.000000 Joule-0.9.9/joule/models/data_store/sql/row_count.sql
+-rw-r--r--   0 jdonnal    (501) staff       (20)    11847 2019-10-04 00:27:20.000000 Joule-0.9.9/joule/models/data_store/timescale.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)     8032 2019-10-04 00:29:49.000000 Joule-0.9.9/joule/models/data_store/timescale_inserter.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)     7683 2019-07-03 01:34:14.000000 Joule-0.9.9/joule/models/element.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)     4912 2019-05-09 14:20:06.000000 Joule-0.9.9/joule/models/folder.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)      979 2019-05-09 14:20:06.000000 Joule-0.9.9/joule/models/follower.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)     1290 2019-05-09 14:20:06.000000 Joule-0.9.9/joule/models/master.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)       83 2019-01-12 01:45:31.000000 Joule-0.9.9/joule/models/meta.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)     2946 2019-05-15 21:39:02.000000 Joule-0.9.9/joule/models/module.py
+drwxr-xr-x   0 jdonnal    (501) staff       (20)        0 2019-11-21 20:50:45.000000 Joule-0.9.9/joule/models/pipes/
+-rw-r--r--   0 jdonnal    (501) staff       (20)      382 2019-01-12 01:45:31.000000 Joule-0.9.9/joule/models/pipes/__init__.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)      219 2019-08-13 00:07:39.000000 Joule-0.9.9/joule/models/pipes/errors.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)      875 2019-01-12 01:45:31.000000 Joule-0.9.9/joule/models/pipes/factories.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)     5251 2019-03-02 18:35:49.000000 Joule-0.9.9/joule/models/pipes/input_pipe.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)     8719 2019-07-24 20:08:18.000000 Joule-0.9.9/joule/models/pipes/local_pipe.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)     3597 2019-11-07 02:16:36.000000 Joule-0.9.9/joule/models/pipes/output_pipe.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)     9313 2019-02-26 02:09:04.000000 Joule-0.9.9/joule/models/pipes/pipe.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)      283 2019-05-09 14:20:06.000000 Joule-0.9.9/joule/models/proxy.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)    11826 2019-07-03 01:31:42.000000 Joule-0.9.9/joule/models/stream.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)     7440 2019-09-11 15:34:37.000000 Joule-0.9.9/joule/models/supervisor.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)    16440 2019-10-03 20:43:18.000000 Joule-0.9.9/joule/models/worker.py
+drwxr-xr-x   0 jdonnal    (501) staff       (20)        0 2019-11-21 20:50:45.000000 Joule-0.9.9/joule/resources/
+-rw-r--r--   0 jdonnal    (501) staff       (20)      267 2019-05-09 14:20:06.000000 Joule-0.9.9/joule/resources/joule.service
+drwxr-xr-x   0 jdonnal    (501) staff       (20)        0 2019-11-21 20:50:45.000000 Joule-0.9.9/joule/resources/templates/
+-rw-r--r--   0 jdonnal    (501) staff       (20)     1766 2019-11-13 01:04:01.000000 Joule-0.9.9/joule/resources/templates/main.conf.jinja2
+-rw-r--r--   0 jdonnal    (501) staff       (20)      740 2019-02-20 14:21:11.000000 Joule-0.9.9/joule/resources/templates/module.example
+-rw-r--r--   0 jdonnal    (501) staff       (20)     1013 2019-02-20 13:10:26.000000 Joule-0.9.9/joule/resources/templates/stream.example
+drwxr-xr-x   0 jdonnal    (501) staff       (20)        0 2019-11-21 20:50:45.000000 Joule-0.9.9/joule/services/
+-rw-r--r--   0 jdonnal    (501) staff       (20)        0 2019-01-12 01:45:31.000000 Joule-0.9.9/joule/services/__init__.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)      804 2019-01-12 01:45:31.000000 Joule-0.9.9/joule/services/helpers.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)     6468 2019-09-11 21:04:01.000000 Joule-0.9.9/joule/services/load_config.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)     3142 2019-01-12 01:45:31.000000 Joule-0.9.9/joule/services/load_modules.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)     2436 2019-01-12 01:45:31.000000 Joule-0.9.9/joule/services/load_streams.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)     5056 2019-10-17 01:09:02.000000 Joule-0.9.9/joule/services/parse_pipe_config.py
+drwxr-xr-x   0 jdonnal    (501) staff       (20)        0 2019-11-21 20:50:45.000000 Joule-0.9.9/joule/utilities/
+-rw-r--r--   0 jdonnal    (501) staff       (20)      422 2019-07-24 23:58:30.000000 Joule-0.9.9/joule/utilities/__init__.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)     1755 2019-08-07 18:44:38.000000 Joule-0.9.9/joule/utilities/connection_info.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)     2578 2019-01-12 01:45:31.000000 Joule-0.9.9/joule/utilities/interval_tools.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)     1547 2019-07-03 16:23:28.000000 Joule-0.9.9/joule/utilities/misc.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)      426 2019-01-25 02:08:22.000000 Joule-0.9.9/joule/utilities/stream.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)     1985 2019-06-20 20:40:11.000000 Joule-0.9.9/joule/utilities/time.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)      200 2019-11-21 20:50:45.000000 Joule-0.9.9/setup.cfg
+-rw-r--r--   0 jdonnal    (501) staff       (20)     2439 2019-07-09 01:21:43.000000 Joule-0.9.9/setup.py
+-rw-r--r--   0 jdonnal    (501) staff       (20)    68611 2019-01-12 01:45:31.000000 Joule-0.9.9/versioneer.py
```

### Comparing `Joule-0.9.8/Joule.egg-info/PKG-INFO` & `Joule-0.9.9/Joule.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: Joule
-Version: 0.9.8
+Version: 0.9.9
 Summary: Decentralized data processing for IoT platforms
 Home-page: http://wattsworth.net/joule
 Author: John Donnal
 Author-email: donnal@usna.edu
 License: open source (see LICENSE)
 Download-URL: https://github.com/wattsworth/joule
 Description: .. image:: https://coveralls.io/repos/github/wattsworth/joule/badge.svg?branch=master
```

### Comparing `Joule-0.9.8/Joule.egg-info/SOURCES.txt` & `Joule-0.9.9/Joule.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/PKG-INFO` & `Joule-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: Joule
-Version: 0.9.8
+Version: 0.9.9
 Summary: Decentralized data processing for IoT platforms
 Home-page: http://wattsworth.net/joule
 Author: John Donnal
 Author-email: donnal@usna.edu
 License: open source (see LICENSE)
 Download-URL: https://github.com/wattsworth/joule
 Description: .. image:: https://coveralls.io/repos/github/wattsworth/joule/badge.svg?branch=master
```

### Comparing `Joule-0.9.8/README.rst` & `Joule-0.9.9/README.rst`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/api/annotation.py` & `Joule-0.9.9/joule/api/annotation.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/api/data.py` & `Joule-0.9.9/joule/api/data.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/api/db.py` & `Joule-0.9.9/joule/api/db.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/api/folder.py` & `Joule-0.9.9/joule/api/folder.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/api/folder_type.py` & `Joule-0.9.9/joule/api/folder_type.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/api/helpers.py` & `Joule-0.9.9/joule/api/helpers.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/api/master.py` & `Joule-0.9.9/joule/api/master.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/api/module.py` & `Joule-0.9.9/joule/api/module.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/api/node/base_node.py` & `Joule-0.9.9/joule/api/node/base_node.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/api/node/tcp_node.py` & `Joule-0.9.9/joule/api/node/tcp_node.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/api/node/unix_node.py` & `Joule-0.9.9/joule/api/node/unix_node.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/api/proxy.py` & `Joule-0.9.9/joule/api/proxy.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/api/session/base_session.py` & `Joule-0.9.9/joule/api/session/base_session.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/api/session/tcp_session.py` & `Joule-0.9.9/joule/api/session/tcp_session.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/api/session/unix_session.py` & `Joule-0.9.9/joule/api/session/unix_session.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/api/stream.py` & `Joule-0.9.9/joule/api/stream.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/cli/__init__.py` & `Joule-0.9.9/joule/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/cli/admin/authorize.py` & `Joule-0.9.9/joule/cli/admin/authorize.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/cli/admin/backup.py` & `Joule-0.9.9/joule/cli/admin/backup.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/cli/admin/erase.py` & `Joule-0.9.9/joule/cli/admin/erase.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/cli/admin/ingest.py` & `Joule-0.9.9/joule/cli/admin/ingest.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/cli/admin/initialize.py` & `Joule-0.9.9/joule/cli/admin/initialize.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/cli/admin/local_postgres_templates/postgresql.conf.jinja2` & `Joule-0.9.9/joule/cli/admin/local_postgres_templates/postgresql.conf.jinja2`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/cli/config.py` & `Joule-0.9.9/joule/cli/config.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/cli/data/copy.py` & `Joule-0.9.9/joule/cli/data/copy.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/cli/data/intervals.py` & `Joule-0.9.9/joule/cli/data/intervals.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/cli/data/read.py` & `Joule-0.9.9/joule/cli/data/read.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/cli/data/remove.py` & `Joule-0.9.9/joule/cli/data/remove.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/cli/folder.py` & `Joule-0.9.9/joule/cli/folder.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/cli/follower/delete.py` & `Joule-0.9.9/joule/cli/follower/delete.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/cli/follower/list.py` & `Joule-0.9.9/joule/cli/follower/list.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/cli/master/add.py` & `Joule-0.9.9/joule/cli/master/add.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/cli/master/delete.py` & `Joule-0.9.9/joule/cli/master/delete.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/cli/master/list.py` & `Joule-0.9.9/joule/cli/master/list.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/cli/module/info.py` & `Joule-0.9.9/joule/cli/module/info.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/cli/module/list.py` & `Joule-0.9.9/joule/cli/module/list.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/cli/module/logs.py` & `Joule-0.9.9/joule/cli/module/logs.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/cli/node/add.py` & `Joule-0.9.9/joule/cli/node/add.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/cli/node/info.py` & `Joule-0.9.9/joule/cli/node/info.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/cli/node/list.py` & `Joule-0.9.9/joule/cli/node/list.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/cli/proxy/info.py` & `Joule-0.9.9/joule/cli/proxy/info.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/cli/proxy/list.py` & `Joule-0.9.9/joule/cli/proxy/list.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/cli/stream/annotation.py` & `Joule-0.9.9/joule/cli/stream/annotation.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/cli/stream/destroy.py` & `Joule-0.9.9/joule/cli/stream/destroy.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/cli/stream/info.py` & `Joule-0.9.9/joule/cli/stream/info.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/cli/stream/list.py` & `Joule-0.9.9/joule/cli/stream/list.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/cli/stream/move.py` & `Joule-0.9.9/joule/cli/stream/move.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/client/base_module.py` & `Joule-0.9.9/joule/client/base_module.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,15 +127,15 @@
 
         if parsed_args is None:  # pragma: no cover
             parser = argparse.ArgumentParser()
             self._build_args(parser)
             module_args = helpers.module_args()
             parsed_args = parser.parse_args(module_args)
 
-        asyncio.set_event_loop_policy(uvloop.EventLoopPolicy())
+        #asyncio.set_event_loop_policy(uvloop.EventLoopPolicy())
         loop = asyncio.get_event_loop()
         self.stop_requested = False
         if parsed_args.api_socket != "unset":
             # should be set by the joule daemon
             if 'JOULE_CA_FILE' in os.environ:
                 cafile = os.environ['JOULE_CA_FILE']
             else:
```

### Comparing `Joule-0.9.8/joule/client/builtins/__pycache__/file_reader.cpython-36.pyc` & `Joule-0.9.9/joule/client/builtins/__pycache__/file_reader.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/client/builtins/__pycache__/mean_filter.cpython-36.pyc` & `Joule-0.9.9/joule/client/builtins/__pycache__/mean_filter.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/client/builtins/__pycache__/median_filter.cpython-36.pyc` & `Joule-0.9.9/joule/client/builtins/__pycache__/median_filter.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/client/builtins/__pycache__/random_reader.cpython-36.pyc` & `Joule-0.9.9/joule/client/builtins/__pycache__/random_reader.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/client/builtins/__pycache__/visualizer.cpython-36.pyc` & `Joule-0.9.9/joule/client/builtins/__pycache__/visualizer.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/client/builtins/assets/css/bootstrap.min.css` & `Joule-0.9.9/joule/client/builtins/assets/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/client/builtins/assets/css/bootstrap.min.css.map` & `Joule-0.9.9/joule/client/builtins/assets/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/client/builtins/assets/css/index.css` & `Joule-0.9.9/joule/client/builtins/assets/css/index.css`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/client/builtins/assets/js/bootstrap.bundle.min.js` & `Joule-0.9.9/joule/client/builtins/assets/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/client/builtins/assets/js/bootstrap.bundle.min.js.map` & `Joule-0.9.9/joule/client/builtins/assets/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/client/builtins/assets/js/index.js` & `Joule-0.9.9/joule/client/builtins/assets/js/index.js`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/client/builtins/assets/js/jquery-3.3.1.min.js` & `Joule-0.9.9/joule/client/builtins/assets/js/jquery-3.3.1.min.js`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/client/builtins/assets/js/jquery-3.3.1.min.map` & `Joule-0.9.9/joule/client/builtins/assets/js/jquery-3.3.1.min.map`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/client/builtins/assets/js/popper.min.js` & `Joule-0.9.9/joule/client/builtins/assets/js/popper.min.js`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/client/builtins/assets/js/popper.min.js.map` & `Joule-0.9.9/joule/client/builtins/assets/js/popper.min.js.map`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/client/builtins/assets/templates/base.jinja2` & `Joule-0.9.9/joule/client/builtins/assets/templates/base.jinja2`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/client/builtins/assets/templates/index.jinja2` & `Joule-0.9.9/joule/client/builtins/assets/templates/index.jinja2`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/client/builtins/file_reader.py` & `Joule-0.9.9/joule/client/builtins/file_reader.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/client/builtins/mean_filter.py` & `Joule-0.9.9/joule/client/builtins/mean_filter.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/client/builtins/median_filter.py` & `Joule-0.9.9/joule/client/builtins/median_filter.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/client/builtins/random_reader.py` & `Joule-0.9.9/joule/client/builtins/random_reader.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/client/builtins/visualizer.py` & `Joule-0.9.9/joule/client/builtins/visualizer.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/client/composite_module.py` & `Joule-0.9.9/joule/client/composite_module.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/client/filter_module.py` & `Joule-0.9.9/joule/client/filter_module.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/client/fir_filter_module.py` & `Joule-0.9.9/joule/client/fir_filter_module.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/client/helpers/args.py` & `Joule-0.9.9/joule/client/helpers/args.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/client/helpers/pipes.py` & `Joule-0.9.9/joule/client/helpers/pipes.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/client/reader_module.py` & `Joule-0.9.9/joule/client/reader_module.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/controllers/__init__.py` & `Joule-0.9.9/joule/controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/controllers/annotation_controller.py` & `Joule-0.9.9/joule/controllers/annotation_controller.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/controllers/app_controller.py` & `Joule-0.9.9/joule/controllers/app_controller.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/controllers/data_controller.py` & `Joule-0.9.9/joule/controllers/data_controller.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/controllers/folder_controller.py` & `Joule-0.9.9/joule/controllers/folder_controller.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/controllers/follower_controller.py` & `Joule-0.9.9/joule/controllers/follower_controller.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/controllers/master_controller.py` & `Joule-0.9.9/joule/controllers/master_controller.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/controllers/module_controller.py` & `Joule-0.9.9/joule/controllers/module_controller.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/controllers/proxy_controller.py` & `Joule-0.9.9/joule/controllers/proxy_controller.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/controllers/root_controller.py` & `Joule-0.9.9/joule/controllers/root_controller.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/controllers/stream_controller.py` & `Joule-0.9.9/joule/controllers/stream_controller.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/daemon.py` & `Joule-0.9.9/joule/daemon.py`

 * *Files 0% similar despite different names*

```diff
@@ -290,15 +290,15 @@
         log.error("Invalid configuration: %s" % e)
         exit(1)
 
     # uvloop uses libuv which does not support
     # connections to abstract namespace sockets
     # https://github.com/joyent/libuv/issues/1486
 
-    asyncio.set_event_loop_policy(uvloop.EventLoopPolicy())
+    #asyncio.set_event_loop_policy(uvloop.EventLoopPolicy())
 
     loop = asyncio.get_event_loop()
     loop.set_debug(True)
     daemon = Daemon(my_config)
     try:
         daemon.initialize(loop)
     except SQLAlchemyError as e:
```

### Comparing `Joule-0.9.8/joule/errors.py` & `Joule-0.9.9/joule/errors.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/middleware.py` & `Joule-0.9.9/joule/middleware.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/models/__init__.py` & `Joule-0.9.9/joule/models/__init__.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/models/annotation.py` & `Joule-0.9.9/joule/models/annotation.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/models/config.py` & `Joule-0.9.9/joule/models/config.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/models/data_store/data_store.py` & `Joule-0.9.9/joule/models/data_store/data_store.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/models/data_store/nilmdb.py` & `Joule-0.9.9/joule/models/data_store/nilmdb.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/models/data_store/nilmdb_helpers.py` & `Joule-0.9.9/joule/models/data_store/nilmdb_helpers.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/models/data_store/nilmdb_inserter.py` & `Joule-0.9.9/joule/models/data_store/nilmdb_inserter.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/models/data_store/psql_helpers.py` & `Joule-0.9.9/joule/models/data_store/psql_helpers.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/models/data_store/sql/info.sql` & `Joule-0.9.9/joule/models/data_store/sql/info.sql`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/models/data_store/sql/row_count.sql` & `Joule-0.9.9/joule/models/data_store/sql/row_count.sql`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/models/data_store/timescale.py` & `Joule-0.9.9/joule/models/data_store/timescale.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/models/data_store/timescale_inserter.py` & `Joule-0.9.9/joule/models/data_store/timescale_inserter.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/models/element.py` & `Joule-0.9.9/joule/models/element.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/models/folder.py` & `Joule-0.9.9/joule/models/folder.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/models/follower.py` & `Joule-0.9.9/joule/models/follower.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/models/master.py` & `Joule-0.9.9/joule/models/master.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/models/module.py` & `Joule-0.9.9/joule/models/module.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/models/pipes/factories.py` & `Joule-0.9.9/joule/models/pipes/factories.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/models/pipes/input_pipe.py` & `Joule-0.9.9/joule/models/pipes/input_pipe.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/models/pipes/local_pipe.py` & `Joule-0.9.9/joule/models/pipes/local_pipe.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/models/pipes/output_pipe.py` & `Joule-0.9.9/joule/models/pipes/output_pipe.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/models/pipes/pipe.py` & `Joule-0.9.9/joule/models/pipes/pipe.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/models/stream.py` & `Joule-0.9.9/joule/models/stream.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/models/supervisor.py` & `Joule-0.9.9/joule/models/supervisor.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/models/worker.py` & `Joule-0.9.9/joule/models/worker.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/resources/templates/main.conf.jinja2` & `Joule-0.9.9/joule/resources/templates/main.conf.jinja2`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/resources/templates/module.example` & `Joule-0.9.9/joule/resources/templates/module.example`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/resources/templates/stream.example` & `Joule-0.9.9/joule/resources/templates/stream.example`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/services/helpers.py` & `Joule-0.9.9/joule/services/helpers.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/services/load_config.py` & `Joule-0.9.9/joule/services/load_config.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/services/load_modules.py` & `Joule-0.9.9/joule/services/load_modules.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/services/load_streams.py` & `Joule-0.9.9/joule/services/load_streams.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/services/parse_pipe_config.py` & `Joule-0.9.9/joule/services/parse_pipe_config.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/utilities/connection_info.py` & `Joule-0.9.9/joule/utilities/connection_info.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/utilities/interval_tools.py` & `Joule-0.9.9/joule/utilities/interval_tools.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/utilities/misc.py` & `Joule-0.9.9/joule/utilities/misc.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/joule/utilities/time.py` & `Joule-0.9.9/joule/utilities/time.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/setup.py` & `Joule-0.9.9/setup.py`

 * *Files identical despite different names*

### Comparing `Joule-0.9.8/versioneer.py` & `Joule-0.9.9/versioneer.py`

 * *Files identical despite different names*

