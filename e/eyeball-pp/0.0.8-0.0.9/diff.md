# Comparing `tmp/eyeball_pp-0.0.8.tar.gz` & `tmp/eyeball_pp-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eyeball_pp-0.0.8.tar", last modified: Fri Aug  4 02:32:18 2023, max compression
+gzip compressed data, was "eyeball_pp-0.0.9.tar", last modified: Fri Aug  4 05:39:06 2023, max compression
```

## Comparing `eyeball_pp-0.0.8.tar` & `eyeball_pp-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 revant     (501) staff       (20)        0 2023-08-04 02:32:18.285427 eyeball_pp-0.0.8/
--rw-r--r--   0 revant     (501) staff       (20)    11357 2023-06-21 17:31:20.000000 eyeball_pp-0.0.8/LICENSE
--rw-r--r--   0 revant     (501) staff       (20)     9022 2023-08-04 02:32:18.285586 eyeball_pp-0.0.8/PKG-INFO
--rw-r--r--   0 revant     (501) staff       (20)     8639 2023-08-03 04:44:59.000000 eyeball_pp-0.0.8/README.md
-drwxr-xr-x   0 revant     (501) staff       (20)        0 2023-08-04 02:32:18.283359 eyeball_pp-0.0.8/eyeball_pp/
--rw-r--r--   0 revant     (501) staff       (20)      881 2023-08-02 22:46:42.000000 eyeball_pp-0.0.8/eyeball_pp/__init__.py
--rw-r--r--   0 revant     (501) staff       (20)     3661 2023-08-03 23:07:44.000000 eyeball_pp-0.0.8/eyeball_pp/classes.py
--rw-r--r--   0 revant     (501) staff       (20)     5419 2023-08-03 23:07:38.000000 eyeball_pp-0.0.8/eyeball_pp/comparators.py
--rw-r--r--   0 revant     (501) staff       (20)      201 2023-06-27 19:58:23.000000 eyeball_pp-0.0.8/eyeball_pp/compare_checkpoints.py
--rw-r--r--   0 revant     (501) staff       (20)    46598 2023-08-04 01:55:30.000000 eyeball_pp-0.0.8/eyeball_pp/eval.py
--rw-r--r--   0 revant     (501) staff       (20)    42067 2023-08-04 01:49:39.000000 eyeball_pp-0.0.8/eyeball_pp/recorders.py
--rw-r--r--   0 revant     (501) staff       (20)     3879 2023-08-03 20:00:41.000000 eyeball_pp-0.0.8/eyeball_pp/utils.py
-drwxr-xr-x   0 revant     (501) staff       (20)        0 2023-08-04 02:32:18.285070 eyeball_pp-0.0.8/eyeball_pp.egg-info/
--rw-r--r--   0 revant     (501) staff       (20)     9022 2023-08-04 02:32:18.000000 eyeball_pp-0.0.8/eyeball_pp.egg-info/PKG-INFO
--rw-r--r--   0 revant     (501) staff       (20)      340 2023-08-04 02:32:18.000000 eyeball_pp-0.0.8/eyeball_pp.egg-info/SOURCES.txt
--rw-r--r--   0 revant     (501) staff       (20)        1 2023-08-04 02:32:18.000000 eyeball_pp-0.0.8/eyeball_pp.egg-info/dependency_links.txt
--rw-r--r--   0 revant     (501) staff       (20)       11 2023-08-04 02:32:18.000000 eyeball_pp-0.0.8/eyeball_pp.egg-info/top_level.txt
--rw-r--r--   0 revant     (501) staff       (20)      527 2023-08-04 02:32:18.286470 eyeball_pp-0.0.8/setup.cfg
--rw-r--r--   0 revant     (501) staff       (20)       38 2023-06-23 17:41:10.000000 eyeball_pp-0.0.8/setup.py
+drwxr-xr-x   0 revant     (501) staff       (20)        0 2023-08-04 05:39:06.163205 eyeball_pp-0.0.9/
+-rw-r--r--   0 revant     (501) staff       (20)    11357 2023-06-21 17:31:20.000000 eyeball_pp-0.0.9/LICENSE
+-rw-r--r--   0 revant     (501) staff       (20)     8907 2023-08-04 05:39:06.163459 eyeball_pp-0.0.9/PKG-INFO
+-rw-r--r--   0 revant     (501) staff       (20)     8524 2023-08-04 03:09:19.000000 eyeball_pp-0.0.9/README.md
+drwxr-xr-x   0 revant     (501) staff       (20)        0 2023-08-04 05:39:06.145704 eyeball_pp-0.0.9/eyeball_pp/
+-rw-r--r--   0 revant     (501) staff       (20)      881 2023-08-02 22:46:42.000000 eyeball_pp-0.0.9/eyeball_pp/__init__.py
+-rw-r--r--   0 revant     (501) staff       (20)     3661 2023-08-03 23:07:44.000000 eyeball_pp-0.0.9/eyeball_pp/classes.py
+-rw-r--r--   0 revant     (501) staff       (20)     5419 2023-08-03 23:07:38.000000 eyeball_pp-0.0.9/eyeball_pp/comparators.py
+-rw-r--r--   0 revant     (501) staff       (20)      201 2023-06-27 19:58:23.000000 eyeball_pp-0.0.9/eyeball_pp/compare_checkpoints.py
+-rw-r--r--   0 revant     (501) staff       (20)    47666 2023-08-04 05:15:40.000000 eyeball_pp-0.0.9/eyeball_pp/eval.py
+-rw-r--r--   0 revant     (501) staff       (20)    42067 2023-08-04 01:49:39.000000 eyeball_pp-0.0.9/eyeball_pp/recorders.py
+-rw-r--r--   0 revant     (501) staff       (20)     3879 2023-08-03 20:00:41.000000 eyeball_pp-0.0.9/eyeball_pp/utils.py
+drwxr-xr-x   0 revant     (501) staff       (20)        0 2023-08-04 05:39:06.162643 eyeball_pp-0.0.9/eyeball_pp.egg-info/
+-rw-r--r--   0 revant     (501) staff       (20)     8907 2023-08-04 05:39:06.000000 eyeball_pp-0.0.9/eyeball_pp.egg-info/PKG-INFO
+-rw-r--r--   0 revant     (501) staff       (20)      340 2023-08-04 05:39:06.000000 eyeball_pp-0.0.9/eyeball_pp.egg-info/SOURCES.txt
+-rw-r--r--   0 revant     (501) staff       (20)        1 2023-08-04 05:39:06.000000 eyeball_pp-0.0.9/eyeball_pp.egg-info/dependency_links.txt
+-rw-r--r--   0 revant     (501) staff       (20)       11 2023-08-04 05:39:06.000000 eyeball_pp-0.0.9/eyeball_pp.egg-info/top_level.txt
+-rw-r--r--   0 revant     (501) staff       (20)      527 2023-08-04 05:39:06.164586 eyeball_pp-0.0.9/setup.cfg
+-rw-r--r--   0 revant     (501) staff       (20)       38 2023-06-23 17:41:10.000000 eyeball_pp-0.0.9/setup.py
```

### Comparing `eyeball_pp-0.0.8/LICENSE` & `eyeball_pp-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `eyeball_pp-0.0.8/PKG-INFO` & `eyeball_pp-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eyeball_pp
-Version: 0.0.8
+Version: 0.0.9
 Summary: A python package for evaluating tasks which use llms
 Home-page: https://github.com/revantk/eyeball-plus-plus
 Author: Revant
 Author-email: revant.kapoor@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -47,20 +47,18 @@
 ```
 If you want to record additional inputs within your function call you can just call `eyeball_pp.record_input('variable_name', value)` inside your function.
 
 If your sytem is more complicated, you can also use the `record_input` and `record_output` functions with the start_recording_session context manager
 ```python
 import eyeball_pp
 
-# your task code 
-...
 with eyeball_pp.start_recording_session(task_name="your_task", checkpoint_id="some_custom_unique_id"):
   eyeball_pp.record_input('input_a', input_a_value)
   eyeball_pp.record_input('input_b', input_b_value)
-  ...
+  # your task code
   eyeball_pp.record_output(output)
 ```
 
 OR without the context manager.. 
 
 ```python
 eyeball_pp.record_input(task_name="your_task", checkpoint_id="some_custom_unique_id", variable_name="input_a", value=input_a_value)
@@ -119,28 +117,29 @@
 ```
 
 The comparison will also output a benchmark.md file in your repo with the comparison results in a tabular format.
 
 # Configuration 
 
 ## Serialization
-For the `record_task` decorator you need to ensure that the inputs to the function and outputs are json serialable. If the variables are custom classes you can define the `to_json` and `from_json` functions on that object. If you want to skip serializing some inputs you can specify that in the decorator as `args_to_skip` 
+For the `record_task` decorator you need to ensure that the inputs to the function and outputs are json serialable. If the variables are custom classes you can define the `to_json` function on that object.
 eg. 
 ```python
 @eyeball_pp.record_task(args_to_skip=["input_a"])
-def your_task_function(input_a, input_b: SomeComplexType) -> str:
+def your_task_function(input_a, input_b: SomeComplexType) -> SomeComplexOutput:
   ...
   return task_output
 
 class SomeComplexType:
   def to_json(self) -> str:
     ...
 
-  def from_json(json_str: str) -> 'SomeComplexType':
-    ...  
+class SomeComplexOutput:
+  def to_json(self) -> str:
+    ...
 ```
 
 ## Sample rate 
 You can set the sample rate for recording, by default it's 1.0
 ```python
 # Set separate config for dev and production 
 if is_dev_build():
```

### Comparing `eyeball_pp-0.0.8/README.md` & `eyeball_pp-0.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -35,20 +35,18 @@
 ```
 If you want to record additional inputs within your function call you can just call `eyeball_pp.record_input('variable_name', value)` inside your function.
 
 If your sytem is more complicated, you can also use the `record_input` and `record_output` functions with the start_recording_session context manager
 ```python
 import eyeball_pp
 
-# your task code 
-...
 with eyeball_pp.start_recording_session(task_name="your_task", checkpoint_id="some_custom_unique_id"):
   eyeball_pp.record_input('input_a', input_a_value)
   eyeball_pp.record_input('input_b', input_b_value)
-  ...
+  # your task code
   eyeball_pp.record_output(output)
 ```
 
 OR without the context manager.. 
 
 ```python
 eyeball_pp.record_input(task_name="your_task", checkpoint_id="some_custom_unique_id", variable_name="input_a", value=input_a_value)
@@ -107,28 +105,29 @@
 ```
 
 The comparison will also output a benchmark.md file in your repo with the comparison results in a tabular format.
 
 # Configuration 
 
 ## Serialization
-For the `record_task` decorator you need to ensure that the inputs to the function and outputs are json serialable. If the variables are custom classes you can define the `to_json` and `from_json` functions on that object. If you want to skip serializing some inputs you can specify that in the decorator as `args_to_skip` 
+For the `record_task` decorator you need to ensure that the inputs to the function and outputs are json serialable. If the variables are custom classes you can define the `to_json` function on that object.
 eg. 
 ```python
 @eyeball_pp.record_task(args_to_skip=["input_a"])
-def your_task_function(input_a, input_b: SomeComplexType) -> str:
+def your_task_function(input_a, input_b: SomeComplexType) -> SomeComplexOutput:
   ...
   return task_output
 
 class SomeComplexType:
   def to_json(self) -> str:
     ...
 
-  def from_json(json_str: str) -> 'SomeComplexType':
-    ...  
+class SomeComplexOutput:
+  def to_json(self) -> str:
+    ...
 ```
 
 ## Sample rate 
 You can set the sample rate for recording, by default it's 1.0
 ```python
 # Set separate config for dev and production 
 if is_dev_build():
```

### Comparing `eyeball_pp-0.0.8/eyeball_pp/__init__.py` & `eyeball_pp-0.0.9/eyeball_pp/__init__.py`

 * *Files identical despite different names*

### Comparing `eyeball_pp-0.0.8/eyeball_pp/classes.py` & `eyeball_pp-0.0.9/eyeball_pp/classes.py`

 * *Files identical despite different names*

### Comparing `eyeball_pp-0.0.8/eyeball_pp/comparators.py` & `eyeball_pp-0.0.9/eyeball_pp/comparators.py`

 * *Files identical despite different names*

### Comparing `eyeball_pp-0.0.8/eyeball_pp/eval.py` & `eyeball_pp-0.0.9/eyeball_pp/eval.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,18 +55,14 @@
 
 
 @runtime_checkable
 class JsonSerializable(Protocol):
     def to_json(self) -> str:
         ...
 
-    @staticmethod
-    def from_json(json_str: str) -> "JsonSerializable":
-        ...
-
 
 T = TypeVar("T", int, float, str, bool, bytes, dict, list, None, JsonSerializable)
 
 
 @dataclass
 class EvaluatorConfig:
     sample_rate: float = 1.0
@@ -1018,18 +1014,41 @@
             return
 
         rolling_averages: list[dict[str, Any]] = []
 
         date_to_use = datetime.datetime.utcnow().date()
         scored_checkpoints.sort(key=lambda x: x.checkpoint_id, reverse=True)
 
+        # Group by reruns if they exist
+        rerun_ids_to_score: dict[str, list[Checkpoint]] = defaultdict(list)
+        for checkpoint in scored_checkpoints:
+            if rerun_id := checkpoint.rerun_metadata.get("id"):
+                rerun_ids_to_score[rerun_id].append(checkpoint)
+
+        rerun_rows = []
+        for rerun_id, checkpoints in sorted(
+            rerun_ids_to_score.items(), key=lambda x: x[0], reverse=True
+        ):
+            # We want to show how many inputs performed better in this re-run ideally
+            # For now let's show score and then change it up
+            row: dict[str, Any] = {"rerun_id": rerun_id}
+            rerun_input_hashes: set[str] = set()
+            for checkpoint in checkpoints:
+                rerun_input_hashes.add(checkpoint.get_input_hash())
+                for output_name, output_score in checkpoint.scores.items():
+                    if output_name not in row:
+                        row[output_name] = output_score.score
+                    else:
+                        row[output_name] += output_score.score
+            row["num_checkpoints_used"] = len(checkpoints)
+            row["input_diversity"] = len(input_hashes)
+            rerun_rows.append(row)
+        output_table(rerun_rows, title="Rerun stats")
+
         for output_name in sorted(output_names_to_score):
-            output_display_name = (
-                output_name if output_name != TASK_OUTPUT_KEY else "Task output"
-            )
             while scored_checkpoints[-1].created_at.date() <= date_to_use:
                 total_score = 0.0
                 num_checkpoints_used = 0
                 input_hash_set = set()
                 for checkpoint in scored_checkpoints:
                     if num_checkpoints_used >= num_samples:
                         break
```

### Comparing `eyeball_pp-0.0.8/eyeball_pp/recorders.py` & `eyeball_pp-0.0.9/eyeball_pp/recorders.py`

 * *Files identical despite different names*

### Comparing `eyeball_pp-0.0.8/eyeball_pp/utils.py` & `eyeball_pp-0.0.9/eyeball_pp/utils.py`

 * *Files identical despite different names*

### Comparing `eyeball_pp-0.0.8/eyeball_pp.egg-info/PKG-INFO` & `eyeball_pp-0.0.9/eyeball_pp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eyeball-pp
-Version: 0.0.8
+Version: 0.0.9
 Summary: A python package for evaluating tasks which use llms
 Home-page: https://github.com/revantk/eyeball-plus-plus
 Author: Revant
 Author-email: revant.kapoor@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -47,20 +47,18 @@
 ```
 If you want to record additional inputs within your function call you can just call `eyeball_pp.record_input('variable_name', value)` inside your function.
 
 If your sytem is more complicated, you can also use the `record_input` and `record_output` functions with the start_recording_session context manager
 ```python
 import eyeball_pp
 
-# your task code 
-...
 with eyeball_pp.start_recording_session(task_name="your_task", checkpoint_id="some_custom_unique_id"):
   eyeball_pp.record_input('input_a', input_a_value)
   eyeball_pp.record_input('input_b', input_b_value)
-  ...
+  # your task code
   eyeball_pp.record_output(output)
 ```
 
 OR without the context manager.. 
 
 ```python
 eyeball_pp.record_input(task_name="your_task", checkpoint_id="some_custom_unique_id", variable_name="input_a", value=input_a_value)
@@ -119,28 +117,29 @@
 ```
 
 The comparison will also output a benchmark.md file in your repo with the comparison results in a tabular format.
 
 # Configuration 
 
 ## Serialization
-For the `record_task` decorator you need to ensure that the inputs to the function and outputs are json serialable. If the variables are custom classes you can define the `to_json` and `from_json` functions on that object. If you want to skip serializing some inputs you can specify that in the decorator as `args_to_skip` 
+For the `record_task` decorator you need to ensure that the inputs to the function and outputs are json serialable. If the variables are custom classes you can define the `to_json` function on that object.
 eg. 
 ```python
 @eyeball_pp.record_task(args_to_skip=["input_a"])
-def your_task_function(input_a, input_b: SomeComplexType) -> str:
+def your_task_function(input_a, input_b: SomeComplexType) -> SomeComplexOutput:
   ...
   return task_output
 
 class SomeComplexType:
   def to_json(self) -> str:
     ...
 
-  def from_json(json_str: str) -> 'SomeComplexType':
-    ...  
+class SomeComplexOutput:
+  def to_json(self) -> str:
+    ...
 ```
 
 ## Sample rate 
 You can set the sample rate for recording, by default it's 1.0
 ```python
 # Set separate config for dev and production 
 if is_dev_build():
```

### Comparing `eyeball_pp-0.0.8/setup.cfg` & `eyeball_pp-0.0.9/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = eyeball_pp
-version = 0.0.8
+version = 0.0.9
 description = A python package for evaluating tasks which use llms
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Revant
 author_email = revant.kapoor@gmail.com
 url = https://github.com/revantk/eyeball-plus-plus
 license_files = LICENSE
```

