# Comparing `tmp/examon_beginners_package-0.1.14.tar.gz` & `tmp/examon_beginners_package-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "examon_beginners_package-0.1.14.tar", max compression
+gzip compressed data, was "examon_beginners_package-0.2.0.tar", max compression
```

## Comparing `examon_beginners_package-0.1.14.tar` & `examon_beginners_package-0.2.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0       24 2023-07-16 20:33:56.622876 examon_beginners_package-0.1.14/examon_beginners_package/__init__.py
--rw-r--r--   0        0        0     1573 2023-07-18 20:43:28.888259 examon_beginners_package-0.1.14/examon_beginners_package/beginners.py
--rw-r--r--   0        0        0      345 2023-08-06 14:52:43.317380 examon_beginners_package-0.1.14/pyproject.toml
--rw-r--r--   0        0        0      350 1970-01-01 00:00:00.000000 examon_beginners_package-0.1.14/PKG-INFO
+-rw-r--r--   0        0        0       24 2023-07-16 20:33:56.622876 examon_beginners_package-0.2.0/examon_beginners_package/__init__.py
+-rw-r--r--   0        0        0     3532 2023-08-07 15:24:04.481477 examon_beginners_package-0.2.0/examon_beginners_package/beginners.py
+-rw-r--r--   0        0        0      344 2023-08-07 15:25:41.461129 examon_beginners_package-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      349 1970-01-01 00:00:00.000000 examon_beginners_package-0.2.0/PKG-INFO
```

