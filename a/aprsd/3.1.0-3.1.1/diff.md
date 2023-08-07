# Comparing `tmp/aprsd-3.1.0.tar.gz` & `tmp/aprsd-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aprsd-3.1.0.tar", last modified: Mon Jul 24 15:27:34 2023, max compression
+gzip compressed data, was "aprsd-3.1.1.tar", last modified: Mon Aug  7 16:01:55 2023, max compression
```

## Comparing `aprsd-3.1.0.tar` & `aprsd-3.1.1.tar`

### file list

```diff
@@ -1,234 +1,234 @@
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:34.308052 aprsd-3.1.0/
--rw-r--r--   0 i530566    (501) staff       (20)      269 2021-08-30 17:18:20.000000 aprsd-3.1.0/.coveragerc
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:33.284960 aprsd-3.1.0/.github/
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:33.429268 aprsd-3.1.0/.github/workflows/
--rw-r--r--   0 i530566    (501) staff       (20)     1461 2023-07-18 00:59:03.000000 aprsd-3.1.0/.github/workflows/manual_build.yml
--rw-r--r--   0 i530566    (501) staff       (20)     1629 2023-07-20 18:34:31.000000 aprsd-3.1.0/.github/workflows/master-build.yml
--rw-r--r--   0 i530566    (501) staff       (20)      523 2023-06-22 11:55:10.000000 aprsd-3.1.0/.github/workflows/python.yml
--rw-r--r--   0 i530566    (501) staff       (20)     1270 2023-07-20 19:10:23.000000 aprsd-3.1.0/.github/workflows/release_build.yml
--rw-r--r--   0 i530566    (501) staff       (20)      536 2021-08-30 17:18:20.000000 aprsd-3.1.0/.pre-commit-config.yaml
--rw-r--r--   0 i530566    (501) staff       (20)      574 2023-06-14 13:31:16.000000 aprsd-3.1.0/.readthedocs.yaml
--rw-r--r--   0 i530566    (501) staff       (20)      430 2023-07-24 15:26:54.000000 aprsd-3.1.0/AUTHORS
--rw-r--r--   0 i530566    (501) staff       (20)    22689 2023-07-24 15:26:54.000000 aprsd-3.1.0/ChangeLog
--rw-r--r--   0 i530566    (501) staff       (20)      753 2021-08-13 16:31:50.000000 aprsd-3.1.0/INSTALL.txt
--rw-r--r--   0 i530566    (501) staff       (20)    10142 2021-08-13 16:31:50.000000 aprsd-3.1.0/LICENSE
--rw-r--r--   0 i530566    (501) staff       (20)       94 2021-08-13 16:31:50.000000 aprsd-3.1.0/MANIFEST.in
--rw-r--r--   0 i530566    (501) staff       (20)     2737 2023-07-08 18:22:21.000000 aprsd-3.1.0/Makefile
--rw-r--r--   0 i530566    (501) staff       (20)    21221 2023-07-24 15:27:34.309527 aprsd-3.1.0/PKG-INFO
--rw-r--r--   0 i530566    (501) staff       (20)    20387 2023-07-16 20:28:02.000000 aprsd-3.1.0/README.rst
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:33.513219 aprsd-3.1.0/aprsd/
--rw-r--r--   0 i530566    (501) staff       (20)      631 2022-12-12 18:34:05.000000 aprsd-3.1.0/aprsd/__init__.py
--rw-r--r--   0 i530566    (501) staff       (20)    10517 2023-07-18 17:07:59.000000 aprsd-3.1.0/aprsd/admin_web.py
--rw-r--r--   0 i530566    (501) staff       (20)     3208 2023-07-16 20:28:22.000000 aprsd-3.1.0/aprsd/cli_helper.py
--rw-r--r--   0 i530566    (501) staff       (20)     8776 2023-07-20 19:10:23.000000 aprsd-3.1.0/aprsd/client.py
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:33.572345 aprsd-3.1.0/aprsd/clients/
--rw-r--r--   0 i530566    (501) staff       (20)        0 2022-12-12 18:34:06.000000 aprsd-3.1.0/aprsd/clients/__init__.py
--rw-r--r--   0 i530566    (501) staff       (20)     7207 2023-07-20 19:10:23.000000 aprsd-3.1.0/aprsd/clients/aprsis.py
--rw-r--r--   0 i530566    (501) staff       (20)     3413 2023-01-19 19:14:47.000000 aprsd-3.1.0/aprsd/clients/kiss.py
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:33.610912 aprsd-3.1.0/aprsd/cmds/
--rw-r--r--   0 i530566    (501) staff       (20)        0 2022-12-12 18:34:05.000000 aprsd-3.1.0/aprsd/cmds/__init__.py
--rw-r--r--   0 i530566    (501) staff       (20)     1763 2023-07-08 21:30:26.000000 aprsd-3.1.0/aprsd/cmds/completion.py
--rw-r--r--   0 i530566    (501) staff       (20)     3074 2023-07-08 21:30:26.000000 aprsd-3.1.0/aprsd/cmds/dev.py
--rw-r--r--   0 i530566    (501) staff       (20)     5348 2023-07-22 21:05:15.000000 aprsd-3.1.0/aprsd/cmds/fetch_stats.py
--rw-r--r--   0 i530566    (501) staff       (20)     2801 2023-07-16 20:28:22.000000 aprsd-3.1.0/aprsd/cmds/healthcheck.py
--rw-r--r--   0 i530566    (501) staff       (20)     7920 2023-07-08 21:30:27.000000 aprsd-3.1.0/aprsd/cmds/list_plugins.py
--rw-r--r--   0 i530566    (501) staff       (20)     6241 2023-07-16 20:28:22.000000 aprsd-3.1.0/aprsd/cmds/listen.py
--rw-r--r--   0 i530566    (501) staff       (20)     4716 2023-07-08 21:30:26.000000 aprsd-3.1.0/aprsd/cmds/send_message.py
--rw-r--r--   0 i530566    (501) staff       (20)     3416 2023-07-08 21:30:26.000000 aprsd-3.1.0/aprsd/cmds/server.py
--rw-r--r--   0 i530566    (501) staff       (20)    13478 2023-07-23 23:19:27.000000 aprsd-3.1.0/aprsd/cmds/webchat.py
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:33.633954 aprsd-3.1.0/aprsd/conf/
--rw-r--r--   0 i530566    (501) staff       (20)     1725 2023-07-16 20:28:21.000000 aprsd-3.1.0/aprsd/conf/__init__.py
--rw-r--r--   0 i530566    (501) staff       (20)     2349 2023-07-16 20:28:22.000000 aprsd-3.1.0/aprsd/conf/client.py
--rw-r--r--   0 i530566    (501) staff       (20)     4863 2023-01-19 19:14:47.000000 aprsd-3.1.0/aprsd/conf/common.py
--rw-r--r--   0 i530566    (501) staff       (20)     1379 2023-07-16 20:28:22.000000 aprsd-3.1.0/aprsd/conf/log.py
--rw-r--r--   0 i530566    (501) staff       (20)     2701 2022-12-29 19:14:43.000000 aprsd-3.1.0/aprsd/conf/opts.py
--rw-r--r--   0 i530566    (501) staff       (20)     2308 2022-12-29 19:14:43.000000 aprsd-3.1.0/aprsd/conf/plugin_common.py
--rw-r--r--   0 i530566    (501) staff       (20)     2332 2022-12-29 19:16:10.000000 aprsd-3.1.0/aprsd/conf/plugin_email.py
--rw-r--r--   0 i530566    (501) staff       (20)      502 2022-12-12 18:34:08.000000 aprsd-3.1.0/aprsd/exception.py
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:33.662518 aprsd-3.1.0/aprsd/log/
--rw-r--r--   0 i530566    (501) staff       (20)        0 2023-07-16 20:28:22.000000 aprsd-3.1.0/aprsd/log/__init__.py
--rw-r--r--   0 i530566    (501) staff       (20)     2678 2023-07-16 20:28:22.000000 aprsd-3.1.0/aprsd/log/log.py
--rw-r--r--   0 i530566    (501) staff       (20)     5545 2023-07-16 20:28:22.000000 aprsd-3.1.0/aprsd/log/rich.py
--rw-r--r--   0 i530566    (501) staff       (20)     4571 2023-07-16 20:28:22.000000 aprsd-3.1.0/aprsd/main.py
--rw-r--r--   0 i530566    (501) staff       (20)      134 2022-12-20 22:38:48.000000 aprsd-3.1.0/aprsd/messaging.py
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:33.673148 aprsd-3.1.0/aprsd/packets/
--rw-r--r--   0 i530566    (501) staff       (20)      432 2023-01-16 16:38:59.000000 aprsd-3.1.0/aprsd/packets/__init__.py
--rw-r--r--   0 i530566    (501) staff       (20)    18801 2023-07-14 15:35:51.000000 aprsd-3.1.0/aprsd/packets/core.py
--rw-r--r--   0 i530566    (501) staff       (20)     1457 2022-12-29 19:14:43.000000 aprsd-3.1.0/aprsd/packets/packet_list.py
--rw-r--r--   0 i530566    (501) staff       (20)     1071 2022-12-29 19:14:43.000000 aprsd-3.1.0/aprsd/packets/seen_list.py
--rw-r--r--   0 i530566    (501) staff       (20)     3205 2022-12-29 19:14:43.000000 aprsd-3.1.0/aprsd/packets/tracker.py
--rw-r--r--   0 i530566    (501) staff       (20)     2880 2022-12-29 19:14:43.000000 aprsd-3.1.0/aprsd/packets/watch_list.py
--rw-r--r--   0 i530566    (501) staff       (20)    16435 2023-04-25 18:29:36.000000 aprsd-3.1.0/aprsd/plugin.py
--rw-r--r--   0 i530566    (501) staff       (20)     2458 2023-04-07 15:21:31.000000 aprsd-3.1.0/aprsd/plugin_utils.py
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:33.730992 aprsd-3.1.0/aprsd/plugins/
--rw-r--r--   0 i530566    (501) staff       (20)        0 2022-12-12 18:34:08.000000 aprsd-3.1.0/aprsd/plugins/__init__.py
--rw-r--r--   0 i530566    (501) staff       (20)    23073 2023-07-16 20:28:22.000000 aprsd-3.1.0/aprsd/plugins/email.py
--rw-r--r--   0 i530566    (501) staff       (20)     1463 2022-12-29 19:18:51.000000 aprsd-3.1.0/aprsd/plugins/fortune.py
--rw-r--r--   0 i530566    (501) staff       (20)     3287 2023-07-10 15:01:50.000000 aprsd-3.1.0/aprsd/plugins/location.py
--rw-r--r--   0 i530566    (501) staff       (20)     1969 2022-12-29 19:14:43.000000 aprsd-3.1.0/aprsd/plugins/notify.py
--rw-r--r--   0 i530566    (501) staff       (20)      763 2022-12-29 19:18:50.000000 aprsd-3.1.0/aprsd/plugins/ping.py
--rw-r--r--   0 i530566    (501) staff       (20)     2458 2022-12-29 19:14:43.000000 aprsd-3.1.0/aprsd/plugins/query.py
--rw-r--r--   0 i530566    (501) staff       (20)     3496 2022-12-29 19:18:51.000000 aprsd-3.1.0/aprsd/plugins/time.py
--rw-r--r--   0 i530566    (501) staff       (20)      849 2022-12-29 19:18:51.000000 aprsd-3.1.0/aprsd/plugins/version.py
--rw-r--r--   0 i530566    (501) staff       (20)    13034 2023-07-15 22:22:29.000000 aprsd-3.1.0/aprsd/plugins/weather.py
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:33.772094 aprsd-3.1.0/aprsd/rpc/
--rw-r--r--   0 i530566    (501) staff       (20)      343 2022-12-31 21:45:32.000000 aprsd-3.1.0/aprsd/rpc/__init__.py
--rw-r--r--   0 i530566    (501) staff       (20)     4641 2023-07-23 23:46:10.000000 aprsd-3.1.0/aprsd/rpc/client.py
--rw-r--r--   0 i530566    (501) staff       (20)     2760 2023-07-20 20:43:39.000000 aprsd-3.1.0/aprsd/rpc/server.py
--rw-r--r--   0 i530566    (501) staff       (20)     7177 2023-07-10 14:44:27.000000 aprsd-3.1.0/aprsd/stats.py
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:33.816413 aprsd-3.1.0/aprsd/threads/
--rw-r--r--   0 i530566    (501) staff       (20)      274 2022-12-20 22:38:48.000000 aprsd-3.1.0/aprsd/threads/__init__.py
--rw-r--r--   0 i530566    (501) staff       (20)     2270 2023-07-20 19:10:23.000000 aprsd-3.1.0/aprsd/threads/aprsd.py
--rw-r--r--   0 i530566    (501) staff       (20)     3921 2023-07-20 19:10:23.000000 aprsd-3.1.0/aprsd/threads/keep_alive.py
--rw-r--r--   0 i530566    (501) staff       (20)     2036 2023-07-16 20:28:22.000000 aprsd-3.1.0/aprsd/threads/log_monitor.py
--rw-r--r--   0 i530566    (501) staff       (20)    10431 2023-07-20 18:38:55.000000 aprsd-3.1.0/aprsd/threads/rx.py
--rw-r--r--   0 i530566    (501) staff       (20)     6437 2023-07-08 21:30:27.000000 aprsd-3.1.0/aprsd/threads/tx.py
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:33.877028 aprsd-3.1.0/aprsd/utils/
--rw-r--r--   0 i530566    (501) staff       (20)     3532 2022-12-16 13:25:52.000000 aprsd-3.1.0/aprsd/utils/__init__.py
--rw-r--r--   0 i530566    (501) staff       (20)     1151 2022-12-20 22:38:48.000000 aprsd-3.1.0/aprsd/utils/counter.py
--rw-r--r--   0 i530566    (501) staff       (20)     3265 2022-12-12 18:34:08.000000 aprsd-3.1.0/aprsd/utils/fuzzyclock.py
--rw-r--r--   0 i530566    (501) staff       (20)     1871 2022-12-20 22:38:48.000000 aprsd-3.1.0/aprsd/utils/json.py
--rw-r--r--   0 i530566    (501) staff       (20)     3200 2022-12-29 19:14:44.000000 aprsd-3.1.0/aprsd/utils/objectstore.py
--rw-r--r--   0 i530566    (501) staff       (20)     1111 2022-12-20 22:38:48.000000 aprsd-3.1.0/aprsd/utils/ring_buffer.py
--rw-r--r--   0 i530566    (501) staff       (20)     5558 2022-12-12 18:34:08.000000 aprsd-3.1.0/aprsd/utils/trace.py
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:33.879119 aprsd-3.1.0/aprsd/web/
--rw-r--r--   0 i530566    (501) staff       (20)        0 2022-12-12 18:34:05.000000 aprsd-3.1.0/aprsd/web/__init__.py
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:33.881149 aprsd-3.1.0/aprsd/web/admin/
--rw-r--r--   0 i530566    (501) staff       (20)        0 2022-12-12 18:34:05.000000 aprsd-3.1.0/aprsd/web/admin/__init__.py
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:33.314036 aprsd-3.1.0/aprsd/web/admin/static/
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:33.907620 aprsd-3.1.0/aprsd/web/admin/static/css/
--rw-r--r--   0 i530566    (501) staff       (20)     1282 2022-11-23 18:33:33.000000 aprsd-3.1.0/aprsd/web/admin/static/css/index.css
--rw-r--r--   0 i530566    (501) staff       (20)     3467 2022-11-23 18:33:33.000000 aprsd-3.1.0/aprsd/web/admin/static/css/prism.css
--rw-r--r--   0 i530566    (501) staff       (20)      644 2022-11-23 18:33:33.000000 aprsd-3.1.0/aprsd/web/admin/static/css/tabs.css
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:33.928268 aprsd-3.1.0/aprsd/web/admin/static/images/
--rw-r--r--   0 i530566    (501) staff       (20)    37797 2022-11-23 18:33:33.000000 aprsd-3.1.0/aprsd/web/admin/static/images/Untitled.png
--rw-r--r--   0 i530566    (501) staff       (20)    52962 2022-11-23 18:33:33.000000 aprsd-3.1.0/aprsd/web/admin/static/images/aprs-symbols-16-0.png
--rw-r--r--   0 i530566    (501) staff       (20)    48951 2022-11-23 18:33:33.000000 aprsd-3.1.0/aprsd/web/admin/static/images/aprs-symbols-16-1.png
--rw-r--r--   0 i530566    (501) staff       (20)    52962 2022-11-23 18:33:33.000000 aprsd-3.1.0/aprsd/web/admin/static/images/aprs-symbols-64-0.png
--rw-r--r--   0 i530566    (501) staff       (20)    48951 2022-11-23 18:33:33.000000 aprsd-3.1.0/aprsd/web/admin/static/images/aprs-symbols-64-1.png
--rw-r--r--   0 i530566    (501) staff       (20)    40716 2022-11-23 18:33:33.000000 aprsd-3.1.0/aprsd/web/admin/static/images/aprs-symbols-64-2.png
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:33.962973 aprsd-3.1.0/aprsd/web/admin/static/js/
--rw-r--r--   0 i530566    (501) staff       (20)     7360 2022-12-20 22:38:48.000000 aprsd-3.1.0/aprsd/web/admin/static/js/charts.js
--rw-r--r--   0 i530566    (501) staff       (20)      658 2023-07-23 01:28:13.000000 aprsd-3.1.0/aprsd/web/admin/static/js/logs.js
--rw-r--r--   0 i530566    (501) staff       (20)     6796 2022-12-29 19:14:44.000000 aprsd-3.1.0/aprsd/web/admin/static/js/main.js
--rw-r--r--   0 i530566    (501) staff       (20)    64705 2022-11-23 18:33:33.000000 aprsd-3.1.0/aprsd/web/admin/static/js/prism.js
--rw-r--r--   0 i530566    (501) staff       (20)     3852 2022-12-29 19:14:44.000000 aprsd-3.1.0/aprsd/web/admin/static/js/send-message.js
--rw-r--r--   0 i530566    (501) staff       (20)      889 2022-11-23 18:33:33.000000 aprsd-3.1.0/aprsd/web/admin/static/js/tabs.js
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:34.005749 aprsd-3.1.0/aprsd/web/admin/static/json-viewer/
--rw-r--r--   0 i530566    (501) staff       (20)     1080 2022-11-23 18:33:33.000000 aprsd-3.1.0/aprsd/web/admin/static/json-viewer/jquery.json-viewer.css
--rw-r--r--   0 i530566    (501) staff       (20)     5020 2022-11-23 18:33:33.000000 aprsd-3.1.0/aprsd/web/admin/static/json-viewer/jquery.json-viewer.js
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:34.007162 aprsd-3.1.0/aprsd/web/admin/templates/
--rw-r--r--   0 i530566    (501) staff       (20)     8034 2023-07-23 23:46:10.000000 aprsd-3.1.0/aprsd/web/admin/templates/index.html
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:33.318699 aprsd-3.1.0/aprsd/web/chat/
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:33.318180 aprsd-3.1.0/aprsd/web/chat/static/
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:34.016733 aprsd-3.1.0/aprsd/web/chat/static/css/
--rw-r--r--   0 i530566    (501) staff       (20)     1376 2022-11-23 18:33:33.000000 aprsd-3.1.0/aprsd/web/chat/static/css/index.css
--rw-r--r--   0 i530566    (501) staff       (20)   174659 2022-11-23 18:33:33.000000 aprsd-3.1.0/aprsd/web/chat/static/css/style.css.map
--rw-r--r--   0 i530566    (501) staff       (20)      718 2022-11-23 18:33:33.000000 aprsd-3.1.0/aprsd/web/chat/static/css/tabs.css
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:34.037680 aprsd-3.1.0/aprsd/web/chat/static/images/
--rw-r--r--   0 i530566    (501) staff       (20)    37797 2022-11-23 18:33:33.000000 aprsd-3.1.0/aprsd/web/chat/static/images/Untitled.png
--rw-r--r--   0 i530566    (501) staff       (20)    52962 2022-11-23 18:33:33.000000 aprsd-3.1.0/aprsd/web/chat/static/images/aprs-symbols-16-0.png
--rw-r--r--   0 i530566    (501) staff       (20)    48951 2022-11-23 18:33:33.000000 aprsd-3.1.0/aprsd/web/chat/static/images/aprs-symbols-16-1.png
--rw-r--r--   0 i530566    (501) staff       (20)    52962 2022-11-23 18:33:33.000000 aprsd-3.1.0/aprsd/web/chat/static/images/aprs-symbols-64-0.png
--rw-r--r--   0 i530566    (501) staff       (20)    48951 2022-11-23 18:33:33.000000 aprsd-3.1.0/aprsd/web/chat/static/images/aprs-symbols-64-1.png
--rw-r--r--   0 i530566    (501) staff       (20)    40716 2022-11-23 18:33:33.000000 aprsd-3.1.0/aprsd/web/chat/static/images/aprs-symbols-64-2.png
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:34.064005 aprsd-3.1.0/aprsd/web/chat/static/js/
--rw-r--r--   0 i530566    (501) staff       (20)     1906 2022-12-16 17:08:52.000000 aprsd-3.1.0/aprsd/web/chat/static/js/gps.js
--rw-r--r--   0 i530566    (501) staff       (20)     1226 2022-11-23 18:33:33.000000 aprsd-3.1.0/aprsd/web/chat/static/js/main.js
--rw-r--r--   0 i530566    (501) staff       (20)     6304 2022-12-04 23:39:18.000000 aprsd-3.1.0/aprsd/web/chat/static/js/send-message-mobile.js
--rw-r--r--   0 i530566    (501) staff       (20)     6041 2022-12-04 23:39:18.000000 aprsd-3.1.0/aprsd/web/chat/static/js/send-message.js
--rw-r--r--   0 i530566    (501) staff       (20)      889 2022-11-23 18:33:33.000000 aprsd-3.1.0/aprsd/web/chat/static/js/tabs.js
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:34.066743 aprsd-3.1.0/aprsd/web/chat/static/json-viewer/
--rw-r--r--   0 i530566    (501) staff       (20)     1080 2022-11-23 18:33:33.000000 aprsd-3.1.0/aprsd/web/chat/static/json-viewer/jquery.json-viewer.css
--rw-r--r--   0 i530566    (501) staff       (20)     5020 2022-11-23 18:33:33.000000 aprsd-3.1.0/aprsd/web/chat/static/json-viewer/jquery.json-viewer.js
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:34.069691 aprsd-3.1.0/aprsd/web/chat/templates/
--rw-r--r--   0 i530566    (501) staff       (20)     4020 2022-12-04 23:39:18.000000 aprsd-3.1.0/aprsd/web/chat/templates/index.html
--rw-r--r--   0 i530566    (501) staff       (20)     4055 2022-12-04 23:39:18.000000 aprsd-3.1.0/aprsd/web/chat/templates/mobile.html
--rw-r--r--   0 i530566    (501) staff       (20)    10009 2023-07-24 13:39:24.000000 aprsd-3.1.0/aprsd/wsgi.py
--rw-r--r--   0 i530566    (501) staff       (20)     1599 2021-08-13 16:31:50.000000 aprsd-3.1.0/aprsd-lnav.json
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:33.568338 aprsd-3.1.0/aprsd.egg-info/
--rw-r--r--   0 i530566    (501) staff       (20)    21221 2023-07-24 15:26:54.000000 aprsd-3.1.0/aprsd.egg-info/PKG-INFO
--rw-r--r--   0 i530566    (501) staff       (20)     5051 2023-07-24 15:27:33.000000 aprsd-3.1.0/aprsd.egg-info/SOURCES.txt
--rw-r--r--   0 i530566    (501) staff       (20)        1 2023-07-24 15:26:54.000000 aprsd-3.1.0/aprsd.egg-info/dependency_links.txt
--rw-r--r--   0 i530566    (501) staff       (20)      171 2023-07-24 15:26:54.000000 aprsd-3.1.0/aprsd.egg-info/entry_points.txt
--rw-r--r--   0 i530566    (501) staff       (20)        1 2023-07-24 15:19:29.000000 aprsd-3.1.0/aprsd.egg-info/not-zip-safe
--rw-r--r--   0 i530566    (501) staff       (20)       46 2023-07-24 15:26:55.000000 aprsd-3.1.0/aprsd.egg-info/pbr.json
--rw-r--r--   0 i530566    (501) staff       (20)     1296 2023-07-24 15:26:54.000000 aprsd-3.1.0/aprsd.egg-info/requires.txt
--rw-r--r--   0 i530566    (501) staff       (20)        6 2023-07-24 15:26:54.000000 aprsd-3.1.0/aprsd.egg-info/top_level.txt
--rw-r--r--   0 i530566    (501) staff       (20)      221 2023-06-22 11:54:27.000000 aprsd-3.1.0/dev-requirements.in
--rw-r--r--   0 i530566    (501) staff       (20)     3898 2023-07-23 23:46:10.000000 aprsd-3.1.0/dev-requirements.txt
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:34.081769 aprsd-3.1.0/docker/
--rw-r--r--   0 i530566    (501) staff       (20)     1748 2023-05-05 15:07:23.000000 aprsd-3.1.0/docker/Dockerfile
--rw-r--r--   0 i530566    (501) staff       (20)     1557 2023-07-24 00:22:47.000000 aprsd-3.1.0/docker/Dockerfile-dev
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:34.107767 aprsd-3.1.0/docker/bin/
--rwxr-xr-x   0 i530566    (501) staff       (20)     1106 2023-07-24 00:22:47.000000 aprsd-3.1.0/docker/bin/admin.sh
--rwxr-xr-x   0 i530566    (501) staff       (20)      864 2023-07-18 00:59:03.000000 aprsd-3.1.0/docker/bin/listen.sh
--rwxr-xr-x   0 i530566    (501) staff       (20)      819 2023-07-18 00:59:03.000000 aprsd-3.1.0/docker/bin/run.sh
--rwxr-xr-x   0 i530566    (501) staff       (20)     2581 2023-04-17 19:01:56.000000 aprsd-3.1.0/docker/build.sh
--rw-r--r--   0 i530566    (501) staff       (20)      327 2022-11-22 00:10:29.000000 aprsd-3.1.0/docker/docker-compose.yml
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:34.137728 aprsd-3.1.0/docs/
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:34.164061 aprsd-3.1.0/docs/_static/
--rw-r--r--   0 i530566    (501) staff       (20)        0 2021-08-13 16:31:50.000000 aprsd-3.1.0/docs/_static/.keep
--rw-r--r--   0 i530566    (501) staff       (20)    77895 2021-08-30 17:18:20.000000 aprsd-3.1.0/docs/_static/aprsd_overview.png
--rw-r--r--   0 i530566    (501) staff       (20)    30397 2021-08-30 17:18:20.000000 aprsd-3.1.0/docs/_static/aprsd_overview.svg
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:34.166276 aprsd-3.1.0/docs/_templates/
--rw-r--r--   0 i530566    (501) staff       (20)        0 2021-08-13 16:31:50.000000 aprsd-3.1.0/docs/_templates/.keep
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:34.225686 aprsd-3.1.0/docs/apidoc/
--rw-r--r--   0 i530566    (501) staff       (20)      477 2023-01-02 19:13:49.000000 aprsd-3.1.0/docs/apidoc/aprsd.clients.rst
--rw-r--r--   0 i530566    (501) staff       (20)     1357 2023-01-02 19:13:49.000000 aprsd-3.1.0/docs/apidoc/aprsd.cmds.rst
--rw-r--r--   0 i530566    (501) staff       (20)     1044 2023-01-02 19:13:49.000000 aprsd-3.1.0/docs/apidoc/aprsd.conf.rst
--rw-r--r--   0 i530566    (501) staff       (20)      468 2023-01-02 19:13:49.000000 aprsd-3.1.0/docs/apidoc/aprsd.logging.rst
--rw-r--r--   0 i530566    (501) staff       (20)      969 2023-01-02 19:13:49.000000 aprsd-3.1.0/docs/apidoc/aprsd.packets.rst
--rw-r--r--   0 i530566    (501) staff       (20)     1523 2023-01-01 19:58:19.000000 aprsd-3.1.0/docs/apidoc/aprsd.plugins.rst
--rw-r--r--   0 i530566    (501) staff       (20)      447 2023-01-02 19:13:49.000000 aprsd-3.1.0/docs/apidoc/aprsd.rpc.rst
--rw-r--r--   0 i530566    (501) staff       (20)     1539 2023-01-02 19:13:49.000000 aprsd-3.1.0/docs/apidoc/aprsd.rst
--rw-r--r--   0 i530566    (501) staff       (20)      934 2023-01-02 19:13:49.000000 aprsd-3.1.0/docs/apidoc/aprsd.threads.rst
--rw-r--r--   0 i530566    (501) staff       (20)     1075 2023-01-02 19:13:49.000000 aprsd-3.1.0/docs/apidoc/aprsd.utils.rst
--rw-r--r--   0 i530566    (501) staff       (20)      168 2023-01-02 19:13:49.000000 aprsd-3.1.0/docs/apidoc/aprsd.web.admin.rst
--rw-r--r--   0 i530566    (501) staff       (20)      225 2023-01-02 19:13:49.000000 aprsd-3.1.0/docs/apidoc/aprsd.web.rst
--rw-r--r--   0 i530566    (501) staff       (20)       52 2023-01-01 19:58:20.000000 aprsd-3.1.0/docs/apidoc/modules.rst
--rw-r--r--   0 i530566    (501) staff       (20)     2997 2021-08-30 17:18:20.000000 aprsd-3.1.0/docs/aprsd.drawio
--rw-r--r--   0 i530566    (501) staff       (20)    19792 2023-01-01 19:57:28.000000 aprsd-3.1.0/docs/changelog.rst
--rw-r--r--   0 i530566    (501) staff       (20)      520 2022-12-12 18:34:04.000000 aprsd-3.1.0/docs/clean_docs.py
--rw-r--r--   0 i530566    (501) staff       (20)     5565 2022-12-29 19:14:44.000000 aprsd-3.1.0/docs/conf.py
--rw-r--r--   0 i530566    (501) staff       (20)     8611 2022-12-29 19:14:44.000000 aprsd-3.1.0/docs/configure.rst
--rw-r--r--   0 i530566    (501) staff       (20)      545 2021-08-13 16:31:50.000000 aprsd-3.1.0/docs/index.rst
--rw-r--r--   0 i530566    (501) staff       (20)     1553 2021-08-13 16:31:50.000000 aprsd-3.1.0/docs/install.rst
--rw-r--r--   0 i530566    (501) staff       (20)     1366 2021-08-13 16:31:50.000000 aprsd-3.1.0/docs/links.rst
--rw-r--r--   0 i530566    (501) staff       (20)     1613 2022-12-29 19:14:44.000000 aprsd-3.1.0/docs/plugin.rst
--rw-r--r--   0 i530566    (501) staff       (20)    20002 2023-01-01 19:57:28.000000 aprsd-3.1.0/docs/readme.rst
--rw-r--r--   0 i530566    (501) staff       (20)     2778 2021-08-13 16:31:50.000000 aprsd-3.1.0/docs/server.rst
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:33.323523 aprsd-3.1.0/examples/
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:34.229188 aprsd-3.1.0/examples/plugins/
--rw-r--r--   0 i530566    (501) staff       (20)        0 2022-12-12 18:34:04.000000 aprsd-3.1.0/examples/plugins/__init__.py
--rw-r--r--   0 i530566    (501) staff       (20)      409 2023-06-14 15:27:00.000000 aprsd-3.1.0/examples/plugins/example_plugin.py
--rw-r--r--   0 i530566    (501) staff       (20)       95 2021-08-30 17:18:20.000000 aprsd-3.1.0/gray.conf
--rw-r--r--   0 i530566    (501) staff       (20)      538 2021-08-30 17:18:20.000000 aprsd-3.1.0/pyproject.toml
--rw-r--r--   0 i530566    (501) staff       (20)      536 2023-07-23 23:46:10.000000 aprsd-3.1.0/requirements.in
--rw-r--r--   0 i530566    (501) staff       (20)     4086 2023-07-23 23:46:10.000000 aprsd-3.1.0/requirements.txt
--rw-r--r--   0 i530566    (501) staff       (20)     1245 2023-07-24 15:27:34.321796 aprsd-3.1.0/setup.cfg
--rw-r--r--   0 i530566    (501) staff       (20)     1015 2022-12-12 18:34:08.000000 aprsd-3.1.0/setup.py
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:34.257471 aprsd-3.1.0/tests/
--rw-r--r--   0 i530566    (501) staff       (20)        0 2022-12-12 18:34:04.000000 aprsd-3.1.0/tests/__init__.py
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:34.264798 aprsd-3.1.0/tests/cmds/
--rw-r--r--   0 i530566    (501) staff       (20)        0 2022-12-12 18:34:07.000000 aprsd-3.1.0/tests/cmds/__init__.py
--rw-r--r--   0 i530566    (501) staff       (20)     1810 2023-07-16 20:28:22.000000 aprsd-3.1.0/tests/cmds/test_send_message.py
--rw-r--r--   0 i530566    (501) staff       (20)     2498 2023-07-20 19:10:23.000000 aprsd-3.1.0/tests/cmds/test_webchat.py
--rw-r--r--   0 i530566    (501) staff       (20)     1674 2022-12-20 22:38:48.000000 aprsd-3.1.0/tests/fake.py
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:34.283374 aprsd-3.1.0/tests/plugins/
--rw-r--r--   0 i530566    (501) staff       (20)        0 2022-12-12 18:34:05.000000 aprsd-3.1.0/tests/plugins/__init__.py
--rw-r--r--   0 i530566    (501) staff       (20)     1112 2022-12-29 19:14:44.000000 aprsd-3.1.0/tests/plugins/test_fortune.py
--rw-r--r--   0 i530566    (501) staff       (20)     4012 2023-06-22 13:42:11.000000 aprsd-3.1.0/tests/plugins/test_location.py
--rw-r--r--   0 i530566    (501) staff       (20)     5895 2022-12-29 19:14:44.000000 aprsd-3.1.0/tests/plugins/test_notify.py
--rw-r--r--   0 i530566    (501) staff       (20)     1395 2022-12-29 19:14:44.000000 aprsd-3.1.0/tests/plugins/test_ping.py
--rw-r--r--   0 i530566    (501) staff       (20)     1696 2022-12-29 19:14:44.000000 aprsd-3.1.0/tests/plugins/test_query.py
--rw-r--r--   0 i530566    (501) staff       (20)     1458 2022-12-29 19:14:44.000000 aprsd-3.1.0/tests/plugins/test_time.py
--rw-r--r--   0 i530566    (501) staff       (20)      970 2022-12-29 19:14:44.000000 aprsd-3.1.0/tests/plugins/test_version.py
--rw-r--r--   0 i530566    (501) staff       (20)     7613 2022-12-29 19:14:44.000000 aprsd-3.1.0/tests/plugins/test_weather.py
--rw-r--r--   0 i530566    (501) staff       (20)      942 2022-12-29 19:14:44.000000 aprsd-3.1.0/tests/test_email.py
--rw-r--r--   0 i530566    (501) staff       (20)      558 2022-12-29 19:14:44.000000 aprsd-3.1.0/tests/test_main.py
--rw-r--r--   0 i530566    (501) staff       (20)     3070 2022-12-22 17:04:16.000000 aprsd-3.1.0/tests/test_packets.py
--rw-r--r--   0 i530566    (501) staff       (20)     6486 2022-12-29 19:14:44.000000 aprsd-3.1.0/tests/test_plugin.py
-drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-07-24 15:27:34.304991 aprsd-3.1.0/tools/
--rwxr-xr-x   0 i530566    (501) staff       (20)      586 2021-08-13 16:31:50.000000 aprsd-3.1.0/tools/fast8.sh
--rw-r--r--   0 i530566    (501) staff       (20)     2596 2022-12-20 22:38:48.000000 aprsd-3.1.0/tox.ini
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-08-07 16:01:55.629464 aprsd-3.1.1/
+-rw-r--r--   0 i530566    (501) staff       (20)      269 2021-08-30 17:18:20.000000 aprsd-3.1.1/.coveragerc
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-08-07 16:01:54.920043 aprsd-3.1.1/.github/
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-08-07 16:01:55.017485 aprsd-3.1.1/.github/workflows/
+-rw-r--r--   0 i530566    (501) staff       (20)     1461 2023-07-18 00:59:03.000000 aprsd-3.1.1/.github/workflows/manual_build.yml
+-rw-r--r--   0 i530566    (501) staff       (20)     1629 2023-07-20 18:34:31.000000 aprsd-3.1.1/.github/workflows/master-build.yml
+-rw-r--r--   0 i530566    (501) staff       (20)      523 2023-06-22 11:55:10.000000 aprsd-3.1.1/.github/workflows/python.yml
+-rw-r--r--   0 i530566    (501) staff       (20)     1270 2023-07-20 19:10:23.000000 aprsd-3.1.1/.github/workflows/release_build.yml
+-rw-r--r--   0 i530566    (501) staff       (20)      536 2021-08-30 17:18:20.000000 aprsd-3.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 i530566    (501) staff       (20)      574 2023-06-14 13:31:16.000000 aprsd-3.1.1/.readthedocs.yaml
+-rw-r--r--   0 i530566    (501) staff       (20)      430 2023-08-07 16:01:31.000000 aprsd-3.1.1/AUTHORS
+-rw-r--r--   0 i530566    (501) staff       (20)    22953 2023-08-07 16:01:30.000000 aprsd-3.1.1/ChangeLog
+-rw-r--r--   0 i530566    (501) staff       (20)      753 2021-08-13 16:31:50.000000 aprsd-3.1.1/INSTALL.txt
+-rw-r--r--   0 i530566    (501) staff       (20)    10142 2021-08-13 16:31:50.000000 aprsd-3.1.1/LICENSE
+-rw-r--r--   0 i530566    (501) staff       (20)       94 2021-08-13 16:31:50.000000 aprsd-3.1.1/MANIFEST.in
+-rw-r--r--   0 i530566    (501) staff       (20)     2737 2023-07-08 18:22:21.000000 aprsd-3.1.1/Makefile
+-rw-r--r--   0 i530566    (501) staff       (20)    21221 2023-08-07 16:01:55.629957 aprsd-3.1.1/PKG-INFO
+-rw-r--r--   0 i530566    (501) staff       (20)    20387 2023-07-16 20:28:02.000000 aprsd-3.1.1/README.rst
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-08-07 16:01:55.055070 aprsd-3.1.1/aprsd/
+-rw-r--r--   0 i530566    (501) staff       (20)      631 2022-12-12 18:34:05.000000 aprsd-3.1.1/aprsd/__init__.py
+-rw-r--r--   0 i530566    (501) staff       (20)    10517 2023-07-18 17:07:59.000000 aprsd-3.1.1/aprsd/admin_web.py
+-rw-r--r--   0 i530566    (501) staff       (20)     3208 2023-07-16 20:28:22.000000 aprsd-3.1.1/aprsd/cli_helper.py
+-rw-r--r--   0 i530566    (501) staff       (20)     9020 2023-07-24 21:03:29.000000 aprsd-3.1.1/aprsd/client.py
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-08-07 16:01:55.074359 aprsd-3.1.1/aprsd/clients/
+-rw-r--r--   0 i530566    (501) staff       (20)        0 2022-12-12 18:34:06.000000 aprsd-3.1.1/aprsd/clients/__init__.py
+-rw-r--r--   0 i530566    (501) staff       (20)     7207 2023-07-20 19:10:23.000000 aprsd-3.1.1/aprsd/clients/aprsis.py
+-rw-r--r--   0 i530566    (501) staff       (20)     3239 2023-07-31 15:15:02.000000 aprsd-3.1.1/aprsd/clients/kiss.py
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-08-07 16:01:55.116411 aprsd-3.1.1/aprsd/cmds/
+-rw-r--r--   0 i530566    (501) staff       (20)        0 2022-12-12 18:34:05.000000 aprsd-3.1.1/aprsd/cmds/__init__.py
+-rw-r--r--   0 i530566    (501) staff       (20)     1763 2023-07-08 21:30:26.000000 aprsd-3.1.1/aprsd/cmds/completion.py
+-rw-r--r--   0 i530566    (501) staff       (20)     3074 2023-07-08 21:30:26.000000 aprsd-3.1.1/aprsd/cmds/dev.py
+-rw-r--r--   0 i530566    (501) staff       (20)     5348 2023-07-22 21:05:15.000000 aprsd-3.1.1/aprsd/cmds/fetch_stats.py
+-rw-r--r--   0 i530566    (501) staff       (20)     2801 2023-07-16 20:28:22.000000 aprsd-3.1.1/aprsd/cmds/healthcheck.py
+-rw-r--r--   0 i530566    (501) staff       (20)     7920 2023-07-08 21:30:27.000000 aprsd-3.1.1/aprsd/cmds/list_plugins.py
+-rw-r--r--   0 i530566    (501) staff       (20)     6241 2023-07-16 20:28:22.000000 aprsd-3.1.1/aprsd/cmds/listen.py
+-rw-r--r--   0 i530566    (501) staff       (20)     4716 2023-07-08 21:30:26.000000 aprsd-3.1.1/aprsd/cmds/send_message.py
+-rw-r--r--   0 i530566    (501) staff       (20)     3416 2023-07-08 21:30:26.000000 aprsd-3.1.1/aprsd/cmds/server.py
+-rw-r--r--   0 i530566    (501) staff       (20)    13657 2023-07-24 21:03:29.000000 aprsd-3.1.1/aprsd/cmds/webchat.py
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-08-07 16:01:55.129447 aprsd-3.1.1/aprsd/conf/
+-rw-r--r--   0 i530566    (501) staff       (20)     1725 2023-07-16 20:28:21.000000 aprsd-3.1.1/aprsd/conf/__init__.py
+-rw-r--r--   0 i530566    (501) staff       (20)     2349 2023-07-16 20:28:22.000000 aprsd-3.1.1/aprsd/conf/client.py
+-rw-r--r--   0 i530566    (501) staff       (20)     4863 2023-01-19 19:14:47.000000 aprsd-3.1.1/aprsd/conf/common.py
+-rw-r--r--   0 i530566    (501) staff       (20)     1379 2023-07-16 20:28:22.000000 aprsd-3.1.1/aprsd/conf/log.py
+-rw-r--r--   0 i530566    (501) staff       (20)     2701 2022-12-29 19:14:43.000000 aprsd-3.1.1/aprsd/conf/opts.py
+-rw-r--r--   0 i530566    (501) staff       (20)     2308 2022-12-29 19:14:43.000000 aprsd-3.1.1/aprsd/conf/plugin_common.py
+-rw-r--r--   0 i530566    (501) staff       (20)     2332 2022-12-29 19:16:10.000000 aprsd-3.1.1/aprsd/conf/plugin_email.py
+-rw-r--r--   0 i530566    (501) staff       (20)      502 2022-12-12 18:34:08.000000 aprsd-3.1.1/aprsd/exception.py
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-08-07 16:01:55.157373 aprsd-3.1.1/aprsd/log/
+-rw-r--r--   0 i530566    (501) staff       (20)        0 2023-07-16 20:28:22.000000 aprsd-3.1.1/aprsd/log/__init__.py
+-rw-r--r--   0 i530566    (501) staff       (20)     2678 2023-07-16 20:28:22.000000 aprsd-3.1.1/aprsd/log/log.py
+-rw-r--r--   0 i530566    (501) staff       (20)     5545 2023-07-16 20:28:22.000000 aprsd-3.1.1/aprsd/log/rich.py
+-rw-r--r--   0 i530566    (501) staff       (20)     4571 2023-07-16 20:28:22.000000 aprsd-3.1.1/aprsd/main.py
+-rw-r--r--   0 i530566    (501) staff       (20)      134 2022-12-20 22:38:48.000000 aprsd-3.1.1/aprsd/messaging.py
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-08-07 16:01:55.201143 aprsd-3.1.1/aprsd/packets/
+-rw-r--r--   0 i530566    (501) staff       (20)      432 2023-01-16 16:38:59.000000 aprsd-3.1.1/aprsd/packets/__init__.py
+-rw-r--r--   0 i530566    (501) staff       (20)    19319 2023-07-31 15:15:02.000000 aprsd-3.1.1/aprsd/packets/core.py
+-rw-r--r--   0 i530566    (501) staff       (20)     1457 2022-12-29 19:14:43.000000 aprsd-3.1.1/aprsd/packets/packet_list.py
+-rw-r--r--   0 i530566    (501) staff       (20)     1071 2022-12-29 19:14:43.000000 aprsd-3.1.1/aprsd/packets/seen_list.py
+-rw-r--r--   0 i530566    (501) staff       (20)     3205 2022-12-29 19:14:43.000000 aprsd-3.1.1/aprsd/packets/tracker.py
+-rw-r--r--   0 i530566    (501) staff       (20)     2880 2022-12-29 19:14:43.000000 aprsd-3.1.1/aprsd/packets/watch_list.py
+-rw-r--r--   0 i530566    (501) staff       (20)    16435 2023-04-25 18:29:36.000000 aprsd-3.1.1/aprsd/plugin.py
+-rw-r--r--   0 i530566    (501) staff       (20)     2456 2023-08-07 15:07:11.000000 aprsd-3.1.1/aprsd/plugin_utils.py
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-08-07 16:01:55.222317 aprsd-3.1.1/aprsd/plugins/
+-rw-r--r--   0 i530566    (501) staff       (20)        0 2022-12-12 18:34:08.000000 aprsd-3.1.1/aprsd/plugins/__init__.py
+-rw-r--r--   0 i530566    (501) staff       (20)    23073 2023-07-16 20:28:22.000000 aprsd-3.1.1/aprsd/plugins/email.py
+-rw-r--r--   0 i530566    (501) staff       (20)     1463 2022-12-29 19:18:51.000000 aprsd-3.1.1/aprsd/plugins/fortune.py
+-rw-r--r--   0 i530566    (501) staff       (20)     3287 2023-07-10 15:01:50.000000 aprsd-3.1.1/aprsd/plugins/location.py
+-rw-r--r--   0 i530566    (501) staff       (20)     1969 2022-12-29 19:14:43.000000 aprsd-3.1.1/aprsd/plugins/notify.py
+-rw-r--r--   0 i530566    (501) staff       (20)      763 2022-12-29 19:18:50.000000 aprsd-3.1.1/aprsd/plugins/ping.py
+-rw-r--r--   0 i530566    (501) staff       (20)     2458 2022-12-29 19:14:43.000000 aprsd-3.1.1/aprsd/plugins/query.py
+-rw-r--r--   0 i530566    (501) staff       (20)     3496 2022-12-29 19:18:51.000000 aprsd-3.1.1/aprsd/plugins/time.py
+-rw-r--r--   0 i530566    (501) staff       (20)      849 2022-12-29 19:18:51.000000 aprsd-3.1.1/aprsd/plugins/version.py
+-rw-r--r--   0 i530566    (501) staff       (20)    13287 2023-08-01 01:53:09.000000 aprsd-3.1.1/aprsd/plugins/weather.py
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-08-07 16:01:55.227994 aprsd-3.1.1/aprsd/rpc/
+-rw-r--r--   0 i530566    (501) staff       (20)      343 2022-12-31 21:45:32.000000 aprsd-3.1.1/aprsd/rpc/__init__.py
+-rw-r--r--   0 i530566    (501) staff       (20)     4641 2023-07-23 23:46:10.000000 aprsd-3.1.1/aprsd/rpc/client.py
+-rw-r--r--   0 i530566    (501) staff       (20)     2847 2023-07-24 21:03:29.000000 aprsd-3.1.1/aprsd/rpc/server.py
+-rw-r--r--   0 i530566    (501) staff       (20)     7139 2023-07-31 15:15:02.000000 aprsd-3.1.1/aprsd/stats.py
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-08-07 16:01:55.254062 aprsd-3.1.1/aprsd/threads/
+-rw-r--r--   0 i530566    (501) staff       (20)      274 2022-12-20 22:38:48.000000 aprsd-3.1.1/aprsd/threads/__init__.py
+-rw-r--r--   0 i530566    (501) staff       (20)     2270 2023-07-20 19:10:23.000000 aprsd-3.1.1/aprsd/threads/aprsd.py
+-rw-r--r--   0 i530566    (501) staff       (20)     3921 2023-07-20 19:10:23.000000 aprsd-3.1.1/aprsd/threads/keep_alive.py
+-rw-r--r--   0 i530566    (501) staff       (20)     2036 2023-07-16 20:28:22.000000 aprsd-3.1.1/aprsd/threads/log_monitor.py
+-rw-r--r--   0 i530566    (501) staff       (20)    10431 2023-07-26 00:46:04.000000 aprsd-3.1.1/aprsd/threads/rx.py
+-rw-r--r--   0 i530566    (501) staff       (20)     6437 2023-07-28 21:20:55.000000 aprsd-3.1.1/aprsd/threads/tx.py
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-08-07 16:01:55.264095 aprsd-3.1.1/aprsd/utils/
+-rw-r--r--   0 i530566    (501) staff       (20)     3532 2022-12-16 13:25:52.000000 aprsd-3.1.1/aprsd/utils/__init__.py
+-rw-r--r--   0 i530566    (501) staff       (20)     1151 2022-12-20 22:38:48.000000 aprsd-3.1.1/aprsd/utils/counter.py
+-rw-r--r--   0 i530566    (501) staff       (20)     3265 2022-12-12 18:34:08.000000 aprsd-3.1.1/aprsd/utils/fuzzyclock.py
+-rw-r--r--   0 i530566    (501) staff       (20)     1871 2022-12-20 22:38:48.000000 aprsd-3.1.1/aprsd/utils/json.py
+-rw-r--r--   0 i530566    (501) staff       (20)     3200 2022-12-29 19:14:44.000000 aprsd-3.1.1/aprsd/utils/objectstore.py
+-rw-r--r--   0 i530566    (501) staff       (20)     1111 2022-12-20 22:38:48.000000 aprsd-3.1.1/aprsd/utils/ring_buffer.py
+-rw-r--r--   0 i530566    (501) staff       (20)     5558 2022-12-12 18:34:08.000000 aprsd-3.1.1/aprsd/utils/trace.py
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-08-07 16:01:55.265772 aprsd-3.1.1/aprsd/web/
+-rw-r--r--   0 i530566    (501) staff       (20)        0 2022-12-12 18:34:05.000000 aprsd-3.1.1/aprsd/web/__init__.py
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-08-07 16:01:55.268034 aprsd-3.1.1/aprsd/web/admin/
+-rw-r--r--   0 i530566    (501) staff       (20)        0 2022-12-12 18:34:05.000000 aprsd-3.1.1/aprsd/web/admin/__init__.py
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-08-07 16:01:54.949200 aprsd-3.1.1/aprsd/web/admin/static/
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-08-07 16:01:55.273877 aprsd-3.1.1/aprsd/web/admin/static/css/
+-rw-r--r--   0 i530566    (501) staff       (20)     1282 2022-11-23 18:33:33.000000 aprsd-3.1.1/aprsd/web/admin/static/css/index.css
+-rw-r--r--   0 i530566    (501) staff       (20)     3467 2022-11-23 18:33:33.000000 aprsd-3.1.1/aprsd/web/admin/static/css/prism.css
+-rw-r--r--   0 i530566    (501) staff       (20)      644 2022-11-23 18:33:33.000000 aprsd-3.1.1/aprsd/web/admin/static/css/tabs.css
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-08-07 16:01:55.307837 aprsd-3.1.1/aprsd/web/admin/static/images/
+-rw-r--r--   0 i530566    (501) staff       (20)    37797 2022-11-23 18:33:33.000000 aprsd-3.1.1/aprsd/web/admin/static/images/Untitled.png
+-rw-r--r--   0 i530566    (501) staff       (20)    52962 2022-11-23 18:33:33.000000 aprsd-3.1.1/aprsd/web/admin/static/images/aprs-symbols-16-0.png
+-rw-r--r--   0 i530566    (501) staff       (20)    48951 2022-11-23 18:33:33.000000 aprsd-3.1.1/aprsd/web/admin/static/images/aprs-symbols-16-1.png
+-rw-r--r--   0 i530566    (501) staff       (20)    52962 2022-11-23 18:33:33.000000 aprsd-3.1.1/aprsd/web/admin/static/images/aprs-symbols-64-0.png
+-rw-r--r--   0 i530566    (501) staff       (20)    48951 2022-11-23 18:33:33.000000 aprsd-3.1.1/aprsd/web/admin/static/images/aprs-symbols-64-1.png
+-rw-r--r--   0 i530566    (501) staff       (20)    40716 2022-11-23 18:33:33.000000 aprsd-3.1.1/aprsd/web/admin/static/images/aprs-symbols-64-2.png
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-08-07 16:01:55.320915 aprsd-3.1.1/aprsd/web/admin/static/js/
+-rw-r--r--   0 i530566    (501) staff       (20)     7360 2022-12-20 22:38:48.000000 aprsd-3.1.1/aprsd/web/admin/static/js/charts.js
+-rw-r--r--   0 i530566    (501) staff       (20)      658 2023-07-23 01:28:13.000000 aprsd-3.1.1/aprsd/web/admin/static/js/logs.js
+-rw-r--r--   0 i530566    (501) staff       (20)     6796 2022-12-29 19:14:44.000000 aprsd-3.1.1/aprsd/web/admin/static/js/main.js
+-rw-r--r--   0 i530566    (501) staff       (20)    64705 2022-11-23 18:33:33.000000 aprsd-3.1.1/aprsd/web/admin/static/js/prism.js
+-rw-r--r--   0 i530566    (501) staff       (20)     3852 2022-12-29 19:14:44.000000 aprsd-3.1.1/aprsd/web/admin/static/js/send-message.js
+-rw-r--r--   0 i530566    (501) staff       (20)      889 2022-11-23 18:33:33.000000 aprsd-3.1.1/aprsd/web/admin/static/js/tabs.js
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-08-07 16:01:55.327772 aprsd-3.1.1/aprsd/web/admin/static/json-viewer/
+-rw-r--r--   0 i530566    (501) staff       (20)     1080 2022-11-23 18:33:33.000000 aprsd-3.1.1/aprsd/web/admin/static/json-viewer/jquery.json-viewer.css
+-rw-r--r--   0 i530566    (501) staff       (20)     5020 2022-11-23 18:33:33.000000 aprsd-3.1.1/aprsd/web/admin/static/json-viewer/jquery.json-viewer.js
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-08-07 16:01:55.329736 aprsd-3.1.1/aprsd/web/admin/templates/
+-rw-r--r--   0 i530566    (501) staff       (20)     8034 2023-07-23 23:46:10.000000 aprsd-3.1.1/aprsd/web/admin/templates/index.html
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-08-07 16:01:54.953753 aprsd-3.1.1/aprsd/web/chat/
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-08-07 16:01:54.953272 aprsd-3.1.1/aprsd/web/chat/static/
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-08-07 16:01:55.354855 aprsd-3.1.1/aprsd/web/chat/static/css/
+-rw-r--r--   0 i530566    (501) staff       (20)     1376 2022-11-23 18:33:33.000000 aprsd-3.1.1/aprsd/web/chat/static/css/index.css
+-rw-r--r--   0 i530566    (501) staff       (20)   174659 2022-11-23 18:33:33.000000 aprsd-3.1.1/aprsd/web/chat/static/css/style.css.map
+-rw-r--r--   0 i530566    (501) staff       (20)      718 2022-11-23 18:33:33.000000 aprsd-3.1.1/aprsd/web/chat/static/css/tabs.css
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-08-07 16:01:55.366475 aprsd-3.1.1/aprsd/web/chat/static/images/
+-rw-r--r--   0 i530566    (501) staff       (20)    37797 2022-11-23 18:33:33.000000 aprsd-3.1.1/aprsd/web/chat/static/images/Untitled.png
+-rw-r--r--   0 i530566    (501) staff       (20)    52962 2022-11-23 18:33:33.000000 aprsd-3.1.1/aprsd/web/chat/static/images/aprs-symbols-16-0.png
+-rw-r--r--   0 i530566    (501) staff       (20)    48951 2022-11-23 18:33:33.000000 aprsd-3.1.1/aprsd/web/chat/static/images/aprs-symbols-16-1.png
+-rw-r--r--   0 i530566    (501) staff       (20)    52962 2022-11-23 18:33:33.000000 aprsd-3.1.1/aprsd/web/chat/static/images/aprs-symbols-64-0.png
+-rw-r--r--   0 i530566    (501) staff       (20)    48951 2022-11-23 18:33:33.000000 aprsd-3.1.1/aprsd/web/chat/static/images/aprs-symbols-64-1.png
+-rw-r--r--   0 i530566    (501) staff       (20)    40716 2022-11-23 18:33:33.000000 aprsd-3.1.1/aprsd/web/chat/static/images/aprs-symbols-64-2.png
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-08-07 16:01:55.412413 aprsd-3.1.1/aprsd/web/chat/static/js/
+-rw-r--r--   0 i530566    (501) staff       (20)     1906 2022-12-16 17:08:52.000000 aprsd-3.1.1/aprsd/web/chat/static/js/gps.js
+-rw-r--r--   0 i530566    (501) staff       (20)     1226 2022-11-23 18:33:33.000000 aprsd-3.1.1/aprsd/web/chat/static/js/main.js
+-rw-r--r--   0 i530566    (501) staff       (20)     6304 2022-12-04 23:39:18.000000 aprsd-3.1.1/aprsd/web/chat/static/js/send-message-mobile.js
+-rw-r--r--   0 i530566    (501) staff       (20)     6041 2022-12-04 23:39:18.000000 aprsd-3.1.1/aprsd/web/chat/static/js/send-message.js
+-rw-r--r--   0 i530566    (501) staff       (20)      889 2022-11-23 18:33:33.000000 aprsd-3.1.1/aprsd/web/chat/static/js/tabs.js
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-08-07 16:01:55.415002 aprsd-3.1.1/aprsd/web/chat/static/json-viewer/
+-rw-r--r--   0 i530566    (501) staff       (20)     1080 2022-11-23 18:33:33.000000 aprsd-3.1.1/aprsd/web/chat/static/json-viewer/jquery.json-viewer.css
+-rw-r--r--   0 i530566    (501) staff       (20)     5020 2022-11-23 18:33:33.000000 aprsd-3.1.1/aprsd/web/chat/static/json-viewer/jquery.json-viewer.js
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-08-07 16:01:55.420626 aprsd-3.1.1/aprsd/web/chat/templates/
+-rw-r--r--   0 i530566    (501) staff       (20)     4020 2022-12-04 23:39:18.000000 aprsd-3.1.1/aprsd/web/chat/templates/index.html
+-rw-r--r--   0 i530566    (501) staff       (20)     4055 2022-12-04 23:39:18.000000 aprsd-3.1.1/aprsd/web/chat/templates/mobile.html
+-rw-r--r--   0 i530566    (501) staff       (20)    10073 2023-07-26 12:47:34.000000 aprsd-3.1.1/aprsd/wsgi.py
+-rw-r--r--   0 i530566    (501) staff       (20)     1599 2021-08-13 16:31:50.000000 aprsd-3.1.1/aprsd-lnav.json
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-08-07 16:01:55.069892 aprsd-3.1.1/aprsd.egg-info/
+-rw-r--r--   0 i530566    (501) staff       (20)    21221 2023-08-07 16:01:31.000000 aprsd-3.1.1/aprsd.egg-info/PKG-INFO
+-rw-r--r--   0 i530566    (501) staff       (20)     5051 2023-08-07 16:01:54.000000 aprsd-3.1.1/aprsd.egg-info/SOURCES.txt
+-rw-r--r--   0 i530566    (501) staff       (20)        1 2023-08-07 16:01:31.000000 aprsd-3.1.1/aprsd.egg-info/dependency_links.txt
+-rw-r--r--   0 i530566    (501) staff       (20)      171 2023-08-07 16:01:31.000000 aprsd-3.1.1/aprsd.egg-info/entry_points.txt
+-rw-r--r--   0 i530566    (501) staff       (20)        1 2023-08-07 15:33:11.000000 aprsd-3.1.1/aprsd.egg-info/not-zip-safe
+-rw-r--r--   0 i530566    (501) staff       (20)       46 2023-08-07 16:01:31.000000 aprsd-3.1.1/aprsd.egg-info/pbr.json
+-rw-r--r--   0 i530566    (501) staff       (20)     1296 2023-08-07 16:01:31.000000 aprsd-3.1.1/aprsd.egg-info/requires.txt
+-rw-r--r--   0 i530566    (501) staff       (20)        6 2023-08-07 16:01:31.000000 aprsd-3.1.1/aprsd.egg-info/top_level.txt
+-rw-r--r--   0 i530566    (501) staff       (20)      221 2023-06-22 11:54:27.000000 aprsd-3.1.1/dev-requirements.in
+-rw-r--r--   0 i530566    (501) staff       (20)     3898 2023-07-23 23:46:10.000000 aprsd-3.1.1/dev-requirements.txt
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-08-07 16:01:55.428633 aprsd-3.1.1/docker/
+-rw-r--r--   0 i530566    (501) staff       (20)     1599 2023-07-24 21:03:29.000000 aprsd-3.1.1/docker/Dockerfile
+-rw-r--r--   0 i530566    (501) staff       (20)     1557 2023-07-24 00:22:47.000000 aprsd-3.1.1/docker/Dockerfile-dev
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-08-07 16:01:55.464744 aprsd-3.1.1/docker/bin/
+-rwxr-xr-x   0 i530566    (501) staff       (20)     1106 2023-07-24 00:22:47.000000 aprsd-3.1.1/docker/bin/admin.sh
+-rwxr-xr-x   0 i530566    (501) staff       (20)      864 2023-07-18 00:59:03.000000 aprsd-3.1.1/docker/bin/listen.sh
+-rwxr-xr-x   0 i530566    (501) staff       (20)      819 2023-07-18 00:59:03.000000 aprsd-3.1.1/docker/bin/run.sh
+-rwxr-xr-x   0 i530566    (501) staff       (20)     2581 2023-04-17 19:01:56.000000 aprsd-3.1.1/docker/build.sh
+-rw-r--r--   0 i530566    (501) staff       (20)      327 2022-11-22 00:10:29.000000 aprsd-3.1.1/docker/docker-compose.yml
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-08-07 16:01:55.515347 aprsd-3.1.1/docs/
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-08-07 16:01:55.548891 aprsd-3.1.1/docs/_static/
+-rw-r--r--   0 i530566    (501) staff       (20)        0 2021-08-13 16:31:50.000000 aprsd-3.1.1/docs/_static/.keep
+-rw-r--r--   0 i530566    (501) staff       (20)    77895 2021-08-30 17:18:20.000000 aprsd-3.1.1/docs/_static/aprsd_overview.png
+-rw-r--r--   0 i530566    (501) staff       (20)    30397 2021-08-30 17:18:20.000000 aprsd-3.1.1/docs/_static/aprsd_overview.svg
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-08-07 16:01:55.550791 aprsd-3.1.1/docs/_templates/
+-rw-r--r--   0 i530566    (501) staff       (20)        0 2021-08-13 16:31:50.000000 aprsd-3.1.1/docs/_templates/.keep
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-08-07 16:01:55.578545 aprsd-3.1.1/docs/apidoc/
+-rw-r--r--   0 i530566    (501) staff       (20)      477 2023-01-02 19:13:49.000000 aprsd-3.1.1/docs/apidoc/aprsd.clients.rst
+-rw-r--r--   0 i530566    (501) staff       (20)     1357 2023-01-02 19:13:49.000000 aprsd-3.1.1/docs/apidoc/aprsd.cmds.rst
+-rw-r--r--   0 i530566    (501) staff       (20)     1044 2023-01-02 19:13:49.000000 aprsd-3.1.1/docs/apidoc/aprsd.conf.rst
+-rw-r--r--   0 i530566    (501) staff       (20)      468 2023-01-02 19:13:49.000000 aprsd-3.1.1/docs/apidoc/aprsd.logging.rst
+-rw-r--r--   0 i530566    (501) staff       (20)      969 2023-01-02 19:13:49.000000 aprsd-3.1.1/docs/apidoc/aprsd.packets.rst
+-rw-r--r--   0 i530566    (501) staff       (20)     1523 2023-01-01 19:58:19.000000 aprsd-3.1.1/docs/apidoc/aprsd.plugins.rst
+-rw-r--r--   0 i530566    (501) staff       (20)      447 2023-01-02 19:13:49.000000 aprsd-3.1.1/docs/apidoc/aprsd.rpc.rst
+-rw-r--r--   0 i530566    (501) staff       (20)     1539 2023-01-02 19:13:49.000000 aprsd-3.1.1/docs/apidoc/aprsd.rst
+-rw-r--r--   0 i530566    (501) staff       (20)      934 2023-01-02 19:13:49.000000 aprsd-3.1.1/docs/apidoc/aprsd.threads.rst
+-rw-r--r--   0 i530566    (501) staff       (20)     1075 2023-01-02 19:13:49.000000 aprsd-3.1.1/docs/apidoc/aprsd.utils.rst
+-rw-r--r--   0 i530566    (501) staff       (20)      168 2023-01-02 19:13:49.000000 aprsd-3.1.1/docs/apidoc/aprsd.web.admin.rst
+-rw-r--r--   0 i530566    (501) staff       (20)      225 2023-01-02 19:13:49.000000 aprsd-3.1.1/docs/apidoc/aprsd.web.rst
+-rw-r--r--   0 i530566    (501) staff       (20)       52 2023-01-01 19:58:20.000000 aprsd-3.1.1/docs/apidoc/modules.rst
+-rw-r--r--   0 i530566    (501) staff       (20)     2997 2021-08-30 17:18:20.000000 aprsd-3.1.1/docs/aprsd.drawio
+-rw-r--r--   0 i530566    (501) staff       (20)    19792 2023-01-01 19:57:28.000000 aprsd-3.1.1/docs/changelog.rst
+-rw-r--r--   0 i530566    (501) staff       (20)      520 2022-12-12 18:34:04.000000 aprsd-3.1.1/docs/clean_docs.py
+-rw-r--r--   0 i530566    (501) staff       (20)     5565 2022-12-29 19:14:44.000000 aprsd-3.1.1/docs/conf.py
+-rw-r--r--   0 i530566    (501) staff       (20)     8611 2022-12-29 19:14:44.000000 aprsd-3.1.1/docs/configure.rst
+-rw-r--r--   0 i530566    (501) staff       (20)      545 2021-08-13 16:31:50.000000 aprsd-3.1.1/docs/index.rst
+-rw-r--r--   0 i530566    (501) staff       (20)     1553 2021-08-13 16:31:50.000000 aprsd-3.1.1/docs/install.rst
+-rw-r--r--   0 i530566    (501) staff       (20)     1366 2021-08-13 16:31:50.000000 aprsd-3.1.1/docs/links.rst
+-rw-r--r--   0 i530566    (501) staff       (20)     1613 2022-12-29 19:14:44.000000 aprsd-3.1.1/docs/plugin.rst
+-rw-r--r--   0 i530566    (501) staff       (20)    20002 2023-01-01 19:57:28.000000 aprsd-3.1.1/docs/readme.rst
+-rw-r--r--   0 i530566    (501) staff       (20)     2778 2021-08-13 16:31:50.000000 aprsd-3.1.1/docs/server.rst
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-08-07 16:01:54.958047 aprsd-3.1.1/examples/
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-08-07 16:01:55.597927 aprsd-3.1.1/examples/plugins/
+-rw-r--r--   0 i530566    (501) staff       (20)        0 2022-12-12 18:34:04.000000 aprsd-3.1.1/examples/plugins/__init__.py
+-rw-r--r--   0 i530566    (501) staff       (20)      409 2023-06-14 15:27:00.000000 aprsd-3.1.1/examples/plugins/example_plugin.py
+-rw-r--r--   0 i530566    (501) staff       (20)       95 2021-08-30 17:18:20.000000 aprsd-3.1.1/gray.conf
+-rw-r--r--   0 i530566    (501) staff       (20)      538 2023-08-07 15:02:58.000000 aprsd-3.1.1/pyproject.toml
+-rw-r--r--   0 i530566    (501) staff       (20)      536 2023-07-23 23:46:10.000000 aprsd-3.1.1/requirements.in
+-rw-r--r--   0 i530566    (501) staff       (20)     4086 2023-07-23 23:46:10.000000 aprsd-3.1.1/requirements.txt
+-rw-r--r--   0 i530566    (501) staff       (20)     1245 2023-08-07 16:01:55.653305 aprsd-3.1.1/setup.cfg
+-rw-r--r--   0 i530566    (501) staff       (20)     1015 2022-12-12 18:34:08.000000 aprsd-3.1.1/setup.py
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-08-07 16:01:55.607255 aprsd-3.1.1/tests/
+-rw-r--r--   0 i530566    (501) staff       (20)        0 2022-12-12 18:34:04.000000 aprsd-3.1.1/tests/__init__.py
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-08-07 16:01:55.611269 aprsd-3.1.1/tests/cmds/
+-rw-r--r--   0 i530566    (501) staff       (20)        0 2022-12-12 18:34:07.000000 aprsd-3.1.1/tests/cmds/__init__.py
+-rw-r--r--   0 i530566    (501) staff       (20)     1810 2023-07-16 20:28:22.000000 aprsd-3.1.1/tests/cmds/test_send_message.py
+-rw-r--r--   0 i530566    (501) staff       (20)     2498 2023-07-20 19:10:23.000000 aprsd-3.1.1/tests/cmds/test_webchat.py
+-rw-r--r--   0 i530566    (501) staff       (20)     1674 2022-12-20 22:38:48.000000 aprsd-3.1.1/tests/fake.py
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-08-07 16:01:55.626727 aprsd-3.1.1/tests/plugins/
+-rw-r--r--   0 i530566    (501) staff       (20)        0 2022-12-12 18:34:05.000000 aprsd-3.1.1/tests/plugins/__init__.py
+-rw-r--r--   0 i530566    (501) staff       (20)     1112 2022-12-29 19:14:44.000000 aprsd-3.1.1/tests/plugins/test_fortune.py
+-rw-r--r--   0 i530566    (501) staff       (20)     4012 2023-06-22 13:42:11.000000 aprsd-3.1.1/tests/plugins/test_location.py
+-rw-r--r--   0 i530566    (501) staff       (20)     5895 2022-12-29 19:14:44.000000 aprsd-3.1.1/tests/plugins/test_notify.py
+-rw-r--r--   0 i530566    (501) staff       (20)     1395 2022-12-29 19:14:44.000000 aprsd-3.1.1/tests/plugins/test_ping.py
+-rw-r--r--   0 i530566    (501) staff       (20)     1696 2022-12-29 19:14:44.000000 aprsd-3.1.1/tests/plugins/test_query.py
+-rw-r--r--   0 i530566    (501) staff       (20)     1458 2022-12-29 19:14:44.000000 aprsd-3.1.1/tests/plugins/test_time.py
+-rw-r--r--   0 i530566    (501) staff       (20)      970 2022-12-29 19:14:44.000000 aprsd-3.1.1/tests/plugins/test_version.py
+-rw-r--r--   0 i530566    (501) staff       (20)     7613 2022-12-29 19:14:44.000000 aprsd-3.1.1/tests/plugins/test_weather.py
+-rw-r--r--   0 i530566    (501) staff       (20)      942 2022-12-29 19:14:44.000000 aprsd-3.1.1/tests/test_email.py
+-rw-r--r--   0 i530566    (501) staff       (20)      558 2022-12-29 19:14:44.000000 aprsd-3.1.1/tests/test_main.py
+-rw-r--r--   0 i530566    (501) staff       (20)     3070 2022-12-22 17:04:16.000000 aprsd-3.1.1/tests/test_packets.py
+-rw-r--r--   0 i530566    (501) staff       (20)     6486 2022-12-29 19:14:44.000000 aprsd-3.1.1/tests/test_plugin.py
+drwxr-xr-x   0 i530566    (501) staff       (20)        0 2023-08-07 16:01:55.628045 aprsd-3.1.1/tools/
+-rwxr-xr-x   0 i530566    (501) staff       (20)      586 2021-08-13 16:31:50.000000 aprsd-3.1.1/tools/fast8.sh
+-rw-r--r--   0 i530566    (501) staff       (20)     2596 2022-12-20 22:38:48.000000 aprsd-3.1.1/tox.ini
```

### Comparing `aprsd-3.1.0/.github/workflows/manual_build.yml` & `aprsd-3.1.1/.github/workflows/manual_build.yml`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/.github/workflows/master-build.yml` & `aprsd-3.1.1/.github/workflows/master-build.yml`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/.github/workflows/python.yml` & `aprsd-3.1.1/.github/workflows/python.yml`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/.github/workflows/release_build.yml` & `aprsd-3.1.1/.github/workflows/release_build.yml`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/.pre-commit-config.yaml` & `aprsd-3.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/.readthedocs.yaml` & `aprsd-3.1.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/ChangeLog` & `aprsd-3.1.1/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,21 @@
 CHANGES
 =======
 
+v3.1.1
+------
+
+* Fixed pep8 failures
+* re-enable USWeatherPlugin to use mapClick
+* Fix sending packets over KISS interface
+* Use config web\_ip for running admin ui from module
+* remove loop log
+* Max out the client reconnect backoff to 5
+* Update the Dockerfile
+
 v3.1.0
 ------
 
 * Changelog updates for v3.1.0
 * Use CONF.admin.web\_port for single launch web admin
 * Fixed sio namespace registration
 * Update Dockerfile-dev to include uwsgi
```

### Comparing `aprsd-3.1.0/INSTALL.txt` & `aprsd-3.1.1/INSTALL.txt`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/LICENSE` & `aprsd-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/Makefile` & `aprsd-3.1.1/Makefile`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/PKG-INFO` & `aprsd-3.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aprsd
-Version: 3.1.0
+Version: 3.1.1
 Summary: Amateur radio APRS daemon which listens for messages and responds
 Home-page: http://aprsd.readthedocs.org
 Author: Craig Lamparter
 Author-email: something@somewhere.com
 License: Apache
 Project-URL: Source, https://github.com/craigerl/aprsd
 Project-URL: Tracker, https://github.com/craigerl/aprsd/issues
```

### Comparing `aprsd-3.1.0/README.rst` & `aprsd-3.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/__init__.py` & `aprsd-3.1.1/aprsd/__init__.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/admin_web.py` & `aprsd-3.1.1/aprsd/admin_web.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/cli_helper.py` & `aprsd-3.1.1/aprsd/cli_helper.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/client.py` & `aprsd-3.1.1/aprsd/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,16 +45,18 @@
         self.filter = filter
         if self._client:
             self._client.set_filter(filter)
 
     @property
     def client(self):
         if not self._client:
+            LOG.info("Creating APRS client")
             self._client = self.setup_connection()
             if self.filter:
+                LOG.info("Creating APRS client filter")
                 self._client.set_filter(self.filter)
         return self._client
 
     def send(self, packet: core.Packet):
         packet_list.PacketList().tx(packet)
         self.client.send(packet)
 
@@ -155,15 +157,19 @@
                 LOG.error(f"Failed to login to APRS-IS Server '{e}'")
                 connected = False
                 time.sleep(backoff)
             except Exception as e:
                 LOG.error(f"Unable to connect to APRS-IS server. '{e}' ")
                 connected = False
                 time.sleep(backoff)
-                backoff = backoff * 2
+                # Don't allow the backoff to go to inifinity.
+                if backoff > 5:
+                    backoff = 5
+                else:
+                    backoff += 1
                 continue
         LOG.debug(f"Logging in to APRS-IS with user '{user}'")
         self._client = aprs_client
         return aprs_client
 
 
 class KISSClient(Client):
```

### Comparing `aprsd-3.1.0/aprsd/clients/aprsis.py` & `aprsd-3.1.1/aprsd/clients/aprsis.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/clients/kiss.py` & `aprsd-3.1.1/aprsd/clients/kiss.py`

 * *Files 6% similar despite different names*

```diff
@@ -77,43 +77,37 @@
             LOG.error("Failed to parse bytes received from KISS interface.")
             LOG.exception(ex)
 
     def consumer(self, callback, blocking=False, immortal=False, raw=False):
         LOG.debug("Start blocking KISS consumer")
         self._parse_callback = callback
         self.kiss.read(callback=self.parse_frame, min_frames=None)
-        LOG.debug("END blocking KISS consumer")
+        LOG.debug(f"END blocking KISS consumer {self.kiss}")
 
     def send(self, packet):
         """Send an APRS Message object."""
 
-        # payload = (':%-9s:%s' % (
-        #     msg.tocall,
-        #     payload
-        # )).encode('US-ASCII'),
-        # payload = str(msg).encode('US-ASCII')
         payload = None
         path = ["WIDE1-1", "WIDE2-1"]
-        if isinstance(packet, core.AckPacket):
-            msg_payload = f"ack{packet.msgNo}"
-        elif isinstance(packet, core.Packet):
-            payload = packet.raw.encode("US-ASCII")
-            path = ["WIDE2-1"]
+        if isinstance(packet, core.Packet):
+            packet.prepare()
+            payload = packet.payload.encode("US-ASCII")
         else:
             msg_payload = f"{packet.raw}{{{str(packet.msgNo)}"
-
-        if not payload:
             payload = (
                 ":{:<9}:{}".format(
                     packet.to_call,
                     msg_payload,
                 )
             ).encode("US-ASCII")
 
-        LOG.debug(f"Send '{payload}' TO KISS")
+        LOG.debug(
+            f"KISS Send '{payload}' TO '{packet.to_call}' From "
+            f"'{packet.from_call}' with PATH '{path}'",
+        )
         frame = Frame.ui(
-            destination=packet.to_call,
+            destination="APZ100",
             source=packet.from_call,
             path=path,
             info=payload,
         )
         self.kiss.write(frame)
```

### Comparing `aprsd-3.1.0/aprsd/cmds/completion.py` & `aprsd-3.1.1/aprsd/cmds/completion.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/cmds/dev.py` & `aprsd-3.1.1/aprsd/cmds/dev.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/cmds/fetch_stats.py` & `aprsd-3.1.1/aprsd/cmds/fetch_stats.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/cmds/healthcheck.py` & `aprsd-3.1.1/aprsd/cmds/healthcheck.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/cmds/list_plugins.py` & `aprsd-3.1.1/aprsd/cmds/list_plugins.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/cmds/listen.py` & `aprsd-3.1.1/aprsd/cmds/listen.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/cmds/send_message.py` & `aprsd-3.1.1/aprsd/cmds/send_message.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/cmds/server.py` & `aprsd-3.1.1/aprsd/cmds/server.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/cmds/webchat.py` & `aprsd-3.1.1/aprsd/cmds/webchat.py`

 * *Files 2% similar despite different names*

```diff
@@ -261,16 +261,20 @@
 def _stats():
     stats_obj = stats.APRSDStats()
     now = datetime.datetime.now()
 
     time_format = "%m-%d-%Y %H:%M:%S"
     stats_dict = stats_obj.stats()
     # Webchat doesnt need these
-    del stats_dict["aprsd"]["watch_list"]
-    del stats_dict["aprsd"]["seen_list"]
+    if "watch_list" in stats_dict["aprsd"]:
+        del stats_dict["aprsd"]["watch_list"]
+    if "seen_list" in stats_dict["aprsd"]:
+        del stats_dict["aprsd"]["seen_list"]
+    if "threads" in stats_dict["aprsd"]:
+        del stats_dict["aprsd"]["threads"]
     # del stats_dict["email"]
     # del stats_dict["plugins"]
     # del stats_dict["messages"]
 
     result = {
         "time": now.strftime(time_format),
         "stats": stats_dict,
```

### Comparing `aprsd-3.1.0/aprsd/conf/__init__.py` & `aprsd-3.1.1/aprsd/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/conf/client.py` & `aprsd-3.1.1/aprsd/conf/client.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/conf/common.py` & `aprsd-3.1.1/aprsd/conf/common.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/conf/log.py` & `aprsd-3.1.1/aprsd/conf/log.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/conf/opts.py` & `aprsd-3.1.1/aprsd/conf/opts.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/conf/plugin_common.py` & `aprsd-3.1.1/aprsd/conf/plugin_common.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/conf/plugin_email.py` & `aprsd-3.1.1/aprsd/conf/plugin_email.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/log/log.py` & `aprsd-3.1.1/aprsd/log/log.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/log/rich.py` & `aprsd-3.1.1/aprsd/log/rich.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/main.py` & `aprsd-3.1.1/aprsd/main.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/packets/core.py` & `aprsd-3.1.1/aprsd/packets/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,14 +53,16 @@
     msgNo: str = field(default_factory=_init_msgNo)   # noqa: N815
     packet_type: str = None
     timestamp: float = field(default_factory=_int_timestamp)
     # Holds the raw text string to be sent over the wire
     # or holds the raw string from input packet
     raw: str = None
     raw_dict: dict = field(repr=False, default_factory=lambda: {})
+    # Built by calling prepare().  raw needs this built first.
+    payload: str = None
 
     # Fields related to sending packets out
     send_count: int = field(repr=False, default=0)
     retry_count: int = field(repr=False, default=3)
     last_send_time: datetime.timedelta = field(repr=False, default=None)
     # Do we allow this packet to be saved to send later?
     allow_delay: bool = field(repr=False, default=True)
@@ -88,19 +90,32 @@
 
     def update_timestamp(self):
         self.timestamp = _int_timestamp()
 
     def prepare(self):
         """Do stuff here that is needed prior to sending over the air."""
         # now build the raw message for sending
+        self._build_payload()
         self._build_raw()
 
+    def _build_payload(self):
+        """The payload is the non headers portion of the packet."""
+        msg = self._filter_for_send().rstrip("\n")
+        self.payload = (
+            f":{self.to_call.ljust(9)}"
+            f":{msg}"
+        )
+
     def _build_raw(self):
-        """Build the self.raw string which is what is sent over the air."""
-        self.raw = self._filter_for_send().rstrip("\n")
+        """Build the self.raw which is what is sent over the air."""
+        self.raw = "{}>APZ100:{}".format(
+            self.from_call,
+            self.payload,
+        )
+        LOG.debug(f"_build_raw: payload '{self.payload}' raw '{self.raw}'")
 
     @staticmethod
     def factory(raw_packet):
         raw = raw_packet
         raw["raw_dict"] = raw.copy()
         translate_fields = {
             "from": "from_call",
@@ -229,50 +244,40 @@
 
 
 @dataclass
 class PathPacket(Packet):
     path: List[str] = field(default_factory=list)
     via: str = None
 
-    def _build_raw(self):
+    def _build_payload(self):
         raise NotImplementedError
 
 
 @dataclass
 class AckPacket(PathPacket):
     response: str = None
 
     def __post__init__(self):
         if self.response:
             LOG.warning("Response set!")
 
-    def _build_raw(self):
-        """Build the self.raw which is what is sent over the air."""
-        self.raw = "{}>APZ100::{}:ack{}".format(
-            self.from_call,
-            self.to_call.ljust(9),
-            self.msgNo,
-        )
+    def _build_payload(self):
+        self.payload = f":{self.to_call.ljust(9)}:ack{self.msgNo}"
 
 
 @dataclass
 class RejectPacket(PathPacket):
     response: str = None
 
     def __post__init__(self):
         if self.response:
             LOG.warning("Response set!")
 
-    def _build_raw(self):
-        """Build the self.raw which is what is sent over the air."""
-        self.raw = "{}>APZ100::{} :rej{}".format(
-            self.from_call,
-            self.to_call.ljust(9),
-            self.msgNo,
-        )
+    def _build_payload(self):
+        self.payload = f":{self.to_call.ljust(9)} :rej{self.msgNo}"
 
 
 @dataclass
 class MessagePacket(PathPacket):
     message_text: str = None
 
     def _filter_for_send(self) -> str:
@@ -281,31 +286,29 @@
         # and ftm400-send is max 64.  setting this to
         # 67 displays 64 on the ftm400. (+3 {01 suffix)
         # feature req: break long ones into two msgs
         message = self.message_text[:67]
         # We all miss George Carlin
         return re.sub("fuck|shit|cunt|piss|cock|bitch", "****", message)
 
-    def _build_raw(self):
-        """Build the self.raw which is what is sent over the air."""
-        self.raw = "{}>APZ100::{}:{}{{{}".format(
-            self.from_call,
+    def _build_payload(self):
+        self.payload = ":{}:{}{{{}".format(
             self.to_call.ljust(9),
             self._filter_for_send().rstrip("\n"),
             str(self.msgNo),
         )
 
 
 @dataclass
 class StatusPacket(PathPacket):
     status: str = None
     messagecapable: bool = False
     comment: str = None
 
-    def _build_raw(self):
+    def _build_payload(self):
         raise NotImplementedError
 
 
 @dataclass
 class GPSPacket(PathPacket):
     latitude: float = 0.00
     longitude: float = 0.00
@@ -396,71 +399,86 @@
             self.timestamp = datetime.datetime.timestamp(local_dt)
 
         utc_offset_timedelta = datetime.datetime.utcnow() - local_dt
         result_utc_datetime = local_dt + utc_offset_timedelta
         time_zulu = result_utc_datetime.strftime("%d%H%M")
         return time_zulu
 
-    def _build_raw(self):
+    def _build_payload(self):
+        """The payload is the non headers portion of the packet."""
         time_zulu = self._build_time_zulu()
+        lat = self.latitude
+        long = self.longitude
+        self.payload = (
+            f"@{time_zulu}z{lat}{self.symbol_table}"
+            f"{long}{self.symbol}"
+        )
+
+        if self.comment:
+            self.payload = f"{self.payload}{self.comment}"
 
+    def _build_raw(self):
         self.raw = (
             f"{self.from_call}>{self.to_call},WIDE2-1:"
-            f"@{time_zulu}z{self.latitude}{self.symbol_table}"
-            f"{self.longitude}{self.symbol}"
+            f"{self.payload}"
         )
-        if self.comment:
-            self.raw = f"{self.raw}{self.comment}"
 
 
 @dataclass
 class MicEPacket(GPSPacket):
     messagecapable: bool = False
     mbits: str = None
     mtype: str = None
     # in MPH
     speed: float = 0.00
     # 0 to 360
     course: int = 0
 
-    def _build_raw(self):
+    def _build_payload(self):
         raise NotImplementedError
 
 
 @dataclass
 class ObjectPacket(GPSPacket):
     alive: bool = True
     raw_timestamp: str = None
     symbol: str = field(default="r")
     # in MPH
     speed: float = 0.00
     # 0 to 360
     course: int = 0
 
+    def _build_payload(self):
+        time_zulu = self._build_time_zulu()
+        lat = self.convert_latitude(self.latitude)
+        long = self.convert_longitude(self.longitude)
+
+        self.payload = (
+            f"*{time_zulu}z{lat}{self.symbol_table}"
+            f"{long}{self.symbol}"
+        )
+
+        if self.comment:
+            self.payload = f"{self.payload}{self.comment}"
+
     def _build_raw(self):
         """
         REPEAT builds packets like
         reply = "{}>APZ100:;{:9s}*{}z{}r{:.3f}MHz {} {}".format(
                 fromcall, callsign, time_zulu, latlon, freq, uplink_tone, offset,
             )
         where fromcall is the callsign that is sending the packet
         callsign is the station callsign for the object
         The frequency, uplink_tone, offset is part of the comment
         """
-        time_zulu = self._build_time_zulu()
-        lat = self.convert_latitude(self.latitude)
-        long = self.convert_longitude(self.longitude)
 
         self.raw = (
             f"{self.from_call}>APZ100:;{self.to_call:9s}"
-            f"*{time_zulu}z{lat}{self.symbol_table}"
-            f"{long}{self.symbol}"
+            f"{self.payload}"
         )
-        if self.comment:
-            self.raw = f"{self.raw}{self.comment}"
 
 
 @dataclass()
 class WeatherPacket(GPSPacket):
     symbol: str = "_"
     wind_speed: float = 0.00
     wind_direction: int = 0
@@ -470,15 +488,15 @@
     rain_1h: float = 0.00
     rain_24h: float = 0.00
     rain_since_midnight: float = 0.00
     humidity: int = 0
     pressure: float = 0.00
     comment: str = None
 
-    def _build_raw(self):
+    def _build_payload(self):
         """Build an uncompressed weather packet
 
         Format =
 
        _CSE/SPDgXXXtXXXrXXXpXXXPXXXhXXbXXXXX%type NEW FORMAT APRS793 June 97
                                                   NOT BACKWARD COMPATIBLE
 
@@ -498,15 +516,14 @@
         % shows software type d=Dos, m=Mac, w=Win, etc
         type shows type of WX instrument
 
         """
         time_zulu = self._build_time_zulu()
 
         contents = [
-            f"{self.from_call}>{self.to_call},WIDE1-1,WIDE2-1:",
             f"@{time_zulu}z{self.latitude}{self.symbol_table}",
             f"{self.longitude}{self.symbol}",
             f"{self.wind_direction:03d}",
             # Speed = sustained 1 minute wind speed in mph
             f"{self.symbol_table}", f"{self.wind_speed:03.0f}",
             # wind gust (peak wind speed in mph in the last 5 minutes)
             f"g{self.wind_gust:03.0f}",
@@ -519,19 +536,24 @@
             # Rainfall (in hundredths of an inch) since midnigt
             f"P{self.rain_since_midnight*100:03.0f}",
             # Humidity
             f"h{self.humidity:02d}",
             # Barometric pressure (in tenths of millibars/tenths of hPascal)
             f"b{self.pressure:05.0f}",
         ]
-
         if self.comment:
             contents.append(self.comment)
+        self.payload = "".join(contents)
+
+    def _build_raw(self):
 
-        self.raw = "".join(contents)
+        self.raw = (
+            f"{self.from_call}>{self.to_call},WIDE1-1,WIDE2-1:"
+            f"{self.payload}"
+        )
 
 
 TYPE_LOOKUP = {
     PACKET_TYPE_WX: WeatherPacket,
     PACKET_TYPE_MESSAGE: MessagePacket,
     PACKET_TYPE_ACK: AckPacket,
     PACKET_TYPE_REJECT: RejectPacket,
```

### Comparing `aprsd-3.1.0/aprsd/packets/packet_list.py` & `aprsd-3.1.1/aprsd/packets/packet_list.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/packets/seen_list.py` & `aprsd-3.1.1/aprsd/packets/seen_list.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/packets/tracker.py` & `aprsd-3.1.1/aprsd/packets/tracker.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/packets/watch_list.py` & `aprsd-3.1.1/aprsd/packets/watch_list.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/plugin.py` & `aprsd-3.1.1/aprsd/plugin.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/plugin_utils.py` & `aprsd-3.1.1/aprsd/plugin_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,17 +29,17 @@
     LOG.debug(f"Fetch station at {lat}, {lon}")
     headers = requests.utils.default_headers()
     headers.update(
         {"User-Agent": "(aprsd, waboring@hemna.com)"},
     )
     try:
         url2 = (
-            # "https://forecast.weather.gov/MapClick.php?lat=%s"
-            # "&lon=%s&FcstType=json" % (lat, lon)
-            f"https://api.weather.gov/points/{lat},{lon}"
+            "https://forecast.weather.gov/MapClick.php?lat=%s"
+            "&lon=%s&FcstType=json" % (lat, lon)
+            # f"https://api.weather.gov/points/{lat},{lon}"
         )
         LOG.debug(f"Fetching weather '{url2}'")
         response = requests.get(url2, headers=headers)
     except Exception as e:
         LOG.error(e)
         raise Exception("Failed to get weather")
     else:
```

### Comparing `aprsd-3.1.0/aprsd/plugins/email.py` & `aprsd-3.1.1/aprsd/plugins/email.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/plugins/fortune.py` & `aprsd-3.1.1/aprsd/plugins/fortune.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/plugins/location.py` & `aprsd-3.1.1/aprsd/plugins/location.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/plugins/notify.py` & `aprsd-3.1.1/aprsd/plugins/notify.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/plugins/ping.py` & `aprsd-3.1.1/aprsd/plugins/ping.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/plugins/query.py` & `aprsd-3.1.1/aprsd/plugins/query.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/plugins/time.py` & `aprsd-3.1.1/aprsd/plugins/time.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/plugins/version.py` & `aprsd-3.1.1/aprsd/plugins/version.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/plugins/weather.py` & `aprsd-3.1.1/aprsd/plugins/weather.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,19 +33,26 @@
     def setup(self):
         self.ensure_aprs_fi_key()
 
     @trace.trace
     def process(self, packet):
         LOG.info("Weather Plugin")
         fromcall = packet.from_call
+        message = packet.get("message_text", None)
         # message = packet.get("message_text", None)
         # ack = packet.get("msgNo", "0")
+        a = re.search(r"^.*\s+(.*)", message)
+        if a is not None:
+            searchcall = a.group(1)
+            searchcall = searchcall.upper()
+        else:
+            searchcall = fromcall
         api_key = CONF.aprs_fi.apiKey
         try:
-            aprs_data = plugin_utils.get_aprs_fi(api_key, fromcall)
+            aprs_data = plugin_utils.get_aprs_fi(api_key, searchcall)
         except Exception as ex:
             LOG.error(f"Failed to fetch aprs.fi data {ex}")
             return "Failed to fetch aprs.fi location"
 
         LOG.debug(f"LocationPlugin: aprs_data = {aprs_data}")
         if not len(aprs_data["entries"]):
             LOG.error("Didn't get any entries from aprs.fi")
```

### Comparing `aprsd-3.1.0/aprsd/rpc/client.py` & `aprsd-3.1.1/aprsd/rpc/client.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/rpc/server.py` & `aprsd-3.1.1/aprsd/rpc/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,18 @@
 CONF = cfg.CONF
 LOG = logging.getLogger("APRSD")
 
 
 def magic_word_authenticator(sock):
     magic = sock.recv(len(CONF.rpc_settings.magic_word)).decode()
     if magic != CONF.rpc_settings.magic_word:
-        raise AuthenticationError(f"wrong magic word {magic}")
+        raise AuthenticationError(
+            f"wrong magic word passed in '{magic}'"
+            f" != '{CONF.rpc_settings.magic_word}'",
+        )
     return sock, None
 
 
 class APRSDRPCThread(threads.APRSDThread):
     def __init__(self):
         super().__init__(name="RPCThread")
         self.thread = ThreadPoolServer(
```

### Comparing `aprsd-3.1.0/aprsd/stats.py` & `aprsd-3.1.1/aprsd/stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -242,15 +242,14 @@
                 "enabled": CONF.email_plugin.enabled,
                 "sent": int(self._email_tx),
                 "received": int(self._email_rx),
                 "thread_last_update": last_update,
             },
             "plugins": plugin_stats,
         }
-        LOG.debug(f"STATS = {stats}")
         LOG.info("APRSD Stats: DONE")
         return stats
 
     def __str__(self):
         pl = packets.PacketList()
         return (
             "Uptime:{} Msgs TX:{} RX:{} "
```

### Comparing `aprsd-3.1.0/aprsd/threads/aprsd.py` & `aprsd-3.1.1/aprsd/threads/aprsd.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/threads/keep_alive.py` & `aprsd-3.1.1/aprsd/threads/keep_alive.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/threads/log_monitor.py` & `aprsd-3.1.1/aprsd/threads/log_monitor.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/threads/rx.py` & `aprsd-3.1.1/aprsd/threads/rx.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/threads/tx.py` & `aprsd-3.1.1/aprsd/threads/tx.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/utils/__init__.py` & `aprsd-3.1.1/aprsd/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/utils/counter.py` & `aprsd-3.1.1/aprsd/utils/counter.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/utils/fuzzyclock.py` & `aprsd-3.1.1/aprsd/utils/fuzzyclock.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/utils/json.py` & `aprsd-3.1.1/aprsd/utils/json.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/utils/objectstore.py` & `aprsd-3.1.1/aprsd/utils/objectstore.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/utils/ring_buffer.py` & `aprsd-3.1.1/aprsd/utils/ring_buffer.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/utils/trace.py` & `aprsd-3.1.1/aprsd/utils/trace.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/web/admin/static/css/index.css` & `aprsd-3.1.1/aprsd/web/admin/static/css/index.css`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/web/admin/static/css/prism.css` & `aprsd-3.1.1/aprsd/web/admin/static/css/prism.css`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/web/admin/static/css/tabs.css` & `aprsd-3.1.1/aprsd/web/admin/static/css/tabs.css`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/web/admin/static/images/Untitled.png` & `aprsd-3.1.1/aprsd/web/admin/static/images/Untitled.png`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/web/admin/static/images/aprs-symbols-16-0.png` & `aprsd-3.1.1/aprsd/web/admin/static/images/aprs-symbols-16-0.png`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/web/admin/static/images/aprs-symbols-16-1.png` & `aprsd-3.1.1/aprsd/web/admin/static/images/aprs-symbols-16-1.png`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/web/admin/static/images/aprs-symbols-64-0.png` & `aprsd-3.1.1/aprsd/web/admin/static/images/aprs-symbols-64-0.png`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/web/admin/static/images/aprs-symbols-64-1.png` & `aprsd-3.1.1/aprsd/web/admin/static/images/aprs-symbols-64-1.png`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/web/admin/static/images/aprs-symbols-64-2.png` & `aprsd-3.1.1/aprsd/web/admin/static/images/aprs-symbols-64-2.png`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/web/admin/static/js/charts.js` & `aprsd-3.1.1/aprsd/web/admin/static/js/charts.js`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/web/admin/static/js/logs.js` & `aprsd-3.1.1/aprsd/web/admin/static/js/logs.js`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/web/admin/static/js/main.js` & `aprsd-3.1.1/aprsd/web/admin/static/js/main.js`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/web/admin/static/js/prism.js` & `aprsd-3.1.1/aprsd/web/admin/static/js/prism.js`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/web/admin/static/js/send-message.js` & `aprsd-3.1.1/aprsd/web/admin/static/js/send-message.js`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/web/admin/static/js/tabs.js` & `aprsd-3.1.1/aprsd/web/admin/static/js/tabs.js`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/web/admin/static/json-viewer/jquery.json-viewer.css` & `aprsd-3.1.1/aprsd/web/admin/static/json-viewer/jquery.json-viewer.css`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/web/admin/static/json-viewer/jquery.json-viewer.js` & `aprsd-3.1.1/aprsd/web/admin/static/json-viewer/jquery.json-viewer.js`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/web/admin/templates/index.html` & `aprsd-3.1.1/aprsd/web/admin/templates/index.html`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/web/chat/static/css/index.css` & `aprsd-3.1.1/aprsd/web/chat/static/css/index.css`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/web/chat/static/css/style.css.map` & `aprsd-3.1.1/aprsd/web/chat/static/css/style.css.map`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/web/chat/static/css/tabs.css` & `aprsd-3.1.1/aprsd/web/chat/static/css/tabs.css`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/web/chat/static/images/Untitled.png` & `aprsd-3.1.1/aprsd/web/chat/static/images/Untitled.png`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/web/chat/static/images/aprs-symbols-16-0.png` & `aprsd-3.1.1/aprsd/web/chat/static/images/aprs-symbols-16-0.png`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/web/chat/static/images/aprs-symbols-16-1.png` & `aprsd-3.1.1/aprsd/web/chat/static/images/aprs-symbols-16-1.png`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/web/chat/static/images/aprs-symbols-64-0.png` & `aprsd-3.1.1/aprsd/web/chat/static/images/aprs-symbols-64-0.png`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/web/chat/static/images/aprs-symbols-64-1.png` & `aprsd-3.1.1/aprsd/web/chat/static/images/aprs-symbols-64-1.png`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/web/chat/static/images/aprs-symbols-64-2.png` & `aprsd-3.1.1/aprsd/web/chat/static/images/aprs-symbols-64-2.png`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/web/chat/static/js/gps.js` & `aprsd-3.1.1/aprsd/web/chat/static/js/gps.js`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/web/chat/static/js/main.js` & `aprsd-3.1.1/aprsd/web/chat/static/js/main.js`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/web/chat/static/js/send-message-mobile.js` & `aprsd-3.1.1/aprsd/web/chat/static/js/send-message-mobile.js`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/web/chat/static/js/send-message.js` & `aprsd-3.1.1/aprsd/web/chat/static/js/send-message.js`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/web/chat/static/js/tabs.js` & `aprsd-3.1.1/aprsd/web/chat/static/js/tabs.js`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/web/chat/static/json-viewer/jquery.json-viewer.css` & `aprsd-3.1.1/aprsd/web/chat/static/json-viewer/jquery.json-viewer.css`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/web/chat/static/json-viewer/jquery.json-viewer.js` & `aprsd-3.1.1/aprsd/web/chat/static/json-viewer/jquery.json-viewer.js`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/web/chat/templates/index.html` & `aprsd-3.1.1/aprsd/web/chat/templates/index.html`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/web/chat/templates/mobile.html` & `aprsd-3.1.1/aprsd/web/chat/templates/mobile.html`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd/wsgi.py` & `aprsd-3.1.1/aprsd/wsgi.py`

 * *Files 4% similar despite different names*

```diff
@@ -326,15 +326,20 @@
     async_mode = "threading"
     sio = socketio.Server(logger=True, async_mode=async_mode)
     app.wsgi_app = socketio.WSGIApp(sio, app.wsgi_app)
     log_level = init_app(log_level="DEBUG")
     setup_logging(app, log_level)
     sio.register_namespace(LoggingNamespace("/logs"))
     CONF.log_opt_values(LOG, logging.DEBUG)
-    app.run(threaded=True, debug=True, port=CONF.admin.web_port)
+    app.run(
+        threaded=True,
+        debug=False,
+        port=CONF.admin.web_port,
+        host=CONF.admin.web_ip,
+    )
 
 
 if __name__ == "uwsgi_file_aprsd_wsgi":
     # Start with
     # uwsgi --http :8000 --gevent 1000 --http-websockets --master -w aprsd.wsgi --callable app
 
     async_mode = "gevent_uwsgi"
```

### Comparing `aprsd-3.1.0/aprsd-lnav.json` & `aprsd-3.1.1/aprsd-lnav.json`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd.egg-info/PKG-INFO` & `aprsd-3.1.1/aprsd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aprsd
-Version: 3.1.0
+Version: 3.1.1
 Summary: Amateur radio APRS daemon which listens for messages and responds
 Home-page: http://aprsd.readthedocs.org
 Author: Craig Lamparter
 Author-email: something@somewhere.com
 License: Apache
 Project-URL: Source, https://github.com/craigerl/aprsd
 Project-URL: Tracker, https://github.com/craigerl/aprsd/issues
```

### Comparing `aprsd-3.1.0/aprsd.egg-info/SOURCES.txt` & `aprsd-3.1.1/aprsd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/aprsd.egg-info/requires.txt` & `aprsd-3.1.1/aprsd.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/dev-requirements.txt` & `aprsd-3.1.1/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/docker/Dockerfile-dev` & `aprsd-3.1.1/docker/Dockerfile-dev`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/docker/bin/admin.sh` & `aprsd-3.1.1/docker/bin/admin.sh`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/docker/bin/listen.sh` & `aprsd-3.1.1/docker/bin/listen.sh`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/docker/bin/run.sh` & `aprsd-3.1.1/docker/bin/run.sh`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/docker/build.sh` & `aprsd-3.1.1/docker/build.sh`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/docs/_static/aprsd_overview.png` & `aprsd-3.1.1/docs/_static/aprsd_overview.png`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/docs/_static/aprsd_overview.svg` & `aprsd-3.1.1/docs/_static/aprsd_overview.svg`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/docs/apidoc/aprsd.cmds.rst` & `aprsd-3.1.1/docs/apidoc/aprsd.cmds.rst`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/docs/apidoc/aprsd.conf.rst` & `aprsd-3.1.1/docs/apidoc/aprsd.conf.rst`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/docs/apidoc/aprsd.packets.rst` & `aprsd-3.1.1/docs/apidoc/aprsd.packets.rst`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/docs/apidoc/aprsd.plugins.rst` & `aprsd-3.1.1/docs/apidoc/aprsd.plugins.rst`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/docs/apidoc/aprsd.rst` & `aprsd-3.1.1/docs/apidoc/aprsd.rst`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/docs/apidoc/aprsd.threads.rst` & `aprsd-3.1.1/docs/apidoc/aprsd.threads.rst`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/docs/apidoc/aprsd.utils.rst` & `aprsd-3.1.1/docs/apidoc/aprsd.utils.rst`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/docs/aprsd.drawio` & `aprsd-3.1.1/docs/aprsd.drawio`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/docs/changelog.rst` & `aprsd-3.1.1/docs/changelog.rst`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/docs/clean_docs.py` & `aprsd-3.1.1/docs/clean_docs.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/docs/conf.py` & `aprsd-3.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/docs/configure.rst` & `aprsd-3.1.1/docs/configure.rst`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/docs/index.rst` & `aprsd-3.1.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/docs/install.rst` & `aprsd-3.1.1/docs/install.rst`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/docs/links.rst` & `aprsd-3.1.1/docs/links.rst`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/docs/plugin.rst` & `aprsd-3.1.1/docs/plugin.rst`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/docs/readme.rst` & `aprsd-3.1.1/docs/readme.rst`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/docs/server.rst` & `aprsd-3.1.1/docs/server.rst`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/pyproject.toml` & `aprsd-3.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/requirements.in` & `aprsd-3.1.1/requirements.in`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/requirements.txt` & `aprsd-3.1.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/setup.cfg` & `aprsd-3.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/setup.py` & `aprsd-3.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/tests/cmds/test_send_message.py` & `aprsd-3.1.1/tests/cmds/test_send_message.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/tests/cmds/test_webchat.py` & `aprsd-3.1.1/tests/cmds/test_webchat.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/tests/fake.py` & `aprsd-3.1.1/tests/fake.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/tests/plugins/test_fortune.py` & `aprsd-3.1.1/tests/plugins/test_fortune.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/tests/plugins/test_location.py` & `aprsd-3.1.1/tests/plugins/test_location.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/tests/plugins/test_notify.py` & `aprsd-3.1.1/tests/plugins/test_notify.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/tests/plugins/test_ping.py` & `aprsd-3.1.1/tests/plugins/test_ping.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/tests/plugins/test_query.py` & `aprsd-3.1.1/tests/plugins/test_query.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/tests/plugins/test_time.py` & `aprsd-3.1.1/tests/plugins/test_time.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/tests/plugins/test_version.py` & `aprsd-3.1.1/tests/plugins/test_version.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/tests/plugins/test_weather.py` & `aprsd-3.1.1/tests/plugins/test_weather.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/tests/test_email.py` & `aprsd-3.1.1/tests/test_email.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/tests/test_main.py` & `aprsd-3.1.1/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/tests/test_packets.py` & `aprsd-3.1.1/tests/test_packets.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/tests/test_plugin.py` & `aprsd-3.1.1/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/tools/fast8.sh` & `aprsd-3.1.1/tools/fast8.sh`

 * *Files identical despite different names*

### Comparing `aprsd-3.1.0/tox.ini` & `aprsd-3.1.1/tox.ini`

 * *Files identical despite different names*

