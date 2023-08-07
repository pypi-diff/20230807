# Comparing `tmp/potnanny-0.1.3.tar.gz` & `tmp/potnanny-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "potnanny-0.1.3.tar", last modified: Sun Jul 30 19:41:33 2023, max compression
+gzip compressed data, was "potnanny-0.1.5.tar", last modified: Mon Aug  7 03:27:47 2023, max compression
```

## Comparing `potnanny-0.1.3.tar` & `potnanny-0.1.5.tar`

### file list

```diff
@@ -1,136 +1,136 @@
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-07-30 19:41:33.606073 potnanny-0.1.3/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)    35113 2023-07-28 04:26:10.000000 potnanny-0.1.3/LICENSE
--rw-rw-r--   0 jeff      (1000) jeff      (1000)       83 2023-07-30 08:13:55.000000 potnanny-0.1.3/MANIFEST.in
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     3215 2023-07-30 19:41:33.606073 potnanny-0.1.3/PKG-INFO
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     2926 2023-07-28 04:26:10.000000 potnanny-0.1.3/README.md
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-07-30 19:41:33.570071 potnanny-0.1.3/potnanny/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/__init__.py
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-07-30 19:41:33.578072 potnanny-0.1.3/potnanny/api/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     2676 2023-07-30 17:34:52.000000 potnanny-0.1.3/potnanny/api/__init__.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     2565 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/api/actions.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     2947 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/api/auth.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     2576 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/api/controls.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      488 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/api/decorators.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     5969 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/api/devices.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      954 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/api/environments.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      173 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/api/index.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     2712 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/api/keychains.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1449 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/api/plugins.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     2852 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/api/rooms.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     3113 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/api/schedules.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1874 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/api/settings.py
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-07-30 19:41:33.566071 potnanny-0.1.3/potnanny/api/static/
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-07-30 19:41:33.582072 potnanny-0.1.3/potnanny/api/static/css/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)    95609 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/api/static/css/bootstrap-icons.css
--rw-rw-r--   0 jeff      (1000) jeff      (1000)   155845 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/api/static/css/bootstrap.min.css
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-07-30 19:41:33.582072 potnanny-0.1.3/potnanny/api/static/css/fonts/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)   121296 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/api/static/css/fonts/bootstrap-icons.woff2
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-07-30 19:41:33.582072 potnanny-0.1.3/potnanny/api/static/htdocs/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     2948 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/api/static/htdocs/index.html
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-07-30 19:41:33.582072 potnanny-0.1.3/potnanny/api/static/js/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)   456323 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/api/static/js/app.js
--rw-rw-r--   0 jeff      (1000) jeff      (1000)    78743 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/api/static/js/bootstrap.bundle.min.js
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-07-30 19:41:33.582072 potnanny-0.1.3/potnanny/api/templates/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     3002 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/api/templates/index.html
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      695 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/api/tests.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     2423 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/api/users.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1449 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/api/utils.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1095 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/api/wifi.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1422 2023-07-30 15:23:44.000000 potnanny-0.1.3/potnanny/app.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     3014 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/cli.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     3239 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/config.py
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-07-30 19:41:33.586072 potnanny-0.1.3/potnanny/controllers/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/controllers/__init__.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      724 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/controllers/cleanup.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      574 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/controllers/device.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     4240 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/controllers/discover.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     3401 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/controllers/environment.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     3401 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/controllers/environment_orig.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     3468 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/controllers/graph.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     4693 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/controllers/outlet.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      843 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/controllers/pipeline.py
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-07-30 19:41:33.590072 potnanny-0.1.3/potnanny/controllers/poll/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)       45 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/controllers/poll/__init__.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     5135 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/controllers/poll/ble.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1532 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/controllers/poll/gpio.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     2479 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/controllers/poll/parse.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1904 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/controllers/poll/poll.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      706 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/controllers/schedule.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      849 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/controllers/trigger.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     3342 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/controllers/worker.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     3043 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/database.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)       73 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/events.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)       83 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/exc.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      662 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/locks.py
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-07-30 19:41:33.590072 potnanny-0.1.3/potnanny/models/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/models/__init__.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     3722 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/models/action.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     4055 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/models/control.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     5689 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/models/device.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1242 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/models/error.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1309 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/models/ext.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     3362 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/models/interface.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1372 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/models/keychain.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1253 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/models/measurement.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1354 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/models/mixins.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1693 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/models/room.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     3838 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/models/schedule.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      942 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/models/trigger.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1830 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/models/user.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1157 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/models/weekday.py
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-07-30 19:41:33.594072 potnanny-0.1.3/potnanny/plugins/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      320 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/plugins/__init__.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      906 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/plugins/base.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      267 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/plugins/category.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     4290 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/plugins/mixins.py
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-07-30 19:41:33.598073 potnanny-0.1.3/potnanny/utils/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      940 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/utils/__init__.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      887 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/utils/eval.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      332 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/utils/lists.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      798 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/utils/network.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      371 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/utils/numbers.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      227 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/utils/paths.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1263 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/utils/pids.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1285 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/utils/plugins.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      363 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/utils/pw.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     2206 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/utils/scanner.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      343 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/utils/serial.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      409 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/utils/shell.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      299 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/utils/temperature.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     2094 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/utils/times.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      822 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/utils/vpd.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     5323 2023-07-28 04:26:10.000000 potnanny-0.1.3/potnanny/utils/wifi.py
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-07-30 19:41:33.574072 potnanny-0.1.3/potnanny.egg-info/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     3215 2023-07-30 19:41:33.000000 potnanny-0.1.3/potnanny.egg-info/PKG-INFO
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     3172 2023-07-30 19:41:33.000000 potnanny-0.1.3/potnanny.egg-info/SOURCES.txt
--rw-rw-r--   0 jeff      (1000) jeff      (1000)        1 2023-07-30 19:41:33.000000 potnanny-0.1.3/potnanny.egg-info/dependency_links.txt
--rw-rw-r--   0 jeff      (1000) jeff      (1000)       47 2023-07-30 19:41:33.000000 potnanny-0.1.3/potnanny.egg-info/entry_points.txt
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      305 2023-07-30 19:41:33.000000 potnanny-0.1.3/potnanny.egg-info/requires.txt
--rw-rw-r--   0 jeff      (1000) jeff      (1000)        9 2023-07-30 19:41:33.000000 potnanny-0.1.3/potnanny.egg-info/top_level.txt
--rw-rw-r--   0 jeff      (1000) jeff      (1000)       38 2023-07-30 19:41:33.606073 potnanny-0.1.3/setup.cfg
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1243 2023-07-30 17:46:31.000000 potnanny-0.1.3/setup.py
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-07-30 19:41:33.606073 potnanny-0.1.3/tests/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     2721 2023-07-28 04:26:10.000000 potnanny-0.1.3/tests/test_ctrl_environments.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1431 2023-07-28 04:26:10.000000 potnanny-0.1.3/tests/test_ctrl_outlet.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      690 2023-07-28 04:26:10.000000 potnanny-0.1.3/tests/test_locks.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     3649 2023-07-28 04:26:10.000000 potnanny-0.1.3/tests/test_model_action.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1197 2023-07-28 04:26:10.000000 potnanny-0.1.3/tests/test_model_control.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1181 2023-07-28 04:26:10.000000 potnanny-0.1.3/tests/test_model_device.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1813 2023-07-28 04:26:10.000000 potnanny-0.1.3/tests/test_model_interface.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     2190 2023-07-28 04:26:10.000000 potnanny-0.1.3/tests/test_model_keychain.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      792 2023-07-28 04:26:10.000000 potnanny-0.1.3/tests/test_model_measurement.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      720 2023-07-28 04:26:10.000000 potnanny-0.1.3/tests/test_model_mixins.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1632 2023-07-28 04:26:10.000000 potnanny-0.1.3/tests/test_model_room.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1736 2023-07-28 04:26:10.000000 potnanny-0.1.3/tests/test_model_user.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      947 2023-07-28 04:26:10.000000 potnanny-0.1.3/tests/test_model_utils.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      767 2023-07-28 04:26:10.000000 potnanny-0.1.3/tests/test_pids.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     3138 2023-07-28 04:26:10.000000 potnanny-0.1.3/tests/test_queries.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      544 2023-07-28 04:26:10.000000 potnanny-0.1.3/tests/test_scanner.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      808 2023-07-28 04:26:10.000000 potnanny-0.1.3/tests/test_utils_eval.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      369 2023-07-28 04:26:10.000000 potnanny-0.1.3/tests/test_utils_lists.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      455 2023-07-28 04:26:10.000000 potnanny-0.1.3/tests/test_utils_numbers.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      333 2023-07-28 04:26:10.000000 potnanny-0.1.3/tests/test_utils_paths.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      428 2023-07-28 04:26:10.000000 potnanny-0.1.3/tests/test_utils_pw.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      450 2023-07-28 04:26:10.000000 potnanny-0.1.3/tests/test_utils_temperature.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      816 2023-07-28 04:26:10.000000 potnanny-0.1.3/tests/test_utils_times.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      326 2023-07-28 04:26:10.000000 potnanny-0.1.3/tests/test_utils_vpd.py
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-08-07 03:27:47.496472 potnanny-0.1.5/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)    35113 2023-07-28 04:26:10.000000 potnanny-0.1.5/LICENSE
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)       83 2023-07-30 08:13:55.000000 potnanny-0.1.5/MANIFEST.in
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     3215 2023-08-07 03:27:47.496472 potnanny-0.1.5/PKG-INFO
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     2926 2023-07-28 04:26:10.000000 potnanny-0.1.5/README.md
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-08-07 03:27:47.464472 potnanny-0.1.5/potnanny/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/__init__.py
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-08-07 03:27:47.472472 potnanny-0.1.5/potnanny/api/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     2675 2023-07-31 14:56:08.000000 potnanny-0.1.5/potnanny/api/__init__.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     2565 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/api/actions.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     2934 2023-08-07 03:23:48.000000 potnanny-0.1.5/potnanny/api/auth.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     2576 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/api/controls.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      488 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/api/decorators.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     5969 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/api/devices.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      954 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/api/environments.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      173 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/api/index.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     2712 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/api/keychains.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1449 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/api/plugins.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     2852 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/api/rooms.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     3113 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/api/schedules.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1874 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/api/settings.py
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-08-07 03:27:47.460472 potnanny-0.1.5/potnanny/api/static/
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-08-07 03:27:47.472472 potnanny-0.1.5/potnanny/api/static/css/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)    95609 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/api/static/css/bootstrap-icons.css
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)   155845 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/api/static/css/bootstrap.min.css
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-08-07 03:27:47.472472 potnanny-0.1.5/potnanny/api/static/css/fonts/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)   121296 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/api/static/css/fonts/bootstrap-icons.woff2
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-08-07 03:27:47.472472 potnanny-0.1.5/potnanny/api/static/htdocs/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     2948 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/api/static/htdocs/index.html
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-08-07 03:27:47.476472 potnanny-0.1.5/potnanny/api/static/js/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)   456333 2023-07-31 14:54:32.000000 potnanny-0.1.5/potnanny/api/static/js/app.js
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)    78743 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/api/static/js/bootstrap.bundle.min.js
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-08-07 03:27:47.476472 potnanny-0.1.5/potnanny/api/templates/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     3002 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/api/templates/index.html
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      695 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/api/tests.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     2423 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/api/users.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1449 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/api/utils.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1095 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/api/wifi.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1422 2023-07-30 15:23:44.000000 potnanny-0.1.5/potnanny/app.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     3014 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/cli.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     3239 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/config.py
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-08-07 03:27:47.480472 potnanny-0.1.5/potnanny/controllers/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/controllers/__init__.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      724 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/controllers/cleanup.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      574 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/controllers/device.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     4240 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/controllers/discover.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     3401 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/controllers/environment.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     3401 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/controllers/environment_orig.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     3468 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/controllers/graph.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     4693 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/controllers/outlet.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      843 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/controllers/pipeline.py
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-08-07 03:27:47.480472 potnanny-0.1.5/potnanny/controllers/poll/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)       45 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/controllers/poll/__init__.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     5135 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/controllers/poll/ble.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1532 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/controllers/poll/gpio.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     2479 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/controllers/poll/parse.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1904 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/controllers/poll/poll.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      706 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/controllers/schedule.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      849 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/controllers/trigger.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     3342 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/controllers/worker.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     3098 2023-08-07 03:21:30.000000 potnanny-0.1.5/potnanny/database.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)       73 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/events.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)       83 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/exc.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      662 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/locks.py
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-08-07 03:27:47.484472 potnanny-0.1.5/potnanny/models/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/models/__init__.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     3722 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/models/action.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     4055 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/models/control.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     5689 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/models/device.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1242 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/models/error.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1309 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/models/ext.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     3362 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/models/interface.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1372 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/models/keychain.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1253 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/models/measurement.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1354 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/models/mixins.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1693 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/models/room.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     3838 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/models/schedule.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      942 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/models/trigger.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1830 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/models/user.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1157 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/models/weekday.py
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-08-07 03:27:47.488472 potnanny-0.1.5/potnanny/plugins/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      320 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/plugins/__init__.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      906 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/plugins/base.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      267 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/plugins/category.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     4290 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/plugins/mixins.py
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-08-07 03:27:47.488472 potnanny-0.1.5/potnanny/utils/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      940 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/utils/__init__.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      887 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/utils/eval.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      332 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/utils/lists.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      798 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/utils/network.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      371 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/utils/numbers.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      227 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/utils/paths.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1263 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/utils/pids.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1285 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/utils/plugins.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      363 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/utils/pw.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     2206 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/utils/scanner.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      343 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/utils/serial.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      409 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/utils/shell.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      299 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/utils/temperature.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     2094 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/utils/times.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      822 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/utils/vpd.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     5323 2023-07-28 04:26:10.000000 potnanny-0.1.5/potnanny/utils/wifi.py
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-08-07 03:27:47.468472 potnanny-0.1.5/potnanny.egg-info/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     3215 2023-08-07 03:27:47.000000 potnanny-0.1.5/potnanny.egg-info/PKG-INFO
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     3172 2023-08-07 03:27:47.000000 potnanny-0.1.5/potnanny.egg-info/SOURCES.txt
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)        1 2023-08-07 03:27:47.000000 potnanny-0.1.5/potnanny.egg-info/dependency_links.txt
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)       47 2023-08-07 03:27:47.000000 potnanny-0.1.5/potnanny.egg-info/entry_points.txt
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      305 2023-08-07 03:27:47.000000 potnanny-0.1.5/potnanny.egg-info/requires.txt
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)        9 2023-08-07 03:27:47.000000 potnanny-0.1.5/potnanny.egg-info/top_level.txt
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)       38 2023-08-07 03:27:47.496472 potnanny-0.1.5/setup.cfg
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1243 2023-08-07 03:25:04.000000 potnanny-0.1.5/setup.py
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-08-07 03:27:47.496472 potnanny-0.1.5/tests/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     2721 2023-07-28 04:26:10.000000 potnanny-0.1.5/tests/test_ctrl_environments.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1431 2023-07-28 04:26:10.000000 potnanny-0.1.5/tests/test_ctrl_outlet.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      690 2023-07-28 04:26:10.000000 potnanny-0.1.5/tests/test_locks.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     3649 2023-07-28 04:26:10.000000 potnanny-0.1.5/tests/test_model_action.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1197 2023-07-28 04:26:10.000000 potnanny-0.1.5/tests/test_model_control.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1181 2023-07-28 04:26:10.000000 potnanny-0.1.5/tests/test_model_device.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1813 2023-07-28 04:26:10.000000 potnanny-0.1.5/tests/test_model_interface.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     2190 2023-07-28 04:26:10.000000 potnanny-0.1.5/tests/test_model_keychain.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      792 2023-07-28 04:26:10.000000 potnanny-0.1.5/tests/test_model_measurement.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      720 2023-07-28 04:26:10.000000 potnanny-0.1.5/tests/test_model_mixins.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1632 2023-07-28 04:26:10.000000 potnanny-0.1.5/tests/test_model_room.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1736 2023-07-28 04:26:10.000000 potnanny-0.1.5/tests/test_model_user.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      947 2023-07-28 04:26:10.000000 potnanny-0.1.5/tests/test_model_utils.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      767 2023-07-28 04:26:10.000000 potnanny-0.1.5/tests/test_pids.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     3138 2023-07-28 04:26:10.000000 potnanny-0.1.5/tests/test_queries.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      544 2023-07-28 04:26:10.000000 potnanny-0.1.5/tests/test_scanner.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      808 2023-07-28 04:26:10.000000 potnanny-0.1.5/tests/test_utils_eval.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      369 2023-07-28 04:26:10.000000 potnanny-0.1.5/tests/test_utils_lists.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      455 2023-07-28 04:26:10.000000 potnanny-0.1.5/tests/test_utils_numbers.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      333 2023-07-28 04:26:10.000000 potnanny-0.1.5/tests/test_utils_paths.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      428 2023-07-28 04:26:10.000000 potnanny-0.1.5/tests/test_utils_pw.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      450 2023-07-28 04:26:10.000000 potnanny-0.1.5/tests/test_utils_temperature.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      816 2023-07-28 04:26:10.000000 potnanny-0.1.5/tests/test_utils_times.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      326 2023-07-28 04:26:10.000000 potnanny-0.1.5/tests/test_utils_vpd.py
```

### Comparing `potnanny-0.1.3/LICENSE` & `potnanny-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/PKG-INFO` & `potnanny-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: potnanny
-Version: 0.1.3
+Version: 0.1.5
 Summary: Potnanny grow room automation controller.
 Home-page: https://github.com/potnanny/application
 Author: J Leary
 Author-email: potnanny@gmail.com
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `potnanny-0.1.3/README.md` & `potnanny-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/potnanny/api/__init__.py` & `potnanny-0.1.5/potnanny/api/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
     # session cookie storage
     key = Fernet.generate_key()
     secret = base64.urlsafe_b64decode(key)
     setup(app, EncryptedCookieStorage(secret,
         cookie_name='POTNANNY_API',
         samesite="None",
-        secure=False
+        secure=True
         )
     )
 
     # simple cookie storage for devel ONLY
     # setup(app, SimpleCookieStorage())
 
     # plug in jinja template handling
```

### Comparing `potnanny-0.1.3/potnanny/api/actions.py` & `potnanny-0.1.5/potnanny/api/actions.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/potnanny/api/auth.py` & `potnanny-0.1.5/potnanny/api/auth.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,29 +23,27 @@
     session['username'] = user.name
     session['roles'] = user.roles
     session.changed()
 
     resp = web.json_response({
         "status": "ok", "msg": "authenticated ok"}, status=200)
 
-    """
     # for optional features
     try:
         kc = await ObjectInterface(Keychain).get_by_name('features')
-        ck = {
+        opts = {
             'username': user.name,
-            'roles': user.roles }
+            'roles': user.roles,
+            'room_limit': kc.attributes['room_limit'],
+            'device_limit': kc.attributes['device_limit'] }
 
-        ck['room_limit'] = kc.attributes['room_limit']
-        ck['device_limit'] = kc.attributes['device_limit']
-        resp.set_cookie("POTNANNY", ck, samesite="None", secure=False)
+        resp.set_cookie("POTNANNY", opts, samesite="None", secure=True)
     except Exception as x:
         logger.warning(x)
         pass
-    """
 
     return resp
 
 
 @routes.post('/api/v1.0/logout')
 @login_required
 async def logout(request):
```

### Comparing `potnanny-0.1.3/potnanny/api/controls.py` & `potnanny-0.1.5/potnanny/api/controls.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/potnanny/api/devices.py` & `potnanny-0.1.5/potnanny/api/devices.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/potnanny/api/environments.py` & `potnanny-0.1.5/potnanny/api/environments.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/potnanny/api/keychains.py` & `potnanny-0.1.5/potnanny/api/keychains.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/potnanny/api/plugins.py` & `potnanny-0.1.5/potnanny/api/plugins.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/potnanny/api/rooms.py` & `potnanny-0.1.5/potnanny/api/rooms.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/potnanny/api/schedules.py` & `potnanny-0.1.5/potnanny/api/schedules.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/potnanny/api/settings.py` & `potnanny-0.1.5/potnanny/api/settings.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/potnanny/api/static/css/bootstrap-icons.css` & `potnanny-0.1.5/potnanny/api/static/css/bootstrap-icons.css`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/potnanny/api/static/css/bootstrap.min.css` & `potnanny-0.1.5/potnanny/api/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/potnanny/api/static/css/fonts/bootstrap-icons.woff2` & `potnanny-0.1.5/potnanny/api/static/css/fonts/bootstrap-icons.woff2`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/potnanny/api/static/htdocs/index.html` & `potnanny-0.1.5/potnanny/api/static/htdocs/index.html`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/potnanny/api/static/js/app.js` & `potnanny-0.1.5/potnanny/api/static/js/app.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1490,20 +1490,22 @@
                     a = s.showModal,
                     c = s.activeModal,
                     l = r(80325).API_URL;
                 t.exports = {
                     deviceForm: function(t) {
                         i.load(t);
                         var e = n("form", {
-                            onsubmit: function(t) {
-                                return t.preventDefault(), c.hide(), i.save(), i.current = {}, n.request({
+                            onsubmit: function(e) {
+                                return e.preventDefault(), c.hide(), i.save(), n.request({
                                     method: "POST",
-                                    url: l + "/devices/" + i.current.id + "/poll",
+                                    url: l + "/devices/" + t + "/poll",
                                     withCredentials: !0
-                                })
+                                }).then((function(t) {
+                                    i.current = {}
+                                }))
                             }
                         }, [n("input[type=text][required].form-control", {
                             id: "name",
                             value: i.current.name,
                             onchange: function(t) {
                                 i.current.name = t.target.value
                             }
```

### Comparing `potnanny-0.1.3/potnanny/api/static/js/bootstrap.bundle.min.js` & `potnanny-0.1.5/potnanny/api/static/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/potnanny/api/templates/index.html` & `potnanny-0.1.5/potnanny/api/templates/index.html`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/potnanny/api/tests.py` & `potnanny-0.1.5/potnanny/api/tests.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/potnanny/api/users.py` & `potnanny-0.1.5/potnanny/api/users.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/potnanny/api/utils.py` & `potnanny-0.1.5/potnanny/api/utils.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/potnanny/api/wifi.py` & `potnanny-0.1.5/potnanny/api/wifi.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/potnanny/app.py` & `potnanny-0.1.5/potnanny/app.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/potnanny/cli.py` & `potnanny-0.1.5/potnanny/cli.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/potnanny/config.py` & `potnanny-0.1.5/potnanny/config.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/potnanny/controllers/cleanup.py` & `potnanny-0.1.5/potnanny/controllers/cleanup.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/potnanny/controllers/device.py` & `potnanny-0.1.5/potnanny/controllers/device.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/potnanny/controllers/discover.py` & `potnanny-0.1.5/potnanny/controllers/discover.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/potnanny/controllers/environment.py` & `potnanny-0.1.5/potnanny/controllers/environment.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/potnanny/controllers/environment_orig.py` & `potnanny-0.1.5/potnanny/controllers/environment_orig.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/potnanny/controllers/graph.py` & `potnanny-0.1.5/potnanny/controllers/graph.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/potnanny/controllers/outlet.py` & `potnanny-0.1.5/potnanny/controllers/outlet.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/potnanny/controllers/pipeline.py` & `potnanny-0.1.5/potnanny/controllers/pipeline.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/potnanny/controllers/poll/ble.py` & `potnanny-0.1.5/potnanny/controllers/poll/ble.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/potnanny/controllers/poll/gpio.py` & `potnanny-0.1.5/potnanny/controllers/poll/gpio.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/potnanny/controllers/poll/parse.py` & `potnanny-0.1.5/potnanny/controllers/poll/parse.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/potnanny/controllers/poll/poll.py` & `potnanny-0.1.5/potnanny/controllers/poll/poll.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/potnanny/controllers/schedule.py` & `potnanny-0.1.5/potnanny/controllers/schedule.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/potnanny/controllers/trigger.py` & `potnanny-0.1.5/potnanny/controllers/trigger.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/potnanny/controllers/worker.py` & `potnanny-0.1.5/potnanny/controllers/worker.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/potnanny/database.py` & `potnanny-0.1.5/potnanny/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,14 +85,18 @@
     from potnanny.models.action import Action
     from potnanny.models.trigger import Trigger
 
     # create tables
     async with engine.begin() as conn:
         await conn.run_sync(Base.metadata.create_all)
 
+    await init_features()
+
+
+async def init_features():
     # create initial default config
     try:
         attrs = {
             'temperature_display': 'F',
             'polling_interval': 10,
             'plugin_path': os.path.expanduser('~/potnanny/plugins'),
             'leaf_offset': -2,
```

### Comparing `potnanny-0.1.3/potnanny/locks.py` & `potnanny-0.1.5/potnanny/locks.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/potnanny/models/action.py` & `potnanny-0.1.5/potnanny/models/action.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/potnanny/models/control.py` & `potnanny-0.1.5/potnanny/models/control.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/potnanny/models/device.py` & `potnanny-0.1.5/potnanny/models/device.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/potnanny/models/error.py` & `potnanny-0.1.5/potnanny/models/error.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/potnanny/models/ext.py` & `potnanny-0.1.5/potnanny/models/ext.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/potnanny/models/interface.py` & `potnanny-0.1.5/potnanny/models/interface.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/potnanny/models/keychain.py` & `potnanny-0.1.5/potnanny/models/keychain.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/potnanny/models/measurement.py` & `potnanny-0.1.5/potnanny/models/measurement.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/potnanny/models/mixins.py` & `potnanny-0.1.5/potnanny/models/mixins.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/potnanny/models/room.py` & `potnanny-0.1.5/potnanny/models/room.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/potnanny/models/schedule.py` & `potnanny-0.1.5/potnanny/models/schedule.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/potnanny/models/trigger.py` & `potnanny-0.1.5/potnanny/models/trigger.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/potnanny/models/user.py` & `potnanny-0.1.5/potnanny/models/user.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/potnanny/models/weekday.py` & `potnanny-0.1.5/potnanny/models/weekday.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/potnanny/plugins/base.py` & `potnanny-0.1.5/potnanny/plugins/base.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/potnanny/plugins/mixins.py` & `potnanny-0.1.5/potnanny/plugins/mixins.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/potnanny/utils/__init__.py` & `potnanny-0.1.5/potnanny/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/potnanny/utils/eval.py` & `potnanny-0.1.5/potnanny/utils/eval.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/potnanny/utils/network.py` & `potnanny-0.1.5/potnanny/utils/network.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/potnanny/utils/pids.py` & `potnanny-0.1.5/potnanny/utils/pids.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/potnanny/utils/plugins.py` & `potnanny-0.1.5/potnanny/utils/plugins.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/potnanny/utils/scanner.py` & `potnanny-0.1.5/potnanny/utils/scanner.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/potnanny/utils/times.py` & `potnanny-0.1.5/potnanny/utils/times.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/potnanny/utils/vpd.py` & `potnanny-0.1.5/potnanny/utils/vpd.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/potnanny/utils/wifi.py` & `potnanny-0.1.5/potnanny/utils/wifi.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/potnanny.egg-info/PKG-INFO` & `potnanny-0.1.5/potnanny.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: potnanny
-Version: 0.1.3
+Version: 0.1.5
 Summary: Potnanny grow room automation controller.
 Home-page: https://github.com/potnanny/application
 Author: J Leary
 Author-email: potnanny@gmail.com
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `potnanny-0.1.3/potnanny.egg-info/SOURCES.txt` & `potnanny-0.1.5/potnanny.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/setup.py` & `potnanny-0.1.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='potnanny',
-    version='0.1.3',
+    version='0.1.5',
     python_requires=">=3.9",
     packages=setuptools.find_packages(),
     include_package_data=True,
     description='Potnanny grow room automation controller.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='J Leary',
```

### Comparing `potnanny-0.1.3/tests/test_ctrl_environments.py` & `potnanny-0.1.5/tests/test_ctrl_environments.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/tests/test_ctrl_outlet.py` & `potnanny-0.1.5/tests/test_ctrl_outlet.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/tests/test_locks.py` & `potnanny-0.1.5/tests/test_locks.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/tests/test_model_action.py` & `potnanny-0.1.5/tests/test_model_action.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/tests/test_model_control.py` & `potnanny-0.1.5/tests/test_model_control.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/tests/test_model_device.py` & `potnanny-0.1.5/tests/test_model_device.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/tests/test_model_interface.py` & `potnanny-0.1.5/tests/test_model_interface.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/tests/test_model_keychain.py` & `potnanny-0.1.5/tests/test_model_keychain.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/tests/test_model_measurement.py` & `potnanny-0.1.5/tests/test_model_measurement.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/tests/test_model_mixins.py` & `potnanny-0.1.5/tests/test_model_mixins.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/tests/test_model_room.py` & `potnanny-0.1.5/tests/test_model_room.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/tests/test_model_user.py` & `potnanny-0.1.5/tests/test_model_user.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/tests/test_model_utils.py` & `potnanny-0.1.5/tests/test_model_utils.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/tests/test_pids.py` & `potnanny-0.1.5/tests/test_pids.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/tests/test_queries.py` & `potnanny-0.1.5/tests/test_queries.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/tests/test_scanner.py` & `potnanny-0.1.5/tests/test_scanner.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/tests/test_utils_eval.py` & `potnanny-0.1.5/tests/test_utils_eval.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.3/tests/test_utils_times.py` & `potnanny-0.1.5/tests/test_utils_times.py`

 * *Files identical despite different names*

