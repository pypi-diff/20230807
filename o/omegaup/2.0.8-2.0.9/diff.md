# Comparing `tmp/omegaup-2.0.8.tar.gz` & `tmp/omegaup-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omegaup-2.0.8.tar", last modified: Sat Nov 12 03:22:42 2022, max compression
+gzip compressed data, was "omegaup-2.0.9.tar", last modified: Sat Nov 12 23:10:00 2022, max compression
```

## Comparing `omegaup-2.0.8.tar` & `omegaup-2.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 03:22:42.566672 omegaup-2.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1515 2022-11-12 03:22:20.000000 omegaup-2.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1403 2022-11-12 03:22:42.566672 omegaup-2.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      871 2022-11-12 03:22:20.000000 omegaup-2.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 03:22:42.566672 omegaup-2.0.8/omegaup/
--rw-r--r--   0 runner    (1001) docker     (121)      454 2022-11-12 03:22:20.000000 omegaup-2.0.8/omegaup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)   689349 2022-11-12 03:22:20.000000 omegaup-2.0.8/omegaup/api.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-12 03:22:20.000000 omegaup-2.0.8/omegaup/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 03:22:42.566672 omegaup-2.0.8/omegaup/validator/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-12 03:22:20.000000 omegaup-2.0.8/omegaup/validator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1473 2022-11-12 03:22:20.000000 omegaup-2.0.8/omegaup/validator/validatortest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 03:22:42.566672 omegaup-2.0.8/omegaup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1403 2022-11-12 03:22:42.000000 omegaup-2.0.8/omegaup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      303 2022-11-12 03:22:42.000000 omegaup-2.0.8/omegaup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-12 03:22:42.000000 omegaup-2.0.8/omegaup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      355 2022-11-12 03:22:42.000000 omegaup-2.0.8/omegaup.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-11-12 03:22:42.000000 omegaup-2.0.8/omegaup.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      923 2022-11-12 03:22:20.000000 omegaup-2.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-12 03:22:42.566672 omegaup-2.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 23:10:00.259204 omegaup-2.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1515 2022-11-12 23:09:40.000000 omegaup-2.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     1403 2022-11-12 23:10:00.259204 omegaup-2.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      871 2022-11-12 23:09:40.000000 omegaup-2.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 23:10:00.259204 omegaup-2.0.9/omegaup/
+-rw-r--r--   0 runner    (1001) docker     (121)      454 2022-11-12 23:09:40.000000 omegaup-2.0.9/omegaup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)   690949 2022-11-12 23:09:40.000000 omegaup-2.0.9/omegaup/api.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-12 23:09:40.000000 omegaup-2.0.9/omegaup/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 23:10:00.259204 omegaup-2.0.9/omegaup/validator/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-12 23:09:40.000000 omegaup-2.0.9/omegaup/validator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1473 2022-11-12 23:09:40.000000 omegaup-2.0.9/omegaup/validator/validatortest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 23:10:00.259204 omegaup-2.0.9/omegaup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1403 2022-11-12 23:10:00.000000 omegaup-2.0.9/omegaup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      303 2022-11-12 23:10:00.000000 omegaup-2.0.9/omegaup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-12 23:10:00.000000 omegaup-2.0.9/omegaup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      355 2022-11-12 23:10:00.000000 omegaup-2.0.9/omegaup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2022-11-12 23:10:00.000000 omegaup-2.0.9/omegaup.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      923 2022-11-12 23:09:40.000000 omegaup-2.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-12 23:10:00.259204 omegaup-2.0.9/setup.cfg
```

### Comparing `omegaup-2.0.8/LICENSE` & `omegaup-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `omegaup-2.0.8/PKG-INFO` & `omegaup-2.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omegaup
-Version: 2.0.8
+Version: 2.0.9
 Summary: Utilities for interacting with omegaUp
 Author-email: omegaUp <lhchavez@omegaup.org>
 Project-URL: Homepage, https://github.com/omegaup/libomegaup
 Project-URL: Bug Tracker, https://github.com/omegaup/libomegaup/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `omegaup-2.0.8/README.md` & `omegaup-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `omegaup-2.0.8/omegaup/api.py` & `omegaup-2.0.9/omegaup/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -10982,21 +10982,25 @@
 class _Run:
     """_Run"""
     alias: str
     classname: str
     contest_alias: Optional[str]
     contest_score: Optional[float]
     country: str
+    execution: Optional[str]
     guid: str
     language: str
     memory: int
+    output: Optional[str]
     penalty: int
     runtime: int
     score: float
     status: str
+    status_memory: Optional[str]
+    status_runtime: Optional[str]
     submit_delay: int
     time: datetime.datetime
     type: Optional[str]
     username: str
     verdict: str
 
     def __init__(
@@ -11014,14 +11018,18 @@
         status: str,
         submit_delay: int,
         time: int,
         username: str,
         verdict: str,
         contest_alias: Optional[str] = None,
         contest_score: Optional[float] = None,
+        execution: Optional[str] = None,
+        output: Optional[str] = None,
+        status_memory: Optional[str] = None,
+        status_runtime: Optional[str] = None,
         type: Optional[str] = None,
         # Ignore any unknown arguments
         **_kwargs: Any,
     ):
         self.alias = alias
         self.classname = classname
         if contest_alias is not None:
@@ -11029,21 +11037,37 @@
         else:
             self.contest_alias = None
         if contest_score is not None:
             self.contest_score = contest_score
         else:
             self.contest_score = None
         self.country = country
+        if execution is not None:
+            self.execution = execution
+        else:
+            self.execution = None
         self.guid = guid
         self.language = language
         self.memory = memory
+        if output is not None:
+            self.output = output
+        else:
+            self.output = None
         self.penalty = penalty
         self.runtime = runtime
         self.score = score
         self.status = status
+        if status_memory is not None:
+            self.status_memory = status_memory
+        else:
+            self.status_memory = None
+        if status_runtime is not None:
+            self.status_runtime = status_runtime
+        else:
+            self.status_runtime = None
         self.submit_delay = submit_delay
         self.time = datetime.datetime.fromtimestamp(time)
         if type is not None:
             self.type = type
         else:
             self.type = None
         self.username = username
@@ -11403,21 +11427,25 @@
     """_RunWithDetails"""
     alias: str
     classname: str
     contest_alias: Optional[str]
     contest_score: Optional[float]
     country: str
     details: Optional['_RunDetailsV2']
+    execution: Optional[str]
     guid: str
     language: str
     memory: int
+    output: Optional[str]
     penalty: int
     runtime: int
     score: float
     status: str
+    status_memory: Optional[str]
+    status_runtime: Optional[str]
     submit_delay: int
     time: datetime.datetime
     type: Optional[str]
     username: str
     verdict: str
 
     def __init__(
@@ -11436,14 +11464,18 @@
         submit_delay: int,
         time: int,
         username: str,
         verdict: str,
         contest_alias: Optional[str] = None,
         contest_score: Optional[float] = None,
         details: Optional[Dict[str, Any]] = None,
+        execution: Optional[str] = None,
+        output: Optional[str] = None,
+        status_memory: Optional[str] = None,
+        status_runtime: Optional[str] = None,
         type: Optional[str] = None,
         # Ignore any unknown arguments
         **_kwargs: Any,
     ):
         self.alias = alias
         self.classname = classname
         if contest_alias is not None:
@@ -11455,21 +11487,37 @@
         else:
             self.contest_score = None
         self.country = country
         if details is not None:
             self.details = _RunDetailsV2(**details)
         else:
             self.details = None
+        if execution is not None:
+            self.execution = execution
+        else:
+            self.execution = None
         self.guid = guid
         self.language = language
         self.memory = memory
+        if output is not None:
+            self.output = output
+        else:
+            self.output = None
         self.penalty = penalty
         self.runtime = runtime
         self.score = score
         self.status = status
+        if status_memory is not None:
+            self.status_memory = status_memory
+        else:
+            self.status_memory = None
+        if status_runtime is not None:
+            self.status_runtime = status_runtime
+        else:
+            self.status_runtime = None
         self.submit_delay = submit_delay
         self.time = datetime.datetime.fromtimestamp(time)
         if type is not None:
             self.type = type
         else:
             self.type = None
         self.username = username
```

### Comparing `omegaup-2.0.8/omegaup/validator/validatortest.py` & `omegaup-2.0.9/omegaup/validator/validatortest.py`

 * *Files identical despite different names*

### Comparing `omegaup-2.0.8/omegaup.egg-info/PKG-INFO` & `omegaup-2.0.9/omegaup.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omegaup
-Version: 2.0.8
+Version: 2.0.9
 Summary: Utilities for interacting with omegaUp
 Author-email: omegaUp <lhchavez@omegaup.org>
 Project-URL: Homepage, https://github.com/omegaup/libomegaup
 Project-URL: Bug Tracker, https://github.com/omegaup/libomegaup/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `omegaup-2.0.8/pyproject.toml` & `omegaup-2.0.9/pyproject.toml`

 * *Files identical despite different names*

