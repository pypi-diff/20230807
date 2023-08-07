# Comparing `tmp/brainchain-0.4.1.tar.gz` & `tmp/brainchain-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brainchain-0.4.1.tar", max compression
+gzip compressed data, was "brainchain-0.4.2.tar", max compression
```

## Comparing `brainchain-0.4.1.tar` & `brainchain-0.4.2.tar`

### file list

```diff
@@ -1,10 +1,12 @@
--rw-r--r--   0        0        0     1732 2023-06-20 22:57:22.671703 brainchain-0.4.1/brainchain/README.md
--rw-r--r--   0        0        0      167 2023-07-06 20:56:21.342669 brainchain-0.4.1/brainchain/__init__.py
--rw-r--r--   0        0        0    11485 2023-07-23 13:18:19.901321 brainchain-0.4.1/brainchain/brainchain.py
--rw-r--r--   0        0        0     5579 2023-06-20 22:25:05.537647 brainchain-0.4.1/brainchain/carnivore.py
--rw-r--r--   0        0        0     2243 2023-07-06 00:06:03.958510 brainchain-0.4.1/brainchain/coredata.py
--rw-r--r--   0        0        0      665 2023-07-20 04:24:18.860063 brainchain-0.4.1/brainchain/factcheck.py
--rw-r--r--   0        0        0    15070 2023-07-05 18:42:36.359889 brainchain-0.4.1/brainchain/requirements.txt
--rw-r--r--   0        0        0     6333 2023-07-06 18:26:20.604519 brainchain-0.4.1/brainchain/sales_intel.py
--rw-r--r--   0        0        0      581 2023-07-23 13:18:23.876547 brainchain-0.4.1/pyproject.toml
--rw-r--r--   0        0        0      612 1970-01-01 00:00:00.000000 brainchain-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     6082 2023-07-28 02:29:35.545159 brainchain-0.4.2/brainchain/.aider.chat.history.md
+-rw-r--r--   0        0        0     1874 2023-07-28 02:29:35.545374 brainchain-0.4.2/brainchain/.aider.input.history
+-rw-r--r--   0        0        0     1732 2023-06-20 22:57:22.671703 brainchain-0.4.2/brainchain/README.md
+-rw-r--r--   0        0        0      167 2023-07-06 20:56:21.342669 brainchain-0.4.2/brainchain/__init__.py
+-rw-r--r--   0        0        0    11485 2023-07-28 02:36:23.299632 brainchain-0.4.2/brainchain/brainchain.py
+-rw-r--r--   0        0        0     5579 2023-06-20 22:25:05.537647 brainchain-0.4.2/brainchain/carnivore.py
+-rw-r--r--   0        0        0     2243 2023-07-06 00:06:03.958510 brainchain-0.4.2/brainchain/coredata.py
+-rw-r--r--   0        0        0      665 2023-07-20 04:24:18.860063 brainchain-0.4.2/brainchain/factcheck.py
+-rw-r--r--   0        0        0    15070 2023-07-05 18:42:36.359889 brainchain-0.4.2/brainchain/requirements.txt
+-rw-r--r--   0        0        0     6333 2023-07-06 18:26:20.604519 brainchain-0.4.2/brainchain/sales_intel.py
+-rw-r--r--   0        0        0      532 2023-07-28 02:32:49.415048 brainchain-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0      612 1970-01-01 00:00:00.000000 brainchain-0.4.2/PKG-INFO
```

### Comparing `brainchain-0.4.1/brainchain/README.md` & `brainchain-0.4.2/brainchain/README.md`

 * *Files identical despite different names*

### Comparing `brainchain-0.4.1/brainchain/brainchain.py` & `brainchain-0.4.2/brainchain/brainchain.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.4.1/brainchain/carnivore.py` & `brainchain-0.4.2/brainchain/carnivore.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.4.1/brainchain/coredata.py` & `brainchain-0.4.2/brainchain/coredata.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.4.1/brainchain/factcheck.py` & `brainchain-0.4.2/brainchain/factcheck.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.4.1/brainchain/requirements.txt` & `brainchain-0.4.2/brainchain/requirements.txt`

 * *Files identical despite different names*

### Comparing `brainchain-0.4.1/brainchain/sales_intel.py` & `brainchain-0.4.2/brainchain/sales_intel.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.4.1/pyproject.toml` & `brainchain-0.4.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "brainchain"
-version = "0.4.1"
+version = "0.4.2"
 description = "Brainchain API client"
-authors = ["Arthur M. Collé <arthur@brainchain.ai>", "Audrey Lorberfeld <alorberfeld@brainchain.ai>"]
+authors = ["Arthur M. Collé <arthur@brainchain.ai>"]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 requests = "2.31.0"
 promptlayer = "0.1.92"
 openai = "0.27.8"
 modal-client = "0.50.2627"
```

### Comparing `brainchain-0.4.1/PKG-INFO` & `brainchain-0.4.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainchain
-Version: 0.4.1
+Version: 0.4.2
 Summary: Brainchain API client
 Author: Arthur M. Collé
 Author-email: arthur@brainchain.ai
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

