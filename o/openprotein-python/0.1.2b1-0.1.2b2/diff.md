# Comparing `tmp/openprotein_python-0.1.2b1.tar.gz` & `tmp/openprotein_python-0.1.2b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openprotein_python-0.1.2b1.tar", max compression
+gzip compressed data, was "openprotein_python-0.1.2b2.tar", max compression
```

## Comparing `openprotein_python-0.1.2b1.tar` & `openprotein_python-0.1.2b2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1543 2023-08-02 06:48:12.466765 openprotein_python-0.1.2b1/LICENSE.txt
--rw-r--r--   0        0        0     3164 2023-08-04 08:49:21.689589 openprotein_python-0.1.2b1/README.md
--rw-r--r--   0        0        0     2038 2023-08-04 07:48:08.230937 openprotein_python-0.1.2b1/openprotein/__init__.py
--rw-r--r--   0        0        0      215 2023-08-04 09:02:27.429044 openprotein_python-0.1.2b1/openprotein/_version.py
--rw-r--r--   0        0        0      127 2023-08-04 06:44:36.034727 openprotein_python-0.1.2b1/openprotein/api/__init__.py
--rw-r--r--   0        0        0    13237 2023-08-04 07:48:16.095012 openprotein_python-0.1.2b1/openprotein/api/data.py
--rw-r--r--   0        0        0     8533 2023-08-04 07:48:18.115031 openprotein_python-0.1.2b1/openprotein/api/design.py
--rw-r--r--   0        0        0    22209 2023-08-04 07:48:20.099050 openprotein_python-0.1.2b1/openprotein/api/embedding.py
--rw-r--r--   0        0        0    14511 2023-08-04 08:03:09.699478 openprotein_python-0.1.2b1/openprotein/api/jobs.py
--rw-r--r--   0        0        0    41896 2023-08-04 07:48:24.079088 openprotein_python-0.1.2b1/openprotein/api/poet.py
--rw-r--r--   0        0        0    17751 2023-08-04 07:48:26.059107 openprotein_python-0.1.2b1/openprotein/api/predict.py
--rw-r--r--   0        0        0    19453 2023-08-04 07:48:28.387129 openprotein_python-0.1.2b1/openprotein/api/train.py
--rw-r--r--   0        0        0     3069 2023-08-04 07:48:10.634960 openprotein_python-0.1.2b1/openprotein/base.py
--rw-r--r--   0        0        0      170 2023-08-04 06:44:36.034727 openprotein_python-0.1.2b1/openprotein/config.py
--rw-r--r--   0        0        0     1146 2023-08-04 06:44:36.034727 openprotein_python-0.1.2b1/openprotein/errors.py
--rw-r--r--   0        0        0     1055 2023-08-04 06:44:36.034727 openprotein_python-0.1.2b1/openprotein/fasta.py
--rw-r--r--   0        0        0     8620 2023-08-04 08:02:42.863225 openprotein_python-0.1.2b1/openprotein/models.py
--rw-r--r--   0        0        0      597 2023-08-04 09:16:16.480865 openprotein_python-0.1.2b1/pyproject.toml
--rw-r--r--   0        0        0     3944 1970-01-01 00:00:00.000000 openprotein_python-0.1.2b1/PKG-INFO
+-rw-r--r--   0        0        0     1543 2023-08-02 06:48:12.466765 openprotein_python-0.1.2b2/LICENSE.txt
+-rw-r--r--   0        0        0     4779 2023-08-04 09:20:47.647431 openprotein_python-0.1.2b2/README.md
+-rw-r--r--   0        0        0     2038 2023-08-04 09:17:01.541290 openprotein_python-0.1.2b2/openprotein/__init__.py
+-rw-r--r--   0        0        0      215 2023-08-04 09:17:01.541290 openprotein_python-0.1.2b2/openprotein/_version.py
+-rw-r--r--   0        0        0      127 2023-08-04 09:17:01.541290 openprotein_python-0.1.2b2/openprotein/api/__init__.py
+-rw-r--r--   0        0        0    13237 2023-08-04 09:17:01.541290 openprotein_python-0.1.2b2/openprotein/api/data.py
+-rw-r--r--   0        0        0     8533 2023-08-04 09:17:01.541290 openprotein_python-0.1.2b2/openprotein/api/design.py
+-rw-r--r--   0        0        0    22209 2023-08-04 09:17:01.541290 openprotein_python-0.1.2b2/openprotein/api/embedding.py
+-rw-r--r--   0        0        0    14511 2023-08-04 09:17:01.541290 openprotein_python-0.1.2b2/openprotein/api/jobs.py
+-rw-r--r--   0        0        0    41896 2023-08-04 09:17:01.541290 openprotein_python-0.1.2b2/openprotein/api/poet.py
+-rw-r--r--   0        0        0    17751 2023-08-04 09:17:01.541290 openprotein_python-0.1.2b2/openprotein/api/predict.py
+-rw-r--r--   0        0        0    19453 2023-08-04 09:17:01.541290 openprotein_python-0.1.2b2/openprotein/api/train.py
+-rw-r--r--   0        0        0     3069 2023-08-04 09:17:01.541290 openprotein_python-0.1.2b2/openprotein/base.py
+-rw-r--r--   0        0        0      170 2023-08-04 09:17:01.541290 openprotein_python-0.1.2b2/openprotein/config.py
+-rw-r--r--   0        0        0     1146 2023-08-04 09:17:01.541290 openprotein_python-0.1.2b2/openprotein/errors.py
+-rw-r--r--   0        0        0     1055 2023-08-04 09:17:01.541290 openprotein_python-0.1.2b2/openprotein/fasta.py
+-rw-r--r--   0        0        0     8620 2023-08-04 09:17:01.541290 openprotein_python-0.1.2b2/openprotein/models.py
+-rw-r--r--   0        0        0      597 2023-08-04 09:21:17.895719 openprotein_python-0.1.2b2/pyproject.toml
+-rw-r--r--   0        0        0     5559 1970-01-01 00:00:00.000000 openprotein_python-0.1.2b2/PKG-INFO
```

### Comparing `openprotein_python-0.1.2b1/LICENSE.txt` & `openprotein_python-0.1.2b2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.1.2b1/openprotein/__init__.py` & `openprotein_python-0.1.2b2/openprotein/__init__.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.1.2b1/openprotein/api/data.py` & `openprotein_python-0.1.2b2/openprotein/api/data.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.1.2b1/openprotein/api/design.py` & `openprotein_python-0.1.2b2/openprotein/api/design.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.1.2b1/openprotein/api/embedding.py` & `openprotein_python-0.1.2b2/openprotein/api/embedding.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.1.2b1/openprotein/api/jobs.py` & `openprotein_python-0.1.2b2/openprotein/api/jobs.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.1.2b1/openprotein/api/poet.py` & `openprotein_python-0.1.2b2/openprotein/api/poet.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.1.2b1/openprotein/api/predict.py` & `openprotein_python-0.1.2b2/openprotein/api/predict.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.1.2b1/openprotein/api/train.py` & `openprotein_python-0.1.2b2/openprotein/api/train.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.1.2b1/openprotein/base.py` & `openprotein_python-0.1.2b2/openprotein/base.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.1.2b1/openprotein/errors.py` & `openprotein_python-0.1.2b2/openprotein/errors.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.1.2b1/openprotein/fasta.py` & `openprotein_python-0.1.2b2/openprotein/fasta.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.1.2b1/openprotein/models.py` & `openprotein_python-0.1.2b2/openprotein/models.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.1.2b1/pyproject.toml` & `openprotein_python-0.1.2b2/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "openprotein_python"
 packages = [{include = "openprotein"}]
-version = "0.1.2b1"
+version = "0.1.2b2"
 description = "OpenProtein Python interface."
 license = "MIT"
 readme = "README.md"
 homepage = "https://docs.openprotein.ai/"
 authors = ["OpenProtein <info@ne47.bio>"]
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `openprotein_python-0.1.2b1/PKG-INFO` & `openprotein_python-0.1.2b2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,80 +1,82 @@
-Metadata-Version: 2.1
-Name: openprotein-python
-Version: 0.1.2b1
-Summary: OpenProtein Python interface.
-Home-page: https://docs.openprotein.ai/
-License: MIT
-Author: OpenProtein
-Author-email: info@ne47.bio
-Requires-Python: >=3.8,<4.0
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Requires-Dist: pandas (>=1)
-Requires-Dist: pydantic (>=1)
-Requires-Dist: requests (>=2)
-Requires-Dist: tqdm (>=4)
-Description-Content-Type: text/markdown
-
 [![PyPI version](https://badge.fury.io/py/openprotein-python.svg)](https://pypi.org/project/openprotein-python/)
 [![Coverage](https://dev.docs.openprotein.ai/api-python/_images/coverage.svg)](https://pypi.org/project/openprotein-python/)
-
 # openprotein-python
-Python interface for the OpenProtein.AI REST API.
+The OpenProtein.AI Python Interface provides a user-friendly library to interact with the OpenProtein.AI REST API, enabling various tasks related to protein analysis and modeling.
 
 ## Installation 
 
-You can install with pip: 
-
+To install the python interface using pip, run the following command: 
 ```
 pip install openprotein-python
 ```
+## Requirements
+
+- Python 3.7 or higher.
+- pydantic version 1.0 or newer.
+- requests version 2.0 or newer.
+- tqdm version 4.0 or newer.
+- pandas version 1.0 or newer.
+
+
 ## Getting started
 
-First, create a session using your login credentials.
+To begin, create a session using your login credentials.
 ```
 import openprotein
+
+# replace USERNAME and PASSWORD with your actual login credentials
 session = openprotein.connect(USERNAME, PASSWORD)
 ```
+## Job Status
 
-Async calls return `AsyncJobFuture` objects that allow tracking the status of the job and retrieving the result when it's ready.
+The interface offers `AsyncJobFuture` objects for asynchronous calls, allowing tracking of job status and result retrieval when ready. Given a future, you can check its status and retrieve results.
 
-Given a future, check its status and retrieve results
+### Checking Job Status
+Check the status of an `AsyncJobFuture` using the following methods:
 ```
-future.refresh() # call the backend to update the job status
-future.done() # returns True if the job is done, meaning the status could be SUCCESS, FAILED, or CANCELLED
-future.wait() # wait until done and then fetch results, verbosity is controlled with verbose arg.
-result = future.get() # get the result from a finished job
+future.refresh()  # call the backend to update the job status
+future.done()     # returns True if the job is done, meaning the status could be SUCCESS, FAILED, or CANCELLED
 ```
 
+### Retrieving Job Results
+Once the job has finished, retrieve the results using the following methods:
+```
+result = future.wait()     # wait until done and then fetch results
 
-### Jobs interface
+#verbosity is controlled with verbose arg
+result = future.get(verbose=True)  # get the result from a finished job
+```
+
+## Jobs Interface
 
-List your jobs, optionally filtered by date, job type, and status.
+### Listing Jobs
+To view all jobs associated with each session, the following method is available, providing an option to filter results by date, job type, or status.
 ```
-session.jobs.list() # list all jobs
-session.jobs.get(JOB_ID) # get a specific job
+session.jobs.list() 
 ```
 
-Resume an `AsyncJobFuture` from where you left off with each API's load_job:
-
-For example for training jobs:
+### Retrieving Specific Job
+For detailed information about a particular job, use the following command with the corresponding job ID:
+``` 
+session.jobs.get(JOB_ID)  # Replace JOB_ID with the ID of the specific job to be retrieved
+```
 
+### Resuming Jobs
+Jobs from prior workflows can be resumed using the load_job method provided by each API. 
 ```
-session.train.load_job(JOB_ID)
+session.train.load_job(JOB_ID)  # Replace JOB_ID with the ID of the training job to resume
 ```
-### PoET interface
 
-Score sequences using the PoET interface.
+## PoET interface
+The PoET Interface allows scoring, generating, and retrieving sequences using the PoET model.
+
+### Scoring Sequences
+To score sequences, use the score function. Provide a prompt and a list of queries. The results will be a list of (sequence, score) pydantic objects.
+
 ```
 prompt_seqs = b'MALWMRLLPLLALLALWGPDPAAAFVNQHLCGSHLVEALYLVCGERGFFYTPKTRREAEDLQVGQVELGGGPGAGSLQPLALEGSLQKRGIVEQCCTSICSLYQLENYCN'
 
 prompt = session.poet.upload_prompt(prompt_seqs)
 ```
 
 ```
@@ -89,38 +91,40 @@
 
 ```
 future = session.poet.score(prompt, queries)
 result = future.wait()
 # result is a list of (sequence, score) pydantic objects
 ```
 
-Score single site variants using the PoET interface.
+### Scoring Single Site Variants
+For scoring single site variants, use the `single_site function`, providing the original sequence and setting `prompt_is_seed` to True if the prompt is a seed sequence.
 ```
 sequence = "MALWMRLLPLLALLALWGPDPAAAFVNQHLCGSHLVEALYLVCGERGFFYTPKTRREAEDLQVGQVELGGGPGAGSLQPLALEGSLQKRGIVEQCCTSICSLYQLENYCN"
 future = session.poet.single_site(prompt, sequence, prompt_is_seed=True) 
 result = future.wait()
 # result is a dictionary of {variant: score}
 ```
 
-Generate sequences from the PoET model.
+### Generating Sequences
+To generate sequences from the PoET model, use the `generate` function with relevant parameters. The result will be a list of generated samples.
 ```
-
 future = session.poet.generate(
     prompt,
     max_seqs_from_msa=1024,
     num_samples=100,
     temperature=1.0,
     topk=15
 )
 samples = future.wait()
 ```
 
-Retrieve the prompt, MSA, or input (seed) sequences for a PoET job.
+### Retrieving Input Sequences
+You can retrieve the prompt, MSA, or seed sequences for a PoET job using the `get_input` function or the individual functions for each type.
 ```
 future.get_input(INPUT_TYPE)
 # or, functions for each type
 future.get_prompt()
 future.get_msa()
 future.get_seed()
 ```
 
-See more at our [Homepage](https://docs.openprotein.ai/)
+See more at our [Homepage](https://docs.openprotein.ai/)
```

