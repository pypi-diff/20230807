# Comparing `tmp/ptsamesite-0.0.4.tar.gz` & `tmp/ptsamesite-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptsamesite-0.0.4.tar", last modified: Mon Mar 28 16:56:22 2022, max compression
+gzip compressed data, was "ptsamesite-1.0.0.tar", last modified: Mon Aug  7 11:48:01 2023, max compression
```

## Comparing `ptsamesite-0.0.4.tar` & `ptsamesite-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2022-03-28 16:56:22.582017 ptsamesite-0.0.4/
--rw-r--r--   0 kali      (1000) kali      (1000)    35823 2021-12-17 14:07:30.000000 ptsamesite-0.0.4/LICENSE
--rw-r--r--   0 kali      (1000) kali      (1000)     2894 2022-03-28 16:56:22.582017 ptsamesite-0.0.4/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)     2539 2022-03-28 16:55:06.000000 ptsamesite-0.0.4/README.md
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2022-03-28 16:56:22.582017 ptsamesite-0.0.4/ptsamesite/
--rw-r--r--   0 kali      (1000) kali      (1000)        0 2021-12-17 14:07:30.000000 ptsamesite-0.0.4/ptsamesite/__init__.py
--rw-r--r--   0 kali      (1000) kali      (1000)     7007 2022-03-28 16:55:00.000000 ptsamesite-0.0.4/ptsamesite/ptsamesite.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2022-03-28 16:56:22.582017 ptsamesite-0.0.4/ptsamesite.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)     2894 2022-03-28 16:56:22.000000 ptsamesite-0.0.4/ptsamesite.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      280 2022-03-28 16:56:22.000000 ptsamesite-0.0.4/ptsamesite.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2022-03-28 16:56:22.000000 ptsamesite-0.0.4/ptsamesite.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       59 2022-03-28 16:56:22.000000 ptsamesite-0.0.4/ptsamesite.egg-info/entry_points.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       50 2022-03-28 16:56:22.000000 ptsamesite-0.0.4/ptsamesite.egg-info/requires.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       11 2022-03-28 16:56:22.000000 ptsamesite-0.0.4/ptsamesite.egg-info/top_level.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2022-03-28 16:56:22.582017 ptsamesite-0.0.4/setup.cfg
--rw-r--r--   0 kali      (1000) kali      (1000)      860 2022-03-28 16:56:02.000000 ptsamesite-0.0.4/setup.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-08-07 11:48:01.172405 ptsamesite-1.0.0/
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)    35823 2023-08-07 10:48:49.000000 ptsamesite-1.0.0/LICENSE
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     3495 2023-08-07 11:48:01.172405 ptsamesite-1.0.0/PKG-INFO
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     3029 2023-08-07 11:42:39.000000 ptsamesite-1.0.0/README.md
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-08-07 11:48:01.168405 ptsamesite-1.0.0/ptsamesite/
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-08-07 10:48:49.000000 ptsamesite-1.0.0/ptsamesite/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       21 2023-08-07 10:48:49.000000 ptsamesite-1.0.0/ptsamesite/_version.py
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     7312 2023-08-07 11:36:40.000000 ptsamesite-1.0.0/ptsamesite/ptsamesite.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-08-07 11:48:01.172405 ptsamesite-1.0.0/ptsamesite.egg-info/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     3495 2023-08-07 11:48:01.000000 ptsamesite-1.0.0/ptsamesite.egg-info/PKG-INFO
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      303 2023-08-07 11:48:01.000000 ptsamesite-1.0.0/ptsamesite.egg-info/SOURCES.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2023-08-07 11:48:01.000000 ptsamesite-1.0.0/ptsamesite.egg-info/dependency_links.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       58 2023-08-07 11:48:01.000000 ptsamesite-1.0.0/ptsamesite.egg-info/entry_points.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       39 2023-08-07 11:48:01.000000 ptsamesite-1.0.0/ptsamesite.egg-info/requires.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       11 2023-08-07 11:48:01.000000 ptsamesite-1.0.0/ptsamesite.egg-info/top_level.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       38 2023-08-07 11:48:01.172405 ptsamesite-1.0.0/setup.cfg
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     1042 2023-08-07 10:48:49.000000 ptsamesite-1.0.0/setup.py
```

### Comparing `ptsamesite-0.0.4/LICENSE` & `ptsamesite-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ptsamesite-0.0.4/PKG-INFO` & `ptsamesite-1.0.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,81 +1,97 @@
 Metadata-Version: 2.1
 Name: ptsamesite
-Version: 0.0.4
-Summary: Same Site Scripting Tester
+Version: 1.0.0
+Summary: Same site scripting detection tool
 Home-page: https://www.penterep.com/
 Author: Penterep
 Author-email: info@penterep.com
 License: GPLv3+
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Environment :: Console
+Classifier: Topic :: Security
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-![penterepTools](https://www.penterep.com/external/penterepToolsLogo.png)
+[![penterepTools](https://www.penterep.com/external/penterepToolsLogo.png)](https://www.penterep.com/)
+
 
 # PTSAMESITE
-> Same Site Scripting Testing Tool
 
-ptsamesite is a tool for testing Same Site Scripting vulnerability. ptsamesite supports mass domain testing.
+> Same site scripting detection tool
+
+ptsamesite is a tool that tests domains for same site scripting vulnerability. <br />
+ptsamesite utilizes threading for fast parallel domain testing.
 
-- Script sends DNS "A" query to domain with 'localhost' as subdomain.
-- If DNS responds with IP '127.0.0.1', the record is prone to Same Site Scripting vulnerability. 
 
 ## Installation
 
 ```
 pip install ptsamesite
 ```
 
 ## Add to PATH
 If you cannot invoke the script in your terminal, its probably because its not in your PATH. Fix it by running commands below.
+
+> Add to PATH for Bash
 ```bash
 echo "export PATH=\"`python3 -m site --user-base`/bin:\$PATH\"" >> ~/.bashrc
 source ~/.bashrc
 ```
 
+> Add to PATH for ZSH
+```bash
+echo "export PATH=\"`python3 -m site --user-base`/bin:\$PATH\"" >> ~/.zshhrc
+source ~/.zshhrc
+```
+
 ## Usage examples
 ```
-$ ptsamesite -d example.com
-$ ptsamesite -d subdomain1.subdomain2.example.com -s
-$ ptsamesite -d example.com example2.com
-$ ptsamesite -f domain_list.txt
+ptsamesite -d example.com                               # Test domain
+ptsamesite -d example.com example2.com                  # Test two domains
+ptsamesite -d subdomain1.subdomain2.example.com -s      # Test domain along with all subdomains
+ptsamesite -f domain_list.txt                           # Test domains from a file
+ptsamesite -f domains_list.txt -s -t 100 -V             # Test domains from a file with all present subdomains, set threads count to 100 and print only vulnerable domains
 ```
 
 ## Options
 ```
 -d  --domain      <domain>   Test domain
 -f  --file        <file>     Test domains from file
--V  --vulnerable             Print only vulnerable domains
--s  --subdomains             Scan all subdomains of given domain
--t  --threads     <threads>  Number of threads (default 20)
--j  --json                   Output in JSON format
+-s  --subdomains             Test all subdomains of given domain (default False)
+-t  --threads     <threads>  Set number of threads (default 20)
+-V  --vulnerable             Show only vulnerable domains
 -v  --version                Show script version and exit
 -h  --help                   Show this help message and exit
+-j  --json                   Output in JSON format
 ```
 
 
 ## Dependencies
-- dnspython
-- tldextract
-- ptlibs
-- ptthreads
+```
+dnspython
+tldextract
+ptlibs
+```
 
 ## Version History
+```
+1.0.0
+    - Code improvements
+    - Updated for ptlibs 1.0.0
+0.0.1 - 0.0.5
+    - Alpha releases
+```
 
-* 0.0.1 - 0.0.4
-    * Alpha releases
-
-## Licence
+## License
 
-Copyright (c) 2020 HACKER Consulting s.r.o.
+Copyright (c) 2023 Penterep Security s.r.o.
 
 ptsamesite is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 ptsamesite is distributed in the hope that it will be useful,
@@ -89,8 +105,7 @@
 ## Warning
 
 You are only allowed to run the tool against the websites which
 you have been given permission to pentest. We do not accept any
 responsibility for any damage/harm that this application causes to your
 computer, or your network. Penterep is not responsible for any illegal
 or malicious use of this code. Be Ethical!
-
```

### Comparing `ptsamesite-0.0.4/README.md` & `ptsamesite-1.0.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,65 +1,80 @@
-![penterepTools](https://www.penterep.com/external/penterepToolsLogo.png)
+[![penterepTools](https://www.penterep.com/external/penterepToolsLogo.png)](https://www.penterep.com/)
+
 
 # PTSAMESITE
-> Same Site Scripting Testing Tool
 
-ptsamesite is a tool for testing Same Site Scripting vulnerability. ptsamesite supports mass domain testing.
+> Same site scripting detection tool
+
+ptsamesite is a tool that tests domains for same site scripting vulnerability. <br />
+ptsamesite utilizes threading for fast parallel domain testing.
 
-- Script sends DNS "A" query to domain with 'localhost' as subdomain.
-- If DNS responds with IP '127.0.0.1', the record is prone to Same Site Scripting vulnerability. 
 
 ## Installation
 
 ```
 pip install ptsamesite
 ```
 
 ## Add to PATH
 If you cannot invoke the script in your terminal, its probably because its not in your PATH. Fix it by running commands below.
+
+> Add to PATH for Bash
 ```bash
 echo "export PATH=\"`python3 -m site --user-base`/bin:\$PATH\"" >> ~/.bashrc
 source ~/.bashrc
 ```
 
+> Add to PATH for ZSH
+```bash
+echo "export PATH=\"`python3 -m site --user-base`/bin:\$PATH\"" >> ~/.zshhrc
+source ~/.zshhrc
+```
+
 ## Usage examples
 ```
-$ ptsamesite -d example.com
-$ ptsamesite -d subdomain1.subdomain2.example.com -s
-$ ptsamesite -d example.com example2.com
-$ ptsamesite -f domain_list.txt
+ptsamesite -d example.com                               # Test domain
+ptsamesite -d example.com example2.com                  # Test two domains
+ptsamesite -d subdomain1.subdomain2.example.com -s      # Test domain along with all subdomains
+ptsamesite -f domain_list.txt                           # Test domains from a file
+ptsamesite -f domains_list.txt -s -t 100 -V             # Test domains from a file with all present subdomains, set threads count to 100 and print only vulnerable domains
 ```
 
 ## Options
 ```
 -d  --domain      <domain>   Test domain
 -f  --file        <file>     Test domains from file
--V  --vulnerable             Print only vulnerable domains
--s  --subdomains             Scan all subdomains of given domain
--t  --threads     <threads>  Number of threads (default 20)
--j  --json                   Output in JSON format
+-s  --subdomains             Test all subdomains of given domain (default False)
+-t  --threads     <threads>  Set number of threads (default 20)
+-V  --vulnerable             Show only vulnerable domains
 -v  --version                Show script version and exit
 -h  --help                   Show this help message and exit
+-j  --json                   Output in JSON format
 ```
 
 
 ## Dependencies
-- dnspython
-- tldextract
-- ptlibs
-- ptthreads
+```
+dnspython
+tldextract
+ptlibs
+```
 
 ## Version History
+```
+1.0.0
+    - Code improvements
+    - Updated for ptlibs 1.0.0
+0.0.1 - 0.0.5
+    - Alpha releases
+```
 
-* 0.0.1 - 0.0.4
-    * Alpha releases
-
-## Licence
+## License
 
-Copyright (c) 2020 HACKER Consulting s.r.o.
+Copyright (c) 2023 Penterep Security s.r.o.
 
 ptsamesite is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 ptsamesite is distributed in the hope that it will be useful,
```

### Comparing `ptsamesite-0.0.4/ptsamesite/ptsamesite.py` & `ptsamesite-1.0.0/ptsamesite/ptsamesite.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,88 +1,88 @@
 #!/usr/bin/python3
 """
-    Same Site Scripting Testing Tool
+    Copyright (c) 2023 Penterep Security s.r.o.
 
-    Copyright (c) 2020 HACKER Consulting s.r.o.
+    ptsamesite - Same site scripting detection tool
 
-    This program is free software: you can redistribute it and/or modify
+    ptsamesite is free software: you can redistribute it and/or modify
     it under the terms of the GNU General Public License as published by
     the Free Software Foundation, either version 3 of the License, or
     (at your option) any later version.
 
-    This program is distributed in the hope that it will be useful,
+    ptsamesite is distributed in the hope that it will be useful,
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+    along with ptsamesite.  If not, see <https://www.gnu.org/licenses/>.
 """
 
-__version__ = "0.0.4"
-
 import argparse
-import sys
+import sys; sys.path.append(__file__.rsplit("/", 1)[0])
 
-from ptlibs import ptmisclib, ptjsonlib
-from ptthreads import ptthreads
+from _version import __version__
+from ptlibs import ptmisclib, ptjsonlib, ptprinthelper
+from ptlibs.threads import ptthreads, printlock
 
 import dns.resolver
 import tldextract
 
 
-class ptsamesite:
+class PtSamesite:
     def __init__(self, args):
-        self.json = args.json
-        self.jsonlib = ptjsonlib.ptjsonlib(self.json)
-        self.json_no = self.jsonlib.add_json("ptsamesite")
-
-        self.data_list = []
-        self.vulnerable = args.vulnerable
-        self.subdomains = args.subdomains
-        self.ptthreads_ = ptthreads.ptthreads()
+        self.ptjsonlib          = ptjsonlib.PtJsonLib()
+        self.ptthreads          = ptthreads.PtThreads()
+        self.use_json           = args.json
+        self.vulnerable         = args.vulnerable
+        self.subdomains         = args.subdomains
+        self.result_list        = []
 
-    def run(self, args):
         try:
-            domains = ptmisclib.read_file(args.file) if args.file else args.domain
+            self.domain_list = ptmisclib.read_file(args.file) if args.file else args.domain
+            self._domain_list_len = len(self.domain_list)
         except FileNotFoundError:
-            ptmisclib.end_error("File not found!", self.json_no, self.ptjsonlib, self.use_json)
-        if self.vulnerable:
-            ptmisclib.ptprint_(ptmisclib.out_ifnot("Vulnerable domains:", "TITLE", self.json))
-        self.ptthreads_.threads(domains, self._test_domain, args.threads)
-        self.jsonlib.add_data(self.json_no, {"result": self.data_list})
-        ptmisclib.ptprint_(ptmisclib.out_if(self.jsonlib.get_all_json(), None, self.json))
-
-    def _test_domain(self, domain):
-        """test domains in paralell"""
-        printlock = ptthreads.printlock()
-        subdomains = self._prepare_subdomains_for_test(domain)
+            self.ptjsonlib.end_error("File not found", self.use_json)
+
+        if len(self.domain_list) > 1 and self.use_json:
+            self.ptjsonlib.end_error("Cannot test more than 1 domain while --json parameter is present", self.use_json)
+
+    def run(self, args) -> None:
+        """Main method"""
+        ptprinthelper.ptprint("Vulnerable domains:", "TITLE", not self.use_json and self.vulnerable)
+
+        self.ptthreads.threads(self.domain_list, self._test_domain, args.threads)
+        self.ptjsonlib.set_status("ok")
+        ptprinthelper.ptprint(self.ptjsonlib.get_result_json(), "", self.use_json)
+
+    def _test_domain(self, domain_list: list):
+        printlock_ = printlock.PrintLock()
+        subdomains = self._prepare_subdomains_for_test(domain_list)
         for subdomain in subdomains:
-            self.data_list.append(self._test_subdomain(subdomain, printlock))
-        printlock.lock_print_output(end="")
+            self.result_list.append(self._test_subdomain(subdomain, printlock_))
+        printlock_.lock_print_output(end="")
 
-    def _test_subdomain(self, subdomain, printlock):
-        printlock.add_string_to_output( ptmisclib.out_ifnot(f"Testing {subdomain}", "TITLE", self.json), not self.vulnerable)
+    def _test_subdomain(self, subdomain, printlock_):
+        printlock_.add_string_to_output( ptprinthelper.out_ifnot(f"Testing {subdomain}", "TITLE", self.use_json, colortext=True), not self.vulnerable)
         data = {"domain": subdomain, "status": "null", "vulnerable": "null", "ip": "null"}
         try:
             resolver = dns.resolver.Resolver()
-            resolver.timeout = 0.05
-            ip = resolver.resolve(subdomain, "A")[0].to_text()
-            # printlock.add_string_to_output( ptmisclib.out_ifnot(f"IP: {ip}", "INFO", self.json), not self.vulnerable)
+            resolver.timeout = 5
+            ip = resolver.resolve(subdomain, "A", lifetime=5)[0].to_text()
             if ip == "127.0.0.1":
-                printlock.add_string_to_output( ptmisclib.out_ifnot(f"Domain is vulnerable to same site scripting", "VULN", self.json), not self.vulnerable)
-                printlock.add_string_to_output( ptmisclib.out_if(subdomain, "", self.vulnerable), self.vulnerable)
-                self.jsonlib.set_vulnerable(self.json_no, True)
+                printlock_.add_string_to_output( ptprinthelper.out_ifnot(f"Vulnerable to same site scripting", "VULN", self.use_json), not self.vulnerable)
+                printlock_.add_string_to_output( ptprinthelper.out_if(subdomain, "", self.vulnerable), self.vulnerable)
+                self.ptjsonlib.add_vulnerability("PTWVSSS", note=subdomain)
                 data.update({"vulnerable": True, "ip": ip, "domain": subdomain, "status": "ok"})
             else:
-                printlock.add_string_to_output( ptmisclib.out_ifnot(f"Domain not vulnerable", "NOTVULN", self.json), not self.vulnerable)
+                printlock_.add_string_to_output( ptprinthelper.out_ifnot(f"Not vulnerable to same site scripting", "NOTVULN", self.use_json), not self.vulnerable)
                 data.update({"vulnerable": False, "ip": ip, "domain": subdomain, "status": "ok"})
-            self.jsonlib.set_status(self.json_no, "ok")
-        except dns.exception.DNSException as e:
-            printlock.add_string_to_output( ptmisclib.out_ifnot(f"Domain not vulnerable", "NOTVULN", self.json), not self.vulnerable)
+        except dns.exception.DNSException:
+            printlock_.add_string_to_output( ptprinthelper.out_ifnot(f"{str(sys.exc_info()[1]).split(':')[0]}", "INFO", self.use_json), not self.vulnerable)
             data.update({"vulnerable": False, "domain": subdomain, "status": "ok"})
         return data
 
     def _prepare_subdomains_for_test(self, domain):
         ext = tldextract.extract(domain)
         subdomains = []
         while domain.startswith("."):
@@ -99,52 +99,53 @@
                 domain = "localhost." + domain
             subdomains.append(domain)
         return subdomains
 
 
 def get_help():
     return [
-        {"description": ["Same Site Scripting Testing Tool"]},
+        {"description": ["Same site scripting detection tool"]},
         {"usage": ["ptsamesite <options>"]},
-        {"usage_example": ["ptsamesite -d example.com", "ptsamesite -d subdomain1.subdomain2.example.com -s", "ptsamesite -d example.com example2.com", "ptsamesite -f domain_list.txt"]},
+        {"usage_example": ["ptsamesite -d example.com", "ptsamesite -d example.com example2.com", "ptsamesite -d subdomain1.subdomain2.example.com -s", "ptsamesite -f domain_list.txt", "ptsamesite -f domains_list.txt -s -V -t 100"]},
         {"options": [
             ["-d",  "--domain",           "<domain>",   "Test domain"],
             ["-f",  "--file",             "<file>",     "Test domains from file"],
-            ["-V", "--vulnerable",        "",           "Print only vulnerable domains"],
-            ["-s", "--subdomains",        "",           "Scan all subdomains of given domain"],
-            ["-t",  "--threads",          "<threads>",  "Number of threads (default 20)"],
-            ["-j",  "--json",             "",           "Output in JSON format"],
+            ["-s",  "--subdomains",       "",           "Test all subdomains of given domain (default False)"],
+            ["-t",  "--threads",          "<threads>",  "Set number of threads (default 20)"],
+            ["-V",  "--vulnerable",       "",           "Show only vulnerable domains"],
             ["-v",  "--version",          "",           "Show script version and exit"],
             ["-h",  "--help",             "",           "Show this help message and exit"],
+            ["-j",  "--json",             "",           "Output in JSON format"],
         ]}
     ]
 
 
 def parse_args():
     parser = argparse.ArgumentParser(add_help=False, usage=f"{SCRIPTNAME} <options>")
-    required = parser.add_argument_group("One of the following arguments is required")
-    required = required.add_mutually_exclusive_group(required=True)
-    required.add_argument("-d", "--domain", type=str, nargs="+")
-    required.add_argument("-f", "--file", type=str)
-    parser.add_argument("-s", "--subdomains", action="store_true")
-    parser.add_argument("-V", "--vulnerable", action="store_true")
-    parser.add_argument("-t", "--threads", default=20, type=int)
-    parser.add_argument("-j", "--json", action="store_true")
-    parser.add_argument("-v", "--version", action="version", version=f"{SCRIPTNAME} {__version__}")
+    exclusive_group = parser.add_mutually_exclusive_group(required=True)
+    exclusive_group.add_argument("-d", "--domain", type=str, nargs="+")
+    exclusive_group.add_argument("-f", "--file",   type=str)
+    parser.add_argument("-t", "--threads",         type=int, default=20)
+    parser.add_argument("-s", "--subdomains",      action="store_true")
+    parser.add_argument("-V", "--vulnerable",      action="store_true")
+    parser.add_argument("-j", "--json",            action="store_true")
+    parser.add_argument("-v", "--version",         action="version", version=f"{SCRIPTNAME} {__version__}")
 
     if len(sys.argv) == 1 or "-h" in sys.argv or "--help" in sys.argv:
-        ptmisclib.help_print(get_help(), SCRIPTNAME, __version__)
+        ptprinthelper.help_print(get_help(), SCRIPTNAME, __version__)
         sys.exit(0)
+
     args = parser.parse_args()
+    ptprinthelper.print_banner(SCRIPTNAME, __version__, args.json, space=0)
     return args
 
 
 def main():
     global SCRIPTNAME
     SCRIPTNAME = "ptsamesite"
     args = parse_args()
-    script = ptsamesite(args)
+    script = PtSamesite(args)
     script.run(args)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `ptsamesite-0.0.4/ptsamesite.egg-info/PKG-INFO` & `ptsamesite-1.0.0/ptsamesite.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,81 +1,97 @@
 Metadata-Version: 2.1
 Name: ptsamesite
-Version: 0.0.4
-Summary: Same Site Scripting Tester
+Version: 1.0.0
+Summary: Same site scripting detection tool
 Home-page: https://www.penterep.com/
 Author: Penterep
 Author-email: info@penterep.com
 License: GPLv3+
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Environment :: Console
+Classifier: Topic :: Security
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-![penterepTools](https://www.penterep.com/external/penterepToolsLogo.png)
+[![penterepTools](https://www.penterep.com/external/penterepToolsLogo.png)](https://www.penterep.com/)
+
 
 # PTSAMESITE
-> Same Site Scripting Testing Tool
 
-ptsamesite is a tool for testing Same Site Scripting vulnerability. ptsamesite supports mass domain testing.
+> Same site scripting detection tool
+
+ptsamesite is a tool that tests domains for same site scripting vulnerability. <br />
+ptsamesite utilizes threading for fast parallel domain testing.
 
-- Script sends DNS "A" query to domain with 'localhost' as subdomain.
-- If DNS responds with IP '127.0.0.1', the record is prone to Same Site Scripting vulnerability. 
 
 ## Installation
 
 ```
 pip install ptsamesite
 ```
 
 ## Add to PATH
 If you cannot invoke the script in your terminal, its probably because its not in your PATH. Fix it by running commands below.
+
+> Add to PATH for Bash
 ```bash
 echo "export PATH=\"`python3 -m site --user-base`/bin:\$PATH\"" >> ~/.bashrc
 source ~/.bashrc
 ```
 
+> Add to PATH for ZSH
+```bash
+echo "export PATH=\"`python3 -m site --user-base`/bin:\$PATH\"" >> ~/.zshhrc
+source ~/.zshhrc
+```
+
 ## Usage examples
 ```
-$ ptsamesite -d example.com
-$ ptsamesite -d subdomain1.subdomain2.example.com -s
-$ ptsamesite -d example.com example2.com
-$ ptsamesite -f domain_list.txt
+ptsamesite -d example.com                               # Test domain
+ptsamesite -d example.com example2.com                  # Test two domains
+ptsamesite -d subdomain1.subdomain2.example.com -s      # Test domain along with all subdomains
+ptsamesite -f domain_list.txt                           # Test domains from a file
+ptsamesite -f domains_list.txt -s -t 100 -V             # Test domains from a file with all present subdomains, set threads count to 100 and print only vulnerable domains
 ```
 
 ## Options
 ```
 -d  --domain      <domain>   Test domain
 -f  --file        <file>     Test domains from file
--V  --vulnerable             Print only vulnerable domains
--s  --subdomains             Scan all subdomains of given domain
--t  --threads     <threads>  Number of threads (default 20)
--j  --json                   Output in JSON format
+-s  --subdomains             Test all subdomains of given domain (default False)
+-t  --threads     <threads>  Set number of threads (default 20)
+-V  --vulnerable             Show only vulnerable domains
 -v  --version                Show script version and exit
 -h  --help                   Show this help message and exit
+-j  --json                   Output in JSON format
 ```
 
 
 ## Dependencies
-- dnspython
-- tldextract
-- ptlibs
-- ptthreads
+```
+dnspython
+tldextract
+ptlibs
+```
 
 ## Version History
+```
+1.0.0
+    - Code improvements
+    - Updated for ptlibs 1.0.0
+0.0.1 - 0.0.5
+    - Alpha releases
+```
 
-* 0.0.1 - 0.0.4
-    * Alpha releases
-
-## Licence
+## License
 
-Copyright (c) 2020 HACKER Consulting s.r.o.
+Copyright (c) 2023 Penterep Security s.r.o.
 
 ptsamesite is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 ptsamesite is distributed in the hope that it will be useful,
@@ -89,8 +105,7 @@
 ## Warning
 
 You are only allowed to run the tool against the websites which
 you have been given permission to pentest. We do not accept any
 responsibility for any damage/harm that this application causes to your
 computer, or your network. Penterep is not responsible for any illegal
 or malicious use of this code. Be Ethical!
-
```

