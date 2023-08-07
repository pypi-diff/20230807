# Comparing `tmp/hypymedia-0.1.7.tar.gz` & `tmp/hypymedia-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypymedia-0.1.7.tar", max compression
+gzip compressed data, was "hypymedia-0.1.8.tar", max compression
```

## Comparing `hypymedia-0.1.7.tar` & `hypymedia-0.1.8.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1065 2023-08-02 02:59:53.232320 hypymedia-0.1.7/LICENSE
--rw-r--r--   0        0        0       11 2023-08-02 02:59:53.232449 hypymedia-0.1.7/README.md
--rw-r--r--   0        0        0     1158 2023-08-02 06:20:00.228959 hypymedia-0.1.7/hypymedia/__init__.py
--rw-r--r--   0        0        0     1698 2023-08-02 06:19:54.715505 hypymedia-0.1.7/hypymedia/html_list.py
--rw-r--r--   0        0        0     1159 2023-08-02 06:17:41.396821 hypymedia-0.1.7/hypymedia/main.py
--rw-r--r--   0        0        0      509 2023-08-02 06:20:54.719314 hypymedia-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      476 1970-01-01 00:00:00.000000 hypymedia-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-08-02 02:59:53.232320 hypymedia-0.1.8/LICENSE
+-rw-r--r--   0        0        0       11 2023-08-02 02:59:53.232449 hypymedia-0.1.8/README.md
+-rw-r--r--   0        0        0     1158 2023-08-02 06:28:06.936636 hypymedia-0.1.8/hypymedia/__init__.py
+-rw-r--r--   0        0        0     2241 2023-08-02 06:27:58.855068 hypymedia-0.1.8/hypymedia/html_list.py
+-rw-r--r--   0        0        0     1175 2023-08-02 06:30:34.782716 hypymedia-0.1.8/hypymedia/main.py
+-rw-r--r--   0        0        0      509 2023-08-02 06:30:52.824066 hypymedia-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      476 1970-01-01 00:00:00.000000 hypymedia-0.1.8/PKG-INFO
```

### Comparing `hypymedia-0.1.7/LICENSE` & `hypymedia-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `hypymedia-0.1.7/hypymedia/__init__.py` & `hypymedia-0.1.8/hypymedia/__init__.py`

 * *Files identical despite different names*

### Comparing `hypymedia-0.1.7/hypymedia/main.py` & `hypymedia-0.1.8/hypymedia/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from typing import Callable
-from html_list import tags
+from .html_list import tags
 
 
 def atts_factory(attributes: dict) -> str:
     """Check k, v pairs and stringify them.
     If value is `True` then return just the key without the value.
     """
     return " ".join(f'{k}="{v}"' if v is not True else k for k, v in attributes.items())
 
 
 ## TAG BUILDER
-def _el_factory(name: str, end_tag: bool = True) -> Callable:
-    if end_tag:
-        return lambda c="", a={}: _element(name, c, a)
-    else:
-        return lambda a={}: _element(name, attributes=a, end_tag=end_tag)
+def _el_factory(tag_name: str, end_tag: bool = True) -> Callable:
+    return (
+        lambda c="", a={}: _element(tag_name, c, a)
+        if end_tag
+        else lambda a={}: _element(tag_name, attributes=a, end_tag=end_tag)
+    )
 
 
 def _element(
     tag: str, content: list | str = "", attributes: dict = None, end_tag: bool = True
 ):
     """Build a HTML tag with attributes and content."""
```

