# Comparing `tmp/semantic_kernel-0.3.5.dev0.tar.gz` & `tmp/semantic_kernel-0.3.6.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semantic_kernel-0.3.5.dev0.tar", max compression
+gzip compressed data, was "semantic_kernel-0.3.6.dev0.tar", max compression
```

## Comparing `semantic_kernel-0.3.5.dev0.tar` & `semantic_kernel-0.3.6.dev0.tar`

### file list

```diff
@@ -1,120 +1,123 @@
--rw-r--r--   0        0        0     1186 2023-05-08 23:38:10.000000 semantic_kernel-0.3.5.dev0/pip/README.md
--rw-r--r--   0        0        0     1514 2023-08-02 21:24:55.086486 semantic_kernel-0.3.5.dev0/pyproject.toml
--rw-r--r--   0        0        0     1375 2023-07-12 19:14:40.912511 semantic_kernel-0.3.5.dev0/semantic_kernel/__init__.py
--rw-r--r--   0        0        0      719 2023-05-25 17:48:21.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/ai/__init__.py
--rw-r--r--   0        0        0     1647 2023-04-30 18:57:02.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/ai/ai_exception.py
--rw-r--r--   0        0        0     1792 2023-06-12 17:06:53.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/ai/chat_completion_client_base.py
--rw-r--r--   0        0        0     1321 2023-07-14 16:57:26.312407 semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/ai/chat_request_settings.py
--rw-r--r--   0        0        0     1484 2023-07-14 16:57:26.312942 semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/ai/complete_request_settings.py
--rw-r--r--   0        0        0      282 2023-04-30 18:57:02.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/ai/embeddings/embedding_generator_base.py
--rw-r--r--   0        0        0      352 2023-04-30 18:57:02.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/ai/hugging_face/__init__.py
--rw-r--r--   0        0        0     6161 2023-06-12 17:06:53.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py
--rw-r--r--   0        0        0     2317 2023-05-08 23:38:10.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py
--rw-r--r--   0        0        0      892 2023-04-30 18:57:02.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/ai/open_ai/__init__.py
--rw-r--r--   0        0        0     2615 2023-05-15 18:12:57.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py
--rw-r--r--   0        0        0     2607 2023-05-15 18:12:57.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py
--rw-r--r--   0        0        0     2602 2023-05-15 18:12:57.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py
--rw-r--r--   0        0        0     8903 2023-07-16 00:59:27.692753 semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py
--rw-r--r--   0        0        0     5788 2023-07-16 00:59:27.693316 semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py
--rw-r--r--   0        0        0     2723 2023-05-15 18:12:57.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py
--rw-r--r--   0        0        0     1616 2023-06-12 17:06:53.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/ai/text_completion_client_base.py
--rw-r--r--   0        0        0      242 2023-07-21 00:24:52.991872 semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/memory/azure_cognitive_search/__init__.py
--rw-r--r--   0        0        0    15609 2023-07-21 00:24:52.992413 semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/memory/azure_cognitive_search/azure_cognitive_search_memory_store.py
--rw-r--r--   0        0        0     8224 2023-07-21 00:24:52.992894 semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/memory/azure_cognitive_search/utils.py
--rw-r--r--   0        0        0      182 2023-05-18 17:32:52.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/memory/chroma/__init__.py
--rw-r--r--   0        0        0    15093 2023-08-02 21:24:01.722277 semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/memory/chroma/chroma_memory_store.py
--rw-r--r--   0        0        0     4426 2023-07-16 00:58:38.000353 semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/memory/chroma/utils.py
--rw-r--r--   0        0        0      133 2023-07-21 00:24:52.995551 semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/memory/milvus/__init__.py
--rw-r--r--   0        0        0    16859 2023-07-21 00:24:52.995917 semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/memory/milvus/milvus_memory_store.py
--rw-r--r--   0        0        0      190 2023-07-06 22:13:35.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/memory/pinecone/__init__.py
--rw-r--r--   0        0        0    14928 2023-07-12 19:14:40.913001 semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/memory/pinecone/pinecone_memory_store.py
--rw-r--r--   0        0        0     1154 2023-07-06 22:13:35.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/memory/pinecone/utils.py
--rw-r--r--   0        0        0      190 2023-07-12 19:14:40.913420 semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/memory/postgres/__init__.py
--rw-r--r--   0        0        0    20480 2023-07-12 19:14:40.913726 semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/memory/postgres/postgres_memory_store.py
--rw-r--r--   0        0        0      182 2023-08-02 21:24:01.723071 semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/memory/qdrant/__init__.py
--rw-r--r--   0        0        0    11910 2023-08-02 21:24:01.723452 semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/memory/qdrant/qdrant_memory_store.py
--rw-r--r--   0        0        0    11295 2023-06-12 17:06:53.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/memory/weaviate/weaviate_memory_store.py
--rw-r--r--   0        0        0      265 2023-08-02 21:24:01.724044 semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/search_engine/__init__.py
--rw-r--r--   0        0        0     2891 2023-08-02 21:24:01.724670 semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/search_engine/bing_connector.py
--rw-r--r--   0        0        0      254 2023-08-02 21:24:01.725238 semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/search_engine/connector.py
--rw-r--r--   0        0        0     3268 2023-08-02 21:24:01.725609 semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/search_engine/google_connector.py
--rw-r--r--   0        0        0      804 2023-07-17 21:15:24.599960 semantic_kernel-0.3.5.dev0/semantic_kernel/core_skills/__init__.py
--rw-r--r--   0        0        0     2510 2023-05-15 18:12:57.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/core_skills/conversation_summary_skill.py
--rw-r--r--   0        0        0     2131 2023-07-16 00:59:27.693756 semantic_kernel-0.3.5.dev0/semantic_kernel/core_skills/file_io_skill.py
--rw-r--r--   0        0        0     3754 2023-04-22 04:06:40.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/core_skills/http_skill.py
--rw-r--r--   0        0        0     3172 2023-08-02 21:24:01.726389 semantic_kernel-0.3.5.dev0/semantic_kernel/core_skills/math_skill.py
--rw-r--r--   0        0        0     4641 2023-04-14 00:51:57.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/core_skills/text_memory_skill.py
--rw-r--r--   0        0        0     2462 2023-07-16 00:59:27.694343 semantic_kernel-0.3.5.dev0/semantic_kernel/core_skills/text_skill.py
--rw-r--r--   0        0        0     7909 2023-07-16 00:59:27.694865 semantic_kernel-0.3.5.dev0/semantic_kernel/core_skills/time_skill.py
--rw-r--r--   0        0        0      678 2023-07-16 00:59:27.695359 semantic_kernel-0.3.5.dev0/semantic_kernel/core_skills/wait_skill.py
--rw-r--r--   0        0        0     1950 2023-07-17 21:15:24.600357 semantic_kernel-0.3.5.dev0/semantic_kernel/core_skills/web_search_engine_skill.py
--rw-r--r--   0        0        0    32289 2023-07-17 21:15:24.601483 semantic_kernel-0.3.5.dev0/semantic_kernel/kernel.py
--rw-r--r--   0        0        0     1726 2023-07-16 00:59:27.695868 semantic_kernel-0.3.5.dev0/semantic_kernel/kernel_exception.py
--rw-r--r--   0        0        0      160 2023-04-13 23:12:46.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/memory/__init__.py
--rw-r--r--   0        0        0     2544 2023-06-08 17:22:29.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/memory/memory_query_result.py
--rw-r--r--   0        0        0     3912 2023-07-12 19:14:40.914195 semantic_kernel-0.3.5.dev0/semantic_kernel/memory/memory_record.py
--rw-r--r--   0        0        0     7272 2023-08-02 21:24:01.726940 semantic_kernel-0.3.5.dev0/semantic_kernel/memory/memory_store_base.py
--rw-r--r--   0        0        0     1666 2023-08-02 21:24:01.727814 semantic_kernel-0.3.5.dev0/semantic_kernel/memory/null_memory.py
--rw-r--r--   0        0        0     6354 2023-07-16 00:42:59.250269 semantic_kernel-0.3.5.dev0/semantic_kernel/memory/semantic_text_memory.py
--rw-r--r--   0        0        0     3418 2023-08-02 21:24:01.728381 semantic_kernel-0.3.5.dev0/semantic_kernel/memory/semantic_text_memory_base.py
--rw-r--r--   0        0        0    12032 2023-05-15 18:12:57.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/memory/volatile_memory_store.py
--rw-r--r--   0        0        0     2361 2023-04-22 04:06:40.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/orchestration/context_variables.py
--rw-r--r--   0        0        0     5079 2023-04-14 00:51:57.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/orchestration/delegate_handlers.py
--rw-r--r--   0        0        0     9005 2023-05-19 23:02:13.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/orchestration/delegate_inference.py
--rw-r--r--   0        0        0      638 2023-04-13 23:12:46.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/orchestration/delegate_types.py
--rw-r--r--   0        0        0     7514 2023-04-14 00:52:05.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/orchestration/sk_context.py
--rw-r--r--   0        0        0    16088 2023-07-06 22:13:35.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/orchestration/sk_function.py
--rw-r--r--   0        0        0     6158 2023-04-30 18:57:02.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/orchestration/sk_function_base.py
--rw-r--r--   0        0        0      408 2023-08-02 21:24:01.729218 semantic_kernel-0.3.5.dev0/semantic_kernel/planning/__init__.py
--rw-r--r--   0        0        0    12891 2023-08-02 21:24:01.729812 semantic_kernel-0.3.5.dev0/semantic_kernel/planning/action_planner/action_planner.py
--rw-r--r--   0        0        0      355 2023-08-02 21:24:01.730504 semantic_kernel-0.3.5.dev0/semantic_kernel/planning/action_planner/skprompt.txt
--rw-r--r--   0        0        0     7538 2023-07-06 22:13:35.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/planning/basic_planner.py
--rw-r--r--   0        0        0    16642 2023-08-02 21:24:01.731111 semantic_kernel-0.3.5.dev0/semantic_kernel/planning/plan.py
--rw-r--r--   0        0        0     1198 2023-08-02 21:24:01.731437 semantic_kernel-0.3.5.dev0/semantic_kernel/planning/planning_exception.py
--rw-r--r--   0        0        0      723 2023-08-02 21:24:01.732600 semantic_kernel-0.3.5.dev0/semantic_kernel/planning/sequential_planner/Skills/SequentialPlanning/config.json
--rw-r--r--   0        0        0     3005 2023-08-02 21:24:01.732891 semantic_kernel-0.3.5.dev0/semantic_kernel/planning/sequential_planner/Skills/SequentialPlanning/skprompt.txt
--rw-r--r--   0        0        0      142 2023-08-02 21:24:01.733143 semantic_kernel-0.3.5.dev0/semantic_kernel/planning/sequential_planner/__init__.py
--rw-r--r--   0        0        0     5761 2023-08-02 21:24:01.733497 semantic_kernel-0.3.5.dev0/semantic_kernel/planning/sequential_planner/sequential_planner.py
--rw-r--r--   0        0        0     1147 2023-08-02 21:24:01.733879 semantic_kernel-0.3.5.dev0/semantic_kernel/planning/sequential_planner/sequential_planner_config.py
--rw-r--r--   0        0        0     8558 2023-08-02 21:24:01.734424 semantic_kernel-0.3.5.dev0/semantic_kernel/planning/sequential_planner/sequential_planner_extensions.py
--rw-r--r--   0        0        0     5515 2023-08-02 21:24:01.734840 semantic_kernel-0.3.5.dev0/semantic_kernel/planning/sequential_planner/sequential_planner_parser.py
--rw-r--r--   0        0        0      932 2023-05-19 23:02:13.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/reliability/pass_through_without_retry.py
--rw-r--r--   0        0        0      694 2023-06-05 21:39:19.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/reliability/retry_mechanism_base.py
--rw-r--r--   0        0        0     2101 2023-04-13 23:12:46.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/semantic_functions/chat_prompt_template.py
--rw-r--r--   0        0        0     2332 2023-04-14 00:51:57.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/semantic_functions/prompt_template.py
--rw-r--r--   0        0        0      506 2023-04-13 23:12:46.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/semantic_functions/prompt_template_base.py
--rw-r--r--   0        0        0     4525 2023-06-12 17:06:53.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/semantic_functions/prompt_template_config.py
--rw-r--r--   0        0        0      671 2023-04-14 00:51:57.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/semantic_functions/semantic_function_config.py
--rw-r--r--   0        0        0      322 2023-04-14 00:51:57.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/skill_definition/__init__.py
--rw-r--r--   0        0        0     2053 2023-04-14 00:51:57.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/skill_definition/function_view.py
--rw-r--r--   0        0        0     2199 2023-06-12 17:06:53.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/skill_definition/functions_view.py
--rw-r--r--   0        0        0     1026 2023-04-14 00:51:57.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/skill_definition/parameter_view.py
--rw-r--r--   0        0        0     2104 2023-04-14 00:51:57.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/skill_definition/read_only_skill_collection.py
--rw-r--r--   0        0        0     1345 2023-04-14 00:51:57.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/skill_definition/read_only_skill_collection_base.py
--rw-r--r--   0        0        0      858 2023-04-13 23:12:46.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/skill_definition/sk_function_context_parameter_decorator.py
--rw-r--r--   0        0        0      837 2023-04-14 00:51:57.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/skill_definition/sk_function_decorator.py
--rw-r--r--   0        0        0     6056 2023-04-14 00:51:57.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/skill_definition/skill_collection.py
--rw-r--r--   0        0        0      803 2023-04-13 23:12:46.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/skill_definition/skill_collection_base.py
--rw-r--r--   0        0        0     1115 2023-04-13 23:12:46.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/template_engine/README.md
--rw-r--r--   0        0        0      830 2023-04-14 00:51:57.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/template_engine/blocks/block.py
--rw-r--r--   0        0        0      228 2023-04-14 00:51:57.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/template_engine/blocks/block_types.py
--rw-r--r--   0        0        0     4577 2023-04-30 18:57:03.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/template_engine/blocks/code_block.py
--rw-r--r--   0        0        0     2653 2023-04-13 23:12:46.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/template_engine/blocks/function_id_block.py
--rw-r--r--   0        0        0      276 2023-04-13 23:12:46.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/template_engine/blocks/symbols.py
--rw-r--r--   0        0        0     1534 2023-04-14 00:51:57.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/template_engine/blocks/text_block.py
--rw-r--r--   0        0        0     2274 2023-04-13 23:12:46.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/template_engine/blocks/val_block.py
--rw-r--r--   0        0        0     2517 2023-04-14 00:51:57.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/template_engine/blocks/var_block.py
--rw-r--r--   0        0        0     6535 2023-04-13 23:12:46.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/template_engine/code_tokenizer.py
--rw-r--r--   0        0        0     6051 2023-04-14 00:51:57.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/template_engine/prompt_template_engine.py
--rw-r--r--   0        0        0      532 2023-04-13 23:12:46.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/template_engine/protocols/code_renderer.py
--rw-r--r--   0        0        0     3043 2023-04-13 23:12:46.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/template_engine/protocols/prompt_templating_engine.py
--rw-r--r--   0        0        0      596 2023-04-13 23:12:46.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/template_engine/protocols/text_renderer.py
--rw-r--r--   0        0        0     7637 2023-04-13 23:12:46.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/template_engine/template_tokenizer.py
--rw-r--r--   0        0        0      473 2023-04-30 18:57:03.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/text/__init__.py
--rw-r--r--   0        0        0      667 2023-04-30 18:57:03.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/text/function_extension.py
--rw-r--r--   0        0        0     8568 2023-07-16 00:58:38.006510 semantic_kernel-0.3.5.dev0/semantic_kernel/text/text_chunker.py
--rw-r--r--   0        0        0      403 2023-04-13 23:12:46.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/utils/null_logger.py
--rw-r--r--   0        0        0     2694 2023-07-12 19:14:40.915313 semantic_kernel-0.3.5.dev0/semantic_kernel/utils/settings.py
--rw-r--r--   0        0        0      221 2023-04-13 23:12:46.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/utils/static_property.py
--rw-r--r--   0        0        0     2198 2023-04-13 23:12:46.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/utils/validation.py
--rw-r--r--   0        0        0     1843 1970-01-01 00:00:00.000000 semantic_kernel-0.3.5.dev0/PKG-INFO
+-rw-r--r--   0        0        0     1186 2023-05-08 23:38:10.000000 semantic_kernel-0.3.6.dev0/pip/README.md
+-rw-r--r--   0        0        0     1577 2023-08-07 16:13:48.135392 semantic_kernel-0.3.6.dev0/pyproject.toml
+-rw-r--r--   0        0        0     1375 2023-07-12 19:14:40.912511 semantic_kernel-0.3.6.dev0/semantic_kernel/__init__.py
+-rw-r--r--   0        0        0      719 2023-05-25 17:48:21.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/ai/__init__.py
+-rw-r--r--   0        0        0     1647 2023-04-30 18:57:02.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/ai/ai_exception.py
+-rw-r--r--   0        0        0     1792 2023-06-12 17:06:53.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/ai/chat_completion_client_base.py
+-rw-r--r--   0        0        0     1321 2023-07-14 16:57:26.312407 semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/ai/chat_request_settings.py
+-rw-r--r--   0        0        0     1484 2023-07-14 16:57:26.312942 semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/ai/complete_request_settings.py
+-rw-r--r--   0        0        0      282 2023-04-30 18:57:02.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/ai/embeddings/embedding_generator_base.py
+-rw-r--r--   0        0        0      352 2023-04-30 18:57:02.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/ai/hugging_face/__init__.py
+-rw-r--r--   0        0        0     6190 2023-08-07 16:13:48.138206 semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py
+-rw-r--r--   0        0        0     2317 2023-05-08 23:38:10.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py
+-rw-r--r--   0        0        0      892 2023-04-30 18:57:02.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/ai/open_ai/__init__.py
+-rw-r--r--   0        0        0     2615 2023-05-15 18:12:57.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py
+-rw-r--r--   0        0        0     2607 2023-05-15 18:12:57.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py
+-rw-r--r--   0        0        0     2602 2023-05-15 18:12:57.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py
+-rw-r--r--   0        0        0     8903 2023-07-16 00:59:27.692753 semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py
+-rw-r--r--   0        0        0     5788 2023-07-16 00:59:27.693316 semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py
+-rw-r--r--   0        0        0     3007 2023-08-07 16:13:48.139150 semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py
+-rw-r--r--   0        0        0     1616 2023-06-12 17:06:53.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/ai/text_completion_client_base.py
+-rw-r--r--   0        0        0      242 2023-07-21 00:24:52.991872 semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/memory/azure_cognitive_search/__init__.py
+-rw-r--r--   0        0        0    15609 2023-07-21 00:24:52.992413 semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/memory/azure_cognitive_search/azure_cognitive_search_memory_store.py
+-rw-r--r--   0        0        0     8224 2023-07-21 00:24:52.992894 semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/memory/azure_cognitive_search/utils.py
+-rw-r--r--   0        0        0      182 2023-05-18 17:32:52.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/memory/chroma/__init__.py
+-rw-r--r--   0        0        0    15093 2023-08-02 21:24:01.722277 semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/memory/chroma/chroma_memory_store.py
+-rw-r--r--   0        0        0     4426 2023-07-16 00:58:38.000353 semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/memory/chroma/utils.py
+-rw-r--r--   0        0        0      133 2023-07-21 00:24:52.995551 semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/memory/milvus/__init__.py
+-rw-r--r--   0        0        0    16859 2023-07-21 00:24:52.995917 semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/memory/milvus/milvus_memory_store.py
+-rw-r--r--   0        0        0      190 2023-07-06 22:13:35.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/memory/pinecone/__init__.py
+-rw-r--r--   0        0        0    14928 2023-07-12 19:14:40.913001 semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/memory/pinecone/pinecone_memory_store.py
+-rw-r--r--   0        0        0     1154 2023-07-06 22:13:35.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/memory/pinecone/utils.py
+-rw-r--r--   0        0        0      190 2023-07-12 19:14:40.913420 semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/memory/postgres/__init__.py
+-rw-r--r--   0        0        0    20480 2023-07-12 19:14:40.913726 semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/memory/postgres/postgres_memory_store.py
+-rw-r--r--   0        0        0      182 2023-08-02 21:24:01.723071 semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/memory/qdrant/__init__.py
+-rw-r--r--   0        0        0    11910 2023-08-02 21:24:01.723452 semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/memory/qdrant/qdrant_memory_store.py
+-rw-r--r--   0        0        0    11295 2023-06-12 17:06:53.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/memory/weaviate/weaviate_memory_store.py
+-rw-r--r--   0        0        0      126 2023-08-07 16:13:48.139679 semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/openapi/__init__.py
+-rw-r--r--   0        0        0    11132 2023-08-07 16:13:48.140037 semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/openapi/sk_openapi.py
+-rw-r--r--   0        0        0      265 2023-08-02 21:24:01.724044 semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/search_engine/__init__.py
+-rw-r--r--   0        0        0     2891 2023-08-02 21:24:01.724670 semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/search_engine/bing_connector.py
+-rw-r--r--   0        0        0      254 2023-08-02 21:24:01.725238 semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/search_engine/connector.py
+-rw-r--r--   0        0        0     3268 2023-08-02 21:24:01.725609 semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/search_engine/google_connector.py
+-rw-r--r--   0        0        0      804 2023-07-17 21:15:24.599960 semantic_kernel-0.3.6.dev0/semantic_kernel/core_skills/__init__.py
+-rw-r--r--   0        0        0     2553 2023-08-07 16:13:48.140835 semantic_kernel-0.3.6.dev0/semantic_kernel/core_skills/conversation_summary_skill.py
+-rw-r--r--   0        0        0     2200 2023-08-07 16:13:48.141276 semantic_kernel-0.3.6.dev0/semantic_kernel/core_skills/file_io_skill.py
+-rw-r--r--   0        0        0     3823 2023-08-07 16:13:48.141662 semantic_kernel-0.3.6.dev0/semantic_kernel/core_skills/http_skill.py
+-rw-r--r--   0        0        0     3264 2023-08-07 16:13:48.142147 semantic_kernel-0.3.6.dev0/semantic_kernel/core_skills/math_skill.py
+-rw-r--r--   0        0        0     4710 2023-08-07 16:13:48.142825 semantic_kernel-0.3.6.dev0/semantic_kernel/core_skills/text_memory_skill.py
+-rw-r--r--   0        0        0     2531 2023-08-07 16:13:48.143278 semantic_kernel-0.3.6.dev0/semantic_kernel/core_skills/text_skill.py
+-rw-r--r--   0        0        0     7978 2023-08-07 16:13:48.143817 semantic_kernel-0.3.6.dev0/semantic_kernel/core_skills/time_skill.py
+-rw-r--r--   0        0        0      747 2023-08-07 16:13:48.144413 semantic_kernel-0.3.6.dev0/semantic_kernel/core_skills/wait_skill.py
+-rw-r--r--   0        0        0     1950 2023-07-17 21:15:24.600357 semantic_kernel-0.3.6.dev0/semantic_kernel/core_skills/web_search_engine_skill.py
+-rw-r--r--   0        0        0    31084 2023-08-07 16:13:48.145351 semantic_kernel-0.3.6.dev0/semantic_kernel/kernel.py
+-rw-r--r--   0        0        0     1726 2023-07-16 00:59:27.695868 semantic_kernel-0.3.6.dev0/semantic_kernel/kernel_exception.py
+-rw-r--r--   0        0        0      160 2023-04-13 23:12:46.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/memory/__init__.py
+-rw-r--r--   0        0        0     2544 2023-06-08 17:22:29.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/memory/memory_query_result.py
+-rw-r--r--   0        0        0     3912 2023-07-12 19:14:40.914195 semantic_kernel-0.3.6.dev0/semantic_kernel/memory/memory_record.py
+-rw-r--r--   0        0        0     7272 2023-08-02 21:24:01.726940 semantic_kernel-0.3.6.dev0/semantic_kernel/memory/memory_store_base.py
+-rw-r--r--   0        0        0     1666 2023-08-02 21:24:01.727814 semantic_kernel-0.3.6.dev0/semantic_kernel/memory/null_memory.py
+-rw-r--r--   0        0        0     6354 2023-07-16 00:42:59.250269 semantic_kernel-0.3.6.dev0/semantic_kernel/memory/semantic_text_memory.py
+-rw-r--r--   0        0        0     3418 2023-08-02 21:24:01.728381 semantic_kernel-0.3.6.dev0/semantic_kernel/memory/semantic_text_memory_base.py
+-rw-r--r--   0        0        0    12032 2023-05-15 18:12:57.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/memory/volatile_memory_store.py
+-rw-r--r--   0        0        0     2361 2023-04-22 04:06:40.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/orchestration/context_variables.py
+-rw-r--r--   0        0        0     5079 2023-04-14 00:51:57.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/orchestration/delegate_handlers.py
+-rw-r--r--   0        0        0     9005 2023-05-19 23:02:13.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/orchestration/delegate_inference.py
+-rw-r--r--   0        0        0      638 2023-04-13 23:12:46.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/orchestration/delegate_types.py
+-rw-r--r--   0        0        0     7514 2023-04-14 00:52:05.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/orchestration/sk_context.py
+-rw-r--r--   0        0        0    21047 2023-08-07 16:13:48.146463 semantic_kernel-0.3.6.dev0/semantic_kernel/orchestration/sk_function.py
+-rw-r--r--   0        0        0     6289 2023-08-07 16:13:48.147317 semantic_kernel-0.3.6.dev0/semantic_kernel/orchestration/sk_function_base.py
+-rw-r--r--   0        0        0      408 2023-08-02 21:24:01.729218 semantic_kernel-0.3.6.dev0/semantic_kernel/planning/__init__.py
+-rw-r--r--   0        0        0    12946 2023-08-07 16:13:48.148064 semantic_kernel-0.3.6.dev0/semantic_kernel/planning/action_planner/action_planner.py
+-rw-r--r--   0        0        0      355 2023-08-02 21:24:01.730504 semantic_kernel-0.3.6.dev0/semantic_kernel/planning/action_planner/skprompt.txt
+-rw-r--r--   0        0        0     7536 2023-08-07 16:13:48.149023 semantic_kernel-0.3.6.dev0/semantic_kernel/planning/basic_planner.py
+-rw-r--r--   0        0        0    16641 2023-08-07 16:13:48.149664 semantic_kernel-0.3.6.dev0/semantic_kernel/planning/plan.py
+-rw-r--r--   0        0        0     1198 2023-08-02 21:24:01.731437 semantic_kernel-0.3.6.dev0/semantic_kernel/planning/planning_exception.py
+-rw-r--r--   0        0        0      723 2023-08-02 21:24:01.732600 semantic_kernel-0.3.6.dev0/semantic_kernel/planning/sequential_planner/Skills/SequentialPlanning/config.json
+-rw-r--r--   0        0        0     3005 2023-08-02 21:24:01.732891 semantic_kernel-0.3.6.dev0/semantic_kernel/planning/sequential_planner/Skills/SequentialPlanning/skprompt.txt
+-rw-r--r--   0        0        0      142 2023-08-02 21:24:01.733143 semantic_kernel-0.3.6.dev0/semantic_kernel/planning/sequential_planner/__init__.py
+-rw-r--r--   0        0        0     5761 2023-08-02 21:24:01.733497 semantic_kernel-0.3.6.dev0/semantic_kernel/planning/sequential_planner/sequential_planner.py
+-rw-r--r--   0        0        0     1147 2023-08-02 21:24:01.733879 semantic_kernel-0.3.6.dev0/semantic_kernel/planning/sequential_planner/sequential_planner_config.py
+-rw-r--r--   0        0        0     8636 2023-08-07 16:13:48.150305 semantic_kernel-0.3.6.dev0/semantic_kernel/planning/sequential_planner/sequential_planner_extensions.py
+-rw-r--r--   0        0        0     5515 2023-08-02 21:24:01.734840 semantic_kernel-0.3.6.dev0/semantic_kernel/planning/sequential_planner/sequential_planner_parser.py
+-rw-r--r--   0        0        0     1001 2023-08-07 16:13:48.151163 semantic_kernel-0.3.6.dev0/semantic_kernel/reliability/pass_through_without_retry.py
+-rw-r--r--   0        0        0      694 2023-06-05 21:39:19.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/reliability/retry_mechanism_base.py
+-rw-r--r--   0        0        0     2101 2023-04-13 23:12:46.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/semantic_functions/chat_prompt_template.py
+-rw-r--r--   0        0        0     2332 2023-04-14 00:51:57.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/semantic_functions/prompt_template.py
+-rw-r--r--   0        0        0      506 2023-04-13 23:12:46.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/semantic_functions/prompt_template_base.py
+-rw-r--r--   0        0        0     4525 2023-06-12 17:06:53.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/semantic_functions/prompt_template_config.py
+-rw-r--r--   0        0        0      671 2023-04-14 00:51:57.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/semantic_functions/semantic_function_config.py
+-rw-r--r--   0        0        0     2793 2023-08-07 16:13:48.151449 semantic_kernel-0.3.6.dev0/semantic_kernel/sk_pydantic.py
+-rw-r--r--   0        0        0      322 2023-04-14 00:51:57.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/skill_definition/__init__.py
+-rw-r--r--   0        0        0      958 2023-08-07 16:13:48.152176 semantic_kernel-0.3.6.dev0/semantic_kernel/skill_definition/function_view.py
+-rw-r--r--   0        0        0     2323 2023-08-07 16:13:48.152617 semantic_kernel-0.3.6.dev0/semantic_kernel/skill_definition/functions_view.py
+-rw-r--r--   0        0        0      506 2023-08-07 16:13:48.153078 semantic_kernel-0.3.6.dev0/semantic_kernel/skill_definition/parameter_view.py
+-rw-r--r--   0        0        0     4821 2023-08-07 16:13:48.153598 semantic_kernel-0.3.6.dev0/semantic_kernel/skill_definition/read_only_skill_collection.py
+-rw-r--r--   0        0        0     1415 2023-08-07 16:13:48.154182 semantic_kernel-0.3.6.dev0/semantic_kernel/skill_definition/read_only_skill_collection_base.py
+-rw-r--r--   0        0        0      817 2023-08-07 16:13:48.155067 semantic_kernel-0.3.6.dev0/semantic_kernel/skill_definition/sk_function_context_parameter_decorator.py
+-rw-r--r--   0        0        0      840 2023-08-07 16:13:48.155620 semantic_kernel-0.3.6.dev0/semantic_kernel/skill_definition/sk_function_decorator.py
+-rw-r--r--   0        0        0     4945 2023-08-07 16:13:48.156191 semantic_kernel-0.3.6.dev0/semantic_kernel/skill_definition/skill_collection.py
+-rw-r--r--   0        0        0      959 2023-08-07 16:13:48.156737 semantic_kernel-0.3.6.dev0/semantic_kernel/skill_definition/skill_collection_base.py
+-rw-r--r--   0        0        0     1115 2023-04-13 23:12:46.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/template_engine/README.md
+-rw-r--r--   0        0        0      918 2023-08-07 16:13:48.157561 semantic_kernel-0.3.6.dev0/semantic_kernel/template_engine/blocks/block.py
+-rw-r--r--   0        0        0      228 2023-04-14 00:51:57.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/template_engine/blocks/block_types.py
+-rw-r--r--   0        0        0     4606 2023-08-07 16:13:48.157992 semantic_kernel-0.3.6.dev0/semantic_kernel/template_engine/blocks/code_block.py
+-rw-r--r--   0        0        0     3053 2023-08-07 16:13:48.158688 semantic_kernel-0.3.6.dev0/semantic_kernel/template_engine/blocks/function_id_block.py
+-rw-r--r--   0        0        0      276 2023-04-13 23:12:46.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/template_engine/blocks/symbols.py
+-rw-r--r--   0        0        0     1519 2023-08-07 16:13:48.159110 semantic_kernel-0.3.6.dev0/semantic_kernel/template_engine/blocks/text_block.py
+-rw-r--r--   0        0        0     2311 2023-08-07 16:13:48.159574 semantic_kernel-0.3.6.dev0/semantic_kernel/template_engine/blocks/val_block.py
+-rw-r--r--   0        0        0     2637 2023-08-07 16:13:48.159998 semantic_kernel-0.3.6.dev0/semantic_kernel/template_engine/blocks/var_block.py
+-rw-r--r--   0        0        0     6604 2023-08-07 16:13:48.160845 semantic_kernel-0.3.6.dev0/semantic_kernel/template_engine/code_tokenizer.py
+-rw-r--r--   0        0        0     6035 2023-08-07 16:13:48.161444 semantic_kernel-0.3.6.dev0/semantic_kernel/template_engine/prompt_template_engine.py
+-rw-r--r--   0        0        0      532 2023-04-13 23:12:46.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/template_engine/protocols/code_renderer.py
+-rw-r--r--   0        0        0     3081 2023-08-07 16:13:48.162236 semantic_kernel-0.3.6.dev0/semantic_kernel/template_engine/protocols/prompt_templating_engine.py
+-rw-r--r--   0        0        0      596 2023-04-13 23:12:46.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/template_engine/protocols/text_renderer.py
+-rw-r--r--   0        0        0     7856 2023-08-07 16:13:48.162888 semantic_kernel-0.3.6.dev0/semantic_kernel/template_engine/template_tokenizer.py
+-rw-r--r--   0        0        0      473 2023-04-30 18:57:03.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/text/__init__.py
+-rw-r--r--   0        0        0      667 2023-04-30 18:57:03.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/text/function_extension.py
+-rw-r--r--   0        0        0     8568 2023-07-16 00:58:38.006510 semantic_kernel-0.3.6.dev0/semantic_kernel/text/text_chunker.py
+-rw-r--r--   0        0        0      403 2023-04-13 23:12:46.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/utils/null_logger.py
+-rw-r--r--   0        0        0     2570 2023-08-07 16:13:48.163472 semantic_kernel-0.3.6.dev0/semantic_kernel/utils/settings.py
+-rw-r--r--   0        0        0      221 2023-04-13 23:12:46.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/utils/static_property.py
+-rw-r--r--   0        0        0     2198 2023-04-13 23:12:46.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/utils/validation.py
+-rw-r--r--   0        0        0     1965 1970-01-01 00:00:00.000000 semantic_kernel-0.3.6.dev0/PKG-INFO
```

### Comparing `semantic_kernel-0.3.5.dev0/pip/README.md` & `semantic_kernel-0.3.6.dev0/pip/README.md`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.5.dev0/pyproject.toml` & `semantic_kernel-0.3.6.dev0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 [tool.poetry]
 name = "semantic-kernel"
-version = "0.3.5.dev"
+version = "0.3.6.dev"
 description = ""
 authors = ["Microsoft <SK-Support@microsoft.com>"]
 readme = "pip/README.md"
 packages = [{include = "semantic_kernel"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 numpy = "^1.24.2"
 openai = "^0.27.0"
 aiofiles = "^23.1.0"
 python-dotenv = "1.0.0"
 regex = "^2023.6.3"
+openapi_core = "^0.18.0"
+prance = "^23.6.21.0"
+pydantic = "<2"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "3.3.3"
 black = {version = "23.7.0", allow-prereleases = true}
 ipykernel = "^6.21.1"
 pytest = "7.4.0"
-ruff = "0.0.281"
+ruff = "0.0.282"
 pytest-asyncio = "0.21.1"
 
 [tool.poetry.group.hugging_face.dependencies]
 transformers = "^4.28.1"
 sentence-transformers = "^2.2.2"
 torch = "2.0.0"
```

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/__init__.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/ai/__init__.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/ai/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/ai/ai_exception.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/ai/ai_exception.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/ai/chat_completion_client_base.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/ai/chat_completion_client_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/ai/chat_request_settings.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/ai/chat_request_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/ai/complete_request_settings.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/ai/complete_request_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,17 @@
             import transformers
         except (ImportError, ModuleNotFoundError):
             raise ImportError(
                 "Please ensure that torch and transformers are installed to use HuggingFaceTextCompletion"
             )
 
         self.device = (
-            "cuda:" + device if device >= 0 and torch.cuda.is_available() else "cpu"
+            "cuda:" + str(device)
+            if device >= 0 and torch.cuda.is_available()
+            else "cpu"
         )
         self.generator = transformers.pipeline(
             task=self._task, model=self._model_id, device=self.device
         )
 
     async def complete_async(
         self, prompt: str, request_settings: CompleteRequestSettings
```

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/ai/open_ai/__init__.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/ai/open_ai/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,34 +48,39 @@
         self._api_key = api_key
         self._api_type = api_type
         self._api_version = api_version
         self._endpoint = endpoint
         self._org_id = org_id
         self._log = log if log is not None else NullLogger()
 
-    async def generate_embeddings_async(self, texts: List[str]) -> ndarray:
+    async def generate_embeddings_async(
+        self, texts: List[str], batch_size: Optional[int] = None
+    ) -> ndarray:
         model_args = {}
         if self._api_type in ["azure", "azure_ad"]:
             model_args["engine"] = self._model_id
         else:
             model_args["model"] = self._model_id
 
         try:
-            response: Any = await openai.Embedding.acreate(
-                **model_args,
-                api_key=self._api_key,
-                api_type=self._api_type,
-                api_base=self._endpoint,
-                api_version=self._api_version,
-                organization=self._org_id,
-                input=texts,
-            )
-
-            # make numpy arrays from the response
-            raw_embeddings = [array(x["embedding"]) for x in response["data"]]
+            raw_embeddings = []
+            batch_size = batch_size or len(texts)
+            for i in range(0, len(texts), batch_size):
+                batch = texts[i : i + batch_size]
+                response: Any = await openai.Embedding.acreate(
+                    **model_args,
+                    api_key=self._api_key,
+                    api_type=self._api_type,
+                    api_base=self._endpoint,
+                    api_version=self._api_version,
+                    organization=self._org_id,
+                    input=batch,
+                )
+                # make numpy arrays from the response
+                raw_embeddings.extend([array(x["embedding"]) for x in response["data"]])
             return array(raw_embeddings)
         except Exception as ex:
             raise AIException(
                 AIException.ErrorCodes.ServiceError,
                 "OpenAI service failed to generate embeddings",
                 ex,
             )
```

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/ai/text_completion_client_base.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/ai/text_completion_client_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/memory/azure_cognitive_search/azure_cognitive_search_memory_store.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/memory/azure_cognitive_search/azure_cognitive_search_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/memory/azure_cognitive_search/utils.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/memory/azure_cognitive_search/utils.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/memory/chroma/chroma_memory_store.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/memory/chroma/chroma_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/memory/chroma/utils.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/memory/chroma/utils.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/memory/milvus/milvus_memory_store.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/memory/milvus/milvus_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/memory/pinecone/pinecone_memory_store.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/memory/pinecone/pinecone_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/memory/pinecone/utils.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/memory/pinecone/utils.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/memory/postgres/postgres_memory_store.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/memory/postgres/postgres_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/memory/qdrant/qdrant_memory_store.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/memory/qdrant/qdrant_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/memory/weaviate/weaviate_memory_store.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/memory/weaviate/weaviate_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/search_engine/bing_connector.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/search_engine/bing_connector.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/search_engine/google_connector.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/search_engine/google_connector.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/core_skills/__init__.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/core_skills/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/core_skills/conversation_summary_skill.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/core_skills/conversation_summary_skill.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,29 +12,31 @@
     Semantic skill that enables conversations summarization.
     """
 
     # The max tokens to process in a single semantic function call.
     _max_tokens = 1024
 
     _summarize_conversation_prompt_template = (
-        "BEGIN CONTENT TO SUMMARIZE:\n"
-        "{{" + "$INPUT" + "}}\n"
-        "END CONTENT TO SUMMARIZE.\n"
-        "Summarize the conversation in 'CONTENT TO SUMMARIZE',\
-            identifying main points of discussion and any conclusions that were reached.\n"
-        "Do not incorporate other general knowledge.\n"
-        "Summary is in plain text, in complete sentences, with no markup or tags.\n"
-        "\nBEGIN SUMMARY:\n"
+        "BEGIN CONTENT TO SUMMARIZE:\n{{"
+        + "$INPUT"
+        + "}}\nEND CONTENT TO SUMMARIZE.\nSummarize the conversation in 'CONTENT TO"
+        " SUMMARIZE',            identifying main points of discussion and any"
+        " conclusions that were reached.\nDo not incorporate other general"
+        " knowledge.\nSummary is in plain text, in complete sentences, with no markup"
+        " or tags.\n\nBEGIN SUMMARY:\n"
     )
 
     def __init__(self, kernel: Kernel):
         self._summarizeConversationFunction = kernel.create_semantic_function(
             ConversationSummarySkill._summarize_conversation_prompt_template,
             skill_name=ConversationSummarySkill.__name__,
-            description="Given a section of a conversation transcript, summarize the part of the conversation.",
+            description=(
+                "Given a section of a conversation transcript, summarize the part of"
+                " the conversation."
+            ),
             max_tokens=ConversationSummarySkill._max_tokens,
             temperature=0.1,
             top_p=0.5,
         )
 
     @sk_function(
         description="Given a long conversation transcript, summarize the conversation.",
```

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/core_skills/file_io_skill.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/core_skills/file_io_skill.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import os
 
 import aiofiles
 
 from semantic_kernel.orchestration.sk_context import SKContext
+from semantic_kernel.sk_pydantic import PydanticField
 from semantic_kernel.skill_definition import sk_function, sk_function_context_parameter
 
 
-class FileIOSkill:
+class FileIOSkill(PydanticField):
     """
     Description: Read and write from a file.
 
     Usage:
         kernel.import_skill(FileIOSkill(), skill_name="file")
 
     Examples:
```

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/core_skills/http_skill.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/core_skills/http_skill.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import json
 
 import aiohttp
 
 from semantic_kernel.orchestration.sk_context import SKContext
+from semantic_kernel.sk_pydantic import PydanticField
 from semantic_kernel.skill_definition import sk_function, sk_function_context_parameter
 
 
-class HttpSkill:
+class HttpSkill(PydanticField):
     """
     A skill that provides HTTP functionality.
 
     Usage:
         kernel.import_skill(HttpSkill(), "http")
 
     Examples:
```

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/core_skills/math_skill.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/core_skills/math_skill.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 
 from semantic_kernel.orchestration.sk_context import SKContext
+from semantic_kernel.sk_pydantic import PydanticField
 from semantic_kernel.skill_definition import sk_function, sk_function_context_parameter
 
 
-class MathSkill:
+class MathSkill(PydanticField):
     """
     Description: MathSkill provides a set of functions to make Math calculations.
 
     Usage:
         kernel.import_skill(MathSkill(), skill_name="math")
 
     Examples:
@@ -73,14 +74,15 @@
 
         context_amount = context["Amount"]
         if context_amount is not None:
             try:
                 amount = int(context_amount)
             except ValueError:
                 raise ValueError(
-                    f"Context amount provided is not in numeric format: {context_amount}"
+                    "Context amount provided is not in numeric format:"
+                    f" {context_amount}"
                 )
 
             result = initial_value + amount if add else initial_value - amount
             return str(result)
         else:
             raise ValueError("Context amount should not be None.")
```

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/core_skills/text_memory_skill.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/core_skills/text_memory_skill.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 from semantic_kernel.orchestration.sk_context import SKContext
+from semantic_kernel.sk_pydantic import PydanticField
 from semantic_kernel.skill_definition import sk_function, sk_function_context_parameter
 
 
-class TextMemorySkill:
+class TextMemorySkill(PydanticField):
     COLLECTION_PARAM = "collection"
     RELEVANCE_PARAM = "relevance"
     KEY_PARAM = "key"
     DEFAULT_COLLECTION = "generic"
     DEFAULT_RELEVANCE = 0.75
 
     # @staticmethod
```

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/core_skills/text_skill.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/core_skills/text_skill.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Copyright (c) Microsoft. All rights reserved.
 
+from semantic_kernel.sk_pydantic import PydanticField
 from semantic_kernel.skill_definition import sk_function
 
 
-class TextSkill:
+class TextSkill(PydanticField):
     """
     TextSkill provides a set of functions to manipulate strings.
 
     Usage:
         kernel.import_skill(TextSkill(), skill_name="text")
 
     Examples:
```

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/core_skills/time_skill.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/core_skills/time_skill.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import datetime
 
+from semantic_kernel.sk_pydantic import PydanticField
 from semantic_kernel.skill_definition import sk_function
 
 
-class TimeSkill:
+class TimeSkill(PydanticField):
     """
     Description: TimeSkill provides a set of functions
                  to get the current time and date.
 
     Usage:
         kernel.import_skill(TimeSkill(), skill_name="time")
```

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/core_skills/wait_skill.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/core_skills/wait_skill.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import asyncio
 
+from semantic_kernel.sk_pydantic import PydanticField
 from semantic_kernel.skill_definition import sk_function
 
 
-class WaitSkill:
+class WaitSkill(PydanticField):
     """
     WaitSkill provides a set of functions to wait for a certain amount of time.
 
     Usage:
         kernel.import_skill(WaitSkill(), skill_name="wait")
 
     Examples:
```

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/core_skills/web_search_engine_skill.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/core_skills/web_search_engine_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/kernel.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/kernel.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import glob
 import importlib
 import inspect
 import os
 from logging import Logger
-from typing import Any, Callable, Dict, List, Optional, Type, TypeVar, Union, cast
+from typing import Any, Callable, Dict, List, Optional, Type, TypeVar, Union
 from uuid import uuid4
 
 from semantic_kernel.connectors.ai.ai_exception import AIException
 from semantic_kernel.connectors.ai.chat_completion_client_base import (
     ChatCompletionClientBase,
 )
 from semantic_kernel.connectors.ai.chat_request_settings import ChatRequestSettings
@@ -31,15 +31,14 @@
 from semantic_kernel.orchestration.sk_context import SKContext
 from semantic_kernel.orchestration.sk_function import SKFunction
 from semantic_kernel.orchestration.sk_function_base import SKFunctionBase
 from semantic_kernel.reliability.pass_through_without_retry import (
     PassThroughWithoutRetry,
 )
 from semantic_kernel.reliability.retry_mechanism_base import RetryMechanismBase
-from semantic_kernel.semantic_functions.chat_prompt_template import ChatPromptTemplate
 from semantic_kernel.semantic_functions.prompt_template import PromptTemplate
 from semantic_kernel.semantic_functions.prompt_template_config import (
     PromptTemplateConfig,
 )
 from semantic_kernel.semantic_functions.semantic_function_config import (
     SemanticFunctionConfig,
 )
@@ -148,14 +147,16 @@
             # run pipeline functions
             context = await self.run_async(
                 pipeline_functions, input_context, input_vars, input_str
             )
 
         elif len(functions) == 1:
             stream_function = functions[0]
+
+            # TODO: Preparing context for function invoke can be refactored as code below are same as run_async
             # if the user passed in a context, prioritize it, but merge with any other inputs
             if input_context is not None:
                 context = input_context
                 if input_vars is not None:
                     context._variables = input_vars.merge_or_overwrite(
                         new_vars=context._variables, overwrite=False
                     )
@@ -185,62 +186,32 @@
                     self._skill_collection.read_only_skill_collection,
                     self._log,
                 )
         else:
             raise ValueError("No functions passed to run")
 
         try:
-            client: ChatCompletionClientBase | TextCompletionClientBase
-            client = stream_function._ai_service
-
-            # Get the closure variables from function for finding function_config
-            closure_vars = stream_function._function.__closure__
-            for var in closure_vars:
-                if isinstance(var.cell_contents, SemanticFunctionConfig):
-                    function_config = var.cell_contents
-                    break
-
-            if function_config.has_chat_prompt:
-                as_chat_prompt = cast(
-                    ChatPromptTemplate, function_config.prompt_template
-                )
+            completion = ""
+            async for stream_message in stream_function.invoke_stream_async(
+                input=None, context=context
+            ):
+                completion += stream_message
+                yield stream_message
 
-                # Similar to non-chat, render prompt (which renders to a
-                # list of <role, content> messages)
-                completion = ""
-                messages = await as_chat_prompt.render_messages_async(context)
-                async for steam_message in client.complete_chat_stream_async(
-                    messages, stream_function._chat_request_settings
-                ):
-                    completion += steam_message
-                    yield steam_message
-
-                # Add the last message from the rendered chat prompt
-                # (which will be the user message) and the response
-                # from the model (the assistant message)
-                _, content = messages[-1]
-                as_chat_prompt.add_user_message(content)
-                as_chat_prompt.add_assistant_message(completion)
-
-                # Update context
-                context.variables.update(completion)
-
-            else:
-                completion = ""
-                prompt = await function_config.prompt_template.render_async(context)
-                async for stream_message in client.complete_stream_async(
-                    prompt, stream_function._ai_request_settings
-                ):
-                    completion += stream_message
-                    yield stream_message
-                context.variables.update(completion)
-
-        except Exception as e:
+        except Exception as ex:
             # TODO: "critical exceptions"
-            context.fail(str(e), e)
+            self._log.error(
+                f"Something went wrong in stream function."
+                f"During function invocation: '{stream_function.skill_name}.{stream_function.name}'. "
+                f"Error description: '{str(ex)}'"
+            )
+            raise KernelException(
+                KernelException.ErrorCodes.FunctionInvokeError,
+                "Error occurred while invoking stream function",
+            )
 
     async def run_async(
         self,
         *functions: Any,
         input_context: Optional[SKContext] = None,
         input_vars: Optional[ContextVariables] = None,
         input_str: Optional[str] = None,
@@ -365,16 +336,21 @@
         if skill_name.strip() == "":
             skill_name = SkillCollection.GLOBAL_SKILL
             self._log.debug(f"Importing skill {skill_name} into the global namespace")
         else:
             self._log.debug(f"Importing skill {skill_name}")
 
         functions = []
+
+        if isinstance(skill_instance, dict):
+            candidates = skill_instance.items()
+        else:
+            candidates = inspect.getmembers(skill_instance, inspect.ismethod)
         # Read every method from the skill instance
-        for _, candidate in inspect.getmembers(skill_instance, inspect.ismethod):
+        for _, candidate in candidates:
             # If the method is a semantic function, register it
             if not hasattr(candidate, "__sk_function__"):
                 continue
 
             functions.append(
                 SKFunction.from_native_method(candidate, skill_name, self.logger)
             )
```

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/kernel_exception.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/kernel_exception.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/memory/memory_query_result.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/memory/memory_query_result.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/memory/memory_record.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/memory/memory_record.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/memory/memory_store_base.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/memory/memory_store_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/memory/null_memory.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/memory/null_memory.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/memory/semantic_text_memory.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/memory/semantic_text_memory.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/memory/semantic_text_memory_base.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/memory/semantic_text_memory_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/memory/volatile_memory_store.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/memory/volatile_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/orchestration/context_variables.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/orchestration/context_variables.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/orchestration/delegate_handlers.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/orchestration/delegate_handlers.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/orchestration/delegate_inference.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/orchestration/delegate_inference.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/orchestration/delegate_types.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/orchestration/delegate_types.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/orchestration/sk_context.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/orchestration/sk_context.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/orchestration/sk_function.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/orchestration/sk_function.py`

 * *Files 13% similar despite different names*

```diff
@@ -75,25 +75,29 @@
 
                 parameters.append(
                     ParameterView(
                         param["name"], param["description"], param["default_value"]
                     )
                 )
 
-        if hasattr(method, "__sk_function_input_description__"):
+        if (
+            hasattr(method, "__sk_function_input_description__")
+            and method.__sk_function_input_description__ is not None
+        ):
             input_param = ParameterView(
                 "input",
                 method.__sk_function_input_description__,
                 method.__sk_function_input_default_value__,
             )
             parameters = [input_param] + parameters
 
         return SKFunction(
             delegate_type=DelegateInference.infer_delegate_type(method),
             delegate_function=method,
+            delegate_stream_function=method,
             parameters=parameters,
             description=method.__sk_function_description__,
             skill_name=skill_name,
             function_name=method.__sk_function_name__,
             is_semantic=False,
             log=log,
         )
@@ -140,17 +144,61 @@
                     context.variables.update(completion)
             except Exception as e:
                 # TODO: "critical exceptions"
                 context.fail(str(e), e)
 
             return context
 
+        async def _local_stream_func(client, request_settings, context):
+            if client is None:
+                raise ValueError("AI LLM service cannot be `None`")
+
+            try:
+                if function_config.has_chat_prompt:
+                    as_chat_prompt = cast(
+                        ChatPromptTemplate, function_config.prompt_template
+                    )
+
+                    # Similar to non-chat, render prompt (which renders to a
+                    # list of <role, content> messages)
+                    completion = ""
+                    messages = await as_chat_prompt.render_messages_async(context)
+                    async for steam_message in client.complete_chat_stream_async(
+                        messages, request_settings
+                    ):
+                        completion += steam_message
+                        yield steam_message
+
+                    # Add the last message from the rendered chat prompt
+                    # (which will be the user message) and the response
+                    # from the model (the assistant message)
+                    _, content = messages[-1]
+                    as_chat_prompt.add_user_message(content)
+                    as_chat_prompt.add_assistant_message(completion)
+
+                    # Update context
+                    context.variables.update(completion)
+                else:
+                    prompt = await function_config.prompt_template.render_async(context)
+
+                    completion = ""
+                    async for stream_message in client.complete_stream_async(
+                        prompt, request_settings
+                    ):
+                        completion += stream_message
+                        yield stream_message
+                    context.variables.update(completion)
+            except Exception as e:
+                # TODO: "critical exceptions"
+                context.fail(str(e), e)
+
         return SKFunction(
             delegate_type=DelegateTypes.ContextSwitchInSKContextOutTaskSKContext,
             delegate_function=_local_func,
+            delegate_stream_function=_local_stream_func,
             parameters=function_config.prompt_template.get_parameters(),
             description=function_config.prompt_template_config.description,
             skill_name=skill_name,
             function_name=function_name,
             is_semantic=True,
             log=log,
         )
@@ -189,23 +237,25 @@
         delegate_function: Callable[..., Any],
         parameters: List[ParameterView],
         description: str,
         skill_name: str,
         function_name: str,
         is_semantic: bool,
         log: Optional[Logger] = None,
+        delegate_stream_function: Optional[Callable[..., Any]] = None,
     ) -> None:
         self._delegate_type = delegate_type
         self._function = delegate_function
         self._parameters = parameters
         self._description = description
         self._skill_name = skill_name
         self._name = function_name
         self._is_semantic = is_semantic
         self._log = log if log is not None else NullLogger()
+        self._stream_function = delegate_stream_function
         self._skill_collection = None
         self._ai_service = None
         self._ai_request_settings = CompleteRequestSettings()
         self._chat_service = None
         self._chat_request_settings = ChatRequestSettings()
 
     def set_default_skill_collection(
@@ -408,14 +458,86 @@
 
         self._log.error("The function is not native")
         raise KernelException(
             KernelException.ErrorCodes.InvalidFunctionType,
             "Invalid operation, the method requires a native function",
         )
 
+    async def invoke_stream_async(
+        self,
+        input: Optional[str] = None,
+        variables: ContextVariables = None,
+        context: Optional[SKContext] = None,
+        memory: Optional[SemanticTextMemoryBase] = None,
+        settings: Optional[CompleteRequestSettings] = None,
+        log: Optional[Logger] = None,
+    ):
+        if context is None:
+            context = SKContext(
+                variables=ContextVariables("") if variables is None else variables,
+                skill_collection=self._skill_collection,
+                memory=memory if memory is not None else NullMemory.instance,
+                logger=log if log is not None else self._log,
+            )
+        else:
+            # If context is passed, we need to merge the variables
+            if variables is not None:
+                context._variables = variables.merge_or_overwrite(
+                    new_vars=context._variables, overwrite=False
+                )
+            if memory is not None:
+                context._memory = memory
+
+        if input is not None:
+            context.variables.update(input)
+
+        try:
+            if self.is_semantic:
+                async for stream_msg in self._invoke_semantic_stream_async(
+                    context, settings
+                ):
+                    yield stream_msg
+            else:
+                async for stream_msg in self._invoke_native_stream_async(context):
+                    yield stream_msg
+        except Exception as e:
+            context.fail(str(e), e)
+            raise KernelException(
+                KernelException.ErrorCodes.FunctionInvokeError,
+                "Error occurred while invoking stream function",
+            )
+
+    async def _invoke_semantic_stream_async(self, context, settings):
+        self._verify_is_semantic()
+
+        self._ensure_context_has_skills(context)
+
+        if settings is None:
+            if self._ai_service is not None:
+                settings = self._ai_request_settings
+            elif self._chat_service is not None:
+                settings = self._chat_request_settings
+            else:
+                raise KernelException(
+                    KernelException.ErrorCodes.UnknownError,
+                    "Semantic functions must have either an AI service or Chat service",
+                )
+
+        service = (
+            self._ai_service if self._ai_service is not None else self._chat_service
+        )
+
+        async for stream_msg in self._stream_function(service, settings, context):
+            yield stream_msg
+
+    async def _invoke_native_stream_async(self, context):
+        result = await self._invoke_native_async(context)
+
+        yield result
+
     def _ensure_context_has_skills(self, context) -> None:
         if context.skills is not None:
             return
 
         context.skills = self._skill_collection
 
     def _trace_function_type_Call(self, type: Enum, log: Logger) -> None:
```

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/orchestration/sk_function_base.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/orchestration/sk_function_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 # Copyright (c) Microsoft. All rights reserved.
 
-from abc import ABC, abstractmethod
+from abc import abstractmethod
 from logging import Logger
-from typing import TYPE_CHECKING, Callable, Optional
+from typing import TYPE_CHECKING, Callable, Optional, TypeVar
 
 from semantic_kernel.connectors.ai.complete_request_settings import (
     CompleteRequestSettings,
 )
 from semantic_kernel.connectors.ai.text_completion_client_base import (
     TextCompletionClientBase,
 )
 from semantic_kernel.memory.semantic_text_memory_base import SemanticTextMemoryBase
 from semantic_kernel.orchestration.context_variables import ContextVariables
 from semantic_kernel.orchestration.sk_context import SKContext
+from semantic_kernel.sk_pydantic import PydanticField
 from semantic_kernel.skill_definition.function_view import FunctionView
 
 if TYPE_CHECKING:
     from semantic_kernel.skill_definition.read_only_skill_collection_base import (
         ReadOnlySkillCollectionBase,
     )
 
 
-class SKFunctionBase(ABC):
+SKFunctionT = TypeVar("SKFunctionT", bound="SKFunctionBase")
+
+
+class SKFunctionBase(PydanticField):
     FUNCTION_PARAM_NAME_REGEX = r"^[0-9A-Za-z_]*$"
     FUNCTION_NAME_REGEX = r"^[0-9A-Za-z_]*$"
     SKILL_NAME_REGEX = r"^[0-9A-Za-z_]*$"
 
     @property
     @abstractmethod
     def name(self) -> str:
```

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/planning/action_planner/action_planner.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/planning/action_planner/action_planner.py`

 * *Files 0% similar despite different names*

```diff
@@ -138,24 +138,26 @@
                 "No suitable function has been identified by ActionPlanner."
             )
             plan = Plan(description=goal)
         elif "." in generated_plan["plan"]["function"]:
             skill, fun = generated_plan["plan"]["function"].split(".")
             function_ref = self._context.skills.get_function(skill, fun)
             self._logger.info(
-                f"ActionPlanner has picked {skill}.{fun}. Reference to this function found in context: {function_ref}"
+                f"ActionPlanner has picked {skill}.{fun}. Reference to this function"
+                f" found in context: {function_ref}"
             )
             plan = Plan(description=goal, function=function_ref)
         else:
             function_ref = self._context.skills.get_function(
                 generated_plan["plan"]["function"]
             )
             self._logger.info(
-                f"ActionPlanner has picked {generated_plan['plan']['function']}. \
-                    Reference to this function found in context: {function_ref}"
+                f"ActionPlanner has picked {generated_plan['plan']['function']}.       "
+                "              Reference to this function found in context:"
+                f" {function_ref}"
             )
             plan = Plan(description=goal, function=function_ref)
 
         for key, val in generated_plan["plan"]["parameters"].items():
             self._logger.info(f"Parameter {key}: val")
             if val:
                 plan.parameters[key] = str(val)
@@ -249,21 +251,21 @@
                 message="Suitable plan not generated by ActionPlanner.",
                 inner_exception=ValueError("No plugins are available."),
             )
 
         functions_view = context.skills.get_functions_view()
         available_functions = []
 
-        for functions in functions_view._native_functions.values():
+        for functions in functions_view.native_functions.values():
             for func in functions:
                 if func.skill_name.lower() == self._skill_name.lower():
                     continue
                 available_functions.append(self._create_function_string(func))
 
-        for functions in functions_view._semantic_functions.values():
+        for functions in functions_view.semantic_functions.values():
             for func in functions:
                 if func.skill_name.lower() == self._skill_name.lower():
                     continue
                 available_functions.append(self._create_function_string(func))
 
         available_functions_str = "\n".join(available_functions)
```

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/planning/basic_planner.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/planning/basic_planner.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,16 +115,16 @@
 
     def _create_available_functions_string(self, kernel: Kernel) -> str:
         """
         Given an instance of the Kernel, create the [AVAILABLE FUNCTIONS]
         string for the prompt.
         """
         # Get a dictionary of skill names to all native and semantic functions
-        native_functions = kernel.skills.get_functions_view()._native_functions
-        semantic_functions = kernel.skills.get_functions_view()._semantic_functions
+        native_functions = kernel.skills.get_functions_view().native_functions
+        semantic_functions = kernel.skills.get_functions_view().semantic_functions
         native_functions.update(semantic_functions)
 
         # Create a mapping between all function names and their descriptions
         # and also a mapping between function names and their parameters
         all_functions = native_functions
         skill_names = list(all_functions.keys())
         all_functions_descriptions_dict = {}
```

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/planning/plan.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/planning/plan.py`

 * *Files 1% similar despite different names*

```diff
@@ -389,15 +389,15 @@
         step_variables = ContextVariables(input_string)
 
         # Priority for remaining stepVariables is:
         # - Function Parameters (pull from variables or state by a key value)
         # - Step Parameters (pull from variables or state by a key value)
         # - All other variables. These are carried over in case the function wants access to the ambient content.
         function_params = step.describe()
-        for param in function_params._parameters:
+        for param in function_params.parameters:
             if param.name.lower() == variables._main_key.lower():
                 continue
 
             if variables.contains_key(param.name):
                 step_variables.set(param.name, variables[param.name])
             elif self._state.contains_key(param.name) and (
                 self._state[param.name] is not None and self._state[param.name] != ""
```

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/planning/planning_exception.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/planning/planning_exception.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/planning/sequential_planner/Skills/SequentialPlanning/config.json` & `semantic_kernel-0.3.6.dev0/semantic_kernel/planning/sequential_planner/Skills/SequentialPlanning/config.json`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/planning/sequential_planner/Skills/SequentialPlanning/skprompt.txt` & `semantic_kernel-0.3.6.dev0/semantic_kernel/planning/sequential_planner/Skills/SequentialPlanning/skprompt.txt`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/planning/sequential_planner/sequential_planner.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/planning/sequential_planner/sequential_planner.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/planning/sequential_planner/sequential_planner_config.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/planning/sequential_planner/sequential_planner_config.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/planning/sequential_planner/sequential_planner_extensions.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/planning/sequential_planner/sequential_planner_extensions.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,29 +27,35 @@
         ]
 
         inputs = "\n".join(inputs)
         qualified_name = SequentialPlannerFunctionViewExtension.to_fully_qualified_name(
             function
         )
 
-        return f"{qualified_name}:\n  description: {function.description}\n  inputs:\n  {inputs}"
+        return (
+            f"{qualified_name}:\n  description: {function.description}\n  inputs:\n "
+            f" {inputs}"
+        )
 
     @staticmethod
     def to_fully_qualified_name(function: FunctionView):
         return f"{function.skill_name}.{function.name}"
 
     @staticmethod
     def to_embedding_string(function: FunctionView):
         inputs = "\n".join(
             [
                 f"    - {parameter.name}: {parameter.description}"
                 for parameter in function.parameters
             ]
         )
-        return f"{function.name}:\n  description: {function.description}\n  inputs:\n{inputs}"
+        return (
+            f"{function.name}:\n  description: {function.description}\n "
+            f" inputs:\n{inputs}"
+        )
 
 
 class SequentialPlannerSKContextExtension:
     PLANNER_MEMORY_COLLECTION_NAME = " Planning.SKFunctionManual"
     PLAN_SK_FUNCTIONS_ARE_REMEMBERED = "Planning.SKFunctionsAreRemembered"
 
     @staticmethod
@@ -93,16 +99,16 @@
                 KernelException.ErrorCodes.SkillCollectionNotSet,
                 "Skill collection not found in the context",
             )
 
         functions_view = context.skills.get_functions_view()
 
         available_functions: List[FunctionView] = [
-            *functions_view._semantic_functions.values(),
-            *functions_view._native_functions.values(),
+            *functions_view.semantic_functions.values(),
+            *functions_view.native_functions.values(),
         ]
         available_functions = itertools.chain.from_iterable(available_functions)
 
         available_functions = [
             func
             for func in available_functions
             if (
```

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/planning/sequential_planner/sequential_planner_parser.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/planning/sequential_planner/sequential_planner_parser.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/reliability/pass_through_without_retry.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/reliability/pass_through_without_retry.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import logging
 from typing import Awaitable, Callable, TypeVar
 
 from semantic_kernel.reliability.retry_mechanism_base import RetryMechanismBase
+from semantic_kernel.sk_pydantic import PydanticField
 
 T = TypeVar("T")
 
 
-class PassThroughWithoutRetry(RetryMechanismBase):
+class PassThroughWithoutRetry(RetryMechanismBase, PydanticField):
     """A retry mechanism that does not retry."""
 
     async def execute_with_retry_async(
         self, action: Callable[[], Awaitable[T]], log: logging.Logger
     ) -> Awaitable[T]:
         """Executes the given action with retry logic.
```

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/reliability/retry_mechanism_base.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/reliability/retry_mechanism_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/semantic_functions/chat_prompt_template.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/semantic_functions/chat_prompt_template.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/semantic_functions/prompt_template.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/semantic_functions/prompt_template.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/semantic_functions/prompt_template_config.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/semantic_functions/prompt_template_config.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/semantic_functions/semantic_function_config.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/semantic_functions/semantic_function_config.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/skill_definition/functions_view.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/skill_definition/functions_view.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,59 +1,62 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 from typing import Dict, List
 
+import pydantic as pdt
+
 from semantic_kernel.kernel_exception import KernelException
+from semantic_kernel.sk_pydantic import SKBaseModel
 from semantic_kernel.skill_definition.function_view import FunctionView
 
 
-class FunctionsView:
-    _semantic_functions: Dict[str, List[FunctionView]]
-    _native_functions: Dict[str, List[FunctionView]]
-
-    def __init__(self) -> None:
-        self._semantic_functions = {}
-        self._native_functions = {}
+class FunctionsView(SKBaseModel):
+    semantic_functions: Dict[str, List[FunctionView]] = pdt.Field(default_factory=dict)
+    native_functions: Dict[str, List[FunctionView]] = pdt.Field(default_factory=dict)
 
     def add_function(self, view: FunctionView) -> "FunctionsView":
         if view.is_semantic:
-            if view.skill_name not in self._semantic_functions:
-                self._semantic_functions[view.skill_name] = []
-            self._semantic_functions[view.skill_name].append(view)
+            if view.skill_name not in self.semantic_functions:
+                self.semantic_functions[view.skill_name] = []
+            self.semantic_functions[view.skill_name].append(view)
         else:
-            if view.skill_name not in self._native_functions:
-                self._native_functions[view.skill_name] = []
-            self._native_functions[view.skill_name].append(view)
+            if view.skill_name not in self.native_functions:
+                self.native_functions[view.skill_name] = []
+            self.native_functions[view.skill_name].append(view)
 
         return self
 
     def is_semantic(self, skill_name: str, function_name: str) -> bool:
-        as_sf = self._semantic_functions.get(skill_name, [])
+        as_sf = self.semantic_functions.get(skill_name, [])
         as_sf = any(f.name == function_name for f in as_sf)
 
-        as_nf = self._native_functions.get(skill_name, [])
+        as_nf = self.native_functions.get(skill_name, [])
         as_nf = any(f.name == function_name for f in as_nf)
 
         if as_sf and as_nf:
             raise KernelException(
                 KernelException.ErrorCodes.AmbiguousImplementation,
-                f"There are 2 functions with the same name: {function_name}."
-                f"One is native and the other semantic.",
+                (
+                    f"There are 2 functions with the same name: {function_name}."
+                    "One is native and the other semantic."
+                ),
             )
 
         return as_sf
 
     def is_native(self, skill_name: str, function_name: str) -> bool:
-        as_sf = self._semantic_functions.get(skill_name, [])
+        as_sf = self.semantic_functions.get(skill_name, [])
         as_sf = any(f.name == function_name for f in as_sf)
 
-        as_nf = self._native_functions.get(skill_name, [])
+        as_nf = self.native_functions.get(skill_name, [])
         as_nf = any(f.name == function_name for f in as_nf)
 
         if as_sf and as_nf:
             raise KernelException(
                 KernelException.ErrorCodes.AmbiguousImplementation,
-                f"There are 2 functions with the same name: {function_name}."
-                f"One is native and the other semantic.",
+                (
+                    f"There are 2 functions with the same name: {function_name}."
+                    "One is native and the other semantic."
+                ),
             )
 
         return as_nf
```

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/skill_definition/read_only_skill_collection.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/skill_definition/read_only_skill_collection_base.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,56 +1,52 @@
 # Copyright (c) Microsoft. All rights reserved.
 
+from abc import ABC, abstractmethod
 from typing import TYPE_CHECKING, Optional
 
-from semantic_kernel.skill_definition.read_only_skill_collection_base import (
-    ReadOnlySkillCollectionBase,
-)
+from semantic_kernel.sk_pydantic import PydanticField
 
 if TYPE_CHECKING:
     from semantic_kernel.orchestration.sk_function_base import SKFunctionBase
     from semantic_kernel.skill_definition.functions_view import FunctionsView
-    from semantic_kernel.skill_definition.skill_collection_base import (
-        SkillCollectionBase,
-    )
 
 
-class ReadOnlySkillCollection(ReadOnlySkillCollectionBase):
-    _skill_collection: "SkillCollectionBase"
-
-    def __init__(self, skill_collection: "SkillCollectionBase") -> None:
-        self._skill_collection = skill_collection
-
+class ReadOnlySkillCollectionBase(PydanticField, ABC):
+    @abstractmethod
     def has_function(self, skill_name: Optional[str], function_name: str) -> bool:
-        return self._skill_collection.has_function(skill_name, function_name)
+        pass
 
+    @abstractmethod
     def has_semantic_function(
         self, skill_name: Optional[str], function_name: str
     ) -> bool:
-        return self._skill_collection.has_semantic_function(skill_name, function_name)
+        pass
 
+    @abstractmethod
     def has_native_function(
         self, skill_name: Optional[str], function_name: str
     ) -> bool:
-        return self._skill_collection.has_native_function(skill_name, function_name)
+        pass
 
+    @abstractmethod
     def get_semantic_function(
         self, skill_name: Optional[str], function_name: str
     ) -> "SKFunctionBase":
-        return self._skill_collection.get_semantic_function(skill_name, function_name)
+        pass
 
+    @abstractmethod
     def get_native_function(
         self, skill_name: Optional[str], function_name: str
     ) -> "SKFunctionBase":
-        return self._skill_collection.get_native_function(skill_name, function_name)
+        pass
 
+    @abstractmethod
     def get_functions_view(
         self, include_semantic: bool = True, include_native: bool = True
     ) -> "FunctionsView":
-        return self._skill_collection.get_functions_view(
-            include_semantic, include_native
-        )
+        pass
 
+    @abstractmethod
     def get_function(
         self, skill_name: Optional[str], function_name: str
     ) -> "SKFunctionBase":
-        return self._skill_collection.get_function(skill_name, function_name)
+        pass
```

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/skill_definition/sk_function_context_parameter_decorator.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/skill_definition/sk_function_context_parameter_decorator.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 # Copyright (c) Microsoft. All rights reserved.
 
-from typing import Optional
-
 
 def sk_function_context_parameter(
-    *, name: str, description: str, default_value: Optional[str] = None
+    *, name: str, description: str, default_value: str = ""
 ):
     """
     Decorator for SK function context parameters.
 
     Args:
         name -- The name of the context parameter
         description -- The description of the context parameter
```

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/skill_definition/sk_function_decorator.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/skill_definition/sk_function_decorator.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 
 def sk_function(
     *,
     description: str = "",
-    name: str = None,
-    input_description: str = None,
-    input_default_value: str = None
+    name: str = "",
+    input_description: str = "",
+    input_default_value: str = "",
 ):
     """
     Decorator for SK functions.
 
     Args:
         description -- The description of the function
         name -- The name of the function
         input_description -- The description of the input
         input_default_value -- The default value of the input
     """
 
     def decorator(func):
         func.__sk_function__ = True
-        func.__sk_function_description__ = description
-        func.__sk_function_name__ = name if name else func.__name__
-        func.__sk_function_input_description__ = input_description
-        func.__sk_function_input_default_value__ = input_default_value
+        func.__sk_function_description__ = description or ""
+        func.__sk_function_name__ = name or func.__name__
+        func.__sk_function_input_description__ = input_description or ""
+        func.__sk_function_input_default_value__ = input_default_value or ""
         return func
 
     return decorator
```

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/template_engine/README.md` & `semantic_kernel-0.3.6.dev0/semantic_kernel/template_engine/README.md`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/template_engine/blocks/code_block.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/template_engine/blocks/code_block.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 from logging import Logger
 from typing import List, Optional, Tuple
 
+import pydantic as pdt
+
 from semantic_kernel.orchestration.sk_function_base import SKFunctionBase
 from semantic_kernel.skill_definition.read_only_skill_collection_base import (
     ReadOnlySkillCollectionBase,
 )
 from semantic_kernel.template_engine.blocks.block import Block
 from semantic_kernel.template_engine.blocks.block_types import BlockTypes
 from semantic_kernel.template_engine.blocks.function_id_block import FunctionIdBlock
 from semantic_kernel.template_engine.code_tokenizer import CodeTokenizer
-from semantic_kernel.template_engine.protocols.code_renderer import CodeRenderer
 
 
-class CodeBlock(Block, CodeRenderer):
+class CodeBlock(Block):
+    _tokens: List[Block] = pdt.PrivateAttr()
+    _validated: bool = pdt.PrivateAttr(default=False)
+
     def __init__(
         self,
         content: str,
         tokens: Optional[List[Block]] = None,
         log: Optional[Logger] = None,
     ):
         super().__init__(content=content and content.strip(), log=log)
```

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/template_engine/blocks/text_block.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/template_engine/blocks/text_block.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,25 +2,27 @@
 
 from logging import Logger
 from typing import Optional, Tuple
 
 from semantic_kernel.orchestration.context_variables import ContextVariables
 from semantic_kernel.template_engine.blocks.block import Block
 from semantic_kernel.template_engine.blocks.block_types import BlockTypes
-from semantic_kernel.template_engine.protocols.text_renderer import TextRenderer
 
 
-class TextBlock(Block, TextRenderer):
-    def __init__(
-        self,
+class TextBlock(Block):
+    @classmethod
+    def from_text(
+        cls,
         text: Optional[str] = None,
         start_index: Optional[int] = None,
         stop_index: Optional[int] = None,
         log: Optional[Logger] = None,
     ):
+        if text is None:
+            return cls(content="", log=log)
         if start_index is not None and stop_index is not None:
             if start_index > stop_index:
                 raise ValueError(
                     f"start_index ({start_index}) must be less than "
                     f"stop_index ({stop_index})"
                 )
 
@@ -29,15 +31,15 @@
 
             text = text[start_index:stop_index]
         elif start_index is not None:
             text = text[start_index:]
         elif stop_index is not None:
             text = text[:stop_index]
 
-        super().__init__(content=text, log=log)
+        return cls(content=text, log=log)
 
     @property
     def type(self) -> BlockTypes:
         return BlockTypes.TEXT
 
     def is_valid(self) -> Tuple[bool, str]:
         return True, ""
```

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/template_engine/blocks/val_block.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/template_engine/blocks/val_block.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 from logging import Logger
 from typing import Optional, Tuple
 
+import pydantic as pdt
+
 from semantic_kernel.orchestration.context_variables import ContextVariables
 from semantic_kernel.template_engine.blocks.block import Block
 from semantic_kernel.template_engine.blocks.block_types import BlockTypes
 from semantic_kernel.template_engine.blocks.symbols import Symbols
-from semantic_kernel.template_engine.protocols.text_renderer import TextRenderer
 
 
-class ValBlock(Block, TextRenderer):
+class ValBlock(Block):
+    _first: str = pdt.PrivateAttr()
+    _last: str = pdt.PrivateAttr()
+    _value: str = pdt.PrivateAttr()
+
     def __init__(self, content: Optional[str] = None, log: Optional[Logger] = None):
         super().__init__(content=content and content.strip(), log=log)
 
         if len(self.content) < 2:
             err = "A value must have single quotes or double quotes on both sides"
             self.log.error(err)
             self._value = ""
```

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/template_engine/blocks/var_block.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/template_engine/blocks/var_block.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,47 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 from logging import Logger
 from re import match as re_match
 from typing import Optional, Tuple
 
+import pydantic as pdt
+
 from semantic_kernel.orchestration.context_variables import ContextVariables
 from semantic_kernel.template_engine.blocks.block import Block
 from semantic_kernel.template_engine.blocks.block_types import BlockTypes
 from semantic_kernel.template_engine.blocks.symbols import Symbols
-from semantic_kernel.template_engine.protocols.text_renderer import TextRenderer
 
 
-class VarBlock(Block, TextRenderer):
+class VarBlock(Block):
+    _name: str = pdt.PrivateAttr()
+
     def __init__(self, content: Optional[str] = None, log: Optional[Logger] = None):
         super().__init__(content=content and content.strip(), log=log)
 
         if len(self.content) < 2:
             err = "The variable name is empty"
             self.log.error(err)
-            self.name = ""
+            self._name = ""
             return
 
-        self.name = self.content[1:]
+        self._name = self.content[1:]
 
     @property
     def type(self) -> BlockTypes:
         return BlockTypes.VARIABLE
 
+    @property
+    def name(self) -> str:
+        return self._name
+
+    @name.setter
+    def name(self, value: str) -> None:
+        self._name = value
+
     def is_valid(self) -> Tuple[bool, str]:
         if not self.content:
             error_msg = (
                 f"A variable must start with the symbol {Symbols.VAR_PREFIX} "
                 "and have a name"
             )
             self.log.error(error_msg)
```

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/template_engine/code_tokenizer.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/template_engine/code_tokenizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 from logging import Logger
 from typing import List
 
+from semantic_kernel.sk_pydantic import PydanticField
 from semantic_kernel.template_engine.blocks.block import Block
 from semantic_kernel.template_engine.blocks.block_types import BlockTypes
 from semantic_kernel.template_engine.blocks.function_id_block import FunctionIdBlock
 from semantic_kernel.template_engine.blocks.symbols import Symbols
 from semantic_kernel.template_engine.blocks.val_block import ValBlock
 from semantic_kernel.template_engine.blocks.var_block import VarBlock
 from semantic_kernel.utils.null_logger import NullLogger
@@ -16,15 +17,15 @@
 # [template]       ::= "" | [variable] " " [template]
 #                         | [value] " " [template]
 #                         | [function-call] " " [template]
 # [variable]       ::= "$" [valid-name]
 # [value]          ::= "'" [text] "'" | '"' [text] '"'
 # [function-call]  ::= [function-id] | [function-id] [parameter]
 # [parameter]      ::= [variable] | [value]
-class CodeTokenizer:
+class CodeTokenizer(PydanticField):
     def __init__(self, log: Logger = None):
         self.log = log or NullLogger()
 
     def tokenize(self, text: str) -> List[Block]:
         # Remove spaces, which are ignored anyway
         text = text.strip() if text else ""
```

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/template_engine/prompt_template_engine.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/template_engine/prompt_template_engine.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 from logging import Logger
 from typing import List, Optional
 
 from semantic_kernel.orchestration.context_variables import ContextVariables
 from semantic_kernel.orchestration.sk_context import SKContext
+from semantic_kernel.sk_pydantic import PydanticField
 from semantic_kernel.template_engine.blocks.block import Block
 from semantic_kernel.template_engine.blocks.block_types import BlockTypes
 from semantic_kernel.template_engine.blocks.text_block import TextBlock
 from semantic_kernel.template_engine.protocols.code_renderer import CodeRenderer
-from semantic_kernel.template_engine.protocols.prompt_templating_engine import (
-    PromptTemplatingEngine,
-)
 from semantic_kernel.template_engine.protocols.text_renderer import TextRenderer
 from semantic_kernel.template_engine.template_tokenizer import TemplateTokenizer
 from semantic_kernel.utils.null_logger import NullLogger
 
 
-class PromptTemplateEngine(PromptTemplatingEngine):
+class PromptTemplateEngine(PydanticField):
     def __init__(self, logger: Optional[Logger] = None) -> None:
         self._logger = logger or NullLogger()
         self._tokenizer = TemplateTokenizer(self._logger)
 
     def extract_blocks(
         self, template_text: Optional[str] = None, validate: bool = True
     ) -> List[Block]:
@@ -103,15 +101,17 @@
         rendered_blocks = []
         for block in blocks:
             if block.type != BlockTypes.VARIABLE:
                 rendered_blocks.append(block)
                 continue
             if not isinstance(block, TextRenderer):
                 raise ValueError("TextBlock must implement TextRenderer protocol")
-            rendered_blocks.append(TextBlock(block.render(variables), log=self._logger))
+            rendered_blocks.append(
+                TextBlock.from_text(block.render(variables), log=self._logger)
+            )
 
         return rendered_blocks
 
     async def render_code_async(
         self, blocks: List[Block], execution_context: SKContext
     ) -> List[Block]:
         """
@@ -129,13 +129,13 @@
         for block in blocks:
             if block.type != BlockTypes.CODE:
                 rendered_blocks.append(block)
                 continue
             if not isinstance(block, CodeRenderer):
                 raise ValueError("CodeBlock must implement CodeRenderer protocol")
             rendered_blocks.append(
-                TextBlock(
+                TextBlock.from_text(
                     await block.render_code_async(execution_context), log=self._logger
                 )
             )
 
         return rendered_blocks
```

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/template_engine/protocols/code_renderer.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/template_engine/protocols/code_renderer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/template_engine/protocols/prompt_templating_engine.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/template_engine/protocols/prompt_templating_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # Copyright (c) Microsoft. All rights reserved.
 
-from typing import List, Optional, Protocol
+from typing import List, Optional, Protocol, runtime_checkable
 
 from semantic_kernel.orchestration.context_variables import ContextVariables
 from semantic_kernel.orchestration.sk_context import SKContext
 from semantic_kernel.template_engine.blocks.block import Block
 
 
+@runtime_checkable
 class PromptTemplatingEngine(Protocol):
     """
     Prompt templating engine protocol.
     """
 
     def extract_blocks(
         self, template_text: Optional[str] = None, validate: bool = True
```

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/template_engine/protocols/text_renderer.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/template_engine/protocols/text_renderer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/template_engine/template_tokenizer.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/template_engine/template_tokenizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 from logging import Logger
 from typing import List
 
+from semantic_kernel.sk_pydantic import PydanticField
 from semantic_kernel.template_engine.blocks.block import Block
 from semantic_kernel.template_engine.blocks.block_types import BlockTypes
 from semantic_kernel.template_engine.blocks.code_block import CodeBlock
 from semantic_kernel.template_engine.blocks.symbols import Symbols
 from semantic_kernel.template_engine.blocks.text_block import TextBlock
 from semantic_kernel.template_engine.code_tokenizer import CodeTokenizer
 from semantic_kernel.utils.null_logger import NullLogger
@@ -16,15 +17,15 @@
 # [template]       ::= "" | [block] | [block] [template]
 # [block]          ::= [sk-block] | [text-block]
 # [sk-block]       ::= "{{" [variable] "}}"
 #                      | "{{" [value] "}}"
 #                      | "{{" [function-call] "}}"
 # [text-block]     ::= [any-char] | [any-char] [text-block]
 # [any-char]       ::= any char
-class TemplateTokenizer:
+class TemplateTokenizer(PydanticField):
     def __init__(self, log: Logger = None):
         self.log = log or NullLogger()
         self.code_tokenizer = CodeTokenizer(self.log)
 
     def tokenize(self, text: str) -> List[Block]:
         # An empty block consists of 4 chars: "{{}}"
         EMPTY_CODE_BLOCK_LENGTH = 4
@@ -32,19 +33,19 @@
         # invalid, e.g. "{{ }}" and "{{$}}"
         MIN_CODE_BLOCK_LENGTH = EMPTY_CODE_BLOCK_LENGTH + 1
 
         text = text or ""
 
         # Render None/empty to ""
         if not text or text == "":
-            return [TextBlock("", log=self.log)]
+            return [TextBlock.from_text("", log=self.log)]
 
         # If the template is "empty" return it as a text block
         if len(text) < MIN_CODE_BLOCK_LENGTH:
-            return [TextBlock(text, log=self.log)]
+            return [TextBlock.from_text(text, log=self.log)]
 
         blocks = []
         end_of_last_block = 0
         block_start_pos = 0
         block_start_found = False
         inside_text_value = False
         text_value_delimiter = None
@@ -95,15 +96,15 @@
                         and next_char == Symbols.BLOCK_ENDER
                     ):
                         # If there is plain text between the current
                         # var/val/code block and the previous one,
                         # add it as a text block
                         if block_start_pos > end_of_last_block:
                             blocks.append(
-                                TextBlock(
+                                TextBlock.from_text(
                                     text,
                                     end_of_last_block,
                                     block_start_pos,
                                     log=self.log,
                                 )
                             )
 
@@ -114,15 +115,17 @@
                             2:-2
                         ].strip()
 
                         if len(content_without_delimiters) == 0:
                             # If what is left is empty, consider the raw block
                             # a TextBlock
                             blocks.append(
-                                TextBlock(content_with_delimiters, log=self.log)
+                                TextBlock.from_text(
+                                    content_with_delimiters, log=self.log
+                                )
                             )
                         else:
                             code_blocks = self.code_tokenizer.tokenize(
                                 content_without_delimiters
                             )
 
                             first_block_type = code_blocks[0].type
@@ -164,15 +167,17 @@
                                 )
 
                         end_of_last_block = cursor + 1
                         block_start_found = False
 
         # If there is something left after the last block, capture it as a TextBlock
         if end_of_last_block < len(text):
-            blocks.append(TextBlock(text, end_of_last_block, len(text), log=self.log))
+            blocks.append(
+                TextBlock.from_text(text, end_of_last_block, len(text), log=self.log)
+            )
 
         return blocks
 
     def _can_be_escaped(self, c: str) -> bool:
         return c in (
             Symbols.DBL_QUOTE,
             Symbols.SGL_QUOTE,
```

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/text/function_extension.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/text/function_extension.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/text/text_chunker.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/text/text_chunker.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/utils/settings.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/utils/settings.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         Tuple[str, str]: The OpenAI API key, the OpenAI organization ID
     """
 
     config = dotenv_values(".env")
     api_key = config.get("OPENAI_API_KEY", None)
     org_id = config.get("OPENAI_ORG_ID", None)
 
-    assert api_key is not None, "OpenAI API key not found in .env file"
+    assert api_key, "OpenAI API key not found in .env file"
 
     # It's okay if the org ID is not found (not required)
     return api_key, org_id
 
 
 def azure_openai_settings_from_dot_env(include_deployment=True) -> Tuple[str, str, str]:
     """
@@ -36,37 +36,33 @@
     config = dotenv_values(".env")
     deployment = config.get("AZURE_OPENAI_DEPLOYMENT_NAME", None)
     api_key = config.get("AZURE_OPENAI_API_KEY", None)
     endpoint = config.get("AZURE_OPENAI_ENDPOINT", None)
 
     # Azure requires the deployment name, the API key and the endpoint URL.
     if include_deployment:
-        assert (
-            deployment is not None
-        ), "Azure OpenAI deployment name not found in .env file"
+        assert deployment, "Azure OpenAI deployment name not found in .env file"
 
-    assert api_key is not None, "Azure OpenAI API key not found in .env file"
-    assert endpoint is not None, "Azure OpenAI endpoint not found in .env file"
+    assert api_key, "Azure OpenAI API key not found in .env file"
+    assert endpoint, "Azure OpenAI endpoint not found in .env file"
 
     return deployment or "", api_key, endpoint
 
 
 def postgres_settings_from_dot_env() -> str:
     """Reads the Postgres connection string from the .env file.
 
     Returns:
         str: The Postgres connection string
     """
     connection_string = None
     config = dotenv_values(".env")
     connection_string = config.get("POSTGRES_CONNECTION_STRING", None)
 
-    assert (
-        connection_string is not None
-    ), "Postgres connection string not found in .env file"
+    assert connection_string, "Postgres connection string not found in .env file"
 
     return connection_string
 
 
 def pinecone_settings_from_dot_env() -> Tuple[str, str]:
     """Reads the Pinecone API key and Environment from the .env file.
 
@@ -75,11 +71,11 @@
     """
 
     api_key, environment = None, None
     config = dotenv_values(".env")
     api_key = config.get("PINECONE_API_KEY", None)
     environment = config.get("PINECONE_ENVIRONMENT", None)
 
-    assert api_key is not None, "Pinecone API key not found in .env file"
-    assert environment is not None, "Pinecone environment not found in .env file"
+    assert api_key, "Pinecone API key not found in .env file"
+    assert environment, "Pinecone environment not found in .env file"
 
     return api_key, environment
```

### Comparing `semantic_kernel-0.3.5.dev0/semantic_kernel/utils/validation.py` & `semantic_kernel-0.3.6.dev0/semantic_kernel/utils/validation.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.5.dev0/PKG-INFO` & `semantic_kernel-0.3.6.dev0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 Metadata-Version: 2.1
 Name: semantic-kernel
-Version: 0.3.5.dev0
+Version: 0.3.6.dev0
 Summary: 
 Author: Microsoft
 Author-email: SK-Support@microsoft.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiofiles (>=23.1.0,<24.0.0)
 Requires-Dist: numpy (>=1.24.2,<2.0.0)
 Requires-Dist: openai (>=0.27.0,<0.28.0)
+Requires-Dist: openapi_core (>=0.18.0,<0.19.0)
+Requires-Dist: prance (>=23.6.21.0,<24.0.0.0)
+Requires-Dist: pydantic (<2)
 Requires-Dist: python-dotenv (==1.0.0)
 Requires-Dist: regex (>=2023.6.3,<2024.0.0)
 Description-Content-Type: text/markdown
 
 # About Semantic Kernel
 
 **Semantic Kernel (SK)** is a lightweight SDK enabling integration of AI Large
```

