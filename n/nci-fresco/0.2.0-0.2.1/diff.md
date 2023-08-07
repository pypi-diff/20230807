# Comparing `tmp/nci-fresco-0.2.0.tar.gz` & `tmp/nci-fresco-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nci-fresco-0.2.0.tar", last modified: Fri Aug  4 05:20:22 2023, max compression
+gzip compressed data, was "nci-fresco-0.2.1.tar", last modified: Mon Aug  7 15:09:16 2023, max compression
```

## Comparing `nci-fresco-0.2.0.tar` & `nci-fresco-0.2.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 z6f      (1428799531) ORNL\Domain Users (1551083765)        0 2023-08-04 05:20:22.398542 nci-fresco-0.2.0/
--rw-r--r--   0 z6f      (1428799531) ORNL\Domain Users (1551083765)     1064 2023-08-04 05:10:10.000000 nci-fresco-0.2.0/LICENSE
--rw-r--r--   0 z6f      (1428799531) ORNL\Domain Users (1551083765)      396 2023-08-04 05:20:22.398405 nci-fresco-0.2.0/PKG-INFO
--rw-r--r--   0 z6f      (1428799531) ORNL\Domain Users (1551083765)    12322 2023-08-04 05:10:10.000000 nci-fresco-0.2.0/README.md
-drwxr-xr-x   0 z6f      (1428799531) ORNL\Domain Users (1551083765)        0 2023-08-04 05:20:22.395608 nci-fresco-0.2.0/fresco/
--rw-r--r--   0 z6f      (1428799531) ORNL\Domain Users (1551083765)        0 2023-08-04 05:10:11.000000 nci-fresco-0.2.0/fresco/__init__.py
-drwxr-xr-x   0 z6f      (1428799531) ORNL\Domain Users (1551083765)        0 2023-08-04 05:20:22.395886 nci-fresco-0.2.0/fresco/abstention/
--rw-r--r--   0 z6f      (1428799531) ORNL\Domain Users (1551083765)        0 2023-08-04 05:10:11.000000 nci-fresco-0.2.0/fresco/abstention/__init__.py
--rw-r--r--   0 z6f      (1428799531) ORNL\Domain Users (1551083765)    20048 2023-08-04 05:10:11.000000 nci-fresco-0.2.0/fresco/abstention/abstention.py
-drwxr-xr-x   0 z6f      (1428799531) ORNL\Domain Users (1551083765)        0 2023-08-04 05:20:22.396173 nci-fresco-0.2.0/fresco/data_loaders/
--rw-r--r--   0 z6f      (1428799531) ORNL\Domain Users (1551083765)        0 2023-08-04 05:10:11.000000 nci-fresco-0.2.0/fresco/data_loaders/__init__.py
--rw-r--r--   0 z6f      (1428799531) ORNL\Domain Users (1551083765)    28779 2023-08-04 05:10:11.000000 nci-fresco-0.2.0/fresco/data_loaders/data_utils.py
-drwxr-xr-x   0 z6f      (1428799531) ORNL\Domain Users (1551083765)        0 2023-08-04 05:20:22.396716 nci-fresco-0.2.0/fresco/models/
--rw-r--r--   0 z6f      (1428799531) ORNL\Domain Users (1551083765)        0 2023-08-04 05:10:11.000000 nci-fresco-0.2.0/fresco/models/__init__.py
--rw-r--r--   0 z6f      (1428799531) ORNL\Domain Users (1551083765)     6462 2023-08-04 05:10:11.000000 nci-fresco-0.2.0/fresco/models/clc.py
--rw-r--r--   0 z6f      (1428799531) ORNL\Domain Users (1551083765)     5042 2023-08-04 05:10:11.000000 nci-fresco-0.2.0/fresco/models/mtcnn.py
--rw-r--r--   0 z6f      (1428799531) ORNL\Domain Users (1551083765)    15786 2023-08-04 05:10:11.000000 nci-fresco-0.2.0/fresco/models/mthisan.py
-drwxr-xr-x   0 z6f      (1428799531) ORNL\Domain Users (1551083765)        0 2023-08-04 05:20:22.396939 nci-fresco-0.2.0/fresco/predict/
--rw-r--r--   0 z6f      (1428799531) ORNL\Domain Users (1551083765)        0 2023-08-04 05:10:11.000000 nci-fresco-0.2.0/fresco/predict/__init__.py
--rwxr-xr-x   0 z6f      (1428799531) ORNL\Domain Users (1551083765)    32084 2023-08-04 05:10:11.000000 nci-fresco-0.2.0/fresco/predict/predictions.py
--rw-r--r--   0 z6f      (1428799531) ORNL\Domain Users (1551083765)    11513 2023-08-04 05:10:11.000000 nci-fresco-0.2.0/fresco/run_clc.py
--rw-r--r--   0 z6f      (1428799531) ORNL\Domain Users (1551083765)     8957 2023-08-04 05:10:11.000000 nci-fresco-0.2.0/fresco/run_ie.py
-drwxr-xr-x   0 z6f      (1428799531) ORNL\Domain Users (1551083765)        0 2023-08-04 05:20:22.397222 nci-fresco-0.2.0/fresco/training/
--rw-r--r--   0 z6f      (1428799531) ORNL\Domain Users (1551083765)        0 2023-08-04 05:10:11.000000 nci-fresco-0.2.0/fresco/training/__init__.py
--rwxr-xr-x   0 z6f      (1428799531) ORNL\Domain Users (1551083765)    33164 2023-08-04 05:10:11.000000 nci-fresco-0.2.0/fresco/training/training.py
-drwxr-xr-x   0 z6f      (1428799531) ORNL\Domain Users (1551083765)        0 2023-08-04 05:20:22.397635 nci-fresco-0.2.0/fresco/validate/
--rw-r--r--   0 z6f      (1428799531) ORNL\Domain Users (1551083765)        0 2023-08-04 05:10:11.000000 nci-fresco-0.2.0/fresco/validate/__init__.py
--rw-r--r--   0 z6f      (1428799531) ORNL\Domain Users (1551083765)      365 2023-08-04 05:10:11.000000 nci-fresco-0.2.0/fresco/validate/exceptions.py
--rw-r--r--   0 z6f      (1428799531) ORNL\Domain Users (1551083765)    23160 2023-08-04 05:10:11.000000 nci-fresco-0.2.0/fresco/validate/validate_params.py
-drwxr-xr-x   0 z6f      (1428799531) ORNL\Domain Users (1551083765)        0 2023-08-04 05:20:22.398244 nci-fresco-0.2.0/nci_fresco.egg-info/
--rw-r--r--   0 z6f      (1428799531) ORNL\Domain Users (1551083765)      396 2023-08-04 05:20:22.000000 nci-fresco-0.2.0/nci_fresco.egg-info/PKG-INFO
--rw-r--r--   0 z6f      (1428799531) ORNL\Domain Users (1551083765)      678 2023-08-04 05:20:22.000000 nci-fresco-0.2.0/nci_fresco.egg-info/SOURCES.txt
--rw-r--r--   0 z6f      (1428799531) ORNL\Domain Users (1551083765)        1 2023-08-04 05:20:22.000000 nci-fresco-0.2.0/nci_fresco.egg-info/dependency_links.txt
--rw-r--r--   0 z6f      (1428799531) ORNL\Domain Users (1551083765)       64 2023-08-04 05:20:22.000000 nci-fresco-0.2.0/nci_fresco.egg-info/requires.txt
--rw-r--r--   0 z6f      (1428799531) ORNL\Domain Users (1551083765)        7 2023-08-04 05:20:22.000000 nci-fresco-0.2.0/nci_fresco.egg-info/top_level.txt
--rw-r--r--   0 z6f      (1428799531) ORNL\Domain Users (1551083765)       38 2023-08-04 05:20:22.398590 nci-fresco-0.2.0/setup.cfg
--rw-r--r--   0 z6f      (1428799531) ORNL\Domain Users (1551083765)      942 2023-08-04 05:20:06.000000 nci-fresco-0.2.0/setup.py
+drwxr-xr-x   0 z6f      (1428799531) ORNL\Domain Users (1551083765)        0 2023-08-07 15:09:16.813490 nci-fresco-0.2.1/
+-rw-r--r--   0 z6f      (1428799531) ORNL\Domain Users (1551083765)     1064 2023-08-07 15:05:52.000000 nci-fresco-0.2.1/LICENSE
+-rw-r--r--   0 z6f      (1428799531) ORNL\Domain Users (1551083765)      396 2023-08-07 15:09:16.813356 nci-fresco-0.2.1/PKG-INFO
+-rw-r--r--   0 z6f      (1428799531) ORNL\Domain Users (1551083765)    12322 2023-08-07 15:05:52.000000 nci-fresco-0.2.1/README.md
+drwxr-xr-x   0 z6f      (1428799531) ORNL\Domain Users (1551083765)        0 2023-08-07 15:09:16.810837 nci-fresco-0.2.1/fresco/
+-rw-r--r--   0 z6f      (1428799531) ORNL\Domain Users (1551083765)        0 2023-08-07 15:05:52.000000 nci-fresco-0.2.1/fresco/__init__.py
+drwxr-xr-x   0 z6f      (1428799531) ORNL\Domain Users (1551083765)        0 2023-08-07 15:09:16.811074 nci-fresco-0.2.1/fresco/abstention/
+-rw-r--r--   0 z6f      (1428799531) ORNL\Domain Users (1551083765)        0 2023-08-07 15:05:52.000000 nci-fresco-0.2.1/fresco/abstention/__init__.py
+-rw-r--r--   0 z6f      (1428799531) ORNL\Domain Users (1551083765)    20048 2023-08-07 15:05:52.000000 nci-fresco-0.2.1/fresco/abstention/abstention.py
+drwxr-xr-x   0 z6f      (1428799531) ORNL\Domain Users (1551083765)        0 2023-08-07 15:09:16.811309 nci-fresco-0.2.1/fresco/data_loaders/
+-rw-r--r--   0 z6f      (1428799531) ORNL\Domain Users (1551083765)        0 2023-08-07 15:05:52.000000 nci-fresco-0.2.1/fresco/data_loaders/__init__.py
+-rw-r--r--   0 z6f      (1428799531) ORNL\Domain Users (1551083765)    29521 2023-08-07 15:05:52.000000 nci-fresco-0.2.1/fresco/data_loaders/data_utils.py
+drwxr-xr-x   0 z6f      (1428799531) ORNL\Domain Users (1551083765)        0 2023-08-07 15:09:16.811779 nci-fresco-0.2.1/fresco/models/
+-rw-r--r--   0 z6f      (1428799531) ORNL\Domain Users (1551083765)        0 2023-08-07 15:05:52.000000 nci-fresco-0.2.1/fresco/models/__init__.py
+-rw-r--r--   0 z6f      (1428799531) ORNL\Domain Users (1551083765)     6462 2023-08-07 15:05:52.000000 nci-fresco-0.2.1/fresco/models/clc.py
+-rw-r--r--   0 z6f      (1428799531) ORNL\Domain Users (1551083765)     5042 2023-08-07 15:05:52.000000 nci-fresco-0.2.1/fresco/models/mtcnn.py
+-rw-r--r--   0 z6f      (1428799531) ORNL\Domain Users (1551083765)    15786 2023-08-07 15:05:52.000000 nci-fresco-0.2.1/fresco/models/mthisan.py
+drwxr-xr-x   0 z6f      (1428799531) ORNL\Domain Users (1551083765)        0 2023-08-07 15:09:16.811983 nci-fresco-0.2.1/fresco/predict/
+-rw-r--r--   0 z6f      (1428799531) ORNL\Domain Users (1551083765)        0 2023-08-07 15:05:52.000000 nci-fresco-0.2.1/fresco/predict/__init__.py
+-rwxr-xr-x   0 z6f      (1428799531) ORNL\Domain Users (1551083765)    31139 2023-08-07 15:05:52.000000 nci-fresco-0.2.1/fresco/predict/predictions.py
+-rw-r--r--   0 z6f      (1428799531) ORNL\Domain Users (1551083765)    11513 2023-08-07 15:05:52.000000 nci-fresco-0.2.1/fresco/run_clc.py
+-rw-r--r--   0 z6f      (1428799531) ORNL\Domain Users (1551083765)     8957 2023-08-07 15:05:52.000000 nci-fresco-0.2.1/fresco/run_ie.py
+drwxr-xr-x   0 z6f      (1428799531) ORNL\Domain Users (1551083765)        0 2023-08-07 15:09:16.812209 nci-fresco-0.2.1/fresco/training/
+-rw-r--r--   0 z6f      (1428799531) ORNL\Domain Users (1551083765)        0 2023-08-07 15:05:52.000000 nci-fresco-0.2.1/fresco/training/__init__.py
+-rwxr-xr-x   0 z6f      (1428799531) ORNL\Domain Users (1551083765)    33225 2023-08-07 15:05:52.000000 nci-fresco-0.2.1/fresco/training/training.py
+drwxr-xr-x   0 z6f      (1428799531) ORNL\Domain Users (1551083765)        0 2023-08-07 15:09:16.812537 nci-fresco-0.2.1/fresco/validate/
+-rw-r--r--   0 z6f      (1428799531) ORNL\Domain Users (1551083765)        0 2023-08-07 15:05:52.000000 nci-fresco-0.2.1/fresco/validate/__init__.py
+-rw-r--r--   0 z6f      (1428799531) ORNL\Domain Users (1551083765)      365 2023-08-07 15:05:52.000000 nci-fresco-0.2.1/fresco/validate/exceptions.py
+-rw-r--r--   0 z6f      (1428799531) ORNL\Domain Users (1551083765)    23160 2023-08-07 15:05:52.000000 nci-fresco-0.2.1/fresco/validate/validate_params.py
+drwxr-xr-x   0 z6f      (1428799531) ORNL\Domain Users (1551083765)        0 2023-08-07 15:09:16.813157 nci-fresco-0.2.1/nci_fresco.egg-info/
+-rw-r--r--   0 z6f      (1428799531) ORNL\Domain Users (1551083765)      396 2023-08-07 15:09:16.000000 nci-fresco-0.2.1/nci_fresco.egg-info/PKG-INFO
+-rw-r--r--   0 z6f      (1428799531) ORNL\Domain Users (1551083765)      678 2023-08-07 15:09:16.000000 nci-fresco-0.2.1/nci_fresco.egg-info/SOURCES.txt
+-rw-r--r--   0 z6f      (1428799531) ORNL\Domain Users (1551083765)        1 2023-08-07 15:09:16.000000 nci-fresco-0.2.1/nci_fresco.egg-info/dependency_links.txt
+-rw-r--r--   0 z6f      (1428799531) ORNL\Domain Users (1551083765)       64 2023-08-07 15:09:16.000000 nci-fresco-0.2.1/nci_fresco.egg-info/requires.txt
+-rw-r--r--   0 z6f      (1428799531) ORNL\Domain Users (1551083765)        7 2023-08-07 15:09:16.000000 nci-fresco-0.2.1/nci_fresco.egg-info/top_level.txt
+-rw-r--r--   0 z6f      (1428799531) ORNL\Domain Users (1551083765)       38 2023-08-07 15:09:16.813534 nci-fresco-0.2.1/setup.cfg
+-rw-r--r--   0 z6f      (1428799531) ORNL\Domain Users (1551083765)      942 2023-08-07 15:09:07.000000 nci-fresco-0.2.1/setup.py
```

### Comparing `nci-fresco-0.2.0/LICENSE` & `nci-fresco-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nci-fresco-0.2.0/README.md` & `nci-fresco-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `nci-fresco-0.2.0/fresco/abstention/abstention.py` & `nci-fresco-0.2.1/fresco/abstention/abstention.py`

 * *Files identical despite different names*

### Comparing `nci-fresco-0.2.0/fresco/data_loaders/data_utils.py` & `nci-fresco-0.2.1/fresco/data_loaders/data_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,24 @@
 
 from torch.utils.data import DataLoader
 from torch.utils.data import Dataset
 
 from fresco.validate import exceptions
 
 
+def word2int(tok, vocab):
+    """Map words to tokens for random embeddings.
+
+        If a word doesn't exist in the training/val split, it is mapped
+        to 'unk', the unknown token.
+
+    """
+    unk = len(vocab)
+    return [x if x is not None else unk for x in tok]
+
 class LabelDict(dict):
     """
     Create dict subclass for correct behaviour when mapping task unks.
     """
     def __init__(self, data, missing):
         super().__init__(data)
         self.data = data
@@ -197,33 +207,39 @@
         else:
             loaded_data['id2word'] = None
 
         return loaded_data
 
     def get_vocab(self):
         """
-        Get the vocab from tokenized data.
+        Get the vocab and word embeddings from tokenized data.
         """
 
         embedding_dim = 300
 
         X = self.inference_data['X']['train']
 
         if 'val' in self.inference_data['X'].keys():
             X = pd.concat([X, self.inference_data['X']['val']])
 
         # find all unique tokens
-        s1 = set(X.iloc[0]).union(X.iloc[1])
-
+        s1 = set(X.iloc[0])
         for x in X:
             s1 = set(x).union(s1)
 
         vocab_len = np.max(list(s1))
+        unk = vocab_len + 1 
+        self.inference_data['X']['test'].apply(lambda d: word2int(d, s1))
         rng = np.random.default_rng(self.model_args['train_kwargs']['random_seed'])
-        self.inference_data['word_embedding'] = rng.standard_normal(size=(vocab_len + 1, embedding_dim), dtype=np.float32) * 0.1
+        unk_embed = rng.normal(size=(1, embedding_dim), scale=0.1)
+        random_embeds = rng.standard_normal(size=(vocab_len, embedding_dim), dtype=np.float32) * 0.1
+        self.inference_data['word_embedding'] = np.concatenate((np.zeros(shape=(1, embedding_dim)),
+                                                                random_embeds,
+                                                                unk_embed),
+                                                                axis=0)
 
     def convert_y(self):
         """
         Add task unknown labels to Y and map values to integers for inference.
 
         Post-condition:
             The data frame with the output, the ys, is modified in place by this function.
```

### Comparing `nci-fresco-0.2.0/fresco/models/clc.py` & `nci-fresco-0.2.1/fresco/models/clc.py`

 * *Files identical despite different names*

### Comparing `nci-fresco-0.2.0/fresco/models/mtcnn.py` & `nci-fresco-0.2.1/fresco/models/mtcnn.py`

 * *Files identical despite different names*

### Comparing `nci-fresco-0.2.0/fresco/models/mthisan.py` & `nci-fresco-0.2.1/fresco/models/mthisan.py`

 * *Files identical despite different names*

### Comparing `nci-fresco-0.2.0/fresco/predict/predictions.py` & `nci-fresco-0.2.1/fresco/predict/predictions.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,16 +9,20 @@
 import time
 import torch
 
 import torch.nn.functional as F
 import numpy as np
 import pandas as pd
 import scipy.special
-import sklearn.metrics
-import torchmetrics
+
+from sklearn.metrics import f1_score
+from sklearn.metrics import accuracy_score
+from sklearn.metrics import precision_score
+from sklearn.metrics import recall_score
+# import torchmetrics
 
 
 class ScoreModel():
     """
     Class to score and make predictions from a trained model.
 
     Args:
@@ -212,44 +216,29 @@
         """
         Compute metrics to evaluate a model.
         """
 
         metrics = {}
         # per task metrics
         for i, task in enumerate(self.tasks):
-            logits = torch.tensor(np.vstack(self.logits[i])).to(self.device)
-            scores = torch.nn.functional.softmax(logits, dim=1)
+            logits = np.vstack(self.logits[i])
+            scores = scipy.special.softmax(logits, axis=-1)
             _trues = [v.item() for v in self.y_trues[task]]
             _preds = [v.item() for v in self.y_preds[task]]
 
-            _trues = torch.tensor(_trues).to(self.device)
-            _preds = torch.tensor(_preds).to(self.device)
-            num_classes = scores.shape[1]
-
-            # macro hack
-            _cat_trues_preds = torch.cat((_trues, _preds), dim=0)
-            scale_classes = num_classes / len(torch.unique(_cat_trues_preds))
-
-            f1_micro = torchmetrics.F1Score(task='multiclass', num_classes=num_classes, average='micro').to(self.device)
-            metrics[f'{task}_micro'] = f1_micro(_preds, _trues)
-            f1_macro = torchmetrics.F1Score(task='multiclass', num_classes=num_classes, average='macro').to(self.device)
-            metrics[f'{task}_macro'] = f1_macro(_preds, _trues) * scale_classes
-
-            accuracy = torchmetrics.Accuracy(task='multiclass', num_classes=num_classes).to(self.device)
-            metrics[f'{task}_accuracy'] = accuracy(_preds, _trues)
-
-            precision_micro = torchmetrics.Precision(task='multiclass', num_classes=num_classes, average='micro').to(self.device)
-            metrics[f'{task}_precision_micro'] = precision_micro(_preds, _trues)
-            precision_macro = torchmetrics.Precision(task='multiclass', num_classes=num_classes, average='macro').to(self.device)
-            metrics[f'{task}_precision_macro'] = precision_macro(_preds, _trues) * scale_classes
-
-            recall_micro = torchmetrics.Recall(task='multiclass', num_classes=num_classes, average='micro').to(self.device)
-            metrics[f'{task}_recall_micro'] = recall_micro(_preds, _trues)
-            recall_macro = torchmetrics.Recall(task='multiclass', num_classes=num_classes, average='macro').to(self.device)
-            metrics[f'{task}_recall_macro'] = recall_macro(_preds, _trues) * scale_classes
+            metrics[f'{task}_micro'] = f1_score(_preds, _trues, average='micro')
+            metrics[f'{task}_macro'] = f1_score(_preds, _trues, average='macro')
+
+            metrics[f'{task}_accuracy'] = accuracy_score(_preds, _trues)
+
+            metrics[f'{task}_precision_micro'] = precision_score(_preds, _trues, average='micro', zero_division=0)
+            metrics[f'{task}_precision_macro'] = precision_score(_preds, _trues, average='macro', zero_division=0)
+
+            metrics[f'{task}_recall_micro'] = recall_score(_preds, _trues, average='micro', zero_division=0)
+            metrics[f'{task}_recall_macro'] = recall_score(_preds, _trues, average='macro', zero_division=0)
 
 
         if self.abstain:
             _ = dac.compute_accuracy(self.y_trues, self.y_preds)
             for i, task in enumerate(self.tasks):
                 metrics[f"{task}_abs_acc"] = dac.accuracy[i]
             for k, v in dac.abs_rates.items():
```

### Comparing `nci-fresco-0.2.0/fresco/run_clc.py` & `nci-fresco-0.2.1/fresco/run_clc.py`

 * *Files identical despite different names*

### Comparing `nci-fresco-0.2.0/fresco/run_ie.py` & `nci-fresco-0.2.1/fresco/run_ie.py`

 * *Files identical despite different names*

### Comparing `nci-fresco-0.2.0/fresco/training/training.py` & `nci-fresco-0.2.1/fresco/training/training.py`

 * *Files 2% similar despite different names*

```diff
@@ -290,35 +290,35 @@
 
             print(f"\nepoch {epoch+1} validation\n", flush=True)
             stop, val_scores = self.score(epoch, val_loader=val_loader, dac=dac)
             all_scores[f'epoch_{epoch}_val_scores'] = val_scores
 
             if val_scores['val_loss'][0] < best_loss:
                 best_loss = val_scores['val_loss'][0]
-                model_weights = self.model.state_dict()
+                torch.save({'epoch': epoch,
+                            'model_state_dict': self.model.state_dict(), 
+                            'opt_state_dict': self.opt.state_dict(),
+                            'val_loss': best_loss
+                            }, self.savename)
 
             if stop:
                 print(f"saving to {self.savename}", flush=True)
-                if model_weights is None:
-                    torch.save(self.model.state_dict(), self.savename)
-                else:
-                    torch.save(model_weights, self.savename)
-                self.model.state_dict = copy.deepcopy(model_weights)
+                # loading weights of best model
+                checkpoint = torch.load(self.savename)
+                self.model.load_state_dict(checkpoint['model_state_dict'])
                 scores = f"epoch_{epoch}_scores_fold{self.fold}_{datetime.datetime.now().strftime('%Y%m%d%H%M%S')}.pkl"
                 with open(self.savepath + scores, "wb") as f_out:
                     pickle.dump(all_scores, f_out, pickle.HIGHEST_PROTOCOL)
                 break
         if epoch + 1 == self.epochs:
             print('\nModel training hit max epochs, not converged')
+            # loading weights of best model
+            checkpoint = torch.load(self.savename)
+            self.model.load_state_dict(checkpoint['model_state_dict'])
             print(f"saving to {self.savename}", flush=True)
-            if model_weights is None:
-                torch.save(self.model.state_dict(), self.savename)
-            else:
-                torch.save(model_weights, self.savename)
-            self.model.state_dict = copy.deepcopy(model_weights)
             scores = f"epoch_{epoch}_scores_fold{self.fold}_{datetime.datetime.now().strftime('%Y%m%d%H%M%S')}.pkl"
             with open(self.savepath + scores, "wb") as f_out:
                 pickle.dump(all_scores, f_out, pickle.HIGHEST_PROTOCOL)
 
     def train_metrics(self, dac=None):
         """
         Compute per-epoch metrics during training.
```

### Comparing `nci-fresco-0.2.0/fresco/validate/validate_params.py` & `nci-fresco-0.2.1/fresco/validate/validate_params.py`

 * *Files identical despite different names*

### Comparing `nci-fresco-0.2.0/nci_fresco.egg-info/SOURCES.txt` & `nci-fresco-0.2.1/nci_fresco.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nci-fresco-0.2.0/setup.py` & `nci-fresco-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='nci-fresco',
-    version='0.2.0',    
+    version='0.2.1',    
     description='',
     url='https://github.com/DOE-NCI-MOSSAIC/FrESCO',
     author='Adam Spannaus',
     author_email='spannausat@ornl.gov',
     license='MIT',
     packages=find_packages(include=['fresco', 'fresco.*']),
     install_requires=[ 'pandas',
```

