# Comparing `tmp/micropython-ds1841-0.1.1.tar.gz` & `tmp/micropython-ds1841-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropython-ds1841-0.1.1.tar", last modified: Sat Jun 17 14:19:26 2023, max compression
+gzip compressed data, was "micropython-ds1841-0.1.2.tar", last modified: Mon Aug  7 13:48:16 2023, max compression
```

## Comparing `micropython-ds1841-0.1.1.tar` & `micropython-ds1841-0.1.2.tar`

### file list

```diff
@@ -1,41 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:19:26.041051 micropython-ds1841-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:19:26.037050 micropython-ds1841-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:19:26.041051 micropython-ds1841-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-17 14:19:10.000000 micropython-ds1841-0.1.1/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-17 14:19:10.000000 micropython-ds1841-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-17 14:19:10.000000 micropython-ds1841-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-06-17 14:19:10.000000 micropython-ds1841-0.1.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-17 14:19:10.000000 micropython-ds1841-0.1.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-17 14:19:10.000000 micropython-ds1841-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-06-17 14:19:26.041051 micropython-ds1841-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-06-17 14:19:10.000000 micropython-ds1841-0.1.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:19:26.041051 micropython-ds1841-0.1.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:19:26.041051 micropython-ds1841-0.1.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-17 14:19:10.000000 micropython-ds1841-0.1.1/docs/_static/Logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-17 14:19:10.000000 micropython-ds1841-0.1.1/docs/_static/Logo.png.license
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-17 14:19:10.000000 micropython-ds1841-0.1.1/docs/_static/extra_css.css
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-17 14:19:10.000000 micropython-ds1841-0.1.1/docs/_static/extra_css.css.license
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-17 14:19:10.000000 micropython-ds1841-0.1.1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 14:19:10.000000 micropython-ds1841-0.1.1/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-17 14:19:10.000000 micropython-ds1841-0.1.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-06-17 14:19:10.000000 micropython-ds1841-0.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-17 14:19:10.000000 micropython-ds1841-0.1.1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-17 14:19:10.000000 micropython-ds1841-0.1.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 14:19:10.000000 micropython-ds1841-0.1.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:19:26.041051 micropython-ds1841-0.1.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-17 14:19:18.000000 micropython-ds1841-0.1.1/examples/ds1841_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-17 14:19:10.000000 micropython-ds1841-0.1.1/examples.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:19:26.041051 micropython-ds1841-0.1.1/micropython_ds1841/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 14:19:18.000000 micropython-ds1841-0.1.1/micropython_ds1841/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-06-17 14:19:18.000000 micropython-ds1841-0.1.1/micropython_ds1841/ds1841.py
--rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-06-17 14:19:18.000000 micropython-ds1841-0.1.1/micropython_ds1841/i2c_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:19:26.041051 micropython-ds1841-0.1.1/micropython_ds1841.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-06-17 14:19:26.000000 micropython-ds1841-0.1.1/micropython_ds1841.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-17 14:19:26.000000 micropython-ds1841-0.1.1/micropython_ds1841.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 14:19:26.000000 micropython-ds1841-0.1.1/micropython_ds1841.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-17 14:19:26.000000 micropython-ds1841-0.1.1/micropython_ds1841.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-17 14:19:26.000000 micropython-ds1841-0.1.1/micropython_ds1841.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-17 14:19:10.000000 micropython-ds1841-0.1.1/package.json
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-17 14:19:18.000000 micropython-ds1841-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-17 14:19:10.000000 micropython-ds1841-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 14:19:26.041051 micropython-ds1841-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:48:16.414621 micropython-ds1841-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:48:16.406620 micropython-ds1841-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:48:16.410621 micropython-ds1841-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-08-07 13:47:54.000000 micropython-ds1841-0.1.2/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-08-07 13:47:54.000000 micropython-ds1841-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-08-07 13:47:54.000000 micropython-ds1841-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-08-07 13:47:54.000000 micropython-ds1841-0.1.2/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-08-07 13:47:54.000000 micropython-ds1841-0.1.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-08-07 13:47:54.000000 micropython-ds1841-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-08-07 13:48:16.414621 micropython-ds1841-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-08-07 13:47:54.000000 micropython-ds1841-0.1.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:48:16.410621 micropython-ds1841-0.1.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:48:16.414621 micropython-ds1841-0.1.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-08-07 13:47:54.000000 micropython-ds1841-0.1.2/docs/_static/Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-08-07 13:47:54.000000 micropython-ds1841-0.1.2/docs/_static/Logo.png.license
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-08-07 13:47:54.000000 micropython-ds1841-0.1.2/docs/_static/extra_css.css
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-08-07 13:47:54.000000 micropython-ds1841-0.1.2/docs/_static/extra_css.css.license
+-rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-08-07 13:47:54.000000 micropython-ds1841-0.1.2/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-08-07 13:47:54.000000 micropython-ds1841-0.1.2/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-08-07 13:47:54.000000 micropython-ds1841-0.1.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5054 2023-08-07 13:47:54.000000 micropython-ds1841-0.1.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-08-07 13:47:54.000000 micropython-ds1841-0.1.2/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-08-07 13:47:54.000000 micropython-ds1841-0.1.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-08-07 13:47:54.000000 micropython-ds1841-0.1.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:48:16.414621 micropython-ds1841-0.1.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-08-07 13:48:06.000000 micropython-ds1841-0.1.2/examples/ds1841_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-08-07 13:47:54.000000 micropython-ds1841-0.1.2/examples.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:48:16.414621 micropython-ds1841-0.1.2/micropython_ds1841/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 13:48:06.000000 micropython-ds1841-0.1.2/micropython_ds1841/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-08-07 13:48:06.000000 micropython-ds1841-0.1.2/micropython_ds1841/ds1841.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-08-07 13:48:06.000000 micropython-ds1841-0.1.2/micropython_ds1841/i2c_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:48:16.414621 micropython-ds1841-0.1.2/micropython_ds1841.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-08-07 13:48:16.000000 micropython-ds1841-0.1.2/micropython_ds1841.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-08-07 13:48:16.000000 micropython-ds1841-0.1.2/micropython_ds1841.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 13:48:16.000000 micropython-ds1841-0.1.2/micropython_ds1841.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-07 13:48:16.000000 micropython-ds1841-0.1.2/micropython_ds1841.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-08-07 13:47:54.000000 micropython-ds1841-0.1.2/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-08-07 13:48:06.000000 micropython-ds1841-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-07 13:47:54.000000 micropython-ds1841-0.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 13:48:16.414621 micropython-ds1841-0.1.2/setup.cfg
```

### Comparing `micropython-ds1841-0.1.1/.pre-commit-config.yaml` & `micropython-ds1841-0.1.2/.pre-commit-config.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,31 @@
 # SPDX-FileCopyrightText: 2023 Jose D. Montoya
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

### Comparing `micropython-ds1841-0.1.1/.pylintrc` & `micropython-ds1841-0.1.2/.pylintrc`

 * *Files identical despite different names*

### Comparing `micropython-ds1841-0.1.1/LICENSE` & `micropython-ds1841-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `micropython-ds1841-0.1.1/PKG-INFO` & `micropython-ds1841-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: micropython-ds1841
-Version: 0.1.1
+Version: 0.1.2
 Summary: MicroPython Driver for the DS1841 Potentiometer
 Author-email: JDM <xxyx@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_DS1841
-Keywords: sensor,micropython,ds1841,micropython,driver,ds1841,potentiometer,analog,devices,resistance
+Keywords: sensor,micropython,ds1841,driver,ds1841,potentiometer,analog,devices,resistance
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: Implementation :: MicroPython
 Description-Content-Type: text/x-rst
```

### Comparing `micropython-ds1841-0.1.1/README.rst` & `micropython-ds1841-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `micropython-ds1841-0.1.1/docs/_static/Logo.png` & `micropython-ds1841-0.1.2/docs/_static/Logo.png`

 * *Files identical despite different names*

### Comparing `micropython-ds1841-0.1.1/examples/ds1841_simpletest.py` & `micropython-ds1841-0.1.2/examples/ds1841_simpletest.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,34 +9,33 @@
 
 i2c = I2C(1, sda=Pin(2), scl=Pin(3))  # Correct I2C pins for RP2040
 ds1841 = ds1841.DS1841(i2c)
 
 wiper_output = ADC(Pin(26, mode=Pin.IN))
 
 while True:
-    # set th
     ds1841.wiper = 127
-    print("Wiper set to %d" % ds1841.wiper)
+    print(f"Wiper set to {ds1841.wiper}")
     voltage = wiper_output.read_u16()
     voltage *= 3.3
     voltage /= 65535
-    print("Wiper voltage: %.2f V" % voltage)
+    print(f"Wiper voltage {voltage::.2%}V")
     print("")
     sleep(1.0)
 
     ds1841.wiper = 0
-    print("Wiper set to %d" % ds1841.wiper)
+    print(f"Wiper set to {ds1841.wiper}")
     voltage = wiper_output.read_u16()
     voltage *= 3.3
     voltage /= 65535
-    print("Wiper voltage: %.2f V" % voltage)
+    print(f"Wiper voltage {voltage::.2%}V")
     print("")
     sleep(1.0)
 
     ds1841.wiper = 63
-    print("Wiper set to %d" % ds1841.wiper)
+    print(f"Wiper set to {ds1841.wiper}")
     voltage = wiper_output.read_u16()
     voltage *= 3.3
     voltage /= 65535
-    print("Wiper voltage: %.2f V" % voltage)
+    print(f"Wiper voltage {voltage::.2%}V")
     print("")
     sleep(1.0)
```

### Comparing `micropython-ds1841-0.1.1/micropython_ds1841/ds1841.py` & `micropython-ds1841-0.1.2/micropython_ds1841/ds1841.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,30 +4,25 @@
 # SPDX-License-Identifier: MIT
 """
 `ds1841`
 ================================================================================
 
 MicroPython Driver for the DS1841 Potentiometer
 
-All code from
-
-Adapted for Micropython
-
-
 * Author(s): Bryan Siepert, Jose D. Montoya
 
 
 """
 
 from time import sleep
 from micropython import const
 from micropython_ds1841.i2c_helpers import CBits, RegisterStruct
 
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 __repo__ = "https://github.com/jposada202020/MicroPython_DS1841.git"
 
 _IVR = const(0x00)
 _CR0 = const(0x02)
 _CR1 = const(0x03)
 _LUTAR = const(0x08)
 _WR = const(0x09)
@@ -51,21 +46,21 @@
 
     Here is an example of using the :class:`DS1841` class.
     First you will need to import the libraries to use the sensor
 
     .. code-block:: python
 
         from machine import Pin, I2C
-        import ds1841
+        from micropython_ds1841 import ds1841
 
     Once this is done you can define your `machine.I2C` object and define your sensor object
 
     .. code-block:: python
 
-        i2c = I2C(sda=Pin28), scl=Pin(3))
+        i2c = I2C(1, sda=Pin(2), scl=Pin(3))
         ds1841 = ds1841.DS1841(i2c)
 
     """
 
     _lut_address = RegisterStruct(_LUTAR, ">B")
     _wiper_register = RegisterStruct(_WR, ">B")
 
@@ -124,15 +119,15 @@
         self._initial_value_register = value
         sleep(0.2)
         self._disable_save_to_eeprom = True
         self._update_mode = True
 
     @property
     def temperature(self) -> int:
-        """The current temperature in degrees celsius"""
+        """The current temperature in Celsius"""
         return self._temperature_register
 
     @property
     def voltage(self) -> float:
         """The current voltage between VCC and GND"""
         return self._voltage_register * _VCC_LSB
```

### Comparing `micropython-ds1841-0.1.1/micropython_ds1841/i2c_helpers.py` & `micropython-ds1841-0.1.2/micropython_ds1841/i2c_helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,18 +35,15 @@
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
 
@@ -65,30 +62,28 @@
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
@@ -113,15 +108,14 @@
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

### Comparing `micropython-ds1841-0.1.1/micropython_ds1841.egg-info/PKG-INFO` & `micropython-ds1841-0.1.2/micropython_ds1841.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: micropython-ds1841
-Version: 0.1.1
+Version: 0.1.2
 Summary: MicroPython Driver for the DS1841 Potentiometer
 Author-email: JDM <xxyx@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_DS1841
-Keywords: sensor,micropython,ds1841,micropython,driver,ds1841,potentiometer,analog,devices,resistance
+Keywords: sensor,micropython,ds1841,driver,ds1841,potentiometer,analog,devices,resistance
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: Implementation :: MicroPython
 Description-Content-Type: text/x-rst
```

### Comparing `micropython-ds1841-0.1.1/micropython_ds1841.egg-info/SOURCES.txt` & `micropython-ds1841-0.1.2/micropython_ds1841.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -23,9 +23,8 @@
 examples/ds1841_simpletest.py
 micropython_ds1841/__init__.py
 micropython_ds1841/ds1841.py
 micropython_ds1841/i2c_helpers.py
 micropython_ds1841.egg-info/PKG-INFO
 micropython_ds1841.egg-info/SOURCES.txt
 micropython_ds1841.egg-info/dependency_links.txt
-micropython_ds1841.egg-info/requires.txt
 micropython_ds1841.egg-info/top_level.txt
```

### Comparing `micropython-ds1841-0.1.1/pyproject.toml` & `micropython-ds1841-0.1.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -8,25 +8,24 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "micropython-ds1841"
 description = "MicroPython Driver for the DS1841 Potentiometer"
-version = "0.1.1"
+version = "0.1.2"
 readme = "README.rst"
 authors = [
     {name = "JDM", email = "xxyx@mailmeto.mozmail.com"}
 ]
 urls = {Homepage = "https://github.com/jposada202020/MicroPython_DS1841"}
 keywords = [
     "sensor",
     "micropython",
     "ds1841",
-    "micropython",
     "driver",
     "ds1841",
     "potentiometer",
     "analog",
     "devices",
     "resistance",
 ]
@@ -38,11 +37,11 @@
     "Topic :: System :: Hardware",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: Implementation :: MicroPython",
 ]
 dynamic = ["dependencies", "optional-dependencies"]
 
 [tool.setuptools]
-py-modules = ["ds1841"]
+packages = ["micropython_ds1841"]
 
 [tool.setuptools.dynamic]
 dependencies = {file = ["requirements.txt"]}
```

