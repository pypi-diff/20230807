# Comparing `tmp/ashcrypt-3.2.1.tar.gz` & `tmp/ashcrypt-3.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ashcrypt-3.2.1.tar", last modified: Mon Aug  7 10:54:57 2023, max compression
+gzip compressed data, was "dist/ashcrypt-3.2.2.tar", last modified: Mon Aug  7 20:15:33 2023, max compression
```

## Comparing `ashcrypt-3.2.1.tar` & `ashcrypt-3.2.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:54:57.000000 ashcrypt-3.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-07 10:54:57.000000 ashcrypt-3.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16950 2023-08-07 10:54:47.000000 ashcrypt-3.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:54:57.000000 ashcrypt-3.2.1/ashcrypt/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-08-07 10:54:47.000000 ashcrypt-3.2.1/ashcrypt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-08-07 10:54:47.000000 ashcrypt-3.2.1/ashcrypt/crypt.py
--rw-r--r--   0 runner    (1001) docker     (123)    10523 2023-08-07 10:54:47.000000 ashcrypt-3.2.1/ashcrypt/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-08-07 10:54:47.000000 ashcrypt-3.2.1/ashcrypt/filecrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)    39274 2023-08-07 10:54:47.000000 ashcrypt-3.2.1/ashcrypt/gui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:54:57.000000 ashcrypt-3.2.1/ashcrypt/sandbox/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 10:54:47.000000 ashcrypt-3.2.1/ashcrypt/sandbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6811 2023-08-07 10:54:47.000000 ashcrypt-3.2.1/ashcrypt/sandbox/clicrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-08-07 10:54:47.000000 ashcrypt-3.2.1/ashcrypt/textcrypt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:54:57.000000 ashcrypt-3.2.1/ashcrypt/unittests/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-07 10:54:47.000000 ashcrypt-3.2.1/ashcrypt/unittests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-08-07 10:54:47.000000 ashcrypt-3.2.1/ashcrypt/unittests/test_crypt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:54:57.000000 ashcrypt-3.2.1/ashcrypt/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 10:54:47.000000 ashcrypt-3.2.1/ashcrypt/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:54:57.000000 ashcrypt-3.2.1/ashcrypt/utils/consts/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-07 10:54:47.000000 ashcrypt-3.2.1/ashcrypt/utils/consts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-08-07 10:54:47.000000 ashcrypt-3.2.1/ashcrypt/utils/consts/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:54:57.000000 ashcrypt-3.2.1/ashcrypt/utils/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-07 10:54:47.000000 ashcrypt-3.2.1/ashcrypt/utils/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-08-07 10:54:47.000000 ashcrypt-3.2.1/ashcrypt/utils/exceptions/dynamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-08-07 10:54:47.000000 ashcrypt-3.2.1/ashcrypt/utils/exceptions/fixed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:54:57.000000 ashcrypt-3.2.1/ashcrypt/utils/safepack/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 10:54:47.000000 ashcrypt-3.2.1/ashcrypt/utils/safepack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-08-07 10:54:47.000000 ashcrypt-3.2.1/ashcrypt/utils/safepack/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-08-07 10:54:47.000000 ashcrypt-3.2.1/ashcrypt/utils/safepack/qr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-08-07 10:54:47.000000 ashcrypt-3.2.1/ashcrypt/utils/safepack/text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:54:57.000000 ashcrypt-3.2.1/ashcrypt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-07 10:54:57.000000 ashcrypt-3.2.1/ashcrypt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-08-07 10:54:57.000000 ashcrypt-3.2.1/ashcrypt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 10:54:57.000000 ashcrypt-3.2.1/ashcrypt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-07 10:54:57.000000 ashcrypt-3.2.1/ashcrypt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-07 10:54:57.000000 ashcrypt-3.2.1/ashcrypt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 10:54:57.000000 ashcrypt-3.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-08-07 10:54:47.000000 ashcrypt-3.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:15:33.000000 ashcrypt-3.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-08-07 20:15:33.000000 ashcrypt-3.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17141 2023-08-07 20:15:22.000000 ashcrypt-3.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:15:33.000000 ashcrypt-3.2.2/ashcrypt/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-08-07 20:15:22.000000 ashcrypt-3.2.2/ashcrypt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-08-07 20:15:22.000000 ashcrypt-3.2.2/ashcrypt/crypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10523 2023-08-07 20:15:22.000000 ashcrypt-3.2.2/ashcrypt/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-08-07 20:15:22.000000 ashcrypt-3.2.2/ashcrypt/filecrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39274 2023-08-07 20:15:22.000000 ashcrypt-3.2.2/ashcrypt/gui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:15:33.000000 ashcrypt-3.2.2/ashcrypt/sandbox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 20:15:22.000000 ashcrypt-3.2.2/ashcrypt/sandbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6811 2023-08-07 20:15:22.000000 ashcrypt-3.2.2/ashcrypt/sandbox/clicrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-08-07 20:15:22.000000 ashcrypt-3.2.2/ashcrypt/textcrypt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:15:33.000000 ashcrypt-3.2.2/ashcrypt/unittests/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-07 20:15:22.000000 ashcrypt-3.2.2/ashcrypt/unittests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-08-07 20:15:22.000000 ashcrypt-3.2.2/ashcrypt/unittests/test_crypt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:15:33.000000 ashcrypt-3.2.2/ashcrypt/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 20:15:22.000000 ashcrypt-3.2.2/ashcrypt/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:15:33.000000 ashcrypt-3.2.2/ashcrypt/utils/consts/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-07 20:15:22.000000 ashcrypt-3.2.2/ashcrypt/utils/consts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-08-07 20:15:22.000000 ashcrypt-3.2.2/ashcrypt/utils/consts/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:15:33.000000 ashcrypt-3.2.2/ashcrypt/utils/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-07 20:15:22.000000 ashcrypt-3.2.2/ashcrypt/utils/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-08-07 20:15:22.000000 ashcrypt-3.2.2/ashcrypt/utils/exceptions/dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-08-07 20:15:22.000000 ashcrypt-3.2.2/ashcrypt/utils/exceptions/fixed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:15:33.000000 ashcrypt-3.2.2/ashcrypt/utils/safepack/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 20:15:22.000000 ashcrypt-3.2.2/ashcrypt/utils/safepack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-08-07 20:15:22.000000 ashcrypt-3.2.2/ashcrypt/utils/safepack/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-08-07 20:15:22.000000 ashcrypt-3.2.2/ashcrypt/utils/safepack/qr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-08-07 20:15:22.000000 ashcrypt-3.2.2/ashcrypt/utils/safepack/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:15:33.000000 ashcrypt-3.2.2/ashcrypt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-08-07 20:15:33.000000 ashcrypt-3.2.2/ashcrypt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-08-07 20:15:33.000000 ashcrypt-3.2.2/ashcrypt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 20:15:33.000000 ashcrypt-3.2.2/ashcrypt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-07 20:15:33.000000 ashcrypt-3.2.2/ashcrypt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-07 20:15:33.000000 ashcrypt-3.2.2/ashcrypt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 20:15:33.000000 ashcrypt-3.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-08-07 20:15:22.000000 ashcrypt-3.2.2/setup.py
```

### Comparing `ashcrypt-3.2.1/PKG-INFO` & `ashcrypt-3.2.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: ashcrypt
-Version: 3.2.1
+Version: 3.2.2
 Summary: Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with a database module to store encrypted content.
 Home-page: https://github.com/AshGw/AES-256.git
 Author: Ashref Gwader
 Author-email: AshrefGw@proton.me
 License: UNKNOWN
 Description: # Cryptography App & Library For AES-256
         ## Docs ## 
-        **Visit The [GitHub](https://github.com/AshGw/AES-256/tree/main) Repository.**
+        **Visit The [GitHub](https://github.com/AshGw/ashcrypt/tree/main) Repository.**
         
         
 Keywords: Cryptography application,cryptography libraryAES-256
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ashcrypt-3.2.1/README.md` & `ashcrypt-3.2.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 # Cryptography App & Library w/ AES-256
-##  Objective ## 
-#### Enhanced Security, Simplicity & Ease of Use For Anyone Willing To Use AES 256.
+##  Why ? ##
+**Tired of juggling passwords and worrying about your private files?**
+<br>**That's exactly why I cooked up this Python library. I craved a hassle-free solution to shield my personal content from prying eyes, and it hit me—maybe others are hunting for the same thing!**
 ## Overview ## 
 ![alt text](important/GUI.png)
 The project incorporates an App & a library called **ashcrypt** : 
 
 **App :** 
 <br>Full-fledged application that integrates all the modules in the library merging them into a unified and powerful software solution for developers and for people with no programming knowledge whatsoever
-<br>check [GUI](https://github.com/AshGw/AES-256#gui) header for more info.
+<br>check [GUI](https://github.com/AshGw/ashcrypt#gui) header for more info.
 
 **Library :** 
 <br>A simple, secure, and developer-oriented library for performing encryption and decryption operations on data using the AES-256 (CBC) encryption algorithm.
 <br>The core of the library is the module `crypt`
 It offers cryptographic capabilities and security measures to safeguard
 sensitive data,  providing a hassle-free experience when dealing with cryptographic libraries.
-<br>View [Features](https://github.com/AshGw/AES-256#features) Header for more details.
+<br>View [Features](https://github.com/AshGw/ashcrypt#features) Header for more details.
 
 
 
 
 
 ### For Developers ###
 The project uses `crypt` module to ensure secure data encryption and decryption for files and text while keeping it very easy and simple to use .
-View the headers for [filecrypt](https://github.com/AshGw/AES-256#filecrypt) and [textcrypt](https://github.com/AshGw/AES-256#textcrypt) to learn more.
+View the headers for [filecrypt](https://github.com/AshGw/ashcrypt#filecrypt) and [textcrypt](https://github.com/AshGw/ashcrypt#textcrypt) to learn more.
 
 
 It also incorporates a database module which is there to allow key management & storage of classified content in a secure, 
 safe and simple manner.
 
-<br>The module has a simple straight forward approach for dealing with sqlite3 databases, even if you're not familiar with Python itself you can still use this module to run SQL queries with built in functions to perform various operations on a given database.<br>Check [database](https://github.com/AshGw/AES-256#database-1) header to learn more.
+<br>The module has a simple straight forward approach for dealing with sqlite3 databases, even if you're not familiar with Python itself you can still use this module to run SQL queries with built in functions to perform various operations on a given database.<br>Check [database](https://github.com/AshGw/ashcrypt#database-1) header to learn more.
 
 ## Installation ##
 ### If you want to use it as a library ###
 You can simply use **pip**
 <br>First upgrade the package installer 
 ```bash
 pip install --upgrade pip 
@@ -49,15 +50,15 @@
 ```
 That's it.
 
 ### Whole repo installation 
 Now if you want to get the whole repo with no manual configurations
 <br>Run this command in the Terminal
 ```bash
-curl -sSfL https://raw.githubusercontent.com/AshGw/AES-256/main/important/setup.sh | bash
+curl -sSfL https://raw.githubusercontent.com/AshGw/ashcrypt/main/important/setup.sh | bash
 ```
 This will run the commands in [setup.sh](important/setup.sh).
 <br>It will clone & install all the dependencies needed on your machine and activate the development mode, inside the directory you're currently at.
 
 **After the library is installed** 
 <br>To run the GUI 
 ```shell
@@ -66,15 +67,15 @@
 
 ## `crypt` Module ##
 The `crypt.py` Module is a comprehensive collection of carefully designed functions and code modules that facilitate the performance and reliability for data encryption and decryption operations  while ensuring security and 
 confidentiality.
 
 <br>It uses primitives from the `cryptography` library with added security features while keeping it simple and highly flexible to provide a head-ache free solution for developers. 
 
-<br>You can check [Features](https://github.com/AshGw/AES-256#features) tag below to learn more about the security features.
+<br>You can check [Features](https://github.com/AshGw/ashcrypt#features) tag below to learn more about the security features.
 
 ### Usage ##
 1) Generate a key if you don't have one already
 ```python
 mainkey = Enc.genkey()
 ```
 2) Before encrypting or decrypting anything, first set the arguments you want to pass, you can have an encrypted message or a  decrypted message , and a mainkey to use.
@@ -318,11 +319,11 @@
 <br>To run the GUI anywhere
 ```shell
 python -m ashcrypt.gui
 ```
 
 
 ## License ##
-This project is licensed under the [MIT LICENSE](https://github.com/AshGw/AES-256/blob/main/LICENSE).
+This project is licensed under the [MIT LICENSE](https://github.com/AshGw/ashcrypt/blob/main/LICENSE).
 ## Acknowledgments ##
 This cryptographic scheme is inspired by secure cryptographic practices and various open-source implementations.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ashcrypt-3.2.1/ashcrypt/crypt.py` & `ashcrypt-3.2.2/ashcrypt/crypt.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.2.1/ashcrypt/database.py` & `ashcrypt-3.2.2/ashcrypt/database.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.2.1/ashcrypt/filecrypt.py` & `ashcrypt-3.2.2/ashcrypt/filecrypt.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.2.1/ashcrypt/gui.py` & `ashcrypt-3.2.2/ashcrypt/gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-import ashcrypt.utils.safepack.text as At
-import ashcrypt.utils.safepack.file as Af
+import ashcrypt.utils.safepack.text as at
+import ashcrypt.utils.safepack.file as af
 from ashcrypt.utils.safepack import qr
 from ashcrypt.utils.consts import Gui
-import ashcrypt.database as Ad
+import ashcrypt.database as ad
 import ttkbootstrap as tk
 import platform
 import secrets
 import os.path
 import string
 import atexit
 import json
@@ -346,26 +346,26 @@
                 conn_path_db = os.path.join(usable_real_path, maindbname)
                 if os.path.isfile(
                         fullpath +
                         f'\\{maindbname}') or os.path.isfile(
                         fullpath +
                         f'/{maindbname}'):
                     db_already_exists_blocker = 1
-                    main_db_conn = Ad.Database(conn_path_db)
+                    main_db_conn = ad.Database(conn_path_db)
                     main_db_conn.addtable()
                     main_db_name_result_var.set('CONNECTED')
                     db_display_text.delete('1.0', tk.END)
                     db_display_text.insert(
                         tk.END, f'Connected to {maindbname}..\n\n')
                     success_maindb_connection_blocker = 1
                     encfiletoolbutt.state(['!disabled'])
                     decfiletoolbutt.state(['!disabled'])
                 else:
                     db_already_exists_blocker = 0
-                    main_db_conn = Ad.Database(conn_path_db)
+                    main_db_conn = ad.Database(conn_path_db)
                     main_db_conn.addtable()
                     db_display_text.delete('1.0', tk.END)
                     db_display_text.insert(
                         tk.END,
                         f"Created and Connected to '{maindbname}'.. in the directory '{fullpath}'\n\n")
                     success_maindb_connection_blocker = 1
                     encfiletoolbutt.state(['!disabled'])
@@ -396,28 +396,28 @@
             conn_path_keys = os.path.join(usable_real_path, keys_db)
             if db_already_exists_blocker == 1:
                 if os.path.isfile(
                         usable_real_path +
                         dbname_keys_win) or os.path.isfile(
                         usable_real_path +
                         dbname_keys_unix):
-                    keys_db_conn = Ad.Database(conn_path_keys)
+                    keys_db_conn = ad.Database(conn_path_keys)
                     keys_db_conn.addtable()
                     db_display_text.insert(
                         tk.END, f"Connected to '{keys_db}' ..\n\n")
                     success_keysdb_connection_blocker = 1
                 else:
-                    keys_db_conn = Ad.Database(conn_path_keys)
+                    keys_db_conn = ad.Database(conn_path_keys)
                     keys_db_conn.addtable()
                     db_display_text.insert(
                         tk.END,
                         f"'{keys_db}' NOT FOUND ! ==> Created and Connected to '{keys_db}' ..\n\n")
                     success_keysdb_connection_blocker = 1
             else:
-                keys_db_conn = Ad.Database(conn_path_keys)
+                keys_db_conn = ad.Database(conn_path_keys)
                 keys_db_conn.addtable()
                 db_display_text.insert(
                     tk.END, f"Created and Connected to '{keys_db}' ..\n\n")
                 success_keysdb_connection_blocker = 1
         except BaseException:
             db_display_text.delete('1.0', tk.END)
             db_display_text.insert(
@@ -615,35 +615,35 @@
 
 
 '''------------TEXT DECRYPTION/ENCRYPTION STARTED--------------'''
 
 
 def encryption():
     m = inputfield1_1.get()
-    if Af.CryptFile.keyverify(
+    if af.CryptFile.keyverify(
             mainkeyvar.get()) == 1 and keySelectionFlag.get() == 1:
         if len(m) > 200:
             outputvar1.set('Too Long')
         else:
             if inputfield1_1.get():
                 progressbar.start()
-                a = At.Crypt(m, mainkeyvar.get())
+                a = at.Crypt(m, mainkeyvar.get())
                 b = a.encrypt()[1]
                 outputvar1.set(b.__str__())
                 if var1.get() == 1:
                     qr.tqr(b)
 
 
 def decryption():
     n = inputfield2_1.get()
-    if Af.CryptFile.keyverify(
+    if af.CryptFile.keyverify(
             mainkeyvar.get()) == 1 and keySelectionFlag.get() == 1:
         if inputfield2_1.get():
             progressbar2.start()
-            a = At.Crypt(n, mainkeyvar.get())
+            a = at.Crypt(n, mainkeyvar.get())
             b = a.decrypt()[1]
             outputvar2.set(b.__str__())
             if var2.get() == 1:
                 if not len(b) > 200:
                     qr.tqr(b)
 
 
@@ -797,15 +797,15 @@
 
 def enc_file():
     global add_enc_to_db, main_db_conn, mainkey
     if 1:
         if keySelectionFlag.get() != 0:
             filename = filenameStringVar.get().strip()
             key = mainkey
-            target = Af.CryptFile(filename, key)
+            target = af.CryptFile(filename, key)
             a = target.encrypt()
             if a == 1:
                 filename = filename + '.crypt'
                 filenameStringVar.set(filename)
                 if platform.system() == 'Windows':
                     resultvarfile.set(
                         '    Encrypted Successfully / added .crypt')
@@ -860,15 +860,15 @@
 
 def decfile():
     global add_dec_to_db, main_db_conn, mainkey
     if 1:
         if keySelectionFlag.get() != 0:
             filename = filenameStringVar.get().strip()
             key = mainkey
-            target = Af.CryptFile(filename, key)
+            target = af.CryptFile(filename, key)
             a = target.decrypt()
             if a == 1:
                 filename = os.path.splitext(filename)[0]
                 filenameStringVar.set(filename)
                 if platform.system() == 'Windows':
                     resultvarfile.set(
                         '    Decrypted Successfully + removed .crypt')
@@ -998,15 +998,15 @@
 
 
 keySelectionFlag = tk.IntVar(value=0)
 
 
 def main_key_wrapper():
     global success_keysdb_connection_blocker, mainkey
-    if Af.CryptFile.keyverify(mainkeyvar.get().strip()) == 1:
+    if af.CryptFile.keyverify(mainkeyvar.get().strip()) == 1:
         mainkey = mainkeyvar.get().strip()
         keyref_gen()
         keyselectionvar.set('       SELECTED')
         keySelectionFlag.set(1)
         try:
             if success_keysdb_connection_blocker and os.path.isfile(
                     filenameStringVar.get().strip()):
@@ -1090,15 +1090,15 @@
                              textvariable=keyselectionvar,
                              bootstyle='info',
                              font='terminal 11 bold')
 keyselectionLabel.place(relx=0.15, rely=0.465, height=50)
 
 
 def genkey():
-    keyGenVar.set(Af.CryptFile.genkey())
+    keyGenVar.set(af.CryptFile.genkey())
 
 
 keyGenVar = tk.StringVar(value='')
 keyGenEntry = tk.Entry(master=frameFile2,
                        font='Calibre 12 bold',
                        textvariable=keyGenVar,
                        width=23)
```

### Comparing `ashcrypt-3.2.1/ashcrypt/sandbox/clicrypt.py` & `ashcrypt-3.2.2/ashcrypt/sandbox/clicrypt.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.2.1/ashcrypt/textcrypt.py` & `ashcrypt-3.2.2/ashcrypt/textcrypt.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.2.1/ashcrypt/unittests/test_crypt.py` & `ashcrypt-3.2.2/ashcrypt/unittests/test_crypt.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.2.1/ashcrypt/utils/exceptions/fixed.py` & `ashcrypt-3.2.2/ashcrypt/utils/exceptions/fixed.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.2.1/ashcrypt/utils/safepack/file.py` & `ashcrypt-3.2.2/ashcrypt/utils/safepack/file.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.2.1/ashcrypt/utils/safepack/text.py` & `ashcrypt-3.2.2/ashcrypt/utils/safepack/text.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.2.1/ashcrypt.egg-info/PKG-INFO` & `ashcrypt-3.2.2/ashcrypt.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: ashcrypt
-Version: 3.2.1
+Version: 3.2.2
 Summary: Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with a database module to store encrypted content.
 Home-page: https://github.com/AshGw/AES-256.git
 Author: Ashref Gwader
 Author-email: AshrefGw@proton.me
 License: UNKNOWN
 Description: # Cryptography App & Library For AES-256
         ## Docs ## 
-        **Visit The [GitHub](https://github.com/AshGw/AES-256/tree/main) Repository.**
+        **Visit The [GitHub](https://github.com/AshGw/ashcrypt/tree/main) Repository.**
         
         
 Keywords: Cryptography application,cryptography libraryAES-256
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ashcrypt-3.2.1/ashcrypt.egg-info/SOURCES.txt` & `ashcrypt-3.2.2/ashcrypt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.2.1/setup.py` & `ashcrypt-3.2.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('ashcrypt/README.md', 'r') as f:
     readme = f.read()
 
 setup(
     name='ashcrypt',
-    version='3.2.1',
+    version='3.2.2',
     author='Ashref Gwader',
     author_email='AshrefGw@proton.me',
     python_requires='>=3.7',
     description="Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along"
                 " with a database module to store encrypted content.",
     long_description_content_type='text/markdown',
     long_description=readme,
```

