# Comparing `tmp/pyjt-0.5.1.tar.gz` & `tmp/pyjt-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjt-0.5.1.tar", last modified: Mon Aug  7 10:24:39 2023, max compression
+gzip compressed data, was "pyjt-0.5.2.tar", last modified: Mon Aug  7 12:31:36 2023, max compression
```

## Comparing `pyjt-0.5.1.tar` & `pyjt-0.5.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:24:39.787375 pyjt-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-08-07 10:23:52.000000 pyjt-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-08-07 10:24:39.783375 pyjt-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-08-07 10:23:52.000000 pyjt-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:24:39.783375 pyjt-0.5.1/pyjt/
--rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-08-07 10:23:52.000000 pyjt-0.5.1/pyjt/ComponentFinder.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-08-07 10:23:52.000000 pyjt-0.5.1/pyjt/Errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-08-07 10:23:52.000000 pyjt-0.5.1/pyjt/Fixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-08-07 10:23:52.000000 pyjt-0.5.1/pyjt/Frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-08-07 10:23:52.000000 pyjt-0.5.1/pyjt/Inspector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-08-07 10:23:52.000000 pyjt-0.5.1/pyjt/Proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7424 2023-08-07 10:23:52.000000 pyjt-0.5.1/pyjt/Robot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-08-07 10:23:52.000000 pyjt-0.5.1/pyjt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:24:39.783375 pyjt-0.5.1/pyjt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-08-07 10:24:39.000000 pyjt-0.5.1/pyjt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-08-07 10:24:39.000000 pyjt-0.5.1/pyjt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 10:24:39.000000 pyjt-0.5.1/pyjt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-07 10:24:39.000000 pyjt-0.5.1/pyjt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-07 10:24:39.000000 pyjt-0.5.1/pyjt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-08-07 10:23:52.000000 pyjt-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 10:24:39.787375 pyjt-0.5.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:24:39.783375 pyjt-0.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-08-07 10:23:52.000000 pyjt-0.5.1/tests/test_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-07 10:23:52.000000 pyjt-0.5.1/tests/test_framefinder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-08-07 10:23:52.000000 pyjt-0.5.1/tests/test_locator.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-08-07 10:23:52.000000 pyjt-0.5.1/tests/test_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-08-07 10:23:52.000000 pyjt-0.5.1/tests/test_textfield.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-08-07 10:23:52.000000 pyjt-0.5.1/tests/test_xpath.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:31:36.860743 pyjt-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-08-07 12:31:00.000000 pyjt-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-08-07 12:31:36.860743 pyjt-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-08-07 12:31:00.000000 pyjt-0.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:31:36.856743 pyjt-0.5.2/pyjt/
+-rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-08-07 12:31:00.000000 pyjt-0.5.2/pyjt/ComponentFinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-08-07 12:31:00.000000 pyjt-0.5.2/pyjt/Errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-08-07 12:31:00.000000 pyjt-0.5.2/pyjt/Fixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-08-07 12:31:00.000000 pyjt-0.5.2/pyjt/Frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-08-07 12:31:00.000000 pyjt-0.5.2/pyjt/Inspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-08-07 12:31:00.000000 pyjt-0.5.2/pyjt/Proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7306 2023-08-07 12:31:00.000000 pyjt-0.5.2/pyjt/Robot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-08-07 12:31:00.000000 pyjt-0.5.2/pyjt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:31:36.856743 pyjt-0.5.2/pyjt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-08-07 12:31:36.000000 pyjt-0.5.2/pyjt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-08-07 12:31:36.000000 pyjt-0.5.2/pyjt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 12:31:36.000000 pyjt-0.5.2/pyjt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-07 12:31:36.000000 pyjt-0.5.2/pyjt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-07 12:31:36.000000 pyjt-0.5.2/pyjt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-08-07 12:31:00.000000 pyjt-0.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 12:31:36.860743 pyjt-0.5.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:31:36.856743 pyjt-0.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-08-07 12:31:00.000000 pyjt-0.5.2/tests/test_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-07 12:31:00.000000 pyjt-0.5.2/tests/test_framefinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-08-07 12:31:00.000000 pyjt-0.5.2/tests/test_locator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-08-07 12:31:00.000000 pyjt-0.5.2/tests/test_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-08-07 12:31:00.000000 pyjt-0.5.2/tests/test_textfield.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-08-07 12:31:00.000000 pyjt-0.5.2/tests/test_xpath.py
```

### Comparing `pyjt-0.5.1/LICENSE` & `pyjt-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyjt-0.5.1/PKG-INFO` & `pyjt-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjt
-Version: 0.5.1
+Version: 0.5.2
 Summary: test automation for java UI applications from python
 Author-email: Claudio Klingler <ck@realtime-projects.com>
 Project-URL: Homepage, https://github.com/realtimeprojects/pyjt
 Project-URL: Bug Tracker, https://github.com/realtimeprojects/pyjt/issues
 Project-URL: Documentation, https://pyjt.readthedocs.io/en/latest/
 Project-URL: Releases, https://github.com/realtimeprojects/pyjt/blob/master/RELEASES.md
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyjt-0.5.1/README.md` & `pyjt-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `pyjt-0.5.1/pyjt/ComponentFinder.py` & `pyjt-0.5.2/pyjt/ComponentFinder.py`

 * *Files identical despite different names*

### Comparing `pyjt-0.5.1/pyjt/Fixture.py` & `pyjt-0.5.2/pyjt/Fixture.py`

 * *Files identical despite different names*

### Comparing `pyjt-0.5.1/pyjt/Frame.py` & `pyjt-0.5.2/pyjt/Frame.py`

 * *Files identical despite different names*

### Comparing `pyjt-0.5.1/pyjt/Inspector.py` & `pyjt-0.5.2/pyjt/Inspector.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,31 +45,30 @@
     def etreemap(component, mapping=None):
         if not mapping:
             mapping = {}
         _id = id(component)
         mapping[_id] = component
         element = etree.Element(str(component.getClass().getSimpleName()))
         text = _getText(component)
-        if text:
+        if text is not None:
             element.set("text", text)
         element.set("name", str(component.getName()))
         title = _getTitle(component)
-        if title:
+        if title is not None:
             element.set("title", str(title))
         element.set("_id", str(_id))
 
         for subelement in component.components():
-            log.debug(f"etree: found {subelement}")
             element.append(Inspector.etreemap(subelement, mapping)[0])
         return (element, mapping)
 
 
 def _getTitle(component):
     if not hasattr(component, 'getTitle'):
-        return "N/A"
+        return None
     return str(component.getTitle())
 
 
 def _getText(component):
     if not hasattr(component, 'getText'):
         return None
     return str(component.getText())
```

### Comparing `pyjt-0.5.1/pyjt/Proxy.py` & `pyjt-0.5.2/pyjt/Proxy.py`

 * *Files identical despite different names*

### Comparing `pyjt-0.5.1/pyjt/Robot.py` & `pyjt-0.5.2/pyjt/Robot.py`

 * *Files 8% similar despite different names*

```diff
@@ -136,20 +136,17 @@
         """
         position = control.getLocationOnScreen()
         self._robot.mouseMove(position.x + 2, position.y + 2)
 
     def click(self):
         """ Execute a click of the left mouse. """
         import java
-        log.debug("zmousedown")
         btn = java.awt.event.InputEvent.getMaskForButton(1)
         self._robot.mousePress(btn)
-        log.debug(f"sleeping for {1 / self._typespeed}")
         time.sleep(1 / self._typespeed)
-        log.debug("mouseup")
         self._robot.mouseRelease(btn)
 
     def selectAll(self):
         """ Emulate selecting all text in the current context by pressing CTRL-A. """
         from java.awt.event import KeyEvent
         self._typeVKs([KeyEvent.VK_CONTROL, KeyEvent.VK_A])
```

### Comparing `pyjt-0.5.1/pyjt/__init__.py` & `pyjt-0.5.2/pyjt/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjt-0.5.1/pyjt.egg-info/PKG-INFO` & `pyjt-0.5.2/pyjt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjt
-Version: 0.5.1
+Version: 0.5.2
 Summary: test automation for java UI applications from python
 Author-email: Claudio Klingler <ck@realtime-projects.com>
 Project-URL: Homepage, https://github.com/realtimeprojects/pyjt
 Project-URL: Bug Tracker, https://github.com/realtimeprojects/pyjt/issues
 Project-URL: Documentation, https://pyjt.readthedocs.io/en/latest/
 Project-URL: Releases, https://github.com/realtimeprojects/pyjt/blob/master/RELEASES.md
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyjt-0.5.1/pyproject.toml` & `pyjt-0.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyjt"
-version = "0.5.1"
+version = "0.5.2"
 description="test automation for java UI applications from python"
 authors = [
     { name="Claudio Klingler", email="ck@realtime-projects.com"}
 ]
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `pyjt-0.5.1/tests/test_locator.py` & `pyjt-0.5.2/tests/test_locator.py`

 * *Files identical despite different names*

### Comparing `pyjt-0.5.1/tests/test_textfield.py` & `pyjt-0.5.2/tests/test_textfield.py`

 * *Files identical despite different names*

### Comparing `pyjt-0.5.1/tests/test_xpath.py` & `pyjt-0.5.2/tests/test_xpath.py`

 * *Files identical despite different names*

