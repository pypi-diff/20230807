# Comparing `tmp/TelegramContract2vCard-1.0.0.tar.gz` & `tmp/TelegramContract2vCard-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TelegramContract2vCard-1.0.0.tar", last modified: Mon Aug  7 11:55:15 2023, max compression
+gzip compressed data, was "TelegramContract2vCard-1.0.1.tar", last modified: Mon Aug  7 14:57:44 2023, max compression
```

## Comparing `TelegramContract2vCard-1.0.0.tar` & `TelegramContract2vCard-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-08-07 11:55:15.026023 TelegramContract2vCard-1.0.0/
--rw-rw-rw-   0        0        0      648 2023-08-07 11:55:15.026023 TelegramContract2vCard-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       55 2023-07-03 16:49:59.000000 TelegramContract2vCard-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-08-07 11:55:15.014027 TelegramContract2vCard-1.0.0/TelegramContract2vCard/
--rw-rw-rw-   0        0        0       21 2023-08-07 11:53:20.000000 TelegramContract2vCard-1.0.0/TelegramContract2vCard/__init__.py
--rw-rw-rw-   0        0        0     4020 2023-08-07 10:52:31.000000 TelegramContract2vCard-1.0.0/TelegramContract2vCard/main.py
-drwxrwxrwx   0        0        0        0 2023-08-07 11:55:15.024025 TelegramContract2vCard-1.0.0/TelegramContract2vCard.egg-info/
--rw-rw-rw-   0        0        0      648 2023-08-07 11:55:14.000000 TelegramContract2vCard-1.0.0/TelegramContract2vCard.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      358 2023-08-07 11:55:15.000000 TelegramContract2vCard-1.0.0/TelegramContract2vCard.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-07 11:55:14.000000 TelegramContract2vCard-1.0.0/TelegramContract2vCard.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-08-07 11:55:14.000000 TelegramContract2vCard-1.0.0/TelegramContract2vCard.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       15 2023-08-07 11:55:14.000000 TelegramContract2vCard-1.0.0/TelegramContract2vCard.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-08-07 11:55:14.000000 TelegramContract2vCard-1.0.0/TelegramContract2vCard.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-07 11:55:15.027025 TelegramContract2vCard-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      894 2023-08-07 11:51:25.000000 TelegramContract2vCard-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 14:57:44.586892 TelegramContract2vCard-1.0.1/
+-rw-rw-rw-   0        0        0      648 2023-08-07 14:57:44.585891 TelegramContract2vCard-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1703 2023-08-07 13:05:21.000000 TelegramContract2vCard-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-08-07 14:57:44.575893 TelegramContract2vCard-1.0.1/TelegramContract2vCard/
+-rw-rw-rw-   0        0        0       65 2023-08-07 14:54:03.000000 TelegramContract2vCard-1.0.1/TelegramContract2vCard/__init__.py
+-rw-rw-rw-   0        0        0     4020 2023-08-07 10:52:31.000000 TelegramContract2vCard-1.0.1/TelegramContract2vCard/main.py
+drwxrwxrwx   0        0        0        0 2023-08-07 14:57:44.584894 TelegramContract2vCard-1.0.1/TelegramContract2vCard.egg-info/
+-rw-rw-rw-   0        0        0      648 2023-08-07 14:57:44.000000 TelegramContract2vCard-1.0.1/TelegramContract2vCard.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      358 2023-08-07 14:57:44.000000 TelegramContract2vCard-1.0.1/TelegramContract2vCard.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 14:57:44.000000 TelegramContract2vCard-1.0.1/TelegramContract2vCard.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-08-07 11:55:14.000000 TelegramContract2vCard-1.0.1/TelegramContract2vCard.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       15 2023-08-07 14:57:44.000000 TelegramContract2vCard-1.0.1/TelegramContract2vCard.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-08-07 14:57:44.000000 TelegramContract2vCard-1.0.1/TelegramContract2vCard.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-07 14:57:44.587893 TelegramContract2vCard-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      894 2023-08-07 14:54:18.000000 TelegramContract2vCard-1.0.1/setup.py
```

### Comparing `TelegramContract2vCard-1.0.0/PKG-INFO` & `TelegramContract2vCard-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TelegramContract2vCard
-Version: 1.0.0
+Version: 1.0.1
 Summary: make telegram contacts.html or result.json to vCard automatically
 Home-page: https://github.com/jjh4450/TelegramContract2vCard
 Author: jjh4450
 Author-email: jjh4450git@gmail.com
 Keywords: telegram,contacts,vcf,vcard,html,json,parser
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `TelegramContract2vCard-1.0.0/TelegramContract2vCard/main.py` & `TelegramContract2vCard-1.0.1/TelegramContract2vCard/main.py`

 * *Files identical despite different names*

### Comparing `TelegramContract2vCard-1.0.0/TelegramContract2vCard.egg-info/PKG-INFO` & `TelegramContract2vCard-1.0.1/TelegramContract2vCard.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TelegramContract2vCard
-Version: 1.0.0
+Version: 1.0.1
 Summary: make telegram contacts.html or result.json to vCard automatically
 Home-page: https://github.com/jjh4450/TelegramContract2vCard
 Author: jjh4450
 Author-email: jjh4450git@gmail.com
 Keywords: telegram,contacts,vcf,vcard,html,json,parser
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `TelegramContract2vCard-1.0.0/setup.py` & `TelegramContract2vCard-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='TelegramContract2vCard',
-    version='1.0.0',
+    version='1.0.1',
     description='make telegram contacts.html or result.json to vCard automatically',
     author='jjh4450',
     author_email='jjh4450git@gmail.com',
     url='https://github.com/jjh4450/TelegramContract2vCard',
     install_requires=["beautifulsoup4"],
     packages=find_packages(exclude=[]),
     keywords=['telegram', 'contacts', 'vcf', 'vcard', 'html', 'json', 'parser'],
```

