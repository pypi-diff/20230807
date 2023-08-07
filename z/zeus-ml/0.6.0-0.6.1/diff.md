# Comparing `tmp/zeus-ml-0.6.0.tar.gz` & `tmp/zeus-ml-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zeus-ml-0.6.0.tar", last modified: Fri Jul 28 20:53:57 2023, max compression
+gzip compressed data, was "zeus-ml-0.6.1.tar", last modified: Mon Aug  7 21:06:50 2023, max compression
```

## Comparing `zeus-ml-0.6.0.tar` & `zeus-ml-0.6.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:53:57.447402 zeus-ml-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-28 20:53:53.000000 zeus-ml-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7352 2023-07-28 20:53:57.447402 zeus-ml-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-07-28 20:53:53.000000 zeus-ml-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-28 20:53:53.000000 zeus-ml-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:53:57.447402 zeus-ml-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-28 20:53:53.000000 zeus-ml-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:53:57.447402 zeus-ml-0.6.0/zeus/
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-28 20:53:53.000000 zeus-ml-0.6.0/zeus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-07-28 20:53:53.000000 zeus-ml-0.6.0/zeus/analyze.py
--rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-07-28 20:53:53.000000 zeus-ml-0.6.0/zeus/callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     6779 2023-07-28 20:53:53.000000 zeus-ml-0.6.0/zeus/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-07-28 20:53:53.000000 zeus-ml-0.6.0/zeus/job.py
--rw-r--r--   0 runner    (1001) docker     (123)    15334 2023-07-28 20:53:53.000000 zeus-ml-0.6.0/zeus/monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:53:57.447402 zeus-ml-0.6.0/zeus/optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-28 20:53:53.000000 zeus-ml-0.6.0/zeus/optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19026 2023-07-28 20:53:53.000000 zeus-ml-0.6.0/zeus/optimizer/power_limit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:53:57.447402 zeus-ml-0.6.0/zeus/policy/
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-28 20:53:53.000000 zeus-ml-0.6.0/zeus/policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-07-28 20:53:53.000000 zeus-ml-0.6.0/zeus/policy/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-07-28 20:53:53.000000 zeus-ml-0.6.0/zeus/policy/mab.py
--rw-r--r--   0 runner    (1001) docker     (123)    19970 2023-07-28 20:53:53.000000 zeus-ml-0.6.0/zeus/policy/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:53:57.447402 zeus-ml-0.6.0/zeus/run/
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-28 20:53:53.000000 zeus-ml-0.6.0/zeus/run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49008 2023-07-28 20:53:53.000000 zeus-ml-0.6.0/zeus/run/dataloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    15157 2023-07-28 20:53:53.000000 zeus-ml-0.6.0/zeus/run/master.py
--rw-r--r--   0 runner    (1001) docker     (123)    36532 2023-07-28 20:53:53.000000 zeus-ml-0.6.0/zeus/simulate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:53:57.447402 zeus-ml-0.6.0/zeus/util/
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-28 20:53:53.000000 zeus-ml-0.6.0/zeus/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-28 20:53:53.000000 zeus-ml-0.6.0/zeus/util/check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-07-28 20:53:53.000000 zeus-ml-0.6.0/zeus/util/framework.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-07-28 20:53:53.000000 zeus-ml-0.6.0/zeus/util/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-28 20:53:53.000000 zeus-ml-0.6.0/zeus/util/lr_scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-07-28 20:53:53.000000 zeus-ml-0.6.0/zeus/util/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     6813 2023-07-28 20:53:53.000000 zeus-ml-0.6.0/zeus/util/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:53:57.447402 zeus-ml-0.6.0/zeus_ml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7352 2023-07-28 20:53:57.000000 zeus-ml-0.6.0/zeus_ml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-28 20:53:57.000000 zeus-ml-0.6.0/zeus_ml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:53:57.000000 zeus-ml-0.6.0/zeus_ml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-28 20:53:57.000000 zeus-ml-0.6.0/zeus_ml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-28 20:53:57.000000 zeus-ml-0.6.0/zeus_ml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:06:50.576103 zeus-ml-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-07 21:06:45.000000 zeus-ml-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7352 2023-08-07 21:06:50.576103 zeus-ml-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-08-07 21:06:45.000000 zeus-ml-0.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-08-07 21:06:45.000000 zeus-ml-0.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 21:06:50.576103 zeus-ml-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-08-07 21:06:45.000000 zeus-ml-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:06:50.572103 zeus-ml-0.6.1/zeus/
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-08-07 21:06:45.000000 zeus-ml-0.6.1/zeus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-08-07 21:06:45.000000 zeus-ml-0.6.1/zeus/analyze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-08-07 21:06:45.000000 zeus-ml-0.6.1/zeus/callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6779 2023-08-07 21:06:45.000000 zeus-ml-0.6.1/zeus/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-08-07 21:06:45.000000 zeus-ml-0.6.1/zeus/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17444 2023-08-07 21:06:45.000000 zeus-ml-0.6.1/zeus/monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:06:50.572103 zeus-ml-0.6.1/zeus/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-08-07 21:06:45.000000 zeus-ml-0.6.1/zeus/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19026 2023-08-07 21:06:45.000000 zeus-ml-0.6.1/zeus/optimizer/power_limit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:06:50.572103 zeus-ml-0.6.1/zeus/policy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-08-07 21:06:45.000000 zeus-ml-0.6.1/zeus/policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-08-07 21:06:45.000000 zeus-ml-0.6.1/zeus/policy/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-08-07 21:06:45.000000 zeus-ml-0.6.1/zeus/policy/mab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19915 2023-08-07 21:06:45.000000 zeus-ml-0.6.1/zeus/policy/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:06:50.572103 zeus-ml-0.6.1/zeus/run/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-08-07 21:06:45.000000 zeus-ml-0.6.1/zeus/run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48992 2023-08-07 21:06:45.000000 zeus-ml-0.6.1/zeus/run/dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15134 2023-08-07 21:06:45.000000 zeus-ml-0.6.1/zeus/run/master.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36532 2023-08-07 21:06:45.000000 zeus-ml-0.6.1/zeus/simulate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:06:50.576103 zeus-ml-0.6.1/zeus/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-08-07 21:06:45.000000 zeus-ml-0.6.1/zeus/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-08-07 21:06:45.000000 zeus-ml-0.6.1/zeus/util/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-08-07 21:06:45.000000 zeus-ml-0.6.1/zeus/util/framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-08-07 21:06:45.000000 zeus-ml-0.6.1/zeus/util/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-08-07 21:06:45.000000 zeus-ml-0.6.1/zeus/util/lr_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-08-07 21:06:45.000000 zeus-ml-0.6.1/zeus/util/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6813 2023-08-07 21:06:45.000000 zeus-ml-0.6.1/zeus/util/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:06:50.576103 zeus-ml-0.6.1/zeus_ml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7352 2023-08-07 21:06:50.000000 zeus-ml-0.6.1/zeus_ml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-08-07 21:06:50.000000 zeus-ml-0.6.1/zeus_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 21:06:50.000000 zeus-ml-0.6.1/zeus_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-08-07 21:06:50.000000 zeus-ml-0.6.1/zeus_ml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-07 21:06:50.000000 zeus-ml-0.6.1/zeus_ml.egg-info/top_level.txt
```

### Comparing `zeus-ml-0.6.0/LICENSE` & `zeus-ml-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zeus-ml-0.6.0/PKG-INFO` & `zeus-ml-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zeus-ml
-Version: 0.6.0
+Version: 0.6.1
 Summary: A framework for deep learning energy measurement and optimization.
 Home-page: https://github.com/SymbioticLab/Zeus
 Author: Jae-Won Chung
 Author-email: jwnchung@umich.edu
 License: Apache-2.0
 Project-URL: Documentation, https://ml.energy/zeus
 Keywords: deep-learning,power,energy,sustainability,mlsys
```

### Comparing `zeus-ml-0.6.0/README.md` & `zeus-ml-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `zeus-ml-0.6.0/pyproject.toml` & `zeus-ml-0.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `zeus-ml-0.6.0/setup.py` & `zeus-ml-0.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     "test": ["pytest==7.3.2", "pytest-mock==3.10.0", "pytest-xdist==3.3.1"],
     "torch": ["torch==2.0.1"],
 }
 extras_require["dev"] = extras_require["lint"] + extras_require["test"] + extras_require["torch"]
 
 setup(
     name="zeus-ml",
-    version="0.6.0",
+    version="0.6.1",
     description="A framework for deep learning energy measurement and optimization.",
     long_description=open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/SymbioticLab/Zeus",
     author="Jae-Won Chung",
     author_email="jwnchung@umich.edu",
     license="Apache-2.0",
```

### Comparing `zeus-ml-0.6.0/zeus/__init__.py` & `zeus-ml-0.6.1/zeus/__init__.py`

 * *Files identical despite different names*

### Comparing `zeus-ml-0.6.0/zeus/analyze.py` & `zeus-ml-0.6.1/zeus/analyze.py`

 * *Files identical despite different names*

### Comparing `zeus-ml-0.6.0/zeus/callback.py` & `zeus-ml-0.6.1/zeus/callback.py`

 * *Files identical despite different names*

### Comparing `zeus-ml-0.6.0/zeus/controller.py` & `zeus-ml-0.6.1/zeus/controller.py`

 * *Files identical despite different names*

### Comparing `zeus-ml-0.6.0/zeus/job.py` & `zeus-ml-0.6.1/zeus/job.py`

 * *Files identical despite different names*

### Comparing `zeus-ml-0.6.0/zeus/monitor.py` & `zeus-ml-0.6.1/zeus/monitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,14 +95,15 @@
         nvml_gpu_indices (`list[int]`): Indices of all the CUDA devices to monitor, from
             NVML/system's perspective.
     """
 
     def __init__(
         self,
         gpu_indices: list[int] | None = None,
+        approx_instant_energy: bool = False,
         monitor_exec: str = "zeus_monitor",
         log_file: str | Path | None = None,
     ) -> None:
         """Instantiate the monitor.
 
         For Volta or newer GPUs, energy consumption is measured very cheaply with the
         `nvmlDeviceGetTotalEnergyConsumption` API. The API is not supported on older
@@ -114,17 +115,27 @@
             gpu_indices: Indices of all the CUDA devices to monitor. Time/Energy measurements
                 will begin and end at the same time for these GPUs (i.e., synchronized).
                 If None, all the GPUs available will be used. `CUDA_VISIBLE_DEVICES`
                 is respected if set, e.g., GPU index `1` passed into `gpu_indices` when
                 `CUDA_VISIBLE_DEVICES=2,3` will be interpreted as CUDA device `3`.
                 `CUDA_VISIBLE_DEVICES`s formatted with comma-separated indices are supported.
                 (Default: `None`)
+            approx_instant_energy: When the execution time of a measurement window is
+                shorter than the NVML energy counter's update period, energy consumption will
+                be shows as zero. In this case, if `approx_instant_energy` is True, the
+                window's energy consumption will be approximated by multiplying the current
+                instantaneous power consumption with the window's execution time. This should
+                be a better estimate than zero, but it's still an approximation.
+                (Default: `False`)
             monitor_exec: Zeus monitor executable. (Default: `"zeus_monitor"`)
             log_file: Path to the log CSV file. If `None`, logging will be disabled.
         """
+        # Save arguments.
+        self.approx_instant_energy = approx_instant_energy
+
         # Initialize NVML.
         pynvml.nvmlInit()
 
         # Sanity check.
         if gpu_indices is not None and not gpu_indices:
             raise ValueError("`gpu_indices` must be None or non-empty.")
 
@@ -250,14 +261,24 @@
         """Check whether the given GPU is Volta or newer."""
         gpu_handle = self.gpu_handles[gpu]
         return (
             pynvml.nvmlDeviceGetArchitecture(gpu_handle)
             >= pynvml.NVML_DEVICE_ARCH_VOLTA
         )
 
+    def _get_instant_power(self) -> tuple[dict[int, float], float]:
+        """Measure the power consumption of all GPUs at the current time."""
+        power_measurement_start_time: float = time.monotonic()
+        power = {
+            i: pynvml.nvmlDeviceGetPowerUsage(h) / 1000.0
+            for i, h in self.gpu_handles.items()
+        }
+        power_measurement_time = time.monotonic() - power_measurement_start_time
+        return power, power_measurement_time
+
     def begin_window(self, key: str, sync_cuda: bool = True) -> None:
         """Begin a new measurement window.
 
         Args:
             key: Unique name of the measurement window.
             sync_cuda: Whether to synchronize CUDA before starting the measurement window.
                 (Default: `True`)
@@ -303,14 +324,24 @@
         """
         # Retrieve the start time and energy consumption of this window.
         try:
             start_time, start_energy = self.measurement_states.pop(key)
         except KeyError:
             raise ValueError(f"Measurement window '{key}' does not exist") from None
 
+        # Take instant power consumption measurements.
+        # This, in theory, is introducing extra NVMLs call in the critical path
+        # even if computation time is not so short. However, it is reasonable to
+        # expect that computation time would be short if the user explicitly
+        # turned on the `approx_instant_energy` option. Calling this function
+        # as early as possible will lead to more accurate energy approximation.
+        power, power_measurement_time = (
+            self._get_instant_power() if self.approx_instant_energy else ({}, 0.0)
+        )
+
         # Call cudaSynchronize to make sure we freeze at the right time.
         if sync_cuda:
             for gpu_index in self.gpu_handles:
                 cuda_sync(gpu_index)
 
         # If the measurement window is cancelled, return an empty Measurement object.
         if cancel:
@@ -331,14 +362,22 @@
             else:
                 energy_consumption[gpu_index] = analyze.energy(
                     self._monitor_log_path(gpu_index),
                     start_time - self.monitor_start_time,
                     end_time - self.monitor_start_time,
                 )
 
+        # Approximate zero energy consumption.
+        if self.approx_instant_energy:
+            for gpu_index in self.gpu_indices:
+                if energy_consumption[gpu_index] == 0.0:
+                    energy_consumption[gpu_index] = power[gpu_index] * (
+                        time_consumption - power_measurement_time
+                    )
+
         self._log(f"Measurement window '{key}' ended.")
 
         # Add to log file.
         if self.log_file is not None:
             self.log_file.write(
                 f"{start_time},{key},{time_consumption},"
                 + ",".join(map(str, energy_consumption.values()))
```

### Comparing `zeus-ml-0.6.0/zeus/optimizer/__init__.py` & `zeus-ml-0.6.1/zeus/optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `zeus-ml-0.6.0/zeus/optimizer/power_limit.py` & `zeus-ml-0.6.1/zeus/optimizer/power_limit.py`

 * *Files identical despite different names*

### Comparing `zeus-ml-0.6.0/zeus/policy/__init__.py` & `zeus-ml-0.6.1/zeus/policy/__init__.py`

 * *Files identical despite different names*

### Comparing `zeus-ml-0.6.0/zeus/policy/interface.py` & `zeus-ml-0.6.1/zeus/policy/interface.py`

 * *Files identical despite different names*

### Comparing `zeus-ml-0.6.0/zeus/policy/mab.py` & `zeus-ml-0.6.1/zeus/policy/mab.py`

 * *Files identical despite different names*

### Comparing `zeus-ml-0.6.0/zeus/policy/optimizer.py` & `zeus-ml-0.6.1/zeus/policy/optimizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,17 +133,15 @@
             arm_rewards = np.array(self.history[job][batch_size])
             variance = np.var(arm_rewards)
             # When there is only one observation for the arm, the variance is zero.
             # NOTE: We might still want to have a pre-determined reward precision here
             #       because sampling from an infinite precision Gaussian distribution
             #       always returns the mean (the observation), and it will hamper
             #       exploration in the early stage.
-            precision = (
-                np.inf if variance == 0.0 else np.reciprocal(variance)
-            )  # ruff: noqa: PLR2004
+            precision = np.inf if variance == 0.0 else np.reciprocal(variance)
             mab = self.mabs[job]
             mab.arm_reward_prec[batch_size] = precision
             mab.fit_arm(batch_size, arm_rewards, reset=True)
             self.mabs[job] = mab
             if self.verbose:
                 arm_rewards_repr = ", ".join([f"{r:.2f}" for r in arm_rewards])
                 self._log(
```

### Comparing `zeus-ml-0.6.0/zeus/run/__init__.py` & `zeus-ml-0.6.1/zeus/run/__init__.py`

 * *Files identical despite different names*

### Comparing `zeus-ml-0.6.0/zeus/run/dataloader.py` & `zeus-ml-0.6.1/zeus/run/dataloader.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 import pynvml
 import torch
 import torch.distributed as dist
 from torch.utils.data import DataLoader
 from torch.utils.data.distributed import DistributedSampler
 
 from zeus.monitor import ZeusMonitor, Measurement
-from zeus.util.check import get_env
+from zeus.util.env import get_env
 from zeus.util.metric import ZeusCostThresholdExceededError, zeus_cost
 from zeus.util.logging import get_logger
 
 
 # JIT profiling states
 NOT_PROFILING = "NOT_PROFILING"
 WARMING_UP = "WARMING_UP"
@@ -953,22 +953,21 @@
         # Cache the dataloader iterator.
         self.iter = super().__iter__()
 
         if self.rank == 0:
             # Push profiling window for the current epoch.
             # Note that both train and eval dataloaders will push one profiling window *separately*.
             self._begin_measurement("__ZeusDataLoader_epoch")
-            # The power limit of the GPU is only changed by the train dataloader.
-            if self._is_train:  # ruff: noqa: SIM102
-                # If we're not profiling, use the steady state power limit.
-                # If we are profiling, the power limit will be set in __next__ with warmup.
-                # Power limit result is already loaded in when initializing the train dataloader,
-                # so we just set the power limit directly.
-                if not self._should_profile:
-                    self._set_gpu_steady_power_limit()
+            # The power limit of the GPU is only changed by the train dataloader (`self._is_train`).
+            # If we're not profiling, use the steady state power limit (`self._should_profile`).
+            # If we are profiling, the power limit will be set in __next__ with warmup.
+            # Power limit result is already loaded in when initializing the train dataloader,
+            # so we just set the power limit directly.
+            if self._is_train and not self._should_profile:
+                self._set_gpu_steady_power_limit()
 
         return self
 
     def __next__(self):
         """Signal the beginning of an iteration."""
         # Update counters.
         self.sample_num += 1
```

### Comparing `zeus-ml-0.6.0/zeus/run/master.py` & `zeus-ml-0.6.1/zeus/run/master.py`

 * *Files 0% similar despite different names*

```diff
@@ -267,15 +267,15 @@
             A list of [`HistoryEntry`][zeus.analyze.HistoryEntry] objects for each job run.
         """
         # Sanity checks
         if job.default_bs is None:
             raise ValueError("You must provide a default batch size for the job.")
         if job.command is None:
             raise ValueError("You must provide a command format string for the job.")
-        if eta_knob < 0.0 or eta_knob > 1.0:  # ruff: noqa: PLR2004
+        if eta_knob < 0.0 or eta_knob > 1.0:
             raise ValueError("eta_knob must be in [0.0, 1.0].")
 
         print(f"[Zeus Master] {job} x {num_recurrence}")
         print(f"[Zeus Master] Batch sizes: {batch_sizes}")
 
         # Copy all internal state so that simulation does not modify any
         # internal state and is deterministic w.r.t. the random seed.
```

### Comparing `zeus-ml-0.6.0/zeus/simulate.py` & `zeus-ml-0.6.1/zeus/simulate.py`

 * *Files identical despite different names*

### Comparing `zeus-ml-0.6.0/zeus/util/__init__.py` & `zeus-ml-0.6.1/zeus/util/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,11 +10,11 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Utility functions and classes."""
 
-from zeus.util.check import get_env
+from zeus.util.env import get_env
 from zeus.util.logging import FileAndConsole
 from zeus.util.lr_scaler import LinearScaler, SquareRootScaler
 from zeus.util.metric import zeus_cost, ZeusCostThresholdExceededError
```

### Comparing `zeus-ml-0.6.0/zeus/util/check.py` & `zeus-ml-0.6.1/zeus/util/env.py`

 * *Files identical despite different names*

### Comparing `zeus-ml-0.6.0/zeus/util/framework.py` & `zeus-ml-0.6.1/zeus/util/framework.py`

 * *Files identical despite different names*

### Comparing `zeus-ml-0.6.0/zeus/util/logging.py` & `zeus-ml-0.6.1/zeus/util/logging.py`

 * *Files identical despite different names*

### Comparing `zeus-ml-0.6.0/zeus/util/lr_scaler.py` & `zeus-ml-0.6.1/zeus/util/lr_scaler.py`

 * *Files identical despite different names*

### Comparing `zeus-ml-0.6.0/zeus/util/metric.py` & `zeus-ml-0.6.1/zeus/util/metric.py`

 * *Files identical despite different names*

### Comparing `zeus-ml-0.6.0/zeus/util/testing.py` & `zeus-ml-0.6.1/zeus/util/testing.py`

 * *Files identical despite different names*

### Comparing `zeus-ml-0.6.0/zeus_ml.egg-info/PKG-INFO` & `zeus-ml-0.6.1/zeus_ml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zeus-ml
-Version: 0.6.0
+Version: 0.6.1
 Summary: A framework for deep learning energy measurement and optimization.
 Home-page: https://github.com/SymbioticLab/Zeus
 Author: Jae-Won Chung
 Author-email: jwnchung@umich.edu
 License: Apache-2.0
 Project-URL: Documentation, https://ml.energy/zeus
 Keywords: deep-learning,power,energy,sustainability,mlsys
```

### Comparing `zeus-ml-0.6.0/zeus_ml.egg-info/SOURCES.txt` & `zeus-ml-0.6.1/zeus_ml.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 zeus/policy/interface.py
 zeus/policy/mab.py
 zeus/policy/optimizer.py
 zeus/run/__init__.py
 zeus/run/dataloader.py
 zeus/run/master.py
 zeus/util/__init__.py
-zeus/util/check.py
+zeus/util/env.py
 zeus/util/framework.py
 zeus/util/logging.py
 zeus/util/lr_scaler.py
 zeus/util/metric.py
 zeus/util/testing.py
 zeus_ml.egg-info/PKG-INFO
 zeus_ml.egg-info/SOURCES.txt
```

