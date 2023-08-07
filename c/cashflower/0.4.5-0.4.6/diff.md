# Comparing `tmp/cashflower-0.4.5.tar.gz` & `tmp/cashflower-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cashflower-0.4.5.tar", last modified: Sun Jul 16 13:53:05 2023, max compression
+gzip compressed data, was "cashflower-0.4.6.tar", last modified: Mon Aug  7 15:11:54 2023, max compression
```

## Comparing `cashflower-0.4.5.tar` & `cashflower-0.4.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:53:05.973244 cashflower-0.4.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-16 13:52:54.000000 cashflower-0.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-16 13:52:54.000000 cashflower-0.4.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-07-16 13:53:05.973244 cashflower-0.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-16 13:52:54.000000 cashflower-0.4.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:53:05.973244 cashflower-0.4.5/cashflower/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-16 13:52:54.000000 cashflower-0.4.5/cashflower/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14933 2023-07-16 13:52:54.000000 cashflower-0.4.5/cashflower/cashflow.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-16 13:52:54.000000 cashflower-0.4.5/cashflower/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-07-16 13:52:54.000000 cashflower-0.4.5/cashflower/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:53:05.973244 cashflower-0.4.5/cashflower/model_tpl/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-16 13:52:54.000000 cashflower-0.4.5/cashflower/model_tpl/input.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-16 13:52:54.000000 cashflower-0.4.5/cashflower/model_tpl/model.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-16 13:52:54.000000 cashflower-0.4.5/cashflower/model_tpl/run.py-tpl
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-16 13:52:54.000000 cashflower-0.4.5/cashflower/model_tpl/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     7753 2023-07-16 13:52:54.000000 cashflower-0.4.5/cashflower/start.py
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-16 13:52:54.000000 cashflower-0.4.5/cashflower/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:53:05.973244 cashflower-0.4.5/cashflower.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-07-16 13:53:05.000000 cashflower-0.4.5/cashflower.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-16 13:53:05.000000 cashflower-0.4.5/cashflower.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 13:53:05.000000 cashflower-0.4.5/cashflower.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-16 13:53:05.000000 cashflower-0.4.5/cashflower.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-16 13:53:05.000000 cashflower-0.4.5/cashflower.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 13:53:05.973244 cashflower-0.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-16 13:52:54.000000 cashflower-0.4.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:53:05.973244 cashflower-0.4.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-07-16 13:52:54.000000 cashflower-0.4.5/tests/test_cashflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-16 13:52:54.000000 cashflower-0.4.5/tests/test_start.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-07-16 13:52:54.000000 cashflower-0.4.5/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:11:54.218541 cashflower-0.4.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-08-07 15:11:42.000000 cashflower-0.4.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-07 15:11:42.000000 cashflower-0.4.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-08-07 15:11:54.218541 cashflower-0.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-08-07 15:11:42.000000 cashflower-0.4.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:11:54.218541 cashflower-0.4.6/cashflower/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-08-07 15:11:42.000000 cashflower-0.4.6/cashflower/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12556 2023-08-07 15:11:42.000000 cashflower-0.4.6/cashflower/cashflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-07 15:11:42.000000 cashflower-0.4.6/cashflower/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-08-07 15:11:42.000000 cashflower-0.4.6/cashflower/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:11:54.218541 cashflower-0.4.6/cashflower/model_tpl/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-08-07 15:11:42.000000 cashflower-0.4.6/cashflower/model_tpl/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-08-07 15:11:42.000000 cashflower-0.4.6/cashflower/model_tpl/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-08-07 15:11:42.000000 cashflower-0.4.6/cashflower/model_tpl/run.py-tpl
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-08-07 15:11:42.000000 cashflower-0.4.6/cashflower/model_tpl/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10011 2023-08-07 15:11:42.000000 cashflower-0.4.6/cashflower/start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-08-07 15:11:42.000000 cashflower-0.4.6/cashflower/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:11:54.218541 cashflower-0.4.6/cashflower.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-08-07 15:11:54.000000 cashflower-0.4.6/cashflower.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-08-07 15:11:54.000000 cashflower-0.4.6/cashflower.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 15:11:54.000000 cashflower-0.4.6/cashflower.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-07 15:11:54.000000 cashflower-0.4.6/cashflower.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-07 15:11:54.000000 cashflower-0.4.6/cashflower.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 15:11:54.218541 cashflower-0.4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-08-07 15:11:42.000000 cashflower-0.4.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:11:54.218541 cashflower-0.4.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-08-07 15:11:42.000000 cashflower-0.4.6/tests/test_cashflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-08-07 15:11:42.000000 cashflower-0.4.6/tests/test_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-08-07 15:11:42.000000 cashflower-0.4.6/tests/test_utils.py
```

### Comparing `cashflower-0.4.5/LICENSE` & `cashflower-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cashflower-0.4.5/PKG-INFO` & `cashflower-0.4.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cashflower
-Version: 0.4.5
+Version: 0.4.6
 Summary: Framework for actuarial cash flow models
 Home-page: https://github.com/acturtle/cashflower
 Author: Zuzanna Chmielewska
 Project-URL: Source, https://github.com/acturtle/cashflower
 Project-URL: Tracker, https://github.com/acturtle/cashflower/issues
 Project-URL: Documentation, https://cashflower.acturtle.com
 Requires-Python: >=3.9
```

### Comparing `cashflower-0.4.5/README.md` & `cashflower-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `cashflower-0.4.5/cashflower/cashflow.py` & `cashflower-0.4.6/cashflower/cashflow.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 import functools
-import itertools
-import networkx as nx
 import time
 import pandas as pd
 
 from .error import CashflowModelError
 from .utils import get_object_by_name, print_log, split_to_ranges, updt
-from .graph import get_calc_direction, get_calls, get_predecessors
 
 
 def variable(repeat=None):
     """Decorator"""
     def wrapper(func):
         # Variable must have parameter 't' or no parameters at all
         if func.__code__.co_argcount > 1:
@@ -237,65 +234,14 @@
         self.output = None
 
     def run(self, part=None):
         """Orchestrate all steps of the cash flow model run."""
         one_core = part == 0 or part is None  # single or first part
         print_log(f"Building model '{self.name}'", one_core)
 
-        # Get variables' calls
-        for variable in self.variables:
-            variable.calls = get_calls(variable, self.variables)
-
-        # Create directed graph for all variables
-        DG = nx.DiGraph()
-        for variable in self.variables:
-            DG.add_node(variable)
-            for predecessor in variable.calls:
-                DG.add_edge(predecessor, variable)
-
-        # Draw graph
-        # nx.draw(DG, with_labels=True, font_weight='bold')
-        # plt.show()
-
-        # Set calc_order in variables
-        calc_order = 0
-        while DG.nodes:
-            nodes_without_predecessors = [node for node in DG.nodes if len(list(DG.predecessors(node))) == 0]
-            if len(nodes_without_predecessors) > 0:
-                for node in nodes_without_predecessors:
-                    calc_order += 1
-                    node.calc_order = calc_order
-                DG.remove_nodes_from(nodes_without_predecessors)
-            else:  # it's a cycle
-                cycles = list(nx.simple_cycles(DG))
-                cycles_without_predecessors = [c for c in cycles if len(get_predecessors(c[0], DG)) == len(c)]
-
-                if len(cycles_without_predecessors) == 0:
-                    big_cycle = list(set(list(itertools.chain(*cycles))))
-                    cycles_without_predecessors = [big_cycle]
-
-                for cycle_without_predecessors in cycles_without_predecessors:
-                    calc_order += 1
-                    for node in cycle_without_predecessors:
-                        node.calc_order = calc_order
-                        node.cycle = True
-                    DG.remove_nodes_from(cycle_without_predecessors)
-
-        # Sort variables for calculation order
-        self.variables = sorted(self.variables, key=lambda x: (x.calc_order, x.name))
-
-        # Get calc_direction of calculation
-        max_calc_order = self.variables[-1].calc_order
-        for calc_order in range(1, max_calc_order+1):
-            # Either a single variable or a cycle
-            variables = [variable for variable in self.variables if variable.calc_order == calc_order]
-            calc_direction = get_calc_direction(variables)
-            for variable in variables:
-                variable.calc_direction = calc_direction
-
         # Iterate over model points
         main = get_object_by_name(self.model_point_sets, "main")
         print_log(f"Total number of model points: {main.data.shape[0]}", one_core)
         if one_core and self.settings["MULTIPROCESSING"]:
             if len(main) > self.cpu_count:
                 print_log(f"Multiprocessing on {self.cpu_count} cores")
                 print_log(f"Calculation of ca. {len(main) // self.cpu_count} model points per core")
```

### Comparing `cashflower-0.4.5/cashflower/graph.py` & `cashflower-0.4.6/cashflower/graph.py`

 * *Files identical despite different names*

### Comparing `cashflower-0.4.5/cashflower/utils.py` & `cashflower-0.4.6/cashflower/utils.py`

 * *Files identical despite different names*

### Comparing `cashflower-0.4.5/cashflower.egg-info/PKG-INFO` & `cashflower-0.4.6/cashflower.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cashflower
-Version: 0.4.5
+Version: 0.4.6
 Summary: Framework for actuarial cash flow models
 Home-page: https://github.com/acturtle/cashflower
 Author: Zuzanna Chmielewska
 Project-URL: Source, https://github.com/acturtle/cashflower
 Project-URL: Tracker, https://github.com/acturtle/cashflower/issues
 Project-URL: Documentation, https://cashflower.acturtle.com
 Requires-Python: >=3.9
```

### Comparing `cashflower-0.4.5/cashflower.egg-info/SOURCES.txt` & `cashflower-0.4.6/cashflower.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cashflower-0.4.5/setup.py` & `cashflower-0.4.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,9 +20,9 @@
     project_urls={
         'Source': 'https://github.com/acturtle/cashflower',
         'Tracker': 'https://github.com/acturtle/cashflower/issues',
         'Documentation': 'https://cashflower.acturtle.com',
     },
     python_requires='>=3.9',
     url="https://github.com/acturtle/cashflower",
-    version="0.4.5",
+    version="0.4.6",
 )
```

### Comparing `cashflower-0.4.5/tests/test_cashflow.py` & `cashflower-0.4.6/tests/test_cashflow.py`

 * *Files identical despite different names*

### Comparing `cashflower-0.4.5/tests/test_start.py` & `cashflower-0.4.6/tests/test_start.py`

 * *Files identical despite different names*

### Comparing `cashflower-0.4.5/tests/test_utils.py` & `cashflower-0.4.6/tests/test_utils.py`

 * *Files identical despite different names*

