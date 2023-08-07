# Comparing `tmp/muffin-0.99.1.tar.gz` & `tmp/muffin-0.99.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "muffin-0.99.1.tar", max compression
+gzip compressed data, was "muffin-0.99.2.tar", max compression
```

## Comparing `muffin-0.99.1.tar` & `muffin-0.99.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     9874 2023-07-06 09:15:53.036352 muffin-0.99.1/README.rst
--rw-r--r--   0        0        0      982 2023-07-06 09:15:53.040352 muffin-0.99.1/muffin/__init__.py
--rw-r--r--   0        0        0     5213 2023-07-06 09:15:53.040352 muffin-0.99.1/muffin/app.py
--rw-r--r--   0        0        0       71 2023-07-06 09:15:53.040352 muffin-0.99.1/muffin/constants.py
--rw-r--r--   0        0        0      701 2023-07-06 09:15:53.040352 muffin-0.99.1/muffin/errors.py
--rw-r--r--   0        0        0     3755 2023-07-06 09:15:53.040352 muffin-0.99.1/muffin/handler.py
--rw-r--r--   0        0        0     8820 2023-07-06 09:15:53.040352 muffin-0.99.1/muffin/manage.py
--rw-r--r--   0        0        0     2877 2023-07-06 09:15:53.040352 muffin-0.99.1/muffin/plugins.py
--rw-r--r--   0        0        0        0 2023-07-06 09:15:53.040352 muffin-0.99.1/muffin/py.typed
--rw-r--r--   0        0        0     2705 2023-07-06 09:15:53.040352 muffin-0.99.1/muffin/pytest.py
--rw-r--r--   0        0        0      153 2023-07-06 09:15:53.040352 muffin-0.99.1/muffin/types.py
--rw-r--r--   0        0        0     2905 2023-07-06 09:15:53.040352 muffin-0.99.1/muffin/utils.py
--rw-r--r--   0        0        0     2990 2023-07-06 09:15:53.044352 muffin-0.99.1/pyproject.toml
--rw-r--r--   0        0        0    11329 1970-01-01 00:00:00.000000 muffin-0.99.1/PKG-INFO
+-rw-r--r--   0        0        0     9874 2023-08-07 14:02:33.282856 muffin-0.99.2/README.rst
+-rw-r--r--   0        0        0     1016 2023-08-07 14:02:33.282856 muffin-0.99.2/muffin/__init__.py
+-rw-r--r--   0        0        0     5213 2023-08-07 14:02:33.282856 muffin-0.99.2/muffin/app.py
+-rw-r--r--   0        0        0       71 2023-08-07 14:02:33.282856 muffin-0.99.2/muffin/constants.py
+-rw-r--r--   0        0        0      701 2023-08-07 14:02:33.282856 muffin-0.99.2/muffin/errors.py
+-rw-r--r--   0        0        0     3755 2023-08-07 14:02:33.282856 muffin-0.99.2/muffin/handler.py
+-rw-r--r--   0        0        0     8820 2023-08-07 14:02:33.282856 muffin-0.99.2/muffin/manage.py
+-rw-r--r--   0        0        0     2877 2023-08-07 14:02:33.282856 muffin-0.99.2/muffin/plugins.py
+-rw-r--r--   0        0        0        0 2023-08-07 14:02:33.282856 muffin-0.99.2/muffin/py.typed
+-rw-r--r--   0        0        0     2692 2023-08-07 14:02:33.282856 muffin-0.99.2/muffin/pytest.py
+-rw-r--r--   0        0        0      153 2023-08-07 14:02:33.282856 muffin-0.99.2/muffin/types.py
+-rw-r--r--   0        0        0     2905 2023-08-07 14:02:33.286857 muffin-0.99.2/muffin/utils.py
+-rw-r--r--   0        0        0     2992 2023-08-07 14:02:33.286857 muffin-0.99.2/pyproject.toml
+-rw-r--r--   0        0        0    11329 1970-01-01 00:00:00.000000 muffin-0.99.2/PKG-INFO
```

### Comparing `muffin-0.99.1/README.rst` & `muffin-0.99.2/README.rst`

 * *Files identical despite different names*

### Comparing `muffin-0.99.1/muffin/__init__.py` & `muffin-0.99.2/muffin/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     ResponseText,
     ResponseWebSocket,
 )
 from asgi_tools.tests import ASGITestClient as TestClient
 
 from .app import Application
 from .errors import MuffinError
-from .handler import Handler
+from .handler import Handler, route_method
 
 __all__ = (
     "ASGIConnectionClosedError",
     "ASGIError",
     "ASGIInvalidMethodError",
     "ASGINotFoundError",
     "Application",
@@ -40,8 +40,9 @@
     "ResponseJSON",
     "ResponseRedirect",
     "ResponseSSE",
     "ResponseStream",
     "ResponseText",
     "ResponseWebSocket",
     "TestClient",
+    "route_method",
 )
```

### Comparing `muffin-0.99.1/muffin/app.py` & `muffin-0.99.2/muffin/app.py`

 * *Files identical despite different names*

### Comparing `muffin-0.99.1/muffin/errors.py` & `muffin-0.99.2/muffin/errors.py`

 * *Files identical despite different names*

### Comparing `muffin-0.99.1/muffin/handler.py` & `muffin-0.99.2/muffin/handler.py`

 * *Files identical despite different names*

### Comparing `muffin-0.99.1/muffin/manage.py` & `muffin-0.99.2/muffin/manage.py`

 * *Files identical despite different names*

### Comparing `muffin-0.99.1/muffin/plugins.py` & `muffin-0.99.2/muffin/plugins.py`

 * *Files identical despite different names*

### Comparing `muffin-0.99.1/muffin/pytest.py` & `muffin-0.99.2/muffin/pytest.py`

 * *Files 5% similar despite different names*

```diff
@@ -72,23 +72,25 @@
         yield muffin_app
 
 
 @asynccontextmanager
 async def lifecycle(app: Application):
     """Setup plugins and run lifespan events."""
 
-    async with AsyncExitStack() as stack:
-        for plugin in app.plugins.values():
-            conftest = getattr(plugin, "conftest", None)
-            if conftest:
-                app.logger.info("Setup plugin '%s'", plugin.name)
-                await stack.enter_async_context(conftest())
-
-        # Manage lifespan
-        async with manage_lifespan(app):
-            yield app
+    plugin_conf = [
+        plugin.conftest
+        for plugin in app.plugins.values()
+        if hasattr(plugin, "conftest") and plugin.conftest
+    ]
+
+    # Manage lifespan and prepare plugins
+    async with AsyncExitStack() as stack, manage_lifespan(app):
+        for conftest in plugin_conf:
+            await stack.enter_async_context(conftest())
+
+        yield app
 
 
 @pytest.fixture()
 def client(app):
     """Generate a test client for the app."""
     return ASGITestClient(app)
```

### Comparing `muffin-0.99.1/muffin/utils.py` & `muffin-0.99.2/muffin/utils.py`

 * *Files identical despite different names*

### Comparing `muffin-0.99.1/pyproject.toml` & `muffin-0.99.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "muffin"
-version = "0.99.1"
+version = "0.99.2"
 description = "Muffin is a fast, simple and asyncronous web-framework for Python 3 (asyncio, trio, curio)"
 readme = "README.rst"
 license = "MIT"
 authors = ["Kirill Klenov <horneds@gmail.com>"]
 keywords = ["asgi", "web", "web framework", "asyncio", "trio", "curio"]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
@@ -90,24 +90,24 @@
 target-version = ["py38", "py39", "py310", "py311"]
 preview = true
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 isolated_build = true
-envlist = py38,py39,py310,py311,pypy39
+envlist = py38,py39,py310,py311,pypy310
 
 [testenv]
 allowlist_externals = poetry
 commands_pre =
     poetry install --no-root --sync --with dev
 commands =
     poetry run pytest --mypy tests --import-mode importlib
 
-[testenv:pypy39]
+[testenv:pypy310]
 allowlist_externals = poetry
 commands_pre =
     poetry install --no-root --sync --with dev
 commands =
     poetry run pytest tests --import-mode importlib
 """
```

### Comparing `muffin-0.99.1/PKG-INFO` & `muffin-0.99.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muffin
-Version: 0.99.1
+Version: 0.99.2
 Summary: Muffin is a fast, simple and asyncronous web-framework for Python 3 (asyncio, trio, curio)
 Home-page: https://github.com/klen/muffin
 License: MIT
 Keywords: asgi,web,web framework,asyncio,trio,curio
 Author: Kirill Klenov
 Author-email: horneds@gmail.com
 Requires-Python: >=3.8,<4.0
```

