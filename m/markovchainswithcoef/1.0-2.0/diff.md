# Comparing `tmp/markovchainswithcoef-1.0.tar.gz` & `tmp/markovchainswithcoef-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markovchainswithcoef-1.0.tar", last modified: Tue Aug  1 14:13:16 2023, max compression
+gzip compressed data, was "markovchainswithcoef-2.0.tar", last modified: Mon Aug  7 11:19:50 2023, max compression
```

## Comparing `markovchainswithcoef-1.0.tar` & `markovchainswithcoef-2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-08-01 14:13:16.841146 markovchainswithcoef-1.0/
--rw-r--r--   0 mac        (501) staff       (20)    11357 2023-08-01 12:42:22.000000 markovchainswithcoef-1.0/LICENSE
--rw-r--r--   0 mac        (501) staff       (20)      761 2023-08-01 14:13:16.841271 markovchainswithcoef-1.0/PKG-INFO
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-08-01 14:13:16.839449 markovchainswithcoef-1.0/markovchainswithcoef/
--rw-r--r--   0 mac        (501) staff       (20)      233 2023-08-01 14:06:19.000000 markovchainswithcoef-1.0/markovchainswithcoef/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     4787 2023-08-01 13:21:05.000000 markovchainswithcoef-1.0/markovchainswithcoef/markovchains.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-08-01 14:13:16.840886 markovchainswithcoef-1.0/markovchainswithcoef.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)      761 2023-08-01 14:13:16.000000 markovchainswithcoef-1.0/markovchainswithcoef.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      315 2023-08-01 14:13:16.000000 markovchainswithcoef-1.0/markovchainswithcoef.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2023-08-01 14:13:16.000000 markovchainswithcoef-1.0/markovchainswithcoef.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)       35 2023-08-01 14:13:16.000000 markovchainswithcoef-1.0/markovchainswithcoef.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)       21 2023-08-01 14:13:16.000000 markovchainswithcoef-1.0/markovchainswithcoef.egg-info/top_level.txt
--rw-r--r--   0 mac        (501) staff       (20)       38 2023-08-01 14:13:16.841673 markovchainswithcoef-1.0/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)     1146 2023-08-01 14:12:33.000000 markovchainswithcoef-1.0/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-08-07 11:19:50.621822 markovchainswithcoef-2.0/
+-rw-r--r--   0 mac        (501) staff       (20)    11357 2023-08-01 12:42:22.000000 markovchainswithcoef-2.0/LICENSE
+-rw-r--r--   0 mac        (501) staff       (20)      781 2023-08-07 11:19:50.621991 markovchainswithcoef-2.0/PKG-INFO
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-08-07 11:19:50.620230 markovchainswithcoef-2.0/markovchainswithcoef/
+-rw-r--r--   0 mac        (501) staff       (20)      253 2023-08-07 11:17:22.000000 markovchainswithcoef-2.0/markovchainswithcoef/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     6466 2023-08-07 11:15:28.000000 markovchainswithcoef-2.0/markovchainswithcoef/markovchains.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-08-07 11:19:50.621595 markovchainswithcoef-2.0/markovchainswithcoef.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)      781 2023-08-07 11:19:50.000000 markovchainswithcoef-2.0/markovchainswithcoef.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      315 2023-08-07 11:19:50.000000 markovchainswithcoef-2.0/markovchainswithcoef.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2023-08-07 11:19:50.000000 markovchainswithcoef-2.0/markovchainswithcoef.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)       48 2023-08-07 11:19:50.000000 markovchainswithcoef-2.0/markovchainswithcoef.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)       21 2023-08-07 11:19:50.000000 markovchainswithcoef-2.0/markovchainswithcoef.egg-info/top_level.txt
+-rw-r--r--   0 mac        (501) staff       (20)       38 2023-08-07 11:19:50.622396 markovchainswithcoef-2.0/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)     1181 2023-08-07 10:57:02.000000 markovchainswithcoef-2.0/setup.py
```

### Comparing `markovchainswithcoef-1.0/LICENSE` & `markovchainswithcoef-2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `markovchainswithcoef-1.0/PKG-INFO` & `markovchainswithcoef-2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: markovchainswithcoef
-Version: 1.0
+Version: 2.0
 Summary: Add-On to markovclick module for Markov's chain with date-time koef and draw module on pygraphviz
 Home-page: https://github.com/chaparr0/markovchainswithcoef
-Author: chaparr0
+Author: chaparr0 (K.R.V. and K.A.M.)
 Author-email: madeingoa@gmail.com
 License: Apache License, Version 2.0, see LICENSE file
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `markovchainswithcoef-1.0/markovchainswithcoef/markovchains.py` & `markovchainswithcoef-2.0/markovchainswithcoef/markovchains.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 import numpy as np
 from markovclick.models import MarkovClickstream
 import pygraphviz as pgv
 from collections import Counter
 
 from pypdf import PdfWriter, PdfReader
 
+from sklearn.linear_model import LinearRegression
+
+import datetime
+
 class MarkovChainsWC(MarkovClickstream):
 
     def __init__(self, clickstream_list: list = None, prefixed: bool = True, time_cilckstream: list = None,
                  reg_srok_clickstream: list = None) -> object:
 
         self.clickstream_list = clickstream_list
         self.prefixed = prefixed
@@ -29,14 +33,39 @@
 
         self.populate_count_matrix()
         super().compute_prob_matrix()
 
         self.label_node_dict = None
         self.get_label_node()
 
+        self.transition_time_predictions = dict()
+        self.__get_transition_time_predictions()
+
+    def __get_transition_time_predictions(self):
+        flattened_clickstream = list(chain.from_iterable(self.clickstream_list))
+        time_data = np.array([(self.time_cilckstream[i + 1] - self.time_cilckstream[i]).total_seconds() / 3600
+                              for i in range(len(flattened_clickstream) - 1)])
+        X = np.array([[self.pages.index(flattened_clickstream[i]), self.pages.index(flattened_clickstream[i + 1])]
+                      for i in range(len(flattened_clickstream) - 1)])
+        y = time_data.reshape(-1, 1)
+
+        model = LinearRegression()
+        model.fit(X, y)
+
+        for i, page_i in enumerate(self.pages):
+            for j, page_j in enumerate(self.pages):
+                if self.prob_matrix[i,j] == 0:
+                    self.transition_time_predictions[(page_i,page_j)] = None
+                else:
+                    state_pair = np.array([[self.pages.index(page_i), self.pages.index(page_j)]])
+                    predicted_hours = max(0, model.predict(state_pair)[0])
+                    total_seconds = int(predicted_hours * 3600)
+                    time_delta_str = str(datetime.timedelta(seconds=total_seconds))
+                    self.transition_time_predictions[(page_i, page_j)] = time_delta_str
+
     @property
     def count_matrix(self):
         """
         Sets attribute to access the count matrix
         """
         return self._count_matrix
 
@@ -93,26 +122,27 @@
     def draw_node(self,least_percent : float = 0, graph_label : str = '', filename : str = 'result'):
         G = pgv.AGraph(directed=True)
 
         for state in self.pages:
             for transition in self.pages:
                 rate = self.prob_matrix[self.pages.index(state),self.pages.index(transition)]
                 if rate >= least_percent:
+                    transition_time = self.transition_time_predictions.get((state, transition), "N/A")
                     if rate < 0.25:
                         G.add_edge(state, transition,
-                                   label=f"prob = {round(rate, 2)}", color='#93d42a')
+                                   label=f"prob = {round(rate, 2)}\ntime = {transition_time}", color='#93d42a',fontsize=8)
                     elif rate < 0.5:
                         G.add_edge(state, transition,
-                                   label=f"prob = {round(rate, 2)}", color='#2aafd4')
+                                   label=f"prob = {round(rate, 2)}\ntime = {transition_time}", color='#2aafd4',fontsize=8)
                     elif rate < 0.75:
                         G.add_edge(state, transition,
-                                   label=f"prob = {round(rate, 2)}", color='#d4a62a')
+                                   label=f"prob = {round(rate, 2)}\ntime = {transition_time}", color='#d4a62a',fontsize=8)
                     elif rate > 0.75:
                         G.add_edge(state, transition,
-                                   label=f"prob = {round(rate, 2)}", color='#d42a2a')
+                                   label=f"prob = {round(rate, 2)}\ntime = {transition_time}", color='#d42a2a',fontsize=8)
 
         for key,value in self.label_node_dict.items():
             try:
                 n = G.get_node(key)
                 n.attr['label'] = f'{key} ({value})'
             except:
                 pass
```

### Comparing `markovchainswithcoef-1.0/markovchainswithcoef.egg-info/PKG-INFO` & `markovchainswithcoef-2.0/markovchainswithcoef.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: markovchainswithcoef
-Version: 1.0
+Version: 2.0
 Summary: Add-On to markovclick module for Markov's chain with date-time koef and draw module on pygraphviz
 Home-page: https://github.com/chaparr0/markovchainswithcoef
-Author: chaparr0
+Author: chaparr0 (K.R.V. and K.A.M.)
 Author-email: madeingoa@gmail.com
 License: Apache License, Version 2.0, see LICENSE file
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `markovchainswithcoef-1.0/setup.py` & `markovchainswithcoef-2.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,41 +3,41 @@
 
 """
 :authors: chaparr0
 :license: Apache License, Version 2.0, see LICENSE file
 :copyright: (c) 2023 chaparr0
 """
 
-version = '1.0'
+version = '2.0'
 
 """
 with open('README.md',encoding='utf-8') as f:
     long_description = f.read()
 """
 
 long_description = """
 Add-On to markovclick module for Markov's chain with date-time koef and draw module on pygraphviz
 """
 
 setup(
     name='markovchainswithcoef',
     version=version,
 
-    author='chaparr0',
+    author='chaparr0 (K.R.V. and K.A.M.)',
     author_email='madeingoa@gmail.com',
 
     description=long_description,
     long_description=long_description,
 
     url='https://github.com/chaparr0/markovchainswithcoef',
 
     license='Apache License, Version 2.0, see LICENSE file',
 
     packages=['markovchainswithcoef'],
-    install_requires=['numpy','markovclick','pygraphviz','pypdf'],
+    install_requires=['numpy','markovclick','pygraphviz','pypdf','scikit-learn'],
 
     classifiers=[
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
```

