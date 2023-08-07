# Comparing `tmp/litellm-0.1.352.tar.gz` & `tmp/litellm-0.1.353.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litellm-0.1.352.tar", max compression
+gzip compressed data, was "litellm-0.1.353.tar", max compression
```

## Comparing `litellm-0.1.352.tar` & `litellm-0.1.353.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     1065 2023-08-07 17:45:52.674388 litellm-0.1.352/LICENSE
--rw-r--r--   0        0        0     2617 2023-08-07 17:45:52.674388 litellm-0.1.352/README.md
--rw-r--r--   0        0        0     6148 2023-08-07 17:45:52.674388 litellm-0.1.352/litellm/.DS_Store
--rw-r--r--   0        0        0     2014 2023-08-07 17:45:52.674388 litellm-0.1.352/litellm/__init__.py
--rw-r--r--   0        0        0       15 2023-08-07 17:45:52.674388 litellm-0.1.352/litellm/integrations/__init__.py
--rw-r--r--   0        0        0      201 2023-08-07 17:45:52.674388 litellm-0.1.352/litellm/integrations/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     4923 2023-08-07 17:45:52.674388 litellm-0.1.352/litellm/integrations/__pycache__/aispend.cpython-311.pyc
--rw-r--r--   0        0        0     4690 2023-08-07 17:45:52.674388 litellm-0.1.352/litellm/integrations/__pycache__/berrispend.cpython-311.pyc
--rw-r--r--   0        0        0     4567 2023-08-07 17:45:52.674388 litellm-0.1.352/litellm/integrations/__pycache__/helicone.cpython-311.pyc
--rw-r--r--   0        0        0     5615 2023-08-07 17:45:52.674388 litellm-0.1.352/litellm/integrations/__pycache__/supabase.cpython-311.pyc
--rw-r--r--   0        0        0     5706 2023-08-07 17:45:52.674388 litellm-0.1.352/litellm/integrations/aispend.py
--rw-r--r--   0        0        0     5779 2023-08-07 17:45:52.674388 litellm-0.1.352/litellm/integrations/berrispend.py
--rw-r--r--   0        0        0     3548 2023-08-07 17:45:52.674388 litellm-0.1.352/litellm/integrations/helicone.py
--rw-r--r--   0        0        0     6294 2023-08-07 17:45:52.674388 litellm-0.1.352/litellm/integrations/supabase.py
--rw-r--r--   0        0        0    14057 2023-08-07 17:45:52.674388 litellm-0.1.352/litellm/main.py
--rw-r--r--   0        0        0     1580 2023-08-07 17:45:52.674388 litellm-0.1.352/litellm/tests/__pycache__/test_bad_params.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     3738 2023-08-07 17:45:52.674388 litellm-0.1.352/litellm/tests/__pycache__/test_client.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     5895 2023-08-07 17:45:52.674388 litellm-0.1.352/litellm/tests/__pycache__/test_completion.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     2732 2023-08-07 17:45:52.674388 litellm-0.1.352/litellm/tests/__pycache__/test_exceptions.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     2352 2023-08-07 17:45:52.674388 litellm-0.1.352/litellm/tests/__pycache__/test_logging.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     1468 2023-08-07 17:45:52.674388 litellm-0.1.352/litellm/tests/__pycache__/test_model_fallback.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     1289 2023-08-07 17:45:52.674388 litellm-0.1.352/litellm/tests/__pycache__/test_timeout.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0       36 2023-08-07 17:45:52.674388 litellm-0.1.352/litellm/tests/litellm_uuid.txt
--rw-r--r--   0        0        0      920 2023-08-07 17:45:52.674388 litellm-0.1.352/litellm/tests/test_api_key_param.py
--rw-r--r--   0        0        0      629 2023-08-07 17:45:52.674388 litellm-0.1.352/litellm/tests/test_async_fn.py
--rw-r--r--   0        0        0     1434 2023-08-07 17:45:52.674388 litellm-0.1.352/litellm/tests/test_bad_params.py
--rw-r--r--   0        0        0      863 2023-08-07 17:45:52.678388 litellm-0.1.352/litellm/tests/test_berrispend_integration.py
--rw-r--r--   0        0        0     2578 2023-08-07 17:45:52.678388 litellm-0.1.352/litellm/tests/test_client.py
--rw-r--r--   0        0        0     4537 2023-08-07 17:45:52.678388 litellm-0.1.352/litellm/tests/test_completion.py
--rw-r--r--   0        0        0     5840 2023-08-07 17:45:52.678388 litellm-0.1.352/litellm/tests/test_exceptions.py
--rw-r--r--   0        0        0      706 2023-08-07 17:45:52.678388 litellm-0.1.352/litellm/tests/test_helicone_integration.py
--rw-r--r--   0        0        0     1703 2023-08-07 17:45:52.678388 litellm-0.1.352/litellm/tests/test_logging.py
--rw-r--r--   0        0        0      852 2023-08-07 17:45:52.678388 litellm-0.1.352/litellm/tests/test_model_fallback.py
--rw-r--r--   0        0        0      960 2023-08-07 17:45:52.678388 litellm-0.1.352/litellm/tests/test_no_client.py
--rw-r--r--   0        0        0      506 2023-08-07 17:45:52.678388 litellm-0.1.352/litellm/tests/test_proxy_api.py
--rw-r--r--   0        0        0     1682 2023-08-07 17:45:52.678388 litellm-0.1.352/litellm/tests/test_secrets.py
--rw-r--r--   0        0        0      938 2023-08-07 17:45:52.678388 litellm-0.1.352/litellm/tests/test_supabase_integration.py
--rw-r--r--   0        0        0      530 2023-08-07 17:45:52.678388 litellm-0.1.352/litellm/tests/test_timeout.py
--rw-r--r--   0        0        0        6 2023-08-07 17:45:52.674388 litellm-0.1.352/litellm/tests.txt
--rw-r--r--   0        0        0     2893 2023-08-07 17:45:52.678388 litellm-0.1.352/litellm/timeout.py
--rw-r--r--   0        0        0    23684 2023-08-07 17:45:52.678388 litellm-0.1.352/litellm/utils.py
--rw-r--r--   0        0        0      512 2023-08-07 17:45:52.678388 litellm-0.1.352/pyproject.toml
--rw-r--r--   0        0        0     3473 1970-01-01 00:00:00.000000 litellm-0.1.352/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-08-07 18:33:49.640112 litellm-0.1.353/LICENSE
+-rw-r--r--   0        0        0     2617 2023-08-07 18:33:49.640112 litellm-0.1.353/README.md
+-rw-r--r--   0        0        0     6148 2023-08-07 18:33:49.644112 litellm-0.1.353/litellm/.DS_Store
+-rw-r--r--   0        0        0     2134 2023-08-07 18:33:49.644112 litellm-0.1.353/litellm/__init__.py
+-rw-r--r--   0        0        0       15 2023-08-07 18:33:49.644112 litellm-0.1.353/litellm/integrations/__init__.py
+-rw-r--r--   0        0        0      201 2023-08-07 18:33:49.644112 litellm-0.1.353/litellm/integrations/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     4923 2023-08-07 18:33:49.644112 litellm-0.1.353/litellm/integrations/__pycache__/aispend.cpython-311.pyc
+-rw-r--r--   0        0        0     4690 2023-08-07 18:33:49.644112 litellm-0.1.353/litellm/integrations/__pycache__/berrispend.cpython-311.pyc
+-rw-r--r--   0        0        0     4567 2023-08-07 18:33:49.644112 litellm-0.1.353/litellm/integrations/__pycache__/helicone.cpython-311.pyc
+-rw-r--r--   0        0        0     5615 2023-08-07 18:33:49.644112 litellm-0.1.353/litellm/integrations/__pycache__/supabase.cpython-311.pyc
+-rw-r--r--   0        0        0     5706 2023-08-07 18:33:49.644112 litellm-0.1.353/litellm/integrations/aispend.py
+-rw-r--r--   0        0        0     5779 2023-08-07 18:33:49.644112 litellm-0.1.353/litellm/integrations/berrispend.py
+-rw-r--r--   0        0        0     3548 2023-08-07 18:33:49.644112 litellm-0.1.353/litellm/integrations/helicone.py
+-rw-r--r--   0        0        0     6294 2023-08-07 18:33:49.644112 litellm-0.1.353/litellm/integrations/supabase.py
+-rw-r--r--   0        0        0    14057 2023-08-07 18:33:49.644112 litellm-0.1.353/litellm/main.py
+-rw-r--r--   0        0        0     1580 2023-08-07 18:33:49.644112 litellm-0.1.353/litellm/tests/__pycache__/test_bad_params.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     3738 2023-08-07 18:33:49.644112 litellm-0.1.353/litellm/tests/__pycache__/test_client.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     5895 2023-08-07 18:33:49.644112 litellm-0.1.353/litellm/tests/__pycache__/test_completion.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     2732 2023-08-07 18:33:49.644112 litellm-0.1.353/litellm/tests/__pycache__/test_exceptions.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     2352 2023-08-07 18:33:49.644112 litellm-0.1.353/litellm/tests/__pycache__/test_logging.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     1468 2023-08-07 18:33:49.644112 litellm-0.1.353/litellm/tests/__pycache__/test_model_fallback.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     1289 2023-08-07 18:33:49.644112 litellm-0.1.353/litellm/tests/__pycache__/test_timeout.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0       36 2023-08-07 18:33:49.644112 litellm-0.1.353/litellm/tests/litellm_uuid.txt
+-rw-r--r--   0        0        0      920 2023-08-07 18:33:49.644112 litellm-0.1.353/litellm/tests/test_api_key_param.py
+-rw-r--r--   0        0        0      629 2023-08-07 18:33:49.644112 litellm-0.1.353/litellm/tests/test_async_fn.py
+-rw-r--r--   0        0        0     1434 2023-08-07 18:33:49.644112 litellm-0.1.353/litellm/tests/test_bad_params.py
+-rw-r--r--   0        0        0      863 2023-08-07 18:33:49.644112 litellm-0.1.353/litellm/tests/test_berrispend_integration.py
+-rw-r--r--   0        0        0     2578 2023-08-07 18:33:49.644112 litellm-0.1.353/litellm/tests/test_client.py
+-rw-r--r--   0        0        0     4537 2023-08-07 18:33:49.644112 litellm-0.1.353/litellm/tests/test_completion.py
+-rw-r--r--   0        0        0     5938 2023-08-07 18:33:49.644112 litellm-0.1.353/litellm/tests/test_exceptions.py
+-rw-r--r--   0        0        0      706 2023-08-07 18:33:49.644112 litellm-0.1.353/litellm/tests/test_helicone_integration.py
+-rw-r--r--   0        0        0     1703 2023-08-07 18:33:49.644112 litellm-0.1.353/litellm/tests/test_logging.py
+-rw-r--r--   0        0        0      852 2023-08-07 18:33:49.644112 litellm-0.1.353/litellm/tests/test_model_fallback.py
+-rw-r--r--   0        0        0      960 2023-08-07 18:33:49.644112 litellm-0.1.353/litellm/tests/test_no_client.py
+-rw-r--r--   0        0        0      506 2023-08-07 18:33:49.644112 litellm-0.1.353/litellm/tests/test_proxy_api.py
+-rw-r--r--   0        0        0     1682 2023-08-07 18:33:49.644112 litellm-0.1.353/litellm/tests/test_secrets.py
+-rw-r--r--   0        0        0      938 2023-08-07 18:33:49.644112 litellm-0.1.353/litellm/tests/test_supabase_integration.py
+-rw-r--r--   0        0        0      530 2023-08-07 18:33:49.644112 litellm-0.1.353/litellm/tests/test_timeout.py
+-rw-r--r--   0        0        0        6 2023-08-07 18:33:49.644112 litellm-0.1.353/litellm/tests.txt
+-rw-r--r--   0        0        0     2893 2023-08-07 18:33:49.648113 litellm-0.1.353/litellm/timeout.py
+-rw-r--r--   0        0        0    23684 2023-08-07 18:33:49.648113 litellm-0.1.353/litellm/utils.py
+-rw-r--r--   0        0        0      512 2023-08-07 18:33:49.648113 litellm-0.1.353/pyproject.toml
+-rw-r--r--   0        0        0     3473 1970-01-01 00:00:00.000000 litellm-0.1.353/PKG-INFO
```

### Comparing `litellm-0.1.352/LICENSE` & `litellm-0.1.353/LICENSE`

 * *Files identical despite different names*

### Comparing `litellm-0.1.352/README.md` & `litellm-0.1.353/README.md`

 * *Files identical despite different names*

### Comparing `litellm-0.1.352/litellm/.DS_Store` & `litellm-0.1.353/litellm/.DS_Store`

 * *Files identical despite different names*

### Comparing `litellm-0.1.352/litellm/__init__.py` & `litellm-0.1.353/litellm/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -68,8 +68,9 @@
 ####### EMBEDDING MODELS ###################
 open_ai_embedding_models = [
     'text-embedding-ada-002'
 ]
 from .timeout import timeout
 from .utils import client, logging, exception_type, get_optional_params, modify_integration
 from .main import *  # Import all the symbols from main.py
-from .integrations import *
+from .integrations import *
+from openai.error import AuthenticationError, InvalidRequestError, RateLimitError, ServiceUnavailableError, OpenAIError
```

### Comparing `litellm-0.1.352/litellm/integrations/__pycache__/aispend.cpython-311.pyc` & `litellm-0.1.353/litellm/integrations/__pycache__/aispend.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.352/litellm/integrations/__pycache__/berrispend.cpython-311.pyc` & `litellm-0.1.353/litellm/integrations/__pycache__/berrispend.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.352/litellm/integrations/__pycache__/helicone.cpython-311.pyc` & `litellm-0.1.353/litellm/integrations/__pycache__/helicone.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.352/litellm/integrations/__pycache__/supabase.cpython-311.pyc` & `litellm-0.1.353/litellm/integrations/__pycache__/supabase.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.352/litellm/integrations/aispend.py` & `litellm-0.1.353/litellm/integrations/aispend.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.352/litellm/integrations/berrispend.py` & `litellm-0.1.353/litellm/integrations/berrispend.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.352/litellm/integrations/helicone.py` & `litellm-0.1.353/litellm/integrations/helicone.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.352/litellm/integrations/supabase.py` & `litellm-0.1.353/litellm/integrations/supabase.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.352/litellm/main.py` & `litellm-0.1.353/litellm/main.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.352/litellm/tests/__pycache__/test_bad_params.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.353/litellm/tests/__pycache__/test_bad_params.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.352/litellm/tests/__pycache__/test_client.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.353/litellm/tests/__pycache__/test_client.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.352/litellm/tests/__pycache__/test_completion.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.353/litellm/tests/__pycache__/test_completion.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.352/litellm/tests/__pycache__/test_exceptions.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.353/litellm/tests/__pycache__/test_exceptions.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.352/litellm/tests/__pycache__/test_logging.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.353/litellm/tests/__pycache__/test_logging.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.352/litellm/tests/__pycache__/test_model_fallback.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.353/litellm/tests/__pycache__/test_model_fallback.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.352/litellm/tests/__pycache__/test_timeout.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.353/litellm/tests/__pycache__/test_timeout.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.352/litellm/tests/test_api_key_param.py` & `litellm-0.1.353/litellm/tests/test_api_key_param.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.352/litellm/tests/test_async_fn.py` & `litellm-0.1.353/litellm/tests/test_async_fn.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.352/litellm/tests/test_bad_params.py` & `litellm-0.1.353/litellm/tests/test_bad_params.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.352/litellm/tests/test_berrispend_integration.py` & `litellm-0.1.353/litellm/tests/test_berrispend_integration.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.352/litellm/tests/test_client.py` & `litellm-0.1.353/litellm/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.352/litellm/tests/test_completion.py` & `litellm-0.1.353/litellm/tests/test_completion.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.352/litellm/tests/test_exceptions.py` & `litellm-0.1.353/litellm/tests/test_exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from openai.error import AuthenticationError, InvalidRequestError, RateLimitError, OpenAIError
+# from openai.error import AuthenticationError, InvalidRequestError, RateLimitError, OpenAIError
 import os 
 import sys
 import traceback
 sys.path.insert(0, os.path.abspath('../..'))  # Adds the parent directory to the system path
 import litellm
-from litellm import embedding, completion
+from litellm import embedding, completion, AuthenticationError, InvalidRequestError, RateLimitError, ServiceUnavailableError, OpenAIError
 from concurrent.futures import ThreadPoolExecutor
 import pytest
 
 litellm.failure_callback = ["sentry"]
 # litellm.set_verbose = True
 #### What this tests ####
 #    This tests exception mapping -> trigger an exception from an llm provider -> assert if output is of the expected type
```

### Comparing `litellm-0.1.352/litellm/tests/test_helicone_integration.py` & `litellm-0.1.353/litellm/tests/test_helicone_integration.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.352/litellm/tests/test_logging.py` & `litellm-0.1.353/litellm/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.352/litellm/tests/test_model_fallback.py` & `litellm-0.1.353/litellm/tests/test_model_fallback.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.352/litellm/tests/test_no_client.py` & `litellm-0.1.353/litellm/tests/test_no_client.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.352/litellm/tests/test_secrets.py` & `litellm-0.1.353/litellm/tests/test_secrets.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.352/litellm/tests/test_supabase_integration.py` & `litellm-0.1.353/litellm/tests/test_supabase_integration.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.352/litellm/tests/test_timeout.py` & `litellm-0.1.353/litellm/tests/test_timeout.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.352/litellm/timeout.py` & `litellm-0.1.353/litellm/timeout.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.352/litellm/utils.py` & `litellm-0.1.353/litellm/utils.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.352/pyproject.toml` & `litellm-0.1.353/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "litellm"
-version = "0.1.352"
+version = "0.1.353"
 description = "Library to easily interface with LLM API providers"
 authors = ["BerriAI"]
 license = "MIT License"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `litellm-0.1.352/PKG-INFO` & `litellm-0.1.353/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litellm
-Version: 0.1.352
+Version: 0.1.353
 Summary: Library to easily interface with LLM API providers
 License: MIT
 Author: BerriAI
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

