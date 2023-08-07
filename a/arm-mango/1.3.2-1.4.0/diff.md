# Comparing `tmp/arm_mango-1.3.2.tar.gz` & `tmp/arm_mango-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arm_mango-1.3.2.tar", max compression
+gzip compressed data, was "arm_mango-1.4.0.tar", max compression
```

## Comparing `arm_mango-1.3.2.tar` & `arm_mango-1.4.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    11357 2022-07-09 05:12:38.000000 arm_mango-1.3.2/LICENSE
--rw-r--r--   0        0        0    23264 2023-08-03 14:19:55.422043 arm_mango-1.3.2/README.md
--rw-r--r--   0        0        0      143 2023-01-21 04:22:18.258761 arm_mango-1.3.2/mango/__init__.py
--rwxr-xr-x   0        0        0        0 2023-01-06 12:23:27.333605 arm_mango-1.3.2/mango/domain/__init__.py
--rw-r--r--   0        0        0     2974 2022-07-09 05:12:44.000000 arm_mango-1.3.2/mango/domain/batch_parameter_sampler.py
--rw-r--r--   0        0        0      121 2022-07-09 05:12:44.000000 arm_mango-1.3.2/mango/domain/distribution.py
--rw-r--r--   0        0        0     7246 2023-01-21 04:22:18.259045 arm_mango-1.3.2/mango/domain/domain_space.py
--rw-r--r--   0        0        0    15383 2023-01-21 04:22:18.259322 arm_mango-1.3.2/mango/metatuner.py
--rwxr-xr-x   0        0        0        0 2023-01-06 12:23:27.333678 arm_mango-1.3.2/mango/optimizer/__init__.py
--rw-r--r--   0        0        0      248 2022-07-09 05:12:42.000000 arm_mango-1.3.2/mango/optimizer/base_predictor.py
--rw-r--r--   0        0        0    13839 2023-01-21 04:22:18.259600 arm_mango-1.3.2/mango/optimizer/bayesian_learning.py
--rw-r--r--   0        0        0     1878 2022-07-09 05:12:42.000000 arm_mango-1.3.2/mango/scheduler.py
--rw-r--r--   0        0        0    13348 2023-08-03 14:19:55.425788 arm_mango-1.3.2/mango/tuner.py
--rw-r--r--   0        0        0      752 2023-08-03 14:25:18.677874 arm_mango-1.3.2/pyproject.toml
--rw-r--r--   0        0        0    24174 1970-01-01 00:00:00.000000 arm_mango-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-07-09 05:12:38.000000 arm_mango-1.4.0/LICENSE
+-rw-r--r--   0        0        0    23713 2023-08-07 02:56:27.432212 arm_mango-1.4.0/README.md
+-rw-r--r--   0        0        0      143 2023-01-21 04:22:18.258761 arm_mango-1.4.0/mango/__init__.py
+-rwxr-xr-x   0        0        0        0 2023-01-06 12:23:27.333605 arm_mango-1.4.0/mango/domain/__init__.py
+-rw-r--r--   0        0        0     2974 2022-07-09 05:12:44.000000 arm_mango-1.4.0/mango/domain/batch_parameter_sampler.py
+-rw-r--r--   0        0        0      121 2022-07-09 05:12:44.000000 arm_mango-1.4.0/mango/domain/distribution.py
+-rw-r--r--   0        0        0     7246 2023-01-21 04:22:18.259045 arm_mango-1.4.0/mango/domain/domain_space.py
+-rw-r--r--   0        0        0    15383 2023-01-21 04:22:18.259322 arm_mango-1.4.0/mango/metatuner.py
+-rwxr-xr-x   0        0        0        0 2023-01-06 12:23:27.333678 arm_mango-1.4.0/mango/optimizer/__init__.py
+-rw-r--r--   0        0        0      248 2022-07-09 05:12:42.000000 arm_mango-1.4.0/mango/optimizer/base_predictor.py
+-rw-r--r--   0        0        0    13839 2023-01-21 04:22:18.259600 arm_mango-1.4.0/mango/optimizer/bayesian_learning.py
+-rw-r--r--   0        0        0     1878 2022-07-09 05:12:42.000000 arm_mango-1.4.0/mango/scheduler.py
+-rw-r--r--   0        0        0    14249 2023-08-07 02:56:27.434926 arm_mango-1.4.0/mango/tuner.py
+-rw-r--r--   0        0        0      770 2023-08-07 02:56:27.435568 arm_mango-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0    24662 1970-01-01 00:00:00.000000 arm_mango-1.4.0/PKG-INFO
```

### Comparing `arm_mango-1.3.2/LICENSE` & `arm_mango-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `arm_mango-1.3.2/README.md` & `arm_mango-1.4.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -368,15 +368,25 @@
     '''
         Given a list of samples (each sample is a dict with parameter names as keys)
         Returns a list of True/False elements indicating whether the corresponding sample
         satisfies the constraints or not
     '''
   ```
   See [this](<examples/Test functions for constrained optimization.ipynb>) notebook for an example.
-- *initial_custom*: A list of initial evaluation points to warm up the optimizer instead of random sampling. For example, for a search space with two parameters `x1` and `x2` the input could be:   `[{'x1': 10, 'x2': -5}, {'x1': 0, 'x2': 10}]`. This allows the user to customize the initial evaluation points and therefore guide the optimization process. If this option is given then `initial_random` is ignored.  
+- *initial_custom*: A list of initial evaluation points to warm up the optimizer instead of random sampling. 
+It can be either:  
+  - A list of dict with parameters. For example, for a search space with two parameters `x1` and `x2` the input could be:
+  `[{'x1': 10, 'x2': -5}, {'x1': 0, 'x2': 10}]`. 
+  - A list of tuple with parameters and objective function values. For example, if the objective function is to add 
+  `x1` and `x2` the input could be:
+  `[({'x1': 10, 'x2': -5}, 5), ({'x1': 0, 'x2': 10}, 10)]`. 
+  
+  This allows the user to customize the initial evaluation points and therefore guide the optimization process.
+It also enables starting the optimizer from the results of a previous tuner run (see [this](<examples/warmup.ipynb>) notebook for a working example).
+Note that if `initial_custom` option is given then `initial_random` is ignored.  
 
 
 The default configuration parameters can be modified, as shown below. Only the parameters whose values need to adjusted can be passed as the dictionary.
 
 ```python
 conf_dict = dict(num_iteration=40, domain_size=10000, initial_random=3)
```

### Comparing `arm_mango-1.3.2/mango/domain/batch_parameter_sampler.py` & `arm_mango-1.4.0/mango/domain/batch_parameter_sampler.py`

 * *Files identical despite different names*

### Comparing `arm_mango-1.3.2/mango/domain/domain_space.py` & `arm_mango-1.4.0/mango/domain/domain_space.py`

 * *Files identical despite different names*

### Comparing `arm_mango-1.3.2/mango/metatuner.py` & `arm_mango-1.4.0/mango/metatuner.py`

 * *Files identical despite different names*

### Comparing `arm_mango-1.3.2/mango/optimizer/bayesian_learning.py` & `arm_mango-1.4.0/mango/optimizer/bayesian_learning.py`

 * *Files identical despite different names*

### Comparing `arm_mango-1.3.2/mango/scheduler.py` & `arm_mango-1.4.0/mango/scheduler.py`

 * *Files identical despite different names*

### Comparing `arm_mango-1.3.2/mango/tuner.py` & `arm_mango-1.4.0/mango/tuner.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,76 +1,80 @@
 """
 Main Tuner Class which uses other abstractions.
 General usage is to find the optimal hyper-parameters of the classifier
 """
 
 import copy
-from dataclasses import dataclass, field
+from collections.abc import Mapping, Iterable
+from dataclasses import dataclass
 import logging
 import random
 from typing import Callable
 
 from mango.domain.domain_space import domain_space
 from mango.optimizer.bayesian_learning import BayesianLearning
 from scipy.stats._distn_infrastructure import rv_frozen
 
 from tqdm.auto import tqdm
 import numpy as np
 
 # setting warnings to ignore for now
 import warnings
 
-warnings.filterwarnings('ignore')
+warnings.filterwarnings("ignore")
 
 _logger = logging.getLogger(__name__)
 
 
 class Tuner:
     @dataclass
     class Config:
         domain_size: int = None
         initial_random: int = 2
-        initial_custom: dict = None
+        initial_custom: list = None
         num_iteration: int = 20
         batch_size: int = 1
-        optimizer: str = 'Bayesian'
-        parallel_strategy: str = 'clustering'
+        optimizer: str = "Bayesian"
+        parallel_strategy: str = "clustering"
         surrogate: object = None  # used to test different kernel functions
-        valid_optimizers = ['Bayesian', 'Random']
-        valid_parallel_strategies = ['penalty', 'clustering']
+        valid_optimizers = ["Bayesian", "Random"]
+        valid_parallel_strategies = ["penalty", "clustering"]
         alpha: float = 2.0
         exploration: float = 1.0
         exploration_decay: float = 0.9
         exploration_min: float = 0.1
         fixed_domain: bool = False
         early_stopping: Callable = None
         constraint: Callable = None
 
         def __post_init__(self):
             if self.optimizer not in self.valid_optimizers:
-                raise ValueError(f'optimizer: {self.optimizer} is not valid, should be one of {self.valid_optimizers}')
+                raise ValueError(
+                    f"optimizer: {self.optimizer} is not valid, should be one of {self.valid_optimizers}"
+                )
             if self.parallel_strategy not in self.valid_parallel_strategies:
                 raise ValueError(
-                    f'parallel strategy: {self.parallel_strategy} is not valid, should be one of {self.valid_parallel_strategies}')
+                    f"parallel strategy: {self.parallel_strategy} is not valid, should be one of {self.valid_parallel_strategies}"
+                )
 
         @property
         def is_bayesian(self):
-            return self.optimizer == 'Bayesian'
+            return self.optimizer == "Bayesian"
 
         @property
         def is_random(self):
-            return self.optimizer == 'Random'
+            return self.optimizer == "Random"
 
         @property
         def strategy_is_penalty(self):
-            return self.parallel_strategy == 'penalty'
+            return self.parallel_strategy == "penalty"
 
         @property
         def strategy_is_clustering(self):
-            return self.parallel_strategy == 'clustering'
+            return self.parallel_strategy == "clustering"
 
         def early_stop(self, results):
             if self.early_stopping is None:
                 return False
 
             results = copy.deepcopy(results)
             return self.early_stopping(results)
@@ -86,30 +90,30 @@
 
         self.config = Tuner.Config(**conf_dict)
 
         if self.config.domain_size is None:
             self.config.domain_size = self.calculateDomainSize(self.param_dict)
 
         # overwrite batch size if given as a property of objective function
-        if hasattr(objective, 'batch_size'):
+        if hasattr(objective, "batch_size"):
             self.config.batch_size = objective.batch_size
 
         # save domain size
-        self.ds = domain_space(self.param_dict,
-                               self.config.domain_size,
-                               constraint=self.config.constraint)
+        self.ds = domain_space(
+            self.param_dict, self.config.domain_size, constraint=self.config.constraint
+        )
 
         # stores the results of using the tuner
         self.results = dict()
 
     @staticmethod
     def calculateDomainSize(param_dict):
         """
-           Calculating the domain size to be explored for finding
-           optimum of bayesian optimizer
+        Calculating the domain size to be explored for finding
+        optimum of bayesian optimizer
         """
         # Minimum and maximum domain size
         domain_min = 50000
         domain_max = 500000
 
         domain_size = 1
 
@@ -151,55 +155,75 @@
     def maximize(self):
         return self.run()
 
     def minimize(self):
         self.maximize_objective = False
         return self.run()
 
+    def process_initial_custom(self):
+        init_values = self.config.initial_custom
+
+        if all(isinstance(v, Mapping) for v in init_values):
+            X_tried = copy.deepcopy(init_values)
+            X_list, Y_list = self.runUserObjective(X_tried)
+            return X_list, Y_list, X_tried
+        elif all(isinstance(v, tuple) and len(v) == 2 for v in init_values):
+            X_list = copy.deepcopy([v[0] for v in init_values])
+            Y_list = np.array([v[1] for v in init_values])
+            return X_list, Y_list, X_list
+        else:
+            raise TypeError(
+                f"Elements of initial_custom param should be either a dict of params or tuple (params, y),"
+                f" got: {[type(v).__name__ for v in init_values]}"
+            )
 
     def run_initial(self):
         if self.config.initial_custom is not None:
-            X_tried = copy.deepcopy(self.config.initial_custom)
-            X_list, Y_list = self.runUserObjective(X_tried)
+            return self.process_initial_custom()
         else:
             # getting first few random values
             X_tried = self.ds.get_random_sample(self.config.initial_random)
             X_list, Y_list = self.runUserObjective(X_tried)
 
             # in case initial random results are invalid try different samples
             n_tries = 1
             while len(Y_list) < self.config.initial_random and n_tries < 3:
-                X_tried2 = self.ds.get_random_sample(self.config.initial_random - len(Y_list))
+                X_tried2 = self.ds.get_random_sample(
+                    self.config.initial_random - len(Y_list)
+                )
                 X_list2, Y_list2 = self.runUserObjective(X_tried2)
                 X_tried2.extend(X_tried2)
                 X_list = np.append(X_list, X_list2)
                 Y_list = np.append(Y_list, Y_list2)
                 n_tries += 1
 
             if len(Y_list) == 0:
-                raise ValueError("No valid configuration found to initiate the Bayesian Optimizer")
+                raise ValueError(
+                    "No valid configuration found to initiate the Bayesian Optimizer"
+                )
         return X_list, Y_list, X_tried
 
     def runBayesianOptimizer(self):
         results = dict()
 
         X_list, Y_list, X_tried = self.run_initial()
 
-
         # evaluated hyper parameters are used
         X_init = self.ds.convert_GP_space(X_list)
         Y_init = Y_list.reshape(len(Y_list), 1)
 
         # setting the initial random hyper parameters tried
-        results['random_params'] = X_list
-        results['random_params_objective'] = Y_list
+        results["random_params"] = X_list
+        results["random_params_objective"] = Y_list
 
-        Optimizer = BayesianLearning(surrogate=self.config.surrogate,
-                                     alpha=self.config.alpha,
-                                     domain_size=self.config.domain_size)
+        Optimizer = BayesianLearning(
+            surrogate=self.config.surrogate,
+            alpha=self.config.alpha,
+            domain_size=self.config.domain_size,
+        )
 
         X_sample = X_init
         Y_sample = Y_init
 
         hyper_parameters_tried = X_tried
         objective_function_values = Y_list
         surrogate_values = Y_list
@@ -216,26 +240,31 @@
 
             # adding a Minimum exploration to explore independent of UCB
             if random.random() < self.config.exploration:
                 random_parameters = self.ds.get_random_sample(self.config.batch_size)
                 X_next_batch = self.ds.convert_GP_space(random_parameters)
 
                 if self.config.exploration > self.config.exploration_min:
-                    self.config.exploration = self.config.exploration * self.config.exploration_decay
+                    self.config.exploration = (
+                        self.config.exploration * self.config.exploration_decay
+                    )
 
             elif self.config.strategy_is_penalty:
-                X_next_batch = Optimizer.get_next_batch(X_sample, Y_sample, X_domain_np,
-                                                        batch_size=self.config.batch_size)
+                X_next_batch = Optimizer.get_next_batch(
+                    X_sample, Y_sample, X_domain_np, batch_size=self.config.batch_size
+                )
             elif self.config.strategy_is_clustering:
-                X_next_batch = Optimizer.get_next_batch_clustering(X_sample, Y_sample, X_domain_np,
-                                                                   batch_size=self.config.batch_size)
+                X_next_batch = Optimizer.get_next_batch_clustering(
+                    X_sample, Y_sample, X_domain_np, batch_size=self.config.batch_size
+                )
             else:
                 # assume penalty approach
-                X_next_batch = Optimizer.get_next_batch(X_sample, Y_sample, X_domain_np,
-                                                        batch_size=self.config.batch_size)
+                X_next_batch = Optimizer.get_next_batch(
+                    X_sample, Y_sample, X_domain_np, batch_size=self.config.batch_size
+                )
 
             # Scheduler
             X_next_PS = self.ds.convert_PS_space(X_next_batch)
 
             # if all the xs have failed before, replace them with random sample
             # as we will not get any new information otherwise
             if all(x in x_failed_evaluations for x in X_next_PS):
@@ -255,41 +284,47 @@
 
             Y_next_batch = Y_next_list.reshape(len(Y_next_list), 1)
             # update X_next_batch to successfully evaluated values
             X_next_batch = self.ds.convert_GP_space(X_next_list)
 
             # update the bookeeping of values tried
             hyper_parameters_tried = np.append(hyper_parameters_tried, X_next_list)
-            objective_function_values = np.append(objective_function_values, Y_next_list)
-            surrogate_values = np.append(surrogate_values, Optimizer.surrogate.predict(X_next_batch))
+            objective_function_values = np.append(
+                objective_function_values, Y_next_list
+            )
+            surrogate_values = np.append(
+                surrogate_values, Optimizer.surrogate.predict(X_next_batch)
+            )
 
             # Appending to the current samples
             X_sample = np.vstack((X_sample, X_next_batch))
             Y_sample = np.vstack((Y_sample, Y_next_batch))
 
             # referesh domain if not fixed
             if not self.config.fixed_domain:
                 domain_list = self.ds.get_domain()
                 X_domain_np = self.ds.convert_GP_space(domain_list)
 
-            results['params_tried'] = hyper_parameters_tried
-            results['objective_values'] = objective_function_values
-            results['surrogate_values'] = surrogate_values
-
-            results['best_objective'] = np.max(results['objective_values'])
-            results['best_params'] = results['params_tried'][np.argmax(results['objective_values'])]
+            results["params_tried"] = hyper_parameters_tried
+            results["objective_values"] = objective_function_values
+            results["surrogate_values"] = surrogate_values
+
+            results["best_objective"] = np.max(results["objective_values"])
+            results["best_params"] = results["params_tried"][
+                np.argmax(results["objective_values"])
+            ]
             if self.maximize_objective is False:
-                results['objective_values'] = -1 * results['objective_values']
-                results['best_objective'] = -1 * results['best_objective']
+                results["objective_values"] = -1 * results["objective_values"]
+                results["best_objective"] = -1 * results["best_objective"]
 
-            pbar.set_description("Best score: %s" % results['best_objective'])
+            pbar.set_description("Best score: %s" % results["best_objective"])
 
             # check if early stop criteria has been met
             if self.config.early_stop(results):
-                _logger.info('Early stopping criteria satisfied')
+                _logger.info("Early stopping criteria satisfied")
                 break
 
         # saving the optimizer and ds in the tuner object which can save the surrogate function and ds details
         self.Optimizer = Optimizer
 
         return results
 
@@ -303,34 +338,36 @@
         n_iterations = self.config.num_iteration
         random_hyper_parameters = self.ds.get_random_sample(n_iterations * batch_size)
 
         # running the iterations
         pbar = tqdm(range(0, len(random_hyper_parameters), batch_size))
         for idx in pbar:
             # getting batch by batch random values to try
-            batch_hyper_parameters = random_hyper_parameters[idx:idx + batch_size]
+            batch_hyper_parameters = random_hyper_parameters[idx : idx + batch_size]
             X_list, Y_list = self.runUserObjective(batch_hyper_parameters)
 
             X_sample_list = np.append(X_sample_list, X_list)
             Y_sample_list = np.append(Y_sample_list, Y_list)
 
-            results['params_tried'] = X_sample_list
-            results['objective_values'] = Y_sample_list
+            results["params_tried"] = X_sample_list
+            results["objective_values"] = Y_sample_list
 
-            results['best_objective'] = np.max(results['objective_values'])
-            results['best_params'] = results['params_tried'][np.argmax(results['objective_values'])]
+            results["best_objective"] = np.max(results["objective_values"])
+            results["best_params"] = results["params_tried"][
+                np.argmax(results["objective_values"])
+            ]
             if self.maximize_objective is False:
-                results['objective_values'] = -1 * results['objective_values']
-                results['best_objective'] = -1 * results['best_objective']
+                results["objective_values"] = -1 * results["objective_values"]
+                results["best_objective"] = -1 * results["best_objective"]
 
-            pbar.set_description("Best score: %s" % results['best_objective'])
+            pbar.set_description("Best score: %s" % results["best_objective"])
 
             # check if early stop criteria has been met
             if self.config.early_stop(results):
-                _logger.info('Early stopping criteria satisfied')
+                _logger.info("Early stopping criteria satisfied")
                 break
 
         return results
 
     def runUserObjective(self, X_next_PS):
         # initially assuming entire X_next_PS is evaluated and returned results are only Y values
         X_list_evaluated = X_next_PS
```

### Comparing `arm_mango-1.3.2/PKG-INFO` & `arm_mango-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arm-mango
-Version: 1.3.2
+Version: 1.4.0
 Summary: parallel bayesian optimization over complex search spaces
 Home-page: https://github.com/ARM-software/mango
 License: Apache-2.0
 Author: Sandeep Singh Sandha
 Author-email: sandha.iitr@gmail.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: Apache Software License
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: attrdict (>=2.0.1)
 Requires-Dist: numpy (>=1.17.0)
+Requires-Dist: pytest (>=7.4.0,<8.0.0)
 Requires-Dist: scikit_learn (>=0.21.3)
 Requires-Dist: scipy (>=1.4.1)
 Requires-Dist: tqdm (>=4.36.1)
 Project-URL: Repository, https://github.com/ARM-software/mango
 Description-Content-Type: text/markdown
 
 # Mango: A parallel hyperparameter tuning library
@@ -392,15 +393,25 @@
     '''
         Given a list of samples (each sample is a dict with parameter names as keys)
         Returns a list of True/False elements indicating whether the corresponding sample
         satisfies the constraints or not
     '''
   ```
   See [this](<examples/Test functions for constrained optimization.ipynb>) notebook for an example.
-- *initial_custom*: A list of initial evaluation points to warm up the optimizer instead of random sampling. For example, for a search space with two parameters `x1` and `x2` the input could be:   `[{'x1': 10, 'x2': -5}, {'x1': 0, 'x2': 10}]`. This allows the user to customize the initial evaluation points and therefore guide the optimization process. If this option is given then `initial_random` is ignored.  
+- *initial_custom*: A list of initial evaluation points to warm up the optimizer instead of random sampling. 
+It can be either:  
+  - A list of dict with parameters. For example, for a search space with two parameters `x1` and `x2` the input could be:
+  `[{'x1': 10, 'x2': -5}, {'x1': 0, 'x2': 10}]`. 
+  - A list of tuple with parameters and objective function values. For example, if the objective function is to add 
+  `x1` and `x2` the input could be:
+  `[({'x1': 10, 'x2': -5}, 5), ({'x1': 0, 'x2': 10}, 10)]`. 
+  
+  This allows the user to customize the initial evaluation points and therefore guide the optimization process.
+It also enables starting the optimizer from the results of a previous tuner run (see [this](<examples/warmup.ipynb>) notebook for a working example).
+Note that if `initial_custom` option is given then `initial_random` is ignored.  
 
 
 The default configuration parameters can be modified, as shown below. Only the parameters whose values need to adjusted can be passed as the dictionary.
 
 ```python
 conf_dict = dict(num_iteration=40, domain_size=10000, initial_random=3)
```

