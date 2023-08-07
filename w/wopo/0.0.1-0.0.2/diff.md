# Comparing `tmp/wopo-0.0.1.tar.gz` & `tmp/wopo-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wopo-0.0.1.tar", last modified: Thu Aug  3 11:14:38 2023, max compression
+gzip compressed data, was "wopo-0.0.2.tar", last modified: Mon Aug  7 10:30:29 2023, max compression
```

## Comparing `wopo-0.0.1.tar` & `wopo-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 11:14:38.513497 wopo-0.0.1/
--rw-rw-rw-   0        0        0     1087 2023-08-03 05:46:02.000000 wopo-0.0.1/LICENSE.md
--rw-rw-rw-   0        0        0      636 2023-08-03 11:14:38.511992 wopo-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-08-03 04:35:55.000000 wopo-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-08-03 11:14:38.513497 wopo-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      930 2023-08-03 11:14:22.000000 wopo-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-03 11:14:38.491420 wopo-0.0.1/wopo/
--rw-rw-rw-   0        0        0        0 2023-08-03 06:46:12.000000 wopo-0.0.1/wopo/__init__.py
--rw-rw-rw-   0        0        0     3240 2023-08-03 07:06:21.000000 wopo-0.0.1/wopo/agent.py
--rw-rw-rw-   0        0        0     2399 2023-08-02 07:21:17.000000 wopo-0.0.1/wopo/prompts.py
--rw-rw-rw-   0        0        0     4643 2023-08-03 07:06:24.000000 wopo-0.0.1/wopo/wopo.py
-drwxrwxrwx   0        0        0        0 2023-08-03 11:14:38.510993 wopo-0.0.1/wopo.egg-info/
--rw-rw-rw-   0        0        0      636 2023-08-03 11:14:38.000000 wopo-0.0.1/wopo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      228 2023-08-03 11:14:38.000000 wopo-0.0.1/wopo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 11:14:38.000000 wopo-0.0.1/wopo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-08-03 11:14:38.000000 wopo-0.0.1/wopo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-08-03 11:14:38.000000 wopo-0.0.1/wopo.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-07 10:30:29.446860 wopo-0.0.2/
+-rw-rw-rw-   0        0        0     1087 2023-08-03 05:46:02.000000 wopo-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     5889 2023-08-07 10:30:29.445861 wopo-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5235 2023-08-07 07:59:17.000000 wopo-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-07 10:30:29.446860 wopo-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1059 2023-08-07 10:29:24.000000 wopo-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 10:30:29.426046 wopo-0.0.2/wopo/
+-rw-rw-rw-   0        0        0        0 2023-08-07 10:20:35.000000 wopo-0.0.2/wopo/__init__.py
+-rw-rw-rw-   0        0        0     2992 2023-08-07 07:34:12.000000 wopo-0.0.2/wopo/agent.py
+-rw-rw-rw-   0        0        0     1336 2023-08-07 07:34:02.000000 wopo-0.0.2/wopo/consolidator.py
+-rw-rw-rw-   0        0        0     4726 2023-08-07 07:18:42.000000 wopo-0.0.2/wopo/minifier.py
+-rw-rw-rw-   0        0        0     2859 2023-08-07 06:35:35.000000 wopo-0.0.2/wopo/prompts.py
+-rw-rw-rw-   0        0        0     4565 2023-08-07 07:49:19.000000 wopo-0.0.2/wopo/wopo.py
+drwxrwxrwx   0        0        0        0 2023-08-07 10:30:29.444860 wopo-0.0.2/wopo.egg-info/
+-rw-rw-rw-   0        0        0     5889 2023-08-07 10:30:29.000000 wopo-0.0.2/wopo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      267 2023-08-07 10:30:29.000000 wopo-0.0.2/wopo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 10:30:29.000000 wopo-0.0.2/wopo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-08-07 10:30:29.000000 wopo-0.0.2/wopo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-08-07 10:30:29.000000 wopo-0.0.2/wopo.egg-info/top_level.txt
```

### Comparing `wopo-0.0.1/LICENSE.md` & `wopo-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wopo-0.0.1/setup.py` & `wopo-0.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 from setuptools import setup, find_packages
 import os
-
-VERSION = '0.0.1'
+from pathlib import Path
+VERSION = '0.0.2'
 DESCRIPTION = 'wordlabs open prompt optimiser: Automatic prompt optimisation'
-long_description = 'Non parametric plug and play prompt optimisation'
+this_directory = Path(__file__).parent
+long_description = (this_directory / "README.md").read_text()
 
 # Setting up
 setup(
     name="wopo",
     version=VERSION,
     author="wordlabs.io",
     author_email="<tanishk.kithannae@wordlabs.io>",
+    url="https://github.com/wordlabs-io/wopo",
+    license='LICENSE.txt',
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
     install_requires=['tqdm', 'pandas'],
     keywords=['python', 'nlp', 'prompt', 'optimisation'],
     classifiers=[
-        "Development Status :: 1 - Planning",
+        "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
     ]
 )
```

### Comparing `wopo-0.0.1/wopo/agent.py` & `wopo-0.0.2/wopo/agent.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,22 +3,20 @@
 
 class Agent:
     def __init__(self, prompt: str = None, data: str = None, correct_output: str = None, text_gen = None):
         self.prompt = prompt
         self.original_prompt = prompt 
         self.data = data 
         self.correct_output = correct_output
-        self.prompt_funcs = Prompts()
+        self.prompt_funcs = Prompts(text_gen)
         self.last_output = None
         self.last_feedback = None
         self.step = 0
         self.state = []
-        self.text_gen = text_gen
 
-    
     def update_state(self, prompt: str = None, output: str = None, feedback: str = None, score: int = None):
         self.prompt = prompt
         self.last_output = output
         self.last_feedback = feedback        
         update_dict = {
             self.step: {
                 "prompt": prompt,
@@ -29,22 +27,17 @@
         }
        
         self.state.append(update_dict)
 
         self.step += 1
  
     def generate_prompt_and_output(self, prompt):
-        receive_prompt = self.text_gen(prompt)
-
-        clean_prompt = self.prompt_funcs.clean_prompt(receive_prompt)
-        clean_prompt = self.text_gen(clean_prompt)    
-        
+        clean_prompt = self.prompt_funcs.clean_prompt(prompt)
         receive_output = self.prompt_funcs.execute_prompt(clean_prompt, self.data)
-        receive_output = self.text_gen(receive_output)
-
+        
         return clean_prompt, receive_output
 
 
     def prompt_step(self):
         if self.step == 0:
             design_prompt = self.prompt_funcs.initial_prompt(self.prompt, self.data)
             prompt, output = self.generate_prompt_and_output(design_prompt)
@@ -63,16 +56,15 @@
             last_step = self.log_last_step()
             if last_step["score"] <= score:
                 self.update_state(prompt, output, feedback, score)
 
     
     def check_correctness(self, output):
         correctness_prompt = self.prompt_funcs.correctness_prompt(self.correct_output, output)
-        response = self.text_gen(correctness_prompt)
-        dictified = json.loads(response)
+        dictified = json.loads(correctness_prompt)
         return dictified
 
     def log_last_step(self):
         return self.state[-1][self.step - 1]
     
     def logs(self):
         return self.state
```

### Comparing `wopo-0.0.1/wopo/prompts.py` & `wopo-0.0.2/wopo/prompts.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,15 @@
+import copy
+
 class Prompts:
 
+    def __init__(self, generation_function = None):
+        #assert generation_function is not None, "Text generation not provided, initialisation failed"
+        self.generation_function = copy.deepcopy(generation_function)
+
     def initial_prompt(self, prompt: str, data: str = None):
         prompt = f"""
         Design a prompt in the following format: "Acting as a [role], [task]". The task is being performed on the data called context. Be as clear and detailed in the steps as possible. The entire prompt must be a single paragraph
         The task is as follows: {prompt}
         And the context for the task is as follows: {data}
         """
         return prompt
@@ -14,46 +20,49 @@
 
         prompt: {prompt}
         data: {data}
         expected_output: {expected_output}
         received_output: {received_output}
         feedback: {feedback}
         """
-        return prompt
+        return self.generation_function(prompt)
     
     def execute_prompt(self, prompt:str, data: str):
         prompt = f"""
         {prompt}
 
         {data}
         """
-        return prompt
+        return self.generation_function(prompt)
 
     def clean_prompt(self, prompt: str):
         prompt = f"""
         Given this prompt, only retain steps relevant to the prompt
 
         prompt: {prompt}
         """
 
-        return prompt
+        return self.generation_function(prompt)
 
     def correctness_prompt(self, expected_output: str, received_output: str):
         prompt = f"""
         Compare these two answers. Give them a score between 0 and 100 for similarity. The response must be a JSON string with keys correctness: score, and explanation: contains explanation for why these two are different
 
         expected_output: {expected_output}
 
         received_output: {received_output}
         """
-        return prompt
+        return self.generation_function(prompt)
 
     def consolidation_prompt(self, prompts_list):
         prompts = "\n\n".join(prompts_list)
 
         prompt = f"""
         You are a prompt engineer. Extract all unique points from all the prompts. Then combine all these prompts into one single prompt that is a single paragraph. Only return the combined prompt
 
         {prompts}
         """
 
-        return prompt
+        return self.generation_function(prompt)
+
+    def execute(self, prompt):
+        return self.generation_function(prompt)
```

### Comparing `wopo-0.0.1/wopo/wopo.py` & `wopo-0.0.2/wopo/wopo.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 import os
 import json
 from prefect import task, flow 
+from tqdm import tqdm  
+import copy
+
 from wopo.prompts import Prompts
 from wopo.agent import Agent 
-import pandas as pd
-from tqdm import tqdm  
+from wopo.consolidator import Consolidator
+from wopo.minifier import EntropyMinifier
 
 class WOPO:
-    def __init__(self, prompt, data, text_gen_func = None, process_verbose: bool = False):
+    def __init__(self, prompt, data, text_gen_func = None, strategy: str = "max", process_verbose: bool = False):
         self.agents = [Agent(prompt, datapoint["context"], datapoint["output"], text_gen_func) for datapoint in data]
-        self.prompter = Prompts()
+        self.prompter = Prompts(text_gen_func)
         
         assert text_gen_func is not None, "Text Generation Function not provided"
-        self.text_gen = text_gen_func
+        self.text_gen = copy.deepcopy(text_gen_func)
 
         self.optimal_prompt = None 
+        self.consolidator = Consolidator(strategy = strategy)
 
-    def run_optimisation(self, mode: str = "brute_force", num_iters: int = 1, num_steps_per_iter: int = 1, top_k: int = 1, retries_on_failure: int = 3, retry_delay_seconds: int = 15): 
+    def run_optimisation(self, num_iters: int = 1, num_steps_per_iter: int = 1, top_k: int = 1, random_sample_size: int = 1, cutoff_score: int = 100, retries_on_failure: int = 3, retry_delay_seconds: int = 15): 
 
         results = {}
         agent_states = {}
 
         @task(retries = retries_on_failure, retry_delay_seconds = retry_delay_seconds) 
         def run_one_step_for_agent(a):
             a.prompt_step()
@@ -31,52 +35,32 @@
 
         @flow(retries = retries_on_failure, retry_delay_seconds = retry_delay_seconds) 
         def run_the_step():
             run_one_step_for_agent.map(self.agents)
 
         @flow(retries = retries_on_failure, retry_delay_seconds = retry_delay_seconds)
         def correctness():
-            temp = check_correctness_for_agent.map(self.agents)
-            return temp
-   
-        def consolidate_scores(agent_scores):
-            df = pd.DataFrame.from_dict(agent_scores)
-            avg_score = df["score"].mean()
-            min_score = df["score"].min()
-            max_score = df["score"].max()
-
-            results = {
-                "avg": avg_score,
-                "max": max_score,
-                "min": min_score
-            }
-
-            df = df.nlargest(top_k, "score")
-            df = df["prompt"]
-            prompt_list = df.tolist()
-            if len(prompt_list) > 1:
-                consolidate_prompt = self.prompter.consolidation_prompt(prompt_list)
-                consolidate_prompt = self.text_gen(consolidate_prompt)
-            else:
-                consolidate_prompt = prompt_list[0]
-
-            return consolidate_prompt, results
-
+            correctness_levels = check_correctness_for_agent.map(self.agents)
+            return correctness_levels
 
         for i in tqdm(range(num_iters)):
             
             for step in range(num_steps_per_iter):
                 run_the_step()
         
             correctness_scores = correctness()
             correctness_scores = [a.result() for a in correctness_scores]
-            consolidated_prompt, step_results = consolidate_scores(correctness_scores)
+            consolidated_prompt, step_results = self.consolidator.consolidate(top_k, random_sample_size, correctness_scores)#consolidate_scores(correctness_scores)
             
             agent_states[i] = [agent.logs() for agent in self.agents]
 
+            if step_results['min'] >= cutoff_score:
+                print(f"Early stopping at step {i}, minimum score is {step_results['min']}")
+                break
+
             self.agents = [agent.flush(consolidated_prompt) for agent in self.agents]
             
             results[i] = step_results
 
         self.optimal_prompt = consolidated_prompt
         return consolidated_prompt, results, agent_states
 
@@ -87,15 +71,15 @@
 
         for i in tqdm(range(num_iters)):
             agent.prompt_step()
             if agent.log_last_step()["score"] >= stop_at_score:
                 print(f"Early stopping at step {i}")
                 break
         self.optimal_prompt = agent.prompt 
-        return agent.prompt
+        return agent.prompt, agent.logs()
 
     def run_test(self, data, save_location: str = None):
         assert self.optimal_prompt is not None, "Optimal prompt not provided or found"
         df_data = []
 
         for d in data:
             prompt = self.prompter.execute_prompt(self.optimal_prompt, d["context"])
@@ -114,10 +98,12 @@
             df_data.append(df_data_dict)
         
         df = pd.DataFrame.from_dict(df_data)
         df.to_csv(save_location)
 
         return df
 
+    def minify(self, minification_model: str = 'bert-base-uncased', percentile: int = 0.1):
+        minifier = EntropyMinifier(model_name = minification_model, p = probability)
 
-
+        return minifier.minify(self.optimal_prompt)
```

