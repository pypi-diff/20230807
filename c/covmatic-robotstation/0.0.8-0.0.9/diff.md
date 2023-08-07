# Comparing `tmp/covmatic_robotstation-0.0.8.tar.gz` & `tmp/covmatic_robotstation-0.0.9.tar.gz`

## Comparing `covmatic_robotstation-0.0.8.tar` & `covmatic_robotstation-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 covmatic_robotstation-0.0.8/CHANGELOG.md
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 covmatic_robotstation-0.0.8/protocols/station_robot_execution.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 covmatic_robotstation-0.0.8/src/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 covmatic_robotstation-0.0.8/src/covmatic_robotstation/__init__.py
--rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 covmatic_robotstation-0.0.8/src/covmatic_robotstation/robot.py
--rw-r--r--   0        0        0     3436 2020-02-02 00:00:00.000000 covmatic_robotstation-0.0.8/src/covmatic_robotstation/robot_api.py
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 covmatic_robotstation-0.0.8/src/covmatic_robotstation/robot_station.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 covmatic_robotstation-0.0.8/test/__init__.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 covmatic_robotstation-0.0.8/test/common.py
--rw-r--r--   0        0        0     5867 2020-02-02 00:00:00.000000 covmatic_robotstation-0.0.8/test/test_robot.py
--rw-r--r--   0        0        0     4239 2020-02-02 00:00:00.000000 covmatic_robotstation-0.0.8/test/test_robot_api_http.py
--rw-r--r--   0        0        0     2849 2020-02-02 00:00:00.000000 covmatic_robotstation-0.0.8/test/test_robot_station.py
--rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 covmatic_robotstation-0.0.8/.gitignore
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 covmatic_robotstation-0.0.8/README.md
--rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 covmatic_robotstation-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 covmatic_robotstation-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 covmatic_robotstation-0.0.9/CHANGELOG.md
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 covmatic_robotstation-0.0.9/protocols/station_robot_execution.py
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 covmatic_robotstation-0.0.9/protocols/station_robot_start_at.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 covmatic_robotstation-0.0.9/src/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 covmatic_robotstation-0.0.9/src/covmatic_robotstation/__init__.py
+-rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 covmatic_robotstation-0.0.9/src/covmatic_robotstation/robot.py
+-rw-r--r--   0        0        0     3436 2020-02-02 00:00:00.000000 covmatic_robotstation-0.0.9/src/covmatic_robotstation/robot_api.py
+-rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 covmatic_robotstation-0.0.9/src/covmatic_robotstation/robot_station.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 covmatic_robotstation-0.0.9/test/__init__.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 covmatic_robotstation-0.0.9/test/common.py
+-rw-r--r--   0        0        0     5867 2020-02-02 00:00:00.000000 covmatic_robotstation-0.0.9/test/test_robot.py
+-rw-r--r--   0        0        0     4239 2020-02-02 00:00:00.000000 covmatic_robotstation-0.0.9/test/test_robot_api_http.py
+-rw-r--r--   0        0        0     2849 2020-02-02 00:00:00.000000 covmatic_robotstation-0.0.9/test/test_robot_station.py
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 covmatic_robotstation-0.0.9/.gitignore
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 covmatic_robotstation-0.0.9/README.md
+-rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 covmatic_robotstation-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 covmatic_robotstation-0.0.9/PKG-INFO
```

### Comparing `covmatic_robotstation-0.0.8/CHANGELOG.md` & `covmatic_robotstation-0.0.9/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Covmatic RobotControl
 
+## v0.0.9
+- [RobotStation] Added trash function to pick the plate and drop in the TRASH location
+- [RobotStation] Fixed bug in logs if run_stage was false
+
 ## v0.0.8
 - [RobotStation] Added start_at logic to skip plate transfers if previous stages not run
 - [RobotStation] Added user message for manual transfer if problem requesting robot transfer
 - [API] Added timeout to HTTP requests
 
 ## v0.0.7
```

### Comparing `covmatic_robotstation-0.0.8/protocols/station_robot_execution.py` & `covmatic_robotstation-0.0.9/protocols/station_robot_execution.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
     def _tipracks(self) -> dict:
         return {"_fake_tipracks": "_fake_pipette"}
 
     def body(self):
         self.robot_pick_plate("SLOT1", "TESTPLATE")
         self.robot_drop_plate("SLOT2", "TESTPLATE")
+        self.robot_trash_plate("SLOT1", "TRASHSLOT2", "TRASHPLATE")
 
 
 metadata = {'apiLevel': '2.7'}
 station = FakeStation(ot_name="OTTEST", num_samples=96)
 
 
 def run(ctx):
```

### Comparing `covmatic_robotstation-0.0.8/src/covmatic_robotstation/robot.py` & `covmatic_robotstation-0.0.9/src/covmatic_robotstation/robot.py`

 * *Files identical despite different names*

### Comparing `covmatic_robotstation-0.0.8/src/covmatic_robotstation/robot_api.py` & `covmatic_robotstation-0.0.9/src/covmatic_robotstation/robot_api.py`

 * *Files identical despite different names*

### Comparing `covmatic_robotstation-0.0.8/test/test_robot.py` & `covmatic_robotstation-0.0.9/test/test_robot.py`

 * *Files identical despite different names*

### Comparing `covmatic_robotstation-0.0.8/test/test_robot_api_http.py` & `covmatic_robotstation-0.0.9/test/test_robot_api_http.py`

 * *Files identical despite different names*

### Comparing `covmatic_robotstation-0.0.8/test/test_robot_station.py` & `covmatic_robotstation-0.0.9/test/test_robot_station.py`

 * *Files identical despite different names*

### Comparing `covmatic_robotstation-0.0.8/.gitignore` & `covmatic_robotstation-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `covmatic_robotstation-0.0.8/pyproject.toml` & `covmatic_robotstation-0.0.9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -39,15 +39,18 @@
 [[tool.hatch.envs.test.matrix]]
 python = ["37", "38"]
 
 [tool.hatch.envs.simulate.scripts]
 run = "opentrons_simulate {matrix:protocols} {args}"
 
 [[tool.hatch.envs.simulate.matrix]]
-protocols = ["protocols/station_robot_execution.py"]
+protocols = [
+    "protocols/station_robot_execution.py",
+    "protocols/station_robot_start_at.py"
+]
 
 [tool.coverage.run]
 branch = true
 parallel = true
 omit = [
 ]
```

### Comparing `covmatic_robotstation-0.0.8/PKG-INFO` & `covmatic_robotstation-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: covmatic-robotstation
-Version: 0.0.8
+Version: 0.0.9
 Summary: Extension of a Covmatic Station class that can control a RobotManager instance
 Author-email: Agostino Facotti <agostino.facotti@asst-bergamoest.it>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: covmatic-stations>=2.19.7
```

