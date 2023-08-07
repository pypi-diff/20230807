# Comparing `tmp/tldr_man-1.3.0.tar.gz` & `tmp/tldr_man-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tldr_man-1.3.0.tar", max compression
+gzip compressed data, was "tldr_man-1.3.1.tar", max compression
```

## Comparing `tldr_man-1.3.0.tar` & `tldr_man-1.3.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11357 2022-07-17 04:30:22.662713 tldr_man-1.3.0/LICENSE
--rw-r--r--   0        0        0     3448 2023-06-16 06:22:32.619707 tldr_man-1.3.0/README.md
--rwxr-xr-x   0        0        0      953 2023-07-26 23:52:09.973286 tldr_man-1.3.0/generate_completions.sh
--rw-r--r--   0        0        0     1615 2023-07-26 23:49:13.826183 tldr_man-1.3.0/pyproject.toml
--rw-r--r--   0        0        0       28 2022-07-29 03:20:39.631247 tldr_man-1.3.0/src/tldr_man/__init__.py
--rw-r--r--   0        0        0       37 2022-07-29 03:10:10.456815 tldr_man-1.3.0/src/tldr_man/__main__.py
--rw-r--r--   0        0        0     3329 2023-07-23 05:50:52.182165 tldr_man-1.3.0/src/tldr_man/languages.py
--rwxr-xr-x   0        0        0     6028 2023-07-01 00:18:58.750251 tldr_man-1.3.0/src/tldr_man/main.py
--rw-r--r--   0        0        0    11909 2023-07-26 23:51:52.449555 tldr_man-1.3.0/src/tldr_man/pages.py
--rw-r--r--   0        0        0     1614 2023-06-16 00:35:28.327932 tldr_man-1.3.0/src/tldr_man/platforms.py
--rw-r--r--   0        0        0     1792 2023-07-23 05:50:52.180370 tldr_man-1.3.0/src/tldr_man/shell_completion.py
--rw-r--r--   0        0        0     1359 2023-06-16 04:55:12.255927 tldr_man-1.3.0/src/tldr_man/util.py
--rw-r--r--   0        0        0     6291 2023-07-26 23:53:11.514605 tldr_man-1.3.0/tldr-man.1
--rw-r--r--   0        0        0     5138 1970-01-01 00:00:00.000000 tldr_man-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-07-17 04:30:22.662713 tldr_man-1.3.1/LICENSE
+-rw-r--r--   0        0        0     3448 2023-06-16 06:22:32.619707 tldr_man-1.3.1/README.md
+-rwxr-xr-x   0        0        0     1513 2023-07-28 02:04:52.843477 tldr_man-1.3.1/generate_completions.sh
+-rw-r--r--   0        0        0     1529 2023-08-07 21:12:05.194747 tldr_man-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0       28 2022-07-29 03:20:39.631247 tldr_man-1.3.1/src/tldr_man/__init__.py
+-rw-r--r--   0        0        0       37 2022-07-29 03:10:10.456815 tldr_man-1.3.1/src/tldr_man/__main__.py
+-rw-r--r--   0        0        0     3329 2023-07-23 05:50:52.182165 tldr_man-1.3.1/src/tldr_man/languages.py
+-rwxr-xr-x   0        0        0     6087 2023-08-07 20:54:34.237332 tldr_man-1.3.1/src/tldr_man/main.py
+-rw-r--r--   0        0        0    11902 2023-08-07 21:10:53.116237 tldr_man-1.3.1/src/tldr_man/pages.py
+-rw-r--r--   0        0        0     1614 2023-06-16 00:35:28.327932 tldr_man-1.3.1/src/tldr_man/platforms.py
+-rw-r--r--   0        0        0     2135 2023-08-07 21:04:17.513718 tldr_man-1.3.1/src/tldr_man/shell_completion.py
+-rw-r--r--   0        0        0     1359 2023-06-16 04:55:12.255927 tldr_man-1.3.1/src/tldr_man/util.py
+-rw-r--r--   0        0        0     6277 2023-08-07 21:12:09.223953 tldr_man-1.3.1/tldr-man.1
+-rw-r--r--   0        0        0     5055 1970-01-01 00:00:00.000000 tldr_man-1.3.1/PKG-INFO
```

### Comparing `tldr_man-1.3.0/LICENSE` & `tldr_man-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tldr_man-1.3.0/README.md` & `tldr_man-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `tldr_man-1.3.0/pyproject.toml` & `tldr_man-1.3.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 [tool.poetry]
 name = "tldr-man"
-version = "1.3.0"
+version = "1.3.1"
 description = "Command-line TLDR client that displays tldr-pages as manpages"
 license = 'Apache-2.0'
 readme = "README.md"
 authors = ["Olivia Kinnear <contact@superatomic.dev>"]
 homepage = 'https://tldr-man.superatomic.dev/'
-repository = 'https://github.com/superatomic/tldr-man-client'
-documentation = 'https://github.com/superatomic/tldr-man-client#readme'
+repository = 'https://github.com/superatomic/tldr-man'
+documentation = 'https://github.com/superatomic/tldr-man#readme'
+urls = {'Bug Tracker' = 'https://github.com/superatomic/tldr-man/issues'}
 keywords = ['tldr', 'tldr-pages', 'man', 'manpage', 'tldr-client']
 classifiers = [
     'Development Status :: 5 - Production/Stable',
     'Environment :: Console',
     'Intended Audience :: Developers',
     'Intended Audience :: End Users/Desktop',
     'Intended Audience :: System Administrators',
@@ -25,18 +26,14 @@
     'Topic :: Documentation',
     'Topic :: Software Development :: Documentation',
     'Topic :: Text Processing :: Markup :: Markdown',
     'Topic :: Utilities',
 ]
 include = ["generate_completions.sh", "tldr-man.1"]
 
-[tool.poetry.urls]
-"Bug Tracker" = "https://github.com/superatomic/tldr-man-client/issues"
-"Say Thanks!" = "https://saythanks.io/to/superatomic"
-
 [tool.poetry.dependencies]
 python = "^3.10.4"
 click = "^8.1.3"
 click-help-colors = "^0.9.1"
 requests = "^2.28.1"
 
 [build-system]
```

### Comparing `tldr_man-1.3.0/src/tldr_man/languages.py` & `tldr_man-1.3.1/src/tldr_man/languages.py`

 * *Files identical despite different names*

### Comparing `tldr_man-1.3.0/src/tldr_man/main.py` & `tldr_man-1.3.1/src/tldr_man/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,35 +16,38 @@
 
 """
 tldr-man: Command-line TLDR client that displays tldr-pages as manpages.
 
 Depends on pandoc (and man!). Install `pandoc` from https://pandoc.org/installing.html.
 
 Run `tldr --help` for more information,
-or visit the project repository at https://github.com/superatomic/tldr-man-client.
+or visit the project repository at https://github.com/superatomic/tldr-man.
 """
 
 __author__ = "Olivia Kinnear <contact@superatomic.dev>"
 
 from pathlib import Path
 from contextlib import suppress
 from os import remove
 from functools import wraps
 
 import click
 from click import Context, command, argument, option, version_option, help_option, pass_context
 from click_help_colors import HelpColorsCommand
 
 from tldr_man import pages
-from tldr_man.shell_completion import page_shell_complete, language_shell_complete
+from tldr_man.shell_completion import page_shell_complete, language_shell_complete, patch_bash_completion
 from tldr_man.languages import get_locales
 from tldr_man.platforms import get_page_sections, TLDR_PLATFORMS
 from tldr_man.util import unique, mkstemp_path
 
 
+patch_bash_completion()  # See issue #10
+
+
 def standalone_subcommand(func):
     """Function decorator to reduce boilerplate code at the start and end of all subcommand callback functions."""
     @wraps(func)
     def wrapper(ctx: Context, _param, value):
         if not value or ctx.resilient_parsing:
             return
```

### Comparing `tldr_man-1.3.0/src/tldr_man/pages.py` & `tldr_man-1.3.1/src/tldr_man/pages.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 ZIP_ARCHIVE_URL = "https://tldr.sh/assets/tldr.zip"
 
 MANPAGE_SECTION = '1'
 
 MANPAGE_HEADER = f"""
 % {{name}}({MANPAGE_SECTION}) {{name}}
 %
-% tldr-man-client
+% tldr-man
 
 # NAME
 {{name}} - {{desc}}
 
 # DESCRIPTION
 {{info}}
```

### Comparing `tldr_man-1.3.0/src/tldr_man/platforms.py` & `tldr_man-1.3.1/src/tldr_man/platforms.py`

 * *Files identical despite different names*

### Comparing `tldr_man-1.3.0/src/tldr_man/shell_completion.py` & `tldr_man-1.3.1/src/tldr_man/shell_completion.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Rich shell completions for the client."""
 
 from click import Context, Parameter
-from click.shell_completion import CompletionItem
+from click.shell_completion import CompletionItem, BashComplete
 
 from tldr_man.pages import CACHE_DIR, get_dir_search_order
 from tldr_man.languages import get_locales, all_language_codes
 from tldr_man.platforms import get_page_sections
 
 
 def page_shell_complete(ctx: Context, param: Parameter, incomplete: str) -> list[CompletionItem]:
@@ -40,7 +40,16 @@
     ]
 
 
 def language_shell_complete(_ctx: Context, _param: Parameter, _incomplete: str) -> list[CompletionItem]:
     if not CACHE_DIR.exists():
         return []
     return [CompletionItem(code) for code in all_language_codes()]
+
+
+def patch_bash_completion():
+    """
+    Patches click Bash shell completion generation to not raise an error on generating for Bash versions older than 4.4.
+
+    Fixes <https://github.com/superatomic/tldr-man/issues/10>, <https://github.com/pallets/click/issues/2574>.
+    """
+    BashComplete._check_version = lambda _: None
```

### Comparing `tldr_man-1.3.0/src/tldr_man/util.py` & `tldr_man-1.3.1/src/tldr_man/util.py`

 * *Files identical despite different names*

### Comparing `tldr_man-1.3.0/tldr-man.1` & `tldr_man-1.3.1/tldr-man.1`

 * *Files 2% similar despite different names*

```diff
@@ -242,28 +242,28 @@
 .RS
 set \-gxa MANPATH (tldr \-\-manpath)
 .RE
 .fi
 .SH "HOMEPAGE"
 .PP
 This software is available at
-.UR https://github.com/superatomic/tldr-man-client
+.UR https://github.com/superatomic/tldr-man
 .UE ,
 and can be found on PyPI at
 .UR https://pypi.org/project/tldr-man
 .UE .
 .SH "REPORTING BUGS"
 .PP
 Please report bugs and feature requests in the issue tracker at
-.UR https://github.com/superatomic/tldr-man-client
+.UR https://github.com/superatomic/tldr-man
 .UE .
 Please do your best to provide a reproducible test case for bugs.
 .SH "COPYRIGHT"
 Copyright 2023 Olivia Kinnear
 .br
 Licensed under the Apache License, Version 2.0
 .SH "SEE ALSO"
 .BR man (1),
 .BR pandoc (1),
 .BR man\-pages (7)
 .SH "VERSION"
-1.3.0
+1.3.1
```

### Comparing `tldr_man-1.3.0/PKG-INFO` & `tldr_man-1.3.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tldr-man
-Version: 1.3.0
+Version: 1.3.1
 Summary: Command-line TLDR client that displays tldr-pages as manpages
 Home-page: https://tldr-man.superatomic.dev/
 License: Apache-2.0
 Keywords: tldr,tldr-pages,man,manpage,tldr-client
 Author: Olivia Kinnear
 Author-email: contact@superatomic.dev
 Requires-Python: >=3.10.4,<4.0.0
@@ -26,18 +26,17 @@
 Classifier: Topic :: Documentation
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Text Processing :: Markup :: Markdown
 Classifier: Topic :: Utilities
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: click-help-colors (>=0.9.1,<0.10.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
-Project-URL: Bug Tracker, https://github.com/superatomic/tldr-man-client/issues
-Project-URL: Documentation, https://github.com/superatomic/tldr-man-client#readme
-Project-URL: Repository, https://github.com/superatomic/tldr-man-client
-Project-URL: Say Thanks!, https://saythanks.io/to/superatomic
+Project-URL: Bug Tracker, https://github.com/superatomic/tldr-man/issues
+Project-URL: Documentation, https://github.com/superatomic/tldr-man#readme
+Project-URL: Repository, https://github.com/superatomic/tldr-man
 Description-Content-Type: text/markdown
 
 <div>
     <h1 align="center">tldr-man</h1>
     <h5 align="center">A tldr-pages client that works just like <code>man</code></h5>
 </div>
```

