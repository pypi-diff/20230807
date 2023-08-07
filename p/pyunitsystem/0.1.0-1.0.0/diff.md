# Comparing `tmp/pyunitsystem-0.1.0.tar.gz` & `tmp/pyunitsystem-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyunitsystem-0.1.0.tar", last modified: Fri Aug  4 11:45:04 2023, max compression
+gzip compressed data, was "pyunitsystem-1.0.0.tar", last modified: Mon Aug  7 07:12:37 2023, max compression
```

## Comparing `pyunitsystem-0.1.0.tar` & `pyunitsystem-1.0.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-08-04 11:45:04.197270 pyunitsystem-0.1.0/
--rw-r--r--   0 payno     (1000) payno     (1000)     1218 2023-08-04 11:44:16.000000 pyunitsystem-0.1.0/LICENSE
--rw-r--r--   0 payno     (1000) payno     (1000)     2907 2023-08-04 11:45:04.197270 pyunitsystem-0.1.0/PKG-INFO
--rw-r--r--   0 payno     (1000) payno     (1000)       44 2023-08-04 11:42:59.000000 pyunitsystem-0.1.0/README.md
--rw-r--r--   0 payno     (1000) payno     (1000)     1756 2023-08-04 11:43:17.000000 pyunitsystem-0.1.0/pyproject.toml
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-08-04 11:45:04.197270 pyunitsystem-0.1.0/pyunitsystem/
--rw-r--r--   0 payno     (1000) payno     (1000)      299 2023-08-04 11:35:43.000000 pyunitsystem-0.1.0/pyunitsystem/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1058 2023-08-04 11:43:23.000000 pyunitsystem-0.1.0/pyunitsystem/electriccurrentsystem.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1876 2023-08-04 11:44:57.000000 pyunitsystem-0.1.0/pyunitsystem/energysystem.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1953 2023-08-04 11:44:57.000000 pyunitsystem-0.1.0/pyunitsystem/metricsystem.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-08-04 11:45:04.197270 pyunitsystem-0.1.0/pyunitsystem/test/
--rw-r--r--   0 payno     (1000) payno     (1000)     3288 2023-08-04 11:44:52.000000 pyunitsystem-0.1.0/pyunitsystem/test/test_unitsystem.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1771 2023-08-04 11:44:58.000000 pyunitsystem-0.1.0/pyunitsystem/timesystem.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1621 2023-08-04 11:35:18.000000 pyunitsystem-0.1.0/pyunitsystem/unit.py
--rw-r--r--   0 payno     (1000) payno     (1000)      581 2023-08-04 11:43:53.000000 pyunitsystem-0.1.0/pyunitsystem/voltagesystem.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-08-04 11:45:04.197270 pyunitsystem-0.1.0/pyunitsystem.egg-info/
--rw-r--r--   0 payno     (1000) payno     (1000)     2907 2023-08-04 11:45:04.000000 pyunitsystem-0.1.0/pyunitsystem.egg-info/PKG-INFO
--rw-r--r--   0 payno     (1000) payno     (1000)      421 2023-08-04 11:45:04.000000 pyunitsystem-0.1.0/pyunitsystem.egg-info/SOURCES.txt
--rw-r--r--   0 payno     (1000) payno     (1000)        1 2023-08-04 11:45:04.000000 pyunitsystem-0.1.0/pyunitsystem.egg-info/dependency_links.txt
--rw-r--r--   0 payno     (1000) payno     (1000)       24 2023-08-04 11:45:04.000000 pyunitsystem-0.1.0/pyunitsystem.egg-info/top_level.txt
--rw-r--r--   0 payno     (1000) payno     (1000)       38 2023-08-04 11:45:04.197270 pyunitsystem-0.1.0/setup.cfg
--rw-r--r--   0 payno     (1000) payno     (1000)       38 2023-08-04 11:27:16.000000 pyunitsystem-0.1.0/setup.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-08-07 07:12:37.067546 pyunitsystem-1.0.0/
+-rw-r--r--   0 payno     (1000) payno     (1000)     1218 2023-08-07 06:19:59.000000 pyunitsystem-1.0.0/LICENSE
+-rw-r--r--   0 payno     (1000) payno     (1000)     2928 2023-08-07 07:12:37.067546 pyunitsystem-1.0.0/PKG-INFO
+-rw-r--r--   0 payno     (1000) payno     (1000)       44 2023-08-07 06:19:59.000000 pyunitsystem-1.0.0/README.md
+-rw-r--r--   0 payno     (1000) payno     (1000)     1828 2023-08-07 06:57:08.000000 pyunitsystem-1.0.0/pyproject.toml
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-08-07 07:12:37.067546 pyunitsystem-1.0.0/pyunitsystem/
+-rw-r--r--   0 payno     (1000) payno     (1000)      299 2023-08-07 07:12:22.000000 pyunitsystem-1.0.0/pyunitsystem/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1058 2023-08-07 06:19:59.000000 pyunitsystem-1.0.0/pyunitsystem/electriccurrentsystem.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1890 2023-08-07 06:32:45.000000 pyunitsystem-1.0.0/pyunitsystem/energysystem.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1953 2023-08-07 06:19:59.000000 pyunitsystem-1.0.0/pyunitsystem/metricsystem.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-08-07 07:12:37.067546 pyunitsystem-1.0.0/pyunitsystem/test/
+-rw-r--r--   0 payno     (1000) payno     (1000)     3367 2023-08-07 06:37:37.000000 pyunitsystem-1.0.0/pyunitsystem/test/test_unitsystem.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1771 2023-08-07 06:19:59.000000 pyunitsystem-1.0.0/pyunitsystem/timesystem.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1633 2023-08-07 06:37:46.000000 pyunitsystem-1.0.0/pyunitsystem/unit.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      581 2023-08-07 06:19:59.000000 pyunitsystem-1.0.0/pyunitsystem/voltagesystem.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-08-07 07:12:37.067546 pyunitsystem-1.0.0/pyunitsystem.egg-info/
+-rw-r--r--   0 payno     (1000) payno     (1000)     2928 2023-08-07 07:12:37.000000 pyunitsystem-1.0.0/pyunitsystem.egg-info/PKG-INFO
+-rw-r--r--   0 payno     (1000) payno     (1000)      456 2023-08-07 07:12:37.000000 pyunitsystem-1.0.0/pyunitsystem.egg-info/SOURCES.txt
+-rw-r--r--   0 payno     (1000) payno     (1000)        1 2023-08-07 07:12:37.000000 pyunitsystem-1.0.0/pyunitsystem.egg-info/dependency_links.txt
+-rw-r--r--   0 payno     (1000) payno     (1000)       26 2023-08-07 07:12:37.000000 pyunitsystem-1.0.0/pyunitsystem.egg-info/requires.txt
+-rw-r--r--   0 payno     (1000) payno     (1000)       13 2023-08-07 07:12:37.000000 pyunitsystem-1.0.0/pyunitsystem.egg-info/top_level.txt
+-rw-r--r--   0 payno     (1000) payno     (1000)       38 2023-08-07 07:12:37.067546 pyunitsystem-1.0.0/setup.cfg
+-rw-r--r--   0 payno     (1000) payno     (1000)       38 2023-08-07 06:19:59.000000 pyunitsystem-1.0.0/setup.py
```

### Comparing `pyunitsystem-0.1.0/LICENSE` & `pyunitsystem-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyunitsystem-0.1.0/PKG-INFO` & `pyunitsystem-1.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyunitsystem
-Version: 0.1.0
+Version: 1.0.0
 Summary: dummy unit system
 Author-email: Henri Payno <henri.payno@esrf.fr>, Pierre Paleo <pierre.paleo@esrf.fr>, Alessandro Mirone <mirone@esrf.fr>, Jérôme Lesaint <jerome.lesaint@esrf.fr>
 License: 
         The pyunitsystem library goal is to provide a unit system.
         
         nxtomo is distributed under the MIT license.
         
@@ -48,12 +48,13 @@
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
+Provides-Extra: test
 License-File: LICENSE
 
 # pyunitsystem
 
 dummy low level  unit system
```

### Comparing `pyunitsystem-0.1.0/pyproject.toml` & `pyunitsystem-1.0.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -44,7 +44,13 @@
 [tool.setuptools.dynamic]
 version = {attr = "pyunitsystem.version"}
 readme = {file = ["README.md"]}
 
 
 [tool.setuptools.packages.find]
 where = ["."]  # list of folders that contain the packages (["."] by default)
+
+[project.optional-dependencies]
+test = [
+  "pytest",
+  "pytest-cov",
+]
```

### Comparing `pyunitsystem-0.1.0/pyunitsystem/electriccurrentsystem.py` & `pyunitsystem-1.0.0/pyunitsystem/electriccurrentsystem.py`

 * *Files identical despite different names*

### Comparing `pyunitsystem-0.1.0/pyunitsystem/energysystem.py` & `pyunitsystem-1.0.0/pyunitsystem/energysystem.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,9 +48,10 @@
         elif self is EnergySI.KILOELECTRONVOLT:
             return "keV"
         elif self is EnergySI.MEGAELECTRONVOLT:
             return "meV"
         elif self is EnergySI.GIGAELECTRONVOLT:
             return "geV"
         elif self is EnergySI.ELEMCHARGE:
-            # in fact will never be called because EnergySI.ELEMCHARGE is EnergySI.ELECTRONVOLT
+            # in fact will never be called because
+            # EnergySI.ELEMCHARGE is EnergySI.ELECTRONVOLT
             return "e"
```

### Comparing `pyunitsystem-0.1.0/pyunitsystem/metricsystem.py` & `pyunitsystem-1.0.0/pyunitsystem/metricsystem.py`

 * *Files identical despite different names*

### Comparing `pyunitsystem-0.1.0/pyunitsystem/test/test_unitsystem.py` & `pyunitsystem-1.0.0/pyunitsystem/test/test_unitsystem.py`

 * *Files 13% similar despite different names*

```diff
@@ -23,15 +23,18 @@
     assert (
         EnergySI.from_str(energy_as_str) is energy_as_si
     ), f"check {energy_as_str} == {energy_as_si}"
     assert str(energy_as_si) == energy_as_str
 
 
 def test_failing_energy_conversion():
-    """Insure EnergySI.from_str raise a ValueErrror if cannot convert a string to an energy"""
+    """
+    Ensure EnergySI.from_str raise a ValueErrror if cannot convert
+    a string to an energy
+    """
     with pytest.raises(ValueError):
         EnergySI.from_str("toto")
 
 
 def test_from_value():
     assert EnergySI.from_value(EnergySI.JOULE.value) is EnergySI.JOULE
 
@@ -55,15 +58,18 @@
     ), f"check {metric_as_str} == {metric_as_si}"
     assert str(metric_as_si) == str(
         MetricSystem.from_str(metric_as_str)
     ), f"check {metric_as_str} == {str(metric_as_si)}"
 
 
 def test_failing_metric_conversion():
-    """Insure MetricSystem.from_str raise a ValueErrror if cannot convert a string to an energy"""
+    """
+    Ensure MetricSystem.from_str raise a ValueErrror if cannot convert
+    a string to a metric
+    """
     with pytest.raises(ValueError):
         MetricSystem.from_str("toto")
 
 
 expected_time_conversion = {
     "second": TimeSystem.SECOND,
     "minute": TimeSystem.MINUTE,
@@ -71,36 +77,43 @@
     "day": TimeSystem.DAY,
     "millisecond": TimeSystem.MILLI_SECOND,
     "microsecond": TimeSystem.MICRO_SECOND,
     "nanosecond": TimeSystem.NANO_SECOND,
 }
 
 
-@pytest.mark.parametrize("time_as_str, time_as_si", expected_time_conversion.items())
+@pytest.mark.parametrize(
+    "time_as_str, time_as_si", expected_time_conversion.items()
+)  # noqa E501
 def test_time_conversion(time_as_str, time_as_si):
     assert (
         TimeSystem.from_str(time_as_str) is time_as_si
     ), f"check {time_as_str} == {time_as_si}"
     assert str(time_as_si) == str(
         TimeSystem.from_str(time_as_str)
     ), f"check {time_as_str} == {str(time_as_si)}"
 
 
 def test_failing_voltage_conversion():
-    """Insure VoltageSystem.from_str raise a ValueErrror if cannot convert a string to an energy"""
+    """
+    Ensure VoltageSystem.from_str raise a ValueErrror if cannot convert
+    a string to a voltage
+    """
     with pytest.raises(ValueError):
         VoltageSystem.from_str("toto")
 
 
 expected_voltage_conversion = {
     "volt": VoltageSystem.VOLT,
 }
 
 
-@pytest.mark.parametrize("volt_as_str, volt_as_si", expected_voltage_conversion.items())
+@pytest.mark.parametrize(
+    "volt_as_str, volt_as_si", expected_voltage_conversion.items()
+)  # noqa E501
 def test_voltage_conversion(volt_as_str, volt_as_si):
     assert (
         VoltageSystem.from_str(volt_as_str) is volt_as_si
     ), f"check {volt_as_str} == {volt_as_si}"
     assert str(volt_as_si) == str(
         VoltageSystem.from_str(volt_as_str)
     ), f"check {volt_as_str} == {str(volt_as_si)}"
```

### Comparing `pyunitsystem-0.1.0/pyunitsystem/timesystem.py` & `pyunitsystem-1.0.0/pyunitsystem/timesystem.py`

 * *Files identical despite different names*

### Comparing `pyunitsystem-0.1.0/pyunitsystem/unit.py` & `pyunitsystem-1.0.0/pyunitsystem/unit.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 import enum
 
 
 class _Enum(enum.Enum):
     """Enum with additional class methods."""
 
     @classmethod
@@ -43,17 +42,19 @@
         """Returns a tuple of all member values.
 
         :rtype: Tuple
         """
         return tuple(member.value for member in cls)
 
 
-
 class Unit(_Enum):
-    """Base class for all Unit. Children class are also expected to inherit from silx Enum class"""
+    """
+    Base class for all Unit.
+    Children class are also expected to inherit from silx Enum class
+    """
 
     @classmethod
     def from_str(cls, value: str):
         raise NotImplementedError("Base class")
 
     @classmethod
     def from_value(cls, value):
```

### Comparing `pyunitsystem-0.1.0/pyunitsystem/voltagesystem.py` & `pyunitsystem-1.0.0/pyunitsystem/voltagesystem.py`

 * *Files identical despite different names*

### Comparing `pyunitsystem-0.1.0/pyunitsystem.egg-info/PKG-INFO` & `pyunitsystem-1.0.0/pyunitsystem.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyunitsystem
-Version: 0.1.0
+Version: 1.0.0
 Summary: dummy unit system
 Author-email: Henri Payno <henri.payno@esrf.fr>, Pierre Paleo <pierre.paleo@esrf.fr>, Alessandro Mirone <mirone@esrf.fr>, Jérôme Lesaint <jerome.lesaint@esrf.fr>
 License: 
         The pyunitsystem library goal is to provide a unit system.
         
         nxtomo is distributed under the MIT license.
         
@@ -48,12 +48,13 @@
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
+Provides-Extra: test
 License-File: LICENSE
 
 # pyunitsystem
 
 dummy low level  unit system
```

