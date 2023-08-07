# Comparing `tmp/nonebot-plugin-mcversion-0.2.5.tar.gz` & `tmp/nonebot-plugin-mcversion-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-mcversion-0.2.5.tar", last modified: Mon Aug  7 07:22:16 2023, max compression
+gzip compressed data, was "nonebot-plugin-mcversion-0.2.6.tar", last modified: Mon Aug  7 07:32:07 2023, max compression
```

## Comparing `nonebot-plugin-mcversion-0.2.5.tar` & `nonebot-plugin-mcversion-0.2.6.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1065 2023-08-07 07:22:06.905953 nonebot-plugin-mcversion-0.2.5/LICENSE
--rw-r--r--   0        0        0     1931 2023-08-07 07:22:06.905953 nonebot-plugin-mcversion-0.2.5/README.md
--rw-r--r--   0        0        0     2832 2023-08-07 07:22:06.905953 nonebot-plugin-mcversion-0.2.5/nonebot_plugin_mcversion/__init__.py
--rw-r--r--   0        0        0      642 2023-08-07 07:22:06.905953 nonebot-plugin-mcversion-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     2314 1970-01-01 00:00:00.000000 nonebot-plugin-mcversion-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-08-07 07:31:49.622539 nonebot-plugin-mcversion-0.2.6/LICENSE
+-rw-r--r--   0        0        0     1931 2023-08-07 07:31:49.622539 nonebot-plugin-mcversion-0.2.6/README.md
+-rw-r--r--   0        0        0     2831 2023-08-07 07:31:49.622539 nonebot-plugin-mcversion-0.2.6/nonebot_plugin_mcversion/__init__.py
+-rw-r--r--   0        0        0      642 2023-08-07 07:31:49.622539 nonebot-plugin-mcversion-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     2314 1970-01-01 00:00:00.000000 nonebot-plugin-mcversion-0.2.6/PKG-INFO
```

### Comparing `nonebot-plugin-mcversion-0.2.5/LICENSE` & `nonebot-plugin-mcversion-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-mcversion-0.2.5/README.md` & `nonebot-plugin-mcversion-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-mcversion-0.2.5/nonebot_plugin_mcversion/__init__.py` & `nonebot-plugin-mcversion-0.2.6/nonebot_plugin_mcversion/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from nonebot.plugin import PluginMetadata
+
 __plugin_meta__ = PluginMetadata(
     name="MC版本更新检测",
     description="一个用于检测MC最新版本的插件",
-    usage="使用mcver来获取最新版本号",
+    usage="使用mcver以获取最新版本号",
+    config=Config,
     type="application",
     homepage="https://github.com/CN171-1/nonebot_plugin_mcversion",
-    # 发布必填。
 )
+
 # 导入必要的库
 import os
 import httpx
 from datetime import datetime
 from nonebot import on_command, get_driver, require, Config
 from nonebot.adapters.onebot.v11 import Bot
 from nonebot.adapters.onebot.v11.message import Message
```

### Comparing `nonebot-plugin-mcversion-0.2.5/pyproject.toml` & `nonebot-plugin-mcversion-0.2.6/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-mcversion"
-version = "0.2.5"
+version = "0.2.6"
 description = "NoneBot2 plugin for CheckMCupdate"
 authors = [
     { name = "CN171-1", email = "3428166361@qq.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0rc2",
     "nonebot-adapter-onebot>=2.1.5",
```

### Comparing `nonebot-plugin-mcversion-0.2.5/PKG-INFO` & `nonebot-plugin-mcversion-0.2.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-mcversion
-Version: 0.2.5
+Version: 0.2.6
 Summary: NoneBot2 plugin for CheckMCupdate
 License: MIT
 Author-email: CN171-1 <3428166361@qq.com>
 Requires-Python: >=3.8
 Project-URL: Homepage, https://github.com/CN171-1/nonebot-plugin-mcversion
 Project-URL: Repository, https://github.com/CN171-1/nonebot-plugin-mcversion
 Description-Content-Type: text/markdown
```

