# Comparing `tmp/one-api-tool-0.5.6.tar.gz` & `tmp/one-api-tool-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "one-api-tool-0.5.6.tar", last modified: Sat Aug  5 03:34:45 2023, max compression
+gzip compressed data, was "one-api-tool-0.5.7.tar", last modified: Mon Aug  7 09:04:20 2023, max compression
```

## Comparing `one-api-tool-0.5.6.tar` & `one-api-tool-0.5.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-08-05 03:34:45.061313 one-api-tool-0.5.6/
--rw-r--r--   0 zhangchong   (501) staff       (20)     1055 2023-04-17 11:33:07.000000 one-api-tool-0.5.6/LICENSE
--rw-r--r--   0 zhangchong   (501) staff       (20)     8224 2023-08-05 03:34:45.061124 one-api-tool-0.5.6/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)     7668 2023-07-24 03:57:21.000000 one-api-tool-0.5.6/README.md
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-08-05 03:34:45.059042 one-api-tool-0.5.6/one_api_tool.egg-info/
--rw-r--r--   0 zhangchong   (501) staff       (20)     8224 2023-08-05 03:34:45.000000 one-api-tool-0.5.6/one_api_tool.egg-info/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)      382 2023-08-05 03:34:45.000000 one-api-tool-0.5.6/one_api_tool.egg-info/SOURCES.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-08-05 03:34:45.000000 one-api-tool-0.5.6/one_api_tool.egg-info/dependency_links.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       64 2023-08-05 03:34:45.000000 one-api-tool-0.5.6/one_api_tool.egg-info/entry_points.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       96 2023-08-05 03:34:45.000000 one-api-tool-0.5.6/one_api_tool.egg-info/requires.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        7 2023-08-05 03:34:45.000000 one-api-tool-0.5.6/one_api_tool.egg-info/top_level.txt
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-08-05 03:34:45.060238 one-api-tool-0.5.6/oneapi/
--rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-07-04 04:37:23.000000 one-api-tool-0.5.6/oneapi/__init__.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-08-05 03:34:45.060704 one-api-tool-0.5.6/oneapi/commands/
--rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-26 09:00:27.000000 one-api-tool-0.5.6/oneapi/commands/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     2168 2023-07-22 02:56:10.000000 one-api-tool-0.5.6/oneapi/commands/one_api_requst.py
--rw-r--r--   0 zhangchong   (501) staff       (20)    23838 2023-08-05 03:30:04.000000 one-api-tool-0.5.6/oneapi/one_api.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     1269 2023-08-05 03:32:39.000000 one-api-tool-0.5.6/oneapi/one_api_test.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     3598 2023-07-04 12:02:12.000000 one-api-tool-0.5.6/oneapi/utils.py
--rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-08-05 03:34:45.061360 one-api-tool-0.5.6/setup.cfg
--rw-r--r--   0 zhangchong   (501) staff       (20)     1099 2023-08-05 03:31:24.000000 one-api-tool-0.5.6/setup.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-08-07 09:04:20.793585 one-api-tool-0.5.7/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1055 2023-04-17 11:33:07.000000 one-api-tool-0.5.7/LICENSE
+-rw-r--r--   0 zhangchong   (501) staff       (20)     8224 2023-08-07 09:04:20.793349 one-api-tool-0.5.7/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)     7668 2023-07-24 03:57:21.000000 one-api-tool-0.5.7/README.md
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-08-07 09:04:20.791770 one-api-tool-0.5.7/one_api_tool.egg-info/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     8224 2023-08-07 09:04:20.000000 one-api-tool-0.5.7/one_api_tool.egg-info/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)      382 2023-08-07 09:04:20.000000 one-api-tool-0.5.7/one_api_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-08-07 09:04:20.000000 one-api-tool-0.5.7/one_api_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       64 2023-08-07 09:04:20.000000 one-api-tool-0.5.7/one_api_tool.egg-info/entry_points.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       96 2023-08-07 09:04:20.000000 one-api-tool-0.5.7/one_api_tool.egg-info/requires.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        7 2023-08-07 09:04:20.000000 one-api-tool-0.5.7/one_api_tool.egg-info/top_level.txt
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-08-07 09:04:20.792725 one-api-tool-0.5.7/oneapi/
+-rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-07-04 04:37:23.000000 one-api-tool-0.5.7/oneapi/__init__.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-08-07 09:04:20.792956 one-api-tool-0.5.7/oneapi/commands/
+-rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-26 09:00:27.000000 one-api-tool-0.5.7/oneapi/commands/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     2168 2023-07-22 02:56:10.000000 one-api-tool-0.5.7/oneapi/commands/one_api_requst.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)    24346 2023-08-07 09:02:19.000000 one-api-tool-0.5.7/oneapi/one_api.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1790 2023-08-07 09:03:58.000000 one-api-tool-0.5.7/oneapi/one_api_test.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     3598 2023-07-04 12:02:12.000000 one-api-tool-0.5.7/oneapi/utils.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-08-07 09:04:20.793644 one-api-tool-0.5.7/setup.cfg
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1099 2023-08-07 09:00:58.000000 one-api-tool-0.5.7/setup.py
```

### Comparing `one-api-tool-0.5.6/LICENSE` & `one-api-tool-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.5.6/PKG-INFO` & `one-api-tool-0.5.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: one-api-tool
-Version: 0.5.6
+Version: 0.5.7
 Summary: Use only one line of code to call multiple model APIs similar to ChatGPT. Currently supported: Azure OpenAI Resource endpoint API, OpenAI Official API, and Anthropic Claude series model API.
 Home-page: https://github.com/muximus3/OneAPI
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `one-api-tool-0.5.6/README.md` & `one-api-tool-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.5.6/one_api_tool.egg-info/PKG-INFO` & `one-api-tool-0.5.7/one_api_tool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: one-api-tool
-Version: 0.5.6
+Version: 0.5.7
 Summary: Use only one line of code to call multiple model APIs similar to ChatGPT. Currently supported: Azure OpenAI Resource endpoint API, OpenAI Official API, and Anthropic Claude series model API.
 Home-page: https://github.com/muximus3/OneAPI
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `one-api-tool-0.5.6/oneapi/commands/one_api_requst.py` & `one-api-tool-0.5.7/oneapi/commands/one_api_requst.py`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.5.6/oneapi/one_api.py` & `one-api-tool-0.5.7/oneapi/one_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -310,73 +310,87 @@
 
 
     @staticmethod
     def load_json(file_path):
         with open(file_path, "r") as f:
             return json.load(f)
 
-    def simple_chat(self, prompt: str|list|dict, system:str="", functions:List[Callable]=None, function_call:Optional[str|dict]=None, model:str="", temperature:int=1, max_new_tokens:int=2048, stream:bool=True, **kwargs):
-        if isinstance(self.tool, OpenAITool):
-            msgs = [] if not system else [dict(role="system", content=system)]
-            if isinstance(prompt, str):
-                msgs.append(dict(role="user", content=prompt))
-            elif isinstance(prompt, list):
-                msgs.extend(prompt)
-            elif isinstance(prompt, dict):
-                msgs.append(prompt)
+    @staticmethod 
+    def _preprocess_openai_prompt(prompt: str|list[str]|list[dict], system: str = "") -> List[dict]:
+        msgs = [] if not system else [dict(role="system", content=system)]
+        if isinstance(prompt, str):
+            msgs.append(dict(role="user", content=prompt))
+        elif isinstance(prompt, list) and isinstance(prompt[0], str):
+            msgs.extend([dict(role="user", content=p) if i%2 == 0 else dict(role='assistant', content=p) for i, p in enumerate(prompt)])
+        # for function calls
+        elif isinstance(prompt, list) and isinstance(prompt[0], dict):
+            msgs.extend(prompt)
+        else:
+            raise AssertionError(f"Prompt must be a string, list of strings. Got {type(prompt)} instead.")
+        return msgs
+    @staticmethod
+    def _preprocess_claude_prompt(prompt: str|list[str], system: str = "") -> str:
+        if isinstance(prompt, str):
+            return f"{anthropic.HUMAN_PROMPT} {prompt}{anthropic.AI_PROMPT}" if not system else f"{anthropic.HUMAN_PROMPT} {system}\n\n{prompt}{anthropic.AI_PROMPT}"
+        elif isinstance(prompt, list) and isinstance(prompt[0], str):
+            msg_list = [f"{anthropic.HUMAN_PROMPT} {p}" if i%2 == 0 else f"{anthropic.AI_PROMPT} {p}" for i, p in enumerate(prompt)]
+            if system:
+                msg_list[0] = f"{anthropic.HUMAN_PROMPT} {system}\n\n{prompt[0]}"
+            if len(msg_list) % 2 == 0:
+                msg_list.append(anthropic.HUMAN_PROMPT)
             else:
-                raise AssertionError(f"Prompt must be a string, list of strings, or ChatGPTMessage. Got {type(prompt)} instead.")
+                msg_list.append(anthropic.AI_PROMPT)
+            return "".join(msg_list)
+        else:
+            raise AssertionError(f"Prompt must be a string, list of strings. Got {type(prompt)} instead.")
+    def simple_chat(self, prompt: str|list[str]|list[dict], system:str="", functions:List[Callable]=None, function_call:Optional[str|dict]=None, model:str="", temperature:int=1, max_new_tokens:int=2048, stream:bool=True, **kwargs):
+        if isinstance(self.tool, OpenAITool):
+            msgs = self._preprocess_openai_prompt(prompt, system)
             if isinstance(self.tool.method, AzureMethod):
                 args = AzureDecodingArguments(messages=msgs, engine=model if model else "gpt-35-turbo", temperature=temperature, max_tokens=max_new_tokens, stream=stream, **kwargs)
             elif isinstance(self.tool.method, OpenAIMethod):
                 if functions is not None and isinstance(functions, list):
                     functions = [generate_function_description(func) for func in functions]
                 if function_call is None and functions is not None:
                     function_call = "auto"
                 if function_call is not None and functions is None:
                     function_call = None
                 args = OpenAIDecodingArguments(messages=msgs, functions=functions, function_call=function_call, model=model if model else "gpt-3.5-turbo-0613", temperature=temperature, max_tokens=max_new_tokens, stream=stream, **kwargs)
         elif isinstance(self.tool, ClaudeAITool):
-            args = ClaudeDecodingArguments(prompt=f"{anthropic.HUMAN_PROMPT} {prompt}{anthropic.AI_PROMPT}", model=model if model else "claude-2", temperature=temperature, max_tokens_to_sample=max_new_tokens, stream=stream, **kwargs)
+            prompt = self._preprocess_claude_prompt(prompt, system) 
+            args = ClaudeDecodingArguments(prompt=prompt, model=model if model else "claude-2", temperature=temperature, max_tokens_to_sample=max_new_tokens, stream=stream, **kwargs)
         else:
             raise AssertionError(f"Not supported api type: {type(self.tool)}")
 
         response = self.tool.simple_chat(args)
         return response
 
-    async def asimple_chat(self, prompt: str|list|dict, system:str="", functions:List[Callable]=None, function_call:Optional[str|dict]=None, model:str="", temperature:int=1, max_new_tokens:int=2048, stream:bool=False, **kwargs):
+    async def asimple_chat(self, prompt: str|list[str]|list[dict], system:str="", functions:List[Callable]=None, function_call:Optional[str|dict]=None, model:str="", temperature:int=1, max_new_tokens:int=2048, stream:bool=False, **kwargs):
         if isinstance(self.tool, OpenAITool):
-            msgs = [] if not system else [dict(role="system", content=system)]
-            if isinstance(prompt, str):
-                msgs.append(dict(role="user", content=prompt))
-            elif isinstance(prompt, list):
-                msgs.extend(prompt)
-            elif isinstance(prompt, dict):
-                msgs.append(prompt)
-            else:
-                raise AssertionError(f"Prompt must be a string, list of strings, or ChatGPTMessage. Got {type(prompt)} instead.")
+            msgs = self._preprocess_openai_prompt(prompt, system)
             if isinstance(self.tool.method, AzureMethod):
                 args = AzureDecodingArguments(messages=msgs, engine=model if model else "gpt-35-turbo", temperature=temperature, max_tokens=max_new_tokens, stream=stream, **kwargs)
             elif isinstance(self.tool.method, OpenAIMethod):
                 if functions is not None and isinstance(functions, list):
                     functions = [generate_function_description(func) for func in functions]
                 if function_call is None and functions is not None:
                     function_call = "auto"
                 if function_call is not None and functions is None:
                     function_call = None
                 args = OpenAIDecodingArguments(messages=msgs, functions=functions, function_call=function_call, model=model if model else "gpt-3.5-turbo-0613", temperature=temperature, max_tokens=max_new_tokens, stream=stream, **kwargs)
         elif isinstance(self.tool, ClaudeAITool):
-            args = ClaudeDecodingArguments(prompt=f"{anthropic.HUMAN_PROMPT} {prompt}{anthropic.AI_PROMPT}", model=model if model else "claude-2", temperature=temperature, max_tokens_to_sample=max_new_tokens, stream=stream, **kwargs)
+            prompt = self._preprocess_claude_prompt(prompt, system) 
+            args = ClaudeDecodingArguments(prompt=prompt, model=model if model else "claude-2", temperature=temperature, max_tokens_to_sample=max_new_tokens, stream=stream, **kwargs)
         else:
             raise AssertionError(f"Not supported api type: {type(self.tool)}")
 
         response = await self.tool.asimple_chat(args)
         return response
 
-    def function_chat(self, prompt: str|list|dict, system:str="", functions:List[Callable]=None, function_call:Optional[str|dict]=None, model:str="", temperature:int=1, max_new_tokens:int=2048, stream:bool=True, **kwargs):
+    def function_chat(self, prompt: str|list[str]|list[dict], system:str="", functions:List[Callable]=None, function_call:Optional[str|dict]=None, model:str="", temperature:int=1, max_new_tokens:int=2048, stream:bool=True, **kwargs):
         """A full chain of function calling.
         Step1: Call the model with functions and user prompt.
         Step2: Use the model response to call your API.
         Step3: Send the API response back to the model to summarize.
 
         Args:
             prompt (str | list | dict): User input.
@@ -389,23 +403,15 @@
             stream (bool, optional): Defaults to True.
 
         Raises:
             AssertionError: When no function response found. Usually because of prompt injection.
         """
         assert len(functions) > 0, "No functions found."
         if isinstance(self.tool, OpenAITool) and isinstance(self.tool.method, OpenAIMethod):
-            msgs = [] if not system else [dict(role="system", content=system)]
-            if isinstance(prompt, str):
-                msgs.append(dict(role="user", content=prompt))
-            elif isinstance(prompt, list):
-                msgs.extend(prompt)
-            elif isinstance(prompt, dict):
-                msgs.append(prompt)
-            else:
-                raise AssertionError(f"Prompt must be a string, list of strings, or ChatGPTMessage. Got {type(prompt)} instead.")
+            msgs = self._preprocess_openai_prompt(prompt, system)
             function_response = self.simple_chat(prompt, system, functions, function_call, model, temperature, max_new_tokens, stream, **kwargs)
             if not isinstance(function_response, dict) or not function_response.get("function_call"):
                 raise AssertionError(f"Function call not found in response: {function_response}")
             function_response_detail = function_response.get("function_call")
             logger.debug(f"Function calling step1, function_response_detail: {function_response_detail}")
             arguments = json.loads(function_response_detail["arguments"])
             function_name = function_response_detail["name"]
```

### Comparing `one-api-tool-0.5.6/oneapi/one_api_test.py` & `one-api-tool-0.5.7/oneapi/one_api_test.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,14 +18,20 @@
 
 if __name__ == "__main__":
     claude_config = '../ant/config/anthropic_config_personal.json'
     openai_config = '../ant/config/openapi_official_chenghao.json'
     azure_config = '../ant/config/openapi_azure_config_xiaoduo_dev.json'
     config_file = claude_config
     tool = OneAPITool.from_config_file(config_file)
+    print(tool._preprocess_claude_prompt('今天天气不错？', system='claude'))
+    print('='*20)
+    print(tool._preprocess_claude_prompt(['今天天气不错？','抱歉，我不知道你在说什么', '高血压吃什么药'], 'claude'))
+    # print(tool._preprocess_claude_prompt([dict(role='user',content='今天天气不错？')]))
+    # print(tool._preprocess_claude_prompt([dict(role='user',content='今天天气不错？'), dict(role='assistant',content='抱歉，我不知道你在说什么')]))
+    exit()
 
     prompt = '今天天气不错？'
     prompt = 'how is the weather today?'
     # print(tool.coust_tokens([prompt]))
     res = asyncio.run(tool.asimple_chat(prompt, stream=True))
     print(res)
     # res = asyncio.run(batch_chat([claude_config, openai_config, azure_config], ['心率异常可以局部麻醉吗', '今天天气不错？', '你好？', '上午是几点', '热天吃什么', '胖子爱出汗', '窦性心率是什么'], stream=False))
```

### Comparing `one-api-tool-0.5.6/oneapi/utils.py` & `one-api-tool-0.5.7/oneapi/utils.py`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.5.6/setup.py` & `one-api-tool-0.5.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="one-api-tool",
-    version="0.5.6",
+    version="0.5.7",
     packages=find_packages(),
     install_requires=[
         # Add your library's dependencies here
         "pydantic",
         "openai",
         "anthropic>=0.3",
         "requests",
```

