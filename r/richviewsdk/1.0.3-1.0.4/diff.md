# Comparing `tmp/richviewsdk-1.0.3.tar.gz` & `tmp/richviewsdk-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "richviewsdk-1.0.3.tar", last modified: Sun Aug  6 21:04:02 2023, max compression
+gzip compressed data, was "richviewsdk-1.0.4.tar", last modified: Sun Aug  6 21:20:18 2023, max compression
```

## Comparing `richviewsdk-1.0.3.tar` & `richviewsdk-1.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-08-06 21:04:02.962237 richviewsdk-1.0.3/
--rw-rw-rw-   0        0        0       55 2023-08-06 20:35:29.000000 richviewsdk-1.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2776 2023-08-06 21:04:02.960239 richviewsdk-1.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-06 21:04:02.922232 richviewsdk-1.0.3/richviewsdk/
--rw-rw-rw-   0        0        0    33218 2023-08-06 20:06:17.000000 richviewsdk-1.0.3/richviewsdk/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-06 21:04:02.956246 richviewsdk-1.0.3/richviewsdk.egg-info/
--rw-rw-rw-   0        0        0     2776 2023-08-06 21:04:02.000000 richviewsdk-1.0.3/richviewsdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2023-08-06 21:04:02.000000 richviewsdk-1.0.3/richviewsdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-06 21:04:02.000000 richviewsdk-1.0.3/richviewsdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-08-06 21:04:02.000000 richviewsdk-1.0.3/richviewsdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-08-06 21:04:02.000000 richviewsdk-1.0.3/richviewsdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-06 21:04:02.962237 richviewsdk-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      560 2023-08-06 21:03:25.000000 richviewsdk-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-06 21:20:18.331759 richviewsdk-1.0.4/
+-rw-rw-rw-   0        0        0       55 2023-08-06 20:35:29.000000 richviewsdk-1.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     2776 2023-08-06 21:20:18.329761 richviewsdk-1.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-06 21:20:18.290210 richviewsdk-1.0.4/richviewsdk/
+-rw-rw-rw-   0        0        0    33298 2023-08-06 21:16:17.000000 richviewsdk-1.0.4/richviewsdk/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-06 21:20:18.325225 richviewsdk-1.0.4/richviewsdk.egg-info/
+-rw-rw-rw-   0        0        0     2776 2023-08-06 21:20:18.000000 richviewsdk-1.0.4/richviewsdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2023-08-06 21:20:18.000000 richviewsdk-1.0.4/richviewsdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-06 21:20:18.000000 richviewsdk-1.0.4/richviewsdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-08-06 21:20:18.000000 richviewsdk-1.0.4/richviewsdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-08-06 21:20:18.000000 richviewsdk-1.0.4/richviewsdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-06 21:20:18.331759 richviewsdk-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      560 2023-08-06 21:19:54.000000 richviewsdk-1.0.4/setup.py
```

### Comparing `richviewsdk-1.0.3/PKG-INFO` & `richviewsdk-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: richviewsdk
-Version: 1.0.3
+Version: 1.0.4
 Summary: Package to interact with RichView API.
 Home-page: https://therichview.com/
 Author: Daniel Vecera
 Author-email: daniel@therichview.com
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `richviewsdk-1.0.3/richviewsdk/__init__.py` & `richviewsdk-1.0.4/richviewsdk/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -568,14 +568,15 @@
         withHeadings : bool
             A flag indicating whether the table block has headings
         session : RichViewSession
             The session the table block belongs to
         id : str, optional
             The ID of the table block (default is None)
         """
+        data = self.TableBlockData(content=content, withHeadings=withHeadings)
         super().__init__(report_id=report_id, id=id, type='table', data=data, session=session)
 
     def __repr__(self):
         return f"TableBlock(id={self.block_id})"
 
 
 class CodeBlock(RichViewBlock):
```

### Comparing `richviewsdk-1.0.3/richviewsdk.egg-info/PKG-INFO` & `richviewsdk-1.0.4/richviewsdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: richviewsdk
-Version: 1.0.3
+Version: 1.0.4
 Summary: Package to interact with RichView API.
 Home-page: https://therichview.com/
 Author: Daniel Vecera
 Author-email: daniel@therichview.com
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `richviewsdk-1.0.3/setup.py` & `richviewsdk-1.0.4/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 
 from setuptools import setup, find_packages
 
 setup(
     name='richviewsdk',
-    version='1.0.3',
+    version='1.0.4',
     packages=find_packages(),
     url='https://therichview.com/',
     author='Daniel Vecera',
     author_email='daniel@therichview.com',
     description='Package to interact with RichView API.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

