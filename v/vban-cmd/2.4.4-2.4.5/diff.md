# Comparing `tmp/vban_cmd-2.4.4.tar.gz` & `tmp/vban_cmd-2.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vban_cmd-2.4.4.tar", max compression
+gzip compressed data, was "vban_cmd-2.4.5.tar", max compression
```

## Comparing `vban_cmd-2.4.4.tar` & `vban_cmd-2.4.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1091 2022-03-24 12:30:28.474287 vban_cmd-2.4.4/LICENSE
--rw-r--r--   0        0        0      951 2023-08-05 13:05:11.722868 vban_cmd-2.4.4/pyproject.toml
--rw-r--r--   0        0        0    12875 2023-07-15 07:15:00.451610 vban_cmd-2.4.4/README.md
--rw-r--r--   0        0        0       70 2022-07-12 16:30:51.963399 vban_cmd-2.4.4/vban_cmd/__init__.py
--rw-r--r--   0        0        0     5282 2023-08-05 12:38:42.131764 vban_cmd-2.4.4/vban_cmd/bus.py
--rw-r--r--   0        0        0     1127 2023-06-25 10:36:19.263212 vban_cmd-2.4.4/vban_cmd/command.py
--rw-r--r--   0        0        0     5855 2023-07-11 17:23:11.340063 vban_cmd-2.4.4/vban_cmd/config.py
--rw-r--r--   0        0        0      220 2023-08-02 14:36:24.956502 vban_cmd-2.4.4/vban_cmd/error.py
--rw-r--r--   0        0        0     1621 2023-06-22 09:26:30.424951 vban_cmd-2.4.4/vban_cmd/event.py
--rw-r--r--   0        0        0     6888 2023-08-02 16:14:19.633476 vban_cmd-2.4.4/vban_cmd/factory.py
--rw-r--r--   0        0        0     4130 2023-07-25 14:58:38.295129 vban_cmd-2.4.4/vban_cmd/iremote.py
--rw-r--r--   0        0        0     2418 2023-07-25 14:54:48.277200 vban_cmd-2.4.4/vban_cmd/kinds.py
--rw-r--r--   0        0        0     1158 2023-07-25 15:00:05.263943 vban_cmd-2.4.4/vban_cmd/macrobutton.py
--rw-r--r--   0        0        0     2992 2023-06-25 10:36:33.230612 vban_cmd-2.4.4/vban_cmd/meta.py
--rw-r--r--   0        0        0    10280 2023-08-05 12:40:25.293246 vban_cmd-2.4.4/vban_cmd/packet.py
--rw-r--r--   0        0        0    10143 2023-08-05 12:38:42.132905 vban_cmd-2.4.4/vban_cmd/strip.py
--rw-r--r--   0        0        0     2277 2023-06-25 10:36:40.287522 vban_cmd-2.4.4/vban_cmd/subject.py
--rw-r--r--   0        0        0     2525 2023-07-12 03:46:12.026345 vban_cmd-2.4.4/vban_cmd/util.py
--rw-r--r--   0        0        0     5615 2023-08-05 12:53:07.240889 vban_cmd-2.4.4/vban_cmd/vban.py
--rw-r--r--   0        0        0     7815 2023-08-05 13:04:25.083376 vban_cmd-2.4.4/vban_cmd/vbancmd.py
--rw-r--r--   0        0        0     7274 2023-08-05 12:38:42.133906 vban_cmd-2.4.4/vban_cmd/worker.py
--rw-r--r--   0        0        0    12994 1970-01-01 00:00:00.000000 vban_cmd-2.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-03-24 12:30:28.474287 vban_cmd-2.4.5/LICENSE
+-rw-r--r--   0        0        0      951 2023-08-07 14:56:48.934163 vban_cmd-2.4.5/pyproject.toml
+-rw-r--r--   0        0        0    12875 2023-07-15 07:15:00.451610 vban_cmd-2.4.5/README.md
+-rw-r--r--   0        0        0       70 2022-07-12 16:30:51.963399 vban_cmd-2.4.5/vban_cmd/__init__.py
+-rw-r--r--   0        0        0     5282 2023-08-07 16:25:40.786694 vban_cmd-2.4.5/vban_cmd/bus.py
+-rw-r--r--   0        0        0     1127 2023-08-07 16:32:47.400951 vban_cmd-2.4.5/vban_cmd/command.py
+-rw-r--r--   0        0        0     5855 2023-07-11 17:23:11.340063 vban_cmd-2.4.5/vban_cmd/config.py
+-rw-r--r--   0        0        0      403 2023-08-07 14:28:43.211577 vban_cmd-2.4.5/vban_cmd/error.py
+-rw-r--r--   0        0        0     1621 2023-06-22 09:26:30.424951 vban_cmd-2.4.5/vban_cmd/event.py
+-rw-r--r--   0        0        0     6888 2023-08-02 16:14:19.633476 vban_cmd-2.4.5/vban_cmd/factory.py
+-rw-r--r--   0        0        0     4130 2023-07-25 14:58:38.295129 vban_cmd-2.4.5/vban_cmd/iremote.py
+-rw-r--r--   0        0        0     2418 2023-07-25 14:54:48.277200 vban_cmd-2.4.5/vban_cmd/kinds.py
+-rw-r--r--   0        0        0     1158 2023-07-25 15:00:05.263943 vban_cmd-2.4.5/vban_cmd/macrobutton.py
+-rw-r--r--   0        0        0     2992 2023-06-25 10:36:33.230612 vban_cmd-2.4.5/vban_cmd/meta.py
+-rw-r--r--   0        0        0    10280 2023-08-05 12:40:25.293246 vban_cmd-2.4.5/vban_cmd/packet.py
+-rw-r--r--   0        0        0    10143 2023-08-07 16:26:27.776233 vban_cmd-2.4.5/vban_cmd/strip.py
+-rw-r--r--   0        0        0     2277 2023-06-25 10:36:40.287522 vban_cmd-2.4.5/vban_cmd/subject.py
+-rw-r--r--   0        0        0     2489 2023-08-07 16:20:02.230068 vban_cmd-2.4.5/vban_cmd/util.py
+-rw-r--r--   0        0        0     5615 2023-08-05 12:53:07.240889 vban_cmd-2.4.5/vban_cmd/vban.py
+-rw-r--r--   0        0        0     7815 2023-08-05 13:04:25.083376 vban_cmd-2.4.5/vban_cmd/vbancmd.py
+-rw-r--r--   0        0        0     7274 2023-08-06 19:26:52.970276 vban_cmd-2.4.5/vban_cmd/worker.py
+-rw-r--r--   0        0        0    12994 1970-01-01 00:00:00.000000 vban_cmd-2.4.5/PKG-INFO
```

### Comparing `vban_cmd-2.4.4/LICENSE` & `vban_cmd-2.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.4.4/pyproject.toml` & `vban_cmd-2.4.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vban-cmd"
-version = "2.4.4"
+version = "2.4.5"
 description = "Python interface for the VBAN RT Packet Service (Sendtext)"
 authors = ["onyx-and-iris <code@onyxandiris.online>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/onyx-and-iris/vban-cmd-python"
 
 [tool.poetry.dependencies]
```

### Comparing `vban_cmd-2.4.4/README.md` & `vban_cmd-2.4.5/README.md`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.4.4/vban_cmd/bus.py` & `vban_cmd-2.4.5/vban_cmd/bus.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
     @abstractmethod
     def __str__(self):
         pass
 
     @property
     def identifier(self) -> str:
-        return f"Bus[{self.index}]"
+        return f"bus[{self.index}]"
 
     @property
     def gain(self) -> float:
         def fget():
             val = self.public_packet.busgain[self.index]
             if 0 <= val <= 1200:
                 return val * 0.01
@@ -62,15 +62,15 @@
                 **{param: channel_bool_prop(param) for param in ["on", "ab"]},
             },
         )
         return BUSEQ_cls(remote, index)
 
     @property
     def identifier(self) -> str:
-        return f"Bus[{self.index}].eq"
+        return f"bus[{self.index}].eq"
 
 
 class PhysicalBus(Bus):
     def __str__(self):
         return f"{type(self).__name__}{self.index}"
 
     @property
@@ -112,15 +112,15 @@
             for i in self._remote._get_levels(self.public_packet)[1][
                 self.range[0] : self.range[-1]
             ]
         )
 
     @property
     def identifier(self) -> str:
-        return f"Bus[{self.index}]"
+        return f"bus[{self.index}]"
 
     @property
     def all(self) -> tuple:
         return self.getter()
 
     @property
     def isdirty(self) -> bool:
@@ -134,15 +134,15 @@
     is_updated = isdirty
 
 
 def _make_bus_mode_mixin():
     """Creates a mixin of Bus Modes."""
 
     def identifier(self) -> str:
-        return f"Bus[{self.index}].mode"
+        return f"bus[{self.index}].mode"
 
     def get(self):
         time.sleep(0.01)
         for i, val in enumerate(
             [
                 self.amix,
                 self.bmix,
```

### Comparing `vban_cmd-2.4.4/vban_cmd/command.py` & `vban_cmd-2.4.5/vban_cmd/command.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
                 "hide": action_fn("show", val=0),
             },
         )
         return CMD_cls(remote)
 
     @property
     def identifier(self) -> str:
-        return "Command"
+        return "command"
 
     def set_showvbanchat(self, val: bool):
         self.setter("DialogShow.VBANCHAT", 1 if val else 0)
 
     showvbanchat = property(fset=set_showvbanchat)
 
     def set_lock(self, val: bool):
```

### Comparing `vban_cmd-2.4.4/vban_cmd/config.py` & `vban_cmd-2.4.5/vban_cmd/config.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.4.4/vban_cmd/event.py` & `vban_cmd-2.4.5/vban_cmd/event.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.4.4/vban_cmd/factory.py` & `vban_cmd-2.4.5/vban_cmd/factory.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.4.4/vban_cmd/iremote.py` & `vban_cmd-2.4.5/vban_cmd/iremote.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.4.4/vban_cmd/kinds.py` & `vban_cmd-2.4.5/vban_cmd/kinds.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.4.4/vban_cmd/macrobutton.py` & `vban_cmd-2.4.5/vban_cmd/macrobutton.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.4.4/vban_cmd/meta.py` & `vban_cmd-2.4.5/vban_cmd/meta.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.4.4/vban_cmd/packet.py` & `vban_cmd-2.4.5/vban_cmd/packet.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.4.4/vban_cmd/strip.py` & `vban_cmd-2.4.5/vban_cmd/strip.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
     @abstractmethod
     def __str__(self):
         pass
 
     @property
     def identifier(self) -> str:
-        return f"Strip[{self.index}]"
+        return f"strip[{self.index}]"
 
     @property
     def limit(self) -> int:
         return
 
     @limit.setter
     def limit(self, val: int):
@@ -75,15 +75,15 @@
     def sr(self):
         return
 
 
 class StripComp(IRemote):
     @property
     def identifier(self) -> str:
-        return f"Strip[{self.index}].comp"
+        return f"strip[{self.index}].comp"
 
     @property
     def knob(self) -> float:
         return
 
     @knob.setter
     def knob(self, val: float):
@@ -153,15 +153,15 @@
     def makeup(self, val: bool):
         self.setter("makeup", 1 if val else 0)
 
 
 class StripGate(IRemote):
     @property
     def identifier(self) -> str:
-        return f"Strip[{self.index}].gate"
+        return f"strip[{self.index}].gate"
 
     @property
     def knob(self) -> float:
         return
 
     @knob.setter
     def knob(self, val: float):
@@ -215,29 +215,29 @@
     def release(self, val: float):
         self.setter("Release", val)
 
 
 class StripDenoiser(IRemote):
     @property
     def identifier(self) -> str:
-        return f"Strip[{self.index}].denoiser"
+        return f"strip[{self.index}].denoiser"
 
     @property
     def knob(self) -> float:
         return
 
     @knob.setter
     def knob(self, val: float):
         self.setter("", val)
 
 
 class StripEQ(IRemote):
     @property
     def identifier(self) -> str:
-        return f"Strip[{self.index}].eq"
+        return f"strip[{self.index}].eq"
 
     @property
     def on(self):
         return
 
     @on.setter
     def on(self, val: bool):
@@ -308,15 +308,15 @@
             for i in self._remote._get_levels(self.public_packet)[0][
                 self.range[0] : self.range[-1]
             ]
         )
 
     @property
     def identifier(self) -> str:
-        return f"Strip[{self.index}]"
+        return f"strip[{self.index}]"
 
     @property
     def prefader(self) -> tuple:
         return self.getter()
 
     @property
     def postfader(self) -> tuple:
@@ -341,15 +341,15 @@
 class GainLayer(IRemote):
     def __init__(self, remote, index, i):
         super().__init__(remote, index)
         self._i = i
 
     @property
     def identifier(self) -> str:
-        return f"Strip[{self.index}]"
+        return f"strip[{self.index}]"
 
     @property
     def gain(self) -> float:
         def fget():
             val = getattr(self.public_packet, f"stripgainlayer{self._i+1}")[self.index]
             if 0 <= val <= 1200:
                 return val * 0.01
```

### Comparing `vban_cmd-2.4.4/vban_cmd/subject.py` & `vban_cmd-2.4.5/vban_cmd/subject.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.4.4/vban_cmd/util.py` & `vban_cmd-2.4.5/vban_cmd/util.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,32 +3,30 @@
 
 
 def cache_bool(func, param):
     """Check cache for a bool prop"""
 
     def wrapper(*args, **kwargs):
         self, *rem = args
-        cmd = f"{self.identifier}.{param}"
-        if cmd in self._remote.cache:
-            return self._remote.cache.pop(cmd) == 1
+        if self._cmd(param) in self._remote.cache:
+            return self._remote.cache.pop(self._cmd(param)) == 1
         if self._remote.sync:
             self._remote.clear_dirty()
         return func(*args, **kwargs)
 
     return wrapper
 
 
 def cache_string(func, param):
     """Check cache for a string prop"""
 
     def wrapper(*args, **kwargs):
         self, *rem = args
-        cmd = f"{self.identifier}.{param}"
-        if cmd in self._remote.cache:
-            return self._remote.cache.pop(cmd)
+        if self._cmd(param) in self._remote.cache:
+            return self._remote.cache.pop(self._cmd(param))
         if self._remote.sync:
             self._remote.clear_dirty()
         return func(*args, **kwargs)
 
     return wrapper
```

### Comparing `vban_cmd-2.4.4/vban_cmd/vban.py` & `vban_cmd-2.4.5/vban_cmd/vban.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.4.4/vban_cmd/vbancmd.py` & `vban_cmd-2.4.5/vban_cmd/vbancmd.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.4.4/vban_cmd/worker.py` & `vban_cmd-2.4.5/vban_cmd/worker.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.4.4/PKG-INFO` & `vban_cmd-2.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vban-cmd
-Version: 2.4.4
+Version: 2.4.5
 Summary: Python interface for the VBAN RT Packet Service (Sendtext)
 Home-page: https://github.com/onyx-and-iris/vban-cmd-python
 License: MIT
 Author: onyx-and-iris
 Author-email: code@onyxandiris.online
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

