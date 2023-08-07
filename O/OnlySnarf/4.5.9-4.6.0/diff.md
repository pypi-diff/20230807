# Comparing `tmp/OnlySnarf-4.5.9.tar.gz` & `tmp/OnlySnarf-4.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OnlySnarf-4.5.9.tar", last modified: Fri Aug  4 01:34:54 2023, max compression
+gzip compressed data, was "OnlySnarf-4.6.0.tar", last modified: Mon Aug  7 20:14:45 2023, max compression
```

## Comparing `OnlySnarf-4.5.9.tar` & `OnlySnarf-4.6.0.tar`

### file list

```diff
@@ -1,57 +1,59 @@
-drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-08-04 01:34:54.789213 OnlySnarf-4.5.9/
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    32332 2023-08-04 01:34:34.000000 OnlySnarf-4.5.9/CHANGELOG.md
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1064 2023-04-16 06:45:34.000000 OnlySnarf-4.5.9/LICENSE.txt
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)      141 2023-04-16 06:45:34.000000 OnlySnarf-4.5.9/MANIFEST.in
-drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-08-04 01:34:54.785213 OnlySnarf-4.5.9/OnlySnarf/
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)       75 2023-07-26 00:57:38.000000 OnlySnarf-4.5.9/OnlySnarf/__init__.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)      387 2023-04-16 06:45:34.000000 OnlySnarf-4.5.9/OnlySnarf/__main__.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     2142 2023-08-03 01:40:40.000000 OnlySnarf-4.5.9/OnlySnarf/api.py
-drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-08-04 01:34:54.785213 OnlySnarf-4.5.9/OnlySnarf/classes/
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-16 06:45:34.000000 OnlySnarf-4.5.9/OnlySnarf/classes/__init__.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     4388 2023-04-16 06:45:34.000000 OnlySnarf-4.5.9/OnlySnarf/classes/discount.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1892 2023-04-16 06:45:34.000000 OnlySnarf-4.5.9/OnlySnarf/classes/element.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    16142 2023-07-11 22:15:12.000000 OnlySnarf-4.5.9/OnlySnarf/classes/file.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    12611 2023-08-02 19:27:24.000000 OnlySnarf-4.5.9/OnlySnarf/classes/message.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1986 2023-07-17 07:19:23.000000 OnlySnarf-4.5.9/OnlySnarf/classes/poll.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    14542 2023-05-29 23:06:57.000000 OnlySnarf-4.5.9/OnlySnarf/classes/profile.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    10171 2023-04-16 06:45:34.000000 OnlySnarf-4.5.9/OnlySnarf/classes/promotion.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     4891 2023-07-12 22:40:17.000000 OnlySnarf-4.5.9/OnlySnarf/classes/schedule.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    20341 2023-08-02 19:27:24.000000 OnlySnarf-4.5.9/OnlySnarf/classes/user.py
-drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-08-04 01:34:54.785213 OnlySnarf-4.5.9/OnlySnarf/conf/
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     2249 2023-08-02 19:27:24.000000 OnlySnarf-4.5.9/OnlySnarf/conf/config.conf
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     2353 2023-08-02 19:27:24.000000 OnlySnarf-4.5.9/OnlySnarf/conf/test-config.conf
-drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-08-04 01:34:54.789213 OnlySnarf-4.5.9/OnlySnarf/elements/
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-16 06:45:34.000000 OnlySnarf-4.5.9/OnlySnarf/elements/__init__.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    15689 2023-04-16 06:45:34.000000 OnlySnarf-4.5.9/OnlySnarf/elements/driver.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1401 2023-04-16 06:45:34.000000 OnlySnarf-4.5.9/OnlySnarf/elements/login.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    11335 2023-04-16 06:45:34.000000 OnlySnarf-4.5.9/OnlySnarf/elements/profile.py
-drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-08-04 01:34:54.789213 OnlySnarf-4.5.9/OnlySnarf/lib/
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-16 06:45:34.000000 OnlySnarf-4.5.9/OnlySnarf/lib/__init__.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)   167866 2023-08-03 01:45:45.000000 OnlySnarf-4.5.9/OnlySnarf/lib/driver.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     9500 2023-04-16 06:45:34.000000 OnlySnarf-4.5.9/OnlySnarf/lib/ffmpeg.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     5076 2023-07-17 07:19:23.000000 OnlySnarf-4.5.9/OnlySnarf/menu.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     5006 2023-07-17 07:19:23.000000 OnlySnarf-4.5.9/OnlySnarf/snarf.py
-drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-08-04 01:34:54.789213 OnlySnarf-4.5.9/OnlySnarf/util/
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-16 06:45:34.000000 OnlySnarf-4.5.9/OnlySnarf/util/__init__.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1327 2023-07-17 03:26:29.000000 OnlySnarf-4.5.9/OnlySnarf/util/args.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1062 2023-04-16 06:45:34.000000 OnlySnarf-4.5.9/OnlySnarf/util/colorize.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1591 2023-08-02 19:27:24.000000 OnlySnarf-4.5.9/OnlySnarf/util/config.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     3283 2023-08-03 01:34:26.000000 OnlySnarf-4.5.9/OnlySnarf/util/defaults.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     2025 2023-04-16 06:45:34.000000 OnlySnarf-4.5.9/OnlySnarf/util/logger.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    12451 2023-08-02 19:27:24.000000 OnlySnarf-4.5.9/OnlySnarf/util/optional_args.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    20703 2023-08-03 01:34:20.000000 OnlySnarf-4.5.9/OnlySnarf/util/settings.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     3934 2023-07-11 19:44:50.000000 OnlySnarf-4.5.9/OnlySnarf/util/validators.py
-drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-08-04 01:34:54.785213 OnlySnarf-4.5.9/OnlySnarf.egg-info/
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     4679 2023-08-04 01:34:54.000000 OnlySnarf-4.5.9/OnlySnarf.egg-info/PKG-INFO
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1188 2023-08-04 01:34:54.000000 OnlySnarf-4.5.9/OnlySnarf.egg-info/SOURCES.txt
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        1 2023-08-04 01:34:54.000000 OnlySnarf-4.5.9/OnlySnarf.egg-info/dependency_links.txt
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)      109 2023-08-04 01:34:54.000000 OnlySnarf-4.5.9/OnlySnarf.egg-info/entry_points.txt
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)      104 2023-08-04 01:34:54.000000 OnlySnarf-4.5.9/OnlySnarf.egg-info/requires.txt
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)       91 2023-08-04 01:34:54.000000 OnlySnarf-4.5.9/OnlySnarf.egg-info/top_level.txt
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     4679 2023-08-04 01:34:54.789213 OnlySnarf-4.5.9/PKG-INFO
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     4049 2023-07-06 00:40:42.000000 OnlySnarf-4.5.9/README.md
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)       79 2023-08-04 01:34:54.789213 OnlySnarf-4.5.9/setup.cfg
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1475 2023-08-04 01:34:31.000000 OnlySnarf-4.5.9/setup.py
-drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-08-04 01:34:54.789213 OnlySnarf-4.5.9/tests/
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1209 2023-04-16 06:45:34.000000 OnlySnarf-4.5.9/tests/test_profile.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1451 2023-04-16 06:45:34.000000 OnlySnarf-4.5.9/tests/test_promotion.py
+drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-08-07 20:14:45.841944 OnlySnarf-4.6.0/
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    32650 2023-08-07 20:14:30.000000 OnlySnarf-4.6.0/CHANGELOG.md
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1064 2023-04-16 06:45:34.000000 OnlySnarf-4.6.0/LICENSE.txt
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)      249 2023-08-04 21:10:23.000000 OnlySnarf-4.6.0/MANIFEST.in
+drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-08-07 20:14:45.837944 OnlySnarf-4.6.0/OnlySnarf/
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)       24 2023-08-07 20:10:51.000000 OnlySnarf-4.6.0/OnlySnarf/__init__.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)      387 2023-04-16 06:45:34.000000 OnlySnarf-4.6.0/OnlySnarf/__main__.py
+drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-08-07 20:14:45.837944 OnlySnarf-4.6.0/OnlySnarf/classes/
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-16 06:45:34.000000 OnlySnarf-4.6.0/OnlySnarf/classes/__init__.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    13333 2023-08-04 23:43:14.000000 OnlySnarf-4.6.0/OnlySnarf/classes/config.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     4388 2023-04-16 06:45:34.000000 OnlySnarf-4.6.0/OnlySnarf/classes/discount.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1892 2023-04-16 06:45:34.000000 OnlySnarf-4.6.0/OnlySnarf/classes/element.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    16142 2023-07-11 22:15:12.000000 OnlySnarf-4.6.0/OnlySnarf/classes/file.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    12611 2023-08-02 19:27:24.000000 OnlySnarf-4.6.0/OnlySnarf/classes/message.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1986 2023-07-17 07:19:23.000000 OnlySnarf-4.6.0/OnlySnarf/classes/poll.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    14542 2023-05-29 23:06:57.000000 OnlySnarf-4.6.0/OnlySnarf/classes/profile.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    10171 2023-04-16 06:45:34.000000 OnlySnarf-4.6.0/OnlySnarf/classes/promotion.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     4891 2023-07-12 22:40:17.000000 OnlySnarf-4.6.0/OnlySnarf/classes/schedule.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    20341 2023-08-02 19:27:24.000000 OnlySnarf-4.6.0/OnlySnarf/classes/user.py
+drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-08-07 20:14:45.837944 OnlySnarf-4.6.0/OnlySnarf/conf/
+drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-08-07 20:14:45.837944 OnlySnarf-4.6.0/OnlySnarf/conf/users/
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)      169 2023-08-04 21:37:49.000000 OnlySnarf-4.6.0/OnlySnarf/conf/users/example-user.conf
+drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-08-07 20:14:45.837944 OnlySnarf-4.6.0/OnlySnarf/elements/
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-16 06:45:34.000000 OnlySnarf-4.6.0/OnlySnarf/elements/__init__.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    15689 2023-04-16 06:45:34.000000 OnlySnarf-4.6.0/OnlySnarf/elements/driver.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1401 2023-04-16 06:45:34.000000 OnlySnarf-4.6.0/OnlySnarf/elements/login.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    11335 2023-04-16 06:45:34.000000 OnlySnarf-4.6.0/OnlySnarf/elements/profile.py
+drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-08-07 20:14:45.841944 OnlySnarf-4.6.0/OnlySnarf/lib/
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-16 06:45:34.000000 OnlySnarf-4.6.0/OnlySnarf/lib/__init__.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)   167866 2023-08-03 01:45:45.000000 OnlySnarf-4.6.0/OnlySnarf/lib/driver.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     9500 2023-04-16 06:45:34.000000 OnlySnarf-4.6.0/OnlySnarf/lib/ffmpeg.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     5097 2023-08-04 19:56:36.000000 OnlySnarf-4.6.0/OnlySnarf/lib/menu.py
+drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-08-07 20:14:45.841944 OnlySnarf-4.6.0/OnlySnarf/server/
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     2195 2023-08-04 19:54:19.000000 OnlySnarf-4.6.0/OnlySnarf/server/api.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     5270 2023-08-04 21:10:49.000000 OnlySnarf-4.6.0/OnlySnarf/snarf.py
+drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-08-07 20:14:45.841944 OnlySnarf-4.6.0/OnlySnarf/util/
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-16 06:45:34.000000 OnlySnarf-4.6.0/OnlySnarf/util/__init__.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1327 2023-08-07 20:14:27.000000 OnlySnarf-4.6.0/OnlySnarf/util/args.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1062 2023-04-16 06:45:34.000000 OnlySnarf-4.6.0/OnlySnarf/util/colorize.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1591 2023-08-02 19:27:24.000000 OnlySnarf-4.6.0/OnlySnarf/util/config.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     3338 2023-08-04 04:20:17.000000 OnlySnarf-4.6.0/OnlySnarf/util/defaults.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     2025 2023-04-16 06:45:34.000000 OnlySnarf-4.6.0/OnlySnarf/util/logger.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    12695 2023-08-04 19:51:17.000000 OnlySnarf-4.6.0/OnlySnarf/util/optional_args.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    21582 2023-08-04 23:43:16.000000 OnlySnarf-4.6.0/OnlySnarf/util/settings.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     3934 2023-07-11 19:44:50.000000 OnlySnarf-4.6.0/OnlySnarf/util/validators.py
+drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-08-07 20:14:45.837944 OnlySnarf-4.6.0/OnlySnarf.egg-info/
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     4679 2023-08-07 20:14:45.000000 OnlySnarf-4.6.0/OnlySnarf.egg-info/PKG-INFO
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1207 2023-08-07 20:14:45.000000 OnlySnarf-4.6.0/OnlySnarf.egg-info/SOURCES.txt
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        1 2023-08-07 20:14:45.000000 OnlySnarf-4.6.0/OnlySnarf.egg-info/dependency_links.txt
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)       47 2023-08-07 20:14:45.000000 OnlySnarf-4.6.0/OnlySnarf.egg-info/entry_points.txt
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)      104 2023-08-07 20:14:45.000000 OnlySnarf-4.6.0/OnlySnarf.egg-info/requires.txt
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)      108 2023-08-07 20:14:45.000000 OnlySnarf-4.6.0/OnlySnarf.egg-info/top_level.txt
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     4679 2023-08-07 20:14:45.841944 OnlySnarf-4.6.0/PKG-INFO
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     4049 2023-07-06 00:40:42.000000 OnlySnarf-4.6.0/README.md
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)       79 2023-08-07 20:14:45.841944 OnlySnarf-4.6.0/setup.cfg
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1398 2023-08-07 20:12:08.000000 OnlySnarf-4.6.0/setup.py
+drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-08-07 20:14:45.841944 OnlySnarf-4.6.0/tests/
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1209 2023-04-16 06:45:34.000000 OnlySnarf-4.6.0/tests/test_profile.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1451 2023-04-16 06:45:34.000000 OnlySnarf-4.6.0/tests/test_promotion.py
```

### Comparing `OnlySnarf-4.5.9/CHANGELOG.md` & `OnlySnarf-4.6.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -711,27 +711,35 @@
   - updated driver.poll
   - fixed new message tests
   - added flask to package reqs
   - updated install script
   - updated api scripts to route through snarf
   **4.5.3,4,5,6 : 7/30/2023**
   - api debugging
-**4.5.7,8 : 8/2/2023**
+  **4.5.7,8 : 8/2/2023**
   - fixed twitter login; added phone number to args&config
   - more api debugging w/ aws
   - updated date&time formats
   - debugged api: /message & /post
-**4.5.9 : 8/3/2023**
+  **4.5.9 : 8/3/2023**
   - added update script meant to be run by systemd service script
+  - added config script; requires testing
+**4.5.10 : 8/4/2023**
+  - moved api & menu to cli
+  - updates to config script
+  - tested new config script
+**4.6.0 : 8/7/2023**
+  - minor version bump for working api & cli changes
 
 ------------------------------------------------------------------------------------
 
 ## TODO
 
-- bump minor version for working api
+- add cli args for config to autoconfigure more easily
+- update 'snarf config' to interact with main config file and variables
 
 - look into Marshmellow package for class / object cleanup
 
 
 - add smart idea for getting statement information
 - add better version notes to readme's list of "works on"
 - re-add stuff for testing on multiple platforms ala mac ;)
```

### Comparing `OnlySnarf-4.5.9/LICENSE.txt` & `OnlySnarf-4.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.9/OnlySnarf/api.py` & `OnlySnarf-4.6.0/OnlySnarf/server/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import os
 import json
 from flask import Flask, request
 
-from .util.config import config
-from .util.settings import Settings
-from .snarf import Snarf
+from ..util.config import config
+from ..util.settings import Settings
 
 def create_app():
     app = Flask(__name__)
 
     @app.route('/message', methods=['POST'])
     def message():
         try:
@@ -20,14 +19,15 @@
             except Exception as e: pass
             try: config["price"] = args["price"] or 0
             except Exception as e: pass
             try: config["schedule"] = args["schedule"]
             except Exception as e: pass
             try: config["performers"] = args["performers"]
             except Exception as e: pass
+            from ..snarf import Snarf
             Snarf.message()
             Snarf.close()
         except Exception as e:
             Settings.dev_print(e)
         finally:
             return "", 200
 
@@ -45,14 +45,15 @@
             except Exception as e: pass
             try: config["questions"] = args["questions"]
             except Exception as e: pass
             try: config["duration"] = args["duration"]
             except Exception as e: pass
             try: config["expires"] = args["expires"]
             except Exception as e: pass
+            from ..snarf import Snarf
             Snarf.post()
             Snarf.close()
         except Exception as e:
             Settings.dev_print(e)
         finally:
             return "", 200
```

### Comparing `OnlySnarf-4.5.9/OnlySnarf/classes/discount.py` & `OnlySnarf-4.6.0/OnlySnarf/classes/discount.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.9/OnlySnarf/classes/element.py` & `OnlySnarf-4.6.0/OnlySnarf/classes/element.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.9/OnlySnarf/classes/file.py` & `OnlySnarf-4.6.0/OnlySnarf/classes/file.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.9/OnlySnarf/classes/message.py` & `OnlySnarf-4.6.0/OnlySnarf/classes/message.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.9/OnlySnarf/classes/poll.py` & `OnlySnarf-4.6.0/OnlySnarf/classes/poll.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.9/OnlySnarf/classes/profile.py` & `OnlySnarf-4.6.0/OnlySnarf/classes/profile.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.9/OnlySnarf/classes/promotion.py` & `OnlySnarf-4.6.0/OnlySnarf/classes/promotion.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.9/OnlySnarf/classes/schedule.py` & `OnlySnarf-4.6.0/OnlySnarf/classes/schedule.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.9/OnlySnarf/classes/user.py` & `OnlySnarf-4.6.0/OnlySnarf/classes/user.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.9/OnlySnarf/elements/driver.py` & `OnlySnarf-4.6.0/OnlySnarf/elements/driver.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.9/OnlySnarf/elements/login.py` & `OnlySnarf-4.6.0/OnlySnarf/elements/login.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.9/OnlySnarf/elements/profile.py` & `OnlySnarf-4.6.0/OnlySnarf/elements/profile.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.9/OnlySnarf/lib/driver.py` & `OnlySnarf-4.6.0/OnlySnarf/lib/driver.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.9/OnlySnarf/lib/ffmpeg.py` & `OnlySnarf-4.6.0/OnlySnarf/lib/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.9/OnlySnarf/menu.py` & `OnlySnarf-4.6.0/OnlySnarf/lib/menu.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,19 +2,18 @@
 
 import os
 import time
 import random
 import sys
 import inquirer
 ##
-from .snarf import Snarf
-from .lib.driver import Driver
-from .classes.profile import Profile
-from .util.colorize import colorize
-from .util.settings import Settings
+from ..lib.driver import Driver
+from ..classes.profile import Profile
+from ..util.colorize import colorize
+from ..util.settings import Settings
 
 # from .util.args import parser
 # print(parser)
 # parser.add_parser('menu', help='> access the cli menu')
 
 ####################
 ##### CLI Menu #####
@@ -57,14 +56,15 @@
     def action_menu():
         """
         Prompt the action menu. Cycles back to main menu
 
 
         """
 
+        from ..snarf import Snarf
         action = Menu.ask_action()
         if (action == 'back'): return Menu.main()
         elif (action == 'discount'): Snarf.discount()
         elif (action == 'message'): Snarf.message()
         elif (action == 'post'): Snarf.post()
         elif (action == 'profile'): Profile.menu()
         elif (action == 'promotion'): Snarf.promotion()
@@ -151,15 +151,15 @@
 
 
         """
 
         action = Menu.menu()
         if (action == 'Action'): Menu.action_menu()
         elif (action == 'Settings'): Settings.menu()
-        else: exit()
+        else: exit_handler()
         Menu.main()
 
     def main():
         """
         Primary script entry
```

### Comparing `OnlySnarf-4.5.9/OnlySnarf/snarf.py` & `OnlySnarf-4.6.0/OnlySnarf/snarf.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 #!/usr/bin/python3
 
 from .lib.driver import Driver
+from .lib.menu import Menu
 from .util.settings import Settings
+from .classes.config import Config
 from .classes.discount import Discount
 from .classes.message import Message, Post
 from .classes.profile import Profile
 from .classes.promotion import Promotion
 from .classes.user import User
+from .server import api as API
 
 #################
 ##### Snarf #####
 #################
 
 class Snarf:
 
@@ -29,14 +32,26 @@
 
     @staticmethod
     def close():
         Driver.exit_all()
         Settings.print("*snarf waves goodbye*")
 
     @staticmethod
+    def api():
+        API.main()
+
+    @staticmethod
+    def config():
+        Config.main()
+
+    @staticmethod
+    def menu():
+        Menu.main()
+
+    @staticmethod
     def discount():
 
         """
         Applies a discount to users as provided from args / prompts.
 
 
         """
@@ -169,16 +184,16 @@
 
 import atexit
 atexit.register(exit_handler)
 
 def main():
     try:
         # purge local tmp files
-        from .classes.file import File
-        File.remove_local()
+        # from .classes.file import File
+        # File.remove_local()
         # get the thing, do the thing
         action = Settings.get_action()
         Settings.print("Running - {}".format(action))
         action = getattr(Snarf, action)
         action()
     except Exception as e:
         Settings.dev_print(e)
```

### Comparing `OnlySnarf-4.5.9/OnlySnarf/util/args.py` & `OnlySnarf-4.6.0/OnlySnarf/util/args.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.9/OnlySnarf/util/colorize.py` & `OnlySnarf-4.6.0/OnlySnarf/util/colorize.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.9/OnlySnarf/util/config.py` & `OnlySnarf-4.6.0/OnlySnarf/util/config.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.9/OnlySnarf/util/defaults.py` & `OnlySnarf-4.6.0/OnlySnarf/util/defaults.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,7 +113,8 @@
     print("upload: "+UPLOAD_PATH)
     print("users: "+USERS_PATH)
 
 Path(ROOT_PATH).mkdir(parents=True, exist_ok=True)
 Path(DOWNLOAD_PATH).mkdir(parents=True, exist_ok=True)
 Path(UPLOAD_PATH).mkdir(parents=True, exist_ok=True)
 Path(CONFIGS_PATH).mkdir(parents=True, exist_ok=True)
+Path(PROFILES_PATH).mkdir(parents=True, exist_ok=True)
```

### Comparing `OnlySnarf-4.5.9/OnlySnarf/util/logger.py` & `OnlySnarf-4.6.0/OnlySnarf/util/logger.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.9/OnlySnarf/util/optional_args.py` & `OnlySnarf-4.6.0/OnlySnarf/util/optional_args.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
   ##
   # -tweet
   # enabled tweeting
   parser.add_argument('-tweet', action='store_true', dest='tweeting', help='enable tweeting when posting')
   ##
   # --username
   # OnlyFans username to use
-  parser.add_argument('--username', '--u', type=str, default="", dest='username', help='OnlyFans username to use')
+  parser.add_argument('--username', '--u', type=str, default="default", dest='username', help='OnlyFans username to use')
   ##
   # -phone
   # OnlyFans phone number to use for additional login steps
   parser.add_argument('-phone', type=str, default="", dest='phone', help='OnlyFans phone number to use')
 
   ###############
   ## DEBUGGING ##
@@ -125,14 +125,26 @@
   parser.add_argument('-v', '-verbose', dest="verbose", action='count', default=0, help="verbosity level (max 3)")
 
 
 def apply_subcommand_args(parser):
 
   subparsers = parser.add_subparsers(help='Include a sub-command to run a corresponding action:', dest="action", required=True)
 
+  #########
+  ## API ##
+  #########
+
+  parser_config = subparsers.add_parser('api', help='> flask server')
+
+  ############
+  ## Config ##
+  ############
+
+  parser_config = subparsers.add_parser('config', help='> configuration options')
+
   ##############
   ## Discount ##
   ##############
 
   parser_discount = subparsers.add_parser('discount', help='> discount one or more users')
   userAndUsers = parser_discount.add_mutually_exclusive_group()
   ##
```

### Comparing `OnlySnarf-4.5.9/OnlySnarf/util/settings.py` & `OnlySnarf-4.6.0/OnlySnarf/util/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,14 +75,21 @@
 
     def menu():
         Settings.print("### SETTINGS MENU ###")
         Settings.print("...")
         Settings.print("...")
         Settings.print("...")
 
+    def ensure_paths():
+        Path(DEFAULT.ROOT_PATH).mkdir(parents=True, exist_ok=True)
+        Path(DEFAULT.DOWNLOAD_PATH).mkdir(parents=True, exist_ok=True)
+        Path(DEFAULT.UPLOAD_PATH).mkdir(parents=True, exist_ok=True)
+        Path(DEFAULT.CONFIGS_PATH).mkdir(parents=True, exist_ok=True)
+        Path(DEFAULT.PROFILES_PATH).mkdir(parents=True, exist_ok=True)
+
     ##
     # Getters
     ##
 
     def get_action():
         return config["action"]
 
@@ -248,27 +255,33 @@
     
     def get_promotion_limit():
         return config["promotion_limit"] or None
 
     def get_promotion_method():
         return config["promotion_method"] or None
 
-    def get_password():
-        try: return Settings.get_user_config(Settings.get_username())["onlyfans_password"]
-        except Exception as e: Settings.err_print(e)
+    def get_password(username=None):
+        try:
+            if not username: username = Settings.get_username()
+            return Settings.get_user_config(username)["onlyfans_password"]
+        except Exception as e: pass
         return ""
 
-    def get_password_google():
-        try: return Settings.get_user_config(Settings.get_username())["google_password"]
-        except Exception as e: Settings.err_print(e)
+    def get_password_google(username=None):
+        try:
+            if not username: username = Settings.get_username()
+            return Settings.get_user_config(username)["google_password"]
+        except Exception as e: pass
         return ""
 
-    def get_password_twitter():
-        try: return Settings.get_user_config(Settings.get_username())["twitter_password"]
-        except Exception as e: Settings.err_print(e)
+    def get_password_twitter(username=None):
+        try: 
+            if not username: username = Settings.get_username()
+            return Settings.get_user_config(username)["twitter_password"]
+        except Exception as e: pass
         return ""
 
     def get_download_path():
         try: return config["path_download"]
         except Exception as e: pass
         return DEFAULT.DOWNLOAD_PATH
 
@@ -280,15 +293,14 @@
     def get_config_path():
         try: return config["path_config"]   
         except Exception as e: pass
         return DEFAULT.CONFIG_PATH
 
     def get_local_path():
         localPath = os.path.join(Settings.get_root_path(), Settings.get_username())
-        from pathlib import Path
         Path(localPath).mkdir(parents=True, exist_ok=True)
         for cat in Settings.get_categories():
             Path(os.path.join(localPath, cat)).mkdir(parents=True, exist_ok=True)
         return localPath
 
     def get_reconnect_id():
         return config["session_id"] or ""
@@ -435,48 +447,53 @@
         pass
 
     def get_user_config(username="default"):
         import configparser
         config_file = configparser.ConfigParser()
         # strip email
         if "@" in username: username = username[0 : username.index("@")]
+        username = username.replace(".conf", "") # filename formatting
         Settings.dev_print("retrieving user config: {}".format(username))
-        Settings.dev_print(os.path.join(Settings.get_base_directory(), "conf", "users", username+".conf"))
-        config_file.read(os.path.join(Settings.get_base_directory(), "conf", "users", username+".conf"))
+        Settings.dev_print(os.path.join(Settings.get_base_directory(), "conf/users", username+".conf"))
+        config_file.read(os.path.join(Settings.get_base_directory(), "conf/users", username+".conf"))
         userConfig = {}
         for section in config_file.sections():
             # Settings.dev_print(section)
             for key in config_file[section]:
                 # Settings.dev_print(section, key, config_file[section][key].strip("\""))
                 userConfig[section.lower()+"_"+key.lower()] = config_file[section][key].strip("\"")
         # Settings.dev_print(userConfig)
         return userConfig
 
+    def get_user_config_path(username="default"):
+        if ".conf" not in str(username): username = username+".conf"
+        return os.path.join(Settings.get_base_directory(), "conf/users", username)
+
     def get_username():
         return config["username"] or "default"
 
-    def get_username_onlyfans():
+    def get_username_onlyfans(username=None):
         try:
-            return Settings.get_user_config(Settings.get_username())["onlyfans_username"]
-        except Exception as e:
-            Settings.err_print(e)
+            if not username: username = Settings.get_username()
+            return Settings.get_user_config(username)["onlyfans_username"]
+        except Exception as e: pass
         return ""
 
-    def get_username_google():
+    def get_username_google(username=None):
         try:
-            return Settings.get_user_config(Settings.get_username())["google_username"]
-        except Exception as e:
-            Settings.err_print(e)
+            if not username: username = Settings.get_username()
+            return Settings.get_user_config(username)["google_username"]
+        except Exception as e: pass
         return ""            
 
-    def get_username_twitter():
+    def get_username_twitter(username=None):
         try:
-            return Settings.get_user_config(Settings.get_username())["twitter_username"]
-        except Exception as e:
-            Settings.err_print(e)
+            if not username: username = Settings.get_username()
+            return Settings.get_user_config(username)["twitter_username"]
+        except Exception as e: pass
         return ""
 
     def get_remote_browser_host():
         return config["remote_browser_host"]
 
     def get_remote_browser_port():
         return config["remote_browser_port"]
```

### Comparing `OnlySnarf-4.5.9/OnlySnarf/util/validators.py` & `OnlySnarf-4.6.0/OnlySnarf/util/validators.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.9/OnlySnarf.egg-info/PKG-INFO` & `OnlySnarf-4.6.0/OnlySnarf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OnlySnarf
-Version: 4.5.9
+Version: 4.6.0
 Summary: OnlyFans Content Distribution Tool
 Home-page: https://github.com/skeetzo/onlysnarf
 Author: Skeetzo
 Author-email: WebmasterSkeetzo@gmail.com
 Keywords: OnlyFans,OnlySnarf,selenium,snarf
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: OnlySnarf Version: 4.5.9 Summary: OnlyFans Content
+Metadata-Version: 2.1 Name: OnlySnarf Version: 4.6.0 Summary: OnlyFans Content
 Distribution Tool Home-page: https://github.com/skeetzo/onlysnarf Author:
 Skeetzo Author-email: WebmasterSkeetzo@gmail.com Keywords:
 OnlyFans,OnlySnarf,selenium,snarf Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: System :: Emulators Classifier: License :: OSI Approved ::
 MIT License Classifier: Programming Language :: Python :: 3.8 Classifier:
 Operating System :: OS Independent Description-Content-Type: text/markdown
```

### Comparing `OnlySnarf-4.5.9/OnlySnarf.egg-info/SOURCES.txt` & `OnlySnarf-4.6.0/OnlySnarf.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -2,42 +2,42 @@
 LICENSE.txt
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 OnlySnarf/__init__.py
 OnlySnarf/__main__.py
-OnlySnarf/api.py
-OnlySnarf/menu.py
 OnlySnarf/snarf.py
 OnlySnarf.egg-info/PKG-INFO
 OnlySnarf.egg-info/SOURCES.txt
 OnlySnarf.egg-info/dependency_links.txt
 OnlySnarf.egg-info/entry_points.txt
 OnlySnarf.egg-info/requires.txt
 OnlySnarf.egg-info/top_level.txt
 OnlySnarf/classes/__init__.py
+OnlySnarf/classes/config.py
 OnlySnarf/classes/discount.py
 OnlySnarf/classes/element.py
 OnlySnarf/classes/file.py
 OnlySnarf/classes/message.py
 OnlySnarf/classes/poll.py
 OnlySnarf/classes/profile.py
 OnlySnarf/classes/promotion.py
 OnlySnarf/classes/schedule.py
 OnlySnarf/classes/user.py
-OnlySnarf/conf/config.conf
-OnlySnarf/conf/test-config.conf
+OnlySnarf/conf/users/example-user.conf
 OnlySnarf/elements/__init__.py
 OnlySnarf/elements/driver.py
 OnlySnarf/elements/login.py
 OnlySnarf/elements/profile.py
 OnlySnarf/lib/__init__.py
 OnlySnarf/lib/driver.py
 OnlySnarf/lib/ffmpeg.py
+OnlySnarf/lib/menu.py
+OnlySnarf/server/api.py
 OnlySnarf/util/__init__.py
 OnlySnarf/util/args.py
 OnlySnarf/util/colorize.py
 OnlySnarf/util/config.py
 OnlySnarf/util/defaults.py
 OnlySnarf/util/logger.py
 OnlySnarf/util/optional_args.py
```

### Comparing `OnlySnarf-4.5.9/PKG-INFO` & `OnlySnarf-4.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OnlySnarf
-Version: 4.5.9
+Version: 4.6.0
 Summary: OnlyFans Content Distribution Tool
 Home-page: https://github.com/skeetzo/onlysnarf
 Author: Skeetzo
 Author-email: WebmasterSkeetzo@gmail.com
 Keywords: OnlyFans,OnlySnarf,selenium,snarf
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: OnlySnarf Version: 4.5.9 Summary: OnlyFans Content
+Metadata-Version: 2.1 Name: OnlySnarf Version: 4.6.0 Summary: OnlyFans Content
 Distribution Tool Home-page: https://github.com/skeetzo/onlysnarf Author:
 Skeetzo Author-email: WebmasterSkeetzo@gmail.com Keywords:
 OnlyFans,OnlySnarf,selenium,snarf Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: System :: Emulators Classifier: License :: OSI Approved ::
 MIT License Classifier: Programming Language :: Python :: 3.8 Classifier:
 Operating System :: OS Independent Description-Content-Type: text/markdown
```

### Comparing `OnlySnarf-4.5.9/README.md` & `OnlySnarf-4.6.0/README.md`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.9/setup.py` & `OnlySnarf-4.6.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,43 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="OnlySnarf",
-    version="4.5.9",
+    version="4.6.0",
     author="Skeetzo",
     author_email="WebmasterSkeetzo@gmail.com",
     url = 'https://github.com/skeetzo/onlysnarf',
     keywords = ['OnlyFans', 'OnlySnarf', 'selenium', 'snarf'],
     description="OnlyFans Content Distribution Tool",
     long_description=long_description,
     long_description_content_type="text/markdown",
     # packages=setuptools.find_packages(),
-    packages=["OnlySnarf", "OnlySnarf/classes","OnlySnarf/conf","OnlySnarf/elements","OnlySnarf/lib","OnlySnarf/util"],
+    packages=["OnlySnarf", "OnlySnarf/classes","OnlySnarf/conf","OnlySnarf/elements","OnlySnarf/lib","OnlySnarf/util","OnlySnarf/server"],
     include_package_data=True,
     install_requires=[
         'ffmpeg',
         'inquirer',
         'wget',
         'selenium>=4',
         'webdriver_manager==3.9.0',
         'validators',
         'flask'
-        ],
+    ],
     extras_require={
         'dev': [
             'pytest',
             'flask-unittest'
         ]
     },
     entry_points={
         'console_scripts' : [
-            'onlysnarf = OnlySnarf.menu:main',
-            'snarf = OnlySnarf.snarf:main',
-            'snarfapi = OnlySnarf.api:main'
+            'snarf = OnlySnarf.snarf:main'
         ]
     },
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: End Users/Desktop',
         'Topic :: System :: Emulators',
         'License :: OSI Approved :: MIT License',
```

### Comparing `OnlySnarf-4.5.9/tests/test_profile.py` & `OnlySnarf-4.6.0/tests/test_profile.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.9/tests/test_promotion.py` & `OnlySnarf-4.6.0/tests/test_promotion.py`

 * *Files identical despite different names*

