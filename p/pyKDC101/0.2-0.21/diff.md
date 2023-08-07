# Comparing `tmp/pyKDC101-0.2.tar.gz` & `tmp/pyKDC101-0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyKDC101-0.2.tar", last modified: Fri Aug  4 13:19:37 2023, max compression
+gzip compressed data, was "pyKDC101-0.21.tar", last modified: Mon Aug  7 11:45:54 2023, max compression
```

## Comparing `pyKDC101-0.2.tar` & `pyKDC101-0.21.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 yfo       (1000) yfo       (1000)        0 2023-08-04 13:19:37.756667 pyKDC101-0.2/
--rw-r--r--   0 yfo       (1000) yfo       (1000)     1064 2023-08-04 09:25:21.000000 pyKDC101-0.2/LICENSE
--rw-r--r--   0 yfo       (1000) yfo       (1000)     4290 2023-08-04 13:19:37.756667 pyKDC101-0.2/PKG-INFO
--rw-r--r--   0 yfo       (1000) yfo       (1000)     3433 2023-08-04 13:18:26.000000 pyKDC101-0.2/README.md
--rw-r--r--   0 yfo       (1000) yfo       (1000)      900 2023-08-04 13:15:12.000000 pyKDC101-0.2/pyproject.toml
--rw-r--r--   0 yfo       (1000) yfo       (1000)       38 2023-08-04 13:19:37.756667 pyKDC101-0.2/setup.cfg
-drwxr-xr-x   0 yfo       (1000) yfo       (1000)        0 2023-08-04 13:19:37.755667 pyKDC101-0.2/src/
-drwxr-xr-x   0 yfo       (1000) yfo       (1000)        0 2023-08-04 13:19:37.755667 pyKDC101-0.2/src/pyKDC101/
--rw-r--r--   0 yfo       (1000) yfo       (1000)        0 2023-08-04 09:16:46.000000 pyKDC101-0.2/src/pyKDC101/__init__.py
--rw-r--r--   0 yfo       (1000) yfo       (1000)    20443 2023-08-04 08:26:14.000000 pyKDC101-0.2/src/pyKDC101/pyKDC101.py
-drwxr-xr-x   0 yfo       (1000) yfo       (1000)        0 2023-08-04 13:19:37.756667 pyKDC101-0.2/src/pyKDC101.egg-info/
--rw-r--r--   0 yfo       (1000) yfo       (1000)     4290 2023-08-04 13:19:37.000000 pyKDC101-0.2/src/pyKDC101.egg-info/PKG-INFO
--rw-r--r--   0 yfo       (1000) yfo       (1000)      226 2023-08-04 13:19:37.000000 pyKDC101-0.2/src/pyKDC101.egg-info/SOURCES.txt
--rw-r--r--   0 yfo       (1000) yfo       (1000)        1 2023-08-04 13:19:37.000000 pyKDC101-0.2/src/pyKDC101.egg-info/dependency_links.txt
--rw-r--r--   0 yfo       (1000) yfo       (1000)        9 2023-08-04 13:19:37.000000 pyKDC101-0.2/src/pyKDC101.egg-info/top_level.txt
+drwxr-xr-x   0 yfo       (1000) yfo       (1000)        0 2023-08-07 11:45:54.786305 pyKDC101-0.21/
+-rw-r--r--   0 yfo       (1000) yfo       (1000)     1064 2023-08-04 09:25:21.000000 pyKDC101-0.21/LICENSE
+-rw-r--r--   0 yfo       (1000) yfo       (1000)     4292 2023-08-07 11:45:54.785305 pyKDC101-0.21/PKG-INFO
+-rw-r--r--   0 yfo       (1000) yfo       (1000)     3433 2023-08-04 13:18:26.000000 pyKDC101-0.21/README.md
+-rw-r--r--   0 yfo       (1000) yfo       (1000)      902 2023-08-07 11:27:42.000000 pyKDC101-0.21/pyproject.toml
+-rw-r--r--   0 yfo       (1000) yfo       (1000)       38 2023-08-07 11:45:54.786305 pyKDC101-0.21/setup.cfg
+drwxr-xr-x   0 yfo       (1000) yfo       (1000)        0 2023-08-07 11:45:54.784305 pyKDC101-0.21/src/
+drwxr-xr-x   0 yfo       (1000) yfo       (1000)        0 2023-08-07 11:45:54.785305 pyKDC101-0.21/src/pyKDC101/
+-rw-r--r--   0 yfo       (1000) yfo       (1000)      231 2023-08-07 11:45:28.000000 pyKDC101-0.21/src/pyKDC101/__init__.py
+-rw-r--r--   0 yfo       (1000) yfo       (1000)    20477 2023-08-07 11:36:26.000000 pyKDC101-0.21/src/pyKDC101/core.py
+drwxr-xr-x   0 yfo       (1000) yfo       (1000)        0 2023-08-07 11:45:54.785305 pyKDC101-0.21/src/pyKDC101.egg-info/
+-rw-r--r--   0 yfo       (1000) yfo       (1000)     4292 2023-08-07 11:45:54.000000 pyKDC101-0.21/src/pyKDC101.egg-info/PKG-INFO
+-rw-r--r--   0 yfo       (1000) yfo       (1000)      222 2023-08-07 11:45:54.000000 pyKDC101-0.21/src/pyKDC101.egg-info/SOURCES.txt
+-rw-r--r--   0 yfo       (1000) yfo       (1000)        1 2023-08-07 11:45:54.000000 pyKDC101-0.21/src/pyKDC101.egg-info/dependency_links.txt
+-rw-r--r--   0 yfo       (1000) yfo       (1000)        9 2023-08-07 11:45:54.000000 pyKDC101-0.21/src/pyKDC101.egg-info/top_level.txt
```

### Comparing `pyKDC101-0.2/LICENSE` & `pyKDC101-0.21/LICENSE`

 * *Files identical despite different names*

### Comparing `pyKDC101-0.2/PKG-INFO` & `pyKDC101-0.21/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: pyKDC101
-Version: 0.2
+Version: 0.21
 Summary: Functions and examples to control Thorlabs KDC101 through serial commands
 Author-email: iancynk <ian.cynk@posteo.eu>
 Project-URL: Homepage, https://github.com/iancynk/pyKDC101
 Project-URL: Bug Tracker, https://github.com/iancynk/pyKDC101/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyKDC101
 Functions and examples to control Thorlabs KDC101 through serial.
 Mainly for Python, additionally some basic usage for MATLAB.
 Here, the controller is used to move a Thorlabs rotation stage (PRM1-Z8).
```

### Comparing `pyKDC101-0.2/README.md` & `pyKDC101-0.21/README.md`

 * *Files identical despite different names*

### Comparing `pyKDC101-0.2/pyproject.toml` & `pyKDC101-0.21/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyKDC101"
-version = "0.2"
+version = "0.21"
 authors = [
   { name="iancynk", email="ian.cynk@posteo.eu" },
 ]
 description = "Functions and examples to control Thorlabs KDC101 through serial commands"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX :: Linux",
     "Intended Audience :: Education",
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering",
```

### Comparing `pyKDC101-0.2/src/pyKDC101/pyKDC101.py` & `pyKDC101-0.21/src/pyKDC101/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -190,40 +190,50 @@
                 self.ser.open()
                 time.sleep(0.1)
                 break
             except:
                 print('failed at port', port)
                 pass
         
-        if self.ser.is_open:
-            print('is open: ', self.ser.is_open)
-        else:
-            print('could not find any serial port')
+        if self.DEBUG:
+            if self.ser.is_open:
+                print('port', self.ser.port, 'opened')
         return
     
     
+    def port_is_open(self):
+        try: 
+            if not self.ser.is_open:
+                print('serial port not open')
+                return False
+        except ValueError:
+            print('no serial stage connected, ignoring command')
+            return False
+        return True
+    
+    
     def closestage(self):
         """close serial connection"""
-        if not self.ser.is_open: print('no serial connection'); return
+        if not self.port_is_open(): return
         self.ser.close()
         print('is open: ', self.ser.is_open)
     
     
     def sendcmd(self, string):
         """send a command"""
-        if not self.ser.is_open: print('no serial connection'); return
+        if not self.port_is_open(): return
         splitstring = string.split() # separate in to list of hex values
         cmd = [int(str, 16) for str in splitstring] # convert to integer
         if self.DEBUG: print('sending command: ', cmd)
         self.ser.write(bytes(cmd)) # send integer in binary format to stage
     
     
     def recvreply(self):
         """receive and parse reply"""
-        if not self.ser.is_open: print('no serial connection'); return
+        if not self.port_is_open(): return
         time.sleep(0.04)  # necessary delay
         reply = ''
         while self.ser.in_waiting > 0:
             # read every single byte (converted to hex) and add whitespace
             reply += self.ser.read().hex()
             reply += ' '
         if self.DEBUG:
@@ -240,89 +250,91 @@
         if not reply:
             msg = ''
             params = ''
             return msg, params
         
         mID = reply[0:5] # get the first two bytes as message ID
         header = reply[0:17] # get the first 6 bytes as header
-        if mID == '06 00':
-            # hardware info, 90 bytes (always including header)
-            msg = 'hardware info'
-            length = 84
-        elif mID == '0b 04':
-            msg = 'Enccounter'
-            length = 6
-        elif mID == '12 04':
-            msg = 'Poscounter'
-            length = 6
-        elif mID == '15 04':
-            msg = 'Velparams'
-            length = 14
-        elif mID == '18 04':
-            msg = 'Jogparams'
-            length = 22
-        elif mID == '22 05':
-            msg ='MMI parameters'
-            length = 36
-        elif mID == '3c 04':
-            msg = 'GenMoveparams'
-            length = 6
-        elif mID == '42 04':
-            msg = 'Homeparams'
-            length = 14
-        elif mID == '44 04':
-            msg = 'homed'
-            length = 0
-        elif mID == '47 04':
-            msg = 'Moverelparams'
-            length = 6
-        elif mID == '52 04':
-            msg = 'Moveabsparams'
-            length = 6
-        elif mID == '64 04':
-            msg = 'moved'
-            length = 14
-        elif mID == '66 04':
-            msg = 'stopped'
-            length = 14
-        else:
-            print('not a recogniced message ID:', mID)
-            msg = ''
-            length = 0
+        match mID:
+            case '06 00':
+                # hardware info, 90 bytes (always including header)
+                msg = 'hardware info'
+                length = 84
+            case '0b 04':
+                msg = 'Enccounter'
+                length = 6
+            case '12 04':
+                msg = 'Poscounter'
+                length = 6
+            case '15 04':
+                msg = 'Velparams'
+                length = 14
+            case '18 04':
+                msg = 'Jogparams'
+                length = 22
+            case '22 05':
+                msg ='MMI parameters'
+                length = 36
+            case '3c 04':
+                msg = 'GenMoveparams'
+                length = 6
+            case '42 04':
+                msg = 'Homeparams'
+                length = 14
+            case '44 04':
+                msg = 'homed'
+                length = 0
+            case '47 04':
+                msg = 'Moverelparams'
+                length = 6
+            case '52 04':
+                msg = 'Moveabsparams'
+                length = 6
+            case '64 04':
+                msg = 'moved'
+                length = 14
+            case '66 04':
+                msg = 'stopped'
+                length = 14
+                
+            case _:
+                print('not a recogniced message ID:', mID)
+                msg = ''
+                length = 0
         
         # extract parameter (if more than 6 bytes)
         if length > 0:
             msg_params = reply[18:18+(3*length-1)]
         else:
             msg_params =  ''
         return msg, msg_params
     
     
     # --------------------------------------------------------------------------
     # CONTROLLER INFO/FUNCTIONS
     
     def identify(self):
         """flash display to indicate which controller is addressed"""
-        if not self.ser.is_open: print('no serial connection'); return
+        if not self.port_is_open(): return
         self.sendcmd(self.cmds['identify'])
     
     
     def get_serial(self):
         """get controller serial number"""
-        if not self.ser.is_open: print('no serial connection'); return
+        if not self.port_is_open(): return
         self.sendcmd(self.cmds['req_info'])
         reply = self.recvreply()
         msg, hwinfo = self.decodereply(reply)
         sn = self.hexstr_to_int(hwinfo[0:11]) # 4 byte serial number
         return sn
     
     
     def get_info(self):
         """get hardware information, see APT protocol page 46"""
-        if not self.ser.is_open: print('no serial connection'); return
+        if not self.port_is_open(): return
         self.sendcmd(self.cmds['req_info'])
         reply = self.recvreply()
         msg, hwinfo = self.decodereply(reply)
         sn = self.hexstr_to_int(hwinfo[0:11]) # 4 byte serial number
         model_number = self.hexstr_to_ascii(hwinfo[12:35]) # 8 byte alphanumeric model number
         hw_type = self.hexstr_to_int(hwinfo[36:41]) # 2 byte describes type of hardware
         fw_minor = self.hexstr_to_int(hwinfo[42:44]) # minor firmware version (1 byte)
@@ -335,15 +347,15 @@
         print(f"serial number:\t\t{sn}\nmodel number:\t\t{model_number}\nfirmware version:\t{fw_major}.{fw_interim}.{fw_minor}")
         print(f"hardware type:\t\t{hw_type}\nhardware version:\t{hw_version}")
         print(f"modification state:\t{hw_mod_state}\nnumber of channels:\t{n_channels}")
     
     
     def get_mmi_params(self):
         """get settings for top panel and wheel"""
-        if not self.ser.is_open: print('no serial connection'); return
+        if not self.port_is_open(): return
         self.sendcmd(self.cmds['req_mmiparams'])
         reply = self.recvreply()
         msg, mmiinfo = self.decodereply(reply)
         chan_ident = self.hexstr_to_int(mmiinfo[0:5])
         JSMode = self.hexstr_to_int(mmiinfo[6:11])
         JSMaxVel = self.hexstr_to_int(mmiinfo[12:23])
         JSAccn = self.hexstr_to_int(mmiinfo[24:35])
@@ -356,15 +368,15 @@
         print(f"JSMode: {JSMode}\tJSMaxVel: {JSMaxVel}\tJSAccn: {JSAccn}\tDirSense:{DirSense}")
         print(f"Preset Positions:\t{PreSetPos1}\t{PreSetPos2}")
         print(f"Display Parameters: {DispBrightness}, {DispTimeout}, {DispDimLevel}")
     
     
     def get_disp_params(self):
         """get settings for display"""
-        if not self.ser.is_open: print('no serial connection'); return
+        if not self.port_is_open(): return
         self.sendcmd(self.cmds['req_mmiparams'])
         reply = self.recvreply()
         msg, mmiinfo = self.decodereply(reply)
         DispBrightness = self.hexstr_to_int(mmiinfo[66:71])
         DispTimeout = self.hexstr_to_int(mmiinfo[72:77])
         DispDimLevel = self.hexstr_to_int(mmiinfo[78:83])
         print(f"Display Brightness: {DispBrightness}%")
@@ -377,131 +389,134 @@
     # --------------------------------------------------------------------------
     # STAGE FUNCTIONS
     # careful, these cmds keep running until the stage is done moving!
     # they are waiting for a reply that the motor has reached its designated position
     
     def move_abs_wait(self, angle):
         """absolute movement, wait till movement completed"""
-        if not self.ser.is_open: print('no serial connection'); return
+        if not self.port_is_open(): return
         cmd = self.cmds["move_abs_angle"] + self.convert_angle(angle)
         self.sendcmd(cmd)
         msg = ''
         while not msg == 'moved':
             time.sleep(0.5)
             reply = self.recvreply()
             msg, params = self.decodereply(reply)
-            if self.DEBUG: print('params')
+            if self.DEBUG:
+                if len(params) > 0:
+                    pos = params[6:17]
+                    print('at:', self.convert_enccnt(pos), 'deg')
         if self.DEBUG: print('movement completed')
     
     
     def move_rel_wait(self, angle):
         """relative movement, wait till movement completed"""
-        if not self.ser.is_open: print('no serial connection'); return
+        if not self.port_is_open(): return
         cmd = self.cmds["move_rel_angle"] + self.convert_angle(angle)
         self.sendcmd(cmd)
         msg = ''
         while not msg == 'moved':
             time.sleep(0.5)
             reply = self.recvreply()
             msg, params = self.decodereply(reply)
-            if len(params) > 0:
-                pos = params[6:17]
-                print('at:', self.convert_enccnt(pos), 'deg')
-            if self.DEBUG: print('params')
+            if self.DEBUG:
+                if len(params) > 0:
+                    pos = params[6:17]
+                    print('at:', self.convert_enccnt(pos), 'deg')
         if self.DEBUG: print('movement completed')
     
     
     def move_home_wait(self):
         """move home, wait till movement completed"""
-        if not self.ser.is_open: print('no serial connection'); return
+        if not self.port_is_open(): return
         self.sendcmd(self.cmds["move_home"])
         msg = ''
         while not msg == 'homed':
             time.sleep(0.5)
             reply = self.recvreply()
             msg,_ = self.decodereply(reply)
         if self.DEBUG: print('finally homed')
     
     
     # --------------------------------------------------------------------------
     # interruptible movement cmds
     
     def move_abs(self, angle):
         """absolute movement"""
-        if not self.ser.is_open: print('no serial connection'); return
+        if not self.port_is_open(): return
         cmd = self.cmds["move_abs_angle"] + self.convert_angle(angle)
         self.sendcmd(cmd)
     
     
     def move_rel(self, angle):
         """relative movement"""
-        if not self.ser.is_open: print('no serial connection'); return
+        if not self.port_is_open(): return
         cmd = self.cmds["move_rel_angle"] + self.convert_angle(angle)
         self.sendcmd(cmd)
     
     
     def move_home(self):
         """move home"""
-        if not self.ser.is_open: print('no serial connection'); return
+        if not self.port_is_open(): return
         self.sendcmd(self.cmds["move_home"])
     
     
     def stop_move(self):
         """stop current move: This does NOT interrupt the movement_wait cmds"""
-        if not self.ser.is_open: print('no serial connection'); return
+        if not self.port_is_open(): return
         self.sendcmd(self.cmds["move_stop"])
         msg = ''
         while not msg == 'stopped':
             time.sleep(0.5)
             reply = self.recvreply()
             msg, params = self.decodereply(reply)
-            if len(params) > 0:
-                pos = params[6:17]
-                print('at:', self.convert_enccnt(pos), 'deg')
-            if self.DEBUG: print('params')
+            if self.DEBUG:
+                if len(params) > 0:
+                    pos = params[6:17]
+                    print('at:', self.convert_enccnt(pos), 'deg')
         if self.DEBUG: print('stopped')
     
     
     # --------------------------------------------------------------------------
     # read position of stage
     
     def get_pos_angle(self):
         """
         get position (poscnt) and return as angle
         try it two times because somehow often fails on the first request
         """
-        if not self.ser.is_open: print('no serial connection'); return
+        if not self.port_is_open(): return
         for n in range(2):
             self.sendcmd(self.cmds["req_poscounter"])
             reply = self.recvreply()
             try:
+                if self.DEBUG: print(reply)
                 msg, params = self.decodereply(reply)
                 pos = params[6:]
                 angle = self.convert_enccnt(pos)
                 break
             except ValueError:
                 position = ''
                 angle = ''
-                if self.DEBUG: print(reply)
         return angle
     
     
     def get_enc_angle(self):
         """
         get encoder position (enccnt) and return as angle
         """
-        if not self.ser.is_open: print('no serial connection'); return
+        if not self.port_is_open(): return
         for n in range(2):
             self.sendcmd(self.cmds["req_enccounter"])
             reply = self.recvreply()
             try:
+                if self.DEBUG: print(reply)
                 msg, params = self.decodereply(reply)
                 pos = params[6:]
                 angle = self.convert_enccnt(pos)
                 break
             except ValueError:
                 position = ''
                 angle = ''
-                if self.DEBUG: print(reply)
         return angle
 
 # EOF --------------------------------------------------------------------------
```

### Comparing `pyKDC101-0.2/src/pyKDC101.egg-info/PKG-INFO` & `pyKDC101-0.21/src/pyKDC101.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: pyKDC101
-Version: 0.2
+Version: 0.21
 Summary: Functions and examples to control Thorlabs KDC101 through serial commands
 Author-email: iancynk <ian.cynk@posteo.eu>
 Project-URL: Homepage, https://github.com/iancynk/pyKDC101
 Project-URL: Bug Tracker, https://github.com/iancynk/pyKDC101/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyKDC101
 Functions and examples to control Thorlabs KDC101 through serial.
 Mainly for Python, additionally some basic usage for MATLAB.
 Here, the controller is used to move a Thorlabs rotation stage (PRM1-Z8).
```

