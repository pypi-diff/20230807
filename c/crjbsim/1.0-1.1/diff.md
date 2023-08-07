# Comparing `tmp/crjbsim-1.0.tar.gz` & `tmp/crjbsim-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crjbsim-1.0.tar", last modified: Mon Jul 17 10:45:02 2023, max compression
+gzip compressed data, was "crjbsim-1.1.tar", last modified: Mon Aug  7 19:53:42 2023, max compression
```

## Comparing `crjbsim-1.0.tar` & `crjbsim-1.1.tar`

### file list

```diff
@@ -1,26 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:45:02.910710 crjbsim-1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:45:02.906710 crjbsim-1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:45:02.910710 crjbsim-1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-17 10:44:52.000000 crjbsim-1.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-17 10:44:52.000000 crjbsim-1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-17 10:45:02.910710 crjbsim-1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-17 10:44:52.000000 crjbsim-1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-17 10:44:52.000000 crjbsim-1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-17 10:44:52.000000 crjbsim-1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-17 10:45:02.910710 crjbsim-1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:45:02.906710 crjbsim-1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:45:02.910710 crjbsim-1.0/src/crjbsim/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 10:44:52.000000 crjbsim-1.0/src/crjbsim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-07-17 10:44:52.000000 crjbsim-1.0/src/crjbsim/asncio_des.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-17 10:44:52.000000 crjbsim-1.0/src/crjbsim/des_aware_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-17 10:44:52.000000 crjbsim-1.0/src/crjbsim/discrete_event_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-17 10:44:52.000000 crjbsim-1.0/src/crjbsim/sim.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-17 10:44:52.000000 crjbsim-1.0/src/crjbsim/time_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:45:02.910710 crjbsim-1.0/src/crjbsim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-17 10:45:02.000000 crjbsim-1.0/src/crjbsim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-17 10:45:02.000000 crjbsim-1.0/src/crjbsim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 10:45:02.000000 crjbsim-1.0/src/crjbsim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 10:45:02.000000 crjbsim-1.0/src/crjbsim.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:45:02.910710 crjbsim-1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-07-17 10:44:52.000000 crjbsim-1.0/tests/test_asyncio_des.py
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-07-17 10:44:52.000000 crjbsim-1.0/tests/test_sim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:53:42.890359 crjbsim-1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:53:42.886360 crjbsim-1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:53:42.886360 crjbsim-1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-08-07 19:53:33.000000 crjbsim-1.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-07 19:53:33.000000 crjbsim-1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-08-07 19:53:42.890359 crjbsim-1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-08-07 19:53:33.000000 crjbsim-1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-07 19:53:33.000000 crjbsim-1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-07 19:53:33.000000 crjbsim-1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-08-07 19:53:42.890359 crjbsim-1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:53:42.886360 crjbsim-1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:53:42.890359 crjbsim-1.1/src/crjbsim/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 19:53:33.000000 crjbsim-1.1/src/crjbsim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-08-07 19:53:33.000000 crjbsim-1.1/src/crjbsim/asncio_des.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-08-07 19:53:33.000000 crjbsim-1.1/src/crjbsim/des_aware_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-08-07 19:53:33.000000 crjbsim-1.1/src/crjbsim/discrete_event_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-08-07 19:53:33.000000 crjbsim-1.1/src/crjbsim/scenario_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-08-07 19:53:33.000000 crjbsim-1.1/src/crjbsim/sim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-08-07 19:53:33.000000 crjbsim-1.1/src/crjbsim/time_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:53:42.890359 crjbsim-1.1/src/crjbsim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-08-07 19:53:42.000000 crjbsim-1.1/src/crjbsim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-08-07 19:53:42.000000 crjbsim-1.1/src/crjbsim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 19:53:42.000000 crjbsim-1.1/src/crjbsim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-07 19:53:42.000000 crjbsim-1.1/src/crjbsim.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:53:42.890359 crjbsim-1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-08-07 19:53:33.000000 crjbsim-1.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-08-07 19:53:33.000000 crjbsim-1.1/tests/test_asyncio_des.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-08-07 19:53:33.000000 crjbsim-1.1/tests/test_scenarios.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-08-07 19:53:33.000000 crjbsim-1.1/tests/test_sim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-08-07 19:53:33.000000 crjbsim-1.1/tests/traffic_light_scenario_steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-08-07 19:53:33.000000 crjbsim-1.1/tests/traffic_light_sim.py
```

### Comparing `crjbsim-1.0/setup.cfg` & `crjbsim-1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `crjbsim-1.0/src/crjbsim/asncio_des.py` & `crjbsim-1.1/src/crjbsim/asncio_des.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import functools
 import logging
 import traceback
 from asyncio import AbstractEventLoop, AbstractEventLoopPolicy, events, futures, tasks
 
-from crjbsim import time_provider
+from crjbsim import sim, time_provider
 from crjbsim.discrete_event_scheduler import DiscreteEventScheduler
 
 logger = logging.getLogger()
 
 
 class DiscreteEventLoop(AbstractEventLoop):
     def __init__(self):
@@ -26,16 +26,17 @@
     def call_at(self, when, callback, *args, context=None):
         wrapped = functools.partial(callback, *args)
         return self.scheduler.do_at(when, wrapped)
 
     def run_until_complete(self, future):
         events._set_running_loop(self)
         future = tasks.ensure_future(future, loop=self)
-        self.scheduler.start()
+        self.scheduler.run_to_completion()
         events._set_running_loop(None)
+        return future
 
     def close(self):
         pass
 
     def create_future(self):
         return futures.Future(loop=self)
 
@@ -109,10 +110,11 @@
 
     def get_event_loop(self):
         assert self.loop
         return self.loop
 
     def set_event_loop(self, loop):
         self.loop = loop
+        sim.scheduler = loop.scheduler if loop else None
 
     def new_event_loop(self):
         return DiscreteEventLoop()
```

### Comparing `crjbsim-1.0/src/crjbsim/des_aware_logging.py` & `crjbsim-1.1/src/crjbsim/des_aware_logging.py`

 * *Files identical despite different names*

### Comparing `crjbsim-1.0/tests/test_asyncio_des.py` & `crjbsim-1.1/tests/test_asyncio_des.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,34 @@
 import asyncio
+import functools
 import logging
 import time
 from asyncio import DefaultEventLoopPolicy, events
 from datetime import datetime
 
 from crjbsim import des_aware_logging, sim, time_provider
 from crjbsim.asncio_des import DiscreteEventLoopPolicy
 
 logger = logging.getLogger(__name__)
 
 
+def test_async_des_basic():
+    async def a():
+        async def b():
+            await asyncio.sleep(1)
+        await b()
+
+    try:
+        asyncio.set_event_loop_policy(DiscreteEventLoopPolicy())
+        asyncio.run(a())
+    finally:
+        asyncio.set_event_loop_policy(DefaultEventLoopPolicy())
+
+    assert time_provider.get_time() == 1
+
 async def action(name, delay, repetition):
     logger.info(f"{name} started at {datetime.now()}")
     for i in range(repetition):
         await asyncio.sleep(delay)
         logger.info(f"{name} repetition {i} done at {datetime.now()}")
     logger.info(f"{name} finished at {datetime.now()}")
 
@@ -127,7 +142,26 @@
         asyncio.set_event_loop_policy(DiscreteEventLoopPolicy())
         asyncio.run(mixed_sim())
     finally:
         asyncio.set_event_loop_policy(DefaultEventLoopPolicy())
 
     assert test_list == [1]
     assert time_provider.get_time() == 3
+
+
+def test_async_des_very_mixed():
+    async def sim_movement():
+        await asyncio.sleep(1)
+        print("moved")
+
+    async def mixed_sim():
+        await asyncio.sleep(1)
+        events.get_running_loop().scheduler.do_in(2, sim_movement)
+
+    des_aware_logging.setup()
+    try:
+        asyncio.set_event_loop_policy(DiscreteEventLoopPolicy())
+        asyncio.run(mixed_sim())
+    finally:
+        asyncio.set_event_loop_policy(DefaultEventLoopPolicy())
+
+    assert time_provider.get_time() == 4
```

### Comparing `crjbsim-1.0/tests/test_sim.py` & `crjbsim-1.1/tests/test_sim.py`

 * *Files identical despite different names*

