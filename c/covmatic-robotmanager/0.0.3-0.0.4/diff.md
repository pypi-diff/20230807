# Comparing `tmp/covmatic_robotmanager-0.0.3.tar.gz` & `tmp/covmatic_robotmanager-0.0.4.tar.gz`

## Comparing `covmatic_robotmanager-0.0.3.tar` & `covmatic_robotmanager-0.0.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.3/CHANGELOG.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.3/src/__init__.py
--rw-r--r--   0        0        0     2202 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.3/src/covmatic_robotmanager/EvaHelper.py
--rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.3/src/covmatic_robotmanager/EvaLockThread.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.3/src/covmatic_robotmanager/__init__.py
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.3/src/covmatic_robotmanager/api.py
--rw-r--r--   0        0        0     8287 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.3/src/covmatic_robotmanager/calibrator.py
--rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.3/src/covmatic_robotmanager/config.py
--rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.3/src/covmatic_robotmanager/gripper.py
--rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.3/src/covmatic_robotmanager/main.py
--rw-r--r--   0        0        0    13862 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.3/src/covmatic_robotmanager/movement.py
--rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.3/src/covmatic_robotmanager/positions.py
--rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.3/src/covmatic_robotmanager/robot.py
--rw-r--r--   0        0        0     6230 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.3/src/covmatic_robotmanager/robot_manager.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.3/src/covmatic_robotmanager/singleton.py
--rw-r--r--   0        0        0     4785 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.3/src/covmatic_robotmanager/toolpath.py
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.3/src/covmatic_robotmanager/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.3/test/__init__.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.3/test/common.py
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.3/test/test_manager_plate.py
--rw-r--r--   0        0        0     7197 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.3/test/test_robot_manager.py
--rw-r--r--   0        0        0     2859 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.3/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.3/LICENSE
--rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.3/README.md
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.4/CHANGELOG.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.4/src/__init__.py
+-rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.4/src/covmatic_robotmanager/EvaHelper.py
+-rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.4/src/covmatic_robotmanager/EvaLockThread.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.4/src/covmatic_robotmanager/__init__.py
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.4/src/covmatic_robotmanager/api.py
+-rw-r--r--   0        0        0     8304 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.4/src/covmatic_robotmanager/calibrator.py
+-rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.4/src/covmatic_robotmanager/config.py
+-rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.4/src/covmatic_robotmanager/gripper.py
+-rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.4/src/covmatic_robotmanager/main.py
+-rw-r--r--   0        0        0    14010 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.4/src/covmatic_robotmanager/movement.py
+-rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.4/src/covmatic_robotmanager/positions.py
+-rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.4/src/covmatic_robotmanager/robot.py
+-rw-r--r--   0        0        0     8806 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.4/src/covmatic_robotmanager/robot_manager.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.4/src/covmatic_robotmanager/singleton.py
+-rw-r--r--   0        0        0     4800 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.4/src/covmatic_robotmanager/toolpath.py
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.4/src/covmatic_robotmanager/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.4/test/__init__.py
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.4/test/common.py
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.4/test/test_manager_plate.py
+-rw-r--r--   0        0        0     9928 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.4/test/test_robot_manager.py
+-rw-r--r--   0        0        0     2859 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.4/README.md
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 covmatic_robotmanager-0.0.4/PKG-INFO
```

### Comparing `covmatic_robotmanager-0.0.3/src/covmatic_robotmanager/EvaHelper.py` & `covmatic_robotmanager-0.0.4/src/covmatic_robotmanager/EvaHelper.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 from .singleton import Singleton
 
 
 class EvaHelper(Singleton):
     """ This is a singleton class that should help in interfacing
         with Eva robot.
     """
-    _logger = logging.getLogger(__name__)
+    _logger = logging.getLogger("robotmanager.evahelper")
+
     _eva = None
     _eva_lock_manager = None
 
     def connect(self, eva_ip_address, token):
         self._logger.info("Trying to connect to Eva ip {}...".format(eva_ip_address))
         self._eva = Eva(eva_ip_address, token)
         self._logger.info("Connected to Eva!")
```

### Comparing `covmatic_robotmanager-0.0.3/src/covmatic_robotmanager/EvaLockThread.py` & `covmatic_robotmanager-0.0.4/src/covmatic_robotmanager/EvaLockThread.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import time
 
 from evasdk import Eva
 import threading
 
 
 class EvaLockThread(threading.Thread):
-    def __init__(self, eva: Eva, logger=logging.getLogger(__name__), *args, **kwargs):
+    def __init__(self, eva: Eva, logger=logging.getLogger("robotmanager.evalockthread"), *args, **kwargs):
         super(EvaLockThread, self).__init__(*args, **kwargs)
         self._eva = eva
         self._logger = logger
         self._enabled = True
         self._logger.info("Current state: {}".format(self._eva.lock_status()))
         if self.is_eva_locked:
             self._logger.info("Eva is locked, trying to unlock...")
```

### Comparing `covmatic_robotmanager-0.0.3/src/covmatic_robotmanager/api.py` & `covmatic_robotmanager-0.0.4/src/covmatic_robotmanager/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,25 +2,27 @@
 import logging
 
 from flask import request
 from flask_restful import Api, Resource
 from . import __version__
 from .robot_manager import RobotManager
 
+module_logger = logging.getLogger("robotmanager.api")
+
 
 class RobotManagerApi(Api):
     def __init__(self, *args, **kwargs):
         super(RobotManagerApi, self).__init__(*args, **kwargs)
         self._robot_manager = RobotManager()
         self.add_resource(Version, '/version', resource_class_args=(self._robot_manager,))
         self.add_resource(CheckAction, '/action/check/<string:action_id>', resource_class_args=(self._robot_manager,))
         self.add_resource(RequestAction, '/action/<string:action>/<string:machine>/<string:slot>/<string:plate_name>', resource_class_args=(self._robot_manager,))
 
     def shutdown(self):
-        logging.getLogger().info("Api shutdown called")
+        module_logger.info("Api shutdown called")
         self._robot_manager.shutdown()
 
 
 class RobotManagerResource(Resource):
     def __init__(self, robot_manager):
         super().__init__()
         self._robot_manager = robot_manager
```

### Comparing `covmatic_robotmanager-0.0.3/src/covmatic_robotmanager/calibrator.py` & `covmatic_robotmanager-0.0.4/src/covmatic_robotmanager/calibrator.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Config().pull("")
 
 import os
 from .robot_manager import Robot
 import logging
 
 
-logger = logging.getLogger(__name__)
+logger = logging.getLogger("robotmanager.calibrator")
 
 
 class _Getch:
     """Gets a single character from standard input.  Does not echo to the
 screen."""
     def __init__(self):
         try:
```

### Comparing `covmatic_robotmanager-0.0.3/src/covmatic_robotmanager/config.py` & `covmatic_robotmanager-0.0.4/src/covmatic_robotmanager/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,23 +7,29 @@
 import configargparse
 import os
 import logging
 from .singleton import SingletonMeta
 
 
 class Config(argparse.Namespace, metaclass=SingletonMeta):
-    _logger = logging.getLogger(__name__)
+    _logger = logging.getLogger("robotmanager.config")
 
     @classmethod
     def get_base_config_folder(cls):
         config_dir = os.path.join(os.path.expanduser("~"), ".covmatic")
         cls.create_directory(config_dir)
         return config_dir
 
     @classmethod
+    def get_base_log_folder(cls):
+        log_dir = os.path.join(os.path.expanduser("~"), ".covmatic", "log")
+        cls.create_directory(log_dir)
+        return log_dir
+
+    @classmethod
     def get_config_file_path(cls) -> str:
         return os.path.join(cls.get_base_config_folder(), "robotmanager.conf")
 
     @classmethod
     def get_default_positions_file_path(cls) -> str:
         return os.path.join(cls.get_base_config_folder(), "positions.json")
 
@@ -35,14 +41,15 @@
                                           add_config_file_help=True)
         parser.add_argument('-E', '--eva-ip', metavar='address',  required=True, help="Eva hostname or ip address")
         parser.add_argument('-T', '--eva-token', metavar='token', required=True, help="Eva token")
         parser.add_argument('-P', '--port', type=int, metavar="port", default=5000, help="Server port for requests")
         parser.add_argument('--positions-filepath', metavar="path", type=str, default=cls.get_default_positions_file_path(), help="JSON File to save positions data")
         parser.add_argument('--test-only', dest="test_only", action="store_true", help="enable test-only execution")
         parser.add_argument('--debug-mode', dest="debug_mode", action="store_true", help="enable debug mode to show unhandled exceptions.")
+        parser.add_argument('-L', '--log-folder', dest="log_folder", type=str, default=cls.get_base_log_folder(), help="Folder to store logs in")
         return cls.reset(**parser.parse_known_args()[0].__dict__)
 
     @classmethod
     def pull(cls, description):
         if not cls().__dict__:
             cls.parse(description)
         return cls()
```

### Comparing `covmatic_robotmanager-0.0.3/src/covmatic_robotmanager/gripper.py` & `covmatic_robotmanager-0.0.4/src/covmatic_robotmanager/gripper.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from .EvaHelper import EvaHelper
 
 GRIPPER_HAS_PLATE_LOW_THRESHOLD = 1.0
 GRIPPER_HAS_PLATE_HIGH_THRESHOLD = 5.0
 
 
 class EvaGripper:
-    def __init__(self, logger=logging.getLogger(__name__)):
+    def __init__(self, logger=logging.getLogger("robotmanager.evagripper")):
         self._eva = EvaHelper().eva
         self._logger = logger
 
     def open(self):
         with self._eva.lock():
             self._eva.gpio_set("ee_d0", False)
             self._eva.gpio_set("ee_d1", True)
```

### Comparing `covmatic_robotmanager-0.0.3/src/covmatic_robotmanager/movement.py` & `covmatic_robotmanager-0.0.4/src/covmatic_robotmanager/movement.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 
 class MovementException(Exception):
     pass
 
 
 class Movement:
-    def __init__(self, position_filepath: str, logger=logging.getLogger(__name__)):
+    def __init__(self, position_filepath: str, logger=logging.getLogger("robotmanager.movement")):
         self._eva = EvaHelper().eva
         self._positions = Positions(position_filepath)
         self._logger = logger
         self._eva_helper = EvaHelper()
         self._logger.info("Loaded Eva: {}".format(self._eva_helper.get_robot_info()))
 
     def move_to(self, position):
@@ -218,15 +218,15 @@
             tp.add_movement("target_up", "linear", max_speed=max_speed)
             tp.add_movement("target", "linear", max_speed=approach_speed)
 
     def transfer_plate(self, source_pos, dest_pos, max_speed=None, home_after=True, detach_plate=False):
         self.pick_plate(source_pos, max_speed=max_speed, detach_plate=detach_plate, home_after=home_after)
         self.drop_plate(dest_pos, max_speed=max_speed, home_after=home_after)
 
-    def pick_plate(self, source_pos, max_speed=None, detach_plate=False, home_after=True):
+    def pick_plate(self, source_pos, max_speed=None, detach_plate=False, home_after=True, same_machine=False):
 
         gripper = EvaGripper()
 
         near_height = -0.01
         grip_height = 0.008
         approach_speed = 0.025
 
@@ -243,17 +243,15 @@
             self._eva_helper.check_and_clear_errors()
 
         tp = Toolpath(max_speed=max_speed)
         tp.add_waypoint("pick_home", source_home_pos)
         tp.add_waypoint("pick_pos_up", self.get_joints(source_pos, offset={"z": source_raising_height}))
         tp.add_waypoint("pick_pos_near", self.get_joints(source_pos, offset={"z": near_height}))
         tp.add_waypoint("pick_pos", pick_pos)
-
-        if home_after:
-            tp.add_waypoint("home", self.get_joints("HOME"))
+        tp.add_waypoint("home", self.get_joints("HOME"))
 
         gripper.close()
 
         with ToolpathExecute(tp):
             tp.add_movement("pick_home")
             tp.add_movement("pick_pos_up", "linear")
             tp.add_movement("pick_pos_near", "linear")
@@ -278,25 +276,26 @@
             with ToolpathExecute(tp):
                 tp.add_movement("pick_pos_near", )
                 tp.add_movement("pick_pos_up", "linear", max_speed=approach_speed)
             gripper.close()
             with ToolpathExecute(tp):
                 tp.add_movement("pick_pos_up")
                 tp.add_movement("pick_home", "linear")
-
+                tp.add_movement("home")
             raise MovementException("Plate not grabbed!")
 
         with ToolpathExecute(tp):
             tp.add_movement("pick_pos_near")
             tp.add_movement("pick_pos_up", "linear")
-            tp.add_movement("pick_home", "linear")
-            if home_after:
-                tp.add_movement("home")
+            if not same_machine:
+                tp.add_movement("pick_home", "linear")
+                if home_after:
+                    tp.add_movement("home")
 
-    def drop_plate(self, dest_pos, max_speed=None, home_after=True):
+    def drop_plate(self, dest_pos, max_speed=None, home_after=True, same_machine=False):
 
         gripper = EvaGripper()
 
         near_height = -0.01
         grip_height = 0.008
         approach_speed = 0.025
 
@@ -316,15 +315,16 @@
         tp.add_waypoint("drop_pos_near", self.get_joints(dest_pos, offset={"z": near_height}))
         tp.add_waypoint("drop_pos", self.get_joints(dest_pos, offset={"z": grip_height}))
 
         if home_after:
             tp.add_waypoint("home", self.get_joints("HOME"))
 
         with ToolpathExecute(tp):
-            tp.add_movement("drop_home")
+            if not same_machine:
+                tp.add_movement("drop_home")
             tp.add_movement("drop_pos_up", "linear")
             tp.add_movement("drop_pos_near", "linear")
             tp.add_movement("drop_pos", "linear", max_speed=approach_speed)
 
         gripper.open()
 
         with ToolpathExecute(tp):
```

### Comparing `covmatic_robotmanager-0.0.3/src/covmatic_robotmanager/positions.py` & `covmatic_robotmanager-0.0.4/src/covmatic_robotmanager/positions.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 import logging
 
 
 class Positions:
     def __init__(self,
                  positions_file_path: str,
-                 logger=logging.getLogger(__name__)):
+                 logger=logging.getLogger("robotmanager.positions")):
         self._logger = logger
         self._abs_path = os.path.abspath(positions_file_path)
         self._logger.info("Checking path {}...".format(self._abs_path))
 
         if not os.path.exists(self._abs_path):
             raise Exception("Position file passed must exist: {}".format(self._abs_path))
```

### Comparing `covmatic_robotmanager-0.0.3/src/covmatic_robotmanager/robot.py` & `covmatic_robotmanager-0.0.4/src/covmatic_robotmanager/robot.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 
 class RobotException(Exception):
     pass
 
 
 class Robot:
-    def __init__(self, eva_ip_address, token, position_filepath, logger=logging.getLogger(__name__)):
+    def __init__(self, eva_ip_address, token, position_filepath, logger=logging.getLogger("robotmanager.robot")):
         self._logger = logger
         self._eva_helper = EvaHelper()
         self._eva_helper.connect(eva_ip_address, token)
         self._movement = Movement(position_filepath)
 
     def unlock(self):
         self._eva_helper.disconnect()
@@ -35,23 +35,23 @@
     def move_to_position(self, name: str, speed: float = None, offset: dict = None):
         self._logger.info("Moving to position {} with offset: {}".format(name, offset))
         self._movement.go_to_position(name, speed, offset)
 
     def transfer_plate(self, source_pos, dest_pos, max_speed=None, detach_plate=False):
         self._movement.transfer_plate(source_pos, dest_pos, max_speed, detach_plate=detach_plate)
 
-    def pick_up_plate(self, position):
+    def pick_up_plate(self, position, same_machine: bool = False):
         self._logger.info("Requested pickup from {}".format(position))
         try:
-            self._movement.pick_plate(position)
+            self._movement.pick_plate(position, same_machine=same_machine)
         except MovementException as e:
             self._logger.error("Exception during pickup: {}".format(e))
             raise RobotException(str(e))
 
-    def drop_plate(self, position):
+    def drop_plate(self, position, same_machine: bool = False):
         self._logger.info("Requested drop to {}".format(position))
         try:
-            self._movement.drop_plate(position)
+            self._movement.drop_plate(position, same_machine=same_machine)
         except MovementException as e:
             self._logger.error("Exception during pickup: {}".format(e))
             raise RobotException(str(e))
```

### Comparing `covmatic_robotmanager-0.0.3/src/covmatic_robotmanager/robot_manager.py` & `covmatic_robotmanager-0.0.4/src/covmatic_robotmanager/robot_manager.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,160 +1,213 @@
-import concurrent
-from enum import Enum
-from threading import Event, Thread
-
+from threading import Event, Thread, Lock
 from .robot import Robot, RobotException
-from .singleton import Singleton
+from .singleton import SingletonMeta
 from .config import Config
 from queue import Queue
 import logging
 import uuid
 
 
 class RobotManagerException(Exception):
     pass
 
 
-class RobotManager(Singleton):
-    def __init__(self, logger=logging.getLogger(__name__)):
+class RobotManager(metaclass=SingletonMeta):
+    def __init__(self, logger=logging.getLogger("robotmanager.robotmanager"), start_thread: bool = True):
         self._robot = Robot(eva_ip_address=Config().eva_ip,
                             token=Config().eva_token,
                             position_filepath=Config().positions_filepath)
         self._logger = logger
         self._logger.info("RobotManager initilized)")
         self._actions = []
         self._current_plate = None
-        self._actions_queue = Queue()
+        self._pick_drop_same_machine = False
         self._kill_event = Event()
         self._threads = []
-        self.start_threads()
+        self._actions_lock = Lock()
+        self._start_execution_queue = Queue()
+        if start_thread:
+            self.start_threads()
+
+    @property
+    def _pending_actions(self):
+        with self._actions_lock:
+            return list(filter(lambda x: x['state'] == 'pending', self._actions))
 
     def start_threads(self):
         for f in [self.action_processor_thread]:
             th = Thread(target=f, name=f.__name__)
             self._threads.append(th)
             self._logger.info("Starting thread {}".format(th.name))
             th.start()
 
+    @staticmethod
+    def get_position(machine: str, slot: str) -> str:
+        return "{}-{}".format(machine, slot)
+
+    @staticmethod
+    def get_machine_from_position(position: str) -> str:
+        return position.split('-')[0]
+
     def action_request(self, action, machine, slot, plate_name, options=None):
-        position = "{}-{}".format(machine, slot)
+        position = self.get_position(machine, slot)
         self._logger.info("Requested action {} for {} plate {}".format(action, position, plate_name))
         action_id = str(uuid.uuid4())
         action_element = {
             'action': action,
             'position': position,
             'plate_name': plate_name,
             'id': action_id,
+            'state': 'pending'
         }
-        self._actions_queue.put(action_element)
+        if action == "pick" or action == "terminate":
+            self._logger.info("action request adding action in the beginning: {}".format(action_element))
+            with self._actions_lock:
+                self._actions.insert(0, action_element)
+        else:
+            self._logger.info("action request appending action: {}".format(action_element))
+            with self._actions_lock:
+                self._actions.append(action_element)
+        self._start_execution_queue.put(True)
         return action_id
 
     def shutdown(self):
         self._logger.info("Shutdown command received")
         self._kill_event.set()
-        self._actions_queue.put({"action": "terminate"})
+        self.action_request("terminate", "", "", "")
         for th in self._threads:
             self._logger.info("Joining thread {}".format(th.name))
             th.join()
         self._logger.info("Shutdown exiting")
 
     def action_scheduler(self):
-        done_actions = []
-        self._logger.info("Scheduler: actions are {}".format(self._actions))
-
-        pick_plate_names = map(lambda y: y['plate_name'], filter(lambda x: x['action'] == 'pick', self._actions))
-        drop_plate_names = map(lambda y: y['plate_name'], filter(lambda x: x['action'] == 'drop', self._actions))
-        print("pick: {}".format(list(pick_plate_names)))
-        print("drop: {}".format(list(drop_plate_names)))
-
         while True:
-            pick_plate_names = map(lambda y: y['plate_name'], filter(lambda x: x['action'] == 'pick', self._actions))
-            drop_plate_names = map(lambda y: y['plate_name'], filter(lambda x: x['action'] == 'drop', self._actions))
+            pending_actions = self._pending_actions
+            self._logger.info("Scheduler: actions are {}".format(self._actions))
+            self._logger.info("Scheduler: pending actions are {}".format(pending_actions))
+
+            pick_plate_names = list(map(lambda y: y['plate_name'], filter(lambda x: x['action'] == 'pick', pending_actions)))
+            drop_plate_names = list(map(lambda y: y['plate_name'], filter(lambda x: x['action'] == 'drop', pending_actions)))
 
             a = None
+            self._logger.debug("Current plate: {}".format(self._current_plate))
             if self._current_plate is None:         # We can pick a plate
                 for p in pick_plate_names:
                     if p in drop_plate_names:
-                        a = list(filter(lambda x: x['action'] == 'pick' and x['plate_name'] == p, self._actions))[0]
+                        self._logger.debug("Plate {} found in pick and drop.".format(p))
+                        a_pick = list(filter(lambda x: x['action'] == 'pick' and x['plate_name'] == p, pending_actions))[0]
+                        a_drop = list(filter(lambda x: x['action'] == 'drop' and x['plate_name'] == p, pending_actions))[0]
+                        a = a_pick
+
+                        self._pick_drop_same_machine = (self.get_machine_from_position(a_pick['position']) == self.get_machine_from_position(a_drop['position']))
+                        self._logger.debug("Pick drop same machine set to: {}".format(self._pick_drop_same_machine))
                         self._current_plate = p
+
                         break
             else:
                 if self._current_plate in drop_plate_names:
-                    a = list(filter(lambda x: x['action'] == 'drop' and x['plate_name'] == self._current_plate, self._actions))[0]
+                    a = list(filter(lambda x: x['action'] == 'drop' and x['plate_name'] == self._current_plate, pending_actions))[0]
                     self._current_plate = None
 
             if a is None:
                 break
 
             self._logger.info("Scheduler executing action: {}".format(a))
-            self.execute_action(a)
+            try:
+                self.execute_action(a)
 
-            self._logger.info("Removing action {} from list".format(a))
-            self.remove_action(a)
+                self._logger.info("Removing action {} from list".format(a))
+                self.remove_action(a)
 
-            self._logger.debug("Now actions are: {}".format(self._actions))
+            except Exception as e:
+                self._logger.error("handling error {}".format(e))
+                self.handle_error(a)
 
     def execute_action(self, a):
         action = a["action"]
         position = a["position"]
         self._logger.info("Executing action {} position {}".format(action, position))
+        self._logger.info("Pick Drop same machine is: {}".format(self._pick_drop_same_machine))
         try:
             if action == "pick":
-                self._robot.pick_up_plate(position)
+                self._robot.pick_up_plate(position, self._pick_drop_same_machine)
             elif action == "drop":
-                self._robot.drop_plate(position)
+                self._robot.drop_plate(position, self._pick_drop_same_machine)
+                self._pick_drop_same_machine = False
             else:
                 raise RobotManagerException("Action {} not implemented".format(action))
         except RobotException as e:
-            self._logger.error("Error from robot during action: {}".format(e))
-            self.error_handler()
+            raise RobotManagerException("Error during robot action: {}".format(e))
 
     def remove_action(self, action):
-        for a in self._actions:
-            if a['id'] == action['id']:
-                to_delete = a
-                break
-        else:
-            raise RobotManagerException("Action {} not found in action list".format(action))
-
-        self._actions.remove(to_delete)
+        with self._actions_lock:
+            self._actions.remove(action)
 
     def action_processor_thread(self):
-        self._logger.info("Entered action processor thread")
+        self._logger.info("APT Entered action processor thread")
         while not self._kill_event.isSet():
-            self._logger.info("action processor thread waiting for element")
-            new_action = self._actions_queue.get()
-            if new_action['action'] == "terminate":
+            self._start_execution_queue.get()       # Wait for the signal to start
+
+            if self._actions[0]['action'] == "terminate":
+                self._logger.debug("APT Terminate action received")
                 break
-            if new_action['action'] == "pick":
-                self._logger.info("Adding action in the beginning: {}".format(new_action))
-                self._actions.insert(0, new_action)
-            else:
-                self._actions.append(new_action)
-            self._logger.info("action processor thread elaborating element")
+
             self.action_scheduler()
-        self._logger.info("action processor thread exiting")
+        self._logger.info("APT action processor thread exiting")
 
     def check_action(self, action_id):
         self._logger.info("Checking action id {}".format(action_id))
 
-        state = "pending"
-        if self._actions_queue.empty() and self._is_action_finished(action_id):
+        if self._is_action_finished(action_id):
             state = "finished"
+        else:
+            state = self._action_get_state(action_id)
 
         self._logger.info("Action id {} state {}".format(action_id, state))
         return {"state": state}
 
+    def _get_action_with_id(self, action_id):
+        found_action = None
+        with self._actions_lock:
+            for a in self._actions:
+                if a["id"] == action_id:
+                    found_action = a
+
+        if found_action is None:
+            raise RobotManagerException("Action with id {} not found.".format(action_id))
+        return found_action
+
+    def _action_get_state(self, action_id):
+        self._logger.debug("Action get state for id {}".format(action_id))
+        state = self._get_action_with_id(action_id)["state"]
+
+        self._logger.debug("action id {} state {}".format(action_id, state))
+        self._logger.debug("Action get state actions are: {}".format(self._actions))
+        return state
+
     def _is_action_finished(self, action_id):
         """ Check the actions array to know if the action id passed is finished """
-        for a in self._actions:
-            if a["id"] == action_id:
-                return False
-        return True
-
-    def error_handler(self):
-        """ This function should handle error in some way.
-            for now we just set an internal state to avoid unwanted movement """
-        self._logger.info("Error handling function")
-        self._current_plate = "ERROR"
+        try:
+            self._get_action_with_id(action_id)
+            return False
+        except RobotManagerException as e:
+            self._logger.info("Is action id {} finished got expecter error: {}".format(action_id, e))
+            return True
+
+    def handle_error(self, a):
+        """ This function will set the 'aborted' state on the passed action;
+            if the action is 'pick' it will set the 'aborted' state also on linked drop action
+        """
+
+        with self._actions_lock:
+            a['state'] = 'aborted'
+        self._logger.info("Handle error actions are: {}".format(self._actions))
+
+        if a['action'] == 'pick':
+            with self._actions_lock:
+                drop_action = list(filter(lambda x: x['action'] == 'drop' and x['plate_name'] == a['plate_name'], self._actions))[0]
+                self._logger.info("Found drop action to abort: {}".format(drop_action))
+                drop_action['state'] = 'aborted'
+
+        self._current_plate = None
```

### Comparing `covmatic_robotmanager-0.0.3/src/covmatic_robotmanager/singleton.py` & `covmatic_robotmanager-0.0.4/src/covmatic_robotmanager/singleton.py`

 * *Files identical despite different names*

### Comparing `covmatic_robotmanager-0.0.3/src/covmatic_robotmanager/toolpath.py` & `covmatic_robotmanager-0.0.4/src/covmatic_robotmanager/toolpath.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,15 +120,15 @@
         self._logger.debug("Timeline is {}".format(self._timeline))
 
     def clear_movements(self):
         self._timeline = []
 
 
 class ToolpathExecute:
-    def __init__(self, tp: Toolpath, logger=logging.getLogger(__name__)):
+    def __init__(self, tp: Toolpath, logger=logging.getLogger("robotmanager.toolpath")):
         self._eh = EvaHelper()
         self._tp = tp
         self._logger = logger
 
     def __enter__(self) -> Toolpath:
         self._tp.clear_movements()
         return self._tp
```

### Comparing `covmatic_robotmanager-0.0.3/src/covmatic_robotmanager/utils.py` & `covmatic_robotmanager-0.0.4/src/covmatic_robotmanager/utils.py`

 * *Files identical despite different names*

### Comparing `covmatic_robotmanager-0.0.3/test/test_manager_plate.py` & `covmatic_robotmanager-0.0.4/test/test_manager_plate.py`

 * *Files identical despite different names*

### Comparing `covmatic_robotmanager-0.0.3/.gitignore` & `covmatic_robotmanager-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `covmatic_robotmanager-0.0.3/LICENSE` & `covmatic_robotmanager-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `covmatic_robotmanager-0.0.3/README.md` & `covmatic_robotmanager-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `covmatic_robotmanager-0.0.3/pyproject.toml` & `covmatic_robotmanager-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `covmatic_robotmanager-0.0.3/PKG-INFO` & `covmatic_robotmanager-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: covmatic-robotmanager
-Version: 0.0.3
+Version: 0.0.4
 Summary: Covmatic Robot Manager is a robotic arm manager for action requested by other robots
 Author-email: Agostino Facotti <agostino.facotti@asst-bergamoest.it>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

