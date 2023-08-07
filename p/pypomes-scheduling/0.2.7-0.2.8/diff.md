# Comparing `tmp/pypomes_scheduling-0.2.7.tar.gz` & `tmp/pypomes_scheduling-0.2.8.tar.gz`

## Comparing `pypomes_scheduling-0.2.7.tar` & `pypomes_scheduling-0.2.8.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.7/src/pypomes_scheduling/__init__.py
--rw-r--r--   0        0        0     9751 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.7/src/pypomes_scheduling/scheduling_pomes.py
--rw-r--r--   0        0        0     4748 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.7/src/pypomes_scheduling/threaded_scheduler.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.7/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.7/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.7/README.md
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.7/pyproject.toml
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.8/src/pypomes_scheduling/__init__.py
+-rw-r--r--   0        0        0    10037 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.8/src/pypomes_scheduling/scheduling_pomes.py
+-rw-r--r--   0        0        0     4748 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.8/src/pypomes_scheduling/threaded_scheduler.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.8/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.8/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.8/README.md
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.8/PKG-INFO
```

### Comparing `pypomes_scheduling-0.2.7/src/pypomes_scheduling/scheduling_pomes.py` & `pypomes_scheduling-0.2.8/src/pypomes_scheduling/scheduling_pomes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-from datetime import datetime
-from pypomes_core import exc_format
-from typing import Final
 import logging
 import pytz
 import re
 import sys
+from datetime import datetime
+from pypomes_core import APP_PREFIX, TIMEZONE_LOCAL, env_get_int, exc_format
+from typing import Final
 from .threaded_scheduler import _ThreadedScheduler
 
+SCHEDULER_RETRY_INTERVAL: Final[int] = env_get_int(f"{APP_PREFIX}_SCHEDULER_RETRY_INTERVAL", 10)
+
 __DEFAULT_BADGE: Final[str] = "__default__"
 
 __REGEX_VERIFY_CRON: Final[str] = (
     "/(@(annually|yearly|monthly|weekly|daily|hourly|reboot))|"
     "(@every (\d+(ns|us|µs|ms|s|m|h))+)|((((\d+,)+\d+|(\d+(\/|-)\d+)|\d+|\*) ?){5,7})"
 )
 
@@ -18,24 +20,25 @@
 #   <{ <badge-1>: <scheduler-instance-1>,
 #     ...
 #     <badge-n>: <scheduler-instance-n>
 #   }>
 __schedulers: dict = {}
 
 
-def scheduler_create(errors: list[str], timezone: pytz.BaseTzInfo,
-                     retry_interval: int, logger: logging.Logger = None, badge: str = None) -> bool:
+def scheduler_create(errors: list[str], timezone: pytz.BaseTzInfo = TIMEZONE_LOCAL,
+                     retry_interval: int = SCHEDULER_RETRY_INTERVAL,
+                     logger: logging.Logger = None, badge: str = None) -> bool:
     """
     Create the threaded job scheduler.
 
     This is a wrapper around the package *APScheduler*.
 
     :param errors: incidental errors
-    :param timezone: the timezone to be used
-    :param retry_interval: interval between retry attempts, in minutes
+    :param timezone: the timezone to be used (defaults to the configured local timezone)
+    :param retry_interval: interval between retry attempts, in minutes (defaults to the configured value)
     :param logger: optional logger object
     :param badge: optional badge identifying the scheduler
     :return: True if the scheduler was created, or False otherwise
     """
     # inicialize the return variable
     result: bool = False
```

### Comparing `pypomes_scheduling-0.2.7/src/pypomes_scheduling/threaded_scheduler.py` & `pypomes_scheduling-0.2.8/src/pypomes_scheduling/threaded_scheduler.py`

 * *Files identical despite different names*

### Comparing `pypomes_scheduling-0.2.7/LICENSE` & `pypomes_scheduling-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_scheduling-0.2.7/pyproject.toml` & `pypomes_scheduling-0.2.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 requires = [
     "hatchling"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_scheduling"
-version = "0.2.7"
+version = "0.2.8"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (scheduling module)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
 ]
 dependencies = [
     "pip>=23.2.1",
-    "pypomes_core>=0.2.3",
+    "pypomes_core>=0.2.5",
     "APScheduler>=3.10.1",
     "setuptools>=68.0.0",
     "wheel>=0.41.0"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/TheWiseCoder/PyPomes-Scheduling"
```

### Comparing `pypomes_scheduling-0.2.7/PKG-INFO` & `pypomes_scheduling-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: pypomes_scheduling
-Version: 0.2.7
+Version: 0.2.8
 Summary: A collection of Python pomes, pennyeach (scheduling module)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-Scheduling
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-Scheduling/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: apscheduler>=3.10.1
 Requires-Dist: pip>=23.2.1
-Requires-Dist: pypomes-core>=0.2.3
+Requires-Dist: pypomes-core>=0.2.5
 Requires-Dist: setuptools>=68.0.0
 Requires-Dist: wheel>=0.41.0
```

