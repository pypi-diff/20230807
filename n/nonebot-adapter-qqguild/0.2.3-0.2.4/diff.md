# Comparing `tmp/nonebot_adapter_qqguild-0.2.3.tar.gz` & `tmp/nonebot_adapter_qqguild-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_adapter_qqguild-0.2.3.tar", max compression
+gzip compressed data, was "nonebot_adapter_qqguild-0.2.4.tar", max compression
```

## Comparing `nonebot_adapter_qqguild-0.2.3.tar` & `nonebot_adapter_qqguild-0.2.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1064 2023-06-18 15:43:56.922875 nonebot_adapter_qqguild-0.2.3/LICENSE
--rw-r--r--   0        0        0      895 2023-06-18 15:43:56.922875 nonebot_adapter_qqguild-0.2.3/README.md
--rw-r--r--   0        0        0      239 2023-06-18 15:43:56.926875 nonebot_adapter_qqguild-0.2.3/nonebot/adapters/qqguild/__init__.py
--rw-r--r--   0        0        0    12671 2023-06-18 15:43:56.926875 nonebot_adapter_qqguild-0.2.3/nonebot/adapters/qqguild/adapter.py
--rw-r--r--   0        0        0      113 2023-06-18 15:43:56.926875 nonebot_adapter_qqguild-0.2.3/nonebot/adapters/qqguild/api/__init__.py
--rw-r--r--   0        0        0     9270 2023-06-18 15:43:56.926875 nonebot_adapter_qqguild-0.2.3/nonebot/adapters/qqguild/api/client.py
--rw-r--r--   0        0        0    21428 2023-06-18 15:43:56.926875 nonebot_adapter_qqguild-0.2.3/nonebot/adapters/qqguild/api/handle.py
--rw-r--r--   0        0        0    10734 2023-06-18 15:43:56.926875 nonebot_adapter_qqguild-0.2.3/nonebot/adapters/qqguild/api/model.py
--rw-r--r--   0        0        0     1668 2023-06-18 15:43:56.926875 nonebot_adapter_qqguild-0.2.3/nonebot/adapters/qqguild/api/request.py
--rw-r--r--   0        0        0     1023 2023-06-18 15:43:56.926875 nonebot_adapter_qqguild-0.2.3/nonebot/adapters/qqguild/api/utils.py
--rw-r--r--   0        0        0     6410 2023-06-18 15:43:56.926875 nonebot_adapter_qqguild-0.2.3/nonebot/adapters/qqguild/bot.py
--rw-r--r--   0        0        0     1353 2023-06-18 15:43:56.926875 nonebot_adapter_qqguild-0.2.3/nonebot/adapters/qqguild/config.py
--rw-r--r--   0        0        0     9534 2023-06-18 15:43:56.926875 nonebot_adapter_qqguild-0.2.3/nonebot/adapters/qqguild/event.py
--rw-r--r--   0        0        0     2292 2023-06-18 15:43:56.926875 nonebot_adapter_qqguild-0.2.3/nonebot/adapters/qqguild/exception.py
--rw-r--r--   0        0        0     6703 2023-06-18 15:43:56.926875 nonebot_adapter_qqguild-0.2.3/nonebot/adapters/qqguild/message.py
--rw-r--r--   0        0        0     2087 2023-06-18 15:43:56.926875 nonebot_adapter_qqguild-0.2.3/nonebot/adapters/qqguild/payload.py
--rw-r--r--   0        0        0      982 2023-06-18 15:43:56.926875 nonebot_adapter_qqguild-0.2.3/nonebot/adapters/qqguild/permission.py
--rw-r--r--   0        0        0      874 2023-06-18 15:43:56.926875 nonebot_adapter_qqguild-0.2.3/nonebot/adapters/qqguild/store.py
--rw-r--r--   0        0        0     3416 2023-06-18 15:43:56.926875 nonebot_adapter_qqguild-0.2.3/nonebot/adapters/qqguild/transformer.py
--rw-r--r--   0        0        0      289 2023-06-18 15:43:56.926875 nonebot_adapter_qqguild-0.2.3/nonebot/adapters/qqguild/utils.py
--rw-r--r--   0        0        0     1697 2023-06-18 15:43:56.926875 nonebot_adapter_qqguild-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     1949 1970-01-01 00:00:00.000000 nonebot_adapter_qqguild-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-08-07 04:00:26.434701 nonebot_adapter_qqguild-0.2.4/LICENSE
+-rw-r--r--   0        0        0      895 2023-08-07 04:00:26.434701 nonebot_adapter_qqguild-0.2.4/README.md
+-rw-r--r--   0        0        0      239 2023-08-07 04:00:26.434701 nonebot_adapter_qqguild-0.2.4/nonebot/adapters/qqguild/__init__.py
+-rw-r--r--   0        0        0    13139 2023-08-07 04:00:26.434701 nonebot_adapter_qqguild-0.2.4/nonebot/adapters/qqguild/adapter.py
+-rw-r--r--   0        0        0      113 2023-08-07 04:00:26.434701 nonebot_adapter_qqguild-0.2.4/nonebot/adapters/qqguild/api/__init__.py
+-rw-r--r--   0        0        0     9231 2023-08-07 04:00:26.434701 nonebot_adapter_qqguild-0.2.4/nonebot/adapters/qqguild/api/client.py
+-rw-r--r--   0        0        0    21428 2023-08-07 04:00:26.434701 nonebot_adapter_qqguild-0.2.4/nonebot/adapters/qqguild/api/handle.py
+-rw-r--r--   0        0        0    12214 2023-08-07 04:00:26.434701 nonebot_adapter_qqguild-0.2.4/nonebot/adapters/qqguild/api/model.py
+-rw-r--r--   0        0        0     1668 2023-08-07 04:00:26.434701 nonebot_adapter_qqguild-0.2.4/nonebot/adapters/qqguild/api/request.py
+-rw-r--r--   0        0        0     1023 2023-08-07 04:00:26.434701 nonebot_adapter_qqguild-0.2.4/nonebot/adapters/qqguild/api/utils.py
+-rw-r--r--   0        0        0     6439 2023-08-07 04:00:26.434701 nonebot_adapter_qqguild-0.2.4/nonebot/adapters/qqguild/bot.py
+-rw-r--r--   0        0        0     1353 2023-08-07 04:00:26.438701 nonebot_adapter_qqguild-0.2.4/nonebot/adapters/qqguild/config.py
+-rw-r--r--   0        0        0     9614 2023-08-07 04:00:26.438701 nonebot_adapter_qqguild-0.2.4/nonebot/adapters/qqguild/event.py
+-rw-r--r--   0        0        0     2292 2023-08-07 04:00:26.438701 nonebot_adapter_qqguild-0.2.4/nonebot/adapters/qqguild/exception.py
+-rw-r--r--   0        0        0     6677 2023-08-07 04:00:26.438701 nonebot_adapter_qqguild-0.2.4/nonebot/adapters/qqguild/message.py
+-rw-r--r--   0        0        0     2087 2023-08-07 04:00:26.438701 nonebot_adapter_qqguild-0.2.4/nonebot/adapters/qqguild/payload.py
+-rw-r--r--   0        0        0      982 2023-08-07 04:00:26.438701 nonebot_adapter_qqguild-0.2.4/nonebot/adapters/qqguild/permission.py
+-rw-r--r--   0        0        0      874 2023-08-07 04:00:26.438701 nonebot_adapter_qqguild-0.2.4/nonebot/adapters/qqguild/store.py
+-rw-r--r--   0        0        0     3416 2023-08-07 04:00:26.438701 nonebot_adapter_qqguild-0.2.4/nonebot/adapters/qqguild/transformer.py
+-rw-r--r--   0        0        0      289 2023-08-07 04:00:26.438701 nonebot_adapter_qqguild-0.2.4/nonebot/adapters/qqguild/utils.py
+-rw-r--r--   0        0        0     1955 2023-08-07 04:00:26.438701 nonebot_adapter_qqguild-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     1949 1970-01-01 00:00:00.000000 nonebot_adapter_qqguild-0.2.4/PKG-INFO
```

### Comparing `nonebot_adapter_qqguild-0.2.3/LICENSE` & `nonebot_adapter_qqguild-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_qqguild-0.2.3/README.md` & `nonebot_adapter_qqguild-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_qqguild-0.2.3/nonebot/adapters/qqguild/adapter.py` & `nonebot_adapter_qqguild-0.2.4/nonebot/adapters/qqguild/adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,30 +47,33 @@
     @overrides(BaseAdapter)
     def get_name(cls) -> str:
         return "QQ Guild"
 
     def setup(self) -> None:
         if not isinstance(self.driver, ForwardDriver):
             raise RuntimeError(
-                f"Current driver {self.config.driver} doesn't support forward connections!"
-                "QQ Guild Adapter need a ForwardDriver to work."
+                f"Current driver {self.config.driver} does not support "
+                "forward connections! QQ Guild Adapter need a ForwardDriver to work."
             )
         self.driver.on_startup(self.startup)
         self.driver.on_shutdown(self.shutdown)
 
     async def startup(self) -> None:
         log(
             "DEBUG",
-            f"QQ Guild run in sandbox mode: <y>{self.qqguild_config.qqguild_is_sandbox}</y>",
+            (
+                "QQ Guild run in sandbox mode: "
+                f"<y>{self.qqguild_config.qqguild_is_sandbox}</y>"
+            ),
         )
 
         try:
             self.api_base = self.get_api_base()
         except Exception as e:
-            log("ERROR", f"Failed to parse QQ Guild api base url", e)
+            log("ERROR", "Failed to parse QQ Guild api base url", e)
             raise
 
         log("DEBUG", f"QQ Guild api base url: <y>{escape_tag(str(self.api_base))}</y>")
 
         for bot in self.qqguild_config.qqguild_bots:
             self.tasks.append(asyncio.create_task(self.run_bot(bot)))
 
@@ -133,15 +136,18 @@
         heartbeat_task: Optional["asyncio.Task"] = None
 
         while True:
             try:
                 async with self.websocket(request) as ws:
                     log(
                         "DEBUG",
-                        f"WebSocket Connection to {escape_tag(str(ws_url))} established",
+                        (
+                            "WebSocket Connection to "
+                            f"{escape_tag(str(ws_url))} established"
+                        ),
                     )
 
                     try:
                         # hello
                         heartbeat_interval = await self._hello(ws)
                         if not heartbeat_interval:
                             await asyncio.sleep(RECONNECT_INTERVAL)
@@ -159,35 +165,43 @@
                         )
 
                         # process events
                         await self._loop(bot, ws)
                     except WebSocketClosed as e:
                         log(
                             "ERROR",
-                            f"<r><bg #f8bbd0>WebSocket Closed</bg #f8bbd0></r>",
+                            "<r><bg #f8bbd0>WebSocket Closed</bg #f8bbd0></r>",
                             e,
                         )
                     except Exception as e:
                         log(
                             "ERROR",
-                            "<r><bg #f8bbd0>Error while process data from websocket "
-                            f"{escape_tag(str(ws_url))}. Trying to reconnect...</bg #f8bbd0></r>",
+                            (
+                                "<r><bg #f8bbd0>"
+                                "Error while process data from websocket "
+                                f"{escape_tag(str(ws_url))}. Trying to reconnect..."
+                                "</bg #f8bbd0></r>"
+                            ),
                             e,
                         )
                     finally:
                         if heartbeat_task:
                             heartbeat_task.cancel()
                             heartbeat_task = None
                         self.bot_disconnect(bot)
 
             except Exception as e:
                 log(
                     "ERROR",
-                    "<r><bg #f8bbd0>Error while setup websocket to "
-                    f"{escape_tag(str(ws_url))}. Trying to reconnect...</bg #f8bbd0></r>",
+                    (
+                        "<r><bg #f8bbd0>"
+                        "Error while setup websocket to "
+                        f"{escape_tag(str(ws_url))}. Trying to reconnect..."
+                        "</bg #f8bbd0></r>"
+                    ),
                     e,
                 )
 
             await asyncio.sleep(RECONNECT_INTERVAL)
 
     async def _hello(self, ws: WebSocket):
         """接收并处理服务器的 Hello 事件"""
@@ -196,15 +210,19 @@
             assert isinstance(
                 payload, Hello
             ), f"Received unexpected payload: {payload!r}"
             return payload.data.heartbeat_interval
         except Exception as e:
             log(
                 "ERROR",
-                "<r><bg #f8bbd0>Error while receiving server hello event</bg #f8bbd0></r>",
+                (
+                    "<r><bg #f8bbd0>"
+                    "Error while receiving server hello event"
+                    "</bg #f8bbd0></r>"
+                ),
                 e,
             )
 
     async def _authenticate(self, bot: Bot, ws: WebSocket, shard: Tuple[int, int]):
         """鉴权连接"""
         if not bot.ready:
             payload = Identify.parse_obj(
```

### Comparing `nonebot_adapter_qqguild-0.2.3/nonebot/adapters/qqguild/api/client.py` & `nonebot_adapter_qqguild-0.2.4/nonebot/adapters/qqguild/api/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 from typing import TYPE_CHECKING, List, Optional
 
-from pydantic import Extra, BaseModel
-
 from .model import *
 
 if TYPE_CHECKING:
 
     class ApiClient:
         async def get_guild(self, *, guild_id: int) -> Guild:
             ...
```

### Comparing `nonebot_adapter_qqguild-0.2.3/nonebot/adapters/qqguild/api/handle.py` & `nonebot_adapter_qqguild-0.2.4/nonebot/adapters/qqguild/api/handle.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,30 +20,30 @@
     )
     return parse_obj_as(Guild, await _request(adapter, bot, request))
 
 
 async def _me(adapter: "Adapter", bot: "Bot") -> User:
     request = Request(
         "GET",
-        adapter.get_api_base() / f"users/@me",
+        adapter.get_api_base() / "users/@me",
         headers={"Authorization": adapter.get_authorization(bot.bot_info)},
     )
     return parse_obj_as(User, await _request(adapter, bot, request))
 
 
 async def _guilds(
     adapter: "Adapter",
     bot: "Bot",
-    before: Optional[str] = ...,
-    after: Optional[str] = ...,
-    limit: Optional[float] = ...,
+    before: Optional[str] = None,
+    after: Optional[str] = None,
+    limit: Optional[float] = None,
 ) -> List[Guild]:
     request = Request(
         "GET",
-        adapter.get_api_base() / f"users/@me/guilds",
+        adapter.get_api_base() / "users/@me/guilds",
         params=_exclude_none({"before": before, "after": after, "limit": limit}),
         headers={"Authorization": adapter.get_authorization(bot.bot_info)},
     )
     return parse_obj_as(List[Guild], await _request(adapter, bot, request))
 
 
 async def _get_channels(adapter: "Adapter", bot: "Bot", guild_id: int) -> List[Channel]:
@@ -97,16 +97,16 @@
     return await _request(adapter, bot, request)
 
 
 async def _get_members(
     adapter: "Adapter",
     bot: "Bot",
     guild_id: int,
-    after: Optional[str] = ...,
-    limit: Optional[float] = ...,
+    after: Optional[str] = None,
+    limit: Optional[float] = None,
 ) -> List[Member]:
     request = Request(
         "GET",
         adapter.get_api_base() / f"guilds/{guild_id}/members",
         params=_exclude_none({"after": after, "limit": limit}),
         headers={"Authorization": adapter.get_authorization(bot.bot_info)},
     )
@@ -291,15 +291,15 @@
     )
     return parse_obj_as(Message, await _request(adapter, bot, request))
 
 
 async def _post_dms(adapter: "Adapter", bot: "Bot", **data) -> DMS:
     request = Request(
         "POST",
-        adapter.get_api_base() / f"users/@me/dms",
+        adapter.get_api_base() / "users/@me/dms",
         json=PostDmsBody(**data).dict(exclude_none=True),
         headers={"Authorization": adapter.get_authorization(bot.bot_info)},
     )
     return parse_obj_as(DMS, await _request(adapter, bot, request))
 
 
 async def _post_dms_messages(
@@ -479,24 +479,24 @@
         List[APIPermissionDemand], await _request(adapter, bot, request)
     )
 
 
 async def _url_get(adapter: "Adapter", bot: "Bot") -> UrlGetReturn:
     request = Request(
         "GET",
-        adapter.get_api_base() / f"gateway",
+        adapter.get_api_base() / "gateway",
         headers={"Authorization": adapter.get_authorization(bot.bot_info)},
     )
     return parse_obj_as(UrlGetReturn, await _request(adapter, bot, request))
 
 
 async def _shard_url_get(adapter: "Adapter", bot: "Bot") -> ShardUrlGetReturn:
     request = Request(
         "GET",
-        adapter.get_api_base() / f"gateway/bot",
+        adapter.get_api_base() / "gateway/bot",
         headers={"Authorization": adapter.get_authorization(bot.bot_info)},
     )
     return parse_obj_as(ShardUrlGetReturn, await _request(adapter, bot, request))
 
 
 async def _put_message_reaction(
     adapter: "Adapter", bot: "Bot", channel_id: int, message_id: str, type: int, id: str
```

### Comparing `nonebot_adapter_qqguild-0.2.3/nonebot/adapters/qqguild/api/request.py` & `nonebot_adapter_qqguild-0.2.4/nonebot/adapters/qqguild/api/request.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_qqguild-0.2.3/nonebot/adapters/qqguild/api/utils.py` & `nonebot_adapter_qqguild-0.2.4/nonebot/adapters/qqguild/api/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_qqguild-0.2.3/nonebot/adapters/qqguild/bot.py` & `nonebot_adapter_qqguild-0.2.4/nonebot/adapters/qqguild/bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,16 @@
         bot: Bot 对象
         event: MessageEvent 对象
     """
     if event.message_reference is None:
         return
     try:
         event.reply = await bot.get_message_of_id(
-            channel_id=event.channel_id, message_id=event.message_reference.message_id  # type: ignore
+            channel_id=event.channel_id,  # type: ignore
+            message_id=event.message_reference.message_id,  # type: ignore
         )
         if event.reply.message.author.id == bot.self_info.id:  # type: ignore
             event.to_me = True
     except Exception as e:
         log("WARNING", f"Error when getting message reply info: {repr(e)}", e)
```

### Comparing `nonebot_adapter_qqguild-0.2.3/nonebot/adapters/qqguild/config.py` & `nonebot_adapter_qqguild-0.2.4/nonebot/adapters/qqguild/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_qqguild-0.2.3/nonebot/adapters/qqguild/event.py` & `nonebot_adapter_qqguild-0.2.4/nonebot/adapters/qqguild/event.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,15 +167,16 @@
     @overrides(Event)
     def get_user_id(self) -> str:
         return str(self.user.id)  # type: ignore
 
     @overrides(Event)
     def get_event_description(self) -> str:
         return escape_tag(
-            f"Notice {getattr(self.user, 'username', None)}@[Guild:{self.guild_id}] Roles:{self.roles}"
+            f"Notice {getattr(self.user, 'username', None)}"
+            f"@[Guild:{self.guild_id}] Roles:{self.roles}"
         )
 
     @overrides(Event)
     def get_session_id(self) -> str:
         return str(self.user.id)  # type: ignore
 
 
@@ -213,15 +214,18 @@
     @overrides(Event)
     def get_session_id(self) -> str:
         return str(self.author.id)  # type: ignore
 
     @overrides(BaseEvent)
     def get_event_description(self) -> str:
         return escape_tag(
-            f"Message {self.id} from {getattr(self.author, 'username', None)}@[Guild:{self.guild_id}/{self.channel_id}] Roles:{getattr(self.member, 'roles', None)}: {self.get_message()}"
+            f"Message {self.id} from "
+            f"{getattr(self.author, 'username', None)}"
+            f"@[Guild:{self.guild_id}/{self.channel_id}] "
+            f"Roles:{getattr(self.member, 'roles', None)}: {self.get_message()}"
         )
 
     @overrides(Event)
     def get_message(self) -> Message:
         if not hasattr(self, "_message"):
             setattr(self, "_message", Message.from_guild_message(self))
         return getattr(self, "_message")
@@ -255,15 +259,16 @@
 class DirectMessageCreateEvent(MessageEvent):
     __type__ = EventType.DIRECT_MESSAGE_CREATE
     to_me: bool = True
 
     @overrides(MessageEvent)
     def get_event_description(self) -> str:
         return escape_tag(
-            f"Message {self.id} from {getattr(self.author, 'username', None)}: {self.get_message()}"
+            f"Message {self.id} from "
+            f"{getattr(self.author, 'username', None)}: {self.get_message()}"
         )
 
 
 class DirectMessageDeleteEvent(MessageDeleteEvent):
     __type__ = EventType.DIRECT_MESSAGE_DELETE
```

### Comparing `nonebot_adapter_qqguild-0.2.3/nonebot/adapters/qqguild/exception.py` & `nonebot_adapter_qqguild-0.2.4/nonebot/adapters/qqguild/exception.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_qqguild-0.2.3/nonebot/adapters/qqguild/message.py` & `nonebot_adapter_qqguild-0.2.4/nonebot/adapters/qqguild/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,23 +156,23 @@
     def get_segment_class(cls) -> Type[MessageSegment]:
         return MessageSegment
 
     @overrides(BaseMessage)
     def __add__(
         self, other: Union[str, MessageSegment, Iterable[MessageSegment]]
     ) -> "Message":
-        return super(Message, self).__add__(
+        return super().__add__(
             MessageSegment.text(other) if isinstance(other, str) else other
         )
 
     @overrides(BaseMessage)
     def __radd__(
         self, other: Union[str, MessageSegment, Iterable[MessageSegment]]
     ) -> "Message":
-        return super(Message, self).__radd__(
+        return super().__radd__(
             MessageSegment.text(other) if isinstance(other, str) else other
         )
 
     @staticmethod
     @overrides(BaseMessage)
     def _construct(msg: str) -> Iterable[MessageSegment]:
         text_begin = 0
```

### Comparing `nonebot_adapter_qqguild-0.2.3/nonebot/adapters/qqguild/payload.py` & `nonebot_adapter_qqguild-0.2.4/nonebot/adapters/qqguild/payload.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_qqguild-0.2.3/nonebot/adapters/qqguild/permission.py` & `nonebot_adapter_qqguild-0.2.4/nonebot/adapters/qqguild/permission.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_qqguild-0.2.3/nonebot/adapters/qqguild/store.py` & `nonebot_adapter_qqguild-0.2.4/nonebot/adapters/qqguild/store.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_qqguild-0.2.3/nonebot/adapters/qqguild/transformer.py` & `nonebot_adapter_qqguild-0.2.4/nonebot/adapters/qqguild/transformer.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_qqguild-0.2.3/pyproject.toml` & `nonebot_adapter_qqguild-0.2.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 [tool.poetry]
 name = "nonebot-adapter-qqguild"
-version = "0.2.3"
+version = "0.2.4"
 description = "QQ Guild adapter for nonebot2"
 authors = ["yanyongyu <yyy@nonebot.dev>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/nonebot/adapter-qqguild"
 repository = "https://github.com/nonebot/adapter-qqguild"
 documentation = "https://github.com/nonebot/adapter-qqguild#readme"
 keywords = ["bot", "qq", "qqbot", "qqguild"]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Framework :: Robot Framework",
   "Framework :: Robot Framework :: Library",
   "Operating System :: OS Independent",
-  "Programming Language :: Python :: 3"
-]
-packages = [
-  { include = "nonebot" }
+  "Programming Language :: Python :: 3",
 ]
+packages = [{ include = "nonebot" }]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pydantic = "^1.9.0"
 nonebot2 = "^2.0.0-beta.1"
 
 [tool.poetry.group.dev.dependencies]
 isort = "^5.10.1"
+ruff = "^0.0.282"
 black = "^23.1.0"
 Jinja2 = "^3.0.3"
 nonemoji = "^0.1.3"
 pre-commit = "^3.3.0"
 httpx = ">=0.22.0, <1.0.0"
 nonebot2 = { git = "https://github.com/nonebot/nonebot2.git" }
 
@@ -44,21 +43,29 @@
 profile = "black"
 line_length = 88
 length_sort = true
 skip_gitignore = true
 force_sort_within_sections = true
 extra_standard_library = ["typing_extensions"]
 
-[tool.pycln]
-path = "."
-all = false
+[tool.ruff]
+select = ["E", "W", "F", "UP", "C", "T", "Q"]
+ignore = ["E402", "F403", "F405", "C901", "UP037"]
+
+line-length = 88
+target-version = "py38"
 
 [tool.pyright]
-pythonVersion = "3.8"
 pythonPlatform = "All"
+executionEnvironments = [
+  { root = "./codegen", pythonVersion = "3.10" },
+  { root = "./", pythonVersion = "3.8", extraPaths = [
+    "./",
+  ] },
+]
 
 [tool.codegen]
 url = "https://cdn.jsdelivr.net/gh/tencent-connect/bot-oas/v1/openapi.yaml"
 model-output = "nonebot/adapters/qqguild/api/model.py"
 client-output = "nonebot/adapters/qqguild/api/client.py"
 handle-output = "nonebot/adapters/qqguild/api/handle.py"
```

### Comparing `nonebot_adapter_qqguild-0.2.3/PKG-INFO` & `nonebot_adapter_qqguild-0.2.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-adapter-qqguild
-Version: 0.2.3
+Version: 0.2.4
 Summary: QQ Guild adapter for nonebot2
 Home-page: https://github.com/nonebot/adapter-qqguild
 License: MIT
 Keywords: bot,qq,qqbot,qqguild
 Author: yanyongyu
 Author-email: yyy@nonebot.dev
 Requires-Python: >=3.8,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-adapter-qqguild Version: 0.2.3 Summary: QQ
+Metadata-Version: 2.1 Name: nonebot-adapter-qqguild Version: 0.2.4 Summary: QQ
 Guild adapter for nonebot2 Home-page: https://github.com/nonebot/adapter-
 qqguild License: MIT Keywords: bot,qq,qqbot,qqguild Author: yanyongyu Author-
 email: yyy@nonebot.dev Requires-Python: >=3.8,<4.0 Classifier: Development
 Status :: 5 - Production/Stable Classifier: Framework :: Robot Framework
 Classifier: Framework :: Robot Framework :: Library Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
```

