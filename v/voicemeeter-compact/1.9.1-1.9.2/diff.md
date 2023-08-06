# Comparing `tmp/voicemeeter_compact-1.9.1.tar.gz` & `tmp/voicemeeter_compact-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voicemeeter_compact-1.9.1.tar", max compression
+gzip compressed data, was "voicemeeter_compact-1.9.2.tar", max compression
```

## Comparing `voicemeeter_compact-1.9.1.tar` & `voicemeeter_compact-1.9.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1091 2022-04-11 12:14:57.626259 voicemeeter_compact-1.9.1/LICENSE
--rw-r--r--   0        0        0      730 2023-07-13 00:28:29.352025 voicemeeter_compact-1.9.1/pyproject.toml
--rw-r--r--   0        0        0     6125 2023-07-10 03:18:55.019093 voicemeeter_compact-1.9.1/README.md
--rw-r--r--   0        0        0       51 2022-07-07 14:44:58.582602 voicemeeter_compact-1.9.1/vmcompact/__init__.py
--rw-r--r--   0        0        0     6247 2023-07-13 00:20:26.988130 voicemeeter_compact-1.9.1/vmcompact/app.py
--rw-r--r--   0        0        0     1123 2023-06-24 22:06:19.553026 voicemeeter_compact-1.9.1/vmcompact/banner.py
--rw-r--r--   0        0        0    23962 2023-07-10 23:26:02.030414 voicemeeter_compact-1.9.1/vmcompact/builders.py
--rw-r--r--   0        0        0    11135 2023-07-10 23:59:51.207793 voicemeeter_compact-1.9.1/vmcompact/channels.py
--rw-r--r--   0        0        0     9852 2023-07-10 23:14:22.369555 voicemeeter_compact-1.9.1/vmcompact/config.py
--rw-r--r--   0        0        0     2835 2023-07-07 21:51:19.065698 voicemeeter_compact-1.9.1/vmcompact/configurations.py
--rw-r--r--   0        0        0     2124 2023-06-29 14:29:39.821962 voicemeeter_compact-1.9.1/vmcompact/data.py
--rw-r--r--   0        0        0       86 2023-06-25 11:25:22.327174 voicemeeter_compact-1.9.1/vmcompact/errors.py
--rw-r--r--   0        0        0     9178 2023-07-10 23:25:00.326724 voicemeeter_compact-1.9.1/vmcompact/gainlayer.py
--rw-r--r--   0        0        0   112922 2022-07-01 01:04:51.170192 voicemeeter_compact-1.9.1/vmcompact/img/cat.ico
--rw-r--r--   0        0        0    16901 2023-07-10 22:04:53.242069 voicemeeter_compact-1.9.1/vmcompact/menu.py
--rw-r--r--   0        0        0     3785 2023-06-29 10:52:07.632943 voicemeeter_compact-1.9.1/vmcompact/navigation.py
--rw-r--r--   0        0        0      854 2022-08-02 08:43:15.749028 voicemeeter_compact-1.9.1/vmcompact/subject.py
--rw-r--r--   0        0        0     6909 1970-01-01 00:00:00.000000 voicemeeter_compact-1.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-04-11 12:14:57.626259 voicemeeter_compact-1.9.2/LICENSE
+-rw-r--r--   0        0        0      730 2023-08-06 22:13:23.213843 voicemeeter_compact-1.9.2/pyproject.toml
+-rw-r--r--   0        0        0     6125 2023-07-10 03:18:55.019093 voicemeeter_compact-1.9.2/README.md
+-rw-r--r--   0        0        0       51 2022-07-07 14:44:58.582602 voicemeeter_compact-1.9.2/vmcompact/__init__.py
+-rw-r--r--   0        0        0     6444 2023-08-06 20:16:48.129434 voicemeeter_compact-1.9.2/vmcompact/app.py
+-rw-r--r--   0        0        0     1123 2023-06-24 22:06:19.553026 voicemeeter_compact-1.9.2/vmcompact/banner.py
+-rw-r--r--   0        0        0    23962 2023-08-06 18:20:04.537692 voicemeeter_compact-1.9.2/vmcompact/builders.py
+-rw-r--r--   0        0        0    11393 2023-08-06 18:58:16.778224 voicemeeter_compact-1.9.2/vmcompact/channels.py
+-rw-r--r--   0        0        0     9852 2023-07-10 23:14:22.369555 voicemeeter_compact-1.9.2/vmcompact/config.py
+-rw-r--r--   0        0        0     2835 2023-07-07 21:51:19.065698 voicemeeter_compact-1.9.2/vmcompact/configurations.py
+-rw-r--r--   0        0        0     2124 2023-06-29 14:29:39.821962 voicemeeter_compact-1.9.2/vmcompact/data.py
+-rw-r--r--   0        0        0       86 2023-06-25 11:25:22.327174 voicemeeter_compact-1.9.2/vmcompact/errors.py
+-rw-r--r--   0        0        0     9178 2023-07-10 23:25:00.326724 voicemeeter_compact-1.9.2/vmcompact/gainlayer.py
+-rw-r--r--   0        0        0   112922 2022-07-01 01:04:51.170192 voicemeeter_compact-1.9.2/vmcompact/img/cat.ico
+-rw-r--r--   0        0        0    16909 2023-08-06 21:44:00.907051 voicemeeter_compact-1.9.2/vmcompact/menu.py
+-rw-r--r--   0        0        0     3785 2023-08-06 11:45:37.221440 voicemeeter_compact-1.9.2/vmcompact/navigation.py
+-rw-r--r--   0        0        0      854 2022-08-02 08:43:15.749028 voicemeeter_compact-1.9.2/vmcompact/subject.py
+-rw-r--r--   0        0        0     6909 1970-01-01 00:00:00.000000 voicemeeter_compact-1.9.2/PKG-INFO
```

### Comparing `voicemeeter_compact-1.9.1/LICENSE` & `voicemeeter_compact-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `voicemeeter_compact-1.9.1/pyproject.toml` & `voicemeeter_compact-1.9.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "voicemeeter-compact"
-version = "1.9.1"
+version = "1.9.2"
 description = "A Compact Voicemeeter Remote App"
 authors = ["onyx-and-iris <code@onyxandiris.online>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/onyx-and-iris/voicemeeter-compact"
 
 packages = [{ include = "vmcompact" }]
 include = ["vmcompact/img/cat.ico"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-sv-ttk = "^2.5.1"
+sv-ttk = "^2.5.5"
 tomli = { version = "^2.0.1", python = "<3.11" }
-voicemeeter-api = "^2.3.2"
-vban-cmd = "^2.3.2"
+voicemeeter-api = "^2.4.4"
+vban-cmd = "^2.4.4"
 
 [tool.poetry.dev-dependencies]
 black = { version = "^22.6.0", allow-prereleases = true }
 isort = "^5.12.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `voicemeeter_compact-1.9.1/README.md` & `voicemeeter_compact-1.9.2/README.md`

 * *Files identical despite different names*

### Comparing `voicemeeter_compact-1.9.1/vmcompact/app.py` & `voicemeeter_compact-1.9.2/vmcompact/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,15 @@
         self._vmr.init_thread()
         icon_path = Path(__file__).parent.resolve() / "img" / "cat.ico"
         if icon_path.is_file():
             self.iconbitmap(str(icon_path))
         self.minsize(275, False)
         self.subject = Subject()
         self._configs = None
+        self.protocol("WM_DELETE_WINDOW", self.on_close_window)
         self.menu = self["menu"] = Menus(self, vmr)
         self.styletable = ttk.Style()
         if _configuration.config:
             vmr.apply_config(_configuration.config)
 
         self.build_app()
 
@@ -178,14 +179,19 @@
                         self.menu.menu_vban.entryconfig(j, state="normal")
                         for j, _ in enumerate(self.menu.menu_vban.winfo_children())
                     ]
                 else:
                     self.destroy()
         self.after(250, self.healthcheck_step)
 
+    def on_close_window(self):
+        if _base_values.vban_connected:
+            self._vban.logout()
+        self.destroy()
+
 
 _apps = {kind.name: App.make(kind) for kind in _kinds_all}
 
 
 def connect(kind_id: str, vmr) -> App:
     """return App of the kind requested"""
```

### Comparing `voicemeeter_compact-1.9.1/vmcompact/banner.py` & `voicemeeter_compact-1.9.2/vmcompact/banner.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_compact-1.9.1/vmcompact/builders.py` & `voicemeeter_compact-1.9.2/vmcompact/builders.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_compact-1.9.1/vmcompact/channels.py` & `voicemeeter_compact-1.9.2/vmcompact/channels.py`

 * *Files 5% similar despite different names*

```diff
@@ -147,25 +147,26 @@
                 f"{self.identifier}Mute{self.index}.TButton",
                 background=f'{"red" if  self.mute.get() else "white"}',
             )
 
     def sync_labels(self):
         """sync labelframes according to label text"""
         retval = self.getter("label")
-        self.parent.label_cache[self.id].insert(self.index, retval)
-        if len(retval) > 10:
-            retval = f"{retval[:8]}.."
-        if not retval:
-            self.parent.columnconfigure(self.index, minsize=0)
-            self.parent.parent.subject.remove(self)
-            self.grid_remove()
-        else:
-            self.parent.parent.subject.add(self)
-            self.grid()
-        self.configure(text=retval)
+        if self.parent.label_cache[self.id][self.index] != retval:
+            self.parent.label_cache[self.id][self.index] = retval
+            if len(retval) > 10:
+                retval = f"{retval[:8]}.."
+            if not retval:
+                self.parent.columnconfigure(self.index, minsize=0)
+                self.parent.parent.subject.remove(self)
+                self.grid_remove()
+            else:
+                self.parent.parent.subject.add(self)
+                self.grid()
+            self.configure(text=retval)
 
     def grid_configure(self):
         self.grid(padx=_configuration.channel_xpadding, sticky=(tk.N, tk.S))
         [
             child.grid_configure(padx=1, pady=1, sticky=(tk.W, tk.E))
             for child in self.winfo_children()
             if isinstance(child, ttk.Checkbutton)
@@ -224,23 +225,26 @@
         if self.index < self.parent.parent.kind.num_bus:
             if self.target.levels.is_updated or self.level.get() != -118:
                 val = max(self.target.levels.all)
                 self.level.set((0 if self.mute.get() else 72 + val - 12))
 
 
 class ChannelFrame(ttk.Frame):
-    label_cache = {"strip": list(), "bus": list()}
-
     def init(self, parent, id):
         super().__init__(parent)
         self.parent = parent
         self.id = id
         self.phys_in, self.virt_in = parent.kind.ins
         self.phys_out, self.virt_out = parent.kind.outs
+        self.label_cache = {
+            "strip": [""] * (self.phys_in + self.virt_in),
+            "bus": [""] * (self.phys_out + self.virt_out),
+        }
         self.parent.subject.add(self)
+        self.update_labels()
 
     @property
     def target(self):
         """returns the current interface"""
 
         return self.parent.target
 
@@ -254,21 +258,21 @@
 
         return tuple(
             frame
             for frame in self.winfo_children()
             if isinstance(frame, ttk.LabelFrame)
         )
 
+    def update_labels(self):
+        for labelframe in self.labelframes:
+            labelframe.on_update("labelframe")
+
     def on_update(self, subject):
         if subject == "pdirty":
-            target = getattr(self.target, self.id)
-            num = getattr(self.parent.kind, f"num_{self.id}")
-            if self.label_cache[self.id] != [target[i].label for i in range(num)]:
-                for labelframe in self.labelframes:
-                    labelframe.on_update("labelframe")
+            self.update_labels()
 
     def grid_configure(self):
         [
             self.columnconfigure(i, minsize=_configuration.channel_width)
             for i, _ in enumerate(self.labelframes)
         ]
         [self.rowconfigure(0, minsize=100) for i, _ in enumerate(self.labelframes)]
@@ -276,65 +280,69 @@
     def teardown(self):
         [self.parent.subject.remove(frame) for frame in self.labelframes]
         self.parent.subject.remove(self)
         self.destroy()
         setattr(self.parent, f"{self.identifier}_frame", None)
 
 
-def _make_channelframe(parent, id):
+def _make_channelframe(parent, identifier):
     """
     Creates a Channel Frame class of type strip or bus
     """
 
     phys_in, virt_in = parent.kind.ins
     phys_out, virt_out = parent.kind.outs
 
-    def init_labels(self, id):
+    def init_labels(self):
         """
         Grids each labelframe, grid_removes any without a label
         """
 
         for i, labelframe in enumerate(
-            getattr(self, "strips" if id == "strip" else "buses")
+            getattr(self, "strips" if identifier == "strip" else "buses")
         ):
             labelframe.grid(row=0, column=i)
-            if not labelframe.target.label:
+            label = labelframe.target.label
+            if not label:
                 self.columnconfigure(i, minsize=0)
                 labelframe.grid_remove()
+            self.label_cache[identifier][i] = label
 
     def init_strip(self, *args, **kwargs):
-        self.init(parent, id)
-        self.strips = tuple(Strip(self, i, id) for i in range(phys_in + virt_in))
+        self.init(parent, identifier)
+        self.strips = tuple(
+            Strip(self, i, identifier) for i in range(phys_in + virt_in)
+        )
         self.grid(row=0, column=0, sticky=(tk.W))
         self.grid_configure()
-        init_labels(self, id)
+        init_labels(self)
 
     def init_bus(self, *args, **kwargs):
-        self.init(parent, id)
-        self.buses = tuple(Bus(self, i, id) for i in range(phys_out + virt_out))
+        self.init(parent, identifier)
+        self.buses = tuple(Bus(self, i, identifier) for i in range(phys_out + virt_out))
         if _configuration.extended:
             if _configuration.extends_horizontal:
                 self.grid(row=0, column=2, sticky=(tk.W))
             else:
                 self.grid(row=2, column=0, sticky=(tk.W))
         else:
             self.grid(row=0, column=0)
         self.grid_configure()
-        init_labels(self, id)
+        init_labels(self)
 
-    if id == "strip":
+    if identifier == "strip":
         CHANNELFRAME_cls = type(
-            f"ChannelFrame{id.capitalize()}",
+            f"ChannelFrame{identifier.capitalize()}",
             (ChannelFrame,),
             {
                 "__init__": init_strip,
             },
         )
     else:
         CHANNELFRAME_cls = type(
-            f"ChannelFrame{id.capitalize()}",
+            f"ChannelFrame{identifier.capitalize()}",
             (ChannelFrame,),
             {
                 "__init__": init_bus,
             },
         )
     return CHANNELFRAME_cls(parent)
```

### Comparing `voicemeeter_compact-1.9.1/vmcompact/config.py` & `voicemeeter_compact-1.9.2/vmcompact/config.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_compact-1.9.1/vmcompact/configurations.py` & `voicemeeter_compact-1.9.2/vmcompact/configurations.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_compact-1.9.1/vmcompact/data.py` & `voicemeeter_compact-1.9.2/vmcompact/data.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_compact-1.9.1/vmcompact/gainlayer.py` & `voicemeeter_compact-1.9.2/vmcompact/gainlayer.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_compact-1.9.1/vmcompact/img/cat.ico` & `voicemeeter_compact-1.9.2/vmcompact/img/cat.ico`

 * *Files identical despite different names*

### Comparing `voicemeeter_compact-1.9.1/vmcompact/menu.py` & `voicemeeter_compact-1.9.2/vmcompact/menu.py`

 * *Files 1% similar despite different names*

```diff
@@ -223,15 +223,15 @@
             for j, _ in enumerate(self.menu_vban.winfo_children())
         ]
 
     def action_invoke_voicemeeter(self, cmd):
         if fn := getattr(self.target.command, cmd):
             fn()
         if cmd == "shutdown":
-            self.parent.destroy()
+            self.parent.on_close_window()
 
     def action_set_voicemeeter(self, cmd, val=True):
         if cmd == "lock":
             self._lock.set(val)
             self._unlock.set(not self._lock.get())
         setattr(self.target.command, cmd, val)
```

### Comparing `voicemeeter_compact-1.9.1/vmcompact/navigation.py` & `voicemeeter_compact-1.9.2/vmcompact/navigation.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_compact-1.9.1/vmcompact/subject.py` & `voicemeeter_compact-1.9.2/vmcompact/subject.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_compact-1.9.1/PKG-INFO` & `voicemeeter_compact-1.9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: voicemeeter-compact
-Version: 1.9.1
+Version: 1.9.2
 Summary: A Compact Voicemeeter Remote App
 Home-page: https://github.com/onyx-and-iris/voicemeeter-compact
 License: MIT
 Author: onyx-and-iris
 Author-email: code@onyxandiris.online
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: sv-ttk (>=2.5.1,<3.0.0)
+Requires-Dist: sv-ttk (>=2.5.5,<3.0.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0) ; python_version < "3.11"
-Requires-Dist: vban-cmd (>=2.3.2,<3.0.0)
-Requires-Dist: voicemeeter-api (>=2.3.2,<3.0.0)
+Requires-Dist: vban-cmd (>=2.4.4,<3.0.0)
+Requires-Dist: voicemeeter-api (>=2.4.4,<3.0.0)
 Project-URL: Repository, https://github.com/onyx-and-iris/voicemeeter-compact
 Description-Content-Type: text/markdown
 
 [![PyPI version](https://badge.fury.io/py/voicemeeter-compact.svg)](https://badge.fury.io/py/voicemeeter-compact)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/onyx-and-iris/voicemeeter-compact/blob/main/LICENSE)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 ![OS: Windows](https://img.shields.io/badge/os-windows-red)
```

