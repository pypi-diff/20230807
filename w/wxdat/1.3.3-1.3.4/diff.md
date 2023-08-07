# Comparing `tmp/wxdat-1.3.3.tar.gz` & `tmp/wxdat-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wxdat-1.3.3.tar", max compression
+gzip compressed data, was "wxdat-1.3.4.tar", max compression
```

## Comparing `wxdat-1.3.3.tar` & `wxdat-1.3.4.tar`

### file list

```diff
@@ -1,26 +1,25 @@
--rw-r--r--   0        0        0     1071 2023-01-10 14:02:30.444482 wxdat-1.3.3/LICENSE
--rw-r--r--   0        0        0     2199 2023-01-24 14:38:03.133133 wxdat-1.3.3/README.md
--rw-r--r--   0        0        0      664 2023-07-09 04:51:15.185327 wxdat-1.3.3/pyproject.toml
--rw-r--r--   0        0        0       33 2023-01-07 17:38:11.743809 wxdat-1.3.3/src/wxdat/__init__.py
--rw-r--r--   0        0        0     2260 2023-03-19 14:53:46.007655 wxdat-1.3.3/src/wxdat/__main__.py
--rw-r--r--   0        0        0     5932 2023-06-29 18:55:36.438028 wxdat-1.3.3/src/wxdat/config.py
--rw-r--r--   0        0        0     3711 2023-06-29 18:58:07.039970 wxdat-1.3.3/src/wxdat/database.py
--rw-r--r--   0        0        0     6284 2023-07-09 04:46:47.995444 wxdat-1.3.3/src/wxdat/metrics.py
--rw-r--r--   0        0        0     6892 2023-06-29 18:54:36.448538 wxdat-1.3.3/src/wxdat/providers/__init__.py
--rw-r--r--   0        0        0     4457 2023-01-19 01:01:56.989878 wxdat-1.3.3/src/wxdat/providers/accuweather.py
--rw-r--r--   0        0        0     4075 2023-06-21 03:18:47.374242 wxdat-1.3.3/src/wxdat/providers/ambientwx.py
--rw-r--r--   0        0        0     4104 2023-01-19 01:01:56.991629 wxdat-1.3.3/src/wxdat/providers/noaa.py
--rw-r--r--   0        0        0     6862 2023-01-19 01:01:56.991956 wxdat-1.3.3/src/wxdat/providers/openweather.py
--rw-r--r--   0        0        0     3736 2023-01-19 01:01:56.992601 wxdat-1.3.3/src/wxdat/providers/wunderground.py
--rw-r--r--   0        0        0     3097 2023-01-21 19:50:22.876646 wxdat-1.3.3/src/wxdat/units/__init__.py
--rw-r--r--   0        0        0     3392 2023-01-13 00:50:28.105958 wxdat-1.3.3/src/wxdat/units/distance.py
--rw-r--r--   0        0        0     1931 2023-01-13 00:50:28.106131 wxdat-1.3.3/src/wxdat/units/pressure.py
--rw-r--r--   0        0        0     2798 2023-01-13 00:50:28.106343 wxdat-1.3.3/src/wxdat/units/quantity.py
--rw-r--r--   0        0        0     1209 2023-01-21 19:50:22.876902 wxdat-1.3.3/src/wxdat/units/rate.py
--rw-r--r--   0        0        0     1484 2023-01-13 00:50:28.106471 wxdat-1.3.3/src/wxdat/units/temperature.py
--rw-r--r--   0        0        0     2652 2023-01-13 00:50:28.106680 wxdat-1.3.3/src/wxdat/units/velocity.py
--rw-r--r--   0        0        0      936 2023-01-13 00:50:28.106805 wxdat-1.3.3/src/wxdat/units/volume.py
--rw-r--r--   0        0        0      881 2023-01-13 00:50:28.107000 wxdat-1.3.3/src/wxdat/units/weight.py
--rw-r--r--   0        0        0     1650 2023-03-19 14:53:46.010256 wxdat-1.3.3/src/wxdat/version.py
--rw-r--r--   0        0        0     3314 1970-01-01 00:00:00.000000 wxdat-1.3.3/setup.py
--rw-r--r--   0        0        0     2997 1970-01-01 00:00:00.000000 wxdat-1.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-01-10 14:02:30.444482 wxdat-1.3.4/LICENSE
+-rw-r--r--   0        0        0     2199 2023-01-24 14:38:03.133133 wxdat-1.3.4/README.md
+-rw-r--r--   0        0        0      666 2023-08-07 14:20:06.454452 wxdat-1.3.4/pyproject.toml
+-rw-r--r--   0        0        0       33 2023-01-07 17:38:11.743809 wxdat-1.3.4/src/wxdat/__init__.py
+-rw-r--r--   0        0        0     2260 2023-03-19 14:53:46.007655 wxdat-1.3.4/src/wxdat/__main__.py
+-rw-r--r--   0        0        0     5932 2023-06-29 18:55:36.438028 wxdat-1.3.4/src/wxdat/config.py
+-rw-r--r--   0        0        0     3711 2023-06-29 18:58:07.039970 wxdat-1.3.4/src/wxdat/database.py
+-rw-r--r--   0        0        0     6284 2023-07-09 04:46:47.995444 wxdat-1.3.4/src/wxdat/metrics.py
+-rw-r--r--   0        0        0     6892 2023-07-18 14:44:38.989813 wxdat-1.3.4/src/wxdat/providers/__init__.py
+-rw-r--r--   0        0        0     4457 2023-01-19 01:01:56.989878 wxdat-1.3.4/src/wxdat/providers/accuweather.py
+-rw-r--r--   0        0        0     4075 2023-06-21 03:18:47.374242 wxdat-1.3.4/src/wxdat/providers/ambientwx.py
+-rw-r--r--   0        0        0     4104 2023-01-19 01:01:56.991629 wxdat-1.3.4/src/wxdat/providers/noaa.py
+-rw-r--r--   0        0        0     6862 2023-07-26 02:33:28.406390 wxdat-1.3.4/src/wxdat/providers/openweather.py
+-rw-r--r--   0        0        0     3736 2023-01-19 01:01:56.992601 wxdat-1.3.4/src/wxdat/providers/wunderground.py
+-rw-r--r--   0        0        0     3097 2023-01-21 19:50:22.876646 wxdat-1.3.4/src/wxdat/units/__init__.py
+-rw-r--r--   0        0        0     3392 2023-01-13 00:50:28.105958 wxdat-1.3.4/src/wxdat/units/distance.py
+-rw-r--r--   0        0        0     1931 2023-01-13 00:50:28.106131 wxdat-1.3.4/src/wxdat/units/pressure.py
+-rw-r--r--   0        0        0     2798 2023-01-13 00:50:28.106343 wxdat-1.3.4/src/wxdat/units/quantity.py
+-rw-r--r--   0        0        0     1209 2023-01-21 19:50:22.876902 wxdat-1.3.4/src/wxdat/units/rate.py
+-rw-r--r--   0        0        0     1484 2023-01-13 00:50:28.106471 wxdat-1.3.4/src/wxdat/units/temperature.py
+-rw-r--r--   0        0        0     2652 2023-01-13 00:50:28.106680 wxdat-1.3.4/src/wxdat/units/velocity.py
+-rw-r--r--   0        0        0      936 2023-01-13 00:50:28.106805 wxdat-1.3.4/src/wxdat/units/volume.py
+-rw-r--r--   0        0        0      881 2023-01-13 00:50:28.107000 wxdat-1.3.4/src/wxdat/units/weight.py
+-rw-r--r--   0        0        0     1650 2023-03-19 14:53:46.010256 wxdat-1.3.4/src/wxdat/version.py
+-rw-r--r--   0        0        0     3001 1970-01-01 00:00:00.000000 wxdat-1.3.4/PKG-INFO
```

### Comparing `wxdat-1.3.3/LICENSE` & `wxdat-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `wxdat-1.3.3/README.md` & `wxdat-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `wxdat-1.3.3/pyproject.toml` & `wxdat-1.3.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 name = "wxdat"
-version = "1.3.3"
+version = "1.3.4"
 description = "Weather data explorer."
 authors = ["jheddings <jheddings@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 requests = "^2.31.0"
-click = "^8.1.4"
-prometheus-client = "^0.17.0"
-pydantic = "^1.10.11"
-sqlalchemy = "^2.0.18"
-psycopg2 = "^2.9.6"
+click = "^8.1.6"
+prometheus-client = "^0.17.1"
+pydantic = "^1.10.12"
+sqlalchemy = "^2.0.19"
+psycopg2 = "^2.9.7"
 ratelimit = "^2.2.1"
-pyyaml = "^6.0"
-gitpython = "^3.1.31"
+pyyaml = "^6.0.1"
+gitpython = "^3.1.32"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.3.3"
 pytest = "^7.4.0"
 pytest-vcr = "^1.0.2"
 coverage = "^7.2.7"
```

### Comparing `wxdat-1.3.3/src/wxdat/__main__.py` & `wxdat-1.3.4/src/wxdat/__main__.py`

 * *Files identical despite different names*

### Comparing `wxdat-1.3.3/src/wxdat/config.py` & `wxdat-1.3.4/src/wxdat/config.py`

 * *Files identical despite different names*

### Comparing `wxdat-1.3.3/src/wxdat/database.py` & `wxdat-1.3.4/src/wxdat/database.py`

 * *Files identical despite different names*

### Comparing `wxdat-1.3.3/src/wxdat/metrics.py` & `wxdat-1.3.4/src/wxdat/metrics.py`

 * *Files identical despite different names*

### Comparing `wxdat-1.3.3/src/wxdat/providers/__init__.py` & `wxdat-1.3.4/src/wxdat/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `wxdat-1.3.3/src/wxdat/providers/accuweather.py` & `wxdat-1.3.4/src/wxdat/providers/accuweather.py`

 * *Files identical despite different names*

### Comparing `wxdat-1.3.3/src/wxdat/providers/ambientwx.py` & `wxdat-1.3.4/src/wxdat/providers/ambientwx.py`

 * *Files identical despite different names*

### Comparing `wxdat-1.3.3/src/wxdat/providers/noaa.py` & `wxdat-1.3.4/src/wxdat/providers/noaa.py`

 * *Files identical despite different names*

### Comparing `wxdat-1.3.3/src/wxdat/providers/openweather.py` & `wxdat-1.3.4/src/wxdat/providers/openweather.py`

 * *Files identical despite different names*

### Comparing `wxdat-1.3.3/src/wxdat/providers/wunderground.py` & `wxdat-1.3.4/src/wxdat/providers/wunderground.py`

 * *Files identical despite different names*

### Comparing `wxdat-1.3.3/src/wxdat/units/__init__.py` & `wxdat-1.3.4/src/wxdat/units/__init__.py`

 * *Files identical despite different names*

### Comparing `wxdat-1.3.3/src/wxdat/units/distance.py` & `wxdat-1.3.4/src/wxdat/units/distance.py`

 * *Files identical despite different names*

### Comparing `wxdat-1.3.3/src/wxdat/units/pressure.py` & `wxdat-1.3.4/src/wxdat/units/pressure.py`

 * *Files identical despite different names*

### Comparing `wxdat-1.3.3/src/wxdat/units/quantity.py` & `wxdat-1.3.4/src/wxdat/units/quantity.py`

 * *Files identical despite different names*

### Comparing `wxdat-1.3.3/src/wxdat/units/rate.py` & `wxdat-1.3.4/src/wxdat/units/rate.py`

 * *Files identical despite different names*

### Comparing `wxdat-1.3.3/src/wxdat/units/temperature.py` & `wxdat-1.3.4/src/wxdat/units/temperature.py`

 * *Files identical despite different names*

### Comparing `wxdat-1.3.3/src/wxdat/units/velocity.py` & `wxdat-1.3.4/src/wxdat/units/velocity.py`

 * *Files identical despite different names*

### Comparing `wxdat-1.3.3/src/wxdat/units/volume.py` & `wxdat-1.3.4/src/wxdat/units/volume.py`

 * *Files identical despite different names*

### Comparing `wxdat-1.3.3/src/wxdat/units/weight.py` & `wxdat-1.3.4/src/wxdat/units/weight.py`

 * *Files identical despite different names*

### Comparing `wxdat-1.3.3/src/wxdat/version.py` & `wxdat-1.3.4/src/wxdat/version.py`

 * *Files identical despite different names*

### Comparing `wxdat-1.3.3/PKG-INFO` & `wxdat-1.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: wxdat
-Version: 1.3.3
+Version: 1.3.4
 Summary: Weather data explorer.
 License: MIT
 Author: jheddings
 Author-email: jheddings@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: click (>=8.1.4,<9.0.0)
-Requires-Dist: gitpython (>=3.1.31,<4.0.0)
-Requires-Dist: prometheus-client (>=0.17.0,<0.18.0)
-Requires-Dist: psycopg2 (>=2.9.6,<3.0.0)
-Requires-Dist: pydantic (>=1.10.11,<2.0.0)
-Requires-Dist: pyyaml (>=6.0,<7.0)
+Requires-Dist: click (>=8.1.6,<9.0.0)
+Requires-Dist: gitpython (>=3.1.32,<4.0.0)
+Requires-Dist: prometheus-client (>=0.17.1,<0.18.0)
+Requires-Dist: psycopg2 (>=2.9.7,<3.0.0)
+Requires-Dist: pydantic (>=1.10.12,<2.0.0)
+Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: ratelimit (>=2.2.1,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
-Requires-Dist: sqlalchemy (>=2.0.18,<3.0.0)
+Requires-Dist: sqlalchemy (>=2.0.19,<3.0.0)
 Description-Content-Type: text/markdown
 
 # wxdat #
 
 [![PyPI](https://img.shields.io/pypi/v/wxdat.svg)](https://pypi.org/project/wxdat)
 [![LICENSE](https://img.shields.io/github/license/jheddings/wxdat)](LICENSE)
 [![Style](https://img.shields.io/badge/style-black-black)](https://github.com/ambv/black)
```

