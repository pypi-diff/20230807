# Comparing `tmp/regex-inference-0.0.7.tar.gz` & `tmp/regex-inference-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "regex-inference-0.0.7.tar", last modified: Sun Aug  6 10:48:45 2023, max compression
+gzip compressed data, was "regex-inference-0.0.8.tar", last modified: Mon Aug  7 15:37:02 2023, max compression
```

## Comparing `regex-inference-0.0.7.tar` & `regex-inference-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 10:48:45.973094 regex-inference-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-06 10:48:25.000000 regex-inference-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-08-06 10:48:45.973094 regex-inference-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-08-06 10:48:25.000000 regex-inference-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 10:48:45.973094 regex-inference-0.0.7/regex_inference/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-06 10:48:25.000000 regex-inference-0.0.7/regex_inference/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 10:48:45.973094 regex-inference-0.0.7/regex_inference/inference/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-06 10:48:25.000000 regex-inference-0.0.7/regex_inference/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8884 2023-08-06 10:48:25.000000 regex-inference-0.0.7/regex_inference/inference/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-06 10:48:25.000000 regex-inference-0.0.7/regex_inference/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 10:48:45.973094 regex-inference-0.0.7/regex_inference.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-08-06 10:48:45.000000 regex-inference-0.0.7/regex_inference.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-08-06 10:48:45.000000 regex-inference-0.0.7/regex_inference.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 10:48:45.000000 regex-inference-0.0.7/regex_inference.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-08-06 10:48:45.000000 regex-inference-0.0.7/regex_inference.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-06 10:48:45.000000 regex-inference-0.0.7/regex_inference.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 10:48:45.973094 regex-inference-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-08-06 10:48:25.000000 regex-inference-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:37:02.982059 regex-inference-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-07 15:36:43.000000 regex-inference-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-08-07 15:37:02.982059 regex-inference-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-08-07 15:36:43.000000 regex-inference-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:37:02.982059 regex-inference-0.0.8/regex_inference/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-07 15:36:43.000000 regex-inference-0.0.8/regex_inference/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:37:02.982059 regex-inference-0.0.8/regex_inference/inference/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-07 15:36:43.000000 regex-inference-0.0.8/regex_inference/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11089 2023-08-07 15:36:43.000000 regex-inference-0.0.8/regex_inference/inference/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-07 15:36:43.000000 regex-inference-0.0.8/regex_inference/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:37:02.982059 regex-inference-0.0.8/regex_inference.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-08-07 15:37:02.000000 regex-inference-0.0.8/regex_inference.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-08-07 15:37:02.000000 regex-inference-0.0.8/regex_inference.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 15:37:02.000000 regex-inference-0.0.8/regex_inference.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-08-07 15:37:02.000000 regex-inference-0.0.8/regex_inference.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-07 15:37:02.000000 regex-inference-0.0.8/regex_inference.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 15:37:02.982059 regex-inference-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-08-07 15:36:43.000000 regex-inference-0.0.8/setup.py
```

### Comparing `regex-inference-0.0.7/LICENSE` & `regex-inference-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `regex-inference-0.0.7/PKG-INFO` & `regex-inference-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: regex-inference
-Version: 0.0.7
+Version: 0.0.8
 Summary: Regex Inference Engine based on ChatGPT
 Home-page: https://github.com/jeffrey82221/regex_inference
 Author: jeffreylin
 Author-email: jeffrey82221@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `regex-inference-0.0.7/regex_inference/inference/engine.py` & `regex-inference-0.0.8/regex_inference/inference/engine.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,20 @@
+"""
+TODO:
+- [ ] Consider continual inferencing mode: statistics should evaluate on the future cases.
+- [ ] Add LLMChain to fix the regex with low F1 scores.
+"""
+import typing
+from typing import List, Optional, Callable, Any, Dict
+import re
+import os
+import exrex
 from langchain import PromptTemplate
 from langchain.llms import OpenAI
 from langchain import LLMChain
-from typing import List, Optional, Callable, Any
-import re
-import os
 
 
 def make_verbose(func: Callable) -> Callable:
     def warp(*args: Any, **kwargs: Any) -> Any:
         args_str = str(args)
         kwargs_str = str(kwargs)
         if len(args_str) > 30:
@@ -34,48 +41,90 @@
             model='text-davinci-003',  # https://platform.openai.com/docs/models/gpt-3-5
             client='regex_inference'
         )
         self._mismatch_tolerance = mismatch_tolerance
         self._max_iteration = max_iteration
         self._simpify_regex = simpify_regex
         if verbose:
-            self.run = make_verbose(self.run)  # type: ignore
-            self.filter_mismatch = make_verbose(  # type: ignore
-                self.filter_mismatch)  # type: ignore
-            self._run = make_verbose(self._run)  # type: ignore
-            self._run_simplify_regex = make_verbose(  # type: ignore
-                self._run_simplify_regex)  # type: ignore
-            self._run_alter_regex = make_verbose(  # type: ignore
-                self._run_alter_regex)  # type: ignore
-            self._run_new_inference = make_verbose(  # type: ignore
-                self._run_new_inference)  # type: ignore
+            self._make_verbose()
         self._setup_lang_chains()
 
-    def run(self, patterns: List[str], regex: Optional[str] = None) -> str:
+    @typing.no_type_check
+    def _make_verbose(self):
+        self.run = make_verbose(self.run)
+        self._run_simplify_regex = make_verbose(
+            self._run_simplify_regex)
+        self._run_alter_regex = make_verbose(
+            self._run_alter_regex)
+        self._run_new_inference = make_verbose(
+            self._run_new_inference)
+
+    def run(self, patterns: List[str]) -> str:
+        regex_list = self.get_regex_sequence(patterns)
+        return Engine.merge_regex_sequence(regex_list)
+
+    @staticmethod
+    @typing.no_type_check
+    def get_statistics(
+            patterns: List[str], regex_list: List[str]) -> List[Dict]:
+        """
+        Args:
+            patterns: list of strings to be inferenced
+            regex_list: the regex sequenced inferenced by ChatGPT.
+        Returns:
+            results (list of dict):
+                result (dict with fields):
+                    - regex
+                    - n_sim_patterns (number of strings matching the regex)
+                    - n_matched_patterns
+        """
+        total_cnt = len(patterns)
+        results: List[Dict] = []
+        previous_matched: List[str] = []
+        for i in range(len(regex_list)):
+            result = dict()
+            result['regex'] = regex_list[i]
+            result['n_sim_patterns'] = exrex.count(result['regex'])
+            matched = Engine.filter_match(result['regex'], patterns)
+            result['n_matched_patterns'] = len(
+                set(matched) - set(previous_matched))
+            result['n_target_matching'] = total_cnt
+            total_cnt -= result['n_matched_patterns']
+            previous_matched.extend(matched)
+            previous_matched = list(set(previous_matched))
+            result['precision'] = result['n_matched_patterns'] / \
+                result['n_sim_patterns']
+            result['recall'] = result['n_matched_patterns'] / \
+                result['n_target_matching']
+            if result['precision'] == 0. or result['recall'] == 0.:
+                result['f1'] = 0.
+            else:
+                result['f1'] = 2. / \
+                    (1. / result['precision'] + 1. / result['recall'])
+            results.append(result)
+        return results
+
+    def get_regex_sequence(self, patterns: List[str]) -> List[str]:
         assert len(
             patterns) > 0, '`patterns` input to `run` should no be an empty list'
-        if regex is None:
-            regex = self._run(patterns)
-        if self._simpify_regex:
-            regex = self._run_simplify_regex(regex, patterns)
-        failed_patterns = self.filter_mismatch(regex, patterns)
-        while failed_patterns:
-            failed_regex = self._run(failed_patterns)
-            regex = f'{regex}|{failed_regex}'
-            if self._simpify_regex:
-                regex = self._run_simplify_regex(regex, patterns)
-            failed_patterns = self.filter_mismatch(regex, patterns)
-        return regex
-
-    def _run(self, patterns: List[str], regex: Optional[str] = None) -> str:
-        if regex:
-            regex_result = self._run_alter_regex(regex, patterns)
-        else:
-            regex_result = self._run_new_inference(patterns)
-        return regex_result
+        regex_list = [self._run_new_inference(patterns)]
+        mismatched_patterns = Engine.filter_mismatch(
+            Engine.merge_regex_sequence(regex_list),
+            patterns
+        )
+        while mismatched_patterns:
+            regex = self._run_new_inference(mismatched_patterns)
+            regex_list.append(regex)
+            mismatched_patterns = Engine.filter_mismatch(
+                Engine.merge_regex_sequence(regex_list), patterns)
+        return regex_list
+
+    @staticmethod
+    def merge_regex_sequence(regex_list: List[str]) -> str:
+        return '|'.join(map(lambda x: f'({x})', regex_list))
 
     @staticmethod
     def _convert_patterns_to_prompt(patterns: List[str]) -> str:
         return '\n'.join(map(lambda x: f'"{x}"', patterns))
 
     def _run_alter_regex(self, regex: str, patterns: List[str]) -> str:
         for _ in range(self._max_iteration):
@@ -115,16 +164,30 @@
                 pass
         return result
 
     def explain(self, regex: str) -> None:
         result = self._regex_explain_chain.run(regex)
         print(result)
 
+    @staticmethod
+    def filter_match(regex: str, patterns: List[str]) -> List[str]:
+        try:
+            re_com = re.compile(regex)
+        except BaseException as e:
+            print('syntax error in result_regex:', regex)
+            raise e
+        result = list(
+            filter(
+                lambda x: re_com.fullmatch(x) is not None,
+                patterns))
+        return result
+
+    @staticmethod
     def filter_mismatch(
-            self, regex: str, patterns: List[str]) -> List[str]:
+            regex: str, patterns: List[str]) -> List[str]:
         try:
             re_com = re.compile(regex)
         except BaseException as e:
             print('syntax error in result_regex:', regex)
             raise e
         result = list(filter(lambda x: re_com.fullmatch(x) is None, patterns))
         return result
@@ -147,19 +210,19 @@
             llm=self._openai_llm
         )
 
     @property
     def new_inference_prompt(self) -> PromptTemplate:
         template = """Question: Show me the best and shortest regex that can fully match the strings that I provide to you.
 Note that:
-*. The regex should be made more generalized (e.g., use \\d to represent digit rather than using [0-9]) and shorter than the original regex.
+*. The regex should be as short as possible.
 *. Match sure the resulting regex does not have syntax error.
-*. The character count of the resulting regex should not be larger than 30.
-*. Use \\d to replace [0-9].
-*. Try to focus more on the global pattern rather than the local patterns.
+*. The regex should full match as many strings as possible.
+*. The regex should not match strings that is not provided.
+*. The number of string combinations matching the resulting regex should be as smaller than the number of target strings provided.
 Now, each instance of the strings that should be fully matched is provided line-by-line and wrapped by double quotes as follows:
 {strings}
 
 Note that:
 1. The double quote is not part of the string instance. Ignore the double quote during inferencing the regex.
 2. Provide the resulting regex without wrapping it in quote
 
@@ -170,17 +233,17 @@
         )
         return prompt
 
     @property
     def alter_regex_prompt(self) -> PromptTemplate:
         template = """Question: Alter the regex "{regex}" such that the following requirements is matched:
 *. The pattern fully match the regex still fully match the regex.
-*. The strings that I provide to you also fully match.
-*. The character count of the resulting regex should not be larger than 30.
-*. The regex should be made more generalized (e.g., use \\d to represent digit rather than using [0-9]) and shorter than the original regex.
+*. The regex should full match as many strings provided as possible.
+*. The regex should be as short as possible.
+*. The regex should not match strings that is not provided except for those full match the original regex.
 Now, each instance of the strings is provided line-by-line and wrapped by double quotes as follows:
 {strings}
 
 Note that:
 1. The double quote is not part of the string instance. Ignore the double quote during inferencing the regex.
 2. Provide the resulting regex without wrapping it in quote
 
@@ -191,18 +254,19 @@
         )
         return prompt
 
     @property
     def simplify_regex_prompt(self) -> PromptTemplate:
         template = """
 Please revise the regex "{regex}"
-such that
-*. It becomes as short as possible.
-*. It still fully match all the strings full matched the original regex
-*. It still fully match each of the strings I provided to you.
+such that the following constraint start with *. can be met:
+*. The original regex consists of multiple regex seperated by "|". Try to combine the similar regex.
+*. After combine, the resulting regex should be as short as possible.
+*. The revised regex should still fully match all the strings full matched the original regex
+*. The revised regex should still fully match each of the strings I provided to you.
 Now, each instance of the strings is provided line-by-line and wrapped by double quotes as follows:
 {strings}
 
 
 Note that:
 1. The double quote is not part of the string instance. Ignore the double quote during inferencing the regex.
 2. Provide the resulting regex without wrapping it in quote
```

### Comparing `regex-inference-0.0.7/regex_inference.egg-info/PKG-INFO` & `regex-inference-0.0.8/regex_inference.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: regex-inference
-Version: 0.0.7
+Version: 0.0.8
 Summary: Regex Inference Engine based on ChatGPT
 Home-page: https://github.com/jeffrey82221/regex_inference
 Author: jeffreylin
 Author-email: jeffrey82221@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `regex-inference-0.0.7/setup.py` & `regex-inference-0.0.8/setup.py`

 * *Files identical despite different names*

