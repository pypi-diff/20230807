# Comparing `tmp/omniinfer_client-0.1.0.tar.gz` & `tmp/omniinfer_client-0.2.0.tar.gz`

## Comparing `omniinfer_client-0.1.0.tar` & `omniinfer_client-0.2.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 omniinfer_client-0.1.0/.python-version
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 omniinfer_client-0.1.0/Makefile
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 omniinfer_client-0.1.0/requirements-dev.lock
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 omniinfer_client-0.1.0/requirements.lock
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 omniinfer_client-0.1.0/docs/Makefile
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 omniinfer_client-0.1.0/docs/conf.py
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 omniinfer_client-0.1.0/docs/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 omniinfer_client-0.1.0/docs/make.bat
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 omniinfer_client-0.1.0/docs/modules.rst
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 omniinfer_client-0.1.0/docs/omniinfer_client.rst
--rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 omniinfer_client-0.1.0/examples/controlnet_qrcode.py
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 omniinfer_client-0.1.0/examples/model_search.py
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 omniinfer_client-0.1.0/examples/txt2img_with_lora.py
--rw-r--r--   0        0        0     2516 2020-02-02 00:00:00.000000 omniinfer_client-0.1.0/examples/fixtures/qrcode.png
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 omniinfer_client-0.1.0/src/omniinfer_client/__init__.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 omniinfer_client-0.1.0/src/omniinfer_client/exceptions.py
--rw-r--r--   0        0        0     7135 2020-02-02 00:00:00.000000 omniinfer_client-0.1.0/src/omniinfer_client/omni.py
--rw-r--r--   0        0        0    12078 2020-02-02 00:00:00.000000 omniinfer_client-0.1.0/src/omniinfer_client/proto.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 omniinfer_client-0.1.0/src/omniinfer_client/serializer.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 omniinfer_client-0.1.0/src/omniinfer_client/settings.py
--rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 omniinfer_client-0.1.0/src/omniinfer_client/utils.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 omniinfer_client-0.1.0/src/omniinfer_client/version.py
--rw-r--r--   0        0        0     4152 2020-02-02 00:00:00.000000 omniinfer_client-0.1.0/tests/test_basics.py
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 omniinfer_client-0.1.0/tests/test_model.py
--rw-r--r--   0        0        0     3088 2020-02-02 00:00:00.000000 omniinfer_client-0.1.0/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 omniinfer_client-0.1.0/LICENSE
--rw-r--r--   0        0        0     4537 2020-02-02 00:00:00.000000 omniinfer_client-0.1.0/README.md
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 omniinfer_client-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     6215 2020-02-02 00:00:00.000000 omniinfer_client-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 omniinfer_client-0.2.0/.python-version
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 omniinfer_client-0.2.0/Makefile
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 omniinfer_client-0.2.0/requirements-dev.lock
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 omniinfer_client-0.2.0/requirements.lock
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 omniinfer_client-0.2.0/docs/Makefile
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 omniinfer_client-0.2.0/docs/conf.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 omniinfer_client-0.2.0/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 omniinfer_client-0.2.0/docs/make.bat
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 omniinfer_client-0.2.0/docs/modules.rst
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 omniinfer_client-0.2.0/docs/omniinfer_client.rst
+-rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 omniinfer_client-0.2.0/examples/controlnet_qrcode.py
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 omniinfer_client-0.2.0/examples/model_search.py
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 omniinfer_client-0.2.0/examples/txt2img_with_lora.py
+-rw-r--r--   0        0        0     2516 2020-02-02 00:00:00.000000 omniinfer_client-0.2.0/examples/fixtures/qrcode.png
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 omniinfer_client-0.2.0/src/omniinfer_client/__init__.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 omniinfer_client-0.2.0/src/omniinfer_client/exceptions.py
+-rw-r--r--   0        0        0     7135 2020-02-02 00:00:00.000000 omniinfer_client-0.2.0/src/omniinfer_client/omni.py
+-rw-r--r--   0        0        0    12616 2020-02-02 00:00:00.000000 omniinfer_client-0.2.0/src/omniinfer_client/proto.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 omniinfer_client-0.2.0/src/omniinfer_client/serializer.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 omniinfer_client-0.2.0/src/omniinfer_client/settings.py
+-rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 omniinfer_client-0.2.0/src/omniinfer_client/utils.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 omniinfer_client-0.2.0/src/omniinfer_client/version.py
+-rw-r--r--   0        0        0     4152 2020-02-02 00:00:00.000000 omniinfer_client-0.2.0/tests/test_basics.py
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 omniinfer_client-0.2.0/tests/test_model.py
+-rw-r--r--   0        0        0     3088 2020-02-02 00:00:00.000000 omniinfer_client-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 omniinfer_client-0.2.0/LICENSE
+-rw-r--r--   0        0        0     4537 2020-02-02 00:00:00.000000 omniinfer_client-0.2.0/README.md
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 omniinfer_client-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6334 2020-02-02 00:00:00.000000 omniinfer_client-0.2.0/PKG-INFO
```

### Comparing `omniinfer_client-0.1.0/requirements-dev.lock` & `omniinfer_client-0.2.0/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `omniinfer_client-0.1.0/docs/Makefile` & `omniinfer_client-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `omniinfer_client-0.1.0/docs/conf.py` & `omniinfer_client-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `omniinfer_client-0.1.0/docs/make.bat` & `omniinfer_client-0.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `omniinfer_client-0.1.0/docs/omniinfer_client.rst` & `omniinfer_client-0.2.0/docs/omniinfer_client.rst`

 * *Files identical despite different names*

### Comparing `omniinfer_client-0.1.0/examples/controlnet_qrcode.py` & `omniinfer_client-0.2.0/examples/controlnet_qrcode.py`

 * *Files identical despite different names*

### Comparing `omniinfer_client-0.1.0/examples/model_search.py` & `omniinfer_client-0.2.0/examples/model_search.py`

 * *Files identical despite different names*

### Comparing `omniinfer_client-0.1.0/examples/txt2img_with_lora.py` & `omniinfer_client-0.2.0/examples/txt2img_with_lora.py`

 * *Files identical despite different names*

### Comparing `omniinfer_client-0.1.0/examples/fixtures/qrcode.png` & `omniinfer_client-0.2.0/examples/fixtures/qrcode.png`

 * *Files identical despite different names*

### Comparing `omniinfer_client-0.1.0/src/omniinfer_client/omni.py` & `omniinfer_client-0.2.0/src/omniinfer_client/omni.py`

 * *Files identical despite different names*

### Comparing `omniinfer_client-0.1.0/src/omniinfer_client/proto.py` & `omniinfer_client-0.2.0/src/omniinfer_client/proto.py`

 * *Files 6% similar despite different names*

```diff
@@ -150,14 +150,20 @@
     INVALID_AUTH = 4
     HOST_UNAVAILABLE = 5
     PARAM_RANGE_ERROR = 6
     COST_BALANCE_ERROR = 7
     SAMPLER_NOT_EXISTS = 8
     TIMEOUT = 9
 
+    UNKNOWN = 100
+
+    @classmethod
+    def _missing_(cls, number):
+        return cls(cls.UNKNOWN)
+
 
 @dataclass
 class Txt2ImgResponseData(JSONe):
     task_id: str
     warn: Optional[str] = None
 
 
@@ -209,14 +215,20 @@
     INVALID_AUTH = 4
     HOST_UNAVAILABLE = 5
     PARAM_RANGE_ERROR = 6
     COST_BALANCE_ERROR = 7
     SAMPLER_NOT_EXISTS = 8
     TIMEOUT = 9
 
+    UNKNOWN = 100
+
+    @classmethod
+    def _missing_(cls, number):
+        return cls(cls.UNKNOWN)
+
 
 @dataclass
 class Img2ImgResponseData(JSONe):
     task_id: str
     warn: Optional[str] = None
 
 
@@ -232,14 +244,20 @@
 class ProgressResponseStatusCode(Enum):
     INITIALIZING = 0
     RUNNING = 1
     SUCCESSFUL = 2
     FAILED = 3
     TIMEOUT = 4
 
+    UNKNOWN = 100
+
+    @classmethod
+    def _missing_(cls, number):
+        return cls(cls.UNKNOWN)
+
     def finished(self):
         return self in (ProgressResponseStatusCode.SUCCESSFUL, ProgressResponseStatusCode.FAILED, ProgressResponseStatusCode.TIMEOUT)
 
 
 @dataclass
 class ProgressData(JSONe):
     status: ProgressResponseStatusCode
@@ -265,34 +283,48 @@
     INVALID_AUTH = 4
     HOST_UNAVAILABLE = 5
     PARAM_RANGE_ERROR = 6
     COST_BALANCE_ERROR = 7
     SAMPLER_NOT_EXISTS = 8
     TIMEOUT = 9
 
+    UNKNOWN = 100
+
+    @classmethod
+    def _missing_(cls, number):
+        return cls(cls.UNKNOWN)
+
 
 @dataclass
 class ProgressResponse(JSONe):
     code: ProgressResponseCode
     data: ProgressData
     msg: Optional[str] = ""
 
     def download_images(self):
         if self.data.imgs is not None and len(self.data.imgs) > 0:
             self.data.imgs_bytes = batch_download_images(self.data.imgs)
 
 
 # --------------- Model ---------------
 
+
 class ModelType(Enum):
     CHECKPOINT = "checkpoint"
     LORA = "lora"
     VAE = "vae"
     CONTROLNET = "controlnet"
     TEXT_INVERSION = "textualinversion"
+    UPSCALER = "upscaler"
+
+    UNKNOWN = "unknown"
+
+    @classmethod
+    def _missing_(cls, number):
+        return cls(cls.UNKNOWN)
 
 
 @dataclass
 class CivitaiImageMeta(JSONe):
     prompt: Optional[str] = None
     negative_prompt: Optional[str] = None
     sampler_name: Optional[str] = None
```

### Comparing `omniinfer_client-0.1.0/src/omniinfer_client/utils.py` & `omniinfer_client-0.2.0/src/omniinfer_client/utils.py`

 * *Files identical despite different names*

### Comparing `omniinfer_client-0.1.0/tests/test_basics.py` & `omniinfer_client-0.2.0/tests/test_basics.py`

 * *Files identical despite different names*

### Comparing `omniinfer_client-0.1.0/tests/test_model.py` & `omniinfer_client-0.2.0/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `omniinfer_client-0.1.0/.gitignore` & `omniinfer_client-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `omniinfer_client-0.1.0/LICENSE` & `omniinfer_client-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `omniinfer_client-0.1.0/README.md` & `omniinfer_client-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `omniinfer_client-0.1.0/PKG-INFO` & `omniinfer_client-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 Metadata-Version: 2.1
 Name: omniinfer_client
-Version: 0.1.0
+Version: 0.2.0
 Summary: Omniinfer SDK for Python
+Project-URL: Homepage, https://github.com/omniinfer/python-sdk
+Project-URL: Bug Tracker, https://discord.gg/nzqq8UScpx
 Author-email: Omniinfer <omniinfer@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 omniinfer.io
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

