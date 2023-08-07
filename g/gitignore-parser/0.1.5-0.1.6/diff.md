# Comparing `tmp/gitignore_parser-0.1.5.tar.gz` & `tmp/gitignore_parser-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitignore_parser-0.1.5.tar", last modified: Thu Aug  3 16:39:16 2023, max compression
+gzip compressed data, was "gitignore_parser-0.1.6.tar", last modified: Mon Aug  7 06:53:10 2023, max compression
```

## Comparing `gitignore_parser-0.1.5.tar` & `gitignore_parser-0.1.6.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-08-03 16:39:16.130197 gitignore_parser-0.1.5/
--rw-r--r--   0 michael   (1000) michael   (1000)     1058 2023-08-03 16:39:16.130197 gitignore_parser-0.1.5/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)     1404 2022-08-29 10:41:38.000000 gitignore_parser-0.1.5/README.md
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-08-03 16:39:16.130197 gitignore_parser-0.1.5/gitignore_parser.egg-info/
--rw-r--r--   0 michael   (1000) michael   (1000)     1058 2023-08-03 16:39:16.000000 gitignore_parser-0.1.5/gitignore_parser.egg-info/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)      247 2023-08-03 16:39:16.000000 gitignore_parser-0.1.5/gitignore_parser.egg-info/SOURCES.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-08-03 16:39:16.000000 gitignore_parser-0.1.5/gitignore_parser.egg-info/dependency_links.txt
--rw-r--r--   0 michael   (1000) michael   (1000)       35 2023-08-03 16:39:16.000000 gitignore_parser-0.1.5/gitignore_parser.egg-info/requires.txt
--rw-r--r--   0 michael   (1000) michael   (1000)       17 2023-08-03 16:39:16.000000 gitignore_parser-0.1.5/gitignore_parser.egg-info/top_level.txt
--rw-r--r--   0 michael   (1000) michael   (1000)     7409 2023-08-03 16:38:19.000000 gitignore_parser-0.1.5/gitignore_parser.py
--rw-r--r--   0 michael   (1000) michael   (1000)       79 2023-08-03 16:39:16.130197 gitignore_parser-0.1.5/setup.cfg
--rw-r--r--   0 michael   (1000) michael   (1000)     1332 2023-08-03 16:38:42.000000 gitignore_parser-0.1.5/setup.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-08-07 06:53:10.663365 gitignore_parser-0.1.6/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1125 2022-08-29 10:41:38.000000 gitignore_parser-0.1.6/LICENSE
+-rw-r--r--   0 michael   (1000) michael   (1000)     1254 2023-08-07 06:53:10.663365 gitignore_parser-0.1.6/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)     1404 2022-08-29 10:41:38.000000 gitignore_parser-0.1.6/README.md
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-08-07 06:53:10.663365 gitignore_parser-0.1.6/gitignore_parser.egg-info/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1254 2023-08-07 06:53:10.000000 gitignore_parser-0.1.6/gitignore_parser.egg-info/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)      231 2023-08-07 06:53:10.000000 gitignore_parser-0.1.6/gitignore_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-08-07 06:53:10.000000 gitignore_parser-0.1.6/gitignore_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)       17 2023-08-07 06:53:10.000000 gitignore_parser-0.1.6/gitignore_parser.egg-info/top_level.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)     7409 2023-08-03 16:38:19.000000 gitignore_parser-0.1.6/gitignore_parser.py
+-rw-r--r--   0 michael   (1000) michael   (1000)       81 2023-08-07 06:50:31.000000 gitignore_parser-0.1.6/pyproject.toml
+-rw-r--r--   0 michael   (1000) michael   (1000)       79 2023-08-07 06:53:10.663365 gitignore_parser-0.1.6/setup.cfg
+-rw-r--r--   0 michael   (1000) michael   (1000)     1460 2023-08-07 06:52:08.000000 gitignore_parser-0.1.6/setup.py
```

### Comparing `gitignore_parser-0.1.5/PKG-INFO` & `gitignore_parser-0.1.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,15 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: gitignore_parser
-Version: 0.1.5
+Version: 0.1.6
 Summary: A spec-compliant gitignore parser for Python 3.5+
 Home-page: https://github.com/mherrmann/gitignore_parser
 Author: Michael Herrmann
 Author-email: michael+removethisifyouarehuman@herrmann.io
 License: MIT
-Description: A spec-compliant gitignore parser for Python 3.5+
-        
-        https://github.com/mherrmann/gitignore_parser
 Keywords: gitignore
 Platform: MacOS
 Platform: Windows
 Platform: Debian
 Platform: Fedora
 Platform: CentOS
 Classifier: Development Status :: 3 - Alpha
@@ -20,9 +17,18 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+License-File: LICENSE
+
+A spec-compliant gitignore parser for Python 3.5+
+
+https://github.com/mherrmann/gitignore_parser
```

### Comparing `gitignore_parser-0.1.5/README.md` & `gitignore_parser-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `gitignore_parser-0.1.5/gitignore_parser.egg-info/PKG-INFO` & `gitignore_parser-0.1.6/gitignore_parser.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,15 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: gitignore-parser
-Version: 0.1.5
+Version: 0.1.6
 Summary: A spec-compliant gitignore parser for Python 3.5+
 Home-page: https://github.com/mherrmann/gitignore_parser
 Author: Michael Herrmann
 Author-email: michael+removethisifyouarehuman@herrmann.io
 License: MIT
-Description: A spec-compliant gitignore parser for Python 3.5+
-        
-        https://github.com/mherrmann/gitignore_parser
 Keywords: gitignore
 Platform: MacOS
 Platform: Windows
 Platform: Debian
 Platform: Fedora
 Platform: CentOS
 Classifier: Development Status :: 3 - Alpha
@@ -20,9 +17,18 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+License-File: LICENSE
+
+A spec-compliant gitignore parser for Python 3.5+
+
+https://github.com/mherrmann/gitignore_parser
```

### Comparing `gitignore_parser-0.1.5/gitignore_parser.py` & `gitignore_parser-0.1.6/gitignore_parser.py`

 * *Files identical despite different names*

### Comparing `gitignore_parser-0.1.5/setup.py` & `gitignore_parser-0.1.6/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,36 +5,39 @@
 """
 
 from setuptools import setup
 
 description = 'A spec-compliant gitignore parser for Python 3.5+'
 setup(
     name='gitignore_parser',
-    version='0.1.5',
-    install_requires=["pathlib; python_version < '3.0'"],
+    version='0.1.6',
     description=description,
     long_description=
         description + '\n\nhttps://github.com/mherrmann/gitignore_parser',
     author='Michael Herrmann',
     author_email='michael+removethisifyouarehuman@herrmann.io',
     url='https://github.com/mherrmann/gitignore_parser',
     py_modules=['gitignore_parser'],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
-    
+
         'License :: OSI Approved :: MIT License',
-    
+
         'Operating System :: OS Independent',
-    
+
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
 
         'Topic :: Software Development :: Libraries',
         'Topic :: Software Development :: Libraries :: Python Modules'
     ],
     license='MIT',
     keywords='gitignore',
     platforms=['MacOS', 'Windows', 'Debian', 'Fedora', 'CentOS']
```

