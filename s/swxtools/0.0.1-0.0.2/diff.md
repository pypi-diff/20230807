# Comparing `tmp/swxtools-0.0.1.tar.gz` & `tmp/swxtools-0.0.2.tar.gz`

## Comparing `swxtools-0.0.1.tar` & `swxtools-0.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 swxtools-0.0.1/dot_swxtools.cfg.example
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swxtools-0.0.1/src/swxtools/__init__.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 swxtools-0.0.1/src/swxtools/config.py
--rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 swxtools-0.0.1/src/swxtools/dataframe_tools.py
--rw-r--r--   0        0        0     9212 2020-02-02 00:00:00.000000 swxtools-0.0.1/src/swxtools/download_tools.py
--rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 swxtools-0.0.1/src/swxtools/hapi_client.py
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 swxtools-0.0.1/src/swxtools/hapi_knmi_tools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swxtools-0.0.1/src/swxtools/access/__init__.py
--rw-r--r--   0        0        0     3300 2020-02-02 00:00:00.000000 swxtools-0.0.1/src/swxtools/access/ace.py
--rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 swxtools-0.0.1/src/swxtools/access/dscovr.py
--rw-r--r--   0        0        0     4003 2020-02-02 00:00:00.000000 swxtools-0.0.1/src/swxtools/access/gfz_kp_hp_indices.py
--rw-r--r--   0        0        0     5179 2020-02-02 00:00:00.000000 swxtools-0.0.1/src/swxtools/access/penticton_f10.py
--rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 swxtools-0.0.1/src/swxtools/access/silso_sunspot_number.py
--rw-r--r--   0        0        0    16095 2020-02-02 00:00:00.000000 swxtools-0.0.1/src/swxtools/access/swarm_diss.py
--rw-r--r--   0        0        0     5625 2020-02-02 00:00:00.000000 swxtools-0.0.1/src/swxtools/access/swpc_rt.py
--rw-r--r--   0        0        0    14410 2020-02-02 00:00:00.000000 swxtools-0.0.1/src/swxtools/access/wam_ipe.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swxtools-0.0.1/src/swxtools/orbit/__init__.py
--rw-r--r--   0        0        0     8718 2020-02-02 00:00:00.000000 swxtools-0.0.1/src/swxtools/orbit/kepler.py
--rw-r--r--   0        0        0     3350 2020-02-02 00:00:00.000000 swxtools-0.0.1/src/swxtools/orbit/msis.py
--rw-r--r--   0        0        0     8569 2020-02-02 00:00:00.000000 swxtools-0.0.1/src/swxtools/orbit/tle.py
--rw-r--r--   0        0        0    10403 2020-02-02 00:00:00.000000 swxtools-0.0.1/src/swxtools/orbit/transforms.py
--rw-r--r--   0        0        0    11344 2020-02-02 00:00:00.000000 swxtools-0.0.1/LICENSE
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 swxtools-0.0.1/README.md
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 swxtools-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 swxtools-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 swxtools-0.0.2/dot_swxtools.cfg.example
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swxtools-0.0.2/src/swxtools/__init__.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 swxtools-0.0.2/src/swxtools/config.py
+-rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 swxtools-0.0.2/src/swxtools/dataframe_tools.py
+-rw-r--r--   0        0        0     9212 2020-02-02 00:00:00.000000 swxtools-0.0.2/src/swxtools/download_tools.py
+-rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 swxtools-0.0.2/src/swxtools/hapi_client.py
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 swxtools-0.0.2/src/swxtools/hapi_knmi_tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swxtools-0.0.2/src/swxtools/access/__init__.py
+-rw-r--r--   0        0        0     3300 2020-02-02 00:00:00.000000 swxtools-0.0.2/src/swxtools/access/ace.py
+-rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 swxtools-0.0.2/src/swxtools/access/dscovr.py
+-rw-r--r--   0        0        0     4003 2020-02-02 00:00:00.000000 swxtools-0.0.2/src/swxtools/access/gfz_kp_hp_indices.py
+-rw-r--r--   0        0        0     5179 2020-02-02 00:00:00.000000 swxtools-0.0.2/src/swxtools/access/penticton_f10.py
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 swxtools-0.0.2/src/swxtools/access/silso_sunspot_number.py
+-rw-r--r--   0        0        0    16095 2020-02-02 00:00:00.000000 swxtools-0.0.2/src/swxtools/access/swarm_diss.py
+-rw-r--r--   0        0        0     5625 2020-02-02 00:00:00.000000 swxtools-0.0.2/src/swxtools/access/swpc_rt.py
+-rw-r--r--   0        0        0    14410 2020-02-02 00:00:00.000000 swxtools-0.0.2/src/swxtools/access/wam_ipe.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swxtools-0.0.2/src/swxtools/orbit/__init__.py
+-rw-r--r--   0        0        0     8718 2020-02-02 00:00:00.000000 swxtools-0.0.2/src/swxtools/orbit/kepler.py
+-rw-r--r--   0        0        0     3350 2020-02-02 00:00:00.000000 swxtools-0.0.2/src/swxtools/orbit/msis.py
+-rw-r--r--   0        0        0     8569 2020-02-02 00:00:00.000000 swxtools-0.0.2/src/swxtools/orbit/tle.py
+-rw-r--r--   0        0        0    10403 2020-02-02 00:00:00.000000 swxtools-0.0.2/src/swxtools/orbit/transforms.py
+-rw-r--r--   0        0        0    11344 2020-02-02 00:00:00.000000 swxtools-0.0.2/LICENSE
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 swxtools-0.0.2/README.md
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 swxtools-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 swxtools-0.0.2/PKG-INFO
```

### Comparing `swxtools-0.0.1/src/swxtools/dataframe_tools.py` & `swxtools-0.0.2/src/swxtools/dataframe_tools.py`

 * *Files identical despite different names*

### Comparing `swxtools-0.0.1/src/swxtools/download_tools.py` & `swxtools-0.0.2/src/swxtools/download_tools.py`

 * *Files identical despite different names*

### Comparing `swxtools-0.0.1/src/swxtools/hapi_client.py` & `swxtools-0.0.2/src/swxtools/hapi_client.py`

 * *Files identical despite different names*

### Comparing `swxtools-0.0.1/src/swxtools/hapi_knmi_tools.py` & `swxtools-0.0.2/src/swxtools/hapi_knmi_tools.py`

 * *Files identical despite different names*

### Comparing `swxtools-0.0.1/src/swxtools/access/ace.py` & `swxtools-0.0.2/src/swxtools/access/ace.py`

 * *Files identical despite different names*

### Comparing `swxtools-0.0.1/src/swxtools/access/dscovr.py` & `swxtools-0.0.2/src/swxtools/access/dscovr.py`

 * *Files identical despite different names*

### Comparing `swxtools-0.0.1/src/swxtools/access/gfz_kp_hp_indices.py` & `swxtools-0.0.2/src/swxtools/access/gfz_kp_hp_indices.py`

 * *Files identical despite different names*

### Comparing `swxtools-0.0.1/src/swxtools/access/penticton_f10.py` & `swxtools-0.0.2/src/swxtools/access/penticton_f10.py`

 * *Files identical despite different names*

### Comparing `swxtools-0.0.1/src/swxtools/access/silso_sunspot_number.py` & `swxtools-0.0.2/src/swxtools/access/silso_sunspot_number.py`

 * *Files identical despite different names*

### Comparing `swxtools-0.0.1/src/swxtools/access/swarm_diss.py` & `swxtools-0.0.2/src/swxtools/access/swarm_diss.py`

 * *Files identical despite different names*

### Comparing `swxtools-0.0.1/src/swxtools/access/swpc_rt.py` & `swxtools-0.0.2/src/swxtools/access/swpc_rt.py`

 * *Files identical despite different names*

### Comparing `swxtools-0.0.1/src/swxtools/access/wam_ipe.py` & `swxtools-0.0.2/src/swxtools/access/wam_ipe.py`

 * *Files identical despite different names*

### Comparing `swxtools-0.0.1/src/swxtools/orbit/kepler.py` & `swxtools-0.0.2/src/swxtools/orbit/kepler.py`

 * *Files identical despite different names*

### Comparing `swxtools-0.0.1/src/swxtools/orbit/msis.py` & `swxtools-0.0.2/src/swxtools/orbit/msis.py`

 * *Files identical despite different names*

### Comparing `swxtools-0.0.1/src/swxtools/orbit/tle.py` & `swxtools-0.0.2/src/swxtools/orbit/tle.py`

 * *Files identical despite different names*

### Comparing `swxtools-0.0.1/src/swxtools/orbit/transforms.py` & `swxtools-0.0.2/src/swxtools/orbit/transforms.py`

 * *Files identical despite different names*

### Comparing `swxtools-0.0.1/LICENSE` & `swxtools-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `swxtools-0.0.1/pyproject.toml` & `swxtools-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "swxtools"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Eelco Doornbos", email="eelco.doornbos@knmi.nl" },
 ]
 description = "Collection of tools to work with space weather data, developed at KNMI."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `swxtools-0.0.1/PKG-INFO` & `swxtools-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swxtools
-Version: 0.0.1
+Version: 0.0.2
 Summary: Collection of tools to work with space weather data, developed at KNMI.
 Project-URL: Homepage, https://gitlab.com/KNMI-OSS/spaceweather/swxtools/
 Project-URL: Bug Tracker, https://gitlab.com/KNMI-OSS/spaceweather/-/issues
 Author-email: Eelco Doornbos <eelco.doornbos@knmi.nl>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

