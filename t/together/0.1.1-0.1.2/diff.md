# Comparing `tmp/together-0.1.1.tar.gz` & `tmp/together-0.1.2.tar.gz`

## Comparing `together-0.1.1.tar` & `together-0.1.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 together-0.1.1/.github/workflows/check_code_quality.yml
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 together-0.1.1/src/together/__init__.py
--rw-r--r--   0        0        0     4800 2020-02-02 00:00:00.000000 together-0.1.1/src/together/complete.py
--rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 together-0.1.1/src/together/error.py
--rw-r--r--   0        0        0     9081 2020-02-02 00:00:00.000000 together-0.1.1/src/together/files.py
--rw-r--r--   0        0        0    10886 2020-02-02 00:00:00.000000 together-0.1.1/src/together/finetune.py
--rw-r--r--   0        0        0     2167 2020-02-02 00:00:00.000000 together-0.1.1/src/together/image.py
--rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 together-0.1.1/src/together/models.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 together-0.1.1/src/together/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 together-0.1.1/src/together/cli/__init__.py
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 together-0.1.1/src/together/cli/cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 together-0.1.1/src/together/commands/__init__.py
--rw-r--r--   0        0        0     4098 2020-02-02 00:00:00.000000 together-0.1.1/src/together/commands/chat.py
--rw-r--r--   0        0        0     5107 2020-02-02 00:00:00.000000 together-0.1.1/src/together/commands/complete.py
--rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 together-0.1.1/src/together/commands/files.py
--rw-r--r--   0        0        0     9224 2020-02-02 00:00:00.000000 together-0.1.1/src/together/commands/finetune.py
--rw-r--r--   0        0        0     3692 2020-02-02 00:00:00.000000 together-0.1.1/src/together/commands/image.py
--rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 together-0.1.1/src/together/commands/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 together-0.1.1/src/together/utils/__init__.py
--rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 together-0.1.1/src/together/utils/conversation.py
--rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 together-0.1.1/src/together/utils/utils.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 together-0.1.1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 together-0.1.1/LICENSE
--rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 together-0.1.1/README.md
--rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 together-0.1.1/pyproject.toml
--rw-r--r--   0        0        0    17569 2020-02-02 00:00:00.000000 together-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 together-0.1.2/.github/workflows/check_code_quality.yml
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 together-0.1.2/src/together/__init__.py
+-rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 together-0.1.2/src/together/complete.py
+-rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 together-0.1.2/src/together/error.py
+-rw-r--r--   0        0        0     9081 2020-02-02 00:00:00.000000 together-0.1.2/src/together/files.py
+-rw-r--r--   0        0        0    10886 2020-02-02 00:00:00.000000 together-0.1.2/src/together/finetune.py
+-rw-r--r--   0        0        0     2167 2020-02-02 00:00:00.000000 together-0.1.2/src/together/image.py
+-rw-r--r--   0        0        0     4029 2020-02-02 00:00:00.000000 together-0.1.2/src/together/models.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 together-0.1.2/src/together/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 together-0.1.2/src/together/cli/__init__.py
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 together-0.1.2/src/together/cli/cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 together-0.1.2/src/together/commands/__init__.py
+-rw-r--r--   0        0        0     4098 2020-02-02 00:00:00.000000 together-0.1.2/src/together/commands/chat.py
+-rw-r--r--   0        0        0     5107 2020-02-02 00:00:00.000000 together-0.1.2/src/together/commands/complete.py
+-rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 together-0.1.2/src/together/commands/files.py
+-rw-r--r--   0        0        0     9224 2020-02-02 00:00:00.000000 together-0.1.2/src/together/commands/finetune.py
+-rw-r--r--   0        0        0     3692 2020-02-02 00:00:00.000000 together-0.1.2/src/together/commands/image.py
+-rw-r--r--   0        0        0     3884 2020-02-02 00:00:00.000000 together-0.1.2/src/together/commands/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 together-0.1.2/src/together/utils/__init__.py
+-rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 together-0.1.2/src/together/utils/conversation.py
+-rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 together-0.1.2/src/together/utils/utils.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 together-0.1.2/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 together-0.1.2/LICENSE
+-rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 together-0.1.2/README.md
+-rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 together-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0    18574 2020-02-02 00:00:00.000000 together-0.1.2/PKG-INFO
```

### Comparing `together-0.1.1/.github/workflows/check_code_quality.yml` & `together-0.1.2/.github/workflows/check_code_quality.yml`

 * *Files identical despite different names*

### Comparing `together-0.1.1/src/together/__init__.py` & `together-0.1.2/src/together/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 api_key = os.environ.get("TOGETHER_API_KEY", None)
 
 api_base = "https://api.together.xyz/"
 api_base_complete = urllib.parse.urljoin(api_base, "/api/inference")
 api_base_files = urllib.parse.urljoin(api_base, "/v1/files/")
 api_base_finetune = urllib.parse.urljoin(api_base, "/v1/fine-tunes/")
+api_base_instances = urllib.parse.urljoin(api_base, "instances/")
 
 default_text_model = "togethercomputer/RedPajama-INCITE-7B-Chat"
 default_image_model = "runwayml/stable-diffusion-v1-5"
 log_level = "WARNING"
 
 from .utils.utils import get_logger, verify_api_key, extract_time  # noqa
 from .models import Models
@@ -30,14 +31,15 @@
 
 __all__ = [
     "api_key",
     "api_base",
     "api_base_complete",
     "api_base_files",
     "api_base_finetune",
+    "api_base_instances",
     "default_text_model",
     "default_image_model",
     "get_logger",
     "verify_api_key",
     "extract_time",
     "Models",
     "Complete",
```

### Comparing `together-0.1.1/src/together/complete.py` & `together-0.1.2/src/together/complete.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import json
-from typing import Any, Dict, Iterator, Optional
+from typing import Any, Dict, Iterator, List, Optional
 
 import requests
 import sseclient  # type: ignore
 
 import together
 from together import get_logger, verify_api_key
 
@@ -19,15 +19,15 @@
 
     @classmethod
     def create(
         self,
         prompt: str,
         model: Optional[str] = "",
         max_tokens: Optional[int] = 128,
-        stop: Optional[str] = None,
+        stop: Optional[List[str]] = [],
         temperature: Optional[float] = 0.7,
         top_p: Optional[float] = 0.7,
         top_k: Optional[int] = 50,
         repetition_penalty: Optional[float] = None,
         logprobs: Optional[int] = None,
     ) -> Dict[str, Any]:
         if model == "":
```

### Comparing `together-0.1.1/src/together/error.py` & `together-0.1.2/src/together/error.py`

 * *Files identical despite different names*

### Comparing `together-0.1.1/src/together/files.py` & `together-0.1.2/src/together/files.py`

 * *Files identical despite different names*

### Comparing `together-0.1.1/src/together/finetune.py` & `together-0.1.2/src/together/finetune.py`

 * *Files identical despite different names*

### Comparing `together-0.1.1/src/together/image.py` & `together-0.1.2/src/together/image.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         verify_api_key(logger)
 
     @classmethod
     def create(
         self,
         prompt: str,
         model: Optional[str] = "",
-        steps: Optional[int] = 50,
+        steps: Optional[int] = 20,
         seed: Optional[int] = 42,
         results: Optional[int] = 1,
         height: Optional[int] = 256,
         width: Optional[int] = 256,
     ) -> Dict[str, Any]:
         if model == "":
             model = together.default_image_model
```

### Comparing `together-0.1.1/src/together/cli/cli.py` & `together-0.1.2/src/together/cli/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,14 +9,21 @@
 def main() -> None:
     parser = argparse.ArgumentParser(
         description="Together Python Library",
         prog="together",
     )
 
     parser.add_argument(
+        "-V",
+        "--version",
+        action="version",
+        version="%(prog)s " + together.version,
+    )
+
+    parser.add_argument(
         "--endpoint",
         "-e",
         help="[Optional] Together API Endpoint URL",
         type=str,
         required=False,
         default=None,
     )
```

### Comparing `together-0.1.1/src/together/commands/chat.py` & `together-0.1.2/src/together/commands/chat.py`

 * *Files identical despite different names*

### Comparing `together-0.1.1/src/together/commands/complete.py` & `together-0.1.2/src/together/commands/complete.py`

 * *Files identical despite different names*

### Comparing `together-0.1.1/src/together/commands/files.py` & `together-0.1.2/src/together/commands/files.py`

 * *Files identical despite different names*

### Comparing `together-0.1.1/src/together/commands/finetune.py` & `together-0.1.2/src/together/commands/finetune.py`

 * *Files identical despite different names*

### Comparing `together-0.1.1/src/together/commands/image.py` & `together-0.1.2/src/together/commands/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,27 +29,27 @@
         default=together.default_image_model,
         type=str,
         help=f"The name of the model to query. Default={together.default_image_model}",
     )
 
     subparser.add_argument(
         "--height",
-        default=512,
+        default=256,
         type=int,
         help="Pixel height for generated image results",
     )
     subparser.add_argument(
         "--width",
-        default=512,
+        default=256,
         type=int,
         help="Pixel width for generated image results",
     )
     subparser.add_argument(
         "--steps",
-        default=50,
+        default=20,
         type=int,
         help="Number of steps",
     )
     subparser.add_argument(
         "--seed",
         default=42,
         type=int,
```

### Comparing `together-0.1.1/src/together/commands/models.py` & `together-0.1.2/src/together/commands/models.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,14 +12,17 @@
     COMMAND_NAME = "models"
     parser = subparsers.add_parser(COMMAND_NAME)
 
     child_parsers = parser.add_subparsers(required=True)
 
     _add_list(child_parsers)
     _add_info(child_parsers)
+    _add_instances(child_parsers)
+    _add_start(child_parsers)
+    _add_stop(child_parsers)
 
 
 def _add_list(
     parser: argparse._SubParsersAction[argparse.ArgumentParser],
 ) -> None:
     subparser = parser.add_parser("list")
     subparser.add_argument(
@@ -46,14 +49,53 @@
         help="Raw details of all models",
         default=False,
         action="store_true",
     )
     subparser.set_defaults(func=_run_info)
 
 
+def _add_instances(
+    parser: argparse._SubParsersAction[argparse.ArgumentParser],
+) -> None:
+    subparser = parser.add_parser("instances")
+    subparser.add_argument(
+        "--raw",
+        help="Raw list of instances",
+        default=False,
+        action="store_true",
+    )
+    subparser.set_defaults(func=_run_instances)
+
+
+def _add_start(
+    parser: argparse._SubParsersAction[argparse.ArgumentParser],
+) -> None:
+    subparser = parser.add_parser("start")
+    subparser.add_argument(
+        "model",
+        metavar="MODEL",
+        help="Proper Model API string name",
+        type=str,
+    )
+    subparser.set_defaults(func=_run_start)
+
+
+def _add_stop(
+    parser: argparse._SubParsersAction[argparse.ArgumentParser],
+) -> None:
+    subparser = parser.add_parser("stop")
+    subparser.add_argument(
+        "model",
+        metavar="MODEL",
+        help="Proper Model API string name",
+        type=str,
+    )
+    subparser.set_defaults(func=_run_stop)
+
+
 def _run_list(args: argparse.Namespace) -> None:
     models = Models()
     response = models.list()
     if args.raw:
         print(json.dumps(response, indent=4))
     else:
         model_list = []
@@ -83,7 +125,29 @@
         if i["name"] == args.model:
             if args.raw:
                 print(json.dumps(i, indent=4))
             else:
                 model_info = {key: i[key] for key in visible_keys if key in i}
                 print(json.dumps(model_info, indent=4))
             break
+
+
+def _run_instances(args: argparse.Namespace) -> None:
+    models = Models()
+    response = models.instances()
+    if args.raw:
+        print(json.dumps(response, indent=4))
+    else:
+        started_instances = [key for key in response.keys() if response[key] is True]
+        print(json.dumps(started_instances, indent=4))
+
+
+def _run_start(args: argparse.Namespace) -> None:
+    models = Models()
+    response = models.start(args.model)
+    print(json.dumps(response, indent=4))
+
+
+def _run_stop(args: argparse.Namespace) -> None:
+    models = Models()
+    response = models.stop(args.model)
+    print(json.dumps(response, indent=4))
```

### Comparing `together-0.1.1/src/together/utils/conversation.py` & `together-0.1.2/src/together/utils/conversation.py`

 * *Files identical despite different names*

### Comparing `together-0.1.1/src/together/utils/utils.py` & `together-0.1.2/src/together/utils/utils.py`

 * *Files identical despite different names*

### Comparing `together-0.1.1/.gitignore` & `together-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `together-0.1.1/LICENSE` & `together-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `together-0.1.1/README.md` & `together-0.1.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 
 ```shell Shell
 pip install --upgrade together
 ```
 
 # Usage
 
+> 🚧 You will need to create a free account with [together.ai](https://api.together.xyz/) to obtain a Together API Key.
+
 The Python Library requires your Together API Key to be configured. This key can be found in your Account's settings on the Playground. Simply click on and navigate to Profile Button > Settings > API Keys.
 
 The API Key can be configured by either setting the `TOGETHER_API_KEY` environment variable, like this:
 
 ```shell
 export TOGETHER_API_KEY=xxxxx
 ```
@@ -21,15 +23,34 @@
 Or by setting `together.api_key`:
 
 ```python
 import together
 together.api_key = "xxxxx"
 ```
 
-> 🚧 You will need to start a model instance from the Playground before you can query it from the API
+Once you've provided your API key, you can browse our list of available models:
+
+```python
+import together
+
+# set your API key
+together.api_key = "xxxxx"
+
+# list available models and descriptons
+models = together.Models.list()
+
+# print the first model's name
+print(models[0]['name'])
+```
+
+Let's start an instance of one of the models in the list above. You can also start an instance by clicking play on any model in the [models playground](https://api.together.xyz/playground).
+
+```python
+together.Models.start("togethercomputer/RedPajama-INCITE-7B-Base")
+```
 
 Once you've started a model instance, you can start querying:
 
 ```python
 import together
 
 # set your API key
@@ -43,14 +64,26 @@
 
 output = together.Complete.create("Space robots", model="togethercomputer/RedPajama-INCITE-7B-Base")
 
 # print generated text
 print(output['output']['choices'][0]['text'])
 ```
 
+Check which models have been started or stopped:
+
+```python
+together.Models.instances()
+```
+
+To stop your model instance:
+
+```python
+together.Models.stop("togethercomputer/RedPajama-INCITE-7B-Base")
+```
+
 ## Chat
 
 The `chat` command is a CLI-based chat application that can be used for back-and-forth conversations with models in a pre-defined format.
 
 Refer to the [Chat docs](https://docs.together.ai/docs/python-chat) on how to chat with your favorite models.
 
 ## Complete
@@ -84,17 +117,27 @@
 ```shell
 # list commands
 together --help
 
 # list available models
 together models list
 
+# start a model
+together models start togethercomputer/RedPajama-INCITE-7B-Base
+
 # create completion
 together complete "Space robots" -m togethercomputer/RedPajama-INCITE-7B-Base
+
+# check which models are running
+together models instances
+
+# stop a model
+together models stop togethercomputer/RedPajama-INCITE-7B-Base
 ```
+
 ## Contributing
 1. Clone the repo and make your changes
 2. Run `pip install together['quality']`
 3. From the root of the repo, run
     - `black .`
     - `ruff .`
       - And if necessary, `ruff . --fix`
```

### Comparing `together-0.1.1/pyproject.toml` & `together-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "together"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Together Computer", email="community@together.xyz" },
 ]
 description = "Python client for Together's Cloud Platform!"
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.6"
```

### Comparing `together-0.1.1/PKG-INFO` & `together-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: together
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python client for Together's Cloud Platform!
 Project-URL: Homepage, https://github.com/togethercomputer/together
 Project-URL: Bug Tracker, https://github.com/togethercomputer/together/issues
 Author-email: Together Computer <community@together.xyz>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -231,14 +231,16 @@
 
 ```shell Shell
 pip install --upgrade together
 ```
 
 # Usage
 
+> 🚧 You will need to create a free account with [together.ai](https://api.together.xyz/) to obtain a Together API Key.
+
 The Python Library requires your Together API Key to be configured. This key can be found in your Account's settings on the Playground. Simply click on and navigate to Profile Button > Settings > API Keys.
 
 The API Key can be configured by either setting the `TOGETHER_API_KEY` environment variable, like this:
 
 ```shell
 export TOGETHER_API_KEY=xxxxx
 ```
@@ -246,15 +248,34 @@
 Or by setting `together.api_key`:
 
 ```python
 import together
 together.api_key = "xxxxx"
 ```
 
-> 🚧 You will need to start a model instance from the Playground before you can query it from the API
+Once you've provided your API key, you can browse our list of available models:
+
+```python
+import together
+
+# set your API key
+together.api_key = "xxxxx"
+
+# list available models and descriptons
+models = together.Models.list()
+
+# print the first model's name
+print(models[0]['name'])
+```
+
+Let's start an instance of one of the models in the list above. You can also start an instance by clicking play on any model in the [models playground](https://api.together.xyz/playground).
+
+```python
+together.Models.start("togethercomputer/RedPajama-INCITE-7B-Base")
+```
 
 Once you've started a model instance, you can start querying:
 
 ```python
 import together
 
 # set your API key
@@ -268,14 +289,26 @@
 
 output = together.Complete.create("Space robots", model="togethercomputer/RedPajama-INCITE-7B-Base")
 
 # print generated text
 print(output['output']['choices'][0]['text'])
 ```
 
+Check which models have been started or stopped:
+
+```python
+together.Models.instances()
+```
+
+To stop your model instance:
+
+```python
+together.Models.stop("togethercomputer/RedPajama-INCITE-7B-Base")
+```
+
 ## Chat
 
 The `chat` command is a CLI-based chat application that can be used for back-and-forth conversations with models in a pre-defined format.
 
 Refer to the [Chat docs](https://docs.together.ai/docs/python-chat) on how to chat with your favorite models.
 
 ## Complete
@@ -309,17 +342,27 @@
 ```shell
 # list commands
 together --help
 
 # list available models
 together models list
 
+# start a model
+together models start togethercomputer/RedPajama-INCITE-7B-Base
+
 # create completion
 together complete "Space robots" -m togethercomputer/RedPajama-INCITE-7B-Base
+
+# check which models are running
+together models instances
+
+# stop a model
+together models stop togethercomputer/RedPajama-INCITE-7B-Base
 ```
+
 ## Contributing
 1. Clone the repo and make your changes
 2. Run `pip install together['quality']`
 3. From the root of the repo, run
     - `black .`
     - `ruff .`
       - And if necessary, `ruff . --fix`
```

