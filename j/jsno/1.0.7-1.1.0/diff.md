# Comparing `tmp/jsno-1.0.7.tar.gz` & `tmp/jsno-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsno-1.0.7.tar", last modified: Thu Aug  3 21:12:12 2023, max compression
+gzip compressed data, was "jsno-1.1.0.tar", last modified: Mon Aug  7 13:55:47 2023, max compression
```

## Comparing `jsno-1.0.7.tar` & `jsno-1.1.0.tar`

### file list

```diff
@@ -1,36 +1,44 @@
-drwxr-xr-x   0 pekka      (501) staff       (20)        0 2023-08-03 21:12:12.297030 jsno-1.0.7/
--rw-r--r--   0 pekka      (501) staff       (20)     1060 2023-07-11 17:26:17.000000 jsno-1.0.7/LICENSE
--rw-r--r--   0 pekka      (501) staff       (20)    11194 2023-08-03 21:12:12.296740 jsno-1.0.7/PKG-INFO
--rw-r--r--   0 pekka      (501) staff       (20)     9520 2023-08-03 21:06:29.000000 jsno-1.0.7/README.md
-drwxr-xr-x   0 pekka      (501) staff       (20)        0 2023-08-03 21:12:12.292356 jsno-1.0.7/jsno/
--rw-r--r--   0 pekka      (501) staff       (20)     1811 2023-08-03 20:19:36.000000 jsno-1.0.7/jsno/__init__.py
--rw-r--r--   0 pekka      (501) staff       (20)     2316 2023-07-29 19:39:45.000000 jsno-1.0.7/jsno/abc.py
--rw-r--r--   0 pekka      (501) staff       (20)     1671 2023-08-03 21:11:29.000000 jsno-1.0.7/jsno/constraint.py
--rw-r--r--   0 pekka      (501) staff       (20)     4542 2023-07-29 19:39:45.000000 jsno-1.0.7/jsno/jsonify.py
--rw-r--r--   0 pekka      (501) staff       (20)      710 2023-07-30 15:32:48.000000 jsno-1.0.7/jsno/jsonize.py
--rw-r--r--   0 pekka      (501) staff       (20)      630 2023-07-29 19:08:24.000000 jsno-1.0.7/jsno/method.py
--rw-r--r--   0 pekka      (501) staff       (20)     5612 2023-08-03 21:00:45.000000 jsno-1.0.7/jsno/standard.py
--rw-r--r--   0 pekka      (501) staff       (20)     4469 2023-08-03 21:09:15.000000 jsno-1.0.7/jsno/unjsonify.py
--rw-r--r--   0 pekka      (501) staff       (20)      882 2023-07-29 19:39:45.000000 jsno-1.0.7/jsno/utils.py
--rw-r--r--   0 pekka      (501) staff       (20)     3437 2023-07-29 19:39:45.000000 jsno-1.0.7/jsno/variant.py
-drwxr-xr-x   0 pekka      (501) staff       (20)        0 2023-08-03 21:12:12.293572 jsno-1.0.7/jsno.egg-info/
--rw-r--r--   0 pekka      (501) staff       (20)    11194 2023-08-03 21:12:12.000000 jsno-1.0.7/jsno.egg-info/PKG-INFO
--rw-r--r--   0 pekka      (501) staff       (20)      612 2023-08-03 21:12:12.000000 jsno-1.0.7/jsno.egg-info/SOURCES.txt
--rw-r--r--   0 pekka      (501) staff       (20)        1 2023-08-03 21:12:12.000000 jsno-1.0.7/jsno.egg-info/dependency_links.txt
--rw-r--r--   0 pekka      (501) staff       (20)       23 2023-08-03 21:12:12.000000 jsno-1.0.7/jsno.egg-info/requires.txt
--rw-r--r--   0 pekka      (501) staff       (20)        5 2023-08-03 21:12:12.000000 jsno-1.0.7/jsno.egg-info/top_level.txt
--rw-r--r--   0 pekka      (501) staff       (20)      639 2023-08-03 20:47:22.000000 jsno-1.0.7/pyproject.toml
--rw-r--r--   0 pekka      (501) staff       (20)       38 2023-08-03 21:12:12.297092 jsno-1.0.7/setup.cfg
-drwxr-xr-x   0 pekka      (501) staff       (20)        0 2023-08-03 21:12:12.296423 jsno-1.0.7/tests/
--rw-r--r--   0 pekka      (501) staff       (20)     1223 2023-07-29 19:21:09.000000 jsno-1.0.7/tests/test_abc.py
--rw-r--r--   0 pekka      (501) staff       (20)      936 2023-07-30 15:34:37.000000 jsno-1.0.7/tests/test_ast_example.py
--rw-r--r--   0 pekka      (501) staff       (20)     1515 2023-08-03 21:08:45.000000 jsno-1.0.7/tests/test_constraint.py
--rw-r--r--   0 pekka      (501) staff       (20)     4205 2023-07-29 18:53:29.000000 jsno-1.0.7/tests/test_dataclasses.py
--rw-r--r--   0 pekka      (501) staff       (20)     3220 2023-08-03 21:08:27.000000 jsno-1.0.7/tests/test_dates.py
--rw-r--r--   0 pekka      (501) staff       (20)      165 2023-07-30 07:55:38.000000 jsno-1.0.7/tests/test_dumps_and_loads.py
--rw-r--r--   0 pekka      (501) staff       (20)     1794 2023-07-30 15:34:48.000000 jsno-1.0.7/tests/test_examples.py
--rw-r--r--   0 pekka      (501) staff       (20)     2437 2023-07-29 18:53:15.000000 jsno-1.0.7/tests/test_jsonify.py
--rw-r--r--   0 pekka      (501) staff       (20)     2735 2023-07-29 18:46:29.000000 jsno-1.0.7/tests/test_methods.py
--rw-r--r--   0 pekka      (501) staff       (20)     1713 2023-07-29 18:45:56.000000 jsno-1.0.7/tests/test_standard.py
--rw-r--r--   0 pekka      (501) staff       (20)     4560 2023-08-03 21:08:35.000000 jsno-1.0.7/tests/test_unjsonify.py
--rw-r--r--   0 pekka      (501) staff       (20)     2886 2023-07-29 18:52:46.000000 jsno-1.0.7/tests/test_variant.py
+drwxr-xr-x   0 pekka      (501) staff       (20)        0 2023-08-07 13:55:47.205730 jsno-1.1.0/
+-rw-r--r--   0 pekka      (501) staff       (20)     1060 2023-07-11 17:26:17.000000 jsno-1.1.0/LICENSE
+-rw-r--r--   0 pekka      (501) staff       (20)    13801 2023-08-07 13:55:47.204945 jsno-1.1.0/PKG-INFO
+-rw-r--r--   0 pekka      (501) staff       (20)    12127 2023-08-07 13:53:14.000000 jsno-1.1.0/README.md
+drwxr-xr-x   0 pekka      (501) staff       (20)        0 2023-08-07 13:55:47.192037 jsno-1.1.0/jsno/
+-rw-r--r--   0 pekka      (501) staff       (20)     1968 2023-08-07 13:53:14.000000 jsno-1.1.0/jsno/__init__.py
+-rw-r--r--   0 pekka      (501) staff       (20)     3263 2023-08-07 13:53:14.000000 jsno-1.1.0/jsno/abc.py
+-rw-r--r--   0 pekka      (501) staff       (20)     3093 2023-08-07 13:53:14.000000 jsno-1.1.0/jsno/constraint.py
+-rw-r--r--   0 pekka      (501) staff       (20)     3450 2023-08-07 13:53:14.000000 jsno-1.1.0/jsno/datetime.py
+-rw-r--r--   0 pekka      (501) staff       (20)      472 2023-08-07 13:53:14.000000 jsno-1.1.0/jsno/extra_data.py
+-rw-r--r--   0 pekka      (501) staff       (20)     4921 2023-08-07 13:53:14.000000 jsno-1.1.0/jsno/jsonify.py
+-rw-r--r--   0 pekka      (501) staff       (20)      710 2023-07-30 15:32:48.000000 jsno-1.1.0/jsno/jsonize.py
+-rw-r--r--   0 pekka      (501) staff       (20)      630 2023-08-07 06:49:59.000000 jsno-1.1.0/jsno/method.py
+-rw-r--r--   0 pekka      (501) staff       (20)      793 2023-08-07 13:53:14.000000 jsno-1.1.0/jsno/record.py
+-rw-r--r--   0 pekka      (501) staff       (20)     3380 2023-08-07 13:53:14.000000 jsno-1.1.0/jsno/standard.py
+-rw-r--r--   0 pekka      (501) staff       (20)     2113 2023-08-07 13:53:14.000000 jsno-1.1.0/jsno/tuple.py
+-rw-r--r--   0 pekka      (501) staff       (20)     1232 2023-08-07 13:53:14.000000 jsno-1.1.0/jsno/typeddict.py
+-rw-r--r--   0 pekka      (501) staff       (20)     6650 2023-08-07 13:53:14.000000 jsno-1.1.0/jsno/unjsonify.py
+-rw-r--r--   0 pekka      (501) staff       (20)     2005 2023-08-07 13:53:14.000000 jsno-1.1.0/jsno/utils.py
+-rw-r--r--   0 pekka      (501) staff       (20)     3437 2023-07-29 19:39:45.000000 jsno-1.1.0/jsno/variant.py
+drwxr-xr-x   0 pekka      (501) staff       (20)        0 2023-08-07 13:55:47.194278 jsno-1.1.0/jsno.egg-info/
+-rw-r--r--   0 pekka      (501) staff       (20)    13801 2023-08-07 13:55:47.000000 jsno-1.1.0/jsno.egg-info/PKG-INFO
+-rw-r--r--   0 pekka      (501) staff       (20)      760 2023-08-07 13:55:47.000000 jsno-1.1.0/jsno.egg-info/SOURCES.txt
+-rw-r--r--   0 pekka      (501) staff       (20)        1 2023-08-07 13:55:47.000000 jsno-1.1.0/jsno.egg-info/dependency_links.txt
+-rw-r--r--   0 pekka      (501) staff       (20)       23 2023-08-07 13:55:47.000000 jsno-1.1.0/jsno.egg-info/requires.txt
+-rw-r--r--   0 pekka      (501) staff       (20)        5 2023-08-07 13:55:47.000000 jsno-1.1.0/jsno.egg-info/top_level.txt
+-rw-r--r--   0 pekka      (501) staff       (20)      639 2023-08-07 13:55:13.000000 jsno-1.1.0/pyproject.toml
+-rw-r--r--   0 pekka      (501) staff       (20)       38 2023-08-07 13:55:47.205853 jsno-1.1.0/setup.cfg
+drwxr-xr-x   0 pekka      (501) staff       (20)        0 2023-08-07 13:55:47.204053 jsno-1.1.0/tests/
+-rw-r--r--   0 pekka      (501) staff       (20)     2155 2023-08-05 08:13:56.000000 jsno-1.1.0/tests/test_abc.py
+-rw-r--r--   0 pekka      (501) staff       (20)      936 2023-07-30 15:34:37.000000 jsno-1.1.0/tests/test_ast_example.py
+-rw-r--r--   0 pekka      (501) staff       (20)     2583 2023-08-04 19:08:47.000000 jsno-1.1.0/tests/test_constraint.py
+-rw-r--r--   0 pekka      (501) staff       (20)     5411 2023-08-07 13:53:14.000000 jsno-1.1.0/tests/test_dataclasses.py
+-rw-r--r--   0 pekka      (501) staff       (20)     4771 2023-08-07 13:53:14.000000 jsno-1.1.0/tests/test_dates.py
+-rw-r--r--   0 pekka      (501) staff       (20)      165 2023-07-30 07:55:38.000000 jsno-1.1.0/tests/test_dumps_and_loads.py
+-rw-r--r--   0 pekka      (501) staff       (20)     1794 2023-07-30 15:34:48.000000 jsno-1.1.0/tests/test_examples.py
+-rw-r--r--   0 pekka      (501) staff       (20)     2651 2023-08-06 13:26:16.000000 jsno-1.1.0/tests/test_jsonify.py
+-rw-r--r--   0 pekka      (501) staff       (20)     2735 2023-07-29 18:46:29.000000 jsno-1.1.0/tests/test_methods.py
+-rw-r--r--   0 pekka      (501) staff       (20)      959 2023-08-04 18:24:39.000000 jsno-1.1.0/tests/test_record.py
+-rw-r--r--   0 pekka      (501) staff       (20)     1911 2023-08-07 13:53:14.000000 jsno-1.1.0/tests/test_standard.py
+-rw-r--r--   0 pekka      (501) staff       (20)     1835 2023-08-07 13:53:14.000000 jsno-1.1.0/tests/test_typeddict.py
+-rw-r--r--   0 pekka      (501) staff       (20)     5170 2023-08-05 08:48:15.000000 jsno-1.1.0/tests/test_unjsonify.py
+-rw-r--r--   0 pekka      (501) staff       (20)      277 2023-08-07 13:53:14.000000 jsno-1.1.0/tests/test_utils.py
+-rw-r--r--   0 pekka      (501) staff       (20)     2886 2023-07-29 18:52:46.000000 jsno-1.1.0/tests/test_variant.py
```

### Comparing `jsno-1.0.7/LICENSE` & `jsno-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jsno-1.0.7/PKG-INFO` & `jsno-1.1.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,44 +1,9 @@
-Metadata-Version: 2.1
-Name: jsno
-Version: 1.0.7
-Summary: Convert Python data to and from json-compatible data structures
-License: MIT License
-        
-        Copyright (c) 2023 pek
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: Homepage, https://github.com/pek/jsno
-Keywords: json
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.11
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # jsno
+
 Convert Python data to and from JSON-compatible data structures.
 
 Jsno provides functions that turn any Python values into JSON-compatible
 structures and back. The jsonified data can then be used wherever JSON
 data is required: it can be dumped into a file, sent over the network
 in an API call, or stored in a database that support JSON data.
 
@@ -183,20 +148,25 @@
 _variant family_.
 
 ### Other standard Python types
 
 * tuples
 * ranges
 * enums
-* date and datetime objects (converted to ISO-formatted strings)
+* date and, time and datetime objects (converted to ISO-formatted strings)
+* timedelta and timezone
 * complex
 * decimal.Decimal (converted to JSON strings)
 * pathlib.Path
+* re.Pattern
 * zoneinfo.ZoneInfo
 * Literal (only int and str literals)
+* NamedTuple
+* TypedDict
+* NewType
 
 ## Dumps and loads
 
 Jsno provides shortcut functions _dumps_ and _loads_ with interface that is
 similar to the standard _json_ module function.s _jsno.dumps_ both jsonifies its argument
 and turns it into a JSON-encoded string, similar to standard _json.dumps_
 function. Correspondinly, _jsno.loads_ both decodes and unjsonify JSON data.
@@ -255,14 +225,32 @@
 
 
 def load_game(database, identifier: str) -> GameState:
     json = database.load(identifier)
     return unjsonify[GameState](json)
 ```
 
+## Unjsonify context
+
+By default, the unjsonify raises an error (UjsonifyError), if the JSON object
+that is being converted to a dataclass contains extra keys. This is often the
+most appropriate behavior, for example when converting the request body of an API
+request, it's best to let the caller know that they might have mistyped property
+names in their data. However, sometimes, it's best to just ignore the extra properties,
+for example when reading persistent data that could have obsolete properties in it
+that are not reflected by the dataclass definition.
+
+The extra key behavior can be controlled by running the unjsonification inside
+the approproate _context_:
+
+```py
+with unjsonify.ignore_extra_keys:
+    state = unjsonify[GameState](data)
+```
+
 ## Constraints
 
 Jsno support annotating types with constraints that are boolean valued functions
 that must return True for the unjsonified value for it to be valid. For example,
 to only accept email addresses that contain the "@" character:
 
 ```py
@@ -272,23 +260,69 @@
 @dataclass
 class User:
     username: str
     email: Annotated[str, Constraint(lambda it: "@" in it)]
 
 ```
 
+Constraints are always used within Annotated, so there is a shortcut operator to
+make the definitions clearer. This is equivalent to the definition above:
+
+```py
+@dataclass
+class User:
+    username: str
+    email: str // Constraint(lambda it: "@" in it)
+
+```
+
+Using the `//`-operator, the type of the property is directly after the colon,
+not nested inside an Annotated-expression.
+
 The most typical constraints are those that limit the value or the length of a
 property to a certain range. For these, jsno provides predefined shortcuts:
 
-
 ```py
 @dataclass
 class Player:
-    username: Annotated[str, Constraint.len(min=4, max=16)]
-    credits: Annotated[int, Constraint.range(min=0)]
+    username: str // Constraint.len(min=4, max=16)
+    credits: int // Constraint.range(min=0)
+```
+
+There is also a constraint for matching the value with a regular expression:
+
+```py
+@dataclass
+class Variable:
+    name: str // Constraint.regex("[A-Za-z_][A-Za-z0-9_]*")
+```
+
+Constraints can be joined using the or-operator `|`:
+
+```py
+LiteralInt = Constraint.regex("[0-9]*")
+LiteralString = Constraint.regex('".*"')
+
+@dataclass
+class LiteralValue:
+    value: str // (LiteralInt | LiteralString)
+```
+
+## Anonymous record types
+
+Sometimes it's better to define substructures in complex data inline, without
+lifting them into named types. For this purpose, jsno provides "Record" type
+constructor, to conveniently define one-off dataclasses:
+
+```py
+@dataclass
+class User:
+    username: str
+    email: str
+    apikeys: list[Record(value=str, created_at=datetime)]
 ```
 
 ## Variant families
 
 Sometimes it's useful to have a hierarchy of classes, consisting of several subclasses
 that need to be stored in JSON. A typical example is defining the AST (abstract syntax
 tree) for a domain-specific language. Here's the AST of a simple expression language,
@@ -422,7 +456,34 @@
 Install jsno with pip:
 
 ```bash
 pip install jsno
 ```
 
 Jsno has no 3rd party dependencies.
+
+
+## Release Notes
+
+### Version 1.1.0 (2023-08-07)
+
+* regular expression constraints
+* operator // for constraints
+* joining constraints with | operator
+* anonymous Record types
+* support for datetime.timezone and datetime.timedelta
+* support for re.Pattern
+* support for TypedDict and NewType
+* support for untyped tuples and namedtuples
+* unjsonify context for ignoring extra properties
+* specifying target for extra properties in dataclasses
+* performance improvements for unjsonify
+
+### Version 1.0.7 (2023-08-04)
+
+* support for typing.Annotated
+* constraint annotations
+
+### Version 1.0.6 (2023-08-03)
+
+* support for datetime.time
+
```

### Comparing `jsno-1.0.7/README.md` & `jsno-1.1.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,45 @@
+Metadata-Version: 2.1
+Name: jsno
+Version: 1.1.0
+Summary: Convert Python data to and from json-compatible data structures
+License: MIT License
+        
+        Copyright (c) 2023 pek
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: Homepage, https://github.com/pek/jsno
+Keywords: json
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
 # jsno
+
 Convert Python data to and from JSON-compatible data structures.
 
 Jsno provides functions that turn any Python values into JSON-compatible
 structures and back. The jsonified data can then be used wherever JSON
 data is required: it can be dumped into a file, sent over the network
 in an API call, or stored in a database that support JSON data.
 
@@ -147,20 +184,25 @@
 _variant family_.
 
 ### Other standard Python types
 
 * tuples
 * ranges
 * enums
-* date and datetime objects (converted to ISO-formatted strings)
+* date and, time and datetime objects (converted to ISO-formatted strings)
+* timedelta and timezone
 * complex
 * decimal.Decimal (converted to JSON strings)
 * pathlib.Path
+* re.Pattern
 * zoneinfo.ZoneInfo
 * Literal (only int and str literals)
+* NamedTuple
+* TypedDict
+* NewType
 
 ## Dumps and loads
 
 Jsno provides shortcut functions _dumps_ and _loads_ with interface that is
 similar to the standard _json_ module function.s _jsno.dumps_ both jsonifies its argument
 and turns it into a JSON-encoded string, similar to standard _json.dumps_
 function. Correspondinly, _jsno.loads_ both decodes and unjsonify JSON data.
@@ -219,14 +261,32 @@
 
 
 def load_game(database, identifier: str) -> GameState:
     json = database.load(identifier)
     return unjsonify[GameState](json)
 ```
 
+## Unjsonify context
+
+By default, the unjsonify raises an error (UjsonifyError), if the JSON object
+that is being converted to a dataclass contains extra keys. This is often the
+most appropriate behavior, for example when converting the request body of an API
+request, it's best to let the caller know that they might have mistyped property
+names in their data. However, sometimes, it's best to just ignore the extra properties,
+for example when reading persistent data that could have obsolete properties in it
+that are not reflected by the dataclass definition.
+
+The extra key behavior can be controlled by running the unjsonification inside
+the approproate _context_:
+
+```py
+with unjsonify.ignore_extra_keys:
+    state = unjsonify[GameState](data)
+```
+
 ## Constraints
 
 Jsno support annotating types with constraints that are boolean valued functions
 that must return True for the unjsonified value for it to be valid. For example,
 to only accept email addresses that contain the "@" character:
 
 ```py
@@ -236,23 +296,69 @@
 @dataclass
 class User:
     username: str
     email: Annotated[str, Constraint(lambda it: "@" in it)]
 
 ```
 
+Constraints are always used within Annotated, so there is a shortcut operator to
+make the definitions clearer. This is equivalent to the definition above:
+
+```py
+@dataclass
+class User:
+    username: str
+    email: str // Constraint(lambda it: "@" in it)
+
+```
+
+Using the `//`-operator, the type of the property is directly after the colon,
+not nested inside an Annotated-expression.
+
 The most typical constraints are those that limit the value or the length of a
 property to a certain range. For these, jsno provides predefined shortcuts:
 
-
 ```py
 @dataclass
 class Player:
-    username: Annotated[str, Constraint.len(min=4, max=16)]
-    credits: Annotated[int, Constraint.range(min=0)]
+    username: str // Constraint.len(min=4, max=16)
+    credits: int // Constraint.range(min=0)
+```
+
+There is also a constraint for matching the value with a regular expression:
+
+```py
+@dataclass
+class Variable:
+    name: str // Constraint.regex("[A-Za-z_][A-Za-z0-9_]*")
+```
+
+Constraints can be joined using the or-operator `|`:
+
+```py
+LiteralInt = Constraint.regex("[0-9]*")
+LiteralString = Constraint.regex('".*"')
+
+@dataclass
+class LiteralValue:
+    value: str // (LiteralInt | LiteralString)
+```
+
+## Anonymous record types
+
+Sometimes it's better to define substructures in complex data inline, without
+lifting them into named types. For this purpose, jsno provides "Record" type
+constructor, to conveniently define one-off dataclasses:
+
+```py
+@dataclass
+class User:
+    username: str
+    email: str
+    apikeys: list[Record(value=str, created_at=datetime)]
 ```
 
 ## Variant families
 
 Sometimes it's useful to have a hierarchy of classes, consisting of several subclasses
 that need to be stored in JSON. A typical example is defining the AST (abstract syntax
 tree) for a domain-specific language. Here's the AST of a simple expression language,
@@ -386,7 +492,34 @@
 Install jsno with pip:
 
 ```bash
 pip install jsno
 ```
 
 Jsno has no 3rd party dependencies.
+
+
+## Release Notes
+
+### Version 1.1.0 (2023-08-07)
+
+* regular expression constraints
+* operator // for constraints
+* joining constraints with | operator
+* anonymous Record types
+* support for datetime.timezone and datetime.timedelta
+* support for re.Pattern
+* support for TypedDict and NewType
+* support for untyped tuples and namedtuples
+* unjsonify context for ignoring extra properties
+* specifying target for extra properties in dataclasses
+* performance improvements for unjsonify
+
+### Version 1.0.7 (2023-08-04)
+
+* support for typing.Annotated
+* constraint annotations
+
+### Version 1.0.6 (2023-08-03)
+
+* support for datetime.time
+
```

### Comparing `jsno-1.0.7/jsno/__init__.py` & `jsno-1.1.0/jsno/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,34 +30,40 @@
 A custom class can be made compatible also by marking it with the
 `jsonify_with_method` deorator, and providing jsonify method and
 unjsonify class method.
 
 """
 
 from jsno.constraint import Constraint
+from jsno.extra_data import extra_data
 from jsno.jsonify import jsonify
 from jsno.jsonize import loads, dumps
 from jsno.method import jsonify_with_method
+from jsno.record import Record
 from jsno.standard import jsonify_as_string
 from jsno.unjsonify import unjsonify, UnjsonifyError
 from jsno.variant import get_variantfamily, variantfamily, variantlabel, VariantFamily
 
 # import to register jsonifiers
 import jsno.abc  # noqa
+import jsno.datetime  # noqa
+import jsno.tuple  # noqa
 
 
-__version__ = "1.0.7"
+__version__ = "1.1.0"
 
 __all__ = [
     "dumps",
     "jsonify",
     "jsonify_as_string",
     "jsonify_with_method",
+    "extra_data",
     "get_variantfamily",
     "loads",
     "unjsonify",
     "variantfamily",
     "variantlabel",
     "Constraint",
+    "Record",
     "UnjsonifyError",
     "VariantFamily",
 ]
```

### Comparing `jsno-1.0.7/jsno/abc.py` & `jsno-1.1.0/jsno/tuple.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,107 +1,76 @@
-"""
-Jsonification and unjsonification for abstract base classes
-"""
+import inspect
+import typing
 
-import base64
+from collections.abc import Sequence
 
-from collections.abc import ByteString, Mapping, Sequence, Set
+from jsno.abc import unjsonify_sequence_factory
+from jsno.unjsonify import unjsonify, typecheck, raise_error
 
-from jsno.jsonify import jsonify
-from jsno.unjsonify import unjsonify, typecheck, raise_error, cast
-from jsno.utils import get_args
 
+def unjsonify_typed_factory(as_type):
+    arg_types = typing.get_args(as_type)
 
-# Mapping
+    if arg_types and len(arg_types) == 2 and arg_types[1] is Ellipsis:
+        # special case for a N-length one-type tuple (tuple[T, ...])
+        # note: this accepts the empty tuple. This might not be strictly allowed
+        return unjsonify_sequence_factory(as_type)
 
+    # tuple types of the form tuple[int, str, ...] are not supported now
 
-@jsonify.register(Mapping)
-def _(value):
-    return {str(jsonify(key)): jsonify(val) for (key, val) in value.items()}
+    unjsonifiers = [unjsonify[type_] for type_ in arg_types]
 
+    def specialized(value):
+        if len(value) != len(arg_types):
+            raise_error(value, as_type)
 
-@unjsonify.register(Mapping)
-def _(value, as_type):
-    """
-    Unjsonify any Mapping type. Expects the input value to be
-    a JSON object (dict).
-    """
-
-    typecheck(value, dict, as_type)
-
-    arg_types = get_args(as_type)
-
-    if not arg_types:
-        return cast(value, as_type)
-    else:
-        unjsonify_key = unjsonify[arg_types[0]]
-        unjsonify_val = unjsonify[arg_types[1]]
-
-        as_dict = {
-            unjsonify_key(key): unjsonify_val(val)
-            for (key, val) in value.items()
-        }
-        return cast(as_dict, as_type)
-
-
-# Sequence
-
-
-@jsonify.register(Sequence)
-def jsonify_sequence(value):
-    return [jsonify(val) for val in value]
-
+        return as_type(
+            unjsonify_(item)
+            for (item, unjsonify_) in zip(value, unjsonifiers)
+        )
 
-@unjsonify.register(Sequence)
-def unjsonify_sequence(value, as_type):
-    typecheck(value, list, as_type)
+    return specialized
 
-    arg_types = get_args(as_type)
 
-    if not arg_types:
-        return cast(value, as_type)
-    else:
-        unjsonify_item = unjsonify[arg_types[0]]
-        return cast([unjsonify_item(item) for item in value], as_type)
-
-
-# Set
-
-
-@jsonify.register(Set)
-def _(value):
-    """
-    Set is not a sequence, so it needs it's own jsonifier.
-    Because the order of iterating over a set is not defined, the jsonification
-    tries to sort the set first, to make the results more predictable.
+@unjsonify.register_factory(tuple)
+def _(as_type):
     """
+    Unjsonify tuples. Handles several variants of tuples:
 
-    # if possible, sort the values first.
-    try:
-        value = sorted(value, key=lambda v: (type(v).__name__, v))
-    except Exception:
-        pass
-
-    return jsonify_sequence(value)
-
-
-unjsonify.register(Set)(unjsonify_sequence)
+    * plain old untyped tuple: tuple
+    * typed tuple: tuple[int, str, bool]
+    * n-ary monotyped tuple: tuple[T, ...]
+    * untyped namedtuple
+    * typing.NamedTuple
+    """
 
+    if hasattr(as_type, '__args__'):
+        return unjsonify_typed_factory(as_type)
 
-# ByteString abstract base class
+    annotations = inspect.get_annotations(as_type)
+    if annotations:
+        # typing.NamedTuple
 
+        def specialized_typed_namedtuple(value):
+            typecheck(value, (list, Sequence), as_type)
 
-@jsonify.register(ByteString)
-def _(value):
-    return base64.b64encode(value).decode("ascii")
+            if len(annotations) != len(value):
+                raise_error(value, as_type)
 
+            return as_type(*(
+                unjsonify[type_](val)
+                for (val, (_, type_)) in zip(value, annotations.items())
+            ))
 
-@unjsonify.register(ByteString)
-def _(value, as_type):
-    typecheck(value, str, as_type)
+        return specialized_typed_namedtuple
 
-    try:
-        return base64.b64decode(value.encode("ascii"))
-    except ValueError as exc:
-        detail = exc.args[0]
+    else:
+        # untyped tuple
+        def specialized_untyped(value):
+            if as_type is tuple:
+                # just plain tuple
+                return tuple(value)
+            else:
+                # namedtuple
+                return as_type(*value)
 
-    raise_error(value, as_type, detail)
+        return specialized_untyped
```

### Comparing `jsno-1.0.7/jsno/jsonify.py` & `jsno-1.1.0/jsno/jsonify.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import dataclasses
 import functools
+import typing
 
-from jsno.utils import is_optional, get_dataclass_fields
+from jsno.extra_data import get_extra_data_configuration
+from jsno.utils import is_optional
 from jsno.variant import get_variantfamily
 
 
 """
 valid JSON types.
 """
 JSON = bool | int | float | str | list["JSON"] | dict[str, "JSON"] | None
@@ -19,19 +21,29 @@
     value_type: type = type(value)
 
     if family := get_variantfamily(value_type):
         # if the value's class is a member of a variant family,
         # first add the variant label to the jsonified result
         result[family.label_name] = family.get_label(value_type)
 
-    for field in get_dataclass_fields(value_type):
+    extra_data_property = get_extra_data_configuration(value)
+
+    for field in dataclasses.fields(value_type):
         val = getattr(value, field.name)
 
         # skip optional values that are None
-        if val is not None or not is_optional(field.type):
+        if val is None:
+            # must cast the type to satisfy type checks
+            if is_optional(typing.cast(typing.Hashable, field.type)):
+                continue
+
+        if field.name == extra_data_property:
+            for (key, subval) in val.items():
+                result[key] = jsonify(subval)
+        else:
             result[field.name] = jsonify(val)
 
     return result
 
 
 def jsonify_list(value: list) -> list[JSON]:
     """
```

### Comparing `jsno-1.0.7/jsno/jsonize.py` & `jsno-1.1.0/jsno/jsonize.py`

 * *Files identical despite different names*

### Comparing `jsno-1.0.7/jsno/method.py` & `jsno-1.1.0/jsno/method.py`

 * *Files identical despite different names*

### Comparing `jsno-1.0.7/jsno/variant.py` & `jsno-1.1.0/jsno/variant.py`

 * *Files identical despite different names*

### Comparing `jsno-1.0.7/jsno.egg-info/PKG-INFO` & `jsno-1.1.0/jsno.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsno
-Version: 1.0.7
+Version: 1.1.0
 Summary: Convert Python data to and from json-compatible data structures
 License: MIT License
         
         Copyright (c) 2023 pek
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -31,14 +31,15 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # jsno
+
 Convert Python data to and from JSON-compatible data structures.
 
 Jsno provides functions that turn any Python values into JSON-compatible
 structures and back. The jsonified data can then be used wherever JSON
 data is required: it can be dumped into a file, sent over the network
 in an API call, or stored in a database that support JSON data.
 
@@ -183,20 +184,25 @@
 _variant family_.
 
 ### Other standard Python types
 
 * tuples
 * ranges
 * enums
-* date and datetime objects (converted to ISO-formatted strings)
+* date and, time and datetime objects (converted to ISO-formatted strings)
+* timedelta and timezone
 * complex
 * decimal.Decimal (converted to JSON strings)
 * pathlib.Path
+* re.Pattern
 * zoneinfo.ZoneInfo
 * Literal (only int and str literals)
+* NamedTuple
+* TypedDict
+* NewType
 
 ## Dumps and loads
 
 Jsno provides shortcut functions _dumps_ and _loads_ with interface that is
 similar to the standard _json_ module function.s _jsno.dumps_ both jsonifies its argument
 and turns it into a JSON-encoded string, similar to standard _json.dumps_
 function. Correspondinly, _jsno.loads_ both decodes and unjsonify JSON data.
@@ -255,14 +261,32 @@
 
 
 def load_game(database, identifier: str) -> GameState:
     json = database.load(identifier)
     return unjsonify[GameState](json)
 ```
 
+## Unjsonify context
+
+By default, the unjsonify raises an error (UjsonifyError), if the JSON object
+that is being converted to a dataclass contains extra keys. This is often the
+most appropriate behavior, for example when converting the request body of an API
+request, it's best to let the caller know that they might have mistyped property
+names in their data. However, sometimes, it's best to just ignore the extra properties,
+for example when reading persistent data that could have obsolete properties in it
+that are not reflected by the dataclass definition.
+
+The extra key behavior can be controlled by running the unjsonification inside
+the approproate _context_:
+
+```py
+with unjsonify.ignore_extra_keys:
+    state = unjsonify[GameState](data)
+```
+
 ## Constraints
 
 Jsno support annotating types with constraints that are boolean valued functions
 that must return True for the unjsonified value for it to be valid. For example,
 to only accept email addresses that contain the "@" character:
 
 ```py
@@ -272,23 +296,69 @@
 @dataclass
 class User:
     username: str
     email: Annotated[str, Constraint(lambda it: "@" in it)]
 
 ```
 
+Constraints are always used within Annotated, so there is a shortcut operator to
+make the definitions clearer. This is equivalent to the definition above:
+
+```py
+@dataclass
+class User:
+    username: str
+    email: str // Constraint(lambda it: "@" in it)
+
+```
+
+Using the `//`-operator, the type of the property is directly after the colon,
+not nested inside an Annotated-expression.
+
 The most typical constraints are those that limit the value or the length of a
 property to a certain range. For these, jsno provides predefined shortcuts:
 
-
 ```py
 @dataclass
 class Player:
-    username: Annotated[str, Constraint.len(min=4, max=16)]
-    credits: Annotated[int, Constraint.range(min=0)]
+    username: str // Constraint.len(min=4, max=16)
+    credits: int // Constraint.range(min=0)
+```
+
+There is also a constraint for matching the value with a regular expression:
+
+```py
+@dataclass
+class Variable:
+    name: str // Constraint.regex("[A-Za-z_][A-Za-z0-9_]*")
+```
+
+Constraints can be joined using the or-operator `|`:
+
+```py
+LiteralInt = Constraint.regex("[0-9]*")
+LiteralString = Constraint.regex('".*"')
+
+@dataclass
+class LiteralValue:
+    value: str // (LiteralInt | LiteralString)
+```
+
+## Anonymous record types
+
+Sometimes it's better to define substructures in complex data inline, without
+lifting them into named types. For this purpose, jsno provides "Record" type
+constructor, to conveniently define one-off dataclasses:
+
+```py
+@dataclass
+class User:
+    username: str
+    email: str
+    apikeys: list[Record(value=str, created_at=datetime)]
 ```
 
 ## Variant families
 
 Sometimes it's useful to have a hierarchy of classes, consisting of several subclasses
 that need to be stored in JSON. A typical example is defining the AST (abstract syntax
 tree) for a domain-specific language. Here's the AST of a simple expression language,
@@ -422,7 +492,34 @@
 Install jsno with pip:
 
 ```bash
 pip install jsno
 ```
 
 Jsno has no 3rd party dependencies.
+
+
+## Release Notes
+
+### Version 1.1.0 (2023-08-07)
+
+* regular expression constraints
+* operator // for constraints
+* joining constraints with | operator
+* anonymous Record types
+* support for datetime.timezone and datetime.timedelta
+* support for re.Pattern
+* support for TypedDict and NewType
+* support for untyped tuples and namedtuples
+* unjsonify context for ignoring extra properties
+* specifying target for extra properties in dataclasses
+* performance improvements for unjsonify
+
+### Version 1.0.7 (2023-08-04)
+
+* support for typing.Annotated
+* constraint annotations
+
+### Version 1.0.6 (2023-08-03)
+
+* support for datetime.time
+
```

### Comparing `jsno-1.0.7/jsno.egg-info/SOURCES.txt` & `jsno-1.1.0/jsno.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 LICENSE
 README.md
 pyproject.toml
 jsno/__init__.py
 jsno/abc.py
 jsno/constraint.py
+jsno/datetime.py
+jsno/extra_data.py
 jsno/jsonify.py
 jsno/jsonize.py
 jsno/method.py
+jsno/record.py
 jsno/standard.py
+jsno/tuple.py
+jsno/typeddict.py
 jsno/unjsonify.py
 jsno/utils.py
 jsno/variant.py
 jsno.egg-info/PKG-INFO
 jsno.egg-info/SOURCES.txt
 jsno.egg-info/dependency_links.txt
 jsno.egg-info/requires.txt
@@ -21,10 +26,13 @@
 tests/test_constraint.py
 tests/test_dataclasses.py
 tests/test_dates.py
 tests/test_dumps_and_loads.py
 tests/test_examples.py
 tests/test_jsonify.py
 tests/test_methods.py
+tests/test_record.py
 tests/test_standard.py
+tests/test_typeddict.py
 tests/test_unjsonify.py
+tests/test_utils.py
 tests/test_variant.py
```

### Comparing `jsno-1.0.7/pyproject.toml` & `jsno-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jsno"
-version = "1.0.7"
+version = "1.1.0"
 description = "Convert Python data to and from json-compatible data structures"
 readme = "README.md"
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `jsno-1.0.7/tests/test_ast_example.py` & `jsno-1.1.0/tests/test_ast_example.py`

 * *Files identical despite different names*

### Comparing `jsno-1.0.7/tests/test_constraint.py` & `jsno-1.1.0/tests/test_constraint.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,53 +12,97 @@
     assert unjsonify[PositiveInt](123) == 123
 
     with pytest.raises(UnjsonifyError):
         unjsonify[PositiveInt](0)
 
 
 def test_range():
-    Number = Annotated[int, Constraint.range(min=1, max=3)]
+    Number = int // Constraint.range(min=1, max=3)
 
     assert unjsonify[Number](1) == 1
 
     with pytest.raises(UnjsonifyError):
         unjsonify[Number](0)
 
 
 def test_len_range():
-    Identifier = Annotated[str, Constraint.len(min=16, max=16)]
+    Identifier = str // Constraint.len(min=16, max=16)
 
     assert unjsonify[Identifier]("1234567890abcdef") == "1234567890abcdef"
 
     with pytest.raises(UnjsonifyError):
         unjsonify[Identifier]("whaat")
 
 
 def test_len_min():
-    Identifier = Annotated[str, Constraint.len(min=16)]
+    Identifier = str // Constraint.len(min=16)
 
     assert unjsonify[Identifier]("1234567890abcdef") == "1234567890abcdef"
 
     with pytest.raises(UnjsonifyError):
         unjsonify[Identifier]("whaat")
 
 
 def test_len_max():
-    Identifier = Annotated[str, Constraint.len(max=3)]
+    Identifier = str // Constraint.len(max=3)
 
     assert unjsonify[Identifier]("123") == "123"
 
     with pytest.raises(UnjsonifyError):
         unjsonify[Identifier]("whaat")
 
 
+# defining this outside the type annotation as it confuses flake8
+EmailConstraint = Constraint(lambda it: "@" in it, "Valid email address")
+
+
 @dataclass
 class User:
     username: str
-    email: Annotated[str, Constraint(lambda it: "@" in it, "Valid email address")]
+    email: str // EmailConstraint
 
 
 def test_email_contraint():
     assert (
         unjsonify[User]({"username": "usr", "email": "user@domain.com"}) ==
         User("usr", "user@domain.com")
     )
+
+
+def test_regex():
+    Email = str // Constraint.regex(r"[\w\.]+@([\w-]+\.)+[\w-]{2,4}")
+
+    assert unjsonify[Email]("valid.email@example.com") == "valid.email@example.com"
+
+    with pytest.raises(UnjsonifyError):
+        unjsonify[Email]("valid.email@example@com")
+
+
+def test_double_constrait():
+    Aaaaa = str // Constraint.regex(r"[a]+") // Constraint.len(min=5)
+
+    assert unjsonify[Aaaaa]("aaaaa") == "aaaaa"
+
+    with pytest.raises(UnjsonifyError):
+        unjsonify[Aaaaa]("aaaaaaah")
+
+    with pytest.raises(UnjsonifyError):
+        unjsonify[Aaaaa]("aaa")
+
+
+LiteralInt = Constraint.regex("[0-9]*")
+LiteralString = Constraint.regex('".*"')
+
+
+@dataclass
+class LiteralValue:
+    value: str // (LiteralInt | LiteralString)
+
+
+def test_or_constraint():
+    assert(
+        unjsonify[list[LiteralValue]]([{"value": "123"}, {"value": '"xxx"'}]) ==
+        [LiteralValue("123"), LiteralValue('"xxx"')]
+    )
+
+    with pytest.raises(UnjsonifyError):
+        unjsonify[list[LiteralValue]]([{"value": "foo"}])
```

### Comparing `jsno-1.0.7/tests/test_dataclasses.py` & `jsno-1.1.0/tests/test_dataclasses.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import dataclasses
 import enum
 import pytest
 
 from typing import Any, Dict, List
 
-from jsno import jsonify, unjsonify, jsonify_with_method, UnjsonifyError
+from jsno import extra_data, jsonify, unjsonify, jsonify_with_method, UnjsonifyError
 
 
 class Color(enum.Enum):
     Red = 1
     Green = 2
     Blue = 3
 
@@ -139,35 +139,46 @@
     email = unjsonify[EmailAddress]("foobar@example.com")
 
     assert email == EmailAddress(user="foobar", domain="example.com")
 
 
 def test_ujsonify_with_missing_properties_error():
     with pytest.raises(UnjsonifyError):
-        unjsonify[Brick]({"color": "Yellow"})
+        unjsonify[Brick]({"color": "Red"})
 
 
 def test_ujsonify_with_not_dict_error():
     with pytest.raises(UnjsonifyError):
         unjsonify[Brick]("Something else")
 
 
 def test_unjsonify_dataclass_error():
     with pytest.raises(UnjsonifyError):
-        unjsonify[Box]({})
+        unjsonify[Brick]({})
+
+
+def test_unjsonify_dataclass_extra_key_error():
+    with pytest.raises(UnjsonifyError):
+        unjsonify[Brick]({"color": "Red", "width": 1, "height": 1, "matrial": "xxx"})
+
+
+def test_unjsonify_dataclass_extra_key_ignore():
+    with unjsonify.ignore_extra_keys():
+        brick = unjsonify[Brick]({"color": "Red", "width": 1, "height": 1, "matrial": "xxx"})
+        assert brick == Brick(color=Color.Red, width=1, height=1)
 
 
 @dataclasses.dataclass
 class User:
     username: str
     password: str = 'pAssW0rd'
     metadata: List[Dict[str, Any]] = dataclasses.field(default_factory=list)
 
 
-def test_jsonifty_dataclass_with_default_value():
+def test_jsonify_dataclass_with_default_value():
     assert (
         jsonify(User(username="usr")) ==
         {"username": "usr", "password": "pAssW0rd", "metadata": []}
     )
 
     assert (
         jsonify(User(username="usr", password="", metadata=[{"key": 100}])) ==
@@ -180,7 +191,41 @@
 
     assert user == User(username="usr")
     assert user.password == "pAssW0rd"
 
     user = unjsonify[User]({"username": "usr", "password": "", "metadata": [{"key": 100}]})
 
     assert user == User(username="usr", password="", metadata=[{"key": 100}])
+
+
+@dataclasses.dataclass
+@extra_data(property="metadata")
+class MetaUser:
+    username: str
+    metadata: dict
+
+
+def test_jsonify_dataclass_with_extra_data_property():
+    assert (
+        jsonify(MetaUser(username="usr", metadata={"tags": ["yes"]})) ==
+        {"username": "usr", "tags": ["yes"]}
+    )
+
+
+def test_unjsonify_dataclass_with_extra_data_property():
+    assert (
+        unjsonify[MetaUser]({"username": "usr", "tags": ["yes"]}) ==
+        MetaUser(username="usr", metadata={"tags": ["yes"]})
+    )
+
+
+@dataclasses.dataclass
+@extra_data(ignore=True)
+class Config:
+    username: str
+
+
+def test_unjsonify_dataclass_with_ignore_extra_data():
+    assert (
+        unjsonify[Config]({"username": "usr", "tags": ["yes"]}) ==
+        Config(username="usr")
+    )
```

### Comparing `jsno-1.0.7/tests/test_examples.py` & `jsno-1.1.0/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `jsno-1.0.7/tests/test_jsonify.py` & `jsno-1.1.0/tests/test_jsonify.py`

 * *Files 8% similar despite different names*

```diff
@@ -115,7 +115,14 @@
 
 def test_unjsonify_float_subclass():
 
     class SpecialFloat(float):
         pass
 
     assert jsonify(SpecialFloat(123.4)) == 123.4
+
+
+def test_namedtuple():
+    LogEntry = collections.namedtuple("LogEntry", ["date", "message"])
+
+    entry = LogEntry(date=datetime.date(2023, 8, 5), message="ok")
+    assert jsonify(entry) == ["2023-08-05", "ok"]
```

### Comparing `jsno-1.0.7/tests/test_methods.py` & `jsno-1.1.0/tests/test_methods.py`

 * *Files identical despite different names*

### Comparing `jsno-1.0.7/tests/test_standard.py` & `jsno-1.1.0/tests/test_standard.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import decimal
 import pathlib
+import re
 import zoneinfo
 
 import pytest
 
 from jsno import jsonify, unjsonify, UnjsonifyError, jsonify_as_string
 
 
@@ -66,7 +67,15 @@
     run_tests(range(100), {"start": 0, "stop": 100})
     run_tests(range(10, 0, -1), {"start": 10, "stop": 0, "step": -1})
 
 
 def test_jsonify_range_failure():
     with pytest.raises(UnjsonifyError):
         unjsonify[range]({"start": 1, "stop": 6, "step": 0})
+
+
+def test_jsonify_re_pattern():
+    assert jsonify(re.compile("[a-z]+")) == "[a-z]+"
+
+
+def test_unjsonify_re_pattern():
+    assert unjsonify[re.Pattern]("[a-z]+") == re.compile("[a-z]+")
```

### Comparing `jsno-1.0.7/tests/test_unjsonify.py` & `jsno-1.1.0/tests/test_unjsonify.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import collections
 import datetime
 import pytest
 import zoneinfo
 
-from typing import Annotated, Any, Callable, Optional, List, Literal
+from typing import Annotated, Any, Callable, Optional, List, Literal, NewType
 
 from jsno.unjsonify import unjsonify, UnjsonifyError
 
 
 helsinki = zoneinfo.ZoneInfo("Europe/Helsinki")
 utc = zoneinfo.ZoneInfo("UTC")
 
@@ -43,15 +43,15 @@
     assert counter == {"x": 12, "y": 33}
 
 
 def test_unjsonify_list():
     assert unjsonify[list]([1, 2, 3]) == [1, 2, 3]
 
 
-def test_unjsonify_typed_dict():
+def test_unjsonify_dict_with_types():
     assert unjsonify[dict[str, int]]({'x': 1, 'y': 2}) == {'x': 1, 'y': 2}
 
 
 def test_unjsonify_list_of_floats():
     assert unjsonify[list[float]]([1.0, 2.0, 3.0, 0, -2]) == [1, 2, 3.0, 0, -2]
 
 
@@ -72,17 +72,38 @@
         unjsonify[list[bool]]([True, 120])
 
 
 def test_unjsonify_n_ary_tuple():
     assert unjsonify[tuple[float, ...]]([1.0, 2.0, 3.0]) == (1, 2, 3.0)
 
 
+def test_unjsonify_untyped_tuple():
+    assert unjsonify[tuple]([True, None]) == (True, None)
+
+
+def test_unjsonify_untyped_empty_tuple():
+    assert unjsonify[tuple]([]) == ()
+
+
 def test_unjsonify_empty_tuple():
     assert unjsonify[tuple[()]]([]) == ()
 
+    with pytest.raises(UnjsonifyError):
+        unjsonify[tuple[()]]([123])
+
+
+def test_ujsonify_namedtuple():
+    LogEntry = collections.namedtuple("LogEntry", ["date", "message"])
+
+    entry = LogEntry(date="2023-08-05", message="ok")
+    assert unjsonify[LogEntry](["2023-08-05", "ok"]) == entry
+
+    with pytest.raises(UnjsonifyError):
+        unjsonify[tuple[LogEntry]](["2023-08-05", "ok", "more"])
+
 
 def test_unjsonify_malformed_type_error():
     with pytest.raises(UnjsonifyError):
         unjsonify[tuple[bool, str, ...]]([True, "x"])
 
 
 def test_unjsonify_multiple_typearg_tuple():
@@ -174,10 +195,11 @@
 
 
 def test_unjsonify_not_defined():
     with pytest.raises(TypeError):
         unjsonify[Callable]("call")
 
 
-def test_unjsonify_date_failure():
-    with pytest.raises(TypeError):
-        unjsonify[datetime.date]("today")
+def test_newtype():
+    Point = NewType("Point", tuple[float, float])
+
+    assert unjsonify[Point]([1.2, 3.4]) == (1.2, 3.4)
```

### Comparing `jsno-1.0.7/tests/test_variant.py` & `jsno-1.1.0/tests/test_variant.py`

 * *Files identical despite different names*

