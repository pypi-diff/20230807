# Comparing `tmp/cerebrium-1.3.2.tar.gz` & `tmp/cerebrium-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cerebrium-1.3.2.tar", max compression
+gzip compressed data, was "cerebrium-1.4.0.tar", max compression
```

## Comparing `cerebrium-1.3.2.tar` & `cerebrium-1.4.0.tar`

### file list

```diff
@@ -1,38 +1,39 @@
--rw-r--r--   0        0        0      372 2023-08-04 15:41:33.335070 cerebrium-1.3.2/EXTERNAL_README.md
--rw-r--r--   0        0        0    34594 2023-08-04 15:41:33.335070 cerebrium-1.3.2/LICENSE
--rw-r--r--   0        0        0      360 2023-08-04 15:44:41.015567 cerebrium-1.3.2/cerebrium/__init__.py
--rwxr-xr-x   0        0        0    36049 2023-08-04 15:41:33.335070 cerebrium-1.3.2/cerebrium/cli.py
--rw-r--r--   0        0        0    35162 2023-08-04 15:41:33.339070 cerebrium-1.3.2/cerebrium/conduit.py
--rw-r--r--   0        0        0     5048 2023-08-04 15:41:33.339070 cerebrium-1.3.2/cerebrium/core.py
--rw-r--r--   0        0        0     2488 2023-08-04 15:41:33.339070 cerebrium-1.3.2/cerebrium/errors.py
--rw-r--r--   0        0        0    10182 2023-08-04 15:41:33.339070 cerebrium-1.3.2/cerebrium/flow.py
--rw-r--r--   0        0        0     3070 2023-08-04 15:41:33.339070 cerebrium-1.3.2/cerebrium/logging/arize.py
--rw-r--r--   0        0        0      705 2023-08-04 15:41:33.339070 cerebrium-1.3.2/cerebrium/logging/base.py
--rw-r--r--   0        0        0     3990 2023-08-04 15:41:33.339070 cerebrium-1.3.2/cerebrium/logging/censius.py
--rw-r--r--   0        0        0      600 2023-08-04 15:41:33.339070 cerebrium-1.3.2/cerebrium/models/base.py
--rw-r--r--   0        0        0      550 2023-08-04 15:41:33.339070 cerebrium-1.3.2/cerebrium/models/hf_pipeline.py
--rw-r--r--   0        0        0      431 2023-08-04 15:41:33.339070 cerebrium-1.3.2/cerebrium/models/onnx.py
--rw-r--r--   0        0        0      793 2023-08-04 15:41:33.339070 cerebrium-1.3.2/cerebrium/models/sklearn.py
--rw-r--r--   0        0        0      270 2023-08-04 15:41:33.339070 cerebrium-1.3.2/cerebrium/models/spacy.py
--rw-r--r--   0        0        0      273 2023-08-04 15:41:33.339070 cerebrium-1.3.2/cerebrium/models/torch.py
--rw-r--r--   0        0        0     8545 2023-08-04 15:41:33.339070 cerebrium-1.3.2/cerebrium/requests.py
--rw-r--r--   0        0        0    10957 2023-08-04 15:41:33.339070 cerebrium-1.3.2/cerebrium/trainer/README_Diffusers.md
--rw-r--r--   0        0        0     5592 2023-08-04 15:41:33.339070 cerebrium-1.3.2/cerebrium/trainer/README_Transformers.md
--rw-r--r--   0        0        0      110 2023-08-04 15:41:33.339070 cerebrium-1.3.2/cerebrium/trainer/__init__.py
--rw-r--r--   0        0        0     2515 2023-08-04 15:41:33.339070 cerebrium-1.3.2/cerebrium/trainer/config/diffuser.yaml
--rw-r--r--   0        0        0     1940 2023-08-04 15:41:33.339070 cerebrium-1.3.2/cerebrium/trainer/config/falcon-40b.yaml
--rw-r--r--   0        0        0     1864 2023-08-04 15:41:33.339070 cerebrium-1.3.2/cerebrium/trainer/config/falcon-7b.yaml
--rw-r--r--   0        0        0     1916 2023-08-04 15:41:33.339070 cerebrium-1.3.2/cerebrium/trainer/config/llama-13b.yaml
--rw-r--r--   0        0        0     1692 2023-08-04 15:41:33.339070 cerebrium-1.3.2/cerebrium/trainer/config/llama-7b.yaml
--rw-r--r--   0        0        0     1991 2023-08-04 15:41:33.339070 cerebrium-1.3.2/cerebrium/trainer/config/llama2-13b.yaml
--rw-r--r--   0        0        0     1751 2023-08-04 15:41:33.339070 cerebrium-1.3.2/cerebrium/trainer/config/llama2-7b.yaml
--rw-r--r--   0        0        0     1747 2023-08-04 15:41:33.339070 cerebrium-1.3.2/cerebrium/trainer/config/transformer.yaml
--rw-r--r--   0        0        0    15030 2023-08-04 15:41:33.339070 cerebrium-1.3.2/cerebrium/trainer/diffuser_tuner.py
--rw-r--r--   0        0        0     8826 2023-08-04 15:41:33.339070 cerebrium-1.3.2/cerebrium/trainer/fine_tuner.py
--rw-r--r--   0        0        0     1716 2023-08-04 15:41:33.339070 cerebrium-1.3.2/cerebrium/trainer/finetune_LLM/finetuning_model.py
--rw-r--r--   0        0        0        0 2023-08-04 15:41:33.339070 cerebrium-1.3.2/cerebrium/trainer/finetune_LLM/userDataset/__init__.py
--rw-r--r--   0        0        0     2647 2023-08-04 15:41:33.339070 cerebrium-1.3.2/cerebrium/trainer/finetune_LLM/userDataset/base_dataset.py
--rw-r--r--   0        0        0     4115 2023-08-04 15:41:33.339070 cerebrium-1.3.2/cerebrium/trainer/finetune_LLM/userDataset/data_validator.py
--rw-r--r--   0        0        0     1048 2023-08-04 15:41:33.339070 cerebrium-1.3.2/cerebrium/utils.py
--rw-r--r--   0        0        0     2346 2023-08-04 15:44:41.011567 cerebrium-1.3.2/pyproject.toml
--rw-r--r--   0        0        0     1618 1970-01-01 00:00:00.000000 cerebrium-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0      372 2023-08-07 18:40:54.956560 cerebrium-1.4.0/EXTERNAL_README.md
+-rw-r--r--   0        0        0    34594 2023-08-07 18:40:54.956560 cerebrium-1.4.0/LICENSE
+-rw-r--r--   0        0        0      424 2023-08-07 18:43:25.439590 cerebrium-1.4.0/cerebrium/__init__.py
+-rwxr-xr-x   0        0        0    39067 2023-08-07 18:40:54.960560 cerebrium-1.4.0/cerebrium/cli.py
+-rw-r--r--   0        0        0    36663 2023-08-07 18:40:54.960560 cerebrium-1.4.0/cerebrium/conduit.py
+-rw-r--r--   0        0        0     5297 2023-08-07 18:40:54.960560 cerebrium-1.4.0/cerebrium/core.py
+-rw-r--r--   0        0        0      417 2023-08-07 18:40:54.960560 cerebrium-1.4.0/cerebrium/datatypes.py
+-rw-r--r--   0        0        0     2488 2023-08-07 18:40:54.960560 cerebrium-1.4.0/cerebrium/errors.py
+-rw-r--r--   0        0        0    10182 2023-08-07 18:40:54.960560 cerebrium-1.4.0/cerebrium/flow.py
+-rw-r--r--   0        0        0     3070 2023-08-07 18:40:54.960560 cerebrium-1.4.0/cerebrium/logging/arize.py
+-rw-r--r--   0        0        0      705 2023-08-07 18:40:54.960560 cerebrium-1.4.0/cerebrium/logging/base.py
+-rw-r--r--   0        0        0     3990 2023-08-07 18:40:54.960560 cerebrium-1.4.0/cerebrium/logging/censius.py
+-rw-r--r--   0        0        0      600 2023-08-07 18:40:54.960560 cerebrium-1.4.0/cerebrium/models/base.py
+-rw-r--r--   0        0        0      550 2023-08-07 18:40:54.960560 cerebrium-1.4.0/cerebrium/models/hf_pipeline.py
+-rw-r--r--   0        0        0      431 2023-08-07 18:40:54.960560 cerebrium-1.4.0/cerebrium/models/onnx.py
+-rw-r--r--   0        0        0      793 2023-08-07 18:40:54.960560 cerebrium-1.4.0/cerebrium/models/sklearn.py
+-rw-r--r--   0        0        0      270 2023-08-07 18:40:54.960560 cerebrium-1.4.0/cerebrium/models/spacy.py
+-rw-r--r--   0        0        0      273 2023-08-07 18:40:54.960560 cerebrium-1.4.0/cerebrium/models/torch.py
+-rw-r--r--   0        0        0     8545 2023-08-07 18:40:54.960560 cerebrium-1.4.0/cerebrium/requests.py
+-rw-r--r--   0        0        0    10957 2023-08-07 18:40:54.960560 cerebrium-1.4.0/cerebrium/trainer/README_Diffusers.md
+-rw-r--r--   0        0        0     5592 2023-08-07 18:40:54.960560 cerebrium-1.4.0/cerebrium/trainer/README_Transformers.md
+-rw-r--r--   0        0        0      110 2023-08-07 18:40:54.960560 cerebrium-1.4.0/cerebrium/trainer/__init__.py
+-rw-r--r--   0        0        0     2515 2023-08-07 18:40:54.960560 cerebrium-1.4.0/cerebrium/trainer/config/diffuser.yaml
+-rw-r--r--   0        0        0     1940 2023-08-07 18:40:54.960560 cerebrium-1.4.0/cerebrium/trainer/config/falcon-40b.yaml
+-rw-r--r--   0        0        0     1864 2023-08-07 18:40:54.960560 cerebrium-1.4.0/cerebrium/trainer/config/falcon-7b.yaml
+-rw-r--r--   0        0        0     1916 2023-08-07 18:40:54.960560 cerebrium-1.4.0/cerebrium/trainer/config/llama-13b.yaml
+-rw-r--r--   0        0        0     1692 2023-08-07 18:40:54.960560 cerebrium-1.4.0/cerebrium/trainer/config/llama-7b.yaml
+-rw-r--r--   0        0        0     1991 2023-08-07 18:40:54.960560 cerebrium-1.4.0/cerebrium/trainer/config/llama2-13b.yaml
+-rw-r--r--   0        0        0     1751 2023-08-07 18:40:54.960560 cerebrium-1.4.0/cerebrium/trainer/config/llama2-7b.yaml
+-rw-r--r--   0        0        0     1747 2023-08-07 18:40:54.960560 cerebrium-1.4.0/cerebrium/trainer/config/transformer.yaml
+-rw-r--r--   0        0        0    15099 2023-08-07 18:40:54.960560 cerebrium-1.4.0/cerebrium/trainer/diffuser_tuner.py
+-rw-r--r--   0        0        0     8895 2023-08-07 18:40:54.960560 cerebrium-1.4.0/cerebrium/trainer/fine_tuner.py
+-rw-r--r--   0        0        0     1716 2023-08-07 18:40:54.960560 cerebrium-1.4.0/cerebrium/trainer/finetune_LLM/finetuning_model.py
+-rw-r--r--   0        0        0        0 2023-08-07 18:40:54.960560 cerebrium-1.4.0/cerebrium/trainer/finetune_LLM/userDataset/__init__.py
+-rw-r--r--   0        0        0     2647 2023-08-07 18:40:54.960560 cerebrium-1.4.0/cerebrium/trainer/finetune_LLM/userDataset/base_dataset.py
+-rw-r--r--   0        0        0     4115 2023-08-07 18:40:54.960560 cerebrium-1.4.0/cerebrium/trainer/finetune_LLM/userDataset/data_validator.py
+-rw-r--r--   0        0        0     1048 2023-08-07 18:40:54.960560 cerebrium-1.4.0/cerebrium/utils.py
+-rw-r--r--   0        0        0     2391 2023-08-07 18:43:25.439590 cerebrium-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1618 1970-01-01 00:00:00.000000 cerebrium-1.4.0/PKG-INFO
```

### Comparing `cerebrium-1.3.2/LICENSE` & `cerebrium-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cerebrium-1.3.2/cerebrium/cli.py` & `cerebrium-1.4.0/cerebrium/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 import yaml
 import yaspin
 from termcolor import colored
 from tqdm import tqdm
 from tqdm.utils import CallbackIOWrapper
 
 from cerebrium import trainer
+from cerebrium.datatypes import PythonVersion, Hardware
 from cerebrium import __version__ as cerebrium_version
 
 app = typer.Typer()
 env = os.getenv("ENV", "prod")
 
 dashboard_url = (
     "https://dashboard.cerebrium.ai"
@@ -184,15 +185,15 @@
         "", help="Optional list of conda packages you would like to add."
     ),
     api_key: str = typer.Option(
         "", help="Private API key for the user. Not included in config by default."
     ),
     hardware: str = typer.Option(
         "GPU",
-        help="Hardware to use for the builder deployment. Can be one of 'CPU', 'GPU' or 'A10'.",
+        help="Hardware to use for the builder deployment. Defaults to 'GPU'. Can be one of 'CPU', 'GPU', 'A10', 'TURING_4000', 'TURING_5000', 'AMPERE_A4000', 'AMPERE_A5000', 'AMPERE_A6000', 'AMPERE_A100'",
     ),
     include: str = typer.Option(
         "[./*, main.py, requirements.txt, pkglist.txt, conda_pkglist.txt]",
         help="Comma delimited string list of relative paths to files/folder to include. Defaults to all visible files/folders in project root.",
     ),
     exclude: str = typer.Option(
         "[./.*, ./__*]",  # ignore .git etc. by default
@@ -206,14 +207,19 @@
         bool(os.getenv("CI", False)),
         help="Whether to use TQDM and yaspin animations.",
     ),
 ):
     """
     Initialize an empty Cerebrium Cortex project.
     """
+    # Check the hardware val is valid
+    if hardware:
+        vals = [v.value for v in Hardware]
+        assert hardware in vals, f"Hardware must be one of {vals}"
+        hardware = Hardware(hardware).value
 
     # check if init_dir exists, if not create it
     if not os.path.exists(init_dir):
         os.makedirs(init_dir)
     else:
         # check the init_dir is empty, if not throw error and exit
         if os.listdir(init_dir) and not overwrite:
@@ -285,15 +291,28 @@
 
 @app.command()
 def deploy(
     name: str = typer.Argument(..., help="Name of the builder deployment."),
     api_key: str = typer.Option("", help="Private API key for the user."),
     hardware: str = typer.Option(
         "",
-        help="Hardware to use for the builder deployment. Can be one of 'CPU', 'GPU' or 'A10'.",
+        help="Hardware to use for the builder deployment. Defaults to 'GPU'. Can be one of 'CPU', 'GPU', 'A10', 'TURING_4000', 'TURING_5000', 'AMPERE_A4000', 'AMPERE_A5000', 'AMPERE_A6000', 'AMPERE_A100'",
+    ),
+    min_replicas: Union[int, None] = typer.Option(
+        None,
+        help="Initial minimum number of replicas to create on deployment. Defaults to 1",
+    ),  # TODO finish message depending on if we charge per replica per day or something. Otherwise don't want users increasing this where they don't need to.
+    max_replicas: Union[int, None] = typer.Option(
+        None,
+        help="A hard limit on the maximum number of replicas allow. Defaults to 2 for free users, enterprise and standard users are set to maximum specified in their plan",
+    ),  # TODO finish message depending on if we charge per replica per day or something. Otherwise don't want users increasing this where they don't need to.
+    # TODO do we need a way for users to see the number or replicas they're running or something similar?
+    python_version: str = typer.Option(
+        "",
+        help="Python version to use. Currently, we support '3.8' to '3.11'. Defaults to '3.10'",
     ),
     include: str = typer.Option(
         "",
         help="Comma delimited string list of relative paths to files/folder to include. Defaults to all visible files/folders in project root.",
     ),
     exclude: str = typer.Option(
         "",
@@ -323,20 +342,23 @@
     """
     Deploy a builder deployment to Cerebrium
     """
 
     # Set default params
     params = {
         "hardware": "GPU",
+        "python_version": "3.10",
         "include": "[./*, ./main.py, ./requirements.txt, ./pkglist.txt, ./conda_pkglist.txt]",
         "exclude": "[./.*, ./__*]",  # ignore .git etc. by default
         "log_level": "INFO",
         "init_debug": False,
         "pre_init_debug": False,
         "disable_animation": bool(os.getenv("CI", False)),
+        "min_replicas": None,  # This is set on the backend.
+        "max_replicas": None,
     }
 
     # If a config file is provided, load it in.
     if config_file:
         if not os.path.exists(config_file):
             print(f"Config file {config_file} not found.")
             sys.exit(1)
@@ -352,14 +374,17 @@
         config = {}
 
     # Override the default params with the config file params
     params.update(config)
 
     # Override the default params and config with the command line params
     name = name if name else params.get("name", None)
+    python_version = (
+        python_version if python_version else params.get("python_version", None)
+    )
     api_key = api_key if api_key else params.get("api_key", None)
     hardware = hardware if hardware else params.get("hardware", None)
     include = include if include else params.get("include", None)
     exclude = exclude if exclude else params.get("exclude", None)
     log_level = log_level if log_level else params.get("log_level", None)
     init_debug = (
         init_debug if init_debug is not None else params.get("init_debug", None)
@@ -370,48 +395,64 @@
         else params.get("pre_init_debug", None)
     )
     disable_animation = (
         disable_animation
         if disable_animation is not None
         else params.get("disable_animation", None)
     )
-
-    # # check that the hardware is valid
-    # assert hardware in ["CPU", "GPU", "A10"], "Hardware must be one of 'CPU', 'GPU' or 'A10'."
+    min_replicas = (
+        min_replicas if min_replicas is not None else params.get("min_replicas", None)
+    )
+    max_replicas = (
+        max_replicas if max_replicas is not None else params.get("max_replicas", None)
+    )
 
     # assert name is provided
     if not name:
         print("Please provide a name for your deployment using the --name flag.")
         sys.exit(1)
 
     # set api_key if not provided
     if not api_key:
         print("No API key provided. Using your login API Key. 🗝️")
         api_key = get_api_key()
 
+    if python_version:
+        # Assert that the python version is valid
+        vals = [v.value for v in PythonVersion]
+        assert python_version in vals, f"Python version must be one of {vals}"
+
+    # Check that hardware is valid and assign to enum
+    if hardware:
+        vals = [v.value for v in Hardware]
+        assert hardware in vals, f"Hardware must be one of {vals}"
+        hardware = Hardware(hardware).value
+
     # Safety check to ensure no parameter is None
     if any(
         True
         for elem in [
             name,
             api_key,
+            python_version,
             hardware,
             include,
             exclude,
             log_level,
             init_debug,
             pre_init_debug,
             disable_animation,
         ]
         if elem is None
     ):
         f"All parameters must be provided. Please check your config file and command line arguments, found the following parameters to be None:"
         params = {
             "name": name,
             "api_key": api_key,
+            "python_version": python_version,
             "hardware": hardware,
             "include": include,
             "exclude": exclude,
             "log_level": log_level,
             "init_debug": init_debug,
             "pre_init_debug": pre_init_debug,
             "disable_animation": disable_animation,
@@ -453,21 +494,24 @@
 
     # Hit the deploy endpoint to get the upload URL
     upload_url_response = requests.post(
         f"{api_url}/deploy",
         headers={"Authorization": api_key},
         json={
             "name": name,
+            "python_version": python_version,
             "hardware": hardware.upper(),
             "init_debug": init_debug,
             "pre_init_debug": pre_init_debug,
             "log_level": log_level.upper(),
             "cerebrium_version": cerebrium_version,
             "requirements_hash": requirements_hash,
             "pkglist_hash": pkglist_hash,
+            "min_replicas": min_replicas,
+            "max_replicas": max_replicas,
         },
     )
 
     if upload_url_response.status_code != 200 or (
         upload_url_response.json().get("uploadUrl", None) is None
     ):
         print("API request failed with status code:", upload_url_response.status_code)
@@ -713,16 +757,16 @@
 
     interval = 1  # seconds between polling.
     max_polling_duration = min(max_polling_duration, 60 * 60)
 
     # Poll the trainingLogs and make the output pretty
     seen_index = 0
     t_start = time.time()
-    with yaspin.yaspin(text="CHECKING...", color="green") as spinner:
-        train_status = "CHECKING..."
+    with yaspin.yaspin(text="Fetching...", color="green") as spinner:
+        train_status = "Fetching..."
         while train_status != "succeeded":
             train_status_response = requests.post(
                 f"{api_url}/job-logs",
                 headers={"Authorization": api_key},
                 json={"jobId": job_id},
             )
 
@@ -860,14 +904,17 @@
     ),
     name: str = typer.Option(
         None, help="Name for your training instance. Overrides config file."
     ),
     api_key: Union[str, None] = typer.Option(
         None, help="Private API key for the user. Overrides the config file"
     ),
+    hardware: Union[str, None] = typer.Option(
+        None, help="Hardware to use for training. Defaults to AMPERE_A6000."
+    ),
     config_string: str = typer.Option(
         None,
         help="Config JSON string to use for training. Overrides the config file if the file is provided.",
     ),
     init_debug: bool = typer.Option(
         False,
         help="Stops the container after initialization.",
@@ -909,41 +956,54 @@
     # overwrite with command line args if present
     name = name or config["name"]
     if not api_key:
         api_key = config.get(
             "api_key"
         )  # default to config from either the file or the string
 
+    # Validate hardware
+    hardware = hardware if hardware else config.get("hardware", None)
+    if hardware:
+        vals = [v.value for v in Hardware]
+        assert hardware in vals, f"Hardware must be one of {vals}"
+        hardware = Hardware(hardware).value
+    else:
+        hardware = Hardware.AMPERE_A6000.value
+
     # If api key is not provided in any parameter or config, check if it is in the login config file
     if not api_key:
         api_key = get_api_key()
 
     # get log level
     log_level = log_level or config.get("log_level", "INFO")
 
+    print(f"🌍 Deploying training job {name} with {hardware} hardware to Cerebrium...")
+
     # check which training
     if training_type == "diffuser":
         diffuser_tuning = trainer.DiffuserTuner(
             name=name, config=config, log_level=log_level
         )
         # upload
         diffuser_tuning._upload(
             api_key=api_key,
+            hardware=hardware,
             init_debug=init_debug,
             pre_init_debug=pre_init_debug,
             log_level=log_level,
         )
     elif training_type == "transformer":
         finetuning = trainer.FineTuner(
             name=name,
             config=config,
             log_level=log_level,
         )
         finetuning._upload(
             api_key=api_key,
+            hardware=hardware,
             init_debug=init_debug,
             pre_init_debug=pre_init_debug,
             log_level=log_level,
         )
 
 
 @app.command()
```

### Comparing `cerebrium-1.3.2/cerebrium/conduit.py` & `cerebrium-1.4.0/cerebrium/conduit.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,49 +16,54 @@
 
 from cerebrium import __version__
 from cerebrium.flow import CerebriumFlow, _check_flow_type, _flow_string
 from cerebrium.logging.base import LoggingPlatform
 from cerebrium.models.base import ModelType
 from cerebrium.requests import _cerebrium_request, _poll_deployment_status
 
+from cerebrium.datatypes import PythonVersion, Hardware
+
 REGEX_NAME_PATTERN = "^[a-z0-9-]*$"
 API_KEY = None
 
 
 def _set_api_key(api_key):
     global API_KEY
     API_KEY = api_key
 
 
-class Hardware(enum.Enum):
-    CPU = "cpu"
-    GPU = "gpu"
-    A10 = "a10"
-
-
 class Conduit:
     """
     The Conduit class encompasses the logic required to create a computational graph from a given model flow, as well as the logic required to run the graph on a given input.
 
     Args:
         name (str): The name to deploy the flow under.
         api_key (str): The API key for the Cerebrium account. If not provided, the API key will be read from the CEREBRIUM_API_KEY environment variable.
         flow (CerebriumFlow): The flow to deploy. This is a list of ModelType, model path and postprocessor tuples, as such:
             [(model_type.TORCH, "model.pt", postprocess_f)]
         hardware (Hardware): The hardware to deploy the model on.
+        from_json (str): The path to a JSON file containing the Conduit configuration.
+        requirements_file (str): The path to a requirements.txt file containing the dependencies for the Conduit.
+        min_replicas (int): The minimum number of replicas to deploy. Defaults to 1.
+        max_replicas (int): The maximum number of replicas to deploy. Defaults to 2. This is plan dependent. Please contact Cerebrium for more information.
     """
 
+    # TODO: refine min_replicas description
+
     def __init__(
         self,
         name: str = "",
         api_key: str = "",
         flow: CerebriumFlow = [],
         hardware: Union[Hardware, None] = None,
+        python_version: Union[PythonVersion, None] = None,
         from_json: str = "",
         requirements_file: str = "",
+        min_replicas: Union[int, None] = None,
+        max_replicas: Union[int, None] = None,
     ):
         if not from_json:
             self.api_key = api_key or os.environ.get("CEREBRIUM_API_KEY", "")
             assert name != "" and self.api_key != ""
             # Check that the flow name is valid
             if len(name) > 20:
                 raise ValueError("Conduit name must be less than 20 characters")
@@ -67,39 +72,52 @@
                     "Conduit name can only contain lowercase alphanumeric characters and hyphens"
                 )
             self.name = name
             if flow is not None:
                 self.flow: CerebriumFlow = _check_flow_type(flow)
             self.logger_configs = {}
             self._processors = None
+            self.min_replicas = min_replicas
+            self.max_replicas = max_replicas
+            self.requirements_file = requirements_file
         else:
             with open(from_json, "r") as f:
                 config = json.load(f)
                 self.name = config["name"]
                 self.api_key = config["api_key"]
                 self.flow: CerebriumFlow = config["flow"]
                 self.logger_configs = config["logger_configs"]
                 self._processors = config["processors"]
+                self.requirements_file = config.get("requirements_file")
+                self.min_replicas = config.get("min_replicas")
+                self.max_replicas = config.get("max_replicas")
+                self.hardware = (
+                    Hardware(config["hardware"]) if config.get("hardware") else None
+                )
+                self.python_version = (
+                    PythonVersion(config["python_version"])
+                    if config.get("python_version")
+                    else None
+                )
                 # Set correct ModelTypes in flow
                 for i, (model_type, model_initialization, processors) in enumerate(  # type: ignore
                     self.flow
                 ):
                     self.flow[i] = (
                         ModelType(model_type),
                         model_initialization,
                         processors,
                     )
-                hardware = Hardware(config["hardware"])
         _set_api_key(self.api_key)
         self.graph = []
         self.ready = False
         self.loggers = {}
         self.hardware = hardware or self._determine_hardware()
+        self.python_version = python_version or PythonVersion.PYTHON_3_10
 
-        self.requirements_file = requirements_file
         if self.requirements_file:
             assert os.path.exists(
                 self.requirements_file
             ), f"Requirements file {self.requirements_file} does not exist"
             assert os.path.isfile(
                 self.requirements_file
             ), f"Requirements file {self.requirements_file} is not a file"
@@ -111,28 +129,28 @@
             #     with open("./requirements.txt", "rb") as f:
             #         self.requirements_hash = hashlib.md5(f.read()).hexdigest()
 
         try:
             from torch.cuda import is_available
 
             self.device = (
-                "cuda" if self.hardware == Hardware.GPU and is_available() else "cpu"
+                "cuda" if self.hardware != Hardware.CPU and is_available() else "cpu"
             )
         except ImportError:
             self.device = "cpu"
         self.contains_torch_model = False
 
     def _determine_hardware(self):
         # Set the default hardware to GPU if the flow contains a Torch, ONNX or HuggingFace model
         if any(
             model_type
             in [ModelType.TORCH, ModelType.ONNX, ModelType.HUGGINGFACE_PIPELINE]
             for model_type, _, _ in self.flow
         ):
-            return Hardware.GPU
+            return Hardware.TURING_4000
         else:
             return Hardware.CPU
 
     def load(self, directory: str = "/cache/", direct_from_flow: bool = False):
         """
         Load the Conduit components from the stored Model Flow into the computation graph.
 
@@ -315,15 +333,18 @@
 
     def write_processors(self):
         if not self._processors:
             return
         app_name = os.getenv("APP_NAME", "")
         assert app_name != "", "APP_NAME environment variable not set"
         # get python version from the runtime
-        processor_path = f"/miniconda/envs/{app_name}/lib/python3.10/conduit_processors"
+        python_version = os.getenv("PYTHON_VERSION", "3.10")
+        processor_path = (
+            f"/miniconda/envs/{app_name}/lib/python{python_version}/conduit_processors"
+        )
         os.makedirs(processor_path, exist_ok=True)
         # Create the processors.py file
         with open(
             f"{processor_path}/processors.py",
             "w",
         ) as f:
             f.write(
@@ -654,15 +675,15 @@
                             "post": None
                             if p[2].get("post", None) is None
                             else getsource(p[2]["post"]),  # type: ignore
                         }
                         for p in self.flow
                     ],
                     "hardware": self.hardware.value,
-                    # "requirements_hash": self.requirements_hash if self.requirements_file else ""
+                    "python_version": self.python_version.value,
                 },
                 f,
                 indent=2,
             )
 
     def _upload(self, url):
         """
@@ -768,14 +789,17 @@
             "POST",
             self.api_key,
             payload={
                 "name": self.name,
                 "cerebrium_version": __version__ if env == "prod" else "0.1.1_dev",
                 "hardware": self.hardware.value.upper(),
                 "source": "conduit",
+                "min_replicas": self.min_replicas,
+                "max_replicas": self.max_replicas,
+                "python_version": self.python_version.value,
             },
             enable_spinner=(
                 True,
                 ("Authenticating...", "Authenticated with Cerebrium!"),
             ),
         )
         upload_url = upload_url_response["data"]["uploadUrl"]
```

### Comparing `cerebrium-1.3.2/cerebrium/core.py` & `cerebrium-1.4.0/cerebrium/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 from cerebrium.conduit import Conduit
 from cerebrium.flow import CerebriumFlow
 from cerebrium.requests import _cerebrium_request, ENV
 from cerebrium.utils import _convert_input_data
 from cerebrium.errors import CerebriumError
 
+
 IS_SERVER = os.getenv("IS_SERVER", "false")
 _objects = {}
 if os.path.exists("secrets.json"):
     with open("secrets.json") as f:
         SECRETS = json.load(f)
 elif os.path.exists("secrets.yaml"):
     with open("secrets.yaml") as f:
@@ -35,14 +36,18 @@
 
 def upload(file_name):
     # Upload a file to Cerebrium S3 and return a URL to the file
     from cerebrium.conduit import API_KEY
     from boto3 import client
 
     if API_KEY and IS_SERVER == "true":
+        if not os.environ.get("HARDWARE") in ("GPU", "A10"):
+            raise CerebriumError(
+                "File storage is only available on GPU and A10 hardware at this time. We are working on expanding this to other hardware."
+            )
         s3_client = client("s3")
         file_id = str(uuid4())
         s3_client.upload_file(file_name, f"cerebrium-file-storage-{ENV}", id)
         return _cerebrium_request(
             method="getFileUrl",
             http_method="POST",
             api_key=API_KEY,
```

### Comparing `cerebrium-1.3.2/cerebrium/errors.py` & `cerebrium-1.4.0/cerebrium/errors.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.3.2/cerebrium/flow.py` & `cerebrium-1.4.0/cerebrium/flow.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.3.2/cerebrium/logging/arize.py` & `cerebrium-1.4.0/cerebrium/logging/arize.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.3.2/cerebrium/logging/base.py` & `cerebrium-1.4.0/cerebrium/logging/base.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.3.2/cerebrium/logging/censius.py` & `cerebrium-1.4.0/cerebrium/logging/censius.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.3.2/cerebrium/models/base.py` & `cerebrium-1.4.0/cerebrium/models/base.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.3.2/cerebrium/models/hf_pipeline.py` & `cerebrium-1.4.0/cerebrium/models/hf_pipeline.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.3.2/cerebrium/models/sklearn.py` & `cerebrium-1.4.0/cerebrium/models/sklearn.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.3.2/cerebrium/requests.py` & `cerebrium-1.4.0/cerebrium/requests.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.3.2/cerebrium/trainer/README_Diffusers.md` & `cerebrium-1.4.0/cerebrium/trainer/README_Diffusers.md`

 * *Files identical despite different names*

### Comparing `cerebrium-1.3.2/cerebrium/trainer/README_Transformers.md` & `cerebrium-1.4.0/cerebrium/trainer/README_Transformers.md`

 * *Files identical despite different names*

### Comparing `cerebrium-1.3.2/cerebrium/trainer/config/diffuser.yaml` & `cerebrium-1.4.0/cerebrium/trainer/config/diffuser.yaml`

 * *Files identical despite different names*

### Comparing `cerebrium-1.3.2/cerebrium/trainer/config/falcon-40b.yaml` & `cerebrium-1.4.0/cerebrium/trainer/config/falcon-40b.yaml`

 * *Files identical despite different names*

### Comparing `cerebrium-1.3.2/cerebrium/trainer/config/falcon-7b.yaml` & `cerebrium-1.4.0/cerebrium/trainer/config/falcon-7b.yaml`

 * *Files identical despite different names*

### Comparing `cerebrium-1.3.2/cerebrium/trainer/config/llama-13b.yaml` & `cerebrium-1.4.0/cerebrium/trainer/config/llama-13b.yaml`

 * *Files identical despite different names*

### Comparing `cerebrium-1.3.2/cerebrium/trainer/config/llama-7b.yaml` & `cerebrium-1.4.0/cerebrium/trainer/config/llama-7b.yaml`

 * *Files identical despite different names*

### Comparing `cerebrium-1.3.2/cerebrium/trainer/config/llama2-13b.yaml` & `cerebrium-1.4.0/cerebrium/trainer/config/llama2-13b.yaml`

 * *Files identical despite different names*

### Comparing `cerebrium-1.3.2/cerebrium/trainer/config/llama2-7b.yaml` & `cerebrium-1.4.0/cerebrium/trainer/config/llama2-7b.yaml`

 * *Files identical despite different names*

### Comparing `cerebrium-1.3.2/cerebrium/trainer/config/transformer.yaml` & `cerebrium-1.4.0/cerebrium/trainer/config/transformer.yaml`

 * *Files identical despite different names*

### Comparing `cerebrium-1.3.2/cerebrium/trainer/diffuser_tuner.py` & `cerebrium-1.4.0/cerebrium/trainer/diffuser_tuner.py`

 * *Files 2% similar despite different names*

```diff
@@ -261,15 +261,20 @@
             zip.write(config_path, arcname="finetune_config.yaml")
             self.create_local_dataset(zip)
 
         if self.log_level.upper() == "DEBUG":
             print(f"Created zip file at {zip_path} and ready for upload!")
 
     def _upload(
-        self, api_key, init_debug=False, pre_init_debug=False, log_level="INFO"
+        self,
+        api_key,
+        init_debug=False,
+        pre_init_debug=False,
+        log_level="INFO",
+        hardware="AMPERE_A6000",
     ):
         """Upload the config files to cerebrium for training."""
         dataset_hash = "DATASET_FILE_DOESNT_EXIST"
         # Calc MD5 hash of user's dataset
         assert os.path.exists(
             self.config.train_image_dir
         ), "Dataset file cannot be found. Please check the path you have entered!"
@@ -282,15 +287,15 @@
         upload_url_response = _cerebrium_request(
             method="train",
             http_method="POST",
             api_key=api_key,
             payload={
                 "name": self.name,
                 "hf_model_path": self.config.hf_model_path,
-                "hardware": "A10",
+                "hardware": hardware,
                 "init_debug": init_debug,
                 "pre_init_debug": pre_init_debug,
                 "log_level": log_level,
                 "cerebrium_version": __version__,
                 # "dataset_hash": dataset_hash,
             },
         )
```

### Comparing `cerebrium-1.3.2/cerebrium/trainer/fine_tuner.py` & `cerebrium-1.4.0/cerebrium/trainer/fine_tuner.py`

 * *Files 3% similar despite different names*

```diff
@@ -119,15 +119,20 @@
         config_dict["dataset"] = config_dict["dataset"].to_dict()
 
         with open(filename, "w") as f:
             # json.dump(config_dict, fp=f, indent=2, sort_keys=True)
             yaml.dump(config_dict, f, sort_keys=False, version=(1, 2))
 
     def _upload(
-        self, api_key, init_debug=False, pre_init_debug=False, log_level="INFO"
+        self,
+        api_key,
+        init_debug=False,
+        pre_init_debug=False,
+        log_level="INFO",
+        hardware="AMPERE_A6000",
     ):  # sourcery skip: extract-method
         dataset_hash = "DATASET_FILE_DOESNT_EXIST"
 
         # Calc MD5 hash of user's dataset
         assert os.path.exists(
             self.config["dataset_path"]
         ), "Dataset file cannot be found. Please check the path you have entered!"
@@ -137,15 +142,15 @@
         upload_url_response = _cerebrium_request(
             method="train",
             http_method="POST",
             api_key=api_key,
             payload={
                 "name": self.config["name"],
                 "hf_model_path": self.config["hf_model_path"],
-                "hardware": "A10",
+                "hardware": hardware,
                 "init_debug": init_debug,
                 "pre_init_debug": pre_init_debug,
                 "log_level": log_level,
                 "cerebrium_version": __version__,
                 "dataset_hash": dataset_hash,
             },
         )
```

### Comparing `cerebrium-1.3.2/cerebrium/trainer/finetune_LLM/finetuning_model.py` & `cerebrium-1.4.0/cerebrium/trainer/finetune_LLM/finetuning_model.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.3.2/cerebrium/trainer/finetune_LLM/userDataset/base_dataset.py` & `cerebrium-1.4.0/cerebrium/trainer/finetune_LLM/userDataset/base_dataset.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.3.2/cerebrium/trainer/finetune_LLM/userDataset/data_validator.py` & `cerebrium-1.4.0/cerebrium/trainer/finetune_LLM/userDataset/data_validator.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.3.2/cerebrium/utils.py` & `cerebrium-1.4.0/cerebrium/utils.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.3.2/pyproject.toml` & `cerebrium-1.4.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cerebrium"
-version = "1.3.2"
+version = "1.4.0"
 description = ""
 authors = ["Elijah Roussos <elijah@cerebrium.ai>"]
 license = "AGPL-3.0-only"
 readme = "EXTERNAL_README.md"
 exclude = ["tests/*", "dist/*", "webhook/*", "builder/*", "prebuilt/*", "common/*", "examples/*", "trainer/*", "README.md"]
 
 [tool.poetry.urls]
@@ -55,14 +55,16 @@
 [tool.poetry.group.server.dependencies]
 ddtrace = ">=1.15,<1.20.0"
 datadog = ">=0.45,<0.51.0"
 celery = {extras = ["s3", "sqs"], version = "5.3.1"}
 boto3 = "1.28.8"
 fastapi = "0.88.0"
 uvicorn = "0.23.1"
+mangum = "0.17.0"
+python-multipart = "0.0.6"
 
 
 [tool.poetry.group.ml]
 optional = true
 
 [tool.poetry.group.ml.dependencies]
 xgboost = "1.7.6"
```

### Comparing `cerebrium-1.3.2/PKG-INFO` & `cerebrium-1.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerebrium
-Version: 1.3.2
+Version: 1.4.0
 Summary: 
 License: AGPL-3.0-only
 Author: Elijah Roussos
 Author-email: elijah@cerebrium.ai
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
```

