# Comparing `tmp/cog2-0.1.8.tar.gz` & `tmp/cog2-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cog2-0.1.8.tar", max compression
+gzip compressed data, was "cog2-0.1.9.tar", max compression
```

## Comparing `cog2-0.1.8.tar` & `cog2-0.1.9.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0      471 2023-07-25 06:52:04.663746 cog2-0.1.8/README.md
--rw-r--r--   0        0        0        0 2023-07-24 00:37:04.090024 cog2-0.1.8/cog2/__init__.py
--rw-r--r--   0        0        0     3693 2023-07-29 03:01:38.550106 cog2-0.1.8/cog2/main.py
--rw-r--r--   0        0        0      426 2023-07-29 03:01:38.543229 cog2-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      990 1970-01-01 00:00:00.000000 cog2-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      471 2023-07-25 06:52:04.663746 cog2-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2023-07-24 00:37:04.090024 cog2-0.1.9/cog2/__init__.py
+-rw-r--r--   0        0        0      708 2023-08-07 03:55:21.963513 cog2-0.1.9/cog2/base.yaml
+-rw-r--r--   0        0        0     5986 2023-08-07 04:39:02.168639 cog2-0.1.9/cog2/main.py
+-rw-r--r--   0        0        0      428 2023-08-07 04:37:47.256142 cog2-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      990 1970-01-01 00:00:00.000000 cog2-0.1.9/PKG-INFO
```

### Comparing `cog2-0.1.8/PKG-INFO` & `cog2-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cog2
-Version: 0.1.8
+Version: 0.1.9
 Summary: wizmodel.com wiz sdk
 Author: incoming
 Author-email: 18320122+incomingflyingbrick@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

