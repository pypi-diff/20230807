# Comparing `tmp/BanglaSpeech2Text-0.0.9.tar.gz` & `tmp/BanglaSpeech2Text-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BanglaSpeech2Text-0.0.9.tar", last modified: Fri Jan 13 12:18:02 2023, max compression
+gzip compressed data, was "BanglaSpeech2Text-1.0.1.tar", last modified: Mon Aug  7 15:49:24 2023, max compression
```

## Comparing `BanglaSpeech2Text-0.0.9.tar` & `BanglaSpeech2Text-1.0.1.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-01-13 12:18:02.155764 BanglaSpeech2Text-0.0.9/
-drwxrwxrwx   0        0        0        0 2023-01-13 12:18:02.136213 BanglaSpeech2Text-0.0.9/BanglaSpeech2Text.egg-info/
--rw-rw-rw-   0        0        0     5865 2023-01-13 12:17:59.000000 BanglaSpeech2Text-0.0.9/BanglaSpeech2Text.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      543 2023-01-13 12:18:01.000000 BanglaSpeech2Text-0.0.9/BanglaSpeech2Text.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-13 12:17:59.000000 BanglaSpeech2Text-0.0.9/BanglaSpeech2Text.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-01-12 15:49:57.000000 BanglaSpeech2Text-0.0.9/BanglaSpeech2Text.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      367 2023-01-13 12:17:59.000000 BanglaSpeech2Text-0.0.9/BanglaSpeech2Text.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-01-13 12:17:59.000000 BanglaSpeech2Text-0.0.9/BanglaSpeech2Text.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1083 2023-01-12 06:03:07.000000 BanglaSpeech2Text-0.0.9/LICENSE
--rw-rw-rw-   0        0        0       24 2023-01-12 14:46:32.000000 BanglaSpeech2Text-0.0.9/MANIFEST.in
--rw-rw-rw-   0        0        0     5865 2023-01-13 12:18:02.154765 BanglaSpeech2Text-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     4176 2023-01-13 10:47:24.000000 BanglaSpeech2Text-0.0.9/README.md
-drwxrwxrwx   0        0        0        0 2023-01-13 12:18:02.145763 BanglaSpeech2Text-0.0.9/banglaspeech2text/
--rw-rw-rw-   0        0        0       76 2023-01-12 15:00:04.000000 BanglaSpeech2Text-0.0.9/banglaspeech2text/__init__.py
--rw-rw-rw-   0        0        0     3994 2023-01-13 11:37:18.000000 BanglaSpeech2Text-0.0.9/banglaspeech2text/speech2text.py
-drwxrwxrwx   0        0        0        0 2023-01-13 12:18:02.152765 BanglaSpeech2Text-0.0.9/banglaspeech2text/utils/
--rw-rw-rw-   0        0        0      535 2023-01-13 11:37:00.000000 BanglaSpeech2Text-0.0.9/banglaspeech2text/utils/__init__.py
--rw-rw-rw-   0        0        0    12299 2023-01-13 10:34:47.000000 BanglaSpeech2Text-0.0.9/banglaspeech2text/utils/download_models.py
--rw-rw-rw-   0        0        0      447 2023-01-13 11:55:53.000000 BanglaSpeech2Text-0.0.9/banglaspeech2text/utils/download_path.py
--rw-rw-rw-   0        0        0     2359 2023-01-13 11:55:27.000000 BanglaSpeech2Text-0.0.9/banglaspeech2text/utils/extras.py
--rw-rw-rw-   0        0        0     1553 2023-01-13 09:21:18.000000 BanglaSpeech2Text-0.0.9/banglaspeech2text/utils/install_packages.py
--rw-rw-rw-   0        0        0       42 2023-01-13 12:18:02.155764 BanglaSpeech2Text-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0     2235 2023-01-13 12:17:15.000000 BanglaSpeech2Text-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 15:49:24.525382 BanglaSpeech2Text-1.0.1/
+drwxrwxrwx   0        0        0        0 2023-08-07 15:49:24.451387 BanglaSpeech2Text-1.0.1/BanglaSpeech2Text.egg-info/
+-rw-rw-rw-   0        0        0     7574 2023-08-07 15:49:22.000000 BanglaSpeech2Text-1.0.1/BanglaSpeech2Text.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      581 2023-08-07 15:49:23.000000 BanglaSpeech2Text-1.0.1/BanglaSpeech2Text.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 15:49:22.000000 BanglaSpeech2Text-1.0.1/BanglaSpeech2Text.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-08-07 15:49:22.000000 BanglaSpeech2Text-1.0.1/BanglaSpeech2Text.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-08-07 15:49:22.000000 BanglaSpeech2Text-1.0.1/BanglaSpeech2Text.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       89 2023-08-07 15:49:22.000000 BanglaSpeech2Text-1.0.1/BanglaSpeech2Text.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-08-07 15:49:22.000000 BanglaSpeech2Text-1.0.1/BanglaSpeech2Text.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    11558 2023-08-07 07:49:10.000000 BanglaSpeech2Text-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0       32 2023-08-07 07:49:10.000000 BanglaSpeech2Text-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     7574 2023-08-07 15:49:24.523382 BanglaSpeech2Text-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5981 2023-08-07 15:45:00.000000 BanglaSpeech2Text-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-08-07 15:49:24.495381 BanglaSpeech2Text-1.0.1/banglaspeech2text/
+-rw-rw-rw-   0        0        0       53 2023-08-07 07:49:10.000000 BanglaSpeech2Text-1.0.1/banglaspeech2text/__init__.py
+-rw-rw-rw-   0        0        0     3610 2023-08-07 15:38:48.000000 BanglaSpeech2Text-1.0.1/banglaspeech2text/cli.py
+-rw-rw-rw-   0        0        0    19452 2023-08-07 15:04:13.000000 BanglaSpeech2Text-1.0.1/banglaspeech2text/speech2text.py
+drwxrwxrwx   0        0        0        0 2023-08-07 15:49:24.520381 BanglaSpeech2Text-1.0.1/banglaspeech2text/utils/
+-rw-rw-rw-   0        0        0      213 2023-08-07 13:03:05.000000 BanglaSpeech2Text-1.0.1/banglaspeech2text/utils/__init__.py
+-rw-rw-rw-   0        0        0     1271 2023-08-07 12:51:29.000000 BanglaSpeech2Text-1.0.1/banglaspeech2text/utils/helpers.py
+-rw-rw-rw-   0        0        0     1123 2023-08-07 07:49:10.000000 BanglaSpeech2Text-1.0.1/banglaspeech2text/utils/listed_models.json
+-rw-rw-rw-   0        0        0     1421 2023-08-07 07:49:10.000000 BanglaSpeech2Text-1.0.1/banglaspeech2text/utils/models.py
+-rw-rw-rw-   0        0        0     1123 2023-08-07 07:49:10.000000 BanglaSpeech2Text-1.0.1/listed_models.json
+-rw-rw-rw-   0        0        0       42 2023-08-07 15:49:24.525382 BanglaSpeech2Text-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     2246 2023-08-07 15:21:45.000000 BanglaSpeech2Text-1.0.1/setup.py
```

### Comparing `BanglaSpeech2Text-0.0.9/BanglaSpeech2Text.egg-info/SOURCES.txt` & `BanglaSpeech2Text-1.0.1/BanglaSpeech2Text.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 LICENSE
 MANIFEST.in
 README.md
+listed_models.json
 setup.py
 BanglaSpeech2Text.egg-info/PKG-INFO
 BanglaSpeech2Text.egg-info/SOURCES.txt
 BanglaSpeech2Text.egg-info/dependency_links.txt
+BanglaSpeech2Text.egg-info/entry_points.txt
 BanglaSpeech2Text.egg-info/not-zip-safe
 BanglaSpeech2Text.egg-info/requires.txt
 BanglaSpeech2Text.egg-info/top_level.txt
 banglaspeech2text/__init__.py
+banglaspeech2text/cli.py
 banglaspeech2text/speech2text.py
 banglaspeech2text/utils/__init__.py
-banglaspeech2text/utils/download_models.py
-banglaspeech2text/utils/download_path.py
-banglaspeech2text/utils/extras.py
-banglaspeech2text/utils/install_packages.py
+banglaspeech2text/utils/helpers.py
+banglaspeech2text/utils/listed_models.json
+banglaspeech2text/utils/models.py
```

### Comparing `BanglaSpeech2Text-0.0.9/setup.py` & `BanglaSpeech2Text-1.0.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from setuptools import setup, find_packages
 
-version = '0.0.9'
-description = 'An open-source offline speech-to-text package for Bangla language. Fine-tuned on the latest whisper speech to text model for optimal performance.'
+version = '1.0.1'
+description = 'An open-source offline speech-to-text package for Bangla language.'
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 name = 'BanglaSpeech2Text'
-author = 'Sifat (shhossain)'
-email = '<hossain@gmail.com>'
+author = 'sifat (shhossain)'
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
-keywords = ['python','speech to text','voice to text','bangla speech to text', 'bangla speech recognation', 'whisper model', 'bangla asr model', 'offline speech to text', 'offline bangla speech to text', 'offline bangla voice recognation']
+keywords = ['python','speech to text','voice to text','bangla speech to text', 'bangla speech recognation', 'whisper model', 'bangla asr model', 'offline speech to text', 'offline bangla speech to text', 'offline bangla voice recognation', 'voice recognation']
 
 classifiers = [
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
     'Intended Audience :: Education',
     'Intended Audience :: Science/Research',
     'License :: OSI Approved :: MIT License',
@@ -36,25 +35,31 @@
 
 projects_links = {
     "Documentation": "https://github.com/shhossain/BanglaSpeech2Text",
     "Source": "https://github.com/shhossain/BanglaSpeech2Text",
     "Bug Tracker": "https://github.com/shhossain/BanglaSpeech2Text/issues",
 }
 
+
+
 setup(
     name=name,
     version=version,
     description=description,
     long_description=long_description,
     long_description_content_type='text/markdown',
     author=author,
-    author_email=email,
     url="https://github.com/shhossain/BanglaSpeech2Text",
     project_urls=projects_links,
     packages=find_packages(),
     install_requires=required,
     keywords=keywords,
     classifiers=classifiers,
     python_requires='>=3.6',
     include_package_data=True,
     zip_safe=False,
+    entry_points={
+        'console_scripts': [
+            'bnstt = banglaspeech2text.cli:main',
+        ],
+    },
 )
```

