# Comparing `tmp/censius-1.7.5.tar.gz` & `tmp/censius-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "censius-1.7.5.tar", last modified: Wed Jul  5 08:16:18 2023, max compression
+gzip compressed data, was "censius-1.8.1.tar", last modified: Mon Aug  7 11:48:12 2023, max compression
```

## Comparing `censius-1.7.5.tar` & `censius-1.8.1.tar`

### file list

```diff
@@ -1,38 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:16:18.746959 censius-1.7.5/
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-05 08:16:18.746959 censius-1.7.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-05 08:16:15.000000 censius-1.7.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-05 08:16:15.000000 censius-1.7.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 08:16:18.746959 censius-1.7.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-05 08:16:15.000000 censius-1.7.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:16:18.734959 censius-1.7.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:16:18.738959 censius-1.7.5/src/censius/
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-05 08:16:15.000000 censius-1.7.5/src/censius/CensiusParent.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-05 08:16:15.000000 censius-1.7.5/src/censius/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-05 08:16:16.000000 censius-1.7.5/src/censius/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-05 08:16:15.000000 censius-1.7.5/src/censius/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:16:18.746959 censius-1.7.5/src/censius/ml/
--rw-r--r--   0 runner    (1001) docker     (123)    33608 2023-07-05 08:16:15.000000 censius-1.7.5/src/censius/ml/CensiusClient.py
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-05 08:16:15.000000 censius-1.7.5/src/censius/ml/Dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-05 08:16:15.000000 censius-1.7.5/src/censius/ml/DatasetType.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-05 08:16:15.000000 censius-1.7.5/src/censius/ml/Explanation.py
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-05 08:16:15.000000 censius-1.7.5/src/censius/ml/ExplanationType.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-05 08:16:15.000000 censius-1.7.5/src/censius/ml/ModelType.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-05 08:16:15.000000 censius-1.7.5/src/censius/ml/Prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-05 08:16:15.000000 censius-1.7.5/src/censius/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-07-05 08:16:15.000000 censius-1.7.5/src/censius/ml/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    14033 2023-07-05 08:16:15.000000 censius-1.7.5/src/censius/ml/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)    21301 2023-07-05 08:16:15.000000 censius-1.7.5/src/censius/ml/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:16:18.746959 censius-1.7.5/src/censius/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)     5162 2023-07-05 08:16:15.000000 censius-1.7.5/src/censius/nlp/CensiusClient.py
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-05 08:16:15.000000 censius-1.7.5/src/censius/nlp/DatasetType.py
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-05 08:16:15.000000 censius-1.7.5/src/censius/nlp/ModelType.py
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-05 08:16:15.000000 censius-1.7.5/src/censius/nlp/UseCase.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-05 08:16:15.000000 censius-1.7.5/src/censius/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-05 08:16:15.000000 censius-1.7.5/src/censius/nlp/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-07-05 08:16:15.000000 censius-1.7.5/src/censius/nlp/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:16:18.742959 censius-1.7.5/src/censius.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-05 08:16:18.000000 censius-1.7.5/src/censius.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-05 08:16:18.000000 censius-1.7.5/src/censius.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 08:16:18.000000 censius-1.7.5/src/censius.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-05 08:16:18.000000 censius-1.7.5/src/censius.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-05 08:16:18.000000 censius-1.7.5/src/censius.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:48:12.215489 censius-1.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-08-07 11:48:12.215489 censius-1.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-08-07 11:48:10.000000 censius-1.8.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-07 11:48:10.000000 censius-1.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 11:48:12.215489 censius-1.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-08-07 11:48:10.000000 censius-1.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:48:12.211489 censius-1.8.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:48:12.215489 censius-1.8.1/src/censius/
+-rw-r--r--   0 runner    (1001) docker     (123)    35723 2023-08-07 11:48:10.000000 censius-1.8.1/src/censius/CensiusClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-08-07 11:48:10.000000 censius-1.8.1/src/censius/CensiusParent.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-07 11:48:10.000000 censius-1.8.1/src/censius/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-08-07 11:48:10.000000 censius-1.8.1/src/censius/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-08-07 11:48:10.000000 censius-1.8.1/src/censius/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:48:12.215489 censius-1.8.1/src/censius/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)    33608 2023-08-07 11:48:10.000000 censius-1.8.1/src/censius/ml/CensiusClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-07 11:48:10.000000 censius-1.8.1/src/censius/ml/Dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-08-07 11:48:10.000000 censius-1.8.1/src/censius/ml/DatasetType.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-07 11:48:10.000000 censius-1.8.1/src/censius/ml/Explanation.py
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-07 11:48:10.000000 censius-1.8.1/src/censius/ml/ExplanationType.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-07 11:48:10.000000 censius-1.8.1/src/censius/ml/ModelType.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-07 11:48:10.000000 censius-1.8.1/src/censius/ml/Prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-08-07 11:48:10.000000 censius-1.8.1/src/censius/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-08-07 11:48:10.000000 censius-1.8.1/src/censius/ml/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14033 2023-08-07 11:48:10.000000 censius-1.8.1/src/censius/ml/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21301 2023-08-07 11:48:10.000000 censius-1.8.1/src/censius/ml/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:48:12.215489 censius-1.8.1/src/censius/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-08-07 11:48:10.000000 censius-1.8.1/src/censius/nlp/CensiusClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-07 11:48:10.000000 censius-1.8.1/src/censius/nlp/DatasetType.py
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-07 11:48:10.000000 censius-1.8.1/src/censius/nlp/ModelType.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-07 11:48:10.000000 censius-1.8.1/src/censius/nlp/UseCase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-08-07 11:48:10.000000 censius-1.8.1/src/censius/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-08-07 11:48:10.000000 censius-1.8.1/src/censius/nlp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-08-07 11:48:10.000000 censius-1.8.1/src/censius/nlp/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:48:12.215489 censius-1.8.1/src/censius/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-08-07 11:48:10.000000 censius-1.8.1/src/censius/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-08-07 11:48:10.000000 censius-1.8.1/src/censius/validation/base_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-08-07 11:48:10.000000 censius-1.8.1/src/censius/validation/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-08-07 11:48:10.000000 censius-1.8.1/src/censius/validation/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-08-07 11:48:10.000000 censius-1.8.1/src/censius/validation/rules_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 11:48:10.000000 censius-1.8.1/src/censius/validation/training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-08-07 11:48:10.000000 censius-1.8.1/src/censius/validation/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-08-07 11:48:10.000000 censius-1.8.1/src/censius/validation/yaml_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:48:12.215489 censius-1.8.1/src/censius.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-08-07 11:48:12.000000 censius-1.8.1/src/censius.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-08-07 11:48:12.000000 censius-1.8.1/src/censius.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 11:48:12.000000 censius-1.8.1/src/censius.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-08-07 11:48:12.000000 censius-1.8.1/src/censius.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-07 11:48:12.000000 censius-1.8.1/src/censius.egg-info/top_level.txt
```

### Comparing `censius-1.7.5/setup.py` & `censius-1.8.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="censius",
-    version="1.7.5",
+    version="1.8.1",
     description="API for Censius",
     long_description=long_description,
     long_description_content_type="text/markdown",
     py_modules=["censius/client"],
     package_dir={"": "src"},
-    packages=["censius", "censius.nlp", "censius.ml"],
-    install_requires=["requests", "jsonschema", "pandas", "numpy"],
+    packages=["censius", "censius.nlp", "censius.ml", "censius.validation"],
+    install_requires=[
+        "requests>=2.25",
+        "jsonschema==3.2",
+        "pandas>=1.3,<2.0",
+        "numpy>=1.21",
+        "elemeta==1.0.6",
+        "pyyaml>=5.4",
+        "pydantic>=1.8,<2.0",
+    ],
     extras_require={"dev": ["pytest>=3.7", "pdoc3==0.9.2"]},
     url="https://github.com/Censius/censius-logs-python-sdk",
     author="Censius",
     author_email="dev@censius.ai",
     keywords=[],
 )
```

### Comparing `censius-1.7.5/src/censius/CensiusParent.py` & `censius-1.8.1/src/censius/CensiusParent.py`

 * *Files identical despite different names*

### Comparing `censius-1.7.5/src/censius/ml/CensiusClient.py` & `censius-1.8.1/src/censius/ml/CensiusClient.py`

 * *Files identical despite different names*

### Comparing `censius-1.7.5/src/censius/ml/constants.py` & `censius-1.8.1/src/censius/ml/constants.py`

 * *Files identical despite different names*

### Comparing `censius-1.7.5/src/censius/ml/schemas.py` & `censius-1.8.1/src/censius/ml/schemas.py`

 * *Files identical despite different names*

### Comparing `censius-1.7.5/src/censius/ml/utils.py` & `censius-1.8.1/src/censius/ml/utils.py`

 * *Files identical despite different names*

### Comparing `censius-1.7.5/src/censius/nlp/CensiusClient.py` & `censius-1.8.1/src/censius/nlp/CensiusClient.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,16 +17,16 @@
         error_flag, msg = validate_input(kwargs, register_training_valid)
         if error_flag:
             return msg
 
         file_path = kwargs["file"]
         dataset_type = kwargs["dataset_type"]
         dataset_name = kwargs["name"]
+        usecase = kwargs["use_case"]
         project_id = self.project_id
-        usecase = "llm"
         dataset_version = 1
         modality = "tabular"
 
         reader_for_total_chunk = pd.read_csv(file_path, chunksize=BULK_CHUNK_SIZE)
         num_chunks = sum(1 for _ in reader_for_total_chunk)
         reader_for_size = pd.read_csv(file_path, chunksize=BULK_CHUNK_SIZE)
         size = sum(len(chunk) for chunk in reader_for_size)
@@ -97,29 +97,32 @@
         return response.json()
 
     def log(self, *args, **kwargs):
         error_flag, msg = validate_input(kwargs, log_valid)
         if error_flag:
             return msg
 
-        input_data = "random string"
+        input_data = kwargs["input"]
         log_id = kwargs["log_id"]
         model_id = kwargs["model_id"]
         prediction = kwargs["prediction"]
         referenced_output = kwargs["referenced_output"]
         timestamp = kwargs["timestamp"]
 
         payload = {
             "prediction": prediction,
             "referenced_output": referenced_output,
             "input": input_data,
             "timestamp": timestamp,
             "log_id": log_id,
             "model_id": model_id,
         }
+        if "confidence_score" in kwargs:
+            payload["confidence_score"] = kwargs["confidence_score"]
+
         url = LLM_REGISTER_LOGS(self.project_id)
         headers = self.get_headers()
         payload = json.dumps(payload)
         response = requests.request("POST", url, headers=headers, data=payload)
         if response.status_code != 200:
             print("Failed to add logs", response.text)
             return
```

### Comparing `censius-1.7.5/src/censius/nlp/constants.py` & `censius-1.8.1/src/censius/nlp/constants.py`

 * *Files identical despite different names*

### Comparing `censius-1.7.5/src/censius/nlp/schema.py` & `censius-1.8.1/src/censius/nlp/schema.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,16 +12,21 @@
             "errorMessage": "Filename `file` is required and must be a string",
         },
         "dataset_type": {
             "type": "string",
             "enum": [DatasetType.TEXT],
             "errorMessage": "Dataset `dataset_type` is required and must be from the list of supported dataset types",
         },
+        "use_case": {
+            "type": "string",
+            "enum": [UseCase.SUMMARIZATION, UseCase.SENTIMENT_CLASSIFICATION],
+            "errorMessage": "UseCase `use_case` is required and must be from the list of supported use cases",
+        },
     },
-    "required": ["name", "file", "dataset_type"],
+    "required": ["name", "file", "dataset_type", "use_case"],
 }
 
 
 register_model_valid = {
     "type": "object",
     "properties": {
         "model_name": {
@@ -31,15 +36,15 @@
         "model_type": {
             "type": "string",
             "enum": [ModelType.LLM],
             "errorMessage": "ModelType `model_type` is required and must be from the list of supported types",
         },
         "use_case": {
             "type": "string",
-            "enum": [UseCase.SUMMARIZATION],
+            "enum": [UseCase.SUMMARIZATION, UseCase.SENTIMENT_CLASSIFICATION],
             "errorMessage": "UseCase `use_case` is required and must be from the list of supported use cases",
         },
         "dataset_id": {
             "type": "integer",
             "errorMessage": "Dataset `dataset_id` is required and must be an integer",
         },
     },
@@ -80,10 +85,16 @@
             "type": "string",
             "errorMessage": " `prediction` is required field, representing the prediction of the model",
         },
         "timestamp": {
             "type": "integer",
             "errorMessage": " `timestamp` is required field, must be in milliseconds example: 1627958400000",
         },
+        "confidence_score": {
+            "type": "number",
+            "minimum": 0,
+            "maximum": 1,
+            "errorMessage": " `confidence_score` must be in number between 0 and 1",
+        }
     },
-    "required": ["log_id", "model_id", "referenced_output", "prediction", "timestamp"],
+    "required": ["log_id", "model_id", "input", "referenced_output", "prediction", "timestamp"],
 }
```

