# Comparing `tmp/LN2_Monitor-0.0.1.tar.gz` & `tmp/LN2_Monitor-3.11.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LN2_Monitor-0.0.1.tar", last modified: Mon Aug  7 21:23:14 2023, max compression
+gzip compressed data, was "LN2_Monitor-3.11.7.tar", last modified: Mon Jul 24 21:31:29 2023, max compression
```

## Comparing `LN2_Monitor-0.0.1.tar` & `LN2_Monitor-3.11.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-08-07 21:23:14.304565 LN2_Monitor-0.0.1/
-drwxrwxrwx   0        0        0        0 2023-08-07 21:23:14.296435 LN2_Monitor-0.0.1/LN2_Monitor.egg-info/
--rw-rw-rw-   0        0        0     2599 2023-08-07 21:23:14.000000 LN2_Monitor-0.0.1/LN2_Monitor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      423 2023-08-07 21:23:14.000000 LN2_Monitor-0.0.1/LN2_Monitor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-07 21:23:14.000000 LN2_Monitor-0.0.1/LN2_Monitor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-08-07 21:23:14.000000 LN2_Monitor-0.0.1/LN2_Monitor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-08-07 21:23:14.000000 LN2_Monitor-0.0.1/LN2_Monitor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2599 2023-08-07 21:23:14.303566 LN2_Monitor-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2051 2023-07-24 21:35:34.000000 LN2_Monitor-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-08-07 21:23:14.299565 LN2_Monitor-0.0.1/ln2_monitor/
--rw-rw-rw-   0        0        0        0 2023-07-18 20:07:57.000000 LN2_Monitor-0.0.1/ln2_monitor/__init__.py
--rw-rw-rw-   0        0        0     3399 2023-07-18 19:22:36.000000 LN2_Monitor-0.0.1/ln2_monitor/d1.py
--rw-rw-rw-   0        0        0      627 2023-08-07 21:22:29.000000 LN2_Monitor-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-07 21:23:14.305567 LN2_Monitor-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      651 2023-07-24 21:21:38.000000 LN2_Monitor-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 21:31:29.396992 LN2_Monitor-3.11.7/
+drwxrwxrwx   0        0        0        0 2023-07-24 21:31:29.391949 LN2_Monitor-3.11.7/LN2_Monitor.egg-info/
+-rw-rw-rw-   0        0        0     2368 2023-07-24 21:31:29.000000 LN2_Monitor-3.11.7/LN2_Monitor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      423 2023-07-24 21:31:29.000000 LN2_Monitor-3.11.7/LN2_Monitor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 21:31:29.000000 LN2_Monitor-3.11.7/LN2_Monitor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-07-24 21:31:29.000000 LN2_Monitor-3.11.7/LN2_Monitor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-24 21:31:29.000000 LN2_Monitor-3.11.7/LN2_Monitor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2368 2023-07-24 21:31:29.396992 LN2_Monitor-3.11.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1845 2023-07-19 21:47:29.000000 LN2_Monitor-3.11.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-24 21:31:29.395948 LN2_Monitor-3.11.7/ln2_monitor/
+-rw-rw-rw-   0        0        0        0 2023-07-18 20:07:57.000000 LN2_Monitor-3.11.7/ln2_monitor/__init__.py
+-rw-rw-rw-   0        0        0     3399 2023-07-18 19:22:36.000000 LN2_Monitor-3.11.7/ln2_monitor/d1.py
+-rw-rw-rw-   0        0        0      602 2023-07-19 21:49:38.000000 LN2_Monitor-3.11.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-24 21:31:29.396992 LN2_Monitor-3.11.7/setup.cfg
+-rw-rw-rw-   0        0        0      651 2023-07-24 21:21:38.000000 LN2_Monitor-3.11.7/setup.py
```

### Comparing `LN2_Monitor-0.0.1/LN2_Monitor.egg-info/PKG-INFO` & `LN2_Monitor-3.11.7/LN2_Monitor.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: LN2-Monitor
-Version: 0.0.1
-Summary: A Project that helps automate the weighing of LN2
+Version: 3.11.7
+Summary: A small example package
 Home-page: https://github.com/dav17393/LN2_Monitor
 Author: Jordan Wheeler, David Shin
 Author-email: "dav17393, wheeler1711" <wheeler1711@gmail.com>
 Project-URL: Homepage, https://github.com/dav17393/LN2_Monitor
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -17,28 +17,23 @@
 
 **Required Softwares:**
 
 PyUSB 1.0 (https://sourceforge.net/projects/pyusb/files/PyUSB%201.0/)
 
 libusb-win32 (https://sourceforge.net/projects/libusb-win32/)
 
-pip install ln2-monitor
-then go into python and input "from ln2_monitor import d1". 
-input "scale = d1.SCL()"
-
-**How to run the Software:**
-
-After opening up the program, download both softwares and run the libusb-win32 software. In device selection, select the USB input device with product ID 8009(pid:8009). Then pipinstall pyusb, numpy, and matplot. Then run the code by changing the directory whichever folder the d1 file was downloaded to. Then switch powershell to python and import the d1 file. Set scale = d1.SCL() and run scale.main() or scale.plot() to start plotting and transferring the data to a txt file. You can also run scale.getkg() or scale.getdata() to get the kg or the array respectively. The basic minimum and maximum weights(kg) are set to default as the blucifer cryostat. Scale.setweight() can be run to change the minumum and maximum weight of the cryostat.
-
-To turn off "auto-sleep" mode on the scale, hold the kg/lb button and turn the scale on. 
-
 **The array that is returned when calling the scale.main(), scale.plot(), or scale.getdata() functions can be translated as shown below:**
 array('B'[3, 2, 11, 255, 0, 0])
 
 The first element is always 3 and negatable.
 The second element is also negatable.
 The third element will only return either 2 or 11, with 2 meaning the scale is in kg mode and 11 meaning the scale is in lbs/oz mode.
 The fourth element is the scale factor. A value of 255 means the scaling factor is 10^-1(0.1), a value of 254 means a scaling factor of 10^-2(0.01), and so on. 
 The fourth and fifth elements together are used to determine the weight.
 The sixth element is also negatable. 
 
+
+**How to run the Software:**
+
+After opening up the program, download both softwares and run the libusb-win32 software. In device selection, select the USB input device with product ID 8009(pid:8009). Then pipinstall pyusb, numpy, and matplot. Then run the code by changing the directory whichever folder the d1 file was downloaded to. Then switch powershell to python and import the d1 file. Set scale = d1.SCL() and run scale.main() or scale.plot() to start plotting and transferring the data to a txt file. You can also run scale.getkg() or scale.getdata() to get the kg or the array respectively. The basic minimum and maximum weights(kg) are set to default as the blucifer cryostat. Scale.setweight() can be run to change the minumum and maximum weight of the cryostat.
+
 Enjoy!
```

### Comparing `LN2_Monitor-0.0.1/PKG-INFO` & `LN2_Monitor-3.11.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: LN2_Monitor
-Version: 0.0.1
-Summary: A Project that helps automate the weighing of LN2
+Version: 3.11.7
+Summary: A small example package
 Home-page: https://github.com/dav17393/LN2_Monitor
 Author: Jordan Wheeler, David Shin
 Author-email: "dav17393, wheeler1711" <wheeler1711@gmail.com>
 Project-URL: Homepage, https://github.com/dav17393/LN2_Monitor
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -17,28 +17,23 @@
 
 **Required Softwares:**
 
 PyUSB 1.0 (https://sourceforge.net/projects/pyusb/files/PyUSB%201.0/)
 
 libusb-win32 (https://sourceforge.net/projects/libusb-win32/)
 
-pip install ln2-monitor
-then go into python and input "from ln2_monitor import d1". 
-input "scale = d1.SCL()"
-
-**How to run the Software:**
-
-After opening up the program, download both softwares and run the libusb-win32 software. In device selection, select the USB input device with product ID 8009(pid:8009). Then pipinstall pyusb, numpy, and matplot. Then run the code by changing the directory whichever folder the d1 file was downloaded to. Then switch powershell to python and import the d1 file. Set scale = d1.SCL() and run scale.main() or scale.plot() to start plotting and transferring the data to a txt file. You can also run scale.getkg() or scale.getdata() to get the kg or the array respectively. The basic minimum and maximum weights(kg) are set to default as the blucifer cryostat. Scale.setweight() can be run to change the minumum and maximum weight of the cryostat.
-
-To turn off "auto-sleep" mode on the scale, hold the kg/lb button and turn the scale on. 
-
 **The array that is returned when calling the scale.main(), scale.plot(), or scale.getdata() functions can be translated as shown below:**
 array('B'[3, 2, 11, 255, 0, 0])
 
 The first element is always 3 and negatable.
 The second element is also negatable.
 The third element will only return either 2 or 11, with 2 meaning the scale is in kg mode and 11 meaning the scale is in lbs/oz mode.
 The fourth element is the scale factor. A value of 255 means the scaling factor is 10^-1(0.1), a value of 254 means a scaling factor of 10^-2(0.01), and so on. 
 The fourth and fifth elements together are used to determine the weight.
 The sixth element is also negatable. 
 
+
+**How to run the Software:**
+
+After opening up the program, download both softwares and run the libusb-win32 software. In device selection, select the USB input device with product ID 8009(pid:8009). Then pipinstall pyusb, numpy, and matplot. Then run the code by changing the directory whichever folder the d1 file was downloaded to. Then switch powershell to python and import the d1 file. Set scale = d1.SCL() and run scale.main() or scale.plot() to start plotting and transferring the data to a txt file. You can also run scale.getkg() or scale.getdata() to get the kg or the array respectively. The basic minimum and maximum weights(kg) are set to default as the blucifer cryostat. Scale.setweight() can be run to change the minumum and maximum weight of the cryostat.
+
 Enjoy!
```

### Comparing `LN2_Monitor-0.0.1/README.md` & `LN2_Monitor-3.11.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -3,28 +3,23 @@
 
 **Required Softwares:**
 
 PyUSB 1.0 (https://sourceforge.net/projects/pyusb/files/PyUSB%201.0/)
 
 libusb-win32 (https://sourceforge.net/projects/libusb-win32/)
 
-pip install ln2-monitor
-then go into python and input "from ln2_monitor import d1". 
-input "scale = d1.SCL()"
-
-**How to run the Software:**
-
-After opening up the program, download both softwares and run the libusb-win32 software. In device selection, select the USB input device with product ID 8009(pid:8009). Then pipinstall pyusb, numpy, and matplot. Then run the code by changing the directory whichever folder the d1 file was downloaded to. Then switch powershell to python and import the d1 file. Set scale = d1.SCL() and run scale.main() or scale.plot() to start plotting and transferring the data to a txt file. You can also run scale.getkg() or scale.getdata() to get the kg or the array respectively. The basic minimum and maximum weights(kg) are set to default as the blucifer cryostat. Scale.setweight() can be run to change the minumum and maximum weight of the cryostat.
-
-To turn off "auto-sleep" mode on the scale, hold the kg/lb button and turn the scale on. 
-
 **The array that is returned when calling the scale.main(), scale.plot(), or scale.getdata() functions can be translated as shown below:**
 array('B'[3, 2, 11, 255, 0, 0])
 
 The first element is always 3 and negatable.
 The second element is also negatable.
 The third element will only return either 2 or 11, with 2 meaning the scale is in kg mode and 11 meaning the scale is in lbs/oz mode.
 The fourth element is the scale factor. A value of 255 means the scaling factor is 10^-1(0.1), a value of 254 means a scaling factor of 10^-2(0.01), and so on. 
 The fourth and fifth elements together are used to determine the weight.
 The sixth element is also negatable. 
 
+
+**How to run the Software:**
+
+After opening up the program, download both softwares and run the libusb-win32 software. In device selection, select the USB input device with product ID 8009(pid:8009). Then pipinstall pyusb, numpy, and matplot. Then run the code by changing the directory whichever folder the d1 file was downloaded to. Then switch powershell to python and import the d1 file. Set scale = d1.SCL() and run scale.main() or scale.plot() to start plotting and transferring the data to a txt file. You can also run scale.getkg() or scale.getdata() to get the kg or the array respectively. The basic minimum and maximum weights(kg) are set to default as the blucifer cryostat. Scale.setweight() can be run to change the minumum and maximum weight of the cryostat.
+
 Enjoy!
```

### Comparing `LN2_Monitor-0.0.1/ln2_monitor/d1.py` & `LN2_Monitor-3.11.7/ln2_monitor/d1.py`

 * *Files identical despite different names*

### Comparing `LN2_Monitor-0.0.1/pyproject.toml` & `LN2_Monitor-3.11.7/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 
 [project]
 name = "LN2_Monitor"
-version = "0.0.1"
+version = "3.11.7"
 authors = [
   { name="dav17393, wheeler1711", email="wheeler1711@gmail.com" },
 ]
-description = "A Project that helps automate the weighing of LN2"
+description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `LN2_Monitor-0.0.1/setup.py` & `LN2_Monitor-3.11.7/setup.py`

 * *Files identical despite different names*

