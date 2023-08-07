# Comparing `tmp/tiledb-cf-0.6.2.tar.gz` & `tmp/tiledb-cf-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiledb-cf-0.6.2.tar", last modified: Thu Feb  3 17:00:50 2022, max compression
+gzip compressed data, was "tiledb-cf-0.7.0.tar", last modified: Mon Aug  7 16:03:24 2023, max compression
```

## Comparing `tiledb-cf-0.6.2.tar` & `tiledb-cf-0.7.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 17:00:50.894539 tiledb-cf-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-02-03 17:00:44.000000 tiledb-cf-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3802 2022-02-03 17:00:50.894539 tiledb-cf-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2637 2022-02-03 17:00:44.000000 tiledb-cf-0.6.2/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      511 2022-02-03 17:00:44.000000 tiledb-cf-0.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1709 2022-02-03 17:00:50.894539 tiledb-cf-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-03 17:00:44.000000 tiledb-cf-0.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 17:00:50.890539 tiledb-cf-0.6.2/tiledb/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 17:00:50.890539 tiledb-cf-0.6.2/tiledb/cf/
--rw-r--r--   0 runner    (1001) docker     (121)      835 2022-02-03 17:00:44.000000 tiledb-cf-0.6.2/tiledb/cf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-02-03 17:00:44.000000 tiledb-cf-0.6.2/tiledb/cf/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2427 2022-02-03 17:00:44.000000 tiledb-cf-0.6.2/tiledb/cf/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)    29790 2022-02-03 17:00:44.000000 tiledb-cf-0.6.2/tiledb/cf/core.py
--rw-r--r--   0 runner    (1001) docker     (121)    45890 2022-02-03 17:00:44.000000 tiledb-cf-0.6.2/tiledb/cf/creator.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 17:00:50.890539 tiledb-cf-0.6.2/tiledb/cf/netcdf_engine/
--rw-r--r--   0 runner    (1001) docker     (121)      720 2022-02-03 17:00:44.000000 tiledb-cf-0.6.2/tiledb/cf/netcdf_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13482 2022-02-03 17:00:44.000000 tiledb-cf-0.6.2/tiledb/cf/netcdf_engine/_array_converters.py
--rw-r--r--   0 runner    (1001) docker     (121)     6602 2022-02-03 17:00:44.000000 tiledb-cf-0.6.2/tiledb/cf/netcdf_engine/_attr_converters.py
--rw-r--r--   0 runner    (1001) docker     (121)    19006 2022-02-03 17:00:44.000000 tiledb-cf-0.6.2/tiledb/cf/netcdf_engine/_dim_converters.py
--rw-r--r--   0 runner    (1001) docker     (121)     6754 2022-02-03 17:00:44.000000 tiledb-cf-0.6.2/tiledb/cf/netcdf_engine/_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     5633 2022-02-03 17:00:44.000000 tiledb-cf-0.6.2/tiledb/cf/netcdf_engine/api.py
--rw-r--r--   0 runner    (1001) docker     (121)    47281 2022-02-03 17:00:44.000000 tiledb-cf-0.6.2/tiledb/cf/netcdf_engine/converter.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 17:00:50.890539 tiledb-cf-0.6.2/tiledb/cf/xarray_engine/
--rw-r--r--   0 runner    (1001) docker     (121)      154 2022-02-03 17:00:44.000000 tiledb-cf-0.6.2/tiledb/cf/xarray_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    19645 2022-02-03 17:00:44.000000 tiledb-cf-0.6.2/tiledb/cf/xarray_engine/backend_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 17:00:50.894539 tiledb-cf-0.6.2/tiledb_cf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3802 2022-02-03 17:00:50.000000 tiledb-cf-0.6.2/tiledb_cf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      731 2022-02-03 17:00:50.000000 tiledb-cf-0.6.2/tiledb_cf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-03 17:00:50.000000 tiledb-cf-0.6.2/tiledb_cf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      136 2022-02-03 17:00:50.000000 tiledb-cf-0.6.2/tiledb_cf.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-03 17:00:50.000000 tiledb-cf-0.6.2/tiledb_cf.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      209 2022-02-03 17:00:50.000000 tiledb-cf-0.6.2/tiledb_cf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-02-03 17:00:50.000000 tiledb-cf-0.6.2/tiledb_cf.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:03:24.947866 tiledb-cf-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-07 16:03:21.000000 tiledb-cf-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-08-07 16:03:24.947866 tiledb-cf-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-08-07 16:03:21.000000 tiledb-cf-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-08-07 16:03:21.000000 tiledb-cf-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-08-07 16:03:24.947866 tiledb-cf-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 16:03:21.000000 tiledb-cf-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:03:24.943866 tiledb-cf-0.7.0/tiledb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:03:24.947866 tiledb-cf-0.7.0/tiledb/cf/
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-08-07 16:03:21.000000 tiledb-cf-0.7.0/tiledb/cf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-07 16:03:21.000000 tiledb-cf-0.7.0/tiledb/cf/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-08-07 16:03:21.000000 tiledb-cf-0.7.0/tiledb/cf/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29732 2023-08-07 16:03:21.000000 tiledb-cf-0.7.0/tiledb/cf/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44898 2023-08-07 16:03:21.000000 tiledb-cf-0.7.0/tiledb/cf/creator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:03:24.947866 tiledb-cf-0.7.0/tiledb/cf/netcdf_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-08-07 16:03:21.000000 tiledb-cf-0.7.0/tiledb/cf/netcdf_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13365 2023-08-07 16:03:21.000000 tiledb-cf-0.7.0/tiledb/cf/netcdf_engine/_array_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-08-07 16:03:21.000000 tiledb-cf-0.7.0/tiledb/cf/netcdf_engine/_attr_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19006 2023-08-07 16:03:21.000000 tiledb-cf-0.7.0/tiledb/cf/netcdf_engine/_dim_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7205 2023-08-07 16:03:21.000000 tiledb-cf-0.7.0/tiledb/cf/netcdf_engine/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5474 2023-08-07 16:03:21.000000 tiledb-cf-0.7.0/tiledb/cf/netcdf_engine/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46328 2023-08-07 16:03:21.000000 tiledb-cf-0.7.0/tiledb/cf/netcdf_engine/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:03:24.947866 tiledb-cf-0.7.0/tiledb/cf/xarray_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-08-07 16:03:21.000000 tiledb-cf-0.7.0/tiledb/cf/xarray_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19645 2023-08-07 16:03:21.000000 tiledb-cf-0.7.0/tiledb/cf/xarray_engine/backend_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:03:24.947866 tiledb-cf-0.7.0/tiledb_cf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-08-07 16:03:24.000000 tiledb-cf-0.7.0/tiledb_cf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-08-07 16:03:24.000000 tiledb-cf-0.7.0/tiledb_cf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 16:03:24.000000 tiledb-cf-0.7.0/tiledb_cf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-08-07 16:03:24.000000 tiledb-cf-0.7.0/tiledb_cf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 16:03:24.000000 tiledb-cf-0.7.0/tiledb_cf.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-08-07 16:03:24.000000 tiledb-cf-0.7.0/tiledb_cf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-07 16:03:24.000000 tiledb-cf-0.7.0/tiledb_cf.egg-info/top_level.txt
```

### Comparing `tiledb-cf-0.6.2/LICENSE` & `tiledb-cf-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tiledb-cf-0.6.2/PKG-INFO` & `tiledb-cf-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: tiledb-cf
-Version: 0.6.2
+Version: 0.7.0
 Summary: TileDB Python library for supporting Climate and Forecast datasets.
 Home-page: https://github.com/TileDB-Inc/TileDB-CF-Py
 Author: TileDB, Inc.
 Author-email: help@tiledb.io
 License: MIT
 Project-URL: Documentation, https://docs.tiledb.com
 Keywords: tiledb,climate,forecast,netcdf
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -100,9 +99,7 @@
 
   --help                          Show this message and exit.
 ```
 
 ## Development
 
 For information on contributing to this project see the [CONTRIBUTING](CONTRIBUTING.md) document.
-
-
```

#### html2text {}

```diff
@@ -1,38 +1,38 @@
-Metadata-Version: 2.1 Name: tiledb-cf Version: 0.6.2 Summary: TileDB Python
+Metadata-Version: 2.1 Name: tiledb-cf Version: 0.7.0 Summary: TileDB Python
 library for supporting Climate and Forecast datasets. Home-page: https://
 github.com/TileDB-Inc/TileDB-CF-Py Author: TileDB, Inc. Author-email:
 help@tiledb.io License: MIT Project-URL: Documentation, https://docs.tiledb.com
-Keywords: tiledb,climate,forecast,netcdf Platform: UNKNOWN Classifier:
-Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Information Technology Classifier: Intended
-Audience :: Science/Research Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent Classifier: Programming Language
-:: Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: Implementation ::
-PyPy Classifier: Topic :: Software Development Requires-Python: >=3.7
-Description-Content-Type: text/markdown Provides-Extra: docs Provides-Extra:
-netCDF4 Provides-Extra: xarray Provides-Extra: parallel Provides-Extra:
-examples License-File: LICENSE [TileDB_logo] # TileDB-CF-Py The TileDB-CF-Py
-library is a Python library for supporting the NetCDF data model in the [TileDB
-storage engine](https://github.com/TileDB-Inc/TileDB). TileDB-CF-Py provides
-readers and writers for viewing and manipulating TileDB arrays and groups using
-TileDB CF Dataspaces - a special TileDB group that follows the requirements in
-[tiledb-cf-spec.md](tiledb-cf-spec.md). ## TileDB Quick Links * [Homepage]
-(https://tiledb.com) * [Documentation](https://docs.tiledb.com/main/) * [Forum]
-(https://forum.tiledb.io/) * [Organization](https://github.com/TileDB-Inc/) ##
-Getting Started ### Quick Installation This project is available from [PyPI]
-(https://pypi.org/project/tiledb/) and may be installed with ``pip``: ```bash
-pip install tiledb-cf ``` ### Documentation #### API Documentation To build the
-API documentation do the following from this projects root directory: 1.
-Install required packages: ```bash python3 -m pip install tiledb-cf[docs] ```
-2. Make the HTML document: ```bash make -C docs/ html ``` 3. Open [docs/_build/
-html/index.html](./docs/_build/html/index.html) in a web browser of your
-choice. #### Example Notebooks Example Jupyter notebooks are available in the
+Keywords: tiledb,climate,forecast,netcdf Classifier: Development Status :: 3 -
+Alpha Classifier: Intended Audience :: Developers Classifier: Intended Audience
+:: Information Technology Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
+:: OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.7 Classifier: Programming Language ::
+Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: Implementation :: PyPy Classifier: Topic ::
+Software Development Requires-Python: >=3.7 Description-Content-Type: text/
+markdown Provides-Extra: docs Provides-Extra: netCDF4 Provides-Extra: xarray
+Provides-Extra: parallel Provides-Extra: examples License-File: LICENSE [TileDB
+logo] # TileDB-CF-Py The TileDB-CF-Py library is a Python library for
+supporting the NetCDF data model in the [TileDB storage engine](https://
+github.com/TileDB-Inc/TileDB). TileDB-CF-Py provides readers and writers for
+viewing and manipulating TileDB arrays and groups using TileDB CF Dataspaces -
+a special TileDB group that follows the requirements in [tiledb-cf-spec.md]
+(tiledb-cf-spec.md). ## TileDB Quick Links * [Homepage](https://tiledb.com) *
+[Documentation](https://docs.tiledb.com/main/) * [Forum](https://
+forum.tiledb.io/) * [Organization](https://github.com/TileDB-Inc/) ## Getting
+Started ### Quick Installation This project is available from [PyPI](https://
+pypi.org/project/tiledb/) and may be installed with ``pip``: ```bash pip
+install tiledb-cf ``` ### Documentation #### API Documentation To build the API
+documentation do the following from this projects root directory: 1. Install
+required packages: ```bash python3 -m pip install tiledb-cf[docs] ``` 2. Make
+the HTML document: ```bash make -C docs/ html ``` 3. Open [docs/_build/html/
+index.html](./docs/_build/html/index.html) in a web browser of your choice.
+#### Example Notebooks Example Jupyter notebooks are available in the
 [examples](./examples) folder. #### Command Line Interface TileDB-CF provides a
 command line interface. Currently, it has the following commands: ```bash
 Usage: tiledb-cf netcdf-convert [OPTIONS] Converts a NetCDF input file to
 nested TileDB groups. Options: -i, --input-file TEXT The path or URI to the
 NetCDF file that will be converted. [required] -o, --output-uri TEXT The URI
 for the output TileDB group. [required] --input-group-path TEXT The path in the
 input NetCDF for the root group that will be converted. [default: /] --
```

### Comparing `tiledb-cf-0.6.2/README.md` & `tiledb-cf-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `tiledb-cf-0.6.2/setup.cfg` & `tiledb-cf-0.7.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = tiledb-cf
-version = 0.6.2
+version = 0.7.0
 description = TileDB Python library for supporting Climate and Forecast datasets.
 author = TileDB, Inc.
 author_email = help@tiledb.io
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
 keywords = tiledb, climate, forecast, netcdf
@@ -31,15 +31,15 @@
 	tiledb.cf
 	tiledb.cf.netcdf_engine
 	tiledb.cf.xarray_engine
 python_requires = >=3.7
 install_requires = 
 	numpy >= 1.16.5
 	setuptools >= 40.4
-	tiledb >= 0.9.3
+	tiledb >= 0.21.2
 	click >= 0.7.0
 
 [options.extras_require]
 docs = 
 	Sphinx
 	sphinx-autodoc-typehints
 	sphinx-rtd-theme
@@ -51,15 +51,15 @@
 [options.entry_points]
 console_scripts = 
 	tiledb-cf = tiledb.cf:cli
 xarray.backends = 
 	tiledb = tiledb.cf.xarray_engine.backend_engine:TileDBBackendEntrypoint
 
 [flake8]
-ignore = E41,E203,E226,E302,E402,W503
+ignore = E41,E203,E226,E302,E402,W503,B024
 max-line-length = 88
 exclude = docs/* ./.*
 max-complexity = 10
 per-file-ignores = __init__.py:F401
 
 [mypy]
 ignore_missing_imports = True
```

### Comparing `tiledb-cf-0.6.2/tiledb/cf/__init__.py` & `tiledb-cf-0.7.0/tiledb/cf/__init__.py`

 * *Files identical despite different names*

### Comparing `tiledb-cf-0.6.2/tiledb/cf/cli.py` & `tiledb-cf-0.7.0/tiledb/cf/cli.py`

 * *Files identical despite different names*

### Comparing `tiledb-cf-0.6.2/tiledb/cf/core.py` & `tiledb-cf-0.7.0/tiledb/cf/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,18 +55,14 @@
         f'<tr><td style="text-align: left;">sparse={schema.sparse}</td></tr>\n'
     )
     if schema.sparse:
         output.write(
             f'<tr><td style="text-align: left;">allows_duplicates'
             f"={schema.allows_duplicates}</td></tr>\n"
         )
-    output.write(
-        f'<tr><td style="text-align: left">coords_filters={schema.coords_filters}'
-        f"</td>\n"
-    )
     output.write("</table>\n")
     output.write("</li>\n")
     output.write("</ul>\n")
     return output.getvalue()
 
 
 def _get_array_uri(group_uri: str, array_name: str, is_virtual: bool) -> str:
@@ -482,15 +478,16 @@
             array = array_names[0]
         array_key = (array, attr)
         tiledb_arrays = self._open_arrays.pop(array_key)
         if len(tiledb_arrays) > 1:
             with warnings.catch_warnings():
                 warnings.warn(
                     f"Closing more than one array reference with name: {array}."
-                    f"If you are using another reference it is now closed."
+                    f"If you are using another reference it is now closed.",
+                    stacklevel=3,
                 )
         for tdb_array in tiledb_arrays:
             tdb_array.close()
 
 
 class VirtualGroup(Group):
     """Class for accessing group metadata and arrays in a virtual TileDB group.
@@ -539,15 +536,16 @@
             is_virtual: (DEPRECATED) If ``True``, create arrays in a flat directory
                 without creating a TileDB group.
             append: If ``True``, add to existing group. Not valid for virtual groups.
         """
         if append:
             with warnings.catch_warnings():
                 warnings.warn(
-                    "Ignoring parameter append. Cannot append to a virtual group."
+                    "Ignoring parameter append. Cannot append to a virtual group.",
+                    stacklevel=3,
                 )
         if group_schema.metadata_schema is not None:
             tiledb.Array.create(
                 uri=_get_metadata_array_uri(uri, is_virtual=True),
                 schema=group_schema.metadata_schema,
                 key=_get_array_key(key, METADATA_ARRAY_NAME),
                 ctx=ctx,
@@ -692,15 +690,15 @@
         else:
             self._metadata_schema = metadata_schema
         if array_schemas is None:
             self._array_schema_table = {}
         else:
             self._array_schema_table = dict(array_schemas)
         self._attr_to_arrays: Dict[str, List[str]] = defaultdict(list)
-        for (schema_name, schema) in self._array_schema_table.items():
+        for schema_name, schema in self._array_schema_table.items():
             for attr in schema:
                 attr_name = attr.name
                 self._attr_to_arrays[attr_name].append(schema_name)
 
     def __eq__(self, other: Any):
         if not isinstance(other, GroupSchema):
             return False
```

### Comparing `tiledb-cf-0.6.2/tiledb/cf/creator.py` & `tiledb-cf-0.7.0/tiledb/cf/creator.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,15 +101,14 @@
         self,
         array_name: str,
         dims: Sequence[str],
         cell_order: str = "row-major",
         tile_order: str = "row-major",
         capacity: int = 0,
         tiles: Optional[Sequence[int]] = None,
-        coords_filters: Optional[tiledb.FilterList] = None,
         dim_filters: Optional[Dict[str, tiledb.FilterList]] = None,
         offsets_filters: Optional[tiledb.FilterList] = None,
         attrs_filters: Optional[tiledb.FilterList] = None,
         allows_duplicates: bool = False,
         sparse: bool = False,
     ):
         """Adds a new array to the CF dataspace.
@@ -127,19 +126,16 @@
                 curve.
             tile_order: The order in which TileDB stores the tiles on disk. Valid values
                 are: ``row-major`` or ``C`` (default) for row major; or ``col-major`` or
                 ``F`` for column major.
             capacity: The number of cells in a data tile of a sparse fragment.
             tiles: An optional ordered list of tile sizes for the dimensions of the
                 array. The length must match the number of dimensions in the array.
-            coords_filters: Filters for all dimensions that are not otherwise set by
-                ``dim_filters.``
             dim_filters: A dict from dimension name to a :class:`tiledb.FilterList`
-                for dimensions in the array. Overrides the values set in
-                ``coords_filters``.
+                for dimensions in the array.
             offsets_filters: Filters for the offsets for variable length attributes or
                 dimensions.
             attrs_filters: Default filters to use when adding an attribute to the
                 array.
             allows_duplicates: Specifies if multiple values can be stored at the same
                  coordinate. Only allowed for sparse arrays.
             sparse: Specifies if the array is a sparse TileDB array (true) or dense
@@ -149,15 +145,14 @@
             dataspace_registry=self._registry,
             name=array_name,
             dims=dims,
             cell_order=cell_order,
             tile_order=tile_order,
             capacity=capacity,
             tiles=tiles,
-            coords_filters=coords_filters,
             dim_filters=dim_filters,
             offsets_filters=offsets_filters,
             attrs_filters=attrs_filters,
             allows_duplicates=allows_duplicates,
             sparse=sparse,
         )
 
@@ -330,14 +325,15 @@
         array_schemas = {}
         for array_creator in self._registry.array_creators():
             try:
                 array_schemas[array_creator.name] = array_creator.to_schema(ctx)
             except tiledb.libtiledb.TileDBError as err:
                 raise RuntimeError(
                     f"Failed to create an ArraySchema for array '{array_creator.name}'."
+                    f" {str(err)}"
                 ) from err
         group_schema = GroupSchema(array_schemas)
         return group_schema
 
 
 class DataspaceRegistry:
     def __init__(self):
@@ -493,16 +489,14 @@
         cell_order: The order in which TileDB stores the cells on disk inside a
             tile. Valid values are: ``row-major`` (default) or ``C`` for row major;
             ``col-major`` or ``F`` for column major; or ``Hilbert`` for a Hilbert curve.
         tile_order: The order in which TileDB stores the tiles on disk. Valid values
             are: ``row-major`` or ``C`` (default) for row major; or ``col-major`` or
             ``F`` for column major.
         capacity: The number of cells in a data tile of a sparse fragment.
-        coords_filters: Filters for all dimensions that are not specified explicitly by
-            ``dim_filters``.
         offsets_filters: Filters for the offsets for variable length attributes or
             dimensions.
         attrs_filters: Default filters to use when adding an attribute to the array.
         allows_duplicates: Specifies if multiple values can be stored at the same
              coordinate. Only allowed for sparse arrays.
         sparse: If ``True``, creates a sparse array. Otherwise, create
     """
@@ -512,15 +506,14 @@
         dataspace_registry: DataspaceRegistry,
         name: str,
         dims: Sequence[str],
         cell_order: str = "row-major",
         tile_order: str = "row-major",
         capacity: int = 0,
         tiles: Optional[Sequence[int]] = None,
-        coords_filters: Optional[tiledb.FilterList] = None,
         dim_filters: Optional[Dict[str, tiledb.FilterList]] = None,
         offsets_filters: Optional[tiledb.FilterList] = None,
         attrs_filters: Optional[tiledb.FilterList] = None,
         allows_duplicates: bool = False,
         sparse: bool = False,
     ):
         if isinstance(dims, str):
@@ -534,15 +527,14 @@
             dataspace_registry, name, dims
         )
         self.cell_order = cell_order
         self.tile_order = tile_order
         self.capacity = capacity
         if tiles is not None:
             self._domain_creator.tiles = tiles
-        self.coords_filters = coords_filters
         if dim_filters is not None:
             for dim_name, filters in dim_filters.items():
                 self._domain_creator.dim_creator(dim_name).filters = filters
         self.offsets_filters = offsets_filters
         self.attrs_filters = attrs_filters
         self.allows_duplicates = allows_duplicates
         self.sparse = sparse
@@ -568,21 +560,14 @@
             f"     cell_order='{self.cell_order}',\n"
             f"     tile_order='{self.tile_order}',\n"
         )
         output.write(f"     capacity={self.capacity},\n")
         output.write(f"     sparse={self.sparse},\n")
         if self.sparse:
             output.write(f"     allows_duplicates={self.allows_duplicates},\n")
-        if self.coords_filters is not None:
-            output.write("     coords_filters=FilterList([")
-            for index, coord_filter in enumerate(self.coords_filters):
-                output.write(f"{repr(coord_filter)}")
-                if index < len(self.coords_filters):
-                    output.write(", ")
-            output.write("])\n")
         output.write("  )")
         return output.getvalue()
 
     def _register(
         self, dataspace_registry: DataspaceRegistry, name: str, dim_names: Sequence[str]
     ):
         dim_creators = tuple(
@@ -701,17 +686,14 @@
             f"<tr><td {cell_style}>sparse={self.sparse}</td></tr>\n"
         )
         if self.sparse:
             output.write(
                 f"<tr><td {cell_style}>allows_duplicates"
                 f"={self.allows_duplicates}</td></tr>\n"
             )
-        output.write(
-            f"<tr><td {cell_style}>coords_filters={self.coords_filters}</td></tr>\n"
-        )
         output.write("</table>\n")
         output.write("</li>\n")
         output.write("</ul>\n")
         return output.getvalue()
 
     def remove_attr_creator(self, attr_name):
         """Removes the requested attribute from the array.
@@ -733,15 +715,14 @@
         attrs = tuple(attr_creator.to_tiledb(ctx) for attr_creator in self)
         return tiledb.ArraySchema(
             domain=domain,
             attrs=attrs,
             cell_order=self.cell_order,
             tile_order=self.tile_order,
             capacity=self.capacity,
-            coords_filters=self.coords_filters,
             offsets_filters=self.offsets_filters,
             allows_duplicates=self.allows_duplicates,
             sparse=self.sparse,
             ctx=ctx,
         )
```

### Comparing `tiledb-cf-0.6.2/tiledb/cf/netcdf_engine/__init__.py` & `tiledb-cf-0.7.0/tiledb/cf/netcdf_engine/__init__.py`

 * *Files identical despite different names*

### Comparing `tiledb-cf-0.6.2/tiledb/cf/netcdf_engine/_array_converters.py` & `tiledb-cf-0.7.0/tiledb/cf/netcdf_engine/_array_converters.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,16 +27,14 @@
         cell_order: The order in which TileDB stores the cells on disk inside a
             tile. Valid values are: ``row-major`` (default) or ``C`` for row major;
             ``col-major`` or ``F`` for column major; or ``Hilbert`` for a Hilbert curve.
         tile_order: The order in which TileDB stores the tiles on disk. Valid values
             are: ``row-major`` or ``C`` (default) for row major; or ``col-major`` or
             ``F`` for column major.
         capacity: The number of cells in a data tile of a sparse fragment.
-        coords_filters: Filters for all dimensions that are not specified explicitly by
-            ``dim_filters``.
         offsets_filters: Filters for the offsets for variable length attributes or
             dimensions.
         attrs_filters: Default filters to use when adding an attribute to the array.
         allows_duplicates: Specifies if multiple values can be stored at the same
              coordinate. Only allowed for sparse arrays.
     """
```

### Comparing `tiledb-cf-0.6.2/tiledb/cf/netcdf_engine/_attr_converters.py` & `tiledb-cf-0.7.0/tiledb/cf/netcdf_engine/_attr_converters.py`

 * *Files identical despite different names*

### Comparing `tiledb-cf-0.6.2/tiledb/cf/netcdf_engine/_dim_converters.py` & `tiledb-cf-0.7.0/tiledb/cf/netcdf_engine/_dim_converters.py`

 * *Files identical despite different names*

### Comparing `tiledb-cf-0.6.2/tiledb/cf/netcdf_engine/_utils.py` & `tiledb-cf-0.7.0/tiledb/cf/netcdf_engine/_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,15 +50,16 @@
                 isinstance(value, str)
                 or not np.issubdtype(value.dtype, np.number)
                 or np.size(value) != 1
             ):
                 with warnings.catch_warnings():
                     warnings.warn(
                         f"Attribute '{key}' has value='{value}' that not a number. "
-                        f"Using default {key}={default} instead."
+                        f"Using default {key}={default} instead.",
+                        stacklevel=3,
                     )
                 return default
             if not np.isscalar(value):
                 value = value.item()
         return value
     return default
 
@@ -111,18 +112,33 @@
             values = scale_factor * values
         add_offset = get_netcdf_metadata(variable, "add_offset", is_number=True)
         if add_offset is not None:
             values = values + add_offset
     return values
 
 
-def get_variable_chunks(variable: netCDF4.Variable) -> Optional[Tuple[int, ...]]:
-    """Returns the chunks from a NetCDF variable if chunked and ``None`` otherwise."""
+def get_variable_chunks(
+    variable: netCDF4.Variable, unlimited_dim_size
+) -> Optional[Tuple[int, ...]]:
+    """
+    Returns the chunks from a NetCDF variable if chunked and ``None`` otherwise.
+
+
+    If one of the dimensions has a unlimited dimension, the chunk size will be
+    reduced to the unlimited_dim_size.
+    """
     chunks = variable.chunking()
-    return None if chunks is None or chunks == "contiguous" else tuple(chunks)
+    if chunks is None or chunks == "contiguous":
+        return None
+    return tuple(
+        min(ck, dim.size if unlimited_dim_size is None else unlimited_dim_size)
+        if dim.isunlimited()
+        else ck
+        for ck, dim in zip(chunks, variable.get_dims())
+    )
 
 
 @contextmanager
 def open_netcdf_group(
     group: Optional[Union[netCDF4.Dataset, netCDF4.Group]] = None,
     input_file: Optional[Union[str, Path]] = None,
     group_path: Optional[str] = None,
@@ -173,8 +189,11 @@
         value = tuple(value.tolist())
     elif isinstance(value, np.generic):
         value = (value.tolist(),)
     try:
         meta[key] = value
     except ValueError as err:  # pragma: no cover
         with warnings.catch_warnings():
-            warnings.warn(f"Failed to set metadata `{key}={value}` with error: {err}")
+            warnings.warn(
+                f"Failed to set metadata `{key}={value}` with error: {err}",
+                stacklevel=3,
+            )
```

### Comparing `tiledb-cf-0.6.2/tiledb/cf/netcdf_engine/api.py` & `tiledb-cf-0.7.0/tiledb/cf/netcdf_engine/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,14 @@
     tiles_by_var: Optional[Dict[str, Dict[str, Optional[Sequence[int]]]]] = None,
     tiles_by_dims: Optional[
         Dict[str, Dict[Sequence[str], Optional[Sequence[int]]]]
     ] = None,
     coords_to_dims: bool = False,
     collect_attrs: bool = True,
     unpack_vars: bool = False,
-    coords_filters: Optional[tiledb.FilterList] = None,
     offsets_filters: Optional[tiledb.FilterList] = None,
     attrs_filters: Optional[tiledb.FilterList] = None,
     copy_metadata: bool = True,
     use_virtual_groups: bool = False,
 ):
     """Converts a NetCDF input file to nested TileDB CF dataspaces.
 
@@ -63,15 +62,14 @@
             dimension into a TileDB dimension and the coordinate variable into a
             TileDB attribute.
         collect_attrs: If ``True``, store all attributes with the same dimensions in
             the same array. Otherwise, store each attribute in a scalar array.
         unpack_vars: Unpack NetCDF variables with NetCDF attributes ``scale_factor``
             or ``add_offset`` using the transformation ``scale_factor * value +
             unpack``.
-        coords_filters: Default filters for all dimensions.
         offsets_filters: Default filters for all offsets for variable attributes
             and dimensions.
         attrs_filters: Default filters for all attributes.
         copy_metadata: If  ``True`` copy NetCDF group and variable attributes to
             TileDB metadata. If ``False`` do not copy metadata.
         use_virtual_groups: If ``True``, create a virtual group using ``output_uri``
             as the name for the group metadata array. All other arrays will be named
@@ -93,15 +91,14 @@
             unlimited_dim_size,
             dim_dtype,
             tiles_by_var.get(netcdf_group.path),
             tiles_by_dims.get(netcdf_group.path),
             coords_to_dims=coords_to_dims,
             collect_attrs=collect_attrs,
             unpack_vars=unpack_vars,
-            coords_filters=coords_filters,
             offsets_filters=offsets_filters,
             attrs_filters=attrs_filters,
         )
         if use_virtual_groups:
             group_uri = (
                 output_uri
                 if netcdf_group.path == "/"
```

### Comparing `tiledb-cf-0.6.2/tiledb/cf/netcdf_engine/converter.py` & `tiledb-cf-0.7.0/tiledb/cf/netcdf_engine/converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,14 @@
         unlimited_dim_size: Optional[int] = None,
         dim_dtype: np.dtype = _DEFAULT_INDEX_DTYPE,
         tiles_by_var: Optional[Dict[str, Optional[Sequence[int]]]] = None,
         tiles_by_dims: Optional[Dict[Sequence[str], Optional[Sequence[int]]]] = None,
         coords_to_dims: bool = False,
         collect_attrs: bool = True,
         unpack_vars: bool = False,
-        coords_filters: Optional[tiledb.FilterList] = None,
         offsets_filters: Optional[tiledb.FilterList] = None,
         attrs_filters: Optional[tiledb.FilterList] = None,
     ):
         """Returns a :class:`NetCDF4ConverterEngine` from a group in a NetCDF file.
 
         Parameters:
             input_file: The input NetCDF file to generate the converter engine from.
@@ -76,15 +75,14 @@
                 dimension into a TileDB dimension and the coordinate variable into a
                 TileDB attribute.
             collect_attrs: If True, store all attributes with the same dimensions
                 in the same array. Otherwise, store each attribute in a scalar array.
             unpack_vars: Unpack NetCDF variables with NetCDF attributes ``scale_factor``
                 or ``add_offset`` using the transformation ``scale_factor * value +
                 unpack``.
-            coords_filters: Default filters for all dimensions.
             offsets_filters: Default filters for all offsets for variable attributes
                 and dimensions.
             attrs_filters: Default filters for all attributes.
         """
         with open_netcdf_group(input_file=input_file, group_path=group_path) as group:
             return cls.from_group(
                 group,
@@ -93,15 +91,14 @@
                 tiles_by_var,
                 tiles_by_dims,
                 default_input_file=input_file,
                 default_group_path=group_path,
                 coords_to_dims=coords_to_dims,
                 collect_attrs=collect_attrs,
                 unpack_vars=unpack_vars,
-                coords_filters=coords_filters,
                 offsets_filters=offsets_filters,
                 attrs_filters=attrs_filters,
             )
 
     @classmethod
     def from_group(
         cls,
@@ -109,15 +106,14 @@
         unlimited_dim_size: Optional[int] = None,
         dim_dtype: np.dtype = _DEFAULT_INDEX_DTYPE,
         tiles_by_var: Optional[Dict[str, Optional[Sequence[int]]]] = None,
         tiles_by_dims: Optional[Dict[Sequence[str], Optional[Sequence[int]]]] = None,
         coords_to_dims: bool = False,
         collect_attrs: bool = True,
         unpack_vars: bool = False,
-        coords_filters: Optional[tiledb.FilterList] = None,
         offsets_filters: Optional[tiledb.FilterList] = None,
         attrs_filters: Optional[tiledb.FilterList] = None,
         default_input_file: Optional[Union[str, Path]] = None,
         default_group_path: Optional[str] = None,
     ):
         """Returns a :class:`NetCDF4ConverterEngine` from a :class:`netCDF4.Group`.
 
@@ -136,15 +132,14 @@
                 dimension into a TileDB dimension and the coordinate variable into a
                 TileDB attribute.
             collect_attrs: If ``True``, store all attributes with the same dimensions
                 in the same array. Otherwise, store each attribute in a scalar array.
             unpack_vars: Unpack NetCDF variables with NetCDF attributes ``scale_factor``
                 or ``add_offset`` using the transformation ``scale_factor * value +
                 unpack``.
-            coords_filters: Default filters for all dimensions.
             offsets_filters: Default filters for all offsets for variable attributes
                 and dimensions.
             attrs_filters: Default filters for all attributes.
             default_input_file: If not ``None``, the default NetCDF input file to copy
                 data from.
             default_group_path: If not ``None``, the default NetCDF group to copy data
                 from. Use ``'/'`` to specify the root group.
@@ -154,30 +149,28 @@
                 netcdf_group=netcdf_group,
                 unlimited_dim_size=unlimited_dim_size,
                 dim_dtype=dim_dtype,
                 tiles_by_var=tiles_by_var,
                 tiles_by_dims=tiles_by_dims,
                 coords_to_dims=coords_to_dims,
                 unpack_vars=unpack_vars,
-                coords_filters=coords_filters,
                 offsets_filters=offsets_filters,
                 attrs_filters=attrs_filters,
                 default_input_file=default_input_file,
                 default_group_path=default_group_path,
             )
         return cls._from_group_to_attr_per_array(
             netcdf_group=netcdf_group,
             unlimited_dim_size=unlimited_dim_size,
             dim_dtype=dim_dtype,
             tiles_by_var=tiles_by_var,
             tiles_by_dims=tiles_by_dims,
             coords_to_dims=coords_to_dims,
             unpack_vars=unpack_vars,
             scalar_array_name="scalars",
-            coords_filters=coords_filters,
             offsets_filters=offsets_filters,
             attrs_filters=attrs_filters,
             default_input_file=default_input_file,
             default_group_path=default_group_path,
         )
 
     @classmethod  # noqa: C901
@@ -187,15 +180,14 @@
         unlimited_dim_size: Optional[int],
         dim_dtype: np.dtype,
         tiles_by_var: Optional[Dict[str, Optional[Sequence[int]]]],
         tiles_by_dims: Optional[Dict[Sequence[str], Optional[Sequence[int]]]],
         coords_to_dims: bool,
         scalar_array_name: str,
         unpack_vars: bool,
-        coords_filters: Optional[tiledb.FilterList],
         offsets_filters: Optional[tiledb.FilterList],
         attrs_filters: Optional[tiledb.FilterList],
         default_input_file: Optional[Union[str, Path]],
         default_group_path: Optional[str],
     ):
         """Returns a :class:`NetCDF4ConverterEngine` from a :class:`netCDF4.Group`.
 
@@ -218,15 +210,14 @@
                 TileDB attribute.
             scalar_array_name: Name for the array the stores all NetCDF scalar
                 variables. Cannot be the same name as any of the NetCDF variables in
                 the provided NetCDF group.
             unpack_vars: Unpack NetCDF variables with NetCDF attributes ``scale_factor``
                 or ``add_offset`` using the transformation ``scale_factor * value +
                 unpack``.
-            coords_filters: Default filters for all dimensions.
             offsets_filters: Default filters for all offsets for variable attributes
                 and dimensions.
             attrs_filters: Default filters for all attributes.
             default_input_file: If not ``None``, the default NetCDF input file to copy
                 data from.
             default_group_path: If not ``None``, the default NetCDF group to copy data
                 from. Use ``'/'`` to specify the root group.
@@ -252,15 +243,14 @@
                 if scalar_array_name not in {
                     array_creator.name for array_creator in converter.array_creators()
                 }:
                     converter.add_scalar_to_dim_converter("__scalars", dim_dtype)
                     converter.add_array_converter(
                         scalar_array_name,
                         ("__scalars",),
-                        coords_filters=coords_filters,
                         offsets_filters=offsets_filters,
                         attrs_filters=attrs_filters,
                     )
                 converter.add_var_to_attr_converter(ncvar, scalar_array_name)
             else:
                 for dim in ncvar.get_dims():
                     if dim.name not in {
@@ -275,23 +265,24 @@
                 has_coord_dim = any(
                     dim_name in coord_names for dim_name in ncvar.dimensions
                 )
                 tiles = tiles_by_var.get(
                     ncvar.name,
                     tiles_by_dims.get(
                         ncvar.dimensions,
-                        None if has_coord_dim else get_variable_chunks(ncvar),
+                        None
+                        if has_coord_dim
+                        else get_variable_chunks(ncvar, unlimited_dim_size),
                     ),
                 )
                 converter.add_array_converter(
                     array_name,
                     ncvar.dimensions,
                     tiles=tiles,
                     sparse=has_coord_dim,
-                    coords_filters=coords_filters,
                     offsets_filters=offsets_filters,
                     attrs_filters=attrs_filters,
                 )
                 converter.add_var_to_attr_converter(
                     ncvar, array_name, unpack=unpack_vars
                 )
         return converter
@@ -302,15 +293,14 @@
         netcdf_group: netCDF4.Group,
         unlimited_dim_size: Optional[int],
         dim_dtype: np.dtype,
         tiles_by_var: Optional[Dict[str, Optional[Sequence[int]]]],
         tiles_by_dims: Optional[Dict[Sequence[str], Optional[Sequence[int]]]],
         coords_to_dims: bool,
         unpack_vars: bool,
-        coords_filters: Optional[tiledb.FilterList],
         offsets_filters: Optional[tiledb.FilterList],
         attrs_filters: Optional[tiledb.FilterList],
         default_input_file: Optional[Union[str, Path]],
         default_group_path: Optional[str],
     ):
         """Returns a :class:`NetCDF4ConverterEngine` from a :class:`netCDF4.Group`.
 
@@ -330,15 +320,14 @@
             coords_to_dims: If ``True``, convert the NetCDF coordinate variable into a
                 TileDB dimension for sparse arrays. Otherwise, convert the coordinate
                 dimension into a TileDB dimension and the coordinate variable into a
                 TileDB attribute.
             unpack_vars: Unpack NetCDF variables with NetCDF attributes ``scale_factor``
                 or ``add_offset`` using the transformation ``scale_factor * value +
                 unpack``.
-            coords_filters: Default filters for all dimensions.
             offsets_filters: Default filters for all offsets for variable attributes
                 and dimensions.
             attrs_filters: Default filters for all attributes.
             default_input_file: If not ``None``, the default NetCDF input file to copy
                 data from.
             default_group_path: If not ``None``, the default NetCDF group to copy data
                 from. Use ``'/'`` to specify the root group.
@@ -362,15 +351,15 @@
                     converter.add_scalar_to_dim_converter("__scalars", dim_dtype)
                 dim_names = ncvar.dimensions if ncvar.dimensions else ("__scalars",)
                 dims_to_vars[dim_names].append(ncvar.name)
                 chunks = tiles_by_var.get(
                     ncvar.name,
                     None
                     if any(dim_name in coord_names for dim_name in ncvar.dimensions)
-                    else get_variable_chunks(ncvar),
+                    else get_variable_chunks(ncvar, unlimited_dim_size),
                 )
                 if chunks is not None:
                     autotiles[dim_names] = (
                         None
                         if dim_names in autotiles and chunks != autotiles[dim_names]
                         else chunks
                     )
@@ -391,15 +380,14 @@
             has_coord_dim = any(dim_name in coord_names for dim_name in dim_names)
             chunks = autotiles.get(dim_names)
             converter.add_array_converter(
                 f"array{count}",
                 dim_names,
                 tiles=chunks,
                 sparse=has_coord_dim,
-                coords_filters=coords_filters,
                 offsets_filters=offsets_filters,
                 attrs_filters=attrs_filters,
             )
             for var_name in dims_to_vars[dim_names]:
                 converter.add_var_to_attr_converter(
                     netcdf_group.variables[var_name],
                     f"array{count}",
@@ -484,15 +472,14 @@
         self,
         array_name: str,
         dims: Sequence[str],
         cell_order: str = "row-major",
         tile_order: str = "row-major",
         capacity: int = 0,
         tiles: Optional[Sequence[int]] = None,
-        coords_filters: Optional[tiledb.FilterList] = None,
         dim_filters: Optional[Dict[str, tiledb.FilterList]] = None,
         offsets_filters: Optional[tiledb.FilterList] = None,
         attrs_filters: Optional[tiledb.FilterList] = None,
         allows_duplicates: bool = False,
         sparse: bool = False,
     ):
         """Adds a new NetCDF to TileDB array converter to the CF dataspace.
@@ -510,18 +497,16 @@
                 curve.
             tile_order: The order in which TileDB stores the tiles on disk. Valid values
                 are: ``row-major`` or ``C`` (default) for row major; or ``col-major`` or
                 ``F`` for column major.
             capacity: The number of cells in a data tile of a sparse fragment.
             tiles: An optional ordered list of tile sizes for the dimensions of the
                 array. The length must match the number of dimensions in the array.
-            coords_filters: Filters for all dimensions that are not otherwise set by
-                ``dim_filters.``
             dim_filters: A dict from dimension name to a ``FilterList`` for dimensions
-                in the array. Overrides the values set in ``coords_filters``.
+                in the array.
             offsets_filters: Filters for the offsets for variable length attributes or
                 dimensions.
             attrs_filters: Default filters to use when adding an attribute to the array.
             allows_duplicates: Specifies if multiple values can be stored at the same
                  coordinate. Only allowed for sparse arrays.
             sparse: Specifies if the array is a sparse TileDB array (true) or dense
                 TileDB array (false).
@@ -530,15 +515,14 @@
             dataspace_registry=self._registry,
             name=array_name,
             dims=dims,
             cell_order=cell_order,
             tile_order=tile_order,
             capacity=capacity,
             tiles=tiles,
-            coords_filters=coords_filters,
             dim_filters=dim_filters,
             offsets_filters=offsets_filters,
             attrs_filters=attrs_filters,
             allows_duplicates=allows_duplicates,
             sparse=sparse,
         )
```

### Comparing `tiledb-cf-0.6.2/tiledb/cf/xarray_engine/backend_engine.py` & `tiledb-cf-0.7.0/tiledb/cf/xarray_engine/backend_engine.py`

 * *Files identical despite different names*

### Comparing `tiledb-cf-0.6.2/tiledb_cf.egg-info/PKG-INFO` & `tiledb-cf-0.7.0/tiledb_cf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: tiledb-cf
-Version: 0.6.2
+Version: 0.7.0
 Summary: TileDB Python library for supporting Climate and Forecast datasets.
 Home-page: https://github.com/TileDB-Inc/TileDB-CF-Py
 Author: TileDB, Inc.
 Author-email: help@tiledb.io
 License: MIT
 Project-URL: Documentation, https://docs.tiledb.com
 Keywords: tiledb,climate,forecast,netcdf
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -100,9 +99,7 @@
 
   --help                          Show this message and exit.
 ```
 
 ## Development
 
 For information on contributing to this project see the [CONTRIBUTING](CONTRIBUTING.md) document.
-
-
```

#### html2text {}

```diff
@@ -1,38 +1,38 @@
-Metadata-Version: 2.1 Name: tiledb-cf Version: 0.6.2 Summary: TileDB Python
+Metadata-Version: 2.1 Name: tiledb-cf Version: 0.7.0 Summary: TileDB Python
 library for supporting Climate and Forecast datasets. Home-page: https://
 github.com/TileDB-Inc/TileDB-CF-Py Author: TileDB, Inc. Author-email:
 help@tiledb.io License: MIT Project-URL: Documentation, https://docs.tiledb.com
-Keywords: tiledb,climate,forecast,netcdf Platform: UNKNOWN Classifier:
-Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Information Technology Classifier: Intended
-Audience :: Science/Research Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent Classifier: Programming Language
-:: Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: Implementation ::
-PyPy Classifier: Topic :: Software Development Requires-Python: >=3.7
-Description-Content-Type: text/markdown Provides-Extra: docs Provides-Extra:
-netCDF4 Provides-Extra: xarray Provides-Extra: parallel Provides-Extra:
-examples License-File: LICENSE [TileDB_logo] # TileDB-CF-Py The TileDB-CF-Py
-library is a Python library for supporting the NetCDF data model in the [TileDB
-storage engine](https://github.com/TileDB-Inc/TileDB). TileDB-CF-Py provides
-readers and writers for viewing and manipulating TileDB arrays and groups using
-TileDB CF Dataspaces - a special TileDB group that follows the requirements in
-[tiledb-cf-spec.md](tiledb-cf-spec.md). ## TileDB Quick Links * [Homepage]
-(https://tiledb.com) * [Documentation](https://docs.tiledb.com/main/) * [Forum]
-(https://forum.tiledb.io/) * [Organization](https://github.com/TileDB-Inc/) ##
-Getting Started ### Quick Installation This project is available from [PyPI]
-(https://pypi.org/project/tiledb/) and may be installed with ``pip``: ```bash
-pip install tiledb-cf ``` ### Documentation #### API Documentation To build the
-API documentation do the following from this projects root directory: 1.
-Install required packages: ```bash python3 -m pip install tiledb-cf[docs] ```
-2. Make the HTML document: ```bash make -C docs/ html ``` 3. Open [docs/_build/
-html/index.html](./docs/_build/html/index.html) in a web browser of your
-choice. #### Example Notebooks Example Jupyter notebooks are available in the
+Keywords: tiledb,climate,forecast,netcdf Classifier: Development Status :: 3 -
+Alpha Classifier: Intended Audience :: Developers Classifier: Intended Audience
+:: Information Technology Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
+:: OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.7 Classifier: Programming Language ::
+Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: Implementation :: PyPy Classifier: Topic ::
+Software Development Requires-Python: >=3.7 Description-Content-Type: text/
+markdown Provides-Extra: docs Provides-Extra: netCDF4 Provides-Extra: xarray
+Provides-Extra: parallel Provides-Extra: examples License-File: LICENSE [TileDB
+logo] # TileDB-CF-Py The TileDB-CF-Py library is a Python library for
+supporting the NetCDF data model in the [TileDB storage engine](https://
+github.com/TileDB-Inc/TileDB). TileDB-CF-Py provides readers and writers for
+viewing and manipulating TileDB arrays and groups using TileDB CF Dataspaces -
+a special TileDB group that follows the requirements in [tiledb-cf-spec.md]
+(tiledb-cf-spec.md). ## TileDB Quick Links * [Homepage](https://tiledb.com) *
+[Documentation](https://docs.tiledb.com/main/) * [Forum](https://
+forum.tiledb.io/) * [Organization](https://github.com/TileDB-Inc/) ## Getting
+Started ### Quick Installation This project is available from [PyPI](https://
+pypi.org/project/tiledb/) and may be installed with ``pip``: ```bash pip
+install tiledb-cf ``` ### Documentation #### API Documentation To build the API
+documentation do the following from this projects root directory: 1. Install
+required packages: ```bash python3 -m pip install tiledb-cf[docs] ``` 2. Make
+the HTML document: ```bash make -C docs/ html ``` 3. Open [docs/_build/html/
+index.html](./docs/_build/html/index.html) in a web browser of your choice.
+#### Example Notebooks Example Jupyter notebooks are available in the
 [examples](./examples) folder. #### Command Line Interface TileDB-CF provides a
 command line interface. Currently, it has the following commands: ```bash
 Usage: tiledb-cf netcdf-convert [OPTIONS] Converts a NetCDF input file to
 nested TileDB groups. Options: -i, --input-file TEXT The path or URI to the
 NetCDF file that will be converted. [required] -o, --output-uri TEXT The URI
 for the output TileDB group. [required] --input-group-path TEXT The path in the
 input NetCDF for the root group that will be converted. [default: /] --
```

### Comparing `tiledb-cf-0.6.2/tiledb_cf.egg-info/SOURCES.txt` & `tiledb-cf-0.7.0/tiledb_cf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

