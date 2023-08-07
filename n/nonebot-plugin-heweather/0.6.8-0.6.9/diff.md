# Comparing `tmp/nonebot_plugin_heweather-0.6.8.tar.gz` & `tmp/nonebot_plugin_heweather-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_heweather-0.6.8.tar", last modified: Wed Jun 21 08:41:15 2023, max compression
+gzip compressed data, was "nonebot_plugin_heweather-0.6.9.tar", last modified: Tue Jun 27 01:31:36 2023, max compression
```

## Comparing `nonebot_plugin_heweather-0.6.8.tar` & `nonebot_plugin_heweather-0.6.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1062 2023-06-21 08:41:07.723333 nonebot_plugin_heweather-0.6.8/LICENSE
--rw-r--r--   0        0        0     2272 2023-06-21 08:41:07.723333 nonebot_plugin_heweather-0.6.8/README.md
--rw-r--r--   0        0        0     1975 2023-06-21 08:41:07.731333 nonebot_plugin_heweather-0.6.8/nonebot_plugin_heweather/__init__.py
--rw-r--r--   0        0        0      435 2023-06-21 08:41:07.731333 nonebot_plugin_heweather-0.6.8/nonebot_plugin_heweather/config.py
--rw-r--r--   0        0        0     1104 2023-06-21 08:41:07.731333 nonebot_plugin_heweather-0.6.8/nonebot_plugin_heweather/model.py
--rw-r--r--   0        0        0     1785 2023-06-21 08:41:07.731333 nonebot_plugin_heweather-0.6.8/nonebot_plugin_heweather/render_pic.py
--rwxr-xr-x   0        0        0    69948 2023-06-21 08:41:07.731333 nonebot_plugin_heweather-0.6.8/nonebot_plugin_heweather/templates/css/fonts/qweather-icons.ttf
--rwxr-xr-x   0        0        0    27920 2023-06-21 08:41:07.731333 nonebot_plugin_heweather-0.6.8/nonebot_plugin_heweather/templates/css/fonts/qweather-icons.woff
--rwxr-xr-x   0        0        0    19688 2023-06-21 08:41:07.731333 nonebot_plugin_heweather-0.6.8/nonebot_plugin_heweather/templates/css/fonts/qweather-icons.woff2
--rwxr-xr-x   0        0        0    20240 2023-06-21 08:41:07.731333 nonebot_plugin_heweather-0.6.8/nonebot_plugin_heweather/templates/css/qweather-icons.css
--rwxr-xr-x   0        0        0     9784 2023-06-21 08:41:07.731333 nonebot_plugin_heweather-0.6.8/nonebot_plugin_heweather/templates/css/qweather-icons.json
--rw-r--r--   0        0        0     2850 2023-06-21 08:41:07.731333 nonebot_plugin_heweather-0.6.8/nonebot_plugin_heweather/templates/css/weather.css
--rw-r--r--   0        0        0     5219 2023-06-21 08:41:07.731333 nonebot_plugin_heweather-0.6.8/nonebot_plugin_heweather/templates/weather.html
--rw-r--r--   0        0        0     4978 2023-06-21 08:41:07.731333 nonebot_plugin_heweather-0.6.8/nonebot_plugin_heweather/weather_data.py
--rw-r--r--   0        0        0      993 2023-06-21 08:41:15.807415 nonebot_plugin_heweather-0.6.8/pyproject.toml
--rw-r--r--   0        0        0        6 2023-06-21 08:41:07.735333 nonebot_plugin_heweather-0.6.8/tests/.gitignore
--rw-r--r--   0        0        0        0 2023-06-21 08:41:07.735333 nonebot_plugin_heweather-0.6.8/tests/__init__.py
--rw-r--r--   0        0        0      487 2023-06-21 08:41:07.735333 nonebot_plugin_heweather-0.6.8/tests/conftest.py
--rw-r--r--   0        0        0      784 2023-06-21 08:41:07.735333 nonebot_plugin_heweather-0.6.8/tests/test_heweather.py
--rw-r--r--   0        0        0     4103 1970-01-01 00:00:00.000000 nonebot_plugin_heweather-0.6.8/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-06-27 01:31:22.738371 nonebot_plugin_heweather-0.6.9/LICENSE
+-rw-r--r--   0        0        0     2272 2023-06-27 01:31:22.738371 nonebot_plugin_heweather-0.6.9/README.md
+-rw-r--r--   0        0        0     1975 2023-06-27 01:31:22.742371 nonebot_plugin_heweather-0.6.9/nonebot_plugin_heweather/__init__.py
+-rw-r--r--   0        0        0      435 2023-06-27 01:31:22.742371 nonebot_plugin_heweather-0.6.9/nonebot_plugin_heweather/config.py
+-rw-r--r--   0        0        0     1104 2023-06-27 01:31:22.742371 nonebot_plugin_heweather-0.6.9/nonebot_plugin_heweather/model.py
+-rw-r--r--   0        0        0     1785 2023-06-27 01:31:22.746371 nonebot_plugin_heweather-0.6.9/nonebot_plugin_heweather/render_pic.py
+-rwxr-xr-x   0        0        0    69948 2023-06-27 01:31:22.746371 nonebot_plugin_heweather-0.6.9/nonebot_plugin_heweather/templates/css/fonts/qweather-icons.ttf
+-rwxr-xr-x   0        0        0    27920 2023-06-27 01:31:22.746371 nonebot_plugin_heweather-0.6.9/nonebot_plugin_heweather/templates/css/fonts/qweather-icons.woff
+-rwxr-xr-x   0        0        0    19688 2023-06-27 01:31:22.746371 nonebot_plugin_heweather-0.6.9/nonebot_plugin_heweather/templates/css/fonts/qweather-icons.woff2
+-rwxr-xr-x   0        0        0    20240 2023-06-27 01:31:22.746371 nonebot_plugin_heweather-0.6.9/nonebot_plugin_heweather/templates/css/qweather-icons.css
+-rwxr-xr-x   0        0        0     9784 2023-06-27 01:31:22.746371 nonebot_plugin_heweather-0.6.9/nonebot_plugin_heweather/templates/css/qweather-icons.json
+-rw-r--r--   0        0        0     2850 2023-06-27 01:31:22.746371 nonebot_plugin_heweather-0.6.9/nonebot_plugin_heweather/templates/css/weather.css
+-rw-r--r--   0        0        0     5219 2023-06-27 01:31:22.746371 nonebot_plugin_heweather-0.6.9/nonebot_plugin_heweather/templates/weather.html
+-rw-r--r--   0        0        0     5022 2023-06-27 01:31:22.746371 nonebot_plugin_heweather-0.6.9/nonebot_plugin_heweather/weather_data.py
+-rw-r--r--   0        0        0      993 2023-06-27 01:31:36.810701 nonebot_plugin_heweather-0.6.9/pyproject.toml
+-rw-r--r--   0        0        0        6 2023-06-27 01:31:22.746371 nonebot_plugin_heweather-0.6.9/tests/.gitignore
+-rw-r--r--   0        0        0        0 2023-06-27 01:31:22.746371 nonebot_plugin_heweather-0.6.9/tests/__init__.py
+-rw-r--r--   0        0        0      487 2023-06-27 01:31:22.746371 nonebot_plugin_heweather-0.6.9/tests/conftest.py
+-rw-r--r--   0        0        0      784 2023-06-27 01:31:22.746371 nonebot_plugin_heweather-0.6.9/tests/test_heweather.py
+-rw-r--r--   0        0        0     4103 1970-01-01 00:00:00.000000 nonebot_plugin_heweather-0.6.9/PKG-INFO
```

### Comparing `nonebot_plugin_heweather-0.6.8/LICENSE` & `nonebot_plugin_heweather-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_heweather-0.6.8/README.md` & `nonebot_plugin_heweather-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_heweather-0.6.8/nonebot_plugin_heweather/__init__.py` & `nonebot_plugin_heweather-0.6.9/nonebot_plugin_heweather/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_heweather-0.6.8/nonebot_plugin_heweather/model.py` & `nonebot_plugin_heweather-0.6.9/nonebot_plugin_heweather/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_heweather-0.6.8/nonebot_plugin_heweather/render_pic.py` & `nonebot_plugin_heweather-0.6.9/nonebot_plugin_heweather/render_pic.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_heweather-0.6.8/nonebot_plugin_heweather/templates/css/fonts/qweather-icons.ttf` & `nonebot_plugin_heweather-0.6.9/nonebot_plugin_heweather/templates/css/fonts/qweather-icons.ttf`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_heweather-0.6.8/nonebot_plugin_heweather/templates/css/fonts/qweather-icons.woff` & `nonebot_plugin_heweather-0.6.9/nonebot_plugin_heweather/templates/css/fonts/qweather-icons.woff`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_heweather-0.6.8/nonebot_plugin_heweather/templates/css/fonts/qweather-icons.woff2` & `nonebot_plugin_heweather-0.6.9/nonebot_plugin_heweather/templates/css/fonts/qweather-icons.woff2`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_heweather-0.6.8/nonebot_plugin_heweather/templates/css/qweather-icons.css` & `nonebot_plugin_heweather-0.6.9/nonebot_plugin_heweather/templates/css/qweather-icons.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_heweather-0.6.8/nonebot_plugin_heweather/templates/css/qweather-icons.json` & `nonebot_plugin_heweather-0.6.9/nonebot_plugin_heweather/templates/css/qweather-icons.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_heweather-0.6.8/nonebot_plugin_heweather/templates/css/weather.css` & `nonebot_plugin_heweather-0.6.9/nonebot_plugin_heweather/templates/css/weather.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_heweather-0.6.8/nonebot_plugin_heweather/templates/weather.html` & `nonebot_plugin_heweather-0.6.9/nonebot_plugin_heweather/templates/weather.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_heweather-0.6.8/nonebot_plugin_heweather/weather_data.py` & `nonebot_plugin_heweather-0.6.9/nonebot_plugin_heweather/weather_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import asyncio
+from typing import Union, Optional
 
 from nonebot.log import logger
 from httpx import Response, AsyncClient
 
 from .model import AirApi, NowApi, DailyApi, WarningApi
 
 
@@ -40,15 +41,15 @@
                 logger.info("使用个人开发版API")
         else:
             raise ConfigError(
                 "api_type 必须是为 (int)0 -> 普通版, (int)1 -> 个人开发版, (int)2 -> 商业版"
                 f"\n当前为: ({type(self.api_type)}){self.api_type}"
             )
 
-    def __init__(self, city_name: str, api_key: str, api_type: int | str = 0):
+    def __init__(self, city_name: str, api_key: str, api_type: Union[int, str] = 0):
         self.city_name = city_name
         self.apikey = api_key
         self.api_type = int(api_type)
         self.__url__()
 
         # self.now: Optional[Dict[str, str]] = None
         # self.daily = None
@@ -128,14 +129,14 @@
             url=self.url_air,
             params={"location": self.city_id, "key": self.apikey},
         )
         self._check_response(res)
         return AirApi(**res.json())
 
     @property
-    async def _warning(self) -> WarningApi | None:
+    async def _warning(self) -> Optional[WarningApi]:
         res = await self._get_data(
             url=self.url_weather_warning,
             params={"location": self.city_id, "key": self.apikey},
         )
         self._check_response(res)
         return None if res.json().get("code") == "204" else WarningApi(**res.json())
```

### Comparing `nonebot_plugin_heweather-0.6.8/pyproject.toml` & `nonebot_plugin_heweather-0.6.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-heweather"
-version = "0.6.8"
+version = "0.6.9"
 description = "Get Heweather information and convert to pictures"
 authors = [
     { name = "kexue", email = "xana278@foxmail.com" },
 ]
 dependencies = [
     "httpx<1.0.0,>=0.18.0",
     "nonebot-plugin-htmlrender>=0.0.4.3",
```

### Comparing `nonebot_plugin_heweather-0.6.8/tests/test_heweather.py` & `nonebot_plugin_heweather-0.6.9/tests/test_heweather.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_heweather-0.6.8/PKG-INFO` & `nonebot_plugin_heweather-0.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-heweather
-Version: 0.6.8
+Version: 0.6.9
 Summary: Get Heweather information and convert to pictures
 Author-Email: kexue <xana278@foxmail.com>
 License: MIT License
         
         Copyright (c) 2021 kexue
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-heweather Version: 0.6.8 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-heweather Version: 0.6.9 Summary:
 Get Heweather information and convert to pictures Author-Email: kexue
 foxmail.com> License: MIT License Copyright (c) 2021 kexue Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
```

