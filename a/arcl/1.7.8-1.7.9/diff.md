# Comparing `tmp/arcl-1.7.8.tar.gz` & `tmp/arcl-1.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcl-1.7.8.tar", max compression
+gzip compressed data, was "arcl-1.7.9.tar", max compression
```

## Comparing `arcl-1.7.8.tar` & `arcl-1.7.9.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0       83 2022-11-10 16:29:23.919826 arcl-1.7.8/arcl/__init__.py
--rw-r--r--   0        0        0       48 2022-11-10 16:29:23.919826 arcl-1.7.8/arcl/__main__.py
--rw-r--r--   0        0        0     7370 2022-11-10 16:29:23.919826 arcl-1.7.8/arcl/auth.py
--rw-r--r--   0        0        0     5445 2022-11-10 16:29:23.919826 arcl-1.7.8/arcl/cli.py
--rw-r--r--   0        0        0     2060 2022-11-10 16:29:23.919826 arcl-1.7.8/arcl/config.py
--rw-r--r--   0        0        0      686 2022-11-10 16:29:23.919826 arcl-1.7.8/arcl/token_cache.py
--rw-r--r--   0        0        0      608 2022-11-10 16:29:23.923826 arcl-1.7.8/pyproject.toml
--rw-r--r--   0        0        0      808 1970-01-01 00:00:00.000000 arcl-1.7.8/setup.py
--rw-r--r--   0        0        0      642 1970-01-01 00:00:00.000000 arcl-1.7.8/PKG-INFO
+-rw-r--r--   0        0        0     3394 2022-11-22 11:03:26.866327 arcl-1.7.9/README.md
+-rw-r--r--   0        0        0       83 2022-11-22 11:03:26.866327 arcl-1.7.9/arcl/__init__.py
+-rw-r--r--   0        0        0       48 2022-11-22 11:03:26.866327 arcl-1.7.9/arcl/__main__.py
+-rw-r--r--   0        0        0     7370 2022-11-22 11:03:26.866327 arcl-1.7.9/arcl/auth.py
+-rw-r--r--   0        0        0     5445 2022-11-22 11:03:26.870327 arcl-1.7.9/arcl/cli.py
+-rw-r--r--   0        0        0     2060 2022-11-22 11:03:26.870327 arcl-1.7.9/arcl/config.py
+-rw-r--r--   0        0        0      686 2022-11-22 11:03:26.870327 arcl-1.7.9/arcl/token_cache.py
+-rw-r--r--   0        0        0      628 2022-11-22 11:03:26.870327 arcl-1.7.9/pyproject.toml
+-rw-r--r--   0        0        0     4280 1970-01-01 00:00:00.000000 arcl-1.7.9/setup.py
+-rw-r--r--   0        0        0     4078 1970-01-01 00:00:00.000000 arcl-1.7.9/PKG-INFO
```

### Comparing `arcl-1.7.8/arcl/auth.py` & `arcl-1.7.9/arcl/auth.py`

 * *Files identical despite different names*

### Comparing `arcl-1.7.8/arcl/cli.py` & `arcl-1.7.9/arcl/cli.py`

 * *Files identical despite different names*

### Comparing `arcl-1.7.8/arcl/config.py` & `arcl-1.7.9/arcl/config.py`

 * *Files identical despite different names*

### Comparing `arcl-1.7.8/arcl/token_cache.py` & `arcl-1.7.9/arcl/token_cache.py`

 * *Files identical despite different names*

