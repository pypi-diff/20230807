# Comparing `tmp/pyaogmaneo-2.1.2.tar.gz` & `tmp/pyaogmaneo-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaogmaneo-2.1.2.tar", last modified: Mon Jul 31 00:20:52 2023, max compression
+gzip compressed data, was "pyaogmaneo-2.1.3.tar", last modified: Mon Aug  7 18:18:50 2023, max compression
```

## Comparing `pyaogmaneo-2.1.2.tar` & `pyaogmaneo-2.1.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-07-31 00:20:52.900270 pyaogmaneo-2.1.2/
-drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-07-31 00:20:52.900270 pyaogmaneo-2.1.2/CMake/
--rw-r--r--   0 ericl     (1000) ericl     (1001)     1250 2023-03-18 01:02:16.000000 pyaogmaneo-2.1.2/CMake/FindAOgmaNeo.cmake
--rw-r--r--   0 ericl     (1000) ericl     (1001)     2620 2023-07-31 00:18:20.000000 pyaogmaneo-2.1.2/CMakeLists.txt
--rw-r--r--   0 ericl     (1000) ericl     (1001)    17842 2022-12-03 02:07:03.000000 pyaogmaneo-2.1.2/LICENSE.md
--rw-r--r--   0 ericl     (1000) ericl     (1001)       64 2022-12-03 02:07:03.000000 pyaogmaneo-2.1.2/MANIFEST.in
--rw-r--r--   0 ericl     (1000) ericl     (1001)      785 2023-07-31 00:20:52.900270 pyaogmaneo-2.1.2/PKG-INFO
--rw-r--r--   0 ericl     (1000) ericl     (1001)     2412 2023-06-22 14:37:40.000000 pyaogmaneo-2.1.2/README.md
-drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-07-31 00:20:52.900270 pyaogmaneo-2.1.2/pyaogmaneo.egg-info/
--rw-r--r--   0 ericl     (1000) ericl     (1001)      785 2023-07-31 00:20:52.000000 pyaogmaneo-2.1.2/pyaogmaneo.egg-info/PKG-INFO
--rw-r--r--   0 ericl     (1000) ericl     (1001)      505 2023-07-31 00:20:52.000000 pyaogmaneo-2.1.2/pyaogmaneo.egg-info/SOURCES.txt
--rw-r--r--   0 ericl     (1000) ericl     (1001)        1 2023-07-31 00:20:52.000000 pyaogmaneo-2.1.2/pyaogmaneo.egg-info/dependency_links.txt
--rw-r--r--   0 ericl     (1000) ericl     (1001)        1 2023-06-29 17:53:40.000000 pyaogmaneo-2.1.2/pyaogmaneo.egg-info/not-zip-safe
--rw-r--r--   0 ericl     (1000) ericl     (1001)       11 2023-07-31 00:20:52.000000 pyaogmaneo-2.1.2/pyaogmaneo.egg-info/top_level.txt
--rw-r--r--   0 ericl     (1000) ericl     (1001)      101 2023-01-13 01:36:37.000000 pyaogmaneo-2.1.2/pyproject.toml
--rw-r--r--   0 ericl     (1000) ericl     (1001)       38 2023-07-31 00:20:52.900270 pyaogmaneo-2.1.2/setup.cfg
--rw-r--r--   0 ericl     (1000) ericl     (1001)     4204 2023-07-31 00:18:29.000000 pyaogmaneo-2.1.2/setup.py
-drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-07-31 00:20:52.900270 pyaogmaneo-2.1.2/source/
-drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-07-31 00:20:52.900270 pyaogmaneo-2.1.2/source/pyaogmaneo/
--rw-r--r--   0 ericl     (1000) ericl     (1001)     1071 2023-06-22 14:37:40.000000 pyaogmaneo-2.1.2/source/pyaogmaneo/py_helpers.cpp
--rw-r--r--   0 ericl     (1000) ericl     (1001)     1783 2023-06-22 14:37:40.000000 pyaogmaneo-2.1.2/source/pyaogmaneo/py_helpers.h
--rw-r--r--   0 ericl     (1000) ericl     (1001)    15776 2023-07-30 17:43:03.000000 pyaogmaneo-2.1.2/source/pyaogmaneo/py_hierarchy.cpp
--rw-r--r--   0 ericl     (1000) ericl     (1001)     7013 2023-07-30 17:43:03.000000 pyaogmaneo-2.1.2/source/pyaogmaneo/py_hierarchy.h
--rw-r--r--   0 ericl     (1000) ericl     (1001)     8140 2023-07-30 17:43:03.000000 pyaogmaneo-2.1.2/source/pyaogmaneo/py_image_encoder.cpp
--rw-r--r--   0 ericl     (1000) ericl     (1001)     3217 2023-07-26 01:03:23.000000 pyaogmaneo-2.1.2/source/pyaogmaneo/py_image_encoder.h
--rw-r--r--   0 ericl     (1000) ericl     (1001)     9243 2023-07-30 17:43:03.000000 pyaogmaneo-2.1.2/source/pyaogmaneo/py_module.cpp
+drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-08-07 18:18:50.048994 pyaogmaneo-2.1.3/
+drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-08-07 18:18:50.048994 pyaogmaneo-2.1.3/CMake/
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     1250 2023-03-18 01:02:16.000000 pyaogmaneo-2.1.3/CMake/FindAOgmaNeo.cmake
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     2620 2023-08-07 18:16:16.000000 pyaogmaneo-2.1.3/CMakeLists.txt
+-rw-r--r--   0 ericl     (1000) ericl     (1001)    17842 2022-12-03 02:07:03.000000 pyaogmaneo-2.1.3/LICENSE.md
+-rw-r--r--   0 ericl     (1000) ericl     (1001)       64 2022-12-03 02:07:03.000000 pyaogmaneo-2.1.3/MANIFEST.in
+-rw-r--r--   0 ericl     (1000) ericl     (1001)      785 2023-08-07 18:18:50.048994 pyaogmaneo-2.1.3/PKG-INFO
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     2412 2023-06-22 14:37:40.000000 pyaogmaneo-2.1.3/README.md
+drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-08-07 18:18:50.048994 pyaogmaneo-2.1.3/pyaogmaneo.egg-info/
+-rw-r--r--   0 ericl     (1000) ericl     (1001)      785 2023-08-07 18:18:49.000000 pyaogmaneo-2.1.3/pyaogmaneo.egg-info/PKG-INFO
+-rw-r--r--   0 ericl     (1000) ericl     (1001)      505 2023-08-07 18:18:50.000000 pyaogmaneo-2.1.3/pyaogmaneo.egg-info/SOURCES.txt
+-rw-r--r--   0 ericl     (1000) ericl     (1001)        1 2023-08-07 18:18:49.000000 pyaogmaneo-2.1.3/pyaogmaneo.egg-info/dependency_links.txt
+-rw-r--r--   0 ericl     (1000) ericl     (1001)        1 2023-06-29 17:53:40.000000 pyaogmaneo-2.1.3/pyaogmaneo.egg-info/not-zip-safe
+-rw-r--r--   0 ericl     (1000) ericl     (1001)       11 2023-08-07 18:18:49.000000 pyaogmaneo-2.1.3/pyaogmaneo.egg-info/top_level.txt
+-rw-r--r--   0 ericl     (1000) ericl     (1001)      101 2023-01-13 01:36:37.000000 pyaogmaneo-2.1.3/pyproject.toml
+-rw-r--r--   0 ericl     (1000) ericl     (1001)       38 2023-08-07 18:18:50.048994 pyaogmaneo-2.1.3/setup.cfg
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     4204 2023-08-07 18:16:35.000000 pyaogmaneo-2.1.3/setup.py
+drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-08-07 18:18:50.045661 pyaogmaneo-2.1.3/source/
+drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-08-07 18:18:50.048994 pyaogmaneo-2.1.3/source/pyaogmaneo/
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     1071 2023-06-22 14:37:40.000000 pyaogmaneo-2.1.3/source/pyaogmaneo/py_helpers.cpp
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     1783 2023-06-22 14:37:40.000000 pyaogmaneo-2.1.3/source/pyaogmaneo/py_helpers.h
+-rw-r--r--   0 ericl     (1000) ericl     (1001)    15776 2023-08-07 18:09:36.000000 pyaogmaneo-2.1.3/source/pyaogmaneo/py_hierarchy.cpp
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     7013 2023-08-07 18:09:36.000000 pyaogmaneo-2.1.3/source/pyaogmaneo/py_hierarchy.h
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     8140 2023-08-07 16:40:04.000000 pyaogmaneo-2.1.3/source/pyaogmaneo/py_image_encoder.cpp
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     3217 2023-08-07 18:16:54.000000 pyaogmaneo-2.1.3/source/pyaogmaneo/py_image_encoder.h
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     9236 2023-08-07 18:09:36.000000 pyaogmaneo-2.1.3/source/pyaogmaneo/py_module.cpp
```

### Comparing `pyaogmaneo-2.1.2/CMake/FindAOgmaNeo.cmake` & `pyaogmaneo-2.1.3/CMake/FindAOgmaNeo.cmake`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.1.2/CMakeLists.txt` & `pyaogmaneo-2.1.3/CMakeLists.txt`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     find_package(AOgmaNeo)
 else()
     message(STATUS "Not using system installation of AOgmaNeo, will download from repository")
 
     FetchContent_Declare(
         AOgmaNeo
         GIT_REPOSITORY https://github.com/ogmacorp/AOgmaNeo.git
-        GIT_TAG 50588dd81a02a94747abe79f2fb81c721a33f81d
+        GIT_TAG 8940111ea090e09c0d71820132e6c393145d99d9
     )
 
     FetchContent_GetProperties(AOgmaNeo)
 
     if(NOT AOgmaNeo_POPULATED)
         FetchContent_Populate(AOgmaNeo)
         add_subdirectory(${aogmaneo_SOURCE_DIR} ${aogmaneo_BINARY_DIR})
```

### Comparing `pyaogmaneo-2.1.2/LICENSE.md` & `pyaogmaneo-2.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.1.2/PKG-INFO` & `pyaogmaneo-2.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaogmaneo
-Version: 2.1.2
+Version: 2.1.3
 Summary: Python bindings for the AOgmaNeo library
 Home-page: https://ogmacorp.com/
 Author: Ogma Intelligent Systems Corp
 Author-email: info@ogmacorp.com
 License: Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `pyaogmaneo-2.1.2/README.md` & `pyaogmaneo-2.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.1.2/pyaogmaneo.egg-info/PKG-INFO` & `pyaogmaneo-2.1.3/pyaogmaneo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaogmaneo
-Version: 2.1.2
+Version: 2.1.3
 Summary: Python bindings for the AOgmaNeo library
 Home-page: https://ogmacorp.com/
 Author: Ogma Intelligent Systems Corp
 Author-email: info@ogmacorp.com
 License: Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `pyaogmaneo-2.1.2/setup.py` & `pyaogmaneo-2.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,15 @@
             os.makedirs(self.build_temp)
 
         subprocess.check_call([ 'cmake', ext.sourcedir ] + cmake_args, cwd=self.build_temp, env=env)
         subprocess.check_call([ 'cmake', '--build', '.' ] + build_args, cwd=self.build_temp)
 
 setup(
     name="pyaogmaneo",
-    version="2.1.2",
+    version="2.1.3",
     description="Python bindings for the AOgmaNeo library",
     long_description='https://github.com/ogmacorp/PyAOgmaNeo',
     author='Ogma Intelligent Systems Corp',
     author_email='info@ogmacorp.com',
     url='https://ogmacorp.com/',
     license='Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License',
     classifiers=[
```

### Comparing `pyaogmaneo-2.1.2/source/pyaogmaneo/py_helpers.cpp` & `pyaogmaneo-2.1.3/source/pyaogmaneo/py_helpers.cpp`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.1.2/source/pyaogmaneo/py_helpers.h` & `pyaogmaneo-2.1.3/source/pyaogmaneo/py_helpers.h`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.1.2/source/pyaogmaneo/py_hierarchy.cpp` & `pyaogmaneo-2.1.3/source/pyaogmaneo/py_hierarchy.cpp`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.1.2/source/pyaogmaneo/py_hierarchy.h` & `pyaogmaneo-2.1.3/source/pyaogmaneo/py_hierarchy.h`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.1.2/source/pyaogmaneo/py_image_encoder.cpp` & `pyaogmaneo-2.1.3/source/pyaogmaneo/py_image_encoder.cpp`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.1.2/source/pyaogmaneo/py_image_encoder.h` & `pyaogmaneo-2.1.3/source/pyaogmaneo/py_image_encoder.h`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 #pragma once
 
 #include "py_helpers.h"
 #include <aogmaneo/image_encoder.h>
 
 namespace pyaon {
-const int image_encoder_magic = 6221138;
+const int image_encoder_magic = 3251108;
 
 struct Image_Visible_Layer_Desc {
     std::tuple<int, int, int> size;
 
     int radius;
 
     Image_Visible_Layer_Desc(
```

### Comparing `pyaogmaneo-2.1.2/source/pyaogmaneo/py_module.cpp` & `pyaogmaneo-2.1.3/source/pyaogmaneo/py_module.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
                 int,
                 int
             >(),
             py::arg("size") = std::tuple<int, int, int>({ 4, 4, 16 }),
             py::arg("io_type") = pyaon::prediction,
             py::arg("up_radius") = 2,
             py::arg("down_radius") = 2,
-            py::arg("history_capacity") = 64
+            py::arg("history_capacity") = 128
         )
         .def_readwrite("size", &pyaon::IO_Desc::size)
         .def_readwrite("io_type", &pyaon::IO_Desc::type)
         .def_readwrite("up_radius", &pyaon::IO_Desc::up_radius)
         .def_readwrite("down_radius", &pyaon::IO_Desc::down_radius)
         .def_readwrite("history_capacity", &pyaon::IO_Desc::history_capacity);
 
@@ -80,16 +80,16 @@
         .def_readwrite("lr", &aon::Decoder::Params::lr)
         .def_readwrite("gcurve", &aon::Decoder::Params::gcurve);
 
     py::class_<aon::Actor::Params>(m, "ActorParams")
         .def(py::init<>())
         .def_readwrite("vlr", &aon::Actor::Params::vlr)
         .def_readwrite("alr", &aon::Actor::Params::alr)
-        .def_readwrite("bias", &aon::Actor::Params::bias)
         .def_readwrite("discount", &aon::Actor::Params::discount)
+        .def_readwrite("bias", &aon::Actor::Params::bias)
         .def_readwrite("temperature", &aon::Actor::Params::temperature)
         .def_readwrite("min_steps", &aon::Actor::Params::min_steps)
         .def_readwrite("history_iters", &aon::Actor::Params::history_iters);
 
     py::class_<aon::Hierarchy::Layer_Params>(m, "LayerParams")
         .def(py::init<>())
         .def_readwrite("encoder", &aon::Hierarchy::Layer_Params::encoder)
@@ -159,15 +159,15 @@
         )
         .def_readwrite("size", &pyaon::Image_Visible_Layer_Desc::size)
         .def_readwrite("radius", &pyaon::Image_Visible_Layer_Desc::radius);
 
     // bind params
     py::class_<aon::Image_Encoder::Params>(m, "ImageEncoderParams")
         .def(py::init<>())
-        .def_readwrite("threshold", &aon::Image_Encoder::Params::threshold)
+        .def_readwrite("scale", &aon::Image_Encoder::Params::scale)
         .def_readwrite("falloff", &aon::Image_Encoder::Params::falloff)
         .def_readwrite("lr", &aon::Image_Encoder::Params::lr)
         .def_readwrite("rr", &aon::Image_Encoder::Params::rr);
 
     py::class_<pyaon::Image_Encoder>(m, "ImageEncoder")
         .def(py::init<
                 const std::tuple<int, int, int>&,
```

