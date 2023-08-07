# Comparing `tmp/chemnlp-2023.3.4.tar.gz` & `tmp/chemnlp-2023.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chemnlp-2023.3.4.tar", last modified: Sun Mar  5 16:32:29 2023, max compression
+gzip compressed data, was "chemnlp-2023.7.1.tar", last modified: Mon Aug  7 12:49:12 2023, max compression
```

## Comparing `chemnlp-2023.3.4.tar` & `chemnlp-2023.7.1.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2023-03-05 16:32:29.588508 chemnlp-2023.3.4/
--rw-r--r--   0 knc6     (54782) 642div   (36677)     1103 2023-03-05 16:30:50.000000 chemnlp-2023.3.4/LICENSE
--rw-r--r--   0 knc6     (54782) 642div   (36677)     2527 2023-03-05 16:32:29.588508 chemnlp-2023.3.4/PKG-INFO
--rw-r--r--   0 knc6     (54782) 642div   (36677)     2061 2023-03-05 16:30:50.000000 chemnlp-2023.3.4/README.md
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2023-03-05 16:32:29.552508 chemnlp-2023.3.4/chemnlp/
--rw-r--r--   0 knc6     (54782) 642div   (36677)      244 2023-03-05 16:30:50.000000 chemnlp-2023.3.4/chemnlp/__init__.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2023-03-05 16:32:29.568508 chemnlp-2023.3.4/chemnlp/classification/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       40 2023-03-05 16:30:50.000000 chemnlp-2023.3.4/chemnlp/classification/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     7644 2023-03-05 16:30:50.000000 chemnlp-2023.3.4/chemnlp/classification/bert_classify.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    14392 2023-03-05 16:30:50.000000 chemnlp-2023.3.4/chemnlp/classification/scikit_class.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2023-03-05 16:32:29.572508 chemnlp-2023.3.4/chemnlp/clustering/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       36 2023-03-05 16:30:50.000000 chemnlp-2023.3.4/chemnlp/clustering/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     5749 2023-03-05 16:30:50.000000 chemnlp-2023.3.4/chemnlp/clustering/tsne.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2023-03-05 16:32:29.580508 chemnlp-2023.3.4/chemnlp/utils/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       41 2023-03-05 16:30:50.000000 chemnlp-2023.3.4/chemnlp/utils/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     3846 2023-03-05 16:30:50.000000 chemnlp-2023.3.4/chemnlp/utils/keywords.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     1214 2023-03-05 16:30:50.000000 chemnlp-2023.3.4/chemnlp/utils/process_doc.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)      541 2023-03-05 16:30:50.000000 chemnlp-2023.3.4/chemnlp/utils/run_chemnlp.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2023-03-05 16:32:29.584508 chemnlp-2023.3.4/chemnlp/wordcloud/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       37 2023-03-05 16:30:50.000000 chemnlp-2023.3.4/chemnlp/wordcloud/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     1100 2023-03-05 16:30:50.000000 chemnlp-2023.3.4/chemnlp/wordcloud/make_wordcloud.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2023-03-05 16:32:29.564509 chemnlp-2023.3.4/chemnlp.egg-info/
--rw-r--r--   0 knc6     (54782) 642div   (36677)     2527 2023-03-05 16:32:28.000000 chemnlp-2023.3.4/chemnlp.egg-info/PKG-INFO
--rw-r--r--   0 knc6     (54782) 642div   (36677)      548 2023-03-05 16:32:29.000000 chemnlp-2023.3.4/chemnlp.egg-info/SOURCES.txt
--rw-r--r--   0 knc6     (54782) 642div   (36677)        1 2023-03-05 16:32:28.000000 chemnlp-2023.3.4/chemnlp.egg-info/dependency_links.txt
--rw-r--r--   0 knc6     (54782) 642div   (36677)      146 2023-03-05 16:32:29.000000 chemnlp-2023.3.4/chemnlp.egg-info/requires.txt
--rw-r--r--   0 knc6     (54782) 642div   (36677)        8 2023-03-05 16:32:29.000000 chemnlp-2023.3.4/chemnlp.egg-info/top_level.txt
--rw-r--r--   0 knc6     (54782) 642div   (36677)       38 2023-03-05 16:32:29.588508 chemnlp-2023.3.4/setup.cfg
--rw-r--r--   0 knc6     (54782) 642div   (36677)      973 2023-03-05 16:30:50.000000 chemnlp-2023.3.4/setup.py
+drwxr-xr-x   0 kamalch   (1000) kamalch   (1000)        0 2023-08-07 12:49:12.238988 chemnlp-2023.7.1/
+-rw-r--r--   0 kamalch   (1000) kamalch   (1000)     1103 2023-08-07 12:40:20.000000 chemnlp-2023.7.1/LICENSE
+-rw-r--r--   0 kamalch   (1000) kamalch   (1000)     3070 2023-08-07 12:49:12.238988 chemnlp-2023.7.1/PKG-INFO
+-rw-r--r--   0 kamalch   (1000) kamalch   (1000)     2656 2023-08-07 12:40:20.000000 chemnlp-2023.7.1/README.md
+drwxr-xr-x   0 kamalch   (1000) kamalch   (1000)        0 2023-08-07 12:49:12.228989 chemnlp-2023.7.1/chemnlp/
+-rw-r--r--   0 kamalch   (1000) kamalch   (1000)      244 2023-08-07 12:40:20.000000 chemnlp-2023.7.1/chemnlp/__init__.py
+drwxr-xr-x   0 kamalch   (1000) kamalch   (1000)        0 2023-08-07 12:49:12.228989 chemnlp-2023.7.1/chemnlp/classification/
+-rw-r--r--   0 kamalch   (1000) kamalch   (1000)       40 2023-08-07 12:40:20.000000 chemnlp-2023.7.1/chemnlp/classification/__init__.py
+-rw-r--r--   0 kamalch   (1000) kamalch   (1000)     7849 2023-08-07 12:40:20.000000 chemnlp-2023.7.1/chemnlp/classification/bert_classify.py
+-rw-r--r--   0 kamalch   (1000) kamalch   (1000)    25495 2023-08-07 12:40:20.000000 chemnlp-2023.7.1/chemnlp/classification/gnn_class.py
+-rw-r--r--   0 kamalch   (1000) kamalch   (1000)    14392 2023-08-07 12:40:20.000000 chemnlp-2023.7.1/chemnlp/classification/scikit_class.py
+drwxr-xr-x   0 kamalch   (1000) kamalch   (1000)        0 2023-08-07 12:49:12.228989 chemnlp-2023.7.1/chemnlp/clustering/
+-rw-r--r--   0 kamalch   (1000) kamalch   (1000)       36 2023-08-07 12:40:20.000000 chemnlp-2023.7.1/chemnlp/clustering/__init__.py
+-rw-r--r--   0 kamalch   (1000) kamalch   (1000)     5749 2023-08-07 12:40:20.000000 chemnlp-2023.7.1/chemnlp/clustering/tsne.py
+drwxr-xr-x   0 kamalch   (1000) kamalch   (1000)        0 2023-08-07 12:49:12.228989 chemnlp-2023.7.1/chemnlp/utils/
+-rw-r--r--   0 kamalch   (1000) kamalch   (1000)       41 2023-08-07 12:40:20.000000 chemnlp-2023.7.1/chemnlp/utils/__init__.py
+-rw-r--r--   0 kamalch   (1000) kamalch   (1000)     3846 2023-08-07 12:40:20.000000 chemnlp-2023.7.1/chemnlp/utils/keywords.py
+-rw-r--r--   0 kamalch   (1000) kamalch   (1000)     1214 2023-08-07 12:40:20.000000 chemnlp-2023.7.1/chemnlp/utils/process_doc.py
+-rw-r--r--   0 kamalch   (1000) kamalch   (1000)      541 2023-08-07 12:40:20.000000 chemnlp-2023.7.1/chemnlp/utils/run_chemnlp.py
+drwxr-xr-x   0 kamalch   (1000) kamalch   (1000)        0 2023-08-07 12:49:12.238988 chemnlp-2023.7.1/chemnlp/wordcloud/
+-rw-r--r--   0 kamalch   (1000) kamalch   (1000)       37 2023-08-07 12:40:20.000000 chemnlp-2023.7.1/chemnlp/wordcloud/__init__.py
+-rw-r--r--   0 kamalch   (1000) kamalch   (1000)     1100 2023-08-07 12:40:20.000000 chemnlp-2023.7.1/chemnlp/wordcloud/make_wordcloud.py
+drwxr-xr-x   0 kamalch   (1000) kamalch   (1000)        0 2023-08-07 12:49:12.228989 chemnlp-2023.7.1/chemnlp.egg-info/
+-rw-r--r--   0 kamalch   (1000) kamalch   (1000)     3070 2023-08-07 12:49:12.000000 chemnlp-2023.7.1/chemnlp.egg-info/PKG-INFO
+-rw-r--r--   0 kamalch   (1000) kamalch   (1000)      584 2023-08-07 12:49:12.000000 chemnlp-2023.7.1/chemnlp.egg-info/SOURCES.txt
+-rw-r--r--   0 kamalch   (1000) kamalch   (1000)        1 2023-08-07 12:49:12.000000 chemnlp-2023.7.1/chemnlp.egg-info/dependency_links.txt
+-rw-r--r--   0 kamalch   (1000) kamalch   (1000)      146 2023-08-07 12:49:12.000000 chemnlp-2023.7.1/chemnlp.egg-info/requires.txt
+-rw-r--r--   0 kamalch   (1000) kamalch   (1000)        8 2023-08-07 12:49:12.000000 chemnlp-2023.7.1/chemnlp.egg-info/top_level.txt
+-rw-r--r--   0 kamalch   (1000) kamalch   (1000)       38 2023-08-07 12:49:12.238988 chemnlp-2023.7.1/setup.cfg
+-rw-r--r--   0 kamalch   (1000) kamalch   (1000)      958 2023-08-07 12:40:20.000000 chemnlp-2023.7.1/setup.py
```

### Comparing `chemnlp-2023.3.4/LICENSE` & `chemnlp-2023.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chemnlp-2023.3.4/PKG-INFO` & `chemnlp-2023.7.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: chemnlp
-Version: 2023.3.4
+Version: 2023.7.1
 Summary: chemnlp
 Home-page: https://github.com/usnistgov/chemnlp
-Author: Kamal Choudhary, Mathew Kelley
+Author: Kamal Choudhary
 Author-email: kamal.choudhary@nist.gov
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![name](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/knc6/jarvis-tools-notebooks/blob/master/ChemNLP_Example.ipynb)
+[![name](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/knc6/jarvis-tools-notebooks/blob/master/jarvis-tools-notebooks/ChemNLP_Example.ipynb)
+![alt text](https://github.com/usnistgov/chemnlp/actions/workflows/main.yml/badge.svg)
+[![DOI](https://zenodo.org/badge/523320947.svg)](https://zenodo.org/badge/latestdoi/523320947)
+
 
 # ChemNLP
 
 # Table of Contents
 * [Introduction](#intro)
 * [Installation](#install)
 * [Examples](#example)
@@ -78,22 +79,25 @@
 
 #### Text classification example
 
 ```
 python chemnlp/classification/scikit_class.py --csv_path chemnlp/sample_data/cond_mat_small.csv
 ```
 
+[Google Colab example for installation and text classification](https://colab.research.google.com/github/knc6/jarvis-tools-notebooks/blob/master/jarvis-tools-notebooks/ChemNLP_Example.ipynb)
+
+[Google Colab example for Text Generation with HuggingFace](https://colab.research.google.com/github/knc6/jarvis-tools-notebooks/blob/master/jarvis-tools-notebooks/ChemNLP_TitleToAbstract.ipynb)
+
+
 <a name="webapp"></a>
 Using the webapp
 ---------
 The webapp is available at: https://jarvis.nist.gov/jarvischemnlp
 
 ![JARVIS-ChemNLP](https://github.com/usnistgov/chemnlp/blob/develop/chemnlp/PTable.PNG)
 
 <a name="reference"></a>
 Reference
 ---------
 
 
 [ChemNLP: A Natural Language Processing based Library for Materials Chemistry Text Data](https://arxiv.org/abs/2209.08203)
-
-
```

### Comparing `chemnlp-2023.3.4/README.md` & `chemnlp-2023.7.1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-[![name](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/knc6/jarvis-tools-notebooks/blob/master/ChemNLP_Example.ipynb)
+[![name](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/knc6/jarvis-tools-notebooks/blob/master/jarvis-tools-notebooks/ChemNLP_Example.ipynb)
+![alt text](https://github.com/usnistgov/chemnlp/actions/workflows/main.yml/badge.svg)
+[![DOI](https://zenodo.org/badge/523320947.svg)](https://zenodo.org/badge/latestdoi/523320947)
+
 
 # ChemNLP
 
 # Table of Contents
 * [Introduction](#intro)
 * [Installation](#install)
 * [Examples](#example)
@@ -62,14 +65,19 @@
 
 #### Text classification example
 
 ```
 python chemnlp/classification/scikit_class.py --csv_path chemnlp/sample_data/cond_mat_small.csv
 ```
 
+[Google Colab example for installation and text classification](https://colab.research.google.com/github/knc6/jarvis-tools-notebooks/blob/master/jarvis-tools-notebooks/ChemNLP_Example.ipynb)
+
+[Google Colab example for Text Generation with HuggingFace](https://colab.research.google.com/github/knc6/jarvis-tools-notebooks/blob/master/jarvis-tools-notebooks/ChemNLP_TitleToAbstract.ipynb)
+
+
 <a name="webapp"></a>
 Using the webapp
 ---------
 The webapp is available at: https://jarvis.nist.gov/jarvischemnlp
 
 ![JARVIS-ChemNLP](https://github.com/usnistgov/chemnlp/blob/develop/chemnlp/PTable.PNG)
```

### Comparing `chemnlp-2023.3.4/chemnlp/classification/bert_classify.py` & `chemnlp-2023.7.1/chemnlp/classification/bert_classify.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,16 +27,16 @@
 
 # os.environ["CUDA_LAUNCH_BLOCKING"] = "1"
 # !export CUDA_LAUNCH_BLOCKING="1"
 
 
 def train_classifier(
     df=None,
-    key="term",
-    value="title",
+    key="categories",
+    value="title_abstract",
     batch_size=32,
     epochs=5,
     seed_val=17,
     test_size=0.2,
     random_state=0,
     max_length=128,
     lr=0.001,
@@ -244,10 +244,13 @@
         tqdm.write(f"Validation loss: {val_loss}")
         tqdm.write(f"F1 Score (Weighted): {val_f1}")
         tqdm.write(f"Accuracy: {val_acc}")
         # accuracy_per_class(predictions, true_vals)
 
 
 if __name__ == "__main__":
-    df = pd.read_csv("cond_mat.csv")
+    # df = pd.read_csv("cond_mat.csv")
+    df = pd.read_csv("/wrk/knc6/AtomNLP/Summarize/cond_mat.csv")
+    fname = "/wrk/knc6/AtomNLP/chemnlp/chemnlp/sample_data/cond_mat_small.csv"
+    # df = pd.read_csv(fname)
 
-    train_classifier(df=df)
+    train_classifier(df=df, max_length=8)
```

### Comparing `chemnlp-2023.3.4/chemnlp/classification/scikit_class.py` & `chemnlp-2023.7.1/chemnlp/classification/scikit_class.py`

 * *Files identical despite different names*

### Comparing `chemnlp-2023.3.4/chemnlp/clustering/tsne.py` & `chemnlp-2023.7.1/chemnlp/clustering/tsne.py`

 * *Files identical despite different names*

### Comparing `chemnlp-2023.3.4/chemnlp/utils/keywords.py` & `chemnlp-2023.7.1/chemnlp/utils/keywords.py`

 * *Files identical despite different names*

### Comparing `chemnlp-2023.3.4/chemnlp/utils/process_doc.py` & `chemnlp-2023.7.1/chemnlp/utils/process_doc.py`

 * *Files identical despite different names*

### Comparing `chemnlp-2023.3.4/chemnlp/utils/run_chemnlp.py` & `chemnlp-2023.7.1/chemnlp/utils/run_chemnlp.py`

 * *Files identical despite different names*

### Comparing `chemnlp-2023.3.4/chemnlp/wordcloud/make_wordcloud.py` & `chemnlp-2023.7.1/chemnlp/wordcloud/make_wordcloud.py`

 * *Files identical despite different names*

### Comparing `chemnlp-2023.3.4/chemnlp.egg-info/PKG-INFO` & `chemnlp-2023.7.1/chemnlp.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: chemnlp
-Version: 2023.3.4
+Version: 2023.7.1
 Summary: chemnlp
 Home-page: https://github.com/usnistgov/chemnlp
-Author: Kamal Choudhary, Mathew Kelley
+Author: Kamal Choudhary
 Author-email: kamal.choudhary@nist.gov
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![name](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/knc6/jarvis-tools-notebooks/blob/master/ChemNLP_Example.ipynb)
+[![name](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/knc6/jarvis-tools-notebooks/blob/master/jarvis-tools-notebooks/ChemNLP_Example.ipynb)
+![alt text](https://github.com/usnistgov/chemnlp/actions/workflows/main.yml/badge.svg)
+[![DOI](https://zenodo.org/badge/523320947.svg)](https://zenodo.org/badge/latestdoi/523320947)
+
 
 # ChemNLP
 
 # Table of Contents
 * [Introduction](#intro)
 * [Installation](#install)
 * [Examples](#example)
@@ -78,22 +79,25 @@
 
 #### Text classification example
 
 ```
 python chemnlp/classification/scikit_class.py --csv_path chemnlp/sample_data/cond_mat_small.csv
 ```
 
+[Google Colab example for installation and text classification](https://colab.research.google.com/github/knc6/jarvis-tools-notebooks/blob/master/jarvis-tools-notebooks/ChemNLP_Example.ipynb)
+
+[Google Colab example for Text Generation with HuggingFace](https://colab.research.google.com/github/knc6/jarvis-tools-notebooks/blob/master/jarvis-tools-notebooks/ChemNLP_TitleToAbstract.ipynb)
+
+
 <a name="webapp"></a>
 Using the webapp
 ---------
 The webapp is available at: https://jarvis.nist.gov/jarvischemnlp
 
 ![JARVIS-ChemNLP](https://github.com/usnistgov/chemnlp/blob/develop/chemnlp/PTable.PNG)
 
 <a name="reference"></a>
 Reference
 ---------
 
 
 [ChemNLP: A Natural Language Processing based Library for Materials Chemistry Text Data](https://arxiv.org/abs/2209.08203)
-
-
```

### Comparing `chemnlp-2023.3.4/chemnlp.egg-info/SOURCES.txt` & `chemnlp-2023.7.1/chemnlp.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 chemnlp.egg-info/PKG-INFO
 chemnlp.egg-info/SOURCES.txt
 chemnlp.egg-info/dependency_links.txt
 chemnlp.egg-info/requires.txt
 chemnlp.egg-info/top_level.txt
 chemnlp/classification/__init__.py
 chemnlp/classification/bert_classify.py
+chemnlp/classification/gnn_class.py
 chemnlp/classification/scikit_class.py
 chemnlp/clustering/__init__.py
 chemnlp/clustering/tsne.py
 chemnlp/utils/__init__.py
 chemnlp/utils/keywords.py
 chemnlp/utils/process_doc.py
 chemnlp/utils/run_chemnlp.py
```

### Comparing `chemnlp-2023.3.4/setup.py` & `chemnlp-2023.7.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="chemnlp",
-    version="2023.3.4",
-    author="Kamal Choudhary, Mathew Kelley",
+    version="2023.7.1",
+    author="Kamal Choudhary",
     author_email="kamal.choudhary@nist.gov",
     description="chemnlp",
     install_requires=[
         "numpy>=1.22.0",
         "scipy>=1.6.3",
         "jarvis-tools>=2021.07.19",
         "ChemDataExtractor>=1.3.0",
```

