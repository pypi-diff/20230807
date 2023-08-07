# Comparing `tmp/cfgparser-1.0.4.tar.gz` & `tmp/cfgparser-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfgparser-1.0.4.tar", last modified: Sun Aug  6 02:14:40 2023, max compression
+gzip compressed data, was "cfgparser-1.0.5.tar", last modified: Mon Aug  7 02:55:16 2023, max compression
```

## Comparing `cfgparser-1.0.4.tar` & `cfgparser-1.0.5.tar`

### file list

```diff
@@ -1,22 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:14:40.026437 cfgparser-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-08-06 02:14:29.000000 cfgparser-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-08-06 02:14:40.026437 cfgparser-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-08-06 02:14:29.000000 cfgparser-1.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 02:14:40.026437 cfgparser-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     7342 2023-08-06 02:14:29.000000 cfgparser-1.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:14:40.026437 cfgparser-1.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:14:40.026437 cfgparser-1.0.4/src/cfgparser/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:14:40.026437 cfgparser-1.0.4/src/cfgparser/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 02:14:29.000000 cfgparser-1.0.4/src/cfgparser/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-08-06 02:14:29.000000 cfgparser-1.0.4/src/cfgparser/io/fileloader.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-08-06 02:14:29.000000 cfgparser-1.0.4/src/cfgparser/io/jsonfileloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-08-06 02:14:29.000000 cfgparser-1.0.4/src/cfgparser/json_config_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:14:40.026437 cfgparser-1.0.4/src/cfgparser/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 02:14:29.000000 cfgparser-1.0.4/src/cfgparser/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-08-06 02:14:29.000000 cfgparser-1.0.4/src/cfgparser/utils/dynamic_type_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-08-06 02:14:29.000000 cfgparser-1.0.4/src/cfgparser/utils/execution_timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:14:40.026437 cfgparser-1.0.4/src/cfgparser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-08-06 02:14:39.000000 cfgparser-1.0.4/src/cfgparser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-08-06 02:14:39.000000 cfgparser-1.0.4/src/cfgparser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 02:14:39.000000 cfgparser-1.0.4/src/cfgparser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-06 02:14:39.000000 cfgparser-1.0.4/src/cfgparser.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 02:55:16.794769 cfgparser-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-08-07 02:55:07.000000 cfgparser-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-08-07 02:55:16.794769 cfgparser-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-08-07 02:55:07.000000 cfgparser-1.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 02:55:16.794769 cfgparser-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7356 2023-08-07 02:55:07.000000 cfgparser-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 02:55:16.794769 cfgparser-1.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 02:55:16.794769 cfgparser-1.0.5/src/cfgparser/
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-08-07 02:55:07.000000 cfgparser-1.0.5/src/cfgparser/config_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 02:55:16.794769 cfgparser-1.0.5/src/cfgparser/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 02:55:07.000000 cfgparser-1.0.5/src/cfgparser/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-08-07 02:55:07.000000 cfgparser-1.0.5/src/cfgparser/io/fileloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-08-07 02:55:07.000000 cfgparser-1.0.5/src/cfgparser/io/jsonfileloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-08-07 02:55:07.000000 cfgparser-1.0.5/src/cfgparser/io/yamlfileloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-07 02:55:07.000000 cfgparser-1.0.5/src/cfgparser/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 02:55:16.794769 cfgparser-1.0.5/src/cfgparser/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 02:55:07.000000 cfgparser-1.0.5/src/cfgparser/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-08-07 02:55:07.000000 cfgparser-1.0.5/src/cfgparser/utils/dynamic_type_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-08-07 02:55:07.000000 cfgparser-1.0.5/src/cfgparser/utils/execution_timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-08-07 02:55:07.000000 cfgparser-1.0.5/src/cfgparser/utils/union_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 02:55:16.794769 cfgparser-1.0.5/src/cfgparser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-08-07 02:55:16.000000 cfgparser-1.0.5/src/cfgparser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-08-07 02:55:16.000000 cfgparser-1.0.5/src/cfgparser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 02:55:16.000000 cfgparser-1.0.5/src/cfgparser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-07 02:55:16.000000 cfgparser-1.0.5/src/cfgparser.egg-info/top_level.txt
```

### Comparing `cfgparser-1.0.4/LICENSE` & `cfgparser-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cfgparser-1.0.4/PKG-INFO` & `cfgparser-1.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: cfgparser
-Version: 1.0.4
-Summary: Python package that allows to parse typed JSON configs defined by python dataclasses
+Version: 1.0.5
+Summary: Python package that allows to parse typed configs defined by python dataclasses
 Home-page: https://github.com/CaRniFeXeR/PythonConfigParser
 Author: Florian Kowarsch
 Author-email: flo.kowarsch@yahoo.de
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/CaRniFeXeR/PythonConfigParser/issues
 Project-URL: Source, https://github.com/CaRniFeXeR/PythonConfigParser/
 Description: # PythonConfigParser
@@ -37,26 +37,26 @@
         
         ### from file 
         
         First initialize the config parser with the path to the module with the config definitions.
         
         ```python
         
-        parser = JSONConfigParser(datastructure_module_name="mysrc.datastructures.configs")
+        parser = ConfigParser(datastructure_module_name="mysrc.datastructures.configs")
         # Then parse the config from file.
         my_config = parser.parse_from_file("myconfig.json")
         
         ```
         
         ### from dictionary
         
         ```python
         
         my_config_dict = {"type_name" : "mysrc.datastructures.configs.a"}
-        my_config = JSONConfigParser().parse(my_config_dict)
+        my_config = ConfigParser().parse(my_config_dict)
         
         ```
         
         
         #### type definition
         There are two ways to define the configs type:
         - specified in the config itself
@@ -64,43 +64,44 @@
             - path to the config class must be specified as str in the config as key "type_name"
         - specified when parsing the config
             - if the config has no key "typed_config" set, the type can be specified when parsing the config
             
         ```python
         from mysrc.datastructures.configs import a
         my_config_dict = {"some_key" : "some_value"}
-        my_config = JSONConfigParser().parse_typed(my_config_dict,a)
+        my_config = ConfigParser().parse_typed(my_config_dict,a)
         
         ```
         
+        By default every field can be explicitly set to None. If you don't what this behaviour you can set the flag "allow_none" to False.
         
+        ```python
+            cfgparser.settings.allow_none = False
+        ```
         
         ## Features
         
-        - fully typed json configs
+        - fully typed json and yaml configs
         - nested configs
+        - complex union and optional types
         - dict object into typed dataclass
         
         ## Installation
         
         ```
         pip install cfgparser
         ```
         
-        ## Coming Features
+        ## Features Roadmap
         
-        - yaml support
-        - typed optional support
-        - typed union support
         - specify config from cli
-        - cd pipeline 
         - post hock
         - distributed configs
         
-Keywords: config,praser,JSON,typed-parsing,dataclass
+Keywords: config,parser,YAML,JSON,typed-parsing,dataclass,lightweight
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `cfgparser-1.0.4/README.md` & `cfgparser-1.0.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -27,26 +27,26 @@
 
 ### from file 
 
 First initialize the config parser with the path to the module with the config definitions.
 
 ```python
 
-parser = JSONConfigParser(datastructure_module_name="mysrc.datastructures.configs")
+parser = ConfigParser(datastructure_module_name="mysrc.datastructures.configs")
 # Then parse the config from file.
 my_config = parser.parse_from_file("myconfig.json")
 
 ```
 
 ### from dictionary
 
 ```python
 
 my_config_dict = {"type_name" : "mysrc.datastructures.configs.a"}
-my_config = JSONConfigParser().parse(my_config_dict)
+my_config = ConfigParser().parse(my_config_dict)
 
 ```
 
 
 #### type definition
 There are two ways to define the configs type:
 - specified in the config itself
@@ -54,34 +54,35 @@
     - path to the config class must be specified as str in the config as key "type_name"
 - specified when parsing the config
     - if the config has no key "typed_config" set, the type can be specified when parsing the config
     
 ```python
 from mysrc.datastructures.configs import a
 my_config_dict = {"some_key" : "some_value"}
-my_config = JSONConfigParser().parse_typed(my_config_dict,a)
+my_config = ConfigParser().parse_typed(my_config_dict,a)
 
 ```
 
+By default every field can be explicitly set to None. If you don't what this behaviour you can set the flag "allow_none" to False.
 
+```python
+    cfgparser.settings.allow_none = False
+```
 
 ## Features
 
-- fully typed json configs
+- fully typed json and yaml configs
 - nested configs
+- complex union and optional types
 - dict object into typed dataclass
 
 ## Installation
 
 ```
 pip install cfgparser
 ```
 
-## Coming Features
+## Features Roadmap
 
-- yaml support
-- typed optional support
-- typed union support
 - specify config from cli
-- cd pipeline 
 - post hock
 - distributed configs
```

### Comparing `cfgparser-1.0.4/setup.py` & `cfgparser-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,19 @@
     name="cfgparser",  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/guides/single-sourcing-package-version/
-    version="1.0.4",  # Required
+    version="1.0.5",  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
-    description="Python package that allows to parse typed JSON configs defined by python dataclasses",  # Optional
+    description="Python package that allows to parse typed configs defined by python dataclasses",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
     # Often, this is the same as your README, so you can just read it in from
     # that file directly (as we have already done above)
     #
     # This field corresponds to the "Description" metadata field:
@@ -97,15 +97,15 @@
     ],
     # This field adds keywords for your project which will appear on the
     # project page. What does your project relate to?
     #
     # Note that this is a list of additional keywords, separated
     # by commas, to be used to assist searching for the distribution in a
     # larger catalog.
-    keywords="config, praser, JSON, typed-parsing, dataclass",  # Optional
+    keywords="config, parser, YAML, JSON, typed-parsing, dataclass, lightweight",  # Optional
     # When your source code is in a subdirectory under the project root, e.g.
     # `src/`, it is necessary to specify the `package_dir` argument.
     package_dir={"": "src"},  # Optional
     # You can just specify package directories manually here if your project is
     # simple. Or you can use find_packages().
     #
     # Alternatively, if you just want to distribute a single Python file, use
```

### Comparing `cfgparser-1.0.4/src/cfgparser/io/fileloader.py` & `cfgparser-1.0.5/src/cfgparser/io/fileloader.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from abc import ABC
+from abc import ABC, abstractmethod
 from pathlib import Path
 
 
 class FileLoader(ABC):
 
     def __init__(self, inputfile: Path):
 
@@ -12,13 +12,17 @@
         if isinstance(inputfile, str):
             inputfile = Path(inputfile)
 
         self.checkFileExists(inputfile)
 
         self.inputfile = inputfile
 
+    @abstractmethod
+    def load_file(self):
+        pass
+
     def checkFileExists(self, inputfile: Path):
 
         if not inputfile.exists():
             message = f"'{inputfile}' does not exist"
             print(message)
             raise Exception(message)
```

### Comparing `cfgparser-1.0.4/src/cfgparser/utils/dynamic_type_loader.py` & `cfgparser-1.0.5/src/cfgparser/utils/dynamic_type_loader.py`

 * *Files identical despite different names*

### Comparing `cfgparser-1.0.4/src/cfgparser.egg-info/PKG-INFO` & `cfgparser-1.0.5/src/cfgparser.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: cfgparser
-Version: 1.0.4
-Summary: Python package that allows to parse typed JSON configs defined by python dataclasses
+Version: 1.0.5
+Summary: Python package that allows to parse typed configs defined by python dataclasses
 Home-page: https://github.com/CaRniFeXeR/PythonConfigParser
 Author: Florian Kowarsch
 Author-email: flo.kowarsch@yahoo.de
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/CaRniFeXeR/PythonConfigParser/issues
 Project-URL: Source, https://github.com/CaRniFeXeR/PythonConfigParser/
 Description: # PythonConfigParser
@@ -37,26 +37,26 @@
         
         ### from file 
         
         First initialize the config parser with the path to the module with the config definitions.
         
         ```python
         
-        parser = JSONConfigParser(datastructure_module_name="mysrc.datastructures.configs")
+        parser = ConfigParser(datastructure_module_name="mysrc.datastructures.configs")
         # Then parse the config from file.
         my_config = parser.parse_from_file("myconfig.json")
         
         ```
         
         ### from dictionary
         
         ```python
         
         my_config_dict = {"type_name" : "mysrc.datastructures.configs.a"}
-        my_config = JSONConfigParser().parse(my_config_dict)
+        my_config = ConfigParser().parse(my_config_dict)
         
         ```
         
         
         #### type definition
         There are two ways to define the configs type:
         - specified in the config itself
@@ -64,43 +64,44 @@
             - path to the config class must be specified as str in the config as key "type_name"
         - specified when parsing the config
             - if the config has no key "typed_config" set, the type can be specified when parsing the config
             
         ```python
         from mysrc.datastructures.configs import a
         my_config_dict = {"some_key" : "some_value"}
-        my_config = JSONConfigParser().parse_typed(my_config_dict,a)
+        my_config = ConfigParser().parse_typed(my_config_dict,a)
         
         ```
         
+        By default every field can be explicitly set to None. If you don't what this behaviour you can set the flag "allow_none" to False.
         
+        ```python
+            cfgparser.settings.allow_none = False
+        ```
         
         ## Features
         
-        - fully typed json configs
+        - fully typed json and yaml configs
         - nested configs
+        - complex union and optional types
         - dict object into typed dataclass
         
         ## Installation
         
         ```
         pip install cfgparser
         ```
         
-        ## Coming Features
+        ## Features Roadmap
         
-        - yaml support
-        - typed optional support
-        - typed union support
         - specify config from cli
-        - cd pipeline 
         - post hock
         - distributed configs
         
-Keywords: config,praser,JSON,typed-parsing,dataclass
+Keywords: config,parser,YAML,JSON,typed-parsing,dataclass,lightweight
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

