# Comparing `tmp/lenio-ai-prompt-engineer-1.1.0.tar.gz` & `tmp/lenio-ai-prompt-engineer-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lenio-ai-prompt-engineer-1.1.0.tar", last modified: Fri Aug  4 15:54:55 2023, max compression
+gzip compressed data, was "lenio-ai-prompt-engineer-1.2.0.tar", last modified: Mon Aug  7 20:30:24 2023, max compression
```

## Comparing `lenio-ai-prompt-engineer-1.1.0.tar` & `lenio-ai-prompt-engineer-1.2.0.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 camilo.basualdo   (501) staff       (20)        0 2023-08-04 15:54:55.348674 lenio-ai-prompt-engineer-1.1.0/
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)       68 2023-08-04 15:54:55.348072 lenio-ai-prompt-engineer-1.1.0/PKG-INFO
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)     1808 2023-07-28 15:29:57.000000 lenio-ai-prompt-engineer-1.1.0/README.md
-drwxr-xr-x   0 camilo.basualdo   (501) staff       (20)        0 2023-08-04 15:54:55.324279 lenio-ai-prompt-engineer-1.1.0/cli/
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)        0 2023-07-27 15:34:24.000000 lenio-ai-prompt-engineer-1.1.0/cli/__init__.py
-drwxr-xr-x   0 camilo.basualdo   (501) staff       (20)        0 2023-08-04 15:54:55.329972 lenio-ai-prompt-engineer-1.1.0/cli/evals/
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)       98 2023-08-01 21:09:44.000000 lenio-ai-prompt-engineer-1.1.0/cli/evals/__init__.py
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)     4225 2023-08-04 13:18:49.000000 lenio-ai-prompt-engineer-1.1.0/cli/evals/classification.py
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)     7998 2023-08-04 15:51:37.000000 lenio-ai-prompt-engineer-1.1.0/cli/evals/elovalue.py
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)     4100 2023-08-03 22:49:29.000000 lenio-ai-prompt-engineer-1.1.0/cli/evals/equal.py
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)     4108 2023-08-04 13:41:49.000000 lenio-ai-prompt-engineer-1.1.0/cli/evals/includes.py
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)     1380 2023-08-03 22:53:37.000000 lenio-ai-prompt-engineer-1.1.0/cli/generation.py
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)     7855 2023-08-04 15:51:27.000000 lenio-ai-prompt-engineer-1.1.0/cli/main.py
-drwxr-xr-x   0 camilo.basualdo   (501) staff       (20)        0 2023-08-04 15:54:55.339943 lenio-ai-prompt-engineer-1.1.0/cli/promptChange/
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)      254 2023-08-02 14:59:15.000000 lenio-ai-prompt-engineer-1.1.0/cli/promptChange/__init__.py
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)     1175 2023-08-03 16:41:52.000000 lenio-ai-prompt-engineer-1.1.0/cli/promptChange/grammatical_errors.py
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)      250 2023-08-01 23:12:10.000000 lenio-ai-prompt-engineer-1.1.0/cli/promptChange/lowercase.py
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)      438 2023-08-01 22:44:17.000000 lenio-ai-prompt-engineer-1.1.0/cli/promptChange/random_lowercase.py
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)      503 2023-08-01 22:44:27.000000 lenio-ai-prompt-engineer-1.1.0/cli/promptChange/random_lowercase_word.py
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)      438 2023-08-01 22:44:12.000000 lenio-ai-prompt-engineer-1.1.0/cli/promptChange/random_uppercase.py
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)      503 2023-08-01 22:44:22.000000 lenio-ai-prompt-engineer-1.1.0/cli/promptChange/random_uppercase_word.py
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)     1110 2023-08-03 18:30:27.000000 lenio-ai-prompt-engineer-1.1.0/cli/promptChange/synonymous_prompt.py
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)      250 2023-08-01 22:44:08.000000 lenio-ai-prompt-engineer-1.1.0/cli/promptChange/uppercase.py
-drwxr-xr-x   0 camilo.basualdo   (501) staff       (20)        0 2023-08-04 15:54:55.347012 lenio-ai-prompt-engineer-1.1.0/lenio_ai_prompt_engineer.egg-info/
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)       68 2023-08-04 15:54:55.000000 lenio-ai-prompt-engineer-1.1.0/lenio_ai_prompt_engineer.egg-info/PKG-INFO
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)      791 2023-08-04 15:54:55.000000 lenio-ai-prompt-engineer-1.1.0/lenio_ai_prompt_engineer.egg-info/SOURCES.txt
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)        1 2023-08-04 15:54:55.000000 lenio-ai-prompt-engineer-1.1.0/lenio_ai_prompt_engineer.egg-info/dependency_links.txt
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)       59 2023-08-04 15:54:55.000000 lenio-ai-prompt-engineer-1.1.0/lenio_ai_prompt_engineer.egg-info/entry_points.txt
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)       44 2023-08-04 15:54:55.000000 lenio-ai-prompt-engineer-1.1.0/lenio_ai_prompt_engineer.egg-info/requires.txt
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)        4 2023-08-04 15:54:55.000000 lenio-ai-prompt-engineer-1.1.0/lenio_ai_prompt_engineer.egg-info/top_level.txt
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)       38 2023-08-04 15:54:55.348895 lenio-ai-prompt-engineer-1.1.0/setup.cfg
--rw-r--r--   0 camilo.basualdo   (501) staff       (20)      388 2023-08-04 15:54:49.000000 lenio-ai-prompt-engineer-1.1.0/setup.py
+drwxr-xr-x   0 camilo.basualdo   (501) staff       (20)        0 2023-08-07 20:30:24.540533 lenio-ai-prompt-engineer-1.2.0/
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)       68 2023-08-07 20:30:24.539865 lenio-ai-prompt-engineer-1.2.0/PKG-INFO
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)     2955 2023-08-07 20:24:36.000000 lenio-ai-prompt-engineer-1.2.0/README.md
+drwxr-xr-x   0 camilo.basualdo   (501) staff       (20)        0 2023-08-07 20:30:24.522242 lenio-ai-prompt-engineer-1.2.0/cli/
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)        0 2023-07-27 15:34:24.000000 lenio-ai-prompt-engineer-1.2.0/cli/__init__.py
+drwxr-xr-x   0 camilo.basualdo   (501) staff       (20)        0 2023-08-07 20:30:24.525510 lenio-ai-prompt-engineer-1.2.0/cli/evals/
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)       98 2023-08-01 21:09:44.000000 lenio-ai-prompt-engineer-1.2.0/cli/evals/__init__.py
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)     4015 2023-08-07 16:39:39.000000 lenio-ai-prompt-engineer-1.2.0/cli/evals/classification.py
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)     7920 2023-08-07 19:35:22.000000 lenio-ai-prompt-engineer-1.2.0/cli/evals/elovalue.py
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)     3867 2023-08-07 15:30:35.000000 lenio-ai-prompt-engineer-1.2.0/cli/evals/equal.py
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)     3810 2023-08-07 18:54:01.000000 lenio-ai-prompt-engineer-1.2.0/cli/evals/includes.py
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)     1402 2023-08-07 02:29:30.000000 lenio-ai-prompt-engineer-1.2.0/cli/generation.py
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)     3039 2023-08-07 19:25:44.000000 lenio-ai-prompt-engineer-1.2.0/cli/iteration.py
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)     9535 2023-08-07 20:01:14.000000 lenio-ai-prompt-engineer-1.2.0/cli/main.py
+drwxr-xr-x   0 camilo.basualdo   (501) staff       (20)        0 2023-08-07 20:30:24.533419 lenio-ai-prompt-engineer-1.2.0/cli/promptChange/
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)      254 2023-08-02 14:59:15.000000 lenio-ai-prompt-engineer-1.2.0/cli/promptChange/__init__.py
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)     1175 2023-08-03 16:41:52.000000 lenio-ai-prompt-engineer-1.2.0/cli/promptChange/grammatical_errors.py
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)      250 2023-08-01 23:12:10.000000 lenio-ai-prompt-engineer-1.2.0/cli/promptChange/lowercase.py
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)      438 2023-08-01 22:44:17.000000 lenio-ai-prompt-engineer-1.2.0/cli/promptChange/random_lowercase.py
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)      503 2023-08-01 22:44:27.000000 lenio-ai-prompt-engineer-1.2.0/cli/promptChange/random_lowercase_word.py
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)      438 2023-08-01 22:44:12.000000 lenio-ai-prompt-engineer-1.2.0/cli/promptChange/random_uppercase.py
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)      503 2023-08-01 22:44:22.000000 lenio-ai-prompt-engineer-1.2.0/cli/promptChange/random_uppercase_word.py
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)     1110 2023-08-03 18:30:27.000000 lenio-ai-prompt-engineer-1.2.0/cli/promptChange/synonymous_prompt.py
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)      250 2023-08-01 22:44:08.000000 lenio-ai-prompt-engineer-1.2.0/cli/promptChange/uppercase.py
+drwxr-xr-x   0 camilo.basualdo   (501) staff       (20)        0 2023-08-07 20:30:24.538866 lenio-ai-prompt-engineer-1.2.0/lenio_ai_prompt_engineer.egg-info/
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)       68 2023-08-07 20:30:24.000000 lenio-ai-prompt-engineer-1.2.0/lenio_ai_prompt_engineer.egg-info/PKG-INFO
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)      808 2023-08-07 20:30:24.000000 lenio-ai-prompt-engineer-1.2.0/lenio_ai_prompt_engineer.egg-info/SOURCES.txt
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)        1 2023-08-07 20:30:24.000000 lenio-ai-prompt-engineer-1.2.0/lenio_ai_prompt_engineer.egg-info/dependency_links.txt
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)       59 2023-08-07 20:30:24.000000 lenio-ai-prompt-engineer-1.2.0/lenio_ai_prompt_engineer.egg-info/entry_points.txt
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)       44 2023-08-07 20:30:24.000000 lenio-ai-prompt-engineer-1.2.0/lenio_ai_prompt_engineer.egg-info/requires.txt
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)        4 2023-08-07 20:30:24.000000 lenio-ai-prompt-engineer-1.2.0/lenio_ai_prompt_engineer.egg-info/top_level.txt
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)       38 2023-08-07 20:30:24.541365 lenio-ai-prompt-engineer-1.2.0/setup.cfg
+-rw-r--r--   0 camilo.basualdo   (501) staff       (20)      388 2023-08-07 20:30:11.000000 lenio-ai-prompt-engineer-1.2.0/setup.py
```

### Comparing `lenio-ai-prompt-engineer-1.1.0/cli/evals/classification.py` & `lenio-ai-prompt-engineer-1.2.0/cli/evals/classification.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,74 +1,72 @@
 import openai
 
 class Classification:
-    def __init__(self, description, test_cases, number_of_prompts, generation_model, generation_model_temperature, generation_model_max_tokens, candidate_model, candidate_model_temperature, prompts):
+    def __init__(self, description, test_cases, number_of_prompts, model_test, model_test_temperature, model_test_max_tokens, model_generation, model_generation_temperature, prompts):
         self.description = description
         self.test_cases = test_cases
         self.number_of_prompts = number_of_prompts
-        self.generation_model = generation_model
-        self.candidate_model_temperature = candidate_model_temperature
-        self.generation_model_temperature = generation_model_temperature
-        self.generation_model_max_tokens = generation_model_max_tokens
-        self.candidate_model = candidate_model
+        self.model_test = model_test
+        self.model_generation = model_generation
+        self.model_test_temperature = model_test_temperature
+        self.model_test_max_tokens = model_test_max_tokens
+        self.model_generation_temperature = model_generation_temperature
         self.system_gen_system_prompt = """Your job is to generate system prompts for GPT, given a description of the use-case and some test cases.
 
         The prompts you will be generating will be for classifiers, with 'true' and 'false' being the only possible outputs.
 
         In your generated prompt, you should describe how the AI should behave in plain English. Include what it will see, and what it's allowed to output. Be creative in with prompts to get the best possible results. The AI knows it's an AI -- you don't need to tell it this.
 
         You will be graded based on the performance of your prompt... but don't cheat! You cannot include specifics about the test cases in your prompt. Any prompts with examples will be disqualified.
 
         Most importantly, output NOTHING but the prompt. Do not include anything else in your message."""
         self.prompts = prompts
 
     def test_candidate_prompts(self):
         prompt_results = {prompt: {'correct': 0, 'total': 0} for prompt in self.prompts}
-        results = [{"description": self.description, "method": "Classification"}]
+        results = [{"description": self.description, "method": "Equal"}]
         for prompt in self.prompts:
             prompt_and_results = [{"prompt": prompt}]
             for test_case in self.test_cases:
-                x = openai.ChatCompletion.create(
-                    model=self.generation_model,
+                response = openai.ChatCompletion.create(
+                    model=self.model_test,
                     messages=[
                         {"role": "system", "content": prompt},
-                        {"role": "user", "content": f"{test_case['prompt']}"}
+                        {"role": "user", "content": f"{test_case[0]}"}
                     ],
                     logit_bias={
                         '1904': 100,  # 'true' token
                         '3934': 100,  # 'false' token
                     },
-                    max_tokens=self.generation_model_max_tokens,
-                    temperature=self.generation_model_temperature,
+                    max_tokens=self.model_test_max_tokens,
+                    temperature=self.model_test_temperature,
                 ).choices[0].message.content
                 # Update model results
-                if x == test_case['answer']:
+                if response.lower() == test_case[1].lower():
                     prompt_results[prompt]['correct'] += 1
                 prompt_results[prompt]['total'] += 1
-                prompt_and_results.append({"test": test_case['prompt'], "answer": x, "ideal": test_case['answer'], "result": x == test_case['answer']})
+                prompt_and_results.append({"test": test_case[0], "answer": response, "ideal": test_case[1], "result": response.lower() == test_case[1].lower()})
             results.append(prompt_and_results)
             prompt_and_results = []
 
         # Calculate and print the percentage of correct answers and average time for each model
         best_prompt = self.prompts[0]
-        second_best_prompt = self.prompts[1]
         best_percentage = 0
-        second_best_percentage = 0
         data_list = []
         for i, prompt in enumerate(self.prompts):
             correct = prompt_results[prompt]['correct']
             total = prompt_results[prompt]['total']
             percentage = (correct / total) * 100
             data_list.append({"prompt": prompt, "rating": percentage})
             print(f"Prompt {i+1} got {percentage:.2f}% correct.")
             if percentage >= best_percentage:
-                second_best_percentage = best_percentage
-                second_best_prompt = best_prompt
                 best_percentage = percentage
                 best_prompt = prompt
-        best_prompts = [{"prompt": best_prompt, "rating": best_percentage}, {"prompt": second_best_prompt, "rating": second_best_percentage}]
+        sorted_data = sorted(data_list, key=lambda x: x['rating'], reverse=True)
+        print(sorted_data)
+        best_prompts = [sorted_data[0], sorted_data[1]]
         print(f"The best prompt was '{best_prompt}' with a correctness of {best_percentage:.2f}%.")
-        data_list.append(results)
-        return data_list, best_prompts
+        sorted_data.append(results)
+        return sorted_data, best_prompts
     
     def evaluate_optimal_prompt(self):
         return self.test_candidate_prompts()
```

### Comparing `lenio-ai-prompt-engineer-1.1.0/cli/evals/elovalue.py` & `lenio-ai-prompt-engineer-1.2.0/cli/evals/elovalue.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,24 +7,24 @@
 K = 32
 
 N_RETRIES = 3  # number of times to retry a call to the ranking model if it fails
 RANKING_MODEL = 'gpt-3.5-turbo'
 RANKING_MODEL_TEMPERATURE = 0.5
 
 class Elo:
-    def __init__(self, description, test_cases, number_of_prompts, generation_model, generation_model_temperature, generation_model_max_tokens, candidate_model, candidate_model_temperature, prompts):
+    def __init__(self, description, test_cases, number_of_prompts, model_test, model_test_temperature, model_test_max_tokens, model_generation, model_generation_temperature, prompts):
         self.description = description
         self.test_cases = test_cases
         self.number_of_prompts = number_of_prompts
-        self.generation_model = generation_model
-        self.generation_model_temperature = generation_model_temperature
-        self.generation_model_max_tokens = generation_model_max_tokens
-        self.candidate_model = candidate_model
-        self.candidate_model_temperature = candidate_model_temperature
-        self.system_gen_system_prompt = """Your job is to generate system prompts for GPT-4, given a description of the use-case and some test cases.
+        self.model_test = model_test
+        self.model_test_temperature = model_test_temperature
+        self.model_test_max_tokens = model_test_max_tokens
+        self.model_generation = model_generation
+        self.model_generation_temperature = model_generation_temperature
+        self.system_gen_system_prompt = """Your job is to generate system prompts for GPT, given a description of the use-case and some test cases.
 
 The prompts you will be generating will be for freeform tasks, such as generating a landing page headline, an intro paragraph, solving a math problem, etc.
 
 In your generated prompt, you should describe how the AI should behave in plain English. Include what it will see, and what it's allowed to output. Be creative with prompts to get the best possible results. The AI knows it's an AI -- you don't need to tell it this.
 
 You will be graded based on the performance of your prompt... but don't cheat! You cannot include specifics about the test cases in your prompt. Any prompts with examples will be disqualified.
 
@@ -54,15 +54,15 @@
     @retry(stop=stop_after_attempt(N_RETRIES), wait=wait_exponential(multiplier=1, min=4, max=70))
     def get_score(self, test_case, pos1, pos2, ranking_model_name, ranking_model_temperature):    
         score = openai.ChatCompletion.create(
             model=ranking_model_name,
             messages=[
                 {"role": "system", "content": self.ranking_system_prompt},
                 {"role": "user", "content": f"""Task: {self.description.strip()}
-    Prompt: {test_case['prompt']}
+    Prompt: {test_case}
     Generation A: {pos1}
     Generation B: {pos2}"""}
             ],
             logit_bias={
                 '32': 100,  # 'A' token
                 '33': 100,  # 'B' token
             },
@@ -70,21 +70,21 @@
             temperature=ranking_model_temperature,
         ).choices[0].message.content
         return score
 
     @retry(stop=stop_after_attempt(N_RETRIES), wait=wait_exponential(multiplier=1, min=4, max=70))
     def get_generation(self, prompt, test_case):
         generation = openai.ChatCompletion.create(
-            model=self.generation_model,
+            model=self.model_test,
             messages=[
                 {"role": "system", "content": prompt},
-                {"role": "user", "content": f"{test_case['prompt']}"}
+                {"role": "user", "content": f"{test_case}"}
             ],
-            max_tokens=self.generation_model_max_tokens,
-            temperature=self.generation_model_temperature,
+            max_tokens=self.model_test_max_tokens,
+            temperature=self.model_test_temperature,
         ).choices[0].message.content
         return generation
 
     def test_candidate_prompts(self):
     # Initialize each prompt with an ELO rating of 1200
         prompt_ratings = {prompt: 1200 for prompt in self.prompts}
 
@@ -101,15 +101,15 @@
 
         # For each pair of prompts
         for prompt1, prompt2 in itertools.combinations(self.prompts, 2):
             # For each test case
             for test_case in self.test_cases:
 
                 # Get the value of the "prompt" field as a string
-                prompt_content = test_case.get("prompt", "")
+                prompt_content = test_case
 
                 # Update progress bar
                 pbar.update()
 
                 # Generate outputs for each prompt
                 generation1 = self.get_generation(prompt1, test_case)
                 generation2 = self.get_generation(prompt2, test_case)
@@ -152,9 +152,10 @@
     def evaluate_optimal_prompt(self): 
         prompt_ratings = self.test_candidate_prompts()
         data_list = []
         for prompt, rating in sorted(prompt_ratings[0].items(), key=lambda item: item[1], reverse=True):
             data_list.append({"prompt": prompt, "rating": rating})
         data_list.append(prompt_ratings[1])
         data_list.append(prompt_ratings[2])
-        best_prompts = [data_list[0], data_list[0]]
+        best_prompts = [data_list[0], data_list[1]]
+        print(best_prompts)
         return data_list, best_prompts
```

### Comparing `lenio-ai-prompt-engineer-1.1.0/cli/evals/equal.py` & `lenio-ai-prompt-engineer-1.2.0/cli/evals/equal.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import openai
 
 class Equal:
-    def __init__(self, description, test_cases, number_of_prompts, generation_model, generation_model_temperature, generation_model_max_tokens, candidate_model, candidate_model_temperature, prompts):
+    def __init__(self, description, test_cases, number_of_prompts, model_test, model_test_temperature, model_test_max_tokens, model_generation, model_generation_temperature, prompts):
         self.description = description
         self.test_cases = test_cases
         self.number_of_prompts = number_of_prompts
-        self.generation_model = generation_model
-        self.generation_model_temperature = generation_model_temperature
-        self.generation_model_max_tokens = generation_model_max_tokens
-        self.candidate_model = candidate_model
-        self.candidate_model_temperature = candidate_model_temperature
+        self.model_test = model_test
+        self.model_test_temperature = model_test_temperature
+        self.model_test_max_tokens = model_test_max_tokens
+        self.model_generation = model_generation
+        self.model_generation_temperature = model_generation_temperature
         self.prompts = prompts
         self.system_gen_system_prompt = """Your job is to generate system prompts for GPT, given a description of the use-case and some test cases.
 
 In your generated prompt, you should describe how the AI should behave in plain English. Include what it will see, and what it's allowed to output. Be creative with prompts to get the best possible results. The AI knows it's an AI -- you don't need to tell it this.
                  
 Remember that the prompt should only allow the AI to answer the answer and nothing else. No explanation is necessary.
 
@@ -23,48 +23,46 @@
 
     def test_candidate_prompts(self):
         prompt_results = {prompt: {'correct': 0, 'total': 0} for prompt in self.prompts}
         results = [{"description": self.description, "method": "Equal"}]
         for prompt in self.prompts:
             prompt_and_results = [{"prompt": prompt}]
             for test_case in self.test_cases:
-                x = openai.ChatCompletion.create(
-                    model=self.generation_model,
+                response = openai.ChatCompletion.create(
+                    model=self.model_test,
                     messages=[
                         {"role": "system", "content": prompt},
-                        {"role": "user", "content": f"{test_case['prompt']}"}
+                        {"role": "user", "content": f"{test_case[0]}"}
                     ],
-                    max_tokens=self.generation_model_max_tokens,
-                    temperature=self.generation_model_temperature,
+                    max_tokens=self.model_test_max_tokens,
+                    temperature=self.model_test_temperature,
                 ).choices[0].message.content
                 # Update model results
-                if x.lower() == test_case['answer'].lower():
+                if response.lower() == test_case[1].lower():
                     prompt_results[prompt]['correct'] += 1
                 prompt_results[prompt]['total'] += 1
-                prompt_and_results.append({"test": test_case['prompt'], "answer": x, "ideal": test_case['answer'], "result": x.lower() == test_case['answer'].lower()})
+                prompt_and_results.append({"test": test_case[0], "answer": response, "ideal": test_case[1], "result": response.lower() == test_case[1].lower()})
             results.append(prompt_and_results)
             prompt_and_results = []
 
         # Calculate and print the percentage of correct answers and average time for each model
         best_prompt = self.prompts[0]
-        second_best_prompt = self.prompts[1]
         best_percentage = 0
-        second_best_percentage = 0
         data_list = []
         for i, prompt in enumerate(self.prompts):
             correct = prompt_results[prompt]['correct']
             total = prompt_results[prompt]['total']
             percentage = (correct / total) * 100
             data_list.append({"prompt": prompt, "rating": percentage})
             print(f"Prompt {i+1} got {percentage:.2f}% correct.")
             if percentage >= best_percentage:
-                second_best_percentage = best_percentage
-                second_best_prompt = best_prompt
                 best_percentage = percentage
                 best_prompt = prompt
-        best_prompts = [{"prompt": best_prompt, "rating": best_percentage}, {"prompt": second_best_prompt, "rating": second_best_percentage}]
+        sorted_data = sorted(data_list, key=lambda x: x['rating'], reverse=True)
+        print(sorted_data)
+        best_prompts = [sorted_data[0], sorted_data[1]]
         print(f"The best prompt was '{best_prompt}' with a correctness of {best_percentage:.2f}%.")
-        data_list.append(results)
-        return data_list, best_prompts
+        sorted_data.append(results)
+        return sorted_data, best_prompts
     
     def evaluate_optimal_prompt(self):
         return self.test_candidate_prompts()
```

### Comparing `lenio-ai-prompt-engineer-1.1.0/cli/evals/includes.py` & `lenio-ai-prompt-engineer-1.2.0/cli/evals/includes.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,70 +1,68 @@
 import openai
 
 class Includes:
-    def __init__(self, description, test_cases, number_of_prompts, generation_model, generation_model_temperature, generation_model_max_tokens, candidate_model, candidate_model_temperature, prompts):
+    def __init__(self, description, test_cases, number_of_prompts, model_test, model_test_temperature, model_test_max_tokens, model_generation, model_generation_temperature, prompts):
         self.description = description
         self.test_cases = test_cases
         self.number_of_prompts = number_of_prompts
-        self.generation_model = generation_model
-        self.candidate_model_temperature = candidate_model_temperature
-        self.generation_model_temperature = generation_model_temperature
-        self.generation_model_max_tokens = generation_model_max_tokens
-        self.candidate_model = candidate_model
+        self.model_test = model_test
+        self.model_generation = model_generation
+        self.model_test_temperature = model_test_temperature
+        self.model_test_max_tokens = model_test_max_tokens
+        self.model_generation_temperature = model_generation_temperature
         self.system_gen_system_prompt = """Your job is to generate system prompts for GPT, given a description of the use-case and some test cases.
 
         In your generated prompt, you should describe how the AI should behave in plain English. Include what it will see, and what it's allowed to output. Be creative in with prompts to get the best possible results. The AI knows it's an AI -- you don't need to tell it this.
 
         You will be graded based on the performance of your prompt... but don't cheat! You cannot include specifics about the test cases in your prompt. Any prompts with examples will be disqualified.
 
-        Specify in the prompts that you generate that they give a step-by-step response. Your final response has to be between <result></result> tags.
+        Specify in the prompts that you generate that they give a step-by-step response.
 
         Most importantly, output NOTHING but the prompt. Do not include anything else in your message."""
         self.prompts = prompts
 
     def test_candidate_prompts(self):
         prompt_results = {prompt: {'correct': 0, 'total': 0} for prompt in self.prompts}
-        results = [{"description": self.description, "method": "Includes"}]
+        results = [{"description": self.description, "method": "Equal"}]
         for prompt in self.prompts:
             prompt_and_results = [{"prompt": prompt}]
             for test_case in self.test_cases:
-                x = openai.ChatCompletion.create(
-                    model=self.generation_model,
+                response = openai.ChatCompletion.create(
+                    model=self.model_test,
                     messages=[
                         {"role": "system", "content": prompt},
-                        {"role": "user", "content": f"{test_case['prompt']}"}
+                        {"role": "user", "content": f"{test_case[0]}"}
                     ],
-                    max_tokens=self.generation_model_max_tokens,
-                    temperature=self.generation_model_temperature,
+                    max_tokens=self.model_test_max_tokens,
+                    temperature=self.model_test_temperature,
                 ).choices[0].message.content
                 # Update model results
-                if test_case['answer'].lower() in x.lower():
+                if test_case[1].lower() in response.lower():
                     prompt_results[prompt]['correct'] += 1
                 prompt_results[prompt]['total'] += 1
-                prompt_and_results.append({"test": test_case['prompt'], "answer": x, "ideal": test_case['answer'], "result": x.lower() in test_case['answer'].lower()})
+                prompt_and_results.append({"test": test_case[0], "answer": response, "ideal": test_case[1], "result": test_case[1].lower() in response.lower()})
             results.append(prompt_and_results)
             prompt_and_results = []
 
         # Calculate and print the percentage of correct answers and average time for each model
         best_prompt = self.prompts[0]
-        second_best_prompt = self.prompts[1]
         best_percentage = 0
-        second_best_percentage = 0
         data_list = []
         for i, prompt in enumerate(self.prompts):
             correct = prompt_results[prompt]['correct']
             total = prompt_results[prompt]['total']
             percentage = (correct / total) * 100
             data_list.append({"prompt": prompt, "rating": percentage})
             print(f"Prompt {i+1} got {percentage:.2f}% correct.")
             if percentage >= best_percentage:
-                second_best_percentage = best_percentage
-                second_best_prompt = best_prompt
                 best_percentage = percentage
                 best_prompt = prompt
-        best_prompts = [{"prompt": best_prompt, "rating": best_percentage}, {"prompt": second_best_prompt, "rating": second_best_percentage}]
+        sorted_data = sorted(data_list, key=lambda x: x['rating'], reverse=True)
+        print(sorted_data)
+        best_prompts = [sorted_data[0], sorted_data[1]]
         print(f"The best prompt was '{best_prompt}' with a correctness of {best_percentage:.2f}%.")
-        data_list.append(results)
-        return data_list, best_prompts
+        sorted_data.append(results)
+        return sorted_data, best_prompts
     
     def evaluate_optimal_prompt(self):
         return self.test_candidate_prompts()
```

### Comparing `lenio-ai-prompt-engineer-1.1.0/cli/generation.py` & `lenio-ai-prompt-engineer-1.2.0/cli/generation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import openai
 
-def generate_candidate_prompts(system_gen_system_prompt, test_cases, description, candidate_model, candidate_model_temperature, number_of_prompts, prompt_features=None):
+def generate_candidate_prompts(system_gen_system_prompt, test_cases, description, model_generation, model_generation_temperature, number_of_prompts, prompt_features=None):
         if prompt_features is not None:
             outputs = openai.ChatCompletion.create(
-            model='gpt-4',
+            model=model_generation,
             messages=[
                 {"role": "system", "content": system_gen_system_prompt + ' ' + prompt_features},
                 {"role": "user", "content": f"Here are some test cases:`{test_cases}`\n\nHere is the description of the use-case: `{description.strip()}`\n\nRespond with your prompt, and nothing else. Be creative."}
                 ],
-            temperature=candidate_model_temperature,
+            temperature=model_generation_temperature,
             n=number_of_prompts)
         else:
              outputs = openai.ChatCompletion.create(
-            model='gpt-4',
+            model=model_generation,
             messages=[
                 {"role": "system", "content": system_gen_system_prompt},
                 {"role": "user", "content": f"Here are some test cases:`{test_cases}`\n\nHere is the description of the use-case: `{description.strip()}`\n\nRespond with your prompt, and nothing else. Be creative."}
                 ],
-            temperature=candidate_model_temperature,
+            temperature=model_generation_temperature,
             n=number_of_prompts)
 
         prompts = []
         for i in outputs.choices:
             prompts.append(i.message.content)
         return prompts
```

### Comparing `lenio-ai-prompt-engineer-1.1.0/cli/main.py` & `lenio-ai-prompt-engineer-1.2.0/cli/main.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,96 +1,94 @@
 import argparse
 import os
 import openai
 import json
 import matplotlib.pyplot as plt
-from . import generation
+from . import generation, iteration
 from .evals import elovalue, classification, equal, includes
 from .promptChange import uppercase, lowercase, random_uppercase, random_lowercase, random_lowercase_word, random_uppercase_word, synonymous_prompt, grammatical_errors
 import yaml
 import textwrap
 import numpy as np
 from collections import defaultdict
+from dotenv import load_dotenv
+load_dotenv()
+openai.api_key = os.getenv("OPENAI_API_KEY")
 
 # It loads and reads the content of a given YAML file and returns its content as a Python dictionary or list.
 def read_yaml(file_name):
     with open(file_name, 'r') as file:
         content = yaml.safe_load(file)
     return content
 
 def run_evaluation(file):
 
     # Extract the 'yaml_file' attribute from the input 'file' object
     yaml_file_path = os.path.abspath(file)
     # Read the content of the YAML file
     yaml_content = read_yaml(yaml_file_path)
-    # Extract the first key (block_name) from the YAML content
-    block_name = list(yaml_content.keys())[0]
 
     # Extract the 'description', 'test_cases', 'number_of_prompts', 'candidate_model', 'generation_model',
     # 'generation_model_temperature', 'generation_model_max_tokens', and 'method' from the YAML content
-    description = yaml_content[block_name]['description']
-    test_cases = yaml_content[block_name]['test_cases']
-    number_of_prompts = yaml_content[block_name]['number_of_prompts']
-    candidate_model = yaml_content[block_name]['candidate_model']
-    candidate_model_temperature = yaml_content[block_name]['candidate_model_temperature']
-    generation_model = yaml_content[block_name]['generation_model']
-    generation_model_temperature = yaml_content[block_name]['generation_model_temperature']
-    generation_model_max_tokens = yaml_content[block_name]['generation_model_max_tokens']
-    prompt_change = yaml_content[block_name]['prompt_change']
-    method = yaml_content[block_name]['method']
-    iterations = yaml_content[block_name]['iterations']
+    description = yaml_content['test']['description']
+    test_cases = yaml_content['test']['cases']
+    method = yaml_content['test']['method']
+    model_test = yaml_content['test']['model']['name']
+    model_test_temperature = yaml_content['test']['model']['temperature']
+    model_test_max_tokens = yaml_content['test']['model']['max_tokens']
+    prompts_value = yaml_content['prompts']['content']
+    number_of_prompts = yaml_content['prompts']['number']
+    prompt_features = yaml_content['prompts']['features']
+    prompt_change = yaml_content['prompts']['change']
+    model_generation = yaml_content['generation']['model']['name']
+    model_generation_temperature = yaml_content['generation']['model']['temperature']
+    iterations = yaml_content['iterations']['number']
 
     if method == 'elovalue.Elo':
         class_method = elovalue.Elo
     elif method == 'classification.Classification':
         class_method = classification.Classification
     elif method == 'equal.Equal':
         class_method = equal.Equal
     elif method == 'includes.Includes':
         class_method = includes.Includes
 
     # Initialize an object of the class obtained from the 'method'
-    object_class = class_method(description, test_cases, number_of_prompts, generation_model, generation_model_temperature, generation_model_max_tokens, candidate_model, candidate_model_temperature, None)
+    object_class = class_method(description, test_cases, number_of_prompts, model_test, model_test_temperature, model_test_max_tokens, model_generation, model_generation_temperature, None)
     # Checks if the prompts to evaluate already exist and if not, creates them
-    if 'prompts' in yaml_content[block_name]:
-        prompts_value = yaml_content[block_name]['prompts']
-    else:
-        if 'prompt_features' in yaml_content[block_name]:
-            prompt_features = yaml_content[block_name]['prompt_features']
-            prompts_value = generation.generate_candidate_prompts(object_class.system_gen_system_prompt, object_class.test_cases, object_class.description, object_class.candidate_model, object_class.candidate_model_temperature, object_class.number_of_prompts, prompt_features)
+    if prompts_value == []:
+        if prompt_features != 'None':
+            
+            prompts_value = generation.generate_candidate_prompts(object_class.system_gen_system_prompt, object_class.test_cases, object_class.description, object_class.model_generation, object_class.model_generation_temperature, object_class.number_of_prompts, prompt_features)
         else:
-            prompts_value = generation.generate_candidate_prompts(object_class.system_gen_system_prompt, object_class.test_cases, object_class.description, object_class.candidate_model, object_class.candidate_model_temperature, object_class.number_of_prompts)
+            prompts_value = generation.generate_candidate_prompts(object_class.system_gen_system_prompt, object_class.test_cases, object_class.description, object_class.model_generation, object_class.model_generation_temperature, object_class.number_of_prompts)
 
     
-    if prompt_change == 'yes':
-        change = yaml_content[block_name]['change']
-        if change == 'uppercase':
+    if prompt_change != 'None':
+        if prompt_change == 'uppercase':
             prompts_value = uppercase.convert_prompts(prompts_value)
-        elif change == 'lowercase':
+        elif prompt_change == 'lowercase':
             prompts_value = lowercase.convert_prompts(prompts_value)
-        elif change == 'random_uppercase':
+        elif prompt_change == 'random_uppercase':
             prompts_value = random_uppercase.convert_prompts(prompts_value)
-        elif change == 'random_lowercase':
+        elif prompt_change == 'random_lowercase':
             prompts_value = random_lowercase.convert_prompts(prompts_value)
-        elif change == 'random_lowercase_word':
+        elif prompt_change == 'random_lowercase_word':
             prompts_value = random_lowercase_word.convert_prompts(prompts_value)
-        elif change == 'random_uppercase_word':
+        elif prompt_change == 'random_uppercase_word':
             prompts_value = random_uppercase_word.convert_prompts(prompts_value)
-        elif change == 'synonymous_prompt':
+        elif prompt_change == 'synonymous_prompt':
             prompts_value = synonymous_prompt.convert_prompts(prompts_value)
-        elif change == 'grammatical_errors':
+        elif prompt_change == 'grammatical_errors':
             prompts_value = grammatical_errors.convert_prompts(prompts_value)
 
-    evaluable_object = class_method(description, test_cases, number_of_prompts, generation_model, generation_model_temperature, generation_model_max_tokens, candidate_model, candidate_model_temperature, prompts_value)
+    evaluable_object = class_method(description, test_cases, number_of_prompts, model_test, model_test_temperature, model_test_max_tokens, model_generation, model_generation_temperature, prompts_value)
     
     # Evaluate the prompts
     results = evaluable_object.evaluate_optimal_prompt()
-    iterations_prompts = results[1]
-    prompts_to_change = results[1]
 
     yaml_folder = os.path.dirname(file)
     if method == 'elovalue.Elo':
         # Group "elo" values by prompt using a dictionary
         elos_by_prompt = defaultdict(list)
         for item in results[0][number_of_prompts + 1]:
             prompt = item["prompt"]
@@ -110,39 +108,80 @@
         plt.title('Scatter Plot: Elo by Prompt')
         plt.legend()
         plt.show()
         output_plot_path = os.path.join(yaml_folder, "scatter_plot.png")
         plt.savefig(output_plot_path)
         print(f"Scatter plot saved in: {output_plot_path}")
 
-    while iterations > 0:
-        new_prompts = []
-
-        for item in prompts_to_change:
-            prompt_content = item["prompt"]
-            new_prompts.append(prompt_content)
-
-        candidate_prompts = []
-        for best_prompt in new_prompts:
-            candidates = generation.generate_candidate_prompts("Your job is to generate a prompt similar to a prompt you are going to receive. Generate a new one by modifying words or phrases but in such a way that the meaning of the prompt is preserved. What you return has to be a reformulation of what you received and nothing more, no explanation is necessary. Don't return phrases like 'Here are some examples:', just say the prompt", best_prompt, description, candidate_model, candidate_model_temperature, 1, prompt_features=None)
-            candidate_prompts.extend(candidates)
-
-        new_prompts.extend(candidate_prompts)
-
-        evaluable_object = class_method(description, test_cases, 4, generation_model, generation_model_temperature, generation_model_max_tokens, candidate_model, candidate_model_temperature, new_prompts)
-        prompts_to_change = evaluable_object.evaluate_optimal_prompt()[1]
-        iterations_prompts.append(prompts_to_change)
-        iterations = iterations - 1 
-    
     # Full path of the output.json file in the same folder as the YAML
     output_json_path = os.path.join(yaml_folder, "output.json")
     # Convert the result to JSON format and save it to the output.json file
     with open(output_json_path, "w") as json_file:
-        json.dump(results, json_file)
+        json.dump(results[0], json_file)
     print(f"Result saved in: {output_json_path}")
+    old_prompts = results[1]
+    print(old_prompts)
+    number_of_iteration = 1
+    if method != 'elovalue.Elo':
+        while iterations > 0:
+            filename = f'output_iteration_{number_of_iteration}.json'
+            json_file_path = os.path.join(yaml_folder, filename)
+            combine_prompts = []
+            new_results = iteration.iterations(description, test_cases, number_of_prompts - 2, model_test, model_test_temperature, model_test_max_tokens, model_generation, model_generation_temperature, old_prompts, method)
+            with open(json_file_path, 'w') as file:
+                json.dump(new_results[0], file, indent=4)
+            iterations = iterations - 1
+            number_of_iteration = number_of_iteration + 1
+            combine_prompts.append(old_prompts)
+            combine_prompts.append(new_results[1])
+            combined_data = [item for sublist in combine_prompts for item in sublist]
+            sorted_data = sorted(combined_data, key=lambda x: x['rating'], reverse=True)
+            old_prompts = [sorted_data[0], sorted_data[1]]
+    else:
+        while iterations > 0:
+            prompt_contents = [item['prompt'] for item in old_prompts]
+            filename = f'output_iteration_{number_of_iteration}.json'
+            json_file_path = os.path.join(yaml_folder, filename)
+            combine_prompts = []
+            new_results = iteration.iterations(description, test_cases, number_of_prompts - 2, model_test, model_test_temperature, model_test_max_tokens, model_generation, model_generation_temperature, prompt_contents, method)
+            print(new_results[1])
+            with open(json_file_path, 'w') as file:
+                json.dump(new_results[0], file, indent=4)
+
+            elos_by_prompt = defaultdict(list)
+            for item in new_results[0][number_of_prompts + 1]:
+                prompt = item["prompt"]
+                elo = item["elo"]
+                elos_by_prompt[prompt].append(elo)
+
+            # Create a scatter plot
+            for prompt, elos in elos_by_prompt.items():
+                prompt_truncated = textwrap.shorten(prompt, width=20, placeholder="...")
+                x = np.arange(1, len(elos) + 1)
+                y = np.array(elos)
+                x_smooth = np.linspace(x.min(), x.max(), 200)
+                y_smooth = np.interp(x_smooth, x, y)
+                plt.plot(x_smooth, y_smooth, linewidth=1.5, markersize=6, label=prompt_truncated)
+            plt.xlabel('Comparisons')
+            plt.ylabel('Elo')
+            plt.title('Scatter Plot: Elo by Prompt')
+            plt.legend()
+            plt.show()
+            scatter = f'scatter_plot_{number_of_iteration}.png'
+            output_plot_path = os.path.join(yaml_folder, scatter)
+            plt.savefig(output_plot_path)
+            print(f"Scatter plot saved in: {output_plot_path}")
+
+            iterations = iterations - 1
+            number_of_iteration = number_of_iteration + 1
+            old_prompts = new_results[1]
+    filename = f'output_best_prompts_and_results.json'
+    json_file_path = os.path.join(yaml_folder, filename)
+    with open(json_file_path, 'w') as file:
+        json.dump(old_prompts, file, indent=4)
     
 
 def main():
     parser = argparse.ArgumentParser(description="Read YAML file and get key values.")
     parser.add_argument("yaml_file", help="Name of the YAML file to read.")
     args = parser.parse_args()
     run_evaluation(args.yaml_file)
```

### Comparing `lenio-ai-prompt-engineer-1.1.0/cli/promptChange/grammatical_errors.py` & `lenio-ai-prompt-engineer-1.2.0/cli/promptChange/grammatical_errors.py`

 * *Files identical despite different names*

### Comparing `lenio-ai-prompt-engineer-1.1.0/cli/promptChange/synonymous_prompt.py` & `lenio-ai-prompt-engineer-1.2.0/cli/promptChange/synonymous_prompt.py`

 * *Files identical despite different names*

### Comparing `lenio-ai-prompt-engineer-1.1.0/lenio_ai_prompt_engineer.egg-info/SOURCES.txt` & `lenio-ai-prompt-engineer-1.2.0/lenio_ai_prompt_engineer.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 README.md
 setup.py
 cli/__init__.py
 cli/generation.py
+cli/iteration.py
 cli/main.py
 cli/evals/__init__.py
 cli/evals/classification.py
 cli/evals/elovalue.py
 cli/evals/equal.py
 cli/evals/includes.py
 cli/promptChange/__init__.py
```

