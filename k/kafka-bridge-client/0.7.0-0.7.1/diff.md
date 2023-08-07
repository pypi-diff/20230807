# Comparing `tmp/kafka-bridge-client-0.7.0.tar.gz` & `tmp/kafka_bridge_client-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kafka-bridge-client-0.7.0.tar", max compression
+gzip compressed data, was "kafka_bridge_client-0.7.1.tar", max compression
```

## Comparing `kafka-bridge-client-0.7.0.tar` & `kafka_bridge_client-0.7.1.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1066 2022-02-18 13:57:59.995166 kafka-bridge-client-0.7.0/LICENSE
--rw-r--r--   0        0        0     1853 2022-07-12 15:53:04.794922 kafka-bridge-client-0.7.0/README.md
--rw-r--r--   0        0        0      198 2022-02-18 16:26:44.980738 kafka-bridge-client-0.7.0/kafka_bridge_client/__init__.py
--rw-r--r--   0        0        0     9212 2022-07-12 15:53:04.795482 kafka-bridge-client-0.7.0/kafka_bridge_client/consumer.py
--rw-r--r--   0        0        0      512 2022-02-18 16:26:44.981194 kafka-bridge-client-0.7.0/kafka_bridge_client/exceptions.py
--rw-r--r--   0        0        0     3754 2022-07-12 15:51:57.022293 kafka-bridge-client-0.7.0/kafka_bridge_client/producer.py
--rw-r--r--   0        0        0      504 2022-07-12 15:56:09.636318 kafka-bridge-client-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     2682 2022-07-12 15:57:05.923077 kafka-bridge-client-0.7.0/setup.py
--rw-r--r--   0        0        0     2596 2022-07-12 15:57:05.923503 kafka-bridge-client-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-08-07 13:03:26.149353 kafka_bridge_client-0.7.1/LICENSE
+-rw-r--r--   0        0        0     1853 2023-08-07 13:03:26.149418 kafka_bridge_client-0.7.1/README.md
+-rw-r--r--   0        0        0      198 2023-08-07 13:03:26.149503 kafka_bridge_client-0.7.1/kafka_bridge_client/__init__.py
+-rw-r--r--   0        0        0     9212 2023-08-07 13:03:26.149581 kafka_bridge_client-0.7.1/kafka_bridge_client/consumer.py
+-rw-r--r--   0        0        0      512 2023-08-07 13:03:26.149628 kafka_bridge_client-0.7.1/kafka_bridge_client/exceptions.py
+-rw-r--r--   0        0        0     3754 2023-08-07 13:03:26.149693 kafka_bridge_client-0.7.1/kafka_bridge_client/producer.py
+-rw-r--r--   0        0        0      504 2023-08-07 13:15:44.867884 kafka_bridge_client-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     2698 1970-01-01 00:00:00.000000 kafka_bridge_client-0.7.1/PKG-INFO
```

### Comparing `kafka-bridge-client-0.7.0/LICENSE` & `kafka_bridge_client-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kafka-bridge-client-0.7.0/README.md` & `kafka_bridge_client-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `kafka-bridge-client-0.7.0/kafka_bridge_client/consumer.py` & `kafka_bridge_client-0.7.1/kafka_bridge_client/consumer.py`

 * *Files identical despite different names*

### Comparing `kafka-bridge-client-0.7.0/kafka_bridge_client/exceptions.py` & `kafka_bridge_client-0.7.1/kafka_bridge_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `kafka-bridge-client-0.7.0/kafka_bridge_client/producer.py` & `kafka_bridge_client-0.7.1/kafka_bridge_client/producer.py`

 * *Files identical despite different names*

### Comparing `kafka-bridge-client-0.7.0/PKG-INFO` & `kafka_bridge_client-0.7.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: kafka-bridge-client
-Version: 0.7.0
+Version: 0.7.1
 Summary: Python client for Strimzi Kafka Bridge
 Home-page: https://github.com/shafa-dev/kafka-bridge-client
 License: MIT
 Author: Bogdan Zaseka
 Author-email: zaseka.bogdan@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.7.4,<4.0.0)
-Requires-Dist: mypy-extensions (>=0.4.3,<0.5.0)
+Requires-Dist: mypy-extensions (>=1.0.0,<2.0.0)
 Requires-Dist: requests (>=2.27.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 # kafka-bridge-client
 Python async client for [Strimzi Kafka Bridge](https://github.com/strimzi/strimzi-kafka-bridge) and [Confluent REST Proxy](https://docs.confluent.io/platform/current/kafka-rest/index.html) Package include consumer only.
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
```

