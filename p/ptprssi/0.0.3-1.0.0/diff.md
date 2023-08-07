# Comparing `tmp/ptprssi-0.0.3.tar.gz` & `tmp/ptprssi-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptprssi-0.0.3.tar", last modified: Mon Mar 28 16:36:19 2022, max compression
+gzip compressed data, was "ptprssi-1.0.0.tar", last modified: Mon Aug  7 10:19:17 2023, max compression
```

## Comparing `ptprssi-0.0.3.tar` & `ptprssi-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2022-03-28 16:36:19.199174 ptprssi-0.0.3/
--rw-r--r--   0 kali      (1000) kali      (1000)    35823 2021-12-17 14:07:30.000000 ptprssi-0.0.3/LICENSE
--rw-r--r--   0 kali      (1000) kali      (1000)     2890 2022-03-28 16:36:19.199174 ptprssi-0.0.3/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)     2549 2022-03-28 16:36:14.000000 ptprssi-0.0.3/README.md
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2022-03-28 16:36:19.199174 ptprssi-0.0.3/ptprssi/
--rw-r--r--   0 kali      (1000) kali      (1000)        0 2021-12-17 14:07:30.000000 ptprssi-0.0.3/ptprssi/__init__.py
--rw-r--r--   0 kali      (1000) kali      (1000)     8075 2022-03-28 16:35:33.000000 ptprssi-0.0.3/ptprssi/ptprssi.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2022-03-28 16:36:19.199174 ptprssi-0.0.3/ptprssi.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)     2890 2022-03-28 16:36:19.000000 ptprssi-0.0.3/ptprssi.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      253 2022-03-28 16:36:19.000000 ptprssi-0.0.3/ptprssi.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2022-03-28 16:36:19.000000 ptprssi-0.0.3/ptprssi.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       50 2022-03-28 16:36:19.000000 ptprssi-0.0.3/ptprssi.egg-info/entry_points.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       25 2022-03-28 16:36:19.000000 ptprssi-0.0.3/ptprssi.egg-info/requires.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        8 2022-03-28 16:36:19.000000 ptprssi-0.0.3/ptprssi.egg-info/top_level.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2022-03-28 16:36:19.199174 ptprssi-0.0.3/setup.cfg
--rw-r--r--   0 kali      (1000) kali      (1000)      782 2022-03-28 16:35:37.000000 ptprssi-0.0.3/setup.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-08-07 10:19:17.428537 ptprssi-1.0.0/
+-rwxrw-rw-   0 daniel    (1000) daniel    (1000)    35823 2023-01-11 20:44:27.000000 ptprssi-1.0.0/LICENSE
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     3146 2023-08-07 10:19:17.424537 ptprssi-1.0.0/PKG-INFO
+-rwxrw-rw-   0 daniel    (1000) daniel    (1000)     2659 2023-08-07 09:48:59.000000 ptprssi-1.0.0/README.md
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-08-07 10:19:17.424537 ptprssi-1.0.0/ptprssi/
+-rwxrw-rw-   0 daniel    (1000) daniel    (1000)        0 2023-01-11 20:44:27.000000 ptprssi-1.0.0/ptprssi/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       21 2023-04-19 12:46:57.000000 ptprssi-1.0.0/ptprssi/_version.py
+-rwxrw-rw-   0 daniel    (1000) daniel    (1000)     7854 2023-08-07 10:06:43.000000 ptprssi-1.0.0/ptprssi/ptprssi.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-08-07 10:19:17.424537 ptprssi-1.0.0/ptprssi.egg-info/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     3146 2023-08-07 10:19:17.000000 ptprssi-1.0.0/ptprssi.egg-info/PKG-INFO
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      273 2023-08-07 10:19:17.000000 ptprssi-1.0.0/ptprssi.egg-info/SOURCES.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2023-08-07 10:19:17.000000 ptprssi-1.0.0/ptprssi.egg-info/dependency_links.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       49 2023-08-07 10:19:17.000000 ptprssi-1.0.0/ptprssi.egg-info/entry_points.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       31 2023-08-07 10:19:17.000000 ptprssi-1.0.0/ptprssi.egg-info/requires.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        8 2023-08-07 10:19:17.000000 ptprssi-1.0.0/ptprssi.egg-info/top_level.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       38 2023-08-07 10:19:17.428537 ptprssi-1.0.0/setup.cfg
+-rwxrw-rw-   0 daniel    (1000) daniel    (1000)      998 2023-08-07 10:00:47.000000 ptprssi-1.0.0/setup.py
```

### Comparing `ptprssi-0.0.3/LICENSE` & `ptprssi-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ptprssi-0.0.3/PKG-INFO` & `ptprssi-1.0.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,99 +1,98 @@
 Metadata-Version: 2.1
 Name: ptprssi
-Version: 0.0.3
-Summary: PRSSI Testing Tool
+Version: 1.0.0
+Summary: Path-relative style sheet import testing tool
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
 
 
 # PTPRSSI
-> Path-relative Style Sheet Import Testing Tool
-
-ptprssi is a tool for testing path-relative style sheet import vulnerabilities.
+> Path-relative style sheet import testing tool
 
 ## Installation
-
 ```
 pip install ptprssi
 ```
 
-### Add to PATH
+## Add to PATH
 If you cannot invoke the script in your terminal, its probably because its not in your PATH. Fix it by running commands below.
 
-Add to path for BASH
+> Add to PATH for Bash
 ```bash
 echo "export PATH=\"`python3 -m site --user-base`/bin:\$PATH\"" >> ~/.bashrc
 source ~/.bashrc
 ```
-Add to path for ZSH
+
+> Add to PATH for ZSH
 ```bash
 echo "export PATH=\"`python3 -m site --user-base`/bin:\$PATH\"" >> ~/.zshhrc
 source ~/.zshhrc
 ```
 
 ## Usage examples
 ```
-prssi -u https://www.example.com/
-ptprssi -u https://www.example.com/ -r
+ptprssi -u https://www.example.com/
+ptprssi -u https://www.example.com/ --redirects
 ```
 
 ## Options
 ```
 -u   --url         <url>           Connect to URL
--r   --redirects                   Follow redirects
 -p   --proxy       <proxy>         Set proxy (e.g. http://127.0.0.1:8080)
 -H   --headers     <header:value>  Set custom header(s)
+-T   --timeout     <timeout>       Set timeout (default 10s)
 -ua  --user-agent  <ua>            Set User-Agent header
 -c   --cookie      <cookie>        Set cookie
--j   --json                        Output in JSON format
+-r   --redirects                   Follow redirects (default False)
+-C   --cache                       Cache HTTP communication (load from tmp in future)
 -v   --version                     Show script version and exit
 -h   --help                        Show this help message and exit
+-j   --json                        Output in JSON format
 ```
 
 ## Dependencies
 ```
-ptlibs
 requests
-lxml
 bs4
+lxml
+ptlibs
 ```
 
-## Dependencies
-   - bs4
-   - lxml
-   - requests
-   - ptlibs
-
 ## Version History
-    0.0.1 - 0.0.3
-        Alpha releases
+```
+1.0.0
+    - Code improvements
+    - Updated for ptlibs 1.0.0
+0.0.1 - 0.0.4
+    - Alpha releases
+```
 
-## Licence
+## License
 
-Copyright (c) 2020 HACKER Consulting s.r.o.
+Copyright (c) 2023 Penterep Security s.r.o.
 
-This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
+ptprssi is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 
-This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
+ptprssi is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 
-You should have received a copy of the GNU General Public License along with this program. If not, see https://www.gnu.org/licenses/.
+You should have received a copy of the GNU General Public License along with ptprssi. If not, see https://www.gnu.org/licenses/.
 
 ## Warning
 
 You are only allowed to run the tool against the websites which
 you have been given permission to pentest. We do not accept any
 responsibility for any damage/harm that this application causes to your
 computer, or your network. Penterep is not responsible for any illegal
 or malicious use of this code. Be Ethical!
-
```

### Comparing `ptprssi-0.0.3/README.md` & `ptprssi-1.0.0/ptprssi.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,82 +1,98 @@
-![penterepTools](https://www.penterep.com/external/penterepToolsLogo.png)
-
-
-# PTPRSSI
-> Path-relative Style Sheet Import Testing Tool
-
-ptprssi is a tool for testing path-relative style sheet import vulnerabilities.
-
-## Installation
-
-```
-pip install ptprssi
-```
-
-### Add to PATH
-If you cannot invoke the script in your terminal, its probably because its not in your PATH. Fix it by running commands below.
-
-Add to path for BASH
-```bash
-echo "export PATH=\"`python3 -m site --user-base`/bin:\$PATH\"" >> ~/.bashrc
-source ~/.bashrc
-```
-Add to path for ZSH
-```bash
-echo "export PATH=\"`python3 -m site --user-base`/bin:\$PATH\"" >> ~/.zshhrc
-source ~/.zshhrc
-```
-
-## Usage examples
-```
-prssi -u https://www.example.com/
-ptprssi -u https://www.example.com/ -r
-```
-
-## Options
-```
--u   --url         <url>           Connect to URL
--r   --redirects                   Follow redirects
--p   --proxy       <proxy>         Set proxy (e.g. http://127.0.0.1:8080)
--H   --headers     <header:value>  Set custom header(s)
--ua  --user-agent  <ua>            Set User-Agent header
--c   --cookie      <cookie>        Set cookie
--j   --json                        Output in JSON format
--v   --version                     Show script version and exit
--h   --help                        Show this help message and exit
-```
-
-## Dependencies
-```
-ptlibs
-requests
-lxml
-bs4
-```
-
-## Dependencies
-   - bs4
-   - lxml
-   - requests
-   - ptlibs
-
-## Version History
-    0.0.1 - 0.0.3
-        Alpha releases
-
-## Licence
-
-Copyright (c) 2020 HACKER Consulting s.r.o.
-
-This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
-
-This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License along with this program. If not, see https://www.gnu.org/licenses/.
-
-## Warning
-
-You are only allowed to run the tool against the websites which
-you have been given permission to pentest. We do not accept any
-responsibility for any damage/harm that this application causes to your
-computer, or your network. Penterep is not responsible for any illegal
-or malicious use of this code. Be Ethical!
+Metadata-Version: 2.1
+Name: ptprssi
+Version: 1.0.0
+Summary: Path-relative style sheet import testing tool
+Home-page: https://www.penterep.com/
+Author: Penterep
+Author-email: info@penterep.com
+License: GPLv3+
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Environment :: Console
+Classifier: Topic :: Security
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![penterepTools](https://www.penterep.com/external/penterepToolsLogo.png)](https://www.penterep.com/)
+
+
+# PTPRSSI
+> Path-relative style sheet import testing tool
+
+## Installation
+```
+pip install ptprssi
+```
+
+## Add to PATH
+If you cannot invoke the script in your terminal, its probably because its not in your PATH. Fix it by running commands below.
+
+> Add to PATH for Bash
+```bash
+echo "export PATH=\"`python3 -m site --user-base`/bin:\$PATH\"" >> ~/.bashrc
+source ~/.bashrc
+```
+
+> Add to PATH for ZSH
+```bash
+echo "export PATH=\"`python3 -m site --user-base`/bin:\$PATH\"" >> ~/.zshhrc
+source ~/.zshhrc
+```
+
+## Usage examples
+```
+ptprssi -u https://www.example.com/
+ptprssi -u https://www.example.com/ --redirects
+```
+
+## Options
+```
+-u   --url         <url>           Connect to URL
+-p   --proxy       <proxy>         Set proxy (e.g. http://127.0.0.1:8080)
+-H   --headers     <header:value>  Set custom header(s)
+-T   --timeout     <timeout>       Set timeout (default 10s)
+-ua  --user-agent  <ua>            Set User-Agent header
+-c   --cookie      <cookie>        Set cookie
+-r   --redirects                   Follow redirects (default False)
+-C   --cache                       Cache HTTP communication (load from tmp in future)
+-v   --version                     Show script version and exit
+-h   --help                        Show this help message and exit
+-j   --json                        Output in JSON format
+```
+
+## Dependencies
+```
+requests
+bs4
+lxml
+ptlibs
+```
+
+## Version History
+```
+1.0.0
+    - Code improvements
+    - Updated for ptlibs 1.0.0
+0.0.1 - 0.0.4
+    - Alpha releases
+```
+
+## License
+
+Copyright (c) 2023 Penterep Security s.r.o.
+
+ptprssi is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
+
+ptprssi is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License along with ptprssi. If not, see https://www.gnu.org/licenses/.
+
+## Warning
+
+You are only allowed to run the tool against the websites which
+you have been given permission to pentest. We do not accept any
+responsibility for any damage/harm that this application causes to your
+computer, or your network. Penterep is not responsible for any illegal
+or malicious use of this code. Be Ethical!
```

