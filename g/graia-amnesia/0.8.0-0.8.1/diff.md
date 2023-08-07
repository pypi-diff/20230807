# Comparing `tmp/graia_amnesia-0.8.0.tar.gz` & `tmp/graia_amnesia-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graia_amnesia-0.8.0.tar", last modified: Sun Aug  6 13:52:36 2023, max compression
+gzip compressed data, was "graia_amnesia-0.8.1.tar", last modified: Sun Aug  6 14:09:51 2023, max compression
```

## Comparing `graia_amnesia-0.8.0.tar` & `graia_amnesia-0.8.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1070 2023-08-06 13:52:25.327967 graia_amnesia-0.8.0/LICENSE
--rw-r--r--   0        0        0     1804 2023-08-06 13:52:25.327967 graia_amnesia-0.8.0/README.md
--rw-r--r--   0        0        0      631 2023-08-06 13:52:36.500010 graia_amnesia-0.8.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-08-06 13:52:25.331967 graia_amnesia-0.8.0/src/graia/amnesia/__init__.py
--rw-r--r--   0        0        0        0 2023-08-06 13:52:25.331967 graia_amnesia-0.8.0/src/graia/amnesia/builtins/__init__.py
--rw-r--r--   0        0        0     3337 2023-08-06 13:52:25.331967 graia_amnesia-0.8.0/src/graia/amnesia/builtins/asgi/__init__.py
--rw-r--r--   0        0        0     6238 2023-08-06 13:52:25.331967 graia_amnesia-0.8.0/src/graia/amnesia/builtins/asgi/asgitypes.py
--rw-r--r--   0        0        0     2800 2023-08-06 13:52:25.331967 graia_amnesia-0.8.0/src/graia/amnesia/builtins/asgi/middleware.py
--rw-r--r--   0        0        0     2539 2023-08-06 13:52:25.331967 graia_amnesia-0.8.0/src/graia/amnesia/builtins/memcache.py
--rw-r--r--   0        0        0      276 2023-08-06 13:52:25.331967 graia_amnesia-0.8.0/src/graia/amnesia/message/__init__.py
--rw-r--r--   0        0        0    19775 2023-08-06 13:52:25.331967 graia_amnesia-0.8.0/src/graia/amnesia/message/chain.py
--rw-r--r--   0        0        0     2078 2023-08-06 13:52:25.331967 graia_amnesia-0.8.0/src/graia/amnesia/message/element.py
--rw-r--r--   0        0        0     2222 2023-08-06 13:52:25.331967 graia_amnesia-0.8.0/src/graia/amnesia/message/formatter.py
--rw-r--r--   0        0        0     2539 2023-08-06 13:52:25.331967 graia_amnesia-0.8.0/src/graia/amnesia/utilles.py
--rw-r--r--   0        0        0     2123 1970-01-01 00:00:00.000000 graia_amnesia-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-08-06 14:09:39.768997 graia_amnesia-0.8.1/LICENSE
+-rw-r--r--   0        0        0     1804 2023-08-06 14:09:39.768997 graia_amnesia-0.8.1/README.md
+-rw-r--r--   0        0        0      605 2023-08-06 14:09:51.017239 graia_amnesia-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-06 14:09:39.768997 graia_amnesia-0.8.1/src/graia/amnesia/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-06 14:09:39.768997 graia_amnesia-0.8.1/src/graia/amnesia/builtins/__init__.py
+-rw-r--r--   0        0        0     3337 2023-08-06 14:09:39.768997 graia_amnesia-0.8.1/src/graia/amnesia/builtins/asgi/__init__.py
+-rw-r--r--   0        0        0     6238 2023-08-06 14:09:39.768997 graia_amnesia-0.8.1/src/graia/amnesia/builtins/asgi/asgitypes.py
+-rw-r--r--   0        0        0     2800 2023-08-06 14:09:39.768997 graia_amnesia-0.8.1/src/graia/amnesia/builtins/asgi/middleware.py
+-rw-r--r--   0        0        0     2539 2023-08-06 14:09:39.768997 graia_amnesia-0.8.1/src/graia/amnesia/builtins/memcache.py
+-rw-r--r--   0        0        0      276 2023-08-06 14:09:39.768997 graia_amnesia-0.8.1/src/graia/amnesia/message/__init__.py
+-rw-r--r--   0        0        0    19775 2023-08-06 14:09:39.768997 graia_amnesia-0.8.1/src/graia/amnesia/message/chain.py
+-rw-r--r--   0        0        0     2078 2023-08-06 14:09:39.768997 graia_amnesia-0.8.1/src/graia/amnesia/message/element.py
+-rw-r--r--   0        0        0     2222 2023-08-06 14:09:39.768997 graia_amnesia-0.8.1/src/graia/amnesia/message/formatter.py
+-rw-r--r--   0        0        0     2539 2023-08-06 14:09:39.768997 graia_amnesia-0.8.1/src/graia/amnesia/utilles.py
+-rw-r--r--   0        0        0     2154 1970-01-01 00:00:00.000000 graia_amnesia-0.8.1/PKG-INFO
```

### Comparing `graia_amnesia-0.8.0/LICENSE` & `graia_amnesia-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `graia_amnesia-0.8.0/README.md` & `graia_amnesia-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `graia_amnesia-0.8.0/pyproject.toml` & `graia_amnesia-0.8.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 [project]
 name = "graia-amnesia"
-version = "0.8.0"
+version = "0.8.1"
 authors = [
     { name = "GreyElaina", email = "GreyElaina@outlook.com" },
 ]
 requires-python = ">=3.8,<4.0"
 dependencies = [
     "launart>=0.7.0,<1.0.0",
     "typing-extensions>=4.0.0",
+    "uvicorn>=0.23.2",
 ]
 readme = "README.md"
 description = "a collection of shared components for graia"
 
 [project.license]
 text = "MIT"
 
-[project.urls]
-
-[project.optional-dependencies]
-
 [tool.pdm.build]
 includes = [
     "src/graia",
 ]
 
 [tool.pdm.dev-dependencies]
 dev = [
```

### Comparing `graia_amnesia-0.8.0/src/graia/amnesia/builtins/asgi/__init__.py` & `graia_amnesia-0.8.1/src/graia/amnesia/builtins/asgi/__init__.py`

 * *Files identical despite different names*

### Comparing `graia_amnesia-0.8.0/src/graia/amnesia/builtins/asgi/asgitypes.py` & `graia_amnesia-0.8.1/src/graia/amnesia/builtins/asgi/asgitypes.py`

 * *Files identical despite different names*

### Comparing `graia_amnesia-0.8.0/src/graia/amnesia/builtins/asgi/middleware.py` & `graia_amnesia-0.8.1/src/graia/amnesia/builtins/asgi/middleware.py`

 * *Files identical despite different names*

### Comparing `graia_amnesia-0.8.0/src/graia/amnesia/builtins/memcache.py` & `graia_amnesia-0.8.1/src/graia/amnesia/builtins/memcache.py`

 * *Files identical despite different names*

### Comparing `graia_amnesia-0.8.0/src/graia/amnesia/message/chain.py` & `graia_amnesia-0.8.1/src/graia/amnesia/message/chain.py`

 * *Files identical despite different names*

### Comparing `graia_amnesia-0.8.0/src/graia/amnesia/message/element.py` & `graia_amnesia-0.8.1/src/graia/amnesia/message/element.py`

 * *Files identical despite different names*

### Comparing `graia_amnesia-0.8.0/src/graia/amnesia/message/formatter.py` & `graia_amnesia-0.8.1/src/graia/amnesia/message/formatter.py`

 * *Files identical despite different names*

### Comparing `graia_amnesia-0.8.0/src/graia/amnesia/utilles.py` & `graia_amnesia-0.8.1/src/graia/amnesia/utilles.py`

 * *Files identical despite different names*

### Comparing `graia_amnesia-0.8.0/PKG-INFO` & `graia_amnesia-0.8.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: graia-amnesia
-Version: 0.8.0
+Version: 0.8.1
 Summary: a collection of shared components for graia
 Author-Email: GreyElaina <GreyElaina@outlook.com>
 License: MIT
 Requires-Python: <4.0,>=3.8
 Requires-Dist: launart<1.0.0,>=0.7.0
 Requires-Dist: typing-extensions>=4.0.0
+Requires-Dist: uvicorn>=0.23.2
 Description-Content-Type: text/markdown
 
 <div align="center">
 
 # Amnesia
 
 _A collection of common components for Graia Project._
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: graia-amnesia Version: 0.8.0 Summary: a collection
+Metadata-Version: 2.1 Name: graia-amnesia Version: 0.8.1 Summary: a collection
 of shared components for graia Author-Email: GreyElaina
 outlook.com> License: MIT Requires-Python: <4.0,>=3.8 Requires-Dist:
-launart<1.0.0,>=0.7.0 Requires-Dist: typing-extensions>=4.0.0 Description-
-Content-Type: text/markdown
+launart<1.0.0,>=0.7.0 Requires-Dist: typing-extensions>=4.0.0 Requires-Dist:
+uvicorn>=0.23.2 Description-Content-Type: text/markdown
       # Amnesia _A collection of common components for Graia Project._ >
         äºæ¯æå¤©ä»å°å°æ¥. > æ¯ä¸å¤©é½ä¼å¸¦æ¥æ°çéé,
                 çºµä½¿æç»å¿å´ä¹ä¸ä¼å®³ææå¤©å°æ¥.
       [PyPI] [code_style] [https://img.shields.io/badge/%20imports-isort-
  %231674b1?style=flat&labelColor=ef8336] [https://results.pre-commit.ci/badge/
                     github/GraiaProject/Amnesia/master.svg]
 ## ç®è¿° Amnesia æ¯ä¸ç³»åå±ç¨ç»ä»¶çéå, åå«äºä»¥ä¸åå®¹: -
```

