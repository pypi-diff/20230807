# Comparing `tmp/iamlistening-3.1.4.tar.gz` & `tmp/iamlistening-3.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iamlistening-3.1.4.tar", max compression
+gzip compressed data, was "iamlistening-3.1.5.tar", max compression
```

## Comparing `iamlistening-3.1.4.tar` & `iamlistening-3.1.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1064 2023-08-06 14:11:03.794532 iamlistening-3.1.4/LICENSE
--rw-r--r--   0        0        0     2755 2023-08-06 14:11:03.794532 iamlistening-3.1.4/README.md
--rw-r--r--   0        0        0       81 2023-08-06 14:11:05.414533 iamlistening-3.1.4/iamlistening/__init__.py
--rw-r--r--   0        0        0      688 2023-08-06 14:11:03.794532 iamlistening-3.1.4/iamlistening/config.py
--rw-r--r--   0        0        0     1376 2023-08-06 14:11:03.794532 iamlistening-3.1.4/iamlistening/default_settings.toml
--rw-r--r--   0        0        0     1673 2023-08-06 14:11:03.794532 iamlistening-3.1.4/iamlistening/main.py
--rw-r--r--   0        0        0        0 2023-08-06 14:11:03.794532 iamlistening-3.1.4/iamlistening/platform/__init__.py
--rw-r--r--   0        0        0     3275 2023-08-06 14:11:03.794532 iamlistening-3.1.4/iamlistening/platform/chat_manager.py
--rw-r--r--   0        0        0        0 2023-08-06 14:11:03.794532 iamlistening-3.1.4/iamlistening/platform/clients/__init__.py
--rw-r--r--   0        0        0      876 2023-08-06 14:11:03.794532 iamlistening-3.1.4/iamlistening/platform/clients/discord.py
--rw-r--r--   0        0        0      738 2023-08-06 14:11:03.794532 iamlistening-3.1.4/iamlistening/platform/clients/guilded.py
--rw-r--r--   0        0        0      672 2023-08-06 14:11:03.794532 iamlistening-3.1.4/iamlistening/platform/clients/lemmy.py
--rw-r--r--   0        0        0     1349 2023-08-06 14:11:03.794532 iamlistening-3.1.4/iamlistening/platform/clients/mastodon.py
--rw-r--r--   0        0        0     1616 2023-08-06 14:11:03.794532 iamlistening-3.1.4/iamlistening/platform/clients/matrix.py
--rw-r--r--   0        0        0      912 2023-08-06 14:11:03.794532 iamlistening-3.1.4/iamlistening/platform/clients/revolt.py
--rw-r--r--   0        0        0      806 2023-08-06 14:11:03.794532 iamlistening-3.1.4/iamlistening/platform/clients/rocket_chat.py
--rw-r--r--   0        0        0     1176 2023-08-06 14:11:03.794532 iamlistening-3.1.4/iamlistening/platform/clients/telegram.py
--rw-r--r--   0        0        0      568 2023-08-06 14:11:03.794532 iamlistening-3.1.4/iamlistening/platform/clients/tinode.py
--rw-r--r--   0        0        0     3221 2023-08-06 14:11:05.406533 iamlistening-3.1.4/pyproject.toml
--rw-r--r--   0        0        0     4005 1970-01-01 00:00:00.000000 iamlistening-3.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-08-07 10:25:08.873431 iamlistening-3.1.5/LICENSE
+-rw-r--r--   0        0        0     2457 2023-08-07 10:25:08.873431 iamlistening-3.1.5/README.md
+-rw-r--r--   0        0        0       81 2023-08-07 10:25:18.557492 iamlistening-3.1.5/iamlistening/__init__.py
+-rw-r--r--   0        0        0      688 2023-08-07 10:25:08.881431 iamlistening-3.1.5/iamlistening/config.py
+-rw-r--r--   0        0        0     1376 2023-08-07 10:25:08.881431 iamlistening-3.1.5/iamlistening/default_settings.toml
+-rw-r--r--   0        0        0     1673 2023-08-07 10:25:08.881431 iamlistening-3.1.5/iamlistening/main.py
+-rw-r--r--   0        0        0        0 2023-08-07 10:25:08.881431 iamlistening-3.1.5/iamlistening/platform/__init__.py
+-rw-r--r--   0        0        0     3276 2023-08-07 10:25:08.881431 iamlistening-3.1.5/iamlistening/platform/chat_manager.py
+-rw-r--r--   0        0        0       56 2023-08-07 10:25:08.881431 iamlistening-3.1.5/iamlistening/platform/clients/__init__.py
+-rw-r--r--   0        0        0      876 2023-08-07 10:25:08.881431 iamlistening-3.1.5/iamlistening/platform/clients/discord.py
+-rw-r--r--   0        0        0      738 2023-08-07 10:25:08.881431 iamlistening-3.1.5/iamlistening/platform/clients/guilded.py
+-rw-r--r--   0        0        0      672 2023-08-07 10:25:08.881431 iamlistening-3.1.5/iamlistening/platform/clients/lemmy.py
+-rw-r--r--   0        0        0     1349 2023-08-07 10:25:08.881431 iamlistening-3.1.5/iamlistening/platform/clients/mastodon.py
+-rw-r--r--   0        0        0     1616 2023-08-07 10:25:08.881431 iamlistening-3.1.5/iamlistening/platform/clients/matrix.py
+-rw-r--r--   0        0        0      912 2023-08-07 10:25:08.881431 iamlistening-3.1.5/iamlistening/platform/clients/revolt.py
+-rw-r--r--   0        0        0      806 2023-08-07 10:25:08.881431 iamlistening-3.1.5/iamlistening/platform/clients/rocket_chat.py
+-rw-r--r--   0        0        0     1176 2023-08-07 10:25:08.881431 iamlistening-3.1.5/iamlistening/platform/clients/telegram.py
+-rw-r--r--   0        0        0      568 2023-08-07 10:25:08.881431 iamlistening-3.1.5/iamlistening/platform/clients/tinode.py
+-rw-r--r--   0        0        0     3313 2023-08-07 10:25:18.545492 iamlistening-3.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3707 1970-01-01 00:00:00.000000 iamlistening-3.1.5/PKG-INFO
```

### Comparing `iamlistening-3.1.4/LICENSE` & `iamlistening-3.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `iamlistening-3.1.4/README.md` & `iamlistening-3.1.5/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 
 <table style="border: 1px solid transparent">
   <tr>
     <td>
 <a href="https://talkytrader.github.io/wiki/"><img src="https://img.shields.io/badge/Wiki-%23000000.svg?style=for-the-badge&logo=wikipedia&logoColor=white"></a>
-<a href="https://github.com/mraniki/tt/"><img src="https://img.shields.io/badge/github-%23000000.svg?style=for-the-badge&logo=github&logoColor=white"></a>
-<a href="https://coindrop.to/mraniki"><img src="https://img.shields.io/badge/tips-000000?style=for-the-badge&logo=buymeacoffee&logoColor=white"></a><br>
-<a href="https://hub.docker.com/r/mraniki/tt"><img src="https://img.shields.io/docker/pulls/mraniki/tt?style=for-the-badge"></a>
-<a href="https://t.me/TTTalkyTraderChat/1"><img src="https://img.shields.io/badge/talky-blue?style=for-the-badge&logo=telegram&logoColor=white"></a><br>
+<a href="https://github.com/mraniki/tt/"><img src="https://img.shields.io/badge/github-%23000000.svg?style=for-the-badge&logo=github&logoColor=white"></a><br>
+<a href="https://hub.docker.com/r/mraniki/tt"><img src="https://img.shields.io/docker/pulls/mraniki/tt?style=for-the-badge"></a><br>
     </td>
     <td align="center"><img width="200" alt="Logo" src="https://user-images.githubusercontent.com/8766259/242846519-f76331f6-8821-49eb-8f1c-06aedd8557be.jpeg"></td>
   </tr>
   <tr>
     <td>
       <a href="https://pypi.org/project/iamlistening/"><img src="https://img.shields.io/pypi/v/iamlistening?style=for-the-badge&logo=PyPI&logoColor=white"></a><br>
       <a href="https://pypi.org/project/iamlistening/"><img src="https://img.shields.io/pypi/dm/iamlistening?style=for-the-badge&logo=PyPI&logoColor=white&label=pypi&labelColor=grey"></a><br>
```

#### html2text {}

```diff
@@ -1,16 +1,13 @@
 [https://img.shields.io/badge/Wiki-%23000000.svg?style=for-
 the-badge&logo=wikipedia&logoColor=white] [https://
-img.shields.io/badge/github-%23000000.svg?style=for-the-
-badge&logo=github&logoColor=white] [https://img.shields.io/
-badge/tips-000000?style=for-the-                                     [Logo]
-badge&logo=buymeacoffee&logoColor=white]
+img.shields.io/badge/github-%23000000.svg?style=for-the-             [Logo]
+badge&logo=github&logoColor=white]
 [https://img.shields.io/docker/pulls/mraniki/tt?style=for-
-the-badge] [https://img.shields.io/badge/talky-
-blue?style=for-the-badge&logo=telegram&logoColor=white]
+the-badge]
 [https://img.shields.io/pypi/v/iamlistening?style=for-the-
 badge&logo=PyPI&logoColor=white]
 [https://img.shields.io/pypi/dm/iamlistening?style=for-the-
 badge&logo=PyPI&logoColor=white&label=pypi&labelColor=grey] A python package to
 [https://img.shields.io/github/actions/workflow/status/     listen to messaging
 mraniki/iamlistening/%F0%9F%91%B7Flow.yml?style=for-the-    platforms,
 badge&logo=GitHub&logoColor=white]                          such as discord,
```

### Comparing `iamlistening-3.1.4/iamlistening/config.py` & `iamlistening-3.1.5/iamlistening/config.py`

 * *Files identical despite different names*

### Comparing `iamlistening-3.1.4/iamlistening/default_settings.toml` & `iamlistening-3.1.5/iamlistening/default_settings.toml`

 * *Files identical despite different names*

### Comparing `iamlistening-3.1.4/iamlistening/main.py` & `iamlistening-3.1.5/iamlistening/main.py`

 * *Files identical despite different names*

### Comparing `iamlistening-3.1.4/iamlistening/platform/chat_manager.py` & `iamlistening-3.1.5/iamlistening/platform/chat_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 
         Args:
             platform (str): The platform to use
 
         Returns:
             PlatformHandler
 
+
         """
         handler = None
         if platform == "telegram":
             from .clients.telegram import TelegramHandler
             handler = TelegramHandler()
         elif platform == "discord":
             from .clients.discord import DiscordHandler
```

### Comparing `iamlistening-3.1.4/iamlistening/platform/clients/discord.py` & `iamlistening-3.1.5/iamlistening/platform/clients/discord.py`

 * *Files identical despite different names*

### Comparing `iamlistening-3.1.4/iamlistening/platform/clients/guilded.py` & `iamlistening-3.1.5/iamlistening/platform/clients/guilded.py`

 * *Files identical despite different names*

### Comparing `iamlistening-3.1.4/iamlistening/platform/clients/lemmy.py` & `iamlistening-3.1.5/iamlistening/platform/clients/lemmy.py`

 * *Files identical despite different names*

### Comparing `iamlistening-3.1.4/iamlistening/platform/clients/mastodon.py` & `iamlistening-3.1.5/iamlistening/platform/clients/mastodon.py`

 * *Files identical despite different names*

### Comparing `iamlistening-3.1.4/iamlistening/platform/clients/matrix.py` & `iamlistening-3.1.5/iamlistening/platform/clients/matrix.py`

 * *Files identical despite different names*

### Comparing `iamlistening-3.1.4/iamlistening/platform/clients/revolt.py` & `iamlistening-3.1.5/iamlistening/platform/clients/revolt.py`

 * *Files identical despite different names*

### Comparing `iamlistening-3.1.4/iamlistening/platform/clients/rocket_chat.py` & `iamlistening-3.1.5/iamlistening/platform/clients/rocket_chat.py`

 * *Files identical despite different names*

### Comparing `iamlistening-3.1.4/iamlistening/platform/clients/telegram.py` & `iamlistening-3.1.5/iamlistening/platform/clients/telegram.py`

 * *Files identical despite different names*

### Comparing `iamlistening-3.1.4/iamlistening/platform/clients/tinode.py` & `iamlistening-3.1.5/iamlistening/platform/clients/tinode.py`

 * *Files identical despite different names*

### Comparing `iamlistening-3.1.4/pyproject.toml` & `iamlistening-3.1.5/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "iamlistening"
-version = "3.1.4"
+version = "3.1.5"
 description = "A python package to interact with messaging platform."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = [
     "bot","messaging",
     "discord", "telegram","matrix","rocket chat",
@@ -75,17 +75,21 @@
 pytest-mock = "^3.11.1"
 pytest-loguru = "^0.2.0"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
-sphinx = ">=5,<6"
-sphinx_bootstrap_theme = "^0.8.1"
-sphinxext-remoteliteralinclude = "^0.4.0"
+sphinx = "^7.0.0"
+pydata-sphinx-theme = "^0.13.3"
+sphinx-hoverxref = "^1.3.0"
+sphinx-notfound-page = "^0.8.3"
+sphinx_copybutton = "0.5.2"
+myst_parser = "^2.0.0"
+sphinx_design = "^0.5.0"
 
 
 [tool.pytest.ini_options]
 pythonpath = "."
 testpaths = "tests"
 python_classes = "Test*"
 log_format = "%(asctime)s - %(levelname)s - %(name)s - %(message)s"
```

### Comparing `iamlistening-3.1.4/PKG-INFO` & `iamlistening-3.1.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iamlistening
-Version: 3.1.4
+Version: 3.1.5
 Summary: A python package to interact with messaging platform.
 License: MIT
 Keywords: bot,messaging,discord,telegram,matrix,rocket chat
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -28,18 +28,16 @@
 Description-Content-Type: text/markdown
 
 
 <table style="border: 1px solid transparent">
   <tr>
     <td>
 <a href="https://talkytrader.github.io/wiki/"><img src="https://img.shields.io/badge/Wiki-%23000000.svg?style=for-the-badge&logo=wikipedia&logoColor=white"></a>
-<a href="https://github.com/mraniki/tt/"><img src="https://img.shields.io/badge/github-%23000000.svg?style=for-the-badge&logo=github&logoColor=white"></a>
-<a href="https://coindrop.to/mraniki"><img src="https://img.shields.io/badge/tips-000000?style=for-the-badge&logo=buymeacoffee&logoColor=white"></a><br>
-<a href="https://hub.docker.com/r/mraniki/tt"><img src="https://img.shields.io/docker/pulls/mraniki/tt?style=for-the-badge"></a>
-<a href="https://t.me/TTTalkyTraderChat/1"><img src="https://img.shields.io/badge/talky-blue?style=for-the-badge&logo=telegram&logoColor=white"></a><br>
+<a href="https://github.com/mraniki/tt/"><img src="https://img.shields.io/badge/github-%23000000.svg?style=for-the-badge&logo=github&logoColor=white"></a><br>
+<a href="https://hub.docker.com/r/mraniki/tt"><img src="https://img.shields.io/docker/pulls/mraniki/tt?style=for-the-badge"></a><br>
     </td>
     <td align="center"><img width="200" alt="Logo" src="https://user-images.githubusercontent.com/8766259/242846519-f76331f6-8821-49eb-8f1c-06aedd8557be.jpeg"></td>
   </tr>
   <tr>
     <td>
       <a href="https://pypi.org/project/iamlistening/"><img src="https://img.shields.io/pypi/v/iamlistening?style=for-the-badge&logo=PyPI&logoColor=white"></a><br>
       <a href="https://pypi.org/project/iamlistening/"><img src="https://img.shields.io/pypi/dm/iamlistening?style=for-the-badge&logo=PyPI&logoColor=white&label=pypi&labelColor=grey"></a><br>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: iamlistening Version: 3.1.4 Summary: A python
+Metadata-Version: 2.1 Name: iamlistening Version: 3.1.5 Summary: A python
 package to interact with messaging platform. License: MIT Keywords:
 bot,messaging,discord,telegram,matrix,rocket chat Author: mraniki Author-email:
 8766259+mraniki@users.noreply.github.com Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: Mastodon.py
 (>=1.8.1,<2.0.0) Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0) Requires-Dist:
@@ -13,21 +13,18 @@
 Dist: telethon (>=1.28.5,<2.0.0) Requires-Dist: tinode_grpc (>=0.22.3,<0.23.0)
 Project-URL: Changelog, https://github.com/mraniki/iamlistening/blob/dev/
 CHANGELOG.rst Project-URL: Issues, https://github.com/mraniki/iamlistening/
 issues Project-URL: Support, https://github.com/mraniki/iamlistening/
 discussions Description-Content-Type: text/markdown
 [https://img.shields.io/badge/Wiki-%23000000.svg?style=for-
 the-badge&logo=wikipedia&logoColor=white] [https://
-img.shields.io/badge/github-%23000000.svg?style=for-the-
-badge&logo=github&logoColor=white] [https://img.shields.io/
-badge/tips-000000?style=for-the-                                     [Logo]
-badge&logo=buymeacoffee&logoColor=white]
+img.shields.io/badge/github-%23000000.svg?style=for-the-             [Logo]
+badge&logo=github&logoColor=white]
 [https://img.shields.io/docker/pulls/mraniki/tt?style=for-
-the-badge] [https://img.shields.io/badge/talky-
-blue?style=for-the-badge&logo=telegram&logoColor=white]
+the-badge]
 [https://img.shields.io/pypi/v/iamlistening?style=for-the-
 badge&logo=PyPI&logoColor=white]
 [https://img.shields.io/pypi/dm/iamlistening?style=for-the-
 badge&logo=PyPI&logoColor=white&label=pypi&labelColor=grey] A python package to
 [https://img.shields.io/github/actions/workflow/status/     listen to messaging
 mraniki/iamlistening/%F0%9F%91%B7Flow.yml?style=for-the-    platforms,
 badge&logo=GitHub&logoColor=white]                          such as discord,
```

