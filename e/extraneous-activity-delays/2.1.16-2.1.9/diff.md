# Comparing `tmp/extraneous_activity_delays-2.1.16.tar.gz` & `tmp/extraneous_activity_delays-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extraneous_activity_delays-2.1.16.tar", max compression
+gzip compressed data, was "extraneous_activity_delays-2.1.9.tar", max compression
```

## Comparing `extraneous_activity_delays-2.1.16.tar` & `extraneous_activity_delays-2.1.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    11349 2023-08-07 09:36:59.343847 extraneous_activity_delays-2.1.16/LICENSE
--rw-r--r--   0        0        0     9404 2023-08-07 09:36:59.343847 extraneous_activity_delays-2.1.16/README.md
--rw-r--r--   0        0        0      556 2023-08-07 09:36:59.399847 extraneous_activity_delays-2.1.16/pyproject.toml
--rw-r--r--   0        0        0       64 2023-08-07 09:36:59.399847 extraneous_activity_delays-2.1.16/src/extraneous_activity_delays/__init__.py
--rw-r--r--   0        0        0     7610 2023-08-07 09:36:59.399847 extraneous_activity_delays-2.1.16/src/extraneous_activity_delays/config.py
--rw-r--r--   0        0        0    14588 2023-08-07 09:36:59.399847 extraneous_activity_delays-2.1.16/src/extraneous_activity_delays/delay_discoverer.py
--rw-r--r--   0        0        0    16156 2023-08-07 09:36:59.399847 extraneous_activity_delays-2.1.16/src/extraneous_activity_delays/enhance_with_delays.py
--rw-r--r--   0        0        0       53 2023-08-07 09:36:59.399847 extraneous_activity_delays-2.1.16/src/extraneous_activity_delays/prosimos/__init__.py
--rw-r--r--   0        0        0     2358 2023-08-07 09:36:59.399847 extraneous_activity_delays-2.1.16/src/extraneous_activity_delays/prosimos/simulation_model_enhancer.py
--rw-r--r--   0        0        0     2118 2023-08-07 09:36:59.399847 extraneous_activity_delays-2.1.16/src/extraneous_activity_delays/prosimos/simulator.py
--rw-r--r--   0        0        0       53 2023-08-07 09:36:59.399847 extraneous_activity_delays-2.1.16/src/extraneous_activity_delays/qbp/__init__.py
--rw-r--r--   0        0        0     4372 2023-08-07 09:36:59.399847 extraneous_activity_delays-2.1.16/src/extraneous_activity_delays/qbp/simulation_model_enhancer.py
--rw-r--r--   0        0        0     1593 2023-08-07 09:36:59.399847 extraneous_activity_delays-2.1.16/src/extraneous_activity_delays/qbp/simulator.py
--rw-r--r--   0        0        0       60 2023-08-07 09:36:59.399847 extraneous_activity_delays-2.1.16/src/extraneous_activity_delays/utils/__init__.py
--rw-r--r--   0        0        0     3194 2023-08-07 09:36:59.399847 extraneous_activity_delays-2.1.16/src/extraneous_activity_delays/utils/bpmn_enhancement.py
--rw-r--r--   0        0        0      810 2023-08-07 09:36:59.399847 extraneous_activity_delays-2.1.16/src/extraneous_activity_delays/utils/file_manager.py
--rw-r--r--   0        0        0    10114 1970-01-01 00:00:00.000000 extraneous_activity_delays-2.1.16/PKG-INFO
+-rw-r--r--   0        0        0    11349 2023-05-10 11:11:52.365418 extraneous_activity_delays-2.1.9/LICENSE
+-rw-r--r--   0        0        0     9404 2023-05-24 10:39:33.962708 extraneous_activity_delays-2.1.9/README.md
+-rw-r--r--   0        0        0      553 2023-05-24 10:27:55.491113 extraneous_activity_delays-2.1.9/pyproject.toml
+-rw-r--r--   0        0        0       64 2023-05-24 10:09:51.247101 extraneous_activity_delays-2.1.9/src/extraneous_activity_delays/__init__.py
+-rw-r--r--   0        0        0     6580 2023-05-24 10:36:04.338823 extraneous_activity_delays-2.1.9/src/extraneous_activity_delays/config.py
+-rw-r--r--   0        0        0    13561 2023-05-24 10:11:56.745400 extraneous_activity_delays-2.1.9/src/extraneous_activity_delays/delay_discoverer.py
+-rw-r--r--   0        0        0    16020 2023-05-24 10:11:56.759114 extraneous_activity_delays-2.1.9/src/extraneous_activity_delays/enhance_with_delays.py
+-rw-r--r--   0        0        0       53 2023-05-24 10:09:51.253732 extraneous_activity_delays-2.1.9/src/extraneous_activity_delays/prosimos/__init__.py
+-rw-r--r--   0        0        0     2358 2023-05-24 10:11:56.721128 extraneous_activity_delays-2.1.9/src/extraneous_activity_delays/prosimos/simulation_model_enhancer.py
+-rw-r--r--   0        0        0     2118 2023-05-24 10:11:56.715176 extraneous_activity_delays-2.1.9/src/extraneous_activity_delays/prosimos/simulator.py
+-rw-r--r--   0        0        0       53 2023-05-24 10:09:51.260582 extraneous_activity_delays-2.1.9/src/extraneous_activity_delays/qbp/__init__.py
+-rw-r--r--   0        0        0     4372 2023-05-24 10:11:56.729581 extraneous_activity_delays-2.1.9/src/extraneous_activity_delays/qbp/simulation_model_enhancer.py
+-rw-r--r--   0        0        0     1593 2023-05-24 10:11:56.717662 extraneous_activity_delays-2.1.9/src/extraneous_activity_delays/qbp/simulator.py
+-rw-r--r--   0        0        0       60 2023-05-24 10:09:51.266529 extraneous_activity_delays-2.1.9/src/extraneous_activity_delays/utils/__init__.py
+-rw-r--r--   0        0        0     3194 2023-05-24 10:11:56.736893 extraneous_activity_delays-2.1.9/src/extraneous_activity_delays/utils/bpmn_enhancement.py
+-rw-r--r--   0        0        0      810 2023-05-24 10:11:56.726632 extraneous_activity_delays-2.1.9/src/extraneous_activity_delays/utils/file_manager.py
+-rw-r--r--   0        0        0    10110 1970-01-01 00:00:00.000000 extraneous_activity_delays-2.1.9/PKG-INFO
```

### Comparing `extraneous_activity_delays-2.1.16/LICENSE` & `extraneous_activity_delays-2.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `extraneous_activity_delays-2.1.16/README.md` & `extraneous_activity_delays-2.1.9/README.md`

 * *Files identical despite different names*

### Comparing `extraneous_activity_delays-2.1.16/pyproject.toml` & `extraneous_activity_delays-2.1.9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "extraneous-activity-delays"
-version = "2.1.16"
+version = "2.1.9"
 description = ""
 authors = ["David Chapela de la Campa <david.chapela.delacampa@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9, <3.12"
-prosimos = "^1.2.6"
+prosimos = "^1.2.4"
 hyperopt = "^0.2.7"
 lxml = "^4.9.2"
 log-distance-measures = "^1.0.2"
-start-time-estimator = "^1.10.10"
-pix-framework = "^0.10.0"
+start-time-estimator = "^1.10.9"
+pix-framework = "^0.8.3"
 
 [tool.ruff]
 line-length = 120
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
```

### Comparing `extraneous_activity_delays-2.1.16/src/extraneous_activity_delays/config.py` & `extraneous_activity_delays-2.1.9/src/extraneous_activity_delays/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -79,20 +79,14 @@
     Extraneous delays parameters:
         should_consider_timer       Function taking as input a list of seconds for all the delays that activity has registered, and
                                     returning a bool indicating if those delays should be considered as a timer, or discarded as outliers.
         time_gap                    For complex extraneous delays, maximum interval of time allowed from a work item (task of off-duty
                                     interval) to another work item to not consider that the resource was available in that interval. For
                                     example, a resource works in a task from 16.00 to 17.49, but their off-duty period starts at 18.49. If
                                     time-gap is set to >11 minutes, it won't be counted as an available period.
-        extrapolate                 If 'True', when computing the first and last available times (complex delays), instead of computing
-                                    the first available time as such, move it to half its distance between itself and the enablement of
-                                    the activity instance. For example, if the enablement is at 1, and the discovered first available time
-                                    is at 5, the first available time is corrected to 3 (the middle point). The same is done for the last
-                                    available and the start of the activity instance. The objective is to reduce potential mis-estimations
-                                    as the real first and last available times are unknown, but within those two intervals.
 
     Optimization process parameters:
         num_iterations              Number of iterations of the hyper-optimization search.
         num_evaluation_simulations  Number of simulations performed with each enhanced BPMN model to evaluate its quality.
         max_alpha                   Maximum scale factor to multiply the discovered timers in the hyper-optimization.
         training_partition_ratio    Float value between 0.0 and 1.0 (or None). If None, train and validate the hyper-parametrization using
                                     the full event log passed as argument. Otherwise, perform the hyper-parametrization with a hold-out
@@ -104,41 +98,38 @@
         concurrency_thresholds      Thresholds for the concurrency oracle (heuristics or overlapping).
         working_schedules           Dictionary with the resources as key and the working calendars (RCalendar) as value.
 
     General parameters:
         process_name                Name of the process to use in the output files (BPMN and simulated log files).
         log_ids                     Identifiers for each key element (e.g. executed activity or resource).
         debug                       Boolean denoting whether to print debug information or not.
-        clean_intermediate_files    Boolean denoting whether to remove the folders of the non-best solutions or not.
     """
 
     # Extraneous delays options
-    discovery_method: DiscoveryMethod = DiscoveryMethod.COMPLEX
+    discovery_method: DiscoveryMethod = DiscoveryMethod.NAIVE
     timer_placement: TimerPlacement = TimerPlacement.BEFORE
     simulation_engine: SimulationEngine = SimulationEngine.PROSIMOS
     optimization_metric: OptimizationMetric = OptimizationMetric.RELATIVE_EMD
     # Extraneous delays parameters
     should_consider_timer: Callable[[list], bool] = _should_consider_timer
     time_gap: pd.Timedelta = pd.Timedelta(seconds=1)
-    extrapolate_complex_delays_estimation: bool = False
     # Optimization process parameters
     num_iterations: int = 100
     num_evaluation_simulations: int = 3
     max_alpha: float = 10.0
     training_partition_ratio: float = None
     # Enabled time & resource availability estimations
     concurrency_thresholds: ConcurrencyThresholds = field(
         default_factory=lambda: ConcurrencyThresholds(df=0.5)
     )
     working_schedules: dict = field(default_factory=dict)
     # General parameters
     process_name: str = "process"
     log_ids: EventLogIDs = field(default_factory=lambda: DEFAULT_CSV_IDS)
     debug: bool = False
-    clean_intermediate_files: bool = False
     # Paths
     PATH_PROJECT = get_project_dir()
     PATH_INPUTS = PATH_PROJECT.joinpath("inputs")
     PATH_OUTPUTS = PATH_PROJECT.joinpath("outputs")
     PATH_EXTERNAL_TOOLS = PATH_PROJECT.joinpath("external_tools")
     PATH_QBP = (
         PATH_PROJECT.joinpath("external_tools")
```

### Comparing `extraneous_activity_delays-2.1.16/src/extraneous_activity_delays/delay_discoverer.py` & `extraneous_activity_delays-2.1.9/src/extraneous_activity_delays/delay_discoverer.py`

 * *Files 5% similar despite different names*

```diff
@@ -154,15 +154,14 @@
             indexes += [index]
             first_instant, last_instant = _get_first_and_last_available(
                 beginning=event[log_ids.enabled_time],
                 end=event[log_ids.start_time],
                 starts=list(performed_events[log_ids.start_time]) + [interval.start for interval in resource_off_duty],
                 ends=list(performed_events[log_ids.end_time]) + [interval.end for interval in resource_off_duty],
                 time_gap=config.time_gap,
-                extrapolate=config.extrapolate_complex_delays_estimation,
             )
             if first_instant:
                 # Available instants found
                 first_available += [first_instant]
                 last_available += [last_instant]
             else:
                 # Busy during all the waiting time, set start time as availability
@@ -178,29 +177,23 @@
 
 def _get_first_and_last_available(
     beginning: pd.Timestamp,
     end: pd.Timestamp,
     starts: list,
     ends: list,
     time_gap: pd.Timedelta,
-    extrapolate: bool = False,
 ) -> Tuple[pd.Timestamp, pd.Timestamp]:
     """
     Get the first instant from the period [from]-[to] where the resource was available for a [time_gap] amount of time.
 
     :param beginning:   Start of the interval where to search.
     :param end:         End of the interval where to search.
     :param starts:      List of instants where either a non-working period or an activity instance started.
     :param ends:        List of instants where either an activity instance or a non-working period finished.
     :param time_gap:    Minimum time gap required for a non-working period to be considered as such.
-    :param extrapolate: If 'True', instead of getting the first available time as such, move it to half its distance
-                        between itself and the beginning of the interval. For example, if the beginning is at 1, and
-                        the discovered first available time is at 5, the extrapolated one is 3 (the middle point). The
-                        same is done with the last available and the end of the interval. The objective is to reduce
-                        potential mis-estimations as the real first available time is unknown.
 
     :return: A tuple with the first and last timestamps within all [start] and [end] timestamps where the
     resource was available for a [time_gap] amount of time.
     """
     # Add beginning and end of interval as artificial instant activities
     starts += [beginning, end]
     ends += [beginning, end]
@@ -221,22 +214,21 @@
     i = 0
     active = 0  # Number of active unavailable intervals
     while not first_available and i < len(times):
         # Increase active unavailable intervals if current timestamps is 'start', or decrease otherwise
         active += 1 if times[i][1] == "start" else -1
         # Check if no active unavailable intervals
         if active == 0 and (  # No active unavailable intervals at this point, and
-            i + 1 == len(times) or  # either this is the last point, or
-            times[i + 1][0] - times[i][0] >= time_gap  # there is an available time gap with enough duration
-        ):
+            i + 1 == len(times) or times[i + 1][0] - times[i][0] >= time_gap  # either this is the last point, or
+        ):  # there is an available time gap with enough duration
             # Resource available at this point, check time gap until next event
             first_available = times[i][0]
         i += 1
     # If time gap found, search for last available, not necessary otherwise
-    if not pd.isna(first_available):
+    if first_available:
         # Go over them end->start, until a moment with no active unavailable intervals is reached
         i = len(times) - 1  # Index to go over the timestamps
         active = 0  # Number of active unavailable intervals
         while not last_available and i > 0:
             if times[i][0] <= first_available:
                 # If the search reached [first_available], set to it and finish
                 last_available = first_available
@@ -247,19 +239,15 @@
                 if active == 0 and (  # No active unavailable intervals at this point, and
                     i == 0
                     or times[i][0] - times[i - 1][0] >= time_gap  # either this is the last point in the search, or
                 ):  # there is an available time gap with enough duration
                     # Resource available at this point, check time gap until next event
                     last_available = times[i][0]
             i -= 1
-    # If we are extrapolating the timestamps AND both timestamps were found
-    if extrapolate and not pd.isna(first_available) and not pd.isna(last_available):
-        first_available = first_available - ((first_available - beginning) / 2)
-        last_available = last_available + ((end - last_available) / 2)
-    # Return first and last available timestamps
+    # Return first available
     return first_available, last_available
 
 
 def _should_compute_enabled_times(event_log: pd.DataFrame, config: Configuration):
     return config.log_ids.enabled_time not in event_log.columns or (
         config.timer_placement == TimerPlacement.AFTER and config.log_ids.enabling_activity not in event_log.columns
     )
```

### Comparing `extraneous_activity_delays-2.1.16/src/extraneous_activity_delays/enhance_with_delays.py` & `extraneous_activity_delays-2.1.9/src/extraneous_activity_delays/enhance_with_delays.py`

 * *Files 5% similar despite different names*

```diff
@@ -123,59 +123,58 @@
                 self.event_log.copy(),
             )
         self.simulation_model = copy.deepcopy(simulation_model)
         self.configuration = configuration
         self.log_ids = configuration.log_ids
         # Compute extraneous delay timers
         if self.configuration.discovery_method == DiscoveryMethod.NAIVE:
-            self.initial_timers = compute_naive_extraneous_activity_delays(
+            self.timers = compute_naive_extraneous_activity_delays(
                 self.event_log,
                 self.configuration,
                 self.configuration.should_consider_timer,
             )
         elif self.configuration.discovery_method == DiscoveryMethod.COMPLEX:
-            self.initial_timers = compute_complex_extraneous_activity_delays(
+            self.timers = compute_complex_extraneous_activity_delays(
                 self.event_log,
                 self.configuration,
                 self.configuration.should_consider_timer,
             )
         else:
             raise ValueError("Invalid delay discovery method selected!")
         # Hyper-optimization search space
         self.opt_space = {
-            activity: hp.uniform(activity, 0.0, self.configuration.max_alpha) for activity in self.initial_timers.keys()
+            activity: hp.uniform(activity, 0.0, self.configuration.max_alpha) for activity in self.timers.keys()
         }
         baseline_iteration_params = [
-            {activity: 0.0 for activity in self.initial_timers.keys()},  # No timers
-            {activity: 1.0 for activity in self.initial_timers.keys()},  # Discovered timers
+            {activity: 0.0 for activity in self.timers.keys()},  # No timers
+            {activity: 1.0 for activity in self.timers.keys()},  # Discovered timers
         ]
         # Variable to store the information of each optimization trial
         self.opt_trials = generate_trials_to_calculate(
             baseline_iteration_params
         )  # Force the first trial to be with this values
         # Result attributes
         self.best_timers = {}
         self.losses = []
 
     def enhance_simulation_model_with_delays(self) -> SimulationModel:
-        if len(self.initial_timers) > 0:
+        if len(self.timers) > 0:
             # Launch hyper-optimization with the timers
             best_result = fmin(
                 fn=self._enhancement_iteration,
                 space=self.opt_space,
                 algo=tpe.suggest,
                 max_evals=self.configuration.num_iterations,
                 trials=self.opt_trials,
                 show_progressbar=False,
             )
             # Remove all folders except best trial one
-            if self.configuration.clean_intermediate_files:
-                for result in self.opt_trials.results:
-                    if result["output_folder"] != self.opt_trials.best_trial["result"]["output_folder"]:
-                        delete_folder(result["output_folder"])
+            for result in self.opt_trials.results:
+                if result["output_folder"] != self.opt_trials.best_trial["result"]["output_folder"]:
+                    delete_folder(result["output_folder"])
             # Process the best parameters result
             best_alphas = {activity: round(best_result[activity], 2) for activity in best_result}
             # Transform timers based on [best_alphas]
             scaled_timers = self._get_scaled_timers(best_alphas)
             self.best_timers = scaled_timers
             # Enhance process model
             if self.configuration.simulation_engine == SimulationEngine.PROSIMOS:
@@ -346,13 +345,13 @@
                 sim_log_ids,
                 bin_size,
             )
 
     def _get_scaled_timers(self, alphas: dict):
         scaled_timers = {}
         # For each timer
-        for activity in self.initial_timers:
+        for activity in self.timers:
             # If the scaling factor is not 0.0 create a timer
             if (activity in alphas) and (alphas[activity] > 0.0):
-                scaled_timers[activity] = self.initial_timers[activity].scale_distribution(alphas[activity])
+                scaled_timers[activity] = self.timers[activity].scale_distribution(alphas[activity])
         # Return timers
         return scaled_timers
```

### Comparing `extraneous_activity_delays-2.1.16/src/extraneous_activity_delays/prosimos/simulation_model_enhancer.py` & `extraneous_activity_delays-2.1.9/src/extraneous_activity_delays/prosimos/simulation_model_enhancer.py`

 * *Files identical despite different names*

### Comparing `extraneous_activity_delays-2.1.16/src/extraneous_activity_delays/prosimos/simulator.py` & `extraneous_activity_delays-2.1.9/src/extraneous_activity_delays/prosimos/simulator.py`

 * *Files identical despite different names*

### Comparing `extraneous_activity_delays-2.1.16/src/extraneous_activity_delays/qbp/simulation_model_enhancer.py` & `extraneous_activity_delays-2.1.9/src/extraneous_activity_delays/qbp/simulation_model_enhancer.py`

 * *Files identical despite different names*

### Comparing `extraneous_activity_delays-2.1.16/src/extraneous_activity_delays/qbp/simulator.py` & `extraneous_activity_delays-2.1.9/src/extraneous_activity_delays/qbp/simulator.py`

 * *Files identical despite different names*

### Comparing `extraneous_activity_delays-2.1.16/src/extraneous_activity_delays/utils/bpmn_enhancement.py` & `extraneous_activity_delays-2.1.9/src/extraneous_activity_delays/utils/bpmn_enhancement.py`

 * *Files identical despite different names*

### Comparing `extraneous_activity_delays-2.1.16/src/extraneous_activity_delays/utils/file_manager.py` & `extraneous_activity_delays-2.1.9/src/extraneous_activity_delays/utils/file_manager.py`

 * *Files identical despite different names*

### Comparing `extraneous_activity_delays-2.1.16/PKG-INFO` & `extraneous_activity_delays-2.1.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: extraneous-activity-delays
-Version: 2.1.16
+Version: 2.1.9
 Summary: 
 Author: David Chapela de la Campa
 Author-email: david.chapela.delacampa@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: hyperopt (>=0.2.7,<0.3.0)
 Requires-Dist: log-distance-measures (>=1.0.2,<2.0.0)
 Requires-Dist: lxml (>=4.9.2,<5.0.0)
-Requires-Dist: pix-framework (>=0.10.0,<0.11.0)
-Requires-Dist: prosimos (>=1.2.6,<2.0.0)
-Requires-Dist: start-time-estimator (>=1.10.10,<2.0.0)
+Requires-Dist: pix-framework (>=0.8.3,<0.9.0)
+Requires-Dist: prosimos (>=1.2.4,<2.0.0)
+Requires-Dist: start-time-estimator (>=1.10.9,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Extraneous activity delays BPS model enhancer
 
 ![build](https://github.com/AutomatedProcessImprovement/extraneous-activity-delays/actions/workflows/build.yaml/badge.svg)
 ![version](https://img.shields.io/github/v/tag/AutomatedProcessImprovement/extraneous-activity-delays)
```

