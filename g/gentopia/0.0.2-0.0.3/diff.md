# Comparing `tmp/gentopia-0.0.2.tar.gz` & `tmp/gentopia-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gentopia-0.0.2.tar", last modified: Tue Aug  1 23:57:35 2023, max compression
+gzip compressed data, was "gentopia-0.0.3.tar", last modified: Mon Aug  7 01:37:05 2023, max compression
```

## Comparing `gentopia-0.0.2.tar` & `gentopia-0.0.3.tar`

### file list

```diff
@@ -1,161 +1,163 @@
-drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-01 23:57:35.802369 gentopia-0.0.2/
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     1067 2023-07-29 06:32:27.000000 gentopia-0.0.2/LICENSE
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     7234 2023-08-01 23:57:35.802369 gentopia-0.0.2/PKG-INFO
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     6881 2023-08-01 23:57:15.000000 gentopia-0.0.2/README.md
-drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-01 23:57:35.786369 gentopia-0.0.2/gentopia/
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      970 2023-07-15 05:02:37.000000 gentopia-0.0.2/gentopia/__init__.py
-drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-01 23:57:35.786369 gentopia-0.0.2/gentopia/agent/
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)       33 2023-07-03 16:27:20.000000 gentopia-0.0.2/gentopia/agent/__init__.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     3490 2023-07-27 03:27:55.000000 gentopia-0.0.2/gentopia/agent/base_agent.py
-drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-01 23:57:35.786369 gentopia-0.0.2/gentopia/agent/openai/
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)       42 2023-06-22 05:41:38.000000 gentopia-0.0.2/gentopia/agent/openai/__init__.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     9156 2023-07-27 03:27:55.000000 gentopia-0.0.2/gentopia/agent/openai/agent.py
-drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-01 23:57:35.786369 gentopia-0.0.2/gentopia/agent/openai_memory/
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)       40 2023-07-10 23:23:40.000000 gentopia-0.0.2/gentopia/agent/openai_memory/__init__.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)    10125 2023-07-27 03:27:55.000000 gentopia-0.0.2/gentopia/agent/openai_memory/agent.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     1195 2023-07-15 14:57:36.000000 gentopia-0.0.2/gentopia/agent/openai_memory/load_memory.py
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     1353 2023-07-27 03:24:25.000000 gentopia-0.0.2/gentopia/agent/plugin_manager.py
-drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-01 23:57:35.786369 gentopia-0.0.2/gentopia/agent/react/
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)       30 2023-06-16 00:45:03.000000 gentopia-0.0.2/gentopia/agent/react/__init__.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     9794 2023-07-27 03:27:55.000000 gentopia-0.0.2/gentopia/agent/react/agent.py
-drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-01 23:57:35.786369 gentopia-0.0.2/gentopia/agent/rewoo/
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)       30 2023-06-16 00:45:03.000000 gentopia-0.0.2/gentopia/agent/rewoo/__init__.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)    14079 2023-07-27 03:25:32.000000 gentopia-0.0.2/gentopia/agent/rewoo/agent.py
-drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-01 23:57:35.790369 gentopia-0.0.2/gentopia/agent/rewoo/nodes/
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     3270 2023-07-08 05:17:15.000000 gentopia-0.0.2/gentopia/agent/rewoo/nodes/Planner.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     2677 2023-07-08 05:17:15.000000 gentopia-0.0.2/gentopia/agent/rewoo/nodes/Solver.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)        0 2023-06-13 13:12:30.000000 gentopia-0.0.2/gentopia/agent/rewoo/nodes/__init__.py
-drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-01 23:57:35.790369 gentopia-0.0.2/gentopia/agent/vanilla/
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)       32 2023-06-16 00:45:03.000000 gentopia-0.0.2/gentopia/agent/vanilla/__init__.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     5055 2023-07-15 14:57:36.000000 gentopia-0.0.2/gentopia/agent/vanilla/agent.py
-drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-01 23:57:35.790369 gentopia-0.0.2/gentopia/assembler/
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)       30 2023-07-06 14:53:35.000000 gentopia-0.0.2/gentopia/assembler/__init__.py
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     9849 2023-07-23 00:45:38.000000 gentopia-0.0.2/gentopia/assembler/agent_assembler.py
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     2637 2023-07-23 00:45:38.000000 gentopia-0.0.2/gentopia/assembler/config.py
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     4069 2023-07-15 14:57:36.000000 gentopia-0.0.2/gentopia/assembler/loader.py
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)      671 2023-07-15 14:57:36.000000 gentopia-0.0.2/gentopia/assembler/task.py
-drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-01 23:57:35.790369 gentopia-0.0.2/gentopia/llm/
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      169 2023-07-23 00:45:38.000000 gentopia-0.0.2/gentopia/llm/__init__.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      771 2023-06-21 06:58:48.000000 gentopia-0.0.2/gentopia/llm/base_llm.py
-drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-01 23:57:35.790369 gentopia-0.0.2/gentopia/llm/client/
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      155 2023-07-23 00:45:38.000000 gentopia-0.0.2/gentopia/llm/client/__init__.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)    10652 2023-07-23 00:45:38.000000 gentopia-0.0.2/gentopia/llm/client/huggingface.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)    12848 2023-07-15 14:57:36.000000 gentopia-0.0.2/gentopia/llm/client/openai.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     2347 2023-07-15 14:57:36.000000 gentopia-0.0.2/gentopia/llm/llm_info.py
-drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-01 23:57:35.794369 gentopia-0.0.2/gentopia/llm/loaders/
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)        0 2023-06-16 14:36:29.000000 gentopia-0.0.2/gentopia/llm/loaders/__init__.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      550 2023-06-20 04:55:33.000000 gentopia-0.0.2/gentopia/llm/loaders/airoboros.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      943 2023-06-16 14:36:29.000000 gentopia-0.0.2/gentopia/llm/loaders/alpaca.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      943 2023-06-16 14:36:29.000000 gentopia-0.0.2/gentopia/llm/loaders/baize.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      882 2023-06-16 14:36:29.000000 gentopia-0.0.2/gentopia/llm/loaders/bloom.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      585 2023-06-16 14:36:29.000000 gentopia-0.0.2/gentopia/llm/loaders/camel.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      519 2023-06-16 14:36:29.000000 gentopia-0.0.2/gentopia/llm/loaders/falcon.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      732 2023-06-16 14:36:29.000000 gentopia-0.0.2/gentopia/llm/loaders/flan_alpaca.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      951 2023-06-16 14:36:29.000000 gentopia-0.0.2/gentopia/llm/loaders/guanaco.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      446 2023-06-16 14:36:29.000000 gentopia-0.0.2/gentopia/llm/loaders/kullm.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      545 2023-06-16 14:36:29.000000 gentopia-0.0.2/gentopia/llm/loaders/mpt.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      545 2023-06-16 14:36:29.000000 gentopia-0.0.2/gentopia/llm/loaders/redpajama.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     1019 2023-06-16 14:36:29.000000 gentopia-0.0.2/gentopia/llm/loaders/replit.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      549 2023-06-16 14:36:29.000000 gentopia-0.0.2/gentopia/llm/loaders/samantha_vicuna.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      647 2023-06-16 14:36:29.000000 gentopia-0.0.2/gentopia/llm/loaders/stablelm.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      482 2023-06-16 14:36:29.000000 gentopia-0.0.2/gentopia/llm/loaders/starchat.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      599 2023-06-16 14:36:29.000000 gentopia-0.0.2/gentopia/llm/loaders/t5_vicuna.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      689 2023-06-16 14:36:29.000000 gentopia-0.0.2/gentopia/llm/loaders/vicuna.py
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)      762 2023-06-20 04:55:33.000000 gentopia-0.0.2/gentopia/llm/test_llm.py
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     1837 2023-07-08 05:17:15.000000 gentopia-0.0.2/gentopia/llm/wrap_llm.py
-drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-01 23:57:35.794369 gentopia-0.0.2/gentopia/manager/
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-06-20 04:55:33.000000 gentopia-0.0.2/gentopia/manager/__init__.py
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)      853 2023-06-20 04:55:33.000000 gentopia-0.0.2/gentopia/manager/base_llm_manager.py
-drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-01 23:57:35.794369 gentopia-0.0.2/gentopia/manager/llm_client/
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-06-20 04:55:33.000000 gentopia-0.0.2/gentopia/manager/llm_client/__init__.py
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)      559 2023-06-20 04:55:33.000000 gentopia-0.0.2/gentopia/manager/llm_client/base_llm_client.py
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     1784 2023-06-20 04:55:33.000000 gentopia-0.0.2/gentopia/manager/llm_client/local_llm_client.py
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     3418 2023-06-20 04:55:33.000000 gentopia-0.0.2/gentopia/manager/local_llm_manager.py
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)      359 2023-06-20 04:55:33.000000 gentopia-0.0.2/gentopia/manager/server_info.py
-drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-01 23:57:35.794369 gentopia-0.0.2/gentopia/memory/
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)        0 2023-07-10 23:23:40.000000 gentopia-0.0.2/gentopia/memory/__init__.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     8872 2023-07-23 00:45:38.000000 gentopia-0.0.2/gentopia/memory/api.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     1323 2023-07-23 00:45:38.000000 gentopia-0.0.2/gentopia/memory/base_memory.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      238 2023-07-10 23:23:40.000000 gentopia-0.0.2/gentopia/memory/document.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)    17492 2023-07-23 00:45:38.000000 gentopia-0.0.2/gentopia/memory/embeddings.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     5492 2023-07-23 00:45:38.000000 gentopia-0.0.2/gentopia/memory/serializable.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     5236 2023-07-23 00:45:38.000000 gentopia-0.0.2/gentopia/memory/utils.py
-drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-01 23:57:35.794369 gentopia-0.0.2/gentopia/memory/vectorstores/
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)        0 2023-07-27 06:32:36.000000 gentopia-0.0.2/gentopia/memory/vectorstores/__init__.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)    15210 2023-07-23 00:45:38.000000 gentopia-0.0.2/gentopia/memory/vectorstores/chroma.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)    14915 2023-07-23 00:45:38.000000 gentopia-0.0.2/gentopia/memory/vectorstores/pinecone.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)    29000 2023-07-23 00:45:38.000000 gentopia-0.0.2/gentopia/memory/vectorstores/vectorstore.py
-drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-01 23:57:35.794369 gentopia-0.0.2/gentopia/model/
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)       85 2023-07-03 16:27:20.000000 gentopia-0.0.2/gentopia/model/__init__.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     1436 2023-07-10 23:23:40.000000 gentopia-0.0.2/gentopia/model/agent_model.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      715 2023-07-06 14:53:35.000000 gentopia-0.0.2/gentopia/model/completion_model.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     1658 2023-07-23 00:45:38.000000 gentopia-0.0.2/gentopia/model/param_model.py
-drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-01 23:57:35.794369 gentopia-0.0.2/gentopia/output/
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)      967 2023-07-23 00:45:38.000000 gentopia-0.0.2/gentopia/output/__init__.py
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     6529 2023-07-15 14:57:33.000000 gentopia-0.0.2/gentopia/output/base_output.py
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     5513 2023-07-15 14:57:33.000000 gentopia-0.0.2/gentopia/output/console_output.py
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     3383 2023-07-15 14:57:33.000000 gentopia-0.0.2/gentopia/output/print_output.py
-drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-01 23:57:35.798370 gentopia-0.0.2/gentopia/prompt/
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      128 2023-07-27 03:40:32.000000 gentopia-0.0.2/gentopia/prompt/__init__.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     1341 2023-07-27 05:33:19.000000 gentopia-0.0.2/gentopia/prompt/prompt_template.py
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)      824 2023-07-27 03:40:32.000000 gentopia-0.0.2/gentopia/prompt/react.py
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     3720 2023-07-27 03:40:32.000000 gentopia-0.0.2/gentopia/prompt/rewoo.py
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)      198 2023-07-12 12:18:52.000000 gentopia-0.0.2/gentopia/prompt/tmp.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      286 2023-07-15 14:57:36.000000 gentopia-0.0.2/gentopia/prompt/vanilla.py
-drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-01 23:57:35.798370 gentopia-0.0.2/gentopia/resource/
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)        0 2023-06-16 14:36:29.000000 gentopia-0.0.2/gentopia/resource/__init__.py
-drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-01 23:57:35.798370 gentopia-0.0.2/gentopia/tools/
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     1289 2023-07-27 03:27:55.000000 gentopia-0.0.2/gentopia/tools/__init__.py
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     1665 2023-07-27 03:27:55.000000 gentopia-0.0.2/gentopia/tools/arxiv_search.py
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     9037 2023-07-23 00:45:38.000000 gentopia-0.0.2/gentopia/tools/basetool.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     5998 2023-07-27 03:40:32.000000 gentopia-0.0.2/gentopia/tools/bing_search.py
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     1488 2023-07-27 03:27:55.000000 gentopia-0.0.2/gentopia/tools/calculator.py
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     1743 2023-07-27 03:27:55.000000 gentopia-0.0.2/gentopia/tools/code_interpreter.py
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     1902 2023-07-27 03:27:55.000000 gentopia-0.0.2/gentopia/tools/file_operation.py
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)      855 2023-07-27 03:27:55.000000 gentopia-0.0.2/gentopia/tools/google_search.py
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     3542 2023-07-27 03:27:55.000000 gentopia-0.0.2/gentopia/tools/gradio.py
-drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-01 23:57:35.798370 gentopia-0.0.2/gentopia/tools/gradio_tools/
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)        0 2023-07-01 23:00:56.000000 gentopia-0.0.2/gentopia/tools/gradio_tools/__init__.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     2155 2023-07-12 12:18:52.000000 gentopia-0.0.2/gentopia/tools/gradio_tools/api.py
-drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-01 23:57:35.798370 gentopia-0.0.2/gentopia/tools/gradio_tools/tools/
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     1244 2023-07-12 12:18:52.000000 gentopia-0.0.2/gentopia/tools/gradio_tools/tools/__init__.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     3514 2023-07-15 14:57:33.000000 gentopia-0.0.2/gentopia/tools/gradio_tools/tools/bark.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     1074 2023-07-12 12:18:52.000000 gentopia-0.0.2/gentopia/tools/gradio_tools/tools/clip_interrogator.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     1152 2023-07-12 12:18:52.000000 gentopia-0.0.2/gentopia/tools/gradio_tools/tools/document_qa.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     3326 2023-07-23 00:45:38.000000 gentopia-0.0.2/gentopia/tools/gradio_tools/tools/gradio_tool.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     1138 2023-07-12 12:18:52.000000 gentopia-0.0.2/gentopia/tools/gradio_tools/tools/image_captioning.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     1187 2023-07-12 12:18:52.000000 gentopia-0.0.2/gentopia/tools/gradio_tools/tools/image_to_music.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     1028 2023-07-12 12:18:52.000000 gentopia-0.0.2/gentopia/tools/gradio_tools/tools/prompt_generator.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     2352 2023-07-12 12:18:52.000000 gentopia-0.0.2/gentopia/tools/gradio_tools/tools/sam_with_clip.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     1371 2023-07-12 12:18:52.000000 gentopia-0.0.2/gentopia/tools/gradio_tools/tools/stable_diffusion.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     1021 2023-07-12 12:18:52.000000 gentopia-0.0.2/gentopia/tools/gradio_tools/tools/text_to_video.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     1037 2023-07-12 12:18:52.000000 gentopia-0.0.2/gentopia/tools/gradio_tools/tools/whisper.py
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     1100 2023-07-27 03:27:55.000000 gentopia-0.0.2/gentopia/tools/search_doc.py
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     4952 2023-07-27 03:27:55.000000 gentopia-0.0.2/gentopia/tools/shell.py
-drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-01 23:57:35.798370 gentopia-0.0.2/gentopia/tools/utils/
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)       23 2023-07-13 14:37:51.000000 gentopia-0.0.2/gentopia/tools/utils/__init__.py
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     2355 2023-07-13 14:37:51.000000 gentopia-0.0.2/gentopia/tools/utils/docstore.py
-drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-01 23:57:35.802369 gentopia-0.0.2/gentopia/tools/utils/document_loaders/
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-07-23 00:45:38.000000 gentopia-0.0.2/gentopia/tools/utils/document_loaders/__init__.py
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     1639 2023-07-23 00:45:38.000000 gentopia-0.0.2/gentopia/tools/utils/document_loaders/base_loader.py
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)      737 2023-07-23 00:45:38.000000 gentopia-0.0.2/gentopia/tools/utils/document_loaders/text_loader.py
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)    16131 2023-07-23 00:45:38.000000 gentopia-0.0.2/gentopia/tools/utils/document_loaders/text_splitter.py
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     1579 2023-07-23 00:45:38.000000 gentopia-0.0.2/gentopia/tools/utils/vector_store.py
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     6101 2023-07-27 03:27:55.000000 gentopia-0.0.2/gentopia/tools/weather.py
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     1298 2023-07-27 03:27:55.000000 gentopia-0.0.2/gentopia/tools/web_page.py
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     2316 2023-07-27 03:27:55.000000 gentopia-0.0.2/gentopia/tools/wikipedia.py
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     1482 2023-07-27 03:27:55.000000 gentopia-0.0.2/gentopia/tools/wolfram_alpha.py
-drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-01 23:57:35.802369 gentopia-0.0.2/gentopia/utils/
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-06-24 07:59:31.000000 gentopia-0.0.2/gentopia/utils/__init__.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      688 2023-07-23 00:45:38.000000 gentopia-0.0.2/gentopia/utils/cost_helpers.py
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-06-24 07:59:31.000000 gentopia-0.0.2/gentopia/utils/display_utils.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      878 2023-07-23 00:45:38.000000 gentopia-0.0.2/gentopia/utils/text_helpers.py
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     1690 2023-07-27 03:40:32.000000 gentopia-0.0.2/gentopia/utils/util.py
-drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-01 23:57:35.786369 gentopia-0.0.2/gentopia.egg-info/
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     7234 2023-08-01 23:57:35.000000 gentopia-0.0.2/gentopia.egg-info/PKG-INFO
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     4390 2023-08-01 23:57:35.000000 gentopia-0.0.2/gentopia.egg-info/SOURCES.txt
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)        1 2023-08-01 23:57:35.000000 gentopia-0.0.2/gentopia.egg-info/dependency_links.txt
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      308 2023-08-01 23:57:35.000000 gentopia-0.0.2/gentopia.egg-info/requires.txt
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)        9 2023-08-01 23:57:35.000000 gentopia-0.0.2/gentopia.egg-info/top_level.txt
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)       38 2023-08-01 23:57:35.802369 gentopia-0.0.2/setup.cfg
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     1190 2023-08-01 23:56:55.000000 gentopia-0.0.2/setup.py
+drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-07 01:37:05.111283 gentopia-0.0.3/
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     1067 2023-07-29 06:32:27.000000 gentopia-0.0.3/LICENSE
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     7251 2023-08-07 01:37:05.111283 gentopia-0.0.3/PKG-INFO
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     6898 2023-08-07 01:36:17.000000 gentopia-0.0.3/README.md
+drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-07 01:37:05.099283 gentopia-0.0.3/gentopia/
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      970 2023-07-15 05:02:37.000000 gentopia-0.0.3/gentopia/__init__.py
+drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-07 01:37:05.099283 gentopia-0.0.3/gentopia/agent/
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)       33 2023-07-03 16:27:20.000000 gentopia-0.0.3/gentopia/agent/__init__.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     3490 2023-07-27 03:27:55.000000 gentopia-0.0.3/gentopia/agent/base_agent.py
+drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-07 01:37:05.099283 gentopia-0.0.3/gentopia/agent/openai/
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)       42 2023-06-22 05:41:38.000000 gentopia-0.0.3/gentopia/agent/openai/__init__.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     9156 2023-07-27 03:27:55.000000 gentopia-0.0.3/gentopia/agent/openai/agent.py
+drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-07 01:37:05.099283 gentopia-0.0.3/gentopia/agent/openai_memory/
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)       40 2023-07-10 23:23:40.000000 gentopia-0.0.3/gentopia/agent/openai_memory/__init__.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)    10125 2023-07-27 03:27:55.000000 gentopia-0.0.3/gentopia/agent/openai_memory/agent.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     1195 2023-07-15 14:57:36.000000 gentopia-0.0.3/gentopia/agent/openai_memory/load_memory.py
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     1353 2023-07-27 03:24:25.000000 gentopia-0.0.3/gentopia/agent/plugin_manager.py
+drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-07 01:37:05.099283 gentopia-0.0.3/gentopia/agent/react/
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)       30 2023-06-16 00:45:03.000000 gentopia-0.0.3/gentopia/agent/react/__init__.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     9794 2023-07-27 03:27:55.000000 gentopia-0.0.3/gentopia/agent/react/agent.py
+drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-07 01:37:05.099283 gentopia-0.0.3/gentopia/agent/rewoo/
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)       30 2023-06-16 00:45:03.000000 gentopia-0.0.3/gentopia/agent/rewoo/__init__.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)    14079 2023-07-27 03:25:32.000000 gentopia-0.0.3/gentopia/agent/rewoo/agent.py
+drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-07 01:37:05.099283 gentopia-0.0.3/gentopia/agent/rewoo/nodes/
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     3270 2023-07-08 05:17:15.000000 gentopia-0.0.3/gentopia/agent/rewoo/nodes/Planner.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     2677 2023-07-08 05:17:15.000000 gentopia-0.0.3/gentopia/agent/rewoo/nodes/Solver.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)        0 2023-06-13 13:12:30.000000 gentopia-0.0.3/gentopia/agent/rewoo/nodes/__init__.py
+drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-07 01:37:05.099283 gentopia-0.0.3/gentopia/agent/vanilla/
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)       32 2023-06-16 00:45:03.000000 gentopia-0.0.3/gentopia/agent/vanilla/__init__.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     5055 2023-07-15 14:57:36.000000 gentopia-0.0.3/gentopia/agent/vanilla/agent.py
+drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-07 01:37:05.099283 gentopia-0.0.3/gentopia/assembler/
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)       30 2023-07-06 14:53:35.000000 gentopia-0.0.3/gentopia/assembler/__init__.py
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     9849 2023-07-23 00:45:38.000000 gentopia-0.0.3/gentopia/assembler/agent_assembler.py
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     2637 2023-07-23 00:45:38.000000 gentopia-0.0.3/gentopia/assembler/config.py
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     4069 2023-07-15 14:57:36.000000 gentopia-0.0.3/gentopia/assembler/loader.py
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)      671 2023-07-15 14:57:36.000000 gentopia-0.0.3/gentopia/assembler/task.py
+drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-07 01:37:05.103283 gentopia-0.0.3/gentopia/llm/
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      169 2023-07-23 00:45:38.000000 gentopia-0.0.3/gentopia/llm/__init__.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      771 2023-06-21 06:58:48.000000 gentopia-0.0.3/gentopia/llm/base_llm.py
+drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-07 01:37:05.103283 gentopia-0.0.3/gentopia/llm/client/
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      155 2023-07-23 00:45:38.000000 gentopia-0.0.3/gentopia/llm/client/__init__.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)    10652 2023-07-23 00:45:38.000000 gentopia-0.0.3/gentopia/llm/client/huggingface.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)    12848 2023-07-15 14:57:36.000000 gentopia-0.0.3/gentopia/llm/client/openai.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     2347 2023-07-15 14:57:36.000000 gentopia-0.0.3/gentopia/llm/llm_info.py
+drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-07 01:37:05.103283 gentopia-0.0.3/gentopia/llm/loaders/
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)        0 2023-06-16 14:36:29.000000 gentopia-0.0.3/gentopia/llm/loaders/__init__.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      550 2023-06-20 04:55:33.000000 gentopia-0.0.3/gentopia/llm/loaders/airoboros.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      943 2023-06-16 14:36:29.000000 gentopia-0.0.3/gentopia/llm/loaders/alpaca.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      943 2023-06-16 14:36:29.000000 gentopia-0.0.3/gentopia/llm/loaders/baize.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      882 2023-06-16 14:36:29.000000 gentopia-0.0.3/gentopia/llm/loaders/bloom.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      585 2023-06-16 14:36:29.000000 gentopia-0.0.3/gentopia/llm/loaders/camel.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      519 2023-06-16 14:36:29.000000 gentopia-0.0.3/gentopia/llm/loaders/falcon.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      732 2023-06-16 14:36:29.000000 gentopia-0.0.3/gentopia/llm/loaders/flan_alpaca.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      951 2023-06-16 14:36:29.000000 gentopia-0.0.3/gentopia/llm/loaders/guanaco.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      446 2023-06-16 14:36:29.000000 gentopia-0.0.3/gentopia/llm/loaders/kullm.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      545 2023-06-16 14:36:29.000000 gentopia-0.0.3/gentopia/llm/loaders/mpt.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      545 2023-06-16 14:36:29.000000 gentopia-0.0.3/gentopia/llm/loaders/redpajama.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     1019 2023-06-16 14:36:29.000000 gentopia-0.0.3/gentopia/llm/loaders/replit.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      549 2023-06-16 14:36:29.000000 gentopia-0.0.3/gentopia/llm/loaders/samantha_vicuna.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      647 2023-06-16 14:36:29.000000 gentopia-0.0.3/gentopia/llm/loaders/stablelm.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      482 2023-06-16 14:36:29.000000 gentopia-0.0.3/gentopia/llm/loaders/starchat.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      599 2023-06-16 14:36:29.000000 gentopia-0.0.3/gentopia/llm/loaders/t5_vicuna.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      689 2023-06-16 14:36:29.000000 gentopia-0.0.3/gentopia/llm/loaders/vicuna.py
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)      762 2023-06-20 04:55:33.000000 gentopia-0.0.3/gentopia/llm/test_llm.py
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     1837 2023-07-08 05:17:15.000000 gentopia-0.0.3/gentopia/llm/wrap_llm.py
+drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-07 01:37:05.103283 gentopia-0.0.3/gentopia/manager/
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-06-20 04:55:33.000000 gentopia-0.0.3/gentopia/manager/__init__.py
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)      853 2023-06-20 04:55:33.000000 gentopia-0.0.3/gentopia/manager/base_llm_manager.py
+drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-07 01:37:05.103283 gentopia-0.0.3/gentopia/manager/llm_client/
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-06-20 04:55:33.000000 gentopia-0.0.3/gentopia/manager/llm_client/__init__.py
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)      559 2023-06-20 04:55:33.000000 gentopia-0.0.3/gentopia/manager/llm_client/base_llm_client.py
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     1784 2023-06-20 04:55:33.000000 gentopia-0.0.3/gentopia/manager/llm_client/local_llm_client.py
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     3418 2023-06-20 04:55:33.000000 gentopia-0.0.3/gentopia/manager/local_llm_manager.py
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)      359 2023-06-20 04:55:33.000000 gentopia-0.0.3/gentopia/manager/server_info.py
+drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-07 01:37:05.107283 gentopia-0.0.3/gentopia/memory/
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)        0 2023-07-10 23:23:40.000000 gentopia-0.0.3/gentopia/memory/__init__.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     8872 2023-07-23 00:45:38.000000 gentopia-0.0.3/gentopia/memory/api.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     1323 2023-07-23 00:45:38.000000 gentopia-0.0.3/gentopia/memory/base_memory.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      238 2023-07-10 23:23:40.000000 gentopia-0.0.3/gentopia/memory/document.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)    17492 2023-07-23 00:45:38.000000 gentopia-0.0.3/gentopia/memory/embeddings.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     5492 2023-07-23 00:45:38.000000 gentopia-0.0.3/gentopia/memory/serializable.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     5236 2023-07-23 00:45:38.000000 gentopia-0.0.3/gentopia/memory/utils.py
+drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-07 01:37:05.107283 gentopia-0.0.3/gentopia/memory/vectorstores/
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)        0 2023-07-27 06:32:36.000000 gentopia-0.0.3/gentopia/memory/vectorstores/__init__.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)    15210 2023-07-23 00:45:38.000000 gentopia-0.0.3/gentopia/memory/vectorstores/chroma.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)    14915 2023-07-23 00:45:38.000000 gentopia-0.0.3/gentopia/memory/vectorstores/pinecone.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)    29000 2023-07-23 00:45:38.000000 gentopia-0.0.3/gentopia/memory/vectorstores/vectorstore.py
+drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-07 01:37:05.107283 gentopia-0.0.3/gentopia/model/
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)       85 2023-07-03 16:27:20.000000 gentopia-0.0.3/gentopia/model/__init__.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     1436 2023-07-10 23:23:40.000000 gentopia-0.0.3/gentopia/model/agent_model.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      715 2023-07-06 14:53:35.000000 gentopia-0.0.3/gentopia/model/completion_model.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     1658 2023-07-23 00:45:38.000000 gentopia-0.0.3/gentopia/model/param_model.py
+drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-07 01:37:05.107283 gentopia-0.0.3/gentopia/output/
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)      967 2023-07-23 00:45:38.000000 gentopia-0.0.3/gentopia/output/__init__.py
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     6641 2023-08-07 01:36:17.000000 gentopia-0.0.3/gentopia/output/base_output.py
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     5513 2023-07-15 14:57:33.000000 gentopia-0.0.3/gentopia/output/console_output.py
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     3383 2023-07-15 14:57:33.000000 gentopia-0.0.3/gentopia/output/print_output.py
+drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-07 01:37:05.107283 gentopia-0.0.3/gentopia/prompt/
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      128 2023-07-27 03:40:32.000000 gentopia-0.0.3/gentopia/prompt/__init__.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     1341 2023-07-27 05:33:19.000000 gentopia-0.0.3/gentopia/prompt/prompt_template.py
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)      824 2023-07-27 03:40:32.000000 gentopia-0.0.3/gentopia/prompt/react.py
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     3720 2023-07-27 03:40:32.000000 gentopia-0.0.3/gentopia/prompt/rewoo.py
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)      198 2023-07-12 12:18:52.000000 gentopia-0.0.3/gentopia/prompt/tmp.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      286 2023-07-15 14:57:36.000000 gentopia-0.0.3/gentopia/prompt/vanilla.py
+drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-07 01:37:05.107283 gentopia-0.0.3/gentopia/resource/
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)        0 2023-06-16 14:36:29.000000 gentopia-0.0.3/gentopia/resource/__init__.py
+drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-07 01:37:05.107283 gentopia-0.0.3/gentopia/tools/
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     1684 2023-08-07 01:36:17.000000 gentopia-0.0.3/gentopia/tools/__init__.py
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     1665 2023-07-27 03:27:55.000000 gentopia-0.0.3/gentopia/tools/arxiv_search.py
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     9037 2023-07-23 00:45:38.000000 gentopia-0.0.3/gentopia/tools/basetool.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     5998 2023-07-27 03:40:32.000000 gentopia-0.0.3/gentopia/tools/bing_search.py
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     1488 2023-07-27 03:27:55.000000 gentopia-0.0.3/gentopia/tools/calculator.py
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     1743 2023-07-27 03:27:55.000000 gentopia-0.0.3/gentopia/tools/code_interpreter.py
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     1517 2023-08-07 01:36:17.000000 gentopia-0.0.3/gentopia/tools/duckduckgo.py
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     1902 2023-07-27 03:27:55.000000 gentopia-0.0.3/gentopia/tools/file_operation.py
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)    10275 2023-08-07 01:36:17.000000 gentopia-0.0.3/gentopia/tools/google_scholar.py
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)      855 2023-07-27 03:27:55.000000 gentopia-0.0.3/gentopia/tools/google_search.py
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     3542 2023-07-27 03:27:55.000000 gentopia-0.0.3/gentopia/tools/gradio.py
+drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-07 01:37:05.107283 gentopia-0.0.3/gentopia/tools/gradio_tools/
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)        0 2023-07-01 23:00:56.000000 gentopia-0.0.3/gentopia/tools/gradio_tools/__init__.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     2155 2023-07-12 12:18:52.000000 gentopia-0.0.3/gentopia/tools/gradio_tools/api.py
+drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-07 01:37:05.111283 gentopia-0.0.3/gentopia/tools/gradio_tools/tools/
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     1244 2023-07-12 12:18:52.000000 gentopia-0.0.3/gentopia/tools/gradio_tools/tools/__init__.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     3514 2023-07-15 14:57:33.000000 gentopia-0.0.3/gentopia/tools/gradio_tools/tools/bark.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     1074 2023-07-12 12:18:52.000000 gentopia-0.0.3/gentopia/tools/gradio_tools/tools/clip_interrogator.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     1152 2023-07-12 12:18:52.000000 gentopia-0.0.3/gentopia/tools/gradio_tools/tools/document_qa.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     3326 2023-07-23 00:45:38.000000 gentopia-0.0.3/gentopia/tools/gradio_tools/tools/gradio_tool.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     1138 2023-07-12 12:18:52.000000 gentopia-0.0.3/gentopia/tools/gradio_tools/tools/image_captioning.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     1187 2023-07-12 12:18:52.000000 gentopia-0.0.3/gentopia/tools/gradio_tools/tools/image_to_music.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     1028 2023-07-12 12:18:52.000000 gentopia-0.0.3/gentopia/tools/gradio_tools/tools/prompt_generator.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     2352 2023-07-12 12:18:52.000000 gentopia-0.0.3/gentopia/tools/gradio_tools/tools/sam_with_clip.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     1371 2023-07-12 12:18:52.000000 gentopia-0.0.3/gentopia/tools/gradio_tools/tools/stable_diffusion.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     1021 2023-07-12 12:18:52.000000 gentopia-0.0.3/gentopia/tools/gradio_tools/tools/text_to_video.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     1037 2023-07-12 12:18:52.000000 gentopia-0.0.3/gentopia/tools/gradio_tools/tools/whisper.py
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     1100 2023-07-27 03:27:55.000000 gentopia-0.0.3/gentopia/tools/search_doc.py
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     4952 2023-07-27 03:27:55.000000 gentopia-0.0.3/gentopia/tools/shell.py
+drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-07 01:37:05.111283 gentopia-0.0.3/gentopia/tools/utils/
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)       23 2023-07-13 14:37:51.000000 gentopia-0.0.3/gentopia/tools/utils/__init__.py
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     2355 2023-07-13 14:37:51.000000 gentopia-0.0.3/gentopia/tools/utils/docstore.py
+drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-07 01:37:05.111283 gentopia-0.0.3/gentopia/tools/utils/document_loaders/
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-07-23 00:45:38.000000 gentopia-0.0.3/gentopia/tools/utils/document_loaders/__init__.py
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     1639 2023-07-23 00:45:38.000000 gentopia-0.0.3/gentopia/tools/utils/document_loaders/base_loader.py
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)      737 2023-07-23 00:45:38.000000 gentopia-0.0.3/gentopia/tools/utils/document_loaders/text_loader.py
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)    16131 2023-07-23 00:45:38.000000 gentopia-0.0.3/gentopia/tools/utils/document_loaders/text_splitter.py
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     1579 2023-07-23 00:45:38.000000 gentopia-0.0.3/gentopia/tools/utils/vector_store.py
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     6101 2023-07-27 03:27:55.000000 gentopia-0.0.3/gentopia/tools/weather.py
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     1298 2023-07-27 03:27:55.000000 gentopia-0.0.3/gentopia/tools/web_page.py
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     2316 2023-07-27 03:27:55.000000 gentopia-0.0.3/gentopia/tools/wikipedia.py
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     1482 2023-07-27 03:27:55.000000 gentopia-0.0.3/gentopia/tools/wolfram_alpha.py
+drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-07 01:37:05.111283 gentopia-0.0.3/gentopia/utils/
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-06-24 07:59:31.000000 gentopia-0.0.3/gentopia/utils/__init__.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      688 2023-07-23 00:45:38.000000 gentopia-0.0.3/gentopia/utils/cost_helpers.py
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-06-24 07:59:31.000000 gentopia-0.0.3/gentopia/utils/display_utils.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      878 2023-07-23 00:45:38.000000 gentopia-0.0.3/gentopia/utils/text_helpers.py
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     1690 2023-07-27 03:40:32.000000 gentopia-0.0.3/gentopia/utils/util.py
+drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-07 01:37:05.099283 gentopia-0.0.3/gentopia.egg-info/
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     7251 2023-08-07 01:37:05.000000 gentopia-0.0.3/gentopia.egg-info/PKG-INFO
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     4452 2023-08-07 01:37:05.000000 gentopia-0.0.3/gentopia.egg-info/SOURCES.txt
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)        1 2023-08-07 01:37:05.000000 gentopia-0.0.3/gentopia.egg-info/dependency_links.txt
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      310 2023-08-07 01:37:05.000000 gentopia-0.0.3/gentopia.egg-info/requires.txt
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)        9 2023-08-07 01:37:05.000000 gentopia-0.0.3/gentopia.egg-info/top_level.txt
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)       38 2023-08-07 01:37:05.111283 gentopia-0.0.3/setup.cfg
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     1192 2023-08-07 01:36:58.000000 gentopia-0.0.3/setup.py
```

### Comparing `gentopia-0.0.2/LICENSE` & `gentopia-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/PKG-INFO` & `gentopia-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: gentopia
-Version: 0.0.2
+Version: 0.0.3
 Summary: Gentopia provides extensive utilities to assembles ALM agents driven by configs.
 Home-page: https://github.com/Gentopia-AI/Gentopia
 Author: billxbf
 Author-email: billxbf@gmail.com
 License: MIT license
 Description-Content-Type: text/markdown
 Provides-Extra: huggingface
 License-File: LICENSE
 
 # Gentopia 
 🌎 *Collective Growth of Intelligent Agents.* 🦙
 
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-![Static Badge](https://img.shields.io/badge/release-beta-blue)
-[![Static Badge](https://img.shields.io/badge/Documentation-8A2BE2)](https://gentopia.readthedocs.io/en/latest/index.html)
+[![PyPI](https://img.shields.io/pypi/v/gentopia)](https://pypi.org/project/gentopia/)
+[![Read the Docs](https://img.shields.io/readthedocs/gentopia)](https://gentopia.readthedocs.io/en/latest/index.html)
 [![Static Badge](https://img.shields.io/badge/GentPool-blue)](https://github.com/Gentopia-AI/GentPool)
-[![Static Badge](https://img.shields.io/badge/backlog-grey)](https://github.com/orgs/Gentopia-AI/projects/1)
+[![Static Badge](https://img.shields.io/badge/backlog-pink)](https://github.com/orgs/Gentopia-AI/projects/1)
 [![Open Issues](https://img.shields.io/github/issues-raw/Gentopia-AI/Gentopia)](https://github.com/Gentopia-AI/Gentopia/issues)
 [![Dependency Status](https://img.shields.io/librariesio/github/Gentopia-AI/Gentopia)](https://libraries.io/github/Gentopia-AI/Gentopia)
 
 [![Twitter Follow](https://img.shields.io/twitter/follow/GentopiaAI)](https://twitter.com/GentopiaAI)
 [![](https://dcbadge.vercel.app/api/server/ASPP9MY9QK?compact=true&style=flat)](https://discord.gg/ASPP9MY9QK)
 [![YouTube Channel Subscribers](https://img.shields.io/youtube/channel/views/UC9QCjcsHJVKjKZ2Zmrq83vA)](https://www.youtube.com/channel/UC9QCjcsHJVKjKZ2Zmrq83vA)
 [![GitHub star chart](https://img.shields.io/github/stars/Gentopia-AI/Gentopia?style=social)](https://star-history.com/Gentopia-AI/Gentopia)
```

### Comparing `gentopia-0.0.2/README.md` & `gentopia-0.0.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # Gentopia 
 🌎 *Collective Growth of Intelligent Agents.* 🦙
 
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-![Static Badge](https://img.shields.io/badge/release-beta-blue)
-[![Static Badge](https://img.shields.io/badge/Documentation-8A2BE2)](https://gentopia.readthedocs.io/en/latest/index.html)
+[![PyPI](https://img.shields.io/pypi/v/gentopia)](https://pypi.org/project/gentopia/)
+[![Read the Docs](https://img.shields.io/readthedocs/gentopia)](https://gentopia.readthedocs.io/en/latest/index.html)
 [![Static Badge](https://img.shields.io/badge/GentPool-blue)](https://github.com/Gentopia-AI/GentPool)
-[![Static Badge](https://img.shields.io/badge/backlog-grey)](https://github.com/orgs/Gentopia-AI/projects/1)
+[![Static Badge](https://img.shields.io/badge/backlog-pink)](https://github.com/orgs/Gentopia-AI/projects/1)
 [![Open Issues](https://img.shields.io/github/issues-raw/Gentopia-AI/Gentopia)](https://github.com/Gentopia-AI/Gentopia/issues)
 [![Dependency Status](https://img.shields.io/librariesio/github/Gentopia-AI/Gentopia)](https://libraries.io/github/Gentopia-AI/Gentopia)
 
 [![Twitter Follow](https://img.shields.io/twitter/follow/GentopiaAI)](https://twitter.com/GentopiaAI)
 [![](https://dcbadge.vercel.app/api/server/ASPP9MY9QK?compact=true&style=flat)](https://discord.gg/ASPP9MY9QK)
 [![YouTube Channel Subscribers](https://img.shields.io/youtube/channel/views/UC9QCjcsHJVKjKZ2Zmrq83vA)](https://www.youtube.com/channel/UC9QCjcsHJVKjKZ2Zmrq83vA)
 [![GitHub star chart](https://img.shields.io/github/stars/Gentopia-AI/Gentopia?style=social)](https://star-history.com/Gentopia-AI/Gentopia)
```

### Comparing `gentopia-0.0.2/gentopia/__init__.py` & `gentopia-0.0.3/gentopia/__init__.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/agent/base_agent.py` & `gentopia-0.0.3/gentopia/agent/base_agent.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/agent/openai/agent.py` & `gentopia-0.0.3/gentopia/agent/openai/agent.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/agent/openai_memory/agent.py` & `gentopia-0.0.3/gentopia/agent/openai_memory/agent.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/agent/openai_memory/load_memory.py` & `gentopia-0.0.3/gentopia/agent/openai_memory/load_memory.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/agent/plugin_manager.py` & `gentopia-0.0.3/gentopia/agent/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/agent/react/agent.py` & `gentopia-0.0.3/gentopia/agent/react/agent.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/agent/rewoo/agent.py` & `gentopia-0.0.3/gentopia/agent/rewoo/agent.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/agent/rewoo/nodes/Planner.py` & `gentopia-0.0.3/gentopia/agent/rewoo/nodes/Planner.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/agent/rewoo/nodes/Solver.py` & `gentopia-0.0.3/gentopia/agent/rewoo/nodes/Solver.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/agent/vanilla/agent.py` & `gentopia-0.0.3/gentopia/agent/vanilla/agent.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/assembler/agent_assembler.py` & `gentopia-0.0.3/gentopia/assembler/agent_assembler.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/assembler/config.py` & `gentopia-0.0.3/gentopia/assembler/config.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/assembler/loader.py` & `gentopia-0.0.3/gentopia/assembler/loader.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/assembler/task.py` & `gentopia-0.0.3/gentopia/assembler/task.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/llm/base_llm.py` & `gentopia-0.0.3/gentopia/llm/base_llm.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/llm/client/huggingface.py` & `gentopia-0.0.3/gentopia/llm/client/huggingface.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/llm/client/openai.py` & `gentopia-0.0.3/gentopia/llm/client/openai.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/llm/llm_info.py` & `gentopia-0.0.3/gentopia/llm/llm_info.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/llm/loaders/airoboros.py` & `gentopia-0.0.3/gentopia/llm/loaders/airoboros.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/llm/loaders/alpaca.py` & `gentopia-0.0.3/gentopia/llm/loaders/alpaca.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/llm/loaders/baize.py` & `gentopia-0.0.3/gentopia/llm/loaders/baize.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/llm/loaders/bloom.py` & `gentopia-0.0.3/gentopia/llm/loaders/bloom.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/llm/loaders/camel.py` & `gentopia-0.0.3/gentopia/llm/loaders/camel.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/llm/loaders/falcon.py` & `gentopia-0.0.3/gentopia/llm/loaders/falcon.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/llm/loaders/flan_alpaca.py` & `gentopia-0.0.3/gentopia/llm/loaders/flan_alpaca.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/llm/loaders/guanaco.py` & `gentopia-0.0.3/gentopia/llm/loaders/guanaco.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/llm/loaders/mpt.py` & `gentopia-0.0.3/gentopia/llm/loaders/mpt.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/llm/loaders/redpajama.py` & `gentopia-0.0.3/gentopia/llm/loaders/redpajama.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/llm/loaders/replit.py` & `gentopia-0.0.3/gentopia/llm/loaders/replit.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/llm/loaders/samantha_vicuna.py` & `gentopia-0.0.3/gentopia/llm/loaders/samantha_vicuna.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/llm/loaders/stablelm.py` & `gentopia-0.0.3/gentopia/llm/loaders/stablelm.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/llm/loaders/t5_vicuna.py` & `gentopia-0.0.3/gentopia/llm/loaders/t5_vicuna.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/llm/loaders/vicuna.py` & `gentopia-0.0.3/gentopia/llm/loaders/vicuna.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/llm/test_llm.py` & `gentopia-0.0.3/gentopia/llm/test_llm.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/llm/wrap_llm.py` & `gentopia-0.0.3/gentopia/llm/wrap_llm.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/manager/base_llm_manager.py` & `gentopia-0.0.3/gentopia/manager/base_llm_manager.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/manager/llm_client/base_llm_client.py` & `gentopia-0.0.3/gentopia/manager/llm_client/base_llm_client.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/manager/llm_client/local_llm_client.py` & `gentopia-0.0.3/gentopia/manager/llm_client/local_llm_client.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/manager/local_llm_manager.py` & `gentopia-0.0.3/gentopia/manager/local_llm_manager.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/memory/api.py` & `gentopia-0.0.3/gentopia/memory/api.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/memory/base_memory.py` & `gentopia-0.0.3/gentopia/memory/base_memory.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/memory/embeddings.py` & `gentopia-0.0.3/gentopia/memory/embeddings.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/memory/serializable.py` & `gentopia-0.0.3/gentopia/memory/serializable.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/memory/utils.py` & `gentopia-0.0.3/gentopia/memory/utils.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/memory/vectorstores/chroma.py` & `gentopia-0.0.3/gentopia/memory/vectorstores/chroma.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/memory/vectorstores/pinecone.py` & `gentopia-0.0.3/gentopia/memory/vectorstores/pinecone.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/memory/vectorstores/vectorstore.py` & `gentopia-0.0.3/gentopia/memory/vectorstores/vectorstore.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/model/agent_model.py` & `gentopia-0.0.3/gentopia/model/agent_model.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/model/completion_model.py` & `gentopia-0.0.3/gentopia/model/completion_model.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/model/param_model.py` & `gentopia-0.0.3/gentopia/model/param_model.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/output/__init__.py` & `gentopia-0.0.3/gentopia/output/__init__.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/output/base_output.py` & `gentopia-0.0.3/gentopia/output/base_output.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,14 +75,15 @@
         None
 
         Returns:
         --------
         None
         """
         self.logger = logging
+        self.log = []
 
     def stop(self):
         """
         Stop the output.
 
         Parameters:
         -----------
@@ -191,14 +192,16 @@
         stream : bool, optional
             Not used, defaults to False.
 
         Returns:
         --------
         None
         """
+        if not stream:
+            self.log.append(item)
         if check_log():
             self.logger.info('-'*20)
             self.logger.info(item)
             self.logger.info('-' * 20)
 
     def clear(self):
         """
@@ -223,14 +226,15 @@
         content : str
             The content to log.
 
         Returns:
         --------
         None
         """
+        self.log.append(content)
         if check_log():
             self.logger.info(content)
 
     def format_json(self, json_obj: str):
         """
         Format a JSON object.
```

### Comparing `gentopia-0.0.2/gentopia/output/console_output.py` & `gentopia-0.0.3/gentopia/output/console_output.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/output/print_output.py` & `gentopia-0.0.3/gentopia/output/print_output.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/prompt/prompt_template.py` & `gentopia-0.0.3/gentopia/prompt/prompt_template.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/prompt/react.py` & `gentopia-0.0.3/gentopia/prompt/react.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/prompt/rewoo.py` & `gentopia-0.0.3/gentopia/prompt/rewoo.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/tools/__init__.py` & `gentopia-0.0.3/gentopia/tools/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from .basetool import BaseTool
 from .google_search import GoogleSearch
+from .google_scholar import *
 from .calculator import Calculator
 from .wikipedia import Wikipedia
 from .wolfram_alpha import WolframAlpha
 from .web_page import WebPage
 from .arxiv_search import ArxivSearch
 from .weather import *
 from .shell import RunShell
 from .search_doc import SearchDoc
 from .gradio import *
 from .code_interpreter import PythonCodeInterpreter
 from .file_operation import WriteFile, ReadFile
+from .duckduckgo import DuckDuckGo
 
 
 def load_tools(name: str) -> BaseTool:
     name2tool = {
         "arxiv_search": ArxivSearch,
         "calculator": Calculator,
         "python_code_interpreter": PythonCodeInterpreter,
@@ -29,11 +31,18 @@
         "search_doc": SearchDoc,
         "bash_shell": RunShell,
         "get_future_weather": GetFutureWeather,
         "get_today_weather": GetTodayWeather,
         "wikipedia": Wikipedia,
         "web_page": WebPage,
         "wolfram_alpha": WolframAlpha,
+        "duckduckgo": DuckDuckGo,
+        "search_author_by_name": SearchAuthorByName,
+        "search_author_by_interests": SearchAuthorByInterests,
+        "author_uid2paper": AuthorUID2Paper,
+        "search_paper": SearchPaper,
+        "search_related_paper": SearchRelatedPaper,
+        "search_cite_paper": SearchCitePaper,
     }
     if name not in name2tool:
         raise NotImplementedError
     return name2tool[name]
```

### Comparing `gentopia-0.0.2/gentopia/tools/arxiv_search.py` & `gentopia-0.0.3/gentopia/tools/arxiv_search.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/tools/basetool.py` & `gentopia-0.0.3/gentopia/tools/basetool.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/tools/bing_search.py` & `gentopia-0.0.3/gentopia/tools/bing_search.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/tools/calculator.py` & `gentopia-0.0.3/gentopia/tools/calculator.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/tools/code_interpreter.py` & `gentopia-0.0.3/gentopia/tools/code_interpreter.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/tools/file_operation.py` & `gentopia-0.0.3/gentopia/tools/file_operation.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/tools/google_search.py` & `gentopia-0.0.3/gentopia/tools/google_search.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/tools/gradio.py` & `gentopia-0.0.3/gentopia/tools/gradio.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/tools/gradio_tools/api.py` & `gentopia-0.0.3/gentopia/tools/gradio_tools/api.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/tools/gradio_tools/tools/__init__.py` & `gentopia-0.0.3/gentopia/tools/gradio_tools/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/tools/gradio_tools/tools/bark.py` & `gentopia-0.0.3/gentopia/tools/gradio_tools/tools/bark.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/tools/gradio_tools/tools/clip_interrogator.py` & `gentopia-0.0.3/gentopia/tools/gradio_tools/tools/clip_interrogator.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/tools/gradio_tools/tools/document_qa.py` & `gentopia-0.0.3/gentopia/tools/gradio_tools/tools/document_qa.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/tools/gradio_tools/tools/gradio_tool.py` & `gentopia-0.0.3/gentopia/tools/gradio_tools/tools/gradio_tool.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/tools/gradio_tools/tools/image_captioning.py` & `gentopia-0.0.3/gentopia/tools/gradio_tools/tools/image_captioning.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/tools/gradio_tools/tools/image_to_music.py` & `gentopia-0.0.3/gentopia/tools/gradio_tools/tools/image_to_music.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/tools/gradio_tools/tools/prompt_generator.py` & `gentopia-0.0.3/gentopia/tools/gradio_tools/tools/prompt_generator.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/tools/gradio_tools/tools/sam_with_clip.py` & `gentopia-0.0.3/gentopia/tools/gradio_tools/tools/sam_with_clip.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/tools/gradio_tools/tools/stable_diffusion.py` & `gentopia-0.0.3/gentopia/tools/gradio_tools/tools/stable_diffusion.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/tools/gradio_tools/tools/text_to_video.py` & `gentopia-0.0.3/gentopia/tools/gradio_tools/tools/text_to_video.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/tools/gradio_tools/tools/whisper.py` & `gentopia-0.0.3/gentopia/tools/gradio_tools/tools/whisper.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/tools/search_doc.py` & `gentopia-0.0.3/gentopia/tools/search_doc.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/tools/shell.py` & `gentopia-0.0.3/gentopia/tools/shell.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/tools/utils/docstore.py` & `gentopia-0.0.3/gentopia/tools/utils/docstore.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/tools/utils/document_loaders/base_loader.py` & `gentopia-0.0.3/gentopia/tools/utils/document_loaders/base_loader.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/tools/utils/document_loaders/text_loader.py` & `gentopia-0.0.3/gentopia/tools/utils/document_loaders/text_loader.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/tools/utils/document_loaders/text_splitter.py` & `gentopia-0.0.3/gentopia/tools/utils/document_loaders/text_splitter.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/tools/utils/vector_store.py` & `gentopia-0.0.3/gentopia/tools/utils/vector_store.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/tools/weather.py` & `gentopia-0.0.3/gentopia/tools/weather.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/tools/web_page.py` & `gentopia-0.0.3/gentopia/tools/web_page.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/tools/wikipedia.py` & `gentopia-0.0.3/gentopia/tools/wikipedia.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/tools/wolfram_alpha.py` & `gentopia-0.0.3/gentopia/tools/wolfram_alpha.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/utils/cost_helpers.py` & `gentopia-0.0.3/gentopia/utils/cost_helpers.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/utils/text_helpers.py` & `gentopia-0.0.3/gentopia/utils/text_helpers.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia/utils/util.py` & `gentopia-0.0.3/gentopia/utils/util.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.2/gentopia.egg-info/PKG-INFO` & `gentopia-0.0.3/gentopia.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: gentopia
-Version: 0.0.2
+Version: 0.0.3
 Summary: Gentopia provides extensive utilities to assembles ALM agents driven by configs.
 Home-page: https://github.com/Gentopia-AI/Gentopia
 Author: billxbf
 Author-email: billxbf@gmail.com
 License: MIT license
 Description-Content-Type: text/markdown
 Provides-Extra: huggingface
 License-File: LICENSE
 
 # Gentopia 
 🌎 *Collective Growth of Intelligent Agents.* 🦙
 
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-![Static Badge](https://img.shields.io/badge/release-beta-blue)
-[![Static Badge](https://img.shields.io/badge/Documentation-8A2BE2)](https://gentopia.readthedocs.io/en/latest/index.html)
+[![PyPI](https://img.shields.io/pypi/v/gentopia)](https://pypi.org/project/gentopia/)
+[![Read the Docs](https://img.shields.io/readthedocs/gentopia)](https://gentopia.readthedocs.io/en/latest/index.html)
 [![Static Badge](https://img.shields.io/badge/GentPool-blue)](https://github.com/Gentopia-AI/GentPool)
-[![Static Badge](https://img.shields.io/badge/backlog-grey)](https://github.com/orgs/Gentopia-AI/projects/1)
+[![Static Badge](https://img.shields.io/badge/backlog-pink)](https://github.com/orgs/Gentopia-AI/projects/1)
 [![Open Issues](https://img.shields.io/github/issues-raw/Gentopia-AI/Gentopia)](https://github.com/Gentopia-AI/Gentopia/issues)
 [![Dependency Status](https://img.shields.io/librariesio/github/Gentopia-AI/Gentopia)](https://libraries.io/github/Gentopia-AI/Gentopia)
 
 [![Twitter Follow](https://img.shields.io/twitter/follow/GentopiaAI)](https://twitter.com/GentopiaAI)
 [![](https://dcbadge.vercel.app/api/server/ASPP9MY9QK?compact=true&style=flat)](https://discord.gg/ASPP9MY9QK)
 [![YouTube Channel Subscribers](https://img.shields.io/youtube/channel/views/UC9QCjcsHJVKjKZ2Zmrq83vA)](https://www.youtube.com/channel/UC9QCjcsHJVKjKZ2Zmrq83vA)
 [![GitHub star chart](https://img.shields.io/github/stars/Gentopia-AI/Gentopia?style=social)](https://star-history.com/Gentopia-AI/Gentopia)
```

### Comparing `gentopia-0.0.2/gentopia.egg-info/SOURCES.txt` & `gentopia-0.0.3/gentopia.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,17 @@
 gentopia/resource/__init__.py
 gentopia/tools/__init__.py
 gentopia/tools/arxiv_search.py
 gentopia/tools/basetool.py
 gentopia/tools/bing_search.py
 gentopia/tools/calculator.py
 gentopia/tools/code_interpreter.py
+gentopia/tools/duckduckgo.py
 gentopia/tools/file_operation.py
+gentopia/tools/google_scholar.py
 gentopia/tools/google_search.py
 gentopia/tools/gradio.py
 gentopia/tools/search_doc.py
 gentopia/tools/shell.py
 gentopia/tools/weather.py
 gentopia/tools/web_page.py
 gentopia/tools/wikipedia.py
```

### Comparing `gentopia-0.0.2/setup.py` & `gentopia-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gentopia',
-    version='0.0.2',
+    version='0.0.3',
     packages=find_packages(exclude=['llm', 'llm.*']),
     url='https://github.com/Gentopia-AI/Gentopia',
     license='MIT license',
     author='billxbf',
     author_email='billxbf@gmail.com',
     description='Gentopia provides extensive utilities to assembles ALM agents driven by configs.',
     long_description=open('README.md').read(),
@@ -37,11 +37,11 @@
         'requests',
         'setuptools',
         'uvicorn',
         'openai',
         'pexpect',
         'gradio_client',
         'pinecone-client',
-        'chroma',
         'chromadb',
+        'tiktoken',
     ],
 )
```

