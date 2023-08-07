# Comparing `tmp/serious-1.2.2.tar.gz` & `tmp/serious-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serious-1.2.2.tar", last modified: Tue Mar 14 19:25:07 2023, max compression
+gzip compressed data, was "serious-1.2.5.tar", last modified: Mon Aug  7 16:21:30 2023, max compression
```

## Comparing `serious-1.2.2.tar` & `serious-1.2.5.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-14 19:25:07.470487 serious-1.2.2/
--rw-r--r--   0 vsts      (1001) docker     (123)     1069 2023-03-14 19:24:43.000000 serious-1.2.2/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (123)     8314 2023-03-14 19:25:07.470487 serious-1.2.2/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     5701 2023-03-14 19:24:43.000000 serious-1.2.2/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-14 19:25:07.466487 serious-1.2.2/serious/
--rw-r--r--   0 vsts      (1001) docker     (123)      773 2023-03-14 19:24:43.000000 serious-1.2.2/serious/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      389 2023-03-14 19:24:43.000000 serious-1.2.2/serious/checks.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7500 2023-03-14 19:24:43.000000 serious-1.2.2/serious/descriptors.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-14 19:25:07.466487 serious-1.2.2/serious/dict/
--rw-r--r--   0 vsts      (1001) docker     (123)      159 2023-03-14 19:24:43.000000 serious-1.2.2/serious/dict/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4052 2023-03-14 19:24:43.000000 serious-1.2.2/serious/dict/model.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6216 2023-03-14 19:24:43.000000 serious-1.2.2/serious/errors.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-14 19:25:07.466487 serious-1.2.2/serious/json/
--rw-r--r--   0 vsts      (1001) docker     (123)      131 2023-03-14 19:24:43.000000 serious-1.2.2/serious/json/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1443 2023-03-14 19:24:43.000000 serious-1.2.2/serious/json/checks.py
--rw-r--r--   0 vsts      (1001) docker     (123)      235 2023-03-14 19:24:43.000000 serious-1.2.2/serious/json/errors.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5702 2023-03-14 19:24:43.000000 serious-1.2.2/serious/json/model.py
--rw-r--r--   0 vsts      (1001) docker     (123)      558 2023-03-14 19:24:43.000000 serious-1.2.2/serious/json/utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-14 19:25:07.470487 serious-1.2.2/serious/serialization/
--rw-r--r--   0 vsts      (1001) docker     (123)     1416 2023-03-14 19:24:43.000000 serious-1.2.2/serious/serialization/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1411 2023-03-14 19:24:43.000000 serious-1.2.2/serious/serialization/check_immutable.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2950 2023-03-14 19:24:43.000000 serious-1.2.2/serious/serialization/context.py
--rw-r--r--   0 vsts      (1001) docker     (123)    24503 2023-03-14 19:24:43.000000 serious-1.2.2/serious/serialization/field_serializers.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1229 2023-03-14 19:24:43.000000 serious-1.2.2/serious/serialization/key_mapper.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9493 2023-03-14 19:24:43.000000 serious-1.2.2/serious/serialization/model.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1844 2023-03-14 19:24:43.000000 serious-1.2.2/serious/serialization/serializer.py
--rw-r--r--   0 vsts      (1001) docker     (123)      790 2023-03-14 19:24:43.000000 serious-1.2.2/serious/test_utils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6969 2023-03-14 19:24:43.000000 serious-1.2.2/serious/types.py
--rw-r--r--   0 vsts      (1001) docker     (123)      294 2023-03-14 19:24:43.000000 serious-1.2.2/serious/utils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1617 2023-03-14 19:24:43.000000 serious-1.2.2/serious/validation.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-14 19:25:07.466487 serious-1.2.2/serious.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)     8314 2023-03-14 19:25:07.000000 serious-1.2.2/serious.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      753 2023-03-14 19:25:07.000000 serious-1.2.2/serious.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-03-14 19:25:07.000000 serious-1.2.2/serious.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-03-14 19:25:07.000000 serious-1.2.2/serious.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)        8 2023-03-14 19:25:07.000000 serious-1.2.2/serious.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-03-14 19:25:07.470487 serious-1.2.2/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1572 2023-03-14 19:24:43.000000 serious-1.2.2/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-07 16:21:30.883362 serious-1.2.5/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1069 2023-08-07 16:21:06.000000 serious-1.2.5/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (123)     6866 2023-08-07 16:21:30.883362 serious-1.2.5/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     5701 2023-08-07 16:21:06.000000 serious-1.2.5/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-07 16:21:30.883362 serious-1.2.5/serious/
+-rw-r--r--   0 vsts      (1001) docker     (123)      773 2023-08-07 16:21:06.000000 serious-1.2.5/serious/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      389 2023-08-07 16:21:06.000000 serious-1.2.5/serious/checks.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7650 2023-08-07 16:21:06.000000 serious-1.2.5/serious/descriptors.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-07 16:21:30.883362 serious-1.2.5/serious/dict/
+-rw-r--r--   0 vsts      (1001) docker     (123)      159 2023-08-07 16:21:06.000000 serious-1.2.5/serious/dict/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4052 2023-08-07 16:21:06.000000 serious-1.2.5/serious/dict/model.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6216 2023-08-07 16:21:06.000000 serious-1.2.5/serious/errors.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-07 16:21:30.883362 serious-1.2.5/serious/json/
+-rw-r--r--   0 vsts      (1001) docker     (123)      131 2023-08-07 16:21:06.000000 serious-1.2.5/serious/json/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1443 2023-08-07 16:21:06.000000 serious-1.2.5/serious/json/checks.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      235 2023-08-07 16:21:06.000000 serious-1.2.5/serious/json/errors.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5702 2023-08-07 16:21:06.000000 serious-1.2.5/serious/json/model.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      558 2023-08-07 16:21:06.000000 serious-1.2.5/serious/json/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-08-07 16:21:06.000000 serious-1.2.5/serious/py.typed
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-07 16:21:30.883362 serious-1.2.5/serious/serialization/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1416 2023-08-07 16:21:06.000000 serious-1.2.5/serious/serialization/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1411 2023-08-07 16:21:06.000000 serious-1.2.5/serious/serialization/check_immutable.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3052 2023-08-07 16:21:06.000000 serious-1.2.5/serious/serialization/context.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    24540 2023-08-07 16:21:06.000000 serious-1.2.5/serious/serialization/field_serializers.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1229 2023-08-07 16:21:06.000000 serious-1.2.5/serious/serialization/key_mapper.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9493 2023-08-07 16:21:06.000000 serious-1.2.5/serious/serialization/model.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1844 2023-08-07 16:21:06.000000 serious-1.2.5/serious/serialization/serializer.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      790 2023-08-07 16:21:06.000000 serious-1.2.5/serious/test_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6969 2023-08-07 16:21:06.000000 serious-1.2.5/serious/types.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      294 2023-08-07 16:21:06.000000 serious-1.2.5/serious/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1617 2023-08-07 16:21:06.000000 serious-1.2.5/serious/validation.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-07 16:21:30.883362 serious-1.2.5/serious.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     6866 2023-08-07 16:21:30.000000 serious-1.2.5/serious.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      770 2023-08-07 16:21:30.000000 serious-1.2.5/serious.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-08-07 16:21:30.000000 serious-1.2.5/serious.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-08-07 16:21:30.000000 serious-1.2.5/serious.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)        8 2023-08-07 16:21:30.000000 serious-1.2.5/serious.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-08-07 16:21:30.883362 serious-1.2.5/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1573 2023-08-07 16:21:06.000000 serious-1.2.5/setup.py
```

### Comparing `serious-1.2.2/LICENSE` & `serious-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `serious-1.2.2/PKG-INFO` & `serious-1.2.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,210 +1,210 @@
 Metadata-Version: 2.1
 Name: serious
-Version: 1.2.2
+Version: 1.2.5
 Summary: Easily serialize dataclasses to and from JSON
 Home-page: https://github.com/mdrachuk/serious
 Author: mdrachuk
 Author-email: misha@drach.uk
 License: MIT
 Project-URL: Pipelines, https://dev.azure.com/misha-drachuk/serious
 Project-URL: Source, https://github.com/mdrachuk/serious/
 Project-URL: Issues, https://github.com/mdrachuk/serious/issues
-Description: # serious
-        [![PyPI](https://img.shields.io/pypi/v/serious)][pypi]
-        [![Build Status](https://img.shields.io/azure-devops/build/misha-drachuk/serious/2)](https://dev.azure.com/misha-drachuk/serious/_build/latest?definitionId=1&branchName=master)
-        [![Test Coverage](https://img.shields.io/coveralls/github/mdrachuk/serious/master)](https://coveralls.io/github/mdrachuk/serious)
-        [![Supported Python](https://img.shields.io/pypi/pyversions/serious)][pypi]
-        [![Documentation](https://img.shields.io/readthedocs/serious)][docs]
-        
-        A dataclass model toolkit: serialization, validation, and more.
-        
-        [Documentation][docs]
-        
-        
-        ## Features
-        - Model definitions in pure Python.
-        - Validation showing up in code coverage.
-        - Type annotations for all public-facing APIs.
-        - (Optionally) ensures immutability.
-        - Easily extensible.
-        - Made for people.
-        - Documented rigorously.
-        
-        ## Basics
-        ### Installation
-        Available from [PyPI][pypi]:
-        ```shell
-        pip install serious
-        ```
-        
-        ### Quick Example
-        
-        Central part of Serious API are different [Models][doc-models].
-        
-        Given a regular dataclass:
-        ```python
-        from dataclasses import dataclass
-        
-        @dataclass
-        class Person:
-            name: str
-        ```
-        
-        Let’s create a `JsonModel`:  
-        ```python
-        from serious.json import JsonModel
-            
-        model = JsonModel(Person)
-        ```
-        
-        And use its [dump/load methods][doc-serialization]:
-        ```python
-        person = Person('Albert Einstein')
-        
-        model.dump(person) # {"name": "Albert Einstein"}
-        ```
-        
-        ### Validation
-        To add validation to the example above all we need is to add `__validate__` method to person:
-        ```python
-        from dataclasses import dataclass
-        from typing import Optional
-        from serious import ValidationError, Email
-        
-        @dataclass
-        class Person:
-            name: str
-            email: Optional[Email]
-            phone: Optional[str]
-        
-            def __validate__(self):
-                if len(self.name) == 0:
-                    raise ValidationError('Every person needs a name')
-                if self.phone is None and self.email is None:
-                    raise ValidationError('At least some contact should be present')
-        ```
-        
-        [More on validation.][doc-validation]
-        
-        
-        ### Supported formats:
-        - [x] [JSON][doc-json-model]
-        - [x] [Python Dictionaries][doc-dict-model]
-        - [ ] YAML
-        - [ ] Form data
-        
-        
-        ### Supported field types
-        [More in docs.][doc-types]
-        
-        - Other dataclasses
-        - Primitives: `str`, `int`, `float`, `bool`
-        - Dictionaries: only with string keys: `Dict[str, Any]`  
-        - Lists, [sets][set], [deques][deque]: python collections of any serializable type
-        - [Tuples][tuple] both with and without ellipsis:
-            - tuples as set of independent elements (e.g. `Tuple[str, int, date]`) 
-            - with ellipses, acting as a frozen list (`Tuple[str, ...]`)
-        - [Enumerations][enum] by value:
-            - of primitives (e.g. `OperatingSystem(Enum)`) 
-            - typed enums (`Color(str, Enum)` and `FilePermission(IntFlag)`)
-        - [Decimal][decimal]: encoded to JSON as string 
-        - [Datetime][datetime], [date][date] and [time][time]: encoded to the [ISO 8601][iso8601] formatted string
-        - [UUID][uuid]
-        - `serious.types.Timestamp`: a UTC timestamp since [UNIX epoch][epoch] as float ms value 
-        - `serious.types.Email`: a string Tiny Type that supports validation and contains additional properties 
-        - custom immutable alternatives to native python types in `serious.types`: `FrozenList`, `FrozenDict`
-        
-        ## A bigger example
-        
-        ```python
-        from dataclasses import dataclass
-        from serious import JsonModel, ValidationError
-        from typing import List
-        from enum import Enum
-        
-        class Specialty(Enum):
-            Worker = 1
-            Fool = 2
-        
-        
-        @dataclass(frozen=True)
-        class Minion:
-            name: str
-            type: Specialty
-        
-        
-        @dataclass(frozen=True)
-        class Boss:
-            name: str
-            minions: List[Minion]
-            
-            def __validate__(self):
-                if len(self.minions) < 2:
-                    raise ValidationError('What kind of boss are you?')
-        
-        
-        boss = Boss("me", [Minion('evil minion', Specialty.Fool), Minion('very evil minion', Specialty.Worker)])
-        boss_json = """{
-            "name": "me",
-            "minions": [
-                {
-                    "name": "evil minion",
-                    "type": "Fool"
-                },
-                {
-                    "name": "very evil minion",
-                    "type": "Worker"
-                }
-            ]
-        }"""
-        
-        model = JsonModel(Boss, indent=4)
-        
-        assert model.dump(boss) == boss_json
-        assert model.load(boss_json) == boss
-        ```
-        
-        
-        ## Acknowledgements
-        Initially, a fork of [@lidatong/dataclasses-json](https://github.com/lidatong/dataclasses-json).
-        
-        [pypi]: https://pypi.org/project/serious/
-        [dataclass]: https://docs.python.org/3/library/dataclasses.html
-        [iso8601]: https://en.wikipedia.org/wiki/ISO_8601
-        [epoch]: https://en.wikipedia.org/wiki/Unix_time
-        [enum]: https://docs.python.org/3/library/enum.html
-        [decimal]: https://docs.python.org/3/library/decimal.html
-        [tuple]: https://docs.python.org/3/library/stdtypes.html#tuple
-        [list]: https://docs.python.org/3/library/stdtypes.html#list
-        [set]: https://docs.python.org/3/library/stdtypes.html#set
-        [deque]: https://docs.python.org/3.7/library/collections.html#collections.deque
-        [datetime]: https://docs.python.org/3.7/library/datetime.html#datetime.datetime
-        [date]: https://docs.python.org/3.7/library/datetime.html#datetime.date
-        [time]: https://docs.python.org/3.7/library/datetime.html#datetime.time
-        [uuid]: https://docs.python.org/3.7/library/uuid.html?highlight=uuid#uuid.UUID
-        [doc-types]: https://serious.readthedocs.io/en/latest/types/
-        [doc-models]: https://serious.readthedocs.io/en/latest/models/
-        [doc-json-model]: https://serious.readthedocs.io/en/latest/models/#jsonmodel
-        [doc-dict-model]: https://serious.readthedocs.io/en/latest/models/#dictmodel
-        [doc-serialization]: https://serious.readthedocs.io/en/latest/serialization/ (Serialization documentation)
-        [doc-validation]: https://serious.readthedocs.io/en/latest/validation/ (Validation documentation)
-        [docs]: https://serious.readthedocs.io/en/latest/ 
-        
 Keywords: dataclasses json serialization
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: POSIX :: BSD
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# serious
+[![PyPI](https://img.shields.io/pypi/v/serious)][pypi]
+[![Build Status](https://img.shields.io/azure-devops/build/misha-drachuk/serious/2)](https://dev.azure.com/misha-drachuk/serious/_build/latest?definitionId=1&branchName=master)
+[![Test Coverage](https://img.shields.io/coveralls/github/mdrachuk/serious/master)](https://coveralls.io/github/mdrachuk/serious)
+[![Supported Python](https://img.shields.io/pypi/pyversions/serious)][pypi]
+[![Documentation](https://img.shields.io/readthedocs/serious)][docs]
+
+A dataclass model toolkit: serialization, validation, and more.
+
+[Documentation][docs]
+
+
+## Features
+- Model definitions in pure Python.
+- Validation showing up in code coverage.
+- Type annotations for all public-facing APIs.
+- (Optionally) ensures immutability.
+- Easily extensible.
+- Made for people.
+- Documented rigorously.
+
+## Basics
+### Installation
+Available from [PyPI][pypi]:
+```shell
+pip install serious
+```
+
+### Quick Example
+
+Central part of Serious API are different [Models][doc-models].
+
+Given a regular dataclass:
+```python
+from dataclasses import dataclass
+
+@dataclass
+class Person:
+    name: str
+```
+
+Let’s create a `JsonModel`:  
+```python
+from serious.json import JsonModel
+    
+model = JsonModel(Person)
+```
+
+And use its [dump/load methods][doc-serialization]:
+```python
+person = Person('Albert Einstein')
+
+model.dump(person) # {"name": "Albert Einstein"}
+```
+
+### Validation
+To add validation to the example above all we need is to add `__validate__` method to person:
+```python
+from dataclasses import dataclass
+from typing import Optional
+from serious import ValidationError, Email
+
+@dataclass
+class Person:
+    name: str
+    email: Optional[Email]
+    phone: Optional[str]
+
+    def __validate__(self):
+        if len(self.name) == 0:
+            raise ValidationError('Every person needs a name')
+        if self.phone is None and self.email is None:
+            raise ValidationError('At least some contact should be present')
+```
+
+[More on validation.][doc-validation]
+
+
+### Supported formats:
+- [x] [JSON][doc-json-model]
+- [x] [Python Dictionaries][doc-dict-model]
+- [ ] YAML
+- [ ] Form data
+
+
+### Supported field types
+[More in docs.][doc-types]
+
+- Other dataclasses
+- Primitives: `str`, `int`, `float`, `bool`
+- Dictionaries: only with string keys: `Dict[str, Any]`  
+- Lists, [sets][set], [deques][deque]: python collections of any serializable type
+- [Tuples][tuple] both with and without ellipsis:
+    - tuples as set of independent elements (e.g. `Tuple[str, int, date]`) 
+    - with ellipses, acting as a frozen list (`Tuple[str, ...]`)
+- [Enumerations][enum] by value:
+    - of primitives (e.g. `OperatingSystem(Enum)`) 
+    - typed enums (`Color(str, Enum)` and `FilePermission(IntFlag)`)
+- [Decimal][decimal]: encoded to JSON as string 
+- [Datetime][datetime], [date][date] and [time][time]: encoded to the [ISO 8601][iso8601] formatted string
+- [UUID][uuid]
+- `serious.types.Timestamp`: a UTC timestamp since [UNIX epoch][epoch] as float ms value 
+- `serious.types.Email`: a string Tiny Type that supports validation and contains additional properties 
+- custom immutable alternatives to native python types in `serious.types`: `FrozenList`, `FrozenDict`
+
+## A bigger example
+
+```python
+from dataclasses import dataclass
+from serious import JsonModel, ValidationError
+from typing import List
+from enum import Enum
+
+class Specialty(Enum):
+    Worker = 1
+    Fool = 2
+
+
+@dataclass(frozen=True)
+class Minion:
+    name: str
+    type: Specialty
+
+
+@dataclass(frozen=True)
+class Boss:
+    name: str
+    minions: List[Minion]
+    
+    def __validate__(self):
+        if len(self.minions) < 2:
+            raise ValidationError('What kind of boss are you?')
+
+
+boss = Boss("me", [Minion('evil minion', Specialty.Fool), Minion('very evil minion', Specialty.Worker)])
+boss_json = """{
+    "name": "me",
+    "minions": [
+        {
+            "name": "evil minion",
+            "type": "Fool"
+        },
+        {
+            "name": "very evil minion",
+            "type": "Worker"
+        }
+    ]
+}"""
+
+model = JsonModel(Boss, indent=4)
+
+assert model.dump(boss) == boss_json
+assert model.load(boss_json) == boss
+```
+
+
+## Acknowledgements
+Initially, a fork of [@lidatong/dataclasses-json](https://github.com/lidatong/dataclasses-json).
+
+[pypi]: https://pypi.org/project/serious/
+[dataclass]: https://docs.python.org/3/library/dataclasses.html
+[iso8601]: https://en.wikipedia.org/wiki/ISO_8601
+[epoch]: https://en.wikipedia.org/wiki/Unix_time
+[enum]: https://docs.python.org/3/library/enum.html
+[decimal]: https://docs.python.org/3/library/decimal.html
+[tuple]: https://docs.python.org/3/library/stdtypes.html#tuple
+[list]: https://docs.python.org/3/library/stdtypes.html#list
+[set]: https://docs.python.org/3/library/stdtypes.html#set
+[deque]: https://docs.python.org/3.7/library/collections.html#collections.deque
+[datetime]: https://docs.python.org/3.7/library/datetime.html#datetime.datetime
+[date]: https://docs.python.org/3.7/library/datetime.html#datetime.date
+[time]: https://docs.python.org/3.7/library/datetime.html#datetime.time
+[uuid]: https://docs.python.org/3.7/library/uuid.html?highlight=uuid#uuid.UUID
+[doc-types]: https://serious.readthedocs.io/en/latest/types/
+[doc-models]: https://serious.readthedocs.io/en/latest/models/
+[doc-json-model]: https://serious.readthedocs.io/en/latest/models/#jsonmodel
+[doc-dict-model]: https://serious.readthedocs.io/en/latest/models/#dictmodel
+[doc-serialization]: https://serious.readthedocs.io/en/latest/serialization/ (Serialization documentation)
+[doc-validation]: https://serious.readthedocs.io/en/latest/validation/ (Validation documentation)
+[docs]: https://serious.readthedocs.io/en/latest/
```

### Comparing `serious-1.2.2/README.md` & `serious-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `serious-1.2.2/serious/__init__.py` & `serious-1.2.5/serious/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,8 +16,8 @@
 
 from .dict import DictModel
 from .errors import ModelError, ValidationError, LoadError, DumpError
 from .json import JsonModel
 from .types import Timestamp, Email, FrozenList, FrozenDict
 from .validation import validate
 
-__version__ = '1.2.2'
+__version__ = '1.2.5'
```

### Comparing `serious-1.2.2/serious/descriptors.py` & `serious-1.2.5/serious/descriptors.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 The data is carried by `TypeDescriptor`s which are created by a call to `serious.descriptors.describe(cls)`.
 """
 from __future__ import annotations
 
 __all__ = ['TypeDescriptor', 'describe', 'DescTypes', 'scan_types']
 
 from dataclasses import dataclass, fields, is_dataclass
-from typing import Type, Any, TypeVar, get_type_hints, Dict, Mapping, List, Union, Iterable, Optional
+from types import UnionType
+from typing import Type, Any, TypeVar, get_type_hints, Dict, Mapping, List, Union, Iterable, Optional, cast
 
 from .types import FrozenDict, FrozenList
 
 T = TypeVar('T')
 
 GenericParams = Mapping[Any, 'TypeDescriptor']
 
@@ -101,15 +102,17 @@
     **Examples**:
      - `Tuple[str]` -> `<TypeDescriptor cls=tuple params={0: <TypeDescriptor cls=str>}>`;
      - `Optional[int]` -> `<TypeDescriptor cls=int is_optional=True>`.
     """
     params: GenericParams = {}
     is_optional = _is_optional(cls)
     if is_optional:
-        cls = cls.__args__[0]
+        _args = set(cls.__args__)
+        _args.remove(type(None))
+        cls = cast(Type, Union[tuple(_args)])
 
     try:
         is_typed_dict = issubclass(cls, dict) and bool(getattr(cls, '__annotations__', None))
     except TypeError:
         is_typed_dict = False
 
     if hasattr(cls, '__orig_bases__') and is_dataclass(cls):
@@ -194,10 +197,10 @@
 
     `DescTypes` allow checks of the descriptor tree."""
     return DescTypes.scan(desc, known=[])
 
 
 def _is_optional(cls: Type) -> bool:
     """Returns True if the provided type is `Optional`."""
-    return getattr(cls, '__origin__', None) == Union \
-        and len(cls.__args__) == 2 \
-        and cls.__args__[1] == type(None)
+    return (getattr(cls, '__origin__', None) == Union or isinstance(cls, UnionType)) \
+        and len(cls.__args__) > 1 \
+        and type(None) in set(cls.__args__)
```

### Comparing `serious-1.2.2/serious/dict/model.py` & `serious-1.2.5/serious/dict/model.py`

 * *Files identical despite different names*

### Comparing `serious-1.2.2/serious/errors.py` & `serious-1.2.5/serious/errors.py`

 * *Files identical despite different names*

### Comparing `serious-1.2.2/serious/json/checks.py` & `serious-1.2.5/serious/json/checks.py`

 * *Files identical despite different names*

### Comparing `serious-1.2.2/serious/json/model.py` & `serious-1.2.5/serious/json/model.py`

 * *Files identical despite different names*

### Comparing `serious-1.2.2/serious/json/utils.py` & `serious-1.2.5/serious/json/utils.py`

 * *Files identical despite different names*

### Comparing `serious-1.2.2/serious/serialization/__init__.py` & `serious-1.2.5/serious/serialization/__init__.py`

 * *Files identical despite different names*

### Comparing `serious-1.2.2/serious/serialization/check_immutable.py` & `serious-1.2.5/serious/serialization/check_immutable.py`

 * *Files identical despite different names*

### Comparing `serious-1.2.2/serious/serialization/context.py` & `serious-1.2.5/serious/serialization/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,17 @@
         self._steps.pop()
 
     @property
     def stack(self) -> FrozenList[SerializationStep]:
         """The stack is included in errors, mentioning the fields, array indexes, dictionary keys, etc."""
         return FrozenList(self._steps)
 
+    def __repr__(self):
+        return f"<Context: {'.'.join([step.name for step in self._steps])}>"
+
     @abstractmethod
     def run(self, step: str, serializer: Serializer, value: Any) -> Any:
         """Execute serializer in context.
 
         Implementations:
         - includes the current step in the stack,
         - executes current steps serializer,
```

### Comparing `serious-1.2.2/serious/serialization/field_serializers.py` & `serious-1.2.5/serious/serialization/field_serializers.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 ]
 
 import re
 from dataclasses import replace
 from datetime import datetime, date, time
 from decimal import Decimal
 from enum import Enum
-from typing import Any, Optional, Dict, List, Union, Pattern, Iterable, Type, Tuple, Literal
+from typing import Any, Optional, Dict, List, Union, Pattern, Iterable, Type, Tuple, Literal, TypeVar
 from uuid import UUID
 
 from serious.descriptors import TypeDescriptor
 from serious.errors import ValidationError
 from serious.types import Timestamp, FrozenList, FrozenDict
 from .context import Context, Loading, Dumping
 from .serializer import FieldSerializer, Serializer
@@ -382,21 +382,24 @@
     def load(self, value: Any, ctx: Loading) -> Any:
         return self._serializer.load(value, ctx)
 
     def dump(self, value: Any, ctx: Dumping) -> Any:
         return self._serializer.dump(value, ctx)
 
 
+S = TypeVar("S", bound=Serializer)
+
+
 class OrdinalAlias(Serializer[Any, Any]):
     """Serializes values using the provided serializer at the currently set index.
     The index is set via calling instance as a function.
     Step name is changed to match the index.
     """
 
-    def __init__(self, serializers: List[Serializer]):
+    def __init__(self, serializers: List[S]):
         self._serializers = serializers
 
     def __call__(self, index: int) -> OrdinalAlias:
         self._index = index
         return self
 
     def step_name(self) -> str:
```

### Comparing `serious-1.2.2/serious/serialization/key_mapper.py` & `serious-1.2.5/serious/serialization/key_mapper.py`

 * *Files identical despite different names*

### Comparing `serious-1.2.2/serious/serialization/model.py` & `serious-1.2.5/serious/serialization/model.py`

 * *Files identical despite different names*

### Comparing `serious-1.2.2/serious/serialization/serializer.py` & `serious-1.2.5/serious/serialization/serializer.py`

 * *Files identical despite different names*

### Comparing `serious-1.2.2/serious/test_utils.py` & `serious-1.2.5/serious/test_utils.py`

 * *Files identical despite different names*

### Comparing `serious-1.2.2/serious/types.py` & `serious-1.2.5/serious/types.py`

 * *Files identical despite different names*

### Comparing `serious-1.2.2/serious/validation.py` & `serious-1.2.5/serious/validation.py`

 * *Files identical despite different names*

### Comparing `serious-1.2.2/serious.egg-info/PKG-INFO` & `serious-1.2.5/serious.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,210 +1,210 @@
 Metadata-Version: 2.1
 Name: serious
-Version: 1.2.2
+Version: 1.2.5
 Summary: Easily serialize dataclasses to and from JSON
 Home-page: https://github.com/mdrachuk/serious
 Author: mdrachuk
 Author-email: misha@drach.uk
 License: MIT
 Project-URL: Pipelines, https://dev.azure.com/misha-drachuk/serious
 Project-URL: Source, https://github.com/mdrachuk/serious/
 Project-URL: Issues, https://github.com/mdrachuk/serious/issues
-Description: # serious
-        [![PyPI](https://img.shields.io/pypi/v/serious)][pypi]
-        [![Build Status](https://img.shields.io/azure-devops/build/misha-drachuk/serious/2)](https://dev.azure.com/misha-drachuk/serious/_build/latest?definitionId=1&branchName=master)
-        [![Test Coverage](https://img.shields.io/coveralls/github/mdrachuk/serious/master)](https://coveralls.io/github/mdrachuk/serious)
-        [![Supported Python](https://img.shields.io/pypi/pyversions/serious)][pypi]
-        [![Documentation](https://img.shields.io/readthedocs/serious)][docs]
-        
-        A dataclass model toolkit: serialization, validation, and more.
-        
-        [Documentation][docs]
-        
-        
-        ## Features
-        - Model definitions in pure Python.
-        - Validation showing up in code coverage.
-        - Type annotations for all public-facing APIs.
-        - (Optionally) ensures immutability.
-        - Easily extensible.
-        - Made for people.
-        - Documented rigorously.
-        
-        ## Basics
-        ### Installation
-        Available from [PyPI][pypi]:
-        ```shell
-        pip install serious
-        ```
-        
-        ### Quick Example
-        
-        Central part of Serious API are different [Models][doc-models].
-        
-        Given a regular dataclass:
-        ```python
-        from dataclasses import dataclass
-        
-        @dataclass
-        class Person:
-            name: str
-        ```
-        
-        Let’s create a `JsonModel`:  
-        ```python
-        from serious.json import JsonModel
-            
-        model = JsonModel(Person)
-        ```
-        
-        And use its [dump/load methods][doc-serialization]:
-        ```python
-        person = Person('Albert Einstein')
-        
-        model.dump(person) # {"name": "Albert Einstein"}
-        ```
-        
-        ### Validation
-        To add validation to the example above all we need is to add `__validate__` method to person:
-        ```python
-        from dataclasses import dataclass
-        from typing import Optional
-        from serious import ValidationError, Email
-        
-        @dataclass
-        class Person:
-            name: str
-            email: Optional[Email]
-            phone: Optional[str]
-        
-            def __validate__(self):
-                if len(self.name) == 0:
-                    raise ValidationError('Every person needs a name')
-                if self.phone is None and self.email is None:
-                    raise ValidationError('At least some contact should be present')
-        ```
-        
-        [More on validation.][doc-validation]
-        
-        
-        ### Supported formats:
-        - [x] [JSON][doc-json-model]
-        - [x] [Python Dictionaries][doc-dict-model]
-        - [ ] YAML
-        - [ ] Form data
-        
-        
-        ### Supported field types
-        [More in docs.][doc-types]
-        
-        - Other dataclasses
-        - Primitives: `str`, `int`, `float`, `bool`
-        - Dictionaries: only with string keys: `Dict[str, Any]`  
-        - Lists, [sets][set], [deques][deque]: python collections of any serializable type
-        - [Tuples][tuple] both with and without ellipsis:
-            - tuples as set of independent elements (e.g. `Tuple[str, int, date]`) 
-            - with ellipses, acting as a frozen list (`Tuple[str, ...]`)
-        - [Enumerations][enum] by value:
-            - of primitives (e.g. `OperatingSystem(Enum)`) 
-            - typed enums (`Color(str, Enum)` and `FilePermission(IntFlag)`)
-        - [Decimal][decimal]: encoded to JSON as string 
-        - [Datetime][datetime], [date][date] and [time][time]: encoded to the [ISO 8601][iso8601] formatted string
-        - [UUID][uuid]
-        - `serious.types.Timestamp`: a UTC timestamp since [UNIX epoch][epoch] as float ms value 
-        - `serious.types.Email`: a string Tiny Type that supports validation and contains additional properties 
-        - custom immutable alternatives to native python types in `serious.types`: `FrozenList`, `FrozenDict`
-        
-        ## A bigger example
-        
-        ```python
-        from dataclasses import dataclass
-        from serious import JsonModel, ValidationError
-        from typing import List
-        from enum import Enum
-        
-        class Specialty(Enum):
-            Worker = 1
-            Fool = 2
-        
-        
-        @dataclass(frozen=True)
-        class Minion:
-            name: str
-            type: Specialty
-        
-        
-        @dataclass(frozen=True)
-        class Boss:
-            name: str
-            minions: List[Minion]
-            
-            def __validate__(self):
-                if len(self.minions) < 2:
-                    raise ValidationError('What kind of boss are you?')
-        
-        
-        boss = Boss("me", [Minion('evil minion', Specialty.Fool), Minion('very evil minion', Specialty.Worker)])
-        boss_json = """{
-            "name": "me",
-            "minions": [
-                {
-                    "name": "evil minion",
-                    "type": "Fool"
-                },
-                {
-                    "name": "very evil minion",
-                    "type": "Worker"
-                }
-            ]
-        }"""
-        
-        model = JsonModel(Boss, indent=4)
-        
-        assert model.dump(boss) == boss_json
-        assert model.load(boss_json) == boss
-        ```
-        
-        
-        ## Acknowledgements
-        Initially, a fork of [@lidatong/dataclasses-json](https://github.com/lidatong/dataclasses-json).
-        
-        [pypi]: https://pypi.org/project/serious/
-        [dataclass]: https://docs.python.org/3/library/dataclasses.html
-        [iso8601]: https://en.wikipedia.org/wiki/ISO_8601
-        [epoch]: https://en.wikipedia.org/wiki/Unix_time
-        [enum]: https://docs.python.org/3/library/enum.html
-        [decimal]: https://docs.python.org/3/library/decimal.html
-        [tuple]: https://docs.python.org/3/library/stdtypes.html#tuple
-        [list]: https://docs.python.org/3/library/stdtypes.html#list
-        [set]: https://docs.python.org/3/library/stdtypes.html#set
-        [deque]: https://docs.python.org/3.7/library/collections.html#collections.deque
-        [datetime]: https://docs.python.org/3.7/library/datetime.html#datetime.datetime
-        [date]: https://docs.python.org/3.7/library/datetime.html#datetime.date
-        [time]: https://docs.python.org/3.7/library/datetime.html#datetime.time
-        [uuid]: https://docs.python.org/3.7/library/uuid.html?highlight=uuid#uuid.UUID
-        [doc-types]: https://serious.readthedocs.io/en/latest/types/
-        [doc-models]: https://serious.readthedocs.io/en/latest/models/
-        [doc-json-model]: https://serious.readthedocs.io/en/latest/models/#jsonmodel
-        [doc-dict-model]: https://serious.readthedocs.io/en/latest/models/#dictmodel
-        [doc-serialization]: https://serious.readthedocs.io/en/latest/serialization/ (Serialization documentation)
-        [doc-validation]: https://serious.readthedocs.io/en/latest/validation/ (Validation documentation)
-        [docs]: https://serious.readthedocs.io/en/latest/ 
-        
 Keywords: dataclasses json serialization
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: POSIX :: BSD
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# serious
+[![PyPI](https://img.shields.io/pypi/v/serious)][pypi]
+[![Build Status](https://img.shields.io/azure-devops/build/misha-drachuk/serious/2)](https://dev.azure.com/misha-drachuk/serious/_build/latest?definitionId=1&branchName=master)
+[![Test Coverage](https://img.shields.io/coveralls/github/mdrachuk/serious/master)](https://coveralls.io/github/mdrachuk/serious)
+[![Supported Python](https://img.shields.io/pypi/pyversions/serious)][pypi]
+[![Documentation](https://img.shields.io/readthedocs/serious)][docs]
+
+A dataclass model toolkit: serialization, validation, and more.
+
+[Documentation][docs]
+
+
+## Features
+- Model definitions in pure Python.
+- Validation showing up in code coverage.
+- Type annotations for all public-facing APIs.
+- (Optionally) ensures immutability.
+- Easily extensible.
+- Made for people.
+- Documented rigorously.
+
+## Basics
+### Installation
+Available from [PyPI][pypi]:
+```shell
+pip install serious
+```
+
+### Quick Example
+
+Central part of Serious API are different [Models][doc-models].
+
+Given a regular dataclass:
+```python
+from dataclasses import dataclass
+
+@dataclass
+class Person:
+    name: str
+```
+
+Let’s create a `JsonModel`:  
+```python
+from serious.json import JsonModel
+    
+model = JsonModel(Person)
+```
+
+And use its [dump/load methods][doc-serialization]:
+```python
+person = Person('Albert Einstein')
+
+model.dump(person) # {"name": "Albert Einstein"}
+```
+
+### Validation
+To add validation to the example above all we need is to add `__validate__` method to person:
+```python
+from dataclasses import dataclass
+from typing import Optional
+from serious import ValidationError, Email
+
+@dataclass
+class Person:
+    name: str
+    email: Optional[Email]
+    phone: Optional[str]
+
+    def __validate__(self):
+        if len(self.name) == 0:
+            raise ValidationError('Every person needs a name')
+        if self.phone is None and self.email is None:
+            raise ValidationError('At least some contact should be present')
+```
+
+[More on validation.][doc-validation]
+
+
+### Supported formats:
+- [x] [JSON][doc-json-model]
+- [x] [Python Dictionaries][doc-dict-model]
+- [ ] YAML
+- [ ] Form data
+
+
+### Supported field types
+[More in docs.][doc-types]
+
+- Other dataclasses
+- Primitives: `str`, `int`, `float`, `bool`
+- Dictionaries: only with string keys: `Dict[str, Any]`  
+- Lists, [sets][set], [deques][deque]: python collections of any serializable type
+- [Tuples][tuple] both with and without ellipsis:
+    - tuples as set of independent elements (e.g. `Tuple[str, int, date]`) 
+    - with ellipses, acting as a frozen list (`Tuple[str, ...]`)
+- [Enumerations][enum] by value:
+    - of primitives (e.g. `OperatingSystem(Enum)`) 
+    - typed enums (`Color(str, Enum)` and `FilePermission(IntFlag)`)
+- [Decimal][decimal]: encoded to JSON as string 
+- [Datetime][datetime], [date][date] and [time][time]: encoded to the [ISO 8601][iso8601] formatted string
+- [UUID][uuid]
+- `serious.types.Timestamp`: a UTC timestamp since [UNIX epoch][epoch] as float ms value 
+- `serious.types.Email`: a string Tiny Type that supports validation and contains additional properties 
+- custom immutable alternatives to native python types in `serious.types`: `FrozenList`, `FrozenDict`
+
+## A bigger example
+
+```python
+from dataclasses import dataclass
+from serious import JsonModel, ValidationError
+from typing import List
+from enum import Enum
+
+class Specialty(Enum):
+    Worker = 1
+    Fool = 2
+
+
+@dataclass(frozen=True)
+class Minion:
+    name: str
+    type: Specialty
+
+
+@dataclass(frozen=True)
+class Boss:
+    name: str
+    minions: List[Minion]
+    
+    def __validate__(self):
+        if len(self.minions) < 2:
+            raise ValidationError('What kind of boss are you?')
+
+
+boss = Boss("me", [Minion('evil minion', Specialty.Fool), Minion('very evil minion', Specialty.Worker)])
+boss_json = """{
+    "name": "me",
+    "minions": [
+        {
+            "name": "evil minion",
+            "type": "Fool"
+        },
+        {
+            "name": "very evil minion",
+            "type": "Worker"
+        }
+    ]
+}"""
+
+model = JsonModel(Boss, indent=4)
+
+assert model.dump(boss) == boss_json
+assert model.load(boss_json) == boss
+```
+
+
+## Acknowledgements
+Initially, a fork of [@lidatong/dataclasses-json](https://github.com/lidatong/dataclasses-json).
+
+[pypi]: https://pypi.org/project/serious/
+[dataclass]: https://docs.python.org/3/library/dataclasses.html
+[iso8601]: https://en.wikipedia.org/wiki/ISO_8601
+[epoch]: https://en.wikipedia.org/wiki/Unix_time
+[enum]: https://docs.python.org/3/library/enum.html
+[decimal]: https://docs.python.org/3/library/decimal.html
+[tuple]: https://docs.python.org/3/library/stdtypes.html#tuple
+[list]: https://docs.python.org/3/library/stdtypes.html#list
+[set]: https://docs.python.org/3/library/stdtypes.html#set
+[deque]: https://docs.python.org/3.7/library/collections.html#collections.deque
+[datetime]: https://docs.python.org/3.7/library/datetime.html#datetime.datetime
+[date]: https://docs.python.org/3.7/library/datetime.html#datetime.date
+[time]: https://docs.python.org/3.7/library/datetime.html#datetime.time
+[uuid]: https://docs.python.org/3.7/library/uuid.html?highlight=uuid#uuid.UUID
+[doc-types]: https://serious.readthedocs.io/en/latest/types/
+[doc-models]: https://serious.readthedocs.io/en/latest/models/
+[doc-json-model]: https://serious.readthedocs.io/en/latest/models/#jsonmodel
+[doc-dict-model]: https://serious.readthedocs.io/en/latest/models/#dictmodel
+[doc-serialization]: https://serious.readthedocs.io/en/latest/serialization/ (Serialization documentation)
+[doc-validation]: https://serious.readthedocs.io/en/latest/validation/ (Validation documentation)
+[docs]: https://serious.readthedocs.io/en/latest/
```

### Comparing `serious-1.2.2/serious.egg-info/SOURCES.txt` & `serious-1.2.5/serious.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 README.md
 setup.py
 serious/__init__.py
 serious/checks.py
 serious/descriptors.py
 serious/errors.py
+serious/py.typed
 serious/test_utils.py
 serious/types.py
 serious/utils.py
 serious/validation.py
 serious.egg-info/PKG-INFO
 serious.egg-info/SOURCES.txt
 serious.egg-info/dependency_links.txt
```

### Comparing `serious-1.2.2/setup.py` & `serious-1.2.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     author_email='misha@drach.uk',
     description="Easily serialize dataclasses to and from JSON",
     long_description=readme(),
     long_description_content_type='text/markdown',
     url="https://github.com/mdrachuk/serious",
     license="MIT",
     keywords="dataclasses json serialization",
-    python_requires=">=3.8",
+    python_requires=">=3.10",
     project_urls={
         'Pipelines': 'https://dev.azure.com/misha-drachuk/serious',
         'Source': 'https://github.com/mdrachuk/serious/',
         'Issues': 'https://github.com/mdrachuk/serious/issues',
     },
     include_package_data=True,
     classifiers=[
```

