# Comparing `tmp/sen2vec-1.70.tar.gz` & `tmp/sen2vec-1.71.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\sen2vec-1.70.tar", last modified: Thu Dec  1 03:34:58 2022, max compression
+gzip compressed data, was "dist\sen2vec-1.71.tar", last modified: Mon Aug  7 07:35:43 2023, max compression
```

## Comparing `sen2vec-1.70.tar` & `sen2vec-1.71.tar`

### file list

```diff
@@ -1,39 +1,23 @@
-drwxrwxrwx   0        0        0        0 2022-12-01 03:34:58.000000 sen2vec-1.70/
--rw-rw-rw-   0        0        0     1575 2022-12-01 03:34:58.000000 sen2vec-1.70/PKG-INFO
--rw-rw-rw-   0        0        0      517 2022-03-26 11:28:46.000000 sen2vec-1.70/README.md
-drwxrwxrwx   0        0        0        0 2022-12-01 03:34:58.000000 sen2vec-1.70/sen2vec/
--rw-rw-rw-   0        0        0      205 2021-12-03 22:52:08.000000 sen2vec-1.70/sen2vec/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-01 03:34:58.000000 sen2vec-1.70/sen2vec/models/
--rw-rw-rw-   0        0        0      421 2022-04-07 01:09:39.000000 sen2vec-1.70/sen2vec/models/__init__.py
--rw-rw-rw-   0        0        0    16896 2021-12-04 01:15:24.000000 sen2vec-1.70/sen2vec/models/__main__.pyd
--rw-rw-rw-   0        0        0    60336 2021-12-04 02:29:13.000000 sen2vec-1.70/sen2vec/models/__main__.so
--rw-rw-rw-   0        0        0   565760 2022-12-01 03:03:05.000000 sen2vec-1.70/sen2vec/models/bert.pyd
--rw-rw-rw-   0        0        0  3094640 2022-12-01 03:14:02.000000 sen2vec-1.70/sen2vec/models/bert.so
--rw-rw-rw-   0        0        0    60416 2022-01-22 09:50:09.000000 sen2vec-1.70/sen2vec/models/file_utils.pyd
--rw-rw-rw-   0        0        0   410712 2022-01-22 09:48:07.000000 sen2vec-1.70/sen2vec/models/file_utils.so
--rw-rw-rw-   0        0        0   300032 2022-01-14 10:41:11.000000 sen2vec-1.70/sen2vec/models/modeling.pyd
--rw-rw-rw-   0        0        0  2540552 2022-01-14 11:25:55.000000 sen2vec-1.70/sen2vec/models/modeling.so
--rw-rw-rw-   0        0        0    12838 2021-12-13 06:23:18.000000 sen2vec-1.70/sen2vec/models/tokenization.py
-drwxrwxrwx   0        0        0        0 2022-12-01 03:34:58.000000 sen2vec-1.70/sen2vec/sampled/
--rw-rw-rw-   0        0        0      128 2021-09-22 02:21:03.000000 sen2vec-1.70/sen2vec/sampled/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-01 03:34:58.000000 sen2vec-1.70/sen2vec/sampled/bertwwm_pretrain/
--rw-rw-rw-   0        0        0        2 2021-09-22 02:21:03.000000 sen2vec-1.70/sen2vec/sampled/bertwwm_pretrain/added_tokens.json
--rw-rw-rw-   0        0        0      647 2021-09-22 02:21:03.000000 sen2vec-1.70/sen2vec/sampled/bertwwm_pretrain/config.json
--rw-rw-rw-   0        0        0       39 2021-09-22 02:21:03.000000 sen2vec-1.70/sen2vec/sampled/bertwwm_pretrain/model_config.txt
--rw-rw-rw-   0        0        0       27 2021-09-22 02:21:03.000000 sen2vec-1.70/sen2vec/sampled/bertwwm_pretrain/model_url.txt
--rw-rw-rw-   0        0        0      112 2021-09-22 02:21:03.000000 sen2vec-1.70/sen2vec/sampled/bertwwm_pretrain/special_tokens_map.json
--rw-rw-rw-   0        0        0       19 2021-09-22 02:21:03.000000 sen2vec-1.70/sen2vec/sampled/bertwwm_pretrain/tokenizer_config.json
--rw-rw-rw-   0        0        0   109540 2021-09-22 02:21:03.000000 sen2vec-1.70/sen2vec/sampled/bertwwm_pretrain/vocab.txt
--rw-rw-rw-   0        0        0     4070 2021-12-03 22:52:08.000000 sen2vec-1.70/sen2vec/sampled/downloader.py
--rw-rw-rw-   0        0        0    11955 2022-05-27 21:49:16.000000 sen2vec-1.70/sen2vec/sen2vec.py
-drwxrwxrwx   0        0        0        0 2022-12-01 03:34:58.000000 sen2vec-1.70/sen2vec/util/
--rw-rw-rw-   0        0        0      124 2021-09-22 02:21:03.000000 sen2vec-1.70/sen2vec/util/__init__.py
--rw-rw-rw-   0        0        0     5267 2022-05-24 23:10:53.000000 sen2vec-1.70/sen2vec/util/tools.py
--rw-rw-rw-   0        0        0     3432 2022-02-27 05:23:50.000000 sen2vec-1.70/sen2vec/util/utils.py
-drwxrwxrwx   0        0        0        0 2022-12-01 03:34:58.000000 sen2vec-1.70/sen2vec.egg-info/
--rw-rw-rw-   0        0        0     1575 2022-12-01 03:34:58.000000 sen2vec-1.70/sen2vec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      930 2022-12-01 03:34:58.000000 sen2vec-1.70/sen2vec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-01 03:34:58.000000 sen2vec-1.70/sen2vec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2022-12-01 03:34:58.000000 sen2vec-1.70/sen2vec.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-12-01 03:34:58.000000 sen2vec-1.70/setup.cfg
--rw-rw-rw-   0        0        0     3325 2022-12-01 02:58:14.000000 sen2vec-1.70/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 07:35:43.000000 sen2vec-1.71/
+-rw-rw-rw-   0        0        0     1763 2023-08-07 07:35:43.000000 sen2vec-1.71/PKG-INFO
+-rw-rw-rw-   0        0        0      517 2022-03-26 11:28:46.000000 sen2vec-1.71/README.md
+drwxrwxrwx   0        0        0        0 2023-08-07 07:35:43.000000 sen2vec-1.71/sen2vec/
+-rw-rw-rw-   0        0        0      205 2021-12-03 22:52:08.000000 sen2vec-1.71/sen2vec/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-07 07:35:43.000000 sen2vec-1.71/sen2vec/models/
+-rw-rw-rw-   0        0        0      421 2022-04-07 01:09:39.000000 sen2vec-1.71/sen2vec/models/__init__.py
+-rw-rw-rw-   0        0        0    12838 2021-12-13 06:23:18.000000 sen2vec-1.71/sen2vec/models/tokenization.py
+drwxrwxrwx   0        0        0        0 2023-08-07 07:35:43.000000 sen2vec-1.71/sen2vec/sampled/
+-rw-rw-rw-   0        0        0      128 2021-09-22 02:21:03.000000 sen2vec-1.71/sen2vec/sampled/__init__.py
+-rw-rw-rw-   0        0        0     4070 2021-12-03 22:52:08.000000 sen2vec-1.71/sen2vec/sampled/downloader.py
+-rw-rw-rw-   0        0        0    12005 2023-08-07 06:44:37.000000 sen2vec-1.71/sen2vec/sen2vec.py
+drwxrwxrwx   0        0        0        0 2023-08-07 07:35:43.000000 sen2vec-1.71/sen2vec/util/
+-rw-rw-rw-   0        0        0      124 2021-09-22 02:21:03.000000 sen2vec-1.71/sen2vec/util/__init__.py
+-rw-rw-rw-   0        0        0     5442 2023-08-07 07:00:58.000000 sen2vec-1.71/sen2vec/util/tools.py
+-rw-rw-rw-   0        0        0     3432 2022-02-27 05:23:50.000000 sen2vec-1.71/sen2vec/util/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-07 07:35:43.000000 sen2vec-1.71/sen2vec.egg-info/
+-rw-rw-rw-   0        0        0     1763 2023-08-07 07:35:42.000000 sen2vec-1.71/sen2vec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      366 2023-08-07 07:35:43.000000 sen2vec-1.71/sen2vec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 07:35:42.000000 sen2vec-1.71/sen2vec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-08-07 07:35:43.000000 sen2vec-1.71/sen2vec.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-07 07:35:43.000000 sen2vec-1.71/setup.cfg
+-rw-rw-rw-   0        0        0     3325 2023-08-07 06:11:16.000000 sen2vec-1.71/setup.py
```

### Comparing `sen2vec-1.70/PKG-INFO` & `sen2vec-1.71/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 Metadata-Version: 2.1
 Name: sen2vec
-Version: 1.70
+Version: 1.71
 Summary: - A sen2vec MODEL that can transform sentence to vector, for Finance mainly, pytorch needed.
+Home-page: UNKNOWN
 Author: xczcx
 Author-email: 2292879219@qq.com
+License: UNKNOWN
+Description: - Sen2vec module provides convenient solution to transform sentences to vectors.
+        - The vectors transformed contain high level of information of the original sentences, 
+        - and this method has a wide range of applications in downstream tasks.
+        - The method could be directly applied to NLP tasks, 
+        - as well as other machine learning assignments, integrated with any structured data.
+        - According to application scenarios, such as the sample size of downstream tasks,
+        - the dimension of vector extracted by sen2vec varies.
+        - The vectors transformed are able to carry out the four fundamental operations of arithmetic,
+        - and could calculate the average, the intersection angle and the distance,
+        - based on different code instructions of the original information.
+        - The method sen2vec_fi is currently used to analyze financial texts,
+        - and will be developed into different versions to meet demands in diverse areas. 
+        - There are two ways to employ sen2vec:
+        - Use the default models we provide by function sen2vec_download() and sen2vec_fi
+        - Use the self-defined models: from sen2vec import sen2vec
+        - For more information: Please contact author.
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
-
-- Sen2vec module provides convenient solution to transform sentences to vectors.
-- The vectors transformed contain high level of information of the original sentences, 
-- and this method has a wide range of applications in downstream tasks.
-- The method could be directly applied to NLP tasks, 
-- as well as other machine learning assignments, integrated with any structured data.
-- According to application scenarios, such as the sample size of downstream tasks,
-- the dimension of vector extracted by sen2vec varies.
-- The vectors transformed are able to carry out the four fundamental operations of arithmetic,
-- and could calculate the average, the intersection angle and the distance,
-- based on different code instructions of the original information.
-- The method sen2vec_fi is currently used to analyze financial texts,
-- and will be developed into different versions to meet demands in diverse areas. 
-- There are two ways to employ sen2vec:
-- Use the default models we provide by function sen2vec_download() and sen2vec_fi
-- Use the self-defined models: from sen2vec import sen2vec
-- For more information: Please contact author.
```

### Comparing `sen2vec-1.70/README.md` & `sen2vec-1.71/README.md`

 * *Files identical despite different names*

### Comparing `sen2vec-1.70/sen2vec/models/tokenization.py` & `sen2vec-1.71/sen2vec/models/tokenization.py`

 * *Files identical despite different names*

### Comparing `sen2vec-1.70/sen2vec/sampled/downloader.py` & `sen2vec-1.71/sen2vec/sampled/downloader.py`

 * *Files identical despite different names*

### Comparing `sen2vec-1.70/sen2vec/sen2vec.py` & `sen2vec-1.71/sen2vec/sen2vec.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,15 @@
         CONFIG.__init__(self)
         if model_config is not None:
             self.model_config = model_config
             self.model_path = self.model_config[3] if len(model_config) == 4 else None
         self.model_name = self.model_config[0]
         self.vec_dim = self.model_config[1]
         self.num_class = self.model_config[2]
+        _, self.utils = Model_Tools.utils_load_()
 
     def sen2vec_fi(self, data, title, by_sentence=False):
         """
         Use the self-defined models:
             from sen2vec import sen2vec
             model_config = (model_name, vec_dim, num_class, model_path)  # (set your model config)
             s = sen2vec(model_config)  # (set your model config)
```

### Comparing `sen2vec-1.70/sen2vec/util/tools.py` & `sen2vec-1.71/sen2vec/util/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,20 @@
     def model_name_check_(cls, config):
         fa1 = True if 'seq' in config.model_name else False
         fa2 = True if 'ner' in config.model_name or 'simp' in config.model_name or 'qa' in config.model_name or \
                       'cls' in config.model_name or 'ori' in config.model_name or \
                       any(nd in config.model_name for nd in config.ver_list) else False
         return fa1, fa2
 
+    @classmethod
+    def utils_load_(cls, *args, **kwargs):
+        x = import_module('sen2vec.models.bert')
+        utils = x.Utils(*args, **kwargs)
+        return x, utils
+
 
 class Data_Tools(object):
     split_mark = ';;'
 
     def data_pre_process_(self, data, title):
         sen2vec_index_ = data[[title]].reset_index()['index'].to_list()
         data['sen2vec_index_'] = sen2vec_index_
```

### Comparing `sen2vec-1.70/sen2vec/util/utils.py` & `sen2vec-1.71/sen2vec/util/utils.py`

 * *Files identical despite different names*

### Comparing `sen2vec-1.70/sen2vec.egg-info/PKG-INFO` & `sen2vec-1.71/sen2vec.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 Metadata-Version: 2.1
 Name: sen2vec
-Version: 1.70
+Version: 1.71
 Summary: - A sen2vec MODEL that can transform sentence to vector, for Finance mainly, pytorch needed.
+Home-page: UNKNOWN
 Author: xczcx
 Author-email: 2292879219@qq.com
+License: UNKNOWN
+Description: - Sen2vec module provides convenient solution to transform sentences to vectors.
+        - The vectors transformed contain high level of information of the original sentences, 
+        - and this method has a wide range of applications in downstream tasks.
+        - The method could be directly applied to NLP tasks, 
+        - as well as other machine learning assignments, integrated with any structured data.
+        - According to application scenarios, such as the sample size of downstream tasks,
+        - the dimension of vector extracted by sen2vec varies.
+        - The vectors transformed are able to carry out the four fundamental operations of arithmetic,
+        - and could calculate the average, the intersection angle and the distance,
+        - based on different code instructions of the original information.
+        - The method sen2vec_fi is currently used to analyze financial texts,
+        - and will be developed into different versions to meet demands in diverse areas. 
+        - There are two ways to employ sen2vec:
+        - Use the default models we provide by function sen2vec_download() and sen2vec_fi
+        - Use the self-defined models: from sen2vec import sen2vec
+        - For more information: Please contact author.
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
-
-- Sen2vec module provides convenient solution to transform sentences to vectors.
-- The vectors transformed contain high level of information of the original sentences, 
-- and this method has a wide range of applications in downstream tasks.
-- The method could be directly applied to NLP tasks, 
-- as well as other machine learning assignments, integrated with any structured data.
-- According to application scenarios, such as the sample size of downstream tasks,
-- the dimension of vector extracted by sen2vec varies.
-- The vectors transformed are able to carry out the four fundamental operations of arithmetic,
-- and could calculate the average, the intersection angle and the distance,
-- based on different code instructions of the original information.
-- The method sen2vec_fi is currently used to analyze financial texts,
-- and will be developed into different versions to meet demands in diverse areas. 
-- There are two ways to employ sen2vec:
-- Use the default models we provide by function sen2vec_download() and sen2vec_fi
-- Use the self-defined models: from sen2vec import sen2vec
-- For more information: Please contact author.
```

### Comparing `sen2vec-1.70/setup.py` & `sen2vec-1.71/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding: utf-8
 from setuptools import setup
 import setuptools
 
 
 setup(
     name='sen2vec',
-    version='1.70',
+    version='1.71',
     description='- A sen2vec MODEL that can transform sentence to vector, for Finance mainly, pytorch needed.',
     long_description='- Sen2vec module provides convenient solution to transform sentences to vectors.\n'
                      '- The vectors transformed contain high level of information of the original sentences, \n'
                      '- and this method has a wide range of applications in downstream tasks.\n'
                      '- The method could be directly applied to NLP tasks, \n'
                      '- as well as other machine learning assignments, integrated with any structured data.\n'
                      '- According to application scenarios, such as the sample size of downstream tasks,\n'
```

