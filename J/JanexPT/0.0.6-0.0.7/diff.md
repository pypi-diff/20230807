# Comparing `tmp/JanexPT-0.0.6.tar.gz` & `tmp/JanexPT-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JanexPT-0.0.6.tar", last modified: Mon Aug  7 19:58:02 2023, max compression
+gzip compressed data, was "JanexPT-0.0.7.tar", last modified: Mon Aug  7 19:59:46 2023, max compression
```

## Comparing `JanexPT-0.0.6.tar` & `JanexPT-0.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-08-07 19:58:02.482515 JanexPT-0.0.6/
-drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-08-07 19:58:02.478515 JanexPT-0.0.6/JanexPT/
-drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-08-07 19:58:02.478515 JanexPT-0.0.6/JanexPT/JanexSub/
--rw-r--r--   0 cipher    (1000) cipher    (1000)        0 2023-08-07 14:45:22.000000 JanexPT-0.0.6/JanexPT/JanexSub/JanexSub.py
--rw-r--r--   0 cipher    (1000) cipher    (1000)        0 2023-08-07 14:45:22.000000 JanexPT-0.0.6/JanexPT/JanexSub/__init__.py
--rw-r--r--   0 cipher    (1000) cipher    (1000)       20 2023-08-07 14:45:22.000000 JanexPT-0.0.6/JanexPT/__init__.py
--rw-r--r--   0 cipher    (1000) cipher    (1000)      252 2023-08-07 14:45:22.000000 JanexPT-0.0.6/JanexPT/chat.py
--rw-r--r--   0 cipher    (1000) cipher    (1000)     3853 2023-08-07 19:57:39.000000 JanexPT-0.0.6/JanexPT/main.py
--rw-r--r--   0 cipher    (1000) cipher    (1000)     4414 2023-08-07 14:45:22.000000 JanexPT-0.0.6/JanexPT/train.py
-drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-08-07 19:58:02.478515 JanexPT-0.0.6/JanexPT.egg-info/
--rw-r--r--   0 cipher    (1000) cipher    (1000)     1972 2023-08-07 19:58:02.000000 JanexPT-0.0.6/JanexPT.egg-info/PKG-INFO
--rw-r--r--   0 cipher    (1000) cipher    (1000)      307 2023-08-07 19:58:02.000000 JanexPT-0.0.6/JanexPT.egg-info/SOURCES.txt
--rw-r--r--   0 cipher    (1000) cipher    (1000)        1 2023-08-07 19:58:02.000000 JanexPT-0.0.6/JanexPT.egg-info/dependency_links.txt
--rw-r--r--   0 cipher    (1000) cipher    (1000)       20 2023-08-07 19:58:02.000000 JanexPT-0.0.6/JanexPT.egg-info/requires.txt
--rw-r--r--   0 cipher    (1000) cipher    (1000)        8 2023-08-07 19:58:02.000000 JanexPT-0.0.6/JanexPT.egg-info/top_level.txt
--rw-r--r--   0 cipher    (1000) cipher    (1000)     2930 2023-08-07 14:45:22.000000 JanexPT-0.0.6/LICENSE
--rw-r--r--   0 cipher    (1000) cipher    (1000)     1972 2023-08-07 19:58:02.478515 JanexPT-0.0.6/PKG-INFO
--rw-r--r--   0 cipher    (1000) cipher    (1000)     1580 2023-08-07 19:52:47.000000 JanexPT-0.0.6/README.md
--rw-r--r--   0 cipher    (1000) cipher    (1000)       38 2023-08-07 19:58:02.482515 JanexPT-0.0.6/setup.cfg
--rw-r--r--   0 cipher    (1000) cipher    (1000)     1312 2023-08-07 19:57:44.000000 JanexPT-0.0.6/setup.py
+drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-08-07 19:59:46.353858 JanexPT-0.0.7/
+drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-08-07 19:59:46.349858 JanexPT-0.0.7/JanexPT/
+drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-08-07 19:59:46.353858 JanexPT-0.0.7/JanexPT/JanexSub/
+-rw-r--r--   0 cipher    (1000) cipher    (1000)        0 2023-08-07 14:45:22.000000 JanexPT-0.0.7/JanexPT/JanexSub/JanexSub.py
+-rw-r--r--   0 cipher    (1000) cipher    (1000)        0 2023-08-07 14:45:22.000000 JanexPT-0.0.7/JanexPT/JanexSub/__init__.py
+-rw-r--r--   0 cipher    (1000) cipher    (1000)       20 2023-08-07 14:45:22.000000 JanexPT-0.0.7/JanexPT/__init__.py
+-rw-r--r--   0 cipher    (1000) cipher    (1000)      252 2023-08-07 14:45:22.000000 JanexPT-0.0.7/JanexPT/chat.py
+-rw-r--r--   0 cipher    (1000) cipher    (1000)     3861 2023-08-07 19:59:22.000000 JanexPT-0.0.7/JanexPT/main.py
+-rw-r--r--   0 cipher    (1000) cipher    (1000)     4414 2023-08-07 14:45:22.000000 JanexPT-0.0.7/JanexPT/train.py
+drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-08-07 19:59:46.353858 JanexPT-0.0.7/JanexPT.egg-info/
+-rw-r--r--   0 cipher    (1000) cipher    (1000)     1972 2023-08-07 19:59:46.000000 JanexPT-0.0.7/JanexPT.egg-info/PKG-INFO
+-rw-r--r--   0 cipher    (1000) cipher    (1000)      307 2023-08-07 19:59:46.000000 JanexPT-0.0.7/JanexPT.egg-info/SOURCES.txt
+-rw-r--r--   0 cipher    (1000) cipher    (1000)        1 2023-08-07 19:59:46.000000 JanexPT-0.0.7/JanexPT.egg-info/dependency_links.txt
+-rw-r--r--   0 cipher    (1000) cipher    (1000)       20 2023-08-07 19:59:46.000000 JanexPT-0.0.7/JanexPT.egg-info/requires.txt
+-rw-r--r--   0 cipher    (1000) cipher    (1000)        8 2023-08-07 19:59:46.000000 JanexPT-0.0.7/JanexPT.egg-info/top_level.txt
+-rw-r--r--   0 cipher    (1000) cipher    (1000)     2930 2023-08-07 14:45:22.000000 JanexPT-0.0.7/LICENSE
+-rw-r--r--   0 cipher    (1000) cipher    (1000)     1972 2023-08-07 19:59:46.353858 JanexPT-0.0.7/PKG-INFO
+-rw-r--r--   0 cipher    (1000) cipher    (1000)     1580 2023-08-07 19:52:47.000000 JanexPT-0.0.7/README.md
+-rw-r--r--   0 cipher    (1000) cipher    (1000)       38 2023-08-07 19:59:46.353858 JanexPT-0.0.7/setup.cfg
+-rw-r--r--   0 cipher    (1000) cipher    (1000)     1312 2023-08-07 19:59:34.000000 JanexPT-0.0.7/setup.py
```

### Comparing `JanexPT-0.0.6/JanexPT/main.py` & `JanexPT-0.0.7/JanexPT/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
 
         for intent in self.intents['intents']:
             if tag == intent["tag"]:
                 return intent
 
     def response_compare(self, input_string, classification):
         print(classification.get("tag"))
-        BestResponse = self.IntentMatcher.response_compare(input_string, intent)
+        BestResponse = self.IntentMatcher.response_compare(input_string, classification)
         return BestResponse
 
     def trainpt(self):
         try:
             open("train.py", "r")
             os.system("python3 train.py")
         except:
```

### Comparing `JanexPT-0.0.6/JanexPT/train.py` & `JanexPT-0.0.7/JanexPT/train.py`

 * *Files identical despite different names*

### Comparing `JanexPT-0.0.6/JanexPT.egg-info/PKG-INFO` & `JanexPT-0.0.7/JanexPT.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JanexPT
-Version: 0.0.6
+Version: 0.0.7
 Home-page: https://github.com/Cipher58/Janex-Pytorch
 Download-URL: https://github.com/Cipher58/Janex-Pytorch
 Author: Cipher58
 Author-email: cipher58public@gmail.com
 License: Lily 1.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `JanexPT-0.0.6/LICENSE` & `JanexPT-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `JanexPT-0.0.6/PKG-INFO` & `JanexPT-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JanexPT
-Version: 0.0.6
+Version: 0.0.7
 Home-page: https://github.com/Cipher58/Janex-Pytorch
 Download-URL: https://github.com/Cipher58/Janex-Pytorch
 Author: Cipher58
 Author-email: cipher58public@gmail.com
 License: Lily 1.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `JanexPT-0.0.6/README.md` & `JanexPT-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `JanexPT-0.0.6/setup.py` & `JanexPT-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 setuptools.setup(
     # Here is the module name.
     name="JanexPT",
 
     # version of the module
-    version="0.0.6",
+    version="0.0.7",
 
     # Name of Author
     author="Cipher58",
 
     download_url = 'https://github.com/Cipher58/Janex-Pytorch',
 
     # your Email address
```

