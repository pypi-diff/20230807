# Comparing `tmp/harmony_toolbox-1.2.0.tar.gz` & `tmp/harmony_toolbox-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "harmony_toolbox-1.2.0.tar", last modified: Fri Aug  4 22:44:26 2023, max compression
+gzip compressed data, was "harmony_toolbox-1.2.2.tar", last modified: Sun Aug  6 22:18:00 2023, max compression
```

## Comparing `harmony_toolbox-1.2.0.tar` & `harmony_toolbox-1.2.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)        0 2023-08-04 22:44:26.315449 harmony_toolbox-1.2.0/
--rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)     1066 2023-04-04 17:13:12.000000 harmony_toolbox-1.2.0/LICENSE
--rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)      146 2023-04-04 17:13:12.000000 harmony_toolbox-1.2.0/MANIFEST.in
--rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)     1680 2023-08-04 22:44:26.316452 harmony_toolbox-1.2.0/PKG-INFO
--rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)     1058 2023-04-04 17:13:12.000000 harmony_toolbox-1.2.0/README.md
--rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)      121 2023-04-04 17:13:12.000000 harmony_toolbox-1.2.0/pyproject.toml
--rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)      141 2023-06-30 15:28:08.000000 harmony_toolbox-1.2.0/requirements.txt
--rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)      736 2023-08-04 22:44:26.323452 harmony_toolbox-1.2.0/setup.cfg
--rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)       37 2023-04-04 17:13:12.000000 harmony_toolbox-1.2.0/setup.py
-drwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)        0 2023-08-04 22:44:25.855155 harmony_toolbox-1.2.0/src/
-drwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)        0 2023-08-04 22:44:26.130661 harmony_toolbox-1.2.0/src/harmony_toolbox.egg-info/
--rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)     1680 2023-08-04 22:44:25.000000 harmony_toolbox-1.2.0/src/harmony_toolbox.egg-info/PKG-INFO
--rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)      344 2023-08-04 22:44:25.000000 harmony_toolbox-1.2.0/src/harmony_toolbox.egg-info/SOURCES.txt
--rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)        1 2023-08-04 22:44:25.000000 harmony_toolbox-1.2.0/src/harmony_toolbox.egg-info/dependency_links.txt
--rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)        8 2023-08-04 22:44:25.000000 harmony_toolbox-1.2.0/src/harmony_toolbox.egg-info/top_level.txt
-drwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)        0 2023-08-04 22:44:26.282452 harmony_toolbox-1.2.0/src/toolbox/
--rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)        0 2023-03-24 16:13:56.000000 harmony_toolbox-1.2.0/src/toolbox/__init__.py
--rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)     2297 2023-08-04 21:35:21.000000 harmony_toolbox-1.2.0/src/toolbox/config.py
--rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)    53489 2023-08-04 22:21:21.000000 harmony_toolbox-1.2.0/src/toolbox/library.py
--rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)    36219 2023-08-04 22:20:07.000000 harmony_toolbox-1.2.0/src/toolbox/toolbox.py
+drwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)        0 2023-08-06 22:18:00.056137 harmony_toolbox-1.2.2/
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)     1066 2023-04-04 17:13:12.000000 harmony_toolbox-1.2.2/LICENSE
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)      146 2023-04-04 17:13:12.000000 harmony_toolbox-1.2.2/MANIFEST.in
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)     1680 2023-08-06 22:18:00.057139 harmony_toolbox-1.2.2/PKG-INFO
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)     1058 2023-08-06 19:43:06.000000 harmony_toolbox-1.2.2/README.md
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)      121 2023-04-04 17:13:12.000000 harmony_toolbox-1.2.2/pyproject.toml
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)      154 2023-08-06 05:59:09.000000 harmony_toolbox-1.2.2/requirements.txt
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)      736 2023-08-06 22:18:00.066817 harmony_toolbox-1.2.2/setup.cfg
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)       37 2023-04-04 17:13:12.000000 harmony_toolbox-1.2.2/setup.py
+drwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)        0 2023-08-06 22:17:59.538567 harmony_toolbox-1.2.2/src/
+drwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)        0 2023-08-06 22:17:59.850320 harmony_toolbox-1.2.2/src/harmony_toolbox.egg-info/
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)     1680 2023-08-06 22:17:59.000000 harmony_toolbox-1.2.2/src/harmony_toolbox.egg-info/PKG-INFO
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)      344 2023-08-06 22:17:59.000000 harmony_toolbox-1.2.2/src/harmony_toolbox.egg-info/SOURCES.txt
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)        1 2023-08-06 22:17:59.000000 harmony_toolbox-1.2.2/src/harmony_toolbox.egg-info/dependency_links.txt
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)        8 2023-08-06 22:17:59.000000 harmony_toolbox-1.2.2/src/harmony_toolbox.egg-info/top_level.txt
+drwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)        0 2023-08-06 22:18:00.013446 harmony_toolbox-1.2.2/src/toolbox/
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)        0 2023-03-24 16:13:56.000000 harmony_toolbox-1.2.2/src/toolbox/__init__.py
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)     2754 2023-08-06 22:16:54.000000 harmony_toolbox-1.2.2/src/toolbox/config.py
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)    57217 2023-08-06 22:14:53.000000 harmony_toolbox-1.2.2/src/toolbox/library.py
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)    37334 2023-08-06 19:26:09.000000 harmony_toolbox-1.2.2/src/toolbox/toolbox.py
```

### Comparing `harmony_toolbox-1.2.0/LICENSE` & `harmony_toolbox-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `harmony_toolbox-1.2.0/PKG-INFO` & `harmony_toolbox-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: harmony_toolbox
-Version: 1.2.0
+Version: 1.2.2
 Summary: Harmony ONE Validator Node Toolbox and Easy Setup
 Home-page: https://github.com/easy-node-pro/harmony-toolbox
 Author: EasyNode.PRO
 Author-email: support@easynode.pro
 Project-URL: Bug Tracker, https://github.com/easy-node-pro/harmony-toolbox/issues
 Project-URL: repository, https://github.com/easy-node-pro/harmony-toolbox
 Classifier: Programming Language :: Python :: 3
```

### Comparing `harmony_toolbox-1.2.0/README.md` & `harmony_toolbox-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `harmony_toolbox-1.2.0/setup.cfg` & `harmony_toolbox-1.2.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = harmony_toolbox
-version = 1.2.0
+version = 1.2.2
 author = EasyNode.PRO
 author_email = support@easynode.pro
 description = Harmony ONE Validator Node Toolbox and Easy Setup
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/easy-node-pro/harmony-toolbox
 project_urls =
```

### Comparing `harmony_toolbox-1.2.0/src/harmony_toolbox.egg-info/PKG-INFO` & `harmony_toolbox-1.2.2/src/harmony_toolbox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: harmony-toolbox
-Version: 1.2.0
+Version: 1.2.2
 Summary: Harmony ONE Validator Node Toolbox and Easy Setup
 Home-page: https://github.com/easy-node-pro/harmony-toolbox
 Author: EasyNode.PRO
 Author-email: support@easynode.pro
 Project-URL: Bug Tracker, https://github.com/easy-node-pro/harmony-toolbox/issues
 Project-URL: repository, https://github.com/easy-node-pro/harmony-toolbox
 Classifier: Programming Language :: Python :: 3
```

### Comparing `harmony_toolbox-1.2.0/src/toolbox/config.py` & `harmony_toolbox-1.2.2/src/toolbox/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,35 @@
-import os
-import socket
-import requests
+import socket, requests, json
 from os import environ, path
 from dotenv import load_dotenv
 
 load_dotenv(f"{path.expanduser('~')}/.easynode.env")
 
 
 def get_url(timeout=5) -> str:
     try:
-        response = requests.get("https://ident.me", timeout=timeout)
+        response = requests.get("https://api.ipify.org?format=json", timeout=timeout)
         response.raise_for_status()  # Raises a HTTPError if the response was unsuccessful
-        result = response.text
+
+        # Parse the JSON response
+        ip_data = response.json()
+        result = ip_data["ip"]
     except requests.exceptions.RequestException as x:
-        print(type(x), x)
-        result = "0.0.0.0"
+        try:
+            response = requests.get("https://ident.me", timeout=timeout)
+            response.raise_for_status()  # Raises a HTTPError if the response was unsuccessful
+            result = response.text
+        except requests.exceptions.RequestException as x:
+            print(type(x), x)
+            result = "0.0.0.0"
     return result
 
 
 class EnvironmentVariables:
-    easy_version = "1.2.0"
+    easy_version = "1.2.2"
     server_host_name = socket.gethostname()
     user_home_dir = path.expanduser("~")
     dotenv_file = f"{user_home_dir}/.easynode.env"
     active_user = path.split(user_home_dir)[-1]
     harmony_dir = environ.get("HARMONY_DIR") or f"{user_home_dir}/harmony"
     bls_key_file = path.join(harmony_dir, "blskey.pass")
     hmy_app = path.join(harmony_dir, "hmy")
@@ -35,14 +41,15 @@
     password_path = path.join(harmony_dir, "passphrase.txt")
     external_ip = get_url()
     main_menu_regular = path.join(toolbox_location, "src", "messages", "regularmenu.txt")
     rpc_endpoints = ["https://api.s0.t.hmny.io", "https://api.harmony.one", "https://rpc.ankr.com/harmony"]
     rpc_endpoints_max_connection_retries = 10
     hmy_tmp_path = "/tmp/hmy"
     harmony_tmp_path = "/tmp/harmony"
+    folder_checks = ["harmony", "harmony0", "harmony1", "harmony2", "harmony3", "harmony4"]
 
     @staticmethod
     def get_working_endpoint(endpoints):
         for endpoint in endpoints:
             try:
                 response = requests.get(endpoint, timeout=5)
                 if response.status_code == 200:
```

### Comparing `harmony_toolbox-1.2.0/src/toolbox/library.py` & `harmony_toolbox-1.2.2/src/toolbox/library.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import psutil, platform, dotenv, os, subprocess, requests, pyhmy, shutil, hashlib, re, json, subprocess, getpass
 from os import environ
 from dotenv import load_dotenv
 from simple_term_menu import TerminalMenu
 from colorama import Fore, Style, Back
-from pathlib import Path
-from pyhmy import account, staking, validator, numbers
+from pyhmy import account, staking, numbers
 from json import load, dump
 from toolbox.config import EnvironmentVariables
 from collections import namedtuple
 from datetime import datetime
 from subprocess import PIPE, run
+from concurrent.futures import ThreadPoolExecutor
+from typing import Tuple
 
 load_dotenv(EnvironmentVariables.dotenv_file)
 
 
 class print_stuff:
     def __init__(self, reset: int = 0):
         self.reset = reset
@@ -53,15 +54,15 @@
     return
 
 
 # loader intro splash screen
 def loader_intro():
     print(Fore.GREEN)
     print_stars()
-    p = f"""
+    p = """
                     ____ ____ ____ ____ _________ ____ ____ ____ ____           
                     ||E |||a |||s |||y |||       |||N |||o |||d |||e ||          
                     ||__|||__|||__|||__|||_______|||__|||__|||__|||__||          
                     |/__\|/__\|/__\|/__\|/_______\|/__\|/__\|/__\|/__\|          
                 ____ ____ ____ ____ ____ ____ ____ _________ ____ ____ ____ 
                 ||H |||a |||r |||m |||o |||n |||y |||       |||O |||N |||E ||
                 ||__|||__|||__|||__|||__|||__|||__|||_______|||__|||__|||__||
@@ -76,29 +77,56 @@
                             |/__\|/__\|/__\|/__\|/__\|/__\|/__\|   
     """
     print(p)
 
 
 def old_toolbox_check():
     if os.path.exists(f"{EnvironmentVariables.user_home_dir}/validatortoolbox"):
-        print_stars()
         print(
             Fore.GREEN
-            + "*\n* Old folder found, Exiting toolbox.\n*\n* Please renmae your ~/validatortoolbox folder to ~/harmony-toolbox and update your command paths!\n*\n* Run: cd ~/ && mv ~/validatortoolbox ~/harmony-toolbox\n*\n* After you run the move command, relaunch with: python3 ~/harmony-toolbox/src/menu.py\n*"
+            + f"{string_stars()}\n* Old folder found, Exiting toolbox.\n*\n* Please renmae your ~/validatortoolbox folder to ~/harmony-toolbox and update your command paths!\n*\n* Run: cd ~/ && mv ~/validatortoolbox ~/harmony-toolbox\n*\n* After you run the move command, relaunch with: python3 ~/harmony-toolbox/src/menu.py\n*{string_stars()}"
         )
-        print_stars()
         raise SystemExit(0)
 
 
 # Install Harmony ONE
-def install_hmy():
-    os.chdir(f"{environ.get('HARMONY_DIR')}")
-    process_command(f"curl -LO https://harmony.one/hmycli && mv hmycli hmy && chmod +x hmy")
-    print_stars()
-    print("* hmy application installed.")
+def update_hmy_binary():
+    load_dotenv(EnvironmentVariables.dotenv_file)
+    hmy_dir = environ.get("HARMONY_DIR")
+    download_url = "https://harmony.one/hmycli"
+    destination_path = f"{hmy_dir}/hmy"
+
+    try:
+        # Download the hmycli
+        response = requests.get(download_url, stream=True)
+        response.raise_for_status()
+
+        # Save the downloaded content to the destination path
+        with open(destination_path, "wb") as file:
+            for chunk in response.iter_content(chunk_size=8192):
+                file.write(chunk)
+
+        # Set execute permissions
+        os.chmod(destination_path, 0o755)
+
+        # Get version string
+        software_versions = version_checks(hmy_dir)
+
+        if software_versions:
+            print(f"* hmy application installed.")
+            return software_versions
+        else:
+            print(f"* Version Check Failed.")
+            return None
+
+    except requests.RequestException as e:
+        print(f"* Error while downloading hmy using requests: {e}")
+
+    except OSError as e:
+        print(f"* Error while saving or setting permissions for hmy: {e}")
 
 
 # Code to update the harmony.conf after an upgrade and other text files.
 def update_text_file(fileName, originalText, newText):
     with open(fileName, "r") as f:
         filedata = f.read()
 
@@ -106,68 +134,62 @@
 
     with open(fileName, "w") as f:
         f.write(newdata)
 
 
 # Setup a wallet, ask if they need to import one (not required but no toolbox menu without a wallet)
 def recover_wallet():
-    print_stars()
-    print("* Wallet Configuration                                                                      *")
-    print_stars()
+    print(
+        f"{string_stars()}\n* Wallet Configuration                                                                      *\n{string_stars()}\n"
+    )
     question = ask_yes_no(
-        f"* If you would like to import a wallet for manual wallet actions, and for using our claim and send functions, answer yes.\n* If you only want to load your validator address for stats answer no.\n* Would you like to add your wallet to this server? (YES/NO) "
+        "* If you would like to import a wallet for manual wallet actions, and for using our claim and send functions, answer yes.\n* If you only want to load your validator address for stats answer no.\n* Would you like to add your wallet to this server? (YES/NO) "
     )
     # if yes, find recovery type
     if question:
         recovery_type()
         load_var_file(EnvironmentVariables.dotenv_file)
         print(
-            f'\n* Verify the address above matches the address below:\n* Detected Wallet: {Fore.YELLOW}{environ.get("VALIDATOR_WALLET")}{Fore.GREEN}\n* If a different wallet is showing you can remove it and retry it after installation.\n*\n* .{environ.get("HARMONY_DIR")}/hmy keys remove {EnvironmentVariables.active_user}\n*\n* To restore a wallet once again, run the following:\n*\n* .{environ.get("HARMONY_DIR")}/hmy keys recover-from-mnemonic {EnvironmentVariables.active_user} {environ.get("PASS_SWITCH")}\n*'
+            f'\n* Verify the address above matches the address below:\n* Detected Wallet: {Fore.YELLOW}{environ.get("VALIDATOR_WALLET")}{Fore.GREEN}\n* If a different wallet is showing you can remove it and retry it after installation.\n*\n* .{environ.get("HARMONY_DIR")}/hmy keys remove {EnvironmentVariables.active_user}\n*\n* To restore a wallet once again, run the following:\n*\n* .{environ.get("HARMONY_DIR")}/hmy keys recover-from-mnemonic {EnvironmentVariables.active_user} {environ.get("PASS_SWITCH")}\n{string_stars()}'
         )
-        print_stars()
         input("* Verify your wallet information above.\n* Press ENTER to continue Installation.")
     else:
         while True:
             wallet = input(
-                f"* If you'd like to use the management menu, we need a one1 or 0x address, please input your address now: "
+                "* If you'd like to use the management menu, we need a one1 or 0x address, please input your address now: "
             )
             if wallet.startswith("one1") or wallet.startswith("0x"):
                 # Re-enter the wallet to verify
-                verify_wallet = input(f"* Please re-enter your wallet address for verification: ")
+                verify_wallet = input("* Please re-enter your wallet address for verification: ")
                 if wallet == verify_wallet:
                     set_var(EnvironmentVariables.dotenv_file, "VALIDATOR_WALLET", wallet)
                     break
                 else:
                     print("The entered wallets do not match. Please try again.")
             else:
                 print("Invalid wallet address. It should start with one1 or 0x. Please try again.")
     return
 
 
-def pull_harmony_update(harmony_dir, harmony_conf):
+def update_harmony_binary():
     arch = os.uname().machine
+    harmony_dir = environ.get("HARMONY_DIR")
     os.chdir(f"{harmony_dir}")
-    if environ.get("NETWORK") == "testnet":
-        process_command("curl -LO https://harmony.one/binary_testnet && mv binary_testnet harmony && chmod +x harmony")
-        process_command("./harmony config dump --network testnet harmony.conf")
-    if environ.get("NETWORK") == "mainnet":
-        if arch.startswith("arm"):
-            process_command("curl -LO https://harmony.one/binary-arm64 && mv binary-arm64 harmony && chmod +x harmony")
-        if arch == "x86_64":
-            process_command("curl -LO https://harmony.one/binary && mv binary harmony && chmod +x harmony")
-        process_command("./harmony config dump harmony.conf")
-    update_text_file(harmony_conf, "MaxKeys = 10", "MaxKeys = 13")
-    update_text_file(harmony_conf, " DisablePrivateIPScan = false", " DisablePrivateIPScan = true")
-    print_stars()
-    print("* harmony.conf MaxKeys modified to 13 & DisablePrivateIPScan set to true.")
-    if os.path.isfile(f"{environ.get('HARMONY_DIR')}/blskey.pass"):
-        update_text_file(harmony_conf, 'PassFile = ""', f'PassFile = "blskey.pass"')
+    if arch.startswith("arm"):
+        process_command("curl -LO https://harmony.one/binary-arm64 && mv binary-arm64 harmony && chmod +x harmony")
+    if arch == "x86_64":
+        process_command("curl -LO https://harmony.one/binary && mv binary harmony && chmod +x harmony")
+    process_command("./harmony config dump harmony.conf")
+    update_text_file(f"{harmony_dir}/harmony.conf", "MaxKeys = 10", "MaxKeys = 13")
+    update_text_file(f"{harmony_dir}/harmony.conf", " DisablePrivateIPScan = false", " DisablePrivateIPScan = true")
+    print(f"* harmony.conf MaxKeys modified to 13 & DisablePrivateIPScan set to true.")
+    if os.path.isfile(f"{harmony_dir}/blskey.pass"):
+        update_text_file(f"{harmony_dir}/harmony.conf", 'PassFile = ""', 'PassFile = "blskey.pass"')
         print("* blskey.pass found, updated harmony.conf")
-    print_stars()
-    print(f"* Harmony {environ.get('NETWORK')} application installed & ~/harmony/harmony.conf created. ")
+    print(f"* Harmony binary installed & {harmony_dir}/harmony.conf created. ")
     return
 
 
 # Search harmony.conf for the proper port to hit
 def find_port(folder):
     with open(f"{folder}/harmony.conf") as f:
         data_file = f.readlines()
@@ -179,138 +201,121 @@
                 return line[9:]
             count += 1
 
 
 # build list of installs
 def get_folders():
     folders = {}
-    if os.path.isfile(f"{EnvironmentVariables.user_home_dir}/harmony/harmony.conf"):
-        port = find_port(f"{EnvironmentVariables.user_home_dir}/harmony")
-        folders["harmony"] = port
-        print(f"* Found ~/harmony folder, on port {port}")
-    if os.path.isfile(f"{EnvironmentVariables.user_home_dir}/harmony0/harmony.conf"):
-        port = find_port(f"{EnvironmentVariables.user_home_dir}/harmony0")
-        folders["harmony0"] = port
-        print(f"* Found ~/harmony1 folder, on port {port}")
-    if os.path.isfile(f"{EnvironmentVariables.user_home_dir}/harmony1/harmony.conf"):
-        port = find_port(f"{EnvironmentVariables.user_home_dir}/harmony1")
-        folders["harmony1"] = port
-        print(f"* Found ~/harmony1 folder, on port {port}")
-    if os.path.isfile(f"{EnvironmentVariables.user_home_dir}/harmony2/harmony.conf"):
-        port = find_port(f"{EnvironmentVariables.user_home_dir}/harmony2")
-        folders["harmony2"] = port
-        print(f"* Found ~/harmony2 folder, on port {port}")
-    if os.path.isfile(f"{EnvironmentVariables.user_home_dir}/harmony3/harmony.conf"):
-        port = find_port(f"{EnvironmentVariables.user_home_dir}/harmony3")
-        folders["harmony3"] = port
-        print(f"* Found ~/harmony3 folder, on port {port}")
+    for f in EnvironmentVariables.folder_checks:
+        if os.path.isfile(f"{EnvironmentVariables.user_home_dir}/{f}/harmony.conf"):
+            port = find_port(f"{EnvironmentVariables.user_home_dir}/{f}")
+            folders[f"{f}"] = port
+            print(f"* Found ~/{f} folder, on port {port}")
     print_stars()
     return folders
 
 
-def validator_stats_output(folders) -> None:
+def process_folder(folder, port):
+    if folder == "None":
+        return
+    current_full_path = f"{EnvironmentVariables.user_home_dir}/{folder}"
+    software_versions = version_checks(current_full_path)
+    try:
+        local_server = [
+            f"{EnvironmentVariables.user_home_dir}/{folder}/hmy",
+            "utility",
+            "metadata",
+            f"--node=http://localhost:{port}",
+        ]
+        result_local_server = run(local_server, stdout=PIPE, stderr=PIPE, universal_newlines=True)
+        local_data = json.loads(result_local_server.stdout)
+        remote_server = [
+            f"{EnvironmentVariables.user_home_dir}/{folder}/hmy",
+            "utility",
+            "metadata",
+            f"--node=https://api.s{local_data['result']['shard-id']}.t.hmny.io",
+        ]
+        result_remote_server = run(remote_server, stdout=PIPE, stderr=PIPE, universal_newlines=True)
+        remote_data = json.loads(result_remote_server.stdout)
+        if local_data["result"]["shard-id"] == 0:
+            result_string = (
+                f'* Results for the current folder: {current_full_path}\n* Current harmony version: {Fore.YELLOW}{software_versions["harmony_version"]}{Fore.GREEN}, has upgrade available: {software_versions["harmony_upgrade"]}\n* Current hmy version: {Fore.YELLOW}{software_versions["hmy_version"]}{Fore.GREEN}, has upgrade available: {software_versions["hmy_upgrade"]}'
+                + f"\n* Remote Shard {local_data['result']['shard-id']} Epoch: {remote_data['result']['current-epoch']}, Current Block: {remote_data['result']['current-block-number']}"
+                + f"\n*  Local Shard {local_data['result']['shard-id']} Epoch: {local_data['result']['current-epoch']}, Current Block: {(local_data['result']['current-block-number'])}"
+                + f"\n*   Local Shard {local_data['result']['shard-id']} Size: {get_db_size(f'{current_full_path}', local_data['result']['shard-id'])}"
+            )
+        else:
+            result_string = (
+                f'* Results for the current folder: {current_full_path}\n* Current harmony version: {Fore.YELLOW}{software_versions["harmony_version"]}{Fore.GREEN}, has upgrade available: {software_versions["harmony_upgrade"]}\n* Current hmy version: {Fore.YELLOW}{software_versions["hmy_version"]}{Fore.GREEN}, has upgrade available: {software_versions["hmy_upgrade"]}'
+                + f"\n* Remote Shard {local_data['result']['shard-id']} Epoch: {remote_data['result']['current-epoch']}, Current Block: {remote_data['result']['current-block-number']}"
+                + f"\n*  Local Shard {local_data['result']['shard-id']} Epoch: {local_data['result']['current-epoch']}, Current Block: {(local_data['result']['current-block-number'])}"
+                + f"\n*   Local Shard 0 Size: {get_db_size(f'{current_full_path}', '0')}\n*   Local Shard {local_data['result']['shard-id']} Size: {get_db_size(f'{current_full_path}', local_data['result']['shard-id'])}"
+            )
+        result_string += f"\n{string_stars()}"
+        return result_string
+    except Exception as e:
+        error_message = f"* Error, Service Offline or Unresponsive on port {port}: {e}"
+        return error_message
+
+
+def validator_stats_output() -> None:
+    folders = get_folders()
     config = EnvironmentVariables()
     # Get server stats & wallet balances
     load_1, load_5, load_15 = os.getloadavg()
     sign_percentage = get_sign_pct()
-    total_balance = get_wallet_balance(environ.get("VALIDATOR_WALLET"))
+    validator_wallet_balance = get_wallet_balance(environ.get("VALIDATOR_WALLET"))
     # Print Menu
-    print_stars()
     print(
-        f"{Fore.GREEN}* harmony-toolbox for {Fore.CYAN}Harmony ONE{Fore.GREEN} Validators by Easy Node   v{EnvironmentVariables.easy_version}{Style.RESET_ALL}{Fore.WHITE}   https://easynode.pro {Fore.GREEN}*"
+        f"{Fore.GREEN}{string_stars()}\n* harmony-toolbox for {Fore.CYAN}Harmony ONE{Fore.GREEN} Validators by Easy Node   v{EnvironmentVariables.easy_version}{Style.RESET_ALL}{Fore.WHITE}   https://easynode.pro {Fore.GREEN}*"
     )
-    print_stars()
     print(
-        f'* Your validator wallet address is: {Fore.RED}{str(environ.get("VALIDATOR_WALLET"))}{Fore.GREEN}\n* Your $ONE balance is:             {Fore.CYAN}{str(round(total_balance, 2))}{Fore.GREEN}\n* Your pending $ONE rewards are:    {Fore.CYAN}{str(round(get_rewards_balance(config.working_rpc_endpoint, environ.get("VALIDATOR_WALLET")), 2))}{Fore.GREEN}\n* Server Hostname & IP:             {EnvironmentVariables.server_host_name} - {Fore.YELLOW}{EnvironmentVariables.external_ip}{Fore.GREEN}'
+        f'{string_stars()}\n* Your validator wallet address is: {Fore.RED}{str(environ.get("VALIDATOR_WALLET"))}{Fore.GREEN}\n* Your $ONE balance is:             {Fore.CYAN}{str(round(validator_wallet_balance, 2))}{Fore.GREEN}\n* Your pending $ONE rewards are:    {Fore.CYAN}{str(round(get_rewards_balance(config.working_rpc_endpoint, environ.get("VALIDATOR_WALLET")), 2))}{Fore.GREEN}\n* Server Hostname & IP:             {EnvironmentVariables.server_host_name} - {Fore.YELLOW}{EnvironmentVariables.external_ip}{Fore.GREEN}'
     )
     for folder in folders:
         harmony_service_status(folder)
     print(
         f"* Epoch Signing Percentage:         {Style.BRIGHT}{Fore.GREEN}{Back.BLUE}{sign_percentage} %{Style.RESET_ALL}{Fore.GREEN}\n* Current user home dir free space: {Fore.CYAN}{free_space_check(EnvironmentVariables.user_home_dir): >6}{Fore.GREEN}"
     )
     print(
-        f"* CPU Load Averages: {round(load_1, 2)} over 1 min, {round(load_5, 2)} over 5 min, {round(load_15, 2)} over 15 min"
+        f"* CPU Load Averages: {round(load_1, 2)} over 1 min, {round(load_5, 2)} over 5 min, {round(load_15, 2)} over 15 min\n{string_stars()}"
     )
-    print_stars()
     remote_shard_0 = [
         f"{EnvironmentVariables.user_home_dir}/{list(folders.items())[0][0]}/hmy",
         "utility",
         "metadata",
-        f"--node=https://api.s0.t.hmny.io",
+        "--node=https://api.s0.t.hmny.io",
     ]
     result_shard_0 = run(remote_shard_0, stdout=PIPE, stderr=PIPE, universal_newlines=True)
     remote_0_data = json.loads(result_shard_0.stdout)
     print(
-        f"* Remote Shard 0 Epoch: {remote_0_data['result']['current-epoch']}, Current Block: {remote_0_data['result']['current-block-number']}"
+        f"* Remote Shard 0 Epoch: {remote_0_data['result']['current-epoch']}, Current Block: {remote_0_data['result']['current-block-number']}\n{string_stars()}"
     )
-    print_stars()
-    for folder in folders:
-        current_full_path = f"{EnvironmentVariables.user_home_dir}/{folder}"
-        software_versions = version_checks(current_full_path)
-        print(
-            f'* Results for the current folder: {current_full_path}\n* Current harmony version: {Fore.YELLOW}{software_versions["harmony_version"]}{Fore.GREEN}, has upgrade available: {software_versions["harmony_upgrade"]}\n* Current hmy version: {Fore.YELLOW}{software_versions["hmy_version"]}{Fore.GREEN}, has upgrade available: {software_versions["hmy_upgrade"]}'
-        )
-        local_server = [
-            f"{EnvironmentVariables.user_home_dir}/{folder}/hmy",
-            "utility",
-            "metadata",
-            f"--node=http://localhost:{folders[folder]}",
-        ]
-        result_local_server = run(local_server, stdout=PIPE, stderr=PIPE, universal_newlines=True)
-        try:
-            local_data = json.loads(result_local_server.stdout)
-            remote_server = [
-                f"{EnvironmentVariables.user_home_dir}/{folder}/hmy",
-                "utility",
-                "metadata",
-                f"--node=https://api.s{local_data['result']['shard-id']}.t.hmny.io",
-            ]
-            result_remote_server = run(remote_server, stdout=PIPE, stderr=PIPE, universal_newlines=True)
-            remote_data = json.loads(result_remote_server.stdout)
-            print(
-                f"* Remote Shard {local_data['result']['shard-id']} Epoch: {remote_data['result']['current-epoch']}, Current Block: {remote_data['result']['current-block-number']}"
-            )
-            if local_data["result"]["shard-id"] == 0:
-                print(
-                    f"*  Local Shard {local_data['result']['shard-id']} Epoch: {local_data['result']['current-epoch']}, Current Block: {(local_data['result']['current-block-number'])}"
-                    + f"\n*   Local Shard {local_data['result']['shard-id']} Size: {get_db_size(f'{current_full_path}', local_data['result']['shard-id'])}"
-                )
-            else:
-                print(
-                    f"*  Local Shard {local_data['result']['shard-id']} Epoch: {local_data['result']['current-epoch']}, Current Block: {(local_data['result']['current-block-number'])}"
-                    + f"\n*   Local Shard 0 Size: {get_db_size(f'{current_full_path}', '0')}\n*   Local Shard {local_data['result']['shard-id']} Size: {get_db_size(f'{current_full_path}', local_data['result']['shard-id'])}"
-                )
 
-            print_stars()
-        except Exception as e:
-            print(f"* Error, Service Offline or Unresponsive: {e}")
-            print_stars()
+    # Concurrently process each folder
+    with ThreadPoolExecutor(max_workers=10) as executor:
+        folder_results = list(executor.map(process_folder, folders.keys(), folders.values()))
+
+    # Now print results for each folder
+    for result in folder_results:
+        if result:
+            print(result)
 
 
 def harmony_service_status(service="harmony") -> None:
     status = subprocess.call(["systemctl", "is-active", "--quiet", service])
     if status == 0:
-        if service == "harmony":
-            print(
-                f"* {service} Service is:               "
-                + Fore.BLACK
-                + Back.GREEN
-                + "   Online  "
-                + Style.RESET_ALL
-                + Fore.GREEN
-            )
-        else:
-            print(
-                f"* {service} Service is:              "
-                + Fore.BLACK
-                + Back.GREEN
-                + "   Online  "
-                + Style.RESET_ALL
-                + Fore.GREEN
-            )
+        print(
+            f"* {service} Service is:               "
+            + Fore.BLACK
+            + Back.GREEN
+            + "   Online  "
+            + Style.RESET_ALL
+            + Fore.GREEN
+        )
     else:
         print(
             f"* {service} Service is:               "
             + Fore.WHITE
             + Back.RED
             + "  *** Offline *** "
             + Style.RESET_ALL
@@ -338,43 +343,45 @@
     harmony_db_size = harmony_db_size.rstrip("\t")
     countTrim = len(environ.get("HARMONY_DIR")) + 13
     return harmony_db_size[:-countTrim]
 
 
 def recovery_type():
     print_stars()
-    print("* Wallet Recovery Type!                                                                     *")
-    print_stars()
+    print(
+        f"{string_stars()}\n* Wallet Recovery Type!                                                                     *\n{string_stars()}"
+    )
     print("* [0] = Mnemonic phrase recovery (aka seed phrase)                                          *")
-    print("* [1] = Private Key recovery                                                                *")
-    print_stars()
+    print(
+        f"* [1] = Private Key recovery                                                                *\n{string_stars()}"
+    )
     menu_options = [
         "[0] - Mnemonic Phrase Recovery",
         "[1] - Private Key Recovery",
     ]
     terminal_menu = TerminalMenu(
         menu_options, title="* Which type of restore method would you like to use for your validator wallet?"
     )
     results = terminal_menu.show()
     passphrase_set()
     if results == 0:
         # Mnemonic Recovery Here
-        process_command(
-            f"{environ.get('HARMONY_DIR')}/hmy keys recover-from-mnemonic {EnvironmentVariables.active_user} --passphrase-file passphrase.txt"
+        # --passphrase-file passphrase.txt not working atm on ./hmy keys
+        run_command(
+            f"{environ.get('HARMONY_DIR')}/hmy keys recover-from-mnemonic {EnvironmentVariables.active_user} --passphrase"
         )
-        print_stars()
         set_wallet_env()
     elif results == 1:
         # Private Key Recovery Here
         print("* Private key recovery requires your private information in the command itself.")
-        private = input("* Please enter your private key to restore your wallet: ")
-        process_command(
-            f"{environ.get('HARMONY_DIR')}/hmy keys import-private-key {private} {EnvironmentVariables.active_user} --passphrase-file passphrase.txt"
+        private = getpass.getpass("* Please enter your private key to restore your wallet: ")
+        # --passphrase-file passphrase.txt not working atm on ./hmy keys
+        run_command(
+            f"{environ.get('HARMONY_DIR')}/hmy keys import-private-key {private} {EnvironmentVariables.active_user} --passphrase"
         )
-        print_stars()
         set_wallet_env()
 
 
 def passphrase_status():
     load_var_file(EnvironmentVariables.dotenv_file)
     if os.path.exists(EnvironmentVariables.hmy_wallet_store):
         passphrase_set()
@@ -387,18 +394,18 @@
         set_var(EnvironmentVariables.dotenv_file, "PASS_SWITCH", "--passphrase")
     load_var_file(EnvironmentVariables.dotenv_file)
 
 
 def passphrase_set():
     if os.path.exists(f"{environ.get('HARMONY_DIR')}/passphrase.txt"):
         return
-    import getpass
 
-    print(f"* Setup {environ.get('HARMONY_DIR')}/passphrase.txt file for use with autobidder & harmony-toolbox.")
-    print_stars()
+    print(
+        f"{Fore.GREEN}* Setup {environ.get('HARMONY_DIR')}/passphrase.txt file for use with autobidder & harmony-toolbox.\n{string_stars()}"
+    )
     # take input
     while True:
         print("* ")
         password_1 = getpass.getpass(
             prompt="* Please set a wallet password for this node\n* Enter your password now: ", stream=None
         )
         password_2 = getpass.getpass(prompt="* Re-enter your password: ", stream=None)
@@ -409,27 +416,43 @@
             break
     # Save file, we won't encrypt because if someone has access to the file, they will also have the salt and decrypt code at their disposal.
     save_text(f"{environ.get('HARMONY_DIR')}/passphrase.txt", password_1)
     load_var_file(EnvironmentVariables.dotenv_file)
     passphrase_status()
 
 
-def process_command(command: str, shell=True, print_output=True) -> bool:
+def process_command(command: str, shell=True, print_output=True) -> Tuple[bool, str]:
     result = subprocess.run(command, shell=shell, stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
 
-    if print_output and result.stdout:
-        print(result.stdout)
+    # Command was successful
+    if result.returncode == 0:
+        if print_output and result.stdout:
+            print(result.stdout)
+        return True, result.stdout
 
-    if result.returncode != 0:
+    # Command failed
+    if print_output:
+        print(f"Error executing command: {result.stderr}")
+    return False, result.stderr
+
+
+def run_command(command: str, shell=True, print_output=True) -> bool:
+    try:
+        if print_output:
+            subprocess.run(command, shell=shell, check=True)
+        else:
+            # Suppress the output if print_output is set to False
+            with open(os.devnull, "w") as fnull:
+                subprocess.run(command, shell=shell, check=True, stdout=fnull, stderr=fnull)
+        return True
+    except subprocess.CalledProcessError as e:
         if print_output:
-            print(f"Error executing command: {result.stderr}")
+            print(f"Error executing command: {e}")
         return False
 
-    return True
-
 
 def ask_yes_no(question: str) -> bool:
     yes_no_answer = ""
     while not yes_no_answer.startswith(("Y", "N")):
         yes_no_answer = input(f"{question}: ").upper()
     if yes_no_answer.startswith("Y"):
         return True
@@ -468,15 +491,15 @@
     command = f"{environ.get('HARMONY_DIR')}/hmy keys list"
     result = subprocess.run(command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
 
     if result.returncode != 0:
         print(f"Error executing command: {result.stderr}")
         return None
 
-    lines = result.stdout.strip().split('\n')
+    lines = result.stdout.strip().split("\n")
     for line in lines[2:]:  # Skip the header line & blank
         name, address = line.strip().split(None, 1)  # Split by whitespace, max 1 split
         if address == wallet_id:
             return name
 
     print(f"Wallet ID {wallet_id} not found in the output.")
     return None
@@ -500,22 +523,24 @@
         "One1000Lakes",
         "ONECelestial",
         "PeaceLoveHarmony",
         "PiStake",
         "Quick.One",
         "TEC Viva",
         "Tr4ck3r",
-        "Quit"
+        "Quit",
     ]
 
     selected_indexes = []
     selected_names = []
 
     for _ in range(7):
-        print("* Highlight an option and hit enter to add it to your list.\n* (pick up to 7, 'Quit' to finish if less than 7 selections):")
+        print(
+            "* Highlight an option and hit enter to add it to your list.\n* (pick up to 7, 'Quit' to finish if less than 7 selections):"
+        )
         terminal_menu = TerminalMenu(options, title="Choose a governance member:")
         choice_index = terminal_menu.show()
 
         # Check if the "Quit" option was selected
         if choice_index == len(options) - 1:
             print("Quitting the selection process.")
             break
@@ -531,19 +556,15 @@
     # Return selected indexes and names as a string
     selected_indexes_str = "[" + ", ".join(map(str, [index + 1 for index in selected_indexes])) + "]"
     selected_names_str = "[" + ", ".join(selected_names) + "]"
     return selected_indexes_str, selected_names_str
 
 
 def proposal_choices_option() -> None:
-    options = [
-        "HIP-30v2",
-        "Governance for Harmony Recovery Wallet",
-        "Quit"
-    ]
+    options = ["HIP-30v2", "Governance for Harmony Recovery Wallet", "Quit"]
 
     print("* Current proposals:\n*\n*")
 
     terminal_menu = TerminalMenu(options, title="Choose a proposal to vote on:")
     choice_index = terminal_menu.show()
 
     # Check if the "Quit" option was selected
@@ -555,18 +576,20 @@
     selected_proposal = options[choice_index]
     question = ask_yes_no(f"* Would you like to vote on {selected_proposal}? (YES/NO): ")
     if question:
         return question, selected_proposal
     else:
         return question, None
 
+
 def get_vote_choice() -> (int, str):
     print(Fore.GREEN)
-    print("* How would you like to vote on this proposal?                                                 *")
-    print_stars()
+    print(
+        f"* How would you like to vote on this proposal?                                                 *\n{string_stars()}"
+    )
     menu_options = [
         "[1] - Yes",
         "[2] - No",
         "[3] - Abstain",
         "[4] - Quit",
     ]
     terminal_menu = TerminalMenu(menu_options, title="* Which Shard will this node operate on? ")
@@ -574,81 +597,98 @@
     if vote_choice_index == 3:  # The index of the "Quit" option
         return None, "Quit"
     vote_choice_num = vote_choice_index + 1
     vote_choice_text = menu_options[vote_choice_index].split(" - ")[1]
     return vote_choice_num, vote_choice_text
 
 
+def get_available_space(directory: str) -> int:
+    """Returns available space in given directory in GB."""
+    statvfs = os.statvfs(directory)
+    return (statvfs.f_frsize * statvfs.f_bavail) / (1024**3)
+
+
+def check_space_requirements(shard: int, directory: str) -> bool:
+    available_space = get_available_space(directory)
+    if shard == 0 and available_space < 400:
+        if not os.listdir(directory):
+            shutil.rmtree(f"{directory}")
+        os.remove(f"{EnvironmentVariables.user_home_dir}/.easynode.env")
+        input(f"* Warning: There is not enough space to load shard 0 into {directory}.\n* Restart the toolbox and select a volume with more free space when prompted on the install location.\n* Press ENTER to quit.")
+        raise SystemExit(0)
+    elif shard in [1, 2, 3] and available_space < 50:
+        if not os.listdir(directory):
+            shutil.rmtree(f"{directory}")
+        os.remove(f"{EnvironmentVariables.user_home_dir}/.easynode.env")
+        input(f"* Warning: There is not enough space to load shard {shard} into {directory}.\n* Restart the toolbox and select a volume with more free space when prompted on the install location.\n* Press ENTER to quit.")
+        raise SystemExit(0)
+    return True
+
+
 def get_shard_menu() -> None:
     if not environ.get("SHARD"):
-        print_stars()
-        print("* Gathering more information about your server.                                             *")
-        print_stars()
-        print("* Which shard do you want this node run on?                                                 *")
-        print_stars()
+        print(f"{string_stars()}\n* Gathering more information about your server.\n{string_stars()}")
+        print(f"* Which shard do you want this node to sign blocks on?\n{string_stars()}")
         menu_options = [
             "[0] - Shard 0",
             "[1] - Shard 1",
             "[2] - Shard 2",
             "[3] - Shard 3",
         ]
-        terminal_menu = TerminalMenu(menu_options, title="* Which Shard will this node operate on? ")
-        our_shard = str(terminal_menu.show())
-        set_var(EnvironmentVariables.dotenv_file, "SHARD", our_shard)
+        terminal_menu = TerminalMenu(menu_options, title="* Which Shard will this node sign blocks on? ")
+        our_shard = int(terminal_menu.show())
+
+        set_var(EnvironmentVariables.dotenv_file, "SHARD", str(our_shard))
         return our_shard
 
 
 def set_main_or_test() -> None:
-    if not environ.get("NETWORK"):
-        print_stars()
-        print("* Setup config not found, which blockchain does this node run on?                           *")
-        print_stars()
-        print("* [0] - Mainnet                                                                             *")
-        print("* [1] - Testnet                                                                             *")
-        print_stars()
-        menu_options = [
-            "[0] Mainnet",
-            "[1] Testnet",
-        ]
-        terminal_menu = TerminalMenu(menu_options, title="Mainnet or Testnet")
-        results = terminal_menu.show()
-        if results == 0:
-            set_var(EnvironmentVariables.dotenv_file, "NETWORK", "mainnet")
-            set_var(EnvironmentVariables.dotenv_file, "NETWORK_SWITCH", "t")
-            set_var(EnvironmentVariables.dotenv_file, "RPC_NET", "https://rpc.s0.t.hmny.io")
-            set_var(EnvironmentVariables.dotenv_file, "RPC_NET_SHARD", f"https://rpc.s{environ.get('SHARD')}.t.hmny.io")
-        if results == 1:
-            set_var(EnvironmentVariables.dotenv_file, "NETWORK", "testnet")
-            set_var(EnvironmentVariables.dotenv_file, "NETWORK_SWITCH", "b")
-            set_var(EnvironmentVariables.dotenv_file, "RPC_NET", "https://rpc.s0.b.hmny.io")
-            set_var(EnvironmentVariables.dotenv_file, "RPC_NET_SHARD", f"https://rpc.s{environ.get('SHARD')}.b.hmny.io")
+    if environ.get("NETWORK") != "mainnet":
+        set_network("t")
+    # if not environ.get("NETWORK"):
+    #    print_stars()
+    #    print("* Setup config not found, which blockchain does this node run on?                           *")
+    #    print_stars()
+    #    print("* [0] - Mainnet                                                                             *")
+    #    print("* [1] - Testnet                                                                             *")
+    #    print_stars()
+    #    menu_options = [
+    #        "[0] Mainnet",
+    #        "[1] Testnet",
+    #    ]
+    #    terminal_menu = TerminalMenu(menu_options, title="Mainnet or Testnet")
+    #    results = terminal_menu.show()
+    #    if results == 0:
+    #        set_network("t")
+    #    if results == 1:
+    #        set_network("b")
     return
 
 
 def get_wallet_address():
     print("* Signing Node, No Wallet!                                                                  *")
     print("* You are attempting to launch the menu but no wallet has been loaded, as you chose         *")
-    print("* If you would like to use the menu on the server, complete the following:                  *")
-    print_stars()
+    print(
+        f"* If you would like to use the menu on the server, complete the following:                  *\n{string_stars()}"
+    )
     print("* Edit ~/.easynode.env and add your wallet address on a new line like this example:         *")
-    print("* VALIDATOR_WALLET='one1thisisjustanexamplewalletreplaceme'                                 *")
-    print_stars()
+    print(
+        f"* VALIDATOR_WALLET='one1thisisjustanexamplewalletreplaceme'                                 *\n{string_stars()}"
+    )
     raise SystemExit(0)
 
 
 def get_validator_info():
     config = EnvironmentVariables()
     validator_data = -1
     try:
         validator_data = staking.get_validator_information(environ.get("VALIDATOR_WALLET"), config.working_rpc_endpoint)
         return validator_data
     except Exception:
-        current += 1
-
-    return validator_data
+        return validator_data
 
 
 def current_price():
     try:
         response = requests.get(EnvironmentVariables.onePriceURL, timeout=5)
     except (ValueError, KeyError, TypeError):
         response = "0.0000"
@@ -677,15 +717,15 @@
         return get_balance
 
 
 def get_rewards_balance(endpoint, wallet_addr):
     totalRewards = 0
     try:
         validator_rewards = staking.get_delegations_by_delegator(wallet_addr, endpoint)
-    except (Exception, ConnectionError) as e:
+    except (Exception, ConnectionError):
         return totalRewards
 
     for i in validator_rewards:
         totalRewards = totalRewards + i["reward"]
     totalRewards = pyhmy.numbers.convert_atto_to_one(totalRewards)
 
     if totalRewards >= 0:
@@ -701,27 +741,18 @@
     try:
         with open(fn, "r", encoding="utf-8") as j:
             data = load(j)
             if single_key:
                 return data.get(single_key)
             return data
     except FileNotFoundError as e:
-        # print(f"File not Found  ::  {e}")
+        print(f"File not Found  ::  {e}")
         return {}
 
 
-def wallet_pending_rewards(wallet):
-    res, walletBalance = get_rewards_balance(wallet, save_data=True, display=False)
-    totalRewards = 0
-    for i in walletBalance["result"]:
-        totalRewards = totalRewards + i["reward"]
-    totalRewards = "{:,}".format(round(totalRewards * 0.000000000000000001, 2))
-    return totalRewards
-
-
 def get_sign_pct() -> str:
     config = EnvironmentVariables()
     hmy_external_rpc = f"{environ.get('HARMONY_DIR')}/hmy --node='{config.working_rpc_endpoint}'"
     output = subprocess.getoutput(
         f"{hmy_external_rpc} blockchain validator information {environ.get('VALIDATOR_WALLET')} | grep signing-percentage"
     )
     output_stripped = output.lstrip('        "current-epoch-signing-percentage": "').rstrip('",')
@@ -732,253 +763,303 @@
         return str(roundSignPerc)
     except (OSError, ValueError):
         output_stripped = "0"
         return str(output_stripped)
 
 
 def get_local_version(folder):
-    harmony_version = subprocess.getoutput(f"{folder}/harmony -V")
-    output_harmony_version = re.search(r"version (v\d+-v\d+\.\d+\.\d+-\d+-g[0-9a-f]+ )\(", harmony_version)
-    hmy_version = subprocess.getoutput(f"{folder}/hmy version")
-    return output_harmony_version.group(1)[:-2], hmy_version[62:-15]
+    output_harmony_version = None
+    hmy_version = None
+
+    if os.path.exists(f"{folder}/harmony"):
+        harmony_version = subprocess.getoutput(f"{folder}/harmony -V")
+        match = re.search(r"version (v\d+-v\d+\.\d+\.\d+-\d+-g[0-9a-f]+ )\(", harmony_version)
+        if match:
+            output_harmony_version = match.group(1)[:-2]
+
+    if os.path.exists(f"{folder}/hmy"):
+        hmy_version_raw = subprocess.getoutput(f"{folder}/hmy version")
+        hmy_version = hmy_version_raw[62:-15]
+
+    if not output_harmony_version or not hmy_version:
+        return None
+
+    return output_harmony_version, hmy_version
 
 
 def set_mod_x(file):
     subprocess.run(["chmod", "+x", file])
 
 
 def check_online_version():
+    harmony_version_str = "Offline"
+    hmy_ver = "Offline"
     try:
-        subprocess.check_output(
-            ["wget", "https://harmony.one/binary", "-O", EnvironmentVariables.harmony_tmp_path],
-            stderr=subprocess.STDOUT,
-        )
-        set_mod_x(EnvironmentVariables.harmony_tmp_path)
-        harmony_ver = subprocess.getoutput(f"{EnvironmentVariables.harmony_tmp_path} -V")
-        output_harmony_version = re.search(r"version (v\d+-v\d+\.\d+\.\d+-\d+-g[0-9a-f]+ )\(", harmony_ver)
-    except subprocess.CalledProcessError:
-        print(f"* Error - Website for harmony upgrade is offline, setting to offline.")
-        harmony_ver = "Offline"
-    try:
-        subprocess.check_output(
-            ["wget", "https://harmony.one/hmycli", "-O", EnvironmentVariables.hmy_tmp_path], stderr=subprocess.STDOUT
-        )
-        set_mod_x(EnvironmentVariables.hmy_tmp_path)
-        hmy_ver = subprocess.getoutput(f"{EnvironmentVariables.hmy_tmp_path} version")
-        hmy_ver = hmy_ver[62:-15]
-    except subprocess.CalledProcessError:
-        print(f"* Error - Website for hmy upgrade is offline, setting to offline.")
-        hmy_ver = "Offline"
-    return output_harmony_version.group(1)[:-2], hmy_ver
+        with open(os.devnull, "wb") as devnull:
+            subprocess.call(
+                ["wget", "https://harmony.one/binary", "-O", EnvironmentVariables.harmony_tmp_path],
+                stdout=devnull,
+                stderr=devnull,
+            )
+            set_mod_x(EnvironmentVariables.harmony_tmp_path)
+            harmony_ver = subprocess.getoutput(f"{EnvironmentVariables.harmony_tmp_path} -V")
+            output_harmony_version = re.search(r"version (v\d+-v\d+\.\d+\.\d+-\d+-g[0-9a-f]+ )\(", harmony_ver)
+            harmony_version_str = output_harmony_version.group(1)[:-2]
+            subprocess.call(
+                ["wget", "https://harmony.one/hmycli", "-O", EnvironmentVariables.hmy_tmp_path],
+                stdout=devnull,
+                stderr=devnull,
+            )
+            set_mod_x(EnvironmentVariables.hmy_tmp_path)
+            hmy_ver = subprocess.getoutput(f"{EnvironmentVariables.hmy_tmp_path} version")
+            hmy_ver = hmy_ver[62:-15]
+            return harmony_version_str, hmy_ver
+    except (AttributeError, subprocess.CalledProcessError):
+        # print("* Error - Website for hmy upgrade is offline, setting to offline.")
+        return harmony_version_str, hmy_ver
 
 
 def first_env_check(env_file) -> None:
     first_time = load_var_file(env_file)
     return first_time
 
 
 def version_checks(harmony_folder):
     software_versions = {}
-    software_versions["harmony_version"], software_versions["hmy_version"] = get_local_version(f"{harmony_folder}")
-    software_versions["online_harmony_version"], software_versions["online_hmy_version"] = check_online_version()
+    local_versions = get_local_version(f"{harmony_folder}")
+    online_versions = check_online_version()
+
+    # Check if the local versions exist. If not, set to a default value.
+    software_versions["harmony_version"] = local_versions[0] if local_versions else "Not Found"
+    software_versions["hmy_version"] = local_versions[1] if local_versions else "Not Found"
+
+    # Check if the online versions exist. If not, set to a default value.
+    software_versions["online_harmony_version"] = online_versions[0] if online_versions else "Not Found"
+    software_versions["online_hmy_version"] = online_versions[1] if online_versions else "Not Found"
+
     # Check versions, if matching False (No Upgrade Required), non-match True (Upgrade Required)
     if (
         software_versions["harmony_version"] == software_versions["online_harmony_version"]
         or software_versions["online_harmony_version"] == "Offline"
+        or software_versions["harmony_version"] == "Not Found"
     ):
         software_versions["harmony_upgrade"] = "False"
     else:
         software_versions["harmony_upgrade"] = "True"
+
     if (
         software_versions["hmy_version"] == software_versions["online_hmy_version"]
         or software_versions["online_hmy_version"] == "Offline"
+        or software_versions["hmy_version"] == "Not Found"
     ):
         software_versions["hmy_upgrade"] = "False"
     else:
         software_versions["hmy_upgrade"] = "True"
+
     return software_versions
 
 
 def first_setup():
     # Find Shard #
     get_shard_menu()
     # Get Mainnet or Testnet
     set_main_or_test()
     # Look for a harmony install or install.
     check_for_install()
-    print_stars()
     return
 
 
 # looks for ~/harmony or installs it if it's not there. Asks to overwrite if it finds it, run at your own risk.
 def check_for_install() -> str:
     if os.path.exists(f"{EnvironmentVariables.user_home_dir}/harmony"):
         question = ask_yes_no(
             "* You already have a harmony folder on this system, would you like to re-run installation and rclone on this server? (YES/NO)"
         )
         if question:
             install_harmony()
-            print_stars()
             # Wallet Setup
             recover_wallet()
-            print_stars()
             # Check passphrase if wallet is added
             passphrase_status()
-            print_stars()
-            print("* All harmony files now installed. Database download starting now...")
-            print_stars()
+            print(f"* All harmony files now installed. Database download starting now...\n{string_stars()}")
             clone_shards()
             finish_node_install()
         else:
             if os.path.isdir(f"{EnvironmentVariables.user_home_dir}/harmony"):
                 print(
                     "* Exiting Harmony Validator Toolbox\n* You already have a folder at ~/harmony.\n* Contact Easy Node for help setting up if this is an existing Harmony server."
                 )
             if os.path.isfile(f"{EnvironmentVariables.user_home_dir}/harmony"):
                 print(
                     "* Exiting Harmony Validator Toolbox\n* You already have a file at ~/harmony.\n* Contact Easy Node for help setting up if this is an existing Harmony server with a custom configuration."
                 )
             raise SystemExit(0)
     else:
-        print(f"* You selected Shard: {environ.get('SHARD')}. ")
+        print(f"{Fore.GREEN}* You selected Shard: {environ.get('SHARD')}. ")
         install_harmony()
-        print_stars()
         # Wallet Setup
         recover_wallet()
-        print_stars()
         # Check passphrase if wallet is added
         passphrase_status()
-        print_stars()
-        print("* All harmony files now installed. Database download starting now...")
-        print_stars()
+        print(f"* All harmony files now installed. Database download starting now...\n{string_stars()}")
         clone_shards()
         finish_node_install()
     return
 
 
+def install_rclone():
+    # Fetch the content of the script
+    url = "https://rclone.org/install.sh"
+    response = requests.get(url)
+
+    # Check if the request was successful
+    if response.status_code != 200:
+        print("* Failed to download the script.")
+        return False
+
+    script_content = response.text
+
+    # Execute the fetched content
+    try:
+        process = subprocess.Popen(
+            ["sudo", "bash"], stdin=subprocess.PIPE, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL
+        )
+        process.communicate(input=script_content.encode())
+        if process.returncode != 0:
+            return False
+        return True
+    except Exception as e:
+        print(f"Error: {e}")
+        return False
+
+
 # Installer Module
 def install_harmony() -> None:
-    # Checks Passed at this point, only 1 folder in /mnt and it's probably our volume (can scope this down further later)
-    print_stars()
-    print("* Install Location")
-    print_stars()
-    question = ask_yes_no(
-        f"* Answer yes if you'd like to setup harmony in the default location\n* {EnvironmentVariables.user_home_dir}/harmony\n* Or answer no to choose a custom folder (for a volume or 2nd disk setup): (YES/NO) "
-    )
-    if question:
-        set_var(EnvironmentVariables.dotenv_file, "HARMONY_DIR", f"{EnvironmentVariables.user_home_dir}/harmony")
-    else:
-        answer = input(
-            "\n* Please enter the full path to a location you'd like to install harmony into.\n* The folder should not exist yet for best results (example: /mnt/volume1/harmony): "
+    while True:
+        print(f"{string_stars()}\n* Install Location\n{string_stars()}")
+        default_path = f"{EnvironmentVariables.user_home_dir}/harmony"
+        question = ask_yes_no(
+            f"* Do you want to setup harmony in the default location?\n* {default_path}\n* "
+            "Or select 'No' to choose a custom folder (for a volume or 2nd disk setup): (YES/NO) "
         )
-        if not os.path.exists(answer):
-            question = ask_yes_no(
-                f"* That path {answer} doesn't exist yet.\n* Do you want to create the folder {answer} and install the harmony files here? (YES/NO) "
-            )
-            if question:
-                set_var(EnvironmentVariables.dotenv_file, "HARMONY_DIR", f"{answer}")
-            else:
-                install_harmony()
+        if question:
+            # Has the space, install away
+            install_path = default_path
+            service_name = os.path.basename(default_path)
+            break
         else:
-            question = ask_yes_no(
-                f"* Are you sure you want to isntall into the already existing folder {answer}? (YES/NO) "
+            custom_path = input(
+                "\n* Please enter the full path to a location you'd like to install harmony into.\n* "
+                "We suggest using your shard number at the end of harmony for compatability with toolbox, ie: /home/serviceharmony/harmony1 : "
             )
-            if question:
-                set_var(EnvironmentVariables.dotenv_file, "HARMONY_DIR", f"{answer}")
+            if os.path.exists(custom_path):
+                question = ask_yes_no(
+                    f"* The folder {custom_path} already exists.\n* Are you sure you want to install into this existing folder? (YES/NO) "
+                )
+                if question:
+                    install_path = custom_path
+                    service_name = os.path.basename(custom_path)
+                    break
             else:
-                install_harmony()
-        set_var(EnvironmentVariables.dotenv_file, "HARMONY_DIR", f"{answer}")
-        process_command(f"sudo mkdir -p {environ.get('HARMONY_DIR')}")
-        process_command(f"sudo chown {EnvironmentVariables.active_user} {environ.get('HARMONY_DIR')}")
-    print_stars()
-    print("* Creating all Harmony Files & Folders")
-    process_command(f"mkdir -p {environ.get('HARMONY_DIR')}/.hmy/blskeys")
+                question = ask_yes_no(
+                    f"* The path {custom_path} doesn't exist yet.\n* Do you want to create it and install the harmony files here? (YES/NO) "
+                )
+                if question:
+                    install_path = custom_path
+                    service_name = os.path.basename(custom_path)
+                    break
+
+    set_var(EnvironmentVariables.dotenv_file, "HARMONY_DIR", install_path)
+    set_var(EnvironmentVariables.dotenv_file, "SERVICE_NAME", service_name)
+
+    # Create the directory if not exists, and set ownership
+    process_command(f"sudo mkdir -p {install_path}")
+    process_command(f"sudo chown {EnvironmentVariables.active_user} {install_path}")
+    
+    # Check space requirements for the selected shard
+    shard_value = int(environ.get('SHARD'))
+    check_space_requirements(shard_value, install_path)
+    
+    print(f"{string_stars()}\n* Creating all Harmony Files & Folders")
+    process_command(f"mkdir -p {install_path}/.hmy/blskeys")
 
     # Setup folders now that symlink exists or we know we're using ~/harmony
     if not os.path.isdir(f"{EnvironmentVariables.user_home_dir}/.hmy_cli/account-keys/"):
         process_command(f"mkdir -p {EnvironmentVariables.user_home_dir}/.hmy_cli/account-keys/")
     if not os.path.isdir(f"{environ.get('HARMONY_DIR')}/.hmy/blskeys"):
-        print("* Creating all Harmony Files & Folders")
         process_command(f"mkdir -p {environ.get('HARMONY_DIR')}/.hmy/blskeys")
     # Change to ~/harmony folder
     os.chdir(f"{environ.get('HARMONY_DIR')}")
-    print_stars()
     # Install hmy
-    install_hmy()
-    print_stars()
+    update_hmy_binary()
     # Install harmony
-    pull_harmony_update(environ.get("HARMONY_DIR"), f"{environ.get('HARMONY_DIR')}/harmony.conf")
+    update_harmony_binary()
     # install hmy files
-    print("* Installing rclone application & rclone configuration files")
-    print_stars()
+    print(f"* Installing rclone application & rclone configuration files")
     # check for working rclone site and download
     try:
-        process_command("curl https://rclone.org/install.sh | sudo bash")
+        install_rclone()
     except (ValueError, KeyError, TypeError):
         result = ask_yes_no(
             "* rclone site is offline, we can install rclone from the Ubuntu repo as a workaround, do you want to continue? (Y/N): "
         )
         if result:
             # If rclone curl is down, install rclone with apt instead
             subprocess.run("sudo apt install rclone -y")
+        else:
+            finish_node()
 
     process_command(
         f"mkdir -p {EnvironmentVariables.user_home_dir}/.config/rclone && cp {EnvironmentVariables.toolbox_location}/src/bin/rclone.conf {EnvironmentVariables.user_home_dir}/.config/rclone/"
     )
-    print_stars()
     # Setup the harmony service file
-    print("* Customizing, Moving & Enabling your harmony.service systemd file")
+    print(f"* Customizing, Moving & Enabling your {service_name}.service systemd file")
 
     # Set initial file for customization
     service_file_path = f"{EnvironmentVariables.toolbox_location}/src/bin/harmony.service"
 
     # Read the service file
     with open(service_file_path, "r") as file:
         filedata = file.read()
 
     # Replace the paths with the value of HARMONY_DIR
-    harmony_dir = environ.get("HARMONY_DIR")
-    if harmony_dir:
-        filedata = filedata.replace("WorkingDirectory=/home/serviceharmony/harmony", f"WorkingDirectory={harmony_dir}")
-        filedata = filedata.replace(
-            "ExecStart=/home/serviceharmony/harmony/harmony -c harmony.conf",
-            f"ExecStart={harmony_dir}/harmony -c harmony.conf",
-        )
+    filedata = filedata.replace("WorkingDirectory=/home/serviceharmony/harmony", f"WorkingDirectory={install_path}")
+    filedata = filedata.replace(
+        "ExecStart=/home/serviceharmony/harmony/harmony -c harmony.conf",
+        f"ExecStart={install_path}/harmony -c harmony.conf",
+    )
 
     # Write the file out again
-    with open("harmony.service", "w") as file:
+    with open(f"{service_name}.service", "w") as file:
         file.write(filedata)
 
     # Move the modified service file into place, change the permissions and enable the service
-    # Update these steps in the future to use a dynamic harmony.service name?
-    subprocess.run(["sudo", "mv", "harmony.service", "/etc/systemd/system/harmony.service"], check=True)
-    subprocess.run(["sudo", "chmod", "a-x", "/etc/systemd/system/harmony.service"], check=True)
-    subprocess.run(["sudo", "systemctl", "enable", "harmony.service"], check=True)
+    subprocess.run(["sudo", "mv", f"{service_name}.service", f"/etc/systemd/system/{service_name}.service"], check=True)
+    subprocess.run(["sudo", "chmod", "a-x", f"/etc/systemd/system/{service_name}.service"], check=True)
+    subprocess.run(["sudo", "systemctl", "enable", f"{service_name}.service"], check=True)
 
 
 # Database Downloader
 def clone_shards():
     # Move to ~/harmony
     os.chdir(f"{environ.get('HARMONY_DIR')}")
 
     if environ.get("SHARD") != "0":
         # If we're not on shard 0, download the numbered shard DB here.
-        print(f"* Now cloning shard {environ.get('SHARD')}")
-        print_stars()
-        process_command(
+        print(f"* Now cloning shard {environ.get('SHARD')}\n{string_stars()}")
+        run_command(
             f"rclone -P sync release:pub.harmony.one/{environ.get('NETWORK')}.min/harmony_db_{environ.get('SHARD')} {environ.get('HARMONY_DIR')}/harmony_db_{environ.get('SHARD')} --multi-thread-streams 4 --transfers=32"
         )
-        print_stars()
-        print(f"* Shard {environ.get('SHARD')} completed.\n* Shard 0 will be created when you start your service.")
-        print_stars()
+        print(
+            f"{string_stars()}\n* Shard {environ.get('SHARD')} completed.\n* Shard 0 will be created when you start your service.\n{string_stars()}"
+        )
     else:
         # If we're on shard 0, grab the snap DB here.
-        print("* Now cloning Shard 0, kick back and relax for awhile...")
-        print_stars()
-        process_command(
+        print(f"* Now cloning Shard 0, kick back and relax for awhile...\n{string_stars()}")
+        run_command(
             f"rclone -P -L --checksum sync release:pub.harmony.one/{environ.get('NETWORK')}.snap/harmony_db_0 {environ.get('HARMONY_DIR')}/harmony_db_0 --multi-thread-streams 4 --transfers=32"
         )
 
 
 # is this used?
 def set_mounted_point():
     # First let's make sure your volume is mounted
@@ -993,55 +1074,57 @@
         dotenv.set_key(EnvironmentVariables.dotenv_file, "HARMONY_DIR", myLongHmyPath)
     else:
         dotenv.set_key(EnvironmentVariables.dotenv_file, "HARMONY_DIR", f"{environ.get('HARMONY_DIR')}")
 
 
 def finish_node_install():
     load_var_file(EnvironmentVariables.dotenv_file)
-    print_stars()
     print(
-        "* Installation is completed"
+        f"{string_stars()}\n* Installation is completed"
         + "\n* Create a new wallet or recover your existing wallet into ./hmy"
         + "\n* Create or upload your bls key & pass files into ~/harmony/.hmy/blskeys"
-        + "\n* Finally, reboot to start synchronization."
+        + f"\n* Finally, reboot to start synchronization.\n{string_stars()}"
     )
-    print_stars()
     if environ.get("NODE_WALLET") == "false":
         print(
             "* Post installation quick tips:"
             + "\n* To recover your wallet on this server run:"
-            + f"\n* python3 ~/harmony-toolboxload_wallet.py"
+            + "\n* python3 ~/harmony-toolbox/load_wallet.py"
             + "\n*"
             + "\n* To create BLS keys run:"
-            + f'\n* ./hmy keys generate-bls-keys --count 1 --shard {environ.get("SHARD")} --passphrase'
-            + "\n*"
+            + f'\n* {environ.get("HARMONY_DIR")}/hmy keys generate-bls-keys --count 1 --shard {environ.get("SHARD")} --passphrase'
+            + f"\n*\n{string_stars()}"
         )
     else:
         print(
             "* Post installation quick tips:"
             + "\n* To recover your wallet again, run:"
-            + f"\n* python3 ~/harmony-toolboxload_wallet.py"
+            + "\n* python3 ~/harmony-toolbox/load_wallet.py"
             + "\n*"
             + "\n* To create BLS keys run:"
-            + f'\n* ./hmy keys generate-bls-keys --count 1 --shard {environ.get("SHARD")} {environ.get("PASS_SWITCH")}'
-            + "\n*"
+            + f'\n* {environ.get("HARMONY_DIR")}/hmy keys generate-bls-keys --count 1 --shard {environ.get("SHARD")} {environ.get("PASS_SWITCH")}'
+            + f"\n*\n{string_stars()}"
         )
-    print_stars()
-    print("* Thanks for using Easy Node - Validator Node Server Software Installer!")
-    print_stars()
+    print(f"* Thanks for using Easy Node - Validator Node Server Software Installer!\n{string_stars()}")
     raise SystemExit(0)
 
 
 def free_space_check(mount) -> str:
     ourDiskMount = get_HARMONY_DIR(mount)
     _, _, free = shutil.disk_usage(ourDiskMount)
     freeConverted = str(converted_unit(free))
     return freeConverted
 
 
+def free_space_size(mount) -> str:
+    ourDiskMount = get_HARMONY_DIR(mount)
+    _, _, free = shutil.disk_usage(ourDiskMount)
+    return free
+
+
 def server_drive_check(dot_env, directory) -> None:
     if environ.get("HARMONY_DIR") is not None:
         ourDiskMount = environ.get("HARMONY_DIR")
     else:
         dotenv.set_key(dot_env, "HARMONY_DIR", directory)
         load_var_file(dot_env)
         ourDiskMount = environ.get("HARMONY_DIR")
@@ -1060,16 +1143,15 @@
         + free_space_check(directory)
         + " Free\n"
         + used
         + " Used\n"
         + total
         + " Total"
     )
-    print_stars()
-    input("Disk check complete, press ENTER to return to the main menu. ")
+    input(f"{string_stars()}\nDisk check complete, press ENTER to return to the main menu. ")
 
 
 def disk_partitions(all=False):
     disk_ntuple = namedtuple("partition", "device mountpoint fstype")
     # Return all mounted partitions as a nameduple.
     # If all == False return physical partitions only.
     phydevs = []
@@ -1105,18 +1187,17 @@
         if pathname == HARMONY_DIR:
             break
         parent_device = os.stat(pathname).st_dev
     return HARMONY_DIR
 
 
 def refreshing_stats_message() -> str:
-    print(Fore.GREEN)
-    print_stars()
-    print(f"* Getting the latest local & blockchain information now, one moment while we load...")
-    print_stars()
+    print(
+        f"{Fore.GREEN}{string_stars()}\n* Getting the latest local & blockchain information now, one moment while we load...\n{string_stars()}"
+    )
     return
 
 
 def converted_unit(n):
     symbols = ("K", "M", "G", "T", "P", "E", "Z", "Y")
     prefix = {}
     for i, s in enumerate(symbols):
@@ -1230,16 +1311,15 @@
     print(f"Total Bytes Sent: {get_size(net_io.bytes_sent)}")
     print(f"Total Bytes Received: {get_size(net_io.bytes_recv)}")
     input("Press ENTER to return to the main menu.")
     return
 
 
 def coming_soon():
-    print("* This option isn't available on your system, yet!")
-    print_stars()
+    print(f"* This option isn't available on your system, yet!\n{string_stars()}")
     input("* Press enter to return to the main menu.")
 
 
 def run_ubuntu_updater() -> None:
     os_upgrades()
     print()
 
@@ -1247,27 +1327,40 @@
 def os_upgrades() -> None:
     upgrades = (
         "sudo apt update",
         "sudo apt upgrade -y",
         "sudo apt dist-upgrade -y",
         "sudo apt autoremove -y",
     )
-    print_stars()
     for x in upgrades:
+        print_stars()
         process_command(x)
-    print_stars()
+        print_stars()
+
+
+def set_network(network):
+    set_var(EnvironmentVariables.dotenv_file, "NETWORK", "mainnet")
+    set_var(EnvironmentVariables.dotenv_file, "NETWORK_SWITCH", network)
+    set_var(EnvironmentVariables.dotenv_file, "RPC_NET", f"https://rpc.s0.{network}.hmny.io")
+    if environ.get("SHARD") != "0":
+        set_var(EnvironmentVariables.dotenv_file, "RPC_NET_SHARD", f"https://rpc.s{environ.get('SHARD')}.t.hmny.io")
+    return
 
 
 def menu_ubuntu_updates() -> str:
-    question = ask_yes_no(f"* Are you sure you would like to proceed with Linux apt Upgrades? (Y/N) ")
+    question = ask_yes_no("* Are you sure you would like to proceed with Linux apt Upgrades? (Y/N) ")
     if question:
         run_ubuntu_updater()
         input("* OS Updates completed, press ENTER to return to the main menu. ")
 
 
+def clear_screen():
+    os.system("cls" if os.name == "nt" else "clear")
+
+
 def menu_reboot_server() -> str:
     question = ask_yes_no(
         Fore.RED
         + "WARNING: YOU WILL MISS BLOCKS WHILE YOU REBOOT YOUR ENTIRE SERVER.\n\n"
         + "Reconnect after a few moments & Run the Validator Toolbox Menu again with: python3 ~/harmony-toolbox/start.py\n"
         + Fore.WHITE
         + "Are you sure you would like to proceed with rebooting your server?\n\nType 'Yes' or 'No' to continue"
@@ -1280,17 +1373,16 @@
 
 def finish_node():
     print(
         "* Thanks for using Easy Node Toolbox - Making everything Easy Mode!"
         + "\n*\n* We serve up free tools and guides for validators every day."
         + "\n*\n* Check our guides out at https://docs.easynode.pro\n*\n"
         + "* Please consider joining our discord & supporting us one time or monthly\n* for our"
-        + " tools and guides at https://bit.ly/easynodediscord today!\n*\n* Goodbye!"
+        + f" tools and guides at https://bit.ly/easynodediscord today!\n*\n* Goodbye!\n{string_stars()}"
     )
-    print_stars()
     raise SystemExit(0)
 
 
 def compare_two_files(input1, input2) -> None:
     # open the files
     file1 = open(input1, "rb")
     file2 = open(input2, "rb")
```

### Comparing `harmony_toolbox-1.2.0/src/toolbox/toolbox.py` & `harmony_toolbox-1.2.2/src/toolbox/toolbox.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,42 @@
-import os, requests, time, json, subprocess
+import os, requests, time, json, subprocess, pytz
 from pytimedinput import timedInteger
-from subprocess import Popen, PIPE, run
+from subprocess import PIPE, run
 from ast import literal_eval
 from toolbox.config import EnvironmentVariables
 from os import environ
 from datetime import datetime
 from colorama import Fore, Back, Style
-from pyhmy import blockchain, transaction
+from pyhmy import blockchain, numbers
 from requests.exceptions import HTTPError
 from toolbox.library import (
     process_command,
     print_stars,
     print_stars,
-    print_whitespace,
     ask_yes_no,
     return_txt,
     find_port,
-    install_hmy,
+    update_hmy_binary,
     get_sign_pct,
     load_var_file,
     get_wallet_balance,
     get_rewards_balance,
     string_stars,
     set_var,
     free_space_check,
     server_drive_check,
     all_sys_info,
-    coming_soon,
     get_vote_choice,
     get_validator_wallet_name,
     governance_member_voting,
     proposal_choices_option,
     menu_ubuntu_updates,
     menu_reboot_server,
     finish_node,
-    pull_harmony_update,
+    update_harmony_binary,
     version_checks,
     harmony_service_status,
     get_folders,
     validator_stats_output,
     get_db_size,
     first_setup,
     update_text_file,
@@ -110,160 +108,153 @@
     if args.collect_send:
         rewards_collector(config.working_rpc_endpoint, True)
         finish_node()
 
 
 def run_multistats():
     refreshing_stats_message()
-    folders = get_folders()
-    validator_stats_output(folders)
+    validator_stats_output()
     return
 
 
-def collect_rewards(pending_rewards_balance, networkCall=EnvironmentVariables.hmy_app):
-    print(f"*\n* Collecting {pending_rewards_balance} $ONE Rewards, awaiting confirmation...\n")
+def collect_rewards(pending_rewards_balance, validator_wallet, networkCall=EnvironmentVariables.hmy_app):
+    print(f"*\n* Collecting {pending_rewards_balance} $ONE Rewards, awaiting confirmation...")
     command = f"{networkCall} staking collect-rewards --delegator-addr {environ.get('VALIDATOR_WALLET')} --gas-price 100 {environ.get('PASS_SWITCH')}"
     result = process_command(command, True, False)
     if result:
-        print("*\n*\n* Rewards collection Finished.\n")
+        print("*\n*\n* Rewards collection Finished.")
+        print_stars()
+        print(
+            Fore.GREEN + f"* mainnet rewards for {validator_wallet} have been collected." + Style.RESET_ALL + Fore.GREEN
+        )
+        print_stars()
     else:
         print("*\n*\n* Rewards collection Failed.\n")
 
 
 def send_rewards(networkCall, sendAmount, rewards_wallet):
     command = f"{networkCall} transfer --amount {sendAmount} --from {environ.get('VALIDATOR_WALLET')} --from-shard 0 --to {rewards_wallet} --to-shard 0 --gas-price 100 {environ.get('PASS_SWITCH')}"
     result = process_command(command, True, False)
     if result:
-        print("*\n*\n* Rewards sending Finished.\n")
+        print("*\n* Rewards sending Finished.")
     else:
-        print("*\n*\n* Rewards sending Failed.\n")
+        print("*\n* Rewards sending Failed.")
 
 
 def send_rewards_func(suggested_send, validator_wallet_balance, rewards_wallet, validator_wallet, bypass=False):
-    if bypass == False:
-        print("*\n*\n")
-        print_stars()
-        print("\n* Send your Harmony ONE Rewards?")
-        print_stars()
-        question = ask_yes_no(
-            f"* You have {validator_wallet_balance} $ONE available to send. We suggest sending {suggested_send} $ONE using your reservation settings.\n* Would you like to send {suggested_send} $ONE to {rewards_wallet} now? (YES/NO)"
-        )
-        if question == False:
-            print("*\n*\n* Skipping sending of rewards.\n")
-            return
-    print(f"*\n*\n* Sending {suggested_send} $ONE Rewards to {rewards_wallet}, awaiting confirmation...\n")
+    print(f"*\n*\n* Sending {suggested_send} $ONE Rewards to {rewards_wallet}, awaiting confirmation...")
     send_rewards(EnvironmentVariables.hmy_app, suggested_send, rewards_wallet)
     validator_wallet_balance = get_wallet_balance(validator_wallet)
     rewards_wallet_balance = get_wallet_balance(rewards_wallet)
-    print(f"*\n*\n* Current Validator Wallet Balance: {validator_wallet_balance} $ONE\n*")
-    print(f"*\n*\n* Current Rewards Wallet Balance: {rewards_wallet_balance} $ONE\n*\n*")
+    print(f"*\n* Current Validator Wallet Balance: {validator_wallet_balance} $ONE")
+    print(f"* Current Rewards Wallet Balance: {rewards_wallet_balance} $ONE\n*")
     return
 
 
 def rewards_sender(
     rewards_wallet=environ.get("REWARDS_WALLET"),
     validator_wallet=environ.get("VALIDATOR_WALLET"),
 ) -> None:
     validator_wallet_balance = get_wallet_balance(validator_wallet)
     suggested_send = validator_wallet_balance - int(environ.get("GAS_RESERVE"))
     if suggested_send >= 1:
-        send_rewards_func(suggested_send, validator_wallet_balance, rewards_wallet, validator_wallet)
+        question = ask_yes_no(
+            f"* You have {validator_wallet_balance} $ONE available to send. We suggest sending {suggested_send} $ONE using your reservation settings.\n* Would you like to send {suggested_send} $ONE to {rewards_wallet} now? (YES/NO)"
+        )
+        if question:
+            send_rewards_func(suggested_send, validator_wallet_balance, rewards_wallet, validator_wallet)
+        else:
+            print("*\n* Skipping sending of rewards.")
     else:
-        print("*\n* Wallet balance is less than your gas reservation, please try again later.\n*\n")
+        print("*\n* Wallet balance is less than your gas reservation, please try again later.")
     validator_wallet_balance = get_wallet_balance(validator_wallet)
     rewards_wallet_balance = get_wallet_balance(rewards_wallet)
     print(
-        f"*\n*\n* Current Validator Wallet Balance: {validator_wallet_balance} $ONE\n*\n* Current Rewards Wallet Balance: {rewards_wallet_balance}\n*\n*"
+        f"*\n* Current Validator Wallet Balance: {validator_wallet_balance} $ONE\n* Current Rewards Wallet Balance: {rewards_wallet_balance}\n*"
     )
     return
 
 
 def rewards_collector(
     rpc,
     bypass=False,
     rewards_wallet=environ.get("REWARDS_WALLET"),
     validator_wallet=environ.get("VALIDATOR_WALLET"),
 ) -> None:
     pending_rewards_balance = get_rewards_balance(rpc, validator_wallet)
-    print_stars()
-    print("* Harmony ONE Rewards Collection")
-    print_stars()
-    if bypass == False:
-        question = ask_yes_no(
-            f"*\n* For your validator wallet {validator_wallet}\n* You have {pending_rewards_balance} $ONE pending.\n* Would you like to collect your rewards on the Harmony mainnet? (YES/NO) "
-        )
-        if question:
-            bypass = True
-        else:
-            print("*\n*\n* Skipping collection of rewards.\n")
-    if bypass == True:
-        collect_rewards(pending_rewards_balance)
-        print_stars()
-        print(
-            Fore.GREEN + f"* mainnet rewards for {validator_wallet} have been collected." + Style.RESET_ALL + Fore.GREEN
-        )
-        print_stars()
+    
+    print(f"{string_stars()}\n* Harmony ONE Rewards Collection\n{string_stars()}")
+    
+    if bypass or ask_yes_no(
+        f"*\n* For your validator wallet {validator_wallet}\n* You have {pending_rewards_balance} $ONE pending.\n* Would you like to collect your rewards on the Harmony {environ.get('NETWORK')}? (YES/NO) "
+    ):
+        collect_rewards(pending_rewards_balance, validator_wallet)
+    else:
+        print("*\n* Skipping collection of rewards.")
+
     validator_wallet_balance = get_wallet_balance(validator_wallet)
     suggested_send = validator_wallet_balance - int(environ.get("GAS_RESERVE"))
+    
     if suggested_send >= 1:
-        send_rewards_func(suggested_send, validator_wallet_balance, rewards_wallet, validator_wallet, bypass)
+        if bypass or ask_yes_no(
+            f"* You have {validator_wallet_balance} $ONE available to send. We suggest sending {suggested_send} $ONE using your reservation settings.\n* Would you like to send {suggested_send} $ONE to {rewards_wallet} now? (YES/NO)"
+        ):
+            send_rewards_func(suggested_send, validator_wallet_balance, rewards_wallet, validator_wallet, bypass)
+        else:
+            print("*\n* Skipping sending of rewards.")
     else:
-        validator_wallet_balance = get_wallet_balance(validator_wallet)
         rewards_wallet_balance = get_wallet_balance(rewards_wallet)
-        print(f"*\n*\n* Balance too low to send to rewards wallet\n")
-        print(f"*\n*\n* Current Validator Wallet Balance: {validator_wallet_balance} $ONE\n*")
-        print(f"* Current Rewards Wallet Balance: {rewards_wallet_balance} $ONE\n*\n*")
+        print("*\n* Balance too low to send to rewards wallet")
+        print(f"*\n* Current Validator Wallet Balance: {validator_wallet_balance} $ONE*")
+        print(f"* Current Rewards Wallet Balance: {rewards_wallet_balance} $ONE\n*")
+    
     return
 
 
 def menu_topper_regular(software_versions) -> None:
     config = EnvironmentVariables()
     # Get stats & balances
     try:
         load_1, load_5, load_15 = os.getloadavg()
         sign_percentage = get_sign_pct()
-        total_balance = get_wallet_balance(environ.get("VALIDATOR_WALLET"))
+        validator_wallet_balance = get_wallet_balance(environ.get("VALIDATOR_WALLET"))
         remote_data_shard_0, local_data_shard, remote_data_shard = menu_validator_stats()
     except (ValueError, KeyError, TypeError) as e:
         print(f"* Error fetching data: {e}")
     # Print Menu
-    print_stars()
     print(
-        f'{Fore.GREEN}* Validator Toolbox for {Fore.CYAN}Harmony ONE{Fore.GREEN} Validators by Easy Node   v{environ.get("EASY_VERSION")}{Fore.WHITE}   https://easynode.pro {Fore.GREEN}*'
+        f'{Fore.GREEN}{string_stars()}\n* Validator Toolbox for {Fore.CYAN}Harmony ONE{Fore.GREEN} Validators by Easy Node   v{environ.get("EASY_VERSION")}{Fore.WHITE}   https://easynode.pro {Fore.GREEN}\n{string_stars()}'
     )
-    print_stars()
     print(
-        f'* Your validator wallet address is: {Fore.RED}{str(environ.get("VALIDATOR_WALLET"))}{Fore.GREEN}\n* Your $ONE balance is:             {Fore.CYAN}{str(round(total_balance, 2))}{Fore.GREEN}\n* Your pending $ONE rewards are:    {Fore.CYAN}{str(round(get_rewards_balance(config.working_rpc_endpoint, environ.get("VALIDATOR_WALLET")), 2))}{Fore.GREEN}\n* Server Hostname & IP:             {Fore.BLUE}{EnvironmentVariables.server_host_name}{Fore.GREEN} - {Fore.YELLOW}{EnvironmentVariables.external_ip}{Fore.GREEN}'
+        f'* Your validator wallet address is: {Fore.RED}{str(environ.get("VALIDATOR_WALLET"))}{Fore.GREEN}\n* Your $ONE balance is:             {Fore.CYAN}{str(round(validator_wallet_balance, 2))}{Fore.GREEN}\n* Your pending $ONE rewards are:    {Fore.CYAN}{str(round(get_rewards_balance(config.working_rpc_endpoint, environ.get("VALIDATOR_WALLET")), 2))}{Fore.GREEN}\n* Server Hostname & IP:             {Fore.BLUE}{EnvironmentVariables.server_host_name}{Fore.GREEN} - {Fore.YELLOW}{EnvironmentVariables.external_ip}{Fore.GREEN}'
     )
     harmony_service_status(environ.get("SERVICE_NAME", "harmony"))
     print(
-        f'* Epoch Signing Percentage:         {Style.BRIGHT}{Fore.GREEN}{Back.BLUE}{sign_percentage} %{Style.RESET_ALL}{Fore.GREEN}\n* Current disk space free: {Fore.CYAN}{free_space_check(os.environ.get("HARMONY_DIR")): >6}{Fore.GREEN}\n* Current harmony version: {Fore.YELLOW}{software_versions["harmony_version"]}{Fore.GREEN}, has upgrade available: {software_versions["harmony_upgrade"]}\n* Current hmy version: {Fore.YELLOW}{software_versions["hmy_version"]}{Fore.GREEN}, has upgrade available: {software_versions["hmy_upgrade"]}'
+        f'* Epoch Signing Percentage:         {Style.BRIGHT}{Fore.GREEN}{Back.BLUE}{sign_percentage} %{Style.RESET_ALL}{Fore.GREEN}\n* Current disk space free: {Fore.CYAN}{free_space_check(os.environ.get("HARMONY_DIR")): >6}{Fore.GREEN}\n* Current harmony version: {Fore.YELLOW}{software_versions["harmony_version"]}{Fore.GREEN}, has upgrade available: {software_versions["harmony_upgrade"]}\n* Current hmy version: {Fore.YELLOW}{software_versions["hmy_version"]}{Fore.GREEN}, has upgrade available: {software_versions["hmy_upgrade"]}\n{string_stars()}'
     )
-    print_stars()
     if environ.get("SHARD") != "0":
         print(
-            f"* Note: Running on shard {environ.get('SHARD')}, Shard 0 is no longer needed locally and should be under 300MB\n* Remote Shard 0 Epoch: {remote_data_shard_0['result']['shard-chain-header']['epoch']}, Current Block: {literal_eval(remote_data_shard_0['result']['shard-chain-header']['number'])}, Local Shard 0 Size: {get_db_size(os.environ.get('HARMONY_DIR'), '0')}"
+            f"* Shard {environ.get('SHARD')} Stats:\n{string_stars()}\n* Remote Shard 0 Epoch: {remote_data_shard_0['result']['shard-chain-header']['epoch']}, Current Block: {literal_eval(remote_data_shard_0['result']['shard-chain-header']['number'])}, Local Shard 0 Size: {get_db_size(os.environ.get('HARMONY_DIR'), '0')}"
         )
         print(
             f"* Remote Shard {environ.get('SHARD')} Epoch: {remote_data_shard['result']['shard-chain-header']['epoch']}, Current Block: {literal_eval(remote_data_shard['result']['shard-chain-header']['number'])}"
         )
         print(
             f"*  Local Shard {environ.get('SHARD')} Epoch: {local_data_shard['result']['shard-chain-header']['epoch']}, Current Block: {literal_eval(local_data_shard['result']['shard-chain-header']['number'])}, Local Shard {environ.get('SHARD')} Size: {get_db_size(os.environ.get('HARMONY_DIR'), environ.get('SHARD'))}"
         )
     if environ.get("SHARD") == "0":
         print(
-            f"* Remote Shard {environ.get('SHARD')} Epoch: {remote_data_shard_0['result']['shard-chain-header']['epoch']}, Current Block: {literal_eval(remote_data_shard_0['result']['shard-chain-header']['number'])}"
+            f"* Shard {environ.get('SHARD')} Stats:\n{string_stars()}\n* Remote Shard {environ.get('SHARD')} Epoch: {remote_data_shard_0['result']['shard-chain-header']['epoch']}, Current Block: {literal_eval(remote_data_shard_0['result']['shard-chain-header']['number'])}"
         )
         print(
             f"*  Local Shard {environ.get('SHARD')} Epoch: {local_data_shard['result']['shard-chain-header']['epoch']}, Current Block: {literal_eval(local_data_shard['result']['shard-chain-header']['number'])}"
         )
     print(
-        f"* CPU Load Averages: {round(load_1, 2)} over 1 min, {round(load_5, 2)} over 5 min, {round(load_15, 2)} over 15 min"
+        f"* CPU Load Averages: {round(load_1, 2)} over 1 min, {round(load_5, 2)} over 5 min, {round(load_15, 2)} over 15 min\n{string_stars()}"
     )
-    print_stars()
 
 
 def menu_regular(software_versions) -> None:
     menu_topper_regular(software_versions)
     for x in return_txt(EnvironmentVariables.main_menu_regular):
         x = x.strip()
         try:
@@ -271,17 +262,16 @@
         except SyntaxError:
             pass
         if x:
             print(x)
 
 
 def get_wallet_json(wallet: str) -> str:
-    test_or_main = environ.get("NETWORK")
     try:
-        response = requests.get(f"https://api.stake.hmny.io/networks/{test_or_main}/validators/{wallet}")
+        response = requests.get(f"https://api.stake.hmny.io/networks/{environ.get('NETWORK')}/validators/{wallet}")
         response.raise_for_status()
         # access JSOn content
         json_response = response.json()
     #        print("Entire JSON response")
     #        print(json_response)
     except HTTPError as http_err:
         print(f"HTTP error occurred: {http_err}")
@@ -298,25 +288,24 @@
 
 
 def tmi_server_info() -> None:
     validator_wallet = environ.get("VALIDATOR_WALLET")
     json_response = get_wallet_json(validator_wallet)
     for key, value in json_response.items():
         print(key, ":", value)
-    print_stars()
-    input("Press ENTER to return to the main menu.")
+    input(f"{string_stars()}\nPress ENTER to return to the main menu.")
 
 
 def set_rewards_wallet() -> None:
     rewards_wallet = environ.get("REWARDS_WALLET")
     gas_reserve = environ.get("GAS_RESERVE")
     if rewards_wallet is None:
         question = ask_yes_no("* Would you like to add an address to send your rewards too? (YES/NO)")
         if question:
-            rewards_wallet = input(f"* Input your one1 address to send rewards into, please input your address now: ")
+            rewards_wallet = input("* Input your one1 address to send rewards into, please input your address now: ")
             if rewards_wallet.startswith("one1"):
                 set_var(EnvironmentVariables.dotenv_file, "REWARDS_WALLET", rewards_wallet)
             else:
                 print("* Wallet does not start with one1, please try again.")
                 return
         return
     else:
@@ -371,17 +360,15 @@
     config = EnvironmentVariables()
     menu_check_balance(config.working_rpc_endpoint, environ.get("VALIDATOR_WALLET"))
 
 
 def bingo_checker():
     command = f"grep BINGO {os.environ.get('HARMONY_DIR')}/latest/zerolog-harmony.log | tail -10"
     process_command(command, shell=True, print_output=True)
-    print_stars()
-    print("* Press enter to return to the main menu.")
-    print_stars()
+    print(f"{string_stars()}\n* Press enter to return to the main menu.\n{string_stars()}")
     input()
 
 
 def run_rewards_collector() -> None:
     config = EnvironmentVariables()
     rewards_collector(config.working_rpc_endpoint)
     return
@@ -395,32 +382,36 @@
     if environ.get("REFRESH_TIME") is None:
         set_var(EnvironmentVariables.dotenv_file, "REFRESH_TIME", "30")
     if environ.get("REFRESH_OPTION") is None:
         set_var(EnvironmentVariables.dotenv_file, "REFRESH_OPTION", "True")
     if environ.get("HARMONY_DIR") is None:
         if os.path.isdir(f"{EnvironmentVariables.user_home_dir}/harmony"):
             set_var(EnvironmentVariables.dotenv_file, "HARMONY_DIR", f"{EnvironmentVariables.user_home_dir}/harmony")
+            set_var(EnvironmentVariables.dotenv_file, "SERVICE_NAME", "harmony")
             return
         elif os.path.isfile(f"{EnvironmentVariables.user_home_dir}/harmony"):
             try:
                 subprocess.run(f"{EnvironmentVariables.user_home_dir}/harmony -V", check=True)
                 set_var(EnvironmentVariables.dotenv_file, "HARMONY_DIR", f"{EnvironmentVariables.user_home_dir}")
+                set_var(EnvironmentVariables.dotenv_file, "SERVICE_NAME", "harmony")
                 return
             except subprocess.CalledProcessError as e:
                 print(
-                    "* Well this is odd, somehow harmony was not found.\n*\n* You can add the HARMONY_DIR variable to your ~/.easynode.env file\n* Example default location: HARMONY_DIR = /home/serviceharmony/harmony\n*\n* Or contact Easy Node for custom configuration help."
+                    f"* Well this is odd, somehow harmony was not found.\n*\n* You can add the HARMONY_DIR variable to your ~/.easynode.env file\n* Example default location: HARMONY_DIR = /home/serviceharmony/harmony\n*\n* Or contact Easy Node for custom configuration help.\* Error: {e}"
                 )
                 raise SystemExit(0)
         else:
             first_setup()
+    if environ.get("SERVICE_NAME") is None:
+        set_var(EnvironmentVariables.dotenv_file, "SERVICE_NAME", "harmony")
     # always set conf to 13 keys, shard max
     if os.path.exists(EnvironmentVariables.harmony_conf):
         update_text_file(EnvironmentVariables.harmony_conf, "MaxKeys = 10", "MaxKeys = 13")
     if os.path.isfile(f"{os.environ.get('HARMONY_DIR')}/blskey.pass"):
-        update_text_file(EnvironmentVariables.harmony_conf, 'PassFile = ""', f'PassFile = "blskey.pass"')
+        update_text_file(EnvironmentVariables.harmony_conf, 'PassFile = ""', 'PassFile = "blskey.pass"')
     passphrase_status()
     get_shard_menu()
     set_main_or_test()
     if environ.get("VALIDATOR_WALLET") is None:
         # Recover wallet or have them add address
         recover_wallet()
 
@@ -467,17 +458,15 @@
             f"*  20 - Disable auto-update       - Disable Refresh or Change Delay Timer: {str(environ.get('REFRESH_TIME'))} seconds"
         )
     else:
         print(f"*  20 - Enable Auto update        - Enable Update Timer")
 
 
 def harmony_voting() -> None:
-    print_stars()
-    print("* Harmony Voting")
-    print_stars()
+    print(f"{string_stars()}\n* Harmony Voting\n{string_stars()}")
     question, proposal = proposal_choices_option()
     if proposal == "Quit" or question == False:
         return
     validator_wallet_name = get_validator_wallet_name(environ.get("VALIDATOR_WALLET"))
     if proposal == "HIP-30v2":
         vote_choice_option, vote_choice_text = get_vote_choice()
         if vote_choice_text == "Quit":
@@ -544,22 +533,20 @@
         999: menu_reboot_server,
     }
     while True:
         load_var_file(EnvironmentVariables.dotenv_file)
         menu_regular(software_versions)
         if software_versions["harmony_upgrade"] == "True":
             print(
-                f'* The harmony binary has an update available to version {software_versions["online_harmony_version"]}\n* Option #10 will upgrade you, but you may miss a block while it upgrades & restarts.\n* Currently installed version {software_versions["harmony_version"]}'
+                f'* The harmony binary has an update available to version {software_versions["online_harmony_version"]}\n* Option #10 will upgrade you, but you may miss a block while it upgrades & restarts.\n* Currently installed version {software_versions["harmony_version"]}\n{string_stars()}'
             )
-            print_stars()
         if software_versions["hmy_upgrade"] == "True":
             print(
-                f'* The hmy binary has an update available to version {software_versions["online_hmy_version"]}\n* Option #11 will upgrade you.\n* Currently installed version {software_versions["hmy_version"]}'
+                f'* The hmy binary has an update available to version {software_versions["online_hmy_version"]}\n* Option #11 will upgrade you.\n* Currently installed version {software_versions["hmy_version"]}\n{string_stars()}'
             )
-            print_stars()
         if environ.get("REFRESH_OPTION") == "True":
             try:
                 # run timed input
                 option, timedOut = timedInteger(
                     f"* Auto refresh enabled, Enter your menu choice: ",
                     timeout=int(environ.get("REFRESH_TIME")),
                     resetOnInput=True,
@@ -569,15 +556,15 @@
                     start_regular_node()
                 else:
                     print_stars()
                     menu_options[option]()
                     if option != 1:
                         start_regular_node()
             except KeyError:
-                print(f"* Bad option, try again. Press enter to continue.")
+                print("* Bad option, try again. Press enter to continue.")
                 print_stars()
                 input()
                 start_regular_node()
         else:
             try:
                 option, timedOut = timedInteger(
                     "* Auto refresh disabled, Enter your menu choice: ",
@@ -593,33 +580,40 @@
                 print(f"* Bad option, try again. Press enter to continue.")
                 print_stars()
                 input()
                 start_regular_node()
 
 
 def service_menu_option() -> None:
-    status = process_command("systemctl is-active --quiet harmony", True, False)
-    if status == 0:
+    status = process_command(f"systemctl is-active --quiet {environ.get('SERVICE_NAME')}", True, False)
+    if status:
         print(
             f"*   8 - {Fore.RED}Stop Harmony Service      {Fore.GREEN}- {Fore.YELLOW}{Back.RED}WARNING: You will miss blocks while stopped!   {Style.RESET_ALL}{Fore.GREEN}"
         )
         print(
             f"*   9 - Restart Harmony Service   - {Back.RED}{Fore.YELLOW}WARNING: You will miss blocks during a restart!{Style.RESET_ALL}{Fore.GREEN}"
         )
     else:
-        print(f"*   8 - Start Harmony Service")
+        print("*   8 - Start Harmony Service")
     return
 
 
+def update_menu_option(software_versions) -> None:
+    if software_versions["harmony_upgrade"] == "True":
+        print(f"*  10 - Update Harmony App Binary - For New Harmony Releases ONLY, {Fore.YELLOW}{Back.RED}WARNING: You will miss blocks during upgrade.{Style.RESET_ALL}{Fore.GREEN}")
+    if software_versions["hmy_upgrade"] == "True":
+        print("*  11 - Update hmy CLI App        - Update harmony binary file, run anytime!")
+
 def hip_voting_option() -> None:
-    # Specify the deadline in server's local time
-    deadline = datetime(2023, 8, 9, 20, 59)
+    # Specify the deadline in UTC
+    utc = pytz.utc
+    deadline = utc.localize(datetime(2023, 8, 9, 20, 59))
 
-    # Get the current time in server's local time
-    current_time = datetime.now()
+    # Get the current time in UTC
+    current_time = datetime.now(utc)
 
     # Check if the current time is before or after the deadline
     active_vote = current_time < deadline
 
     if active_vote:
         print("*   7 - Harmony Governance Voting - Cast your vote for HIP-30v2")
     else:
@@ -641,42 +635,55 @@
     return folder_name
 
 
 def hmy_cli_upgrade():
     question = ask_yes_no(
         "* Are you sure you would like to proceed with updating the Harmony CLI file?\n\nType 'Yes' or 'No' to continue"
     )
-    if question:
+    
+    if not question:
+        print("* Update canceled.")
+        return
+    
+    try:
+        # Backup the current version of hmy CLI
         folder_name = make_backup_dir()
         process_command(f"cp {environ.get('HARMONY_DIR')}/hmy {folder_name}")
         print_stars()
-        install_hmy()
+        
+        # Install the new version
+        software_versions = update_hmy_binary()
         print_stars()
-        print("Harmony cli has been updated to: ")
-        process_command(f"{environ.get('HARMONY_DIR')}/hmy version")
+        
+        # Print the updated version
+        print(f"Harmony cli has been updated to: {software_versions['hmy_version']}")
         print_stars()
+
+        # Update the environment variable
         set_var(EnvironmentVariables.dotenv_file, "HMY_UPGRADE_AVAILABLE", "False")
-        input("* Update completed, press ENTER to return to the main menu. ")
+        
+    except Exception as e:  # Catch generic errors, though you might want to catch more specific exceptions
+        print(f"{string_stars()}\n* An error occurred during the update: {e}\n{string_stars()}")
+        # Handle the error or possibly re-raise it depending on your requirements
+        return
+
+    input("* Update completed, press ENTER to return to the main menu. ")
 
 
 def update_harmony_app():
     os.chdir(f"{os.environ.get('HARMONY_DIR')}")
-    print_stars()
-    print("Currently installed version: ")
+    print(f"{string_stars()}\nCurrently installed version: ")
     process_command("./harmony -V")
     folder_name = make_backup_dir()
     process_command(
         f"cp {os.environ.get('HARMONY_DIR')}/harmony {os.environ.get('HARMONY_DIR')}/harmony.conf {folder_name}"
     )
-    print_stars()
-    print("Downloading current harmony binary file from harmony.one: ")
-    print_stars()
-    pull_harmony_update(os.environ.get("HARMONY_DIR"), EnvironmentVariables.harmony_conf)
-    print_stars()
-    print("Updated version: ")
+    print(f"{string_stars()}\nDownloading current harmony binary file from harmony.one: \n{string_stars()}")
+    update_harmony_binary(os.environ.get("HARMONY_DIR"), EnvironmentVariables.harmony_conf)
+    print(f"{string_stars()}\nUpdated version: ")
     process_command("./harmony -V")
     if environ.get("SHARD") != "0":
         size = 0
         for path, dirs, files in os.walk(f"{os.environ.get('HARMONY_DIR')}/harmony_db_0"):
             for f in files:
                 fp = os.path.join(path, f)
                 size += os.path.getsize(fp)
@@ -693,16 +700,15 @@
                     process_command("sudo service harmony start")
                     process_command(f"rm -r {os.environ.get('HARMONY_DIR')}/harmony_db_0_old")
                 else:
                     print("Skipping removal of 0, but it's no longer required, fyi!")
             else:
                 print("Your database 0 is already trimmed, enjoy!")
     process_command("sudo service harmony restart")
-    print_stars()
-    print("Harmony Service is restarting, waiting 10 seconds for restart.")
+    print(f"{string_stars()}\nHarmony Service is restarting, waiting 10 seconds for restart.")
     set_var(EnvironmentVariables.dotenv_file, "HARMONY_UPGRADE_AVAILABLE", "False")
     time.sleep(10)
 
 
 def menu_validator_stats():
     load_var_file(EnvironmentVariables.dotenv_file)
     remote_shard_0 = [
@@ -725,17 +731,16 @@
             "--node",
             f"http://localhost:{http_port}",
         ]
         result_local_shard = run(local_shard, stdout=PIPE, stderr=PIPE, universal_newlines=True)
         local_data_shard = json.loads(result_local_shard.stdout)
     except (ValueError, KeyError, TypeError) as e:
         print(
-            f"* Local Server Offline\n*\n* Run troubleshooting, See our documents site for info on how to manually troubleshoot:\n* https://docs.easynode.pro/harmony/post#validator-toolbox-troubleshooting\n*"
+            f"* Local Server Offline\n*\n* Run troubleshooting, See our documents site for info on how to manually troubleshoot:\n* https://docs.easynode.pro/harmony/post#validator-toolbox-troubleshooting\n{string_stars()}"
         )
-        print_stars()
         finish_node()
 
     if environ.get("SHARD") != "0":
         remote_shard = [
             f"{environ.get('HARMONY_DIR')}/hmy",
             "blockchain",
             "latest-headers",
@@ -781,17 +786,19 @@
         + "* WARNING: YOU WILL MISS BLOCKS WHILE YOU UPGRADE THE HARMONY SERVICE.\n\n"
         + Fore.WHITE
         + "* Are you sure you would like to proceed?\n\nType 'Yes' or 'No' to continue"
     )
     if question:
         update_harmony_app()
 
+def menu_service_stop_start():
+    menu_service_stop_start_trigger(environ.get("HARMONY_SERVICE"))
 
-def menu_service_stop_start() -> str:
-    status = process_command("systemctl is-active --quiet harmony")
+def menu_service_stop_start_trigger(service) -> str:
+    status = process_command(f"systemctl is-active --quiet {service}")
     if status != 0:
         process_command("sudo service harmony start")
         print()
         print("* Harmony Service Has Been Started.")
         print()
         input("* Press ENTER to return to the main menu.")
     else:
@@ -833,38 +840,33 @@
 
 def menu_active_bls() -> str:
     validator_wallet = environ.get("VALIDATOR_WALLET")
     json_response = get_wallet_json(validator_wallet)
     print("* This is a list of your BLS Keys that are active for the next election.")
     for i, x in enumerate(json_response["bls-public-keys"]):
         print(f"BLS Key {i+1} {x}")
-    print_stars()
-    print("* Press ENTER to return to the main menu.")
-    print_stars()
+    print(f"{string_stars()}\n* Press ENTER to return to the main menu.\n{string_stars()}")
     input()
 
 
 # is this used?
 def is_float(value):
     try:
         float(value)
         return True
     except ValueError:
         return False
 
 
 def menu_check_balance(rpc, validator_wallet) -> None:
     if environ.get("NODE_TYPE") == "regular":
-        print("* Calling mainnet and testnet for balances...")
-        print_stars()
-        total_balance, total_balance_test = get_wallet_balance(validator_wallet)
-        print(f"* Your Validator Wallet Balance on Mainnet is: {total_balance} Harmony ONE Coins")
-        print(f"* Your Pending Validator Rewards are: {get_rewards_balance(rpc, validator_wallet)}")
-        print(f"* Your Validator Wallet Balance on Testnet is: {total_balance_test} Harmony ONE Test Coins")
-        print_stars()
+        print(f"* Calling mainnet for balances...{string_stars()}")
+        validator_wallet_balance = get_wallet_balance(validator_wallet)
+        print(f"* Your Validator Wallet Balance on Mainnet is: {validator_wallet_balance} Harmony ONE Coins")
+        print(f"* Your Pending Validator Rewards are: {get_rewards_balance(rpc, validator_wallet)}\n{string_stars()}")
         i = 0
         while i < 1:
             question = ask_yes_no("* Would you like to check another Harmony ONE Address? (YES/NO) ")
             if question:
                 balanceCheckAny()
             else:
                 i = 1
@@ -879,21 +881,19 @@
 
 
 def balanceCheckAny():
     check_wallet = input(
         "* Type the address of the Harmony ONE Wallet you would like to check.\n"
         + "* Only one wallets will work, no 0x addresses : "
     )
-    print("* Calling mainnet and testnet for balances...")
-    print_stars()
-    total_balance, total_balance_test = get_wallet_balance(check_wallet)
+    print(f"* Calling mainnet for balances...\n{string_stars()}")
+    wallet_balance = get_wallet_balance(check_wallet)
     print(
-        f"* The Mainnet Wallet Balance is: {total_balance} Harmony ONE Coins\n* The Testnet Wallet Balance is: {total_balance_test} Harmony ONE Test Coins"
+        f"* The Mainnet Wallet Balance is: {wallet_balance} Harmony ONE Coins\n{string_stars()}"
     )
-    print_stars()
     input("* Press ENTER to continue.")
 
 
 def get_current_epoch():
     config = EnvironmentVariables()
     current_epoch = 0
     try:
```

