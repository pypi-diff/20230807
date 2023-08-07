# Comparing `tmp/litellm-0.1.351.tar.gz` & `tmp/litellm-0.1.352.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litellm-0.1.351.tar", max compression
+gzip compressed data, was "litellm-0.1.352.tar", max compression
```

## Comparing `litellm-0.1.351.tar` & `litellm-0.1.352.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     1065 2023-08-06 05:44:51.800746 litellm-0.1.351/LICENSE
--rw-r--r--   0        0        0     2575 2023-08-06 05:44:51.800746 litellm-0.1.351/README.md
--rw-r--r--   0        0        0     6148 2023-08-06 05:44:51.800746 litellm-0.1.351/litellm/.DS_Store
--rw-r--r--   0        0        0     2014 2023-08-06 05:44:51.800746 litellm-0.1.351/litellm/__init__.py
--rw-r--r--   0        0        0       15 2023-08-06 05:44:51.800746 litellm-0.1.351/litellm/integrations/__init__.py
--rw-r--r--   0        0        0      201 2023-08-06 05:44:51.800746 litellm-0.1.351/litellm/integrations/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     4923 2023-08-06 05:44:51.800746 litellm-0.1.351/litellm/integrations/__pycache__/aispend.cpython-311.pyc
--rw-r--r--   0        0        0     4690 2023-08-06 05:44:51.800746 litellm-0.1.351/litellm/integrations/__pycache__/berrispend.cpython-311.pyc
--rw-r--r--   0        0        0     4567 2023-08-06 05:44:51.800746 litellm-0.1.351/litellm/integrations/__pycache__/helicone.cpython-311.pyc
--rw-r--r--   0        0        0     5615 2023-08-06 05:44:51.800746 litellm-0.1.351/litellm/integrations/__pycache__/supabase.cpython-311.pyc
--rw-r--r--   0        0        0     5706 2023-08-06 05:44:51.800746 litellm-0.1.351/litellm/integrations/aispend.py
--rw-r--r--   0        0        0     5779 2023-08-06 05:44:51.800746 litellm-0.1.351/litellm/integrations/berrispend.py
--rw-r--r--   0        0        0     3548 2023-08-06 05:44:51.800746 litellm-0.1.351/litellm/integrations/helicone.py
--rw-r--r--   0        0        0     6294 2023-08-06 05:44:51.800746 litellm-0.1.351/litellm/integrations/supabase.py
--rw-r--r--   0        0        0    14045 2023-08-06 05:44:51.800746 litellm-0.1.351/litellm/main.py
--rw-r--r--   0        0        0     1580 2023-08-06 05:44:51.804746 litellm-0.1.351/litellm/tests/__pycache__/test_bad_params.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     3738 2023-08-06 05:44:51.804746 litellm-0.1.351/litellm/tests/__pycache__/test_client.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     5895 2023-08-06 05:44:51.804746 litellm-0.1.351/litellm/tests/__pycache__/test_completion.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     2732 2023-08-06 05:44:51.804746 litellm-0.1.351/litellm/tests/__pycache__/test_exceptions.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     2352 2023-08-06 05:44:51.804746 litellm-0.1.351/litellm/tests/__pycache__/test_logging.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     1468 2023-08-06 05:44:51.804746 litellm-0.1.351/litellm/tests/__pycache__/test_model_fallback.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     1289 2023-08-06 05:44:51.804746 litellm-0.1.351/litellm/tests/__pycache__/test_timeout.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0       36 2023-08-06 05:44:51.804746 litellm-0.1.351/litellm/tests/litellm_uuid.txt
--rw-r--r--   0        0        0      920 2023-08-06 05:44:51.804746 litellm-0.1.351/litellm/tests/test_api_key_param.py
--rw-r--r--   0        0        0      629 2023-08-06 05:44:51.804746 litellm-0.1.351/litellm/tests/test_async_fn.py
--rw-r--r--   0        0        0     1434 2023-08-06 05:44:51.804746 litellm-0.1.351/litellm/tests/test_bad_params.py
--rw-r--r--   0        0        0      863 2023-08-06 05:44:51.804746 litellm-0.1.351/litellm/tests/test_berrispend_integration.py
--rw-r--r--   0        0        0     2578 2023-08-06 05:44:51.804746 litellm-0.1.351/litellm/tests/test_client.py
--rw-r--r--   0        0        0     4537 2023-08-06 05:44:51.804746 litellm-0.1.351/litellm/tests/test_completion.py
--rw-r--r--   0        0        0     5840 2023-08-06 05:44:51.804746 litellm-0.1.351/litellm/tests/test_exceptions.py
--rw-r--r--   0        0        0      706 2023-08-06 05:44:51.804746 litellm-0.1.351/litellm/tests/test_helicone_integration.py
--rw-r--r--   0        0        0     1703 2023-08-06 05:44:51.804746 litellm-0.1.351/litellm/tests/test_logging.py
--rw-r--r--   0        0        0      852 2023-08-06 05:44:51.804746 litellm-0.1.351/litellm/tests/test_model_fallback.py
--rw-r--r--   0        0        0      960 2023-08-06 05:44:51.804746 litellm-0.1.351/litellm/tests/test_no_client.py
--rw-r--r--   0        0        0      506 2023-08-06 05:44:51.804746 litellm-0.1.351/litellm/tests/test_proxy_api.py
--rw-r--r--   0        0        0     1682 2023-08-06 05:44:51.804746 litellm-0.1.351/litellm/tests/test_secrets.py
--rw-r--r--   0        0        0      938 2023-08-06 05:44:51.804746 litellm-0.1.351/litellm/tests/test_supabase_integration.py
--rw-r--r--   0        0        0      530 2023-08-06 05:44:51.804746 litellm-0.1.351/litellm/tests/test_timeout.py
--rw-r--r--   0        0        0        6 2023-08-06 05:44:51.804746 litellm-0.1.351/litellm/tests.txt
--rw-r--r--   0        0        0     2893 2023-08-06 05:44:51.804746 litellm-0.1.351/litellm/timeout.py
--rw-r--r--   0        0        0    23684 2023-08-06 05:44:51.804746 litellm-0.1.351/litellm/utils.py
--rw-r--r--   0        0        0      512 2023-08-06 05:44:51.804746 litellm-0.1.351/pyproject.toml
--rw-r--r--   0        0        0     3431 1970-01-01 00:00:00.000000 litellm-0.1.351/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-08-07 17:45:52.674388 litellm-0.1.352/LICENSE
+-rw-r--r--   0        0        0     2617 2023-08-07 17:45:52.674388 litellm-0.1.352/README.md
+-rw-r--r--   0        0        0     6148 2023-08-07 17:45:52.674388 litellm-0.1.352/litellm/.DS_Store
+-rw-r--r--   0        0        0     2014 2023-08-07 17:45:52.674388 litellm-0.1.352/litellm/__init__.py
+-rw-r--r--   0        0        0       15 2023-08-07 17:45:52.674388 litellm-0.1.352/litellm/integrations/__init__.py
+-rw-r--r--   0        0        0      201 2023-08-07 17:45:52.674388 litellm-0.1.352/litellm/integrations/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     4923 2023-08-07 17:45:52.674388 litellm-0.1.352/litellm/integrations/__pycache__/aispend.cpython-311.pyc
+-rw-r--r--   0        0        0     4690 2023-08-07 17:45:52.674388 litellm-0.1.352/litellm/integrations/__pycache__/berrispend.cpython-311.pyc
+-rw-r--r--   0        0        0     4567 2023-08-07 17:45:52.674388 litellm-0.1.352/litellm/integrations/__pycache__/helicone.cpython-311.pyc
+-rw-r--r--   0        0        0     5615 2023-08-07 17:45:52.674388 litellm-0.1.352/litellm/integrations/__pycache__/supabase.cpython-311.pyc
+-rw-r--r--   0        0        0     5706 2023-08-07 17:45:52.674388 litellm-0.1.352/litellm/integrations/aispend.py
+-rw-r--r--   0        0        0     5779 2023-08-07 17:45:52.674388 litellm-0.1.352/litellm/integrations/berrispend.py
+-rw-r--r--   0        0        0     3548 2023-08-07 17:45:52.674388 litellm-0.1.352/litellm/integrations/helicone.py
+-rw-r--r--   0        0        0     6294 2023-08-07 17:45:52.674388 litellm-0.1.352/litellm/integrations/supabase.py
+-rw-r--r--   0        0        0    14057 2023-08-07 17:45:52.674388 litellm-0.1.352/litellm/main.py
+-rw-r--r--   0        0        0     1580 2023-08-07 17:45:52.674388 litellm-0.1.352/litellm/tests/__pycache__/test_bad_params.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     3738 2023-08-07 17:45:52.674388 litellm-0.1.352/litellm/tests/__pycache__/test_client.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     5895 2023-08-07 17:45:52.674388 litellm-0.1.352/litellm/tests/__pycache__/test_completion.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     2732 2023-08-07 17:45:52.674388 litellm-0.1.352/litellm/tests/__pycache__/test_exceptions.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     2352 2023-08-07 17:45:52.674388 litellm-0.1.352/litellm/tests/__pycache__/test_logging.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     1468 2023-08-07 17:45:52.674388 litellm-0.1.352/litellm/tests/__pycache__/test_model_fallback.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     1289 2023-08-07 17:45:52.674388 litellm-0.1.352/litellm/tests/__pycache__/test_timeout.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0       36 2023-08-07 17:45:52.674388 litellm-0.1.352/litellm/tests/litellm_uuid.txt
+-rw-r--r--   0        0        0      920 2023-08-07 17:45:52.674388 litellm-0.1.352/litellm/tests/test_api_key_param.py
+-rw-r--r--   0        0        0      629 2023-08-07 17:45:52.674388 litellm-0.1.352/litellm/tests/test_async_fn.py
+-rw-r--r--   0        0        0     1434 2023-08-07 17:45:52.674388 litellm-0.1.352/litellm/tests/test_bad_params.py
+-rw-r--r--   0        0        0      863 2023-08-07 17:45:52.678388 litellm-0.1.352/litellm/tests/test_berrispend_integration.py
+-rw-r--r--   0        0        0     2578 2023-08-07 17:45:52.678388 litellm-0.1.352/litellm/tests/test_client.py
+-rw-r--r--   0        0        0     4537 2023-08-07 17:45:52.678388 litellm-0.1.352/litellm/tests/test_completion.py
+-rw-r--r--   0        0        0     5840 2023-08-07 17:45:52.678388 litellm-0.1.352/litellm/tests/test_exceptions.py
+-rw-r--r--   0        0        0      706 2023-08-07 17:45:52.678388 litellm-0.1.352/litellm/tests/test_helicone_integration.py
+-rw-r--r--   0        0        0     1703 2023-08-07 17:45:52.678388 litellm-0.1.352/litellm/tests/test_logging.py
+-rw-r--r--   0        0        0      852 2023-08-07 17:45:52.678388 litellm-0.1.352/litellm/tests/test_model_fallback.py
+-rw-r--r--   0        0        0      960 2023-08-07 17:45:52.678388 litellm-0.1.352/litellm/tests/test_no_client.py
+-rw-r--r--   0        0        0      506 2023-08-07 17:45:52.678388 litellm-0.1.352/litellm/tests/test_proxy_api.py
+-rw-r--r--   0        0        0     1682 2023-08-07 17:45:52.678388 litellm-0.1.352/litellm/tests/test_secrets.py
+-rw-r--r--   0        0        0      938 2023-08-07 17:45:52.678388 litellm-0.1.352/litellm/tests/test_supabase_integration.py
+-rw-r--r--   0        0        0      530 2023-08-07 17:45:52.678388 litellm-0.1.352/litellm/tests/test_timeout.py
+-rw-r--r--   0        0        0        6 2023-08-07 17:45:52.674388 litellm-0.1.352/litellm/tests.txt
+-rw-r--r--   0        0        0     2893 2023-08-07 17:45:52.678388 litellm-0.1.352/litellm/timeout.py
+-rw-r--r--   0        0        0    23684 2023-08-07 17:45:52.678388 litellm-0.1.352/litellm/utils.py
+-rw-r--r--   0        0        0      512 2023-08-07 17:45:52.678388 litellm-0.1.352/pyproject.toml
+-rw-r--r--   0        0        0     3473 1970-01-01 00:00:00.000000 litellm-0.1.352/PKG-INFO
```

### Comparing `litellm-0.1.351/LICENSE` & `litellm-0.1.352/LICENSE`

 * *Files identical despite different names*

### Comparing `litellm-0.1.351/README.md` & `litellm-0.1.352/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # *🚅 litellm*
 [![PyPI Version](https://img.shields.io/pypi/v/litellm.svg)](https://pypi.org/project/litellm/)
-[![PyPI Version](https://img.shields.io/badge/stable%20version-v0.1.1-blue?color=green&link=https://pypi.org/project/litellm/0.1.1/)](https://pypi.org/project/litellm/0.1.1/)
+[![PyPI Version](https://img.shields.io/badge/stable%20version-v0.1.345-blue?color=green&link=https://pypi.org/project/litellm/0.1.1/)](https://pypi.org/project/litellm/0.1.1/)
 [![CircleCI](https://dl.circleci.com/status-badge/img/gh/BerriAI/litellm/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/BerriAI/litellm/tree/main)
 ![Downloads](https://img.shields.io/pypi/dm/litellm)
 [![litellm](https://img.shields.io/badge/%20%F0%9F%9A%85%20liteLLM-OpenAI%7CAzure%7CAnthropic%7CPalm%7CCohere-blue?color=green)](https://github.com/BerriAI/litellm)
 
-[![](https://dcbadge.vercel.app/api/server/wuPM9dRgDw)](https://discord.gg/wuPM9dRgDw)
+Get Support / Join the community 👉 [![](https://dcbadge.vercel.app/api/server/wuPM9dRgDw)](https://discord.gg/wuPM9dRgDw)
 
 a simple & light package to call OpenAI, Azure, Cohere, Anthropic API Endpoints 
 
 litellm manages:
 - translating inputs to completion and embedding endpoints
 - guarantees consistent output, text responses will always be available at `['choices'][0]['message']['content']`
 
@@ -44,15 +44,15 @@
 # openrouter call
 response = completion("google/palm-2-codechat-bison", messages)
 ```
 Code Sample: [Getting Started Notebook](https://colab.research.google.com/drive/1gR3pY-JzDZahzpVdbGBtrNGDBmzUNJaJ?usp=sharing)
 
 Stable version
 ```
-pip install litellm==0.1.1
+pip install litellm==0.1.345
 ```
 
 ## Streaming Queries
 liteLLM supports streaming the model response back, pass `stream=True` to get a streaming iterator in response.
 ```python
 response = completion(model="gpt-3.5-turbo", messages=messages, stream=True)
 for chunk in response:
```

### Comparing `litellm-0.1.351/litellm/.DS_Store` & `litellm-0.1.352/litellm/.DS_Store`

 * *Files identical despite different names*

### Comparing `litellm-0.1.351/litellm/__init__.py` & `litellm-0.1.352/litellm/__init__.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.351/litellm/integrations/__pycache__/aispend.cpython-311.pyc` & `litellm-0.1.352/litellm/integrations/__pycache__/aispend.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.351/litellm/integrations/__pycache__/berrispend.cpython-311.pyc` & `litellm-0.1.352/litellm/integrations/__pycache__/berrispend.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.351/litellm/integrations/__pycache__/helicone.cpython-311.pyc` & `litellm-0.1.352/litellm/integrations/__pycache__/helicone.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.351/litellm/integrations/__pycache__/supabase.cpython-311.pyc` & `litellm-0.1.352/litellm/integrations/__pycache__/supabase.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.351/litellm/integrations/aispend.py` & `litellm-0.1.352/litellm/integrations/aispend.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.351/litellm/integrations/berrispend.py` & `litellm-0.1.352/litellm/integrations/berrispend.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.351/litellm/integrations/helicone.py` & `litellm-0.1.352/litellm/integrations/helicone.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.351/litellm/integrations/supabase.py` & `litellm-0.1.352/litellm/integrations/supabase.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.351/litellm/main.py` & `litellm-0.1.352/litellm/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -225,15 +225,15 @@
         )
       completion_response = completion.completion
       ## LOGGING
       logging(model=model, input=prompt, azure=azure, additional_args={"max_tokens": max_tokens, "original_response": completion_response}, logger_fn=logger_fn)
       prompt_tokens = anthropic.count_tokens(prompt)
       completion_tokens = anthropic.count_tokens(completion_response)
       ## RESPONSE OBJECT
-      print(f"model_response: {model_response}")
+      print_verbose(f"raw model_response: {model_response}")
       model_response["choices"][0]["message"]["content"] = completion_response
       model_response["created"] = time.time()
       model_response["model"] = model
       model_response["usage"] = {
           "prompt_tokens": prompt_tokens,
           "completion_tokens": completion_tokens,
           "total_tokens": prompt_tokens + completion_tokens
```

### Comparing `litellm-0.1.351/litellm/tests/__pycache__/test_bad_params.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.352/litellm/tests/__pycache__/test_bad_params.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.351/litellm/tests/__pycache__/test_client.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.352/litellm/tests/__pycache__/test_client.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.351/litellm/tests/__pycache__/test_completion.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.352/litellm/tests/__pycache__/test_completion.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.351/litellm/tests/__pycache__/test_exceptions.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.352/litellm/tests/__pycache__/test_exceptions.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.351/litellm/tests/__pycache__/test_logging.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.352/litellm/tests/__pycache__/test_logging.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.351/litellm/tests/__pycache__/test_model_fallback.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.352/litellm/tests/__pycache__/test_model_fallback.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.351/litellm/tests/__pycache__/test_timeout.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.352/litellm/tests/__pycache__/test_timeout.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.351/litellm/tests/test_api_key_param.py` & `litellm-0.1.352/litellm/tests/test_api_key_param.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.351/litellm/tests/test_async_fn.py` & `litellm-0.1.352/litellm/tests/test_async_fn.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.351/litellm/tests/test_bad_params.py` & `litellm-0.1.352/litellm/tests/test_bad_params.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.351/litellm/tests/test_berrispend_integration.py` & `litellm-0.1.352/litellm/tests/test_berrispend_integration.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.351/litellm/tests/test_client.py` & `litellm-0.1.352/litellm/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.351/litellm/tests/test_completion.py` & `litellm-0.1.352/litellm/tests/test_completion.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.351/litellm/tests/test_exceptions.py` & `litellm-0.1.352/litellm/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.351/litellm/tests/test_helicone_integration.py` & `litellm-0.1.352/litellm/tests/test_helicone_integration.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.351/litellm/tests/test_logging.py` & `litellm-0.1.352/litellm/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.351/litellm/tests/test_model_fallback.py` & `litellm-0.1.352/litellm/tests/test_model_fallback.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.351/litellm/tests/test_no_client.py` & `litellm-0.1.352/litellm/tests/test_no_client.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.351/litellm/tests/test_secrets.py` & `litellm-0.1.352/litellm/tests/test_secrets.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.351/litellm/tests/test_supabase_integration.py` & `litellm-0.1.352/litellm/tests/test_supabase_integration.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.351/litellm/tests/test_timeout.py` & `litellm-0.1.352/litellm/tests/test_timeout.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.351/litellm/timeout.py` & `litellm-0.1.352/litellm/timeout.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.351/litellm/utils.py` & `litellm-0.1.352/litellm/utils.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.351/pyproject.toml` & `litellm-0.1.352/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "litellm"
-version = "0.1.351"
+version = "0.1.352"
 description = "Library to easily interface with LLM API providers"
 authors = ["BerriAI"]
 license = "MIT License"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `litellm-0.1.351/PKG-INFO` & `litellm-0.1.352/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litellm
-Version: 0.1.351
+Version: 0.1.352
 Summary: Library to easily interface with LLM API providers
 License: MIT
 Author: BerriAI
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -19,20 +19,20 @@
 Requires-Dist: replicate (>=0.10.0,<0.11.0)
 Requires-Dist: tenacity (>=8.0.1,<9.0.0)
 Requires-Dist: tiktoken (>=0.4.0,<0.5.0)
 Description-Content-Type: text/markdown
 
 # *🚅 litellm*
 [![PyPI Version](https://img.shields.io/pypi/v/litellm.svg)](https://pypi.org/project/litellm/)
-[![PyPI Version](https://img.shields.io/badge/stable%20version-v0.1.1-blue?color=green&link=https://pypi.org/project/litellm/0.1.1/)](https://pypi.org/project/litellm/0.1.1/)
+[![PyPI Version](https://img.shields.io/badge/stable%20version-v0.1.345-blue?color=green&link=https://pypi.org/project/litellm/0.1.1/)](https://pypi.org/project/litellm/0.1.1/)
 [![CircleCI](https://dl.circleci.com/status-badge/img/gh/BerriAI/litellm/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/BerriAI/litellm/tree/main)
 ![Downloads](https://img.shields.io/pypi/dm/litellm)
 [![litellm](https://img.shields.io/badge/%20%F0%9F%9A%85%20liteLLM-OpenAI%7CAzure%7CAnthropic%7CPalm%7CCohere-blue?color=green)](https://github.com/BerriAI/litellm)
 
-[![](https://dcbadge.vercel.app/api/server/wuPM9dRgDw)](https://discord.gg/wuPM9dRgDw)
+Get Support / Join the community 👉 [![](https://dcbadge.vercel.app/api/server/wuPM9dRgDw)](https://discord.gg/wuPM9dRgDw)
 
 a simple & light package to call OpenAI, Azure, Cohere, Anthropic API Endpoints 
 
 litellm manages:
 - translating inputs to completion and embedding endpoints
 - guarantees consistent output, text responses will always be available at `['choices'][0]['message']['content']`
 
@@ -67,15 +67,15 @@
 # openrouter call
 response = completion("google/palm-2-codechat-bison", messages)
 ```
 Code Sample: [Getting Started Notebook](https://colab.research.google.com/drive/1gR3pY-JzDZahzpVdbGBtrNGDBmzUNJaJ?usp=sharing)
 
 Stable version
 ```
-pip install litellm==0.1.1
+pip install litellm==0.1.345
 ```
 
 ## Streaming Queries
 liteLLM supports streaming the model response back, pass `stream=True` to get a streaming iterator in response.
 ```python
 response = completion(model="gpt-3.5-turbo", messages=messages, stream=True)
 for chunk in response:
```

