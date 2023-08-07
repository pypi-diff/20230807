# Comparing `tmp/runusb-2023.1.1.tar.gz` & `tmp/runusb-2023.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runusb-2023.1.1.tar", last modified: Sun Aug  6 13:15:28 2023, max compression
+gzip compressed data, was "runusb-2023.1.2.tar", last modified: Mon Aug  7 20:17:52 2023, max compression
```

## Comparing `runusb-2023.1.1.tar` & `runusb-2023.1.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 13:15:28.651271 runusb-2023.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 13:15:28.647271 runusb-2023.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 13:15:28.647271 runusb-2023.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-08-06 13:15:06.000000 runusb-2023.1.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-08-06 13:15:06.000000 runusb-2023.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-08-06 13:15:06.000000 runusb-2023.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-08-06 13:15:28.651271 runusb-2023.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-08-06 13:15:06.000000 runusb-2023.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-08-06 13:15:06.000000 runusb-2023.1.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 13:15:28.651271 runusb-2023.1.1/runusb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 13:15:06.000000 runusb-2023.1.1/runusb/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14197 2023-08-06 13:15:06.000000 runusb-2023.1.1/runusb/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 13:15:28.651271 runusb-2023.1.1/runusb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-08-06 13:15:28.000000 runusb-2023.1.1/runusb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-08-06 13:15:28.000000 runusb-2023.1.1/runusb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 13:15:28.000000 runusb-2023.1.1/runusb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-06 13:15:28.000000 runusb-2023.1.1/runusb.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-06 13:15:28.000000 runusb-2023.1.1/runusb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-06 13:15:28.000000 runusb-2023.1.1/runusb.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 13:15:28.647271 runusb-2023.1.1/script/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 13:15:28.651271 runusb-2023.1.1/script/linting/
--rwxr-xr-x   0 runner    (1001) docker     (123)       89 2023-08-06 13:15:06.000000 runusb-2023.1.1/script/linting/lint
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-08-06 13:15:06.000000 runusb-2023.1.1/script/linting/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 13:15:28.651271 runusb-2023.1.1/script/typing/
--rwxr-xr-x   0 runner    (1001) docker     (123)       81 2023-08-06 13:15:06.000000 runusb-2023.1.1/script/typing/check
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-06 13:15:06.000000 runusb-2023.1.1/script/typing/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-08-06 13:15:28.651271 runusb-2023.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 13:15:06.000000 runusb-2023.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 13:15:28.647271 runusb-2023.1.1/stubs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 13:15:28.651271 runusb-2023.1.1/stubs/RPi/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-08-06 13:15:06.000000 runusb-2023.1.1/stubs/RPi/GPIO.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 13:15:06.000000 runusb-2023.1.1/stubs/RPi/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 13:15:28.651271 runusb-2023.1.1/stubs/logger_extras/
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-08-06 13:15:06.000000 runusb-2023.1.1/stubs/logger_extras/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:17:52.341735 runusb-2023.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:17:52.333735 runusb-2023.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:17:52.337735 runusb-2023.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-08-07 20:17:33.000000 runusb-2023.1.2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-08-07 20:17:33.000000 runusb-2023.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-08-07 20:17:33.000000 runusb-2023.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-08-07 20:17:52.341735 runusb-2023.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-08-07 20:17:33.000000 runusb-2023.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-08-07 20:17:33.000000 runusb-2023.1.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:17:52.337735 runusb-2023.1.2/runusb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 20:17:33.000000 runusb-2023.1.2/runusb/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14197 2023-08-07 20:17:33.000000 runusb-2023.1.2/runusb/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:17:52.337735 runusb-2023.1.2/runusb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-08-07 20:17:52.000000 runusb-2023.1.2/runusb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-08-07 20:17:52.000000 runusb-2023.1.2/runusb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 20:17:52.000000 runusb-2023.1.2/runusb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-07 20:17:52.000000 runusb-2023.1.2/runusb.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-07 20:17:52.000000 runusb-2023.1.2/runusb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-07 20:17:52.000000 runusb-2023.1.2/runusb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:17:52.333735 runusb-2023.1.2/script/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:17:52.337735 runusb-2023.1.2/script/linting/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       89 2023-08-07 20:17:33.000000 runusb-2023.1.2/script/linting/lint
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-08-07 20:17:33.000000 runusb-2023.1.2/script/linting/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:17:52.341735 runusb-2023.1.2/script/typing/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       81 2023-08-07 20:17:33.000000 runusb-2023.1.2/script/typing/check
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-07 20:17:33.000000 runusb-2023.1.2/script/typing/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-08-07 20:17:52.341735 runusb-2023.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 20:17:33.000000 runusb-2023.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:17:52.333735 runusb-2023.1.2/stubs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:17:52.341735 runusb-2023.1.2/stubs/RPi/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-08-07 20:17:33.000000 runusb-2023.1.2/stubs/RPi/GPIO.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 20:17:33.000000 runusb-2023.1.2/stubs/RPi/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:17:52.341735 runusb-2023.1.2/stubs/logger_extras/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-08-07 20:17:33.000000 runusb-2023.1.2/stubs/logger_extras/__init__.pyi
```

### Comparing `runusb-2023.1.1/.github/workflows/ci.yml` & `runusb-2023.1.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `runusb-2023.1.1/.gitignore` & `runusb-2023.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `runusb-2023.1.1/LICENSE` & `runusb-2023.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `runusb-2023.1.1/PKG-INFO` & `runusb-2023.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runusb
-Version: 2023.1.1
+Version: 2023.1.2
 Summary: Automagic running of USB sticks
 Home-page: https://github.com/sourcebots/runusb
 Author: "Alistair Lynn"
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: mqtt
```

### Comparing `runusb-2023.1.1/runusb/__main__.py` & `runusb-2023.1.2/runusb/__main__.py`

 * *Files identical despite different names*

### Comparing `runusb-2023.1.1/runusb.egg-info/PKG-INFO` & `runusb-2023.1.2/runusb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runusb
-Version: 2023.1.1
+Version: 2023.1.2
 Summary: Automagic running of USB sticks
 Home-page: https://github.com/sourcebots/runusb
 Author: "Alistair Lynn"
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: mqtt
```

### Comparing `runusb-2023.1.1/setup.cfg` & `runusb-2023.1.2/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 author = "Alistair Lynn"
 url = https://github.com/sourcebots/runusb
 
 [options]
 python_requires = >=3.8
 packages = find:
 install_requires = 
-	logger-extras==0.3.3
+	logger-extras==0.3.4
 	rpi.GPIO==0.7.1
 
 [options.extras_require]
-mqtt = logger-extras[mqtt]==0.3.3
+mqtt = logger-extras[mqtt]==0.3.4
 
 [options.entry_points]
 console_scripts = 
 	runusb = runusb.__main__:main
 
 [flake8]
 exclude =
```

### Comparing `runusb-2023.1.1/stubs/logger_extras/__init__.pyi` & `runusb-2023.1.2/stubs/logger_extras/__init__.pyi`

 * *Files identical despite different names*

