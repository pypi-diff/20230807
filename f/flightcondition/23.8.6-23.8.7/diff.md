# Comparing `tmp/flightcondition-23.8.6.tar.gz` & `tmp/flightcondition-23.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flightcondition-23.8.6.tar", last modified: Sat Aug  5 02:54:20 2023, max compression
+gzip compressed data, was "flightcondition-23.8.7.tar", last modified: Mon Aug  7 01:48:58 2023, max compression
```

## Comparing `flightcondition-23.8.6.tar` & `flightcondition-23.8.7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0 mcjones   (1000) mcjones   (1000)        0 2023-08-05 02:54:20.851021 flightcondition-23.8.6/
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     1073 2022-03-31 22:06:28.000000 flightcondition-23.8.6/LICENSE
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)    13973 2023-08-05 02:54:20.853023 flightcondition-23.8.6/PKG-INFO
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)    13044 2023-08-05 01:00:28.000000 flightcondition-23.8.6/README.md
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     1677 2023-08-05 02:54:20.867025 flightcondition-23.8.6/setup.cfg
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)      132 2022-07-21 02:57:11.000000 flightcondition-23.8.6/setup.py
-drwxrwxrwx   0 mcjones   (1000) mcjones   (1000)        0 2023-08-05 02:54:19.587271 flightcondition-23.8.6/src/
-drwxrwxrwx   0 mcjones   (1000) mcjones   (1000)        0 2023-08-05 02:54:20.339289 flightcondition-23.8.6/src/flightcondition/
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)      587 2022-08-17 22:55:21.000000 flightcondition-23.8.6/src/flightcondition/__init__.py
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     7086 2023-08-05 01:40:36.000000 flightcondition-23.8.6/src/flightcondition/__main__.py
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)    24495 2023-08-05 02:53:31.000000 flightcondition-23.8.6/src/flightcondition/atmosphere.py
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     8554 2022-08-21 19:03:21.000000 flightcondition-23.8.6/src/flightcondition/boundarylayer.py
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     8185 2023-08-05 00:49:22.000000 flightcondition-23.8.6/src/flightcondition/common.py
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     3529 2022-08-16 02:55:24.000000 flightcondition-23.8.6/src/flightcondition/constants.py
-drwxrwxrwx   0 mcjones   (1000) mcjones   (1000)        0 2023-08-05 02:54:20.790318 flightcondition-23.8.6/src/flightcondition/data/
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     4453 2023-01-20 22:21:17.000000 flightcondition-23.8.6/src/flightcondition/data/constants_en.txt
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)    30564 2023-01-20 22:21:17.000000 flightcondition-23.8.6/src/flightcondition/data/fc_units_en.txt
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)    51115 2023-08-05 00:40:30.000000 flightcondition-23.8.6/src/flightcondition/flightcondition.py
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)    11868 2023-01-24 00:34:12.000000 flightcondition-23.8.6/src/flightcondition/isentropicflow.py
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     4127 2022-08-16 02:54:54.000000 flightcondition-23.8.6/src/flightcondition/nondimensional.py
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     2662 2022-08-16 02:54:58.000000 flightcondition-23.8.6/src/flightcondition/normalshock.py
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     6157 2023-08-05 02:53:31.000000 flightcondition-23.8.6/src/flightcondition/units.py
-drwxrwxrwx   0 mcjones   (1000) mcjones   (1000)        0 2023-08-05 02:54:20.664956 flightcondition-23.8.6/src/flightcondition.egg-info/
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)    13973 2023-08-05 02:54:19.000000 flightcondition-23.8.6/src/flightcondition.egg-info/PKG-INFO
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)      794 2023-08-05 02:54:19.000000 flightcondition-23.8.6/src/flightcondition.egg-info/SOURCES.txt
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)        1 2023-08-05 02:54:19.000000 flightcondition-23.8.6/src/flightcondition.egg-info/dependency_links.txt
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)       67 2023-08-05 02:54:19.000000 flightcondition-23.8.6/src/flightcondition.egg-info/entry_points.txt
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)       26 2023-08-05 02:54:19.000000 flightcondition-23.8.6/src/flightcondition.egg-info/requires.txt
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)       16 2023-08-05 02:54:19.000000 flightcondition-23.8.6/src/flightcondition.egg-info/top_level.txt
--rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)        1 2022-04-24 20:23:49.000000 flightcondition-23.8.6/src/flightcondition.egg-info/zip-safe
+drwxrwxrwx   0 mcjones   (1000) mcjones   (1000)        0 2023-08-07 01:48:58.464860 flightcondition-23.8.7/
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     1073 2022-03-31 22:06:28.000000 flightcondition-23.8.7/LICENSE
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)    13973 2023-08-07 01:48:58.467391 flightcondition-23.8.7/PKG-INFO
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)    13044 2023-08-05 01:00:28.000000 flightcondition-23.8.7/README.md
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     1677 2023-08-07 01:48:58.478078 flightcondition-23.8.7/setup.cfg
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)      132 2022-07-21 02:57:11.000000 flightcondition-23.8.7/setup.py
+drwxrwxrwx   0 mcjones   (1000) mcjones   (1000)        0 2023-08-07 01:48:57.128612 flightcondition-23.8.7/src/
+drwxrwxrwx   0 mcjones   (1000) mcjones   (1000)        0 2023-08-07 01:48:57.907547 flightcondition-23.8.7/src/flightcondition/
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)      587 2022-08-17 22:55:21.000000 flightcondition-23.8.7/src/flightcondition/__init__.py
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     7086 2023-08-05 01:40:36.000000 flightcondition-23.8.7/src/flightcondition/__main__.py
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)    24534 2023-08-07 01:45:30.000000 flightcondition-23.8.7/src/flightcondition/atmosphere.py
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     8554 2022-08-21 19:03:21.000000 flightcondition-23.8.7/src/flightcondition/boundarylayer.py
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     8190 2023-08-07 01:41:17.000000 flightcondition-23.8.7/src/flightcondition/common.py
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     3529 2022-08-16 02:55:24.000000 flightcondition-23.8.7/src/flightcondition/constants.py
+drwxrwxrwx   0 mcjones   (1000) mcjones   (1000)        0 2023-08-07 01:48:58.403319 flightcondition-23.8.7/src/flightcondition/data/
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     4453 2023-01-20 22:21:17.000000 flightcondition-23.8.7/src/flightcondition/data/constants_en.txt
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)    30564 2023-01-20 22:21:17.000000 flightcondition-23.8.7/src/flightcondition/data/fc_units_en.txt
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)    51255 2023-08-07 01:43:38.000000 flightcondition-23.8.7/src/flightcondition/flightcondition.py
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)    11868 2023-01-24 00:34:12.000000 flightcondition-23.8.7/src/flightcondition/isentropicflow.py
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     4128 2023-08-07 01:34:03.000000 flightcondition-23.8.7/src/flightcondition/nondimensional.py
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     2662 2022-08-16 02:54:58.000000 flightcondition-23.8.7/src/flightcondition/normalshock.py
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)     6157 2023-08-05 02:53:31.000000 flightcondition-23.8.7/src/flightcondition/units.py
+drwxrwxrwx   0 mcjones   (1000) mcjones   (1000)        0 2023-08-07 01:48:58.272071 flightcondition-23.8.7/src/flightcondition.egg-info/
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)    13973 2023-08-07 01:48:56.000000 flightcondition-23.8.7/src/flightcondition.egg-info/PKG-INFO
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)      794 2023-08-07 01:48:56.000000 flightcondition-23.8.7/src/flightcondition.egg-info/SOURCES.txt
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)        1 2023-08-07 01:48:56.000000 flightcondition-23.8.7/src/flightcondition.egg-info/dependency_links.txt
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)       67 2023-08-07 01:48:56.000000 flightcondition-23.8.7/src/flightcondition.egg-info/entry_points.txt
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)       26 2023-08-07 01:48:56.000000 flightcondition-23.8.7/src/flightcondition.egg-info/requires.txt
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)       16 2023-08-07 01:48:56.000000 flightcondition-23.8.7/src/flightcondition.egg-info/top_level.txt
+-rwxrwxrwx   0 mcjones   (1000) mcjones   (1000)        1 2022-04-24 20:23:49.000000 flightcondition-23.8.7/src/flightcondition.egg-info/zip-safe
```

### Comparing `flightcondition-23.8.6/LICENSE` & `flightcondition-23.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `flightcondition-23.8.6/PKG-INFO` & `flightcondition-23.8.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flightcondition
-Version: 23.8.6
+Version: 23.8.7
 Summary: Compute airspeed (true/calibrated/equivalent/Mach), atmospheric data, and other flight condition quantities, with easy unit conversion.
 Home-page: https://github.com/MattCJones/flightcondition
 Author: Matthew C. Jones
 Author-email: matt.c.jones.aoe@gmail.com
 License: MIT License
 Keywords: utility,aerospace,engineering,design
 Platform: UNKNOWN
```

### Comparing `flightcondition-23.8.6/README.md` & `flightcondition-23.8.7/README.md`

 * *Files identical despite different names*

### Comparing `flightcondition-23.8.6/setup.cfg` & `flightcondition-23.8.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 	License :: OSI Approved :: MIT License
 	Natural Language :: English
 	Operating System :: OS Independent
 	Topic :: Scientific/Engineering
 	Topic :: Utilities
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
-version = 23.08.06
+version = 23.08.07
 
 [options]
 packages = find:
 package_dir = 
 	= src
 zip_safe = True
 python_requires = >=3.8
```

### Comparing `flightcondition-23.8.6/src/flightcondition/__init__.py` & `flightcondition-23.8.7/src/flightcondition/__init__.py`

 * *Files identical despite different names*

### Comparing `flightcondition-23.8.6/src/flightcondition/__main__.py` & `flightcondition-23.8.7/src/flightcondition/__main__.py`

 * *Files identical despite different names*

### Comparing `flightcondition-23.8.6/src/flightcondition/atmosphere.py` & `flightcondition-23.8.7/src/flightcondition/atmosphere.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     check_length_dimensioned, check_US_length_units,\
     check_pressure_dimensioned, check_temperature_dimensioned
 
 
 class Layer(DimensionalData):
     """Class to compute and store layer data. """
 
-    names = {
+    names_dict = {
         'name': 'layer_name',
         'H_base': 'base_geopotential_height',
         'T_base': 'base_geopotential_temperature',
         'T_grad': 'temperature_gradient',
         'p_base': 'base_static_pressure',
     }
 
@@ -58,15 +58,15 @@
             self._H_base[idx] = Atmo.H_base[jdx]
             self._T_base[idx] = Atmo.T_base[jdx]
             self._T_grad[idx] = Atmo.T_grad[jdx]
             self._p_base[idx] = Atmo.p_base[jdx]
 
         # Initialize access by full quantity name through .byname.<name>
         self.byname = AliasAttributes(
-            varsobj_arr=[self, ], names_dict_arr=[__class__.names, ])
+            varsobj_arr=[self, ], names_dict_arr=[__class__.names_dict, ])
 
     @staticmethod
     def _layer_idx(H):
         """Find index for layer data.
 
         Args:
             H_arr (length): Geopotential altitude
@@ -115,17 +115,17 @@
             H_base_units   = 'km'
             T_base_units   = 'degK'
             T_grad_units   = 'degK/km'
             p_base_units   = 'Pa'
 
         # Insert longer variable name into output
         if max_sym_chars is None:
-            max_sym_chars = max([len(v) for v in self.names.keys()])
+            max_sym_chars = max([len(v) for v in self.names_dict.keys()])
         if max_name_chars is None:
-            max_name_chars = max([len(v) for v in self.names.values()])
+            max_name_chars = max([len(v) for v in self.names_dict.values()])
 
         H_base_str = self._vartostr(var=self.H_base, var_str='H_base',
                                     to_units=H_base_units,
                                     max_sym_chars=max_sym_chars,
                                     max_name_chars=max_name_chars,
                                     fmt_val="10.5g", pretty_print=pretty_print)
         T_base_str = self._vartostr(var=self.T_base, var_str='T_base',
@@ -219,15 +219,15 @@
 
         # Compute additional properties such as mean free path
         # Explore the class data structure for all options
         print( f"\nThe mean free path = {atm.MFP:.3g}")
         # >>> The mean free path = [7.25e-08 4.04e-05 0.00564] yd
     """
 
-    names = {
+    names_dict = {
         'h': 'geometric_altitude',
         'H': 'geopotential_altitude',
         'p': 'pressure',
         'T': 'temperature',
         'rho': 'density',
         'a': 'sound_speed',
         'mu': 'dynamic_viscosity',
@@ -293,15 +293,15 @@
             if check_US_length_units(h):
                 self.units = 'US'
             else:
                 self.units = 'SI'
 
         # Initialize access by full quantity name through .byname.<name>
         self.byname = AliasAttributes(
-            varsobj_arr=[self, ], names_dict_arr=[__class__.names, ])
+            varsobj_arr=[self, ], names_dict_arr=[__class__.names_dict, ])
 
     def tostring(self, full_output=None, units=None, max_sym_chars=None,
                  max_name_chars=None, pretty_print=True):
         """String representation of data structure.
 
         Args:
             full_output (bool): Set to True for full output
@@ -339,17 +339,17 @@
             nu_units  = 'm^2/s'
             k_units   = 'W/m/K'
             g_units   = 'm/s^2'
             MFP_units = 'm'
 
         # Insert longer variable name into output
         if max_sym_chars is None:
-            max_sym_chars = max([len(v) for v in self.names.keys()])
+            max_sym_chars = max([len(v) for v in self.names_dict.keys()])
         if max_name_chars is None:
-            max_name_chars = max([len(v) for v in self.names.values()])
+            max_name_chars = max([len(v) for v in self.names_dict.values()])
 
         h_str = self._vartostr(var=self.h, var_str='h', to_units=h_units,
                                max_sym_chars=max_sym_chars,
                                max_name_chars=max_name_chars,
                                fmt_val="10.5g", pretty_print=pretty_print)
         H_str = self._vartostr(var=self.H, var_str='H', to_units=H_units,
                                max_sym_chars=max_sym_chars,
@@ -601,15 +601,14 @@
         check_dimensioned(p)
         check_pressure_dimensioned(p)
         # Check that p is same size as h
         if np.size(p) != np.size(self._h):
             raise AttributeError("Input array must be same size as altitude")
         self._p = p
 
-
     @_property_decorators
     def T(self):
         """Ambient air temperature :math:`T` """
         # Only compute T if not user set
         if self._T is not None:
             T = self._T
         else:
```

### Comparing `flightcondition-23.8.6/src/flightcondition/boundarylayer.py` & `flightcondition-23.8.7/src/flightcondition/boundarylayer.py`

 * *Files identical despite different names*

### Comparing `flightcondition-23.8.6/src/flightcondition/common.py` & `flightcondition-23.8.7/src/flightcondition/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,58 +20,58 @@
 class AliasAttributes():
     """Nested alias class to reference quantities by prescribed aliases. """
 
     def __init__(self, varsobj_arr, names_dict_arr):
         """Populate full names and link to variable
         Args:
             varsobj (list): List of objects that holds all of the variables
-            names_dict (list): List of dictionaries that maps variables to
+            names_dict_arr (list): List of dictionaries that maps variables to
                 their alias names
         """
         # Avoid infinite loop when setting properties
         super().__setattr__("varsobj_arr", varsobj_arr)
         super().__setattr__("names_dict_arr", names_dict_arr)
 
     def __dir__(self):
-        """Add tab completion for alias names. """
+        """Add tab completion for alias names_dict. """
         # Avoid infinite loop when loading varsobj and names_dict
         names_dict_arr = super().__getattribute__("names_dict_arr")
         names_arr = []
         for names_dict in names_dict_arr:
-            for varname in names_dict.values():
-                names_arr.append(varname)
+            for name in names_dict.values():
+                names_arr.append(name)
         return names_arr
 
     def __getattribute__(self, attr):
         """Get referenced quantity
 
         Args:
             attr (str): attribute name
         """
         # Avoid infinite loop when loading varsobj and names_dict
         varsobj_arr = super().__getattribute__("varsobj_arr")
         names_dict_arr = super().__getattribute__("names_dict_arr")
         for varsobj, names_dict in zip(varsobj_arr, names_dict_arr):
-            for var, varname in names_dict.items():
-                if attr == varname:
+            for var, name in names_dict.items():
+                if attr == name:
                     return getattr(varsobj, var)
 
     def __setattr__(self, attr, attrval):
         """Set referenced quantity
 
         Args:
             attr (str): attribute name
             attrval (quantity): attribute value
         """
         # Avoid infinite loop when loading varsobj and names_dict
         varsobj_arr = super().__getattribute__("varsobj_arr")
         names_dict_arr = super().__getattribute__("names_dict_arr")
         for varsobj, names_dict in zip(varsobj_arr, names_dict_arr):
-            for var, varname in names_dict.items():
-                if attr == varname:
+            for var, name in names_dict.items():
+                if attr == name:
                     return setattr(varsobj, var, attrval)
 
     def __repr__(self):
         """Output string representation of class object.
 
         Returns:
             str: Full string output
@@ -88,25 +88,25 @@
         except TypeError:
             return ""
 
 
 class DimensionalData:
     """Parent class to hold dimensional data"""
 
-    names = {}
+    names_dict = {}
 
     def __eq__(self, other):
         """Check equality.
         Returns:
             dict: Dictionary representation of object
         """
         if other.__class__ is not self.__class__:
             return NotImplemented
 
-        for var in self.names.keys():
+        for var in self.names_dict.keys():
             a = self.asdict[var]
             b = other.asdict[var]
             if not (np.shape(a) == np.shape(b)):
                 return False
             else:
                 if not ((a == b) | (np.isnan(a) & np.isnan(b))).all():
                     return False
@@ -142,34 +142,34 @@
         return self.tostring(full_output=full_output)
 
     def _asdict_template(self, names_dict=None):
         """Return class data as dictionary.
 
         Args:
             names_dict (dict): Optionally specified variable names
-                dicitonary
+                dictionary
 
         Returns:
             dict: Class data
         """
         if names_dict is None:
-            names_dict = self.names
+            names_dict = self.names_dict
         obj_dict = {}
-        for var, varname in names_dict.items():
+        for var, name in names_dict.items():
             obj_dict[var] = getattr(self, var)
         return obj_dict
 
     @property
     def asdict(self):
         """Return class data as dictionary.
 
         Returns:
             dict: Class data
         """
-        return self._asdict_template(self.names)
+        return self._asdict_template(self.names_dict)
 
     def print(self, *args, **kwargs):
         """Print tostring() function to stdout. """
         print(self.tostring(*args, **kwargs))
 
     def tostring(self, full_output=True):
         """Override this function to output string representation of class
@@ -197,15 +197,15 @@
             fmt_val (str): String for formatting value
             pretty_print (bool): Pretty print format
 
         Returns:
             str: formatted string
         """
         pp_ = "~P" if pretty_print else ""
-        var_name = self.names[var_str]
+        name = self.names_dict[var_str]
         if to_units is None:
             var_units_str = ""
         else:
             var.ito(to_units)
             var_units_str = f"{var.units:{pp_}}"
 
         if np.size(var) > 6:
@@ -215,15 +215,15 @@
                 mag = var.magnitude
             var_val_str = (f"[{mag[0]:{fmt_val}} {mag[1]:{fmt_val}} "
                            f"{mag[2]:{fmt_val}} ... {mag[-3]:{fmt_val}} "
                            f"{mag[-2]:{fmt_val}} {mag[-1]:{fmt_val}}] "
                            f"{var_units_str}")
         else:
             var_val_str = f"{var:{fmt_val}{pp_}}"
-        var_str = (f"{var_name:{max_name_chars}s} {var_str:{max_sym_chars}s} ="
+        var_str = (f"{name:{max_name_chars}s} {var_str:{max_sym_chars}s} ="
                    f" {var_val_str}")
         return var_str
 
     @staticmethod
     def _arg_from_alias(alias_list, kwargs_dict):
         """Determine argument from hidden alias list
```

### Comparing `flightcondition-23.8.6/src/flightcondition/constants.py` & `flightcondition-23.8.7/src/flightcondition/constants.py`

 * *Files identical despite different names*

### Comparing `flightcondition-23.8.6/src/flightcondition/data/constants_en.txt` & `flightcondition-23.8.7/src/flightcondition/data/constants_en.txt`

 * *Files identical despite different names*

### Comparing `flightcondition-23.8.6/src/flightcondition/data/fc_units_en.txt` & `flightcondition-23.8.7/src/flightcondition/data/fc_units_en.txt`

 * *Files identical despite different names*

### Comparing `flightcondition-23.8.6/src/flightcondition/flightcondition.py` & `flightcondition-23.8.7/src/flightcondition/flightcondition.py`

 * *Files 8% similar despite different names*

```diff
@@ -86,15 +86,15 @@
         # >>> [ True  True  True]
 
         # Or by their sub-categories: `byalt`, `byvel`, or `bylen`
         print(fc.byvel.TAS == fc.byvel.byname.true_airspeed)
         # >>> [ True  True  True]
     """
     # Define dictionaries mapping variables to their full names
-    _byalt_names = Atmosphere.names
+    _byalt_names = Atmosphere.names_dict
     _byvel_names = {
         'TAS': 'true_airspeed',
         'CAS': 'calibrated_airspeed',
         'EAS': 'equivalent_airspeed',
         'KTAS': 'knots_true_airspeed',
         'KCAS': 'knots_calibrated_airspeed',
         'KEAS': 'knots_equivalent_airspeed',
@@ -114,18 +114,18 @@
         'Re': 'reynolds_number',
         'h_BL_lamr': 'boundary_thickness_laminar',
         'h_BL_turb': 'boundary_thickness_turbulent',
         'Cf_lamr': 'friction_coefficient_laminar',
         'Cf_turb': 'friction_coefficient_turbulent',
         'h_yplus1': 'wall_distance_yplus1',
     }
-    names = {}
-    names.update(_byalt_names)
-    names.update(_byvel_names)
-    names.update(_bylen_names)
+    names_dict = {}
+    names_dict.update(_byalt_names)
+    names_dict.update(_byvel_names)
+    names_dict.update(_bylen_names)
 
 # =========================================================================== #
 #                       GENERAL FUNCTIONS & PROPERTIES                        #
 # =========================================================================== #
     def __init__(
         self, h=None, M=None, TAS=None, CAS=None, EAS=None, L=None, Re=None,
         units=None, full_output=None, **kwargs,
@@ -149,15 +149,15 @@
             L (length): Length scale - aliases are 'ell', 'bylen', 'length',
                 'length_scale', 'l'
             Re (dimless): Reynolds number - alternative to velocity or length
                 scale but not both - aliases are 'Re_L', 'reynolds_number'
             units (str): Set to 'US' for US units or 'SI' for SI
             full_output (bool): Set to True for full output
         """
-        # Initalize Atmosphere super class
+        # Initialize Atmosphere super class
         super().__init__(h=h, units=units, full_output=full_output, **kwargs)
         self._byalt_tostring = super().tostring
 
         # Computer sea level properties
         self._atm0 = Atmosphere(h=0*unit('kft'))
 
         # Need to cycle self.units to properly set default units
@@ -237,15 +237,15 @@
         # Check if special L_m syntactic sugar is used
         L_m_aliases = ['L_m', 'ell_m', 'm']
         if h is None:
             L_m = __class__._arg_from_alias(L_m_aliases, kwargs)
             if L_m is not None:
                 L = L_m * unit('m')
 
-        # If length scale is not input, default to unity with dimentionals unit
+        # If length scale is not input, default to unity with dimensional unit
         # based on US or SI determination
         if L is None:
             if Re is None:
                 L_unit = unit('ft') if self.units == 'US' else unit('m')
                 self.L = 1.0 * L_unit
             else:
                 Re *= dimless
@@ -311,43 +311,43 @@
 
         # Set variable aliases by altitude properties to .byalt.<var>
         byalt_vars = {key: key for key in self._byalt_names.keys()}
         self.byalt = AliasAttributes(
             varsobj_arr=[self, self, self, self, self, self, ],
             names_dict_arr=[
                 byalt_vars,
-                {"_byalt_names": "names"},
+                {"_byalt_names": "names_dict"},
                 {"_byalt_tostring": "tostring"},
                 {"full_output": "full_output"},
                 {"_byalt_byname": "byname"},
                 {"_byalt_asdict": "asdict"},
             ]
         )
 
         # Set variable aliases by velocity properties to .byvel.<var>
         byvel_vars = {key: key for key in self._byvel_names.keys()}
         self.byvel = AliasAttributes(
             varsobj_arr=[self, self, self, self, self, self, ],
             names_dict_arr=[
                 byvel_vars,
-                {"_byvel_names": "names"},
+                {"_byvel_names": "names_dict"},
                 {"_byvel_tostring": "tostring"},
                 {"full_output": "full_output"},
                 {"_byvel_byname": "byname"},
                 {"_byvel_asdict": "asdict"},
             ]
         )
 
         # Set variable aliases by length properties to .bylen.<var>
         bylen_vars = {key: key for key in self._bylen_names.keys()}
         self.bylen = AliasAttributes(
             varsobj_arr=[self, self, self, self, self, self, self, ],
             names_dict_arr=[
                 bylen_vars,
-                {"_bylen_names": "names"},
+                {"_bylen_names": "names_dict"},
                 {"_bylen_tostring": "tostring"},
                 {"full_output": "full_output"},
                 {"_bylen_byname": "byname"},
                 {"_bylen_asdict": "asdict"},
                 {"wall_distance_from_yplus": "wall_distance_from_yplus"},
             ]
         )
@@ -618,16 +618,16 @@
         super(FlightCondition, self.__class__).h.fset(self, h)
 
         # Set airspeed and length array sizes if they are singular and altitude
         # is non-singular
         if hasattr(self, '_M'):
             if __class__._check_compatible_array_size(
                     arr1=h, arr2=self._M,
-                    arr_name1=self.names['h'],
-                    arr_name2=self.names['M'],
+                    arr_name1=self.names_dict['h'],
+                    arr_name2=self.names_dict['M'],
                     raise_warning=True):
                 if self._holdconst_vel_var == 'M':
                     self.M = __class__._reshape_arr1_like_arr2(self._M, h)
                 elif self._holdconst_vel_var == 'TAS':
                     self.TAS = __class__._reshape_arr1_like_arr2(self._TAS, h)
                 elif self._holdconst_vel_var == 'CAS':
                     self.CAS = __class__._reshape_arr1_like_arr2(self._CAS, h)
@@ -635,16 +635,16 @@
                     self.EAS = __class__._reshape_arr1_like_arr2(self._EAS, h)
                 else:  # default to holding EAS constant
                     self.EAS = __class__._reshape_arr1_like_arr2(self._EAS, h)
 
         if hasattr(self, '_L'):
             if __class__._check_compatible_array_size(
                     arr1=h, arr2=self._L,
-                    arr_name1=self.names['h'],
-                    arr_name2=self.names['L'],
+                    arr_name1=self.names_dict['h'],
+                    arr_name2=self.names_dict['L'],
                     raise_warning=True):
                 self._L = __class__._reshape_arr1_like_arr2(self._L, h)
 
 # =========================================================================== #
 #                       VELOCITY FUNCTIONS & PROPERTIES                       #
 # =========================================================================== #
     def _process_input_velocity(self, vel_arr, vel_name="Velocity"):
@@ -656,21 +656,21 @@
 
         Returns:
             bool: True if compatible else False
         """
         if hasattr(self, '_h'):
             if __class__._check_compatible_array_size(
                     arr1=vel_arr, arr2=self._h,
-                    arr_name1=vel_name, arr_name2=self.names["h"],
+                    arr_name1=vel_name, arr_name2=self.names_dict["h"],
                     raise_warning=True, raise_error=True):
                 self._h = __class__._reshape_arr1_like_arr2(self._h, vel_arr)
         if hasattr(self, '_L'):
             if __class__._check_compatible_array_size(
                     arr1=vel_arr, arr2=self._L,
-                    arr_name1=vel_name, arr_name2=self.names["L"],
+                    arr_name1=vel_name, arr_name2=self.names_dict["L"],
                     raise_warning=True):
                 self._L = __class__._reshape_arr1_like_arr2(self._L, vel_arr)
 
     def _byvel_tostring(self, full_output=None, units=None, max_sym_chars=None,
                         max_name_chars=None, pretty_print=True):
         """String representation of data structure.
 
@@ -716,17 +716,17 @@
             T0_units    = 'degK'
             Tr_lamr_units = 'degK'
             Tr_turb_units = 'degK'
             Re_by_L_units = '1/mm'
 
         # Insert longer variable name into output
         if max_sym_chars is None:
-            max_sym_chars = max([len(v) for v in self.names.keys()])
+            max_sym_chars = max([len(v) for v in self.names_dict.keys()])
         if max_name_chars is None:
-            max_name_chars = max([len(v) for v in self.names.values()])
+            max_name_chars = max([len(v) for v in self.names_dict.values()])
 
         M_str = self._vartostr(
             var=self.M, var_str='M', to_units='',
             max_sym_chars=max_sym_chars, max_name_chars=max_name_chars,
             fmt_val="10.5g", pretty_print=pretty_print) + "\n"
         TAS_str = self._vartostr(
             var=self.TAS, var_str='TAS', to_units=TAS_units,
@@ -1000,15 +1000,15 @@
         return self._M
 
     @M.setter
     def M(self, M):
         """Mach number :math:`M` """
         M *= dimless  # add dimless for raw float input
         self._M = __class__._preprocess_arr(M, input_alt=self.h)
-        self._process_input_velocity(self._M, vel_name=self.names['M'])
+        self._process_input_velocity(self._M, vel_name=self.names_dict['M'])
 
         self._TAS = self._TAS_from_M(self.M)
         self._EAS = self._EAS_from_TAS(self.TAS, self.M)
         self._q_c = self._q_c_from_M(self.M)
         self._CAS = self._CAS_from_q_c(self.q_c)
 
         # Out of all velocity quantities, hold this one constant over altitude
@@ -1020,15 +1020,15 @@
         return self._TAS
 
     @TAS.setter
     def TAS(self, TAS):
         """Set true airspeed. """
         self._TAS = __class__._preprocess_arr(TAS, input_alt=self.h)
         self._process_input_velocity(
-            self._TAS, vel_name=self.names['TAS'])
+            self._TAS, vel_name=self.names_dict['TAS'])
 
         self._M = self._M_from_TAS(TAS)
         self._EAS = self._EAS_from_TAS(self.TAS, self.M)
         self._q_c = self._q_c_from_M(self.M)
         self._CAS = self._CAS_from_q_c(self.q_c)
 
         # Out of all velocity quantities, hold this one constant over altitude
@@ -1040,15 +1040,15 @@
         return self._CAS
 
     @CAS.setter
     def CAS(self, CAS):
         """Calibrated airspeed. """
         self._CAS = __class__._preprocess_arr(CAS, input_alt=self.h)
         self._process_input_velocity(
-            self._CAS, vel_name=self.names['CAS'])
+            self._CAS, vel_name=self.names_dict['CAS'])
 
         self._q_c = self._q_c_from_CAS(self.CAS)
         self._M = self._M_from_q_c(self.q_c)
         self._TAS = self._TAS_from_M(self.M)
         self._EAS = self._EAS_from_TAS(self.TAS, self.M)
 
         # Out of all velocity quantities, hold this one constant over altitude
@@ -1060,15 +1060,15 @@
         return self._EAS
 
     @EAS.setter
     def EAS(self, EAS):
         """Set equivalent airspeed. """
         self._EAS = __class__._preprocess_arr(EAS, input_alt=self.h)
         self._process_input_velocity(
-            self._EAS, vel_name=self.names['EAS'])
+            self._EAS, vel_name=self.names_dict['EAS'])
 
         self._M = self._M_from_EAS(self.EAS)
         self._TAS = self._TAS_from_M(self.M)
         self._q_c = self._q_c_from_M(self.M)
         self._CAS = self._CAS_from_q_c(self.q_c)
 
         # Out of all velocity quantities, hold this one constant over altitude
@@ -1203,17 +1203,17 @@
             h_BL_units = 'in'
         else:  # default to SI units
             L_units = 'm'
             h_BL_units = 'mm'
 
         # Insert longer variable name into output
         if max_sym_chars is None:
-            max_sym_chars = max([len(v) for v in self.names.keys()])
+            max_sym_chars = max([len(v) for v in self.names_dict.keys()])
         if max_name_chars is None:
-            max_name_chars = max([len(v) for v in self.names.values()])
+            max_name_chars = max([len(v) for v in self.names_dict.values()])
 
         L_str = self._vartostr(
             var=self.L, var_str='L', to_units=L_units,
             max_sym_chars=max_sym_chars, max_name_chars=max_name_chars,
             fmt_val="10.5g", pretty_print=pretty_print)
         Re_str = self._vartostr(
             var=self.Re, var_str='Re', to_units='',
@@ -1296,24 +1296,24 @@
         self._L = L
 
         # Set altitude and airspeed array sizes if they are singular and length
         # is non-singular
         if hasattr(self, '_h'):
             if __class__._check_compatible_array_size(
                     arr1=self._h, arr2=L,
-                    arr_name1=self.names['h'],
-                    arr_name2=self.names['L'],
+                    arr_name1=self.names_dict['h'],
+                    arr_name2=self.names_dict['L'],
                     raise_warning=True):
                 pass
                 # self._h = __class__._reshape_arr1_like_arr2(self._h, L)
         if hasattr(self, '_M'):
             if __class__._check_compatible_array_size(
                     arr1=self.M, arr2=L,
-                    arr_name1=self.names['M'],
-                    arr_name2=self.names['L'],
+                    arr_name1=self.names_dict['M'],
+                    arr_name2=self.names_dict['L'],
                     raise_warning=True):
                 pass
                 # self.M = __class__._reshape_arr1_like_arr2(self._M, L)
 
     @_property_decorators
     def Re(self):
         """Get Reynolds number :math:`Re`"""
@@ -1325,16 +1325,16 @@
     def Re(self, Re):
         """Set Reynolds number :math:`Re`
         Set the true airspeed based on Reynolds number and length scale. """
         Re *= dimless  # add dimless for raw float input
         Re = self._preprocess_arr(
             Re, input_alt=self.h, input_vel=self.M)
         __class__._check_compatible_array_size(
-            arr1=self.M, arr2=Re, arr_name1=self.names['M'],
-            arr_name2=self.names['L'], raise_warning=True,
+            arr1=self.M, arr2=Re, arr_name1=self.names_dict['M'],
+            arr_name2=self.names_dict['L'], raise_warning=True,
             raise_error=True)
         self.TAS = NonDimensional.reynolds_number_velocity(
             Re_L=Re, L=self.L, nu=self.nu)
 
     @_property_decorators
     def h_BL_lamr(self):
         """Get laminar Boundary Layer Thickness :math:`\\h_BL_{lamr}` """
```

### Comparing `flightcondition-23.8.6/src/flightcondition/isentropicflow.py` & `flightcondition-23.8.7/src/flightcondition/isentropicflow.py`

 * *Files identical despite different names*

### Comparing `flightcondition-23.8.6/src/flightcondition/nondimensional.py` & `flightcondition-23.8.7/src/flightcondition/nondimensional.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
             speed: Velocity
         """
         U = M*a if M is not None else None
         return U
 
     @staticmethod
     def reynolds_number(U, L, nu):
-        """Compute Reynolds number :math:`Re`, the ratio of inertial to viscou
+        """Compute Reynolds number :math:`Re`, the ratio of inertial to viscous
         forces.
 
         Args:
             U (speed): Velocity
             L (length): Length scale
             nu (length^2/time): Kinematic viscosity
```

### Comparing `flightcondition-23.8.6/src/flightcondition/normalshock.py` & `flightcondition-23.8.7/src/flightcondition/normalshock.py`

 * *Files identical despite different names*

### Comparing `flightcondition-23.8.6/src/flightcondition/units.py` & `flightcondition-23.8.7/src/flightcondition/units.py`

 * *Files identical despite different names*

### Comparing `flightcondition-23.8.6/src/flightcondition.egg-info/PKG-INFO` & `flightcondition-23.8.7/src/flightcondition.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flightcondition
-Version: 23.8.6
+Version: 23.8.7
 Summary: Compute airspeed (true/calibrated/equivalent/Mach), atmospheric data, and other flight condition quantities, with easy unit conversion.
 Home-page: https://github.com/MattCJones/flightcondition
 Author: Matthew C. Jones
 Author-email: matt.c.jones.aoe@gmail.com
 License: MIT License
 Keywords: utility,aerospace,engineering,design
 Platform: UNKNOWN
```

### Comparing `flightcondition-23.8.6/src/flightcondition.egg-info/SOURCES.txt` & `flightcondition-23.8.7/src/flightcondition.egg-info/SOURCES.txt`

 * *Files identical despite different names*

