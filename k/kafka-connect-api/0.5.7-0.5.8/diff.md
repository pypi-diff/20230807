# Comparing `tmp/kafka_connect_api-0.5.7.tar.gz` & `tmp/kafka_connect_api-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kafka_connect_api-0.5.7.tar", max compression
+gzip compressed data, was "kafka_connect_api-0.5.8.tar", max compression
```

## Comparing `kafka_connect_api-0.5.7.tar` & `kafka_connect_api-0.5.8.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    16725 2022-06-01 07:03:28.022199 kafka_connect_api-0.5.7/LICENSE
--rw-r--r--   0        0        0     2718 2023-01-15 22:36:04.845700 kafka_connect_api-0.5.7/README.rst
--rw-r--r--   0        0        0      141 2023-06-28 09:11:25.053211 kafka_connect_api-0.5.7/kafka_connect_api/__init__.py
--rw-r--r--   0        0        0     7433 2023-06-28 09:10:53.197835 kafka_connect_api-0.5.7/kafka_connect_api/aws_lambdas.py
--rw-r--r--   0        0        0     3176 2023-03-21 05:47:47.410436 kafka_connect_api-0.5.7/kafka_connect_api/errors.py
--rw-r--r--   0        0        0    12094 2023-03-15 14:09:15.772930 kafka_connect_api-0.5.7/kafka_connect_api/kafka_connect_api.py
--rw-r--r--   0        0        0      162 2023-01-16 10:00:46.616584 kafka_connect_api-0.5.7/kafka_connect_api/tools.py
--rw-r--r--   0        0        0     2043 2023-06-28 09:11:25.053211 kafka_connect_api-0.5.7/pyproject.toml
--rw-r--r--   0        0        0     3643 1970-01-01 00:00:00.000000 kafka_connect_api-0.5.7/PKG-INFO
+-rw-r--r--   0        0        0    16725 2022-06-01 07:03:28.022199 kafka_connect_api-0.5.8/LICENSE
+-rw-r--r--   0        0        0     2718 2023-01-15 22:36:04.845700 kafka_connect_api-0.5.8/README.rst
+-rw-r--r--   0        0        0      141 2023-08-07 20:06:08.104030 kafka_connect_api-0.5.8/kafka_connect_api/__init__.py
+-rw-r--r--   0        0        0     7433 2023-06-28 09:10:53.197835 kafka_connect_api-0.5.8/kafka_connect_api/aws_lambdas.py
+-rw-r--r--   0        0        0     3176 2023-03-21 05:47:47.410436 kafka_connect_api-0.5.8/kafka_connect_api/errors.py
+-rw-r--r--   0        0        0    12094 2023-03-15 14:09:15.772930 kafka_connect_api-0.5.8/kafka_connect_api/kafka_connect_api.py
+-rw-r--r--   0        0        0      162 2023-01-16 10:00:46.616584 kafka_connect_api-0.5.8/kafka_connect_api/tools.py
+-rw-r--r--   0        0        0     2043 2023-08-07 20:06:08.104030 kafka_connect_api-0.5.8/pyproject.toml
+-rw-r--r--   0        0        0     3643 1970-01-01 00:00:00.000000 kafka_connect_api-0.5.8/PKG-INFO
```

### Comparing `kafka_connect_api-0.5.7/LICENSE` & `kafka_connect_api-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `kafka_connect_api-0.5.7/README.rst` & `kafka_connect_api-0.5.8/README.rst`

 * *Files identical despite different names*

### Comparing `kafka_connect_api-0.5.7/kafka_connect_api/aws_lambdas.py` & `kafka_connect_api-0.5.8/kafka_connect_api/aws_lambdas.py`

 * *Files identical despite different names*

### Comparing `kafka_connect_api-0.5.7/kafka_connect_api/errors.py` & `kafka_connect_api-0.5.8/kafka_connect_api/errors.py`

 * *Files identical despite different names*

### Comparing `kafka_connect_api-0.5.7/kafka_connect_api/kafka_connect_api.py` & `kafka_connect_api-0.5.8/kafka_connect_api/kafka_connect_api.py`

 * *Files identical despite different names*

### Comparing `kafka_connect_api-0.5.7/pyproject.toml` & `kafka_connect_api-0.5.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "kafka_connect_api"
-version = "0.5.7"
+version = "0.5.8"
 description = "Apache Kafka Connect client"
 authors = ["John Preston <john@compose-x.io>"]
 license = "MPL-2.0"
 readme = "README.rst"
 classifiers = [
     "Natural Language :: English",
     "Programming Language :: Python :: 3",
@@ -48,15 +48,15 @@
 [tool.poetry.group.dev.dependencies]
 sphinx-autodoc-typehints = "^1.19.4"
 
 [tool.tbump]
 github_url = "https://github.com/compose-x/kafka_connect_api"
 
 [tool.tbump.version]
-current = "0.5.7"
+current = "0.5.8"
 
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
```

### Comparing `kafka_connect_api-0.5.7/PKG-INFO` & `kafka_connect_api-0.5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kafka-connect-api
-Version: 0.5.7
+Version: 0.5.8
 Summary: Apache Kafka Connect client
 License: MPL-2.0
 Author: John Preston
 Author-email: john@compose-x.io
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Information Technology
```

