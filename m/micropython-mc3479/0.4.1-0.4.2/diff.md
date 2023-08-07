# Comparing `tmp/micropython-mc3479-0.4.1.tar.gz` & `tmp/micropython-mc3479-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropython-mc3479-0.4.1.tar", last modified: Sat Jun 17 14:59:10 2023, max compression
+gzip compressed data, was "micropython-mc3479-0.4.2.tar", last modified: Mon Aug  7 13:39:10 2023, max compression
```

## Comparing `micropython-mc3479-0.4.1.tar` & `micropython-mc3479-0.4.2.tar`

### file list

```diff
@@ -1,45 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:59:10.721902 micropython-mc3479-0.4.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:59:10.709901 micropython-mc3479-0.4.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:59:10.713901 micropython-mc3479-0.4.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-17 14:58:55.000000 micropython-mc3479-0.4.1/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-17 14:58:55.000000 micropython-mc3479-0.4.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-17 14:58:55.000000 micropython-mc3479-0.4.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-06-17 14:58:55.000000 micropython-mc3479-0.4.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-17 14:58:55.000000 micropython-mc3479-0.4.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-17 14:58:55.000000 micropython-mc3479-0.4.1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:59:10.713901 micropython-mc3479-0.4.1/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-06-17 14:58:55.000000 micropython-mc3479-0.4.1/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-17 14:58:55.000000 micropython-mc3479-0.4.1/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-17 14:58:55.000000 micropython-mc3479-0.4.1/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-06-17 14:59:10.721902 micropython-mc3479-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-06-17 14:58:55.000000 micropython-mc3479-0.4.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:59:10.717901 micropython-mc3479-0.4.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:59:10.717901 micropython-mc3479-0.4.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-17 14:58:55.000000 micropython-mc3479-0.4.1/docs/_static/Logo.png
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-17 14:58:55.000000 micropython-mc3479-0.4.1/docs/_static/extra_css.css
--rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-06-17 14:58:55.000000 micropython-mc3479-0.4.1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 14:58:55.000000 micropython-mc3479-0.4.1/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-17 14:58:55.000000 micropython-mc3479-0.4.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-06-17 14:58:55.000000 micropython-mc3479-0.4.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-17 14:58:55.000000 micropython-mc3479-0.4.1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-17 14:58:55.000000 micropython-mc3479-0.4.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 14:58:55.000000 micropython-mc3479-0.4.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:59:10.717901 micropython-mc3479-0.4.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-06-17 14:59:03.000000 micropython-mc3479-0.4.1/examples/mc3479_acceleration_range.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-06-17 14:59:03.000000 micropython-mc3479-0.4.1/examples/mc3479_datarate.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-17 14:59:03.000000 micropython-mc3479-0.4.1/examples/mc3479_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-17 14:58:55.000000 micropython-mc3479-0.4.1/examples.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:59:10.717901 micropython-mc3479-0.4.1/micropython_mc3479/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 14:59:03.000000 micropython-mc3479-0.4.1/micropython_mc3479/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-06-17 14:59:03.000000 micropython-mc3479-0.4.1/micropython_mc3479/i2c_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12626 2023-06-17 14:59:03.000000 micropython-mc3479-0.4.1/micropython_mc3479/mc3479.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:59:10.721902 micropython-mc3479-0.4.1/micropython_mc3479.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-06-17 14:59:10.000000 micropython-mc3479-0.4.1/micropython_mc3479.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-17 14:59:10.000000 micropython-mc3479-0.4.1/micropython_mc3479.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 14:59:10.000000 micropython-mc3479-0.4.1/micropython_mc3479.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-17 14:59:10.000000 micropython-mc3479-0.4.1/micropython_mc3479.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-17 14:59:10.000000 micropython-mc3479-0.4.1/micropython_mc3479.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-17 14:58:55.000000 micropython-mc3479-0.4.1/packages.json
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-17 14:59:03.000000 micropython-mc3479-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-17 14:58:55.000000 micropython-mc3479-0.4.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 14:59:10.721902 micropython-mc3479-0.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:39:10.547207 micropython-mc3479-0.4.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:39:10.539207 micropython-mc3479-0.4.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:39:10.543207 micropython-mc3479-0.4.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-08-07 13:38:55.000000 micropython-mc3479-0.4.2/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-08-07 13:38:55.000000 micropython-mc3479-0.4.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-08-07 13:38:55.000000 micropython-mc3479-0.4.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-08-07 13:38:55.000000 micropython-mc3479-0.4.2/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-08-07 13:38:55.000000 micropython-mc3479-0.4.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-08-07 13:38:55.000000 micropython-mc3479-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-08-07 13:39:10.547207 micropython-mc3479-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-08-07 13:38:55.000000 micropython-mc3479-0.4.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:39:10.543207 micropython-mc3479-0.4.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:39:10.543207 micropython-mc3479-0.4.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-08-07 13:38:55.000000 micropython-mc3479-0.4.2/docs/_static/Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-08-07 13:38:55.000000 micropython-mc3479-0.4.2/docs/_static/extra_css.css
+-rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-08-07 13:38:55.000000 micropython-mc3479-0.4.2/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-08-07 13:38:55.000000 micropython-mc3479-0.4.2/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-08-07 13:38:55.000000 micropython-mc3479-0.4.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-08-07 13:38:55.000000 micropython-mc3479-0.4.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-08-07 13:38:55.000000 micropython-mc3479-0.4.2/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-08-07 13:38:55.000000 micropython-mc3479-0.4.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-08-07 13:38:55.000000 micropython-mc3479-0.4.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:39:10.543207 micropython-mc3479-0.4.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-08-07 13:39:03.000000 micropython-mc3479-0.4.2/examples/mc3479_acceleration_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-08-07 13:39:03.000000 micropython-mc3479-0.4.2/examples/mc3479_datarate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-08-07 13:39:03.000000 micropython-mc3479-0.4.2/examples/mc3479_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-08-07 13:38:55.000000 micropython-mc3479-0.4.2/examples.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:39:10.543207 micropython-mc3479-0.4.2/micropython_mc3479/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 13:39:03.000000 micropython-mc3479-0.4.2/micropython_mc3479/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-08-07 13:39:03.000000 micropython-mc3479-0.4.2/micropython_mc3479/i2c_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13385 2023-08-07 13:39:03.000000 micropython-mc3479-0.4.2/micropython_mc3479/mc3479.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:39:10.547207 micropython-mc3479-0.4.2/micropython_mc3479.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-08-07 13:39:10.000000 micropython-mc3479-0.4.2/micropython_mc3479.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-08-07 13:39:10.000000 micropython-mc3479-0.4.2/micropython_mc3479.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 13:39:10.000000 micropython-mc3479-0.4.2/micropython_mc3479.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-07 13:39:10.000000 micropython-mc3479-0.4.2/micropython_mc3479.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-08-07 13:38:55.000000 micropython-mc3479-0.4.2/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-08-07 13:39:03.000000 micropython-mc3479-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-07 13:38:55.000000 micropython-mc3479-0.4.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 13:39:10.547207 micropython-mc3479-0.4.2/setup.cfg
```

### Comparing `micropython-mc3479-0.4.1/.pre-commit-config.yaml` & `micropython-mc3479-0.4.2/.pre-commit-config.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,31 @@
-# SPDX-FileCopyrightText: 2020 Diego Elio Pettenò
+# SPDX-FileCopyrightText: 2023 Jose D. Montoya
 #
 # SPDX-License-Identifier: Unlicense
 
 repos:
   - repo: https://github.com/python/black
-    rev: 22.3.0
+    rev: 23.3.0
     hooks:
       - id: black
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.2.0
+    rev: v4.4.0
     hooks:
       - id: check-yaml
       - id: end-of-file-fixer
       - id: trailing-whitespace
   - repo: https://github.com/pycqa/pylint
-    rev: v2.15.5
+    rev: v2.17.4
     hooks:
       - id: pylint
         name: pylint (library code)
         types: [python]
         args:
           - --disable=consider-using-f-string
-        exclude: "^(docs/|examples/|tests/|setup.py$)"
+        exclude: "^(docs/|examples/|tests/)"
       - id: pylint
         name: pylint (example code)
         description: Run pylint rules on "examples/*.py" files
         types: [python]
         files: "^examples/"
         args:
           - --disable=missing-docstring,invalid-name,consider-using-f-string,duplicate-code
-      - id: pylint
-        name: pylint (test code)
-        description: Run pylint rules on "tests/*.py" files
-        types: [python]
-        files: "^tests/"
-        args:
-          - --disable=missing-docstring,consider-using-f-string,duplicate-code
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `micropython-mc3479-0.4.1/.pylintrc` & `micropython-mc3479-0.4.2/.pylintrc`

 * *Files identical despite different names*

### Comparing `micropython-mc3479-0.4.1/LICENSE` & `micropython-mc3479-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `micropython-mc3479-0.4.1/PKG-INFO` & `micropython-mc3479-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micropython-mc3479
-Version: 0.4.1
+Version: 0.4.2
 Summary: MicroPython Driver for the MC3479 Accelerometer
 Author-email: "Jose D. Montoya" <mc3479@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_MC3479
 Keywords: micropython,mc3479,MicroPython,MC3479,accelerometer,sensor,acceleration
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `micropython-mc3479-0.4.1/README.rst` & `micropython-mc3479-0.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `micropython-mc3479-0.4.1/docs/_static/Logo.png` & `micropython-mc3479-0.4.2/docs/_static/Logo.png`

 * *Files identical despite different names*

### Comparing `micropython-mc3479-0.4.1/docs/_static/favicon.ico` & `micropython-mc3479-0.4.2/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `micropython-mc3479-0.4.1/docs/examples.rst` & `micropython-mc3479-0.4.2/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `micropython-mc3479-0.4.1/examples/mc3479_acceleration_range.py` & `micropython-mc3479-0.4.2/examples/mc3479_acceleration_range.py`

 * *Files identical despite different names*

### Comparing `micropython-mc3479-0.4.1/examples/mc3479_datarate.py` & `micropython-mc3479-0.4.2/examples/mc3479_datarate.py`

 * *Files identical despite different names*

### Comparing `micropython-mc3479-0.4.1/micropython_mc3479/i2c_helpers.py` & `micropython-mc3479-0.4.2/micropython_mc3479/i2c_helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,18 +34,15 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 
 """
 # pylint: disable=too-many-arguments
-try:
-    import struct
-except ImportError:
-    import ustruct as struct
+import struct
 
 
 class CBits:
     """
     Changes bits from a byte register
     """
 
@@ -64,30 +61,28 @@
         self.lsb_first = lsb_first
 
     def __get__(
         self,
         obj,
         objtype=None,
     ) -> int:
-
         mem_value = obj._i2c.readfrom_mem(obj._address, self.register, self.lenght)
 
         reg = 0
         order = range(len(mem_value) - 1, -1, -1)
         if not self.lsb_first:
             order = reversed(order)
         for i in order:
             reg = (reg << 8) | mem_value[i]
 
         reg = (reg & self.bit_mask) >> self.star_bit
 
         return reg
 
     def __set__(self, obj, value: int) -> None:
-
         memory_value = obj._i2c.readfrom_mem(obj._address, self.register, self.lenght)
 
         reg = 0
         order = range(len(memory_value) - 1, -1, -1)
         if not self.lsb_first:
             order = range(0, len(memory_value))
         for i in order:
@@ -112,15 +107,14 @@
         self.lenght = struct.calcsize(form)
 
     def __get__(
         self,
         obj,
         objtype=None,
     ):
-
         if self.lenght <= 2:
             value = struct.unpack(
                 self.format,
                 memoryview(
                     obj._i2c.readfrom_mem(obj._address, self.register, self.lenght)
                 ),
             )[0]
```

### Comparing `micropython-mc3479-0.4.1/micropython_mc3479/mc3479.py` & `micropython-mc3479-0.4.2/micropython_mc3479/mc3479.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,18 +12,22 @@
 
 
 """
 
 from micropython import const
 from micropython_mc3479.i2c_helpers import CBits, RegisterStruct
 
-__version__ = "0.4.1"
+try:
+    from typing import Tuple
+except ImportError:
+    pass
+
+__version__ = "0.4.2"
 __repo__ = "https://github.com/jposada202020/MicroPython_MC3479.git"
 
-_I2C_ADDR = const(0x4C)
 _REG_WHOAMI = const(0x98)
 _SENSOR_STATUS_REG = const(0x05)
 _MODE_REG = const(0x07)
 _ACC_RANGE = const(0x20)
 _ACC_DATA_RATE = const(0x08)
 
 # Acceleration Data
@@ -120,25 +124,25 @@
     # Acceleration Range Conf (0x20)
     _acc_range = CBits(3, _ACC_RANGE, 4)
     _acc_lpf_en = CBits(1, _ACC_RANGE, 3)
     _acc_lpf_setting = CBits(3, _ACC_RANGE, 0)
 
     acceleration_scale = {0: 16384, 1: 8192, 2: 4096, 3: 2048, 4: 2730}
 
-    def __init__(self, i2c, address: int = _I2C_ADDR):
+    def __init__(self, i2c, address: int = 0x4C) -> None:
         self._i2c = i2c
         self._address = address
 
         if self._device_id != 0xA4:
             raise RuntimeError("Failed to find MC3479")
 
         self._mode = NORMAL
 
     @property
-    def acceleration(self):
+    def acceleration(self) -> Tuple[float, float, float]:
         """
         The device has the ability to read all sampled readings
         in a continuous sampling fashion. The device always updates
         the XOUT, YOUT, and ZOUT registers at the chosen output data rate
 
         X, Y, and Z-axis accelerometer measurements are in 16-bit, signed
         2’s complement format. Register addresses 0x0D to 0x12 hold the
@@ -183,22 +187,23 @@
         | :py:const:`MC3479.STANDBY`             | :py:const:`0`           |
         +----------------------------------------+-------------------------+
         | :py:const:`MC3479.NORMAL`              | :py:const:`1`           |
         +----------------------------------------+-------------------------+
 
 
         """
-        return self._mode
+        values = ("STANDBY", "NORMAL")
+        return values[self._mode]
 
     @sensor_mode.setter
-    def sensor_mode(self, value: int):
+    def sensor_mode(self, value: int) -> None:
         self._mode = value
 
     @property
-    def acceleration_range(self) -> int:
+    def acceleration_range(self) -> str:
         """
         The range and scale control register sets the resolution, range,
         and filtering options for the accelerometer. All values are in
         sign-extended 2’s complement format. Values are reported in
         registers 0x0D – 0x12 (the hardware formats the output)
 
         +----------------------------------------+-------------------------+
@@ -221,24 +226,31 @@
         .. code-block:: python
 
             i2c = I2C(sda=Pin(8), scl=Pin(9))  # Correct I2C pins for UM FeatherS2
             mc3479 = MC3479.MC3479(i2c)
             mc3479.acceleration_range = MC3479.ACCEL_RANGE_12G
 
         """
-        return self._acc_range
+        values = (
+            "ACCEL_RANGE_2G",
+            "ACCEL_RANGE_4G",
+            "ACCEL_RANGE_8G",
+            "ACCEL_RANGE_16G",
+            "ACCEL_RANGE_12G",
+        )
+        return values[self._acc_range]
 
     @acceleration_range.setter
-    def acceleration_range(self, value: int):
+    def acceleration_range(self, value: int) -> None:
         self._mode = STANDBY
         self._acc_range = value
         self._mode = NORMAL
 
     @property
-    def lpf_enabled(self) -> int:
+    def lpf_enabled(self) -> str:
         """
         Low Power Filter Enabler
 
         +----------------------------------------+-------------------------+
         | Mode                                   | Value                   |
         +========================================+=========================+
         | :py:const:`MC3479.LPF_ENABLE`          | :py:const:`0b0`         |
@@ -252,24 +264,25 @@
         .. code-block:: python
 
             i2c = I2C(sda=Pin(8), scl=Pin(9))  # Correct I2C pins for UM FeatherS2
             mc3479 = MC3479.MC3479(i2c)
             mc3479.lpf_enabled = MC3479.LPF_ENABLE
 
         """
-        return self._acc_lpf_en
+        values = ("LPF_DISABLE", "LPF_ENABLE")
+        return values[self._acc_lpf_en]
 
     @lpf_enabled.setter
-    def lpf_enabled(self, value: int):
+    def lpf_enabled(self, value: int) -> None:
         self._mode = STANDBY
         self._acc_lpf_en = value
         self._mode = NORMAL
 
     @property
-    def lpf_setting(self) -> int:
+    def lpf_setting(self) -> str:
         """
         Selects the Bandwidth for the Low Power Filter. Depends on the selection
         of the ODR/IDR
 
         +--------------------------------+------------------------------------+
         | Mode                           | Value                              |
         +================================+====================================+
@@ -289,24 +302,25 @@
 
             i2c = I2C(sda=Pin(8), scl=Pin(9))  # Correct I2C pins for UM FeatherS2
             mc3479 = MC3479.MC3479(i2c)
 
             mc3479.lpf_setting = MC3479.BANDWIDTH_5
 
         """
-        return self._acc_lpf_setting
+        values = ("BANDWIDTH_1", "BANDWIDTH_2", "BANDWIDTH_3", "BANDWIDTH_5")
+        return values[self._acc_lpf_setting]
 
     @lpf_setting.setter
-    def lpf_setting(self, value: int):
+    def lpf_setting(self, value: int) -> None:
         self._mode = STANDBY
         self._acc_lpf_setting = value
         self._mode = NORMAL
 
     @property
-    def acceleration_output_data_rate(self) -> int:
+    def acceleration_output_data_rate(self) -> str:
         """
         Define the output data rate in Hz
         The output data rate is dependent of the power mode setting for the sensor
 
         +----------------------------------------+---------------------------------+
         | Mode                                   | Value                           |
         +========================================+=================================+
@@ -333,14 +347,24 @@
         .. code-block:: python
 
             i2c = I2C(sda=Pin(8), scl=Pin(9))  # Correct I2C pins for UM FeatherS2
             mc3479 = MC3479.MC3479(i2c)
             mc3479.acceleration_output_data_rate = MC3479.BANDWIDTH_500
 
         """
-        return self._data_rate
+        values = (
+            "BANDWIDTH_25",
+            "BANDWIDTH_50",
+            "BANDWIDTH_62_5",
+            "BANDWIDTH_100",
+            "BANDWIDTH_125",
+            "BANDWIDTH_250",
+            "BANDWIDTH_500",
+            "BANDWIDTH_1000",
+        )
+        return values[self._data_rate]
 
     @acceleration_output_data_rate.setter
-    def acceleration_output_data_rate(self, value: int):
+    def acceleration_output_data_rate(self, value: int) -> None:
         self._mode = STANDBY
         self._data_rate = value
         self._mode = NORMAL
```

### Comparing `micropython-mc3479-0.4.1/micropython_mc3479.egg-info/PKG-INFO` & `micropython-mc3479-0.4.2/micropython_mc3479.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micropython-mc3479
-Version: 0.4.1
+Version: 0.4.2
 Summary: MicroPython Driver for the MC3479 Accelerometer
 Author-email: "Jose D. Montoya" <mc3479@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_MC3479
 Keywords: micropython,mc3479,MicroPython,MC3479,accelerometer,sensor,acceleration
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `micropython-mc3479-0.4.1/micropython_mc3479.egg-info/SOURCES.txt` & `micropython-mc3479-0.4.2/micropython_mc3479.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 .gitignore
 .pre-commit-config.yaml
 .pylintrc
 .readthedocs.yaml
 LICENSE
 README.rst
 examples.json
-packages.json
+package.json
 pyproject.toml
 requirements.txt
 .github/workflows/release_pypi.yml
-LICENSES/CC-BY-4.0.txt
-LICENSES/MIT.txt
-LICENSES/Unlicense.txt
 docs/api.rst
 docs/conf.py
 docs/examples.rst
 docs/index.rst
 docs/requirements.txt
 docs/_static/Logo.png
 docs/_static/extra_css.css
@@ -26,9 +23,8 @@
 examples/mc3479_simpletest.py
 micropython_mc3479/__init__.py
 micropython_mc3479/i2c_helpers.py
 micropython_mc3479/mc3479.py
 micropython_mc3479.egg-info/PKG-INFO
 micropython_mc3479.egg-info/SOURCES.txt
 micropython_mc3479.egg-info/dependency_links.txt
-micropython_mc3479.egg-info/requires.txt
 micropython_mc3479.egg-info/top_level.txt
```

### Comparing `micropython-mc3479-0.4.1/pyproject.toml` & `micropython-mc3479-0.4.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "micropython-mc3479"
 description = "MicroPython Driver for the MC3479 Accelerometer"
-version = "0.4.1"
+version = "0.4.2"
 readme = "README.rst"
 authors = [
     {name = "Jose D. Montoya", email = "mc3479@mailmeto.mozmail.com"}
 ]
 urls = {Homepage = "https://github.com/jposada202020/MicroPython_MC3479"}
 keywords = [
     "micropython",
```

