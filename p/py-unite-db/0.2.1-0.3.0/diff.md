# Comparing `tmp/py-unite-db-0.2.1.tar.gz` & `tmp/py-unite-db-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-unite-db-0.2.1.tar", last modified: Mon Jan 10 18:11:25 2022, max compression
+gzip compressed data, was "py-unite-db-0.3.0.tar", last modified: Mon Aug  7 10:25:41 2023, max compression
```

## Comparing `py-unite-db-0.2.1.tar` & `py-unite-db-0.3.0.tar`

### file list

```diff
@@ -1,30 +1,31 @@
--rw-r--r--   0 runner    (1001) docker     (121)    18093 2022-01-10 18:09:40.917044 py-unite-db-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2986 2022-01-10 18:09:40.917044 py-unite-db-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      558 2022-01-10 18:11:20.991781 py-unite-db-0.2.1/py_unite_db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3320 2022-01-10 18:09:40.917044 py-unite-db-0.2.1/py_unite_db/api_base.py
--rw-r--r--   0 runner    (1001) docker     (121)      396 2022-01-10 18:09:40.917044 py-unite-db-0.2.1/py_unite_db/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      697 2022-01-10 18:09:40.917044 py-unite-db-0.2.1/py_unite_db/models/base_model.py
--rw-r--r--   0 runner    (1001) docker     (121)      640 2022-01-10 18:09:40.917044 py-unite-db-0.2.1/py_unite_db/models/battle_item.py
--rw-r--r--   0 runner    (1001) docker     (121)     2830 2022-01-10 18:09:40.917044 py-unite-db-0.2.1/py_unite_db/models/held_item.py
--rw-r--r--   0 runner    (1001) docker     (121)      566 2022-01-10 18:09:40.917044 py-unite-db-0.2.1/py_unite_db/models/item.py
--rw-r--r--   0 runner    (1001) docker     (121)     3828 2022-01-10 18:09:40.917044 py-unite-db-0.2.1/py_unite_db/models/pokemon.py
--rw-r--r--   0 runner    (1001) docker     (121)      570 2022-01-10 18:09:40.917044 py-unite-db-0.2.1/py_unite_db/models/stats.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-10 18:09:40.917044 py-unite-db-0.2.1/py_unite_db/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)      374 2022-01-10 18:09:40.917044 py-unite-db-0.2.1/py_unite_db/types.py
--rw-r--r--   0 runner    (1001) docker     (121)     2188 2022-01-10 18:09:40.917044 py-unite-db-0.2.1/py_unite_db/unite_db.py
--rw-r--r--   0 runner    (1001) docker     (121)     1752 2022-01-10 18:09:40.917044 py-unite-db-0.2.1/py_unite_db/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1809 2022-01-10 18:11:21.003781 py-unite-db-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-10 18:09:40.917044 py-unite-db-0.2.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1134 2022-01-10 18:09:40.917044 py-unite-db-0.2.1/tests/mock_unite_db.py
--rw-r--r--   0 runner    (1001) docker     (121)      218 2022-01-10 18:09:40.917044 py-unite-db-0.2.1/tests/responses/battle_items.json
--rw-r--r--   0 runner    (1001) docker     (121)      695 2022-01-10 18:09:40.917044 py-unite-db-0.2.1/tests/responses/held_items.json
--rw-r--r--   0 runner    (1001) docker     (121)      972 2022-01-10 18:09:40.917044 py-unite-db-0.2.1/tests/responses/held_items_2.json
--rw-r--r--   0 runner    (1001) docker     (121)    40039 2022-01-10 18:09:40.917044 py-unite-db-0.2.1/tests/responses/pokemon.json
--rw-r--r--   0 runner    (1001) docker     (121)    40637 2022-01-10 18:09:40.917044 py-unite-db-0.2.1/tests/responses/pokemon_2.json
--rw-r--r--   0 runner    (1001) docker     (121)     4591 2022-01-10 18:09:40.917044 py-unite-db-0.2.1/tests/responses/stats.json
--rw-r--r--   0 runner    (1001) docker     (121)     4579 2022-01-10 18:09:40.917044 py-unite-db-0.2.1/tests/responses/stats_2.json
--rw-r--r--   0 runner    (1001) docker     (121)      411 2022-01-10 18:09:40.917044 py-unite-db-0.2.1/tests/test_battle_items.py
--rw-r--r--   0 runner    (1001) docker     (121)     1708 2022-01-10 18:09:40.917044 py-unite-db-0.2.1/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (121)      609 2022-01-10 18:09:40.917044 py-unite-db-0.2.1/tests/test_held_items.py
--rw-r--r--   0 runner    (1001) docker     (121)     1161 2022-01-10 18:09:40.917044 py-unite-db-0.2.1/tests/test_pokemon.py
--rw-------   0 runner    (1001) docker     (121)     4179 2022-01-10 18:11:25.243728 py-unite-db-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    18093 2023-08-07 10:24:23.887673 py-unite-db-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2986 2023-08-07 10:24:23.887673 py-unite-db-0.3.0/README.md
+-rw-r--r--   0        0        0      558 2023-08-07 10:25:37.675930 py-unite-db-0.3.0/py_unite_db/__init__.py
+-rw-r--r--   0        0        0     3320 2023-08-07 10:24:23.891673 py-unite-db-0.3.0/py_unite_db/api_base.py
+-rw-r--r--   0        0        0      396 2023-08-07 10:24:23.891673 py-unite-db-0.3.0/py_unite_db/models/__init__.py
+-rw-r--r--   0        0        0      672 2023-08-07 10:24:23.891673 py-unite-db-0.3.0/py_unite_db/models/base_model.py
+-rw-r--r--   0        0        0      640 2023-08-07 10:24:23.891673 py-unite-db-0.3.0/py_unite_db/models/battle_item.py
+-rw-r--r--   0        0        0     2830 2023-08-07 10:24:23.891673 py-unite-db-0.3.0/py_unite_db/models/held_item.py
+-rw-r--r--   0        0        0      566 2023-08-07 10:24:23.891673 py-unite-db-0.3.0/py_unite_db/models/item.py
+-rw-r--r--   0        0        0     3828 2023-08-07 10:24:23.891673 py-unite-db-0.3.0/py_unite_db/models/pokemon.py
+-rw-r--r--   0        0        0      570 2023-08-07 10:24:23.891673 py-unite-db-0.3.0/py_unite_db/models/stats.py
+-rw-r--r--   0        0        0        0 2023-08-07 10:24:23.891673 py-unite-db-0.3.0/py_unite_db/py.typed
+-rw-r--r--   0        0        0      379 2023-08-07 10:24:23.891673 py-unite-db-0.3.0/py_unite_db/types.py
+-rw-r--r--   0        0        0     2300 2023-08-07 10:24:23.891673 py-unite-db-0.3.0/py_unite_db/unite_db.py
+-rw-r--r--   0        0        0     1752 2023-08-07 10:24:23.891673 py-unite-db-0.3.0/py_unite_db/utils.py
+-rw-r--r--   0        0        0     2002 2023-08-07 10:25:37.703931 py-unite-db-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-07 10:24:23.891673 py-unite-db-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0     1134 2023-08-07 10:24:23.891673 py-unite-db-0.3.0/tests/mock_unite_db.py
+-rw-r--r--   0        0        0      218 2023-08-07 10:24:23.891673 py-unite-db-0.3.0/tests/responses/battle_items.json
+-rw-r--r--   0        0        0      695 2023-08-07 10:24:23.891673 py-unite-db-0.3.0/tests/responses/held_items.json
+-rw-r--r--   0        0        0      972 2023-08-07 10:24:23.891673 py-unite-db-0.3.0/tests/responses/held_items_2.json
+-rw-r--r--   0        0        0    40039 2023-08-07 10:24:23.891673 py-unite-db-0.3.0/tests/responses/pokemon.json
+-rw-r--r--   0        0        0    40637 2023-08-07 10:24:23.891673 py-unite-db-0.3.0/tests/responses/pokemon_2.json
+-rw-r--r--   0        0        0     4591 2023-08-07 10:24:23.891673 py-unite-db-0.3.0/tests/responses/stats.json
+-rw-r--r--   0        0        0     4579 2023-08-07 10:24:23.891673 py-unite-db-0.3.0/tests/responses/stats_2.json
+-rw-r--r--   0        0        0      557 2023-08-07 10:24:23.891673 py-unite-db-0.3.0/tests/test_api_change.py
+-rw-r--r--   0        0        0      411 2023-08-07 10:24:23.891673 py-unite-db-0.3.0/tests/test_battle_items.py
+-rw-r--r--   0        0        0     1708 2023-08-07 10:24:23.891673 py-unite-db-0.3.0/tests/test_cache.py
+-rw-r--r--   0        0        0      609 2023-08-07 10:24:23.891673 py-unite-db-0.3.0/tests/test_held_items.py
+-rw-r--r--   0        0        0     1161 2023-08-07 10:24:23.891673 py-unite-db-0.3.0/tests/test_pokemon.py
+-rw-r--r--   0        0        0     3308 1970-01-01 00:00:00.000000 py-unite-db-0.3.0/PKG-INFO
```

### Comparing `py-unite-db-0.2.1/LICENSE` & `py-unite-db-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py-unite-db-0.2.1/README.md` & `py-unite-db-0.3.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ![GPL-2 Licensed](https://img.shields.io/badge/license-GPL--2-green)
 [![.github/workflows/ci.yml](https://github.com/jaynewey/py-unite-db/actions/workflows/ci.yml/badge.svg)](https://github.com/jaynewey/py-unite-db/actions/workflows/ci.yml)
 [![PyPI](https://img.shields.io/pypi/v/py-unite-db)](https://pypi.org/project/py-unite-db/)
 [![Docs: MkDocs](https://img.shields.io/badge/docs-mkdocs-blue)](https://jaynewey.github.io/py-unite-db)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![pdm-managed](https://img.shields.io/badge/pdm-managed-blueviolet)](https://pdm.fming.dev)
 
-> Unnofficial Python wrapper for the unite-db.com REST API.
+> Unofficial Python wrapper for the unite-db.com REST API.
 
 ## Introduction
 
 [`unite-db`](https://unite-db.com/) is a website dedicated to maintaining a database on various stats in the game Pokemon Unite including stats for Pokemon, Battle Items and Held Items.
 
 This wrapper provides a simple, Pythonic interface to those stats via a REST API, with automatic result caching.
 
@@ -102,8 +102,8 @@
 ### Docs
 
 This project uses [`mkdocs`](https://mkdocs.org), [`mkdocstrings`](https://github.com/mkdocstrings/mkdocstrings/), [`mkdocs-material`](https://squidfunk.github.io/mkdocs-material/) for its documentation.
 
 ```sh
 $ pdm run fetch_charm
 $ pdm run mkdocs serve
-```
+```
```

### Comparing `py-unite-db-0.2.1/py_unite_db/api_base.py` & `py-unite-db-0.3.0/py_unite_db/api_base.py`

 * *Files identical despite different names*

### Comparing `py-unite-db-0.2.1/py_unite_db/models/base_model.py` & `py-unite-db-0.3.0/py_unite_db/models/base_model.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from typing import Any, Type
+from typing import Any
 
 from pydantic import BaseModel as PydanticBaseModel
 from pydantic import root_validator
 
 
 class BaseModel(PydanticBaseModel):
     """Globally configured Pydantic base model used by api wrapper."""
 
     class Config:
         frozen = True  # Disable mutation of attributes and make hashable
 
     @root_validator(pre=True)
-    def _flatten_tags(cls: Type["BaseModel"], v: dict[str, Any]) -> dict[str, Any]:
+    def _flatten_tags(cls, v: dict[str, Any]) -> dict[str, Any]:
         return cls._transform(v)
 
     @staticmethod
     def _transform(v: dict[str, Any]) -> dict[str, Any]:
         """Override if need to transform the json response before unpacking
 
         By default doesn't transform anything.
```

### Comparing `py-unite-db-0.2.1/py_unite_db/models/battle_item.py` & `py-unite-db-0.3.0/py_unite_db/models/battle_item.py`

 * *Files identical despite different names*

### Comparing `py-unite-db-0.2.1/py_unite_db/models/held_item.py` & `py-unite-db-0.3.0/py_unite_db/models/held_item.py`

 * *Files identical despite different names*

### Comparing `py-unite-db-0.2.1/py_unite_db/models/item.py` & `py-unite-db-0.3.0/py_unite_db/models/item.py`

 * *Files identical despite different names*

### Comparing `py-unite-db-0.2.1/py_unite_db/models/pokemon.py` & `py-unite-db-0.3.0/py_unite_db/models/pokemon.py`

 * *Files identical despite different names*

### Comparing `py-unite-db-0.2.1/py_unite_db/models/stats.py` & `py-unite-db-0.3.0/py_unite_db/models/stats.py`

 * *Files identical despite different names*

### Comparing `py-unite-db-0.2.1/py_unite_db/unite_db.py` & `py-unite-db-0.3.0/py_unite_db/unite_db.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,22 +26,22 @@
     It will be very rare you need to this; the API is not updated that frequently.
     """
 
     def __init__(self, base_url: str, client=None):
         super().__init__(base_url, client)
 
     @endpoint
-    def held_items(self) -> list[HeldItem]:
+    def held_items(self) -> list[HeldItem]:  # type: ignore[empty-body]
         """Get all held items.
 
         Returns list of [`HeldItem`][py_unite_db.models.HeldItem].
         """
 
     @endpoint
-    def battle_items(self) -> list[BattleItem]:
+    def battle_items(self) -> list[BattleItem]:  # type: ignore[empty-body]
         """Get all battle items.
 
         Returns list of [`BattleItem`][py_unite_db.models.BattleItem].
         """
 
     @cached_property
     def pokemon(self) -> list[Pokemon]:
@@ -61,19 +61,19 @@
         # rename default "stats" to "stars"
         for p in pokemon:
             p["stars"] = p.pop("stats", None)
         # join pokemon and stats together, and parse as `Pokemon` model
         return [Pokemon.parse_obj(p | {"stats": stats.get(p["name"])}) for p in pokemon]
 
     @endpoint
-    def _pokemon(self):
+    def _pokemon(self):  # type: ignore[empty-body]
         """Private pokemon getter.
 
         Used in background by [py_unite_db.unite_db.UniteDbBase.pokemon]][]
         """
 
     @endpoint
-    def _stats(self):
+    def _stats(self):  # type: ignore[empty-body]
         """Private stat getter.
 
         Used in background by [py_unite_db.unite_db.UniteDbBase.pokemon]][]
         """
```

### Comparing `py-unite-db-0.2.1/py_unite_db/utils.py` & `py-unite-db-0.3.0/py_unite_db/utils.py`

 * *Files identical despite different names*

### Comparing `py-unite-db-0.2.1/pyproject.toml` & `py-unite-db-0.3.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,49 +1,50 @@
 [project]
 name = "py_unite_db"
-version = "0.2.1"
+version = "0.3.0"
 description = "Unnofficial Python wrapper of the unite-db.com REST API."
-dependencies = [ "uplink~=0.9", "pydantic~=1.8",]
+authors = [
+    { name = "Jay Newey", email = "jay.newey@protonmail.com" },
+]
+dependencies = [
+    "uplink~=0.9",
+    "pydantic~=1.8",
+]
 requires-python = ">=3.9"
 readme = "README.md"
-[[project.authors]]
-name = "Jay Newey"
-email = "jay.newey@protonmail.com"
-
-[build-system]
-requires = [ "pdm-pep517",]
-build-backend = "pdm.pep517.api"
 
 [project.license]
 text = "GPL-2.0-only"
 
 [project.urls]
 homepage = "https://github.com/jaynewey/py-unite-db"
 
-[project.optional-dependencies]
-
-[tool.black]
-exclude = "/(\n    \\.git\n  | \\.mypy_cache\n  | \\.tox\n  | venv\n  | \\.venv\n  | _build\n  | buck-out\n  | build\n  | dist\n  | __pypackages__\n)/\n"
-
-[tool.isort]
-profile = "black"
-
-[tool.semantic_release]
-branch = "main"
-version_variable = [ "py_unite_db/__init__.py:__version__",]
-version_toml = "pyproject.toml:project.version"
-build_command = "pdm build"
-major_on_zero = false
+[build-system]
+requires = [
+    "pdm-pep517",
+]
+build-backend = "pdm.pep517.api"
 
 [tool.pdm.dev-dependencies]
-dev = [ "python-semantic-release~=7.19", "black<22,>=21.11b1", "isort~=5.10", "mypy~=0.910", "flake8~=4.0", "pytest", "requests-mock", "types-requests", "mkdocs", "mkdocs-material", "mkdocstrings",]
-
-[tool.pytest.ini_options]
-testpaths = [ "tests",]
-filterwarnings = "ignore::DeprecationWarning:uplink.clients.*:"
+dev = [
+    "python-semantic-release~=7.19",
+    "black<22,>=21.11b1",
+    "isort~=5.10",
+    "mypy~=0.910",
+    "flake8~=4.0",
+    "pytest",
+    "requests-mock",
+    "types-requests",
+    "mkdocs",
+    "mkdocs-material",
+    "mkdocstrings",
+    "mkdocstrings[python]>=0.18",
+    "setuptools>=68.0.0",
+    "click==8.0.3",
+]
 
 [tool.pdm.scripts.format]
 shell = "pdm run isort py_unite_db tests && pdm run black py_unite_db tests"
 
 [tool.pdm.scripts.formatcheck]
 shell = "pdm run black py_unite_db tests --check"
 
@@ -54,7 +55,29 @@
 shell = "pdm run stubs && pdm run mypy --config-file .stubs/mypy.ini py_unite_db/ tests"
 
 [tool.pdm.scripts.lint]
 shell = "pdm run flake8 py_unite_db tests"
 
 [tool.pdm.scripts.fetch_charm]
 shell = "pdm run python scripts/fetch_charm.py docs/assets/overrides/.icons/"
+
+[tool.black]
+exclude = "/(\n    \\.git\n  | \\.mypy_cache\n  | \\.tox\n  | venv\n  | \\.venv\n  | _build\n  | buck-out\n  | build\n  | dist\n  | __pypackages__\n)/\n"
+
+[tool.isort]
+profile = "black"
+
+[tool.pytest.ini_options]
+testpaths = [
+    "tests",
+]
+filterwarnings = "ignore::DeprecationWarning:uplink.clients.*:"
+markers = "webtest: these tests query the actual live API over the web."
+
+[tool.semantic_release]
+branch = "main"
+version_variable = [
+    "py_unite_db/__init__.py:__version__",
+]
+version_toml = "pyproject.toml:project.version"
+build_command = "pdm build"
+major_on_zero = false
```

### Comparing `py-unite-db-0.2.1/tests/mock_unite_db.py` & `py-unite-db-0.3.0/tests/mock_unite_db.py`

 * *Files identical despite different names*

### Comparing `py-unite-db-0.2.1/tests/responses/held_items.json` & `py-unite-db-0.3.0/tests/responses/held_items.json`

 * *Files identical despite different names*

### Comparing `py-unite-db-0.2.1/tests/responses/held_items_2.json` & `py-unite-db-0.3.0/tests/responses/held_items_2.json`

 * *Files identical despite different names*

### Comparing `py-unite-db-0.2.1/tests/responses/pokemon.json` & `py-unite-db-0.3.0/tests/responses/pokemon.json`

 * *Files identical despite different names*

### Comparing `py-unite-db-0.2.1/tests/responses/pokemon_2.json` & `py-unite-db-0.3.0/tests/responses/pokemon_2.json`

 * *Files identical despite different names*

### Comparing `py-unite-db-0.2.1/tests/responses/stats.json` & `py-unite-db-0.3.0/tests/responses/stats.json`

 * *Files identical despite different names*

### Comparing `py-unite-db-0.2.1/tests/responses/stats_2.json` & `py-unite-db-0.3.0/tests/responses/stats_2.json`

 * *Files identical despite different names*

### Comparing `py-unite-db-0.2.1/tests/test_cache.py` & `py-unite-db-0.3.0/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `py-unite-db-0.2.1/tests/test_held_items.py` & `py-unite-db-0.3.0/tests/test_held_items.py`

 * *Files identical despite different names*

### Comparing `py-unite-db-0.2.1/tests/test_pokemon.py` & `py-unite-db-0.3.0/tests/test_pokemon.py`

 * *Files identical despite different names*

### Comparing `py-unite-db-0.2.1/PKG-INFO` & `py-unite-db-0.3.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,118 +1,120 @@
 Metadata-Version: 2.1
 Name: py_unite_db
-Version: 0.2.1
+Version: 0.3.0
 Summary: Unnofficial Python wrapper of the unite-db.com REST API.
-License: UNKNOWN
+License: GPL-2.0-only
 Author-email: Jay Newey <jay.newey@protonmail.com>
 Requires-Python: >=3.9
 Project-URL: homepage, https://github.com/jaynewey/py-unite-db
 Description-Content-Type: text/markdown
-Description: # py-unite-db 
-        
-        ![GPL-2 Licensed](https://img.shields.io/badge/license-GPL--2-green)
-        [![.github/workflows/ci.yml](https://github.com/jaynewey/py-unite-db/actions/workflows/ci.yml/badge.svg)](https://github.com/jaynewey/py-unite-db/actions/workflows/ci.yml)
-        [![PyPI](https://img.shields.io/pypi/v/py-unite-db)](https://pypi.org/project/py-unite-db/)
-        [![Docs: MkDocs](https://img.shields.io/badge/docs-mkdocs-blue)](https://jaynewey.github.io/py-unite-db)
-        [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-        [![pdm-managed](https://img.shields.io/badge/pdm-managed-blueviolet)](https://pdm.fming.dev)
-        
-        > Unnofficial Python wrapper for the unite-db.com REST API.
-        
-        ## Introduction
-        
-        [`unite-db`](https://unite-db.com/) is a website dedicated to maintaining a database on various stats in the game Pokemon Unite including stats for Pokemon, Battle Items and Held Items.
-        
-        This wrapper provides a simple, Pythonic interface to those stats via a REST API, with automatic result caching.
-        
-        Please be warned that this is an unofficial wrapper and the REST API is a private one, so please do not abuse it.
-        
-        If you are publishing any of the data collected with this API, please give credit to [`unite-db`](https://unite-db.com/). They spend many hours collecting this data.
-        
-        ### Installation
-        
-        The package is installable via `pip`.
-        
-        ```sh
-        pip install py-unite-db
-        ```
-        
-        ### Usage
-        
-        Import the `UniteDb` object:
-        
-        ```python
-        from py_unite_db import UniteDb
-        
-        unite_db = UniteDb()
-        ```
-        
-        Let's get the names of all supporter Pokemon:
-        
-        ```python
-        >>> [pokemon.name for pokemon in unite_db.pokemon if pokemon.role == "Supporter"]
-        ['Blissey', 'Eldegoss', 'Mr.Mime', 'Wigglytuff']
-        ```
-        
-        ## Contributing
-        
-        This project uses [`pdm`](https://pdm.fming.dev).
-        
-        ```sh
-        $ pdm install
-        ```
-        
-        ### Running the tests
-        
-        The project uses [`pytest`](https://docs.pytest.org/).
-        
-        ```sh
-        $ pdm run pytest
-        ```
-        
-        ### Type Checking
-        
-        The project must pass [`mypy`](http://www.mypy-lang.org/) type checking.
-        
-        ```sh
-        $ pdm run typecheck
-        ```
-        
-        If you are using `mypy` with an IDE like VS Code make sure you have run
-        
-        ```sh
-        $ pdm run stubs
-        ```
-        
-        To work around `mypy` not supporting PEP582 yet. See https://github.com/python/mypy/issues/10633 for more info on this.
-        
-        ### Formatting
-        
-        Imports are sorted with [`isort`](https://pycqa.github.io/isort/) and source files are formatted with [`black`](https://github.com/psf/black).
-        
-        ```sh
-        $ pdm run format
-        $ pdm run formatcheck
-        ```
-        
-        If you are using VS Code this will be automatically done on save.
-        
-        ### Linting
-        
-        Linting is provided by [`flake8`](github.com/pycqa/flake8).
-        
-        ```sh
-        $ pdm run lint
-        ```
-        
-        ### Conventional Commits
-        
-        The project follows the conventional commit style.
-        
-        ### Docs
-        
-        This project uses [`mkdocs`](https://mkdocs.org), [`mkdocstrings`](https://github.com/mkdocstrings/mkdocstrings/), [`mkdocs-material`](https://squidfunk.github.io/mkdocs-material/) for its documentation.
-        
-        ```sh
-        $ pdm run fetch_charm
-        $ pdm run mkdocs serve
-        ```
+
+# py-unite-db 
+
+![GPL-2 Licensed](https://img.shields.io/badge/license-GPL--2-green)
+[![.github/workflows/ci.yml](https://github.com/jaynewey/py-unite-db/actions/workflows/ci.yml/badge.svg)](https://github.com/jaynewey/py-unite-db/actions/workflows/ci.yml)
+[![PyPI](https://img.shields.io/pypi/v/py-unite-db)](https://pypi.org/project/py-unite-db/)
+[![Docs: MkDocs](https://img.shields.io/badge/docs-mkdocs-blue)](https://jaynewey.github.io/py-unite-db)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![pdm-managed](https://img.shields.io/badge/pdm-managed-blueviolet)](https://pdm.fming.dev)
+
+> Unofficial Python wrapper for the unite-db.com REST API.
+
+## Introduction
+
+[`unite-db`](https://unite-db.com/) is a website dedicated to maintaining a database on various stats in the game Pokemon Unite including stats for Pokemon, Battle Items and Held Items.
+
+This wrapper provides a simple, Pythonic interface to those stats via a REST API, with automatic result caching.
+
+Please be warned that this is an unofficial wrapper and the REST API is a private one, so please do not abuse it.
+
+If you are publishing any of the data collected with this API, please give credit to [`unite-db`](https://unite-db.com/). They spend many hours collecting this data.
+
+### Installation
+
+The package is installable via `pip`.
+
+```sh
+pip install py-unite-db
+```
+
+### Usage
+
+Import the `UniteDb` object:
+
+```python
+from py_unite_db import UniteDb
+
+unite_db = UniteDb()
+```
+
+Let's get the names of all supporter Pokemon:
+
+```python
+>>> [pokemon.name for pokemon in unite_db.pokemon if pokemon.role == "Supporter"]
+['Blissey', 'Eldegoss', 'Mr.Mime', 'Wigglytuff']
+```
+
+## Contributing
+
+This project uses [`pdm`](https://pdm.fming.dev).
+
+```sh
+$ pdm install
+```
+
+### Running the tests
+
+The project uses [`pytest`](https://docs.pytest.org/).
+
+```sh
+$ pdm run pytest
+```
+
+### Type Checking
+
+The project must pass [`mypy`](http://www.mypy-lang.org/) type checking.
+
+```sh
+$ pdm run typecheck
+```
+
+If you are using `mypy` with an IDE like VS Code make sure you have run
+
+```sh
+$ pdm run stubs
+```
+
+To work around `mypy` not supporting PEP582 yet. See https://github.com/python/mypy/issues/10633 for more info on this.
+
+### Formatting
+
+Imports are sorted with [`isort`](https://pycqa.github.io/isort/) and source files are formatted with [`black`](https://github.com/psf/black).
+
+```sh
+$ pdm run format
+$ pdm run formatcheck
+```
+
+If you are using VS Code this will be automatically done on save.
+
+### Linting
+
+Linting is provided by [`flake8`](github.com/pycqa/flake8).
+
+```sh
+$ pdm run lint
+```
+
+### Conventional Commits
+
+The project follows the conventional commit style.
+
+### Docs
+
+This project uses [`mkdocs`](https://mkdocs.org), [`mkdocstrings`](https://github.com/mkdocstrings/mkdocstrings/), [`mkdocs-material`](https://squidfunk.github.io/mkdocs-material/) for its documentation.
+
+```sh
+$ pdm run fetch_charm
+$ pdm run mkdocs serve
+```
+
```

