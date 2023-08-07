# Comparing `tmp/IOmatchbox-0.22.tar.gz` & `tmp/IOmatchbox-0.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IOmatchbox-0.22.tar", last modified: Mon Aug  7 06:41:50 2023, max compression
+gzip compressed data, was "IOmatchbox-0.23.tar", last modified: Mon Aug  7 12:37:29 2023, max compression
```

## Comparing `IOmatchbox-0.22.tar` & `IOmatchbox-0.23.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 yfo       (1000) yfo       (1000)        0 2023-08-07 06:41:50.548720 IOmatchbox-0.22/
--rw-r--r--   0 yfo       (1000) yfo       (1000)     1064 2023-05-22 13:50:06.000000 IOmatchbox-0.22/LICENSE
--rw-r--r--   0 yfo       (1000) yfo       (1000)     4102 2023-08-07 06:41:50.548720 IOmatchbox-0.22/PKG-INFO
--rw-r--r--   0 yfo       (1000) yfo       (1000)     3195 2023-08-04 14:14:48.000000 IOmatchbox-0.22/README.md
--rw-r--r--   0 yfo       (1000) yfo       (1000)      951 2023-08-07 06:41:21.000000 IOmatchbox-0.22/pyproject.toml
--rw-r--r--   0 yfo       (1000) yfo       (1000)       38 2023-08-07 06:41:50.548720 IOmatchbox-0.22/setup.cfg
-drwxr-xr-x   0 yfo       (1000) yfo       (1000)        0 2023-08-07 06:41:50.546720 IOmatchbox-0.22/src/
-drwxr-xr-x   0 yfo       (1000) yfo       (1000)        0 2023-08-07 06:41:50.547720 IOmatchbox-0.22/src/IOmatchbox/
--rw-r--r--   0 yfo       (1000) yfo       (1000)    15547 2023-08-07 06:40:56.000000 IOmatchbox-0.22/src/IOmatchbox/IOTEC.py
--rw-r--r--   0 yfo       (1000) yfo       (1000)    23987 2023-08-07 06:38:56.000000 IOmatchbox-0.22/src/IOmatchbox/IOmatchbox.py
--rw-r--r--   0 yfo       (1000) yfo       (1000)        0 2023-08-04 09:16:46.000000 IOmatchbox-0.22/src/IOmatchbox/__init__.py
-drwxr-xr-x   0 yfo       (1000) yfo       (1000)        0 2023-08-07 06:41:50.547720 IOmatchbox-0.22/src/IOmatchbox.egg-info/
--rw-r--r--   0 yfo       (1000) yfo       (1000)     4102 2023-08-07 06:41:50.000000 IOmatchbox-0.22/src/IOmatchbox.egg-info/PKG-INFO
--rw-r--r--   0 yfo       (1000) yfo       (1000)      264 2023-08-07 06:41:50.000000 IOmatchbox-0.22/src/IOmatchbox.egg-info/SOURCES.txt
--rw-r--r--   0 yfo       (1000) yfo       (1000)        1 2023-08-07 06:41:50.000000 IOmatchbox-0.22/src/IOmatchbox.egg-info/dependency_links.txt
--rw-r--r--   0 yfo       (1000) yfo       (1000)       11 2023-08-07 06:41:50.000000 IOmatchbox-0.22/src/IOmatchbox.egg-info/top_level.txt
+drwxr-xr-x   0 yfo       (1000) yfo       (1000)        0 2023-08-07 12:37:29.563111 IOmatchbox-0.23/
+-rw-r--r--   0 yfo       (1000) yfo       (1000)     1064 2023-05-22 13:50:06.000000 IOmatchbox-0.23/LICENSE
+-rw-r--r--   0 yfo       (1000) yfo       (1000)     3763 2023-08-07 12:37:29.563111 IOmatchbox-0.23/PKG-INFO
+-rw-r--r--   0 yfo       (1000) yfo       (1000)     2856 2023-08-07 12:23:00.000000 IOmatchbox-0.23/README.md
+-rw-r--r--   0 yfo       (1000) yfo       (1000)      951 2023-08-07 12:22:41.000000 IOmatchbox-0.23/pyproject.toml
+-rw-r--r--   0 yfo       (1000) yfo       (1000)       38 2023-08-07 12:37:29.563111 IOmatchbox-0.23/setup.cfg
+drwxr-xr-x   0 yfo       (1000) yfo       (1000)        0 2023-08-07 12:37:29.561111 IOmatchbox-0.23/src/
+drwxr-xr-x   0 yfo       (1000) yfo       (1000)        0 2023-08-07 12:37:29.562111 IOmatchbox-0.23/src/IOmatchbox/
+-rw-r--r--   0 yfo       (1000) yfo       (1000)    16151 2023-08-07 12:35:26.000000 IOmatchbox-0.23/src/IOmatchbox/IOTEC.py
+-rw-r--r--   0 yfo       (1000) yfo       (1000)    24317 2023-08-07 12:33:43.000000 IOmatchbox-0.23/src/IOmatchbox/IOmatchbox.py
+-rw-r--r--   0 yfo       (1000) yfo       (1000)      277 2023-08-07 12:16:39.000000 IOmatchbox-0.23/src/IOmatchbox/__init__.py
+drwxr-xr-x   0 yfo       (1000) yfo       (1000)        0 2023-08-07 12:37:29.562111 IOmatchbox-0.23/src/IOmatchbox.egg-info/
+-rw-r--r--   0 yfo       (1000) yfo       (1000)     3763 2023-08-07 12:37:29.000000 IOmatchbox-0.23/src/IOmatchbox.egg-info/PKG-INFO
+-rw-r--r--   0 yfo       (1000) yfo       (1000)      264 2023-08-07 12:37:29.000000 IOmatchbox-0.23/src/IOmatchbox.egg-info/SOURCES.txt
+-rw-r--r--   0 yfo       (1000) yfo       (1000)        1 2023-08-07 12:37:29.000000 IOmatchbox-0.23/src/IOmatchbox.egg-info/dependency_links.txt
+-rw-r--r--   0 yfo       (1000) yfo       (1000)       11 2023-08-07 12:37:29.000000 IOmatchbox-0.23/src/IOmatchbox.egg-info/top_level.txt
```

### Comparing `IOmatchbox-0.22/LICENSE` & `IOmatchbox-0.23/LICENSE`

 * *Files identical despite different names*

### Comparing `IOmatchbox-0.22/PKG-INFO` & `IOmatchbox-0.23/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IOmatchbox
-Version: 0.22
+Version: 0.23
 Summary: Functions and examples to control Integrated Optics CW lasers and standalone TECs through serial commands with Python
 Author-email: iancynk <ian.cynk@posteo.eu>
 Project-URL: Homepage, https://github.com/iancynk/IOmatchbox
 Project-URL: Bug Tracker, https://github.com/iancynk/IOmatchbox/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
@@ -30,39 +30,26 @@
 ## Requirements
 Needs `serial` and `pyserial` (both of them are needed for this to work somehow), best installed through:
 ```
 pip install serial pyserial
 ```
 
 ## Usage
-### Pip
 Simply run
 ```
 pip install IOmatchbox
 ```
 Then in your Python script invoke the functions by
 ```
-from IOmatchbox.IOmatchbox import IOM
-from IOmatchbox.IOTEC import IOT
+from IOmatchbox import IOM, IOT
 iom = IOM()
 iot = IOT()
 ```
 With `iom` you can then call all functions and methods of the laser, with `iot` you can communicate with the external TEC.
 
-### Download only file
-Download [IOmatchbox.py](src/IOmatchbox/IOmatchbox.py) and [IOTEC.py](src/IOmatchox/IOTEC.py) and put them in your working directory. 
-
-Then in your Python script invoke the functions by
-```
-from IOmatchbox import IOM
-from IOTEC import IOT
-iom = IOM()
-iot = IOT()
-```
-
 Get some more info with
 ```
 iom.get_settings()
 iom.get_readings()
 iom.laser_status()
 ```
```

### Comparing `IOmatchbox-0.22/README.md` & `IOmatchbox-0.23/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -10,39 +10,26 @@
 ## Requirements
 Needs `serial` and `pyserial` (both of them are needed for this to work somehow), best installed through:
 ```
 pip install serial pyserial
 ```
 
 ## Usage
-### Pip
 Simply run
 ```
 pip install IOmatchbox
 ```
 Then in your Python script invoke the functions by
 ```
-from IOmatchbox.IOmatchbox import IOM
-from IOmatchbox.IOTEC import IOT
+from IOmatchbox import IOM, IOT
 iom = IOM()
 iot = IOT()
 ```
 With `iom` you can then call all functions and methods of the laser, with `iot` you can communicate with the external TEC.
 
-### Download only file
-Download [IOmatchbox.py](src/IOmatchbox/IOmatchbox.py) and [IOTEC.py](src/IOmatchox/IOTEC.py) and put them in your working directory. 
-
-Then in your Python script invoke the functions by
-```
-from IOmatchbox import IOM
-from IOTEC import IOT
-iom = IOM()
-iot = IOT()
-```
-
 Get some more info with
 ```
 iom.get_settings()
 iom.get_readings()
 iom.laser_status()
 ```
```

### Comparing `IOmatchbox-0.22/src/IOmatchbox/IOTEC.py` & `IOmatchbox-0.23/src/IOmatchbox/IOTEC.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         and check whether the connected device has an ID like an IO laser. 
         """
         self.ser = serial.Serial()
         self.ser.baudrate = 115200
         self.ser.bytesize = serial.EIGHTBITS
         self.ser.parity = serial.PARITY_NONE
         self.ser.stopbits = serial.STOPBITS_ONE
-        self.ser.timeout = 5
+        self.ser.timeout = 2
         # self.ser.rtscts = True # enable hardware (TRS/CTS) flow control
         if not port:
             # find available ports depending on operating system
             if sys.platform.startswith('linux') or sys.platform.startswith('cygwin'):
                 available_ports = glob.glob('/dev/ttyUSB*')
             elif sys.platform.startswith('win'):
                 available_ports = ['COM%s' % (i + 1) for i in range(256)]
@@ -98,35 +98,51 @@
             # check if the selected port has an IO TEC by querying info
             _ = self.ser.write("r i".encode())
 
             # check if the info contains "ExternalTEC"
             try:
                 # output comes in five lines, combine it to one string
                 reply = ''
+                self.ser.timeout = 0.5  # reduce timeout to not block channel too long
                 for i in range(5):
                     reply += self.ser.readline().decode('utf-8', 'ignore').strip() + '  '
                 if reply[0:11] == "ExternalTEC":
                     print('connected to', reply[0:11])
-                break
+                    self.ser.timeout = 2
+                else:
+                    self.ser.close()
             except:
                 self.ser.close()
                 time.sleep(0.1)
                 print('not a IO TEC')
                 pass
-
-        # check if connection is open
-        if not self.ser.is_open:
-            print('opening serial port failed')
-            self.ser = None
+        
+        if self.DEBUG:
+            if self.ser.is_open:
+                print('port', self.ser.port, 'opened')
         return
     
     
+    def port_is_open(self):
+        """check whether serial port is open
+        returns false if port is closed or not a serial port
+        """
+        try: 
+            if not self.ser.is_open:
+                print('serial port not open')
+                return False
+        except AttributeError:
+            print('no serial stage connected, ignoring command')
+            return False
+        return True
+    
+    
     def closeTEC(self):
         """close serial connection"""
-        if not self.ser.is_open: print('no serial connection'); return
+        if not self.port_is_open(): return
         self.ser.close()
         if not self.ser.is_open:
             print('connection closed')
     
     # --------------------------------------------------------------------------
     # possible commands (from MB IO user manual)
     
@@ -148,52 +164,52 @@
     # --------------------------------------------------------------------------
     # read out settings with commands
     
     def get_settings(self, output=False):
         """receive TEC settings
         if output=True, will spill the whole string with info, otherwise only returns it
         """
-        _ = self.ser.write(cmds["get_settings"].encode())
+        _ = self.ser.write(self.cmds["get_settings"].encode())
         reply = self.ser.readline().decode('utf-8').strip()
         if output:
             print('Settings: min temp?, max temp?, 0, 255, nan, \
                 64000, autostart mode, access level, set temp')
             print(reply)
             return
         else:
             return reply
     
     
     def get_readings(self, output=False):
         """receive TEC readings
         if output=True, will spill the whole string with info, otherwise only returns it
         """
-        _ = self.ser.write(cmds["get_readings"].encode())
+        _ = self.ser.write(self.cmds["get_readings"].encode())
         reply = self.ser.readline().decode('utf-8').strip()
         if output:
             print('Readings: some temperature, some temperature, TEC temperature, current, \
                 some load, some load, system status, some load, input voltage')
             print(reply)
             return
         else:
             return reply
     
     
     def get_om(self):
         """receive operation mode (APC/ACC)"""
-        _ = self.ser.write(cmds["get_om"].encode())
+        _ = self.ser.write(self.cmds["get_om"].encode())
         reply = self.ser.readline().decode('utf-8').strip()
         print('operation mode:', reply)
     
     
     def get_info(self, output=False):
         """receive TEC information
         if output=True, will spill the whole string with info, otherwise only returns it
         """
-        _ = self.ser.write(cmds["get_info"].encode())
+        _ = self.ser.write(self.cmds["get_info"].encode())
         # output comes in five lines, combine it to one list
         reply = ''
         for i in range(5):
             reply += self.ser.readline().decode('utf-8', 'ignore').strip() + '  '
         
         if output:
             print('Driver Version, serial number, product code, operating time, switch times')
@@ -203,30 +219,30 @@
             return reply
     
     
     def get_optime(self, output=False):
         """receive laser operation time
         if output=True, will spill the whole string with info, otherwise only returns it
         """
-        _ = self.ser.write(cmds["get_optime"].encode())
+        _ = self.ser.write(self.cmds["get_optime"].encode())
         # output comes in two lines, combine it to one list
         reply1 = self.ser.readline().decode('utf-8').strip()[:-1]  # remove trailing dot
         reply2 = self.ser.readline().decode('utf-8').strip()
         reply = reply1 + ', ' + reply2
         if output:
             print('operating hours and how many times the laser diode has been turned on')
             print(reply)
             return
         else:
             return reply
     
     
     def get_access_level(self):
         """receive access level"""
-        _ = self.ser.write(cmds["get_access_level"].encode())
+        _ = self.ser.write(self.cmds["get_access_level"].encode())
         reply = self.ser.readline().decode('utf-8').strip()
         access_level = int(reply.split()[2])
         return access_level
     
     
     def set_access_level(self, level):
         """change user access level (default level over serial is 0)
@@ -244,15 +260,15 @@
                 code = int(input_code)
             except ValueError:
                 print('please input a 5 digit number as access level code')
                 return
         else:
             print('invalid access level, please choose a number in [0..3]')
             return
-    
+        
         cmd = cmds["set_access_level"]+' ' + str(level) + ' ' + input_code
         _ = self.ser.write(cmd.encode())
         reply = self.ser.readline().decode('utf-8').strip()
         # check if access level code worked
         if reply == '<ERR 4>':
             print('invalid code to unlock access level', str(level), ': ', input_code)
         else:
@@ -265,70 +281,70 @@
         """set TEC temp (should be in centi-degC, eg 2550)"""
         if self.get_access_level() < 1:
             print('not enough privilege, please update access level to 1 first')
             return
         
         old_settemp = self.get_TEC_set_temp()
         if (settemp > 2000) & (settemp < 3000):
-            _ = self.ser.write((cmds["set_TEC_temp"]+ ' ' + str(settemp)).encode())
+            _ = self.ser.write((self.cmds["set_TEC_temp"]+ ' ' + str(settemp)).encode())
             reply = self.ser.readline().decode('utf-8').strip()
             self.check_reply(reply)
             new_settemp = self.get_TEC_set_temp()
         else:
             print('please give a reasonable input temperature (2000-3000) as integer')
     
     
     def enable_autostart(self):
         """enable autostart on power-on"""
         if self.get_access_level() < 1:
             print('not enough privilege, please update access level to 1 first')
             return
         
-        # errorcode = self.ser.write((cmds["enable_autostart"] + ' 1').encode())
+        # errorcode = self.ser.write((self.cmds["enable_autostart"] + ' 1').encode())
         # reply = self.ser.readline().decode('utf-8').strip()
         # self.check_reply(reply)
         print("Do not use Autostart! It will just heat your base plate without any regulation.")
         print("You're welcome. Glad I could save your laser.")
     
     
     def disable_autostart(self):
         """disable autostart on power-on"""
         if self.get_access_level() < 1:
             print('not enough privilege, please update access level to 1 first')
             return
-    
-        errorcode = self.ser.write((cmds["enable_autostart"] + ' 0').encode())
+        
+        errorcode = self.ser.write((self.cmds["enable_autostart"] + ' 0').encode())
         reply = self.ser.readline().decode('utf-8').strip()
         self.check_reply(reply)
     
     
     def save_changes(self):
         """save changes"""
         if self.get_access_level() < 1:
             print('not enough privilege, please update access level to 1 first')
             return
-    
-        errorcode = self.ser.write(cmds["save_changes"].encode())
+        
+        errorcode = self.ser.write(self.cmds["save_changes"].encode())
         reply = self.ser.readline().decode('utf-8').strip()
         self.check_reply(reply)
     
     
     # --------------------------------------------------------------------------
     # get enable/disable output
     
     def enable_TEC(self):
         """enable TEC"""
-        _ = self.ser.write((cmds["enable_TEC"]+' 1').encode())
+        _ = self.ser.write((self.cmds["enable_TEC"]+' 1').encode())
         reply = self.ser.readline().decode('utf-8').strip()
         self.check_reply(reply)
     
     
     def disable_TEC(self):
         """disable TEC"""
-        errorcode = self.ser.write((cmds["enable_TEC"]+' 0').encode())
+        errorcode = self.ser.write((self.cmds["enable_TEC"]+' 0').encode())
         reply = self.ser.readline().decode('utf-8').strip()
         self.check_reply(reply)
     
     
     # --------------------------------------------------------------------------
     # get single readings
```

### Comparing `IOmatchbox-0.22/src/IOmatchbox/IOmatchbox.py` & `IOmatchbox-0.23/src/IOmatchbox/IOmatchbox.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         and check whether the connected device has an ID like an IO laser. 
         """
         self.ser = serial.Serial()
         self.ser.baudrate = 115200
         self.ser.bytesize = serial.EIGHTBITS
         self.ser.parity = serial.PARITY_NONE
         self.ser.stopbits = serial.STOPBITS_ONE
-        self.ser.timeout = 5
+        self.ser.timeout = 2
         # self.ser.rtscts = True # enable hardware (TRS/CTS) flow control
         if not port:
             # find available ports depending on operating system
             if sys.platform.startswith('linux') or sys.platform.startswith('cygwin'):
                 available_ports = glob.glob('/dev/ttyUSB*')
             elif sys.platform.startswith('win'):
                 available_ports = ['COM%s' % (i + 1) for i in range(256)]
@@ -95,34 +95,46 @@
                 print('failed at port', port)
                 continue
             # check if the selected port has an IO laser by querying the ID
             _ = self.ser.write("NM?".encode())
             # check if the ID contains numbers at [1:4]
             try:
                 reply = self.ser.readline().decode('utf-8').strip()
-                print(reply)
                 int(reply[1:4])
                 print('connected to:', reply[1:-1])
                 break
             except:
                 self.ser.close()
                 time.sleep(0.1)
                 print('not a IO CW laser')
                 pass
         
-        # check if connection is open
-        if not self.ser.is_open:
-            print('opening serial port failed')
-            self.ser = None
+        if self.DEBUG:
+            if self.ser.is_open:
+                print('port', self.ser.port, 'opened')
         return
     
     
+    def port_is_open(self):
+        """check whether serial port is open
+        returns false if port is closed or not a serial port
+        """
+        try: 
+            if not self.ser.is_open:
+                print('serial port not open')
+                return False
+        except AttributeError:
+            print('no serial stage connected, ignoring command')
+            return False
+        return True
+    
+    
     def closelaser(self):
         """close serial connection"""
-        if not self.ser.is_open: print('no serial connection'); return
+        if not self.port_is_open(): return
         self.ser.close()
         if not self.ser.is_open:
             print('connection closed')
     
     # --------------------------------------------------------------------------
     # possible commands (from MB IO user manual)
```

### Comparing `IOmatchbox-0.22/src/IOmatchbox.egg-info/PKG-INFO` & `IOmatchbox-0.23/src/IOmatchbox.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IOmatchbox
-Version: 0.22
+Version: 0.23
 Summary: Functions and examples to control Integrated Optics CW lasers and standalone TECs through serial commands with Python
 Author-email: iancynk <ian.cynk@posteo.eu>
 Project-URL: Homepage, https://github.com/iancynk/IOmatchbox
 Project-URL: Bug Tracker, https://github.com/iancynk/IOmatchbox/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
@@ -30,39 +30,26 @@
 ## Requirements
 Needs `serial` and `pyserial` (both of them are needed for this to work somehow), best installed through:
 ```
 pip install serial pyserial
 ```
 
 ## Usage
-### Pip
 Simply run
 ```
 pip install IOmatchbox
 ```
 Then in your Python script invoke the functions by
 ```
-from IOmatchbox.IOmatchbox import IOM
-from IOmatchbox.IOTEC import IOT
+from IOmatchbox import IOM, IOT
 iom = IOM()
 iot = IOT()
 ```
 With `iom` you can then call all functions and methods of the laser, with `iot` you can communicate with the external TEC.
 
-### Download only file
-Download [IOmatchbox.py](src/IOmatchbox/IOmatchbox.py) and [IOTEC.py](src/IOmatchox/IOTEC.py) and put them in your working directory. 
-
-Then in your Python script invoke the functions by
-```
-from IOmatchbox import IOM
-from IOTEC import IOT
-iom = IOM()
-iot = IOT()
-```
-
 Get some more info with
 ```
 iom.get_settings()
 iom.get_readings()
 iom.laser_status()
 ```
```

