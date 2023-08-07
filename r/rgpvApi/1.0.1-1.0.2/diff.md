# Comparing `tmp/rgpvApi-1.0.1.tar.gz` & `tmp/rgpvApi-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rgpvApi-1.0.1.tar", last modified: Sun Aug  6 10:17:27 2023, max compression
+gzip compressed data, was "rgpvApi-1.0.2.tar", last modified: Mon Aug  7 12:04:27 2023, max compression
```

## Comparing `rgpvApi-1.0.1.tar` & `rgpvApi-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 cro        (501) staff       (20)        0 2023-08-06 10:17:27.176677 rgpvApi-1.0.1/
--rw-r--r--   0 cro        (501) staff       (20)    35148 2023-07-26 12:21:56.000000 rgpvApi-1.0.1/LICENSE.txt
--rw-r--r--   0 cro        (501) staff       (20)      967 2023-08-06 10:17:27.176565 rgpvApi-1.0.1/PKG-INFO
--rw-r--r--   0 cro        (501) staff       (20)      412 2023-08-06 10:12:57.000000 rgpvApi-1.0.1/README.md
-drwxr-xr-x   0 cro        (501) staff       (20)        0 2023-08-06 10:17:27.175551 rgpvApi-1.0.1/rgpvApi/
--rw-r--r--   0 cro        (501) staff       (20)       57 2023-08-06 10:08:49.000000 rgpvApi-1.0.1/rgpvApi/__init__.py
--rw-r--r--   0 cro        (501) staff       (20)    21615 2023-07-31 12:43:39.000000 rgpvApi-1.0.1/rgpvApi/info_api.py
--rw-r--r--   0 cro        (501) staff       (20)    14892 2023-07-31 13:36:59.000000 rgpvApi-1.0.1/rgpvApi/result_api.py
-drwxr-xr-x   0 cro        (501) staff       (20)        0 2023-08-06 10:17:27.176388 rgpvApi-1.0.1/rgpvApi.egg-info/
--rw-r--r--   0 cro        (501) staff       (20)      967 2023-08-06 10:17:27.000000 rgpvApi-1.0.1/rgpvApi.egg-info/PKG-INFO
--rw-r--r--   0 cro        (501) staff       (20)      246 2023-08-06 10:17:27.000000 rgpvApi-1.0.1/rgpvApi.egg-info/SOURCES.txt
--rw-r--r--   0 cro        (501) staff       (20)        1 2023-08-06 10:17:27.000000 rgpvApi-1.0.1/rgpvApi.egg-info/dependency_links.txt
--rw-r--r--   0 cro        (501) staff       (20)       49 2023-08-06 10:17:27.000000 rgpvApi-1.0.1/rgpvApi.egg-info/requires.txt
--rw-r--r--   0 cro        (501) staff       (20)        8 2023-08-06 10:17:27.000000 rgpvApi-1.0.1/rgpvApi.egg-info/top_level.txt
--rw-r--r--   0 cro        (501) staff       (20)       38 2023-08-06 10:17:27.176710 rgpvApi-1.0.1/setup.cfg
--rw-r--r--   0 cro        (501) staff       (20)      883 2023-08-06 10:16:44.000000 rgpvApi-1.0.1/setup.py
+drwxr-xr-x   0 cro        (501) staff       (20)        0 2023-08-07 12:04:27.117794 rgpvApi-1.0.2/
+-rw-r--r--   0 cro        (501) staff       (20)    35148 2023-07-26 12:21:56.000000 rgpvApi-1.0.2/LICENSE.txt
+-rw-r--r--   0 cro        (501) staff       (20)      967 2023-08-07 12:04:27.117621 rgpvApi-1.0.2/PKG-INFO
+-rw-r--r--   0 cro        (501) staff       (20)      412 2023-08-06 10:12:57.000000 rgpvApi-1.0.2/README.md
+drwxr-xr-x   0 cro        (501) staff       (20)        0 2023-08-07 12:04:27.116668 rgpvApi-1.0.2/rgpvApi/
+-rw-r--r--   0 cro        (501) staff       (20)       57 2023-08-06 10:08:49.000000 rgpvApi-1.0.2/rgpvApi/__init__.py
+-rw-r--r--   0 cro        (501) staff       (20)    21615 2023-07-31 12:43:39.000000 rgpvApi-1.0.2/rgpvApi/info_api.py
+-rw-r--r--   0 cro        (501) staff       (20)    14900 2023-08-07 11:56:30.000000 rgpvApi-1.0.2/rgpvApi/result_api.py
+drwxr-xr-x   0 cro        (501) staff       (20)        0 2023-08-07 12:04:27.117418 rgpvApi-1.0.2/rgpvApi.egg-info/
+-rw-r--r--   0 cro        (501) staff       (20)      967 2023-08-07 12:04:27.000000 rgpvApi-1.0.2/rgpvApi.egg-info/PKG-INFO
+-rw-r--r--   0 cro        (501) staff       (20)      246 2023-08-07 12:04:27.000000 rgpvApi-1.0.2/rgpvApi.egg-info/SOURCES.txt
+-rw-r--r--   0 cro        (501) staff       (20)        1 2023-08-07 12:04:27.000000 rgpvApi-1.0.2/rgpvApi.egg-info/dependency_links.txt
+-rw-r--r--   0 cro        (501) staff       (20)       49 2023-08-07 12:04:27.000000 rgpvApi-1.0.2/rgpvApi.egg-info/requires.txt
+-rw-r--r--   0 cro        (501) staff       (20)        8 2023-08-07 12:04:27.000000 rgpvApi-1.0.2/rgpvApi.egg-info/top_level.txt
+-rw-r--r--   0 cro        (501) staff       (20)       38 2023-08-07 12:04:27.117832 rgpvApi-1.0.2/setup.cfg
+-rw-r--r--   0 cro        (501) staff       (20)      883 2023-08-07 12:03:57.000000 rgpvApi-1.0.2/setup.py
```

### Comparing `rgpvApi-1.0.1/LICENSE.txt` & `rgpvApi-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rgpvApi-1.0.1/PKG-INFO` & `rgpvApi-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: rgpvApi
-Version: 1.0.1
+Version: 1.0.2
 Summary: RGPV API wrapper, written in Python.
 Home-page: https://github.com/cro2003/rgpvApi
 Author: cro2003
 Author-email: cro@chirag.software
 License: MIT
 Project-URL: Documnetation, https://cro2003.github.io/rgpvApi/
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
 
 # RGPV API
 RGPV API wrapper, written in Python.
```

### Comparing `rgpvApi-1.0.1/rgpvApi/info_api.py` & `rgpvApi-1.0.2/rgpvApi/info_api.py`

 * *Files identical despite different names*

### Comparing `rgpvApi-1.0.1/rgpvApi/result_api.py` & `rgpvApi-1.0.2/rgpvApi/result_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -212,12 +212,12 @@
     def __captchaSolver(self, link):
         response = self.ReqSession.get(link)
         img = Image.open(io.BytesIO(response.content))
         img = img.convert('L')
         img = ImageOps.invert(img)
         img = img.filter(ImageFilter.SHARPEN)
         text = pytesseract.image_to_string(img)
-        text = str(text).replace(' ', '').replace('\n', '').upper()
+        text = str(text).strip().replace(' ', '').replace('\n', '').upper()
         if len(text)!=5 and self.courseId!=11:
             self.__captchaSolver(link)
         else:
             return text
```

### Comparing `rgpvApi-1.0.1/rgpvApi.egg-info/PKG-INFO` & `rgpvApi-1.0.2/rgpvApi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: rgpvApi
-Version: 1.0.1
+Version: 1.0.2
 Summary: RGPV API wrapper, written in Python.
 Home-page: https://github.com/cro2003/rgpvApi
 Author: cro2003
 Author-email: cro@chirag.software
 License: MIT
 Project-URL: Documnetation, https://cro2003.github.io/rgpvApi/
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
 
 # RGPV API
 RGPV API wrapper, written in Python.
```

### Comparing `rgpvApi-1.0.1/setup.py` & `rgpvApi-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="rgpvApi",
-    version="1.0.1",
+    version="1.0.2",
     description="RGPV API wrapper, written in Python.",
     packages=['rgpvApi'],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/cro2003/rgpvApi",
     project_urls = {
     'Documnetation': 'https://cro2003.github.io/rgpvApi/',
@@ -22,9 +22,9 @@
         "Programming Language :: Python :: 3.11",
         "Operating System :: OS Independent",
     ],
     install_requires=["pytesseract", "requests", "beautifulsoup4"],
     extras_require = {
         "dev": ["twine"],
     },
-    python_requires=">=3.11",
+    python_requires=">=3.10",
 )
```

