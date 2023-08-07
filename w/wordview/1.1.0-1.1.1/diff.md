# Comparing `tmp/wordview-1.1.0.tar.gz` & `tmp/wordview-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wordview-1.1.0.tar", max compression
+gzip compressed data, was "wordview-1.1.1.tar", max compression
```

## Comparing `wordview-1.1.0.tar` & `wordview-1.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     3034 2023-08-05 14:14:11.767025 wordview-1.1.0/CHANGES.rst
--rw-r--r--   0        0        0     1074 2023-08-05 14:14:11.767025 wordview-1.1.0/LICENSE
--rw-r--r--   0        0        0     4047 2023-08-05 14:14:11.767025 wordview-1.1.0/README.rst
--rw-r--r--   0        0        0      936 2023-08-05 14:14:11.859026 wordview-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      163 2023-08-05 14:14:11.859026 wordview-1.1.0/wordview/__init__.py
--rw-r--r--   0        0        0       60 2023-08-05 14:14:11.859026 wordview-1.1.0/wordview/anomaly/__init__.py
--rw-r--r--   0        0        0     7343 2023-08-05 14:14:11.859026 wordview-1.1.0/wordview/anomaly/gaussianize.py
--rw-r--r--   0        0        0     4789 2023-08-05 14:14:11.859026 wordview-1.1.0/wordview/anomaly/normaldist.py
--rw-r--r--   0        0        0       53 2023-08-05 14:14:11.859026 wordview-1.1.0/wordview/bias_analysis/__init__.py
--rw-r--r--   0        0        0     7130 2023-08-05 14:14:11.859026 wordview-1.1.0/wordview/bias_analysis/bias.py
--rw-r--r--   0        0        0     4131 2023-08-05 14:14:11.859026 wordview-1.1.0/wordview/bias_analysis/bias_terms.py
--rw-r--r--   0        0        0       48 2023-08-05 14:14:11.863026 wordview-1.1.0/wordview/clustering/__init__.py
--rw-r--r--   0        0        0     3027 2023-08-05 14:14:11.863026 wordview-1.1.0/wordview/clustering/cluster.py
--rw-r--r--   0        0        0     1340 2023-08-05 14:14:11.863026 wordview-1.1.0/wordview/io/dataframe_reader.py
--rw-r--r--   0        0        0       34 2023-08-05 14:14:11.863026 wordview-1.1.0/wordview/mwes/__init__.py
--rw-r--r--   0        0        0     1499 2023-08-05 14:14:11.863026 wordview-1.1.0/wordview/mwes/association_measures.py
--rw-r--r--   0        0        0     9848 2023-08-05 14:14:11.863026 wordview-1.1.0/wordview/mwes/mwe.py
--rw-r--r--   0        0        0     1967 2023-08-05 14:14:11.863026 wordview-1.1.0/wordview/mwes/patterns.py
--rw-r--r--   0        0        0      111 2023-08-05 14:14:11.863026 wordview-1.1.0/wordview/preprocessing/__init__.py
--rw-r--r--   0        0        0     3078 2023-08-05 14:14:11.863026 wordview-1.1.0/wordview/preprocessing/cleaning.py
--rw-r--r--   0        0        0     3718 2023-08-05 14:14:11.863026 wordview-1.1.0/wordview/preprocessing/count.py
--rw-r--r--   0        0        0       75 2023-08-05 14:14:11.863026 wordview-1.1.0/wordview/text_analysis/__init__.py
--rw-r--r--   0        0        0    12315 2023-08-05 14:14:11.863026 wordview-1.1.0/wordview/text_analysis/core.py
--rw-r--r--   0        0        0     8753 2023-08-05 14:14:11.863026 wordview-1.1.0/wordview/text_analysis/wrapper.py
--rw-r--r--   0        0        0     4886 1970-01-01 00:00:00.000000 wordview-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3157 2023-08-07 10:14:17.045697 wordview-1.1.1/CHANGES.rst
+-rw-r--r--   0        0        0     1074 2023-08-07 10:14:17.045697 wordview-1.1.1/LICENSE
+-rw-r--r--   0        0        0     4527 2023-08-07 10:14:17.045697 wordview-1.1.1/README.rst
+-rw-r--r--   0        0        0      936 2023-08-07 10:14:17.233698 wordview-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0      163 2023-08-07 10:14:17.233698 wordview-1.1.1/wordview/__init__.py
+-rw-r--r--   0        0        0       60 2023-08-07 10:14:17.233698 wordview-1.1.1/wordview/anomaly/__init__.py
+-rw-r--r--   0        0        0     7343 2023-08-07 10:14:17.233698 wordview-1.1.1/wordview/anomaly/gaussianize.py
+-rw-r--r--   0        0        0     4789 2023-08-07 10:14:17.233698 wordview-1.1.1/wordview/anomaly/normaldist.py
+-rw-r--r--   0        0        0       53 2023-08-07 10:14:17.233698 wordview-1.1.1/wordview/bias_analysis/__init__.py
+-rw-r--r--   0        0        0     7097 2023-08-07 10:14:17.233698 wordview-1.1.1/wordview/bias_analysis/bias.py
+-rw-r--r--   0        0        0     4131 2023-08-07 10:14:17.233698 wordview-1.1.1/wordview/bias_analysis/bias_terms.py
+-rw-r--r--   0        0        0       48 2023-08-07 10:14:17.233698 wordview-1.1.1/wordview/clustering/__init__.py
+-rw-r--r--   0        0        0     3027 2023-08-07 10:14:17.233698 wordview-1.1.1/wordview/clustering/cluster.py
+-rw-r--r--   0        0        0     1340 2023-08-07 10:14:17.233698 wordview-1.1.1/wordview/io/dataframe_reader.py
+-rw-r--r--   0        0        0       34 2023-08-07 10:14:17.233698 wordview-1.1.1/wordview/mwes/__init__.py
+-rw-r--r--   0        0        0     1499 2023-08-07 10:14:17.233698 wordview-1.1.1/wordview/mwes/association_measures.py
+-rw-r--r--   0        0        0     9848 2023-08-07 10:14:17.233698 wordview-1.1.1/wordview/mwes/mwe.py
+-rw-r--r--   0        0        0     1967 2023-08-07 10:14:17.233698 wordview-1.1.1/wordview/mwes/patterns.py
+-rw-r--r--   0        0        0      111 2023-08-07 10:14:17.233698 wordview-1.1.1/wordview/preprocessing/__init__.py
+-rw-r--r--   0        0        0     3078 2023-08-07 10:14:17.233698 wordview-1.1.1/wordview/preprocessing/cleaning.py
+-rw-r--r--   0        0        0     3718 2023-08-07 10:14:17.233698 wordview-1.1.1/wordview/preprocessing/count.py
+-rw-r--r--   0        0        0       75 2023-08-07 10:14:17.233698 wordview-1.1.1/wordview/text_analysis/__init__.py
+-rw-r--r--   0        0        0    12315 2023-08-07 10:14:17.233698 wordview-1.1.1/wordview/text_analysis/core.py
+-rw-r--r--   0        0        0     8753 2023-08-07 10:14:17.233698 wordview-1.1.1/wordview/text_analysis/wrapper.py
+-rw-r--r--   0        0        0     5366 1970-01-01 00:00:00.000000 wordview-1.1.1/PKG-INFO
```

### Comparing `wordview-1.1.0/CHANGES.rst` & `wordview-1.1.1/CHANGES.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+Version 1.1.1
+-------------
+- Fix minor bugs in bias analysis.
+- Improve fonts and minor details in bias analysis plots.
+
+
 Version 1.1.0
 -------------
 - Add bias detection and analysis feature (based on sentiment analysis)
 - Include 3 bias categories: race, religion, and gender.
 - Include an initial set of key terms for each bias category.
 - Add function to visualize bias analysis in a plot.
 - Add function to visualize bias analysis in a tables.
```

### Comparing `wordview-1.1.0/LICENSE` & `wordview-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wordview-1.1.0/README.rst` & `wordview-1.1.1/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 .. image:: https://img.shields.io/pypi/pyversions/wordview
    :alt: PyPI - Python Version
 
 .. image:: https://img.shields.io/pypi/dm/wordview
    :alt: PyPI - Downloads
 
-Wordview is a Python package for Exploratory Data Analysis (EDA) and Feature Extraction for text.
+Wordview is a Python package for Exploratory Data Analysis (EDA) of text.
 Wordview's Python API is open-source and available under the `MIT
 license <https://en.wikipedia.org/wiki/MIT_License>`__.
 
 |cover|
 
 
 Usage
@@ -47,43 +47,46 @@
 
 Analysis of Labels
 ******************
 Wordview calculates several statistics for labels in labeled datasets whether they are at document or sequence level.
 See `label analysis documentation pages <./docs/source/labels.rst>`__ for usage and examples.
 
 
-Feature Extraction
-###################
-
-Wordview has various functionalities for feature extraction from text, including Multiword Expressions (MWEs), clusters, anomalies and 
-outliers, and more. See the following sections as well as the linked documentation page in each section for details.
-
-Multiword Expressions
-*********************
-
+Extraction & Analysis of Multiword Expressions
+**********************************************
 Multiword Expressions (MWEs) are phrases that can be treated as a single
 semantic unit. E.g. *swimming pool* and *climate change*. MWEs have
 application in different areas including: parsing, language models,
 language generation, terminology extraction, and topic models. Wordview can extract different types of MWEs from text.
 See `MWEs documentation page <./docs/source/mwes.rst>`__ for usage and examples.
 
-Anomalies and Outliers
-**********************
 
+Bias Analysis
+**************
+In the rapidly evolving realm of Natural Language Processing (NLP), downstream models are as unbiased and fair as the data on which they are trained.
+Wordview Bias Analysis module is designed to assist in the rigorous task of ensuring that underlying training datasets are devoid of explicit negative biases related to categories such as gender, race, and religion.
+By identifying and rectifying these biases, Wordview attempts to pave the way for the creation of more inclusive, fair, and unbiased NLP applications, leading to better user experiences and more equitable technology.
+See the `bias analysis documentation page <./docs/source/bias.rst>`__ for usage and examples.
+
+
+Analysis of Anomalies and Outliers
+**********************************
 Anomalies and outliers have wide applications in Machine Learning. While in
 some cases, you can capture them and remove them from the data to improve the
 performance of a downstream ML model, in other cases, they become the data points
 of interest where we endeavor to find them in order to shed light into our data.
 
 Wordview offers several anomaly and outlier detection functions.
 See `anomalies documentation page <./docs/source/anomalies.rst>`__ for usage and examples.
 
 
-Clusters
-*********
+
+
+Cluster Analysis
+****************
 Clustering can be used to identify different groups of documents with similar information, in an unsupervised fashion.
 Despite it's ability to provide valuable insights into your data, you do not need labeled data for clustering. See
 `wordview`'s `clustering documentation page <./docs/source/clustering.rst>`__ for usage and examples.
 
 
 Utilities
 #########
```

### Comparing `wordview-1.1.0/pyproject.toml` & `wordview-1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wordview"
-version = "1.1.0"
+version = "1.1.1"
 description = "Wordview is a Python package for text analysis."
 authors = ["meghdadFar <meghdad.farahmand@gmail.com>"]
 readme = "README.rst"
 include = ["CHANGES.rst"]
 exclude = ["notebooks/", "tests/", "data/"]
 license = "MIT"
 keywords = ["nlp", "text analysis", "statistics"]
```

### Comparing `wordview-1.1.0/wordview/anomaly/gaussianize.py` & `wordview-1.1.1/wordview/anomaly/gaussianize.py`

 * *Files identical despite different names*

### Comparing `wordview-1.1.0/wordview/anomaly/normaldist.py` & `wordview-1.1.1/wordview/anomaly/normaldist.py`

 * *Files identical despite different names*

### Comparing `wordview-1.1.0/wordview/bias_analysis/bias.py` & `wordview-1.1.1/wordview/bias_analysis/bias.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import string
 
-import bias_terms
 import plotly.graph_objects as go
 from nltk import word_tokenize
 from plotly.subplots import make_subplots
 from sentence_transformers import SentenceTransformer
 from tabulate import tabulate  # type: ignore
 from tqdm import tqdm
 from transformers import BertForSequenceClassification, BertTokenizer
 
 from wordview import logger
+from wordview.bias_analysis import bias_terms
 from wordview.io.dataframe_reader import DataFrameReader
 
 
 class BiasDetector:
     def __init__(self, df, text_column):
         # bert-base-multilingual-uncased-sentiment supports English, Dutch, German, French, Spanish, and Italian.
         self.sentiment_model = BertForSequenceClassification.from_pretrained(
@@ -67,26 +67,23 @@
                     intersection = set(tokens).intersection(
                         [cat_term.lower() for cat_term in category_terms]
                     )
                     if intersection:
                         association_result = self._calculate_association(
                             category_terms=intersection, sentence=sentence
                         )
-                        print(
-                            f"> Category type: {category_type}\n\tcategory terms: {category_terms}\n\tsentence: {sentence}\n\tassoociation: {association_result}\n--------------------"
-                        )
                         category_type_avg_sentiment += association_result
                         n += 1
             category_type_avg_sentiment = (
                 (category_type_avg_sentiment / n) if n > 0 else "-inf"
             )
             biases[category_type] = category_type_avg_sentiment
         return biases
 
-    def show_plot(self):
+    def show_bias_plot(self):
         categories = list(self.biases.keys())
         fig = make_subplots(
             rows=len(categories),
             cols=1,
             subplot_titles=[cat.capitalize() for cat in categories],
         )
         colorscale = [
@@ -114,30 +111,32 @@
                     ticktext=[
                         "Very Negative",
                         "Negative",
                         "Neutral",
                         "Positive",
                         "Very Positive",
                     ],
+                    tickfont=dict(size=16),
+                    titlefont=dict(size=18),
                 ),
                 zauto=False,  # Prevents auto scaling
             )
             fig.add_trace(heatmap, row=index + 1, col=1)
             fig.update_yaxes(showgrid=False, showticklabels=False)
-            fig.update_xaxes(
-                showgrid=False,
-            )
+            fig.update_xaxes(showgrid=False, tickfont=dict(size=16))
         fig.update_layout(
             title="Bias Scores Across Categories",
-            title_font_size=18,  # Increase title font size
+            title_font_size=20,  # Increase title font size
             title_x=0.5,  # Center main title
-            width=1200,  # Fixed width
-            height=300 * len(categories),  # Adjust height based on number of categories
+            width=1000,  # Fixed width
+            height=250 * len(categories),  # Adjust height based on number of categories
             plot_bgcolor="white",  # Set background color to white
         )
+        # Increase font size of subplot titles.
+        fig.update_annotations(font_size=18)
         fig.show()
 
     def print_bias_table(self):
         def sentiment_to_bias(val):
             if val == "-inf":
                 return "Unknown"
             elif val == 0:
```

### Comparing `wordview-1.1.0/wordview/bias_analysis/bias_terms.py` & `wordview-1.1.1/wordview/bias_analysis/bias_terms.py`

 * *Files identical despite different names*

### Comparing `wordview-1.1.0/wordview/clustering/cluster.py` & `wordview-1.1.1/wordview/clustering/cluster.py`

 * *Files identical despite different names*

### Comparing `wordview-1.1.0/wordview/io/dataframe_reader.py` & `wordview-1.1.1/wordview/io/dataframe_reader.py`

 * *Files identical despite different names*

### Comparing `wordview-1.1.0/wordview/mwes/association_measures.py` & `wordview-1.1.1/wordview/mwes/association_measures.py`

 * *Files identical despite different names*

### Comparing `wordview-1.1.0/wordview/mwes/mwe.py` & `wordview-1.1.1/wordview/mwes/mwe.py`

 * *Files identical despite different names*

### Comparing `wordview-1.1.0/wordview/mwes/patterns.py` & `wordview-1.1.1/wordview/mwes/patterns.py`

 * *Files identical despite different names*

### Comparing `wordview-1.1.0/wordview/preprocessing/cleaning.py` & `wordview-1.1.1/wordview/preprocessing/cleaning.py`

 * *Files identical despite different names*

### Comparing `wordview-1.1.0/wordview/preprocessing/count.py` & `wordview-1.1.1/wordview/preprocessing/count.py`

 * *Files identical despite different names*

### Comparing `wordview-1.1.0/wordview/text_analysis/core.py` & `wordview-1.1.1/wordview/text_analysis/core.py`

 * *Files identical despite different names*

### Comparing `wordview-1.1.0/wordview/text_analysis/wrapper.py` & `wordview-1.1.1/wordview/text_analysis/wrapper.py`

 * *Files identical despite different names*

### Comparing `wordview-1.1.0/PKG-INFO` & `wordview-1.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wordview
-Version: 1.1.0
+Version: 1.1.1
 Summary: Wordview is a Python package for text analysis.
 License: MIT
 Keywords: nlp,text analysis,statistics
 Author: meghdadFar
 Author-email: meghdad.farahmand@gmail.com
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
@@ -32,15 +32,15 @@
 
 .. image:: https://img.shields.io/pypi/pyversions/wordview
    :alt: PyPI - Python Version
 
 .. image:: https://img.shields.io/pypi/dm/wordview
    :alt: PyPI - Downloads
 
-Wordview is a Python package for Exploratory Data Analysis (EDA) and Feature Extraction for text.
+Wordview is a Python package for Exploratory Data Analysis (EDA) of text.
 Wordview's Python API is open-source and available under the `MIT
 license <https://en.wikipedia.org/wiki/MIT_License>`__.
 
 |cover|
 
 
 Usage
@@ -72,43 +72,46 @@
 
 Analysis of Labels
 ******************
 Wordview calculates several statistics for labels in labeled datasets whether they are at document or sequence level.
 See `label analysis documentation pages <./docs/source/labels.rst>`__ for usage and examples.
 
 
-Feature Extraction
-###################
-
-Wordview has various functionalities for feature extraction from text, including Multiword Expressions (MWEs), clusters, anomalies and 
-outliers, and more. See the following sections as well as the linked documentation page in each section for details.
-
-Multiword Expressions
-*********************
-
+Extraction & Analysis of Multiword Expressions
+**********************************************
 Multiword Expressions (MWEs) are phrases that can be treated as a single
 semantic unit. E.g. *swimming pool* and *climate change*. MWEs have
 application in different areas including: parsing, language models,
 language generation, terminology extraction, and topic models. Wordview can extract different types of MWEs from text.
 See `MWEs documentation page <./docs/source/mwes.rst>`__ for usage and examples.
 
-Anomalies and Outliers
-**********************
 
+Bias Analysis
+**************
+In the rapidly evolving realm of Natural Language Processing (NLP), downstream models are as unbiased and fair as the data on which they are trained.
+Wordview Bias Analysis module is designed to assist in the rigorous task of ensuring that underlying training datasets are devoid of explicit negative biases related to categories such as gender, race, and religion.
+By identifying and rectifying these biases, Wordview attempts to pave the way for the creation of more inclusive, fair, and unbiased NLP applications, leading to better user experiences and more equitable technology.
+See the `bias analysis documentation page <./docs/source/bias.rst>`__ for usage and examples.
+
+
+Analysis of Anomalies and Outliers
+**********************************
 Anomalies and outliers have wide applications in Machine Learning. While in
 some cases, you can capture them and remove them from the data to improve the
 performance of a downstream ML model, in other cases, they become the data points
 of interest where we endeavor to find them in order to shed light into our data.
 
 Wordview offers several anomaly and outlier detection functions.
 See `anomalies documentation page <./docs/source/anomalies.rst>`__ for usage and examples.
 
 
-Clusters
-*********
+
+
+Cluster Analysis
+****************
 Clustering can be used to identify different groups of documents with similar information, in an unsupervised fashion.
 Despite it's ability to provide valuable insights into your data, you do not need labeled data for clustering. See
 `wordview`'s `clustering documentation page <./docs/source/clustering.rst>`__ for usage and examples.
 
 
 Utilities
 #########
```

