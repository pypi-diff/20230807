# Comparing `tmp/simplematrixbotlib-2.9.0.tar.gz` & `tmp/simplematrixbotlib-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simplematrixbotlib-2.9.0.tar", max compression
+gzip compressed data, was "simplematrixbotlib-2.9.1.tar", max compression
```

## Comparing `simplematrixbotlib-2.9.0.tar` & `simplematrixbotlib-2.9.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1075 2023-05-30 17:18:33.945024 simplematrixbotlib-2.9.0/LICENSE
--rw-r--r--   0        0        0     2271 2023-06-16 13:57:51.753082 simplematrixbotlib-2.9.0/README.md
--rw-r--r--   0        0        0     1232 2023-06-16 13:57:51.753082 simplematrixbotlib-2.9.0/pyproject.toml
--rw-r--r--   0        0        0      315 2023-06-15 21:39:14.814551 simplematrixbotlib-2.9.0/simplematrixbotlib/__init__.py
--rw-r--r--   0        0        0    15217 2023-06-16 13:26:29.928498 simplematrixbotlib-2.9.0/simplematrixbotlib/api.py
--rw-r--r--   0        0        0     4964 2023-06-15 21:39:14.814551 simplematrixbotlib-2.9.0/simplematrixbotlib/auth.py
--rw-r--r--   0        0        0     3041 2023-06-15 21:39:14.814551 simplematrixbotlib-2.9.0/simplematrixbotlib/bot.py
--rw-r--r--   0        0        0     8699 2023-06-15 21:39:14.814551 simplematrixbotlib-2.9.0/simplematrixbotlib/callbacks.py
--rw-r--r--   0        0        0     7698 2023-06-15 21:39:14.814551 simplematrixbotlib-2.9.0/simplematrixbotlib/config.py
--rw-r--r--   0        0        0     1054 2023-06-15 21:39:14.814551 simplematrixbotlib-2.9.0/simplematrixbotlib/listener.py
--rw-r--r--   0        0        0     5088 2023-06-15 21:39:14.814551 simplematrixbotlib-2.9.0/simplematrixbotlib/match.py
--rw-r--r--   0        0        0     3578 1970-01-01 00:00:00.000000 simplematrixbotlib-2.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-05-30 17:18:33.945024 simplematrixbotlib-2.9.1/LICENSE
+-rw-r--r--   0        0        0     2271 2023-07-25 01:19:19.548261 simplematrixbotlib-2.9.1/README.md
+-rw-r--r--   0        0        0     1232 2023-07-25 01:19:00.835962 simplematrixbotlib-2.9.1/pyproject.toml
+-rw-r--r--   0        0        0      315 2023-06-15 21:39:14.814551 simplematrixbotlib-2.9.1/simplematrixbotlib/__init__.py
+-rw-r--r--   0        0        0    15217 2023-06-16 13:26:29.928498 simplematrixbotlib-2.9.1/simplematrixbotlib/api.py
+-rw-r--r--   0        0        0     4964 2023-06-15 21:39:14.814551 simplematrixbotlib-2.9.1/simplematrixbotlib/auth.py
+-rw-r--r--   0        0        0     3041 2023-06-15 21:39:14.814551 simplematrixbotlib-2.9.1/simplematrixbotlib/bot.py
+-rw-r--r--   0        0        0     8699 2023-06-15 21:39:14.814551 simplematrixbotlib-2.9.1/simplematrixbotlib/callbacks.py
+-rw-r--r--   0        0        0     7860 2023-07-25 01:17:28.094470 simplematrixbotlib-2.9.1/simplematrixbotlib/config.py
+-rw-r--r--   0        0        0     1054 2023-06-15 21:39:14.814551 simplematrixbotlib-2.9.1/simplematrixbotlib/listener.py
+-rw-r--r--   0        0        0     5088 2023-06-15 21:39:14.814551 simplematrixbotlib-2.9.1/simplematrixbotlib/match.py
+-rw-r--r--   0        0        0     3578 1970-01-01 00:00:00.000000 simplematrixbotlib-2.9.1/PKG-INFO
```

### Comparing `simplematrixbotlib-2.9.0/LICENSE` & `simplematrixbotlib-2.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `simplematrixbotlib-2.9.0/README.md` & `simplematrixbotlib-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Simple-Matrix-Bot-Lib
-(Version 2.9.0)
+(Version 2.9.1)
 
 Simple-Matrix-Bot-Lib is a Python bot library for the Matrix ecosystem built on [matrix-nio](https://github.com/poljar/matrix-nio).
 
 [View on Github](https://github.com/i10b/simplematrixbotlib) or [View on PyPi](https://pypi.org/project/simplematrixbotlib/) or
 [View docs on readthedocs.io](https://simple-matrix-bot-lib.readthedocs.io/en/latest/)
 
 Learn how you can contribute [here](CONTRIBUTING.md).
```

### Comparing `simplematrixbotlib-2.9.0/pyproject.toml` & `simplematrixbotlib-2.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "simplematrixbotlib"
-version = "2.9.0"
+version = "2.9.1"
 description = "An easy to use bot library for the Matrix ecosystem written in Python."
 authors = ["imbev <imbev@protonmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://codeberg.org/imbev/simplematrixbotlib"
 documentation = "https://simple-matrix-bot-lib.readthedocs.io/en/latest/"
 keywords = [
```

### Comparing `simplematrixbotlib-2.9.0/simplematrixbotlib/api.py` & `simplematrixbotlib-2.9.1/simplematrixbotlib/api.py`

 * *Files identical despite different names*

### Comparing `simplematrixbotlib-2.9.0/simplematrixbotlib/auth.py` & `simplematrixbotlib-2.9.1/simplematrixbotlib/auth.py`

 * *Files identical despite different names*

### Comparing `simplematrixbotlib-2.9.0/simplematrixbotlib/bot.py` & `simplematrixbotlib-2.9.1/simplematrixbotlib/bot.py`

 * *Files identical despite different names*

### Comparing `simplematrixbotlib-2.9.0/simplematrixbotlib/callbacks.py` & `simplematrixbotlib-2.9.1/simplematrixbotlib/callbacks.py`

 * *Files identical despite different names*

### Comparing `simplematrixbotlib-2.9.0/simplematrixbotlib/config.py` & `simplematrixbotlib-2.9.1/simplematrixbotlib/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,19 +6,25 @@
 from nio.crypto import ENCRYPTION_ENABLED
 
 
 def _config_dict_factory(tmp) -> dict:
     return {
         'simplematrixbotlib': {
             'config':
-            {_strip_leading_underscore(name): value
+            {_strip_leading_underscore(name): _extract_pattern_if_neccessary(value)
              for name, value in tmp}
         }
     }
 
+def _extract_pattern_if_neccessary(value):
+    try:
+        return value.pattern
+    except AttributeError:
+        return value
+
 
 def _strip_leading_underscore(tmp: str) -> str:
     return tmp[1:] if tmp[0] == '_' else tmp
 
 
 def _check_set_regex(value: Set[str]) -> Union[Set[re.Pattern], None]:
     new_list = set()
```

### Comparing `simplematrixbotlib-2.9.0/simplematrixbotlib/listener.py` & `simplematrixbotlib-2.9.1/simplematrixbotlib/listener.py`

 * *Files identical despite different names*

### Comparing `simplematrixbotlib-2.9.0/simplematrixbotlib/match.py` & `simplematrixbotlib-2.9.1/simplematrixbotlib/match.py`

 * *Files identical despite different names*

### Comparing `simplematrixbotlib-2.9.0/PKG-INFO` & `simplematrixbotlib-2.9.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplematrixbotlib
-Version: 2.9.0
+Version: 2.9.1
 Summary: An easy to use bot library for the Matrix ecosystem written in Python.
 Home-page: https://codeberg.org/imbev/simplematrixbotlib
 License: MIT
 Keywords: simple,matrix,bot,lib,simple-matrix-bot-lib
 Author: imbev
 Author-email: imbev@protonmail.com
 Requires-Python: >=3.8,<4.0
@@ -25,15 +25,15 @@
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Project-URL: Documentation, https://simple-matrix-bot-lib.readthedocs.io/en/latest/
 Project-URL: Matrix Room, https://matrix.to/#/#simplematrixbotlib:matrix.org
 Project-URL: Repository, https://codeberg.org/imbev/simplematrixbotlib
 Description-Content-Type: text/markdown
 
 # Simple-Matrix-Bot-Lib
-(Version 2.9.0)
+(Version 2.9.1)
 
 Simple-Matrix-Bot-Lib is a Python bot library for the Matrix ecosystem built on [matrix-nio](https://github.com/poljar/matrix-nio).
 
 [View on Github](https://github.com/i10b/simplematrixbotlib) or [View on PyPi](https://pypi.org/project/simplematrixbotlib/) or
 [View docs on readthedocs.io](https://simple-matrix-bot-lib.readthedocs.io/en/latest/)
 
 Learn how you can contribute [here](CONTRIBUTING.md).
```

