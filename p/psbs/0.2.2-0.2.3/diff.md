# Comparing `tmp/psbs-0.2.2.tar.gz` & `tmp/psbs-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psbs-0.2.2.tar", last modified: Sun Aug  6 15:07:41 2023, max compression
+gzip compressed data, was "psbs-0.2.3.tar", last modified: Mon Aug  7 15:17:45 2023, max compression
```

## Comparing `psbs-0.2.2.tar` & `psbs-0.2.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 jcmiller   (501) staff       (20)        0 2023-08-06 15:07:41.699320 psbs-0.2.2/
--rw-r--r--   0 jcmiller   (501) staff       (20)     1069 2023-06-04 01:40:38.000000 psbs-0.2.2/LICENSE
--rw-r--r--   0 jcmiller   (501) staff       (20)     6737 2023-08-06 15:07:41.699504 psbs-0.2.2/PKG-INFO
--rw-r--r--   0 jcmiller   (501) staff       (20)     6065 2023-08-04 20:30:44.000000 psbs-0.2.2/README.md
-drwxr-xr-x   0 jcmiller   (501) staff       (20)        0 2023-08-06 15:07:41.693590 psbs-0.2.2/psbs/
--rw-r--r--   0 jcmiller   (501) staff       (20)        0 2023-06-05 12:31:00.000000 psbs-0.2.2/psbs/__init__.py
--rw-r--r--   0 jcmiller   (501) staff       (20)       32 2023-06-11 15:36:36.000000 psbs-0.2.2/psbs/__main__.py
--rw-r--r--   0 jcmiller   (501) staff       (20)      383 2023-07-23 20:27:08.000000 psbs-0.2.2/psbs/config.py
--rw-r--r--   0 jcmiller   (501) staff       (20)      870 2023-07-29 00:01:45.000000 psbs-0.2.2/psbs/example.txt
--rw-r--r--   0 jcmiller   (501) staff       (20)     1614 2023-08-04 01:50:46.000000 psbs-0.2.2/psbs/extension.py
-drwxr-xr-x   0 jcmiller   (501) staff       (20)        0 2023-08-06 15:07:41.698894 psbs-0.2.2/psbs/extensions/
--rw-r--r--   0 jcmiller   (501) staff       (20)        0 2023-06-18 20:00:51.000000 psbs-0.2.2/psbs/extensions/__init__.py
--rw-r--r--   0 jcmiller   (501) staff       (20)      568 2023-08-04 01:50:46.000000 psbs-0.2.2/psbs/extensions/build.py
--rw-r--r--   0 jcmiller   (501) staff       (20)      451 2023-08-06 12:49:36.000000 psbs-0.2.2/psbs/extensions/filters.py
--rw-r--r--   0 jcmiller   (501) staff       (20)     3069 2023-08-04 01:50:46.000000 psbs-0.2.2/psbs/extensions/images.py
--rw-r--r--   0 jcmiller   (501) staff       (20)    20733 2023-08-04 01:50:46.000000 psbs-0.2.2/psbs/extensions/tiled.py
--rw-r--r--   0 jcmiller   (501) staff       (20)     2916 2023-08-04 18:52:17.000000 psbs-0.2.2/psbs/gister.py
--rw-r--r--   0 jcmiller   (501) staff       (20)     1820 2023-08-06 15:04:23.000000 psbs-0.2.2/psbs/htmlbuilder.py
--rwxr-xr-x   0 jcmiller   (501) staff       (20)     4301 2023-08-06 14:09:41.000000 psbs-0.2.2/psbs/project.py
--rwxr-xr-x   0 jcmiller   (501) staff       (20)     2944 2023-08-06 14:10:04.000000 psbs-0.2.2/psbs/psbs.py
--rw-r--r--   0 jcmiller   (501) staff       (20)     9382 2023-08-06 15:00:57.000000 psbs-0.2.2/psbs/psparser.py
--rw-r--r--   0 jcmiller   (501) staff       (20)     3044 2023-08-04 01:50:46.000000 psbs-0.2.2/psbs/template.py
--rw-r--r--   0 jcmiller   (501) staff       (20)     1118 2023-08-04 23:04:04.000000 psbs-0.2.2/psbs/token.py
--rw-r--r--   0 jcmiller   (501) staff       (20)     1945 2023-06-14 18:47:43.000000 psbs-0.2.2/psbs/utils.py
-drwxr-xr-x   0 jcmiller   (501) staff       (20)        0 2023-08-06 15:07:41.696649 psbs-0.2.2/psbs.egg-info/
--rw-r--r--   0 jcmiller   (501) staff       (20)     6737 2023-08-06 15:07:41.000000 psbs-0.2.2/psbs.egg-info/PKG-INFO
--rw-r--r--   0 jcmiller   (501) staff       (20)      547 2023-08-06 15:07:41.000000 psbs-0.2.2/psbs.egg-info/SOURCES.txt
--rw-r--r--   0 jcmiller   (501) staff       (20)        1 2023-08-06 15:07:41.000000 psbs-0.2.2/psbs.egg-info/dependency_links.txt
--rw-r--r--   0 jcmiller   (501) staff       (20)       40 2023-08-06 15:07:41.000000 psbs-0.2.2/psbs.egg-info/entry_points.txt
--rw-r--r--   0 jcmiller   (501) staff       (20)       49 2023-08-06 15:07:41.000000 psbs-0.2.2/psbs.egg-info/requires.txt
--rw-r--r--   0 jcmiller   (501) staff       (20)        5 2023-08-06 15:07:41.000000 psbs-0.2.2/psbs.egg-info/top_level.txt
--rw-r--r--   0 jcmiller   (501) staff       (20)      103 2023-08-06 15:07:41.700371 psbs-0.2.2/setup.cfg
--rw-r--r--   0 jcmiller   (501) staff       (20)     1277 2023-08-06 15:04:41.000000 psbs-0.2.2/setup.py
+drwxr-xr-x   0 jcmiller   (501) staff       (20)        0 2023-08-07 15:17:45.232893 psbs-0.2.3/
+-rw-r--r--   0 jcmiller   (501) staff       (20)     1069 2023-06-04 01:40:38.000000 psbs-0.2.3/LICENSE
+-rw-r--r--   0 jcmiller   (501) staff       (20)     6737 2023-08-07 15:17:45.233142 psbs-0.2.3/PKG-INFO
+-rw-r--r--   0 jcmiller   (501) staff       (20)     6065 2023-08-04 20:30:44.000000 psbs-0.2.3/README.md
+drwxr-xr-x   0 jcmiller   (501) staff       (20)        0 2023-08-07 15:17:45.225998 psbs-0.2.3/psbs/
+-rw-r--r--   0 jcmiller   (501) staff       (20)        0 2023-06-05 12:31:00.000000 psbs-0.2.3/psbs/__init__.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)       32 2023-06-11 15:36:36.000000 psbs-0.2.3/psbs/__main__.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)      383 2023-07-23 20:27:08.000000 psbs-0.2.3/psbs/config.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)      870 2023-07-29 00:01:45.000000 psbs-0.2.3/psbs/example.txt
+-rw-r--r--   0 jcmiller   (501) staff       (20)     1614 2023-08-04 01:50:46.000000 psbs-0.2.3/psbs/extension.py
+drwxr-xr-x   0 jcmiller   (501) staff       (20)        0 2023-08-07 15:17:45.231926 psbs-0.2.3/psbs/extensions/
+-rw-r--r--   0 jcmiller   (501) staff       (20)        0 2023-06-18 20:00:51.000000 psbs-0.2.3/psbs/extensions/__init__.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)      568 2023-08-04 01:50:46.000000 psbs-0.2.3/psbs/extensions/build.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)     1399 2023-08-07 15:09:24.000000 psbs-0.2.3/psbs/extensions/filters.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)     3069 2023-08-04 01:50:46.000000 psbs-0.2.3/psbs/extensions/images.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)    20733 2023-08-04 01:50:46.000000 psbs-0.2.3/psbs/extensions/tiled.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)     2916 2023-08-04 18:52:17.000000 psbs-0.2.3/psbs/gister.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)     1820 2023-08-06 15:04:23.000000 psbs-0.2.3/psbs/htmlbuilder.py
+-rwxr-xr-x   0 jcmiller   (501) staff       (20)     4301 2023-08-06 14:09:41.000000 psbs-0.2.3/psbs/project.py
+-rwxr-xr-x   0 jcmiller   (501) staff       (20)     2944 2023-08-06 14:10:04.000000 psbs-0.2.3/psbs/psbs.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)     9382 2023-08-06 15:00:57.000000 psbs-0.2.3/psbs/psparser.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)     3086 2023-08-07 15:12:48.000000 psbs-0.2.3/psbs/template.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)     1118 2023-08-04 23:04:04.000000 psbs-0.2.3/psbs/token.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)     1945 2023-06-14 18:47:43.000000 psbs-0.2.3/psbs/utils.py
+drwxr-xr-x   0 jcmiller   (501) staff       (20)        0 2023-08-07 15:17:45.229307 psbs-0.2.3/psbs.egg-info/
+-rw-r--r--   0 jcmiller   (501) staff       (20)     6737 2023-08-07 15:17:45.000000 psbs-0.2.3/psbs.egg-info/PKG-INFO
+-rw-r--r--   0 jcmiller   (501) staff       (20)      547 2023-08-07 15:17:45.000000 psbs-0.2.3/psbs.egg-info/SOURCES.txt
+-rw-r--r--   0 jcmiller   (501) staff       (20)        1 2023-08-07 15:17:45.000000 psbs-0.2.3/psbs.egg-info/dependency_links.txt
+-rw-r--r--   0 jcmiller   (501) staff       (20)       40 2023-08-07 15:17:45.000000 psbs-0.2.3/psbs.egg-info/entry_points.txt
+-rw-r--r--   0 jcmiller   (501) staff       (20)       49 2023-08-07 15:17:45.000000 psbs-0.2.3/psbs.egg-info/requires.txt
+-rw-r--r--   0 jcmiller   (501) staff       (20)        5 2023-08-07 15:17:45.000000 psbs-0.2.3/psbs.egg-info/top_level.txt
+-rw-r--r--   0 jcmiller   (501) staff       (20)      103 2023-08-07 15:17:45.233859 psbs-0.2.3/setup.cfg
+-rw-r--r--   0 jcmiller   (501) staff       (20)     1277 2023-08-07 15:15:53.000000 psbs-0.2.3/setup.py
```

### Comparing `psbs-0.2.2/LICENSE` & `psbs-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `psbs-0.2.2/PKG-INFO` & `psbs-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: psbs
-Version: 0.2.2
+Version: 0.2.3
 Summary: PuzzleScript Build System
 Home-page: https://github.com/jcmiller11/PSBS
-Download-URL: https://github.com/jcmiller11/PSBS/archive/refs/tags/0.2.2.tar.gz
+Download-URL: https://github.com/jcmiller11/PSBS/archive/refs/tags/0.2.3.tar.gz
 Author: J.C. Miller
 Author-email: johncoreymiller@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `psbs-0.2.2/README.md` & `psbs-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `psbs-0.2.2/psbs/example.txt` & `psbs-0.2.3/psbs/example.txt`

 * *Files identical despite different names*

### Comparing `psbs-0.2.2/psbs/extension.py` & `psbs-0.2.3/psbs/extension.py`

 * *Files identical despite different names*

### Comparing `psbs-0.2.2/psbs/extensions/build.py` & `psbs-0.2.3/psbs/extensions/build.py`

 * *Files identical despite different names*

### Comparing `psbs-0.2.2/psbs/extensions/images.py` & `psbs-0.2.3/psbs/extensions/images.py`

 * *Files identical despite different names*

### Comparing `psbs-0.2.2/psbs/extensions/tiled.py` & `psbs-0.2.3/psbs/extensions/tiled.py`

 * *Files identical despite different names*

### Comparing `psbs-0.2.2/psbs/gister.py` & `psbs-0.2.3/psbs/gister.py`

 * *Files identical despite different names*

### Comparing `psbs-0.2.2/psbs/htmlbuilder.py` & `psbs-0.2.3/psbs/htmlbuilder.py`

 * *Files identical despite different names*

### Comparing `psbs-0.2.2/psbs/project.py` & `psbs-0.2.3/psbs/project.py`

 * *Files identical despite different names*

### Comparing `psbs-0.2.2/psbs/psbs.py` & `psbs-0.2.3/psbs/psbs.py`

 * *Files identical despite different names*

### Comparing `psbs-0.2.2/psbs/psparser.py` & `psbs-0.2.3/psbs/psparser.py`

 * *Files identical despite different names*

### Comparing `psbs-0.2.2/psbs/template.py` & `psbs-0.2.3/psbs/template.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
             autoescape=False,
             block_start_string="(%",
             block_end_string="%)",
             variable_start_string="((",
             variable_end_string="))",
             comment_start_string="(#",
             comment_end_string="#)",
+            extensions=['jinja2.ext.do'],
         )
         self.postprocessing_steps = []
         extensions = Extension.get_extensions()
         for extension in extensions:
             if extension.__name__ not in config:
                 config[extension.__name__] = {}
             ext_object = extension(config[extension.__name__])
```

### Comparing `psbs-0.2.2/psbs/token.py` & `psbs-0.2.3/psbs/token.py`

 * *Files identical despite different names*

### Comparing `psbs-0.2.2/psbs/utils.py` & `psbs-0.2.3/psbs/utils.py`

 * *Files identical despite different names*

### Comparing `psbs-0.2.2/psbs.egg-info/PKG-INFO` & `psbs-0.2.3/psbs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: psbs
-Version: 0.2.2
+Version: 0.2.3
 Summary: PuzzleScript Build System
 Home-page: https://github.com/jcmiller11/PSBS
-Download-URL: https://github.com/jcmiller11/PSBS/archive/refs/tags/0.2.2.tar.gz
+Download-URL: https://github.com/jcmiller11/PSBS/archive/refs/tags/0.2.3.tar.gz
 Author: J.C. Miller
 Author-email: johncoreymiller@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `psbs-0.2.2/psbs.egg-info/SOURCES.txt` & `psbs-0.2.3/psbs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `psbs-0.2.2/setup.py` & `psbs-0.2.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='psbs',
-    version='0.2.2',
+    version='0.2.3',
     python_requires='>=3.8',
     description='PuzzleScript Build System',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='J.C. Miller',
     author_email='johncoreymiller@gmail.com',
     url='https://github.com/jcmiller11/PSBS',
-    download_url = 'https://github.com/jcmiller11/PSBS/archive/refs/tags/0.2.2.tar.gz',
+    download_url = 'https://github.com/jcmiller11/PSBS/archive/refs/tags/0.2.3.tar.gz',
     license='MIT',
     packages=find_packages(),
     package_data={'': ['example.txt']},
     include_package_data=True,
     install_requires=[
         'jinja2',
         'pyyaml',
```

