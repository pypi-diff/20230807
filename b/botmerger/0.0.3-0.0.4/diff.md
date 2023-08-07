# Comparing `tmp/botmerger-0.0.3.tar.gz` & `tmp/botmerger-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botmerger-0.0.3.tar", max compression
+gzip compressed data, was "botmerger-0.0.4.tar", max compression
```

## Comparing `botmerger-0.0.3.tar` & `botmerger-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1079 2023-05-20 19:54:52.435984 botmerger-0.0.3/LICENSE
--rw-r--r--   0        0        0     2098 2023-06-22 08:17:38.883841 botmerger-0.0.3/README.md
--rw-r--r--   0        0        0      533 2023-06-20 18:36:34.559558 botmerger-0.0.3/botmerger/__init__.py
--rw-r--r--   0        0        0    10173 2023-06-20 18:36:34.560532 botmerger-0.0.3/botmerger/base.py
--rw-r--r--   0        0        0    11578 2023-06-20 18:36:34.561088 botmerger-0.0.3/botmerger/core.py
--rw-r--r--   0        0        0     1017 2023-06-20 18:36:34.561493 botmerger-0.0.3/botmerger/errors.py
--rw-r--r--   0        0        0        0 2023-06-20 18:36:34.561562 botmerger-0.0.3/botmerger/experimental/__init__.py
--rw-r--r--   0        0        0      464 2023-06-20 18:36:34.562351 botmerger-0.0.3/botmerger/experimental/inquiry_bot.py
--rw-r--r--   0        0        0        0 2023-06-20 18:36:34.562427 botmerger-0.0.3/botmerger/ext/__init__.py
--rw-r--r--   0        0        0     3456 2023-06-20 18:58:55.311347 botmerger-0.0.3/botmerger/ext/discord_integration.py
--rw-r--r--   0        0        0     5921 2023-06-20 18:36:34.563650 botmerger-0.0.3/botmerger/models.py
--rw-r--r--   0        0        0      507 2023-06-20 18:36:34.564717 botmerger-0.0.3/botmerger/utils.py
--rw-r--r--   0        0        0      660 2023-06-22 18:31:31.738368 botmerger-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2561 1970-01-01 00:00:00.000000 botmerger-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1079 2023-05-20 19:54:52.435984 botmerger-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2091 2023-07-08 07:27:42.629913 botmerger-0.0.4/README.md
+-rw-r--r--   0        0        0      497 2023-07-08 07:27:42.630729 botmerger-0.0.4/botmerger/__init__.py
+-rw-r--r--   0        0        0    14531 2023-08-07 17:18:36.860589 botmerger-0.0.4/botmerger/base.py
+-rw-r--r--   0        0        0    18011 2023-08-07 17:18:36.861601 botmerger-0.0.4/botmerger/core.py
+-rw-r--r--   0        0        0     1017 2023-06-20 18:36:34.561493 botmerger-0.0.4/botmerger/errors.py
+-rw-r--r--   0        0        0        0 2023-06-20 18:36:34.561562 botmerger-0.0.4/botmerger/experimental/__init__.py
+-rw-r--r--   0        0        0      501 2023-08-07 17:18:36.862555 botmerger-0.0.4/botmerger/experimental/inquiry_bot.py
+-rw-r--r--   0        0        0        0 2023-06-20 18:36:34.562427 botmerger-0.0.4/botmerger/ext/__init__.py
+-rw-r--r--   0        0        0     3384 2023-08-07 17:18:36.863447 botmerger-0.0.4/botmerger/ext/discord_integration.py
+-rw-r--r--   0        0        0     6604 2023-08-07 17:18:36.864535 botmerger-0.0.4/botmerger/models.py
+-rw-r--r--   0        0        0      507 2023-06-20 18:36:34.564717 botmerger-0.0.4/botmerger/utils.py
+-rw-r--r--   0        0        0      660 2023-08-07 17:18:36.867690 botmerger-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2554 1970-01-01 00:00:00.000000 botmerger-0.0.4/PKG-INFO
```

### Comparing `botmerger-0.0.3/LICENSE` & `botmerger-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `botmerger-0.0.3/README.md` & `botmerger-0.0.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 BotMerger is a fully asynchronous Python framework designed as a messaging platform which allows Large Language Model
 (LLM)-based chatbots to interact with each other in order to "merge" into more complex bots capable of fulfilling
 non-trivial user requests.
 
 ## 📦 Installation
 
 ```shell
-pip install --upgrade botmerger
+pip install -U botmerger
 ```
 
 ## 🚀 Quickstart
 
 TODO
 
 ## 💡 Philosophy
```

### Comparing `botmerger-0.0.3/botmerger/base.py` & `botmerger-0.0.4/botmerger/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,58 +1,99 @@
 # pylint: disable=no-name-in-module,too-many-arguments
 """Base classes for the BotMerger library."""
 from abc import ABC, abstractmethod
-from asyncio import Queue
-from typing import Any, TYPE_CHECKING, Optional, Dict, Callable, Awaitable, Union, List, Tuple
-from uuid import uuid4
+from asyncio import Queue, Lock
+from collections import abc
+from contextvars import ContextVar
+from contextvars import Token
+from typing import (
+    Any,
+    TYPE_CHECKING,
+    Optional,
+    Dict,
+    Callable,
+    Awaitable,
+    Union,
+    List,
+    Tuple,
+    Iterable,
+    AsyncIterable,
+)
+from uuid import uuid4, UUID
 
 from pydantic import BaseModel, UUID4, Field
 
 from botmerger.errors import ErrorWrapper
 
 if TYPE_CHECKING:
-    from botmerger.models import MergedBot, MergedChannel, MergedMessage, MergedParticipant
+    from botmerger.models import MergedBot, MergedMessage, MergedParticipant, MergedUser
 
 SingleTurnHandler = Callable[["SingleTurnContext"], Awaitable[None]]
 MessageContent = Union[str, BaseModel, Any]  # a string, a Pydantic model, a dataclass or a json-serializable object
 MessageType = Union["MergedMessage", MessageContent]
 ObjectKey = Union[UUID4, Tuple[Any, ...]]
 
 
 class BotMerger(ABC):
     """
     An abstract factory of everything else in this library and also the low level implementation of everything else
     in this library. Almost all the methods of almost all the other classes in this library are just a facade for
     methods of this class.
     """
 
+    DEFAULT_USER_UUID = UUID("440633de-aac2-41ae-80aa-7bbf1be7591b")
+    DEFAULT_MSG_CTX_UUID = UUID("0cff89d8-14a8-49c5-92c5-e5a6445bdb6c")
+
+    DEFAULT_USER_NAME = "USER"
+    DEFAULT_MSG_CTX_CONTENT = "DEFAULT MESSAGE CONTEXT"
+
+    async def get_default_user(self) -> "MergedUser":
+        """Get the default user."""
+
+    async def get_default_msg_ctx(self) -> "MergedMessage":
+        """Get the default message context."""
+
     @abstractmethod
-    async def trigger_bot(self, bot: "MergedBot", request: "MergedMessage") -> "BotResponses":
-        """Find a bot by its alias and trigger it with a request."""
+    def trigger_bot(
+        self,
+        bot: "MergedBot",
+        request: Optional[Union[MessageType, "BotResponses"]] = None,
+        requests: Optional[Iterable[Union[MessageType, "BotResponses"]]] = None,
+        override_sender: Optional["MergedParticipant"] = None,
+        override_parent_ctx: Optional["MergedMessage"] = None,
+        rewrite_cache: bool = False,
+        **kwargs,
+    ) -> "BotResponses":
+        """
+        Find a bot by its alias and trigger this bot to respond to a message or messages. Returns an object that can
+        be used to retrieve the bot's response(s) in an asynchronous manner.
+        """
 
     @abstractmethod
     def create_bot(
         self,
         alias: str,
         name: Optional[str] = None,
         description: Optional[str] = None,
+        no_cache: bool = False,
         single_turn: Optional[SingleTurnHandler] = None,
         **kwargs,
     ) -> "MergedBot":
         """
         Create a bot. This version of bot creation function is meant to be called outside an async context (for ex.
         as a decorator to single-turn and multi-turn handler functions).
         """
 
     @abstractmethod
     async def create_bot_async(
         self,
         alias: str,
         name: Optional[str] = None,
         description: Optional[str] = None,
+        no_cache: bool = False,
         single_turn: Optional[SingleTurnHandler] = None,
         **kwargs,
     ) -> "MergedBot":
         """Create a bot while inside an async context."""
 
     @abstractmethod
     def register_local_single_turn_handler(self, bot: "MergedBot", handler: SingleTurnHandler) -> None:
@@ -64,48 +105,36 @@
 
     @abstractmethod
     async def find_or_create_user_channel(
         self,
         channel_type: str,
         channel_id: Any,
         user_display_name: str,
-        **kwargs,
-    ) -> "MergedChannel":
+    ) -> "MergedMessage":
         """
-        Find or create a channel with a user as its owner. Parameters `channel_type` and `channel_specific_id` are
-        used to look up the channel. Parameter `user_display_name` is used to create a user if the channel does not
-        exist and is ignored if the channel already exists.
+        Find or create a channel with a user as its owner. The channel is represented by a MergedMessage object that
+        will serve as parent context for other MergedMessage objects (actual messages that are sent by the user
+        via this channel). Parameters `channel_type` and `channel_specific_id` are used to look up the channel.
+        Parameter `user_display_name` is used to create a user if the channel does not exist and is ignored if the
+        channel already exists.
         """
 
     @abstractmethod
-    async def create_message(
-        self,
-        thread_uuid: UUID4,
-        channel: "MergedChannel",
-        sender: "MergedParticipant",
-        content: "MessageType",
-        indicate_typing_afterwards: Optional[bool],
-        responds_to: Optional["MergedMessage"],
-        goes_after: Optional["MergedMessage"],
-        **kwargs,
-    ) -> "MergedMessage":
-        """
-        Create a message in a given channel. If `content` is another `MergedMessage` instance, then
-        `ForwardedMessage` will be created instead of `OriginalMessage`.
-        """
+    async def create_user(self, name: str, **kwargs) -> "MergedUser":
+        """Create a user."""
 
     @abstractmethod
     async def create_next_message(
         self,
-        thread_uuid: UUID4,
-        channel: "MergedChannel",
-        sender: "MergedParticipant",
         content: "MessageType",
-        indicate_typing_afterwards: Optional[bool],
-        responds_to: Optional["MergedMessage"],
+        still_thinking: Optional[bool],
+        sender: Optional["MergedParticipant"],
+        receiver: "MergedParticipant",
+        parent_context: Optional["MergedMessage"],
+        responds_to: Optional["MergedMessage"] = None,
         **kwargs,
     ) -> "MergedMessage":
         """
         Create a message in a given channel that goes after the last message in a given thread. If `content` is
         another `MergedMessage` instance, then `ForwardedMessage` will be created instead of `OriginalMessage`.
         """
 
@@ -158,107 +187,184 @@
         return self.uuid == other.uuid
 
     def __hash__(self) -> int:
         """The hash of the model is the hash of its uuid."""
         return hash(self.uuid)
 
 
+class BaseMessage:
+    """
+    Base class for messages. This is not a Pydantic model. `content` is property that must be implemented by
+    subclasses one way or another (either as a Pydantic field or as a property).
+    """
+
+    content: Union[str, Any]
+    original_message: "MergedMessage"
+
+
 class BotResponses:
     """
     A class that represents a stream of responses from a bot. It is an async iterator that yields `MergedMessage`
     objects. It also has a method `get_all_responses` that will block until all the responses are received and then
     return them as a list.
     """
 
     _END_OF_RESPONSES = object()
 
-    def __init__(self, request: "MergedMessage") -> None:
-        self.request = request
+    def __init__(self) -> None:
         self.responses_so_far: List["MergedMessage"] = []
-        self._response_queue: Optional[Queue[Union["MergedMessage", object, Exception]]] = Queue()
+        self._response_queue: Optional[Queue[Union["MergedMessage", object, Exception, "BotResponses"]]] = Queue()
         self._error: Optional[ErrorWrapper] = None
+        self._cached_bot_response_iterator: Optional[BotResponses._Iterator] = None
+        self._lock = Lock()
 
-    def __aiter__(self) -> "BotResponses":
-        return self
-
-    async def __anext__(self) -> "MergedMessage":
-        if self._error:
-            raise self._error
-
-        if self._response_queue is None:
-            raise StopAsyncIteration
-
-        response = await self._response_queue.get()
-
-        if isinstance(response, Exception):
-            self._error = ErrorWrapper(error=response)
-            raise self._error
-
-        if response is self._END_OF_RESPONSES:
-            self._response_queue = None
-            raise StopAsyncIteration
-
-        self.responses_so_far.append(response)
-        return response
+    def __aiter__(self) -> "BotResponses._Iterator":
+        return BotResponses._Iterator(self)
 
     async def get_all_responses(self) -> List["MergedMessage"]:
         """Wait until all the responses are received and return them as a list."""
         # make sure all responses are fetched
         async for _ in self:
             pass
         return self.responses_so_far
 
     async def get_final_response(self) -> Optional["MergedMessage"]:
         """Wait until all the responses are received and return the last one or None if there are no responses."""
         responses = await self.get_all_responses()
         return responses[-1] if responses else None
 
+    async def _wait_for_next_response(self) -> "MergedMessage":
+        if self._cached_bot_response_iterator is not None:
+            # we are yielding responses from a cached BotResponses instance
+            response = await anext(self._cached_bot_response_iterator)
+        else:
+            if self._error:
+                raise self._error
+
+            if self._response_queue is None:
+                raise StopAsyncIteration
+
+            response = await self._response_queue.get()
+
+            if isinstance(response, BotResponses):
+                # we are going to yield responses from a cached BotResponses instance
+                self._cached_bot_response_iterator = aiter(response)
+                response = await anext(self._cached_bot_response_iterator)
+
+            else:
+                if isinstance(response, Exception):
+                    self._error = ErrorWrapper(error=response)
+                    raise self._error
+
+                if response is self._END_OF_RESPONSES:
+                    self._response_queue = None
+                    raise StopAsyncIteration
+
+        self.responses_so_far.append(response)
+        return response
+
+    class _Iterator:
+        def __init__(self, bot_responses: "BotResponses") -> None:
+            self._bot_responses = bot_responses
+            self._index = 0
+
+        async def __anext__(self) -> "MergedMessage":
+            try:
+                response = self._bot_responses.responses_so_far[self._index]
+            except IndexError:
+                async with self._bot_responses._lock:
+                    try:
+                        response = self._bot_responses.responses_so_far[self._index]
+                    except IndexError:
+                        # this will also raise StopAsyncIteration if there are no more responses
+                        response = await self._bot_responses._wait_for_next_response()
+
+            self._index += 1
+            return response
+
 
 # noinspection PyProtectedMember
 class SingleTurnContext:
-    # pylint: disable=import-outside-toplevel,protected-access,too-many-arguments
+    # pylint: disable=protected-access,too-many-arguments
     """
     A context object that is passed to a single turn handler function. It is meant to be used as a facade for the
     `MergedBot` and `MergedMessage` objects. It also has a method `yield_response` that is meant to be used by the
     single turn handler function to yield a response to the request.
     """
 
+    requests: Tuple["MergedMessage"]
+
+    _previous_ctx_token: ContextVar[Token] = ContextVar("_previous_ctx_token")
+    _current_context: ContextVar[Optional["SingleTurnContext"]] = ContextVar("_current_context", default=None)
+
     def __init__(
         self,
         merger: BotMerger,
         this_bot: "MergedBot",
-        channel: "MergedChannel",
-        request: "MergedMessage",
         bot_responses: BotResponses,
     ) -> None:
         self.merger = merger
         self.this_bot = this_bot
-        self.channel = channel
-        self.request = request
+
         self._bot_responses = bot_responses
 
+    @property
+    def concluding_request(self) -> "MergedMessage":
+        """The last request that was sent to the bot."""
+        return self.requests[-1]
+
+    async def get_full_conversation(
+        self, max_length: Optional[int] = None, include_invisible_to_bots: bool = False
+    ) -> List["MergedMessage"]:
+        """Get the full conversation history for this message (including this message)."""
+        return await self.concluding_request.get_full_conversation(
+            max_length=max_length, include_invisible_to_bots=include_invisible_to_bots
+        )
+
     async def yield_response(
-        self, response: MessageType, indicate_typing_afterwards: Optional[bool] = None, **kwargs
+        self, response: MessageType, still_thinking: Optional[bool] = None, **kwargs
     ) -> "MergedMessage":
+        """Yield a response to the request."""
         response = await self.merger.create_next_message(
-            thread_uuid=self.request.thread_uuid,
-            channel=self.channel,
-            sender=self.this_bot,
             content=response,
-            indicate_typing_afterwards=indicate_typing_afterwards,
-            responds_to=self.request,
+            still_thinking=still_thinking,
+            sender=self.this_bot,
+            receiver=self.concluding_request.sender,
+            parent_context=self.concluding_request.parent_context,
+            responds_to=self.concluding_request,
             **kwargs,
         )
         self._bot_responses._response_queue.put_nowait(response)
         return response
 
     async def yield_interim_response(self, response: MessageType, **kwargs) -> "MergedMessage":
-        return await self.yield_response(response, indicate_typing_afterwards=True, **kwargs)
+        """Yield an interim response to the request."""
+        return await self.yield_response(response, still_thinking=True, **kwargs)
 
     async def yield_final_response(self, response: MessageType, **kwargs) -> "MergedMessage":
-        return await self.yield_response(response, indicate_typing_afterwards=False, **kwargs)
+        """Yield a final response to the request."""
+        return await self.yield_response(response, still_thinking=False, **kwargs)
 
     async def yield_from(
-        self, another_bot_responses: BotResponses, indicate_typing_afterwards: Optional[bool] = None
+        self,
+        iterable: Iterable[MessageType] | AsyncIterable[MessageType],
+        still_thinking: Optional[bool] = None,
     ) -> None:
-        async for response in another_bot_responses:
-            await self.yield_response(response, indicate_typing_afterwards=indicate_typing_afterwards)
+        """Yield responses to the request from an iterable."""
+        if isinstance(iterable, abc.AsyncIterable):
+            async for response in iterable:
+                await self.yield_response(response, still_thinking=still_thinking)
+        else:
+            for response in iterable:
+                await self.yield_response(response, still_thinking=still_thinking)
+
+    def __enter__(self) -> "SingleTurnContext":
+        """Set this context as the current context."""
+        # TODO emphasize that nesting contexts is not supported unless asyncio.create_task is used for each nesting
+        previous_ctx_token = self._current_context.set(self)  # <- this is the context switch
+        self._previous_ctx_token.set(previous_ctx_token)
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb) -> None:
+        """Restore the context that was current before this one."""
+        previous_ctx_token = self._previous_ctx_token.get()
+        self._current_context.reset(previous_ctx_token)
```

### Comparing `botmerger-0.0.3/botmerger/errors.py` & `botmerger-0.0.4/botmerger/errors.py`

 * *Files identical despite different names*

### Comparing `botmerger-0.0.3/botmerger/ext/discord_integration.py` & `botmerger-0.0.4/botmerger/ext/discord_integration.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,33 +20,31 @@
     async def on_message(discord_message: discord.Message) -> None:
         """Called when a message is sent to a channel (both a user message and a bot message)."""
         if discord_message.author == discord_client.user:
             # make sure we are not embarking on an infinite loop of responding to our own messages
             return
 
         try:
-            merged_channel = await bot.merger.find_or_create_user_channel(
+            channel_msg_ctx = await bot.merger.find_or_create_user_channel(
                 channel_type="discord",
                 channel_id=discord_message.channel.id,
                 user_display_name=discord_message.author.name,
             )
 
-            # prefix_command = discord_message.content.startswith("!")
-            # new_conversation = prefix_command
-
-            user_request = await merged_channel.next_message_from_owner(
+            bot_responses = bot.trigger(
                 discord_message.content,
+                override_sender=channel_msg_ctx.sender,
+                override_parent_ctx=channel_msg_ctx,
                 # extra_fields={
                 #     # TODO is this unsecure ? (given that MergedMessage objects will be passed around between
                 #     #  BotMerger distributed nodes in the future)
                 #     "discord_channel_id": discord_message.channel.id,
                 #     "discord_message_id": discord_message.id,
                 # },
             )
-            bot_responses = await bot.trigger(user_request)
 
             async for response in _iterate_over_responses(bot_responses, discord_message.channel.typing()):
                 response_content = response.content
                 if not isinstance(response_content, str):
                     try:
                         response_content = f"```json\n{json.dumps(response_content, indent=2)}\n```"
                     except Exception as exc:  # pylint: disable=broad-exception-caught
@@ -62,24 +60,26 @@
 
     discord_client.event(on_message)
 
 
 async def _iterate_over_responses(
     bot_responses: BotResponses, typing_context_manager: Any
 ) -> AsyncGenerator[MergedMessage, None]:
+    resp_iterator = aiter(bot_responses)
     response = None
+
     while True:
         try:
-            if not response or response.indicate_typing_afterwards:
+            if not response or response.still_thinking:
                 _typing_context_manager = typing_context_manager
             else:
                 _typing_context_manager = _null_context
 
             async with _typing_context_manager:
-                response = await anext(bot_responses)
+                response = await anext(resp_iterator)
 
         except StopAsyncIteration:
             return
 
         yield response
```

### Comparing `botmerger-0.0.3/botmerger/models.py` & `botmerger-0.0.4/botmerger/models.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,21 @@
-# pylint: disable=no-name-in-module
+# pylint: disable=no-name-in-module,too-many-arguments
 """Models for the BotMerger library."""
-from typing import Any, Optional, Union
-from uuid import uuid4
+from typing import Any, Optional, Union, Iterable, List
 
-from pydantic import Field, UUID4
+from pydantic import Field
 
-from botmerger.base import MergedObject, SingleTurnHandler, BotResponses, MessageContent, MessageType
+from botmerger.base import (
+    MergedObject,
+    SingleTurnHandler,
+    BotResponses,
+    MessageContent,
+    MessageType,
+    BaseMessage,
+)
 
 
 class MergedParticipant(MergedObject):
     """A chat participant."""
 
     name: str
     is_human: bool
@@ -18,63 +24,79 @@
 class MergedBot(MergedParticipant):
     """A bot that can interact with other bots."""
 
     is_human: bool = Field(False, const=True)
 
     alias: str
     description: Optional[str] = None
+    no_cache: bool = False
 
-    async def trigger(
+    def trigger(
         self,
-        request: MessageType,
-        sender: Optional["MergedParticipant"] = None,
-        channel: Optional["MergedChannel"] = None,
+        request: Optional[Union[MessageType, "BotResponses"]] = None,
+        requests: Optional[Iterable[Union[MessageType, "BotResponses"]]] = None,
+        override_sender: Optional[MergedParticipant] = None,
+        override_parent_ctx: Optional["MergedMessage"] = None,
+        rewrite_cache: bool = False,
         **kwargs,
     ) -> BotResponses:
         """
-        Trigger this bot to respond to a message. Returns an object that can be used to retrieve the bot's
+        Trigger this bot to respond to a message or messages. Returns an object that can be used to retrieve the bot's
         response(s) in an asynchronous manner.
         """
-        if isinstance(request, MergedMessage):
-            if sender:
-                raise ValueError("sender is not allowed if request is a MergedMessage")
-            if channel:
-                raise ValueError("channel is not allowed if request is a MergedMessage")
-            if kwargs:
-                raise ValueError("additional keyword arguments are not allowed if request is a MergedMessage")
-
-        else:
-            if not sender:
-                raise ValueError("sender is required if request is not a MergedMessage")
-            if not channel:
-                raise ValueError("channel is required if request is not a MergedMessage")
-
-            request = await self.merger.create_message(
-                thread_uuid=uuid4(),  # create a brand-new thread
-                channel=channel,
-                sender=sender,
-                content=request,
-                indicate_typing_afterwards=False,
-                responds_to=None,
-                goes_after=None,
-                **kwargs,
-            )
-        return await self.merger.trigger_bot(self, request)
+        return self.merger.trigger_bot(
+            bot=self,
+            request=request,
+            requests=requests,
+            override_sender=override_sender,
+            override_parent_ctx=override_parent_ctx,
+            rewrite_cache=rewrite_cache,
+            **kwargs,
+        )
 
     async def get_final_response(
         self,
-        request: MessageType,
-        sender: Optional["MergedParticipant"] = None,
-        channel: Optional["MergedChannel"] = None,
+        request: Optional[Union[MessageType, "BotResponses"]] = None,
+        requests: Optional[Iterable[Union[MessageType, "BotResponses"]]] = None,
+        override_sender: Optional[MergedParticipant] = None,
+        override_parent_ctx: Optional["MergedMessage"] = None,
+        rewrite_cache: bool = False,
         **kwargs,
     ) -> Optional["MergedMessage"]:
         """Get the final response from the bot for a given request."""
-        responses = await self.trigger(request, sender=sender, channel=channel, **kwargs)
+        responses = self.trigger(
+            request=request,
+            requests=requests,
+            override_sender=override_sender,
+            override_parent_ctx=override_parent_ctx,
+            rewrite_cache=rewrite_cache,
+            **kwargs,
+        )
         return await responses.get_final_response()
 
+    async def get_all_responses(
+        self,
+        request: Optional[Union[MessageType, "BotResponses"]] = None,
+        requests: Optional[Iterable[Union[MessageType, "BotResponses"]]] = None,
+        override_sender: Optional[MergedParticipant] = None,
+        override_parent_ctx: Optional["MergedMessage"] = None,
+        rewrite_cache: bool = False,
+        **kwargs,
+    ) -> List["MergedMessage"]:
+        """Get all the responses from the bot for a given request."""
+        responses = self.trigger(
+            request=request,
+            requests=requests,
+            override_sender=override_sender,
+            override_parent_ctx=override_parent_ctx,
+            rewrite_cache=rewrite_cache,
+            **kwargs,
+        )
+        return await responses.get_all_responses()
+
     def single_turn(self, handler: SingleTurnHandler) -> SingleTurnHandler:
         """
         A decorator that registers a local single-turn handler function for this MergedBot. Single-turn means that
         the function will be called as an event handler for a single incoming message (or a single set of messages
         if they were sent as a bundle).
         """
         self.merger.register_local_single_turn_handler(self, handler)
@@ -86,91 +108,82 @@
 
 class MergedUser(MergedParticipant):
     """A user that can interact with bots."""
 
     is_human: bool = Field(True, const=True)
 
 
-class MergedChannel(MergedObject):
-    """A logical channel where interactions between two or more participants happen."""
-
-    channel_type: str
-    channel_id: Any
-    owner: MergedParticipant
-
-    async def next_message_from_owner(
-        self,
-        content: MessageContent,
-        indicate_typing_afterwards: bool = False,
-        responds_to: Optional["MergedMessage"] = None,
-        **kwargs,
-    ) -> "MergedMessage":
-        """
-        Create a new message that goes after the last message in this channel. Mark it as if it was sent by the
-        owner of the channel.
-        """
-        return await self.next_message(
-            sender=self.owner,
-            content=content,
-            indicate_typing_afterwards=indicate_typing_afterwards,
-            responds_to=responds_to,
-            **kwargs,
-        )
-
-    async def next_message(
-        self,
-        sender: MergedParticipant,
-        content: MessageContent,
-        indicate_typing_afterwards: bool = False,
-        responds_to: Optional["MergedMessage"] = None,
-        **kwargs,
-    ) -> "MergedMessage":
-        """Create a new message that goes after the last message in this channel."""
-        return await self.merger.create_next_message(
-            thread_uuid=self.uuid,  # in this case, the thread is the channel itself
-            channel=self,
-            sender=sender,
-            content=content,
-            indicate_typing_afterwards=indicate_typing_afterwards,
-            responds_to=responds_to,
-            **kwargs,
-        )
-
-
-class BaseMessage:
-    """
-    Base class for messages. This is not a Pydantic model. `content` is property that must be implemented by
-    subclasses one way or another (either as a Pydantic field or as a property).
-    """
-
-    content: Union[str, Any]
-
-
 class MergedMessage(BaseMessage, MergedObject):
     """A message that was sent in a channel."""
 
-    channel: MergedChannel
-    thread_uuid: UUID4  # TODO should this be a dedicated MergedThread class ?
     sender: MergedParticipant
-    indicate_typing_afterwards: bool
+    receiver: MergedParticipant
+    still_thinking: bool
+    parent_context: Optional["MergedMessage"]
     responds_to: Optional["MergedMessage"]
     goes_after: Optional["MergedMessage"]
+    invisible_to_bots: bool = False
+
+    async def get_conversation_history(
+        self, max_length: Optional[int] = None, include_invisible_to_bots: bool = False
+    ) -> List["MergedMessage"]:
+        """Get the conversation history for this message (excluding this message)."""
+        # TODO does it need to by async ?
+        # TODO move this functionality to BotMerger ?
+        history = []
+        msg = self.goes_after
+        while msg and (max_length is None or len(history) < max_length):
+            if include_invisible_to_bots or not msg.invisible_to_bots:
+                history.append(msg)
+            msg = msg.goes_after
+        history.reverse()
+        return history
+
+    async def get_full_conversation(
+        self, max_length: Optional[int] = None, include_invisible_to_bots: bool = False
+    ) -> List["MergedMessage"]:
+        """Get the full conversation history for this message (including this message)."""
+        # TODO does it need to by async ?
+        if max_length is not None:
+            # let's account for the current message as well
+            max_length -= 1
+        result = await self.get_conversation_history(
+            max_length=max_length, include_invisible_to_bots=include_invisible_to_bots
+        )
+        if include_invisible_to_bots or not self.invisible_to_bots:
+            result.append(self)
+        return result
+
+    async def get_ultimate_original_message(self) -> "OriginalMessage":
+        """Get the ultimate original message for this message."""
+        # TODO does it need to by async ?
+        msg = self
+        while isinstance(msg, ForwardedMessage):
+            msg = msg.original_message
+        return msg
 
 
 class OriginalMessage(MergedMessage):
     """This subclass represents an original message. It implements `content` as a Pydantic field."""
 
     content: Union[str, Any]
 
+    @property
+    def original_message(self) -> "MergedMessage":
+        """The original message is itself."""
+        return self
+
 
 class ForwardedMessage(MergedMessage):
     """
     This subclass represents a forwarded message. It implements `content` as a property that is delegated to the
     original message.
     """
 
-    original_message: OriginalMessage
+    original_message: MergedMessage
+
+    # TODO does `invisible_to_bots` need to be inherited from the original message as well ?
 
     @property
     def content(self) -> MessageContent:
         """The content of the original message."""
         return self.original_message.content
```

### Comparing `botmerger-0.0.3/pyproject.toml` & `botmerger-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.black]
 line-length = 119
 
 [tool.poetry]
 name = "botmerger"
-version = "0.0.3"
+version = "0.0.4"
 description = ""
 authors = ["Oleksandr Tereshchenko <toporok@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.11"  # TODO extend this to older versions too
```

### Comparing `botmerger-0.0.3/PKG-INFO` & `botmerger-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botmerger
-Version: 0.0.3
+Version: 0.0.4
 Summary: 
 License: MIT
 Author: Oleksandr Tereshchenko
 Author-email: toporok@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -20,15 +20,15 @@
 BotMerger is a fully asynchronous Python framework designed as a messaging platform which allows Large Language Model
 (LLM)-based chatbots to interact with each other in order to "merge" into more complex bots capable of fulfilling
 non-trivial user requests.
 
 ## 📦 Installation
 
 ```shell
-pip install --upgrade botmerger
+pip install -U botmerger
 ```
 
 ## 🚀 Quickstart
 
 TODO
 
 ## 💡 Philosophy
```

