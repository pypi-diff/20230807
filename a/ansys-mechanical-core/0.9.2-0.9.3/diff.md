# Comparing `tmp/ansys_mechanical_core-0.9.2.tar.gz` & `tmp/ansys_mechanical_core-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys_mechanical_core-0.9.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ansys_mechanical_core-0.9.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ansys_mechanical_core-0.9.2.tar` & `ansys_mechanical_core-0.9.3.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0     1089 2023-07-07 14:00:26.682650 ansys_mechanical_core-0.9.2/LICENSE
--rw-r--r--   0        0        0     5448 2023-07-07 14:00:26.682650 ansys_mechanical_core-0.9.2/README.rst
--rw-r--r--   0        0        0     4042 2023-07-07 14:00:26.694651 ansys_mechanical_core-0.9.2/pyproject.toml
--rw-r--r--   0        0        0     1236 2023-07-07 14:00:26.694651 ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/__init__.py
--rw-r--r--   0        0        0      536 2023-07-07 14:00:26.694651 ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/_version.py
--rw-r--r--   0        0        0      138 2023-07-07 14:00:26.694651 ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/embedding/__init__.py
--rw-r--r--   0        0        0     4793 2023-07-07 14:00:26.694651 ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/embedding/app.py
--rw-r--r--   0        0        0     1392 2023-07-07 14:00:26.694651 ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/embedding/config.py
--rw-r--r--   0        0        0      819 2023-07-07 14:00:26.694651 ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/embedding/imports.py
--rw-r--r--   0        0        0     6568 2023-07-07 14:00:26.694651 ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/embedding/initializer.py
--rw-r--r--   0        0        0     1958 2023-07-07 14:00:26.694651 ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/embedding/loader.py
--rw-r--r--   0        0        0     6761 2023-07-07 14:00:26.694651 ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/embedding/logger/__init__.py
--rw-r--r--   0        0        0     4603 2023-07-07 14:00:26.694651 ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/embedding/logger/environ.py
--rw-r--r--   0        0        0     4834 2023-07-07 14:00:26.694651 ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/embedding/logger/linux_api.py
--rw-r--r--   0        0        0      238 2023-07-07 14:00:26.694651 ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/embedding/logger/sinks.py
--rw-r--r--   0        0        0     4094 2023-07-07 14:00:26.694651 ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/embedding/logger/windows_api.py
--rw-r--r--   0        0        0      852 2023-07-07 14:00:26.694651 ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/embedding/resolver.py
--rw-r--r--   0        0        0     1287 2023-07-07 14:00:26.694651 ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/embedding/runtime.py
--rw-r--r--   0        0        0      703 2023-07-07 14:00:26.694651 ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/embedding/shims.py
--rw-r--r--   0        0        0     3312 2023-07-07 14:00:26.694651 ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/errors.py
--rw-r--r--   0        0        0      113 2023-07-07 14:00:26.694651 ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/examples/__init__.py
--rw-r--r--   0        0        0     2990 2023-07-07 14:00:26.694651 ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/examples/downloads.py
--rw-r--r--   0        0        0     5505 2023-07-07 14:00:26.694651 ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/launcher.py
--rw-r--r--   0        0        0    23658 2023-07-07 14:00:26.694651 ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/logging.py
--rw-r--r--   0        0        0    78531 2023-07-07 14:00:26.694651 ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/mechanical.py
--rw-r--r--   0        0        0     4215 2023-07-07 14:00:26.694651 ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/misc.py
--rw-r--r--   0        0        0    25279 2023-07-07 14:00:26.694651 ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/pool.py
--rw-r--r--   0        0        0     8155 1970-01-01 00:00:00.000000 ansys_mechanical_core-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-07-27 14:02:39.302520 ansys_mechanical_core-0.9.3/LICENSE
+-rw-r--r--   0        0        0     5453 2023-07-27 14:02:39.302520 ansys_mechanical_core-0.9.3/README.rst
+-rw-r--r--   0        0        0     4185 2023-07-27 14:02:39.306520 ansys_mechanical_core-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0     1236 2023-07-27 14:02:39.310520 ansys_mechanical_core-0.9.3/src/ansys/mechanical/core/__init__.py
+-rw-r--r--   0        0        0      536 2023-07-27 14:02:39.310520 ansys_mechanical_core-0.9.3/src/ansys/mechanical/core/_version.py
+-rw-r--r--   0        0        0      138 2023-07-27 14:02:39.310520 ansys_mechanical_core-0.9.3/src/ansys/mechanical/core/embedding/__init__.py
+-rw-r--r--   0        0        0     4793 2023-07-27 14:02:39.310520 ansys_mechanical_core-0.9.3/src/ansys/mechanical/core/embedding/app.py
+-rw-r--r--   0        0        0     1392 2023-07-27 14:02:39.310520 ansys_mechanical_core-0.9.3/src/ansys/mechanical/core/embedding/config.py
+-rw-r--r--   0        0        0      819 2023-07-27 14:02:39.310520 ansys_mechanical_core-0.9.3/src/ansys/mechanical/core/embedding/imports.py
+-rw-r--r--   0        0        0     6568 2023-07-27 14:02:39.310520 ansys_mechanical_core-0.9.3/src/ansys/mechanical/core/embedding/initializer.py
+-rw-r--r--   0        0        0     1561 2023-07-27 14:02:39.310520 ansys_mechanical_core-0.9.3/src/ansys/mechanical/core/embedding/loader.py
+-rw-r--r--   0        0        0     6761 2023-07-27 14:02:39.310520 ansys_mechanical_core-0.9.3/src/ansys/mechanical/core/embedding/logger/__init__.py
+-rw-r--r--   0        0        0     4603 2023-07-27 14:02:39.310520 ansys_mechanical_core-0.9.3/src/ansys/mechanical/core/embedding/logger/environ.py
+-rw-r--r--   0        0        0     4834 2023-07-27 14:02:39.310520 ansys_mechanical_core-0.9.3/src/ansys/mechanical/core/embedding/logger/linux_api.py
+-rw-r--r--   0        0        0      238 2023-07-27 14:02:39.310520 ansys_mechanical_core-0.9.3/src/ansys/mechanical/core/embedding/logger/sinks.py
+-rw-r--r--   0        0        0     4094 2023-07-27 14:02:39.310520 ansys_mechanical_core-0.9.3/src/ansys/mechanical/core/embedding/logger/windows_api.py
+-rw-r--r--   0        0        0      852 2023-07-27 14:02:39.310520 ansys_mechanical_core-0.9.3/src/ansys/mechanical/core/embedding/resolver.py
+-rw-r--r--   0        0        0     1287 2023-07-27 14:02:39.310520 ansys_mechanical_core-0.9.3/src/ansys/mechanical/core/embedding/runtime.py
+-rw-r--r--   0        0        0      703 2023-07-27 14:02:39.310520 ansys_mechanical_core-0.9.3/src/ansys/mechanical/core/embedding/shims.py
+-rw-r--r--   0        0        0     3312 2023-07-27 14:02:39.310520 ansys_mechanical_core-0.9.3/src/ansys/mechanical/core/errors.py
+-rw-r--r--   0        0        0      113 2023-07-27 14:02:39.310520 ansys_mechanical_core-0.9.3/src/ansys/mechanical/core/examples/__init__.py
+-rw-r--r--   0        0        0     2990 2023-07-27 14:02:39.310520 ansys_mechanical_core-0.9.3/src/ansys/mechanical/core/examples/downloads.py
+-rw-r--r--   0        0        0     5505 2023-07-27 14:02:39.310520 ansys_mechanical_core-0.9.3/src/ansys/mechanical/core/launcher.py
+-rw-r--r--   0        0        0    23658 2023-07-27 14:02:39.310520 ansys_mechanical_core-0.9.3/src/ansys/mechanical/core/logging.py
+-rw-r--r--   0        0        0    78531 2023-07-27 14:02:39.310520 ansys_mechanical_core-0.9.3/src/ansys/mechanical/core/mechanical.py
+-rw-r--r--   0        0        0     4215 2023-07-27 14:02:39.310520 ansys_mechanical_core-0.9.3/src/ansys/mechanical/core/misc.py
+-rw-r--r--   0        0        0    25279 2023-07-27 14:02:39.310520 ansys_mechanical_core-0.9.3/src/ansys/mechanical/core/pool.py
+-rw-r--r--   0        0        0     5024 2023-07-27 14:02:39.310520 ansys_mechanical_core-0.9.3/src/ansys/mechanical/core/run.py
+-rw-r--r--   0        0        0     8149 1970-01-01 00:00:00.000000 ansys_mechanical_core-0.9.3/PKG-INFO
```

### Comparing `ansys_mechanical_core-0.9.2/LICENSE` & `ansys_mechanical_core-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys_mechanical_core-0.9.2/README.rst` & `ansys_mechanical_core-0.9.3/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
 and later. Here is an example:
 
 .. code:: python
 
    import ansys.mechanical.core as pymechanical
 
    app = pymechanical.App()
-   result = app.ExtAPI.DataModel.Project.ProjectDirectory
+   project_dir = app.ExtAPI.DataModel.Project.ProjectDirectory
 
 Testing and Development
 -----------------------
 If you would like to test or contribute to the development of PyMechanical, please visit
 `PyMechanical - Contributing <https://mechanical.docs.pyansys.com/version/stable/contributing.html>`_.
 
 .. LINKS AND REFERENCES
```

### Comparing `ansys_mechanical_core-0.9.2/pyproject.toml` & `ansys_mechanical_core-0.9.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 # Check https://flit.readthedocs.io/en/latest/pyproject_toml.html for all available sections
 name = "ansys-mechanical-core"
-version = "0.9.2"
+version = "0.9.3"
 description = "A python wrapper for Ansys Mechanical"
 readme = "README.rst"
 requires-python = ">=3.7,<4.0"
 license = {file = "LICENSE"}
 authors = [
     {name = "ANSYS, Inc.", email = "pyansys.core@ansys.com"},
 ]
@@ -26,21 +26,21 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "ansys_api_mechanical==0.1.0",
+    "ansys-platform-instancemanagement>=1.0.1",
     "ansys-pythonnet>=3.1.0rc1",
-    "ansys-tools-path>=0.2.6",
-    "importlib-metadata>=4.0",
+    "ansys-tools-path>=0.3.1",
     "appdirs>=1.4.0",
+    "click>=8.1.3", # for CLI interface
     "grpcio>=1.30.0",
     "protobuf>=3.12.2,<3.21.0",
-    "ansys-platform-instancemanagement>=1.0.1",
     "tqdm>=4.45.0",
 ]
 
 [project.urls]
 Documentation = "https://mechanical.docs.pyansys.com"
 Source = "https://github.com/ansys/pymechanical"
 Homepage = "https://github.com/ansys/pymechanical"
@@ -51,36 +51,39 @@
     "pytest==7.4.0",
     "pytest-cov==4.1.0",
     "pytest-print==0.3.3",
 ]
 doc = [
     "Sphinx==6.2.1", # BLOCKED BY sphinx-design - Cannot upgrade to Sphinx 7 for now
     "ansys-sphinx-theme==0.9.9",
-    "grpcio==1.56.0",
+    "grpcio==1.56.2",
     "imageio-ffmpeg==0.4.8",
     "imageio==2.31.1",
     "jupyter_sphinx==0.4.0",
     "jupyterlab>=3.2.8",
-    "matplotlib==3.7.1",
+    "matplotlib==3.7.2",
     "numpydoc==1.5.0",
     "plotly==5.15.0",
     "pypandoc==1.11",
     "pytest-sphinx==0.5.0",
     "pythreejs==2.4.2",
-    "pyvista==0.40.0",
+    "pyvista==0.41.1",
     "sphinx-autobuild==2021.3.14",
-    "sphinx-autodoc-typehints==1.23.0",
+    "sphinx-autodoc-typehints==1.23.0", # BLOCKED BY sphinx-design - Cannot upgrade to Sphinx 7 for now
     "sphinx-copybutton==0.5.2",
     "sphinx_design==0.4.1",
     "sphinx-gallery==0.13.0",
     "sphinx-notfound-page==0.8.3",
     "sphinxcontrib-websupport==1.2.4",
     "sphinxemoji==0.2.0",
 ]
 
+[project.scripts]
+ansys-mechanical = "ansys.mechanical.core.run:cli"
+
 [tool.flit.module]
 name = "ansys.mechanical.core"
 
 [tool.black]
 line-length = 100
 
 [tool.isort]
```

### Comparing `ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/__init__.py` & `ansys_mechanical_core-0.9.3/src/ansys/mechanical/core/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/_version.py` & `ansys_mechanical_core-0.9.3/src/ansys/mechanical/core/_version.py`

 * *Files identical despite different names*

### Comparing `ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/embedding/app.py` & `ansys_mechanical_core-0.9.3/src/ansys/mechanical/core/embedding/app.py`

 * *Files identical despite different names*

### Comparing `ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/embedding/config.py` & `ansys_mechanical_core-0.9.3/src/ansys/mechanical/core/embedding/config.py`

 * *Files identical despite different names*

### Comparing `ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/embedding/imports.py` & `ansys_mechanical_core-0.9.3/src/ansys/mechanical/core/embedding/imports.py`

 * *Files identical despite different names*

### Comparing `ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/embedding/initializer.py` & `ansys_mechanical_core-0.9.3/src/ansys/mechanical/core/embedding/initializer.py`

 * *Files identical despite different names*

### Comparing `ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/embedding/loader.py` & `ansys_mechanical_core-0.9.3/src/ansys/mechanical/core/embedding/loader.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,14 @@
 """clr_loader for pymechanical embedding. This loads the CLR on both windows and linux."""
+from importlib.metadata import version
 import os
 
-try:
-    from importlib.metadata import version
-
-    HAS_IMPORTLIB = True
-except:  # pragma: no cover
-    # TODO - only support importlib.metadata::version after dropping python3.7 support.
-    # pkg_resources is part of distutils and is considered obsolete.
-    import pkg_resources
-
-    HAS_IMPORTLIB = False
-
 
 def __get_clr_loader_version():
-    if HAS_IMPORTLIB:
-        return version("clr_loader")
-    else:  # pragma: no cover
-        return pkg_resources.get_distribution("clr_loader").version
+    return version("clr_loader")
 
 
 def __get_mono(assembly_dir, config_dir):
     import clr_loader
 
     if __get_clr_loader_version() == "0.2.5":
         libmono = os.path.join(assembly_dir, "libmonosgen-2.0.so")
```

### Comparing `ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/embedding/logger/__init__.py` & `ansys_mechanical_core-0.9.3/src/ansys/mechanical/core/embedding/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/embedding/logger/environ.py` & `ansys_mechanical_core-0.9.3/src/ansys/mechanical/core/embedding/logger/environ.py`

 * *Files identical despite different names*

### Comparing `ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/embedding/logger/linux_api.py` & `ansys_mechanical_core-0.9.3/src/ansys/mechanical/core/embedding/logger/linux_api.py`

 * *Files identical despite different names*

### Comparing `ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/embedding/logger/windows_api.py` & `ansys_mechanical_core-0.9.3/src/ansys/mechanical/core/embedding/logger/windows_api.py`

 * *Files identical despite different names*

### Comparing `ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/embedding/resolver.py` & `ansys_mechanical_core-0.9.3/src/ansys/mechanical/core/embedding/resolver.py`

 * *Files identical despite different names*

### Comparing `ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/embedding/runtime.py` & `ansys_mechanical_core-0.9.3/src/ansys/mechanical/core/embedding/runtime.py`

 * *Files identical despite different names*

### Comparing `ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/embedding/shims.py` & `ansys_mechanical_core-0.9.3/src/ansys/mechanical/core/embedding/shims.py`

 * *Files identical despite different names*

### Comparing `ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/errors.py` & `ansys_mechanical_core-0.9.3/src/ansys/mechanical/core/errors.py`

 * *Files identical despite different names*

### Comparing `ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/examples/downloads.py` & `ansys_mechanical_core-0.9.3/src/ansys/mechanical/core/examples/downloads.py`

 * *Files identical despite different names*

### Comparing `ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/launcher.py` & `ansys_mechanical_core-0.9.3/src/ansys/mechanical/core/launcher.py`

 * *Files identical despite different names*

### Comparing `ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/logging.py` & `ansys_mechanical_core-0.9.3/src/ansys/mechanical/core/logging.py`

 * *Files identical despite different names*

### Comparing `ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/mechanical.py` & `ansys_mechanical_core-0.9.3/src/ansys/mechanical/core/mechanical.py`

 * *Files identical despite different names*

### Comparing `ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/misc.py` & `ansys_mechanical_core-0.9.3/src/ansys/mechanical/core/misc.py`

 * *Files identical despite different names*

### Comparing `ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/pool.py` & `ansys_mechanical_core-0.9.3/src/ansys/mechanical/core/pool.py`

 * *Files identical despite different names*

### Comparing `ansys_mechanical_core-0.9.2/PKG-INFO` & `ansys_mechanical_core-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansys-mechanical-core
-Version: 0.9.2
+Version: 0.9.3
 Summary: A python wrapper for Ansys Mechanical
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Requires-Python: >=3.7,<4.0
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -12,36 +12,36 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Dist: ansys_api_mechanical==0.1.0
+Requires-Dist: ansys-platform-instancemanagement>=1.0.1
 Requires-Dist: ansys-pythonnet>=3.1.0rc1
-Requires-Dist: ansys-tools-path>=0.2.6
-Requires-Dist: importlib-metadata>=4.0
+Requires-Dist: ansys-tools-path>=0.3.1
 Requires-Dist: appdirs>=1.4.0
+Requires-Dist: click>=8.1.3
 Requires-Dist: grpcio>=1.30.0
 Requires-Dist: protobuf>=3.12.2,<3.21.0
-Requires-Dist: ansys-platform-instancemanagement>=1.0.1
 Requires-Dist: tqdm>=4.45.0
 Requires-Dist: Sphinx==6.2.1 ; extra == "doc"
 Requires-Dist: ansys-sphinx-theme==0.9.9 ; extra == "doc"
-Requires-Dist: grpcio==1.56.0 ; extra == "doc"
+Requires-Dist: grpcio==1.56.2 ; extra == "doc"
 Requires-Dist: imageio-ffmpeg==0.4.8 ; extra == "doc"
 Requires-Dist: imageio==2.31.1 ; extra == "doc"
 Requires-Dist: jupyter_sphinx==0.4.0 ; extra == "doc"
 Requires-Dist: jupyterlab>=3.2.8 ; extra == "doc"
-Requires-Dist: matplotlib==3.7.1 ; extra == "doc"
+Requires-Dist: matplotlib==3.7.2 ; extra == "doc"
 Requires-Dist: numpydoc==1.5.0 ; extra == "doc"
 Requires-Dist: plotly==5.15.0 ; extra == "doc"
 Requires-Dist: pypandoc==1.11 ; extra == "doc"
 Requires-Dist: pytest-sphinx==0.5.0 ; extra == "doc"
 Requires-Dist: pythreejs==2.4.2 ; extra == "doc"
-Requires-Dist: pyvista==0.40.0 ; extra == "doc"
+Requires-Dist: pyvista==0.41.1 ; extra == "doc"
 Requires-Dist: sphinx-autobuild==2021.3.14 ; extra == "doc"
 Requires-Dist: sphinx-autodoc-typehints==1.23.0 ; extra == "doc"
 Requires-Dist: sphinx-copybutton==0.5.2 ; extra == "doc"
 Requires-Dist: sphinx_design==0.4.1 ; extra == "doc"
 Requires-Dist: sphinx-gallery==0.13.0 ; extra == "doc"
 Requires-Dist: sphinx-notfound-page==0.8.3 ; extra == "doc"
 Requires-Dist: sphinxcontrib-websupport==1.2.4 ; extra == "doc"
@@ -162,15 +162,15 @@
 and later. Here is an example:
 
 .. code:: python
 
    import ansys.mechanical.core as pymechanical
 
    app = pymechanical.App()
-   result = app.ExtAPI.DataModel.Project.ProjectDirectory
+   project_dir = app.ExtAPI.DataModel.Project.ProjectDirectory
 
 Testing and Development
 -----------------------
 If you would like to test or contribute to the development of PyMechanical, please visit
 `PyMechanical - Contributing <https://mechanical.docs.pyansys.com/version/stable/contributing.html>`_.
 
 .. LINKS AND REFERENCES
```

