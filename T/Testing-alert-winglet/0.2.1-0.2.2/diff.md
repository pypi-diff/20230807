# Comparing `tmp/Testing-alert-winglet-0.2.1.tar.gz` & `tmp/Testing-alert-winglet-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Testing-alert-winglet-0.2.1.tar", last modified: Mon Aug  7 18:58:02 2023, max compression
+gzip compressed data, was "Testing-alert-winglet-0.2.2.tar", last modified: Mon Aug  7 19:06:33 2023, max compression
```

## Comparing `Testing-alert-winglet-0.2.1.tar` & `Testing-alert-winglet-0.2.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-08-07 18:58:02.415518 Testing-alert-winglet-0.2.1/
--rw-rw-rw-   0        0        0     1090 2023-07-26 14:10:13.000000 Testing-alert-winglet-0.2.1/LICENSE
--rw-rw-rw-   0        0        0      470 2023-08-07 18:39:30.000000 Testing-alert-winglet-0.2.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2760 2023-08-07 18:58:02.415518 Testing-alert-winglet-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     1737 2023-08-07 17:00:09.000000 Testing-alert-winglet-0.2.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-08-07 18:58:02.392241 Testing-alert-winglet-0.2.1/apps/
-drwxrwxrwx   0        0        0        0 2023-08-07 18:58:02.411325 Testing-alert-winglet-0.2.1/apps/Testing_alert_winglet.egg-info/
--rw-rw-rw-   0        0        0     2760 2023-08-07 18:58:02.000000 Testing-alert-winglet-0.2.1/apps/Testing_alert_winglet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      708 2023-08-07 18:58:02.000000 Testing-alert-winglet-0.2.1/apps/Testing_alert_winglet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-07 18:58:02.000000 Testing-alert-winglet-0.2.1/apps/Testing_alert_winglet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-08-07 18:58:02.000000 Testing-alert-winglet-0.2.1/apps/Testing_alert_winglet.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-08-07 18:58:02.000000 Testing-alert-winglet-0.2.1/apps/Testing_alert_winglet.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-08-07 18:58:02.412366 Testing-alert-winglet-0.2.1/apps/alert_winglet/
--rw-rw-rw-   0        0        0        0 2023-07-26 14:11:02.000000 Testing-alert-winglet-0.2.1/apps/alert_winglet/__init__.py
--rw-rw-rw-   0        0        0      160 2023-07-31 07:24:20.000000 Testing-alert-winglet-0.2.1/apps/alert_winglet/apps.py
-drwxrwxrwx   0        0        0        0 2023-08-07 18:58:02.413406 Testing-alert-winglet-0.2.1/apps/alert_winglet/base/
--rw-rw-rw-   0        0        0        0 2023-07-26 14:11:02.000000 Testing-alert-winglet-0.2.1/apps/alert_winglet/base/__init__.py
--rw-rw-rw-   0        0        0      329 2023-07-26 14:11:02.000000 Testing-alert-winglet-0.2.1/apps/alert_winglet/base/manager.py
--rw-rw-rw-   0        0        0      142 2023-07-26 14:11:02.000000 Testing-alert-winglet-0.2.1/apps/alert_winglet/base/sender.py
-drwxrwxrwx   0        0        0        0 2023-08-07 18:58:02.414479 Testing-alert-winglet-0.2.1/apps/alert_winglet/discord/
--rw-rw-rw-   0        0        0        0 2023-07-26 14:11:02.000000 Testing-alert-winglet-0.2.1/apps/alert_winglet/discord/__init__.py
--rw-rw-rw-   0        0        0     4650 2023-08-07 13:40:43.000000 Testing-alert-winglet-0.2.1/apps/alert_winglet/discord/manager.py
--rw-rw-rw-   0        0        0     4653 2023-08-07 13:40:43.000000 Testing-alert-winglet-0.2.1/apps/alert_winglet/discord/sender.py
-drwxrwxrwx   0        0        0        0 2023-08-07 18:58:02.415518 Testing-alert-winglet-0.2.1/apps/alert_winglet/tests/
--rw-rw-rw-   0        0        0        0 2023-08-07 13:40:43.000000 Testing-alert-winglet-0.2.1/apps/alert_winglet/tests/__init__.py
--rw-rw-rw-   0        0        0     2874 2023-08-07 13:40:43.000000 Testing-alert-winglet-0.2.1/apps/alert_winglet/tests/test_manager.py
--rw-rw-rw-   0        0        0     2051 2023-08-07 13:40:43.000000 Testing-alert-winglet-0.2.1/apps/alert_winglet/tests/test_sender.py
--rw-rw-rw-   0        0        0       94 2023-08-07 18:33:44.000000 Testing-alert-winglet-0.2.1/pyproject.toml
--rw-rw-rw-   0        0        0     1045 2023-08-07 18:58:02.415518 Testing-alert-winglet-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0       98 2023-08-07 18:53:56.000000 Testing-alert-winglet-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 19:06:33.311784 Testing-alert-winglet-0.2.2/
+-rw-rw-rw-   0        0        0     1090 2023-07-26 14:10:13.000000 Testing-alert-winglet-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0      470 2023-08-07 18:59:46.000000 Testing-alert-winglet-0.2.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2904 2023-08-07 19:06:33.311784 Testing-alert-winglet-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1737 2023-08-07 17:00:09.000000 Testing-alert-winglet-0.2.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-08-07 19:06:33.295602 Testing-alert-winglet-0.2.2/apps/
+drwxrwxrwx   0        0        0        0 2023-08-07 19:06:33.311784 Testing-alert-winglet-0.2.2/apps/Testing_alert_winglet.egg-info/
+-rw-rw-rw-   0        0        0     2904 2023-08-07 19:06:33.000000 Testing-alert-winglet-0.2.2/apps/Testing_alert_winglet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      708 2023-08-07 19:06:33.000000 Testing-alert-winglet-0.2.2/apps/Testing_alert_winglet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 19:06:33.000000 Testing-alert-winglet-0.2.2/apps/Testing_alert_winglet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-08-07 19:06:33.000000 Testing-alert-winglet-0.2.2/apps/Testing_alert_winglet.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 19:06:33.000000 Testing-alert-winglet-0.2.2/apps/Testing_alert_winglet.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-07 19:06:33.311784 Testing-alert-winglet-0.2.2/apps/alert_winglet/
+-rw-rw-rw-   0        0        0        0 2023-07-26 14:11:02.000000 Testing-alert-winglet-0.2.2/apps/alert_winglet/__init__.py
+-rw-rw-rw-   0        0        0      160 2023-07-31 07:24:20.000000 Testing-alert-winglet-0.2.2/apps/alert_winglet/apps.py
+drwxrwxrwx   0        0        0        0 2023-08-07 19:06:33.311784 Testing-alert-winglet-0.2.2/apps/alert_winglet/base/
+-rw-rw-rw-   0        0        0        0 2023-07-26 14:11:02.000000 Testing-alert-winglet-0.2.2/apps/alert_winglet/base/__init__.py
+-rw-rw-rw-   0        0        0      329 2023-07-26 14:11:02.000000 Testing-alert-winglet-0.2.2/apps/alert_winglet/base/manager.py
+-rw-rw-rw-   0        0        0      142 2023-07-26 14:11:02.000000 Testing-alert-winglet-0.2.2/apps/alert_winglet/base/sender.py
+drwxrwxrwx   0        0        0        0 2023-08-07 19:06:33.311784 Testing-alert-winglet-0.2.2/apps/alert_winglet/discord/
+-rw-rw-rw-   0        0        0        0 2023-07-26 14:11:02.000000 Testing-alert-winglet-0.2.2/apps/alert_winglet/discord/__init__.py
+-rw-rw-rw-   0        0        0     4650 2023-08-07 13:40:43.000000 Testing-alert-winglet-0.2.2/apps/alert_winglet/discord/manager.py
+-rw-rw-rw-   0        0        0     4653 2023-08-07 13:40:43.000000 Testing-alert-winglet-0.2.2/apps/alert_winglet/discord/sender.py
+drwxrwxrwx   0        0        0        0 2023-08-07 19:06:33.311784 Testing-alert-winglet-0.2.2/apps/alert_winglet/tests/
+-rw-rw-rw-   0        0        0        0 2023-08-07 13:40:43.000000 Testing-alert-winglet-0.2.2/apps/alert_winglet/tests/__init__.py
+-rw-rw-rw-   0        0        0     2874 2023-08-07 13:40:43.000000 Testing-alert-winglet-0.2.2/apps/alert_winglet/tests/test_manager.py
+-rw-rw-rw-   0        0        0     2051 2023-08-07 13:40:43.000000 Testing-alert-winglet-0.2.2/apps/alert_winglet/tests/test_sender.py
+-rw-rw-rw-   0        0        0       94 2023-08-07 18:33:44.000000 Testing-alert-winglet-0.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0     1045 2023-08-07 19:06:33.311784 Testing-alert-winglet-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      280 2023-08-07 19:02:09.000000 Testing-alert-winglet-0.2.2/setup.py
```

### Comparing `Testing-alert-winglet-0.2.1/LICENSE` & `Testing-alert-winglet-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Testing-alert-winglet-0.2.1/PKG-INFO` & `Testing-alert-winglet-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: Testing-alert-winglet
-Version: 0.2.1
+Version: 0.2.2
 Summary: A Django app to send any exception to discord channel.
 Author: Mojtaba
 Author-email: Mojtabadavi14@gmail.com
 License: MIT License
+Project-URL: Issues, https://github.com/Mojitaba34/alert-winglet/issues
+Project-URL: Source Code, https://github.com/Mojitaba34/alert-winglet
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `Testing-alert-winglet-0.2.1/README.rst` & `Testing-alert-winglet-0.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `Testing-alert-winglet-0.2.1/apps/Testing_alert_winglet.egg-info/PKG-INFO` & `Testing-alert-winglet-0.2.2/apps/Testing_alert_winglet.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: Testing-alert-winglet
-Version: 0.2.1
+Version: 0.2.2
 Summary: A Django app to send any exception to discord channel.
 Author: Mojtaba
 Author-email: Mojtabadavi14@gmail.com
 License: MIT License
+Project-URL: Issues, https://github.com/Mojitaba34/alert-winglet/issues
+Project-URL: Source Code, https://github.com/Mojitaba34/alert-winglet
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `Testing-alert-winglet-0.2.1/apps/Testing_alert_winglet.egg-info/SOURCES.txt` & `Testing-alert-winglet-0.2.2/apps/Testing_alert_winglet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Testing-alert-winglet-0.2.1/apps/alert_winglet/discord/manager.py` & `Testing-alert-winglet-0.2.2/apps/alert_winglet/discord/manager.py`

 * *Files identical despite different names*

### Comparing `Testing-alert-winglet-0.2.1/apps/alert_winglet/discord/sender.py` & `Testing-alert-winglet-0.2.2/apps/alert_winglet/discord/sender.py`

 * *Files identical despite different names*

### Comparing `Testing-alert-winglet-0.2.1/apps/alert_winglet/tests/test_manager.py` & `Testing-alert-winglet-0.2.2/apps/alert_winglet/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `Testing-alert-winglet-0.2.1/apps/alert_winglet/tests/test_sender.py` & `Testing-alert-winglet-0.2.2/apps/alert_winglet/tests/test_sender.py`

 * *Files identical despite different names*

### Comparing `Testing-alert-winglet-0.2.1/setup.cfg` & `Testing-alert-winglet-0.2.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2054 6573 7469 6e67 2d61 6c65 7274   = Testing-alert
 00000020: 2d77 696e 676c 6574 0d0a 7665 7273 696f  -winglet..versio
-00000030: 6e20 3d20 302e 322e 310d 0a64 6573 6372  n = 0.2.1..descr
+00000030: 6e20 3d20 302e 322e 320d 0a64 6573 6372  n = 0.2.2..descr
 00000040: 6970 7469 6f6e 203d 2041 2044 6a61 6e67  iption = A Djang
 00000050: 6f20 6170 7020 746f 2073 656e 6420 616e  o app to send an
 00000060: 7920 6578 6365 7074 696f 6e20 746f 2064  y exception to d
 00000070: 6973 636f 7264 2063 6861 6e6e 656c 2e0d  iscord channel..
 00000080: 0a6c 6f6e 675f 6465 7363 7269 7074 696f  .long_descriptio
 00000090: 6e5f 636f 6e74 656e 745f 7479 7065 203d  n_content_type =
 000000a0: 2074 6578 742f 782d 7273 740d 0a6c 6f6e   text/x-rst..lon
```

