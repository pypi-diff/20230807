# Comparing `tmp/arduino_exporter-0.6.0.tar.gz` & `tmp/arduino_exporter-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arduino_exporter-0.6.0.tar", last modified: Sun Jul 30 21:37:27 2023, max compression
+gzip compressed data, was "arduino_exporter-0.6.1.tar", last modified: Mon Aug  7 20:51:28 2023, max compression
```

## Comparing `arduino_exporter-0.6.0.tar` & `arduino_exporter-0.6.1.tar`

### file list

```diff
@@ -1,48 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 21:37:27.738630 arduino_exporter-0.6.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 21:37:27.734630 arduino_exporter-0.6.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-30 21:37:01.000000 arduino_exporter-0.6.0/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-30 21:37:01.000000 arduino_exporter-0.6.0/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 21:37:27.734630 arduino_exporter-0.6.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-30 21:37:01.000000 arduino_exporter-0.6.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-30 21:37:01.000000 arduino_exporter-0.6.0/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 21:37:27.734630 arduino_exporter-0.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-30 21:37:01.000000 arduino_exporter-0.6.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-30 21:37:01.000000 arduino_exporter-0.6.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-30 21:37:01.000000 arduino_exporter-0.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-30 21:37:01.000000 arduino_exporter-0.6.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-30 21:37:01.000000 arduino_exporter-0.6.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-07-30 21:37:01.000000 arduino_exporter-0.6.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-30 21:37:01.000000 arduino_exporter-0.6.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-30 21:37:01.000000 arduino_exporter-0.6.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-30 21:37:01.000000 arduino_exporter-0.6.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-07-30 21:37:27.738630 arduino_exporter-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-07-30 21:37:01.000000 arduino_exporter-0.6.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 21:37:27.734630 arduino_exporter-0.6.0/cache/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-30 21:37:01.000000 arduino_exporter-0.6.0/cache/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 21:37:27.734630 arduino_exporter-0.6.0/deploy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 21:37:01.000000 arduino_exporter-0.6.0/deploy/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-30 21:37:01.000000 arduino_exporter-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-30 21:37:01.000000 arduino_exporter-0.6.0/renovate.json
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-07-30 21:37:27.738630 arduino_exporter-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-30 21:37:01.000000 arduino_exporter-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 21:37:27.730630 arduino_exporter-0.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 21:37:27.734630 arduino_exporter-0.6.0/src/arduino_exporter/
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-07-30 21:37:01.000000 arduino_exporter-0.6.0/src/arduino_exporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-07-30 21:37:01.000000 arduino_exporter-0.6.0/src/arduino_exporter/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 21:37:27.738630 arduino_exporter-0.6.0/src/arduino_exporter/exception/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-30 21:37:01.000000 arduino_exporter-0.6.0/src/arduino_exporter/exception/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7711 2023-07-30 21:37:01.000000 arduino_exporter-0.6.0/src/arduino_exporter/prometheus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-07-30 21:37:01.000000 arduino_exporter-0.6.0/src/arduino_exporter/serial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-07-30 21:37:01.000000 arduino_exporter-0.6.0/src/arduino_exporter/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 21:37:27.738630 arduino_exporter-0.6.0/src/arduino_exporter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-07-30 21:37:27.000000 arduino_exporter-0.6.0/src/arduino_exporter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-30 21:37:27.000000 arduino_exporter-0.6.0/src/arduino_exporter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 21:37:27.000000 arduino_exporter-0.6.0/src/arduino_exporter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-30 21:37:27.000000 arduino_exporter-0.6.0/src/arduino_exporter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 21:37:27.000000 arduino_exporter-0.6.0/src/arduino_exporter.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-30 21:37:27.000000 arduino_exporter-0.6.0/src/arduino_exporter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-30 21:37:27.000000 arduino_exporter-0.6.0/src/arduino_exporter.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 21:37:27.738630 arduino_exporter-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-30 21:37:01.000000 arduino_exporter-0.6.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-30 21:37:01.000000 arduino_exporter-0.6.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-30 21:37:01.000000 arduino_exporter-0.6.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:51:28.985695 arduino_exporter-0.6.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:51:28.969695 arduino_exporter-0.6.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-08-07 20:51:00.000000 arduino_exporter-0.6.1/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-07 20:51:00.000000 arduino_exporter-0.6.1/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:51:28.973695 arduino_exporter-0.6.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-08-07 20:51:00.000000 arduino_exporter-0.6.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-08-07 20:51:00.000000 arduino_exporter-0.6.1/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:51:28.973695 arduino_exporter-0.6.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-08-07 20:51:00.000000 arduino_exporter-0.6.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-08-07 20:51:00.000000 arduino_exporter-0.6.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-08-07 20:51:00.000000 arduino_exporter-0.6.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-07 20:51:00.000000 arduino_exporter-0.6.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-08-07 20:51:00.000000 arduino_exporter-0.6.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-08-07 20:51:00.000000 arduino_exporter-0.6.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-08-07 20:51:00.000000 arduino_exporter-0.6.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-07 20:51:00.000000 arduino_exporter-0.6.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-07 20:51:00.000000 arduino_exporter-0.6.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-08-07 20:51:28.985695 arduino_exporter-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-08-07 20:51:00.000000 arduino_exporter-0.6.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:51:28.973695 arduino_exporter-0.6.1/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-07 20:51:00.000000 arduino_exporter-0.6.1/cache/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:51:28.973695 arduino_exporter-0.6.1/deploy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 20:51:00.000000 arduino_exporter-0.6.1/deploy/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:51:28.957695 arduino_exporter-0.6.1/etc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:51:28.957695 arduino_exporter-0.6.1/etc/systemd/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:51:28.977695 arduino_exporter-0.6.1/etc/systemd/system/
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-08-07 20:51:00.000000 arduino_exporter-0.6.1/etc/systemd/system/arduino_exporter.service
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-08-07 20:51:00.000000 arduino_exporter-0.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-07 20:51:00.000000 arduino_exporter-0.6.1/renovate.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-08-07 20:51:28.989695 arduino_exporter-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-08-07 20:51:00.000000 arduino_exporter-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:51:28.957695 arduino_exporter-0.6.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:51:28.981695 arduino_exporter-0.6.1/src/arduino_exporter/
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-08-07 20:51:00.000000 arduino_exporter-0.6.1/src/arduino_exporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-08-07 20:51:00.000000 arduino_exporter-0.6.1/src/arduino_exporter/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:51:28.985695 arduino_exporter-0.6.1/src/arduino_exporter/exception/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-08-07 20:51:00.000000 arduino_exporter-0.6.1/src/arduino_exporter/exception/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7844 2023-08-07 20:51:00.000000 arduino_exporter-0.6.1/src/arduino_exporter/prometheus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-08-07 20:51:00.000000 arduino_exporter-0.6.1/src/arduino_exporter/serial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-08-07 20:51:00.000000 arduino_exporter-0.6.1/src/arduino_exporter/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:51:28.985695 arduino_exporter-0.6.1/src/arduino_exporter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-08-07 20:51:28.000000 arduino_exporter-0.6.1/src/arduino_exporter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-08-07 20:51:28.000000 arduino_exporter-0.6.1/src/arduino_exporter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 20:51:28.000000 arduino_exporter-0.6.1/src/arduino_exporter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-08-07 20:51:28.000000 arduino_exporter-0.6.1/src/arduino_exporter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 20:51:28.000000 arduino_exporter-0.6.1/src/arduino_exporter.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-08-07 20:51:28.000000 arduino_exporter-0.6.1/src/arduino_exporter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-07 20:51:28.000000 arduino_exporter-0.6.1/src/arduino_exporter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:51:28.985695 arduino_exporter-0.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-08-07 20:51:00.000000 arduino_exporter-0.6.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-08-07 20:51:00.000000 arduino_exporter-0.6.1/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-08-07 20:51:00.000000 arduino_exporter-0.6.1/tox.ini
```

### Comparing `arduino_exporter-0.6.0/.github/workflows/release.yml` & `arduino_exporter-0.6.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `arduino_exporter-0.6.0/.gitignore` & `arduino_exporter-0.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `arduino_exporter-0.6.0/CHANGELOG.rst` & `arduino_exporter-0.6.1/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `arduino_exporter-0.6.0/CODE_OF_CONDUCT.md` & `arduino_exporter-0.6.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `arduino_exporter-0.6.0/CONTRIBUTING.rst` & `arduino_exporter-0.6.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `arduino_exporter-0.6.0/LICENSE.txt` & `arduino_exporter-0.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `arduino_exporter-0.6.0/Makefile` & `arduino_exporter-0.6.1/Makefile`

 * *Files identical despite different names*

### Comparing `arduino_exporter-0.6.0/PKG-INFO` & `arduino_exporter-0.6.1/src/arduino_exporter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: arduino_exporter
-Version: 0.6.0
+Name: arduino-exporter
+Version: 0.6.1
 Summary: Arduino Prometheus Exporter.
 Home-page: https://github.com/clivern/arduino_exporter/
 Author: Clivern
 Author-email: hello@clivern.com
 License: MIT
 Project-URL: Documentation, https://github.com/clivern/arduino_exporter/
 Project-URL: Source, https://github.com/clivern/arduino_exporter/
@@ -51,16 +51,16 @@
     $ pip install arduino-exporter
 
 
 3. To run the arduino exporter process. You can use systemd to run the process on PC or Raspberry PI. The serial port value can be retrieved from arduino IDE.
 
 .. code-block::
 
-    $ arduino_exporter server run -s $serial_port --p $http_port
-    $ arduino_exporter server run -s /dev/cu.usbmodem14101 --p 8000
+    $ arduino_exporter server run -s $serial_port -p $http_port
+    $ arduino_exporter server run -s /dev/cu.usbmodem14101 -p 8000
 
 
 4. Upload a sketch to the arduino to send the metrics to the serial port.
 
 .. code-block::
 
     #define LED 13
```

### Comparing `arduino_exporter-0.6.0/README.rst` & `arduino_exporter-0.6.1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -31,16 +31,16 @@
     $ pip install arduino-exporter
 
 
 3. To run the arduino exporter process. You can use systemd to run the process on PC or Raspberry PI. The serial port value can be retrieved from arduino IDE.
 
 .. code-block::
 
-    $ arduino_exporter server run -s $serial_port --p $http_port
-    $ arduino_exporter server run -s /dev/cu.usbmodem14101 --p 8000
+    $ arduino_exporter server run -s $serial_port -p $http_port
+    $ arduino_exporter server run -s /dev/cu.usbmodem14101 -p 8000
 
 
 4. Upload a sketch to the arduino to send the metrics to the serial port.
 
 .. code-block::
 
     #define LED 13
```

### Comparing `arduino_exporter-0.6.0/setup.cfg` & `arduino_exporter-0.6.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `arduino_exporter-0.6.0/setup.py` & `arduino_exporter-0.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `arduino_exporter-0.6.0/src/arduino_exporter/__init__.py` & `arduino_exporter-0.6.1/src/arduino_exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `arduino_exporter-0.6.0/src/arduino_exporter/cli.py` & `arduino_exporter-0.6.1/src/arduino_exporter/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,14 +58,15 @@
     "port",
     type=click.INT,
     default=8000,
     help="The HTTP server port",
 )
 def run(serial, port):
     try:
+        print(f"Starting server on port {port}")
         server = Server(int(port))
         prometheus = Prometheus()
         serial = Serial(serial)
 
         server.add_callback(lambda: time.sleep(1))
         server.add_callback(lambda: prometheus.store(serial.read()))
         server.run()
```

### Comparing `arduino_exporter-0.6.0/src/arduino_exporter/exception/__init__.py` & `arduino_exporter-0.6.1/src/arduino_exporter/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `arduino_exporter-0.6.0/src/arduino_exporter/prometheus.py` & `arduino_exporter-0.6.1/src/arduino_exporter/prometheus.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,16 +57,20 @@
         if data is None:
             return
 
         # Avoid any bad input
         try:
             item = json.loads(data.strip())
         except Exception:
+            print(f"Invalid data received {data}")
             return
 
+        typ = item["type"]
+        print(f"New metric received with type {typ}")
+
         if "help" not in item.keys():
             item["help"] = ""
 
         if "labels" not in item.keys():
             item["labels"] = {}
 
         if item["type"] == "counter" or item["type"] == "c":
```

### Comparing `arduino_exporter-0.6.0/src/arduino_exporter/serial.py` & `arduino_exporter-0.6.1/src/arduino_exporter/serial.py`

 * *Files identical despite different names*

### Comparing `arduino_exporter-0.6.0/src/arduino_exporter/server.py` & `arduino_exporter-0.6.1/src/arduino_exporter/server.py`

 * *Files identical despite different names*

### Comparing `arduino_exporter-0.6.0/src/arduino_exporter.egg-info/PKG-INFO` & `arduino_exporter-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: arduino-exporter
-Version: 0.6.0
+Name: arduino_exporter
+Version: 0.6.1
 Summary: Arduino Prometheus Exporter.
 Home-page: https://github.com/clivern/arduino_exporter/
 Author: Clivern
 Author-email: hello@clivern.com
 License: MIT
 Project-URL: Documentation, https://github.com/clivern/arduino_exporter/
 Project-URL: Source, https://github.com/clivern/arduino_exporter/
@@ -51,16 +51,16 @@
     $ pip install arduino-exporter
 
 
 3. To run the arduino exporter process. You can use systemd to run the process on PC or Raspberry PI. The serial port value can be retrieved from arduino IDE.
 
 .. code-block::
 
-    $ arduino_exporter server run -s $serial_port --p $http_port
-    $ arduino_exporter server run -s /dev/cu.usbmodem14101 --p 8000
+    $ arduino_exporter server run -s $serial_port -p $http_port
+    $ arduino_exporter server run -s /dev/cu.usbmodem14101 -p 8000
 
 
 4. Upload a sketch to the arduino to send the metrics to the serial port.
 
 .. code-block::
 
     #define LED 13
```

### Comparing `arduino_exporter-0.6.0/src/arduino_exporter.egg-info/SOURCES.txt` & `arduino_exporter-0.6.1/src/arduino_exporter.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 .github/FUNDING.yml
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/feature_request.md
 .github/workflows/ci.yml
 .github/workflows/release.yml
 cache/.gitignore
 deploy/.gitkeep
+etc/systemd/system/arduino_exporter.service
 src/arduino_exporter/__init__.py
 src/arduino_exporter/cli.py
 src/arduino_exporter/prometheus.py
 src/arduino_exporter/serial.py
 src/arduino_exporter/server.py
 src/arduino_exporter.egg-info/PKG-INFO
 src/arduino_exporter.egg-info/SOURCES.txt
```

### Comparing `arduino_exporter-0.6.0/tests/__init__.py` & `arduino_exporter-0.6.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `arduino_exporter-0.6.0/tests/test_client.py` & `arduino_exporter-0.6.1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `arduino_exporter-0.6.0/tox.ini` & `arduino_exporter-0.6.1/tox.ini`

 * *Files identical despite different names*

