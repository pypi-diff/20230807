# Comparing `tmp/nonebot_plugin_lostark_wandering_trader-0.0.6.tar.gz` & `tmp/nonebot_plugin_lostark_wandering_trader-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_lostark_wandering_trader-0.0.6.tar", last modified: Sat Aug  5 16:30:25 2023, max compression
+gzip compressed data, was "dist/nonebot_plugin_lostark_wandering_trader-0.0.7.tar", last modified: Mon Aug  7 01:04:04 2023, max compression
```

## Comparing `nonebot_plugin_lostark_wandering_trader-0.0.6.tar` & `nonebot_plugin_lostark_wandering_trader-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 gongmin    (501) staff       (20)        0 2023-08-05 16:30:25.276607 nonebot_plugin_lostark_wandering_trader-0.0.6/
--rw-r--r--   0 gongmin    (501) staff       (20)     1064 2023-08-05 07:52:38.000000 nonebot_plugin_lostark_wandering_trader-0.0.6/LICENSE
--rw-r--r--   0 gongmin    (501) staff       (20)     5974 2023-08-05 16:30:25.276453 nonebot_plugin_lostark_wandering_trader-0.0.6/PKG-INFO
--rw-r--r--   0 gongmin    (501) staff       (20)     4034 2023-08-05 12:37:24.000000 nonebot_plugin_lostark_wandering_trader-0.0.6/README.md
-drwxr-xr-x   0 gongmin    (501) staff       (20)        0 2023-08-05 16:30:25.275304 nonebot_plugin_lostark_wandering_trader-0.0.6/nonebot_plugin_lostark_wandering_trader/
--rw-r--r--   0 gongmin    (501) staff       (20)    10132 2023-08-05 12:37:24.000000 nonebot_plugin_lostark_wandering_trader-0.0.6/nonebot_plugin_lostark_wandering_trader/__init__.py
--rw-r--r--   0 gongmin    (501) staff       (20)      273 2023-08-05 12:37:24.000000 nonebot_plugin_lostark_wandering_trader-0.0.6/nonebot_plugin_lostark_wandering_trader/config.py
-drwxr-xr-x   0 gongmin    (501) staff       (20)        0 2023-08-05 16:30:25.276184 nonebot_plugin_lostark_wandering_trader-0.0.6/nonebot_plugin_lostark_wandering_trader.egg-info/
--rw-r--r--   0 gongmin    (501) staff       (20)     5974 2023-08-05 16:30:25.000000 nonebot_plugin_lostark_wandering_trader-0.0.6/nonebot_plugin_lostark_wandering_trader.egg-info/PKG-INFO
--rw-r--r--   0 gongmin    (501) staff       (20)      457 2023-08-05 16:30:25.000000 nonebot_plugin_lostark_wandering_trader-0.0.6/nonebot_plugin_lostark_wandering_trader.egg-info/SOURCES.txt
--rw-r--r--   0 gongmin    (501) staff       (20)        1 2023-08-05 16:30:25.000000 nonebot_plugin_lostark_wandering_trader-0.0.6/nonebot_plugin_lostark_wandering_trader.egg-info/dependency_links.txt
--rw-r--r--   0 gongmin    (501) staff       (20)      110 2023-08-05 16:30:25.000000 nonebot_plugin_lostark_wandering_trader-0.0.6/nonebot_plugin_lostark_wandering_trader.egg-info/requires.txt
--rw-r--r--   0 gongmin    (501) staff       (20)       40 2023-08-05 16:30:25.000000 nonebot_plugin_lostark_wandering_trader-0.0.6/nonebot_plugin_lostark_wandering_trader.egg-info/top_level.txt
--rw-r--r--   0 gongmin    (501) staff       (20)      630 2023-08-05 16:20:19.000000 nonebot_plugin_lostark_wandering_trader-0.0.6/pyproject.toml
--rw-r--r--   0 gongmin    (501) staff       (20)       38 2023-08-05 16:30:25.276663 nonebot_plugin_lostark_wandering_trader-0.0.6/setup.cfg
--rw-r--r--   0 gongmin    (501) staff       (20)     1304 2023-08-05 16:20:37.000000 nonebot_plugin_lostark_wandering_trader-0.0.6/setup.py
+drwxr-xr-x   0 gongmin    (501) staff       (20)        0 2023-08-07 01:04:04.380325 nonebot_plugin_lostark_wandering_trader-0.0.7/
+-rw-r--r--   0 gongmin    (501) staff       (20)     1064 2023-08-02 03:29:04.000000 nonebot_plugin_lostark_wandering_trader-0.0.7/LICENSE
+-rw-r--r--   0 gongmin    (501) staff       (20)     5974 2023-08-07 01:04:04.379674 nonebot_plugin_lostark_wandering_trader-0.0.7/PKG-INFO
+-rw-r--r--   0 gongmin    (501) staff       (20)     4034 2023-08-07 00:58:36.000000 nonebot_plugin_lostark_wandering_trader-0.0.7/README.md
+drwxr-xr-x   0 gongmin    (501) staff       (20)        0 2023-08-07 01:04:04.365177 nonebot_plugin_lostark_wandering_trader-0.0.7/nonebot_plugin_lostark_wandering_trader/
+-rw-r--r--   0 gongmin    (501) staff       (20)    10534 2023-08-07 00:59:06.000000 nonebot_plugin_lostark_wandering_trader-0.0.7/nonebot_plugin_lostark_wandering_trader/__init__.py
+-rw-r--r--   0 gongmin    (501) staff       (20)      273 2023-08-07 00:58:36.000000 nonebot_plugin_lostark_wandering_trader-0.0.7/nonebot_plugin_lostark_wandering_trader/config.py
+drwxr-xr-x   0 gongmin    (501) staff       (20)        0 2023-08-07 01:04:04.376915 nonebot_plugin_lostark_wandering_trader-0.0.7/nonebot_plugin_lostark_wandering_trader.egg-info/
+-rw-r--r--   0 gongmin    (501) staff       (20)     5974 2023-08-07 01:04:04.000000 nonebot_plugin_lostark_wandering_trader-0.0.7/nonebot_plugin_lostark_wandering_trader.egg-info/PKG-INFO
+-rw-r--r--   0 gongmin    (501) staff       (20)      457 2023-08-07 01:04:04.000000 nonebot_plugin_lostark_wandering_trader-0.0.7/nonebot_plugin_lostark_wandering_trader.egg-info/SOURCES.txt
+-rw-r--r--   0 gongmin    (501) staff       (20)        1 2023-08-07 01:04:04.000000 nonebot_plugin_lostark_wandering_trader-0.0.7/nonebot_plugin_lostark_wandering_trader.egg-info/dependency_links.txt
+-rw-r--r--   0 gongmin    (501) staff       (20)      110 2023-08-07 01:04:04.000000 nonebot_plugin_lostark_wandering_trader-0.0.7/nonebot_plugin_lostark_wandering_trader.egg-info/requires.txt
+-rw-r--r--   0 gongmin    (501) staff       (20)       40 2023-08-07 01:04:04.000000 nonebot_plugin_lostark_wandering_trader-0.0.7/nonebot_plugin_lostark_wandering_trader.egg-info/top_level.txt
+-rw-r--r--   0 gongmin    (501) staff       (20)      630 2023-08-07 01:03:56.000000 nonebot_plugin_lostark_wandering_trader-0.0.7/pyproject.toml
+-rw-r--r--   0 gongmin    (501) staff       (20)       38 2023-08-07 01:04:04.380557 nonebot_plugin_lostark_wandering_trader-0.0.7/setup.cfg
+-rw-r--r--   0 gongmin    (501) staff       (20)     1304 2023-08-07 01:04:00.000000 nonebot_plugin_lostark_wandering_trader-0.0.7/setup.py
```

### Comparing `nonebot_plugin_lostark_wandering_trader-0.0.6/LICENSE` & `nonebot_plugin_lostark_wandering_trader-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_lostark_wandering_trader-0.0.6/PKG-INFO` & `nonebot_plugin_lostark_wandering_trader-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_lostark_wandering_trader
-Version: 0.0.6
+Version: 0.0.7
 Summary: NoneBot lostark cn wandering trader plugin
 Home-page: https://github.com/EmiyaGm/nonebot-plugin-lostark-wandering-trader
 Author: EmiyaGm
 Author-email: EmiyaGm <464723943@qq.com>
 License: MIT License
         
         Copyright (c) 2023 EmiyaGm
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 Metadata-Version: 2.1 Name: nonebot_plugin_lostark_wandering_trader Version:
-0.0.6 Summary: NoneBot lostark cn wandering trader plugin Home-page: https://
+0.0.7 Summary: NoneBot lostark cn wandering trader plugin Home-page: https://
 github.com/EmiyaGm/nonebot-plugin-lostark-wandering-trader Author: EmiyaGm
 Author-email: EmiyaGm <464723943@qq.com> License: MIT License Copyright (c)
 2023 EmiyaGm Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation files (the
 "Software"), to deal in the Software without restriction, including without
 limitation the rights to use, copy, modify, merge, publish, distribute,
 sublicense, and/or sell copies of the Software, and to permit persons to whom
```

### Comparing `nonebot_plugin_lostark_wandering_trader-0.0.6/README.md` & `nonebot_plugin_lostark_wandering_trader-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_lostark_wandering_trader-0.0.6/nonebot_plugin_lostark_wandering_trader/__init__.py` & `nonebot_plugin_lostark_wandering_trader-0.0.7/nonebot_plugin_lostark_wandering_trader/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 except:
     plugin_config = {
         'user_ids': [],
         'group_ids': [],
         'time': 1,
         'server_id': 6,
         'rarity': [],
+        'send_type': []
     }
     
 notice_data = []
 
 @scheduler.scheduled_job("cron", minute=f"*/{plugin_config.get('time')}", id="check_trader")
 async def check_trader():
     global notice_data
@@ -92,48 +93,57 @@
                             cname = card.get('name', '')
                             response = lname + f' 出{cname}了！' + f'稀有度为{rarity}' + f' 提报人: {username}'
                             for qq in plugin_config.get('user_ids'):
                                 await bot.call_api('send_private_msg', **{
                                     'user_id': qq,
                                     'message': response
                                 })
-                            for group in plugin_config.get('group_ids'):
-                                await bot.call_api('send_group_msg', **{
-                                    'group_id': group,
-                                    'message': response
-                                })
+                            try:
+                                for group in plugin_config.get('group_ids'):
+                                    await bot.call_api('send_group_msg', **{
+                                        'group_id': group,
+                                        'message': response
+                                    })
+                            except:
+                                pass
                             time.sleep(1)
                         rapport_confirm = False
                         if rapport.get('rarity') == 'Legendary' and "rapport" in send_type_array:
                             rapport_confirm = True
                         if rapport_confirm:
                             rname = rapport.get('name', '')
                             response = lname + f' 出{rname}了！' + '稀有度为传说' + f' 提报人: {username}'
                             for qq in plugin_config.get('user_ids'):
                                 await bot.call_api('send_private_msg', **{
                                     'user_id': qq,
                                     'message': response
                                 })
-                            for group in plugin_config.get('group_ids'):
-                                await bot.call_api('send_group_msg', **{
-                                    'group_id': group,
-                                    'message': response
-                                })
+                            try:
+                                for group in plugin_config.get('group_ids'):
+                                    await bot.call_api('send_group_msg', **{
+                                        'group_id': group,
+                                        'message': response
+                                    })
+                            except:
+                                pass
                             time.sleep(1)
                         if confirm or rapport_confirm:
                             for qq in plugin_config.get('user_ids'):
                                 await bot.call_api('send_private_msg', **{
                                     'user_id': qq,
                                     'message': MessageSegment.image(f"https://www.emrpg.com/{image}")
                                 })
-                            for group in plugin_config.get('group_ids'):
-                                await bot.call_api('send_group_msg', **{
-                                    'group_id': group,
-                                    'message': MessageSegment.image(f"https://www.emrpg.com/{image}")
-                                })
+                            try:
+                                for group in plugin_config.get('group_ids'):
+                                    await bot.call_api('send_group_msg', **{
+                                        'group_id': group,
+                                        'message': MessageSegment.image(f"https://www.emrpg.com/{image}")
+                                    })
+                            except:
+                                pass
                             time.sleep(1)
                 notice_data[index] = result
         else:
             notice_data[index] = []
             
 
 trader = on_keyword({"下一个商人"}, priority=1)
```

### Comparing `nonebot_plugin_lostark_wandering_trader-0.0.6/nonebot_plugin_lostark_wandering_trader.egg-info/PKG-INFO` & `nonebot_plugin_lostark_wandering_trader-0.0.7/nonebot_plugin_lostark_wandering_trader.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-lostark-wandering-trader
-Version: 0.0.6
+Version: 0.0.7
 Summary: NoneBot lostark cn wandering trader plugin
 Home-page: https://github.com/EmiyaGm/nonebot-plugin-lostark-wandering-trader
 Author: EmiyaGm
 Author-email: EmiyaGm <464723943@qq.com>
 License: MIT License
         
         Copyright (c) 2023 EmiyaGm
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 Metadata-Version: 2.1 Name: nonebot-plugin-lostark-wandering-trader Version:
-0.0.6 Summary: NoneBot lostark cn wandering trader plugin Home-page: https://
+0.0.7 Summary: NoneBot lostark cn wandering trader plugin Home-page: https://
 github.com/EmiyaGm/nonebot-plugin-lostark-wandering-trader Author: EmiyaGm
 Author-email: EmiyaGm <464723943@qq.com> License: MIT License Copyright (c)
 2023 EmiyaGm Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation files (the
 "Software"), to deal in the Software without restriction, including without
 limitation the rights to use, copy, modify, merge, publish, distribute,
 sublicense, and/or sell copies of the Software, and to permit persons to whom
```

### Comparing `nonebot_plugin_lostark_wandering_trader-0.0.6/pyproject.toml` & `nonebot_plugin_lostark_wandering_trader-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot_plugin_lostark_wandering_trader"
-version = "0.0.6"
+version = "0.0.7"
 description = "NoneBot lostark cn wandering trader plugin"
 authors = [
     {name = "EmiyaGm", email = "464723943@qq.com"},
 ]
 dependencies = [
     "httpx<1.0.0,>=0.18.0",
     "nonebot_plugin_apscheduler>=0.3.0",
```

### Comparing `nonebot_plugin_lostark_wandering_trader-0.0.6/setup.py` & `nonebot_plugin_lostark_wandering_trader-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     with io.open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
         long_description = '\n' + f.read()
 except FileNotFoundError:
     long_description = "NoneBot lostark cn wandering trader plugin"
 
 setuptools.setup(
     name="nonebot_plugin_lostark_wandering_trader",
-    version="0.0.6",
+    version="0.0.7",
     license='MIT',
     author="EmiyaGm",
     author_email="464723943@qq.com",
     description="NoneBot lostark cn wandering trader plugin",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/EmiyaGm/nonebot-plugin-lostark-wandering-trader",
```

