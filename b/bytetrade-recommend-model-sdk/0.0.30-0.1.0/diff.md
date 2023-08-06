# Comparing `tmp/bytetrade-recommend-model-sdk-0.0.30.tar.gz` & `tmp/bytetrade-recommend-model-sdk-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bytetrade-recommend-model-sdk-0.0.30.tar", last modified: Thu Jul 27 07:08:53 2023, max compression
+gzip compressed data, was "bytetrade-recommend-model-sdk-0.1.0.tar", last modified: Sun Aug  6 22:14:59 2023, max compression
```

## Comparing `bytetrade-recommend-model-sdk-0.0.30.tar` & `bytetrade-recommend-model-sdk-0.1.0.tar`

### file list

```diff
@@ -1,61 +1,63 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-27 07:08:53.543876 bytetrade-recommend-model-sdk-0.0.30/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       59 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.30/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       74 2023-07-27 07:08:53.543876 bytetrade-recommend-model-sdk-0.0.30/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1904 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.30/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-27 07:08:53.539876 bytetrade-recommend-model-sdk-0.0.30/bytetrade_recommend_model_sdk.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       74 2023-07-27 07:08:53.000000 bytetrade-recommend-model-sdk-0.0.30/bytetrade_recommend_model_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2178 2023-07-27 07:08:53.000000 bytetrade-recommend-model-sdk-0.0.30/bytetrade_recommend_model_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-27 07:08:53.000000 bytetrade-recommend-model-sdk-0.0.30/bytetrade_recommend_model_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      155 2023-07-27 07:08:53.000000 bytetrade-recommend-model-sdk-0.0.30/bytetrade_recommend_model_sdk.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       20 2023-07-27 07:08:53.000000 bytetrade-recommend-model-sdk-0.0.30/bytetrade_recommend_model_sdk.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-27 07:08:53.539876 bytetrade-recommend-model-sdk-0.0.30/recommend_model_sdk/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.30/recommend_model_sdk/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-27 07:08:53.539876 bytetrade-recommend-model-sdk-0.0.30/recommend_model_sdk/embeddings/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.30/recommend_model_sdk/embeddings/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3875 2023-07-16 23:12:22.000000 bytetrade-recommend-model-sdk-0.0.30/recommend_model_sdk/embeddings/bert_embedding.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      872 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.30/recommend_model_sdk/embeddings/embedding_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5430 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.30/recommend_model_sdk/embeddings/word2vec_embedding.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-27 07:08:53.539876 bytetrade-recommend-model-sdk-0.0.30/recommend_model_sdk/mind_sdk/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.30/recommend_model_sdk/mind_sdk/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-27 07:08:53.539876 bytetrade-recommend-model-sdk-0.0.30/recommend_model_sdk/mind_sdk/config/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.30/recommend_model_sdk/mind_sdk/config/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      675 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.30/recommend_model_sdk/mind_sdk/config/content_similar_config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      396 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.30/recommend_model_sdk/mind_sdk/config/dnn_click_predictor_config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      201 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.30/recommend_model_sdk/mind_sdk/config/mind_base_config.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-27 07:08:53.543876 bytetrade-recommend-model-sdk-0.0.30/recommend_model_sdk/mind_sdk/dataset/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.30/recommend_model_sdk/mind_sdk/dataset/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4244 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.30/recommend_model_sdk/mind_sdk/dataset/mind_base_dataset.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1769 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.30/recommend_model_sdk/mind_sdk/dataset/mind_behaviours_dataset.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2719 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.30/recommend_model_sdk/mind_sdk/dataset/mind_behaviours_parsed_dataset.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2180 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.30/recommend_model_sdk/mind_sdk/dataset/mind_news_dataset.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2873 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.30/recommend_model_sdk/mind_sdk/dataset/mind_user_dataset.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-27 07:08:53.543876 bytetrade-recommend-model-sdk-0.0.30/recommend_model_sdk/mind_sdk/eval/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.30/recommend_model_sdk/mind_sdk/eval/__init_.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1113 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.30/recommend_model_sdk/mind_sdk/eval/eval_operation.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11667 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.30/recommend_model_sdk/mind_sdk/eval/mind_eval_tool.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-27 07:08:53.543876 bytetrade-recommend-model-sdk-0.0.30/recommend_model_sdk/mind_sdk/exp/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.30/recommend_model_sdk/mind_sdk/exp/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11826 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.30/recommend_model_sdk/mind_sdk/exp/mind_dnn_click_predictor_train_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       96 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.30/recommend_model_sdk/mind_sdk/experiment_enum.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-27 07:08:53.543876 bytetrade-recommend-model-sdk-0.0.30/recommend_model_sdk/mind_sdk/model/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.30/recommend_model_sdk/mind_sdk/model/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14888 2023-07-16 23:12:22.000000 bytetrade-recommend-model-sdk-0.0.30/recommend_model_sdk/mind_sdk/model/content_similar_model.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2330 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.30/recommend_model_sdk/mind_sdk/model/dnn_click_predictor.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-27 07:08:53.543876 bytetrade-recommend-model-sdk-0.0.30/recommend_model_sdk/proto_class/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.30/recommend_model_sdk/proto_class/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    24560 2023-07-27 04:06:42.000000 bytetrade-recommend-model-sdk-0.0.30/recommend_model_sdk/proto_class/embedding_pb2.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-27 07:08:53.543876 bytetrade-recommend-model-sdk-0.0.30/recommend_model_sdk/recommend/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.30/recommend_model_sdk/recommend/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4976 2023-07-16 23:12:22.000000 bytetrade-recommend-model-sdk-0.0.30/recommend_model_sdk/recommend/recommend_common_util.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1774 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.30/recommend_model_sdk/recommend/recommend_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2150 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.30/recommend_model_sdk/recommend/time_weight_decay_tool.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-27 07:08:53.543876 bytetrade-recommend-model-sdk-0.0.30/recommend_model_sdk/resources/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.30/recommend_model_sdk/resources/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2508 2023-07-16 23:12:22.000000 bytetrade-recommend-model-sdk-0.0.30/recommend_model_sdk/resources/model_management.json
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-27 07:08:53.543876 bytetrade-recommend-model-sdk-0.0.30/recommend_model_sdk/tools/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.30/recommend_model_sdk/tools/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5148 2023-07-21 12:55:09.000000 bytetrade-recommend-model-sdk-0.0.30/recommend_model_sdk/tools/aws_s3_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10416 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.30/recommend_model_sdk/tools/common_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    38787 2023-07-27 06:58:55.000000 bytetrade-recommend-model-sdk-0.0.30/recommend_model_sdk/tools/model_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-27 07:08:53.543876 bytetrade-recommend-model-sdk-0.0.30/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1125 2023-07-27 07:05:19.000000 bytetrade-recommend-model-sdk-0.0.30/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-06 22:14:59.573473 bytetrade-recommend-model-sdk-0.1.0/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       59 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.1.0/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       73 2023-08-06 22:14:59.573473 bytetrade-recommend-model-sdk-0.1.0/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1904 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.1.0/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-06 22:14:59.569473 bytetrade-recommend-model-sdk-0.1.0/bytetrade_recommend_model_sdk.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       73 2023-08-06 22:14:59.000000 bytetrade-recommend-model-sdk-0.1.0/bytetrade_recommend_model_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2266 2023-08-06 22:14:59.000000 bytetrade-recommend-model-sdk-0.1.0/bytetrade_recommend_model_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-08-06 22:14:59.000000 bytetrade-recommend-model-sdk-0.1.0/bytetrade_recommend_model_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      155 2023-08-06 22:14:59.000000 bytetrade-recommend-model-sdk-0.1.0/bytetrade_recommend_model_sdk.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       20 2023-08-06 22:14:59.000000 bytetrade-recommend-model-sdk-0.1.0/bytetrade_recommend_model_sdk.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-06 22:14:59.569473 bytetrade-recommend-model-sdk-0.1.0/recommend_model_sdk/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.1.0/recommend_model_sdk/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-06 22:14:59.569473 bytetrade-recommend-model-sdk-0.1.0/recommend_model_sdk/embeddings/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.1.0/recommend_model_sdk/embeddings/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3875 2023-07-16 23:12:22.000000 bytetrade-recommend-model-sdk-0.1.0/recommend_model_sdk/embeddings/bert_embedding.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      872 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.1.0/recommend_model_sdk/embeddings/embedding_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5430 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.1.0/recommend_model_sdk/embeddings/word2vec_embedding.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-06 22:14:59.569473 bytetrade-recommend-model-sdk-0.1.0/recommend_model_sdk/mind_sdk/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.1.0/recommend_model_sdk/mind_sdk/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-06 22:14:59.569473 bytetrade-recommend-model-sdk-0.1.0/recommend_model_sdk/mind_sdk/config/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.1.0/recommend_model_sdk/mind_sdk/config/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      675 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.1.0/recommend_model_sdk/mind_sdk/config/content_similar_config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      396 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.1.0/recommend_model_sdk/mind_sdk/config/dnn_click_predictor_config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      201 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.1.0/recommend_model_sdk/mind_sdk/config/mind_base_config.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-06 22:14:59.569473 bytetrade-recommend-model-sdk-0.1.0/recommend_model_sdk/mind_sdk/dataset/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.1.0/recommend_model_sdk/mind_sdk/dataset/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4244 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.1.0/recommend_model_sdk/mind_sdk/dataset/mind_base_dataset.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1769 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.1.0/recommend_model_sdk/mind_sdk/dataset/mind_behaviours_dataset.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2719 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.1.0/recommend_model_sdk/mind_sdk/dataset/mind_behaviours_parsed_dataset.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2180 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.1.0/recommend_model_sdk/mind_sdk/dataset/mind_news_dataset.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2873 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.1.0/recommend_model_sdk/mind_sdk/dataset/mind_user_dataset.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-06 22:14:59.569473 bytetrade-recommend-model-sdk-0.1.0/recommend_model_sdk/mind_sdk/eval/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.1.0/recommend_model_sdk/mind_sdk/eval/__init_.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1113 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.1.0/recommend_model_sdk/mind_sdk/eval/eval_operation.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11667 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.1.0/recommend_model_sdk/mind_sdk/eval/mind_eval_tool.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-06 22:14:59.573473 bytetrade-recommend-model-sdk-0.1.0/recommend_model_sdk/mind_sdk/exp/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.1.0/recommend_model_sdk/mind_sdk/exp/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11826 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.1.0/recommend_model_sdk/mind_sdk/exp/mind_dnn_click_predictor_train_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       96 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.1.0/recommend_model_sdk/mind_sdk/experiment_enum.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-06 22:14:59.573473 bytetrade-recommend-model-sdk-0.1.0/recommend_model_sdk/mind_sdk/model/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.1.0/recommend_model_sdk/mind_sdk/model/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18601 2023-08-05 01:34:07.000000 bytetrade-recommend-model-sdk-0.1.0/recommend_model_sdk/mind_sdk/model/content_similar_model.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2330 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.1.0/recommend_model_sdk/mind_sdk/model/dnn_click_predictor.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-06 22:14:59.573473 bytetrade-recommend-model-sdk-0.1.0/recommend_model_sdk/proto_class/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.1.0/recommend_model_sdk/proto_class/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    28146 2023-07-28 12:51:55.000000 bytetrade-recommend-model-sdk-0.1.0/recommend_model_sdk/proto_class/embedding_pb2.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-06 22:14:59.573473 bytetrade-recommend-model-sdk-0.1.0/recommend_model_sdk/recommend/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.1.0/recommend_model_sdk/recommend/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2414 2023-08-03 02:44:16.000000 bytetrade-recommend-model-sdk-0.1.0/recommend_model_sdk/recommend/common_enum.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4976 2023-07-16 23:12:22.000000 bytetrade-recommend-model-sdk-0.1.0/recommend_model_sdk/recommend/recommend_common_util.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3900 2023-08-03 04:23:43.000000 bytetrade-recommend-model-sdk-0.1.0/recommend_model_sdk/recommend/recommend_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2150 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.1.0/recommend_model_sdk/recommend/time_weight_decay_tool.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-06 22:14:59.573473 bytetrade-recommend-model-sdk-0.1.0/recommend_model_sdk/resources/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.1.0/recommend_model_sdk/resources/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2508 2023-07-16 23:12:22.000000 bytetrade-recommend-model-sdk-0.1.0/recommend_model_sdk/resources/model_management.json
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-06 22:14:59.573473 bytetrade-recommend-model-sdk-0.1.0/recommend_model_sdk/tools/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.1.0/recommend_model_sdk/tools/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5148 2023-07-21 12:55:09.000000 bytetrade-recommend-model-sdk-0.1.0/recommend_model_sdk/tools/aws_s3_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11485 2023-08-05 01:20:48.000000 bytetrade-recommend-model-sdk-0.1.0/recommend_model_sdk/tools/common_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    42654 2023-08-02 00:11:49.000000 bytetrade-recommend-model-sdk-0.1.0/recommend_model_sdk/tools/model_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    30727 2023-08-05 01:09:46.000000 bytetrade-recommend-model-sdk-0.1.0/recommend_model_sdk/tools/weaviate_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-08-06 22:14:59.573473 bytetrade-recommend-model-sdk-0.1.0/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1124 2023-08-06 22:13:07.000000 bytetrade-recommend-model-sdk-0.1.0/setup.py
```

### Comparing `bytetrade-recommend-model-sdk-0.0.30/README.md` & `bytetrade-recommend-model-sdk-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.30/bytetrade_recommend_model_sdk.egg-info/SOURCES.txt` & `bytetrade-recommend-model-sdk-0.1.0/bytetrade_recommend_model_sdk.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -30,16 +30,18 @@
 recommend_model_sdk/mind_sdk/exp/mind_dnn_click_predictor_train_tool.py
 recommend_model_sdk/mind_sdk/model/__init__.py
 recommend_model_sdk/mind_sdk/model/content_similar_model.py
 recommend_model_sdk/mind_sdk/model/dnn_click_predictor.py
 recommend_model_sdk/proto_class/__init__.py
 recommend_model_sdk/proto_class/embedding_pb2.py
 recommend_model_sdk/recommend/__init__.py
+recommend_model_sdk/recommend/common_enum.py
 recommend_model_sdk/recommend/recommend_common_util.py
 recommend_model_sdk/recommend/recommend_tool.py
 recommend_model_sdk/recommend/time_weight_decay_tool.py
 recommend_model_sdk/resources/__init__.py
 recommend_model_sdk/resources/model_management.json
 recommend_model_sdk/tools/__init__.py
 recommend_model_sdk/tools/aws_s3_tool.py
 recommend_model_sdk/tools/common_tool.py
-recommend_model_sdk/tools/model_tool.py
+recommend_model_sdk/tools/model_tool.py
+recommend_model_sdk/tools/weaviate_tool.py
```

### Comparing `bytetrade-recommend-model-sdk-0.0.30/recommend_model_sdk/embeddings/bert_embedding.py` & `bytetrade-recommend-model-sdk-0.1.0/recommend_model_sdk/embeddings/bert_embedding.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.30/recommend_model_sdk/embeddings/embedding_tool.py` & `bytetrade-recommend-model-sdk-0.1.0/recommend_model_sdk/embeddings/embedding_tool.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.30/recommend_model_sdk/embeddings/word2vec_embedding.py` & `bytetrade-recommend-model-sdk-0.1.0/recommend_model_sdk/embeddings/word2vec_embedding.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.30/recommend_model_sdk/mind_sdk/config/content_similar_config.py` & `bytetrade-recommend-model-sdk-0.1.0/recommend_model_sdk/mind_sdk/config/content_similar_config.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.30/recommend_model_sdk/mind_sdk/dataset/mind_base_dataset.py` & `bytetrade-recommend-model-sdk-0.1.0/recommend_model_sdk/mind_sdk/dataset/mind_base_dataset.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.30/recommend_model_sdk/mind_sdk/dataset/mind_behaviours_dataset.py` & `bytetrade-recommend-model-sdk-0.1.0/recommend_model_sdk/mind_sdk/dataset/mind_behaviours_dataset.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.30/recommend_model_sdk/mind_sdk/dataset/mind_behaviours_parsed_dataset.py` & `bytetrade-recommend-model-sdk-0.1.0/recommend_model_sdk/mind_sdk/dataset/mind_behaviours_parsed_dataset.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.30/recommend_model_sdk/mind_sdk/dataset/mind_news_dataset.py` & `bytetrade-recommend-model-sdk-0.1.0/recommend_model_sdk/mind_sdk/dataset/mind_news_dataset.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.30/recommend_model_sdk/mind_sdk/dataset/mind_user_dataset.py` & `bytetrade-recommend-model-sdk-0.1.0/recommend_model_sdk/mind_sdk/dataset/mind_user_dataset.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.30/recommend_model_sdk/mind_sdk/eval/eval_operation.py` & `bytetrade-recommend-model-sdk-0.1.0/recommend_model_sdk/mind_sdk/eval/eval_operation.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.30/recommend_model_sdk/mind_sdk/eval/mind_eval_tool.py` & `bytetrade-recommend-model-sdk-0.1.0/recommend_model_sdk/mind_sdk/eval/mind_eval_tool.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.30/recommend_model_sdk/mind_sdk/exp/mind_dnn_click_predictor_train_tool.py` & `bytetrade-recommend-model-sdk-0.1.0/recommend_model_sdk/mind_sdk/exp/mind_dnn_click_predictor_train_tool.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.30/recommend_model_sdk/mind_sdk/model/content_similar_model.py` & `bytetrade-recommend-model-sdk-0.1.0/recommend_model_sdk/mind_sdk/model/content_similar_model.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-from common_util.common_tool import CommonTool
+from recommend_model_sdk.tools.common_tool import CommonTool
 from recommend_model_sdk.mind_sdk.config.content_similar_config import ContentSimilarConfig
 from recommend_model_sdk.tools.aws_s3_tool import AWSS3Tool
 from recommend_model_sdk.recommend.recommend_common_util import RecommendCommonUtil
+from recommend_model_sdk.tools.weaviate_tool import WeaviateTool
 
 
 from datetime import datetime
 import faiss
 
 import numpy as np
 import torch
@@ -291,8 +292,66 @@
               result_tuple_list.append((self.__base_index_to_document_id[current_index],current_weight))
         
         if len(result_tuple_list)  < 1:
             self.__logger.debug('after complete result_tuple_list is small than 1')
             return self.recall_empty(limit)
         return result_tuple_list
               
-              
+    
+
+class WeaviateContentSimilarModelRecall:
+    def __init__(self,config) -> None:
+        
+        self.__recommend_common_util = RecommendCommonUtil()
+        self.__common_tool = CommonTool()
+        self.__logger = self.__common_tool.get_logger()
+        if isinstance(config, ContentSimilarConfig) is False:
+            raise ValueError("ContentSimilarModel is not model")
+        self.__config = config
+        recommend_environment =self.__common_tool.get_default_environment_variable()
+        if recommend_environment["weaviate_cloud"]:
+            self.__weaviate_tool = WeaviateTool(model_root_dir=recommend_environment['model_path'],
+                                                cloud=recommend_environment["weaviate_cloud"], 
+                                                cloud_url=recommend_environment['cloud_weaviate_url'],
+                                                cloud_api_key=recommend_environment['cloud_weaviate_api_key'],
+                                                )
+            self.__logger.debug("weaviate is cloud")
+        else:
+            self.__weaviate_tool = WeaviateTool(model_root_dir=recommend_environment['model_path'],
+                                    cloud=recommend_environment["weaviate_cloud"], 
+                                    private_ip=recommend_environment['private_weaviate_ip'],
+                                    private_port=int(recommend_environment['private_weaviate_port']),
+                                    )
+            self.__logger.debug("weaviate is private")
+        
+        
+        
+    def get_user_vector(self,candidate_news_id_to_embedding):
+        current_list_embedding = list()
+        for current_id, current_embedding_info in candidate_news_id_to_embedding.items():
+            current_list_embedding.append(current_embedding_info['embedding'])
+        if len(current_list_embedding) > self.__config.num_clicked_news_a_user:
+            current_list_embedding = current_list_embedding[:self.__config.num_clicked_news_a_user]
+        stack_candidate_embedding = np.stack(current_list_embedding)
+        
+        user_embedding = stack_candidate_embedding.sum(axis=0,keepdims=True)
+        return user_embedding
+    
+    def recall(self,candidate_news_id_to_embedding,limit,
+               package_range_list=None,start_time=None,end_time=None,
+               major_language=None,category_list=None):
+        """
+        """
+        if len(candidate_news_id_to_embedding) < 1:
+            raise ValueError("candidate_news_id_to_embedding length samll than 1")
+
+        # self.__recommend_common_util.validate_candidate_document_id_to_item(candidate_news_id_to_embedding,self.__embedding_shape)
+        user_embedding = self.get_user_vector(candidate_news_id_to_embedding)
+        article_list = self.__weaviate_tool.search_nearest(self.__config.embedding_model_name,self.__config.embedding_model_version,limit,
+                                                           embedding=user_embedding.tolist()[0],package_range_list=package_range_list
+                                                           ,start_time=start_time,end_time=end_time,
+                                                           major_language=major_language,category_list=category_list)
+        article_list.sort(key=lambda item:item['certainty'] , reverse=True) # here reverse is  true or false, is not important, because search nearest have got right result
+        url_and_weight_tuple = list()
+        for current_article in article_list:
+            url_and_weight_tuple.append((current_article['url'],current_article['certainty']))
+        return url_and_weight_tuple
```

### Comparing `bytetrade-recommend-model-sdk-0.0.30/recommend_model_sdk/mind_sdk/model/dnn_click_predictor.py` & `bytetrade-recommend-model-sdk-0.1.0/recommend_model_sdk/mind_sdk/model/dnn_click_predictor.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.30/recommend_model_sdk/proto_class/embedding_pb2.py` & `bytetrade-recommend-model-sdk-0.1.0/recommend_model_sdk/proto_class/embedding_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='embedding.proto',
   package='',
   syntax='proto3',
   serialized_options=None,
-  serialized_pb=_b('\n\x0f\x65mbedding.proto\"\xf5\x01\n\x07\x41rticle\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x11\n\tfull_text\x18\x02 \x01(\t\x12\x12\n\ncreated_at\x18\x03 \x01(\x12\x12\x14\n\x0cpublished_at\x18\x04 \x01(\x12\x12\r\n\x05title\x18\x05 \x01(\t\x12\x0e\n\x06\x61uthor\x18\x06 \x01(\t\x12\x0f\n\x07\x63ontent\x18\x07 \x01(\t\x12\x0f\n\x07\x66\x65\x65\x64_id\x18\x08 \x01(\x04\x12\x0c\n\x04hash\x18\t \x01(\t\x12\x11\n\timage_url\x18\n \x01(\t\x12\x14\n\x0ckeyword_list\x18\x0b \x03(\t\x12\x10\n\x08\x63loud_id\x18\x0c \x01(\x04\x12\x16\n\x0emajor_language\x18\r \x01(\t\"\x83\x01\n\tEmbedding\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x12\n\nmodel_name\x18\x02 \x01(\t\x12\x15\n\rmodel_version\x18\x03 \x01(\t\x12\x12\n\nembeddings\x18\x04 \x03(\x02\x12*\n\x10subdocembeddings\x18\x05 \x03(\x0b\x32\x10.SubdocEmbedding\";\n\x0fSubdocEmbedding\x12\x14\n\x0csubdoc_index\x18\x01 \x01(\r\x12\x12\n\nembeddings\x18\x02 \x03(\x02\"K\n\rLatestPackage\x12\x1a\n\x08\x61rticles\x18\x01 \x03(\x0b\x32\x08.Article\x12\x1e\n\nembeddings\x18\x02 \x03(\x0b\x32\n.Embedding\",\n\x0e\x41rticlePackage\x12\x1a\n\x08\x61rticles\x18\x01 \x03(\x0b\x32\x08.Article\"2\n\x10\x45mbeddingPakcage\x12\x1e\n\nembeddings\x18\x01 \x03(\x0b\x32\n.Embedding\"\xc1\x01\n\x04\x46\x65\x65\x64\x12\n\n\x02id\x18\x01 \x01(\x03\x12\x10\n\x08\x66\x65\x65\x64_url\x18\x02 \x01(\t\x12\x10\n\x08site_url\x18\x03 \x01(\t\x12\r\n\x05title\x18\x04 \x01(\t\x12\x13\n\x0b\x63\x61tegory_id\x18\x05 \x01(\x03\x12\x16\n\x0e\x63\x61tegory_title\x18\x06 \x01(\t\x12\x0f\n\x07icon_id\x18\x07 \x01(\x03\x12\x11\n\ticon_type\x18\x08 \x01(\t\x12\x14\n\x0cicon_content\x18\t \x01(\x0c\x12\x13\n\x0b\x64\x65scription\x18\n \x01(\t\"#\n\x0b\x46\x65\x65\x64Package\x12\x14\n\x05\x66\x65\x65\x64s\x18\x01 \x03(\x0b\x32\x05.Feed\"A\n\x11KeywordSortedInfo\x12\x0c\n\x04urls\x18\x01 \x03(\t\x12\r\n\x05\x66\x65\x65\x64s\x18\x02 \x03(\x03\x12\x0f\n\x07keyword\x18\x03 \x01(\t\"M\n\x18KeywordSortedInfoPackage\x12\x31\n\x15keyword_sortinfo_list\x18\x01 \x03(\x0b\x32\x12.KeywordSortedInfob\x06proto3')
+  serialized_pb=_b('\n\x0f\x65mbedding.proto\"\xf5\x01\n\x07\x41rticle\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x11\n\tfull_text\x18\x02 \x01(\t\x12\x12\n\ncreated_at\x18\x03 \x01(\x12\x12\x14\n\x0cpublished_at\x18\x04 \x01(\x12\x12\r\n\x05title\x18\x05 \x01(\t\x12\x0e\n\x06\x61uthor\x18\x06 \x01(\t\x12\x0f\n\x07\x63ontent\x18\x07 \x01(\t\x12\x0f\n\x07\x66\x65\x65\x64_id\x18\x08 \x01(\x04\x12\x0c\n\x04hash\x18\t \x01(\t\x12\x11\n\timage_url\x18\n \x01(\t\x12\x14\n\x0ckeyword_list\x18\x0b \x03(\t\x12\x10\n\x08\x63loud_id\x18\x0c \x01(\x04\x12\x16\n\x0emajor_language\x18\r \x01(\t\"\x83\x01\n\tEmbedding\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x12\n\nmodel_name\x18\x02 \x01(\t\x12\x15\n\rmodel_version\x18\x03 \x01(\t\x12\x12\n\nembeddings\x18\x04 \x03(\x02\x12*\n\x10subdocembeddings\x18\x05 \x03(\x0b\x32\x10.SubdocEmbedding\";\n\x0fSubdocEmbedding\x12\x14\n\x0csubdoc_index\x18\x01 \x01(\r\x12\x12\n\nembeddings\x18\x02 \x03(\x02\"K\n\rLatestPackage\x12\x1a\n\x08\x61rticles\x18\x01 \x03(\x0b\x32\x08.Article\x12\x1e\n\nembeddings\x18\x02 \x03(\x0b\x32\n.Embedding\",\n\x0e\x41rticlePackage\x12\x1a\n\x08\x61rticles\x18\x01 \x03(\x0b\x32\x08.Article\"2\n\x10\x45mbeddingPakcage\x12\x1e\n\nembeddings\x18\x01 \x03(\x0b\x32\n.Embedding\"\xc1\x01\n\x04\x46\x65\x65\x64\x12\n\n\x02id\x18\x01 \x01(\x03\x12\x10\n\x08\x66\x65\x65\x64_url\x18\x02 \x01(\t\x12\x10\n\x08site_url\x18\x03 \x01(\t\x12\r\n\x05title\x18\x04 \x01(\t\x12\x13\n\x0b\x63\x61tegory_id\x18\x05 \x01(\x03\x12\x16\n\x0e\x63\x61tegory_title\x18\x06 \x01(\t\x12\x0f\n\x07icon_id\x18\x07 \x01(\x03\x12\x11\n\ticon_type\x18\x08 \x01(\t\x12\x14\n\x0cicon_content\x18\t \x01(\x0c\x12\x13\n\x0b\x64\x65scription\x18\n \x01(\t\"#\n\x0b\x46\x65\x65\x64Package\x12\x14\n\x05\x66\x65\x65\x64s\x18\x01 \x03(\x0b\x32\x05.Feed\"A\n\x11KeywordSortedInfo\x12\x0c\n\x04urls\x18\x01 \x03(\t\x12\r\n\x05\x66\x65\x65\x64s\x18\x02 \x03(\x03\x12\x0f\n\x07keyword\x18\x03 \x01(\t\"M\n\x18KeywordSortedInfoPackage\x12\x31\n\x15keyword_sortinfo_list\x18\x01 \x03(\x0b\x32\x12.KeywordSortedInfo\"U\n\x08\x43\x61tegory\x12\x10\n\x08\x63\x61tegory\x18\x01 \x01(\t\x12\r\n\x05level\x18\x02 \x01(\t\x12\x18\n\x10subcategory_list\x18\x03 \x03(\t\x12\x0e\n\x06parent\x18\x04 \x01(\t\"3\n\x0f\x43\x61tegoryPackage\x12 \n\rcategory_list\x18\x01 \x03(\x0b\x32\t.Categoryb\x06proto3')
 )
 
 
 
 
 _ARTICLE = _descriptor.Descriptor(
   name='Article',
@@ -533,31 +533,117 @@
   extension_ranges=[],
   oneofs=[
   ],
   serialized_start=937,
   serialized_end=1014,
 )
 
+
+_CATEGORY = _descriptor.Descriptor(
+  name='Category',
+  full_name='Category',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='category', full_name='Category.category', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=_b("").decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='level', full_name='Category.level', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=_b("").decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='subcategory_list', full_name='Category.subcategory_list', index=2,
+      number=3, type=9, cpp_type=9, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='parent', full_name='Category.parent', index=3,
+      number=4, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=_b("").decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=1016,
+  serialized_end=1101,
+)
+
+
+_CATEGORYPACKAGE = _descriptor.Descriptor(
+  name='CategoryPackage',
+  full_name='CategoryPackage',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='category_list', full_name='CategoryPackage.category_list', index=0,
+      number=1, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=1103,
+  serialized_end=1154,
+)
+
 _EMBEDDING.fields_by_name['subdocembeddings'].message_type = _SUBDOCEMBEDDING
 _LATESTPACKAGE.fields_by_name['articles'].message_type = _ARTICLE
 _LATESTPACKAGE.fields_by_name['embeddings'].message_type = _EMBEDDING
 _ARTICLEPACKAGE.fields_by_name['articles'].message_type = _ARTICLE
 _EMBEDDINGPAKCAGE.fields_by_name['embeddings'].message_type = _EMBEDDING
 _FEEDPACKAGE.fields_by_name['feeds'].message_type = _FEED
 _KEYWORDSORTEDINFOPACKAGE.fields_by_name['keyword_sortinfo_list'].message_type = _KEYWORDSORTEDINFO
+_CATEGORYPACKAGE.fields_by_name['category_list'].message_type = _CATEGORY
 DESCRIPTOR.message_types_by_name['Article'] = _ARTICLE
 DESCRIPTOR.message_types_by_name['Embedding'] = _EMBEDDING
 DESCRIPTOR.message_types_by_name['SubdocEmbedding'] = _SUBDOCEMBEDDING
 DESCRIPTOR.message_types_by_name['LatestPackage'] = _LATESTPACKAGE
 DESCRIPTOR.message_types_by_name['ArticlePackage'] = _ARTICLEPACKAGE
 DESCRIPTOR.message_types_by_name['EmbeddingPakcage'] = _EMBEDDINGPAKCAGE
 DESCRIPTOR.message_types_by_name['Feed'] = _FEED
 DESCRIPTOR.message_types_by_name['FeedPackage'] = _FEEDPACKAGE
 DESCRIPTOR.message_types_by_name['KeywordSortedInfo'] = _KEYWORDSORTEDINFO
 DESCRIPTOR.message_types_by_name['KeywordSortedInfoPackage'] = _KEYWORDSORTEDINFOPACKAGE
+DESCRIPTOR.message_types_by_name['Category'] = _CATEGORY
+DESCRIPTOR.message_types_by_name['CategoryPackage'] = _CATEGORYPACKAGE
 _sym_db.RegisterFileDescriptor(DESCRIPTOR)
 
 Article = _reflection.GeneratedProtocolMessageType('Article', (_message.Message,), dict(
   DESCRIPTOR = _ARTICLE,
   __module__ = 'embedding_pb2'
   # @@protoc_insertion_point(class_scope:Article)
   ))
@@ -622,9 +708,23 @@
 KeywordSortedInfoPackage = _reflection.GeneratedProtocolMessageType('KeywordSortedInfoPackage', (_message.Message,), dict(
   DESCRIPTOR = _KEYWORDSORTEDINFOPACKAGE,
   __module__ = 'embedding_pb2'
   # @@protoc_insertion_point(class_scope:KeywordSortedInfoPackage)
   ))
 _sym_db.RegisterMessage(KeywordSortedInfoPackage)
 
+Category = _reflection.GeneratedProtocolMessageType('Category', (_message.Message,), dict(
+  DESCRIPTOR = _CATEGORY,
+  __module__ = 'embedding_pb2'
+  # @@protoc_insertion_point(class_scope:Category)
+  ))
+_sym_db.RegisterMessage(Category)
+
+CategoryPackage = _reflection.GeneratedProtocolMessageType('CategoryPackage', (_message.Message,), dict(
+  DESCRIPTOR = _CATEGORYPACKAGE,
+  __module__ = 'embedding_pb2'
+  # @@protoc_insertion_point(class_scope:CategoryPackage)
+  ))
+_sym_db.RegisterMessage(CategoryPackage)
+
 
 # @@protoc_insertion_point(module_scope)
```

### Comparing `bytetrade-recommend-model-sdk-0.0.30/recommend_model_sdk/recommend/recommend_common_util.py` & `bytetrade-recommend-model-sdk-0.1.0/recommend_model_sdk/recommend/recommend_common_util.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.30/recommend_model_sdk/recommend/time_weight_decay_tool.py` & `bytetrade-recommend-model-sdk-0.1.0/recommend_model_sdk/recommend/time_weight_decay_tool.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.30/recommend_model_sdk/resources/model_management.json` & `bytetrade-recommend-model-sdk-0.1.0/recommend_model_sdk/resources/model_management.json`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.30/recommend_model_sdk/tools/aws_s3_tool.py` & `bytetrade-recommend-model-sdk-0.1.0/recommend_model_sdk/tools/aws_s3_tool.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.30/recommend_model_sdk/tools/common_tool.py` & `bytetrade-recommend-model-sdk-0.1.0/recommend_model_sdk/tools/common_tool.py`

 * *Files 18% similar despite different names*

```diff
@@ -218,8 +218,23 @@
         list_str = list(set_str)
         list_str.sort()
         
         concat_str = ''
         for current_str in list_str:
             concat_str = concat_str + current_str
         digest = hashlib.md5(concat_str.encode()).hexdigest()
-        return digest
+        return digest
+    
+    def get_default_environment_variable(self):
+        default_environment = dict()
+        default_environment["model_path"] =  os.environ.get('model_path', "/ssd/code/MODEL_CLIENT")
+        default_environment["weaviate_cloud"] = os.environ.get("weaviate_cloud",False)
+        default_cloud_weaviate_url = 'https://test-recommend-9b6u510q.weaviate.network'
+        default_cloud_weaviate_api_key = 'mxG7eRQWdu1ruLaCixZUdoLaTrkAsuiifTLw'
+        default_environment["cloud_weaviate_url"] = os.environ.get('cloud_weaviate_url',default_cloud_weaviate_url)
+        default_environment["cloud_weaviate_api_key"] = os.environ.get('cloud_weaviate_api_key',default_cloud_weaviate_api_key)
+        default_private_weaviate_ip = "127.0.0.1"
+        default_private_weaviate_port = 9000
+        default_environment["private_weaviate_ip"] = os.environ.get("private_weaviate_ip",default_private_weaviate_ip)
+        default_environment["private_weaviate_port"] = os.environ.get("private_weaviate_port",default_private_weaviate_port)
+        return default_environment
+
```

### Comparing `bytetrade-recommend-model-sdk-0.0.30/recommend_model_sdk/tools/model_tool.py` & `bytetrade-recommend-model-sdk-0.1.0/recommend_model_sdk/tools/model_tool.py`

 * *Files 3% similar despite different names*

```diff
@@ -516,15 +516,33 @@
             elif model_related_files_suffix[original_current_file_name] == "direct":
                 response = self.__awss3tool.download(last_formt_dst_file,s3_bucket_name,file_name_key)
                 self.__logger.debug(f'download bucket {s3_bucket_name} file_name_key {file_name_key} response {response}')
             if os.path.exists(last_formt_dst_file) is False:
                 return False
         return True
                 
-                
+    def download_list_increment_package(self,model_name,model_version,list_package):
+        if isinstance(list_package,list) is False:
+            raise ValueError("list_package is not list")
+        for current_package in list_package:
+            if isinstance(current_package,str) is False:
+                raise ValueError("current_package is not str")
+        self.valid_model_name_and_version(model_name,model_version)
+        
+        merge_url_to_article_dict = dict()
+        merge_url_to_embedding_dict = dict()
+        for current_package in list_package:
+            url_to_article_dict,url_to_embedding_dict = self.download_increment_package(model_name,model_version,current_package)
+            merge_url_to_article_dict.update(url_to_article_dict)
+            merge_url_to_embedding_dict.update(url_to_embedding_dict)
+            
+        return merge_url_to_article_dict,merge_url_to_embedding_dict
+        
+        
+        
     def download_increment_package(self,model_name,model_version,package_key,publish_time=None):
         """_summary_
         download increment embedding package
         Args:
             model_name (_type_): _description_
             model_version (_type_): _description_
             latest_number (_type_): _description_
@@ -730,8 +748,63 @@
         language_type = None
         try:
             language_type = detect(text)
         except Exception as ex:
             self.__logger.debug(f'language_type ex: {str(ex)}')
         return language_type
         
-        
+
+    def download_latest_all_category(self):
+        '''
+        {
+            "category_name":{
+                "category":"",
+                "level":"first",
+                "subcategory_list":[] first level have
+                "parent":"" second level have
+            }
+        }
+        '''
+        latest_package_key = 'all_category'
+        common_dir = os.path.join(self.__model_root_dir,'common')
+        if os.path.exists(common_dir) is False or os.path.isdir(common_dir) is False:
+            os.makedirs(common_dir)
+        current_feed_path = os.path.join(common_dir,latest_package_key)
+        current_bucket_name = 'gpu-model-data'
+                           
+        need_redownload = False
+        if os.path.exists(latest_package_key) is False:
+            self.__logger.debug(f'current_all_feeds_path {current_feed_path}  not exist')
+            need_redownload = True
+        else:
+            exist_protobuf_compress_hash = self.__common_tool.calculate_md5_for_big_file(current_feed_path)
+            self.__logger.debug(f'current_feed_path {current_feed_path} does  exist ,exist file hash {exist_protobuf_compress_hash}')
+            response_header = self.__awss3tool.get_object_header(current_bucket_name, latest_package_key)
+            if ("ResponseMetadata" not in response_header or 
+                "HTTPStatusCode" not in response_header["ResponseMetadata"] or
+                response_header["ResponseMetadata"]["HTTPStatusCode"] != 200):
+                raise ValueError(f'current_bucket { current_bucket_name} key {latest_package_key} not exist')
+            if response_header["Metadata"]["md5_digest"] != exist_protobuf_compress_hash:
+                need_redownload = True
+                
+        if need_redownload:
+            result = self.__awss3tool.get_object_byte(current_bucket_name,latest_package_key)
+            if result["success"] is False:
+                raise ValueError(f"download embedding package fail result {result}")
+            current_package_compress_byte = result["bytes"]
+            with open(current_feed_path,'wb') as f:
+                f.write(current_package_compress_byte)
+            self.__logger.debug(f'need_download {current_feed_path}')
+        else:
+            with open(current_feed_path,'rb') as f:
+                current_package_compress_byte = f.read()
+        
+        decompress_bytes = zlib.decompress(current_package_compress_byte)
+        current_latest_package = rec_proto_embebding.CategoryPackage()
+        current_latest_package.ParseFromString(decompress_bytes)
+        
+        all_category_dict = MessageToDict(current_latest_package,preserving_proto_field_name=True)
+        all_category_list = all_category_dict["category_list"]
+        category_name_to_category = dict()
+        for current_category in all_category_list:
+            category_name_to_category[current_category["category"]] = current_category
+        return category_name_to_category
```

### Comparing `bytetrade-recommend-model-sdk-0.0.30/setup.py` & `bytetrade-recommend-model-sdk-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 sys.path.append(os.path.dirname(__file__) + "/recommend-model")
 
 
 
 
 setup(
     name="bytetrade-recommend-model-sdk",
-    version="0.0.30",
+    version="0.1.0",
     # packages=find_packages(exclude="unit_test"),
     install_requires=[
         "pandas==2.0.0",
         "gensim==4.3.1",
         "protobuf==3.20.1",
         "nltk==3.8.1",
         "boto3",
```

