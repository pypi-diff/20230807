# Comparing `tmp/aio_pika-9.2.0.tar.gz` & `tmp/aio_pika-9.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aio_pika-9.2.0.tar", max compression
+gzip compressed data, was "aio_pika-9.2.1.tar", max compression
```

## Comparing `aio_pika-9.2.0.tar` & `aio_pika-9.2.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    15357 2023-07-24 18:32:09.544633 aio_pika-9.2.0/README.rst
--rw-r--r--   0        0        0     1153 2023-03-09 17:26:20.374813 aio_pika-9.2.0/aio_pika/__init__.py
--rw-r--r--   0        0        0    25283 2023-07-28 10:20:38.626427 aio_pika-9.2.0/aio_pika/abc.py
--rw-r--r--   0        0        0    14701 2023-06-01 15:55:44.121581 aio_pika-9.2.0/aio_pika/channel.py
--rw-r--r--   0        0        0    11373 2023-07-28 10:20:38.627934 aio_pika-9.2.0/aio_pika/connection.py
--rw-r--r--   0        0        0     1304 2022-05-25 16:48:09.069546 aio_pika-9.2.0/aio_pika/exceptions.py
--rw-r--r--   0        0        0     6730 2023-06-01 15:55:44.124351 aio_pika-9.2.0/aio_pika/exchange.py
--rw-r--r--   0        0        0      246 2022-07-06 12:21:30.146673 aio_pika-9.2.0/aio_pika/log.py
--rw-r--r--   0        0        0    19763 2023-06-01 15:55:44.125260 aio_pika-9.2.0/aio_pika/message.py
--rw-r--r--   0        0        0      233 2020-05-21 16:45:24.000000 aio_pika-9.2.0/aio_pika/patterns/__init__.py
--rw-r--r--   0        0        0     1427 2023-06-01 15:55:44.126438 aio_pika-9.2.0/aio_pika/patterns/base.py
--rw-r--r--   0        0        0     6208 2023-06-01 15:55:44.128054 aio_pika-9.2.0/aio_pika/patterns/master.py
--rw-r--r--   0        0        0    14727 2023-06-07 14:58:48.045474 aio_pika-9.2.0/aio_pika/patterns/rpc.py
--rw-r--r--   0        0        0     4177 2023-06-01 15:55:44.130894 aio_pika-9.2.0/aio_pika/pool.py
--rw-r--r--   0        0        0        1 2019-02-24 19:52:26.000000 aio_pika-9.2.0/aio_pika/py.typed
--rw-r--r--   0        0        0    16598 2023-06-01 15:55:44.131780 aio_pika-9.2.0/aio_pika/queue.py
--rw-r--r--   0        0        0     8275 2023-07-24 18:23:35.142833 aio_pika-9.2.0/aio_pika/robust_channel.py
--rw-r--r--   0        0        0    10677 2023-07-28 10:20:38.628792 aio_pika-9.2.0/aio_pika/robust_connection.py
--rw-r--r--   0        0        0     2889 2023-06-01 15:55:44.136022 aio_pika-9.2.0/aio_pika/robust_exchange.py
--rw-r--r--   0        0        0     4683 2023-07-04 14:24:49.233661 aio_pika-9.2.0/aio_pika/robust_queue.py
--rw-r--r--   0        0        0     8639 2023-06-01 15:55:44.138218 aio_pika-9.2.0/aio_pika/tools.py
--rw-r--r--   0        0        0     2065 2023-06-01 15:55:44.139689 aio_pika-9.2.0/aio_pika/transaction.py
--rw-r--r--   0        0        0     3269 2023-07-28 10:25:54.710488 aio_pika-9.2.0/pyproject.toml
--rw-r--r--   0        0        0    16960 1970-01-01 00:00:00.000000 aio_pika-9.2.0/PKG-INFO
+-rw-r--r--   0        0        0    15357 2023-07-24 18:32:09.544633 aio_pika-9.2.1/README.rst
+-rw-r--r--   0        0        0     1153 2023-03-09 17:26:20.374813 aio_pika-9.2.1/aio_pika/__init__.py
+-rw-r--r--   0        0        0    25283 2023-07-28 10:20:38.626427 aio_pika-9.2.1/aio_pika/abc.py
+-rw-r--r--   0        0        0    14701 2023-06-01 15:55:44.121581 aio_pika-9.2.1/aio_pika/channel.py
+-rw-r--r--   0        0        0    11373 2023-07-28 10:20:38.627934 aio_pika-9.2.1/aio_pika/connection.py
+-rw-r--r--   0        0        0     1304 2022-05-25 16:48:09.069546 aio_pika-9.2.1/aio_pika/exceptions.py
+-rw-r--r--   0        0        0     6730 2023-06-01 15:55:44.124351 aio_pika-9.2.1/aio_pika/exchange.py
+-rw-r--r--   0        0        0      246 2022-07-06 12:21:30.146673 aio_pika-9.2.1/aio_pika/log.py
+-rw-r--r--   0        0        0    19763 2023-06-01 15:55:44.125260 aio_pika-9.2.1/aio_pika/message.py
+-rw-r--r--   0        0        0      233 2020-05-21 16:45:24.000000 aio_pika-9.2.1/aio_pika/patterns/__init__.py
+-rw-r--r--   0        0        0     1427 2023-06-01 15:55:44.126438 aio_pika-9.2.1/aio_pika/patterns/base.py
+-rw-r--r--   0        0        0     6208 2023-06-01 15:55:44.128054 aio_pika-9.2.1/aio_pika/patterns/master.py
+-rw-r--r--   0        0        0    14727 2023-06-07 14:58:48.045474 aio_pika-9.2.1/aio_pika/patterns/rpc.py
+-rw-r--r--   0        0        0     4177 2023-06-01 15:55:44.130894 aio_pika-9.2.1/aio_pika/pool.py
+-rw-r--r--   0        0        0        1 2019-02-24 19:52:26.000000 aio_pika-9.2.1/aio_pika/py.typed
+-rw-r--r--   0        0        0    16598 2023-06-01 15:55:44.131780 aio_pika-9.2.1/aio_pika/queue.py
+-rw-r--r--   0        0        0     8017 2023-08-07 13:42:40.320642 aio_pika-9.2.1/aio_pika/robust_channel.py
+-rw-r--r--   0        0        0    10677 2023-07-28 10:20:38.628792 aio_pika-9.2.1/aio_pika/robust_connection.py
+-rw-r--r--   0        0        0     2889 2023-06-01 15:55:44.136022 aio_pika-9.2.1/aio_pika/robust_exchange.py
+-rw-r--r--   0        0        0     4683 2023-07-04 14:24:49.233661 aio_pika-9.2.1/aio_pika/robust_queue.py
+-rw-r--r--   0        0        0     8639 2023-06-01 15:55:44.138218 aio_pika-9.2.1/aio_pika/tools.py
+-rw-r--r--   0        0        0     2065 2023-06-01 15:55:44.139689 aio_pika-9.2.1/aio_pika/transaction.py
+-rw-r--r--   0        0        0     3269 2023-08-07 13:44:20.213435 aio_pika-9.2.1/pyproject.toml
+-rw-r--r--   0        0        0    16960 1970-01-01 00:00:00.000000 aio_pika-9.2.1/PKG-INFO
```

### Comparing `aio_pika-9.2.0/README.rst` & `aio_pika-9.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `aio_pika-9.2.0/aio_pika/__init__.py` & `aio_pika-9.2.1/aio_pika/__init__.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.2.0/aio_pika/abc.py` & `aio_pika-9.2.1/aio_pika/abc.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.2.0/aio_pika/channel.py` & `aio_pika-9.2.1/aio_pika/channel.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.2.0/aio_pika/connection.py` & `aio_pika-9.2.1/aio_pika/connection.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.2.0/aio_pika/exceptions.py` & `aio_pika-9.2.1/aio_pika/exceptions.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.2.0/aio_pika/exchange.py` & `aio_pika-9.2.1/aio_pika/exchange.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.2.0/aio_pika/message.py` & `aio_pika-9.2.1/aio_pika/message.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.2.0/aio_pika/patterns/base.py` & `aio_pika-9.2.1/aio_pika/patterns/base.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.2.0/aio_pika/patterns/master.py` & `aio_pika-9.2.1/aio_pika/patterns/master.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.2.0/aio_pika/patterns/rpc.py` & `aio_pika-9.2.1/aio_pika/patterns/rpc.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.2.0/aio_pika/pool.py` & `aio_pika-9.2.1/aio_pika/pool.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.2.0/aio_pika/queue.py` & `aio_pika-9.2.1/aio_pika/queue.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.2.0/aio_pika/robust_channel.py` & `aio_pika-9.2.1/aio_pika/robust_channel.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,21 +64,19 @@
         self._exchanges = defaultdict(WeakSet)
         self._queues = defaultdict(WeakSet)
         self._prefetch_count: int = 0
         self._prefetch_size: int = 0
         self._global_qos: bool = False
         self.reopen_callbacks: CallbackCollection = CallbackCollection(self)
         self.__restore_lock = asyncio.Lock()
-        self.__ready = asyncio.Event()
         self.__restored = asyncio.Event()
-        self.__restored.set()
         self.close_callbacks.add(self.__close_callback)
 
     async def ready(self) -> None:
-        await self.__ready.wait()
+        await self._connection.ready()
         await self.__restored.wait()
 
     async def get_underlay_channel(self) -> aiormq.abc.AbstractChannel:
         await self._connection.ready()
         return await super().get_underlay_channel()
 
     async def restore(self, channel: Any = None) -> None:
@@ -102,15 +100,14 @@
             # outside, for example, if the connection is closed.
             # Of course, here you need to exit from this function
             # as soon as possible and to avoid a recovery attempt.
             return
 
         in_restore_state = not self.__restored.is_set()
         self.__restored.clear()
-        self.__ready.clear()
 
         if self._closed or in_restore_state:
             return
 
         await self.restore()
 
     async def _open(self) -> None:
@@ -135,29 +132,29 @@
 
         for queue in queues:
             await queue.restore()
 
         if hasattr(self, "default_exchange"):
             self.default_exchange.channel = self
 
-        self.__ready.set()
+        self.__restored.set()
 
     async def set_qos(
         self,
         prefetch_count: int = 0,
         prefetch_size: int = 0,
         global_: bool = False,
         timeout: TimeoutType = None,
         all_channels: Optional[bool] = None,
     ) -> aiormq.spec.Basic.QosOk:
         if all_channels is not None:
             warn('Use "global_" instead of "all_channels"', DeprecationWarning)
             global_ = all_channels
 
-        await self._connection.ready()
+        await self.ready()
 
         self._prefetch_count = prefetch_count
         self._prefetch_size = prefetch_size
         self._global_qos = global_
 
         return await super().set_qos(
             prefetch_count=prefetch_count,
@@ -174,15 +171,14 @@
         auto_delete: bool = False,
         internal: bool = False,
         passive: bool = False,
         arguments: Optional[Dict[str, Any]] = None,
         timeout: TimeoutType = None,
         robust: bool = True,
     ) -> AbstractRobustExchange:
-        await self._connection.ready()
         await self.ready()
         exchange = (
             await super().declare_exchange(
                 name=name,
                 type=type,
                 durable=durable,
                 auto_delete=auto_delete,
@@ -202,15 +198,14 @@
     async def exchange_delete(
         self,
         exchange_name: str,
         timeout: TimeoutType = None,
         if_unused: bool = False,
         nowait: bool = False,
     ) -> aiormq.spec.Exchange.DeleteOk:
-        await self._connection.ready()
         await self.ready()
         result = await super().exchange_delete(
             exchange_name=exchange_name,
             timeout=timeout,
             if_unused=if_unused,
             nowait=nowait,
         )
@@ -225,15 +220,14 @@
         exclusive: bool = False,
         passive: bool = False,
         auto_delete: bool = False,
         arguments: Optional[Dict[str, Any]] = None,
         timeout: TimeoutType = None,
         robust: bool = True,
     ) -> AbstractRobustQueue:
-        await self._connection.ready()
         await self.ready()
         queue: RobustQueue = await super().declare_queue(   # type: ignore
             name=name,
             durable=durable,
             exclusive=exclusive,
             passive=passive,
             auto_delete=auto_delete,
@@ -248,15 +242,14 @@
         self,
         queue_name: str,
         timeout: TimeoutType = None,
         if_unused: bool = False,
         if_empty: bool = False,
         nowait: bool = False,
     ) -> aiormq.spec.Queue.DeleteOk:
-        await self._connection.ready()
         await self.ready()
         result = await super().queue_delete(
             queue_name=queue_name,
             timeout=timeout,
             if_unused=if_unused,
             if_empty=if_empty,
             nowait=nowait,
```

### Comparing `aio_pika-9.2.0/aio_pika/robust_connection.py` & `aio_pika-9.2.1/aio_pika/robust_connection.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.2.0/aio_pika/robust_exchange.py` & `aio_pika-9.2.1/aio_pika/robust_exchange.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.2.0/aio_pika/robust_queue.py` & `aio_pika-9.2.1/aio_pika/robust_queue.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.2.0/aio_pika/tools.py` & `aio_pika-9.2.1/aio_pika/tools.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.2.0/aio_pika/transaction.py` & `aio_pika-9.2.1/aio_pika/transaction.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.2.0/pyproject.toml` & `aio_pika-9.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aio-pika"
-version = "9.2.0"
+version = "9.2.1"
 description = "Wrapper around the aiormq for asyncio and humans"
 authors = ["Dmitry Orlov <me@mosquito.su>"]
 readme = "README.rst"
 license = "Apache-2.0"
 keywords=["rabbitmq", "asyncio", "amqp", "amqp 0.9.1", "aiormq"]
 homepage = "https://github.com/mosquito/aio-pika"
 classifiers = [
```

### Comparing `aio_pika-9.2.0/PKG-INFO` & `aio_pika-9.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aio-pika
-Version: 9.2.0
+Version: 9.2.1
 Summary: Wrapper around the aiormq for asyncio and humans
 Home-page: https://github.com/mosquito/aio-pika
 License: Apache-2.0
 Keywords: rabbitmq,asyncio,amqp,amqp 0.9.1,aiormq
 Author: Dmitry Orlov
 Author-email: me@mosquito.su
 Requires-Python: >=3.7,<4.0
```

