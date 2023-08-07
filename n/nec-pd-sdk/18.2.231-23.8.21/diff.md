# Comparing `tmp/nec_pd_sdk-18.2.231.tar.gz` & `tmp/nec_pd_sdk-23.8.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nec_pd_sdk-18.2.231.tar", last modified: Fri Feb 23 12:38:54 2018, max compression
+gzip compressed data, was "nec_pd_sdk-23.8.21.tar", last modified: Mon Aug  7 18:33:33 2023, max compression
```

## Comparing `nec_pd_sdk-18.2.231.tar` & `nec_pd_sdk-23.8.21.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2018-02-23 12:38:54.000000 nec_pd_sdk-18.2.231/
--rw-r--r--   0 pi        (1000) pi        (1000)       38 2018-02-23 12:38:54.000000 nec_pd_sdk-18.2.231/setup.cfg
--rw-r--r--   0 pi        (1000) pi        (1000)     1825 2018-02-23 12:28:49.000000 nec_pd_sdk-18.2.231/README.rst
--rw-r--r--   0 pi        (1000) pi        (1000)     2809 2018-02-23 12:38:54.000000 nec_pd_sdk-18.2.231/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)     3761 2018-02-23 12:32:29.000000 nec_pd_sdk-18.2.231/setup.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2018-02-23 12:38:54.000000 nec_pd_sdk-18.2.231/nec_pd_sdk/
--rw-r--r--   0 pi        (1000) pi        (1000)    31083 2018-02-22 13:05:56.000000 nec_pd_sdk-18.2.231/nec_pd_sdk/controls.txt
--rw-r--r--   0 pi        (1000) pi        (1000)    18713 2018-02-22 13:05:56.000000 nec_pd_sdk-18.2.231/nec_pd_sdk/constants.py
--rw-r--r--   0 pi        (1000) pi        (1000)   193013 2018-02-23 12:28:49.000000 nec_pd_sdk-18.2.231/nec_pd_sdk/nec_pd_sdk.py
--rw-r--r--   0 pi        (1000) pi        (1000)     7389 2018-02-23 12:28:49.000000 nec_pd_sdk-18.2.231/nec_pd_sdk/opcode_decoding.py
--rw-r--r--   0 pi        (1000) pi        (1000)       51 2018-02-23 12:28:49.000000 nec_pd_sdk-18.2.231/nec_pd_sdk/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     6579 2018-02-23 12:28:49.000000 nec_pd_sdk-18.2.231/nec_pd_sdk/protocol.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2018-02-23 12:38:54.000000 nec_pd_sdk-18.2.231/nec_pd_sdk.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)      337 2018-02-23 12:38:54.000000 nec_pd_sdk-18.2.231/nec_pd_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)     2809 2018-02-23 12:38:54.000000 nec_pd_sdk-18.2.231/nec_pd_sdk.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)       16 2018-02-23 12:38:54.000000 nec_pd_sdk-18.2.231/nec_pd_sdk.egg-info/requires.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       11 2018-02-23 12:38:54.000000 nec_pd_sdk-18.2.231/nec_pd_sdk.egg-info/top_level.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2018-02-23 12:38:54.000000 nec_pd_sdk-18.2.231/nec_pd_sdk.egg-info/dependency_links.txt
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-08-07 18:33:33.766510 nec_pd_sdk-23.8.21/
+-rw-r--r--   0 pi        (1000) pi        (1000)     2899 2023-08-07 18:33:33.766510 nec_pd_sdk-23.8.21/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)     1877 2023-08-02 18:32:42.000000 nec_pd_sdk-23.8.21/README.rst
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-08-07 18:33:33.766510 nec_pd_sdk-23.8.21/nec_pd_sdk/
+-rw-r--r--   0 pi        (1000) pi        (1000)      174 2023-08-02 18:29:38.000000 nec_pd_sdk-23.8.21/nec_pd_sdk/__init__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    23540 2023-08-02 18:29:38.000000 nec_pd_sdk-23.8.21/nec_pd_sdk/constants.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    37071 2023-08-02 18:29:38.000000 nec_pd_sdk-23.8.21/nec_pd_sdk/controls.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)   195298 2023-08-02 18:29:38.000000 nec_pd_sdk-23.8.21/nec_pd_sdk/nec_pd_sdk.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     7458 2023-08-02 18:29:38.000000 nec_pd_sdk-23.8.21/nec_pd_sdk/opcode_decoding.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     6640 2023-08-02 18:29:38.000000 nec_pd_sdk-23.8.21/nec_pd_sdk/protocol.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-08-07 18:33:33.766510 nec_pd_sdk-23.8.21/nec_pd_sdk.egg-info/
+-rw-r--r--   0 pi        (1000) pi        (1000)     2899 2023-08-07 18:33:33.000000 nec_pd_sdk-23.8.21/nec_pd_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      337 2023-08-07 18:33:33.000000 nec_pd_sdk-23.8.21/nec_pd_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-08-07 18:33:33.000000 nec_pd_sdk-23.8.21/nec_pd_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       16 2023-08-07 18:33:33.000000 nec_pd_sdk-23.8.21/nec_pd_sdk.egg-info/requires.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       11 2023-08-07 18:33:33.000000 nec_pd_sdk-23.8.21/nec_pd_sdk.egg-info/top_level.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       38 2023-08-07 18:33:33.766510 nec_pd_sdk-23.8.21/setup.cfg
+-rw-r--r--   0 pi        (1000) pi        (1000)     3783 2023-08-02 18:30:30.000000 nec_pd_sdk-23.8.21/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `nec_pd_sdk-18.2.231/README.rst` & `nec_pd_sdk-23.8.21/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,17 @@
 
 pip3 install nec_pd_sdk
 
 License
 --------------
 The MIT License
 
-Copyright (c) 2017-2018 NEC Display Solutions, Ltd.
+Copyright (c) 2023 Sharp NEC Display Solutions, Ltd.
+
+Copyright (c) 2017-20 NEC Display Solutions, Ltd.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `nec_pd_sdk-18.2.231/PKG-INFO` & `nec_pd_sdk-23.8.21/nec_pd_sdk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
-Name: nec_pd_sdk
-Version: 18.2.231
+Name: nec-pd-sdk
+Version: 23.8.21
 Summary: NEC PD SDK
 Home-page: https://github.com/necsoftware/necpdsdk
 Author: NEC Display Solutions, Ltd.
 Author-email: techsupport@necdisplay.com
 License: MIT
-Download-URL: https://github.com/NECDisplaySolutions/necpdsdk.git
+Download-URL: https://github.com/SharpNECDisplaySolutions/necpdsdk.git
 Description: NEC PD SDK
         =======================
         
         Python library interface for communicating via LAN or RS232 with NEC large-screen displays.  
         
         
         Documentation
@@ -27,15 +27,17 @@
         
         pip3 install nec_pd_sdk
         
         License
         --------------
         The MIT License
         
-        Copyright (c) 2017-2018 NEC Display Solutions, Ltd.
+        Copyright (c) 2023 Sharp NEC Display Solutions, Ltd.
+        
+        Copyright (c) 2017-20 NEC Display Solutions, Ltd.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
@@ -56,14 +58,14 @@
         Added scheduling functions
         Added CPU Temperature based cooling fan control
         Added "command_ip_address_read" function to read the IP address of the display
         Added OPCODE definitions for new COMPUTE MODULE FAN CONTROL and AUTO SHUTDOWN
         Added new IR remote keys definitions
         Added new OPCODES definitions and controls.txt
         
-Keywords: NEC pd sdk
+Keywords: Sharp NEC pd sdk
 Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `nec_pd_sdk-18.2.231/setup.py` & `nec_pd_sdk-23.8.21/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,52 +17,52 @@
 
 setup(
     name='nec_pd_sdk',
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='18.2.231',
+    version='23.8.21',
 
     description='NEC PD SDK',
     long_description=long_description,
 
     # The project's main homepage.
     url='https://github.com/necsoftware/necpdsdk',
-    download_url = 'https://github.com/NECDisplaySolutions/necpdsdk.git',
+    download_url = 'https://github.com/SharpNECDisplaySolutions/necpdsdk.git',
 
     # Author details
     author='NEC Display Solutions, Ltd.',
     author_email='techsupport@necdisplay.com',
 
     # Choose your license
     license='MIT',
 
     # See https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         # How mature is this project? Common values are
         #   3 - Alpha
         #   4 - Beta
         #   5 - Production/Stable
-        'Development Status :: 3 - Alpha',
+        'Development Status :: 5 - Production/Stable',
 
         # Indicate who your project is intended for
         'Intended Audience :: Developers',
         'Topic :: Software Development',
 
         # Pick your license as you wish (should match "license" above)
         'License :: OSI Approved :: MIT License',
 
         # Specify the Python versions you support here. In particular, ensure
         # that you indicate whether you support Python 2, Python 3 or both.
         'Programming Language :: Python :: 2.7',
     ],
 
     # What does your project relate to?
-    keywords='NEC pd sdk',
+    keywords='Sharp NEC pd sdk',
 
     # You can just specify the packages manually here if your project is
     # simple. Or you can use find_packages().
     #packages=find_packages(exclude=['contrib', 'docs', 'test*']),
     packages=["nec_pd_sdk"],
```

### Comparing `nec_pd_sdk-18.2.231/nec_pd_sdk/controls.txt` & `nec_pd_sdk-23.8.21/nec_pd_sdk/controls.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # NEC Large-screen opcode control definitions
-# Revision 20180118
-# Copyright (C) 2017-18 NEC Display Solutons, Ltd.
-# maintained by Will Hollingworth
+Revision: 230717
+# Copyright (C) 2017-18 NEC Display Solutions, Ltd.
+# Copyright (C) 2023 Sharp NEC Display Solutions, Ltd
+# written by Will Hollingworth <William.Hollingworth at sharpusa.com>
 # See LICENSE.rst for details.
 #
+
 0004,"Reset|Factory Reset",1,1,"Execute"
 0006,"Reset|Geometry Reset",1,1,"Execute"
 0008,"Reset|Color Reset",1,1,"Execute"
 000E,"Adjust|Clock",0
 0010,"Picture|Brightness",0
 0012,"Picture|Contrast",0,"Low","High"
 0014,"Picture|Color|Select Color Preset",1,9,"10000K",11,"User 1",2,"Native"
@@ -15,17 +17,17 @@
 0018,"Picture|Color|Gain|Green Gain",0
 001A,"Picture|Color|Gain|Blue Gain",0
 001E,"Adjust|Auto Setup",1,1,"Execute"
 0020,"Adjust|H Position",0,"Left","Right"
 0030,"Adjust|V Position",0,"Bottom","Top"
 003E,"Adjust|Clock Phase",0
 0054,"Picture|Color|Color Temp",0,"2600K","10000K"
-0060,"Input",1,1,"VGA",2,"RGB/HV",3,"DVI",4,"DVI2",5,"Video1",6,"Video2",7,"S-Video",10,"TV",12,"DVD/HD1",13,"Option",14,"DVD/HD2",15,"DisplayPort",16,"DisplayPort2",17,"HDMI",18,"HDMI2",19,"HDMI3(E series)",20,"USB",128,"DisplayPort3",130,"HDMI3",131,"HDMI4",132,"PRESET1",133,"PRESET2",134,"PRESET3",135,"Media Player",136,"Compute Module"
+0060,"Input",1,1,"VGA",2,"RGB/HV",3,"DVI",4,"DVI2",5,"Video1",6,"Video2",7,"S-Video",9,"TV (E series)",10,"TV",12,"DVD/HD1",13,"Option",14,"DVD/HD2",15,"DisplayPort",16,"DisplayPort2",17,"HDMI",18,"HDMI2",19,"HDMI3(E series)",20,"USB",128,"DisplayPort3",130,"HDMI3",131,"HDMI4",132,"PRESET1",133,"PRESET2",134,"PRESET3",135,"Media Player",136,"Compute Module",137,"USB-C"
 0062,"Audio|Audio Volume",0
-0068,"OSD|OSD Language",1,1,"English",2,"German",3,"French",4,"Spanish",5,"Japanese",6,"Italian",7,"Swedish",9,"Russian",14,"Chinese"
+0068,"OSD|OSD Language",1,1,"English",2,"German",3,"French",4,"Spanish",5,"Japanese",6,"Italian",7,"Swedish",9,"Russian",14,"Chinese",15,"Czech"
 008A,"Picture|Color|Saturation",0,"Pale","Saturated"
 008B,"TV Channel",1,1,"Up",2,"Down"
 008C,"Picture|Sharpness",0,"Soft","Sharp"
 008D,"Audio|Mute",1,0,"Unmute (Set only)",1,"Mute",2,"Unmute"
 008F,"Audio|Audio Treble",0
 0090,"Picture|Color|Tint",0,"Purplish","Greenish"
 0091,"Audio|Audio Bass",0
@@ -41,123 +43,167 @@
 00B0,"Settings",1,1,"Store Current",2,"Restore Factory"
 00B6,"Monitor Type (read only)",1,1,"CRT (SM)",2,"CRT (AG)",3,"TFT LCD"
 00D6,"Power Mode (read only)",1,1,"On",2,"Standby",3,"Suspend",4,"Off"
 00DA,"Scan Mode (VESA)",1,1,"Over-scan",2,"Under-scan"
 00DF,"VCP Version (read only)",0
 00E1,"Power Save",1,0,"Off",1,"On"
 00EF,"OSD|OSD Position",1,0,"Center",1,"Top-Left",2,"Top-Right",3,"Bottom-Left",4,"Bottom-Right"
+
 00FA,"Total Operating Time (30 min) (read only)",0
 00FB,"Key Lock",1,0,"Unlock",1,"Lock"
 00FC,"OSD|OSD Turn Off Delay",0,"","x5 sec"
 00FF,"Operating Time On (30 min) (read only)",0
-021A,"Picture|Picture Mode",1,1,"sRGB",3,"Hi-Bright",4,"Standard",5,"Cinema",6,"ISF-Day",7,"ISF-Night",8,"Custom 1",9,"Custom 2",11,"Ambient-1",12,"Ambient-2",13,"SVE-1",14,"SVE-2",15,"SVE-3",16,"SVE-4",17,"SVE-5"
+
+0212,"Picture|Color|6 Axis Saturation Red",0,"Pale","Saturated"
+0213,"Picture|Color|6 Axis Saturation Yellow",0,"Pale","Saturated"
+0214,"Picture|Color|6 Axis Saturation Green",0,"Pale","Saturated"
+0215,"Picture|Color|6 Axis Saturation Cyan",0,"Pale","Saturated"
+0216,"Picture|Color|6 Axis Saturation Blue",0,"Pale","Saturated"
+0217,"Picture|Color|6 Axis Saturation Magenta",0,"Pale","Saturated"
+
+021A,"Picture|Picture Mode",1,1,"sRGB",3,"Hi-Bright",4,"Standard",5,"Cinema",6,"ISF-Day",7,"ISF-Night",8,"Custom 1",9,"Custom 2",11,"Ambient-1",12,"Ambient-2",13,"SVE-1",14,"SVE-2",15,"SVE-3",16,"SVE-4",17,"SVE-5",23,"Dynamic",24,"Energy Saving",25,"Game",26,"HDR Dynamic",27,"HDR Video",28,"Retail",29,"Conferencing",30,"Transportation",31,"Native"
+
 021F,"Picture|Color|Color",0,"Pale","Saturated"
 0220,"Picture|Noise Reduction",0,"Off","High"
 0221,"Color System",1,1,"NTSC",2,"PAL",3,"SECAM",4,"Auto",5,"4.43NTSC",6,"PAL-60"
 0223,"Picture|Film Mode",1,1,"Off",2,"Auto"
 0225,"Scan Conversion",1,1,"Off (Interlace)",2,"Enable (IP On/Progressive)"
 0226,"Picture|Noise Reduction Level",0
+
 022B,"Off Timer (hours)",0,"Off",24,"24 Hours"
 022C,"Audio|MTS Audio",1,1,"Main",2,"Sub",3,"Main + Sub",4,"Stereo",5,"Mono",6,"Dual"
-022D,"Auto Brightness",1,0,"Off",1,"On"
+022D,"Auto Brightness",1,0,"Off",1,"On (Mode1)",2,"Mode2"
 022E,"Audio|Audio Input",1,1,"Audio 1",2,"Audio 2",3,"Audio 3",4,"HDMI",6,"TV/Option",7,"DisplayPort",8,"DisplayPort 2",10,"HDMI 2",11,"HDMI 3",12,"HDMI 4",13,"Media Player",14,"Compute Module"
+
 0231,"Reset|Sound Reset",1,1,"Execute"
+
 0234,"Audio|Surround Sound",1,1,"Off",2,"Low",3,"High"
+
 0238,"OSD|OSD H Position",0,"Left","Right"
 0239,"OSD|OSD V Position",0,"Down","Up"
-023D,"OSD|Information OSD",0,"Disable","Seconds"
+
+023D,"OSD|Information OSD",1,0,"Disable",1,"Enable",3,"3 Seconds",4,"4 Seconds",5,"5 Seconds",6,"6 Seconds",7,"7 Seconds",8,"8 Seconds",9,"9 Seconds",10,"10 Seconds"
 023E,"Monitor ID",0,"",""
 023F,"IR Control",1,1,"Normal",2,"Primary",3,"Secondary",4,"Lock (Off)"
+
 0240,"Input Detect",1,0,"First Detect",1,"Last Detect",2,"None",3,"Video Detect",4,"Custom Detect"
-0241,"OSD|OSD Rotation",1,0,"Normal",1,"Rotated"
+0241,"OSD|OSD Rotation",1,0,"Normal",1,"Rotated",2,"Auto"
+
 0250,"Adjust|H Resolution",0
 0251,"Adjust|V Resolution",0
-0268,"Picture|Gamma",1,1,"Native",4,"2.2",8,"2.4",7,"S Curve",5,"DICOM Sim",6,"Programmable",9,"Custom value",11,"sRGB",12,"LStar",13,"Programmable 2",14,"Programmable 3"
+
+0268,"Picture|Gamma",1,1,"Native",4,"2.2",8,"2.4",7,"S Curve",5,"DICOM Sim",6,"Programmable",9,"Custom value",11,"sRGB",12,"LStar",13,"Programmable 2",14,"Programmable 3",15,"Rec.1886",16,"HDR-Hybrid Log",17,"HDR-ST2084(PQ)"
+
 026C,"Adjust|Aspect|Zoom H Expansion",0,"100%","300%"
 026D,"Adjust|Aspect|Zoom V Expansion",0,"100%","300%"
 026F,"Adjust|Aspect|Zoom",0,"100%","300%"
-0270,"Adjust|Aspect|Aspect",1,1,"Normal",2,"Full",3,"Wide",4,"Zoom",5,"Trim",6,"Dynamic",7,"1:1"
+0270,"Adjust|Aspect|Aspect",1,1,"Normal",2,"Full",3,"Wide",4,"Zoom",5,"Trim",6,"Dynamic",7,"1:1",10,"Cinema",11,"Auto"
 0271,"PIP|PIP Size",1,1,"Small",2,"Middle",3,"Large"
 0272,"PIP|PIP Mode",1,1,"Off",2,"PIP",3,"POP",4,"Still",5,"PBP(1-3) / Side by Side (Aspect)",6,"Side by Side (Full)"
 0273,"PIP|PIP Input (Sub Input)",1,1,"VGA",2,"RGB/HV",3,"DVI",4,"DVI2",5,"Video1",6,"Video2",7,"S-Video",10,"TV",12,"DVD/HD1",13,"Option",14,"DVD/HD2",15,"DisplayPort",16,"DisplayPort2",17,"HDMI",18,"HDMI2",19,"HDMI3",20,"USB",128,"DisplayPort3"
 0274,"PIP|PIP H Position",0,"Left","Right"
 0275,"PIP|PIP V Position",0,"Bottom","Top"
 0276,"Still Capture",1,0,"Off",1,"Capture"
+
 0278,"Select Temperature Sensor",1,1,"Sensor #1",2,"Sensor #2",3,"Sensor #3"
 0279,"Read Temperature Sensor (read only)",0
 027A,"Fan|Fan Select",1,1,"Fan 1",2,"Fan 2",3,"Fan 3",4,"Fan 1+2",5,"Fan 1+2+3"
 027B,"Fan|Fan Status (read only)",1,0,"Off",1,"On",2,"Error"
-027D,"Fan|Fan Control",1,1,"Auto (No offset)",2,"Forced On",3,"Auto (offset -2)",4,"Auto (offset -4)",5,"Auto (offset -6)",6,"Auto (offset -8)",7,"Auto (offset -10)"
 
+027D,"Fan|Fan Control",1,1,"Auto (No offset)",2,"Forced On",3,"Auto (offset -2)",4,"Auto (offset -4)",5,"Auto (offset -6)",6,"Auto (offset -8)",7,"Auto (offset -10)"
 027E,"Backlight PWM Red (x100 read only)",0
 027F,"Backlight PWM Green (x100 read only)",0
 0280,"Backlight PWM Blue (x100 read only)",0
 
-028D,"Picture|Adaptive Contrast",1,1,"Off",2,"Low",3,"Middle",4,"High"
+028D,"Picture|Adaptive Contrast",1,1,"Off",2,"Low (On)",3,"Middle",4,"High"
 029A,"Standby Mode",1,1,"Standby",2,"ECO Standby"
 029E,"SCART Mode",1,0,"Off",1,"On"
+
 02B3,"SpectraView Engine|Luminance set",0
 02B4,"Current Luminance (read only)",0
 02B5,"Bright Sensor Read (read only)",0
+
 02B8,"OSD|OSD Transparency",1,1,"Off (Opaque)",2,"Type 1",3,"Type 2"
+
 02BE,"Power LED Indicator",1,1,"On",2,"Off"
+
 02C3,"Test Pattern|VT Mode",1,1,"Normal",2,"VT Mode"
+
 02C8,"SpectraView Engine|Test Pattern",1,1,"Off",2,"On"
+
 02CA,"CSC Gain",0
-02CB,"Reset|Menu Tree Reset",1,1,"Factory Reset WARNING!!!",2,"Reset Picture",3,"Reset Adjust",4,"Reset Audio",5,"Reset Schedule",6,"Reset PIP",7,"Reset OSD",8,"Reset Multi Display",9,"Reset Display Protection",10,"Reset Advanced Option",11,"Reset Advanced Option 2",12,"Reset External Control",13,"Reset Remote Control"
+02CB,"Reset|Menu Tree Reset",1,1,"Factory Reset WARNING!!!",2,"Reset Picture",3,"Reset Adjust",4,"Reset Audio",5,"Reset Schedule",6,"Reset PIP",7,"Reset OSD",8,"Reset Multi Display",9,"Reset Display Protection",10,"Reset Advanced Option",11,"Reset Advanced Option 2",12,"Reset External Control",13,"Reset Remote Control",14,"Reset Compute Module",15,"Reset Slot",16,"Reset Network",17,"Reset Protect",18,"Reset System",19,"Reset Input"
 02CC,"Adjust|Aspect|Zoom H Position",0,"Left Side","Right Side"
 02CD,"Adjust|Aspect|Zoom V Position",0,"Down Side","Up Side"
 02CE,"Adjust|Aspect|Base Zoom",1,1,"Off",2,"Custom",3,"16:9-Zoom",4,"14:9-Zoom",5,"Dynamic"
 02CF,"DVI Mode",1,1,"DVI-PC",2,"DVI-HD"
 02D0,"Tile Matrix|Tile Matrix # H Monitors",0,"",""
 02D1,"Tile Matrix|Tile Matrix # V Monitors",0,"",""
 02D2,"Tile Matrix|Tile Matrix Position",0,"Top Left","Bottom Right"
 02D3,"Tile Matrix|Tile Matrix Mode",1,1,"Disable (Off) and display frame",2,"Enable (On)",3,"Disable (Off) and hide frame"
 02D5,"Tile Matrix|Tile Matrix Tile Comp",1,1,"Disable (Off)",2,"Enable (On)"
 02D6,"Video (AV Input) Power Save",1,1,"Disable",2,"Enable"
 02D7,"Image Flip",1,1,"None",2,"H Flip",3,"V Flip",4,"180 Rotate"
 02D8,"Power On Delay",0,"Off","Seconds"
+
 02DA,"Adjust|Input Resolution",1,1,"Auto",2,"1024x768",3,"1280x768",4,"1360x768",5,"1366x768",6,"1400x1050",7,"1680x1050"
 02DB,"Screen Saver|Screen Saver Gamma",1,1,"Normal",2,"On"
 02DC,"Screen Saver|Screen Saver Brightness",1,1,"Normal",2,"Decrease Brightness"
 02DD,"Screen Saver|Screen Saver Motion",0,"Off","x10 Seconds"
 02DF,"Side Border Color",0,"Black","White"
+
 02E1,"Long Cable|Manual Sync Terminate",1,1,"Hi (2.2 kOhm)",2,"Lo (75 Ohm)"
+
 02E3,"Scan Mode",1,1,"Under-scan",2,"Over-scan",3,"Auto"
 02E4,"Reset|Advanced Option Reset",1,1,"Execute"
 02E5,"Enable Schedule (set only)",1,1,"Schedule #1",2,"Schedule #2",3,"Schedule #3",4,"Schedule #4",5,"Schedule #5",6,"Schedule #6",7,"Schedule #7"
 02E6,"Disable Schedule (set only)",1,1,"Schedule #1",2,"Schedule #2",3,"Schedule #3",4,"Schedule #4",5,"Schedule #5",6,"Schedule #6",7,"Schedule #7"
+
 02E8,"SpectraView Engine|Custom Gamma Value",0
+
 02EA,"OSD|Signal Information",1,1,"Off",2,"On"
+
 02EE,"Uniformity Correction Level",0,"Min","Max"
+
 02F0,"Long Cable|Comp DVI",1,1,"Mode 0",2,"Mode 1",3,"Mode 2",4,"Mode 3"
+02F1,"Picture|Color|6 Axis Brightness Red",0,"Low","High"
+02F2,"Picture|Color|6 Axis Brightness Yellow",0,"Low","High"
+02F3,"Picture|Color|6 Axis Brightness Green",0,"Low","High"
+02F4,"Picture|Color|6 Axis Brightness Cyan",0,"Low","High"
+02F5,"Picture|Color|6 Axis Brightness Blue",0,"Low","High"
+02F6,"Picture|Color|6 Axis Brightness Magenta",0,"Low","High"
+
 02F8,"Reset|Gamma Programmable Reset",1,1,"Execute"
 02F9,"Gamma Programmable LUT Size",1,1,"8 bit",2,"10 bit"
+
 1000,"ISF",1,1,"Off",2,"On"
 1001,"ISF Mode",1,1,"ISF-Day",2,"ISF-Night",17,"ISF-Day (not adjusted)",18,"ISF-Night (not adjusted)"
 1002,"ISF Data Copy",1,1,"Execute"
+
 1008,"PIP|Text Ticker Mode",1,1,"Off",2,"Horizontal",3,"Vertical"
 1009,"PIP|Text Ticker Position",0,"Top/Left","Bottom/Right"
 100A,"PIP|Text Ticker Size",0,"Narrow","Wide"
 100B,"PIP|Text Ticker Blend",0,"10%","100%"
 100C,"PIP|Text Ticker Detect",1,1,"Auto",2,"Off"
 100D,"PIP|Text Ticker Fade In",1,1,"On",2,"Off"
+
 1010,"Carbon Footprint (g) (read only)",0
 1011,"Carbon Footprint (kg) (read only)",0
+
 1026,"Carbon Usage (g) (read only)",0
 1027,"Carbon Usage (kg) (read only)",0
 1028,"Carbon Footprint Savings No Reset (g) (read only)",0
 1029,"Carbon Footprint Savings No Reset (kg) (read only)",0
 102A,"Carbon Usage No Reset (g) (read only)",0
 102B,"Carbon Usage No Reset (kg) (read only)",0
-102E,"Custom Detect Priority 1",1,1,"VGA",2,"RGB/HV",3,"DVI",4,"DVI2",5,"Video1",6,"Video2",7,"S-Video",10,"TV",12,"DVD/HD1",13,"Option",14,"DVD/HD2",15,"DisplayPort",16,"DisplayPort2",17,"HDMI",18,"HDMI2",20,"USB",128,"DisplayPort3",130,"HDMI3",131,"HDMI4",132,"PRESET1",133,"PRESET2",134,"PRESET3",135,"Media Player",136,"Compute Module"
-102F,"Custom Detect Priority 2",1,1,"VGA",2,"RGB/HV",3,"DVI",4,"DVI2",5,"Video1",6,"Video2",7,"S-Video",10,"TV",12,"DVD/HD1",13,"Option",14,"DVD/HD2",15,"DisplayPort",16,"DisplayPort2",17,"HDMI",18,"HDMI2",20,"USB",128,"DisplayPort3",130,"HDMI3",131,"HDMI4",132,"PRESET1",133,"PRESET2",134,"PRESET3",135,"Media Player",136,"Compute Module"
-1030,"Custom Detect Priority 3",1,1,"VGA",2,"RGB/HV",3,"DVI",4,"DVI2",5,"Video1",6,"Video2",7,"S-Video",10,"TV",12,"DVD/HD1",13,"Option",14,"DVD/HD2",15,"DisplayPort",16,"DisplayPort2",17,"HDMI",18,"HDMI2",20,"USB",128,"DisplayPort3",130,"HDMI3",131,"HDMI4",132,"PRESET1",133,"PRESET2",134,"PRESET3",135,"Media Player",136,"Compute Module"
-1031,"Custom Detect Priority 4",1,1,"VGA",2,"RGB/HV",3,"DVI",4,"DVI2",5,"Video1",6,"Video2",7,"S-Video",10,"TV",12,"DVD/HD1",13,"Option",14,"DVD/HD2",15,"DisplayPort",16,"DisplayPort2",17,"HDMI",18,"HDMI2",20,"USB",128,"DisplayPort3",130,"HDMI3",131,"HDMI4",132,"PRESET1",133,"PRESET2",134,"PRESET3",135,"Media Player",136,"Compute Module"
-1032,"Custom Detect Priority 5",1,1,"VGA",2,"RGB/HV",3,"DVI",4,"DVI2",5,"Video1",6,"Video2",7,"S-Video",10,"TV",12,"DVD/HD1",13,"Option",14,"DVD/HD2",15,"DisplayPort",16,"DisplayPort2",17,"HDMI",18,"HDMI2",20,"USB",128,"DisplayPort3",130,"HDMI3",131,"HDMI4",132,"PRESET1",133,"PRESET2",134,"PRESET3",135,"Media Player",136,"Compute Module"
+102E,"Custom Detect Priority 1",1,1,"VGA",2,"RGB/HV",3,"DVI",4,"DVI2",5,"Video1",6,"Video2",7,"S-Video",10,"TV",12,"DVD/HD1",13,"Option",14,"DVD/HD2",15,"DisplayPort",16,"DisplayPort2",17,"HDMI",18,"HDMI2",20,"USB",128,"DisplayPort3",130,"HDMI3",131,"HDMI4",132,"PRESET1",133,"PRESET2",134,"PRESET3",135,"Media Player",136,"Compute Module",137,"USB-C"
+102F,"Custom Detect Priority 2",1,1,"VGA",2,"RGB/HV",3,"DVI",4,"DVI2",5,"Video1",6,"Video2",7,"S-Video",10,"TV",12,"DVD/HD1",13,"Option",14,"DVD/HD2",15,"DisplayPort",16,"DisplayPort2",17,"HDMI",18,"HDMI2",20,"USB",128,"DisplayPort3",130,"HDMI3",131,"HDMI4",132,"PRESET1",133,"PRESET2",134,"PRESET3",135,"Media Player",136,"Compute Module",137,"USB-C"
+1030,"Custom Detect Priority 3",1,1,"VGA",2,"RGB/HV",3,"DVI",4,"DVI2",5,"Video1",6,"Video2",7,"S-Video",10,"TV",12,"DVD/HD1",13,"Option",14,"DVD/HD2",15,"DisplayPort",16,"DisplayPort2",17,"HDMI",18,"HDMI2",20,"USB",128,"DisplayPort3",130,"HDMI3",131,"HDMI4",132,"PRESET1",133,"PRESET2",134,"PRESET3",135,"Media Player",136,"Compute Module",137,"USB-C"
+1031,"Custom Detect Priority 4",1,1,"VGA",2,"RGB/HV",3,"DVI",4,"DVI2",5,"Video1",6,"Video2",7,"S-Video",10,"TV",12,"DVD/HD1",13,"Option",14,"DVD/HD2",15,"DisplayPort",16,"DisplayPort2",17,"HDMI",18,"HDMI2",20,"USB",128,"DisplayPort3",130,"HDMI3",131,"HDMI4",132,"PRESET1",133,"PRESET2",134,"PRESET3",135,"Media Player",136,"Compute Module",137,"USB-C"
+1032,"Custom Detect Priority 5",1,1,"VGA",2,"RGB/HV",3,"DVI",4,"DVI2",5,"Video1",6,"Video2",7,"S-Video",10,"TV",12,"DVD/HD1",13,"Option",14,"DVD/HD2",15,"DisplayPort",16,"DisplayPort2",17,"HDMI",18,"HDMI2",20,"USB",128,"DisplayPort3",130,"HDMI3",131,"HDMI4",132,"PRESET1",133,"PRESET2",134,"PRESET3",135,"Media Player",136,"Compute Module",137,"USB-C"
 1033,"Ambient Brightness Low",0,"Dark","Bright"
 1034,"Ambient Brightness High",0,"Dark","Bright"
 1035,"Screen Saver|Screen Saver Zoom",0
 1036,"Long Cable|Comp Manual Pole",0
 1037,"Long Cable|Comp Manual Peak",0
 1038,"Long Cable|Comp Manual Gain",0
 1039,"Long Cable|Comp Manual Offset",0
@@ -165,75 +211,88 @@
 103B,"Test Pattern|Test Pattern Green Level",0,"Dark","Bright"
 103C,"Test Pattern|Test Pattern Blue Level",0,"Dark","Bright"
 103D,"Long Cable|Comp Manual Equalize",1,1,"Off",2,"On"
 103E,"External Control|External Control",1,1,"RS232C",2,"LAN"
 103F,"Fan|Fan Speed",1,1,"High",2,"Low"
 1040,"HDMI Signal",1,1,"Expand",2,"Raw",3,"Auto"
 1041,"OPS|Option Slot Power",1,1,"Off (linked)",2,"On",3,"Auto"
+
 #1049,"EDID Switch",1,1,"Timing 1 (1280x768@60Hz)",2,"Timing 2 (1360x768@60Hz)",3,"Timing 3 (1366x768@60Hz)",4,"Timing 4 (1920x1080@60Hz)",5,"Timing 5"
 1049,"EDID Switch",1,1,"Timing 1",2,"Timing 2",3,"Timing 3",4,"Timing 4",5,"Timing 5"
+
 104A,"Tile Matrix|Tile Matrix Memory",1,1,"Common for all inputs",2,"Per Input"
-1050,"SpectraView Engine|Picture Mode",1,1,"Programmable 1",2,"Programmable 2",3,"Programmable 3",4,"Programmable 4",5,"Programmable 5"
-1051,"SpectraView Engine|Preset",1,1,"sRGB",2,"AdobeRGB",3,"DCI",4,"REC-Bt709",5,"High Bright",6,"Full",7,"DICOM",8,"Programmable 1",9,"Programmable 2",10,"Programmable 3",11,"Programmable 4",12,"Programmable 5",13,"eciRGB v2"
+
+1050,"SpectraView Engine|Picture Mode",1,1,"Programmable 1",2,"Programmable 2",3,"Programmable 3",4,"Programmable 4",5,"Programmable 5",6,"Programmable 6",7,"Programmable 7",8,"Programmable 8",9,"Programmable 9",10,"Programmable 10"
+1051,"SpectraView Engine|Preset",1,1,"sRGB",2,"AdobeRGB",3,"DCI",4,"REC-Bt709",5,"High Bright",6,"Full",7,"DICOM",8,"Programmable 1",9,"Programmable 2",10,"Programmable 3",11,"Programmable 4",12,"Programmable 5",13,"eciRGB v2",19,"Low Blue",20,"Rec.2100(HLG)",21,"Rec.2100(PQ)",22,"Signage",23,"TV Studio"
 1052,"SpectraView Engine|Target White Point CIE x (x1000)",0
 1053,"SpectraView Engine|Target White Point CIE y (x1000)",0
 1054,"SpectraView Engine|Black Level (x10)",0
 1055,"SpectraView Engine|Target Colorspace Red CIE x (x1000)",0
 1056,"SpectraView Engine|Target Colorspace Red CIE y (x1000)",0
 1057,"SpectraView Engine|Target Colorspace Green CIE x (x1000)",0
 1058,"SpectraView Engine|Target Colorspace Green CIE y (x1000)",0
 1059,"SpectraView Engine|Target Colorspace Blue CIE x (x1000)",0
 105A,"SpectraView Engine|Target Colorspace Blue CIE y (x1000)",0
 105B,"SpectraView Engine|Color Vision Emulation",1,1,"Off",2,"Type P",3,"Type D",4,"Type T",5,"Grayscale"
 105C,"SpectraView Engine|Metamerism",1,1,"Off",2,"On"
-1069,"SpectraView Engine|Print Preview (3D LUT)",1,1,"Off",2,"On"
+
+1064,"Blank Signal Skip",1,1,"Off",2,"On"
+
+1069,"SpectraView Engine|Print Preview (3D LUT)",1,1,"Off",2,"On",3,"Compare"
+
 106B,"SpectraView Engine|3D LUT/Prog Gamma Select",1,1,"Programmable 1",2,"Programmable 2",3,"Programmable 3",4,"Programmable 4",5,"Programmable 5"
+
 1070,"SpectraView Engine|Reset Picture Mode",1,1,"Reset"
 1071,"SpectraView Engine|Target Colorspace Reset",1,1,"Reset"
+
 1075,"Human Sensing|Human Sensing Mode",1,1,"Disable",2,"Auto Off",3,"Deep",4,"Custom"
 1076,"Human Sensing|Human Sensing Reading",0
 1077,"Human Sensing|Human Sensing Threshold",0
 1078,"Human Sensing|Human Sensing Start Time",0
+
 107E,"BNC Mode",1,1,"RGB Mode (Default)",2,"PComponent",3,"Video"
 107F,"Group ID",0
-1080,"Audio|PIP Audio",1,1,"Main",2,"Sub",3,"Window 1",4,"Window 2",5,"Window 3",6,"Window 4"
+1080,"Audio|PIP Audio",1,1,"Main",2,"Sub",3,"Window 1",4,"Window 2",5,"Window 3",6,"Window 4",20,"DisplayPort1",21,"DisplayPort2",22,"HDMI1",23,"HDMI2",24,"Option (Digital)",26,"Compute Module"
 1081,"Audio|Audio Line Out",1,1,"Fixed",2,"Variable"
 1082,"PIP|Keep PIP Mode",1,1,"Off",2,"On"
 1083,"PIP|PIP Aspect",1,1,"Normal",2,"Full",3,"Wide",4,"Zoom",5,"Trim",6,"Expand"
 1084,"Closed Caption",1,1,"Off",2,"CC1",3,"CC2",4,"CC3",5,"CC4",6,"TT1",7,"TT2",8,"TT3",9,"TT4"
 1085,"External Control|ID All Reply",1,1,"On",2,"Off"
 1086,"Input Change",1,1,"Normal",2,"Quick",3,"SuperQuick"
 1087,"Motion Compensation (120Hz)",1,1,"On",2,"Off"
 1088,"Edge Compensation (Mura)",1,1,"On",2,"Off"
 1089,"OSD|OSD Off",1,1,"On",2,"Off"
 108A,"Shutdown",1,1,"Off",2,"On"
 108B,"Option LAN Alert",1,1,"Off",2,"On"
 108C,"Edge Comp Type",1,1,"Type 1",2,"Type 2",3,"Type 3"
 108D,"Edge Comp Brightness",1,1,"10%",2,"20%",3,"30%",4,"40%"
 108E,"D-SUB Mode",1,1,"RGB",2,"Component"
+
 1095,"OSD|Display ID on OSD",1,0,"Off",1,"On"
 
 1097,"SpectraView Engine|Color Convert Status (read only)",1,0,"Done",1,"Busy"
-
 1098,"Expert Analog Video|ADC Offset Base Red",0,"Dark","Bright"
 1099,"Expert Analog Video|ADC Offset Base Green",0,"Dark","Bright"
 109A,"Expert Analog Video|ADC Offset Base Blue",0,"Dark","Bright"
 109B,"Expert Analog Video|ADC Offset Red",0,"Dark","Bright"
 109C,"Expert Analog Video|ADC Offset Green",0,"Dark","Bright"
 109D,"Expert Analog Video|ADC Offset Blue",0,"Dark","Bright"
 109E,"Expert Analog Video|ADC Gain Red",0,"Dark","Bright"
 109F,"Expert Analog Video|ADC Gain Green",0,"Dark","Bright"
 10A0,"Expert Analog Video|ADC Gain Blue",0,"Dark","Bright"
 10A1,"Digital Closed Caption",1,1,"Off",2,"Service1",3,"Service2",4,"Service3",5,"Service4",6,"Service5",7,"Service6"
+
 10AD,"Audio|Audio Volume Step",1,1,"Increment",2,"Decrement"
+
 10B0,"Audio|Option Slot Audio",1,1,"Analog",2,"Digital"
 10B1,"USB Power",1,1,"Auto",2,"On"
+10B2,"Audio|Sound mode",1,1,"Standard",2,"Movie",3,"Music",4,"News",5,"Custom"
+10B3,"Audio|Audio Language",1,2,"English",3,"French",10,"Spanish"
 
 10B5,"PIP|PBP Type",1,1,"PBP1=2 Windows",2,"PIP=2 Windows",3,"PIP=3 Windows / PBP1=3 Windows",4,"PBP2=3 Windows",5,"PBP3=3 Windows",6,"PBP1=4 Windows"
-
 10B6,"Screen Mute",1,1,"On",2,"Off"
 10B7,"Auto Adjust",1,1,"Off",2,"On"
 10B8,"OSD|OSD Flip",1,1,"Off",2,"On"
 10B9,"PIP|PIP Size (Variable)",0,"Small","Large"
 10BA,"Memo Display",1,1,"On",2,"Off"
 10BC,"Power On Delay - Link to ID",1,1,"Off",2,"On"
 10BE,"DDCI",1,1,"Disable",2,"Enable"
@@ -247,137 +306,132 @@
 10C6,"Human Sensing|Human Sensing Backlight",0,"Dark","Bright"
 10C7,"Human Sensing|Human Sensing Volume",0
 10C8,"Room Light Sensing",1,1,"Off",2,"Mode 1",3,"Mode 2"
 10C9,"Room Ambient Brightness Max",0
 10CA,"Audio|Audio Delay SW",1,1,"Off",2,"On"
 10CB,"Audio|Audio Delay",0,"Short","Long"
 10CB,"Model ID",0
-10CE,"Input Change Super Input 1",1,0,"-",1,"VGA",2,"RGB/HV",3,"DVI",4,"DVI2",5,"Video1",6,"Video2",7,"S-Video",10,"TV",12,"DVD/HD1",13,"Option",14,"DVD/HD2",15,"DisplayPort",16,"DisplayPort2",17,"HDMI",18,"HDMI2",20,"USB",128,"DisplayPort3",130,"HDMI3",131,"HDMI4",132,"PRESET1",133,"PRESET2",134,"PRESET3",135,"Media Player",136,"Compute Module"
-10CF,"Input Change Super Input 2",1,0,"-",1,"VGA",2,"RGB/HV",3,"DVI",4,"DVI2",5,"Video1",6,"Video2",7,"S-Video",10,"TV",12,"DVD/HD1",13,"Option",14,"DVD/HD2",15,"DisplayPort",16,"DisplayPort2",17,"HDMI",18,"HDMI2",20,"USB",128,"DisplayPort3",130,"HDMI3",131,"HDMI4",132,"PRESET1",133,"PRESET2",134,"PRESET3",135,"Media Player",136,"Compute Module"
-10D0,"Human Sensing|Human Sensing Input",1,1,"VGA",2,"RGB/HV",3,"DVI",4,"DVI2",5,"Video1",6,"Video2",7,"S-Video",10,"TV",12,"DVD/HD1",13,"Option",14,"DVD/HD2",15,"DisplayPort",16,"DisplayPort2",17,"HDMI",18,"HDMI2",20,"USB",128,"DisplayPort3",130,"HDMI3",131,"HDMI4",132,"PRESET1",133,"PRESET2",134,"PRESET3",135,"Media Player",136,"Compute Module"
+10CE,"Input Change Super Input 1",1,0,"-",1,"VGA",2,"RGB/HV",3,"DVI",4,"DVI2",5,"Video1",6,"Video2",7,"S-Video",10,"TV",12,"DVD/HD1",13,"Option",14,"DVD/HD2",15,"DisplayPort",16,"DisplayPort2",17,"HDMI",18,"HDMI2",20,"USB",128,"DisplayPort3",130,"HDMI3",131,"HDMI4",132,"PRESET1",133,"PRESET2",134,"PRESET3",135,"Media Player",136,"Compute Module",137,"USB-C"
+10CF,"Input Change Super Input 2",1,0,"-",1,"VGA",2,"RGB/HV",3,"DVI",4,"DVI2",5,"Video1",6,"Video2",7,"S-Video",10,"TV",12,"DVD/HD1",13,"Option",14,"DVD/HD2",15,"DisplayPort",16,"DisplayPort2",17,"HDMI",18,"HDMI2",20,"USB",128,"DisplayPort3",130,"HDMI3",131,"HDMI4",132,"PRESET1",133,"PRESET2",134,"PRESET3",135,"Media Player",136,"Compute Module",137,"USB-C"
+10D0,"Human Sensing|Human Sensing Input",1,1,"VGA",2,"RGB/HV",3,"DVI",4,"DVI2",5,"Video1",6,"Video2",7,"S-Video",10,"TV",12,"DVD/HD1",13,"Option",14,"DVD/HD2",15,"DisplayPort",16,"DisplayPort2",17,"HDMI",18,"HDMI2",20,"USB",128,"DisplayPort3",130,"HDMI3",131,"HDMI4",132,"PRESET1",133,"PRESET2",134,"PRESET3",135,"Media Player",136,"Compute Module",137,"USB-C"
 10D2,"Power Save Timer",1,1,"Off",2,"On (Auto Standby)"
-10D3,"LAN Power",1,1,"Off",2,"On"
-10D4,"IR Lock|IR Lock Settings Mode Select",1,1,"Unlock",2,"Lock All",3,"Custom Lock"
-10D5,"IR Lock|IR Lock Settings Power",1,1,"Unlock",2,"Lock"
-10D6,"IR Lock|IR Lock Settings Volume",1,1,"Unlock",2,"Lock"
-10D7,"IR Lock|IR Lock Settings Min Volume",0
-10D8,"IR Lock|IR Lock Settings Max Volume",0
-10D9,"IR Lock|IR Lock Settings Input",1,1,"Unlock",2,"Lock"
-10DA,"IR Lock|IR Lock Settings Unlock Select 1",1,0,"-",1,"VGA",2,"RGB/HV",3,"DVI",4,"DVI2",5,"Video1",6,"Video2",7,"S-Video",10,"TV",12,"DVD/HD1",13,"Option",14,"DVD/HD2",15,"DisplayPort",16,"DisplayPort2",17,"HDMI",18,"HDMI2",20,"USB",128,"DisplayPort3",130,"HDMI3",131,"HDMI4",132,"PRESET1",133,"PRESET2",134,"PRESET3",135,"Media Player",136,"Compute Module"
-10DB,"IR Lock|IR Lock Settings Unlock Select 2",1,0,"-",1,"VGA",2,"RGB/HV",3,"DVI",4,"DVI2",5,"Video1",6,"Video2",7,"S-Video",10,"TV",12,"DVD/HD1",13,"Option",14,"DVD/HD2",15,"DisplayPort",16,"DisplayPort2",17,"HDMI",18,"HDMI2",20,"USB",128,"DisplayPort3",130,"HDMI3",131,"HDMI4",132,"PRESET1",133,"PRESET2",134,"PRESET3",135,"Media Player",136,"Compute Module"
-10DC,"IR Lock|IR Lock Settings Unlock Select 3",1,0,"-",1,"VGA",2,"RGB/HV",3,"DVI",4,"DVI2",5,"Video1",6,"Video2",7,"S-Video",10,"TV",12,"DVD/HD1",13,"Option",14,"DVD/HD2",15,"DisplayPort",16,"DisplayPort2",17,"HDMI",18,"HDMI2",20,"USB",128,"DisplayPort3",130,"HDMI3",131,"HDMI4",132,"PRESET1",133,"PRESET2",134,"PRESET3",135,"Media Player",136,"Compute Module"
+10D3,"LAN|LAN Power",1,1,"Off",2,"On"
+10D4,"Control|IR Lock Settings|IR Lock Mode Select",1,1,"Unlock",2,"Lock All",3,"Custom Lock"
+10D5,"Control|IR Lock Settings|IR Lock Power",1,1,"Unlock",2,"Lock"
+10D6,"Control|IR Lock Settings|IR Lock Volume",1,1,"Unlock",2,"Lock"
+10D7,"Control|IR Lock Settings|IR Lock Min Volume",0
+10D8,"Control|IR Lock Settings|IR Lock Max Volume",0
+10D9,"Control|IR Lock Settings|IR Lock Input",1,1,"Unlock",2,"Lock"
+10DA,"Control|IR Lock Settings|IR Lock Unlock Select 1",1,0,"-",1,"VGA",2,"RGB/HV",3,"DVI",4,"DVI2",5,"Video1",6,"Video2",7,"S-Video",10,"TV",12,"DVD/HD1",13,"Option",14,"DVD/HD2",15,"DisplayPort",16,"DisplayPort2",17,"HDMI",18,"HDMI2",20,"USB",128,"DisplayPort3",130,"HDMI3",131,"HDMI4",132,"PRESET1",133,"PRESET2",134,"PRESET3",135,"Media Player",136,"Compute Module",137,"USB-C"
+10DB,"Control|IR Lock Settings|IR Lock Unlock Select 2",1,0,"-",1,"VGA",2,"RGB/HV",3,"DVI",4,"DVI2",5,"Video1",6,"Video2",7,"S-Video",10,"TV",12,"DVD/HD1",13,"Option",14,"DVD/HD2",15,"DisplayPort",16,"DisplayPort2",17,"HDMI",18,"HDMI2",20,"USB",128,"DisplayPort3",130,"HDMI3",131,"HDMI4",132,"PRESET1",133,"PRESET2",134,"PRESET3",135,"Media Player",136,"Compute Module",137,"USB-C"
+10DC,"Control|IR Lock Settings|IR Lock Unlock Select 3",1,0,"-",1,"VGA",2,"RGB/HV",3,"DVI",4,"DVI2",5,"Video1",6,"Video2",7,"S-Video",10,"TV",12,"DVD/HD1",13,"Option",14,"DVD/HD2",15,"DisplayPort",16,"DisplayPort2",17,"HDMI",18,"HDMI2",20,"USB",128,"DisplayPort3",130,"HDMI3",131,"HDMI4",132,"PRESET1",133,"PRESET2",134,"PRESET3",135,"Media Player",136,"Compute Module",137,"USB-C"
 10DD,"Human Sensing|Human Sensing Backlight On/Off",1,1,"Off",2,"On"
 10DE,"Human Sensing|Human Sensing Volume On/Off",1,1,"Off",2,"On"
 10DF,"Human Sensing|Human Sensing Input On/Off",1,1,"Off",2,"On"
 10E0,"Fan|Fan Control Sensor 1 Set Temperature",0
 10E1,"Fan|Fan Control Sensor 1 Temperature from max",0
 10E2,"Fan|Fan Control Sensor 2 Set Temperature",0
 10E3,"Fan|Fan Control Sensor 2 Temperature from max",0
 10E4,"Fan|Fan Control Sensor 3 Set Temperature",0
 10E5,"Fan|Fan Control Sensor 3 Temperature from max",0
+
 10EA,"Video Loop Out Setting",1,1,"On",2,"Off"
 10EC,"Intelligent Wireless Data",1,1,"Off",2,"On"
 10EE,"RF-Tag Destination ID (read only)",1,0,"World Wide",1,"North America",2,"Europe",3,"China",4,"Japan",5,"Taiwan"
 10EF,"Bowling Mode",1,1,"Off",2,"On"
 10F0,"Human Sensing|Human Sensor attachment status (read only)",1,1,"Not installed",2,"Installed"
 10F1,"DisplayPort Terminal Select",1,1,"DisplayPort 1",2,"DisplayPort 2",3,"DisplayPort3"
-10F2,"DisplayPort Terminal Type",1,1,"1.1a",2,"1.2"
+10F2,"DisplayPort Terminal Type",1,1,"1.1a",2,"1.2",3,"1.4"
 10F5,"Extended Power Save",1,1,"Disable",2,"Auto Power Save",3,"Auto Standby"
 10F6,"Auto Power Save Time (sec x5)",0
 10F7,"Auto Standby Time (sec x5)",0
-
-
 10F8,"Panel|Native White CIE x (x1000 read only)",0
 10F9,"Panel|Native White CIE y (x1000 read only)",0
 10FA,"Panel|Native Red CIE x (x1000 read only)",0
 10FB,"Panel|Native Red CIE y (x1000 read only)",0
 10FC,"Panel|Native Green CIE x (x1000 read only)",0
 10FD,"Panel|Native Green CIE y (x1000 read only)",0
 10FE,"Panel|Native Blue CIE x (x1000 read only)",0
 10FF,"Panel|Native Blue CIE y (x1000 read only)",0
 1100,"Panel|Native Max Brightness (read only)",0
-
 1101,"Tile Matrix|Frame Comp Mode",1,1,"None",2,"Auto",3,"Manual"
 1102,"Tile Matrix|Frame Comp Auto Value",1,200,"2.0",150,"1.5",100,"1.0",50,"0.5"
 1103,"Tile Matrix|Frame Comp Manual Value",1,25,"0.25",50,"0.50",75,"0.75",100,"1.00",125,"1.25",150,"1.50",175,"1.75",200,"2.00"
 1104,"Tile Matrix|V Scan Reverse Mode",1,1,"None",2,"Auto",3,"Manual"
 1105,"Tile Matrix|V Scan Reverse Manual",1,1,"Non Reverse",2,"Reverse"
+1106,"Input (Alt)",1,3,"DVI1",4,"DVI2",13,"Option",15,"DisplayPort",16,"DisplayPort2",17,"HDMI1",18,"HDMI2",130,"HDMI3",131,"HDMI4",132,"PRESET1",133,"PRESET2",134,"PRESET3",135,"Media Player",136,"Compute Module",137,"USB-C"
 
-1106,"Input (Alt)",1,3,"DVI1",4,"DVI2",13,"Option",15,"DisplayPort",16,"DisplayPort2",17,"HDMI1",18,"HDMI2",130,"HDMI3",131,"HDMI4",132,"PRESET1",133,"PRESET2",134,"PRESET3",135,"Media Player",136,"Compute Module"
 1109,"UHD Upscaling",1,1,"Off",2,"Low",3,"Mid",4,"High"
+
 110B,"PIP|Active Window",1,1,"Window 1",2,"Window 2",3,"Window 3",4,"Window 4"
-110D,"PIP|Active Frame",1,1,"Off",2,"On"
-110E,"PIP|Input Select Window 1",1,1,"VGA",2,"RGB/HV",3,"DVI",4,"DVI2",5,"Video1",6,"Video2",7,"S-Video",10,"TV",12,"DVD/HD1",13,"Option",14,"DVD/HD2",15,"DisplayPort",16,"DisplayPort2",17,"HDMI",18,"HDMI2",20,"USB",128,"DisplayPort3",130,"HDMI3",131,"HDMI4",132,"PRESET1",133,"PRESET2",134,"PRESET3",135,"Media Player",136,"Compute Module"
-110F,"PIP|Input Select Window 2",1,1,"VGA",2,"RGB/HV",3,"DVI",4,"DVI2",5,"Video1",6,"Video2",7,"S-Video",10,"TV",12,"DVD/HD1",13,"Option",14,"DVD/HD2",15,"DisplayPort",16,"DisplayPort2",17,"HDMI",18,"HDMI2",20,"USB",128,"DisplayPort3",130,"HDMI3",131,"HDMI4",132,"PRESET1",133,"PRESET2",134,"PRESET3",135,"Media Player",136,"Compute Module"
-1110,"PIP|Input Select Window 3",1,1,"VGA",2,"RGB/HV",3,"DVI",4,"DVI2",5,"Video1",6,"Video2",7,"S-Video",10,"TV",12,"DVD/HD1",13,"Option",14,"DVD/HD2",15,"DisplayPort",16,"DisplayPort2",17,"HDMI",18,"HDMI2",20,"USB",128,"DisplayPort3",130,"HDMI3",131,"HDMI4",132,"PRESET1",133,"PRESET2",134,"PRESET3",135,"Media Player",136,"Compute Module"
-1111,"PIP|Input Select Window 4",1,1,"VGA",2,"RGB/HV",3,"DVI",4,"DVI2",5,"Video1",6,"Video2",7,"S-Video",10,"TV",12,"DVD/HD1",13,"Option",14,"DVD/HD2",15,"DisplayPort",16,"DisplayPort2",17,"HDMI",18,"HDMI2",20,"USB",128,"DisplayPort3",130,"HDMI3",131,"HDMI4",132,"PRESET1",133,"PRESET2",134,"PRESET3",135,"Media Player",136,"Compute Module"
-1112,"PIP|Pivot Window 1",1,1,"Off",2,"Rotate 90"
-1113,"PIP|Pivot Window 2",1,1,"Off",2,"Rotate 90"
-1114,"PIP|Pivot Window 3",1,1,"Off",2,"Rotate 90"
-1115,"PIP|Pivot Window 4",1,1,"Off",2,"Rotate 90"
-1116,"PIP|Pivot All Windows",1,1,"Off",2,"Rotate 90"
 
+110D,"PIP|Active Frame",1,1,"Off",2,"On"
+110E,"PIP|Input Select Window 1",1,1,"VGA",2,"RGB/HV",3,"DVI",4,"DVI2",5,"Video1",6,"Video2",7,"S-Video",10,"TV",12,"DVD/HD1",13,"Option",14,"DVD/HD2",15,"DisplayPort",16,"DisplayPort2",17,"HDMI",18,"HDMI2",20,"USB",128,"DisplayPort3",130,"HDMI3",131,"HDMI4",132,"PRESET1",133,"PRESET2",134,"PRESET3",135,"Media Player",136,"Compute Module",137,"USB-C"
+110F,"PIP|Input Select Window 2",1,1,"VGA",2,"RGB/HV",3,"DVI",4,"DVI2",5,"Video1",6,"Video2",7,"S-Video",10,"TV",12,"DVD/HD1",13,"Option",14,"DVD/HD2",15,"DisplayPort",16,"DisplayPort2",17,"HDMI",18,"HDMI2",20,"USB",128,"DisplayPort3",130,"HDMI3",131,"HDMI4",132,"PRESET1",133,"PRESET2",134,"PRESET3",135,"Media Player",136,"Compute Module",137,"USB-C"
+1110,"PIP|Input Select Window 3",1,1,"VGA",2,"RGB/HV",3,"DVI",4,"DVI2",5,"Video1",6,"Video2",7,"S-Video",10,"TV",12,"DVD/HD1",13,"Option",14,"DVD/HD2",15,"DisplayPort",16,"DisplayPort2",17,"HDMI",18,"HDMI2",20,"USB",128,"DisplayPort3",130,"HDMI3",131,"HDMI4",132,"PRESET1",133,"PRESET2",134,"PRESET3",135,"Media Player",136,"Compute Module",137,"USB-C"
+1111,"PIP|Input Select Window 4",1,1,"VGA",2,"RGB/HV",3,"DVI",4,"DVI2",5,"Video1",6,"Video2",7,"S-Video",10,"TV",12,"DVD/HD1",13,"Option",14,"DVD/HD2",15,"DisplayPort",16,"DisplayPort2",17,"HDMI",18,"HDMI2",20,"USB",128,"DisplayPort3",130,"HDMI3",131,"HDMI4",132,"PRESET1",133,"PRESET2",134,"PRESET3",135,"Media Player",136,"Compute Module",137,"USB-C"
+1112,"PIP|Pivot Window 1",1,1,"Off",2,"Rotate 90",4,"Rotate 270"
+1113,"PIP|Pivot Window 2",1,1,"Off",2,"Rotate 90",4,"Rotate 270"
+1114,"PIP|Pivot Window 3",1,1,"Off",2,"Rotate 90",4,"Rotate 270"
+1115,"PIP|Pivot Window 4",1,1,"Off",2,"Rotate 90",4,"Rotate 270"
+1116,"PIP|Pivot All Windows",1,1,"Off",2,"Rotate 90",4,"Rotate 270"
 1117,"OSD|Communications Information",1,1,"Off",2,"On"
-
 1118,"HDMI/DVI Select",1,1,"HDMI",2,"DVI",3,"Combo HDMI/DVI"
-1119,"DisplayPortBit Rate",1,1,"RBR",2,"HBR",3,"HBR2"
+1119,"DisplayPortBit Rate",1,1,"RBR",2,"HBR",3,"HBR2",4,"HBR3"
 111A,"Long Cable|Comp DVI2",1,1,"Mode 0",2,"Mode 1",3,"Mode 2",4,"Mode 3"
 111B,"Long Cable|Comp HDMI1",1,1,"Mode 0",2,"Mode 1",3,"Mode 2",4,"Mode 3"
 111C,"Long Cable|Comp HDMI2",1,1,"Mode 0",2,"Mode 1",3,"Mode 2",4,"Mode 3"
 111D,"Long Cable|Comp HDMI3",1,1,"Mode 0",2,"Mode 1",3,"Mode 2",4,"Mode 3"
 111E,"Long Cable|Comp HDMI4",1,1,"Mode 0",2,"Mode 1",3,"Mode 2",4,"Mode 3"
-
 111F,"Input Configuration|Preset 1 Mode",1,1,"Off",2,"Left & Right",3,"Top & Bottom"
 1120,"Input Configuration|Preset 2 Mode",1,1,"Off",2,"Left & Right",3,"Top & Bottom"
 1121,"Input Configuration|Preset 3 Mode",1,1,"Off",2,"Left & Right",3,"Top & Bottom"
-1122,"Input Configuration|Top Left",1,1,"VGA",2,"RGB/HV",3,"DVI",4,"DVI2",5,"Video1",6,"Video2",7,"S-Video",10,"TV",12,"DVD/HD1",13,"Option",14,"DVD/HD2",15,"DisplayPort",16,"DisplayPort2",17,"HDMI",18,"HDMI2",20,"USB",128,"DisplayPort3",130,"HDMI3",131,"HDMI4",132,"PRESET1",133,"PRESET2",134,"PRESET3",135,"Media Player",136,"Compute Module"
-1123,"Input Configuration|Top Right",1,1,"VGA",2,"RGB/HV",3,"DVI",4,"DVI2",5,"Video1",6,"Video2",7,"S-Video",10,"TV",12,"DVD/HD1",13,"Option",14,"DVD/HD2",15,"DisplayPort",16,"DisplayPort2",17,"HDMI",18,"HDMI2",20,"USB",128,"DisplayPort3",130,"HDMI3",131,"HDMI4",132,"PRESET1",133,"PRESET2",134,"PRESET3",135,"Media Player",136,"Compute Module"
-1124,"Input Configuration|Bottom Left",1,1,"VGA",2,"RGB/HV",3,"DVI",4,"DVI2",5,"Video1",6,"Video2",7,"S-Video",10,"TV",12,"DVD/HD1",13,"Option",14,"DVD/HD2",15,"DisplayPort",16,"DisplayPort2",17,"HDMI",18,"HDMI2",20,"USB",128,"DisplayPort3",130,"HDMI3",131,"HDMI4",132,"PRESET1",133,"PRESET2",134,"PRESET3",135,"Media Player",136,"Compute Module"
-1125,"Input Configuration|Bottom Right",1,1,"VGA",2,"RGB/HV",3,"DVI",4,"DVI2",5,"Video1",6,"Video2",7,"S-Video",10,"TV",12,"DVD/HD1",13,"Option",14,"DVD/HD2",15,"DisplayPort",16,"DisplayPort2",17,"HDMI",18,"HDMI2",20,"USB",128,"DisplayPort3",130,"HDMI3",131,"HDMI4",132,"PRESET1",133,"PRESET2",134,"PRESET3",135,"Media Player",136,"Compute Module"
-1126,"Input Configuration|Left",1,1,"VGA",2,"RGB/HV",3,"DVI",4,"DVI2",5,"Video1",6,"Video2",7,"S-Video",10,"TV",12,"DVD/HD1",13,"Option",14,"DVD/HD2",15,"DisplayPort",16,"DisplayPort2",17,"HDMI",18,"HDMI2",20,"USB",128,"DisplayPort3",130,"HDMI3",131,"HDMI4",132,"PRESET1",133,"PRESET2",134,"PRESET3",135,"Media Player",136,"Compute Module"
-1127,"Input Configuration|Right",1,1,"VGA",2,"RGB/HV",3,"DVI",4,"DVI2",5,"Video1",6,"Video2",7,"S-Video",10,"TV",12,"DVD/HD1",13,"Option",14,"DVD/HD2",15,"DisplayPort",16,"DisplayPort2",17,"HDMI",18,"HDMI2",20,"USB",128,"DisplayPort3",130,"HDMI3",131,"HDMI4",132,"PRESET1",133,"PRESET2",134,"PRESET3",135,"Media Player",136,"Compute Module"
-1128,"Input Configuration|Top",1,1,"VGA",2,"RGB/HV",3,"DVI",4,"DVI2",5,"Video1",6,"Video2",7,"S-Video",10,"TV",12,"DVD/HD1",13,"Option",14,"DVD/HD2",15,"DisplayPort",16,"DisplayPort2",17,"HDMI",18,"HDMI2",20,"USB",128,"DisplayPort3",130,"HDMI3",131,"HDMI4",132,"PRESET1",133,"PRESET2",134,"PRESET3",135,"Media Player",136,"Compute Module"
-1129,"Input Configuration|Bottom",1,1,"VGA",2,"RGB/HV",3,"DVI",4,"DVI2",5,"Video1",6,"Video2",7,"S-Video",10,"TV",12,"DVD/HD1",13,"Option",14,"DVD/HD2",15,"DisplayPort",16,"DisplayPort2",17,"HDMI",18,"HDMI2",20,"USB",128,"DisplayPort3",130,"HDMI3",131,"HDMI4",132,"PRESET1",133,"PRESET2",134,"PRESET3",135,"Media Player",136,"Compute Module"
-
-112A,"Text Ticker|Window 1",1,1,"VGA",2,"RGB/HV",3,"DVI",4,"DVI2",5,"Video1",6,"Video2",7,"S-Video",10,"TV",12,"DVD/HD1",13,"Option",14,"DVD/HD2",15,"DisplayPort",16,"DisplayPort2",17,"HDMI",18,"HDMI2",20,"USB",128,"DisplayPort3",130,"HDMI3",131,"HDMI4",132,"PRESET1",133,"PRESET2",134,"PRESET3",135,"Media Player",136,"Compute Module"
-112B,"Text Ticker|Window 2",1,1,"VGA",2,"RGB/HV",3,"DVI",4,"DVI2",5,"Video1",6,"Video2",7,"S-Video",10,"TV",12,"DVD/HD1",13,"Option",14,"DVD/HD2",15,"DisplayPort",16,"DisplayPort2",17,"HDMI",18,"HDMI2",20,"USB",128,"DisplayPort3",130,"HDMI3",131,"HDMI4",132,"PRESET1",133,"PRESET2",134,"PRESET3",135,"Media Player",136,"Compute Module"
-
+1122,"Input Configuration|Top Left",1,1,"VGA",2,"RGB/HV",3,"DVI",4,"DVI2",5,"Video1",6,"Video2",7,"S-Video",10,"TV",12,"DVD/HD1",13,"Option",14,"DVD/HD2",15,"DisplayPort",16,"DisplayPort2",17,"HDMI",18,"HDMI2",20,"USB",128,"DisplayPort3",130,"HDMI3",131,"HDMI4",132,"PRESET1",133,"PRESET2",134,"PRESET3",135,"Media Player",136,"Compute Module",137,"USB-C"
+1123,"Input Configuration|Top Right",1,1,"VGA",2,"RGB/HV",3,"DVI",4,"DVI2",5,"Video1",6,"Video2",7,"S-Video",10,"TV",12,"DVD/HD1",13,"Option",14,"DVD/HD2",15,"DisplayPort",16,"DisplayPort2",17,"HDMI",18,"HDMI2",20,"USB",128,"DisplayPort3",130,"HDMI3",131,"HDMI4",132,"PRESET1",133,"PRESET2",134,"PRESET3",135,"Media Player",136,"Compute Module",137,"USB-C"
+1124,"Input Configuration|Bottom Left",1,1,"VGA",2,"RGB/HV",3,"DVI",4,"DVI2",5,"Video1",6,"Video2",7,"S-Video",10,"TV",12,"DVD/HD1",13,"Option",14,"DVD/HD2",15,"DisplayPort",16,"DisplayPort2",17,"HDMI",18,"HDMI2",20,"USB",128,"DisplayPort3",130,"HDMI3",131,"HDMI4",132,"PRESET1",133,"PRESET2",134,"PRESET3",135,"Media Player",136,"Compute Module",137,"USB-C"
+1125,"Input Configuration|Bottom Right",1,1,"VGA",2,"RGB/HV",3,"DVI",4,"DVI2",5,"Video1",6,"Video2",7,"S-Video",10,"TV",12,"DVD/HD1",13,"Option",14,"DVD/HD2",15,"DisplayPort",16,"DisplayPort2",17,"HDMI",18,"HDMI2",20,"USB",128,"DisplayPort3",130,"HDMI3",131,"HDMI4",132,"PRESET1",133,"PRESET2",134,"PRESET3",135,"Media Player",136,"Compute Module",137,"USB-C"
+1126,"Input Configuration|Left",1,1,"VGA",2,"RGB/HV",3,"DVI",4,"DVI2",5,"Video1",6,"Video2",7,"S-Video",10,"TV",12,"DVD/HD1",13,"Option",14,"DVD/HD2",15,"DisplayPort",16,"DisplayPort2",17,"HDMI",18,"HDMI2",20,"USB",128,"DisplayPort3",130,"HDMI3",131,"HDMI4",132,"PRESET1",133,"PRESET2",134,"PRESET3",135,"Media Player",136,"Compute Module",137,"USB-C"
+1127,"Input Configuration|Right",1,1,"VGA",2,"RGB/HV",3,"DVI",4,"DVI2",5,"Video1",6,"Video2",7,"S-Video",10,"TV",12,"DVD/HD1",13,"Option",14,"DVD/HD2",15,"DisplayPort",16,"DisplayPort2",17,"HDMI",18,"HDMI2",20,"USB",128,"DisplayPort3",130,"HDMI3",131,"HDMI4",132,"PRESET1",133,"PRESET2",134,"PRESET3",135,"Media Player",136,"Compute Module",137,"USB-C"
+1128,"Input Configuration|Top",1,1,"VGA",2,"RGB/HV",3,"DVI",4,"DVI2",5,"Video1",6,"Video2",7,"S-Video",10,"TV",12,"DVD/HD1",13,"Option",14,"DVD/HD2",15,"DisplayPort",16,"DisplayPort2",17,"HDMI",18,"HDMI2",20,"USB",128,"DisplayPort3",130,"HDMI3",131,"HDMI4",132,"PRESET1",133,"PRESET2",134,"PRESET3",135,"Media Player",136,"Compute Module",137,"USB-C"
+1129,"Input Configuration|Bottom",1,1,"VGA",2,"RGB/HV",3,"DVI",4,"DVI2",5,"Video1",6,"Video2",7,"S-Video",10,"TV",12,"DVD/HD1",13,"Option",14,"DVD/HD2",15,"DisplayPort",16,"DisplayPort2",17,"HDMI",18,"HDMI2",20,"USB",128,"DisplayPort3",130,"HDMI3",131,"HDMI4",132,"PRESET1",133,"PRESET2",134,"PRESET3",135,"Media Player",136,"Compute Module",137,"USB-C"
+112A,"Text Ticker|Input Window 1",1,1,"VGA",2,"RGB/HV",3,"DVI",4,"DVI2",5,"Video1",6,"Video2",7,"S-Video",10,"TV",12,"DVD/HD1",13,"Option",14,"DVD/HD2",15,"DisplayPort",16,"DisplayPort2",17,"HDMI",18,"HDMI2",20,"USB",128,"DisplayPort3",130,"HDMI3",131,"HDMI4",132,"PRESET1",133,"PRESET2",134,"PRESET3",135,"Media Player",136,"Compute Module",137,"USB-C"
+112B,"Text Ticker|Input Window 2",1,1,"VGA",2,"RGB/HV",3,"DVI",4,"DVI2",5,"Video1",6,"Video2",7,"S-Video",10,"TV",12,"DVD/HD1",13,"Option",14,"DVD/HD2",15,"DisplayPort",16,"DisplayPort2",17,"HDMI",18,"HDMI2",20,"USB",128,"DisplayPort3",130,"HDMI3",131,"HDMI4",132,"PRESET1",133,"PRESET2",134,"PRESET3",135,"Media Player",136,"Compute Module",137,"USB-C"
 112C,"Adjust|Aspect|Extension Zoom",0
 112D,"Adjust|Aspect|Extension H Zoom",0
 112E,"Adjust|Aspect|Extension V Zoom",0
-
 112F,"Video Sync Type",1,1,"Separate",2,"Composite",3,"Sync-on-green",4,"Digital"
 
-
 1147,"SpectraView Engine|SpectraView Engine Mode",1,1,"Off",2,"On"
 
 114C,"Human Sensing|Human Sensor Status",1,1,"No detect",2,"Detected"
+
+114E,"Backlight Local Dimming",1,1,"Off",2,"Low",3,"Mid",4,"High"
 114F,"Command Transfer",1,1,"Off",2,"On"
+
 1157,"OSD|Close/Mute OSD",1,1,"Close (off)",2,"On"
 
 1162,"Slot 2 CH Setting",1,1,"Auto",2,"1ch",3,"2ch"
-1163,"Slot 2 CH Select",1,1,"HDMI",2,"DisplayPort"
-
+1163,"Slot 2 CH Select",1,1,"HDMI",2,"DisplayPort",3,"Auto"
 
 1167,"Multi Input|Terminal Settings|DisplayPort",1,1,"SST",2,"MST"
 1168,"Multi Input|Terminal Settings|HDMI",1,1,"Mode1 (1.4)",2,"Mode2 (2.0)"
-1169,"Control|IR Lock Settings|Channel",1,1,"Unlock",2,"Lock"
-116A,"Control|Key Lock Settings|Mode Select",1,1,"Unlock",2,"Lock All"
-116B,"Control|Key Lock Settings|Power",1,1,"Unlock",2,"Lock"
-116C,"Control|Key Lock Settings|Volume",1,1,"Unlock",2,"Lock"
-116D,"Control|Key Lock Settings|Min Volume",0
-116E,"Control|Key Lock Settings|Max Volume",0
-116F,"Control|Key Lock Settings|Input",1,1,"Unlock",2,"Lock"
-1170,"Control|Key Lock Settings|Channel",1,1,"Unlock",2,"Lock"
+1169,"Control|IR Lock Settings|IR Lock Channel",1,1,"Unlock",2,"Lock"
+116A,"Control|Key Lock Settings|Key Lock Mode Select",1,1,"Unlock",2,"Lock All"
+116B,"Control|Key Lock Settings|Key Lock Power",1,1,"Unlock",2,"Lock"
+116C,"Control|Key Lock Settings|Key Lock Volume",1,1,"Unlock",2,"Lock"
+116D,"Control|Key Lock Settings|Key Lock Min Volume",0
+116E,"Control|Key Lock Settings|Key Lock Max Volume",0
+116F,"Control|Key Lock Settings|Key Lock Input",1,1,"Unlock",2,"Lock"
+1170,"Control|Key Lock Settings|Key Lock Channel",1,1,"Unlock",2,"Lock"
 1171,"Control|Power Indicator|Schedule Indicator",1,1,"Off",2,"On"
 1172,"Control|USB|USB Touch Power",1,1,"Off",2,"On"
 1173,"Control|USB|USB External Control",1,1,"Disable",2,"Enable"
 1174,"Control|USB|USB PC Source",1,1,"Auto",2,"External PC",3,"Internal PC",4,"Compute Module"
-1175,"Control|USB|USB Power",1,1,"On",2,"Auto"
-1176,"Control|CEC",1,1,"Off",2,"On"
+1175,"Control|USB|USB Power",1,1,"On",2,"Auto",3,"Off"
+1176,"Control|CEC",1,1,"Off",2,"Mode1 (On)",3,"Mode2"
 1177,"Control|CEC Auto Turn Off",1,1,"No",2,"Yes"
 1178,"Control|CEC Audio Receiver",1,1,"No",2,"Yes"
 1179,"Control|CEC Search Device",1,1,"No",2,"Yes"
 117A,"OSD|Key Guide",1,1,"Off",2,"On"
 117B,"Power Save Message",1,1,"Off",2,"On"
 117C,"Compute Module|Power Supply",1,1,"Off",2,"On"
 117D,"Compute Module|Auto Power On",1,1,"Disable",2,"Enable"
@@ -387,33 +441,99 @@
 1181,"Compute Module|Shutdown Signal",1,1,"Disable",2,"Enable"
 1182,"Compute Module|Power Supply Off Delay",0,"","sec"
 1183,"DP Power setting",1,1,"Off",2,"On",3,"Auto"
 1184,"Dual Link HDCP SW",1,1,"1",2,"2"
 1185,"Internal Touch",1,1,"Disable",2,"Enable"
 1186,"HDMI SW Through",1,1,"Off",2,"On"
 
+1191,"Equalizer|DisplayPort1 setting",0
 1192,"SpectraView Engine|Test Pattern Red Level",0,"Dark","Bright"
 1193,"SpectraView Engine|Test Pattern Green Level",0,"Dark","Bright"
 1194,"SpectraView Engine|Test Pattern Blue Level",0,"Dark","Bright"
 
 1196,"Tile Matrix|Tile Comp H Size",0
 1197,"Tile Matrix|Tile Comp V Size",0
 1198,"Tile Matrix|Tile Comp H Adjustment",0
 1199,"Tile Matrix|Tile Comp V Adjustment",0
 
-119B,"Compute Module|Watchdog Timer|Enable",1,1,"Disable",2,"Enable"
-119C,"Compute Module|Watchdog Timer|Start Up Time (sec x10)",0
-119D,"Compute Module|Watchdog Timer|Period Time (sec x10)",0
-119E,"Compute Module|Watchdog Timer|Reset",1,0,"Disabled",1,"Reset/Run",2,"Stop"
+119B,"Compute Module|Watchdog Timer|Watchdog Timer Enable",1,1,"Disable",2,"Enable"
+119C,"Compute Module|Watchdog Timer|Watchdog Timer Start Up Time (sec x10)",0
+119D,"Compute Module|Watchdog Timer|Watchdog Timer Period Time (sec x10)",0
+119E,"Compute Module|Watchdog Timer|Watchdog Timer Reset",1,0,"Disabled",1,"Reset/Run",2,"Stop"
+
+11A0,"Input Select for DisplayPort Switch",1,1,"DisplayPort",2,"USB-C"
+11A1,"Video Level|Custom White level",0
+11A2,"Video Level|Custom Black level",0
+11A3,"Color Space Select",1,1,"Auto",2,"RGB",3,"YCbCr(Bt.601)",4,"YCbCr(Bt.709)",5,"YCbCr(Bt.2020)"
 
+11A7,"PMS mode",1,1,"Standard",2,"Performance"
+
+11AE,"Low latency mode",1,1,"Off",3,"Auto"
+
+11B0,"SpectraView Engine|Number of Picture Modes",0
 11B1,"Color Processing Mode",1,1,"RGB",2,"YUV",3,"Auto"
-11B2,"Signal Format (read only)",1,1,"RGB",2,"YUV"
+#11B2,"Signal Format (read only)",1,1,"RGB",2,"YUV"
+11B2,"HDR Gamma Auto Select",1,1,"On",2,"Off"
 
+11B4,"G-sensor Orientation (read only)",1,1,"0'",2,"90' CCW",3,"180'",2,"270' CCW"
 11B5,"Compute Module|Fan Power Mode",1,1,"Off",2,"On",3,"Auto"
 11B6,"Compute Module|Fan Power Status (read only)",1,1,"Off",2,"On"
 11B7,"Compute Module|Auto Shutdown",1,1,"Disable",2,"Enable"
-
+11B8,"SpectraView Engine|System Gamma (HybridLog gamma)",0
+11B9,"SpectraView Engine|Peak lumi. (ST2084(PQ) gamma)",0
+11BA,"Audio|Speaker Select",1,1,"Off",2,"On",3,"Auto"
+
+11C0,"Tile Matrix|Tile Cut",1,1,"No",2,"Yes"
+11C1,"Tile Matrix|Tile Cut|H Adjustment",0
+11C2,"Tile Matrix|Tile Cut|V Adjustment",0
+
+11C7,"Uniformity|Corner position",1,0,"TopLeft",1,"TopRight",2,"BottomLeft",3,"BottomRight"
+11C8,"Uniformity|Adjustment Area",1,0,"Wide",1,"Medium",2,"Narrow"
+11C9,"Uniformity|Value",0
+11CC,"Uniformity|Auto",1,1,"Off",2,"On"
+11CD,"Uniformity|Manual",1,1,"Off",2,"On"
+
+11CF,"LAN|Display Control LAN Port",1,1,"Disable",2,"Enable"
+11D0,"LAN|Media Player LAN Port",1,1,"Disable",2,"Enable"
+11D1,"LAN|Compute Module LAN Port",1,1,"Disable",2,"Enable"
+11D2,"HDCP version",1,1,"HDCP 1.4",2,"HDCP 2.2"
+11D3,"USB-C data setting",1,1,"USB 2.0",2,"USB 3.1"
+11D4,"HDR HLG Gamma Auto",1,1,"Lumi",2,"MDML",3,"MCLL"
+11D5,"HDR PQ Gamma Auto",1,1,"Lumi",2,"MDML",3,"MCLL"
+11D6,"EQ auto setting",1,1,"Auto",2,"Manual"
+11D7,"SpectraView Engine|SVE Version",0
+11D8,"Audio Preset",1,1,"Retail",2,"Conferencing",3,"HighBright",4,"Transportation",5,"Custom1",7,"Native"
+11D9,"Slot|Active Slot",1,1,"Option",2,"Compute Module"
+11DA,"Slot|Option Power Supply",1,1,"On",2,"Off"
+11DB,"Slot|Option Soft Power Button",1,1,"Execute"
+11DC,"Slot|Option Reset",1,1,"Execute"
+11DD,"Slot|Option Auto Power Up",1,1,"Disable",2,"Enable"
+11DE,"Slot|Option Auto Shut Down",1,1,"Disable",2,"Enable"
+11DF,"Slot|Option Power On Delay Time",0
+11E0,"Slot|Compute Module Soft Power Button",1,1,"Execute"
+11E1,"Slot|Compute Module Reset",1,1,"Execute"
+11E2,"Slot|Option Power Auto Off",1,1,"Separate",2,"Tied"
+11E3,"Slot|Option Power Off Show Warning",1,1,"Disable",2,"Enable"
+11E4,"Lock Settings Select",1,1,"Key",2,"IR",3,"Both"
+11E5,"HDR Mode",1,1,"Off",2,"On",3,"Auto"
+11E6,"OSD Size",1,1,"Normal",2,"Expand"
+11E7,"Slot|Option System Fan Requirement (read only)",1,1,"No",2,"Yes"
+11E8,"Slot|Compute Module System Fan Requirement (read only)",1,1,"No",2,"Yes"
+11E9,"Mute Setting",1,1,"Audio",2,"Video",3,"Audio & Video"
+11EA,"Quick Start",1,1,"Disable",2,"Enable"
+11EB,"PIP|Multi Picture Mode Select",1,1,"Off",2,"2PIP",3,"2PBP",4,"4PBP"
+11EE,"Power Save Mode",1,1,"Mode 1",2,"Mode 2"
+11F0,"LAN|Network Port Switch|HTTP Server",1,1,"Disable",2,"Enable"
+11F1,"LAN|Network Port Switch|PJLink",1,1,"Disable",2,"Enable"
+11F2,"LAN|Network Port Switch|AMX Beacon",1,1,"Disable",2,"Enable"
+11F3,"LAN|Network Port Switch|Crestron",1,1,"Disable",2,"Enable"
+11F4,"LAN|Network Port Switch|PC Control",1,1,"Disable",2,"Enable"
+11F5,"Ambient Illuminance Low",0
+11F6,"Ambient Illuminance High",0
+11F7,"DisplayPort Power DP1",1,1,"Off",2,"On"
+11F8,"DisplayPort Power DP2",1,1,"Off",2,"On"
+11F9,"DisplayPort Power DP Out",1,1,"Off",2,"On"
 11FA,"Total Operating Time (upper) (minutes) (read only)",0
 11FB,"Total Operating Time (lower) (minutes) (read only)",0
+11FD,"HDR version",1,1,"Disable",2,"Enable"
 11FE,"Operating Time On (upper) (minutes) (read only)",0
 11FF,"Operating Time On (lower) (minutes) (read only)",0
-
```

### Comparing `nec_pd_sdk-18.2.231/nec_pd_sdk/constants.py` & `nec_pd_sdk-23.8.21/nec_pd_sdk/constants.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """constants.py - Various constants used for communicating with NEC large-screen displays.
-Revision: 180220
+Revision: 230717
 """
 #
 #
 # Copyright (C) 2016-18 NEC Display Solutions, Ltd
-# written by Will Hollingworth <whollingworth at necdisplay.com>
+# Copyright (C) 2023 Sharp NEC Display Solutions, Ltd
+# written by Will Hollingworth <William.Hollingworth at sharpusa.com>
 # See LICENSE.rst for details.
 #
 
 # timeout in seconds for establishing a TCP connection
 connect_timeout = 2.0
 # timeout in seconds for waiting for a reply from the display
 reply_timeout = 7.0
@@ -51,18 +52,25 @@
 OPCODE_PICTURE__COLOR__6_AXIS_COLOR_MAGENTA = 0x00a0
 OPCODE_SETTINGS = 0x00b0
 OPCODE_MONITOR_TYPE_READ_ONLY = 0x00b6
 OPCODE_POWER_MODE_READ_ONLY = 0x00d6
 OPCODE_SCAN_MODE = 0x00da
 OPCODE_VCP_VERSION_READ_ONLY = 0x00df
 OPCODE_POWER_SAVE = 0x00e1
+OPCODE_OSD_POSITION = 0x00ef
 OPCODE_TOTAL_OPERATING_TIME_30_MIN_READ_ONLY = 0x00fa
 OPCODE_KEY_LOCK = 0x00fb
 OPCODE_OSD__OSD_TURN_OFF_DELAY = 0x00fc
 OPCODE_OPERATING_TIME_ON_30_MIN_READ_ONLY = 0x00ff
+OPCODE_PICTURE__COLOR__6_AXIS_SATURATION_RED = 0x0212
+OPCODE_PICTURE__COLOR__6_AXIS_SATURATION_YELLOW = 0x0213
+OPCODE_PICTURE__COLOR__6_AXIS_SATURATION_GREEN = 0x0214
+OPCODE_PICTURE__COLOR__6_AXIS_SATURATION_CYAN = 0x0215
+OPCODE_PICTURE__COLOR__6_AXIS_SATURATION_BLUE = 0x0216
+OPCODE_PICTURE__COLOR__6_AXIS_SATURATION_MAGENTA = 0x0217
 OPCODE_PICTURE__PICTURE_MODE = 0x021a
 OPCODE_PICTURE__COLOR__COLOR = 0x021f
 OPCODE_PICTURE__NOISE_REDUCTION = 0x0220
 OPCODE_COLOR_SYSTEM = 0x0221
 OPCODE_PICTURE__FILM_MODE = 0x0223
 OPCODE_SCAN_CONVERSION = 0x0225
 OPCODE_NOISE_REDUCTION = 0x0226
@@ -102,14 +110,15 @@
 OPCODE_SCART_MODE = 0x029e
 OPCODE_SPECTRAVIEW_ENGINE__LUMINANCE_SET = 0x02b3
 OPCODE_CURRENT_LUMINANCE_READ_ONLY = 0x02b4
 OPCODE_BRIGHT_SENSOR_READ_READ_ONLY = 0x02b5
 OPCODE_OSD__OSD_TRANSPARENCY = 0x02b8
 OPCODE_POWER_LED_INDICATOR = 0x02be
 OPCODE_TEST_PATTERN__VT_MODE = 0x02c3
+OPCODE_TEST_PATTERN__SPECTRAVIEW_ENGINE = 0x02c8
 OPCODE_CSC_GAIN = 0x02ca
 OPCODE_RESET__MENU_TREE_RESET = 0x02cb
 OPCODE_ADJUST__ASPECT__ZOOM_H_POSITION = 0x02cc
 OPCODE_ADJUST__ASPECT__ZOOM_V_POSITION = 0x02cd
 OPCODE_ADJUST__ASPECT__BASE_ZOOM = 0x02ce
 OPCODE_DVI_MODE = 0x02cf
 OPCODE_TILE_MATRIX__TILE_MATRIX_H_MONITORS = 0x02d0
@@ -130,14 +139,20 @@
 OPCODE_RESET__ADVANCED_OPTION_RESET = 0x02e4
 OPCODE_ENABLE_SCHEDULE = 0x02e5
 OPCODE_DISABLE_SCHEDULE = 0x02e6
 OPCODE_SPECTRAVIEW_ENGINE__CUSTOM_GAMMA_VALUE = 0x02e8
 OPCODE_SIGNAL_INFORMATION = 0x02ea
 OPCODE_UNIFORMITY_CORRECTION_LEVEL = 0x02ee
 OPCODE_LONG_CABLE__COMP_DVI = 0x02f0
+OPCODE_PICTURE__COLOR__6_AXIS_BRIGHTNESS_RED = 0x02F1
+OPCODE_PICTURE__COLOR__6_AXIS_BRIGHTNESS_YELLOW = 0x02F2
+OPCODE_PICTURE__COLOR__6_AXIS_BRIGHTNESS_GREEN = 0x02F3
+OPCODE_PICTURE__COLOR__6_AXIS_BRIGHTNESS_CYAN = 0x02F4
+OPCODE_PICTURE__COLOR__6_AXIS_BRIGHTNESS_BLUE = 0x02F5
+OPCODE_PICTURE__COLOR__6_AXIS_BRIGHTNESS_MAGENTA = 0x02F6
 OPCODE_RESET__GAMMA_PROGRAMMABLE_RESET = 0x02f8
 OPCODE_GAMMA_PROGRAMMABLE_LUT_SIZE = 0x02f9
 OPCODE_ISF = 0x1000
 OPCODE_ISF_MODE = 0x1001
 OPCODE_ISF_DATA_COPY = 0x1002
 OPCODE_PIP__TEXT_TICKER_MODE = 0x1008
 OPCODE_PIP__TEXT_TICKER_POSITION = 0x1009
@@ -184,14 +199,15 @@
 OPCODE_SPECTRAVIEW_ENGINE__TARGET_COLORSPACE_RED_CIE_Y_X1000 = 0x1056
 OPCODE_SPECTRAVIEW_ENGINE__TARGET_COLORSPACE_GREEN_CIE_X_X1000 = 0x1057
 OPCODE_SPECTRAVIEW_ENGINE__TARGET_COLORSPACE_GREEN_CIE_Y_X1000 = 0x1058
 OPCODE_SPECTRAVIEW_ENGINE__TARGET_COLORSPACE_BLUE_CIE_X_X1000 = 0x1059
 OPCODE_SPECTRAVIEW_ENGINE__TARGET_COLORSPACE_BLUE_CIE_Y_X1000 = 0x105a
 OPCODE_SPECTRAVIEW_ENGINE__COLOR_VISION_EMULATION = 0x105b
 OPCODE_SPECTRAVIEW_ENGINE__METAMERISM = 0x105c
+OPCODE_BLANK_SIGNAL_SKIP = 0x1064
 OPCODE_SPECTRAVIEW_ENGINE__PRINT_PREVIEW_3D_LUT = 0x1069
 OPCODE_SPECTRAVIEW_ENGINE__3D_LUTPROG_GAMMA_SELECT = 0x106b
 OPCODE_SPECTRAVIEW_ENGINE__RESET_PICTURE_MODE = 0x1070
 OPCODE_SPECTRAVIEW_ENGINE__TARGET_COLORSPACE_RESET = 0x1071
 OPCODE_HUMAN_SENSING__HUMAN_SENSING_MODE = 0x1075
 OPCODE_HUMAN_SENSING__HUMAN_SENSING_READING = 0x1076
 OPCODE_HUMAN_SENSING__HUMAN_SENSING_THRESHOLD = 0x1077
@@ -222,32 +238,39 @@
 OPCODE_EXPERT_ANALOG_VIDEO__ADC_OFFSET_BLUE = 0x109d
 OPCODE_EXPERT_ANALOG_VIDEO__ADC_GAIN_RED = 0x109e
 OPCODE_EXPERT_ANALOG_VIDEO__ADC_GAIN_GREEN = 0x109f
 OPCODE_EXPERT_ANALOG_VIDEO__ADC_GAIN_BLUE = 0x10a0
 OPCODE_DIGITAL_CLOSED_CAPTION = 0x10a1
 OPCODE_AUDIO__AUDIO_VOLUME_STEP = 0x10ad
 OPCODE_AUDIO__OPTION_SLOT_AUDIO = 0x10b0
+OPCODE_USB__POWER = 0x10B1
+OPCODE_AUDIO__MODE = 0x10B2
+OPCODE_AUDIO__LANGUAGE = 0x10B3
 OPCODE_PIP__PBP_TYPE = 0x10b5
 OPCODE_SCREEN_MUTE = 0x10b6
 OPCODE_AUTO_ADJUST = 0x10b7
 OPCODE_OSD__OSD_FLIP = 0x10b8
 OPCODE_PIP__PIP_SIZE__VARIABLE = 0x10b9
 OPCODE_MEMO_DISPLAY = 0x10ba
 OPCODE_POWER_ON_DELAY_LINK_TO_ID = 0x10bc
 OPCODE_DDCI = 0x10be
+OPCODE_RESET__IP_ADDRESS_RESET = 0x10BF
 OPCODE_OPS__INTERNAL_PC_OFF_WARNING = 0x10c0
 OPCODE_OPS__INTERNAL_PC_AUTO_OFF = 0x10c1
 OPCODE_OPS__INTERNAL_PC_START = 0x10c2
 OPCODE_OPS__INTERNAL_PC_FORCE_QUIT = 0x10c3
 OPCODE_TOUCH_PANEL_POWER_SUPPLY = 0x10c4
 OPCODE_TOUCH_PANEL_PC_SOURCE = 0x10c5
 OPCODE_HUMAN_SENSING__HUMAN_SENSING_BACKLIGHT = 0x10c6
 OPCODE_HUMAN_SENSING__HUMAN_SENSING_VOLUME = 0x10c7
 OPCODE_ROOM_LIGHT_SENSING = 0x10c8
 OPCODE_ROOM_AMBIENT_BRIGHTNESS_MAX = 0x10c9
+OPCODE_AUDIO__DELAY_SW = 0x10CA
+OPCODE_AUDIO__DELAY = 0x10CB
+OPCODE_MODEL_ID = 0x10CB
 OPCODE_INPUT_CHANGE_SUPER_INPUT_1 = 0x10ce
 OPCODE_INPUT_CHANGE_SUPER_INPUT_2 = 0x10cf
 OPCODE_HUMAN_SENSING__HUMAN_SENSING_INPUT = 0x10d0
 OPCODE_POWER_SAVE_TIMER = 0x10d2
 OPCODE_LAN_POWER = 0x10d3
 OPCODE_IR_LOCK_SETTINGS_MODE_SELECT = 0x10d4
 OPCODE_IR_LOCK_SETTINGS_POWER = 0x10d5
@@ -273,14 +296,23 @@
 OPCODE_BOWLING_MODE = 0x10ef
 OPCODE_HUMAN_SENSING__HUMAN_SENSOR_ATTACHMENT_STATUS_READ_ONLY = 0x10f0
 OPCODE_DISPLAYPORT_TERMINAL_SELECT = 0x10f1
 OPCODE_DISPLAYPORT_TERMINAL_TYPE = 0x10f2
 OPCODE_EXTENDED_POWER_SAVE = 0x10f5
 OPCODE_AUTO_POWER_SAVE_TIME_SEC_X5 = 0x10f6
 OPCODE_AUTO_STANDBY_TIME_SEC_X5 = 0x10f7
+OPCODE_PANEL__NATIVE_WHITE_CIE_x = 0x10F8
+OPCODE_PANEL__NATIVE_WHITE_CIE_y = 0x10F9
+OPCODE_PANEL__NATIVE_RED_CIE_x = 0x10FA
+OPCODE_PANEL__NATIVE_RED_CIE_y = 0x10FB
+OPCODE_PANEL__NATIVE_GREEN_CIE_x = 0x10FC
+OPCODE_PANEL__NATIVE_GREEN_CIE_y = 0x10FD
+OPCODE_PANEL__NATIVE_BLUE_CIE_x = 0x10FE
+OPCODE_PANEL__NATIVE_BLUE_CIE_y = 0x10FF
+OPCODE_PANEL__NATIVE_MAX_BRIGHTNESS = 0x1100
 OPCODE_TILE_MATRIX__FRAME_COMP_MODE = 0x1101
 OPCODE_TILE_MATRIX__FRAME_COMP_AUTO_VALUE = 0x1102
 OPCODE_TILE_MATRIX__FRAME_COMP_MANUAL_VALUE = 0x1103
 OPCODE_TILE_MATRIX__V_SCAN_REVERSE_MODE = 0x1104
 OPCODE_TILE_MATRIX__V_SCAN_REVERSE_MANUAL = 0x1105
 OPCODE_INPUT_ALT = 0x1106
 OPCODE_UHD_UPSCALING = 0x1109
@@ -315,18 +347,22 @@
 OPCODE_INPUT_CONFIGURATION__TOP = 0x1128
 OPCODE_INPUT_CONFIGURATION__BOTTOM = 0x1129
 OPCODE_TEXT_TICKER__WINDOW_1 = 0x112a
 OPCODE_TEXT_TICKER__WINDOW_2 = 0x112b
 OPCODE_ADJUST__ASPECT__EXTENSION_ZOOM = 0x112c
 OPCODE_ADJUST__ASPECT__EXTENSION_H_ZOOM = 0x112d
 OPCODE_ADJUST__ASPECT__EXTENSION_V_ZOOM = 0x112e
+OPCODE_VIDEO_SYNC_TYPE = 0x112F
 OPCODE_SPECTRAVIEW_ENGINE__SPECTRAVIEW_ENGINE_MODE = 0x1147
 OPCODE_HUMAN_SENSING_HUMAN_SENSOR_STATUS = 0x114c
+OPCODE_BACKLIGHT_LOCAL_DIMMING = 0x114E
 OPCODE_COMMAND_TRANSFER = 0x114f
 OPCODE_OSD_CLOSE_OSD = 0x1157
+OPCODE_SLOT_CH2_SETTING = 0x1162
+OPCODE_SLOT_CH2_SELECT = 0x1163
 OPCODE_MULTI_INPUT_TERMINAL_SETTINGS_DISPLAYPORT = 0x1167
 OPCODE_MULTI_INPUT_TERMINAL_SETTINGS_HDMI = 0x1168
 OPCODE_CONTROL_IR_LOCK_SETTINGS_CHANNEL = 0x1169
 OPCODE_CONTROL_KEY_LOCK_SETTINGS_MODE_SELECT = 0x116a
 OPCODE_CONTROL_KEY_LOCK_SETTINGS_POWER = 0x116b
 OPCODE_CONTROL_KEY_LOCK_SETTINGS_VOLUME = 0x116c
 OPCODE_CONTROL_KEY_LOCK_SETTINGS_MIN_VOLUME = 0x116d
@@ -351,25 +387,93 @@
 OPCODE_COMPUTE_MODULE_MONITOR_CONTROL = 0x1180
 OPCODE_COMPUTE_MODULE_SHUTDOWN_SIGNAL = 0x1181
 OPCODE_COMPUTE_MODULE_POWER_SUPPLY_OFF_DELAY = 0x1182
 OPCODE_DP_POWER_SETTING = 0x1183
 OPCODE_DUAL_LINK_HDCP_SWITCH = 0x1184
 OPCODE_INTERNAL_TOUCH = 0x1185
 OPCODE_HDMI_SW_THROUGH = 0x1186
+OPCODE_EQUALIZER__DISPLAYPORT1_SETTING = 0x1191
+OPCODE_SPECTRAVIEW_ENGINE__TEST_PATTERN_RED_LEVEL = 0x1192
+OPCODE_SPECTRAVIEW_ENGINE__TEST_PATTERN_GREEN_LEVEL = 0x1193
+OPCODE_SPECTRAVIEW_ENGINE__TEST_PATTERN_BLUE_LEVEL = 0x1194
+OPCODE_TILE_MATRIX__TILE_COMP_H_SIZE = 0x1196
+OPCODE_TILE_MATRIX__TILE_COMP_V_SIZE = 0x1197
+OPCODE_TILE_MATRIX__TILE_COMP_H_ADJUSTMENT = 0x1198
+OPCODE_TILE_MATRIX__TILE_COMP_V_ADJUSTMENT = 0x1199
 OPCODE_COMPUTE_MODULE_WATCHDOG_TIMER_ENABLE = 0x119b
 OPCODE_COMPUTE_MODULE_WATCHDOG_TIMER_START_UP_TIME = 0x119c
 OPCODE_COMPUTE_MODULE_WATCHDOG_TIMER_PERIOD_TIME = 0x119d
 OPCODE_COMPUTE_MODULE_WATCHDOG_TIMER_RESET = 0x119e
-
+OPCODE_DISPLAYPORT_INPUT_SELECT = 0x11A0
+OPCODE_VIDEO_LEVEL__CUSTOM_WHITE_LEVEL = 0x11A1
+OPCODE_VIDEO_LEVEL__CUSTOM_BLACK_LEVEL = 0x11A2
+OPCODE_COLOR_SPACE_SELECT = 0x11A3
+OPCODE_PMS_MODE = 0x11A7
+OPCODE_LOW_LATENCY_MODE = 0x11AE
+OPCODE_SPECTRAVIEW_ENGINE__NUMBER_OF_PICTURE_MODES = 0x11B0
+OPCODE_COLOR_PROCESSING_MODE = 0x11B1
+OPCODE_HDR_GAMMA_AUTO_SELECT = 0x11B2
+OPCODE_G_SENSOR_ORIENTATION_READ = 0x11B4
 OPCODE_COMPUTE_MODULE_FAN_POWER_MODE = 0x11b5
 OPCODE_COMPUTE_MODULE_FAN_POWER_STATUS = 0x11b6
 OPCODE_COMPUTE_MODULE_AUTO_SHUTDOWN = 0x11b7
-
+OPCODE_SPECTRAVIEW_ENGINE__SYSTEM_GAMMA_HLG = 0x11B8
+OPCODE_SPECTRAVIEW_ENGINE__PEAK_LUMINANCE = 0x11B9
+OPCODE_AUDIO__SPEAKER_SELECT = 0x11BA
+OPCODE_TILE_MATRIX__TILE_CUT = 0x11C0
+OPCODE_TILE_MATRIX__TILE_CUT_H_ADJUSTMENT = 0x11C1
+OPCODE_TILE_MATRIX__TILE_CUT_V_ADJUSTMENT = 0x11C2
+OPCODE_UNIFORMITY__CORNER_POSITION = 0x11C7
+OPCODE_UNIFORMITY__ADJUSTMENT_AREA = 0x11C8
+OPCODE_UNIFORMITY__VALUE = 0x11C9
+OPCODE_UNIFORMITY__AUTO = 0x11CC
+OPCODE_UNIFORMITY__MANUAL = 0x11CD
+OPCODE_LAN__DISPLAY_CONTROL_LAN_PORT = 0x11CF
+OPCODE_LAN__MEDIA_PLAYER_LAN_PORT = 0x11D0
+OPCODE_LAN__COMPUTE_MODULE_LAN_PORT = 0x11D1
+OPCODE_HDCP_VERSION = 0x11D2
+OPCODE_USB_C_DATA_SETTING = 0x11D3
+OPCODE_HDR_HLG_GAMMA_AUTO = 0x11D4
+OPCODE_HDR_PQ_GAMMA_AUTO = 0x11D5
+OPCODE_EQ_AUTO_SETTING = 0x11D6
+OPCODE_SPECTRAVIEW_ENGINE__VERSION = 0x11D7
+OPCODE_AUDIO__PRESET = 0x11D8
+OPCODE_SLOT__ACTIVE_SLOT = 0x11D9
+OPCODE_SLOT__OPTION_POWER_SUPPLY = 0x11DA
+OPCODE_SLOT__OPTION_SOFT_POWER_BUTTON = 0x11DB
+OPCODE_SLOT__OPTION_RESET = 0x11DC
+OPCODE_SLOT__OPTION_AUTO_POWER_UP = 0x11DD
+OPCODE_SLOT__OPTION_AUTO_SHUT_DOWN = 0x11DE
+OPCODE_SLOT__OPTION_POWER_ON_DELAY_TIME = 0x11DF
+OPCODE_SLOT__COMPUTE_MODULE_SOFT_POWER_BUTTON = 0x11E0
+OPCODE_SLOT__COMPUTE_MODULE_RESET = 0x11E1
+OPCODE_SLOT__OPTION_POWER_AUTO_OFF = 0x11E2
+OPCODE_SLOT__OPTION_POWER_OFF_SHOW_WARNING = 0x11E3
+OPCODE_LOCK_SETTINGS_SELECT = 0x11E4
+OPCODE_HDR_MODE = 0x11E5
+OPCODE_OSD__SIZE = 0x11E6
+OPCODE_SLOT__OPTION_SYSTEM_FAN_REQUIREMENT = 0x11E7
+OPCODE_SLOT__COMPUTE_MODULE_SYSTEM_FAN_REQUIREMENT = 0x11E8
+OPCODE_MUTE_SETTING = 0x11E9
+OPCODE_QUICK_START = 0x11EA
+OPCODE_PIP__MULTI_PICTURE_MODE_SELECT = 0x11EB
+OPCODE_POWER_SAVE_MODE = 0x11EE
+OPCODE_LAN__NETWORK_PORT__HTTP_SERVER = 0x11F0
+OPCODE_LAN__NETWORK_PORT__PJLINK = 0x11F1
+OPCODE_LAN__NETWORK_PORT__AMX_BEACON = 0x11F2
+OPCODE_LAN__NETWORK_PORT__CRESTRON = 0x11F3
+OPCODE_LAN__NETWORK_PORT__PC_CONTROL = 0x11F4
+OPCODE_AMBIENT_ILLUMINANCE_LOW = 0x11F5
+OPCODE_AMBIENT_ILLUMINANCE_HIGH = 0x11F6
+OPCODE_DISPLAYPORT_POWER_DP1 = 0x11F7
+OPCODE_DISPLAYPORT_POWER_DP2 = 0x11F8
+OPCODE_DISPLAYPORT_POWER_DP_OUT = 0x11F9
 OPCODE_TOTAL_OPERATING_TIME__UPPER___MINUTES___READ_ONLY_ = 0x11fa
 OPCODE_TOTAL_OPERATING_TIME__LOWER___MINUTES___READ_ONLY_ = 0x11fb
+OPCODE_HDR_VERSION = 0x11FD
 OPCODE_OPERATING_TIME_ON__UPPER___MINUTES___READ_ONLY_ = 0x11fe
 OPCODE_OPERATING_TIME_ON__LOWER___MINUTES___READ_ONLY_ = 0x11ff
 
 # dictionary of codes for use when sending IR remote button emulation commands
 # e.g. command_send_ir_remote_control_code() and helper_send_ir_remote_control_codes()
 PD_IR_COMMAND_CODES = {
     'power': 0x03,
@@ -435,15 +539,20 @@
     'multipicture_mode': 0x63,
     'multipicture_change': 0x26,
     'multipicture_picture_aspect': 0x62,
     'multipicture_rotate': 0x60,
     'multipicture_rotate_all': 0x61,
     'preset1': 0x5c,
     'preset2': 0x5d,
-    'preset3': 0x5e
+    'preset3': 0x5e,
+    'input': 0x01,
+    'usb_c': 0x78,
+    'home': 0x79,
+    'backlight+': 0x7a,
+    'backlight-': 0x7b
 }
 
 
 # dictionary of diagnostic error codes that can be returned by the display
 # e.g. helper_self_diagnosis_status_text() and command_self_diagnosis_status_read()
 DISPLAY_DIAGNOSTIC_ERROR_CODES = {
     0x00: "Normal",
@@ -469,15 +578,21 @@
     0xC0: "Option board (SLOT3) abnormality",
     0xD0: "PROOF OF PLAY buffer full",
     0xD1: "RTC error",
     0xE0: "System/EEPROM error",
     0xE1: "Pegasus error",
     0xE2: "LPM-Mission communication error",
     0xE3: "NFC-EEPROM error",
-    0xE4: "CPLD error"
+    0xE4: "CPLD error",
+    0xE5: "HDMI_SW1 error",
+    0xE6: "HDMI_SW2 error",
+    0xE7: "Scaler DP block abnormal",
+    0xE8: "Garnet EEPROM error",
+    0xEB: "Wrong orientation (G sensor)",
+    0xEC: "Strong impact (G sensor)"
 }
 
 # dictionary of fan status modes returned by the display
 DISPLAY_FAN_STATUS = {
     0x00: "Off",
     0x01: "On",
     0x02: "Error"
```

### Comparing `nec_pd_sdk-18.2.231/nec_pd_sdk/nec_pd_sdk.py` & `nec_pd_sdk-23.8.21/nec_pd_sdk/nec_pd_sdk.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 # -*- coding: utf-8 -*-
 """nec_pd_sdk.py - High level functions for communicating via LAN or RS232 with NEC large-screen displays.
-
+Revision: 230717
 """
 #
 #
 # Copyright (C) 2016-18 NEC Display Solutions, Ltd
-# written by Will Hollingworth <whollingworth at necdisplay.com>
+# Copyright (C) 2023 Sharp NEC Display Solutions, Ltd
+# written by Will Hollingworth <William.Hollingworth at sharpusa.com>
 # See LICENSE.rst for details.
 
 # TODO == Helper Functions ==
 # daylight savings decode
 # command_auto_power_save_time_write - helper
 # opcode unsupported exception
 # POP reserved_1 decode
 
-
-
 from collections import namedtuple
 import socket
 import string
 import serial
 import logging
 import time
 import datetime
-from enum import Enum
+# from enum import Enum
 from .protocol import *
 from .constants import *
 
-
 PDDateTimeTuple = namedtuple('PDDateTimeTuple', ['status',
                                                  'year',
                                                  'month',
                                                  'day',
                                                  'weekday',
                                                  'hour',
                                                  'minute',
@@ -56,40 +54,40 @@
                                                  'extension_7'])
 
 PDScheduleEnableDisableTuple = namedtuple('PDScheduleEnableDisable', ['status',
                                                                       'program_no',
                                                                       'enable_disable'])
 
 PDAdvancedScheduleTuple = namedtuple('PDAdvancedScheduleTuple', ['status',
-                                                 'program_no',
-                                                 'event',
-                                                 'hour',
-                                                 'minute',
-                                                 'input',
-                                                 'week',
-                                                 'type',
-                                                 'picture_mode',
-                                                 'year',
-                                                 'month',
-                                                 'day',
-                                                 'order',
-                                                 'extension_1',
-                                                 'extension_2',
-                                                 'extension_3'])
+                                                                 'program_no',
+                                                                 'event',
+                                                                 'hour',
+                                                                 'minute',
+                                                                 'input',
+                                                                 'week',
+                                                                 'type',
+                                                                 'picture_mode',
+                                                                 'year',
+                                                                 'month',
+                                                                 'day',
+                                                                 'order',
+                                                                 'extension_1',
+                                                                 'extension_2',
+                                                                 'extension_3'])
 
 PDHolidayTuple = namedtuple('PDHolidayTuple', ['status',
-                                        'id',
-                                        'type',
-                                        'year',
-                                        'month',
-                                        'day',
-                                        'week_of_month',
-                                        'day_of_week',
-                                        'end_month',
-                                        'end_day'])
+                                               'id',
+                                               'type',
+                                               'year',
+                                               'month',
+                                               'day',
+                                               'week_of_month',
+                                               'day_of_week',
+                                               'end_month',
+                                               'end_day'])
 
 PDWeekendTuple = namedtuple('PDWeekendTuple', ['status',
                                                'weekend'])
 
 PDDaylightSavingsTuple = namedtuple('PDDaylightSavingsTuple', ['status',
                                                                'begin_month',
                                                                'begin_day1',
@@ -124,15 +122,14 @@
                                                                      'hour',
                                                                      'minute',
                                                                      'second',
                                                                      'reserved_1',
                                                                      'reserved_2',
                                                                      'reserved_3'])
 
-
 PDHelperProofOfPlayLogItemTuple = namedtuple('PDHelperProofOfPlayLogItemTuple', ['status',
                                                                                  'log_number',
                                                                                  'input',
                                                                                  'signal_h_resolution',
                                                                                  'signal_v_resolution',
                                                                                  'audio_input',
                                                                                  'audio_input_status',
@@ -144,15 +141,14 @@
                                                                                  'reserved_3'])
 
 PDProofOfPlayStatusTuple = namedtuple('PDProofOfPlayStatusTuple', ['error_status',
                                                                    'total_number',
                                                                    'maximum_number',
                                                                    'current_status'])
 
-
 PDTileMatrixProfileTuple = namedtuple('PDTileMatrixProfileTuple',
                                       ['profile_number',
                                        'h_monitors',
                                        'v_monitors',
                                        'position',
                                        'tile_comp'])
 
@@ -195,15 +191,16 @@
                                    'reserved_17',
                                    'reserved_18',
                                    'reserved_19',
                                    'reserved_20',
                                    'reserved_21',
                                    'reserved_22'])
 
-class PDSchedule():
+
+class PDSchedule:
     """
     This class holds the definitions values of schedule items
     """
 
     OnEvent = 1
     OffEvent = 2
 
@@ -219,19 +216,21 @@
     Tuesday = 0x02
     Wednesday = 0x04
     Thursday = 0x08
     Friday = 0x10
     Saturday = 0x20
     Sunday = 0x40
 
+
 def retry(function):
     """
     Attempts to retry a command if there was a protocol error.
     Closes and reopens the port to flush the buffers.
     """
+
     def _retry(self, *args, **kwargs):
         try:
             # reply = function(*args, **kwargs)
             reply = function(self, *args, **kwargs)
             # print "reply: ", reply
             return reply
         except (PDUnexpectedReplyError, PDNullMessageReplyError, PDTimeoutError) as msg:
@@ -246,26 +245,27 @@
                 raise
             except PDNullMessageReplyError as msg:
                 logging.error('command retry failed with error "%s" so assume unsupported', msg)
                 raise PDCommandNotSupportedError('retry failed so assume unsupported')
         except PDCommandNotSupportedError as msg:
             logging.debug('unsupported command error "%s" so do not retry', msg)
             raise
-        except:
+        except Exception:
             logging.debug('an unhandled error type so do not retry')
             raise
 
     return _retry
 
 
 class MySerial(serial.Serial):  # subclass, inherits from serial
     """
     Add our own functions for serial support to mimic those in 'socket', so we can use the same
     function names.
     """
+
     def settimeout(self, length):
         self.timeout = length
 
     def recv(self, length):
         return self.read(length)
 
     def sendall(self, data):
@@ -391,22 +391,22 @@
         :return: namedtuple 'PDOpCodeGetSetTuple'
         """
         logging.debug('opcode=%04xh', opcode)
         assert 0x0000 <= opcode <= 0xffff
         send_data = []
         send_data.extend(ascii_encode_value_4_bytes(opcode))
         write_command(self.f,
-                               send_data,
-                               self.destination_address,
-                               0x43)
+                      send_data,
+                      self.destination_address,
+                      0x43)
         reply_data, reply_message_type, reply_destination_address = read_command_reply(self.f, True)
         if len(reply_data) == 16:
             if reply_message_type != 0x44:
                 logging.error('unexpected reply received')
-                raise unexpectedReply                
+                raise unexpectedReply
             offset = 0
             # result
             parameter_len = 2
             reply_result = ascii_decode_value(reply_data[offset:offset + parameter_len])
             offset += parameter_len
             # opcode
             parameter_len = 4
@@ -502,15 +502,15 @@
             if reply_data[0:4] != ascii_encode_value_4_bytes(0x0200):
                 logging.error('unexpected reply received')
                 raise unexpectedReply
             if reply_data[4:8] != ascii_encode_value_4_bytes(0xD600):
                 logging.error('unexpected reply received')
                 raise unexpectedReply
             # value parameter
-            state = ascii_decode_value(reply_data[12:12+4])
+            state = ascii_decode_value(reply_data[12:12 + 4])
         else:
             logging.error('unexpected reply length: %i (expected 16)', len(reply_data))
             raise unexpectedReply
         return state
 
     @retry
     def command_power_status_set(self, state):
@@ -670,29 +670,29 @@
             if reply_data[6:8] != ascii_encode_value_2_bytes(fw_type):
                 logging.error('unexpected reply received')
                 raise unexpectedReply
             for x in reply_data[8:]:
                 if x == 0:
                     break
                 version_string += chr(x)
-            return version_string                
+            return version_string
         else:
             logging.error('unexpected reply length: %i (expected >=8)', len(reply_data))
             raise unexpectedReply
 
     @retry
     def command_save_current_settings(self):
         """
         Saves all changes to the display.
 
         :return:
         """
         send_data = []
         logging.debug('')
-        send_data.extend(_encode_value_2_bytes(0x0C))
+        send_data.extend(ascii_encode_value_2_bytes(0x0C))
         write_command(self.f, send_data, self.destination_address, 0x41)
         reply_data, reply_message_type, reply_destination_address = read_command_reply(self.f, True)
         if len(reply_data) == 4:
             if reply_message_type != 0x42:
                 logging.error('unexpected reply received')
                 raise unexpectedReply
             # save current settings Command reply
@@ -738,14 +738,59 @@
             offset += parameter_len
             return status_byte, h_freq, v_freq
         else:
             logging.error('unexpected reply length: %i (expected 12)', len(reply_data))
             raise unexpectedReply
 
     @retry
+    def command_get_terminal_list(self):
+        """
+        Reads the list of supported video inputs (terminals).
+
+        :return: status_byte, number of inputs, list of inputs
+        """
+        logging.debug('')
+        send_data = []
+        input_terminal_list = []
+        send_data.extend(ascii_encode_value_4_bytes(0xCA0F))
+        send_data.extend(ascii_encode_value_2_bytes(0x00))
+        write_command(self.f, send_data, self.destination_address, 0x41)
+        reply_data, reply_message_type, reply_destination_address = read_command_reply(self.f, True)
+        if len(reply_data) > 10:
+            if reply_message_type != 0x42:
+                logging.error('unexpected reply received')
+                raise unexpectedReply
+            if reply_data[0:4] != ascii_encode_value_4_bytes(0xCB0F):
+                logging.error('unexpected reply received')
+                raise unexpectedReply
+            if reply_data[4:6] != ascii_encode_value_2_bytes(0x00):
+                logging.error('unexpected reply received')
+                raise unexpectedReply
+            offset = 6
+            # status_byte
+            parameter_len = 2
+            status_byte = ascii_decode_value(reply_data[offset:offset + parameter_len])
+            offset += parameter_len
+
+            # number of terminals
+            parameter_len = 2
+            number_of_terminals = ascii_decode_value(reply_data[offset:offset + parameter_len])
+            offset += parameter_len
+
+            # list of terminals
+            while offset < len(reply_data):
+                x = ascii_decode_value(reply_data[offset:offset + 2])
+                offset += 2
+                input_terminal_list.append(x)
+            return status_byte, number_of_terminals, input_terminal_list
+        else:
+            logging.error('unexpected reply length: %i (expected 10 or more)', len(reply_data))
+            raise unexpectedReply
+
+    @retry
     def command_date_and_time_read(self):
         """
         Reads the date and time from the display's real time clock. Note that years are 0-99.
 
         :return: PDDateTimeTuple
         """
         logging.debug('')
@@ -899,22 +944,21 @@
 
         :param program_no: zero based program number (0 - 30)
         :return: PDAdvancedScheduleTuple
         """
         #  Note: program_no is 0 based (OSD is 1 based)
         logging.debug('program_no=%i', program_no)
         send_data = []
-        assert 0 <= program_no <= 30 
+        assert 0 <= program_no <= 30
         send_data.extend(ascii_encode_value_4_bytes(0xC23D))
         send_data.extend(ascii_encode_value_2_bytes(program_no))
         write_command(self.f, send_data, self.destination_address, 0x41)
         reply_data, reply_message_type, reply_destination_address = read_command_reply(self.f, True)
 
         return self.get_advanced_schedule_from_message(0xC23D, reply_message_type, reply_data)
-        
 
     @retry
     def command_advanced_schedule_write(self, program_no, schedule_in):
         """
         Writes a schedule to the display. Note: program_no is 0 based (OSD is 1 based).
         Raises "PDCommandStatusReturnedError" if the returned status is not 'No Error'.
 
@@ -926,18 +970,18 @@
         assert 0 < schedule_in.event <= 2
 
         assert 0 <= schedule_in.hour <= 24
         assert 0 <= schedule_in.minute <= 60
         assert 0 <= schedule_in.input <= 255
         assert 0 <= schedule_in.week <= 0x7F
         assert 0 <= schedule_in.picture_mode <= 255
-        #assert 0 <= schedule_in.year <= 255
-        #assert 0 <= schedule_in.month <= 255
-        #assert 0 <= schedule_in.day <= 255
-        #assert 0 <= schedule_in.order <= 255
+        # assert 0 <= schedule_in.year <= 255
+        # assert 0 <= schedule_in.month <= 255
+        # assert 0 <= schedule_in.day <= 255
+        # assert 0 <= schedule_in.order <= 255
         assert 0 <= schedule_in.extension_1 <= 255
         assert 0 <= schedule_in.extension_2 <= 255
         assert 0 <= schedule_in.extension_3 <= 255
         logging.debug('program_no=%i hour=%i minute=%i turn_off_hour=%i turn_off_minute=%i '
                       'timer_input=%i week_setting=%i option=%i picture_mode=%i extension_1=%i extension_2=%i'
                       ' extension_3=%i extension_4=%i extension_5=%i extension_6=%i extension_7=%i',
                       schedule_in.hour,
@@ -984,60 +1028,59 @@
 
         :param program_no: zero based program number (0 - 30)
         :param enable_disable: 1 for enable and 0 for disable
         :return: PDScheduleEnableDisableTuple
         """
 
         send_data = []
-        assert 0 <= program_no <= 30 
+        assert 0 <= program_no <= 30
         send_data.extend(ascii_encode_value_4_bytes(0xC23F))
         send_data.extend(ascii_encode_value_2_bytes(program_no))
         send_data.extend(ascii_encode_value_2_bytes(enable_disable))
         write_command(self.f, send_data, self.destination_address, 0x41)
         reply_data, reply_message_type, reply_destination_address = read_command_reply(self.f, True)
 
         if len(reply_data) != 10:
             logging.error('unexpected reply length: %i (expected 10)', len(reply_data))
             raise unexpectedReply
-        
+
         if reply_message_type != 0x42:
             logging.error('unexpected reply received')
             raise unexpectedReply
 
         if reply_data[0:4] != ascii_encode_value_4_bytes(0xC33F):
             logging.error('unexpected reply received')
             raise unexpectedReply
 
-        offset = 4;
-        parameter_len = 2;
-        reply_status = ascii_decode_value(reply_data[offset:offset + parameter_len]) 
+        offset = 4
+        parameter_len = 2
+        reply_status = ascii_decode_value(reply_data[offset:offset + parameter_len])
         offset += parameter_len
 
         reply_program_no = ascii_decode_value(reply_data[offset:offset + parameter_len])
         offset += parameter_len
 
         reply_enable_disable = ascii_decode_value(reply_data[offset:offset + parameter_len])
 
         return PDScheduleEnableDisableTuple(status=reply_status,
                                             program_no=reply_program_no,
                                             enable_disable=reply_enable_disable)
-        
 
     @retry
     def command_schedule_read(self, program_no):
         """
         Reads a schedule to the display. Note: program_no is 0 based (OSD is 1 based).
 
         :param program_no: zero based program number (0 - 6)
         :return: PDScheduleTuple
         """
         #  Note: program_no is 0 based (OSD is 1 based)
         logging.debug('program_no=%i', program_no)
         send_data = []
-        assert 0 <= program_no <= 7 
+        assert 0 <= program_no <= 7
         send_data.extend(ascii_encode_value_4_bytes(0xC221))
         send_data.extend(ascii_encode_value_2_bytes(program_no))
         write_command(self.f, send_data, self.destination_address, 0x41)
         reply_data, reply_message_type, reply_destination_address = read_command_reply(self.f, True)
 
         return self.get_schedule_from_message(0xC221, reply_message_type, reply_data)
 
@@ -1116,36 +1159,36 @@
 
         :param program_no: zero based program number (0 - 30)
         :param enable_disable: 1 for enable and 0 for disable
         :return: PDScheduleEnableDisableTuple
         """
 
         send_data = []
-        assert 0 <= program_no <= 30 
+        assert 0 <= program_no <= 30
         send_data.extend(ascii_encode_value_4_bytes(0xC215))
         send_data.extend(ascii_encode_value_2_bytes(program_no))
         send_data.extend(ascii_encode_value_2_bytes(enable_disable))
         write_command(self.f, send_data, self.destination_address, 0x41)
         reply_data, reply_message_type, reply_destination_address = read_command_reply(self.f, True)
 
         if len(reply_data) != 10:
             logging.error('unexpected reply length: %i (expected 10)', len(reply_data))
             raise unexpectedReply
-        
+
         if reply_message_type != 0x42:
             logging.error('unexpected reply received')
             raise unexpectedReply
 
         if reply_data[0:4] != ascii_encode_value_4_bytes(0xC315):
             logging.error('unexpected reply received')
             raise unexpectedReply
 
-        offset = 4;
-        parameter_len = 2;
-        reply_status = ascii_decode_value(reply_data[offset:offset + parameter_len]) 
+        offset = 4
+        parameter_len = 2
+        reply_status = ascii_decode_value(reply_data[offset:offset + parameter_len])
         offset += parameter_len
 
         reply_program_no = ascii_decode_value(reply_data[offset:offset + parameter_len])
         offset += parameter_len
 
         reply_enable_disable = ascii_decode_value(reply_data[offset:offset + parameter_len])
 
@@ -1157,15 +1200,15 @@
         """
         Read the holiday from the device
 
         :param program_no: The holiday to read
         :return: PDHolidayTuple
         """
         send_data = []
-        assert 0 <= program_no <= 50 
+        assert 0 <= program_no <= 50
         send_data.extend(ascii_encode_value_4_bytes(0xCA19))
         send_data.extend(ascii_encode_value_2_bytes(0))
         send_data.extend(ascii_encode_value_2_bytes(program_no))
         write_command(self.f, send_data, self.destination_address, 0x41)
         reply_data, reply_message_type, reply_destination_address = read_command_reply(self.f, True)
 
         return self.get_holiday_from_message(program_no, 0x00, reply_message_type, reply_data)
@@ -1175,15 +1218,15 @@
         Write the holiday
 
         :param program_no: 0 based program number
         :param holiday: PDHolidayTuple
         :return: PDHolidayTuple
         """
 
-        assert 0 <= program_no <= 50 
+        assert 0 <= program_no <= 50
         send_data = []
         send_data.extend(ascii_encode_value_4_bytes(0xCA19))
         send_data.extend(ascii_encode_value_2_bytes(0x01))
         send_data.extend(ascii_encode_value_2_bytes(program_no))
         send_data.extend(ascii_encode_value_2_bytes(holiday.type))
         year = holiday.year
         if holiday.year > 2000:
@@ -1219,15 +1262,15 @@
         send_data.extend(ascii_encode_value_2_bytes(0x00))
         write_command(self.f, send_data, self.destination_address, 0x41)
         reply_data, reply_message_type, reply_destination_address = read_command_reply(self.f, True)
 
         if len(reply_data) != 8:
             logging.error('unexpected reply length: %i (expected 8)', len(reply_data))
             raise unexpectedReply
-        
+
         if reply_data[0:4] != ascii_encode_value_4_bytes(0xCB1A):
             logging.error('unexpected reply')
             raise unexpectedReply
 
         offset = 4
         parameter_len = 2
         if reply_data[offset: offset + parameter_len] != ascii_encode_value_2_bytes(0x00):
@@ -1255,79 +1298,78 @@
         send_data.extend(ascii_encode_value_2_bytes(weekend.weekend))
         write_command(self.f, send_data, self.destination_address, 0x41)
         reply_data, reply_message_type, reply_destination_address = read_command_reply(self.f, True)
 
         if len(reply_data) != 10:
             logging.error('unexpected reply length: %i (expected 10)', len(reply_data))
             raise unexpectedReply
-        
+
         if reply_data[0:4] != ascii_encode_value_4_bytes(0xCB1A):
-            logging.error('unexpedted reply')
+            logging.error('unexpected reply')
             raise unexpectedReply
 
         offset = 4
         parameter_len = 2
 
         if reply_data[offset: offset + parameter_len] != ascii_encode_value_2_bytes(0x01):
-            logging.error('unexpedted reply')
+            logging.error('unexpected reply')
             raise unexpectedReply
 
         offset += parameter_len
 
         status = ascii_decode_value(reply_data[offset: offset + parameter_len])
         offset += parameter_len
         weekend_bitfield = ascii_decode_value(reply_data[offset: offset + parameter_len])
 
         return PDWeekendTuple(status=status,
                               weekend=weekend_bitfield)
 
-
     def get_schedule_from_message(self, command, reply_message_type, reply_data):
         """
         Processes the data from a schedule read or write and returns the schedule
 
-        :param command: Command that was send (read or write)
+        :param command: Command that was sent (read or write)
         :param reply_message_type: Type of reply message received
         :param reply_data: Data received in the reply
         :return: PDScheduleTuple
         """
 
         # Initial offset is 4
         offset = 4
- 
+
         # Data length default
         data_len = 0
 
         # Reply status default
         reply_status = 0
 
         # Read Command
         # Set length and check received command
         if command == 0xC221:
             data_len = 36
             if reply_data[0:4] != ascii_encode_value_4_bytes(0xC321):
                 logging.error('unexpected reply received')
                 raise unexpectedReply
-        # Write Commmand
+        # Write Command
         # Set length, check received command and get status
         elif command == 0xC222:
             data_len = 38
             if reply_data[0:4] != ascii_encode_value_4_bytes(0xC322):
                 logging.error('unexpected reply received')
                 raise unexpectedReply
-    
+
             parameter_len = 2
             reply_status = ascii_decode_value(reply_data[offset:offset + parameter_len])
             offset += parameter_len
 
         # Check the length
         if len(reply_data) != data_len:
             logging.error('unexpected reply length: %i (expected %i)', len(reply_data), data_len)
             raise unexpectedReply
-    
+
         # Check the replay type
         if reply_message_type != 0x42:
             logging.error('unexpected reply received')
             raise unexpectedReply
 
         # Set default "null" values
         reply_hour = 24
@@ -1397,15 +1439,15 @@
         reply_extension_6 = ascii_decode_value(reply_data[offset:offset + parameter_len])
         offset += parameter_len
 
         # extension_7
         reply_extension_7 = ascii_decode_value(reply_data[offset:offset + parameter_len])
         offset += parameter_len
 
-        return PDScheduleTuple(status=0,
+        return PDScheduleTuple(status=reply_status,
                                program_no=reply_program_no,
                                turn_on_hour=reply_turn_on_hour,
                                turn_on_minute=reply_turn_on_minute,
                                turn_off_hour=reply_turn_off_hour,
                                turn_off_minute=reply_turn_off_minute,
                                timer_input=reply_timer_input,
                                week_setting=reply_week_setting,
@@ -1427,45 +1469,45 @@
         :param reply_message_type: Type of reply message received
         :param reply_data: Data received in the reply
         :return: PDAdvancedScheduleTuple
         """
 
         # Initial offset is 4 
         offset = 4
-   
+
         # Data length default
         data_len = 0
-    
+
         # Reply status default
         reply_status = 0
-    
+
         # Read Command
         # Set length and check received command
         if command == 0xC23D:
             data_len = 34
             if reply_data[0:4] != ascii_encode_value_4_bytes(0xC33D):
                 logging.error('unexpected reply received')
                 raise unexpectedReply
-        # Write Commmand
+        # Write Command
         # Set length, check received command and get status
         elif command == 0xC23E:
             data_len = 36
             if reply_data[0:4] != ascii_encode_value_4_bytes(0xC33E):
                 logging.error('unexpected reply received')
                 raise unexpectedReply
-    
+
             parameter_len = 2
             reply_status = ascii_decode_value(reply_data[offset:offset + parameter_len])
             offset += parameter_len
 
         # Check the length
         if len(reply_data) != data_len:
             logging.error('unexpected reply length: %i (expected %i)', len(reply_data), data_len)
             raise unexpectedReply
-    
+
         # Check the replay type
         if reply_message_type != 0x42:
             logging.error('unexpected reply received')
             raise unexpectedReply
 
         # Set default "null" values
         reply_hour = 24
@@ -1492,15 +1534,15 @@
         offset += parameter_len
         reply_minute = ascii_decode_value(reply_data[offset:offset + parameter_len])
         offset += parameter_len
 
         # input
         reply_input = ascii_decode_value(reply_data[offset:offset + parameter_len])
         offset += parameter_len
- 
+
         # week
         reply_week = ascii_decode_value(reply_data[offset:offset + parameter_len])
         offset += parameter_len
 
         # type
         reply_type = ascii_decode_value(reply_data[offset:offset + parameter_len])
         offset += parameter_len
@@ -1537,90 +1579,91 @@
         offset += parameter_len
 
         # extension_3
         reply_extension_3 = ascii_decode_value(reply_data[offset:offset + parameter_len])
         offset += parameter_len
 
         return PDAdvancedScheduleTuple(status=reply_status,
-                                   program_no=reply_program_no,
-                                   event=reply_event,
-                                   hour=reply_hour,
-                                   minute=reply_minute,
-                                   input=reply_input,
-                                   week=reply_week,
-                                   type=reply_type,
-                                   picture_mode=reply_picture_mode,
-                                   year=reply_year,
-                                   month=reply_month,
-                                   day=reply_day,
-                                   order=reply_order,
-                                   extension_1=reply_extension_1,
-                                   extension_2=reply_extension_2,
-                                   extension_3=reply_extension_3)
-
+                                       program_no=reply_program_no,
+                                       event=reply_event,
+                                       hour=reply_hour,
+                                       minute=reply_minute,
+                                       input=reply_input,
+                                       week=reply_week,
+                                       type=reply_type,
+                                       picture_mode=reply_picture_mode,
+                                       year=reply_year,
+                                       month=reply_month,
+                                       day=reply_day,
+                                       order=reply_order,
+                                       extension_1=reply_extension_1,
+                                       extension_2=reply_extension_2,
+                                       extension_3=reply_extension_3)
 
-    def get_holiday_from_message(this, program_no, command, reply_message_type, reply_data):
+    def get_holiday_from_message(self, program_no, command, reply_message_type, reply_data):
         """
         Processes the data from a holiday read or write and returns the holiday
       
         :param program_no: The holiday number
         :param command: Command that was sent (read or write)
         :param reply_message_type: Type of reply message received
         :param reply_data: Data received in the reply
         :return: PDHolidayTuple
         """
         # Initial offset is 6 
         offset = 6
-   
+
         # Data length default
         data_len = 0
-    
+
         # Reply status default
         reply_status = 0
-    
+
         # Read Command
         # Set length and check received command
         if command == 0x00:
             data_len = 24
-            if reply_data[0:4] != ascii_encode_value_4_bytes(0xCB19) and reply_data[5:6] != ascii_encode_value_2_bytes(0x00):
+            if reply_data[0:4] != ascii_encode_value_4_bytes(0xCB19) and reply_data[5:6] != ascii_encode_value_2_bytes(
+                    0x00):
                 logging.error('1 unexpected reply received')
                 raise unexpectedReply
-        # Write Commmand
+        # Write Command
         # Set length, check received command and get status
         elif command == 0x01:
             data_len = 26
             print("reply_data[5:6]: ", reply_data[5:6])
-            if reply_data[0:4] != ascii_encode_value_4_bytes(0xCB19) and reply_data[4:5] != ascii_encode_value_2_bytes(0x01):
+            if reply_data[0:4] != ascii_encode_value_4_bytes(0xCB19) and reply_data[4:5] != ascii_encode_value_2_bytes(
+                    0x01):
                 logging.error('2 unexpected reply received')
                 raise unexpectedReply
-    
+
             parameter_len = 2
             reply_status = ascii_decode_value(reply_data[offset:offset + parameter_len])
             offset += parameter_len
 
         # Check the length
         if len(reply_data) != data_len:
             logging.error('3 unexpected reply length: %i (expected %i)', len(reply_data), data_len)
             raise unexpectedReply
-    
+
         # Check the reply type
         if reply_message_type != 0x42:
             logging.error('4 unexpected reply received')
             raise unexpectedReply
 
         # Parameter length is 2 for all the params.  
         parameter_len = 2
 
         reply_id = ascii_decode_value(reply_data[offset: offset + parameter_len])
         offset += parameter_len
-   
-        if (reply_id != program_no):
+
+        if reply_id != program_no:
             logging.error('5 unexpected reply received')
             raise unexpectedReply
- 
+
         reply_type = ascii_decode_value(reply_data[offset: offset + parameter_len])
         offset += parameter_len
 
         reply_year = ascii_decode_value(reply_data[offset: offset + parameter_len])
         if reply_year > 0:
             reply_year += 2000
 
@@ -1631,15 +1674,15 @@
 
         # Initialize Values
         reply_day = 0
         reply_end_month = 0
         reply_end_day = 0
         reply_week_of_month = 0
         reply_day_of_week = 0
-        
+
         # Single Date
         if reply_type & 0x02:
             reply_day = ascii_decode_value(reply_data[offset: offset + parameter_len])
             offset += parameter_len
 
             # Date Range
             if reply_type & 0x01:
@@ -1662,16 +1705,15 @@
                               type=reply_type,
                               year=reply_year,
                               month=reply_month,
                               day=reply_day,
                               week_of_month=reply_week_of_month,
                               day_of_week=reply_day_of_week,
                               end_month=reply_end_month,
-                              end_day=reply_end_day)  
-         
+                              end_day=reply_end_day)
 
     @retry
     def command_lan_mac_address_read(self):
         """
         Reads the LAN MAC address of the display.
         Raises "PDCommandStatusReturnedError" if the returned status is not 'No Error'.
 
@@ -1704,15 +1746,15 @@
                 raise unexpectedReply
             offset += 2
             # IPV
             parameter_len = 2
             ipv = ascii_decode_value(reply_data[offset:offset + parameter_len])
             offset += parameter_len
             mac = ""
-            while offset+1 < len(reply_data):
+            while offset + 1 < len(reply_data):
                 x = ascii_decode_value(reply_data[offset:offset + 2])
                 mac += format(x, "x")
                 offset += 2
                 if offset < len(reply_data):
                     mac += "-"
             return mac, ipv
         else:
@@ -1754,15 +1796,15 @@
                 raise unexpectedReply
             offset += 2
             # IPV
             parameter_len = 2
             ipv = ascii_decode_value(reply_data[offset:offset + parameter_len])
             offset += parameter_len
             ip = ""
-            while offset+1 < len(reply_data):
+            while offset + 1 < len(reply_data):
                 x = ascii_decode_value(reply_data[offset:offset + 2])
                 ip += format(x, "d")
                 offset += 2
                 if offset < len(reply_data):
                     ip += "."
             return ip, ipv
         else:
@@ -2544,15 +2586,15 @@
         :return: asset_string reply
         """
         logging.debug('offset=%i in_string=%s', offset, in_string)
         send_data = []
         asset_string = ""
         assert 0 <= offset <= 64
         assert 0 <= len(in_string) <= 32
-        assert offset+len(in_string) <= 64
+        assert offset + len(in_string) <= 64
         send_data.extend(ascii_encode_value_4_bytes(0xC00E))
         send_data.extend(ascii_encode_value_2_bytes(offset))
         for x in in_string:
             send_data.extend([ord(x)])
         # pad with null
         for i in range(len(in_string), 32):
             send_data.extend([0])
@@ -2929,15 +2971,15 @@
         assert len(password) == 4
         logging.debug('secure_mode=%i password=%s', secure_mode, password)
         send_data = []
         send_data.extend(ascii_encode_value_4_bytes(0xC21D))
         send_data.extend(ascii_encode_value_2_bytes(secure_mode))
         for char in password:
             assert 0x30 <= ord(char) <= 0x39
-            send_data.extend(ascii_encode_value_2_bytes(ord(char)-0x30))
+            send_data.extend(ascii_encode_value_2_bytes(ord(char) - 0x30))
         write_command(self.f, send_data, self.destination_address, 0x41)
         reply_data, reply_message_type, reply_destination_address = read_command_reply(self.f, True)
         if len(reply_data) == 8:
             if reply_message_type != 0x42:
                 logging.error('unexpected reply received')
                 raise unexpectedReply
             if reply_data[0:4] != ascii_encode_value_4_bytes(0xC31D):
@@ -2981,15 +3023,15 @@
             logging.error('unexpected reply length: %i (expected 8)', len(reply_data))
             raise unexpectedReply
         return status
 
     @retry
     def command_get_proof_of_play_status(self):
         """
-        Reads the current proof of play status from the the display.
+        Reads the current proof of play status from the display.
 
         :return: PDProofOfPlayStatusTuple
         """
         logging.debug('')
         send_data = []
         send_data.extend(ascii_encode_value_4_bytes(0xCA15))
         send_data.extend(ascii_encode_value_2_bytes(0x02))
@@ -3016,15 +3058,15 @@
         else:
             logging.error('unexpected reply length: %i (expected 18)', len(reply_data))
             raise unexpectedReply
 
     @retry
     def command_get_proof_of_play_current(self):
         """
-        Reads the latest proof of play log from the the display.
+        Reads the latest proof of play log from the display.
         Raises "PDCommandStatusReturnedError" if the returned status is not 'No Error'.
 
         :return: PDProofOfPlayLogItemTuple
         """
         logging.debug('')
         send_data = []
         send_data.extend(ascii_encode_value_4_bytes(0xCA15))
@@ -3112,21 +3154,21 @@
             parameter_len = 2
             reply_reserved_2 = ascii_decode_value(reply_data[offset:offset + parameter_len])
             offset += parameter_len
 
             parameter_len = 2
             reply_reserved_3 = ascii_decode_value(reply_data[offset:offset + parameter_len])
             offset += parameter_len
-            
-            return PDProofOfPlayLogItemTuple(status=reply_status, 
+
+            return PDProofOfPlayLogItemTuple(status=reply_status,
                                              log_number=reply_log_number,
-                                             input=reply_input, 
+                                             input=reply_input,
                                              signal_h_resolution=reply_signal_h_resolution,
-                                             signal_v_resolution=reply_signal_v_resolution, 
-                                             audio_input=reply_audio_input, 
+                                             signal_v_resolution=reply_signal_v_resolution,
+                                             audio_input=reply_audio_input,
                                              audio_input_status=reply_audio_input_status,
                                              picture_status=reply_picture_status,
                                              audio_status=reply_audio_status,
                                              year=reply_year,
                                              month=reply_month,
                                              day=reply_day,
                                              hour=reply_hour,
@@ -3138,23 +3180,23 @@
         else:
             logging.error('unexpected reply length: %i (expected 50)', len(reply_data))
             raise unexpectedReply
 
     @retry
     def command_get_proof_of_play_number_to_number(self, from_number, to_number):
         """
-        Reads a specific proof of play log from the the display.
+        Reads a specific proof of play log from the display.
         Note: only support reading 1 log at a time.
         Raises "PDCommandStatusReturnedError" if the returned status is not 'No Error'.
 
         :param from_number:
         :param to_number:
         :return:
         """
-        assert from_number == to_number   # only support reading 1 log at a time
+        assert from_number == to_number  # only support reading 1 log at a time
         assert 0 <= from_number <= 0xffff
         logging.debug('from_number=%i to_number=%i', from_number, to_number)
         send_data = []
         send_data.extend(ascii_encode_value_4_bytes(0xCA15))
         send_data.extend(ascii_encode_value_2_bytes(0x03))
         send_data.extend(ascii_encode_value_4_bytes(from_number))
         send_data.extend(ascii_encode_value_4_bytes(to_number))
@@ -3243,20 +3285,20 @@
             parameter_len = 2
             reply_reserved_2 = ascii_decode_value(reply_data[offset:offset + parameter_len])
             offset += parameter_len
 
             parameter_len = 2
             reply_reserved_3 = ascii_decode_value(reply_data[offset:offset + parameter_len])
             offset += parameter_len
-            return PDProofOfPlayLogItemTuple(status=reply_status, 
+            return PDProofOfPlayLogItemTuple(status=reply_status,
                                              log_number=reply_log_number,
-                                             input=reply_input, 
+                                             input=reply_input,
                                              signal_h_resolution=reply_signal_h_resolution,
-                                             signal_v_resolution=reply_signal_v_resolution, 
-                                             audio_input=reply_audio_input, 
+                                             signal_v_resolution=reply_signal_v_resolution,
+                                             audio_input=reply_audio_input,
                                              audio_input_status=reply_audio_input_status,
                                              picture_status=reply_picture_status,
                                              audio_status=reply_audio_status,
                                              year=reply_year,
                                              month=reply_month,
                                              day=reply_day,
                                              hour=reply_hour,
@@ -3312,15 +3354,15 @@
         return capability_string
 
     @retry
     def command_tile_matrix_profile_contents_write(self, settings):
         """
         Saves Tile Matrix settings into a memory so that they can be recalled instantly.
 
-        :param settings PDTileMatrixProfileTuple
+        :param settings: PDTileMatrixProfileTuple
         profile_number: memory location to store profile settings in (0-4)
         h_monitors: number of columns (1-10)
         v_monitors: number of rows (1-10)
         position: position of this display (from top left) (1-100)
         tile_comp: use tile compensation (1=off 2=on)
         :return:
         """
@@ -3603,63 +3645,63 @@
             offset = 8
             # profile_number
             parameter_len = 2
             profile_number = ascii_decode_value(reply_data[offset:offset + parameter_len])
             offset += parameter_len
             # pip_pbp_mode
             pip_pbp_mode = ascii_decode_value(reply_data[offset:offset + parameter_len])
-            offset += parameter_len        
+            offset += parameter_len
             # picture1_input
             picture1_input = ascii_decode_value(reply_data[offset:offset + parameter_len])
             offset += parameter_len
             # picture2_input
             picture2_input = ascii_decode_value(reply_data[offset:offset + parameter_len])
             offset += parameter_len
             # picture3_input
             picture3_input = ascii_decode_value(reply_data[offset:offset + parameter_len])
             offset += parameter_len
             # picture4_input
             picture4_input = ascii_decode_value(reply_data[offset:offset + parameter_len])
-            offset += parameter_len            
+            offset += parameter_len
             # picture1_size
             picture1_size = ascii_decode_value(reply_data[offset:offset + parameter_len])
             offset += parameter_len
             # picture2_size
             picture2_size = ascii_decode_value(reply_data[offset:offset + parameter_len])
             offset += parameter_len
             # picture3_size
             picture3_size = ascii_decode_value(reply_data[offset:offset + parameter_len])
             offset += parameter_len
             # picture4_size
             picture4_size = ascii_decode_value(reply_data[offset:offset + parameter_len])
-            offset += parameter_len            
+            offset += parameter_len
             # picture1_aspect
             picture1_aspect = ascii_decode_value(reply_data[offset:offset + parameter_len])
             offset += parameter_len
             # picture2_aspect
             picture2_aspect = ascii_decode_value(reply_data[offset:offset + parameter_len])
             offset += parameter_len
             # picture3_aspect
             picture3_aspect = ascii_decode_value(reply_data[offset:offset + parameter_len])
             offset += parameter_len
             # picture4_aspect
             picture4_aspect = ascii_decode_value(reply_data[offset:offset + parameter_len])
-            offset += parameter_len            
+            offset += parameter_len
             # picture1_h_position
             picture1_h_position = ascii_decode_value(reply_data[offset:offset + parameter_len])
             offset += parameter_len
             # picture2_h_position
             picture2_h_position = ascii_decode_value(reply_data[offset:offset + parameter_len])
             offset += parameter_len
             # picture3_h_position
             picture3_h_position = ascii_decode_value(reply_data[offset:offset + parameter_len])
             offset += parameter_len
             # picture4_h_position
             picture4_h_position = ascii_decode_value(reply_data[offset:offset + parameter_len])
-            offset += parameter_len            
+            offset += parameter_len
             # picture1_v_position
             picture1_v_position = ascii_decode_value(reply_data[offset:offset + parameter_len])
             offset += parameter_len
             # picture2_v_position
             picture2_v_position = ascii_decode_value(reply_data[offset:offset + parameter_len])
             offset += parameter_len
             # picture3_v_position
@@ -3850,15 +3892,15 @@
         :return: a list of values in 'c corresponding to each sensor
         """
         logging.debug('')
         temperatures = []
         reply = self.command_get_parameter(OPCODE_SELECT_TEMPERATURE_SENSOR)
         if reply.result == 0x00:  # supported
             for x in range(0, reply.max_value):
-                self.command_set_parameter(OPCODE_SELECT_TEMPERATURE_SENSOR, x+1)
+                self.command_set_parameter(OPCODE_SELECT_TEMPERATURE_SENSOR, x + 1)
                 temperatures.append(
                     self.command_get_parameter(OPCODE_READ_TEMPERATURE_SENSOR_READ_ONLY).current_value / 2.0)
             return temperatures
         return
 
     def helper_get_fan_statuses(self):
         """
@@ -3867,15 +3909,15 @@
         :return: a list of the text status of each available fan
         """
         logging.debug('')
         status = []
         reply = self.command_get_parameter(OPCODE_FAN__FAN_SELECT)
         if reply.result == 0x00:  # supported
             for x in range(0, reply.max_value):
-                self.command_set_parameter(OPCODE_FAN__FAN_SELECT, x+1)
+                self.command_set_parameter(OPCODE_FAN__FAN_SELECT, x + 1)
                 value = self.command_get_parameter(OPCODE_FAN__FAN_STATUS_READ_ONLY).current_value
                 if value in DISPLAY_FAN_STATUS:
                     status.append(DISPLAY_FAN_STATUS[value])
                 else:
                     status.append("Unknown")
             return status
         return
@@ -3883,15 +3925,15 @@
     def helper_self_diagnosis_status_text(self):
         """
         Performs "command_self_diagnosis_status_read" and formats the reply into
         a string of the decoded error code(s).
 
         :return: single string with decoded error codes separated by ';'
         """
-        logging.debug('')
+        # logging.debug('')
         text = ""
         result_codes = self.command_self_diagnosis_status_read()
         for code in result_codes:
             try:
                 text += (DISPLAY_DIAGNOSTIC_ERROR_CODES[code]) + "; "
             except KeyError:
                 text += ("Unknown error code - " + hex(code)) + "; "
@@ -3902,16 +3944,16 @@
         Performs "command_get_timing_report" and formats into a readable string.
 
         :return: string with timing information
         """
         logging.debug('')
         text = ""
         status_byte, h_freq, v_freq = self.command_get_timing_report()
-        text += "H Frequency: " + str(h_freq/100.0) + " kHz, "
-        text += "V Frequency: " + str(v_freq/100.0) + " Hz, "
+        text += "H Frequency: " + str(h_freq / 100.0) + " kHz, "
+        text += "V Frequency: " + str(v_freq / 100.0) + " Hz, "
         if status_byte & 0x80:
             text += "Out of range, "
         if status_byte & 0x40:
             text += "Unstable, "
         if status_byte & 0x02:
             text += "+H Sync, "
         else:
@@ -3984,15 +4026,15 @@
         Helper function for helper_date_and_time_write that takes a 'datetime'.
 
         :param in_datetime: a Python datetime
         :param in_daylight_savings:
         :return: same as command_date_and_time_write
         """
         logging.debug('')
-        param = PDDateTimeTuple(year=in_datetime.year-2000,
+        param = PDDateTimeTuple(year=in_datetime.year - 2000,
                                 month=in_datetime.month,
                                 day=in_datetime.day,
                                 weekday=0,
                                 hour=in_datetime.hour,
                                 minute=in_datetime.minute,
                                 daylight_savings=in_daylight_savings,
                                 status=0)
@@ -4005,15 +4047,15 @@
 
         :param in_datetime: a Python datetime
         :return: same as command_date_and_time_write
         """
         logging.debug('')
         value = self.command_date_and_time_read()
 
-        param = PDDateTimeTuple(year=in_datetime.year-2000,
+        param = PDDateTimeTuple(year=in_datetime.year - 2000,
                                 month=in_datetime.month,
                                 day=in_datetime.day,
                                 weekday=0,
                                 hour=in_datetime.hour,
                                 minute=in_datetime.minute,
                                 daylight_savings=value.daylight_savings,
                                 status=0)
@@ -4075,28 +4117,30 @@
         :return: a list of firmware version strings
         """
         logging.debug('')
         reply = []
         for x in range(0, 4):
             try:
                 reply.append(self.command_firmware_version_read(x).rstrip())
-            except (PDNullMessageReplyError,  PDCommandNotSupportedError):
+            except (PDNullMessageReplyError, PDCommandNotSupportedError):
                 # older monitor may not support, so try to read from capability string
                 cap_string = self.helper_capabilities_request()
-                index_start = string.find(cap_string, "mpu_ver(")
-                index_end = string.find(cap_string, ")", index_start)
+                # index_start = string.find(cap_string, "mpu_ver(")
+                index_start = cap_string.find("mpu_ver(")
+                index_end = cap_string.find(")", index_start)
+                # index_end = string.find(cap_string, ")", index_start)
                 if index_start > 0 and index_end > 0:
-                    reply.append(cap_string[index_start+len("mpu_ver("):index_end])
+                    reply.append(cap_string[index_start + len("mpu_ver("):index_end])
                     return reply
                 raise PDCommandNotSupportedError
         return reply
 
     def helper_get_proof_of_play_current(self):
         """
-        Reads the latest proof of play log from the the display and returns the date & time as a Python datetime.
+        Reads the latest proof of play log from the display and returns the date & time as a Python datetime.
 
         :return: PDHelperProofOfPlayLogItemTuple
         """
         logging.debug('')
         reply = self.command_get_proof_of_play_current()
         return PDHelperProofOfPlayLogItemTuple(status=reply.status,
                                                log_number=reply.log_number,
@@ -4135,74 +4179,73 @@
                                                audio_status=reply.audio_status,
                                                date_time=datetime.datetime(reply.year, reply.month, reply.day,
                                                                            reply.hour, reply.minute),
                                                reserved_1=reply.reserved_1,
                                                reserved_2=reply.reserved_2,
                                                reserved_3=reply.reserved_3)
 
-
     def helper_read_schedules(self):
         """
         Helper function to read all the schedules and return them as a list of schedules
 
         :return: A list of PDScheduleTuple
         """
 
         reply = []
-        for x in range (1, 7):
+        for x in range(1, 7):
             reply.append(self.command_schedule_read(x))
 
         return reply
 
     def helper_read_advanced_schedules(self):
         """
         Helper function to read all the advanced schedules and return them as a list of schedules
 
         :return: A list of PDAdvancedScheduleTuple
         """
 
         reply = []
-        for x in range (1, 30):
+        for x in range(1, 30):
             reply.append(self.command_advanced_schedule_read(x))
 
         return reply
 
     def helper_read_holidays(self):
         """
-        Helper function to reall all the holidays and return them as a list of holidays
+        Helper function to read all the holidays and return them as a list of holidays
 
         :return: A list of PDHolidayTuple
         """
 
         reply = []
-        for x in range (1, 50):
+        for x in range(1, 50):
             reply.append(self.command_holiday_read(x))
 
         return reply
 
     def helper_advanced_schedule_is_empty(self, schedule):
         """
-        Helper function to determin if the schedule is empty
+        Helper function to determine if the schedule is empty
 
         :param schedule: Schedule
-        :return: True if the scheule is empty
+        :return: True if the schedule is empty
         """
 
         reply = False
         if schedule.hour == 24 and schedule.minute == 60:
             reply = True
 
         return reply
-    
+
     def helper_advanced_schedule_is_enabled(self, schedule):
         """
-        Helper function to determin if the schedule is enabled
+        Helper function to determine if the schedule is enabled
 
         :param schedule: Schedule
-        :return: True if the scheule is enabled
+        :return: True if the schedule is enabled
         """
 
         reply = False
         if schedule.type & 0x04:
             reply = True
 
         return reply
@@ -4210,185 +4253,185 @@
     def helper_advanced_schedule_is_every_day(self, schedule):
         """
         Helper function to determine if the schedule type is Every Day
 
         :param schedule: Schedule 
         :return: True if the schedule type is every day.
         """
-   
+
         reply = False
         if schedule.type & 0x01:
             reply = True
 
         return reply
 
     def helper_advanced_schedule_is_every(self, schedule):
         """
         Helper function to determine if the schedule type is Every 
 
         :param schedule: Schedule 
         :return: True if the schedule type is every 
         """
-   
+
         reply = False
         if schedule.type & 0x02 and schedule.week != 0:
             reply = True
 
         return reply
 
     def helper_advanced_schedule_is_specific_days(self, schedule):
         """
         Helper function to determine if the schedule type is Specific Days 
 
         :param schedule: Schedule 
         :return: True if the schedule type is specific days 
         """
-   
+
         reply = False
         if schedule.type & 0x02 and schedule.week == 0:
             reply = True
 
         return reply
 
     def helper_advanced_schedule_is_weekdays(self, schedule):
         """
         Helper function to determine if the schedule type is Weekdays
 
         :param schedule: Schedule 
         :return: True if the schedule type is Weekdays
         """
-   
+
         reply = False
-        if schedule.type & 0x08: 
+        if schedule.type & 0x08:
             reply = True
 
         return reply
- 
+
     def helper_advanced_schedule_is_weekends(self, schedule):
         """
         Helper function to determine if the schedule type is Weekends
 
         :param schedule: Schedule 
         :return: True if the schedule type is Weekends
         """
-   
+
         reply = False
-        if schedule.type & 0x10: 
+        if schedule.type & 0x10:
             reply = True
 
         return reply
- 
+
     def helper_advanced_schedule_is_holidays(self, schedule):
         """
         Helper function to determine if the schedule type is holidays
 
         :param schedule: Schedule 
         :return: True if the schedule type is holidays
         """
-   
+
         reply = False
-        if schedule.type & 0x20: 
+        if schedule.type & 0x20:
             reply = True
 
         return reply
- 
+
     def helper_advanced_schedule_is_one_day(self, schedule):
         """
         Helper function to determine if the schedule type is one_day
 
         :param schedule: Schedule 
         :return: True if the schedule type is one_day
         """
-   
+
         reply = False
-        if schedule.type & 0x40: 
+        if schedule.type & 0x40:
             reply = True
 
         return reply
- 
+
     def helper_advanced_schedule_type_string(self, schedule):
         """
         Helper function to return the type string
 
         :param schedule: Schedule
         :return: Type string
         """
 
-        str = ""
+        text = ""
         if schedule.type & 0x01:
-            str = "Every Day"
+            text = "Every Day"
         elif schedule.type & 0x02:
             if schedule.week != 0:
-                str = "Every "
+                text = "Every "
             else:
-                str = "Specific Days"
+                text = "Specific Days"
         elif schedule.type & 0x08:
-            str = "Weekdays"
+            text = "Weekdays"
         elif schedule.type & 0x10:
-            str = "Weekends"
+            text = "Weekends"
         elif schedule.type & 0x20:
-            str = "Holidays"
+            text = "Holidays"
         elif schedule.type & 0x40:
-            str = "One Day on "
+            text = "One Day on "
 
-        return str
+        return text
 
     def helper_advanced_schedule_week_string(self, week):
         """
         Helper function to get the week string
 
         :param week: Schedule week
         :return: Week String such as "Mon, Tues, Fri"
         """
 
-        str = ""
+        text = ""
         if week & 0x01:
-            str += "Mon"
+            text += "Mon"
         if week & 0x02:
-            if str != "":
-                str += ", "
-            str += "Tues" 
+            if text != "":
+                text += ", "
+            text += "Tues"
         if week & 0x04:
-            if str != "":
-                str += ", "
-            str += "Wed"
+            if text != "":
+                text += ", "
+            text += "Wed"
         if week & 0x08:
-            if str != "":
-                str += ", "
-            str += "Thurs"
+            if text != "":
+                text += ", "
+            text += "Thurs"
         if week & 0x10:
-            if str != "":
-                str != ", "
-            str += "Fri"
+            if text != "":
+                text += ", "
+            text += "Fri"
         if week & 0x20:
-            if str != "":
-                str += ", "
-            str += "Sat"
+            if text != "":
+                text += ", "
+            text += "Sat"
         if week & 0x40:
-            if str != "":
-                str += ", "
-            str += "Sun"
+            if text != "":
+                text += ", "
+            text += "Sun"
 
-        return str;
+        return text
 
     def helper_advanced_schedule_set_type(self, type, enable):
         """
         Set the schedule type.  If enable is True, then also include
         the enable bit in the schedule.
 
         :param type: Type of schedule.  See the class PDSchedule for types
         :param enable: If True, also enable the schedule
         :return: The Schedule Type
         """
 
-        schedType = type;
-        if enable == True:
-            schedType += PDSchedule.Enabled
+        schedule_type = type
+        if enable:
+            schedule_type += PDSchedule.Enabled
 
-        return schedType
+        return schedule_type
 
     def helper_advanced_schedule_set_week(self, week):
         """
         Set the week.
 
         :param week: Array of Days to set
         :return: The week
```

### Comparing `nec_pd_sdk-18.2.231/nec_pd_sdk/opcode_decoding.py` & `nec_pd_sdk-23.8.21/nec_pd_sdk/opcode_decoding.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """opcode_decoding.py - Tools for working with opcodes and opcode values
+Revision: 230717
 """
 # Reads and parses a text file containing a list of opcodes and their
 # textual "nice names". For opcodes that have specific / discrete value
 # settings, the values and textual "nice names" for each are included.
 # Once the file is parsed, the resulting dictionaries can be accessed
 # using the included helper functions.
 #
 # Copyright (C) 2016-18 NEC Display Solutions, Ltd
-# written by Will Hollingworth <whollingworth at necdisplay.com>
+# Copyright (C) 2023 Sharp NEC Display Solutions, Ltd
+# written by Will Hollingworth <William.Hollingworth at sharpusa.com>
 # See LICENSE.rst for details.
 #
 
 import os
 
 opcode_to_name_dict = dict()
 opcode_values_to_name_dict = dict()
@@ -46,15 +48,15 @@
                         offset = 3
                         vcp_values = dict()
                         while offset+1 < len(words):  # read the opcode's pairs of int values and value text
                             vcp_values[int(words[offset])] = words[offset+1][1:-1]
                             offset += 2
                         opcode_values_to_name_dict[opcode] = vcp_values
                 except ValueError:
-                    print ("convert error")
+                    print("convert error")
     assert len(opcode_to_name_dict) > 0
     assert len(opcode_values_to_name_dict) > 0
     return
 
 
 def opcode_to_nice_name(opcode):
     """
@@ -72,15 +74,15 @@
         return opcode_to_name_dict[opcode]
     return
 
 
 def nice_name_to_opcode(name):
     """
     Given a text nice name it returns a numerical opcode (if exists)
-    Note: string must be an exact match (case sensitive)
+    Note: string must be an exact match (case-sensitive)
 
     Use this to lookup the opcode from the textual name of an opcode.
     e.g. "Input" -> 0x0060
 
     :param name: the text "nice name" of the opcode to lookup
     :return: a numerical value for the opcode (if exists)
     """
@@ -111,15 +113,15 @@
     return
 
 
 def opcode_nice_value_name_to_value(opcode, nice_value_name):
     """
     Given a numerical opcode and a string with the nice name of the value,
       it returns the value (if exists)
-    Note: "nice_value_name" string must be an exact match (case sensitive)
+    Note: "nice_value_name" string must be an exact match (case-sensitive)
 
     Use this to lookup the value for a particular opcode given the nice name of the value
     e.g. opcode 0x0060 (Input) with "VGA" -> value 1
 
     :param opcode: a numerical value for the opcode
     :param nice_value_name: the text "nice name" of the opcode value
     :return: a numerical value for the opcode value (if exists)
@@ -131,17 +133,17 @@
         if nice_value_name in name_dict:
             return name_dict[nice_value_name]
     return
 
 
 def get_opcode_list():
     """
-    Use this to get a sorted numerical list of all of the known opcodes
+    Use this to get a sorted numerical list of all the known opcodes
 
-    :return: A numerical list of all of the known opcodes
+    :return: A numerical list of all the known opcodes
     """
     assert len(opcode_to_name_dict)  # forgot to load_opcode_dict
     keys = list(opcode_to_name_dict.keys())
     keys.sort()
     return keys
```

### Comparing `nec_pd_sdk-18.2.231/nec_pd_sdk/protocol.py` & `nec_pd_sdk-23.8.21/nec_pd_sdk/protocol.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # -*- coding: utf-8 -*-
 """protocol.py - Lower level protocol handling functions for communicating with NEC large-screen displays
-Revision: 170322
+Revision: 230717
 """
 #
 #
 # Copyright (C) 2016-18 NEC Display Solutions, Ltd
-# written by Will Hollingworth <whollingworth at necdisplay.com>
+# Copyright (C) 2023 Sharp NEC Display Solutions, Ltd
+# written by Will Hollingworth <William.Hollingworth at sharpusa.com>
 # See LICENSE.rst for details.
 #
 
 
 import logging
 
 
@@ -32,14 +33,15 @@
 class PDCommandStatusReturnedError(PDError):
     pass
 
 
 class PDCommandNotSupportedError(PDError):
     pass
 
+
 unexpectedReply = PDUnexpectedReplyError('Unexpected reply received')
 nullMessageReply = PDNullMessageReplyError('NULL message reply (monitor busy or unknown command)')
 replyTimeout = PDTimeoutError('Reply timeout (no reply within timeout period)')
 commandStatusReturnedError = PDCommandStatusReturnedError('Command status returned error')
 
 
 def write_command(f, data, destination_address, message_type):
@@ -70,19 +72,19 @@
     for x in output_data[1:]:
         checksum ^= x
     # print "checksum:", hex(checksum)
     output_data.append(checksum)
     # delimiter
     output_data.append(0x0D)
     # print "output_data:", output_data
-    # send_data(f, output_data)
+    # send__data(f, output_data)
     for x in output_data:
         logging.debug('output_data: %02xh', x)
     #   print "output_data: ", hex(x)
-    send_data(f, bytearray(output_data))
+    send__data(f, bytearray(output_data))
     return
 
 
 def read_command_reply(f, destination_reply_is_monitor_id):
     payload_data = []
     checksum = 0
     # SOH
@@ -116,19 +118,19 @@
     checksum ^= c
     # message length (2 bytes)
     c = read_data(f, 2)
     message_length = int(c, 16)
     logging.debug('message_length=%02xh', message_length)
     # Python3 is read as int, so don't need the ord
     # Python2 needs the ord
-    if (isinstance(c[0], int)):
+    if isinstance(c[0], int):
         checksum ^= c[0]
     else:
         checksum ^= ord(c[0])
-    if (isinstance(c[0], int)):
+    if isinstance(c[0], int):
         checksum ^= c[1]
     else:
         checksum ^= ord(c[1])
     # message payload
     if message_length > 0:
         c = read_character_as_ord(f)
         if c != 0x02:
@@ -195,36 +197,36 @@
 def ascii_decode_value(data):
     value = 0
     for byte in data:
         value *= 16
         if 48 <= byte <= 57:
             value += byte - 48
         elif 65 <= byte <= 72:
-                value += byte - 65 + 10
+            value += byte - 65 + 10
         elif 97 <= byte <= 104:
-                value += byte - 97 + 10
+            value += byte - 97 + 10
         else:
             # invalid value
             logging.error('invalid hex character: %i', byte)
             value = 0
     return value
 
 
-def send_data(f, data):
+def send__data(f, data):
     f.sendall(data)
 
 
 def read_data(f, length):
     try:
         reply = f.recv(length)
         if len(reply) == 0:
             logging.error('replyTimeout')
             raise replyTimeout
         return reply
-    except:
+    except Exception:
         raise replyTimeout
 
 
 def read_character_as_ord(f):
     return ord(read_data(f, 1))
```

### Comparing `nec_pd_sdk-18.2.231/nec_pd_sdk.egg-info/PKG-INFO` & `nec_pd_sdk-23.8.21/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
-Name: nec-pd-sdk
-Version: 18.2.231
+Name: nec_pd_sdk
+Version: 23.8.21
 Summary: NEC PD SDK
 Home-page: https://github.com/necsoftware/necpdsdk
 Author: NEC Display Solutions, Ltd.
 Author-email: techsupport@necdisplay.com
 License: MIT
-Download-URL: https://github.com/NECDisplaySolutions/necpdsdk.git
+Download-URL: https://github.com/SharpNECDisplaySolutions/necpdsdk.git
 Description: NEC PD SDK
         =======================
         
         Python library interface for communicating via LAN or RS232 with NEC large-screen displays.  
         
         
         Documentation
@@ -27,15 +27,17 @@
         
         pip3 install nec_pd_sdk
         
         License
         --------------
         The MIT License
         
-        Copyright (c) 2017-2018 NEC Display Solutions, Ltd.
+        Copyright (c) 2023 Sharp NEC Display Solutions, Ltd.
+        
+        Copyright (c) 2017-20 NEC Display Solutions, Ltd.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
@@ -56,14 +58,14 @@
         Added scheduling functions
         Added CPU Temperature based cooling fan control
         Added "command_ip_address_read" function to read the IP address of the display
         Added OPCODE definitions for new COMPUTE MODULE FAN CONTROL and AUTO SHUTDOWN
         Added new IR remote keys definitions
         Added new OPCODES definitions and controls.txt
         
-Keywords: NEC pd sdk
+Keywords: Sharp NEC pd sdk
 Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2.7
```

