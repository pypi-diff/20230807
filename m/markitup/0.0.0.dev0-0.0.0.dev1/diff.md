# Comparing `tmp/markitup-0.0.0.dev0.tar.gz` & `tmp/markitup-0.0.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markitup-0.0.0.dev0.tar", last modified: Mon Aug  7 03:17:48 2023, max compression
+gzip compressed data, was "markitup-0.0.0.dev1.tar", last modified: Mon Aug  7 16:24:20 2023, max compression
```

## Comparing `markitup-0.0.0.dev0.tar` & `markitup-0.0.0.dev1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:17:48.037805 markitup-0.0.0.dev0/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-07 03:17:48.037805 markitup-0.0.0.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-08-07 03:17:39.000000 markitup-0.0.0.dev0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 03:17:48.037805 markitup-0.0.0.dev0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:17:48.033805 markitup-0.0.0.dev0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:17:48.037805 markitup-0.0.0.dev0/src/markitup/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-07 03:17:39.000000 markitup-0.0.0.dev0/src/markitup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18783 2023-08-07 03:17:39.000000 markitup-0.0.0.dev0/src/markitup/html.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-08-07 03:17:39.000000 markitup-0.0.0.dev0/src/markitup/md.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:17:48.037805 markitup-0.0.0.dev0/src/markitup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-07 03:17:48.000000 markitup-0.0.0.dev0/src/markitup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-08-07 03:17:48.000000 markitup-0.0.0.dev0/src/markitup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 03:17:48.000000 markitup-0.0.0.dev0/src/markitup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 03:17:47.000000 markitup-0.0.0.dev0/src/markitup.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-07 03:17:48.000000 markitup-0.0.0.dev0/src/markitup.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:24:20.522688 markitup-0.0.0.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-07 16:24:20.522688 markitup-0.0.0.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-08-07 16:24:12.000000 markitup-0.0.0.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 16:24:20.522688 markitup-0.0.0.dev1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:24:20.522688 markitup-0.0.0.dev1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:24:20.522688 markitup-0.0.0.dev1/src/markitup/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-07 16:24:12.000000 markitup-0.0.0.dev1/src/markitup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18844 2023-08-07 16:24:12.000000 markitup-0.0.0.dev1/src/markitup/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-08-07 16:24:12.000000 markitup-0.0.0.dev1/src/markitup/md.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:24:20.522688 markitup-0.0.0.dev1/src/markitup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-07 16:24:20.000000 markitup-0.0.0.dev1/src/markitup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-08-07 16:24:20.000000 markitup-0.0.0.dev1/src/markitup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 16:24:20.000000 markitup-0.0.0.dev1/src/markitup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 16:24:20.000000 markitup-0.0.0.dev1/src/markitup.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-07 16:24:20.000000 markitup-0.0.0.dev1/src/markitup.egg-info/top_level.txt
```

### Comparing `markitup-0.0.0.dev0/pyproject.toml` & `markitup-0.0.0.dev1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -13,10 +13,10 @@
 where = ["src"]
 namespaces = true
 
 
 # ----------------------------------------- Project Metadata -------------------------------------
 #
 [project]
-version = "0.0.0.dev0"
+version = "0.0.0.dev1"
 name = "markitup"
 requires-python = ">=3.9"
```

### Comparing `markitup-0.0.0.dev0/src/markitup/html.py` & `markitup-0.0.0.dev1/src/markitup/html.py`

 * *Files 1% similar despite different names*

```diff
@@ -658,15 +658,15 @@
         tag_seperator: Optional[str] = "\n",
         content_indent: Optional[str] = "\t",
         **attrs,
     ):
         attrs["open"] = open
         if summary is not None:
             if not isinstance(summary, SUMMARY):
-                summary = SUMMARY(content=summary)
+                summary = SUMMARY(content=summary, content_indent=content_indent, tag_seperator=tag_seperator),
             content = [summary, BR(), content]
         super().__init__(
             tag=f"details",
             attrs=attrs,
             content=content,
             tag_seperator=tag_seperator,
             content_indent=content_indent,
```

