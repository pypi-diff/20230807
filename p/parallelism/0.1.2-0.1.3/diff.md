# Comparing `tmp/parallelism-0.1.2.tar.gz` & `tmp/parallelism-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parallelism-0.1.2.tar", last modified: Sat Aug  5 13:32:31 2023, max compression
+gzip compressed data, was "parallelism-0.1.3.tar", last modified: Sun Aug  6 23:20:26 2023, max compression
```

## Comparing `parallelism-0.1.2.tar` & `parallelism-0.1.3.tar`

### file list

```diff
@@ -1,45 +1,48 @@
-drwxrwxrwx   0        0        0        0 2023-08-05 13:32:31.103814 parallelism-0.1.2/
--rw-rw-rw-   0        0        0     3238 2023-07-28 18:24:12.000000 parallelism-0.1.2/.gitignore
--rw-rw-rw-   0        0        0      115 2023-07-29 07:17:10.000000 parallelism-0.1.2/.readthedocs.yaml
--rw-rw-rw-   0        0        0     1088 2023-07-28 18:24:12.000000 parallelism-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     2710 2023-08-05 13:32:31.103814 parallelism-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2090 2023-08-05 13:30:29.000000 parallelism-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-08-05 13:32:30.963221 parallelism-0.1.2/docs/
-drwxrwxrwx   0        0        0        0 2023-08-05 13:32:30.978841 parallelism-0.1.2/docs/api_reference/
--rw-rw-rw-   0        0        0     6550 2023-08-04 23:52:47.000000 parallelism-0.1.2/docs/api_reference/scheduled_task.rst
--rw-rw-rw-   0        0        0     9746 2023-08-05 12:39:04.000000 parallelism-0.1.2/docs/api_reference/task_scheduler.rst
--rw-rw-rw-   0        0        0      341 2023-07-29 11:22:19.000000 parallelism-0.1.2/docs/conf.py
--rw-rw-rw-   0        0        0     1367 2023-08-05 13:30:29.000000 parallelism-0.1.2/docs/index.rst
-drwxrwxrwx   0        0        0        0 2023-08-05 13:32:30.994462 parallelism-0.1.2/parallelism/
--rw-rw-rw-   0        0        0      296 2023-08-05 13:31:54.000000 parallelism-0.1.2/parallelism/__init__.py
--rw-rw-rw-   0        0        0     8668 2023-08-04 22:27:47.000000 parallelism-0.1.2/parallelism/api_reference.py
--rw-rw-rw-   0        0        0      395 2023-07-17 16:01:03.000000 parallelism-0.1.2/parallelism/config.py
-drwxrwxrwx   0        0        0        0 2023-08-05 13:32:31.041340 parallelism-0.1.2/parallelism/core/
--rw-rw-rw-   0        0        0        0 2023-07-10 17:22:05.000000 parallelism-0.1.2/parallelism/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-05 13:32:31.056983 parallelism-0.1.2/parallelism/core/exceptions/
--rw-rw-rw-   0        0        0        0 2023-07-14 23:41:33.000000 parallelism-0.1.2/parallelism/core/exceptions/__init__.py
--rw-rw-rw-   0        0        0      369 2023-07-14 23:57:59.000000 parallelism-0.1.2/parallelism/core/exceptions/dependency_error.py
--rw-rw-rw-   0        0        0      333 2023-07-28 10:57:43.000000 parallelism-0.1.2/parallelism/core/exceptions/worker_error.py
-drwxrwxrwx   0        0        0        0 2023-08-05 13:32:31.072570 parallelism-0.1.2/parallelism/core/executors/
--rw-rw-rw-   0        0        0        0 2023-07-10 17:30:09.000000 parallelism-0.1.2/parallelism/core/executors/__init__.py
--rw-rw-rw-   0        0        0     1474 2023-07-13 20:44:05.000000 parallelism-0.1.2/parallelism/core/executors/process_executor.py
--rw-rw-rw-   0        0        0      890 2023-07-10 17:35:23.000000 parallelism-0.1.2/parallelism/core/executors/thread_executor.py
-drwxrwxrwx   0        0        0        0 2023-08-05 13:32:31.103814 parallelism-0.1.2/parallelism/core/handlers/
--rw-rw-rw-   0        0        0        0 2023-07-13 20:15:30.000000 parallelism-0.1.2/parallelism/core/handlers/__init__.py
--rw-rw-rw-   0        0        0     3209 2023-07-29 17:55:18.000000 parallelism-0.1.2/parallelism/core/handlers/dependency_handler.py
--rw-rw-rw-   0        0        0     7063 2023-08-05 00:35:04.000000 parallelism-0.1.2/parallelism/core/handlers/function_handler.py
--rw-rw-rw-   0        0        0     2124 2023-07-21 23:15:08.000000 parallelism-0.1.2/parallelism/core/handlers/parameters_handler.py
--rw-rw-rw-   0        0        0     3778 2023-08-05 00:37:16.000000 parallelism-0.1.2/parallelism/core/handlers/shared_memory_handler.py
--rw-rw-rw-   0        0        0      344 2023-08-04 11:42:19.000000 parallelism-0.1.2/parallelism/core/raise_exception.py
--rw-rw-rw-   0        0        0     1275 2023-08-02 21:46:54.000000 parallelism-0.1.2/parallelism/core/return_value.py
--rw-rw-rw-   0        0        0     3182 2023-08-02 21:46:54.000000 parallelism-0.1.2/parallelism/core/scheduled_task.py
--rw-rw-rw-   0        0        0      474 2023-08-04 11:46:52.000000 parallelism-0.1.2/parallelism/core/scheduler_result.py
--rw-rw-rw-   0        0        0     7203 2023-08-04 11:48:06.000000 parallelism-0.1.2/parallelism/core/task_scheduler.py
--rw-rw-rw-   0        0        0      506 2023-07-14 10:52:01.000000 parallelism-0.1.2/parallelism/logger.py
-drwxrwxrwx   0        0        0        0 2023-08-05 13:32:31.010088 parallelism-0.1.2/parallelism.egg-info/
--rw-rw-rw-   0        0        0     2710 2023-08-05 13:32:30.000000 parallelism-0.1.2/parallelism.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1102 2023-08-05 13:32:30.000000 parallelism-0.1.2/parallelism.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-05 13:32:30.000000 parallelism-0.1.2/parallelism.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-08-05 13:32:30.000000 parallelism-0.1.2/parallelism.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      851 2023-07-28 19:13:04.000000 parallelism-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-05 13:32:31.103814 parallelism-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-06 23:20:26.211015 parallelism-0.1.3/
+-rw-rw-rw-   0        0        0     3238 2023-07-28 18:24:12.000000 parallelism-0.1.3/.gitignore
+-rw-rw-rw-   0        0        0      115 2023-07-29 07:17:10.000000 parallelism-0.1.3/.readthedocs.yaml
+-rw-rw-rw-   0        0        0     1088 2023-07-28 18:24:12.000000 parallelism-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     3077 2023-08-06 23:20:26.211015 parallelism-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2090 2023-08-05 13:30:29.000000 parallelism-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-08-06 23:20:26.117286 parallelism-0.1.3/docs/
+drwxrwxrwx   0        0        0        0 2023-08-06 23:20:26.117286 parallelism-0.1.3/docs/api_reference/
+-rw-rw-rw-   0        0        0     7338 2023-08-06 22:53:29.000000 parallelism-0.1.3/docs/api_reference/scheduled_task.rst
+-rw-rw-rw-   0        0        0    10368 2023-08-06 22:53:29.000000 parallelism-0.1.3/docs/api_reference/task_scheduler.rst
+-rw-rw-rw-   0        0        0      341 2023-07-29 11:22:19.000000 parallelism-0.1.3/docs/conf.py
+-rw-rw-rw-   0        0        0     1367 2023-08-05 13:30:29.000000 parallelism-0.1.3/docs/index.rst
+drwxrwxrwx   0        0        0        0 2023-08-06 23:20:26.132907 parallelism-0.1.3/parallelism/
+-rw-rw-rw-   0        0        0      296 2023-08-06 22:54:13.000000 parallelism-0.1.3/parallelism/__init__.py
+-rw-rw-rw-   0        0        0    13454 2023-08-06 22:01:09.000000 parallelism-0.1.3/parallelism/api_reference.py
+-rw-rw-rw-   0        0        0      395 2023-07-17 16:01:03.000000 parallelism-0.1.3/parallelism/config.py
+drwxrwxrwx   0        0        0        0 2023-08-06 23:20:26.179772 parallelism-0.1.3/parallelism/core/
+-rw-rw-rw-   0        0        0        0 2023-07-10 17:22:05.000000 parallelism-0.1.3/parallelism/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-06 23:20:26.195393 parallelism-0.1.3/parallelism/core/exceptions/
+-rw-rw-rw-   0        0        0        0 2023-07-14 23:41:33.000000 parallelism-0.1.3/parallelism/core/exceptions/__init__.py
+-rw-rw-rw-   0        0        0      369 2023-07-14 23:57:59.000000 parallelism-0.1.3/parallelism/core/exceptions/dependency_error.py
+-rw-rw-rw-   0        0        0      798 2023-08-06 21:37:46.000000 parallelism-0.1.3/parallelism/core/exceptions/resource_error.py
+-rw-rw-rw-   0        0        0      333 2023-07-28 10:57:43.000000 parallelism-0.1.3/parallelism/core/exceptions/worker_error.py
+drwxrwxrwx   0        0        0        0 2023-08-06 23:20:26.195393 parallelism-0.1.3/parallelism/core/executors/
+-rw-rw-rw-   0        0        0        0 2023-07-10 17:30:09.000000 parallelism-0.1.3/parallelism/core/executors/__init__.py
+-rw-rw-rw-   0        0        0     1474 2023-07-13 20:44:05.000000 parallelism-0.1.3/parallelism/core/executors/process_executor.py
+-rw-rw-rw-   0        0        0      890 2023-07-10 17:35:23.000000 parallelism-0.1.3/parallelism/core/executors/thread_executor.py
+drwxrwxrwx   0        0        0        0 2023-08-06 23:20:26.211015 parallelism-0.1.3/parallelism/core/handlers/
+-rw-rw-rw-   0        0        0        0 2023-07-13 20:15:30.000000 parallelism-0.1.3/parallelism/core/handlers/__init__.py
+-rw-rw-rw-   0        0        0     3209 2023-07-29 17:55:18.000000 parallelism-0.1.3/parallelism/core/handlers/dependency_handler.py
+-rw-rw-rw-   0        0        0    10141 2023-08-06 21:40:59.000000 parallelism-0.1.3/parallelism/core/handlers/function_handler.py
+-rw-rw-rw-   0        0        0     2124 2023-07-21 23:15:08.000000 parallelism-0.1.3/parallelism/core/handlers/parameters_handler.py
+-rw-rw-rw-   0        0        0     2407 2023-08-06 20:49:03.000000 parallelism-0.1.3/parallelism/core/handlers/resource_handler.py
+-rw-rw-rw-   0        0        0     4002 2023-08-06 21:16:25.000000 parallelism-0.1.3/parallelism/core/handlers/shared_memory_handler.py
+-rw-rw-rw-   0        0        0     2250 2023-08-06 19:36:43.000000 parallelism-0.1.3/parallelism/core/handlers/worker_handler.py
+-rw-rw-rw-   0        0        0      344 2023-08-04 11:42:19.000000 parallelism-0.1.3/parallelism/core/raise_exception.py
+-rw-rw-rw-   0        0        0     1275 2023-08-02 21:46:54.000000 parallelism-0.1.3/parallelism/core/return_value.py
+-rw-rw-rw-   0        0        0     3612 2023-08-06 21:16:25.000000 parallelism-0.1.3/parallelism/core/scheduled_task.py
+-rw-rw-rw-   0        0        0      474 2023-08-04 11:46:52.000000 parallelism-0.1.3/parallelism/core/scheduler_result.py
+-rw-rw-rw-   0        0        0     8194 2023-08-06 21:16:25.000000 parallelism-0.1.3/parallelism/core/task_scheduler.py
+-rw-rw-rw-   0        0        0      506 2023-07-14 10:52:01.000000 parallelism-0.1.3/parallelism/logger.py
+drwxrwxrwx   0        0        0        0 2023-08-06 23:20:26.179772 parallelism-0.1.3/parallelism.egg-info/
+-rw-rw-rw-   0        0        0     3077 2023-08-06 23:20:25.000000 parallelism-0.1.3/parallelism.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1238 2023-08-06 23:20:26.000000 parallelism-0.1.3/parallelism.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-06 23:20:25.000000 parallelism-0.1.3/parallelism.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-08-06 23:20:25.000000 parallelism-0.1.3/parallelism.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1186 2023-08-06 23:18:08.000000 parallelism-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-06 23:20:26.211015 parallelism-0.1.3/setup.cfg
```

### Comparing `parallelism-0.1.2/.gitignore` & `parallelism-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `parallelism-0.1.2/LICENSE` & `parallelism-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `parallelism-0.1.2/PKG-INFO` & `parallelism-0.1.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 Metadata-Version: 2.1
 Name: parallelism
-Version: 0.1.2
-Summary: Empowering workflows with parallelism
+Version: 0.1.3
+Summary: Enhance Parallel Task Execution
 Author: Idan Hazan
 License: MIT
 Project-URL: homepage, https://github.com/idanhazan/parallelism
 Project-URL: repository, https://github.com/idanhazan/parallelism
 Project-URL: documentation, https://parallelism.readthedocs.io
-Keywords: parallelism,parallel,task,scheduler
-Classifier: Programming Language :: Python :: 3
+Keywords: parallelism,parallel,scheduled,task,scheduler
+Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.11
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # parallelism
 
 The Parallelism library offers a powerful set of tools for managing concurrent task execution using both processes and threads.
 It aims to simplify the development of parallel programs, providing a higher-level interface for distributing tasks across multiple execution units.
```

### Comparing `parallelism-0.1.2/README.md` & `parallelism-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `parallelism-0.1.2/docs/api_reference/scheduled_task.rst` & `parallelism-0.1.3/docs/api_reference/scheduled_task.rst`

 * *Files 7% similar despite different names*

```diff
@@ -183,14 +183,31 @@
 ...     with ProcessPoolExecutor(max_workers=2) as executor:
 ...         pass
 ...     with ThreadPoolExecutor(max_workers=4) as executor:
 ...         pass
 ...
 >>> p = scheduled_task(Process, 'p', func, processes=2, threads=4)
 
+Processor & Memory
+******************
+
+Resource Usage Estimation:
+
+In the following use cases, the `scheduled_task` function incorporates the estimation of system resources to enhance task execution efficiency.
+The parameters `system_processor`, `system_memory`, `graphics_processor`, and `graphics_memory` allow you to specify the estimated resource usage for each task,
+ensuring optimized resource allocation within the system.
+
+By estimating 60.5% system processor and 75% system memory usage, these tasks are unable to run concurrently due to resource limitations.
+
+>>> def func():
+...     pass
+...
+>>> p = scheduled_task(Process, 'p', func, system_processor=60.5, system_memory=75)
+>>> t = scheduled_task(Thread, 't', func, system_processor=60.5, system_memory=75)
+
 Continual
 *********
 
 Storing Task Return Values:
 
 This example illustrates how to manage stored return values.
 `p`'s return value is stored due to the `continual=True` parameter, while `t`'s return value is not stored.
```

### Comparing `parallelism-0.1.2/docs/api_reference/task_scheduler.rst` & `parallelism-0.1.3/docs/api_reference/task_scheduler.rst`

 * *Files 4% similar despite different names*

```diff
@@ -169,59 +169,67 @@
 ...     return a / b
 ...
 >>> def func2(x):
 ...     print(f'func2(x={x})\n', end='')
 ...     return x
 ...
 >>> p1 = scheduled_task(Process, 'p1', func1, (5, 2))
->>> p2 = scheduled_task(Process, 'p2', func1, (3, 0))
->>> p3 = scheduled_task(Process, 'p3', func1, (9, 0), processes=2)
->>> p4 = scheduled_task(Process, 'p4', func1, (7, 2))
+>>> p2 = scheduled_task(Process, 'p2', func1, (6, 0))
+>>> p3 = scheduled_task(Process, 'p3', func1, (6, 0), processes=2)
+>>> p4 = scheduled_task(Process, 'p4', func1, (6, 0), system_processor=12.6, system_memory=34.7)
+>>> p5 = scheduled_task(Process, 'p5', func1, (7, 2))
 >>> t1 = scheduled_task(Thread, 't1', func2, (p1.return_value,), continual=True)
 >>> t2 = scheduled_task(Thread, 't2', func2, (p2.return_value,), continual=True)
 >>> t3 = scheduled_task(Thread, 't3', func2, (p3.return_value,), continual=True)
 >>> t4 = scheduled_task(Thread, 't4', func2, (p4.return_value,), continual=True)
->>> s1 = task_scheduler(tasks=(p1, p2, p3, p4, t1, t2, t3, t4), processes=2, threads=2)
+>>> t5 = scheduled_task(Thread, 't5', func2, (p5.return_value,), continual=True)
+>>> s1 = task_scheduler(tasks=(p1, p2, p3, p4, p5, t1, t2, t3, t4, t5), processes=2, threads=2, system_processor=10, system_memory=25)
 TIMESTAMP [WARNING] [parallelism:PID:TID] - 'p3' is being canceled, due to lack of 1 process
-TIMESTAMP [WARNING] [parallelism:PID:TID] - 't3' is being canceled, due to task 'p3'
+TIMESTAMP [WARNING] [parallelism:PID:TID] - 'p4' is being canceled, due to lack of 2.6% CPU and 9.7% RAM
 func1(a=5, b=2)                           # Task 'p1' has been started
-func1(a=3, b=0)                           # Task 'p2' has been started
+func1(a=6, b=0)                           # Task 'p2' has been started
+TIMESTAMP [WARNING] [parallelism:PID:TID] - 't3' is being canceled, due to task 'p3'
+TIMESTAMP [WARNING] [parallelism:PID:TID] - 't4' is being canceled, due to task 'p4'
 TIMESTAMP [INFO] [parallelism:PID:TID]    - 'p1' ran approximately ... nanoseconds
-func1(a=7, b=2)                           # Task 'p4' has been started
+func1(a=7, b=2)                           # Task 'p5' has been started
 func2(x=2.5)                              # Task 't1' has been started
 TIMESTAMP [ERROR] [parallelism:PID:TID]   - 'p2' ran approximately ... microseconds - ZeroDivisionError('division by zero')
 TIMESTAMP [WARNING] [parallelism:PID:TID] - 't2' is being canceled, due to task 'p2'
-TIMESTAMP [INFO] [parallelism:PID:TID]    - 'p4' ran approximately ... nanoseconds
-func2(x=3.5)                              # Task 't4' has been started
+TIMESTAMP [INFO] [parallelism:PID:TID]    - 'p5' ran approximately ... nanoseconds
+func2(x=3.5)                              # Task 't5' has been started
 TIMESTAMP [INFO] [parallelism:PID:TID]    - 't1' ran approximately ... nanoseconds
-TIMESTAMP [INFO] [parallelism:PID:TID]    - 't4' ran approximately ... nanoseconds
+TIMESTAMP [INFO] [parallelism:PID:TID]    - 't5' ran approximately ... nanoseconds
 >>> s1.execution_time
 {
     'p3': datetime.datetime(...),
-    't3': datetime.datetime(...),
+    'p4': datetime.datetime(...),
     'p1': datetime.datetime(...),
     'p2': datetime.datetime(...),
-    't2': datetime.datetime(...),
-    'p4': datetime.datetime(...),
-    't1': datetime.datetime(...),
+    't3': datetime.datetime(...),
     't4': datetime.datetime(...),
+    'p5': datetime.datetime(...),
+    't1': datetime.datetime(...),
+    't2': datetime.datetime(...),
+    't5': datetime.datetime(...),
 }
 >>> s1.elapsed_time
 {
     'p1': float(...),
     'p2': float(...),
-    'p4': float(...),
+    'p5': float(...),
     't1': float(...),
-    't4': float(...),
+    't5': float(...),
 }
 >>> s1.raise_exception
 {
     'p3': WorkerError("'p3' has been canceled", (1, 0)),
-    't3': DependencyError("'t3' has been canceled", ('p3',)),
+    'p4': ResourceError("'p4' has been canceled", (2.6, 9.7, 0, 0)),
     'p2': ZeroDivisionError('division by zero'),
-    't2': DependencyError("'t3' has been canceled", ('p2',)),
+    't3': DependencyError("'t3' has been canceled", ('p3',)),
+    't4': DependencyError("'t4' has been canceled", ('p4',)),
+    't2': DependencyError("'t2' has been canceled", ('p2',)),
 }
 >>> s1.return_value
 {
     't1': 2.5,
-    't4': 3.5,
+    't5': 3.5,
 }
```

### Comparing `parallelism-0.1.2/docs/index.rst` & `parallelism-0.1.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `parallelism-0.1.2/parallelism/core/executors/process_executor.py` & `parallelism-0.1.3/parallelism/core/executors/process_executor.py`

 * *Files identical despite different names*

### Comparing `parallelism-0.1.2/parallelism/core/executors/thread_executor.py` & `parallelism-0.1.3/parallelism/core/executors/thread_executor.py`

 * *Files identical despite different names*

### Comparing `parallelism-0.1.2/parallelism/core/handlers/dependency_handler.py` & `parallelism-0.1.3/parallelism/core/handlers/dependency_handler.py`

 * *Files identical despite different names*

### Comparing `parallelism-0.1.2/parallelism/core/handlers/parameters_handler.py` & `parallelism-0.1.3/parallelism/core/handlers/parameters_handler.py`

 * *Files identical despite different names*

### Comparing `parallelism-0.1.2/parallelism/core/handlers/shared_memory_handler.py` & `parallelism-0.1.3/parallelism/core/handlers/shared_memory_handler.py`

 * *Files 7% similar despite different names*

```diff
@@ -55,14 +55,18 @@
                 target=task.target,
                 args=(),
                 kwargs={},
                 dependencies=task.dependencies,
                 priority=task.priority,
                 processes=task.processes,
                 threads=task.threads,
+                system_processor=task.system_processor,
+                system_memory=task.system_memory,
+                graphics_processor=task.graphics_processor,
+                graphics_memory=task.graphics_memory,
                 continual=task.continual,
                 initialized=task.initialized,
             )
             del self.proxy[task.name]['execution_time']
             del self.proxy[task.name]['elapsed_time']
             del self.proxy[task.name]['raise_exception']
             del self.proxy[task.name]['return_value']
```

### Comparing `parallelism-0.1.2/parallelism/core/return_value.py` & `parallelism-0.1.3/parallelism/core/return_value.py`

 * *Files identical despite different names*

### Comparing `parallelism-0.1.2/parallelism/core/scheduled_task.py` & `parallelism-0.1.3/parallelism/core/scheduled_task.py`

 * *Files 20% similar despite different names*

```diff
@@ -23,14 +23,18 @@
     target: Callable[..., Any]
     args: Tuple[Any, ...]
     kwargs: Dict[str, Any]
     dependencies: Tuple[ScheduledTask, ...]
     priority: Union[int, float]
     processes: int
     threads: int
+    system_processor: Union[int, float]
+    system_memory: Union[int, float]
+    graphics_processor: Union[int, float]
+    graphics_memory: Union[int, float]
     continual: bool
     initialized: bool
 
     def __hash__(self) -> int:
         return hash(self.name)
 
     def __eq__(self, other: ScheduledTask) -> bool:
@@ -43,14 +47,18 @@
             'target={!r}'.format(self.reformat_target),
             'args={!r}'.format(self.amount_of_args),
             'kwargs={!r}'.format(self.amount_of_kwargs),
             'dependencies={!r}'.format(self.amount_of_dependencies),
             'priority={!r}'.format(self.priority),
             'processes={!r}'.format(self.processes),
             'threads={!r}'.format(self.threads),
+            'system_processor={!r}'.format(self.system_processor),
+            'system_memory={!r}'.format(self.system_memory),
+            'graphics_processor={!r}'.format(self.graphics_processor),
+            'graphics_memory={!r}'.format(self.graphics_memory),
             'continual={!r}'.format(self.continual),
         )
         parameters = ', '.join(parameters)
         return f'{self.__class__.__name__}({parameters})'
 
     @property
     def reformat_executor(self) -> str:
```

### Comparing `parallelism-0.1.2/parallelism/core/task_scheduler.py` & `parallelism-0.1.3/parallelism/core/task_scheduler.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,106 +3,119 @@
 from multiprocessing import Manager, Process
 from threading import Thread
 from typing import TYPE_CHECKING
 
 from parallelism.core.handlers.dependency_handler import DependencyHandler
 from parallelism.core.handlers.function_handler import FunctionHandler
 from parallelism.core.handlers.parameters_handler import ParametersHandler
+from parallelism.core.handlers.resource_handler import ResourceHandler
 from parallelism.core.handlers.shared_memory_handler import SharedMemoryHandler
+from parallelism.core.handlers.worker_handler import WorkerHandler
 from parallelism.core.scheduled_task import ScheduledTask
 from parallelism.core.scheduler_result import SchedulerResult
 
 if TYPE_CHECKING:
-    from typing import Literal, Tuple
+    from typing import Literal, Tuple, Union
 
 __all__ = ('TaskScheduler',)
 
 
 class TaskScheduler:
     __slots__ = (
         'tasks',
         'returns',
         'processes',
         'threads',
+        'system_processor',
+        'system_memory',
+        'graphics_processor',
+        'graphics_memory',
         'manager',
         'proxy',
+        'worker_handler',
+        'resource_handler',
         'dependency_handler',
         'shared_memory_handler',
     )
 
     def __init__(
         self,
         tasks: Tuple[ScheduledTask, ...],
         processes: int,
         threads: int,
+        system_processor: Union[int, float],
+        system_memory: Union[int, float],
+        graphics_processor: Union[int, float],
+        graphics_memory: Union[int, float],
     ) -> None:
         self.tasks = sorted(tasks, key=lambda task: task.priority)
         self.processes = processes
         self.threads = threads
+        self.system_processor = system_processor
+        self.system_memory = system_memory
+        self.graphics_processor = graphics_processor
+        self.graphics_memory = graphics_memory
         self.manager = None
         self.proxy = None
+        self.worker_handler = None
+        self.resource_handler = None
         self.dependency_handler = None
         self.shared_memory_handler = None
 
     @property
     def finished(self) -> bool:
         return all(
             task.initialized and
             self.proxy.get(task.name).get('finish')
             for task in self.tasks
         )
 
-    @property
-    def active_tasks(self) -> Tuple[ScheduledTask, ...]:
-        return tuple(
-            task for task in self.tasks
-            if (
-                task.initialized and
-                self.proxy.get(task.name).get('start') and not
-                self.proxy.get(task.name).get('finish')
-            )
-        )
-
-    @property
-    def active_processes(self) -> int:
-        return sum(
-            task.processes + (1 if isinstance(task.executor, Process) else 0)
-            for task in self.active_tasks
-        )
-
-    @property
-    def active_threads(self) -> int:
-        return sum(
-            task.threads + 1 if isinstance(task.executor, Thread) else 0
-            for task in self.active_tasks
-        )
-
     def execute(self) -> SchedulerResult:
         self.manager = Manager()
         self.proxy = self.manager.dict()
+        self.worker_handler = WorkerHandler(
+            tasks=self.tasks,
+            proxy=self.proxy,
+            processes=self.processes,
+            threads=self.threads,
+        )
+        self.resource_handler = ResourceHandler(
+            tasks=self.tasks,
+            proxy=self.proxy,
+            system_processor=self.system_processor,
+            system_memory=self.system_memory,
+            graphics_processor=self.graphics_processor,
+            graphics_memory=self.graphics_memory,
+        )
         self.dependency_handler = DependencyHandler(
             tasks=self.tasks,
             proxy=self.proxy,
         )
         self.shared_memory_handler = SharedMemoryHandler(
             tasks=self.tasks,
             proxy=self.proxy,
             prerequisites=self.dependency_handler.prerequisites,
         )
         for index, task in enumerate(self.tasks):
-            if not self.enough_workers(task):
+            if not self.worker_handler.enough_workers(task):
                 self.proxy[task.name] = self.manager.dict()
                 task = self.initialize(task, blocked='worker')
                 self.tasks[index] = task
+            if not self.resource_handler.enough_resources(task):
+                self.proxy[task.name] = self.manager.dict()
+                task = self.initialize(task, blocked='resource')
+                self.tasks[index] = task
         while not self.finished:
             for index, task in enumerate(self.tasks):
                 if task.initialized:
                     self.shared_memory_handler.free(index, task)
                     continue
-                if not self.available_worker(task):
+                if not self.resource_handler.enough_resources(task):
+                    continue
+                if not self.worker_handler.available_worker(task):
                     continue
                 if self.dependency_handler.is_blocked(task, status='finish'):
                     continue
                 if self.dependency_handler.is_blocked(task, status='complete'):
                     self.proxy[task.name] = self.manager.dict()
                     task = self.initialize(task, blocked='dependency')
                     self.tasks[index] = task
@@ -122,32 +135,48 @@
             self.shared_memory_handler.raise_exception,
             self.shared_memory_handler.return_value,
         )
 
     def initialize(
         self,
         task: ScheduledTask,
-        blocked: Literal['dependency', 'worker'] = None,
+        blocked: Literal['dependency', 'resource', 'worker'] = None,
     ) -> ScheduledTask:
         full_proxy = self.proxy
         partial_proxy = self.proxy.get(task.name)
         blocker = None
         if blocked == 'dependency':
             tasks = self.dependency_handler.blocking_tasks(task)
             blocker = {'reason': blocked, 'tasks': tasks}
+        if blocked == 'resource':
+            sp = abs(min(0, self.system_processor - task.system_processor))
+            sm = abs(min(0, self.system_memory - task.system_memory))
+            gp = abs(min(0, self.graphics_processor - task.graphics_processor))
+            gm = abs(min(0, self.graphics_memory - task.graphics_memory))
+            blocker = {
+                'reason': blocked,
+                'system_processor': sp,
+                'system_memory': sm,
+                'graphics_processor': gp,
+                'graphics_memory': gm,
+            }
         if blocked == 'worker':
             processes = 0
             threads = 0
             if task.executor.__base__ == Process:
                 processes = abs(min(0, self.processes - (task.processes + 1)))
                 threads = abs(min(0, self.threads))
             if task.executor.__base__ == Thread:
                 processes = abs(min(0, self.processes - task.processes))
                 threads = abs(min(0, self.threads - (task.threads + 1)))
-            blocker = {'reason': blocked, 'processes': processes, 'threads': threads}
+            blocker = {
+                'reason': blocked,
+                'processes': processes,
+                'threads': threads,
+            }
         function_handler = FunctionHandler(
             name=task.name,
             target=task.target,
             proxy=partial_proxy,
             blocker=blocker,
         )
         if blocked:
@@ -169,30 +198,14 @@
             target=task.target,
             args=task.args,
             kwargs=task.kwargs,
             dependencies=task.dependencies,
             priority=task.priority,
             processes=task.processes,
             threads=task.threads,
+            system_processor=task.system_processor,
+            system_memory=task.system_memory,
+            graphics_processor=task.graphics_processor,
+            graphics_memory=task.graphics_memory,
             continual=task.continual,
             initialized=True,
         )
-
-    def enough_workers(self, task: ScheduledTask) -> bool:
-        return bool(
-            task.executor.__base__ == Process and
-            task.processes < self.processes
-        ) or bool(
-            task.executor.__base__ == Thread and
-            task.processes < self.processes and
-            task.threads < self.threads
-        )
-
-    def available_worker(self, task: ScheduledTask) -> bool:
-        return bool(
-            task.executor.__base__ == Process and
-            self.active_processes + task.processes < self.processes
-        ) or bool(
-            task.executor.__base__ == Thread and
-            self.active_processes + task.processes < self.processes and
-            self.active_threads + task.threads < self.threads
-        )
```

### Comparing `parallelism-0.1.2/parallelism.egg-info/PKG-INFO` & `parallelism-0.1.3/parallelism.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 Metadata-Version: 2.1
 Name: parallelism
-Version: 0.1.2
-Summary: Empowering workflows with parallelism
+Version: 0.1.3
+Summary: Enhance Parallel Task Execution
 Author: Idan Hazan
 License: MIT
 Project-URL: homepage, https://github.com/idanhazan/parallelism
 Project-URL: repository, https://github.com/idanhazan/parallelism
 Project-URL: documentation, https://parallelism.readthedocs.io
-Keywords: parallelism,parallel,task,scheduler
-Classifier: Programming Language :: Python :: 3
+Keywords: parallelism,parallel,scheduled,task,scheduler
+Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.11
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # parallelism
 
 The Parallelism library offers a powerful set of tools for managing concurrent task execution using both processes and threads.
 It aims to simplify the development of parallel programs, providing a higher-level interface for distributing tasks across multiple execution units.
```

### Comparing `parallelism-0.1.2/parallelism.egg-info/SOURCES.txt` & `parallelism-0.1.3/parallelism.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -19,16 +19,19 @@
 parallelism/core/raise_exception.py
 parallelism/core/return_value.py
 parallelism/core/scheduled_task.py
 parallelism/core/scheduler_result.py
 parallelism/core/task_scheduler.py
 parallelism/core/exceptions/__init__.py
 parallelism/core/exceptions/dependency_error.py
+parallelism/core/exceptions/resource_error.py
 parallelism/core/exceptions/worker_error.py
 parallelism/core/executors/__init__.py
 parallelism/core/executors/process_executor.py
 parallelism/core/executors/thread_executor.py
 parallelism/core/handlers/__init__.py
 parallelism/core/handlers/dependency_handler.py
 parallelism/core/handlers/function_handler.py
 parallelism/core/handlers/parameters_handler.py
-parallelism/core/handlers/shared_memory_handler.py
+parallelism/core/handlers/resource_handler.py
+parallelism/core/handlers/shared_memory_handler.py
+parallelism/core/handlers/worker_handler.py
```

