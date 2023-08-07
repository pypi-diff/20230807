# Comparing `tmp/sign_language_translator-0.5.0.tar.gz` & `tmp/sign_language_translator-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sign_language_translator-0.5.0.tar", max compression
+gzip compressed data, was "sign_language_translator-0.6.0.tar", max compression
```

## Comparing `sign_language_translator-0.5.0.tar` & `sign_language_translator-0.6.0.tar`

### file list

```diff
@@ -1,56 +1,60 @@
--rw-r--r--   0        0        0    14574 2023-07-15 20:40:20.026369 sign_language_translator-0.5.0/README.md
--rw-r--r--   0        0        0     1180 2023-07-15 20:40:20.026369 sign_language_translator-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     2567 2023-07-15 20:40:20.026369 sign_language_translator-0.5.0/sign_language_translator/__init__.py
--rw-r--r--   0        0        0     3330 2023-07-15 20:40:20.026369 sign_language_translator-0.5.0/sign_language_translator/cli.py
--rw-r--r--   0        0        0      513 2023-07-15 20:40:20.026369 sign_language_translator-0.5.0/sign_language_translator/config/__init__.py
--rw-r--r--   0        0        0     2381 2023-07-15 20:40:20.026369 sign_language_translator-0.5.0/sign_language_translator/config/enums.py
--rw-r--r--   0        0        0     2184 2023-07-15 20:40:20.026369 sign_language_translator-0.5.0/sign_language_translator/config/helpers.py
--rw-r--r--   0        0        0     1704 2023-07-15 20:40:20.026369 sign_language_translator-0.5.0/sign_language_translator/config/settings.py
--rw-r--r--   0        0        0     1382 2023-07-15 20:40:20.026369 sign_language_translator-0.5.0/sign_language_translator/config/urls.yaml
--rw-r--r--   0        0        0        0 2023-07-15 20:40:20.026369 sign_language_translator-0.5.0/sign_language_translator/data_collection/__init__.py
--rwxr-xr-x   0        0        0    10252 2023-07-15 20:40:20.026369 sign_language_translator-0.5.0/sign_language_translator/data_collection/completeness.py
--rwxr-xr-x   0        0        0     7713 2023-07-15 20:40:20.026369 sign_language_translator-0.5.0/sign_language_translator/data_collection/scraping.py
--rwxr-xr-x   0        0        0     2107 2023-07-15 20:40:20.026369 sign_language_translator-0.5.0/sign_language_translator/data_collection/synonyms.py
--rw-r--r--   0        0        0      250 2023-07-15 20:40:20.026369 sign_language_translator-0.5.0/sign_language_translator/languages/__init__.py
--rw-r--r--   0        0        0      642 2023-07-15 20:40:20.026369 sign_language_translator-0.5.0/sign_language_translator/languages/sign/__init__.py
--rw-r--r--   0        0        0     4982 2023-07-15 20:40:20.026369 sign_language_translator-0.5.0/sign_language_translator/languages/sign/mapping_rules.py
--rw-r--r--   0        0        0     7987 2023-07-15 20:40:20.026369 sign_language_translator-0.5.0/sign_language_translator/languages/sign/pakistan_sign_language.py
--rw-r--r--   0        0        0     3773 2023-07-15 20:40:20.026369 sign_language_translator-0.5.0/sign_language_translator/languages/sign/sign_language.py
--rw-r--r--   0        0        0      355 2023-07-15 20:40:20.026369 sign_language_translator-0.5.0/sign_language_translator/languages/text/__init__.py
--rw-r--r--   0        0        0       80 2023-07-15 20:40:20.026369 sign_language_translator-0.5.0/sign_language_translator/languages/text/english.py
--rw-r--r--   0        0        0     1070 2023-07-15 20:40:20.026369 sign_language_translator-0.5.0/sign_language_translator/languages/text/text_language.py
--rw-r--r--   0        0        0    13072 2023-07-15 20:40:20.026369 sign_language_translator-0.5.0/sign_language_translator/languages/text/urdu.py
--rw-r--r--   0        0        0     2083 2023-07-15 20:40:20.026369 sign_language_translator-0.5.0/sign_language_translator/languages/utils.py
--rw-r--r--   0        0        0    12426 2023-07-15 20:40:20.026369 sign_language_translator-0.5.0/sign_language_translator/languages/vocab.py
--rw-r--r--   0        0        0      571 2023-07-15 20:40:20.026369 sign_language_translator-0.5.0/sign_language_translator/models/__init__.py
--rw-r--r--   0        0        0      455 2023-07-15 20:40:20.026369 sign_language_translator-0.5.0/sign_language_translator/models/language_models/__init__.py
--rwxr-xr-x   0        0        0     1171 2023-07-15 20:40:20.026369 sign_language_translator-0.5.0/sign_language_translator/models/language_models/abstract_language_model.py
--rwxr-xr-x   0        0        0     3277 2023-07-15 20:40:20.026369 sign_language_translator-0.5.0/sign_language_translator/models/language_models/beam_sampling.py
--rwxr-xr-x   0        0        0     2785 2023-07-15 20:40:20.026369 sign_language_translator-0.5.0/sign_language_translator/models/language_models/mixer.py
--rwxr-xr-x   0        0        0     9002 2023-07-15 20:40:20.026369 sign_language_translator-0.5.0/sign_language_translator/models/language_models/simple_language_model.py
--rwxr-xr-x   0        0        0       74 2023-07-15 20:40:20.026369 sign_language_translator-0.5.0/sign_language_translator/models/language_models/transformer_language_model.py
--rw-r--r--   0        0        0        0 2023-07-15 20:40:20.026369 sign_language_translator-0.5.0/sign_language_translator/models/sign_to_text/__init__.py
--rw-r--r--   0        0        0      158 2023-07-15 20:40:20.026369 sign_language_translator-0.5.0/sign_language_translator/models/text_to_sign/__init__.py
--rw-r--r--   0        0        0     3237 2023-07-15 20:40:20.026369 sign_language_translator-0.5.0/sign_language_translator/models/text_to_sign/concatenative_synthesis.py
--rw-r--r--   0        0        0      536 2023-07-15 20:40:20.030370 sign_language_translator-0.5.0/sign_language_translator/models/text_to_sign/t2s_model.py
--rw-r--r--   0        0        0     1845 2023-07-15 20:40:20.030370 sign_language_translator-0.5.0/sign_language_translator/models/utils.py
--rw-r--r--   0        0        0      446 2023-07-15 20:40:20.030370 sign_language_translator-0.5.0/sign_language_translator/text/__init__.py
--rwxr-xr-x   0        0        0     3320 2023-07-15 20:40:20.030370 sign_language_translator-0.5.0/sign_language_translator/text/metrics.py
--rwxr-xr-x   0        0        0      882 2023-07-15 20:40:20.030370 sign_language_translator-0.5.0/sign_language_translator/text/preprocess.py
--rwxr-xr-x   0        0        0     1333 2023-07-15 20:40:20.030370 sign_language_translator-0.5.0/sign_language_translator/text/subtitles.py
--rw-r--r--   0        0        0     4248 2023-07-15 20:40:20.030370 sign_language_translator-0.5.0/sign_language_translator/text/tagger.py
--rw-r--r--   0        0        0     4800 2023-07-15 20:40:20.030370 sign_language_translator-0.5.0/sign_language_translator/text/tokenizer.py
--rwxr-xr-x   0        0        0     9223 2023-07-15 20:40:20.030370 sign_language_translator-0.5.0/sign_language_translator/text/utils.py
--rwxr-xr-x   0        0        0      590 2023-07-15 20:40:20.030370 sign_language_translator-0.5.0/sign_language_translator/utils/__init__.py
--rwxr-xr-x   0        0        0     3675 2023-07-15 20:40:20.030370 sign_language_translator-0.5.0/sign_language_translator/utils/data_loader.py
--rw-r--r--   0        0        0     4376 2023-07-15 20:40:20.030370 sign_language_translator-0.5.0/sign_language_translator/utils/download.py
--rwxr-xr-x   0        0        0    13542 2023-07-15 20:40:20.030370 sign_language_translator-0.5.0/sign_language_translator/utils/landmarks_info.py
--rwxr-xr-x   0        0        0    10351 2023-07-15 20:40:20.030370 sign_language_translator-0.5.0/sign_language_translator/utils/sign_data_attributes.py
--rwxr-xr-x   0        0        0     2822 2023-07-15 20:40:20.030370 sign_language_translator-0.5.0/sign_language_translator/utils/tree.py
--rw-r--r--   0        0        0      535 2023-07-15 20:40:20.030370 sign_language_translator-0.5.0/sign_language_translator/utils/utils.py
--rw-r--r--   0        0        0        0 2023-07-15 20:40:20.030370 sign_language_translator-0.5.0/sign_language_translator/vision/__init__.py
--rwxr-xr-x   0        0        0    18024 2023-07-15 20:40:20.030370 sign_language_translator-0.5.0/sign_language_translator/vision/concatenate.py
--rwxr-xr-x   0        0        0     7980 2023-07-15 20:40:20.030370 sign_language_translator-0.5.0/sign_language_translator/vision/embed.py
--rwxr-xr-x   0        0        0    33628 2023-07-15 20:40:20.030370 sign_language_translator-0.5.0/sign_language_translator/vision/transforms.py
--rwxr-xr-x   0        0        0    30236 2023-07-15 20:40:20.030370 sign_language_translator-0.5.0/sign_language_translator/vision/visualization.py
--rw-r--r--   0        0        0    16076 1970-01-01 00:00:00.000000 sign_language_translator-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    26475 2023-08-07 12:18:55.242593 sign_language_translator-0.6.0/README.md
+-rw-r--r--   0        0        0     1215 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     2964 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/__init__.py
+-rw-r--r--   0        0        0     6925 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/cli.py
+-rw-r--r--   0        0        0      513 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/config/__init__.py
+-rw-r--r--   0        0        0     6245 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/config/enums.py
+-rw-r--r--   0        0        0     1736 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/config/helpers.py
+-rw-r--r--   0        0        0     1768 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/config/settings.py
+-rw-r--r--   0        0        0     2572 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/config/urls.yaml
+-rw-r--r--   0        0        0        0 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/data_collection/__init__.py
+-rwxr-xr-x   0        0        0    10252 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/data_collection/completeness.py
+-rwxr-xr-x   0        0        0     7713 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/data_collection/scraping.py
+-rwxr-xr-x   0        0        0     2107 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/data_collection/synonyms.py
+-rw-r--r--   0        0        0      250 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/languages/__init__.py
+-rw-r--r--   0        0        0      642 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/languages/sign/__init__.py
+-rw-r--r--   0        0        0     4982 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/languages/sign/mapping_rules.py
+-rw-r--r--   0        0        0     7989 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/languages/sign/pakistan_sign_language.py
+-rw-r--r--   0        0        0     3773 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/languages/sign/sign_language.py
+-rw-r--r--   0        0        0      355 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/languages/text/__init__.py
+-rw-r--r--   0        0        0       80 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/languages/text/english.py
+-rw-r--r--   0        0        0     1070 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/languages/text/text_language.py
+-rw-r--r--   0        0        0    13164 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/languages/text/urdu.py
+-rw-r--r--   0        0        0     2083 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/languages/utils.py
+-rw-r--r--   0        0        0    12432 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/languages/vocab.py
+-rw-r--r--   0        0        0     1773 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/models/__init__.py
+-rw-r--r--   0        0        0     3297 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/models/_utils.py
+-rw-r--r--   0        0        0     1958 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/models/language_models/__init__.py
+-rwxr-xr-x   0        0        0     2699 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/models/language_models/abstract_language_model.py
+-rwxr-xr-x   0        0        0     5407 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/models/language_models/beam_sampling.py
+-rwxr-xr-x   0        0        0     7775 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/models/language_models/mixer.py
+-rwxr-xr-x   0        0        0    11347 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/models/language_models/ngram_language_model.py
+-rw-r--r--   0        0        0      873 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/models/language_models/transformer_language_model/__init__.py
+-rw-r--r--   0        0        0    13121 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/models/language_models/transformer_language_model/layers.py
+-rw-r--r--   0        0        0    18592 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/models/language_models/transformer_language_model/model.py
+-rw-r--r--   0        0        0    15500 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/models/language_models/transformer_language_model/train.py
+-rw-r--r--   0        0        0        0 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/models/sign_to_text/__init__.py
+-rw-r--r--   0        0        0      264 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/models/text_to_sign/__init__.py
+-rw-r--r--   0        0        0     3237 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/models/text_to_sign/concatenative_synthesis.py
+-rw-r--r--   0        0        0      536 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/models/text_to_sign/t2s_model.py
+-rw-r--r--   0        0        0    12989 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/models/utils.py
+-rw-r--r--   0        0        0      466 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/text/__init__.py
+-rwxr-xr-x   0        0        0     3320 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/text/metrics.py
+-rwxr-xr-x   0        0        0      882 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/text/preprocess.py
+-rwxr-xr-x   0        0        0     1333 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/text/subtitles.py
+-rw-r--r--   0        0        0     4248 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/text/tagger.py
+-rw-r--r--   0        0        0     4800 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/text/tokenizer.py
+-rwxr-xr-x   0        0        0    12817 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/text/utils.py
+-rwxr-xr-x   0        0        0      850 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/utils/__init__.py
+-rwxr-xr-x   0        0        0     3675 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/utils/data_loader.py
+-rw-r--r--   0        0        0     5076 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/utils/download.py
+-rwxr-xr-x   0        0        0    13542 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/utils/landmarks_info.py
+-rwxr-xr-x   0        0        0    10351 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/utils/sign_data_attributes.py
+-rwxr-xr-x   0        0        0     2822 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/utils/tree.py
+-rw-r--r--   0        0        0     1414 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/utils/utils.py
+-rw-r--r--   0        0        0        0 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/vision/__init__.py
+-rwxr-xr-x   0        0        0    18024 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/vision/concatenate.py
+-rwxr-xr-x   0        0        0     7980 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/vision/embed.py
+-rwxr-xr-x   0        0        0    33628 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/vision/transforms.py
+-rwxr-xr-x   0        0        0    30236 2023-08-07 12:18:55.246594 sign_language_translator-0.6.0/sign_language_translator/vision/visualization.py
+-rw-r--r--   0        0        0    27995 1970-01-01 00:00:00.000000 sign_language_translator-0.6.0/PKG-INFO
```

### Comparing `sign_language_translator-0.5.0/pyproject.toml` & `sign_language_translator-0.6.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "sign_language_translator"
-version = "0.5.0"
-description = "Translate between spoken/text and sign language using AI."
+version = "0.6.0"
+description = "Translate between spoken/text languages and sign language videos using AI."
 authors = ["Mudassar Iqbal <mdsriqb@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "sign_language_translator"}]
 repository = "https://github.com/sign-language-translator/sign-language-translator"
 keywords = ["sign", "translation", "pose", "pakistan", "deep-learning", "computer-vision", "nlp", "sign-language", "sign-language-translation"]
 
@@ -15,15 +15,15 @@
 matplotlib = "^3.7.2"
 mediapipe = "0.9.1.0"
 moviepy = "^1.0.3"
 numpy = "^1.25.1"
 pandas = "^2.0.3"
 pillow = "^10.0.0"
 scipy = "^1.11.1"
-torch = "^2.0.1"
+torch = ">=2.0.0,<2.0.1 || >2.0.1"
 scikit-image = "^0.21.0"
 beautifulsoup4 = "^4.12.2"
 deep-translator = "^1.11.4"
 opencv-contrib-python = "^4.8.0.74"
 tqdm = "^4.65.0"
 pyyaml = "^6.0"
 click = "^8.1.4"
```

### Comparing `sign_language_translator-0.5.0/sign_language_translator/__init__.py` & `sign_language_translator-0.6.0/sign_language_translator/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,25 +3,27 @@
 The goal is to provide a user friendly API to novel Sign Language Translation solutions that can easily adapt to any regional sign language.
 
 ## Usage
 
 ```python
 import sign_language_translator as slt
 
-# download dataset (by default, dataset is downloaded within the install directory)
-# slt.set_dataset_dir("path/to/sign-language-datasets") # optional
-# slt.download("id")
+# download dataset or models (by default, dataset is auto-downloaded within the install directory)
+# slt.set_resource_dir("path/to/sign-language-datasets") # optional. Helps when data is synced with cloud
+
+# slt.utils.download("path", "url") # optional
+# slt.utils.download_resource(".*.json") # optional
 
 # ------------------------------------------
 
 # Load text-to-sign model
 # deep_t2s_model = slt.get_model("generative_t2s_base-01") # pytorch
 # rule-based model (concatenates clips of each word)
 t2s_model = slt.get_model(
-    model_code = "ConcatenativeSynthesis", # slt.enums.ModelCodes.CONCATENATIVE_SYNTHESIS.value
+    model_code = "concatenative-synthesis", # slt.ModelCodes.CONCATENATIVE_SYNTHESIS.value
     text_language = "English", # or object of any child of slt.languages.text.text_language.TextLanguage class
     sign_language = "PakistanSignLanguage", # or object of any child of slt.languages.sign.sign_language.SignLanguage class
     sign_feature_model = "mediapipe_pose_v2_hand_v1",
 )
 
 text = "hello world!"
 sign_language_sentence = t2s_model(text)
@@ -52,31 +54,41 @@
     languages,
     models,
     text,
     utils,
     vision,
 )
 from sign_language_translator.config import enums
-from sign_language_translator.config.settings import Settings, set_dataset_dir
+from sign_language_translator.config.enums import (
+    ModelCodes,
+    TextLanguages as TextLanguageCodes,
+    SignLanguages as SignLanguageCodes,
+)
+from sign_language_translator.config.settings import Settings, set_resources_dir
 from sign_language_translator.languages import get_sign_language, get_text_language
 from sign_language_translator.models import get_model
 
-
 __version__ = config.helpers.get_package_version()
 
 __all__ = [
-    "set_dataset_dir",
+    # config
+    "set_resources_dir",
     "Settings",
+    # modules
     "vision",
     "text",
     "data_collection",
     "models",
     "languages",
     "utils",
     "config",
     "enums",
+    # classes (enum)
+    "ModelCodes",
+    "TextLanguageCodes",
+    "SignLanguageCodes",
     # object loaders
     "get_sign_language",
     "get_text_language",
     "get_model"
     # "get_feature_model"
 ]
```

### Comparing `sign_language_translator-0.5.0/sign_language_translator/config/__init__.py` & `sign_language_translator-0.6.0/sign_language_translator/config/__init__.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.5.0/sign_language_translator/config/settings.py` & `sign_language_translator-0.6.0/sign_language_translator/config/settings.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,59 +1,57 @@
 """defines settings constants for global context
 
 Module Structure:
 - Settings (class): contains config constants as class variables.
-- set_dataset_dir(path: str) -> None: Sets the dataset directory path in Settings.
+- set_resources_dir(path: str) -> None: Sets the resources(dataset/models) directory path in Settings.
 """
 
 from os.path import dirname, isdir, join
 
-from sign_language_translator.config.helpers import (
-    get_package_version,
-    prepare_filename_url_dict,
-)
+from sign_language_translator.config.helpers import prepare_filename_url_dict
 
 
 class Settings:
     """Class containing settings and configuration parameters
     for the sign language translator library."""
 
-    DATASET_ROOT_DIRECTORY: str = join(
-        dirname(dirname(__file__)), "sign-language-datasets"
+    RESOURCES_ROOT_DIRECTORY: str = join(
+        dirname(dirname(__file__)), "sign-language-resources"
     )
-    """The root directory path where the sign language datasets are stored."""
+    """The root directory path where the sign language datasets & models are stored."""
 
     FILENAME_SEPARATOR = "_"
     """The separator used in dataset filenames to separate different attributes."""
 
     FILENAME_CONNECTOR = "-"
     """The connector used in filenames to join parts of same attribute."""
 
     FILE_TO_URLS = prepare_filename_url_dict(
-        get_package_version(), join(dirname(__file__), "urls.yaml")
+        join(dirname(__file__), "urls.yaml")
     )
     """A dictionary mapping filenames to their corresponding URLs, based on the package version."""
 
     AUTO_DOWNLOAD = True
     """A flag indicating whether automatic downloading of missing dataset files is enabled."""
 
 
-def set_dataset_dir(path: str) -> None:
-    """Set the sign-language-datasets directory path.
+def set_resources_dir(path: str) -> None:
+    """Set the SLT resources directory path.
+    Helpful when sign-language-datasets from the cloud is mounted on disk.
 
     Args:
-        path (str): The path to the dataset directory.
+        path (str): The path to the resources/dataset/models directory.
 
     Raises:
         AssertionError: If the provided path is not a directory.
     """
 
     assert isdir(path), f"the provided path is not a directory. Path: {path}"
 
-    Settings.DATASET_ROOT_DIRECTORY = path
+    Settings.RESOURCES_ROOT_DIRECTORY = path
     # ? trigger an event
 
 
 __all__ = [
     "Settings",
-    "set_dataset_dir",
+    "set_resources_dir",
 ]
```

### Comparing `sign_language_translator-0.5.0/sign_language_translator/config/urls.yaml` & `sign_language_translator-0.6.0/sign_language_translator/config/urls.yaml`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,43 @@
 datasets:
-  - name: sign-language-dataset-1
-    version: 1.0.0
+  - name: word-mapping-dataset
     files:
       - name: sign_recordings/collection_to_label_to_language_to_words.json
         url: https://raw.githubusercontent.com/sign-language-translator/sign-language-datasets/e86a579a8d87180526fc73539544f18d0a8a3755/sign_recordings/collection_to_label_to_language_to_words.json
       - name: sign_recordings/organization_to_language_to_constructable_words.json
         url: https://raw.githubusercontent.com/sign-language-translator/sign-language-datasets/e86a579a8d87180526fc73539544f18d0a8a3755/sign_recordings/organization_to_language_to_constructable_words.json
       - name: sign_recordings/recordings_labels.json
         url: https://raw.githubusercontent.com/sign-language-translator/sign-language-datasets/e86a579a8d87180526fc73539544f18d0a8a3755/sign_recordings/recordings_labels.json
       - name: text_preprocessing.json
         url: https://raw.githubusercontent.com/sign-language-translator/sign-language-datasets/e86a579a8d87180526fc73539544f18d0a8a3755/text_preprocessing.json
       - name: language_to_token_to_id.json
         url: https://raw.githubusercontent.com/sign-language-translator/sign-language-datasets/e86a579a8d87180526fc73539544f18d0a8a3755/language_to_token_to_id.json
 
-package_versions:
-  - version: 0.4.2
-    dataset_version: 1.0.0
+models:
+  - name: language-models
+    files:
+      - name: models/names-stat-lm-w1.json
+        url: https://github.com/sign-language-translator/sign-language-datasets/releases/download/v0.0.1/names-stat-lm-w1.json
+      - name: models/names-stat-lm-w2.json
+        url: https://github.com/sign-language-translator/sign-language-datasets/releases/download/v0.0.1/names-stat-lm-w2.json
+      - name: models/names-stat-lm-w3.json
+        url: https://github.com/sign-language-translator/sign-language-datasets/releases/download/v0.0.1/names-stat-lm-w3.json
+      - name: models/ur-supported-token-unambiguous-mixed-ngram-w1-w6-lm.pkl
+        url: https://github.com/sign-language-translator/sign-language-datasets/releases/download/v0.0.1/ur-supported-token-unambiguous-mixed-ngram-w1-w6-lm.pkl
+      - name: models/tlm_14.0M.pt
+        url: https://github.com/sign-language-translator/sign-language-datasets/releases/download/v0.0.1/tlm_8.7M.pt
+
+  - name: text-to-sign
+    files:
+      - name: x.x
+        url: https://
 
-  - version: 0.5.0
-    dataset_version: 1.0.0
+  - name: sign-to-text
+    files:
+      - name: x.y
+        url: https://
+
+others:
+  - name: extra-url-files
+    files:
+      - name: extra_urls.yaml
+        url: "https://raw.githubusercontent.com/sign-language-translator/sign-language-datasets/1456b64b4ed38247a7a792f706403af1ed2287b4/extra_urls.yaml"
```

### Comparing `sign_language_translator-0.5.0/sign_language_translator/data_collection/completeness.py` & `sign_language_translator-0.6.0/sign_language_translator/data_collection/completeness.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.5.0/sign_language_translator/data_collection/scraping.py` & `sign_language_translator-0.6.0/sign_language_translator/data_collection/scraping.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.5.0/sign_language_translator/data_collection/synonyms.py` & `sign_language_translator-0.6.0/sign_language_translator/data_collection/synonyms.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.5.0/sign_language_translator/languages/sign/__init__.py` & `sign_language_translator-0.6.0/sign_language_translator/languages/sign/__init__.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.5.0/sign_language_translator/languages/sign/mapping_rules.py` & `sign_language_translator-0.6.0/sign_language_translator/languages/sign/mapping_rules.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.5.0/sign_language_translator/languages/sign/pakistan_sign_language.py` & `sign_language_translator-0.6.0/sign_language_translator/languages/sign/pakistan_sign_language.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     STOPWORDS = {"is", "am", "are"}
 
     def __init__(self) -> None:
         # load word maps and info from dataset files
         self.vocab = Vocab(
             language=r"^(?!.*\bcomponents\b).*$",  # r".*",
             sign_collections=[r"pk-hfad(-\d+)?"],  # [r"pk-.+"]
-            data_root_dir=Settings.DATASET_ROOT_DIRECTORY,
+            data_root_dir=Settings.RESOURCES_ROOT_DIRECTORY,
             arg_is_regex=True,
         )
         # restructure dict values
         self.word_to_sign_dict = {
             word: self._make_equal_weight_sign_dict(labels)
             for word, labels in self.vocab.word_to_labels.items()
         }
```

### Comparing `sign_language_translator-0.5.0/sign_language_translator/languages/sign/sign_language.py` & `sign_language_translator-0.6.0/sign_language_translator/languages/sign/sign_language.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.5.0/sign_language_translator/languages/text/text_language.py` & `sign_language_translator-0.6.0/sign_language_translator/languages/text/text_language.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.5.0/sign_language_translator/languages/text/urdu.py` & `sign_language_translator-0.6.0/sign_language_translator/languages/text/urdu.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import re
-import string
+from string import ascii_uppercase, digits
 from typing import Any, Dict, Iterable, List, Set, Union
 
 from sign_language_translator.config.settings import Settings
 from sign_language_translator.languages.text.text_language import TextLanguage
 from sign_language_translator.languages.vocab import Vocab
 from sign_language_translator.text.preprocess import (
     remove_space_before_punctuation,
@@ -26,15 +26,15 @@
     def allowed_characters(cls) -> Set[str]:
         return cls.ALLOWED_CHARACTERS
 
     def __init__(self) -> None:
         self.vocab = Vocab(
             language=self.name(),
             sign_collections=[r".*"],
-            data_root_dir=Settings.DATASET_ROOT_DIRECTORY,
+            data_root_dir=Settings.RESOURCES_ROOT_DIRECTORY,
             arg_is_regex=True,
         )
 
         self.non_sentence_end_tokens = {
             # letters (A.B.C.) & spelled out letters (Ay, Bee, See)
             w.upper()
             for wc in self.vocab.supported_words_with_word_sense
@@ -42,21 +42,18 @@
             if (("double-handed-letter)" in wc) and (not w.isascii()))
             or (len(w) == 1 and w.isalpha())
         }
 
         self.tokenizer = SignTokenizer(
             word_regex=self.word_regex(),
             compound_words=(
-                self.vocab.supported_words # TODO why does this variable exist?
+                self.vocab.supported_words  # TODO why does this variable exist?
                 | self.vocab.supported_words_with_word_sense
-                | {
-                    w
-                    for word in self.vocab.words_to_numbers.keys()
-                    for w in [word, word.replace("-", " ")]
-                }
+                | set(self.vocab.words_to_numbers.keys())
+                | set(self.vocab.person_names)
             ),  # TODO: | one-hundred twenty-three (\d[ \d]*): ["100", "23"] --> ["123"]
             end_of_sentence_tokens=self.END_OF_SENTENCE_MARKS,
             full_stops=self.FULL_STOPS,
             non_sentence_end_words=self.non_sentence_end_tokens,
             tokenized_word_sense_pattern=[self.URDU_WORD_REGEX, r"\(", [r"نام"], r"\)"],
         )
 
@@ -113,42 +110,47 @@
         ]
         self.tagger = Tagger(
             rules=self.tagging_rules,
             default=Tags.DEFAULT,
         )
 
     def preprocess(self, text: str) -> str:
+
+        # TODO: optimize (especially regex)
         text = self.character_normalize(text)
 
         # spell fix
         text = replace_words(
             text,
             word_map=self.vocab.misspelled_to_correct,  # :TODO: split joint words
             word_regex=self.word_regex(),
         )
-        text = remove_space_before_punctuation(text, self.PUNCTUATION)
         text = self.delete_unallowed_characters(text)
         text = re.sub(r"[۔\.][۔\. ]+[\.۔]", "۔۔۔", text)
         text = re.sub(r"[ \t]+", " ", text)
+        text = remove_space_before_punctuation(text, self.PUNCTUATION)
         text = text.strip()
 
         return text
 
     def tokenize(self, text: str) -> List[str]:
         tokens = self.tokenizer.tokenize(
             text, join_compound_words=True, join_word_sense=True
         )
         return tokens
 
     def sentence_tokenize(self, text: str) -> List[str]:
         sentences = self.tokenizer.sentence_tokenize(text)
-        sentences = [sentence.strip() for sentence in sentences]
+        if len(sentences) > 1:
+            sentences[1:] = [sentence.lstrip() for sentence in sentences[1:]]
+            sentences[:-1] = [sentence.rstrip() for sentence in sentences[:-1]]
+        # sentences = [sen for sen in sentences if sen]
         return sentences
 
-    def detokenize(self, tokens: str) -> str:
+    def detokenize(self, tokens: Iterable[str]) -> str:
         text = self.tokenizer.detokenize(tokens)
         return text
 
     def tag(self, tokens: Union[str, Iterable[str]]) -> List[Any]:
         if isinstance(tokens, str):
             tokens = [tokens]
 
@@ -183,15 +185,15 @@
 
     QUOTATION_MARKS = """ ' " ” “ ’ ‘ """.split()
     BRACKETS: List[str] = ["(", ")"]
     SYMBOLS: List[str] = PUNCTUATION + QUOTATION_MARKS + BRACKETS + [" ", "-"]
 
     PUNCTUATION_REGEX = r"[" + "".join([re.escape(punc) for punc in PUNCTUATION]) + r"]"
     URDU_DIACRITICS = " ٍ ً ٰ َ ُ ِ ".split()
-    URDU_WORD_REGEX = r"[\w" + "".join(URDU_DIACRITICS) + r"]+"
+    URDU_WORD_REGEX = r"[\w" + "".join(URDU_DIACRITICS) + r"]+"  # TODO: r"[[^\W\d_]"+ "".join(URDU_DIACRITICS) + r"]+"
 
     NUMBER_REGEX = r"\d+(?:[\.:]\d+)*"
 
     CHARACTER_TO_WORD = {
         "ﷲ": "اللہ",
         "ﷺ": "صلی اللہ علیہ وسلم",
         "﷽": "بسم اللہ الرحمن الرحیم",
@@ -361,18 +363,16 @@
 
         # End of the code borrowed from UrduHack
 
     ALLOWED_CHARACTERS = (
         set(CORRECT_URDU_CHARACTERS_TO_INCORRECT.keys())
         | set(URDU_DIACRITICS)
         | set(SYMBOLS)
-        | set(string.ascii_uppercase)  # acronyms
-        # TODO: remove ascii_lowercase when word-senses are also urdu in dataset
-        # | set(string.ascii_lowercase)  # word-sense
-        | set(string.digits)
+        | set(ascii_uppercase)  # acronyms
+        | set(digits)
         | set("()!.,?/[]{} ")
     )
     UNALLOWED_CHARACTERS_REGEX = (
         "[^" + "".join(map(re.escape, ALLOWED_CHARACTERS)) + "]"
     )
```

### Comparing `sign_language_translator-0.5.0/sign_language_translator/languages/utils.py` & `sign_language_translator-0.6.0/sign_language_translator/languages/utils.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.5.0/sign_language_translator/languages/vocab.py` & `sign_language_translator-0.6.0/sign_language_translator/languages/vocab.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 class Vocab:
     """loads data from files for a specific language and specified sign_collections"""
 
     def __init__(
         self,
         language: str = r"$.",
         sign_collections: Iterable[str] = (r"$.",),
-        data_root_dir: str = Settings.DATASET_ROOT_DIRECTORY,
+        data_root_dir: str = Settings.RESOURCES_ROOT_DIRECTORY,
         arg_is_regex: bool = True,
     ) -> None:
         # save arguments
         self.language = language
         self.sign_collections = sign_collections
         self.data_root_dir = data_root_dir
         self.arg_is_regex = arg_is_regex
@@ -305,16 +305,16 @@
         return ambiguous_2_unambiguous
 
     def _download_resource(self, full_path: str):
         if not Settings.AUTO_DOWNLOAD:
             return
         if os.path.exists(full_path):
             return
-        if full_path.startswith(Settings.DATASET_ROOT_DIRECTORY):
-            filename = full_path[len(Settings.DATASET_ROOT_DIRECTORY) :]
+        if full_path.startswith(Settings.RESOURCES_ROOT_DIRECTORY):
+            filename = full_path[len(Settings.RESOURCES_ROOT_DIRECTORY) :]
             filename = re.escape(filename.strip(os.path.sep))
             download_resource(filename, overwrite=False)
 
     # load sign video/features
 
 
 __all__ = [
```

### Comparing `sign_language_translator-0.5.0/sign_language_translator/models/text_to_sign/concatenative_synthesis.py` & `sign_language_translator-0.6.0/sign_language_translator/models/text_to_sign/concatenative_synthesis.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.5.0/sign_language_translator/models/text_to_sign/t2s_model.py` & `sign_language_translator-0.6.0/sign_language_translator/models/text_to_sign/t2s_model.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.5.0/sign_language_translator/text/metrics.py` & `sign_language_translator-0.6.0/sign_language_translator/text/metrics.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.5.0/sign_language_translator/text/preprocess.py` & `sign_language_translator-0.6.0/sign_language_translator/text/preprocess.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.5.0/sign_language_translator/text/subtitles.py` & `sign_language_translator-0.6.0/sign_language_translator/text/subtitles.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.5.0/sign_language_translator/text/tagger.py` & `sign_language_translator-0.6.0/sign_language_translator/text/tagger.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.5.0/sign_language_translator/text/tokenizer.py` & `sign_language_translator-0.6.0/sign_language_translator/text/tokenizer.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.5.0/sign_language_translator/text/utils.py` & `sign_language_translator-0.6.0/sign_language_translator/text/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,20 @@
-"""other functions
+"""
+Utility Functions for Text Processing
+
+This module contains utility functions for text processing tasks.
+
+Functions:
+    make_ngrams: Creates n-grams from a given sequence.
+    extract_supported_subsequences_indexes: Extracts the indexes of subsequences based on provided tags and skipped items.
+    extract_supported_subsequences: Extracts subsequences from a given sequence based on provided tags and skipped items.
+    concatenate_sentence_terminals: Concatenates start and end of sentence tokens to a list of sentences.
+
+Classes:
+    ListRegex: A utility class for finding sub-lists within a list of strings that match specified patterns.
 """
 
 import re
 from typing import Any, Iterable, List, Set, Tuple
 
 
 def make_ngrams(sequence: Iterable, n: int) -> List[Iterable]:
@@ -18,19 +30,61 @@
             The type of list items is same as sequence argument.
     """
 
     start = 0
     end = len(sequence) - n  # type: ignore
 
     ngrams = (
-        [sequence[i : i + n] for i in range(start, end + 1)] if end >= start else [] # type: ignore
+        [sequence[i : i + n] for i in range(start, end + 1)] if end >= start else []  # type: ignore
     )
     return ngrams
 
 
+def extract_supported_subsequences_indexes(
+    sequence: Iterable[Any],
+    tags: Iterable[Any],
+    supported_tags: Set[Any],
+    skipped_items: Set[Any],
+) -> List[List[int]]:
+    """Extract indexes of supported subsequences from a sequence based on tags and skipped items.
+
+    Args:
+        sequence (Iterable[Any]): The input sequence.
+        tags (Iterable[Any]): Tags corresponding to each item in the sequence.
+        supported_tags (Set[Any]): Set of tags indicating support for a subsequence.
+        skipped_items (Set[Any]): Set of items to be skipped.
+
+    Returns:
+        List[List[int]]: A list indices of supported subsequences, where each inner list represents a subsequence.
+
+    Examples:
+        >>> sequence = [1, 2, 3, 4, 5, 6]
+        >>> tags = ['A', 'A', 'B', 'A', 'A', 'C']
+        >>> supported_tags = {'A'}
+        >>> skipped_items = {2}
+        >>> extract_supported_subsequences(sequence, tags, supported_tags, skipped_items)
+        [[0], [3, 4]]
+    """
+
+    all_subsequences = []
+    subsequence = []
+    for i, (token, tag) in enumerate(zip(sequence, tags)):
+        if (tag in supported_tags) and (token not in skipped_items):
+            subsequence.append(i)
+        else:
+            if subsequence:
+                all_subsequences.append(subsequence)
+                subsequence = []
+
+    if subsequence:
+        all_subsequences.append(subsequence)
+
+    return all_subsequences
+
+
 def extract_supported_subsequences(
     sequence: Iterable[Any],
     tags: Iterable[Any],
     supported_tags: Set[Any],
     skipped_items: Set[Any],
 ) -> List[List[Any]]:
     """Extract supported subsequences from a sequence based on tags and skipped items.
@@ -49,30 +103,62 @@
         >>> tags = ['A', 'A', 'B', 'A', 'A', 'C']
         >>> supported_tags = {'A'}
         >>> skipped_items = {2}
         >>> extract_supported_subsequences(sequence, tags, supported_tags, skipped_items)
         [[1], [4, 5]]
     """
 
-    subsequences = []
-    subseq = []
-    for token, tag in zip(sequence, tags):
-        if (tag in supported_tags) and (token not in skipped_items):
-            subseq.append(token)
-        else:
-            if subseq:
-                subsequences.append(subseq)
-                subseq = []
+    indexes = extract_supported_subsequences_indexes(
+        sequence=sequence,
+        tags=tags,
+        supported_tags=supported_tags,
+        skipped_items=skipped_items,
+    )
 
-    if subseq:
-        subsequences.append(subseq)
+    subsequences = [[sequence[i] for i in index] for index in indexes]  # type: ignore
 
     return subsequences
 
 
+def concatenate_sentence_terminals(sentences: List, start_token, end_token):
+    """
+    Inserts start and end tokens between the sentences the input list and
+    concatenates them to the sentences (useful when the input is coming from a sentence tokenizer.)
+
+    This function takes a list of sentences and adds a start token to the beginning
+    of each sentence except the first and an end token to the end of each sentence except the last.
+
+    Parameters:
+        sentences (List): A list of sentences to be processed.
+            Sentences can be strings or list of tokens or any type but it must support + operator for concatenation.
+        start_token: The token to be added at the start of sentences. Must be same type as a sentence.
+        end_token: The token to be added at the end of sentences. Must be same type as a sentence.
+
+    Returns:
+        List: A new list of sentences with start and end tokens inserted.
+
+    Example:
+        sentences = ["Hello!", "How are you?", "Goodbye."]
+        start_token = "<start>"
+        end_token = "<end>"
+        result = concatenate_sentence_terminals(sentences, start_token, end_token)
+        # Output: ["Hello!<end>", "<start>How are you?<end>", "<start>Goodbye."]
+    """
+
+    new_sentences = []
+    for i, sentence in enumerate(sentences):
+        if i > 0:
+            sentence = start_token + sentence
+        if i < len(sentences) - 1:
+            sentence = sentence + end_token
+        new_sentences.append(sentence)
+
+    return new_sentences
+
+
 class ListRegex:
     """A utility class for finding sub-lists within a list of strings that match specified patterns.
 
     ListRegex provides methods for
     matching patterns against items in a list,
     searching for the first occurrence of patterns,
     finding all occurrences of patterns,
@@ -105,15 +191,17 @@
     patterns = ["orange", ["grape", "kiwi"]]
     result = ListRegex.find_all(items, patterns)
     # Output: [['orange', 'grape'], ['orange', 'kiwi']]
     ```
     """
 
     @staticmethod
-    def match(items: List[str], patterns: List[str | List | Tuple]) -> Tuple[int, int] | None:
+    def match(
+        items: List[str], patterns: List[str | List | Tuple]
+    ) -> Tuple[int, int] | None:
         """
         Matches the given patterns against the items in the list.
         Applies the patterns at the start of the list of string.
 
         Args:
             items (List[str]): The sequence of strings to be matched.
             patterns (List[str|List]): The patterns to be matched against the items.
@@ -254,10 +342,12 @@
                 break
 
         return spans
 
 
 __all__ = [
     "make_ngrams",
+    "extract_supported_subsequences_indexes",
     "extract_supported_subsequences",
+    "concatenate_sentence_terminals",
     "ListRegex",
 ]
```

### Comparing `sign_language_translator-0.5.0/sign_language_translator/utils/__init__.py` & `sign_language_translator-0.6.0/sign_language_translator/utils/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 """This module provides utility functions for the sign language translator package.
 
 Functions:
-- download: A function for downloading files.
+- download: A function for downloading files from urls.
+- download_resource: A function for downloading resource files based on filename regex.
 - tree: A function for printing a directory tree.
+- sample_one_index: Select an index based on the given probability distribution.
 - search_in_values_to_retrieve_key: search inside every dict value and return the key on match.
 """
 
-from sign_language_translator.utils.download import download_resource
+from sign_language_translator.utils.download import download, download_resource
 from sign_language_translator.utils.tree import tree
-from sign_language_translator.utils.utils import search_in_values_to_retrieve_key
+from sign_language_translator.utils.utils import (
+    sample_one_index,
+    search_in_values_to_retrieve_key,
+)
 
 __all__ = [
     "tree",
+    "download",
     "download_resource",
     "search_in_values_to_retrieve_key",
+    "sample_one_index",
 ]
```

### Comparing `sign_language_translator-0.5.0/sign_language_translator/utils/data_loader.py` & `sign_language_translator-0.6.0/sign_language_translator/utils/data_loader.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.5.0/sign_language_translator/utils/download.py` & `sign_language_translator-0.6.0/sign_language_translator/utils/download.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,31 +2,38 @@
 Module for downloading files from URLs and managing package resources.
 
 This module provides functions for downloading files from specified URLs and saving them to the given file paths.
 It also includes a function for downloading package resources matching a specified filename regex and saving them
 to the appropriate file paths.
 
 Functions:
-- download(file_path, url, overwrite=False, progress_bar=False, timeout=20.0):
+- download(file_path, url, overwrite=False, progress_bar=False, timeout=20.0, chunk_size=65536):
     Downloads a file from the specified URL and saves it to the given file path.
 - download_package_resource(filename_regex, overwrite=False, progress_bar=False, timeout=20.0):
     Downloads package resources matching the given filename regex and saves them to the appropriate file paths.
 """
 
 import os
 import re
+from time import time
 
 import requests
 from tqdm.auto import tqdm
 
 from sign_language_translator.config.settings import Settings
 
 
 def download(
-    file_path: str, url: str, overwrite=False, progress_bar=False, timeout: float = 20.0
+    file_path: str,
+    url: str,
+    overwrite=False,
+    progress_bar=False,
+    timeout: float = 20.0,
+    leave=True,
+    chunk_size=65536,
 ) -> bool:
     """
     Downloads a file from the specified URL and saves it to the given file path.
 
     Args:
         file_path (str): The path where the downloaded file will be saved.
         url (str): The URL of the file to be downloaded.
@@ -36,48 +43,68 @@
 
     Returns:
         bool: True if the file is downloaded successfully, False otherwise.
 
     Raises:
         FileExistsError: if overwrite is False and the destination path already contains a file.
     """
+
+    # TODO: resume failed download
+
     if os.path.exists(file_path) and not overwrite:
         raise FileExistsError(f"There is already a file at {file_path}")
 
     try:
         response = requests.get(url, stream=True, timeout=timeout)
         response.raise_for_status()
 
         os.makedirs(os.path.dirname(file_path), exist_ok=True)
 
         with open(file_path, "wb") as fp:
-            stream = response.iter_content(chunk_size=1024)
+            stream = response.iter_content(chunk_size=chunk_size)
 
             if progress_bar:
                 total_bytes = int(
                     response.headers.get("content-length", 0)
                 )  # for some reason, some bars finish too early
                 stream = tqdm(
                     stream,
-                    total=(total_bytes // 1024) + 1,
+                    total=(total_bytes // chunk_size) + 1,
                     desc=f"Downloading {os.path.split(file_path)[-1]}",
+                    leave=leave,
+                    unit="chunk",
                 )
 
+            start_time = time()
+            speed = 0
             for chunk in stream:
                 if chunk:
                     fp.write(chunk)
 
+                # display download speed
+                if progress_bar:
+                    speed = (len(chunk)/(1024**2)/(time() - start_time) + speed)/2
+                    stream.set_postfix_str(  # type:ignore
+                        f"{speed:.3f}MB/s"
+                    )
+                    start_time = time()
+
         return True
 
     except requests.exceptions.RequestException:
         return False
 
 
 def download_resource(
-    filename_regex: str, overwrite=False, progress_bar=False, timeout: float = 20.0
+    filename_regex: str,
+    overwrite=False,
+    progress_bar=False,
+    timeout: float = 20.0,
+    leave=True,
+    chunk_size=65536,
 ) -> bool:
     """
     Downloads package resources matching the given filename regex and saves them to the appropriate file paths.
 
     Args:
         filename_regex (str): Regular expression pattern to match the desired filenames.
         overwrite (bool, optional): If False, skips downloading if the resource file already exists. Defaults to False.
@@ -92,26 +119,28 @@
         key: val
         for key, val in Settings.FILE_TO_URLS.items()
         if re.match(filename_regex, key)
     }
     statuses = []
     for filename, url in matching_filenames_to_url.items():
         # Make sure that the file/directory exists
-        file_path = os.path.join(Settings.DATASET_ROOT_DIRECTORY, filename)
+        file_path = os.path.join(Settings.RESOURCES_ROOT_DIRECTORY, filename)
         if os.path.exists(file_path) and not overwrite:
             continue
         os.makedirs(os.path.dirname(file_path), exist_ok=True)
 
         # Download the file from the URL
         status = download(
             file_path,
             url,
             progress_bar=progress_bar,
             timeout=timeout,
             overwrite=overwrite,
+            leave=leave,
+            chunk_size=chunk_size,
         )
         statuses.append(status)
 
     return all(statuses or [False])
 
 
 __all__ = [
```

### Comparing `sign_language_translator-0.5.0/sign_language_translator/utils/landmarks_info.py` & `sign_language_translator-0.6.0/sign_language_translator/utils/landmarks_info.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.5.0/sign_language_translator/utils/sign_data_attributes.py` & `sign_language_translator-0.6.0/sign_language_translator/utils/sign_data_attributes.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.5.0/sign_language_translator/utils/tree.py` & `sign_language_translator-0.6.0/sign_language_translator/utils/tree.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.5.0/sign_language_translator/vision/concatenate.py` & `sign_language_translator-0.6.0/sign_language_translator/vision/concatenate.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.5.0/sign_language_translator/vision/embed.py` & `sign_language_translator-0.6.0/sign_language_translator/vision/embed.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.5.0/sign_language_translator/vision/transforms.py` & `sign_language_translator-0.6.0/sign_language_translator/vision/transforms.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.5.0/sign_language_translator/vision/visualization.py` & `sign_language_translator-0.6.0/sign_language_translator/vision/visualization.py`

 * *Files identical despite different names*

