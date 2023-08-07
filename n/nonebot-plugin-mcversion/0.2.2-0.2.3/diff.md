# Comparing `tmp/nonebot-plugin-mcversion-0.2.2.tar.gz` & `tmp/nonebot-plugin-mcversion-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-mcversion-0.2.2.tar", last modified: Sun Jul 30 06:21:02 2023, max compression
+gzip compressed data, was "nonebot-plugin-mcversion-0.2.3.tar", last modified: Mon Aug  7 07:00:25 2023, max compression
```

## Comparing `nonebot-plugin-mcversion-0.2.2.tar` & `nonebot-plugin-mcversion-0.2.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1065 2023-07-30 06:20:51.911943 nonebot-plugin-mcversion-0.2.2/LICENSE
--rw-r--r--   0        0        0     1931 2023-07-30 06:20:51.911943 nonebot-plugin-mcversion-0.2.2/README.md
--rw-r--r--   0        0        0     2497 2023-07-30 06:20:51.911943 nonebot-plugin-mcversion-0.2.2/nonebot_plugin_mcversion/__init__.py
--rw-r--r--   0        0        0      621 2023-07-30 06:20:51.911943 nonebot-plugin-mcversion-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     2314 1970-01-01 00:00:00.000000 nonebot-plugin-mcversion-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-08-07 07:00:11.359087 nonebot-plugin-mcversion-0.2.3/LICENSE
+-rw-r--r--   0        0        0     1931 2023-08-07 07:00:11.359087 nonebot-plugin-mcversion-0.2.3/README.md
+-rw-r--r--   0        0        0     2497 2023-08-07 07:00:11.359087 nonebot-plugin-mcversion-0.2.3/nonebot_plugin_mcversion/__init__.py
+-rw-r--r--   0        0        0      642 2023-08-07 07:00:11.359087 nonebot-plugin-mcversion-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     2314 1970-01-01 00:00:00.000000 nonebot-plugin-mcversion-0.2.3/PKG-INFO
```

### Comparing `nonebot-plugin-mcversion-0.2.2/LICENSE` & `nonebot-plugin-mcversion-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-mcversion-0.2.2/README.md` & `nonebot-plugin-mcversion-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-mcversion-0.2.2/nonebot_plugin_mcversion/__init__.py` & `nonebot-plugin-mcversion-0.2.3/nonebot_plugin_mcversion/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-mcversion-0.2.2/pyproject.toml` & `nonebot-plugin-mcversion-0.2.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 [project]
 name = "nonebot-plugin-mcversion"
-version = "0.2.2"
+version = "0.2.3"
 description = "NoneBot2 plugin for CheckMCupdate"
 authors = [
     { name = "CN171-1", email = "3428166361@qq.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0rc2",
     "nonebot-adapter-onebot>=2.1.5",
     "nonebot-plugin-apscheduler>=0.2.0",
+    "httpx>=0.24.0",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
```

### Comparing `nonebot-plugin-mcversion-0.2.2/PKG-INFO` & `nonebot-plugin-mcversion-0.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-mcversion
-Version: 0.2.2
+Version: 0.2.3
 Summary: NoneBot2 plugin for CheckMCupdate
 License: MIT
 Author-email: CN171-1 <3428166361@qq.com>
 Requires-Python: >=3.8
 Project-URL: Homepage, https://github.com/CN171-1/nonebot-plugin-mcversion
 Project-URL: Repository, https://github.com/CN171-1/nonebot-plugin-mcversion
 Description-Content-Type: text/markdown
```

