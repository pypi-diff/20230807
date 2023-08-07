# Comparing `tmp/iamlistening-3.1.5.tar.gz` & `tmp/iamlistening-3.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iamlistening-3.1.5.tar", max compression
+gzip compressed data, was "iamlistening-3.1.6.tar", max compression
```

## Comparing `iamlistening-3.1.5.tar` & `iamlistening-3.1.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1064 2023-08-07 10:25:08.873431 iamlistening-3.1.5/LICENSE
--rw-r--r--   0        0        0     2457 2023-08-07 10:25:08.873431 iamlistening-3.1.5/README.md
--rw-r--r--   0        0        0       81 2023-08-07 10:25:18.557492 iamlistening-3.1.5/iamlistening/__init__.py
--rw-r--r--   0        0        0      688 2023-08-07 10:25:08.881431 iamlistening-3.1.5/iamlistening/config.py
--rw-r--r--   0        0        0     1376 2023-08-07 10:25:08.881431 iamlistening-3.1.5/iamlistening/default_settings.toml
--rw-r--r--   0        0        0     1673 2023-08-07 10:25:08.881431 iamlistening-3.1.5/iamlistening/main.py
--rw-r--r--   0        0        0        0 2023-08-07 10:25:08.881431 iamlistening-3.1.5/iamlistening/platform/__init__.py
--rw-r--r--   0        0        0     3276 2023-08-07 10:25:08.881431 iamlistening-3.1.5/iamlistening/platform/chat_manager.py
--rw-r--r--   0        0        0       56 2023-08-07 10:25:08.881431 iamlistening-3.1.5/iamlistening/platform/clients/__init__.py
--rw-r--r--   0        0        0      876 2023-08-07 10:25:08.881431 iamlistening-3.1.5/iamlistening/platform/clients/discord.py
--rw-r--r--   0        0        0      738 2023-08-07 10:25:08.881431 iamlistening-3.1.5/iamlistening/platform/clients/guilded.py
--rw-r--r--   0        0        0      672 2023-08-07 10:25:08.881431 iamlistening-3.1.5/iamlistening/platform/clients/lemmy.py
--rw-r--r--   0        0        0     1349 2023-08-07 10:25:08.881431 iamlistening-3.1.5/iamlistening/platform/clients/mastodon.py
--rw-r--r--   0        0        0     1616 2023-08-07 10:25:08.881431 iamlistening-3.1.5/iamlistening/platform/clients/matrix.py
--rw-r--r--   0        0        0      912 2023-08-07 10:25:08.881431 iamlistening-3.1.5/iamlistening/platform/clients/revolt.py
--rw-r--r--   0        0        0      806 2023-08-07 10:25:08.881431 iamlistening-3.1.5/iamlistening/platform/clients/rocket_chat.py
--rw-r--r--   0        0        0     1176 2023-08-07 10:25:08.881431 iamlistening-3.1.5/iamlistening/platform/clients/telegram.py
--rw-r--r--   0        0        0      568 2023-08-07 10:25:08.881431 iamlistening-3.1.5/iamlistening/platform/clients/tinode.py
--rw-r--r--   0        0        0     3313 2023-08-07 10:25:18.545492 iamlistening-3.1.5/pyproject.toml
--rw-r--r--   0        0        0     3707 1970-01-01 00:00:00.000000 iamlistening-3.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-08-07 12:04:38.200574 iamlistening-3.1.6/LICENSE
+-rw-r--r--   0        0        0     2457 2023-08-07 12:04:38.200574 iamlistening-3.1.6/README.md
+-rw-r--r--   0        0        0       81 2023-08-07 12:04:40.080722 iamlistening-3.1.6/iamlistening/__init__.py
+-rw-r--r--   0        0        0      688 2023-08-07 12:04:38.204574 iamlistening-3.1.6/iamlistening/config.py
+-rw-r--r--   0        0        0     1376 2023-08-07 12:04:38.204574 iamlistening-3.1.6/iamlistening/default_settings.toml
+-rw-r--r--   0        0        0     1673 2023-08-07 12:04:38.204574 iamlistening-3.1.6/iamlistening/main.py
+-rw-r--r--   0        0        0        0 2023-08-07 12:04:38.204574 iamlistening-3.1.6/iamlistening/platform/__init__.py
+-rw-r--r--   0        0        0     3276 2023-08-07 12:04:38.204574 iamlistening-3.1.6/iamlistening/platform/chat_manager.py
+-rw-r--r--   0        0        0       56 2023-08-07 12:04:38.204574 iamlistening-3.1.6/iamlistening/platform/clients/__init__.py
+-rw-r--r--   0        0        0      876 2023-08-07 12:04:38.204574 iamlistening-3.1.6/iamlistening/platform/clients/discord.py
+-rw-r--r--   0        0        0      738 2023-08-07 12:04:38.204574 iamlistening-3.1.6/iamlistening/platform/clients/guilded.py
+-rw-r--r--   0        0        0      672 2023-08-07 12:04:38.204574 iamlistening-3.1.6/iamlistening/platform/clients/lemmy.py
+-rw-r--r--   0        0        0     1349 2023-08-07 12:04:38.204574 iamlistening-3.1.6/iamlistening/platform/clients/mastodon.py
+-rw-r--r--   0        0        0     1616 2023-08-07 12:04:38.204574 iamlistening-3.1.6/iamlistening/platform/clients/matrix.py
+-rw-r--r--   0        0        0      912 2023-08-07 12:04:38.204574 iamlistening-3.1.6/iamlistening/platform/clients/revolt.py
+-rw-r--r--   0        0        0      806 2023-08-07 12:04:38.204574 iamlistening-3.1.6/iamlistening/platform/clients/rocket_chat.py
+-rw-r--r--   0        0        0     1176 2023-08-07 12:04:38.204574 iamlistening-3.1.6/iamlistening/platform/clients/telegram.py
+-rw-r--r--   0        0        0      568 2023-08-07 12:04:38.204574 iamlistening-3.1.6/iamlistening/platform/clients/tinode.py
+-rw-r--r--   0        0        0     3313 2023-08-07 12:04:40.072721 iamlistening-3.1.6/pyproject.toml
+-rw-r--r--   0        0        0     3707 1970-01-01 00:00:00.000000 iamlistening-3.1.6/PKG-INFO
```

### Comparing `iamlistening-3.1.5/LICENSE` & `iamlistening-3.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `iamlistening-3.1.5/README.md` & `iamlistening-3.1.6/README.md`

 * *Files identical despite different names*

### Comparing `iamlistening-3.1.5/iamlistening/config.py` & `iamlistening-3.1.6/iamlistening/config.py`

 * *Files identical despite different names*

### Comparing `iamlistening-3.1.5/iamlistening/default_settings.toml` & `iamlistening-3.1.6/iamlistening/default_settings.toml`

 * *Files identical despite different names*

### Comparing `iamlistening-3.1.5/iamlistening/main.py` & `iamlistening-3.1.6/iamlistening/main.py`

 * *Files identical despite different names*

### Comparing `iamlistening-3.1.5/iamlistening/platform/chat_manager.py` & `iamlistening-3.1.6/iamlistening/platform/chat_manager.py`

 * *Files identical despite different names*

### Comparing `iamlistening-3.1.5/iamlistening/platform/clients/discord.py` & `iamlistening-3.1.6/iamlistening/platform/clients/discord.py`

 * *Files identical despite different names*

### Comparing `iamlistening-3.1.5/iamlistening/platform/clients/guilded.py` & `iamlistening-3.1.6/iamlistening/platform/clients/guilded.py`

 * *Files identical despite different names*

### Comparing `iamlistening-3.1.5/iamlistening/platform/clients/lemmy.py` & `iamlistening-3.1.6/iamlistening/platform/clients/lemmy.py`

 * *Files identical despite different names*

### Comparing `iamlistening-3.1.5/iamlistening/platform/clients/mastodon.py` & `iamlistening-3.1.6/iamlistening/platform/clients/mastodon.py`

 * *Files identical despite different names*

### Comparing `iamlistening-3.1.5/iamlistening/platform/clients/matrix.py` & `iamlistening-3.1.6/iamlistening/platform/clients/matrix.py`

 * *Files identical despite different names*

### Comparing `iamlistening-3.1.5/iamlistening/platform/clients/revolt.py` & `iamlistening-3.1.6/iamlistening/platform/clients/revolt.py`

 * *Files identical despite different names*

### Comparing `iamlistening-3.1.5/iamlistening/platform/clients/rocket_chat.py` & `iamlistening-3.1.6/iamlistening/platform/clients/rocket_chat.py`

 * *Files identical despite different names*

### Comparing `iamlistening-3.1.5/iamlistening/platform/clients/telegram.py` & `iamlistening-3.1.6/iamlistening/platform/clients/telegram.py`

 * *Files identical despite different names*

### Comparing `iamlistening-3.1.5/iamlistening/platform/clients/tinode.py` & `iamlistening-3.1.6/iamlistening/platform/clients/tinode.py`

 * *Files identical despite different names*

### Comparing `iamlistening-3.1.5/pyproject.toml` & `iamlistening-3.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "iamlistening"
-version = "3.1.5"
+version = "3.1.6"
 description = "A python package to interact with messaging platform."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = [
     "bot","messaging",
     "discord", "telegram","matrix","rocket chat",
```

### Comparing `iamlistening-3.1.5/PKG-INFO` & `iamlistening-3.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iamlistening
-Version: 3.1.5
+Version: 3.1.6
 Summary: A python package to interact with messaging platform.
 License: MIT
 Keywords: bot,messaging,discord,telegram,matrix,rocket chat
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: iamlistening Version: 3.1.5 Summary: A python
+Metadata-Version: 2.1 Name: iamlistening Version: 3.1.6 Summary: A python
 package to interact with messaging platform. License: MIT Keywords:
 bot,messaging,discord,telegram,matrix,rocket chat Author: mraniki Author-email:
 8766259+mraniki@users.noreply.github.com Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: Mastodon.py
 (>=1.8.1,<2.0.0) Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0) Requires-Dist:
```

