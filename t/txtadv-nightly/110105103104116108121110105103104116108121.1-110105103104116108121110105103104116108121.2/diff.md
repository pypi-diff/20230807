# Comparing `tmp/txtadv_nightly-110105103104116108121110105103104116108121.1.tar.gz` & `tmp/txtadv_nightly-110105103104116108121110105103104116108121.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "txtadv_nightly-110105103104116108121110105103104116108121.1.tar", max compression
+gzip compressed data, was "txtadv_nightly-110105103104116108121110105103104116108121.2.tar", max compression
```

## Comparing `txtadv_nightly-110105103104116108121110105103104116108121.1.tar` & `txtadv_nightly-110105103104116108121110105103104116108121.2.tar`

### file list

```diff
@@ -1,12 +1,16 @@
--rw-r--r--   0        0        0     1068 2023-03-19 13:40:22.089727 txtadv_nightly-110105103104116108121110105103104116108121.1/LICENSE
--rw-r--r--   0        0        0      508 2023-03-19 13:40:22.089727 txtadv_nightly-110105103104116108121110105103104116108121.1/pyproject.toml
--rw-r--r--   0        0        0      414 2023-03-19 13:40:22.093727 txtadv_nightly-110105103104116108121110105103104116108121.1/txtadv_nightly/BUILD_DESC.md
--rw-r--r--   0        0        0    11499 2023-03-19 13:40:22.093727 txtadv_nightly-110105103104116108121110105103104116108121.1/txtadv_nightly/__init__.py
--rw-r--r--   0        0        0      759 2023-03-19 13:40:22.093727 txtadv_nightly-110105103104116108121110105103104116108121.1/txtadv_nightly/color/__init__.py
--rw-r--r--   0        0        0     7006 2023-03-19 13:40:22.093727 txtadv_nightly-110105103104116108121110105103104116108121.1/txtadv_nightly/commands/__init__.py
--rw-r--r--   0        0        0        0 2023-03-19 13:40:22.093727 txtadv_nightly-110105103104116108121110105103104116108121.1/txtadv_nightly/file/__init__.py
--rw-r--r--   0        0        0     2546 2023-03-19 13:40:22.093727 txtadv_nightly-110105103104116108121110105103104116108121.1/txtadv_nightly/file/load.py
--rw-r--r--   0        0        0     1696 2023-03-19 13:40:22.093727 txtadv_nightly-110105103104116108121110105103104116108121.1/txtadv_nightly/file/save.py
--rw-r--r--   0        0        0      720 2023-03-19 13:40:22.093727 txtadv_nightly-110105103104116108121110105103104116108121.1/txtadv_nightly/location/__init__.py
--rw-r--r--   0        0        0     1955 2023-03-19 13:40:22.093727 txtadv_nightly-110105103104116108121110105103104116108121.1/txtadv_nightly/messaging/__init__.py
--rw-r--r--   0        0        0      877 1970-01-01 00:00:00.000000 txtadv_nightly-110105103104116108121110105103104116108121.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-05 15:06:54.299875 txtadv_nightly-110105103104116108121110105103104116108121.2/LICENSE
+-rw-r--r--   0        0        0      508 2023-06-05 15:06:54.351875 txtadv_nightly-110105103104116108121110105103104116108121.2/pyproject.toml
+-rw-r--r--   0        0        0      414 2023-06-05 15:06:54.351875 txtadv_nightly-110105103104116108121110105103104116108121.2/txtadv_nightly/BUILD_DESC.md
+-rw-r--r--   0        0        0    11466 2023-06-05 15:06:54.351875 txtadv_nightly-110105103104116108121110105103104116108121.2/txtadv_nightly/__init__.py
+-rw-r--r--   0        0        0      786 2023-06-05 15:06:54.351875 txtadv_nightly-110105103104116108121110105103104116108121.2/txtadv_nightly/color/__init__.py
+-rw-r--r--   0        0        0     7006 2023-06-05 15:06:54.351875 txtadv_nightly-110105103104116108121110105103104116108121.2/txtadv_nightly/commands/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 15:06:54.351875 txtadv_nightly-110105103104116108121110105103104116108121.2/txtadv_nightly/file/__init__.py
+-rw-r--r--   0        0        0     2418 2023-06-05 15:06:54.351875 txtadv_nightly-110105103104116108121110105103104116108121.2/txtadv_nightly/file/load.py
+-rw-r--r--   0        0        0     1895 2023-06-05 15:06:54.351875 txtadv_nightly-110105103104116108121110105103104116108121.2/txtadv_nightly/file/save.py
+-rw-r--r--   0        0        0      720 2023-06-05 15:06:54.351875 txtadv_nightly-110105103104116108121110105103104116108121.2/txtadv_nightly/location/__init__.py
+-rw-r--r--   0        0        0     2118 2023-06-05 15:06:54.351875 txtadv_nightly-110105103104116108121110105103104116108121.2/txtadv_nightly/messaging/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 15:06:54.351875 txtadv_nightly-110105103104116108121110105103104116108121.2/txtadv_nightly/multiplayer/__init__.py
+-rw-r--r--   0        0        0       32 2023-06-05 15:06:54.351875 txtadv_nightly-110105103104116108121110105103104116108121.2/txtadv_nightly/multiplayer/recieve.py
+-rw-r--r--   0        0        0     2212 2023-06-05 15:06:54.351875 txtadv_nightly-110105103104116108121110105103104116108121.2/txtadv_nightly/multiplayer/taw.proto
+-rw-r--r--   0        0        0     5884 2023-06-05 15:06:54.351875 txtadv_nightly-110105103104116108121110105103104116108121.2/txtadv_nightly/multiplayer/taw_pb2.py
+-rw-r--r--   0        0        0      877 1970-01-01 00:00:00.000000 txtadv_nightly-110105103104116108121110105103104116108121.2/PKG-INFO
```

### Comparing `txtadv_nightly-110105103104116108121110105103104116108121.1/LICENSE` & `txtadv_nightly-110105103104116108121110105103104116108121.2/LICENSE`

 * *Files identical despite different names*

### Comparing `txtadv_nightly-110105103104116108121110105103104116108121.1/txtadv_nightly/__init__.py` & `txtadv_nightly-110105103104116108121110105103104116108121.2/txtadv_nightly/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """A feature-rich text adventure framework in Python."""
 import sys
 import os
-from typing import List
 from txtadv import commands
 from txtadv.messaging import info, setinfomode, no_origin, origin, error as err
 
 __version__ = 1.0
 
 
 class _CONSTANTS:
@@ -222,34 +221,33 @@
 
     def pickup(self, item: Item):
         """Pickup an item."""
         item.move(self.inventory)
 
 
 class Entity(Player):
-    """An Entity. Can be described as a scripted player."""
+    """An Entity. Can be described as a scripted player.(NOTE: Still very much in development. We suggest not using it currently."""
 
     def __init__(self, startloc: Room, file_name: str):
         self.colored = False
         self.prevcontext = 0
         self.context = 0
         self.file_name = file_name
         with open(file_name, 'r', encoding='ascii') as file:
             with open(os.devnull, 'w', encoding='ascii') as null:
                 super().__init__(startloc, file, null, colored=False)
 
     def exec_from_file(self, file_name):
         """Set the file executed from"""
-        with open(file_name, 'r', encoding='ascii') as file:
-            self.instream = file
+        self.file_name = file_name
+        self.instream = open(self.file_name, 'r', encoding='ascii')
 
     def tick(self, world):
         """Tickes the entity and makes it perform an action."""
         #pylint: disable=consider-using-with
-        self.instream = open(self.file_name, 'r', encoding='ascii')
         self.outstream = open(os.devnull, 'w', encoding='ascii')
         #pylint: enable=consider-using-with
         self.exec(self.instream.readline(), world)
 
     def exec(self, instruction, world):
         """Executes an instruction for this Entity."""
         cmd_count = 0
@@ -287,15 +285,15 @@
 
 class World:
     """The World class. Contains a starting room, a list of commands, and at least one player."""
 
     def __init__(
             self,
             start: Room,
-            cmds: List[commands.Command] = _CONSTANTS.global_cmds) -> None:
+            cmds = _CONSTANTS.global_cmds) -> None:
         self.start = start
         if callable(cmds):
             self.cmds = cmds()
         else:
             self.cmds = cmds
         self.players = [Player(start, sys.stdin, sys.stdout)]
         self.entities = []
@@ -340,15 +338,15 @@
 
     def add_entity(self, entity: Entity) -> None:
         """Adds an Entity to this World."""
         self.entities.append(entity)
 
     def new_chat(self, message, source, local=None) -> None:
         #pylint: disable-next=line-too-long
-        """DO NOT USE. Instead run World.chat_event.trigger(message: str, source: str, local: NoneType or Room"""
+        """DO NOT USE. Instead run World.chat_event.trigger(message: str, source: str, local: NoneType or Room)"""
         self.chat.append(source + " says: " + message)
         setinfomode(no_origin)
         if local is None:
             for player in self.players:
                 info(source + " says: " + message + "\n", player)
             setinfomode(origin)
             return
```

### Comparing `txtadv_nightly-110105103104116108121110105103104116108121.1/txtadv_nightly/color/__init__.py` & `txtadv_nightly-110105103104116108121110105103104116108121.2/txtadv_nightly/color/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,10 +20,10 @@
 def colored(text, color):
     """Colored text"""
     if color.startswith('\u001b'):
         return color + text + RESET
     return globals()[color.upper()] + text + RESET
 
 def background_color(color):
-    """Set the background color. DOES NOT EXCEPT RGB COLOR STRINGS!"""
-    os.system('setterm -term linux -back $'+color+' -fore white -clear')
+    """Set the background color. Only accepts colors in the form 'red' or 'green', not txtadv.color.RED or \u001b[36m"""
+    os.system('setterm -term linux -back '+color)
```

### Comparing `txtadv_nightly-110105103104116108121110105103104116108121.1/txtadv_nightly/commands/__init__.py` & `txtadv_nightly-110105103104116108121110105103104116108121.2/txtadv_nightly/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `txtadv_nightly-110105103104116108121110105103104116108121.1/txtadv_nightly/file/load.py` & `txtadv_nightly-110105103104116108121110105103104116108121.2/txtadv_nightly/file/load.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,56 +3,61 @@
 import inspect
 import sys
 import marshal
 import pickle
 import json
 from .. import messaging
 from .. import __init__ as txtadv
+
 savepath = os.path.dirname(inspect.getfile(txtadv)) + "/saves"
 
 
 class Call:
     """The class that's used to make this module callable"""
 
     def single_load(self, item):
         """Load a single item"""
         try:
             return json.loads(item)
-        except TypeError:
+        except json.decoder.JSONDecodeError:
             try:
                 return marshal.loads(item)
-            except TypeError:
+            except (EOFError, TypeError, ValueError):
                 try:
-                    return marshal.loads(item.__code__)
-                except AttributeError:
-                    try:
-                        return pickle.loads(item)
-                    #pylint: disable-next=duplicate-code
-                    except pickle.PicklingError:
-                        messaging.error(
-                            #pylint: disable-next=line-too-long
-                            f"Sorry, we found an {item.__class__.__name__} with the name/signature {item} that is an invalid object for the world storage system. This means that you aren't basing it on an Object, an Item, a Player, a Room, or an Entity. Please make it be based on one of those.\n",
-                            sys.stdout)
-                        return bytes()
+                    return pickle.loads(item)
+                #pylint: disable-next=duplicate-code
+                except (TypeError, pickle.UnpicklingError):
+                    messaging.error(
+                        #pylint: disable-next=line-too-long
+                        "Sorry, while trying to load an item, it wasn't stored as json data, marshal data, or pickle data\n",
+                        sys.stdout)
+                    return bytes()
 
     def __call__(self, filename):
         try:
             #pylint: disable-next=consider-using-with
-            file = pickle.load(open(filename+".save",'rb'))
-        except (FileNotFoundError, IsADirectoryError, TypeError, pickle.UnpicklingError):
+            file = pickle.load(open(filename + ".save", 'rb'))
+        except (FileNotFoundError, IsADirectoryError, TypeError,
+                pickle.UnpicklingError):
             #pylint: disable-next=line-too-long
-            messaging.error(f"Attempted load of invalid save/nonexistant save {filename}!\n",sys.stdout)
+            messaging.error(
+                f"Attempted load of invalid save/nonexistant save {filename}!\n",
+                sys.stdout)
             return
         if file.__class__.__name__ != "dict":
-            messaging.error(f"Attempted load of invalid save {filename}!\n",sys.stdout)
+            messaging.error(f"Attempted load of invalid save {filename}!\n",
+                            sys.stdout)
             return
-        if file["__VERSION__"] != txtadv.__VERSION__:
+        if file["__VERSION__"] != txtadv.__version__:
             #pylint: disable-next=line-too-long
-            file_version = file["__VERSION__"] # I do this instead of putting it in the f-string directly because for some reason if I do, pylint and python get VERY mad
+            file_version = file[
+                "__VERSION__"]  # I do this instead of putting it in the f-string directly because for some reason if I do, pylint and python get VERY mad
             #pylint: disable-next=line-too-long
-            messaging.error(f"Attempted load of save {filename} which has a file version of {file_version}, but this copy of txtadv is still on version {txtadv.__VERSION__}!\n",sys.stdout)
+            messaging.error(
+                f"Attempted load of save {filename} which has a file version of {file_version}, but this copy of txtadv is still on version {txtadv.__VERSION__}!\n",
+                sys.stdout)
         copy = {}
         for ite in file.items():
             copy[ite] = self.single_load(ite)
 
 
 sys.modules[__name__] = Call()
```

### Comparing `txtadv_nightly-110105103104116108121110105103104116108121.1/txtadv_nightly/file/save.py` & `txtadv_nightly-110105103104116108121110105103104116108121.2/txtadv_nightly/file/save.py`

 * *Files 17% similar despite different names*

```diff
@@ -33,14 +33,20 @@
                             sys.stdout)
                         return bytes()
 
     def __call__(self, item):
         copy = {}
         for ite in item.__class__.save.append("__class__"):
             copy[ite] = self.single_save(item.__getitem__(ite))
-        copy["__VERSION__"] = txtadv.__VERSION__
+        copy["__VERSION__"] = txtadv.__version__
         #pylint: disable-next=consider-using-with
         pickle.dump(copy,open(savepath+"/"+item.__name__,'wb'))
         return pickle.dumps(copy)
 
+    def save_to_file(self, item):
+        """Save to a file"""
+        data = self(item)
+        with open(item.__name__ + '.' + item.__class__.__name__, 'wb') as file:
+            file.write(data)
+
 
 sys.modules[__name__] = Call()
```

### Comparing `txtadv_nightly-110105103104116108121110105103104116108121.1/txtadv_nightly/location/__init__.py` & `txtadv_nightly-110105103104116108121110105103104116108121.2/txtadv_nightly/location/__init__.py`

 * *Files identical despite different names*

### Comparing `txtadv_nightly-110105103104116108121110105103104116108121.1/txtadv_nightly/messaging/__init__.py` & `txtadv_nightly-110105103104116108121110105103104116108121.2/txtadv_nightly/messaging/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,39 +27,50 @@
 def info(message, target):
     """Print an info message to the target"""
     ocolored(message, target, 'black')
 
 
 def ocolored(message, target, color):
     """Print an colored message to the target if it is supported."""
+    write = True
     try:
+        target.write("")
+    except AttributeError:
+        write = False
+    try:
+        assert target.colored
+    except (AssertionError, AttributeError):
+        
+    if write:
         if target.colored:
             if inspect.stack == origin:
-                target.outstream.write(
+                target.write(
                     colored(
                         inspect.stack()[1].function.upper() + ": " + message,
                         color))
-                target.write(
+            else:
+                target.write(colored(message, color))
+        else:
+            if inspect.stack == origin:
+                target.write(inspect.stack()[1].function.upper() + ": " +
+                             message)
+            else:
+                target.write(message)
+    else:
+        if target.colored:
+            if inspect.stack == origin:
+                target.outstream.write(
                     colored(
                         inspect.stack()[1].function.upper() + ": " + message,
                         color))
             else:
                 target.outstream.write(colored(message, color))
-                target.write(colored(message, color))
         else:
             if inspect.stack == origin:
                 target.outstream.write(inspect.stack()[1].function.upper() +
                                        ": " + message)
-                target.write(inspect.stack()[1].function.upper() + ": " +
-                             message)
             else:
                 target.outstream.write(message)
-                target.write(message)
-    except AttributeError:
-        if inspect.stack == origin:
-            target.write(inspect.stack()[1].function.upper() + ": " + message)
-        else:
-            target.write(message)
-    try:
-        target.outstream.flush()
-    except AttributeError:
+    if write:
         target.flush()
+    else:
+        target.outstream.flush()
```

### Comparing `txtadv_nightly-110105103104116108121110105103104116108121.1/PKG-INFO` & `txtadv_nightly-110105103104116108121110105103104116108121.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: txtadv-nightly
-Version: 110105103104116108121110105103104116108121.1
+Version: 110105103104116108121110105103104116108121.2
 Summary: The nightly version of txtadv, a feature-rich text adventure library!
 License: MIT
 Author: sdft
 Author-email: averse.abfun@gmail.com
 Requires-Python: >=3.10.0,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

