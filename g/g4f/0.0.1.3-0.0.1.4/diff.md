# Comparing `tmp/g4f-0.0.1.3.tar.gz` & `tmp/g4f-0.0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "g4f-0.0.1.3.tar", last modified: Fri Jul 21 20:44:02 2023, max compression
+gzip compressed data, was "g4f-0.0.1.4.tar", last modified: Mon Aug  7 11:40:03 2023, max compression
```

## Comparing `g4f-0.0.1.3.tar` & `g4f-0.0.1.4.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxr-xr-x   0 tek        (501) staff       (20)        0 2023-07-21 20:44:02.692022 g4f-0.0.1.3/
--rw-r--r--   0 tek        (501) staff       (20)    35149 2023-04-16 23:05:26.000000 g4f-0.0.1.3/LICENSE
--rw-r--r--   0 tek        (501) staff       (20)    19188 2023-07-21 20:44:02.691728 g4f-0.0.1.3/PKG-INFO
--rw-r--r--   0 tek        (501) staff       (20)    18440 2023-07-17 23:18:39.000000 g4f-0.0.1.3/README.md
-drwxr-xr-x   0 tek        (501) staff       (20)        0 2023-07-21 20:44:02.683951 g4f-0.0.1.3/g4f/
-drwxr-xr-x   0 tek        (501) staff       (20)        0 2023-07-21 20:44:02.685596 g4f-0.0.1.3/g4f/Provider/
--rw-r--r--   0 tek        (501) staff       (20)      501 2023-07-16 19:31:22.000000 g4f-0.0.1.3/g4f/Provider/Provider.py
-drwxr-xr-x   0 tek        (501) staff       (20)        0 2023-07-21 20:44:02.691400 g4f-0.0.1.3/g4f/Provider/Providers/
--rw-r--r--   0 tek        (501) staff       (20)     1411 2023-07-16 19:00:36.000000 g4f-0.0.1.3/g4f/Provider/Providers/AItianhu.py
--rw-r--r--   0 tek        (501) staff       (20)     1362 2023-07-16 18:59:46.000000 g4f-0.0.1.3/g4f/Provider/Providers/Acytoo.py
--rw-r--r--   0 tek        (501) staff       (20)     1243 2023-07-16 19:00:33.000000 g4f-0.0.1.3/g4f/Provider/Providers/AiService.py
--rw-r--r--   0 tek        (501) staff       (20)     1578 2023-07-16 19:00:07.000000 g4f-0.0.1.3/g4f/Provider/Providers/Aichat.py
--rw-r--r--   0 tek        (501) staff       (20)     3102 2023-07-16 19:00:12.000000 g4f-0.0.1.3/g4f/Provider/Providers/Ails.py
--rw-r--r--   0 tek        (501) staff       (20)     2618 2023-07-16 19:01:02.000000 g4f-0.0.1.3/g4f/Provider/Providers/Bard.py
--rw-r--r--   0 tek        (501) staff       (20)    13017 2023-07-16 19:01:09.000000 g4f-0.0.1.3/g4f/Provider/Providers/Bing.py
--rw-r--r--   0 tek        (501) staff       (20)      952 2023-07-16 19:01:46.000000 g4f-0.0.1.3/g4f/Provider/Providers/BingHuan.py
--rw-r--r--   0 tek        (501) staff       (20)     2033 2023-07-16 19:01:49.000000 g4f-0.0.1.3/g4f/Provider/Providers/ChatgptAi.py
--rw-r--r--   0 tek        (501) staff       (20)     3763 2023-07-16 19:02:36.000000 g4f-0.0.1.3/g4f/Provider/Providers/ChatgptLogin.py
--rw-r--r--   0 tek        (501) staff       (20)     1451 2023-07-16 19:02:54.000000 g4f-0.0.1.3/g4f/Provider/Providers/DeepAi.py
--rw-r--r--   0 tek        (501) staff       (20)     2229 2023-07-21 20:42:14.000000 g4f-0.0.1.3/g4f/Provider/Providers/DfeHub.py
--rw-r--r--   0 tek        (501) staff       (20)     1977 2023-07-16 19:03:36.000000 g4f-0.0.1.3/g4f/Provider/Providers/EasyChat.py
--rw-r--r--   0 tek        (501) staff       (20)     1209 2023-07-16 19:03:41.000000 g4f-0.0.1.3/g4f/Provider/Providers/Forefront.py
--rw-r--r--   0 tek        (501) staff       (20)     2178 2023-07-16 19:03:43.000000 g4f-0.0.1.3/g4f/Provider/Providers/GetGpt.py
--rw-r--r--   0 tek        (501) staff       (20)     3761 2023-07-16 19:07:34.000000 g4f-0.0.1.3/g4f/Provider/Providers/H2o.py
--rw-r--r--   0 tek        (501) staff       (20)     1728 2023-07-16 19:08:58.000000 g4f-0.0.1.3/g4f/Provider/Providers/Liaobots.py
--rw-r--r--   0 tek        (501) staff       (20)     1396 2023-07-16 19:09:35.000000 g4f-0.0.1.3/g4f/Provider/Providers/Lockchat.py
--rw-r--r--   0 tek        (501) staff       (20)      945 2023-07-17 00:24:27.000000 g4f-0.0.1.3/g4f/Provider/Providers/Theb.py
--rw-r--r--   0 tek        (501) staff       (20)    17642 2023-07-16 19:30:13.000000 g4f-0.0.1.3/g4f/Provider/Providers/Vercel.py
--rw-r--r--   0 tek        (501) staff       (20)     2640 2023-07-16 19:30:16.000000 g4f-0.0.1.3/g4f/Provider/Providers/Wewordle.py
--rw-r--r--   0 tek        (501) staff       (20)      654 2023-07-16 19:30:07.000000 g4f-0.0.1.3/g4f/Provider/Providers/You.py
--rw-r--r--   0 tek        (501) staff       (20)     1394 2023-07-16 19:30:48.000000 g4f-0.0.1.3/g4f/Provider/Providers/Yqcloud.py
--rw-r--r--   0 tek        (501) staff       (20)        0 2023-07-21 20:42:14.000000 g4f-0.0.1.3/g4f/Provider/Providers/__init__.py
--rw-r--r--   0 tek        (501) staff       (20)      353 2023-07-16 18:49:10.000000 g4f-0.0.1.3/g4f/Provider/__init__.py
--rw-r--r--   0 tek        (501) staff       (20)     1691 2023-07-16 19:31:26.000000 g4f-0.0.1.3/g4f/__init__.py
--rw-r--r--   0 tek        (501) staff       (20)     7561 2023-07-16 18:58:49.000000 g4f-0.0.1.3/g4f/models.py
--rw-r--r--   0 tek        (501) staff       (20)      110 2023-07-16 17:53:33.000000 g4f-0.0.1.3/g4f/typing.py
--rw-r--r--   0 tek        (501) staff       (20)     1700 2023-07-16 17:53:33.000000 g4f-0.0.1.3/g4f/utils.py
-drwxr-xr-x   0 tek        (501) staff       (20)        0 2023-07-21 20:44:02.685097 g4f-0.0.1.3/g4f.egg-info/
--rw-r--r--   0 tek        (501) staff       (20)    19188 2023-07-21 20:44:02.000000 g4f-0.0.1.3/g4f.egg-info/PKG-INFO
--rw-r--r--   0 tek        (501) staff       (20)     1075 2023-07-21 20:44:02.000000 g4f-0.0.1.3/g4f.egg-info/SOURCES.txt
--rw-r--r--   0 tek        (501) staff       (20)        1 2023-07-21 20:44:02.000000 g4f-0.0.1.3/g4f.egg-info/dependency_links.txt
--rw-r--r--   0 tek        (501) staff       (20)       84 2023-07-21 20:44:02.000000 g4f-0.0.1.3/g4f.egg-info/requires.txt
--rw-r--r--   0 tek        (501) staff       (20)        4 2023-07-21 20:44:02.000000 g4f-0.0.1.3/g4f.egg-info/top_level.txt
--rw-r--r--   0 tek        (501) staff       (20)       38 2023-07-21 20:44:02.692107 g4f-0.0.1.3/setup.cfg
--rw-r--r--   0 tek        (501) staff       (20)     1318 2023-07-21 20:43:58.000000 g4f-0.0.1.3/setup.py
+drwxr-xr-x   0 tek        (501) staff       (20)        0 2023-08-07 11:40:03.666060 g4f-0.0.1.4/
+-rw-r--r--   0 tek        (501) staff       (20)    35149 2023-04-16 23:05:26.000000 g4f-0.0.1.4/LICENSE
+-rw-r--r--   0 tek        (501) staff       (20)    19390 2023-08-07 11:40:03.665315 g4f-0.0.1.4/PKG-INFO
+-rw-r--r--   0 tek        (501) staff       (20)    18642 2023-08-07 11:38:29.000000 g4f-0.0.1.4/README.md
+drwxr-xr-x   0 tek        (501) staff       (20)        0 2023-08-07 11:40:03.656299 g4f-0.0.1.4/g4f/
+drwxr-xr-x   0 tek        (501) staff       (20)        0 2023-08-07 11:40:03.658063 g4f-0.0.1.4/g4f/Provider/
+-rw-r--r--   0 tek        (501) staff       (20)      501 2023-07-16 19:31:22.000000 g4f-0.0.1.4/g4f/Provider/Provider.py
+drwxr-xr-x   0 tek        (501) staff       (20)        0 2023-08-07 11:40:03.665009 g4f-0.0.1.4/g4f/Provider/Providers/
+-rw-r--r--   0 tek        (501) staff       (20)     1459 2023-07-24 01:34:22.000000 g4f-0.0.1.4/g4f/Provider/Providers/AItianhu.py
+-rw-r--r--   0 tek        (501) staff       (20)     1362 2023-07-16 18:59:46.000000 g4f-0.0.1.4/g4f/Provider/Providers/Acytoo.py
+-rw-r--r--   0 tek        (501) staff       (20)     1243 2023-07-16 19:00:33.000000 g4f-0.0.1.4/g4f/Provider/Providers/AiService.py
+-rw-r--r--   0 tek        (501) staff       (20)     1578 2023-07-16 19:00:07.000000 g4f-0.0.1.4/g4f/Provider/Providers/Aichat.py
+-rw-r--r--   0 tek        (501) staff       (20)     3327 2023-08-07 11:38:29.000000 g4f-0.0.1.4/g4f/Provider/Providers/Ails.py
+-rw-r--r--   0 tek        (501) staff       (20)     2618 2023-07-16 19:01:02.000000 g4f-0.0.1.4/g4f/Provider/Providers/Bard.py
+-rw-r--r--   0 tek        (501) staff       (20)    13076 2023-08-07 11:38:29.000000 g4f-0.0.1.4/g4f/Provider/Providers/Bing.py
+-rw-r--r--   0 tek        (501) staff       (20)      952 2023-07-16 19:01:46.000000 g4f-0.0.1.4/g4f/Provider/Providers/BingHuan.py
+-rw-r--r--   0 tek        (501) staff       (20)     2033 2023-07-16 19:01:49.000000 g4f-0.0.1.4/g4f/Provider/Providers/ChatgptAi.py
+-rw-r--r--   0 tek        (501) staff       (20)     3790 2023-07-24 01:34:22.000000 g4f-0.0.1.4/g4f/Provider/Providers/ChatgptLogin.py
+-rw-r--r--   0 tek        (501) staff       (20)     3252 2023-08-07 11:38:29.000000 g4f-0.0.1.4/g4f/Provider/Providers/DeepAi.py
+-rw-r--r--   0 tek        (501) staff       (20)     2342 2023-07-24 01:34:22.000000 g4f-0.0.1.4/g4f/Provider/Providers/DfeHub.py
+-rw-r--r--   0 tek        (501) staff       (20)     2090 2023-07-24 01:34:22.000000 g4f-0.0.1.4/g4f/Provider/Providers/EasyChat.py
+-rw-r--r--   0 tek        (501) staff       (20)     1209 2023-07-16 19:03:41.000000 g4f-0.0.1.4/g4f/Provider/Providers/Forefront.py
+-rw-r--r--   0 tek        (501) staff       (20)     2178 2023-07-16 19:03:43.000000 g4f-0.0.1.4/g4f/Provider/Providers/GetGpt.py
+-rw-r--r--   0 tek        (501) staff       (20)     3761 2023-07-16 19:07:34.000000 g4f-0.0.1.4/g4f/Provider/Providers/H2o.py
+-rw-r--r--   0 tek        (501) staff       (20)     1728 2023-07-16 19:08:58.000000 g4f-0.0.1.4/g4f/Provider/Providers/Liaobots.py
+-rw-r--r--   0 tek        (501) staff       (20)     1404 2023-07-24 01:34:22.000000 g4f-0.0.1.4/g4f/Provider/Providers/Lockchat.py
+-rw-r--r--   0 tek        (501) staff       (20)      945 2023-07-17 00:24:27.000000 g4f-0.0.1.4/g4f/Provider/Providers/Theb.py
+-rw-r--r--   0 tek        (501) staff       (20)    14250 2023-07-24 01:36:21.000000 g4f-0.0.1.4/g4f/Provider/Providers/Vercel.py
+-rw-r--r--   0 tek        (501) staff       (20)     2640 2023-07-16 19:30:16.000000 g4f-0.0.1.4/g4f/Provider/Providers/Wewordle.py
+-rw-r--r--   0 tek        (501) staff       (20)      654 2023-07-16 19:30:07.000000 g4f-0.0.1.4/g4f/Provider/Providers/You.py
+-rw-r--r--   0 tek        (501) staff       (20)     1394 2023-07-16 19:30:48.000000 g4f-0.0.1.4/g4f/Provider/Providers/Yqcloud.py
+-rw-r--r--   0 tek        (501) staff       (20)        0 2023-07-21 20:42:14.000000 g4f-0.0.1.4/g4f/Provider/Providers/__init__.py
+-rw-r--r--   0 tek        (501) staff       (20)     1506 2023-08-07 11:38:29.000000 g4f-0.0.1.4/g4f/Provider/Providers/opchatgpts.py
+-rw-r--r--   0 tek        (501) staff       (20)      369 2023-08-07 11:38:29.000000 g4f-0.0.1.4/g4f/Provider/__init__.py
+-rw-r--r--   0 tek        (501) staff       (20)     1680 2023-08-07 11:38:29.000000 g4f-0.0.1.4/g4f/__init__.py
+-rw-r--r--   0 tek        (501) staff       (20)     5591 2023-08-07 11:38:29.000000 g4f-0.0.1.4/g4f/models.py
+-rw-r--r--   0 tek        (501) staff       (20)      110 2023-07-16 17:53:33.000000 g4f-0.0.1.4/g4f/typing.py
+-rw-r--r--   0 tek        (501) staff       (20)     1700 2023-07-16 17:53:33.000000 g4f-0.0.1.4/g4f/utils.py
+drwxr-xr-x   0 tek        (501) staff       (20)        0 2023-08-07 11:40:03.657656 g4f-0.0.1.4/g4f.egg-info/
+-rw-r--r--   0 tek        (501) staff       (20)    19390 2023-08-07 11:40:03.000000 g4f-0.0.1.4/g4f.egg-info/PKG-INFO
+-rw-r--r--   0 tek        (501) staff       (20)     1112 2023-08-07 11:40:03.000000 g4f-0.0.1.4/g4f.egg-info/SOURCES.txt
+-rw-r--r--   0 tek        (501) staff       (20)        1 2023-08-07 11:40:03.000000 g4f-0.0.1.4/g4f.egg-info/dependency_links.txt
+-rw-r--r--   0 tek        (501) staff       (20)       84 2023-08-07 11:40:03.000000 g4f-0.0.1.4/g4f.egg-info/requires.txt
+-rw-r--r--   0 tek        (501) staff       (20)        4 2023-08-07 11:40:03.000000 g4f-0.0.1.4/g4f.egg-info/top_level.txt
+-rw-r--r--   0 tek        (501) staff       (20)       38 2023-08-07 11:40:03.666256 g4f-0.0.1.4/setup.cfg
+-rw-r--r--   0 tek        (501) staff       (20)     1318 2023-08-07 11:39:56.000000 g4f-0.0.1.4/setup.py
```

### Comparing `g4f-0.0.1.3/LICENSE` & `g4f-0.0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `g4f-0.0.1.3/PKG-INFO` & `g4f-0.0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: g4f
-Version: 0.0.1.3
+Version: 0.0.1.4
 Summary: The official gpt4free repository | various collection of powerful language models
 Author: Tekky
 Author-email: <support@g4f.ai>
 Keywords: python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
-![image](https://github.com/onlpx/gpt4free-v2/assets/98614666/7886223b-c1d1-4260-82aa-da5741f303bb)
+
+![248433934-7886223b-c1d1-4260-82aa-da5741f303bb](https://github.com/xtekky/gpt4free/assets/98614666/ea012c87-76e0-496a-8ac4-e2de090cc6c9)
 
 By using this repository or any code related to it, you agree to the [legal notice](./LEGAL_NOTICE.md). The author is not responsible for any copies, forks, or reuploads made by other users. This is the author's only account and repository. To prevent impersonation or irresponsible actions, you may comply with the GNU GPL license this Repository uses.
 
 This (quite censored) New Version of gpt4free, was just released, it may contain bugs, open an issue or contribute a PR when encountering one, some features were disabled.
 Docker is for now not available but I would be happy if someone contributes a PR. The g4f GUI will be uploaded soon enough.
 
 ### New
@@ -107,15 +108,15 @@
 response = g4f.ChatCompletion.create(model='gpt-3.5-turbo', messages=[
                                      {"role": "user", "content": "Hello world"}], stream=True)
 
 for message in response:
     print(message)
 
 # normal response
-response = g4f.ChatCompletion.create(model=g4f.Model.gpt_4, messages=[
+response = g4f.ChatCompletion.create(model=g4f.models.gpt_4, messages=[
                                      {"role": "user", "content": "hi"}]) # alterative model setting
 
 print(response)
 
 
 # Set with provider
 response = g4f.ChatCompletion.create(model='gpt-3.5-turbo', provider=g4f.Provider.Forefront, messages=[
@@ -199,14 +200,15 @@
 | [free.easychat.work](https://free.easychat.work) | `g4f.Provider.EasyChat` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
 | [chat.acytoo.com](https://chat.acytoo.com/api/completions) | `g4f.Provider.Acytoo` | ✔️ | ❌ | ❌ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
 | [chat.dfehub.com](https://chat.dfehub.com/api/chat) | `g4f.Provider.DfeHub` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
 | [aiservice.vercel.app](https://aiservice.vercel.app/api/chat/answer) | `g4f.Provider.AiService` | ✔️ | ❌ | ❌ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
 | [b.ai-huan.xyz](https://b.ai-huan.xyz) | `g4f.Provider.BingHuan` | ✔️ | ✔️ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
 | [wewordle.org](https://wewordle.org/gptapi/v1/android/turbo) | `g4f.Provider.Wewordle` | ✔️ | ❌ | ❌ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
 | [chatgpt.ai](https://chatgpt.ai/gpt-4/) | `g4f.Provider.ChatgptAi` | ❌ | ✔️ | ❌ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
+| [opchatgpts.net](https://opchatgpts.net) | `g4f.Provider.opchatgpts` | ✔️ | ❌ | ❌ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
 
 
 ### Other Models
 
 | Model| Base Provider | Provider | Website |
 | ------- | ----------- | ---- |---- |
 | palm2 | Google | `g4f.Provider.Bard` | [bard.google.com](https://bard.google.com/) |
```

### Comparing `g4f-0.0.1.3/README.md` & `g4f-0.0.1.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-![image](https://github.com/onlpx/gpt4free-v2/assets/98614666/7886223b-c1d1-4260-82aa-da5741f303bb)
+
+![248433934-7886223b-c1d1-4260-82aa-da5741f303bb](https://github.com/xtekky/gpt4free/assets/98614666/ea012c87-76e0-496a-8ac4-e2de090cc6c9)
 
 By using this repository or any code related to it, you agree to the [legal notice](./LEGAL_NOTICE.md). The author is not responsible for any copies, forks, or reuploads made by other users. This is the author's only account and repository. To prevent impersonation or irresponsible actions, you may comply with the GNU GPL license this Repository uses.
 
 This (quite censored) New Version of gpt4free, was just released, it may contain bugs, open an issue or contribute a PR when encountering one, some features were disabled.
 Docker is for now not available but I would be happy if someone contributes a PR. The g4f GUI will be uploaded soon enough.
 
 ### New
@@ -90,15 +91,15 @@
 response = g4f.ChatCompletion.create(model='gpt-3.5-turbo', messages=[
                                      {"role": "user", "content": "Hello world"}], stream=True)
 
 for message in response:
     print(message)
 
 # normal response
-response = g4f.ChatCompletion.create(model=g4f.Model.gpt_4, messages=[
+response = g4f.ChatCompletion.create(model=g4f.models.gpt_4, messages=[
                                      {"role": "user", "content": "hi"}]) # alterative model setting
 
 print(response)
 
 
 # Set with provider
 response = g4f.ChatCompletion.create(model='gpt-3.5-turbo', provider=g4f.Provider.Forefront, messages=[
@@ -182,14 +183,15 @@
 | [free.easychat.work](https://free.easychat.work) | `g4f.Provider.EasyChat` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
 | [chat.acytoo.com](https://chat.acytoo.com/api/completions) | `g4f.Provider.Acytoo` | ✔️ | ❌ | ❌ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
 | [chat.dfehub.com](https://chat.dfehub.com/api/chat) | `g4f.Provider.DfeHub` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
 | [aiservice.vercel.app](https://aiservice.vercel.app/api/chat/answer) | `g4f.Provider.AiService` | ✔️ | ❌ | ❌ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
 | [b.ai-huan.xyz](https://b.ai-huan.xyz) | `g4f.Provider.BingHuan` | ✔️ | ✔️ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
 | [wewordle.org](https://wewordle.org/gptapi/v1/android/turbo) | `g4f.Provider.Wewordle` | ✔️ | ❌ | ❌ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
 | [chatgpt.ai](https://chatgpt.ai/gpt-4/) | `g4f.Provider.ChatgptAi` | ❌ | ✔️ | ❌ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
+| [opchatgpts.net](https://opchatgpts.net) | `g4f.Provider.opchatgpts` | ✔️ | ❌ | ❌ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
 
 
 ### Other Models
 
 | Model| Base Provider | Provider | Website |
 | ------- | ----------- | ---- |---- |
 | palm2 | Google | `g4f.Provider.Bard` | [bard.google.com](https://bard.google.com/) |
```

### Comparing `g4f-0.0.1.3/g4f/Provider/Providers/AItianhu.py` & `g4f-0.0.1.4/g4f/Provider/Providers/AItianhu.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,16 +18,16 @@
     headers = {
         "user-agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36"
     }
     data = {
         "prompt": base,
         "options": {},
         "systemMessage": "You are ChatGPT, a large language model trained by OpenAI. Follow the user's instructions carefully. Respond using markdown.",
-        "temperature": 0.8,
-        "top_p": 1
+        "temperature": kwargs.get("temperature", 0.8),
+        "top_p": kwargs.get("top_p", 1)
     }
     response = requests.post(url, headers=headers, json=data)
     if response.status_code == 200:
         lines = response.text.strip().split('\n')
         res = json.loads(lines[-1])
         yield res['text']
     else:
```

### Comparing `g4f-0.0.1.3/g4f/Provider/Providers/Acytoo.py` & `g4f-0.0.1.4/g4f/Provider/Providers/Acytoo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.0.1.3/g4f/Provider/Providers/AiService.py` & `g4f-0.0.1.4/g4f/Provider/Providers/AiService.py`

 * *Files identical despite different names*

### Comparing `g4f-0.0.1.3/g4f/Provider/Providers/Aichat.py` & `g4f-0.0.1.4/g4f/Provider/Providers/Aichat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.0.1.3/g4f/Provider/Providers/Ails.py` & `g4f-0.0.1.4/g4f/Provider/Providers/Ails.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,25 +33,27 @@
 
     def format_timestamp(timestamp: int) -> str:
 
         e = timestamp
         n = e % 10
         r = n + 1 if n % 2 == 0 else n
         return str(e - n + r)
-
+    def getV():
+        crossref = requests.get("https://ai.ls"+ requests.get("https://ai.ls/?chat=1").text.split('crossorigin href="')[1].split('"')[0]).text.split('G4="')[1].split('"')[0]
+        return crossref
 
 def _create_completion(model: str, messages: list, temperature: float = 0.6, stream: bool = False, **kwargs):
 
     headers = {
         'authority': 'api.caipacity.com',
         'accept': '*/*',
         'accept-language': 'en,fr-FR;q=0.9,fr;q=0.8,es-ES;q=0.7,es;q=0.6,en-US;q=0.5,am;q=0.4,de;q=0.3',
         'authorization': 'Bearer free',
         'client-id': str(uuid.uuid4()),
-        'client-v': '0.1.249',
+        'client-v': Utils.getV(),
         'content-type': 'application/json',
         'origin': 'https://ai.ls',
         'referer': 'https://ai.ls/',
         'sec-ch-ua': '"Not.A/Brand";v="8", "Chromium";v="114", "Google Chrome";v="114"',
         'sec-ch-ua-mobile': '?0',
         'sec-ch-ua-platform': '"Windows"',
         'sec-fetch-dest': 'empty',
@@ -71,23 +73,23 @@
         't': timestamp,
         's': Utils.hash({
             't': timestamp,
             'm': messages[-1]['content']})}
 
     json_data = json.dumps(separators=(',', ':'), obj={
         'model': 'gpt-3.5-turbo',
-        'temperature': 0.6,
+        'temperature': temperature,
         'stream': True,
          'messages': messages} | sig)
 
     response = requests.post('https://api.caipacity.com/v1/chat/completions', 
                              headers=headers, data=json_data, stream=True)
 
     for token in response.iter_lines():
         if b'content' in token:
             completion_chunk = json.loads(token.decode().replace('data: ', ''))
             token = completion_chunk['choices'][0]['delta'].get('content')
             if token != None:
                 yield token
 
 params = f'g4f.Providers.{os.path.basename(__file__)[:-3]} supports: ' + \
-    '(%s)' % ', '.join([f"{name}: {get_type_hints(_create_completion)[name].__name__}" for name in _create_completion.__code__.co_varnames[:_create_completion.__code__.co_argcount]])
+    '(%s)' % ', '.join([f"{name}: {get_type_hints(_create_completion)[name].__name__}" for name in _create_completion.__code__.co_varnames[:_create_completion.__code__.co_argcount]])
```

### Comparing `g4f-0.0.1.3/g4f/Provider/Providers/Bard.py` & `g4f-0.0.1.4/g4f/Provider/Providers/Bard.py`

 * *Files identical despite different names*

### Comparing `g4f-0.0.1.3/g4f/Provider/Providers/Bing.py` & `g4f-0.0.1.4/g4f/Provider/Providers/Bing.py`

 * *Files 2% similar despite different names*

```diff
@@ -301,27 +301,28 @@
                 final = True
                 if wss and not wss.closed:
                     await wss.close()
                 if session and not session.closed:
                     await session.close()
 
 
-def run(generator):
-    loop = asyncio.get_event_loop()
-    gen = generator.__aiter__()
-
-    while True:
-        try:
-            next_val = loop.run_until_complete(gen.__anext__())
-            yield next_val
+def run(generator):  
+    loop = asyncio.new_event_loop()  
+    asyncio.set_event_loop(loop)  
+    gen = generator.__aiter__()  
+  
+    while True:  
+        try:  
+            next_val = loop.run_until_complete(gen.__anext__())  
+            yield next_val  
+  
+        except StopAsyncIteration:  
+            break  
+    #print('Done')  
 
-        except StopAsyncIteration:
-            break
-
-    #print('Done')
 
 
 def convert(messages):
     context = ""
 
     for message in messages:
         context += "[%s](#message)\n%s\n\n" % (message['role'],
```

### Comparing `g4f-0.0.1.3/g4f/Provider/Providers/BingHuan.py` & `g4f-0.0.1.4/g4f/Provider/Providers/BingHuan.py`

 * *Files identical despite different names*

### Comparing `g4f-0.0.1.3/g4f/Provider/Providers/ChatgptAi.py` & `g4f-0.0.1.4/g4f/Provider/Providers/ChatgptAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.0.1.3/g4f/Provider/Providers/ChatgptLogin.py` & `g4f-0.0.1.4/g4f/Provider/Providers/ChatgptLogin.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         'prompt': 'Converse as if you were an AI assistant. Be friendly, creative.',
         'context': 'Converse as if you were an AI assistant. Be friendly, creative.',
         'messages': conversation,
         'newMessage': messages[-1]['content'],
         'userName': '<div class="mwai-name-text">User:</div>',
         'aiName': '<div class="mwai-name-text">AI:</div>',
         'model': 'gpt-3.5-turbo',
-        'temperature': 0.8,
+        'temperature': kwargs.get('temperature', 0.8),
         'maxTokens': 1024,
         'maxResults': 1,
         'apiKey': '',
         'service': 'openai',
         'embeddingsIndex': '',
         'stop': '',
         'clientId': os.urandom(6).hex()
```

### Comparing `g4f-0.0.1.3/g4f/Provider/Providers/DfeHub.py` & `g4f-0.0.1.4/g4f/Provider/Providers/DfeHub.py`

 * *Files 15% similar despite different names*

```diff
@@ -28,18 +28,18 @@
         'user-agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36',
         'x-requested-with': 'XMLHttpRequest',
     }
 
     json_data = {
         'messages': messages,
         'model': 'gpt-3.5-turbo',
-        'temperature': 0.5,
-        'presence_penalty': 0,
-        'frequency_penalty': 0,
-        'top_p': 1,
+        'temperature': kwargs.get('temperature', 0.5),
+        'presence_penalty': kwargs.get('presence_penalty', 0),
+        'frequency_penalty': kwargs.get('frequency_penalty', 0),
+        'top_p': kwargs.get('top_p', 1),
         "stream": True,
     }
     response = requests.post('https://chat.dfehub.com/api/openai/v1/chat/completions',
         headers=headers, json=json_data)
     
     for chunk in response.iter_lines():
         if b'detail' in chunk:
```

### Comparing `g4f-0.0.1.3/g4f/Provider/Providers/EasyChat.py` & `g4f-0.0.1.4/g4f/Provider/Providers/EasyChat.py`

 * *Files 13% similar despite different names*

```diff
@@ -30,18 +30,18 @@
         'x-requested-with': 'XMLHttpRequest',
     }
 
     json_data = {
         'messages': messages,
         'stream': True,
         'model': model,
-        'temperature': 0.5,
-        'presence_penalty': 0,
-        'frequency_penalty': 0,
-        'top_p': 1,
+        'temperature': kwargs.get('temperature', 0.5),
+        'presence_penalty': kwargs.get('presence_penalty', 0),
+        'frequency_penalty': kwargs.get('frequency_penalty', 0),
+        'top_p': kwargs.get('top_p', 1),
     }
 
     response = requests.post('https://free.easychat.work/api/openai/v1/chat/completions',
         headers=headers, json=json_data)
     
     for chunk in response.iter_lines():
         if b'content' in chunk:
```

### Comparing `g4f-0.0.1.3/g4f/Provider/Providers/Forefront.py` & `g4f-0.0.1.4/g4f/Provider/Providers/Forefront.py`

 * *Files identical despite different names*

### Comparing `g4f-0.0.1.3/g4f/Provider/Providers/GetGpt.py` & `g4f-0.0.1.4/g4f/Provider/Providers/GetGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.0.1.3/g4f/Provider/Providers/H2o.py` & `g4f-0.0.1.4/g4f/Provider/Providers/H2o.py`

 * *Files identical despite different names*

### Comparing `g4f-0.0.1.3/g4f/Provider/Providers/Liaobots.py` & `g4f-0.0.1.4/g4f/Provider/Providers/Liaobots.py`

 * *Files identical despite different names*

### Comparing `g4f-0.0.1.3/g4f/Provider/Providers/Lockchat.py` & `g4f-0.0.1.4/g4f/Provider/Providers/Lockchat.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 supports_stream = True
 needs_auth = False
 working = False
 
 def _create_completion(model: str, messages: list, stream: bool, temperature: float = 0.7, **kwargs):
 
     payload = {
-        "temperature": 0.7,
+        "temperature": temperature,
         "messages": messages,
         "model": model,
         "stream": True,
     }
     headers = {
         "user-agent": "ChatX/39 CFNetwork/1408.0.4 Darwin/22.5.0",
     }
```

### Comparing `g4f-0.0.1.3/g4f/Provider/Providers/Theb.py` & `g4f-0.0.1.4/g4f/Provider/Providers/Theb.py`

 * *Files identical despite different names*

### Comparing `g4f-0.0.1.3/g4f/Provider/Providers/Wewordle.py` & `g4f-0.0.1.4/g4f/Provider/Providers/Wewordle.py`

 * *Files identical despite different names*

### Comparing `g4f-0.0.1.3/g4f/Provider/Providers/You.py` & `g4f-0.0.1.4/g4f/Provider/Providers/You.py`

 * *Files identical despite different names*

### Comparing `g4f-0.0.1.3/g4f/Provider/Providers/Yqcloud.py` & `g4f-0.0.1.4/g4f/Provider/Providers/Yqcloud.py`

 * *Files identical despite different names*

### Comparing `g4f-0.0.1.3/g4f/__init__.py` & `g4f-0.0.1.4/g4f/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import sys
 from . import Provider
-from g4f.models import Model, ModelUtils
+from g4f import models
 
 logging = False
 
 class ChatCompletion:
     @staticmethod
-    def create(model: Model.model or str, messages: list, provider: Provider.Provider = None, stream: bool = False, auth: str = False, **kwargs):
+    def create(model: models.Model | str, messages: list, provider: Provider.Provider = None, stream: bool = False, auth: str = False, **kwargs):
         kwargs['auth'] = auth
         if provider and provider.working == False:
             return f'{provider.__name__} is not working'
 
         if provider and provider.needs_auth and not auth:
             print(
                 f'ValueError: {provider.__name__} requires authentication (use auth="cookie or token or jwt ..." param)', file=sys.stderr)
             sys.exit(1)
 
         try:
             if isinstance(model, str):
                 try:
-                    model = ModelUtils.convert[model]
+                    model = models.ModelUtils.convert[model]
                 except KeyError:
                     raise Exception(f'The model: {model} does not exist')
 
             engine = model.best_provider if not provider else provider
 
             if not engine.supports_stream and stream == True:
                 print(
```

### Comparing `g4f-0.0.1.3/g4f/utils.py` & `g4f-0.0.1.4/g4f/utils.py`

 * *Files identical despite different names*

### Comparing `g4f-0.0.1.3/g4f.egg-info/PKG-INFO` & `g4f-0.0.1.4/g4f.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: g4f
-Version: 0.0.1.3
+Version: 0.0.1.4
 Summary: The official gpt4free repository | various collection of powerful language models
 Author: Tekky
 Author-email: <support@g4f.ai>
 Keywords: python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
-![image](https://github.com/onlpx/gpt4free-v2/assets/98614666/7886223b-c1d1-4260-82aa-da5741f303bb)
+
+![248433934-7886223b-c1d1-4260-82aa-da5741f303bb](https://github.com/xtekky/gpt4free/assets/98614666/ea012c87-76e0-496a-8ac4-e2de090cc6c9)
 
 By using this repository or any code related to it, you agree to the [legal notice](./LEGAL_NOTICE.md). The author is not responsible for any copies, forks, or reuploads made by other users. This is the author's only account and repository. To prevent impersonation or irresponsible actions, you may comply with the GNU GPL license this Repository uses.
 
 This (quite censored) New Version of gpt4free, was just released, it may contain bugs, open an issue or contribute a PR when encountering one, some features were disabled.
 Docker is for now not available but I would be happy if someone contributes a PR. The g4f GUI will be uploaded soon enough.
 
 ### New
@@ -107,15 +108,15 @@
 response = g4f.ChatCompletion.create(model='gpt-3.5-turbo', messages=[
                                      {"role": "user", "content": "Hello world"}], stream=True)
 
 for message in response:
     print(message)
 
 # normal response
-response = g4f.ChatCompletion.create(model=g4f.Model.gpt_4, messages=[
+response = g4f.ChatCompletion.create(model=g4f.models.gpt_4, messages=[
                                      {"role": "user", "content": "hi"}]) # alterative model setting
 
 print(response)
 
 
 # Set with provider
 response = g4f.ChatCompletion.create(model='gpt-3.5-turbo', provider=g4f.Provider.Forefront, messages=[
@@ -199,14 +200,15 @@
 | [free.easychat.work](https://free.easychat.work) | `g4f.Provider.EasyChat` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
 | [chat.acytoo.com](https://chat.acytoo.com/api/completions) | `g4f.Provider.Acytoo` | ✔️ | ❌ | ❌ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
 | [chat.dfehub.com](https://chat.dfehub.com/api/chat) | `g4f.Provider.DfeHub` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
 | [aiservice.vercel.app](https://aiservice.vercel.app/api/chat/answer) | `g4f.Provider.AiService` | ✔️ | ❌ | ❌ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
 | [b.ai-huan.xyz](https://b.ai-huan.xyz) | `g4f.Provider.BingHuan` | ✔️ | ✔️ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
 | [wewordle.org](https://wewordle.org/gptapi/v1/android/turbo) | `g4f.Provider.Wewordle` | ✔️ | ❌ | ❌ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
 | [chatgpt.ai](https://chatgpt.ai/gpt-4/) | `g4f.Provider.ChatgptAi` | ❌ | ✔️ | ❌ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
+| [opchatgpts.net](https://opchatgpts.net) | `g4f.Provider.opchatgpts` | ✔️ | ❌ | ❌ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
 
 
 ### Other Models
 
 | Model| Base Provider | Provider | Website |
 | ------- | ----------- | ---- |---- |
 | palm2 | Google | `g4f.Provider.Bard` | [bard.google.com](https://bard.google.com/) |
```

### Comparing `g4f-0.0.1.3/g4f.egg-info/SOURCES.txt` & `g4f-0.0.1.4/g4f.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -31,8 +31,9 @@
 g4f/Provider/Providers/Liaobots.py
 g4f/Provider/Providers/Lockchat.py
 g4f/Provider/Providers/Theb.py
 g4f/Provider/Providers/Vercel.py
 g4f/Provider/Providers/Wewordle.py
 g4f/Provider/Providers/You.py
 g4f/Provider/Providers/Yqcloud.py
-g4f/Provider/Providers/__init__.py
+g4f/Provider/Providers/__init__.py
+g4f/Provider/Providers/opchatgpts.py
```

### Comparing `g4f-0.0.1.3/setup.py` & `g4f-0.0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
     
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
-VERSION = '0.0.1.3'
+VERSION = '0.0.1.4'
 DESCRIPTION = 'The official gpt4free repository | various collection of powerful language models'
 
 # Setting up
 setup(
     name="g4f",
     version=VERSION,
     author="Tekky",
```

