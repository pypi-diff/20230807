# Comparing `tmp/smart_app_framework-2.2.0rc8-py3-none-any.whl.zip` & `tmp/smart_app_framework-2.3.0rc1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 306348 bytes, number of entries: 333
+Zip file size: 306833 bytes, number of entries: 334
 -rw-r--r--  2.0 unx      113 b- defN 80-Jan-01 00:00 core/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 core/basic_models/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 core/basic_models/actions/__init__.py
 -rw-r--r--  2.0 unx    10756 b- defN 80-Jan-01 00:00 core/basic_models/actions/basic_actions.py
--rw-r--r--  2.0 unx     6265 b- defN 80-Jan-01 00:00 core/basic_models/actions/client_profile_actions.py
+-rw-r--r--  2.0 unx     6902 b- defN 80-Jan-01 00:00 core/basic_models/actions/client_profile_actions.py
 -rw-r--r--  2.0 unx     1203 b- defN 80-Jan-01 00:00 core/basic_models/actions/command.py
 -rw-r--r--  2.0 unx     3083 b- defN 80-Jan-01 00:00 core/basic_models/actions/counter_actions.py
 -rw-r--r--  2.0 unx     1249 b- defN 80-Jan-01 00:00 core/basic_models/actions/external_actions.py
 -rw-r--r--  2.0 unx    21919 b- defN 80-Jan-01 00:00 core/basic_models/actions/push_action.py
 -rw-r--r--  2.0 unx    14039 b- defN 80-Jan-01 00:00 core/basic_models/actions/smartpay.py
 -rw-r--r--  2.0 unx    18234 b- defN 80-Jan-01 00:00 core/basic_models/actions/string_actions.py
 -rw-r--r--  2.0 unx     3538 b- defN 80-Jan-01 00:00 core/basic_models/actions/variable_actions.py
@@ -36,14 +36,15 @@
 -rw-r--r--  2.0 unx     6240 b- defN 80-Jan-01 00:00 core/basic_models/requirement/user_text_requirements.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 core/basic_models/scenarios/__init__.py
 -rw-r--r--  2.0 unx     4594 b- defN 80-Jan-01 00:00 core/basic_models/scenarios/base_scenario.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 core/basic_models/variables/__init__.py
 -rw-r--r--  2.0 unx     1553 b- defN 80-Jan-01 00:00 core/basic_models/variables/variables.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 core/configs/__init__.py
 -rw-r--r--  2.0 unx     1931 b- defN 80-Jan-01 00:00 core/configs/base_config.py
+-rw-r--r--  2.0 unx       64 b- defN 80-Jan-01 00:00 core/configs/config_constants.py
 -rw-r--r--  2.0 unx      514 b- defN 80-Jan-01 00:00 core/configs/global_constants.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 core/db_adapter/__init__.py
 -rw-r--r--  2.0 unx     2329 b- defN 80-Jan-01 00:00 core/db_adapter/aioredis_adapter.py
 -rw-r--r--  2.0 unx     3035 b- defN 80-Jan-01 00:00 core/db_adapter/aioredis_sentinel_adapter.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 core/db_adapter/ceph/__init__.py
 -rw-r--r--  2.0 unx     2413 b- defN 80-Jan-01 00:00 core/db_adapter/ceph/ceph_adapter.py
 -rw-r--r--  2.0 unx      114 b- defN 80-Jan-01 00:00 core/db_adapter/ceph/ceph_exception.py
@@ -58,15 +59,15 @@
 -rw-r--r--  2.0 unx     1155 b- defN 80-Jan-01 00:00 core/descriptions/descriptions.py
 -rw-r--r--  2.0 unx     1662 b- defN 80-Jan-01 00:00 core/descriptions/descriptions_items.py
 -rw-r--r--  2.0 unx      626 b- defN 80-Jan-01 00:00 core/descriptions/smart_updatable_descriptions_items.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 core/logging/__init__.py
 -rw-r--r--  2.0 unx      568 b- defN 80-Jan-01 00:00 core/logging/logger_constants.py
 -rw-r--r--  2.0 unx      937 b- defN 80-Jan-01 00:00 core/logging/logger_formatter.py
 -rw-r--r--  2.0 unx      386 b- defN 80-Jan-01 00:00 core/logging/logger_handlers.py
--rw-r--r--  2.0 unx     5264 b- defN 80-Jan-01 00:00 core/logging/logger_utils.py
+-rw-r--r--  2.0 unx     5323 b- defN 80-Jan-01 00:00 core/logging/logger_utils.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 core/message/__init__.py
 -rw-r--r--  2.0 unx      765 b- defN 80-Jan-01 00:00 core/message/app_info.py
 -rw-r--r--  2.0 unx     1370 b- defN 80-Jan-01 00:00 core/message/device.py
 -rw-r--r--  2.0 unx     9475 b- defN 80-Jan-01 00:00 core/message/from_message.py
 -rw-r--r--  2.0 unx      120 b- defN 80-Jan-01 00:00 core/message/message_constants.py
 -rw-r--r--  2.0 unx      179 b- defN 80-Jan-01 00:00 core/message/msg_validator.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 core/model/__init__.py
@@ -87,30 +88,30 @@
 -rw-r--r--  2.0 unx      733 b- defN 80-Jan-01 00:00 core/monitoring/twisted_server.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 core/mq/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 core/mq/kafka/__init__.py
 -rw-r--r--  2.0 unx     2792 b- defN 80-Jan-01 00:00 core/mq/kafka/async_kafka_publisher.py
 -rw-r--r--  2.0 unx      300 b- defN 80-Jan-01 00:00 core/mq/kafka/base_kafka_consumer.py
 -rw-r--r--  2.0 unx      175 b- defN 80-Jan-01 00:00 core/mq/kafka/base_kafka_publisher.py
 -rw-r--r--  2.0 unx     5208 b- defN 80-Jan-01 00:00 core/mq/kafka/kafka_consumer.py
--rw-r--r--  2.0 unx     4526 b- defN 80-Jan-01 00:00 core/mq/kafka/kafka_publisher.py
+-rw-r--r--  2.0 unx     4624 b- defN 80-Jan-01 00:00 core/mq/kafka/kafka_publisher.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 core/names/__init__.py
 -rw-r--r--  2.0 unx      749 b- defN 80-Jan-01 00:00 core/names/field.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 core/repositories/__init__.py
 -rw-r--r--  2.0 unx     1392 b- defN 80-Jan-01 00:00 core/repositories/base_repository.py
 -rw-r--r--  2.0 unx     7705 b- defN 80-Jan-01 00:00 core/repositories/classifier_repository.py
 -rw-r--r--  2.0 unx      519 b- defN 80-Jan-01 00:00 core/repositories/csv_repository.py
 -rw-r--r--  2.0 unx     1580 b- defN 80-Jan-01 00:00 core/repositories/dill_repository.py
 -rw-r--r--  2.0 unx     2707 b- defN 80-Jan-01 00:00 core/repositories/file_repository.py
 -rw-r--r--  2.0 unx     2541 b- defN 80-Jan-01 00:00 core/repositories/folder_repository.py
 -rw-r--r--  2.0 unx      588 b- defN 80-Jan-01 00:00 core/repositories/items_repository.py
 -rw-r--r--  2.0 unx     1674 b- defN 80-Jan-01 00:00 core/repositories/shard_repository.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 core/request/__init__.py
 -rw-r--r--  2.0 unx      921 b- defN 80-Jan-01 00:00 core/request/base_request.py
 -rw-r--r--  2.0 unx      268 b- defN 80-Jan-01 00:00 core/request/external_requests.py
--rw-r--r--  2.0 unx     2452 b- defN 80-Jan-01 00:00 core/request/kafka_request.py
+-rw-r--r--  2.0 unx     2434 b- defN 80-Jan-01 00:00 core/request/kafka_request.py
 -rw-r--r--  2.0 unx     1750 b- defN 80-Jan-01 00:00 core/request/rest_request.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 core/text_preprocessing/__init__.py
 -rw-r--r--  2.0 unx     2167 b- defN 80-Jan-01 00:00 core/text_preprocessing/base.py
 -rw-r--r--  2.0 unx     1238 b- defN 80-Jan-01 00:00 core/text_preprocessing/constants.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 core/text_preprocessing/grammem/__init__.py
 -rw-r--r--  2.0 unx     1816 b- defN 80-Jan-01 00:00 core/text_preprocessing/grammem/grammem_constants.py
 -rw-r--r--  2.0 unx    12320 b- defN 80-Jan-01 00:00 core/text_preprocessing/helpers.py
@@ -239,15 +240,15 @@
 -rw-r--r--  2.0 unx     3369 b- defN 80-Jan-01 00:00 smart_kit/models/dialogue_manager.py
 -rw-r--r--  2.0 unx     5280 b- defN 80-Jan-01 00:00 smart_kit/models/smartapp_model.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 smart_kit/names/__init__.py
 -rw-r--r--  2.0 unx      144 b- defN 80-Jan-01 00:00 smart_kit/names/action_params_names.py
 -rw-r--r--  2.0 unx      124 b- defN 80-Jan-01 00:00 smart_kit/names/field.py
 -rw-r--r--  2.0 unx      360 b- defN 80-Jan-01 00:00 smart_kit/names/message_names.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 smart_kit/request/__init__.py
--rw-r--r--  2.0 unx     1394 b- defN 80-Jan-01 00:00 smart_kit/request/kafka_request.py
+-rw-r--r--  2.0 unx     1887 b- defN 80-Jan-01 00:00 smart_kit/request/kafka_request.py
 -rw-r--r--  2.0 unx    24642 b- defN 80-Jan-01 00:00 smart_kit/resources/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 smart_kit/start_points/__init__.py
 -rw-r--r--  2.0 unx     1198 b- defN 80-Jan-01 00:00 smart_kit/start_points/app.py
 -rw-r--r--  2.0 unx     6735 b- defN 80-Jan-01 00:00 smart_kit/start_points/base_main_loop.py
 -rw-r--r--  2.0 unx       56 b- defN 80-Jan-01 00:00 smart_kit/start_points/constants.py
 -rw-r--r--  2.0 unx     7976 b- defN 80-Jan-01 00:00 smart_kit/start_points/main_loop_async_http.py
 -rw-r--r--  2.0 unx     7147 b- defN 80-Jan-01 00:00 smart_kit/start_points/main_loop_http.py
@@ -325,11 +326,11 @@
 -rw-r--r--  2.0 unx     1325 b- defN 80-Jan-01 00:00 smart_kit/utils/cache.py
 -rw-r--r--  2.0 unx     3946 b- defN 80-Jan-01 00:00 smart_kit/utils/diff.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 smart_kit/utils/logger_writer/__init__.py
 -rw-r--r--  2.0 unx     3322 b- defN 80-Jan-01 00:00 smart_kit/utils/logger_writer/logger_formatter.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 smart_kit/utils/monitoring.py
 -rw-r--r--  2.0 unx      332 b- defN 80-Jan-01 00:00 smart_kit/utils/object_location.py
 -rw-r--r--  2.0 unx      320 b- defN 80-Jan-01 00:00 smart_kit/utils/picklable_mock.py
--rw-r--r--  2.0 unx    10824 b- defN 80-Jan-01 00:00 smart_app_framework-2.2.0rc8.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 smart_app_framework-2.2.0rc8.dist-info/WHEEL
-?rw-r--r--  2.0 unx    32268 b- defN 16-Jan-01 00:00 smart_app_framework-2.2.0rc8.dist-info/RECORD
-333 files, 986512 bytes uncompressed, 253742 bytes compressed:  74.3%
+-rw-r--r--  2.0 unx    10824 b- defN 80-Jan-01 00:00 smart_app_framework-2.3.0rc1.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 smart_app_framework-2.3.0rc1.dist-info/WHEEL
+?rw-r--r--  2.0 unx    32355 b- defN 16-Jan-01 00:00 smart_app_framework-2.3.0rc1.dist-info/RECORD
+334 files, 987932 bytes uncompressed, 254087 bytes compressed:  74.3%
```

## zipnote {}

```diff
@@ -117,14 +117,17 @@
 
 Filename: core/configs/__init__.py
 Comment: 
 
 Filename: core/configs/base_config.py
 Comment: 
 
+Filename: core/configs/config_constants.py
+Comment: 
+
 Filename: core/configs/global_constants.py
 Comment: 
 
 Filename: core/db_adapter/__init__.py
 Comment: 
 
 Filename: core/db_adapter/aioredis_adapter.py
@@ -984,17 +987,17 @@
 
 Filename: smart_kit/utils/object_location.py
 Comment: 
 
 Filename: smart_kit/utils/picklable_mock.py
 Comment: 
 
-Filename: smart_app_framework-2.2.0rc8.dist-info/METADATA
+Filename: smart_app_framework-2.3.0rc1.dist-info/METADATA
 Comment: 
 
-Filename: smart_app_framework-2.2.0rc8.dist-info/WHEEL
+Filename: smart_app_framework-2.3.0rc1.dist-info/WHEEL
 Comment: 
 
-Filename: smart_app_framework-2.2.0rc8.dist-info/RECORD
+Filename: smart_app_framework-2.3.0rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## core/basic_models/actions/client_profile_actions.py

```diff
@@ -1,12 +1,13 @@
 from typing import Dict, Any, Optional, Union, List
 
 from core.basic_models.actions.command import Command
 from core.basic_models.actions.string_actions import StringAction
-from core.configs.global_constants import KAFKA
+from core.configs.config_constants import REPLY_TOPIC_KEY
+from core.configs.global_constants import KAFKA, KAFKA_REPLY_TOPIC
 from core.text_preprocessing.base import BaseTextPreprocessingResult
 from core.utils.pickle_copy import pickle_deepcopy
 from scenarios.user.user_model import User
 from smart_kit.configs import settings
 
 GIVE_ME_MEMORY = "GIVE_ME_MEMORY"
 REMEMBER_THIS = "REMEMBER_THIS"
@@ -58,20 +59,22 @@
             ],
             "consumer": {
                 "projectId": config["template_settings"]["project_id"]
             }
         })
         settings_kafka_key = config["template_settings"].get("client_profile_kafka_key")
         self.kafka_key: str = self.kafka_key or settings_kafka_key or self.DEFAULT_KAFKA_KEY
-        self.request_data = {
-            "topic_key": "client_info",
-            "kafka_key": self.kafka_key,
-            "kafka_replyTopic":
-                config["template_settings"]["consumer_topic"]
-        }
+        if self.request_data is None:
+            self.request_data = dict()
+        if "topic_key" not in self.request_data:
+            self.request_data["topic_key"] = "client_info"
+        if "kafka_key" not in self.request_data:
+            self.request_data["kafka_key"] = self.kafka_key
+        if REPLY_TOPIC_KEY not in self.request_data and KAFKA_REPLY_TOPIC not in self.request_data:
+            self.request_data[KAFKA_REPLY_TOPIC] = config["template_settings"]["consumer_topic"]
 
     async def run(self, user: User, text_preprocessing_result: BaseTextPreprocessingResult,
                   params: Optional[Dict[str, Union[str, float, int]]] = None) -> Optional[List[Command]]:
         if self.behavior:
             callback_id = user.message.generate_new_callback_id()
             scenario_id = user.last_scenarios.last_scenario_name if hasattr(user, 'last_scenarios') else None
             user.behaviors.add(callback_id, self.behavior, scenario_id,
@@ -156,18 +159,20 @@
     async def run(self, user: User, text_preprocessing_result: BaseTextPreprocessingResult,
                   params: Optional[Dict[str, Union[str, float, int]]] = None) -> Optional[List[Command]]:
         self._nodes.update({
             "consumer": {
                 "projectId": user.settings["template_settings"]["project_id"]
             }
         })
-        settings_kafka_key: Optional[str] = user.settings["template_settings"].get("client_profile_kafka_key")
-        kafka_key: str = self.kafka_key or settings_kafka_key or self.DEFAULT_KAFKA_KEY
-        self.request_data = {
-            "topic_key": "client_info_remember",
-            "kafka_key": kafka_key,
-            "kafka_replyTopic":
-                user.settings["template_settings"]["consumer_topic"]
-        }
+        if self.request_data is None:
+            self.request_data = dict()
+        if "topic_key" not in self.request_data:
+            self.request_data["topic_key"] = "client_info_remember"
+        if "kafka_key" not in self.request_data:
+            settings_kafka_key: Optional[str] = user.settings["template_settings"].get("client_profile_kafka_key")
+            kafka_key: str = self.kafka_key or settings_kafka_key or self.DEFAULT_KAFKA_KEY
+            self.request_data["kafka_key"] = kafka_key
+        if REPLY_TOPIC_KEY not in self.request_data and KAFKA_REPLY_TOPIC not in self.request_data:
+            self.request_data[KAFKA_REPLY_TOPIC] = user.settings["template_settings"]["consumer_topic"]
 
         commands = await super().run(user, text_preprocessing_result, params)
         return commands
```

## core/logging/logger_utils.py

```diff
@@ -6,27 +6,28 @@
 
 import timeout_decorator
 
 import core.basic_models.classifiers.classifiers_constants as cls_const
 import core.logging.logger_constants as log_const
 import scenarios.logging.logger_constants as scenarios_log_const
 from core.basic_models.classifiers.basic_classifiers import Classifier
+from core.configs.global_constants import KAFKA_REPLY_TOPIC
 from core.utils.masking_message import masking
 from core.utils.stats_timer import StatsTimer
 
 MESSAGE_ID_STR = "message_id"
 UID_STR = "uid"
 LOGGING_UUID = "logging_uuid"
 CLASS_NAME = "class_name"
 LOG_STORE_FOR = "log_store_for"
 HEADERS = "headers"
 
 
 class LoggerMessageCreator:
-    LOGGER_HEADERS = ["kafka_replyTopic", "app_callback_id"]
+    LOGGER_HEADERS = [KAFKA_REPLY_TOPIC, "app_callback_id"]
     ART_NAMES = [
         "channel", "type", "device_channel", "device_channel_version", "device_platform", "group",
         "device_platform_version", "device_platform_client_type", "csa_profile_id", "test_deploy"
     ]
 
     @classmethod
     def update_user_params(cls, user, params):
```

## core/mq/kafka/kafka_publisher.py

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 import logging
 import os
 import time
-from typing import Union
+from typing import Union, Optional, List, Tuple, Any
 
 from confluent_kafka import Producer
 
 import core.logging.logger_constants as log_const
 from core.logging.logger_utils import log
 from core.monitoring.monitoring import monitoring
 from core.mq.kafka.base_kafka_publisher import BaseKafkaPublisher
@@ -24,15 +24,15 @@
             timestamp = time.strftime("_%d%m%Y_")
             debug_logger.addHandler(logging.FileHandler(
                 "{}/kafka_publisher_debug{}{}.log".format(internal_log_path, timestamp, os.getpid())
             ))
             conf["logger"] = debug_logger
         self._producer = Producer(**conf)
 
-    def send(self, value: Union[str, bytes], key=None, topic_key=None, headers=None):
+    def send(self, value: Union[str, bytes], key=None, topic_key=None, headers: Optional[List[Tuple[Any, Any]]] = None):
         try:
             topic = self._config["topic"]
             if topic_key is not None:
                 topic = topic[topic_key]
             producer_params = dict()
             if key is not None:
                 producer_params["key"] = key
@@ -43,15 +43,15 @@
                 log_const.KEY_NAME: log_const.EXCEPTION_VALUE
             }
             log("KafkaProducer: Local producer queue is full (%(queue_amount)s messages awaiting delivery):"
                 " try again\n", params=params, level="ERROR")
             monitoring.got_counter("kafka_producer_exception")
         self._poll()
 
-    def send_to_topic(self, value, key=None, topic=None, headers=None):
+    def send_to_topic(self, value, key=None, topic=None, headers: Optional[List[Tuple[Any, Any]]] = None):
         try:
             if topic is None:
                 params = {
                     "message": str(value),
                     log_const.KEY_NAME: log_const.EXCEPTION_VALUE
                 }
                 log("KafkaProducer: Failed sending message %{message}s. Topic is not defined", params=params,
```

## core/request/kafka_request.py

```diff
@@ -9,15 +9,15 @@
 
 class KafkaRequest(BaseRequest):
     TOPIC_KEY = "topic_key"
     KAFKA_KEY = "kafka_key"
     TOPIC = "topic"
 
     def __init__(self, items, id=None):
-        super(KafkaRequest, self).__init__(items)
+        super().__init__(items)
         items = items or {}
         self.topic_key = items.get(self.TOPIC_KEY)
         self.kafka_key = items.get(self.KAFKA_KEY)
         # topic_key has priority over topic
         self.topic = items.get(self.TOPIC)
 
     def update_empty_items(self, items: Dict[str, str]):
```

## smart_kit/request/kafka_request.py

```diff
@@ -1,31 +1,40 @@
 from core.configs.global_constants import CALLBACK_ID_HEADER, KAFKA_REPLY_TOPIC
 from core.request.kafka_request import KafkaRequest
+from core.configs.config_constants import REPLY_TOPIC_KEY, REPLY_TOPIC
+from smart_kit.configs.settings import Settings
 
 
 class SmartKitKafkaRequest(KafkaRequest):
     KAFKA_REPLY_TOPIC = KAFKA_REPLY_TOPIC
     KAFKA_EXTRA_HEADERS = "kafka_extraHeaders"
+    REPLY_TOPIC_KEY = REPLY_TOPIC_KEY
 
     def __init__(self, items, id=None):
-        super(SmartKitKafkaRequest, self).__init__(items)
+        super().__init__(items)
         items = items or {}
         self._callback_id = items.get(self._callback_id_header_name)
         self._kafka_replyTopic = items.get(self.KAFKA_REPLY_TOPIC)
         self._kafka_extraHeaders = items.get(self.KAFKA_EXTRA_HEADERS) or {}
+        # _reply_topic_key has priority over _kafka_replyTopic
+        self._reply_topic_key = items.get(self.REPLY_TOPIC_KEY)
 
     @property
     def _callback_id_header_name(self):
         return CALLBACK_ID_HEADER
 
     def _get_new_headers(self, source_mq_message):
-        headers_dict = dict(super(SmartKitKafkaRequest, self)._get_new_headers(source_mq_message))
+        headers_dict = dict(super()._get_new_headers(source_mq_message))
         if self._callback_id:
             headers_dict[self._callback_id_header_name] = str(self._callback_id).encode()
-        if self._kafka_replyTopic:
+        if self._reply_topic_key:
+            reply_topics = Settings()["template_settings"][REPLY_TOPIC]
+            mapped_reply_topic = reply_topics[self._reply_topic_key]
+            headers_dict[self.KAFKA_REPLY_TOPIC] = str(mapped_reply_topic).encode()
+        elif self._kafka_replyTopic:
             headers_dict[self.KAFKA_REPLY_TOPIC] = str(self._kafka_replyTopic).encode()
         if self._kafka_extraHeaders:
             for k, v in self._kafka_extraHeaders.items():
                 headers_dict[k] = str(v).encode()
         headers_list = list(headers_dict.items())
         return headers_list
```

## Comparing `smart_app_framework-2.2.0rc8.dist-info/METADATA` & `smart_app_framework-2.3.0rc1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smart-app-framework
-Version: 2.2.0rc8
+Version: 2.3.0rc1
 Summary: Python-фреймворк, который позволяет создавать смартапы для виртуальных ассистентов Салют.
 Author: Salute Developers
 Author-email: developer@sberdevices.ru
 Requires-Python: >=3.8.1,<3.12
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
```

## Comparing `smart_app_framework-2.2.0rc8.dist-info/RECORD` & `smart_app_framework-2.3.0rc1.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 core/__init__.py,sha256=uN5KPc2Ikr0wwB3EtulLr431nXKfiPRfVYG9xJtzGNA,113
 core/basic_models/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 core/basic_models/actions/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 core/basic_models/actions/basic_actions.py,sha256=pAabc2bpsWg7yPus6OZYTzNYEwXfBVOOWqIb94GRMG4,10756
-core/basic_models/actions/client_profile_actions.py,sha256=C1sqkRyK1dJYwqEvAYpPv-ahuqlibGhbUYRr95HpExM,6265
+core/basic_models/actions/client_profile_actions.py,sha256=BkQg4hgY_n2B-W859Sie79552ALLIX3t9HuLrOHZ9ic,6902
 core/basic_models/actions/command.py,sha256=jOKwl0uilTYC7ZcXgcPFrxq6PTPY7zw6xc7R_RySCm8,1203
 core/basic_models/actions/counter_actions.py,sha256=I82Ej9ygVU3HWzsHF1vIQuX4BLxls3g0a183IkhfFA0,3083
 core/basic_models/actions/external_actions.py,sha256=4D5HMqX_CjHyLqbZRjrGfA7Gzyt6ggEmkFGpeL_Yayk,1249
 core/basic_models/actions/push_action.py,sha256=ZO2CgTSBJlU5OXbkijwAU0CE4KgRfqNMIsjtBksH5Pk,21919
 core/basic_models/actions/smartpay.py,sha256=gHAhQZFouC8fGm4FiIltBoqkrPc2Cdq0R1zPhfdtWNs,14039
 core/basic_models/actions/string_actions.py,sha256=iv0jIz00aaLsmqjF5HXpe0npx4ZvKkS6-kVCIIsCjnE,18234
 core/basic_models/actions/variable_actions.py,sha256=AHUxhR6bEQ0yS2VLEYBP11JnvnbpcQYjAjaWJGLSYIM,3538
@@ -35,14 +35,15 @@
 core/basic_models/requirement/user_text_requirements.py,sha256=rLIxrdIVI8ssOr-UdrTL-Fydg2oX3LylKdQ8VXAgoX8,6240
 core/basic_models/scenarios/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 core/basic_models/scenarios/base_scenario.py,sha256=mEvnvU7trAjOTu9i0tpFvQ5WLNL_MzT4SBsgESH8JK0,4594
 core/basic_models/variables/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 core/basic_models/variables/variables.py,sha256=7b_QJsUIBnqMg2wh1Gqua7XTg1EWJubPmQPovVSyU_8,1553
 core/configs/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 core/configs/base_config.py,sha256=JMoNL3BbAebKamcKMwNsveQ-_LX0dgljWDOu0IGb9Xk,1931
+core/configs/config_constants.py,sha256=AZb0qUHyYMcDrIE1EvB3eXNoGv5zWoJbP4LVfo_YYfQ,64
 core/configs/global_constants.py,sha256=KAy2QQ8ZPE5ri1GmtyuxEGEN4qlS6sopyN-a_GCEUAk,514
 core/db_adapter/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 core/db_adapter/aioredis_adapter.py,sha256=JKrYC66tHuWPyO3A-xeX5NU1PsH_TPApEKw5oxFYVWE,2329
 core/db_adapter/aioredis_sentinel_adapter.py,sha256=IKNL5SjLcj-HZ76Adalbs4IVxzhrR5NEs489rTr6A04,3035
 core/db_adapter/ceph/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 core/db_adapter/ceph/ceph_adapter.py,sha256=hK8GB5pFaNEZ5hopJ2V_2ks4x7LktBcD5dkbdgPJ-vA,2413
 core/db_adapter/ceph/ceph_exception.py,sha256=UUFOfRdcUVbc-9wPUZVUjToRGSNI-kAbRWPqmf-tOqw,114
@@ -57,15 +58,15 @@
 core/descriptions/descriptions.py,sha256=FGbN8EYbSm5FkIJDSrQgY7BJaKZjpn7sXxdWUzx3pIg,1155
 core/descriptions/descriptions_items.py,sha256=LWBTAOssEnFJKS94bsigV1vAzNSDoV_-OZEyh8cdavc,1662
 core/descriptions/smart_updatable_descriptions_items.py,sha256=997QG44D9DDyx9Kh7M_YHGzMNjTlAiMnsRT4kG4RO9g,626
 core/logging/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 core/logging/logger_constants.py,sha256=hn56NJa4uT94uZ56W7nVFxV8rJp2fczrBHJLhh2XFPM,568
 core/logging/logger_formatter.py,sha256=3gBZq87MQIj2f45MF5AcsJNAoLJVM6aUYE7C2hd-6p0,937
 core/logging/logger_handlers.py,sha256=RWetoI6jCU7UUnZrxKol0kPxOLRaMSv-h0VhzUSC5y8,386
-core/logging/logger_utils.py,sha256=gwbCzCFmdtxj0RfKOXG4HfW--YOPttHWKf8GycFvBF8,5264
+core/logging/logger_utils.py,sha256=peJfa3384S7dPJUjlE-YbBSfeNko9d1Pylc264PkztQ,5323
 core/message/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 core/message/app_info.py,sha256=N35Q5NIuwi7CADWt8DqLcg97h0IVt9Up6WhQhwmdeZ4,765
 core/message/device.py,sha256=u7XbFgDDx7n8vScd_KgMySt_ztrYnoRzwmfr4ukMOFo,1370
 core/message/from_message.py,sha256=b3-5-uOrFCU1xJ2EChW5lh7fQHGgJjyNE5lPaQkt7A4,9475
 core/message/message_constants.py,sha256=K_ZvW_IvW7bBDo5PrrWFBlfPGq9WJQuz5a4O9YWmEsc,120
 core/message/msg_validator.py,sha256=tFm5A9yTE5HoPntYPS5057c43viDuODNLryeL2mRzUI,179
 core/model/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
@@ -86,30 +87,30 @@
 core/monitoring/twisted_server.py,sha256=dsTl1ArOPPwRnFC7w9Vd9ydmHpk1lLgkxSC-UNiOpQw,733
 core/mq/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 core/mq/kafka/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 core/mq/kafka/async_kafka_publisher.py,sha256=qo3HmnUjXaXpNHPudRVykErwDlbHkM7v5ztOnIQxG5k,2792
 core/mq/kafka/base_kafka_consumer.py,sha256=AF6T7m8A2jv3RYFP3Wn0ASnEfIZblW0wc6uhUFWlZu8,300
 core/mq/kafka/base_kafka_publisher.py,sha256=aH9hXVkWbKYkxd0O2fKNmv-36LJURQzIIcIH9mBVO0A,175
 core/mq/kafka/kafka_consumer.py,sha256=UAxRDPDyrg6YtD3EYlGcAZqdLHL2l4IXSwyTrOJTImw,5208
-core/mq/kafka/kafka_publisher.py,sha256=xsGwXcDMOhL1JyJXsw3ZOjsO9Chi1GvRez11dgKdZVA,4526
+core/mq/kafka/kafka_publisher.py,sha256=Kytj7aDKCCIi3uDFK8Rka-UjuXq2xMZn8FNSUaO0YfA,4624
 core/names/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 core/names/field.py,sha256=VebaUeRz5Zsi6Q2ER0dc8DQY7eOcNq1teFiKbCni-uA,749
 core/repositories/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 core/repositories/base_repository.py,sha256=XboNMvoaSI-ZnqJcAztYCQ0gnEsUsFxNBDU8ql4ARwU,1392
 core/repositories/classifier_repository.py,sha256=jKnGOcg5np4luzwWfxTKidsRMJU5rlnT5H0f5EKbXXw,7705
 core/repositories/csv_repository.py,sha256=j0pPlqHh3lJ0Sc4DUI-FNLfms8bp4zTusYNcybkgkzs,519
 core/repositories/dill_repository.py,sha256=tmFpqJDJ-cTw0N2kEGjJG2ZBM-ajjWBcLbfCAAHy9Sk,1580
 core/repositories/file_repository.py,sha256=WItjRrdOjYYrDkUuRTkYtV_ppPevzHQxTXwWPaaW034,2707
 core/repositories/folder_repository.py,sha256=UHCPKGC8bZRT0MfvRIx8zrgbnsq2pXLVYKSiT1wlx5E,2541
 core/repositories/items_repository.py,sha256=OlLFvFIAkQ769ks6kwJo8jZcD9HwJ3l1r_Mu8mM28QI,588
 core/repositories/shard_repository.py,sha256=PMfB5S5ozYXYZjeGCBRw6C0-3yESs0tYphfUAvaY8ww,1674
 core/request/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 core/request/base_request.py,sha256=aXjPvajEMmgKNYvw3k1NLo92iTB3XcvWwnBjq2PSr7I,921
 core/request/external_requests.py,sha256=Q6jrloXWh5yAFprT8fArdzZ4-YX4RV_oCAMYDMEINBU,268
-core/request/kafka_request.py,sha256=oaLiddXQHq37NNgtDc8OaSeKU_uL6giZdFBJ-2I4FbQ,2452
+core/request/kafka_request.py,sha256=Y7COJRc-8-Cxg82UUjp6kG_Jg4MKaJApBRcVoF1jefc,2434
 core/request/rest_request.py,sha256=mNmVaXQ7H5lxRIsQvK54zItxQjpNCPyqq4wSoh33uPs,1750
 core/text_preprocessing/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 core/text_preprocessing/base.py,sha256=EKeYU95jXkVnnvkpNhMIY8SaETgePDtq_1h4Us1ecF0,2167
 core/text_preprocessing/constants.py,sha256=mLeSz0eX2oIdqfBg21Wn9HWf5QTac3sjou7SHxIpHZc,1238
 core/text_preprocessing/grammem/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 core/text_preprocessing/grammem/grammem_constants.py,sha256=ksEcF0x6YGiPL18QobO_DNVFfW1WdNiXfBSXaAFyfog,1816
 core/text_preprocessing/helpers.py,sha256=5VgF5AxWkeQu9RjUg4LJzU0_MjoqnIp415uomlKhc5o,12320
@@ -238,15 +239,15 @@
 smart_kit/models/dialogue_manager.py,sha256=SbZ_et_yeD9Mw_OPDE6zIfITMAkpaPBWcrir6kMHNFE,3369
 smart_kit/models/smartapp_model.py,sha256=7iI3KlWd9qwYz5zR0lxS9BrAhJGqvIhnXYn3ZCSCTEs,5280
 smart_kit/names/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 smart_kit/names/action_params_names.py,sha256=6zLYlEBgeBL6SzCjeLAgojxUOUPcYl0-I77mUKU6av8,144
 smart_kit/names/field.py,sha256=H9A7y0yI03Mr2N9WHCTN6tJ38lm-xHWdCLI4fBDWwu0,124
 smart_kit/names/message_names.py,sha256=pJTk9uFLz8mnHB_PY0kGDjQ9vpWZYbJF24GKAAmD0Mc,360
 smart_kit/request/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-smart_kit/request/kafka_request.py,sha256=cWYtOOiqh7Yz3AVV6Y31_lRTDwYILRr3N4yfcns3T7w,1394
+smart_kit/request/kafka_request.py,sha256=IREnerZ9WOtqUM1zaV7fMG60SgpX2pScJCtV5HDW3u8,1887
 smart_kit/resources/__init__.py,sha256=wn2ybqp9FpcZB__W4XTDdbyuRoYRFihO_Lp-WQEPhJc,24642
 smart_kit/start_points/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 smart_kit/start_points/app.py,sha256=8lcZV7SiEBzFdcF7oe-54w7hmyHfK9PQ_IDa64_kVjM,1198
 smart_kit/start_points/base_main_loop.py,sha256=Kcedoy-rAhjk2HChcxb-sWY-XlE3ptMcB4VZT6HO6WY,6735
 smart_kit/start_points/constants.py,sha256=d_XQfL3YxYswZd5AFIwugqv8EimD18ZFfPRcPJpAgK0,56
 smart_kit/start_points/main_loop_async_http.py,sha256=o2tOOpkt-J0T3fJzS-cKVBqAEwEsmshWeACbudzzBfg,7976
 smart_kit/start_points/main_loop_http.py,sha256=TNNHuwrqbrg7fpLY1pY_J43dA2hbsNs-_MePOyqo_s8,7147
@@ -324,10 +325,10 @@
 smart_kit/utils/cache.py,sha256=Lut5HMkfoeiRwCCnZoSHw7srWYn3Y0fD-hUJWckDBf8,1325
 smart_kit/utils/diff.py,sha256=UP2Zmp0VW4YZpDPe_lGQ-5L_wF5wd7J4B33kXyUINmQ,3946
 smart_kit/utils/logger_writer/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 smart_kit/utils/logger_writer/logger_formatter.py,sha256=n5N4FHjXyeZAASjVB2zhoOMsbnWiixI0OQsk4KkcDFg,3322
 smart_kit/utils/monitoring.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 smart_kit/utils/object_location.py,sha256=uJmTxBBeeyvwahiA1TMKr2rzDW9R1bh-FwK663zoBe4,332
 smart_kit/utils/picklable_mock.py,sha256=PxrgnKue58GFpVZMBGIQq36LPnITFzfNA21euCbfViE,320
-smart_app_framework-2.2.0rc8.dist-info/METADATA,sha256=IwGzi60U0Y1sy4mKvNvxNBdjK0X-jS57bSzzEfCQnR0,10824
-smart_app_framework-2.2.0rc8.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
-smart_app_framework-2.2.0rc8.dist-info/RECORD,,
+smart_app_framework-2.3.0rc1.dist-info/METADATA,sha256=UVwV1mIVOuM8wM7knO_qDfcndj8aT79FsIV8W-5JLCQ,10824
+smart_app_framework-2.3.0rc1.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+smart_app_framework-2.3.0rc1.dist-info/RECORD,,
```

