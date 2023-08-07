# Comparing `tmp/whisper-live-0.0.4.tar.gz` & `tmp/whisper-live-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whisper-live-0.0.4.tar", last modified: Wed Aug  2 08:12:26 2023, max compression
+gzip compressed data, was "whisper-live-0.0.5.tar", last modified: Mon Aug  7 15:13:33 2023, max compression
```

## Comparing `whisper-live-0.0.4.tar` & `whisper-live-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 vineet    (1000) vineet    (1000)        0 2023-08-02 08:12:26.277721 whisper-live-0.0.4/
--rw-rw-r--   0 vineet    (1000) vineet    (1000)     1085 2023-07-10 09:30:36.000000 whisper-live-0.0.4/LICENSE
--rw-rw-r--   0 vineet    (1000) vineet    (1000)     4306 2023-08-02 08:12:26.277721 whisper-live-0.0.4/PKG-INFO
--rw-rw-r--   0 vineet    (1000) vineet    (1000)     3848 2023-08-02 08:00:41.000000 whisper-live-0.0.4/README.md
--rw-rw-r--   0 vineet    (1000) vineet    (1000)       38 2023-08-02 08:12:26.277721 whisper-live-0.0.4/setup.cfg
--rw-rw-r--   0 vineet    (1000) vineet    (1000)     1316 2023-08-02 08:11:19.000000 whisper-live-0.0.4/setup.py
-drwxrwxr-x   0 vineet    (1000) vineet    (1000)        0 2023-08-02 08:12:26.277721 whisper-live-0.0.4/whisper_live/
--rw-rw-r--   0 vineet    (1000) vineet    (1000)        0 2023-07-31 14:05:43.000000 whisper-live-0.0.4/whisper_live/__init__.py
--rw-rw-r--   0 vineet    (1000) vineet    (1000)     9299 2023-08-02 08:11:53.000000 whisper-live-0.0.4/whisper_live/client.py
--rw-rw-r--   0 vineet    (1000) vineet    (1000)    11926 2023-08-02 08:00:21.000000 whisper-live-0.0.4/whisper_live/server.py
--rw-rw-r--   0 vineet    (1000) vineet    (1000)    32804 2023-07-31 14:00:59.000000 whisper-live-0.0.4/whisper_live/transcriber.py
-drwxrwxr-x   0 vineet    (1000) vineet    (1000)        0 2023-08-02 08:12:26.277721 whisper-live-0.0.4/whisper_live.egg-info/
--rw-rw-r--   0 vineet    (1000) vineet    (1000)     4306 2023-08-02 08:12:26.000000 whisper-live-0.0.4/whisper_live.egg-info/PKG-INFO
--rw-rw-r--   0 vineet    (1000) vineet    (1000)      304 2023-08-02 08:12:26.000000 whisper-live-0.0.4/whisper_live.egg-info/SOURCES.txt
--rw-rw-r--   0 vineet    (1000) vineet    (1000)        1 2023-08-02 08:12:26.000000 whisper-live-0.0.4/whisper_live.egg-info/dependency_links.txt
--rw-rw-r--   0 vineet    (1000) vineet    (1000)      107 2023-08-02 08:12:26.000000 whisper-live-0.0.4/whisper_live.egg-info/requires.txt
--rw-rw-r--   0 vineet    (1000) vineet    (1000)       13 2023-08-02 08:12:26.000000 whisper-live-0.0.4/whisper_live.egg-info/top_level.txt
+drwxrwxr-x   0 vineet    (1000) vineet    (1000)        0 2023-08-07 15:13:33.057587 whisper-live-0.0.5/
+-rw-rw-r--   0 vineet    (1000) vineet    (1000)     1085 2023-07-10 09:30:36.000000 whisper-live-0.0.5/LICENSE
+-rw-rw-r--   0 vineet    (1000) vineet    (1000)     4833 2023-08-07 15:13:33.057587 whisper-live-0.0.5/PKG-INFO
+-rw-rw-r--   0 vineet    (1000) vineet    (1000)     4375 2023-08-07 15:09:14.000000 whisper-live-0.0.5/README.md
+-rw-rw-r--   0 vineet    (1000) vineet    (1000)       38 2023-08-07 15:13:33.057587 whisper-live-0.0.5/setup.cfg
+-rw-rw-r--   0 vineet    (1000) vineet    (1000)     1316 2023-08-07 15:13:22.000000 whisper-live-0.0.5/setup.py
+drwxrwxr-x   0 vineet    (1000) vineet    (1000)        0 2023-08-07 15:13:33.053587 whisper-live-0.0.5/whisper_live/
+-rw-rw-r--   0 vineet    (1000) vineet    (1000)        0 2023-07-31 14:05:43.000000 whisper-live-0.0.5/whisper_live/__init__.py
+-rw-rw-r--   0 vineet    (1000) vineet    (1000)     9299 2023-08-02 08:11:53.000000 whisper-live-0.0.5/whisper_live/client.py
+-rw-rw-r--   0 vineet    (1000) vineet    (1000)    11997 2023-08-07 15:02:53.000000 whisper-live-0.0.5/whisper_live/server.py
+-rw-rw-r--   0 vineet    (1000) vineet    (1000)    32804 2023-07-31 14:00:59.000000 whisper-live-0.0.5/whisper_live/transcriber.py
+drwxrwxr-x   0 vineet    (1000) vineet    (1000)        0 2023-08-07 15:13:33.057587 whisper-live-0.0.5/whisper_live.egg-info/
+-rw-rw-r--   0 vineet    (1000) vineet    (1000)     4833 2023-08-07 15:13:33.000000 whisper-live-0.0.5/whisper_live.egg-info/PKG-INFO
+-rw-rw-r--   0 vineet    (1000) vineet    (1000)      304 2023-08-07 15:13:33.000000 whisper-live-0.0.5/whisper_live.egg-info/SOURCES.txt
+-rw-rw-r--   0 vineet    (1000) vineet    (1000)        1 2023-08-07 15:13:33.000000 whisper-live-0.0.5/whisper_live.egg-info/dependency_links.txt
+-rw-rw-r--   0 vineet    (1000) vineet    (1000)      107 2023-08-07 15:13:33.000000 whisper-live-0.0.5/whisper_live.egg-info/requires.txt
+-rw-rw-r--   0 vineet    (1000) vineet    (1000)       13 2023-08-07 15:13:33.000000 whisper-live-0.0.5/whisper_live.egg-info/top_level.txt
```

### Comparing `whisper-live-0.0.4/LICENSE` & `whisper-live-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `whisper-live-0.0.4/PKG-INFO` & `whisper-live-0.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whisper-live
-Version: 0.0.4
+Version: 0.0.5
 Summary: A nearly-live implementation of OpenAI's Whisper.
 Home-page: https://github.com/collabora/WhisperLive
 Author: Collabora Ltd
 Author-email: vineet.suryan@collabora.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
@@ -68,28 +68,35 @@
 ### Chrome Extension
 - Refer to [Audio-Transcription-Chrome](https://github.com/collabora/whisper-live/tree/main/Audio-Transcription-Chrome#readme) to use Chrome extension.
 
 ### Firefox Extension
 - Refer to [Audio-Transcription-Firefox](https://github.com/collabora/whisper-live/tree/main/Audio-Transcription-Firefox#readme) to use Mozilla Firefox extension.
 
 ## Whisper Live Server in Docker
-- Build docker container
+- GPU
 ```bash
- docker build . -t whisper-live
+ docker build . -t whisper-live -f docker/Dockerfile.gpu
+ docker run -it --gpus all -p 9090:9090 whisper-live:latest
 ```
 
-- Run docker container
+- CPU
 ```bash
- docker run -it --gpus all -p 9090:9090 whisper-live:latest
+ docker build . -t whisper-live -f docker/Dockerfile.cpu
+ docker run -it -p 9090:9090 whisper-live:latest
 ```
+**Note**: By default we use "small" model size. To build docker image for a different model size, change the size in server.py and then build the docker image.
 
 ## Future Work
 - [ ] Add translation to other languages on top of transcription.
 - [ ] TensorRT backend for Whisper.
 
+## Contact
+
+We are available to help you with both Open Source and proprietary AI projects. You can reach us via the Collabora website or [vineet.suryan@collabora.com](mailto:vineet.suryan@collabora.com) and [marcus.edel@collabora.com](mailto:marcus.edel@collabora.com).
+
 ## Citations
 ```bibtex
 @article{Whisper
   title = {Robust Speech Recognition via Large-Scale Weak Supervision},
   url = {https://arxiv.org/abs/2212.04356},
   author = {Radford, Alec and Kim, Jong Wook and Xu, Tao and Brockman, Greg and McLeavey, Christine and Sutskever, Ilya},
   publisher = {arXiv},
```

### Comparing `whisper-live-0.0.4/README.md` & `whisper-live-0.0.5/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -54,28 +54,35 @@
 ### Chrome Extension
 - Refer to [Audio-Transcription-Chrome](https://github.com/collabora/whisper-live/tree/main/Audio-Transcription-Chrome#readme) to use Chrome extension.
 
 ### Firefox Extension
 - Refer to [Audio-Transcription-Firefox](https://github.com/collabora/whisper-live/tree/main/Audio-Transcription-Firefox#readme) to use Mozilla Firefox extension.
 
 ## Whisper Live Server in Docker
-- Build docker container
+- GPU
 ```bash
- docker build . -t whisper-live
+ docker build . -t whisper-live -f docker/Dockerfile.gpu
+ docker run -it --gpus all -p 9090:9090 whisper-live:latest
 ```
 
-- Run docker container
+- CPU
 ```bash
- docker run -it --gpus all -p 9090:9090 whisper-live:latest
+ docker build . -t whisper-live -f docker/Dockerfile.cpu
+ docker run -it -p 9090:9090 whisper-live:latest
 ```
+**Note**: By default we use "small" model size. To build docker image for a different model size, change the size in server.py and then build the docker image.
 
 ## Future Work
 - [ ] Add translation to other languages on top of transcription.
 - [ ] TensorRT backend for Whisper.
 
+## Contact
+
+We are available to help you with both Open Source and proprietary AI projects. You can reach us via the Collabora website or [vineet.suryan@collabora.com](mailto:vineet.suryan@collabora.com) and [marcus.edel@collabora.com](mailto:marcus.edel@collabora.com).
+
 ## Citations
 ```bibtex
 @article{Whisper
   title = {Robust Speech Recognition via Large-Scale Weak Supervision},
   url = {https://arxiv.org/abs/2212.04356},
   author = {Radford, Alec and Kim, Jong Wook and Xu, Tao and Brockman, Greg and McLeavey, Christine and Sutskever, Ilya},
   publisher = {arXiv},
```

### Comparing `whisper-live-0.0.4/setup.py` & `whisper-live-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(name="whisper-live",
-      version="0.0.4",
+      version="0.0.5",
       description="A nearly-live implementation of OpenAI's Whisper.",
       long_description=README,
       long_description_content_type="text/markdown",
       include_package_data=True,
       url="https://github.com/collabora/WhisperLive",
       author="Collabora Ltd",
       author_email="vineet.suryan@collabora.com",
```

### Comparing `whisper-live-0.0.4/whisper_live/client.py` & `whisper-live-0.0.5/whisper_live/client.py`

 * *Files identical despite different names*

### Comparing `whisper-live-0.0.4/whisper_live/server.py` & `whisper-live-0.0.5/whisper_live/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,18 +75,19 @@
     SERVER_READY = "SERVER_READY"
 
     def __init__(self, websocket, task="transcribe", device=None, multilingual=False, language=None):
         self.data = b""
         self.frames = b""
         self.language = language if multilingual else "en"
         self.task = task
+        device = "cuda" if torch.cuda.is_available() else "cpu"
         self.transcriber = WhisperModel(
             "small" if multilingual else "small.en", 
-            device=device if device else "cuda",
-            compute_type="float16", 
+            device=device,
+            compute_type="int8" if device=="cpu" else "float16", 
             local_files_only=False,
         )
         
         # voice activity detection model
         self.vad_model, _ = torch.hub.load(repo_or_dir='snakers4/silero-vad',
                                            model='silero_vad',
                                            force_reload=True,
```

### Comparing `whisper-live-0.0.4/whisper_live/transcriber.py` & `whisper-live-0.0.5/whisper_live/transcriber.py`

 * *Files identical despite different names*

### Comparing `whisper-live-0.0.4/whisper_live.egg-info/PKG-INFO` & `whisper-live-0.0.5/whisper_live.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whisper-live
-Version: 0.0.4
+Version: 0.0.5
 Summary: A nearly-live implementation of OpenAI's Whisper.
 Home-page: https://github.com/collabora/WhisperLive
 Author: Collabora Ltd
 Author-email: vineet.suryan@collabora.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
@@ -68,28 +68,35 @@
 ### Chrome Extension
 - Refer to [Audio-Transcription-Chrome](https://github.com/collabora/whisper-live/tree/main/Audio-Transcription-Chrome#readme) to use Chrome extension.
 
 ### Firefox Extension
 - Refer to [Audio-Transcription-Firefox](https://github.com/collabora/whisper-live/tree/main/Audio-Transcription-Firefox#readme) to use Mozilla Firefox extension.
 
 ## Whisper Live Server in Docker
-- Build docker container
+- GPU
 ```bash
- docker build . -t whisper-live
+ docker build . -t whisper-live -f docker/Dockerfile.gpu
+ docker run -it --gpus all -p 9090:9090 whisper-live:latest
 ```
 
-- Run docker container
+- CPU
 ```bash
- docker run -it --gpus all -p 9090:9090 whisper-live:latest
+ docker build . -t whisper-live -f docker/Dockerfile.cpu
+ docker run -it -p 9090:9090 whisper-live:latest
 ```
+**Note**: By default we use "small" model size. To build docker image for a different model size, change the size in server.py and then build the docker image.
 
 ## Future Work
 - [ ] Add translation to other languages on top of transcription.
 - [ ] TensorRT backend for Whisper.
 
+## Contact
+
+We are available to help you with both Open Source and proprietary AI projects. You can reach us via the Collabora website or [vineet.suryan@collabora.com](mailto:vineet.suryan@collabora.com) and [marcus.edel@collabora.com](mailto:marcus.edel@collabora.com).
+
 ## Citations
 ```bibtex
 @article{Whisper
   title = {Robust Speech Recognition via Large-Scale Weak Supervision},
   url = {https://arxiv.org/abs/2212.04356},
   author = {Radford, Alec and Kim, Jong Wook and Xu, Tao and Brockman, Greg and McLeavey, Christine and Sutskever, Ilya},
   publisher = {arXiv},
```

