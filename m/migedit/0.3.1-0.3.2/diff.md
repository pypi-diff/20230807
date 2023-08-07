# Comparing `tmp/migedit-0.3.1.tar.gz` & `tmp/migedit-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "migedit-0.3.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "migedit-0.3.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `migedit-0.3.1.tar` & `migedit-0.3.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1799 2023-07-27 10:46:05.001162 migedit-0.3.1/.gitignore
--rw-r--r--   0        0        0     1079 2023-07-27 10:46:05.001162 migedit-0.3.1/LICENSE
--rw-r--r--   0        0        0     1269 2023-07-31 13:51:42.491040 migedit-0.3.1/README.md
--rw-r--r--   0        0        0     8902 2023-07-31 13:51:47.059074 migedit-0.3.1/migedit.py
--rw-r--r--   0        0        0      459 2023-07-31 12:28:47.251569 migedit-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     1644 1970-01-01 00:00:00.000000 migedit-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1799 2023-07-27 10:46:05.001162 migedit-0.3.2/.gitignore
+-rw-r--r--   0        0        0     1079 2023-07-27 10:46:05.001162 migedit-0.3.2/LICENSE
+-rw-r--r--   0        0        0     1393 2023-08-07 08:11:37.559628 migedit-0.3.2/README.md
+-rw-r--r--   0        0        0     9357 2023-08-07 08:10:27.063123 migedit-0.3.2/migedit.py
+-rw-r--r--   0        0        0      459 2023-07-31 12:28:47.251569 migedit-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     1768 1970-01-01 00:00:00.000000 migedit-0.3.2/PKG-INFO
```

### Comparing `migedit-0.3.1/.gitignore` & `migedit-0.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `migedit-0.3.1/LICENSE` & `migedit-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `migedit-0.3.1/README.md` & `migedit-0.3.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 `migedit.get_mig_profiles()`
 to get a list of all available MIG instance configurations.
 
 `migedit.make_mig_devices(0, ["1g.10gb"])`
 to remove old MIG instances and create new ones.
 
 # Changelog:'
+- 3.2: Added `remove_mig_devices()`. Empty command will now remove instances only. Added parsing of comma separated values.
 - 3.1: Added `remove_old` flag.
 - 3.0: Support for non-A100 devices (H100, A30, etc.) by dynamically grabbing available profiles.
 - 2.0: Support for Shared Memory Mig Mode (with 7g.40gb instances)
 - 1.1: Various bugfixes
 - 1.0: Initial
 
 ## Supported platforms
```

### Comparing `migedit-0.3.1/migedit.py` & `migedit-0.3.2/migedit.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """MIG Editor. CLI/importable module to automatically delete and create MIG gpu/cpu instances."""
 
-__version__ = "0.3.1"
+__version__ = "0.3.2"
 
 import argparse
 import os
 import re
 import time
 
 from subprocess import Popen, PIPE
@@ -99,22 +99,39 @@
 
     Returns:
         list: Transposed list
     """
     return [list(i) for i in zip(*input_list)]
 
 
+def remove_mig_devices():
+    """Remove all instances.
+
+    Raises:
+        ValueError: Remove instances failed.
+    """    
+    result = "".join(_execute_command(f"sudo nvidia-smi mig -dci")).lower()
+    if "failed" in result or "unable" in result:
+        raise ValueError(result)
+
+    result = "".join(_execute_command(f"sudo nvidia-smi mig -dgi")).lower()
+    if "failed" in result or "unable" in result:
+        raise ValueError(result)
+    time.sleep(1)
+
+
 def make_mig_devices(
     gpu: int,
     profiles: list,
     available_mig: list = [],
     available_smig: list = [],
     remove_old: bool = True,
+    verbose: bool = False,
 ) -> list:
-    """Remove any old MIG instances and create MIG instances on gpu following profiles
+    """Create MIG instances on gpu following profiles and (optionally) remove old instances.
 
     Args:
         gpu (int): GPU instance to create on
         profiles (list): List of profiles to use
         available_mig (list, optional): Available MIG profiles. Automatically retrieves profiles if empty
         available_smig (list, optional): Available shared MIG profiles. Automatically retrieves profiles if empty
         remove_old (bool, optional): Whether to remove old MIG instances. Defaults to True.
@@ -123,33 +140,28 @@
         ValueError: Command failed
 
     Returns:
         list: Allocated MIG instances
 
     """
 
+    # Split commas in profiles
+    profiles = [y for x in profiles for y in x.split(",")]
+
     # Retrieve missing profile availability data
     if (not available_mig) or (not available_smig):
         options_mig, options_smig = get_mig_profiles()
 
         if not available_mig:
             available_mig = options_mig
         if not available_smig:
             available_smig = options_smig
 
-    # Remove old instances
     if remove_old:
-        result = "".join(_execute_command(f"sudo nvidia-smi mig -dci")).lower()
-        if "failed" in result or "unable" in result:
-            raise ValueError(result)
-
-        result = "".join(_execute_command(f"sudo nvidia-smi mig -dgi")).lower()
-        if "failed" in result or "unable" in result:
-            raise ValueError(result)
-        time.sleep(1)
+        remove_mig_devices()
 
     devicetemp = []
 
     # TODO: remove this temp code
     shared_mig_gpui = {}
 
     # This supports Multi-MIG, which doesn't actually work right now
@@ -217,17 +229,18 @@
 
     for index, device, instance, gpu_instance, mig_id in devicetemp:
         while (entity_id := _get_dcgmi_instance_id(device, gpu_instance)) is None:
             time.sleep(
                 0.5
             )  # Wait for the rather slow DCGMI discovery to yield a GPU entity id
 
-        print(
-            f"Device {device}: Allocated {instance} ({gpu_instance}) with entity id ({entity_id}) and UUID ({mig_id})"
-        )
+        if verbose:
+            print(
+                f"Device {device}: Allocated {instance} ({gpu_instance}) with entity id ({entity_id}) and UUID ({mig_id})"
+            )
         results.append((device, instance, gpu_instance, entity_id, mig_id))
 
     return results
 
 
 def get_mig_profiles() -> tuple[dict, dict]:
     """Retrieve all available mig profiles
@@ -291,18 +304,21 @@
         help="ID instance number of the GPU to manage MIG on.",
     )
     parser.add_argument(
         "-p",
         "--profiles",
         metavar="PROFILES",
         nargs="+",
-        help=f"""Space seperated list of MIG profiles to use.\nOptions:\n\t{f"{NEWTAB}".join([f'{k: <3} or {v}' for k,v in (available_mig | available_smig).items()])}""",
-        required=True,
+        help=f"""Space seperated list of MIG profiles to use. Will only remove instances if not specified.\nOptions:\n\t{f"{NEWTAB}".join([f'{k: <3} or {v}' for k,v in (available_mig | available_smig).items()])}""",
     )
 
     args = parser.parse_args()
 
-    make_mig_devices(args.instance, args.profiles, available_mig, available_smig)
+    if args.profiles is not None:
+        make_mig_devices(args.instance, args.profiles, available_mig=available_mig, available_smig=available_smig, verbose=True)
+    else:
+        remove_mig_devices()
+        print("Succesfully removed all MIG instances.")
 
 
 if __name__ == "__main__":
     _cli()
```

### Comparing `migedit-0.3.1/PKG-INFO` & `migedit-0.3.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: migedit
-Version: 0.3.1
+Version: 0.3.2
 Summary: MIG Editor. CLI/importable module to automatically delete and create MIG gpu/cpu instances.
 Author-email: Ties Robroek <migedit@trobroek.com>
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Project-URL: Home, https://github.com/Sipondo/migedit
 
@@ -33,14 +33,15 @@
 `migedit.get_mig_profiles()`
 to get a list of all available MIG instance configurations.
 
 `migedit.make_mig_devices(0, ["1g.10gb"])`
 to remove old MIG instances and create new ones.
 
 # Changelog:'
+- 3.2: Added `remove_mig_devices()`. Empty command will now remove instances only. Added parsing of comma separated values.
 - 3.1: Added `remove_old` flag.
 - 3.0: Support for non-A100 devices (H100, A30, etc.) by dynamically grabbing available profiles.
 - 2.0: Support for Shared Memory Mig Mode (with 7g.40gb instances)
 - 1.1: Various bugfixes
 - 1.0: Initial
 
 ## Supported platforms
```

