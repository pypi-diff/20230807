# Comparing `tmp/mikan_card_downloader-1.2.0.tar.gz` & `tmp/mikan_card_downloader-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mikan_card_downloader-1.2.0.tar", max compression
+gzip compressed data, was "mikan_card_downloader-1.2.1.tar", max compression
```

## Comparing `mikan_card_downloader-1.2.0.tar` & `mikan_card_downloader-1.2.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    35149 2021-11-29 13:57:47.295968 mikan_card_downloader-1.2.0/LICENSE
--rw-r--r--   0        0        0     1041 2023-08-06 21:29:30.042111 mikan_card_downloader-1.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-20 20:32:09.133338 mikan_card_downloader-1.2.0/src/mikan/__init__.py
--rw-r--r--   0        0        0     1536 2023-05-05 22:20:27.438705 mikan_card_downloader-1.2.0/src/mikan/classes.py
--rw-r--r--   0        0        0     1491 2023-07-26 18:37:20.320555 mikan_card_downloader-1.2.0/src/mikan/config.py
--rw-r--r--   0        0        0     3360 2023-08-06 21:27:00.227335 mikan_card_downloader-1.2.0/src/mikan/downloader.py
--rw-r--r--   0        0        0     5673 2023-05-31 10:47:12.451838 mikan_card_downloader-1.2.0/src/mikan/html_parser.py
--rw-r--r--   0        0        0     1382 2023-04-23 20:48:44.204752 mikan_card_downloader-1.2.0/src/mikan/json_utils.py
--rwxr-xr-x   0        0        0     2402 2023-08-06 21:27:00.227335 mikan_card_downloader-1.2.0/src/mikan/main.py
--rw-r--r--   0        0        0        0 2023-04-20 20:32:09.133338 mikan_card_downloader-1.2.0/src/mikan/py.typed
--rw-r--r--   0        0        0      594 1970-01-01 00:00:00.000000 mikan_card_downloader-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2021-11-29 13:57:47.295968 mikan_card_downloader-1.2.1/LICENSE
+-rw-r--r--   0        0        0     1041 2023-08-07 01:48:23.810289 mikan_card_downloader-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-20 20:32:09.133338 mikan_card_downloader-1.2.1/src/mikan/__init__.py
+-rw-r--r--   0        0        0     1536 2023-05-05 22:20:27.438705 mikan_card_downloader-1.2.1/src/mikan/classes.py
+-rw-r--r--   0        0        0     1491 2023-07-26 18:37:20.320555 mikan_card_downloader-1.2.1/src/mikan/config.py
+-rw-r--r--   0        0        0     3312 2023-08-07 01:29:29.992843 mikan_card_downloader-1.2.1/src/mikan/downloader.py
+-rw-r--r--   0        0        0     5622 2023-08-07 01:40:43.541854 mikan_card_downloader-1.2.1/src/mikan/html_parser.py
+-rw-r--r--   0        0        0     1382 2023-04-23 20:48:44.204752 mikan_card_downloader-1.2.1/src/mikan/json_utils.py
+-rwxr-xr-x   0        0        0     2402 2023-08-06 21:27:00.227335 mikan_card_downloader-1.2.1/src/mikan/main.py
+-rw-r--r--   0        0        0        0 2023-04-20 20:32:09.133338 mikan_card_downloader-1.2.1/src/mikan/py.typed
+-rw-r--r--   0        0        0      594 1970-01-01 00:00:00.000000 mikan_card_downloader-1.2.1/PKG-INFO
```

### Comparing `mikan_card_downloader-1.2.0/LICENSE` & `mikan_card_downloader-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mikan_card_downloader-1.2.0/pyproject.toml` & `mikan_card_downloader-1.2.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mikan-card-downloader"
-version = "1.2.0"
+version = "1.2.1"
 description = "Downloads cards and stills from SIFAS and SIF."
 authors = ["DemonicSavage"]
 license = "GPLv3"
 packages = [
     {include = "mikan", from = "src"}
 ]
```

### Comparing `mikan_card_downloader-1.2.0/src/mikan/classes.py` & `mikan_card_downloader-1.2.1/src/mikan/classes.py`

 * *Files identical despite different names*

### Comparing `mikan_card_downloader-1.2.0/src/mikan/config.py` & `mikan_card_downloader-1.2.1/src/mikan/config.py`

 * *Files identical despite different names*

### Comparing `mikan_card_downloader-1.2.0/src/mikan/downloader.py` & `mikan_card_downloader-1.2.1/src/mikan/downloader.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,15 +52,14 @@
     async def __aexit__(self, ext_type: None, value: None, trace: None) -> None:
         await self.session.close()
 
     async def download_file(self, item: str) -> None:
         try:
             res = await self.session.get(f"https:{item}")
             if res.status == 200:
-                # res_data = await res.read()
                 self.path.mkdir(exist_ok=True, parents=True)
 
                 with open(self.path / self.get_card_image_name(item), "wb") as file:
                     async for chunk in res.content.iter_any():
                         file.write(chunk)
 
                 message = f"Downloaded item {self.get_card_image_name(item)}."
@@ -72,15 +71,15 @@
 
     def get_card_image_name(self, url: str) -> str:
         return url.split("/")[-1]
 
     async def get(self) -> None:
         tasks: list[Coroutine[Any, Any, None]] = []
 
-        for _, item in self.objs[self.img_type.results_dir].items():
+        for item in self.objs[self.img_type.results_dir].values():
             tasks.extend(
                 [
                     self.download_file(card)
                     for card in item
                     if not (self.path / self.get_card_image_name(card)).exists()
                 ]
             )
```

### Comparing `mikan_card_downloader-1.2.0/src/mikan/html_parser.py` & `mikan_card_downloader-1.2.1/src/mikan/html_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 # You should have received a copy of the GNU General Public License
 
 from __future__ import annotations
 
 import asyncio
 import re
-from typing import Any, Coroutine
+from typing import Any
 
 import aiohttp
 import bs4
 
 from mikan.classes import Item, SIFCard, Still
 
 
@@ -52,25 +52,26 @@
         elif self.img_type == Still:
             self.item_parser = StillParser()
 
     async def request_url_data(self, url: str) -> aiohttp.ClientResponse:
         return await self.session.get(url)
 
     async def get_page(self, idx: int) -> list[None]:
-        tasks: list[Coroutine[Any, Any, None]] = []
         data = (
             await self.request_url_data(f"{self.img_type.list_url_template}{idx}")
             if self.img_type != SIFCard
             else idx
         )
         page = await self.list_parser.get_page(data)
 
-        for item in page:
-            if str(item) not in self.objs[self.img_type.results_dir]:
-                tasks.append(self.add_item_to_object_list(item))
+        tasks = [
+            self.add_item_to_object_list(item)
+            for item in page
+            if str(item) not in self.objs[self.img_type.results_dir]
+        ]
 
         res: list[None] = await asyncio.gather(*tasks, return_exceptions=False)
 
         return res
 
     async def get_cards_from_pages(self) -> None:
         num_pages = (
```

### Comparing `mikan_card_downloader-1.2.0/src/mikan/json_utils.py` & `mikan_card_downloader-1.2.1/src/mikan/json_utils.py`

 * *Files identical despite different names*

### Comparing `mikan_card_downloader-1.2.0/src/mikan/main.py` & `mikan_card_downloader-1.2.1/src/mikan/main.py`

 * *Files identical despite different names*

### Comparing `mikan_card_downloader-1.2.0/PKG-INFO` & `mikan_card_downloader-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mikan-card-downloader
-Version: 1.2.0
+Version: 1.2.1
 Summary: Downloads cards and stills from SIFAS and SIF.
 License: GPLv3
 Author: DemonicSavage
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

