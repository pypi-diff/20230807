# Comparing `tmp/easyecs-0.7.0.tar.gz` & `tmp/easyecs-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyecs-0.7.0.tar", max compression
+gzip compressed data, was "easyecs-0.7.1.tar", max compression
```

## Comparing `easyecs-0.7.0.tar` & `easyecs-0.7.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     2331 2023-08-06 22:07:12.281604 easyecs-0.7.0/README.md
--rw-r--r--   0        0        0        0 2023-08-06 22:07:12.297604 easyecs-0.7.0/easyecs/__init__.py
--rwxr-xr-x   0        0        0     9052 2023-08-06 22:07:12.297604 easyecs-0.7.0/easyecs/cli.py
--rw-r--r--   0        0        0        0 2023-08-06 22:07:12.301604 easyecs-0.7.0/easyecs/cloudformation/__init__.py
--rw-r--r--   0        0        0       90 2023-08-06 22:07:12.301604 easyecs-0.7.0/easyecs/cloudformation/client.py
--rw-r--r--   0        0        0     3522 2023-08-06 22:07:12.301604 easyecs-0.7.0/easyecs/cloudformation/fetch.py
--rw-r--r--   0        0        0        0 2023-08-06 22:07:12.301604 easyecs-0.7.0/easyecs/cloudformation/stack/__init__.py
--rw-r--r--   0        0        0     1921 2023-08-06 22:07:12.301604 easyecs-0.7.0/easyecs/cloudformation/stack/create.py
--rw-r--r--   0        0        0     1131 2023-08-06 22:07:12.301604 easyecs-0.7.0/easyecs/cloudformation/stack/delete.py
--rw-r--r--   0        0        0     3274 2023-08-06 22:07:12.301604 easyecs-0.7.0/easyecs/cloudformation/stack/update.py
--rw-r--r--   0        0        0     5469 2023-08-06 22:07:12.301604 easyecs-0.7.0/easyecs/cloudformation/template/__init__.py
--rw-r--r--   0        0        0     7426 2023-08-06 22:07:12.301604 easyecs-0.7.0/easyecs/cloudformation/template/task_definition.py
--rw-r--r--   0        0        0    11704 2023-08-06 22:07:12.301604 easyecs-0.7.0/easyecs/command/__init__.py
--rw-r--r--   0        0        0     2188 2023-08-06 22:07:12.301604 easyecs-0.7.0/easyecs/docker/__init__.py
--rw-r--r--   0        0        0        0 2023-08-06 22:07:12.301604 easyecs-0.7.0/easyecs/helpers/__init__.py
--rw-r--r--   0        0        0      264 2023-08-06 22:07:12.301604 easyecs-0.7.0/easyecs/helpers/color.py
--rw-r--r--   0        0        0     2292 2023-08-06 22:07:12.301604 easyecs-0.7.0/easyecs/helpers/common.py
--rw-r--r--   0        0        0     1895 2023-08-06 22:07:12.301604 easyecs-0.7.0/easyecs/helpers/loader.py
--rw-r--r--   0        0        0      531 2023-08-06 22:07:12.301604 easyecs-0.7.0/easyecs/helpers/selector.py
--rw-r--r--   0        0        0     3272 2023-08-06 22:07:12.301604 easyecs-0.7.0/easyecs/helpers/settings.py
--rw-r--r--   0        0        0       42 2023-08-06 22:07:12.301604 easyecs-0.7.0/easyecs/helpers/signal.py
--rw-r--r--   0        0        0     3129 2023-08-06 22:07:12.301604 easyecs-0.7.0/easyecs/model/ecs.py
--rw-r--r--   0        0        0      607 2023-08-06 22:07:12.301604 easyecs-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     3065 1970-01-01 00:00:00.000000 easyecs-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     2331 2023-08-07 07:26:39.699084 easyecs-0.7.1/README.md
+-rw-r--r--   0        0        0        0 2023-08-07 07:26:39.719085 easyecs-0.7.1/easyecs/__init__.py
+-rwxr-xr-x   0        0        0     9052 2023-08-07 07:26:39.719085 easyecs-0.7.1/easyecs/cli.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:26:39.719085 easyecs-0.7.1/easyecs/cloudformation/__init__.py
+-rw-r--r--   0        0        0       90 2023-08-07 07:26:39.719085 easyecs-0.7.1/easyecs/cloudformation/client.py
+-rw-r--r--   0        0        0     3522 2023-08-07 07:26:39.719085 easyecs-0.7.1/easyecs/cloudformation/fetch.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:26:39.719085 easyecs-0.7.1/easyecs/cloudformation/stack/__init__.py
+-rw-r--r--   0        0        0     1921 2023-08-07 07:26:39.719085 easyecs-0.7.1/easyecs/cloudformation/stack/create.py
+-rw-r--r--   0        0        0     1131 2023-08-07 07:26:39.719085 easyecs-0.7.1/easyecs/cloudformation/stack/delete.py
+-rw-r--r--   0        0        0     3274 2023-08-07 07:26:39.719085 easyecs-0.7.1/easyecs/cloudformation/stack/update.py
+-rw-r--r--   0        0        0     5469 2023-08-07 07:26:39.719085 easyecs-0.7.1/easyecs/cloudformation/template/__init__.py
+-rw-r--r--   0        0        0     7430 2023-08-07 07:26:39.719085 easyecs-0.7.1/easyecs/cloudformation/template/task_definition.py
+-rw-r--r--   0        0        0    11908 2023-08-07 07:26:39.719085 easyecs-0.7.1/easyecs/command/__init__.py
+-rw-r--r--   0        0        0     2188 2023-08-07 07:26:39.719085 easyecs-0.7.1/easyecs/docker/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:26:39.719085 easyecs-0.7.1/easyecs/helpers/__init__.py
+-rw-r--r--   0        0        0      264 2023-08-07 07:26:39.719085 easyecs-0.7.1/easyecs/helpers/color.py
+-rw-r--r--   0        0        0     2292 2023-08-07 07:26:39.719085 easyecs-0.7.1/easyecs/helpers/common.py
+-rw-r--r--   0        0        0     1895 2023-08-07 07:26:39.719085 easyecs-0.7.1/easyecs/helpers/loader.py
+-rw-r--r--   0        0        0      531 2023-08-07 07:26:39.719085 easyecs-0.7.1/easyecs/helpers/selector.py
+-rw-r--r--   0        0        0     3272 2023-08-07 07:26:39.719085 easyecs-0.7.1/easyecs/helpers/settings.py
+-rw-r--r--   0        0        0       42 2023-08-07 07:26:39.719085 easyecs-0.7.1/easyecs/helpers/signal.py
+-rw-r--r--   0        0        0     3129 2023-08-07 07:26:39.719085 easyecs-0.7.1/easyecs/model/ecs.py
+-rw-r--r--   0        0        0      607 2023-08-07 07:26:39.719085 easyecs-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     3065 1970-01-01 00:00:00.000000 easyecs-0.7.1/PKG-INFO
```

### Comparing `easyecs-0.7.0/README.md` & `easyecs-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `easyecs-0.7.0/easyecs/cli.py` & `easyecs-0.7.1/easyecs/cli.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.7.0/easyecs/cloudformation/fetch.py` & `easyecs-0.7.1/easyecs/cloudformation/fetch.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.7.0/easyecs/cloudformation/stack/create.py` & `easyecs-0.7.1/easyecs/cloudformation/stack/create.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.7.0/easyecs/cloudformation/stack/delete.py` & `easyecs-0.7.1/easyecs/cloudformation/stack/delete.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.7.0/easyecs/cloudformation/stack/update.py` & `easyecs-0.7.1/easyecs/cloudformation/stack/update.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.7.0/easyecs/cloudformation/template/__init__.py` & `easyecs-0.7.1/easyecs/cloudformation/template/__init__.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.7.0/easyecs/cloudformation/template/task_definition.py` & `easyecs-0.7.1/easyecs/cloudformation/template/task_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
 def add_volumes_to_task_definition(task_definition, ecs_data):
     from aws_cdk.aws_ecs import (
         EfsVolumeConfiguration,
     )
 
     """Add EFS volumes to the task definition."""
-    for volume in ecs_data.task_definition.volumes:
+    for volume in ecs_data.task_definition.efs_volumes:
         efs_volume_configuration = EfsVolumeConfiguration(file_system_id=volume.id)
         task_definition.add_volume(
             name=volume.name, efs_volume_configuration=efs_volume_configuration
         )
 
 
 def add_containers_to_task_definition(
```

### Comparing `easyecs-0.7.0/easyecs/command/__init__.py` & `easyecs-0.7.1/easyecs/command/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,20 +111,24 @@
             input_dirname = dirname(input)
             output_dirname = dirname(output)
             i = inotify.adapters.InotifyTree(input_dirname)
             events = i.event_gen(yield_nones=False, timeout_s=0.1)
             for event in events:
                 (_, type_names, path, filename) = event
                 if set(type_names).issubset(sync_events):
+                    if input_dirname.startswith("/"):
+                        cmd_input_dirname = input_dirname[1:]
+                    else:
+                        cmd_input_dirname = input_dirname
                     tar_cmd = [
                         "tar",
                         "-czvf",
                         "-",
                         input,
-                        f"--transform=s,{input_dirname}/,{output_dirname}/,",
+                        f"--transform=s,{cmd_input_dirname}/,{output_dirname}/,",
                     ]
                     proc_tar_local = subprocess.run(
                         tar_cmd,
                         start_new_session=True,
                         check=True,
                         capture_output=True,
                     )
```

### Comparing `easyecs-0.7.0/easyecs/docker/__init__.py` & `easyecs-0.7.1/easyecs/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.7.0/easyecs/helpers/common.py` & `easyecs-0.7.1/easyecs/helpers/common.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.7.0/easyecs/helpers/loader.py` & `easyecs-0.7.1/easyecs/helpers/loader.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.7.0/easyecs/helpers/selector.py` & `easyecs-0.7.1/easyecs/helpers/selector.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.7.0/easyecs/helpers/settings.py` & `easyecs-0.7.1/easyecs/helpers/settings.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.7.0/easyecs/model/ecs.py` & `easyecs-0.7.1/easyecs/model/ecs.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.7.0/pyproject.toml` & `easyecs-0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "easyecs"
-version = "0.7.0"
+version = "0.7.1"
 description = ""
 authors = ["BONVARLET Benjamin <benjaminbonvarlet96@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 click = "^8.1.6"
```

### Comparing `easyecs-0.7.0/PKG-INFO` & `easyecs-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyecs
-Version: 0.7.0
+Version: 0.7.1
 Summary: 
 Author: BONVARLET Benjamin
 Author-email: benjaminbonvarlet96@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

