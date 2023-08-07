# Comparing `tmp/nonebot-plugin-mcversion-0.2.3.tar.gz` & `tmp/nonebot-plugin-mcversion-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-mcversion-0.2.3.tar", last modified: Mon Aug  7 07:00:25 2023, max compression
+gzip compressed data, was "nonebot-plugin-mcversion-0.2.4.tar", last modified: Mon Aug  7 07:14:52 2023, max compression
```

## Comparing `nonebot-plugin-mcversion-0.2.3.tar` & `nonebot-plugin-mcversion-0.2.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1065 2023-08-07 07:00:11.359087 nonebot-plugin-mcversion-0.2.3/LICENSE
--rw-r--r--   0        0        0     1931 2023-08-07 07:00:11.359087 nonebot-plugin-mcversion-0.2.3/README.md
--rw-r--r--   0        0        0     2497 2023-08-07 07:00:11.359087 nonebot-plugin-mcversion-0.2.3/nonebot_plugin_mcversion/__init__.py
--rw-r--r--   0        0        0      642 2023-08-07 07:00:11.359087 nonebot-plugin-mcversion-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     2314 1970-01-01 00:00:00.000000 nonebot-plugin-mcversion-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-08-07 07:14:38.955904 nonebot-plugin-mcversion-0.2.4/LICENSE
+-rw-r--r--   0        0        0     1931 2023-08-07 07:14:38.955904 nonebot-plugin-mcversion-0.2.4/README.md
+-rw-r--r--   0        0        0     2831 2023-08-07 07:14:38.955904 nonebot-plugin-mcversion-0.2.4/nonebot_plugin_mcversion/__init__.py
+-rw-r--r--   0        0        0      642 2023-08-07 07:14:38.955904 nonebot-plugin-mcversion-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     2314 1970-01-01 00:00:00.000000 nonebot-plugin-mcversion-0.2.4/PKG-INFO
```

### Comparing `nonebot-plugin-mcversion-0.2.3/LICENSE` & `nonebot-plugin-mcversion-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-mcversion-0.2.3/README.md` & `nonebot-plugin-mcversion-0.2.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 ## 使用
 
 1. 使用 `mcver` , `mcversion` ,`MC版本` 来获取当前最新MC版本
 2. 程序会每分钟自动检查 Minecraft 是否有新版本，若有则会在指定的群组内发送消息。
 
 ## 配置
 
-在配置文件中可以进行以下设置：
+在配置文件中必须进行以下设置：
 
 - `mcver_group_id`：指定检查 Minecraft 更新后发送消息的群组 ID。
 
 ```python
 mcver_group_id = [123456, 789012]
 ```
```

### Comparing `nonebot-plugin-mcversion-0.2.3/nonebot_plugin_mcversion/__init__.py` & `nonebot-plugin-mcversion-0.2.4/nonebot_plugin_mcversion/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 # 导入必要的库
 import os
 import httpx
+from nonebot.plugin import PluginMetadata
+__plugin_meta__ = PluginMetadata(
+    name="MC版本更新检测",
+    description="一个用于检测MC最新版本的插件",
+    usage="使用mcver来获取最新版本号",
+    type="application",
+    homepage="https://github.com/Sydrr0/nonebot_plugin_mcversion",
+    # 发布必填。
+)
 from datetime import datetime
 from nonebot import on_command, get_driver, require, Config
 from nonebot.adapters.onebot.v11 import Bot
 from nonebot.adapters.onebot.v11.message import Message
 
 env_config = Config(**get_driver().config.dict())
 mcver_group_id = list(env_config.mcver_group_id)
```

### Comparing `nonebot-plugin-mcversion-0.2.3/pyproject.toml` & `nonebot-plugin-mcversion-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-mcversion"
-version = "0.2.3"
+version = "0.2.4"
 description = "NoneBot2 plugin for CheckMCupdate"
 authors = [
     { name = "CN171-1", email = "3428166361@qq.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0rc2",
     "nonebot-adapter-onebot>=2.1.5",
```

### Comparing `nonebot-plugin-mcversion-0.2.3/PKG-INFO` & `nonebot-plugin-mcversion-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-mcversion
-Version: 0.2.3
+Version: 0.2.4
 Summary: NoneBot2 plugin for CheckMCupdate
 License: MIT
 Author-email: CN171-1 <3428166361@qq.com>
 Requires-Python: >=3.8
 Project-URL: Homepage, https://github.com/CN171-1/nonebot-plugin-mcversion
 Project-URL: Repository, https://github.com/CN171-1/nonebot-plugin-mcversion
 Description-Content-Type: text/markdown
@@ -69,15 +69,15 @@
 ## 使用
 
 1. 使用 `mcver` , `mcversion` ,`MC版本` 来获取当前最新MC版本
 2. 程序会每分钟自动检查 Minecraft 是否有新版本，若有则会在指定的群组内发送消息。
 
 ## 配置
 
-在配置文件中可以进行以下设置：
+在配置文件中必须进行以下设置：
 
 - `mcver_group_id`：指定检查 Minecraft 更新后发送消息的群组 ID。
 
 ```python
 mcver_group_id = [123456, 789012]
 ```
```

