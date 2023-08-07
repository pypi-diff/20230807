# Comparing `tmp/sungrow_http_config-0.0.5.tar.gz` & `tmp/sungrow_http_config-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sungrow_http_config-0.0.5.tar", last modified: Fri Aug  4 09:31:26 2023, max compression
+gzip compressed data, was "sungrow_http_config-0.0.6.tar", last modified: Mon Aug  7 10:03:56 2023, max compression
```

## Comparing `sungrow_http_config-0.0.5.tar` & `sungrow_http_config-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-08-04 09:31:26.690481 sungrow_http_config-0.0.5/
--rw-r--r--   0 ross       (501) staff       (20)     1072 2023-08-01 09:53:21.000000 sungrow_http_config-0.0.5/LICENSE
--rw-r--r--   0 ross       (501) staff       (20)     1760 2023-08-04 09:31:26.690020 sungrow_http_config-0.0.5/PKG-INFO
--rw-r--r--   0 ross       (501) staff       (20)     1202 2023-08-03 12:35:38.000000 sungrow_http_config-0.0.5/README.md
--rw-r--r--   0 ross       (501) staff       (20)      711 2023-08-04 09:31:03.000000 sungrow_http_config-0.0.5/pyproject.toml
--rw-r--r--   0 ross       (501) staff       (20)       38 2023-08-04 09:31:26.690618 sungrow_http_config-0.0.5/setup.cfg
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-08-04 09:31:26.683187 sungrow_http_config-0.0.5/src/
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-08-04 09:31:26.685999 sungrow_http_config-0.0.5/src/sungrow_http_config/
--rw-r--r--   0 ross       (501) staff       (20)    10146 2023-08-04 09:30:47.000000 sungrow_http_config-0.0.5/src/sungrow_http_config/SungrowHttpConfig.py
--rw-r--r--   0 ross       (501) staff       (20)        1 2023-08-01 09:55:24.000000 sungrow_http_config-0.0.5/src/sungrow_http_config/__init__.py
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-08-04 09:31:26.689244 sungrow_http_config-0.0.5/src/sungrow_http_config.egg-info/
--rw-r--r--   0 ross       (501) staff       (20)     1760 2023-08-04 09:31:26.000000 sungrow_http_config-0.0.5/src/sungrow_http_config.egg-info/PKG-INFO
--rw-r--r--   0 ross       (501) staff       (20)      347 2023-08-04 09:31:26.000000 sungrow_http_config-0.0.5/src/sungrow_http_config.egg-info/SOURCES.txt
--rw-r--r--   0 ross       (501) staff       (20)        1 2023-08-04 09:31:26.000000 sungrow_http_config-0.0.5/src/sungrow_http_config.egg-info/dependency_links.txt
--rw-r--r--   0 ross       (501) staff       (20)       46 2023-08-04 09:31:26.000000 sungrow_http_config-0.0.5/src/sungrow_http_config.egg-info/requires.txt
--rw-r--r--   0 ross       (501) staff       (20)       20 2023-08-04 09:31:26.000000 sungrow_http_config-0.0.5/src/sungrow_http_config.egg-info/top_level.txt
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-08-07 10:03:56.147609 sungrow_http_config-0.0.6/
+-rw-r--r--   0 ross       (501) staff       (20)     1072 2023-08-01 09:53:21.000000 sungrow_http_config-0.0.6/LICENSE
+-rw-r--r--   0 ross       (501) staff       (20)     1760 2023-08-07 10:03:56.147178 sungrow_http_config-0.0.6/PKG-INFO
+-rw-r--r--   0 ross       (501) staff       (20)     1202 2023-08-03 12:35:38.000000 sungrow_http_config-0.0.6/README.md
+-rw-r--r--   0 ross       (501) staff       (20)      711 2023-08-07 10:03:12.000000 sungrow_http_config-0.0.6/pyproject.toml
+-rw-r--r--   0 ross       (501) staff       (20)       38 2023-08-07 10:03:56.147745 sungrow_http_config-0.0.6/setup.cfg
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-08-07 10:03:56.142175 sungrow_http_config-0.0.6/src/
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-08-07 10:03:56.144410 sungrow_http_config-0.0.6/src/sungrow_http_config/
+-rw-r--r--   0 ross       (501) staff       (20)    10448 2023-08-07 10:02:49.000000 sungrow_http_config-0.0.6/src/sungrow_http_config/SungrowHttpConfig.py
+-rw-r--r--   0 ross       (501) staff       (20)        1 2023-08-01 09:55:24.000000 sungrow_http_config-0.0.6/src/sungrow_http_config/__init__.py
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-08-07 10:03:56.146650 sungrow_http_config-0.0.6/src/sungrow_http_config.egg-info/
+-rw-r--r--   0 ross       (501) staff       (20)     1760 2023-08-07 10:03:56.000000 sungrow_http_config-0.0.6/src/sungrow_http_config.egg-info/PKG-INFO
+-rw-r--r--   0 ross       (501) staff       (20)      347 2023-08-07 10:03:56.000000 sungrow_http_config-0.0.6/src/sungrow_http_config.egg-info/SOURCES.txt
+-rw-r--r--   0 ross       (501) staff       (20)        1 2023-08-07 10:03:56.000000 sungrow_http_config-0.0.6/src/sungrow_http_config.egg-info/dependency_links.txt
+-rw-r--r--   0 ross       (501) staff       (20)       46 2023-08-07 10:03:56.000000 sungrow_http_config-0.0.6/src/sungrow_http_config.egg-info/requires.txt
+-rw-r--r--   0 ross       (501) staff       (20)       20 2023-08-07 10:03:56.000000 sungrow_http_config-0.0.6/src/sungrow_http_config.egg-info/top_level.txt
```

### Comparing `sungrow_http_config-0.0.5/LICENSE` & `sungrow_http_config-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sungrow_http_config-0.0.5/PKG-INFO` & `sungrow_http_config-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sungrow_http_config
-Version: 0.0.5
+Version: 0.0.6
 Summary: A package to manipulate settings on Sungrow Inverters
 Author-email: Ross Williamson <ross@inertia.net.nz>
 Project-URL: Homepage, https://github.com/ross-w/sungrow_exportlimit
 Project-URL: Bug Tracker, https://github.com/ross-w/sungrow_exportlimit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sungrow_http_config-0.0.5/README.md` & `sungrow_http_config-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `sungrow_http_config-0.0.5/pyproject.toml` & `sungrow_http_config-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sungrow_http_config"
-version = "0.0.5"
+version = "0.0.6"
 dependencies = [
   "requests_retry_on_exceptions",
   "urllib3",
   "pymodbus"
 ]
 authors = [
   { name="Ross Williamson", email="ross@inertia.net.nz" },
```

### Comparing `sungrow_http_config-0.0.5/src/sungrow_http_config/SungrowHttpConfig.py` & `sungrow_http_config-0.0.6/src/sungrow_http_config/SungrowHttpConfig.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,14 +159,23 @@
             "protocol": 0x00,
         }
         message = modbus_register_write.WriteSingleRegisterRequest(**arguments)
         raw_packet = framer.buildPacket(message)
         packet = c.encode(raw_packet, "hex_codec").decode("utf-8").upper()
         return packet
 
+    def getDeviceSerialNumber(self):
+        """ Retrieve the device serial number to uniquely identify it
+        :returns: String containting the serial number of the inverter
+        """
+        if self.productVersion == {}:
+            self.connect()
+
+        return self.productVersion["dev_sn"]
+
     def setExportLimit(self, dekawattLimit):
         """ Enable export limit and set to 0kW (zero export limit)
         :param dekawattLimit: Limit to set, in dekawatts (kW * 100). Note 0 == unlimited, so set 1 for 0.01kW
         :returns: True if successful
         """
 
         msg1 = self._sendHexMessageToDevice("010679F400AA511B") # Turn on feed-in limitation
```

### Comparing `sungrow_http_config-0.0.5/src/sungrow_http_config.egg-info/PKG-INFO` & `sungrow_http_config-0.0.6/src/sungrow_http_config.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sungrow-http-config
-Version: 0.0.5
+Version: 0.0.6
 Summary: A package to manipulate settings on Sungrow Inverters
 Author-email: Ross Williamson <ross@inertia.net.nz>
 Project-URL: Homepage, https://github.com/ross-w/sungrow_exportlimit
 Project-URL: Bug Tracker, https://github.com/ross-w/sungrow_exportlimit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

