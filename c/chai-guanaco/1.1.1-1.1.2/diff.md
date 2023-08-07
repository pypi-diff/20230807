# Comparing `tmp/chai-guanaco-1.1.1.tar.gz` & `tmp/chai-guanaco-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/chai-guanaco-1.1.1.tar", last modified: Fri Aug  4 23:04:51 2023, max compression
+gzip compressed data, was "dist/chai-guanaco-1.1.2.tar", last modified: Mon Aug  7 16:17:27 2023, max compression
```

## Comparing `chai-guanaco-1.1.1.tar` & `chai-guanaco-1.1.2.tar`

### file list

```diff
@@ -1,20 +1,39 @@
-drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-08-04 23:04:51.000000 chai-guanaco-1.1.1/
--rw-rw-r--   0 tom       (1002) tom       (1002)     9482 2023-08-04 23:04:51.000000 chai-guanaco-1.1.1/PKG-INFO
--rw-rw-r--   0 tom       (1002) tom       (1002)     8036 2023-08-04 23:04:33.000000 chai-guanaco-1.1.1/README.md
-drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-08-04 23:04:51.000000 chai-guanaco-1.1.1/chai_guanaco.egg-info/
--rw-rw-r--   0 tom       (1002) tom       (1002)     9482 2023-08-04 23:04:50.000000 chai-guanaco-1.1.1/chai_guanaco.egg-info/PKG-INFO
--rw-rw-r--   0 tom       (1002) tom       (1002)      452 2023-08-04 23:04:50.000000 chai-guanaco-1.1.1/chai_guanaco.egg-info/SOURCES.txt
--rw-rw-r--   0 tom       (1002) tom       (1002)        1 2023-08-04 23:04:50.000000 chai-guanaco-1.1.1/chai_guanaco.egg-info/dependency_links.txt
--rw-rw-r--   0 tom       (1002) tom       (1002)        1 2023-08-04 23:04:50.000000 chai-guanaco-1.1.1/chai_guanaco.egg-info/not-zip-safe
--rw-rw-r--   0 tom       (1002) tom       (1002)        9 2023-08-04 23:04:50.000000 chai-guanaco-1.1.1/chai_guanaco.egg-info/requires.txt
--rw-rw-r--   0 tom       (1002) tom       (1002)       13 2023-08-04 23:04:50.000000 chai-guanaco-1.1.1/chai_guanaco.egg-info/top_level.txt
--rw-rw-r--   0 tom       (1002) tom       (1002)       38 2023-08-04 23:04:51.000000 chai-guanaco-1.1.1/setup.cfg
--rw-rw-r--   0 tom       (1002) tom       (1002)      746 2023-08-04 23:04:48.000000 chai-guanaco-1.1.1/setup.py
-drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-08-04 23:04:51.000000 chai-guanaco-1.1.1/src/
-drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-08-04 23:04:51.000000 chai-guanaco-1.1.1/src/chai_guanaco/
--rw-rw-r--   0 tom       (1002) tom       (1002)        0 2023-08-04 23:04:33.000000 chai-guanaco-1.1.1/src/chai_guanaco/__init__.py
--rw-rw-r--   0 tom       (1002) tom       (1002)      467 2023-08-04 23:04:33.000000 chai-guanaco-1.1.1/src/chai_guanaco/feedback.py
--rw-rw-r--   0 tom       (1002) tom       (1002)     1385 2023-08-04 23:04:33.000000 chai-guanaco-1.1.1/src/chai_guanaco/submit.py
-drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-08-04 23:04:51.000000 chai-guanaco-1.1.1/tests/
--rw-rw-r--   0 tom       (1002) tom       (1002)      969 2023-08-04 23:04:33.000000 chai-guanaco-1.1.1/tests/test_feedback.py
--rw-rw-r--   0 tom       (1002) tom       (1002)     2998 2023-08-04 23:04:33.000000 chai-guanaco-1.1.1/tests/test_submit.py
+drwxrwxr-x   0 alex      (1003) alex      (1003)        0 2023-08-07 16:17:27.000000 chai-guanaco-1.1.2/
+-rw-rw-r--   0 alex      (1003) alex      (1003)       72 2023-08-07 16:08:30.000000 chai-guanaco-1.1.2/MANIFEST.in
+-rw-rw-r--   0 alex      (1003) alex      (1003)    11603 2023-08-07 16:17:27.000000 chai-guanaco-1.1.2/PKG-INFO
+-rw-rw-r--   0 alex      (1003) alex      (1003)     9789 2023-08-07 16:08:30.000000 chai-guanaco-1.1.2/README.md
+-rw-rw-r--   0 alex      (1003) alex      (1003)       46 2023-07-26 22:05:52.000000 chai-guanaco-1.1.2/requirements.txt
+-rw-rw-r--   0 alex      (1003) alex      (1003)       38 2023-08-07 16:17:27.000000 chai-guanaco-1.1.2/setup.cfg
+-rw-rw-r--   0 alex      (1003) alex      (1003)      978 2023-08-07 16:17:24.000000 chai-guanaco-1.1.2/setup.py
+drwxrwxr-x   0 alex      (1003) alex      (1003)        0 2023-08-07 16:17:27.000000 chai-guanaco-1.1.2/src/
+drwxrwxr-x   0 alex      (1003) alex      (1003)        0 2023-08-07 16:17:27.000000 chai-guanaco-1.1.2/src/chai_guanaco/
+-rw-rw-r--   0 alex      (1003) alex      (1003)      270 2023-07-26 22:05:52.000000 chai-guanaco-1.1.2/src/chai_guanaco/__init__.py
+-rw-rw-r--   0 alex      (1003) alex      (1003)     4841 2023-07-26 22:05:52.000000 chai-guanaco-1.1.2/src/chai_guanaco/chat.py
+-rw-rw-r--   0 alex      (1003) alex      (1003)     3259 2023-07-26 22:05:52.000000 chai-guanaco-1.1.2/src/chai_guanaco/feedback.py
+-rw-rw-r--   0 alex      (1003) alex      (1003)     1756 2023-07-26 22:05:52.000000 chai-guanaco-1.1.2/src/chai_guanaco/formatters.py
+-rw-rw-r--   0 alex      (1003) alex      (1003)     1966 2023-07-26 22:05:52.000000 chai-guanaco-1.1.2/src/chai_guanaco/login_cli.py
+-rw-rw-r--   0 alex      (1003) alex      (1003)     7397 2023-08-04 23:43:39.000000 chai-guanaco-1.1.2/src/chai_guanaco/metrics.py
+drwxrwxr-x   0 alex      (1003) alex      (1003)        0 2023-08-07 16:17:27.000000 chai-guanaco-1.1.2/src/chai_guanaco/resources/
+drwxrwxr-x   0 alex      (1003) alex      (1003)        0 2023-08-07 16:17:27.000000 chai-guanaco-1.1.2/src/chai_guanaco/resources/bot_config/
+-rw-rw-r--   0 alex      (1003) alex      (1003)     1332 2023-08-04 21:30:33.000000 chai-guanaco-1.1.2/src/chai_guanaco/resources/bot_config/blade.json
+-rw-rw-r--   0 alex      (1003) alex      (1003)     1529 2023-08-04 21:30:33.000000 chai-guanaco-1.1.2/src/chai_guanaco/resources/bot_config/captain_wyatt.json
+-rw-rw-r--   0 alex      (1003) alex      (1003)     2031 2023-08-04 21:30:33.000000 chai-guanaco-1.1.2/src/chai_guanaco/resources/bot_config/coffee_shop_girl.json
+-rw-rw-r--   0 alex      (1003) alex      (1003)     1305 2023-08-04 21:30:33.000000 chai-guanaco-1.1.2/src/chai_guanaco/resources/bot_config/filbert.json
+-rw-rw-r--   0 alex      (1003) alex      (1003)     1050 2023-08-04 21:30:33.000000 chai-guanaco-1.1.2/src/chai_guanaco/resources/bot_config/leo.json
+-rw-rw-r--   0 alex      (1003) alex      (1003)     1053 2023-08-04 21:30:33.000000 chai-guanaco-1.1.2/src/chai_guanaco/resources/bot_config/levi.json
+-rw-rw-r--   0 alex      (1003) alex      (1003)     1821 2023-08-04 21:30:33.000000 chai-guanaco-1.1.2/src/chai_guanaco/resources/bot_config/mr_wilson.json
+-rw-rw-r--   0 alex      (1003) alex      (1003)     1094 2023-08-04 21:30:33.000000 chai-guanaco-1.1.2/src/chai_guanaco/resources/bot_config/nerd_girl.json
+-rw-rw-r--   0 alex      (1003) alex      (1003)     2205 2023-08-04 21:30:33.000000 chai-guanaco-1.1.2/src/chai_guanaco/resources/bot_config/scaramouche.json
+-rw-rw-r--   0 alex      (1003) alex      (1003)     1386 2023-08-04 21:30:33.000000 chai-guanaco-1.1.2/src/chai_guanaco/resources/bot_config/story_teller.json
+-rw-rw-r--   0 alex      (1003) alex      (1003)     2510 2023-08-04 21:30:33.000000 chai-guanaco-1.1.2/src/chai_guanaco/resources/bot_config/vampire_queen.json
+-rw-rw-r--   0 alex      (1003) alex      (1003)     2246 2023-08-04 21:30:33.000000 chai-guanaco-1.1.2/src/chai_guanaco/resources/bot_config/wednesday_addams.json
+-rw-rw-r--   0 alex      (1003) alex      (1003)     5474 2023-08-04 21:24:56.000000 chai-guanaco-1.1.2/src/chai_guanaco/submit.py
+-rw-rw-r--   0 alex      (1003) alex      (1003)     1945 2023-07-26 22:05:52.000000 chai-guanaco-1.1.2/src/chai_guanaco/utils.py
+drwxrwxr-x   0 alex      (1003) alex      (1003)        0 2023-08-07 16:17:27.000000 chai-guanaco-1.1.2/src/chai_guanaco.egg-info/
+-rw-rw-r--   0 alex      (1003) alex      (1003)    11603 2023-08-07 16:17:27.000000 chai-guanaco-1.1.2/src/chai_guanaco.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1003) alex      (1003)     1199 2023-08-07 16:17:27.000000 chai-guanaco-1.1.2/src/chai_guanaco.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1003) alex      (1003)        1 2023-08-07 16:17:27.000000 chai-guanaco-1.1.2/src/chai_guanaco.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1003) alex      (1003)       61 2023-08-07 16:17:27.000000 chai-guanaco-1.1.2/src/chai_guanaco.egg-info/entry_points.txt
+-rw-rw-r--   0 alex      (1003) alex      (1003)        1 2023-08-07 15:14:15.000000 chai-guanaco-1.1.2/src/chai_guanaco.egg-info/not-zip-safe
+-rw-rw-r--   0 alex      (1003) alex      (1003)       46 2023-08-07 16:17:27.000000 chai-guanaco-1.1.2/src/chai_guanaco.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1003) alex      (1003)       13 2023-08-07 16:17:27.000000 chai-guanaco-1.1.2/src/chai_guanaco.egg-info/top_level.txt
```

### Comparing `chai-guanaco-1.1.1/PKG-INFO` & `chai-guanaco-1.1.2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,158 +1,193 @@
-Metadata-Version: 2.1
-Name: chai-guanaco
-Version: 1.1.1
-Summary: Chai Guanaco
-Home-page: https://www.chai-research.com
-Author: Chai Research Corp.
-Author-email: hello@chai-research.com
-License: MIT
-Description: [![Guanaco Banner](https://imgur.com/uba9Jce.png)](https://www.chai-research.com/competition.html)
-        
-        [![Pull Requests Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat)](http://makeapullrequest.com)
-        [![first-timers-only Friendly](https://img.shields.io/badge/first--timers--only-friendly-blue.svg)](http://www.firsttimersonly.com/)
-        
-        [Chai Guanaco](https://www.chai-research.com/competition.html) is part of the Chai Guanaco Competition, accelerating community AGI.
-        
-        It's the world's first open community challenge with real-user evaluations. You can submit any GPT-J based 6B models, it will be directly deployed on the [Chai App](https://apps.apple.com/us/app/chai-chat-with-ai-bots/id1544750895) where our over 500K daily active users will be providing live feedback. Get to top of the leaderboard and share the $1 million cash prize!
-        
-        
-        ## The Guanaco Guide
-        
-        🥇 **Evaluation & Prizes:** Depending on the phase of the competition, a suite of user-level evaluation metrics will be used (i.e. thumbs up / thumbs down rate). Your model will be ranked in real-time compared with other models, you can view the leaderboard at anytime with the pip package
-        
-        🕵️ **Real-time user feedback:** After your model is deployed, it will go through an safety + integrity checker, once passed, it will be deployed directly to our users who will provide written feedback that you can view via the pip package.
-        
-        
-        🤖 **Model requirements:** Currently, we support *any* models based off [GPT-J 6B](https://huggingface.co/EleutherAI/gpt-j-6b) (i.e. 6B parameters with GPT2 tokenizer). All you need to do is push your model directly to huggingface. Support for more model types is coming soon!
-        
-        ⚙️ **Sampling parameters:** During submission, we allow for custom model generation parameters such as temperature. Once your model is deployed on our platform, it will be using the parameters you've provided to generate chat completions.
-        
-        
-        ## How Does It Work?
-        
-        -   The `chai_guanaco` pip package provides a way to easily submit your language model, all you need to do is ensure it is on HuggingFace 🤗
-        -   We will automatically **Tritonize** your model for fast inference and host it in our internal GPU cluster 🚀
-        -   Once deployed, Chai users on our platform who enter the **arena mode** will be rating your model directly, providing you with both quantatitive and verbal feedback 📈
-        -   Both the public leaderboard and **user feedback** for your model can be directly downloaded via the `chai_guanaco` package 🧠
-        -   Cash prizes will be allocated according to your position in the leaderboard 💰
-        
-        [![Chai Pipeline](https://imgur.com/LtMWOAq.png)](https://www.chai-research.com/competition.html)
-        
-        ## 🚀 Getting Started
-        
-        **Getting Developer Key**
-        
-        Join the [competition discord](https://discord.gg/7mXdjAkw2s), introduce yourself and ask for a developer key. Login-based authentication is coming next 🤗
-        
-        
-        **Submitting A Model**
-        
-        Use [pip](https://github.com/pypa/pip) to install the Chai Guanaco package
-        
-        ```sh
-        pip install chai-guanaco
-        ```
-        
-        Upload any GPT-J 6B based language model *with a tokenizer* to huggingface, i.e. [EleutherAI/gpt-j-6b](https://huggingface.co/EleutherAI/gpt-j-6b). Read [this guide](https://huggingface.co/docs/transformers/model_sharing) if you are unsure. Click the *Use in Transformers* button in huggingface to get the your huggingface model ID (i.e. "EleutherAI/gpt-j-6b")
-        
-        To submit model simply run:
-        
-        ```python
-        from chai_guanaco.submit import submit_model
-        
-        model_url = "EleutherAI/gpt-j-6b" # Your model URL
-        developer_key = "CR_XXXX" # Your developer key
-        submission_parameters = {'model_repo': model_url}
-        response = submit_model(submission_parameters, developer_key)
-        submission_id = response['submission_id']
-        print(submission_id)
-        ````
-        which outputs your submission id, unique to your model submission.
-        
-        To verify the status of a submission, you can use the following command:
-        
-        ```python
-        from chai_guanaco.submit import get_model_info
-        
-        model_info = get_model_info(submission_id, developer_key)
-        print(model_info)
-        ```
-        Once the `status` field shows `success` it means your model has been successfully submitted. A submission typically takes around 10 minutes for the tritonisation process to complete.
-        
-        **Getting User Feedback**
-        
-        Once your model has been submitted, it is automatically deployed to the Chai Platform where real-life users will evaluate your model performance. To view their feedback, run:
-        
-        ```python
-        from chai_guanaco.feedback import get_feedback
-        
-        model_feedback = get_feedback(submission_id, developer_key)
-        print(model_feedback)
-        ```
-        
-        Here, you will find a pandas dataframe with all the user feedback for your model, including the conversation each user has had with your model.
-        
-        **Getting Live Leaderboard**
-        
-        To see how your model performs against other models, run:
-        ```python
-        from chai_guanaco.feedback import display_leaderboard
-        
-        display_leaderboard(developer_key)
-        ```
-        which prints out the current leaderboard, with your models positions highlighted
-        
-        **Re-Submitting Models**
-        
-        Because it is a competition, you are allowed to test a single model at any given time. However, you can deactivate a model and submit a new one. To do this, simply run:
-        
-        ```python
-        from chai_guanaco.submit import deactivate_model
-        
-        deactivate_model(submission_id, developer_key)
-        ```
-        Which will deactive your model, don't worry, all the model feedback will still be saved, it just means the model will no longer be exposed to users. You can then re-submit by repeating the model submission step.
-        
-        **Retrieve Your Model Submission IDs**
-        
-        In case you have forgotten your submission ids / want to view all past submissions, run:
-        
-        ```python
-        from chai_guanaco.submit import get_my_submissions
-        
-        submission_ids = get_my_submissions(developer_key)
-        print(submission_ids)
-        ```
-        Here you will see all your model submission_ids along with their status, which is either `failed`, `inactive` or `deployed`.
-        
-        **Advanced Submission**
-        
-        You can tweak the model generation sampling parameters by passing the parameters you want during model submission, for example:
-        
-        ```python
-        from chai_guanaco.submit import submit_model
-        
-        generation_params= {"temperature": 1.0, "top_p": 1.0, "top_k": 40, "repetition_penalty": 1.0}
-        submission_parameters = {'model_repo': model_url, 'generation_params': generation_params}
-        response = submit_model(submission_parameters, developer_key)
-        ```
-        
-        ## Resources
-        |                                                                        |                                                                                                 |
-        | ---------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------|
-        | 📒 [Fine tuning guide](https://huggingface.co/docs/transformers/training) | Guide on language model finetuning                                                           |
-        | 💾 [Datasets](https://dataset-ideas.tiiny.site/) | Curated list of open-sourced datasets to get started with finetuning                                                  |
-        | 💖 [Guanaco Discord](https://haystack.deepset.ai/tutorials)                   | Our Guanaco competition discord                                                          |
-        |🚀 [Deepspeed Guide](https://huggingface.co/docs/transformers/main_classes/deepspeed)     | Guide for training with Deepspeed (faster training without GPU bottleneck)    |
-        |💬 [Example Conversations](https://huggingface.co/docs/transformers/main_classes/deepspeed)     | Here you can find 1000 example conversations from the Chai Platform     |
-        | ⚒️ [Build with us](https://boards.greenhouse.io/nexus/jobs/5319721003)| If you think what we are building is cool, join us!|
-        
-        
-        ## 🦙 Hosted & Sponsored By
-        
-        <a href="https://www.chai-research.com/"><img src="https://i.imgur.com/optjNAw.png" alt="Chai Logo" height="70"/></a>
-        
-        <a href="https://www.coreweave.com/"><img src="https://imgur.com/oJyuH8q.png" alt="Coreweave Logo" height="70"/></a>
-        
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
+[![Guanaco Banner](https://imgur.com/wJHIeAU.png)](https://www.chai-research.com/competition.html)
+
+[![Pull Requests Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat)](http://makeapullrequest.com)
+[![first-timers-only Friendly](https://img.shields.io/badge/first--timers--only-friendly-blue.svg)](http://www.firsttimersonly.com/)
+
+[Chai Guanaco](https://www.chai-research.com/competition.html) is part of the Chai Guanaco Competition, accelerating community AGI.
+
+It's the world's first open community challenge with real-user evaluations. You can submit any GPT-J based 6B models, it will be directly deployed on the [Chai App](http://tosto.re/chaiapp) where our over 500K daily active users will be providing live feedback. Get to top of the leaderboard and share the $1 million cash prize!
+
+## Quick Start
+
+[Chai Guanaco Jupyter Notebook Quickstart](https://datalore.jetbrains.com/notebook/ABxxIKqVGejPnF8zH6zFpx/WQd6vDlfCDux5wzuoAeF8m)
+
+
+## The Guanaco Guide
+
+🥇 **Evaluation & Prizes:** Depending on the phase of the competition, a suite of user-level evaluation metrics will be used (i.e. thumbs up / thumbs down rate). Your model will be ranked in real-time compared with other models, you can view the leaderboard at anytime with the pip package
+
+🕵️ **Real-time user feedback:** After your model is deployed, it will go through an safety + integrity checker, once passed, it will be deployed directly to our users who will provide written feedback that you can view via the pip package.
+
+🤖 **Model requirements:** Currently, we support *any* models based off [LLaMA 2](https://huggingface.co/docs/transformers/model_doc/llama2) (i.e. 7/13B parameters with LLaMA tokenizer). All you need to do is push your model directly to huggingface. Support for more model types is coming soon!
+
+⚙️ **Sampling parameters:** During submission, we allow for custom model generation parameters such as temperature. Once your model is deployed on our platform, it will be using the parameters you've provided to generate chat completions.
+
+📚 **Rules:** By default, 1 developer key per person, each key can deploy 1 model to users at a time. Message in discord if you would like the limit bumped up 😀
+
+
+## How Does It Work?
+
+-   The `chai_guanaco` pip package provides a way to easily submit your language model, all you need to do is ensure it is on HuggingFace 🤗
+-   We will automatically **Tritonize** your model for fast inference and host it in our internal GPU cluster 🚀
+-   Once deployed, Chai users on our platform who enter the **arena mode** will be rating your model directly, providing you with both quantatitive and verbal feedback 📈
+-   Both the public leaderboard and **user feedback** for your model can be directly downloaded via the `chai_guanaco` package 🧠
+-   Cash prizes will be allocated according to your position in the leaderboard 💰
+
+[![Chai Pipeline](https://imgur.com/LtMWOAq.png)](https://www.chai-research.com/competition.html)
+
+## 🚀 Getting Started
+
+**Getting Developer Key**
+
+Join the [competition discord](https://discord.gg/7mXdjAkw2s), introduce yourself and ask for a developer key. Login-based authentication is coming next 🤗
+
+
+**Installation**
+
+Use [pip](https://github.com/pypa/pip) to install the Chai Guanaco package
+
+```sh
+pip install chai-guanaco
+```
+
+For one-off authentication run the following in your terminal:
+
+```sh
+chai-guanaco login
+```
+
+And pass in your developer key when prompted, you can always logout using `chai-guanaco logout`.
+
+**Model Submission**
+
+Upload any Llama based language model *with a tokenizer* to huggingface, i.e. [NousResearch/Llama-2-7b-chat-hf](https://huggingface.co/NousResearch/Llama-2-7b-chat-hf). Read [this guide](https://huggingface.co/docs/transformers/model_sharing) if you are unsure. Click the *Use in Transformers* button in huggingface to get the your huggingface model ID (i.e. "NousResearch/Llama-2-7b-chat-hf")
+
+To submit model simply run:
+
+```python
+import chai_guanaco as chai
+
+model_url = "NousResearch/Llama-2-7b-chat-hf" # Your model URL
+
+generation_params = {
+	'temperature': 1.0,
+	'repetition_penalty': 1.13,
+	'top_p': 0.2,
+	"top_k": 40,
+	"stopping_words": ['\n'],
+	"presence_penalty": 0.,
+	"frequency_penalty": 0.
+	}
+submission_parameters = {'model_repo': model_url, 'generation_params': generation_params, 'model_name': 'my-awesome-llama'}
+
+submitter = chai.ModelSubmitter()
+submission_id = submitter.submit(submission_parameters)
+```
+
+This will display an animation while your model is being deployed, a typical
+deployment takes approximately 10 minutes. Note the `model_name` parameter is used for show-casing your model on the leaderboard and it should help you with identifying your model
+
+
+**Chat With Your Model Submission**
+
+Once your model is deployed, you can verify its behaviour and raw input by running:
+
+```python
+chatbot = chai.SubmissionChatbot(submission_id)
+chatbot.chat('nerd_girl', show_model_input=False)
+```
+
+Here you can have a dialog with one of the bots we have provided. To quit the chat, simply enter "exit". Note that, in order to prevent spamming, each model submission is limited to 1000 chat messages from the Chai Guanaco pip package.
+
+You can get a list of avaliable bots by running:
+
+```python
+chatbot.show_avaliable_bots()
+```
+
+Finally, to enter a chat session that prints out the raw input that was fed into your model at each turn of the conversation, you can run:
+
+```python
+chatbot.chat('nerd_girl', show_model_input=True)
+```
+
+**Getting User Feedback**
+
+Once your model has been submitted, it is automatically deployed to the Chai Platform where real-life users will evaluate your model performance. To view their feedback, run:
+
+```python
+model_feedback = chai.get_feedback(submission_id)
+model_feedback.sample()
+```
+
+Which will print out one of the users' conversation, together with meta information associated with the conversation (i.e. rating and user feedback).
+
+To get all the feedback for your model, run...
+
+```python
+df = model_feedback.df
+print(df)
+```
+
+This outputs a Pandas `DataFrame`, where each row corresponds to a user conversation with your model, together with their feedback.
+
+**Getting Live Leaderboard**
+
+To view the public leaderboard used to determine prizes (which only shows the best model submitted by each developer):
+```python
+df = chai.display_leaderboard(detailed=False)
+```
+
+To see how your model performs against other models, run:
+```python
+df = chai.display_leaderboard(detailed=True)
+```
+which prints out the current leaderboard according to the most recent competition metrics, you can also access raw leaderboard is dumped to `df`
+
+**Re-Submitting Models**
+
+Because it is a competition, you are allowed to test a single model at any given time. However, you can deactivate a model and submit a new one. To do this, simply run:
+
+```python
+chai.deactivate_model(submission_id)
+```
+Which will deactive your model, don't worry, all the model feedback will still be saved, it just means the model will no longer be exposed to users. You can then re-submit by repeating the model submission step.
+
+**Retrieve Your Model Submission IDs**
+
+In case you have forgotten your submission ids / want to view all past submissions, run:
+
+```python
+submission_ids = chai.get_my_submissions()
+print(submission_ids)
+```
+Here you will see all your model submission_ids along with their status, which is either `failed`, `inactive` or `deployed`.
+
+**Advanced Usage**
+- This package caches various data, such as your developer key, in the folder `~/.chai-guanaco`. To change this, you can set the environment variable `GUANACO_DATA_DIR` to point to a different folder. You may need to re-run `chai-guanaco login` to update the cached developer key.
+- You can also access the raw feedback data by running
+	```python
+	model_feedback = chai.get_feedback(submission_id)
+	raw_data = model_feedback.raw_data
+	```
+- To submit your model with custom formatting, you can create your own
+  `PromptFormatter`. For more details and examples, please see [here](https://wild-chatter-b52.notion.site/Guanaco-Custom-Formatters-1f64f94b9cf54c819a341988aec5766a).
+
+
+
+## Resources
+|                                                                        |                                                                                                 |
+| ---------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------|
+| 📒 [Fine tuning guide](https://huggingface.co/docs/transformers/training) | Guide on language model finetuning                                                           |
+| 💾 [Datasets](https://dataset-ideas.tiiny.site/) | Curated list of open-sourced datasets to get started with finetuning                                                  |
+| 💖 [Guanaco Discord](https://discord.gg/7mXdjAkw2s)                   | Our Guanaco competition discord                                                          |
+|🚀 [Deepspeed Guide](https://huggingface.co/docs/transformers/main_classes/deepspeed)     | Guide for training with Deepspeed (faster training without GPU bottleneck)    |
+|💬 [Example Conversations](https://huggingface.co/datasets/ChaiML/100_example_conversations)     | Here you can find 100 example conversations from the Chai Platform     |
+| ⚒️ [Build with us](https://boards.greenhouse.io/nexus/jobs/5319721003)| If you think what we are building is cool, join us!|
+
+
+## 🦙 Hosted & Sponsored By
+
+<a href="https://www.chai-research.com/"><img src="https://imgur.com/u3rOQDJ.png" alt="Chai Logo" height="90"/></a>
+
+<a href="https://www.coreweave.com/"><img src="https://imgur.com/oJyuH8q.png" alt="Coreweave Logo" height="70"/></a>
```

### Comparing `chai-guanaco-1.1.1/chai_guanaco.egg-info/PKG-INFO` & `chai-guanaco-1.1.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,41 @@
 Metadata-Version: 2.1
 Name: chai-guanaco
-Version: 1.1.1
+Version: 1.1.2
 Summary: Chai Guanaco
 Home-page: https://www.chai-research.com
 Author: Chai Research Corp.
 Author-email: hello@chai-research.com
 License: MIT
-Description: [![Guanaco Banner](https://imgur.com/uba9Jce.png)](https://www.chai-research.com/competition.html)
+Description: [![Guanaco Banner](https://imgur.com/wJHIeAU.png)](https://www.chai-research.com/competition.html)
         
         [![Pull Requests Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat)](http://makeapullrequest.com)
         [![first-timers-only Friendly](https://img.shields.io/badge/first--timers--only-friendly-blue.svg)](http://www.firsttimersonly.com/)
         
         [Chai Guanaco](https://www.chai-research.com/competition.html) is part of the Chai Guanaco Competition, accelerating community AGI.
         
-        It's the world's first open community challenge with real-user evaluations. You can submit any GPT-J based 6B models, it will be directly deployed on the [Chai App](https://apps.apple.com/us/app/chai-chat-with-ai-bots/id1544750895) where our over 500K daily active users will be providing live feedback. Get to top of the leaderboard and share the $1 million cash prize!
+        It's the world's first open community challenge with real-user evaluations. You can submit any GPT-J based 6B models, it will be directly deployed on the [Chai App](http://tosto.re/chaiapp) where our over 500K daily active users will be providing live feedback. Get to top of the leaderboard and share the $1 million cash prize!
+        
+        ## Quick Start
+        
+        [Chai Guanaco Jupyter Notebook Quickstart](https://datalore.jetbrains.com/notebook/ABxxIKqVGejPnF8zH6zFpx/WQd6vDlfCDux5wzuoAeF8m)
         
         
         ## The Guanaco Guide
         
         🥇 **Evaluation & Prizes:** Depending on the phase of the competition, a suite of user-level evaluation metrics will be used (i.e. thumbs up / thumbs down rate). Your model will be ranked in real-time compared with other models, you can view the leaderboard at anytime with the pip package
         
         🕵️ **Real-time user feedback:** After your model is deployed, it will go through an safety + integrity checker, once passed, it will be deployed directly to our users who will provide written feedback that you can view via the pip package.
         
-        
-        🤖 **Model requirements:** Currently, we support *any* models based off [GPT-J 6B](https://huggingface.co/EleutherAI/gpt-j-6b) (i.e. 6B parameters with GPT2 tokenizer). All you need to do is push your model directly to huggingface. Support for more model types is coming soon!
+        🤖 **Model requirements:** Currently, we support *any* models based off [LLaMA 2](https://huggingface.co/docs/transformers/model_doc/llama2) (i.e. 7/13B parameters with LLaMA tokenizer). All you need to do is push your model directly to huggingface. Support for more model types is coming soon!
         
         ⚙️ **Sampling parameters:** During submission, we allow for custom model generation parameters such as temperature. Once your model is deployed on our platform, it will be using the parameters you've provided to generate chat completions.
         
+        📚 **Rules:** By default, 1 developer key per person, each key can deploy 1 model to users at a time. Message in discord if you would like the limit bumped up 😀
+        
         
         ## How Does It Work?
         
         -   The `chai_guanaco` pip package provides a way to easily submit your language model, all you need to do is ensure it is on HuggingFace 🤗
         -   We will automatically **Tritonize** your model for fast inference and host it in our internal GPU cluster 🚀
         -   Once deployed, Chai users on our platform who enter the **arena mode** will be rating your model directly, providing you with both quantatitive and verbal feedback 📈
         -   Both the public leaderboard and **user feedback** for your model can be directly downloaded via the `chai_guanaco` package 🧠
@@ -41,118 +46,159 @@
         ## 🚀 Getting Started
         
         **Getting Developer Key**
         
         Join the [competition discord](https://discord.gg/7mXdjAkw2s), introduce yourself and ask for a developer key. Login-based authentication is coming next 🤗
         
         
-        **Submitting A Model**
+        **Installation**
         
         Use [pip](https://github.com/pypa/pip) to install the Chai Guanaco package
         
         ```sh
         pip install chai-guanaco
         ```
         
-        Upload any GPT-J 6B based language model *with a tokenizer* to huggingface, i.e. [EleutherAI/gpt-j-6b](https://huggingface.co/EleutherAI/gpt-j-6b). Read [this guide](https://huggingface.co/docs/transformers/model_sharing) if you are unsure. Click the *Use in Transformers* button in huggingface to get the your huggingface model ID (i.e. "EleutherAI/gpt-j-6b")
+        For one-off authentication run the following in your terminal:
+        
+        ```sh
+        chai-guanaco login
+        ```
+        
+        And pass in your developer key when prompted, you can always logout using `chai-guanaco logout`.
+        
+        **Model Submission**
+        
+        Upload any Llama based language model *with a tokenizer* to huggingface, i.e. [NousResearch/Llama-2-7b-chat-hf](https://huggingface.co/NousResearch/Llama-2-7b-chat-hf). Read [this guide](https://huggingface.co/docs/transformers/model_sharing) if you are unsure. Click the *Use in Transformers* button in huggingface to get the your huggingface model ID (i.e. "NousResearch/Llama-2-7b-chat-hf")
         
         To submit model simply run:
         
         ```python
-        from chai_guanaco.submit import submit_model
+        import chai_guanaco as chai
         
-        model_url = "EleutherAI/gpt-j-6b" # Your model URL
-        developer_key = "CR_XXXX" # Your developer key
-        submission_parameters = {'model_repo': model_url}
-        response = submit_model(submission_parameters, developer_key)
-        submission_id = response['submission_id']
-        print(submission_id)
-        ````
-        which outputs your submission id, unique to your model submission.
+        model_url = "NousResearch/Llama-2-7b-chat-hf" # Your model URL
         
-        To verify the status of a submission, you can use the following command:
+        generation_params = {
+        	'temperature': 1.0,
+        	'repetition_penalty': 1.13,
+        	'top_p': 0.2,
+        	"top_k": 40,
+        	"stopping_words": ['\n'],
+        	"presence_penalty": 0.,
+        	"frequency_penalty": 0.
+        	}
+        submission_parameters = {'model_repo': model_url, 'generation_params': generation_params, 'model_name': 'my-awesome-llama'}
+        
+        submitter = chai.ModelSubmitter()
+        submission_id = submitter.submit(submission_parameters)
+        ```
+        
+        This will display an animation while your model is being deployed, a typical
+        deployment takes approximately 10 minutes. Note the `model_name` parameter is used for show-casing your model on the leaderboard and it should help you with identifying your model
+        
+        
+        **Chat With Your Model Submission**
+        
+        Once your model is deployed, you can verify its behaviour and raw input by running:
         
         ```python
-        from chai_guanaco.submit import get_model_info
+        chatbot = chai.SubmissionChatbot(submission_id)
+        chatbot.chat('nerd_girl', show_model_input=False)
+        ```
+        
+        Here you can have a dialog with one of the bots we have provided. To quit the chat, simply enter "exit". Note that, in order to prevent spamming, each model submission is limited to 1000 chat messages from the Chai Guanaco pip package.
+        
+        You can get a list of avaliable bots by running:
         
-        model_info = get_model_info(submission_id, developer_key)
-        print(model_info)
+        ```python
+        chatbot.show_avaliable_bots()
+        ```
+        
+        Finally, to enter a chat session that prints out the raw input that was fed into your model at each turn of the conversation, you can run:
+        
+        ```python
+        chatbot.chat('nerd_girl', show_model_input=True)
         ```
-        Once the `status` field shows `success` it means your model has been successfully submitted. A submission typically takes around 10 minutes for the tritonisation process to complete.
         
         **Getting User Feedback**
         
         Once your model has been submitted, it is automatically deployed to the Chai Platform where real-life users will evaluate your model performance. To view their feedback, run:
         
         ```python
-        from chai_guanaco.feedback import get_feedback
+        model_feedback = chai.get_feedback(submission_id)
+        model_feedback.sample()
+        ```
+        
+        Which will print out one of the users' conversation, together with meta information associated with the conversation (i.e. rating and user feedback).
         
-        model_feedback = get_feedback(submission_id, developer_key)
-        print(model_feedback)
+        To get all the feedback for your model, run...
+        
+        ```python
+        df = model_feedback.df
+        print(df)
         ```
         
-        Here, you will find a pandas dataframe with all the user feedback for your model, including the conversation each user has had with your model.
+        This outputs a Pandas `DataFrame`, where each row corresponds to a user conversation with your model, together with their feedback.
         
         **Getting Live Leaderboard**
         
-        To see how your model performs against other models, run:
+        To view the public leaderboard used to determine prizes (which only shows the best model submitted by each developer):
         ```python
-        from chai_guanaco.feedback import display_leaderboard
+        df = chai.display_leaderboard(detailed=False)
+        ```
         
-        display_leaderboard(developer_key)
+        To see how your model performs against other models, run:
+        ```python
+        df = chai.display_leaderboard(detailed=True)
         ```
-        which prints out the current leaderboard, with your models positions highlighted
+        which prints out the current leaderboard according to the most recent competition metrics, you can also access raw leaderboard is dumped to `df`
         
         **Re-Submitting Models**
         
         Because it is a competition, you are allowed to test a single model at any given time. However, you can deactivate a model and submit a new one. To do this, simply run:
         
         ```python
-        from chai_guanaco.submit import deactivate_model
-        
-        deactivate_model(submission_id, developer_key)
+        chai.deactivate_model(submission_id)
         ```
         Which will deactive your model, don't worry, all the model feedback will still be saved, it just means the model will no longer be exposed to users. You can then re-submit by repeating the model submission step.
         
         **Retrieve Your Model Submission IDs**
         
         In case you have forgotten your submission ids / want to view all past submissions, run:
         
         ```python
-        from chai_guanaco.submit import get_my_submissions
-        
-        submission_ids = get_my_submissions(developer_key)
+        submission_ids = chai.get_my_submissions()
         print(submission_ids)
         ```
         Here you will see all your model submission_ids along with their status, which is either `failed`, `inactive` or `deployed`.
         
-        **Advanced Submission**
-        
-        You can tweak the model generation sampling parameters by passing the parameters you want during model submission, for example:
+        **Advanced Usage**
+        - This package caches various data, such as your developer key, in the folder `~/.chai-guanaco`. To change this, you can set the environment variable `GUANACO_DATA_DIR` to point to a different folder. You may need to re-run `chai-guanaco login` to update the cached developer key.
+        - You can also access the raw feedback data by running
+        	```python
+        	model_feedback = chai.get_feedback(submission_id)
+        	raw_data = model_feedback.raw_data
+        	```
+        - To submit your model with custom formatting, you can create your own
+          `PromptFormatter`. For more details and examples, please see [here](https://wild-chatter-b52.notion.site/Guanaco-Custom-Formatters-1f64f94b9cf54c819a341988aec5766a).
         
-        ```python
-        from chai_guanaco.submit import submit_model
         
-        generation_params= {"temperature": 1.0, "top_p": 1.0, "top_k": 40, "repetition_penalty": 1.0}
-        submission_parameters = {'model_repo': model_url, 'generation_params': generation_params}
-        response = submit_model(submission_parameters, developer_key)
-        ```
         
         ## Resources
         |                                                                        |                                                                                                 |
         | ---------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------|
         | 📒 [Fine tuning guide](https://huggingface.co/docs/transformers/training) | Guide on language model finetuning                                                           |
         | 💾 [Datasets](https://dataset-ideas.tiiny.site/) | Curated list of open-sourced datasets to get started with finetuning                                                  |
-        | 💖 [Guanaco Discord](https://haystack.deepset.ai/tutorials)                   | Our Guanaco competition discord                                                          |
+        | 💖 [Guanaco Discord](https://discord.gg/7mXdjAkw2s)                   | Our Guanaco competition discord                                                          |
         |🚀 [Deepspeed Guide](https://huggingface.co/docs/transformers/main_classes/deepspeed)     | Guide for training with Deepspeed (faster training without GPU bottleneck)    |
-        |💬 [Example Conversations](https://huggingface.co/docs/transformers/main_classes/deepspeed)     | Here you can find 1000 example conversations from the Chai Platform     |
+        |💬 [Example Conversations](https://huggingface.co/datasets/ChaiML/100_example_conversations)     | Here you can find 100 example conversations from the Chai Platform     |
         | ⚒️ [Build with us](https://boards.greenhouse.io/nexus/jobs/5319721003)| If you think what we are building is cool, join us!|
         
         
         ## 🦙 Hosted & Sponsored By
         
-        <a href="https://www.chai-research.com/"><img src="https://i.imgur.com/optjNAw.png" alt="Chai Logo" height="70"/></a>
+        <a href="https://www.chai-research.com/"><img src="https://imgur.com/u3rOQDJ.png" alt="Chai Logo" height="90"/></a>
         
         <a href="https://www.coreweave.com/"><img src="https://imgur.com/oJyuH8q.png" alt="Coreweave Logo" height="70"/></a>
         
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `chai-guanaco-1.1.1/setup.py` & `chai-guanaco-1.1.2/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,35 @@
 from pathlib import Path
 import os
 from setuptools import find_packages, setup
 
 current_dir = Path(__file__).parent
 long_description = (current_dir / "README.md").read_text()
 
+with open('requirements.txt') as f:
+    requirements = f.read().splitlines()
+
 if os.environ.get('CI_COMMIT_TAG', None):
     version = os.environ['CI_COMMIT_TAG']
 else:
-    version = "1.1.1"
+    version = "1.1.2"
 
 setup(
     name='chai-guanaco',
     version=version,
     description='Chai Guanaco',
     author='Chai Research Corp.',
     author_email='hello@chai-research.com',
     license='MIT',
-    packages=["chai_guanaco"],
-    package_dir={"chai_guanaco": "./src/chai_guanaco/"},
+    packages=['chai_guanaco'],
+    package_dir={"": "src"},
+    package_data={"chai_guanaco": ["resources/*"]},
     url='https://www.chai-research.com',
     zip_safe=False,
     long_description=long_description,
     long_description_content_type='text/markdown',
-    install_requires=['requests']
+    install_requires=requirements,
+    include_package_data=True,
+    entry_points={
+        'console_scripts': ['chai-guanaco=chai_guanaco.login_cli:cli'],
+    },
 )
```

