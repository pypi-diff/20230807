# Comparing `tmp/JanexPT-0.0.4.tar.gz` & `tmp/JanexPT-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JanexPT-0.0.4.tar", last modified: Sun Aug  6 13:13:27 2023, max compression
+gzip compressed data, was "JanexPT-0.0.5.tar", last modified: Mon Aug  7 19:53:22 2023, max compression
```

## Comparing `JanexPT-0.0.4.tar` & `JanexPT-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-08-06 13:13:27.377815 JanexPT-0.0.4/
-drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-08-06 13:13:27.377815 JanexPT-0.0.4/JanexPT/
-drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-08-06 13:13:27.377815 JanexPT-0.0.4/JanexPT/JanexSub/
--rw-r--r--   0 cipher    (1000) cipher    (1000)        0 2023-08-05 14:49:33.000000 JanexPT-0.0.4/JanexPT/JanexSub/JanexSub.py
--rw-r--r--   0 cipher    (1000) cipher    (1000)        0 2023-08-05 14:49:33.000000 JanexPT-0.0.4/JanexPT/JanexSub/__init__.py
--rw-r--r--   0 cipher    (1000) cipher    (1000)       20 2023-08-05 15:15:17.000000 JanexPT-0.0.4/JanexPT/__init__.py
--rw-r--r--   0 cipher    (1000) cipher    (1000)      252 2023-08-05 15:58:06.000000 JanexPT-0.0.4/JanexPT/chat.py
--rw-r--r--   0 cipher    (1000) cipher    (1000)     3998 2023-08-06 12:48:21.000000 JanexPT-0.0.4/JanexPT/main.py
--rw-r--r--   0 cipher    (1000) cipher    (1000)     4414 2023-08-06 12:38:40.000000 JanexPT-0.0.4/JanexPT/train.py
-drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-08-06 13:13:27.377815 JanexPT-0.0.4/JanexPT.egg-info/
--rw-r--r--   0 cipher    (1000) cipher    (1000)     1892 2023-08-06 13:13:27.000000 JanexPT-0.0.4/JanexPT.egg-info/PKG-INFO
--rw-r--r--   0 cipher    (1000) cipher    (1000)      307 2023-08-06 13:13:27.000000 JanexPT-0.0.4/JanexPT.egg-info/SOURCES.txt
--rw-r--r--   0 cipher    (1000) cipher    (1000)        1 2023-08-06 13:13:27.000000 JanexPT-0.0.4/JanexPT.egg-info/dependency_links.txt
--rw-r--r--   0 cipher    (1000) cipher    (1000)       17 2023-08-06 13:13:27.000000 JanexPT-0.0.4/JanexPT.egg-info/requires.txt
--rw-r--r--   0 cipher    (1000) cipher    (1000)        8 2023-08-06 13:13:27.000000 JanexPT-0.0.4/JanexPT.egg-info/top_level.txt
--rw-r--r--   0 cipher    (1000) cipher    (1000)     2930 2023-08-05 14:49:33.000000 JanexPT-0.0.4/LICENSE
--rw-r--r--   0 cipher    (1000) cipher    (1000)     1892 2023-08-06 13:13:27.377815 JanexPT-0.0.4/PKG-INFO
--rw-r--r--   0 cipher    (1000) cipher    (1000)     1500 2023-08-05 16:10:30.000000 JanexPT-0.0.4/README.md
--rw-r--r--   0 cipher    (1000) cipher    (1000)       38 2023-08-06 13:13:27.377815 JanexPT-0.0.4/setup.cfg
--rw-r--r--   0 cipher    (1000) cipher    (1000)     1320 2023-08-06 13:13:02.000000 JanexPT-0.0.4/setup.py
+drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-08-07 19:53:22.836290 JanexPT-0.0.5/
+drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-08-07 19:53:22.832290 JanexPT-0.0.5/JanexPT/
+drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-08-07 19:53:22.832290 JanexPT-0.0.5/JanexPT/JanexSub/
+-rw-r--r--   0 cipher    (1000) cipher    (1000)        0 2023-08-07 14:45:22.000000 JanexPT-0.0.5/JanexPT/JanexSub/JanexSub.py
+-rw-r--r--   0 cipher    (1000) cipher    (1000)        0 2023-08-07 14:45:22.000000 JanexPT-0.0.5/JanexPT/JanexSub/__init__.py
+-rw-r--r--   0 cipher    (1000) cipher    (1000)       20 2023-08-07 14:45:22.000000 JanexPT-0.0.5/JanexPT/__init__.py
+-rw-r--r--   0 cipher    (1000) cipher    (1000)      252 2023-08-07 14:45:22.000000 JanexPT-0.0.5/JanexPT/chat.py
+-rw-r--r--   0 cipher    (1000) cipher    (1000)     3831 2023-08-07 19:51:20.000000 JanexPT-0.0.5/JanexPT/main.py
+-rw-r--r--   0 cipher    (1000) cipher    (1000)     4414 2023-08-07 14:45:22.000000 JanexPT-0.0.5/JanexPT/train.py
+drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-08-07 19:53:22.832290 JanexPT-0.0.5/JanexPT.egg-info/
+-rw-r--r--   0 cipher    (1000) cipher    (1000)     1972 2023-08-07 19:53:22.000000 JanexPT-0.0.5/JanexPT.egg-info/PKG-INFO
+-rw-r--r--   0 cipher    (1000) cipher    (1000)      307 2023-08-07 19:53:22.000000 JanexPT-0.0.5/JanexPT.egg-info/SOURCES.txt
+-rw-r--r--   0 cipher    (1000) cipher    (1000)        1 2023-08-07 19:53:22.000000 JanexPT-0.0.5/JanexPT.egg-info/dependency_links.txt
+-rw-r--r--   0 cipher    (1000) cipher    (1000)       20 2023-08-07 19:53:22.000000 JanexPT-0.0.5/JanexPT.egg-info/requires.txt
+-rw-r--r--   0 cipher    (1000) cipher    (1000)        8 2023-08-07 19:53:22.000000 JanexPT-0.0.5/JanexPT.egg-info/top_level.txt
+-rw-r--r--   0 cipher    (1000) cipher    (1000)     2930 2023-08-07 14:45:22.000000 JanexPT-0.0.5/LICENSE
+-rw-r--r--   0 cipher    (1000) cipher    (1000)     1972 2023-08-07 19:53:22.836290 JanexPT-0.0.5/PKG-INFO
+-rw-r--r--   0 cipher    (1000) cipher    (1000)     1580 2023-08-07 19:52:47.000000 JanexPT-0.0.5/README.md
+-rw-r--r--   0 cipher    (1000) cipher    (1000)       38 2023-08-07 19:53:22.836290 JanexPT-0.0.5/setup.cfg
+-rw-r--r--   0 cipher    (1000) cipher    (1000)     1312 2023-08-07 19:53:10.000000 JanexPT-0.0.5/setup.py
```

### Comparing `JanexPT-0.0.4/JanexPT/main.py` & `JanexPT-0.0.5/JanexPT/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,22 +12,17 @@
 import random
 import json
 
 import torch
 import torch.nn as nn
 from torch.utils.data import Dataset, DataLoader
 
-IM = IntentMatcher("intents.json", "thesaurus.json")
-
-def tokenize(sentence):
-    input_string = sentence
-    return IM.tokenize(input_string)
 
 def stem(word):
-    return IM.stem(word.lower())
+    return stemmer.stem(word.lower())
 
 def bag_of_words(tokenized_sentence, words):
     # stem each word
     sentence_words = [stem(word) for word in tokenized_sentence]
     # initialize bag with 0 for each word
     bag = np.zeros(len(words), dtype=np.float32)
     for idx, w in enumerate(words):
@@ -69,32 +64,28 @@
         return self.n_samples
 
 class JanexPT:
     def __init__(self, intents_file_path, thesaurus_file_path, UIName):
         self.intents_file_path = intents_file_path
         self.thesaurus_file_path = thesaurus_file_path
         self.FILE = "data.pth"
-        try:
-            self.data = torch.load(self.FILE)
-        except:
-            self.trainpt()
-            self.data = torch.load(self.FILE)
+        self.data = torch.load(self.FILE)
         self.device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')
         self.input_size = self.data["input_size"]
         self.hidden_size = self.data["hidden_size"]
         self.output_size = self.data["output_size"]
         self.all_words = self.data['all_words']
         self.tags = self.data['tags']
         self.model_state = self.data["model_state"]
         self.model = NeuralNet(self.input_size, self.hidden_size, self.output_size).to(self.device)
         self.UIName = UIName
         self.IntentMatcher = IntentMatcher(intents_file_path, thesaurus_file_path)
         self.intents = self.IntentMatcher.train()
 
-    def SayToAI(self, input_string, user):
+    def pattern_compare(self, input_string, user):
         self.model.load_state_dict(self.model_state)
         self.model.eval()
         sentence = input_string
 
         sentence = self.IntentMatcher.tokenize(sentence)
 
         X = bag_of_words(sentence, self.all_words)
@@ -107,17 +98,20 @@
         tag = self.tags[predicted.item()]
 
         probs = torch.softmax(output, dim=1)
         probs = probs[0][predicted.item()]
 
         for intent in self.intents['intents']:
             if tag == intent["tag"]:
-                print(tag)
-                BestResponse = self.IntentMatcher.response_compare(input_string, intent)
-                return BestResponse
+                return intent
+
+    def response_compare(self, input_string, classification):
+        print(tag)
+        BestResponse = self.IntentMatcher.response_compare(input_string, intent)
+        return BestResponse
 
     def trainpt(self):
         try:
             open("train.py", "r")
             os.system("python3 train.py")
         except:
             print("Janex-PyTorch: Train program not detected, downloading from Github.")
```

### Comparing `JanexPT-0.0.4/JanexPT/train.py` & `JanexPT-0.0.5/JanexPT/train.py`

 * *Files identical despite different names*

### Comparing `JanexPT-0.0.4/JanexPT.egg-info/PKG-INFO` & `JanexPT-0.0.5/JanexPT.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JanexPT
-Version: 0.0.4
+Version: 0.0.5
 Home-page: https://github.com/Cipher58/Janex-Pytorch
 Download-URL: https://github.com/Cipher58/Janex-Pytorch
 Author: Cipher58
 Author-email: cipher58public@gmail.com
 License: Lily 1.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -40,13 +40,14 @@
 ```
 
 Next, you need to give the program some text you wish to send to your AI, and then send it.
 ```
 YourInput = input("You: ")
 YourName = "Bob" # Whatever you wish your AI to refer to you as
 
-Response = JanexPT.SayToAI(YourInput, YourName)
+classification = JanexPT.pattern_compare(YourInput, YourName)
+response = JanexPT.response_compare(input_string, classification)
 
-print(Response)
+print(response)
 ```
 
 And there we have it, the code will use a NeuralNet to predict which class your input belongs in, and then uses the Janex library to pick the best response from those available.
```

### Comparing `JanexPT-0.0.4/LICENSE` & `JanexPT-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `JanexPT-0.0.4/PKG-INFO` & `JanexPT-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JanexPT
-Version: 0.0.4
+Version: 0.0.5
 Home-page: https://github.com/Cipher58/Janex-Pytorch
 Download-URL: https://github.com/Cipher58/Janex-Pytorch
 Author: Cipher58
 Author-email: cipher58public@gmail.com
 License: Lily 1.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -40,13 +40,14 @@
 ```
 
 Next, you need to give the program some text you wish to send to your AI, and then send it.
 ```
 YourInput = input("You: ")
 YourName = "Bob" # Whatever you wish your AI to refer to you as
 
-Response = JanexPT.SayToAI(YourInput, YourName)
+classification = JanexPT.pattern_compare(YourInput, YourName)
+response = JanexPT.response_compare(input_string, classification)
 
-print(Response)
+print(response)
 ```
 
 And there we have it, the code will use a NeuralNet to predict which class your input belongs in, and then uses the Janex library to pick the best response from those available.
```

### Comparing `JanexPT-0.0.4/README.md` & `JanexPT-0.0.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -27,13 +27,14 @@
 ```
 
 Next, you need to give the program some text you wish to send to your AI, and then send it.
 ```
 YourInput = input("You: ")
 YourName = "Bob" # Whatever you wish your AI to refer to you as
 
-Response = JanexPT.SayToAI(YourInput, YourName)
+classification = JanexPT.pattern_compare(YourInput, YourName)
+response = JanexPT.response_compare(input_string, classification)
 
-print(Response)
+print(response)
 ```
 
 And there we have it, the code will use a NeuralNet to predict which class your input belongs in, and then uses the Janex library to pick the best response from those available.
```

### Comparing `JanexPT-0.0.4/setup.py` & `JanexPT-0.0.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 setuptools.setup(
     # Here is the module name.
     name="JanexPT",
 
     # version of the module
-    version="0.0.4",
+    version="0.0.5",
 
     # Name of Author
     author="Cipher58",
 
     download_url = 'https://github.com/Cipher58/Janex-Pytorch',
 
     # your Email address
@@ -33,17 +33,16 @@
     packages=setuptools.find_packages(),
 
 
     #if module has dependencies i.e. if your package rely on other package at pypi.org
     # then you must add there, in order to download every requirement of package
 
     install_requires=[
-        "Janex",
+        "CipherProgram",
         "torch",
-        "nltk",
         ],
 
 
     license="Lily 1.0",
 
     # classifiers like program is suitable for python3, just leave as it is.
     classifiers=[
```

