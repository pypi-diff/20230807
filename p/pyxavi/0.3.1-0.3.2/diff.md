# Comparing `tmp/pyxavi-0.3.1.tar.gz` & `tmp/pyxavi-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxavi-0.3.1.tar", max compression
+gzip compressed data, was "pyxavi-0.3.2.tar", max compression
```

## Comparing `pyxavi-0.3.1.tar` & `pyxavi-0.3.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1041 2023-08-06 22:00:22.371972 pyxavi-0.3.1/CHANGELOG.md
--rw-r--r--   0        0        0    35149 2023-08-01 05:28:28.621212 pyxavi-0.3.1/LICENSE
--rw-r--r--   0        0        0     4667 2023-08-06 22:00:22.371972 pyxavi-0.3.1/README.md
--rw-r--r--   0        0        0     1601 2023-08-06 22:00:22.371972 pyxavi-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      298 2023-08-06 08:44:06.701424 pyxavi-0.3.1/pyxavi/__init__
--rw-r--r--   0        0        0      962 2023-08-01 05:28:28.621212 pyxavi-0.3.1/pyxavi/config.py
--rw-r--r--   0        0        0     9504 2023-08-06 08:44:06.701424 pyxavi-0.3.1/pyxavi/debugger.py
--rw-r--r--   0        0        0     3083 2023-08-01 05:28:28.621212 pyxavi-0.3.1/pyxavi/janitor.py
--rw-r--r--   0        0        0     1544 2023-08-01 05:28:28.621212 pyxavi-0.3.1/pyxavi/logger.py
--rw-r--r--   0        0        0     1440 2023-08-01 05:28:28.621212 pyxavi-0.3.1/pyxavi/media.py
--rw-r--r--   0        0        0     3323 2023-08-01 05:28:28.621212 pyxavi-0.3.1/pyxavi/storage.py
--rw-r--r--   0        0        0      719 2023-08-06 08:44:06.701424 pyxavi-0.3.1/pyxavi/terminal_color.py
--rw-r--r--   0        0        0     5520 1970-01-01 00:00:00.000000 pyxavi-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1132 2023-08-07 09:21:29.055340 pyxavi-0.3.2/CHANGELOG.md
+-rw-r--r--   0        0        0    35149 2023-08-01 05:28:28.621212 pyxavi-0.3.2/LICENSE
+-rw-r--r--   0        0        0     4667 2023-08-06 22:00:22.371972 pyxavi-0.3.2/README.md
+-rw-r--r--   0        0        0     1601 2023-08-07 09:21:29.055340 pyxavi-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      298 2023-08-06 08:44:06.701424 pyxavi-0.3.2/pyxavi/__init__
+-rw-r--r--   0        0        0      962 2023-08-01 05:28:28.621212 pyxavi-0.3.2/pyxavi/config.py
+-rw-r--r--   0        0        0     9525 2023-08-07 09:21:29.055340 pyxavi-0.3.2/pyxavi/debugger.py
+-rw-r--r--   0        0        0     3083 2023-08-01 05:28:28.621212 pyxavi-0.3.2/pyxavi/janitor.py
+-rw-r--r--   0        0        0     1544 2023-08-01 05:28:28.621212 pyxavi-0.3.2/pyxavi/logger.py
+-rw-r--r--   0        0        0     1440 2023-08-01 05:28:28.621212 pyxavi-0.3.2/pyxavi/media.py
+-rw-r--r--   0        0        0     3323 2023-08-01 05:28:28.621212 pyxavi-0.3.2/pyxavi/storage.py
+-rw-r--r--   0        0        0      719 2023-08-06 08:44:06.701424 pyxavi-0.3.2/pyxavi/terminal_color.py
+-rw-r--r--   0        0        0     5520 1970-01-01 00:00:00.000000 pyxavi-0.3.2/PKG-INFO
```

### Comparing `pyxavi-0.3.1/CHANGELOG.md` & `pyxavi-0.3.2/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# v0.3.2
+
+- Make non built-in objects inspection depth controlable in `dd` recurdive call
+
 # v0.3.1
 
 - Iterate over the `pyproject.toml` and the `README.md` to make them more appealing in pypi.org
 
 # v0.3.0
 
 - Rewrite the `debugger.dd`.
```

### Comparing `pyxavi-0.3.1/LICENSE` & `pyxavi-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyxavi-0.3.1/README.md` & `pyxavi-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `pyxavi-0.3.1/pyproject.toml` & `pyxavi-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyxavi"
-version = "0.3.1"
+version = "0.3.2"
 description = "Set of utilities to assist on simple Python projects"
 authors = ["Xavier Arnaus <xavi@arnaus.net>"]
 readme = "README.md"
 license = "GPLv3"
 repository = "https://github.com/XaviArnaus/pyxavi"
 homepage = "https://github.com/XaviArnaus/pyxavi"
 include = [
```

### Comparing `pyxavi-0.3.1/pyxavi/config.py` & `pyxavi-0.3.2/pyxavi/config.py`

 * *Files identical despite different names*

### Comparing `pyxavi-0.3.1/pyxavi/debugger.py` & `pyxavi-0.3.2/pyxavi/debugger.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,15 +149,15 @@
             leave_char = f"{COLOR.DICT_KEY}{LEAVE_DICT}{COLOR.END}"
 
             try:
                 for key, element in what.__dict__.items():
                     sub_is_complex, sub_content_item = dump(
                         what=element,
                         level=level + 1,
-                        max_deep_level=NON_BUILTIN_OBJECTS_MAX_DEPTH,
+                        max_deep_level=min(max_deep_level, NON_BUILTIN_OBJECTS_MAX_DEPTH),
                         colorise=colorise
                     )
                     sub_content_item = f"{COLOR.STR}\"{key}\"{COLOR.END}: {sub_content_item}"
                     sub_content.append(sub_content_item)
                     sub_complexity.append(sub_is_complex)
             except RuntimeError:
                 sub_content.append(f"{COLOR.ERROR}Unknown{COLOR.END}")
```

### Comparing `pyxavi-0.3.1/pyxavi/janitor.py` & `pyxavi-0.3.2/pyxavi/janitor.py`

 * *Files identical despite different names*

### Comparing `pyxavi-0.3.1/pyxavi/logger.py` & `pyxavi-0.3.2/pyxavi/logger.py`

 * *Files identical despite different names*

### Comparing `pyxavi-0.3.1/pyxavi/media.py` & `pyxavi-0.3.2/pyxavi/media.py`

 * *Files identical despite different names*

### Comparing `pyxavi-0.3.1/pyxavi/storage.py` & `pyxavi-0.3.2/pyxavi/storage.py`

 * *Files identical despite different names*

### Comparing `pyxavi-0.3.1/pyxavi/terminal_color.py` & `pyxavi-0.3.2/pyxavi/terminal_color.py`

 * *Files identical despite different names*

### Comparing `pyxavi-0.3.1/PKG-INFO` & `pyxavi-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxavi
-Version: 0.3.1
+Version: 0.3.2
 Summary: Set of utilities to assist on simple Python projects
 Home-page: https://github.com/XaviArnaus/pyxavi
 License: GPLv3
 Author: Xavier Arnaus
 Author-email: xavi@arnaus.net
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

