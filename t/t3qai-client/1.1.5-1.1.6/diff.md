# Comparing `tmp/t3qai_client-1.1.5-py3-none-any.whl.zip` & `tmp/t3qai_client-1.1.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 15090 bytes, number of entries: 8
+Zip file size: 15097 bytes, number of entries: 8
 -rw-rw-rw-  2.0 fat     1639 b- defN 23-Aug-03 08:00 t3qai_client/__init__.py
--rw-rw-rw-  2.0 fat    23381 b- defN 23-Aug-07 05:58 t3qai_client/t3qai_helper.py
+-rw-rw-rw-  2.0 fat    23380 b- defN 23-Aug-07 06:42 t3qai_client/t3qai_helper.py
 -rw-rw-rw-  2.0 fat     6417 b- defN 23-Aug-07 06:00 t3qai_client/t3qai_serving.py
--rw-rw-rw-  2.0 fat    11533 b- defN 23-Aug-07 06:02 t3qai_client-1.1.5.dist-info/LICENSE-2.0.txt
--rw-rw-rw-  2.0 fat     2850 b- defN 23-Aug-07 06:02 t3qai_client-1.1.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-07 06:02 t3qai_client-1.1.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       13 b- defN 23-Aug-07 06:02 t3qai_client-1.1.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      673 b- defN 23-Aug-07 06:02 t3qai_client-1.1.5.dist-info/RECORD
-8 files, 46598 bytes uncompressed, 13914 bytes compressed:  70.1%
+-rw-rw-rw-  2.0 fat    11533 b- defN 23-Aug-07 06:43 t3qai_client-1.1.6.dist-info/LICENSE-2.0.txt
+-rw-rw-rw-  2.0 fat     2850 b- defN 23-Aug-07 06:43 t3qai_client-1.1.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-07 06:43 t3qai_client-1.1.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       13 b- defN 23-Aug-07 06:43 t3qai_client-1.1.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      673 b- defN 23-Aug-07 06:43 t3qai_client-1.1.6.dist-info/RECORD
+8 files, 46597 bytes uncompressed, 13921 bytes compressed:  70.1%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: t3qai_client/t3qai_helper.py
 Comment: 
 
 Filename: t3qai_client/t3qai_serving.py
 Comment: 
 
-Filename: t3qai_client-1.1.5.dist-info/LICENSE-2.0.txt
+Filename: t3qai_client-1.1.6.dist-info/LICENSE-2.0.txt
 Comment: 
 
-Filename: t3qai_client-1.1.5.dist-info/METADATA
+Filename: t3qai_client-1.1.6.dist-info/METADATA
 Comment: 
 
-Filename: t3qai_client-1.1.5.dist-info/WHEEL
+Filename: t3qai_client-1.1.6.dist-info/WHEEL
 Comment: 
 
-Filename: t3qai_client-1.1.5.dist-info/top_level.txt
+Filename: t3qai_client-1.1.6.dist-info/top_level.txt
 Comment: 
 
-Filename: t3qai_client-1.1.5.dist-info/RECORD
+Filename: t3qai_client-1.1.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## t3qai_client/t3qai_helper.py

```diff
@@ -549,15 +549,15 @@
     
 def inference_set_logger():
     """
     Inference logger setup
     """
     _log_directory = 'logs'
     _log_filename =  'oper.log'
-    _log_level = 'DEBUG'
+    _log_level = 'INFO'
     
     logger = logging.getLogger()
     # 핸들러 초기화 추가 
     logger.handlers = []
 
     logger_path = inference_load_path().get("logger_path")
```

## Comparing `t3qai_client-1.1.5.dist-info/LICENSE-2.0.txt` & `t3qai_client-1.1.6.dist-info/LICENSE-2.0.txt`

 * *Files identical despite different names*

## Comparing `t3qai_client-1.1.5.dist-info/METADATA` & `t3qai_client-1.1.6.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t3qai-client
-Version: 1.1.5
+Version: 1.1.6
 Summary: t3qai client module
 Home-page: UNKNOWN
 Author: t3q
 Author-email: lab@t3q.com
 License: UNKNOWN
 Keywords: t3q,t3qai,t3qai client,t3qai_client
 Platform: UNKNOWN
```

## Comparing `t3qai_client-1.1.5.dist-info/RECORD` & `t3qai_client-1.1.6.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 t3qai_client/__init__.py,sha256=77s_ELw_PXqJY82x2hWn6OU8CDZCxKdvtN5wsvP7xIY,1639
-t3qai_client/t3qai_helper.py,sha256=jbIhutp9HW-hlE8WKuW7eCm3B_OdO01vs6TNlzejEQI,23381
+t3qai_client/t3qai_helper.py,sha256=MKDbnQfZkegmh0-PPotrhCqFGXGvtyIdOrJev4N10r0,23380
 t3qai_client/t3qai_serving.py,sha256=WCIYgBqIaO0tb9swzwqPufpLMGflGSerFFohqK6RJ8w,6417
-t3qai_client-1.1.5.dist-info/LICENSE-2.0.txt,sha256=thx4yBYMK9EojcuEfGeSPZ4xsnPVNBR8XYMtziBGiWI,11533
-t3qai_client-1.1.5.dist-info/METADATA,sha256=wbsFOwlr3h8Y1RxbJITwQyKYUfYPWBDFL620QlwKNyo,2850
-t3qai_client-1.1.5.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-t3qai_client-1.1.5.dist-info/top_level.txt,sha256=-peQr4CAunIVn62-N5YE4UpLbZJ76mWPDOJGcy36mN8,13
-t3qai_client-1.1.5.dist-info/RECORD,,
+t3qai_client-1.1.6.dist-info/LICENSE-2.0.txt,sha256=thx4yBYMK9EojcuEfGeSPZ4xsnPVNBR8XYMtziBGiWI,11533
+t3qai_client-1.1.6.dist-info/METADATA,sha256=wk-Gnh7BS8w0EdVa8-098ly-GLyEzavGhe8n1yYS2y0,2850
+t3qai_client-1.1.6.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+t3qai_client-1.1.6.dist-info/top_level.txt,sha256=-peQr4CAunIVn62-N5YE4UpLbZJ76mWPDOJGcy36mN8,13
+t3qai_client-1.1.6.dist-info/RECORD,,
```

