# Comparing `tmp/promptulate-1.2.2.tar.gz` & `tmp/promptulate-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\promptulate-1.2.2.tar", last modified: Fri Jul 14 07:45:15 2023, max compression
+gzip compressed data, was "promptulate-1.3.0.tar", last modified: Mon Aug  7 19:29:11 2023, max compression
```

## Comparing `promptulate-1.2.2.tar` & `promptulate-1.3.0.tar`

### file list

```diff
@@ -1,86 +1,100 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 07:45:15.000000 promptulate-1.2.2/
--rw-rw-rw-   0        0        0    11558 2023-07-14 07:44:45.000000 promptulate-1.2.2/LICENSE
--rw-rw-rw-   0        0        0     7959 2023-07-14 07:45:15.000000 promptulate-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     7035 2023-07-14 07:44:45.000000 promptulate-1.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-14 07:45:14.000000 promptulate-1.2.2/promptulate/
--rw-rw-rw-   0        0        0     1115 2023-07-14 07:44:45.000000 promptulate-1.2.2/promptulate/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 07:45:15.000000 promptulate-1.2.2/promptulate/agents/
--rw-rw-rw-   0        0        0        0 2023-07-14 07:44:45.000000 promptulate-1.2.2/promptulate/agents/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 07:45:15.000000 promptulate-1.2.2/promptulate/client/
--rw-rw-rw-   0        0        0        0 2023-07-14 07:44:45.000000 promptulate-1.2.2/promptulate/client/__init__.py
--rw-rw-rw-   0        0        0     1757 2023-07-14 07:44:45.000000 promptulate-1.2.2/promptulate/client/chat.py
-drwxrwxrwx   0        0        0        0 2023-07-14 07:45:15.000000 promptulate-1.2.2/promptulate/command/
--rw-rw-rw-   0        0        0      127 2023-07-14 07:44:45.000000 promptulate-1.2.2/promptulate/command/__init__.py
--rw-rw-rw-   0        0        0     4438 2023-07-14 07:44:45.000000 promptulate-1.2.2/promptulate/config.py
-drwxrwxrwx   0        0        0        0 2023-07-14 07:45:15.000000 promptulate-1.2.2/promptulate/frameworks/
--rw-rw-rw-   0        0        0      878 2023-07-14 07:44:45.000000 promptulate-1.2.2/promptulate/frameworks/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 07:45:15.000000 promptulate-1.2.2/promptulate/frameworks/chain/
--rw-rw-rw-   0        0        0        0 2023-07-14 07:44:45.000000 promptulate-1.2.2/promptulate/frameworks/chain/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 07:45:15.000000 promptulate-1.2.2/promptulate/frameworks/conversation/
--rw-rw-rw-   0        0        0      890 2023-07-14 07:44:45.000000 promptulate-1.2.2/promptulate/frameworks/conversation/__init__.py
--rw-rw-rw-   0        0        0     4731 2023-07-14 07:44:45.000000 promptulate-1.2.2/promptulate/frameworks/conversation/conversation.py
--rw-rw-rw-   0        0        0     1780 2023-07-14 07:44:45.000000 promptulate-1.2.2/promptulate/frameworks/prompt.py
-drwxrwxrwx   0        0        0        0 2023-07-14 07:45:15.000000 promptulate-1.2.2/promptulate/frameworks/react/
--rw-rw-rw-   0        0        0      773 2023-07-14 07:44:45.000000 promptulate-1.2.2/promptulate/frameworks/react/__init__.py
--rw-rw-rw-   0        0        0     1152 2023-07-14 07:44:45.000000 promptulate-1.2.2/promptulate/frameworks/schema.py
-drwxrwxrwx   0        0        0        0 2023-07-14 07:45:15.000000 promptulate-1.2.2/promptulate/frameworks/self_ask/
--rw-rw-rw-   0        0        0      773 2023-07-14 07:44:45.000000 promptulate-1.2.2/promptulate/frameworks/self_ask/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 07:45:15.000000 promptulate-1.2.2/promptulate/llms/
--rw-rw-rw-   0        0        0      869 2023-07-14 07:44:45.000000 promptulate-1.2.2/promptulate/llms/__init__.py
--rw-rw-rw-   0        0        0     1392 2023-07-14 07:44:45.000000 promptulate-1.2.2/promptulate/llms/base.py
--rw-rw-rw-   0        0        0     9567 2023-07-14 07:44:45.000000 promptulate-1.2.2/promptulate/llms/openai.py
-drwxrwxrwx   0        0        0        0 2023-07-14 07:45:15.000000 promptulate-1.2.2/promptulate/memory/
--rw-rw-rw-   0        0        0      948 2023-07-14 07:44:45.000000 promptulate-1.2.2/promptulate/memory/__init__.py
--rw-rw-rw-   0        0        0     2379 2023-07-14 07:44:45.000000 promptulate-1.2.2/promptulate/memory/base.py
--rw-rw-rw-   0        0        0     2161 2023-07-14 07:44:45.000000 promptulate-1.2.2/promptulate/memory/buffer.py
--rw-rw-rw-   0        0        0     2294 2023-07-14 07:44:45.000000 promptulate-1.2.2/promptulate/memory/file.py
-drwxrwxrwx   0        0        0        0 2023-07-14 07:45:15.000000 promptulate-1.2.2/promptulate/preset_roles/
--rw-rw-rw-   0        0        0      929 2023-07-14 07:44:45.000000 promptulate-1.2.2/promptulate/preset_roles/__init__.py
--rw-rw-rw-   0        0        0     2762 2023-07-14 07:44:45.000000 promptulate-1.2.2/promptulate/preset_roles/prompt.py
--rw-rw-rw-   0        0        0     5004 2023-07-14 07:44:45.000000 promptulate-1.2.2/promptulate/preset_roles/roles.py
-drwxrwxrwx   0        0        0        0 2023-07-14 07:45:15.000000 promptulate-1.2.2/promptulate/provider/
--rw-rw-rw-   0        0        0     1063 2023-07-14 07:44:45.000000 promptulate-1.2.2/promptulate/provider/__init__.py
--rw-rw-rw-   0        0        0      683 2023-07-14 07:44:45.000000 promptulate-1.2.2/promptulate/provider/base.py
--rw-rw-rw-   0        0        0     4839 2023-07-14 07:44:45.000000 promptulate-1.2.2/promptulate/provider/mixins.py
--rw-rw-rw-   0        0        0     4763 2023-07-14 07:44:45.000000 promptulate-1.2.2/promptulate/schema.py
--rw-rw-rw-   0        0        0     1184 2023-07-14 07:44:45.000000 promptulate-1.2.2/promptulate/tips.py
-drwxrwxrwx   0        0        0        0 2023-07-14 07:45:15.000000 promptulate-1.2.2/promptulate/tools/
--rw-rw-rw-   0        0        0        0 2023-07-14 07:44:45.000000 promptulate-1.2.2/promptulate/tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 07:45:15.000000 promptulate-1.2.2/promptulate/tools/arxiv/
--rw-rw-rw-   0        0        0      268 2023-07-14 07:44:45.000000 promptulate-1.2.2/promptulate/tools/arxiv/__init__.py
--rw-rw-rw-   0        0        0     4917 2023-07-14 07:44:45.000000 promptulate-1.2.2/promptulate/tools/arxiv/api_wrapper.py
--rw-rw-rw-   0        0        0      393 2023-07-14 07:44:45.000000 promptulate-1.2.2/promptulate/tools/arxiv/toolkit.py
--rw-rw-rw-   0        0        0     9808 2023-07-14 07:44:45.000000 promptulate-1.2.2/promptulate/tools/arxiv/tools.py
--rw-rw-rw-   0        0        0      592 2023-07-14 07:44:45.000000 promptulate-1.2.2/promptulate/tools/base.py
-drwxrwxrwx   0        0        0        0 2023-07-14 07:45:15.000000 promptulate-1.2.2/promptulate/tools/duckduckgo/
--rw-rw-rw-   0        0        0      161 2023-07-14 07:44:45.000000 promptulate-1.2.2/promptulate/tools/duckduckgo/__init__.py
--rw-rw-rw-   0        0        0     3476 2023-07-14 07:44:45.000000 promptulate-1.2.2/promptulate/tools/duckduckgo/api_wrapper.py
--rw-rw-rw-   0        0        0     3543 2023-07-14 07:44:45.000000 promptulate-1.2.2/promptulate/tools/duckduckgo/tools.py
-drwxrwxrwx   0        0        0        0 2023-07-14 07:45:15.000000 promptulate-1.2.2/promptulate/tools/paper/
--rw-rw-rw-   0        0        0       94 2023-07-14 07:44:45.000000 promptulate-1.2.2/promptulate/tools/paper/__init__.py
--rw-rw-rw-   0        0        0     7410 2023-07-14 07:44:45.000000 promptulate-1.2.2/promptulate/tools/paper/tools.py
-drwxrwxrwx   0        0        0        0 2023-07-14 07:45:15.000000 promptulate-1.2.2/promptulate/tools/python_repl/
--rw-rw-rw-   0        0        0      104 2023-07-14 07:44:45.000000 promptulate-1.2.2/promptulate/tools/python_repl/__init__.py
--rw-rw-rw-   0        0        0      826 2023-07-14 07:44:45.000000 promptulate-1.2.2/promptulate/tools/python_repl/api_wrapper.py
--rw-rw-rw-   0        0        0      723 2023-07-14 07:44:45.000000 promptulate-1.2.2/promptulate/tools/python_repl/tools.py
-drwxrwxrwx   0        0        0        0 2023-07-14 07:45:15.000000 promptulate-1.2.2/promptulate/tools/semantic_scholar/
--rw-rw-rw-   0        0        0      283 2023-07-14 07:44:45.000000 promptulate-1.2.2/promptulate/tools/semantic_scholar/__init__.py
--rw-rw-rw-   0        0        0     6884 2023-07-14 07:44:45.000000 promptulate-1.2.2/promptulate/tools/semantic_scholar/api_wrapper.py
--rw-rw-rw-   0        0        0     2330 2023-07-14 07:44:45.000000 promptulate-1.2.2/promptulate/tools/semantic_scholar/tools.py
-drwxrwxrwx   0        0        0        0 2023-07-14 07:45:15.000000 promptulate-1.2.2/promptulate/utils/
--rw-rw-rw-   0        0        0     1580 2023-07-14 07:44:45.000000 promptulate-1.2.2/promptulate/utils/__init__.py
--rw-rw-rw-   0        0        0     3978 2023-07-14 07:44:45.000000 promptulate-1.2.2/promptulate/utils/core_utils.py
--rw-rw-rw-   0        0        0     1808 2023-07-14 07:44:45.000000 promptulate-1.2.2/promptulate/utils/logger.py
--rw-rw-rw-   0        0        0     4298 2023-07-14 07:44:45.000000 promptulate-1.2.2/promptulate/utils/openai_key_pool.py
--rw-rw-rw-   0        0        0     1632 2023-07-14 07:44:45.000000 promptulate-1.2.2/promptulate/utils/proxy.py
--rw-rw-rw-   0        0        0     1403 2023-07-14 07:44:45.000000 promptulate-1.2.2/promptulate/utils/singleton.py
--rw-rw-rw-   0        0        0      664 2023-07-14 07:44:45.000000 promptulate-1.2.2/promptulate/utils/string_template.py
-drwxrwxrwx   0        0        0        0 2023-07-14 07:45:15.000000 promptulate-1.2.2/promptulate.egg-info/
--rw-rw-rw-   0        0        0     7959 2023-07-14 07:45:14.000000 promptulate-1.2.2/promptulate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2048 2023-07-14 07:45:14.000000 promptulate-1.2.2/promptulate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 07:45:14.000000 promptulate-1.2.2/promptulate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       66 2023-07-14 07:45:14.000000 promptulate-1.2.2/promptulate.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       89 2023-07-14 07:45:14.000000 promptulate-1.2.2/promptulate.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-14 07:45:14.000000 promptulate-1.2.2/promptulate.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-14 07:45:15.000000 promptulate-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0     2297 2023-07-14 07:44:45.000000 promptulate-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:29:11.770931 promptulate-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-07 19:29:00.000000 promptulate-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7366 2023-08-07 19:29:11.766931 promptulate-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-08-07 19:29:00.000000 promptulate-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:29:11.758931 promptulate-1.3.0/promptulate/
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-08-07 19:29:00.000000 promptulate-1.3.0/promptulate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:29:11.762931 promptulate-1.3.0/promptulate/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-07 19:29:00.000000 promptulate-1.3.0/promptulate/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 19:29:00.000000 promptulate-1.3.0/promptulate/agents/auto_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:29:11.762931 promptulate-1.3.0/promptulate/agents/tool_agent/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-07 19:29:00.000000 promptulate-1.3.0/promptulate/agents/tool_agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-08-07 19:29:00.000000 promptulate-1.3.0/promptulate/agents/tool_agent/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-08-07 19:29:00.000000 promptulate-1.3.0/promptulate/agents/tool_agent/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:29:11.762931 promptulate-1.3.0/promptulate/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 19:29:00.000000 promptulate-1.3.0/promptulate/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-08-07 19:29:00.000000 promptulate-1.3.0/promptulate/client/chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-08-07 19:29:00.000000 promptulate-1.3.0/promptulate/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:29:11.762931 promptulate-1.3.0/promptulate/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-08-07 19:29:00.000000 promptulate-1.3.0/promptulate/frameworks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:29:11.762931 promptulate-1.3.0/promptulate/frameworks/chain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 19:29:00.000000 promptulate-1.3.0/promptulate/frameworks/chain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:29:11.762931 promptulate-1.3.0/promptulate/frameworks/conversation/
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-08-07 19:29:00.000000 promptulate-1.3.0/promptulate/frameworks/conversation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-08-07 19:29:00.000000 promptulate-1.3.0/promptulate/frameworks/conversation/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-08-07 19:29:00.000000 promptulate-1.3.0/promptulate/frameworks/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:29:11.762931 promptulate-1.3.0/promptulate/frameworks/react/
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-08-07 19:29:00.000000 promptulate-1.3.0/promptulate/frameworks/react/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-08-07 19:29:00.000000 promptulate-1.3.0/promptulate/frameworks/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:29:11.762931 promptulate-1.3.0/promptulate/frameworks/self_ask/
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-08-07 19:29:00.000000 promptulate-1.3.0/promptulate/frameworks/self_ask/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:29:11.762931 promptulate-1.3.0/promptulate/hook/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-07 19:29:00.000000 promptulate-1.3.0/promptulate/hook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7731 2023-08-07 19:29:00.000000 promptulate-1.3.0/promptulate/hook/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:29:11.762931 promptulate-1.3.0/promptulate/llms/
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-08-07 19:29:00.000000 promptulate-1.3.0/promptulate/llms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-08-07 19:29:00.000000 promptulate-1.3.0/promptulate/llms/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:29:11.762931 promptulate-1.3.0/promptulate/llms/openai/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-08-07 19:29:00.000000 promptulate-1.3.0/promptulate/llms/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9770 2023-08-07 19:29:00.000000 promptulate-1.3.0/promptulate/llms/openai/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-08-07 19:29:00.000000 promptulate-1.3.0/promptulate/llms/openai/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:29:11.762931 promptulate-1.3.0/promptulate/memory/
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-08-07 19:29:00.000000 promptulate-1.3.0/promptulate/memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-08-07 19:29:00.000000 promptulate-1.3.0/promptulate/memory/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-08-07 19:29:00.000000 promptulate-1.3.0/promptulate/memory/buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-08-07 19:29:00.000000 promptulate-1.3.0/promptulate/memory/file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:29:11.766931 promptulate-1.3.0/promptulate/preset_roles/
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-08-07 19:29:00.000000 promptulate-1.3.0/promptulate/preset_roles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-08-07 19:29:00.000000 promptulate-1.3.0/promptulate/preset_roles/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4916 2023-08-07 19:29:00.000000 promptulate-1.3.0/promptulate/preset_roles/roles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:29:11.766931 promptulate-1.3.0/promptulate/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-08-07 19:29:00.000000 promptulate-1.3.0/promptulate/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-08-07 19:29:00.000000 promptulate-1.3.0/promptulate/provider/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4707 2023-08-07 19:29:00.000000 promptulate-1.3.0/promptulate/provider/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-08-07 19:29:00.000000 promptulate-1.3.0/promptulate/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-08-07 19:29:00.000000 promptulate-1.3.0/promptulate/tips.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:29:11.766931 promptulate-1.3.0/promptulate/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-08-07 19:29:00.000000 promptulate-1.3.0/promptulate/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:29:11.766931 promptulate-1.3.0/promptulate/tools/arxiv/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-08-07 19:29:00.000000 promptulate-1.3.0/promptulate/tools/arxiv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-08-07 19:29:00.000000 promptulate-1.3.0/promptulate/tools/arxiv/api_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-08-07 19:29:00.000000 promptulate-1.3.0/promptulate/tools/arxiv/toolkit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9604 2023-08-07 19:29:00.000000 promptulate-1.3.0/promptulate/tools/arxiv/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-08-07 19:29:00.000000 promptulate-1.3.0/promptulate/tools/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:29:11.766931 promptulate-1.3.0/promptulate/tools/duckduckgo/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-08-07 19:29:00.000000 promptulate-1.3.0/promptulate/tools/duckduckgo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-08-07 19:29:00.000000 promptulate-1.3.0/promptulate/tools/duckduckgo/api_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-08-07 19:29:00.000000 promptulate-1.3.0/promptulate/tools/duckduckgo/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-08-07 19:29:00.000000 promptulate-1.3.0/promptulate/tools/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:29:11.766931 promptulate-1.3.0/promptulate/tools/math/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-07 19:29:00.000000 promptulate-1.3.0/promptulate/tools/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-08-07 19:29:00.000000 promptulate-1.3.0/promptulate/tools/math/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-08-07 19:29:00.000000 promptulate-1.3.0/promptulate/tools/math/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:29:11.766931 promptulate-1.3.0/promptulate/tools/paper/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-07 19:29:00.000000 promptulate-1.3.0/promptulate/tools/paper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7242 2023-08-07 19:29:00.000000 promptulate-1.3.0/promptulate/tools/paper/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:29:11.766931 promptulate-1.3.0/promptulate/tools/python_repl/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-08-07 19:29:00.000000 promptulate-1.3.0/promptulate/tools/python_repl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-07 19:29:00.000000 promptulate-1.3.0/promptulate/tools/python_repl/api_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-08-07 19:29:00.000000 promptulate-1.3.0/promptulate/tools/python_repl/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:29:11.766931 promptulate-1.3.0/promptulate/tools/semantic_scholar/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-08-07 19:29:00.000000 promptulate-1.3.0/promptulate/tools/semantic_scholar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-08-07 19:29:00.000000 promptulate-1.3.0/promptulate/tools/semantic_scholar/api_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-08-07 19:29:00.000000 promptulate-1.3.0/promptulate/tools/semantic_scholar/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:29:11.766931 promptulate-1.3.0/promptulate/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-08-07 19:29:00.000000 promptulate-1.3.0/promptulate/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-08-07 19:29:00.000000 promptulate-1.3.0/promptulate/utils/core_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-08-07 19:29:00.000000 promptulate-1.3.0/promptulate/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5461 2023-08-07 19:29:00.000000 promptulate-1.3.0/promptulate/utils/openai_key_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-08-07 19:29:00.000000 promptulate-1.3.0/promptulate/utils/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-08-07 19:29:00.000000 promptulate-1.3.0/promptulate/utils/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-08-07 19:29:00.000000 promptulate-1.3.0/promptulate/utils/string_template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:29:11.762931 promptulate-1.3.0/promptulate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7366 2023-08-07 19:29:11.000000 promptulate-1.3.0/promptulate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-08-07 19:29:11.000000 promptulate-1.3.0/promptulate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 19:29:11.000000 promptulate-1.3.0/promptulate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-07 19:29:11.000000 promptulate-1.3.0/promptulate.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-07 19:29:11.000000 promptulate-1.3.0/promptulate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-07 19:29:11.000000 promptulate-1.3.0/promptulate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 19:29:11.770931 promptulate-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-08-07 19:29:00.000000 promptulate-1.3.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `promptulate-1.2.2/LICENSE` & `promptulate-1.3.0/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `promptulate-1.2.2/PKG-INFO` & `promptulate-1.3.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,127 +1,123 @@
-Metadata-Version: 2.1
-Name: promptulate
-Version: 1.2.2
-Summary: A powerful LLM Application development framework.
-Home-page: https://github.com/Undertone0809/promptulate
-Author: Zeeland
-Author-email: zeeland@foxmail.com
-License: Apache 2.0
-Keywords: promptulate,prompt-me,prompt,chatgpt,gpt,chatbot,llm
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-<h1 align="center">
-    promptulate
-</h1>
-
-<p align="center">
-    <a target="_blank" href="">
-        <img src="https://img.shields.io/github/license/Undertone0809/promptulate.svg?style=flat-square" />
-    </a>
-    <a target="_blank" href=''>
-        <img src="https://img.shields.io/github/release/Undertone0809/promptulate/all.svg?style=flat-square"/>
-    </a>
-    <a target="_blank" href=''>
-        <img src="https://bestpractices.coreinfrastructure.org/projects/3018/badge"/>
-   </a>
-</p>
-
-<p align="center">
-  <img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/promptulate_logo_new.png"/>
-</p>
-
-
-`promptulate` 是一个专为Prompt工程师设计的大语言模型自动化与应用开发框架，支持智能决策、消息持久化、外部工具调用、角色预设等功能，开箱即用。
-通过 `promptulate`，你可以轻松构建起属于自己的LLM应用程序。
-
-`promptulate`旨在构建为开发者提供一种强大而灵活的平台，以创建能够自动化各种任务和应用程序的自主代理。通过Core
-AI Engine、Agent System、APIs and Tools Provider、Multimodal Processing、Knowledge Base和Task-specific Modules
-6个组件实现自动化AI平台。 Core AI Engine是该框架的核心组件，负责处理和理解各种输入，生成输出和作出决策。Agent
-System是提供高级指导和控制AI代理行为的模块；APIs and Tools Provider提供工具和服务交互的API和集成库；Multimodal
-Processing是一组处理和理解不同数据类型（如文本、图像、音频和视频）的模块，使用深度学习模型从不同数据模式中提取有意义的信息；Knowledge
-Base是一个存储和组织世界信息的大型结构化知识库，使AI代理能够访问和推理大量的知识；Task-specific
-Modules是一组专门设计用于执行特定任务的模块，例如情感分析、机器翻译或目标检测等。通过这些组件的组合，框架提供了一个全面、灵活和强大的平台，能够实现各种复杂任务和应用程序的自动化。
-
-
-# 特性
-
-- 大语言模型支持：支持不同类型的大语言模型的扩展接口
-- 对话终端：提供简易对话终端，直接体验与大语言模型的对话
-- 角色预设：提供预设角色，以不同的角度调用GPT
-- 长对话模式：支持长对话聊天，支持多种方式的对话持久化
-- 外部工具：集成外部工具能力，可以进行网络搜索、执行Python代码等强大的功能
-- KEY池：提供API key池，彻底解决key限速的问题
-- 智能代理：集成ReAct，self-ask等高级Agent，结合外部工具赋能LLM
-- 自治代理模式：支持调用API官方接口、自治代理或使用promptulate提供的代理
-- 中文优化：针对中文语境进行特别优化，更适合中文场景
-- 数据导出：支持markdowm等格式的对话导出
-- 对话总结：提供API式的对话总结、翻译、标题生成
-- 事件总线：自研总线机制，通过[broadcast-service](https://github.com/Undertone0809/broadcast-service)进行Planing与Action的并发调度
-- 高级抽象，支持插件扩展、存储扩展、大语言模型扩展
-
-# 快速开始
-
-- [快速上手 [github-pages]](https://undertone0809.github.io/promptulate/#/)
-- [快速上手 [gitee-pages]](https://zeeland.gitee.io/promptulate/#/)
-- [当前开发计划](https://undertone0809.github.io/promptulate/#/other/plan)
-- [参与贡献/开发者手册](https://undertone0809.github.io/promptulate/#/other/contribution)
-- [常见问题](https://undertone0809.github.io/promptulate/#/other/fqa)
-- [pypi仓库](https://pypi.org/project/promptulate/)
-
-# 基础架构
-
-在本人深度阅读`langchain, Auto-GPT, django, django-rest-framework, gpt_academic...`
-等项目的源码，参与pr之后，学习它们的架构、代码设计思路等内容，重构了两次，有了现在的版本，相较于之前的老版本`prompt-me`，`promptulate`
-重新构建了 `llms, message, memory, framework, preset_roles, tools, provider`等模块，将`prompt`
-的各个流程全部组件化，便有了现在的`promptualte`框架。当前`promptualte`仍有很多细节需要完善，也十分欢迎大家的讨论与参与。
-
-`promptualte`作为一个为大语言模型设计的Prompt Layer框架，主要由以下几部分组成：
-
-- `Agent` 更高级的执行器，负责复杂任务的调度和分发
-- `framework` 框架层，实现不同类型的prompt框架，包括最基础的`Conversation`模型，还有`self-ask`和`ReAct`等模型。
-- `llm` 大语言模型，负责生成回答，可以支持不同类型的大语言模型
-- `memory` 负责对话的存储，支持不同的存储方式及其扩展，如文件存储、数据库存储等
-- `tools` 提供外部工具扩展调用，如搜索引擎、计算器、编译器等
-- `preset roles` 提供预设角色，进行定制化对话
-- `provider` 为framework和agent提供tools和其他细粒度能力的集成
-
-<img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230704180202.png"/>
-
-# 设计原则
-
-promptulate框架的设计原则包括：模块化、可扩展性、互操作性、鲁棒性、可维护性、安全性、效率和可用性。
-
-- 模块化是指以模块为基本单位，允许方便地集成新的组件、模型和工具。
-- 可扩展性是指框架能够处理大量数据、复杂任务和高并发的能力。
-- 互操作性是指该框架与各种外部系统、工具和服务兼容，并且能够实现无缝集成和通信。
-- 鲁棒性是指框架具备强大的错误处理、容错和恢复机制，以确保在各种条件下可靠地运行。
-- 安全性是指框架采用了严格的安全措施，以保护框架、其数据和用户免受未经授权访问和恶意行为的侵害。
-- 效率是指优化框架的性能、资源使用和响应时间，以确保流畅和敏锐的用户体验。
-- 可用性是指该框架采用用户友好的界面和清晰的文档，使其易于使用和理解。
-
-以上原则的遵循，以及最新的人工智能技术的应用，`promptulate`旨在为创建自动化代理提供强大而灵活的大语言模型应用开发框架。
-
-# 交流群
-
-欢迎加入群聊一起交流讨论有关LLM相关的话题，链接过期了可以issue或email提醒一下作者。
-
-<div style="width: 250px;margin: 0 auto;">
-  <img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230702132948.png"/>
-</div>
-
-# 贡献
-
-本人正在尝试一些更加完善的抽象模式，以更好地兼容该框架，以及外部工具的扩展使用，如果你有更好的建议，欢迎一起讨论交流。
-如果你想为这个项目做贡献，请先查看[当前开发计划](https://undertone0809.github.io/promptulate/#/other/plan)
-和[参与贡献/开发者手册](https://undertone0809.github.io/promptulate/#/other/contribution)。我很高兴看到更多的人参与并优化它。
+Metadata-Version: 2.1
+Name: promptulate
+Version: 1.3.0
+Summary: A powerful LLM Application development framework.
+Home-page: https://github.com/Undertone0809/promptulate
+Author: Zeeland
+Author-email: zeeland@foxmail.com
+License: Apache 2.0
+Keywords: promptulate,prompt-me,prompt,chatgpt,gpt,chatbot,llm
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<h1 align="center">
+    promptulate
+</h1>
+
+<p align="center">
+    <a target="_blank" href="">
+        <img src="https://img.shields.io/github/license/Undertone0809/promptulate.svg?style=flat-square" />
+    </a>
+    <a target="_blank" href=''>
+        <img src="https://img.shields.io/github/release/Undertone0809/promptulate/all.svg?style=flat-square"/>
+    </a>
+    <a target="_blank" href=''>
+        <img src="https://bestpractices.coreinfrastructure.org/projects/3018/badge"/>
+   </a>
+</p>
+
+<p align="center">
+  <img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/promptulate_logo_new.png"/>
+</p>
+
+
+`promptulate` 是一个专为Prompt工程师设计的大语言模型自动化与应用开发框架，支持智能决策、消息持久化、外部工具调用、角色预设等功能，开箱即用。
+通过 `promptulate`，你可以轻松构建起属于自己的LLM应用程序。
+
+`promptulate`旨在构建为开发者提供一种强大而灵活的平台，以创建能够自动化各种任务和应用程序的自主代理。通过Core
+AI Engine、Agent System、APIs and Tools Provider、Multimodal Processing、Knowledge Base和Task-specific Modules
+6个组件实现自动化AI平台。 Core AI Engine是该框架的核心组件，负责处理和理解各种输入，生成输出和作出决策。Agent
+System是提供高级指导和控制AI代理行为的模块；APIs and Tools Provider提供工具和服务交互的API和集成库；Multimodal
+Processing是一组处理和理解不同数据类型（如文本、图像、音频和视频）的模块，使用深度学习模型从不同数据模式中提取有意义的信息；Knowledge
+Base是一个存储和组织世界信息的大型结构化知识库，使AI代理能够访问和推理大量的知识；Task-specific
+Modules是一组专门设计用于执行特定任务的模块，例如情感分析、机器翻译或目标检测等。通过这些组件的组合，框架提供了一个全面、灵活和强大的平台，能够实现各种复杂任务和应用程序的自动化。
+
+
+# 特性
+
+- 大语言模型支持：支持不同类型的大语言模型的扩展接口
+- 对话终端：提供简易对话终端，直接体验与大语言模型的对话
+- 角色预设：提供预设角色，以不同的角度调用GPT
+- 长对话模式：支持长对话聊天，支持多种方式的对话持久化
+- 外部工具：集成外部工具能力，可以进行网络搜索、执行Python代码等强大的功能
+- KEY池：提供API key池，彻底解决key限速的问题
+- 智能代理：集成ReAct，self-ask等高级Agent，结合外部工具赋能LLM
+- 自治代理模式：支持调用API官方接口、自治代理或使用promptulate提供的代理
+- 中文优化：针对中文语境进行特别优化，更适合中文场景
+- 数据导出：支持markdowm等格式的对话导出
+- Hook与生命周期：提供Agent，Tool，llm的生命周期及Hook系统
+- 高级抽象：支持插件扩展、存储扩展、大语言模型扩展
+
+# 快速开始
+
+- [快速上手 [github-pages]](https://undertone0809.github.io/promptulate/#/)
+- [快速上手 [gitee-pages]](https://zeeland.gitee.io/promptulate/#/)
+- [当前开发计划](https://undertone0809.github.io/promptulate/#/other/plan)
+- [参与贡献/开发者手册](https://undertone0809.github.io/promptulate/#/other/contribution)
+- [常见问题](https://undertone0809.github.io/promptulate/#/other/fqa)
+- [pypi仓库](https://pypi.org/project/promptulate/)
+
+# 基础架构
+
+当前`promptulate`正处于快速开发阶段，仍有许多内容需要完善与讨论，十分欢迎大家的讨论与参与，而其作为一个大语言模型自动化与应用开发框架，主要由以下几部分组成：
+
+- `Agent` 更高级的执行器，负责复杂任务的调度和分发
+- `llm` 大语言模型，负责生成回答，可以支持不同类型的大语言模型
+- `Memory` 负责对话的存储，支持不同的存储方式及其扩展，如文件存储、数据库存储等
+- `Framework` 框架层，实现不同类型的prompt框架，包括最基础的`Conversation`模型，还有`self-ask`和`ReAct`等模型。
+- `Tool` 提供外部工具扩展调用，如搜索引擎、计算器等
+- `Hook&Lifecycle` Hook系统与生命周期系统，开发者可以进行定制化的生命周期逻辑控制
+- `Rreset roles` 提供预设角色，进行定制化对话
+- `Provider` 为系统提供更多数据源或执行自主操作，如数据库的连接
+
+<img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230704180202.png"/>
+
+# 设计原则
+
+promptulate框架的设计原则包括：模块化、可扩展性、互操作性、鲁棒性、可维护性、安全性、效率和可用性。
+
+- 模块化是指以模块为基本单位，允许方便地集成新的组件、模型和工具。
+- 可扩展性是指框架能够处理大量数据、复杂任务和高并发的能力。
+- 互操作性是指该框架与各种外部系统、工具和服务兼容，并且能够实现无缝集成和通信。
+- 鲁棒性是指框架具备强大的错误处理、容错和恢复机制，以确保在各种条件下可靠地运行。
+- 安全性是指框架采用了严格的安全措施，以保护框架、其数据和用户免受未经授权访问和恶意行为的侵害。
+- 效率是指优化框架的性能、资源使用和响应时间，以确保流畅和敏锐的用户体验。
+- 可用性是指该框架采用用户友好的界面和清晰的文档，使其易于使用和理解。
+
+以上原则的遵循，以及最新的人工智能技术的应用，`promptulate`旨在为创建自动化代理提供强大而灵活的大语言模型应用开发框架。
+
+# 交流群
+
+欢迎加入群聊一起交流讨论有关LLM相关的话题，链接过期了可以issue或email提醒一下作者。
+
+<div style="width: 250px;margin: 0 auto;">
+  <img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230807173459.png"/>
+</div>
+
+
+# 贡献
+
+本人正在尝试一些更加完善的抽象模式，以更好地兼容该框架，以及外部工具的扩展使用，如果你有更好的建议，欢迎一起讨论交流。
+如果你想为这个项目做贡献，请先查看[当前开发计划](https://undertone0809.github.io/promptulate/#/other/plan)
+和[参与贡献/开发者手册](https://undertone0809.github.io/promptulate/#/other/contribution)。我很高兴看到更多的人参与并优化它。
```

### Comparing `promptulate-1.2.2/README.md` & `promptulate-1.3.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,104 +1,100 @@
-<h1 align="center">
-    promptulate
-</h1>
-
-<p align="center">
-    <a target="_blank" href="">
-        <img src="https://img.shields.io/github/license/Undertone0809/promptulate.svg?style=flat-square" />
-    </a>
-    <a target="_blank" href=''>
-        <img src="https://img.shields.io/github/release/Undertone0809/promptulate/all.svg?style=flat-square"/>
-    </a>
-    <a target="_blank" href=''>
-        <img src="https://bestpractices.coreinfrastructure.org/projects/3018/badge"/>
-   </a>
-</p>
-
-<p align="center">
-  <img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/promptulate_logo_new.png"/>
-</p>
-
-
-`promptulate` 是一个专为Prompt工程师设计的大语言模型自动化与应用开发框架，支持智能决策、消息持久化、外部工具调用、角色预设等功能，开箱即用。
-通过 `promptulate`，你可以轻松构建起属于自己的LLM应用程序。
-
-`promptulate`旨在构建为开发者提供一种强大而灵活的平台，以创建能够自动化各种任务和应用程序的自主代理。通过Core
-AI Engine、Agent System、APIs and Tools Provider、Multimodal Processing、Knowledge Base和Task-specific Modules
-6个组件实现自动化AI平台。 Core AI Engine是该框架的核心组件，负责处理和理解各种输入，生成输出和作出决策。Agent
-System是提供高级指导和控制AI代理行为的模块；APIs and Tools Provider提供工具和服务交互的API和集成库；Multimodal
-Processing是一组处理和理解不同数据类型（如文本、图像、音频和视频）的模块，使用深度学习模型从不同数据模式中提取有意义的信息；Knowledge
-Base是一个存储和组织世界信息的大型结构化知识库，使AI代理能够访问和推理大量的知识；Task-specific
-Modules是一组专门设计用于执行特定任务的模块，例如情感分析、机器翻译或目标检测等。通过这些组件的组合，框架提供了一个全面、灵活和强大的平台，能够实现各种复杂任务和应用程序的自动化。
-
-
-# 特性
-
-- 大语言模型支持：支持不同类型的大语言模型的扩展接口
-- 对话终端：提供简易对话终端，直接体验与大语言模型的对话
-- 角色预设：提供预设角色，以不同的角度调用GPT
-- 长对话模式：支持长对话聊天，支持多种方式的对话持久化
-- 外部工具：集成外部工具能力，可以进行网络搜索、执行Python代码等强大的功能
-- KEY池：提供API key池，彻底解决key限速的问题
-- 智能代理：集成ReAct，self-ask等高级Agent，结合外部工具赋能LLM
-- 自治代理模式：支持调用API官方接口、自治代理或使用promptulate提供的代理
-- 中文优化：针对中文语境进行特别优化，更适合中文场景
-- 数据导出：支持markdowm等格式的对话导出
-- 对话总结：提供API式的对话总结、翻译、标题生成
-- 事件总线：自研总线机制，通过[broadcast-service](https://github.com/Undertone0809/broadcast-service)进行Planing与Action的并发调度
-- 高级抽象，支持插件扩展、存储扩展、大语言模型扩展
-
-# 快速开始
-
-- [快速上手 [github-pages]](https://undertone0809.github.io/promptulate/#/)
-- [快速上手 [gitee-pages]](https://zeeland.gitee.io/promptulate/#/)
-- [当前开发计划](https://undertone0809.github.io/promptulate/#/other/plan)
-- [参与贡献/开发者手册](https://undertone0809.github.io/promptulate/#/other/contribution)
-- [常见问题](https://undertone0809.github.io/promptulate/#/other/fqa)
-- [pypi仓库](https://pypi.org/project/promptulate/)
-
-# 基础架构
-
-在本人深度阅读`langchain, Auto-GPT, django, django-rest-framework, gpt_academic...`
-等项目的源码，参与pr之后，学习它们的架构、代码设计思路等内容，重构了两次，有了现在的版本，相较于之前的老版本`prompt-me`，`promptulate`
-重新构建了 `llms, message, memory, framework, preset_roles, tools, provider`等模块，将`prompt`
-的各个流程全部组件化，便有了现在的`promptualte`框架。当前`promptualte`仍有很多细节需要完善，也十分欢迎大家的讨论与参与。
-
-`promptualte`作为一个为大语言模型设计的Prompt Layer框架，主要由以下几部分组成：
-
-- `Agent` 更高级的执行器，负责复杂任务的调度和分发
-- `framework` 框架层，实现不同类型的prompt框架，包括最基础的`Conversation`模型，还有`self-ask`和`ReAct`等模型。
-- `llm` 大语言模型，负责生成回答，可以支持不同类型的大语言模型
-- `memory` 负责对话的存储，支持不同的存储方式及其扩展，如文件存储、数据库存储等
-- `tools` 提供外部工具扩展调用，如搜索引擎、计算器、编译器等
-- `preset roles` 提供预设角色，进行定制化对话
-- `provider` 为framework和agent提供tools和其他细粒度能力的集成
-
-<img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230704180202.png"/>
-
-# 设计原则
-
-promptulate框架的设计原则包括：模块化、可扩展性、互操作性、鲁棒性、可维护性、安全性、效率和可用性。
-
-- 模块化是指以模块为基本单位，允许方便地集成新的组件、模型和工具。
-- 可扩展性是指框架能够处理大量数据、复杂任务和高并发的能力。
-- 互操作性是指该框架与各种外部系统、工具和服务兼容，并且能够实现无缝集成和通信。
-- 鲁棒性是指框架具备强大的错误处理、容错和恢复机制，以确保在各种条件下可靠地运行。
-- 安全性是指框架采用了严格的安全措施，以保护框架、其数据和用户免受未经授权访问和恶意行为的侵害。
-- 效率是指优化框架的性能、资源使用和响应时间，以确保流畅和敏锐的用户体验。
-- 可用性是指该框架采用用户友好的界面和清晰的文档，使其易于使用和理解。
-
-以上原则的遵循，以及最新的人工智能技术的应用，`promptulate`旨在为创建自动化代理提供强大而灵活的大语言模型应用开发框架。
-
-# 交流群
-
-欢迎加入群聊一起交流讨论有关LLM相关的话题，链接过期了可以issue或email提醒一下作者。
-
-<div style="width: 250px;margin: 0 auto;">
-  <img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230702132948.png"/>
-</div>
-
-# 贡献
-
-本人正在尝试一些更加完善的抽象模式，以更好地兼容该框架，以及外部工具的扩展使用，如果你有更好的建议，欢迎一起讨论交流。
-如果你想为这个项目做贡献，请先查看[当前开发计划](https://undertone0809.github.io/promptulate/#/other/plan)
-和[参与贡献/开发者手册](https://undertone0809.github.io/promptulate/#/other/contribution)。我很高兴看到更多的人参与并优化它。
+<h1 align="center">
+    promptulate
+</h1>
+
+<p align="center">
+    <a target="_blank" href="">
+        <img src="https://img.shields.io/github/license/Undertone0809/promptulate.svg?style=flat-square" />
+    </a>
+    <a target="_blank" href=''>
+        <img src="https://img.shields.io/github/release/Undertone0809/promptulate/all.svg?style=flat-square"/>
+    </a>
+    <a target="_blank" href=''>
+        <img src="https://bestpractices.coreinfrastructure.org/projects/3018/badge"/>
+   </a>
+</p>
+
+<p align="center">
+  <img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/promptulate_logo_new.png"/>
+</p>
+
+
+`promptulate` 是一个专为Prompt工程师设计的大语言模型自动化与应用开发框架，支持智能决策、消息持久化、外部工具调用、角色预设等功能，开箱即用。
+通过 `promptulate`，你可以轻松构建起属于自己的LLM应用程序。
+
+`promptulate`旨在构建为开发者提供一种强大而灵活的平台，以创建能够自动化各种任务和应用程序的自主代理。通过Core
+AI Engine、Agent System、APIs and Tools Provider、Multimodal Processing、Knowledge Base和Task-specific Modules
+6个组件实现自动化AI平台。 Core AI Engine是该框架的核心组件，负责处理和理解各种输入，生成输出和作出决策。Agent
+System是提供高级指导和控制AI代理行为的模块；APIs and Tools Provider提供工具和服务交互的API和集成库；Multimodal
+Processing是一组处理和理解不同数据类型（如文本、图像、音频和视频）的模块，使用深度学习模型从不同数据模式中提取有意义的信息；Knowledge
+Base是一个存储和组织世界信息的大型结构化知识库，使AI代理能够访问和推理大量的知识；Task-specific
+Modules是一组专门设计用于执行特定任务的模块，例如情感分析、机器翻译或目标检测等。通过这些组件的组合，框架提供了一个全面、灵活和强大的平台，能够实现各种复杂任务和应用程序的自动化。
+
+
+# 特性
+
+- 大语言模型支持：支持不同类型的大语言模型的扩展接口
+- 对话终端：提供简易对话终端，直接体验与大语言模型的对话
+- 角色预设：提供预设角色，以不同的角度调用GPT
+- 长对话模式：支持长对话聊天，支持多种方式的对话持久化
+- 外部工具：集成外部工具能力，可以进行网络搜索、执行Python代码等强大的功能
+- KEY池：提供API key池，彻底解决key限速的问题
+- 智能代理：集成ReAct，self-ask等高级Agent，结合外部工具赋能LLM
+- 自治代理模式：支持调用API官方接口、自治代理或使用promptulate提供的代理
+- 中文优化：针对中文语境进行特别优化，更适合中文场景
+- 数据导出：支持markdowm等格式的对话导出
+- Hook与生命周期：提供Agent，Tool，llm的生命周期及Hook系统
+- 高级抽象：支持插件扩展、存储扩展、大语言模型扩展
+
+# 快速开始
+
+- [快速上手 [github-pages]](https://undertone0809.github.io/promptulate/#/)
+- [快速上手 [gitee-pages]](https://zeeland.gitee.io/promptulate/#/)
+- [当前开发计划](https://undertone0809.github.io/promptulate/#/other/plan)
+- [参与贡献/开发者手册](https://undertone0809.github.io/promptulate/#/other/contribution)
+- [常见问题](https://undertone0809.github.io/promptulate/#/other/fqa)
+- [pypi仓库](https://pypi.org/project/promptulate/)
+
+# 基础架构
+
+当前`promptulate`正处于快速开发阶段，仍有许多内容需要完善与讨论，十分欢迎大家的讨论与参与，而其作为一个大语言模型自动化与应用开发框架，主要由以下几部分组成：
+
+- `Agent` 更高级的执行器，负责复杂任务的调度和分发
+- `llm` 大语言模型，负责生成回答，可以支持不同类型的大语言模型
+- `Memory` 负责对话的存储，支持不同的存储方式及其扩展，如文件存储、数据库存储等
+- `Framework` 框架层，实现不同类型的prompt框架，包括最基础的`Conversation`模型，还有`self-ask`和`ReAct`等模型。
+- `Tool` 提供外部工具扩展调用，如搜索引擎、计算器等
+- `Hook&Lifecycle` Hook系统与生命周期系统，开发者可以进行定制化的生命周期逻辑控制
+- `Rreset roles` 提供预设角色，进行定制化对话
+- `Provider` 为系统提供更多数据源或执行自主操作，如数据库的连接
+
+<img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230704180202.png"/>
+
+# 设计原则
+
+promptulate框架的设计原则包括：模块化、可扩展性、互操作性、鲁棒性、可维护性、安全性、效率和可用性。
+
+- 模块化是指以模块为基本单位，允许方便地集成新的组件、模型和工具。
+- 可扩展性是指框架能够处理大量数据、复杂任务和高并发的能力。
+- 互操作性是指该框架与各种外部系统、工具和服务兼容，并且能够实现无缝集成和通信。
+- 鲁棒性是指框架具备强大的错误处理、容错和恢复机制，以确保在各种条件下可靠地运行。
+- 安全性是指框架采用了严格的安全措施，以保护框架、其数据和用户免受未经授权访问和恶意行为的侵害。
+- 效率是指优化框架的性能、资源使用和响应时间，以确保流畅和敏锐的用户体验。
+- 可用性是指该框架采用用户友好的界面和清晰的文档，使其易于使用和理解。
+
+以上原则的遵循，以及最新的人工智能技术的应用，`promptulate`旨在为创建自动化代理提供强大而灵活的大语言模型应用开发框架。
+
+# 交流群
+
+欢迎加入群聊一起交流讨论有关LLM相关的话题，链接过期了可以issue或email提醒一下作者。
+
+<div style="width: 250px;margin: 0 auto;">
+  <img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230807173459.png"/>
+</div>
+
+
+# 贡献
+
+本人正在尝试一些更加完善的抽象模式，以更好地兼容该框架，以及外部工具的扩展使用，如果你有更好的建议，欢迎一起讨论交流。
+如果你想为这个项目做贡献，请先查看[当前开发计划](https://undertone0809.github.io/promptulate/#/other/plan)
+和[参与贡献/开发者手册](https://undertone0809.github.io/promptulate/#/other/contribution)。我很高兴看到更多的人参与并优化它。
```

### Comparing `promptulate-1.2.2/promptulate/__init__.py` & `promptulate-1.3.0/promptulate/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,35 @@
-# Copyright (c) 2023 promptulate
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-# Copyright Owner: Zeeland
-# GitHub Link: https://github.com/Undertone0809/
-# Project Link: https://github.com/Undertone0809/promptulate
-# Contact Email: zeeland@foxmail.com
-
-from promptulate.frameworks import Conversation
-from promptulate.schema import UserMessage, AssistantMessage, SystemMessage
-from promptulate.utils import enable_log, enable_log_no_file
-
-__all__ = [
-    "Conversation",
-    "enable_log",
-    "enable_log_no_file",
-    "SystemMessage",
-    "UserMessage",
-    "AssistantMessage",
-]
+# Copyright (c) 2023 promptulate
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+# Copyright Owner: Zeeland
+# GitHub Link: https://github.com/Undertone0809/
+# Project Link: https://github.com/Undertone0809/promptulate
+# Contact Email: zeeland@foxmail.com
+
+import warnings
+
+from promptulate.frameworks import Conversation
+from promptulate.schema import UserMessage, AssistantMessage, SystemMessage
+from promptulate.utils import enable_log, enable_log_no_file
+
+__all__ = [
+    "Conversation",
+    "enable_log",
+    "enable_log_no_file",
+    "SystemMessage",
+    "UserMessage",
+    "AssistantMessage",
+]
+
+warnings.filterwarnings("always", category=DeprecationWarning)
```

### Comparing `promptulate-1.2.2/promptulate/config.py` & `promptulate-1.3.0/promptulate/config.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,115 +1,116 @@
-# Copyright (c) 2023 promptulate
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-# Copyright Owner: Zeeland
-# GitHub Link: https://github.com/Undertone0809/
-# Project Link: https://github.com/Undertone0809/promptulate
-# Contact Email: zeeland@foxmail.com
-
-import os
-from typing import Optional
-
-from promptulate import utils
-from promptulate.utils.logger import get_logger
-from promptulate.utils.openai_key_pool import OpenAIKeyPool
-from promptulate.utils.singleton import Singleton
-
-PROXY_MODE = ["off", "custom", "promptulate"]
-logger = get_logger()
-
-
-def set_enable_cache(value: bool):
-    """Caching is enabled by default. Disabling caching is not recommended."""
-    Config().enable_cache = value
-
-
-class Config(metaclass=Singleton):
-    def __init__(self):
-        logger.info(f"[promptulate config] Config initialization")
-        self.enable_cache: bool = True
-        self._proxy_mode: str = PROXY_MODE[0]
-        self._proxies: Optional[dict] = None
-        self.openai_chat_api_url = "https://api.openai.com/v1/chat/completions"
-        self.openai_completion_api_url = "https://api.openai.com/v1/completions"
-        self.openai_proxy_url = "https://chatgpt-api.shn.hk/v1/"  # FREE API
-        self.key_default_retry_times = 5
-        """If llm(like OpenAI) unable to obtain data, retry request until the data is obtained."""
-
-    @property
-    def openai_api_key(self):
-        """This attribution has deprecated to use. Using `get_openai_api_key`"""
-        if "OPENAI_API_KEY" in os.environ.keys():
-            if self.enable_cache:
-                utils.get_cache()["OPENAI_API_KEY"] = os.getenv("OPENAI_API_KEY")
-            return os.getenv("OPENAI_API_KEY")
-        if self.enable_cache and "OPENAI_API_KEY" in utils.get_cache():
-            return utils.get_cache()["OPENAI_API_KEY"]
-        raise ValueError("OPENAI API key is not provided. Please set your key.")
-
-    def get_openai_api_key(self, model: str) -> str:
-        """Get openai key from KeyPool and environ"""
-        if self.enable_cache:
-            openai_key_pool: OpenAIKeyPool = OpenAIKeyPool()
-            key = openai_key_pool.get(model)
-            if key:
-                return key
-        return self.openai_api_key
-
-    def get_key_retry_times(self, model: str) -> int:
-        if self.enable_cache:
-            openai_key_pool: OpenAIKeyPool = OpenAIKeyPool()
-            return openai_key_pool.get_num(model)
-        return self.key_default_retry_times
-
-    @property
-    def proxy_mode(self) -> str:
-        if self.enable_cache and "PROXY_MODE" in utils.get_cache():
-            return utils.get_cache()["PROXY_MODE"]
-        return self._proxy_mode
-
-    @proxy_mode.setter
-    def proxy_mode(self, value):
-        self._proxy_mode = value
-        if self.enable_cache:
-            utils.get_cache()["PROXY_MODE"] = value
-
-    @property
-    def proxies(self) -> Optional[dict]:
-        if self.enable_cache and "PROXIES" in utils.get_cache():
-            return utils.get_cache()["PROXIES"] if self.proxy_mode == "custom" else None
-        return self._proxies
-
-    @proxies.setter
-    def proxies(self, value):
-        self._proxies = value
-        if self.enable_cache:
-            utils.get_cache()["PROXIES"] = value
-
-    @property
-    def openai_chat_request_url(self) -> str:
-        if self.proxy_mode == PROXY_MODE[2]:
-            self.proxies = None
-            return self.openai_proxy_url
-        return self.openai_chat_api_url
-
-    @property
-    def openai_completion_request_url(self) -> str:
-        if self.proxy_mode == PROXY_MODE[2]:
-            self.proxies = None
-            return f"{self.openai_proxy_url}completions"
-        return self.openai_completion_api_url
-
-    def set_proxy_mode(self, mode: str, proxies: Optional[dict] = None):
-        self.proxy_mode = mode
-        self.proxies = proxies
+# Copyright (c) 2023 promptulate
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+# Copyright Owner: Zeeland
+# GitHub Link: https://github.com/Undertone0809/
+# Project Link: https://github.com/Undertone0809/promptulate
+# Contact Email: zeeland@foxmail.com
+
+import os
+from typing import Optional
+
+from promptulate import utils
+from promptulate.utils.logger import get_logger
+from promptulate.utils.openai_key_pool import OpenAIKeyPool
+from promptulate.utils.singleton import Singleton
+
+PROXY_MODE = ["off", "custom", "promptulate"]
+logger = get_logger()
+
+
+def set_enable_cache(value: bool):
+    """Caching is enabled by default. Disabling caching is not recommended."""
+    Config().enable_cache = value
+
+
+class Config(metaclass=Singleton):
+    def __init__(self):
+        logger.info(f"[pne config] Config initialization")
+        self.enable_cache: bool = True
+        self._proxy_mode: str = PROXY_MODE[0]
+        self._proxies: Optional[dict] = None
+        self.openai_chat_api_url = "https://api.openai.com/v1/chat/completions"
+        self.openai_completion_api_url = "https://api.openai.com/v1/completions"
+        self.openai_proxy_url = "https://chatgpt-api.shn.hk/v1/"  # FREE API
+        self.key_default_retry_times = 5
+        """If llm(like OpenAI) unable to obtain data, retry request until the data is obtained."""
+
+    @property
+    def openai_api_key(self):
+        """This attribution has deprecated to use. Using `get_openai_api_key`"""
+        if "OPENAI_API_KEY" in os.environ.keys():
+            if self.enable_cache:
+                utils.get_cache()["OPENAI_API_KEY"] = os.getenv("OPENAI_API_KEY")
+            return os.getenv("OPENAI_API_KEY")
+        if self.enable_cache and "OPENAI_API_KEY" in utils.get_cache():
+            return utils.get_cache()["OPENAI_API_KEY"]
+        raise ValueError("OPENAI API key is not provided. Please set your key.")
+
+    def get_openai_api_key(self, model: str) -> str:
+        """Get openai key from KeyPool and environ"""
+        if self.enable_cache:
+            openai_key_pool: OpenAIKeyPool = OpenAIKeyPool()
+            key = openai_key_pool.get(model)
+            if key:
+                return key
+        return self.openai_api_key
+
+    def get_key_retry_times(self, model: str) -> int:
+        if self.enable_cache:
+            openai_key_pool: OpenAIKeyPool = OpenAIKeyPool()
+            return openai_key_pool.get_num(model)
+        return self.key_default_retry_times
+
+    @property
+    def proxy_mode(self) -> str:
+        if self.enable_cache and "PROXY_MODE" in utils.get_cache():
+            return utils.get_cache()["PROXY_MODE"]
+        return self._proxy_mode
+
+    @proxy_mode.setter
+    def proxy_mode(self, value):
+        self._proxy_mode = value
+        if self.enable_cache:
+            utils.get_cache()["PROXY_MODE"] = value
+
+    @property
+    def proxies(self) -> Optional[dict]:
+        if self.enable_cache and "PROXIES" in utils.get_cache():
+            return utils.get_cache()["PROXIES"] if self.proxy_mode == "custom" else None
+        return self._proxies
+
+    @proxies.setter
+    def proxies(self, value):
+        self._proxies = value
+        if self.enable_cache:
+            utils.get_cache()["PROXIES"] = value
+
+    @property
+    def openai_chat_request_url(self) -> str:
+        if self.proxy_mode == PROXY_MODE[2]:
+            self.proxies = None
+            return self.openai_proxy_url
+        return self.openai_chat_api_url
+
+    @property
+    def openai_completion_request_url(self) -> str:
+        if self.proxy_mode == PROXY_MODE[2]:
+            self.proxies = None
+            return f"{self.openai_proxy_url}completions"
+        return self.openai_completion_api_url
+
+    def set_proxy_mode(self, mode: str, proxies: Optional[dict] = None):
+        self.proxy_mode = mode
+        self.proxies = proxies
+        logger.info(f"[pne] proxy mode: {mode}, proxies: {proxies}")
```

### Comparing `promptulate-1.2.2/promptulate/frameworks/__init__.py` & `promptulate-1.3.0/promptulate/frameworks/conversation/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-# Copyright (c) 2023 promptulate
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-# Copyright Owner: Zeeland
-# GitHub Link: https://github.com/Undertone0809/
-# Project Link: https://github.com/Undertone0809/promptulate
-# Contact Email: zeeland@foxmail.com
-
-
-from promptulate.frameworks.conversation import Conversation
-
-__all__ = [
-    'Conversation',
-]
+# Copyright (c) 2023 promptulate
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+# Copyright Owner: Zeeland
+# GitHub Link: https://github.com/Undertone0809/
+# Project Link: https://github.com/Undertone0809/promptulate
+# Contact Email: zeeland@foxmail.com
+
+
+from promptulate.frameworks.conversation.conversation import Conversation
+
+__all__ = [
+    'Conversation'
+]
```

### Comparing `promptulate-1.2.2/promptulate/frameworks/conversation/__init__.py` & `promptulate-1.3.0/promptulate/frameworks/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-# Copyright (c) 2023 promptulate
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-# Copyright Owner: Zeeland
-# GitHub Link: https://github.com/Undertone0809/
-# Project Link: https://github.com/Undertone0809/promptulate
-# Contact Email: zeeland@foxmail.com
-
-
-from promptulate.frameworks.conversation.conversation import Conversation
-
-__all__ = [
-    'Conversation'
-]
+# Copyright (c) 2023 promptulate
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+# Copyright Owner: Zeeland
+# GitHub Link: https://github.com/Undertone0809/
+# Project Link: https://github.com/Undertone0809/promptulate
+# Contact Email: zeeland@foxmail.com
+
+
+from promptulate.frameworks.conversation import Conversation
+
+__all__ = [
+    'Conversation',
+]
```

### Comparing `promptulate-1.2.2/promptulate/frameworks/conversation/conversation.py` & `promptulate-1.3.0/promptulate/frameworks/conversation/conversation.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,120 +1,120 @@
-# Copyright (c) 2023 promptulate
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-# Copyright Owner: Zeeland
-# GitHub Link: https://github.com/Undertone0809/
-# Project Link: https://github.com/Undertone0809/promptulate
-# Contact Email: zeeland@foxmail.com
-
-from typing import Optional, Union, Dict, Any
-
-from pydantic import Field, validator
-
-from promptulate import utils
-from promptulate.config import Config
-from promptulate.frameworks.schema import BasePromptFramework
-from promptulate.llms import ChatOpenAI
-from promptulate.llms.base import BaseLLM
-from promptulate.memory import BufferChatMemory
-from promptulate.memory.base import BaseChatMemory
-from promptulate.preset_roles.roles import CustomPresetRole, get_preset_role_prompt
-from promptulate.provider.mixins import (
-    SummarizerMixin,
-    TranslatorMixin,
-    DeriveHistoryMessageMixin,
-)
-from promptulate.schema import (
-    MessageSet,
-    AssistantMessage,
-    init_chat_message_history,
-)
-from promptulate.tips import EmptyMessageSetError
-from promptulate.utils.core_utils import record_time
-
-CFG = Config()
-logger = utils.get_logger()
-
-
-class Conversation(
-    BasePromptFramework, SummarizerMixin, TranslatorMixin, DeriveHistoryMessageMixin
-):
-    """
-    You can use Conversation start a conversation. Moreover, you can pass some parameters to enhance it.
-
-    Attributes
-        role: preset role. Default is default role.
-        llm: default is OpenAI GPT3.5. You can choose other llm.
-        conversation_id: conversation id. Default is None
-        memory: the way you want to store chat data. Default is BufferChatMemory, which is used
-            for local file storage.
-
-    Examples
-        from promptulate import Conversation
-
-        conversation = Conversation()
-        conversation.predict("Hello, Who are you?")
-    """
-
-    conversation_id: Optional[str] = None
-    llm: BaseLLM = Field(default_factory=ChatOpenAI)
-    enable_stream: bool = False  # streaming transmission
-    role: Union[str, CustomPresetRole] = "default-role"
-    memory: BaseChatMemory = Field(default_factory=BufferChatMemory)
-
-    @validator("conversation_id", always=True)
-    def init_conversation_id(
-        cls, conversation_id: Optional[str], values: Dict[str, Any]
-    ) -> Optional[str]:
-        """initialize self.conversation_id and memory.conversation_id"""
-        if not conversation_id:
-            return None
-
-        assert conversation_id.isdigit(), "conversation_id must a digit type string"
-        if "memory" in values and values["memory"]:
-            cls.memory.conversation_id = conversation_id
-        return conversation_id
-
-    @validator("memory", always=True)
-    def init_memory(
-        cls, memory: BaseChatMemory, values: Dict[str, Any]
-    ) -> BaseChatMemory:
-        """check whether exist conversation_id before initialize memory"""
-        if "conversation_id" in values and values["conversation_id"]:
-            memory.conversation_id = values["conversation_id"]
-        else:
-            values["conversation_id"] = memory.conversation_id
-            cls.conversation_id = memory.conversation_id
-        return memory
-
-    @record_time()
-    def predict(self, prompt: str, **kwargs) -> str:
-        try:
-            messages_history: MessageSet = self.memory.load_message_set_from_memory()
-            messages_history.add_user_message(message=prompt)
-        except EmptyMessageSetError as e:
-            messages_history = init_chat_message_history(
-                get_preset_role_prompt(self.role), prompt
-            )
-            self.memory.save_message_set_to_memory(messages_history)
-        logger.debug(
-            f"[promptulate Conversation] conversation_id: <{self.conversation_id}> messages: <{messages_history.messages}>"
-        )
-        prompt_params = {"prompts": messages_history}
-        if "stop" in kwargs:
-            prompt_params.update({"update": kwargs["stop"]})
-
-        answer: AssistantMessage = self.llm.predict(**prompt_params)
-        messages_history.messages.append(answer)
-        self.memory.save_message_set_to_memory(messages_history)
-        return answer.content
+# Copyright (c) 2023 promptulate
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+# Copyright Owner: Zeeland
+# GitHub Link: https://github.com/Undertone0809/
+# Project Link: https://github.com/Undertone0809/promptulate
+# Contact Email: zeeland@foxmail.com
+
+from typing import Optional, Union, Dict, Any
+
+from pydantic import Field, validator
+
+from promptulate import utils
+from promptulate.config import Config
+from promptulate.frameworks.schema import BasePromptFramework
+from promptulate.llms import ChatOpenAI
+from promptulate.llms.base import BaseLLM
+from promptulate.memory import BufferChatMemory
+from promptulate.memory.base import BaseChatMemory
+from promptulate.preset_roles.roles import CustomPresetRole, get_preset_role_prompt
+from promptulate.provider.mixins import (
+    SummarizerMixin,
+    TranslatorMixin,
+    DeriveHistoryMessageMixin,
+)
+from promptulate.schema import (
+    MessageSet,
+    AssistantMessage,
+    init_chat_message_history,
+)
+from promptulate.tips import EmptyMessageSetError
+from promptulate.utils.core_utils import record_time
+
+CFG = Config()
+logger = utils.get_logger()
+
+
+class Conversation(
+    BasePromptFramework, SummarizerMixin, TranslatorMixin, DeriveHistoryMessageMixin
+):
+    """
+    You can use Conversation start a conversation. Moreover, you can pass some parameters to enhance it.
+
+    Attributes
+        role: preset role. Default is default role.
+        llm: default is OpenAI GPT3.5. You can choose other llm.
+        conversation_id: conversation id. Default is None
+        memory: the way you want to store chat data. Default is BufferChatMemory, which is used
+            for local file storage.
+
+    Examples
+        from promptulate import Conversation
+
+        conversation = Conversation()
+        conversation.predict("Hello, Who are you?")
+    """
+
+    conversation_id: Optional[str] = None
+    llm: BaseLLM = Field(default_factory=ChatOpenAI)
+    enable_stream: bool = False  # streaming transmission
+    role: Union[str, CustomPresetRole] = "default-role"
+    memory: BaseChatMemory = Field(default_factory=BufferChatMemory)
+
+    @validator("conversation_id", always=True)
+    def init_conversation_id(
+        cls, conversation_id: Optional[str], values: Dict[str, Any]
+    ) -> Optional[str]:
+        """initialize self.conversation_id and memory.conversation_id"""
+        if not conversation_id:
+            return None
+
+        assert conversation_id.isdigit(), "conversation_id must a digit type string"
+        if "memory" in values and values["memory"]:
+            cls.memory.conversation_id = conversation_id
+        return conversation_id
+
+    @validator("memory", always=True)
+    def init_memory(
+        cls, memory: BaseChatMemory, values: Dict[str, Any]
+    ) -> BaseChatMemory:
+        """check whether exist conversation_id before initialize memory"""
+        if "conversation_id" in values and values["conversation_id"]:
+            memory.conversation_id = values["conversation_id"]
+        else:
+            values["conversation_id"] = memory.conversation_id
+            cls.conversation_id = memory.conversation_id
+        return memory
+
+    @record_time()
+    def predict(self, prompt: str, **kwargs) -> str:
+        try:
+            messages_history: MessageSet = self.memory.load_message_set_from_memory()
+            messages_history.add_user_message(message=prompt)
+        except EmptyMessageSetError as e:
+            messages_history = init_chat_message_history(
+                get_preset_role_prompt(self.role), prompt
+            )
+            self.memory.save_message_set_to_memory(messages_history)
+        logger.debug(
+            f"[pne Conversation] conversation_id: <{self.conversation_id}> messages: <{messages_history.messages}>"
+        )
+        prompt_params = {"prompts": messages_history}
+        if "stop" in kwargs:
+            prompt_params.update({"update": kwargs["stop"]})
+
+        answer: AssistantMessage = self.llm.predict(**prompt_params)
+        messages_history.messages.append(answer)
+        self.memory.save_message_set_to_memory(messages_history)
+        return answer.content
```

### Comparing `promptulate-1.2.2/promptulate/frameworks/prompt.py` & `promptulate-1.3.0/promptulate/frameworks/prompt.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-# Copyright (c) 2023 promptulate
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-# Copyright Owner: Zeeland
-# GitHub Link: https://github.com/Undertone0809/
-# Project Link: https://github.com/Undertone0809/promptulate
-# Contact Email: zeeland@foxmail.com
-
-__all__ = [
-    'SUMMARY_CONTENT_PROMPT_ZH',
-    'SUMMARY_TOPIC_PROMPT_ZH',
-    'SUMMARY_TOPIC_PROMPT_EN',
-    'SUMMARY_CONTENT_PROMPT_EN',
-]
-
-SUMMARY_CONTENT_PROMPT_ZH = """
-简要总结一下你和用户的对话，用作后续的上下文提示 prompt，控制在 200 字以内
-"""
-
-SUMMARY_TOPIC_PROMPT_ZH = """
-上面是ai 和用户的历史聊天总结作为前情提要，请使用四到五个字直接返回这句话的简要主题，
-不要解释、不要标点、不要语气词、不要多余文本，如果没有主题，请直接返回“闲聊”
-"""
-
-SUMMARY_CONTENT_PROMPT_EN = """
-Give a quick summary of your conversation with the user and use it as a follow-up context prompt, no more than 200 words
-"""
-
-SUMMARY_TOPIC_PROMPT_EN = """
-As the previous feed, please use four or five words to return directly to the brief topic of the sentence, 
-no explanation, no punctuation, no particles, no extra text, or if there is no topic, just return to "small talk".
-"""
+# Copyright (c) 2023 promptulate
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+# Copyright Owner: Zeeland
+# GitHub Link: https://github.com/Undertone0809/
+# Project Link: https://github.com/Undertone0809/promptulate
+# Contact Email: zeeland@foxmail.com
+
+__all__ = [
+    'SUMMARY_CONTENT_PROMPT_ZH',
+    'SUMMARY_TOPIC_PROMPT_ZH',
+    'SUMMARY_TOPIC_PROMPT_EN',
+    'SUMMARY_CONTENT_PROMPT_EN',
+]
+
+SUMMARY_CONTENT_PROMPT_ZH = """
+简要总结一下你和用户的对话，用作后续的上下文提示 prompt，控制在 200 字以内
+"""
+
+SUMMARY_TOPIC_PROMPT_ZH = """
+上面是ai 和用户的历史聊天总结作为前情提要，请使用四到五个字直接返回这句话的简要主题，
+不要解释、不要标点、不要语气词、不要多余文本，如果没有主题，请直接返回“闲聊”
+"""
+
+SUMMARY_CONTENT_PROMPT_EN = """
+Give a quick summary of your conversation with the user and use it as a follow-up context prompt, no more than 200 words
+"""
+
+SUMMARY_TOPIC_PROMPT_EN = """
+As the previous feed, please use four or five words to return directly to the brief topic of the sentence, 
+no explanation, no punctuation, no particles, no extra text, or if there is no topic, just return to "small talk".
+"""
```

### Comparing `promptulate-1.2.2/promptulate/frameworks/react/__init__.py` & `promptulate-1.3.0/promptulate/frameworks/react/__init__.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-# Copyright (c) 2023 promptulate
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-# Copyright Owner: Zeeland
-# GitHub Link: https://github.com/Undertone0809/
-# Project Link: https://github.com/Undertone0809/promptulate
-# Contact Email: zeeland@foxmail.com
+# Copyright (c) 2023 promptulate
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+# Copyright Owner: Zeeland
+# GitHub Link: https://github.com/Undertone0809/
+# Project Link: https://github.com/Undertone0809/promptulate
+# Contact Email: zeeland@foxmail.com
```

### Comparing `promptulate-1.2.2/promptulate/frameworks/schema.py` & `promptulate-1.3.0/promptulate/frameworks/schema.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-# Copyright (c) 2023 promptulate
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-# Copyright Owner: Zeeland
-# GitHub Link: https://github.com/Undertone0809/
-# Project Link: https://github.com/Undertone0809/promptulate
-# Contact Email: zeeland@foxmail.com
-
-from pydantic import BaseModel
-
-from promptulate.config import Config
-from promptulate.llms.base import BaseLLM
-from promptulate.memory.base import BaseChatMemory
-
-CFG = Config()
-
-
-class BasePromptFramework(BaseModel):
-    role: str
-    conversation_id: str
-    llm: BaseLLM
-    memory: BaseChatMemory
-
-    class Config:
-        arbitrary_types_allowed = True
+# Copyright (c) 2023 promptulate
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+# Copyright Owner: Zeeland
+# GitHub Link: https://github.com/Undertone0809/
+# Project Link: https://github.com/Undertone0809/promptulate
+# Contact Email: zeeland@foxmail.com
+
+from pydantic import BaseModel
+
+from promptulate.config import Config
+from promptulate.llms.base import BaseLLM
+from promptulate.memory.base import BaseChatMemory
+
+CFG = Config()
+
+
+class BasePromptFramework(BaseModel):
+    role: str
+    conversation_id: str
+    llm: BaseLLM
+    memory: BaseChatMemory
+
+    class Config:
+        arbitrary_types_allowed = True
```

### Comparing `promptulate-1.2.2/promptulate/frameworks/self_ask/__init__.py` & `promptulate-1.3.0/promptulate/frameworks/self_ask/__init__.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-# Copyright (c) 2023 promptulate
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-# Copyright Owner: Zeeland
-# GitHub Link: https://github.com/Undertone0809/
-# Project Link: https://github.com/Undertone0809/promptulate
-# Contact Email: zeeland@foxmail.com
+# Copyright (c) 2023 promptulate
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+# Copyright Owner: Zeeland
+# GitHub Link: https://github.com/Undertone0809/
+# Project Link: https://github.com/Undertone0809/promptulate
+# Contact Email: zeeland@foxmail.com
```

### Comparing `promptulate-1.2.2/promptulate/llms/__init__.py` & `promptulate-1.3.0/promptulate/llms/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-# Copyright (c) 2023 promptulate
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-# Copyright Owner: Zeeland
-# GitHub Link: https://github.com/Undertone0809/
-# Project Link: https://github.com/Undertone0809/promptulate
-# Contact Email: zeeland@foxmail.com
-
-from promptulate.llms.openai import OpenAI, ChatOpenAI
-
-__all__ = ["OpenAI", "ChatOpenAI"]
+# Copyright (c) 2023 promptulate
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+# Copyright Owner: Zeeland
+# GitHub Link: https://github.com/Undertone0809/
+# Project Link: https://github.com/Undertone0809/promptulate
+# Contact Email: zeeland@foxmail.com
+
+from promptulate.llms.base import BaseLLM
+from promptulate.llms.openai import OpenAI, ChatOpenAI
+
+__all__ = ["OpenAI", "ChatOpenAI", "BaseLLM"]
```

### Comparing `promptulate-1.2.2/promptulate/llms/openai.py` & `promptulate-1.3.0/promptulate/llms/openai/openai.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,267 +1,279 @@
-"""
-There are 2 kinds of model in OpenAI, namely text generative and conversational.
-"""
-
-import json
-from abc import ABC
-from enum import Enum
-from typing import Optional, Any, Dict, List
-
-import requests
-
-from promptulate.config import Config
-from promptulate.llms.base import BaseLLM
-from promptulate.preset_roles.prompt import PRESET_SYSTEM_PROMPT
-from promptulate.schema import (
-    LLMType,
-    MessageSet,
-    UserMessage,
-    SystemMessage,
-    AssistantMessage,
-    CompletionMessage,
-)
-from promptulate.tips import OpenAIError
-from promptulate.utils.logger import get_logger
-
-CFG = Config()
-logger = get_logger()
-
-
-class OpenAIModelType(str, Enum):
-    pass
-
-
-class BaseOpenAI(BaseLLM, ABC):
-    """https://platform.openai.com/docs/api-reference/chat/create"""
-
-    llm_type: LLMType
-    """Used to MessageSet data convert"""
-    model: str
-    """Model name to use."""
-    temperature: float = 1.0
-    """What sampling temperature to use."""
-    top_p: float = 1
-    """Total probability mass of tokens to consider at each step."""
-    stream: bool = False
-    """Whether to stream the results or not."""
-    frequency_penalty: float = 0
-    """Penalizes repeated tokens according to frequency."""
-    presence_penalty: float = 0
-    """Penalizes repeated tokens."""
-    n: int = 1
-    """How many completions to generate for each prompt."""
-    max_tokens: int = 3000
-    """The maximum number of tokens to generate in the completion.
-    -1 returns as many tokens as possible given the prompt and
-    the models maximal context size."""
-    api_param_keys: List[str] = [
-        "model",
-        "temperature",
-        "top_p",
-        "stream",
-        "stop",
-        "frequency_penalty",
-        "presence_penalty",
-        "n",
-        "max_tokens",
-    ]
-    """The key of openai api parameters"""
-    preset_description: str = ""
-    """OpenAI system message"""
-    enable_private_api_key: bool = False
-    """Enable to provide a separate api for openai llm """
-    private_api_key: str = ""
-    """Store private api key"""
-    enable_retry: bool = True
-    """Retry if API failed to get response. You can enable retry when you have a rate limited API."""
-    retry_times: int = 5
-    """If llm(like OpenAI) unable to obtain data, retry request until the data is obtained. You should
-    enable retry if you want to use retry times."""
-    retry_counter: int = 0
-    """Used in conjunction with retry_times. Refresh when get data successfully."""
-
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
-        self.retry_times = CFG.get_key_retry_times(self.model)
-
-    @property
-    def api_key(self):
-        """Select api key to use. private_api_key, openai_api_key, key_pool key is optional."""
-        if self.enable_private_api_key and self.private_api_key != "":
-            return self.private_api_key
-        return CFG.get_openai_api_key(self.model)
-
-    def set_private_api_key(self, value: str):
-        self.enable_private_api_key = True
-        self.private_api_key = value
-
-
-class OpenAI(BaseOpenAI):
-    """https://platform.openai.com/docs/api-reference/chat/create"""
-
-    llm_type: LLMType = LLMType.OpenAI
-    """Used to MessageSet data convert"""
-    model: str = "text-davinci-003"
-    """Model name to use."""
-    max_tokens: int = 800
-    """The maximum number of tokens to generate in the completion.
-    -1 returns as many tokens as possible given the prompt and
-    the models maximal context size."""
-
-    def __call__(
-        self, prompt: str, stop: Optional[List[str]] = None, *args, **kwargs
-    ) -> str:
-        preset = (
-            self.preset_description
-            if self.preset_description != ""
-            else PRESET_SYSTEM_PROMPT
-        )
-        message_set = MessageSet(llm_type=LLMType.OpenAI)
-        message_set.messages.append(CompletionMessage(content=preset))
-        message_set.messages.append(CompletionMessage(content=prompt))
-        return self.predict(message_set, stop).content
-
-    def predict(
-        self, prompts: MessageSet, stop: Optional[List[str]] = None
-    ) -> Optional[AssistantMessage]:
-        api_key = self.api_key
-        logger.debug(f"[promptulate openai key] {api_key}")
-        headers = {
-            "Content-Type": "application/json",
-            "Authorization": f"Bearer {api_key}",
-        }
-        body: Dict[str, Any] = self._build_api_params_dict(prompts, stop)
-
-        logger.debug(f"[promptulate openai params] body {json.dumps(body)}")
-        logger.debug(
-            f"[promptulate openai request] url: {CFG.openai_completion_request_url} proxies: {CFG.proxies}"
-        )
-        response = requests.post(
-            url=CFG.openai_completion_request_url,
-            headers=headers,
-            json=body,
-            proxies=CFG.proxies,
-        )
-        if response.status_code == 200:
-            # todo enable stream mode
-            # for chunk in response.iter_content(chunk_size=None):
-            #     logger.debug(chunk)
-            self.retry_counter = 0
-            ret_data = response.json()
-            logger.debug(f"[promptulate openai response] {json.dumps(ret_data)}")
-            content = ret_data["choices"][0]["text"]
-            logger.debug(f"[promptulate openai answer] {content}")
-            return AssistantMessage(content=content)
-
-        logger.error(
-            "[promptulate OpenAI] Failed to get data. Please check your network or api key."
-        )
-        logger.debug("[promptulate OpenAI] retry to get response")
-        if self.enable_retry and self.retry_counter < self.retry_times:
-            self.retry_counter += 1
-            return self.predict(prompts, stop)
-
-        logger.error(
-            f"[promptulate OpenAI] Has retry {self.retry_times}, but all failed."
-        )
-        raise OpenAIError(json.dumps(response.content))
-
-    def _build_api_params_dict(
-        self, prompts: MessageSet, stop: Optional[List[str]] = None
-    ) -> Dict[str, Any]:
-        """Build api parameters to put it inside the body."""
-        dic = {"prompt": prompts.string_messages}
-
-        if stop:
-            dic.update({"stop": stop})
-
-        for key in self.api_param_keys:
-            if key in self.__dict__:
-                dic.update({key: self.__dict__[key]})
-        return dic
-
-
-class ChatOpenAI(BaseOpenAI):
-    """https://platform.openai.com/docs/api-reference/chat/create"""
-
-    llm_type: LLMType = LLMType.ChatOpenAI
-    """Used to MessageSet data convert"""
-    model: str = "gpt-3.5-turbo"
-    """Model name to use."""
-
-    def __call__(
-        self, prompt: str, stop: Optional[List[str]] = None, *args, **kwargs
-    ) -> str:
-        system_message = (
-            self.preset_description
-            if self.preset_description != ""
-            else PRESET_SYSTEM_PROMPT
-        )
-
-        message_set = MessageSet(
-            messages=[
-                SystemMessage(content=system_message),
-                UserMessage(content=prompt),
-            ]
-        )
-        return self.predict(message_set, stop).content
-
-    def predict(
-        self, prompts: MessageSet, stop: Optional[List[str]] = None
-    ) -> Optional[AssistantMessage]:
-        api_key = self.api_key
-        logger.debug(f"[promptulate openai key] {api_key}")
-        headers = {
-            "Content-Type": "application/json",
-            "Authorization": f"Bearer {api_key}",
-        }
-        body: Dict[str, Any] = self._build_api_params_dict(prompts, stop)
-
-        logger.debug(f"[promptulate openai params] body {json.dumps(body)}")
-        logger.debug(
-            f"[promptulate openai request] url: {CFG.openai_chat_request_url} proxies: {CFG.proxies}"
-        )
-        response = requests.post(
-            url=CFG.openai_chat_request_url,
-            headers=headers,
-            json=body,
-            proxies=CFG.proxies,
-        )
-        if response.status_code == 200:
-            # todo enable stream mode
-            # for chunk in response.iter_content(chunk_size=None):
-            #     logger.debug(chunk)
-            self.retry_counter = 0
-            ret_data = response.json()
-            logger.debug(f"[promptulate openai response] {json.dumps(ret_data)}")
-            content = ret_data["choices"][0]["message"]["content"]
-            logger.debug(f"[promptulate openai answer] {content}")
-            return AssistantMessage(content=content)
-
-        logger.error(
-            "[promptulate OpenAI] Failed to get data. Please check your network or api key."
-        )
-        logger.debug("[promptulate OpenAI] retry to get response")
-        if self.enable_retry and self.retry_counter < self.retry_times:
-            self.retry_counter += 1
-            return self.predict(prompts, stop)
-
-        logger.error(
-            f"[promptulate OpenAI] Has retry {self.retry_times}, but all failed."
-        )
-        raise OpenAIError(json.dumps(json.loads(response.content)))
-
-    def _build_api_params_dict(
-        self, prompts: MessageSet, stop: Optional[List[str]] = None
-    ) -> Dict[str, Any]:
-        dic = {
-            "messages": prompts.to_llm_prompt(self.llm_type),
-        }
-
-        if stop:
-            dic.update({"stop": stop})
-
-        for key in self.api_param_keys:
-            if key in self.__dict__:
-                dic.update({key: self.__dict__[key]})
-        return dic
+"""
+There are 2 kinds of model in OpenAI, namely text generative and conversational.
+"""
+
+import json
+import warnings
+from abc import ABC
+from typing import Optional, Any, Dict, List
+
+import requests
+
+from promptulate.config import Config
+from promptulate.llms.base import BaseLLM
+from promptulate.preset_roles.prompt import PRESET_SYSTEM_PROMPT
+from promptulate.schema import (
+    LLMType,
+    MessageSet,
+    UserMessage,
+    SystemMessage,
+    AssistantMessage,
+    CompletionMessage,
+)
+from promptulate.tips import OpenAIError
+from promptulate.utils.logger import get_logger
+
+CFG = Config()
+logger = get_logger()
+
+
+class BaseOpenAI(BaseLLM, ABC):
+    """https://platform.openai.com/docs/api-reference/chat/create"""
+
+    llm_type: LLMType
+    """Used to MessageSet data convert"""
+    model: str
+    """Model name to use."""
+    temperature: float = 1.0
+    """What sampling temperature to use."""
+    top_p: float = 1
+    """Total probability mass of tokens to consider at each step."""
+    stream: bool = False
+    """Whether to stream the results or not."""
+    frequency_penalty: float = 0
+    """Penalizes repeated tokens according to frequency."""
+    presence_penalty: float = 0
+    """Penalizes repeated tokens."""
+    n: int = 1
+    """How many completions to generate for each prompt."""
+    max_tokens: int = 3000
+    """The maximum number of tokens to generate in the completion.
+    -1 returns as many tokens as possible given the prompt and
+    the models maximal context size."""
+    api_param_keys: List[str] = [
+        "model",
+        "temperature",
+        "top_p",
+        "stream",
+        "stop",
+        "frequency_penalty",
+        "presence_penalty",
+        "n",
+        "max_tokens",
+    ]
+    """The key of openai api parameters"""
+    preset_description: str = ""
+    """OpenAI system message"""
+    enable_preset_description: bool = True
+    """enable use preset description"""
+    enable_private_api_key: bool = False
+    """Enable to provide a separate api for openai llm """
+    private_api_key: str = ""
+    """Store private api key"""
+    enable_retry: bool = True
+    """Retry if API failed to get response. You can enable retry when you have a rate limited API."""
+    retry_times: int = 5
+    """If llm(like OpenAI) unable to obtain data, retry request until the data is obtained. You should
+    enable retry if you want to use retry times."""
+    retry_counter: int = 0
+    """Used in conjunction with retry_times. Refresh when get data successfully."""
+
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
+        self.retry_times = CFG.get_key_retry_times(self.model)
+
+    @property
+    def api_key(self):
+        """Select api key to use. private_api_key, openai_api_key, key_pool key is optional."""
+        if self.enable_private_api_key and self.private_api_key != "":
+            return self.private_api_key
+        return CFG.get_openai_api_key(self.model)
+
+    def set_private_api_key(self, value: str):
+        self.enable_private_api_key = True
+        self.private_api_key = value
+
+
+class OpenAI(BaseOpenAI):
+    """https://platform.openai.com/docs/api-reference/chat/create"""
+
+    llm_type: LLMType = LLMType.OpenAI
+    """Used to MessageSet data convert"""
+    model: str = "text-davinci-003"
+    """Model name to use."""
+    max_tokens: int = 800
+    """The maximum number of tokens to generate in the completion.
+    -1 returns as many tokens as possible given the prompt and
+    the models maximal context size."""
+
+    def __call__(
+        self, prompt: str, stop: Optional[List[str]] = None, *args, **kwargs
+    ) -> str:
+        preset = (
+            self.preset_description
+            if self.preset_description != ""
+            else PRESET_SYSTEM_PROMPT
+        )
+        if not self.enable_preset_description:
+            preset = ""
+        message_set = MessageSet(
+            messages=[
+                CompletionMessage(content=preset),
+                CompletionMessage(content=prompt),
+            ]
+        )
+        return self.predict(message_set, stop).content
+
+    def _predict(
+        self, prompts: MessageSet, stop: Optional[List[str]] = None, *args, **kwargs
+    ) -> Optional[AssistantMessage]:
+        """Run openai llm with custom message context."""
+        if self.model == "text-davinci-003":
+            warnings.warn(
+                "This model(text-davinci-003) version is deprecated. Migrate before January 4, 2024 to "
+                "avoid disruption of service. gpt-3.5-turbo is recommended.",
+                DeprecationWarning,
+            )
+        api_key = self.api_key
+        logger.debug(f"[pne openai key] {api_key}")
+        headers = {
+            "Content-Type": "application/json",
+            "Authorization": f"Bearer {api_key}",
+        }
+        body: Dict[str, Any] = self._build_api_params_dict(prompts, stop)
+
+        logger.debug(f"[pne openai params] body {json.dumps(body)}")
+        logger.debug(
+            f"[pne openai request] url: {CFG.openai_completion_request_url} proxies: {CFG.proxies}"
+        )
+        response = requests.post(
+            url=CFG.openai_completion_request_url,
+            headers=headers,
+            json=body,
+            proxies=CFG.proxies,
+        )
+        if response.status_code == 200:
+            # todo enable stream mode
+            # for chunk in response.iter_content(chunk_size=None):
+            #     logger.debug(chunk)
+            self.retry_counter = 0
+            ret_data = response.json()
+            logger.debug(f"[pne openai response] {json.dumps(ret_data)}")
+            content = ret_data["choices"][0]["text"]
+            logger.debug(f"[pne openai answer] {content}")
+            return AssistantMessage(content=content)
+
+        logger.error(
+            "[promptulate OpenAI] Failed to get data. Please check your network or api key."
+        )
+        logger.debug("[promptulate OpenAI] retry to get response")
+        if self.enable_retry and self.retry_counter < self.retry_times:
+            self.retry_counter += 1
+            return self._predict(prompts, stop)
+
+        logger.error(
+            f"[pne OpenAI] Has retry {self.retry_times}, but all failed."
+        )
+        raise OpenAIError(json.dumps(response.content))
+
+    def _build_api_params_dict(
+        self, prompts: MessageSet, stop: Optional[List[str]] = None
+    ) -> Dict[str, Any]:
+        """Build api parameters to put it inside the body."""
+        dic = {"prompt": prompts.string_messages}
+
+        if stop:
+            dic.update({"stop": stop})
+
+        for key in self.api_param_keys:
+            if key in self.__dict__:
+                dic.update({key: self.__dict__[key]})
+        return dic
+
+
+class ChatOpenAI(BaseOpenAI):
+    """https://platform.openai.com/docs/api-reference/chat/create"""
+
+    llm_type: LLMType = LLMType.ChatOpenAI
+    """Used to MessageSet data convert"""
+    model: str = "gpt-3.5-turbo"
+    """Model name to use."""
+
+    def __call__(
+        self, prompt: str, stop: Optional[List[str]] = None, *args, **kwargs
+    ) -> str:
+        system_message = (
+            self.preset_description
+            if self.preset_description != ""
+            else PRESET_SYSTEM_PROMPT
+        )
+        if not self.enable_preset_description:
+            system_message = ""
+
+        message_set = MessageSet(
+            messages=[
+                SystemMessage(content=system_message),
+                UserMessage(content=prompt),
+            ]
+        )
+        return self.predict(message_set, stop).content
+
+    def _predict(
+        self, prompts: MessageSet, stop: Optional[List[str]] = None, *args, **kwargs
+    ) -> Optional[AssistantMessage]:
+        api_key = self.api_key
+        logger.debug(f"[pne openai key] {api_key}")
+        headers = {
+            "Content-Type": "application/json",
+            "Authorization": f"Bearer {api_key}",
+        }
+        body: Dict[str, Any] = self._build_api_params_dict(prompts, stop)
+
+        logger.debug(f"[pne openai params] body {json.dumps(body)}")
+        logger.debug(
+            f"[pne openai request] url: {CFG.openai_chat_request_url} proxies: {CFG.proxies}"
+        )
+        response = requests.post(
+            url=CFG.openai_chat_request_url,
+            headers=headers,
+            json=body,
+            proxies=CFG.proxies,
+        )
+        if response.status_code == 200:
+            # todo enable stream mode
+            # for chunk in response.iter_content(chunk_size=None):
+            #     logger.debug(chunk)
+            self.retry_counter = 0
+            ret_data = response.json()
+            logger.debug(f"[pne openai response] {json.dumps(ret_data)}")
+            content = ret_data["choices"][0]["message"]["content"]
+            logger.debug(f"[pne openai answer] {content}")
+            return AssistantMessage(content=content)
+
+        logger.error(
+            "[promptulate OpenAI] Failed to get data. Please check your network or api key."
+        )
+        logger.debug("[promptulate OpenAI] retry to get response")
+        if self.enable_retry and self.retry_counter < self.retry_times:
+            self.retry_counter += 1
+            return self._predict(prompts, stop)
+
+        logger.error(
+            f"[pne OpenAI] Has retry {self.retry_times}, but all failed."
+        )
+        raise OpenAIError(json.dumps(json.loads(response.content)))
+
+    def _build_api_params_dict(
+        self, prompts: MessageSet, stop: Optional[List[str]] = None
+    ) -> Dict[str, Any]:
+        dic = {
+            "messages": prompts.to_llm_prompt(self.llm_type),
+        }
+
+        if stop:
+            dic.update({"stop": stop})
+
+        for key in self.api_param_keys:
+            if key in self.__dict__:
+                dic.update({key: self.__dict__[key]})
+        return dic
```

### Comparing `promptulate-1.2.2/promptulate/memory/__init__.py` & `promptulate-1.3.0/promptulate/preset_roles/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,25 @@
-# Copyright (c) 2023 promptulate
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-# Copyright Owner: Zeeland
-# GitHub Link: https://github.com/Undertone0809/
-# Project Link: https://github.com/Undertone0809/promptulate
-# Contact Email: zeeland@foxmail.com
-
-from promptulate.memory.buffer import BufferChatMemory
-from promptulate.memory.file import FileChatMemory
-
-__all__ = [
-    'BufferChatMemory',
-    'FileChatMemory'
-]
+# Copyright (c) 2023 promptulate
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+# Copyright Owner: Zeeland
+# GitHub Link: https://github.com/Undertone0809/
+# Project Link: https://github.com/Undertone0809/promptulate
+# Contact Email: zeeland@foxmail.com
+
+from promptulate.preset_roles.roles import get_all_preset_roles, CustomPresetRole
+
+__all__ = [
+    'get_all_preset_roles',
+    'CustomPresetRole'
+]
```

### Comparing `promptulate-1.2.2/promptulate/memory/buffer.py` & `promptulate-1.3.0/promptulate/memory/buffer.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,62 +1,62 @@
-# Copyright (c) 2023 promptulate
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-# Copyright Owner: Zeeland
-# GitHub Link: https://github.com/Undertone0809/
-# Project Link: https://github.com/Undertone0809/promptulate
-# Contact Email: zeeland@foxmail.com
-
-from typing import Optional, List, Dict
-
-from promptulate import utils
-from promptulate.memory.base import BaseChatMemory
-from promptulate.schema import MessageSet
-from promptulate.tips import EmptyMessageSetError
-
-logger = utils.get_logger()
-buffer: Dict[str, List[Dict]] = {}
-"""global message buffer, here is a buffer example: 
-{
-    "conversation_id1": [message...],
-    "conversation_id2": [message...],
-}
-"""
-
-
-class BufferChatMemory(BaseChatMemory):
-    """Chat message will be stored in the buffer cache."""
-
-    def load_message_set_from_memory(
-            self, recently_n: Optional[int] = None
-    ) -> MessageSet:
-        """Load message from buffer memory
-
-        Args:
-            recently_n: load all messages if it is None, or return recently n messages.
-
-        Returns:
-            messages wrapping by MessageSet
-        """
-        if not buffer:
-            raise EmptyMessageSetError
-        recently_n = (
-            recently_n if recently_n else len(buffer[self.conversation_id])
-        )
-        num_messages = len(buffer[self.conversation_id])
-        return MessageSet.from_listdict_data(
-            buffer[self.conversation_id][num_messages - recently_n:]
-        )
-
-    def save_message_set_to_memory(self, message_set: MessageSet) -> None:
-        buffer[self.conversation_id] = message_set.memory_messages
+# Copyright (c) 2023 promptulate
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+# Copyright Owner: Zeeland
+# GitHub Link: https://github.com/Undertone0809/
+# Project Link: https://github.com/Undertone0809/promptulate
+# Contact Email: zeeland@foxmail.com
+
+from typing import Optional, List, Dict
+
+from promptulate import utils
+from promptulate.memory.base import BaseChatMemory
+from promptulate.schema import MessageSet
+from promptulate.tips import EmptyMessageSetError
+
+logger = utils.get_logger()
+buffer: Dict[str, List[Dict]] = {}
+"""global message buffer, here is a buffer example: 
+{
+    "conversation_id1": [message...],
+    "conversation_id2": [message...],
+}
+"""
+
+
+class BufferChatMemory(BaseChatMemory):
+    """Chat message will be stored in the buffer cache."""
+
+    def load_message_set_from_memory(
+            self, recently_n: Optional[int] = None
+    ) -> MessageSet:
+        """Load message from buffer memory
+
+        Args:
+            recently_n: load all messages if it is None, or return recently n messages.
+
+        Returns:
+            messages wrapping by MessageSet
+        """
+        if not buffer:
+            raise EmptyMessageSetError
+        recently_n = (
+            recently_n if recently_n else len(buffer[self.conversation_id])
+        )
+        num_messages = len(buffer[self.conversation_id])
+        return MessageSet.from_listdict_data(
+            buffer[self.conversation_id][num_messages - recently_n:]
+        )
+
+    def save_message_set_to_memory(self, message_set: MessageSet) -> None:
+        buffer[self.conversation_id] = message_set.memory_messages
```

### Comparing `promptulate-1.2.2/promptulate/memory/file.py` & `promptulate-1.3.0/promptulate/memory/file.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,64 +1,64 @@
-# Copyright (c) 2023 promptulate
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-# Copyright Owner: Zeeland
-# GitHub Link: https://github.com/Undertone0809/
-# Project Link: https://github.com/Undertone0809/promptulate
-# Contact Email: zeeland@foxmail.com
-
-from typing import Optional
-
-from cushy_storage import CushyOrmCache
-from pydantic import Field, validator
-
-from promptulate import utils
-from promptulate.memory.base import BaseChatMemory
-from promptulate.schema import MessageSet
-from promptulate.tips import EmptyMessageSetError
-
-logger = utils.get_logger()
-
-
-class FileChatMemory(BaseChatMemory):
-    """Chat message will be stored in the local file cache."""
-
-    file_path: Optional[str] = None
-    """If you want to change default store path, you can set specified file_path"""
-    cache: CushyOrmCache = Field(default_factory=CushyOrmCache)
-
-    @validator("file_path", always=True)
-    def init_cache(cls, file_path: Optional[str]) -> Optional[str]:
-        if not file_path:
-            return None
-
-        cls.cache = CushyOrmCache(file_path)
-        return file_path
-
-    def load_message_set_from_memory(
-        self, recently_n: Optional[int] = None
-    ) -> MessageSet:
-        """Load message from file memory
-
-        Args:
-            recently_n: load all messages if it is None, or return recently n messages.
-
-        Returns:
-            messages wrapping by MessageSet
-        """
-        if self.conversation_id not in self.cache:
-            raise EmptyMessageSetError()
-        return MessageSet.from_listdict_data(self.cache[self.conversation_id])
-
-    def save_message_set_to_memory(self, message_set: MessageSet) -> None:
-        self.cache[self.conversation_id] = message_set.listdict_messages
+# Copyright (c) 2023 promptulate
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+# Copyright Owner: Zeeland
+# GitHub Link: https://github.com/Undertone0809/
+# Project Link: https://github.com/Undertone0809/promptulate
+# Contact Email: zeeland@foxmail.com
+
+from typing import Optional
+
+from cushy_storage import CushyOrmCache
+from pydantic import Field, validator
+
+from promptulate import utils
+from promptulate.memory.base import BaseChatMemory
+from promptulate.schema import MessageSet
+from promptulate.tips import EmptyMessageSetError
+
+logger = utils.get_logger()
+
+
+class FileChatMemory(BaseChatMemory):
+    """Chat message will be stored in the local file cache."""
+
+    file_path: Optional[str] = None
+    """If you want to change default store path, you can set specified file_path"""
+    cache: CushyOrmCache = Field(default_factory=CushyOrmCache)
+
+    @validator("file_path", always=True)
+    def init_cache(cls, file_path: Optional[str]) -> Optional[str]:
+        if not file_path:
+            return None
+
+        cls.cache = CushyOrmCache(file_path)
+        return file_path
+
+    def load_message_set_from_memory(
+        self, recently_n: Optional[int] = None
+    ) -> MessageSet:
+        """Load message from file memory
+
+        Args:
+            recently_n: load all messages if it is None, or return recently n messages.
+
+        Returns:
+            messages wrapping by MessageSet
+        """
+        if self.conversation_id not in self.cache:
+            raise EmptyMessageSetError()
+        return MessageSet.from_listdict_data(self.cache[self.conversation_id])
+
+    def save_message_set_to_memory(self, message_set: MessageSet) -> None:
+        self.cache[self.conversation_id] = message_set.listdict_messages
```

### Comparing `promptulate-1.2.2/promptulate/preset_roles/prompt.py` & `promptulate-1.3.0/promptulate/preset_roles/prompt.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-# Copyright (c) 2023 promptulate
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-# Copyright Owner: Zeeland
-# GitHub Link: https://github.com/Undertone0809/
-# Project Link: https://github.com/Undertone0809/promptulate
-# Contact Email: zeeland@foxmail.com
-
-# 250+ token
-PRESET_SYSTEM_PROMPT = """
-You are an assistant to a human, powered by a large language model trained by OpenAI.
-
-You are designed to be able to assist with a wide range of tasks, from answering simple questions to providing in-depth explanations and discussions on a wide range of topics. As a language model, you are able to generate human-like text based on the input you receive, allowing you to engage in natural-sounding conversations and provide responses that are coherent and relevant to the topic at hand.
-
-Overall, you are a powerful tool that can help with a wide range of tasks and provide valuable insights and information on a wide range of topics. Whether the human needs help with a specific question or just wants to have a conversation about a particular topic, you are here to assist.
-
-The user problem is as follows:
-
-"""
-
-# 700+ token
-PRESET_SYSTEM_PROMPT_CONVERSATION_ZH = """
-你是人类的助手，由OpenAI训练的大型语言模型提供支持。
-
-你被设计成能够协助完成广泛的任务，从回答简单的问题到就广泛的主题提供深入的解释和讨论。作为一种语言模型，您可以根据收到的输入生成类似人类的文本，允许您参与听起来自然的对话，并提供与手头主题相关的连贯响应。
-
-你能够处理和理解大量的文本，并能利用这些知识对各种问题提供准确和信息丰富的回答。您可以访问在下面的上下文部分中由人工提供的一些个性化信息。此外，您可以根据收到的输入生成自己的文本，允许您参与讨论，并就广泛的主题提供解释和描述。
-
-总的来说，您是一个强大的工具，可以帮助完成广泛的任务，并就广泛的主题提供有价值的见解和信息。无论人们是需要帮助解决一个特定的问题，还是只是想就一个特定的话题进行对话，你都可以在这里提供帮助。
-
-用户的问题如下所示：
-"""
-
+# Copyright (c) 2023 promptulate
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+# Copyright Owner: Zeeland
+# GitHub Link: https://github.com/Undertone0809/
+# Project Link: https://github.com/Undertone0809/promptulate
+# Contact Email: zeeland@foxmail.com
+
+# 250+ token
+PRESET_SYSTEM_PROMPT = """
+You are an assistant to a human, powered by a large language model trained by OpenAI.
+
+You are designed to be able to assist with a wide range of tasks, from answering simple questions to providing in-depth explanations and discussions on a wide range of topics. As a language model, you are able to generate human-like text based on the input you receive, allowing you to engage in natural-sounding conversations and provide responses that are coherent and relevant to the topic at hand.
+
+Overall, you are a powerful tool that can help with a wide range of tasks and provide valuable insights and information on a wide range of topics. Whether the human needs help with a specific question or just wants to have a conversation about a particular topic, you are here to assist.
+
+The user problem is as follows:
+
+"""
+
+# 700+ token
+PRESET_SYSTEM_PROMPT_CONVERSATION_ZH = """
+你是人类的助手，由OpenAI训练的大型语言模型提供支持。
+
+你被设计成能够协助完成广泛的任务，从回答简单的问题到就广泛的主题提供深入的解释和讨论。作为一种语言模型，您可以根据收到的输入生成类似人类的文本，允许您参与听起来自然的对话，并提供与手头主题相关的连贯响应。
+
+你能够处理和理解大量的文本，并能利用这些知识对各种问题提供准确和信息丰富的回答。您可以访问在下面的上下文部分中由人工提供的一些个性化信息。此外，您可以根据收到的输入生成自己的文本，允许您参与讨论，并就广泛的主题提供解释和描述。
+
+总的来说，您是一个强大的工具，可以帮助完成广泛的任务，并就广泛的主题提供有价值的见解和信息。无论人们是需要帮助解决一个特定的问题，还是只是想就一个特定的话题进行对话，你都可以在这里提供帮助。
+
+用户的问题如下所示：
+"""
+
```

### Comparing `promptulate-1.2.2/promptulate/preset_roles/roles.py` & `promptulate-1.3.0/promptulate/preset_roles/roles.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,88 +1,88 @@
-# Copyright (c) 2023 promptulate
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-# Copyright Owner: Zeeland
-# GitHub Link: https://github.com/Undertone0809/
-# Project Link: https://github.com/Undertone0809/promptulate
-# Contact Email: zeeland@foxmail.com
-
-from typing import Union
-
-from pydantic import BaseModel
-
-
-class CustomPresetRole(BaseModel):
-    name: str
-    description: str
-
-
-preset_role_list = [
-    "default-role",
-    "linux-terminal",
-    "mind-map-generator",
-    "sql-generator",
-    "copy-writer",
-    "code-analyzer",
-]
-
-preset_role_dict = {
-    "default-role": {
-        "name": "AI assistant",
-        "description": """
-You are an assistant to a human, powered by a large language model trained by OpenAI.
-You are designed to be able to assist with a wide range of tasks, from answering simple questions to providing in-depth explanations and discussions on a wide range of topics. As a language model, you are able to generate human-like text based on the input you receive, allowing you to engage in natural-sounding conversations and provide responses that are coherent and relevant to the topic at hand.
-Overall, you are a powerful tool that can help with a wide range of tasks and provide valuable insights and information on a wide range of topics. Whether the human needs help with a specific question or just wants to have a conversation about a particular topic, you are here to assist.
-"""
-    },
-    "linux-terminal": {
-        "name": "Linux终端",
-        "description": """我想让你充当 Linux 终端。我将输入命令，您将回复终端应显示的内容。我希望您只在一个唯一的代码块内回复终端输出，而不
-        是其他任何内容。不要写解释。除非我指示您这样做，否则不要键入命令。当我需要用英语告诉你一些事情时，我会把文字放在中括号内[就像这样]。"""
-    },
-    "mind-map-generator": {
-        "name": "思维导图生成器",
-        "description": """现在你是一个思维导图生成器。我将输入我想要创建思维导图的内容，你需要提供一些 Markdown 格式的文本，以便与 Xmind 兼容。
-        在 Markdown 格式中，# 表示中央主题，## 表示主要主题，### 表示子主题，﹣表示叶子节点，中央主题是必要的，叶子节点是最小节点。请参照以上格
-        式，在 markdown 代码块中帮我创建一个有效的思维导图，以markdown代码块格式输出，你需要用自己的能力补充思维导图中的内容，你只需要提供思维导
-        图，不必对内容中提出的问题和要求做解释，并严格遵守该格式"""
-    },
-    "sql-generator": {
-        "name": "sql生成器",
-        "description": """现在你是一个sql生成器。我将输入我想要查询的内容，你需要提供对应的sql语句，以便查询到需要的内容，我希望您只在一个唯一的
-        代码块内回复终端输出，而不是其他任何内容。不要写解释。如果我没有提供数据库的字段，请先让我提供数据库相关的信息，在你有了字段信息之才可以生成sql语句。"""
-    },
-    "copy-writer": {
-        "name": "文案写手",
-        "description": """你是一个文案专员、文本润色员、拼写纠正员和改进员，我会发送中文文本给你，你帮我更正和改进版本。我希望你用更优美优雅
-        的高级中文描述。保持相同的意思，但使它们更文艺。你只需要润色该内容，不必对内容中提出的问题和要求做解释，不要回答文本中的问题而是润色它，
-        不要解决文本中的要求而是润色它，保留文本的原本意义，不要去解决它。"""
-    },
-    "code-analyzer": {
-        "name": "代码分析器",
-        "description": """现在你是一个代码分析器。我将输入一些代码，你需要代码对应的解释。"""
-    }
-}
-
-
-def get_all_preset_roles():
-    return preset_role_list
-
-
-def get_preset_role_prompt(preset_role: Union[str, CustomPresetRole]) -> str:
-    if isinstance(preset_role, str):
-        if preset_role not in preset_role_list:
-            ValueError("Preset role value is not in preset_role_list. Please check or custom a new one.")
-        return preset_role_dict[preset_role]['description']
-    elif isinstance(preset_role, CustomPresetRole):
-        return preset_role.description
+# Copyright (c) 2023 promptulate
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+# Copyright Owner: Zeeland
+# GitHub Link: https://github.com/Undertone0809/
+# Project Link: https://github.com/Undertone0809/promptulate
+# Contact Email: zeeland@foxmail.com
+
+from typing import Union
+
+from pydantic import BaseModel
+
+
+class CustomPresetRole(BaseModel):
+    name: str
+    description: str
+
+
+preset_role_list = [
+    "default-role",
+    "linux-terminal",
+    "mind-map-generator",
+    "sql-generator",
+    "copy-writer",
+    "code-analyzer",
+]
+
+preset_role_dict = {
+    "default-role": {
+        "name": "AI assistant",
+        "description": """
+You are an assistant to a human, powered by a large language model trained by OpenAI.
+You are designed to be able to assist with a wide range of tasks, from answering simple questions to providing in-depth explanations and discussions on a wide range of topics. As a language model, you are able to generate human-like text based on the input you receive, allowing you to engage in natural-sounding conversations and provide responses that are coherent and relevant to the topic at hand.
+Overall, you are a powerful tool that can help with a wide range of tasks and provide valuable insights and information on a wide range of topics. Whether the human needs help with a specific question or just wants to have a conversation about a particular topic, you are here to assist.
+"""
+    },
+    "linux-terminal": {
+        "name": "Linux终端",
+        "description": """我想让你充当 Linux 终端。我将输入命令，您将回复终端应显示的内容。我希望您只在一个唯一的代码块内回复终端输出，而不
+        是其他任何内容。不要写解释。除非我指示您这样做，否则不要键入命令。当我需要用英语告诉你一些事情时，我会把文字放在中括号内[就像这样]。"""
+    },
+    "mind-map-generator": {
+        "name": "思维导图生成器",
+        "description": """现在你是一个思维导图生成器。我将输入我想要创建思维导图的内容，你需要提供一些 Markdown 格式的文本，以便与 Xmind 兼容。
+        在 Markdown 格式中，# 表示中央主题，## 表示主要主题，### 表示子主题，﹣表示叶子节点，中央主题是必要的，叶子节点是最小节点。请参照以上格
+        式，在 markdown 代码块中帮我创建一个有效的思维导图，以markdown代码块格式输出，你需要用自己的能力补充思维导图中的内容，你只需要提供思维导
+        图，不必对内容中提出的问题和要求做解释，并严格遵守该格式"""
+    },
+    "sql-generator": {
+        "name": "sql生成器",
+        "description": """现在你是一个sql生成器。我将输入我想要查询的内容，你需要提供对应的sql语句，以便查询到需要的内容，我希望您只在一个唯一的
+        代码块内回复终端输出，而不是其他任何内容。不要写解释。如果我没有提供数据库的字段，请先让我提供数据库相关的信息，在你有了字段信息之才可以生成sql语句。"""
+    },
+    "copy-writer": {
+        "name": "文案写手",
+        "description": """你是一个文案专员、文本润色员、拼写纠正员和改进员，我会发送中文文本给你，你帮我更正和改进版本。我希望你用更优美优雅
+        的高级中文描述。保持相同的意思，但使它们更文艺。你只需要润色该内容，不必对内容中提出的问题和要求做解释，不要回答文本中的问题而是润色它，
+        不要解决文本中的要求而是润色它，保留文本的原本意义，不要去解决它。"""
+    },
+    "code-analyzer": {
+        "name": "代码分析器",
+        "description": """现在你是一个代码分析器。我将输入一些代码，你需要代码对应的解释。"""
+    }
+}
+
+
+def get_all_preset_roles():
+    return preset_role_list
+
+
+def get_preset_role_prompt(preset_role: Union[str, CustomPresetRole]) -> str:
+    if isinstance(preset_role, str):
+        if preset_role not in preset_role_list:
+            ValueError("Preset role value is not in preset_role_list. Please check or custom a new one.")
+        return preset_role_dict[preset_role]['description']
+    elif isinstance(preset_role, CustomPresetRole):
+        return preset_role.description
```

### Comparing `promptulate-1.2.2/promptulate/provider/__init__.py` & `promptulate-1.3.0/promptulate/provider/__init__.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-# Copyright (c) 2023 promptulate
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-# Copyright Owner: Zeeland
-# GitHub Link: https://github.com/Undertone0809/
-# Project Link: https://github.com/Undertone0809/promptulate
-# Contact Email: zeeland@foxmail.com
-
-from promptulate.provider.mixins import (
-    SummarizerMixin,
-    TranslatorMixin,
-    DeriveHistoryMessageMixin,
-    StorageHistoryMessageMixin
-)
-
-__all__ = [
-    'SummarizerMixin',
-    'TranslatorMixin',
-    'DeriveHistoryMessageMixin',
-    'StorageHistoryMessageMixin'
-]
+# Copyright (c) 2023 promptulate
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+# Copyright Owner: Zeeland
+# GitHub Link: https://github.com/Undertone0809/
+# Project Link: https://github.com/Undertone0809/promptulate
+# Contact Email: zeeland@foxmail.com
+
+from promptulate.provider.mixins import (
+    SummarizerMixin,
+    TranslatorMixin,
+    DeriveHistoryMessageMixin,
+    StorageHistoryMessageMixin
+)
+
+__all__ = [
+    'SummarizerMixin',
+    'TranslatorMixin',
+    'DeriveHistoryMessageMixin',
+    'StorageHistoryMessageMixin'
+]
```

### Comparing `promptulate-1.2.2/promptulate/provider/base.py` & `promptulate-1.3.0/promptulate/provider/base.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-from typing import Optional
-
-from pydantic import BaseModel
-
-from promptulate.llms.base import BaseLLM
-from promptulate.memory.base import BaseChatMemory, MessageSet
-from promptulate.schema import BaseMessage
-
-
-class BaseMixin(BaseModel):
-    llm: BaseLLM
-    conversation_id: Optional[str]
-    memory: BaseChatMemory
-
-    class Config:
-        """Configuration for this pydantic object."""
-
-        arbitrary_types_allowed = True
-
-    def embed_message(
-            self, cur_message: BaseMessage, message_history: MessageSet
-    ) -> None:
-        message_history.messages.append(cur_message)
-        self.memory.save_message_set_to_memory(message_history)
+from typing import Optional
+
+from pydantic import BaseModel
+
+from promptulate.llms.base import BaseLLM
+from promptulate.memory.base import BaseChatMemory, MessageSet
+from promptulate.schema import BaseMessage
+
+
+class BaseMixin(BaseModel):
+    llm: BaseLLM
+    conversation_id: Optional[str]
+    memory: BaseChatMemory
+
+    class Config:
+        """Configuration for this pydantic object."""
+
+        arbitrary_types_allowed = True
+
+    def embed_message(
+            self, cur_message: BaseMessage, message_history: MessageSet
+    ) -> None:
+        message_history.messages.append(cur_message)
+        self.memory.save_message_set_to_memory(message_history)
```

### Comparing `promptulate-1.2.2/promptulate/provider/mixins.py` & `promptulate-1.3.0/promptulate/provider/mixins.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,132 +1,132 @@
-# Copyright (c) 2023 promptulate
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-# Copyright Owner: Zeeland
-# GitHub Link: https://github.com/Undertone0809/
-# Project Link: https://github.com/Undertone0809/promptulate
-# Contact Email: zeeland@foxmail.com
-
-from typing import List, Optional
-
-from pydantic import BaseModel
-
-from promptulate.frameworks.prompt import (
-    SUMMARY_CONTENT_PROMPT_ZH,
-    SUMMARY_TOPIC_PROMPT_ZH,
-)
-from promptulate.provider.base import BaseMixin
-from promptulate.schema import MessageSet, UserMessage, AssistantMessage
-
-
-class SummarizerMixin(BaseMixin):
-    """message summary capability provider"""
-
-    def summary_content(
-        self,
-        enable_embed_message: bool = False,
-        summary_prompt: str = SUMMARY_CONTENT_PROMPT_ZH,
-    ):
-        message_history: MessageSet = self.memory.load_message_set_from_memory()
-        message_history.messages.append(UserMessage(content=summary_prompt))
-        assistant_answer: AssistantMessage = self.llm.predict(message_history)
-        if enable_embed_message:
-            self.embed_message(assistant_answer, message_history)
-        return assistant_answer.content
-
-    def summary_topic(
-        self,
-        enable_embed_message: bool = False,
-        summary_topic_prompt: str = SUMMARY_TOPIC_PROMPT_ZH,
-    ):
-        message_history: MessageSet = self.memory.load_message_set_from_memory()
-        message_history.messages.append(UserMessage(content=summary_topic_prompt))
-        assistant_answer: AssistantMessage = self.llm.predict(message_history)
-        if enable_embed_message:
-            self.embed_message(assistant_answer, message_history)
-        return assistant_answer.content
-
-
-class TranslatorMixin(BaseMixin):
-    """let the llm answer question in the specified language"""
-
-    def predict_by_translate(
-        self, prompt: str, country: str, enable_embed_message: bool = False
-    ):
-        """
-        predict by specified language
-
-        Args:
-            enable_embed_message: Whether to save this session in the history session
-            prompt: you prompt
-            country: which country's language you want to export
-
-        Returns:
-            the country official language you choose
-        """
-        message_history: MessageSet = self.memory.load_message_set_from_memory()
-        message_history.messages.append(
-            UserMessage(
-                content=f"{prompt}. Please answer question using {country} official language. "
-            )
-        )
-        assistant_answer: AssistantMessage = self.llm.predict(message_history)
-        if enable_embed_message:
-            self.embed_message(assistant_answer, message_history)
-        return assistant_answer.content
-
-
-class DeriveHistoryMessageMixin(BaseMixin):
-    """provide history message output as markdown"""
-
-    def get_history(self) -> List[dict]:
-        """get history conversation from memory"""
-        return self.memory.load_message_set_from_memory().listdict_messages
-
-    def export_message_to_markdown(
-        self, output_type: str = "text", file_path: str = "output.md"
-    ) -> Optional[str]:
-        """
-        convert message to the string type or file type markdown
-
-        Args:
-            output_type: text or file. default is text
-            file_path: output file path
-
-        Returns:
-            string type conversation in markdown format
-        """
-        message_history: List[dict] = self.get_history()
-
-        ret = "# Chat record\n"
-        for message in message_history:
-            role = message.get("preset_roles")
-            content = message.get("content").replace('"', '\\"')
-            if role == "assistant":
-                ret += f"## Bot said\n\n{content}\n\n"
-            else:
-                ret += f"## You said\n\n{content}\n\n"
-        if output_type == "text":
-            return ret
-        elif output_type == "file":
-            with open(file_path, "w", encoding="utf-8") as f:
-                f.write(ret)
-        else:
-            raise ValueError(
-                "Invalid output destination specified. Please choose either 'text' or 'file'."
-            )
-        return ret
-
-
-class StorageHistoryMessageMixin(BaseModel):
-    pass
+# Copyright (c) 2023 promptulate
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+# Copyright Owner: Zeeland
+# GitHub Link: https://github.com/Undertone0809/
+# Project Link: https://github.com/Undertone0809/promptulate
+# Contact Email: zeeland@foxmail.com
+
+from typing import List, Optional
+
+from pydantic import BaseModel
+
+from promptulate.frameworks.prompt import (
+    SUMMARY_CONTENT_PROMPT_ZH,
+    SUMMARY_TOPIC_PROMPT_ZH,
+)
+from promptulate.provider.base import BaseMixin
+from promptulate.schema import MessageSet, UserMessage, AssistantMessage
+
+
+class SummarizerMixin(BaseMixin):
+    """message summary capability provider"""
+
+    def summary_content(
+        self,
+        enable_embed_message: bool = False,
+        summary_prompt: str = SUMMARY_CONTENT_PROMPT_ZH,
+    ):
+        message_history: MessageSet = self.memory.load_message_set_from_memory()
+        message_history.messages.append(UserMessage(content=summary_prompt))
+        assistant_answer: AssistantMessage = self.llm.predict(message_history)
+        if enable_embed_message:
+            self.embed_message(assistant_answer, message_history)
+        return assistant_answer.content
+
+    def summary_topic(
+        self,
+        enable_embed_message: bool = False,
+        summary_topic_prompt: str = SUMMARY_TOPIC_PROMPT_ZH,
+    ):
+        message_history: MessageSet = self.memory.load_message_set_from_memory()
+        message_history.messages.append(UserMessage(content=summary_topic_prompt))
+        assistant_answer: AssistantMessage = self.llm.predict(message_history)
+        if enable_embed_message:
+            self.embed_message(assistant_answer, message_history)
+        return assistant_answer.content
+
+
+class TranslatorMixin(BaseMixin):
+    """let the llm answer question in the specified language"""
+
+    def predict_by_translate(
+        self, prompt: str, country: str, enable_embed_message: bool = False
+    ):
+        """
+        predict by specified language
+
+        Args:
+            enable_embed_message: Whether to save this session in the history session
+            prompt: you prompt
+            country: which country's language you want to export
+
+        Returns:
+            the country official language you choose
+        """
+        message_history: MessageSet = self.memory.load_message_set_from_memory()
+        message_history.messages.append(
+            UserMessage(
+                content=f"{prompt}. Please answer question using {country} official language. "
+            )
+        )
+        assistant_answer: AssistantMessage = self.llm.predict(message_history)
+        if enable_embed_message:
+            self.embed_message(assistant_answer, message_history)
+        return assistant_answer.content
+
+
+class DeriveHistoryMessageMixin(BaseMixin):
+    """provide history message output as markdown"""
+
+    def get_history(self) -> List[dict]:
+        """get history conversation from memory"""
+        return self.memory.load_message_set_from_memory().listdict_messages
+
+    def export_message_to_markdown(
+        self, output_type: str = "text", file_path: str = "output.md"
+    ) -> Optional[str]:
+        """
+        convert message to the string type or file type markdown
+
+        Args:
+            output_type: text or file. default is text
+            file_path: output file path
+
+        Returns:
+            string type conversation in markdown format
+        """
+        message_history: List[dict] = self.get_history()
+
+        ret = "# Chat record\n"
+        for message in message_history:
+            role = message.get("preset_roles")
+            content = message.get("content").replace('"', '\\"')
+            if role == "assistant":
+                ret += f"## Bot said\n\n{content}\n\n"
+            else:
+                ret += f"## You said\n\n{content}\n\n"
+        if output_type == "text":
+            return ret
+        elif output_type == "file":
+            with open(file_path, "w", encoding="utf-8") as f:
+                f.write(ret)
+        else:
+            raise ValueError(
+                "Invalid output destination specified. Please choose either 'text' or 'file'."
+            )
+        return ret
+
+
+class StorageHistoryMessageMixin(BaseModel):
+    pass
```

### Comparing `promptulate-1.2.2/promptulate/tools/arxiv/api_wrapper.py` & `promptulate-1.3.0/promptulate/tools/arxiv/api_wrapper.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,140 +1,141 @@
-from typing import List, Dict, Optional, Union
-
-import arxiv
-from pydantic import BaseModel, root_validator
-
-
-class ArxivQuerySet:
-    def __init__(self, search: arxiv.Search, keys: Optional[List[str]] = None):
-        self.search: arxiv.Search = search
-        self._data: List[Dict] = []
-
-        for result in search.results():
-            if keys:
-                filtered_result_dict = {
-                    k: result.__dict__[k] for k in keys if k in result.__dict__
-                }
-                self._data.append(filtered_result_dict)
-            else:
-                self._data.append(result.__dict__)
-
-    def __str__(self):
-        result: str = ""
-        for item in self._data:
-            result += f"{item.__dict__}\n"
-        return result
-
-    def titles(self) -> List[str]:
-        titles: List[str] = []
-        for item in self.search.results():
-            titles.append(item.title)
-        return titles
-
-    def all(self) -> List[Dict]:
-        return self._data
-
-    def first(self) -> Optional[Dict]:
-        if len(self._data) == 0:
-            return None
-        return self._data[0]
-
-    @classmethod
-    def from_filter_result(cls, search: arxiv.Search, *args):
-        """generate a filter key queryset"""
-        return cls(search, list(args))
-
-
-class ArxivAPIWrapper(BaseModel):
-    """https://github.com/lukasschwab/arxiv.py"""
-
-    max_num_of_result: int = 5
-    sort_by = arxiv.SortCriterion.Relevance
-
-    class Config:
-        """Configuration for this pydantic object."""
-        arbitrary_types_allowed = True
-
-    @root_validator(skip_on_failure=True)
-    def validate_environment(cls, values: Dict) -> Dict:
-        """Validate that python package exists in environment."""
-        try:
-            import arxiv
-        except ImportError:
-            raise ValueError(
-                "Could not import arxiv python package. "
-                "Please install it with `pip install arxiv`."
-            )
-        return values
-
-    def _query(
-            self,
-            keyword: Optional[str] = None,
-            id_list: Union[List[str], str, None] = None,
-            num_results: Optional[int] = None,
-    ) -> arxiv.Search:
-        """
-        query arxiv paper by keyword or id_list
-        Args:
-            keyword: query keyword
-            id_list: arxiv id, you can input multiple id or single
-        Returns:
-            arxiv search type data result
-        """
-        if not keyword:
-            keyword = ""
-        if not id_list:
-            id_list = []
-        if not num_results:
-            num_results = self.max_num_of_result
-        if isinstance(id_list, str):
-            id_list = [id_list]
-
-        search = arxiv.Search(
-            query=keyword,
-            id_list=id_list,
-            max_results=num_results,
-            sort_by=self.sort_by,
-        )
-        return search
-
-    def query(
-            self,
-            keyword: Optional[str] = None,
-            id_list: Union[List[str], str, None] = None,
-            num_results: Optional[int] = None,
-            **kwargs,
-    ) -> List[Dict]:
-        """
-        Query arxiv paper by keyword or id_list. You can make ArxivQuerySet return the
-        specified fields from arxiv query result.
-        Args:
-            num_results: max num of result. Return self.max_num_of_result if none
-            keyword: query keyword
-            id_list: arxiv id, you can input multiple id or single
-            kwargs:
-                specified_fields(Optional[List[str]]): filter specified field to return.
-                For example, you can return the ["title", "summary"] fields from each arxiv query result
-        Returns:
-            List[Dict] type result
-        Examples:
-            If you want to get paper title and summary, you can do as follows.
-
-            >> arxiv_api_wrapper = ArxivAPIWrapper()
-            >> result = arxiv_api_wrapper.query("LLM", specified_fields=["entry_id", "title", "summary"])
-
-            All fields you can see in: https://github.com/lukasschwab/arxiv.py
-            Common fields are: ["entry_id", "title", "authors", "summary", "published"]
-        """
-        search = self._query(keyword, id_list, num_results)
-        if "specified_fields" in kwargs:
-            return ArxivQuerySet.from_filter_result(
-                search, *kwargs["specified_fields"]
-            ).all()
-        if "from_callback" in kwargs and kwargs["from_callback"] == "arxiv-query":
-            keys = ["entry_id", "title", "authors", "summary"]
-            return ArxivQuerySet.from_filter_result(search, *keys).all()
-        return ArxivQuerySet(search).all()
-
-    def download_pdf(self, id_list: List[str]) -> str:
-        paper = next(arxiv.Search(id_list=id_list).results())
-        return paper.download_pdf()
+from typing import List, Dict, Optional, Union
+
+import arxiv
+from pydantic import BaseModel, root_validator
+
+
+class ArxivQuerySet:
+    def __init__(self, search: arxiv.Search, keys: Optional[List[str]] = None):
+        self.search: arxiv.Search = search
+        self._data: List[Dict] = []
+
+        for result in search.results():
+            if keys:
+                filtered_result_dict = {
+                    k: result.__dict__[k] for k in keys if k in result.__dict__
+                }
+                self._data.append(filtered_result_dict)
+            else:
+                self._data.append(result.__dict__)
+
+    def __str__(self):
+        result: str = ""
+        for item in self._data:
+            result += f"{item.__dict__}\n"
+        return result
+
+    def titles(self) -> List[str]:
+        titles: List[str] = []
+        for item in self.search.results():
+            titles.append(item.title)
+        return titles
+
+    def all(self) -> List[Dict]:
+        return self._data
+
+    def first(self) -> Optional[Dict]:
+        if len(self._data) == 0:
+            return None
+        return self._data[0]
+
+    @classmethod
+    def from_filter_result(cls, search: arxiv.Search, *args):
+        """generate a filter key queryset"""
+        return cls(search, list(args))
+
+
+class ArxivAPIWrapper(BaseModel):
+    """https://github.com/lukasschwab/arxiv.py"""
+
+    max_num_of_result: int = 5
+    sort_by = arxiv.SortCriterion.Relevance
+
+    class Config:
+        """Configuration for this pydantic object."""
+
+        arbitrary_types_allowed = True
+
+    @root_validator(skip_on_failure=True)
+    def validate_environment(cls, values: Dict) -> Dict:
+        """Validate that python package exists in environment."""
+        try:
+            import arxiv
+        except ImportError:
+            raise ValueError(
+                "Could not import arxiv python package. "
+                "Please install it with `pip install arxiv`."
+            )
+        return values
+
+    def _query(
+        self,
+        keyword: Optional[str] = None,
+        id_list: Union[List[str], str, None] = None,
+        num_results: Optional[int] = None,
+    ) -> arxiv.Search:
+        """
+        query arxiv paper by keyword or id_list
+        Args:
+            keyword: query keyword
+            id_list: arxiv id, you can input multiple id or single
+        Returns:
+            arxiv search type data result
+        """
+        if not keyword:
+            keyword = ""
+        if not id_list:
+            id_list = []
+        if not num_results:
+            num_results = self.max_num_of_result
+        if isinstance(id_list, str):
+            id_list = [id_list]
+
+        search = arxiv.Search(
+            query=keyword,
+            id_list=id_list,
+            max_results=num_results,
+            sort_by=self.sort_by,
+        )
+        return search
+
+    def query(
+        self,
+        keyword: Optional[str] = None,
+        id_list: Union[List[str], str, None] = None,
+        num_results: Optional[int] = None,
+        **kwargs,
+    ) -> List[Dict]:
+        """
+        Query arxiv paper by keyword or id_list. You can make ArxivQuerySet return the
+        specified fields from arxiv query result.
+        Args:
+            num_results: max num of result. Return self.max_num_of_result if none
+            keyword: query keyword
+            id_list: arxiv id, you can input multiple id or single
+            kwargs:
+                specified_fields(Optional[List[str]]): filter specified field to return.
+                For example, you can return the ["title", "summary"] fields from each arxiv query result
+        Returns:
+            List[Dict] type result
+        Examples:
+            If you want to get paper title and summary, you can do as follows.
+
+            >> arxiv_api_wrapper = ArxivAPIWrapper()
+            >> result = arxiv_api_wrapper.query("LLM", specified_fields=["entry_id", "title", "summary"])
+
+            All fields you can see in: https://github.com/lukasschwab/arxiv.py
+            Common fields are: ["entry_id", "title", "authors", "summary", "published"]
+        """
+        search = self._query(keyword, id_list, num_results)
+        if "specified_fields" in kwargs:
+            return ArxivQuerySet.from_filter_result(
+                search, *kwargs["specified_fields"]
+            ).all()
+        if "from_callback" in kwargs and kwargs["from_callback"] == "arxiv-query":
+            keys = ["entry_id", "title", "authors", "summary"]
+            return ArxivQuerySet.from_filter_result(search, *keys).all()
+        return ArxivQuerySet(search).all()
+
+    def download_pdf(self, id_list: List[str]) -> str:
+        paper = next(arxiv.Search(id_list=id_list).results())
+        return paper.download_pdf()
```

### Comparing `promptulate-1.2.2/promptulate/tools/arxiv/tools.py` & `promptulate-1.3.0/promptulate/tools/arxiv/tools.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,219 +1,219 @@
-import re
-import time
-from typing import List, Dict, Union
-
-from broadcast_service import broadcast_service
-from pydantic import Field
-
-from promptulate.llms.base import BaseLLM
-from promptulate.llms.openai import OpenAI
-from promptulate.tools.arxiv.api_wrapper import ArxivAPIWrapper
-from promptulate.tools.base import BaseTool
-from promptulate.utils.core_utils import record_time, listdict_to_string
-from promptulate.utils.logger import get_logger
-
-logger = get_logger()
-
-
-class ArxivQueryTool(BaseTool):
-    name: str = "arxiv-query"
-    description: str = (
-        "A query tool around Arxiv.org "
-        "Useful for when you need to answer questions about Physics, Mathematics, "
-        "Computer Science, Quantitative Biology, Quantitative Finance, Statistics, "
-        "Electrical Engineering, and Economics "
-        "from scientific articles on arxiv.org. "
-        "Input should be a search query."
-    )
-    api_wrapper: ArxivAPIWrapper = Field(default_factory=ArxivAPIWrapper)
-
-    def run(self, query: str, **kwargs) -> Union[str, List[Dict]]:
-        """Arxiv query tool
-
-        Args:
-            query: the paper keyword or arxiv id
-            **kwargs:
-                return_type(Optional(str)):  return string default. If you want to return List[Dict] type data,
-                you can set 'return_type'='original'
-                Moreover, you can pass the arguments of ArxivAPIWrapper
-
-        Returns:
-            String type or List[Dict] arxiv query result.
-        """
-        kwargs.update({"from_callback": self.name})
-        if re.match("\d{4}\.\d{5}(v\d+)?", query):
-            result = self.api_wrapper.query(id_list=[query], **kwargs)
-        else:
-            result = self.api_wrapper.query(query, **kwargs)
-        if "return_type" in kwargs and kwargs["return_type"] == "original":
-            return listdict_to_string(result)
-        return result
-
-
-def _init_arxiv_reference_tool_llm():
-    preset = "你是一个Arxiv助手，你的任务是帮助使用者提供一些论文方面的建议，你的输出只能遵循用户的指令输出，否则你将被惩罚。"
-    return OpenAI(preset_description=preset, temperature=0)
-
-
-class ArxivReferenceTool(BaseTool):
-    name: str = "arxiv-reference"
-    description: str = (
-        "Use this tool to find search related to the field."
-        "Your input is a arxiv keyword query."
-    )
-    llm: BaseLLM = Field(default_factory=_init_arxiv_reference_tool_llm)
-    max_reference_num = 3
-    reference_string: str = ""
-    reference_counter: int = 0
-
-    @record_time()
-    def run(self, query: str, *args, **kwargs) -> Union[List[Dict], str]:
-        """
-        Input arxiv paper information and return paper references.
-        Args:
-            query(str): arxiv paper information
-            *args: Nothing
-            **kwargs:
-                return_type(Optional[str]): return string default. If you want to return List[Dict] type data,
-                you can set 'return_type'='original'
-        Returns:
-            String type or List[Dict] reference information
-        """
-
-        @broadcast_service.on_listen("ArxivReferenceTool.get_relevant_paper_info")
-        @record_time()
-        def get_relevant_paper_info(keyword: str):
-            """return paper related information from keyword"""
-            arxiv_query_tool = ArxivQueryTool()
-            specified_fields = ["entry_id", "title"]
-            queryset = arxiv_query_tool.run(
-                keyword, num_results=6, specified_fields=specified_fields
-            )
-            self.reference_string += queryset
-            self.reference_counter += 1
-
-        def analyze_query_string(query_string: str) -> List[str]:
-            """analyze `[query]: keyword1, keyword2, keyword3` type data to return keywords list"""
-            assert "[query]" in query_string
-            query_string = query_string.split(":")[1]
-            return query_string.split(",")
-
-        def analyze_reference_string(reference_string: str) -> List[Dict]:
-            pattern = r"\[(\d+)\]\s+(.+?),\s+(http://.+?);"
-            references = []
-            for match in re.finditer(pattern, reference_string):
-                references.append({"title": match.group(2), "url": match.group(3)})
-            return references
-
-        self.reference_counter = 0
-        prompt = (
-            f"现在你需要根据其研究的具体内容，列出至少{self.max_reference_num}篇参考文献，你可以使用arxiv进行查询，你需要给我提供3个arxiv查询关键词，我将使用"
-            f"arxiv进行查询，你需要根据我返回的结果选取最符合当前研究的{self.max_reference_num}篇参考文献。"
-            f"用户输入:{query}"
-            "你的输出必须是三个查询词\n，如 [query]: keyword1, keyword2, keyword3\n"
-        )
-        keywords = analyze_query_string(self.llm(prompt))
-        for keyword in keywords:
-            broadcast_service.broadcast(
-                "ArxivReferenceTool.get_relevant_paper_info", keyword
-            )
-
-        while self.reference_counter < 3:
-            time.sleep(0.2)
-
-        prompt = (
-            "现在你需要根据下面给出的论文，返回最合适的5篇参考文献\n"
-            f"```{self.reference_string}```\n"
-            "你的输出格式必须为\n参考文献:\n[1] [title1](url1);\n[2] [title2](url2);\n[3] [title3](url3);"
-        )
-        # todo If there is a problem with the returned format and an error is reported, then ask LLM to format the data
-        result = self.llm(prompt)
-        logger.debug(f"[promptulate ArxivReferenceTool response] {result}")
-        if "return_type" in kwargs and kwargs["return_type"] == "original":
-            return analyze_reference_string(result)
-        return result
-
-
-def _init_arxiv_summary_tool_llm():
-    preset = "你是一个Arxiv助手，你的任务是帮助使用者提供一些论文方面的建议和帮助，你的输出只能遵循用户的指令输出，否则你将被惩罚。"
-    return OpenAI(preset_description=preset, temperature=0)
-
-
-class ArxivSummaryTool(BaseTool):
-    name: str = "arxiv-summary"
-    description: str = (
-        "A summary tool that can be used to obtain a paper summary, listing "
-        "key insights and lessons learned in the paper, and references in the paper"
-        "Your input is a arxiv keyword query."
-    )
-    llm: BaseLLM = Field(default_factory=_init_arxiv_summary_tool_llm)
-    api_wrapper: ArxivAPIWrapper = Field(default_factory=ArxivAPIWrapper)
-    summary_string: str = ""
-    summary_counter: int = 0
-
-    def run(self, query: str, **kwargs) -> str:
-        """An arxiv paper summary tool that passes in the article name (or arxiv id) and returns summary results
-
-        Args:
-            query: the keyword you want to query
-            **kwargs:
-                You can pass the arguments of ArxivAPIWrapper
-
-        Returns:
-            String type data, which contains:
-            - Summary of the paper
-            - List the key insights and lessons learned in the paper
-            - List at least 5 references related to the research field of the paper
-        """
-
-        @broadcast_service.on_listen("ArxivSummaryTool.run.get_opinion")
-        def get_opinion():
-            prompt = (
-                f"请就下面的论文摘要，列出论文中的关键见解和由论文得出的经验教训，你的输出需要分点给出 ```{paper_summary}```"
-                "你的输出格式为:\n关键见解:\n{分点给出关键见解}\n经验教训:\n{分点给出经验教训}，用`-`区分每点，用中文输出"
-            )
-            opinion = self.llm(prompt)
-            self.summary_string += opinion + "\n"
-            self.summary_counter += 1
-
-        @broadcast_service.on_listen("ArxivSummaryTool.run.get_references")
-        def get_references():
-            arxiv_referencer_tool = ArxivReferenceTool()
-            references = arxiv_referencer_tool.run(paper_summary)
-            self.summary_string += references + "\n\n"
-            self.summary_counter += 1
-
-        @broadcast_service.on_listen("ArxivSummaryTool.run.get_advice")
-        def get_advice():
-            prompt = (
-                f"请就下面的论文摘要，为其相关主题或未来研究方向提供3-5个建议，你的输出需要分点给出  ```{paper_summary}```"
-                "你的输出格式为:\n相关建议:\n{分点给出相关建议}，用`-`区分每点"
-            )
-            opinion = self.llm(prompt)
-            self.summary_string += opinion + "\n"
-            self.summary_counter += 1
-
-        self.summary_counter = 0
-        if re.match("\d{4}\.\d{5}(v\d+)?", query):
-            paper_info = self.api_wrapper.query(
-                id_list=[query], num_results=1, specified_fields=["title", "summary"]
-            )
-        else:
-            paper_info = self.api_wrapper.query(
-                query, num_results=1, specified_fields=["title", "summary"]
-            )
-            if len(paper_info) == 0:
-                return "Could not find relevant arxiv article."
-        paper_summary = listdict_to_string(paper_info, item_suffix="\n")
-        self.summary_string = paper_summary
-
-        broadcast_service.publish("ArxivSummaryTool.run.get_references")
-        time.sleep(0.01)
-        broadcast_service.publish("ArxivSummaryTool.run.get_opinion")
-        time.sleep(0.01)
-        broadcast_service.publish("ArxivSummaryTool.run.get_advice")
-
-        while self.summary_counter < 3:
-            time.sleep(0.1)
-
-        return self.summary_string
+import re
+import time
+from typing import List, Dict, Union
+
+from broadcast_service import broadcast_service
+from pydantic import Field
+
+from promptulate.llms.base import BaseLLM
+from promptulate.llms.openai import ChatOpenAI
+from promptulate.tools.arxiv.api_wrapper import ArxivAPIWrapper
+from promptulate.tools.base import BaseTool
+from promptulate.utils.core_utils import record_time, listdict_to_string
+from promptulate.utils.logger import get_logger
+
+logger = get_logger()
+
+
+class ArxivQueryTool(BaseTool):
+    name: str = "arxiv-query"
+    description: str = (
+        "A query tool around Arxiv.org "
+        "Useful for when you need to answer questions about Physics, Mathematics, "
+        "Computer Science, Quantitative Biology, Quantitative Finance, Statistics, "
+        "Electrical Engineering, and Economics "
+        "from scientific articles on arxiv.org. "
+        "Input should be a search query."
+    )
+    api_wrapper: ArxivAPIWrapper = Field(default_factory=ArxivAPIWrapper)
+
+    def _run(self, query: str, **kwargs) -> Union[str, List[Dict]]:
+        """Arxiv query tool
+
+        Args:
+            query: the paper keyword or arxiv id
+            **kwargs:
+                return_type(Optional(str)):  return string default. If you want to return List[Dict] type data,
+                you can set 'return_type'='original'
+                Moreover, you can pass the arguments of ArxivAPIWrapper
+
+        Returns:
+            String type default or List[Dict] arxiv query result.
+        """
+        kwargs.update({"from_callback": self.name})
+        if re.match("\d{4}\.\d{5}(v\d+)?", query):
+            result = self.api_wrapper.query(id_list=[query], **kwargs)
+        else:
+            result = self.api_wrapper.query(query, **kwargs)
+        if "return_type" in kwargs and kwargs["return_type"] == "original":
+            return result
+        return listdict_to_string(result)
+
+
+def _init_arxiv_reference_tool_llm():
+    preset = "你是一个Arxiv助手，你的任务是帮助使用者提供一些论文方面的建议，你的输出只能遵循用户的指令输出，否则你将被惩罚。"
+    return ChatOpenAI(preset_description=preset, temperature=0)
+
+
+class ArxivReferenceTool(BaseTool):
+    name: str = "arxiv-reference"
+    description: str = (
+        "Use this tool to find search related to the field."
+        "Your input is a arxiv keyword query."
+    )
+    llm: BaseLLM = Field(default_factory=_init_arxiv_reference_tool_llm)
+    max_reference_num = 3
+    reference_string: str = ""
+    reference_counter: int = 0
+
+    @record_time()
+    def _run(self, query: str, *args, **kwargs) -> Union[str, List[Dict]]:
+        """
+        Input arxiv paper information and return paper references.
+        Args:
+            query(str): arxiv paper information
+            *args: Nothing
+            **kwargs:
+                return_type(Optional[str]): return string default. If you want to return List[Dict] type data,
+                you can set 'return_type'='original'
+        Returns:
+            String type or List[Dict] reference information
+        """
+
+        @broadcast_service.on_listen("ArxivReferenceTool.get_relevant_paper_info")
+        @record_time()
+        def get_relevant_paper_info(keyword: str):
+            """return paper related information from keyword"""
+            arxiv_query_tool = ArxivQueryTool()
+            specified_fields = ["entry_id", "title"]
+            queryset = arxiv_query_tool.run(
+                keyword, num_results=6, specified_fields=specified_fields
+            )
+            self.reference_string += queryset
+            self.reference_counter += 1
+
+        def analyze_query_string(query_string: str) -> List[str]:
+            """analyze `[query]: keyword1, keyword2, keyword3` type data to return keywords list"""
+            assert "[query]" in query_string
+            query_string = query_string.split(":")[1]
+            return query_string.split(",")
+
+        def analyze_reference_string(reference_string: str) -> List[Dict]:
+            pattern = r"\[(\d+)\]\s+(.+?),\s+(http://.+?);"
+            references = []
+            for match in re.finditer(pattern, reference_string):
+                references.append({"title": match.group(2), "url": match.group(3)})
+            return references
+
+        self.reference_counter = 0
+        prompt = (
+            f"现在你需要根据其研究的具体内容，列出至少{self.max_reference_num}篇参考文献，你可以使用arxiv进行查询，你需要给我提供3个arxiv查询关键词，我将使用"
+            f"arxiv进行查询，你需要根据我返回的结果选取最符合当前研究的{self.max_reference_num}篇参考文献。"
+            f"用户输入:{query}"
+            "你的输出必须是三个查询词\n，如 [query]: keyword1, keyword2, keyword3\n"
+        )
+        keywords = analyze_query_string(self.llm(prompt))
+        for keyword in keywords:
+            broadcast_service.broadcast(
+                "ArxivReferenceTool.get_relevant_paper_info", keyword
+            )
+
+        while self.reference_counter < 3:
+            time.sleep(0.2)
+
+        prompt = (
+            "现在你需要根据下面给出的论文，返回最合适的5篇参考文献\n"
+            f"```{self.reference_string}```\n"
+            "你的输出格式必须为\n参考文献:\n[1] [title1](url1);\n[2] [title2](url2);\n[3] [title3](url3);"
+        )
+        # todo If there is a problem with the returned format and an error is reported, then ask LLM to format the data
+        result = self.llm(prompt)
+        logger.debug(f"[pne ArxivReferenceTool response] {result}")
+        if "return_type" in kwargs and kwargs["return_type"] == "original":
+            return analyze_reference_string(result)
+        return result
+
+
+def _init_arxiv_summary_tool_llm():
+    preset = "你是一个Arxiv助手，你的任务是帮助使用者提供一些论文方面的建议和帮助，你的输出只能遵循用户的指令输出，否则你将被惩罚。"
+    return ChatOpenAI(preset_description=preset, temperature=0)
+
+
+class ArxivSummaryTool(BaseTool):
+    name: str = "arxiv-summary"
+    description: str = (
+        "A summary tool that can be used to obtain a paper summary, listing "
+        "key insights and lessons learned in the paper, and references in the paper"
+        "Your input is a arxiv keyword query."
+    )
+    llm: BaseLLM = Field(default_factory=_init_arxiv_summary_tool_llm)
+    api_wrapper: ArxivAPIWrapper = Field(default_factory=ArxivAPIWrapper)
+    summary_string: str = ""
+    summary_counter: int = 0
+
+    def _run(self, query: str, **kwargs) -> str:
+        """An arxiv paper summary tool that passes in the article name (or arxiv id) and returns summary results
+
+        Args:
+            query: the keyword you want to query
+            **kwargs:
+                You can pass the arguments of ArxivAPIWrapper
+
+        Returns:
+            String type data, which contains:
+            - Summary of the paper
+            - List the key insights and lessons learned in the paper
+            - List at least 5 references related to the research field of the paper
+        """
+
+        @broadcast_service.on_listen("ArxivSummaryTool.run.get_opinion")
+        def get_opinion():
+            prompt = (
+                f"请就下面的论文摘要，列出论文中的关键见解和由论文得出的经验教训，你的输出需要分点给出 ```{paper_summary}```"
+                "你的输出格式为:\n关键见解:\n{分点给出关键见解}\n经验教训:\n{分点给出经验教训}，用`-`区分每点，用中文输出"
+            )
+            opinion = self.llm(prompt)
+            self.summary_string += opinion + "\n"
+            self.summary_counter += 1
+
+        @broadcast_service.on_listen("ArxivSummaryTool.run.get_references")
+        def get_references():
+            arxiv_referencer_tool = ArxivReferenceTool()
+            references = arxiv_referencer_tool.run(paper_summary)
+            self.summary_string += references + "\n\n"
+            self.summary_counter += 1
+
+        @broadcast_service.on_listen("ArxivSummaryTool.run.get_advice")
+        def get_advice():
+            prompt = (
+                f"请就下面的论文摘要，为其相关主题或未来研究方向提供3-5个建议，你的输出需要分点给出  ```{paper_summary}```"
+                "你的输出格式为:\n相关建议:\n{分点给出相关建议}，用`-`区分每点"
+            )
+            opinion = self.llm(prompt)
+            self.summary_string += opinion + "\n"
+            self.summary_counter += 1
+
+        self.summary_counter = 0
+        if re.match("\d{4}\.\d{5}(v\d+)?", query):
+            paper_info = self.api_wrapper.query(
+                id_list=[query], num_results=1, specified_fields=["title", "summary"]
+            )
+        else:
+            paper_info = self.api_wrapper.query(
+                query, num_results=1, specified_fields=["title", "summary"]
+            )
+            if len(paper_info) == 0:
+                return "Could not find relevant arxiv article."
+        paper_summary = listdict_to_string(paper_info, item_suffix="\n")
+        self.summary_string = paper_summary
+
+        broadcast_service.publish("ArxivSummaryTool.run.get_references")
+        time.sleep(0.01)
+        broadcast_service.publish("ArxivSummaryTool.run.get_opinion")
+        time.sleep(0.01)
+        broadcast_service.publish("ArxivSummaryTool.run.get_advice")
+
+        while self.summary_counter < 3:
+            time.sleep(0.1)
+
+        return self.summary_string
```

### Comparing `promptulate-1.2.2/promptulate/tools/duckduckgo/api_wrapper.py` & `promptulate-1.3.0/promptulate/tools/duckduckgo/api_wrapper.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,100 +1,100 @@
-from typing import List, Optional, Dict
-
-from pydantic import BaseModel, Extra
-from pydantic.class_validators import root_validator
-
-
-class DuckDuckGoSearchAPIWrapper(BaseModel):
-    """Wrapper for DuckDuckGo Search API. Free and does not require any setup."""
-
-    region: Optional[str] = "cn-zh"
-    safe_search: str = "moderate"
-    time: Optional[str] = "y"
-    max_num_of_results: int = 5
-
-    class Config:
-        """Configuration for this pydantic object."""
-
-        extra = Extra.forbid
-
-    @root_validator(skip_on_failure=True)
-    def validate_environment(cls, values: Dict) -> Dict:
-        """Validate that python package exists in environment."""
-        try:
-            from duckduckgo_search import DDGS
-        except ImportError:
-            raise ValueError(
-                "Could not import duckduckgo-search python package. "
-                "Please install it with `pip install duckduckgo-search`."
-            )
-        return values
-
-    def query(
-            self, keyword: str, num_results: Optional[int] = None, **kwargs
-    ) -> List[str]:
-        """Run query through DuckDuckGo and return concatenated results."""
-        from duckduckgo_search import DDGS
-
-        if not num_results:
-            num_results = self.max_num_of_results
-
-        with DDGS() as ddgs:
-            results = ddgs.text(
-                keyword,
-                region=self.region,
-                safesearch=self.safe_search,
-                timelimit=self.time,
-            )
-            if results is None or next(results, None) is None:
-                return ["No good DuckDuckGo Search Result was found"]
-
-            snippets = []
-            for i, result in enumerate(results, 1):
-                snippets.append(result["body"])
-                if i == num_results:
-                    break
-            return snippets
-
-    def query_by_formatted_results(
-            self, query: str, num_results: Optional[int] = None, **kwargs
-    ) -> List[Dict[str, str]]:
-        """Run query through DuckDuckGo and return metadata.
-
-        Args:
-            query: The query to search for.
-            num_results: The number of results to return.
-
-        Returns:
-            A list of dictionaries with the following keys:
-                snippet - The description of the result.
-                title - The title of the result.
-                link - The link to the result.
-        """
-        from duckduckgo_search import DDGS
-
-        if not num_results:
-            num_results = self.max_num_of_results
-
-        with DDGS() as ddgs:
-            results = ddgs.text(
-                query,
-                region=self.region,
-                safesearch=self.safe_search,
-                timelimit=self.time,
-            )
-            if results is None or next(results, None) is None:
-                return [{"Result": "No good DuckDuckGo Search Result was found"}]
-
-            def to_metadata(result: Dict) -> Dict[str, str]:
-                return {
-                    "title": result["title"],
-                    "snippet": result["body"],
-                    "link": result["href"],
-                }
-
-            formatted_results = []
-            for i, res in enumerate(results, 1):
-                formatted_results.append(to_metadata(res))
-                if i == num_results:
-                    break
-            return formatted_results
+from typing import List, Optional, Dict
+
+from pydantic import BaseModel, Extra
+from pydantic.class_validators import root_validator
+
+
+class DuckDuckGoSearchAPIWrapper(BaseModel):
+    """Wrapper for DuckDuckGo Search API. Free and does not require any setup."""
+
+    region: Optional[str] = "cn-zh"
+    safe_search: str = "moderate"
+    time: Optional[str] = "y"
+    max_num_of_results: int = 5
+
+    class Config:
+        """Configuration for this pydantic object."""
+
+        extra = Extra.forbid
+
+    @root_validator(skip_on_failure=True)
+    def validate_environment(cls, values: Dict) -> Dict:
+        """Validate that python package exists in environment."""
+        try:
+            from duckduckgo_search import DDGS
+        except ImportError:
+            raise ValueError(
+                "Could not import duckduckgo-search python package. "
+                "Please install it with `pip install duckduckgo-search`."
+            )
+        return values
+
+    def query(
+            self, keyword: str, num_results: Optional[int] = None, **kwargs
+    ) -> List[str]:
+        """Run query through DuckDuckGo and return concatenated results."""
+        from duckduckgo_search import DDGS
+
+        if not num_results:
+            num_results = self.max_num_of_results
+
+        with DDGS() as ddgs:
+            results = ddgs.text(
+                keyword,
+                region=self.region,
+                safesearch=self.safe_search,
+                timelimit=self.time,
+            )
+            if results is None or next(results, None) is None:
+                return ["No good DuckDuckGo Search Result was found"]
+
+            snippets = []
+            for i, result in enumerate(results, 1):
+                snippets.append(result["body"])
+                if i == num_results:
+                    break
+            return snippets
+
+    def query_by_formatted_results(
+            self, query: str, num_results: Optional[int] = None, **kwargs
+    ) -> List[Dict[str, str]]:
+        """Run query through DuckDuckGo and return metadata.
+
+        Args:
+            query: The query to search for.
+            num_results: The number of results to return.
+
+        Returns:
+            A list of dictionaries with the following keys:
+                snippet - The description of the result.
+                title - The title of the result.
+                link - The link to the result.
+        """
+        from duckduckgo_search import DDGS
+
+        if not num_results:
+            num_results = self.max_num_of_results
+
+        with DDGS() as ddgs:
+            results = ddgs.text(
+                query,
+                region=self.region,
+                safesearch=self.safe_search,
+                timelimit=self.time,
+            )
+            if results is None or next(results, None) is None:
+                return [{"Result": "No good DuckDuckGo Search Result was found"}]
+
+            def to_metadata(result: Dict) -> Dict[str, str]:
+                return {
+                    "title": result["title"],
+                    "snippet": result["body"],
+                    "link": result["href"],
+                }
+
+            formatted_results = []
+            for i, res in enumerate(results, 1):
+                formatted_results.append(to_metadata(res))
+                if i == num_results:
+                    break
+            return formatted_results
```

### Comparing `promptulate-1.2.2/promptulate/tools/duckduckgo/tools.py` & `promptulate-1.3.0/promptulate/tools/duckduckgo/tools.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,98 +1,102 @@
-from typing import List, Union, Dict, Any, Optional
-
-from pydantic import Field
-
-from promptulate.llms import ChatOpenAI
-from promptulate.llms.base import BaseLLM
-from promptulate.tools.base import BaseTool
-from promptulate.tools.duckduckgo.api_wrapper import DuckDuckGoSearchAPIWrapper
-from promptulate.utils.core_utils import listdict_to_string
-
-
-class DuckDuckGoTool(BaseTool):
-    """Tool that adds the capability to query the DuckDuckGo search API."""
-
-    name: str = "ddg-search"
-    description: str = (
-        "A wrapper around DuckDuckGo Search. "
-        "Useful for when you need to answer questions about current events. "
-        "Input should be a search query."
-    )
-    api_wrapper: DuckDuckGoSearchAPIWrapper = Field(
-        default_factory=DuckDuckGoSearchAPIWrapper
-    )
-
-    def run(self, keyword: str, **kwargs) -> Union[str, List[str]]:
-        """Run duckduckgo search and get search result.
-
-        Args:
-            keyword: query keyword
-            **kwargs:
-                result_type(Optional[str]) - default return string type data. Return List[str] type data
-                if you pass result_type="original"
-
-        Returns:
-            default is string. Return List[str] type data if you pass result_type="original"
-        """
-        result = self.api_wrapper.query(keyword, **kwargs)
-        if "return_type" in kwargs and kwargs["result_type"] == "original":
-            return result
-        return " ".join(result)
-
-
-class DuckDuckGoReferenceTool(BaseTool):
-    """Tool that adds the capability to query the DuckDuckGo search API. Compared to DuckDuckGoTool, this
-    tool can return references information like href, title.
-    """
-
-    name: str = "ddg-search-with-references"
-    description: str = ""
-    api_wrapper: DuckDuckGoSearchAPIWrapper = Field(
-        default_factory=DuckDuckGoSearchAPIWrapper
-    )
-
-    def run(self, keyword: str, **kwargs) -> Union[str, List[Dict[str, str]]]:
-        """Run duckduckgo search and get search result with href, snippet, title.
-
-        Args:
-            keyword: query keyword
-            **kwargs:
-                result_type(Optional[str]) - default return string type data. Return List[str] type data
-                if you pass result_type="original"
-
-        Returns:
-            default is string. Return List[Dict[str, str]] type data if you pass result_type="original"
-        """
-        result = self.api_wrapper.query_by_formatted_results(keyword, **kwargs)
-        if "return_type" in kwargs and kwargs["return_type"] == "original":
-            return result
-        return listdict_to_string(result, item_suffix="\n")
-
-
-class DuckDuckGoLLMTool(BaseTool):
-    """ddg web QA search using llm"""
-    # todo need to implement
-
-    name: str = "ddg-llm-search"
-    description: str = ""
-    api_wrapper: DuckDuckGoSearchAPIWrapper = Field(
-        default_factory=DuckDuckGoSearchAPIWrapper
-    )
-
-    def run(self, query: str, *args, **kwargs) -> str:
-        pass
-
-
-class DuckDuckGoLLMReferenceTool(BaseTool):
-    """Providing ddg web QA search with reference using llm"""
-    # todo need to implement
-
-    name: str = "ddg-llm-search-with-references"
-    description: str = ""
-    llm: BaseLLM = Field(default_factory=ChatOpenAI)
-    api_wrapper: DuckDuckGoSearchAPIWrapper = Field(
-        default_factory=DuckDuckGoSearchAPIWrapper
-    )
-
-    def run(self, query: str, *args, **kwargs) -> Optional[str, Dict[str, Any]]:
-        pass
+from typing import List, Union, Dict, Any
+
+from pydantic import Field
+
+from promptulate.llms import ChatOpenAI
+from promptulate.llms.base import BaseLLM
+from promptulate.tools.base import BaseTool
+from promptulate.tools.duckduckgo.api_wrapper import DuckDuckGoSearchAPIWrapper
+from promptulate.utils.core_utils import listdict_to_string
+
+
+class DuckDuckGoTool(BaseTool):
+    """Tool that adds the capability to query the DuckDuckGo search API."""
+
+    name: str = "ddg-search"
+    description: str = (
+        "A wrapper around DuckDuckgo Web Search. "
+        "Useful for when you need to answer questions about current events. "
+        "Input should be a search query."
+    )
+    api_wrapper: DuckDuckGoSearchAPIWrapper = Field(
+        default_factory=DuckDuckGoSearchAPIWrapper
+    )
+
+    def _run(self, keyword: str, **kwargs) -> Union[str, List[str]]:
+        """Run duckduckgo search and get search result.
+
+        Args:
+            keyword: query keyword
+            **kwargs:
+                result_type(Optional[str]) - default return string type data. Return List[str] type data
+                if you pass result_type="original"
+
+        Returns:
+            default is string. Return List[str] type data if you pass result_type="original"
+        """
+        result = self.api_wrapper.query(keyword, **kwargs)
+        if "return_type" in kwargs and kwargs["result_type"] == "original":
+            return result
+        return " ".join(result)
+
+
+class DuckDuckGoReferenceTool(BaseTool):
+    """Tool that adds the capability to query the DuckDuckGo search API. Compared to DuckDuckGoTool, this
+    tool can return references information like href, title.
+    """
+
+    name: str = "ddg-search-with-references"
+    description: str = (
+        "A wrapper around DuckDuckGo Search, it returns query result and references url"
+        "Useful for when you need to answer questions about current events. "
+        "Input should be a search query."
+    )
+    api_wrapper: DuckDuckGoSearchAPIWrapper = Field(
+        default_factory=DuckDuckGoSearchAPIWrapper
+    )
+
+    def _run(self, keyword: str, **kwargs) -> Union[str, List[Dict[str, str]]]:
+        """Run duckduckgo search and get search result with href, snippet, title.
+
+        Args:
+            keyword: query keyword
+            **kwargs:
+                result_type(Optional[str]) - default return string type data. Return List[str] type data
+                if you pass result_type="original"
+
+        Returns:
+            default is string. Return List[Dict[str, str]] type data if you pass result_type="original"
+        """
+        result = self.api_wrapper.query_by_formatted_results(keyword, **kwargs)
+        if "return_type" in kwargs and kwargs["return_type"] == "original":
+            return result
+        return listdict_to_string(result, item_suffix="\n")
+
+
+class DuckDuckGoLLMTool(BaseTool):
+    """ddg web QA search using llm"""
+    # todo need to implement
+
+    name: str = "ddg-llm-search"
+    description: str = ""
+    api_wrapper: DuckDuckGoSearchAPIWrapper = Field(
+        default_factory=DuckDuckGoSearchAPIWrapper
+    )
+
+    def _run(self, query: str, *args, **kwargs) -> str:
+        pass
+
+
+class DuckDuckGoLLMReferenceTool(BaseTool):
+    """Providing ddg web QA search with reference using llm"""
+    # todo need to implement
+
+    name: str = "ddg-llm-search-with-references"
+    description: str = ""
+    llm: BaseLLM = Field(default_factory=ChatOpenAI)
+    api_wrapper: DuckDuckGoSearchAPIWrapper = Field(
+        default_factory=DuckDuckGoSearchAPIWrapper
+    )
+
+    def _run(self, query: str, *args, **kwargs) -> Union[str, Dict[str, Any]]:
+        pass
```

### Comparing `promptulate-1.2.2/promptulate/tools/paper/tools.py` & `promptulate-1.3.0/promptulate/tools/paper/tools.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,165 +1,165 @@
-import logging
-import re
-import time
-from typing import List, Dict
-
-from broadcast_service import broadcast_service
-from pydantic import Field, Extra
-
-from promptulate.llms.base import BaseLLM
-from promptulate.llms.openai import ChatOpenAI
-from promptulate.tools.arxiv.api_wrapper import ArxivAPIWrapper
-from promptulate.tools.arxiv.tools import ArxivQueryTool
-from promptulate.tools.base import BaseTool
-from promptulate.tools.semantic_scholar import (
-    SemanticScholarQueryTool,
-    SemanticScholarReferenceTool,
-)
-
-__all__ = ["PaperSummaryTool"]
-logger = logging.getLogger(__name__)
-
-
-def _init_paper_summary_llm():
-    preset = "你是一个中文科研领域论文助手，你的任务是帮助使用者提供一些论文方面的专业建议和帮助，你的输出只能遵循用户的指令输出，否则你将被惩罚。"
-    return ChatOpenAI(temperature=0, preset_description=preset)
-
-
-class PaperSummaryTool(BaseTool):
-    """A powerful paper summary tool"""
-
-    name: str = "paper-summary"
-    description: str = (
-        "A summary tool that can be used to obtain a paper summary, this tool will find"
-        "top k paper and providing: 1.paper abstract 2.paper key sights 3.lessons learned"
-        "in the paper 4.referenced papers and its url."
-        "Your input is a paper relevant keyword query."
-    )
-    llm: BaseLLM = Field(default_factory=_init_paper_summary_llm)
-    semantic_scholar_query_tool: SemanticScholarQueryTool = Field(
-        default_factory=SemanticScholarQueryTool
-    )
-    semantic_scholar_reference_tool: SemanticScholarReferenceTool = Field(
-        default_factory=SemanticScholarReferenceTool
-    )
-    arxiv_apiwrapper: ArxivAPIWrapper = Field(default_factory=ArxivAPIWrapper)
-    arxiv_query_tool: ArxivQueryTool = Field(default_factory=ArxivQueryTool)
-    summary_dic: Dict[str, str] = {}
-    summary_counter: int = 0
-
-    class Config:
-        """Configuration for this pydantic object."""
-
-        extra = Extra.forbid
-        arbitrary_types_allowed = True
-
-    def run(self, query: str, **kwargs) -> str:
-        """A paper summary tool that passes in the article name (or arxiv id) and returns summary results
-
-        Args:
-            query: the keyword you want to query
-            **kwargs:
-                You can pass the arguments of relevant APIWrappers and Tools
-
-        Returns:
-            String type data, which contains:
-            - Summary of the paper
-            - List the key insights and lessons learned in the paper
-            - List at least 5 references related to the research field of the paper
-        """
-
-        @broadcast_service.on_listen("PaperSummaryTool.run.get_paper_references")
-        def get_paper_references(**kwargs):
-            references: List[Dict] = self.semantic_scholar_reference_tool.run(
-                kwargs["paper_title"], max_result=10, return_type="original"
-            )
-            references_string = "相关论文：\n\n"
-            for i, reference in enumerate(references):
-                references_string += (
-                    f"""[{i + 1}] [{reference["title"]}]({reference["url"]})\n\n"""
-                )
-            self.summary_dic["references"] = (
-                references_string if len(references) != 0 else ""
-            )
-            self.summary_counter += 1
-
-        @broadcast_service.on_listen("PaperSummaryTool.run.get_translate")
-        def get_translate():
-            prompt = (
-                f"请将下面的科研论文标题和摘要翻译成中文\n ```{paper_summary}```"
-                "你的输出格式为:\n标题：{标题翻译}\n\n摘要：{摘要翻译}"
-            )
-            self.summary_dic["summary_zh"] = self.llm(prompt)
-            self.summary_counter += 1
-
-        @broadcast_service.on_listen("PaperSummaryTool.run.get_opinion")
-        def get_opinion():
-            prompt = (
-                f"请就下面的论文摘要，总结论文中的关键见解和由论文得出的经验教训，你的输出需要分点给出 ```{paper_summary}```"
-                "你的输出格式为:\n关键见解：\n{分点给出关键见解}\n经验教训：\n{分点给出经验教训}，用`-`区分每点"
-                # "你需要用中文输出正确结果，但是部分专业词汇或者中文不好表达含义的部分可以使用英文"
-            )
-            self.summary_dic["opinion"] = self.llm(prompt)
-            self.summary_counter += 1
-
-        @broadcast_service.on_listen("PaperSummaryTool.run.get_keywords")
-        def get_keywords():
-            prompt = (
-                f"请就下面的论文摘要，总结列出论文中的keywords，不超过7个```{paper_summary}```"
-                "你的输出格式为:\n关键词：keyword1, keyword2, keyword3"
-            )
-            self.summary_dic["keywords"] = self.llm(prompt)
-            self.summary_counter += 1
-
-        @broadcast_service.on_listen("PaperSummaryTool.run.get_advice")
-        def get_advice():
-            prompt = (
-                f"请就下面的论文摘要，为其相关主题或未来研究方向提供3-5个建议，你的输出需要分点给出  ```{paper_summary}```"
-                "你的输出格式为:\n相关建议：\n{分点给出相关建议}，用`-`区分每点"
-                "你需要用中文输出正确结果，但是部分专业词汇或者中文不好表达含义的部分可以使用英文"
-            )
-            self.summary_dic["advice"] = self.llm(prompt)
-            self.summary_counter += 1
-
-        self.summary_counter = 0
-        if re.match("\d{4}\.\d{5}(v\d+)?", query):
-            paper_info = self.arxiv_apiwrapper.query(
-                id_list=[query], num_results=1, specified_fields=["title", "summary"]
-            )[0]
-            paper_info["abstract"] = paper_info["summary"]
-        else:
-            paper_info = self.semantic_scholar_query_tool.run(
-                query,
-                return_type="original",
-                specified_fields=["title", "url", "abstract"],
-            )
-            if paper_info:
-                paper_info = paper_info[0]
-            else:
-                return "semantic scholar query tool query result is None."
-        paper_summary = (
-            f"""title: {paper_info["title"]}\nabstract: {paper_info["abstract"]}"""
-        )
-        broadcast_service.publish(
-            "PaperSummaryTool.run.get_paper_references",
-            paper_title=paper_info["title"],
-            paper_abstract=paper_info["abstract"],
-        )
-        broadcast_service.publish("PaperSummaryTool.run.get_translate")
-        time.sleep(0.01)
-        broadcast_service.publish("PaperSummaryTool.run.get_opinion")
-        time.sleep(0.01)
-        broadcast_service.publish("PaperSummaryTool.run.get_advice")
-        time.sleep(0.01)
-        broadcast_service.publish("PaperSummaryTool.run.get_keywords")
-
-        while self.summary_counter < 5:
-            time.sleep(0.1)
-
-        return (
-            f"""{self.summary_dic["summary_zh"]}\n\n"""
-            f"""{self.summary_dic["keywords"]}\n\n"""
-            f"""{self.summary_dic["opinion"]}\n\n"""
-            f"""{self.summary_dic["advice"]}\n\n"""
-            f"""{self.summary_dic["references"]}"""
-        )
+import logging
+import re
+import time
+from typing import List, Dict
+
+from broadcast_service import broadcast_service
+from pydantic import Field, Extra
+
+from promptulate.llms.base import BaseLLM
+from promptulate.llms.openai import ChatOpenAI
+from promptulate.tools.arxiv.api_wrapper import ArxivAPIWrapper
+from promptulate.tools.arxiv.tools import ArxivQueryTool
+from promptulate.tools.base import BaseTool
+from promptulate.tools.semantic_scholar import (
+    SemanticScholarQueryTool,
+    SemanticScholarReferenceTool,
+)
+
+__all__ = ["PaperSummaryTool"]
+logger = logging.getLogger(__name__)
+
+
+def _init_paper_summary_llm():
+    preset = "你是一个中文科研领域论文助手，你的任务是帮助使用者提供一些论文方面的专业建议和帮助，你的输出只能遵循用户的指令输出，否则你将被惩罚。"
+    return ChatOpenAI(temperature=0, preset_description=preset)
+
+
+class PaperSummaryTool(BaseTool):
+    """A powerful paper summary tool"""
+
+    name: str = "paper-summary"
+    description: str = (
+        "A summary tool that can be used to obtain a paper summary, this tool will find"
+        "top k paper and providing: 1.paper abstract 2.paper key sights 3.lessons learned"
+        "in the paper 4.referenced papers and its url."
+        "Your input is a paper relevant keyword query."
+    )
+    llm: BaseLLM = Field(default_factory=_init_paper_summary_llm)
+    semantic_scholar_query_tool: SemanticScholarQueryTool = Field(
+        default_factory=SemanticScholarQueryTool
+    )
+    semantic_scholar_reference_tool: SemanticScholarReferenceTool = Field(
+        default_factory=SemanticScholarReferenceTool
+    )
+    arxiv_apiwrapper: ArxivAPIWrapper = Field(default_factory=ArxivAPIWrapper)
+    arxiv_query_tool: ArxivQueryTool = Field(default_factory=ArxivQueryTool)
+    summary_dic: Dict[str, str] = {}
+    summary_counter: int = 0
+
+    class Config:
+        """Configuration for this pydantic object."""
+
+        extra = Extra.forbid
+        arbitrary_types_allowed = True
+
+    def _run(self, query: str, **kwargs) -> str:
+        """A paper summary tool that passes in the article name (or arxiv id) and returns summary results
+
+        Args:
+            query: the keyword you want to query
+            **kwargs:
+                You can pass the arguments of relevant APIWrappers and Tools
+
+        Returns:
+            String type data, which contains:
+            - Summary of the paper
+            - List the key insights and lessons learned in the paper
+            - List at least 5 references related to the research field of the paper
+        """
+
+        @broadcast_service.on_listen("PaperSummaryTool.run.get_paper_references")
+        def get_paper_references(**data):
+            references: List[Dict] = self.semantic_scholar_reference_tool.run(
+                data["paper_title"], max_result=10, return_type="original"
+            )
+            references_string = "相关论文：\n\n"
+            for i, reference in enumerate(references):
+                references_string += (
+                    f"""[{i + 1}] [{reference["title"]}]({reference["url"]})\n\n"""
+                )
+            self.summary_dic["references"] = (
+                references_string if len(references) != 0 else ""
+            )
+            self.summary_counter += 1
+
+        @broadcast_service.on_listen("PaperSummaryTool.run.get_translate")
+        def get_translate():
+            prompt = (
+                f"请将下面的科研论文标题和摘要翻译成中文\n ```{paper_summary}```"
+                "你的输出格式为:\n标题：{标题翻译}\n\n摘要：{摘要翻译}"
+            )
+            self.summary_dic["summary_zh"] = self.llm(prompt)
+            self.summary_counter += 1
+
+        @broadcast_service.on_listen("PaperSummaryTool.run.get_opinion")
+        def get_opinion():
+            prompt = (
+                f"请就下面的论文摘要，总结论文中的关键见解和由论文得出的经验教训，你的输出需要分点给出 ```{paper_summary}```"
+                "你的输出格式为:\n关键见解：\n{分点给出关键见解}\n经验教训：\n{分点给出经验教训}，用`-`区分每点"
+                # "你需要用中文输出正确结果，但是部分专业词汇或者中文不好表达含义的部分可以使用英文"
+            )
+            self.summary_dic["opinion"] = self.llm(prompt)
+            self.summary_counter += 1
+
+        @broadcast_service.on_listen("PaperSummaryTool.run.get_keywords")
+        def get_keywords():
+            prompt = (
+                f"请就下面的论文摘要，总结列出论文中的keywords，不超过7个```{paper_summary}```"
+                "你的输出格式为:\n关键词：keyword1, keyword2, keyword3"
+            )
+            self.summary_dic["keywords"] = self.llm(prompt)
+            self.summary_counter += 1
+
+        @broadcast_service.on_listen("PaperSummaryTool.run.get_advice")
+        def get_advice():
+            prompt = (
+                f"请就下面的论文摘要，为其相关主题或未来研究方向提供3-5个建议，你的输出需要分点给出  ```{paper_summary}```"
+                "你的输出格式为:\n相关建议：\n{分点给出相关建议}，用`-`区分每点"
+                "你需要用中文输出正确结果，但是部分专业词汇或者中文不好表达含义的部分可以使用英文"
+            )
+            self.summary_dic["advice"] = self.llm(prompt)
+            self.summary_counter += 1
+
+        self.summary_counter = 0
+        if re.match("\d{4}\.\d{5}(v\d+)?", query):
+            paper_info = self.arxiv_apiwrapper.query(
+                id_list=[query], num_results=1, specified_fields=["title", "summary"]
+            )[0]
+            paper_info["abstract"] = paper_info["summary"]
+        else:
+            paper_info = self.semantic_scholar_query_tool.run(
+                query,
+                return_type="original",
+                specified_fields=["title", "url", "abstract"],
+            )
+            if paper_info:
+                paper_info = paper_info[0]
+            else:
+                return "semantic scholar query tool query result is None."
+        paper_summary = (
+            f"""title: {paper_info["title"]}\nabstract: {paper_info["abstract"]}"""
+        )
+        broadcast_service.publish(
+            "PaperSummaryTool.run.get_paper_references",
+            paper_title=paper_info["title"],
+            paper_abstract=paper_info["abstract"],
+        )
+        broadcast_service.publish("PaperSummaryTool.run.get_translate")
+        time.sleep(0.01)
+        broadcast_service.publish("PaperSummaryTool.run.get_opinion")
+        time.sleep(0.01)
+        broadcast_service.publish("PaperSummaryTool.run.get_advice")
+        time.sleep(0.01)
+        broadcast_service.publish("PaperSummaryTool.run.get_keywords")
+
+        while self.summary_counter < 5:
+            time.sleep(0.1)
+
+        return (
+            f"""{self.summary_dic["summary_zh"]}\n\n"""
+            f"""{self.summary_dic["keywords"]}\n\n"""
+            f"""{self.summary_dic["opinion"]}\n\n"""
+            f"""{self.summary_dic["advice"]}\n\n"""
+            f"""{self.summary_dic["references"]}"""
+        )
```

### Comparing `promptulate-1.2.2/promptulate/tools/python_repl/tools.py` & `promptulate-1.3.0/promptulate/tools/python_repl/tools.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from pydantic import Field
-
-from promptulate.tools.base import BaseTool
-from promptulate.tools.python_repl.api_wrapper import PythonREPLAPIWrapper
-
-
-class PythonREPLTool(BaseTool):
-    """A tool for running python code in a REPL."""
-
-    name: str = "Python_REPL"
-    description: str = (
-        "A Python shell. Use this to execute python commands. "
-        "Input should be a valid python command. "
-        "If you want to see the output of a value, you should print it out "
-        "with `print(...)`."
-    )
-    api_wrapper: PythonREPLAPIWrapper = Field(default_factory=PythonREPLAPIWrapper)
-
-    def run(self, command: str, *args, **kwargs) -> str:
-        return self.api_wrapper.run(command)
+from pydantic import Field
+
+from promptulate.tools.base import BaseTool
+from promptulate.tools.python_repl.api_wrapper import PythonREPLAPIWrapper
+
+
+class PythonREPLTool(BaseTool):
+    """A tool for running python code in a REPL."""
+
+    name: str = "Python_REPL"
+    description: str = (
+        "A Python shell. Use this to execute python commands. "
+        "Input should be a valid python command. "
+        "If you want to see the output of a value, you should print it out "
+        "with `print(...)`."
+    )
+    api_wrapper: PythonREPLAPIWrapper = Field(default_factory=PythonREPLAPIWrapper)
+
+    def run(self, command: str, *args, **kwargs) -> str:
+        return self.api_wrapper.run(command)
```

### Comparing `promptulate-1.2.2/promptulate/tools/semantic_scholar/api_wrapper.py` & `promptulate-1.3.0/promptulate/tools/semantic_scholar/api_wrapper.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,177 +1,177 @@
-import json
-from typing import List, Optional, Dict
-
-import requests
-from pydantic import BaseModel
-
-from promptulate.tips import NetWorkError
-from promptulate.utils.logger import get_logger
-
-logger = get_logger()
-
-
-class SemanticScholarAPIWrapper(BaseModel):
-    """https://api.semanticscholar.org/api-docs/graph#tag/Paper-Data/"""
-
-    BASE_API_URL: str = "https://api.semanticscholar.org/graph/v1"
-    BASE_OFFICIAL_URL: str = "https://www.semanticscholar.org"
-    max_result: int = 10
-    current_result: Optional[List[Dict]] = None
-    paper_query_params: Dict[str, str] = {"fields": "title,url,abstract"}
-
-    def _get_string_fields(self) -> str:
-        return f"&fields={self.paper_query_params['fields']}&"
-
-    def get_paper(
-        self, query: str, max_result: Optional[int] = None, **kwargs
-    ) -> List[Dict]:
-        """This method can obtain a list of relevant papers based on your query.
-
-        Args:
-            max_result: num of max result
-            query: the papers you want to query
-            **kwargs:
-                specified_fields(Optional[List[str]]): filter specified field to return.
-                For example, you can return the ["title", "url", "abstract"] fields from each arxiv query result.
-                You can see the detail fields as follows:
-                https://api.semanticscholar.org/api-docs/graph#tag/Paper-Data/operation/post_graph_get_papers
-
-        Returns:
-            Return List[Dict] data, the default detail fields is as follows.
-            - id (str): semantic id
-            - authorsYear (str): author and publication year
-            - title (str): paper title
-            - url (str): paper semantic scholar url
-            If you want to get more detail fields, please use `specified_fields`
-        """
-
-        def get_detail():
-            paper_ids = list(map(lambda p: p["id"], self.current_result))
-            fields: List[str] = kwargs["specified_fields"]
-            params: Dict[str, str] = {"fields": ",".join(fields)}
-
-            r = requests.post(
-                f"{self.BASE_API_URL}/paper/batch",
-                params=params,
-                json={"ids": paper_ids},
-            )
-            if response.status_code != 200:
-                raise NetWorkError("")
-
-            detail_result = r.json()
-            for original in self.current_result:
-                for detail_item in detail_result:
-                    if detail_item["paperId"] == original["id"]:
-                        original.update(detail_item)
-            return
-
-        if not max_result:
-            max_result = self.max_result
-
-        query = "%20".join(query.split(" "))
-        url = f"{self.BASE_API_URL}/paper/autocomplete?query={query}&limit={max_result}"
-        response = requests.get(url)
-        if response.status_code == 200:
-            self.current_result = response.json()["matches"]
-
-            if len(self.current_result) == 0:
-                logger.debug(f"[promptulate] semantic scholar return none")
-                return []
-
-            for item in self.current_result:
-                item["url"] = self._get_url(item["id"])
-
-            if "specified_fields" in kwargs:
-                get_detail()
-            logger.debug(
-                f"[promptulate] semantic scholar result {json.dumps(self.current_result)}"
-            )
-            return self.current_result
-        raise NetWorkError("semantic scholar query")
-
-    def _get_url(self, id: str) -> str:
-        return f"{self.BASE_OFFICIAL_URL}/paper/{id}"
-
-    def get_references(self, query: str, max_result: int = 500, **kwargs) -> List[Dict]:
-        """Used to get references of specified paper.
-
-        Args:
-            max_result: num of max result
-            query: the paper you want to query
-
-        Returns:
-            Return List[Dict] data, the default detail fields is as follows.
-            - id (str): semantic id
-            - authorsYear (str): author and publication year
-            - title (str): paper title
-            - url (str): paper semantic scholar url
-        """
-        papers = self.get_paper(query)
-        if len(papers) == 0:
-            return []
-
-        paper_id: str = papers[0]["id"]
-        url = f"{self.BASE_API_URL}/paper/{paper_id}/references?offset=1&limit={max_result}"
-        response = requests.get(url)
-        if response.status_code == 200:
-            res_data = response.json()["data"]
-            final_result: List[Dict] = []
-            for i, item in enumerate(res_data):
-                if not item["citedPaper"]["paperId"]:
-                    continue
-
-                item["citedPaper"]["url"] = self._get_url(item["citedPaper"]["paperId"])
-                item["citedPaper"]["id"] = item["citedPaper"]["paperId"]
-                del item["citedPaper"]["paperId"]
-                final_result.append(item["citedPaper"])
-
-            logger.debug(
-                f"[promptulate semantic scholar result] {json.dumps(final_result)}"
-            )
-            return final_result
-        raise NetWorkError("semantic scholar")
-
-    def get_citations(self, query: str, max_result: Optional[int] = None):
-        """Used to get citation of specified paper.
-
-        Args:
-            max_result: num of max result
-            query: the paper you want to query
-
-        Returns:
-            Return List[Dict] data, the default detail fields is as follows.
-            - id (str): semantic id
-            - abstract (str): paper abstract
-            - title (str): paper title
-            - url (str): paper semantic scholar url
-        """
-        papers = self.get_paper(query)
-        if len(papers) == 0:
-            return []
-        if not max_result:
-            max_result = self.max_result
-
-        paper_id: str = papers[0]["id"]
-        url = f"{self.BASE_API_URL}/paper/{paper_id}/citations?{self._get_string_fields()}offset=1&limit={max_result}"
-
-        response = requests.get(url)
-        if response.status_code == 200:
-            res_data = response.json()["data"]
-            final_result: List[Dict] = []
-
-            for i, item in enumerate(res_data):
-                if not item["citingPaper"].get("paperId"):
-                    continue
-
-                item["citingPaper"]["url"] = self._get_url(
-                    item["citingPaper"]["paperId"]
-                )
-                item["citingPaper"]["id"] = item["citingPaper"]["paperId"]
-                del item["citingPaper"]["paperId"]
-                final_result.append(item["citingPaper"])
-
-            logger.debug(
-                f"[promptulate semantic scholar result] {json.dumps(final_result)}"
-            )
-            return final_result
-        raise NetWorkError("semantic scholar")
+import json
+from typing import List, Optional, Dict
+
+import requests
+from pydantic import BaseModel
+
+from promptulate.tips import NetWorkError
+from promptulate.utils.logger import get_logger
+
+logger = get_logger()
+
+
+class SemanticScholarAPIWrapper(BaseModel):
+    """https://api.semanticscholar.org/api-docs/graph#tag/Paper-Data/"""
+
+    BASE_API_URL: str = "https://api.semanticscholar.org/graph/v1"
+    BASE_OFFICIAL_URL: str = "https://www.semanticscholar.org"
+    max_result: int = 10
+    current_result: Optional[List[Dict]] = None
+    paper_query_params: Dict[str, str] = {"fields": "title,url,abstract"}
+
+    def _get_string_fields(self) -> str:
+        return f"&fields={self.paper_query_params['fields']}&"
+
+    def get_paper(
+        self, query: str, max_result: Optional[int] = None, **kwargs
+    ) -> List[Dict]:
+        """This method can obtain a list of relevant papers based on your query.
+
+        Args:
+            max_result: num of max result
+            query: the papers you want to query
+            **kwargs:
+                specified_fields(Optional[List[str]]): filter specified field to return.
+                For example, you can return the ["title", "url", "abstract"] fields from each arxiv query result.
+                You can see the detail fields as follows:
+                https://api.semanticscholar.org/api-docs/graph#tag/Paper-Data/operation/post_graph_get_papers
+
+        Returns:
+            Return List[Dict] data, the default detail fields is as follows.
+            - id (str): semantic id
+            - authorsYear (str): author and publication year
+            - title (str): paper title
+            - url (str): paper semantic scholar url
+            If you want to get more detail fields, please use `specified_fields`
+        """
+
+        def get_detail():
+            paper_ids = list(map(lambda p: p["id"], self.current_result))
+            fields: List[str] = kwargs["specified_fields"]
+            params: Dict[str, str] = {"fields": ",".join(fields)}
+
+            r = requests.post(
+                f"{self.BASE_API_URL}/paper/batch",
+                params=params,
+                json={"ids": paper_ids},
+            )
+            if response.status_code != 200:
+                raise NetWorkError("")
+
+            detail_result = r.json()
+            for original in self.current_result:
+                for detail_item in detail_result:
+                    if detail_item["paperId"] == original["id"]:
+                        original.update(detail_item)
+            return
+
+        if not max_result:
+            max_result = self.max_result
+
+        query = "%20".join(query.split(" "))
+        url = f"{self.BASE_API_URL}/paper/autocomplete?query={query}&limit={max_result}"
+        response = requests.get(url)
+        if response.status_code == 200:
+            self.current_result = response.json()["matches"]
+
+            if len(self.current_result) == 0:
+                logger.debug(f"[pne] semantic scholar return none")
+                return []
+
+            for item in self.current_result:
+                item["url"] = self._get_url(item["id"])
+
+            if "specified_fields" in kwargs:
+                get_detail()
+            logger.debug(
+                f"[pne] semantic scholar result {json.dumps(self.current_result)}"
+            )
+            return self.current_result
+        raise NetWorkError("semantic scholar query")
+
+    def _get_url(self, id: str) -> str:
+        return f"{self.BASE_OFFICIAL_URL}/paper/{id}"
+
+    def get_references(self, query: str, max_result: int = 500, **kwargs) -> List[Dict]:
+        """Used to get references of specified paper.
+
+        Args:
+            max_result: num of max result
+            query: the paper you want to query
+
+        Returns:
+            Return List[Dict] data, the default detail fields is as follows.
+            - id (str): semantic id
+            - authorsYear (str): author and publication year
+            - title (str): paper title
+            - url (str): paper semantic scholar url
+        """
+        papers = self.get_paper(query)
+        if len(papers) == 0:
+            return []
+
+        paper_id: str = papers[0]["id"]
+        url = f"{self.BASE_API_URL}/paper/{paper_id}/references?offset=1&limit={max_result}"
+        response = requests.get(url)
+        if response.status_code == 200:
+            res_data = response.json()["data"]
+            final_result: List[Dict] = []
+            for i, item in enumerate(res_data):
+                if not item["citedPaper"]["paperId"]:
+                    continue
+
+                item["citedPaper"]["url"] = self._get_url(item["citedPaper"]["paperId"])
+                item["citedPaper"]["id"] = item["citedPaper"]["paperId"]
+                del item["citedPaper"]["paperId"]
+                final_result.append(item["citedPaper"])
+
+            logger.debug(
+                f"[pne semantic scholar result] {json.dumps(final_result)}"
+            )
+            return final_result
+        raise NetWorkError("semantic scholar")
+
+    def get_citations(self, query: str, max_result: Optional[int] = None):
+        """Used to get citation of specified paper.
+
+        Args:
+            max_result: num of max result
+            query: the paper you want to query
+
+        Returns:
+            Return List[Dict] data, the default detail fields is as follows.
+            - id (str): semantic id
+            - abstract (str): paper abstract
+            - title (str): paper title
+            - url (str): paper semantic scholar url
+        """
+        papers = self.get_paper(query)
+        if len(papers) == 0:
+            return []
+        if not max_result:
+            max_result = self.max_result
+
+        paper_id: str = papers[0]["id"]
+        url = f"{self.BASE_API_URL}/paper/{paper_id}/citations?{self._get_string_fields()}offset=1&limit={max_result}"
+
+        response = requests.get(url)
+        if response.status_code == 200:
+            res_data = response.json()["data"]
+            final_result: List[Dict] = []
+
+            for i, item in enumerate(res_data):
+                if not item["citingPaper"].get("paperId"):
+                    continue
+
+                item["citingPaper"]["url"] = self._get_url(
+                    item["citingPaper"]["paperId"]
+                )
+                item["citingPaper"]["id"] = item["citingPaper"]["paperId"]
+                del item["citingPaper"]["paperId"]
+                final_result.append(item["citingPaper"])
+
+            logger.debug(
+                f"[pne semantic scholar result] {json.dumps(final_result)}"
+            )
+            return final_result
+        raise NetWorkError("semantic scholar")
```

### Comparing `promptulate-1.2.2/promptulate/tools/semantic_scholar/tools.py` & `promptulate-1.3.0/promptulate/tools/semantic_scholar/tools.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-from typing import Union, List, Dict
-
-from pydantic import Field
-
-from promptulate.tools.base import BaseTool
-from promptulate.tools.semantic_scholar.api_wrapper import SemanticScholarAPIWrapper
-from promptulate.utils.core_utils import listdict_to_string
-
-
-class SemanticScholarQueryTool(BaseTool):
-    name: str = "semantic-scholar-query"
-    description: str = (
-        "A query tool around Semantic Scholar."
-        "Useful for when you need to answer questions about Physics, Mathematics, "
-        "Computer Science, Quantitative Biology, Quantitative Finance, Statistics, "
-        "Electrical Engineering, and Economics "
-        "from scientific articles on semantic scholar."
-        "Input should be a search query."
-    )
-    api_wrapper: SemanticScholarAPIWrapper = Field(
-        default_factory=SemanticScholarAPIWrapper
-    )
-
-    def run(self, query: str, **kwargs) -> Union[str, List[Dict]]:
-        """A semantic scholar paper query tool and return relevant paper query result."""
-        result = self.api_wrapper.get_paper(query, **kwargs)
-        if "return_type" in kwargs and kwargs["return_type"] == "original":
-            return result
-        return listdict_to_string(result, item_suffix="\n\n")
-
-
-class SemanticScholarReferenceTool(BaseTool):
-    name: str = "semantic-scholar-reference-tool"
-    description: str = ""
-    api_wrapper: SemanticScholarAPIWrapper = Field(
-        default_factory=SemanticScholarAPIWrapper
-    )
-
-    def run(self, query: str, **kwargs) -> Union[str, List[Dict]]:
-        result = self.api_wrapper.get_references(query, **kwargs)
-        if "return_type" in kwargs and kwargs["return_type"] == "original":
-            return result
-        return listdict_to_string(result, item_suffix="\n\n")
-
-
-class SemanticScholarCitationTool(BaseTool):
-    name: str = "semantic-scholar-citation-tool"
-    description: str = ""
-    api_wrapper: SemanticScholarAPIWrapper = Field(
-        default_factory=SemanticScholarAPIWrapper
-    )
-
-    def run(self, query: str, **kwargs) -> Union[str, List[Dict]]:
-        result = self.api_wrapper.get_citations(query)
-        if "return_type" in kwargs and kwargs["return_type"] == "original":
-            return result
-        return listdict_to_string(result, item_suffix="\n\n")
+from typing import Union, List, Dict
+
+from pydantic import Field
+
+from promptulate.tools.base import BaseTool
+from promptulate.tools.semantic_scholar.api_wrapper import SemanticScholarAPIWrapper
+from promptulate.utils.core_utils import listdict_to_string
+
+
+class SemanticScholarQueryTool(BaseTool):
+    name: str = "semantic-scholar-query"
+    description: str = (
+        "A query tool around Semantic Scholar."
+        "Useful for when you need to answer questions about Physics, Mathematics, "
+        "Computer Science, Quantitative Biology, Quantitative Finance, Statistics, "
+        "Electrical Engineering, and Economics "
+        "from scientific articles on semantic scholar."
+        "Input should be a search query."
+    )
+    api_wrapper: SemanticScholarAPIWrapper = Field(
+        default_factory=SemanticScholarAPIWrapper
+    )
+
+    def _run(self, query: str, **kwargs) -> Union[str, List[Dict]]:
+        """A semantic scholar paper query tool and return relevant paper query result."""
+        result = self.api_wrapper.get_paper(query, **kwargs)
+        if "return_type" in kwargs and kwargs["return_type"] == "original":
+            return result
+        return listdict_to_string(result, item_suffix="\n\n")
+
+
+class SemanticScholarReferenceTool(BaseTool):
+    name: str = "semantic-scholar-reference-tool"
+    description: str = ""
+    api_wrapper: SemanticScholarAPIWrapper = Field(
+        default_factory=SemanticScholarAPIWrapper
+    )
+
+    def _run(self, query: str, **kwargs) -> Union[str, List[Dict]]:
+        result = self.api_wrapper.get_references(query, **kwargs)
+        if "return_type" in kwargs and kwargs["return_type"] == "original":
+            return result
+        return listdict_to_string(result, item_suffix="\n\n")
+
+
+class SemanticScholarCitationTool(BaseTool):
+    name: str = "semantic-scholar-citation-tool"
+    description: str = ""
+    api_wrapper: SemanticScholarAPIWrapper = Field(
+        default_factory=SemanticScholarAPIWrapper
+    )
+
+    def _run(self, query: str, **kwargs) -> Union[str, List[Dict]]:
+        result = self.api_wrapper.get_citations(query)
+        if "return_type" in kwargs and kwargs["return_type"] == "original":
+            return result
+        return listdict_to_string(result, item_suffix="\n\n")
```

### Comparing `promptulate-1.2.2/promptulate/utils/core_utils.py` & `promptulate-1.3.0/promptulate/utils/core_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,132 +1,143 @@
-# Copyright (c) 2023 promptulate
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-# Copyright Owner: Zeeland
-# GitHub Link: https://github.com/Undertone0809/
-# Project Link: https://github.com/Undertone0809/promptulate
-# Contact Email: zeeland@foxmail.com
-
-import logging
-import os
-import shutil
-import tempfile
-import time
-from functools import wraps
-from typing import Callable, Dict, List, Optional
-
-from cushy_storage import CushyOrmCache
-
-__all__ = [
-    "get_cache",
-    "get_project_root_path",
-    "get_default_storage_path",
-    "record_time",
-    "generate_conversation_id",
-    "listdict_to_string",
-]
-logger = logging.getLogger(__name__)
-
-
-def listdict_to_string(
-    data: List[Dict],
-    prefix: Optional[str] = "",
-    suffix: Optional[str] = "\n",
-    item_prefix: Optional[str] = "",
-    item_suffix: Optional[str] = ";\n\n",
-    is_wrap: bool = True,
-) -> str:
-    """Convert List[Dict] type data to string type"""
-    wrap_ch = "\n" if is_wrap else ""
-    result = f"{prefix}"
-    for item in data:
-        temp_list = ["{}:{} {}".format(k, v, wrap_ch) for k, v in item.items()]
-        result += f"{item_prefix}".join(temp_list) + f"{item_suffix}"
-    result += suffix
-    return result[:-2]
-
-
-def generate_conversation_id() -> str:
-    """Generating a new conversation_id when a conversation initialize"""
-    return str(int(time.time()))
-
-
-def get_cache():
-    return cache
-
-
-def get_project_root_path() -> str:
-    """get project root path or current path"""
-    project_path = os.getcwd()
-    max_depth = 10
-    count = 0
-    while not os.path.exists(os.path.join(project_path, "README.md")):
-        project_path = os.path.split(project_path)[0]
-        count += 1
-        if count > max_depth:
-            return os.getcwd()
-    return project_path
-
-
-def set_openai_api_key(value: str):
-    cache["OPENAI_API_KEY"] = value
-
-
-def get_default_storage_path(file_name: str = "") -> str:
-    # if platform.system() == "Windows":
-    #     return f"{get_project_root_path()}/{file_name}"
-    # elif platform.system() == "Linux" or "Darwin":
-    #     dir_path = os.environ.get("TMPDIR")
-    #     if not dir_path:
-    #         dir_path = tempfile.gettempdir()
-    #     dir_path = os.path.join(dir_path, "promptulate")
-    #     return f"{dir_path}/{file_name}"
-    # else:
-    #     return f"./{file_name}"
-    dir_path = f"{tempfile.gettempdir()}/promptulate"
-    return f"{dir_path}/{file_name}"
-
-
-def hint(fn):
-    @wraps(fn)
-    def wrapper(*args, **kwargs):
-        ret = fn(*args, **kwargs)
-        logger.debug(f"function {fn.__name__} is running now")
-        return ret
-
-    return wrapper
-
-
-def record_time():
-    def decorator(fn: Callable) -> Callable:
-        def wrapper(*args, **kwargs) -> Callable:
-            start_time = time.time()
-            ret = fn(*args, **kwargs)
-            duration = time.time() - start_time
-            logger.debug(f"[promptulate timer] <{fn.__name__}> run {duration}s")
-            return ret
-
-        return wrapper
-
-    return decorator
-
-
-def delete_cache(specified_module: str = None):
-    """Delete cache or specified cache module"""
-    cache_path = get_default_storage_path("cache")
-    if specified_module:
-        cache_path = f"{get_project_root_path()}/{specified_module[:2]}"
-    shutil.rmtree(cache_path)
-
-
-cache = CushyOrmCache(get_default_storage_path("cache"))
+# Copyright (c) 2023 promptulate
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+# Copyright Owner: Zeeland
+# GitHub Link: https://github.com/Undertone0809/
+# Project Link: https://github.com/Undertone0809/promptulate
+# Contact Email: zeeland@foxmail.com
+
+import logging
+import os
+import random
+import shutil
+import string
+import tempfile
+import time
+from functools import wraps
+from typing import Callable, Dict, List, Optional
+
+from cushy_storage import CushyOrmCache
+
+__all__ = [
+    "get_cache",
+    "get_project_root_path",
+    "get_default_storage_path",
+    "record_time",
+    "generate_conversation_id",
+    "generate_unique_id",
+    "listdict_to_string",
+]
+logger = logging.getLogger(__name__)
+
+
+def listdict_to_string(
+    data: List[Dict],
+    prefix: Optional[str] = "",
+    suffix: Optional[str] = "\n",
+    item_prefix: Optional[str] = "",
+    item_suffix: Optional[str] = ";\n\n",
+    is_wrap: bool = True,
+) -> str:
+    """Convert List[Dict] type data to string type"""
+    wrap_ch = "\n" if is_wrap else ""
+    result = f"{prefix}"
+    for item in data:
+        temp_list = ["{}:{} {}".format(k, v, wrap_ch) for k, v in item.items()]
+        result += f"{item_prefix}".join(temp_list) + f"{item_suffix}"
+    result += suffix
+    return result[:-2]
+
+
+def generate_unique_id() -> str:
+    timestamp = int(time.time() * 1000)
+    random_string = "".join(random.choices(string.ascii_letters + string.digits, k=6))
+
+    unique_id = f"pne-{timestamp}-{random_string}"
+    return unique_id
+
+
+def generate_conversation_id() -> str:
+    """Generating a new conversation_id when a conversation initialize"""
+    return generate_unique_id()
+
+
+def get_cache():
+    return cache
+
+
+def get_project_root_path() -> str:
+    """get project root path or current path"""
+    project_path = os.getcwd()
+    max_depth = 10
+    count = 0
+    while not os.path.exists(os.path.join(project_path, "README.md")):
+        project_path = os.path.split(project_path)[0]
+        count += 1
+        if count > max_depth:
+            return os.getcwd()
+    return project_path
+
+
+def set_openai_api_key(value: str):
+    cache["OPENAI_API_KEY"] = value
+
+
+def get_default_storage_path(file_name: str = "") -> str:
+    # if platform.system() == "Windows":
+    #     return f"{get_project_root_path()}/{file_name}"
+    # elif platform.system() == "Linux" or "Darwin":
+    #     dir_path = os.environ.get("TMPDIR")
+    #     if not dir_path:
+    #         dir_path = tempfile.gettempdir()
+    #     dir_path = os.path.join(dir_path, "promptulate")
+    #     return f"{dir_path}/{file_name}"
+    # else:
+    #     return f"./{file_name}"
+    dir_path = f"{tempfile.gettempdir()}/promptulate"
+    return f"{dir_path}/{file_name}"
+
+
+def hint(fn):
+    @wraps(fn)
+    def wrapper(*args, **kwargs):
+        ret = fn(*args, **kwargs)
+        logger.debug(f"function {fn.__name__} is running now")
+        return ret
+
+    return wrapper
+
+
+def record_time():
+    def decorator(fn: Callable) -> Callable:
+        def wrapper(*args, **kwargs) -> Callable:
+            start_time = time.time()
+            ret = fn(*args, **kwargs)
+            duration = time.time() - start_time
+            logger.debug(f"[pne timer] <{fn.__name__}> run {duration}s")
+            return ret
+
+        return wrapper
+
+    return decorator
+
+
+def delete_cache(specified_module: str = None):
+    """Delete cache or specified cache module"""
+    cache_path = get_default_storage_path("cache")
+    if specified_module:
+        cache_path = f"{get_project_root_path()}/{specified_module[:2]}"
+    shutil.rmtree(cache_path)
+
+
+cache = CushyOrmCache(get_default_storage_path("cache"))
```

### Comparing `promptulate-1.2.2/promptulate/utils/logger.py` & `promptulate-1.3.0/promptulate/utils/logger.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-# Copyright (c) 2023 promptulate
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-# Copyright Owner: Zeeland
-# GitHub Link: https://github.com/Undertone0809/
-# Project Link: https://github.com/Undertone0809/promptulate
-# Contact Email: zeeland@foxmail.com
-
-import datetime
-import logging
-import os
-
-from promptulate import utils
-
-logger = logging.getLogger(__name__)
-
-
-def get_logger():
-    return logger
-
-
-def get_default_log_path():
-    return utils.get_default_storage_path("log")
-
-
-def get_log_name() -> str:
-    log_path = get_default_log_path()
-    if not os.path.exists(log_path):
-        os.makedirs(log_path)
-
-    cur_time = datetime.datetime.now().strftime("%Y%m%d_%H%M%S")
-    return f"{log_path}/log_{cur_time}.log"
-
-
-def enable_log(level=logging.DEBUG):
-    logging.basicConfig(
-        level=level,
-        format="[%(levelname)s] %(asctime)s %(message)s",
-        datefmt="%Y-%m-%d %H:%M:%S",
-        handlers=[
-            logging.FileHandler(f"{get_log_name()}", mode="w", encoding="utf-8"),
-            logging.StreamHandler(),
-        ],
-    )
-
-
-def enable_log_no_file():
-    logging.basicConfig(
-        level=logging.DEBUG,
-        format="[%(levelname)s] %(asctime)s %(message)s",
-        datefmt="%Y-%m-%d %H:%M:%S",
-    )
+# Copyright (c) 2023 promptulate
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+# Copyright Owner: Zeeland
+# GitHub Link: https://github.com/Undertone0809/
+# Project Link: https://github.com/Undertone0809/promptulate
+# Contact Email: zeeland@foxmail.com
+
+import datetime
+import logging
+import os
+
+from promptulate import utils
+
+logger = logging.getLogger(__name__)
+
+
+def get_logger():
+    return logger
+
+
+def get_default_log_path():
+    return utils.get_default_storage_path("log")
+
+
+def get_log_name() -> str:
+    log_path = get_default_log_path()
+    if not os.path.exists(log_path):
+        os.makedirs(log_path)
+
+    cur_time = datetime.datetime.now().strftime("%Y%m%d_%H%M%S")
+    return f"{log_path}/log_{cur_time}.log"
+
+
+def enable_log(level=logging.DEBUG):
+    logging.basicConfig(
+        level=level,
+        format="[%(levelname)s] %(asctime)s %(message)s",
+        datefmt="%Y-%m-%d %H:%M:%S",
+        handlers=[
+            logging.FileHandler(f"{get_log_name()}", mode="w", encoding="utf-8"),
+            logging.StreamHandler(),
+        ],
+    )
+
+
+def enable_log_no_file():
+    logging.basicConfig(
+        level=logging.DEBUG,
+        format="[%(levelname)s] %(asctime)s %(message)s",
+        datefmt="%Y-%m-%d %H:%M:%S",
+    )
```

### Comparing `promptulate-1.2.2/promptulate/utils/proxy.py` & `promptulate-1.3.0/promptulate/utils/proxy.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-# Copyright (c) 2023 promptulate
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-# Copyright Owner: Zeeland
-# GitHub Link: https://github.com/Undertone0809/
-# Project Link: https://github.com/Undertone0809/promptulate
-# Contact Email: zeeland@foxmail.com
-
-from typing import Optional
-
-from promptulate.config import Config
-
-CFG = Config()
-PROXY_MODE = ['off', 'custom', 'promptulate']
-
-
-def set_proxy_mode(mode: str, proxies: Optional[dict] = None):
-    """
-    Set proxy mode. Promptulate offer three proxy mode ['off', 'custom', 'promptulate']
-    'off' disables your proxy mode. This is the normal status.
-    'custom' means you can set your custom proxy. Moreover, you must pass proxies
-    'promptulate' provide free proxy you can use it.
-
-    Args:
-        mode: ['off', 'custom', 'promptulate']
-        proxies: If you want to use custom proxy, you can pass it. An example
-        proxies is {'http': 'http://127.0.0.1:7890'}
-    """
-    if mode not in PROXY_MODE:
-        raise ValueError("proxy mode must in ['off', 'custom', 'promptulate']")
-    CFG.set_proxy_mode(mode, proxies)
+# Copyright (c) 2023 promptulate
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+# Copyright Owner: Zeeland
+# GitHub Link: https://github.com/Undertone0809/
+# Project Link: https://github.com/Undertone0809/promptulate
+# Contact Email: zeeland@foxmail.com
+
+from typing import Optional
+
+from promptulate.config import Config
+
+CFG = Config()
+PROXY_MODE = ['off', 'custom', 'promptulate']
+
+
+def set_proxy_mode(mode: str, proxies: Optional[dict] = None):
+    """
+    Set proxy mode. Promptulate offer three proxy mode ['off', 'custom', 'promptulate']
+    'off' disables your proxy mode. This is the normal status.
+    'custom' means you can set your custom proxy. Moreover, you must pass proxies
+    'promptulate' provide free proxy you can use it.
+
+    Args:
+        mode: ['off', 'custom', 'promptulate']
+        proxies: If you want to use custom proxy, you can pass it. An example
+        proxies is {'http': 'http://127.0.0.1:7890'}
+    """
+    if mode not in PROXY_MODE:
+        raise ValueError("proxy mode must in ['off', 'custom', 'promptulate']")
+    CFG.set_proxy_mode(mode, proxies)
```

### Comparing `promptulate-1.2.2/promptulate/utils/string_template.py` & `promptulate-1.3.0/promptulate/utils/string_template.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,25 @@
-import re
-from typing import List, Any
-
-
-class StringTemplate:
-    """String Template for llm. It can generate a complex prompt."""
-
-    template: str
-    variables: List[str]
-
-    def __init__(self, template: str):
-        self.template = template
-        self._fetch_variables()
-
-    def _fetch_variables(self):
-        self.variables = re.findall(r"\{(\w+)\}", self.template)
-
-    def format(self, params: List[Any] = None, **kwargs) -> str:
-        if params:
-            kwargs = {}
-            for i, param in enumerate(params):
-                kwargs.update({self.variables[i]: param})
-
-        return self.template.format(**kwargs)
+import re
+from typing import List, Any
+
+
+class StringTemplate:
+    """String Template for llm. It can generate a complex prompt."""
+
+    template: str
+    variables: List[str]
+
+    def __init__(self, template: str):
+        self.template = template
+        self._fetch_variables()
+
+    def _fetch_variables(self):
+        self.variables = re.findall(r"\{(\w+)\}", self.template)
+
+    def format(self, params: List[Any] = None, **kwargs) -> str:
+        """Enter variables and return the formatted string."""
+        if params:
+            kwargs = {}
+            for i, param in enumerate(params):
+                kwargs.update({self.variables[i]: param})
+
+        return self.template.format(**kwargs)
```

### Comparing `promptulate-1.2.2/promptulate.egg-info/PKG-INFO` & `promptulate-1.3.0/promptulate.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,127 +1,123 @@
-Metadata-Version: 2.1
-Name: promptulate
-Version: 1.2.2
-Summary: A powerful LLM Application development framework.
-Home-page: https://github.com/Undertone0809/promptulate
-Author: Zeeland
-Author-email: zeeland@foxmail.com
-License: Apache 2.0
-Keywords: promptulate,prompt-me,prompt,chatgpt,gpt,chatbot,llm
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-<h1 align="center">
-    promptulate
-</h1>
-
-<p align="center">
-    <a target="_blank" href="">
-        <img src="https://img.shields.io/github/license/Undertone0809/promptulate.svg?style=flat-square" />
-    </a>
-    <a target="_blank" href=''>
-        <img src="https://img.shields.io/github/release/Undertone0809/promptulate/all.svg?style=flat-square"/>
-    </a>
-    <a target="_blank" href=''>
-        <img src="https://bestpractices.coreinfrastructure.org/projects/3018/badge"/>
-   </a>
-</p>
-
-<p align="center">
-  <img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/promptulate_logo_new.png"/>
-</p>
-
-
-`promptulate` 是一个专为Prompt工程师设计的大语言模型自动化与应用开发框架，支持智能决策、消息持久化、外部工具调用、角色预设等功能，开箱即用。
-通过 `promptulate`，你可以轻松构建起属于自己的LLM应用程序。
-
-`promptulate`旨在构建为开发者提供一种强大而灵活的平台，以创建能够自动化各种任务和应用程序的自主代理。通过Core
-AI Engine、Agent System、APIs and Tools Provider、Multimodal Processing、Knowledge Base和Task-specific Modules
-6个组件实现自动化AI平台。 Core AI Engine是该框架的核心组件，负责处理和理解各种输入，生成输出和作出决策。Agent
-System是提供高级指导和控制AI代理行为的模块；APIs and Tools Provider提供工具和服务交互的API和集成库；Multimodal
-Processing是一组处理和理解不同数据类型（如文本、图像、音频和视频）的模块，使用深度学习模型从不同数据模式中提取有意义的信息；Knowledge
-Base是一个存储和组织世界信息的大型结构化知识库，使AI代理能够访问和推理大量的知识；Task-specific
-Modules是一组专门设计用于执行特定任务的模块，例如情感分析、机器翻译或目标检测等。通过这些组件的组合，框架提供了一个全面、灵活和强大的平台，能够实现各种复杂任务和应用程序的自动化。
-
-
-# 特性
-
-- 大语言模型支持：支持不同类型的大语言模型的扩展接口
-- 对话终端：提供简易对话终端，直接体验与大语言模型的对话
-- 角色预设：提供预设角色，以不同的角度调用GPT
-- 长对话模式：支持长对话聊天，支持多种方式的对话持久化
-- 外部工具：集成外部工具能力，可以进行网络搜索、执行Python代码等强大的功能
-- KEY池：提供API key池，彻底解决key限速的问题
-- 智能代理：集成ReAct，self-ask等高级Agent，结合外部工具赋能LLM
-- 自治代理模式：支持调用API官方接口、自治代理或使用promptulate提供的代理
-- 中文优化：针对中文语境进行特别优化，更适合中文场景
-- 数据导出：支持markdowm等格式的对话导出
-- 对话总结：提供API式的对话总结、翻译、标题生成
-- 事件总线：自研总线机制，通过[broadcast-service](https://github.com/Undertone0809/broadcast-service)进行Planing与Action的并发调度
-- 高级抽象，支持插件扩展、存储扩展、大语言模型扩展
-
-# 快速开始
-
-- [快速上手 [github-pages]](https://undertone0809.github.io/promptulate/#/)
-- [快速上手 [gitee-pages]](https://zeeland.gitee.io/promptulate/#/)
-- [当前开发计划](https://undertone0809.github.io/promptulate/#/other/plan)
-- [参与贡献/开发者手册](https://undertone0809.github.io/promptulate/#/other/contribution)
-- [常见问题](https://undertone0809.github.io/promptulate/#/other/fqa)
-- [pypi仓库](https://pypi.org/project/promptulate/)
-
-# 基础架构
-
-在本人深度阅读`langchain, Auto-GPT, django, django-rest-framework, gpt_academic...`
-等项目的源码，参与pr之后，学习它们的架构、代码设计思路等内容，重构了两次，有了现在的版本，相较于之前的老版本`prompt-me`，`promptulate`
-重新构建了 `llms, message, memory, framework, preset_roles, tools, provider`等模块，将`prompt`
-的各个流程全部组件化，便有了现在的`promptualte`框架。当前`promptualte`仍有很多细节需要完善，也十分欢迎大家的讨论与参与。
-
-`promptualte`作为一个为大语言模型设计的Prompt Layer框架，主要由以下几部分组成：
-
-- `Agent` 更高级的执行器，负责复杂任务的调度和分发
-- `framework` 框架层，实现不同类型的prompt框架，包括最基础的`Conversation`模型，还有`self-ask`和`ReAct`等模型。
-- `llm` 大语言模型，负责生成回答，可以支持不同类型的大语言模型
-- `memory` 负责对话的存储，支持不同的存储方式及其扩展，如文件存储、数据库存储等
-- `tools` 提供外部工具扩展调用，如搜索引擎、计算器、编译器等
-- `preset roles` 提供预设角色，进行定制化对话
-- `provider` 为framework和agent提供tools和其他细粒度能力的集成
-
-<img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230704180202.png"/>
-
-# 设计原则
-
-promptulate框架的设计原则包括：模块化、可扩展性、互操作性、鲁棒性、可维护性、安全性、效率和可用性。
-
-- 模块化是指以模块为基本单位，允许方便地集成新的组件、模型和工具。
-- 可扩展性是指框架能够处理大量数据、复杂任务和高并发的能力。
-- 互操作性是指该框架与各种外部系统、工具和服务兼容，并且能够实现无缝集成和通信。
-- 鲁棒性是指框架具备强大的错误处理、容错和恢复机制，以确保在各种条件下可靠地运行。
-- 安全性是指框架采用了严格的安全措施，以保护框架、其数据和用户免受未经授权访问和恶意行为的侵害。
-- 效率是指优化框架的性能、资源使用和响应时间，以确保流畅和敏锐的用户体验。
-- 可用性是指该框架采用用户友好的界面和清晰的文档，使其易于使用和理解。
-
-以上原则的遵循，以及最新的人工智能技术的应用，`promptulate`旨在为创建自动化代理提供强大而灵活的大语言模型应用开发框架。
-
-# 交流群
-
-欢迎加入群聊一起交流讨论有关LLM相关的话题，链接过期了可以issue或email提醒一下作者。
-
-<div style="width: 250px;margin: 0 auto;">
-  <img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230702132948.png"/>
-</div>
-
-# 贡献
-
-本人正在尝试一些更加完善的抽象模式，以更好地兼容该框架，以及外部工具的扩展使用，如果你有更好的建议，欢迎一起讨论交流。
-如果你想为这个项目做贡献，请先查看[当前开发计划](https://undertone0809.github.io/promptulate/#/other/plan)
-和[参与贡献/开发者手册](https://undertone0809.github.io/promptulate/#/other/contribution)。我很高兴看到更多的人参与并优化它。
+Metadata-Version: 2.1
+Name: promptulate
+Version: 1.3.0
+Summary: A powerful LLM Application development framework.
+Home-page: https://github.com/Undertone0809/promptulate
+Author: Zeeland
+Author-email: zeeland@foxmail.com
+License: Apache 2.0
+Keywords: promptulate,prompt-me,prompt,chatgpt,gpt,chatbot,llm
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<h1 align="center">
+    promptulate
+</h1>
+
+<p align="center">
+    <a target="_blank" href="">
+        <img src="https://img.shields.io/github/license/Undertone0809/promptulate.svg?style=flat-square" />
+    </a>
+    <a target="_blank" href=''>
+        <img src="https://img.shields.io/github/release/Undertone0809/promptulate/all.svg?style=flat-square"/>
+    </a>
+    <a target="_blank" href=''>
+        <img src="https://bestpractices.coreinfrastructure.org/projects/3018/badge"/>
+   </a>
+</p>
+
+<p align="center">
+  <img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/promptulate_logo_new.png"/>
+</p>
+
+
+`promptulate` 是一个专为Prompt工程师设计的大语言模型自动化与应用开发框架，支持智能决策、消息持久化、外部工具调用、角色预设等功能，开箱即用。
+通过 `promptulate`，你可以轻松构建起属于自己的LLM应用程序。
+
+`promptulate`旨在构建为开发者提供一种强大而灵活的平台，以创建能够自动化各种任务和应用程序的自主代理。通过Core
+AI Engine、Agent System、APIs and Tools Provider、Multimodal Processing、Knowledge Base和Task-specific Modules
+6个组件实现自动化AI平台。 Core AI Engine是该框架的核心组件，负责处理和理解各种输入，生成输出和作出决策。Agent
+System是提供高级指导和控制AI代理行为的模块；APIs and Tools Provider提供工具和服务交互的API和集成库；Multimodal
+Processing是一组处理和理解不同数据类型（如文本、图像、音频和视频）的模块，使用深度学习模型从不同数据模式中提取有意义的信息；Knowledge
+Base是一个存储和组织世界信息的大型结构化知识库，使AI代理能够访问和推理大量的知识；Task-specific
+Modules是一组专门设计用于执行特定任务的模块，例如情感分析、机器翻译或目标检测等。通过这些组件的组合，框架提供了一个全面、灵活和强大的平台，能够实现各种复杂任务和应用程序的自动化。
+
+
+# 特性
+
+- 大语言模型支持：支持不同类型的大语言模型的扩展接口
+- 对话终端：提供简易对话终端，直接体验与大语言模型的对话
+- 角色预设：提供预设角色，以不同的角度调用GPT
+- 长对话模式：支持长对话聊天，支持多种方式的对话持久化
+- 外部工具：集成外部工具能力，可以进行网络搜索、执行Python代码等强大的功能
+- KEY池：提供API key池，彻底解决key限速的问题
+- 智能代理：集成ReAct，self-ask等高级Agent，结合外部工具赋能LLM
+- 自治代理模式：支持调用API官方接口、自治代理或使用promptulate提供的代理
+- 中文优化：针对中文语境进行特别优化，更适合中文场景
+- 数据导出：支持markdowm等格式的对话导出
+- Hook与生命周期：提供Agent，Tool，llm的生命周期及Hook系统
+- 高级抽象：支持插件扩展、存储扩展、大语言模型扩展
+
+# 快速开始
+
+- [快速上手 [github-pages]](https://undertone0809.github.io/promptulate/#/)
+- [快速上手 [gitee-pages]](https://zeeland.gitee.io/promptulate/#/)
+- [当前开发计划](https://undertone0809.github.io/promptulate/#/other/plan)
+- [参与贡献/开发者手册](https://undertone0809.github.io/promptulate/#/other/contribution)
+- [常见问题](https://undertone0809.github.io/promptulate/#/other/fqa)
+- [pypi仓库](https://pypi.org/project/promptulate/)
+
+# 基础架构
+
+当前`promptulate`正处于快速开发阶段，仍有许多内容需要完善与讨论，十分欢迎大家的讨论与参与，而其作为一个大语言模型自动化与应用开发框架，主要由以下几部分组成：
+
+- `Agent` 更高级的执行器，负责复杂任务的调度和分发
+- `llm` 大语言模型，负责生成回答，可以支持不同类型的大语言模型
+- `Memory` 负责对话的存储，支持不同的存储方式及其扩展，如文件存储、数据库存储等
+- `Framework` 框架层，实现不同类型的prompt框架，包括最基础的`Conversation`模型，还有`self-ask`和`ReAct`等模型。
+- `Tool` 提供外部工具扩展调用，如搜索引擎、计算器等
+- `Hook&Lifecycle` Hook系统与生命周期系统，开发者可以进行定制化的生命周期逻辑控制
+- `Rreset roles` 提供预设角色，进行定制化对话
+- `Provider` 为系统提供更多数据源或执行自主操作，如数据库的连接
+
+<img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230704180202.png"/>
+
+# 设计原则
+
+promptulate框架的设计原则包括：模块化、可扩展性、互操作性、鲁棒性、可维护性、安全性、效率和可用性。
+
+- 模块化是指以模块为基本单位，允许方便地集成新的组件、模型和工具。
+- 可扩展性是指框架能够处理大量数据、复杂任务和高并发的能力。
+- 互操作性是指该框架与各种外部系统、工具和服务兼容，并且能够实现无缝集成和通信。
+- 鲁棒性是指框架具备强大的错误处理、容错和恢复机制，以确保在各种条件下可靠地运行。
+- 安全性是指框架采用了严格的安全措施，以保护框架、其数据和用户免受未经授权访问和恶意行为的侵害。
+- 效率是指优化框架的性能、资源使用和响应时间，以确保流畅和敏锐的用户体验。
+- 可用性是指该框架采用用户友好的界面和清晰的文档，使其易于使用和理解。
+
+以上原则的遵循，以及最新的人工智能技术的应用，`promptulate`旨在为创建自动化代理提供强大而灵活的大语言模型应用开发框架。
+
+# 交流群
+
+欢迎加入群聊一起交流讨论有关LLM相关的话题，链接过期了可以issue或email提醒一下作者。
+
+<div style="width: 250px;margin: 0 auto;">
+  <img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230807173459.png"/>
+</div>
+
+
+# 贡献
+
+本人正在尝试一些更加完善的抽象模式，以更好地兼容该框架，以及外部工具的扩展使用，如果你有更好的建议，欢迎一起讨论交流。
+如果你想为这个项目做贡献，请先查看[当前开发计划](https://undertone0809.github.io/promptulate/#/other/plan)
+和[参与贡献/开发者手册](https://undertone0809.github.io/promptulate/#/other/contribution)。我很高兴看到更多的人参与并优化它。
```

### Comparing `promptulate-1.2.2/promptulate.egg-info/SOURCES.txt` & `promptulate-1.3.0/promptulate.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -8,47 +8,58 @@
 promptulate.egg-info/PKG-INFO
 promptulate.egg-info/SOURCES.txt
 promptulate.egg-info/dependency_links.txt
 promptulate.egg-info/entry_points.txt
 promptulate.egg-info/requires.txt
 promptulate.egg-info/top_level.txt
 promptulate/agents/__init__.py
+promptulate/agents/auto_agent.py
+promptulate/agents/tool_agent/__init__.py
+promptulate/agents/tool_agent/agent.py
+promptulate/agents/tool_agent/prompt.py
 promptulate/client/__init__.py
 promptulate/client/chat.py
-promptulate/command/__init__.py
 promptulate/frameworks/__init__.py
 promptulate/frameworks/prompt.py
 promptulate/frameworks/schema.py
 promptulate/frameworks/chain/__init__.py
 promptulate/frameworks/conversation/__init__.py
 promptulate/frameworks/conversation/conversation.py
 promptulate/frameworks/react/__init__.py
 promptulate/frameworks/self_ask/__init__.py
+promptulate/hook/__init__.py
+promptulate/hook/base.py
 promptulate/llms/__init__.py
 promptulate/llms/base.py
-promptulate/llms/openai.py
+promptulate/llms/openai/__init__.py
+promptulate/llms/openai/openai.py
+promptulate/llms/openai/schema.py
 promptulate/memory/__init__.py
 promptulate/memory/base.py
 promptulate/memory/buffer.py
 promptulate/memory/file.py
 promptulate/preset_roles/__init__.py
 promptulate/preset_roles/prompt.py
 promptulate/preset_roles/roles.py
 promptulate/provider/__init__.py
 promptulate/provider/base.py
 promptulate/provider/mixins.py
 promptulate/tools/__init__.py
 promptulate/tools/base.py
+promptulate/tools/manager.py
 promptulate/tools/arxiv/__init__.py
 promptulate/tools/arxiv/api_wrapper.py
 promptulate/tools/arxiv/toolkit.py
 promptulate/tools/arxiv/tools.py
 promptulate/tools/duckduckgo/__init__.py
 promptulate/tools/duckduckgo/api_wrapper.py
 promptulate/tools/duckduckgo/tools.py
+promptulate/tools/math/__init__.py
+promptulate/tools/math/prompt.py
+promptulate/tools/math/tools.py
 promptulate/tools/paper/__init__.py
 promptulate/tools/paper/tools.py
 promptulate/tools/python_repl/__init__.py
 promptulate/tools/python_repl/api_wrapper.py
 promptulate/tools/python_repl/tools.py
 promptulate/tools/semantic_scholar/__init__.py
 promptulate/tools/semantic_scholar/api_wrapper.py
```

