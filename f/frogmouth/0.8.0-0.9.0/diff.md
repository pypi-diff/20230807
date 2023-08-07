# Comparing `tmp/frogmouth-0.8.0.tar.gz` & `tmp/frogmouth-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frogmouth-0.8.0.tar", max compression
+gzip compressed data, was "frogmouth-0.9.0.tar", max compression
```

## Comparing `frogmouth-0.8.0.tar` & `frogmouth-0.9.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1072 2023-04-27 14:46:52.801782 frogmouth-0.8.0/LICENSE
--rw-r--r--   0        0        0     2752 2023-04-30 07:26:36.700670 frogmouth-0.8.0/README.md
--rw-r--r--   0        0        0      283 2023-07-20 08:13:55.752709 frogmouth-0.8.0/frogmouth/__init__.py
--rw-r--r--   0        0        0      112 2023-04-27 14:46:52.802125 frogmouth-0.8.0/frogmouth/__main__.py
--rw-r--r--   0        0        0       74 2023-04-27 14:46:52.802222 frogmouth-0.8.0/frogmouth/app/__init__.py
--rw-r--r--   0        0        0     2070 2023-04-30 11:10:42.375933 frogmouth-0.8.0/frogmouth/app/app.py
--rw-r--r--   0        0        0      395 2023-04-27 14:46:52.802403 frogmouth-0.8.0/frogmouth/data/__init__.py
--rw-r--r--   0        0        0     1639 2023-04-27 14:46:52.802497 frogmouth-0.8.0/frogmouth/data/bookmarks.py
--rw-r--r--   0        0        0     2270 2023-05-09 08:04:58.867587 frogmouth-0.8.0/frogmouth/data/config.py
--rw-r--r--   0        0        0      582 2023-04-27 14:46:52.802650 frogmouth-0.8.0/frogmouth/data/data_directory.py
--rw-r--r--   0        0        0     1370 2023-04-27 14:46:52.802714 frogmouth-0.8.0/frogmouth/data/history.py
--rw-r--r--   0        0        0      354 2023-04-27 14:46:52.802828 frogmouth-0.8.0/frogmouth/dialogs/__init__.py
--rw-r--r--   0        0        0      565 2023-04-28 13:52:42.406602 frogmouth-0.8.0/frogmouth/dialogs/error.py
--rw-r--r--   0        0        0     4658 2023-05-30 09:10:09.565607 frogmouth-0.8.0/frogmouth/dialogs/help_dialog.py
--rw-r--r--   0        0        0      269 2023-04-27 14:55:30.387330 frogmouth-0.8.0/frogmouth/dialogs/information.py
--rw-r--r--   0        0        0     2544 2023-05-09 08:04:58.868437 frogmouth-0.8.0/frogmouth/dialogs/input_dialog.py
--rw-r--r--   0        0        0     2168 2023-04-29 20:35:07.295162 frogmouth-0.8.0/frogmouth/dialogs/text_dialog.py
--rw-r--r--   0        0        0     3602 2023-05-03 09:31:33.036152 frogmouth-0.8.0/frogmouth/dialogs/yes_no_dialog.py
--rw-r--r--   0        0        0       83 2023-04-27 14:46:52.803485 frogmouth-0.8.0/frogmouth/screens/__init__.py
--rw-r--r--   0        0        0    20103 2023-05-30 09:10:09.565826 frogmouth-0.8.0/frogmouth/screens/main.py
--rw-r--r--   0        0        0      402 2023-05-18 13:41:34.484301 frogmouth-0.8.0/frogmouth/utility/__init__.py
--rw-r--r--   0        0        0      894 2023-04-28 13:00:47.734733 frogmouth-0.8.0/frogmouth/utility/advertising.py
--rw-r--r--   0        0        0     5373 2023-05-30 09:10:09.565984 frogmouth-0.8.0/frogmouth/utility/forge.py
--rw-r--r--   0        0        0     1206 2023-05-09 08:04:58.868785 frogmouth-0.8.0/frogmouth/utility/type_tests.py
--rw-r--r--   0        0        0      184 2023-04-27 14:46:52.804110 frogmouth-0.8.0/frogmouth/widgets/__init__.py
--rw-r--r--   0        0        0     6015 2023-05-09 08:04:58.868929 frogmouth-0.8.0/frogmouth/widgets/navigation.py
--rw-r--r--   0        0        0      298 2023-04-27 14:46:52.804311 frogmouth-0.8.0/frogmouth/widgets/navigation_panes/__init__.py
--rw-r--r--   0        0        0     5740 2023-07-20 08:13:55.753505 frogmouth-0.8.0/frogmouth/widgets/navigation_panes/bookmarks.py
--rw-r--r--   0        0        0     5790 2023-07-20 08:13:55.754227 frogmouth-0.8.0/frogmouth/widgets/navigation_panes/history.py
--rw-r--r--   0        0        0     3071 2023-05-09 08:04:58.869180 frogmouth-0.8.0/frogmouth/widgets/navigation_panes/local_files.py
--rw-r--r--   0        0        0      665 2023-05-03 09:31:33.037312 frogmouth-0.8.0/frogmouth/widgets/navigation_panes/navigation_pane.py
--rw-r--r--   0        0        0     2341 2023-05-09 08:04:58.869286 frogmouth-0.8.0/frogmouth/widgets/navigation_panes/table_of_contents.py
--rw-r--r--   0        0        0    12260 2023-05-18 13:41:34.484532 frogmouth-0.8.0/frogmouth/widgets/omnibox.py
--rw-r--r--   0        0        0    10907 2023-05-30 09:10:09.566549 frogmouth-0.8.0/frogmouth/widgets/viewer.py
--rw-r--r--   0        0        0     1437 2023-07-20 08:13:55.755003 frogmouth-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     4323 1970-01-01 00:00:00.000000 frogmouth-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-04-27 14:46:52.801782 frogmouth-0.9.0/LICENSE
+-rw-r--r--   0        0        0     2752 2023-04-30 07:26:36.700670 frogmouth-0.9.0/README.md
+-rw-r--r--   0        0        0      283 2023-08-07 09:55:07.866860 frogmouth-0.9.0/frogmouth/__init__.py
+-rw-r--r--   0        0        0      112 2023-04-27 14:46:52.802125 frogmouth-0.9.0/frogmouth/__main__.py
+-rw-r--r--   0        0        0       74 2023-04-27 14:46:52.802222 frogmouth-0.9.0/frogmouth/app/__init__.py
+-rw-r--r--   0        0        0     2070 2023-04-30 11:10:42.375933 frogmouth-0.9.0/frogmouth/app/app.py
+-rw-r--r--   0        0        0      395 2023-04-27 14:46:52.802403 frogmouth-0.9.0/frogmouth/data/__init__.py
+-rw-r--r--   0        0        0     1639 2023-04-27 14:46:52.802497 frogmouth-0.9.0/frogmouth/data/bookmarks.py
+-rw-r--r--   0        0        0     2270 2023-05-09 08:04:58.867587 frogmouth-0.9.0/frogmouth/data/config.py
+-rw-r--r--   0        0        0      582 2023-04-27 14:46:52.802650 frogmouth-0.9.0/frogmouth/data/data_directory.py
+-rw-r--r--   0        0        0     1370 2023-04-27 14:46:52.802714 frogmouth-0.9.0/frogmouth/data/history.py
+-rw-r--r--   0        0        0      354 2023-04-27 14:46:52.802828 frogmouth-0.9.0/frogmouth/dialogs/__init__.py
+-rw-r--r--   0        0        0      565 2023-04-28 13:52:42.406602 frogmouth-0.9.0/frogmouth/dialogs/error.py
+-rw-r--r--   0        0        0     4658 2023-05-30 09:10:09.565607 frogmouth-0.9.0/frogmouth/dialogs/help_dialog.py
+-rw-r--r--   0        0        0      269 2023-04-27 14:55:30.387330 frogmouth-0.9.0/frogmouth/dialogs/information.py
+-rw-r--r--   0        0        0     2544 2023-05-09 08:04:58.868437 frogmouth-0.9.0/frogmouth/dialogs/input_dialog.py
+-rw-r--r--   0        0        0     2168 2023-04-29 20:35:07.295162 frogmouth-0.9.0/frogmouth/dialogs/text_dialog.py
+-rw-r--r--   0        0        0     3602 2023-05-03 09:31:33.036152 frogmouth-0.9.0/frogmouth/dialogs/yes_no_dialog.py
+-rw-r--r--   0        0        0       83 2023-04-27 14:46:52.803485 frogmouth-0.9.0/frogmouth/screens/__init__.py
+-rw-r--r--   0        0        0    20103 2023-05-30 09:10:09.565826 frogmouth-0.9.0/frogmouth/screens/main.py
+-rw-r--r--   0        0        0      402 2023-05-18 13:41:34.484301 frogmouth-0.9.0/frogmouth/utility/__init__.py
+-rw-r--r--   0        0        0      894 2023-04-28 13:00:47.734733 frogmouth-0.9.0/frogmouth/utility/advertising.py
+-rw-r--r--   0        0        0     5373 2023-05-30 09:10:09.565984 frogmouth-0.9.0/frogmouth/utility/forge.py
+-rw-r--r--   0        0        0     1206 2023-05-09 08:04:58.868785 frogmouth-0.9.0/frogmouth/utility/type_tests.py
+-rw-r--r--   0        0        0      184 2023-04-27 14:46:52.804110 frogmouth-0.9.0/frogmouth/widgets/__init__.py
+-rw-r--r--   0        0        0     6015 2023-05-09 08:04:58.868929 frogmouth-0.9.0/frogmouth/widgets/navigation.py
+-rw-r--r--   0        0        0      298 2023-04-27 14:46:52.804311 frogmouth-0.9.0/frogmouth/widgets/navigation_panes/__init__.py
+-rw-r--r--   0        0        0     5740 2023-07-20 08:13:55.753505 frogmouth-0.9.0/frogmouth/widgets/navigation_panes/bookmarks.py
+-rw-r--r--   0        0        0     5790 2023-07-20 08:13:55.754227 frogmouth-0.9.0/frogmouth/widgets/navigation_panes/history.py
+-rw-r--r--   0        0        0     3071 2023-05-09 08:04:58.869180 frogmouth-0.9.0/frogmouth/widgets/navigation_panes/local_files.py
+-rw-r--r--   0        0        0      665 2023-05-03 09:31:33.037312 frogmouth-0.9.0/frogmouth/widgets/navigation_panes/navigation_pane.py
+-rw-r--r--   0        0        0     2341 2023-05-09 08:04:58.869286 frogmouth-0.9.0/frogmouth/widgets/navigation_panes/table_of_contents.py
+-rw-r--r--   0        0        0    12260 2023-05-18 13:41:34.484532 frogmouth-0.9.0/frogmouth/widgets/omnibox.py
+-rw-r--r--   0        0        0    10655 2023-08-07 09:55:07.867988 frogmouth-0.9.0/frogmouth/widgets/viewer.py
+-rw-r--r--   0        0        0     1437 2023-08-07 09:55:07.868790 frogmouth-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     4327 1970-01-01 00:00:00.000000 frogmouth-0.9.0/PKG-INFO
```

### Comparing `frogmouth-0.8.0/LICENSE` & `frogmouth-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `frogmouth-0.8.0/README.md` & `frogmouth-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `frogmouth-0.8.0/frogmouth/app/app.py` & `frogmouth-0.9.0/frogmouth/app/app.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.8.0/frogmouth/data/bookmarks.py` & `frogmouth-0.9.0/frogmouth/data/bookmarks.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.8.0/frogmouth/data/config.py` & `frogmouth-0.9.0/frogmouth/data/config.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.8.0/frogmouth/data/data_directory.py` & `frogmouth-0.9.0/frogmouth/data/data_directory.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.8.0/frogmouth/data/history.py` & `frogmouth-0.9.0/frogmouth/data/history.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.8.0/frogmouth/dialogs/error.py` & `frogmouth-0.9.0/frogmouth/dialogs/error.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.8.0/frogmouth/dialogs/help_dialog.py` & `frogmouth-0.9.0/frogmouth/dialogs/help_dialog.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.8.0/frogmouth/dialogs/input_dialog.py` & `frogmouth-0.9.0/frogmouth/dialogs/input_dialog.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.8.0/frogmouth/dialogs/text_dialog.py` & `frogmouth-0.9.0/frogmouth/dialogs/text_dialog.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.8.0/frogmouth/dialogs/yes_no_dialog.py` & `frogmouth-0.9.0/frogmouth/dialogs/yes_no_dialog.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.8.0/frogmouth/screens/main.py` & `frogmouth-0.9.0/frogmouth/screens/main.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.8.0/frogmouth/utility/advertising.py` & `frogmouth-0.9.0/frogmouth/utility/advertising.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.8.0/frogmouth/utility/forge.py` & `frogmouth-0.9.0/frogmouth/utility/forge.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.8.0/frogmouth/utility/type_tests.py` & `frogmouth-0.9.0/frogmouth/utility/type_tests.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.8.0/frogmouth/widgets/navigation.py` & `frogmouth-0.9.0/frogmouth/widgets/navigation.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.8.0/frogmouth/widgets/navigation_panes/bookmarks.py` & `frogmouth-0.9.0/frogmouth/widgets/navigation_panes/bookmarks.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.8.0/frogmouth/widgets/navigation_panes/history.py` & `frogmouth-0.9.0/frogmouth/widgets/navigation_panes/history.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.8.0/frogmouth/widgets/navigation_panes/local_files.py` & `frogmouth-0.9.0/frogmouth/widgets/navigation_panes/local_files.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.8.0/frogmouth/widgets/navigation_panes/navigation_pane.py` & `frogmouth-0.9.0/frogmouth/widgets/navigation_panes/navigation_pane.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.8.0/frogmouth/widgets/navigation_panes/table_of_contents.py` & `frogmouth-0.9.0/frogmouth/widgets/navigation_panes/table_of_contents.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.8.0/frogmouth/widgets/omnibox.py` & `frogmouth-0.9.0/frogmouth/widgets/omnibox.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.8.0/frogmouth/widgets/viewer.py` & `frogmouth-0.9.0/frogmouth/widgets/viewer.py`

 * *Files 4% similar despite different names*

```diff
@@ -184,27 +184,25 @@
     async def _local_load(self, location: Path, remember: bool = True) -> None:
         """Load a Markdown document from a local file.
 
         Args:
             location: The location to load from.
             remember: Should we remember the location in th ehistory?
         """
-        # At the moment Textual's Markdown widget's load method captures
-        # *all* exceptions and just returns a true/false. It would be
-        # better to get an exception here and be able to properly report
-        # the problem. Alas, right now, we can't.
-        if await self.document.load(location):
-            self._post_load(location, remember)
-        else:
+        try:
+            await self.document.load(location)
+        except OSError as error:
             self.app.push_screen(
                 ErrorDialog(
                     "Error loading local document",
-                    f"{location}\n\nThere was an error loading the document.",
+                    f"{location}\n\n{error}.",
                 )
             )
+        else:
+            self._post_load(location, remember)
 
     @work(exclusive=True)
     async def _remote_load(self, location: URL, remember: bool = True) -> None:
         """Load a Markdown document from a URL.
 
         Args:
             location: The location to load from.
```

### Comparing `frogmouth-0.8.0/pyproject.toml` & `frogmouth-0.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "frogmouth"
 homepage = "https://github.com/Textualize/frogmouth"
-version = "0.8.0"
+version = "0.9.0"
 description = "A Markdown document viewer for the terminal"
 authors = ["Dave Pearson <dave@textualize.io>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "frogmouth"}]
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -24,22 +24,22 @@
     "Programming Language :: Python :: 3.9",
     "Topic :: Software Development :: Documentation",
     "Topic :: Text Processing :: Markup :: Markdown",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-textual = {version = ">=0.30.0"}
+textual = {version = "^0.32"}
 typing-extensions = "^4.5.0"
 httpx = "^0.24.1"
 xdg = "^6.0.0"
 
 
 [tool.poetry.group.dev.dependencies]
-textual-dev = "*"
+textual-dev = "^1.1"
 mypy = "^1.1.1"
 pylint = "^2.17.1"
 pre-commit = "^3.2.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `frogmouth-0.8.0/PKG-INFO` & `frogmouth-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frogmouth
-Version: 0.8.0
+Version: 0.9.0
 Summary: A Markdown document viewer for the terminal
 Home-page: https://github.com/Textualize/frogmouth
 License: MIT
 Author: Dave Pearson
 Author-email: dave@textualize.io
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -26,15 +26,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Text Processing :: Markup :: Markdown
 Requires-Dist: httpx (>=0.24.1,<0.25.0)
-Requires-Dist: textual (>=0.30.0)
+Requires-Dist: textual (>=0.32,<0.33)
 Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
 Requires-Dist: xdg (>=6.0.0,<7.0.0)
 Description-Content-Type: text/markdown
 
 
 <p align="center">
   <img src="https://user-images.githubusercontent.com/554369/234892488-856f9da7-7b82-4429-ac35-0d0545bf0d24.png"  width="300" align="center"/>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: frogmouth Version: 0.8.0 Summary: A Markdown
+Metadata-Version: 2.1 Name: frogmouth Version: 0.9.0 Summary: A Markdown
 document viewer for the terminal Home-page: https://github.com/Textualize/
 frogmouth License: MIT Author: Dave Pearson Author-email: dave@textualize.io
 Requires-Python: >=3.8,<4.0 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop Classifier: Intended
 Audience :: Information Technology Classifier: Intended Audience :: Other
 Audience Classifier: License :: OSI Approved :: MIT License Classifier:
@@ -13,16 +13,16 @@
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Topic :: Software
 Development :: Documentation Classifier: Topic :: Text Processing :: Markup ::
 Markdown Requires-Dist: httpx (>=0.24.1,<0.25.0) Requires-Dist: textual
-(>=0.30.0) Requires-Dist: typing-extensions (>=4.5.0,<5.0.0) Requires-Dist: xdg
-(>=6.0.0,<7.0.0) Description-Content-Type: text/markdown
+(>=0.32,<0.33) Requires-Dist: typing-extensions (>=4.5.0,<5.0.0) Requires-Dist:
+xdg (>=6.0.0,<7.0.0) Description-Content-Type: text/markdown
 [https://user-images.githubusercontent.com/554369/234892488-856f9da7-7b82-4429-
                             ac35-0d0545bf0d24.png]
 [![Discord](https://img.shields.io/discord/1026214085173461072)](https://
 discord.gg/Enf6Z3qhVr) # Frogmouth Frogmouth is a Markdown viewer / browser for
 your terminal, built with [Textual](https://github.com/Textualize/textual).
 Frogmouth can open `*.md` files locally or via a URL. There is a familiar
 browser-like navigation stack, history, bookmarks, and table of contents.
```

