# Comparing `tmp/nonebot_plugin_chatrecorder-0.2.5.tar.gz` & `tmp/nonebot_plugin_chatrecorder-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_chatrecorder-0.2.5.tar", max compression
+gzip compressed data, was "nonebot_plugin_chatrecorder-0.3.0.tar", max compression
```

## Comparing `nonebot_plugin_chatrecorder-0.2.5.tar` & `nonebot_plugin_chatrecorder-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,25 @@
--rw-r--r--   0        0        0     2979 2023-07-26 15:06:50.802185 nonebot_plugin_chatrecorder-0.2.5/README.md
--rw-r--r--   0        0        0      602 2023-07-26 15:06:50.802185 nonebot_plugin_chatrecorder-0.2.5/nonebot_plugin_chatrecorder/__init__.py
--rw-r--r--   0        0        0       37 2023-07-26 15:06:50.802185 nonebot_plugin_chatrecorder-0.2.5/nonebot_plugin_chatrecorder/adapters/__init__.py
--rw-r--r--   0        0        0     4855 2023-07-26 15:06:50.802185 nonebot_plugin_chatrecorder-0.2.5/nonebot_plugin_chatrecorder/adapters/onebot_v11.py
--rw-r--r--   0        0        0     3327 2023-07-26 15:06:50.802185 nonebot_plugin_chatrecorder-0.2.5/nonebot_plugin_chatrecorder/adapters/onebot_v12.py
--rw-r--r--   0        0        0      317 2023-07-26 15:06:50.802185 nonebot_plugin_chatrecorder-0.2.5/nonebot_plugin_chatrecorder/config.py
--rw-r--r--   0        0        0      483 2023-07-26 15:06:50.802185 nonebot_plugin_chatrecorder-0.2.5/nonebot_plugin_chatrecorder/consts.py
--rw-r--r--   0        0        0      402 2023-07-26 15:06:50.802185 nonebot_plugin_chatrecorder-0.2.5/nonebot_plugin_chatrecorder/exception.py
--rw-r--r--   0        0        0     1859 2023-07-26 15:06:50.802185 nonebot_plugin_chatrecorder-0.2.5/nonebot_plugin_chatrecorder/message.py
--rw-r--r--   0        0        0     1703 2023-07-26 15:06:50.802185 nonebot_plugin_chatrecorder-0.2.5/nonebot_plugin_chatrecorder/migrations/2cad88d938f1_init_db.py
--rw-r--r--   0        0        0     3732 2023-07-26 15:06:50.802185 nonebot_plugin_chatrecorder-0.2.5/nonebot_plugin_chatrecorder/migrations/7228a3a08576_ob12.py
--rw-r--r--   0        0        0     1517 2023-07-26 15:06:50.802185 nonebot_plugin_chatrecorder-0.2.5/nonebot_plugin_chatrecorder/migrations/9bca28bcb998_msg_type.py
--rw-r--r--   0        0        0     1731 2023-07-26 15:06:50.802185 nonebot_plugin_chatrecorder-0.2.5/nonebot_plugin_chatrecorder/model.py
--rw-r--r--   0        0        0     6206 2023-07-26 15:06:50.802185 nonebot_plugin_chatrecorder-0.2.5/nonebot_plugin_chatrecorder/record.py
--rw-r--r--   0        0        0     2587 2023-07-26 15:06:50.802185 nonebot_plugin_chatrecorder-0.2.5/nonebot_plugin_chatrecorder/record.pyi
--rw-r--r--   0        0        0      365 2023-07-26 15:06:50.802185 nonebot_plugin_chatrecorder-0.2.5/nonebot_plugin_chatrecorder/utils.py
--rw-r--r--   0        0        0     1183 2023-07-26 15:06:50.806185 nonebot_plugin_chatrecorder-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     3789 1970-01-01 00:00:00.000000 nonebot_plugin_chatrecorder-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     4619 2023-08-07 07:53:10.082179 nonebot_plugin_chatrecorder-0.3.0/README.md
+-rw-r--r--   0        0        0     1031 2023-08-07 07:53:10.082179 nonebot_plugin_chatrecorder-0.3.0/nonebot_plugin_chatrecorder/__init__.py
+-rw-r--r--   0        0        0       75 2023-08-07 07:53:10.082179 nonebot_plugin_chatrecorder-0.3.0/nonebot_plugin_chatrecorder/adapters/__init__.py
+-rw-r--r--   0        0        0     4528 2023-08-07 07:53:10.082179 nonebot_plugin_chatrecorder-0.3.0/nonebot_plugin_chatrecorder/adapters/console.py
+-rw-r--r--   0        0        0     4908 2023-08-07 07:53:10.082179 nonebot_plugin_chatrecorder-0.3.0/nonebot_plugin_chatrecorder/adapters/kaiheila.py
+-rw-r--r--   0        0        0     5209 2023-08-07 07:53:10.082179 nonebot_plugin_chatrecorder-0.3.0/nonebot_plugin_chatrecorder/adapters/onebot_v11.py
+-rw-r--r--   0        0        0     3675 2023-08-07 07:53:10.086180 nonebot_plugin_chatrecorder-0.3.0/nonebot_plugin_chatrecorder/adapters/onebot_v12.py
+-rw-r--r--   0        0        0     4150 2023-08-07 07:53:10.086180 nonebot_plugin_chatrecorder-0.3.0/nonebot_plugin_chatrecorder/adapters/qqguild.py
+-rw-r--r--   0        0        0     5091 2023-08-07 07:53:10.086180 nonebot_plugin_chatrecorder-0.3.0/nonebot_plugin_chatrecorder/adapters/telegram.py
+-rw-r--r--   0        0        0      317 2023-08-07 07:53:10.086180 nonebot_plugin_chatrecorder-0.3.0/nonebot_plugin_chatrecorder/config.py
+-rw-r--r--   0        0        0      766 2023-08-07 07:53:10.086180 nonebot_plugin_chatrecorder-0.3.0/nonebot_plugin_chatrecorder/consts.py
+-rw-r--r--   0        0        0      402 2023-08-07 07:53:10.086180 nonebot_plugin_chatrecorder-0.3.0/nonebot_plugin_chatrecorder/exception.py
+-rw-r--r--   0        0        0     2389 2023-08-07 07:53:10.086180 nonebot_plugin_chatrecorder-0.3.0/nonebot_plugin_chatrecorder/message.py
+-rw-r--r--   0        0        0     1703 2023-08-07 07:53:10.086180 nonebot_plugin_chatrecorder-0.3.0/nonebot_plugin_chatrecorder/migrations/2cad88d938f1_init_db.py
+-rw-r--r--   0        0        0     1917 2023-08-07 07:53:10.086180 nonebot_plugin_chatrecorder-0.3.0/nonebot_plugin_chatrecorder/migrations/44cce443d2c0_drop_column.py
+-rw-r--r--   0        0        0     3732 2023-08-07 07:53:10.086180 nonebot_plugin_chatrecorder-0.3.0/nonebot_plugin_chatrecorder/migrations/7228a3a08576_ob12.py
+-rw-r--r--   0        0        0     2992 2023-08-07 07:53:10.086180 nonebot_plugin_chatrecorder-0.3.0/nonebot_plugin_chatrecorder/migrations/902a51ac4032_add_session.py
+-rw-r--r--   0        0        0     1517 2023-08-07 07:53:10.086180 nonebot_plugin_chatrecorder-0.3.0/nonebot_plugin_chatrecorder/migrations/9bca28bcb998_msg_type.py
+-rw-r--r--   0        0        0     1165 2023-08-07 07:53:10.086180 nonebot_plugin_chatrecorder-0.3.0/nonebot_plugin_chatrecorder/migrations/de6827ead8fe_foreignkey.py
+-rw-r--r--   0        0        0     1429 2023-08-07 07:53:10.086180 nonebot_plugin_chatrecorder-0.3.0/nonebot_plugin_chatrecorder/model.py
+-rw-r--r--   0        0        0     9675 2023-08-07 07:53:10.086180 nonebot_plugin_chatrecorder-0.3.0/nonebot_plugin_chatrecorder/record.py
+-rw-r--r--   0        0        0     4624 2023-08-07 07:53:10.086180 nonebot_plugin_chatrecorder-0.3.0/nonebot_plugin_chatrecorder/record.pyi
+-rw-r--r--   0        0        0      273 2023-08-07 07:53:10.086180 nonebot_plugin_chatrecorder-0.3.0/nonebot_plugin_chatrecorder/utils.py
+-rw-r--r--   0        0        0     1402 2023-08-07 07:53:10.086180 nonebot_plugin_chatrecorder-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5484 1970-01-01 00:00:00.000000 nonebot_plugin_chatrecorder-0.3.0/PKG-INFO
```

### Comparing `nonebot_plugin_chatrecorder-0.2.5/nonebot_plugin_chatrecorder/adapters/onebot_v11.py` & `nonebot_plugin_chatrecorder-0.3.0/nonebot_plugin_chatrecorder/adapters/onebot_v11.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,109 +2,112 @@
 import hashlib
 from datetime import datetime
 from pathlib import Path
 from typing import Any, Dict, Optional, Type
 
 from nonebot.adapters import Bot as BaseBot
 from nonebot.message import event_postprocessor
-from nonebot.typing import overrides
 from nonebot_plugin_datastore import create_session
+from nonebot_plugin_session import Session, SessionLevel, extract_session
+from nonebot_plugin_session.model import get_or_add_session_model
+from typing_extensions import override
 
 from ..config import plugin_config
 from ..consts import (
     IMAGE_CACHE_DIR,
     RECORD_CACHE_DIR,
     VIDEO_CACHE_DIR,
     SupportedAdapter,
+    SupportedPlatform,
 )
 from ..message import (
     JsonMsg,
     MessageDeserializer,
     MessageSerializer,
     register_deserializer,
     register_serializer,
     serialize_message,
 )
 from ..model import MessageRecord
 
 try:
-    from nonebot.adapters.onebot.v11 import (
-        Bot,
-        GroupMessageEvent,
-        Message,
-        MessageEvent,
-        MessageSegment,
-    )
+    from nonebot.adapters.onebot.v11 import Bot, Message, MessageEvent, MessageSegment
+
+    adapter = SupportedAdapter.onebot_v11
 
     @event_postprocessor
     async def record_recv_msg(bot: Bot, event: MessageEvent):
+        session = extract_session(bot, event)
+        async with create_session() as db_session:
+            session_model = await get_or_add_session_model(session, db_session)
+
         record = MessageRecord(
-            bot_type=bot.type,
-            bot_id=bot.self_id,
-            platform="qq",
+            session_id=session_model.id,
             time=datetime.utcfromtimestamp(event.time),
             type=event.post_type,
-            detail_type=event.message_type,
             message_id=str(event.message_id),
-            message=serialize_message(bot, event.message),
+            message=serialize_message(adapter, event.message),
             plain_text=event.message.extract_plain_text(),
-            user_id=str(event.user_id),
-            group_id=str(event.group_id)
-            if isinstance(event, GroupMessageEvent)
-            else None,
         )
-
-        async with create_session() as session:
-            session.add(record)
-            await session.commit()
+        async with create_session() as db_session:
+            db_session.add(record)
+            await db_session.commit()
 
     if plugin_config.chatrecorder_record_send_msg:
 
         @Bot.on_called_api
         async def record_send_msg(
             bot: BaseBot,
             e: Optional[Exception],
             api: str,
             data: Dict[str, Any],
             result: Optional[Dict[str, Any]],
         ):
+            if not isinstance(bot, Bot):
+                return
             if e or not result:
                 return
             if api not in ["send_msg", "send_private_msg", "send_group_msg"]:
                 return
 
             if api == "send_group_msg" or (
                 api == "send_msg"
                 and (
                     data.get("message_type") == "group"
                     or (data.get("message_type") == None and data.get("group_id"))
                 )
             ):
-                detail_type = "group"
+                level = SessionLevel.LEVEL2
             else:
-                detail_type = "private"
+                level = SessionLevel.LEVEL1
+
+            session = Session(
+                bot_id=bot.self_id,
+                bot_type=bot.type,
+                platform=SupportedPlatform.qq,
+                level=level,
+                id1=str(data.get("user_id", "")) or None,
+                id2=str(data.get("group_id", "")) or None,
+                id3=None,
+            )
+            async with create_session() as db_session:
+                session_model = await get_or_add_session_model(session, db_session)
 
             message = Message(data["message"])
             record = MessageRecord(
-                bot_type=bot.type,
-                bot_id=bot.self_id,
-                platform="qq",
+                session_id=session_model.id,
                 time=datetime.utcnow(),
                 type="message_sent",
-                detail_type=detail_type,
                 message_id=str(result["message_id"]),
-                message=serialize_message(bot, message),
+                message=serialize_message(adapter, message),
                 plain_text=message.extract_plain_text(),
-                user_id=str(bot.self_id),
-                group_id=str(data.get("group_id", "")) or None,
             )
-
-            async with create_session() as session:
-                session.add(record)
-                await session.commit()
+            async with create_session() as db_session:
+                db_session.add(record)
+                await db_session.commit()
 
     def cache_b64_msg(msg: Message):
         for seg in msg:
             if seg.type == "image":
                 cache_b64_msg_seg(seg, IMAGE_CACHE_DIR)
             elif seg.type == "record":
                 cache_b64_msg_seg(seg, RECORD_CACHE_DIR)
@@ -129,24 +132,23 @@
         else:
             with cache_file_path.open("wb") as f:
                 f.write(data)
             replace_seg_file(cache_file_path)
 
     class Serializer(MessageSerializer[Message]):
         @classmethod
-        @overrides(MessageSerializer)
+        @override
         def serialize(cls, msg: Message) -> JsonMsg:
             cache_b64_msg(msg)
             return super().serialize(msg)
 
     class Deserializer(MessageDeserializer[Message]):
         @classmethod
-        @overrides(MessageDeserializer)
+        @override
         def get_message_class(cls) -> Type[Message]:
             return Message
 
-    adapter = SupportedAdapter.onebot_v11
     register_serializer(adapter, Serializer)
     register_deserializer(adapter, Deserializer)
 
 except ImportError:
     pass
```

### Comparing `nonebot_plugin_chatrecorder-0.2.5/nonebot_plugin_chatrecorder/adapters/onebot_v12.py` & `nonebot_plugin_chatrecorder-0.3.0/nonebot_plugin_chatrecorder/adapters/onebot_v12.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,104 +1,109 @@
 from datetime import datetime
 from typing import Any, Dict, Optional, Type
 
 from nonebot.adapters import Bot as BaseBot
 from nonebot.message import event_postprocessor
-from nonebot.typing import overrides
 from nonebot_plugin_datastore import create_session
+from nonebot_plugin_session import Session, SessionLevel, extract_session
+from nonebot_plugin_session.model import get_or_add_session_model
+from typing_extensions import override
 
 from ..config import plugin_config
 from ..consts import SupportedAdapter
 from ..message import (
     MessageDeserializer,
     MessageSerializer,
     register_deserializer,
     register_serializer,
     serialize_message,
 )
 from ..model import MessageRecord
 
 try:
-    from nonebot.adapters.onebot.v12 import (
-        Bot,
-        ChannelMessageEvent,
-        GroupMessageEvent,
-        Message,
-        MessageEvent,
-    )
+    from nonebot.adapters.onebot.v12 import Bot, Message, MessageEvent
+
+    adapter = SupportedAdapter.onebot_v12
 
     @event_postprocessor
     async def record_recv_msg(bot: Bot, event: MessageEvent):
+        session = extract_session(bot, event)
+        async with create_session() as db_session:
+            session_model = await get_or_add_session_model(session, db_session)
+
         record = MessageRecord(
-            bot_type=bot.type,
-            bot_id=bot.self_id,
-            platform=bot.platform,
+            session_id=session_model.id,
             time=event.time,
             type=event.type,
-            detail_type=event.detail_type,
             message_id=event.message_id,
-            message=serialize_message(bot, event.message),
+            message=serialize_message(adapter, event.message),
             plain_text=event.message.extract_plain_text(),
-            user_id=event.user_id,
-            group_id=event.group_id if isinstance(event, GroupMessageEvent) else None,
-            guild_id=event.guild_id if isinstance(event, ChannelMessageEvent) else None,
-            channel_id=event.channel_id
-            if isinstance(event, ChannelMessageEvent)
-            else None,
         )
-
-        async with create_session() as session:
-            session.add(record)
-            await session.commit()
+        async with create_session() as db_session:
+            db_session.add(record)
+            await db_session.commit()
 
     if plugin_config.chatrecorder_record_send_msg:
 
         @Bot.on_called_api
         async def record_send_msg(
             bot: BaseBot,
             e: Optional[Exception],
             api: str,
             data: Dict[str, Any],
             result: Optional[Dict[str, Any]],
         ):
+            if not isinstance(bot, Bot):
+                return
             if e or not result:
                 return
             if api not in ["send_message"]:
                 return
-            assert isinstance(bot, Bot)
 
-            message = Message(data["message"])
-            record = MessageRecord(
-                bot_type=bot.type,
+            detail_type = data["detail_type"]
+            level = SessionLevel.LEVEL0
+            if detail_type == "channel":
+                level = SessionLevel.LEVEL3
+            elif detail_type == "group":
+                level = SessionLevel.LEVEL2
+            elif detail_type == "private":
+                level = SessionLevel.LEVEL1
+
+            session = Session(
                 bot_id=bot.self_id,
+                bot_type=bot.type,
                 platform=bot.platform,
+                level=level,
+                id1=data.get("user_id"),
+                id2=data.get("group_id") or data.get("channel_id"),
+                id3=data.get("guild_id"),
+            )
+            async with create_session() as db_session:
+                session_model = await get_or_add_session_model(session, db_session)
+
+            message = Message(data["message"])
+            record = MessageRecord(
+                session_id=session_model.id,
                 time=datetime.utcfromtimestamp(result["time"]),
                 type="message_sent",
-                detail_type=data["detail_type"],
                 message_id=result["message_id"],
-                message=serialize_message(bot, message),
+                message=serialize_message(adapter, message),
                 plain_text=message.extract_plain_text(),
-                user_id=str(bot.self_id),
-                group_id=data.get("group_id"),
-                guild_id=data.get("guild_id"),
-                channel_id=data.get("channel_id"),
             )
-
-            async with create_session() as session:
-                session.add(record)
-                await session.commit()
+            async with create_session() as db_session:
+                db_session.add(record)
+                await db_session.commit()
 
     class Serializer(MessageSerializer[Message]):
         pass
 
     class Deserializer(MessageDeserializer[Message]):
         @classmethod
-        @overrides(MessageDeserializer)
+        @override
         def get_message_class(cls) -> Type[Message]:
             return Message
 
-    adapter = SupportedAdapter.onebot_v12
     register_serializer(adapter, Serializer)
     register_deserializer(adapter, Deserializer)
 
 except ImportError:
     pass
```

### Comparing `nonebot_plugin_chatrecorder-0.2.5/nonebot_plugin_chatrecorder/migrations/2cad88d938f1_init_db.py` & `nonebot_plugin_chatrecorder-0.3.0/nonebot_plugin_chatrecorder/migrations/2cad88d938f1_init_db.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_chatrecorder-0.2.5/nonebot_plugin_chatrecorder/migrations/7228a3a08576_ob12.py` & `nonebot_plugin_chatrecorder-0.3.0/nonebot_plugin_chatrecorder/migrations/7228a3a08576_ob12.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_chatrecorder-0.2.5/nonebot_plugin_chatrecorder/migrations/9bca28bcb998_msg_type.py` & `nonebot_plugin_chatrecorder-0.3.0/nonebot_plugin_chatrecorder/migrations/9bca28bcb998_msg_type.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_chatrecorder-0.2.5/pyproject.toml` & `nonebot_plugin_chatrecorder-0.3.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [tool.poetry]
 name = "nonebot_plugin_chatrecorder"
-version = "0.2.5"
+version = "0.3.0"
 description = "适用于 Nonebot2 的聊天记录插件"
 authors = ["meetwq <meetwq@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/noneplugin/nonebot-plugin-chatrecorder"
 repository = "https://github.com/noneplugin/nonebot-plugin-chatrecorder"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 nonebot2 = { version = "^2.0.0", extras = ["fastapi"] }
-nonebot-plugin-datastore = "^1.0.0"
+nonebot-plugin-datastore = "^1.1.0"
+nonebot-plugin-session = ">=0.0.8,<0.1.0"
 
 [tool.poetry.group.dev.dependencies]
 nb-cli = "^1.0.0"
 black = "^22.8.0"
 
 [tool.poetry.group.test.dependencies]
 pytest-cov = "^4.0.0"
@@ -26,15 +27,19 @@
 asyncpg = "^0.27.0"
 aiomysql = "^0.1.0"
 
 [tool.poetry.group.adapters]
 optional = true
 
 [tool.poetry.group.adapters.dependencies]
-nonebot-adapter-onebot = "^2.2.0"
+nonebot-adapter-onebot = "^2.2.2"
+nonebot-adapter-console = "^0.4.0"
+nonebot-adapter-qqguild = "^0.2.1"
+nonebot-adapter-kaiheila = { version = "^0.2.4", python = ">=3.9" }
+nonebot-adapter-telegram = "^0.1.0b13"
 
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
 addopts = "--cov=nonebot_plugin_chatrecorder --cov-report=term-missing"
 
 [tool.nonebot]
 plugins = ["nonebot_plugin_chatrecorder"]
```

