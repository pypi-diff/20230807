# Comparing `tmp/bpy_addon_build-0.2.0.tar.gz` & `tmp/bpy_addon_build-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bpy_addon_build-0.2.0.tar", max compression
+gzip compressed data, was "bpy_addon_build-0.2.1.tar", max compression
```

## Comparing `bpy_addon_build-0.2.0.tar` & `bpy_addon_build-0.2.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     5351 2023-07-25 22:14:33.854613 bpy_addon_build-0.2.0/bpy_addon_build/__init__.py
--rw-r--r--   0        0        0     1644 2023-07-24 22:05:51.530691 bpy_addon_build-0.2.0/bpy_addon_build/actions.py
--rw-r--r--   0        0        0     1021 2023-07-24 22:05:51.530691 bpy_addon_build-0.2.0/bpy_addon_build/yaml_conf.py
--rw-r--r--   0        0        0      548 2023-07-25 22:16:13.648344 bpy_addon_build-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      730 1970-01-01 00:00:00.000000 bpy_addon_build-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     5451 2023-08-07 10:58:27.084731 bpy_addon_build-0.2.1/bpy_addon_build/__init__.py
+-rw-r--r--   0        0        0     1644 2023-08-07 10:39:22.221551 bpy_addon_build-0.2.1/bpy_addon_build/actions.py
+-rw-r--r--   0        0        0     1021 2023-08-07 10:39:22.221551 bpy_addon_build-0.2.1/bpy_addon_build/yaml_conf.py
+-rw-r--r--   0        0        0      548 2023-08-07 10:58:42.405533 bpy_addon_build-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      730 1970-01-01 00:00:00.000000 bpy_addon_build-0.2.1/PKG-INFO
```

### Comparing `bpy_addon_build-0.2.0/bpy_addon_build/__init__.py` & `bpy_addon_build-0.2.1/bpy_addon_build/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,26 +18,25 @@
     "~/Library/Application Support/Blender/{0}/scripts/addons",
     "~/.config/blender/{0}/scripts/addons",
 ]
 
 # Rich console
 console = Console()
 
-
 USAGE = """
 Usage:
     bpy-addon-build (-h | --help)
     bpy-addon-build ((-b | --during-build) <action>) [<file>]
     bpy-addon-build [<file>] [((-b | --during-build) <action>)] ((-v | --versions) <versions>...)
     bpy-addon-build [<file>]
 
 Options:
-  -h --help     Show this screen.
-  -b --during-build      Execute a set of actions in addition to the default action
-  -v 
+    (-h | --help)                     Show this screen.
+    (-b | --during-build) <action>    Execute a set of actions in addition to the default action
+    (-v | --versions) <versions>...   Install to the specified versions
 """
 
 
 # Parse a file from a Path
 def parse_file(file: Path) -> yaml_conf.BpyBuildYaml:
     with open(file, "r") as f:
         yaml_config: yaml_conf.BpyBuildYaml = yaml_conf.BpyBuildYaml(f, file)
```

### Comparing `bpy_addon_build-0.2.0/bpy_addon_build/actions.py` & `bpy_addon_build-0.2.1/bpy_addon_build/actions.py`

 * *Files identical despite different names*

### Comparing `bpy_addon_build-0.2.0/bpy_addon_build/yaml_conf.py` & `bpy_addon_build-0.2.1/bpy_addon_build/yaml_conf.py`

 * *Files identical despite different names*

### Comparing `bpy_addon_build-0.2.0/pyproject.toml` & `bpy_addon_build-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bpy-addon-build"
-version = "0.2.0"
+version = "0.2.1"
 description = "A build system to make building and testing Blender addons 10 times easier"
 authors = ["StandingPad"]
 license = "MIT"
 homepage = "https://github.com/StandingPadAnimations/bpy-build"
 
 [tool.poetry.dependencies]
 python = "^3.7"
```

### Comparing `bpy_addon_build-0.2.0/PKG-INFO` & `bpy_addon_build-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bpy-addon-build
-Version: 0.2.0
+Version: 0.2.1
 Summary: A build system to make building and testing Blender addons 10 times easier
 Home-page: https://github.com/StandingPadAnimations/bpy-build
 License: MIT
 Author: StandingPad
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

