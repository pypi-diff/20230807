# Comparing `tmp/pyserialsensors-0.9.8.tar.gz` & `tmp/pyserialsensors-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyserialsensors-0.9.8.tar", last modified: Thu Jun 24 06:56:07 2021, max compression
+gzip compressed data, was "dist/pyserialsensors-0.9.9.tar", last modified: Thu Jun 24 07:01:59 2021, max compression
```

## Comparing `pyserialsensors-0.9.8.tar` & `pyserialsensors-0.9.9.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxrwxr-x   0 niehaus   (1000) niehaus   (1000)        0 2021-06-24 06:56:07.955113 pyserialsensors-0.9.8/
--rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      267 2021-04-11 16:06:30.000000 pyserialsensors-0.9.8/AUTHORS.rst
--rw-rw-r--   0 niehaus   (1000) niehaus   (1000)     3702 2021-06-23 21:28:40.000000 pyserialsensors-0.9.8/CONTRIBUTING.rst
--rw-rw-r--   0 niehaus   (1000) niehaus   (1000)       89 2021-03-23 22:25:47.000000 pyserialsensors-0.9.8/HISTORY.rst
--rw-rw-r--   0 niehaus   (1000) niehaus   (1000)     1068 2021-03-23 20:55:54.000000 pyserialsensors-0.9.8/LICENSE
--rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      357 2021-03-23 19:38:37.000000 pyserialsensors-0.9.8/MANIFEST.in
--rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      926 2021-06-24 06:56:07.955113 pyserialsensors-0.9.8/PKG-INFO
--rw-rw-r--   0 niehaus   (1000) niehaus   (1000)     1542 2021-06-23 21:28:40.000000 pyserialsensors-0.9.8/README.rst
-drwxrwxr-x   0 niehaus   (1000) niehaus   (1000)        0 2021-06-24 06:56:07.955113 pyserialsensors-0.9.8/docs/
--rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      711 2021-03-23 19:38:37.000000 pyserialsensors-0.9.8/docs/Makefile
--rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      123 2021-03-23 19:38:37.000000 pyserialsensors-0.9.8/docs/authors.rst
--rwxrwxr-x   0 niehaus   (1000) niehaus   (1000)     5055 2021-06-23 21:28:40.000000 pyserialsensors-0.9.8/docs/conf.py
--rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      128 2021-03-23 19:38:37.000000 pyserialsensors-0.9.8/docs/contributing.rst
--rw-rw-r--   0 niehaus   (1000) niehaus   (1000)     1858 2021-03-23 19:38:37.000000 pyserialsensors-0.9.8/docs/defs.rst
--rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      450 2021-03-23 19:38:37.000000 pyserialsensors-0.9.8/docs/hardware.rst
--rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      123 2021-03-23 19:38:37.000000 pyserialsensors-0.9.8/docs/history.rst
--rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      506 2021-03-23 19:38:37.000000 pyserialsensors-0.9.8/docs/index.rst
--rw-rw-r--   0 niehaus   (1000) niehaus   (1000)     1281 2021-03-23 19:38:37.000000 pyserialsensors-0.9.8/docs/installation.rst
--rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      872 2021-03-23 19:38:37.000000 pyserialsensors-0.9.8/docs/make.bat
--rw-rw-r--   0 niehaus   (1000) niehaus   (1000)       82 2021-03-23 22:22:34.000000 pyserialsensors-0.9.8/docs/modules.rst
--rw-rw-r--   0 niehaus   (1000) niehaus   (1000)     1302 2021-03-23 20:11:58.000000 pyserialsensors-0.9.8/docs/pyserialsensors.core.rst
--rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      452 2021-03-23 20:11:58.000000 pyserialsensors-0.9.8/docs/pyserialsensors.devices.nau7802.rst
--rw-rw-r--   0 niehaus   (1000) niehaus   (1000)     2332 2021-03-23 20:11:58.000000 pyserialsensors-0.9.8/docs/pyserialsensors.devices.rst
--rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      633 2021-03-23 20:11:58.000000 pyserialsensors-0.9.8/docs/pyserialsensors.devices.sdp.rst
--rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      860 2021-03-23 20:11:58.000000 pyserialsensors-0.9.8/docs/pyserialsensors.examples.rst
--rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      293 2021-03-23 22:22:34.000000 pyserialsensors-0.9.8/docs/pyserialsensors.rst
--rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      122 2021-03-23 19:38:37.000000 pyserialsensors-0.9.8/docs/readme.rst
-drwxrwxr-x   0 niehaus   (1000) niehaus   (1000)        0 2021-06-24 06:56:07.955113 pyserialsensors-0.9.8/docs/sensors/
--rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      279 2021-03-23 19:38:37.000000 pyserialsensors-0.9.8/docs/sensors/ads1015.rst
--rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      306 2021-03-23 19:38:37.000000 pyserialsensors-0.9.8/docs/sensors/bme280.rst
--rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      290 2021-03-23 19:38:37.000000 pyserialsensors-0.9.8/docs/sensors/max31865.rst
--rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      322 2021-03-23 19:38:51.000000 pyserialsensors-0.9.8/docs/sensors/nau7802.rst
--rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      244 2021-03-23 19:38:37.000000 pyserialsensors-0.9.8/docs/sensors/pac30x5.rst
--rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      269 2021-03-23 19:38:37.000000 pyserialsensors-0.9.8/docs/sensors/scd30.rst
--rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      294 2021-03-23 19:38:37.000000 pyserialsensors-0.9.8/docs/sensors/sdp8xx.rst
--rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      278 2021-03-23 19:38:37.000000 pyserialsensors-0.9.8/docs/sensors/sfm3xxx.rst
--rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      290 2021-03-23 19:38:37.000000 pyserialsensors-0.9.8/docs/sensors/shtxx.rst
--rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      319 2021-03-23 19:38:37.000000 pyserialsensors-0.9.8/docs/sensors.rst
--rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      180 2021-03-23 19:38:37.000000 pyserialsensors-0.9.8/docs/usage.rst
-drwxrwxr-x   0 niehaus   (1000) niehaus   (1000)        0 2021-06-24 06:56:07.955113 pyserialsensors-0.9.8/pyserialsensors/
--rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      117 2021-06-24 06:55:54.000000 pyserialsensors-0.9.8/pyserialsensors/__init__.py
-drwxrwxr-x   0 niehaus   (1000) niehaus   (1000)        0 2021-06-24 06:56:07.955113 pyserialsensors-0.9.8/pyserialsensors/core/
--rw-r--r--   0 niehaus   (1000) niehaus   (1000)       94 2021-05-11 20:46:23.000000 pyserialsensors-0.9.8/pyserialsensors/core/__init__.py
--rw-rw-r--   0 niehaus   (1000) niehaus   (1000)     1577 2021-06-23 21:45:06.000000 pyserialsensors-0.9.8/pyserialsensors/core/comPortController.py
--rw-r--r--   0 niehaus   (1000) niehaus   (1000)     3556 2021-05-11 20:46:23.000000 pyserialsensors-0.9.8/pyserialsensors/core/error.py
--rw-rw-r--   0 niehaus   (1000) niehaus   (1000)     3338 2021-06-23 22:00:21.000000 pyserialsensors-0.9.8/pyserialsensors/core/i2controller.py
--rw-rw-r--   0 niehaus   (1000) niehaus   (1000)     2855 2021-06-23 21:45:09.000000 pyserialsensors-0.9.8/pyserialsensors/core/i2cscan.py
--rw-rw-r--   0 niehaus   (1000) niehaus   (1000)    17537 2021-06-24 06:21:26.000000 pyserialsensors-0.9.8/pyserialsensors/core/sensor.py
--rw-rw-r--   0 niehaus   (1000) niehaus   (1000)     9271 2021-06-24 06:52:09.000000 pyserialsensors-0.9.8/pyserialsensors/core/toolbox.py
-drwxrwxr-x   0 niehaus   (1000) niehaus   (1000)        0 2021-06-24 06:56:07.955113 pyserialsensors-0.9.8/pyserialsensors/devices/
--rw-r--r--   0 niehaus   (1000) niehaus   (1000)     5417 2021-06-23 22:08:45.000000 pyserialsensors-0.9.8/pyserialsensors/devices/FTDI.py
--rw-rw-r--   0 niehaus   (1000) niehaus   (1000)     7185 2021-06-23 21:45:09.000000 pyserialsensors-0.9.8/pyserialsensors/devices/MUX.py
--rw-r--r--   0 niehaus   (1000) niehaus   (1000)       94 2021-05-11 20:46:23.000000 pyserialsensors-0.9.8/pyserialsensors/devices/__init__.py
--rw-r--r--   0 niehaus   (1000) niehaus   (1000)    11393 2021-05-11 20:46:23.000000 pyserialsensors-0.9.8/pyserialsensors/devices/ads1015.py
--rw-r--r--   0 niehaus   (1000) niehaus   (1000)    17834 2021-05-11 20:46:23.000000 pyserialsensors-0.9.8/pyserialsensors/devices/bme280.py
--rw-rw-r--   0 niehaus   (1000) niehaus   (1000)     7900 2021-06-24 06:21:20.000000 pyserialsensors-0.9.8/pyserialsensors/devices/max31865.py
-drwxrwxr-x   0 niehaus   (1000) niehaus   (1000)        0 2021-06-24 06:56:07.955113 pyserialsensors-0.9.8/pyserialsensors/devices/nau7802/
--rw-r--r--   0 niehaus   (1000) niehaus   (1000)       94 2021-05-11 20:46:23.000000 pyserialsensors-0.9.8/pyserialsensors/devices/nau7802/__init__.py
--rw-r--r--   0 niehaus   (1000) niehaus   (1000)    18811 2021-05-11 20:46:23.000000 pyserialsensors-0.9.8/pyserialsensors/devices/nau7802/nau7802.py
--rw-r--r--   0 niehaus   (1000) niehaus   (1000)     6226 2021-05-11 20:46:23.000000 pyserialsensors-0.9.8/pyserialsensors/devices/qwiicrelay.py
--rw-r--r--   0 niehaus   (1000) niehaus   (1000)    10249 2021-05-11 20:46:23.000000 pyserialsensors-0.9.8/pyserialsensors/devices/s8000.py
--rw-rw-r--   0 niehaus   (1000) niehaus   (1000)     9538 2021-06-23 21:45:09.000000 pyserialsensors-0.9.8/pyserialsensors/devices/scd30.py
-drwxrwxr-x   0 niehaus   (1000) niehaus   (1000)        0 2021-06-24 06:56:07.955113 pyserialsensors-0.9.8/pyserialsensors/devices/sdp/
--rw-r--r--   0 niehaus   (1000) niehaus   (1000)       94 2021-05-11 20:46:23.000000 pyserialsensors-0.9.8/pyserialsensors/devices/sdp/__init__.py
--rw-r--r--   0 niehaus   (1000) niehaus   (1000)     6792 2021-05-11 20:46:23.000000 pyserialsensors-0.9.8/pyserialsensors/devices/sdp/sdp8xx.py
--rw-r--r--   0 niehaus   (1000) niehaus   (1000)     5409 2021-05-11 20:46:23.000000 pyserialsensors-0.9.8/pyserialsensors/devices/sfm3xxx.py
--rw-r--r--   0 niehaus   (1000) niehaus   (1000)     4711 2021-05-11 20:46:23.000000 pyserialsensors-0.9.8/pyserialsensors/devices/shtxx.py
--rw-rw-r--   0 niehaus   (1000) niehaus   (1000)    11625 2021-06-23 21:45:09.000000 pyserialsensors-0.9.8/pyserialsensors/devices/smgair2.py
--rw-rw-r--   0 niehaus   (1000) niehaus   (1000)     8545 2021-06-23 21:45:09.000000 pyserialsensors-0.9.8/pyserialsensors/devices/sps30.py
-drwxrwxr-x   0 niehaus   (1000) niehaus   (1000)        0 2021-06-24 06:56:07.955113 pyserialsensors-0.9.8/pyserialsensors/examples/
--rw-r--r--   0 niehaus   (1000) niehaus   (1000)       94 2021-05-11 20:46:23.000000 pyserialsensors-0.9.8/pyserialsensors/examples/__init__.py
--rwxrwxr-x   0 niehaus   (1000) niehaus   (1000)     2841 2021-06-23 21:45:06.000000 pyserialsensors-0.9.8/pyserialsensors/examples/example_mean.py
--rwxrwxr-x   0 niehaus   (1000) niehaus   (1000)     4600 2021-06-23 22:07:47.000000 pyserialsensors-0.9.8/pyserialsensors/examples/example_single_read.py
--rw-r--r--   0 niehaus   (1000) niehaus   (1000)      669 2021-05-11 20:46:23.000000 pyserialsensors-0.9.8/pyserialsensors/examples/example_uart.py
-drwxrwxr-x   0 niehaus   (1000) niehaus   (1000)        0 2021-06-24 06:56:07.955113 pyserialsensors-0.9.8/pyserialsensors/tests/
--rw-r--r--   0 niehaus   (1000) niehaus   (1000)       94 2021-05-11 20:46:23.000000 pyserialsensors-0.9.8/pyserialsensors/tests/__init__.py
--rw-r--r--   0 niehaus   (1000) niehaus   (1000)      378 2021-05-11 20:46:23.000000 pyserialsensors-0.9.8/pyserialsensors/tests/test_comPort.py
--rw-r--r--   0 niehaus   (1000) niehaus   (1000)     4620 2021-05-11 20:46:23.000000 pyserialsensors-0.9.8/pyserialsensors/tests/test_sensor_s8000.py
--rw-r--r--   0 niehaus   (1000) niehaus   (1000)     1922 2021-05-11 20:46:23.000000 pyserialsensors-0.9.8/pyserialsensors/tests/test_sensor_smgair.py
-drwxrwxr-x   0 niehaus   (1000) niehaus   (1000)        0 2021-06-24 06:56:07.955113 pyserialsensors-0.9.8/pyserialsensors/tools/
--rw-r--r--   0 niehaus   (1000) niehaus   (1000)        0 2021-05-11 20:46:23.000000 pyserialsensors-0.9.8/pyserialsensors/tools/__init__.py
--rw-r--r--   0 niehaus   (1000) niehaus   (1000)     2079 2021-05-11 20:46:23.000000 pyserialsensors-0.9.8/pyserialsensors/tools/bulk.py
-drwxrwxr-x   0 niehaus   (1000) niehaus   (1000)        0 2021-06-24 06:56:07.955113 pyserialsensors-0.9.8/pyserialsensors.egg-info/
--rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      926 2021-06-24 06:56:07.000000 pyserialsensors-0.9.8/pyserialsensors.egg-info/PKG-INFO
--rw-rw-r--   0 niehaus   (1000) niehaus   (1000)     2199 2021-06-24 06:56:07.000000 pyserialsensors-0.9.8/pyserialsensors.egg-info/SOURCES.txt
--rw-rw-r--   0 niehaus   (1000) niehaus   (1000)        1 2021-06-24 06:56:07.000000 pyserialsensors-0.9.8/pyserialsensors.egg-info/dependency_links.txt
--rw-rw-r--   0 niehaus   (1000) niehaus   (1000)       77 2021-06-24 06:56:07.000000 pyserialsensors-0.9.8/pyserialsensors.egg-info/requires.txt
--rw-rw-r--   0 niehaus   (1000) niehaus   (1000)       16 2021-06-24 06:56:07.000000 pyserialsensors-0.9.8/pyserialsensors.egg-info/top_level.txt
--rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      455 2021-06-24 06:56:07.959113 pyserialsensors-0.9.8/setup.cfg
--rw-rw-r--   0 niehaus   (1000) niehaus   (1000)     1428 2021-06-24 06:55:54.000000 pyserialsensors-0.9.8/setup.py
+drwxrwxr-x   0 niehaus   (1000) niehaus   (1000)        0 2021-06-24 07:01:59.369518 pyserialsensors-0.9.9/
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      267 2021-04-11 16:06:30.000000 pyserialsensors-0.9.9/AUTHORS.rst
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)     3702 2021-06-23 21:28:40.000000 pyserialsensors-0.9.9/CONTRIBUTING.rst
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)       89 2021-03-23 22:25:47.000000 pyserialsensors-0.9.9/HISTORY.rst
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)     1068 2021-03-23 20:55:54.000000 pyserialsensors-0.9.9/LICENSE
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      357 2021-03-23 19:38:37.000000 pyserialsensors-0.9.9/MANIFEST.in
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      926 2021-06-24 07:01:59.369518 pyserialsensors-0.9.9/PKG-INFO
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)     1542 2021-06-23 21:28:40.000000 pyserialsensors-0.9.9/README.rst
+drwxrwxr-x   0 niehaus   (1000) niehaus   (1000)        0 2021-06-24 07:01:59.365518 pyserialsensors-0.9.9/docs/
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      711 2021-03-23 19:38:37.000000 pyserialsensors-0.9.9/docs/Makefile
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      123 2021-03-23 19:38:37.000000 pyserialsensors-0.9.9/docs/authors.rst
+-rwxrwxr-x   0 niehaus   (1000) niehaus   (1000)     5055 2021-06-23 21:28:40.000000 pyserialsensors-0.9.9/docs/conf.py
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      128 2021-03-23 19:38:37.000000 pyserialsensors-0.9.9/docs/contributing.rst
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)     1858 2021-03-23 19:38:37.000000 pyserialsensors-0.9.9/docs/defs.rst
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      450 2021-03-23 19:38:37.000000 pyserialsensors-0.9.9/docs/hardware.rst
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      123 2021-03-23 19:38:37.000000 pyserialsensors-0.9.9/docs/history.rst
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      506 2021-03-23 19:38:37.000000 pyserialsensors-0.9.9/docs/index.rst
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)     1281 2021-03-23 19:38:37.000000 pyserialsensors-0.9.9/docs/installation.rst
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      872 2021-03-23 19:38:37.000000 pyserialsensors-0.9.9/docs/make.bat
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)       82 2021-03-23 22:22:34.000000 pyserialsensors-0.9.9/docs/modules.rst
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)     1302 2021-03-23 20:11:58.000000 pyserialsensors-0.9.9/docs/pyserialsensors.core.rst
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      452 2021-03-23 20:11:58.000000 pyserialsensors-0.9.9/docs/pyserialsensors.devices.nau7802.rst
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)     2332 2021-03-23 20:11:58.000000 pyserialsensors-0.9.9/docs/pyserialsensors.devices.rst
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      633 2021-03-23 20:11:58.000000 pyserialsensors-0.9.9/docs/pyserialsensors.devices.sdp.rst
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      860 2021-03-23 20:11:58.000000 pyserialsensors-0.9.9/docs/pyserialsensors.examples.rst
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      293 2021-03-23 22:22:34.000000 pyserialsensors-0.9.9/docs/pyserialsensors.rst
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      122 2021-03-23 19:38:37.000000 pyserialsensors-0.9.9/docs/readme.rst
+drwxrwxr-x   0 niehaus   (1000) niehaus   (1000)        0 2021-06-24 07:01:59.365518 pyserialsensors-0.9.9/docs/sensors/
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      279 2021-03-23 19:38:37.000000 pyserialsensors-0.9.9/docs/sensors/ads1015.rst
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      306 2021-03-23 19:38:37.000000 pyserialsensors-0.9.9/docs/sensors/bme280.rst
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      290 2021-03-23 19:38:37.000000 pyserialsensors-0.9.9/docs/sensors/max31865.rst
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      322 2021-03-23 19:38:51.000000 pyserialsensors-0.9.9/docs/sensors/nau7802.rst
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      244 2021-03-23 19:38:37.000000 pyserialsensors-0.9.9/docs/sensors/pac30x5.rst
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      269 2021-03-23 19:38:37.000000 pyserialsensors-0.9.9/docs/sensors/scd30.rst
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      294 2021-03-23 19:38:37.000000 pyserialsensors-0.9.9/docs/sensors/sdp8xx.rst
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      278 2021-03-23 19:38:37.000000 pyserialsensors-0.9.9/docs/sensors/sfm3xxx.rst
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      290 2021-03-23 19:38:37.000000 pyserialsensors-0.9.9/docs/sensors/shtxx.rst
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      319 2021-03-23 19:38:37.000000 pyserialsensors-0.9.9/docs/sensors.rst
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      180 2021-03-23 19:38:37.000000 pyserialsensors-0.9.9/docs/usage.rst
+drwxrwxr-x   0 niehaus   (1000) niehaus   (1000)        0 2021-06-24 07:01:59.365518 pyserialsensors-0.9.9/pyserialsensors/
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      117 2021-06-24 07:01:47.000000 pyserialsensors-0.9.9/pyserialsensors/__init__.py
+drwxrwxr-x   0 niehaus   (1000) niehaus   (1000)        0 2021-06-24 07:01:59.369518 pyserialsensors-0.9.9/pyserialsensors/core/
+-rw-r--r--   0 niehaus   (1000) niehaus   (1000)       94 2021-05-11 20:46:23.000000 pyserialsensors-0.9.9/pyserialsensors/core/__init__.py
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)     1577 2021-06-23 21:45:06.000000 pyserialsensors-0.9.9/pyserialsensors/core/comPortController.py
+-rw-r--r--   0 niehaus   (1000) niehaus   (1000)     3556 2021-05-11 20:46:23.000000 pyserialsensors-0.9.9/pyserialsensors/core/error.py
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)     3338 2021-06-23 22:00:21.000000 pyserialsensors-0.9.9/pyserialsensors/core/i2controller.py
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)     2855 2021-06-23 21:45:09.000000 pyserialsensors-0.9.9/pyserialsensors/core/i2cscan.py
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)    17537 2021-06-24 06:21:26.000000 pyserialsensors-0.9.9/pyserialsensors/core/sensor.py
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)     9259 2021-06-24 07:01:09.000000 pyserialsensors-0.9.9/pyserialsensors/core/toolbox.py
+drwxrwxr-x   0 niehaus   (1000) niehaus   (1000)        0 2021-06-24 07:01:59.369518 pyserialsensors-0.9.9/pyserialsensors/devices/
+-rw-r--r--   0 niehaus   (1000) niehaus   (1000)     5417 2021-06-23 22:08:45.000000 pyserialsensors-0.9.9/pyserialsensors/devices/FTDI.py
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)     7185 2021-06-23 21:45:09.000000 pyserialsensors-0.9.9/pyserialsensors/devices/MUX.py
+-rw-r--r--   0 niehaus   (1000) niehaus   (1000)       94 2021-05-11 20:46:23.000000 pyserialsensors-0.9.9/pyserialsensors/devices/__init__.py
+-rw-r--r--   0 niehaus   (1000) niehaus   (1000)    11393 2021-05-11 20:46:23.000000 pyserialsensors-0.9.9/pyserialsensors/devices/ads1015.py
+-rw-r--r--   0 niehaus   (1000) niehaus   (1000)    17834 2021-05-11 20:46:23.000000 pyserialsensors-0.9.9/pyserialsensors/devices/bme280.py
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)     7900 2021-06-24 06:21:20.000000 pyserialsensors-0.9.9/pyserialsensors/devices/max31865.py
+drwxrwxr-x   0 niehaus   (1000) niehaus   (1000)        0 2021-06-24 07:01:59.369518 pyserialsensors-0.9.9/pyserialsensors/devices/nau7802/
+-rw-r--r--   0 niehaus   (1000) niehaus   (1000)       94 2021-05-11 20:46:23.000000 pyserialsensors-0.9.9/pyserialsensors/devices/nau7802/__init__.py
+-rw-r--r--   0 niehaus   (1000) niehaus   (1000)    18811 2021-05-11 20:46:23.000000 pyserialsensors-0.9.9/pyserialsensors/devices/nau7802/nau7802.py
+-rw-r--r--   0 niehaus   (1000) niehaus   (1000)     6226 2021-05-11 20:46:23.000000 pyserialsensors-0.9.9/pyserialsensors/devices/qwiicrelay.py
+-rw-r--r--   0 niehaus   (1000) niehaus   (1000)    10249 2021-05-11 20:46:23.000000 pyserialsensors-0.9.9/pyserialsensors/devices/s8000.py
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)     9538 2021-06-23 21:45:09.000000 pyserialsensors-0.9.9/pyserialsensors/devices/scd30.py
+drwxrwxr-x   0 niehaus   (1000) niehaus   (1000)        0 2021-06-24 07:01:59.369518 pyserialsensors-0.9.9/pyserialsensors/devices/sdp/
+-rw-r--r--   0 niehaus   (1000) niehaus   (1000)       94 2021-05-11 20:46:23.000000 pyserialsensors-0.9.9/pyserialsensors/devices/sdp/__init__.py
+-rw-r--r--   0 niehaus   (1000) niehaus   (1000)     6792 2021-05-11 20:46:23.000000 pyserialsensors-0.9.9/pyserialsensors/devices/sdp/sdp8xx.py
+-rw-r--r--   0 niehaus   (1000) niehaus   (1000)     5409 2021-05-11 20:46:23.000000 pyserialsensors-0.9.9/pyserialsensors/devices/sfm3xxx.py
+-rw-r--r--   0 niehaus   (1000) niehaus   (1000)     4711 2021-05-11 20:46:23.000000 pyserialsensors-0.9.9/pyserialsensors/devices/shtxx.py
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)    11625 2021-06-23 21:45:09.000000 pyserialsensors-0.9.9/pyserialsensors/devices/smgair2.py
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)     8545 2021-06-23 21:45:09.000000 pyserialsensors-0.9.9/pyserialsensors/devices/sps30.py
+drwxrwxr-x   0 niehaus   (1000) niehaus   (1000)        0 2021-06-24 07:01:59.369518 pyserialsensors-0.9.9/pyserialsensors/examples/
+-rw-r--r--   0 niehaus   (1000) niehaus   (1000)       94 2021-05-11 20:46:23.000000 pyserialsensors-0.9.9/pyserialsensors/examples/__init__.py
+-rwxrwxr-x   0 niehaus   (1000) niehaus   (1000)     2841 2021-06-23 21:45:06.000000 pyserialsensors-0.9.9/pyserialsensors/examples/example_mean.py
+-rwxrwxr-x   0 niehaus   (1000) niehaus   (1000)     4600 2021-06-23 22:07:47.000000 pyserialsensors-0.9.9/pyserialsensors/examples/example_single_read.py
+-rw-r--r--   0 niehaus   (1000) niehaus   (1000)      669 2021-05-11 20:46:23.000000 pyserialsensors-0.9.9/pyserialsensors/examples/example_uart.py
+drwxrwxr-x   0 niehaus   (1000) niehaus   (1000)        0 2021-06-24 07:01:59.369518 pyserialsensors-0.9.9/pyserialsensors/tests/
+-rw-r--r--   0 niehaus   (1000) niehaus   (1000)       94 2021-05-11 20:46:23.000000 pyserialsensors-0.9.9/pyserialsensors/tests/__init__.py
+-rw-r--r--   0 niehaus   (1000) niehaus   (1000)      378 2021-05-11 20:46:23.000000 pyserialsensors-0.9.9/pyserialsensors/tests/test_comPort.py
+-rw-r--r--   0 niehaus   (1000) niehaus   (1000)     4620 2021-05-11 20:46:23.000000 pyserialsensors-0.9.9/pyserialsensors/tests/test_sensor_s8000.py
+-rw-r--r--   0 niehaus   (1000) niehaus   (1000)     1922 2021-05-11 20:46:23.000000 pyserialsensors-0.9.9/pyserialsensors/tests/test_sensor_smgair.py
+drwxrwxr-x   0 niehaus   (1000) niehaus   (1000)        0 2021-06-24 07:01:59.369518 pyserialsensors-0.9.9/pyserialsensors/tools/
+-rw-r--r--   0 niehaus   (1000) niehaus   (1000)        0 2021-05-11 20:46:23.000000 pyserialsensors-0.9.9/pyserialsensors/tools/__init__.py
+-rw-r--r--   0 niehaus   (1000) niehaus   (1000)     2079 2021-05-11 20:46:23.000000 pyserialsensors-0.9.9/pyserialsensors/tools/bulk.py
+drwxrwxr-x   0 niehaus   (1000) niehaus   (1000)        0 2021-06-24 07:01:59.369518 pyserialsensors-0.9.9/pyserialsensors.egg-info/
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      926 2021-06-24 07:01:59.000000 pyserialsensors-0.9.9/pyserialsensors.egg-info/PKG-INFO
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)     2199 2021-06-24 07:01:59.000000 pyserialsensors-0.9.9/pyserialsensors.egg-info/SOURCES.txt
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)        1 2021-06-24 07:01:59.000000 pyserialsensors-0.9.9/pyserialsensors.egg-info/dependency_links.txt
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)       77 2021-06-24 07:01:59.000000 pyserialsensors-0.9.9/pyserialsensors.egg-info/requires.txt
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)       16 2021-06-24 07:01:59.000000 pyserialsensors-0.9.9/pyserialsensors.egg-info/top_level.txt
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      455 2021-06-24 07:01:59.369518 pyserialsensors-0.9.9/setup.cfg
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)     1428 2021-06-24 07:01:47.000000 pyserialsensors-0.9.9/setup.py
```

### Comparing `pyserialsensors-0.9.8/CONTRIBUTING.rst` & `pyserialsensors-0.9.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pyserialsensors-0.9.8/LICENSE` & `pyserialsensors-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyserialsensors-0.9.8/PKG-INFO` & `pyserialsensors-0.9.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyserialsensors
-Version: 0.9.8
+Version: 0.9.9
 Summary: German Aerospace Center
 Home-page: https://gitlab.com/Egenskaber/pyserialsensors
 Author: German Aerospace Center
 Author-email: konstantin+pypi@niehaus-web.com
 License: MIT
 Description: Python interface for a FT232H measurement suite based on I2C, SPI and UART sensors.
```

### Comparing `pyserialsensors-0.9.8/README.rst` & `pyserialsensors-0.9.9/README.rst`

 * *Files identical despite different names*

### Comparing `pyserialsensors-0.9.8/docs/Makefile` & `pyserialsensors-0.9.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyserialsensors-0.9.8/docs/conf.py` & `pyserialsensors-0.9.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyserialsensors-0.9.8/docs/defs.rst` & `pyserialsensors-0.9.9/docs/defs.rst`

 * *Files identical despite different names*

### Comparing `pyserialsensors-0.9.8/docs/installation.rst` & `pyserialsensors-0.9.9/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `pyserialsensors-0.9.8/docs/make.bat` & `pyserialsensors-0.9.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyserialsensors-0.9.8/docs/pyserialsensors.core.rst` & `pyserialsensors-0.9.9/docs/pyserialsensors.core.rst`

 * *Files identical despite different names*

### Comparing `pyserialsensors-0.9.8/docs/pyserialsensors.devices.rst` & `pyserialsensors-0.9.9/docs/pyserialsensors.devices.rst`

 * *Files identical despite different names*

### Comparing `pyserialsensors-0.9.8/docs/pyserialsensors.devices.sdp.rst` & `pyserialsensors-0.9.9/docs/pyserialsensors.devices.sdp.rst`

 * *Files identical despite different names*

### Comparing `pyserialsensors-0.9.8/docs/pyserialsensors.examples.rst` & `pyserialsensors-0.9.9/docs/pyserialsensors.examples.rst`

 * *Files identical despite different names*

### Comparing `pyserialsensors-0.9.8/pyserialsensors/core/comPortController.py` & `pyserialsensors-0.9.9/pyserialsensors/core/comPortController.py`

 * *Files identical despite different names*

### Comparing `pyserialsensors-0.9.8/pyserialsensors/core/error.py` & `pyserialsensors-0.9.9/pyserialsensors/core/error.py`

 * *Files identical despite different names*

### Comparing `pyserialsensors-0.9.8/pyserialsensors/core/i2controller.py` & `pyserialsensors-0.9.9/pyserialsensors/core/i2controller.py`

 * *Files identical despite different names*

### Comparing `pyserialsensors-0.9.8/pyserialsensors/core/i2cscan.py` & `pyserialsensors-0.9.9/pyserialsensors/core/i2cscan.py`

 * *Files identical despite different names*

### Comparing `pyserialsensors-0.9.8/pyserialsensors/core/sensor.py` & `pyserialsensors-0.9.9/pyserialsensors/core/sensor.py`

 * *Files identical despite different names*

### Comparing `pyserialsensors-0.9.8/pyserialsensors/core/toolbox.py` & `pyserialsensors-0.9.9/pyserialsensors/core/toolbox.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     SDP8XX,
     QwiicQuadRelay,
 ]
 
 UART_SENSOR_CLASSES = [SPS30, SMGair2, S8000]
 
 
-def scan_spi(spibus, loglvl: int = logging.ERROR, measurement_obj=None):
+def scan_spi(spibus, loglvl: int = logging.ERROR, **kwargs):
     if type(spibus) is SpiController:
         spibus = [spibus]
     elif type(spibus) is not list:
         raise TypeError(
             f"spibus in scan_spi is of type {type(spibus)} but only list \
                   and pyftdi.spi.SpiController are supported"
         )
```

### Comparing `pyserialsensors-0.9.8/pyserialsensors/devices/FTDI.py` & `pyserialsensors-0.9.9/pyserialsensors/devices/FTDI.py`

 * *Files identical despite different names*

### Comparing `pyserialsensors-0.9.8/pyserialsensors/devices/MUX.py` & `pyserialsensors-0.9.9/pyserialsensors/devices/MUX.py`

 * *Files identical despite different names*

### Comparing `pyserialsensors-0.9.8/pyserialsensors/devices/ads1015.py` & `pyserialsensors-0.9.9/pyserialsensors/devices/ads1015.py`

 * *Files identical despite different names*

### Comparing `pyserialsensors-0.9.8/pyserialsensors/devices/bme280.py` & `pyserialsensors-0.9.9/pyserialsensors/devices/bme280.py`

 * *Files identical despite different names*

### Comparing `pyserialsensors-0.9.8/pyserialsensors/devices/max31865.py` & `pyserialsensors-0.9.9/pyserialsensors/devices/max31865.py`

 * *Files identical despite different names*

### Comparing `pyserialsensors-0.9.8/pyserialsensors/devices/nau7802/nau7802.py` & `pyserialsensors-0.9.9/pyserialsensors/devices/nau7802/nau7802.py`

 * *Files identical despite different names*

### Comparing `pyserialsensors-0.9.8/pyserialsensors/devices/qwiicrelay.py` & `pyserialsensors-0.9.9/pyserialsensors/devices/qwiicrelay.py`

 * *Files identical despite different names*

### Comparing `pyserialsensors-0.9.8/pyserialsensors/devices/s8000.py` & `pyserialsensors-0.9.9/pyserialsensors/devices/s8000.py`

 * *Files identical despite different names*

### Comparing `pyserialsensors-0.9.8/pyserialsensors/devices/scd30.py` & `pyserialsensors-0.9.9/pyserialsensors/devices/scd30.py`

 * *Files identical despite different names*

### Comparing `pyserialsensors-0.9.8/pyserialsensors/devices/sdp/sdp8xx.py` & `pyserialsensors-0.9.9/pyserialsensors/devices/sdp/sdp8xx.py`

 * *Files identical despite different names*

### Comparing `pyserialsensors-0.9.8/pyserialsensors/devices/sfm3xxx.py` & `pyserialsensors-0.9.9/pyserialsensors/devices/sfm3xxx.py`

 * *Files identical despite different names*

### Comparing `pyserialsensors-0.9.8/pyserialsensors/devices/shtxx.py` & `pyserialsensors-0.9.9/pyserialsensors/devices/shtxx.py`

 * *Files identical despite different names*

### Comparing `pyserialsensors-0.9.8/pyserialsensors/devices/smgair2.py` & `pyserialsensors-0.9.9/pyserialsensors/devices/smgair2.py`

 * *Files identical despite different names*

### Comparing `pyserialsensors-0.9.8/pyserialsensors/devices/sps30.py` & `pyserialsensors-0.9.9/pyserialsensors/devices/sps30.py`

 * *Files identical despite different names*

### Comparing `pyserialsensors-0.9.8/pyserialsensors/examples/example_mean.py` & `pyserialsensors-0.9.9/pyserialsensors/examples/example_mean.py`

 * *Files identical despite different names*

### Comparing `pyserialsensors-0.9.8/pyserialsensors/examples/example_single_read.py` & `pyserialsensors-0.9.9/pyserialsensors/examples/example_single_read.py`

 * *Files identical despite different names*

### Comparing `pyserialsensors-0.9.8/pyserialsensors/examples/example_uart.py` & `pyserialsensors-0.9.9/pyserialsensors/examples/example_uart.py`

 * *Files identical despite different names*

### Comparing `pyserialsensors-0.9.8/pyserialsensors/tests/test_sensor_s8000.py` & `pyserialsensors-0.9.9/pyserialsensors/tests/test_sensor_s8000.py`

 * *Files identical despite different names*

### Comparing `pyserialsensors-0.9.8/pyserialsensors/tests/test_sensor_smgair.py` & `pyserialsensors-0.9.9/pyserialsensors/tests/test_sensor_smgair.py`

 * *Files identical despite different names*

### Comparing `pyserialsensors-0.9.8/pyserialsensors/tools/bulk.py` & `pyserialsensors-0.9.9/pyserialsensors/tools/bulk.py`

 * *Files identical despite different names*

### Comparing `pyserialsensors-0.9.8/pyserialsensors.egg-info/PKG-INFO` & `pyserialsensors-0.9.9/pyserialsensors.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyserialsensors
-Version: 0.9.8
+Version: 0.9.9
 Summary: German Aerospace Center
 Home-page: https://gitlab.com/Egenskaber/pyserialsensors
 Author: German Aerospace Center
 Author-email: konstantin+pypi@niehaus-web.com
 License: MIT
 Description: Python interface for a FT232H measurement suite based on I2C, SPI and UART sensors.
```

### Comparing `pyserialsensors-0.9.8/pyserialsensors.egg-info/SOURCES.txt` & `pyserialsensors-0.9.9/pyserialsensors.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyserialsensors-0.9.8/setup.py` & `pyserialsensors-0.9.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 # get the log description
 with io.open(path.join(here, "DESCRIPTION.rst"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="pyserialsensors",
-    version="0.9.8",
+    version="0.9.9",
     description="German Aerospace Center",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/Egenskaber/pyserialsensors",
     author="German Aerospace Center",
     author_email="konstantin+pypi@niehaus-web.com",
     install_requires=[
```

