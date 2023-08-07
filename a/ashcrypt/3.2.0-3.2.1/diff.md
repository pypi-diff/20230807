# Comparing `tmp/ashcrypt-3.2.0.tar.gz` & `tmp/ashcrypt-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ashcrypt-3.2.0.tar", last modified: Sun Aug  6 11:28:23 2023, max compression
+gzip compressed data, was "dist/ashcrypt-3.2.1.tar", last modified: Mon Aug  7 10:54:57 2023, max compression
```

## Comparing `ashcrypt-3.2.0.tar` & `ashcrypt-3.2.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 11:28:23.000000 ashcrypt-3.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-06 11:28:23.000000 ashcrypt-3.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17170 2023-08-06 11:28:12.000000 ashcrypt-3.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 11:28:23.000000 ashcrypt-3.2.0/ashcrypt/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-06 11:28:12.000000 ashcrypt-3.2.0/ashcrypt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-08-06 11:28:12.000000 ashcrypt-3.2.0/ashcrypt/crypt.py
--rw-r--r--   0 runner    (1001) docker     (123)    10523 2023-08-06 11:28:12.000000 ashcrypt-3.2.0/ashcrypt/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-08-06 11:28:12.000000 ashcrypt-3.2.0/ashcrypt/filecrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)    39274 2023-08-06 11:28:12.000000 ashcrypt-3.2.0/ashcrypt/gui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 11:28:23.000000 ashcrypt-3.2.0/ashcrypt/sandbox/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 11:28:12.000000 ashcrypt-3.2.0/ashcrypt/sandbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6811 2023-08-06 11:28:12.000000 ashcrypt-3.2.0/ashcrypt/sandbox/clicrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-08-06 11:28:12.000000 ashcrypt-3.2.0/ashcrypt/textcrypt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 11:28:23.000000 ashcrypt-3.2.0/ashcrypt/unittests/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-06 11:28:12.000000 ashcrypt-3.2.0/ashcrypt/unittests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-08-06 11:28:12.000000 ashcrypt-3.2.0/ashcrypt/unittests/test_crypt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 11:28:23.000000 ashcrypt-3.2.0/ashcrypt/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 11:28:12.000000 ashcrypt-3.2.0/ashcrypt/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 11:28:23.000000 ashcrypt-3.2.0/ashcrypt/utils/consts/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-06 11:28:12.000000 ashcrypt-3.2.0/ashcrypt/utils/consts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-08-06 11:28:12.000000 ashcrypt-3.2.0/ashcrypt/utils/consts/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 11:28:23.000000 ashcrypt-3.2.0/ashcrypt/utils/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-06 11:28:12.000000 ashcrypt-3.2.0/ashcrypt/utils/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-08-06 11:28:12.000000 ashcrypt-3.2.0/ashcrypt/utils/exceptions/dynamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-08-06 11:28:12.000000 ashcrypt-3.2.0/ashcrypt/utils/exceptions/fixed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 11:28:23.000000 ashcrypt-3.2.0/ashcrypt/utils/safepack/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 11:28:12.000000 ashcrypt-3.2.0/ashcrypt/utils/safepack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-08-06 11:28:12.000000 ashcrypt-3.2.0/ashcrypt/utils/safepack/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-08-06 11:28:12.000000 ashcrypt-3.2.0/ashcrypt/utils/safepack/qr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-08-06 11:28:12.000000 ashcrypt-3.2.0/ashcrypt/utils/safepack/text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 11:28:23.000000 ashcrypt-3.2.0/ashcrypt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-06 11:28:23.000000 ashcrypt-3.2.0/ashcrypt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-08-06 11:28:23.000000 ashcrypt-3.2.0/ashcrypt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 11:28:23.000000 ashcrypt-3.2.0/ashcrypt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-06 11:28:23.000000 ashcrypt-3.2.0/ashcrypt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-06 11:28:23.000000 ashcrypt-3.2.0/ashcrypt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 11:28:23.000000 ashcrypt-3.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-08-06 11:28:12.000000 ashcrypt-3.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:54:57.000000 ashcrypt-3.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-07 10:54:57.000000 ashcrypt-3.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16950 2023-08-07 10:54:47.000000 ashcrypt-3.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:54:57.000000 ashcrypt-3.2.1/ashcrypt/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-08-07 10:54:47.000000 ashcrypt-3.2.1/ashcrypt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-08-07 10:54:47.000000 ashcrypt-3.2.1/ashcrypt/crypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10523 2023-08-07 10:54:47.000000 ashcrypt-3.2.1/ashcrypt/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-08-07 10:54:47.000000 ashcrypt-3.2.1/ashcrypt/filecrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39274 2023-08-07 10:54:47.000000 ashcrypt-3.2.1/ashcrypt/gui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:54:57.000000 ashcrypt-3.2.1/ashcrypt/sandbox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 10:54:47.000000 ashcrypt-3.2.1/ashcrypt/sandbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6811 2023-08-07 10:54:47.000000 ashcrypt-3.2.1/ashcrypt/sandbox/clicrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-08-07 10:54:47.000000 ashcrypt-3.2.1/ashcrypt/textcrypt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:54:57.000000 ashcrypt-3.2.1/ashcrypt/unittests/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-07 10:54:47.000000 ashcrypt-3.2.1/ashcrypt/unittests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-08-07 10:54:47.000000 ashcrypt-3.2.1/ashcrypt/unittests/test_crypt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:54:57.000000 ashcrypt-3.2.1/ashcrypt/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 10:54:47.000000 ashcrypt-3.2.1/ashcrypt/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:54:57.000000 ashcrypt-3.2.1/ashcrypt/utils/consts/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-07 10:54:47.000000 ashcrypt-3.2.1/ashcrypt/utils/consts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-08-07 10:54:47.000000 ashcrypt-3.2.1/ashcrypt/utils/consts/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:54:57.000000 ashcrypt-3.2.1/ashcrypt/utils/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-07 10:54:47.000000 ashcrypt-3.2.1/ashcrypt/utils/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-08-07 10:54:47.000000 ashcrypt-3.2.1/ashcrypt/utils/exceptions/dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-08-07 10:54:47.000000 ashcrypt-3.2.1/ashcrypt/utils/exceptions/fixed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:54:57.000000 ashcrypt-3.2.1/ashcrypt/utils/safepack/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 10:54:47.000000 ashcrypt-3.2.1/ashcrypt/utils/safepack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-08-07 10:54:47.000000 ashcrypt-3.2.1/ashcrypt/utils/safepack/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-08-07 10:54:47.000000 ashcrypt-3.2.1/ashcrypt/utils/safepack/qr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-08-07 10:54:47.000000 ashcrypt-3.2.1/ashcrypt/utils/safepack/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:54:57.000000 ashcrypt-3.2.1/ashcrypt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-07 10:54:57.000000 ashcrypt-3.2.1/ashcrypt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-08-07 10:54:57.000000 ashcrypt-3.2.1/ashcrypt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 10:54:57.000000 ashcrypt-3.2.1/ashcrypt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-07 10:54:57.000000 ashcrypt-3.2.1/ashcrypt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-07 10:54:57.000000 ashcrypt-3.2.1/ashcrypt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 10:54:57.000000 ashcrypt-3.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-08-07 10:54:47.000000 ashcrypt-3.2.1/setup.py
```

### Comparing `ashcrypt-3.2.0/PKG-INFO` & `ashcrypt-3.2.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ashcrypt
-Version: 3.2.0
+Version: 3.2.1
 Summary: Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with a database module to store encrypted content.
 Home-page: https://github.com/AshGw/AES-256.git
 Author: Ashref Gwader
 Author-email: AshrefGw@proton.me
 License: UNKNOWN
 Description: # Cryptography App & Library For AES-256
         ## Docs ##
```

### Comparing `ashcrypt-3.2.0/README.md` & `ashcrypt-3.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -85,21 +85,21 @@
 ```python
 mainkey = '6ce113be19e898c2b98df82b7fa8efb166928925fc05574a54eb1114c3410900'
 ```
 The message can be of type str or bytes.
 ```python 
 message = 'Hello There'  # str
 message = b'Hello There' # bytes
-```
-an encrypted message ( to decrypt ): 
-```python
+
+# an encrypted message ( to decrypt ): 
+
 message = 'ZEfikRiNQ4EE1y5E-Qn4gQbo8goVpWLPstqTlgWtoRq1CK_oeMz4oelCYNpM-NZyzSIKk7DazkAUO9HcZJzWWMXR6zqRjNTN-c1Q6vRWSkj1g20oL6JbzUvEJL3xvY2-Fye1simoOAr7YP5YHAnSYAAAADIA0juak_JYQnzXQ-apJ8azahvngigFrHRg142g7OqvfA=='
-```
-or bytes encrypted message ( to decrypt ):
-```python
+
+# or bytes encrypted message ( to decrypt ):
+
 message = b'dG\xe2\x91\x18\x8dC\x81\x04\xd7.D\xf9\t\xf8\x81\x06\xe8\xf2\n\x15\xa5b\xcf\xb2\xda\x93\x96\x05\xad\xa1\x1a\xb5\x08\xaf\xe8x\xcc\xf8\xa1\xe9B`\xdaL\xf8\xd6r\xcd"\n\x93\xb0\xda\xce@\x14;\xd1\xdcd\x9c\xd6X\xc5\xd1\xeb:\x91\x8c\xd4\xcd\xf9\xcdP\xea\xf4VJH\xf5\x83m(/\xa2[\xcdK\xc4$\xbd\xf1\xbd\x8d\xbe\x17\'\xb5\xb2)\xa88\n\xfb`\xfeX\x1c\t\xd2`\x00\x00\x002\x00\xd2;\x9a\x93\xf2XB|\xd7C\xe6\xa9\'\xc6\xb3j\x1b\xe7\x82(\x05\xact`\xd7\x8d\xa0\xec\xea\xaf|'
 ```
 3) Now pass the arguments accordingly. If you have a normal message and you try to decrypt it, an Exception will be raised so pass the arguments to the right classes. 
 <br><br>So first create an instance of either the `Enc` or `Dec` class. 
 <br>Here I chose to encrypt a message 
 ```python
 a = Enc(message, mainkey)
@@ -210,19 +210,14 @@
 <br>Index `[1]` contains the encrypted/decrypted content.
 
 ## `database` ##
 To support efficient content management, I have integrated this database module to enable the storage and retrieval of encrypted content in a safe and secure manner using sqlite.
 
 Ensuring that the encrypted data remains organized and readily accessible to anyone with the right key. Any content going in must be encrypted with a key that you must keep secured.
 
-**Note** that in `database.py` I'm using `dataclasses` module which was introduced in `python 3.7`, so make sure to install it if you have an older version.
-Run:
-```python
-pip install dataclasses
-```
 
 ### Usage ## 
 In this module I'm providing built-in functions to make it easier to perform usual queries over Sqlite tables , by default it creates a table `Classified` with two default columns :
 
 **content** : This can be a single character or a whole movie in binary, that depends on your specific needs.
 
 **key** : This key column wasn't indeed meant to store a key itself but rather store a reference to the actual key.
```

### Comparing `ashcrypt-3.2.0/ashcrypt/crypt.py` & `ashcrypt-3.2.1/ashcrypt/crypt.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.2.0/ashcrypt/database.py` & `ashcrypt-3.2.1/ashcrypt/database.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.2.0/ashcrypt/filecrypt.py` & `ashcrypt-3.2.1/ashcrypt/filecrypt.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.2.0/ashcrypt/gui.py` & `ashcrypt-3.2.1/ashcrypt/gui.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.2.0/ashcrypt/sandbox/clicrypt.py` & `ashcrypt-3.2.1/ashcrypt/sandbox/clicrypt.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.2.0/ashcrypt/textcrypt.py` & `ashcrypt-3.2.1/ashcrypt/textcrypt.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.2.0/ashcrypt/unittests/test_crypt.py` & `ashcrypt-3.2.1/ashcrypt/unittests/test_crypt.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.2.0/ashcrypt/utils/exceptions/fixed.py` & `ashcrypt-3.2.1/ashcrypt/utils/exceptions/fixed.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.2.0/ashcrypt/utils/safepack/file.py` & `ashcrypt-3.2.1/ashcrypt/utils/safepack/file.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.2.0/ashcrypt/utils/safepack/text.py` & `ashcrypt-3.2.1/ashcrypt/utils/safepack/text.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.2.0/ashcrypt.egg-info/PKG-INFO` & `ashcrypt-3.2.1/ashcrypt.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ashcrypt
-Version: 3.2.0
+Version: 3.2.1
 Summary: Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with a database module to store encrypted content.
 Home-page: https://github.com/AshGw/AES-256.git
 Author: Ashref Gwader
 Author-email: AshrefGw@proton.me
 License: UNKNOWN
 Description: # Cryptography App & Library For AES-256
         ## Docs ##
```

### Comparing `ashcrypt-3.2.0/ashcrypt.egg-info/SOURCES.txt` & `ashcrypt-3.2.1/ashcrypt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.2.0/setup.py` & `ashcrypt-3.2.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('ashcrypt/README.md', 'r') as f:
     readme = f.read()
 
 setup(
     name='ashcrypt',
-    version='3.2.0',
+    version='3.2.1',
     author='Ashref Gwader',
     author_email='AshrefGw@proton.me',
     python_requires='>=3.7',
     description="Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along"
                 " with a database module to store encrypted content.",
     long_description_content_type='text/markdown',
     long_description=readme,
```

