# Comparing `tmp/malwoverview-5.3.tar.gz` & `tmp/malwoverview-5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "malwoverview-5.3.tar", last modified: Tue Jun 27 02:19:50 2023, max compression
+gzip compressed data, was "malwoverview-5.4.tar", last modified: Mon Aug  7 18:59:43 2023, max compression
```

## Comparing `malwoverview-5.3.tar` & `malwoverview-5.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 02:19:50.669625 malwoverview-5.3/
--rw-r--r--   0 root         (0) root         (0)      233 2023-06-27 01:55:55.000000 malwoverview-5.3/.malwapi.conf
--rw-r--r--   0 root         (0) root         (0)    35149 2023-06-27 01:55:55.000000 malwoverview-5.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)    35430 2023-06-27 02:19:50.669625 malwoverview-5.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    34905 2023-06-27 01:57:01.000000 malwoverview-5.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 02:19:50.665625 malwoverview-5.3/malwoverview/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 01:55:55.000000 malwoverview-5.3/malwoverview/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)   612059 2023-06-27 01:55:55.000000 malwoverview-5.3/malwoverview/malwoverview.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 02:19:50.669625 malwoverview-5.3/malwoverview.egg-info/
--rw-r--r--   0 root         (0) root         (0)    35430 2023-06-27 02:19:50.000000 malwoverview-5.3/malwoverview.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      273 2023-06-27 02:19:50.000000 malwoverview-5.3/malwoverview.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 02:19:50.000000 malwoverview-5.3/malwoverview.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      154 2023-06-27 02:19:50.000000 malwoverview-5.3/malwoverview.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-27 02:19:50.000000 malwoverview-5.3/malwoverview.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-27 02:19:50.669625 malwoverview-5.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1328 2023-06-27 01:55:55.000000 malwoverview-5.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 18:59:43.780086 malwoverview-5.4/
+-rw-r--r--   0 root         (0) root         (0)      234 2023-08-07 18:57:15.000000 malwoverview-5.4/.malwapi.conf
+-rw-r--r--   0 root         (0) root         (0)    35147 2023-08-07 18:57:15.000000 malwoverview-5.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    35846 2023-08-07 18:59:43.780086 malwoverview-5.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    35321 2023-08-07 18:58:11.000000 malwoverview-5.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 18:59:43.776086 malwoverview-5.4/malwoverview/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 18:57:16.000000 malwoverview-5.4/malwoverview/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)   614191 2023-08-07 18:57:16.000000 malwoverview-5.4/malwoverview/malwoverview.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 18:59:43.780086 malwoverview-5.4/malwoverview.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    35846 2023-08-07 18:59:43.000000 malwoverview-5.4/malwoverview.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      273 2023-08-07 18:59:43.000000 malwoverview-5.4/malwoverview.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 18:59:43.000000 malwoverview-5.4/malwoverview.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      185 2023-08-07 18:59:43.000000 malwoverview-5.4/malwoverview.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-07 18:59:43.000000 malwoverview-5.4/malwoverview.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-07 18:59:43.780086 malwoverview-5.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1356 2023-08-07 18:57:15.000000 malwoverview-5.4/setup.py
```

### Comparing `malwoverview-5.3/LICENSE` & `malwoverview-5.4/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -29,16 +29,16 @@
   To protect your rights, we need to prevent others from denying you
 these rights or asking you to surrender the rights.  Therefore, you have
 certain responsibilities if you distribute copies of the software, or if
 you modify it: responsibilities to respect the freedom of others.
 
   For example, if you distribute copies of such a program, whether
 gratis or for a fee, you must pass on to the recipients the same
-freedoms that you received.  You must make sure that they, too, receive
-or can get the source code.  And you must show them these terms so they
+freedoms that you received. You must make sure that they, too, receive
+or can get the source code. And you must show them these terms so they
 know their rights.
 
   Developers that use the GNU GPL protect your rights with two steps:
 (1) assert copyright on the software, and (2) offer you this License
 giving you legal permission to copy, distribute and/or modify it.
 
   For the developers' and authors' protection, the GPL clearly explains
```

### Comparing `malwoverview-5.3/PKG-INFO` & `malwoverview-5.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: malwoverview
-Version: 5.3
+Version: 5.4
 Summary: Malwoverview is a first response tool for threat hunting.
 Home-page: https://github.com/alexandreborges/malwoverview
 Author: Alexandre Borges
 Author-email: alexandreborges@blackstormsecurity.com
 License: GNU GPL v3.0
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -25,15 +25,15 @@
       but WITHOUT ANY WARRANTY; without even the implied warranty of
       MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
       GNU General Public License for more details.
 
       See GNU Public License on <http://www.gnu.org/licenses/>.
 
 
-# Current Version: 5.3
+# Current Version: 5.4
 
      Important note:  Malwoverview does NOT submit samples to any endpoint by default, 
      so it respects possible Non-Disclosure Agreements (NDAs). There're specific options
      that explicitly submit samples, but these options are explained in the help.
 
 
 # ABOUT
@@ -110,29 +110,29 @@
       * Add Python binary directory to the PATH variable by editing .bash_profile file in your home 
         directory. Example:
 
           export PATH=$PATH:/Users/alexandreborges/Library/Python/3.9/bin
 
       * Execute: . ./.bash_profile
 
-If you are installing Malwoverview on Windows, you must execute the following commands AFTER 
-installing Malwoverview:
-
-      * python -m pip uninstall python-magic
-      * python -m pip install python-magic-bin 
+If you are installing Malwoverview on Windows, make sure that the following conditions are true  
+AFTER having installed Malwoverview:
 
+      * python-magic is NOT installed. (pip show python-magic)
+      * python-magic-bin IS installed. (pip show python-magic-bin)
+      
 To use Malwoverview you should insert VirusTotal, Hybrid Analysis, URLHaus, Malshare, Polyswarm,
 Alien Vault, Malpedia  and Triage into the .malwapi.conf configuration file 
 (the default one at the home directory (/home/[username] or /root) -- if the file doesn't exist,
 so you should create it) or you could create a custom configuration file and indicate it by 
 using the -c option.
 
-Nonetheless, starting on version 4.4.2, it isn't longer necessary to insert all APIs into .malwapi.conf
-before using Malwoverview. Therefore, users can only insert few APIs and use the respective options 
-to these APIs.
+Nonetheless, starting on version 4.4.2, it isn't longer necessary to insert all APIs into 
+.malwapi.conf file before using Malwoverview. Therefore, users can only insert few APIs 
+and use the respective options to these APIs.
 
 * A special note about the Alien Vault: it is necessary to subscribe to pulses on Alien Vault 
 website before using -n 1 option.
 
 The .malwapi.conf configuration file (from the the home directory -- /home/[username] or /root) 
 has the following format:
 
@@ -387,14 +387,25 @@
     malwoverview.py -i 11 -I list
     malwoverview.py -i 12 -I rebrand.ly
     malwoverview.py -i 13 -I list | more
 
 
 # HISTORY
 
+Version 5.4:
+
+      This version:
+
+            * Fixes issues related to URLHaus.
+            * Fixes issues related to Polyswarm.
+            * Fixes issues related to Malware Bazaar.
+            * Fixes issues related to InQuest.
+            * Introduces changes to the help description. 
+            * Introduces changes to installation process. 
+
 Version 5.3:
 
       This version:
 
             * Fixes issues related to Malshare (-l and -L options).
             * Adds a new Malshare option (-l 7) to list all samples 
               from last 24 hours.
```

### Comparing `malwoverview-5.3/README.md` & `malwoverview-5.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
       but WITHOUT ANY WARRANTY; without even the implied warranty of
       MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
       GNU General Public License for more details.
 
       See GNU Public License on <http://www.gnu.org/licenses/>.
 
 
-# Current Version: 5.3
+# Current Version: 5.4
 
      Important note:  Malwoverview does NOT submit samples to any endpoint by default, 
      so it respects possible Non-Disclosure Agreements (NDAs). There're specific options
      that explicitly submit samples, but these options are explained in the help.
 
 
 # ABOUT
@@ -96,29 +96,29 @@
       * Add Python binary directory to the PATH variable by editing .bash_profile file in your home 
         directory. Example:
 
           export PATH=$PATH:/Users/alexandreborges/Library/Python/3.9/bin
 
       * Execute: . ./.bash_profile
 
-If you are installing Malwoverview on Windows, you must execute the following commands AFTER 
-installing Malwoverview:
-
-      * python -m pip uninstall python-magic
-      * python -m pip install python-magic-bin 
+If you are installing Malwoverview on Windows, make sure that the following conditions are true  
+AFTER having installed Malwoverview:
 
+      * python-magic is NOT installed. (pip show python-magic)
+      * python-magic-bin IS installed. (pip show python-magic-bin)
+      
 To use Malwoverview you should insert VirusTotal, Hybrid Analysis, URLHaus, Malshare, Polyswarm,
 Alien Vault, Malpedia  and Triage into the .malwapi.conf configuration file 
 (the default one at the home directory (/home/[username] or /root) -- if the file doesn't exist,
 so you should create it) or you could create a custom configuration file and indicate it by 
 using the -c option.
 
-Nonetheless, starting on version 4.4.2, it isn't longer necessary to insert all APIs into .malwapi.conf
-before using Malwoverview. Therefore, users can only insert few APIs and use the respective options 
-to these APIs.
+Nonetheless, starting on version 4.4.2, it isn't longer necessary to insert all APIs into 
+.malwapi.conf file before using Malwoverview. Therefore, users can only insert few APIs 
+and use the respective options to these APIs.
 
 * A special note about the Alien Vault: it is necessary to subscribe to pulses on Alien Vault 
 website before using -n 1 option.
 
 The .malwapi.conf configuration file (from the the home directory -- /home/[username] or /root) 
 has the following format:
 
@@ -373,14 +373,25 @@
     malwoverview.py -i 11 -I list
     malwoverview.py -i 12 -I rebrand.ly
     malwoverview.py -i 13 -I list | more
 
 
 # HISTORY
 
+Version 5.4:
+
+      This version:
+
+            * Fixes issues related to URLHaus.
+            * Fixes issues related to Polyswarm.
+            * Fixes issues related to Malware Bazaar.
+            * Fixes issues related to InQuest.
+            * Introduces changes to the help description. 
+            * Introduces changes to installation process. 
+
 Version 5.3:
 
       This version:
 
             * Fixes issues related to Malshare (-l and -L options).
             * Adds a new Malshare option (-l 7) to list all samples 
               from last 24 hours.
```

### Comparing `malwoverview-5.3/malwoverview/malwoverview.py` & `malwoverview-5.4/malwoverview/malwoverview.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 #CONTRIBUTORS
 
 # Alexandre Borges (project owner)
 # Corey Forman (https://github.com/digitalsleuth)
 # Christian Clauss (https://github.com/cclauss)
 
-# Malwoverview.py: version 5.3
+# Malwoverview.py: version 5.4
 
 import os
 import sys
 import re
 import pefile
 import peutils
 import magic
@@ -58,15 +58,15 @@
 from requests import Request, Session, exceptions
 
 # On Windows systems, it is necessary to install python-magic-bin: pip install python-magic-bin
 
 __author__ = "Alexandre Borges"
 __copyright__ = "Copyright 2018-2021, Alexandre Borges"
 __license__ = "GNU General Public License v3.0"
-__version__ = "5.3"
+__version__ = "5.4"
 __email__ = "alexandreborges at blackstormsecurity.com"
 
 haurl = 'https://www.hybrid-analysis.com/api/v2'
 urlfilevt3 = 'https://www.virustotal.com/api/v3/files'
 urlurlvt3 = 'https://www.virustotal.com/api/v3/urls'
 urlipvt3 = 'https://www.virustotal.com/api/v3/ip_addresses'
 urldomainvt3 = 'https://www.virustotal.com/api/v3/domains'
@@ -2485,46 +2485,69 @@
                         print(mycolors.reset + "\nSHA256: " +  mycolors.foreground.red + "%s" + "None", end=' ') 
                     if(x.md5):
                         print(mycolors.reset + "MD5: " + mycolors.foreground.green + "%s" % x.md5, end=' ')
                     else:
                         print(mycolors.reset + "MD5: " + mycolors.foreground.green + "%s" + "None", end=' ')
             print(mycolors.reset + "\n")
             sys.exit(0)
+        
+        try:
+
+            if (metainfo == 5):
+                metaresults = polyswarm.search_by_metadata("strings.ipv4:" + poly)
+            if (metainfo == 6):
+                metaresults = polyswarm.search_by_metadata("strings.domains:" + poly)
+            if (metainfo == 7):
+                poly = (r'"' + poly + r'"')
+                metaresults = polyswarm.search_by_metadata("strings.urls:" + poly)
+            if (metainfo == 8):
+                poly = ('scan.latest_scan.\*.metadata.malware_family:' + poly)
+                metaresults = polyswarm.search_by_metadata(poly)
+
+        except Exception:
+            if (bkg == 1):
+                print((mycolors.foreground.lightred + "\nInformation not found on Polyswarm.\n"))
+            else:
+                print((mycolors.foreground.red + "\nInformation not found on Polyswarm.\n"))
+            print(mycolors.reset)
+            exit(0)
 
-        if (metainfo == 5):
-            metaresults = polyswarm.search_by_metadata("strings.ipv4:" + poly)
-        if (metainfo == 6):
-            metaresults = polyswarm.search_by_metadata("strings.domains:" + poly)
-        if (metainfo == 7):
-            poly = (r'"' + poly + r'"')
-            metaresults = polyswarm.search_by_metadata("strings.urls:" + poly)
-        if (metainfo == 8):
-            poly = ('scan.latest_scan.\*.metadata.malware_family:' + poly)
-            metaresults = polyswarm.search_by_metadata(poly)
         for y in metaresults:
             if (bkg == 1):
                 if (y.sha256):
                     print(mycolors.reset + "\nSHA256: " +  mycolors.foreground.lightcyan + "%s" % y.sha256, end=' ') 
                 else:
                     print(mycolors.reset + "Result: " + mycolors.foreground.yellow + "Sample not found!", end=' ')
                     exit(0)
-                score = next(polyswarm.search(y.sha256))
+               
+                try:
+                    score = next(polyswarm.search(y.sha256))
+                except Exception:
+                    score.polyscore = "None"
+                    pass
+
                 print(mycolors.reset + "Polyscore: " +  mycolors.foreground.yellow + "%20s" % score.polyscore, end=' ') 
                 if (str(y.scan.get('detections',{}).get('malicious'))) != 'None':
                     print(mycolors.reset + "scan: " + mycolors.foreground.yellow + "%s" % y.scan.get('detections', {}).get('malicious'), end=' ') 
                     print("/ " + "%2s malicious" % y.scan.get('detections',{}).get('total'), end=' ')
                 else:
                     print(mycolors.reset + "scan: " + mycolors.foreground.pink + "not scanned yet", end=' ')
             else:
                 if (y.sha256):
                     print(mycolors.reset + "\nSHA256: " +  mycolors.foreground.green + "%s" % y.sha256, end=' ') 
                 else:
                     print(mycolors.reset + "scan: " + mycolors.foreground.purple + "Sample not found!", end=' ')
                     exit(0)
-                score = next(polyswarm.search(y.sha256))
+
+                try:
+                    score = next(polyswarm.search(y.sha256))
+                except Exception:
+                    score.polyscore = "None"
+                    pass
+
                 print(mycolors.reset + "Polyscore: " +  mycolors.foreground.red + "%20s" % score.polyscore, end=' ') 
                 if (str(y.scan.get('detections',{}).get('malicious'))) != 'None':
                     print(mycolors.reset + "scan: " + mycolors.foreground.red + "%s" % y.scan.get('detections', {}).get('malicious'), end=' ') 
                     print("/ " + "%2s malicious" % y.scan.get('detections',{}).get('total'), end=' ')
                 else:
                     print(mycolors.reset + "Result: " + mycolors.foreground.purple + "not scanned yet", end=' ')
 
@@ -3477,27 +3500,39 @@
                 else:
                     print(Fore.BLACK + "\n")
 
                 for i in allpayloads:
                     x = x + 1
                     if (bkg == 1):
                         print(mycolors.reset + "Payload_%d:\t" % x, end='')
-                        print(mycolors.foreground.pink + "firstseen:%12s" % i['firstseen'], end = '     ' )
-                        print(mycolors.foreground.yellow + "filename: %-30s" % i['filename'].ljust(40), end = ' ' + "")
-                        print(mycolors.foreground.lightred + "filetype: %s" % i['file_type'].ljust(10) + Fore.WHITE, end= ' ' + "")
+                        if ('firstseen' in i):
+                            if (i['firstseen'] is not None):
+                                print(mycolors.foreground.pink + "firstseen:%12s" % i['firstseen'], end = '     ' )
+                        if ('filename' in i):
+                            if (i['filename'] is not None):
+                                print(mycolors.foreground.yellow + "filename: %-30s" % i['filename'].ljust(40), end = ' ' + "")
+                        if ('file_type' in i):
+                            if (i['file_type'] is not None):
+                                print(mycolors.foreground.lightred + "filetype: %s" % i['file_type'].ljust(10) + Fore.WHITE, end= ' ' + "")
                         results = i['virustotal']
                         if (results) is not None:
                             print(mycolors.foreground.lightcyan + "VirusTotal: %s" % results['result'] + Fore.WHITE)
                         else:
                             print(mycolors.foreground.lightcyan + "VirusTotal: Not Found" + Fore.WHITE)
                     else:
                         print(mycolors.reset + "Payload_%d:\t" % x, end='')
-                        print(mycolors.foreground.purple + "firstseen:%12s" % i['firstseen'], end = '     ')
-                        print(mycolors.foreground.green + "filename: %-30s" % i['filename'].ljust(40), end = ' ' + "")
-                        print(mycolors.foreground.red + "filetype: %s" % i['file_type'].ljust(10) + Fore.BLACK, end = '' + "")
+                        if ('firstseen' in i):
+                            if (i['firstseen'] is not None):
+                                print(mycolors.foreground.purple + "firstseen:%12s" % i['firstseen'], end = '     ')
+                        if ('filename' in i):
+                            if (i['filename'] is not None):
+                                print(mycolors.foreground.green + "filename: %-30s" % i['filename'].ljust(40), end = ' ' + "")
+                        if ('file_type' in i):
+                            if (i['file_type'] is not None):
+                                print(mycolors.foreground.red + "filetype: %s" % i['file_type'].ljust(10) + Fore.BLACK, end = '' + "")
                         results = i['virustotal']
                         if (results) is not None:
                             print(mycolors.foreground.blue + "VirusTotal: %s" % results['result'] + Fore.BLACK)
                         else:
                             print(mycolors.foreground.blue + "VirusTotal: Not Found" + Fore.BLACK)
 
                 print(mycolors.reset + "\nSample Hashes")
@@ -5181,25 +5216,34 @@
                 print(mycolors.foreground.red + "\nThe -I parameter with the provided SHA256 hash is required!\n" + mycolors.reset)
             exit(1)
 
         requestsession = requests.Session( )
         requestsession.headers.update({'Accept': 'application/octet-stream'})
         requestsession.headers.update({'Authorization':INQUESTAPI})
         inquestresponse = requestsession.get(inquest + '/download?sha256=' + inquestx)
-
+        
         if (inquestresponse.status_code == 400):
             inquesttext = json.loads(inquestresponse.text)
 
             if 'error' in inquesttext:
                 if inquesttext['error'] == "Supplied 'sha256' value is not a valid hash.":
                     if (bkg == 1):
                         print(mycolors.foreground.lightred + "\nThe provided SHA256 hash is not valid!\n" + mycolors.reset)
                     else:
                         print(mycolors.foreground.red + "\nThe provided SHA256 hash is not valid!\n" + mycolors.reset)
                     exit(1)
+            
+        if (inquestresponse.status_code == 403 or inquestresponse.status_code == 500):
+            inquesttext = json.loads(inquestresponse.text)
+
+            if (bkg == 1):
+                print(mycolors.foreground.lightred + "\nThe sample is not available for download!\n" + mycolors.reset)
+            else:
+                print(mycolors.foreground.red + "\nThe sample is not available for download!\n" + mycolors.reset)
+            exit(1)
 
         open(inquestx + '.bin', 'wb').write(inquestresponse.content)
         if (bkg == 1):
             print("\n" + mycolors.foreground.yellow + "SAMPLE SAVED as: " + inquestx + ".bin" + mycolors.reset, end=' ')
         if (bkg == 0):
             print("\n" + mycolors.foreground.blue + "SAMPLE SAVED as: " + inquestx + ".bin" + mycolors.reset, end=' ')
 
@@ -5238,14 +5282,15 @@
 
         requestsession = requests.Session( )
         requestsession.headers.update({'Accept': 'application/json'})
         requestsession.headers.update({'Authorization':INQUESTAPI})
         inquestresponse = requestsession.get(inquest + '/search/hash/sha256?hash=' + inquestx)
         inquesttext = json.loads(inquestresponse.text)
 
+
         if (inquestresponse.status_code == 400 or inquestresponse.status_code == 500):
             inquesttext = json.loads(inquestresponse.text)
 
             if 'error' in inquesttext:
                 if inquesttext['error'] == "The 'source' parameter must be one of md5, sha1, sha256, sha512":
                     if (bkg == 1):
                         print(mycolors.foreground.lightred + "\nThe provided hash is not a SHA256 hash!\n" + mycolors.reset)
@@ -7156,15 +7201,16 @@
         print("\n")
         print((mycolors.reset + "THREATFOX REPORT".center(100)), end='')
         print((mycolors.reset + "".center(28)), end='')
         print("\n" + (100*'-').center(50))
 
         requestsession = requests.Session( )
         requestsession.headers.update({'accept':'application/json'})
-        params = {'query':"get_iocs" , 'days':bazaarx}
+        params = {'query':"get_iocs" , 'days':int(bazaarx)}
+
         bazaarresponse = requestsession.post(url=bazaar, data=json.dumps(params))
         bazaartext = json.loads(bazaarresponse.text)
 
         if (bkg == 1):
             for i in bazaartext.keys():
                 if (i == "data"):
                     if (bazaartext['data'] is not None):
@@ -10361,15 +10407,15 @@
     bazaararg = ''
     triage = 0
     triagearg = ''
     virustotalarg = ''
     ipaddrvtx = ''
     ffpname = ''
 
-    parser = argparse.ArgumentParser(prog=None, description="Malwoverview is a first response tool for threat hunting written by Alexandre Borges. This version is 5.3", usage= "python malwoverview.py -c <API configuration file> -d <directory> -o <0|1> -v <1-13> -V <virustotal arg> -a <1-15> -w <0|1> -A <filename> -l <1-7> -L <hash> -j <1-7> -J <URLhaus argument> -p <1-8> -P <polyswarm argument> -y <1-5> -Y <file name> -n <1-5> -N <argument> -m <1-8> -M <argument> -b <1-10> -B <arg> -x <1-7> -X <arg> -i <1-13> -I <INQUEST argument>")
+    parser = argparse.ArgumentParser(prog=None, description="Malwoverview is a first response tool for threat hunting written by Alexandre Borges. This version is 5.4", usage= "python malwoverview.py -c <API configuration file> -d <directory> -o <0|1> -v <1-13> -V <virustotal arg> -a <1-15> -w <0|1> -A <filename> -l <1-7> -L <hash> -j <1-7> -J <URLhaus argument> -p <1-8> -P <polyswarm argument> -y <1-5> -Y <file name> -n <1-5> -N <argument> -m <1-8> -M <argument> -b <1-10> -B <arg> -x <1-7> -X <arg> -i <1-13> -I <INQUEST argument>")
     parser.add_argument('-c', '--config', dest='config', type=str, metavar = "CONFIG FILE", default = (USER_HOME_DIR + '.malwapi.conf'), help='Use a custom config file to specify API\'s.')
     parser.add_argument('-d', '--directory', dest='direct',type=str, metavar = "DIRECTORY", help='Specifies the directory containing malware samples to be checked against VIRUS TOTAL. Use the option -D to decide whether you are being using a public VT API or a Premium VT API.')
     parser.add_argument('-o', '--background', dest='backg', type=int,default = 1, metavar = "BACKGROUND", help='Adapts the output colors to a light background color terminal. The default is dark background color terminal.')
     parser.add_argument('-v', '--virustotal_option', dest='virustotaloption', type=int,default = 0, metavar = "VIRUSTOTAL", help='-v 1: given a file using -V option, it queries the VIRUS TOTAL database (API v.3) to get the report for the given file through -V option.; -v 2: it shows an antivirus report for a given file using -V option (API v.3); -v 3: equal to -v2, but the binary\'s IAT and EAT are also shown (API v.3); -v 4: it extracts the overlay; -v 5: submits an URL to VT scanning; -v 6: submits an IP address to Virus Total; -v 7: this options gets a report on the provided domain from Virus Total; -v 8: verifies a given hash against Virus Total; -v 9: submits a sample to VT (up to 32 MB). Use forward slash to specify the target file on Windows systems. Demands passing sample file with -V option; -v 10: verifies hashes from a provided file through option -V. This option uses public VT API v.3; -v 11: verifies hashes from a provided file through option -V. This option uses Premium API v.3; -v 12: it shows behaviour information of a sample given a hash through option -V. This option uses VT API v.3; -v 13: it submits LARGE files (above 32 MB) to VT using API v.3;')
     parser.add_argument('-V', '--virustotal_arg', dest='virustotalarg', type=str, metavar = "VIRUSTOTAL_ARG", help='Provides arguments for -v option.')
     parser.add_argument('-a', '--hybrid_option', dest='haoption', type=int,default = 0, metavar = "HYBRID_ANALYSIS", help='This parameter fetches reports from HYBRID ANALYSIS, download samples and submits samples to be analyzed. The possible values are: 1: gets a report for a given hash or sample from a Windows 7 32-bit environment; 2: gets a report for a given hash or sample from a Windows 7 32-bit environment (HWP Support); 3: gets a report for given hash or sample from a Windows 64-bit environment; 4: gets a report for a given hash or sample from an Android environment; 5: gets a report for a given hash or sample from a Linux 64-bit environment; 6: submits a sample to Windows 7 32-bit environment; 7. submits a sample to Windows 7 32-bit environment with HWP support environment; 8. submits a sample to Windows 7 64-bit environment ; 9. submits a sample to an Android environment ; 10. submits a sample to a Linux 64-bit environment; 11. downloads a sample from a Windows 7 32-bit environment; 12. downloads a sample from a Windows 7 32-bit HWP environment; 13. downloads a sample from a Windows 7 64-bit environment; 14. downloads a sample from an Android environment; 15. downloads a sample from a Linux 64-bit environment.')
     parser.add_argument('-A', '--ha_arg', dest='haarg', type=str, metavar = "SUBMIT_HA", help='Provides an argument for -a option from HYBRID ANALYSIS.')
@@ -10383,15 +10429,15 @@
     parser.add_argument('-y', '--android_option', dest='androidoption', type=int, default = 0, metavar = "ANDROID_OPTION", help='This ANDROID option has multiple possible values: <1>: Check all third-party APK packages from the USB-connected Android device against Hybrid Analysis using multithreads. Notes: the Android device does not need to be rooted and the system does need to have the adb tool in the PATH environment variable; <2>: Check all third-party APK packages from the USB-connected Android device against VirusTotal using Public API (slower because of 60 seconds delay for each 4 hashes). Notes: the Android device does not need to be rooted and the system does need to have adb tool in the PATH environment variable; <3>: Check all third-party APK packages from the USB-connected Android device against VirusTotal using multithreads (only for Private Virus API). Notes: the Android device does not need to be rooted and the system needs to have adb tool in the PATH environment variable; <4> Sends an third-party APK from your USB-connected Android device to Hybrid Analysis; 5. Sends an third-party APK from your USB-connected Android device to Virus-Total.')
     parser.add_argument('-Y', '--android_arg', dest='androidarg', type=str, metavar = "ANDROID_ARG", help='This option provides the argument for -y from ANDROID.')
     parser.add_argument('-n', '--alienvault', dest='alienvault', type=int, default = 0, metavar = "ALIENVAULT", help='Checks multiple information from ALIENVAULT. The possible values are: 1: Get the subscribed pulses ; 2: Get information about an IP address; 3: Get information about a domain; 4: Get information about a hash; 5: Get information about a URL.')
     parser.add_argument('-N', '--alienvaultargs', dest='alienvaultargs', type=str, metavar = "ALIENVAULT_ARGS", help='Provides argument to ALIENVAULT -n option.')
     parser.add_argument('-m', '--malpedia', dest='malpedia', type=int, default = 0, metavar = "MALPEDIA", help='This option is related to MALPEDIA and presents different meanings depending on the chosen value. Thus, 1: List meta information for all families ; 2: List all actors ID ; 3: List all available payloads organized by family from Malpedia; 4: Get meta information from an specific actor, so it is necessary to use the -M option. Additionally, try to confirm the correct actor ID by executing malwoverview with option -m 3; 5: List all families IDs; 6: Get meta information from an specific family, so it is necessary to use the -M option. Additionally, try to confirm the correct family ID by executing malwoverview with option -m 5; 7: Get a malware sample from malpedia (zip format -- password: infected). It is necessary to specify the requested hash by using -M option; 8: Get a zip file containing Yara rules for a specific family (get the possible families using -m 5), which must be specified by using -M option.')
     parser.add_argument('-M', '--malpediarg', dest='malpediaarg', type=str, metavar = "MALPEDIAARG", help='This option provides an argument to the -m option, which is related to MALPEDIA.')
     parser.add_argument('-b', '--bazaar', dest='bazaar', type=int, default = 0, metavar = "BAZAAR", help='Checks multiple information from MALWARE BAZAAR and THREATFOX. The possible values are: 1: (Bazaar) Query information about a malware hash sample ; 2: (Bazaar) Get information and a list of malware samples associated and according to a specific tag; 3: (Bazaar) Get a list of malware samples according to a given imphash; 4: (Bazaar) Query latest malware samples; 5: (Bazaar) Download a malware sample from Malware Bazaar by providing a SHA256 hash. The downloaded sample is zipped using the following password: infected; 6: (ThreatFox) Get current IOC dataset from last x days given by option -B (maximum of 7 days); 7: (ThreatFox) Search for the specified IOC on ThreatFox given by option -B; 8: (ThreatFox) Search IOCs according to the specified tag given by option -B; 9: (ThreatFox) Search IOCs according to the specified malware family provided by option -B; 10. (ThreatFox) List all available malware families.')
-    parser.add_argument('-B', '--bazaararg', dest='bazaararg', type=str, metavar = "BAZAAR_ARG", help='Provides argument to -b MALWARE BAZAAR and THREAT FOX option. If you specified "-b 1" then the -B\'s argument must be a hash; If you specified "-b 2" then -B\'s argument must be a malware tag; If you specified "-b 3" then the argument must be a imphash; If you specified "-b 4", so the argument must be "100 or time", where "100" lists last "100 samples" and "time" lists last samples added to Malware Bazaar in the last 60 minutes; If you specified "-b 5" then the -B\'s argument must be a SHA256 hash; If you specified "-b 6", so the -B\'s value is the number of DAYS to filter IOCs. The maximum is 7 (days); If you used "-b 7" so the -B\'s argument is the IOC you want to search for; If you used "-b 8", so the -B\'s argument is the TAG you want search for; If you used "-b 9", so the -B argument is the malware family you want to search for;')
+    parser.add_argument('-B', '--bazaararg', dest='bazaararg', type=str, metavar = "BAZAAR_ARG", help='Provides argument to -b MALWARE BAZAAR and THREAT FOX option. If you specified "-b 1" then the -B\'s argument must be a hash and a report about the sample will be retrieved; If you specified "-b 2" then -B\'s argument must be a malware tag and last samples matching this tag will be shown; If you specified "-b 3" then the argument must be a imphash and last samples matching this impshash will be shown; If you specified "-b 4", so the argument must be "100 or time", where "100" lists last "100 samples" and "time" lists last samples added to Malware Bazaar in the last 60 minutes; If you specified "-b 5", so the sample will be downloaded and -B\'s argument must be a SHA256 hash of the sample that you want to download from Malware Bazaar; If you specified "-b 6" then a list of IOCs will be retrieved and the -B\'s value is the number of DAYS to filter such IOCs. The maximum time is 7 (days); If you used "-b 7" so the -B\'s argument is the IOC you want to search for; If you used "-b 8", so the -B\'s argument is the IOC\'s TAG that you want search for; If you used "-b 9", so the -B argument is the malware family that you want to search for IOCs;')
     parser.add_argument('-x', '--triage', dest='triage', type=int,default = 0, metavar = "TRIAGE", help='Provides information from TRIAGE according to the specified value: <1> this option gets sample\'s general information by providing an argument with -X option in the following possible formats: sha256:<value>, sha1:<value>, md5:<value>, family:<value>, score:<value>, tag:<value>, url:<value>, wallet:<value>, ip:<value>; <2> Get a sumary report for a given Triage ID (got from option -x 1) ; <3> Submit a sample for analysis ; <4> Submit a sample through a URL for analysis ; <5> Download sample specified by the Triage ID; <6> Download pcapng file from sample associated to given Triage ID; <7> Get a dynamic report for the given Triage ID (got from option -x 1);')
     parser.add_argument('-X', '--triagearg', dest='triagearg', type=str, metavar = "TRIAGE_ARG", help='Provides argument for options especified by -x option. Pay attention: the format of this argument depends on provided -x value.')
     parser.add_argument('-i', '--inquest', dest='inquest', type=int, default = 0, metavar = "INQUEST", help='Retrieves multiple information from INQUEST. The possible values are: 1: Downloads a sample; 2: Retrives information about a sample given a SHA256; 3: Retrieves information about a sample given a MD5 hash; 4: Gets the most recent list of threats. To this option, the -I argument must be "list" (lowercase and without double quotes) ; 5: Retrives threats related to a provided domain; 6. Retrieves a list of samples related to the given IP address; 7. Retrives a list of sample related to the given e-mail address; 8. Retrieves a list of samples related to the given filename; 9. Retrieves a list of samples related to a given URL; 10. Retrieves information about a specified IOC; 11. List a list of IOCs. Note: you must pass "list" (without double quotes) as argument to -I; 12. Check for a given keyword in the reputation database; 13. List artifacts in the reputation dabatabse. Note: you must pass "list" (without double quotes) as argument to -I.')
     parser.add_argument('-I', '--inquestarg', dest='inquestarg', type=str, metavar = "INQUEST_ARG", help='Provides argument to INQUEST -i option.')
 
     args = parser.parse_args()
```

### Comparing `malwoverview-5.3/malwoverview.egg-info/PKG-INFO` & `malwoverview-5.4/malwoverview.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: malwoverview
-Version: 5.3
+Version: 5.4
 Summary: Malwoverview is a first response tool for threat hunting.
 Home-page: https://github.com/alexandreborges/malwoverview
 Author: Alexandre Borges
 Author-email: alexandreborges@blackstormsecurity.com
 License: GNU GPL v3.0
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -25,15 +25,15 @@
       but WITHOUT ANY WARRANTY; without even the implied warranty of
       MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
       GNU General Public License for more details.
 
       See GNU Public License on <http://www.gnu.org/licenses/>.
 
 
-# Current Version: 5.3
+# Current Version: 5.4
 
      Important note:  Malwoverview does NOT submit samples to any endpoint by default, 
      so it respects possible Non-Disclosure Agreements (NDAs). There're specific options
      that explicitly submit samples, but these options are explained in the help.
 
 
 # ABOUT
@@ -110,29 +110,29 @@
       * Add Python binary directory to the PATH variable by editing .bash_profile file in your home 
         directory. Example:
 
           export PATH=$PATH:/Users/alexandreborges/Library/Python/3.9/bin
 
       * Execute: . ./.bash_profile
 
-If you are installing Malwoverview on Windows, you must execute the following commands AFTER 
-installing Malwoverview:
-
-      * python -m pip uninstall python-magic
-      * python -m pip install python-magic-bin 
+If you are installing Malwoverview on Windows, make sure that the following conditions are true  
+AFTER having installed Malwoverview:
 
+      * python-magic is NOT installed. (pip show python-magic)
+      * python-magic-bin IS installed. (pip show python-magic-bin)
+      
 To use Malwoverview you should insert VirusTotal, Hybrid Analysis, URLHaus, Malshare, Polyswarm,
 Alien Vault, Malpedia  and Triage into the .malwapi.conf configuration file 
 (the default one at the home directory (/home/[username] or /root) -- if the file doesn't exist,
 so you should create it) or you could create a custom configuration file and indicate it by 
 using the -c option.
 
-Nonetheless, starting on version 4.4.2, it isn't longer necessary to insert all APIs into .malwapi.conf
-before using Malwoverview. Therefore, users can only insert few APIs and use the respective options 
-to these APIs.
+Nonetheless, starting on version 4.4.2, it isn't longer necessary to insert all APIs into 
+.malwapi.conf file before using Malwoverview. Therefore, users can only insert few APIs 
+and use the respective options to these APIs.
 
 * A special note about the Alien Vault: it is necessary to subscribe to pulses on Alien Vault 
 website before using -n 1 option.
 
 The .malwapi.conf configuration file (from the the home directory -- /home/[username] or /root) 
 has the following format:
 
@@ -387,14 +387,25 @@
     malwoverview.py -i 11 -I list
     malwoverview.py -i 12 -I rebrand.ly
     malwoverview.py -i 13 -I list | more
 
 
 # HISTORY
 
+Version 5.4:
+
+      This version:
+
+            * Fixes issues related to URLHaus.
+            * Fixes issues related to Polyswarm.
+            * Fixes issues related to Malware Bazaar.
+            * Fixes issues related to InQuest.
+            * Introduces changes to the help description. 
+            * Introduces changes to installation process. 
+
 Version 5.3:
 
       This version:
 
             * Fixes issues related to Malshare (-l and -L options).
             * Adds a new Malshare option (-l 7) to list all samples 
               from last 24 hours.
```

### Comparing `malwoverview-5.3/setup.py` & `malwoverview-5.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 USER_HOME_DIR = str(Path.home()) + os.sep
 
 with open("README.md", encoding='utf8') as readme:
     long_description = readme.read()
 
 setup(
     name="malwoverview",
-    version="5.3",
+    version="5.4",
     author="Alexandre Borges",
     author_email="alexandreborges@blackstormsecurity.com",
     license="GNU GPL v3.0",
     url="https://github.com/alexandreborges/malwoverview",
     description=("Malwoverview is a first response tool for threat hunting."),
     long_description=long_description,
     long_description_content_type="text/markdown",
@@ -24,15 +24,15 @@
     'Operating System :: OS Independent',
     'License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)',
     'Programming Language :: Python :: 3',
     ],
     install_requires=[
         "pefile",
         "colorama",
-        "python-magic",
+        "python-magic; platform_system == 'Linux'",
         "simplejson",
         "requests",
         "validators",
         "geocoder",
         "polyswarm-api",
         "pathlib",
         "configparser",
```

