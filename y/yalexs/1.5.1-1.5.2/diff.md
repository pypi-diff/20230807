# Comparing `tmp/yalexs-1.5.1.tar.gz` & `tmp/yalexs-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yalexs-1.5.1.tar", last modified: Mon May 22 13:47:56 2023, max compression
+gzip compressed data, was "yalexs-1.5.2.tar", last modified: Sun Aug  6 22:09:22 2023, max compression
```

## Comparing `yalexs-1.5.1.tar` & `yalexs-1.5.2.tar`

### file list

```diff
@@ -1,102 +1,104 @@
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-22 13:47:56.159559 yalexs-1.5.1/
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-22 13:47:56.144459 yalexs-1.5.1/.github/
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-22 13:47:56.147228 yalexs-1.5.1/.github/workflows/
--rw-r--r--   0 bdraco     (501) staff       (20)     2254 2023-05-17 14:08:38.000000 yalexs-1.5.1/.github/workflows/ci.yaml
--rw-r--r--   0 bdraco     (501) staff       (20)     1180 2023-02-17 14:03:03.000000 yalexs-1.5.1/.gitignore
--rw-r--r--   0 bdraco     (501) staff       (20)     1063 2023-02-17 14:03:03.000000 yalexs-1.5.1/LICENSE
--rw-r--r--   0 bdraco     (501) staff       (20)      398 2023-02-17 14:03:03.000000 yalexs-1.5.1/MANIFEST
--rw-r--r--   0 bdraco     (501) staff       (20)      666 2023-05-22 13:47:56.159633 yalexs-1.5.1/PKG-INFO
--rw-r--r--   0 bdraco     (501) staff       (20)     4569 2023-02-17 14:03:03.000000 yalexs-1.5.1/README.md
--rw-r--r--   0 bdraco     (501) staff       (20)       66 2023-02-17 14:03:03.000000 yalexs-1.5.1/build.sh
--rw-r--r--   0 bdraco     (501) staff       (20)     4283 2023-02-17 14:03:03.000000 yalexs-1.5.1/known_activities.md
--rw-r--r--   0 bdraco     (501) staff       (20)     1337 2023-02-17 14:03:03.000000 yalexs-1.5.1/pylintrc
--rw-r--r--   0 bdraco     (501) staff       (20)       91 2023-05-17 14:08:38.000000 yalexs-1.5.1/requirements.txt
--rw-r--r--   0 bdraco     (501) staff       (20)      141 2023-05-22 13:33:40.000000 yalexs-1.5.1/requirements_tests.txt
--rw-r--r--   0 bdraco     (501) staff       (20)      886 2023-05-22 13:47:56.159902 yalexs-1.5.1/setup.cfg
--rw-r--r--   0 bdraco     (501) staff       (20)     1054 2023-05-22 13:47:41.000000 yalexs-1.5.1/setup.py
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-22 13:47:56.149159 yalexs-1.5.1/tests/
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-22 13:47:56.155481 yalexs-1.5.1/tests/fixtures/
--rw-r--r--   0 bdraco     (501) staff       (20)      311 2023-02-17 14:03:03.000000 yalexs-1.5.1/tests/fixtures/auto_lock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      926 2023-02-17 14:03:03.000000 yalexs-1.5.1/tests/fixtures/auto_relock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      918 2023-02-17 14:03:03.000000 yalexs-1.5.1/tests/fixtures/auto_unlock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1331 2023-02-17 14:03:03.000000 yalexs-1.5.1/tests/fixtures/bluetooth_lock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      774 2023-02-17 14:03:03.000000 yalexs-1.5.1/tests/fixtures/door_closed_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      777 2023-02-17 14:03:03.000000 yalexs-1.5.1/tests/fixtures/door_closed_activity_wrong_deviceid.json
--rw-r--r--   0 bdraco     (501) staff       (20)      780 2023-02-17 14:03:03.000000 yalexs-1.5.1/tests/fixtures/door_closed_activity_wrong_houseid.json
--rw-r--r--   0 bdraco     (501) staff       (20)      772 2023-02-17 14:03:03.000000 yalexs-1.5.1/tests/fixtures/door_open_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1475 2023-02-17 14:03:03.000000 yalexs-1.5.1/tests/fixtures/doorbell_motion_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      907 2023-02-17 14:03:03.000000 yalexs-1.5.1/tests/fixtures/doorbell_motion_activity_no_image.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1501 2023-02-17 14:03:03.000000 yalexs-1.5.1/tests/fixtures/doorbell_motion_activity_old.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1495 2023-02-17 14:03:03.000000 yalexs-1.5.1/tests/fixtures/doorbell_motion_activity_wrong.json
--rw-r--r--   0 bdraco     (501) staff       (20)     3198 2023-02-17 14:03:03.000000 yalexs-1.5.1/tests/fixtures/get_doorbell.battery_full.json
--rw-r--r--   0 bdraco     (501) staff       (20)     3188 2023-02-17 14:03:03.000000 yalexs-1.5.1/tests/fixtures/get_doorbell.battery_low.json
--rw-r--r--   0 bdraco     (501) staff       (20)     3197 2023-02-17 14:03:03.000000 yalexs-1.5.1/tests/fixtures/get_doorbell.battery_medium.json
--rw-r--r--   0 bdraco     (501) staff       (20)     2488 2023-02-17 14:03:03.000000 yalexs-1.5.1/tests/fixtures/get_doorbell.json
--rw-r--r--   0 bdraco     (501) staff       (20)     3780 2023-02-17 14:03:03.000000 yalexs-1.5.1/tests/fixtures/get_doorbell.offline.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1898 2023-02-17 14:03:03.000000 yalexs-1.5.1/tests/fixtures/get_doorbell_missing_image.json
--rw-r--r--   0 bdraco     (501) staff       (20)     2255 2023-02-17 14:03:03.000000 yalexs-1.5.1/tests/fixtures/get_doorbells.json
--rw-r--r--   0 bdraco     (501) staff       (20)     9741 2023-02-17 14:03:03.000000 yalexs-1.5.1/tests/fixtures/get_house_activities.json
--rw-r--r--   0 bdraco     (501) staff       (20)     2744 2023-02-17 14:03:03.000000 yalexs-1.5.1/tests/fixtures/get_lock.doorsense_init.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1182 2023-02-17 14:03:03.000000 yalexs-1.5.1/tests/fixtures/get_lock.nostatus_with_doorsense.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1680 2023-02-17 14:03:03.000000 yalexs-1.5.1/tests/fixtures/get_lock.offline.json
--rw-r--r--   0 bdraco     (501) staff       (20)     2745 2023-02-17 14:03:03.000000 yalexs-1.5.1/tests/fixtures/get_lock.online.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1368 2023-02-17 14:03:03.000000 yalexs-1.5.1/tests/fixtures/get_lock.online_with_doorsense.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1373 2023-02-17 14:03:03.000000 yalexs-1.5.1/tests/fixtures/get_lock.online_with_doorsense_disabled.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1633 2023-02-17 14:03:03.000000 yalexs-1.5.1/tests/fixtures/get_lock_v2.online.json
--rw-r--r--   0 bdraco     (501) staff       (20)      408 2023-02-17 14:03:03.000000 yalexs-1.5.1/tests/fixtures/get_locks.json
--rw-r--r--   0 bdraco     (501) staff       (20)      664 2023-02-17 14:03:03.000000 yalexs-1.5.1/tests/fixtures/get_pins.json
--rw-r--r--   0 bdraco     (501) staff       (20)      848 2023-02-17 14:03:03.000000 yalexs-1.5.1/tests/fixtures/keypad_lock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      682 2023-02-17 14:03:03.000000 yalexs-1.5.1/tests/fixtures/lock.json
--rw-r--r--   0 bdraco     (501) staff       (20)      800 2023-02-17 14:03:03.000000 yalexs-1.5.1/tests/fixtures/lock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      641 2023-02-17 14:03:03.000000 yalexs-1.5.1/tests/fixtures/lock_without_doorstate.json
--rw-r--r--   0 bdraco     (501) staff       (20)      315 2023-02-17 14:03:03.000000 yalexs-1.5.1/tests/fixtures/manual_lock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      321 2023-02-17 14:03:03.000000 yalexs-1.5.1/tests/fixtures/manual_unlock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      458 2023-02-17 14:03:03.000000 yalexs-1.5.1/tests/fixtures/pin_unlock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      409 2023-02-17 14:03:03.000000 yalexs-1.5.1/tests/fixtures/pin_unlock_activity_missing_image.json
--rw-r--r--   0 bdraco     (501) staff       (20)      479 2023-02-17 14:03:03.000000 yalexs-1.5.1/tests/fixtures/pin_unlock_activity_with_image.json
--rw-r--r--   0 bdraco     (501) staff       (20)      827 2023-02-17 14:03:03.000000 yalexs-1.5.1/tests/fixtures/remote_lock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      435 2023-02-17 14:03:03.000000 yalexs-1.5.1/tests/fixtures/remote_lock_activity_v4.json
--rw-r--r--   0 bdraco     (501) staff       (20)      441 2023-02-17 14:03:03.000000 yalexs-1.5.1/tests/fixtures/remote_unlock_activity_v4.json
--rw-r--r--   0 bdraco     (501) staff       (20)      559 2023-02-17 14:03:03.000000 yalexs-1.5.1/tests/fixtures/remote_unlock_activity_v4_2.json
--rw-r--r--   0 bdraco     (501) staff       (20)      686 2023-02-17 14:03:03.000000 yalexs-1.5.1/tests/fixtures/unlock.json
--rw-r--r--   0 bdraco     (501) staff       (20)      732 2023-02-17 14:03:03.000000 yalexs-1.5.1/tests/fixtures/unlock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      648 2023-02-17 14:03:03.000000 yalexs-1.5.1/tests/fixtures/unlock_without_doorstate.json
--rw-r--r--   0 bdraco     (501) staff       (20)    14818 2023-05-17 14:08:38.000000 yalexs-1.5.1/tests/test_activity.py
--rw-r--r--   0 bdraco     (501) staff       (20)    33779 2023-05-17 14:08:38.000000 yalexs-1.5.1/tests/test_api.py
--rw-r--r--   0 bdraco     (501) staff       (20)    42924 2023-05-17 21:45:20.000000 yalexs-1.5.1/tests/test_api_async.py
--rw-r--r--   0 bdraco     (501) staff       (20)     7495 2023-02-17 14:03:03.000000 yalexs-1.5.1/tests/test_authenticator.py
--rw-r--r--   0 bdraco     (501) staff       (20)     8968 2023-05-17 14:08:38.000000 yalexs-1.5.1/tests/test_authenticator_async.py
--rw-r--r--   0 bdraco     (501) staff       (20)    17841 2023-05-18 17:20:56.000000 yalexs-1.5.1/tests/test_pubnub_activity.py
--rw-r--r--   0 bdraco     (501) staff       (20)    15595 2023-05-22 13:33:40.000000 yalexs-1.5.1/tests/test_util.py
--rw-r--r--   0 bdraco     (501) staff       (20)     1316 2023-02-17 14:33:57.000000 yalexs-1.5.1/tox.ini
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-22 13:47:56.158749 yalexs-1.5.1/yalexs/
--rw-r--r--   0 bdraco     (501) staff       (20)      114 2023-05-22 13:47:41.000000 yalexs-1.5.1/yalexs/__init__.py
--rw-r--r--   0 bdraco     (501) staff       (20)    14170 2023-05-22 13:33:40.000000 yalexs-1.5.1/yalexs/activity.py
--rw-r--r--   0 bdraco     (501) staff       (20)     9979 2023-05-17 18:54:43.000000 yalexs-1.5.1/yalexs/api.py
--rw-r--r--   0 bdraco     (501) staff       (20)    15152 2023-05-22 13:47:36.000000 yalexs-1.5.1/yalexs/api_async.py
--rw-r--r--   0 bdraco     (501) staff       (20)    11644 2023-05-22 13:33:40.000000 yalexs-1.5.1/yalexs/api_common.py
--rw-r--r--   0 bdraco     (501) staff       (20)     4838 2023-05-17 14:08:38.000000 yalexs-1.5.1/yalexs/authenticator.py
--rw-r--r--   0 bdraco     (501) staff       (20)     5306 2023-05-17 18:44:25.000000 yalexs-1.5.1/yalexs/authenticator_async.py
--rw-r--r--   0 bdraco     (501) staff       (20)     5282 2023-05-22 13:33:40.000000 yalexs-1.5.1/yalexs/authenticator_common.py
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-22 13:47:56.159438 yalexs-1.5.1/yalexs/backports/
--rw-r--r--   0 bdraco     (501) staff       (20)        0 2023-05-17 14:08:38.000000 yalexs-1.5.1/yalexs/backports/__init__.py
--rw-r--r--   0 bdraco     (501) staff       (20)     1020 2023-05-17 14:08:38.000000 yalexs-1.5.1/yalexs/backports/enum.py
--rw-r--r--   0 bdraco     (501) staff       (20)     1846 2023-05-18 17:02:22.000000 yalexs-1.5.1/yalexs/bridge.py
--rw-r--r--   0 bdraco     (501) staff       (20)     1283 2023-05-22 13:33:40.000000 yalexs-1.5.1/yalexs/const.py
--rw-r--r--   0 bdraco     (501) staff       (20)     1399 2023-02-17 14:03:03.000000 yalexs-1.5.1/yalexs/device.py
--rw-r--r--   0 bdraco     (501) staff       (20)     4251 2023-05-22 13:33:40.000000 yalexs-1.5.1/yalexs/doorbell.py
--rw-r--r--   0 bdraco     (501) staff       (20)      776 2023-05-17 21:45:20.000000 yalexs-1.5.1/yalexs/exceptions.py
--rw-r--r--   0 bdraco     (501) staff       (20)     1044 2023-05-18 17:02:22.000000 yalexs-1.5.1/yalexs/keypad.py
--rw-r--r--   0 bdraco     (501) staff       (20)     7922 2023-05-22 13:33:40.000000 yalexs-1.5.1/yalexs/lock.py
--rw-r--r--   0 bdraco     (501) staff       (20)     2403 2023-05-22 13:33:40.000000 yalexs-1.5.1/yalexs/pin.py
--rw-r--r--   0 bdraco     (501) staff       (20)     4555 2023-05-17 21:25:12.000000 yalexs-1.5.1/yalexs/pubnub_activity.py
--rw-r--r--   0 bdraco     (501) staff       (20)     4484 2023-05-22 13:11:27.000000 yalexs-1.5.1/yalexs/pubnub_async.py
--rw-r--r--   0 bdraco     (501) staff       (20)      298 2023-05-22 13:33:40.000000 yalexs-1.5.1/yalexs/time.py
--rw-r--r--   0 bdraco     (501) staff       (20)     1088 2023-02-17 14:03:03.000000 yalexs-1.5.1/yalexs/users.py
--rw-r--r--   0 bdraco     (501) staff       (20)     3913 2023-05-22 13:33:40.000000 yalexs-1.5.1/yalexs/util.py
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-22 13:47:56.159251 yalexs-1.5.1/yalexs.egg-info/
--rw-r--r--   0 bdraco     (501) staff       (20)      666 2023-05-22 13:47:56.000000 yalexs-1.5.1/yalexs.egg-info/PKG-INFO
--rw-r--r--   0 bdraco     (501) staff       (20)     2884 2023-05-22 13:47:56.000000 yalexs-1.5.1/yalexs.egg-info/SOURCES.txt
--rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-05-22 13:47:56.000000 yalexs-1.5.1/yalexs.egg-info/dependency_links.txt
--rw-r--r--   0 bdraco     (501) staff       (20)      107 2023-05-22 13:47:56.000000 yalexs-1.5.1/yalexs.egg-info/requires.txt
--rw-r--r--   0 bdraco     (501) staff       (20)        7 2023-05-22 13:47:56.000000 yalexs-1.5.1/yalexs.egg-info/top_level.txt
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-08-06 22:09:22.223002 yalexs-1.5.2/
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-08-06 22:09:22.207411 yalexs-1.5.2/.github/
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-08-06 22:09:22.209977 yalexs-1.5.2/.github/workflows/
+-rw-r--r--   0 bdraco     (501) staff       (20)     2254 2023-05-17 14:08:38.000000 yalexs-1.5.2/.github/workflows/ci.yaml
+-rw-r--r--   0 bdraco     (501) staff       (20)     1180 2023-02-17 14:03:03.000000 yalexs-1.5.2/.gitignore
+-rw-r--r--   0 bdraco     (501) staff       (20)     1063 2023-02-17 14:03:03.000000 yalexs-1.5.2/LICENSE
+-rw-r--r--   0 bdraco     (501) staff       (20)      398 2023-02-17 14:03:03.000000 yalexs-1.5.2/MANIFEST
+-rw-r--r--   0 bdraco     (501) staff       (20)      666 2023-08-06 22:09:22.223077 yalexs-1.5.2/PKG-INFO
+-rw-r--r--   0 bdraco     (501) staff       (20)     4569 2023-02-17 14:03:03.000000 yalexs-1.5.2/README.md
+-rw-r--r--   0 bdraco     (501) staff       (20)       66 2023-02-17 14:03:03.000000 yalexs-1.5.2/build.sh
+-rw-r--r--   0 bdraco     (501) staff       (20)     4283 2023-02-17 14:03:03.000000 yalexs-1.5.2/known_activities.md
+-rw-r--r--   0 bdraco     (501) staff       (20)     1337 2023-02-17 14:03:03.000000 yalexs-1.5.2/pylintrc
+-rw-r--r--   0 bdraco     (501) staff       (20)       91 2023-05-17 14:08:38.000000 yalexs-1.5.2/requirements.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)      141 2023-05-22 13:33:40.000000 yalexs-1.5.2/requirements_tests.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)      886 2023-08-06 22:09:22.223352 yalexs-1.5.2/setup.cfg
+-rw-r--r--   0 bdraco     (501) staff       (20)     1054 2023-08-06 22:09:07.000000 yalexs-1.5.2/setup.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-08-06 22:09:22.211885 yalexs-1.5.2/tests/
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-08-06 22:09:22.218081 yalexs-1.5.2/tests/fixtures/
+-rw-r--r--   0 bdraco     (501) staff       (20)      311 2023-02-17 14:03:03.000000 yalexs-1.5.2/tests/fixtures/auto_lock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      926 2023-02-17 14:03:03.000000 yalexs-1.5.2/tests/fixtures/auto_relock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      918 2023-02-17 14:03:03.000000 yalexs-1.5.2/tests/fixtures/auto_unlock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1331 2023-02-17 14:03:03.000000 yalexs-1.5.2/tests/fixtures/bluetooth_lock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      774 2023-02-17 14:03:03.000000 yalexs-1.5.2/tests/fixtures/door_closed_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      777 2023-02-17 14:03:03.000000 yalexs-1.5.2/tests/fixtures/door_closed_activity_wrong_deviceid.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      780 2023-02-17 14:03:03.000000 yalexs-1.5.2/tests/fixtures/door_closed_activity_wrong_houseid.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      772 2023-02-17 14:03:03.000000 yalexs-1.5.2/tests/fixtures/door_open_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1475 2023-02-17 14:03:03.000000 yalexs-1.5.2/tests/fixtures/doorbell_motion_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      907 2023-02-17 14:03:03.000000 yalexs-1.5.2/tests/fixtures/doorbell_motion_activity_no_image.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1501 2023-02-17 14:03:03.000000 yalexs-1.5.2/tests/fixtures/doorbell_motion_activity_old.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1495 2023-02-17 14:03:03.000000 yalexs-1.5.2/tests/fixtures/doorbell_motion_activity_wrong.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     3198 2023-02-17 14:03:03.000000 yalexs-1.5.2/tests/fixtures/get_doorbell.battery_full.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     3188 2023-02-17 14:03:03.000000 yalexs-1.5.2/tests/fixtures/get_doorbell.battery_low.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     3197 2023-02-17 14:03:03.000000 yalexs-1.5.2/tests/fixtures/get_doorbell.battery_medium.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     2488 2023-02-17 14:03:03.000000 yalexs-1.5.2/tests/fixtures/get_doorbell.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     3780 2023-02-17 14:03:03.000000 yalexs-1.5.2/tests/fixtures/get_doorbell.offline.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1898 2023-02-17 14:03:03.000000 yalexs-1.5.2/tests/fixtures/get_doorbell_missing_image.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     2255 2023-02-17 14:03:03.000000 yalexs-1.5.2/tests/fixtures/get_doorbells.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     9741 2023-02-17 14:03:03.000000 yalexs-1.5.2/tests/fixtures/get_house_activities.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     2744 2023-02-17 14:03:03.000000 yalexs-1.5.2/tests/fixtures/get_lock.doorsense_init.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1182 2023-02-17 14:03:03.000000 yalexs-1.5.2/tests/fixtures/get_lock.nostatus_with_doorsense.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1680 2023-02-17 14:03:03.000000 yalexs-1.5.2/tests/fixtures/get_lock.offline.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     2745 2023-02-17 14:03:03.000000 yalexs-1.5.2/tests/fixtures/get_lock.online.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1368 2023-02-17 14:03:03.000000 yalexs-1.5.2/tests/fixtures/get_lock.online_with_doorsense.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1373 2023-02-17 14:03:03.000000 yalexs-1.5.2/tests/fixtures/get_lock.online_with_doorsense_disabled.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1633 2023-02-17 14:03:03.000000 yalexs-1.5.2/tests/fixtures/get_lock_v2.online.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      408 2023-02-17 14:03:03.000000 yalexs-1.5.2/tests/fixtures/get_locks.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      664 2023-02-17 14:03:03.000000 yalexs-1.5.2/tests/fixtures/get_pins.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      848 2023-02-17 14:03:03.000000 yalexs-1.5.2/tests/fixtures/keypad_lock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      682 2023-02-17 14:03:03.000000 yalexs-1.5.2/tests/fixtures/lock.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      366 2023-08-06 22:02:35.000000 yalexs-1.5.2/tests/fixtures/lock_accessory_motion_detect.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      800 2023-02-17 14:03:03.000000 yalexs-1.5.2/tests/fixtures/lock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     2745 2023-08-06 22:09:05.000000 yalexs-1.5.2/tests/fixtures/lock_with_doorbell.online.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      641 2023-02-17 14:03:03.000000 yalexs-1.5.2/tests/fixtures/lock_without_doorstate.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      315 2023-02-17 14:03:03.000000 yalexs-1.5.2/tests/fixtures/manual_lock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      321 2023-02-17 14:03:03.000000 yalexs-1.5.2/tests/fixtures/manual_unlock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      458 2023-02-17 14:03:03.000000 yalexs-1.5.2/tests/fixtures/pin_unlock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      409 2023-02-17 14:03:03.000000 yalexs-1.5.2/tests/fixtures/pin_unlock_activity_missing_image.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      479 2023-02-17 14:03:03.000000 yalexs-1.5.2/tests/fixtures/pin_unlock_activity_with_image.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      827 2023-02-17 14:03:03.000000 yalexs-1.5.2/tests/fixtures/remote_lock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      435 2023-02-17 14:03:03.000000 yalexs-1.5.2/tests/fixtures/remote_lock_activity_v4.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      441 2023-02-17 14:03:03.000000 yalexs-1.5.2/tests/fixtures/remote_unlock_activity_v4.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      559 2023-02-17 14:03:03.000000 yalexs-1.5.2/tests/fixtures/remote_unlock_activity_v4_2.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      686 2023-02-17 14:03:03.000000 yalexs-1.5.2/tests/fixtures/unlock.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      732 2023-02-17 14:03:03.000000 yalexs-1.5.2/tests/fixtures/unlock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      648 2023-02-17 14:03:03.000000 yalexs-1.5.2/tests/fixtures/unlock_without_doorstate.json
+-rw-r--r--   0 bdraco     (501) staff       (20)    15210 2023-08-06 22:02:35.000000 yalexs-1.5.2/tests/test_activity.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    33779 2023-05-17 14:08:38.000000 yalexs-1.5.2/tests/test_api.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    43482 2023-08-06 22:09:05.000000 yalexs-1.5.2/tests/test_api_async.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     7495 2023-02-17 14:03:03.000000 yalexs-1.5.2/tests/test_authenticator.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     8968 2023-05-17 14:08:38.000000 yalexs-1.5.2/tests/test_authenticator_async.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    17841 2023-08-06 21:48:58.000000 yalexs-1.5.2/tests/test_pubnub_activity.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    15595 2023-05-22 13:33:40.000000 yalexs-1.5.2/tests/test_util.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     1316 2023-02-17 14:33:57.000000 yalexs-1.5.2/tox.ini
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-08-06 22:09:22.222114 yalexs-1.5.2/yalexs/
+-rw-r--r--   0 bdraco     (501) staff       (20)      114 2023-08-06 22:09:07.000000 yalexs-1.5.2/yalexs/__init__.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    14170 2023-08-06 21:46:09.000000 yalexs-1.5.2/yalexs/activity.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     9979 2023-05-17 18:54:43.000000 yalexs-1.5.2/yalexs/api.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    15152 2023-08-06 22:02:57.000000 yalexs-1.5.2/yalexs/api_async.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    11644 2023-05-22 13:33:40.000000 yalexs-1.5.2/yalexs/api_common.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     4838 2023-05-17 14:08:38.000000 yalexs-1.5.2/yalexs/authenticator.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     5306 2023-05-17 18:44:25.000000 yalexs-1.5.2/yalexs/authenticator_async.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     5282 2023-05-22 13:33:40.000000 yalexs-1.5.2/yalexs/authenticator_common.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-08-06 22:09:22.222883 yalexs-1.5.2/yalexs/backports/
+-rw-r--r--   0 bdraco     (501) staff       (20)        0 2023-05-17 14:08:38.000000 yalexs-1.5.2/yalexs/backports/__init__.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     1020 2023-05-17 14:08:38.000000 yalexs-1.5.2/yalexs/backports/enum.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     1846 2023-05-18 17:02:22.000000 yalexs-1.5.2/yalexs/bridge.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     1283 2023-05-22 13:33:40.000000 yalexs-1.5.2/yalexs/const.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     1399 2023-02-17 14:03:03.000000 yalexs-1.5.2/yalexs/device.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     4251 2023-05-22 13:33:40.000000 yalexs-1.5.2/yalexs/doorbell.py
+-rw-r--r--   0 bdraco     (501) staff       (20)      776 2023-05-17 21:45:20.000000 yalexs-1.5.2/yalexs/exceptions.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     1044 2023-05-18 17:02:22.000000 yalexs-1.5.2/yalexs/keypad.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     8038 2023-08-06 22:09:05.000000 yalexs-1.5.2/yalexs/lock.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     2403 2023-05-22 13:33:40.000000 yalexs-1.5.2/yalexs/pin.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     4555 2023-05-17 21:25:12.000000 yalexs-1.5.2/yalexs/pubnub_activity.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     4484 2023-05-22 13:11:27.000000 yalexs-1.5.2/yalexs/pubnub_async.py
+-rw-r--r--   0 bdraco     (501) staff       (20)      298 2023-05-22 13:33:40.000000 yalexs-1.5.2/yalexs/time.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     1088 2023-02-17 14:03:03.000000 yalexs-1.5.2/yalexs/users.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     3913 2023-05-22 13:33:40.000000 yalexs-1.5.2/yalexs/util.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-08-06 22:09:22.222716 yalexs-1.5.2/yalexs.egg-info/
+-rw-r--r--   0 bdraco     (501) staff       (20)      666 2023-08-06 22:09:22.000000 yalexs-1.5.2/yalexs.egg-info/PKG-INFO
+-rw-r--r--   0 bdraco     (501) staff       (20)     2979 2023-08-06 22:09:22.000000 yalexs-1.5.2/yalexs.egg-info/SOURCES.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-08-06 22:09:22.000000 yalexs-1.5.2/yalexs.egg-info/dependency_links.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)      107 2023-08-06 22:09:22.000000 yalexs-1.5.2/yalexs.egg-info/requires.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)        7 2023-08-06 22:09:22.000000 yalexs-1.5.2/yalexs.egg-info/top_level.txt
```

### Comparing `yalexs-1.5.1/.github/workflows/ci.yaml` & `yalexs-1.5.2/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `yalexs-1.5.1/.gitignore` & `yalexs-1.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `yalexs-1.5.1/LICENSE` & `yalexs-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yalexs-1.5.1/PKG-INFO` & `yalexs-1.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yalexs
-Version: 1.5.1
+Version: 1.5.2
 Summary: Python API for Yale Access (formerly August) Smart Lock and Doorbell
 Home-page: https://github.com/bdraco/yalexs
 Author: bdraco
 Author-email: nick@koston.org
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `yalexs-1.5.1/README.md` & `yalexs-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `yalexs-1.5.1/known_activities.md` & `yalexs-1.5.2/known_activities.md`

 * *Files identical despite different names*

### Comparing `yalexs-1.5.1/pylintrc` & `yalexs-1.5.2/pylintrc`

 * *Files identical despite different names*

### Comparing `yalexs-1.5.1/setup.cfg` & `yalexs-1.5.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.5.1
+current_version = 1.5.2
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version="{current_version}"
 replace = version="{new_version}"
```

### Comparing `yalexs-1.5.1/setup.py` & `yalexs-1.5.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="yalexs",
-    version="1.5.1",
+    version="1.5.2",
     python_requires=">=3.9",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
```

### Comparing `yalexs-1.5.1/tests/fixtures/auto_relock_activity.json` & `yalexs-1.5.2/tests/fixtures/auto_relock_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.5.1/tests/fixtures/auto_unlock_activity.json` & `yalexs-1.5.2/tests/fixtures/auto_unlock_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.5.1/tests/fixtures/bluetooth_lock_activity.json` & `yalexs-1.5.2/tests/fixtures/bluetooth_lock_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.5.1/tests/fixtures/door_closed_activity.json` & `yalexs-1.5.2/tests/fixtures/door_closed_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.5.1/tests/fixtures/door_closed_activity_wrong_deviceid.json` & `yalexs-1.5.2/tests/fixtures/door_closed_activity_wrong_deviceid.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.5.1/tests/fixtures/door_closed_activity_wrong_houseid.json` & `yalexs-1.5.2/tests/fixtures/door_closed_activity_wrong_houseid.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.5.1/tests/fixtures/door_open_activity.json` & `yalexs-1.5.2/tests/fixtures/door_open_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.5.1/tests/fixtures/doorbell_motion_activity.json` & `yalexs-1.5.2/tests/fixtures/doorbell_motion_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.5.1/tests/fixtures/doorbell_motion_activity_no_image.json` & `yalexs-1.5.2/tests/fixtures/doorbell_motion_activity_no_image.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.5.1/tests/fixtures/doorbell_motion_activity_old.json` & `yalexs-1.5.2/tests/fixtures/doorbell_motion_activity_old.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.5.1/tests/fixtures/doorbell_motion_activity_wrong.json` & `yalexs-1.5.2/tests/fixtures/doorbell_motion_activity_wrong.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.5.1/tests/fixtures/get_doorbell.battery_full.json` & `yalexs-1.5.2/tests/fixtures/get_doorbell.battery_full.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.5.1/tests/fixtures/get_doorbell.battery_low.json` & `yalexs-1.5.2/tests/fixtures/get_doorbell.battery_low.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.5.1/tests/fixtures/get_doorbell.battery_medium.json` & `yalexs-1.5.2/tests/fixtures/get_doorbell.battery_medium.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.5.1/tests/fixtures/get_doorbell.json` & `yalexs-1.5.2/tests/fixtures/get_doorbell.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.5.1/tests/fixtures/get_doorbell.offline.json` & `yalexs-1.5.2/tests/fixtures/get_doorbell.offline.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.5.1/tests/fixtures/get_doorbell_missing_image.json` & `yalexs-1.5.2/tests/fixtures/get_doorbell_missing_image.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.5.1/tests/fixtures/get_doorbells.json` & `yalexs-1.5.2/tests/fixtures/get_doorbells.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.5.1/tests/fixtures/get_house_activities.json` & `yalexs-1.5.2/tests/fixtures/get_house_activities.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.5.1/tests/fixtures/get_lock.doorsense_init.json` & `yalexs-1.5.2/tests/fixtures/get_lock.doorsense_init.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.5.1/tests/fixtures/get_lock.nostatus_with_doorsense.json` & `yalexs-1.5.2/tests/fixtures/get_lock.nostatus_with_doorsense.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.5.1/tests/fixtures/get_lock.offline.json` & `yalexs-1.5.2/tests/fixtures/get_lock.offline.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.5.1/tests/fixtures/get_lock.online.json` & `yalexs-1.5.2/tests/fixtures/get_lock.online.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.5.1/tests/fixtures/get_lock.online_with_doorsense.json` & `yalexs-1.5.2/tests/fixtures/get_lock.online_with_doorsense.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.5.1/tests/fixtures/get_lock.online_with_doorsense_disabled.json` & `yalexs-1.5.2/tests/fixtures/get_lock.online_with_doorsense_disabled.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.5.1/tests/fixtures/get_lock_v2.online.json` & `yalexs-1.5.2/tests/fixtures/get_lock_v2.online.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.5.1/tests/fixtures/get_pins.json` & `yalexs-1.5.2/tests/fixtures/get_pins.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.5.1/tests/fixtures/keypad_lock_activity.json` & `yalexs-1.5.2/tests/fixtures/keypad_lock_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.5.1/tests/fixtures/lock.json` & `yalexs-1.5.2/tests/fixtures/lock.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.5.1/tests/fixtures/lock_activity.json` & `yalexs-1.5.2/tests/fixtures/lock_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.5.1/tests/fixtures/lock_without_doorstate.json` & `yalexs-1.5.2/tests/fixtures/lock_without_doorstate.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.5.1/tests/fixtures/remote_lock_activity.json` & `yalexs-1.5.2/tests/fixtures/remote_lock_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.5.1/tests/fixtures/remote_unlock_activity_v4_2.json` & `yalexs-1.5.2/tests/fixtures/remote_unlock_activity_v4_2.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.5.1/tests/fixtures/unlock.json` & `yalexs-1.5.2/tests/fixtures/unlock.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.5.1/tests/fixtures/unlock_activity.json` & `yalexs-1.5.2/tests/fixtures/unlock_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.5.1/tests/fixtures/unlock_without_doorstate.json` & `yalexs-1.5.2/tests/fixtures/unlock_without_doorstate.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.5.1/tests/test_activity.py` & `yalexs-1.5.2/tests/test_activity.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,14 +44,15 @@
     ACTIVITY_ACTIONS_DOORBELL_DING,
     ACTIVITY_ACTIONS_DOORBELL_IMAGE_CAPTURE,
     ACTIVITY_ACTIONS_DOORBELL_MOTION,
     ACTIVITY_ACTIONS_DOORBELL_VIEW,
     ACTIVITY_ACTIONS_LOCK_OPERATION,
     SOURCE_LOG,
     ActivityType,
+    DoorbellDingActivity,
     LockOperationActivity,
 )
 from yalexs.api_async import ApiAsync
 from yalexs.api_common import API_GET_LOCK_URL, ApiCommon
 from yalexs.const import DEFAULT_BRAND
 from yalexs.lock import LockDoorStatus, LockStatus
 
@@ -325,14 +326,21 @@
             SOURCE_LOG, json.loads(load_fixture("auto_relock_activity.json"))
         )
         assert auto_relock_operation_activity.operated_by == "I have no picture"
         assert auto_relock_operation_activity.operated_remote is False
         assert auto_relock_operation_activity.operated_autorelock is True
         assert auto_relock_operation_activity.operated_keypad is False
 
+    def test_get_lock_button_pressed(self):
+        doorbell_ding_activity = DoorbellDingActivity(
+            SOURCE_LOG, json.loads(load_fixture("lock_accessory_motion_detect.json"))
+        )
+        assert doorbell_ding_activity.activity_start_time.timestamp() == 1691249378.0
+        assert doorbell_ding_activity.activity_end_time.timestamp() == 1691249378.0
+
 
 class TestActivityApiAsync(aiounittest.AsyncTestCase):
     @aioresponses()
     async def test_async_get_lock_detail_bridge_online(self, mock):
         mock.get(
             ApiCommon(DEFAULT_BRAND)
             .get_brand_url(API_GET_LOCK_URL)
```

### Comparing `yalexs-1.5.1/tests/test_api.py` & `yalexs-1.5.2/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.5.1/tests/test_api_async.py` & `yalexs-1.5.2/tests/test_api_async.py`

 * *Files 1% similar despite different names*

```diff
@@ -372,14 +372,15 @@
         )
 
         api = ApiAsync(ClientSession())
         lock = await api.async_get_lock_detail(
             ACCESS_TOKEN, "A6697750D607098BAE8D6BAA11EF8063"
         )
 
+        assert lock.doorbell is False
         self.assertEqual("A6697750D607098BAE8D6BAA11EF8063", lock.device_id)
         self.assertEqual("Front Door Lock", lock.device_name)
         self.assertEqual("000000000000", lock.house_id)
         self.assertEqual("X2FSW05DGA", lock.serial_number)
         self.assertEqual("109717e9-3.0.44-3.0.30", lock.firmware_version)
         self.assertEqual(88, lock.battery_level)
         self.assertEqual("AUG-SL02-M02-S02", lock.model)
@@ -398,14 +399,30 @@
             dateutil.parser.parse("2017-12-10T04:48:30.272Z"), lock.lock_status_datetime
         )
         self.assertEqual(
             dateutil.parser.parse("2017-12-10T04:48:30.272Z"), lock.door_state_datetime
         )
 
     @aioresponses()
+    async def test_async_get_lock_with_doorbell(self, mock):
+        mock.get(
+            ApiCommon(DEFAULT_BRAND)
+            .get_brand_url(API_GET_LOCK_URL)
+            .format(lock_id="A6697750D607098BAE8D6BAA11EF8063"),
+            body=load_fixture("lock_with_doorbell.online.json"),
+        )
+
+        api = ApiAsync(ClientSession())
+        lock = await api.async_get_lock_detail(
+            ACCESS_TOKEN, "A6697750D607098BAE8D6BAA11EF8063"
+        )
+
+        assert lock.doorbell is True
+
+    @aioresponses()
     async def test_async_get_v2_lock_detail_bridge_online(self, mock):
         mock.get(
             ApiCommon(DEFAULT_BRAND)
             .get_brand_url(API_GET_LOCK_URL)
             .format(lock_id="snip"),
             body=load_fixture("get_lock_v2.online.json"),
         )
```

### Comparing `yalexs-1.5.1/tests/test_authenticator.py` & `yalexs-1.5.2/tests/test_authenticator.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.5.1/tests/test_authenticator_async.py` & `yalexs-1.5.2/tests/test_authenticator_async.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.5.1/tests/test_pubnub_activity.py` & `yalexs-1.5.2/tests/test_pubnub_activity.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.5.1/tests/test_util.py` & `yalexs-1.5.2/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.5.1/tox.ini` & `yalexs-1.5.2/tox.ini`

 * *Files identical despite different names*

### Comparing `yalexs-1.5.1/yalexs/activity.py` & `yalexs-1.5.2/yalexs/activity.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.5.1/yalexs/api.py` & `yalexs-1.5.2/yalexs/api.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.5.1/yalexs/api_async.py` & `yalexs-1.5.2/yalexs/api_async.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.5.1/yalexs/api_common.py` & `yalexs-1.5.2/yalexs/api_common.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.5.1/yalexs/authenticator.py` & `yalexs-1.5.2/yalexs/authenticator.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.5.1/yalexs/authenticator_async.py` & `yalexs-1.5.2/yalexs/authenticator_async.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.5.1/yalexs/authenticator_common.py` & `yalexs-1.5.2/yalexs/authenticator_common.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.5.1/yalexs/backports/enum.py` & `yalexs-1.5.2/yalexs/backports/enum.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.5.1/yalexs/bridge.py` & `yalexs-1.5.2/yalexs/bridge.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.5.1/yalexs/const.py` & `yalexs-1.5.2/yalexs/const.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.5.1/yalexs/device.py` & `yalexs-1.5.2/yalexs/device.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.5.1/yalexs/doorbell.py` & `yalexs-1.5.2/yalexs/doorbell.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.5.1/yalexs/exceptions.py` & `yalexs-1.5.2/yalexs/exceptions.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.5.1/yalexs/keypad.py` & `yalexs-1.5.2/yalexs/keypad.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.5.1/yalexs/lock.py` & `yalexs-1.5.2/yalexs/lock.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,14 +103,19 @@
         self._data = data
 
     @property
     def model(self):
         return self._model
 
     @property
+    def doorbell(self) -> bool:
+        # Type 7 is a doorman
+        return self._data["Type"] == 7
+
+    @property
     def battery_level(self):
         return self._battery_level
 
     @property
     def keypad(self):
         return self._keypad_detail
```

### Comparing `yalexs-1.5.1/yalexs/pin.py` & `yalexs-1.5.2/yalexs/pin.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.5.1/yalexs/pubnub_activity.py` & `yalexs-1.5.2/yalexs/pubnub_activity.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.5.1/yalexs/pubnub_async.py` & `yalexs-1.5.2/yalexs/pubnub_async.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.5.1/yalexs/users.py` & `yalexs-1.5.2/yalexs/users.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.5.1/yalexs/util.py` & `yalexs-1.5.2/yalexs/util.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.5.1/yalexs.egg-info/PKG-INFO` & `yalexs-1.5.2/yalexs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yalexs
-Version: 1.5.1
+Version: 1.5.2
 Summary: Python API for Yale Access (formerly August) Smart Lock and Doorbell
 Home-page: https://github.com/bdraco/yalexs
 Author: bdraco
 Author-email: nick@koston.org
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `yalexs-1.5.1/yalexs.egg-info/SOURCES.txt` & `yalexs-1.5.2/yalexs.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -45,15 +45,17 @@
 tests/fixtures/get_lock.online_with_doorsense.json
 tests/fixtures/get_lock.online_with_doorsense_disabled.json
 tests/fixtures/get_lock_v2.online.json
 tests/fixtures/get_locks.json
 tests/fixtures/get_pins.json
 tests/fixtures/keypad_lock_activity.json
 tests/fixtures/lock.json
+tests/fixtures/lock_accessory_motion_detect.json
 tests/fixtures/lock_activity.json
+tests/fixtures/lock_with_doorbell.online.json
 tests/fixtures/lock_without_doorstate.json
 tests/fixtures/manual_lock_activity.json
 tests/fixtures/manual_unlock_activity.json
 tests/fixtures/pin_unlock_activity.json
 tests/fixtures/pin_unlock_activity_missing_image.json
 tests/fixtures/pin_unlock_activity_with_image.json
 tests/fixtures/remote_lock_activity.json
```

