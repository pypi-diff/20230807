# Comparing `tmp/pykoi-0.0.2.tar.gz` & `tmp/pykoi-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykoi-0.0.2.tar", max compression
+gzip compressed data, was "pykoi-0.0.3.tar", max compression
```

## Comparing `pykoi-0.0.2.tar` & `pykoi-0.0.3.tar`

### file list

```diff
@@ -1,92 +1,95 @@
--rw-r--r--   0        0        0    11357 2023-07-29 23:35:02.238057 pykoi-0.0.2/LICENSE.txt
--rw-r--r--   0        0        0     1753 2023-08-01 05:21:35.549386 pykoi-0.0.2/README.md
--rw-r--r--   0        0        0      462 2023-07-31 07:48:56.593127 pykoi-0.0.2/pykoi/__init__.py
--rw-r--r--   0        0        0    17630 2023-07-30 23:19:20.518401 pykoi-0.0.2/pykoi/application.py
--rw-r--r--   0        0        0        0 2023-07-29 23:35:02.243138 pykoi-0.0.2/pykoi/component/__init__.py
--rw-r--r--   0        0        0     3910 2023-07-29 23:35:02.243218 pykoi-0.0.2/pykoi/component/base.py
--rw-r--r--   0        0        0     3291 2023-08-01 05:26:24.768975 pykoi-0.0.2/pykoi/component/chatbot_comparator.py
--rw-r--r--   0        0        0     1033 2023-07-29 23:35:02.243328 pykoi-0.0.2/pykoi/component/chatbot_database_factory.py
--rw-r--r--   0        0        0      139 2023-07-29 23:35:02.243375 pykoi-0.0.2/pykoi/component/constants.py
--rw-r--r--   0        0        0        0 2023-07-29 23:35:02.243424 pykoi-0.0.2/pykoi/db/__init__.py
--rw-r--r--   0        0        0     3175 2023-07-29 23:35:02.243507 pykoi-0.0.2/pykoi/db/abs_database.py
--rw-r--r--   0        0        0     6521 2023-07-29 23:35:02.243569 pykoi-0.0.2/pykoi/db/comparator_database.py
--rw-r--r--   0        0        0      756 2023-07-31 07:48:56.593275 pykoi-0.0.2/pykoi/db/constants.py
--rw-r--r--   0        0        0     6985 2023-07-29 23:35:02.243702 pykoi-0.0.2/pykoi/db/qa_database.py
--rw-r--r--   0        0        0     5883 2023-07-31 07:48:56.593422 pykoi-0.0.2/pykoi/db/ranking_database.py
--rw-r--r--   0        0        0      248 2023-07-29 23:35:02.243850 pykoi-0.0.2/pykoi/frontend/.gitignore
--rw-r--r--   0        0        0     2956 2023-07-29 23:35:02.243912 pykoi-0.0.2/pykoi/frontend/README.md
--rw-r--r--   0        0        0    31654 2023-07-31 07:48:56.593639 pykoi-0.0.2/pykoi/frontend/dist/assets/index-f75c1c12.css
--rw-r--r--   0        0        0   134563 2023-07-31 07:48:56.594277 pykoi-0.0.2/pykoi/frontend/dist/assets/index-fc1a91e8.js
--rw-r--r--   0        0        0      452 2023-07-31 07:48:56.594441 pykoi-0.0.2/pykoi/frontend/dist/index.html
--rw-r--r--   0        0        0     1498 2023-07-29 23:35:02.244816 pykoi-0.0.2/pykoi/frontend/dist/vite.svg
--rw-r--r--   0        0        0      360 2023-07-29 23:35:02.244869 pykoi-0.0.2/pykoi/frontend/index.html
--rw-r--r--   0        0        0      938 2023-07-29 23:35:02.244937 pykoi-0.0.2/pykoi/frontend/jsconfig.json
--rw-r--r--   0        0        0      581 2023-07-29 23:35:02.244992 pykoi-0.0.2/pykoi/frontend/package.json
--rw-r--r--   0        0        0     1498 2023-07-29 23:35:02.245082 pykoi-0.0.2/pykoi/frontend/public/vite.svg
--rw-r--r--   0        0        0     1711 2023-07-30 23:19:20.519624 pykoi-0.0.2/pykoi/frontend/src/App.svelte
--rw-r--r--   0        0        0    10286 2023-07-29 23:35:02.245272 pykoi-0.0.2/pykoi/frontend/src/app.css
--rw-r--r--   0        0        0     1951 2023-07-29 23:35:02.245362 pykoi-0.0.2/pykoi/frontend/src/assets/svelte.svg
--rw-r--r--   0        0        0     4901 2023-07-29 23:35:02.245523 pykoi-0.0.2/pykoi/frontend/src/lib/Annotations/QuestionRating.svelte
--rw-r--r--   0        0        0      290 2023-07-29 23:35:02.245604 pykoi-0.0.2/pykoi/frontend/src/lib/Chatbots/Chat.svelte
--rw-r--r--   0        0        0     8876 2023-07-29 23:35:02.245708 pykoi-0.0.2/pykoi/frontend/src/lib/Chatbots/Chatbot.svelte
--rw-r--r--   0        0        0    10723 2023-07-31 07:48:56.594707 pykoi-0.0.2/pykoi/frontend/src/lib/Chatbots/ComparisonChat.svelte
--rw-r--r--   0        0        0    10985 2023-07-30 23:19:20.520058 pykoi-0.0.2/pykoi/frontend/src/lib/Chatbots/RankChatComparison.svelte
--rw-r--r--   0        0        0     8748 2023-07-30 23:19:20.520243 pykoi-0.0.2/pykoi/frontend/src/lib/Chatbots/RankChatbotOld.svelte
--rw-r--r--   0        0        0     8748 2023-07-30 23:19:20.520475 pykoi-0.0.2/pykoi/frontend/src/lib/Chatbots/RankedChatbot.svelte
--rw-r--r--   0        0        0     6295 2023-07-30 23:19:20.520621 pykoi-0.0.2/pykoi/frontend/src/lib/Comparison/BumpChart.svelte
--rw-r--r--   0        0        0      507 2023-07-29 23:35:02.246162 pykoi-0.0.2/pykoi/frontend/src/lib/Comparison/Cell.svelte
--rw-r--r--   0        0        0     5351 2023-07-30 23:19:20.520740 pykoi-0.0.2/pykoi/frontend/src/lib/Comparison/ComparisonChart.svelte
--rw-r--r--   0        0        0     4924 2023-07-30 23:19:20.520861 pykoi-0.0.2/pykoi/frontend/src/lib/Comparison/CumulativeScore.svelte
--rw-r--r--   0        0        0     5027 2023-07-30 23:19:20.520979 pykoi-0.0.2/pykoi/frontend/src/lib/Comparison/CumulativeStack.svelte
--rw-r--r--   0        0        0     4952 2023-07-30 23:19:20.521096 pykoi-0.0.2/pykoi/frontend/src/lib/Comparison/Heatmap.svelte
--rw-r--r--   0        0        0     3269 2023-07-30 23:19:20.521232 pykoi-0.0.2/pykoi/frontend/src/lib/Comparison/HorizontalBar.svelte
--rw-r--r--   0        0        0     5916 2023-07-30 23:19:20.521356 pykoi-0.0.2/pykoi/frontend/src/lib/Comparison/Table.svelte
--rw-r--r--   0        0        0     9692 2023-07-29 23:35:02.246653 pykoi-0.0.2/pykoi/frontend/src/lib/Comparison/data.js
--rw-r--r--   0        0        0     2018 2023-07-30 23:19:20.521484 pykoi-0.0.2/pykoi/frontend/src/lib/Comparison/store.js
--rw-r--r--   0        0        0     3644 2023-07-31 07:48:56.594904 pykoi-0.0.2/pykoi/frontend/src/lib/Dashboards/DashboardFeedback/ColumnChart.svelte
--rw-r--r--   0        0        0     3905 2023-07-29 23:35:02.246928 pykoi-0.0.2/pykoi/frontend/src/lib/Dashboards/DashboardFeedback/HistogramAnswer.svelte
--rw-r--r--   0        0        0     3890 2023-07-29 23:35:02.246987 pykoi-0.0.2/pykoi/frontend/src/lib/Dashboards/DashboardFeedback/HistogramQuestion.svelte
--rw-r--r--   0        0        0     4421 2023-07-29 23:35:02.247047 pykoi-0.0.2/pykoi/frontend/src/lib/Dashboards/DashboardFeedback/HorizontalStackedBar.svelte
--rw-r--r--   0        0        0     2701 2023-07-29 23:35:02.247105 pykoi-0.0.2/pykoi/frontend/src/lib/Dashboards/DashboardFeedback/MetricCardAbsolute.svelte
--rw-r--r--   0        0        0     2638 2023-07-29 23:35:02.247166 pykoi-0.0.2/pykoi/frontend/src/lib/Dashboards/DashboardFeedback/MetricCardPercentage.svelte
--rw-r--r--   0        0        0     1384 2023-07-29 23:35:02.247225 pykoi-0.0.2/pykoi/frontend/src/lib/Dashboards/DashboardFeedback/QACard.svelte
--rw-r--r--   0        0        0      998 2023-07-31 07:48:56.595032 pykoi-0.0.2/pykoi/frontend/src/lib/Dashboards/DashboardFeedback/QATable.svelte
--rw-r--r--   0        0        0     3326 2023-07-29 23:35:02.247365 pykoi-0.0.2/pykoi/frontend/src/lib/Dashboards/Feedback.svelte
--rw-r--r--   0        0        0     4317 2023-07-29 23:35:02.247488 pykoi-0.0.2/pykoi/frontend/src/lib/Evaluation/Bar.svelte
--rw-r--r--   0        0        0     4311 2023-07-29 23:35:02.247543 pykoi-0.0.2/pykoi/frontend/src/lib/Evaluation/BumpChart.svelte
--rw-r--r--   0        0        0      507 2023-07-29 23:35:02.247600 pykoi-0.0.2/pykoi/frontend/src/lib/Evaluation/Cell.svelte
--rw-r--r--   0        0        0     3651 2023-07-29 23:35:02.247649 pykoi-0.0.2/pykoi/frontend/src/lib/Evaluation/ComparisonChart.svelte
--rw-r--r--   0        0        0     5362 2023-07-29 23:35:02.247712 pykoi-0.0.2/pykoi/frontend/src/lib/Evaluation/EvalLineChart.svelte
--rw-r--r--   0        0        0     3910 2023-07-29 23:35:02.247757 pykoi-0.0.2/pykoi/frontend/src/lib/Evaluation/LineChart.svelte
--rw-r--r--   0        0        0     3611 2023-07-29 23:35:02.247816 pykoi-0.0.2/pykoi/frontend/src/lib/Evaluation/RLHFEvaluation.svelte
--rw-r--r--   0        0        0     5069 2023-07-29 23:35:02.247882 pykoi-0.0.2/pykoi/frontend/src/lib/Evaluation/Table.svelte
--rw-r--r--   0        0        0     4655 2023-07-29 23:35:02.247934 pykoi-0.0.2/pykoi/frontend/src/lib/Evaluation/data.js
--rw-r--r--   0        0        0      584 2023-07-29 23:35:02.247984 pykoi-0.0.2/pykoi/frontend/src/lib/Evaluation/store.js
--rw-r--r--   0        0        0      380 2023-07-29 23:35:02.248077 pykoi-0.0.2/pykoi/frontend/src/lib/UIComponents/Dropdown.svelte
--rw-r--r--   0        0        0      191 2023-07-29 23:35:02.248132 pykoi-0.0.2/pykoi/frontend/src/main.js
--rw-r--r--   0        0        0     6818 2023-07-29 23:35:02.248201 pykoi-0.0.2/pykoi/frontend/src/normalize.css
--rw-r--r--   0        0        0      586 2023-07-31 07:48:56.595166 pykoi-0.0.2/pykoi/frontend/src/store.js
--rw-r--r--   0        0        0     9194 2023-07-29 23:35:02.248302 pykoi-0.0.2/pykoi/frontend/src/styles.css
--rw-r--r--   0        0        0     1725 2023-07-31 07:48:56.595300 pykoi-0.0.2/pykoi/frontend/src/utils.js
--rw-r--r--   0        0        0       71 2023-07-29 23:35:02.248401 pykoi-0.0.2/pykoi/frontend/src/vite-env.d.ts
--rw-r--r--   0        0        0      228 2023-07-29 23:35:02.248463 pykoi-0.0.2/pykoi/frontend/svelte.config.js
--rw-r--r--   0        0        0      177 2023-07-29 23:35:02.248512 pykoi-0.0.2/pykoi/frontend/vite.config.js
--rw-r--r--   0        0        0        0 2023-08-01 05:26:24.769038 pykoi-0.0.2/pykoi/interactives/__init__.py
--rw-r--r--   0        0        0    30580 2023-08-01 05:26:24.769471 pykoi-0.0.2/pykoi/interactives/barchart.py
--rw-r--r--   0        0        0        0 2023-07-29 23:35:02.248566 pykoi-0.0.2/pykoi/llm/__init__.py
--rw-r--r--   0        0        0     1203 2023-07-29 23:35:02.248632 pykoi-0.0.2/pykoi/llm/abs_llm.py
--rw-r--r--   0        0        0      455 2023-07-29 23:35:02.248682 pykoi-0.0.2/pykoi/llm/constants.py
--rw-r--r--   0        0        0     3751 2023-08-01 05:21:35.587141 pykoi-0.0.2/pykoi/llm/huggingface.py
--rw-r--r--   0        0        0     9257 2023-08-01 05:21:35.587256 pykoi-0.0.2/pykoi/llm/instruct_pipeline.py
--rw-r--r--   0        0        0     2077 2023-07-29 23:35:02.248800 pykoi-0.0.2/pykoi/llm/model_factory.py
--rw-r--r--   0        0        0     2440 2023-07-29 23:35:02.248858 pykoi-0.0.2/pykoi/llm/openai.py
--rw-r--r--   0        0        0     3797 2023-07-29 23:35:02.248920 pykoi-0.0.2/pykoi/llm/peft_huggingface.py
--rw-r--r--   0        0        0        0 2023-07-29 23:35:02.248971 pykoi-0.0.2/pykoi/rlhf/__init__.py
--rw-r--r--   0        0        0    12377 2023-07-31 07:48:56.595643 pykoi-0.0.2/pykoi/rlhf/config.py
--rw-r--r--   0        0        0       21 2023-07-29 23:35:02.249106 pykoi-0.0.2/pykoi/rlhf/rl_finetuning.py
--rw-r--r--   0        0        0    27621 2023-07-31 07:48:56.595876 pykoi-0.0.2/pykoi/rlhf/rlhf.py
--rw-r--r--   0        0        0       31 2023-07-29 23:35:02.249377 pykoi-0.0.2/pykoi/rlhf/rw_finetuning.py
--rw-r--r--   0        0        0     8145 2023-07-31 07:48:56.596054 pykoi-0.0.2/pykoi/rlhf/supervised_finetuning.py
--rw-r--r--   0        0        0     1014 2023-07-29 23:35:02.249509 pykoi-0.0.2/pykoi/state.py
--rw-r--r--   0        0        0      689 2023-08-01 05:57:59.479559 pykoi-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2811 1970-01-01 00:00:00.000000 pykoi-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-28 03:17:36.059231 pykoi-0.0.3/LICENSE.txt
+-rw-r--r--   0        0        0     1753 2023-08-07 07:39:05.947198 pykoi-0.0.3/README.md
+-rw-r--r--   0        0        0      609 2023-08-07 07:39:17.106386 pykoi-0.0.3/pykoi/__init__.py
+-rw-r--r--   0        0        0    18484 2023-08-07 07:39:06.107124 pykoi-0.0.3/pykoi/application.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:39:06.107275 pykoi-0.0.3/pykoi/chat/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:39:06.107404 pykoi-0.0.3/pykoi/chat/db/__init__.py
+-rw-r--r--   0        0        0     3217 2023-08-07 07:39:06.107754 pykoi-0.0.3/pykoi/chat/db/abs_database.py
+-rw-r--r--   0        0        0     6539 2023-08-07 07:39:06.107951 pykoi-0.0.3/pykoi/chat/db/comparator_database.py
+-rw-r--r--   0        0        0      757 2023-08-07 07:39:06.108209 pykoi-0.0.3/pykoi/chat/db/constants.py
+-rw-r--r--   0        0        0     7007 2023-08-07 07:39:06.108466 pykoi-0.0.3/pykoi/chat/db/qa_database.py
+-rw-r--r--   0        0        0     5918 2023-08-07 07:39:06.108734 pykoi-0.0.3/pykoi/chat/db/ranking_database.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:39:06.108887 pykoi-0.0.3/pykoi/chat/llm/__init__.py
+-rw-r--r--   0        0        0     1247 2023-08-07 07:39:06.109125 pykoi-0.0.3/pykoi/chat/llm/abs_llm.py
+-rw-r--r--   0        0        0      255 2023-08-07 07:39:06.109346 pykoi-0.0.3/pykoi/chat/llm/constants.py
+-rw-r--r--   0        0        0     4026 2023-08-07 07:39:06.109538 pykoi-0.0.3/pykoi/chat/llm/huggingface.py
+-rw-r--r--   0        0        0     9999 2023-08-07 07:39:06.109956 pykoi-0.0.3/pykoi/chat/llm/instruct_pipeline.py
+-rw-r--r--   0        0        0     1979 2023-08-07 07:39:06.110251 pykoi-0.0.3/pykoi/chat/llm/model_factory.py
+-rw-r--r--   0        0        0     2668 2023-08-07 07:39:06.110566 pykoi-0.0.3/pykoi/chat/llm/openai.py
+-rw-r--r--   0        0        0     4025 2023-08-07 07:39:06.110835 pykoi-0.0.3/pykoi/chat/llm/peft_huggingface.py
+-rw-r--r--   0        0        0        0 2023-07-28 03:17:36.064112 pykoi-0.0.3/pykoi/component/__init__.py
+-rw-r--r--   0        0        0     3963 2023-08-07 07:39:06.111163 pykoi-0.0.3/pykoi/component/base.py
+-rw-r--r--   0        0        0     3647 2023-08-07 07:39:06.111426 pykoi-0.0.3/pykoi/component/chatbot_comparator.py
+-rw-r--r--   0        0        0     1042 2023-08-07 07:39:06.111677 pykoi-0.0.3/pykoi/component/chatbot_database_factory.py
+-rw-r--r--   0        0        0      139 2023-07-28 03:17:36.064387 pykoi-0.0.3/pykoi/component/constants.py
+-rw-r--r--   0        0        0      248 2023-07-28 03:17:36.064797 pykoi-0.0.3/pykoi/frontend/.gitignore
+-rw-r--r--   0        0        0     2956 2023-07-28 03:17:36.064882 pykoi-0.0.3/pykoi/frontend/README.md
+-rw-r--r--   0        0        0    31654 2023-08-02 07:41:16.796141 pykoi-0.0.3/pykoi/frontend/dist/assets/index-f75c1c12.css
+-rw-r--r--   0        0        0   134563 2023-08-02 07:41:16.799933 pykoi-0.0.3/pykoi/frontend/dist/assets/index-fc1a91e8.js
+-rw-r--r--   0        0        0      452 2023-08-02 07:41:16.800123 pykoi-0.0.3/pykoi/frontend/dist/index.html
+-rw-r--r--   0        0        0     1498 2023-07-30 20:34:15.890204 pykoi-0.0.3/pykoi/frontend/dist/vite.svg
+-rw-r--r--   0        0        0      360 2023-07-28 03:17:36.065707 pykoi-0.0.3/pykoi/frontend/index.html
+-rw-r--r--   0        0        0      938 2023-07-28 03:17:36.065763 pykoi-0.0.3/pykoi/frontend/jsconfig.json
+-rw-r--r--   0        0        0      581 2023-07-28 03:17:36.065811 pykoi-0.0.3/pykoi/frontend/package.json
+-rw-r--r--   0        0        0     1498 2023-07-28 03:17:36.065890 pykoi-0.0.3/pykoi/frontend/public/vite.svg
+-rw-r--r--   0        0        0     1711 2023-07-31 02:36:42.777272 pykoi-0.0.3/pykoi/frontend/src/App.svelte
+-rw-r--r--   0        0        0    10286 2023-07-28 03:17:36.066086 pykoi-0.0.3/pykoi/frontend/src/app.css
+-rw-r--r--   0        0        0     1951 2023-07-28 03:17:36.066188 pykoi-0.0.3/pykoi/frontend/src/assets/svelte.svg
+-rw-r--r--   0        0        0     4901 2023-07-28 03:17:36.066360 pykoi-0.0.3/pykoi/frontend/src/lib/Annotations/QuestionRating.svelte
+-rw-r--r--   0        0        0      290 2023-07-28 03:17:36.066469 pykoi-0.0.3/pykoi/frontend/src/lib/Chatbots/Chat.svelte
+-rw-r--r--   0        0        0     8876 2023-07-28 03:17:36.066581 pykoi-0.0.3/pykoi/frontend/src/lib/Chatbots/Chatbot.svelte
+-rw-r--r--   0        0        0    10723 2023-08-02 07:41:16.800335 pykoi-0.0.3/pykoi/frontend/src/lib/Chatbots/ComparisonChat.svelte
+-rw-r--r--   0        0        0    10985 2023-07-31 02:36:42.777514 pykoi-0.0.3/pykoi/frontend/src/lib/Chatbots/RankChatComparison.svelte
+-rw-r--r--   0        0        0     8748 2023-07-31 02:36:42.777778 pykoi-0.0.3/pykoi/frontend/src/lib/Chatbots/RankChatbotOld.svelte
+-rw-r--r--   0        0        0     8748 2023-07-30 20:51:42.598743 pykoi-0.0.3/pykoi/frontend/src/lib/Chatbots/RankedChatbot.svelte
+-rw-r--r--   0        0        0     6295 2023-07-30 20:51:42.599158 pykoi-0.0.3/pykoi/frontend/src/lib/Comparison/BumpChart.svelte
+-rw-r--r--   0        0        0      507 2023-07-28 03:17:36.067038 pykoi-0.0.3/pykoi/frontend/src/lib/Comparison/Cell.svelte
+-rw-r--r--   0        0        0     5351 2023-07-31 02:36:42.778071 pykoi-0.0.3/pykoi/frontend/src/lib/Comparison/ComparisonChart.svelte
+-rw-r--r--   0        0        0     4924 2023-07-30 00:59:42.352803 pykoi-0.0.3/pykoi/frontend/src/lib/Comparison/CumulativeScore.svelte
+-rw-r--r--   0        0        0     5027 2023-07-30 00:59:42.353142 pykoi-0.0.3/pykoi/frontend/src/lib/Comparison/CumulativeStack.svelte
+-rw-r--r--   0        0        0     4952 2023-07-30 04:56:55.351706 pykoi-0.0.3/pykoi/frontend/src/lib/Comparison/Heatmap.svelte
+-rw-r--r--   0        0        0     3269 2023-07-30 04:56:55.351950 pykoi-0.0.3/pykoi/frontend/src/lib/Comparison/HorizontalBar.svelte
+-rw-r--r--   0        0        0     5916 2023-07-30 04:56:55.352211 pykoi-0.0.3/pykoi/frontend/src/lib/Comparison/Table.svelte
+-rw-r--r--   0        0        0     9692 2023-07-30 00:59:42.355220 pykoi-0.0.3/pykoi/frontend/src/lib/Comparison/data.js
+-rw-r--r--   0        0        0     2018 2023-07-30 20:51:42.599507 pykoi-0.0.3/pykoi/frontend/src/lib/Comparison/store.js
+-rw-r--r--   0        0        0     3644 2023-08-02 07:41:16.800635 pykoi-0.0.3/pykoi/frontend/src/lib/Dashboards/DashboardFeedback/ColumnChart.svelte
+-rw-r--r--   0        0        0     3905 2023-07-28 03:17:36.068046 pykoi-0.0.3/pykoi/frontend/src/lib/Dashboards/DashboardFeedback/HistogramAnswer.svelte
+-rw-r--r--   0        0        0     3890 2023-07-28 03:17:36.068119 pykoi-0.0.3/pykoi/frontend/src/lib/Dashboards/DashboardFeedback/HistogramQuestion.svelte
+-rw-r--r--   0        0        0     4421 2023-07-28 03:17:36.068191 pykoi-0.0.3/pykoi/frontend/src/lib/Dashboards/DashboardFeedback/HorizontalStackedBar.svelte
+-rw-r--r--   0        0        0     2701 2023-07-28 03:17:36.068259 pykoi-0.0.3/pykoi/frontend/src/lib/Dashboards/DashboardFeedback/MetricCardAbsolute.svelte
+-rw-r--r--   0        0        0     2638 2023-07-28 03:17:36.068321 pykoi-0.0.3/pykoi/frontend/src/lib/Dashboards/DashboardFeedback/MetricCardPercentage.svelte
+-rw-r--r--   0        0        0     1384 2023-07-28 03:17:36.068384 pykoi-0.0.3/pykoi/frontend/src/lib/Dashboards/DashboardFeedback/QACard.svelte
+-rw-r--r--   0        0        0      998 2023-08-02 07:41:16.800838 pykoi-0.0.3/pykoi/frontend/src/lib/Dashboards/DashboardFeedback/QATable.svelte
+-rw-r--r--   0        0        0     3326 2023-07-28 03:17:36.068523 pykoi-0.0.3/pykoi/frontend/src/lib/Dashboards/Feedback.svelte
+-rw-r--r--   0        0        0     4317 2023-07-28 03:17:36.068640 pykoi-0.0.3/pykoi/frontend/src/lib/Evaluation/Bar.svelte
+-rw-r--r--   0        0        0     4311 2023-07-28 03:17:36.068727 pykoi-0.0.3/pykoi/frontend/src/lib/Evaluation/BumpChart.svelte
+-rw-r--r--   0        0        0      507 2023-07-28 03:17:36.068793 pykoi-0.0.3/pykoi/frontend/src/lib/Evaluation/Cell.svelte
+-rw-r--r--   0        0        0     3651 2023-07-28 03:17:36.068852 pykoi-0.0.3/pykoi/frontend/src/lib/Evaluation/ComparisonChart.svelte
+-rw-r--r--   0        0        0     5362 2023-07-28 03:17:36.068930 pykoi-0.0.3/pykoi/frontend/src/lib/Evaluation/EvalLineChart.svelte
+-rw-r--r--   0        0        0     3910 2023-07-28 03:17:36.068986 pykoi-0.0.3/pykoi/frontend/src/lib/Evaluation/LineChart.svelte
+-rw-r--r--   0        0        0     3611 2023-07-28 03:17:36.069049 pykoi-0.0.3/pykoi/frontend/src/lib/Evaluation/RLHFEvaluation.svelte
+-rw-r--r--   0        0        0     5069 2023-07-28 03:17:36.069116 pykoi-0.0.3/pykoi/frontend/src/lib/Evaluation/Table.svelte
+-rw-r--r--   0        0        0     4655 2023-07-28 03:17:36.069185 pykoi-0.0.3/pykoi/frontend/src/lib/Evaluation/data.js
+-rw-r--r--   0        0        0      584 2023-07-28 03:17:36.069239 pykoi-0.0.3/pykoi/frontend/src/lib/Evaluation/store.js
+-rw-r--r--   0        0        0      380 2023-07-28 03:17:36.069325 pykoi-0.0.3/pykoi/frontend/src/lib/UIComponents/Dropdown.svelte
+-rw-r--r--   0        0        0      191 2023-07-28 03:17:36.069380 pykoi-0.0.3/pykoi/frontend/src/main.js
+-rw-r--r--   0        0        0     6818 2023-07-28 03:17:36.069449 pykoi-0.0.3/pykoi/frontend/src/normalize.css
+-rw-r--r--   0        0        0      586 2023-08-02 07:41:16.801117 pykoi-0.0.3/pykoi/frontend/src/store.js
+-rw-r--r--   0        0        0     9194 2023-07-28 03:17:36.069592 pykoi-0.0.3/pykoi/frontend/src/styles.css
+-rw-r--r--   0        0        0     1725 2023-08-02 07:41:16.801375 pykoi-0.0.3/pykoi/frontend/src/utils.js
+-rw-r--r--   0        0        0       71 2023-07-28 03:17:36.069716 pykoi-0.0.3/pykoi/frontend/src/vite-env.d.ts
+-rw-r--r--   0        0        0      228 2023-07-28 03:17:36.069783 pykoi-0.0.3/pykoi/frontend/svelte.config.js
+-rw-r--r--   0        0        0      177 2023-07-28 03:17:36.069844 pykoi-0.0.3/pykoi/frontend/vite.config.js
+-rw-r--r--   0        0        0        0 2023-08-07 07:39:06.111735 pykoi-0.0.3/pykoi/interactives/__init__.py
+-rw-r--r--   0        0        0    30580 2023-08-07 07:39:06.112153 pykoi-0.0.3/pykoi/interactives/barchart.py
+-rw-r--r--   0        0        0        0 2023-08-04 05:18:56.790736 pykoi-0.0.3/pykoi/rlhf/__init__.py
+-rw-r--r--   0        0        0    12733 2023-08-07 07:39:06.112492 pykoi-0.0.3/pykoi/rlhf/config.py
+-rw-r--r--   0        0        0    13406 2023-08-07 07:39:06.112949 pykoi-0.0.3/pykoi/rlhf/rl_finetuning.py
+-rw-r--r--   0        0        0    11549 2023-08-07 07:39:06.113238 pykoi-0.0.3/pykoi/rlhf/rw_finetuning.py
+-rw-r--r--   0        0        0     8387 2023-08-07 07:39:06.113594 pykoi-0.0.3/pykoi/rlhf/supervised_finetuning.py
+-rw-r--r--   0        0        0     1014 2023-08-03 01:59:55.421837 pykoi-0.0.3/pykoi/state.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:39:06.113818 pykoi-0.0.3/pykoi/telemetry/__init__.py
+-rw-r--r--   0        0        0     3308 2023-08-07 07:39:06.114390 pykoi-0.0.3/pykoi/telemetry/events.py
+-rw-r--r--   0        0        0     3469 2023-08-07 07:39:06.114590 pykoi-0.0.3/pykoi/telemetry/telemetry.py
+-rw-r--r--   0        0        0      745 2023-08-07 07:39:26.951928 pykoi-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2913 1970-01-01 00:00:00.000000 pykoi-0.0.3/PKG-INFO
```

### Comparing `pykoi-0.0.2/LICENSE.txt` & `pykoi-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pykoi-0.0.2/README.md` & `pykoi-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pykoi-0.0.2/pykoi/application.py` & `pykoi-0.0.3/pykoi/application.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 """Application module."""
 import os
 import socket
-
+import time
+from datetime import datetime
 from typing import List, Optional, Any, Dict, Union
 from fastapi import FastAPI, Depends, HTTPException, status
 from fastapi.security import HTTPBasic, HTTPBasicCredentials
 from passlib.context import CryptContext
 from fastapi.responses import JSONResponse
 from fastapi.staticfiles import StaticFiles
 from pydantic import BaseModel
 from pyngrok import ngrok
 from starlette.middleware.cors import CORSMiddleware
 from pykoi.component.base import Dropdown
+from pykoi.telemetry.telemetry import Telemetry
+from pykoi.telemetry.events import (
+    AppStartEvent,
+    AppStopEvent)
+
+
+oauth_scheme = HTTPBasic()
 
 
 class UpdateQATable(BaseModel):
     id: int
     vote_status: str
 
 
@@ -36,32 +44,14 @@
     answer: str
 
 
 class ComparatorInsertRequest(BaseModel):
     data: List[ModelAnswer]
 
 
-def find_free_port():
-    with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
-        s.bind(("", 0))  # binds to an arbitrary free port
-        return s.getsockname()[1]
-
-
-# def find_free_port():
-#     s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-#     s.bind(("", 0))  # binds to an arbitrary free port
-#     s.listen(1)
-#     port = s.getsockname()[1]
-#     s.close()
-#     return port
-
-
-oauth_scheme = HTTPBasic()
-
-
 class UserInDB:
     def __init__(self, username: str, hashed_password: str):
         self.username = username
         self.hashed_password = hashed_password
 
 
 class Application:
@@ -71,26 +61,34 @@
 
     def __init__(
         self,
         share: bool = False,
         debug: bool = False,
         username: Union[None, str, List] = None,
         password: Union[None, str, List] = None,
+        host: str = "127.0.0.1",
+        port: int = 5000,
+        enable_telemetry: bool = True,
     ):
         """
         Initialize the Application.
 
         Args:
             share (bool, optional): If True, the application will be shared via ngrok. Defaults to False.
             debug (bool, optional): If True, the application will run in debug mode. Defaults to False.
             username (str, optional): The username for authentication. Defaults to None.
             password (str, optional): The password for authentication. Defaults to None.
+            host (str): The host to run the application on. Defaults to None.
+            port (int): The port to run the application on. Defaults to None.
+            enable_telemetry (bool, optional): If True, enable_telemetry will be enabled. Defaults to True.
         """
         self._debug = debug
         self._share = share
+        self._host = host
+        self._port = port
         self.data_sources = {}
         self.components = []
         if username and password:
             self._auth = True
         else:
             self._auth = False
         if isinstance(username, str):
@@ -98,37 +96,42 @@
         if isinstance(password, str):
             password = [password]
         if (
             username is not None
             and password is not None
             and len(username) != len(password)
         ):
-            raise ValueError("The length of username and password must be the same.")
+            raise ValueError(
+                "The length of username and password must be the same."
+            )
         self._pwd_context = CryptContext(schemes=["bcrypt"], deprecated="auto")
 
         self._fake_users_db = {}
         if username is not None and password is not None:
             for user_name, pass_word in zip(username, password):
                 self._fake_users_db[user_name] = UserInDB(
                     username=user_name,
                     hashed_password=self._pwd_context.hash(pass_word),
                 )
+        self._telemetry = Telemetry(enable_telemetry)
 
     def authenticate_user(self, fake_db, username: str, password: str):
         if self._auth:
             user = fake_db.get(username)
             if not user:
                 return False
             if not self._pwd_context.verify(password, user.hashed_password):
                 return False
             return user
         else:
             return "no_auth"
 
-    def auth_required(self, credentials: HTTPBasicCredentials = Depends(oauth_scheme)):
+    def auth_required(
+        self, credentials: HTTPBasicCredentials = Depends(oauth_scheme)
+    ):
         user = self.authenticate_user(
             self._fake_users_db, credentials.username, credentials.password
         )
         if not user:
             raise HTTPException(
                 status_code=status.HTTP_401_UNAUTHORIZED,
                 detail="Incorrect username or password",
@@ -223,15 +226,17 @@
         async def inference_ranking_table(
             message: str,
             request_body: InferenceRankingTable,
             user: Union[None, UserInDB] = Depends(self.get_auth_dependency()),
         ):
             try:
                 num_of_response = request_body.n
-                output = component["component"].model.predict(message, num_of_response)
+                output = component["component"].model.predict(
+                    message, num_of_response
+                )
                 # Check the type of each item in the output list
                 return {
                     "log": "Inference complete",
                     "status": "200",
                     "question": message,
                     "answer": output,
                 }
@@ -255,15 +260,17 @@
 
         @app.get("/chat/ranking_table/retrieve")
         async def retrieve_ranking_table(
             user: Union[None, UserInDB] = Depends(self.get_auth_dependency())
         ):
             try:
                 print("retrieve_ranking_table")
-                rows = component["component"].database.retrieve_all_question_answers()
+                rows = component[
+                    "component"
+                ].database.retrieve_all_question_answers()
                 return {"rows": rows, "log": "Table retrieved", "status": "200"}
             except Exception as ex:
                 return {"log": f"Table retrieval failed: {ex}", "status": "500"}
 
     def create_feedback_route(self, app: FastAPI, component: Dict[str, Any]):
         """
         Create feedback routes for the application.
@@ -274,30 +281,34 @@
         """
 
         @app.get("/chat/qa_table/retrieve")
         async def retrieve_qa_table(
             user: Union[None, UserInDB] = Depends(self.get_auth_dependency())
         ):
             try:
-                rows = component["component"].database.retrieve_all_question_answers()
+                rows = component[
+                    "component"
+                ].database.retrieve_all_question_answers()
                 return {"rows": rows, "log": "Table retrieved", "status": "200"}
             except Exception as ex:
                 return {"log": f"Table retrieval failed: {ex}", "status": "500"}
 
         @app.get("/chat/ranking_table/close")
         async def close_ranking_table(
             user: Union[None, UserInDB] = Depends(self.get_auth_dependency())
         ):
             try:
                 component["component"].database.close_connection()
                 return {"log": "Table closed", "status": "200"}
             except Exception as ex:
                 return {"log": f"Table close failed: {ex}", "status": "500"}
 
-    def create_chatbot_comparator_route(self, app: FastAPI, component: Dict[str, Any]):
+    def create_chatbot_comparator_route(
+        self, app: FastAPI, component: Dict[str, Any]
+    ):
         """
         Create chatbot comparator routes for the application.
 
         Args:
             app (FastAPI): The FastAPI application.
             component (Dict[str, Any]): The component for which the routes are being created.
         """
@@ -433,15 +444,17 @@
             Args:
                 id (str): The id of the data source.
                 data_source (Any): The data source.
             """
 
             @app.get(f"/data/{id}")
             async def get_data(
-                user: Union[None, UserInDB] = Depends(self.get_auth_dependency())
+                user: Union[None, UserInDB] = Depends(
+                    self.get_auth_dependency()
+                )
             ):
                 data = data_source.fetch_func()
                 return JSONResponse(data)
 
         for id, data_source in self.data_sources.items():
             create_data_route(id, data_source)
 
@@ -462,28 +475,39 @@
                 html=True,
             ),
             name="static",
         )
 
         @app.get("/{path:path}")
         async def read_item(
-            path: str, user: Union[None, UserInDB] = Depends(self.get_auth_dependency())
+            path: str,
+            user: Union[None, UserInDB] = Depends(self.get_auth_dependency()),
         ):
             return {"path": path}
 
         # debug mode should be set to False in production because
         # it will start two processes when debug mode is enabled.
 
         # Set the ngrok tunnel if share is True
-        port = find_free_port()
+        start_event = AppStartEvent(
+            start_time=time.time(),
+            date_time=datetime.utcfromtimestamp(time.time())
+        )
+        self._telemetry.capture(start_event)
+
         if self._share:
-            public_url = ngrok.connect(port)
+            public_url = ngrok.connect(self._host + ":" + str(self._port))
             print("Public URL:", public_url)
             import uvicorn
 
-            uvicorn.run(app, host="127.0.0.1", port=port)
+            uvicorn.run(app, host=self._host, port=self._port)
             print("Stopping server...")
             ngrok.disconnect(public_url)
         else:
             import uvicorn
 
-            uvicorn.run(app, host="127.0.0.1", port=port)
+            uvicorn.run(app, host=self._host, port=self._port)
+        self._telemetry.capture(AppStopEvent(
+            end_time=time.time(),
+            date_time=datetime.utcfromtimestamp(time.time()),
+            duration=time.time() - start_event.start_time
+        ))
```

### Comparing `pykoi-0.0.2/pykoi/component/base.py` & `pykoi-0.0.3/pykoi/component/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Base classes for components."""
 import uuid
 from typing import Callable, List, Optional, Union
 
 from pykoi.component.chatbot_database_factory import ChatbotDatabaseFactory
 from pykoi.component.constants import FeedbackType
-from pykoi.db.qa_database import QuestionAnswerDatabase
-from pykoi.db.ranking_database import RankingDatabase
-from pykoi.llm.abs_llm import AbsLlm
+from pykoi.chat.db.qa_database import QuestionAnswerDatabase
+from pykoi.chat.db.ranking_database import RankingDatabase
+from pykoi.chat.llm.abs_llm import AbsLlm
 
 
 class DataSource:
     """
     DataSource class is used to fetch data from a source using a provided function.
 
     Attributes:
@@ -37,25 +37,29 @@
     Attributes:
         id (str): The unique identifier for the component.
         data_source (DataSource): The data source for the component.
         svelte_component (str): The name of the Svelte component.
         props (Dict[str, Any]): Additional properties for the component.
     """
 
-    def __init__(self, fetch_func: Optional[Callable], svelte_component: str, **kwargs):
+    def __init__(
+        self, fetch_func: Optional[Callable], svelte_component: str, **kwargs
+    ):
         """
         Initialize a new instance of Component.
 
         Args:
             fetch_func (Callable, optional): The function to fetch data for the component.
             svelte_component (str): The name of the Svelte component.
             kwargs: Additional properties for the component.
         """
         self.id = str(uuid.uuid4())  # Generate a unique ID
-        self.data_source = DataSource(self.id, fetch_func) if fetch_func else None
+        self.data_source = (
+            DataSource(self.id, fetch_func) if fetch_func else None
+        )
         self.svelte_component = svelte_component
         self.props = kwargs
 
 
 class Dropdown(Component):
     """
     Dropdown class represents a dropdown component.
```

### Comparing `pykoi-0.0.2/pykoi/component/chatbot_comparator.py` & `pykoi-0.0.3/pykoi/component/chatbot_comparator.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 """Chatbot comparator component."""
 import time
 import pandas as pd
 
 from typing import List
 
 from pykoi.component.base import Component
-from pykoi.db.comparator_database import ComparatorDatabase, ComparatorQuestionDatabase
-from pykoi.llm.abs_llm import AbsLlm
+from pykoi.chat.db.comparator_database import (
+    ComparatorDatabase,
+    ComparatorQuestionDatabase,
+)
+from pykoi.chat.llm.abs_llm import AbsLlm
 from pykoi.interactives.barchart import Barchart
 
 
 def df_to_js_array(df):
     records = df.to_dict(orient="records")
     return records
 
@@ -33,15 +36,21 @@
         super().__init__(None, "Compare", **kwargs)
         self.models = {}
         for model in models:
             self.add(model)
         self.question_db = ComparatorQuestionDatabase()
         self.comparator_db = ComparatorDatabase()
         self.inference_results = pd.DataFrame(
-            columns=["question", "model", "answer", "latency", "length_in_tokens"]
+            columns=[
+                "question",
+                "model",
+                "answer",
+                "latency",
+                "length_in_tokens",
+            ]
         )  # Added this line
 
     def add(self, model: AbsLlm):
         """
         Adds a model to the comparator.
 
         Args:
@@ -81,21 +90,33 @@
                 latency = time.time() - start_time
 
                 # Calculate the length of the response in tokens (assuming white space as token separator)
                 length_in_tokens = len(response[0].split())
 
                 # Store the question, model name, response, latency, and length in the results list
                 results.append(
-                    [question, model_name, response[0], latency, length_in_tokens]
+                    [
+                        question,
+                        model_name,
+                        response[0],
+                        latency,
+                        length_in_tokens,
+                    ]
                 )
 
         # Convert the results into a DataFrame
         self.inference_results = pd.DataFrame(
             results,
-            columns=["question", "model", "answer", "latency", "length_in_tokens"],
+            columns=[
+                "question",
+                "model",
+                "answer",
+                "latency",
+                "length_in_tokens",
+            ],
         )
 
         return self.inference_results
 
     def visualize(self):
         records = df_to_js_array(self.inference_results)
         return Barchart()(data=records)
```

### Comparing `pykoi-0.0.2/pykoi/component/chatbot_database_factory.py` & `pykoi-0.0.3/pykoi/component/chatbot_database_factory.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Chatbot Database Factory class."""
 from typing import Union
 
 from pykoi.component.constants import FeedbackType
-from pykoi.db.qa_database import QuestionAnswerDatabase
-from pykoi.db.ranking_database import RankingDatabase
+from pykoi.chat.db.qa_database import QuestionAnswerDatabase
+from pykoi.chat.db.ranking_database import RankingDatabase
 
 
 class ChatbotDatabaseFactory:
     """
     A factory class for creating chatbot databases.
     """
 
@@ -26,9 +26,9 @@
         if feedback == FeedbackType.VOTE:
             return QuestionAnswerDatabase()
         elif feedback == FeedbackType.RANK:
             return RankingDatabase()
         else:
             raise ValueError(
                 f"Invalid feedback name: {feedback}. "
-                f"Valid values are: 'question_answer', 'ranking'."
+                "Valid values are: 'question_answer', 'ranking'."
             )
```

### Comparing `pykoi-0.0.2/pykoi/db/abs_database.py` & `pykoi-0.0.3/pykoi/chat/db/abs_database.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,19 @@
 """abs database"""
 import abc
 import sqlite3
 import threading
 
-from typing import (
-    List,
-    Tuple
-)
+from typing import List, Tuple
 
 
 class AbsDatabase:
     """Base Database class"""
 
-    def __init__(self,
-                 db_file: str,
-                 debug: bool = False) -> None:
+    def __init__(self, db_file: str, debug: bool = False) -> None:
         """
         Initializes a new instance of the BaseDatabase class.
 
         Args:
             db_file (str): The path to the SQLite database file.
             debug (bool, optional): Whether to print debug messages. Defaults to False.
         """
@@ -72,34 +67,42 @@
     def insert(self, **kwargs) -> None:
         """
         Inserts into the database.
 
         Args:
             kwargs (dict): The key-value pairs to insert into the database.
         """
-        raise NotImplementedError("Insert method must be implemented by subclasses.")
+        raise NotImplementedError(
+            "Insert method must be implemented by subclasses."
+        )
 
     @abc.abstractmethod
     def update(self, **kwargs) -> None:
         """
         Updates the database.
 
         Args:
             kwargs (dict): The key-value pairs to update in the database.
         """
-        raise NotImplementedError("Update method must be implemented by subclasses.")
+        raise NotImplementedError(
+            "Update method must be implemented by subclasses."
+        )
 
     def retrieve_all(self) -> List[Tuple]:
         """
         Retrieves all pairs from the database.
         """
-        raise NotImplementedError("Retrieve method must be implemented by subclasses.")
+        raise NotImplementedError(
+            "Retrieve method must be implemented by subclasses."
+        )
 
     @abc.abstractmethod
     def print_table(self, rows: str) -> None:
         """
         Prints the table to the console.
 
         Args:
             rows (str): The rows to print.
         """
-        raise NotImplementedError("Print method must be implemented by subclasses.")
+        raise NotImplementedError(
+            "Print method must be implemented by subclasses."
+        )
```

### Comparing `pykoi-0.0.2/pykoi/db/comparator_database.py` & `pykoi-0.0.3/pykoi/chat/db/comparator_database.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 """Comparator Database"""
 import datetime
 import os
 
-from typing import (
-    List,
-    Tuple
-)
+from typing import List, Tuple
 
-from pykoi.db.abs_database import AbsDatabase
+from pykoi.chat.db.abs_database import AbsDatabase
 
 
 class ComparatorQuestionDatabase(AbsDatabase):
     """Comparator Question Database class"""
 
-    def __init__(self,
-                 db_file: str = os.path.join(os.getcwd(), "comparator.db"),
-                 debug: bool = False) -> None:
+    def __init__(
+        self,
+        db_file: str = os.path.join(os.getcwd(), "comparator.db"),
+        debug: bool = False,
+    ) -> None:
         """
         Initializes a new instance of the ComparatorQuestionDatabase class.
 
         Args:
             db_file (str): The path to the SQLite database file.
             debug (bool, optional): Whether to print debug messages. Defaults to False.
         """
@@ -62,15 +61,16 @@
         return cursor.lastrowid
 
     def update(self, **kwargs) -> None:
         """
         Updates the database.
         """
         raise NotImplementedError(
-            "ComparatorQuestionDatabase does not support update.")
+            "ComparatorQuestionDatabase does not support update."
+        )
 
     def retrieve_all(self) -> List[Tuple]:
         """
         Retrieves all pairs from the database.
 
         Returns:
             list: A list of tuples.
@@ -89,25 +89,25 @@
         Prints the contents of the table in a formatted manner.
 
         Args:
             rows (list): A list of tuples where each tuple represents a row in the table.
                         Each tuple contains five elements: ID, Question.
         """
         for row in rows:
-            print(
-                f"ID: {row[0]}, Question: {row[1]}, Timestamp: {row[2]}"
-            )
+            print(f"ID: {row[0]}, Question: {row[1]}, Timestamp: {row[2]}")
 
 
 class ComparatorDatabase(AbsDatabase):
     """ComparatorDatabase class."""
 
-    def __init__(self,
-                 db_file: str = os.path.join(os.getcwd(), "comparator.db"),
-                 debug: bool = False) -> None:
+    def __init__(
+        self,
+        db_file: str = os.path.join(os.getcwd(), "comparator.db"),
+        debug: bool = False,
+    ) -> None:
         query = """
         CREATE TABLE IF NOT EXISTS comparator (
             id INTEGER PRIMARY KEY AUTOINCREMENT,
             model TEXT NOT NULL,
             qid INTEGER NOT NULL,
             rank INTEGER NOT NULL,
             answer TEXT NOT NULL,
@@ -131,26 +131,33 @@
         """
         with self._lock:
             cursor = self.get_cursor()
             cursor.execute(check_query, (kwargs["model"], kwargs["qid"]))
             existing_row = cursor.fetchone()
 
             if existing_row is not None:
-                raise ValueError(f"Row with model={kwargs['model']} and qid={kwargs['qid']} already exists")
+                raise ValueError(
+                    f"Row with model={kwargs['model']} and"
+                    f" qid={kwargs['qid']} already exists"
+                )
 
             query = """
             INSERT INTO comparator (model, qid, rank, answer, timestamp)
             VALUES (?, ?, ?, ?, ?);
             """
-            cursor.execute(query,
-                           (kwargs["model"],
-                            kwargs["qid"],
-                            kwargs["rank"],
-                            kwargs["answer"],
-                            timestamp))
+            cursor.execute(
+                query,
+                (
+                    kwargs["model"],
+                    kwargs["qid"],
+                    kwargs["rank"],
+                    kwargs["answer"],
+                    timestamp,
+                ),
+            )
             self.get_connection().commit()
 
         if self._debug:
             rows = self.retrieve_all()
             print("Table contents after inserting table")
             self.print_table(rows)
 
@@ -165,18 +172,16 @@
         UPDATE comparator
         SET rank = ?
         WHERE qid = ? AND model = ?;
         """
         with self._lock:
             cursor = self.get_cursor()
             cursor.execute(
-                query,
-                (kwargs["rank"],
-                 kwargs["qid"],
-                 kwargs["model"]))
+                query, (kwargs["rank"], kwargs["qid"], kwargs["model"])
+            )
             self.get_connection().commit()
         if self._debug:
             rows = self.retrieve_all()
             print("Table contents after updating table")
             self.print_table(rows)
 
     def retrieve_all(self) -> List[Tuple]:
```

### Comparing `pykoi-0.0.2/pykoi/db/constants.py` & `pykoi-0.0.3/pykoi/chat/db/constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """database constants"""
 
 # question_answer table
-QA_CSV_HEADER_ID = 'ID'
-QA_CSV_HEADER_QUESTION = 'Question'
-QA_CSV_HEADER_ANSWER = 'Answer'
-QA_CSV_HEADER_VOTE_STATUS = 'Vote Status'
-QA_CSV_HEADER_TIMESTAMPS = 'Timestamp'
+QA_CSV_HEADER_ID = "ID"
+QA_CSV_HEADER_QUESTION = "Question"
+QA_CSV_HEADER_ANSWER = "Answer"
+QA_CSV_HEADER_VOTE_STATUS = "Vote Status"
+QA_CSV_HEADER_TIMESTAMPS = "Timestamp"
 QA_CSV_HEADER = (
     QA_CSV_HEADER_ID,
     QA_CSV_HEADER_QUESTION,
     QA_CSV_HEADER_ANSWER,
     QA_CSV_HEADER_VOTE_STATUS,
-    QA_CSV_HEADER_TIMESTAMPS
+    QA_CSV_HEADER_TIMESTAMPS,
 )
 
 # ranking table
 RANKING_CSV_HEADER_ID = "ID"
 RANKING_CSV_HEADER_QUESTION = "Question"
 RANKING_CSV_HEADER_UP_RANKING_ANSWER = "Up Ranking Answer"
 RANKING_CSV_HEADER_LOW_RANKING_ANSWER = "Low Ranking Answer"
```

### Comparing `pykoi-0.0.2/pykoi/db/qa_database.py` & `pykoi-0.0.3/pykoi/chat/db/qa_database.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,22 +3,24 @@
 import datetime
 import os
 import sqlite3
 import threading
 
 import pandas as pd
 
-from pykoi.db.constants import QA_CSV_HEADER
+from pykoi.chat.db.constants import QA_CSV_HEADER
 
 
 class QuestionAnswerDatabase:
     """Question Answer Database class"""
 
     def __init__(
-        self, db_file: str = os.path.join(os.getcwd(), "qd.db"), debug: bool = False
+        self,
+        db_file: str = os.path.join(os.getcwd(), "qd.db"),
+        debug: bool = False,
     ):
         """
         Initializes a new instance of the QuestionAnswerDatabase class.
 
         Args:
             db_file (str): The path to the SQLite database file.
             debug (bool, optional): Whether to print debug messages. Defaults to False.
```

### Comparing `pykoi-0.0.2/pykoi/db/ranking_database.py` & `pykoi-0.0.3/pykoi/chat/db/ranking_database.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import csv
 import os
 import sqlite3
 import threading
 
 import pandas as pd
 
-from pykoi.db.constants import RANKING_CSV_HEADER
+from pykoi.chat.db.constants import RANKING_CSV_HEADER
 
 
 class RankingDatabase:
     """Ranking Database class"""
 
     def __init__(
         self,
@@ -82,15 +82,17 @@
         """
         query = """
         INSERT INTO ranking (question, up_ranking_answer, low_ranking_answer)
         VALUES (?, ?, ?);
         """
         with self._lock:
             cursor = self.get_cursor()
-            cursor.execute(query, (question, up_ranking_answer, low_ranking_answer))
+            cursor.execute(
+                query, (question, up_ranking_answer, low_ranking_answer)
+            )
             self.get_connection().commit()
 
         if self._debug:
             rows = self.retrieve_all_question_answers()
             print("Table contents after inserting entry:")
             self.print_table(rows)
```

### Comparing `pykoi-0.0.2/pykoi/frontend/README.md` & `pykoi-0.0.3/pykoi/frontend/README.md`

 * *Files identical despite different names*

### Comparing `pykoi-0.0.2/pykoi/frontend/dist/assets/index-f75c1c12.css` & `pykoi-0.0.3/pykoi/frontend/dist/assets/index-f75c1c12.css`

 * *Files identical despite different names*

### Comparing `pykoi-0.0.2/pykoi/frontend/dist/assets/index-fc1a91e8.js` & `pykoi-0.0.3/pykoi/frontend/dist/assets/index-fc1a91e8.js`

 * *Files identical despite different names*

### Comparing `pykoi-0.0.2/pykoi/frontend/dist/vite.svg` & `pykoi-0.0.3/pykoi/frontend/dist/vite.svg`

 * *Files identical despite different names*

### Comparing `pykoi-0.0.2/pykoi/frontend/jsconfig.json` & `pykoi-0.0.3/pykoi/frontend/jsconfig.json`

 * *Files identical despite different names*

### Comparing `pykoi-0.0.2/pykoi/frontend/package.json` & `pykoi-0.0.3/pykoi/frontend/package.json`

 * *Files identical despite different names*

### Comparing `pykoi-0.0.2/pykoi/frontend/public/vite.svg` & `pykoi-0.0.3/pykoi/frontend/public/vite.svg`

 * *Files identical despite different names*

### Comparing `pykoi-0.0.2/pykoi/frontend/src/App.svelte` & `pykoi-0.0.3/pykoi/frontend/src/App.svelte`

 * *Files identical despite different names*

### Comparing `pykoi-0.0.2/pykoi/frontend/src/app.css` & `pykoi-0.0.3/pykoi/frontend/src/app.css`

 * *Files identical despite different names*

### Comparing `pykoi-0.0.2/pykoi/frontend/src/assets/svelte.svg` & `pykoi-0.0.3/pykoi/frontend/src/assets/svelte.svg`

 * *Files identical despite different names*

### Comparing `pykoi-0.0.2/pykoi/frontend/src/lib/Annotations/QuestionRating.svelte` & `pykoi-0.0.3/pykoi/frontend/src/lib/Annotations/QuestionRating.svelte`

 * *Files identical despite different names*

### Comparing `pykoi-0.0.2/pykoi/frontend/src/lib/Chatbots/Chatbot.svelte` & `pykoi-0.0.3/pykoi/frontend/src/lib/Chatbots/Chatbot.svelte`

 * *Files identical despite different names*

### Comparing `pykoi-0.0.2/pykoi/frontend/src/lib/Chatbots/ComparisonChat.svelte` & `pykoi-0.0.3/pykoi/frontend/src/lib/Chatbots/ComparisonChat.svelte`

 * *Files identical despite different names*

### Comparing `pykoi-0.0.2/pykoi/frontend/src/lib/Chatbots/RankChatComparison.svelte` & `pykoi-0.0.3/pykoi/frontend/src/lib/Chatbots/RankChatComparison.svelte`

 * *Files identical despite different names*

### Comparing `pykoi-0.0.2/pykoi/frontend/src/lib/Chatbots/RankChatbotOld.svelte` & `pykoi-0.0.3/pykoi/frontend/src/lib/Chatbots/RankChatbotOld.svelte`

 * *Files identical despite different names*

### Comparing `pykoi-0.0.2/pykoi/frontend/src/lib/Chatbots/RankedChatbot.svelte` & `pykoi-0.0.3/pykoi/frontend/src/lib/Chatbots/RankedChatbot.svelte`

 * *Files identical despite different names*

### Comparing `pykoi-0.0.2/pykoi/frontend/src/lib/Comparison/BumpChart.svelte` & `pykoi-0.0.3/pykoi/frontend/src/lib/Comparison/BumpChart.svelte`

 * *Files identical despite different names*

### Comparing `pykoi-0.0.2/pykoi/frontend/src/lib/Comparison/ComparisonChart.svelte` & `pykoi-0.0.3/pykoi/frontend/src/lib/Comparison/ComparisonChart.svelte`

 * *Files identical despite different names*

### Comparing `pykoi-0.0.2/pykoi/frontend/src/lib/Comparison/CumulativeScore.svelte` & `pykoi-0.0.3/pykoi/frontend/src/lib/Comparison/CumulativeScore.svelte`

 * *Files identical despite different names*

### Comparing `pykoi-0.0.2/pykoi/frontend/src/lib/Comparison/CumulativeStack.svelte` & `pykoi-0.0.3/pykoi/frontend/src/lib/Comparison/CumulativeStack.svelte`

 * *Files identical despite different names*

### Comparing `pykoi-0.0.2/pykoi/frontend/src/lib/Comparison/Heatmap.svelte` & `pykoi-0.0.3/pykoi/frontend/src/lib/Comparison/Heatmap.svelte`

 * *Files identical despite different names*

### Comparing `pykoi-0.0.2/pykoi/frontend/src/lib/Comparison/HorizontalBar.svelte` & `pykoi-0.0.3/pykoi/frontend/src/lib/Comparison/HorizontalBar.svelte`

 * *Files identical despite different names*

### Comparing `pykoi-0.0.2/pykoi/frontend/src/lib/Comparison/Table.svelte` & `pykoi-0.0.3/pykoi/frontend/src/lib/Comparison/Table.svelte`

 * *Files identical despite different names*

### Comparing `pykoi-0.0.2/pykoi/frontend/src/lib/Comparison/data.js` & `pykoi-0.0.3/pykoi/frontend/src/lib/Comparison/data.js`

 * *Files identical despite different names*

### Comparing `pykoi-0.0.2/pykoi/frontend/src/lib/Comparison/store.js` & `pykoi-0.0.3/pykoi/frontend/src/lib/Comparison/store.js`

 * *Files identical despite different names*

### Comparing `pykoi-0.0.2/pykoi/frontend/src/lib/Dashboards/DashboardFeedback/ColumnChart.svelte` & `pykoi-0.0.3/pykoi/frontend/src/lib/Dashboards/DashboardFeedback/ColumnChart.svelte`

 * *Files identical despite different names*

### Comparing `pykoi-0.0.2/pykoi/frontend/src/lib/Dashboards/DashboardFeedback/HistogramAnswer.svelte` & `pykoi-0.0.3/pykoi/frontend/src/lib/Dashboards/DashboardFeedback/HistogramAnswer.svelte`

 * *Files identical despite different names*

### Comparing `pykoi-0.0.2/pykoi/frontend/src/lib/Dashboards/DashboardFeedback/HistogramQuestion.svelte` & `pykoi-0.0.3/pykoi/frontend/src/lib/Dashboards/DashboardFeedback/HistogramQuestion.svelte`

 * *Files identical despite different names*

### Comparing `pykoi-0.0.2/pykoi/frontend/src/lib/Dashboards/DashboardFeedback/HorizontalStackedBar.svelte` & `pykoi-0.0.3/pykoi/frontend/src/lib/Dashboards/DashboardFeedback/HorizontalStackedBar.svelte`

 * *Files identical despite different names*

### Comparing `pykoi-0.0.2/pykoi/frontend/src/lib/Dashboards/DashboardFeedback/MetricCardAbsolute.svelte` & `pykoi-0.0.3/pykoi/frontend/src/lib/Dashboards/DashboardFeedback/MetricCardAbsolute.svelte`

 * *Files identical despite different names*

### Comparing `pykoi-0.0.2/pykoi/frontend/src/lib/Dashboards/DashboardFeedback/MetricCardPercentage.svelte` & `pykoi-0.0.3/pykoi/frontend/src/lib/Dashboards/DashboardFeedback/MetricCardPercentage.svelte`

 * *Files identical despite different names*

### Comparing `pykoi-0.0.2/pykoi/frontend/src/lib/Dashboards/DashboardFeedback/QACard.svelte` & `pykoi-0.0.3/pykoi/frontend/src/lib/Dashboards/DashboardFeedback/QACard.svelte`

 * *Files identical despite different names*

### Comparing `pykoi-0.0.2/pykoi/frontend/src/lib/Dashboards/DashboardFeedback/QATable.svelte` & `pykoi-0.0.3/pykoi/frontend/src/lib/Dashboards/DashboardFeedback/QATable.svelte`

 * *Files identical despite different names*

### Comparing `pykoi-0.0.2/pykoi/frontend/src/lib/Dashboards/Feedback.svelte` & `pykoi-0.0.3/pykoi/frontend/src/lib/Dashboards/Feedback.svelte`

 * *Files identical despite different names*

### Comparing `pykoi-0.0.2/pykoi/frontend/src/lib/Evaluation/Bar.svelte` & `pykoi-0.0.3/pykoi/frontend/src/lib/Evaluation/Bar.svelte`

 * *Files identical despite different names*

### Comparing `pykoi-0.0.2/pykoi/frontend/src/lib/Evaluation/BumpChart.svelte` & `pykoi-0.0.3/pykoi/frontend/src/lib/Evaluation/BumpChart.svelte`

 * *Files identical despite different names*

### Comparing `pykoi-0.0.2/pykoi/frontend/src/lib/Evaluation/ComparisonChart.svelte` & `pykoi-0.0.3/pykoi/frontend/src/lib/Evaluation/ComparisonChart.svelte`

 * *Files identical despite different names*

### Comparing `pykoi-0.0.2/pykoi/frontend/src/lib/Evaluation/EvalLineChart.svelte` & `pykoi-0.0.3/pykoi/frontend/src/lib/Evaluation/EvalLineChart.svelte`

 * *Files identical despite different names*

### Comparing `pykoi-0.0.2/pykoi/frontend/src/lib/Evaluation/LineChart.svelte` & `pykoi-0.0.3/pykoi/frontend/src/lib/Evaluation/LineChart.svelte`

 * *Files identical despite different names*

### Comparing `pykoi-0.0.2/pykoi/frontend/src/lib/Evaluation/RLHFEvaluation.svelte` & `pykoi-0.0.3/pykoi/frontend/src/lib/Evaluation/RLHFEvaluation.svelte`

 * *Files identical despite different names*

### Comparing `pykoi-0.0.2/pykoi/frontend/src/lib/Evaluation/Table.svelte` & `pykoi-0.0.3/pykoi/frontend/src/lib/Evaluation/Table.svelte`

 * *Files identical despite different names*

### Comparing `pykoi-0.0.2/pykoi/frontend/src/lib/Evaluation/data.js` & `pykoi-0.0.3/pykoi/frontend/src/lib/Evaluation/data.js`

 * *Files identical despite different names*

### Comparing `pykoi-0.0.2/pykoi/frontend/src/lib/Evaluation/store.js` & `pykoi-0.0.3/pykoi/frontend/src/lib/Evaluation/store.js`

 * *Files identical despite different names*

### Comparing `pykoi-0.0.2/pykoi/frontend/src/normalize.css` & `pykoi-0.0.3/pykoi/frontend/src/normalize.css`

 * *Files identical despite different names*

### Comparing `pykoi-0.0.2/pykoi/frontend/src/store.js` & `pykoi-0.0.3/pykoi/frontend/src/store.js`

 * *Files identical despite different names*

### Comparing `pykoi-0.0.2/pykoi/frontend/src/styles.css` & `pykoi-0.0.3/pykoi/frontend/src/styles.css`

 * *Files identical despite different names*

### Comparing `pykoi-0.0.2/pykoi/frontend/src/utils.js` & `pykoi-0.0.3/pykoi/frontend/src/utils.js`

 * *Files identical despite different names*

### Comparing `pykoi-0.0.2/pykoi/interactives/barchart.py` & `pykoi-0.0.3/pykoi/interactives/barchart.py`

 * *Files identical despite different names*

### Comparing `pykoi-0.0.2/pykoi/llm/abs_llm.py` & `pykoi-0.0.3/pykoi/chat/llm/abs_llm.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,19 +21,23 @@
         Args:
             message (str): The input message used to predict the next word.
             num_of_response (int): How many completions to generate for each prompt.
 
         Raises:
             NotImplementedError: This method must be implemented by subclasses.
         """
-        raise NotImplementedError("This method must be implemented by subclasses.")
+        raise NotImplementedError(
+            "This method must be implemented by subclasses."
+        )
 
     @property
     def name(self):
         """Return the name of the model.
 
         This method must be implemented by any subclass of `AbsLlm`.
 
         Raises:
             NotImplementedError: This method must be implemented by subclasses.
         """
-        raise NotImplementedError("This method must be implemented by subclasses.")
+        raise NotImplementedError(
+            "This method must be implemented by subclasses."
+        )
```

### Comparing `pykoi-0.0.2/pykoi/llm/huggingface.py` & `pykoi-0.0.3/pykoi/chat/llm/huggingface.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 """Huggingface model for Language Model (LLM)."""
 from transformers import AutoModelForCausalLM, AutoTokenizer
 
-from pykoi.llm.abs_llm import AbsLlm
+from pykoi.chat.llm.abs_llm import AbsLlm
 
 
 class HuggingfaceModel(AbsLlm):
     """
     This class is a wrapper for the Huggingface model for Language Model (LLM) Chain.
     It inherits from the abstract base class AbsLlm.
     """
+
     model_source = "huggingface"
 
     def __init__(
         self,
         pretrained_model_name_or_path: str,
+        name: str = None,
         trust_remote_code: bool = True,
         load_in_8bit: bool = True,
         max_length: int = 100,
         device_map: str = "auto",
     ):
         """
         Initialize the Huggingface model.
 
         Args:
             pretrained_model_name_or_path (str): The name or path of the pretrained model.
+            name (str): The name of the model
             trust_remote_code (bool): Whether to trust the remote code. Default is True.
             load_in_8bit (bool): Whether to load the model in 8-bit. Default is True.
             max_length (int): The maximum length for the model. Default is 100.
             device_map (str): The device map for the model. Default is "auto".
         """
         # running on cpu can be slow!!!
         print("[HuggingfaceModel] loading model...")
@@ -42,56 +45,69 @@
             pretrained_model_name_or_path,
             trust_remote_code=trust_remote_code,
             load_in_8bit=load_in_8bit,
             device_map=device_map,
         )
         self._max_length = max_length
         self._pretrained_model_name_or_path = pretrained_model_name_or_path
+        self._name = name
         super().__init__()
 
     @property
     def name(self):
-        return "_".join([
-            str(HuggingfaceModel.model_source),
-            str(self._pretrained_model_name_or_path),
-            str(self._max_length)
-        ])
+        if self._name:
+            return self._name
+        return "_".join(
+            [
+                str(HuggingfaceModel.model_source),
+                str(self._pretrained_model_name_or_path),
+                str(self._max_length),
+            ]
+        )
 
     def predict(self, message: str, num_of_response: int = 1):
         """
         Predict the next word based on the input message.
 
         Args:
             message (str): The input message for the model.
             num_of_response (int): The number of response to generate. Default is 1.
 
         Returns:
             List[str]: List of response.
         """
-        ## TODO: need to refractor and include all the derivatives of dolly family
+        # TODO: need to refractor and include all the derivatives of dolly family
         if "dolly" in self._pretrained_model_name_or_path:
-            from pykoi.llm.instruct_pipeline import InstructionTextGenerationPipeline
-            generate_text = InstructionTextGenerationPipeline(model=self._model, 
-                                                              tokenizer=self._tokenizer)
+            from pykoi.chat.llm.instruct_pipeline import (
+                InstructionTextGenerationPipeline,
+            )
+
+            generate_text = InstructionTextGenerationPipeline(
+                model=self._model, tokenizer=self._tokenizer
+            )
             res = generate_text(message)
             response = [res[0]["generated_text"]]
-        ## all other models except dolly family
+        # all other models except dolly family
         else:
             print("[HuggingfaceModel] encode...")
             input_ids = self._tokenizer.encode(message, return_tensors="pt")
             input_ids = input_ids.to("cuda")
             print("[HuggingfaceModel] generate...")
             output_ids = self._model.generate(
                 input_ids,
                 max_length=self._max_length,
                 num_return_sequences=num_of_response,
                 do_sample=True,
                 temperature=0.3,
             )
             print("[HuggingfaceModel] decode...")
             response = [
-                self._tokenizer.decode(ids, skip_special_tokens=True) for ids in output_ids
+                self._tokenizer.decode(ids, skip_special_tokens=True)
+                for ids in output_ids
             ]
 
-            response = [resp.split("\n")[1] for resp in response if "\n" in resp]
+            response = [
+                "\n".join(resp.split("\n")[1:]) 
+                for resp in response if "\n" in resp
+            ]
 
         return response
```

### Comparing `pykoi-0.0.2/pykoi/llm/instruct_pipeline.py` & `pykoi-0.0.3/pykoi/chat/llm/instruct_pipeline.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 
 logger = logging.getLogger(__name__)
 
 INSTRUCTION_KEY = "### Instruction:"
 RESPONSE_KEY = "### Response:"
 END_KEY = "### End"
 INTRO_BLURB = (
-    "Below is an instruction that describes a task. Write a response that appropriately completes the request."
+    "Below is an instruction that describes a task. Write a response that"
+    " appropriately completes the request."
 )
 
 # This is the prompt that is used for generating responses using an already trained model.  It ends with the response
 # key, where the job of the model is to provide the completion that follows it (i.e. the response itself).
 PROMPT_FOR_GENERATION_FORMAT = """{intro}
 
 {instruction_key}
@@ -51,71 +52,94 @@
         RuntimeError: if more than one ID was generated
 
     Returns:
         int: the token ID for the given key
     """
     token_ids = tokenizer.encode(key)
     if len(token_ids) > 1:
-        raise ValueError(f"Expected only a single token for '{key}' but found {token_ids}")
+        raise ValueError(
+            f"Expected only a single token for '{key}' but found {token_ids}"
+        )
     return token_ids[0]
 
 
 class InstructionTextGenerationPipeline(Pipeline):
     def __init__(
-        self, *args, do_sample: bool = True, max_new_tokens: int = 256, top_p: float = 0.92, top_k: int = 0, **kwargs
+        self,
+        *args,
+        do_sample: bool = True,
+        max_new_tokens: int = 256,
+        top_p: float = 0.92,
+        top_k: int = 0,
+        **kwargs,
     ):
         """Initialize the pipeline
 
         Args:
             do_sample (bool, optional): Whether or not to use sampling. Defaults to True.
             max_new_tokens (int, optional): Max new tokens after the prompt to generate. Defaults to 128.
             top_p (float, optional): If set to float < 1, only the smallest set of most probable tokens with
                 probabilities that add up to top_p or higher are kept for generation. Defaults to 0.92.
             top_k (int, optional): The number of highest probability vocabulary tokens to keep for top-k-filtering.
                 Defaults to 0.
         """
-        super().__init__(*args, do_sample=do_sample, max_new_tokens=max_new_tokens, top_p=top_p, top_k=top_k,
-                         **kwargs)
+        super().__init__(
+            *args,
+            do_sample=do_sample,
+            max_new_tokens=max_new_tokens,
+            top_p=top_p,
+            top_k=top_k,
+            **kwargs,
+        )
 
-    def _sanitize_parameters(self,
-                             return_full_text: bool = None,
-                             **generate_kwargs):
+    def _sanitize_parameters(
+        self, return_full_text: bool = None, **generate_kwargs
+    ):
         preprocess_params = {}
 
         # newer versions of the tokenizer configure the response key as a special token.  newer versions still may
         # append a newline to yield a single token.  find whatever token is configured for the response key.
         tokenizer_response_key = next(
-            (token for token in self.tokenizer.additional_special_tokens if token.startswith(RESPONSE_KEY)), None
+            (
+                token
+                for token in self.tokenizer.additional_special_tokens
+                if token.startswith(RESPONSE_KEY)
+            ),
+            None,
         )
 
         response_key_token_id = None
         end_key_token_id = None
         if tokenizer_response_key:
             try:
-                response_key_token_id = get_special_token_id(self.tokenizer, tokenizer_response_key)
+                response_key_token_id = get_special_token_id(
+                    self.tokenizer, tokenizer_response_key
+                )
                 end_key_token_id = get_special_token_id(self.tokenizer, END_KEY)
 
                 # Ensure generation stops once it generates "### End"
                 generate_kwargs["eos_token_id"] = end_key_token_id
             except ValueError:
                 pass
 
         forward_params = generate_kwargs
         postprocess_params = {
             "response_key_token_id": response_key_token_id,
-            "end_key_token_id": end_key_token_id
+            "end_key_token_id": end_key_token_id,
         }
 
         if return_full_text is not None:
             postprocess_params["return_full_text"] = return_full_text
 
         return preprocess_params, forward_params, postprocess_params
 
     def preprocess(self, instruction_text, **generate_kwargs):
-        prompt_text = PROMPT_FOR_GENERATION_FORMAT.format(instruction=instruction_text)
+        prompt_text = PROMPT_FOR_GENERATION_FORMAT.format(
+            instruction=instruction_text
+        )
         inputs = self.tokenizer(
             prompt_text,
             return_tensors="pt",
         )
         inputs["prompt_text"] = prompt_text
         inputs["instruction_text"] = instruction_text
         return inputs
@@ -129,86 +153,116 @@
             attention_mask = None
             in_b = 1
         else:
             in_b = input_ids.shape[0]
 
         generated_sequence = self.model.generate(
             input_ids=input_ids.to(self.model.device),
-            attention_mask=attention_mask.to(self.model.device) if attention_mask is not None else None,
+            attention_mask=attention_mask.to(self.model.device)
+            if attention_mask is not None
+            else None,
             pad_token_id=self.tokenizer.pad_token_id,
             **generate_kwargs,
         )
 
         out_b = generated_sequence.shape[0]
         if self.framework == "pt":
-            generated_sequence = generated_sequence.reshape(in_b, out_b // in_b, *generated_sequence.shape[1:])
+            generated_sequence = generated_sequence.reshape(
+                in_b, out_b // in_b, *generated_sequence.shape[1:]
+            )
         elif self.framework == "tf":
-            generated_sequence = tf.reshape(generated_sequence, (in_b, out_b // in_b, *generated_sequence.shape[1:]))
+            generated_sequence = tf.reshape(
+                generated_sequence,
+                (in_b, out_b // in_b, *generated_sequence.shape[1:]),
+            )
 
         instruction_text = model_inputs.pop("instruction_text")
-        return {"generated_sequence": generated_sequence, "input_ids": input_ids, "instruction_text": instruction_text}
-
-    def postprocess(self, model_outputs, response_key_token_id, end_key_token_id, return_full_text: bool = False):
+        return {
+            "generated_sequence": generated_sequence,
+            "input_ids": input_ids,
+            "instruction_text": instruction_text,
+        }
 
+    def postprocess(
+        self,
+        model_outputs,
+        response_key_token_id,
+        end_key_token_id,
+        return_full_text: bool = False,
+    ):
         generated_sequence = model_outputs["generated_sequence"][0]
         instruction_text = model_outputs["instruction_text"]
 
-        generated_sequence: List[List[int]] = generated_sequence.numpy().tolist()
+        generated_sequence: List[
+            List[int]
+        ] = generated_sequence.numpy().tolist()
         records = []
         for sequence in generated_sequence:
-
             # The response will be set to this variable if we can identify it.
             decoded = None
 
             # If we have token IDs for the response and end, then we can find the tokens and only decode between them.
             if response_key_token_id and end_key_token_id:
                 # Find where "### Response:" is first found in the generated tokens.  Considering this is part of the
                 # prompt, we should definitely find it.  We will return the tokens found after this token.
                 try:
                     response_pos = sequence.index(response_key_token_id)
                 except ValueError:
-                    logger.warn(f"Could not find response key {response_key_token_id} in: {sequence}")
+                    logger.warn(
+                        "Could not find response key"
+                        f" {response_key_token_id} in: {sequence}"
+                    )
                     response_pos = None
 
                 if response_pos:
                     # Next find where "### End" is located.  The model has been trained to end its responses with this
                     # sequence (or actually, the token ID it maps to, since it is a special token).  We may not find
                     # this token, as the response could be truncated.  If we don't find it then just return everything
                     # to the end.  Note that even though we set eos_token_id, we still see the this token at the end.
                     try:
                         end_pos = sequence.index(end_key_token_id)
                     except ValueError:
                         end_pos = None
 
-                    decoded = self.tokenizer.decode(sequence[response_pos + 1 : end_pos]).strip()
+                    decoded = self.tokenizer.decode(
+                        sequence[response_pos + 1 : end_pos]
+                    ).strip()
 
             if not decoded:
                 # Otherwise we'll decode everything and use a regex to find the response and end.
 
                 fully_decoded = self.tokenizer.decode(sequence)
 
                 # The response appears after "### Response:".  The model has been trained to append "### End" at the
                 # end.
-                m = re.search(r"#+\s*Response:\s*(.+?)#+\s*End", fully_decoded, flags=re.DOTALL)
+                m = re.search(
+                    r"#+\s*Response:\s*(.+?)#+\s*End",
+                    fully_decoded,
+                    flags=re.DOTALL,
+                )
 
                 if m:
                     decoded = m.group(1).strip()
                 else:
                     # The model might not generate the "### End" sequence before reaching the max tokens.  In this case,
                     # return everything after "### Response:".
-                    m = re.search(r"#+\s*Response:\s*(.+)", fully_decoded, flags=re.DOTALL)
+                    m = re.search(
+                        r"#+\s*Response:\s*(.+)", fully_decoded, flags=re.DOTALL
+                    )
                     if m:
                         decoded = m.group(1).strip()
                     else:
-                        logger.warn(f"Failed to find response in:\n{fully_decoded}")
+                        logger.warn(
+                            f"Failed to find response in:\n{fully_decoded}"
+                        )
 
             # If the full text is requested, then append the decoded text to the original instruction.
             # This technically isn't the full text, as we format the instruction in the prompt the model has been
             # trained on, but to the client it will appear to be the full text.
             if return_full_text:
                 decoded = f"{instruction_text}\n{decoded}"
 
             rec = {"generated_text": decoded}
 
             records.append(rec)
 
-        return records
+        return records
```

### Comparing `pykoi-0.0.2/pykoi/llm/model_factory.py` & `pykoi-0.0.3/pykoi/chat/llm/model_factory.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 """This module defines a factory for creating language models."""
 
 from typing import Union
 
-from pykoi.llm.abs_llm import AbsLlm
-from pykoi.llm.constants import ModelSource
+from pykoi.chat.llm.abs_llm import AbsLlm
+from pykoi.chat.llm.constants import ModelSource
 
 
 class ModelFactory:
     """
     A factory class for creating language models.
 
     This class provides a static method `create_model` which creates a
     language model instance based on the given name.
-
-    Methods:
-        create_model(model_source: Union[str, ModelSource], **kwargs) -> AbsLlm:
-            Creates a language model based on the given name.
     """
 
     @staticmethod
     def create_model(model_source: Union[str, ModelSource], **kwargs) -> AbsLlm:
         """
         Create a language model based on the given name.
 
@@ -37,22 +33,24 @@
 
         Raises:
             ValueError: If the given model name is not valid.
         """
         try:
             model_source = ModelSource(model_source)
             if model_source == ModelSource.OPENAI:
-                from pykoi.llm.openai import OpenAIModel
+                from pykoi.chat.llm.openai import OpenAIModel
 
                 return OpenAIModel(**kwargs)
             elif model_source == ModelSource.HUGGINGFACE:
-                from pykoi.llm.huggingface import HuggingfaceModel
+                from pykoi.chat.llm.huggingface import HuggingfaceModel
 
                 return HuggingfaceModel(**kwargs)
             elif model_source == ModelSource.PEFT_HUGGINGFACE:
-                from pykoi.llm.peft_huggingface import PeftHuggingfacemodel
+                from pykoi.chat.llm.peft_huggingface import PeftHuggingfacemodel
 
                 return PeftHuggingfacemodel(**kwargs)
             else:
-                raise ValueError(f"[llm_factory]: Unknown model source " f"{model_source}")
+                raise ValueError(
+                    f"[llm_factory]: Unknown model source {model_source}"
+                )
         except ValueError as ex:
             raise ValueError("[llm_factory]: initialize model failure") from ex
```

### Comparing `pykoi-0.0.2/pykoi/llm/openai.py` & `pykoi-0.0.3/pykoi/chat/llm/openai.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """This module provides a wrapper for the OpenAI model."""
 import openai
 
-from pykoi.llm.abs_llm import AbsLlm
+from pykoi.chat.llm.abs_llm import AbsLlm
 
 
 class OpenAIModel(AbsLlm):
     """
     A class that wraps the OpenAI model for use in the LLMChain.
 
     Attributes:
@@ -13,45 +13,54 @@
         _max_tokens (int): The maximum number of tokens to generate.
         _temperature (float): The temperature to use for the OpenAI model.
 
     Methods:
         __init__(self, api_key: str, engine: str, max_tokens: int, temperature: float): Initializes the OpenAI model.
         predict(self, message: str): Predicts the next word based on the given message.
     """
+
     model_source = "openai"
 
     def __init__(
         self,
         api_key: str,
+        name: str = None,
         engine: str = "davinci",
         max_tokens: int = 100,
         temperature: float = 0.5,
     ):
         """
         Initializes the OpenAI model with the given parameters.
 
         Args:
             api_key (str): The API key for the OpenAI model.
+            name (str): The name of the model. Defaults to None.
             engine (str, optional): The engine to use for the OpenAI model. Defaults to "davinci".
             max_tokens (int, optional): The maximum number of tokens to generate. Defaults to 100.
             temperature (float, optional): The temperature to use for the OpenAI model. Defaults to 0.5.
         """
         openai.api_key = api_key
         self._engine = engine
         self._max_tokens = max_tokens
         self._temperature = temperature
+        self._name = name
         super().__init__()
 
     @property
     def name(self):
-        return "_".join([
-            str(OpenAIModel.model_source),
-            str(self._engine),
-            str(self._max_tokens),
-            str(self._temperature)])
+        if self._name:
+            return self._name
+        return "_".join(
+            [
+                str(OpenAIModel.model_source),
+                str(self._engine),
+                str(self._max_tokens),
+                str(self._temperature),
+            ]
+        )
 
     def predict(self, message: str, num_of_response: int = 1):
         """
         Predicts the next word based on the given message.
 
         Args:
             message (str): The message to base the prediction on.
```

### Comparing `pykoi-0.0.2/pykoi/llm/peft_huggingface.py` & `pykoi-0.0.3/pykoi/chat/llm/peft_huggingface.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,42 +1,45 @@
 """Huggingface PEFT model for Language Model (LLM)."""
 import torch
 
 from transformers import AutoModelForCausalLM, AutoTokenizer
 from peft import PeftModel
 
-from pykoi.llm.abs_llm import AbsLlm
+from pykoi.chat.llm.abs_llm import AbsLlm
 
 
 class PeftHuggingfacemodel(AbsLlm):
     """
     This class is a wrapper for the Huggingface PEFT model for Language Model (LLM).
 
     Attributes:
         _model (PeftModel): The PEFT model.
         _tokenizer (AutoTokenizer): The tokenizer for the model.
         _max_length (int): The maximum length of the generated text.
     """
+
     model_source = "peft_huggingface"
 
     def __init__(
         self,
         base_model_path: str,
         lora_model_path: str,
+        name: str = None,
         trust_remote_code: bool = True,
         load_in_8bit: bool = True,
         max_length: int = 100,
         device_map: str = "auto",
     ):
         """
         The constructor for PeftHuggingfacemodel class.
 
         Args:
             base_model_path (str): The path to the base model.
             lora_model_path (str): The path to the lora model.
+            name (str): The name of the model. Defaults to None.
             trust_remote_code (bool, optional): Whether to trust remote code. Defaults to True.
             load_in_8bit (bool, optional): Whether to load in 8bit. Defaults to True.
             max_length (int, optional): The maximum length of the generated text. Defaults to 100.
             device_map (str, optional): The device map. Defaults to "auto".
         """
         print("[HuggingfaceModel] loading base model...")
         base_model = AutoModelForCausalLM.from_pretrained(
@@ -46,39 +49,44 @@
             trust_remote_code=trust_remote_code,
             load_in_8bit=load_in_8bit,
             device_map=device_map,
         )
 
         print("[HuggingfaceModel] loading perf model...")
         self._model = PeftModel.from_pretrained(
-            model=base_model,
-            model_id=lora_model_path)
+            model=base_model, model_id=lora_model_path
+        )
 
         print("[HuggingfaceModel] loading tokenizer...")
         self._tokenizer = AutoTokenizer.from_pretrained(
             pretrained_model_name_or_path=base_model_path,
             trust_remote_code=trust_remote_code,
             load_in_8bit=load_in_8bit,
             device_map=device_map,
         )
         self._max_length = max_length
         self._base_model_path = base_model_path
         self._lora_model_path = lora_model_path
+        self._name = name
         self._model.to("cuda")
         self._model.eval()
         super().__init__()
 
     @property
     def name(self):
-        return "_".join([
-            str(PeftHuggingfacemodel.model_source),
-            str(self._base_model_path),
-            str(self._lora_model_path),
-            str(self._max_length)
-        ])
+        if self._name:
+            return self._name
+        return "_".join(
+            [
+                str(PeftHuggingfacemodel.model_source),
+                str(self._base_model_path),
+                str(self._lora_model_path),
+                str(self._max_length),
+            ]
+        )
 
     def predict(self, message: str, num_of_response: int = 1):
         """
         Predict the next word based on the input message.
 
         Args:
             message (str): The input message for the model.
@@ -96,14 +104,15 @@
             max_length=self._max_length,
             num_return_sequences=num_of_response,
             do_sample=True,
             temperature=0.3,
         )
         print("[HuggingfaceModel] decode...")
         response = [
-            self._tokenizer.decode(ids, skip_special_tokens=True) for ids in output_ids
+            self._tokenizer.decode(ids, skip_special_tokens=True)
+            for ids in output_ids
         ]
         print("response: ", response)
 
         response = [resp.split("\n")[1] for resp in response if "\n" in resp]
 
         return response
```

### Comparing `pykoi-0.0.2/pykoi/rlhf/config.py` & `pykoi-0.0.3/pykoi/rlhf/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 """RLHF configuration file."""
 
 from dataclasses import dataclass, field
-from typing import (
-    List,
-    Optional
-)
+from typing import List, Optional
 
 from accelerate import Accelerator
 from peft import LoraConfig, TaskType
 
 
 @dataclass
 class RLHFConfig:
@@ -17,30 +14,45 @@
     The parameters are divided into three steps:
         - Step 1: SFT (Supervised Fine-Tuning) parameters
         - Step 2: Reward Modeling parameters
         - Step 3: Reinforcement Learning parameters
     """
 
     base_model_path: str = field(
-        default="meta-llama/Llama-2-7b-hf",
-        metadata={"help": "Huggingface model name or a local path to the base model."},
+        default="elinas/llama-7b-hf-transformers-4.29",
+        metadata={
+            "help": "Huggingface model name or a local path to the base model."
+        },
     )
     dataset_type: Optional[str] = field(
         default="local_db",
-        metadata={"help": "'local_db':load from your local database `qd.db` path; \
-                  'local_csv':load from a local csv path; 'huggingface': load a huggingface dataset."})
+        metadata={
+            "help": (
+                "'local_db':load from your local database `qd.db` path;        "
+                "           'local_csv':load from a local csv path;"
+                " 'huggingface': load a huggingface dataset."
+            )
+        },
+    )
     dataset_name: Optional[str] = field(
         default="qd.db",
-        metadata={"help": "A local path to a csv dataset or a database; Or a Huggingface "
-                  "dataset name (e.g. 'lvwerra/stack-exchange-paired')."})
+        metadata={
+            "help": (
+                "A local path to a csv dataset or a database; Or a Huggingface "
+                "dataset name (e.g. 'lvwerra/stack-exchange-paired')."
+            )
+        },
+    )
     train_test_split_ratio: Optional[float] = field(
         default=0.1,
         metadata={
-            "help": "The ratio represents the proportion of the test dataset to \
-                  include in the train and test split."
+            "help": (
+                "The ratio represents the proportion of the test dataset to    "
+                "               include in the train and test split."
+            )
         },
     )
     streaming: Optional[bool] = field(
         default=False, metadata={"help": "Whether to use streaming."}
     )
     shuffle_buffer: Optional[int] = field(
         default=5000, metadata={"help": "Size of the shuffle buffer."}
@@ -58,75 +70,88 @@
     per_device_train_batch_size: Optional[int] = field(
         default=2, metadata={"help": "Batch size per device for training."}
     )
     per_device_eval_batch_size: Optional[int] = field(
         default=8, metadata={"help": "Batch size per device for evaluation."}
     )
     gradient_accumulation_steps: Optional[int] = field(
-        default=4, metadata={"help": "Number of steps for gradient accumulation."}
+        default=4,
+        metadata={"help": "Number of steps for gradient accumulation."},
     )
     eos_token_id: Optional[int] = field(
         default=49152, metadata={"help": "End-of-sequence token ID."}
     )
     learning_rate: Optional[float] = field(
         default=1e-5, metadata={"help": "Learning rate."}
     )
     weight_decay: Optional[float] = field(
         default=0.01, metadata={"help": "Weight decay."}
     )
     local_rank: Optional[int] = field(
         default=-1, metadata={"help": "Used for multi-gpu."}
     )
-    fp16: Optional[bool] = field(default=True, metadata={"help": "Enable FP16."})
-    bf16: Optional[bool] = field(default=False, metadata={"help": "Enable BF16."})
+    fp16: Optional[bool] = field(
+        default=True, metadata={"help": "Enable FP16."}
+    )
+    bf16: Optional[bool] = field(
+        default=False, metadata={"help": "Enable BF16."}
+    )
     load_in_8bit: Optional[bool] = field(
         default=True,
         metadata={"help": "Whether load the model weights in 8-bit or not."},
     )
     device_map: Optional[dict] = field(
         default_factory=lambda: {"": Accelerator().process_index},
         metadata={
-            "help": "specify the mapping of model layers to specific devices, such as different GPUs \
-                  in a multi-GPU setup. This can be helpful for distributing the computational load of a \
-                  large model across multiple GPUs."
+            "help": (
+                "specify the mapping of model layers to specific devices, such"
+                " as different GPUs                   in a multi-GPU setup."
+                " This can be helpful for distributing the computational load"
+                " of a                   large model across multiple GPUs."
+            )
         },
     )
     gradient_checkpointing: Optional[bool] = field(
         default=False, metadata={"help": "Enable gradient checkpointing."}
     )
     seed: Optional[int] = field(default=0, metadata={"help": "Random seed."})
     num_workers: Optional[int] = field(
         default=None, metadata={"help": "Number of workers."}
     )
     output_dir: Optional[str] = field(
         default="./rlhf_checkpoints",
         metadata={"help": "Output directory for all model weights."},
     )
-    log_freq: Optional[int] = field(default=1, metadata={"help": "Logging frequency."})
+    log_freq: Optional[int] = field(
+        default=1, metadata={"help": "Logging frequency."}
+    )
     eval_freq: Optional[int] = field(
         default=1000, metadata={"help": "Evaluation frequency."}
     )
     save_freq: Optional[int] = field(
         default=1000, metadata={"help": "Model saving frequency."}
     )
     push_to_hub: Optional[bool] = field(
-        default=False, metadata={"help": "Whether push to Huggingface Hub or not."}
+        default=False,
+        metadata={"help": "Whether push to Huggingface Hub or not."},
     )
 
     ## Step 1 SFT parameters
     max_steps: Optional[int] = field(
         default=5, metadata={"help": "Maximum number of training steps."}
     )
     dataset_subset_sft: Optional[str] = field(
         default="data/finetune",
         metadata={"help": "Subset folder of the dataset to use."},
     )
     dataset_subset_sft_train: Optional[int] = field(
         default=10000,
-        metadata={"help": "The size of the subset of the training data to use."},
+        metadata={
+            "help": "The size of the subset of the training data to use."
+        },
     )
     split: Optional[str] = field(
         default="train", metadata={"help": "Dataset split to use."}
     )
     question_title: Optional[str] = field(
         default="Question",
         metadata={"help": "the column name of questions from the database."},
@@ -137,28 +162,26 @@
     )
     size_valid_set: Optional[int] = field(
         default=4000, metadata={"help": "Size of the validation/eval set."}
     )
     sft_lora_path: Optional[str] = field(
         default="step1_supervised_finetuning_lora_final/",
         metadata={
-            "help": "Output directory for step 1 supervised finetuning's Lora weights."
-        },
-    )
-    sft_merged_path: Optional[str] = field(
-        default="step1_supervised_finetuning_merged/",
-        metadata={
-            "help": "Output directory for step 1 supervised finetuning's merged weights."
+            "help": (
+                "Output directory for step 1 supervised finetuning's Lora"
+                " weights."
+            )
         },
     )
     lr_scheduler_type_sft: Optional[str] = field(
         default="cosine", metadata={"help": "Type of learning rate scheduler."}
     )
     num_warmup_steps: Optional[int] = field(
-        default=100, metadata={"help": "Number of warmup steps for the scheduler."}
+        default=100,
+        metadata={"help": "Number of warmup steps for the scheduler."},
     )
     lora_config_rl: Optional[LoraConfig] = field(
         default=LoraConfig(
             r=32,
             lora_alpha=64,
             lora_dropout=0.05,
             bias="none",
@@ -167,27 +190,26 @@
         metadata={"help": "LoRA configuration."},
     )
 
     # Step 2 reward modeling parameters
     reward_model_path: Optional[str] = field(
         default="databricks/dolly-v2-3b",
         metadata={
-            "help": "Huggingface model name or a local path to the reward model."
+            "help": (
+                "Huggingface model name or a local path to the reward model."
+            )
         },
     )
     reward_lora_path: Optional[str] = field(
-        default="step1_supervised_finetuning_lora_final/",
+        default="step2_reward_finetuning_lora_final/",
         metadata={
-            "help": "Output directory for step 1 supervised finetuning's Lora weights."
-        },
-    )
-    reward_merged_path: Optional[str] = field(
-        default="step1_supervised_finetuning_merged/",
-        metadata={
-            "help": "Output directory for step 1 supervised finetuning's merged weights."
+            "help": (
+                "Output directory for step 1 supervised finetuning's Lora"
+                " weights."
+            )
         },
     )
     resume_from_checkpoint: Optional[bool] = field(
         default=False,
         metadata={"help": "If you want to resume training where it left off."},
     )
     dataset_reward_folder: Optional[str] = field(
@@ -196,15 +218,17 @@
     )
     dataset_eval_folder: Optional[str] = field(
         default="data/evaluation",
         metadata={"help": "Subset folder of the evaluation dataset to use."},
     )
     reward_num_of_data: Optional[int] = field(
         default=1000,
-        metadata={"help": "The size of the subset of the training data to use."},
+        metadata={
+            "help": "The size of the subset of the training data to use."
+        },
     )
     max_seq_length_reward: Optional[int] = field(
         default=512, metadata={"help": "Maximum sequence length."}
     )
     # dataset_subset_reward_eval: Optional[int] = field(
     #     default=400,
     #     metadata={"help": "The size of the subset of the validation/eval data to use."})
@@ -218,22 +242,25 @@
     )
     remove_unused_columns: Optional[bool] = field(
         default=False,
         metadata={"help": "Whether to remove unused columns from the dataset."},
     )
     label_names: Optional[List[str]] = field(
         default_factory=list,
-        metadata={"help": "List of column names in the dataset to use as labels."},
+        metadata={
+            "help": "List of column names in the dataset to use as labels."
+        },
     )
     logging_strategy: Optional[str] = field(
         default="steps",
         metadata={"help": "The strategy used for logging during training."},
     )
     logging_steps: Optional[int] = field(
-        default=10, metadata={"help": "The number of steps between each logging."}
+        default=10,
+        metadata={"help": "The number of steps between each logging."},
     )
     # callbacks: Optional[List[TrainerCallback]] = field(
     #     default=[], ## PeftSavingCallback()
     #     metadata={"help": "The callbacks to use for training."}),
     # optim: Optional[str] = field(
     #     default="adamw_hf", metadata={"help": "The optimizer to use."})
     # lr_scheduler_type_rw: str = field(
@@ -249,25 +276,32 @@
         ),
         metadata={"help": "LoRA configuration."},
     )
 
     # Step 3 RL parameters
     dataset_subset_rl: Optional[str] = field(
         default="data",
-        metadata={"help": "Subset folder of the dataset to use."}, ## TODO
+        metadata={"help": "Subset folder of the dataset to use."},  ## TODO
     )
     dataset_subset_rl_train: Optional[int] = field(
         default=10000,
-        metadata={"help": "The size of the subset of the training data to use."},
+        metadata={
+            "help": "The size of the subset of the training data to use."
+        },
     )
     adafactor: Optional[bool] = field(
-        default=False, metadata={"help": "whether to use the adafactor optimizer"}
+        default=False,
+        metadata={"help": "whether to use the adafactor optimizer"},
+    )
+    top_k: Optional[float] = field(
+        default=0.0, metadata={"help": "Value for top_k"}
+    )
+    top_p: Optional[float] = field(
+        default=1.0, metadata={"help": "Value for top_p"}
     )
-    top_k: Optional[float] = field(default=0.0, metadata={"help": "Value for top_k"})
-    top_p: Optional[float] = field(default=1.0, metadata={"help": "Value for top_p"})
     do_sample: Optional[bool] = field(
         default=True, metadata={"help": "Flag for sampling"}
     )
     eos_token_id: Optional[int] = field(
         default=100_000, metadata={"help": "End of sentence token id"}
     )
     output_min_length: Optional[int] = field(
@@ -279,37 +313,49 @@
     mini_batch_size: Optional[int] = field(
         default=1, metadata={"help": "the PPO minibatch size"}
     )
     ppo_batch_size: Optional[int] = field(
         default=8, metadata={"help": "the PPO batch size"}
     )
     ppo_epochs: Optional[int] = field(
-        default=10, metadata={"help": "the number of optimisation epochs per batch of samples"}
+        default=10,
+        metadata={
+            "help": "the number of optimisation epochs per batch of samples"
+        },
     )
     total_epochs: Optional[int] = field(
         default=100, metadata={"help": "number of total epochs"}
     )
     early_stopping: Optional[bool] = field(
         default=False, metadata={"help": "whether to early stop"}
     )
     target_kl: Optional[float] = field(
         default=0.1, metadata={"help": "kl target for early stopping"}
     )
     reward_baseline: Optional[float] = field(
         default=0.0,
-        metadata={"help": "a baseline value that is subtracted from the reward"},
+        metadata={
+            "help": "a baseline value that is subtracted from the reward"
+        },
     )
     init_kl_coef: Optional[float] = field(
         default=0.2,
         metadata={
-            "help": "Initial KL penalty coefficient (used for adaptive and linear control)"
+            "help": (
+                "Initial KL penalty coefficient (used for adaptive and linear"
+                " control)"
+            )
         },
     )
     adap_kl_ctrl: Optional[bool] = field(
-        default=True, metadata={"help": "Use adaptive KL control, otherwise linear"}
+        default=True,
+        metadata={"help": "Use adaptive KL control, otherwise linear"},
     )
     rl_lora_path: Optional[str] = field(
-        default="step1_reinforcement_learning_final_lora_weights/",
+        default="step3_reinforcement_learning_final_lora_weights/",
         metadata={
-            "help": "Output directory for step 1 supervised finetuning's Lora weights."
+            "help": (
+                "Output directory for step 3 reinforcement learning's Lora"
+                " weights."
+            )
         },
     )
```

### Comparing `pykoi-0.0.2/pykoi/rlhf/supervised_finetuning.py` & `pykoi-0.0.3/pykoi/rlhf/supervised_finetuning.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,63 +1,68 @@
 """superised_finetuning."""
 import os
 from typing import Optional
 import torch
 
-from datasets import (
-    Dataset,
-    load_dataset)
-from peft import (
-    PeftConfig,
-    PeftModel)
+from datasets import Dataset, load_dataset
+from peft import PeftConfig, PeftModel
 from transformers import (
     AutoModelForCausalLM,
     AutoModelForSequenceClassification,
     AutoTokenizer,
-    TrainingArguments)
+    TrainingArguments,
+)
 
 from trl import SFTTrainer
 from trl.trainer.utils import ConstantLengthDataset
-from pykoi.db.constants import (
+from pykoi.chat.db.constants import (
     QA_CSV_HEADER_ID,
     QA_CSV_HEADER_QUESTION,
     QA_CSV_HEADER_ANSWER,
-    QA_CSV_HEADER_VOTE_STATUS)
-from pykoi.db.qa_database import QuestionAnswerDatabase
+    QA_CSV_HEADER_VOTE_STATUS,
+)
+from pykoi.chat.db.qa_database import QuestionAnswerDatabase
 from pykoi.rlhf.config import RLHFConfig
 
 
-class SupervisedFinetuning():
+class SupervisedFinetuning:
     """
     A class representing the supervised finetuning trainer.
 
     Attributes:
         rlhf_config (RLHFConfig): The RLHF configuration object.
         tokenizer (AutoTokenizer): The tokenizer used for tokenizing the input data.
         num_proc (int): The number of workers to use for data loading.
         dataset (Dict[str, Dataset]): A dictionary containing the train and eval datasets.
         torch_dtype (torch.dtype): The torch data type to use for training.
         training_args (TrainingArguments): The training arguments for the trainer.
         model (AutoModelForCausalLM): The model to train.
         trainer (SFTTrainer): The trainer object used for training the model.
     """
+
     def __init__(self, rlhf_config: RLHFConfig):
         """
         Initializes the SFTTrainer object.
 
         Args:
             rlhf_config (RLHFConfig): The RLHF configuration object.
         """
         self._rlhf_config = rlhf_config
-        self.tokenizer = AutoTokenizer.from_pretrained(rlhf_config.base_model_path)
+        self.tokenizer = AutoTokenizer.from_pretrained(
+            rlhf_config.base_model_path
+        )
         self.num_proc = (
-            self._rlhf_config.num_workers if not self._rlhf_config.streaming else None
+            self._rlhf_config.num_workers
+            if not self._rlhf_config.streaming
+            else None
         )
         self.dataset = self.create_datasets(self.tokenizer, self._rlhf_config)
-        self.torch_dtype = torch.bfloat16 if self._rlhf_config.bf16 else torch.float16
+        self.torch_dtype = (
+            torch.bfloat16 if self._rlhf_config.bf16 else torch.float16
+        )
         # self.torch_dtype = torch.bfloat16 if bf16 else (torch.float16 if fp16 else torch.float32)
         self.training_args = TrainingArguments(
             output_dir=self._rlhf_config.output_dir,
             dataloader_drop_last=True,
             evaluation_strategy=self._rlhf_config.evaluation_strategy,
             max_steps=self._rlhf_config.max_steps,
             eval_steps=self._rlhf_config.eval_freq,
@@ -92,33 +97,36 @@
 
     def train(self):
         """
         Trains the model using the SFTTrainer object.
         """
         self.trainer.train()
 
-    def load_lora(self,
-                  base_model_path: Optional[str] = None,
-                  lora_model_path: Optional[str] = None):
-
+    def load_lora(
+        self,
+        base_model_path: Optional[str] = None,
+        lora_model_path: Optional[str] = None,
+    ):
         if base_model_path is None:
             base_model_path = self._rlhf_config.base_model_path
 
         # Load lora config
         if lora_model_path is None:
             lora_config = self.trainer.model.config
         else:
             lora_config = PeftConfig.from_pretrained(lora_model_path)
 
         # Load the base tokenizer and model
         tokenizer = AutoTokenizer.from_pretrained(base_model_path)
         if lora_config.task_type == "SEQ_CLS":
             # peft is for reward model so load sequence classification
             base_model = AutoModelForSequenceClassification.from_pretrained(
-                base_model_path, num_labels=1, torch_dtype=self._rlhf_config.torch_dtype
+                base_model_path,
+                num_labels=1,
+                torch_dtype=self._rlhf_config.torch_dtype,
             )
         elif lora_config.task_type == "CAUSAL_LM":
             base_model = AutoModelForCausalLM.from_pretrained(
                 base_model_path,
                 return_dict=True,
                 torch_dtype=self._rlhf_config.torch_dtype,
             )
@@ -126,61 +134,74 @@
             raise ValueError("Invalid task_type in lora_config")
 
         # Merge the base model and the Lora model
         model = PeftModel.from_pretrained(base_model, lora_config)
         return model, tokenizer
 
     def save(self, output_path=None):
-
         if output_path is None:
             output_path = os.path.join(
                 self._rlhf_config.output_dir, self._rlhf_config.sft_lora_path
             )
         self.trainer.save_model(output_path)
 
     def train_and_save(self, output_path=None):
         self.trainer.train()
         self.save(output_path)
 
     def prepare_sample_text(self, example):
         """Prepare the text from a sample of the dataset."""
-        text = f"Question: {example[self._rlhf_config.question_title]}\n\n\
-            Answer: {example[self._rlhf_config.answer_title]}"
+        text = (
+            f"Question: {example[self._rlhf_config.question_title]}\n\n        "
+            f"    Answer: {example[self._rlhf_config.answer_title]}"
+        )
         return text
 
     def create_datasets(self, tokenizer, args):
         if args.dataset_type == "local_db":
             qa_database = QuestionAnswerDatabase()
             my_data_pd = qa_database.retrieve_all_question_answers_as_pandas()
-            my_data_pd = my_data_pd[my_data_pd[QA_CSV_HEADER_VOTE_STATUS] == "up"]
-            my_data_pd = my_data_pd[[QA_CSV_HEADER_ID,
-                                     QA_CSV_HEADER_QUESTION,
-                                     QA_CSV_HEADER_ANSWER]]
-            print("My local database has {} up vote samples for SFT".format(my_data_pd.shape[0]))
+            my_data_pd = my_data_pd[
+                my_data_pd[QA_CSV_HEADER_VOTE_STATUS] == "up"
+            ]
+            my_data_pd = my_data_pd[
+                [QA_CSV_HEADER_ID, QA_CSV_HEADER_QUESTION, QA_CSV_HEADER_ANSWER]
+            ]
+            print(
+                "My local database has {} up vote samples for SFT".format(
+                    my_data_pd.shape[0]
+                )
+            )
             dataset = Dataset.from_dict(my_data_pd)
         elif args.dataset_type == "local_csv":
-            dataset = load_dataset('csv', data_files=args.dataset_name)
+            dataset = load_dataset("csv", data_files=args.dataset_name)
             dataset = dataset[args.split]  # Convert DatasetDict to Dataset
         elif args.dataset_type == "huggingface":
             dataset = load_dataset(
                 args.dataset_name,
                 data_dir=args.dataset_subset_sft,
                 split=args.split,
                 use_auth_token=True,
                 num_proc=self.num_proc,
                 streaming=args.streaming,
             )
             dataset = dataset[args.split]  # Convert DatasetDict to Dataset
         else:
-            raise FileNotFoundError(f"No (supported) data files or dataset script found {args.dataset_type}")
+            raise FileNotFoundError(
+                "No (supported) data files or dataset script found"
+                f" {args.dataset_type}"
+            )
 
-        dataset = dataset.train_test_split(test_size=args.train_test_split_ratio, 
-                                           seed=args.seed)
-        print(f"Size of the train set: {len(dataset['train'])}. \
-              Size of the validation set: {len(dataset['test'])}")
+        dataset = dataset.train_test_split(
+            test_size=args.train_test_split_ratio, seed=args.seed
+        )
+        print(
+            f"Size of the train set: {len(dataset['train'])}.              "
+            f" Size of the validation set: {len(dataset['test'])}"
+        )
 
         train_dataset = ConstantLengthDataset(
             tokenizer,
             dataset["train"],
             formatting_func=self.prepare_sample_text,
             infinite=True,
             seq_length=args.max_seq_length,
```

### Comparing `pykoi-0.0.2/pykoi/state.py` & `pykoi-0.0.3/pykoi/state.py`

 * *Files identical despite different names*

### Comparing `pykoi-0.0.2/pyproject.toml` & `pykoi-0.0.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pykoi"
-version = "0.0.02"
+version = "0.0.3"
 description = ""
 authors = ["CambioML <wanwanaiai45@gmail.com>"]
 license = "Apache"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.13"
@@ -22,14 +22,17 @@
 datasets = "2.13.1"
 evaluate = "0.4.0"
 peft = "0.4.0"
 trl = "0.4.7"
 openai = "0.27.8"
 passlib = "1.7.4"
 bcrypt = "4.0.1"
+scikit-learn = "1.3.0"
+torch = "2.0.1"
+posthog = "3.0.1"
 
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.3.3"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `pykoi-0.0.2/PKG-INFO` & `pykoi-0.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pykoi
-Version: 0.0.2
+Version: 0.0.3
 Summary: 
 License: Apache
 Author: CambioML
 Author-email: wanwanaiai45@gmail.com
 Requires-Python: >=3.9,<3.13
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -18,18 +18,21 @@
 Requires-Dist: einops (==0.6.1)
 Requires-Dist: evaluate (==0.4.0)
 Requires-Dist: fastapi (==0.100.0)
 Requires-Dist: openai (==0.27.8)
 Requires-Dist: pandas (==2.0.3)
 Requires-Dist: passlib (==1.7.4)
 Requires-Dist: peft (==0.4.0)
+Requires-Dist: posthog (==3.0.1)
 Requires-Dist: pydantic (==2.1.1)
 Requires-Dist: pyngrok (==6.0.0)
+Requires-Dist: scikit-learn (==1.3.0)
 Requires-Dist: scipy (==1.11.1)
 Requires-Dist: starlette (==0.27.0)
+Requires-Dist: torch (==2.0.1)
 Requires-Dist: transformers (==4.31.0)
 Requires-Dist: trl (==0.4.7)
 Requires-Dist: uvicorn (==0.23.1)
 Description-Content-Type: text/markdown
 
 
 # :whale2: pykoi: Active learning in one unified interface :ocean:!
```

