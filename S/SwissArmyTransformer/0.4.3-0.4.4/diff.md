# Comparing `tmp/SwissArmyTransformer-0.4.3.tar.gz` & `tmp/SwissArmyTransformer-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/mingding/SwissArmyTransformer/dist/.tmp-qslo7ee3/SwissArmyTransformer-0.4.3.tar", last modified: Thu Jul 20 02:34:36 2023, max compression
+gzip compressed data, was "/home/mingding/SwissArmyTransformer/dist/.tmp-o28yxwdk/SwissArmyTransformer-0.4.4.tar", last modified: Mon Aug  7 07:09:06 2023, max compression
```

## Comparing `SwissArmyTransformer-0.4.3.tar` & `SwissArmyTransformer-0.4.4.tar`

### file list

```diff
@@ -1,176 +1,176 @@
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-20 02:34:36.043721 SwissArmyTransformer-0.4.3/
--rw-rw-r--   0 mingding  (1001) mingding  (1001)    11338 2023-04-06 14:24:30.000000 SwissArmyTransformer-0.4.3/LICENSE
--rw-rw-r--   0 mingding  (1001) mingding  (1001)      191 2023-06-28 10:22:33.000000 SwissArmyTransformer-0.4.3/MANIFEST.in
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     9893 2023-07-20 02:34:36.043721 SwissArmyTransformer-0.4.3/PKG-INFO
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     9521 2023-07-19 11:34:10.000000 SwissArmyTransformer-0.4.3/README.md
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-20 02:34:36.023721 SwissArmyTransformer-0.4.3/SwissArmyTransformer.egg-info/
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     9893 2023-07-20 02:34:35.000000 SwissArmyTransformer-0.4.3/SwissArmyTransformer.egg-info/PKG-INFO
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     4934 2023-07-20 02:34:36.000000 SwissArmyTransformer-0.4.3/SwissArmyTransformer.egg-info/SOURCES.txt
--rw-rw-r--   0 mingding  (1001) mingding  (1001)        1 2023-07-20 02:34:35.000000 SwissArmyTransformer-0.4.3/SwissArmyTransformer.egg-info/dependency_links.txt
--rw-rw-r--   0 mingding  (1001) mingding  (1001)       90 2023-07-20 02:34:35.000000 SwissArmyTransformer-0.4.3/SwissArmyTransformer.egg-info/requires.txt
--rw-rw-r--   0 mingding  (1001) mingding  (1001)        4 2023-07-20 02:34:35.000000 SwissArmyTransformer-0.4.3/SwissArmyTransformer.egg-info/top_level.txt
--rw-rw-r--   0 mingding  (1001) mingding  (1001)       89 2023-06-28 07:19:19.000000 SwissArmyTransformer-0.4.3/requirements.txt
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-20 02:34:36.023721 SwissArmyTransformer-0.4.3/sat/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      433 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.4.3/sat/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    25746 2023-07-19 11:34:10.000000 SwissArmyTransformer-0.4.3/sat/arguments.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-20 02:34:36.027721 SwissArmyTransformer-0.4.3/sat/data_utils/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      288 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.3/sat/data_utils/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    15633 2023-07-19 11:34:10.000000 SwissArmyTransformer-0.4.3/sat/data_utils/configure_data.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     2676 2023-06-28 10:22:33.000000 SwissArmyTransformer-0.4.3/sat/data_utils/datasets.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1894 2023-05-14 16:34:50.000000 SwissArmyTransformer-0.4.3/sat/data_utils/hf_dataset.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     7028 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.3/sat/data_utils/samplers.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     7129 2023-06-28 10:22:33.000000 SwissArmyTransformer-0.4.3/sat/data_utils/webds.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-20 02:34:36.027721 SwissArmyTransformer-0.4.3/sat/generation/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.3/sat/generation/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     9777 2023-07-05 09:18:31.000000 SwissArmyTransformer-0.4.3/sat/generation/autoregressive_sampling.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3218 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.3/sat/generation/cuda2d_sampling.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1709 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.3/sat/generation/magnify.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-20 02:34:36.027721 SwissArmyTransformer-0.4.3/sat/generation/sampling_strategies/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      161 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.3/sat/generation/sampling_strategies/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4300 2023-07-19 11:34:10.000000 SwissArmyTransformer-0.4.3/sat/generation/sampling_strategies/base_strategy.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     7659 2023-07-19 11:34:10.000000 SwissArmyTransformer-0.4.3/sat/generation/sampling_strategies/beam_search_strategy.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     2270 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.3/sat/generation/sampling_strategies/iterative_entfilter_strategy.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3201 2023-04-28 08:57:23.000000 SwissArmyTransformer-0.4.3/sat/generation/utils.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     5187 2023-05-16 12:24:16.000000 SwissArmyTransformer-0.4.3/sat/helpers.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-20 02:34:36.027721 SwissArmyTransformer-0.4.3/sat/model/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      214 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.4.3/sat/model/__init__.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-20 02:34:36.027721 SwissArmyTransformer-0.4.3/sat/model/attention/
--rw-rw-r--   0 mingding  (1001) mingding  (1001)      110 2023-06-06 14:36:22.000000 SwissArmyTransformer-0.4.3/sat/model/attention/__init__.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     3654 2023-06-07 06:54:10.000000 SwissArmyTransformer-0.4.3/sat/model/attention/memory_efficient_attention.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    16317 2023-07-19 11:34:10.000000 SwissArmyTransformer-0.4.3/sat/model/base_model.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1731 2023-07-05 09:18:31.000000 SwissArmyTransformer-0.4.3/sat/model/cached_autoregressive_model.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     5479 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.4.3/sat/model/encoder_decoder_model.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-20 02:34:36.027721 SwissArmyTransformer-0.4.3/sat/model/finetune/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      187 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.3/sat/model/finetune/__init__.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     2659 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.3/sat/model/finetune/adapter.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     2019 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.3/sat/model/finetune/ffadd.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     3879 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.3/sat/model/finetune/lora.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)    12034 2023-07-20 02:34:12.000000 SwissArmyTransformer-0.4.3/sat/model/finetune/lora2.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1110 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.3/sat/model/finetune/mlp_head.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1611 2023-07-19 11:34:10.000000 SwissArmyTransformer-0.4.3/sat/model/finetune/prompt_tuning.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      391 2023-06-06 14:36:32.000000 SwissArmyTransformer-0.4.3/sat/model/mixins.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-20 02:34:36.027721 SwissArmyTransformer-0.4.3/sat/model/normalization/
--rw-rw-r--   0 mingding  (1001) mingding  (1001)       24 2023-07-05 09:18:31.000000 SwissArmyTransformer-0.4.3/sat/model/normalization/__init__.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)      610 2023-07-05 09:18:31.000000 SwissArmyTransformer-0.4.3/sat/model/normalization/rms.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-20 02:34:36.031721 SwissArmyTransformer-0.4.3/sat/model/official/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      676 2023-07-05 09:18:31.000000 SwissArmyTransformer-0.4.3/sat/model/official/__init__.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     1923 2023-07-05 09:18:31.000000 SwissArmyTransformer-0.4.3/sat/model/official/bert_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)    10409 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.3/sat/model/official/cait_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     7173 2023-07-19 11:34:10.000000 SwissArmyTransformer-0.4.3/sat/model/official/chatglm2_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)    11846 2023-07-19 11:34:10.000000 SwissArmyTransformer-0.4.3/sat/model/official/chatglm_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     7294 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.4.3/sat/model/official/clip_model.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     9612 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.4.3/sat/model/official/cuda2d_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     1310 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.3/sat/model/official/distill_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     3942 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.3/sat/model/official/dpr_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     7369 2023-05-14 14:59:40.000000 SwissArmyTransformer-0.4.3/sat/model/official/eva2_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)    13903 2023-06-06 13:57:30.000000 SwissArmyTransformer-0.4.3/sat/model/official/glm130B_model.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3751 2023-05-10 18:09:38.000000 SwissArmyTransformer-0.4.3/sat/model/official/glm_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)      978 2023-07-19 11:34:10.000000 SwissArmyTransformer-0.4.3/sat/model/official/gpt2_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     4648 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.3/sat/model/official/gptneo_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     5113 2023-07-19 11:34:10.000000 SwissArmyTransformer-0.4.3/sat/model/official/llama_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     8336 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.3/sat/model/official/mae_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)      262 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.3/sat/model/official/roberta_model.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    14715 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.3/sat/model/official/t5_model.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     6254 2023-05-27 05:12:45.000000 SwissArmyTransformer-0.4.3/sat/model/official/vit_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     2969 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.3/sat/model/official/yolos_model.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-20 02:34:36.031721 SwissArmyTransformer-0.4.3/sat/model/position_embedding/
--rw-rw-r--   0 mingding  (1001) mingding  (1001)      296 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.3/sat/model/position_embedding/__init__.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     5388 2023-07-19 11:34:10.000000 SwissArmyTransformer-0.4.3/sat/model/position_embedding/rotary_embeddings.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     2713 2023-07-05 09:18:31.000000 SwissArmyTransformer-0.4.3/sat/model/position_embedding/rotary_embeddings_original.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     4078 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.3/sat/model/position_embedding/sincos2d.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     5021 2023-05-16 18:46:06.000000 SwissArmyTransformer-0.4.3/sat/model/position_embedding/vision_rotary_embeddings.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     1199 2023-07-19 11:34:10.000000 SwissArmyTransformer-0.4.3/sat/model/registry.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    29395 2023-07-19 11:34:10.000000 SwissArmyTransformer-0.4.3/sat/model/transformer.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-20 02:34:36.031721 SwissArmyTransformer-0.4.3/sat/mpu/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     2263 2023-07-19 11:34:10.000000 SwissArmyTransformer-0.4.3/sat/mpu/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4716 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.3/sat/mpu/cross_entropy.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4018 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.3/sat/mpu/data.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     6435 2023-07-19 11:34:10.000000 SwissArmyTransformer-0.4.3/sat/mpu/initialize.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    22165 2023-07-19 11:34:10.000000 SwissArmyTransformer-0.4.3/sat/mpu/layers.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4136 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.3/sat/mpu/mappings.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     3898 2023-07-19 11:34:10.000000 SwissArmyTransformer-0.4.3/sat/mpu/operation.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3924 2023-07-05 09:18:31.000000 SwissArmyTransformer-0.4.3/sat/mpu/utils.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-20 02:34:36.031721 SwissArmyTransformer-0.4.3/sat/ops/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1159 2023-07-19 11:34:10.000000 SwissArmyTransformer-0.4.3/sat/ops/__init__.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-20 02:34:36.023721 SwissArmyTransformer-0.4.3/sat/ops/csrc/
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-20 02:34:36.035721 SwissArmyTransformer-0.4.3/sat/ops/csrc/adam/
--rw-rw-r--   0 mingding  (1001) mingding  (1001)      947 2023-06-28 10:22:33.000000 SwissArmyTransformer-0.4.3/sat/ops/csrc/adam/fused_ema_adam_frontend.cpp
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     5595 2023-06-28 10:22:33.000000 SwissArmyTransformer-0.4.3/sat/ops/csrc/adam/multi_tensor_apply.cuh
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     7076 2023-06-28 10:22:33.000000 SwissArmyTransformer-0.4.3/sat/ops/csrc/adam/multi_tensor_ema_adam.cu
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-20 02:34:36.035721 SwissArmyTransformer-0.4.3/sat/ops/csrc/includes/
--rw-rw-r--   0 mingding  (1001) mingding  (1001)      336 2023-06-28 10:22:33.000000 SwissArmyTransformer-0.4.3/sat/ops/csrc/includes/compat.h
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     6388 2023-06-28 10:22:33.000000 SwissArmyTransformer-0.4.3/sat/ops/csrc/includes/type_shim.h
--rw-rw-r--   0 mingding  (1001) mingding  (1001)    10712 2023-06-28 10:22:33.000000 SwissArmyTransformer-0.4.3/sat/ops/fused_ema_adam.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1159 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.4.3/sat/ops/layernorm.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     2067 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.3/sat/ops/local_attention_function.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)      578 2023-06-07 05:52:48.000000 SwissArmyTransformer-0.4.3/sat/ops/memory_efficient_attention.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-20 02:34:36.035721 SwissArmyTransformer-0.4.3/sat/ops/ops_builder/
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     1982 2023-06-28 10:22:33.000000 SwissArmyTransformer-0.4.3/sat/ops/ops_builder/__init__.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)    28554 2023-06-28 10:22:33.000000 SwissArmyTransformer-0.4.3/sat/ops/ops_builder/builder.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)      957 2023-06-28 10:22:33.000000 SwissArmyTransformer-0.4.3/sat/ops/ops_builder/fused_ema_adam.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)      389 2023-06-05 05:26:26.000000 SwissArmyTransformer-0.4.3/sat/ops/scaled_mask_softmax.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-20 02:34:36.035721 SwissArmyTransformer-0.4.3/sat/quantization/
--rw-rw-r--   0 mingding  (1001) mingding  (1001)       29 2023-05-16 09:41:04.000000 SwissArmyTransformer-0.4.3/sat/quantization/__init__.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)    18674 2023-05-16 09:41:04.000000 SwissArmyTransformer-0.4.3/sat/quantization/kernels.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-20 02:34:36.035721 SwissArmyTransformer-0.4.3/sat/resources/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)       33 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.3/sat/resources/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     6815 2023-07-19 11:34:10.000000 SwissArmyTransformer-0.4.3/sat/resources/download.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     3531 2023-07-19 11:34:10.000000 SwissArmyTransformer-0.4.3/sat/resources/urls.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-20 02:34:36.035721 SwissArmyTransformer-0.4.3/sat/tokenization/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3810 2023-05-14 16:27:55.000000 SwissArmyTransformer-0.4.3/sat/tokenization/__init__.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-20 02:34:36.035721 SwissArmyTransformer-0.4.3/sat/tokenization/cogview/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      303 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.3/sat/tokenization/cogview/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     5092 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.3/sat/tokenization/cogview/sp_tokenizer.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1767 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.3/sat/tokenization/cogview/templates.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     7095 2023-05-14 16:38:45.000000 SwissArmyTransformer-0.4.3/sat/tokenization/cogview/unified_tokenizer.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-20 02:34:36.035721 SwissArmyTransformer-0.4.3/sat/tokenization/cogview/vqvae/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      167 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.3/sat/tokenization/cogview/vqvae/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     7691 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.3/sat/tokenization/cogview/vqvae/api.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    30392 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.3/sat/tokenization/cogview/vqvae/vqvae_diffusion.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    12917 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.3/sat/tokenization/cogview/vqvae/vqvae_zc.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     2453 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.3/sat/tokenization/cogview/vqvae_tokenizer.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-20 02:34:36.023721 SwissArmyTransformer-0.4.3/sat/tokenization/embed_assets/
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-20 02:34:36.035721 SwissArmyTransformer-0.4.3/sat/tokenization/embed_assets/chinese_sentencepiece/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)  1021864 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.3/sat/tokenization/embed_assets/chinese_sentencepiece/cog-pretrain.model
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)   723078 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.3/sat/tokenization/embed_assets/chinese_sentencepiece/cog-pretrain.vocab
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-20 02:34:36.039721 SwissArmyTransformer-0.4.3/sat/tokenization/embed_assets/english_tokenizer/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)   231508 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.3/sat/tokenization/embed_assets/english_tokenizer/bert-base-uncased-vocab.txt
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)   231508 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.3/sat/tokenization/embed_assets/english_tokenizer/bert-large-uncased-vocab.txt
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)   456318 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.3/sat/tokenization/embed_assets/english_tokenizer/gpt2-merges.txt
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)  1042301 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.3/sat/tokenization/embed_assets/english_tokenizer/gpt2-vocab.json
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)   456318 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.3/sat/tokenization/embed_assets/english_tokenizer/roberta-merges.txt
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)   898823 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.3/sat/tokenization/embed_assets/english_tokenizer/roberta-vocab.json
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-20 02:34:36.043721 SwissArmyTransformer-0.4.3/sat/tokenization/glm/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)       87 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.3/sat/tokenization/glm/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3272 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.3/sat/tokenization/glm/sp_tokenizer.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    23223 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.3/sat/tokenization/glm/tokenization.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    13844 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.3/sat/tokenization/glm/tokenization_gpt2.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)    14571 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.3/sat/tokenization/glm/tokenization_wordpiece.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3271 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.3/sat/tokenization/hf_tokenizer.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-20 02:34:36.043721 SwissArmyTransformer-0.4.3/sat/tokenization/icetk_glm_130B/
--rw-rw-r--   0 mingding  (1001) mingding  (1001)       40 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.3/sat/tokenization/icetk_glm_130B/__init__.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     9661 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.3/sat/tokenization/icetk_glm_130B/ice_tokenizer.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     2295 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.3/sat/tokenization/icetk_glm_130B/tokenizer.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-20 02:34:36.043721 SwissArmyTransformer-0.4.3/sat/training/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.4.3/sat/training/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    24074 2023-07-19 11:34:10.000000 SwissArmyTransformer-0.4.3/sat/training/deepspeed_training.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      392 2023-07-19 11:34:10.000000 SwissArmyTransformer-0.4.3/sat/training/deepspeed_zero0.json
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      999 2023-07-19 11:34:10.000000 SwissArmyTransformer-0.4.3/sat/training/deepspeed_zero1.json
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1151 2023-07-19 11:34:10.000000 SwissArmyTransformer-0.4.3/sat/training/deepspeed_zero2.json
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3475 2023-05-14 16:38:27.000000 SwissArmyTransformer-0.4.3/sat/training/learning_rates.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    11576 2023-07-05 09:18:31.000000 SwissArmyTransformer-0.4.3/sat/training/model_io.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4488 2023-05-14 16:28:13.000000 SwissArmyTransformer-0.4.3/sat/training/utils.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     9665 2023-07-19 11:34:10.000000 SwissArmyTransformer-0.4.3/sat/transformer_defaults.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)       38 2023-07-20 02:34:36.043721 SwissArmyTransformer-0.4.3/setup.cfg
--rw-rw-r--   0 mingding  (1001) mingding  (1001)      880 2023-07-20 02:34:26.000000 SwissArmyTransformer-0.4.3/setup.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-07-20 02:34:36.043721 SwissArmyTransformer-0.4.3/tests/
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     2000 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.3/tests/test_base_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     1530 2023-04-21 12:58:44.000000 SwissArmyTransformer-0.4.3/tests/test_inference.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)      290 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.3/tests/test_list_info.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     3104 2023-06-07 06:54:04.000000 SwissArmyTransformer-0.4.3/tests/test_mea.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)      913 2023-07-05 09:18:31.000000 SwissArmyTransformer-0.4.3/tests/test_model_parallel.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     2134 2023-05-10 18:09:38.000000 SwissArmyTransformer-0.4.3/tests/test_nested_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)      611 2023-05-18 18:05:46.000000 SwissArmyTransformer-0.4.3/tests/test_speed.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     4078 2023-04-21 12:58:44.000000 SwissArmyTransformer-0.4.3/tests/test_train.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     4078 2023-05-17 07:43:42.000000 SwissArmyTransformer-0.4.3/tests/test_train_dp.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     4336 2023-05-10 18:09:38.000000 SwissArmyTransformer-0.4.3/tests/test_train_nested.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-08-07 07:09:06.873337 SwissArmyTransformer-0.4.4/
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)    11338 2023-04-06 14:24:30.000000 SwissArmyTransformer-0.4.4/LICENSE
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)      191 2023-06-28 10:22:33.000000 SwissArmyTransformer-0.4.4/MANIFEST.in
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     9893 2023-08-07 07:09:06.873337 SwissArmyTransformer-0.4.4/PKG-INFO
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     9521 2023-07-19 11:34:10.000000 SwissArmyTransformer-0.4.4/README.md
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-08-07 07:09:06.845337 SwissArmyTransformer-0.4.4/SwissArmyTransformer.egg-info/
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     9893 2023-08-07 07:09:06.000000 SwissArmyTransformer-0.4.4/SwissArmyTransformer.egg-info/PKG-INFO
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     4934 2023-08-07 07:09:06.000000 SwissArmyTransformer-0.4.4/SwissArmyTransformer.egg-info/SOURCES.txt
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)        1 2023-08-07 07:09:06.000000 SwissArmyTransformer-0.4.4/SwissArmyTransformer.egg-info/dependency_links.txt
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)       90 2023-08-07 07:09:06.000000 SwissArmyTransformer-0.4.4/SwissArmyTransformer.egg-info/requires.txt
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)        4 2023-08-07 07:09:06.000000 SwissArmyTransformer-0.4.4/SwissArmyTransformer.egg-info/top_level.txt
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)       89 2023-06-28 07:19:19.000000 SwissArmyTransformer-0.4.4/requirements.txt
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-08-07 07:09:06.845337 SwissArmyTransformer-0.4.4/sat/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      433 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.4.4/sat/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    25746 2023-07-19 11:34:10.000000 SwissArmyTransformer-0.4.4/sat/arguments.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-08-07 07:09:06.845337 SwissArmyTransformer-0.4.4/sat/data_utils/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      288 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.4/sat/data_utils/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    15633 2023-07-19 11:34:10.000000 SwissArmyTransformer-0.4.4/sat/data_utils/configure_data.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     2676 2023-06-28 10:22:33.000000 SwissArmyTransformer-0.4.4/sat/data_utils/datasets.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1894 2023-05-14 16:34:50.000000 SwissArmyTransformer-0.4.4/sat/data_utils/hf_dataset.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     7028 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.4/sat/data_utils/samplers.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     7178 2023-08-07 07:07:38.000000 SwissArmyTransformer-0.4.4/sat/data_utils/webds.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-08-07 07:09:06.845337 SwissArmyTransformer-0.4.4/sat/generation/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.4/sat/generation/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     9787 2023-07-24 03:04:00.000000 SwissArmyTransformer-0.4.4/sat/generation/autoregressive_sampling.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3218 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.4/sat/generation/cuda2d_sampling.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1709 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.4/sat/generation/magnify.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-08-07 07:09:06.845337 SwissArmyTransformer-0.4.4/sat/generation/sampling_strategies/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      161 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.4/sat/generation/sampling_strategies/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4300 2023-07-19 11:34:10.000000 SwissArmyTransformer-0.4.4/sat/generation/sampling_strategies/base_strategy.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     7659 2023-07-19 11:34:10.000000 SwissArmyTransformer-0.4.4/sat/generation/sampling_strategies/beam_search_strategy.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     2270 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.4/sat/generation/sampling_strategies/iterative_entfilter_strategy.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3201 2023-04-28 08:57:23.000000 SwissArmyTransformer-0.4.4/sat/generation/utils.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     5187 2023-05-16 12:24:16.000000 SwissArmyTransformer-0.4.4/sat/helpers.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-08-07 07:09:06.845337 SwissArmyTransformer-0.4.4/sat/model/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      214 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.4.4/sat/model/__init__.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-08-07 07:09:06.845337 SwissArmyTransformer-0.4.4/sat/model/attention/
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)      110 2023-06-06 14:36:22.000000 SwissArmyTransformer-0.4.4/sat/model/attention/__init__.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     3654 2023-06-07 06:54:10.000000 SwissArmyTransformer-0.4.4/sat/model/attention/memory_efficient_attention.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    16317 2023-07-19 11:34:10.000000 SwissArmyTransformer-0.4.4/sat/model/base_model.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1731 2023-07-05 09:18:31.000000 SwissArmyTransformer-0.4.4/sat/model/cached_autoregressive_model.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     5479 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.4.4/sat/model/encoder_decoder_model.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-08-07 07:09:06.849337 SwissArmyTransformer-0.4.4/sat/model/finetune/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      187 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.4/sat/model/finetune/__init__.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     2659 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.4/sat/model/finetune/adapter.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     2019 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.4/sat/model/finetune/ffadd.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     3879 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.4/sat/model/finetune/lora.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)    12034 2023-07-20 02:34:12.000000 SwissArmyTransformer-0.4.4/sat/model/finetune/lora2.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1110 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.4/sat/model/finetune/mlp_head.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1611 2023-07-19 11:34:10.000000 SwissArmyTransformer-0.4.4/sat/model/finetune/prompt_tuning.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      391 2023-06-06 14:36:32.000000 SwissArmyTransformer-0.4.4/sat/model/mixins.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-08-07 07:09:06.849337 SwissArmyTransformer-0.4.4/sat/model/normalization/
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)       24 2023-07-05 09:18:31.000000 SwissArmyTransformer-0.4.4/sat/model/normalization/__init__.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)      610 2023-07-05 09:18:31.000000 SwissArmyTransformer-0.4.4/sat/model/normalization/rms.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-08-07 07:09:06.853337 SwissArmyTransformer-0.4.4/sat/model/official/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      676 2023-07-05 09:18:31.000000 SwissArmyTransformer-0.4.4/sat/model/official/__init__.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     1923 2023-07-05 09:18:31.000000 SwissArmyTransformer-0.4.4/sat/model/official/bert_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)    10409 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.4/sat/model/official/cait_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     7173 2023-07-19 11:34:10.000000 SwissArmyTransformer-0.4.4/sat/model/official/chatglm2_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)    11846 2023-07-19 11:34:10.000000 SwissArmyTransformer-0.4.4/sat/model/official/chatglm_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     7294 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.4.4/sat/model/official/clip_model.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     9612 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.4.4/sat/model/official/cuda2d_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     1310 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.4/sat/model/official/distill_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     3942 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.4/sat/model/official/dpr_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     7369 2023-05-14 14:59:40.000000 SwissArmyTransformer-0.4.4/sat/model/official/eva2_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)    13903 2023-06-06 13:57:30.000000 SwissArmyTransformer-0.4.4/sat/model/official/glm130B_model.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3751 2023-05-10 18:09:38.000000 SwissArmyTransformer-0.4.4/sat/model/official/glm_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)      978 2023-07-19 11:34:10.000000 SwissArmyTransformer-0.4.4/sat/model/official/gpt2_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     4648 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.4/sat/model/official/gptneo_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     5123 2023-07-24 03:04:00.000000 SwissArmyTransformer-0.4.4/sat/model/official/llama_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     8336 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.4/sat/model/official/mae_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)      262 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.4/sat/model/official/roberta_model.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    14715 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.4/sat/model/official/t5_model.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     6254 2023-05-27 05:12:45.000000 SwissArmyTransformer-0.4.4/sat/model/official/vit_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     2969 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.4/sat/model/official/yolos_model.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-08-07 07:09:06.857337 SwissArmyTransformer-0.4.4/sat/model/position_embedding/
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)      296 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.4/sat/model/position_embedding/__init__.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     5388 2023-07-19 11:34:10.000000 SwissArmyTransformer-0.4.4/sat/model/position_embedding/rotary_embeddings.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     2713 2023-07-05 09:18:31.000000 SwissArmyTransformer-0.4.4/sat/model/position_embedding/rotary_embeddings_original.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     4078 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.4/sat/model/position_embedding/sincos2d.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     5021 2023-05-16 18:46:06.000000 SwissArmyTransformer-0.4.4/sat/model/position_embedding/vision_rotary_embeddings.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     1199 2023-07-19 11:34:10.000000 SwissArmyTransformer-0.4.4/sat/model/registry.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    29354 2023-08-07 07:07:38.000000 SwissArmyTransformer-0.4.4/sat/model/transformer.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-08-07 07:09:06.857337 SwissArmyTransformer-0.4.4/sat/mpu/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     2263 2023-07-19 11:34:10.000000 SwissArmyTransformer-0.4.4/sat/mpu/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4716 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.4/sat/mpu/cross_entropy.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4018 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.4/sat/mpu/data.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     6435 2023-07-19 11:34:10.000000 SwissArmyTransformer-0.4.4/sat/mpu/initialize.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    22165 2023-07-19 11:34:10.000000 SwissArmyTransformer-0.4.4/sat/mpu/layers.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4136 2023-07-24 07:39:22.000000 SwissArmyTransformer-0.4.4/sat/mpu/mappings.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     3898 2023-07-19 11:34:10.000000 SwissArmyTransformer-0.4.4/sat/mpu/operation.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3924 2023-07-05 09:18:31.000000 SwissArmyTransformer-0.4.4/sat/mpu/utils.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-08-07 07:09:06.857337 SwissArmyTransformer-0.4.4/sat/ops/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1159 2023-07-19 11:34:10.000000 SwissArmyTransformer-0.4.4/sat/ops/__init__.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-08-07 07:09:06.841337 SwissArmyTransformer-0.4.4/sat/ops/csrc/
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-08-07 07:09:06.861337 SwissArmyTransformer-0.4.4/sat/ops/csrc/adam/
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)      947 2023-06-28 10:22:33.000000 SwissArmyTransformer-0.4.4/sat/ops/csrc/adam/fused_ema_adam_frontend.cpp
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     5595 2023-06-28 10:22:33.000000 SwissArmyTransformer-0.4.4/sat/ops/csrc/adam/multi_tensor_apply.cuh
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     7076 2023-06-28 10:22:33.000000 SwissArmyTransformer-0.4.4/sat/ops/csrc/adam/multi_tensor_ema_adam.cu
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-08-07 07:09:06.861337 SwissArmyTransformer-0.4.4/sat/ops/csrc/includes/
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)      336 2023-06-28 10:22:33.000000 SwissArmyTransformer-0.4.4/sat/ops/csrc/includes/compat.h
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     6388 2023-06-28 10:22:33.000000 SwissArmyTransformer-0.4.4/sat/ops/csrc/includes/type_shim.h
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)    10712 2023-06-28 10:22:33.000000 SwissArmyTransformer-0.4.4/sat/ops/fused_ema_adam.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1159 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.4.4/sat/ops/layernorm.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     2067 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.4/sat/ops/local_attention_function.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)      578 2023-06-07 05:52:48.000000 SwissArmyTransformer-0.4.4/sat/ops/memory_efficient_attention.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-08-07 07:09:06.861337 SwissArmyTransformer-0.4.4/sat/ops/ops_builder/
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     1982 2023-06-28 10:22:33.000000 SwissArmyTransformer-0.4.4/sat/ops/ops_builder/__init__.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)    28554 2023-06-28 10:22:33.000000 SwissArmyTransformer-0.4.4/sat/ops/ops_builder/builder.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)      957 2023-06-28 10:22:33.000000 SwissArmyTransformer-0.4.4/sat/ops/ops_builder/fused_ema_adam.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)      389 2023-06-05 05:26:26.000000 SwissArmyTransformer-0.4.4/sat/ops/scaled_mask_softmax.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-08-07 07:09:06.861337 SwissArmyTransformer-0.4.4/sat/quantization/
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)       29 2023-05-16 09:41:04.000000 SwissArmyTransformer-0.4.4/sat/quantization/__init__.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)    18674 2023-05-16 09:41:04.000000 SwissArmyTransformer-0.4.4/sat/quantization/kernels.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-08-07 07:09:06.861337 SwissArmyTransformer-0.4.4/sat/resources/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)       33 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.4/sat/resources/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     6815 2023-07-19 11:34:10.000000 SwissArmyTransformer-0.4.4/sat/resources/download.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     3531 2023-07-19 11:34:10.000000 SwissArmyTransformer-0.4.4/sat/resources/urls.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-08-07 07:09:06.861337 SwissArmyTransformer-0.4.4/sat/tokenization/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3810 2023-05-14 16:27:55.000000 SwissArmyTransformer-0.4.4/sat/tokenization/__init__.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-08-07 07:09:06.861337 SwissArmyTransformer-0.4.4/sat/tokenization/cogview/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      303 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.4/sat/tokenization/cogview/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     5092 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.4/sat/tokenization/cogview/sp_tokenizer.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1767 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.4/sat/tokenization/cogview/templates.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     7095 2023-05-14 16:38:45.000000 SwissArmyTransformer-0.4.4/sat/tokenization/cogview/unified_tokenizer.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-08-07 07:09:06.861337 SwissArmyTransformer-0.4.4/sat/tokenization/cogview/vqvae/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      167 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.4/sat/tokenization/cogview/vqvae/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     7691 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.4/sat/tokenization/cogview/vqvae/api.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    30392 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.4/sat/tokenization/cogview/vqvae/vqvae_diffusion.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    12917 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.4/sat/tokenization/cogview/vqvae/vqvae_zc.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     2453 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.4/sat/tokenization/cogview/vqvae_tokenizer.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-08-07 07:09:06.841337 SwissArmyTransformer-0.4.4/sat/tokenization/embed_assets/
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-08-07 07:09:06.865337 SwissArmyTransformer-0.4.4/sat/tokenization/embed_assets/chinese_sentencepiece/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)  1021864 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.4/sat/tokenization/embed_assets/chinese_sentencepiece/cog-pretrain.model
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)   723078 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.4/sat/tokenization/embed_assets/chinese_sentencepiece/cog-pretrain.vocab
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-08-07 07:09:06.869337 SwissArmyTransformer-0.4.4/sat/tokenization/embed_assets/english_tokenizer/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)   231508 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.4/sat/tokenization/embed_assets/english_tokenizer/bert-base-uncased-vocab.txt
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)   231508 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.4/sat/tokenization/embed_assets/english_tokenizer/bert-large-uncased-vocab.txt
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)   456318 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.4/sat/tokenization/embed_assets/english_tokenizer/gpt2-merges.txt
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)  1042301 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.4/sat/tokenization/embed_assets/english_tokenizer/gpt2-vocab.json
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)   456318 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.4/sat/tokenization/embed_assets/english_tokenizer/roberta-merges.txt
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)   898823 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.4/sat/tokenization/embed_assets/english_tokenizer/roberta-vocab.json
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-08-07 07:09:06.869337 SwissArmyTransformer-0.4.4/sat/tokenization/glm/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)       87 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.4/sat/tokenization/glm/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3272 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.4/sat/tokenization/glm/sp_tokenizer.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    23223 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.4/sat/tokenization/glm/tokenization.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    13844 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.4/sat/tokenization/glm/tokenization_gpt2.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)    14571 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.4/sat/tokenization/glm/tokenization_wordpiece.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3271 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.4/sat/tokenization/hf_tokenizer.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-08-07 07:09:06.869337 SwissArmyTransformer-0.4.4/sat/tokenization/icetk_glm_130B/
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)       40 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.4/sat/tokenization/icetk_glm_130B/__init__.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     9661 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.4/sat/tokenization/icetk_glm_130B/ice_tokenizer.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     2295 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.4/sat/tokenization/icetk_glm_130B/tokenizer.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-08-07 07:09:06.869337 SwissArmyTransformer-0.4.4/sat/training/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.4.4/sat/training/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    24074 2023-07-19 11:34:10.000000 SwissArmyTransformer-0.4.4/sat/training/deepspeed_training.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      392 2023-07-19 11:34:10.000000 SwissArmyTransformer-0.4.4/sat/training/deepspeed_zero0.json
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      999 2023-07-19 11:34:10.000000 SwissArmyTransformer-0.4.4/sat/training/deepspeed_zero1.json
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1151 2023-07-19 11:34:10.000000 SwissArmyTransformer-0.4.4/sat/training/deepspeed_zero2.json
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3475 2023-05-14 16:38:27.000000 SwissArmyTransformer-0.4.4/sat/training/learning_rates.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    11619 2023-08-07 07:07:38.000000 SwissArmyTransformer-0.4.4/sat/training/model_io.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4488 2023-05-14 16:28:13.000000 SwissArmyTransformer-0.4.4/sat/training/utils.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     9862 2023-08-07 07:07:38.000000 SwissArmyTransformer-0.4.4/sat/transformer_defaults.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)       38 2023-08-07 07:09:06.873337 SwissArmyTransformer-0.4.4/setup.cfg
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)      880 2023-08-07 07:08:48.000000 SwissArmyTransformer-0.4.4/setup.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-08-07 07:09:06.873337 SwissArmyTransformer-0.4.4/tests/
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     2000 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.4/tests/test_base_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     1530 2023-04-21 12:58:44.000000 SwissArmyTransformer-0.4.4/tests/test_inference.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)      290 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.4.4/tests/test_list_info.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     3104 2023-06-07 06:54:04.000000 SwissArmyTransformer-0.4.4/tests/test_mea.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)      913 2023-07-05 09:18:31.000000 SwissArmyTransformer-0.4.4/tests/test_model_parallel.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     2134 2023-05-10 18:09:38.000000 SwissArmyTransformer-0.4.4/tests/test_nested_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)      611 2023-05-18 18:05:46.000000 SwissArmyTransformer-0.4.4/tests/test_speed.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     4078 2023-04-21 12:58:44.000000 SwissArmyTransformer-0.4.4/tests/test_train.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     4078 2023-05-17 07:43:42.000000 SwissArmyTransformer-0.4.4/tests/test_train_dp.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     4336 2023-05-10 18:09:38.000000 SwissArmyTransformer-0.4.4/tests/test_train_nested.py
```

### Comparing `SwissArmyTransformer-0.4.3/LICENSE` & `SwissArmyTransformer-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/PKG-INFO` & `SwissArmyTransformer-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SwissArmyTransformer
-Version: 0.4.3
+Version: 0.4.4
 Summary: A transformer-based framework with finetuning as the first class citizen.
 Home-page: https://github.com/THUDM/SwissArmyTransformer
 Author: Ming Ding, et al.
 Author-email: dm_thu@qq.com
 License: Apache 2.0 license
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
```

### Comparing `SwissArmyTransformer-0.4.3/README.md` & `SwissArmyTransformer-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/SwissArmyTransformer.egg-info/PKG-INFO` & `SwissArmyTransformer-0.4.4/SwissArmyTransformer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SwissArmyTransformer
-Version: 0.4.3
+Version: 0.4.4
 Summary: A transformer-based framework with finetuning as the first class citizen.
 Home-page: https://github.com/THUDM/SwissArmyTransformer
 Author: Ming Ding, et al.
 Author-email: dm_thu@qq.com
 License: Apache 2.0 license
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
```

### Comparing `SwissArmyTransformer-0.4.3/SwissArmyTransformer.egg-info/SOURCES.txt` & `SwissArmyTransformer-0.4.4/SwissArmyTransformer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/arguments.py` & `SwissArmyTransformer-0.4.4/sat/arguments.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/data_utils/configure_data.py` & `SwissArmyTransformer-0.4.4/sat/data_utils/configure_data.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/data_utils/datasets.py` & `SwissArmyTransformer-0.4.4/sat/data_utils/datasets.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/data_utils/hf_dataset.py` & `SwissArmyTransformer-0.4.4/sat/data_utils/hf_dataset.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/data_utils/samplers.py` & `SwissArmyTransformer-0.4.4/sat/data_utils/samplers.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/data_utils/webds.py` & `SwissArmyTransformer-0.4.4/sat/data_utils/webds.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,15 +147,15 @@
                 if '*' in include_dir:
                     include_dir, n = include_dir.split('*')
                     n = int(n)
                 else:
                     n = 1
                 for cur_dir, dirs, files in os.walk(include_dir):
                     for f in files:
-                        if f.endswith('tar'):
+                        if f.endswith('tar') and os.path.getsize(os.path.join(cur_dir,f)) > 0:
                             # other_paths.append(os.path.join(cur_dir,f))
                             other_paths.extend([os.path.join(cur_dir,f)]*n)
             # print(f'Adding dataset paths {",".join(other_paths)}')
             from braceexpand import braceexpand
             if len(path) > 0: # not "" 
                 path = list(braceexpand(path)) + other_paths
             else:
```

### Comparing `SwissArmyTransformer-0.4.3/sat/generation/autoregressive_sampling.py` & `SwissArmyTransformer-0.4.4/sat/generation/autoregressive_sampling.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
         # forward
         if log_attention_weights is not None:
             log_attention_weights_part = log_attention_weights[..., index: counter+1, :counter+1] # TODO memlen
         else:
             log_attention_weights_part = None
 
         logits, *output_per_layers = model(
-            tokens[:, index:], 
+            input_ids=tokens[:, index:], 
             position_ids=position_ids[..., index: counter+1],
             attention_mask=attention_mask[..., index: counter+1, :counter+1], # TODO memlen
             mems=mems,
             log_attention_weights=log_attention_weights_part,
             **kw_args
         )
         mem_kv = [o['mem_kv'] for o in output_per_layers]
```

### Comparing `SwissArmyTransformer-0.4.3/sat/generation/cuda2d_sampling.py` & `SwissArmyTransformer-0.4.4/sat/generation/cuda2d_sampling.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/generation/magnify.py` & `SwissArmyTransformer-0.4.4/sat/generation/magnify.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/generation/sampling_strategies/base_strategy.py` & `SwissArmyTransformer-0.4.4/sat/generation/sampling_strategies/base_strategy.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/generation/sampling_strategies/beam_search_strategy.py` & `SwissArmyTransformer-0.4.4/sat/generation/sampling_strategies/beam_search_strategy.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/generation/sampling_strategies/iterative_entfilter_strategy.py` & `SwissArmyTransformer-0.4.4/sat/generation/sampling_strategies/iterative_entfilter_strategy.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/generation/utils.py` & `SwissArmyTransformer-0.4.4/sat/generation/utils.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/helpers.py` & `SwissArmyTransformer-0.4.4/sat/helpers.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/model/attention/memory_efficient_attention.py` & `SwissArmyTransformer-0.4.4/sat/model/attention/memory_efficient_attention.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/model/base_model.py` & `SwissArmyTransformer-0.4.4/sat/model/base_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/model/cached_autoregressive_model.py` & `SwissArmyTransformer-0.4.4/sat/model/cached_autoregressive_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/model/encoder_decoder_model.py` & `SwissArmyTransformer-0.4.4/sat/model/encoder_decoder_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/model/finetune/adapter.py` & `SwissArmyTransformer-0.4.4/sat/model/finetune/adapter.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/model/finetune/ffadd.py` & `SwissArmyTransformer-0.4.4/sat/model/finetune/ffadd.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/model/finetune/lora.py` & `SwissArmyTransformer-0.4.4/sat/model/finetune/lora.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/model/finetune/lora2.py` & `SwissArmyTransformer-0.4.4/sat/model/finetune/lora2.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/model/finetune/mlp_head.py` & `SwissArmyTransformer-0.4.4/sat/model/finetune/mlp_head.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/model/finetune/prompt_tuning.py` & `SwissArmyTransformer-0.4.4/sat/model/finetune/prompt_tuning.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/model/normalization/rms.py` & `SwissArmyTransformer-0.4.4/sat/model/normalization/rms.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/model/official/__init__.py` & `SwissArmyTransformer-0.4.4/sat/model/official/__init__.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/model/official/bert_model.py` & `SwissArmyTransformer-0.4.4/sat/model/official/bert_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/model/official/cait_model.py` & `SwissArmyTransformer-0.4.4/sat/model/official/cait_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/model/official/chatglm2_model.py` & `SwissArmyTransformer-0.4.4/sat/model/official/chatglm2_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/model/official/chatglm_model.py` & `SwissArmyTransformer-0.4.4/sat/model/official/chatglm_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/model/official/clip_model.py` & `SwissArmyTransformer-0.4.4/sat/model/official/clip_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/model/official/cuda2d_model.py` & `SwissArmyTransformer-0.4.4/sat/model/official/cuda2d_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/model/official/distill_model.py` & `SwissArmyTransformer-0.4.4/sat/model/official/distill_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/model/official/dpr_model.py` & `SwissArmyTransformer-0.4.4/sat/model/official/dpr_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/model/official/eva2_model.py` & `SwissArmyTransformer-0.4.4/sat/model/official/eva2_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/model/official/glm130B_model.py` & `SwissArmyTransformer-0.4.4/sat/model/official/glm130B_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/model/official/glm_model.py` & `SwissArmyTransformer-0.4.4/sat/model/official/glm_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/model/official/gpt2_model.py` & `SwissArmyTransformer-0.4.4/sat/model/official/gpt2_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/model/official/gptneo_model.py` & `SwissArmyTransformer-0.4.4/sat/model/official/gptneo_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/model/official/llama_model.py` & `SwissArmyTransformer-0.4.4/sat/model/official/llama_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         attention_fn = attention_fn_default
         if 'attention_fn' in self.hooks:
             attention_fn = self.hooks['attention_fn']
 
         mixed_raw_layer = self.query_key_value(hidden_states)
         (mixed_query_layer,
             mixed_key_layer,
-            mixed_value_layer) = split_tensor_along_last_dim(mixed_raw_layer, 3)
+            mixed_value_layer) = split_tensor_along_last_dim(mixed_raw_layer, self.stride)
 
         dropout_fn = self.attention_dropout if self.training else None
 
         query_layer = self._transpose_for_scores(mixed_query_layer)
         key_layer = self._transpose_for_scores(mixed_key_layer)
         value_layer = self._transpose_for_scores(mixed_value_layer)
         cos, sin = origin.rotary_emb(value_layer, seq_len=kw_args['position_ids'].max()+1)
```

### Comparing `SwissArmyTransformer-0.4.3/sat/model/official/mae_model.py` & `SwissArmyTransformer-0.4.4/sat/model/official/mae_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/model/official/t5_model.py` & `SwissArmyTransformer-0.4.4/sat/model/official/t5_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/model/official/vit_model.py` & `SwissArmyTransformer-0.4.4/sat/model/official/vit_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/model/official/yolos_model.py` & `SwissArmyTransformer-0.4.4/sat/model/official/yolos_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/model/position_embedding/rotary_embeddings.py` & `SwissArmyTransformer-0.4.4/sat/model/position_embedding/rotary_embeddings.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/model/position_embedding/rotary_embeddings_original.py` & `SwissArmyTransformer-0.4.4/sat/model/position_embedding/rotary_embeddings_original.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/model/position_embedding/sincos2d.py` & `SwissArmyTransformer-0.4.4/sat/model/position_embedding/sincos2d.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/model/position_embedding/vision_rotary_embeddings.py` & `SwissArmyTransformer-0.4.4/sat/model/position_embedding/vision_rotary_embeddings.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/model/registry.py` & `SwissArmyTransformer-0.4.4/sat/model/registry.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/model/transformer.py` & `SwissArmyTransformer-0.4.4/sat/model/transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 import math
 import copy
 import torch
 import torch.nn.functional as F
 
 from sat import mpu
-from sat.mpu import get_model_parallel_world_size,ColumnParallelLinear, RowParallelLinear, VocabParallelEmbedding, gather_from_model_parallel_region, copy_to_model_parallel_region, checkpoint
+from sat.mpu import get_model_parallel_world_size, ColumnParallelLinear, RowParallelLinear, VocabParallelEmbedding, gather_from_model_parallel_region, copy_to_model_parallel_region, checkpoint
 
 
 from sat.mpu.utils import divide, sqrt, scaled_init_method, unscaled_init_method, gelu
 from sat.ops.layernorm import LayerNorm
 
 from sat.transformer_defaults import HOOKS_DEFAULT, standard_attention, split_tensor_along_last_dim
 
@@ -366,15 +366,15 @@
                  checkpoint_activations=False,
                  checkpoint_num_layers=1,
                  layernorm_epsilon=1.0e-5,
                  init_method_std=0.02,
                  inner_hidden_size=None,
                  hidden_size_per_attention_head=None,
                  layernorm_order='pre',
-                 parallel_output=True,
+                 parallel_output=False,
                  is_decoder=False,
                  cross_attn_hidden_size=None,
                  use_bias=True,
                  use_qkv_bias=False,
                  num_multi_query_heads=0,
                  activation_func=gelu,
                  layernorm=LayerNorm,
@@ -619,18 +619,15 @@
         if self.use_final_layernorm:
             logits = self.final_layernorm(hidden_states)
         else:
             logits = hidden_states
 
         logits = copy_to_model_parallel_region(logits)
         if 'final_forward' in self.hooks:
-            logits_parallel = self.hooks['final_forward'](logits, **kw_args)
+            logits_parallel = self.hooks['final_forward'](logits, **kw_args, parallel_output=self.parallel_output)
         else:
-            logits_parallel = HOOKS_DEFAULT['final_forward'](self, logits, **kw_args)
-
-        if not self.parallel_output:
-            logits_parallel = gather_from_model_parallel_region(logits_parallel)
+            logits_parallel = HOOKS_DEFAULT['final_forward'](self, logits, **kw_args, parallel_output=self.parallel_output)
 
         outputs = [logits_parallel]
         outputs.extend(output_per_layers)
         
         return outputs
```

### Comparing `SwissArmyTransformer-0.4.3/sat/mpu/__init__.py` & `SwissArmyTransformer-0.4.4/sat/mpu/__init__.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/mpu/cross_entropy.py` & `SwissArmyTransformer-0.4.4/sat/mpu/cross_entropy.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/mpu/data.py` & `SwissArmyTransformer-0.4.4/sat/mpu/data.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/mpu/initialize.py` & `SwissArmyTransformer-0.4.4/sat/mpu/initialize.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/mpu/layers.py` & `SwissArmyTransformer-0.4.4/sat/mpu/layers.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/mpu/mappings.py` & `SwissArmyTransformer-0.4.4/sat/mpu/mappings.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/mpu/operation.py` & `SwissArmyTransformer-0.4.4/sat/mpu/operation.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/mpu/utils.py` & `SwissArmyTransformer-0.4.4/sat/mpu/utils.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/ops/__init__.py` & `SwissArmyTransformer-0.4.4/sat/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/ops/csrc/adam/fused_ema_adam_frontend.cpp` & `SwissArmyTransformer-0.4.4/sat/ops/csrc/adam/fused_ema_adam_frontend.cpp`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/ops/csrc/adam/multi_tensor_apply.cuh` & `SwissArmyTransformer-0.4.4/sat/ops/csrc/adam/multi_tensor_apply.cuh`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/ops/csrc/adam/multi_tensor_ema_adam.cu` & `SwissArmyTransformer-0.4.4/sat/ops/csrc/adam/multi_tensor_ema_adam.cu`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/ops/csrc/includes/type_shim.h` & `SwissArmyTransformer-0.4.4/sat/ops/csrc/includes/type_shim.h`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/ops/fused_ema_adam.py` & `SwissArmyTransformer-0.4.4/sat/ops/fused_ema_adam.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/ops/layernorm.py` & `SwissArmyTransformer-0.4.4/sat/ops/layernorm.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/ops/local_attention_function.py` & `SwissArmyTransformer-0.4.4/sat/ops/local_attention_function.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/ops/memory_efficient_attention.py` & `SwissArmyTransformer-0.4.4/sat/ops/memory_efficient_attention.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/ops/ops_builder/__init__.py` & `SwissArmyTransformer-0.4.4/sat/ops/ops_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/ops/ops_builder/builder.py` & `SwissArmyTransformer-0.4.4/sat/ops/ops_builder/builder.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/ops/ops_builder/fused_ema_adam.py` & `SwissArmyTransformer-0.4.4/sat/ops/ops_builder/fused_ema_adam.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/quantization/kernels.py` & `SwissArmyTransformer-0.4.4/sat/quantization/kernels.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/resources/download.py` & `SwissArmyTransformer-0.4.4/sat/resources/download.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/resources/urls.py` & `SwissArmyTransformer-0.4.4/sat/resources/urls.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/tokenization/__init__.py` & `SwissArmyTransformer-0.4.4/sat/tokenization/__init__.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/tokenization/cogview/sp_tokenizer.py` & `SwissArmyTransformer-0.4.4/sat/tokenization/cogview/sp_tokenizer.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/tokenization/cogview/templates.py` & `SwissArmyTransformer-0.4.4/sat/tokenization/cogview/templates.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/tokenization/cogview/unified_tokenizer.py` & `SwissArmyTransformer-0.4.4/sat/tokenization/cogview/unified_tokenizer.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/tokenization/cogview/vqvae/api.py` & `SwissArmyTransformer-0.4.4/sat/tokenization/cogview/vqvae/api.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/tokenization/cogview/vqvae/vqvae_diffusion.py` & `SwissArmyTransformer-0.4.4/sat/tokenization/cogview/vqvae/vqvae_diffusion.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/tokenization/cogview/vqvae/vqvae_zc.py` & `SwissArmyTransformer-0.4.4/sat/tokenization/cogview/vqvae/vqvae_zc.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/tokenization/cogview/vqvae_tokenizer.py` & `SwissArmyTransformer-0.4.4/sat/tokenization/cogview/vqvae_tokenizer.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/tokenization/embed_assets/chinese_sentencepiece/cog-pretrain.model` & `SwissArmyTransformer-0.4.4/sat/tokenization/embed_assets/chinese_sentencepiece/cog-pretrain.model`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/tokenization/embed_assets/chinese_sentencepiece/cog-pretrain.vocab` & `SwissArmyTransformer-0.4.4/sat/tokenization/embed_assets/chinese_sentencepiece/cog-pretrain.vocab`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/tokenization/embed_assets/english_tokenizer/bert-base-uncased-vocab.txt` & `SwissArmyTransformer-0.4.4/sat/tokenization/embed_assets/english_tokenizer/bert-base-uncased-vocab.txt`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/tokenization/embed_assets/english_tokenizer/bert-large-uncased-vocab.txt` & `SwissArmyTransformer-0.4.4/sat/tokenization/embed_assets/english_tokenizer/bert-large-uncased-vocab.txt`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/tokenization/embed_assets/english_tokenizer/gpt2-merges.txt` & `SwissArmyTransformer-0.4.4/sat/tokenization/embed_assets/english_tokenizer/gpt2-merges.txt`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/tokenization/embed_assets/english_tokenizer/gpt2-vocab.json` & `SwissArmyTransformer-0.4.4/sat/tokenization/embed_assets/english_tokenizer/gpt2-vocab.json`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/tokenization/embed_assets/english_tokenizer/roberta-merges.txt` & `SwissArmyTransformer-0.4.4/sat/tokenization/embed_assets/english_tokenizer/roberta-merges.txt`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/tokenization/embed_assets/english_tokenizer/roberta-vocab.json` & `SwissArmyTransformer-0.4.4/sat/tokenization/embed_assets/english_tokenizer/roberta-vocab.json`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/tokenization/glm/sp_tokenizer.py` & `SwissArmyTransformer-0.4.4/sat/tokenization/glm/sp_tokenizer.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/tokenization/glm/tokenization.py` & `SwissArmyTransformer-0.4.4/sat/tokenization/glm/tokenization.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/tokenization/glm/tokenization_gpt2.py` & `SwissArmyTransformer-0.4.4/sat/tokenization/glm/tokenization_gpt2.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/tokenization/glm/tokenization_wordpiece.py` & `SwissArmyTransformer-0.4.4/sat/tokenization/glm/tokenization_wordpiece.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/tokenization/hf_tokenizer.py` & `SwissArmyTransformer-0.4.4/sat/tokenization/hf_tokenizer.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/tokenization/icetk_glm_130B/ice_tokenizer.py` & `SwissArmyTransformer-0.4.4/sat/tokenization/icetk_glm_130B/ice_tokenizer.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/tokenization/icetk_glm_130B/tokenizer.py` & `SwissArmyTransformer-0.4.4/sat/tokenization/icetk_glm_130B/tokenizer.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/training/deepspeed_training.py` & `SwissArmyTransformer-0.4.4/sat/training/deepspeed_training.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/training/deepspeed_zero1.json` & `SwissArmyTransformer-0.4.4/sat/training/deepspeed_zero1.json`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/training/deepspeed_zero2.json` & `SwissArmyTransformer-0.4.4/sat/training/deepspeed_zero2.json`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/training/learning_rates.py` & `SwissArmyTransformer-0.4.4/sat/training/learning_rates.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/training/model_io.py` & `SwissArmyTransformer-0.4.4/sat/training/model_io.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,15 @@
         if optimizer.optimizer.__class__.__name__ ==  "FusedEmaAdam" :
             update_ema_parameters_to_model(optimizer)
             if mpu.get_data_parallel_rank() == 0:
                 print_rank0('Saving Ema Model...')
                 save_ds_checkpoint(iteration, model, lr_scheduler, args, True)
     elif args.mode == 'inference':
         os.makedirs(os.path.join(args.save, str(iteration)), exist_ok=True)
-        torch.save({'module': model.state_dict()}, os.path.join(args.save, str(iteration), 'mp_rank_00_model_states.pt'))
+        torch.save({'module': model.state_dict()}, os.path.join(args.save, str(iteration), 'mp_rank_{:02d}_model_states.pt'.format(int(os.environ.get("RANK", 0)))))
     else:
         raise ValueError("training without deepspeed is not supported.")
     # Wait so everyone is done (necessary)
     torch.distributed.barrier()
     # And update the latest iteration
     if torch.distributed.get_rank() == 0:
         tracker_filename = get_checkpoint_tracker_filename(args.save)
```

### Comparing `SwissArmyTransformer-0.4.3/sat/training/utils.py` & `SwissArmyTransformer-0.4.4/sat/training/utils.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/sat/transformer_defaults.py` & `SwissArmyTransformer-0.4.4/sat/transformer_defaults.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     if int(torch.__version__.split('.')[0]) >= 2 and scaling_attention_score and (is_full or is_low_triangle):
         # Pytorch 2.0 attention uses very much memory if attention_mask is float, and has NaN bug if attention_mask is None.
         dropout_p = 0. if attention_dropout is None or not attention_dropout.training else attention_dropout.p
         return torch.nn.functional.scaled_dot_product_attention(
             query_layer, key_layer, value_layer, 
             attn_mask=None,
             dropout_p=dropout_p,
-            is_causal=is_low_triangle.item()
+            is_causal=not is_full
         )
     else:
         return standard_attention(
             query_layer, key_layer, value_layer, attention_mask,
             attention_dropout=attention_dropout, log_attention_weights=log_attention_weights,
             scaling_attention_score=scaling_attention_score, **kwargs
         )
@@ -136,16 +136,20 @@
 
 def word_embedding_forward_default(self, input_ids, output_cross_layer, **kw_args):
     return self.transformer.word_embeddings(input_ids)
 
 def position_embedding_forward_default(self, position_ids, output_cross_layer, **kw_args):
     return self.transformer.position_embeddings(position_ids)
 
+from sat.mpu import gather_from_model_parallel_region
 def final_forward_default(self, logits, **kw_args):
-    return F.linear(logits, self.transformer.word_embeddings.weight)
+    logits_parallel = F.linear(logits, self.transformer.word_embeddings.weight)
+    if not kw_args['parallel_output']:
+        logits_parallel = gather_from_model_parallel_region(logits_parallel)
+    return logits_parallel
 
 def layer_forward_default(self, hidden_states, mask, *args, **kw_args):
     '''
         hidden_states: [batch, seq_len, hidden_size]
         mask: [(1, 1), seq_len, seq_len]
     '''
     self = self.transformer.layers[kw_args['layer_id']]
```

### Comparing `SwissArmyTransformer-0.4.3/setup.py` & `SwissArmyTransformer-0.4.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 def _requirements():
     return Path("requirements.txt").read_text()
 
 setup(
     name="SwissArmyTransformer",
-    version='0.4.3',
+    version='0.4.4',
     description="A transformer-based framework with finetuning as the first class citizen.",
     long_description=Path("README.md").read_text(),
     long_description_content_type="text/markdown",
     install_requires=_requirements(),
     entry_points={},
     packages=find_packages(),
     url="https://github.com/THUDM/SwissArmyTransformer",
```

### Comparing `SwissArmyTransformer-0.4.3/tests/test_base_model.py` & `SwissArmyTransformer-0.4.4/tests/test_base_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/tests/test_inference.py` & `SwissArmyTransformer-0.4.4/tests/test_inference.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/tests/test_mea.py` & `SwissArmyTransformer-0.4.4/tests/test_mea.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/tests/test_model_parallel.py` & `SwissArmyTransformer-0.4.4/tests/test_model_parallel.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/tests/test_nested_model.py` & `SwissArmyTransformer-0.4.4/tests/test_nested_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/tests/test_speed.py` & `SwissArmyTransformer-0.4.4/tests/test_speed.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/tests/test_train.py` & `SwissArmyTransformer-0.4.4/tests/test_train.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/tests/test_train_dp.py` & `SwissArmyTransformer-0.4.4/tests/test_train_dp.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.4.3/tests/test_train_nested.py` & `SwissArmyTransformer-0.4.4/tests/test_train_nested.py`

 * *Files identical despite different names*

