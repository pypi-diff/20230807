# Comparing `tmp/pvipy-0.4.0.tar.gz` & `tmp/pvipy-0.5.0.tar.gz`

## Comparing `pvipy-0.4.0.tar` & `pvipy-0.5.0.tar`

### file list

```diff
@@ -1,46 +1,54 @@
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 pvipy-0.4.0/whatsnew.txt
--rw-r--r--   0        0        0     3594 2020-02-02 00:00:00.000000 pvipy-0.4.0/examples/basics1.py
--rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 pvipy-0.4.0/examples/browse_for_targets.py
--rw-r--r--   0        0        0     3633 2020-02-02 00:00:00.000000 pvipy-0.4.0/examples/gui1.py
--rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 pvipy-0.4.0/examples/linknode1.py
--rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 pvipy-0.4.0/examples/list_objects1.py
--rw-r--r--   0        0        0     2936 2020-02-02 00:00:00.000000 pvipy-0.4.0/examples/list_objects2.py
--rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 pvipy-0.4.0/examples/list_objects3.py
--rw-r--r--   0        0        0     3180 2020-02-02 00:00:00.000000 pvipy-0.4.0/examples/list_objects4.py
--rw-r--r--   0        0        0     2928 2020-02-02 00:00:00.000000 pvipy-0.4.0/examples/list_objects5.py
--rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 pvipy-0.4.0/examples/list_objects6.py
--rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 pvipy-0.4.0/examples/logger1.py
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 pvipy-0.4.0/examples/logger2.py
--rw-r--r--   0        0        0     2461 2020-02-02 00:00:00.000000 pvipy-0.4.0/examples/logger3.py
--rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 pvipy-0.4.0/examples/modules1.py
--rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 pvipy-0.4.0/examples/modules2.py
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 pvipy-0.4.0/examples/modules3.py
--rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 pvipy-0.4.0/examples/set_ip_address.py
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 pvipy-0.4.0/examples/simple1.py
--rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 pvipy-0.4.0/examples/simple2.py
--rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 pvipy-0.4.0/examples/simple3.py
--rw-r--r--   0        0        0    11572 2020-02-02 00:00:00.000000 pvipy-0.4.0/pvi/Connection.py
--rw-r--r--   0        0        0     8505 2020-02-02 00:00:00.000000 pvipy-0.4.0/pvi/Cpu.py
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 pvipy-0.4.0/pvi/Device.py
--rw-r--r--   0        0        0   108627 2020-02-02 00:00:00.000000 pvipy-0.4.0/pvi/Error.py
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 pvipy-0.4.0/pvi/Line.py
--rw-r--r--   0        0        0    10176 2020-02-02 00:00:00.000000 pvipy-0.4.0/pvi/Module.py
--rw-r--r--   0        0        0     8597 2020-02-02 00:00:00.000000 pvipy-0.4.0/pvi/Object.py
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 pvipy-0.4.0/pvi/Station.py
--rw-r--r--   0        0        0     3200 2020-02-02 00:00:00.000000 pvipy-0.4.0/pvi/Task.py
--rw-r--r--   0        0        0     5925 2020-02-02 00:00:00.000000 pvipy-0.4.0/pvi/Variable.py
--rw-r--r--   0        0        0    16722 2020-02-02 00:00:00.000000 pvipy-0.4.0/pvi/VariableType.py
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 pvipy-0.4.0/pvi/__init__.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 pvipy-0.4.0/pvi/include/__init__.py
--rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 pvipy-0.4.0/pvi/include/common_h.py
--rw-r--r--   0        0        0    16521 2020-02-02 00:00:00.000000 pvipy-0.4.0/pvi/include/pvi_h.py
--rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 pvipy-0.4.0/pvi/utils/BrDataObjectFile.py
--rw-r--r--   0        0        0     2732 2020-02-02 00:00:00.000000 pvipy-0.4.0/pvi/utils/BrFile.py
--rw-r--r--   0        0        0     7554 2020-02-02 00:00:00.000000 pvipy-0.4.0/pvi/utils/BrLoggerFile.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 pvipy-0.4.0/pvi/utils/__init__.py
--rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 pvipy-0.4.0/tests/test1.py
--rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 pvipy-0.4.0/.gitignore
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 pvipy-0.4.0/LICENSE
--rw-r--r--   0        0        0     6223 2020-02-02 00:00:00.000000 pvipy-0.4.0/README.md
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 pvipy-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     6607 2020-02-02 00:00:00.000000 pvipy-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 pvipy-0.5.0/whatsnew.txt
+-rw-r--r--   0        0        0     3594 2020-02-02 00:00:00.000000 pvipy-0.5.0/examples/basics1.py
+-rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 pvipy-0.5.0/examples/browse_for_targets.py
+-rw-r--r--   0        0        0     3633 2020-02-02 00:00:00.000000 pvipy-0.5.0/examples/gui1.py
+-rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 pvipy-0.5.0/examples/linknode1.py
+-rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 pvipy-0.5.0/examples/list_objects1.py
+-rw-r--r--   0        0        0     2936 2020-02-02 00:00:00.000000 pvipy-0.5.0/examples/list_objects2.py
+-rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 pvipy-0.5.0/examples/list_objects3.py
+-rw-r--r--   0        0        0     3180 2020-02-02 00:00:00.000000 pvipy-0.5.0/examples/list_objects4.py
+-rw-r--r--   0        0        0     2928 2020-02-02 00:00:00.000000 pvipy-0.5.0/examples/list_objects5.py
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 pvipy-0.5.0/examples/list_objects6.py
+-rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 pvipy-0.5.0/examples/logger1.py
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 pvipy-0.5.0/examples/logger2.py
+-rw-r--r--   0        0        0     2461 2020-02-02 00:00:00.000000 pvipy-0.5.0/examples/logger3.py
+-rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 pvipy-0.5.0/examples/modules1.py
+-rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 pvipy-0.5.0/examples/modules2.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 pvipy-0.5.0/examples/modules3.py
+-rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 pvipy-0.5.0/examples/profiler1.py
+-rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 pvipy-0.5.0/examples/profiler2.py
+-rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 pvipy-0.5.0/examples/set_ip_address.py
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 pvipy-0.5.0/examples/simple1.py
+-rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 pvipy-0.5.0/examples/simple2.py
+-rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 pvipy-0.5.0/examples/simple3.py
+-rw-r--r--   0        0        0    11572 2020-02-02 00:00:00.000000 pvipy-0.5.0/pvi/Connection.py
+-rw-r--r--   0        0        0     8505 2020-02-02 00:00:00.000000 pvipy-0.5.0/pvi/Cpu.py
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 pvipy-0.5.0/pvi/Device.py
+-rw-r--r--   0        0        0   108627 2020-02-02 00:00:00.000000 pvipy-0.5.0/pvi/Error.py
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 pvipy-0.5.0/pvi/Line.py
+-rw-r--r--   0        0        0    10176 2020-02-02 00:00:00.000000 pvipy-0.5.0/pvi/Module.py
+-rw-r--r--   0        0        0     8597 2020-02-02 00:00:00.000000 pvipy-0.5.0/pvi/Object.py
+-rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 pvipy-0.5.0/pvi/Station.py
+-rw-r--r--   0        0        0     3200 2020-02-02 00:00:00.000000 pvipy-0.5.0/pvi/Task.py
+-rw-r--r--   0        0        0     5925 2020-02-02 00:00:00.000000 pvipy-0.5.0/pvi/Variable.py
+-rw-r--r--   0        0        0    16722 2020-02-02 00:00:00.000000 pvipy-0.5.0/pvi/VariableType.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pvipy-0.5.0/pvi/__about__.py
+-rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 pvipy-0.5.0/pvi/__init__.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 pvipy-0.5.0/pvi/include/__init__.py
+-rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 pvipy-0.5.0/pvi/include/common_h.py
+-rw-r--r--   0        0        0    16521 2020-02-02 00:00:00.000000 pvipy-0.5.0/pvi/include/pvi_h.py
+-rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 pvipy-0.5.0/pvi/utils/BrDataObjectFile.py
+-rw-r--r--   0        0        0     2758 2020-02-02 00:00:00.000000 pvipy-0.5.0/pvi/utils/BrFile.py
+-rw-r--r--   0        0        0     7554 2020-02-02 00:00:00.000000 pvipy-0.5.0/pvi/utils/BrLoggerFile.py
+-rw-r--r--   0        0        0    11906 2020-02-02 00:00:00.000000 pvipy-0.5.0/pvi/utils/BrProfilerDataFile.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 pvipy-0.5.0/pvi/utils/__init__.py
+-rw-r--r--   0        0        0    50144 2020-02-02 00:00:00.000000 pvipy-0.5.0/tests/profiler1.pd
+-rw-r--r--   0        0        0   105564 2020-02-02 00:00:00.000000 pvipy-0.5.0/tests/profiler2.pd
+-rw-r--r--   0        0        0   111216 2020-02-02 00:00:00.000000 pvipy-0.5.0/tests/profiler3.pd
+-rw-r--r--   0        0        0     2473 2020-02-02 00:00:00.000000 pvipy-0.5.0/tests/test1.py
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 pvipy-0.5.0/tests/test2.py
+-rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 pvipy-0.5.0/.gitignore
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 pvipy-0.5.0/LICENSE
+-rw-r--r--   0        0        0     6741 2020-02-02 00:00:00.000000 pvipy-0.5.0/README.md
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 pvipy-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     7113 2020-02-02 00:00:00.000000 pvipy-0.5.0/PKG-INFO
```

### Comparing `pvipy-0.4.0/examples/basics1.py` & `pvipy-0.5.0/examples/basics1.py`

 * *Files identical despite different names*

### Comparing `pvipy-0.4.0/examples/browse_for_targets.py` & `pvipy-0.5.0/examples/browse_for_targets.py`

 * *Files identical despite different names*

### Comparing `pvipy-0.4.0/examples/gui1.py` & `pvipy-0.5.0/examples/gui1.py`

 * *Files identical despite different names*

### Comparing `pvipy-0.4.0/examples/linknode1.py` & `pvipy-0.5.0/examples/linknode1.py`

 * *Files identical despite different names*

### Comparing `pvipy-0.4.0/examples/list_objects1.py` & `pvipy-0.5.0/examples/list_objects1.py`

 * *Files identical despite different names*

### Comparing `pvipy-0.4.0/examples/list_objects2.py` & `pvipy-0.5.0/examples/list_objects2.py`

 * *Files identical despite different names*

### Comparing `pvipy-0.4.0/examples/list_objects3.py` & `pvipy-0.5.0/examples/list_objects3.py`

 * *Files identical despite different names*

### Comparing `pvipy-0.4.0/examples/list_objects4.py` & `pvipy-0.5.0/examples/list_objects4.py`

 * *Files identical despite different names*

### Comparing `pvipy-0.4.0/examples/list_objects5.py` & `pvipy-0.5.0/examples/list_objects5.py`

 * *Files identical despite different names*

### Comparing `pvipy-0.4.0/examples/list_objects6.py` & `pvipy-0.5.0/examples/list_objects6.py`

 * *Files identical despite different names*

### Comparing `pvipy-0.4.0/examples/logger1.py` & `pvipy-0.5.0/examples/logger1.py`

 * *Files identical despite different names*

### Comparing `pvipy-0.4.0/examples/logger2.py` & `pvipy-0.5.0/examples/logger2.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,10 @@
 # logger2.py
 # An example that shows the application possibilities of https://github.com/hilch/Pvi.py
 #
-# PLC counterpart is B&R's 'coffee machine' running on ArSim 
-# as provided with Automation Studio 4.1.17.113 (which
-# can be downloaded free of charge from https://www.br-automation.com)
-#
 # extract all logger from a systemdump container and save them as csv.
 #
 
 import tarfile
 import tempfile
 import os
 import csv
```

### Comparing `pvipy-0.4.0/examples/logger3.py` & `pvipy-0.5.0/examples/logger3.py`

 * *Files identical despite different names*

### Comparing `pvipy-0.4.0/examples/modules1.py` & `pvipy-0.5.0/examples/modules1.py`

 * *Files identical despite different names*

### Comparing `pvipy-0.4.0/examples/modules2.py` & `pvipy-0.5.0/examples/modules2.py`

 * *Files identical despite different names*

### Comparing `pvipy-0.4.0/examples/modules3.py` & `pvipy-0.5.0/examples/modules3.py`

 * *Files identical despite different names*

### Comparing `pvipy-0.4.0/examples/set_ip_address.py` & `pvipy-0.5.0/examples/set_ip_address.py`

 * *Files identical despite different names*

### Comparing `pvipy-0.4.0/examples/simple1.py` & `pvipy-0.5.0/examples/simple1.py`

 * *Files identical despite different names*

### Comparing `pvipy-0.4.0/examples/simple2.py` & `pvipy-0.5.0/examples/simple2.py`

 * *Files identical despite different names*

### Comparing `pvipy-0.4.0/examples/simple3.py` & `pvipy-0.5.0/examples/simple3.py`

 * *Files identical despite different names*

### Comparing `pvipy-0.4.0/pvi/Connection.py` & `pvipy-0.5.0/pvi/Connection.py`

 * *Files identical despite different names*

### Comparing `pvipy-0.4.0/pvi/Cpu.py` & `pvipy-0.5.0/pvi/Cpu.py`

 * *Files identical despite different names*

### Comparing `pvipy-0.4.0/pvi/Device.py` & `pvipy-0.5.0/pvi/Device.py`

 * *Files identical despite different names*

### Comparing `pvipy-0.4.0/pvi/Error.py` & `pvipy-0.5.0/pvi/Error.py`

 * *Files identical despite different names*

### Comparing `pvipy-0.4.0/pvi/Line.py` & `pvipy-0.5.0/pvi/Line.py`

 * *Files identical despite different names*

### Comparing `pvipy-0.4.0/pvi/Module.py` & `pvipy-0.5.0/pvi/Module.py`

 * *Files identical despite different names*

### Comparing `pvipy-0.4.0/pvi/Object.py` & `pvipy-0.5.0/pvi/Object.py`

 * *Files identical despite different names*

### Comparing `pvipy-0.4.0/pvi/Station.py` & `pvipy-0.5.0/pvi/Station.py`

 * *Files identical despite different names*

### Comparing `pvipy-0.4.0/pvi/Task.py` & `pvipy-0.5.0/pvi/Task.py`

 * *Files identical despite different names*

### Comparing `pvipy-0.4.0/pvi/Variable.py` & `pvipy-0.5.0/pvi/Variable.py`

 * *Files identical despite different names*

### Comparing `pvipy-0.4.0/pvi/VariableType.py` & `pvipy-0.5.0/pvi/VariableType.py`

 * *Files identical despite different names*

### Comparing `pvipy-0.4.0/pvi/__init__.py` & `pvipy-0.5.0/pvi/__init__.py`

 * *Files identical despite different names*

### Comparing `pvipy-0.4.0/pvi/include/common_h.py` & `pvipy-0.5.0/pvi/include/common_h.py`

 * *Files identical despite different names*

### Comparing `pvipy-0.4.0/pvi/include/pvi_h.py` & `pvipy-0.5.0/pvi/include/pvi_h.py`

 * *Files identical despite different names*

### Comparing `pvipy-0.4.0/pvi/utils/BrDataObjectFile.py` & `pvipy-0.5.0/pvi/utils/BrDataObjectFile.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 # ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 
 from .BrFile import *
 
 class BrDataObjectFile(BrFile):
     '''
-    class for a *.br file containing logger data
+    class for a *.br file containing data object
     '''
     def __init__(self, filename: str):
         super().__init__(filename)
         if self._fileType != BrFileType.DATA_OBJECT:
             raise TypeError(f'content is not a B&R data module (Type is {self._fileType})')
 
     @property
```

### Comparing `pvipy-0.4.0/pvi/utils/BrFile.py` & `pvipy-0.5.0/pvi/utils/BrFile.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from enum import Enum, unique
 import os
 import struct
 
 
 @unique
 class BrFileType(Enum):
+    UNKNOWN = 0
     CYCLIC_RESOURCE = 0x11
     SYSTEM_OBJECT = 0x12
     IDLE_TIME_OBJECT = 0x13
     OBJECT_OF_A_TIMER_RESOURCE = 0x14
     INTERRUPT_OBJECT = 0x15
     EXCEPTION_OBJECT = 0x16
     AVT_LIBRARY = 0x21
@@ -39,42 +40,43 @@
     ADVANCED_TRAP_LIBRARY = 0x28
     OPTIMIZED_IO_MODULE = 0x31
     IO_MAPPING = 0x32
     DATA_OBJECT = 0x41
     FIRMWARE_MODULE = 0x43
     NC_DRIVER = 0x45
     MOTION_DATA_OBJECT = 0x46
-    UNKNOWN1 = 0x4c
+    PROFILER_DATA_OBJECT = 0x4c
     LOGGER_MODULE = 0x53
     TARGET_SYSTEM_CONFIGURATION = 0x81
     NETWORK_CONFIGURATION_MODULE = 0x82
     RUNTIME_CONFIGURATION = 0x84
     TEXT_CONFIG = 0x88
     TC_DATA = 0xd1
     UNIT_DEFINITION_MODULE = 0xd2
-
+    
+    @classmethod
+    def _missing_(cls, value):
+        return BrFileType.UNKNOWN
 
 class BrFile():
     '''
     base class for all *.br files
     '''
     def __init__(self, filename : str ):
         self.__name = os.path.basename(filename)
         with open(filename, 'rb') as f:
             self._content = f.read()
-        magic_number = struct.unpack_from('>H', self._content, 0)[0]
-        if magic_number != 0x2b97:
+        magicNumber, self._fileType, self._subType, self._fileSize  = struct.unpack_from('>HBB10xI', self._content, 0) # big-endian
+        if magicNumber != 0x2b97:
             raise TypeError('content is not a B&R module !')
-        try:
-            self.__fileType = BrFileType(self._content[2])
-        except ValueError:
-            self.__fileType = hex(self._content[2])
+
 
     @property
-    def fileType(self)-> BrFileType:
-        return self.__fileType
+    def fileType(self):
+        return BrFileType(self._fileType)
+
 
     def __repr__(self) -> str:
-        return f'File ({str(self.__fileType)})'
+        return f'File ({str(self._fileType)})'
```

### Comparing `pvipy-0.4.0/pvi/utils/BrLoggerFile.py` & `pvipy-0.5.0/pvi/utils/BrLoggerFile.py`

 * *Files identical despite different names*

### Comparing `pvipy-0.4.0/tests/test1.py` & `pvipy-0.5.0/tests/test1.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 # test against 'coffee machine' in AS 4.1.17.113 SP
+from pathlib import Path
+import time
 import sys
-sys.path.append('C:\\projects\Pvi.py')
-
-from time import sleep
 import hashlib
-from pvi import *
 
+pviPath = str(Path(__file__).parents[1])
+cwd = str(Path(__file__).parents[0])
+
+sys.path.append( pviPath )
+
+from pvi import *
 
 pviConnection = Connection() # start a Pvi connection
 line = Line( pviConnection.root, 'LNANSL', CD='LNANSL')
 device = Device( line, 'TCP', CD='/IF=TcpIp' )
 cpu = Cpu( device, 'myArsim', CD='/IP=127.0.0.1' )
 
 run = True
@@ -18,22 +22,23 @@
     global run
 
      
     if error == 0:
         # read content
         allObjects = cpu.externalObjects
 
-
+        dataType = None
         tasks = dict()
         for taskName in ['mainlogic', 'feeder', 'conveyor', 'brewing', 'heating', 'visCtrl','visAlarm', 'visTrend' ] :
             task = Task( cpu, taskName )
             variableNames = [ _['name'] for _ in task.externalObjects]
             variables = list()                    
             for variableName in variableNames:
                 variable = Variable(task, variableName)
+
                 try:
                     dataType = variable.dataType
                     value = variable.value
                 except PviError as e:
                     print(e)
                 variables.append( { "Name" : variableName, "Type" : dataType} )
                 variable.kill()
@@ -67,10 +72,10 @@
 
 
 cpu.errorChanged = cpuErrorChanged
 
 
 while run:
     pviConnection.doEvents() # must be cyclically called
-    sleep(0.1)
+    time.sleep(0.1)
```

### Comparing `pvipy-0.4.0/.gitignore` & `pvipy-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pvipy-0.4.0/LICENSE` & `pvipy-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pvipy-0.4.0/README.md` & `pvipy-0.5.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,125 +1,151 @@
-[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-[![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
-[![Made For B&R](https://github.com/hilch/BandR-badges/blob/main/Made-For-BrAutomation.svg)](https://www.br-automation.com)
-
-# Pvi.py
-Python wrapper for [B&amp;R Pvi (process visualization interface)](https://www.br-automation.com/en/products/software/automation-software/automation-netpvi/).
-
-In times of more modern protocols like OPC-UA, this may seem a bit old-fashioned. 
-But PVI has some hidden strengths and is also very versatile. 
-Have a look into the documentation of the 'Lines' (ANSL, INA2000, NET2000, MTC, ADI, DCAN, SNMP, MODBUS, MININET) and what they are used for.
-In most cases it is used just to communicate with B&R PLCs with 'ANSL' and 'SNMP'.
-Unfortunately its native C-language interface is very complex and also PVI Services (C#) can be a high barrier to entry.
-It's a lot more fun with Python !
-
-# PVI installation and license
-PVI needs a previous installation of 'PVI Development Setup' from [B&R's homepage](https://www.br-automation.com).
-Without a PVI license 1TG0500.02 (+ TG Guard e.g. 0TG1000.02) PVI will run for two hours ("Trial license")
-). 
-After this period all PVI based programs will stop working (or will not even start).
-In that case PVI-Manager must be stopped and restarted again. 
-This can be very annoying if Automation Studio is being used in the background at the same time, because it then has to be restarted as well.
-Contact your local B&R office to buy a valid license if trial license is not sufficient for you.
-
-# Installation
-```
-pip install pvipy
-```
-
-# Usage
-PVI uses a complex interface to define objects and their parameters but it is well documented
-in its online help system and also in Automation Studio help system.
-There is no point in repeating this here since most of its parameters still apply in this Python interface.
-Instead, look at the examples to use parts from this for your programs.
-
-# Examples
-
-## Start here
-### [simple1.py](examples/simple1.py) (ANSL)
-this simple example just registers a variable, reads its value and then exit after a few seconds
-
-### [simple2.py](examples/simple2.py) (ANSL)
-this simple example just registers a variable for reading and another for writing. In fact we switch on the 'coffee machine' and watch its temperature ...
-
-### [simple3.py](examples/simple3.py) (INA2000)
-this simple example just registers a variable for reading and another for writing. In fact we switch on the 'coffee machine' and watch its temperature ...
-This is similar to simple2.py but we use a control running AR 3.x. ANSL is not available here and we change to good old INA2000
-
-
-## Basics
-### [basics1.py](examples/basics1.py) (ANSL)
-shows reading and writing of basic data types
-
-## Create Lists of objects
-### [list_objects1.py](examples/list_objects1.py) (ANSL)
-this example lists objects with 'global scope' (modules, task and global variables)
-from 'coffee machine' cpu and returns status information about them
-
-### [list_objects2.py](examples/list_objects2.py) (ANSL)
-this example lists global and local variables and their content
-
-### [list_objects3.py](examples/list_objects3.py) (ANSL)
-this example lists all local variables of a specific task and their content
-
-### [list_objects4.py](examples/list_objects4.py) (INA2000)
-this example lists objects with 'global scope' (modules, task and global variables)
-from 'coffee machine' cpu and returns status information about them
-
-This is similar to list_objects1.py but since we use a control running < AR 4.x ANSL is not available here and we change to good old INA2000
-
-### [list_objects5.py](examples/list_objects5.py) (INA2000)
-this example lists global and local variables and their content
-
-This is similar to list_objects2.py but since we use a control running < AR 4.x ANSL is not available here and we change to good old INA2000
-
-### [list_objects6.py](examples/list_objects6.py) (INA2000)
-this example lists all local variables of a specific task and their content
-
-This is similar to list_objects3.py but since we use a control running < AR 4.x ANSL is not available here and we change to good old INA2000
-
-
-## Handling modules
-### [modules1.py](examples/modules1.py) (ANSL)
-this simple example creates a module on CPU by downloading a bytestream and checks if it exists
-
-### [modules2.py](examples/modules2.py) (ANSL)
-this simple example creates a module on CPU by downloading a bytestream and afterwards uploads it again
-
-### [modules3.py](examples/modules3.py) 
-in this exammple we search for BR files (*.br) in a folder and read the type of content
-
-## Handling logger data
-
-### [logger1.py](examples/logger1.py) (ANSL)
-this example uploads some loggers from CPU
-
-### [logger2.py](examples/logger2.py) 
-extract all logger from a systemdump container and save them as csv
-
-### [logger3.py](examples/logger3.py) (INA2000)
-this example uploads some loggers from CPU
-
-This is similar to logger1.py but since we use a control running < AR 4.x ANSL is not available here and we change to good old INA2000
-
-
-## GUI
-### [gui1.py](examples/gui1.py) (ANSL)
-this example shows the usage of Pvi.py in tkinter
-
-## IO
-### [linknode1.py](examples/linknode1.py) (ANSL)
-this simple example just toggles an forced output
-
-## Simple Network Managament Protocol (SNMP)
-(if you are looking for a 'real' program consider to use [brsnmp](https://github.com/hilch/brsnmp) )
-
-### [browse_for_targets.py](examples/browse_for_targets.py)
-this example searches for B&R plc in local network with PVI's 'SNMP' line and lists their properties
-
-### [set_ip_address.py](examples/set_ip_address.py)
-this example searches for a specific B&R plc in local network with PVI's 'SNMP' line and changes its IP address
-
-## Test environment
-Current test environment is AS4.1.17.113 / PVI 4.1.12 which can be [downloaded from B&R website](https://www.br-automation.com/en/downloads/software/automation-studio/automation-studio-41/automation-studio-v41/) and Python 3.8
-
-
+Metadata-Version: 2.1
+Name: pvipy
+Version: 0.5.0
+Summary: Python connector for B&R Pvi (process visualization interface)
+Project-URL: Homepage, https://github.com/hilch/Pvi.py
+Project-URL: Bug Tracker, https://github.com/hilch/Pvi.py/issues
+Author: Christoph Hilchenbach
+License-File: LICENSE
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
+[![Made For B&R](https://github.com/hilch/BandR-badges/blob/main/Made-For-BrAutomation.svg)](https://www.br-automation.com)
+
+# Pvi.py
+Python wrapper for [B&amp;R Pvi (process visualization interface)](https://www.br-automation.com/en/products/software/automation-software/automation-netpvi/).
+
+In times of more modern protocols like OPC-UA, this may seem a bit old-fashioned. 
+But PVI has some hidden strengths and is also very versatile. 
+Have a look into the documentation of the 'Lines' (ANSL, INA2000, NET2000, MTC, ADI, DCAN, SNMP, MODBUS, MININET) and what they are used for.
+In most cases it is used just to communicate with B&R PLCs with 'ANSL' and 'SNMP'.
+Unfortunately its native C-language interface is very complex and also PVI Services (C#) can be a high barrier to entry.
+It's a lot more fun with Python !
+
+# PVI installation and license
+PVI needs a previous installation of 'PVI Development Setup' from [B&R's homepage](https://www.br-automation.com).
+Without a PVI license 1TG0500.02 (+ TG Guard e.g. 0TG1000.02) PVI will run for two hours ("Trial license")
+). 
+After this period all PVI based programs will stop working (or will not even start).
+In that case PVI-Manager must be stopped and restarted again. 
+This can be very annoying if Automation Studio is being used in the background at the same time, because it then has to be restarted as well.
+Contact your local B&R office to buy a valid license if trial license is not sufficient for you.
+
+# Installation
+```
+pip install pvipy
+```
+
+# Usage
+PVI uses a complex interface to define objects and their parameters but it is well documented
+in its online help system and also in Automation Studio help system.
+There is no point in repeating this here since most of its parameters still apply in this Python interface.
+Instead, look at the examples to use parts from this for your programs.
+
+# Examples
+
+## Start here
+### [simple1.py](examples/simple1.py) (ANSL)
+this simple example just registers a variable, reads its value and then exit after a few seconds
+
+### [simple2.py](examples/simple2.py) (ANSL)
+this simple example just registers a variable for reading and another for writing. In fact we switch on the 'coffee machine' and watch its temperature ...
+
+### [simple3.py](examples/simple3.py) (INA2000)
+this simple example just registers a variable for reading and another for writing. In fact we switch on the 'coffee machine' and watch its temperature ...
+This is similar to simple2.py but we use a control running AR 3.x. ANSL is not available here and we change to good old INA2000
+
+
+## Basics
+### [basics1.py](examples/basics1.py) (ANSL)
+shows reading and writing of basic data types
+
+## Create Lists of objects
+### [list_objects1.py](examples/list_objects1.py) (ANSL)
+this example lists objects with 'global scope' (modules, task and global variables)
+from 'coffee machine' cpu and returns status information about them
+
+### [list_objects2.py](examples/list_objects2.py) (ANSL)
+this example lists global and local variables and their content
+
+### [list_objects3.py](examples/list_objects3.py) (ANSL)
+this example lists all local variables of a specific task and their content
+
+### [list_objects4.py](examples/list_objects4.py) (INA2000)
+this example lists objects with 'global scope' (modules, task and global variables)
+from 'coffee machine' cpu and returns status information about them
+
+This is similar to list_objects1.py but since we use a control running < AR 4.x ANSL is not available here and we change to good old INA2000
+
+### [list_objects5.py](examples/list_objects5.py) (INA2000)
+this example lists global and local variables and their content
+
+This is similar to list_objects2.py but since we use a control running < AR 4.x ANSL is not available here and we change to good old INA2000
+
+### [list_objects6.py](examples/list_objects6.py) (INA2000)
+this example lists all local variables of a specific task and their content
+
+This is similar to list_objects3.py but since we use a control running < AR 4.x ANSL is not available here and we change to good old INA2000
+
+
+## Handling modules
+### [modules1.py](examples/modules1.py) (ANSL)
+this simple example creates a module on CPU by downloading a bytestream and checks if it exists
+
+### [modules2.py](examples/modules2.py) (ANSL)
+this simple example creates a module on CPU by downloading a bytestream and afterwards uploads it again
+
+### [modules3.py](examples/modules3.py) 
+in this exammple we search for BR files (*.br) in a folder and read the type of content
+
+## Handling logger data
+
+### [logger1.py](examples/logger1.py) (ANSL)
+this example uploads some loggers from CPU
+
+### [logger2.py](examples/logger2.py) 
+extract all logger from a systemdump container and save them as csv.
+Handling logger files is still beta since the file format is not public.
+The known structure was found out by reverse engineering.
+
+### [logger3.py](examples/logger3.py) (INA2000)
+this example uploads some loggers from CPU
+
+This is similar to logger1.py but since we use a control running < AR 4.x ANSL is not available here and we change to good old INA2000
+
+## Handling profiler data
+
+handling profiler files is still beta since the file format is not public.
+The known structure was found out by reverse engineering.
+
+### [profiler1.py](examples/profiler1.py)
+extract all profiler data *.pd file and save it to csv
+
+### [profiler2.py](examples/profiler2.py)
+extract all profiler data from a systemdump container and save it to csv
+
+## GUI
+### [gui1.py](examples/gui1.py) (ANSL)
+this example shows the usage of Pvi.py in tkinter
+
+## IO
+### [linknode1.py](examples/linknode1.py) (ANSL)
+this simple example just toggles an forced output
+
+## Simple Network Managament Protocol (SNMP)
+(if you are looking for a 'real' program consider to use [brsnmp](https://github.com/hilch/brsnmp) )
+
+### [browse_for_targets.py](examples/browse_for_targets.py)
+this example searches for B&R plc in local network with PVI's 'SNMP' line and lists their properties
+
+### [set_ip_address.py](examples/set_ip_address.py)
+this example searches for a specific B&R plc in local network with PVI's 'SNMP' line and changes its IP address
+
+## Test environment
+Current test environment is AS4.1.17.113 / PVI 4.1.12 which can be [downloaded from B&R website](https://www.br-automation.com/en/downloads/software/automation-studio/automation-studio-41/automation-studio-v41/) and Python 3.8
+
+
```

