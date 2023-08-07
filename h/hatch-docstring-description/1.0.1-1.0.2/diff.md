# Comparing `tmp/hatch_docstring_description-1.0.1.tar.gz` & `tmp/hatch_docstring_description-1.0.2.tar.gz`

## Comparing `hatch_docstring_description-1.0.1.tar` & `hatch_docstring_description-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,17 @@
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 hatch_docstring_description-1.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 hatch_docstring_description-1.0.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 hatch_docstring_description-1.0.1/.github/workflows/pub.yml
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 hatch_docstring_description-1.0.1/.vscode/launch.json
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 hatch_docstring_description-1.0.1/.vscode/settings.json
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 hatch_docstring_description-1.0.1/src/hatch_docstring_description/__init__.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 hatch_docstring_description-1.0.1/src/hatch_docstring_description/hooks.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_docstring_description-1.0.1/src/hatch_docstring_description/py.typed
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 hatch_docstring_description-1.0.1/src/hatch_docstring_description/read_description.py
--rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 hatch_docstring_description-1.0.1/tests/test_basic.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 hatch_docstring_description-1.0.1/.gitignore
--rw-r--r--   0        0        0    34893 2020-02-02 00:00:00.000000 hatch_docstring_description-1.0.1/LICENSE.md
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 hatch_docstring_description-1.0.1/README.rst
--rw-r--r--   0        0        0     2254 2020-02-02 00:00:00.000000 hatch_docstring_description-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 hatch_docstring_description-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 hatch_docstring_description-1.0.2/.editorconfig
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 hatch_docstring_description-1.0.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 hatch_docstring_description-1.0.2/.prettierrc.yaml
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 hatch_docstring_description-1.0.2/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 hatch_docstring_description-1.0.2/.github/workflows/pub.yml
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 hatch_docstring_description-1.0.2/.vscode/launch.json
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 hatch_docstring_description-1.0.2/.vscode/settings.json
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 hatch_docstring_description-1.0.2/src/hatch_docstring_description/__init__.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 hatch_docstring_description-1.0.2/src/hatch_docstring_description/hooks.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_docstring_description-1.0.2/src/hatch_docstring_description/py.typed
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 hatch_docstring_description-1.0.2/src/hatch_docstring_description/read_description.py
+-rw-r--r--   0        0        0     3956 2020-02-02 00:00:00.000000 hatch_docstring_description-1.0.2/tests/test_basic.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 hatch_docstring_description-1.0.2/.gitignore
+-rw-r--r--   0        0        0    34893 2020-02-02 00:00:00.000000 hatch_docstring_description-1.0.2/LICENSE.md
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 hatch_docstring_description-1.0.2/README.rst
+-rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 hatch_docstring_description-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 hatch_docstring_description-1.0.2/PKG-INFO
```

### Comparing `hatch_docstring_description-1.0.1/.github/workflows/ci.yml` & `hatch_docstring_description-1.0.2/.github/workflows/ci.yml`

 * *Files 22% similar despite different names*

```diff
@@ -3,29 +3,32 @@
 on:
   push:
     branches: [main]
   pull_request:
     branches: [main]
 
 env:
-  FORCE_COLOR: '1'
+  FORCE_COLOR: "1"
 
 concurrency:
   group: ${{ github.workflow }}-${{ github.event.pull_request.number || github.sha }}
   cancel-in-progress: true
 
 jobs:
   test:
     runs-on: ubuntu-latest
+    strategy:
+      matrix:
+        python-version: ["3.8", "3.11"]
     steps:
-    - uses: actions/checkout@v3
-    - uses: actions/setup-python@v4
-      with:
-        python-version: '3.11'
-        cache: 'pip'
-    - run: pipx install hatch
-    - run: pip install -e .
-    - run: hatch run cov
-    - uses: codecov/codecov-action@v3
-      with:
-        files: .cache/coverage.xml
-        token: ${{ secrets.CODECOV_TOKEN }}
+      - uses: actions/checkout@v3
+      - uses: actions/setup-python@v4
+        with:
+          python-version: ${{ matrix.python-version }}
+          cache: "pip"
+      - run: pipx install hatch
+      - run: pip install -e .
+      - run: hatch run cov
+      - uses: codecov/codecov-action@v3
+        with:
+          files: .cache/coverage.xml
+          token: ${{ secrets.CODECOV_TOKEN }}
```

### Comparing `hatch_docstring_description-1.0.1/src/hatch_docstring_description/read_description.py` & `hatch_docstring_description-1.0.2/src/hatch_docstring_description/read_description.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,41 @@
+"""Implementation of the hook class."""
+
+from __future__ import annotations
+
 import ast
 from pathlib import Path
-from typing import Any, cast
+from typing import Any
 
-from hatchling.builders.wheel import WheelBuilder
+from hatchling.builders.wheel import WheelBuilder, WheelBuilderConfig
 from hatchling.metadata.plugin.interface import MetadataHookInterface
 
 
 class ReadDescriptionHook(MetadataHookInterface):
     """Metadata hook reading the first sentence of the docstring into `description`."""
 
     PLUGIN_NAME = "docstring-description"
 
     def update(self, metadata: dict[str, Any]) -> None:
         """See https://ofek.dev/hatch/latest/plugins/metadata-hook/ for more information."""
-
         if "description" in metadata or "description" not in metadata.get("dynamic", []):
             msg = "You need to add 'description' to your `dynamic` fields and not to `[project]`."
             raise TypeError(msg)
 
         if self.config.get("path"):
             path = Path(self.root) / self.config["path"]
         else:
-            packages = cast(list[str], WheelBuilder(self.root).config.packages)
-            if len(packages) != 1:
-                msg = "Multiple packages not supported" if len(packages) > 1 else f"No packages found in {self.root}"
+            cfg: WheelBuilderConfig = WheelBuilder(self.root).config
+            if len(cfg.packages) != 1:
+                msg = (
+                    "Multiple packages not supported" if len(cfg.packages) > 1 else f"No packages found in {self.root}"
+                )
                 raise RuntimeError(msg)
-            stem = Path(self.root) / packages[0]
+            stem = Path(self.root) / cfg.packages[0]
             path = (stem / "__init__.py") if stem.is_dir() else stem.with_name(f"{stem.name}.py")
         metadata["description"] = read_description(path)
 
 
 def read_description(pkg_file: Path) -> str:
-    """Returns the first sentence of the docstring."""
+    """Return the first sentence of the docstring."""
     mod = ast.parse(pkg_file.read_text(), pkg_file)
     return ast.get_docstring(mod)
```

### Comparing `hatch_docstring_description-1.0.1/LICENSE.md` & `hatch_docstring_description-1.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hatch_docstring_description-1.0.1/README.rst` & `hatch_docstring_description-1.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `hatch_docstring_description-1.0.1/pyproject.toml` & `hatch_docstring_description-1.0.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 requires = ["hatchling", "hatch-vcs"]
 build-backend = "hatchling.build"
 
 [project]
 name = "hatch-docstring-description"
 dynamic = ["version", "description"]
 readme = "README.rst"
-requires-python = ">=3.9"
+requires-python = ">=3.8"
 license = "GPL-3.0-or-later"
 authors = [
-  { name = "Philipp A.", email = "flying-sheep@web.de" },
+    { name = "Philipp A.", email = "flying-sheep@web.de" },
 ]
 # urls.Documentation = "https://github.com/flying-sheep/hatch-docstring-description#readme"
 urls.Issues = "https://github.com/flying-sheep/hatch-docstring-description/issues"
 urls.Source = "https://github.com/flying-sheep/hatch-docstring-description"
 classifiers = [
-  "Development Status :: 4 - Beta",
-  "Programming Language :: Python",
-  "Programming Language :: Python :: 3",
-  "Framework :: Hatch",
+    "Development Status :: 4 - Beta",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3",
+    "Framework :: Hatch",
 ]
 dependencies = ["hatchling"]
 
 [project.entry-points.hatch]
 docstring-description = "hatch_docstring_description.hooks"
 
 [tool.hatch.version]
@@ -33,72 +33,55 @@
   "coverage[toml]>=6.5",
   "pytest",
 ]
 [tool.hatch.envs.default.scripts]
 test = "pytest {args:tests}"
 test-cov = "coverage run -m pytest {args:tests}"
 cov-report = [
-  "- coverage combine",
-  "coverage xml",
-  "coverage report",
+    "- coverage combine",
+    "coverage xml",
+    "coverage report",
 ]
 cov = [
-  "test-cov",
-  "cov-report",
+    "test-cov",
+    "cov-report",
 ]
 
 [[tool.hatch.envs.all.matrix]]
 python = ["3.8", "3.9", "3.10", "3.11"]
 
 [tool.black]
 line-length = 120
 
 [tool.ruff]
 line-length = 120
-select = [
-  "A",
-  "ARG",
-  "B",
-  "C",
-  "DTZ",
-  "E",
-  "EM",
-  "F",
-  "FBT",
-  "I",
-  "ICN",
-  "ISC",
-  "N",
-  "PLC",
-  "PLE",
-  "PLR",
-  "PLW",
-  "Q",
-  "RUF",
-  "S",
-  "T",
-  "TID",
-  "UP",
-  "W",
-  "YTT",
-]
+select = ["ALL"]
 ignore = [
-  # Allow dict() syntax
-  "C408",
-  # Ignore checks for possible passwords
-  "S105", "S106", "S107",
+    # No self types
+    "ANN101",
+    # Allow dict() syntax
+    "C408",
+    # Mutually exclusive checks
+    "D203", "D213",
+    # TODO comments are OK
+    "FIX002",
+    # Ignore checks for possible passwords
+    "S105", "S106", "S107",
 ]
+allowed-confusables = ["’", "×"]
 
 [tool.ruff.isort]
 known-first-party = ["hatch_docstring_description"]
 
 [tool.ruff.per-file-ignores]
 "tests/**/*" = [
-  "ARG001", # fixtures can look like unused parameters
-  "S101", # tests can use magic values
+    "ARG001", # fixtures can look like unused parameters
+    "D103", # test functions don’t need docstrings
+    "INP001", # test directories shouldn’t contain __init__.py
+    "S101", # tests can use magic values
 ]
 
 [tool.coverage.run]
 source_pkgs = ["hatch_docstring_description"]
 branch = true
 parallel = true
 data_file = ".cache/coverage"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `hatch_docstring_description-1.0.1/PKG-INFO` & `hatch_docstring_description-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: hatch-docstring-description
-Version: 1.0.1
+Version: 1.0.2
 Project-URL: Issues, https://github.com/flying-sheep/hatch-docstring-description/issues
 Project-URL: Source, https://github.com/flying-sheep/hatch-docstring-description
 Author-email: "Philipp A." <flying-sheep@web.de>
 License-Expression: GPL-3.0-or-later
 License-File: LICENSE.md
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Hatch
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Requires-Dist: hatchling
 Description-Content-Type: text/x-rst
 
 hatch-docstring-description
 ===========================
 
 |PyPI Version| |PyPI Python Version| |Coverage|
```

