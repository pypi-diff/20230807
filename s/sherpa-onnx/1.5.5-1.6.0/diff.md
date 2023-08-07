# Comparing `tmp/sherpa-onnx-1.5.5.tar.gz` & `tmp/sherpa-onnx-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sherpa-onnx-1.5.5.tar", last modified: Tue Aug  1 06:34:20 2023, max compression
+gzip compressed data, was "sherpa-onnx-1.6.0.tar", last modified: Mon Aug  7 05:09:29 2023, max compression
```

## Comparing `sherpa-onnx-1.5.5.tar` & `sherpa-onnx-1.6.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:34:20.713956 sherpa-onnx-1.5.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-08-01 06:22:12.000000 sherpa-onnx-1.5.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-08-01 06:34:20.713956 sherpa-onnx-1.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-08-01 06:22:12.000000 sherpa-onnx-1.5.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 06:34:20.713956 sherpa-onnx-1.5.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-08-01 06:22:12.000000 sherpa-onnx-1.5.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:34:20.709956 sherpa-onnx-1.5.5/sherpa-onnx/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:34:20.709956 sherpa-onnx-1.5.5/sherpa-onnx/python/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:34:20.713956 sherpa-onnx-1.5.5/sherpa-onnx/python/sherpa_onnx/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-08-01 06:34:20.000000 sherpa-onnx-1.5.5/sherpa-onnx/python/sherpa_onnx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7583 2023-08-01 06:22:12.000000 sherpa-onnx-1.5.5/sherpa-onnx/python/sherpa_onnx/offline_recognizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5988 2023-08-01 06:22:12.000000 sherpa-onnx-1.5.5/sherpa-onnx/python/sherpa_onnx/online_recognizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-08-01 06:22:12.000000 sherpa-onnx-1.5.5/sherpa-onnx/python/sherpa_onnx/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:34:20.713956 sherpa-onnx-1.5.5/sherpa_onnx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-08-01 06:34:20.000000 sherpa-onnx-1.5.5/sherpa_onnx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-08-01 06:34:20.000000 sherpa-onnx-1.5.5/sherpa_onnx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 06:34:20.000000 sherpa-onnx-1.5.5/sherpa_onnx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 06:34:20.000000 sherpa-onnx-1.5.5/sherpa_onnx.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-01 06:34:20.000000 sherpa-onnx-1.5.5/sherpa_onnx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-01 06:34:20.000000 sherpa-onnx-1.5.5/sherpa_onnx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 05:09:29.709365 sherpa-onnx-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-08-07 04:56:02.000000 sherpa-onnx-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-08-07 05:09:29.709365 sherpa-onnx-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-08-07 04:56:02.000000 sherpa-onnx-1.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 05:09:29.709365 sherpa-onnx-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-08-07 04:56:02.000000 sherpa-onnx-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 05:09:29.709365 sherpa-onnx-1.6.0/sherpa-onnx/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 05:09:29.709365 sherpa-onnx-1.6.0/sherpa-onnx/python/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 05:09:29.709365 sherpa-onnx-1.6.0/sherpa-onnx/python/sherpa_onnx/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-08-07 05:09:29.000000 sherpa-onnx-1.6.0/sherpa-onnx/python/sherpa_onnx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9624 2023-08-07 04:56:02.000000 sherpa-onnx-1.6.0/sherpa-onnx/python/sherpa_onnx/offline_recognizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5988 2023-08-07 04:56:02.000000 sherpa-onnx-1.6.0/sherpa-onnx/python/sherpa_onnx/online_recognizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-08-07 04:56:02.000000 sherpa-onnx-1.6.0/sherpa-onnx/python/sherpa_onnx/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 05:09:29.709365 sherpa-onnx-1.6.0/sherpa_onnx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-08-07 05:09:29.000000 sherpa-onnx-1.6.0/sherpa_onnx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-08-07 05:09:29.000000 sherpa-onnx-1.6.0/sherpa_onnx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 05:09:29.000000 sherpa-onnx-1.6.0/sherpa_onnx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 05:09:29.000000 sherpa-onnx-1.6.0/sherpa_onnx.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-07 05:09:29.000000 sherpa-onnx-1.6.0/sherpa_onnx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-07 05:09:29.000000 sherpa-onnx-1.6.0/sherpa_onnx.egg-info/top_level.txt
```

### Comparing `sherpa-onnx-1.5.5/LICENSE` & `sherpa-onnx-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.5.5/PKG-INFO` & `sherpa-onnx-1.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sherpa-onnx
-Version: 1.5.5
+Version: 1.6.0
 Summary: UNKNOWN
 Home-page: https://github.com/k2-fsa/sherpa-onnx
 Author: The sherpa-onnx development team
 Author-email: dpovey@gmail.com
 License: Apache licensed, as found in the LICENSE file
 Platform: UNKNOWN
 Classifier: Programming Language :: C++
```

### Comparing `sherpa-onnx-1.5.5/setup.py` & `sherpa-onnx-1.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.5.5/sherpa-onnx/python/sherpa_onnx/offline_recognizer.py` & `sherpa-onnx-1.6.0/sherpa-onnx/python/sherpa_onnx/offline_recognizer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 # Copyright (c)  2023 by manyeyes
+# Copyright (c)  2023  Xiaomi Corporation
 from pathlib import Path
 from typing import List, Optional
 
 from _sherpa_onnx import (
     OfflineFeatureExtractorConfig,
     OfflineModelConfig,
     OfflineNemoEncDecCtcModelConfig,
     OfflineParaformerModelConfig,
+    OfflineWhisperModelConfig,
 )
 from _sherpa_onnx import OfflineRecognizer as _Recognizer
 from _sherpa_onnx import (
     OfflineRecognizerConfig,
     OfflineStream,
     OfflineTransducerModelConfig,
 )
@@ -65,15 +67,15 @@
           num_threads:
             Number of threads for neural network computation.
           sample_rate:
             Sample rate of the training data used to train the model.
           feature_dim:
             Dimension of the feature used to train the model.
           decoding_method:
-            Support only greedy_search for now.
+            Valid values: greedy_search, modified_beam_search.
           debug:
             True to show debug messages.
           provider:
             onnxruntime execution providers. Valid values are: cpu, cuda, coreml.
         """
         self = cls.__new__(cls)
         model_config = OfflineModelConfig(
@@ -133,15 +135,15 @@
           num_threads:
             Number of threads for neural network computation.
           sample_rate:
             Sample rate of the training data used to train the model.
           feature_dim:
             Dimension of the feature used to train the model.
           decoding_method:
-            Valid values are greedy_search, modified_beam_search.
+            Valid values are greedy_search.
           debug:
             True to show debug messages.
           provider:
             onnxruntime execution providers. Valid values are: cpu, cuda, coreml.
         """
         self = cls.__new__(cls)
         model_config = OfflineModelConfig(
@@ -181,30 +183,30 @@
         """
         Please refer to
         `<https://k2-fsa.github.io/sherpa/onnx/pretrained_models/index.html>`_
         to download pre-trained models for different languages, e.g., Chinese,
         English, etc.
 
         Args:
+          model:
+            Path to ``model.onnx``.
           tokens:
             Path to ``tokens.txt``. Each line in ``tokens.txt`` contains two
             columns::
 
                 symbol integer_id
 
-          model:
-            Path to ``model.onnx``.
           num_threads:
             Number of threads for neural network computation.
           sample_rate:
             Sample rate of the training data used to train the model.
           feature_dim:
             Dimension of the feature used to train the model.
           decoding_method:
-            Valid values are greedy_search, modified_beam_search.
+            Valid values are greedy_search.
           debug:
             True to show debug messages.
           provider:
             onnxruntime execution providers. Valid values are: cpu, cuda, coreml.
         """
         self = cls.__new__(cls)
         model_config = OfflineModelConfig(
@@ -222,14 +224,76 @@
         )
 
         recognizer_config = OfflineRecognizerConfig(
             feat_config=feat_config,
             model_config=model_config,
             decoding_method=decoding_method,
         )
+        self.recognizer = _Recognizer(recognizer_config)
+        return self
+
+    @classmethod
+    def from_whisper(
+        cls,
+        encoder: str,
+        decoder: str,
+        tokens: str,
+        num_threads: int,
+        decoding_method: str = "greedy_search",
+        debug: bool = False,
+        provider: str = "cpu",
+    ):
+        """
+        Please refer to
+        `<https://k2-fsa.github.io/sherpa/onnx/pretrained_models/index.html>`_
+        to download pre-trained models for different kinds of whisper models,
+        e.g., tiny, tiny.en, base, base.en, etc.
+
+        Args:
+          encoder_model:
+            Path to the encoder model, e.g., tiny-encoder.onnx,
+            tiny-encoder.int8.onnx, tiny-encoder.ort, etc.
+          decoder_model:
+            Path to the encoder model, e.g., tiny-encoder.onnx,
+            tiny-encoder.int8.onnx, tiny-encoder.ort, etc.
+          tokens:
+            Path to ``tokens.txt``. Each line in ``tokens.txt`` contains two
+            columns::
+
+                symbol integer_id
+
+          num_threads:
+            Number of threads for neural network computation.
+          decoding_method:
+            Valid values: greedy_search.
+          debug:
+            True to show debug messages.
+          provider:
+            onnxruntime execution providers. Valid values are: cpu, cuda, coreml.
+        """
+        self = cls.__new__(cls)
+        model_config = OfflineModelConfig(
+            whisper=OfflineWhisperModelConfig(encoder=encoder, decoder=decoder),
+            tokens=tokens,
+            num_threads=num_threads,
+            debug=debug,
+            provider=provider,
+            model_type="whisper",
+        )
+
+        feat_config = OfflineFeatureExtractorConfig(
+            sampling_rate=16000,
+            feature_dim=80,
+        )
+
+        recognizer_config = OfflineRecognizerConfig(
+            feat_config=feat_config,
+            model_config=model_config,
+            decoding_method=decoding_method,
+        )
         self.recognizer = _Recognizer(recognizer_config)
         return self
 
     def create_stream(self, contexts_list: Optional[List[List[int]]] = None):
         if contexts_list is None:
             return self.recognizer.create_stream()
         else:
```

### Comparing `sherpa-onnx-1.5.5/sherpa-onnx/python/sherpa_onnx/online_recognizer.py` & `sherpa-onnx-1.6.0/sherpa-onnx/python/sherpa_onnx/online_recognizer.py`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.5.5/sherpa-onnx/python/sherpa_onnx/utils.py` & `sherpa-onnx-1.6.0/sherpa-onnx/python/sherpa_onnx/utils.py`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.5.5/sherpa_onnx.egg-info/PKG-INFO` & `sherpa-onnx-1.6.0/sherpa_onnx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sherpa-onnx
-Version: 1.5.5
+Version: 1.6.0
 Summary: UNKNOWN
 Home-page: https://github.com/k2-fsa/sherpa-onnx
 Author: The sherpa-onnx development team
 Author-email: dpovey@gmail.com
 License: Apache licensed, as found in the LICENSE file
 Platform: UNKNOWN
 Classifier: Programming Language :: C++
```

