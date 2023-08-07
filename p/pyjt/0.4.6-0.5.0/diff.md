# Comparing `tmp/pyjt-0.4.6.tar.gz` & `tmp/pyjt-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjt-0.4.6.tar", last modified: Fri Aug  4 12:23:53 2023, max compression
+gzip compressed data, was "pyjt-0.5.0.tar", last modified: Mon Aug  7 10:10:34 2023, max compression
```

## Comparing `pyjt-0.4.6.tar` & `pyjt-0.5.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:23:53.048629 pyjt-0.4.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-08-04 12:23:21.000000 pyjt-0.4.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-08-04 12:23:53.048629 pyjt-0.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-08-04 12:23:21.000000 pyjt-0.4.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:23:53.048629 pyjt-0.4.6/pyjt/
--rw-r--r--   0 runner    (1001) docker     (123)     6464 2023-08-04 12:23:21.000000 pyjt-0.4.6/pyjt/ComponentFinder.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-08-04 12:23:21.000000 pyjt-0.4.6/pyjt/Errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-08-04 12:23:21.000000 pyjt-0.4.6/pyjt/Fixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-08-04 12:23:21.000000 pyjt-0.4.6/pyjt/Frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-08-04 12:23:21.000000 pyjt-0.4.6/pyjt/Inspector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-08-04 12:23:21.000000 pyjt-0.4.6/pyjt/Proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7424 2023-08-04 12:23:21.000000 pyjt-0.4.6/pyjt/Robot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-08-04 12:23:21.000000 pyjt-0.4.6/pyjt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:23:53.048629 pyjt-0.4.6/pyjt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-08-04 12:23:53.000000 pyjt-0.4.6/pyjt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-08-04 12:23:53.000000 pyjt-0.4.6/pyjt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:23:53.000000 pyjt-0.4.6/pyjt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-04 12:23:53.000000 pyjt-0.4.6/pyjt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-04 12:23:53.000000 pyjt-0.4.6/pyjt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-04 12:23:21.000000 pyjt-0.4.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:23:53.048629 pyjt-0.4.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:23:53.048629 pyjt-0.4.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-08-04 12:23:21.000000 pyjt-0.4.6/tests/test_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-04 12:23:21.000000 pyjt-0.4.6/tests/test_framefinder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-08-04 12:23:21.000000 pyjt-0.4.6/tests/test_locator.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-08-04 12:23:21.000000 pyjt-0.4.6/tests/test_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-08-04 12:23:21.000000 pyjt-0.4.6/tests/test_textfield.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:10:34.263547 pyjt-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-08-07 10:09:59.000000 pyjt-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-08-07 10:10:34.263547 pyjt-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-08-07 10:09:59.000000 pyjt-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:10:34.259547 pyjt-0.5.0/pyjt/
+-rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-08-07 10:09:59.000000 pyjt-0.5.0/pyjt/ComponentFinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-08-07 10:09:59.000000 pyjt-0.5.0/pyjt/Errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-08-07 10:09:59.000000 pyjt-0.5.0/pyjt/Fixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-08-07 10:09:59.000000 pyjt-0.5.0/pyjt/Frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-08-07 10:09:59.000000 pyjt-0.5.0/pyjt/Inspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-08-07 10:09:59.000000 pyjt-0.5.0/pyjt/Proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7424 2023-08-07 10:09:59.000000 pyjt-0.5.0/pyjt/Robot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-08-07 10:09:59.000000 pyjt-0.5.0/pyjt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:10:34.263547 pyjt-0.5.0/pyjt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-08-07 10:10:34.000000 pyjt-0.5.0/pyjt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-08-07 10:10:34.000000 pyjt-0.5.0/pyjt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 10:10:34.000000 pyjt-0.5.0/pyjt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-07 10:10:34.000000 pyjt-0.5.0/pyjt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-07 10:10:34.000000 pyjt-0.5.0/pyjt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-08-07 10:09:59.000000 pyjt-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 10:10:34.263547 pyjt-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:10:34.263547 pyjt-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-08-07 10:09:59.000000 pyjt-0.5.0/tests/test_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-07 10:09:59.000000 pyjt-0.5.0/tests/test_framefinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-08-07 10:09:59.000000 pyjt-0.5.0/tests/test_locator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-08-07 10:09:59.000000 pyjt-0.5.0/tests/test_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-08-07 10:09:59.000000 pyjt-0.5.0/tests/test_textfield.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-08-07 10:09:59.000000 pyjt-0.5.0/tests/test_xpath.py
```

### Comparing `pyjt-0.4.6/LICENSE` & `pyjt-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyjt-0.4.6/PKG-INFO` & `pyjt-0.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjt
-Version: 0.4.6
+Version: 0.5.0
 Summary: test automation for java UI applications from python
 Author-email: Claudio Klingler <ck@realtime-projects.com>
 Project-URL: Homepage, https://github.com/realtimeprojects/pyjt
 Project-URL: Bug Tracker, https://github.com/realtimeprojects/pyjt/issues
 Project-URL: Documentation, https://pyjt.readthedocs.io/en/latest/
 Project-URL: Releases, https://github.com/realtimeprojects/pyjt/blob/master/RELEASES.md
 Classifier: Programming Language :: Python :: 3
@@ -50,15 +50,15 @@
         # find the frame window titled "Hello World"
         frame = pyjt.FrameFinder.find(title="Hello World")
 
         # Locate and click a button on the frame
         frame.locate(JButton, text="Ok").click()
 
         # Locate and fill text to an text field
-        frame.locate(JTextField, name="textfield1").fill("John Smith")
+        frame.find_by_xpath('//JTextField[@name="textfield1"]').fill("John Smith")
 
         # Close the frame (application)
         frame.close()
 
 ## Further documentation
 
 Check the [documentation on rtfd.io](https://pyjt.readthedocs.io/en/latest/)
```

### Comparing `pyjt-0.4.6/README.md` & `pyjt-0.5.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         # find the frame window titled "Hello World"
         frame = pyjt.FrameFinder.find(title="Hello World")
 
         # Locate and click a button on the frame
         frame.locate(JButton, text="Ok").click()
 
         # Locate and fill text to an text field
-        frame.locate(JTextField, name="textfield1").fill("John Smith")
+        frame.find_by_xpath('//JTextField[@name="textfield1"]').fill("John Smith")
 
         # Close the frame (application)
         frame.close()
 
 ## Further documentation
 
 Check the [documentation on rtfd.io](https://pyjt.readthedocs.io/en/latest/)
```

### Comparing `pyjt-0.4.6/pyjt/ComponentFinder.py` & `pyjt-0.5.0/pyjt/ComponentFinder.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import time
 import logging
+from lxml import etree
 
 from pyjt.Proxy import Proxy
+from pyjt.Inspector import Inspector
 
 log = logging.getLogger(__name__)
 
 
 class Locator:
     """ The Locator determines if a component matches specific search
         criteria.
@@ -137,14 +139,30 @@
             log.debug(f"retry({locator})")
             hit = ComponentFinder._locate(window, locator)
             if hit is not None:
                 return hit
         return None
 
     @staticmethod
+    def find_by_xpath(control, xpath, timeout=None):
+        timeout = timeout if timeout else ComponentFinder.DEFAULT_TIMEOUT
+        timer = Timer(timeout, ComponentFinder.DEFAULT_DELAY).start()
+        xp = etree.XPath(xpath)
+
+        while not timer.elapsed():
+            log.debug(f"retry({xpath})")
+            (tree, mapping) = Inspector.etreemap(control)
+            el = xp(tree)
+            if not el:
+                continue
+            _id = el[0].get("_id")
+            log.warning(_id)
+            return mapping[int(_id)]
+
+    @staticmethod
     def findIn(func, locator=None, timeout=None):
         timeout = timeout if timeout else ComponentFinder.DEFAULT_TIMEOUT
         timer = Timer(timeout, ComponentFinder.DEFAULT_DELAY).start()
 
         while not timer.elapsed():
             log.debug(f"retry({locator})")
             windows = func()
```

### Comparing `pyjt-0.4.6/pyjt/Frame.py` & `pyjt-0.5.0/pyjt/Frame.py`

 * *Files identical despite different names*

### Comparing `pyjt-0.4.6/pyjt/Proxy.py` & `pyjt-0.5.0/pyjt/Proxy.py`

 * *Files identical despite different names*

### Comparing `pyjt-0.4.6/pyjt/Robot.py` & `pyjt-0.5.0/pyjt/Robot.py`

 * *Files identical despite different names*

### Comparing `pyjt-0.4.6/pyjt/__init__.py` & `pyjt-0.5.0/pyjt/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,55 @@
 # flake8: noqa: F401
 import os
 import importlib
 import jpype
 import jpype.imports
 
 def start(classpath=None):
-    """ Start the pyjt JVM.
+    """ Start the JVM.
 
-        Needs to be called before using pyjt.
-
-        :param classpath:   If set, use this classpath for the JVM, otherwise
-                            use CLASSPATH environment variable.
+        Args:
+            classpath (string):
+                If set, use this classpath for the JVM, otherwise
+                use CLASSPATH environment variable.
+
+        Needs to be called before using pyjt. Only after starting
+        the jvm you can import java classes using:
+
+        .. code:: python
+            import javax
+            from java.awt import Component
     """
     cp = os.environ.get('CLASSPATH', '') if classpath is None else classpath
     jpype.startJVM(jpype.getDefaultJVMPath(), f"-Djava.class.path={cp}")
 
 def stop():
+    """ Stop the JVM. """
     jpype.shutdownJVM()
 
 
 
 def run(app, args=[""]):
     """ Run the main function of **app**.
 
         This helper function will start the **app** by invoking it's
         "main" function.
 
+        Args:
+            app (string):      The application to be started, e.g. ``myapp.Application``
+            args (string[]):   The arguments for the main function
+
         Note:
 
             You can as well start your application manually, assuming
             your application is in MyApplication.java, the could would look
             like:
 
+            .. code:: python
+
                 import MyApplication
                 MyApplication.main()
     """
     module = importlib.import_module(app)
     module.main(args)
 
 def shutdown():
```

### Comparing `pyjt-0.4.6/pyjt.egg-info/PKG-INFO` & `pyjt-0.5.0/pyjt.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjt
-Version: 0.4.6
+Version: 0.5.0
 Summary: test automation for java UI applications from python
 Author-email: Claudio Klingler <ck@realtime-projects.com>
 Project-URL: Homepage, https://github.com/realtimeprojects/pyjt
 Project-URL: Bug Tracker, https://github.com/realtimeprojects/pyjt/issues
 Project-URL: Documentation, https://pyjt.readthedocs.io/en/latest/
 Project-URL: Releases, https://github.com/realtimeprojects/pyjt/blob/master/RELEASES.md
 Classifier: Programming Language :: Python :: 3
@@ -50,15 +50,15 @@
         # find the frame window titled "Hello World"
         frame = pyjt.FrameFinder.find(title="Hello World")
 
         # Locate and click a button on the frame
         frame.locate(JButton, text="Ok").click()
 
         # Locate and fill text to an text field
-        frame.locate(JTextField, name="textfield1").fill("John Smith")
+        frame.find_by_xpath('//JTextField[@name="textfield1"]').fill("John Smith")
 
         # Close the frame (application)
         frame.close()
 
 ## Further documentation
 
 Check the [documentation on rtfd.io](https://pyjt.readthedocs.io/en/latest/)
```

### Comparing `pyjt-0.4.6/tests/test_locator.py` & `pyjt-0.5.0/tests/test_locator.py`

 * *Files identical despite different names*

### Comparing `pyjt-0.4.6/tests/test_textfield.py` & `pyjt-0.5.0/tests/test_textfield.py`

 * *Files identical despite different names*

