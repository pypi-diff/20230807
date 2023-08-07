# Comparing `tmp/yafti-0.7.0.tar.gz` & `tmp/yafti-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yafti-0.7.0.tar", max compression
+gzip compressed data, was "yafti-0.7.1.tar", max compression
```

## Comparing `yafti-0.7.0.tar` & `yafti-0.7.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0    11358 2023-07-05 23:37:24.939910 yafti-0.7.0/LICENSE
--rw-r--r--   0        0        0    10051 2023-07-05 23:37:24.939910 yafti-0.7.0/README.md
--rw-r--r--   0        0        0     1533 2023-07-05 23:37:24.939910 yafti-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      560 2023-07-05 23:37:24.939910 yafti-0.7.0/yafti/__init__.py
--rw-r--r--   0        0        0     1087 2023-07-05 23:37:24.939910 yafti-0.7.0/yafti/__main__.py
--rw-r--r--   0        0        0     2081 2023-07-05 23:37:24.939910 yafti-0.7.0/yafti/abc.py
--rw-r--r--   0        0        0     2455 2023-07-05 23:37:24.939910 yafti-0.7.0/yafti/app.py
--rw-r--r--   0        0        0     1813 2023-07-05 23:37:24.939910 yafti-0.7.0/yafti/events.py
--rw-r--r--   0        0        0      532 2023-07-05 23:37:24.939910 yafti-0.7.0/yafti/log.py
--rw-r--r--   0        0        0     1571 2023-07-05 23:37:24.939910 yafti-0.7.0/yafti/parser.py
--rw-r--r--   0        0        0     6823 2023-07-05 23:37:24.939910 yafti-0.7.0/yafti/plugin/flatpak.py
--rw-r--r--   0        0        0     3070 2023-07-05 23:37:24.939910 yafti-0.7.0/yafti/plugin/run.py
--rw-r--r--   0        0        0      302 2023-07-05 23:37:24.939910 yafti-0.7.0/yafti/registry.py
--rw-r--r--   0        0        0     3278 2023-07-05 23:37:24.939910 yafti-0.7.0/yafti/screen/consent.py
--rw-r--r--   0        0        0     2227 2023-07-05 23:37:24.939910 yafti-0.7.0/yafti/screen/console.py
--rw-r--r--   0        0        0     1817 2023-07-05 23:37:24.939910 yafti-0.7.0/yafti/screen/dialog.py
--rw-r--r--   0        0        0       50 2023-07-05 23:37:24.939910 yafti-0.7.0/yafti/screen/package/__init__.py
--rw-r--r--   0        0        0      317 2023-07-05 23:37:24.939910 yafti-0.7.0/yafti/screen/package/models.py
--rw-r--r--   0        0        0       98 2023-07-05 23:37:24.939910 yafti-0.7.0/yafti/screen/package/screen/__init__.py
--rw-r--r--   0        0        0     5232 2023-07-05 23:37:24.939910 yafti-0.7.0/yafti/screen/package/screen/install.py
--rw-r--r--   0        0        0     4021 2023-07-05 23:37:24.939910 yafti-0.7.0/yafti/screen/package/screen/package.py
--rw-r--r--   0        0        0     5522 2023-07-05 23:37:24.939910 yafti-0.7.0/yafti/screen/package/screen/picker.py
--rw-r--r--   0        0        0     1368 2023-07-05 23:37:24.939910 yafti-0.7.0/yafti/screen/package/state.py
--rw-r--r--   0        0        0      509 2023-07-05 23:37:24.939910 yafti-0.7.0/yafti/screen/package/utils.py
--rw-r--r--   0        0        0     3413 2023-07-05 23:37:24.939910 yafti-0.7.0/yafti/screen/title.py
--rw-r--r--   0        0        0     1214 2023-07-05 23:37:24.939910 yafti-0.7.0/yafti/screen/utils.py
--rw-r--r--   0        0        0     5216 2023-07-05 23:37:24.939910 yafti-0.7.0/yafti/screen/window.py
--rw-r--r--   0        0        0      448 2023-07-05 23:37:24.939910 yafti-0.7.0/yafti/setup.py
--rw-r--r--   0        0        0       32 2023-07-05 23:37:24.939910 yafti-0.7.0/yafti/share.py
--rw-r--r--   0        0        0    10948 1970-01-01 00:00:00.000000 yafti-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-08-07 03:05:28.278830 yafti-0.7.1/LICENSE
+-rw-r--r--   0        0        0    10051 2023-08-07 03:05:28.278830 yafti-0.7.1/README.md
+-rw-r--r--   0        0        0     1533 2023-08-07 03:05:28.282830 yafti-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0      560 2023-08-07 03:05:28.282830 yafti-0.7.1/yafti/__init__.py
+-rw-r--r--   0        0        0     1271 2023-08-07 03:05:28.282830 yafti-0.7.1/yafti/__main__.py
+-rw-r--r--   0        0        0     2081 2023-08-07 03:05:28.282830 yafti-0.7.1/yafti/abc.py
+-rw-r--r--   0        0        0     2534 2023-08-07 03:05:28.282830 yafti-0.7.1/yafti/app.py
+-rw-r--r--   0        0        0     1813 2023-08-07 03:05:28.282830 yafti-0.7.1/yafti/events.py
+-rw-r--r--   0        0        0      532 2023-08-07 03:05:28.282830 yafti-0.7.1/yafti/log.py
+-rw-r--r--   0        0        0     1571 2023-08-07 03:05:28.282830 yafti-0.7.1/yafti/parser.py
+-rw-r--r--   0        0        0     6823 2023-08-07 03:05:28.282830 yafti-0.7.1/yafti/plugin/flatpak.py
+-rw-r--r--   0        0        0     3070 2023-08-07 03:05:28.282830 yafti-0.7.1/yafti/plugin/run.py
+-rw-r--r--   0        0        0      302 2023-08-07 03:05:28.282830 yafti-0.7.1/yafti/registry.py
+-rw-r--r--   0        0        0     3278 2023-08-07 03:05:28.282830 yafti-0.7.1/yafti/screen/consent.py
+-rw-r--r--   0        0        0     2227 2023-08-07 03:05:28.282830 yafti-0.7.1/yafti/screen/console.py
+-rw-r--r--   0        0        0     1817 2023-08-07 03:05:28.282830 yafti-0.7.1/yafti/screen/dialog.py
+-rw-r--r--   0        0        0       50 2023-08-07 03:05:28.282830 yafti-0.7.1/yafti/screen/package/__init__.py
+-rw-r--r--   0        0        0      317 2023-08-07 03:05:28.282830 yafti-0.7.1/yafti/screen/package/models.py
+-rw-r--r--   0        0        0       98 2023-08-07 03:05:28.282830 yafti-0.7.1/yafti/screen/package/screen/__init__.py
+-rw-r--r--   0        0        0     5311 2023-08-07 03:05:28.282830 yafti-0.7.1/yafti/screen/package/screen/install.py
+-rw-r--r--   0        0        0     4270 2023-08-07 03:05:28.282830 yafti-0.7.1/yafti/screen/package/screen/package.py
+-rw-r--r--   0        0        0     5621 2023-08-07 03:05:28.282830 yafti-0.7.1/yafti/screen/package/screen/picker.py
+-rw-r--r--   0        0        0     1453 2023-08-07 03:05:28.282830 yafti-0.7.1/yafti/screen/package/state.py
+-rw-r--r--   0        0        0      653 2023-08-07 03:05:28.282830 yafti-0.7.1/yafti/screen/package/utils.py
+-rw-r--r--   0        0        0     3413 2023-08-07 03:05:28.282830 yafti-0.7.1/yafti/screen/title.py
+-rw-r--r--   0        0        0     1214 2023-08-07 03:05:28.282830 yafti-0.7.1/yafti/screen/utils.py
+-rw-r--r--   0        0        0     5216 2023-08-07 03:05:28.282830 yafti-0.7.1/yafti/screen/window.py
+-rw-r--r--   0        0        0      448 2023-08-07 03:05:28.282830 yafti-0.7.1/yafti/setup.py
+-rw-r--r--   0        0        0       32 2023-08-07 03:05:28.282830 yafti-0.7.1/yafti/share.py
+-rw-r--r--   0        0        0    10948 1970-01-01 00:00:00.000000 yafti-0.7.1/PKG-INFO
```

### Comparing `yafti-0.7.0/LICENSE` & `yafti-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yafti-0.7.0/README.md` & `yafti-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `yafti-0.7.0/pyproject.toml` & `yafti-0.7.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "yafti"
-version = "0.7.0"
+version = "0.7.1"
 description = "Yet another first time installer"
 authors = ["Marco Ceppi <marco@ceppi.net>"]
 license = "Apache 2.0"
 readme = "README.md"
 homepage = "https://github.com/ublue-os/yafti"
 repository = "https://github.com/ublue-os/yafti"
 classifiers = [
@@ -37,15 +37,15 @@
 "yafti.screen.console" = "yafti.screen.console:ConsoleScreen"
 "yafti.screen.consent" = "yafti.screen.consent:ConsentScreen"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 isort = "^5.12.0"
 pytest = "^7.2.1"
-ruff = ">=0.0.254,<0.0.271"
+ruff = ">=0.0.254,<0.0.283"
 coverage = "^7.2.1"
 pytest-cov = "^4.0.0"
 pytest-asyncio = ">=0.20.3,<0.22.0"
 
 [tool.isort]
 profile = "black"
 multi_line_output = 3
```

### Comparing `yafti-0.7.0/yafti/__init__.py` & `yafti-0.7.1/yafti/__init__.py`

 * *Files identical despite different names*

### Comparing `yafti-0.7.0/yafti/__main__.py` & `yafti-0.7.1/yafti/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,30 +11,37 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import logging
+from typing import Annotated
 
 import typer
 import yaml
 
 import yafti.setup  # noqa
 from yafti import log
 from yafti.app import Yafti
 from yafti.parser import Config
 
 
-def run(config: typer.FileText = typer.Argument("/etc/yafti.yml"), debug: bool = False):
+def run(
+    config: typer.FileText = typer.Argument("/etc/yafti.yml"),
+    debug: bool = False,
+    force_run: Annotated[
+        bool, typer.Option("-f", "--force", help="Ignore run mode and force run")
+    ] = False,
+):
     log.set_level(logging.DEBUG if debug else logging.INFO)
     log.debug("starting up", config=config, debug=debug)
     config = Config.parse_obj(yaml.safe_load(config))
     app = Yafti(config)
-    app.run(None)
+    app.run(None, force_run=force_run)
 
 
 def app():
     typer.run(run)
 
 
 if __name__ == "__main__":
```

### Comparing `yafti-0.7.0/yafti/abc.py` & `yafti-0.7.1/yafti/abc.py`

 * *Files identical despite different names*

### Comparing `yafti-0.7.0/yafti/app.py` & `yafti-0.7.1/yafti/app.py`

 * *Files 16% similar despite different names*

```diff
@@ -27,35 +27,36 @@
 
 class Yafti(Adw.Application):
     def __init__(self, cfg: Config = None, loop=None):
         super().__init__(application_id="it.ublue.Yafti")
         self.config = cfg
         self.loop = loop or gbulb.get_event_loop()
 
-    def run(self, *args, **kwargs):
+    def run(self, *args, force_run: bool = False, **kwargs):
         configured_mode = self.config.properties.mode
         _p: Path = self.config.properties.path.expanduser()
         # TODO(GH-#103): Remove this prior to 1.0 release. Start.
         _old_p = Path("~/.config/yafti-last-run").expanduser()
         if _old_p.exists() and _old_p.resolve() != _p.resolve():
             if not _p.parent.is_dir():
                 _p.parent.mkdir(mode=0o755, parents=True, exist_ok=True)
             if _p.is_file():
                 _p.unlink()
             _old_p.rename(_p)
         # TODO(GH-#103): End.
-        if configured_mode == YaftiRunModes.disable:
-            return
-
-        if configured_mode == YaftiRunModes.changed:
-            if _p.exists() and _p.read_text() == self.config_sha:
+        if not force_run:
+            if configured_mode == YaftiRunModes.disable:
                 return
 
-        if configured_mode == YaftiRunModes.ignore and _p.exists():
-            return
+            if configured_mode == YaftiRunModes.changed:
+                if _p.exists() and _p.read_text() == self.config_sha:
+                    return
+
+            if configured_mode == YaftiRunModes.ignore and _p.exists():
+                return
 
         super().run(*args, **kwargs)
 
     def do_activate(self):
         win = Window(application=self)
         win.present()
         self.loop.run()
```

### Comparing `yafti-0.7.0/yafti/events.py` & `yafti-0.7.1/yafti/events.py`

 * *Files identical despite different names*

### Comparing `yafti-0.7.0/yafti/log.py` & `yafti-0.7.1/yafti/log.py`

 * *Files identical despite different names*

### Comparing `yafti-0.7.0/yafti/parser.py` & `yafti-0.7.1/yafti/parser.py`

 * *Files identical despite different names*

### Comparing `yafti-0.7.0/yafti/plugin/flatpak.py` & `yafti-0.7.1/yafti/plugin/flatpak.py`

 * *Files identical despite different names*

### Comparing `yafti-0.7.0/yafti/plugin/run.py` & `yafti-0.7.1/yafti/plugin/run.py`

 * *Files identical despite different names*

### Comparing `yafti-0.7.0/yafti/screen/consent.py` & `yafti-0.7.1/yafti/screen/consent.py`

 * *Files identical despite different names*

### Comparing `yafti-0.7.0/yafti/screen/console.py` & `yafti-0.7.1/yafti/screen/console.py`

 * *Files identical despite different names*

### Comparing `yafti-0.7.0/yafti/screen/dialog.py` & `yafti-0.7.1/yafti/screen/dialog.py`

 * *Files identical despite different names*

### Comparing `yafti-0.7.0/yafti/screen/package/screen/install.py` & `yafti-0.7.1/yafti/screen/package/screen/install.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import Optional
 
 import yafti.share
 from yafti import events
 from yafti import log
 from yafti.abc import YaftiScreen
 from yafti.screen.console import ConsoleScreen
-from yafti.screen.package.state import STATE
+from yafti.screen.package.state import PackageScreenState
 
 _xml = """\
 <?xml version="1.0" encoding="UTF-8"?>
 <interface>
   <requires lib="gtk" version="4.0"/>
   <template class="YaftiPackageInstallScreen" parent="GtkBox">
     <property name="orientation">vertical</property>
@@ -73,26 +73,28 @@
     btn_console = Gtk.Template.Child()
     started = False
     already_run = False
     pulse = True
 
     def __init__(
         self,
+        id: str,
         title: str = "Package Installation",
         package_manager: str = "yafti.plugin.flatpak",
         package_manager_defaults: Optional[dict] = None,
         **kwargs,
     ):
         super().__init__(**kwargs)
         from yafti.registry import PLUGINS
 
         self.status_page.set_title(title)
         self.package_manager = PLUGINS.get(package_manager)
         self.package_manager_defaults = package_manager_defaults or {}
         self.btn_console.connect("clicked", self.toggle_console)
+        self.state = PackageScreenState(id)
 
     async def on_activate(self):
         if self.started or self.already_run:
             return
         self.console = ConsoleScreen()
         self.started = True
         events.on("btn_next", self.next)
@@ -110,15 +112,15 @@
         while self.pulse:
             self.pkg_progress.pulse()
             await asyncio.sleep(0.5)
 
     def draw(self):
         self.console.hide()
         self.append(self.console)
-        packages = [item.replace("pkg:", "") for item in STATE.get_on("pkg:")]
+        packages = [item.replace("pkg:", "") for item in self.state.get_on("pkg:")]
         asyncio.create_task(self.do_pulse())
         return self.install(packages)
 
     def run_package_manager(self, packge_config):
         try:
             config = json.loads(packge_config)
         except json.decoder.JSONDecodeError as e:
```

### Comparing `yafti-0.7.0/yafti/screen/package/screen/package.py` & `yafti-0.7.1/yafti/screen/package/screen/package.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from gi.repository import Adw, Gtk
 
 import yafti.share
 from yafti import events
 from yafti.abc import YaftiScreen, YaftiScreenConfig
 from yafti.screen.package.models import PackageConfig, PackageGroupConfig
 from yafti.screen.package.screen import PackageInstallScreen, PackagePickerScreen
-from yafti.screen.package.state import STATE
-from yafti.screen.package.utils import parse_packages
+from yafti.screen.package.state import PackageScreenState
+from yafti.screen.package.utils import parse_packages, generate_fingerprint
 
 _xml = """\
 <?xml version="1.0" encoding="UTF-8"?>
 <interface>
   <requires lib="gtk" version="4.0"/>
   <template class="YaftiPackageScreen" parent="AdwBin">
     <property name="halign">fill</property>
@@ -58,25 +58,30 @@
     ):
         super().__init__(**kwargs)
         self.title = title
         self.packages = groups or packages
         self.show_terminal = show_terminal
         self.package_manager = package_manager
         self.package_manager_defaults = package_manager_defaults
-        STATE.load(parse_packages(self.packages))
+        self.fingerprint = generate_fingerprint(self.packages)
+        self.state = PackageScreenState(self.fingerprint)
+        self.state.load(parse_packages(self.packages))
         self.pkg_carousel.connect("page-changed", self.changed)
         self.draw()
 
     def draw(self):
         self.pkg_carousel.append(
-            PackagePickerScreen(title=self.title, packages=self.packages)
+            PackagePickerScreen(
+                id=self.fingerprint, title=self.title, packages=self.packages
+            )
         )
         self.pkg_carousel.append(
             PackageInstallScreen(
                 title=self.title,
+                id=self.fingerprint,
                 package_manager=self.package_manager,
                 package_manager_defaults=self.package_manager_defaults,
             )
         )
 
     def on_activate(self):
         events.on("btn_next", self.next)
```

### Comparing `yafti-0.7.0/yafti/screen/package/screen/picker.py` & `yafti-0.7.1/yafti/screen/package/screen/picker.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from gi.repository import Adw, Gtk
 from pydantic import BaseModel
 
 from yafti import log
 from yafti.abc import YaftiScreen
 from yafti.screen.dialog import DialogBox
-from yafti.screen.package.state import STATE
+from yafti.screen.package.state import PackageScreenState
 from yafti.screen.utils import find_parent
 
 _xml = """\
 <?xml version="1.0" encoding="UTF-8"?>
 <interface>
   <requires lib="gtk" version="4.0"/>
   <template class="YaftiPackagePickerScreen" parent="AdwBin">
@@ -54,43 +54,45 @@
 
     class Config(BaseModel):
         title: str = "Package Installation"
         packages: list | dict
 
     def __init__(
         self,
+        id: str,
         title: str,
         packages: list | dict,
         **kwargs,
     ):
         super().__init__(**kwargs)
         self.status_page.set_title(title)
         self.packages = packages
+        self.state = PackageScreenState(id)
         self.draw()
 
     def draw(self):
         if isinstance(self.packages, list):
             # TODO: Implement a list of packages and not package groups
             return
 
         for name, details in self.packages.items():
             action_row = Adw.ActionRow(title=name, subtitle=details.get("description"))
 
             def state_set(group, _, value):
-                STATE.set(f"group:{group}", value)
+                self.state.set(f"group:{group}", value)
                 d = self.packages.get(group)
                 for pkg in d.get("packages", []):
                     for pkg_name in pkg.values():
                         if isinstance(pkg_name, dict):
                             pkg_name = json.dumps(pkg_name)
-                        STATE.set(f"pkg:{pkg_name}", value)
+                        self.state.set(f"pkg:{pkg_name}", value)
 
             state_set(name, None, details.get("default", True))
             _switcher = Gtk.Switch()
-            _switcher.set_active(STATE.get(f"group:{name}"))
+            _switcher.set_active(self.state.get(f"group:{name}"))
             _switcher.set_valign(Gtk.Align.CENTER)
 
             state_set_fn = partial(state_set, name)
             _switcher.connect("state-set", state_set_fn)
             action_row.add_suffix(_switcher)
 
             _customize = Gtk.Button()
@@ -144,18 +146,18 @@
             for name, pkg in item.items():
                 _apps_action_row = Adw.ActionRow(
                     title=name,
                 )
                 _app_switcher = Gtk.Switch()
                 if isinstance(pkg, dict):
                     pkg = json.dumps(pkg)
-                _app_switcher.set_active(STATE.get(f"pkg:{pkg}"))
+                _app_switcher.set_active(self.state.get(f"pkg:{pkg}"))
                 _app_switcher.set_valign(Gtk.Align.CENTER)
 
                 def set_state(pkg, btn, value):
                     log.debug("state-set", pkg=pkg, value=value)
-                    STATE.set(f"pkg:{pkg}", value)
+                    self.state.set(f"pkg:{pkg}", value)
 
                 set_state_func = partial(set_state, pkg)
                 _app_switcher.connect("state-set", set_state_func)
                 _apps_action_row.add_suffix(_app_switcher)
                 yield _apps_action_row
```

### Comparing `yafti-0.7.0/yafti/screen/package/state.py` & `yafti-0.7.1/yafti/screen/package/state.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from pydantic import validate_arguments
 
 
 class PackageScreenState:
     __slots__ = ["state"]
 
-    @classmethod
-    def from_dict(cls, data: dict) -> "PackageScreenState":
-        self = cls()
-        self.load(data)
-        return self
+    def __new__(cls, id: str):
+        if not hasattr(cls, "instances"):
+            cls.instances = {}
+        if id not in cls.instances:
+            cls.instances[id] = super(PackageScreenState, cls).__new__(cls)
+        return cls.instances[id]
+
+    def __init__(self, id: str):
+        self.state = {}
 
     @validate_arguments
     def load(self, data: dict):
         for k, v in data.items():
             self.set(k, v)
 
-    def __init__(self):
-        self.state = {}
-
     @validate_arguments
     def remove(self, item: str) -> None:
         del self.state[item]
 
     @validate_arguments
     def on(self, item: str) -> None:
         self.set(item, True)
@@ -49,10 +50,7 @@
 
     def keys(self) -> list[str]:
         return list(self.state.keys())
 
     @validate_arguments
     def get(self, item: str) -> bool:
         return self.state.get(item)
-
-
-STATE = PackageScreenState()
```

### Comparing `yafti-0.7.0/yafti/screen/title.py` & `yafti-0.7.1/yafti/screen/title.py`

 * *Files identical despite different names*

### Comparing `yafti-0.7.0/yafti/screen/utils.py` & `yafti-0.7.1/yafti/screen/utils.py`

 * *Files identical despite different names*

### Comparing `yafti-0.7.0/yafti/screen/window.py` & `yafti-0.7.1/yafti/screen/window.py`

 * *Files identical despite different names*

### Comparing `yafti-0.7.0/PKG-INFO` & `yafti-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yafti
-Version: 0.7.0
+Version: 0.7.1
 Summary: Yet another first time installer
 Home-page: https://github.com/ublue-os/yafti
 License: Apache 2.0
 Author: Marco Ceppi
 Author-email: marco@ceppi.net
 Requires-Python: >=3.11,<4.0
 Classifier: Environment :: X11 Applications :: GTK
```

