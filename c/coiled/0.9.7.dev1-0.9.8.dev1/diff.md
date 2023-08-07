# Comparing `tmp/coiled-0.9.7.dev1.tar.gz` & `tmp/coiled-0.9.8.dev1.tar.gz`

## Comparing `coiled-0.9.7.dev1.tar` & `coiled-0.9.8.dev1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 coiled-0.9.7.dev1/coiled/__init__.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 coiled-0.9.7.dev1/coiled/_version.py
--rw-r--r--   0        0        0     7539 2020-02-02 00:00:00.000000 coiled-0.9.7.dev1/coiled/analytics.py
--rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 coiled-0.9.7.dev1/coiled/auth.py
--rw-r--r--   0        0        0    25266 2020-02-02 00:00:00.000000 coiled-0.9.7.dev1/coiled/capture_environment.py
--rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 coiled-0.9.7.dev1/coiled/cluster.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 coiled-0.9.7.dev1/coiled/coiled.yaml
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 coiled-0.9.7.dev1/coiled/compatibility.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 coiled-0.9.7.dev1/coiled/config.py
--rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 coiled-0.9.7.dev1/coiled/context.py
--rw-r--r--   0        0        0   102304 2020-02-02 00:00:00.000000 coiled-0.9.7.dev1/coiled/core.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 coiled-0.9.7.dev1/coiled/errors.py
--rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 coiled-0.9.7.dev1/coiled/exceptions.py
--rw-r--r--   0        0        0     8932 2020-02-02 00:00:00.000000 coiled-0.9.7.dev1/coiled/function.py
--rw-r--r--   0        0        0    20192 2020-02-02 00:00:00.000000 coiled-0.9.7.dev1/coiled/scan.py
--rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 coiled-0.9.7.dev1/coiled/shutdown.py
--rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 coiled-0.9.7.dev1/coiled/software.py
--rw-r--r--   0        0        0     9203 2020-02-02 00:00:00.000000 coiled-0.9.7.dev1/coiled/types.py
--rw-r--r--   0        0        0    56920 2020-02-02 00:00:00.000000 coiled-0.9.7.dev1/coiled/utils.py
--rw-r--r--   0        0        0     7986 2020-02-02 00:00:00.000000 coiled-0.9.7.dev1/coiled/websockets.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.9.7.dev1/coiled/cli/__init__.py
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 coiled-0.9.7.dev1/coiled/cli/config.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 coiled-0.9.7.dev1/coiled/cli/core.py
--rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 coiled-0.9.7.dev1/coiled/cli/curl.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 coiled-0.9.7.dev1/coiled/cli/diagnostics.py
--rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 coiled-0.9.7.dev1/coiled/cli/env.py
--rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 coiled-0.9.7.dev1/coiled/cli/login.py
--rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 coiled-0.9.7.dev1/coiled/cli/package_sync.py
--rw-r--r--   0        0        0     8699 2020-02-02 00:00:00.000000 coiled-0.9.7.dev1/coiled/cli/prefect.py
--rw-r--r--   0        0        0     7359 2020-02-02 00:00:00.000000 coiled-0.9.7.dev1/coiled/cli/run.py
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 coiled-0.9.7.dev1/coiled/cli/utils.py
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 coiled-0.9.7.dev1/coiled/cli/cluster/__init__.py
--rw-r--r--   0        0        0    13823 2020-02-02 00:00:00.000000 coiled-0.9.7.dev1/coiled/cli/cluster/better_logs.py
--rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 coiled-0.9.7.dev1/coiled/cli/cluster/logs.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 coiled-0.9.7.dev1/coiled/cli/cluster/metrics.py
--rw-r--r--   0        0        0     5799 2020-02-02 00:00:00.000000 coiled-0.9.7.dev1/coiled/cli/cluster/ssh.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 coiled-0.9.7.dev1/coiled/cli/cluster/utils.py
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 coiled-0.9.7.dev1/coiled/cli/notebook/__init__.py
--rw-r--r--   0        0        0    15422 2020-02-02 00:00:00.000000 coiled-0.9.7.dev1/coiled/cli/notebook/notebook.py
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 coiled-0.9.7.dev1/coiled/cli/setup/__init__.py
--rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 coiled-0.9.7.dev1/coiled/cli/setup/amp.py
--rw-r--r--   0        0        0    49135 2020-02-02 00:00:00.000000 coiled-0.9.7.dev1/coiled/cli/setup/aws.py
--rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 coiled-0.9.7.dev1/coiled/cli/setup/entry.py
--rw-r--r--   0        0        0    27132 2020-02-02 00:00:00.000000 coiled-0.9.7.dev1/coiled/cli/setup/gcp.py
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 coiled-0.9.7.dev1/coiled/cli/setup/prometheus.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 coiled-0.9.7.dev1/coiled/cli/setup/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.9.7.dev1/coiled/extensions/__init__.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 coiled-0.9.7.dev1/coiled/extensions/prefect/__init__.py
--rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 coiled-0.9.7.dev1/coiled/extensions/prefect/runners.py
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 coiled-0.9.7.dev1/coiled/extensions/prefect/workers.py
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 coiled-0.9.7.dev1/coiled/v2/__init__.py
--rw-r--r--   0        0        0   100342 2020-02-02 00:00:00.000000 coiled-0.9.7.dev1/coiled/v2/cluster.py
--rw-r--r--   0        0        0    59198 2020-02-02 00:00:00.000000 coiled-0.9.7.dev1/coiled/v2/core.py
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 coiled-0.9.7.dev1/coiled/v2/cwi_log_link.py
--rw-r--r--   0        0        0     8570 2020-02-02 00:00:00.000000 coiled-0.9.7.dev1/coiled/v2/states.py
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 coiled-0.9.7.dev1/coiled/v2/widgets/__init__.py
--rw-r--r--   0        0        0    16304 2020-02-02 00:00:00.000000 coiled-0.9.7.dev1/coiled/v2/widgets/rich.py
--rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 coiled-0.9.7.dev1/coiled/v2/widgets/util.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 coiled-0.9.7.dev1/.gitignore
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 coiled-0.9.7.dev1/LICENSE
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 coiled-0.9.7.dev1/README.md
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 coiled-0.9.7.dev1/pyproject.toml
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 coiled-0.9.7.dev1/PKG-INFO
+-rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 coiled-0.9.8.dev1/coiled/__init__.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 coiled-0.9.8.dev1/coiled/_version.py
+-rw-r--r--   0        0        0     7539 2020-02-02 00:00:00.000000 coiled-0.9.8.dev1/coiled/analytics.py
+-rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 coiled-0.9.8.dev1/coiled/auth.py
+-rw-r--r--   0        0        0    25266 2020-02-02 00:00:00.000000 coiled-0.9.8.dev1/coiled/capture_environment.py
+-rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 coiled-0.9.8.dev1/coiled/cluster.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 coiled-0.9.8.dev1/coiled/coiled.yaml
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 coiled-0.9.8.dev1/coiled/compatibility.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 coiled-0.9.8.dev1/coiled/config.py
+-rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 coiled-0.9.8.dev1/coiled/context.py
+-rw-r--r--   0        0        0   102304 2020-02-02 00:00:00.000000 coiled-0.9.8.dev1/coiled/core.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 coiled-0.9.8.dev1/coiled/errors.py
+-rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 coiled-0.9.8.dev1/coiled/exceptions.py
+-rw-r--r--   0        0        0     8983 2020-02-02 00:00:00.000000 coiled-0.9.8.dev1/coiled/function.py
+-rw-r--r--   0        0        0    20192 2020-02-02 00:00:00.000000 coiled-0.9.8.dev1/coiled/scan.py
+-rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 coiled-0.9.8.dev1/coiled/shutdown.py
+-rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 coiled-0.9.8.dev1/coiled/software.py
+-rw-r--r--   0        0        0     9203 2020-02-02 00:00:00.000000 coiled-0.9.8.dev1/coiled/types.py
+-rw-r--r--   0        0        0    57526 2020-02-02 00:00:00.000000 coiled-0.9.8.dev1/coiled/utils.py
+-rw-r--r--   0        0        0     7986 2020-02-02 00:00:00.000000 coiled-0.9.8.dev1/coiled/websockets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.9.8.dev1/coiled/cli/__init__.py
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 coiled-0.9.8.dev1/coiled/cli/config.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 coiled-0.9.8.dev1/coiled/cli/core.py
+-rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 coiled-0.9.8.dev1/coiled/cli/curl.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 coiled-0.9.8.dev1/coiled/cli/diagnostics.py
+-rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 coiled-0.9.8.dev1/coiled/cli/env.py
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 coiled-0.9.8.dev1/coiled/cli/login.py
+-rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 coiled-0.9.8.dev1/coiled/cli/package_sync.py
+-rw-r--r--   0        0        0     8699 2020-02-02 00:00:00.000000 coiled-0.9.8.dev1/coiled/cli/prefect.py
+-rw-r--r--   0        0        0     7422 2020-02-02 00:00:00.000000 coiled-0.9.8.dev1/coiled/cli/run.py
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 coiled-0.9.8.dev1/coiled/cli/utils.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 coiled-0.9.8.dev1/coiled/cli/cluster/__init__.py
+-rw-r--r--   0        0        0    13823 2020-02-02 00:00:00.000000 coiled-0.9.8.dev1/coiled/cli/cluster/better_logs.py
+-rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 coiled-0.9.8.dev1/coiled/cli/cluster/logs.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 coiled-0.9.8.dev1/coiled/cli/cluster/metrics.py
+-rw-r--r--   0        0        0     5799 2020-02-02 00:00:00.000000 coiled-0.9.8.dev1/coiled/cli/cluster/ssh.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 coiled-0.9.8.dev1/coiled/cli/cluster/utils.py
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 coiled-0.9.8.dev1/coiled/cli/notebook/__init__.py
+-rw-r--r--   0        0        0    15422 2020-02-02 00:00:00.000000 coiled-0.9.8.dev1/coiled/cli/notebook/notebook.py
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 coiled-0.9.8.dev1/coiled/cli/setup/__init__.py
+-rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 coiled-0.9.8.dev1/coiled/cli/setup/amp.py
+-rw-r--r--   0        0        0    49135 2020-02-02 00:00:00.000000 coiled-0.9.8.dev1/coiled/cli/setup/aws.py
+-rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 coiled-0.9.8.dev1/coiled/cli/setup/entry.py
+-rw-r--r--   0        0        0    27132 2020-02-02 00:00:00.000000 coiled-0.9.8.dev1/coiled/cli/setup/gcp.py
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 coiled-0.9.8.dev1/coiled/cli/setup/prometheus.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 coiled-0.9.8.dev1/coiled/cli/setup/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.9.8.dev1/coiled/extensions/__init__.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 coiled-0.9.8.dev1/coiled/extensions/prefect/__init__.py
+-rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 coiled-0.9.8.dev1/coiled/extensions/prefect/runners.py
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 coiled-0.9.8.dev1/coiled/extensions/prefect/workers.py
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 coiled-0.9.8.dev1/coiled/v2/__init__.py
+-rw-r--r--   0        0        0   100342 2020-02-02 00:00:00.000000 coiled-0.9.8.dev1/coiled/v2/cluster.py
+-rw-r--r--   0        0        0    59198 2020-02-02 00:00:00.000000 coiled-0.9.8.dev1/coiled/v2/core.py
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 coiled-0.9.8.dev1/coiled/v2/cwi_log_link.py
+-rw-r--r--   0        0        0     8570 2020-02-02 00:00:00.000000 coiled-0.9.8.dev1/coiled/v2/states.py
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 coiled-0.9.8.dev1/coiled/v2/widgets/__init__.py
+-rw-r--r--   0        0        0    16304 2020-02-02 00:00:00.000000 coiled-0.9.8.dev1/coiled/v2/widgets/rich.py
+-rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 coiled-0.9.8.dev1/coiled/v2/widgets/util.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 coiled-0.9.8.dev1/.gitignore
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 coiled-0.9.8.dev1/LICENSE
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 coiled-0.9.8.dev1/README.md
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 coiled-0.9.8.dev1/pyproject.toml
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 coiled-0.9.8.dev1/PKG-INFO
```

### Comparing `coiled-0.9.7.dev1/coiled/__init__.py` & `coiled-0.9.8.dev1/coiled/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.7.dev1/coiled/analytics.py` & `coiled-0.9.8.dev1/coiled/analytics.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.7.dev1/coiled/auth.py` & `coiled-0.9.8.dev1/coiled/auth.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.7.dev1/coiled/capture_environment.py` & `coiled-0.9.8.dev1/coiled/capture_environment.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.7.dev1/coiled/cluster.py` & `coiled-0.9.8.dev1/coiled/cluster.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.7.dev1/coiled/coiled.yaml` & `coiled-0.9.8.dev1/coiled/coiled.yaml`

 * *Files identical despite different names*

### Comparing `coiled-0.9.7.dev1/coiled/context.py` & `coiled-0.9.8.dev1/coiled/context.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.7.dev1/coiled/core.py` & `coiled-0.9.8.dev1/coiled/core.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.7.dev1/coiled/exceptions.py` & `coiled-0.9.8.dev1/coiled/exceptions.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.7.dev1/coiled/function.py` & `coiled-0.9.8.dev1/coiled/function.py`

 * *Files 1% similar despite different names*

```diff
@@ -216,17 +216,18 @@
     >>> futures = [f(i) for i in range(1000)]  # parallelize with a for loop
     >>> [future.result() for future in futures]
     ...
     """
 
     def decorator(func) -> Function:
         nonlocal cpu
-        environ = None
+
+        environ = coiled.utils.unset_single_thread_defaults()
         if container and "rapidsai" in container:
-            environ = {"DISABLE_JUPYTER": "true"}  # needed for "stable" RAPIDS image
+            environ = {"DISABLE_JUPYTER": "true", **environ}  # needed for "stable" RAPIDS image
 
         if memory is None and cpu is None and not vm_type:
             cpu = 2
 
         cluster_kwargs = dict(
             account=account,
             n_workers=0,
```

### Comparing `coiled-0.9.7.dev1/coiled/scan.py` & `coiled-0.9.8.dev1/coiled/scan.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.7.dev1/coiled/shutdown.py` & `coiled-0.9.8.dev1/coiled/shutdown.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.7.dev1/coiled/software.py` & `coiled-0.9.8.dev1/coiled/software.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.7.dev1/coiled/types.py` & `coiled-0.9.8.dev1/coiled/types.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.7.dev1/coiled/utils.py` & `coiled-0.9.8.dev1/coiled/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1615,7 +1615,21 @@
         try:
             if error.__traceback__:
                 loc["error_filename"] = error.__traceback__.tb_next.tb_next.tb_frame.f_code.co_filename  # type: ignore
                 loc["error_line"] = str(error.__traceback__.tb_next.tb_next.tb_frame.f_lineno)  # type: ignore
         except Exception:
             pass
     return loc
+
+
+def unset_single_thread_defaults() -> dict:
+    """
+    Returns the env vars required to unset the default pre-spawn config that makes certain libraries
+    run in single-thread mode.
+    """
+    env = {}
+    # there are libraries that distributed by default sets to be single-threaded
+    # we want to unset these default values since we're running single task on a (potentially) big machine
+    for key in ("OMP_NUM_THREADS", "MKL_NUM_THREADS", "OPENBLAS_NUM_THREADS"):
+        if dask.config.get(f"distributed.nanny.pre-spawn-environ.{key}", 1) == 1:
+            env = {key: "", **env}
+    return env
```

### Comparing `coiled-0.9.7.dev1/coiled/websockets.py` & `coiled-0.9.8.dev1/coiled/websockets.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.7.dev1/coiled/cli/config.py` & `coiled-0.9.8.dev1/coiled/cli/config.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.7.dev1/coiled/cli/core.py` & `coiled-0.9.8.dev1/coiled/cli/core.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.7.dev1/coiled/cli/curl.py` & `coiled-0.9.8.dev1/coiled/cli/curl.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.7.dev1/coiled/cli/env.py` & `coiled-0.9.8.dev1/coiled/cli/env.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.7.dev1/coiled/cli/login.py` & `coiled-0.9.8.dev1/coiled/cli/login.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.7.dev1/coiled/cli/package_sync.py` & `coiled-0.9.8.dev1/coiled/cli/package_sync.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.7.dev1/coiled/cli/prefect.py` & `coiled-0.9.8.dev1/coiled/cli/prefect.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.7.dev1/coiled/cli/run.py` & `coiled-0.9.8.dev1/coiled/cli/run.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from dask.utils import parse_timedelta
 from packaging.version import Version
 from rich import print
 
 import coiled
 from coiled.compatibility import DISTRIBUTED_VERSION
 from coiled.core import logger as coiled_logger
-from coiled.utils import error_info_for_tracking
+from coiled.utils import error_info_for_tracking, unset_single_thread_defaults
 
 from ..shutdown import NoClientShutdown
 from .cluster.better_logs import better_logs
 from .utils import CONTEXT_SETTINGS
 
 MINIMUM_DISTRIBUTED_VERSION = Version("2023.6.0")
 
@@ -104,17 +104,17 @@
     if DISTRIBUTED_VERSION < MINIMUM_DISTRIBUTED_VERSION:
         # Relies on scheduler having scratch space, which was added in https://github.com/dask/distributed/pull/7802
         raise RuntimeError(
             f"`coiled run` requires distributed>={MINIMUM_DISTRIBUTED_VERSION} "
             f"(distributed={DISTRIBUTED_VERSION} is installed)"
         )
 
-    env = None
+    env = unset_single_thread_defaults()
     if container and "rapidsai" in container:
-        env = {"DISABLE_JUPYTER": "true"}  # needed for "stable" RAPIDS image
+        env = {"DISABLE_JUPYTER": "true", **env}  # needed for "stable" RAPIDS image
 
     if not command:
         raise ValueError("command must be specified")
 
     keepalive = parse_timedelta(keepalive)
     shutdown_on_close = keepalive is None
```

### Comparing `coiled-0.9.7.dev1/coiled/cli/utils.py` & `coiled-0.9.8.dev1/coiled/cli/utils.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.7.dev1/coiled/cli/cluster/__init__.py` & `coiled-0.9.8.dev1/coiled/cli/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.7.dev1/coiled/cli/cluster/better_logs.py` & `coiled-0.9.8.dev1/coiled/cli/cluster/better_logs.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.7.dev1/coiled/cli/cluster/logs.py` & `coiled-0.9.8.dev1/coiled/cli/cluster/logs.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.7.dev1/coiled/cli/cluster/metrics.py` & `coiled-0.9.8.dev1/coiled/cli/cluster/metrics.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.7.dev1/coiled/cli/cluster/ssh.py` & `coiled-0.9.8.dev1/coiled/cli/cluster/ssh.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.7.dev1/coiled/cli/cluster/utils.py` & `coiled-0.9.8.dev1/coiled/cli/cluster/utils.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.7.dev1/coiled/cli/notebook/__init__.py` & `coiled-0.9.8.dev1/coiled/cli/notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.7.dev1/coiled/cli/notebook/notebook.py` & `coiled-0.9.8.dev1/coiled/cli/notebook/notebook.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.7.dev1/coiled/cli/setup/__init__.py` & `coiled-0.9.8.dev1/coiled/cli/setup/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.7.dev1/coiled/cli/setup/amp.py` & `coiled-0.9.8.dev1/coiled/cli/setup/amp.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.7.dev1/coiled/cli/setup/aws.py` & `coiled-0.9.8.dev1/coiled/cli/setup/aws.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.7.dev1/coiled/cli/setup/entry.py` & `coiled-0.9.8.dev1/coiled/cli/setup/entry.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.7.dev1/coiled/cli/setup/gcp.py` & `coiled-0.9.8.dev1/coiled/cli/setup/gcp.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.7.dev1/coiled/cli/setup/prometheus.py` & `coiled-0.9.8.dev1/coiled/cli/setup/prometheus.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.7.dev1/coiled/extensions/prefect/runners.py` & `coiled-0.9.8.dev1/coiled/extensions/prefect/runners.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.7.dev1/coiled/extensions/prefect/workers.py` & `coiled-0.9.8.dev1/coiled/extensions/prefect/workers.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.7.dev1/coiled/v2/__init__.py` & `coiled-0.9.8.dev1/coiled/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.7.dev1/coiled/v2/cluster.py` & `coiled-0.9.8.dev1/coiled/v2/cluster.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.7.dev1/coiled/v2/core.py` & `coiled-0.9.8.dev1/coiled/v2/core.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.7.dev1/coiled/v2/cwi_log_link.py` & `coiled-0.9.8.dev1/coiled/v2/cwi_log_link.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.7.dev1/coiled/v2/states.py` & `coiled-0.9.8.dev1/coiled/v2/states.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.7.dev1/coiled/v2/widgets/__init__.py` & `coiled-0.9.8.dev1/coiled/v2/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.7.dev1/coiled/v2/widgets/rich.py` & `coiled-0.9.8.dev1/coiled/v2/widgets/rich.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.7.dev1/coiled/v2/widgets/util.py` & `coiled-0.9.8.dev1/coiled/v2/widgets/util.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.7.dev1/README.md` & `coiled-0.9.8.dev1/README.md`

 * *Files identical despite different names*

### Comparing `coiled-0.9.7.dev1/pyproject.toml` & `coiled-0.9.8.dev1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `coiled-0.9.7.dev1/PKG-INFO` & `coiled-0.9.8.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coiled
-Version: 0.9.7.dev1
+Version: 0.9.8.dev1
 Project-URL: Homepage, https://coiled.io
 Maintainer-email: Coiled <info@coiled.io>
 License-File: LICENSE
 Requires-Python: >=3.7
 Requires-Dist: aiohttp
 Requires-Dist: backoff
 Requires-Dist: boto3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: coiled Version: 0.9.7.dev1 Project-URL: Homepage,
+Metadata-Version: 2.1 Name: coiled Version: 0.9.8.dev1 Project-URL: Homepage,
 https://coiled.io Maintainer-email: Coiled
 coiled.io> License-File: LICENSE Requires-Python: >=3.7 Requires-Dist: aiohttp
 Requires-Dist: backoff Requires-Dist: boto3 Requires-Dist: click>=7.1 Requires-
 Dist: dask>=2.23.0 Requires-Dist: distributed>=2.23.0 Requires-Dist: filelock
 Requires-Dist: gilknocker>=0.4.1 Requires-Dist: importlib-metadata Requires-
 Dist: ipywidgets Requires-Dist: jmespath Requires-Dist: jsondiff Requires-Dist:
 packaging Requires-Dist: pip Requires-Dist: pip>=19.3 Requires-Dist:
```

