# Comparing `tmp/simpletransformers-0.9.0.tar.gz` & `tmp/simpletransformers-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/simpletransformers-0.9.0.tar", last modified: Sat Nov 30 11:51:50 2019, max compression
+gzip compressed data, was "dist/simpletransformers-0.9.1.tar", last modified: Sat Nov 30 13:18:30 2019, max compression
```

## Comparing `simpletransformers-0.9.0.tar` & `simpletransformers-0.9.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-30 11:51:50.313473 simpletransformers-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (115)    49993 2019-11-30 11:51:50.313473 simpletransformers-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (115)    42061 2019-11-30 11:51:38.000000 simpletransformers-0.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (115)       38 2019-11-30 11:51:50.313473 simpletransformers-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (115)      996 2019-11-30 11:51:38.000000 simpletransformers-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-30 11:51:50.309472 simpletransformers-0.9.0/simpletransformers/
--rw-r--r--   0 runner    (1001) docker     (115)       27 2019-11-30 11:51:38.000000 simpletransformers-0.9.0/simpletransformers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-30 11:51:50.309472 simpletransformers-0.9.0/simpletransformers/classification/
--rw-r--r--   0 runner    (1001) docker     (115)      195 2019-11-30 11:51:38.000000 simpletransformers-0.9.0/simpletransformers/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)    31107 2019-11-30 11:51:38.000000 simpletransformers-0.9.0/simpletransformers/classification/classification_model.py
--rw-r--r--   0 runner    (1001) docker     (115)    13290 2019-11-30 11:51:38.000000 simpletransformers-0.9.0/simpletransformers/classification/classification_utils.py
--rw-r--r--   0 runner    (1001) docker     (115)     5818 2019-11-30 11:51:38.000000 simpletransformers-0.9.0/simpletransformers/classification/multi_label_classification_model.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-30 11:51:50.309472 simpletransformers-0.9.0/simpletransformers/classification/transformer_models/
--rw-r--r--   0 runner    (1001) docker     (115)        0 2019-11-30 11:51:38.000000 simpletransformers-0.9.0/simpletransformers/classification/transformer_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)     4769 2019-11-30 11:51:38.000000 simpletransformers-0.9.0/simpletransformers/classification/transformer_models/albert_model.py
--rw-r--r--   0 runner    (1001) docker     (115)     4740 2019-11-30 11:51:38.000000 simpletransformers-0.9.0/simpletransformers/classification/transformer_models/bert_model.py
--rw-r--r--   0 runner    (1001) docker     (115)     4771 2019-11-30 11:51:38.000000 simpletransformers-0.9.0/simpletransformers/classification/transformer_models/camembert_model.py
--rw-r--r--   0 runner    (1001) docker     (115)     4025 2019-11-30 11:51:38.000000 simpletransformers-0.9.0/simpletransformers/classification/transformer_models/distilbert_model.py
--rw-r--r--   0 runner    (1001) docker     (115)     4733 2019-11-30 11:51:38.000000 simpletransformers-0.9.0/simpletransformers/classification/transformer_models/roberta_model.py
--rw-r--r--   0 runner    (1001) docker     (115)     3962 2019-11-30 11:51:38.000000 simpletransformers-0.9.0/simpletransformers/classification/transformer_models/xlm_model.py
--rw-r--r--   0 runner    (1001) docker     (115)     5818 2019-11-30 11:51:38.000000 simpletransformers-0.9.0/simpletransformers/classification/transformer_models/xlnet_model.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-30 11:51:50.309472 simpletransformers-0.9.0/simpletransformers/custom_models/
--rw-r--r--   0 runner    (1001) docker     (115)        0 2019-11-30 11:51:38.000000 simpletransformers-0.9.0/simpletransformers/custom_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)    13080 2019-11-30 11:51:38.000000 simpletransformers-0.9.0/simpletransformers/custom_models/models.py
--rw-r--r--   0 runner    (1001) docker     (115)      128 2019-11-30 11:51:38.000000 simpletransformers-0.9.0/simpletransformers/model.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-30 11:51:50.309472 simpletransformers-0.9.0/simpletransformers/ner/
--rw-r--r--   0 runner    (1001) docker     (115)       53 2019-11-30 11:51:38.000000 simpletransformers-0.9.0/simpletransformers/ner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)    23795 2019-11-30 11:51:38.000000 simpletransformers-0.9.0/simpletransformers/ner/ner_model.py
--rw-r--r--   0 runner    (1001) docker     (115)     9017 2019-11-30 11:51:38.000000 simpletransformers-0.9.0/simpletransformers/ner/ner_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-30 11:51:50.309472 simpletransformers-0.9.0/simpletransformers/question_answering/
--rw-r--r--   0 runner    (1001) docker     (115)       97 2019-11-30 11:51:38.000000 simpletransformers-0.9.0/simpletransformers/question_answering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)    27448 2019-11-30 11:51:38.000000 simpletransformers-0.9.0/simpletransformers/question_answering/question_answering_model.py
--rw-r--r--   0 runner    (1001) docker     (115)    61780 2019-11-30 11:51:38.000000 simpletransformers-0.9.0/simpletransformers/question_answering/question_answering_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-30 11:51:50.309472 simpletransformers-0.9.0/simpletransformers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (115)    49993 2019-11-30 11:51:50.000000 simpletransformers-0.9.0/simpletransformers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (115)     1445 2019-11-30 11:51:50.000000 simpletransformers-0.9.0/simpletransformers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (115)        1 2019-11-30 11:51:50.000000 simpletransformers-0.9.0/simpletransformers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (115)       79 2019-11-30 11:51:50.000000 simpletransformers-0.9.0/simpletransformers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (115)       19 2019-11-30 11:51:50.000000 simpletransformers-0.9.0/simpletransformers.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-30 13:18:30.647469 simpletransformers-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (115)    49993 2019-11-30 13:18:30.647469 simpletransformers-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (115)    42061 2019-11-30 13:18:18.000000 simpletransformers-0.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (115)       38 2019-11-30 13:18:30.647469 simpletransformers-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (115)      996 2019-11-30 13:18:18.000000 simpletransformers-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-30 13:18:30.643469 simpletransformers-0.9.1/simpletransformers/
+-rw-r--r--   0 runner    (1001) docker     (115)       27 2019-11-30 13:18:18.000000 simpletransformers-0.9.1/simpletransformers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-30 13:18:30.647469 simpletransformers-0.9.1/simpletransformers/classification/
+-rw-r--r--   0 runner    (1001) docker     (115)      195 2019-11-30 13:18:18.000000 simpletransformers-0.9.1/simpletransformers/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)    31107 2019-11-30 13:18:18.000000 simpletransformers-0.9.1/simpletransformers/classification/classification_model.py
+-rw-r--r--   0 runner    (1001) docker     (115)    13290 2019-11-30 13:18:18.000000 simpletransformers-0.9.1/simpletransformers/classification/classification_utils.py
+-rw-r--r--   0 runner    (1001) docker     (115)     5884 2019-11-30 13:18:18.000000 simpletransformers-0.9.1/simpletransformers/classification/multi_label_classification_model.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-30 13:18:30.647469 simpletransformers-0.9.1/simpletransformers/classification/transformer_models/
+-rw-r--r--   0 runner    (1001) docker     (115)        0 2019-11-30 13:18:18.000000 simpletransformers-0.9.1/simpletransformers/classification/transformer_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)     4769 2019-11-30 13:18:18.000000 simpletransformers-0.9.1/simpletransformers/classification/transformer_models/albert_model.py
+-rw-r--r--   0 runner    (1001) docker     (115)     4740 2019-11-30 13:18:18.000000 simpletransformers-0.9.1/simpletransformers/classification/transformer_models/bert_model.py
+-rw-r--r--   0 runner    (1001) docker     (115)     4771 2019-11-30 13:18:18.000000 simpletransformers-0.9.1/simpletransformers/classification/transformer_models/camembert_model.py
+-rw-r--r--   0 runner    (1001) docker     (115)     4025 2019-11-30 13:18:18.000000 simpletransformers-0.9.1/simpletransformers/classification/transformer_models/distilbert_model.py
+-rw-r--r--   0 runner    (1001) docker     (115)     4733 2019-11-30 13:18:18.000000 simpletransformers-0.9.1/simpletransformers/classification/transformer_models/roberta_model.py
+-rw-r--r--   0 runner    (1001) docker     (115)     3962 2019-11-30 13:18:18.000000 simpletransformers-0.9.1/simpletransformers/classification/transformer_models/xlm_model.py
+-rw-r--r--   0 runner    (1001) docker     (115)     5818 2019-11-30 13:18:18.000000 simpletransformers-0.9.1/simpletransformers/classification/transformer_models/xlnet_model.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-30 13:18:30.647469 simpletransformers-0.9.1/simpletransformers/custom_models/
+-rw-r--r--   0 runner    (1001) docker     (115)        0 2019-11-30 13:18:18.000000 simpletransformers-0.9.1/simpletransformers/custom_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)    13080 2019-11-30 13:18:18.000000 simpletransformers-0.9.1/simpletransformers/custom_models/models.py
+-rw-r--r--   0 runner    (1001) docker     (115)      128 2019-11-30 13:18:18.000000 simpletransformers-0.9.1/simpletransformers/model.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-30 13:18:30.647469 simpletransformers-0.9.1/simpletransformers/ner/
+-rw-r--r--   0 runner    (1001) docker     (115)       53 2019-11-30 13:18:18.000000 simpletransformers-0.9.1/simpletransformers/ner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)    23795 2019-11-30 13:18:18.000000 simpletransformers-0.9.1/simpletransformers/ner/ner_model.py
+-rw-r--r--   0 runner    (1001) docker     (115)     9017 2019-11-30 13:18:18.000000 simpletransformers-0.9.1/simpletransformers/ner/ner_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-30 13:18:30.647469 simpletransformers-0.9.1/simpletransformers/question_answering/
+-rw-r--r--   0 runner    (1001) docker     (115)       97 2019-11-30 13:18:18.000000 simpletransformers-0.9.1/simpletransformers/question_answering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)    27448 2019-11-30 13:18:18.000000 simpletransformers-0.9.1/simpletransformers/question_answering/question_answering_model.py
+-rw-r--r--   0 runner    (1001) docker     (115)    61780 2019-11-30 13:18:18.000000 simpletransformers-0.9.1/simpletransformers/question_answering/question_answering_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-30 13:18:30.643469 simpletransformers-0.9.1/simpletransformers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (115)    49993 2019-11-30 13:18:30.000000 simpletransformers-0.9.1/simpletransformers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (115)     1445 2019-11-30 13:18:30.000000 simpletransformers-0.9.1/simpletransformers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (115)        1 2019-11-30 13:18:30.000000 simpletransformers-0.9.1/simpletransformers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (115)       79 2019-11-30 13:18:30.000000 simpletransformers-0.9.1/simpletransformers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (115)       19 2019-11-30 13:18:30.000000 simpletransformers-0.9.1/simpletransformers.egg-info/top_level.txt
```

### Comparing `simpletransformers-0.9.0/PKG-INFO` & `simpletransformers-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simpletransformers
-Version: 0.9.0
+Version: 0.9.1
 Summary: An easy-to-use wrapper library for the Transformers library.
 Home-page: https://test.pypi.org/legacy/
 Author: Thilina Rajapakse
 Author-email: chaturangarajapakshe@gmail.com
 License: UNKNOWN
 Description: [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0) [![Downloads](https://pepy.tech/badge/simpletransformers)](https://pepy.tech/project/simpletransformers)
```

### Comparing `simpletransformers-0.9.0/README.md` & `simpletransformers-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `simpletransformers-0.9.0/setup.py` & `simpletransformers-0.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="simpletransformers",
-    version="0.9.0",
+    version="0.9.1",
     author="Thilina Rajapakse",
     author_email="chaturangarajapakshe@gmail.com",
     description="An easy-to-use wrapper library for the Transformers library.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://test.pypi.org/legacy/",
     packages=find_packages(),
```

### Comparing `simpletransformers-0.9.0/simpletransformers/classification/classification_model.py` & `simpletransformers-0.9.1/simpletransformers/classification/classification_model.py`

 * *Files identical despite different names*

### Comparing `simpletransformers-0.9.0/simpletransformers/classification/classification_utils.py` & `simpletransformers-0.9.1/simpletransformers/classification/classification_utils.py`

 * *Files identical despite different names*

### Comparing `simpletransformers-0.9.0/simpletransformers/classification/multi_label_classification_model.py` & `simpletransformers-0.9.1/simpletransformers/classification/multi_label_classification_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,15 @@
             'albert':     (AlbertConfig, AlbertForMultiLabelSequenceClassification, AlbertTokenizer)
         }
 
         config_class, model_class, tokenizer_class = MODEL_CLASSES[model_type]
         self.tokenizer = tokenizer_class.from_pretrained(model_name)
         self.num_labels = num_labels
         self.pos_weight = pos_weight
+        self.sliding_window = False
 
         if use_cuda:
             if torch.cuda.is_available():
                 self.device = torch.device("cuda")
             else:
                 raise ValueError("'use_cuda' set to True when cuda is unavailable. Make sure CUDA is available or set use_cuda=False.")
         else:
@@ -77,14 +78,16 @@
             'weight_decay': 0,
             'learning_rate': 4e-5,
             'adam_epsilon': 1e-8,
             'warmup_ratio': 0.06,
             'warmup_steps': 0,
             'max_grad_norm': 1.0,
 
+            'stride': False,
+
             'logging_steps': 50,
             'save_steps': 2000,
             'evaluate_during_training': False,
 
             'overwrite_output_dir': False,
             'reprocess_input_data': False,
```

### Comparing `simpletransformers-0.9.0/simpletransformers/classification/transformer_models/albert_model.py` & `simpletransformers-0.9.1/simpletransformers/classification/transformer_models/albert_model.py`

 * *Files identical despite different names*

### Comparing `simpletransformers-0.9.0/simpletransformers/classification/transformer_models/bert_model.py` & `simpletransformers-0.9.1/simpletransformers/classification/transformer_models/bert_model.py`

 * *Files identical despite different names*

### Comparing `simpletransformers-0.9.0/simpletransformers/classification/transformer_models/camembert_model.py` & `simpletransformers-0.9.1/simpletransformers/classification/transformer_models/camembert_model.py`

 * *Files identical despite different names*

### Comparing `simpletransformers-0.9.0/simpletransformers/classification/transformer_models/distilbert_model.py` & `simpletransformers-0.9.1/simpletransformers/classification/transformer_models/distilbert_model.py`

 * *Files identical despite different names*

### Comparing `simpletransformers-0.9.0/simpletransformers/classification/transformer_models/roberta_model.py` & `simpletransformers-0.9.1/simpletransformers/classification/transformer_models/roberta_model.py`

 * *Files identical despite different names*

### Comparing `simpletransformers-0.9.0/simpletransformers/classification/transformer_models/xlm_model.py` & `simpletransformers-0.9.1/simpletransformers/classification/transformer_models/xlm_model.py`

 * *Files identical despite different names*

### Comparing `simpletransformers-0.9.0/simpletransformers/classification/transformer_models/xlnet_model.py` & `simpletransformers-0.9.1/simpletransformers/classification/transformer_models/xlnet_model.py`

 * *Files identical despite different names*

### Comparing `simpletransformers-0.9.0/simpletransformers/custom_models/models.py` & `simpletransformers-0.9.1/simpletransformers/custom_models/models.py`

 * *Files identical despite different names*

### Comparing `simpletransformers-0.9.0/simpletransformers/ner/ner_model.py` & `simpletransformers-0.9.1/simpletransformers/ner/ner_model.py`

 * *Files identical despite different names*

### Comparing `simpletransformers-0.9.0/simpletransformers/ner/ner_utils.py` & `simpletransformers-0.9.1/simpletransformers/ner/ner_utils.py`

 * *Files identical despite different names*

### Comparing `simpletransformers-0.9.0/simpletransformers/question_answering/question_answering_model.py` & `simpletransformers-0.9.1/simpletransformers/question_answering/question_answering_model.py`

 * *Files identical despite different names*

### Comparing `simpletransformers-0.9.0/simpletransformers/question_answering/question_answering_utils.py` & `simpletransformers-0.9.1/simpletransformers/question_answering/question_answering_utils.py`

 * *Files identical despite different names*

### Comparing `simpletransformers-0.9.0/simpletransformers.egg-info/PKG-INFO` & `simpletransformers-0.9.1/simpletransformers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simpletransformers
-Version: 0.9.0
+Version: 0.9.1
 Summary: An easy-to-use wrapper library for the Transformers library.
 Home-page: https://test.pypi.org/legacy/
 Author: Thilina Rajapakse
 Author-email: chaturangarajapakshe@gmail.com
 License: UNKNOWN
 Description: [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0) [![Downloads](https://pepy.tech/badge/simpletransformers)](https://pepy.tech/project/simpletransformers)
```

### Comparing `simpletransformers-0.9.0/simpletransformers.egg-info/SOURCES.txt` & `simpletransformers-0.9.1/simpletransformers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

