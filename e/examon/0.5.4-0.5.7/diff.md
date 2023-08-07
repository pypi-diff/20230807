# Comparing `tmp/examon-0.5.4.tar.gz` & `tmp/examon-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "examon-0.5.4.tar", max compression
+gzip compressed data, was "examon-0.5.7.tar", max compression
```

## Comparing `examon-0.5.4.tar` & `examon-0.5.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      820 2023-07-18 13:39:43.297716 examon-0.5.4/README.md
--rwxr-xr-x   0        0        0        0 2023-01-06 12:36:14.367207 examon-0.5.4/examon/__init__.py
--rwxr-xr-x   0        0        0       24 2023-01-28 12:15:25.205762 examon-0.5.4/examon/lib/__init__.py
--rw-r--r--   0        0        0      536 2023-07-27 13:57:45.119515 examon-0.5.4/examon/lib/examon_config.py
--rw-r--r--   0        0        0     1751 2023-07-15 11:53:35.970348 examon-0.5.4/examon/lib/examon_engine.py
--rw-r--r--   0        0        0     1541 2023-07-15 12:06:34.065368 examon-0.5.4/examon/lib/examon_engine_factory.py
--rw-r--r--   0        0        0     2382 2023-07-27 13:35:59.867607 examon-0.5.4/examon/lib/package_manager.py
--rw-r--r--   0        0        0      820 2023-07-27 13:35:59.872649 examon-0.5.4/examon/lib/pip_installer.py
--rw-r--r--   0        0        0     1116 2023-07-28 14:55:00.396350 examon-0.5.4/examon/lib/results_manager.py
--rwxr-xr-x   0        0        0      606 2023-07-15 11:48:57.713181 examon-0.5.4/examon/lib/stats.py
--rw-r--r--   0        0        0      367 2023-07-15 11:53:35.880898 examon-0.5.4/examon/lib/streak_tracker.py
--rwxr-xr-x   0        0        0       99 2023-07-12 20:13:15.318911 examon-0.5.4/examon/main.py
--rwxr-xr-x   0        0        0        0 2023-01-20 16:32:50.288125 examon-0.5.4/examon/view/__init__.py
--rw-r--r--   0        0        0        0 2023-07-09 19:56:53.890002 examon-0.5.4/examon/view/cli/__init__.py
--rwxr-xr-x   0        0        0     1918 2023-07-25 06:03:38.544248 examon-0.5.4/examon/view/cli/examon_arg_parse.py
--rw-r--r--   0        0        0     2600 2023-07-29 16:53:54.452624 examon-0.5.4/examon/view/cli/interactive.py
--rwxr-xr-x   0        0        0      946 2023-07-23 10:24:31.594694 examon-0.5.4/examon/view/cli/main.py
--rw-r--r--   0        0        0      301 2023-07-15 12:15:59.351678 examon-0.5.4/examon/view/cli/overview.py
--rw-r--r--   0        0        0     1949 2023-07-27 13:41:27.906806 examon-0.5.4/examon/view/cli/package.py
--rw-r--r--   0        0        0     1903 2023-07-28 14:55:00.383978 examon-0.5.4/examon/view/cli/runner.py
--rwxr-xr-x   0        0        0      862 2023-07-15 11:53:35.671820 examon-0.5.4/examon/view/formatter_options.py
--rwxr-xr-x   0        0        0        0 2023-01-22 21:43:58.660247 examon-0.5.4/examon/view/input/__init__.py
--rwxr-xr-x   0        0        0      706 2023-07-08 09:55:03.400755 examon-0.5.4/examon/view/input/answer_question.py
--rwxr-xr-x   0        0        0        0 2023-01-22 21:44:07.847782 examon-0.5.4/examon/view/output/__init__.py
--rwxr-xr-x   0        0        0     2001 2023-07-29 20:47:42.245738 examon-0.5.4/examon/view/output/question.py
--rwxr-xr-x   0        0        0      546 2023-07-30 18:42:22.446931 examon-0.5.4/pyproject.toml
--rw-r--r--   0        0        0     1433 1970-01-01 00:00:00.000000 examon-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0      820 2023-07-18 13:39:43.297716 examon-0.5.7/README.md
+-rwxr-xr-x   0        0        0        0 2023-01-06 12:36:14.367207 examon-0.5.7/examon/__init__.py
+-rwxr-xr-x   0        0        0       24 2023-01-28 12:15:25.205762 examon-0.5.7/examon/lib/__init__.py
+-rw-r--r--   0        0        0      536 2023-07-27 13:57:45.119515 examon-0.5.7/examon/lib/examon_config.py
+-rw-r--r--   0        0        0     1758 2023-08-06 15:00:45.298085 examon-0.5.7/examon/lib/examon_engine.py
+-rw-r--r--   0        0        0     1557 2023-08-07 05:25:57.528851 examon-0.5.7/examon/lib/examon_engine_factory.py
+-rw-r--r--   0        0        0     2382 2023-07-27 13:35:59.867607 examon-0.5.7/examon/lib/package_manager.py
+-rw-r--r--   0        0        0      926 2023-08-07 15:52:03.956871 examon-0.5.7/examon/lib/pip_installer.py
+-rw-r--r--   0        0        0     1116 2023-07-28 14:55:00.396350 examon-0.5.7/examon/lib/results_manager.py
+-rwxr-xr-x   0        0        0      607 2023-08-06 16:04:46.171819 examon-0.5.7/examon/lib/stats.py
+-rw-r--r--   0        0        0      367 2023-07-15 11:53:35.880898 examon-0.5.7/examon/lib/streak_tracker.py
+-rwxr-xr-x   0        0        0       99 2023-07-12 20:13:15.318911 examon-0.5.7/examon/main.py
+-rwxr-xr-x   0        0        0        0 2023-01-20 16:32:50.288125 examon-0.5.7/examon/view/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-09 19:56:53.890002 examon-0.5.7/examon/view/cli/__init__.py
+-rwxr-xr-x   0        0        0     1937 2023-08-07 05:51:54.677996 examon-0.5.7/examon/view/cli/examon_arg_parse.py
+-rw-r--r--   0        0        0     2497 2023-07-30 19:28:29.637561 examon-0.5.7/examon/view/cli/interactive.py
+-rwxr-xr-x   0        0        0      946 2023-07-23 10:24:31.594694 examon-0.5.7/examon/view/cli/main.py
+-rw-r--r--   0        0        0      558 2023-08-06 16:10:43.706479 examon-0.5.7/examon/view/cli/overview.py
+-rw-r--r--   0        0        0     1949 2023-08-06 15:34:38.961002 examon-0.5.7/examon/view/cli/package.py
+-rw-r--r--   0        0        0     1956 2023-08-07 06:29:53.687811 examon-0.5.7/examon/view/cli/runner.py
+-rwxr-xr-x   0        0        0      862 2023-07-15 11:53:35.671820 examon-0.5.7/examon/view/formatter_options.py
+-rwxr-xr-x   0        0        0        0 2023-01-22 21:43:58.660247 examon-0.5.7/examon/view/input/__init__.py
+-rwxr-xr-x   0        0        0      706 2023-07-08 09:55:03.400755 examon-0.5.7/examon/view/input/answer_question.py
+-rwxr-xr-x   0        0        0        0 2023-01-22 21:44:07.847782 examon-0.5.7/examon/view/output/__init__.py
+-rwxr-xr-x   0        0        0     2003 2023-08-06 15:13:46.381357 examon-0.5.7/examon/view/output/question.py
+-rwxr-xr-x   0        0        0      554 2023-08-07 18:23:15.054576 examon-0.5.7/pyproject.toml
+-rw-r--r--   0        0        0     1427 1970-01-01 00:00:00.000000 examon-0.5.7/PKG-INFO
```

### Comparing `examon-0.5.4/README.md` & `examon-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `examon-0.5.4/examon/lib/examon_config.py` & `examon-0.5.7/examon/lib/examon_config.py`

 * *Files identical despite different names*

### Comparing `examon-0.5.4/examon/lib/examon_engine.py` & `examon-0.5.7/examon/lib/examon_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from examon_core.question_response import QuestionResponse
+from examon_core.models.question_response import QuestionResponse
 from examon.lib.streak_tracker import StreakTracker
 
 
 class ExamonEngine:
     def __init__(self, questions=None,
                  stats_outputter=None,
                  view_mappings=None):
```

### Comparing `examon-0.5.4/examon/lib/examon_engine_factory.py` & `examon-0.5.7/examon/lib/examon_engine_factory.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-from examon_core.question import BaseQuestion, ExpectedResultQuestion, \
+from examon_core.models.question import BaseQuestion, MultiChoiceQuestion, \
     InputParameterQuestion
 from examon_core.examon_item_registry import ExamonItemRegistry
 
-from examon.view.input.answer_question import AnswerInputter,\
+from examon.view.input.answer_question import AnswerInputter, \
     FreeTextAnswerInputter
-from examon.view.output.question import ExpectedResultQuestionOutputter, \
+from examon.view.output.question import MultiChoiceQuestionOutputter, \
     InputParameterQuestionOutputter, FreeTextQuestionOutputter
 from .stats import Stats
 from .examon_engine import ExamonEngine
 
 
 class ExamonEngineFactory:
     @staticmethod
-    def build(tag, formatter_class, auto_answer=None):
+    def build(examon_filter, formatter_class, auto_answer=None):
         def fetch_inputter(enabled, inputter):
             return enabled if enabled else inputter
 
-        registry = ExamonItemRegistry.registry(tag)
+        registry = ExamonItemRegistry.registry(examon_filter)
         view_mappings = {
-            ExpectedResultQuestion.__name__: {
-                'outputter': ExpectedResultQuestionOutputter(formatter_class),
+            MultiChoiceQuestion.__name__: {
+                'outputter': MultiChoiceQuestionOutputter(formatter_class),
                 'inputter': fetch_inputter(auto_answer, AnswerInputter())
             },
             InputParameterQuestion.__name__: {
                 'outputter': InputParameterQuestionOutputter(formatter_class),
                 'inputter': fetch_inputter(auto_answer, AnswerInputter())
             }, BaseQuestion.__name__: {
                 'outputter': FreeTextQuestionOutputter(formatter_class),
```

### Comparing `examon-0.5.4/examon/lib/package_manager.py` & `examon-0.5.7/examon/lib/package_manager.py`

 * *Files identical despite different names*

### Comparing `examon-0.5.4/examon/lib/pip_installer.py` & `examon-0.5.7/examon/lib/pip_installer.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 import subprocess
 import sys
 import importlib.util
 import logging
+import os.path
+import os
+
+from .examon_config import DEFAULT_FOLDER
 
 
 class PipInstaller:
     @staticmethod
     def install(packages):
         logging.info(f"installing {len(packages)} repos")
         for package in packages:
-            with open('pip_install.log', "w") as outfile:
+            with open(f'{os.path.expanduser(DEFAULT_FOLDER)}/pip_install.log', "w") as outfile:
                 cmd = [sys.executable, "-m", "pip", "install", package['name'], '--upgrade']
                 logging.debug(cmd)
                 subprocess.run(cmd, stdout=outfile)
 
     @staticmethod
     def is_package_installed(package_name):
         if importlib.util.find_spec(package_name) is None:
```

### Comparing `examon-0.5.4/examon/lib/results_manager.py` & `examon-0.5.7/examon/lib/results_manager.py`

 * *Files identical despite different names*

### Comparing `examon-0.5.4/examon/lib/stats.py` & `examon-0.5.7/examon/lib/stats.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from collections import Counter
 
 
 class Stats:
     @staticmethod
     def calc_stats(questions):
+
         return {
             'total_questions': len(questions),
             'tags_summary': Stats.uniq_tags(questions),
             'tags': Stats.tag_count(questions),
         }
 
     @staticmethod
```

### Comparing `examon-0.5.4/examon/view/cli/examon_arg_parse.py` & `examon-0.5.7/examon/view/cli/examon_arg_parse.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,22 +29,22 @@
         run_subparser = subparsers.add_parser('run', help='Run the quiz')
         run_subparser.add_argument("--formatter", help='')
         run_subparser.add_argument("--tag", help='')
         run_subparser.add_argument("--tags", help='')
         run_subparser.add_argument("--tags-mandatory", help='')
         run_subparser.add_argument("--max-questions", help='')
         run_subparser.add_argument("--file", help='')
+        run_subparser.add_argument("--difficulty", help='')
 
         subparsers.add_parser('tag',
                               help='Tag Information',
                               aliases=['tags'])
 
         subparsers.add_parser('overview',
-                              help='Tag Information',
-                              aliases=['tags'])
+                              help='Question Bank Overview')
 
 
 class ExamonArgParseFactory:
     @staticmethod
     def build():
         parser = argparse.ArgumentParser(prog='Examon CLI')
         cli_args = ExamonArgParse(parser, FormatterOptions()).parse()
```

### Comparing `examon-0.5.4/examon/view/cli/interactive.py` & `examon-0.5.7/examon/view/cli/interactive.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,16 +13,15 @@
               |-   . , ,-: ;-.-. ,-. ;-. 
               |     X  | | | | | | | | | 
               `--' ' ` `-` ' ' ' `-' ' '
         """
 
 
 class InteractiveCLI:
-    DEFAULT_PACKAGES = ['examon_beginners_package', 'examon_easy_package',
-                        'examon_intermediate_package', 'examon_pcap_package']
+    DEFAULT_PACKAGES = ['examon_beginners_package']
 
     @staticmethod
     def process_command():
         print(ASCII_ART)
         manager = PackageManager()
         for package in InteractiveCLI.DEFAULT_PACKAGES:
             manager.add(package)
@@ -38,15 +37,15 @@
 
         for active in [*terminal_menu.chosen_menu_entries]:
             manager.add(active)
             manager.add_active(active)
         manager.persist()
 
         manager.load()
-        # PipInstaller.install(manager.packages)
+        PipInstaller.install(manager.packages)
         PipInstaller.import_packages(manager.active_packages)
 
         available_tags = ExamonItemRegistry.unique_tags()
         all_tags_filter = None
         if len(available_tags) > 0:
             terminal_menu = TerminalMenu(
                 available_tags,
```

### Comparing `examon-0.5.4/examon/view/cli/main.py` & `examon-0.5.7/examon/view/cli/main.py`

 * *Files identical despite different names*

### Comparing `examon-0.5.4/examon/view/cli/package.py` & `examon-0.5.7/examon/view/cli/package.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 from examon.lib.pip_installer import PipInstaller
 
 class PackageManagerCli:
     @staticmethod
     def process_command(cli_args):
         package_manager = PackageManager()
         if cli_args.sub_command == 'add':
-            package_manager.add(cli_args.name, cli_args.pip_url)
             package_manager.load()
+            package_manager.add(cli_args.name, cli_args.pip_url)
             package_manager.persist()
         elif cli_args.sub_command == 'remove':
-            package_manager.remove(cli_args.name)
             package_manager.load()
+            package_manager.remove(cli_args.name)
             package_manager.remove_active(cli_args.name)
             package_manager.persist()
         elif cli_args.sub_command == 'add_active':
-            package_manager.add_active(cli_args.name)
             package_manager.load()
+            package_manager.add_active(cli_args.name)
             package_manager.persist()
         elif cli_args.sub_command == 'remove_active':
-            package_manager.remove_active(cli_args.name)
             package_manager.load()
+            package_manager.remove_active(cli_args.name)
             package_manager.persist()
         elif cli_args.sub_command == 'install':
             package_manager.load()
             PipInstaller.install(package_manager.packages)
         elif cli_args.sub_command == 'list':
             package_manager.load()
             print('')
```

### Comparing `examon-0.5.4/examon/view/cli/runner.py` & `examon-0.5.7/examon/view/cli/runner.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,14 +16,15 @@
         if questions is not None:
             questions = int(questions)
 
         item_registry_filter = ItemRegistryFilter(
             tags_any=RunnerCli.get_tags(cli_args),
             tags_all=RunnerCli.tags_as_array(cli_args.tags_mandatory),
             max_questions=questions,
+            difficulty_category=cli_args.difficulty,
         )
         examon_engine = ExamonEngineFactory.build(
             item_registry_filter, FormatterOptions()[
                 cli_args.formatter])
         examon_engine.run()
 
         if cli_args.file:
```

### Comparing `examon-0.5.4/examon/view/formatter_options.py` & `examon-0.5.7/examon/view/formatter_options.py`

 * *Files identical despite different names*

### Comparing `examon-0.5.4/examon/view/input/answer_question.py` & `examon-0.5.7/examon/view/input/answer_question.py`

 * *Files identical despite different names*

### Comparing `examon-0.5.4/examon/view/output/question.py` & `examon-0.5.7/examon/view/output/question.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 class BaseQuestionOutputter():
     def __init__(self, formatter_class):
         self.formatter_class = formatter_class
 
     def print_metrics(self, question):
-        print(f'Difficulty: {question.metrics.calc_difficulty()}')
+        print(f'Difficulty: {question.metrics.categorised_difficulty}')
 
     def present_summary(self, summary):
         os.system('clear')
         print(f'You are: {summary}')
 
     def present_question(self, question):
         print(
@@ -41,15 +41,15 @@
         print(test)
         print(question.return_value)
         print('')
         print('')
         self.display_print_logs(question)
 
 
-class ExpectedResultQuestionOutputter(BaseQuestionOutputter):
+class MultiChoiceQuestionOutputter(BaseQuestionOutputter):
     def present_question(self, question):
         print('')
         self.print_metrics(question)
         print('What is the result of the last print statement?')
         print('')
         super().present_question(question)
         print('')
```

### Comparing `examon-0.5.4/pyproject.toml` & `examon-0.5.7/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "examon"
-version = "0.5.4"
+version = "0.5.7"
 description = ""
 authors = ["Jarrod Folino <jdfolino@icloud.com>"]
 readme = "README.md"
 packages = [{include = "examon"}]
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = ">=3.9,<3.12"
 pygments = "^2.13.0"
 inquirer = "^3.1.1"
-simple-term-menu = "^1.6.1"
-examon-core = "1.1.0"
+simple-term-menu = "1.6.1"
+examon-core = ">=1.2.1"
 dataclasses-serialization = "^1.3.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "7.2.1"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `examon-0.5.4/PKG-INFO` & `examon-0.5.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: examon
-Version: 0.5.4
+Version: 0.5.7
 Summary: 
 Author: Jarrod Folino
 Author-email: jdfolino@icloud.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: dataclasses-serialization (>=1.3.1,<2.0.0)
-Requires-Dist: examon-core (==1.1.0)
+Requires-Dist: examon-core (>=1.2.1)
 Requires-Dist: inquirer (>=3.1.1,<4.0.0)
 Requires-Dist: pygments (>=2.13.0,<3.0.0)
-Requires-Dist: simple-term-menu (>=1.6.1,<2.0.0)
+Requires-Dist: simple-term-menu (==1.6.1)
 Description-Content-Type: text/markdown
 
 # ExamOn
 
 ## Prequisites
 
 * Python 3.9.15 or later
```

