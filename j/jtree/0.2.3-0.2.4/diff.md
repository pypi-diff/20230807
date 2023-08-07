# Comparing `tmp/jtree-0.2.3.tar.gz` & `tmp/jtree-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jtree-0.2.3.tar", last modified: Tue Dec 27 02:58:23 2022, max compression
+gzip compressed data, was "jtree-0.2.4.tar", last modified: Mon Aug  7 10:40:24 2023, max compression
```

## Comparing `jtree-0.2.3.tar` & `jtree-0.2.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2022-12-27 02:58:23.075802 jtree-0.2.3/
--rw-rw-rw-   0        0        0      891 2022-12-24 06:23:48.000000 jtree-0.2.3/.editorconfig
-drwxrwxrwx   0        0        0        0 2022-12-27 02:58:22.153486 jtree-0.2.3/.github/
-drwxrwxrwx   0        0        0        0 2022-12-27 02:58:22.278482 jtree-0.2.3/.github/workflows/
--rw-rw-rw-   0        0        0      857 2022-12-26 07:38:58.000000 jtree-0.2.3/.github/workflows/check.yml
--rw-rw-rw-   0        0        0      121 2022-12-26 05:55:24.000000 jtree-0.2.3/.gitignore
--rw-rw-rw-   0        0        0     1079 2022-12-11 08:08:30.000000 jtree-0.2.3/LICENSE
--rw-rw-rw-   0        0        0      117 2022-12-24 04:38:05.000000 jtree-0.2.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2711 2022-12-27 02:58:23.060178 jtree-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0      638 2022-12-15 10:37:59.000000 jtree-0.2.3/README.md
-drwxrwxrwx   0        0        0        0 2022-12-27 02:58:22.356610 jtree-0.2.3/jtree/
--rw-rw-rw-   0        0        0     2149 2022-12-27 02:56:48.000000 jtree-0.2.3/jtree/__init__.py
--rw-rw-rw-   0        0        0     1858 2022-12-27 02:23:07.000000 jtree-0.2.3/jtree/__main__.py
-drwxrwxrwx   0        0        0        0 2022-12-27 02:58:23.028931 jtree-0.2.3/jtree/css/
--rw-rw-rw-   0        0        0      318 2022-12-27 02:18:41.000000 jtree-0.2.3/jtree/css/layout.css
--rw-rw-rw-   0        0        0     1891 2022-12-27 02:46:31.000000 jtree-0.2.3/jtree/widgets.py
-drwxrwxrwx   0        0        0        0 2022-12-27 02:58:23.028931 jtree-0.2.3/jtree.egg-info/
--rw-rw-rw-   0        0        0     2711 2022-12-27 02:58:21.000000 jtree-0.2.3/jtree.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      395 2022-12-27 02:58:22.000000 jtree-0.2.3/jtree.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-27 02:58:21.000000 jtree-0.2.3/jtree.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2022-12-27 02:58:21.000000 jtree-0.2.3/jtree.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      142 2022-12-27 02:58:21.000000 jtree-0.2.3/jtree.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2022-12-27 02:58:21.000000 jtree-0.2.3/jtree.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1848 2022-12-27 02:56:48.000000 jtree-0.2.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-12-27 02:58:23.075802 jtree-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0       41 2022-12-11 09:12:14.000000 jtree-0.2.3/setup.py
-drwxrwxrwx   0        0        0        0 2022-12-27 02:58:22.169106 jtree-0.2.3/tests/
-drwxrwxrwx   0        0        0        0 2022-12-27 02:58:23.044557 jtree-0.2.3/tests/fixtures/
--rw-rw-rw-   0        0        0     6360 2022-12-13 16:23:20.000000 jtree-0.2.3/tests/fixtures/deployment.json
--rw-rw-rw-   0        0        0      418 2022-12-26 23:09:05.000000 jtree-0.2.3/tox.ini
+drwxrwxrwx   0        0        0        0 2023-08-07 10:40:24.033728 jtree-0.2.4/
+-rw-rw-rw-   0        0        0      891 2023-08-07 09:28:39.000000 jtree-0.2.4/.editorconfig
+drwxrwxrwx   0        0        0        0 2023-08-07 10:40:23.377614 jtree-0.2.4/.github/
+drwxrwxrwx   0        0        0        0 2023-08-07 10:40:23.689691 jtree-0.2.4/.github/workflows/
+-rw-rw-rw-   0        0        0      857 2023-08-07 09:28:39.000000 jtree-0.2.4/.github/workflows/check.yml
+-rw-rw-rw-   0        0        0      121 2023-08-07 09:28:39.000000 jtree-0.2.4/.gitignore
+-rw-rw-rw-   0        0        0     1099 2023-08-07 09:28:39.000000 jtree-0.2.4/LICENSE
+-rw-rw-rw-   0        0        0      117 2023-08-07 09:28:39.000000 jtree-0.2.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     2711 2023-08-07 10:40:24.028146 jtree-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0      638 2023-08-07 09:28:39.000000 jtree-0.2.4/README.md
+drwxrwxrwx   0        0        0        0 2023-08-07 10:40:23.759236 jtree-0.2.4/jtree/
+-rw-rw-rw-   0        0        0     1975 2023-08-07 10:23:22.000000 jtree-0.2.4/jtree/__init__.py
+-rw-rw-rw-   0        0        0     1836 2023-08-07 09:28:39.000000 jtree-0.2.4/jtree/__main__.py
+drwxrwxrwx   0        0        0        0 2023-08-07 10:40:24.018126 jtree-0.2.4/jtree/css/
+-rw-rw-rw-   0        0        0      318 2023-08-07 09:28:39.000000 jtree-0.2.4/jtree/css/layout.css
+-rw-rw-rw-   0        0        0     1924 2023-08-07 09:58:38.000000 jtree-0.2.4/jtree/widgets.py
+drwxrwxrwx   0        0        0        0 2023-08-07 10:40:24.013130 jtree-0.2.4/jtree.egg-info/
+-rw-rw-rw-   0        0        0     2711 2023-08-07 10:40:22.000000 jtree-0.2.4/jtree.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      395 2023-08-07 10:40:23.000000 jtree-0.2.4/jtree.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 10:40:22.000000 jtree-0.2.4/jtree.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-08-07 10:40:22.000000 jtree-0.2.4/jtree.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      142 2023-08-07 10:40:22.000000 jtree-0.2.4/jtree.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-08-07 10:40:22.000000 jtree-0.2.4/jtree.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1848 2023-08-07 10:23:22.000000 jtree-0.2.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-07 10:40:24.034685 jtree-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0       41 2023-08-07 09:28:39.000000 jtree-0.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 10:40:23.564887 jtree-0.2.4/tests/
+drwxrwxrwx   0        0        0        0 2023-08-07 10:40:24.023128 jtree-0.2.4/tests/fixtures/
+-rw-rw-rw-   0        0        0     6360 2023-08-07 09:28:39.000000 jtree-0.2.4/tests/fixtures/deployment.json
+-rw-rw-rw-   0        0        0      418 2023-08-07 09:28:39.000000 jtree-0.2.4/tox.ini
```

### Comparing `jtree-0.2.3/.editorconfig` & `jtree-0.2.4/.editorconfig`

 * *Files identical despite different names*

### Comparing `jtree-0.2.3/.github/workflows/check.yml` & `jtree-0.2.4/.github/workflows/check.yml`

 * *Files identical despite different names*

### Comparing `jtree-0.2.3/LICENSE` & `jtree-0.2.4/LICENSE`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022 Oleksis Fraga Menéndez
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) 2022 Oleksis Fraga Menéndez
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `jtree-0.2.3/PKG-INFO` & `jtree-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jtree
-Version: 0.2.3
+Version: 0.2.4
 Summary: jtree is a command line interface (CLI) for displaying JavaScript Object Notation (JSON) in a tree view
 Author-email: Oleksis Fraga Menéndez <oleksis.fraga@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Oleksis Fraga Menéndez
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `jtree-0.2.3/README.md` & `jtree-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `jtree-0.2.3/jtree/__init__.py` & `jtree-0.2.4/jtree/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 from __future__ import annotations
 
 import json
 import sys
-import tempfile
 from typing import TYPE_CHECKING
 
 from textual.app import App, ComposeResult
 from textual.binding import Binding
 from textual.containers import Container
 from textual.widgets import Footer, Header
 
 from jtree.widgets import JSONDocument, JSONTree, TreeView
 
 if TYPE_CHECKING:
     from io import TextIOWrapper
 
 __prog_name__ = "jtree"
-__version__ = "0.2.3"
+__version__ = "0.2.4"
 
 
 class JSONTreeApp(App):
     TITLE = __prog_name__
     SUB_TITLE = f"A JSON Tree Viewer ({__version__})"
     CSS_PATH = "css/layout.css"
 
@@ -34,22 +33,21 @@
         self,
         json_file: TextIOWrapper,
         driver_class=None,
         css_path=None,
         watch_css=False,
     ):
         super().__init__(driver_class, css_path, watch_css)
-        with tempfile.TemporaryFile() as fp_temp:
-            if json_file is sys.stdin:
-                fp_temp.write(sys.stdin.read().encode(encoding="utf-8"))
-            else:
-                fp_temp.write(json_file.read().encode(encoding="utf-8"))
-                json_file.close()
-            fp_temp.seek(0)
-            self.json_data = fp_temp.read().decode("utf-8")
+        self.json_data: str = ""
+
+        if json_file is sys.stdin:
+            self.json_data = "".join(sys.stdin.readlines())
+        else:
+            self.json_data = json_file.read()
+            json_file.close()
 
     def compose(self) -> ComposeResult:
         yield Header()
         yield Container(
             TreeView(id="tree-view"), JSONDocument(id="json-document"), id="app-grid"
         )
         yield Footer()
```

### Comparing `jtree-0.2.3/jtree/__main__.py` & `jtree-0.2.4/jtree/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,14 @@
         default=sys.stdin,
     )
     parser.add_argument(
         "--log", nargs="?", help="Log level for enable debugpy", default="INFO"
     )
 
     args = parser.parse_args()
-    json_data = None
     numeric_level = getattr(logging, args.log.upper(), None)
 
     if not isinstance(numeric_level, int):
         print(f"Invalid log level {args.log!r}")
 
     if numeric_level == logging.DEBUG:
         import debugpy
```

### Comparing `jtree-0.2.3/jtree/widgets.py` & `jtree-0.2.4/jtree/widgets.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from __future__ import annotations
 
 from rich.highlighter import ReprHighlighter
 from rich.syntax import Syntax
 from rich.text import Text
 from textual.app import ComposeResult
 from textual.widget import Widget
-from textual.widgets import Static, Tree, TreeNode
+from textual.widgets import Static, Tree
+from textual.widgets.tree import TreeNode
 
 highlighter = ReprHighlighter()
 
 
 class JSONDocument(Static):
     def load(self, json_data) -> bool:
         try:
```

### Comparing `jtree-0.2.3/jtree.egg-info/PKG-INFO` & `jtree-0.2.4/jtree.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jtree
-Version: 0.2.3
+Version: 0.2.4
 Summary: jtree is a command line interface (CLI) for displaying JavaScript Object Notation (JSON) in a tree view
 Author-email: Oleksis Fraga Menéndez <oleksis.fraga@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Oleksis Fraga Menéndez
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `jtree-0.2.3/pyproject.toml` & `jtree-0.2.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jtree"
-version = "0.2.3"
+version = "0.2.4"
 description = "jtree is a command line interface (CLI) for displaying JavaScript Object Notation (JSON) in a tree view"
 readme = "README.md"
 authors = [{ name = "Oleksis Fraga Menéndez", email = "oleksis.fraga@gmail.com" }]
 urls.Homepage = "https://github.com/oleksis/jtree"
 urls.Tracker = "https://github.com/oleksis/jtree/issues"
 license = { file = "LICENSE" }
 classifiers = [
@@ -41,15 +41,15 @@
 
 [tool.setuptools.packages.find]
 where = ["."]
 include = ["jtree*"]
 exclude = ["jtree.tests*"]
 
 [tool.bumpver]
-current_version = "0.2.3"
+current_version = "0.2.4"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `jtree-0.2.3/tests/fixtures/deployment.json` & `jtree-0.2.4/tests/fixtures/deployment.json`

 * *Files identical despite different names*

