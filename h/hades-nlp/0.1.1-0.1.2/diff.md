# Comparing `tmp/hades_nlp-0.1.1.tar.gz` & `tmp/hades_nlp-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hades_nlp-0.1.1.tar", max compression
+gzip compressed data, was "hades_nlp-0.1.2.tar", max compression
```

## Comparing `hades_nlp-0.1.1.tar` & `hades_nlp-0.1.2.tar`

### file list

```diff
@@ -1,33 +1,32 @@
--rw-r--r--   0        0        0        0 2023-02-24 19:39:47.784992 hades_nlp-0.1.1/hades/__init__.py
--rw-r--r--   0        0        0      117 2023-02-24 19:39:47.785992 hades_nlp-0.1.1/hades/data_loading/__init__.py
--rw-r--r--   0        0        0     4372 2023-02-24 19:39:47.785992 hades_nlp-0.1.1/hades/data_loading/load_data.py
--rw-r--r--   0        0        0     9315 2023-02-24 19:39:47.786992 hades_nlp-0.1.1/hades/data_loading/utils.py
--rw-r--r--   0        0        0        0 2023-02-24 19:39:47.786992 hades_nlp-0.1.1/hades/plots/__init__.py
--rw-r--r--   0        0        0     1280 2023-02-24 19:39:47.787994 hades_nlp-0.1.1/hades/plots/simple_plots.py
--rw-r--r--   0        0        0     4022 2023-02-24 19:39:47.788995 hades_nlp-0.1.1/hades/plots/topics.py
--rw-r--r--   0        0        0      209 2023-02-24 19:39:47.788995 hades_nlp-0.1.1/hades/summaries/__init__.py
--rw-r--r--   0        0        0     3082 2023-02-24 19:39:47.789992 hades_nlp-0.1.1/hades/summaries/summarize.py
--rw-r--r--   0        0        0      109 2023-02-24 19:39:47.790994 hades_nlp-0.1.1/hades/topic_analysis/__init__.py
--rw-r--r--   0        0        0     3146 2023-02-24 19:39:47.790994 hades_nlp-0.1.1/hades/topic_analysis/cca.py
--rw-r--r--   0        0        0     3925 2023-02-24 19:39:47.792224 hades_nlp-0.1.1/hades/topic_analysis/sentence_topic_analyser.py
--rw-r--r--   0        0        0      478 2023-02-24 19:39:47.793232 hades_nlp-0.1.1/hades/topic_analysis/stats.py
--rw-r--r--   0        0        0       78 2023-02-24 19:39:47.793232 hades_nlp-0.1.1/hades/topic_modeling/__init__.py
--rw-r--r--   0        0        0     5468 2023-02-24 19:39:47.794238 hades_nlp-0.1.1/hades/topic_modeling/model.py
--rw-r--r--   0        0        0      126 2023-02-24 19:39:47.794238 hades_nlp-0.1.1/hades/topic_modeling/model_optimizer/__init__.py
--rw-r--r--   0        0        0    11999 2023-02-24 19:39:47.795245 hades_nlp-0.1.1/hades/topic_modeling/model_optimizer/model_optimizer.py
--rw-r--r--   0        0        0     6638 2023-02-24 19:39:47.795245 hades_nlp-0.1.1/hades/topic_modeling/model_optimizer/utils.py
--rw-r--r--   0        0        0     1710 2023-02-24 19:39:47.796252 hades_nlp-0.1.1/hades/topic_modeling/topic_probs.py
--rw-r--r--   0        0        0     3055 2023-02-24 19:39:47.796252 hades_nlp-0.1.1/hades/topic_modeling/utils.py
--rw-r--r--   0        0        0        0 2023-02-24 19:39:47.797268 hades_nlp-0.1.1/hades_app/__init__.py
--rw-r--r--   0        0        0     2729 2023-02-24 19:39:47.798293 hades_nlp-0.1.1/hades_app/config.py
--rw-r--r--   0        0        0    17619 2023-02-24 19:39:47.799314 hades_nlp-0.1.1/hades_app/main.py
--rw-r--r--   0        0        0     1063 2023-02-24 19:39:47.799314 hades_nlp-0.1.1/hades_app/run_app.py
--rw-r--r--   0        0        0      629 2023-02-24 19:39:47.800339 hades_nlp-0.1.1/hades_app/utils/__init__.py
--rw-r--r--   0        0        0     2001 2023-02-24 19:39:47.800339 hades_nlp-0.1.1/hades_app/utils/clustering.py
--rw-r--r--   0        0        0    11878 2023-02-24 19:39:47.801347 hades_nlp-0.1.1/hades_app/utils/plots.py
--rw-r--r--   0        0        0      388 2023-02-24 19:39:47.801347 hades_nlp-0.1.1/hades_app/utils/stats.py
--rw-r--r--   0        0        0     1084 2023-02-24 19:42:45.537227 hades_nlp-0.1.1/LICENSE
--rw-r--r--   0        0        0     1442 2023-02-24 20:52:17.016768 hades_nlp-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4176 2023-02-24 20:27:55.043393 hades_nlp-0.1.1/README.md
--rw-r--r--   0        0        0     5926 1970-01-01 00:00:00.000000 hades_nlp-0.1.1/setup.py
--rw-r--r--   0        0        0     5736 1970-01-01 00:00:00.000000 hades_nlp-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-25 12:19:54.558324 hades_nlp-0.1.2/hades/__init__.py
+-rw-r--r--   0        0        0      161 2023-08-07 09:04:21.573634 hades_nlp-0.1.2/hades/data_loading/__init__.py
+-rw-r--r--   0        0        0     4372 2023-07-25 12:19:54.559326 hades_nlp-0.1.2/hades/data_loading/load_data.py
+-rw-r--r--   0        0        0     9315 2023-07-25 12:19:54.559326 hades_nlp-0.1.2/hades/data_loading/utils.py
+-rw-r--r--   0        0        0        0 2023-07-25 12:19:54.560325 hades_nlp-0.1.2/hades/plots/__init__.py
+-rw-r--r--   0        0        0     1280 2023-07-25 12:19:54.561327 hades_nlp-0.1.2/hades/plots/simple_plots.py
+-rw-r--r--   0        0        0     4022 2023-07-25 12:19:54.561327 hades_nlp-0.1.2/hades/plots/topics.py
+-rw-r--r--   0        0        0      209 2023-07-25 12:19:54.562471 hades_nlp-0.1.2/hades/summaries/__init__.py
+-rw-r--r--   0        0        0     3080 2023-08-07 07:03:38.388326 hades_nlp-0.1.2/hades/summaries/summarize.py
+-rw-r--r--   0        0        0      109 2023-07-25 12:19:54.563479 hades_nlp-0.1.2/hades/topic_analysis/__init__.py
+-rw-r--r--   0        0        0     3146 2023-07-25 12:19:54.563479 hades_nlp-0.1.2/hades/topic_analysis/cca.py
+-rw-r--r--   0        0        0     3925 2023-07-25 12:19:54.563479 hades_nlp-0.1.2/hades/topic_analysis/sentence_topic_analyser.py
+-rw-r--r--   0        0        0      478 2023-07-25 12:19:54.564481 hades_nlp-0.1.2/hades/topic_analysis/stats.py
+-rw-r--r--   0        0        0       78 2023-08-07 06:59:16.247376 hades_nlp-0.1.2/hades/topic_modeling/__init__.py
+-rw-r--r--   0        0        0     5468 2023-07-26 21:03:14.630064 hades_nlp-0.1.2/hades/topic_modeling/model.py
+-rw-r--r--   0        0        0      126 2023-08-07 06:59:16.249375 hades_nlp-0.1.2/hades/topic_modeling/model_optimizer/__init__.py
+-rw-r--r--   0        0        0    12187 2023-08-07 07:05:22.191961 hades_nlp-0.1.2/hades/topic_modeling/model_optimizer/model_optimizer.py
+-rw-r--r--   0        0        0     6638 2023-08-07 06:59:16.253808 hades_nlp-0.1.2/hades/topic_modeling/model_optimizer/utils.py
+-rw-r--r--   0        0        0     1710 2023-07-25 12:19:54.566482 hades_nlp-0.1.2/hades/topic_modeling/topic_probs.py
+-rw-r--r--   0        0        0     3055 2023-07-25 12:19:54.567842 hades_nlp-0.1.2/hades/topic_modeling/utils.py
+-rw-r--r--   0        0        0        0 2023-07-25 12:19:54.567842 hades_nlp-0.1.2/hades_app/__init__.py
+-rw-r--r--   0        0        0     2729 2023-07-25 12:19:54.568853 hades_nlp-0.1.2/hades_app/config.py
+-rw-r--r--   0        0        0    17588 2023-07-26 21:15:53.080612 hades_nlp-0.1.2/hades_app/main.py
+-rw-r--r--   0        0        0     1063 2023-07-25 12:19:54.570851 hades_nlp-0.1.2/hades_app/run_app.py
+-rw-r--r--   0        0        0      629 2023-07-25 12:19:54.571851 hades_nlp-0.1.2/hades_app/utils/__init__.py
+-rw-r--r--   0        0        0     1981 2023-07-26 21:16:32.500455 hades_nlp-0.1.2/hades_app/utils/clustering.py
+-rw-r--r--   0        0        0    11878 2023-07-25 12:19:54.572878 hades_nlp-0.1.2/hades_app/utils/plots.py
+-rw-r--r--   0        0        0      388 2023-07-25 12:19:54.572878 hades_nlp-0.1.2/hades_app/utils/stats.py
+-rw-r--r--   0        0        0     1084 2023-07-25 12:19:54.556327 hades_nlp-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1459 2023-08-07 11:09:03.227958 hades_nlp-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4174 2023-08-07 11:09:43.675739 hades_nlp-0.1.2/README.md
+-rw-r--r--   0        0        0     5830 1970-01-01 00:00:00.000000 hades_nlp-0.1.2/PKG-INFO
```

### Comparing `hades_nlp-0.1.1/hades/data_loading/load_data.py` & `hades_nlp-0.1.2/hades/data_loading/load_data.py`

 * *Files identical despite different names*

### Comparing `hades_nlp-0.1.1/hades/data_loading/utils.py` & `hades_nlp-0.1.2/hades/data_loading/utils.py`

 * *Files identical despite different names*

### Comparing `hades_nlp-0.1.1/hades/plots/simple_plots.py` & `hades_nlp-0.1.2/hades/plots/simple_plots.py`

 * *Files identical despite different names*

### Comparing `hades_nlp-0.1.1/hades/plots/topics.py` & `hades_nlp-0.1.2/hades/plots/topics.py`

 * *Files identical despite different names*

### Comparing `hades_nlp-0.1.1/hades/summaries/summarize.py` & `hades_nlp-0.1.2/hades/summaries/summarize.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 
 def extract_n_most_important_sentences(text: str, n_of_sentences: int) -> str:
     """Function extracting n most important sentences from text using BERT model"""
     result = model(text, num_sentences=n_of_sentences)
     return result
 
 
-def abstractive_summary(extractive_summary: str, gpt3_model: str = "text-davinci-003", temperature: int = 0.7) -> str:
+def abstractive_summary(extractive_summary: str, gpt_model: str = "text-davinci-003", temperature: int = 0.7) -> str:
     """Function making abstractive summaries out of previously extracted most important sentences"""
     prompt = extractive_summary + ' Summarize the text above in three sentences: \n'
-    response = openai.Completion.create(model=gpt3_model, prompt=prompt, temperature=temperature, max_tokens=120)
+    response = openai.Completion.create(model=gpt_model, prompt=prompt, temperature=temperature, max_tokens=120)
     return response['choices'][0]['text']
 
 
 def make_summary(text: str, n_extract_sentences: int) -> str:
     """
     Function making abstractive summaries out of previously extracted most important sentences
     Args:
```

### Comparing `hades_nlp-0.1.1/hades/topic_analysis/cca.py` & `hades_nlp-0.1.2/hades/topic_analysis/cca.py`

 * *Files identical despite different names*

### Comparing `hades_nlp-0.1.1/hades/topic_analysis/sentence_topic_analyser.py` & `hades_nlp-0.1.2/hades/topic_analysis/sentence_topic_analyser.py`

 * *Files identical despite different names*

### Comparing `hades_nlp-0.1.1/hades/topic_modeling/model.py` & `hades_nlp-0.1.2/hades/topic_modeling/model.py`

 * *Files identical despite different names*

### Comparing `hades_nlp-0.1.1/hades/topic_modeling/model_optimizer/model_optimizer.py` & `hades_nlp-0.1.2/hades/topic_modeling/model_optimizer/model_optimizer.py`

 * *Files 5% similar despite different names*

```diff
@@ -174,35 +174,35 @@
             value.replace(":", "").replace(" ", "_").replace(",", "").replace("/", "_").replace("(", "").replace(
                 ")", "").replace("&", "").replace("-", "_") for value in self.column_filter.values()
         ])
         self.encoded_docs.to_csv(path + filter_name + "_encoded_docs.csv")
         self.lemmas_dictionary.save(path + filter_name + "_dictionary.dict")
         self.best_model.save(path + filter_name + "_lda_model.model")
 
-    def name_topics_automatically_gpt3(
+    def name_topics_automatically(
         self,
         num_keywords: int = 15,
-        gpt3_model: str = "text-davinci-003",
+        gpt_model: str = "text-davinci-003",
         temperature: int = 0.5,
     ):
-        """Generate topic names using GPT-3 model."""
+        """Generate topic names using GPT model."""
         if openai.api_key == None:
             warnings.warn("""
                 Topic names not updated: no api key set;
                 Key can be set using function set_openai_key(key)
                 Organization can be set using function set_openai_organization(organization)
                 """)
             return
         topics_keywords = self.get_topics_df(num_keywords)
         exculded = []
         for i in range(self.topics_num):
             keywords = topics_keywords[topics_keywords["topic_id"] == i].word.to_list()
             weights = topics_keywords[topics_keywords["topic_id"] == i].importance.to_list()
             prompt = _generate_prompt(keywords, weights, exculded)
-            title = _generate_title(prompt, gpt3_model, temperature)
+            title = _generate_title(prompt, gpt_model, temperature)
             self.topic_names_dict[i] = title
             exculded.append(title)
 
     def name_topics_manually(self, topic_names: Union[List[str], Dict[int, str]]):
         """Manually name topics."""
         if isinstance(topic_names, list):
             dict_update = {i: topic_names[i] for i in range(len(topic_names))}
@@ -211,14 +211,19 @@
         updated_dict = deepcopy(self.topic_names_dict)
         updated_dict.update(dict_update)
         if updated_dict.keys() == self.topic_names_dict.keys():
             self.topic_names_dict = updated_dict
         else:
             warnings.warn("Topic names not updated: incorrect topic names given")
 
+    def get_topic_names(self):
+        """Prints topic names."""
+        for topic_id in range(len(self.topic_names_dict)):
+            print(f"{topic_id}:", self.topic_names_dict[topic_id])
+
 
 def get_best_topics_num(cvs: Dict[int, float]) -> int:
     """Returns best number of topics based on coherence values."""
     return max(cvs, key=cvs.get)
 
 
 def get_models(
```

### Comparing `hades_nlp-0.1.1/hades/topic_modeling/model_optimizer/utils.py` & `hades_nlp-0.1.2/hades/topic_modeling/model_optimizer/utils.py`

 * *Files identical despite different names*

### Comparing `hades_nlp-0.1.1/hades/topic_modeling/topic_probs.py` & `hades_nlp-0.1.2/hades/topic_modeling/topic_probs.py`

 * *Files identical despite different names*

### Comparing `hades_nlp-0.1.1/hades/topic_modeling/utils.py` & `hades_nlp-0.1.2/hades/topic_modeling/utils.py`

 * *Files identical despite different names*

### Comparing `hades_nlp-0.1.1/hades_app/config.py` & `hades_nlp-0.1.2/hades_app/config.py`

 * *Files identical despite different names*

### Comparing `hades_nlp-0.1.1/hades_app/main.py` & `hades_nlp-0.1.2/hades_app/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     f = open(file_path)
     j = json.load(f)
     f.close()
     return j
 
 
 @click.command()
-@click.option('--config-path', default='dupa', help='Path to config.json file.')
+@click.option('--config-path', default='config.json', help='Path to config.json file.')
 def main(config_path: str):
     config = Config(config_path)
     if 'en' not in st.session_state:
             st.session_state.en =  spacy.load('en_core_web_sm')
 
     st.markdown(
         f"""
@@ -193,16 +193,16 @@
                 "Select option",
                 config.metric_choices.keys(),
                 format_func=lambda x: config.metric_choices[x],
                 index=0,
             )
             min_cluster_size = st.number_input(
                 f"Select minimum cluster size",
-                min_value=1,
-                value=5,
+                min_value=2,
+                value=2,
             )
             min_samples = st.number_input(
                 f"Select minimum number of samples",
                 min_value=1,
                 value=1,
             )
             cluster_selection_epsilon = st.number_input(
@@ -281,15 +281,15 @@
     with tabs[0]:
         selected_document = st.selectbox("Select document", sorted(topics[config.id_column].unique()), index=0)
         st.header(f"Document details: {selected_document}")
 
         st.markdown(f"""<h4 style="padding-top: 0px;">Section summary:</h4>""", unsafe_allow_html=True)
         st.write(summaries[selected_section][selected_document])
         st.markdown(f"""<hr style='margin: 0px;'>""", unsafe_allow_html=True)
-        clean_topics = [topic_name.split(" ", 1)[1] for topic_name in topic_names]
+        clean_topics =  list(topic_names)
         selected_topic = st.selectbox(
             "Select topic",
             clean_topics,
             index=0)
         topic_num = 0
         for idx, topic in enumerate(clean_topics):
             if selected_topic == topic:
@@ -303,15 +303,15 @@
             for word in ess_sentence_splitted:
                 word_en = st.session_state.en(word)
                 is_imp = bool(word_en[0].lemma_ in ess_words)
                 if is_imp:
                     sentence.append((
                         str(word),
                         str(np.round(100*essential_sentences[selected_document][str(topic_num)]['words'][word_en[0].lemma_], 2)),
-                        "#afa"))
+                        "#ff4b4b"))
                 else:
                     sentence.append(str(word + " "))
             annotated_text(*sentence)
             st.markdown(f"""</br>""", unsafe_allow_html=True)
 
         st.header(f"Compare documents")
         selected_entities = st.multiselect(
```

### Comparing `hades_nlp-0.1.1/hades_app/run_app.py` & `hades_nlp-0.1.2/hades_app/run_app.py`

 * *Files identical despite different names*

### Comparing `hades_nlp-0.1.1/hades_app/utils/__init__.py` & `hades_nlp-0.1.2/hades_app/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hades_nlp-0.1.1/hades_app/utils/clustering.py` & `hades_nlp-0.1.2/hades_app/utils/clustering.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from typing import Callable, Union
 import numpy as np
 import pandas as pd
 import scipy.cluster.hierarchy as hc
-from sklearn.cluster import KMeans
+from sklearn.cluster import KMeans, HDBSCAN
 import scipy.spatial as sp
-from hdbscan import HDBSCAN
 
 
 def calculate_linkage_matrix(
     topic_probs: pd.DataFrame, method: str = "average", metric: str = "cosine"
 ) -> np.ndarray:
     return hc.linkage(topic_probs, method=method, metric=_get_metric(metric))
 
@@ -40,15 +39,15 @@
                         random_state: int = 42) -> np.ndarray:
     kmeans = KMeans(n_clusters=n_clusters, random_state=random_state, n_init=n_init).fit(topic_probs)
     return kmeans.labels_
 
 
 def get_hdbscan_clusters(
     distance_matrix: pd.DataFrame,
-    min_cluster_size: int = 5,
+    min_cluster_size: int = 2,
     min_samples: int = None,
     cluster_selection_epsilon: int = 0.0,
 ):
     hdbscan = HDBSCAN(
         metric="precomputed",
         min_cluster_size=min_cluster_size,
         min_samples=min_samples,
```

### Comparing `hades_nlp-0.1.1/hades_app/utils/plots.py` & `hades_nlp-0.1.2/hades_app/utils/plots.py`

 * *Files identical despite different names*

### Comparing `hades_nlp-0.1.1/LICENSE` & `hades_nlp-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hades_nlp-0.1.1/pyproject.toml` & `hades_nlp-0.1.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,47 +1,48 @@
 [tool.poetry]
 name = "hades-nlp"
-version = "0.1.1"
+version = "0.1.2"
 description = "Homologous Automated Document Exploration and Summarization - A powerful tool for comparing similarly structured documents"
 authors = ["Artur Żółkowski <artur.zolkowski@wp.pl>", "Piotr Wilczyński <piotrwil288@gmail.com>", "Mateusz Krzyziński <krzyzinskimateusz23@gmail.com>", "Emilia Wiśnios <wisniosemilia@gmail.com>"]
 packages = [
     { include = "hades"},
     { include = "hades_app"},
 ]
 keywords = ["nlp", "documents", "topic modeling", "summarization", "machine learning", "natural language processing", "text analysis", "text mining", "text summarization"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 hades = "hades_app.run_app:cli"
 
 [tool.poetry.dependencies]
-python = "^3.9,<3.9.7||>3.9.7,<3.10"
+python = "^3.9,<3.9.7||>3.9.7,<4"
 pandas = "^1.4.3"
 numpy = "^1.23.1"
 spacy = "^3.3.1"
 black = "^22.6.0"
 scipy = "^1.8.1"
-gensim = "^4.2.0"
+gensim = "^4.3.1"
 swifter = "^1.2.0"
 PyPDF2 = "^2.6.0"
-matplotlib = "^3.5.2"
-seaborn = "^0.11.2"
+matplotlib = ">3.5.2"
+seaborn = ">=0.12.2"
 pyLDAvis = "^3.3.1"
-hdbscan = "^0.8.28"
 pycountry = "^22.3.5"
 statsmodels = "^0.13.2"
 openai = "^0.23.0"
 umap-learn = "^0.5.3"
-llvmlite = "0.39.1"
+llvmlite = "^0.40.1"
 streamlit = "1.16.0"
 contextualized-topic-models = "^2.4.2"
 st-annotated-text = "^3.0.0"
 click = "^8.1.3"
 bert-extractive-summarizer = "^0.10.1"
 plotly = "^5.9.0"
+setuptools = ">58.1.0"
+altair = "<5"
 
 [tool.black]
 line-length = 100
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `hades_nlp-0.1.1/README.md` & `hades_nlp-0.1.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 ## Overview
 `HADES` is a **Python** package for comparing similarly structured documents. HADES is designed to streamline the work of professionals dealing with large volumes of documents, such as policy documents, legal acts, and scientific papers. The tool employs a multi-step pipeline that begins with processing PDF documents using topic modeling, summarization, and analysis of the most important words for each topic. The process concludes with an interactive web app with visualizations that facilitate the comparison of the documents. HADES has the potential to significantly improve the productivity of professionals dealing with high volumes of documents, reducing the time and effort required to complete tasks related to comparative document analysis.
 
 ## Installation
 Latest released version of the `HADES` package is available on [Python Package Index (PyPI)](https://pypi.org/project/hades-nlp/):
 
-1. Install spacy `en-core-web-lg` and `en-core-web-sm` models for English language according to the [instructions](https://spacy.io/models/en)
+1. Install spacy `en-core-web-sm` or `en-core-web-lg` model for English language according to the [instructions](https://spacy.io/models/en)
 
 2. Install `HADES` package using pip:
 
 ```sh
 pip install -U hades-nlp
 ```
 The source code and development version is currently hosted on [GitHub](https://github.com/MI2DataLab/HADES).
```

### Comparing `hades_nlp-0.1.1/setup.py` & `hades_nlp-0.1.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,64 +1,115 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: hades-nlp
+Version: 0.1.2
+Summary: Homologous Automated Document Exploration and Summarization - A powerful tool for comparing similarly structured documents
+Keywords: nlp,documents,topic modeling,summarization,machine learning,natural language processing,text analysis,text mining,text summarization
+Author: Artur Żółkowski
+Author-email: artur.zolkowski@wp.pl
+Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: PyPDF2 (>=2.6.0,<3.0.0)
+Requires-Dist: altair (<5)
+Requires-Dist: bert-extractive-summarizer (>=0.10.1,<0.11.0)
+Requires-Dist: black (>=22.6.0,<23.0.0)
+Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: contextualized-topic-models (>=2.4.2,<3.0.0)
+Requires-Dist: gensim (>=4.3.1,<5.0.0)
+Requires-Dist: llvmlite (>=0.40.1,<0.41.0)
+Requires-Dist: matplotlib (>3.5.2)
+Requires-Dist: numpy (>=1.23.1,<2.0.0)
+Requires-Dist: openai (>=0.23.0,<0.24.0)
+Requires-Dist: pandas (>=1.4.3,<2.0.0)
+Requires-Dist: plotly (>=5.9.0,<6.0.0)
+Requires-Dist: pyLDAvis (>=3.3.1,<4.0.0)
+Requires-Dist: pycountry (>=22.3.5,<23.0.0)
+Requires-Dist: scipy (>=1.8.1,<2.0.0)
+Requires-Dist: seaborn (>=0.12.2)
+Requires-Dist: setuptools (>58.1.0)
+Requires-Dist: spacy (>=3.3.1,<4.0.0)
+Requires-Dist: st-annotated-text (>=3.0.0,<4.0.0)
+Requires-Dist: statsmodels (>=0.13.2,<0.14.0)
+Requires-Dist: streamlit (==1.16.0)
+Requires-Dist: swifter (>=1.2.0,<2.0.0)
+Requires-Dist: umap-learn (>=0.5.3,<0.6.0)
+Description-Content-Type: text/markdown
+
+# HADES: Homologous Automated Document Exploration and Summarization
+A powerful tool for comparing similarly structured documents
+
+[![PyPI version](https://badge.fury.io/py/hades-nlp.svg)](https://pypi.org/project/hades-nlp/)
+[![Downloads](https://static.pepy.tech/badge/hades-nlp)](https://pepy.tech/project/hades-nlp)
+
+## Overview
+`HADES` is a **Python** package for comparing similarly structured documents. HADES is designed to streamline the work of professionals dealing with large volumes of documents, such as policy documents, legal acts, and scientific papers. The tool employs a multi-step pipeline that begins with processing PDF documents using topic modeling, summarization, and analysis of the most important words for each topic. The process concludes with an interactive web app with visualizations that facilitate the comparison of the documents. HADES has the potential to significantly improve the productivity of professionals dealing with high volumes of documents, reducing the time and effort required to complete tasks related to comparative document analysis.
+
+## Installation
+Latest released version of the `HADES` package is available on [Python Package Index (PyPI)](https://pypi.org/project/hades-nlp/):
+
+1. Install spacy `en-core-web-sm` or `en-core-web-lg` model for English language according to the [instructions](https://spacy.io/models/en)
+
+2. Install `HADES` package using pip:
+
+```sh
+pip install -U hades-nlp
+```
+The source code and development version is currently hosted on [GitHub](https://github.com/MI2DataLab/HADES).
+## Usage
+The `HADES` package is designed to be used in a Python environment. The package can be imported as follows:
+
+```python
+from hades.data_loading import load_processed_data
+from hades.topic_modeling import ModelOptimizer, save_data_for_app, set_openai_key
+from my_documents_data import PARAGRAPHS, COMMON_WORDS, STOPWORDS
+```
+The `load_processed_data` function loads the documents to be processed. The `ModelOptimizer` class is used to optimize the topic modeling process. The `save_data_for_app` function saves the data for the interactive web app. The `set_openai_key` function sets the OpenAI API key.
+`my_documents_data` contains the informations about the documents to be processed. The `PARAGRAPHS` variable is a list of strings that represent the paragraphs of the documents. The `COMMON_WORDS` variable is a list of strings that represent the most common words in the documents. The `STOPWORDS` variable is a list of strings that represent the most common words in the documents that should be excluded from the analysis.
+
+First, the documents are loaded and processed:
+```python
+set_openai_key("my openai key")
+data_path = "my/data/path"
+processed_df = load_processed_data(
+    data_path=data_path,
+    stop_words=STOPWORDS,
+    id_column='country',
+    flattened_by_col='my_column',
+)
+```
+After the documents are loaded, the topic modeling process is optimized for each paragraph:
+```python
+model_optimizers = []
+for paragraph in PARAGRAPHS:
+    filter_dict = {'paragraph': paragraph}
+    model_optimizer = ModelOptimizer(
+        processed_df,
+        'country',
+        'section',
+        filter_dict,
+        "lda",
+        COMMON_WORDS[paragraph],
+        (3,6),
+        alpha=100
+    )
+    model_optimizer.name_topics_automatically_gpt3()
+    model_optimizers.append(model_optimizer)
+
+```
+For each paragraph, the `ModelOptimizer` class is used to optimize the topic modeling process. The `name_topics_automatically_gpt3` function automatically names the topics using the OpenAI GPT-3 API. User can also use the `name_topics_manually` function to manually name the topics.
+
+Finally, the data is saved for the interactive web app:
+```python
+save_data_for_app(model_optimizers, path='path/to/results', do_summaries=True)
+```
+The `save_data_for_app` function saves the data for the interactive web app. The `do_summaries` parameter is set to `True` to generate summaries for each topic.
+
+When the data is saved, the interactive web app can be launched:
+```sh
+hades run-app --config path/to/results/config.json
+```
 
-packages = \
-['hades',
- 'hades.data_loading',
- 'hades.plots',
- 'hades.summaries',
- 'hades.topic_analysis',
- 'hades.topic_modeling',
- 'hades.topic_modeling.model_optimizer',
- 'hades_app',
- 'hades_app.utils']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['PyPDF2>=2.6.0,<3.0.0',
- 'bert-extractive-summarizer>=0.10.1,<0.11.0',
- 'black>=22.6.0,<23.0.0',
- 'click>=8.1.3,<9.0.0',
- 'contextualized-topic-models>=2.4.2,<3.0.0',
- 'gensim>=4.2.0,<5.0.0',
- 'hdbscan>=0.8.28,<0.9.0',
- 'llvmlite==0.39.1',
- 'matplotlib>=3.5.2,<4.0.0',
- 'numpy>=1.23.1,<2.0.0',
- 'openai>=0.23.0,<0.24.0',
- 'pandas>=1.4.3,<2.0.0',
- 'plotly>=5.9.0,<6.0.0',
- 'pyLDAvis>=3.3.1,<4.0.0',
- 'pycountry>=22.3.5,<23.0.0',
- 'scipy>=1.8.1,<2.0.0',
- 'seaborn>=0.11.2,<0.12.0',
- 'spacy>=3.3.1,<4.0.0',
- 'st-annotated-text>=3.0.0,<4.0.0',
- 'statsmodels>=0.13.2,<0.14.0',
- 'streamlit==1.16.0',
- 'swifter>=1.2.0,<2.0.0',
- 'umap-learn>=0.5.3,<0.6.0']
-
-entry_points = \
-{'console_scripts': ['hades = hades_app.run_app:cli']}
-
-setup_kwargs = {
-    'name': 'hades-nlp',
-    'version': '0.1.1',
-    'description': 'Homologous Automated Document Exploration and Summarization - A powerful tool for comparing similarly structured documents',
-    'long_description': '# HADES: Homologous Automated Document Exploration and Summarization\nA powerful tool for comparing similarly structured documents\n\n[![PyPI version](https://badge.fury.io/py/hades-nlp.svg)](https://pypi.org/project/hades-nlp/)\n[![Downloads](https://static.pepy.tech/badge/hades-nlp)](https://pepy.tech/project/hades-nlp)\n\n## Overview\n`HADES` is a **Python** package for comparing similarly structured documents. HADES is designed to streamline the work of professionals dealing with large volumes of documents, such as policy documents, legal acts, and scientific papers. The tool employs a multi-step pipeline that begins with processing PDF documents using topic modeling, summarization, and analysis of the most important words for each topic. The process concludes with an interactive web app with visualizations that facilitate the comparison of the documents. HADES has the potential to significantly improve the productivity of professionals dealing with high volumes of documents, reducing the time and effort required to complete tasks related to comparative document analysis.\n\n## Installation\nLatest released version of the `HADES` package is available on [Python Package Index (PyPI)](https://pypi.org/project/hades-nlp/):\n\n1. Install spacy `en-core-web-lg` and `en-core-web-sm` models for English language according to the [instructions](https://spacy.io/models/en)\n\n2. Install `HADES` package using pip:\n\n```sh\npip install -U hades-nlp\n```\nThe source code and development version is currently hosted on [GitHub](https://github.com/MI2DataLab/HADES).\n## Usage\nThe `HADES` package is designed to be used in a Python environment. The package can be imported as follows:\n\n```python\nfrom hades.data_loading import load_processed_data\nfrom hades.topic_modeling import ModelOptimizer, save_data_for_app, set_openai_key\nfrom my_documents_data import PARAGRAPHS, COMMON_WORDS, STOPWORDS\n```\nThe `load_processed_data` function loads the documents to be processed. The `ModelOptimizer` class is used to optimize the topic modeling process. The `save_data_for_app` function saves the data for the interactive web app. The `set_openai_key` function sets the OpenAI API key.\n`my_documents_data` contains the informations about the documents to be processed. The `PARAGRAPHS` variable is a list of strings that represent the paragraphs of the documents. The `COMMON_WORDS` variable is a list of strings that represent the most common words in the documents. The `STOPWORDS` variable is a list of strings that represent the most common words in the documents that should be excluded from the analysis.\n\nFirst, the documents are loaded and processed:\n```python\nset_openai_key("my openai key")\ndata_path = "my/data/path"\nprocessed_df = load_processed_data(\n    data_path=data_path,\n    stop_words=STOPWORDS,\n    id_column=\'country\',\n    flattened_by_col=\'my_column\',\n)\n```\nAfter the documents are loaded, the topic modeling process is optimized for each paragraph:\n```python\nmodel_optimizers = []\nfor paragraph in PARAGRAPHS:\n    filter_dict = {\'paragraph\': paragraph}\n    model_optimizer = ModelOptimizer(\n        processed_df,\n        \'country\',\n        \'section\',\n        filter_dict,\n        "lda",\n        COMMON_WORDS[paragraph],\n        (3,6),\n        alpha=100\n    )\n    model_optimizer.name_topics_automatically_gpt3()\n    model_optimizers.append(model_optimizer)\n\n```\nFor each paragraph, the `ModelOptimizer` class is used to optimize the topic modeling process. The `name_topics_automatically_gpt3` function automatically names the topics using the OpenAI GPT-3 API. User can also use the `name_topics_manually` function to manually name the topics.\n\nFinally, the data is saved for the interactive web app:\n```python\nsave_data_for_app(model_optimizers, path=\'path/to/results\', do_summaries=True)\n```\nThe `save_data_for_app` function saves the data for the interactive web app. The `do_summaries` parameter is set to `True` to generate summaries for each topic.\n\nWhen the data is saved, the interactive web app can be launched:\n```sh\nhades run-app --config path/to/results/config.json\n```\n\n***\n\n',
-    'author': 'Artur Żółkowski',
-    'author_email': 'artur.zolkowski@wp.pl',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*, !=3.10.*, !=3.11.*',
-}
+***
 
 
-setup(**setup_kwargs)
```

