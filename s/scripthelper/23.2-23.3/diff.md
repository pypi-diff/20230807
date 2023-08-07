# Comparing `tmp/scripthelper-23.2.tar.gz` & `tmp/scripthelper-23.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scripthelper-23.2.tar", last modified: Thu Feb 16 09:03:58 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `scripthelper-23.2.tar` & `scripthelper-23.3.tar`

### file list

```diff
@@ -1,15 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-02-16 09:03:58.367126 scripthelper-23.2/
--rw-rw-rw-   0        0        0     1091 2022-01-18 07:45:17.000000 scripthelper-23.2/LICENSE
--rw-rw-rw-   0        0        0     6533 2023-02-16 09:03:58.365126 scripthelper-23.2/PKG-INFO
--rw-rw-rw-   0        0        0     2045 2023-02-16 08:57:39.000000 scripthelper-23.2/README.md
-drwxrwxrwx   0        0        0        0 2023-02-16 09:03:58.341125 scripthelper-23.2/scripthelper/
--rw-rw-rw-   0        0        0     8238 2023-02-16 08:40:43.000000 scripthelper-23.2/scripthelper/__init__.py
--rw-rw-rw-   0        0        0        0 2022-03-25 12:43:26.000000 scripthelper-23.2/scripthelper/py.typed
-drwxrwxrwx   0        0        0        0 2023-02-16 09:03:58.363125 scripthelper-23.2/scripthelper.egg-info/
--rw-rw-rw-   0        0        0     6533 2023-02-16 09:03:57.000000 scripthelper-23.2/scripthelper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2023-02-16 09:03:58.000000 scripthelper-23.2/scripthelper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-16 09:03:57.000000 scripthelper-23.2/scripthelper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      123 2023-02-16 09:03:57.000000 scripthelper-23.2/scripthelper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-02-16 09:03:57.000000 scripthelper-23.2/scripthelper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-16 09:03:58.368128 scripthelper-23.2/setup.cfg
--rw-rw-rw-   0        0        0     2057 2023-02-16 08:59:54.000000 scripthelper-23.2/setup.py
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 scripthelper-23.3/CHANGELOG.md
+-rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 scripthelper-23.3/README.md
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 scripthelper-23.3/compile-readme.py
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 scripthelper-23.3/example1.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 scripthelper-23.3/example10.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 scripthelper-23.3/example2.py
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 scripthelper-23.3/example2b.py
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 scripthelper-23.3/example3.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 scripthelper-23.3/example4.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 scripthelper-23.3/example4module.py
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 scripthelper-23.3/example5.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 scripthelper-23.3/example6.py
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 scripthelper-23.3/example7.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 scripthelper-23.3/example8.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 scripthelper-23.3/example9.py
+-rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 scripthelper-23.3/justfile
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 scripthelper-23.3/mypy.ini
+-rw-r--r--   0        0        0    10672 2020-02-02 00:00:00.000000 scripthelper-23.3/test_examples.py
+-rw-r--r--   0        0        0     8563 2020-02-02 00:00:00.000000 scripthelper-23.3/src/scripthelper/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scripthelper-23.3/src/scripthelper/py.typed
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 scripthelper-23.3/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 scripthelper-23.3/LICENSE
+-rw-r--r--   0        0        0     6335 2020-02-02 00:00:00.000000 scripthelper-23.3/README.compiled.md
+-rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 scripthelper-23.3/pyproject.toml
+-rw-r--r--   0        0        0     7370 2020-02-02 00:00:00.000000 scripthelper-23.3/PKG-INFO
```

### Comparing `scripthelper-23.2/LICENSE` & `scripthelper-23.3/LICENSE`

 * *Files identical despite different names*

### Comparing `scripthelper-23.2/PKG-INFO` & `scripthelper-23.3/README.compiled.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,7 @@
-Metadata-Version: 2.1
-Name: scripthelper
-Version: 23.2
-Summary: Helper module for creating simple Python scripts
-Home-page: https://github.com/presidento/scripthelper
-Author: Máté Farkas
-Author-email: fm@farkas-mate.hu
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: System Administrators
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Utilities
-Classifier: Typing :: Typed
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # scripthelper
 
 Helper module for simple command line Python scripts.
 
 
 ## Basic usage
 
@@ -73,22 +50,25 @@
 
 ```python
 #!/usr/bin/env python3
 import scripthelper
 
 logger = scripthelper.getLogger(__name__)
 
+
 def greet(name):
     logger.info(f"Hello {name}")
 
+
 def main():
     scripthelper.add_argument("--name", default="World")
     args = scripthelper.initialize()
     greet(args.name)
 
+
 main()
 ```
 
 ## Progressbar works with logging, too
 
 [example3.py](https://github.com/presidento/scripthelper/blob/master/example3.py):
 
@@ -203,46 +183,78 @@
 ```python
 #!/usr/bin/env python3
 import scripthelper
 from dataclasses import dataclass
 
 scripthelper.bootstrap()
 
+
 @dataclass
 class Item:
     name: str
     value: int
 
+
 something = {
     "string": "value1",
     "bool": True,
     "none": None,
     "integer": 1234,
-    "item": Item("name", 999)
+    "item": Item("name", 999),
 }
 
 scripthelper.pp(something)
 ```
 
 ## Has built-in persisted state handler
 
+The state is persisted immediately in the background in YAML. Mutable objects (`list`, `dict`) also can be used.
+
 [example9.py](https://github.com/presidento/scripthelper/blob/master/example9.py):
 
 ```python
 #!/usr/bin/env python3
 import scripthelper
 
 logger = scripthelper.bootstrap()
-state = scripthelper.PersistedState(processed_id=0)
+state = scripthelper.PersistedState(processed_id=0, to_remember=[])
 
 state.processed_id += 1
+state.to_remember.append(f"Element {state.processed_id}")
+while len(state.to_remember) > 2:
+    state.to_remember.pop(0)
+
 logger.info(f"Processing item #{state.processed_id}")
+for item in state.to_remember:
+    logger.info(f"- {item}")
 ```
 
 ```
-$ python example9.py
+$ python3 example9.py
 INFO Processing item #1
-$ python example9.py
+INFO - Element 1
+
+$ python3 example9.py
 INFO Processing item #2
-$ python example9.py
+INFO - Element 1
+INFO - Element 2
+
+$ python3 example9.py
 INFO Processing item #3
+INFO - Element 2
+INFO - Element 3
 ```
+
+## Helps issue a warning only once
+
+[example10.py](https://github.com/presidento/scripthelper/blob/master/example10.py):
+
+```python
+#!/usr/bin/env python3
+import scripthelper
+
+scripthelper.bootstrap()
+
+for _ in range(10):
+    scripthelper.warning_once("Item #12 has some errors")
+```
+
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `scripthelper-23.2/README.md` & `scripthelper-23.3/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -57,17 +57,31 @@
 
 ## Has built-in colored pretty printer
 
 See [example7.py](example7.py)
 
 ## Has built-in persisted state handler
 
+The state is persisted immediately in the background in YAML. Mutable objects (`list`, `dict`) also can be used.
+
 See [example9.py](example9.py)
 
 ```
-$ python example9.py
+$ python3 example9.py
 INFO Processing item #1
-$ python example9.py
+INFO - Element 1
+
+$ python3 example9.py
 INFO Processing item #2
-$ python example9.py
+INFO - Element 1
+INFO - Element 2
+
+$ python3 example9.py
 INFO Processing item #3
+INFO - Element 2
+INFO - Element 3
 ```
+
+## Helps issue a warning only once
+
+See [example10.py](example10.py)
+
```

### Comparing `scripthelper-23.2/scripthelper/__init__.py` & `scripthelper-23.3/src/scripthelper/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     "CRITICAL",
     "ERROR",
     "WARNING",
     "INFO",
     "VERBOSE",
     "DEBUG",
     "SPAM",
+    "warning_once",
     # Warning
     "warn",
     # Argument parsing and bootstrap
     "bootstrap",
     "bootstrap_args",
     "initialize",
     "add_arguments",
@@ -160,14 +161,27 @@
     It is an alias for verboselogs.VerboseLogger.
     Can be used as the logging.getLogger() method.
     Extends built-in logger with levels: verbose, spam
     """
     return verboselogs.VerboseLogger(name)
 
 
+_WARNING_ONCE_CACHE = set()
+
+
+def warning_once(msg, *args, **kwargs):
+    """Issue a warning only once
+
+    Only the first call will be logged with the same message."""
+    if msg in _WARNING_ONCE_CACHE:
+        return
+    _WARNING_ONCE_CACHE.add(msg)
+    logger.warning(msg, *args, **kwargs)
+
+
 args: argparse.Namespace  # Parsed arguments, will be set during bootstrap
 
 parser = argparse.ArgumentParser()
 parser.add_argument(
     "-v",
     "--verbose",
     action="count",
@@ -217,15 +231,15 @@
     file_log_handler.setFormatter(formatter)
     file_log_handler.setLevel(level)
     logging.getLogger().addHandler(file_log_handler)
 
 
 def progressbar(*args, disable=None, **kwargs):
     """See tqdm.tqdm
-    
+
     The default value for 'disable' is None, meaning
         - enable progressbar on terminals
         - disable progressbar on non-tty
     (checking the type of stderr)"""
     kwargs["disable"] = disable
     return tqdm.tqdm(*args, **kwargs)
 
@@ -236,23 +250,25 @@
         prettyprinter.cpprint(*args, **kwargs)
     else:
         prettyprinter.pprint(*args, **kwargs)
 
 
 pp = pprint
 
+
 class PersistedState(persistedstate.PersistedState):
     def __init__(self, _filename=None, **kwargs):
         filename = _filename
         if filename is None:
             caller_module = inspect.getmodule(inspect.stack()[1][0])
             module_file: str = caller_module.__file__  # type:ignore
             filename = pathlib.Path(module_file).with_suffix(".state").as_posix()
         return super().__init__(filename, **kwargs)
 
+
 def bootstrap_args() -> Tuple[verboselogs.VerboseLogger, argparse.Namespace]:
     """Bootstraps the framework
 
     returns (logger, args)
         The logger for main scripts
         And the parsed argument"""
     global args
@@ -282,10 +298,10 @@
 
     returns logger - the logger for the main script"""
     return bootstrap_args()[0]
 
 
 def initialize() -> argparse.Namespace:
     """Bootstraps the framework
-    
+
     return args - the parsed arguments"""
     return bootstrap_args()[1]
```

### Comparing `scripthelper-23.2/scripthelper.egg-info/PKG-INFO` & `scripthelper-23.3/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,248 +1,293 @@
-Metadata-Version: 2.1
-Name: scripthelper
-Version: 23.2
-Summary: Helper module for creating simple Python scripts
-Home-page: https://github.com/presidento/scripthelper
-Author: Máté Farkas
-Author-email: fm@farkas-mate.hu
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: System Administrators
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Utilities
-Classifier: Typing :: Typed
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# scripthelper
-
-Helper module for simple command line Python scripts.
-
-
-## Basic usage
-
-[example1.py](https://github.com/presidento/scripthelper/blob/master/example1.py):
-
-```python
-#!/usr/bin/env python3
-import scripthelper
-
-logger = scripthelper.bootstrap()
-
-logger.critical("critical message")
-logger.error("error message")
-logger.warning("warning message")
-logger.info("info message")
-logger.verbose("verbose message")
-logger.debug("debug message")
-logger.spam("spam message")
-```
-
-It just works. Try `--verbose` and `--quiet`  command line options, too.
-It uses colored log messages on a terminal.
-See `--help` for more information.
-
-## Adding other command line parameters
-
-[example2.py](https://github.com/presidento/scripthelper/blob/master/example2.py):
-
-```python
-#!/usr/bin/env python3
-import scripthelper
-
-scripthelper.add_argument("-n", "--name", help="Name to greet")
-logger, args = scripthelper.bootstrap_args()
-
-if args.name:
-    logger.debug("Name was provided")
-    logger.info(f"Hello {args.name}")
-else:
-    logger.warning("Name was not provided")
-```
-
-For bigger scripts it is good idea to have the logger at the very beginning, and encapsulate the argument parsing phase, which is typically in the main function:
-
-[example2b.py](https://github.com/presidento/scripthelper/blob/master/example2b.py):
-
-```python
-#!/usr/bin/env python3
-import scripthelper
-
-logger = scripthelper.getLogger(__name__)
-
-def greet(name):
-    logger.info(f"Hello {name}")
-
-def main():
-    scripthelper.add_argument("--name", default="World")
-    args = scripthelper.initialize()
-    greet(args.name)
-
-main()
-```
-
-## Progressbar works with logging, too
-
-[example3.py](https://github.com/presidento/scripthelper/blob/master/example3.py):
-
-```python
-#!/usr/bin/env python3
-import scripthelper
-import time
-
-logger = scripthelper.bootstrap()
-
-logger.info("Doing the calculations...")
-for i in scripthelper.progressbar(range(100)):
-    if i % 20 == 0:
-        logger.verbose(f"Iteration {i}")
-    if i % 5 == 0:
-        logger.debug(f"Iteration {i}")
-    if logger.isEnabledFor(scripthelper.SPAM):
-        logger.spam(f"Iteration {i}")
-    time.sleep(0.01)
-logger.info("Done")
-```
-
-It is automatically disabled on non-tty `stderr` by default.
-
-## Extended log levels can be used in modules
-
-[example4.py](https://github.com/presidento/scripthelper/blob/master/example4.py):
-
-```python
-#!/usr/bin/env python3
-import scripthelper
-import example4module
-
-scripthelper.bootstrap()
-example4module.do_the_things()
-```
-
-[example4module.py](https://github.com/presidento/scripthelper/blob/master/example4module.py):
-
-```python
-#!/usr/bin/env python3
-import scripthelper
-
-logger = scripthelper.getLogger(__name__)
-
-
-def do_the_things():
-    logger.verbose("Calling logger.verbose raises an exception if it does not work.")
-    logger.info("Hello from a module.")
-```
-
-## You can easily preserve logs in files
-
-[example5.py](https://github.com/presidento/scripthelper/blob/master/example5.py):
-
-```python
-#!/usr/bin/env python3
-import scripthelper
-
-logger = scripthelper.bootstrap()
-scripthelper.setup_file_logging()
-
-logger.critical("critical message")
-logger.error("error message")
-logger.warning("warning message")
-logger.info("info message")
-logger.verbose("verbose message")
-logger.debug("debug message")
-logger.spam("spam message")
-```
-
-## It handles exceptions, warnings
-
-[example6.py](https://github.com/presidento/scripthelper/blob/master/example6.py):
-
-```python
-#!/usr/bin/env python3
-import scripthelper
-
-scripthelper.bootstrap()
-
-
-def uncaught_exception_test():
-    this_variable = "will be displayed in stack trace"
-    as_well_as = "the other variables"
-    raise RuntimeError("This exception should be handled.")
-
-
-scripthelper.warn("This user warning will be captured.")
-uncaught_exception_test()
-```
-
-The local variables will be displayed in stack trace, for example:
-
-```
-WARNING C:\***\scripthelper\example6.py:13: UserWarning: This user warning will be captured.
-  scripthelper.warn("This user warning will be captured.")
-
-CRITICAL Uncaught RuntimeError: This exception should be handled.
-Traceback with variables (most recent call last):
-  File "C:\***\scripthelper\example6.py", line 10, in uncaught_exception_test
-    raise RuntimeError("This exception should be handled.")
-      this_variable = 'will be displayed in stack trace'
-      as_well_as = 'the other variables'
-builtins.RuntimeError: This exception should be handled.
-```
-
-## Has built-in colored pretty printer
-
-[example7.py](https://github.com/presidento/scripthelper/blob/master/example7.py):
-
-```python
-#!/usr/bin/env python3
-import scripthelper
-from dataclasses import dataclass
-
-scripthelper.bootstrap()
-
-@dataclass
-class Item:
-    name: str
-    value: int
-
-something = {
-    "string": "value1",
-    "bool": True,
-    "none": None,
-    "integer": 1234,
-    "item": Item("name", 999)
-}
-
-scripthelper.pp(something)
-```
-
-## Has built-in persisted state handler
-
-[example9.py](https://github.com/presidento/scripthelper/blob/master/example9.py):
-
-```python
-#!/usr/bin/env python3
-import scripthelper
-
-logger = scripthelper.bootstrap()
-state = scripthelper.PersistedState(processed_id=0)
-
-state.processed_id += 1
-logger.info(f"Processing item #{state.processed_id}")
-```
-
-```
-$ python example9.py
-INFO Processing item #1
-$ python example9.py
-INFO Processing item #2
-$ python example9.py
-INFO Processing item #3
-```
+Metadata-Version: 2.1
+Name: scripthelper
+Version: 23.3
+Summary: Helper module for creating simple Python scripts
+Project-URL: Homepage, https://github.com/presidento/scripthelper
+Project-URL: Changelog, https://github.com/presidento/scripthelper/blob/main/CHANGELOG.md
+Author-email: Máté Farkas <fm@farkas-mate.hu>
+License: MIT License
+License-File: LICENSE
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: System Administrators
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Utilities
+Classifier: Typing :: Typed
+Requires-Dist: coloredlogs>=10.0
+Requires-Dist: persistedstate>=23.6
+Requires-Dist: prettyprinter>=0.18.0
+Requires-Dist: tqdm>=4.31.1
+Requires-Dist: traceback-with-variables>=2.0.1
+Requires-Dist: verboselogs>=1.7
+Provides-Extra: dev
+Requires-Dist: black; extra == 'dev'
+Requires-Dist: build; extra == 'dev'
+Requires-Dist: mypy; extra == 'dev'
+Requires-Dist: twine; extra == 'dev'
+Description-Content-Type: text/markdown
+
+# scripthelper
+
+Helper module for simple command line Python scripts.
+
+
+## Basic usage
+
+[example1.py](https://github.com/presidento/scripthelper/blob/master/example1.py):
+
+```python
+#!/usr/bin/env python3
+import scripthelper
+
+logger = scripthelper.bootstrap()
+
+logger.critical("critical message")
+logger.error("error message")
+logger.warning("warning message")
+logger.info("info message")
+logger.verbose("verbose message")
+logger.debug("debug message")
+logger.spam("spam message")
+```
+
+It just works. Try `--verbose` and `--quiet`  command line options, too.
+It uses colored log messages on a terminal.
+See `--help` for more information.
+
+## Adding other command line parameters
+
+[example2.py](https://github.com/presidento/scripthelper/blob/master/example2.py):
+
+```python
+#!/usr/bin/env python3
+import scripthelper
+
+scripthelper.add_argument("-n", "--name", help="Name to greet")
+logger, args = scripthelper.bootstrap_args()
+
+if args.name:
+    logger.debug("Name was provided")
+    logger.info(f"Hello {args.name}")
+else:
+    logger.warning("Name was not provided")
+```
+
+For bigger scripts it is good idea to have the logger at the very beginning, and encapsulate the argument parsing phase, which is typically in the main function:
+
+[example2b.py](https://github.com/presidento/scripthelper/blob/master/example2b.py):
+
+```python
+#!/usr/bin/env python3
+import scripthelper
+
+logger = scripthelper.getLogger(__name__)
+
+
+def greet(name):
+    logger.info(f"Hello {name}")
+
+
+def main():
+    scripthelper.add_argument("--name", default="World")
+    args = scripthelper.initialize()
+    greet(args.name)
+
+
+main()
+```
+
+## Progressbar works with logging, too
+
+[example3.py](https://github.com/presidento/scripthelper/blob/master/example3.py):
+
+```python
+#!/usr/bin/env python3
+import scripthelper
+import time
+
+logger = scripthelper.bootstrap()
+
+logger.info("Doing the calculations...")
+for i in scripthelper.progressbar(range(100)):
+    if i % 20 == 0:
+        logger.verbose(f"Iteration {i}")
+    if i % 5 == 0:
+        logger.debug(f"Iteration {i}")
+    if logger.isEnabledFor(scripthelper.SPAM):
+        logger.spam(f"Iteration {i}")
+    time.sleep(0.01)
+logger.info("Done")
+```
+
+It is automatically disabled on non-tty `stderr` by default.
+
+## Extended log levels can be used in modules
+
+[example4.py](https://github.com/presidento/scripthelper/blob/master/example4.py):
+
+```python
+#!/usr/bin/env python3
+import scripthelper
+import example4module
+
+scripthelper.bootstrap()
+example4module.do_the_things()
+```
+
+[example4module.py](https://github.com/presidento/scripthelper/blob/master/example4module.py):
+
+```python
+#!/usr/bin/env python3
+import scripthelper
+
+logger = scripthelper.getLogger(__name__)
+
+
+def do_the_things():
+    logger.verbose("Calling logger.verbose raises an exception if it does not work.")
+    logger.info("Hello from a module.")
+```
+
+## You can easily preserve logs in files
+
+[example5.py](https://github.com/presidento/scripthelper/blob/master/example5.py):
+
+```python
+#!/usr/bin/env python3
+import scripthelper
+
+logger = scripthelper.bootstrap()
+scripthelper.setup_file_logging()
+
+logger.critical("critical message")
+logger.error("error message")
+logger.warning("warning message")
+logger.info("info message")
+logger.verbose("verbose message")
+logger.debug("debug message")
+logger.spam("spam message")
+```
+
+## It handles exceptions, warnings
+
+[example6.py](https://github.com/presidento/scripthelper/blob/master/example6.py):
+
+```python
+#!/usr/bin/env python3
+import scripthelper
+
+scripthelper.bootstrap()
+
+
+def uncaught_exception_test():
+    this_variable = "will be displayed in stack trace"
+    as_well_as = "the other variables"
+    raise RuntimeError("This exception should be handled.")
+
+
+scripthelper.warn("This user warning will be captured.")
+uncaught_exception_test()
+```
+
+The local variables will be displayed in stack trace, for example:
+
+```
+WARNING C:\***\scripthelper\example6.py:13: UserWarning: This user warning will be captured.
+  scripthelper.warn("This user warning will be captured.")
+
+CRITICAL Uncaught RuntimeError: This exception should be handled.
+Traceback with variables (most recent call last):
+  File "C:\***\scripthelper\example6.py", line 10, in uncaught_exception_test
+    raise RuntimeError("This exception should be handled.")
+      this_variable = 'will be displayed in stack trace'
+      as_well_as = 'the other variables'
+builtins.RuntimeError: This exception should be handled.
+```
+
+## Has built-in colored pretty printer
+
+[example7.py](https://github.com/presidento/scripthelper/blob/master/example7.py):
+
+```python
+#!/usr/bin/env python3
+import scripthelper
+from dataclasses import dataclass
+
+scripthelper.bootstrap()
+
+
+@dataclass
+class Item:
+    name: str
+    value: int
+
+
+something = {
+    "string": "value1",
+    "bool": True,
+    "none": None,
+    "integer": 1234,
+    "item": Item("name", 999),
+}
+
+scripthelper.pp(something)
+```
+
+## Has built-in persisted state handler
+
+The state is persisted immediately in the background in YAML. Mutable objects (`list`, `dict`) also can be used.
+
+[example9.py](https://github.com/presidento/scripthelper/blob/master/example9.py):
+
+```python
+#!/usr/bin/env python3
+import scripthelper
+
+logger = scripthelper.bootstrap()
+state = scripthelper.PersistedState(processed_id=0, to_remember=[])
+
+state.processed_id += 1
+state.to_remember.append(f"Element {state.processed_id}")
+while len(state.to_remember) > 2:
+    state.to_remember.pop(0)
+
+logger.info(f"Processing item #{state.processed_id}")
+for item in state.to_remember:
+    logger.info(f"- {item}")
+```
+
+```
+$ python3 example9.py
+INFO Processing item #1
+INFO - Element 1
+
+$ python3 example9.py
+INFO Processing item #2
+INFO - Element 1
+INFO - Element 2
+
+$ python3 example9.py
+INFO Processing item #3
+INFO - Element 2
+INFO - Element 3
+```
+
+## Helps issue a warning only once
+
+[example10.py](https://github.com/presidento/scripthelper/blob/master/example10.py):
+
+```python
+#!/usr/bin/env python3
+import scripthelper
+
+scripthelper.bootstrap()
+
+for _ in range(10):
+    scripthelper.warning_once("Item #12 has some errors")
+```
+
```

