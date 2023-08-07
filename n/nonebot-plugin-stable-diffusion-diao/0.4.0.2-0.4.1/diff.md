# Comparing `tmp/nonebot_plugin_stable_diffusion_diao-0.4.0.2.tar.gz` & `tmp/nonebot_plugin_stable_diffusion_diao-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_stable_diffusion_diao-0.4.0.2.tar", last modified: Sat Aug  5 16:24:06 2023, max compression
+gzip compressed data, was "nonebot_plugin_stable_diffusion_diao-0.4.1.tar", last modified: Mon Aug  7 04:54:33 2023, max compression
```

## Comparing `nonebot_plugin_stable_diffusion_diao-0.4.0.2.tar` & `nonebot_plugin_stable_diffusion_diao-0.4.1.tar`

### file list

```diff
@@ -1,39 +1,40 @@
--rw-r--r--   0        0        0     1082 2023-05-28 09:58:15.375966 nonebot_plugin_stable_diffusion_diao-0.4.0.2/LICENSE
--rw-r--r--   0        0        0      692 2023-08-05 16:23:56.171061 nonebot_plugin_stable_diffusion_diao-0.4.0.2/nonebot_plugin_stable_diffusion_diao/__init__.py
--rw-r--r--   0        0        0    28643 2023-08-05 16:15:52.274941 nonebot_plugin_stable_diffusion_diao-0.4.0.2/nonebot_plugin_stable_diffusion_diao/aidraw.py
--rw-r--r--   0        0        0     6142 2023-08-03 14:38:58.225454 nonebot_plugin_stable_diffusion_diao-0.4.0.2/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402430 nonebot_plugin_stable_diffusion_diao-0.4.0.2/nonebot_plugin_stable_diffusion_diao/amusement/ramdomgirl.py
--rw-r--r--   0        0        0    65701 2023-08-03 14:39:09.188114 nonebot_plugin_stable_diffusion_diao-0.4.0.2/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py
--rw-r--r--   0        0        0     4259 2023-07-23 09:16:00.588115 nonebot_plugin_stable_diffusion_diao-0.4.0.2/nonebot_plugin_stable_diffusion_diao/amusement/vits.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402952 nonebot_plugin_stable_diffusion_diao-0.4.0.2/nonebot_plugin_stable_diffusion_diao/amusement/wordbank.py
--rw-r--r--   0        0        0      699 2023-05-28 09:58:15.404033 nonebot_plugin_stable_diffusion_diao-0.4.0.2/nonebot_plugin_stable_diffusion_diao/backend/__init__.py
--rw-r--r--   0        0        0    17343 2023-08-05 06:16:23.495307 nonebot_plugin_stable_diffusion_diao-0.4.0.2/nonebot_plugin_stable_diffusion_diao/backend/base.py
--rw-r--r--   0        0        0     1279 2023-05-28 09:58:15.404557 nonebot_plugin_stable_diffusion_diao-0.4.0.2/nonebot_plugin_stable_diffusion_diao/backend/naifu.py
--rw-r--r--   0        0        0     1659 2023-05-28 09:58:15.405158 nonebot_plugin_stable_diffusion_diao-0.4.0.2/nonebot_plugin_stable_diffusion_diao/backend/novelai.py
--rw-r--r--   0        0        0     8687 2023-08-05 04:18:20.845342 nonebot_plugin_stable_diffusion_diao-0.4.0.2/nonebot_plugin_stable_diffusion_diao/backend/sd.py
--rw-r--r--   0        0        0    20931 2023-08-05 06:16:35.081043 nonebot_plugin_stable_diffusion_diao-0.4.0.2/nonebot_plugin_stable_diffusion_diao/config.py
--rw-r--r--   0        0        0    11921 2023-08-05 05:23:20.600432 nonebot_plugin_stable_diffusion_diao-0.4.0.2/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py
--rw-r--r--   0        0        0     3340 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.4.0.2/nonebot_plugin_stable_diffusion_diao/extension/anlas.py
--rw-r--r--   0        0        0     1935 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.4.0.2/nonebot_plugin_stable_diffusion_diao/extension/control_net.py
--rw-r--r--   0        0        0     2724 2023-08-05 06:16:27.628128 nonebot_plugin_stable_diffusion_diao-0.4.0.2/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py
--rw-r--r--   0        0        0     2699 2023-07-24 18:34:46.822788 nonebot_plugin_stable_diffusion_diao-0.4.0.2/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py
--rw-r--r--   0        0        0    11332 2023-07-24 18:23:17.528164 nonebot_plugin_stable_diffusion_diao-0.4.0.2/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py
--rw-r--r--   0        0        0     4139 2023-07-22 04:35:59.105979 nonebot_plugin_stable_diffusion_diao-0.4.0.2/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py
--rw-r--r--   0        0        0    47852 2023-08-05 06:16:29.349873 nonebot_plugin_stable_diffusion_diao-0.4.0.2/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py
--rw-r--r--   0        0        0     6353 2023-08-05 06:16:09.106340 nonebot_plugin_stable_diffusion_diao-0.4.0.2/nonebot_plugin_stable_diffusion_diao/extension/translation.py
--rw-r--r--   0        0        0      400 2023-05-28 09:58:15.409671 nonebot_plugin_stable_diffusion_diao-0.4.0.2/nonebot_plugin_stable_diffusion_diao/fifo.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.4.0.2/nonebot_plugin_stable_diffusion_diao/locales/__init__.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.4.0.2/nonebot_plugin_stable_diffusion_diao/locales/en.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.4.0.2/nonebot_plugin_stable_diffusion_diao/locales/jp.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.4.0.2/nonebot_plugin_stable_diffusion_diao/locales/moe_jp.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.4.0.2/nonebot_plugin_stable_diffusion_diao/locales/moe_zh.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.4.0.2/nonebot_plugin_stable_diffusion_diao/locales/zh.py
--rw-r--r--   0        0        0     1905 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.4.0.2/nonebot_plugin_stable_diffusion_diao/manage.py
--rw-r--r--   0        0        0     4685 2023-08-05 16:23:54.378729 nonebot_plugin_stable_diffusion_diao-0.4.0.2/nonebot_plugin_stable_diffusion_diao/utils/__init__.py
--rw-r--r--   0        0        0     2066 2023-07-30 13:00:25.198724 nonebot_plugin_stable_diffusion_diao-0.4.0.2/nonebot_plugin_stable_diffusion_diao/utils/data.py
--rw-r--r--   0        0        0     6148 2023-07-24 18:32:12.882405 nonebot_plugin_stable_diffusion_diao-0.4.0.2/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py
--rw-r--r--   0        0        0     1005 2023-08-05 16:23:26.586630 nonebot_plugin_stable_diffusion_diao-0.4.0.2/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py
--rw-r--r--   0        0        0      733 2023-07-05 13:24:21.506297 nonebot_plugin_stable_diffusion_diao-0.4.0.2/nonebot_plugin_stable_diffusion_diao/utils/save.py
--rw-r--r--   0        0        0     1985 2023-07-10 14:03:49.047428 nonebot_plugin_stable_diffusion_diao-0.4.0.2/nonebot_plugin_stable_diffusion_diao/version.py
--rw-r--r--   0        0        0      728 2023-08-05 16:24:06.858852 nonebot_plugin_stable_diffusion_diao-0.4.0.2/pyproject.toml
--rw-r--r--   0        0        0      485 1970-01-01 00:00:00.000000 nonebot_plugin_stable_diffusion_diao-0.4.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-05-28 09:58:15.375966 nonebot_plugin_stable_diffusion_diao-0.4.1/LICENSE
+-rw-r--r--   0        0        0      703 2023-08-06 09:18:32.524827 nonebot_plugin_stable_diffusion_diao-0.4.1/nonebot_plugin_stable_diffusion_diao/__init__.py
+-rw-r--r--   0        0        0    28643 2023-08-05 16:15:52.274941 nonebot_plugin_stable_diffusion_diao-0.4.1/nonebot_plugin_stable_diffusion_diao/aidraw.py
+-rw-r--r--   0        0        0     6220 2023-08-07 03:34:07.767680 nonebot_plugin_stable_diffusion_diao-0.4.1/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402430 nonebot_plugin_stable_diffusion_diao-0.4.1/nonebot_plugin_stable_diffusion_diao/amusement/ramdomgirl.py
+-rw-r--r--   0        0        0    65701 2023-08-03 14:39:09.188114 nonebot_plugin_stable_diffusion_diao-0.4.1/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py
+-rw-r--r--   0        0        0     4259 2023-07-23 09:16:00.588115 nonebot_plugin_stable_diffusion_diao-0.4.1/nonebot_plugin_stable_diffusion_diao/amusement/vits.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402952 nonebot_plugin_stable_diffusion_diao-0.4.1/nonebot_plugin_stable_diffusion_diao/amusement/wordbank.py
+-rw-r--r--   0        0        0      699 2023-05-28 09:58:15.404033 nonebot_plugin_stable_diffusion_diao-0.4.1/nonebot_plugin_stable_diffusion_diao/backend/__init__.py
+-rw-r--r--   0        0        0    17343 2023-08-05 06:16:23.495307 nonebot_plugin_stable_diffusion_diao-0.4.1/nonebot_plugin_stable_diffusion_diao/backend/base.py
+-rw-r--r--   0        0        0     1279 2023-05-28 09:58:15.404557 nonebot_plugin_stable_diffusion_diao-0.4.1/nonebot_plugin_stable_diffusion_diao/backend/naifu.py
+-rw-r--r--   0        0        0     1659 2023-05-28 09:58:15.405158 nonebot_plugin_stable_diffusion_diao-0.4.1/nonebot_plugin_stable_diffusion_diao/backend/novelai.py
+-rw-r--r--   0        0        0     8687 2023-08-05 04:18:20.845342 nonebot_plugin_stable_diffusion_diao-0.4.1/nonebot_plugin_stable_diffusion_diao/backend/sd.py
+-rw-r--r--   0        0        0    21114 2023-08-07 03:37:09.688742 nonebot_plugin_stable_diffusion_diao-0.4.1/nonebot_plugin_stable_diffusion_diao/config.py
+-rw-r--r--   0        0        0    11921 2023-08-05 05:23:20.600432 nonebot_plugin_stable_diffusion_diao-0.4.1/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py
+-rw-r--r--   0        0        0     3340 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.4.1/nonebot_plugin_stable_diffusion_diao/extension/anlas.py
+-rw-r--r--   0        0        0     8172 2023-08-07 04:53:33.872074 nonebot_plugin_stable_diffusion_diao-0.4.1/nonebot_plugin_stable_diffusion_diao/extension/civitai.py
+-rw-r--r--   0        0        0     1935 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.4.1/nonebot_plugin_stable_diffusion_diao/extension/control_net.py
+-rw-r--r--   0        0        0     2724 2023-08-05 06:16:27.628128 nonebot_plugin_stable_diffusion_diao-0.4.1/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py
+-rw-r--r--   0        0        0     2699 2023-07-24 18:34:46.822788 nonebot_plugin_stable_diffusion_diao-0.4.1/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py
+-rw-r--r--   0        0        0    11332 2023-07-24 18:23:17.528164 nonebot_plugin_stable_diffusion_diao-0.4.1/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py
+-rw-r--r--   0        0        0     4139 2023-07-22 04:35:59.105979 nonebot_plugin_stable_diffusion_diao-0.4.1/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py
+-rw-r--r--   0        0        0    47944 2023-08-07 03:34:25.072810 nonebot_plugin_stable_diffusion_diao-0.4.1/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py
+-rw-r--r--   0        0        0     6378 2023-08-07 03:33:48.271023 nonebot_plugin_stable_diffusion_diao-0.4.1/nonebot_plugin_stable_diffusion_diao/extension/translation.py
+-rw-r--r--   0        0        0      400 2023-05-28 09:58:15.409671 nonebot_plugin_stable_diffusion_diao-0.4.1/nonebot_plugin_stable_diffusion_diao/fifo.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.4.1/nonebot_plugin_stable_diffusion_diao/locales/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.4.1/nonebot_plugin_stable_diffusion_diao/locales/en.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.4.1/nonebot_plugin_stable_diffusion_diao/locales/jp.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.4.1/nonebot_plugin_stable_diffusion_diao/locales/moe_jp.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.4.1/nonebot_plugin_stable_diffusion_diao/locales/moe_zh.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.4.1/nonebot_plugin_stable_diffusion_diao/locales/zh.py
+-rw-r--r--   0        0        0     1905 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.4.1/nonebot_plugin_stable_diffusion_diao/manage.py
+-rw-r--r--   0        0        0     5222 2023-08-07 03:27:37.914834 nonebot_plugin_stable_diffusion_diao-0.4.1/nonebot_plugin_stable_diffusion_diao/utils/__init__.py
+-rw-r--r--   0        0        0     2065 2023-08-05 16:30:13.201017 nonebot_plugin_stable_diffusion_diao-0.4.1/nonebot_plugin_stable_diffusion_diao/utils/data.py
+-rw-r--r--   0        0        0     6148 2023-07-24 18:32:12.882405 nonebot_plugin_stable_diffusion_diao-0.4.1/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py
+-rw-r--r--   0        0        0     1005 2023-08-05 16:23:26.586630 nonebot_plugin_stable_diffusion_diao-0.4.1/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py
+-rw-r--r--   0        0        0      733 2023-07-05 13:24:21.506297 nonebot_plugin_stable_diffusion_diao-0.4.1/nonebot_plugin_stable_diffusion_diao/utils/save.py
+-rw-r--r--   0        0        0     1985 2023-07-10 14:03:49.047428 nonebot_plugin_stable_diffusion_diao-0.4.1/nonebot_plugin_stable_diffusion_diao/version.py
+-rw-r--r--   0        0        0      726 2023-08-07 04:54:33.983831 nonebot_plugin_stable_diffusion_diao-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      483 1970-01-01 00:00:00.000000 nonebot_plugin_stable_diffusion_diao-0.4.1/PKG-INFO
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.0.2/LICENSE` & `nonebot_plugin_stable_diffusion_diao-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.0.2/nonebot_plugin_stable_diffusion_diao/__init__.py` & `nonebot_plugin_stable_diffusion_diao-0.4.1/nonebot_plugin_stable_diffusion_diao/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from . import config, manage
 from .aidraw import AIDRAW
 from nonebot.plugin import PluginMetadata
 from .extension.deepdanbooru import deepdanbooru
 from .amusement import today_girl, chatgpt_tagger, vits
-from .extension import sd_extra_api_func, aidraw_help
+from .extension import sd_extra_api_func, aidraw_help, civitai
+
 
 __plugin_meta__ = PluginMetadata(
     name="AI绘图",
     description="调用novelai进行二次元AI绘图",
     usage=f"发送 绘画帮助 获取更多帮助\n基础用法:\n.aidraw[指令] [空格] loli,[参数]\n示例:.aidraw loli,cute,kawaii,\n项目地址:https://github.com/Mutsukibot/tree/nonebot-plugin-novelai\n说明书：https://sena-nana.github.io/MutsukiDocs/",
 )
 __all__ = ["AIDRAW", "__plugin_meta__"]
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.0.2/nonebot_plugin_stable_diffusion_diao/aidraw.py` & `nonebot_plugin_stable_diffusion_diao-0.4.1/nonebot_plugin_stable_diffusion_diao/aidraw.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.0.2/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py` & `nonebot_plugin_stable_diffusion_diao-0.4.1/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,17 @@
             "top_p":1,
             "frequency_penalty": 0,
             "presence_penalty": 0.6,
             "stop": [" Human:", " AI:"]
         }
 
         async with aiohttp.ClientSession(headers=header) as session:
-            async with session.post(url=f"https://{config.openai_proxy_site}/v1/chat/completions",json=payload) as resp:
+            async with session.post(url=f"https://{config.openai_proxy_site}/v1/chat/completions", 
+                                    json=payload, proxy=config.proxy_site
+            ) as resp:
                 print(resp.status)
                 all_resp = await resp.json()
                 resp = all_resp["choices"][0]["message"]["content"]
                 return resp
 
 
 user_session = {}
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.0.2/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py` & `nonebot_plugin_stable_diffusion_diao-0.4.1/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.0.2/nonebot_plugin_stable_diffusion_diao/amusement/vits.py` & `nonebot_plugin_stable_diffusion_diao-0.4.1/nonebot_plugin_stable_diffusion_diao/amusement/vits.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.0.2/nonebot_plugin_stable_diffusion_diao/backend/__init__.py` & `nonebot_plugin_stable_diffusion_diao-0.4.1/nonebot_plugin_stable_diffusion_diao/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.0.2/nonebot_plugin_stable_diffusion_diao/backend/base.py` & `nonebot_plugin_stable_diffusion_diao-0.4.1/nonebot_plugin_stable_diffusion_diao/backend/base.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.0.2/nonebot_plugin_stable_diffusion_diao/backend/naifu.py` & `nonebot_plugin_stable_diffusion_diao-0.4.1/nonebot_plugin_stable_diffusion_diao/backend/naifu.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.0.2/nonebot_plugin_stable_diffusion_diao/backend/novelai.py` & `nonebot_plugin_stable_diffusion_diao-0.4.1/nonebot_plugin_stable_diffusion_diao/backend/novelai.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.0.2/nonebot_plugin_stable_diffusion_diao/backend/sd.py` & `nonebot_plugin_stable_diffusion_diao-0.4.1/nonebot_plugin_stable_diffusion_diao/backend/sd.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.0.2/nonebot_plugin_stable_diffusion_diao/config.py` & `nonebot_plugin_stable_diffusion_diao-0.4.1/nonebot_plugin_stable_diffusion_diao/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,14 +195,15 @@
     auto_match = True  # 是否自动匹配
     hr_off_when_cn = True  # 使用controlnet功能的时候关闭高清修复
     backend_name_list = []
     backend_site_list = []
     only_super_user = True  # 只有超级用户才能永久更换模型, 雕雕没有小号来测试了, 悲
     tiled_diffusion = False  # 使用tiled-diffusion来生成图片
     save_img = True  # 是否保存图片(API侧)
+    proxy_site: None or str = None  # 只支持http代理, 设置代理以便访问C站, OPENAI, 翻译等, 经过考虑, 还请填写完整的URL, 例如 "http://192.168.5.1:11082"
     # 允许单群设置的设置
     def keys(cls):
         return ("novelai_cd", "novelai_tags", "novelai_on", "novelai_ntags", "novelai_revoke", "novelai_h", "novelai_htype", "novelai_picaudit", "novelai_pure", "novelai_site")
 
     def __getitem__(cls, item):
         return getattr(cls, item)
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.0.2/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py` & `nonebot_plugin_stable_diffusion_diao-0.4.1/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.0.2/nonebot_plugin_stable_diffusion_diao/extension/anlas.py` & `nonebot_plugin_stable_diffusion_diao-0.4.1/nonebot_plugin_stable_diffusion_diao/extension/anlas.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.0.2/nonebot_plugin_stable_diffusion_diao/extension/control_net.py` & `nonebot_plugin_stable_diffusion_diao-0.4.1/nonebot_plugin_stable_diffusion_diao/extension/control_net.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.0.2/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py` & `nonebot_plugin_stable_diffusion_diao-0.4.1/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.0.2/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py` & `nonebot_plugin_stable_diffusion_diao-0.4.1/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.0.2/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py` & `nonebot_plugin_stable_diffusion_diao-0.4.1/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.0.2/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py` & `nonebot_plugin_stable_diffusion_diao-0.4.1/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.0.2/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py` & `nonebot_plugin_stable_diffusion_diao-0.4.1/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py`

 * *Files 1% similar despite different names*

```diff
@@ -382,20 +382,20 @@
     except KeyError:
         await get_models.finish("输入错误,索引错误")
 
 
 async def aiohttp_func(way, url, payload={}):
     try:
         if way == "post":
-            async with aiohttp.ClientSession() as session:
+            async with aiohttp.ClientSession(timeout=aiohttp.ClientTimeout(total=1800)) as session:
                 async with session.post(url=url, json=payload) as resp:
                     resp_data = await resp.json()
                     return resp_data, resp.status
         else:
-            async with aiohttp.ClientSession() as session:
+            async with aiohttp.ClientSession(timeout=aiohttp.ClientTimeout(total=1800)) as session:
                 async with session.get(url=url) as resp:
                     resp_data = await resp.json()
                     return resp_data, resp.status
     except Exception:
         return None
 
 
@@ -1173,8 +1173,9 @@
         if script_index:
             select_script_args = resp[0][script_index]["args"]
             print(select_script_args)
             await risk_control(bot, event, str(select_script_args), True)
         await risk_control(bot, event, script_name, True)
         
     else:
-        await get_scripts.finish("请按照以下格式获取脚本信息\n例如 获取脚本0 再使用 获取脚本0_2 查看具体脚本所需的参数")
+        await get_scripts.finish("请按照以下格式获取脚本信息\n例如 获取脚本0 再使用 获取脚本0_2 查看具体脚本所需的参数")
+
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.0.2/nonebot_plugin_stable_diffusion_diao/extension/translation.py` & `nonebot_plugin_stable_diffusion_diao-0.4.1/nonebot_plugin_stable_diffusion_diao/extension/translation.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,15 +115,15 @@
     try:
         if to == "zh":
             from_ = "en"
         else:
             from_="zh"
         async with aiohttp.ClientSession()as session:
             data = {"data": [input, from_, to]}
-            async with session.post("https://mikeee-gradio-gtr.hf.space/api/predict", json=data)as resp:
+            async with session.post("https://mikeee-gradio-gtr.hf.space/api/predict", json=data, proxy=config.proxy_site)as resp:
                 if resp.status != 200:
                     logger.error(f"谷歌代理翻译接口调用失败,错误代码{resp.status},{await resp.text()}")
                 result = await resp.json()
                 result=result["data"][0]
                 logger.debug(f"谷歌代理翻译启动，获取到{input},翻译后{result}")
                 return result
     except Exception:
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.0.2/nonebot_plugin_stable_diffusion_diao/manage.py` & `nonebot_plugin_stable_diffusion_diao-0.4.1/nonebot_plugin_stable_diffusion_diao/manage.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.0.2/nonebot_plugin_stable_diffusion_diao/utils/__init__.py` & `nonebot_plugin_stable_diffusion_diao-0.4.1/nonebot_plugin_stable_diffusion_diao/utils/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -62,16 +62,21 @@
     async with aiohttp.ClientSession() as session:
         async with session.post(url=f"http://{backend_site}/sdapi/v1/reload-checkpoint") as resp:
             if resp.status not in [200, 201]:
                 logger.error(f"重载模型失败，错误:{await resp.text()}")
             logger.info("重载模型成功")
             
             
-async def pic_audit_standalone(img_base64, is_return_tags=False, audit=False):
-    
+async def pic_audit_standalone(img_base64, 
+                               is_return_tags=False, 
+                               audit=False, 
+                               return_none=False
+):
+    if isinstance(img_base64, bytes):
+        img_base64 = base64.b64encode(img_base64).decode()
     payload = {"image": img_base64, "model": f"{config.tagger_model}", "threshold": 0.35 }
 
     async with aiohttp.ClientSession() as session:
         async with session.post(url=f"http://{config.novelai_tagger_site}/tagger/v1/interrogate", json=payload) as resp:
             if resp.status not in [200, 201]:
                 resp_text = await resp.text()
                 logger.error(f"API失败，错误信息:{resp.status, resp_text}")
@@ -89,14 +94,20 @@
                     percent = f":{tags[i]*100:.2f}".rjust(6)
                     message += f"[{to_user}{percent}%]\n"
                     to_user_dict[to_user] = tags[i]
                 value = list(to_user_dict.values())
                 value.sort(reverse=True)
                 reverse_dict = {value: key for key, value in to_user_dict.items()}
                 message += (f"最终结果为:{reverse_dict[value[0]].rjust(5)}")
+    if return_none:
+        value = list(possibilities.values())
+        value.sort(reverse=True)
+        reverse_dict = {value: key for key, value in possibilities.items()}
+        logger.info(message)
+        return True if reverse_dict[value[0]] == "questionable" or reverse_dict[value[0]] == "explicit" else False
     if is_return_tags:
         return message, tags
     if audit:
         return possibilities, message
     return message
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.0.2/nonebot_plugin_stable_diffusion_diao/utils/data.py` & `nonebot_plugin_stable_diffusion_diao-0.4.1/nonebot_plugin_stable_diffusion_diao/utils/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from ..config import config
 # 基础优化tag
-basetag = "masterpiece, best quality,"
+basetag = "masterpiece,best quality,"
 
 # 基础排除tag
 lowQuality = "easynegative,badhandv4"
 
 # 屏蔽词
 # htags = "nsfw|nude|naked|nipple|blood|censored|vagina|gag|gokkun|hairjob|tentacle|oral|fellatio|areolae|lactation|paizuri|piercing|sex|footjob|masturbation|hips|penis|testicles|ejaculation|cum|tamakeri|pussy|pubic|clitoris|mons|cameltoe|grinding|crotch|cervix|cunnilingus|insertion|penetration|fisting|fingering|peeing|ass|buttjob|spanked|anus|anal|anilingus|enema|x-ray|wakamezake|humiliation|tally|futa|incest|twincest|pegging|femdom|ganguro|bestiality|gangbang|3P|tribadism|molestation|voyeurism|exhibitionism|rape|spitroast|cock|69|doggystyle|missionary|virgin|shibari|bondage|bdsm|rope|pillory|stocks|bound|hogtie|frogtie|suspension|anal|dildo|vibrator|hitachi|nyotaimori|vore|amputee|transformation|bloody"
 htags = r"\b(nsfw|no\s*clothes|mucus|micturition|urethra|Urinary|Urination|climax|n\s*o\s*c\s*l\s*o\s*t\s*h\s*e\s*s|n[ -]?o[ -]?c[ -]?l[ -]?o[ -]?t[ -]?h[ -]?e[ -]?s|nudity|nude|naked|nipple|blood|censored|vagina|gag|gokkun|hairjob|tentacle|oral|fellatio|areolae|lactation|paizuri|piercing|sex|footjob|masturbation|hips|penis|testicles|ejaculation|cum|tamakeri|pussy|pubic|clitoris|mons|cameltoe|grinding|crotch|cervix|cunnilingus|insertion|penetration|fisting|fingering|peeing|buttjob|spanked|anus|anal|anilingus|enema|x-ray|wakamezake|humiliation|tally|futa|incest|twincest|pegging|porn|Orgasm|womb|femdom|ganguro|bestiality|gangbang|3P|tribadism|molestation|voyeurism|exhibitionism|rape|spitroast|cock|69|doggystyle|missionary|virgin|shibari|bondage|bdsm|rope|pillory|stocks|bound|hogtie|frogtie|suspension|anal|dildo|vibrator|hitachi|nyotaimori|vore|amputee|transformation|bloody|pornhub)\b"
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.0.2/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py` & `nonebot_plugin_stable_diffusion_diao-0.4.1/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.0.2/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py` & `nonebot_plugin_stable_diffusion_diao-0.4.1/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.0.2/nonebot_plugin_stable_diffusion_diao/utils/save.py` & `nonebot_plugin_stable_diffusion_diao-0.4.1/nonebot_plugin_stable_diffusion_diao/utils/save.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.0.2/nonebot_plugin_stable_diffusion_diao/version.py` & `nonebot_plugin_stable_diffusion_diao-0.4.1/nonebot_plugin_stable_diffusion_diao/version.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.4.0.2/pyproject.toml` & `nonebot_plugin_stable_diffusion_diao-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-stable-diffusion-diao"
-version = "0.4.0.2"
+version = "0.4.1"
 description = "主要面对stable-diffusion-webui-api的nonebot2插件"
 authors = [
     { name = "DiaoDaiaChan", email = "diaodaiachan@qq.com" },
 ]
 dependencies = [
     "aiofiles>=23.1.0",
     "aiohttp>=3.8.4",
```

