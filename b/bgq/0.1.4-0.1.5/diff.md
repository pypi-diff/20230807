# Comparing `tmp/bgq-0.1.4.tar.gz` & `tmp/bgq-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bgq-0.1.4.tar", max compression
+gzip compressed data, was "bgq-0.1.5.tar", max compression
```

## Comparing `bgq-0.1.4.tar` & `bgq-0.1.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     5511 2023-02-20 22:11:58.266189 bgq-0.1.4/bgq.py
--rw-r--r--   0        0        0     1173 2023-08-05 05:13:31.135955 bgq-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     5327 2023-05-21 23:01:24.047902 bgq-0.1.4/webint_jobs/__init__.py
--rw-r--r--   0        0        0      354 2023-01-27 00:43:31.639971 bgq-0.1.4/webint_jobs/templates/__init__.py
--rw-r--r--   0        0        0      139 2023-01-27 00:43:31.639971 bgq-0.1.4/webint_jobs/templates/by_module.html
--rw-r--r--   0        0        0      620 2023-01-27 00:43:31.647971 bgq-0.1.4/webint_jobs/templates/by_object.html
--rw-r--r--   0        0        0     1064 2023-01-27 00:43:31.643971 bgq-0.1.4/webint_jobs/templates/index.html
--rw-r--r--   0        0        0     1086 2023-01-27 00:43:31.643971 bgq-0.1.4/webint_jobs/templates/job.html
--rw-r--r--   0        0        0     1217 2023-01-27 00:43:31.647971 bgq-0.1.4/webint_jobs/templates/run.html
--rw-r--r--   0        0        0     1040 2023-01-27 00:43:31.639971 bgq-0.1.4/webint_jobs/templates/schedules.html
--rw-r--r--   0        0        0      612 2023-01-27 00:43:31.635971 bgq-0.1.4/webint_jobs/templates/slow.html
--rw-r--r--   0        0        0      966 1970-01-01 00:00:00.000000 bgq-0.1.4/setup.py
--rw-r--r--   0        0        0      738 1970-01-01 00:00:00.000000 bgq-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     5511 2023-08-07 01:20:56.938333 bgq-0.1.5/bgq.py
+-rw-r--r--   0        0        0     1154 2023-08-07 02:14:33.608643 bgq-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     5327 2023-05-21 23:01:24.047902 bgq-0.1.5/webint_jobs/__init__.py
+-rw-r--r--   0        0        0      354 2023-01-27 00:43:31.639971 bgq-0.1.5/webint_jobs/templates/__init__.py
+-rw-r--r--   0        0        0      139 2023-01-27 00:43:31.639971 bgq-0.1.5/webint_jobs/templates/by_module.html
+-rw-r--r--   0        0        0      620 2023-01-27 00:43:31.647971 bgq-0.1.5/webint_jobs/templates/by_object.html
+-rw-r--r--   0        0        0     1064 2023-01-27 00:43:31.643971 bgq-0.1.5/webint_jobs/templates/index.html
+-rw-r--r--   0        0        0     1086 2023-01-27 00:43:31.643971 bgq-0.1.5/webint_jobs/templates/job.html
+-rw-r--r--   0        0        0     1217 2023-01-27 00:43:31.647971 bgq-0.1.5/webint_jobs/templates/run.html
+-rw-r--r--   0        0        0     1040 2023-01-27 00:43:31.639971 bgq-0.1.5/webint_jobs/templates/schedules.html
+-rw-r--r--   0        0        0      612 2023-01-27 00:43:31.635971 bgq-0.1.5/webint_jobs/templates/slow.html
+-rw-r--r--   0        0        0      939 1970-01-01 00:00:00.000000 bgq-0.1.5/setup.py
+-rw-r--r--   0        0        0      697 1970-01-01 00:00:00.000000 bgq-0.1.5/PKG-INFO
```

### Comparing `bgq-0.1.4/bgq.py` & `bgq-0.1.5/bgq.py`

 * *Files identical despite different names*

### Comparing `bgq-0.1.4/pyproject.toml` & `bgq-0.1.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bgq"
-version = "0.1.4"
+version = "0.1.5"
 description = "a simple asynchronous background job queue"
 homepage = "https://ragt.ag/code/projects/bgq"
 repository = "https://ragt.ag/code/projects/bgq.git"
 documentation = "https://ragt.ag/code/projects/bgq/api"
 authors = ["Angelo Gladding <angelo@ragt.ag>"]
 license = "BSD-2-Clause"
 packages = [{include="bgq.py"}, {include="webint_jobs"}]
@@ -16,17 +16,16 @@
 jobs = "webint_jobs:app"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.11"
 sqlyte = ">0.0.50"
 txtint = ">0.0.68"
 webagt = ">0.0.5"
-webint = ">0.0.569"
+webint = ">=0.1.56"
 pendulum = "^2.1.2"
-gevent = "^23.7.0"
 
 [tool.poetry.group.dev.dependencies]
 gmpg = {path="../gmpg", develop=true}
 sqlyte = {path="../sqlyte", develop=true}
 txtint = {path="../txtint", develop=true}
 webagt = {path="../webagt", develop=true}
 webint = {path="../webint", develop=true}
```

### Comparing `bgq-0.1.4/webint_jobs/__init__.py` & `bgq-0.1.5/webint_jobs/__init__.py`

 * *Files identical despite different names*

### Comparing `bgq-0.1.4/webint_jobs/templates/by_object.html` & `bgq-0.1.5/webint_jobs/templates/by_object.html`

 * *Files identical despite different names*

### Comparing `bgq-0.1.4/webint_jobs/templates/index.html` & `bgq-0.1.5/webint_jobs/templates/index.html`

 * *Files identical despite different names*

### Comparing `bgq-0.1.4/webint_jobs/templates/job.html` & `bgq-0.1.5/webint_jobs/templates/job.html`

 * *Files identical despite different names*

### Comparing `bgq-0.1.4/webint_jobs/templates/run.html` & `bgq-0.1.5/webint_jobs/templates/run.html`

 * *Files identical despite different names*

### Comparing `bgq-0.1.4/webint_jobs/templates/schedules.html` & `bgq-0.1.5/webint_jobs/templates/schedules.html`

 * *Files identical despite different names*

### Comparing `bgq-0.1.4/webint_jobs/templates/slow.html` & `bgq-0.1.5/webint_jobs/templates/slow.html`

 * *Files identical despite different names*

### Comparing `bgq-0.1.4/setup.py` & `bgq-0.1.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,27 +6,26 @@
 
 package_data = \
 {'': ['*']}
 
 modules = \
 ['bgq']
 install_requires = \
-['gevent>=23.7.0,<24.0.0',
- 'pendulum>=2.1.2,<3.0.0',
+['pendulum>=2.1.2,<3.0.0',
  'sqlyte>0.0.50',
  'txtint>0.0.68',
  'webagt>0.0.5',
- 'webint>0.0.569']
+ 'webint>=0.1.56']
 
 entry_points = \
 {'console_scripts': ['bgq = bgq:main'], 'webapps': ['jobs = webint_jobs:app']}
 
 setup_kwargs = {
     'name': 'bgq',
-    'version': '0.1.4',
+    'version': '0.1.5',
     'description': 'a simple asynchronous background job queue',
     'long_description': 'None',
     'author': 'Angelo Gladding',
     'author_email': 'angelo@ragt.ag',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://ragt.ag/code/projects/bgq',
```

### Comparing `bgq-0.1.4/PKG-INFO` & `bgq-0.1.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: bgq
-Version: 0.1.4
+Version: 0.1.5
 Summary: a simple asynchronous background job queue
 Home-page: https://ragt.ag/code/projects/bgq
 License: BSD-2-Clause
 Author: Angelo Gladding
 Author-email: angelo@ragt.ag
 Requires-Python: >=3.10,<3.11
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: gevent (>=23.7.0,<24.0.0)
 Requires-Dist: pendulum (>=2.1.2,<3.0.0)
 Requires-Dist: sqlyte (>0.0.50)
 Requires-Dist: txtint (>0.0.68)
 Requires-Dist: webagt (>0.0.5)
-Requires-Dist: webint (>0.0.569)
+Requires-Dist: webint (>=0.1.56)
 Project-URL: Documentation, https://ragt.ag/code/projects/bgq/api
 Project-URL: Repository, https://ragt.ag/code/projects/bgq.git
```

