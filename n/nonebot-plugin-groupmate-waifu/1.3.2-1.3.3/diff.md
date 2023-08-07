# Comparing `tmp/nonebot_plugin_groupmate_waifu-1.3.2.tar.gz` & `tmp/nonebot_plugin_groupmate_waifu-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_groupmate_waifu-1.3.2.tar", last modified: Fri Aug  4 21:23:11 2023, max compression
+gzip compressed data, was "nonebot_plugin_groupmate_waifu-1.3.3.tar", last modified: Mon Aug  7 12:07:13 2023, max compression
```

## Comparing `nonebot_plugin_groupmate_waifu-1.3.2.tar` & `nonebot_plugin_groupmate_waifu-1.3.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 21:23:11.078557 nonebot_plugin_groupmate_waifu-1.3.2/
--rw-rw-rw-   0        0        0     1065 2022-08-13 09:26:37.000000 nonebot_plugin_groupmate_waifu-1.3.2/LICENSE
--rw-rw-rw-   0        0        0      279 2023-08-04 21:23:11.078055 nonebot_plugin_groupmate_waifu-1.3.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-04 21:23:11.067554 nonebot_plugin_groupmate_waifu-1.3.2/nonebot_plugin_groupmate_waifu/
--rw-rw-rw-   0        0        0    21218 2023-08-04 21:21:34.000000 nonebot_plugin_groupmate_waifu-1.3.2/nonebot_plugin_groupmate_waifu/__init__.py
--rw-rw-rw-   0        0        0      354 2023-07-17 15:11:43.000000 nonebot_plugin_groupmate_waifu-1.3.2/nonebot_plugin_groupmate_waifu/config.py
--rw-rw-rw-   0        0        0     2015 2023-07-21 12:53:08.000000 nonebot_plugin_groupmate_waifu-1.3.2/nonebot_plugin_groupmate_waifu/utils.py
-drwxrwxrwx   0        0        0        0 2023-08-04 21:23:11.076554 nonebot_plugin_groupmate_waifu-1.3.2/nonebot_plugin_groupmate_waifu.egg-info/
--rw-rw-rw-   0        0        0      279 2023-08-04 21:23:10.000000 nonebot_plugin_groupmate_waifu-1.3.2/nonebot_plugin_groupmate_waifu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      409 2023-08-04 21:23:10.000000 nonebot_plugin_groupmate_waifu-1.3.2/nonebot_plugin_groupmate_waifu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 21:23:10.000000 nonebot_plugin_groupmate_waifu-1.3.2/nonebot_plugin_groupmate_waifu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2023-08-04 21:23:10.000000 nonebot_plugin_groupmate_waifu-1.3.2/nonebot_plugin_groupmate_waifu.egg-info/requires.txt
--rw-rw-rw-   0        0        0       31 2023-08-04 21:23:10.000000 nonebot_plugin_groupmate_waifu-1.3.2/nonebot_plugin_groupmate_waifu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-04 21:23:11.079055 nonebot_plugin_groupmate_waifu-1.3.2/setup.cfg
--rw-rw-rw-   0        0        0      567 2023-08-04 21:23:07.000000 nonebot_plugin_groupmate_waifu-1.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 12:07:13.454850 nonebot_plugin_groupmate_waifu-1.3.3/
+-rw-rw-rw-   0        0        0     1065 2022-08-13 09:26:37.000000 nonebot_plugin_groupmate_waifu-1.3.3/LICENSE
+-rw-rw-rw-   0        0        0      279 2023-08-07 12:07:13.454350 nonebot_plugin_groupmate_waifu-1.3.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-07 12:07:13.445842 nonebot_plugin_groupmate_waifu-1.3.3/nonebot_plugin_groupmate_waifu/
+-rw-rw-rw-   0        0        0    21212 2023-08-07 12:06:04.000000 nonebot_plugin_groupmate_waifu-1.3.3/nonebot_plugin_groupmate_waifu/__init__.py
+-rw-rw-rw-   0        0        0      354 2023-07-17 15:11:43.000000 nonebot_plugin_groupmate_waifu-1.3.3/nonebot_plugin_groupmate_waifu/config.py
+-rw-rw-rw-   0        0        0     2015 2023-07-21 12:53:08.000000 nonebot_plugin_groupmate_waifu-1.3.3/nonebot_plugin_groupmate_waifu/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-07 12:07:13.452849 nonebot_plugin_groupmate_waifu-1.3.3/nonebot_plugin_groupmate_waifu.egg-info/
+-rw-rw-rw-   0        0        0      279 2023-08-07 12:07:13.000000 nonebot_plugin_groupmate_waifu-1.3.3/nonebot_plugin_groupmate_waifu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      409 2023-08-07 12:07:13.000000 nonebot_plugin_groupmate_waifu-1.3.3/nonebot_plugin_groupmate_waifu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 12:07:13.000000 nonebot_plugin_groupmate_waifu-1.3.3/nonebot_plugin_groupmate_waifu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2023-08-07 12:07:13.000000 nonebot_plugin_groupmate_waifu-1.3.3/nonebot_plugin_groupmate_waifu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       31 2023-08-07 12:07:13.000000 nonebot_plugin_groupmate_waifu-1.3.3/nonebot_plugin_groupmate_waifu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-07 12:07:13.454850 nonebot_plugin_groupmate_waifu-1.3.3/setup.cfg
+-rw-rw-rw-   0        0        0      567 2023-08-07 12:07:10.000000 nonebot_plugin_groupmate_waifu-1.3.3/setup.py
```

### Comparing `nonebot_plugin_groupmate_waifu-1.3.2/LICENSE` & `nonebot_plugin_groupmate_waifu-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_groupmate_waifu-1.3.2/nonebot_plugin_groupmate_waifu/__init__.py` & `nonebot_plugin_groupmate_waifu-1.3.3/nonebot_plugin_groupmate_waifu/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -242,15 +242,15 @@
                 msg = tips + MessageSegment.image(file = await user_img(waifu_id)) + f"『{member['card'] or member['nickname']}』！"
             await bot.send(event,msg,at_sender = True)
             return False
 
     if at:
         if at == rec.get(at):
             X = HE
-            del rec[waifu_id]
+            del rec[at]
         else:
             X = random.randint(1,100)
 
         if 0 < X <= HE:
             waifu_id = at
             tips = "恭喜你娶到了群友!\n" + tips
         elif HE < X <= BE:
```

### Comparing `nonebot_plugin_groupmate_waifu-1.3.2/nonebot_plugin_groupmate_waifu/utils.py` & `nonebot_plugin_groupmate_waifu-1.3.3/nonebot_plugin_groupmate_waifu/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_groupmate_waifu-1.3.2/setup.py` & `nonebot_plugin_groupmate_waifu-1.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup,find_namespace_packages
 
 setup(
 name='nonebot_plugin_groupmate_waifu',
-version='1.3.2',
+version='1.3.3',
 description='娶群友',
 #long_description=open('README.md','r').read(),
 author='karisaya',
 author_email='1048827424@qq.com',
 license='MIT license',
 include_package_data=True,
 packages=find_namespace_packages(include=["nonebot_plugin_groupmate_waifu"]),
```

