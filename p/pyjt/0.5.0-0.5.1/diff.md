# Comparing `tmp/pyjt-0.5.0.tar.gz` & `tmp/pyjt-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjt-0.5.0.tar", last modified: Mon Aug  7 10:10:34 2023, max compression
+gzip compressed data, was "pyjt-0.5.1.tar", last modified: Mon Aug  7 10:24:39 2023, max compression
```

## Comparing `pyjt-0.5.0.tar` & `pyjt-0.5.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:10:34.263547 pyjt-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-08-07 10:09:59.000000 pyjt-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-08-07 10:10:34.263547 pyjt-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-08-07 10:09:59.000000 pyjt-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:10:34.259547 pyjt-0.5.0/pyjt/
--rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-08-07 10:09:59.000000 pyjt-0.5.0/pyjt/ComponentFinder.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-08-07 10:09:59.000000 pyjt-0.5.0/pyjt/Errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-08-07 10:09:59.000000 pyjt-0.5.0/pyjt/Fixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-08-07 10:09:59.000000 pyjt-0.5.0/pyjt/Frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-08-07 10:09:59.000000 pyjt-0.5.0/pyjt/Inspector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-08-07 10:09:59.000000 pyjt-0.5.0/pyjt/Proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7424 2023-08-07 10:09:59.000000 pyjt-0.5.0/pyjt/Robot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-08-07 10:09:59.000000 pyjt-0.5.0/pyjt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:10:34.263547 pyjt-0.5.0/pyjt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-08-07 10:10:34.000000 pyjt-0.5.0/pyjt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-08-07 10:10:34.000000 pyjt-0.5.0/pyjt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 10:10:34.000000 pyjt-0.5.0/pyjt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-07 10:10:34.000000 pyjt-0.5.0/pyjt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-07 10:10:34.000000 pyjt-0.5.0/pyjt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-08-07 10:09:59.000000 pyjt-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 10:10:34.263547 pyjt-0.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:10:34.263547 pyjt-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-08-07 10:09:59.000000 pyjt-0.5.0/tests/test_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-07 10:09:59.000000 pyjt-0.5.0/tests/test_framefinder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-08-07 10:09:59.000000 pyjt-0.5.0/tests/test_locator.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-08-07 10:09:59.000000 pyjt-0.5.0/tests/test_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-08-07 10:09:59.000000 pyjt-0.5.0/tests/test_textfield.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-08-07 10:09:59.000000 pyjt-0.5.0/tests/test_xpath.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:24:39.787375 pyjt-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-08-07 10:23:52.000000 pyjt-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-08-07 10:24:39.783375 pyjt-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-08-07 10:23:52.000000 pyjt-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:24:39.783375 pyjt-0.5.1/pyjt/
+-rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-08-07 10:23:52.000000 pyjt-0.5.1/pyjt/ComponentFinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-08-07 10:23:52.000000 pyjt-0.5.1/pyjt/Errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-08-07 10:23:52.000000 pyjt-0.5.1/pyjt/Fixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-08-07 10:23:52.000000 pyjt-0.5.1/pyjt/Frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-08-07 10:23:52.000000 pyjt-0.5.1/pyjt/Inspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-08-07 10:23:52.000000 pyjt-0.5.1/pyjt/Proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7424 2023-08-07 10:23:52.000000 pyjt-0.5.1/pyjt/Robot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-08-07 10:23:52.000000 pyjt-0.5.1/pyjt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:24:39.783375 pyjt-0.5.1/pyjt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-08-07 10:24:39.000000 pyjt-0.5.1/pyjt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-08-07 10:24:39.000000 pyjt-0.5.1/pyjt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 10:24:39.000000 pyjt-0.5.1/pyjt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-07 10:24:39.000000 pyjt-0.5.1/pyjt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-07 10:24:39.000000 pyjt-0.5.1/pyjt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-08-07 10:23:52.000000 pyjt-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 10:24:39.787375 pyjt-0.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:24:39.783375 pyjt-0.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-08-07 10:23:52.000000 pyjt-0.5.1/tests/test_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-07 10:23:52.000000 pyjt-0.5.1/tests/test_framefinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-08-07 10:23:52.000000 pyjt-0.5.1/tests/test_locator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-08-07 10:23:52.000000 pyjt-0.5.1/tests/test_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-08-07 10:23:52.000000 pyjt-0.5.1/tests/test_textfield.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-08-07 10:23:52.000000 pyjt-0.5.1/tests/test_xpath.py
```

### Comparing `pyjt-0.5.0/LICENSE` & `pyjt-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyjt-0.5.0/PKG-INFO` & `pyjt-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjt
-Version: 0.5.0
+Version: 0.5.1
 Summary: test automation for java UI applications from python
 Author-email: Claudio Klingler <ck@realtime-projects.com>
 Project-URL: Homepage, https://github.com/realtimeprojects/pyjt
 Project-URL: Bug Tracker, https://github.com/realtimeprojects/pyjt/issues
 Project-URL: Documentation, https://pyjt.readthedocs.io/en/latest/
 Project-URL: Releases, https://github.com/realtimeprojects/pyjt/blob/master/RELEASES.md
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyjt-0.5.0/README.md` & `pyjt-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `pyjt-0.5.0/pyjt/ComponentFinder.py` & `pyjt-0.5.1/pyjt/ComponentFinder.py`

 * *Files identical despite different names*

### Comparing `pyjt-0.5.0/pyjt/Fixture.py` & `pyjt-0.5.1/pyjt/Fixture.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,23 +73,30 @@
                 xpath (string): The xpath used for searching
 
             Returns:
                 Fixture:
                     A fixture reference to the first component
                     matching the given xpath expression.
 
+            Raises:
+                ElementNotFoundError:
+                    If no element was found matching the given xpath
+
             Example:
 
             .. code:: python
 
                     # search for a JTextField inside a Container which also contains
                     # a label with the text "Name"
-                    frame.find_by_xpath("//Container[//JLabel[@text="Name"]]/JTextField
+                    textfield = frame.find_by_xpath('//Container[//JLabel[@text="Name"]]/JTextField')
         """
-        return ComponentFinder.find_by_xpath(self, xpath)
+        fixture = ComponentFinder.find_by_xpath(self, xpath)
+        if not fixture:
+            raise ElementNotFoundError(f"No element found matching xpath: '{xpath}'")
+        return fixture
 
     def click(self):
         """ Move the mouse over this control and execute a click. """
         log.debug(f"click({self._control})")
         self.robot.move(self._control)
         log.debug(f"executing click({self._control})")
         self.robot.click()
```

### Comparing `pyjt-0.5.0/pyjt/Frame.py` & `pyjt-0.5.1/pyjt/Frame.py`

 * *Files identical despite different names*

### Comparing `pyjt-0.5.0/pyjt/Inspector.py` & `pyjt-0.5.1/pyjt/Inspector.py`

 * *Files identical despite different names*

### Comparing `pyjt-0.5.0/pyjt/Proxy.py` & `pyjt-0.5.1/pyjt/Proxy.py`

 * *Files identical despite different names*

### Comparing `pyjt-0.5.0/pyjt/Robot.py` & `pyjt-0.5.1/pyjt/Robot.py`

 * *Files identical despite different names*

### Comparing `pyjt-0.5.0/pyjt/__init__.py` & `pyjt-0.5.1/pyjt/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjt-0.5.0/pyjt.egg-info/PKG-INFO` & `pyjt-0.5.1/pyjt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjt
-Version: 0.5.0
+Version: 0.5.1
 Summary: test automation for java UI applications from python
 Author-email: Claudio Klingler <ck@realtime-projects.com>
 Project-URL: Homepage, https://github.com/realtimeprojects/pyjt
 Project-URL: Bug Tracker, https://github.com/realtimeprojects/pyjt/issues
 Project-URL: Documentation, https://pyjt.readthedocs.io/en/latest/
 Project-URL: Releases, https://github.com/realtimeprojects/pyjt/blob/master/RELEASES.md
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyjt-0.5.0/pyproject.toml` & `pyjt-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyjt"
-version = "0.5.0"
+version = "0.5.1"
 description="test automation for java UI applications from python"
 authors = [
     { name="Claudio Klingler", email="ck@realtime-projects.com"}
 ]
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `pyjt-0.5.0/tests/test_locator.py` & `pyjt-0.5.1/tests/test_locator.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 from pyjt import Locator, ElementNotFoundError
 
+from tools import assert_raises
+
 import logging
 
 
 def test_locator_has_fail(helloworld, java, javax):
     loc = Locator(role=java.awt.Container).contains(role=javax.swing.JLabel, text="Namex:")
-    try:
-        helloworld.locate(loc)
-    except ElementNotFoundError:
-        return
-    assert False
+    assert_raises(ElementNotFoundError, lambda: helloworld.locate(loc))
 
 
 def test_locator_has(helloworld, java, javax):
     loc = Locator(role=java.awt.Container).has(role=javax.swing.JLabel, text="Name:")
     tf3 = helloworld.locate(loc)
     logging.warning(tf3)
     assert tf3 is not None
```

### Comparing `pyjt-0.5.0/tests/test_textfield.py` & `pyjt-0.5.1/tests/test_textfield.py`

 * *Files identical despite different names*

### Comparing `pyjt-0.5.0/tests/test_xpath.py` & `pyjt-0.5.1/tests/test_xpath.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,26 @@
+from pyjt import ElementNotFoundError
 from lxml import etree
+from tools import assert_raises
 
 import logging
 
 
+def test_miss(helloworld, java, javax):
+    xpath = "//JLabel[contains(@text, 'XName')]"
+    assert_raises(ElementNotFoundError, lambda: helloworld.find_by_xpath(xpath))
+
+
 def test_simple_xpath(helloworld, java, javax):
     xpath = "//JLabel[contains(@text, 'Name')]"
     label = helloworld.find_by_xpath(xpath)
     assert label.getText() == "Name:"
+    xpath = "//JLabel[contains(@text, 'Name')]"
+    label = helloworld.find_by_xpath(xpath)
+    assert label.getText() == "Name:"
 
 
 def test_advanced_xpath(helloworld, java, javax):
     xpath = "//Container[//JLabel[contains(@text, 'Name')]]/JTextField"
     logging.warning(etree.tostring(helloworld.etree()))
     tf = helloworld.find_by_xpath(xpath)
     tf.fill("xpath")
```

