# Comparing `tmp/vector_vault-2.1.7.tar.gz` & `tmp/vector_vault-2.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-2.1.7.tar", last modified: Sun Aug  6 16:37:32 2023, max compression
+gzip compressed data, was "vector_vault-2.1.8.tar", last modified: Mon Aug  7 02:46:54 2023, max compression
```

## Comparing `vector_vault-2.1.7.tar` & `vector_vault-2.1.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-08-06 16:37:32.639297 vector_vault-2.1.7/
--rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-2.1.7/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)    26434 2023-08-06 16:37:32.639102 vector_vault-2.1.7/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)    25775 2023-08-06 16:28:50.000000 vector_vault-2.1.7/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-08-06 16:37:32.639334 vector_vault-2.1.7/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1046 2023-08-06 16:37:02.000000 vector_vault-2.1.7/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-08-06 16:37:32.630103 vector_vault-2.1.7/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)    26434 2023-08-06 16:37:32.000000 vector_vault-2.1.7/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      456 2023-08-06 16:37:32.000000 vector_vault-2.1.7/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-08-06 16:37:32.000000 vector_vault-2.1.7/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-08-06 16:37:32.000000 vector_vault-2.1.7/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-08-06 16:37:32.000000 vector_vault-2.1.7/vector_vault.egg-info/top_level.txt
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-08-06 16:37:32.638529 vector_vault-2.1.7/vectorvault/
--rw-r--r--   0 johnrood   (501) staff       (20)      171 2023-06-09 19:04:41.000000 vector_vault-2.1.7/vectorvault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)    13996 2023-08-06 16:37:28.000000 vector_vault-2.1.7/vectorvault/ai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     2119 2023-06-27 02:14:51.000000 vector_vault-2.1.7/vectorvault/cloud_api.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3148 2023-07-18 22:45:16.000000 vector_vault-2.1.7/vectorvault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1883 2023-06-08 04:35:26.000000 vector_vault-2.1.7/vectorvault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)      707 2023-06-08 04:35:41.000000 vector_vault-2.1.7/vectorvault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)     2600 2023-07-18 22:45:26.000000 vector_vault-2.1.7/vectorvault/itemize.py
--rw-r--r--   0 johnrood   (501) staff       (20)    16773 2023-07-21 20:42:10.000000 vector_vault-2.1.7/vectorvault/tools_gpt.py
--rw-r--r--   0 johnrood   (501) staff       (20)    36592 2023-08-06 16:27:34.000000 vector_vault-2.1.7/vectorvault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)     4084 2023-07-16 04:42:19.000000 vector_vault-2.1.7/vectorvault/vecreq.py
--rw-r--r--   0 johnrood   (501) staff       (20)      399 2023-06-08 04:36:04.000000 vector_vault-2.1.7/vectorvault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-08-07 02:46:54.773221 vector_vault-2.1.8/
+-rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-2.1.8/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    28067 2023-08-07 02:46:54.773059 vector_vault-2.1.8/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    27408 2023-08-06 20:06:54.000000 vector_vault-2.1.8/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-08-07 02:46:54.773260 vector_vault-2.1.8/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1046 2023-08-07 02:46:28.000000 vector_vault-2.1.8/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-08-07 02:46:54.769273 vector_vault-2.1.8/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    28067 2023-08-07 02:46:54.000000 vector_vault-2.1.8/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      456 2023-08-07 02:46:54.000000 vector_vault-2.1.8/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-08-07 02:46:54.000000 vector_vault-2.1.8/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-08-07 02:46:54.000000 vector_vault-2.1.8/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-08-07 02:46:54.000000 vector_vault-2.1.8/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-08-07 02:46:54.772690 vector_vault-2.1.8/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      171 2023-06-09 19:04:41.000000 vector_vault-2.1.8/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    14352 2023-08-07 01:04:28.000000 vector_vault-2.1.8/vectorvault/ai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     2119 2023-06-27 02:14:51.000000 vector_vault-2.1.8/vectorvault/cloud_api.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3148 2023-07-18 22:45:16.000000 vector_vault-2.1.8/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1883 2023-06-08 04:35:26.000000 vector_vault-2.1.8/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      707 2023-06-08 04:35:41.000000 vector_vault-2.1.8/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     2600 2023-07-18 22:45:26.000000 vector_vault-2.1.8/vectorvault/itemize.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    16787 2023-08-06 19:45:14.000000 vector_vault-2.1.8/vectorvault/tools_gpt.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    36861 2023-08-06 17:13:56.000000 vector_vault-2.1.8/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     4084 2023-07-16 04:42:19.000000 vector_vault-2.1.8/vectorvault/vecreq.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      399 2023-06-08 04:36:04.000000 vector_vault-2.1.8/vectorvault/wrap.py
```

### Comparing `vector_vault-2.1.7/LICENSE` & `vector_vault-2.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-2.1.7/PKG-INFO` & `vector_vault-2.1.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_vault
-Version: 2.1.7
+Version: 2.1.8
 Summary: Customize ChatGPT and unleash the full potential of generative AI with Vector Vault
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -13,31 +13,36 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![alt text](https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/297fde6c-f5b4-4076-83bc-81dcfdbffebe/Vector+Vault+Header+5000.jpg)
 
-Vector Vault is a vector database cloud service built to make generative ai chat quick and easy. It allows you to seamlessly vectorize data and access it from the cloud. It's scalable to both small projects and large applications with millions of users. Vector Vault has been designed with a user-friendly code interface to make the process of working with vector search easy and let you focus on what matters. Vector Vault ensures secure and isolated data handling and enables you to create and interact with vector databases - aka "vaults" - in under one second response times, from our serverless cloud architecture backed by Google. 
+Vector Vault is a cloud-native vector database combined with OpenAI. Easily call ChatGPT or GPT4 and customize how they respond. Take any text data, vectorize it, and add it to the cloud vector database in 3 lines of code. Vector Vault enables you to quickly and securely create and interact with your vector databases - aka "Vaults". Vaults are hosted on serverless distributed cloud architecture backed by Google, making `vectorvault` scalable to any project size. 
 
-We've integrated all the chat options people like to use with LangChain. By combining vector databases with OpenAI's chat in the `vectorvault` package, we've been able to hide a lot of the complexity in the background and make it really easy to build the kind of custom chat experience you want to build. 
+`vectorvault` takes inspiration from LangChain and integrates their most popular chat features and LLM tools. However, by combining vector databases with OpenAI's chat into one single package, `vectorvault` is able to hide most of the complexity, making it simple to build custom chat experiences. The main value of the `vectorvault` package is how few lines of code you'll need to write to create the expirience you're goign for. It's much simpler and easier to use ChatGPT with the `vectorvault` package than OpenAI's default package. Customize what ChatGPT says by adding the kind of things you want it to say to the Vault. When you call the `get_chat()` function with "get_context=True", whatever you have added to the Vault will be the way ChatGPT sounds. Check out [PhilosophyGPT](https://philbrosophy.web.app) for an example of this (which was made using Vector Vault).
 
-With Vector Vault, integrating vector search results into your chat app is not only easy, it's the default. If you have been looking for a fast and reliable way to use vector databases with ChatGPT, then Vector Vault is for you. You will need an api key in order to access the Vault Cloud. If you don't already have one, you can sign up for a free account at [VectorVault.io](https://vectorvault.io)
+Make bots with knowledge and personalities. Create dynamic game characters with goals and opinions, AI support reps for a product/service, or your alter ego AI self. Use the "LLM Exclusive Tools" to create AI smart automation in code. The possibilities are endless and only limited by your imagination.
+
+Check out the tutorials in the Examples folder. You don't need a Vector Vault API key to use the tools or chat features, but you will need one to access the Vault Cloud. If you don't already have one, you can sign up for a free account at [VectorVault.io](https://vectorvault.io). While the service is paid at production scale, the first tier is free, and the following tiers are very affordable.
 
 <br>
 
 ### Full Python API:
 
 `pip install vector-vault` : install
 <br>
 `from vectorvault import Vault` : import
 <br>
-`v = Vault(user='your_eamil', api_key='your_api_key')` : Open a Vault instance 
+`v = Vault(
+  user='your_eamil', 
+  api_key='your_api_key',
+  openai_key='your_openai_api_key')` Create Vault Instance and Connect to OpenAI. *(Also call `verbose=True` to print all communications and notifications to the terminal while building)*
 <br>
-`v.add(text, meta=None, name='', split=False, split_size=1000)` : Loads data to be added to the Vault, with automatic text splitting for long texts. `text` is a text string. `meta` is a dictionary. `split=True` will split your text input, based on your `split_size`, which will be the approximate size of each split. For each split, a new item will automatically be created. `name` is a shortcut to adding a name field to the meta without creating a dictionary. If you don't create a dictionary, one with generic information will be created. If you don't assign a name, a generic one will be created. `text` is the only required input.
+`v.add(text, meta=None, name='', split=False, split_size=1000)` : Loads data to be added to the Vault, with automatic text splitting for long texts. `text` is a text string. `meta` is a dictionary. *(`split=True` will split your text input, based on your `split_size`. For each split, a new item will be created. `name` parameter is a shortcut to adding a "name" field to the metadata. If you don't add a name or any metadata, generic info will be added for you. `text` is the only required input)*
 <br>
 `v.get_vectors()` : Retrieves vectors embeddings for all loaded data. *(No parameters)*
 <br>
 `v.save()` : Saves all loaded data with embeddings to the Vault (cloud), along with any metadata. *(No parameters)*
 <br>
 `v.delete()` : Deletes the current Vault and all contents. *(No parameters)*
 <br>
@@ -50,35 +55,69 @@
 `v.get_total_items()` : Returns the total number of items in the Vault
 <br>
 `v.clear_cache()` : Clears the cache for all the loaded items - *`add()` loads an item*
 <br>
 `v.get_items_by_vector(vector, n)` : Returns vector similar items. Requires input vector, returns similar items. `n` is number of items you want returned, default = 4
 <br>
 `v.get_distance(id1, id2)`  : For getting the vector distance between two items `id1` and `id2` in the Vault. 
-
->> Items can be retrieved from the Vault with a nearest neighbor search using `get_similar()` and the item_ids can be found in the metadata. Item_ids are numeric and sequential, so accessing all items in the Vault can be done by iterating from beginning to end - e.g. `for i in range vault.get_total_items():`
+<br>*Items can be retrieved from the Vault with a nearest neighbor search using `get_similar()` and the item_ids can be found in the metadata. Item_ids are numeric and sequential, so accessing all items in the Vault can be done by iterating from beginning to end - e.g. `for i in range vault.get_total_items():`*
 
 `v.get_item_vector(id)` : returns the vector for item `id` in the Vault.
 <br>
 `v.get_items(ids)` : returns a list containing your item(s). `ids` is a list of ids, one or many
 <br>
 `v.cloud_stream(function)` : For cloud application yielding the chat stream, like a flask app. Called like *`v.cloud_stream(v.get_chat_stream('some_text'))`* in the return of a flask app.
 <br>
 `v.print_stream(function)` : For locally printing the chat stream. Called like *`v.print_stream(v.get_chat_stream('some_text'))`*. You can also assign a variable to it like *`reply = v.print_stream()`*  It still streams to the console, but the final complete text will also be available in the *`reply`* variable.
 <br>
 `v.get_chat()` : Retrieves a response from ChatGPT, with parameters for handling conversation history, summarizing responses, and retrieving context-based responses that reference similar data in the vault. *(See dedicated section below on using this function and its' parameters)*
 <br>
 `v.get_chat_stream()` : Retrieves a response from ChatGPT in stream format, with parameters for handling conversation history, summarizing responses, and retrieving context-based responses that reference similar data in the Vault. *(See dedicated section below on using this function and its' parameters)*
 <br>
+<br>
+<br>
 
+### LLM Exclusive Tools (`v.tools`):
+• `get_rating`:
+ Useful to get a quality rating
+<br>
+• `get_yes_no`:
+ Useful for getting a difinitive answer 
+<br>
+• `get_binary`:
+ Useful for getting a definitive answer in 0/1 format
+<br>
+• `get_match`:
+ Useful to get an exact match to a single option within a set of options -> in: (text and list of answers) -> out: (exact match to one answer in list of answer)
+<br>
+• `get_topic`:
+ Useful to classify the topic of conversation
+<br>
+• `match_or_make`:
+ Get a match to a list of options, or make a new one if unrelated
+ Useful if you aren't sure if the input will match one of your existing list options, and need flexibility of creating a new one. When starting from an empty list. - will create it from scratch
 
+```python
+# Tools example 1:
+number_out_of_ten = v.tools.get_rating('how does LeBron James compare to Michael Jordan')
 
->> `get_vectors()` utilizes OpenAI's embeddings api, internally batches vector embeddings with the text-embeddings-ada-002 model, and comes with auto rate-limiting and concurrent requests for maximum processing speed
+# Tools example 2: 
+this_or_that = v.tools.get_binary('should I turn right or left, 0 for right, 1 for left')
 
+# Tools example 3: 
+answer = v.tools.get_yes_no('should I use Vector Vault to build my next AI project?')
 
+print(answer)
+```
+>> yes
+
+
+
+<br>
+<br>
 <br>
 
 # Access The Vault:
 <p align="center">
   <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/2acebcaa-f5dd-44c9-8bba-c10723bc7064/Vector+Vault+Vault+2000.png" width="60%" height="60%" />
 </p>
 
@@ -397,29 +436,30 @@
 ```
 
 Getting context from the Vault is usually the goal when customizing text generation, and doing that requires additional prompt variables.
 `llm_w_context` and `llm__w_context_stream` models inject the history, context, and user input all in one prompt. In this case, your custom prompt needs to have `history`, `context` and `question` formattable in the prompt like so:
 
 *Example Custom Prompt:*  
 ```python
-custom_prompt = """
-    Use the following Context to answer the Question at the end. 
-    Answer as if you were the modern voice of the context, without referencing the context or mentioning that fact any context has been given. Make sure to not just repeat what is referenced. Don't preface or give any warnings at the end.
+# You can build a custom prompt with custom variables:
+my_prompt = """
+    Use the following information to answer the Question at the end. 
 
-    Chat History (if any): {history}
+    Math Result: {math_answer}
 
-    Additional Context: {context}
+    Known Variables: {known_vars}
 
     Question: {question}
 
     (Respond to the Question directly. Be the voice of the context, and most importantly: be interesting, engaging, and helpful) 
     Answer:
 """ 
-response = vault.get_chat(text, chat_history, get_context=True, custom_prompt=my_prompt)
+response = vault.get_chat(custom_prompt=my_prompt)
 ```
+A custom prompt makes the get_chat() function flexible for any use case. Check ai.py to see the stock prompt templates, and get a better idea of how they work...or just send me a message in Discord.
 
 <br>
 
 
 ## Normal Usage:
 ```python
 # connect to the vault you want to use
@@ -534,15 +574,15 @@
 ```
 
 Getting context from the Vault is usually the goal when customizing text generation, and doing that requires additional prompt variables.
 `llm_w_context` and `llm__w_context_stream` models inject the history, context, and user input all in one prompt. In this case, your custom prompt needs to have `history`, `context` and `question` formattable in the prompt like so:
 
 *Example with Custom Prompt:*  
 ```python
-custom_prompt = """
+my_prompt = """
     Use the following Context to answer the Question at the end. 
     Answer as if you were the modern voice of the context, without referencing the context or mentioning that fact any context has been given. Make sure to not just repeat what is referenced. Don't preface or give any warnings at the end.
 
     Chat History (if any): {history}
 
     Additional Context: {context}
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `vector_vault-2.1.7/README.md` & `vector_vault-2.1.8/vector_vault.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,48 @@
+Metadata-Version: 2.1
+Name: vector-vault
+Version: 2.1.8
+Summary: Customize ChatGPT and unleash the full potential of generative AI with Vector Vault
+Home-page: https://github.com/John-Rood/VectorVault
+Author: VectorVault.io
+Author-email: john@johnrood.com
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ![alt text](https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/297fde6c-f5b4-4076-83bc-81dcfdbffebe/Vector+Vault+Header+5000.jpg)
 
-Vector Vault is a vector database cloud service built to make generative ai chat quick and easy. It allows you to seamlessly vectorize data and access it from the cloud. It's scalable to both small projects and large applications with millions of users. Vector Vault has been designed with a user-friendly code interface to make the process of working with vector search easy and let you focus on what matters. Vector Vault ensures secure and isolated data handling and enables you to create and interact with vector databases - aka "vaults" - in under one second response times, from our serverless cloud architecture backed by Google. 
+Vector Vault is a cloud-native vector database combined with OpenAI. Easily call ChatGPT or GPT4 and customize how they respond. Take any text data, vectorize it, and add it to the cloud vector database in 3 lines of code. Vector Vault enables you to quickly and securely create and interact with your vector databases - aka "Vaults". Vaults are hosted on serverless distributed cloud architecture backed by Google, making `vectorvault` scalable to any project size. 
+
+`vectorvault` takes inspiration from LangChain and integrates their most popular chat features and LLM tools. However, by combining vector databases with OpenAI's chat into one single package, `vectorvault` is able to hide most of the complexity, making it simple to build custom chat experiences. The main value of the `vectorvault` package is how few lines of code you'll need to write to create the expirience you're goign for. It's much simpler and easier to use ChatGPT with the `vectorvault` package than OpenAI's default package. Customize what ChatGPT says by adding the kind of things you want it to say to the Vault. When you call the `get_chat()` function with "get_context=True", whatever you have added to the Vault will be the way ChatGPT sounds. Check out [PhilosophyGPT](https://philbrosophy.web.app) for an example of this (which was made using Vector Vault).
 
-We've integrated all the chat options people like to use with LangChain. By combining vector databases with OpenAI's chat in the `vectorvault` package, we've been able to hide a lot of the complexity in the background and make it really easy to build the kind of custom chat experience you want to build. 
+Make bots with knowledge and personalities. Create dynamic game characters with goals and opinions, AI support reps for a product/service, or your alter ego AI self. Use the "LLM Exclusive Tools" to create AI smart automation in code. The possibilities are endless and only limited by your imagination.
 
-With Vector Vault, integrating vector search results into your chat app is not only easy, it's the default. If you have been looking for a fast and reliable way to use vector databases with ChatGPT, then Vector Vault is for you. You will need an api key in order to access the Vault Cloud. If you don't already have one, you can sign up for a free account at [VectorVault.io](https://vectorvault.io)
+Check out the tutorials in the Examples folder. You don't need a Vector Vault API key to use the tools or chat features, but you will need one to access the Vault Cloud. If you don't already have one, you can sign up for a free account at [VectorVault.io](https://vectorvault.io). While the service is paid at production scale, the first tier is free, and the following tiers are very affordable.
 
 <br>
 
 ### Full Python API:
 
 `pip install vector-vault` : install
 <br>
 `from vectorvault import Vault` : import
 <br>
-`v = Vault(user='your_eamil', api_key='your_api_key')` : Open a Vault instance 
+`v = Vault(
+  user='your_eamil', 
+  api_key='your_api_key',
+  openai_key='your_openai_api_key')` Create Vault Instance and Connect to OpenAI. *(Also call `verbose=True` to print all communications and notifications to the terminal while building)*
 <br>
-`v.add(text, meta=None, name='', split=False, split_size=1000)` : Loads data to be added to the Vault, with automatic text splitting for long texts. `text` is a text string. `meta` is a dictionary. `split=True` will split your text input, based on your `split_size`, which will be the approximate size of each split. For each split, a new item will automatically be created. `name` is a shortcut to adding a name field to the meta without creating a dictionary. If you don't create a dictionary, one with generic information will be created. If you don't assign a name, a generic one will be created. `text` is the only required input.
+`v.add(text, meta=None, name='', split=False, split_size=1000)` : Loads data to be added to the Vault, with automatic text splitting for long texts. `text` is a text string. `meta` is a dictionary. *(`split=True` will split your text input, based on your `split_size`. For each split, a new item will be created. `name` parameter is a shortcut to adding a "name" field to the metadata. If you don't add a name or any metadata, generic info will be added for you. `text` is the only required input)*
 <br>
 `v.get_vectors()` : Retrieves vectors embeddings for all loaded data. *(No parameters)*
 <br>
 `v.save()` : Saves all loaded data with embeddings to the Vault (cloud), along with any metadata. *(No parameters)*
 <br>
 `v.delete()` : Deletes the current Vault and all contents. *(No parameters)*
 <br>
@@ -33,36 +55,70 @@
 `v.get_total_items()` : Returns the total number of items in the Vault
 <br>
 `v.clear_cache()` : Clears the cache for all the loaded items - *`add()` loads an item*
 <br>
 `v.get_items_by_vector(vector, n)` : Returns vector similar items. Requires input vector, returns similar items. `n` is number of items you want returned, default = 4
 <br>
 `v.get_distance(id1, id2)`  : For getting the vector distance between two items `id1` and `id2` in the Vault. 
-
->> Items can be retrieved from the Vault with a nearest neighbor search using `get_similar()` and the item_ids can be found in the metadata. Item_ids are numeric and sequential, so accessing all items in the Vault can be done by iterating from beginning to end - e.g. `for i in range vault.get_total_items():`
+<br>*Items can be retrieved from the Vault with a nearest neighbor search using `get_similar()` and the item_ids can be found in the metadata. Item_ids are numeric and sequential, so accessing all items in the Vault can be done by iterating from beginning to end - e.g. `for i in range vault.get_total_items():`*
 
 `v.get_item_vector(id)` : returns the vector for item `id` in the Vault.
 <br>
 `v.get_items(ids)` : returns a list containing your item(s). `ids` is a list of ids, one or many
 <br>
 `v.cloud_stream(function)` : For cloud application yielding the chat stream, like a flask app. Called like *`v.cloud_stream(v.get_chat_stream('some_text'))`* in the return of a flask app.
 <br>
 `v.print_stream(function)` : For locally printing the chat stream. Called like *`v.print_stream(v.get_chat_stream('some_text'))`*. You can also assign a variable to it like *`reply = v.print_stream()`*  It still streams to the console, but the final complete text will also be available in the *`reply`* variable.
 <br>
 `v.get_chat()` : Retrieves a response from ChatGPT, with parameters for handling conversation history, summarizing responses, and retrieving context-based responses that reference similar data in the vault. *(See dedicated section below on using this function and its' parameters)*
 <br>
 `v.get_chat_stream()` : Retrieves a response from ChatGPT in stream format, with parameters for handling conversation history, summarizing responses, and retrieving context-based responses that reference similar data in the Vault. *(See dedicated section below on using this function and its' parameters)*
 <br>
+<br>
+<br>
+
+### LLM Exclusive Tools (`v.tools`):
+• `get_rating`:
+ Useful to get a quality rating
+<br>
+• `get_yes_no`:
+ Useful for getting a difinitive answer 
+<br>
+• `get_binary`:
+ Useful for getting a definitive answer in 0/1 format
+<br>
+• `get_match`:
+ Useful to get an exact match to a single option within a set of options -> in: (text and list of answers) -> out: (exact match to one answer in list of answer)
+<br>
+• `get_topic`:
+ Useful to classify the topic of conversation
+<br>
+• `match_or_make`:
+ Get a match to a list of options, or make a new one if unrelated
+ Useful if you aren't sure if the input will match one of your existing list options, and need flexibility of creating a new one. When starting from an empty list. - will create it from scratch
 
+```python
+# Tools example 1:
+number_out_of_ten = v.tools.get_rating('how does LeBron James compare to Michael Jordan')
+
+# Tools example 2: 
+this_or_that = v.tools.get_binary('should I turn right or left, 0 for right, 1 for left')
+
+# Tools example 3: 
+answer = v.tools.get_yes_no('should I use Vector Vault to build my next AI project?')
 
+print(answer)
+```
+>> yes
 
->> `get_vectors()` utilizes OpenAI's embeddings api, internally batches vector embeddings with the text-embeddings-ada-002 model, and comes with auto rate-limiting and concurrent requests for maximum processing speed
 
 
 <br>
+<br>
+<br>
 
 # Access The Vault:
 <p align="center">
   <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/2acebcaa-f5dd-44c9-8bba-c10723bc7064/Vector+Vault+Vault+2000.png" width="60%" height="60%" />
 </p>
 
 Install Vector Vault:
@@ -380,29 +436,30 @@
 ```
 
 Getting context from the Vault is usually the goal when customizing text generation, and doing that requires additional prompt variables.
 `llm_w_context` and `llm__w_context_stream` models inject the history, context, and user input all in one prompt. In this case, your custom prompt needs to have `history`, `context` and `question` formattable in the prompt like so:
 
 *Example Custom Prompt:*  
 ```python
-custom_prompt = """
-    Use the following Context to answer the Question at the end. 
-    Answer as if you were the modern voice of the context, without referencing the context or mentioning that fact any context has been given. Make sure to not just repeat what is referenced. Don't preface or give any warnings at the end.
+# You can build a custom prompt with custom variables:
+my_prompt = """
+    Use the following information to answer the Question at the end. 
 
-    Chat History (if any): {history}
+    Math Result: {math_answer}
 
-    Additional Context: {context}
+    Known Variables: {known_vars}
 
     Question: {question}
 
     (Respond to the Question directly. Be the voice of the context, and most importantly: be interesting, engaging, and helpful) 
     Answer:
 """ 
-response = vault.get_chat(text, chat_history, get_context=True, custom_prompt=my_prompt)
+response = vault.get_chat(custom_prompt=my_prompt)
 ```
+A custom prompt makes the get_chat() function flexible for any use case. Check ai.py to see the stock prompt templates, and get a better idea of how they work...or just send me a message in Discord.
 
 <br>
 
 
 ## Normal Usage:
 ```python
 # connect to the vault you want to use
@@ -517,15 +574,15 @@
 ```
 
 Getting context from the Vault is usually the goal when customizing text generation, and doing that requires additional prompt variables.
 `llm_w_context` and `llm__w_context_stream` models inject the history, context, and user input all in one prompt. In this case, your custom prompt needs to have `history`, `context` and `question` formattable in the prompt like so:
 
 *Example with Custom Prompt:*  
 ```python
-custom_prompt = """
+my_prompt = """
     Use the following Context to answer the Question at the end. 
     Answer as if you were the modern voice of the context, without referencing the context or mentioning that fact any context has been given. Make sure to not just repeat what is referenced. Don't preface or give any warnings at the end.
 
     Chat History (if any): {history}
 
     Additional Context: {context}
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `vector_vault-2.1.7/setup.py` & `vector_vault-2.1.8/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="2.1.7",
+    version="2.1.8",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="Customize ChatGPT and unleash the full potential of generative AI with Vector Vault",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/John-Rood/VectorVault",
```

### Comparing `vector_vault-2.1.7/vector_vault.egg-info/PKG-INFO` & `vector_vault-2.1.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,43 +1,31 @@
-Metadata-Version: 2.1
-Name: vector-vault
-Version: 2.1.7
-Summary: Customize ChatGPT and unleash the full potential of generative AI with Vector Vault
-Home-page: https://github.com/John-Rood/VectorVault
-Author: VectorVault.io
-Author-email: john@johnrood.com
-Classifier: License :: Other/Proprietary License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ![alt text](https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/297fde6c-f5b4-4076-83bc-81dcfdbffebe/Vector+Vault+Header+5000.jpg)
 
-Vector Vault is a vector database cloud service built to make generative ai chat quick and easy. It allows you to seamlessly vectorize data and access it from the cloud. It's scalable to both small projects and large applications with millions of users. Vector Vault has been designed with a user-friendly code interface to make the process of working with vector search easy and let you focus on what matters. Vector Vault ensures secure and isolated data handling and enables you to create and interact with vector databases - aka "vaults" - in under one second response times, from our serverless cloud architecture backed by Google. 
+Vector Vault is a cloud-native vector database combined with OpenAI. Easily call ChatGPT or GPT4 and customize how they respond. Take any text data, vectorize it, and add it to the cloud vector database in 3 lines of code. Vector Vault enables you to quickly and securely create and interact with your vector databases - aka "Vaults". Vaults are hosted on serverless distributed cloud architecture backed by Google, making `vectorvault` scalable to any project size. 
+
+`vectorvault` takes inspiration from LangChain and integrates their most popular chat features and LLM tools. However, by combining vector databases with OpenAI's chat into one single package, `vectorvault` is able to hide most of the complexity, making it simple to build custom chat experiences. The main value of the `vectorvault` package is how few lines of code you'll need to write to create the expirience you're goign for. It's much simpler and easier to use ChatGPT with the `vectorvault` package than OpenAI's default package. Customize what ChatGPT says by adding the kind of things you want it to say to the Vault. When you call the `get_chat()` function with "get_context=True", whatever you have added to the Vault will be the way ChatGPT sounds. Check out [PhilosophyGPT](https://philbrosophy.web.app) for an example of this (which was made using Vector Vault).
 
-We've integrated all the chat options people like to use with LangChain. By combining vector databases with OpenAI's chat in the `vectorvault` package, we've been able to hide a lot of the complexity in the background and make it really easy to build the kind of custom chat experience you want to build. 
+Make bots with knowledge and personalities. Create dynamic game characters with goals and opinions, AI support reps for a product/service, or your alter ego AI self. Use the "LLM Exclusive Tools" to create AI smart automation in code. The possibilities are endless and only limited by your imagination.
 
-With Vector Vault, integrating vector search results into your chat app is not only easy, it's the default. If you have been looking for a fast and reliable way to use vector databases with ChatGPT, then Vector Vault is for you. You will need an api key in order to access the Vault Cloud. If you don't already have one, you can sign up for a free account at [VectorVault.io](https://vectorvault.io)
+Check out the tutorials in the Examples folder. You don't need a Vector Vault API key to use the tools or chat features, but you will need one to access the Vault Cloud. If you don't already have one, you can sign up for a free account at [VectorVault.io](https://vectorvault.io). While the service is paid at production scale, the first tier is free, and the following tiers are very affordable.
 
 <br>
 
 ### Full Python API:
 
 `pip install vector-vault` : install
 <br>
 `from vectorvault import Vault` : import
 <br>
-`v = Vault(user='your_eamil', api_key='your_api_key')` : Open a Vault instance 
+`v = Vault(
+  user='your_eamil', 
+  api_key='your_api_key',
+  openai_key='your_openai_api_key')` Create Vault Instance and Connect to OpenAI. *(Also call `verbose=True` to print all communications and notifications to the terminal while building)*
 <br>
-`v.add(text, meta=None, name='', split=False, split_size=1000)` : Loads data to be added to the Vault, with automatic text splitting for long texts. `text` is a text string. `meta` is a dictionary. `split=True` will split your text input, based on your `split_size`, which will be the approximate size of each split. For each split, a new item will automatically be created. `name` is a shortcut to adding a name field to the meta without creating a dictionary. If you don't create a dictionary, one with generic information will be created. If you don't assign a name, a generic one will be created. `text` is the only required input.
+`v.add(text, meta=None, name='', split=False, split_size=1000)` : Loads data to be added to the Vault, with automatic text splitting for long texts. `text` is a text string. `meta` is a dictionary. *(`split=True` will split your text input, based on your `split_size`. For each split, a new item will be created. `name` parameter is a shortcut to adding a "name" field to the metadata. If you don't add a name or any metadata, generic info will be added for you. `text` is the only required input)*
 <br>
 `v.get_vectors()` : Retrieves vectors embeddings for all loaded data. *(No parameters)*
 <br>
 `v.save()` : Saves all loaded data with embeddings to the Vault (cloud), along with any metadata. *(No parameters)*
 <br>
 `v.delete()` : Deletes the current Vault and all contents. *(No parameters)*
 <br>
@@ -50,36 +38,70 @@
 `v.get_total_items()` : Returns the total number of items in the Vault
 <br>
 `v.clear_cache()` : Clears the cache for all the loaded items - *`add()` loads an item*
 <br>
 `v.get_items_by_vector(vector, n)` : Returns vector similar items. Requires input vector, returns similar items. `n` is number of items you want returned, default = 4
 <br>
 `v.get_distance(id1, id2)`  : For getting the vector distance between two items `id1` and `id2` in the Vault. 
-
->> Items can be retrieved from the Vault with a nearest neighbor search using `get_similar()` and the item_ids can be found in the metadata. Item_ids are numeric and sequential, so accessing all items in the Vault can be done by iterating from beginning to end - e.g. `for i in range vault.get_total_items():`
+<br>*Items can be retrieved from the Vault with a nearest neighbor search using `get_similar()` and the item_ids can be found in the metadata. Item_ids are numeric and sequential, so accessing all items in the Vault can be done by iterating from beginning to end - e.g. `for i in range vault.get_total_items():`*
 
 `v.get_item_vector(id)` : returns the vector for item `id` in the Vault.
 <br>
 `v.get_items(ids)` : returns a list containing your item(s). `ids` is a list of ids, one or many
 <br>
 `v.cloud_stream(function)` : For cloud application yielding the chat stream, like a flask app. Called like *`v.cloud_stream(v.get_chat_stream('some_text'))`* in the return of a flask app.
 <br>
 `v.print_stream(function)` : For locally printing the chat stream. Called like *`v.print_stream(v.get_chat_stream('some_text'))`*. You can also assign a variable to it like *`reply = v.print_stream()`*  It still streams to the console, but the final complete text will also be available in the *`reply`* variable.
 <br>
 `v.get_chat()` : Retrieves a response from ChatGPT, with parameters for handling conversation history, summarizing responses, and retrieving context-based responses that reference similar data in the vault. *(See dedicated section below on using this function and its' parameters)*
 <br>
 `v.get_chat_stream()` : Retrieves a response from ChatGPT in stream format, with parameters for handling conversation history, summarizing responses, and retrieving context-based responses that reference similar data in the Vault. *(See dedicated section below on using this function and its' parameters)*
 <br>
+<br>
+<br>
+
+### LLM Exclusive Tools (`v.tools`):
+• `get_rating`:
+ Useful to get a quality rating
+<br>
+• `get_yes_no`:
+ Useful for getting a difinitive answer 
+<br>
+• `get_binary`:
+ Useful for getting a definitive answer in 0/1 format
+<br>
+• `get_match`:
+ Useful to get an exact match to a single option within a set of options -> in: (text and list of answers) -> out: (exact match to one answer in list of answer)
+<br>
+• `get_topic`:
+ Useful to classify the topic of conversation
+<br>
+• `match_or_make`:
+ Get a match to a list of options, or make a new one if unrelated
+ Useful if you aren't sure if the input will match one of your existing list options, and need flexibility of creating a new one. When starting from an empty list. - will create it from scratch
 
+```python
+# Tools example 1:
+number_out_of_ten = v.tools.get_rating('how does LeBron James compare to Michael Jordan')
+
+# Tools example 2: 
+this_or_that = v.tools.get_binary('should I turn right or left, 0 for right, 1 for left')
+
+# Tools example 3: 
+answer = v.tools.get_yes_no('should I use Vector Vault to build my next AI project?')
 
+print(answer)
+```
+>> yes
 
->> `get_vectors()` utilizes OpenAI's embeddings api, internally batches vector embeddings with the text-embeddings-ada-002 model, and comes with auto rate-limiting and concurrent requests for maximum processing speed
 
 
 <br>
+<br>
+<br>
 
 # Access The Vault:
 <p align="center">
   <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/2acebcaa-f5dd-44c9-8bba-c10723bc7064/Vector+Vault+Vault+2000.png" width="60%" height="60%" />
 </p>
 
 Install Vector Vault:
@@ -397,29 +419,30 @@
 ```
 
 Getting context from the Vault is usually the goal when customizing text generation, and doing that requires additional prompt variables.
 `llm_w_context` and `llm__w_context_stream` models inject the history, context, and user input all in one prompt. In this case, your custom prompt needs to have `history`, `context` and `question` formattable in the prompt like so:
 
 *Example Custom Prompt:*  
 ```python
-custom_prompt = """
-    Use the following Context to answer the Question at the end. 
-    Answer as if you were the modern voice of the context, without referencing the context or mentioning that fact any context has been given. Make sure to not just repeat what is referenced. Don't preface or give any warnings at the end.
+# You can build a custom prompt with custom variables:
+my_prompt = """
+    Use the following information to answer the Question at the end. 
 
-    Chat History (if any): {history}
+    Math Result: {math_answer}
 
-    Additional Context: {context}
+    Known Variables: {known_vars}
 
     Question: {question}
 
     (Respond to the Question directly. Be the voice of the context, and most importantly: be interesting, engaging, and helpful) 
     Answer:
 """ 
-response = vault.get_chat(text, chat_history, get_context=True, custom_prompt=my_prompt)
+response = vault.get_chat(custom_prompt=my_prompt)
 ```
+A custom prompt makes the get_chat() function flexible for any use case. Check ai.py to see the stock prompt templates, and get a better idea of how they work...or just send me a message in Discord.
 
 <br>
 
 
 ## Normal Usage:
 ```python
 # connect to the vault you want to use
@@ -534,15 +557,15 @@
 ```
 
 Getting context from the Vault is usually the goal when customizing text generation, and doing that requires additional prompt variables.
 `llm_w_context` and `llm__w_context_stream` models inject the history, context, and user input all in one prompt. In this case, your custom prompt needs to have `history`, `context` and `question` formattable in the prompt like so:
 
 *Example with Custom Prompt:*  
 ```python
-custom_prompt = """
+my_prompt = """
     Use the following Context to answer the Question at the end. 
     Answer as if you were the modern voice of the context, without referencing the context or mentioning that fact any context has been given. Make sure to not just repeat what is referenced. Don't preface or give any warnings at the end.
 
     Chat History (if any): {history}
 
     Additional Context: {context}
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `vector_vault-2.1.7/vectorvault/ai.py` & `vector_vault-2.1.8/vectorvault/ai.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 class AI:
     def __init__(self) -> None:
         pass
 
     # This function returns a ChatGPT completion based on a provided input.
     def llm(self, user_input: str = None, history: str = None, model='gpt-3.5-turbo', max_tokens=4000, custom_prompt=False):
         '''
-            If you pass in a custom_prompt with content already fully filled in, and no user_input, it will process your custom_prompt only without changing       
+            If you pass in a custom_prompt with content already fully filled in, and no user_input, 
+            it will process your custom_prompt only without changing       
         '''
         max_tokens = max_tokens * 4 if model == 'gpt-3.5-turbo-16k' else max_tokens
         max_tokens = max_tokens * 8 if model == 'gpt-4-32k' else max_tokens
         prompt_template = custom_prompt if custom_prompt else """{content}""" 
         if user_input:
             intokes = self.get_tokens(user_input)
             histokes = self.get_tokens(history) if history else 0
@@ -24,209 +25,215 @@
                 if history:
                     intokes = self.get_tokens(user_input)
                     tokes_left = max_tokens - intokes
                     chars_left = int(tokes_left * 4)
                     history = history[-chars_left:]
                 else: # no history. If it was overlimit, then it was taken care of above
                     pass
+            prompt = prompt_template.format(content=user_input)
+
             if history:
-                prompt = prompt_template.format(content=user_input)
                 response = openai.ChatCompletion.create(
                     model=model,
                     messages=[
                         {"role": "system", "content": f"Chat history: {history}"},
                         {"role": "user", "content": f"{prompt}"}]
                 )
                 return response['choices'][0]['message']['content']
             else:
                 # 'model' is the name of the model to use
                 # 'messages' is a list of message objects that mimics a conversation.
-                # Each object has a 'role' that can be 'system', 'user', or 'assistant', and a 'content' which is the actual content of the message.
-                prompt = prompt_template.format(content=user_input)
+                # Each object has a 'role' that can be either 'system', 'user', or 'assistant', and then 'content' is the actual content of the message.
                 response = openai.ChatCompletion.create(
                     model=model,
                     messages=[{"role": "user", "content": f"{prompt}"}]
                 )
                 return response['choices'][0]['message']['content']
-        else: # make no changes, and return response to passed in custom_prompt
+        else: # make no changes, and return response to custom_prompt
             if custom_prompt:
                 response = openai.ChatCompletion.create(
                     model=model,
                     messages=[{"role": "user", "content": f"{custom_prompt}"}]
                 )
                 return response['choices'][0]['message']['content']
             else:
                 raise 'Error: Need custom_prompt if no user_input'
             
                     
-    def llm_w_context(self, user_input, context, history=None, model='gpt-3.5-turbo', max_tokens=4000, custom_prompt=False):
+    def llm_w_context(self, user_input = None, context = None, history=None, model='gpt-3.5-turbo', max_tokens=4000, custom_prompt=False):
         prompt_template = custom_prompt if custom_prompt else """
         Use the following Context to answer the Question at the end. 
-        Answer as if you were the modern voice of the context, without referencing the context or mentioning that fact any context has been given. Make sure to not just repeat what is referenced. Don't preface or give any warnings at the end.
+        Answer as if you were the modern voice of the context, without referencing the context or mentioning 
+        the fact that any context has been given. Make sure to not just repeat what is referenced. Don't preface or give any warnings at the end.
 
         Chat History (if any): {history}
 
         Additional Context: {context}
 
         Question: {content}
 
         (Answer the question directly. Be the voice of the context, and most importantly: be interesting, engaging, and helpful) 
         Answer:""" 
 
         max_tokens = max_tokens * 4 if model == 'gpt-3.5-turbo-16k' else max_tokens
         max_tokens = max_tokens * 8 if model == 'gpt-4-32k' else max_tokens
 
-        intokes = self.get_tokens(user_input)
-        contokes = self.get_tokens(context)
-        history = history if history else ""
-        histokes = self.get_tokens(history)
-        promptokes = self.get_tokens(prompt_template)
-
-        if (intokes + contokes + histokes + promptokes) > max_tokens * .9:
-            tokes_left = max_tokens - intokes
-            if len(history) > 1:
-                tokes_left = (max_tokens/2) - intokes 
-                char_left = int(tokes_left * 4)
-                history = history[-char_left:]
-                tokes_left_after_hist = max_tokens - self.get_tokens(user_input + history)
-                char_left_after_hist = int(tokes_left_after_hist * 4)
-                context = context[-char_left_after_hist:]
-                double_check = self.get_tokens(user_input+history+context+prompt_template)
-                if double_check > max_tokens: 
-                    overby = double_check - max_tokens
-                    char_to_take_away = overby * 5
-                    context_length = len(context)
-                    remove_from_context = int(context_length - char_to_take_away)
-                    context = context[-remove_from_context:] 
-            else:
-                char_left = int(tokes_left * 4) 
-                context = context[-char_left:]
-                double_check = self.get_tokens(user_input + context)
-                if double_check > max_tokens:
-                    overby = double_check - max_tokens
-                    char_to_take_away = overby * 5
-                    context_length = len(context)
-                    remove_from_context = int(context_length - char_to_take_away)
-                    context = context[-remove_from_context:] 
-
-        # Format the prompt
-        user_input = history + user_input
-        prompt = prompt_template.format(context=context, history=history, content=user_input)
+        if user_input and context:
+            intokes = self.get_tokens(user_input)
+            contokes = self.get_tokens(context)
+            history = history if history else ""
+            histokes = self.get_tokens(history)
+            promptokes = self.get_tokens(prompt_template)
+
+            if (intokes + contokes + histokes + promptokes) > max_tokens * .9:
+                tokes_left = max_tokens - intokes
+                if len(history) > 1:
+                    tokes_left = (max_tokens/2) - intokes 
+                    char_left = int(tokes_left * 4)
+                    history = history[-char_left:]
+                    tokes_left_after_hist = max_tokens - self.get_tokens(user_input + history)
+                    char_left_after_hist = int(tokes_left_after_hist * 4)
+                    context = context[-char_left_after_hist:]
+                    double_check = self.get_tokens(user_input+history+context+prompt_template)
+                    if double_check > max_tokens: 
+                        overby = double_check - max_tokens
+                        char_to_take_away = overby * 5
+                        context_length = len(context)
+                        remove_from_context = int(context_length - char_to_take_away)
+                        context = context[-remove_from_context:] 
+                else:
+                    char_left = int(tokes_left * 4) 
+                    context = context[-char_left:]
+                    double_check = self.get_tokens(user_input + context)
+                    if double_check > max_tokens:
+                        overby = double_check - max_tokens
+                        char_to_take_away = overby * 5
+                        context_length = len(context)
+                        remove_from_context = int(context_length - char_to_take_away)
+                        context = context[-remove_from_context:] 
+
+            # Format the prompt
+            user_input = history + user_input
+            prompt = prompt_template.format(context=context, history=history, content=user_input)
+
         response = openai.ChatCompletion.create(
             model=model,
             messages=[
                 {"role": "user", "content": f"{prompt}"}],
         )
         return response['choices'][0]['message']['content']
 
 
-    def llm_stream(self, user_input, history=None, model='gpt-3.5-turbo', max_tokens=4000, custom_prompt=False):
+    def llm_stream(self, user_input = None, history=None, model='gpt-3.5-turbo', max_tokens=4000, custom_prompt=False):
         '''
             Stream version of "llm"
         '''
         max_tokens = max_tokens * 4 if model == 'gpt-3.5-turbo-16k' else max_tokens
         max_tokens = max_tokens * 8 if model == 'gpt-4-32k' else max_tokens
         prompt_template = custom_prompt if custom_prompt else """{content}""" 
-        intokes = self.get_tokens(user_input)
-        histokes = self.get_tokens(history) if history else 0
-        if intokes + histokes > max_tokens:
-            tokes_left = max_tokens - intokes - histokes
-            if tokes_left < 0: # way too much input
-                char_to_remove = (tokes_left * -1) * 5 # make positive and remove that amount
-                user_input = user_input[char_to_remove:] # get in front of it, chop at max
-            if history:
-                intokes = self.get_tokens(user_input)
-                tokes_left = max_tokens - intokes
-                chars_left = int(tokes_left * 4)
-                history = history[-chars_left:]
-            else: # no history. If it was overlimit, then it was taken care of above
-                pass
-        if history:
+        
+        if user_input:
+            intokes = self.get_tokens(user_input)
+            histokes = self.get_tokens(history) if history else 0
+            if intokes + histokes > max_tokens:
+                tokes_left = max_tokens - intokes - histokes
+                if tokes_left < 0: # way too much input
+                    char_to_remove = (tokes_left * -1) * 5 # make positive and remove that amount
+                    user_input = user_input[char_to_remove:] # get in front of it, chop at max
+                if history:
+                    intokes = self.get_tokens(user_input)
+                    tokes_left = max_tokens - intokes
+                    chars_left = int(tokes_left * 4)
+                    history = history[-chars_left:]
+                else: # no history. If it was overlimit, then it was taken care of above
+                    pass
             prompt = prompt_template.format(content=user_input)
+        if history:
             response = openai.ChatCompletion.create(
                 model=model,
                 messages=[
                     {"role": "system", "content": f"Chat history: {history}"},
                     {"role": "user", "content": f"{prompt}"}]
             )
             for message in response:
                 choices = message.get('choices', [])
                 if choices:
                     delta = choices[0].get('delta', {})
                     if 'content' in delta:
                         content = delta['content']
                         yield content
         else:
-            prompt = prompt_template.format(content=user_input)
             response = openai.ChatCompletion.create(
                 model=model,
                 messages=[{"role": "user", "content": f"{prompt}"}],
                 stream=True
             )
             for message in response:
                 choices = message.get('choices', [])
                 if choices:
                     delta = choices[0].get('delta', {})
                     if 'content' in delta:
                         content = delta['content']
                         yield content
                         
                     
-    def llm_w_context_stream(self, user_input, context, history=None, model='gpt-3.5-turbo', max_tokens=4000, custom_prompt=False):
+    def llm_w_context_stream(self, user_input = None, context = None, history=None, model='gpt-3.5-turbo', max_tokens=4000, custom_prompt=False):
         prompt_template = custom_prompt if custom_prompt else """
         Use the following Context to answer the Question at the end. 
-        Answer as if you were the modern voice of the context, without referencing the context or mentioning that fact any context has been given. Make sure to not just repeat what is referenced. Don't preface or give any warnings at the end.
+        Answer as if you were the modern voice of the context, without referencing the context or mentioning 
+        the fact that any context has been given. Make sure to not just repeat what is referenced. Don't preface or give any warnings at the end.
 
         Chat History (if any): {history}
 
         Additional Context: {context}
 
         Question: {content}
 
         (Respond to the Question directly. Be the voice of the context, and most importantly: be interesting, engaging, and helpful) 
         Answer:""" 
 
         max_tokens = max_tokens * 4 if model == 'gpt-3.5-turbo-16k' else max_tokens
         max_tokens = max_tokens * 8 if model == 'gpt-4-32k' else max_tokens
 
-        intokes = self.get_tokens(user_input)
-        contokes = self.get_tokens(context)
-        history = history if history else ""
-        histokes = self.get_tokens(history)
-        promptokes = self.get_tokens(prompt_template)
-
-        if (intokes + contokes + histokes + promptokes) > max_tokens * .9:
-            tokes_left = max_tokens - intokes
-            if len(history) > 1:
-                tokes_left = (max_tokens/2) - intokes 
-                char_left = int(tokes_left * 4)
-                history = history[-char_left:]
-                tokes_left_after_hist = max_tokens - self.get_tokens(user_input + history)
-                char_left_after_hist = int(tokes_left_after_hist * 4)
-                context = context[-char_left_after_hist:]
-                double_check = self.get_tokens(user_input+history+context+prompt_template)
-                if double_check > max_tokens: 
-                    overby = double_check - max_tokens
-                    char_to_take_away = overby * 5
-                    context_length = len(context)
-                    remove_from_context = int(context_length - char_to_take_away)
-                    context = context[-remove_from_context:] 
-            else:
-                char_left = int(tokes_left * 4) 
-                context = context[-char_left:]
-                double_check = self.get_tokens(user_input + context)
-                if double_check > max_tokens:
-                    overby = double_check - max_tokens
-                    char_to_take_away = overby * 5
-                    context_length = len(context)
-                    remove_from_context = int(context_length - char_to_take_away)
-                    context = context[-remove_from_context:] 
-
-        prompt = prompt_template.format(context=context, history=history, content=user_input)
-        user_input = history + user_input
+        if user_input:
+            intokes = self.get_tokens(user_input)
+            contokes = self.get_tokens(context)
+            history = history if history else ""
+            histokes = self.get_tokens(history)
+            promptokes = self.get_tokens(prompt_template)
+            if (intokes + contokes + histokes + promptokes) > max_tokens * .9:
+                tokes_left = max_tokens - intokes
+                if len(history) > 1:
+                    tokes_left = (max_tokens/2) - intokes 
+                    char_left = int(tokes_left * 4)
+                    history = history[-char_left:]
+                    tokes_left_after_hist = max_tokens - self.get_tokens(user_input + history)
+                    char_left_after_hist = int(tokes_left_after_hist * 4)
+                    context = context[-char_left_after_hist:]
+                    double_check = self.get_tokens(user_input+history+context+prompt_template)
+                    if double_check > max_tokens: 
+                        overby = double_check - max_tokens
+                        char_to_take_away = overby * 5
+                        context_length = len(context)
+                        remove_from_context = int(context_length - char_to_take_away)
+                        context = context[-remove_from_context:] 
+                else:
+                    char_left = int(tokes_left * 4) 
+                    context = context[-char_left:]
+                    double_check = self.get_tokens(user_input + context)
+                    if double_check > max_tokens:
+                        overby = double_check - max_tokens
+                        char_to_take_away = overby * 5
+                        context_length = len(context)
+                        remove_from_context = int(context_length - char_to_take_away)
+                        context = context[-remove_from_context:] 
+
+            user_input = history + user_input
+            prompt = prompt_template.format(context=context, history=history, content=user_input)
+        
         response = openai.ChatCompletion.create(
             model=model,
             messages=[
                 {"role": "user", "content": f"{prompt}"}],
             stream=True
         )
         for message in response:
```

### Comparing `vector_vault-2.1.7/vectorvault/cloud_api.py` & `vector_vault-2.1.8/vectorvault/cloud_api.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.1.7/vectorvault/cloudmanager.py` & `vector_vault-2.1.8/vectorvault/cloudmanager.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.1.7/vectorvault/creds.py` & `vector_vault-2.1.8/vectorvault/creds.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.1.7/vectorvault/download.py` & `vector_vault-2.1.8/vectorvault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.1.7/vectorvault/itemize.py` & `vector_vault-2.1.8/vectorvault/itemize.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.1.7/vectorvault/tools_gpt.py` & `vector_vault-2.1.8/vectorvault/tools_gpt.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,20 +20,20 @@
         1. `get_rating`:
             Useful to get a quality rating
 
         2. `get_yes_no`:
             Useful for getting a difinitive answer 
 
         3. `get_binary`:
-            Useful for getting numeric input on a difinitive answer
+            Useful for getting a definitive answer in 0/1 format
         
         4. `get_match`:
-            Useful to get an exact match to one option in a set of options
-            in: (text and list of answers)
-            out: (exact match to one answer in list of answer)
+            Useful to get an exact match to a single option within a set of options 
+            -> in: (text and list of answers) 
+            -> out: (exact match to one answer in list of answer)
 
         5. `get_topic`:
             Useful to classify the topic of conversation
         
         6. `match_or_make` (M&M):
             Get a match to a list of options, or make a new one if unrelated
             Useful if you aren't sure if the input will match one of your existing list options, and need flexibility of creating a new one
```

### Comparing `vector_vault-2.1.7/vectorvault/vault.py` & `vector_vault-2.1.8/vectorvault/vault.py`

 * *Files 1% similar despite different names*

```diff
@@ -443,14 +443,18 @@
         self.first_run = False
         if self.verbose == True:
             print("get vectors time --- %s seconds ---" % (time.time() - start_time))
 
     def get_chat(self, text: str, history: str = None, summary: bool = False, get_context = False, n_context = 4, return_context = False, history_search = False, model='gpt-3.5-turbo', include_context_meta=False, custom_prompt=False):
         '''
             Chat get response from OpenAI's ChatGPT. 
+            Models: ChatGPT = "gpt-3.5-turbo" • GPT4 = "gpt-4" 
+            Large Context Models: ChatGPT 16k = "gpt-3.5-turbo-16k" • GPT4 32k = "gpt-4-32k"
+            Best Versions: "gpt-3.5-turbo-0301" is March 2023 ChatGPT (best version) - "gpt-4-0314" (best version)
+
             Rate limiting, auto retries, and chat histroy slicing built-in so you can chat with ease. 
             Enter your text, add optional chat history, and optionally choose a summary response (default: summmary = False)
 
             - Example Signle Usage: 
             `response = vault.get_chat(text)`
 
             - Example Chat: 
@@ -512,15 +516,15 @@
                 (Respond to the Question directly. Be the voice of the context, and most importantly: be interesting, engaging, and helpful) 
                 Answer:
             """ 
             response = vault.get_chat(text, chat_history, get_context=True, custom_prompt=my_prompt)
             ```
 
         '''
-        
+
         model = model.lower()
         start_time = time.time()
         if not self.last_chat_time:
             self.last_chat_time = start_time - 20
         
         if not self.needed_sleep_time:
             self.needed_sleep_time = 0
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `vector_vault-2.1.7/vectorvault/vecreq.py` & `vector_vault-2.1.8/vectorvault/vecreq.py`

 * *Files identical despite different names*

