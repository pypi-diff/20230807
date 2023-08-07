# Comparing `tmp/grblhud-1.1.0.tar.gz` & `tmp/grblhud-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grblhud-1.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "grblhud-1.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `grblhud-1.1.0.tar` & `grblhud-1.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1085 2023-06-10 12:49:32.174417 grblhud-1.1.0/LICENSE
--rw-r--r--   0        0        0     5642 2023-08-05 15:23:55.947899 grblhud-1.1.0/README.md
--rw-r--r--   0        0        0     4801 2023-06-10 12:55:49.202815 grblhud-1.1.0/grblhud/README.md
--rw-r--r--   0        0        0       81 2023-08-05 15:00:02.236925 grblhud-1.1.0/grblhud/__init__.py
--rw-r--r--   0        0        0     1476 2023-06-10 11:58:10.835254 grblhud-1.1.0/grblhud/__main__.py
--rw-r--r--   0        0        0    14158 2023-08-05 14:52:50.818228 grblhud-1.1.0/grblhud/grblbuffer.py
--rw-r--r--   0        0        0    33299 2023-08-05 14:54:48.460599 grblhud-1.1.0/grblhud/grblhudloop.py
--rw-r--r--   0        0        0     6053 2023-06-10 11:58:10.835254 grblhud-1.1.0/grblhud/grblmessages.py
--rw-r--r--   0        0        0     8040 2023-06-10 11:58:10.835254 grblhud-1.1.0/grblhud/lineinput.py
--rw-r--r--   0        0        0     2994 2023-06-10 11:58:10.825254 grblhud-1.1.0/grblhud/unblockedgetch.py
--rw-r--r--   0        0        0      645 2023-06-10 12:50:36.895883 grblhud-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     6131 1970-01-01 00:00:00.000000 grblhud-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-06-10 12:49:32.174417 grblhud-1.2.0/LICENSE
+-rw-r--r--   0        0        0     5917 2023-08-07 10:48:11.312829 grblhud-1.2.0/README.md
+-rw-r--r--   0        0        0     4801 2023-06-10 12:55:49.202815 grblhud-1.2.0/grblhud/README.md
+-rw-r--r--   0        0        0       81 2023-08-07 10:14:10.107699 grblhud-1.2.0/grblhud/__init__.py
+-rw-r--r--   0        0        0     1476 2023-06-10 11:58:10.835254 grblhud-1.2.0/grblhud/__main__.py
+-rw-r--r--   0        0        0    14340 2023-08-07 10:33:48.394369 grblhud-1.2.0/grblhud/grblbuffer.py
+-rw-r--r--   0        0        0    40172 2023-08-07 10:33:57.774572 grblhud-1.2.0/grblhud/grblhudloop.py
+-rw-r--r--   0        0        0     6053 2023-06-10 11:58:10.835254 grblhud-1.2.0/grblhud/grblmessages.py
+-rw-r--r--   0        0        0     8040 2023-06-10 11:58:10.835254 grblhud-1.2.0/grblhud/lineinput.py
+-rw-r--r--   0        0        0     2994 2023-06-10 11:58:10.825254 grblhud-1.2.0/grblhud/unblockedgetch.py
+-rw-r--r--   0        0        0      645 2023-06-10 12:50:36.895883 grblhud-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6406 1970-01-01 00:00:00.000000 grblhud-1.2.0/PKG-INFO
```

### Comparing `grblhud-1.1.0/LICENSE` & `grblhud-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `grblhud-1.1.0/README.md` & `grblhud-1.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # grblhub
 Grblhub is a command line based tool to handle grbl code.
 
 It features full control of the grbl v1.1 device and supports <i>realtime</i> direct commands and buffered streaming of commands and programs.</br>
 Grbl state is in line viewable, showing (all) machine states i.e. <i>Idle, Run, Hold, Jog, Alarm, Door, Check, Home, Sleep</i> in color. State also includes current buffered (pending) gcode blocks (and no scrolling <i>ok's</i>)</br>
 Grbl v1.1 error and Alarm code definitions are shown when they occur.
 Spindle and Feed settings can be updated realtime while gcode (G1) is running; gcode programs can be loaded and run with specific <i>Spindle</i> and <i>Feed</i> settings.</br>
+It is possible to easily draw a bounding box of a gcode program and set a new origin. CNC machines can do a Z probe to easily put the bit right on top of the object (to be CNC'd).</br>
 Gcode loops are simulated (using a very simple WHILE DO syntax that must be annotated within the gcode) and can be run separately and (be) iterated at will.
 Soft and hard-resets can be issued and <i>Ctrl-D</i> makes a full stop (to machine state <i>Door</i>).
 This makes it easy to laser draw and cut without the need to (re)connect the device, so drawings and cuts have full (relative) machine precision.</br>   
 
 Grblhub is tested on several platforms - arm64/intel - and operating systems - Linux/macosx and two grbl v1.1 devices (a lasercutter and a CNC router)
 
 Information on grbl commands: https://github.com/gnea/grbl/blob/master/doc/markdown/commands.md
@@ -70,35 +71,35 @@
   --serialdevice /dev/<serial-tty-name>
                         serial device on linux (default: /dev/ttyUSB0 115200 baud)
   --status /dev/<terminal-tty-name>, -s /dev/<terminal-tty-name>
                         grbl status output (default: no output)
   -V, --version         show version number and exit
 
 [somedir]$ grblhud
-Opened serial port /dev/ttyUSB0 at 115200 bauds (bits/s)
 Initializing grbl...
-okok
-okok
+
+Grbl 1.1h ['$' for help]
 Status report every 0.1 seconds (WPos coordinates)
 Start command queue
-0|[Idle XYZ:-5.000,00.000,00.000 FS:0,0] grbl> help
+0|[Idle XYZ:-0.700,-0.400,-1.000 FS:0,0] grbl> help
 grblhud commands:
    (<Ctrl><D>) or FSTOP                              (FULL STOP, issue softreset to continue)
 
  - cls                                               (clear screen)
  - load <filename>                                   (load file to buffer)
  - run [LOOP] <(file/loop)name> [F<eed>] [S<peed>]   (run from buffer)
  - S+10, S+1, S-10, S-1                              (Speed up/down 10% 1%)
  - F+10, F+1, F-10, F-1                              (Feed up/down 10% 1%)
  - softstop                                          (purge command buffer, but let machine buffer run till empty)
  - softreset                                         (issue soft reset command)
  - hardreset                                         (hard reset: close/open serial port)
  - sleep                                             ($SLP command)
  - Zprobe                                            (lower head until 'probe' contact is made)
- - Zorigin <coord>                                   (make 'probe' point the new Z<coord>)
+ - origin [X<coord>][Y<coord>][Z<coord>]             (make current XYZ: [X<coord>][Y<coord>][Z<coord>] (shift work coordinates)
+ - Bbox [(X<min>,Y<min>):(X<max>,Y<max>)] [F<eed>]   (draw a bounding box with laser set to low )
  - Stoggle                                           (Spindle on/off, in 'Hold' state only)
 
 grbl commands:
  - $ (grbl help)
      $$ (view Grbl settings)
      $# (view # parameters)
      $G (view parser state)
@@ -110,9 +111,9 @@
      $X (kill alarm lock)
      $H (run homing cycle)
      ~ (cycle start)
      ! (feed hold)
      ? (current status)
      ctrl-x/command + x/softreset (reset Grbl)
 
-0|[Idle XYZ:-5.000,00.000,00.000 FS:0,0] grbl> exit
+0|[Idle XYZ:-0.700,-0.400,-1.000 FS:0,0] grbl> 
 ```
```

### Comparing `grblhud-1.1.0/grblhud/README.md` & `grblhud-1.2.0/grblhud/README.md`

 * *Files identical despite different names*

### Comparing `grblhud-1.1.0/grblhud/__main__.py` & `grblhud-1.2.0/grblhud/__main__.py`

 * *Files identical despite different names*

### Comparing `grblhud-1.1.0/grblhud/grblbuffer.py` & `grblhud-1.2.0/grblhud/grblbuffer.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,15 @@
         self.status_out = status_out
 
         # init
         self.grblinput = grblinput
         self.init_buffer()
         self.WCO = {"X" : 0.0, "Y" : 0.0, "Z" : 0.0}
         self.machinestatus = { "state" : "", "X" : 0.0, "Y" : 0.0, "Z" : 0.0, "Feed" : 0, "Speed" : 0 }
+        self.machinesettings = {}
 
         # status report
         self.status_plain = False
 
         # create and start query process
         self.grblstatus = threading.Thread(target=self.status, args=(.1,))
         self.grblstatus.start()
@@ -216,16 +217,19 @@
                             else:
                                 # add meaning to settings
                                 # $1=25
                                 setting = re.search("^\$[0-9]+=[0-9]+(\.[0-9]+)?",otds)
                                 if setting:
                                     setting = re.search("^\$[0-9]+",setting.group())
                                     if setting and int(setting.group()[1:]) in grbl_settings.keys():
+                                        value = re.search("=[0-9]+(\.[0-9]+)?",otds)
+                                        # save machine settings
+                                        if value:
+                                            self.machinesettings[setting.group()] = value.group()[1:]
 
-                                        #otds += (" " * ((25 > len(otds)) ? (25 - len(otds)) : 1 )) + (" + grbl_settings[int(setting.group()[1:])] + ")"
                                         otds += " " * ((25 - len(otds)) if len(otds) < 25 else 1)  + "(" + grbl_settings[int(setting.group()[1:])] + ")"
                             print(otds)
                 else:
                     # Note: ignore incomming pending ok's until counting is in balance.
                     # this is needed at startup when the device is in 'Hold' state
                     if self.serial_buffer_count:            # Delete the block character count corresponding to the last 'ok'
                         self.gcode_count += 1               # update g-code counter
```

### Comparing `grblhud-1.1.0/grblhud/grblhudloop.py` & `grblhud-1.2.0/grblhud/grblhudloop.py`

 * *Files 14% similar despite different names*

```diff
@@ -66,27 +66,30 @@
         resp_1 += " (" + grbl_alarm[int(alrm.group()[6:])] + ")"
     return resp + resp_1
 
 def wait_for_it(ser):
     """
     Wait for grbl response (if any)
     """
-    print(wait_on_line(ser), flush = True)
-
-    # fallback if response is delayed
-    # (note the read timeout set in machine_open())
-    while ser.in_waiting:
-        print(wait_on_line(ser), flush = True)
+    resp = wait_on_line(ser)
+    if resp:
+        print(resp, flush = True)
+    else:
+        # fallback if response is delayed
+        # (note the read timeout set in machine_open())
+        sleep(1)
+        while ser.in_waiting:
+            print(wait_on_line(ser), flush = True)
 
 def machine_init(ser):
     """
     Wakeup, report its wakeup message (if any)
     """
     # Wake up grbl
-    print ("Initializing grbl...")
+    print ("Initializing grbl...\n")
     ser.write("\r\n\r\n".encode())
 
     # Wait for grbl to initialize and print startup text (if any)
     wait_for_it(ser)
 
     # flush input (stray 'ok's may ruin strict block counting)
     ser.reset_input_buffer()
@@ -132,14 +135,15 @@
     """
 
     # buffered gcode file info ('load' and 'run' command)
     gcodeFile = { "name" : "", "bBox" : "", "buffer" : [], "WHILE" : {} }
 
     # init serial device
     ser = machine_open(args.serialdevice)
+
     # init device
     machine_init(ser)
 
     # terminal for status output (or None)
     terminal = args.status
 
     # create instance of Input class
@@ -197,15 +201,16 @@
                 print(" - S+10, S+1, S-10, S-1                              (Speed up/down 10% 1%)")
                 print(" - F+10, F+1, F-10, F-1                              (Feed up/down 10% 1%)")
                 print(" - softstop                                          (purge command buffer, but let machine buffer run till empty)")
                 print(" - softreset                                         (issue soft reset command)")
                 print(" - hardreset                                         (hard reset: close/open serial port)")
                 print(" - sleep                                             ($SLP command)")
                 print(" - Zprobe                                            (lower head until 'probe' contact is made)")
-                print(" - Zorigin <coord>                                   (make 'probe' point the new Z<coord>)")
+                print(" - origin [X<coord>][Y<coord>][Z<coord>]             (make current XYZ: [X<coord>][Y<coord>][Z<coord>] (shift work coordinates)")
+                print(" - Bbox [(X<min>,Y<min>):(X<max>,Y<max>)] [F<eed>]   (draw a bounding box with laser set to low )")
                 print(" - Stoggle                                           (Spindle on/off, in 'Hold' state only)")
                 print()
                 print("grbl commands:")
                 print(" - $ (grbl help)")
                 print("     $$ (view Grbl settings)")
                 print("     $# (view # parameters)")
                 print("     $G (view parser state)")
@@ -329,16 +334,16 @@
                         # do not do that gcodeFile["buffer"].append('; ' + gcodeFile["name"])
                         print("Loading file", gcodeFile["name"], "into memory buffer ...\n")
                         # for line in f:
                         for i, line in enumerate(f):
                             print("[" + str(i) + "]\t", line, end = '')
                             # get bbox if any
                             # find line like: '; Boundingbox: (X7.231380,Y8.677330) to (X78.658588,Y24.579710)'
-                            if line.find("Boundingbox") >= 0:
-                                gcodeFile["bBox"] = line[line.find("Boundingbox"):].strip()
+                            if line.find("Boundingbox:") >= 0:
+                                gcodeFile["bBox"] = line[line.find("Boundingbox:") + len("Boundingbox:"):].strip()
 
                             #    #100 = 1
                             #    WHILE [#100 LE 5] DO1
                             #    (Some G-Code Blocks Go Here to Be Repeated Each Loop)
                             #    #100 = #100 + 1 (Increase #100 by 1 each iteration of the loop)
                             #    END1
 
@@ -398,15 +403,15 @@
                                     break
 
                             gcodeFile["buffer"].append(line)
 
                         if not abort:
                             # give load summary
                             if len(gcodeFile["buffer"]) > 0:
-                                print("\nFile loaded", len(gcodeFile["buffer"]) - 1, "lines", gcodeFile["bBox"])
+                                print("\nFile loaded", len(gcodeFile["buffer"]) - 1, "lines, Bbox:", gcodeFile["bBox"])
                             if gcodeFile["WHILE"]:
                                 print("Detected the following loop(s):")
                                 for loop in gcodeFile['WHILE']:
                                     # {'pcstart': 13, 'pcend': 16, 'count': 2}
                                     print("    " + loop + ": ", gcodeFile['WHILE'][loop]['count'], " X [", gcodeFile['WHILE'][loop]['pcstart'],
                                           "]-[", gcodeFile['WHILE'][loop]['pcend'], "]", sep = '')
                                 print("    (Note that loops can be run separately using 'run LOOP <loopname> [F<feed>] [S<speed>]')\n")
@@ -460,15 +465,15 @@
                                     print("Entered invalid loop count:", setcount)
                                     continue
 
                             if count <= 0:
                                 print("Invalid loop count must be > 0:", count)
                                 continue
 
-                            print("Run loop '" + loopname + "'", count, "X,", FS_update + ",", gcodeFile["bBox"])
+                            print("Run loop '" + loopname + "'", count, "X,", FS_update + ", Bbox: ", gcodeFile["bBox"])
                             if not count_321():
                                 # abort
                                 continue
 
                             if FS_update:
                                 # make sure F and S are set correctly (before loop start)
                                 grblbuffer.put("M4 " + FS_update)
@@ -492,15 +497,15 @@
                         print("Cannot find loop with label '" + loopname + "', abort run!")
                     continue
 
                 filePath = line[line.find(' ') + 1:]
                 fileName = os.path.basename(filePath)
                 if fileName == gcodeFile["name"]:
                     with Grblbuffer.serialio_lock:
-                        print("Run", fileName, FS_update, gcodeFile["bBox"])
+                        print("Run", fileName, FS_update, "Bbox: ", gcodeFile["bBox"])
                         if not count_321():
                             # abort
                             continue
 
                         # unroll loop(s);
                         # get while loop info
                         for i, line in enumerate(gcodeFile["buffer"]):
@@ -630,61 +635,178 @@
                             # Set100%
                             grblbuffer.serial.write(b'\x90')
                     sleep(0.02)
                 continue
 
             # G38.n Straight Probe (https://linuxcnc.org/docs/html/gcode/g-code.html)
             if line.find("Zprobe") >= 0:
-                # direct command: soft reset
+                # Z-axis probe command
+                if "$32" in grblbuffer.machinesettings and int(grblbuffer.machinesettings["$32"]) == 1:
+                    print(f'Machine is in laser mode! (setting $32={grblbuffer.machinesettings["$32"]})')
+                    print("command aborted")
+                    continue
                 with Grblbuffer.serialio_lock:
                     Grblbuffer.STATUS_PAUZE = True
                     print("Lower head until 'probe' contact is made.")
                     print()
                     print("Make sure a (double) wire is conected to the 'probe' contacts on the machine board and one")
-                    print("wire - on the other end - is connected to a metal object you are setting origin Z0 to, while")
-                    print("the other is connected to the router bit (or a point that is in electric contact).")
+                    print("wire - on the other end - is connected to a metal object that is on top of the object you are")
+                    print("setting the origin Z0 to, while the other is connected to the router bit (or a point that is")
+                    print("in electric contact).")
                     print("You can make a test run - using this command - to check if the machine halts when you connect the wires by hand.")
-                    print("After a successfull probe command, 'Zorigin <offset>' can be used to make the probe point, the new Z origin.")
+                    print("After a successfull probe command, 'origin Z<metal_object_height>' can be used to make the probe point Z<metal_object_height>.")
                     print()
-                    sr = input("Issue Zprobe (enter <Ctrl><D> to abort) (yes/no)? ")
+                    sr = input("Issue probe (enter <Ctrl><D> to abort) (yes/no)? ")
                     if sr.find("yes") >= 0:
                         grblbuffer.serial.write("G38.2 Z-25 F24\n".encode())
                         print("\ngrbl> G38.2 Z-25 F24\n")
                     else:
                         print("command aborted")
                     Grblbuffer.STATUS_PAUZE = False
                 continue
 
             # G92 Coordinate System Offset (https://linuxcnc.org/docs/html/gcode/g-code.html)
-            if line.find("Zorigin") >= 0:
-                # Set Z<coord> to probe point
-                offset = re.search(" [0-9]+(\.[0-9]+)?",line)
-                if offset:
-                    coord = offset.group()[1:]
+            if line.find("origin") >= 0:
+                # get coordinates
+                Xoffset = re.search("X[0-9]+(\.[0-9]+)?",line)
+                Yoffset = re.search("Y[0-9]+(\.[0-9]+)?",line)
+                Zoffset = re.search("Z[0-9]+(\.[0-9]+)?",line)
+                if Xoffset:
+                    Xoffset = Xoffset.group()
+                else:
+                    Xoffset = ""
+                if Yoffset:
+                    Yoffset = Yoffset.group()
                 else:
-                    coord = "0"
+                    Yoffset = ""
+                if Zoffset:
+                    Zoffset = Zoffset.group()
+                else:
+                    Zoffset = ""
+
+                if not (Xoffset or Yoffset or Zoffset):
+                    print("At least one origin offset must be given!\nCommand aborted.")
+                    continue
+
                 with Grblbuffer.serialio_lock:
                     Grblbuffer.STATUS_PAUZE = True
-                    print("Set Z<coord> to probe point.")
+                    print("Set X<coord>Y<coord>Z<coord> to current point. (shift the Work Coordinate System)")
                     print()
                     print("For example: to make the top of a wood 'slab' to be CNC'd, the Z origin (Z0), a probe can be run (lowered)")
-                    print("that makes contact to a thin metal plate on top of it. If the plate thickness is 2.1 mm, command 'Zorigin 2.1'")
+                    print("that makes contact to a thin metal plate on top of it. If the plate thickness is 2.1 mm, command 'origin Z2.1'")
                     print("will make the probe point Z2.1, which is 2.1 mm above the wood 'slab'. After removing the thin metal plate,")
                     print("command 'G1 Z0 F24' (move to Z0 with low speed, to be carefull) will make the router bit just touch the top")
-                    print("of the 'slab'. Metal objects to be CNC'd can do with command 'Zorigin' (without an argument).")
+                    print("of the 'slab'. Metal objects to be CNC'd can do with command 'origin Z0' (with 0 offset).")
                     print()
                     print("Note that status report coordinates at the start of each grblhud commandline reflect the new coordinate offset")
                     print("because it uses Work Position (WPos).")
                     print()
-                    sr = input("Issue command 'Zorigin " + coord + "' (yes/no)? ")
+                    sr = input(f"Issue command 'origin {Xoffset}{Yoffset}{Zoffset}' (yes/no)? ")
                     if sr.find("yes") >= 0:
-                        grblbuffer.serial.write(("G92 Z" + coord + "\n").encode())
-                        print("\ngrbl> G92 Z" + coord + "\n")
+                        grblbuffer.serial.write((f"G92 {Xoffset}{Yoffset}{Zoffset}\n").encode())
+                        print(f"\ngrbl> G92 {Xoffset}{Yoffset}{Zoffset}\n")
+                    else:
+                        print("command aborted")
+                    Grblbuffer.STATUS_PAUZE = False
+                continue
+
+            # draw bounding box with low power laser setting
+            # gcodeFile = { "name" : "", "bBox" : "", "buffer" : [], "WHILE" : {} }
+            if line.find("Bbox") >= 0:
+            # if re.search("^run +[^<>:;,*|\"]+$", line):
+                # Bbox [(X<min>,Y<min>):(X<max>,Y<max>)] [F<eed>] (draw a bounding box of the current gcode file or bbox coordinates)")
+
+                if "$32" in grblbuffer.machinesettings and int(grblbuffer.machinesettings["$32"]) != 1:
+                    print(f'Machine is not in laser mode! (setting $32={grblbuffer.machinesettings["$32"]})')
+                    print("command aborted")
+                    continue
+
+                with Grblbuffer.serialio_lock:
+                    Grblbuffer.STATUS_PAUZE = True
+
+                    fltPatt = "[0-9]+(\.[0-9]+)?"
+
+                    minX = ""
+                    minY = ""
+                    maxX = ""
+                    maxY = ""
+
+                    fromFile = ""
+
+                    feed = re.search(" F[0-9]+",line)
+                    if feed:
+                        feed = feed.group()[1:]
+                        # remove F<nr> from line
+                        line = re.sub(" F[0-9]+", "", line)
+                    else:
+                        feed = "F1000"
+
+                    bboxcoords = re.search(f' \(X{fltPatt},Y{fltPatt}\):\(X{fltPatt},Y{fltPatt}\)',line)
+                    if bboxcoords:
+                        bboxcoords = bboxcoords.group()[1:]
+                        minXY = re.search(f'\(X{fltPatt},Y{fltPatt}\)', bboxcoords).group()
+                        minX = re.search(f'X{fltPatt}',minXY).group()[1:]
+                        minY = re.search(f',Y{fltPatt}',minXY).group()[2:]
+
+                        maxXY = re.search(f':\(X{fltPatt},Y{fltPatt}\)', bboxcoords).group()[1:]
+                        maxX = re.search(f'X{fltPatt}',maxXY).group()[1:]
+                        maxY = re.search(f',Y{fltPatt}',maxXY).group()[2:]
+                    elif len(line) > len("Bbox"):
+                        print("Error in Bbox argument, format is: (X<min>,Y<min>):(X<max>,Y<max>)")
+                    else:
+                        if gcodeFile["name"]:
+                            if gcodeFile["bBox"]:
+                                # bbox coordinates from the current gcode file
+                                # format: '(X7.231380,Y8.677330) to (X78.658588,Y24.579710)'
+                                minXY = re.search(f'^\(X{fltPatt},Y{fltPatt}\) ', gcodeFile["bBox"])
+                                if minXY:
+                                    minX = re.search(f'X{fltPatt}',minXY.group()).group()[1:]
+                                    minY = re.search(f',Y{fltPatt}',minXY.group()).group()[2:]
+
+                                maxXY = re.search(f' +\(X{fltPatt},Y{fltPatt}\)', gcodeFile["bBox"])
+                                if maxXY:
+                                    maxX = re.search(f'X{fltPatt}',maxXY.group()).group()[1:]
+                                    maxY = re.search(f',Y{fltPatt}',maxXY.group()).group()[2:]
+
+                                fromFile = f'- from file {gcodeFile["name"]} -'
+                            else:
+                                print("No Bbox info found in current gcode file.")
+                        else:
+                            print("Currently no gcode file is loaded. Use 'load <filename>' command to load a gcode file.")
+
+                    # check bbox
+                    if minX and minY and maxX and maxY:
+                        if float(minX) <= float(maxX) and float(minY) <= float(maxY):
+                            print(f'Draw bounding box: (X{minX},Y{minY}):(X{maxX},Y{maxY}) {fromFile} with laser intensity set to 1 and speed {feed}.')
+                            print("Make sure the work area is cleared and you wear glasses to be protected!")
+                            sr = input("Draw (yes/no)? ")
+                            if sr.find("yes") >= 0:
+                                grblbuffer.serial.write(("M5\n").encode())
+                                grblbuffer.serial.write((f'G1 X{minX} Y{minY} {feed}\n').encode())
+                                grblbuffer.serial.write(("M3\n").encode())
+                                grblbuffer.serial.write((f'G1 X{maxX} {feed} S1\n').encode())
+                                grblbuffer.serial.write((f'G1 Y{maxY} {feed} S1\n').encode())
+                                grblbuffer.serial.write((f'G1 X{minX} {feed} S1\n').encode())
+                                grblbuffer.serial.write((f'G1 Y{minY} {feed} S1\n').encode())
+                                grblbuffer.serial.write(("M5\n").encode())
+                                print("\ngrbl> M5")
+                                print("grbl> " + f'G1 X{minX} Y{minY} {feed}')
+                                print("grbl> M3")
+                                print("grbl> " + f'G1 X{maxX} {feed} S1')
+                                print("grbl> " + f'G1 Y{maxY} {feed} S1')
+                                print("grbl> " + f'G1 X{minX} {feed} S1')
+                                print("grbl> " + f'G1 Y{minY} {feed} S1')
+                                print("grbl> M5\n")
+                            else:
+                                print("command aborted")
+                        else:
+                            print(f'Bbox info error: (X{minX},Y{minY}):(X{maxX},Y{maxY})\nCommand aborted.')
                     else:
                         print("command aborted")
+
                     Grblbuffer.STATUS_PAUZE = False
                 continue
 
 
             # pauze status report
             Grblbuffer.STATUS_PAUZE = True
```

### Comparing `grblhud-1.1.0/grblhud/grblmessages.py` & `grblhud-1.2.0/grblhud/grblmessages.py`

 * *Files identical despite different names*

### Comparing `grblhud-1.1.0/grblhud/lineinput.py` & `grblhud-1.2.0/grblhud/lineinput.py`

 * *Files identical despite different names*

### Comparing `grblhud-1.1.0/grblhud/unblockedgetch.py` & `grblhud-1.2.0/grblhud/unblockedgetch.py`

 * *Files identical despite different names*

### Comparing `grblhud-1.1.0/pyproject.toml` & `grblhud-1.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `grblhud-1.1.0/PKG-INFO` & `grblhud-1.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grblhud
-Version: 1.1.0
+Version: 1.2.0
 Summary: grblhub: a command line tool to handle grbl code.
 Keywords: grbl,grblv1.1,hud,laser cutter,laser engraving
 Author-email: Johannes Noordanus <mailjohannes.mailnoordanus@gmail.com>
 Requires-Python: >=3.10.6
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: inputimeout >= 1.0.4
@@ -14,14 +14,15 @@
 # grblhub
 Grblhub is a command line based tool to handle grbl code.
 
 It features full control of the grbl v1.1 device and supports <i>realtime</i> direct commands and buffered streaming of commands and programs.</br>
 Grbl state is in line viewable, showing (all) machine states i.e. <i>Idle, Run, Hold, Jog, Alarm, Door, Check, Home, Sleep</i> in color. State also includes current buffered (pending) gcode blocks (and no scrolling <i>ok's</i>)</br>
 Grbl v1.1 error and Alarm code definitions are shown when they occur.
 Spindle and Feed settings can be updated realtime while gcode (G1) is running; gcode programs can be loaded and run with specific <i>Spindle</i> and <i>Feed</i> settings.</br>
+It is possible to easily draw a bounding box of a gcode program and set a new origin. CNC machines can do a Z probe to easily put the bit right on top of the object (to be CNC'd).</br>
 Gcode loops are simulated (using a very simple WHILE DO syntax that must be annotated within the gcode) and can be run separately and (be) iterated at will.
 Soft and hard-resets can be issued and <i>Ctrl-D</i> makes a full stop (to machine state <i>Door</i>).
 This makes it easy to laser draw and cut without the need to (re)connect the device, so drawings and cuts have full (relative) machine precision.</br>   
 
 Grblhub is tested on several platforms - arm64/intel - and operating systems - Linux/macosx and two grbl v1.1 devices (a lasercutter and a CNC router)
 
 Information on grbl commands: https://github.com/gnea/grbl/blob/master/doc/markdown/commands.md
@@ -83,35 +84,35 @@
   --serialdevice /dev/<serial-tty-name>
                         serial device on linux (default: /dev/ttyUSB0 115200 baud)
   --status /dev/<terminal-tty-name>, -s /dev/<terminal-tty-name>
                         grbl status output (default: no output)
   -V, --version         show version number and exit
 
 [somedir]$ grblhud
-Opened serial port /dev/ttyUSB0 at 115200 bauds (bits/s)
 Initializing grbl...
-okok
-okok
+
+Grbl 1.1h ['$' for help]
 Status report every 0.1 seconds (WPos coordinates)
 Start command queue
-0|[Idle XYZ:-5.000,00.000,00.000 FS:0,0] grbl> help
+0|[Idle XYZ:-0.700,-0.400,-1.000 FS:0,0] grbl> help
 grblhud commands:
    (<Ctrl><D>) or FSTOP                              (FULL STOP, issue softreset to continue)
 
  - cls                                               (clear screen)
  - load <filename>                                   (load file to buffer)
  - run [LOOP] <(file/loop)name> [F<eed>] [S<peed>]   (run from buffer)
  - S+10, S+1, S-10, S-1                              (Speed up/down 10% 1%)
  - F+10, F+1, F-10, F-1                              (Feed up/down 10% 1%)
  - softstop                                          (purge command buffer, but let machine buffer run till empty)
  - softreset                                         (issue soft reset command)
  - hardreset                                         (hard reset: close/open serial port)
  - sleep                                             ($SLP command)
  - Zprobe                                            (lower head until 'probe' contact is made)
- - Zorigin <coord>                                   (make 'probe' point the new Z<coord>)
+ - origin [X<coord>][Y<coord>][Z<coord>]             (make current XYZ: [X<coord>][Y<coord>][Z<coord>] (shift work coordinates)
+ - Bbox [(X<min>,Y<min>):(X<max>,Y<max>)] [F<eed>]   (draw a bounding box with laser set to low )
  - Stoggle                                           (Spindle on/off, in 'Hold' state only)
 
 grbl commands:
  - $ (grbl help)
      $$ (view Grbl settings)
      $# (view # parameters)
      $G (view parser state)
@@ -123,10 +124,10 @@
      $X (kill alarm lock)
      $H (run homing cycle)
      ~ (cycle start)
      ! (feed hold)
      ? (current status)
      ctrl-x/command + x/softreset (reset Grbl)
 
-0|[Idle XYZ:-5.000,00.000,00.000 FS:0,0] grbl> exit
+0|[Idle XYZ:-0.700,-0.400,-1.000 FS:0,0] grbl> 
 ```
```

