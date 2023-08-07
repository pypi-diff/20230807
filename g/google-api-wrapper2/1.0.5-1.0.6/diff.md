# Comparing `tmp/google-api-wrapper2-1.0.5.tar.gz` & `tmp/google-api-wrapper2-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-api-wrapper2-1.0.5.tar", max compression
+gzip compressed data, was "google-api-wrapper2-1.0.6.tar", max compression
```

## Comparing `google-api-wrapper2-1.0.5.tar` & `google-api-wrapper2-1.0.6.tar`

### file list

```diff
@@ -1,14 +1,16 @@
--rwxr-xr-x   0        0        0     1286 2021-04-29 20:24:53.463534 google-api-wrapper2-1.0.5/LICENSE
--rw-r--r--   0        0        0     1183 2021-11-26 12:11:02.645318 google-api-wrapper2-1.0.5/README.md
--rw-r--r--   0        0        0        0 2021-03-27 18:40:31.071000 google-api-wrapper2-1.0.5/googleapiwrapper/__init__.py
--rw-r--r--   0        0        0      501 2022-09-14 18:07:09.564705 google-api-wrapper2-1.0.5/googleapiwrapper/common.py
--rw-r--r--   0        0        0    17891 2022-12-28 15:44:09.632977 google-api-wrapper2-1.0.5/googleapiwrapper/gmail_api.py
--rw-r--r--   0        0        0    20691 2022-12-28 13:15:32.010562 google-api-wrapper2-1.0.5/googleapiwrapper/gmail_api_extensions.py
--rw-r--r--   0        0        0     7740 2021-05-08 23:58:24.517357 google-api-wrapper2-1.0.5/googleapiwrapper/gmail_domain.py
--rw-r--r--   0        0        0     5487 2021-12-24 09:23:45.404867 google-api-wrapper2-1.0.5/googleapiwrapper/google_auth.py
--rw-r--r--   0        0        0    30688 2022-10-06 09:40:26.807095 google-api-wrapper2-1.0.5/googleapiwrapper/google_drive.py
--rw-r--r--   0        0        0    20855 2022-09-14 18:07:09.564901 google-api-wrapper2-1.0.5/googleapiwrapper/google_sheet.py
--rw-r--r--   0        0        0      371 2021-05-06 21:52:22.013592 google-api-wrapper2-1.0.5/googleapiwrapper/utils.py
--rw-r--r--   0        0        0      906 2022-12-31 09:18:04.067058 google-api-wrapper2-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     1985 1970-01-01 00:00:00.000000 google-api-wrapper2-1.0.5/setup.py
--rw-r--r--   0        0        0     1853 1970-01-01 00:00:00.000000 google-api-wrapper2-1.0.5/PKG-INFO
+-rwxr-xr-x   0        0        0     1286 2021-04-29 20:24:53.463534 google-api-wrapper2-1.0.6/LICENSE
+-rw-r--r--   0        0        0     1183 2021-11-26 12:11:02.645318 google-api-wrapper2-1.0.6/README.md
+-rw-r--r--   0        0        0        0 2021-03-27 18:40:31.071000 google-api-wrapper2-1.0.6/googleapiwrapper/__init__.py
+-rw-r--r--   0        0        0      501 2022-09-14 18:07:09.564705 google-api-wrapper2-1.0.6/googleapiwrapper/common.py
+-rw-r--r--   0        0        0    22813 2023-06-27 23:22:37.341693 google-api-wrapper2-1.0.6/googleapiwrapper/gmail_api.py
+-rw-r--r--   0        0        0     1803 2023-06-27 23:22:37.346361 google-api-wrapper2-1.0.6/googleapiwrapper/gmail_api_extensions.py
+-rw-r--r--   0        0        0    24092 2023-06-27 23:38:51.941562 google-api-wrapper2-1.0.6/googleapiwrapper/gmail_cache.py
+-rw-r--r--   0        0        0      386 2023-06-27 22:36:32.130117 google-api-wrapper2-1.0.6/googleapiwrapper/gmail_common.py
+-rw-r--r--   0        0        0     9615 2023-06-27 04:26:10.899176 google-api-wrapper2-1.0.6/googleapiwrapper/gmail_domain.py
+-rw-r--r--   0        0        0     5487 2021-12-24 09:23:45.404867 google-api-wrapper2-1.0.6/googleapiwrapper/google_auth.py
+-rw-r--r--   0        0        0    31851 2023-06-27 17:25:28.530932 google-api-wrapper2-1.0.6/googleapiwrapper/google_drive.py
+-rw-r--r--   0        0        0    20855 2022-09-14 18:07:09.564901 google-api-wrapper2-1.0.6/googleapiwrapper/google_sheet.py
+-rw-r--r--   0        0        0     1002 2023-06-26 02:30:20.167883 google-api-wrapper2-1.0.6/googleapiwrapper/utils.py
+-rw-r--r--   0        0        0      906 2023-08-07 00:42:50.007761 google-api-wrapper2-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1985 1970-01-01 00:00:00.000000 google-api-wrapper2-1.0.6/setup.py
+-rw-r--r--   0        0        0     1853 1970-01-01 00:00:00.000000 google-api-wrapper2-1.0.6/PKG-INFO
```

### Comparing `google-api-wrapper2-1.0.5/LICENSE` & `google-api-wrapper2-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `google-api-wrapper2-1.0.5/README.md` & `google-api-wrapper2-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `google-api-wrapper2-1.0.5/googleapiwrapper/gmail_api.py` & `google-api-wrapper2-1.0.6/googleapiwrapper/gmail_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import logging
 import sys
 import datetime
+from collections import defaultdict
 from dataclasses import dataclass
 from typing import List, Dict, Any
 
 from googleapiclient.discovery import build
 from pythoncommons.date_utils import timeit
 
-from googleapiwrapper.gmail_api_extensions import CachingStrategyType, ApiFetchingContext, CacheResultItems
+from googleapiwrapper.gmail_api_extensions import ApiFetchingContext
+from googleapiwrapper.gmail_cache import CacheResultItems, CachingStrategyType
+from googleapiwrapper.gmail_common import GmailRequestType
 from googleapiwrapper.gmail_domain import (
-    ApiItemType,
     Message,
     MessagePartDescriptor,
     MessagePart,
     GmailMessageBodyPart,
     ThreadsResponseField,
     MessagePartField,
     MessagePartBodyField,
@@ -33,63 +35,92 @@
 from googleapiwrapper.google_auth import GoogleApiAuthorizer, AuthedSession
 from pythoncommons.string_utils import auto_str
 
 CONV_CONTEXT_PREFIX = "[API Conversion context] "
 LOG = logging.getLogger(__name__)
 
 
+class GmailRequestLoggerAdapter(logging.LoggerAdapter):
+    def process(self, msg, kwargs):
+        return f"[GMAIL REQUEST] {msg}", kwargs
+
+
+REQ_LOG = GmailRequestLoggerAdapter(LOG, {})
+
+
 class Progress:
-    def __init__(self, item_type: ApiItemType, limit: int = None):
-        self.requests_count = 0
-        self.all_items_count = 0
-        self.processed_items = 0
-        self.new_items_with_last_request = -1
-        self.item_type = item_type
+    def __init__(self, limit: int = None):
+        self.req_counts: Dict[GmailRequestType, int] = defaultdict(int)
+        self.all_items_count: Dict[GmailRequestType, int] = defaultdict(int)
+        self.processed_items: Dict[GmailRequestType, int] = defaultdict(int)
+        self.new_items_with_last_request: Dict[GmailRequestType, int] = defaultdict(int)
+        self.current_item_id: Dict[GmailRequestType, str] = defaultdict(str)
         self.limit = limit
 
-    def _print_status(self):
+    def print_stats(self):
+        LOG.info("=" * 50 + "    STATISTICS    " + "=" * 50)
+        LOG.info("# of requests, by type: %s", self.req_counts)
+        LOG.info("All items count, by type: %s", self.all_items_count)
+        LOG.info("Processed items, by type: %s", self.processed_items)
+        LOG.info("=" * 50 + "    END OF STATISTICS    " + "=" * 50)
+
+    def _print_status(self, req_type: GmailRequestType):
         LOG.info(
-            f"[Request #: {self.requests_count}] "
-            f"Received {self.new_items_with_last_request} more {self.item_type.value}s"
+            f"[# of requests: {self.req_counts[req_type]}] "
+            f"Received {self.new_items_with_last_request[req_type]} more {req_type.value}"
         )
 
-    def incr_requests(self):
-        self.requests_count += 1
+    def incr_requests(self, req_type: GmailRequestType):
+        self.req_counts[req_type] += 1
 
-    def register_new_items(self, number_of_new_items: int, print_status=True):
-        self.all_items_count += number_of_new_items
-        self.new_items_with_last_request = number_of_new_items
+    def register_new_items(self, req_type: GmailRequestType, number_of_new_items: int, print_status=True):
+        self.all_items_count[req_type] += number_of_new_items
+        self.new_items_with_last_request[req_type] = number_of_new_items
         if print_status:
-            self._print_status()
+            self._print_status(req_type)
 
-    def incr_processed_items(self, item_id: str):
-        self.current_item_id = item_id
-        self.processed_items += 1
+    def incr_processed_items(self, req_type: GmailRequestType, item_id: str):
+        self.current_item_id[req_type] = item_id
+        self.processed_items[req_type] += 1
 
-    def is_limit_reached(self):
+    def is_limit_reached(self, req_type: GmailRequestType):
         if self.limit:
-            return self.processed_items > self.limit
+            return self.processed_items[req_type] > self.limit
         return False
 
-    def print_processing_items(self, print_item_id=True):
-        msg = f"Processing {self.item_type.value}s: {self.processed_items} / {self.all_items_count}."
+    def print_processing_items(self, req_type: GmailRequestType, print_item_id=True):
+        msg = f"Processing {req_type.value}: {self.processed_items[req_type]} / {self.all_items_count[req_type]}."
         if print_item_id:
-            msg += f" [Item ID: {self.current_item_id}]"
+            msg += f" [Item ID: {self.current_item_id[req_type]}]"
         LOG.debug(msg)
 
 
 # TODO Move this object as a dependency of ApiFetchingContext
 @auto_str
 class ApiConversionContext:
-    def __init__(self, item_type: ApiItemType, limit: int = None):
-        self.progress = Progress(item_type, limit=limit)
+    def __init__(
+        self,
+        limit: int = None,
+        show_empty_body_errors=True,
+        query: str = None,
+        format: ThreadQueryFormat = None,
+        sanity_check: bool = False,
+        expect_one_message_per_thread: bool = False,
+    ):
+        self.query = query
+        self.sanity_check = sanity_check
+        self.format = format
+        self.expect_one_message_per_thread = expect_one_message_per_thread
+        self.progress = Progress(limit=limit)
+        self.show_empty_body_errors = show_empty_body_errors
         self.decode_errors: List[MessagePartDescriptor] = []
         self.empty_bodies: List[MessagePartDescriptor] = []
 
         # Set later
+        self.threads: GmailThreads or None = None
         self.current_message: Message or None = None
         self.current_message_part: MessagePart or None = None
 
     def register_current_message(self, message: Message):
         self.current_message: Message = message
 
     def register_current_message_part(self, message_part: MessagePart):
@@ -104,15 +135,17 @@
             MessagePartDescriptor(self.current_message, self.current_message_part, gmail_msg_body_part)
         )
 
     def report_empty_body(self, thread_id: str, gmail_msg_body_part: GmailMessageBodyPart):
         details = self._get_current_message_details(
             gmail_msg_body_part, short_message_part=True, short_gmail_message_body_part=True, log_message=False
         )
-        self._log_error(f"Empty message for thread with ID '{thread_id}'.\n" f"Details:\n{details}")
+        if self.show_empty_body_errors:
+            self._log_error(f"Empty message for thread with ID '{thread_id}'.\n" f"Details:\n{details}")
+
         self.empty_bodies.append(
             MessagePartDescriptor(self.current_message, self.current_message_part, gmail_msg_body_part)
         )
 
     @staticmethod
     def _log_error(msg: str):
         LOG.error(CONV_CONTEXT_PREFIX + " " + msg)
@@ -141,14 +174,27 @@
 
     def handle_empty_bodies(self, func):
         # TODO error log all
         for descriptor in self.empty_bodies:
             func(descriptor)
         self.empty_bodies.clear()
 
+    def perform_sanity_check(self, thread_id: str):
+        for desc in self.empty_bodies:
+            d_message_id: str = desc.message.id
+            d_thread_id: str = desc.message.thread_id
+            LOG.debug("Found message id in descriptor: %s", d_message_id)
+            LOG.debug("Found thread id in descriptor: %s", d_thread_id)
+            if thread_id != d_thread_id:
+                thread_ids = set([d.message.thread_id for d in self.empty_bodies])
+                raise ValueError(
+                    "Mismatch in thread ids. "
+                    "Current thread id: {}, found thread_ids: {}".format(thread_id, thread_ids)
+                )
+
 
 CONVERSION_CONTEXT: ApiConversionContext = None
 module = sys.modules[__name__]
 
 
 @dataclass
 class ThreadQueryResults:
@@ -196,88 +242,97 @@
         self.users_svc = self.service.users()
         self.messages_svc = self.users_svc.messages()
         self.threads_svc = self.users_svc.threads()
         self.attachments_svc = self.messages_svc.attachments()
 
     @timeit
     def query_threads(
-        self, query: str = None, limit: int = None, sanity_check=True, expect_one_message_per_thread=False
+        self,
+        query: str = None,
+        limit: int = None,
+        sanity_check=True,
+        expect_one_message_per_thread=False,
+        show_empty_body_errors=True,
+        format: ThreadQueryFormat = ThreadQueryFormat.FULL,
+        offline: bool = False,
     ) -> ThreadQueryResults:
         query_conf: str = (
             f"Query: {query}, Limit: {limit}, Expect one message per thread: {expect_one_message_per_thread}"
         )
         LOG.info(f"Querying gmail threads. Config: {query_conf}")
-        module.CONVERSION_CONTEXT = ApiConversionContext(ApiItemType.THREAD, limit=limit)
+        module.CONVERSION_CONTEXT = ApiConversionContext(
+            query=query,
+            limit=limit,
+            format=format,
+            show_empty_body_errors=show_empty_body_errors,
+            sanity_check=sanity_check,
+            expect_one_message_per_thread=expect_one_message_per_thread,
+        )
         ctx = CONVERSION_CONTEXT
         kwargs = self._get_new_kwargs()
         if query:
             kwargs[ListQueryParam.QUERY.value] = query
         if limit and limit < GmailWrapper.DEFAULT_PAGE_SIZE:
             kwargs[ListQueryParam.MAX_RESULTS.value] = limit
 
-        request = self.threads_svc.list(**kwargs)
-        threads = GmailThreads()
-        while request is not None:
-            response: Dict[str, Any] = request.execute()
-            if response:
-                ctx.progress.incr_requests()
-                list_of_threads: List[Dict[str, str]] = response.get(ThreadsResponseField.THREADS.value, [])
-                ctx.progress.register_new_items(len(list_of_threads), print_status=True)
-                thread_ids: List[str] = [GH.get_field(t, ThreadField.ID) for t in list_of_threads]
-                cache_state: CacheResultItems = self.api_fetching_ctx.get_cache_state_for_threads(
-                    thread_ids, expect_one_message_per_thread
-                )
-                self._log_cache_state_details(cache_state, thread_ids)
-                for idx, thread_id in enumerate(thread_ids):
-                    # TODO consider limiting only real sent requests, not processed items!
-                    ctx.progress.incr_processed_items(thread_id)
-                    if ctx.progress.is_limit_reached():
-                        LOG.warning(f"Reached request limit of {limit}, stop processing more items.")
-                        return ThreadQueryResults(threads)
-                    ctx.progress.print_processing_items()
-                    thread_resp_full = self._request_thread_or_load_from_cache(thread_id, cache_state)
-                    self.api_fetching_ctx.process_thread(thread_resp_full)
-                    thread_obj: Thread = self._convert_to_thread_object(ctx, sanity_check, thread_id, thread_resp_full)
-                    threads.add(thread_obj)  # This action will internally create GmailMessage and rest of the stuff
-            request = self.threads_svc.list_next(request, response)
-
+        if not offline:
+            self._fetch_threads(ctx, kwargs, self._threads_response_handler)
+        else:
+            rt = GmailRequestType.THREADS_LIST
+            ctx.threads = GmailThreads()
+            thread_ids = self.api_fetching_ctx.get_cached_threads()
+            ctx.progress.register_new_items(rt, len(thread_ids), print_status=True)
+            self._process_threads(ctx, rt, thread_ids)
         ctx.handle_encoding_errors()
         LOG.info(f"Finished querying gmail threads. Config: {query_conf}")
-        return ThreadQueryResults(threads)
+        ctx.progress.print_stats()
+        return ThreadQueryResults(ctx.threads)
 
     @staticmethod
     def _log_cache_state_details(cache_state: CacheResultItems, item_ids: List[str]):
         ct_plural: str = cache_state.cache_type_plural
         no_of_items: int = len(item_ids)
         LOG.info(
             f"Found cached {ct_plural} {cache_state.get_no_of_any_cached_for_items()} / {no_of_items}. "
             f"Breakdown of cache state: \n{cache_state.get_status_dict()}"
         )
         LOG.trace(f"API fetching context returned cache state for {len(item_ids)} {ct_plural}: {cache_state}")
 
-    def _query_thread_data_minimal(self, thread_id) -> List[str]:
+    def _fetch_thread_data_minimal(self, thread_id, ctx: ApiConversionContext) -> List[str]:
         # Try to query in minimal format first, hoping that some messages are already in cache
-        thread_resp_minimal: Dict[str, Any] = self._query_thread_data(thread_id, full=False)
+        thread_resp_minimal: Dict[str, Any] = self._fetch_thread_data(thread_id, ctx, format=ThreadQueryFormat.MINIMAL)
         messages_response: List[Dict[str, Any]] = GH.get_field(thread_resp_minimal, ThreadField.MESSAGES)
         message_ids: List[str] = [GH.get_field(msg, MessageField.ID) for msg in messages_response]
         return message_ids
 
-    def _request_thread_or_load_from_cache(self, thread_id: str, cache_state: CacheResultItems):
+    def _request_thread_or_load_from_cache(
+        self, thread_id: str, cache_state: CacheResultItems, ctx: ApiConversionContext
+    ):
+        loaded_from_cache = False
+        accepted_thread_query_formats = (ThreadQueryFormat.FULL, ThreadQueryFormat.RAW)
+        if ctx.format not in accepted_thread_query_formats:
+            raise ValueError(
+                "Expecting Gmail query format to be in: {}. Actual value: {}".format(
+                    accepted_thread_query_formats, ctx.format
+                )
+            )
+
         if not cache_state.is_fully_cached(thread_id):
-            message_ids: List[str] = self._query_thread_data_minimal(thread_id)
+            message_ids: List[str] = self._fetch_thread_data_minimal(thread_id, ctx)
             self.api_fetching_ctx.process_messages(cache_state, thread_id, message_ids)
 
         # Check if thread is now considered as fully cached, given the provided message IDs above
         if cache_state.is_fully_cached(thread_id):
             thread_resp_full = self._get_item_from_cache(cache_state, thread_id)
+            loaded_from_cache = True
         else:
             # Not all messages for this thread are in cache.
-            # In this case, we need to retrieve the thread again, now with full format
-            thread_resp_full: Dict[str, Any] = self._query_thread_data(thread_id, full=True)
-        return thread_resp_full
+            # In this case, we need to retrieve the thread again, now with specified format
+            thread_resp_full: Dict[str, Any] = self._fetch_thread_data(thread_id, ctx, format=ctx.format)
+        return thread_resp_full, loaded_from_cache
 
     @staticmethod
     def _get_item_from_cache(cache_state: CacheResultItems, item_id):
         ct = cache_state.cache_type
         ctc = cache_state.cache_type_capitalized
         thread_id_str = f"{ctc} ID: {item_id}"
         LOG.debug(
@@ -287,44 +342,52 @@
         if not thread_resp_full:
             raise ValueError(f"{ctc} data is None for {ct} ID '{item_id}'. Please check logs.")
         return thread_resp_full
 
     def _convert_to_thread_object(self, ctx, sanity_check: bool, thread_id: str, thread_resp_full):
         messages_response: List[Dict[str, Any]] = GH.get_field(thread_resp_full, ThreadField.MESSAGES)
         messages: List[Message] = [self.parse_api_message(message) for message in messages_response]
-        ctx.handle_empty_bodies(lambda desc: self._request_attachment_or_load_from_cache(desc))
+
+        if sanity_check:
+            ctx.perform_sanity_check(thread_id)
+
         arbitrary_msg_subject: str = messages[0].subject
         thread_obj: Thread = Thread(thread_id, arbitrary_msg_subject, messages)
         if sanity_check:
             self._sanity_check(thread_obj)
         return thread_obj
 
-    def _request_attachment_or_load_from_cache(self, descriptor: MessagePartDescriptor):
+    def request_attachment_or_load_from_cache(self, descriptor: MessagePartDescriptor, ctx: ApiConversionContext):
         # Fix MessagePartBody object that has attachmentId only
         # Quoting from API doc for Field 'attachmentId':
         # When present, contains the ID of an external attachment that can be retrieved in a
         # separate messages.attachments.get request.
         # When not present, the entire content of the message part body is contained in the data field.
         message_id: str = descriptor.message.id
         thread_id: str = descriptor.message.thread_id
         attachment_id = descriptor.message_part.body.attachment_id
         if not message_id or not attachment_id:
-            LOG.error(
-                "Both message_id and attachment_id has to be set in order to load message attachment from cache "
-                f"or to query attachment details from API.\nObject was: {descriptor}"
-            )
+            if ctx.show_empty_body_errors:
+                LOG.error(
+                    "Both message_id and attachment_id has to be set in order to load message attachment from cache "
+                    f"or to query attachment details from API.\nObject was: {descriptor}"
+                )
             return
 
-        cache_state: CacheResultItems = self.api_fetching_ctx.get_cache_state_for_message(thread_id, message_id)
+        cache_state: CacheResultItems = self.api_fetching_ctx.get_cache_state_for_message(
+            thread_id, message_id, attachment_id
+        )
         self._log_cache_state_details(cache_state, [message_id])
         if cache_state.is_fully_cached(message_id):
             attachment_response = self._get_item_from_cache(cache_state, thread_id)
         else:
-            attachment_response: Dict[str, Any] = self._query_attachment(thread_id, message_id, attachment_id)
-        self.api_fetching_ctx.process_attachment_for_message(thread_id, message_id, attachment_response)
+            attachment_response: Dict[str, Any] = self._fetch_attachment(ctx, thread_id, message_id, attachment_id)
+            self.api_fetching_ctx.process_attachment_for_message(
+                thread_id, message_id, attachment_id, attachment_response
+            )
 
         # Fix the GmailMessageBodyPart object's body_data property with the contents of the attachment.
         # TODO consider storing FS instead of whole file contents in memory?
         descriptor.gmail_msg_body_part.body_data = attachment_response
 
     def parse_api_message(self, message: Dict):
         message_part = GH.get_field(message, MessageField.PAYLOAD)
@@ -350,14 +413,18 @@
         )
         return message_part_obj
 
     @staticmethod
     def _parse_headers(message_part):
         headers_list: List[Dict[str, str]] = GH.get_field(message_part, MessagePartField.HEADERS)
         headers: List[Header] = []
+        if not headers_list:
+            LOG.warning("Headers is empty for message part: %s", message_part)
+            return headers
+
         for header_dict in headers_list:
             headers.append(
                 Header(GH.get_field(header_dict, HeaderField.NAME), GH.get_field(header_dict, HeaderField.VALUE))
             )
         return headers
 
     @staticmethod
@@ -365,33 +432,83 @@
         message_part_body_obj = MessagePartBody(
             GH.get_field(messagepart_body, MessagePartBodyField.DATA),
             GH.get_field(messagepart_body, MessagePartBodyField.SIZE),
             GH.get_field(messagepart_body, MessagePartBodyField.ATTACHMENT_ID),
         )
         return message_part_body_obj
 
-    def _query_thread_data(self, thread_id: str, full=True):
-        fmt: ThreadQueryFormat = ThreadQueryFormat.FULL if full else ThreadQueryFormat.MINIMAL
+    def _fetch_thread_data(
+        self, thread_id: str, ctx: ApiConversionContext, format: ThreadQueryFormat = ThreadQueryFormat.MINIMAL
+    ):
         kwargs = self._get_new_kwargs()
         kwargs[ThreadField.ID.value] = thread_id
-        kwargs[ThreadQueryParam.FORMAT.value] = fmt.value
+        kwargs[ThreadQueryParam.FORMAT.value] = format.value
         # TODO print email subject
-        LOG.info(f"Requesting gmail thread with ID '{thread_id}', format: {fmt.value}")
+        REQ_LOG.info(f"Requesting gmail thread with ID '{thread_id}', format: {format.value}")
         tdata = self.threads_svc.get(**kwargs).execute()
+        ctx.progress.incr_requests(GmailRequestType.THREADS_GET)
         return tdata
 
-    def _query_attachment(self, thread_id: str, message_id: str, attachment_id: str) -> Dict[str, Any]:
+    def _fetch_attachment(
+        self, ctx: ApiConversionContext, thread_id: str, message_id: str, attachment_id: str
+    ) -> Dict[str, Any]:
         kwargs = self._get_new_kwargs()
         kwargs[GetAttachmentParam.MESSAGE_ID.value] = message_id
         kwargs[GetAttachmentParam.ATTACHMENT_ID.value] = attachment_id
-        LOG.info(f"Requesting gmail attachment for message with ID '{message_id}', Thread ID '{thread_id}'")
-        return self.attachments_svc.get(**kwargs).execute()
+        REQ_LOG.info(
+            f"Requesting gmail attachment for message with ID '{message_id}', Thread ID '{thread_id}', Attachment ID '{attachment_id}'"
+        )
+        response = self.attachments_svc.get(**kwargs).execute()
+        ctx.progress.incr_requests(GmailRequestType.ATTACHMENTS)
+        return response
 
     @staticmethod
     def _get_new_kwargs():
         kwargs = {}
         kwargs.update(GmailWrapper.DEFAULT_API_FIELDS)
         return kwargs
 
     def _sanity_check(self, thread: Thread):
         # TODO implement checking if all messages have the same subject
         pass
+
+    def _fetch_threads(self, ctx: ApiConversionContext, kwargs, response_handler_func):
+        request = self.threads_svc.list(**kwargs)
+        ctx.threads = GmailThreads()
+        while request is not None:
+            REQ_LOG.info("Requesting gmail threads")
+            response: Dict[str, Any] = request.execute()
+            ctx.progress.incr_requests(GmailRequestType.THREADS_LIST)
+            response_handler_func(ctx, response)
+            request = self.threads_svc.list_next(request, response)
+
+    def _threads_response_handler(self, ctx: ApiConversionContext, response):
+        progress = ctx.progress
+        if response:
+            rt = GmailRequestType.THREADS_LIST
+            list_of_threads: List[Dict[str, str]] = response.get(ThreadsResponseField.THREADS.value, [])
+            progress.register_new_items(rt, len(list_of_threads), print_status=True)
+            thread_ids: List[str] = [GH.get_field(t, ThreadField.ID) for t in list_of_threads]
+            self._process_threads(ctx, rt, thread_ids)
+
+    def _process_threads(self, ctx: ApiConversionContext, rt: GmailRequestType, thread_ids: List[str]):
+        progress = ctx.progress
+
+        cache_state: CacheResultItems = self.api_fetching_ctx.get_cache_state_for_threads(
+            thread_ids, ctx.expect_one_message_per_thread
+        )
+        self._log_cache_state_details(cache_state, thread_ids)
+        for idx, thread_id in enumerate(thread_ids):
+            # TODO consider limiting only real sent requests, not processed items!
+            progress.incr_processed_items(rt, thread_id)
+            if progress.is_limit_reached(rt):
+                LOG.warning(f"Reached request limit of {ctx.limit}, stop processing more items.")
+                return ThreadQueryResults(ctx.threads)
+            progress.print_processing_items(rt)
+            thread_resp_full, loaded_from_cache = self._request_thread_or_load_from_cache(thread_id, cache_state, ctx)
+            if not loaded_from_cache:
+                self.api_fetching_ctx.process_thread(thread_resp_full)
+            thread_obj: Thread = self._convert_to_thread_object(ctx, ctx.sanity_check, thread_id, thread_resp_full)
+            ctx.threads.add(thread_obj)  # This action will internally create GmailMessage and rest of the stuff
+            ctx.handle_empty_bodies(lambda desc: self.request_attachment_or_load_from_cache(desc, ctx))
+
+        self.api_fetching_ctx.print_cache_actions()
```

### Comparing `google-api-wrapper2-1.0.5/googleapiwrapper/gmail_api_extensions.py` & `google-api-wrapper2-1.0.6/googleapiwrapper/gmail_cache.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,30 @@
-import logging
 from abc import ABC, abstractmethod
+from collections import defaultdict
 from dataclasses import dataclass, field
 from enum import Enum
-from typing import List, Dict, Any, Set, Iterable
+from typing import Any, Dict, List, Iterable, Set, Tuple
 
-from pythoncommons.file_utils import JsonFileUtils, FileUtils, FindResultType
-from pythoncommons.string_utils import auto_str
+from pythoncommons.file_utils import FileUtils, FindResultType, JsonFileUtils
+from pythoncommons.string_utils import auto_str, StringUtils
 
+from googleapiwrapper.gmail_common import GmailRequestType
+from googleapiwrapper.gmail_common import (
+    THREADS_DIR_NAME,
+    MESSAGE_DATA_FILENAME,
+    MESSAGE_ID,
+    MESSAGE_DATE,
+    THREAD_JSON_FILENAME,
+    MESSAGES_DIR_NAME,
+)
 from googleapiwrapper.gmail_domain import GenericObjectHelper as GH, ThreadField, MessageField
 from googleapiwrapper.utils import CommonUtils
 
-MESSAGE_DATE = "message_date"
-MESSAGE_ID = "message_id"
-THREAD_JSON_FILENAME = "thread.json"
-MESSAGE_DATA_FILENAME = "message_data"
-THREADS_DIR_NAME = "threads"
-MESSAGES_DIR_NAME = "messages"
+import logging
+
 LOG = logging.getLogger(__name__)
 
 
 class ItemCacheState(Enum):
     NOT_CACHED = "not cached"
     CACHE_LEVEL_NOT_DETERMINED = "cache level not yet determined"
     FULLY_CACHED = "fully cached"
@@ -38,14 +43,85 @@
     type: str
     type_plural: str
 
     def __post_init__(self):
         self.type_capitalized = self.type.title()
 
 
+@dataclass
+class CacheMetrics:
+    items_written: int
+    bytes_written: int
+    items_read: int
+    bytes_read: int
+
+    def _combine(self, other):
+        items_written = self.items_written + other.items_written
+        bytes_written = self.bytes_written + other.bytes_written
+        items_read = self.items_read + other.items_read
+        bytes_read = self.bytes_read + other.bytes_read
+        return CacheMetrics(items_written, bytes_written, items_read, bytes_read)
+
+    @staticmethod
+    def create_for_read(items_read, bytes_read):
+        return CacheMetrics(0, 0, items_read, bytes_read)
+
+    @staticmethod
+    def create_for_write(items_written, bytes_written):
+        return CacheMetrics(items_written, bytes_written, 0, 0)
+
+    @staticmethod
+    def create_empty():
+        return CacheMetrics(0, 0, 0, 0)
+
+    @staticmethod
+    def combine(*actions):
+        if not actions:
+            raise ValueError("Expected at least one instance of " + CacheMetrics.__class__.__name__)
+        result = actions[0]
+        for i in range(1, len(actions)):
+            result = result._combine(actions[i])
+        return result
+
+    def __str__(self):
+        return (
+            self.__class__.__name__
+            + " { "
+            + "items written: "
+            + str(self.items_written)
+            + ", bytes written (dynamic): "
+            + StringUtils.format_bytes_as_str(self.bytes_written)
+            + ", items read: "
+            + str(self.items_read)
+            + ", bytes read (dynamic): "
+            + StringUtils.format_bytes_as_str(self.bytes_read)
+            + " }"
+        )
+
+
+class CacheActionsPerformed:
+    def __init__(self):
+        self._latest: Dict["GmailRequestType", CacheMetrics] = defaultdict(CacheMetrics.create_empty)
+        self._sum: Dict["GmailRequestType", CacheMetrics] = defaultdict(CacheMetrics.create_empty)
+
+    def add(self, request_type: "GmailRequestType", metrics: CacheMetrics):
+        self._latest[request_type] = metrics
+        self._sum[request_type] = self._sum[request_type].combine(metrics)
+        self.log(request_type)
+
+    def log(self, request_type):
+        LOG.trace("Added metrics for %s: %s", request_type, self._latest[request_type])
+        for req_type, metrics in self._sum.items():
+            LOG.trace("Sum metrics for %s: %s", req_type, metrics)
+
+    def print_all(self):
+        for req_type, metrics in self._sum.items():
+            LOG.info("Sum metrics for %s: %s", req_type, metrics)
+
+
 @auto_str
 class CacheResultItems:
     def __init__(self, item_ids: List[str], cache_type: str, cache_type_plural: str = None):
         if not cache_type_plural:
             cache_type_plural = f"{cache_type}s"
         self._meta = CacheMeta(cache_type, cache_type_plural)
         self.item_ids = item_ids
@@ -218,104 +294,131 @@
         pass
 
     @abstractmethod
     def actualize_cache_state(self, cache_state: CacheResultItems, thread_id: str, message_ids: List[str]):
         pass
 
     @abstractmethod
-    def process_attachment_for_message(self, thread_id: str, message_id: str, attachment_response: Dict[str, Any]):
+    def process_attachment_for_message(
+        self, thread_id: str, message_id: str, attachment_id: str, attachment_response: Dict[str, Any]
+    ):
+        pass
+
+    @abstractmethod
+    def get_cache_state_for_message(self, thread_id: str, message_id: str, attachment_id: str):
+        pass
+
+    @abstractmethod
+    def get_cached_threads(self):
         pass
 
     @abstractmethod
-    def get_cache_state_for_message(self, thread_id: str, message_id: str):
+    def print_actions_performed(self):
         pass
 
 
 class FileSystemEmailThreadCacheStrategy(CachingStrategy):
     def __init__(self, output_basedir: str, project_name: str, user_email: str):
         # Cache-related properties
         self.cached_thread_ids: List[str] = []
         # Key: Message ID
-        self.cached_message_attachments: Set[str] = set()
+        self.cached_message_attachments: Set[Tuple[str, str, str]] = set()  # Tuple: (threadID, messageID, attachmentID)
         # Main key: Thread id
         # Inner-dict key: message id, value: message date
         self.thread_to_message_data: Dict[str, Dict[str, str]] = {}
         self.unknown_message_per_thread: Dict[str, Set[str]] = {}
 
         # Other properties
         user_email_converted = CommonUtils.convert_email_address_to_dirname(user_email)
         self.project_acct_basedir = FileUtils.join_path(output_basedir, user_email_converted)
         self.threads_dir = FileUtils.ensure_dir_created(
             FileUtils.join_path(self.project_acct_basedir, THREADS_DIR_NAME)
         )
+        self._cache_actions_performed = CacheActionsPerformed()
         super().__init__(output_basedir, project_name, user_email)
 
+    def get_cached_threads(self):
+        return self.thread_to_message_data.keys()
+
     def fill_cache(self):
         found_thread_dirnames: List[str] = FileUtils.find_files(
             self.threads_dir, find_type=FindResultType.DIRS, regex=".*", single_level=True
         )
         self.cached_thread_ids.extend(found_thread_dirnames)
         for thread_id in self.cached_thread_ids:
-            self._load_message_data_from_file(thread_id)
+            metrics = self._load_message_data_from_file(thread_id)
+            self._cache_actions_performed.add(GmailRequestType.MESSAGES, metrics)
+
         LOG.trace(f"Loaded message data: {self.thread_to_message_data}")
 
-    def _load_message_data_from_file(self, thread_id):
+    def _load_message_data_from_file(self, thread_id) -> CacheMetrics:
         """
         Load all message IDs for all threads but loading all payloads into memory would be costly
         so they are skipped here
         Example message data: [{'message_date': '1620084692000', 'message_id': '1793492a16dc62b5'}]
         """
         message_data_file = FileUtils.join_path(self.threads_dir, thread_id, MESSAGE_DATA_FILENAME)
-        list_of_message_data: List[Dict[str, str]] = self._load_data_from_file(message_data_file)
+        list_of_message_data, metrics = self._load_data_from_file(message_data_file)
         self.thread_to_message_data[thread_id] = {
             msg_data[MESSAGE_ID]: msg_data[MESSAGE_DATE] for msg_data in list_of_message_data
         }
+        return metrics
 
     def process_threads(self, thread_response: Dict[str, Any]):
         # TODO only write to file if required, i.e. thread is not fully cached. Also, make this configurable
         thread_id: str = GH.get_field(thread_response, ThreadField.ID)
-        thread_dir: str = self._write_thread_data_to_file(thread_id, thread_response)
-        self._write_message_data_to_file(thread_dir, thread_response)
-
-    def process_attachment_for_message(self, thread_id: str, message_id: str, attachment_response: Dict[str, Any]):
-        msg_attachment_filename = self._get_attachment_filename(thread_id, message_id, create_messages_dir=True)
-        self._write_to_file(msg_attachment_filename, attachment_response)
+        thread_dir, metrics_1 = self._write_thread_data_to_file(thread_id, thread_response)
+        metrics_2 = self._write_message_data_to_file(thread_dir, thread_response)
+        metrics = CacheMetrics.combine(metrics_1, metrics_2)
+        self._cache_actions_performed.add(GmailRequestType.THREADS_GET, metrics)
+
+    def process_attachment_for_message(
+        self, thread_id: str, message_id: str, attachment_id: str, attachment_response: Dict[str, Any]
+    ):
+        msg_attachment_filename = self._get_attachment_filename(
+            thread_id, message_id, attachment_id, create_messages_dir=True
+        )
+        metrics = self._write_to_file(msg_attachment_filename, attachment_response)
+        self._cache_actions_performed.add(GmailRequestType.ATTACHMENTS, metrics)
 
-    def _write_thread_data_to_file(self, thread_id: str, thread_response):
+    def _write_thread_data_to_file(self, thread_id: str, thread_response) -> Tuple[str, CacheMetrics]:
         current_thread_dir = FileUtils.ensure_dir_created(FileUtils.join_path(self.threads_dir, thread_id))
         raw_thread_json_file = FileUtils.join_path(current_thread_dir, THREAD_JSON_FILENAME)
-        self._write_to_file(raw_thread_json_file, thread_response)
-        return current_thread_dir
+        metrics = self._write_to_file(raw_thread_json_file, thread_response)
+        return current_thread_dir, metrics
 
-    def _write_message_data_to_file(self, thread_dir: str, thread_response):
+    def _write_message_data_to_file(self, thread_dir: str, thread_response) -> CacheMetrics:
         message_data_dicts: List[Dict[str, str]] = self._convert_thread_response_to_message_data_dicts(thread_response)
         message_data_file = FileUtils.join_path(thread_dir, MESSAGE_DATA_FILENAME)
-        self._write_to_file(message_data_file, message_data_dicts)
+        return self._write_to_file(message_data_file, message_data_dicts)
 
     @staticmethod
-    def _load_data_from_file(file):
-        return JsonFileUtils.load_data_from_json_file(file)
+    def _load_data_from_file(file) -> Tuple[List[Dict[str, str]], CacheMetrics]:
+        data, bytes_read = JsonFileUtils.load_data_from_json_file(file)
+        return data, CacheMetrics.create_for_read(1, bytes_read)
 
     @staticmethod
-    def _write_to_file(file, data):
-        JsonFileUtils.write_data_to_file_as_json(file, data, pretty=True)
+    def _write_to_file(file, data) -> CacheMetrics:
+        bytes_written = JsonFileUtils.write_data_to_file_as_json(file, data, pretty=True)
+        return CacheMetrics.create_for_write(1, bytes_written)
 
     def get_cache_state_for_threads(self, thread_ids: List[str], expect_one_message_per_thread: bool):
         unknown_thread_ids: Set[str] = set(thread_ids).difference(set(self.cached_thread_ids))
         if expect_one_message_per_thread:
             # Only query threads that are not in cache, on other words unknown.
             # All known thread IDs are stored in self.thread_ids.
             # When only one message / thread is expected, consider all known threads as fully cached.
 
             fully_cached = {}
             for t_id in self.cached_thread_ids:
                 try:
-                    fully_cached[t_id] = self._get_thread_from_file_system(t_id)
+                    fully_cached[t_id], metrics = self._get_thread_from_file_system(t_id)
+                    self._cache_actions_performed.add(GmailRequestType.THREADS_LIST, metrics)
                 except Exception as e:
-                    LOG.error("Error when processing thread.", e)
+                    LOG.error("Error while processing thread.", e)
                     LOG.warning("Cannot open file for thread: %s. Adding it to not cached threads.", t_id)
                     unknown_thread_ids.add(t_id)
 
             return (
                 CacheResultItems(thread_ids, cache_type="thread")
                 .add_not_cached(unknown_thread_ids)
                 .add_fully_cached(fully_cached)
@@ -326,43 +429,50 @@
         known_thread_ids: Set[str] = set(thread_ids).difference(unknown_thread_ids)
         return (
             CacheResultItems(thread_ids, cache_type="thread")
             .add_not_yet_determined(known_thread_ids)
             .add_not_cached(unknown_thread_ids)
         )
 
-    def get_cache_state_for_message(self, thread_id: str, message_id: str):
+    def get_cache_state_for_message(self, thread_id: str, message_id: str, attachment_id: str):
         """
         Caution: This loads all message data into memory including message payloads + attachments so the resulted
         CacheResultItems should not be kept in memory for a long time as it would just accumulate without any particular reason.
         !!Use it with care!!
         :param thread_id:
         :param message_id:
+        :param attachment_id:
         :return:
         """
         attachment_data = None
-        if message_id not in self.cached_message_attachments:
+        cache_key = (thread_id, message_id, attachment_id)
+        if cache_key not in self.cached_message_attachments:
             # Try to load from Filesystem
-            msg_attachment_filename = self._get_attachment_filename(thread_id, message_id, create_messages_dir=False)
+            msg_attachment_filename = self._get_attachment_filename(
+                thread_id, message_id, attachment_id, create_messages_dir=False
+            )
             if FileUtils.does_file_exist(msg_attachment_filename):
                 attachment_data = self._load_data_from_file(msg_attachment_filename)
-                self.cached_message_attachments.add(thread_id)
+                self.cached_message_attachments.add(cache_key)
 
-        cached = {thread_id: attachment_data} if thread_id in self.cached_message_attachments else {}
+        # if not attachment_data:
+        #     raise ValueError("BUG! Attachment data is not set!")
+        # TODO bug here, attachment_data is None --> Load from disk or memory?
+        cached = {thread_id: attachment_data} if cache_key in self.cached_message_attachments else {}
         not_cached = [] if len(cached) > 0 else [thread_id]
         return (
             CacheResultItems([message_id], cache_type="message attachment")
             .add_not_cached(not_cached)
             .add_fully_cached(cached)
         )
 
-    def _get_attachment_filename(self, thread_id, message_id, create_messages_dir=True):
+    def _get_attachment_filename(self, thread_id, message_id, attachment_id, create_messages_dir=True):
         thread_dir = self._get_thread_dir(thread_id)
         messages_dir: str = self._get_messages_dir(thread_dir, create=create_messages_dir)
-        return FileUtils.join_path(messages_dir, self._get_message_attachment_filename(message_id))
+        return FileUtils.join_path(messages_dir, self._get_message_attachment_filename(message_id, attachment_id))
 
     def _get_thread_dir(self, thread_id):
         thread_dir: str = FileUtils.join_path(self.threads_dir, thread_id)
         if not FileUtils.does_path_exist(thread_dir):
             raise ValueError(
                 f"Thread dir does not exist for thread with ID: {thread_dir}. "
                 f"This should not happen at this point of the execution."
@@ -372,15 +482,15 @@
     @staticmethod
     def _get_messages_dir(thread_dir, create=True):
         messages_dir = FileUtils.join_path(thread_dir, MESSAGES_DIR_NAME)
         if create:
             FileUtils.ensure_dir_created(messages_dir)
         return messages_dir
 
-    def _get_thread_from_file_system(self, thread_id: str):
+    def _get_thread_from_file_system(self, thread_id: str) -> Tuple[Any, CacheMetrics]:
         """
         Caution: This loads all thread data into memory including message payloads.
         !!Use it with care!!
         :param thread_id:
         :return:
         """
         if thread_id not in self.cached_thread_ids:
@@ -391,80 +501,64 @@
     def actualize_cache_state(self, cache_state: CacheResultItems, thread_id: str, message_ids: List[str]):
         message_ids_for_thread: List[str] = (
             self.thread_to_message_data[thread_id].keys() if thread_id in self.thread_to_message_data else []
         )
         self.unknown_message_per_thread[thread_id] = set(message_ids).difference(message_ids_for_thread)
         if self.unknown_message_per_thread[thread_id]:
             cache_state.mark_partially_cached(thread_id)
-            return
-        # Thread is fully cached with all messages
-        cache_state.mark_fully_cached(thread_id, self._get_thread_from_file_system(thread_id))
+        else:
+            # Thread is fully cached with all messages
+            data, metrics = self._get_thread_from_file_system(thread_id)
+            self._cache_actions_performed.add(GmailRequestType.MESSAGES, metrics)
+            cache_state.mark_fully_cached(thread_id, data)
 
     @staticmethod
     def _convert_thread_response_to_message_data_dicts(thread_response):
         messages_response: List[Dict[str, Any]] = GH.get_field(thread_response, ThreadField.MESSAGES)
         message_data_dicts: List[Dict[str, str]] = []
         for msg in messages_response:
             message_data_dicts.append(
                 {MESSAGE_ID: GH.get_field(msg, MessageField.ID), MESSAGE_DATE: GH.get_field(msg, MessageField.DATE)}
             )
         return message_data_dicts
 
     @staticmethod
-    def _get_message_attachment_filename(message_id):
-        return f"message_{message_id}_attachment.txt"
+    def _get_message_attachment_filename(message_id, attachment_id):
+        short_attachment_id = StringUtils.md5_hash(attachment_id)
+        return f"message_{message_id}_attachment_{short_attachment_id}.txt"
+
+    def print_actions_performed(self):
+        self._cache_actions_performed.print_all()
 
 
 class NoCacheStrategy(CachingStrategy):
+    def get_cached_threads(self):
+        LOG.debug(f"Invoked get_cached_threads of {type(self).__name__}")
+        return []
+
     def actualize_cache_state(self, cache_state: CacheResultItems, thread_id: str, message_ids: List[str]):
         LOG.debug(f"Invoked actualize_cache_state of {type(self).__name__}")
 
     def get_cache_state_for_threads(self, thread_ids: List[str], expect_one_message_per_thread):
         return CacheResultItems(thread_ids, cache_type="thread").add_not_cached(thread_ids)
 
-    def get_cache_state_for_message(self, thread_id: str, message_id: str):
+    def get_cache_state_for_message(self, thread_id: str, message_id: str, attachment_id: str):
         return CacheResultItems([thread_id], cache_type="message").add_not_cached([message_id])
 
     def fill_cache(self):
         LOG.debug(f"Invoked fill_cache of {type(self).__name__}")
 
     def process_threads(self, thread_response: Dict[str, Any]):
         LOG.debug(f"Invoked process_threads of {type(self).__name__} with an email thread")
 
-    def process_attachment_for_message(self, thread_id: str, message_id: str, attachment_response: Dict[str, Any]):
+    def process_attachment_for_message(
+        self, thread_id: str, message_id: str, attachment_id: str, attachment_response: Dict[str, Any]
+    ):
         LOG.debug(f"Invoked process_attachment_for_message of {type(self).__name__} with an email attachment")
 
-
-class ApiFetchingContext:
-    def __init__(self, strategy: CachingStrategy) -> None:
-        # TODO log debug cache strategy type
-        self._caching_strategy = strategy
-
-    @property
-    def caching_strategy(self) -> CachingStrategy:
-        return self._caching_strategy
-
-    @caching_strategy.setter
-    def caching_strategy(self, strategy: CachingStrategy) -> None:
-        self._caching_strategy = strategy
-
-    def process_thread(self, thread_response: Dict[str, Any]):
-        self._caching_strategy.process_threads(thread_response)
-
-    def process_messages(self, cache_state: CacheResultItems, thread_id: str, message_ids: List[str]):
-        self._caching_strategy.actualize_cache_state(cache_state, thread_id, message_ids)
-
-    def process_attachment_for_message(self, thread_id: str, message_id: str, attachment_response: Dict[str, Any]):
-        self._caching_strategy.process_attachment_for_message(thread_id, message_id, attachment_response)
-
-    def get_cache_state_for_threads(
-        self, thread_ids: List[str], expect_one_message_per_thread: bool
-    ) -> CacheResultItems:
-        return self._caching_strategy.get_cache_state_for_threads(thread_ids, expect_one_message_per_thread)
-
-    def get_cache_state_for_message(self, thread_id: str, message_id: str) -> CacheResultItems:
-        return self._caching_strategy.get_cache_state_for_message(thread_id, message_id)
+    def print_actions_performed(self):
+        LOG.info("No cache actions were performed!")
 
 
 class CachingStrategyType(Enum):
     NO_CACHE = NoCacheStrategy
     FILESYSTEM_CACHE_STRATEGY = FileSystemEmailThreadCacheStrategy
```

### Comparing `google-api-wrapper2-1.0.5/googleapiwrapper/gmail_domain.py` & `google-api-wrapper2-1.0.6/googleapiwrapper/gmail_domain.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,21 +3,24 @@
 import sys
 from dataclasses import dataclass, field, InitVar
 import datetime
 from enum import Enum
 from typing import List, Dict, Any
 
 from googleapiwrapper.utils import Decoder
+
 LOG = logging.getLogger(__name__)
 
 
 class ThreadQueryFormat(Enum):
+    # https://developers.google.com/gmail/api/reference/rest/v1/Format
     FULL = "full"
     METADATA = "metadata"
     MINIMAL = "minimal"
+    RAW = "raw"
 
 
 class HeaderField(Enum):
     NAME = "name"
     VALUE = "value"
 
 
@@ -65,19 +68,14 @@
     SNIPPET = "snippet"
 
 
 class ThreadQueryParam(Enum):
     FORMAT = "format"
 
 
-class ApiItemType(Enum):
-    THREAD = "thread"
-    MESSAGE = "message"
-
-
 class MimeType(Enum):
     TEXT_PLAIN = "text/plain"
 
 
 @dataclass
 class MessagePartBody:
     data: str
@@ -99,51 +97,91 @@
     id: str
     mime_type: str
     headers: List[Header]
     body: MessagePartBody
     parts: List[Any]  # Cannot refer to MessagePart :(
 
     def short_str(self):
-        return f"{{ ID: {self.id}, " \
-               f"mime_type: {self.mime_type}, " \
-               f"headers: {self.headers}, " \
-               f"body (short): {self.body.short_str()}, " \
-               f"parts (short): {[part.short_str() for part in self.parts]} }}"
+        return (
+            f"{{ ID: {self.id}, "
+            f"mime_type: {self.mime_type}, "
+            f"headers: {self.headers}, "
+            f"body (short): {self.body.short_str()}, "
+            f"parts (short): {[part.short_str() for part in self.parts]} }}"
+        )
 
 
 @dataclass
 class Message:
     id: str
     thread_id: str
     date: datetime.datetime
     snippet: str
     payload: MessagePart
     subject: str = field(init=False)
     message_parts: List[MessagePart] = field(init=False)
 
     def __post_init__(self):
         self.subject = self._get_subject_from_headers()
+        self.sender = self._get_sender_from_headers()
+        self.sender_email = self._extract_sender_email(self.sender)
+        self.recipient = self._get_recipient_from_headers()
+        self.recipient_email = self._extract_recipient_email(self.recipient)
+        self.date_str = self._get_date_from_headers()
         self.message_parts: List[MessagePart] = self._get_all_msg_parts_recursive(self.payload)
 
     def _get_subject_from_headers(self):
+        return self._get_field_from_headers("Subject")
+
+    def _get_sender_from_headers(self):
+        return self._get_field_from_headers("From")
+
+    def _get_recipient_from_headers(self):
+        return self._get_field_from_headers("To")
+
+    def _get_date_from_headers(self):
+        return self._get_field_from_headers("Date")
+
+    def _get_field_from_headers(self, f_name):
         for header in self.payload.headers:
-            if header.name == 'Subject':
+            if header.name == f_name:
                 return header.value
+        LOG.error("Header with name '%s' not found for message with thread ID: %s", f_name, self.thread_id)
         return None
 
     def _get_all_msg_parts_recursive(self, msg_part: MessagePart):
         lst: List[MessagePart] = []
         for part in msg_part.parts:
             lst += self._get_all_msg_parts_recursive(part)
         lst.append(msg_part)
         return lst
 
     def short_str(self):
         return f"{{ ID: {self.id}, snippet: {self.snippet}, subject: {self.subject} }}"
 
+    @staticmethod
+    def _extract_sender_email(s):
+        return Message._extract_email_from_raw(s, "sender")
+
+    @staticmethod
+    def _extract_recipient_email(r):
+        return Message._extract_email_from_raw(r, "recipient")
+
+    @staticmethod
+    def _extract_email_from_raw(raw_str, item_type):
+        try:
+            start = raw_str.index("<")
+            end = raw_str.index(">", start + 1)
+            return raw_str[start + 1 : end]
+        except Exception:
+            LOG.warning(
+                "Cannot extract email address from: %s. Using the original %s as email address", raw_str, item_type
+            )
+            return raw_str
+
 
 @dataclass
 class Thread:
     id: str
     subject: str
     messages: List[Message]
 
@@ -164,29 +202,45 @@
 
 @dataclass
 class GmailMessage:
     msg_id: str
     thread_id: str
     subject: str
     date: datetime.datetime
+    sender: str
+    sender_email: str
+    recipient: str
+    recipient_email: str
+    date_str: str
     message_parts: InitVar[List[MessagePart]]
 
     def __post_init__(self, message_parts):
         self.message_body_parts: List[GmailMessageBodyPart] = self._convert_message_parts(message_parts)
 
     @staticmethod
     def _get_conversion_context():
         module = sys.modules["googleapiwrapper.gmail_api"]
         return module.__getattribute__("CONVERSION_CONTEXT")
 
     @staticmethod
     def from_message(message: Message, thread_id: str):
         GmailMessage._get_conversion_context().register_current_message(message)
         # message.message_parts already contains all MessageParts (recursively collected)
-        return GmailMessage(message.id, thread_id, message.subject, message.date, message.message_parts)
+        return GmailMessage(
+            message.id,
+            thread_id,
+            message.subject,
+            message.date,
+            message.sender,
+            message.sender_email,
+            message.recipient,
+            message.recipient_email,
+            message.date_str,
+            message.message_parts,
+        )
 
     def _convert_message_parts(self, message_parts: List[MessagePart]) -> List[GmailMessageBodyPart]:
         result: List[GmailMessageBodyPart] = []
         CONVERSION_CONTEXT = GmailMessage._get_conversion_context()
         for message_part in message_parts:
             CONVERSION_CONTEXT.register_current_message_part(message_part)
             mime_type: str = message_part.mime_type
@@ -201,62 +255,68 @@
 
     def _decode_base64_encoded_body(self, message_part: MessagePart):
         encoded_body_data = message_part.body.data
         successful = True
         empty = False
         try:
             if encoded_body_data:
-                decoded_body_data = Decoder.decode_base64(encoded_body_data)
+                decoded_body_data = Decoder.decode_base64_urlsafe(encoded_body_data)
             else:
                 decoded_body_data = ""
                 empty = True
         except binascii.Error:
-            LOG.exception(f"Failed to parse base64 encoded data for message with ID: {self.msg_id}."
-                          f"Storing original body data to object and storing original API object as well.")
+            LOG.exception(
+                f"Failed to parse base64 encoded data for message with ID: {self.msg_id}."
+                f"Storing original body data to object and storing original API object as well."
+            )
             decoded_body_data = encoded_body_data
             successful = False
         return decoded_body_data, successful, empty
 
     def get_all_plain_text_parts(self) -> List[GmailMessageBodyPart]:
         return self.get_all_parts_with_type(MimeType.TEXT_PLAIN)
 
     def get_all_parts_with_type(self, mime_type: MimeType) -> List[GmailMessageBodyPart]:
         return self._filter_by_mime_type(mime_type, self.message_body_parts)
 
     @staticmethod
-    def _filter_by_mime_type(mime_type: MimeType, message_parts: List[GmailMessageBodyPart]) -> List[
-        GmailMessageBodyPart]:
+    def _filter_by_mime_type(
+        mime_type: MimeType, message_parts: List[GmailMessageBodyPart]
+    ) -> List[GmailMessageBodyPart]:
         return list(filter(lambda x: x.mime_type == mime_type.value, message_parts))
 
 
 @dataclass
 class MessagePartDescriptor:
     message: Message
     message_part: MessagePart
     gmail_msg_body_part: GmailMessageBodyPart
 
     def __str__(self):
-        return f"{{ mesage: {self.message.short_str()}, " \
-               f"message_part: {self.message_part.short_str()}, " \
-               f"gmail_msg_body_part: {self.gmail_msg_body_part} " \
-               f"}}"
+        return (
+            f"{{ mesage: {self.message.short_str()}, "
+            f"message_part: {self.message_part.short_str()}, "
+            f"gmail_msg_body_part: {self.gmail_msg_body_part} "
+            f"}}"
+        )
 
 
 class GmailThread:
     def __init__(self, api_id, messages: List[GmailMessage]):
         self.api_id = api_id
         self.messages: List[GmailMessage] = messages
 
 
 @dataclass
 class GmailThreads:
     threads: List[GmailThread] = field(default_factory=list)
 
     def add(self, thread: Thread):
-        gmail_thread = GmailThread(thread.id, [GmailMessage.from_message(m, thread.id) for m in thread.messages])
+        messages = [GmailMessage.from_message(m, thread.id) for m in thread.messages]
+        gmail_thread = GmailThread(thread.id, messages)
         self.threads.append(gmail_thread)
 
     @property
     def messages(self) -> List[GmailMessage]:
         return [msg for t in self.threads for msg in t.messages]
```

### Comparing `google-api-wrapper2-1.0.5/googleapiwrapper/google_auth.py` & `google-api-wrapper2-1.0.6/googleapiwrapper/google_auth.py`

 * *Files identical despite different names*

### Comparing `google-api-wrapper2-1.0.5/googleapiwrapper/google_drive.py` & `google-api-wrapper2-1.0.6/googleapiwrapper/google_drive.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,18 @@
+import io
 import logging
 import os
 from dataclasses import dataclass
 from enum import Enum
-from typing import List, Dict, Any, Tuple
+from typing import List, Dict, Any
 
 from googleapiclient.discovery import build
+from googleapiclient.errors import HttpError
 from googleapiclient.http import MediaFileUpload
+from googleapiclient.http import MediaIoBaseDownload
 from pythoncommons.file_utils import FileUtils
 from pythoncommons.object_utils import ObjUtils
 from pythoncommons.string_utils import auto_str, StringUtils
 
 from googleapiwrapper.google_auth import GoogleApiAuthorizer
 
 LOG = logging.getLogger(__name__)
@@ -116,25 +119,27 @@
     MODIFIED_TIME = "modifiedTime"
     CREATED_TIME = "createdTime"
     LINK = "webViewLink"
     MIMETYPE = "mimeType"
     NAME = "name"
     ID = "id"
     PARENTS = "parents"
+    SIZE = "size"
 
     _ALL_FIELDS_WITH_DISPLAY_NAME = [
         (ID, "ID"),
         (NAME, "Name"),
         (MIMETYPE, "Type"),
         (LINK, "Link"),
         (CREATED_TIME, "Created date"),
         (MODIFIED_TIME, "Last modified time"),
         (SHARED_WITH_ME_TIME, "Shared with me date"),
         (F_OWNER, "Owner"),
         (PARENTS, "Parents"),
+        (SIZE, "Size"),
     ]
 
     PRINTABLE_FIELD_DISPLAY_NAMES = [
         "Name",
         "Link",
         "Shared with me date",
         "Owner",
@@ -185,14 +190,15 @@
         link,
         created_date,
         modified_date,
         shared_with_me_date,
         mime_type,
         owners,
         sharing_user: DriveApiUser or None,
+        size,
         parents,
         parent: Any = None,
     ):
         super(DriveApiFile, self).__init__()
         self.id = id
         self.name = StringUtils.replace_special_chars(name)
         self.link = link
@@ -200,14 +206,15 @@
         self.modified_date = modified_date
         self.shared_with_me_date = shared_with_me_date
         self.mime_type = mime_type
         self.owners = owners
 
         sharing_user.name = StringUtils.replace_special_chars(sharing_user.name)
         self.sharing_user = sharing_user
+        self.size = size
         self.parents = parents
         self._parent = parent
 
     @staticmethod
     def create_root_api_file():
         return DriveApiFile("N/A", "/", "N/A", "N/A", "N/A", "N/A", DriveApiMimeType.FOLDER, "N/A", None, None)
 
@@ -747,15 +754,42 @@
             DriveApiWrapper._safe_get(item, FileField.LINK),
             DriveApiWrapper._safe_get(item, FileField.CREATED_TIME),
             DriveApiWrapper._safe_get(item, FileField.MODIFIED_TIME),
             DriveApiWrapper._safe_get(item, FileField.SHARED_WITH_ME_TIME),
             DriveApiWrapper._safe_get(item, FileField.MIMETYPE),
             owners,
             sharing_user,
+            DriveApiWrapper._safe_get(item, FileField.SIZE),
             DriveApiWrapper._safe_get(item, FileField.PARENTS),
         )
 
     @staticmethod
     def _safe_get(d: Dict[str, str], key: str):
         if key not in d:
             return None
         return d[key]
+
+    def download_file(self, file_id):
+        """Downloads a file
+        Args:
+            file_id: ID of the file to download
+        Returns : IO object with location.
+
+        Load pre-authorized user credentials from the environment.
+        TODO(developer) - See https://developers.google.com/identity
+        for guides on implementing OAuth2 for the application.
+        """
+        try:
+            # pylint: disable=maybe-no-member
+            request = self.files_service.get_media(fileId=file_id)
+            file = io.BytesIO()
+            downloader = MediaIoBaseDownload(file, request)
+            done = False
+            while done is False:
+                status, done = downloader.next_chunk()
+                LOG.debug(f"Download {int(status.progress() * 100)}.")
+
+        except HttpError as error:
+            LOG.debug(f"An error occurred: {error}")
+            file = None
+
+        return file
```

### Comparing `google-api-wrapper2-1.0.5/googleapiwrapper/google_sheet.py` & `google-api-wrapper2-1.0.6/googleapiwrapper/google_sheet.py`

 * *Files identical despite different names*

### Comparing `google-api-wrapper2-1.0.5/pyproject.toml` & `google-api-wrapper2-1.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -13,23 +13,23 @@
   | build
   | dist
 )/
 '''
 
 [tool.poetry]
 name = "google-api-wrapper2"
-version = "1.0.5"
+version = "1.0.6"
 description = ""
 authors = ["Szilard Nemeth <szilard.nemeth88@gmail.com>"]
 readme = "README.md"
 packages = [{include = "googleapiwrapper"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-python-common-lib = "1.0.6"
+python-common-lib = "1.0.8"
 google-api-python-client = "2.31.0"
 google-auth-httplib2 = "0.1.0"
 google-auth-oauthlib = "0.4.6"
 oauth2client = "^4.1.3"
 gspread = ">=5.1.1"
```

### Comparing `google-api-wrapper2-1.0.5/setup.py` & `google-api-wrapper2-1.0.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 
 install_requires = \
 ['google-api-python-client==2.31.0',
  'google-auth-httplib2==0.1.0',
  'google-auth-oauthlib==0.4.6',
  'gspread>=5.1.1',
  'oauth2client>=4.1.3,<5.0.0',
- 'python-common-lib==1.0.6']
+ 'python-common-lib==1.0.8']
 
 setup_kwargs = {
     'name': 'google-api-wrapper2',
-    'version': '1.0.5',
+    'version': '1.0.6',
     'description': '',
     'long_description': '# google-api-wrapper\n\nRun ./setup.sh to set up git pre/post push hook scripts.\nThen, a similar script loaded to the environment will execute the pre/post push hook scripts: \nhttps://stackoverflow.com/a/3812238/1106893\n\nFor example loading this script and defining an alias like this will do the trick:\n`alias gpwh="git-push-with-hooks.sh"`\n\n\n## Setup of precommit\n\nConfigure precommit as described in this blogpost: https://ljvmiranda921.github.io/notebook/2018/06/21/precommits-using-black-and-flake8/\nCommands:\n1. Install precommit: `pip install pre-commit`\n2. Make sure to add pre-commit to your path. For example, on a Mac system, pre-commit is installed here: \n   `$HOME/Library/Python/3.8/bin/pre-commit`.\n2. Execute `pre-commit install` to install git hooks in your `.git/` directory.\n\n## Troubleshooting\n\n### Installation issues\nIn case you\'re facing a similar issue:\n```\nAn error has occurred: InvalidManifestError: \n=====> /<userhome>/.cache/pre-commit/repoBP08UH/.pre-commit-hooks.yaml does not exist\nCheck the log at /<userhome>/.cache/pre-commit/pre-commit.log\n```\n, please run: `pre-commit autoupdate`\nMore info here: https://github.com/pre-commit/pre-commit/issues/577',
     'author': 'Szilard Nemeth',
     'author_email': 'szilard.nemeth88@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `google-api-wrapper2-1.0.5/PKG-INFO` & `google-api-wrapper2-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: google-api-wrapper2
-Version: 1.0.5
+Version: 1.0.6
 Summary: 
 Author: Szilard Nemeth
 Author-email: szilard.nemeth88@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: google-api-python-client (==2.31.0)
 Requires-Dist: google-auth-httplib2 (==0.1.0)
 Requires-Dist: google-auth-oauthlib (==0.4.6)
 Requires-Dist: gspread (>=5.1.1)
 Requires-Dist: oauth2client (>=4.1.3,<5.0.0)
-Requires-Dist: python-common-lib (==1.0.6)
+Requires-Dist: python-common-lib (==1.0.8)
 Description-Content-Type: text/markdown
 
 # google-api-wrapper
 
 Run ./setup.sh to set up git pre/post push hook scripts.
 Then, a similar script loaded to the environment will execute the pre/post push hook scripts: 
 https://stackoverflow.com/a/3812238/1106893
```

