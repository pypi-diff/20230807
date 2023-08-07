# Comparing `tmp/datadog_lambda-4.77.0.tar.gz` & `tmp/datadog_lambda-4.78.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datadog_lambda-4.77.0.tar", max compression
+gzip compressed data, was "datadog_lambda-4.78.0.tar", max compression
```

## Comparing `datadog_lambda-4.77.0.tar` & `datadog_lambda-4.78.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    11379 2023-07-29 00:54:04.905729 datadog_lambda-4.77.0/LICENSE
--rw-r--r--   0        0        0      394 2023-07-29 00:54:04.905809 datadog_lambda-4.77.0/LICENSE-3rdparty.csv
--rw-r--r--   0        0        0     3428 2023-07-29 00:54:04.905961 datadog_lambda-4.77.0/README.md
--rw-r--r--   0        0        0      538 2023-07-29 00:54:04.906090 datadog_lambda-4.77.0/datadog_lambda/__init__.py
--rw-r--r--   0        0        0     3653 2023-07-29 00:54:04.906180 datadog_lambda-4.77.0/datadog_lambda/api.py
--rw-r--r--   0        0        0     8013 2023-07-29 00:54:04.906280 datadog_lambda-4.77.0/datadog_lambda/cold_start.py
--rw-r--r--   0        0        0     1669 2023-07-29 00:54:04.906364 datadog_lambda-4.77.0/datadog_lambda/constants.py
--rw-r--r--   0        0        0     4769 2023-07-29 00:54:04.906451 datadog_lambda-4.77.0/datadog_lambda/dogstatsd.py
--rw-r--r--   0        0        0     1199 2023-07-29 00:54:04.906536 datadog_lambda-4.77.0/datadog_lambda/extension.py
--rw-r--r--   0        0        0      994 2023-07-29 00:54:04.906616 datadog_lambda-4.77.0/datadog_lambda/handler.py
--rw-r--r--   0        0        0     4707 2023-07-29 00:54:04.906722 datadog_lambda-4.77.0/datadog_lambda/metric.py
--rw-r--r--   0        0        0      139 2023-07-29 00:54:04.906797 datadog_lambda-4.77.0/datadog_lambda/module_name.py
--rw-r--r--   0        0        0     4641 2023-07-29 00:54:04.906895 datadog_lambda-4.77.0/datadog_lambda/patch.py
--rw-r--r--   0        0        0      243 2023-07-29 00:54:04.906974 datadog_lambda-4.77.0/datadog_lambda/stats_writer.py
--rw-r--r--   0        0        0      403 2023-07-29 00:54:04.907059 datadog_lambda-4.77.0/datadog_lambda/statsd_writer.py
--rw-r--r--   0        0        0     1751 2023-07-29 00:54:04.907139 datadog_lambda-4.77.0/datadog_lambda/tag_object.py
--rw-r--r--   0        0        0     3240 2023-07-29 00:54:04.907240 datadog_lambda-4.77.0/datadog_lambda/tags.py
--rw-r--r--   0        0        0     2522 2023-07-29 00:54:04.907335 datadog_lambda-4.77.0/datadog_lambda/thread_stats_writer.py
--rw-r--r--   0        0        0    47331 2023-07-29 00:54:04.907532 datadog_lambda-4.77.0/datadog_lambda/tracing.py
--rw-r--r--   0        0        0    12082 2023-07-29 00:54:04.907647 datadog_lambda-4.77.0/datadog_lambda/trigger.py
--rw-r--r--   0        0        0    14393 2023-07-29 00:54:04.907751 datadog_lambda-4.77.0/datadog_lambda/wrapper.py
--rw-r--r--   0        0        0     3449 2023-07-29 00:54:04.907833 datadog_lambda-4.77.0/datadog_lambda/xray.py
--rw-r--r--   0        0        0     1313 2023-07-31 14:07:04.189029 datadog_lambda-4.77.0/pyproject.toml
--rw-r--r--   0        0        0     4787 1970-01-01 00:00:00.000000 datadog_lambda-4.77.0/PKG-INFO
+-rw-r--r--   0        0        0    11379 2022-09-22 18:30:00.504292 datadog_lambda-4.78.0/LICENSE
+-rw-r--r--   0        0        0      394 2022-09-22 18:30:00.504380 datadog_lambda-4.78.0/LICENSE-3rdparty.csv
+-rw-r--r--   0        0        0     3428 2023-07-28 17:52:05.373002 datadog_lambda-4.78.0/README.md
+-rw-r--r--   0        0        0      538 2023-02-13 20:46:09.160997 datadog_lambda-4.78.0/datadog_lambda/__init__.py
+-rw-r--r--   0        0        0     3653 2022-09-22 18:30:00.504778 datadog_lambda-4.78.0/datadog_lambda/api.py
+-rw-r--r--   0        0        0     8013 2023-06-30 13:40:04.094622 datadog_lambda-4.78.0/datadog_lambda/cold_start.py
+-rw-r--r--   0        0        0     1669 2023-01-25 19:31:51.675529 datadog_lambda-4.78.0/datadog_lambda/constants.py
+-rw-r--r--   0        0        0     4769 2022-09-22 18:30:00.505031 datadog_lambda-4.78.0/datadog_lambda/dogstatsd.py
+-rw-r--r--   0        0        0     1199 2022-09-22 18:30:00.505121 datadog_lambda-4.78.0/datadog_lambda/extension.py
+-rw-r--r--   0        0        0      994 2022-09-22 18:30:00.505207 datadog_lambda-4.78.0/datadog_lambda/handler.py
+-rw-r--r--   0        0        0     4707 2022-09-22 18:30:00.505343 datadog_lambda-4.78.0/datadog_lambda/metric.py
+-rw-r--r--   0        0        0      139 2022-09-22 18:30:00.505417 datadog_lambda-4.78.0/datadog_lambda/module_name.py
+-rw-r--r--   0        0        0     4641 2022-09-22 18:30:00.505516 datadog_lambda-4.78.0/datadog_lambda/patch.py
+-rw-r--r--   0        0        0      243 2022-09-22 18:30:00.505686 datadog_lambda-4.78.0/datadog_lambda/stats_writer.py
+-rw-r--r--   0        0        0      403 2022-09-22 18:30:00.505792 datadog_lambda-4.78.0/datadog_lambda/statsd_writer.py
+-rw-r--r--   0        0        0     1751 2022-09-22 18:30:00.505884 datadog_lambda-4.78.0/datadog_lambda/tag_object.py
+-rw-r--r--   0        0        0     3240 2022-09-22 18:30:00.505984 datadog_lambda-4.78.0/datadog_lambda/tags.py
+-rw-r--r--   0        0        0     2522 2022-09-22 18:30:00.506089 datadog_lambda-4.78.0/datadog_lambda/thread_stats_writer.py
+-rw-r--r--   0        0        0    49291 2023-08-07 14:59:32.781852 datadog_lambda-4.78.0/datadog_lambda/tracing.py
+-rw-r--r--   0        0        0    12082 2023-04-12 17:19:32.172228 datadog_lambda-4.78.0/datadog_lambda/trigger.py
+-rw-r--r--   0        0        0    14393 2023-06-30 13:40:04.095559 datadog_lambda-4.78.0/datadog_lambda/wrapper.py
+-rw-r--r--   0        0        0     3449 2023-03-22 12:07:02.672991 datadog_lambda-4.78.0/datadog_lambda/xray.py
+-rw-r--r--   0        0        0     1313 2023-08-07 16:08:28.919277 datadog_lambda-4.78.0/pyproject.toml
+-rw-r--r--   0        0        0     4787 1970-01-01 00:00:00.000000 datadog_lambda-4.78.0/PKG-INFO
```

### Comparing `datadog_lambda-4.77.0/LICENSE` & `datadog_lambda-4.78.0/LICENSE`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.77.0/README.md` & `datadog_lambda-4.78.0/README.md`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.77.0/datadog_lambda/__init__.py` & `datadog_lambda-4.78.0/datadog_lambda/__init__.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.77.0/datadog_lambda/api.py` & `datadog_lambda-4.78.0/datadog_lambda/api.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.77.0/datadog_lambda/cold_start.py` & `datadog_lambda-4.78.0/datadog_lambda/cold_start.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.77.0/datadog_lambda/constants.py` & `datadog_lambda-4.78.0/datadog_lambda/constants.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.77.0/datadog_lambda/dogstatsd.py` & `datadog_lambda-4.78.0/datadog_lambda/dogstatsd.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.77.0/datadog_lambda/extension.py` & `datadog_lambda-4.78.0/datadog_lambda/extension.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.77.0/datadog_lambda/handler.py` & `datadog_lambda-4.78.0/datadog_lambda/handler.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.77.0/datadog_lambda/metric.py` & `datadog_lambda-4.78.0/datadog_lambda/metric.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.77.0/datadog_lambda/patch.py` & `datadog_lambda-4.78.0/datadog_lambda/patch.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.77.0/datadog_lambda/tag_object.py` & `datadog_lambda-4.78.0/datadog_lambda/tag_object.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.77.0/datadog_lambda/tags.py` & `datadog_lambda-4.78.0/datadog_lambda/tags.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.77.0/datadog_lambda/thread_stats_writer.py` & `datadog_lambda-4.78.0/datadog_lambda/thread_stats_writer.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.77.0/datadog_lambda/tracing.py` & `datadog_lambda-4.78.0/datadog_lambda/tracing.py`

 * *Files 2% similar despite different names*

```diff
@@ -225,18 +225,37 @@
             }
         ]
     }
 
 
 def extract_context_from_sqs_or_sns_event_or_context(event, lambda_context):
     """
-    Extract Datadog trace context from the first SQS message attributes.
+    Extract Datadog trace context from an SQS event.
+
+    The extraction chain goes as follows:
+    EB => SQS (First records body contains EB context), or
+    SNS => SQS (First records body contains SNS context), or
+    SQS or SNS (`messageAttributes` for SQS context,
+                `MessageAttributes` for SNS context), else
+    Lambda Context.
 
     Falls back to lambda context if no trace data is found in the SQS message attributes.
     """
+
+    # EventBridge => SQS
+    try:
+        (
+            trace_id,
+            parent_id,
+            sampling_priority,
+        ) = _extract_context_from_eventbridge_sqs_event(event)
+        return trace_id, parent_id, sampling_priority
+    except Exception:
+        logger.debug("Failed extracting context as EventBridge to SQS.")
+
     try:
         first_record = event.get("Records")[0]
 
         # logic to deal with SNS => SQS event
         if "body" in first_record:
             body_str = first_record.get("body", {})
             try:
@@ -279,14 +298,38 @@
 
         return trace_id, parent_id, sampling_priority
     except Exception as e:
         logger.debug("The trace extractor returned with error %s", e)
         return extract_context_from_lambda_context(lambda_context)
 
 
+def _extract_context_from_eventbridge_sqs_event(event):
+    """
+    Extracts Datadog trace context from an SQS event triggered by
+    EventBridge.
+
+    This is only possible if first record in `Records` contains a
+    `body` field which contains the EventBridge `detail` as a JSON string.
+    """
+    try:
+        first_record = event.get("Records")[0]
+        if "body" in first_record:
+            body_str = first_record.get("body", {})
+            body = json.loads(body_str)
+
+            detail = body.get("detail")
+            dd_context = detail.get("_datadog")
+            trace_id = dd_context.get(TraceHeader.TRACE_ID)
+            parent_id = dd_context.get(TraceHeader.PARENT_ID)
+            sampling_priority = dd_context.get(TraceHeader.SAMPLING_PRIORITY)
+            return trace_id, parent_id, sampling_priority
+    except Exception:
+        raise
+
+
 def extract_context_from_eventbridge_event(event, lambda_context):
     """
     Extract datadog trace context from an EventBridge message's Details.
     This is only possible if Details is a JSON string.
     """
     try:
         detail = event.get("detail")
@@ -991,42 +1034,54 @@
     args = {
         "service": service_name,
         "resource": queue_name,
         "span_type": "web",
     }
     start_time = int(request_time_epoch) / 1000
 
-    # logic to deal with SNS => SQS event
-    sns_span = None
+    upstream_span = None
     if "body" in event_record:
         body_str = event_record.get("body", {})
         try:
             body = json.loads(body_str)
+
+            # logic to deal with SNS => SQS event
             if body.get("Type", "") == "Notification" and "TopicArn" in body:
                 logger.debug("Found SNS message inside SQS event")
-                sns_span = create_inferred_span_from_sns_event(
+                upstream_span = create_inferred_span_from_sns_event(
                     create_sns_event(body), context
                 )
-                sns_span.finish(finish_time=start_time)
+                upstream_span.finish(finish_time=start_time)
+
+            # EventBridge => SQS
+            elif body.get("detail"):
+                detail = body.get("detail")
+                if detail.get("_datadog"):
+                    logger.debug("Found an EventBridge message inside SQS event")
+                    upstream_span = create_inferred_span_from_eventbridge_event(
+                        body, context
+                    )
+                    upstream_span.finish(finish_time=start_time)
+
         except Exception as e:
             logger.debug(
-                "Unable to create SNS span from SQS message, with error %s" % e
+                "Unable to create upstream span from SQS message, with error %s" % e
             )
             pass
 
     # trace context needs to be set again as it is reset
     # when sns_span.finish executes
     tracer.context_provider.activate(trace_ctx)
     tracer.set_tags({"_dd.origin": "lambda"})
     span = tracer.trace("aws.sqs", **args)
     if span:
         span.set_tags(tags)
     span.start = start_time
-    if sns_span:
-        span.parent_id = sns_span.span_id
+    if upstream_span:
+        span.parent_id = upstream_span.span_id
 
     return span
 
 
 def create_inferred_span_from_sns_event(event, context):
     event_record = get_first_record(event)
     sns_message = event_record.get("Sns")
```

### Comparing `datadog_lambda-4.77.0/datadog_lambda/trigger.py` & `datadog_lambda-4.78.0/datadog_lambda/trigger.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.77.0/datadog_lambda/wrapper.py` & `datadog_lambda-4.78.0/datadog_lambda/wrapper.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.77.0/datadog_lambda/xray.py` & `datadog_lambda-4.78.0/datadog_lambda/xray.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.77.0/pyproject.toml` & `datadog_lambda-4.78.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datadog_lambda"
-version = "4.77.0"
+version = "4.78.0"
 description = "The Datadog AWS Lambda Library"
 authors = ["Datadog, Inc. <dev@datadoghq.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/DataDog/datadog-lambda-python"
 keywords = [
     "datadog",
```

### Comparing `datadog_lambda-4.77.0/PKG-INFO` & `datadog_lambda-4.78.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datadog-lambda
-Version: 4.77.0
+Version: 4.78.0
 Summary: The Datadog AWS Lambda Library
 Home-page: https://github.com/DataDog/datadog-lambda-python
 License: Apache-2.0
 Keywords: datadog,aws,lambda,layer
 Author: Datadog, Inc.
 Author-email: dev@datadoghq.com
 Requires-Python: >=3.7.0,<4
```

