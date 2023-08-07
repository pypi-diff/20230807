# Comparing `tmp/wavefront-pyformance-1.2.3.tar.gz` & `tmp/wavefront-pyformance-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wavefront-pyformance-1.2.3.tar", last modified: Fri Mar 24 01:21:31 2023, max compression
+gzip compressed data, was "wavefront-pyformance-1.2.4.tar", last modified: Mon Aug  7 21:42:01 2023, max compression
```

## Comparing `wavefront-pyformance-1.2.3.tar` & `wavefront-pyformance-1.2.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 01:21:31.026229 wavefront-pyformance-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-24 01:20:54.000000 wavefront-pyformance-1.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6146 2023-03-24 01:21:31.026229 wavefront-pyformance-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-03-24 01:20:54.000000 wavefront-pyformance-1.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-24 01:21:31.026229 wavefront-pyformance-1.2.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2266 2023-03-24 01:20:54.000000 wavefront-pyformance-1.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 01:21:31.022230 wavefront-pyformance-1.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-03-24 01:20:54.000000 wavefront-pyformance-1.2.3/tests/test_wavefront_pyformance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 01:21:31.026229 wavefront-pyformance-1.2.3/wavefront_pyformance/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-24 01:20:54.000000 wavefront-pyformance-1.2.3/wavefront_pyformance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-03-24 01:20:54.000000 wavefront-pyformance-1.2.3/wavefront_pyformance/delta.py
--rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-03-24 01:20:54.000000 wavefront-pyformance-1.2.3/wavefront_pyformance/runtime_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-03-24 01:20:54.000000 wavefront-pyformance-1.2.3/wavefront_pyformance/tagged_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-03-24 01:20:54.000000 wavefront-pyformance-1.2.3/wavefront_pyformance/wavefront_histogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     8998 2023-03-24 01:20:54.000000 wavefront-pyformance-1.2.3/wavefront_pyformance/wavefront_reporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 01:21:31.026229 wavefront-pyformance-1.2.3/wavefront_pyformance.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6146 2023-03-24 01:21:31.000000 wavefront-pyformance-1.2.3/wavefront_pyformance.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-03-24 01:21:31.000000 wavefront-pyformance-1.2.3/wavefront_pyformance.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 01:21:31.000000 wavefront-pyformance-1.2.3/wavefront_pyformance.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-03-24 01:21:31.000000 wavefront-pyformance-1.2.3/wavefront_pyformance.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-24 01:21:31.000000 wavefront-pyformance-1.2.3/wavefront_pyformance.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:42:01.513958 wavefront-pyformance-1.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-07 21:41:21.000000 wavefront-pyformance-1.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6096 2023-08-07 21:42:01.513958 wavefront-pyformance-1.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-08-07 21:41:21.000000 wavefront-pyformance-1.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 21:42:01.513958 wavefront-pyformance-1.2.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2217 2023-08-07 21:41:21.000000 wavefront-pyformance-1.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:42:01.513958 wavefront-pyformance-1.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-08-07 21:41:21.000000 wavefront-pyformance-1.2.4/tests/test_wavefront_pyformance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:42:01.513958 wavefront-pyformance-1.2.4/wavefront_pyformance/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-08-07 21:41:21.000000 wavefront-pyformance-1.2.4/wavefront_pyformance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-08-07 21:41:21.000000 wavefront-pyformance-1.2.4/wavefront_pyformance/delta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5840 2023-08-07 21:41:21.000000 wavefront-pyformance-1.2.4/wavefront_pyformance/runtime_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-08-07 21:41:21.000000 wavefront-pyformance-1.2.4/wavefront_pyformance/tagged_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-08-07 21:41:21.000000 wavefront-pyformance-1.2.4/wavefront_pyformance/wavefront_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8998 2023-08-07 21:41:21.000000 wavefront-pyformance-1.2.4/wavefront_pyformance/wavefront_reporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:42:01.513958 wavefront-pyformance-1.2.4/wavefront_pyformance.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6096 2023-08-07 21:42:01.000000 wavefront-pyformance-1.2.4/wavefront_pyformance.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-08-07 21:42:01.000000 wavefront-pyformance-1.2.4/wavefront_pyformance.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 21:42:01.000000 wavefront-pyformance-1.2.4/wavefront_pyformance.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-07 21:42:01.000000 wavefront-pyformance-1.2.4/wavefront_pyformance.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-07 21:42:01.000000 wavefront-pyformance-1.2.4/wavefront_pyformance.egg-info/top_level.txt
```

### Comparing `wavefront-pyformance-1.2.3/LICENSE` & `wavefront-pyformance-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `wavefront-pyformance-1.2.3/PKG-INFO` & `wavefront-pyformance-1.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: wavefront-pyformance
-Version: 1.2.3
+Version: 1.2.4
 Summary: VMware Aria Operations for Applications Pyformance Library
 Home-page: https://github.com/wavefrontHQ/wavefront-pyformance
 Author: VMware Aria Operations for Applications Team
 Author-email: chitimba@wavefront.com
 License: Apache-2.0
 Keywords: Distributed Tracing,Logging,Metrics,Monitoring,Observability,PyFormance,Tracing,Wavefront,Wavefront Pyformance
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Monitoring
 Classifier: Topic :: System :: Networking :: Monitoring
```

### Comparing `wavefront-pyformance-1.2.3/README.md` & `wavefront-pyformance-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `wavefront-pyformance-1.2.3/setup.py` & `wavefront-pyformance-1.2.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 with open(os.path.join(os.path.abspath(os.path.dirname(__file__)),
                        'README.md')) as fd:
     LONG_DESCRIPTION = fd.read()
 
 setuptools.setup(
     name='wavefront-pyformance',
-    version='1.2.3',  # Please increment with every Pull Request.
+    version='1.2.4',  # Please increment with every Pull Request.
     author='VMware Aria Operations for Applications Team',
     author_email='chitimba@wavefront.com',
     url='https://github.com/wavefrontHQ/wavefront-pyformance',
     license='Apache-2.0',
     description='VMware Aria Operations for Applications Pyformance Library',
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
@@ -42,15 +42,14 @@
         ],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Intended Audience :: Information Technology',
         'Intended Audience :: System Administrators',
         'License :: OSI Approved :: Apache Software License',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Topic :: Software Development :: Libraries :: Python Modules',
         'Topic :: System :: Monitoring',
         'Topic :: System :: Networking :: Monitoring'
```

### Comparing `wavefront-pyformance-1.2.3/tests/test_wavefront_pyformance.py` & `wavefront-pyformance-1.2.4/tests/test_wavefront_pyformance.py`

 * *Files identical despite different names*

### Comparing `wavefront-pyformance-1.2.3/wavefront_pyformance/delta.py` & `wavefront-pyformance-1.2.4/wavefront_pyformance/delta.py`

 * *Files identical despite different names*

### Comparing `wavefront-pyformance-1.2.3/wavefront_pyformance/runtime_metrics.py` & `wavefront-pyformance-1.2.4/wavefront_pyformance/runtime_metrics.py`

 * *Files 4% similar despite different names*

```diff
@@ -111,15 +111,20 @@
         self.registry.gauge("processes.alive",
                             tags=self.custom_tags).set_value(alive)
         self.registry.gauge("processes.daemon",
                             tags=self.custom_tags).set_value(daemon)
 
     def collect_contextswitches(self):
         """Collect Context Switches."""
-        ctx_switches = self.process.num_ctx_switches()
+        try:
+            ctx_switches = self.process.num_ctx_switches()
+        except NotImplementedError:
+            # some platforms do not expose ctx switches information, this is ok
+            ctx_switches = None
+
         if ctx_switches:
             voluntary = ctx_switches.voluntary
             involuntary = ctx_switches.involuntary
             self.registry.gauge("ctxswitch.voluntary",
                                 tags=self.custom_tags).set_value(voluntary)
             self.registry.gauge("ctxswitch.involuntary",
                                 tags=self.custom_tags).set_value(involuntary)
```

### Comparing `wavefront-pyformance-1.2.3/wavefront_pyformance/tagged_registry.py` & `wavefront-pyformance-1.2.4/wavefront_pyformance/tagged_registry.py`

 * *Files identical despite different names*

### Comparing `wavefront-pyformance-1.2.3/wavefront_pyformance/wavefront_histogram.py` & `wavefront-pyformance-1.2.4/wavefront_pyformance/wavefront_histogram.py`

 * *Files identical despite different names*

### Comparing `wavefront-pyformance-1.2.3/wavefront_pyformance/wavefront_reporter.py` & `wavefront-pyformance-1.2.4/wavefront_pyformance/wavefront_reporter.py`

 * *Files identical despite different names*

### Comparing `wavefront-pyformance-1.2.3/wavefront_pyformance.egg-info/PKG-INFO` & `wavefront-pyformance-1.2.4/wavefront_pyformance.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: wavefront-pyformance
-Version: 1.2.3
+Version: 1.2.4
 Summary: VMware Aria Operations for Applications Pyformance Library
 Home-page: https://github.com/wavefrontHQ/wavefront-pyformance
 Author: VMware Aria Operations for Applications Team
 Author-email: chitimba@wavefront.com
 License: Apache-2.0
 Keywords: Distributed Tracing,Logging,Metrics,Monitoring,Observability,PyFormance,Tracing,Wavefront,Wavefront Pyformance
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Monitoring
 Classifier: Topic :: System :: Networking :: Monitoring
```

