# Comparing `tmp/tempmail-python-2.0.0.tar.gz` & `tmp/tempmail-python-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tempmail-python-2.0.0.tar", last modified: Sun Aug  6 10:03:25 2023, max compression
+gzip compressed data, was "tempmail-python-2.1.0.tar", last modified: Mon Aug  7 10:02:17 2023, max compression
```

## Comparing `tempmail-python-2.0.0.tar` & `tempmail-python-2.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 10:03:25.233636 tempmail-python-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-08-06 10:03:15.000000 tempmail-python-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-08-06 10:03:25.233636 tempmail-python-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-08-06 10:03:15.000000 tempmail-python-2.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 10:03:25.233636 tempmail-python-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-08-06 10:03:15.000000 tempmail-python-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 10:03:25.233636 tempmail-python-2.0.0/tempmail/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-08-06 10:03:15.000000 tempmail-python-2.0.0/tempmail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-08-06 10:03:15.000000 tempmail-python-2.0.0/tempmail/providers.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-08-06 10:03:15.000000 tempmail-python-2.0.0/tempmail/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 10:03:25.233636 tempmail-python-2.0.0/tempmail_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-08-06 10:03:25.000000 tempmail-python-2.0.0/tempmail_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-08-06 10:03:25.000000 tempmail-python-2.0.0/tempmail_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 10:03:25.000000 tempmail-python-2.0.0/tempmail_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-06 10:03:25.000000 tempmail-python-2.0.0/tempmail_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-06 10:03:25.000000 tempmail-python-2.0.0/tempmail_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:02:17.107611 tempmail-python-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-08-07 10:02:07.000000 tempmail-python-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-08-07 10:02:17.107611 tempmail-python-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-08-07 10:02:07.000000 tempmail-python-2.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 10:02:17.107611 tempmail-python-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-08-07 10:02:07.000000 tempmail-python-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:02:17.107611 tempmail-python-2.1.0/tempmail/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-08-07 10:02:07.000000 tempmail-python-2.1.0/tempmail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-08-07 10:02:07.000000 tempmail-python-2.1.0/tempmail/providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-08-07 10:02:07.000000 tempmail-python-2.1.0/tempmail/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:02:17.107611 tempmail-python-2.1.0/tempmail_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-08-07 10:02:17.000000 tempmail-python-2.1.0/tempmail_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-08-07 10:02:17.000000 tempmail-python-2.1.0/tempmail_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 10:02:17.000000 tempmail-python-2.1.0/tempmail_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-07 10:02:17.000000 tempmail-python-2.1.0/tempmail_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-07 10:02:17.000000 tempmail-python-2.1.0/tempmail_python.egg-info/top_level.txt
```

### Comparing `tempmail-python-2.0.0/LICENSE` & `tempmail-python-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tempmail-python-2.0.0/PKG-INFO` & `tempmail-python-2.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tempmail-python
-Version: 2.0.0
+Version: 2.1.0
 Summary: Python library for generating and managing temporary email addresses.
 Home-page: https://github.com/cubicbyte/tempmail-python
 Author: cubicbyte
 Author-email: bmaruhnenko@gmail.com
 License: MIT
 Keywords: disposable-email temporary-email temp-email temp-mail email mail email-generator mail-generator
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `tempmail-python-2.0.0/README.md` & `tempmail-python-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `tempmail-python-2.0.0/setup.py` & `tempmail-python-2.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 def read(path: str) -> str:
     with open(path, 'r', encoding='utf-8') as f:
         return f.read()
 
 setup(
     name='tempmail-python',
-    version='2.0.0',
+    version='2.1.0',
     description='Python library for generating and managing temporary email addresses.',
     long_description=read('README.md'),
     long_description_content_type='text/markdown',
     author='cubicbyte',
     author_email='bmaruhnenko@gmail.com',
     url='https://github.com/cubicbyte/tempmail-python',
     packages = find_packages(),
```

### Comparing `tempmail-python-2.0.0/tempmail/providers.py` & `tempmail-python-2.1.0/tempmail/providers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import time
 import random
+from datetime import datetime
 from dataclasses import dataclass
 
 import requests
 
 from . import utils
 
 __all__ = ('OneSecMail',)
@@ -77,14 +78,18 @@
         id: int
         from_addr: str
         subject: str
         date_str: str
         _mail: 'OneSecMail'
 
         @property
+        def date(self) -> datetime:
+            return datetime.fromisoformat(self.date_str)
+
+        @property
         def message(self) -> 'OneSecMail.Message':
             return self._mail.get_message(self.id)
 
         @classmethod
         def from_dict(cls, mail: 'OneSecMail', msg_info: dict[str, any]) -> 'OneSecMail.MessageInfo':
             return cls(
                 _mail=mail,
@@ -95,39 +100,43 @@
                 )
 
     @dataclass
     class Message:
         id: int
         from_addr: str
         subject: str
-        date: str
+        date_str: str
         body: str
         test_body: str
         html_body: str
         _mail: 'OneSecMail'
         _attachments: list[dict[str, any]]
 
+        @property
+        def date(self) -> datetime:
+            return datetime.fromisoformat(self.date_str)
+
+        @property
+        def attachments(self) -> list['OneSecMail.Attachment']:
+            return [OneSecMail.Attachment.from_dict(self._mail, self.id, attachment) for attachment in self._attachments]
+
         @classmethod
         def from_dict(cls, mail: 'OneSecMail', msg: dict[str, any]) -> 'OneSecMail.Message':
             return cls(
                 _mail=mail,
                 _attachments=msg['attachments'],
                 id=msg['id'],
                 from_addr=msg['from'],
                 subject=msg['subject'],
-                date=msg['date'],
+                date_str=msg['date'],
                 body=msg['textBody'],
                 test_body=msg['textBody'],
                 html_body=msg['htmlBody'],
                 )
 
-        @property
-        def attachments(self) -> list['OneSecMail.Attachment']:
-            return [OneSecMail.Attachment.from_dict(self._mail, self.id, attachment) for attachment in self._attachments]
-
     @dataclass
     class Attachment:
         filename: str
         content_type: str
         size: int
         _mail: 'OneSecMail'
         _message_id: int
```

### Comparing `tempmail-python-2.0.0/tempmail_python.egg-info/PKG-INFO` & `tempmail-python-2.1.0/tempmail_python.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tempmail-python
-Version: 2.0.0
+Version: 2.1.0
 Summary: Python library for generating and managing temporary email addresses.
 Home-page: https://github.com/cubicbyte/tempmail-python
 Author: cubicbyte
 Author-email: bmaruhnenko@gmail.com
 License: MIT
 Keywords: disposable-email temporary-email temp-email temp-mail email mail email-generator mail-generator
 Classifier: Development Status :: 5 - Production/Stable
```

