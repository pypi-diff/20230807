# Comparing `tmp/IOmatchbox-0.21.tar.gz` & `tmp/IOmatchbox-0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IOmatchbox-0.21.tar", last modified: Fri Aug  4 14:25:41 2023, max compression
+gzip compressed data, was "IOmatchbox-0.22.tar", last modified: Mon Aug  7 06:41:50 2023, max compression
```

## Comparing `IOmatchbox-0.21.tar` & `IOmatchbox-0.22.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 yfo       (1000) yfo       (1000)        0 2023-08-04 14:25:41.668922 IOmatchbox-0.21/
--rw-r--r--   0 yfo       (1000) yfo       (1000)     1064 2023-05-22 13:50:06.000000 IOmatchbox-0.21/LICENSE
--rw-r--r--   0 yfo       (1000) yfo       (1000)     4102 2023-08-04 14:25:41.668922 IOmatchbox-0.21/PKG-INFO
--rw-r--r--   0 yfo       (1000) yfo       (1000)     3195 2023-08-04 14:14:48.000000 IOmatchbox-0.21/README.md
--rw-r--r--   0 yfo       (1000) yfo       (1000)      951 2023-08-04 14:25:25.000000 IOmatchbox-0.21/pyproject.toml
--rw-r--r--   0 yfo       (1000) yfo       (1000)       38 2023-08-04 14:25:41.668922 IOmatchbox-0.21/setup.cfg
-drwxr-xr-x   0 yfo       (1000) yfo       (1000)        0 2023-08-04 14:25:41.666922 IOmatchbox-0.21/src/
-drwxr-xr-x   0 yfo       (1000) yfo       (1000)        0 2023-08-04 14:25:41.667922 IOmatchbox-0.21/src/IOmatchbox/
--rw-r--r--   0 yfo       (1000) yfo       (1000)    15624 2023-08-04 14:24:28.000000 IOmatchbox-0.21/src/IOmatchbox/IOTEC.py
--rw-r--r--   0 yfo       (1000) yfo       (1000)    24106 2023-08-04 13:51:01.000000 IOmatchbox-0.21/src/IOmatchbox/IOmatchbox.py
--rw-r--r--   0 yfo       (1000) yfo       (1000)        0 2023-08-04 09:16:46.000000 IOmatchbox-0.21/src/IOmatchbox/__init__.py
-drwxr-xr-x   0 yfo       (1000) yfo       (1000)        0 2023-08-04 14:25:41.667922 IOmatchbox-0.21/src/IOmatchbox.egg-info/
--rw-r--r--   0 yfo       (1000) yfo       (1000)     4102 2023-08-04 14:25:41.000000 IOmatchbox-0.21/src/IOmatchbox.egg-info/PKG-INFO
--rw-r--r--   0 yfo       (1000) yfo       (1000)      264 2023-08-04 14:25:41.000000 IOmatchbox-0.21/src/IOmatchbox.egg-info/SOURCES.txt
--rw-r--r--   0 yfo       (1000) yfo       (1000)        1 2023-08-04 14:25:41.000000 IOmatchbox-0.21/src/IOmatchbox.egg-info/dependency_links.txt
--rw-r--r--   0 yfo       (1000) yfo       (1000)       11 2023-08-04 14:25:41.000000 IOmatchbox-0.21/src/IOmatchbox.egg-info/top_level.txt
+drwxr-xr-x   0 yfo       (1000) yfo       (1000)        0 2023-08-07 06:41:50.548720 IOmatchbox-0.22/
+-rw-r--r--   0 yfo       (1000) yfo       (1000)     1064 2023-05-22 13:50:06.000000 IOmatchbox-0.22/LICENSE
+-rw-r--r--   0 yfo       (1000) yfo       (1000)     4102 2023-08-07 06:41:50.548720 IOmatchbox-0.22/PKG-INFO
+-rw-r--r--   0 yfo       (1000) yfo       (1000)     3195 2023-08-04 14:14:48.000000 IOmatchbox-0.22/README.md
+-rw-r--r--   0 yfo       (1000) yfo       (1000)      951 2023-08-07 06:41:21.000000 IOmatchbox-0.22/pyproject.toml
+-rw-r--r--   0 yfo       (1000) yfo       (1000)       38 2023-08-07 06:41:50.548720 IOmatchbox-0.22/setup.cfg
+drwxr-xr-x   0 yfo       (1000) yfo       (1000)        0 2023-08-07 06:41:50.546720 IOmatchbox-0.22/src/
+drwxr-xr-x   0 yfo       (1000) yfo       (1000)        0 2023-08-07 06:41:50.547720 IOmatchbox-0.22/src/IOmatchbox/
+-rw-r--r--   0 yfo       (1000) yfo       (1000)    15547 2023-08-07 06:40:56.000000 IOmatchbox-0.22/src/IOmatchbox/IOTEC.py
+-rw-r--r--   0 yfo       (1000) yfo       (1000)    23987 2023-08-07 06:38:56.000000 IOmatchbox-0.22/src/IOmatchbox/IOmatchbox.py
+-rw-r--r--   0 yfo       (1000) yfo       (1000)        0 2023-08-04 09:16:46.000000 IOmatchbox-0.22/src/IOmatchbox/__init__.py
+drwxr-xr-x   0 yfo       (1000) yfo       (1000)        0 2023-08-07 06:41:50.547720 IOmatchbox-0.22/src/IOmatchbox.egg-info/
+-rw-r--r--   0 yfo       (1000) yfo       (1000)     4102 2023-08-07 06:41:50.000000 IOmatchbox-0.22/src/IOmatchbox.egg-info/PKG-INFO
+-rw-r--r--   0 yfo       (1000) yfo       (1000)      264 2023-08-07 06:41:50.000000 IOmatchbox-0.22/src/IOmatchbox.egg-info/SOURCES.txt
+-rw-r--r--   0 yfo       (1000) yfo       (1000)        1 2023-08-07 06:41:50.000000 IOmatchbox-0.22/src/IOmatchbox.egg-info/dependency_links.txt
+-rw-r--r--   0 yfo       (1000) yfo       (1000)       11 2023-08-07 06:41:50.000000 IOmatchbox-0.22/src/IOmatchbox.egg-info/top_level.txt
```

### Comparing `IOmatchbox-0.21/LICENSE` & `IOmatchbox-0.22/LICENSE`

 * *Files identical despite different names*

### Comparing `IOmatchbox-0.21/PKG-INFO` & `IOmatchbox-0.22/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IOmatchbox
-Version: 0.21
+Version: 0.22
 Summary: Functions and examples to control Integrated Optics CW lasers and standalone TECs through serial commands with Python
 Author-email: iancynk <ian.cynk@posteo.eu>
 Project-URL: Homepage, https://github.com/iancynk/IOmatchbox
 Project-URL: Bug Tracker, https://github.com/iancynk/IOmatchbox/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `IOmatchbox-0.21/README.md` & `IOmatchbox-0.22/README.md`

 * *Files identical despite different names*

### Comparing `IOmatchbox-0.21/pyproject.toml` & `IOmatchbox-0.22/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "IOmatchbox"
-version = "0.21"
+version = "0.22"
 authors = [
   { name="iancynk", email="ian.cynk@posteo.eu" },
 ]
 description = "Functions and examples to control Integrated Optics CW lasers and standalone TECs through serial commands with Python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `IOmatchbox-0.21/src/IOmatchbox/IOTEC.py` & `IOmatchbox-0.22/src/IOmatchbox/IOTEC.py`

 * *Files 4% similar despite different names*

```diff
@@ -92,15 +92,15 @@
                 self.ser.port = port
                 self.ser.open()
                 time.sleep(0.1)
             except:
                 print('failed at port', port)
                 continue
             # check if the selected port has an IO TEC by querying info
-            whatever = self.ser.write("r i".encode())
+            _ = self.ser.write("r i".encode())
 
             # check if the info contains "ExternalTEC"
             try:
                 # output comes in five lines, combine it to one string
                 reply = ''
                 for i in range(5):
                     reply += self.ser.readline().decode('utf-8', 'ignore').strip() + '  '
@@ -148,52 +148,52 @@
     # --------------------------------------------------------------------------
     # read out settings with commands
     
     def get_settings(self, output=False):
         """receive TEC settings
         if output=True, will spill the whole string with info, otherwise only returns it
         """
-        whatever = self.ser.write(cmds["get_settings"].encode())
+        _ = self.ser.write(cmds["get_settings"].encode())
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
-        whatever = self.ser.write(cmds["get_readings"].encode())
+        _ = self.ser.write(cmds["get_readings"].encode())
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
-        whatever = self.ser.write(cmds["get_om"].encode())
+        _ = self.ser.write(cmds["get_om"].encode())
         reply = self.ser.readline().decode('utf-8').strip()
         print('operation mode:', reply)
     
     
     def get_info(self, output=False):
         """receive TEC information
         if output=True, will spill the whole string with info, otherwise only returns it
         """
-        whatever = self.ser.write(cmds["get_info"].encode())
+        _ = self.ser.write(cmds["get_info"].encode())
         # output comes in five lines, combine it to one list
         reply = ''
         for i in range(5):
             reply += self.ser.readline().decode('utf-8', 'ignore').strip() + '  '
         
         if output:
             print('Driver Version, serial number, product code, operating time, switch times')
@@ -203,30 +203,30 @@
             return reply
     
     
     def get_optime(self, output=False):
         """receive laser operation time
         if output=True, will spill the whole string with info, otherwise only returns it
         """
-        whatever = self.ser.write(cmds["get_optime"].encode())
+        _ = self.ser.write(cmds["get_optime"].encode())
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
-        whatever = self.ser.write(cmds["get_access_level"].encode())
+        _ = self.ser.write(cmds["get_access_level"].encode())
         reply = self.ser.readline().decode('utf-8').strip()
         access_level = int(reply.split()[2])
         return access_level
     
     
     def set_access_level(self, level):
         """change user access level (default level over serial is 0)
@@ -246,15 +246,15 @@
                 print('please input a 5 digit number as access level code')
                 return
         else:
             print('invalid access level, please choose a number in [0..3]')
             return
     
         cmd = cmds["set_access_level"]+' ' + str(level) + ' ' + input_code
-        whatever = self.ser.write(cmd.encode())
+        _ = self.ser.write(cmd.encode())
         reply = self.ser.readline().decode('utf-8').strip()
         # check if access level code worked
         if reply == '<ERR 4>':
             print('invalid code to unlock access level', str(level), ': ', input_code)
         else:
             self.check_reply(reply)
         print('Access level:', str(get_access_level()))
@@ -265,15 +265,15 @@
         """set TEC temp (should be in centi-degC, eg 2550)"""
         if self.get_access_level() < 1:
             print('not enough privilege, please update access level to 1 first')
             return
         
         old_settemp = self.get_TEC_set_temp()
         if (settemp > 2000) & (settemp < 3000):
-            whatever = self.ser.write((cmds["set_TEC_temp"]+ ' ' + str(settemp)).encode())
+            _ = self.ser.write((cmds["set_TEC_temp"]+ ' ' + str(settemp)).encode())
             reply = self.ser.readline().decode('utf-8').strip()
             self.check_reply(reply)
             new_settemp = self.get_TEC_set_temp()
         else:
             print('please give a reasonable input temperature (2000-3000) as integer')
     
     
@@ -313,15 +313,15 @@
     
     
     # --------------------------------------------------------------------------
     # get enable/disable output
     
     def enable_TEC(self):
         """enable TEC"""
-        whatever = self.ser.write((cmds["enable_TEC"]+' 1').encode())
+        _ = self.ser.write((cmds["enable_TEC"]+' 1').encode())
         reply = self.ser.readline().decode('utf-8').strip()
         self.check_reply(reply)
     
     
     def disable_TEC(self):
         """disable TEC"""
         errorcode = self.ser.write((cmds["enable_TEC"]+' 0').encode())
@@ -407,12 +407,12 @@
         print('laser diode turned on ', switch_times)
     
     # --------------------------------------------------------------------------
     # send command
     
     def send_cmd(self, cmd):
         """send an arbitrary cmd"""
-        whatever = self.ser.write(cmd.encode())
+        _ = self.ser.write(cmd.encode())
         reply = self.ser.readline().decode('utf-8').strip()
         print(reply)
 
 # EOF --------------------------------------------------------------------------
```

### Comparing `IOmatchbox-0.21/src/IOmatchbox/IOmatchbox.py` & `IOmatchbox-0.22/src/IOmatchbox/IOmatchbox.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
                 self.ser.port = port
                 self.ser.open()
                 time.sleep(0.1)
             except:
                 print('failed at port', port)
                 continue
             # check if the selected port has an IO laser by querying the ID
-            whatever = self.ser.write("NM?".encode())
+            _ = self.ser.write("NM?".encode())
             # check if the ID contains numbers at [1:4]
             try:
                 reply = self.ser.readline().decode('utf-8').strip()
                 print(reply)
                 int(reply[1:4])
                 print('connected to:', reply[1:-1])
                 break
@@ -150,31 +150,31 @@
     
     
     # --------------------------------------------------------------------------
     # read out settings with commands
     
     def get_ID(self):
         """get module ID"""
-        whatever = self.ser.write(self.cmds["product_ID"].encode())
+        _ = self.ser.write(self.cmds["product_ID"].encode())
         reply = self.ser.readline().decode('utf-8').strip()
         print('product ID:', reply[1:-1])
     
     
     def get_productcode(self):
         """get module product code"""
-        whatever = self.ser.write(self.cmds["product_code"].encode())
+        _ = self.ser.write(self.cmds["product_code"].encode())
         reply = self.ser.readline().decode('utf-8').strip()
         print('product code:', reply[1:-1])
     
     
     def get_settings(self, output=False):
         """receive laser settings
         if output=True, will spill the whole string with info, otherwise only returns it
         """
-        whatever = self.ser.write(self.cmds["get_settings"].encode())
+        _ = self.ser.write(self.cmds["get_settings"].encode())
         reply = self.ser.readline().decode('utf-8').strip()
         if output:
             print('Settings: crystal set temp, laser diode set temperature, \
     laser diode set current, feedback DAC set value, optical power set value, \
     laser diode current limit (mA), autostart mode, access level, fan set temp')
             print(reply)
             return
@@ -182,38 +182,38 @@
             return reply
     
     
     def get_readings(self, output=False):
         """receive laser readings
         if output=True, will spill the whole string with info, otherwise only returns it
         """
-        whatever = self.ser.write(self.cmds["get_readings"].encode())
+        _ = self.ser.write(self.cmds["get_readings"].encode())
         reply = self.ser.readline().decode('utf-8').strip()
         if output:
             print('Readings:laser diode temperature, crystal temperature (negative if there is no crystal), \
     laser base temperature, laser diode current, crystal TEC load, \
     laser diode TEC load, system status, fan load, input voltage')
             print(reply)
             return
         else:
             return reply
     
     
     def get_om(self):
         """receive operation mode (APC/ACC)"""
-        whatever = self.ser.write(self.cmds["get_om"].encode())
+        _ = self.ser.write(self.cmds["get_om"].encode())
         reply = self.ser.readline().decode('utf-8').strip()
         print('operation mode:', reply)
     
     
     def get_info(self, output=False):
         """receive laser information
         if output=True, will spill the whole string with info, otherwise only returns it
         """
-        whatever = self.ser.write(self.cmds["get_info"].encode())
+        _ = self.ser.write(self.cmds["get_info"].encode())
         # output comes in five lines, combine it to one list
         reply = ''
         for i in range(5):
             reply += self.ser.readline().decode('utf-8').strip() + '  '
         
         if output:
             print('firmware version, serial number, product code, operating time, \
@@ -224,30 +224,30 @@
             return reply
     
     
     def get_optime(self, output=False):
         """receive laser operation time
         if output=True, will spill the whole string with info, otherwise only returns it
         """
-        whatever = self.ser.write(self.cmds["get_optime"].encode())
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
-        whatever = self.ser.write(self.cmds["get_access_level"].encode())
+        _ = self.ser.write(self.cmds["get_access_level"].encode())
         reply = self.ser.readline().decode('utf-8').strip()
         access_level = int(reply.split()[2])
         return access_level
     
     
     def set_access_level(self, level, input_code=''):
         """change user access level (default level over serial is 0)
@@ -269,15 +269,15 @@
                     print('please input a 5 digit number as access level code')
                     return
             else:
                 print('invalid access level, please choose a number in [0..3]')
                 return
 
         cmd = self.cmds["set_access_level"]+' ' + str(level) + ' ' + input_code
-        whatever = self.ser.write(cmd.encode())
+        _ = self.ser.write(cmd.encode())
         reply = self.ser.readline().decode('utf-8').strip()
         # check if access level code worked
         if reply == '<ERR 4>':
             print('invalid code to unlock access level', str(level), ': ', input_code)
         else:
             self.check_reply(reply)
         print('Access level:', str(self.get_access_level()))
@@ -295,15 +295,15 @@
         # check if there is actually a crystal
         if currtemp < 0:
             print('no crystal, ignoring input')
             return
         
         old_settemp = self.get_crystal_set_temp()
         if (settemp > 2500) & (settemp < 3500):
-            whatever = self.ser.write((self.cmds["set_crystal_temp"]+ ' ' + str(settemp)).encode())
+            _ = self.ser.write((self.cmds["set_crystal_temp"]+ ' ' + str(settemp)).encode())
             reply = self.ser.readline().decode('utf-8').strip()
             self.check_reply(reply)
             new_settemp = self.get_crystal_set_temp()
         else:
             print('please give a reasonable input temperature (2500-3500) as integer')
     
     
@@ -312,15 +312,15 @@
         if self.get_access_level() < 3:
             print('not enough privilege, please update access level to 3 first')
             return
         
         currtemp = self.get_diode_temp_num()
         old_settemp = self.get_diode_set_temp()
         if (settemp > 2500) & (settemp < 3500):
-            whatever = self.ser.write((self.cmds["set_diode_temp"]+ ' ' + str(settemp)).encode())
+            _ = self.ser.write((self.cmds["set_diode_temp"]+ ' ' + str(settemp)).encode())
             reply = self.ser.readline().decode('utf-8').strip()
             self.check_reply(reply)
             new_settemp = self.get_diode_set_temp()
         else:
             print('please give a reasonable input temperature (2500-3500) as integer')
     
     
@@ -330,15 +330,15 @@
             print('not enough privilege, please update access level to 3 first')
             return
         
         currcurr = self.get_diode_current()
         old_setcurr = self.get_diode_set_current()
         currlimit = self.get_diode_current_limit()
         if setcurr <= currlimit:
-            whatever = self.ser.write((self.cmds["set_diode_current"]+ ' ' + str(setcurr)).encode())
+            _ = self.ser.write((self.cmds["set_diode_current"]+ ' ' + str(setcurr)).encode())
             reply = self.ser.readline().decode('utf-8').strip()
             self.check_reply(reply)
             new_setcurr = self.get_diode_set_current()
         elif setcurr > currlimit:
             print('current larger than diode current limit, please set a current less than', currlimit, 'mA')
         else:
             print('please give a reasonable input current')
@@ -350,30 +350,30 @@
             print('not enough privilege, please update access level to 1 first')
             return
         
         oldsetpower = self.get_opt_set_power()
         if oldsetpower == 'nan':
             print('sorry, optical power can not be changed on this device')
         else:
-            whatever = self.ser.write((self.cmds["set_opt_power"] + ' ' + str(setpower)).encode())
+            _ = self.ser.write((self.cmds["set_opt_power"] + ' ' + str(setpower)).encode())
             reply = self.ser.readline().decode('utf-8').strip()
             self.check_reply(reply)
             newsetpower = self.get_opt_set_power()
         return
     
     
     def set_DAC_value(self, setvalue):
         """set feedback DAC value (0..8191)"""
         if self.get_access_level() < 1:
             print('not enough privilege, please update access level to 1 first')
             return
         
         old_setvalue = self.get_DAC_set_value()
         if (setvalue > 0) & (setvalue <= 8191):
-            whatever = self.ser.write((self.cmds["set_feedback_DAC"]+ ' ' + str(setvalue)).encode())
+            _ = self.ser.write((self.cmds["set_feedback_DAC"]+ ' ' + str(setvalue)).encode())
             reply = self.ser.readline().decode('utf-8').strip()
             self.check_reply(reply)
             new_setvalue = self.get_DAC_set_value()
         else:
             print('please give a reasonable input value [0..8191]')
     
     
@@ -381,15 +381,15 @@
         """set fan temp (should be in centi-degC, eg 2550)"""
         if self.get_access_level() < 1:
             print('not enough privilege, please update access level to 1 first')
             return
         
         old_settemp = self.get_fan_set_temp()
         if (settemp > 2500) & (settemp < 3500):
-            whatever = self.ser.write((self.cmds["set_fan_temp"]+ ' ' + str(settemp)).encode())
+            _ = self.ser.write((self.cmds["set_fan_temp"]+ ' ' + str(settemp)).encode())
             reply = self.ser.readline().decode('utf-8').strip()
             self.check_reply(reply)
             new_settemp = self.get_fan_set_temp()
         else:
             print('please give a reasonable input temperature (2500-3500) as integer')
     
     
@@ -426,15 +426,15 @@
         self.check_reply(reply)
     
     # --------------------------------------------------------------------------
     # get enable/disable output
     
     def start_laser(self):
         """enable laser output"""
-        whatever = self.ser.write((self.cmds["enable_laser"]+' 1').encode())
+        _ = self.ser.write((self.cmds["enable_laser"]+' 1').encode())
         reply = self.ser.readline().decode('utf-8').strip()
         self.check_reply(reply)
     
     
     def stop_laser(self):
         """disable laser output"""
         errorcode = self.ser.write((self.cmds["enable_laser"]+' 0').encode())
```

### Comparing `IOmatchbox-0.21/src/IOmatchbox.egg-info/PKG-INFO` & `IOmatchbox-0.22/src/IOmatchbox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IOmatchbox
-Version: 0.21
+Version: 0.22
 Summary: Functions and examples to control Integrated Optics CW lasers and standalone TECs through serial commands with Python
 Author-email: iancynk <ian.cynk@posteo.eu>
 Project-URL: Homepage, https://github.com/iancynk/IOmatchbox
 Project-URL: Bug Tracker, https://github.com/iancynk/IOmatchbox/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

