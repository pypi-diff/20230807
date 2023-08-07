# Comparing `tmp/doy-1.4.tar.gz` & `tmp/doy-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doy-1.4.tar", max compression
+gzip compressed data, was "doy-1.4.1.tar", max compression
```

## Comparing `doy-1.4.tar` & `doy-1.4.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0       30 2022-08-20 20:46:44.060197 doy-1.4/README.md
--rw-r--r--   0        0        0     1121 2022-08-23 10:22:09.091218 doy-1.4/doy/.ipynb_checkpoints/__init__-checkpoint.py
--rw-r--r--   0        0        0     1277 2023-07-13 13:37:12.584726 doy-1.4/doy/.unused.py
--rw-r--r--   0        0        0      176 2023-08-07 14:47:04.045716 doy-1.4/doy/__init__.py
--rw-r--r--   0        0        0      953 2023-06-06 15:22:52.582141 doy-1.4/doy/data.py
--rw-r--r--   0        0        0      510 2023-08-07 14:44:40.232464 doy-1.4/doy/kvstore.py
--rw-r--r--   0        0        0     1542 2023-07-16 14:48:24.576188 doy-1.4/doy/logger.py
--rw-r--r--   0        0        0     4293 2023-06-06 16:07:24.452360 doy-1.4/doy/plotting.py
--rw-r--r--   0        0        0     2300 2023-06-13 16:15:43.417259 doy-1.4/doy/progress.py
--rw-r--r--   0        0        0     2561 2023-06-06 16:24:05.628322 doy-1.4/doy/rich_utils.py
--rw-r--r--   0        0        0     4775 2023-07-16 15:21:29.692855 doy-1.4/doy/utils.py
--rw-r--r--   0        0        0      360 2023-08-07 14:47:16.829827 doy-1.4/pyproject.toml
--rw-r--r--   0        0        0      696 1970-01-01 00:00:00.000000 doy-1.4/setup.py
--rw-r--r--   0        0        0      565 1970-01-01 00:00:00.000000 doy-1.4/PKG-INFO
+-rw-r--r--   0        0        0       30 2022-08-20 20:46:44.060197 doy-1.4.1/README.md
+-rw-r--r--   0        0        0     1121 2022-08-23 10:22:09.091218 doy-1.4.1/doy/.ipynb_checkpoints/__init__-checkpoint.py
+-rw-r--r--   0        0        0     1277 2023-07-13 13:37:12.584726 doy-1.4.1/doy/.unused.py
+-rw-r--r--   0        0        0      176 2023-08-07 14:47:04.045716 doy-1.4.1/doy/__init__.py
+-rw-r--r--   0        0        0      953 2023-06-06 15:22:52.582141 doy-1.4.1/doy/data.py
+-rw-r--r--   0        0        0      510 2023-08-07 14:44:40.232464 doy-1.4.1/doy/kvstore.py
+-rw-r--r--   0        0        0     1542 2023-07-16 14:48:24.576188 doy-1.4.1/doy/logger.py
+-rw-r--r--   0        0        0     4293 2023-06-06 16:07:24.452360 doy-1.4.1/doy/plotting.py
+-rw-r--r--   0        0        0     2300 2023-06-13 16:15:43.417259 doy-1.4.1/doy/progress.py
+-rw-r--r--   0        0        0     2561 2023-06-06 16:24:05.628322 doy-1.4.1/doy/rich_utils.py
+-rw-r--r--   0        0        0     4775 2023-07-16 15:21:29.692855 doy-1.4.1/doy/utils.py
+-rw-r--r--   0        0        0      383 2023-08-07 14:48:15.734340 doy-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0      730 1970-01-01 00:00:00.000000 doy-1.4.1/setup.py
+-rw-r--r--   0        0        0      609 1970-01-01 00:00:00.000000 doy-1.4.1/PKG-INFO
```

### Comparing `doy-1.4/doy/.ipynb_checkpoints/__init__-checkpoint.py` & `doy-1.4.1/doy/.ipynb_checkpoints/__init__-checkpoint.py`

 * *Files identical despite different names*

### Comparing `doy-1.4/doy/.unused.py` & `doy-1.4.1/doy/.unused.py`

 * *Files identical despite different names*

### Comparing `doy-1.4/doy/data.py` & `doy-1.4.1/doy/data.py`

 * *Files identical despite different names*

### Comparing `doy-1.4/doy/logger.py` & `doy-1.4.1/doy/logger.py`

 * *Files identical despite different names*

### Comparing `doy-1.4/doy/plotting.py` & `doy-1.4.1/doy/plotting.py`

 * *Files identical despite different names*

### Comparing `doy-1.4/doy/progress.py` & `doy-1.4.1/doy/progress.py`

 * *Files identical despite different names*

### Comparing `doy-1.4/doy/rich_utils.py` & `doy-1.4.1/doy/rich_utils.py`

 * *Files identical despite different names*

### Comparing `doy-1.4/doy/utils.py` & `doy-1.4.1/doy/utils.py`

 * *Files identical despite different names*

### Comparing `doy-1.4/setup.py` & `doy-1.4.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,19 +4,24 @@
 packages = \
 ['doy', 'doy..ipynb_checkpoints']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['matplotlib>=3.6.2', 'numpy', 'rich>=13.4.1', 'tqdm>=4.65.0', 'wandb>=0.15.5']
+['filelock>=3.12.2,<4.0.0',
+ 'matplotlib>=3.6.2',
+ 'numpy',
+ 'rich>=13.4.1',
+ 'tqdm>=4.65.0',
+ 'wandb>=0.15.5']
 
 setup_kwargs = {
     'name': 'doy',
-    'version': '1.4',
+    'version': '1.4.1',
     'description': '',
     'long_description': '# Doy\n\nSimple utility package\n',
     'author': 'Dominik Schmidt',
     'author_email': 'schmidtdominik30@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `doy-1.4/PKG-INFO` & `doy-1.4.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: doy
-Version: 1.4
+Version: 1.4.1
 Summary: 
 Author: Dominik Schmidt
 Author-email: schmidtdominik30@gmail.com
 Requires-Python: >=3.8
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Requires-Dist: filelock (>=3.12.2,<4.0.0)
 Requires-Dist: matplotlib (>=3.6.2)
 Requires-Dist: numpy
 Requires-Dist: rich (>=13.4.1)
 Requires-Dist: tqdm (>=4.65.0)
 Requires-Dist: wandb (>=0.15.5)
 Description-Content-Type: text/markdown
```

