# Comparing `tmp/shaclapi-0.9.7.tar.gz` & `tmp/shaclapi-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shaclapi-0.9.7.tar", last modified: Mon Feb  6 19:03:48 2023, max compression
+gzip compressed data, was "shaclapi-0.9.8.tar", last modified: Tue Jun 27 13:57:11 2023, max compression
```

## Comparing `shaclapi-0.9.7.tar` & `shaclapi-0.9.8.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 19:03:48.337671 shaclapi-0.9.7/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-02-06 19:03:36.000000 shaclapi-0.9.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    23128 2023-02-06 19:03:48.337671 shaclapi-0.9.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22190 2023-02-06 19:03:36.000000 shaclapi-0.9.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-06 19:03:48.337671 shaclapi-0.9.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-02-06 19:03:36.000000 shaclapi-0.9.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 19:03:48.333671 shaclapi-0.9.7/shaclapi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-06 19:03:36.000000 shaclapi-0.9.7/shaclapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19087 2023-02-06 19:03:36.000000 shaclapi-0.9.7/shaclapi/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12495 2023-02-06 19:03:36.000000 shaclapi-0.9.7/shaclapi/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-02-06 19:03:36.000000 shaclapi-0.9.7/shaclapi/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 19:03:48.337671 shaclapi-0.9.7/shaclapi/multiprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-02-06 19:03:36.000000 shaclapi-0.9.7/shaclapi/multiprocessing/PipeAdapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-02-06 19:03:36.000000 shaclapi-0.9.7/shaclapi/multiprocessing/ThreadEx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 19:03:48.337671 shaclapi-0.9.7/shaclapi/multiprocessing/Xgjoin/
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-02-06 19:03:36.000000 shaclapi-0.9.7/shaclapi/multiprocessing/Xgjoin/OperatorStructures.py
--rw-r--r--   0 runner    (1001) docker     (123)    14796 2023-02-06 19:03:36.000000 shaclapi-0.9.7/shaclapi/multiprocessing/Xgjoin/Xgjoin.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-06 19:03:36.000000 shaclapi-0.9.7/shaclapi/multiprocessing/Xgjoin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 19:03:48.337671 shaclapi-0.9.7/shaclapi/multiprocessing/Xgoptional/
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-02-06 19:03:36.000000 shaclapi-0.9.7/shaclapi/multiprocessing/Xgoptional/OperatorStructures.py
--rw-r--r--   0 runner    (1001) docker     (123)    16993 2023-02-06 19:03:36.000000 shaclapi-0.9.7/shaclapi/multiprocessing/Xgoptional/Xgoptional.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-06 19:03:36.000000 shaclapi-0.9.7/shaclapi/multiprocessing/Xgoptional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-06 19:03:36.000000 shaclapi-0.9.7/shaclapi/multiprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-02-06 19:03:36.000000 shaclapi-0.9.7/shaclapi/multiprocessing/contactSource.py
--rw-r--r--   0 runner    (1001) docker     (123)     8065 2023-02-06 19:03:36.000000 shaclapi-0.9.7/shaclapi/multiprocessing/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-02-06 19:03:36.000000 shaclapi-0.9.7/shaclapi/multiprocessing/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-02-06 19:03:36.000000 shaclapi-0.9.7/shaclapi/output.py
--rw-r--r--   0 runner    (1001) docker     (123)    14603 2023-02-06 19:03:36.000000 shaclapi-0.9.7/shaclapi/query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 19:03:48.337671 shaclapi-0.9.7/shaclapi/reduction/
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-02-06 19:03:36.000000 shaclapi-0.9.7/shaclapi/reduction/Reduction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-02-06 19:03:36.000000 shaclapi-0.9.7/shaclapi/reduction/ValidationResultTransmitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-02-06 19:03:36.000000 shaclapi-0.9.7/shaclapi/reduction/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 19:03:48.337671 shaclapi-0.9.7/shaclapi/reduction/s2spy/
--rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-02-06 19:03:36.000000 shaclapi-0.9.7/shaclapi/reduction/s2spy/ReducedShapeParser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-02-06 19:03:36.000000 shaclapi-0.9.7/shaclapi/reduction/s2spy/ReducedShapeSchema.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-02-06 19:03:36.000000 shaclapi-0.9.7/shaclapi/reduction/s2spy/RuleBasedValidationResultStreaming.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-06 19:03:36.000000 shaclapi-0.9.7/shaclapi/reduction/s2spy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 19:03:48.337671 shaclapi-0.9.7/shaclapi/reduction/travshacl/
--rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-02-06 19:03:36.000000 shaclapi-0.9.7/shaclapi/reduction/travshacl/ReducedShapeParser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-02-06 19:03:36.000000 shaclapi-0.9.7/shaclapi/reduction/travshacl/ReducedShapeSchema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-02-06 19:03:36.000000 shaclapi-0.9.7/shaclapi/reduction/travshacl/ValidationResultStreaming.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-06 19:03:36.000000 shaclapi-0.9.7/shaclapi/reduction/travshacl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7390 2023-02-06 19:03:36.000000 shaclapi-0.9.7/shaclapi/statsCalculation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-02-06 19:03:36.000000 shaclapi-0.9.7/shaclapi/triple.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 19:03:48.337671 shaclapi-0.9.7/shaclapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23128 2023-02-06 19:03:48.000000 shaclapi-0.9.7/shaclapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-02-06 19:03:48.000000 shaclapi-0.9.7/shaclapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-06 19:03:48.000000 shaclapi-0.9.7/shaclapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-02-06 19:03:48.000000 shaclapi-0.9.7/shaclapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-06 19:03:48.000000 shaclapi-0.9.7/shaclapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:57:11.193530 shaclapi-0.9.8/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-27 13:56:58.000000 shaclapi-0.9.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    23179 2023-06-27 13:57:11.193530 shaclapi-0.9.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22190 2023-06-27 13:56:58.000000 shaclapi-0.9.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 13:57:11.193530 shaclapi-0.9.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-06-27 13:56:58.000000 shaclapi-0.9.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:57:11.189530 shaclapi-0.9.8/shaclapi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:58.000000 shaclapi-0.9.8/shaclapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19093 2023-06-27 13:56:58.000000 shaclapi-0.9.8/shaclapi/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12495 2023-06-27 13:56:58.000000 shaclapi-0.9.8/shaclapi/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-27 13:56:58.000000 shaclapi-0.9.8/shaclapi/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:57:11.189530 shaclapi-0.9.8/shaclapi/multiprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-06-27 13:56:58.000000 shaclapi-0.9.8/shaclapi/multiprocessing/PipeAdapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-06-27 13:56:58.000000 shaclapi-0.9.8/shaclapi/multiprocessing/ThreadEx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:57:11.189530 shaclapi-0.9.8/shaclapi/multiprocessing/Xgjoin/
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-06-27 13:56:58.000000 shaclapi-0.9.8/shaclapi/multiprocessing/Xgjoin/OperatorStructures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14796 2023-06-27 13:56:58.000000 shaclapi-0.9.8/shaclapi/multiprocessing/Xgjoin/Xgjoin.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:58.000000 shaclapi-0.9.8/shaclapi/multiprocessing/Xgjoin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:57:11.189530 shaclapi-0.9.8/shaclapi/multiprocessing/Xgoptional/
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-06-27 13:56:58.000000 shaclapi-0.9.8/shaclapi/multiprocessing/Xgoptional/OperatorStructures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16993 2023-06-27 13:56:58.000000 shaclapi-0.9.8/shaclapi/multiprocessing/Xgoptional/Xgoptional.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:58.000000 shaclapi-0.9.8/shaclapi/multiprocessing/Xgoptional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:58.000000 shaclapi-0.9.8/shaclapi/multiprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-06-27 13:56:58.000000 shaclapi-0.9.8/shaclapi/multiprocessing/contactSource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8065 2023-06-27 13:56:58.000000 shaclapi-0.9.8/shaclapi/multiprocessing/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-06-27 13:56:58.000000 shaclapi-0.9.8/shaclapi/multiprocessing/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-27 13:56:58.000000 shaclapi-0.9.8/shaclapi/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14603 2023-06-27 13:56:58.000000 shaclapi-0.9.8/shaclapi/query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:57:11.193530 shaclapi-0.9.8/shaclapi/reduction/
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-06-27 13:56:58.000000 shaclapi-0.9.8/shaclapi/reduction/Reduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-06-27 13:56:58.000000 shaclapi-0.9.8/shaclapi/reduction/ValidationResultTransmitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-27 13:56:58.000000 shaclapi-0.9.8/shaclapi/reduction/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:57:11.193530 shaclapi-0.9.8/shaclapi/reduction/s2spy/
+-rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-06-27 13:56:58.000000 shaclapi-0.9.8/shaclapi/reduction/s2spy/ReducedShapeParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-06-27 13:56:58.000000 shaclapi-0.9.8/shaclapi/reduction/s2spy/ReducedShapeSchema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-27 13:56:58.000000 shaclapi-0.9.8/shaclapi/reduction/s2spy/RuleBasedValidationResultStreaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:58.000000 shaclapi-0.9.8/shaclapi/reduction/s2spy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:57:11.193530 shaclapi-0.9.8/shaclapi/reduction/travshacl/
+-rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-06-27 13:56:58.000000 shaclapi-0.9.8/shaclapi/reduction/travshacl/ReducedShapeParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-06-27 13:56:58.000000 shaclapi-0.9.8/shaclapi/reduction/travshacl/ReducedShapeSchema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-06-27 13:56:58.000000 shaclapi-0.9.8/shaclapi/reduction/travshacl/ValidationResultStreaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 13:56:58.000000 shaclapi-0.9.8/shaclapi/reduction/travshacl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7390 2023-06-27 13:56:58.000000 shaclapi-0.9.8/shaclapi/statsCalculation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-06-27 13:56:58.000000 shaclapi-0.9.8/shaclapi/triple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:57:11.189530 shaclapi-0.9.8/shaclapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23179 2023-06-27 13:57:11.000000 shaclapi-0.9.8/shaclapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-27 13:57:11.000000 shaclapi-0.9.8/shaclapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 13:57:11.000000 shaclapi-0.9.8/shaclapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-27 13:57:11.000000 shaclapi-0.9.8/shaclapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-27 13:57:11.000000 shaclapi-0.9.8/shaclapi.egg-info/top_level.txt
```

### Comparing `shaclapi-0.9.7/PKG-INFO` & `shaclapi-0.9.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: shaclapi
-Version: 0.9.7
+Version: 0.9.8
 Summary: An API implementing optimizations over SHACL validators.
 Home-page: https://github.com/SDM-TIB/shaclAPI
-Download-URL: https://github.com/SDM-TIB/shaclAPI/archive/refs/tags/v0.9.7.tar.gz
+Download-URL: https://github.com/SDM-TIB/shaclAPI/archive/refs/tags/v0.9.8.tar.gz
 Author: Julian Gercke, Philipp D. Rohde, Fabian Johannsen
 Author-email: philipp.rohde@tib.eu
 License: GNU/GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 [![Tests](https://github.com/SDM-TIB/shaclAPI/actions/workflows/test.yml/badge.svg)](https://github.com/SDM-TIB/shaclAPI/actions/workflows/test.yml)
```

### Comparing `shaclapi-0.9.7/README.md` & `shaclapi-0.9.8/README.md`

 * *Files identical despite different names*

### Comparing `shaclapi-0.9.7/setup.py` & `shaclapi-0.9.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 from distutils.core import setup
 from setuptools import find_packages
 
-VERSION = '0.9.7'
+VERSION = '0.9.8'
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='shaclapi',
     version=VERSION,
@@ -17,15 +17,15 @@
     author='Julian Gercke, Philipp D. Rohde, Fabian Johannsen',
     author_email='philipp.rohde@tib.eu',
     url='https://github.com/SDM-TIB/shaclAPI',
     download_url='https://github.com/SDM-TIB/shaclAPI/archive/refs/tags/v' + VERSION + '.tar.gz',
     packages=find_packages(exclude='tests'),
     install_requires=[
         'SPARQLWrapper>=2.0.0',
-        'requests>=2.27.1',
+        'requests>=2.31.0',
         'SHACL2SPARQLpy>=1.1.1',
         'TravSHACL>=1.2.0',
         'multiprocessing_logging>=0.3.1',
         'regex>=2022.3.15'
     ],
     include_package_data=True,
     python_requires='>=3.8',
@@ -33,12 +33,13 @@
         'Development Status :: 4 - Beta',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3 :: Only',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Operating System :: OS Independent',
         'Intended Audience :: Science/Research'
     ]
 )
```

### Comparing `shaclapi-0.9.7/shaclapi/api.py` & `shaclapi-0.9.8/shaclapi/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,15 +221,15 @@
     if not QUEUE_OUTPUT:
         next_result = result_queue.receiver.get()
         output = []
         if config.output_format == 'test':
             while next_result != 'EOF':
                 output = next_result
                 next_result = result_queue.receiver.get()
-                print(len(output['validTargets']), len(output['invalidTargets']))
+                logger.info(len(output['validTargets']), len(output['invalidTargets']))
         else:
             while next_result != 'EOF':
                 output += [next_result]
                 next_result = result_queue.receiver.get()
         logger.debug('Finished collecting results!')
         return Output(output)
     else:
```

### Comparing `shaclapi-0.9.7/shaclapi/config.py` & `shaclapi-0.9.8/shaclapi/config.py`

 * *Files identical despite different names*

### Comparing `shaclapi-0.9.7/shaclapi/logger.py` & `shaclapi-0.9.8/shaclapi/logger.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,8 +19,7 @@
     """
     handler.setFormatter(logging.Formatter(log_format))
     handler.setLevel(level)
     logger = logging.getLogger('shaclapi')
     logger.addHandler(handler)
     logger.setLevel(level)
     install_mp_handler(logger)
-    print('shaclAPI logger assigned!')
```

### Comparing `shaclapi-0.9.7/shaclapi/multiprocessing/PipeAdapter.py` & `shaclapi-0.9.8/shaclapi/multiprocessing/PipeAdapter.py`

 * *Files identical despite different names*

### Comparing `shaclapi-0.9.7/shaclapi/multiprocessing/ThreadEx.py` & `shaclapi-0.9.8/shaclapi/multiprocessing/ThreadEx.py`

 * *Files identical despite different names*

### Comparing `shaclapi-0.9.7/shaclapi/multiprocessing/Xgjoin/OperatorStructures.py` & `shaclapi-0.9.8/shaclapi/multiprocessing/Xgjoin/OperatorStructures.py`

 * *Files identical despite different names*

### Comparing `shaclapi-0.9.7/shaclapi/multiprocessing/Xgjoin/Xgjoin.py` & `shaclapi-0.9.8/shaclapi/multiprocessing/Xgjoin/Xgjoin.py`

 * *Files identical despite different names*

### Comparing `shaclapi-0.9.7/shaclapi/multiprocessing/Xgoptional/OperatorStructures.py` & `shaclapi-0.9.8/shaclapi/multiprocessing/Xgoptional/OperatorStructures.py`

 * *Files identical despite different names*

### Comparing `shaclapi-0.9.7/shaclapi/multiprocessing/Xgoptional/Xgoptional.py` & `shaclapi-0.9.8/shaclapi/multiprocessing/Xgoptional/Xgoptional.py`

 * *Files identical despite different names*

### Comparing `shaclapi-0.9.7/shaclapi/multiprocessing/contactSource.py` & `shaclapi-0.9.8/shaclapi/multiprocessing/contactSource.py`

 * *Files identical despite different names*

### Comparing `shaclapi-0.9.7/shaclapi/multiprocessing/functions.py` & `shaclapi-0.9.8/shaclapi/multiprocessing/functions.py`

 * *Files identical despite different names*

### Comparing `shaclapi-0.9.7/shaclapi/multiprocessing/runner.py` & `shaclapi-0.9.8/shaclapi/multiprocessing/runner.py`

 * *Files identical despite different names*

### Comparing `shaclapi-0.9.7/shaclapi/query.py` & `shaclapi-0.9.8/shaclapi/query.py`

 * *Files identical despite different names*

### Comparing `shaclapi-0.9.7/shaclapi/reduction/Reduction.py` & `shaclapi-0.9.8/shaclapi/reduction/Reduction.py`

 * *Files identical despite different names*

### Comparing `shaclapi-0.9.7/shaclapi/reduction/ValidationResultTransmitter.py` & `shaclapi-0.9.8/shaclapi/reduction/ValidationResultTransmitter.py`

 * *Files identical despite different names*

### Comparing `shaclapi-0.9.7/shaclapi/reduction/__init__.py` & `shaclapi-0.9.8/shaclapi/reduction/__init__.py`

 * *Files identical despite different names*

### Comparing `shaclapi-0.9.7/shaclapi/reduction/s2spy/ReducedShapeParser.py` & `shaclapi-0.9.8/shaclapi/reduction/s2spy/ReducedShapeParser.py`

 * *Files identical despite different names*

### Comparing `shaclapi-0.9.7/shaclapi/reduction/s2spy/ReducedShapeSchema.py` & `shaclapi-0.9.8/shaclapi/reduction/s2spy/ReducedShapeSchema.py`

 * *Files identical despite different names*

### Comparing `shaclapi-0.9.7/shaclapi/reduction/s2spy/RuleBasedValidationResultStreaming.py` & `shaclapi-0.9.8/shaclapi/reduction/s2spy/RuleBasedValidationResultStreaming.py`

 * *Files identical despite different names*

### Comparing `shaclapi-0.9.7/shaclapi/reduction/travshacl/ReducedShapeParser.py` & `shaclapi-0.9.8/shaclapi/reduction/travshacl/ReducedShapeParser.py`

 * *Files identical despite different names*

### Comparing `shaclapi-0.9.7/shaclapi/reduction/travshacl/ReducedShapeSchema.py` & `shaclapi-0.9.8/shaclapi/reduction/travshacl/ReducedShapeSchema.py`

 * *Files identical despite different names*

### Comparing `shaclapi-0.9.7/shaclapi/reduction/travshacl/ValidationResultStreaming.py` & `shaclapi-0.9.8/shaclapi/reduction/travshacl/ValidationResultStreaming.py`

 * *Files identical despite different names*

### Comparing `shaclapi-0.9.7/shaclapi/statsCalculation.py` & `shaclapi-0.9.8/shaclapi/statsCalculation.py`

 * *Files identical despite different names*

### Comparing `shaclapi-0.9.7/shaclapi/triple.py` & `shaclapi-0.9.8/shaclapi/triple.py`

 * *Files identical despite different names*

### Comparing `shaclapi-0.9.7/shaclapi.egg-info/PKG-INFO` & `shaclapi-0.9.8/shaclapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: shaclapi
-Version: 0.9.7
+Version: 0.9.8
 Summary: An API implementing optimizations over SHACL validators.
 Home-page: https://github.com/SDM-TIB/shaclAPI
-Download-URL: https://github.com/SDM-TIB/shaclAPI/archive/refs/tags/v0.9.7.tar.gz
+Download-URL: https://github.com/SDM-TIB/shaclAPI/archive/refs/tags/v0.9.8.tar.gz
 Author: Julian Gercke, Philipp D. Rohde, Fabian Johannsen
 Author-email: philipp.rohde@tib.eu
 License: GNU/GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 [![Tests](https://github.com/SDM-TIB/shaclAPI/actions/workflows/test.yml/badge.svg)](https://github.com/SDM-TIB/shaclAPI/actions/workflows/test.yml)
```

### Comparing `shaclapi-0.9.7/shaclapi.egg-info/SOURCES.txt` & `shaclapi-0.9.8/shaclapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

