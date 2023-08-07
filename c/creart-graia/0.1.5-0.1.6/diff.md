# Comparing `tmp/creart-graia-0.1.5.tar.gz` & `tmp/creart-graia-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "creart-graia-0.1.5.tar", last modified: Fri Jul  1 04:21:13 2022, max compression
+gzip compressed data, was "creart-graia-0.1.6.tar", last modified: Sun Aug  6 15:44:59 2023, max compression
```

## Comparing `creart-graia-0.1.5.tar` & `creart-graia-0.1.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-07-01 04:21:00.552307 creart-graia-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-07-01 04:21:00.552307 creart-graia-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      962 2022-07-01 04:21:00.552307 creart-graia-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-01 04:21:00.552307 creart-graia-0.1.5/src/graia/creart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2482 2022-07-01 04:21:00.552307 creart-graia-0.1.5/src/graia/creart/broadcast.py
--rw-r--r--   0 runner    (1001) docker     (121)     1344 2022-07-01 04:21:00.552307 creart-graia-0.1.5/src/graia/creart/saya.py
--rw-r--r--   0 runner    (1001) docker     (121)     1846 2022-07-01 04:21:00.552307 creart-graia-0.1.5/src/graia/creart/scheduler.py
--rw-------   0 runner    (1001) docker     (121)      229 2022-07-01 04:21:13.936357 creart-graia-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-08-06 15:44:44.845266 creart-graia-0.1.6/LICENSE
+-rw-r--r--   0        0        0       17 2023-08-06 15:44:44.845266 creart-graia-0.1.6/README.md
+-rw-r--r--   0        0        0      578 2023-08-06 15:44:44.845266 creart-graia-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-06 15:44:44.849267 creart-graia-0.1.6/src/graia/creart/__init__.py
+-rw-r--r--   0        0        0     2456 2023-08-06 15:44:44.849267 creart-graia-0.1.6/src/graia/creart/broadcast.py
+-rw-r--r--   0        0        0     1344 2023-08-06 15:44:44.849267 creart-graia-0.1.6/src/graia/creart/saya.py
+-rw-r--r--   0        0        0     1846 2023-08-06 15:44:44.849267 creart-graia-0.1.6/src/graia/creart/scheduler.py
+-rw-r--r--   0        0        0      201 1970-01-01 00:00:00.000000 creart-graia-0.1.6/PKG-INFO
```

### Comparing `creart-graia-0.1.5/LICENSE` & `creart-graia-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `creart-graia-0.1.5/src/graia/creart/broadcast.py` & `creart-graia-0.1.6/src/graia/creart/broadcast.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     def create(
         create_type: type[Broadcast | InterruptControl],
     ) -> Broadcast | InterruptControl:
         from graia.broadcast import Broadcast
         from graia.broadcast.interrupt import InterruptControl
 
         if issubclass(create_type, Broadcast):
-            return create_type(loop=it(AbstractEventLoop))
+            return create_type()
         elif issubclass(create_type, InterruptControl):
             return create_type(it(Broadcast))
 
 
 class BroadcastBehaviourCreator(AbstractCreator):
     targets = (
         CreateTargetInfo(
```

### Comparing `creart-graia-0.1.5/src/graia/creart/saya.py` & `creart-graia-0.1.6/src/graia/creart/saya.py`

 * *Files identical despite different names*

### Comparing `creart-graia-0.1.5/src/graia/creart/scheduler.py` & `creart-graia-0.1.6/src/graia/creart/scheduler.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import asyncio
 from typing import TYPE_CHECKING
 
 from creart import AbstractCreator, CreateTargetInfo, exists_module, it, mixin
 
 from .broadcast import BroadcastCreator
 
 if TYPE_CHECKING:
@@ -27,16 +28,15 @@
     def available() -> bool:
         return exists_module("graia.scheduler")
 
     @staticmethod
     def create(create_type: type[GraiaScheduler]) -> GraiaScheduler:
         from graia.broadcast import Broadcast
 
-        broadcast = it(Broadcast)
-        return create_type(loop=broadcast.loop, broadcast=broadcast)
+        return create_type(loop=it(asyncio.AbstractEventLoop), broadcast=it(Broadcast))
 
 
 class SchedulerBehaviourCreator(AbstractCreator):
     targets = (
         CreateTargetInfo(
             module="graia.scheduler.saya.behaviour",
             identify="GraiaSchedulerBehaviour",
```

