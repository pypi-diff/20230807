# Comparing `tmp/nts-everdrone-1.1.9.tar.gz` & `tmp/nts-everdrone-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nts-everdrone-1.1.9.tar", last modified: Mon Sep 20 07:51:56 2021, max compression
+gzip compressed data, was "nts-everdrone-1.2.0.tar", last modified: Mon Aug  7 09:56:23 2023, max compression
```

## Comparing `nts-everdrone-1.1.9.tar` & `nts-everdrone-1.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-20 07:51:55.999416 nts-everdrone-1.1.9/
--rw-r--r--   0 runner    (1001) docker     (121)      140 2021-09-20 07:51:42.000000 nts-everdrone-1.1.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1787 2021-09-20 07:51:55.999416 nts-everdrone-1.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1073 2021-09-20 07:51:42.000000 nts-everdrone-1.1.9/license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-20 07:51:55.999416 nts-everdrone-1.1.9/nts/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-20 07:51:42.000000 nts-everdrone-1.1.9/nts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       61 2021-09-20 07:51:42.000000 nts-everdrone-1.1.9/nts/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2542 2021-09-20 07:51:42.000000 nts-everdrone-1.1.9/nts/cli.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    10810 2021-09-20 07:51:42.000000 nts-everdrone-1.1.9/nts/downloader.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-20 07:51:55.999416 nts-everdrone-1.1.9/nts_everdrone.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1787 2021-09-20 07:51:55.000000 nts-everdrone-1.1.9/nts_everdrone.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      323 2021-09-20 07:51:55.000000 nts-everdrone-1.1.9/nts_everdrone.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-20 07:51:55.000000 nts-everdrone-1.1.9/nts_everdrone.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-09-20 07:51:55.000000 nts-everdrone-1.1.9/nts_everdrone.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       76 2021-09-20 07:51:55.000000 nts-everdrone-1.1.9/nts_everdrone.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        4 2021-09-20 07:51:55.000000 nts-everdrone-1.1.9/nts_everdrone.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1341 2021-09-20 07:51:42.000000 nts-everdrone-1.1.9/readme.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-09-20 07:51:55.999416 nts-everdrone-1.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      832 2021-09-20 07:51:42.000000 nts-everdrone-1.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:56:23.099155 nts-everdrone-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-08-07 09:56:10.000000 nts-everdrone-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-08-07 09:56:23.099155 nts-everdrone-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-08-07 09:56:10.000000 nts-everdrone-1.2.0/license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:56:23.099155 nts-everdrone-1.2.0/nts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 09:56:10.000000 nts-everdrone-1.2.0/nts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-07 09:56:10.000000 nts-everdrone-1.2.0/nts/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-08-07 09:56:10.000000 nts-everdrone-1.2.0/nts/cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11401 2023-08-07 09:56:10.000000 nts-everdrone-1.2.0/nts/downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:56:23.099155 nts-everdrone-1.2.0/nts_everdrone.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-08-07 09:56:23.000000 nts-everdrone-1.2.0/nts_everdrone.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-08-07 09:56:23.000000 nts-everdrone-1.2.0/nts_everdrone.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 09:56:23.000000 nts-everdrone-1.2.0/nts_everdrone.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-07 09:56:23.000000 nts-everdrone-1.2.0/nts_everdrone.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-08-07 09:56:23.000000 nts-everdrone-1.2.0/nts_everdrone.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-08-07 09:56:23.000000 nts-everdrone-1.2.0/nts_everdrone.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-08-07 09:56:10.000000 nts-everdrone-1.2.0/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 09:56:23.099155 nts-everdrone-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-08-07 09:56:10.000000 nts-everdrone-1.2.0/setup.py
```

### Comparing `nts-everdrone-1.1.9/PKG-INFO` & `nts-everdrone-1.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: nts-everdrone
-Version: 1.1.9
+Version: 1.2.0
 Summary: NTS Radio downloader tool
 Home-page: https://github.com/everdrone/nts
 Author: Giorgio Tropiano
 Author-email: giorgiotropiano@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7.5
 Description-Content-Type: text/markdown
 
 # NTS Radio downloader
@@ -67,9 +66,7 @@
 ```
 
 To change the output directory use the `--out-dir` option, or the `-o` shorthand
 
 ```sh
 nts -o ~/Desktop/NTS links.txt
 ```
-
-
```

### Comparing `nts-everdrone-1.1.9/license` & `nts-everdrone-1.2.0/license`

 * *Files identical despite different names*

### Comparing `nts-everdrone-1.1.9/nts/cli.py` & `nts-everdrone-1.2.0/nts/cli.py`

 * *Files identical despite different names*

### Comparing `nts-everdrone-1.1.9/nts/downloader.py` & `nts-everdrone-1.2.0/nts/downloader.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,22 +4,23 @@
 import sys
 import urllib
 import json
 
 import mutagen
 import requests
 import youtube_dl
+from cssutils import parseStyle
 from bs4 import BeautifulSoup
 
 from mutagen.easyid3 import EasyID3
 from mutagen.id3 import ID3, APIC, COMM
 from mutagen.mp4 import MP4
 
 
-__version__ = '1.1.9'
+__version__ = '1.2.0'
 
 
 # defaults to darwin
 download_dir = '~/Downloads'
 if sys.platform.startswith('win32'):
     download_dir = '%USERPROFILE\\Downloads\\'
 # expand it
@@ -34,29 +35,46 @@
     # guessing there is one
     parsed = parse_nts_data(bs)
     parsed['url'] = nts_url
     # safe_title, date, title, artists, parsed_artists, genres, image_url = parse_nts_data(bs)
 
     button = bs.select('.episode__btn.mixcloud-btn')[0]
     link = button.get('data-src')
-    match = re.match(r'https:\/\/www.mixcloud\.com\/NTSRadio.+$', link)
+    host = None
+
+    if 'https://mixcloud' in link:
+        host = 'mixcloud'
+    elif 'https://soundcloud' in link:
+        host = 'soundcloud'
 
     # get album art. If the one on mixcloud is available, use it. Otherwise,
     # fall back to the nts website.
     page = requests.get(link).content
     bs = BeautifulSoup(page, 'html.parser')
     image_type = ''
-    if len(bs.select('div.album-art')) != 0:
+    image = None
+
+    if host == 'mixcloud' and len(bs.select('div.album-art')) != 0:
         img = bs.select('div.album-art')[0].img
         srcset = img.get('srcset').split()
         img = srcset[-2].split(',')[1]
         image = urllib.request.urlopen(img)
         image_type = image.info().get_content_type()
         image = image.read()
-    elif len(parsed["image_url"]):
+    elif host == 'soundcloud' and len(bs.select('span.image__full')) != 0:
+        style = parseStyle(bs.select('.image__full')[0].get('style'))
+        image = urllib.request.urlopen(style['background-image'])
+        image_type = image.info().get_content_type()
+        image = image.read()
+
+    if image is None and len(parsed['image_url']) > 0:
+        if '/resize/' in parsed['image_url']:
+            # use a bigger image
+            parsed['image_url'] = re.sub(
+                r'/resize/\d+x\d+/', '/resize/1000x1000/', parsed['image_url'])
         image = urllib.request.urlopen(parsed["image_url"])
         image_type = image.info().get_content_type()
         image = image.read()
 
     file_name = f'{parsed["safe_title"]} - {parsed["date"].year}-{parsed["date"].month}-{parsed["date"].day}'
 
     # download
@@ -107,18 +125,16 @@
     station = title_box.div.div.h2.find(text=True, recursive=False)
     if not station:
         station = 'London'
     else:
         station = station.strip()
 
     # bg_tag = bs.select('section#bg[style]')
-    bg_tag = bs.select('section.background-image.visible-desktop[style]')
-    background_image_regex = r'background-image:url\((.*)\)'
-    image_url = re.match(background_image_regex,
-                         bg_tag[0]['style']).groups()[0]
+    bg_tag = bs.select('img.visible-desktop')[0]
+    image_url = bg_tag.get('src') if bg_tag else ''
 
     # sometimes it's just the date
     date = title_box.div.div.h2.span.text
     if ',' in date:
         date = date.split(',')[1].strip()
     else:
         date = date.strip()
@@ -304,21 +320,24 @@
     # add first genre
     if len(parsed['genres']) != 0:
         audio['genre'] = parsed['genres'][0]
     audio.save()
 
     # add cover
     audio = ID3(file_path)
-    audio.delall('APIC')
+    if audio.getall('APIC'):
+        audio.delall('APIC')
     if image_type != '':
-        audio['APIC'] = APIC(
-            encoding=3,
-            mime=image_type,
-            type=3, desc=u'Cover',
-            data=image
+        audio.add(
+            APIC(
+                encoding=3,
+                mime=image_type,
+                type=3, desc=u'Cover',
+                data=image
+            )
         )
 
     # add comment
     audio.delall('COMM')
     audio['COMM'] = COMM(encoding=0, lang='eng',
                          desc=u'', text=[parsed['url']])
     audio.save()
```

### Comparing `nts-everdrone-1.1.9/nts_everdrone.egg-info/PKG-INFO` & `nts-everdrone-1.2.0/nts_everdrone.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: nts-everdrone
-Version: 1.1.9
+Version: 1.2.0
 Summary: NTS Radio downloader tool
 Home-page: https://github.com/everdrone/nts
 Author: Giorgio Tropiano
 Author-email: giorgiotropiano@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7.5
 Description-Content-Type: text/markdown
 
 # NTS Radio downloader
@@ -67,9 +66,7 @@
 ```
 
 To change the output directory use the `--out-dir` option, or the `-o` shorthand
 
 ```sh
 nts -o ~/Desktop/NTS links.txt
 ```
-
-
```

### Comparing `nts-everdrone-1.1.9/readme.md` & `nts-everdrone-1.2.0/readme.md`

 * *Files identical despite different names*

### Comparing `nts-everdrone-1.1.9/setup.py` & `nts-everdrone-1.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="nts-everdrone",
-    version="1.1.9",
+    version="1.2.0",
     author="Giorgio Tropiano",
     author_email="giorgiotropiano@gmail.com",
     description="NTS Radio downloader tool",
     long_description=open('readme.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/everdrone/nts",
     packages=setuptools.find_packages(),
@@ -19,11 +19,12 @@
     entry_points={
         'console_scripts': ['nts=nts.cli:main']
     },
     install_requires=[
         'youtube-dl==2021.6.6',
         'beautifulsoup4==4.9.3',
         'mutagen==1.45.1',
-        'requests==2.26.0'
+        'requests==2.26.0',
+        'cssutils==2.7.1',
     ],
     python_requires='>=3.7.5',
 )
```

