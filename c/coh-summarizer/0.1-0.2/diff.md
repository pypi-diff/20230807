# Comparing `tmp/coh-summarizer-0.1.tar.gz` & `tmp/coh_summarizer-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coh-summarizer-0.1.tar", last modified: Thu Oct 13 13:02:29 2022, max compression
+gzip compressed data, was "coh_summarizer-0.2.tar", last modified: Fri Jun 23 13:28:20 2023, max compression
```

## Comparing `coh-summarizer-0.1.tar` & `coh_summarizer-0.2.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxrwx   0        0        0        0 2022-10-13 13:02:29.681827 coh-summarizer-0.1/
--rw-rw-rw-   0        0        0     1933 2022-10-11 09:57:48.000000 coh-summarizer-0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     1735 2022-10-13 13:02:29.681827 coh-summarizer-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1522 2022-10-13 12:21:37.000000 coh-summarizer-0.1/README.md
--rw-rw-rw-   0        0        0       88 2022-09-15 07:35:20.000000 coh-summarizer-0.1/pyproject.toml
--rw-rw-rw-   0        0        0      530 2022-10-13 13:02:29.681827 coh-summarizer-0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-10-13 13:02:29.644044 coh-summarizer-0.1/src/
-drwxrwxrwx   0        0        0        0 2022-10-13 13:02:29.659680 coh-summarizer-0.1/src/coh_summarizer.egg-info/
--rw-rw-rw-   0        0        0     1735 2022-10-13 13:02:29.000000 coh-summarizer-0.1/src/coh_summarizer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      516 2022-10-13 13:02:29.000000 coh-summarizer-0.1/src/coh_summarizer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-13 13:02:29.000000 coh-summarizer-0.1/src/coh_summarizer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       89 2022-10-13 13:02:29.000000 coh-summarizer-0.1/src/coh_summarizer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2022-10-13 13:02:29.000000 coh-summarizer-0.1/src/coh_summarizer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-10-13 13:02:29.675303 coh-summarizer-0.1/src/summarizer/
--rw-rw-rw-   0        0        0      156 2022-10-11 09:57:48.000000 coh-summarizer-0.1/src/summarizer/__init__.py
--rw-rw-rw-   0        0        0     4533 2022-10-13 11:49:17.000000 coh-summarizer-0.1/src/summarizer/cohesion_sumamrizer.py
-drwxrwxrwx   0        0        0        0 2022-10-13 13:02:29.681827 coh-summarizer-0.1/src/summarizer/libs/
--rw-rw-rw-   0        0        0      116 2022-10-11 09:57:48.000000 coh-summarizer-0.1/src/summarizer/libs/__init__.py
--rw-rw-rw-   0        0        0     2144 2022-10-11 09:57:48.000000 coh-summarizer-0.1/src/summarizer/libs/common.py
--rw-rw-rw-   0        0        0     2364 2022-09-15 07:55:04.000000 coh-summarizer-0.1/src/summarizer/libs/stopwords.txt
--rw-rw-rw-   0        0        0     1061 2022-10-11 09:57:48.000000 coh-summarizer-0.1/src/summarizer/preprocessing.py
--rw-rw-rw-   0        0        0     3810 2022-10-13 12:13:36.000000 coh-summarizer-0.1/src/summarizer/summarizer.py
--rw-rw-rw-   0        0        0      575 2022-10-11 09:57:48.000000 coh-summarizer-0.1/src/summarizer/summarizer_algorithm.py
+drwxrwxrwx   0        0        0        0 2023-06-23 13:28:20.000565 coh_summarizer-0.2/
+-rw-rw-rw-   0        0        0     1933 2023-05-10 17:04:58.000000 coh_summarizer-0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     2007 2023-06-23 13:28:20.001561 coh_summarizer-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1522 2023-05-10 17:04:58.000000 coh_summarizer-0.2/README.md
+-rw-rw-rw-   0        0        0      779 2023-06-23 13:28:20.003600 coh_summarizer-0.2/setup.cfg
+-rw-rw-rw-   0        0        0       71 2023-02-15 12:10:08.000000 coh_summarizer-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 13:28:19.931928 coh_summarizer-0.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-23 13:28:19.967654 coh_summarizer-0.2/src/coh_summarizer.egg-info/
+-rw-rw-rw-   0        0        0     2007 2023-06-23 13:28:19.000000 coh_summarizer-0.2/src/coh_summarizer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      527 2023-06-23 13:28:19.000000 coh_summarizer-0.2/src/coh_summarizer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 13:28:19.000000 coh_summarizer-0.2/src/coh_summarizer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      126 2023-06-23 13:28:19.000000 coh_summarizer-0.2/src/coh_summarizer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-23 13:28:19.000000 coh_summarizer-0.2/src/coh_summarizer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-23 13:28:19.991596 coh_summarizer-0.2/src/summarizer/
+-rw-rw-rw-   0        0        0      156 2023-05-10 17:04:58.000000 coh_summarizer-0.2/src/summarizer/__init__.py
+-rw-rw-rw-   0        0        0     6581 2023-06-23 13:27:42.000000 coh_summarizer-0.2/src/summarizer/cohesion_sumamrizer.py
+-rw-rw-rw-   0        0        0     1482 2023-06-20 11:55:40.000000 coh_summarizer-0.2/src/summarizer/key_words.py
+drwxrwxrwx   0        0        0        0 2023-06-23 13:28:19.999570 coh_summarizer-0.2/src/summarizer/libs/
+-rw-rw-rw-   0        0        0      116 2023-05-10 17:04:58.000000 coh_summarizer-0.2/src/summarizer/libs/__init__.py
+-rw-rw-rw-   0        0        0     2144 2023-05-10 17:04:58.000000 coh_summarizer-0.2/src/summarizer/libs/common.py
+-rw-rw-rw-   0        0        0     1061 2023-05-10 17:04:58.000000 coh_summarizer-0.2/src/summarizer/preprocessing.py
+-rw-rw-rw-   0        0        0     3864 2023-06-23 13:27:41.000000 coh_summarizer-0.2/src/summarizer/summarizer.py
+-rw-rw-rw-   0        0        0      603 2023-05-23 21:16:50.000000 coh_summarizer-0.2/src/summarizer/summarizer_algorithm.py
+-rw-rw-rw-   0        0        0     5828 2023-05-30 16:18:23.000000 coh_summarizer-0.2/src/summarizer/test.py
```

### Comparing `coh-summarizer-0.1/LICENSE.txt` & `coh_summarizer-0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `coh-summarizer-0.1/PKG-INFO` & `coh_summarizer-0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 Metadata-Version: 2.1
-Name: coh-summarizer
-Version: 0.1
-Summary: Algorithms for summarization
-Author: ZILiAT-NASK
+Name: coh_summarizer
+Version: 0.2
+Summary: Summarizer tool
+Home-page: https://github.com/ZILiAT-NASK/Summarizer
+Author: ZILiAT-NASK, Adam Nowakowski
+Author-email: adam.nowakowski@nask.pl
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Summarizer
 Requires model: `pl_nask-0.0.5.tar.gz` from http://mozart.ipipan.waw.pl/~rtuora/spacy/
```

### Comparing `coh-summarizer-0.1/README.md` & `coh_summarizer-0.2/README.md`

 * *Files identical despite different names*

### Comparing `coh-summarizer-0.1/src/coh_summarizer.egg-info/PKG-INFO` & `coh_summarizer-0.2/src/coh_summarizer.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 Metadata-Version: 2.1
 Name: coh-summarizer
-Version: 0.1
-Summary: Algorithms for summarization
-Author: ZILiAT-NASK
+Version: 0.2
+Summary: Summarizer tool
+Home-page: https://github.com/ZILiAT-NASK/Summarizer
+Author: ZILiAT-NASK, Adam Nowakowski
+Author-email: adam.nowakowski@nask.pl
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Summarizer
 Requires model: `pl_nask-0.0.5.tar.gz` from http://mozart.ipipan.waw.pl/~rtuora/spacy/
```

### Comparing `coh-summarizer-0.1/src/coh_summarizer.egg-info/SOURCES.txt` & `coh_summarizer-0.2/src/coh_summarizer.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 LICENSE.txt
 README.md
-pyproject.toml
 setup.cfg
+setup.py
 src/coh_summarizer.egg-info/PKG-INFO
 src/coh_summarizer.egg-info/SOURCES.txt
 src/coh_summarizer.egg-info/dependency_links.txt
 src/coh_summarizer.egg-info/requires.txt
 src/coh_summarizer.egg-info/top_level.txt
 src/summarizer/__init__.py
 src/summarizer/cohesion_sumamrizer.py
+src/summarizer/key_words.py
 src/summarizer/preprocessing.py
 src/summarizer/summarizer.py
 src/summarizer/summarizer_algorithm.py
+src/summarizer/test.py
 src/summarizer/libs/__init__.py
-src/summarizer/libs/common.py
-src/summarizer/libs/stopwords.txt
+src/summarizer/libs/common.py
```

### Comparing `coh-summarizer-0.1/src/summarizer/libs/common.py` & `coh_summarizer-0.2/src/summarizer/libs/common.py`

 * *Files identical despite different names*

### Comparing `coh-summarizer-0.1/src/summarizer/preprocessing.py` & `coh_summarizer-0.2/src/summarizer/preprocessing.py`

 * *Files identical despite different names*

### Comparing `coh-summarizer-0.1/src/summarizer/summarizer.py` & `coh_summarizer-0.2/src/summarizer/summarizer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Copyright 2022 NASK-PIB
 # FIND TERMS AND CONDITIONS IN LICENSE FILE:
 # github.com/ZILiAT-NASK/Summarizer/LICENSE
 
-import morfeusz2
 import spacy
+import morfeusz2
+
 
 from .cohesion_sumamrizer import CohesionSummarizer
 from .preprocessing import preprocess
 from .libs.common import get_logger
 
 
 class Summarizer:
@@ -40,57 +41,57 @@
 
     def get_names(self):
         """Cohesion
         Frequent Lemmas
         Transformers"""
         return [alg.name for alg in self.algorithms]
 
-    def summarize(self, text, limit, unit, algorithm_str='Cohesion'):
+    def summarize(self, text, limit, unit, algorithm_str='Cohesion', alg_type='lemmas'):
         """throws KeyError"""
         algorithm = {alg.name: alg for alg in self.algorithms}[algorithm_str]
         if unit not in ['words', 'chars']:
             raise KeyError("For 'unit' possible options are 'words' and 'chars'.")
-        return self._process(text, algorithm, limit, unit)
+        return self._process(text, algorithm, limit, unit, alg_type)
 
-    def _process(self, text, algorithm, limit, unit):
+    def _process(self, text, algorithm, limit, unit, alg_type):
         out = {
             'status': 'correct',
             'summary': None,
             'event_id': 0,
             'message': None,
             'algorithm': algorithm.name,
         }
         try:
             if self.preprocess:
                 text = preprocess(text)
             n_tokens = len(algorithm.word_tokenizer(text))
             if n_tokens <= 30:
                 raise TooShortInputError
-            if n_tokens <= limit:
-                raise MaxWordsTooLowError
+            # if n_tokens <= limit:
+            #     raise MaxWordsTooLowError
 
-            summary = algorithm(text, limit, unit)
+            summary = algorithm(text, limit, unit, alg_type)
             if len(summary) < 10:
                 raise EmptySummaryError
             out['summary'] = summary
         except (SummarizerError, AttributeError, ArithmeticError, NameError, TypeError, ValueError) as ex:
             out['status'] = 'failed'
+            raise ex
             if isinstance(ex, SummarizerError):
                 out['message'] = self.event_messages[ex.event_id]
                 out['event_id'] = ex.event_id
 
             else:
                 out['message'] = self.event_messages[10]
                 out['event_id'] = 10
             if isinstance(ex, EmptySummaryError):
                 out['summary'] = '[Uwaga: najkrótsze możliwe streszczenie przekracza zadaną długość maksymalną.]'
             else:
                 out['summary'] = '[Nie utworzono podsumowania]'
             self.logger.debug(f"Failed at {algorithm.name} algorithm", exc_info=True)
-            print(ex)
         return out
 
 
 class SummarizerError(Exception):
     event_id: int
```

### Comparing `coh-summarizer-0.1/src/summarizer/summarizer_algorithm.py` & `coh_summarizer-0.2/src/summarizer/summarizer_algorithm.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 from abc import ABC, abstractmethod
 
 
 class SummarizerAlgorithm(ABC):
     name: str
     nlp = None
 
-    def __call__(self, text, limit, unit):
-        return self.summarize(text, limit, unit)
+    def __call__(self, text, limit, unit, type=None):
+        return self.summarize(text, limit, unit, type)
 
     @abstractmethod
-    def summarize(self, text, limit, unit):
+    def summarize(self, text, limit, unit, type=None):
         pass
 
     def rows(self, text):
         return text.strip().split('\n')
 
     def word_tokenizer(self, text):
         return [tok.text for tok in self.nlp.tokenizer(text)]
```

