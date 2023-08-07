# Comparing `tmp/OnlySnarf-4.5.8.tar.gz` & `tmp/OnlySnarf-4.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OnlySnarf-4.5.8.tar", last modified: Wed Aug  2 19:13:12 2023, max compression
+gzip compressed data, was "OnlySnarf-4.5.9.tar", last modified: Fri Aug  4 01:34:54 2023, max compression
```

## Comparing `OnlySnarf-4.5.8.tar` & `OnlySnarf-4.5.9.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-08-02 19:13:12.155930 OnlySnarf-4.5.8/
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    32089 2023-08-02 19:13:00.000000 OnlySnarf-4.5.8/CHANGELOG.md
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1064 2023-04-16 06:45:34.000000 OnlySnarf-4.5.8/LICENSE.txt
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)      141 2023-04-16 06:45:34.000000 OnlySnarf-4.5.8/MANIFEST.in
-drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-08-02 19:13:12.151930 OnlySnarf-4.5.8/OnlySnarf/
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)       75 2023-07-26 00:57:38.000000 OnlySnarf-4.5.8/OnlySnarf/__init__.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)      387 2023-04-16 06:45:34.000000 OnlySnarf-4.5.8/OnlySnarf/__main__.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     2165 2023-08-02 18:50:50.000000 OnlySnarf-4.5.8/OnlySnarf/api.py
-drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-08-02 19:13:12.151930 OnlySnarf-4.5.8/OnlySnarf/classes/
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-16 06:45:34.000000 OnlySnarf-4.5.8/OnlySnarf/classes/__init__.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     4388 2023-04-16 06:45:34.000000 OnlySnarf-4.5.8/OnlySnarf/classes/discount.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1892 2023-04-16 06:45:34.000000 OnlySnarf-4.5.8/OnlySnarf/classes/element.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    16142 2023-07-11 22:15:12.000000 OnlySnarf-4.5.8/OnlySnarf/classes/file.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    12611 2023-07-17 20:29:42.000000 OnlySnarf-4.5.8/OnlySnarf/classes/message.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1986 2023-07-17 07:19:23.000000 OnlySnarf-4.5.8/OnlySnarf/classes/poll.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    14542 2023-05-29 23:06:57.000000 OnlySnarf-4.5.8/OnlySnarf/classes/profile.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    10171 2023-04-16 06:45:34.000000 OnlySnarf-4.5.8/OnlySnarf/classes/promotion.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     4891 2023-07-12 22:40:17.000000 OnlySnarf-4.5.8/OnlySnarf/classes/schedule.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    20341 2023-07-17 21:30:18.000000 OnlySnarf-4.5.8/OnlySnarf/classes/user.py
-drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-08-02 19:13:12.151930 OnlySnarf-4.5.8/OnlySnarf/conf/
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     2249 2023-08-02 18:37:46.000000 OnlySnarf-4.5.8/OnlySnarf/conf/config.conf
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     2353 2023-08-02 18:44:36.000000 OnlySnarf-4.5.8/OnlySnarf/conf/test-config.conf
-drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-08-02 19:13:12.151930 OnlySnarf-4.5.8/OnlySnarf/elements/
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-16 06:45:34.000000 OnlySnarf-4.5.8/OnlySnarf/elements/__init__.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    15689 2023-04-16 06:45:34.000000 OnlySnarf-4.5.8/OnlySnarf/elements/driver.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1401 2023-04-16 06:45:34.000000 OnlySnarf-4.5.8/OnlySnarf/elements/login.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    11335 2023-04-16 06:45:34.000000 OnlySnarf-4.5.8/OnlySnarf/elements/profile.py
-drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-08-02 19:13:12.151930 OnlySnarf-4.5.8/OnlySnarf/lib/
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-16 06:45:34.000000 OnlySnarf-4.5.8/OnlySnarf/lib/__init__.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)   167033 2023-08-02 19:00:43.000000 OnlySnarf-4.5.8/OnlySnarf/lib/driver.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     9500 2023-04-16 06:45:34.000000 OnlySnarf-4.5.8/OnlySnarf/lib/ffmpeg.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     5076 2023-07-17 07:19:23.000000 OnlySnarf-4.5.8/OnlySnarf/menu.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     5006 2023-07-17 07:19:23.000000 OnlySnarf-4.5.8/OnlySnarf/snarf.py
-drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-08-02 19:13:12.155930 OnlySnarf-4.5.8/OnlySnarf/util/
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-16 06:45:34.000000 OnlySnarf-4.5.8/OnlySnarf/util/__init__.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1327 2023-07-17 03:26:29.000000 OnlySnarf-4.5.8/OnlySnarf/util/args.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1062 2023-04-16 06:45:34.000000 OnlySnarf-4.5.8/OnlySnarf/util/colorize.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1591 2023-07-26 01:01:08.000000 OnlySnarf-4.5.8/OnlySnarf/util/config.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     3274 2023-07-17 19:07:11.000000 OnlySnarf-4.5.8/OnlySnarf/util/defaults.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     2025 2023-04-16 06:45:34.000000 OnlySnarf-4.5.8/OnlySnarf/util/logger.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    12451 2023-08-02 18:39:19.000000 OnlySnarf-4.5.8/OnlySnarf/util/optional_args.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    20660 2023-08-02 18:45:04.000000 OnlySnarf-4.5.8/OnlySnarf/util/settings.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     3934 2023-07-11 19:44:50.000000 OnlySnarf-4.5.8/OnlySnarf/util/validators.py
-drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-08-02 19:13:12.151930 OnlySnarf-4.5.8/OnlySnarf.egg-info/
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     4679 2023-08-02 19:13:12.000000 OnlySnarf-4.5.8/OnlySnarf.egg-info/PKG-INFO
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1188 2023-08-02 19:13:12.000000 OnlySnarf-4.5.8/OnlySnarf.egg-info/SOURCES.txt
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        1 2023-08-02 19:13:12.000000 OnlySnarf-4.5.8/OnlySnarf.egg-info/dependency_links.txt
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)      109 2023-08-02 19:13:12.000000 OnlySnarf-4.5.8/OnlySnarf.egg-info/entry_points.txt
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)       94 2023-08-02 19:13:12.000000 OnlySnarf-4.5.8/OnlySnarf.egg-info/requires.txt
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)       91 2023-08-02 19:13:12.000000 OnlySnarf-4.5.8/OnlySnarf.egg-info/top_level.txt
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     4679 2023-08-02 19:13:12.155930 OnlySnarf-4.5.8/PKG-INFO
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     4049 2023-07-06 00:40:42.000000 OnlySnarf-4.5.8/README.md
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)       79 2023-08-02 19:13:12.155930 OnlySnarf-4.5.8/setup.cfg
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1465 2023-08-02 19:13:05.000000 OnlySnarf-4.5.8/setup.py
-drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-08-02 19:13:12.155930 OnlySnarf-4.5.8/tests/
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1209 2023-04-16 06:45:34.000000 OnlySnarf-4.5.8/tests/test_profile.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1451 2023-04-16 06:45:34.000000 OnlySnarf-4.5.8/tests/test_promotion.py
+drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-08-04 01:34:54.789213 OnlySnarf-4.5.9/
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    32332 2023-08-04 01:34:34.000000 OnlySnarf-4.5.9/CHANGELOG.md
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1064 2023-04-16 06:45:34.000000 OnlySnarf-4.5.9/LICENSE.txt
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)      141 2023-04-16 06:45:34.000000 OnlySnarf-4.5.9/MANIFEST.in
+drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-08-04 01:34:54.785213 OnlySnarf-4.5.9/OnlySnarf/
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)       75 2023-07-26 00:57:38.000000 OnlySnarf-4.5.9/OnlySnarf/__init__.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)      387 2023-04-16 06:45:34.000000 OnlySnarf-4.5.9/OnlySnarf/__main__.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     2142 2023-08-03 01:40:40.000000 OnlySnarf-4.5.9/OnlySnarf/api.py
+drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-08-04 01:34:54.785213 OnlySnarf-4.5.9/OnlySnarf/classes/
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-16 06:45:34.000000 OnlySnarf-4.5.9/OnlySnarf/classes/__init__.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     4388 2023-04-16 06:45:34.000000 OnlySnarf-4.5.9/OnlySnarf/classes/discount.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1892 2023-04-16 06:45:34.000000 OnlySnarf-4.5.9/OnlySnarf/classes/element.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    16142 2023-07-11 22:15:12.000000 OnlySnarf-4.5.9/OnlySnarf/classes/file.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    12611 2023-08-02 19:27:24.000000 OnlySnarf-4.5.9/OnlySnarf/classes/message.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1986 2023-07-17 07:19:23.000000 OnlySnarf-4.5.9/OnlySnarf/classes/poll.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    14542 2023-05-29 23:06:57.000000 OnlySnarf-4.5.9/OnlySnarf/classes/profile.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    10171 2023-04-16 06:45:34.000000 OnlySnarf-4.5.9/OnlySnarf/classes/promotion.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     4891 2023-07-12 22:40:17.000000 OnlySnarf-4.5.9/OnlySnarf/classes/schedule.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    20341 2023-08-02 19:27:24.000000 OnlySnarf-4.5.9/OnlySnarf/classes/user.py
+drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-08-04 01:34:54.785213 OnlySnarf-4.5.9/OnlySnarf/conf/
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     2249 2023-08-02 19:27:24.000000 OnlySnarf-4.5.9/OnlySnarf/conf/config.conf
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     2353 2023-08-02 19:27:24.000000 OnlySnarf-4.5.9/OnlySnarf/conf/test-config.conf
+drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-08-04 01:34:54.789213 OnlySnarf-4.5.9/OnlySnarf/elements/
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-16 06:45:34.000000 OnlySnarf-4.5.9/OnlySnarf/elements/__init__.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    15689 2023-04-16 06:45:34.000000 OnlySnarf-4.5.9/OnlySnarf/elements/driver.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1401 2023-04-16 06:45:34.000000 OnlySnarf-4.5.9/OnlySnarf/elements/login.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    11335 2023-04-16 06:45:34.000000 OnlySnarf-4.5.9/OnlySnarf/elements/profile.py
+drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-08-04 01:34:54.789213 OnlySnarf-4.5.9/OnlySnarf/lib/
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-16 06:45:34.000000 OnlySnarf-4.5.9/OnlySnarf/lib/__init__.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)   167866 2023-08-03 01:45:45.000000 OnlySnarf-4.5.9/OnlySnarf/lib/driver.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     9500 2023-04-16 06:45:34.000000 OnlySnarf-4.5.9/OnlySnarf/lib/ffmpeg.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     5076 2023-07-17 07:19:23.000000 OnlySnarf-4.5.9/OnlySnarf/menu.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     5006 2023-07-17 07:19:23.000000 OnlySnarf-4.5.9/OnlySnarf/snarf.py
+drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-08-04 01:34:54.789213 OnlySnarf-4.5.9/OnlySnarf/util/
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-16 06:45:34.000000 OnlySnarf-4.5.9/OnlySnarf/util/__init__.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1327 2023-07-17 03:26:29.000000 OnlySnarf-4.5.9/OnlySnarf/util/args.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1062 2023-04-16 06:45:34.000000 OnlySnarf-4.5.9/OnlySnarf/util/colorize.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1591 2023-08-02 19:27:24.000000 OnlySnarf-4.5.9/OnlySnarf/util/config.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     3283 2023-08-03 01:34:26.000000 OnlySnarf-4.5.9/OnlySnarf/util/defaults.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     2025 2023-04-16 06:45:34.000000 OnlySnarf-4.5.9/OnlySnarf/util/logger.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    12451 2023-08-02 19:27:24.000000 OnlySnarf-4.5.9/OnlySnarf/util/optional_args.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    20703 2023-08-03 01:34:20.000000 OnlySnarf-4.5.9/OnlySnarf/util/settings.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     3934 2023-07-11 19:44:50.000000 OnlySnarf-4.5.9/OnlySnarf/util/validators.py
+drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-08-04 01:34:54.785213 OnlySnarf-4.5.9/OnlySnarf.egg-info/
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     4679 2023-08-04 01:34:54.000000 OnlySnarf-4.5.9/OnlySnarf.egg-info/PKG-INFO
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1188 2023-08-04 01:34:54.000000 OnlySnarf-4.5.9/OnlySnarf.egg-info/SOURCES.txt
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        1 2023-08-04 01:34:54.000000 OnlySnarf-4.5.9/OnlySnarf.egg-info/dependency_links.txt
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)      109 2023-08-04 01:34:54.000000 OnlySnarf-4.5.9/OnlySnarf.egg-info/entry_points.txt
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)      104 2023-08-04 01:34:54.000000 OnlySnarf-4.5.9/OnlySnarf.egg-info/requires.txt
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)       91 2023-08-04 01:34:54.000000 OnlySnarf-4.5.9/OnlySnarf.egg-info/top_level.txt
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     4679 2023-08-04 01:34:54.789213 OnlySnarf-4.5.9/PKG-INFO
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     4049 2023-07-06 00:40:42.000000 OnlySnarf-4.5.9/README.md
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)       79 2023-08-04 01:34:54.789213 OnlySnarf-4.5.9/setup.cfg
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1475 2023-08-04 01:34:31.000000 OnlySnarf-4.5.9/setup.py
+drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-08-04 01:34:54.789213 OnlySnarf-4.5.9/tests/
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1209 2023-04-16 06:45:34.000000 OnlySnarf-4.5.9/tests/test_profile.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1451 2023-04-16 06:45:34.000000 OnlySnarf-4.5.9/tests/test_promotion.py
```

### Comparing `OnlySnarf-4.5.8/CHANGELOG.md` & `OnlySnarf-4.5.9/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -693,39 +693,46 @@
   - fixed get random user for discount test 
 **4.5.0 : 7/11/2023**
   - added wget functionality to input for when a url is provided
   - cleaned up bin/test scripts
   - added basic api setup
   - added test scripts for flask & api
   - beginning modifications for receiving api calls
-**4.5.1 : 7/12/2023**
+  **4.5.1 : 7/12/2023**
   - fixed package req: validators
   - added modifications for running via api
-**4.5.2 : 7/16/2023**
+  **4.5.2 : 7/16/2023**
   - relocated api structure for testing
   - added tests for flask api
   - updates to tests, code flow for missing config / args values
   - added individual message funcationality tests 
-  **7/17/2023**
+    **7/17/2023**
   - continued debugging message tests
   - fixed random user functionality
   - updated driver.poll
   - fixed new message tests
   - added flask to package reqs
   - updated install script
   - updated api scripts to route through snarf
   **4.5.3,4,5,6 : 7/30/2023**
   - api debugging
-  **4.5.7,8 : 8/2/2023**
+**4.5.7,8 : 8/2/2023**
   - fixed twitter login; added phone number to args&config
+  - more api debugging w/ aws
+  - updated date&time formats
+  - debugged api: /message & /post
+**4.5.9 : 8/3/2023**
+  - added update script meant to be run by systemd service script
 
 ------------------------------------------------------------------------------------
 
 ## TODO
 
+- bump minor version for working api
+
 - look into Marshmellow package for class / object cleanup
 
 
 - add smart idea for getting statement information
 - add better version notes to readme's list of "works on"
 - re-add stuff for testing on multiple platforms ala mac ;) 
 
@@ -840,14 +847,18 @@
 chown -R ubuntu /home/ubuntu/.wdm/drivers
 
 what helps in general:
 >> using correct webdriver options generator
 >> specifying binary paths
 >> correct permissions on binary paths
 
+# API
+
+note: the 
+
 # Bugs
 
 **4.1.4**
   - boolean checks from "Settings.is_" functions are failing: replaced with redundant string checks for if == "True"
 **4.3.12**
   - message: drag&drop has decided to occasionally stop working; maybe a selenium version issue?
 **4.4.0**
```

### Comparing `OnlySnarf-4.5.8/LICENSE.txt` & `OnlySnarf-4.5.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.8/OnlySnarf/api.py` & `OnlySnarf-4.5.9/OnlySnarf/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,69 +1,69 @@
+import os
 import json
 from flask import Flask, request
 
 from .util.config import config
 from .util.settings import Settings
 from .snarf import Snarf
 
 def create_app():
     app = Flask(__name__)
 
     @app.route('/message', methods=['POST'])
     def message():
         try:
-            return "", 200
-        finally:
             args = json.loads(request.data)
             Settings.dev_print(args)
             config["text"] = args["text"]
             config["user"] = args["user"]
-            try: config["files"] = args["input"].split(",")
+            try: config["input"] = args["input"].split(",")
             except Exception as e: pass
             try: config["price"] = args["price"] or 0
             except Exception as e: pass
             try: config["schedule"] = args["schedule"]
             except Exception as e: pass
             try: config["performers"] = args["performers"]
             except Exception as e: pass
-            if app.testing:
-                config["debug"] = True
-                config["verbose"] = 3
             Snarf.message()
             Snarf.close()
+        except Exception as e:
+            Settings.dev_print(e)
+        finally:
+            return "", 200
 
     @app.route('/post', methods=['POST'])
     def post():
         try:
-            return "", 200
-        finally:
             args = json.loads(request.data)
             Settings.dev_print(args)
             config["text"] = args["text"]
-            try: config["files"] = args["input"].split(",")
+            try: config["input"] = args["input"].split(",")
             except Exception as e: pass
             try: config["performers"] = args["performers"]
             except Exception as e: pass
             try: config["schedule"] = args["schedule"]
             except Exception as e: pass
             try: config["questions"] = args["questions"]
             except Exception as e: pass
             try: config["duration"] = args["duration"]
             except Exception as e: pass
             try: config["expires"] = args["expires"]
             except Exception as e: pass
-            if app.testing:
-                config["debug"] = True
-                config["verbose"] = 3
             Snarf.post()
             Snarf.close()
+        except Exception as e:
+            Settings.dev_print(e)
+        finally:
+            return "", 200
 
     return app
 
 def main():
     app = create_app()
-    app.debug = True
-    app.testing = True
+    if str(config["debug"]) == "True":
+        app.debug = True
+        app.testing = True
     app.run(host="0.0.0.0", port=5000)
 
 if __name__ == "__main__":
     main()
```

### Comparing `OnlySnarf-4.5.8/OnlySnarf/classes/discount.py` & `OnlySnarf-4.5.9/OnlySnarf/classes/discount.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.8/OnlySnarf/classes/element.py` & `OnlySnarf-4.5.9/OnlySnarf/classes/element.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.8/OnlySnarf/classes/file.py` & `OnlySnarf-4.5.9/OnlySnarf/classes/file.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.8/OnlySnarf/classes/message.py` & `OnlySnarf-4.5.9/OnlySnarf/classes/message.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.8/OnlySnarf/classes/poll.py` & `OnlySnarf-4.5.9/OnlySnarf/classes/poll.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.8/OnlySnarf/classes/profile.py` & `OnlySnarf-4.5.9/OnlySnarf/classes/profile.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.8/OnlySnarf/classes/promotion.py` & `OnlySnarf-4.5.9/OnlySnarf/classes/promotion.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.8/OnlySnarf/classes/schedule.py` & `OnlySnarf-4.5.9/OnlySnarf/classes/schedule.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.8/OnlySnarf/classes/user.py` & `OnlySnarf-4.5.9/OnlySnarf/classes/user.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.8/OnlySnarf/conf/config.conf` & `OnlySnarf-4.5.9/OnlySnarf/conf/config.conf`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.8/OnlySnarf/conf/test-config.conf` & `OnlySnarf-4.5.9/OnlySnarf/conf/test-config.conf`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.8/OnlySnarf/elements/driver.py` & `OnlySnarf-4.5.9/OnlySnarf/elements/driver.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.8/OnlySnarf/elements/login.py` & `OnlySnarf-4.5.9/OnlySnarf/elements/login.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.8/OnlySnarf/elements/profile.py` & `OnlySnarf-4.5.9/OnlySnarf/elements/profile.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.8/OnlySnarf/lib/driver.py` & `OnlySnarf-4.5.9/OnlySnarf/lib/driver.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,14 +134,16 @@
         """
 
         self.init()
         if not self.login():
             if str(Settings.is_debug()) == "True":
                 return False
             os._exit(1)
+        if str(Settings.is_cookies()) == "True":
+            self.cookies_save()
         return True
 
     ###################
     ##### Cookies #####
     ###################
 
     def cookies_load(self):
@@ -1025,17 +1027,16 @@
             Force page goto even if already at url
 
         """
 
         def goto():
             Settings.maybe_print("goto -> onlyfans.com")
             try:
+                self.browser.set_page_load_timeout(10)
                 self.browser.get(ONLYFANS_HOME_URL)
-                # element_present = EC.presence_of_element_located((By.CLASS_NAME, Element.get_element_by_name("loginCheck").getClass()))
-                # WebDriverWait(self.browser, 10).until(element_present)
             except TimeoutException:
                 Settings.dev_print("timed out waiting for page to check login element")
             except WebDriverException as e:
                 Settings.dev_print("error fetching home page")
                 Settings.err_print(e)
             # self.open_tab(ONLYFANS_HOME_URL)
             self.handle_alert()
@@ -1253,24 +1254,51 @@
             Returns
             -------
             bool
                 Whether or not the login check was successful
 
             """
 
+
+            def try_phone():
+                Settings.maybe_print("verifying phone number...")
+                element = self.browser.switch_to.active_element
+                element.send_keys(str(Settings.get_phone_number()))
+                element.send_keys(Keys.ENTER)
+
+            # TODO: requires testing, not successfuly receiving email w/ code to test further
+            def try_email():
+                Settings.print("email verification required - please enter the code sent to your email!")
+                element = self.browser.switch_to.active_element
+                element.send_keys(str(input("Enter code: ")))
+                element.send_keys(Keys.SHIFT + Keys.TAB)
+                element.send_keys(Keys.ENTER)
+
             try:
                 Settings.dev_print("waiting for login check...")
                 WebDriverWait(self.browser, 30, poll_frequency=2).until(EC.visibility_of_element_located((By.CLASS_NAME, Element.get_element_by_name("loginCheck").getClass())))
                 Settings.print("OnlyFans login successful!")
                 Settings.dev_print("login successful - {}".format(which))
                 return True
             except TimeoutException as te:
-                Settings.dev_print(str(te))
-                Settings.print("Login Failure: Timed Out! Please check your credentials.")
-                Settings.print(": If the problem persists, OnlySnarf may require an update.")
+                bodyText = self.browser.find_element(By.TAG_NAME, "body").text
+                Settings.dev_print(bodyText)
+                # check for phone number page
+                if "Verify your identity by entering the phone number associated with your Twitter account." in str(bodyText):
+                    try_phone()
+                    login_check(which)
+                # check for email notification
+                elif "Check your email" in str(bodyText):
+                    try_email()
+                    login_check(which)
+                else:
+                    # Settings.dev_print(str(te))
+                    Settings.print("Login Failure: Timed Out! Please check your credentials.")
+                    Settings.print(": If the problem persists, OnlySnarf may require an update.")
+                    # output page text for debugging
                 return False
             except Exception as e:
                 Driver.error_checker(e)
                 Settings.print("OnlyFans login failure: OnlySnarf may require an update")
                 return False
             return True
         
@@ -1404,22 +1432,14 @@
                 self.browser.find_element("name", "session[username_or_email]").send_keys(username)
                 Settings.dev_print("username entered")
                 # fill in password and hit the login button 
                 password_ = self.browser.find_element("name", "session[password]")
                 password_.send_keys(password)
                 Settings.dev_print("password entered")
                 password_.send_keys(Keys.ENTER)
-                # check for phone number page
-                time.sleep(1)
-                if "Verify your identity by entering the phone number associated with your Twitter account." in str(self.browser.find_element(By.TAG_NAME, 'body').text):
-                    Settings.maybe_print("verifying phone number...")
-                    element = self.browser.switch_to.active_element
-                    element.send_keys(str(Settings.get_phone_number()))
-                    element.send_keys(Keys.ENTER)
-                    time.sleep(1)
                 return login_check("twitter")
             except Exception as e:
                 Settings.dev_print("twitter login failure")
                 Driver.error_checker(e)
             return False
 
         # this needs to go after them because they reconnect then need to login check
@@ -3108,15 +3128,17 @@
             if not self.session_id and not self.session_url:
                 Settings.warn_print("unable to read session data!")
                 return None
             Settings.maybe_print("reconnecting to web browser...")
             Settings.dev_print("reconnect id: {}".format(self.session_id))
             Settings.dev_print("reconnect url: {}".format(self.session_url))
             try:
-                browserAttempt = webdriver.Remote(command_executor=self.session_url, desired_capabilities={})
+                options = webdriver.ChromeOptions()
+                add_options(options)
+                browserAttempt = webdriver.Remote(command_executor=self.session_url, options=options)
                 browserAttempt.close()   # this closes the session's window - it is currently the only one, thus the session itself will be auto-killed, yet:
                 # take the session that's already running
                 browserAttempt.session_id = self.session_id
                 browserAttempt.title # fails check with: 'NoneType' object has no attribute 'title'
                 Settings.print("browser reconnected!")
                 return browserAttempt
             except Exception as e:
```

### Comparing `OnlySnarf-4.5.8/OnlySnarf/lib/ffmpeg.py` & `OnlySnarf-4.5.9/OnlySnarf/lib/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.8/OnlySnarf/menu.py` & `OnlySnarf-4.5.9/OnlySnarf/menu.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.8/OnlySnarf/snarf.py` & `OnlySnarf-4.5.9/OnlySnarf/snarf.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.8/OnlySnarf/util/args.py` & `OnlySnarf-4.5.9/OnlySnarf/util/args.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.8/OnlySnarf/util/colorize.py` & `OnlySnarf-4.5.9/OnlySnarf/util/colorize.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.8/OnlySnarf/util/config.py` & `OnlySnarf-4.5.9/OnlySnarf/util/config.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.8/OnlySnarf/util/defaults.py` & `OnlySnarf-4.5.9/OnlySnarf/util/defaults.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 # Defaults 
 ##
 
 ACTIONS = [ "Discount", "Message", "Post", "Profile", "Promotion" ]
 
 AMOUNT_NONE = 0
 
-DATE_FORMAT = "%m/%d/%Y"
+DATE_FORMAT = "%Y-%m-%d"
 TIME_FORMAT = "%H:%M:%S"
 SCHEDULE_FORMAT = "{} {}".format(DATE_FORMAT, TIME_FORMAT)
 
 date_ = datetime.strptime(str(datetime.now().strftime(SCHEDULE_FORMAT)), SCHEDULE_FORMAT)
 
-DATE = date_.date().strftime(DATE_FORMAT)
-TIME = date_.time().strftime(TIME_FORMAT)
+DATE = date_.date().strftime(DATE_FORMAT)[:10]
+TIME = date_.time().strftime(TIME_FORMAT)[:9]
 SCHEDULE = date_.strftime(SCHEDULE_FORMAT)
 
 TIME_NONE = "00:00:00"
 
 DEFAULT_MESSAGE = ":)"
 DEFAULT_REFRESHER = "hi!"
 DEFAULT_GREETING = "hi! thanks for subscribing :3 do you have any preferences?"
```

### Comparing `OnlySnarf-4.5.8/OnlySnarf/util/logger.py` & `OnlySnarf-4.5.9/OnlySnarf/util/logger.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.8/OnlySnarf/util/optional_args.py` & `OnlySnarf-4.5.9/OnlySnarf/util/optional_args.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.8/OnlySnarf/util/settings.py` & `OnlySnarf-4.5.9/OnlySnarf/util/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,32 +126,14 @@
 
     def get_price_minimum():
         return DEFAULT.PRICE_MINIMUM
 
     def get_price_maximum():
         return DEFAULT.PRICE_MAXIMUM
 
-    def get_date():
-        try:
-            config["date"] = Settings.format_date(config["date"])
-            if str(config["date"]) == DEFAULT.DATE and str(config["schedule"]) != DEFAULT.SCHEDULE and str(config["schedule"] != "None"):
-                if isinstance(config["schedule"], str):
-                    config["date"] = datetime.strptime(config["schedule"], DEFAULT.SCHEDULE_FORMAT).date().strftime(DEFAULT.DATE_FORMAT)
-                else:
-                    config["date"] = config["schedule"].date().strftime(DEFAULT.DATE_FORMAT)
-                config["date"] = datetime.strptime(str(config["date"]), DEFAULT.DATE_FORMAT)
-            else:
-                config["date"] = datetime.strptime(str(config["date"]), DEFAULT.DATE_FORMAT)
-            config["date"] = config["date"].strftime(DEFAULT.DATE_FORMAT)    
-            Settings.maybe_print("date (settings): {}".format(config["date"]))
-            return config["date"]
-        except Exception as e:
-            pass
-        return datetime.strptime(DEFAULT.DATE, DEFAULT.DATE_FORMAT)
-
     def get_default_greeting():
         return DEFAULT.GREETING or ""
 
     def get_default_refresher():
         return DEFAULT.REFRESHER or ""
         
     def get_discount_max_amount():
@@ -328,59 +310,74 @@
 
     def get_remote_password():
         return config["remote_password"] or ""
 
     def get_profile_method():
         return config["profile_method"] or None
 
+    def get_date():
+        try:
+            config["date"] = Settings.format_date(config["date"])
+            if str(config["date"]) == DEFAULT.DATE and str(config["schedule"]) != DEFAULT.SCHEDULE and str(config["schedule"] != "None"):
+                if isinstance(config["schedule"], str):
+                    config["date"] = datetime.strptime(config["schedule"], DEFAULT.SCHEDULE_FORMAT).date().strftime(DEFAULT.DATE_FORMAT)
+                else:
+                    config["date"] = config["schedule"].date().strftime(DEFAULT.DATE_FORMAT)
+                config["date"] = datetime.strptime(str(config["date"]), DEFAULT.DATE_FORMAT)
+            else:
+                config["date"] = datetime.strptime(str(config["date"]), DEFAULT.DATE_FORMAT)
+            config["date"] = config["date"].strftime(DEFAULT.DATE_FORMAT)    
+        except Exception as e:
+            config["date"] = datetime.strptime(DEFAULT.DATE, DEFAULT.DATE_FORMAT)
+        Settings.maybe_print("date (settings): {}".format(str(config["date"])[:10]))
+        return str(config["date"])[:10]
+
+    def get_time():
+        try:
+            config["time"] = Settings.format_time(config["time"])        
+            if (str(config["time"]) == DEFAULT.TIME or str(config["time"]) == DEFAULT.TIME_NONE) and str(config["schedule"]) != DEFAULT.SCHEDULE and str(config["schedule"]) != "None":
+                Settings.dev_print("time from schedule")
+                date = datetime.strptime(str(config["schedule"]), DEFAULT.SCHEDULE_FORMAT)
+                config["time"] = datetime.strptime(str(date.time().strftime(DEFAULT.TIME_FORMAT)), DEFAULT.TIME_FORMAT)
+            else:
+                Settings.dev_print("time from config")
+                config["time"] = datetime.strptime(str(config["time"]), DEFAULT.TIME_FORMAT)
+            config["time"] = config["time"].strftime(DEFAULT.TIME_FORMAT)
+        except Exception as e:
+            config["time"] = datetime.strptime(DEFAULT.TIME, DEFAULT.TIME_FORMAT).strftime(DEFAULT.TIME_FORMAT)
+        Settings.maybe_print("time (settings): {}".format(str(config["time"])[:9]))
+        return str(config["time"])[:9]
+
     def get_schedule():
         schedule = ""
         try:
             schedule = config["schedule"]
             if str(schedule) == "None": schedule = DEFAULT.SCHEDULE
             if str(schedule) == DEFAULT.SCHEDULE:
                 schedule = datetime.strptime(schedule, DEFAULT.SCHEDULE_FORMAT).strftime(DEFAULT.SCHEDULE_FORMAT)
             elif not isinstance(schedule, str):
                 schedule = schedule.strftime(DEFAULT.SCHEDULE_FORMAT)
-            Settings.maybe_print("schedule (settings): {}".format(schedule))
-            return schedule
         except Exception as e:
-            pass
-        return datetime.strptime("{} {}".format(Settings.get_date(), Settings.get_time()), DEFAULT.SCHEDULE_FORMAT).strftime(DEFAULT.SCHEDULE_FORMAT)
+            schedule = datetime.strptime("{} {}".format(Settings.get_date(), Settings.get_time()), DEFAULT.SCHEDULE_FORMAT).strftime(DEFAULT.SCHEDULE_FORMAT)
+        Settings.maybe_print("schedule (settings): {}".format(schedule))
+        return str(schedule)[:20] # must be less than 19 characters
 
     def get_keywords():
         keywords = []
         try:
             keywords = config["keywords"]
             keywords = [n.strip() for n in keywords]
         except Exception as e:
             pass
             # Settings.err_print(e)
         return keywords
 
     def get_text():
         return config["text"] or ""
 
-    def get_time():
-        try:
-            config["time"] = Settings.format_time(config["time"])        
-            if (str(config["time"]) == DEFAULT.TIME or str(config["time"]) == DEFAULT.TIME_NONE) and str(config["schedule"]) != DEFAULT.SCHEDULE and str(config["schedule"]) != "None":
-                Settings.dev_print("time from schedule")
-                date = datetime.strptime(str(config["schedule"]), DEFAULT.SCHEDULE_FORMAT)
-                config["time"] = datetime.strptime(str(date.time().strftime(DEFAULT.TIME_FORMAT)), DEFAULT.TIME_FORMAT)
-            else:
-                Settings.dev_print("time from config")
-                config["time"] = datetime.strptime(str(config["time"]), DEFAULT.TIME_FORMAT)
-            config["time"] = config["time"].strftime(DEFAULT.TIME_FORMAT)
-            Settings.maybe_print("time (settings): {}".format(config["time"]))
-            return config["time"]
-        except Exception as e:
-            pass
-        return datetime.strptime(DEFAULT.TIME, DEFAULT.TIME_FORMAT).strftime(DEFAULT.TIME_FORMAT)
-
     def get_title():
         return config["title"] or ""
         
     def get_skipped_users():
         return config["skipped_users"] or []
         
     def get_questions():
```

### Comparing `OnlySnarf-4.5.8/OnlySnarf/util/validators.py` & `OnlySnarf-4.5.9/OnlySnarf/util/validators.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.8/OnlySnarf.egg-info/PKG-INFO` & `OnlySnarf-4.5.9/OnlySnarf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OnlySnarf
-Version: 4.5.8
+Version: 4.5.9
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
-Metadata-Version: 2.1 Name: OnlySnarf Version: 4.5.8 Summary: OnlyFans Content
+Metadata-Version: 2.1 Name: OnlySnarf Version: 4.5.9 Summary: OnlyFans Content
 Distribution Tool Home-page: https://github.com/skeetzo/onlysnarf Author:
 Skeetzo Author-email: WebmasterSkeetzo@gmail.com Keywords:
 OnlyFans,OnlySnarf,selenium,snarf Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: System :: Emulators Classifier: License :: OSI Approved ::
 MIT License Classifier: Programming Language :: Python :: 3.8 Classifier:
 Operating System :: OS Independent Description-Content-Type: text/markdown
```

### Comparing `OnlySnarf-4.5.8/OnlySnarf.egg-info/SOURCES.txt` & `OnlySnarf-4.5.9/OnlySnarf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.8/PKG-INFO` & `OnlySnarf-4.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OnlySnarf
-Version: 4.5.8
+Version: 4.5.9
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
-Metadata-Version: 2.1 Name: OnlySnarf Version: 4.5.8 Summary: OnlyFans Content
+Metadata-Version: 2.1 Name: OnlySnarf Version: 4.5.9 Summary: OnlyFans Content
 Distribution Tool Home-page: https://github.com/skeetzo/onlysnarf Author:
 Skeetzo Author-email: WebmasterSkeetzo@gmail.com Keywords:
 OnlyFans,OnlySnarf,selenium,snarf Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: System :: Emulators Classifier: License :: OSI Approved ::
 MIT License Classifier: Programming Language :: Python :: 3.8 Classifier:
 Operating System :: OS Independent Description-Content-Type: text/markdown
```

### Comparing `OnlySnarf-4.5.8/README.md` & `OnlySnarf-4.5.9/README.md`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.8/setup.py` & `OnlySnarf-4.5.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="OnlySnarf",
-    version="4.5.8",
+    version="4.5.9",
     author="Skeetzo",
     author_email="WebmasterSkeetzo@gmail.com",
     url = 'https://github.com/skeetzo/onlysnarf',
     keywords = ['OnlyFans', 'OnlySnarf', 'selenium', 'snarf'],
     description="OnlyFans Content Distribution Tool",
     long_description=long_description,
     long_description_content_type="text/markdown",
     # packages=setuptools.find_packages(),
     packages=["OnlySnarf", "OnlySnarf/classes","OnlySnarf/conf","OnlySnarf/elements","OnlySnarf/lib","OnlySnarf/util"],
     include_package_data=True,
     install_requires=[
         'ffmpeg',
         'inquirer',
         'wget',
-        'selenium',
-        'webdriver_manager',
+        'selenium>=4',
+        'webdriver_manager==3.9.0',
         'validators',
         'flask'
         ],
     extras_require={
         'dev': [
             'pytest',
             'flask-unittest'
```

### Comparing `OnlySnarf-4.5.8/tests/test_profile.py` & `OnlySnarf-4.5.9/tests/test_profile.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.8/tests/test_promotion.py` & `OnlySnarf-4.5.9/tests/test_promotion.py`

 * *Files identical despite different names*

