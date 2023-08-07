# Comparing `tmp/t3qai_client-1.1.4-py3-none-any.whl.zip` & `tmp/t3qai_client-1.1.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 15017 bytes, number of entries: 8
+Zip file size: 15090 bytes, number of entries: 8
 -rw-rw-rw-  2.0 fat     1639 b- defN 23-Aug-03 08:00 t3qai_client/__init__.py
--rw-rw-rw-  2.0 fat    23318 b- defN 23-Aug-04 08:20 t3qai_client/t3qai_helper.py
--rw-rw-rw-  2.0 fat     6328 b- defN 23-Aug-03 08:00 t3qai_client/t3qai_serving.py
--rw-rw-rw-  2.0 fat    11533 b- defN 23-Aug-04 08:20 t3qai_client-1.1.4.dist-info/LICENSE-2.0.txt
--rw-rw-rw-  2.0 fat     2850 b- defN 23-Aug-04 08:20 t3qai_client-1.1.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-04 08:20 t3qai_client-1.1.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       13 b- defN 23-Aug-04 08:20 t3qai_client-1.1.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      673 b- defN 23-Aug-04 08:20 t3qai_client-1.1.4.dist-info/RECORD
-8 files, 46446 bytes uncompressed, 13841 bytes compressed:  70.2%
+-rw-rw-rw-  2.0 fat    23381 b- defN 23-Aug-07 05:58 t3qai_client/t3qai_helper.py
+-rw-rw-rw-  2.0 fat     6417 b- defN 23-Aug-07 06:00 t3qai_client/t3qai_serving.py
+-rw-rw-rw-  2.0 fat    11533 b- defN 23-Aug-07 06:02 t3qai_client-1.1.5.dist-info/LICENSE-2.0.txt
+-rw-rw-rw-  2.0 fat     2850 b- defN 23-Aug-07 06:02 t3qai_client-1.1.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-07 06:02 t3qai_client-1.1.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       13 b- defN 23-Aug-07 06:02 t3qai_client-1.1.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      673 b- defN 23-Aug-07 06:02 t3qai_client-1.1.5.dist-info/RECORD
+8 files, 46598 bytes uncompressed, 13914 bytes compressed:  70.1%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: t3qai_client/t3qai_helper.py
 Comment: 
 
 Filename: t3qai_client/t3qai_serving.py
 Comment: 
 
-Filename: t3qai_client-1.1.4.dist-info/LICENSE-2.0.txt
+Filename: t3qai_client-1.1.5.dist-info/LICENSE-2.0.txt
 Comment: 
 
-Filename: t3qai_client-1.1.4.dist-info/METADATA
+Filename: t3qai_client-1.1.5.dist-info/METADATA
 Comment: 
 
-Filename: t3qai_client-1.1.4.dist-info/WHEEL
+Filename: t3qai_client-1.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: t3qai_client-1.1.4.dist-info/top_level.txt
+Filename: t3qai_client-1.1.5.dist-info/top_level.txt
 Comment: 
 
-Filename: t3qai_client-1.1.4.dist-info/RECORD
+Filename: t3qai_client-1.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## t3qai_client/t3qai_helper.py

```diff
@@ -552,14 +552,17 @@
     Inference logger setup
     """
     _log_directory = 'logs'
     _log_filename =  'oper.log'
     _log_level = 'DEBUG'
     
     logger = logging.getLogger()
+    # 핸들러 초기화 추가 
+    logger.handlers = []
+
     logger_path = inference_load_path().get("logger_path")
     
     pathlib.Path(logger_path).mkdir(parents=True, exist_ok=True)
     
     if logger_path and os.path.exists(logger_path):
         log_file_path = os.path.join(logger_path, _log_filename)
         if os.path.exists(log_file_path):
```

## t3qai_client/t3qai_serving.py

```diff
@@ -30,20 +30,24 @@
 from datetime import datetime
 from pydantic import BaseModel
 from typing import Optional, List, Any
 from fastapi import FastAPI, File, UploadFile, Request, Response
 from fastapi.responses import StreamingResponse, PlainTextResponse
 
 from t3qai_client.t3qai_helper import DownloadFile as DownloadFile
+from t3qai_client.t3qai_helper import inference_set_logger
 
 SERVING_PARAMS_FILE = "serving_params.json"
 POD_VOLUME_PATH = "/cache"
 
+inference_set_logger() 
+
 app = FastAPI()
 @app.post("/inference")
+
 async def inference(request: Request):
     """
     Receive json and proceed with inference
     
     Parameters
     ----------
     json data from request body
```

## Comparing `t3qai_client-1.1.4.dist-info/LICENSE-2.0.txt` & `t3qai_client-1.1.5.dist-info/LICENSE-2.0.txt`

 * *Files identical despite different names*

## Comparing `t3qai_client-1.1.4.dist-info/METADATA` & `t3qai_client-1.1.5.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t3qai-client
-Version: 1.1.4
+Version: 1.1.5
 Summary: t3qai client module
 Home-page: UNKNOWN
 Author: t3q
 Author-email: lab@t3q.com
 License: UNKNOWN
 Keywords: t3q,t3qai,t3qai client,t3qai_client
 Platform: UNKNOWN
```

## Comparing `t3qai_client-1.1.4.dist-info/RECORD` & `t3qai_client-1.1.5.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 t3qai_client/__init__.py,sha256=77s_ELw_PXqJY82x2hWn6OU8CDZCxKdvtN5wsvP7xIY,1639
-t3qai_client/t3qai_helper.py,sha256=TnMY0OVstMozVyv-E_4tP3xpjE6yRyqtswB2EcPrQmQ,23318
-t3qai_client/t3qai_serving.py,sha256=aadhlm4Di0gU9s5ZsA3Xch1SjI7wvxNh1ygYOoYty84,6328
-t3qai_client-1.1.4.dist-info/LICENSE-2.0.txt,sha256=thx4yBYMK9EojcuEfGeSPZ4xsnPVNBR8XYMtziBGiWI,11533
-t3qai_client-1.1.4.dist-info/METADATA,sha256=QJEMar7YxZGBbDPcyWwN34_5uSLgMCKPUBhwcwwMmwM,2850
-t3qai_client-1.1.4.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-t3qai_client-1.1.4.dist-info/top_level.txt,sha256=-peQr4CAunIVn62-N5YE4UpLbZJ76mWPDOJGcy36mN8,13
-t3qai_client-1.1.4.dist-info/RECORD,,
+t3qai_client/t3qai_helper.py,sha256=jbIhutp9HW-hlE8WKuW7eCm3B_OdO01vs6TNlzejEQI,23381
+t3qai_client/t3qai_serving.py,sha256=WCIYgBqIaO0tb9swzwqPufpLMGflGSerFFohqK6RJ8w,6417
+t3qai_client-1.1.5.dist-info/LICENSE-2.0.txt,sha256=thx4yBYMK9EojcuEfGeSPZ4xsnPVNBR8XYMtziBGiWI,11533
+t3qai_client-1.1.5.dist-info/METADATA,sha256=wbsFOwlr3h8Y1RxbJITwQyKYUfYPWBDFL620QlwKNyo,2850
+t3qai_client-1.1.5.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+t3qai_client-1.1.5.dist-info/top_level.txt,sha256=-peQr4CAunIVn62-N5YE4UpLbZJ76mWPDOJGcy36mN8,13
+t3qai_client-1.1.5.dist-info/RECORD,,
```

