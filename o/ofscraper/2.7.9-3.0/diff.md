# Comparing `tmp/ofscraper-2.7.9.tar.gz` & `tmp/ofscraper-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofscraper-2.7.9.tar", max compression
+gzip compressed data, was "ofscraper-3.0.tar", max compression
```

## Comparing `ofscraper-2.7.9.tar` & `ofscraper-3.0.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0     1067 2023-08-01 20:28:12.644499 ofscraper-2.7.9/LICENSE
--rw-r--r--   0        0        0     2859 2023-08-01 20:28:12.644499 ofscraper-2.7.9/README.md
--rw-r--r--   0        0        0      607 2023-08-01 20:28:12.652500 ofscraper-2.7.9/ofscraper/__init__.py
--rw-r--r--   0        0        0     1016 2023-08-01 20:28:12.652500 ofscraper-2.7.9/ofscraper/__version__.py
--rw-r--r--   0        0        0      999 2023-08-01 20:28:12.652500 ofscraper-2.7.9/ofscraper/__version__.pye
--rw-r--r--   0        0        0        1 2023-08-01 20:28:12.652500 ofscraper-2.7.9/ofscraper/api/__init__.py
--rw-r--r--   0        0        0     8591 2023-08-01 20:28:12.652500 ofscraper-2.7.9/ofscraper/api/archive.py
--rw-r--r--   0        0        0     9690 2023-08-01 20:28:12.652500 ofscraper-2.7.9/ofscraper/api/highlights.py
--rw-r--r--   0        0        0     1060 2023-08-01 20:28:12.652500 ofscraper-2.7.9/ofscraper/api/init.py
--rw-r--r--   0        0        0     7357 2023-08-01 20:28:12.652500 ofscraper-2.7.9/ofscraper/api/labels.py
--rw-r--r--   0        0        0     3246 2023-08-01 20:28:12.652500 ofscraper-2.7.9/ofscraper/api/me.py
--rw-r--r--   0        0        0     9415 2023-08-01 20:28:12.652500 ofscraper-2.7.9/ofscraper/api/messages.py
--rw-r--r--   0        0        0     9499 2023-08-01 20:28:12.652500 ofscraper-2.7.9/ofscraper/api/paid.py
--rw-r--r--   0        0        0     5645 2023-08-01 20:28:12.652500 ofscraper-2.7.9/ofscraper/api/pinned.py
--rw-r--r--   0        0        0     4393 2023-08-01 20:28:12.652500 ofscraper-2.7.9/ofscraper/api/profile.py
--rw-r--r--   0        0        0     3294 2023-08-01 20:28:12.652500 ofscraper-2.7.9/ofscraper/api/subscriptions.py
--rw-r--r--   0        0        0     9141 2023-08-01 20:28:12.656500 ofscraper-2.7.9/ofscraper/api/timeline.py
--rw-r--r--   0        0        0        0 2023-08-01 20:28:12.656500 ofscraper-2.7.9/ofscraper/classes/__init__.py
--rw-r--r--   0        0        0      804 2023-08-01 20:28:12.656500 ofscraper-2.7.9/ofscraper/classes/labels.py
--rw-r--r--   0        0        0     8491 2023-08-01 20:28:12.656500 ofscraper-2.7.9/ofscraper/classes/media.py
--rw-r--r--   0        0        0     7278 2023-08-01 20:28:12.656500 ofscraper-2.7.9/ofscraper/classes/placeholder.py
--rw-r--r--   0        0        0     3737 2023-08-01 20:28:12.656500 ofscraper-2.7.9/ofscraper/classes/posts.py
--rw-r--r--   0        0        0     4656 2023-08-01 20:28:12.656500 ofscraper-2.7.9/ofscraper/classes/sessionbuilder.py
--rw-r--r--   0        0        0    29810 2023-08-01 20:28:12.656500 ofscraper-2.7.9/ofscraper/classes/table.py
--rw-r--r--   0        0        0    14593 2023-08-01 20:28:12.656500 ofscraper-2.7.9/ofscraper/commands/check.py
--rw-r--r--   0        0        0     5353 2023-08-01 20:28:12.656500 ofscraper-2.7.9/ofscraper/commands/manual.py
--rwxr-xr-x   0        0        0    14111 2023-08-01 20:28:12.656500 ofscraper-2.7.9/ofscraper/commands/scraper.py
--rw-r--r--   0        0        0     6936 2023-08-01 20:28:12.656500 ofscraper-2.7.9/ofscraper/constants.py
--rw-r--r--   0        0        0        1 2023-08-01 20:28:12.656500 ofscraper-2.7.9/ofscraper/db/__init__.py
--rw-r--r--   0        0        0    10059 2023-08-01 20:28:12.656500 ofscraper-2.7.9/ofscraper/db/operations.py
--rw-r--r--   0        0        0     3576 2023-08-01 20:28:12.656500 ofscraper-2.7.9/ofscraper/db/queries.py
--rw-r--r--   0        0        0        1 2023-08-01 20:28:12.656500 ofscraper-2.7.9/ofscraper/interaction/__init__.py
--rw-r--r--   0        0        0     4891 2023-08-01 20:28:12.656500 ofscraper-2.7.9/ofscraper/interaction/like.py
--rw-r--r--   0        0        0      730 2023-08-01 20:28:12.656500 ofscraper-2.7.9/ofscraper/prompts/keybindings.py
--rw-r--r--   0        0        0     5794 2023-08-01 20:28:12.656500 ofscraper-2.7.9/ofscraper/prompts/promptConvert.py
--rw-r--r--   0        0        0     6695 2023-08-01 20:28:12.656500 ofscraper-2.7.9/ofscraper/prompts/prompt_strings.py
--rw-r--r--   0        0        0     7834 2023-08-01 20:28:12.656500 ofscraper-2.7.9/ofscraper/prompts/prompt_validators.py
--rw-r--r--   0        0        0    29433 2023-08-01 20:28:12.656500 ofscraper-2.7.9/ofscraper/prompts/prompts.py
--rw-r--r--   0        0        0     1583 2023-08-01 20:28:12.656500 ofscraper-2.7.9/ofscraper/start.py
--rw-r--r--   0        0        0        1 2023-08-01 20:28:12.656500 ofscraper-2.7.9/ofscraper/utils/__init__.py
--rw-r--r--   0        0        0    12404 2023-08-01 20:28:12.656500 ofscraper-2.7.9/ofscraper/utils/args.py
--rw-r--r--   0        0        0    10197 2023-08-01 20:28:12.656500 ofscraper-2.7.9/ofscraper/utils/auth.py
--rw-r--r--   0        0        0     8977 2023-08-01 20:28:12.656500 ofscraper-2.7.9/ofscraper/utils/binaries.py
--rw-r--r--   0        0        0    13782 2023-08-01 20:28:12.656500 ofscraper-2.7.9/ofscraper/utils/config.py
--rw-r--r--   0        0        0      257 2023-08-01 20:28:12.656500 ofscraper-2.7.9/ofscraper/utils/console.py
--rw-r--r--   0        0        0     1080 2023-08-01 20:28:12.656500 ofscraper-2.7.9/ofscraper/utils/dates.py
--rw-r--r--   0        0        0    28038 2023-08-01 20:28:12.656500 ofscraper-2.7.9/ofscraper/utils/download.py
--rw-r--r--   0        0        0      609 2023-08-01 20:28:12.656500 ofscraper-2.7.9/ofscraper/utils/encoding.py
--rw-r--r--   0        0        0     2865 2023-08-01 20:28:12.660500 ofscraper-2.7.9/ofscraper/utils/exit.py
--rw-r--r--   0        0        0     5564 2023-08-01 20:28:12.660500 ofscraper-2.7.9/ofscraper/utils/filters.py
--rw-r--r--   0        0        0     7367 2023-08-01 20:28:12.660500 ofscraper-2.7.9/ofscraper/utils/logger.py
--rw-r--r--   0        0        0    10686 2023-08-01 20:28:12.660500 ofscraper-2.7.9/ofscraper/utils/of.py
--rw-r--r--   0        0        0     6994 2023-08-01 20:28:12.660500 ofscraper-2.7.9/ofscraper/utils/paths.py
--rw-r--r--   0        0        0     4263 2023-08-01 20:28:12.660500 ofscraper-2.7.9/ofscraper/utils/profiles.py
--rw-r--r--   0        0        0      399 2023-08-01 20:28:12.660500 ofscraper-2.7.9/ofscraper/utils/semaphoreDelayed.py
--rw-r--r--   0        0        0     1211 2023-08-01 20:28:12.660500 ofscraper-2.7.9/ofscraper/utils/separate.py
--rw-r--r--   0        0        0      554 2023-08-01 20:28:12.660500 ofscraper-2.7.9/ofscraper/utils/stdout.py
--rw-r--r--   0        0        0     5638 2023-08-01 20:28:12.660500 ofscraper-2.7.9/ofscraper/utils/userselector.py
--rw-r--r--   0        0        0     1967 2023-08-01 20:28:54.189112 ofscraper-2.7.9/pyproject.toml
--rw-r--r--   0        0        0     4594 1970-01-01 00:00:00.000000 ofscraper-2.7.9/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-08-07 01:25:44.388761 ofscraper-3.0/LICENSE
+-rw-r--r--   0        0        0     2863 2023-08-07 01:25:44.388761 ofscraper-3.0/README.md
+-rwxr-xr-x   0        0        0      254 2023-08-07 01:25:44.396762 ofscraper-3.0/ofscraper/__main__.py
+-rw-r--r--   0        0        0     1016 2023-08-07 01:25:44.396762 ofscraper-3.0/ofscraper/__version__.py
+-rw-r--r--   0        0        0      999 2023-08-07 01:25:44.396762 ofscraper-3.0/ofscraper/__version__.pye
+-rw-r--r--   0        0        0     8736 2023-08-07 01:25:44.396762 ofscraper-3.0/ofscraper/api/archive.py
+-rw-r--r--   0        0        0     9895 2023-08-07 01:25:44.396762 ofscraper-3.0/ofscraper/api/highlights.py
+-rw-r--r--   0        0        0     1029 2023-08-07 01:25:44.396762 ofscraper-3.0/ofscraper/api/init.py
+-rw-r--r--   0        0        0     7568 2023-08-07 01:25:44.396762 ofscraper-3.0/ofscraper/api/labels.py
+-rw-r--r--   0        0        0     2946 2023-08-07 01:25:44.396762 ofscraper-3.0/ofscraper/api/me.py
+-rw-r--r--   0        0        0     9518 2023-08-07 01:25:44.396762 ofscraper-3.0/ofscraper/api/messages.py
+-rw-r--r--   0        0        0     9687 2023-08-07 01:25:44.396762 ofscraper-3.0/ofscraper/api/paid.py
+-rw-r--r--   0        0        0     5730 2023-08-07 01:25:44.396762 ofscraper-3.0/ofscraper/api/pinned.py
+-rw-r--r--   0        0        0     4497 2023-08-07 01:25:44.396762 ofscraper-3.0/ofscraper/api/profile.py
+-rw-r--r--   0        0        0     3384 2023-08-07 01:25:44.396762 ofscraper-3.0/ofscraper/api/subscriptions.py
+-rw-r--r--   0        0        0     9312 2023-08-07 01:25:44.396762 ofscraper-3.0/ofscraper/api/timeline.py
+-rw-r--r--   0        0        0      804 2023-08-07 01:25:44.396762 ofscraper-3.0/ofscraper/classes/labels.py
+-rw-r--r--   0        0        0     8728 2023-08-07 01:25:44.396762 ofscraper-3.0/ofscraper/classes/media.py
+-rw-r--r--   0        0        0     1795 2023-08-07 01:25:44.396762 ofscraper-3.0/ofscraper/classes/multiprocessprogress.py
+-rw-r--r--   0        0        0     8068 2023-08-07 01:25:44.396762 ofscraper-3.0/ofscraper/classes/placeholder.py
+-rw-r--r--   0        0        0     3734 2023-08-07 01:25:44.396762 ofscraper-3.0/ofscraper/classes/posts.py
+-rw-r--r--   0        0        0     4849 2023-08-07 01:25:44.396762 ofscraper-3.0/ofscraper/classes/sessionbuilder.py
+-rw-r--r--   0        0        0    29784 2023-08-07 01:25:44.396762 ofscraper-3.0/ofscraper/classes/table.py
+-rw-r--r--   0        0        0    14816 2023-08-07 01:25:44.396762 ofscraper-3.0/ofscraper/commands/check.py
+-rw-r--r--   0        0        0     5347 2023-08-07 01:25:44.396762 ofscraper-3.0/ofscraper/commands/manual.py
+-rwxr-xr-x   0        0        0    15354 2023-08-07 01:25:44.396762 ofscraper-3.0/ofscraper/commands/scraper.py
+-rw-r--r--   0        0        0     7244 2023-08-07 01:25:44.396762 ofscraper-3.0/ofscraper/constants.py
+-rw-r--r--   0        0        0        1 2023-08-07 01:25:44.400762 ofscraper-3.0/ofscraper/db/__init__.py
+-rw-r--r--   0        0        0    10129 2023-08-07 01:25:44.400762 ofscraper-3.0/ofscraper/db/operations.py
+-rw-r--r--   0        0        0     3576 2023-08-07 01:25:44.400762 ofscraper-3.0/ofscraper/db/queries.py
+-rw-r--r--   0        0        0        1 2023-08-07 01:25:44.400762 ofscraper-3.0/ofscraper/interaction/__init__.py
+-rw-r--r--   0        0        0     4851 2023-08-07 01:25:44.400762 ofscraper-3.0/ofscraper/interaction/like.py
+-rw-r--r--   0        0        0      773 2023-08-07 01:25:44.400762 ofscraper-3.0/ofscraper/prompts/keybindings.py
+-rw-r--r--   0        0        0     6241 2023-08-07 01:25:44.400762 ofscraper-3.0/ofscraper/prompts/promptConvert.py
+-rw-r--r--   0        0        0     7227 2023-08-07 01:25:44.400762 ofscraper-3.0/ofscraper/prompts/prompt_strings.py
+-rw-r--r--   0        0        0     7848 2023-08-07 01:25:44.400762 ofscraper-3.0/ofscraper/prompts/prompt_validators.py
+-rw-r--r--   0        0        0    30797 2023-08-07 01:25:44.400762 ofscraper-3.0/ofscraper/prompts/prompts.py
+-rw-r--r--   0        0        0     3430 2023-08-07 01:25:44.400762 ofscraper-3.0/ofscraper/start.py
+-rw-r--r--   0        0        0        1 2023-08-07 01:25:44.400762 ofscraper-3.0/ofscraper/utils/__init__.py
+-rw-r--r--   0        0        0    14071 2023-08-07 01:25:44.400762 ofscraper-3.0/ofscraper/utils/args.py
+-rw-r--r--   0        0        0    10511 2023-08-07 01:25:44.400762 ofscraper-3.0/ofscraper/utils/auth.py
+-rw-r--r--   0        0        0     8977 2023-08-07 01:25:44.400762 ofscraper-3.0/ofscraper/utils/binaries.py
+-rw-r--r--   0        0        0    14736 2023-08-07 01:25:44.400762 ofscraper-3.0/ofscraper/utils/config.py
+-rw-r--r--   0        0        0      395 2023-08-07 01:25:44.400762 ofscraper-3.0/ofscraper/utils/console.py
+-rw-r--r--   0        0        0     1080 2023-08-07 01:25:44.400762 ofscraper-3.0/ofscraper/utils/dates.py
+-rw-r--r--   0        0        0    41374 2023-08-07 01:25:44.400762 ofscraper-3.0/ofscraper/utils/download.py
+-rw-r--r--   0        0        0      609 2023-08-07 01:25:44.400762 ofscraper-3.0/ofscraper/utils/encoding.py
+-rw-r--r--   0        0        0     3386 2023-08-07 01:25:44.400762 ofscraper-3.0/ofscraper/utils/exit.py
+-rw-r--r--   0        0        0     5665 2023-08-07 01:25:44.400762 ofscraper-3.0/ofscraper/utils/filters.py
+-rw-r--r--   0        0        0    11133 2023-08-07 01:25:44.400762 ofscraper-3.0/ofscraper/utils/logger.py
+-rw-r--r--   0        0        0      189 2023-08-07 01:25:44.400762 ofscraper-3.0/ofscraper/utils/misc.py
+-rw-r--r--   0        0        0    10913 2023-08-07 01:25:44.400762 ofscraper-3.0/ofscraper/utils/of.py
+-rw-r--r--   0        0        0     7251 2023-08-07 01:25:44.400762 ofscraper-3.0/ofscraper/utils/paths.py
+-rw-r--r--   0        0        0     4221 2023-08-07 01:25:44.400762 ofscraper-3.0/ofscraper/utils/profiles.py
+-rw-r--r--   0        0        0      399 2023-08-07 01:25:44.400762 ofscraper-3.0/ofscraper/utils/semaphoreDelayed.py
+-rw-r--r--   0        0        0     1215 2023-08-07 01:25:44.400762 ofscraper-3.0/ofscraper/utils/separate.py
+-rw-r--r--   0        0        0      893 2023-08-07 01:25:44.400762 ofscraper-3.0/ofscraper/utils/stdout.py
+-rw-r--r--   0        0        0     5773 2023-08-07 01:25:44.400762 ofscraper-3.0/ofscraper/utils/userselector.py
+-rw-r--r--   0        0        0     2071 2023-08-07 01:26:23.509405 ofscraper-3.0/pyproject.toml
+-rw-r--r--   0        0        0     4718 1970-01-01 00:00:00.000000 ofscraper-3.0/PKG-INFO
```

### Comparing `ofscraper-2.7.9/LICENSE` & `ofscraper-3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.9/README.md` & `ofscraper-3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,17 @@
   command-line program to download media, and to process other batch operations such as liking and unliking posts.
     
 
 ![CopyQ nsUBdI](https://user-images.githubusercontent.com/67020411/227816586-fb685959-cd3f-45af-adea-14773b7154f9.png)
 
 # Issues
 Open a issue in this repo, or you can mention your issue in the discord
-https://discord.gg/DV3aBeMu
+https://discord.gg/wN7uxEVHRK
+
+
     
 # Feature Requests
 
 https://ofscraper.clearflask.com/feedback
     
 Or the discord
```

### Comparing `ofscraper-2.7.9/ofscraper/__init__.py` & `ofscraper-3.0/ofscraper/utils/encoding.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,10 +4,12 @@
   _____/ ____\______ ________________    ____   ___________ 
  /  _ \   __\/  ___// ___\_  __ \__  \  /  _ \_/ __ \_  __ \
 (  <_> )  |  \___ \\  \___|  | \// __ \(  <_> )  ___/|  | \/
  \____/|__| /____  >\___  >__|  (____  /\____/ \___  >__|   
                  \/     \/           \/            \/         
 """
 
-from .__version__ import __title__, __description__, __url__
-from .__version__ import __author__, __author_email__, __license__
-from .__version__ import __copyright__
+
+def encode_utf_16(string):
+    encoded_string = string.encode('utf-16', 'surrogatepass')
+    decoded_string = encoded_string.decode('utf-16')
+    return decoded_string
```

### Comparing `ofscraper-2.7.9/ofscraper/__version__.py` & `ofscraper-3.0/ofscraper/__version__.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,12 +14,12 @@
 __url__ = 'https://github.com/datawhores/OF-Scraper'
 __license__ = 'GNU General Public License v3 or later (GPLv3+)'
 __copyright__ = 'Copyright 2023'
 
 try:
       
       from dunamai import Version,Pattern
-      __version__ = Version.from_git(pattern="(?P<base>\d+\.\d+\.\d+|\d+\.\d+)").serialize(format="{base}+{branch}.{commit}",metadata=False)
+      __version__ = Version.from_git(pattern="(?P<base>\d+\.\d+\.\w+|\d+\.\w+)").serialize(format="{base}+{branch}.{commit}",metadata=False)
 except:
       import pkg_resources
       __version__= pkg_resources.get_distribution('ofscraper').version
```

### Comparing `ofscraper-2.7.9/ofscraper/__version__.pye` & `ofscraper-3.0/ofscraper/__version__.pye`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.9/ofscraper/api/archive.py` & `ofscraper-3.0/ofscraper/api/archive.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 """
 import time
 import asyncio
 from ofscraper.utils.semaphoreDelayed import semaphoreDelayed
 import logging
 import contextvars
 import math
-from tenacity import retry,stop_after_attempt,wait_random
+from diskcache import Cache
+from tenacity import retry,stop_after_attempt,wait_random,retry_if_not_exception_type
 from rich.progress import Progress
 from rich.progress import (
     Progress,
     TextColumn,
     SpinnerColumn
 )
 from rich.panel import Panel
@@ -28,26 +29,26 @@
 from ..utils import auth
 from ..utils.paths import getcachepath
 import ofscraper.utils.console as console
 import ofscraper.utils.args as args_
 import ofscraper.classes.sessionbuilder as sessionbuilder
 
 
-from diskcache import Cache
-cache = Cache(getcachepath())
-log=logging.getLogger(__package__)
+
+log=logging.getLogger("shared")
 attempt = contextvars.ContextVar("attempt")
 
 sem = semaphoreDelayed(constants.AlT_SEM)
-@retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
+@retry(retry=retry_if_not_exception_type(KeyboardInterrupt),stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
 async def scrape_archived_posts(c, model_id,progress, timestamp=None,required_ids=None) -> list:
     global tasks
     global sem
     posts=None
     attempt.set(attempt.get(0) + 1)
+    
     if timestamp and   (float(timestamp)>(args_.getargs().before or arrow.now()).float_timestamp):
         return []
     if timestamp:
         timestamp=str(timestamp)
         ep = constants.archivedNextEP
         url = ep.format(model_id, timestamp)
     else:
@@ -86,33 +87,35 @@
                             attempt.set(0)
                             tasks.append(asyncio.create_task(scrape_archived_posts(c, model_id,progress,timestamp=posts[-1]['postedAtPrecise'],required_ids=set())))
 
                         elif len(required_ids)>0:
                             attempt.set(0)
                             tasks.append(asyncio.create_task(scrape_archived_posts(c, model_id,progress,timestamp=posts[-1]['postedAtPrecise'],required_ids=required_ids)))
             else:
-                    log.debug(f"[bold]archived request status code:[/bold]{r.status}")
+                    log.debug(f"[bold]archived response status code:[/bold]{r.status}")
                     log.debug(f"[bold]archived response:[/bold] {await r.text_()}")
                     log.debug(f"[bold]archived headers:[/bold] {r.headers}")
                     progress.remove_task(task)
                     r.raise_for_status()
     return posts
 
 async def get_archived_post(model_id): 
+    cache = Cache(getcachepath())
     overall_progress=Progress(SpinnerColumn(style=Style(color="blue")),TextColumn("Getting archived media...\n{task.description}"))
     job_progress=Progress("{task.description}")
     progress_group = Group(
     overall_progress,
     Panel(Group(job_progress)))
     global tasks
     tasks=[]
     min_posts=50
     responseArray=[]
     page_count=0
-    with Live(progress_group, refresh_per_second=5,console=console.shared_console): 
+
+    with Live(progress_group, refresh_per_second=5,console=console.get_shared_console()): 
         
         async with sessionbuilder.sessionBuilder()  as c: 
 
             oldarchived=cache.get(f"archived_{model_id}",default=[])
             log.trace("oldarchive {posts}".format(posts=  "\n\n".join(list(map(lambda x:f"oldarchive: {str(x)}",oldarchived)))))
             oldtimeset=set(map(lambda x:x.get("id"),oldarchived))
             log.debug(f"[bold]Archived Cache[/bold] {len(oldarchived)} found")
@@ -121,15 +124,15 @@
             filteredArray=list(filter(lambda x:x>=(args_.getargs().after or arrow.get(0)).float_timestamp,postedAtArray))
             
         
         
             if len(filteredArray)>min_posts:
                 splitArrays=[filteredArray[i:i+min_posts] for i in range(0, len(filteredArray), min_posts)]
                 #use the previous split for timesamp
-                tasks.append(asyncio.create_task(scrape_archived_posts(c,model_id,job_progress,required_ids=set(splitArrays[0]),timestamp= splitArrays[0][0]-20000)))
+                tasks.append(asyncio.create_task(scrape_archived_posts(c,model_id,job_progress,required_ids=set(splitArrays[0]),timestamp= args_.getargs().after.float_timestamp if args_.getargs().after else None)))
                 [tasks.append(asyncio.create_task(scrape_archived_posts(c,model_id,job_progress,required_ids=set(splitArrays[i]),timestamp=splitArrays[i-1][-1])))
                 for i in range(1,len(splitArrays)-1)]
                 # keeping grabbing until nothign left
                 tasks.append(asyncio.create_task(scrape_archived_posts(c,model_id,job_progress,timestamp=splitArrays[-2][-1])))
             else:
                 tasks.append(asyncio.create_task(scrape_archived_posts(c,model_id,job_progress,timestamp=args_.getargs().after.float_timestamp if args_.getargs().after else None)))
```

### Comparing `ofscraper-2.7.9/ofscraper/api/highlights.py` & `ofscraper-3.0/ofscraper/api/highlights.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
  \____/|__| /____  >\___  >__|  (____  /\____/ \___  >__|   
                  \/     \/           \/            \/         
 """
 
 import asyncio
 import logging
 import contextvars
-from tenacity import retry,stop_after_attempt,wait_random
+from tenacity import retry,stop_after_attempt,wait_random,retry_if_not_exception_type
 from rich.progress import Progress
 from rich.progress import (
     Progress,
     TextColumn,
     SpinnerColumn
 )
 from rich.panel import Panel
@@ -25,30 +25,30 @@
 import ofscraper.constants as c
 import ofscraper.constants as constants
 import ofscraper.utils.auth as auth
 from ofscraper.utils.semaphoreDelayed import semaphoreDelayed
 import ofscraper.utils.console as console
 import ofscraper.classes.sessionbuilder as sessionbuilder
 
-log=logging.getLogger(__package__)
+log=logging.getLogger("shared")
 sem = semaphoreDelayed(1)
 attempt = contextvars.ContextVar("attempt")
 
 async def get_stories_post(model_id):
     overall_progress=Progress(SpinnerColumn(style=Style(color="blue")),TextColumn("Getting story media...\n{task.description}"))
     job_progress=Progress("{task.description}")
     progress_group = Group(
     overall_progress,
     Panel(Group(job_progress)))
 
     output=[]
     page_count=0
     global tasks
     tasks=[]
-    with Live(progress_group, refresh_per_second=5,console=console.shared_console):
+    with Live(progress_group, refresh_per_second=5,console=console.get_shared_console()):
             async with sessionbuilder.sessionBuilder() as c:
                 tasks.append(asyncio.create_task(scrape_stories(c,model_id,job_progress)))
                 page_task = overall_progress.add_task(f' Pages Progress: {page_count}',visible=True) 
                 while len(tasks)!=0:
                     for coro in asyncio.as_completed(tasks):
                         result=await coro or []
                         page_count=page_count+1
@@ -57,15 +57,15 @@
                     tasks=list(filter(lambda x:x.done()==False,tasks))
                 overall_progress.remove_task(page_task)  
     log.trace("stories raw unduped {posts}".format(posts=  "\n\n".join(list(map(lambda x:f"undupedinfo stories: {str(x)}",output)))))
     log.debug(f"[bold]stories+highlight Count without Dupes[/bold] {len(output)} found")
     return output
 
 
-@retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
+@retry(retry=retry_if_not_exception_type(KeyboardInterrupt),stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
 async def scrape_stories( c,user_id,job_progress) -> list:
     global sem
     global tasks
     attempt.set(attempt.get(0) + 1)
     stories=None
     await sem.acquire()
     task=job_progress.add_task(f"Attempt {attempt.get()}/{constants.NUM_TRIES} : user id -> {user_id}",visible=True)
@@ -74,15 +74,15 @@
         if r.ok:
             attempt.set(0)
             stories =await r.json_()
             log.debug(f"stories: -> found stories ids {list(map(lambda x:x.get('id'),stories))}") 
             log.trace("stories: -> stories raw {posts}".format(posts=  "\n\n".join(list(map(lambda x:f"scrapeinfo stories: {str(x)}",stories)))))
             job_progress.remove_task(task)
         else:
-            log.debug(f"[bold]stories request status code:[/bold]{r.status}")
+            log.debug(f"[bold]stories response status code:[/bold]{r.status}")
             log.debug(f"[bold]stories response:[/bold] {await r.text_()}")
             log.debug(f"[bold]stories headers:[/bold] {r.headers}")
             r.raise_for_status()
         return   stories 
         
     
   
@@ -103,15 +103,15 @@
         Panel(Group(job_progress)))
 
         output=[]
 
         page_count=0
         global tasks
         tasks=[]    
-        with Live(progress_group, refresh_per_second=5,console=console.shared_console):
+        with Live(progress_group, refresh_per_second=5,console=console.get_shared_console()):
         
                 tasks.append(asyncio.create_task(scrape_highlight_list(c,model_id,job_progress)))
                 page_task = overall_progress.add_task(f' Pages Progress: {page_count}',visible=True) 
                 while len(tasks)!=0:
                     for coro in asyncio.as_completed(tasks):
                         result=await coro or []
                         page_count=page_count+1
@@ -121,15 +121,15 @@
                 
           
         overall_progress=Progress(SpinnerColumn(style=Style(color="blue")),TextColumn("Getting highlight...\n{task.description}"))
         job_progress=Progress("{task.description}")
         progress_group = Group(
         overall_progress,
         Panel(Group(job_progress)))
-        with Live(progress_group, refresh_per_second=5,console=console.shared_console):
+        with Live(progress_group, refresh_per_second=5,console=console.get_shared_console()):
 
 
             output2=[]
             page_count=0
             tasks=[]
                 
             [tasks.append(asyncio.create_task(scrape_highlights(c,i,job_progress))) for i in output]
@@ -143,15 +143,15 @@
                 tasks=list(filter(lambda x:x.done()==False,tasks))
 
     # log.trace("stories+highlight raw unduped {posts}".format(posts=  "\n\n".join(list(map(lambda x:f"undupedinfo stories+highlight: {str(x)}",output)))))
     # log.debug(f"[bold]stories+highlight Count without Dupes[/bold] {len(output)} found")
     return output2
 
 
-@retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
+@retry(retry=retry_if_not_exception_type(KeyboardInterrupt),stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
 async def scrape_highlight_list( c,user_id,job_progress,offset=0) -> list:
     global sem
     global tasks
     attempt.set(attempt.get(0) + 1)
     await sem.acquire()
     task=job_progress.add_task(f"Attempt {attempt.get()}/{constants.NUM_TRIES}",visible=True)
     async with c.requests(url=constants.highlightsWithStoriesEP.format(user_id,offset))() as r:
@@ -160,22 +160,22 @@
             attempt.set(0)
             resp_data=(await r.json_())
             log.trace(f"highlights list: -> found highlights list data {resp_data}")
             data=get_highlightList(resp_data)
             log.debug(f"highlights list: -> found list ids {data}")
     
         else:
-            log.debug(f"[bold]highlight list request status code:[/bold]{r.status}")
+            log.debug(f"[bold]highlight list response status code:[/bold]{r.status}")
             log.debug(f"[bold]highlight list response:[/bold] {await r.text_()}")
             log.debug(f"[bold]highlight list headers:[/bold] {r.headers}")
     return  data
 
 
 
-@retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
+@retry(retry=retry_if_not_exception_type(KeyboardInterrupt),stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
 async def scrape_highlights( c,id,job_progress) -> list:
     global sem
     global tasks
     attempt.set(attempt.get(0) + 1)
     await sem.acquire()
     task=job_progress.add_task(f"Attempt {attempt.get()}/{constants.NUM_TRIES} highlights id -> {id}",visible=True)
     async with c.requests(url=constants.storyEP.format(id))() as r:
@@ -205,35 +205,34 @@
     
 
 
 
 
 
 
-
 def get_individual_highlights(id,c=None):
     return get_individual_stories(id,c)
     # with c.requests(constants.highlightSPECIFIC.format(id))() as r:
     #     if r.ok:
     #         log.trace(f"highlight raw highlight individua; {r.json()}")
     #         return r.json()
     #     else:
-    #         log.debug(f"[bold]highlight request status code:[/bold]{r.status}")
+    #         log.debug(f"[bold]highlight response status code:[/bold]{r.status}")
     #         log.debug(f"[bold]highlightresponse:[/bold] {r.text_()}")
     #         log.debug(f"[bold]highlight headers:[/bold] {r.headers}")
 
 
 
 
 
 
 def get_individual_stories(id,c=None):
     with c.requests(constants.storiesSPECIFIC.format(id))() as r:
         if r.ok:
             log.trace(f"highlight raw highlight individua; {r.json_()}")
             return r.json()
         else:
-            log.debug(f"[bold]highlight request status code:[/bold]{r.status}")
+            log.debug(f"[bold]highlight response status code:[/bold]{r.status}")
             log.debug(f"[bold]highlightresponse:[/bold] {r.text_()}")
             log.debug(f"[bold]highlight headers:[/bold] {r.headers}")
```

### Comparing `ofscraper-2.7.9/ofscraper/api/init.py` & `ofscraper-3.0/ofscraper/api/init.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,28 +10,28 @@
 
 from . import me
 import traceback
 from rich.console import Console
 import ofscraper.utils.stdout as stdout
 import logging
 
-log=logging.getLogger(__package__)
+log=logging.getLogger("shared")
 
 
 console=Console()
-def print_sign_status(headers):
+def print_sign_status():
     with stdout.lowstdout():
-        status=getstatus(headers)
+        status=getstatus()
         if status=="UP":
             print('Status - \033[32mUP\033[0m')
         else:
             print('Status - \033[31mDOWN\033[0m')
 
 
-def getstatus(headers):
+def getstatus():
     try:
-        me.scrape_user(headers)
+        me.scrape_user()
         return "UP"
     except Exception as e:
         log.traceback(e)
         log.traceback(traceback.format_exc())
         return "DOWN"
```

### Comparing `ofscraper-2.7.9/ofscraper/api/labels.py` & `ofscraper-3.0/ofscraper/api/labels.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 (  <_> )  |  \___ \\  \___|  | \// __ \(  <_> )  ___/|  | \/
  \____/|__| /____  >\___  >__|  (____  /\____/ \___  >__|   
                  \/     \/           \/            \/         
 """
 import asyncio
 import logging
 import contextvars
-from tenacity import retry,stop_after_attempt,wait_random
+from tenacity import retry,stop_after_attempt,wait_random,retry_if_not_exception_type
 from rich.progress import Progress
 from rich.progress import (
     Progress,
     TextColumn,
     SpinnerColumn
 )
 from rich.panel import Panel
@@ -23,15 +23,15 @@
 from rich.style import Style
 import ofscraper.constants as constants
 import ofscraper.utils.console as console
 from ofscraper.utils.semaphoreDelayed import semaphoreDelayed
 import ofscraper.classes.sessionbuilder as sessionbuilder
 
 
-log=logging.getLogger(__package__)
+log=logging.getLogger("shared")
 attempt = contextvars.ContextVar("attempt")
 
 sem = semaphoreDelayed(constants.MAX_SEMAPHORE)
 
 async def get_labels(model_id):
     overall_progress=Progress(SpinnerColumn(style=Style(color="blue")),TextColumn("Getting labels...\n{task.description}"))
     job_progress=Progress("{task.description}")
@@ -39,15 +39,15 @@
     overall_progress,
     Panel(Group(job_progress)))
 
     output=[]
     global tasks
     tasks=[]
     page_count=0
-    with Live(progress_group, refresh_per_second=5,console=console.shared_console):
+    with Live(progress_group, refresh_per_second=5,console=console.get_shared_console()):
        async with sessionbuilder.sessionBuilder() as c: 
 
             tasks.append(asyncio.create_task(scrape_labels(c,model_id,job_progress)))
 
             page_task = overall_progress.add_task(f' Pages Progress: {page_count}',visible=True) 
             while len(tasks)!=0:
                 for coro in asyncio.as_completed(tasks):
@@ -57,15 +57,15 @@
                     output.extend(result)
                 tasks=list(filter(lambda x:x.done()==False,tasks))
             overall_progress.remove_task(page_task)  
     log.trace("post label names unduped {posts}".format(posts= "\n\n".join(map(lambda x:f" label name unduped:{x}",output))))
     log.debug(f"[bold]Labels name count without Dupes[/bold] {len(output)} found")
     return output    
 
-@retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
+@retry(retry=retry_if_not_exception_type(KeyboardInterrupt),stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
 async def scrape_labels(c,model_id,job_progress,offset=0):
     global sem
     global tasks
     labels = None
     attempt.set(attempt.get(0) + 1)
     
     await sem.acquire()
@@ -83,33 +83,33 @@
             if data.get("hasMore"):
                 offset = data.get("nextOffset")
                 tasks.append(asyncio.create_task(scrape_labels(c, model_id,job_progress,offset=offset)))
             job_progress.remove_task(task)
             return data.get("list")
 
         else:
-            log.debug(f"[bold]labels request status code:[/bold]{r.status}")
+            log.debug(f"[bold]labels response status code:[/bold]{r.status}")
             log.debug(f"[bold]labels response:[/bold] {await r.text_()}")
             log.debug(f"[bold]labels headers:[/bold] {r.headers}")
             job_progress.remove_task(task)
             r.raise_for_status()
 
 
 async def get_labelled_posts(labels, username):
-    overall_progress=Progress(SpinnerColumn(style=Style(color="blue")),TextColumn("Getting labels...\n{task.description}"))
+    overall_progress=Progress(SpinnerColumn(style=Style(color="blue")),TextColumn("Getting posts from labels...\n{task.description}"))
     job_progress=Progress("{task.description}")
     progress_group = Group(
     overall_progress,
     Panel(Group(job_progress)))
 
     output={}
     global tasks
     tasks=[]
     page_count=0
-    with Live(progress_group, refresh_per_second=5,console=console.shared_console):
+    with Live(progress_group, refresh_per_second=5,console=console.get_shared_console()):
         async with sessionbuilder.sessionBuilder() as c:
 
             [tasks.append(asyncio.create_task(scrape_labelled_posts(c,label,username,job_progress)))
                 for label in labels]
 
             page_task = overall_progress.add_task(f' Pages Progress: {page_count}',visible=True) 
             while len(tasks)!=0:
@@ -129,36 +129,39 @@
                 tasks=list(filter(lambda x:x.done()==False,tasks))
             overall_progress.remove_task(page_task)  
     log.trace("post label joined {posts}".format(posts=  "\n\n".join(list(map(lambda x:f"label post joined: {str(x)}",list(output.values()))))))
     log.debug(f"[bold]Labels count without Dupes[/bold] {len(output)} found")
 
     return list(output.values())
 
-@retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
+@retry(retry=retry_if_not_exception_type(KeyboardInterrupt),stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
 async def scrape_labelled_posts(c,label,model_id,job_progress,offset=0):
     global sem
     global tasks
     posts = None
     attempt.set(attempt.get(0) + 1)
+    await sem.acquire()
     task=job_progress.add_task(f"Attempt {attempt.get()}/{constants.NUM_TRIES} : offset -> {offset} + label -> {label.get('name')}",visible=True)
     async with c.requests(url=constants.labelledPostsEP.format(model_id, offset, label['id']))() as r:
+        sem.release()
+        
         if r.ok:
             data=await r.json_()
             attempt.set(0)
             posts=list(filter(lambda x:isinstance(x,list),data.values()))[0]
             log.debug(f"offset:{offset} -> labelled posts found {len(posts)}")
             log.debug(f"offset:{offset} -> hasMore value in json {data.get('hasMore','undefined') }")
             log.trace("{offset} -> {posts}".format(offset=offset,posts= "\n\n".join(list(map(lambda x:f"scrapeinfo label {str(x)}",posts)))))  
             if data.get("hasMore"):
                 offset += len(posts)
                 tasks.append(asyncio.create_task(scrape_labelled_posts(c, label, model_id,job_progress,offset=offset)))
             job_progress.remove_task(task)
  
         else:
-            log.debug(f"[bold]labelled posts request status code:[/bold]{r.status}")
+            log.debug(f"[bold]labelled posts response status code:[/bold]{r.status}")
             log.debug(f"[bold]labelled posts response:[/bold] {await r.text_()}")
             log.debug(f"[bold]labelled posts headers:[/bold] {r.headers}")
 
             job_progress.remove_task(task)
             r.raise_for_status()
 
     return label, posts
```

### Comparing `ofscraper-2.7.9/ofscraper/api/me.py` & `ofscraper-3.0/ofscraper/api/me.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,74 +6,64 @@
 (  <_> )  |  \___ \\  \___|  | \// __ \(  <_> )  ___/|  | \/
  \____/|__| /____  >\___  >__|  (____  /\____/ \___  >__|   
                  \/     \/           \/            \/         
 """
 
 import logging
 from functools import lru_cache
-import json
 from rich.console import Console
-from tenacity import retry,stop_after_attempt,wait_random
+from tenacity import retry,stop_after_attempt,wait_random,retry_if_not_exception_type
 import ofscraper.constants as constants
 import ofscraper.utils.encoding as encoding
 import ofscraper.utils.stdout as stdout
 import ofscraper.utils.logger as logger
 import ofscraper.constants as constants
 import ofscraper.utils.paths as paths
 import ofscraper.classes.sessionbuilder as sessionbuilder
 
-log=logging.getLogger(__package__)
-console=Console()
+log=logging.getLogger("shared")
 
-from diskcache import Cache
 
-def scrape_user(headers):
+def scrape_user():
     with sessionbuilder.sessionBuilder(backend="httpx") as c:
-        return _scraper_user_helper(c,json.dumps(headers))
+        return _scraper_user_helper(c)
 
 
-@lru_cache(maxsize=None)
-@retry(stop=stop_after_attempt(0),wait=wait_random(min=constants.OF_MAX, max=constants.OF_MAX),reraise=True,after=lambda retry_state:print(f"Trying to login attempt:{retry_state.attempt_number}/{constants.NUM_TRIES}")) 
-def _scraper_user_helper(c,headers):
-    headers = json.loads(headers)
-    cache = Cache(paths.getcachepath())
-    data=cache.get(f"myinfo_{headers['user-id']}",None)
-    if not data:
-            with c.requests(constants.meEP)() as r:
-                if r.ok:
-                    data=r.json_()
-                    cache.set(f"myinfo_{headers['user-id']}",data,constants.HOURLY_EXPIRY)
-                    cache.close()
-                    logger.updateSenstiveDict(data["id"],"userid")
-                    logger.updateSenstiveDict(data["username"],"username")
-                    logger.updateSenstiveDict(data["name"],"name")
-                else:
-                    log.debug(f"[bold]archived request status code:[/bold]{r.status}")
-                    log.debug(f"[bold]archived response:[/bold] {r.text_()}")
-                    log.debug(f"[bold]archived headers:[/bold] {r.headers}")
-                    r.raise_for_status()
-                
-           
+@retry(retry=retry_if_not_exception_type(KeyboardInterrupt),stop=stop_after_attempt(0),wait=wait_random(min=constants.OF_MAX, max=constants.OF_MAX),reraise=True,after=lambda retry_state:print(f"Trying to login attempt:{retry_state.attempt_number}/{constants.NUM_TRIES}")) 
+def _scraper_user_helper(c):
+    data=None
+    with c.requests(constants.meEP)() as r:
+        if r.ok:
+            data=r.json_()
+            logger.updateSenstiveDict(data["id"],"userid")
+            logger.updateSenstiveDict(data["username"],"username")
+            logger.updateSenstiveDict(data["name"],"name")
+        else:
+            log.debug(f"[bold]user request response status code:[/bold]{r.status}")
+            log.debug(f"[bold]user request response:[/bold] {r.text_()}")
+            log.debug(f"[bold]user request headers:[/bold] {r.headers}")
+            r.raise_for_status()
+                      
     return data
 
 def parse_user(profile):
     name = encoding.encode_utf_16(profile['name'])
     username = profile['username']
 
     return (name, username)
 
 
 def print_user(name, username):
     with stdout.lowstdout():
-        console.print(f'Welcome, {name} | {username}')
-@retry(stop=stop_after_attempt(constants.MAX_SEMAPHORE),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
+        Console().print(f'Welcome, {name} | {username}')
+@retry(retry=retry_if_not_exception_type(KeyboardInterrupt),stop=stop_after_attempt(constants.MAX_SEMAPHORE),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
 def parse_subscriber_count():
     with sessionbuilder.sessionBuilder(backend="httpx") as c:
         with c.requests(constants.subscribeCountEP)() as r:
             if r.ok:
                 data=r.json_()
                 return data["subscriptions"]["all"]
             else:
-                log.debug(f"[bold]archived request status code:[/bold]{r.status}")
-                log.debug(f"[bold]archived response:[/bold] {r.text_()}")
-                log.debug(f"[bold]archived headers:[/bold] {r.headers}")
+                log.debug(f"[bold]subscriber count response status code:[/bold]{r.status}")
+                log.debug(f"[bold]subscriber countresponse:[/bold] {r.text_()}")
+                log.debug(f"[bold]subscriber count headers:[/bold] {r.headers}")
```

### Comparing `ofscraper-2.7.9/ofscraper/api/messages.py` & `ofscraper-3.0/ofscraper/api/messages.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,48 +7,46 @@
  \____/|__| /____  >\___  >__|  (____  /\____/ \___  >__|   
                  \/     \/           \/            \/         
 """
 import asyncio
 import logging
 import ssl
 import contextvars
-from tenacity import retry,stop_after_attempt,wait_random
+from tenacity import retry,stop_after_attempt,wait_random,retry_if_not_exception_type
 from rich.progress import Progress
 from rich.progress import (
     Progress,
     TextColumn,
     SpinnerColumn
 )
 from rich.panel import Panel
 from rich.console import Group
 from rich.live import Live
 from rich.style import Style
 import arrow
-import arrow
+from diskcache import Cache
 import ofscraper.constants as constants
 import ofscraper.utils.auth as auth
 import ofscraper.utils.paths as paths
 from ..utils import auth
 import ofscraper.utils.console as console
 from ofscraper.utils.semaphoreDelayed import semaphoreDelayed
 import ofscraper.utils.args as args_
 import ofscraper.classes.sessionbuilder as sessionbuilder
 
 
-
-from diskcache import Cache
-cache = Cache(paths.getcachepath())
-log=logging.getLogger(__package__)
+log=logging.getLogger("shared")
 attempt = contextvars.ContextVar("attempt")
 
 sem = semaphoreDelayed(constants.MAX_SEMAPHORE)
 
 
 
 async def get_messages(model_id):
+    cache = Cache(paths.getcachepath())
     overall_progress=Progress(SpinnerColumn(style=Style(color="blue"),),TextColumn("Getting Messages...\n{task.description}"))
     job_progress=Progress("{task.description}")
     progress_group = Group(
     overall_progress,
     Panel(Group(job_progress)))
 
     global tasks
@@ -56,15 +54,15 @@
 
 
     tasks=[]
     responseArray=[]
     page_count=0
     #require a min num of posts to be returned
     min_posts=50
-    with Live(progress_group, refresh_per_second=constants.refreshScreen,console=console.shared_console): 
+    with Live(progress_group, refresh_per_second=constants.refreshScreen,console=console.get_shared_console()): 
         async with sessionbuilder.sessionBuilder() as c: 
             oldmessages=cache.get(f"messages_{model_id}",default=[]) if not args_.getargs().no_cache else []
             log.trace("oldamessage {posts}".format(posts=  "\n\n".join(list(map(lambda x:f"oldtimeline: {str(x)}",oldmessages)))))
 
             oldmsgset=set(map(lambda x:x.get("id"),oldmessages))
             log.debug(f"[bold]Messages Cache[/bold] {len(oldmessages)} found")
             oldmessages=list(filter(lambda x:(x.get("createdAt") or x.get("postedAt"))!=None,oldmessages))
@@ -76,14 +74,15 @@
 
         
             
         
             if len(postedAtArray)>min_posts:
                 splitArrays=[postedAtArray[i:i+min_posts] for i in range(0, len(postedAtArray), min_posts)]
                 #use the previous split for message_id
+
                 tasks.append(asyncio.create_task(scrape_messages(c,model_id,job_progress,message_id=None if startdex==0 else splitArrays[0][0] ,required_ids=set(splitArrays[0]))))
                 [tasks.append(asyncio.create_task(scrape_messages(c,model_id,job_progress,required_ids=set(splitArrays[i]),message_id=splitArrays[i-1][-1])))
                 for i in range(1,len(splitArrays)-1)]
                 # keeping grabbing until nothing left
                 tasks.append(asyncio.create_task(scrape_messages(c,model_id,job_progress,message_id=splitArrays[-2][-1])))
             else:
                 tasks.append(asyncio.create_task(scrape_messages(c,model_id,job_progress,message_id=None if startdex==0 else postedAtArray[0])))
@@ -123,15 +122,15 @@
         cache.set(f"messages_{model_id}",[],expire=constants.RESPONSE_EXPIRY)
         cache.set(f"message_check_{model_id}",[],expire=constants.CHECK_EXPIRY)
         cache.close()
         log.debug("Some messages where not retrived resetting cache")
 
     return unduped    
 
-@retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
+@retry(retry=retry_if_not_exception_type(KeyboardInterrupt),stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
 async def scrape_messages(c, model_id, progress,message_id=None,required_ids=None) -> list:
     global sem
     global tasks
     messages=None
     attempt.set(attempt.get(0) + 1)
     ep = constants.messagesNextEP if message_id else constants.messagesEP
     url = ep.format(model_id, message_id)
@@ -169,26 +168,26 @@
 
                         elif len(required_ids)>0:
                             attempt.set(0)
                             tasks.append(asyncio.create_task(scrape_messages(c, model_id,progress,message_id=messages[-1]['id'],required_ids=required_ids)))
                 progress.remove_task(task)
 
             else:
-                log.debug(f"[bold]message request status code:[/bold]{r.status}")
+                log.debug(f"[bold]message response status code:[/bold]{r.status}")
                 log.debug(f"[bold]message response:[/bold] {await r.text_()}")
                 log.debug(f"[bold]message headers:[/bold] {r.headers}")
 
                 progress.remove_task(task)
                 r.raise_for_status()
 
     return messages
 
 def get_individual_post(model_id,postid,c=None):
     with c.requests(url=constants.messageSPECIFIC.format(model_id,postid))() as r:
         if r.ok:
             log.trace(f"message raw individual {r.json()}")
             return r.json()['list'][0]
         else:
-            log.debug(f"[bold]archived request status code:[/bold]{r.status}")
-            log.debug(f"[bold]archived response:[/bold] {r.text_()}")
-            log.debug(f"[bold]archived headers:[/bold] {r.headers}")
+            log.debug(f"[bold]invidual message response status code:[/bold]{r.status}")
+            log.debug(f"[bold]invidual message  response:[/bold] {r.text_()}")
+            log.debug(f"[bold]invidual message  headers:[/bold] {r.headers}")
```

### Comparing `ofscraper-2.7.9/ofscraper/api/paid.py` & `ofscraper-3.0/ofscraper/api/paid.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import contextvars
 from rich.progress import Progress
 from rich.progress import (
     Progress,
     TextColumn,
     SpinnerColumn
 )
-from tenacity import retry,stop_after_attempt,wait_random
+from tenacity import retry,stop_after_attempt,wait_random,retry_if_not_exception_type
 from rich.panel import Panel
 from rich.console import Group
 from rich.live import Live
 from rich.style import Style
 import ofscraper.constants as constants
 from ..utils import auth
 from ..utils.paths import getcachepath
@@ -31,43 +31,44 @@
 from diskcache import Cache
 from ..utils.paths import getcachepath
 from ofscraper.utils.semaphoreDelayed import semaphoreDelayed
 import ofscraper.utils.args as args_ 
 import ofscraper.classes.sessionbuilder as sessionbuilder
 
 
-cache = Cache(getcachepath())
+
 
 paid_content_list_name = 'list'
-log=logging.getLogger(__package__)
+log=logging.getLogger("shared")
 
 sem = semaphoreDelayed(constants.MAX_SEMAPHORE)
 
 attempt = contextvars.ContextVar("attempt")
 
 
 
 
 
 
 
 
 
 async def get_paid_posts(username,model_id):
+    cache = Cache(getcachepath())
     overall_progress=Progress(SpinnerColumn(style=Style(color="blue")),TextColumn("Getting paid media...\n{task.description}"))
     job_progress=Progress("{task.description}")
     progress_group = Group(
     overall_progress,
     Panel(Group(job_progress)))
 
     output=[]
     global tasks
     tasks=[]
     page_count=0
-    with Live(progress_group, refresh_per_second=5,console=console.shared_console):
+    with Live(progress_group, refresh_per_second=5,console=console.get_shared_console()):
         async with sessionbuilder.sessionBuilder() as c:
  
             tasks.append(asyncio.create_task(scrape_paid(c,username,job_progress)))
 
             
             page_task = overall_progress.add_task(f' Pages Progress: {page_count}',visible=True) 
             while len(tasks)!=0:
@@ -83,15 +84,15 @@
     log.trace("paid raw unduped {posts}".format(posts=  "\n\n".join(list(map(lambda x:f"undupedinfo paid: {str(x)}",output)))))
 
     cache.set(f"purchased_check_{model_id}",output,expire=constants.CHECK_EXPIRY)
     cache.close()
     return output
 
 
-@retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
+@retry(retry=retry_if_not_exception_type(KeyboardInterrupt),stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
 async def scrape_paid(c,username,job_progress,offset=0):
     """Takes headers to access onlyfans as an argument and then checks the purchased content
     url to look for any purchased content. If it finds some it will return it as a list."""
     global sem
     global tasks
     media = None
     attempt.set(attempt.get(0) + 1)
@@ -109,38 +110,39 @@
             log.debug(f"offset:{offset} -> found paid content ids {list(map(lambda x:x.get('id'),media))}")
             if  data.get("hasMore"):
                 offset += len(media)
                 tasks.append(asyncio.create_task(scrape_paid(c,username,job_progress,offset=offset)))
             job_progress.remove_task(task)
 
         else:
-            log.debug(f"[bold]paid request status code:[/bold]{r.status}")
+            log.debug(f"[bold]paid response status code:[/bold]{r.status}")
             log.debug(f"[bold]paid response:[/bold] {await r.text_()}")
             log.debug(f"[bold]paid headers:[/bold] {r.headers}")
             job_progress.remove_task(task)
             r.raise_for_status()
     return media
 
 
 
 
 
 async def get_all_paid_posts():
-    overall_progress=Progress(SpinnerColumn(style=Style(color="blue")),TextColumn("Getting paid media...\n{task.description}"))
+    cache = Cache(getcachepath())
+    overall_progress=Progress(SpinnerColumn(style=Style(color="blue")),TextColumn("Getting all paid media...\n{task.description}"))
     job_progress=Progress("{task.description}")
     progress_group = Group(
     overall_progress,
     Panel(Group(job_progress)))
 
     output=[]
     min_posts=100
     global tasks
     tasks=[]
     page_count=0
-    with Live(progress_group, refresh_per_second=5,console=console.shared_console):
+    with Live(progress_group, refresh_per_second=5,console=console.get_shared_console()):
         async with sessionbuilder.sessionBuilder() as c:
             allpaid=cache.get(f"purchased_all",default=[]) if not args_.getargs().no_cache else []
             log.debug(f"[bold]All Paid Cache[/bold] {len(allpaid)} found")
             
         
             if len(allpaid)>min_posts:
                 splitArrays=[i for i in range(0, len(allpaid), min_posts)]
@@ -174,15 +176,15 @@
         unduped.append(post)
     log.debug(f"[bold]Paid Post count[/bold] {len(unduped)} found")
     cache.set(f"purchased_all",list(map(lambda x:x.get("id"),unduped)),expire=constants.RESPONSE_EXPIRY)
     cache.close()
     return unduped
 
 
-@retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
+@retry(retry=retry_if_not_exception_type(KeyboardInterrupt),stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
 async def scrape_all_paid(c,job_progress,offset=0,count=0,required=0):
     """Takes headers to access onlyfans as an argument and then checks the purchased content
     url to look for any purchased content. If it finds some it will return it as a list."""
     global sem
     global tasks
     media = None
     attempt.set(attempt.get(0) + 1)
@@ -215,15 +217,15 @@
                 elif len(count)<len(required):
                     tasks.append(asyncio.create_task(scrape_all_paid(c,job_progress,offset=offset+len(media),required=required,count=count+len(media))))
 
 
             
 
         else:
-            log.debug(f"[bold]paid request status code:[/bold]{r.status}")
+            log.debug(f"[bold]paid response status code:[/bold]{r.status}")
             log.debug(f"[bold]paid response:[/bold] {await r.text_()}")
             log.debug(f"[bold]paid headers:[/bold] {r.headers}")
             job_progress.remove_task(task)
             r.raise_for_status()
     return media
```

### Comparing `ofscraper-2.7.9/ofscraper/api/pinned.py` & `ofscraper-3.0/ofscraper/api/pinned.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 """
 import time
 import asyncio
 from ofscraper.utils.semaphoreDelayed import semaphoreDelayed
 import logging
 import contextvars
 import math
-from tenacity import retry,stop_after_attempt,wait_random
+from tenacity import retry,stop_after_attempt,wait_random,retry_if_not_exception_type
 from rich.progress import Progress
 from rich.progress import (
     Progress,
     TextColumn,
     SpinnerColumn
 )
 from rich.panel import Panel
@@ -27,19 +27,19 @@
 import ofscraper.constants as constants
 from ..utils import auth
 import ofscraper.utils.console as console
 import ofscraper.utils.args as args_
 import ofscraper.classes.sessionbuilder as sessionbuilder
 
 
-log=logging.getLogger(__package__)
+log=logging.getLogger("shared")
 attempt = contextvars.ContextVar("attempt")
 
 sem = semaphoreDelayed(constants.AlT_SEM)
-@retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
+@retry(retry=retry_if_not_exception_type(KeyboardInterrupt),stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
 async def scrape_pinned_posts(c, model_id,progress, timestamp=None) -> list:
     global tasks
     global sem
     posts=None
     attempt.set(attempt.get(0) + 1)
     if timestamp and   (float(timestamp)>(args_.getargs().before or arrow.now()).float_timestamp):
         return []
@@ -71,15 +71,15 @@
                     log.debug(f"{log_id} -> number of pinned post found {len(posts)}")
                     log.debug(f"{log_id} -> first date {posts[0].get('createdAt') or posts[0].get('postedAt')}")
                     log.debug(f"{log_id} -> last date {posts[-1].get('createdAt') or posts[-1].get('postedAt')}")
                     log.debug(f"{log_id} -> found pinned post IDs {list(map(lambda x:x.get('id'),posts))}")
                     log.trace("{log_id} -> pinned raw {posts}".format(log_id=log_id,posts=  "\n\n".join(list(map(lambda x:f"scrapeinfo pinned: {str(x)}",posts)))))
                     tasks.append(asyncio.create_task(scrape_pinned_posts(c, model_id,progress,timestamp=posts[-1]['postedAtPrecise'])))
             else:
-                log.debug(f"[bold]timeline request status code:[/bold]{r.status}")
+                log.debug(f"[bold]timeline response status code:[/bold]{r.status}")
                 log.debug(f"[bold]timeline response:[/bold] {await r.text_()}")
                 log.debug(f"[bold]timeline headers:[/bold] {r.headers}")
                 progress.remove_task(task)
                 r.raise_for_status()
 
         return posts
 
@@ -91,15 +91,15 @@
     Panel(Group(job_progress)))
 
     global tasks
     tasks=[]
     min_posts=50
     responseArray=[]
     page_count=0
-    with Live(progress_group, refresh_per_second=5,console=console.shared_console): 
+    with Live(progress_group, refresh_per_second=5,console=console.get_shared_console()): 
        async with sessionbuilder.sessionBuilder() as c: 
             tasks.append(asyncio.create_task(scrape_pinned_posts(c,model_id,job_progress,timestamp=args_.getargs().after.float_timestamp if args_.getargs().after else None)))
         
 
             page_task = overall_progress.add_task(f' Pages Progress: {page_count}',visible=True)
             while len(tasks)!=0:
                 for coro in asyncio.as_completed(tasks):
```

### Comparing `ofscraper-2.7.9/ofscraper/api/profile.py` & `ofscraper-3.0/ofscraper/api/profile.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,62 +8,62 @@
                  \/     \/           \/            \/         
 """
 import logging
 import contextvars
 
 from typing import Union
 from rich.console import Console
-from tenacity import retry,stop_after_attempt,wait_random
+from tenacity import retry,stop_after_attempt,wait_random,retry_if_not_exception_type
 from ..constants import profileEP,NUM_TRIES,HOURLY_EXPIRY,DAILY_EXPIRY
 from ..utils import auth, encoding
 from xxhash import xxh128
 from diskcache import Cache
 from ..utils.paths import getcachepath
 import ofscraper.constants as constants
 import ofscraper.classes.sessionbuilder as sessionbuilder
 
-cache = Cache(getcachepath())
 
 
-log=logging.getLogger(__package__)
+log=logging.getLogger("shared")
 console=Console()
 attempt = contextvars.ContextVar("attempt")
 
 
 
 
 # can get profile from username or id
 def scrape_profile(username:Union[int, str]) -> dict:
     with sessionbuilder.sessionBuilder(backend="httpx") as c:
         return scrape_profile_helper(c,username)
 
 
   
-@retry(stop=stop_after_attempt(NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
+@retry(retry=retry_if_not_exception_type(KeyboardInterrupt),stop=stop_after_attempt(NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
 def scrape_profile_helper(c,username:Union[int, str]):
+
+    cache = Cache(getcachepath())
     id=cache.get(f"username_{username}",None)
     log.trace(f"username date: {id}")
     if id:
         return id
-    headers = auth.make_headers(auth.read_auth())
     attempt.set(attempt.get(0) + 1)
     log.info(f"Attempt {attempt.get()}/{constants.NUM_TRIES} to get profile {username}")
     with c.requests(profileEP.format(username))() as r:
         if r.ok:
             attempt.set(0)
             cache.set(f"username_{username}",r.json(),int(HOURLY_EXPIRY*2))
             cache.close()
             log.trace(f"username date: {r.json()}")
             return r.json()
         elif r.status==404:
             return {"username":"modeldeleted"}
         else:
-              log.debug(f"[bold]archived request status code:[/bold]{r.status}")
-              log.debug(f"[bold]archived response:[/bold] {r.text_()}")
-              log.debug(f"[bold]archived headers:[/bold] {r.headers}")
+              log.debug(f"[bold]profile response status code:[/bold]{r.status}")
+              log.debug(f"[bold]profile response:[/bold] {r.text_()}")
+              log.debug(f"[bold]profile headers:[/bold] {r.headers}")
               r.raise_for_status()
 
 
 
 
 def parse_profile(profile: dict) -> tuple:
     media = []
@@ -105,23 +105,24 @@
     with sessionbuilder.sessionBuilder(backend="httpx") as c:
         return get_id_helper(c,username)
 
     
         
         
 
-@retry(stop=stop_after_attempt(NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
+@retry(retry=retry_if_not_exception_type(KeyboardInterrupt),stop=stop_after_attempt(NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
 def get_id_helper(c,username):
+    cache = Cache(getcachepath())   
     id=cache.get(f"model_id_{username}",None)
     if id:
         return id
     with c.requests(profileEP.format(username))() as r:
         if r.ok:
             id=r.json()['id']
             cache.set(f"model_id_{username}",id,DAILY_EXPIRY)
             cache.close()
             return id
         else:
-            log.debug(f"[bold]archived request status code:[/bold]{r.status}")
-            log.debug(f"[bold]archived response:[/bold] {r.text_()}")
-            log.debug(f"[bold]archived headers:[/bold] {r.headers}")
+            log.debug(f"[bold]id response status code:[/bold]{r.status}")
+            log.debug(f"[bold]id response:[/bold] {r.text_()}")
+            log.debug(f"[bold]id headers:[/bold] {r.headers}")
             r.raise_for_status()
```

### Comparing `ofscraper-2.7.9/ofscraper/api/subscriptions.py` & `ofscraper-3.0/ofscraper/api/subscriptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,44 +10,44 @@
 
 import asyncio
 from itertools import chain
 import logging
 from rich.console import Console
 import arrow
 console=Console()
-from tenacity import retry,stop_after_attempt,wait_random
+from tenacity import retry,stop_after_attempt,wait_random,retry_if_not_exception_type
 from ..constants import subscriptionsEP,NUM_TRIES
 import ofscraper.constants as constants
-log=logging.getLogger(__package__)
+log=logging.getLogger("shared")
 import ofscraper.classes.sessionbuilder as sessionbuilder
 
 
 async def get_subscriptions(subscribe_count):
     offsets = range(0, subscribe_count, 10)
     async with sessionbuilder.sessionBuilder() as c: 
         tasks = [scrape_subscriptions(c,offset) for offset in offsets]
         subscriptions = await asyncio.gather(*tasks)
         return list(chain.from_iterable(subscriptions))
 
 
 
 
 
-@retry(stop=stop_after_attempt(constants.MAX_SEMAPHORE),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
+@retry(retry=retry_if_not_exception_type(KeyboardInterrupt),stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
 async def scrape_subscriptions(c,offset=0) -> list:
 
         async with c.requests( subscriptionsEP.format(offset))() as r:
             if r.ok:
                 subscriptions = await r.json_()
                 log.debug(f"usernames offset {offset}: usernames retrived -> {list(map(lambda x:x.get('username'),subscriptions))}")      
                 return subscriptions
             else:
-                log.debug(f"[bold]archived request status code:[/bold]{r.status}")
-                log.debug(f"[bold]archived response:[/bold] {await r.text_()}")
-                log.debug(f"[bold]archived headers:[/bold] {r.headers}")
+                log.debug(f"[bold]subscriptions response status code:[/bold]{r.status}")
+                log.debug(f"[bold]subscriptions response:[/bold] {await r.text_()}")
+                log.debug(f"[bold]subscriptions headers:[/bold] {r.headers}")
 
 def parse_subscriptions(subscriptions: list) -> list:
     datenow=arrow.now()
     data = [
         {"name":profile['username']
          ,"id":profile['id'],
          "sub-price":profile.get("currentSubscribePrice",{}),
```

### Comparing `ofscraper-2.7.9/ofscraper/api/timeline.py` & `ofscraper-3.0/ofscraper/api/timeline.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 import time
 import asyncio
 import logging
 import ssl
 import certifi
 import contextvars
 import math
-from tenacity import retry,stop_after_attempt,wait_random
+from diskcache import Cache
+from tenacity import retry,stop_after_attempt,wait_random,retry_if_not_exception_type
 from rich.progress import Progress
 from rich.progress import (
     Progress,
     TextColumn,
     SpinnerColumn
 )
 from rich.panel import Panel
@@ -29,22 +30,19 @@
 from ofscraper.utils.semaphoreDelayed import semaphoreDelayed
 from ..utils import auth
 from ..utils.paths import getcachepath
 import ofscraper.utils.console as console
 import ofscraper.utils.args as args_
 import ofscraper.classes.sessionbuilder as sessionbuilder
 
-
-from diskcache import Cache
-cache = Cache(getcachepath())
-log=logging.getLogger(__package__)
+log=logging.getLogger("shared")
 attempt = contextvars.ContextVar("attempt")
 
 sem = semaphoreDelayed(constants.MAX_SEMAPHORE)
-@retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
+@retry(retry=retry_if_not_exception_type(KeyboardInterrupt),stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
 async def scrape_timeline_posts(c, model_id,progress, timestamp=None,required_ids=None) -> list:
     global tasks
     global sem
     posts=None
     attempt.set(attempt.get(0) + 1)
     if timestamp and   (float(timestamp)>(args_.getargs().before or arrow.now()).float_timestamp):
         return []
@@ -87,55 +85,56 @@
                             attempt.set(0)
                             tasks.append(asyncio.create_task(scrape_timeline_posts(c, model_id,progress,timestamp=posts[-1]['postedAtPrecise'],required_ids=set())))
 
                         elif len(required_ids)>0:
                             attempt.set(0)
                             tasks.append(asyncio.create_task(scrape_timeline_posts(c, model_id,progress,timestamp=posts[-1]['postedAtPrecise'],required_ids=required_ids)))
             else:
-                    log.debug(f"[bold]timeline request status code:[/bold]{r.status}")
+                    log.debug(f"[bold]timeline response status code:[/bold]{r.status}")
                     log.debug(f"[bold]timeline response:[/bold] {await r.text_()}")
                     log.debug(f"[bold]timeline headers:[/bold] {r.headers}")
 
                     progress.remove_task(task)
                     r.raise_for_status()
     return posts
 
 
 
 async def get_timeline_post(model_id): 
+    
     overall_progress=Progress(SpinnerColumn(style=Style(color="blue")),TextColumn("Getting timeline media...\n{task.description}"))
     job_progress=Progress("{task.description}")
     progress_group = Group(
     overall_progress,
     Panel(Group(job_progress)))
 
     global tasks
     tasks=[]
     min_posts=50
     responseArray=[]
     page_count=0
     
-    with Live(progress_group, refresh_per_second=5,console=console.shared_console): 
+    with Live(progress_group, refresh_per_second=5,console=console.get_shared_console()): 
         async with sessionbuilder.sessionBuilder() as c:
-
+            cache = Cache(getcachepath())
             oldtimeline=cache.get(f"timeline_{model_id}",default=[]) if not args_.getargs().no_cache else []
             log.trace("oldtimeline {posts}".format(posts=  "\n\n".join(list(map(lambda x:f"oldtimeline: {str(x)}",oldtimeline)))))
 
             oldtimeset=set(map(lambda x:x.get("id"),oldtimeline))
             log.debug(f"[bold]Timeline Cache[/bold] {len(oldtimeline)} found")
             oldtimeline=list(filter(lambda x:x.get("postedAtPrecise")!=None,oldtimeline))
             postedAtArray=sorted(list(map(lambda x:float(x["postedAtPrecise"]),oldtimeline)))
             filteredArray=list(filter(lambda x:x>=(args_.getargs().after or arrow.get(0)).float_timestamp,postedAtArray))
             
         
         
             if len(filteredArray)>min_posts:
                 splitArrays=[filteredArray[i:i+min_posts] for i in range(0, len(filteredArray), min_posts)]
                 #use the previous split for timesamp
-                tasks.append(asyncio.create_task(scrape_timeline_posts(c,model_id,job_progress,required_ids=set(splitArrays[0]),timestamp= splitArrays[0][0]-20000)))
+                tasks.append(asyncio.create_task(scrape_timeline_posts(c,model_id,job_progress,required_ids=set(splitArrays[0]),timestamp= args_.getargs().after.float_timestamp if args_.getargs().after else None)))
                 [tasks.append(asyncio.create_task(scrape_timeline_posts(c,model_id,job_progress,required_ids=set(splitArrays[i]),timestamp=splitArrays[i-1][-1])))
                 for i in range(1,len(splitArrays)-1)]
                 # keeping grabbing until nothign left
                 tasks.append(asyncio.create_task(scrape_timeline_posts(c,model_id,job_progress,timestamp=splitArrays[-2][-1])))
             else:
                 tasks.append(asyncio.create_task(scrape_timeline_posts(c,model_id,job_progress,timestamp=args_.getargs().after.float_timestamp if args_.getargs().after else None)))
         
@@ -177,12 +176,12 @@
 
 def get_individual_post(id,c=None):
     with c.requests(constants.INDVIDUAL_TIMELINE.format(id))() as r:
         if r.ok:
             log.trace(f"message raw individual {r.json()}")
             return r.json()
         else:
-            log.debug(f"[bold]archived request status code:[/bold]{r.status}")
-            log.debug(f"[bold]archived response:[/bold] {r.text_()}")
-            log.debug(f"[bold]archived headers:[/bold] {r.headers}")
+            log.debug(f"[bold]individual post response status code:[/bold]{r.status}")
+            log.debug(f"[bold]individual post response:[/bold] {r.text_()}")
+            log.debug(f"[bold]individual post headers:[/bold] {r.headers}")
```

### Comparing `ofscraper-2.7.9/ofscraper/classes/labels.py` & `ofscraper-3.0/ofscraper/classes/labels.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.9/ofscraper/classes/media.py` & `ofscraper-3.0/ofscraper/classes/media.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import re
+from bs4 import BeautifulSoup,MarkupResemblesLocatorWarning
 import arrow
-from tenacity import retry,stop_after_attempt,wait_random
+from tenacity import retry,stop_after_attempt,wait_random,retry_if_not_exception_type
 from ..constants import LICENCE_URL
 import ofscraper.utils.args as args_
-import ofscraper.utils.auth as auth
 from mpegdash.parser import MPEGDASHParser
 import ofscraper.constants as constants
 import ofscraper.utils.config as config
-import certifi
-import ssl
 import logging
 import traceback
 import ofscraper.classes.sessionbuilder as sessionbuilder
+#supress warnings
+import warnings
+warnings.filterwarnings("ignore", category=MarkupResemblesLocatorWarning)
 
 
-log=logging.getLogger(__package__)
+log=logging.getLogger("shared")
 class Media():
     def __init__(self, media, count, post):
         self._media = media
         self._count = count
         self._post = post
 
     @property
@@ -124,15 +125,16 @@
 
     @property
     def postid(self):
         return self._post.id
 
     @property
     def text(self):
-        return self._post.text
+        return BeautifulSoup(self._post.text,'html.parser').text
+    
 
     
     @property
     def mpd(self):
         if self.url:
             return None
         return self._media.get("files",{}).get("drm",{}).get("manifest",{}).get("dash")
@@ -160,26 +162,27 @@
         if not self.mpd:
             return None
 
 
 
     @property
     def text_(self):
+
         if self.responsetype_!="Profile":
             text = self.text or self.filename or arrow.get(self.date).format(config.get_date(config.read_config()))
         elif self.responsetype_=="Profile":
             text=f"{arrow.get(self.date).format(config.get_date(config.read_config()))} {self.text or self.filename}"
         if len(text)==0:
             return text
         # this is for removing emojis
         # text=re.sub("[^\x00-\x7F]","",text)
         # this is for removing html tags
-        text = re.sub("<[^>]*>", "", text)
+        # text = re.sub("<[^>]*>", "", text)
         # this for remove random special invalid special characters
-        text = re.sub('[\n<>:"/\|?*]+', '', text)
+        text = re.sub('[\n<>:"/\|?*:;]+', '', text)
         text = re.sub(" +", " ", text)
         text=re.sub(" ",config.get_spacereplacer(config.read_config()),text)
         length = int(config.get_textlength(config.read_config()))
         if length==0 and self._addcount():
                 return f"{text}_{self.count}"
         elif length==0 and not self._addcount():
                 return text
@@ -250,24 +253,24 @@
     def linked(self):
         return None
 
     @property
     def media(self):
         return self._media
     @property
-    @retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True) 
+    @retry(retry=retry_if_not_exception_type(KeyboardInterrupt),stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True) 
     async def parse_mpd(self): 
         if not self.mpd:
             return
         try:
             params={"Policy":self.policy,"Key-Pair-Id":self.keypair,"Signature":self.signature}
             async with sessionbuilder.sessionBuilder() as c:
                 async with c.requests(url=self.mpd,params=params)() as r:
                     if not r.ok:
-                        return None
+                        r.raise_for_status()
                     return MPEGDASHParser.parse(await r.text_())
         except Exception as E:
             log.traceback(traceback.format_exc())
             log.traceback(E)
             raise E
```

### Comparing `ofscraper-2.7.9/ofscraper/classes/placeholder.py` & `ofscraper-3.0/ofscraper/classes/placeholder.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import logging
+import os
 import pathlib
 import ofscraper.utils.paths as paths
 import ofscraper.utils.config as config_
 import ofscraper.utils.profiles as profiles
 import ofscraper.api.me as me
 import arrow
 
 
-log=logging.getLogger(__package__)
+log=logging.getLogger("shared")
 class Placeholders:
     def __init__(self) -> None:
         None
 
     def wrapper(f):
         def wrapper(*args):
             args[0]._variables={}
@@ -42,25 +43,32 @@
         firstletter=username[0].capitalize();self._variables.update({"firstletter":firstletter})
         self._variables.update({"model_id":model_id})
         modelid=model_id;self._variables.update({"modelid":modelid})
 
         log.trace(f"modelid:{model_id}  database placeholders {list(filter(lambda x:x[0] in set(list(self._variables.keys())),list(locals().items())))}")
         if config_.get_allow_code_execution(config_.read_config()):
             formatStr=eval("f'{}'".format(config_.get_metadata(config_.read_config())))
+            
         else:
             formatStr=config_.get_metadata(config_.read_config()).format(       
-                            **self._variables)
+                          **self._variables)
+        data_path=pathlib.Path(formatStr,'user_data.db')
+        data_path=os.path.normpath(data_path )
+        log.trace(f"final database path {data_path}")
+        return pathlib.Path(data_path)
 
-        return pathlib.Path(formatStr,"user_data.db")
 
+  
 
- 
 
     @wrapper
     def getmediadir(self,ele,username,model_id):
+
+        
+        root=pathlib.Path(config_.get_save_location(config_.read_config()))
         self._variables.update({"username":username})
         self._variables.update({"model_id":model_id})
         user_name=username;self._variables.update({"user_name":username})
         modelid=model_id;self._variables.update({"modelid":modelid})
         post_id=ele.postid_;self._variables.update({"post_id":post_id})
         postid=ele.postid_;self._variables.update({"postid":postid})
         media_id=ele.id;self._variables.update({"media_id":media_id})
@@ -86,16 +94,17 @@
         log.trace(f"modelid:{model_id}  mediadir placeholders {list(filter(lambda x:x[0] in set(list(self._variables.keys())),list(locals().items())))}")
         if config_.get_allow_code_execution(config_.read_config()):
             downloadDir=eval("f'{}'".format(config_.get_dirformat(config_.read_config())))
         else:
             
             downloadDir=config_.get_dirformat(config_.read_config())\
             .format(**self._variables)
-            
-        return root /downloadDir  
+        final_path=pathlib.Path(os.path.normpath(root /downloadDir ))
+        log.trace(f"final mediadir path {final_path}")
+        return final_path
     
     
     @wrapper
     def createfilename(self,ele,username,model_id,ext):
         filename=ele.filename_;self._variables.update({"filename":filename})
         file_name=ele.filename_;self._variables.update({"file_name":filename})
         if ele.responsetype_ =="profile":
@@ -131,12 +140,27 @@
         download_type=ele.downloadtype;self._variables.update({"downloadtype":download_type})
 
 
         
 
        
         log.trace(f"modelid:{model_id}  filename placeholders {list(filter(lambda x:x[0] in set(list(self._variables.keys())),list(locals().items())))}")
-      
+        filename=None
         if config_.get_allow_code_execution(config_.read_config()):
-            return eval("f'{}'".format(config_.get_fileformat(config_.read_config())))
+            filename=eval("f'{}'".format(config_.get_fileformat(config_.read_config())))
         else:
-            return config_.get_fileformat(config_.read_config()).format(**self._variables) 
+            filename=config_.get_fileformat(config_.read_config()).format(**self._variables) 
+        log.trace(f"final filename path {filename }")
+        return filename
+        
+        
+
+
+
+# def all_placeholders():
+#       {"user_name","modelid","model_id","username","postid","postid","media_id",
+#        "mediaid","first_letter","firstletter","mediatype","media_type","value","date",
+#        "model_username","modelusername","response_type","responsetype","label","downloadtype","download_type"}
+   
+
+
+
```

### Comparing `ofscraper-2.7.9/ofscraper/classes/posts.py` & `ofscraper-3.0/ofscraper/classes/posts.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 import arrow
 import ofscraper.utils.config as config
 import ofscraper.classes.media as Media
 
-log=logging.getLogger(__package__)
+log=logging.getLogger("shared")
 
 class Post():
     def __init__(self, post, model_id, username, responsetype=None,label=None):
         self._post = post
         self._model_id = int(model_id)
         self._username = username
         self._responsetype_ = responsetype or post.get("responseType")
```

### Comparing `ofscraper-2.7.9/ofscraper/classes/sessionbuilder.py` & `ofscraper-3.0/ofscraper/classes/sessionbuilder.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,28 +15,30 @@
 #  This class allows the user to select which backend aiohttp or httpx they want to use
 #  httpx has better compatiblilty but is slower
 # 
 #####
 
 
 class sessionBuilder:
-    def __init__(self,backend=None, set_header=True,set_sign=True,set_cookies=True):
+    def __init__(self,backend=None, set_header=True,set_sign=True,set_cookies=True,connect_timeout=None,total_timeout=None):
         self._backend=backend or config_.get_backend(config_.read_config())
         self._set_cookies=set_cookies
         self._set_header=set_header
         self._set_sign=set_sign
+        self._connect_timeout=connect_timeout
+        self._total_timeout=None
         
         
      
 
     async def __aenter__(self):
         self._async=True
         if self._backend=="aio":
-            self._session = aiohttp.ClientSession(timeout=aiohttp.ClientTimeout(total=constants.API_REEQUEST_TIMEOUT, connect=None,
-                      sock_connect=None, sock_read=None),connector = aiohttp.TCPConnector(limit=constants.MAX_SEMAPHORE))
+            self._session = aiohttp.ClientSession(timeout=aiohttp.ClientTimeout(total=self._total_timeout, connect=self._connect_timeout,
+                      sock_connect=self._connect_timeout, sock_read=None),connector = aiohttp.TCPConnector(limit=constants.MAX_SEMAPHORE*3))
         
         
         elif self._backend=="httpx":
             self._session= httpx.AsyncClient(http2=True,timeout=None)
     
         return self
     
@@ -57,15 +59,17 @@
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self._session.__exit__(exc_type, exc_val, exc_tb)
    
 
     def _create_headers(self,headers,url):
         headers=headers or {}
-        headers.update(auth.make_headers(auth.read_auth())) if self._set_header else None
+        if self._set_header:
+            new_headers=auth.make_headers(auth.read_auth())
+            headers.update(new_headers)
         headers=self._create_sign(headers,url)
         return headers
     def _create_sign(self,headers,url) : 
             auth.create_sign(url,headers) if self._set_sign else None
             return headers  
       
     def _create_cookies(self):
@@ -73,14 +77,16 @@
 
 
     def requests(self,url=None,method="get",headers=None,cookies=None,json=None,params=None,redirects=True,data=None):
         headers=self._create_headers(headers,url)
         cookies=cookies or self._create_cookies()
         json=json or None
         params=params or None
+        
+
         if self._backend=="aio":
             inner_func=functools.partial(self._session.request,method,url=url,allow_redirects=redirects,params=params,ssl=ssl.create_default_context(cafile=certifi.where()),cookies=cookies,headers=headers,json=json,data=data)
             funct=functools.partial(self._aio_funct_async,inner_func)
 
      
             
         elif self._backend=="httpx" and self._async:
```

### Comparing `ofscraper-2.7.9/ofscraper/classes/table.py` & `ofscraper-3.0/ofscraper/classes/table.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,25 +6,25 @@
 import ofscraper.utils.logger as logger
 from textual import events
 import arrow
 import re
 from diskcache import Cache
 import ofscraper.utils.console as console_
 from ..utils.paths import getcachepath
-cache = Cache(getcachepath())
-log = logging.getLogger(__package__)
 
+log = logging.getLogger("shared")
 
 
 
 
 
 
 
-# console=console_.shared_console
+
+# console=console_.get_shared_console()
 class OutConsole(TextLog):
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
 
 class StyledButton(Button):
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
```

### Comparing `ofscraper-2.7.9/ofscraper/commands/check.py` & `ofscraper-3.0/ofscraper/commands/check.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import re
 import time
 import asyncio
 import threading
 import queue
 import textwrap
 import arrow
+from diskcache import Cache
 import ofscraper.utils.args as args_
 import ofscraper.db.operations as operations
 import ofscraper.api.profile as profile
 import ofscraper.utils.auth as auth
 import ofscraper.api.timeline as timeline
 import ofscraper.api.messages as messages_
 import ofscraper.classes.posts as posts_
@@ -20,42 +21,38 @@
 import ofscraper.utils.console as console_
 import ofscraper.classes.table as table
 import ofscraper.commands.manual as manual
 import ofscraper.utils.download as download
 import ofscraper.db.operations as operations
 import ofscraper.constants as constants
 import ofscraper.classes.sessionbuilder as sessionbuilder
-
-
-from diskcache import Cache
 from ..utils.paths import getcachepath
-cache = Cache(getcachepath())
 
-log = logging.getLogger(__package__)
-args = args_.getargs()
-console=console_.shared_console
+log = logging.getLogger("shared")
+console=console_.get_shared_console()
 ROW_NAMES = "Number","Download_Cart", "UserName", "Downloaded", "Unlocked", "Times_Detected", "Length", "Mediatype", "Post_Date", "Post_Media_Count", "Responsetype", "Price", "Post_ID", "Media_ID", "Text"
 ROWS = []
 app=None
 
 
 def process_download_cart():
+        
         while True:
             global app
             while app and not app.row_queue.empty():
                 log.info("Getting items from queue")
                 try:
                     row,key=app.row_queue.get() 
                     restype=app.row_names.index('Responsetype')
                     username=app.row_names.index('UserName')
                     post_id=app.row_names.index('Post_ID')
                     media_id=app.row_names.index('Media_ID')
                     url=None
                     if row[restype].plain=="message":
-                        url=constants.messagesNextEP.format(row[username].plain,row[post_id].plain)
+                        url=constants.messageTableSPECIFIC.format(row[username].plain,row[post_id].plain)
                     elif row[restype].plain=="post":
                         url=f"{row[post_id]}"
                     elif row[restype].plain=="highlights":
                         url=constants.storyEP.format(row[post_id].plain)
                     elif row[restype].plain=="stories":
                         url=constants.highlightsWithAStoryEP.format(row[post_id].plain)
                     else:
@@ -68,20 +65,20 @@
                     medialist=list(filter(lambda x: x.id==(int(row[media_id].plain) if x.id else None) ,list(media_dict.values())[0]))
                     media=medialist[0] if len(medialist)>0 else []
                     model_id =media.post.model_id
                     username=media.post.username
                     log.info(f"Downloading Invidual media for {username} {media.filename}")
                     operations.create_tables(model_id,username)
                     operations.write_profile_table(model_id,username)
-                    values=asyncio.run(download.process_dicts(
+                    values=download.process_dicts(
                     username,
                     model_id,
                     [media],
-                    ))
-                    if values==None or values[0]!=1:
+                    )
+                    if values==None or values[-1]==1:
                         raise Exception("Download is marked as skipped")
                     log.info("Download Finished")
                     app.update_cell(key,"Download_Cart","[downloaded]")
                     app.update_cell(key,"Downloaded",True)
 
                 except Exception as E:
                         app.update_downloadcart_cell(key,"[failed]")
@@ -94,14 +91,16 @@
 
 
 
 
 
 def post_checker():
     user_dict = {}
+    cache = Cache(getcachepath())
+
     with sessionbuilder.sessionBuilder(backend="httpx") as c:
         links = list(url_helper())
         for ele in links:
             name_match = re.search(f"onlyfans.com/({constants.USERNAME_REGEX}+$)", ele)
             name_match2 = re.search(f"^{constants.USERNAME_REGEX}+$", ele)
 
             if name_match:
@@ -115,28 +114,28 @@
                 continue
             if user_dict.get(user_name):
                 continue
         
             oldtimeline = cache.get(f"timeline_check_{model_id}", default=[])
             user_dict[user_name] = {}
             user_dict[user_name] = user_dict[user_name] or []
-            if len(oldtimeline) > 0 and not args.force:
+            if len(oldtimeline) > 0 and not args_.getargs().force:
                 user_dict[user_name].extend(oldtimeline)
             else:
                 user_dict[user_name] = {}
                 user_dict[user_name] = user_dict[user_name] or []
                 data=asyncio.run(
                     timeline.get_timeline_post( model_id))
                 user_dict[user_name].extend(data)
                 cache.set(
                     f"timeline_check_{model_id}", data, expire=constants.CHECK_EXPIRY)
                 cache.close()
             
             oldarchive = cache.get(f"archived_check_{model_id}", default=[])
-            if len( oldarchive) > 0 and not args.force:
+            if len( oldarchive) > 0 and not args_.getargs().force:
                 user_dict[user_name].extend(oldarchive)
             else:
                 data=asyncio.run(
                     archive.get_archived_post( model_id))
                 user_dict[user_name].extend(data)
                 cache.set(
                     f"archived_check_{model_id}", data, expire=constants.CHECK_EXPIRY)
@@ -169,61 +168,61 @@
     thread_starters(ROWS)
 
 def reset_url():
     #clean up args once check modes are ready to launch
     args=args_.getargs()
     argdict=vars(args)
     if argdict.get("url"):
-        args.url=None
+        args_.getargs().url=None
     if argdict.get("file"):
-        args.file=None
+        args_.getargs().file=None
     if argdict.get("username"):
-        args.username=None
+        args_.getargs().username=None
     args_.changeargs(args)
     
 
 
 
 def set_count(ROWS):
     for count,ele in enumerate(ROWS):
         ele[0]=count+1
 
 
 def message_checker():
     links = list(url_helper())
+    cache = Cache(getcachepath())
     ROWS=[]
     for item in links:
         num_match = re.search(f"({constants.NUMBER_REGEX}+)", item) or re.search(f"^({constants.NUMBER_REGEX}+)$", item)
         name_match = re.search(f"^{constants.USERNAME_REGEX}+$", item)
-        headers = auth.make_headers(auth.read_auth())
         if num_match:
             model_id = num_match.group(1)
             user_name = profile.scrape_profile( model_id)['username']
         elif name_match:
             user_name = name_match.group(0)
             model_id = profile.get_id(user_name) 
         else:
             continue    
         log.info(f"Getting Messages/Paid content for {user_name}")
         # messages
         messages = None
         oldmessages = cache.get(f"message_check_{model_id}", default=[])
         log.debug(f"Number of messages in cache {len(oldmessages)}")
         
-        if len(oldmessages) > 0 and not args.force:
+        if len(oldmessages) > 0 and not args_.getargs().force:
             messages = oldmessages
         else:
             messages = asyncio.run(
                 messages_.get_messages( model_id))
             cache.set(f"message_check_{model_id}",
                         messages, expire=constants.CHECK_EXPIRY)
         oldpaid = cache.get(f"purchased_check_{model_id}", default=[])
         paid = None
         # paid content
-        if len(oldpaid) > 0 and not args.force:
+        if len(oldpaid) > 0 and not args_.getargs().force:
             paid = oldpaid
         else:
             paid = asyncio.run(paid_.get_paid_posts(user_name, model_id))
             cache.set(f"purchased_check_{model_id}",
                       paid, expire=constants.CHECK_EXPIRY)  
         media = get_all_found_media(user_name, messages+paid)
         unduped=[]
@@ -238,25 +237,26 @@
     reset_url()
     set_count(ROWS)
     thread_starters(ROWS)
 
 
 
 def purchase_checker():
+    cache = Cache(getcachepath())
     user_dict = {}
     headers = auth.make_headers(auth.read_auth())
     ROWS = []
-    for user_name in args.username:
+    for user_name in args_.getargs().username:
         user_name=profile.scrape_profile(user_name)["username"]
         user_dict[user_name] = user_dict.get(user_name, [])
         model_id = profile.get_id( user_name)
         oldpaid = cache.get(f"purchased_check_{model_id}", default=[])
         paid = None
         
-        if len(oldpaid) > 0 and not args.force:
+        if len(oldpaid) > 0 and not args_.getargs().force:
             paid = oldpaid
         else:
             paid = asyncio.run(paid_.get_paid_posts(user_name, model_id))
             cache.set(f"purchased_check_{model_id}",
                       paid, expire=constants.CHECK_EXPIRY)
         downloaded = get_downloaded(user_name, model_id)
         media = get_all_found_media(user_name, paid)
@@ -265,15 +265,15 @@
     set_count(ROWS)
     thread_starters(ROWS)
 
 
 def stories_checker():
     user_dict = {}
     ROWS=[]
-    for user_name in args.username:
+    for user_name in args_.getargs().username:
         user_name=profile.scrape_profile(user_name)["username"]
         user_dict[user_name] = user_dict.get(user_name, [])
         model_id = profile.get_id( user_name)    
         stories = asyncio.run(highlights.get_stories_post( model_id))
         highlights_=asyncio.run(highlights.get_highlight_post( model_id))
         highlights_=list(map(lambda x:posts_.Post(
         x, model_id, user_name,"highlights"), highlights_))
@@ -291,16 +291,16 @@
     thread_starters(ROWS)
 
   
 
 
 def url_helper():
     out = []
-    out.extend(args.file or [])
-    out.extend(args.url or [])
+    out.extend(args_.getargs().file or [])
+    out.extend(args_.getargs().url or [])
     return map(lambda x: x.strip(), out)
 
 
 def get_all_found_media(user_name, posts):
 
     temp = []
     model_id = profile.get_id( user_name)
@@ -317,30 +317,31 @@
     operations.create_tables(model_id, user_name)
     paid=get_paid_ids(model_id,user_name) if paid else []
     [downloaded.update({ele: downloaded.get(ele, 0)+1}) for ele in operations.get_media_ids(model_id, user_name)+paid]
 
     return downloaded
 
 def get_paid_ids(model_id,user_name):
+    cache = Cache(getcachepath())
     oldpaid = cache.get(f"purchased_check_{model_id}", default=[])
     paid = None
         
-    if len(oldpaid) > 0 and not args.force:
+    if len(oldpaid) > 0 and not args_.getargs().force:
          paid = oldpaid
     else:
         paid = asyncio.run(paid_.get_paid_posts(user_name, model_id))
         cache.set(f"purchased_check_{model_id}",
                       paid, expire=constants.CHECK_EXPIRY)
     media = get_all_found_media(user_name, paid)
     media=list(filter(lambda x:x.canview==True,media))
     return list(map(lambda x:x.id,media))
 
 
 def thread_starters(ROWS_): 
-    worker_thread = threading.Thread(target=process_download_cart)
+    worker_thread = threading.Thread(target=process_download_cart,daemon=True)
     worker_thread.start()
     start_table(ROWS_)
     
 
 def start_table(ROWS_):
     global app
     loop = asyncio.new_event_loop()
@@ -388,14 +389,15 @@
 def times_helper(ele, mediadict, downloaded):
     return max(len(mediadict.get(ele.id, [])), downloaded.get(ele.id, 0))
 
 def checkmarkhelper(ele):
     return '[]' if unlocked_helper(ele) else "Not Unlocked"
   
 def row_gather(media, downloaded, username):
+    cache = Cache(getcachepath())
 
     # fix text
 
     mediadict = {}
     [mediadict.update({ele.id: mediadict.get(ele.id, []) + [ele]})
      for ele in list(filter(lambda x:x.canview,media))]
     out = []
```

### Comparing `ofscraper-2.7.9/ofscraper/commands/manual.py` & `ofscraper-3.0/ofscraper/commands/manual.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,33 +11,33 @@
 import ofscraper.api.messages as messages_
 import ofscraper.api.highlights as highlights_
 import ofscraper.constants as constants
 import ofscraper.classes.sessionbuilder as sessionbuilder
 import ofscraper.utils.of as of
 
 
-log = logging.getLogger(__package__)
+log = logging.getLogger("shared")
 
 
 def manual_download(urls=None):
     media_dict=get_media_from_urls(urls)
     log.debug(f"Media dict length {len(list(media_dict.values()))}")
     for value in media_dict.values():
         if len(value)==0:
             continue
         model_id =value[0].post.model_id
         username=value[0].post.username
-        log.info(f"Downloading individual media for{username}")
+        log.info(f"Downloading individual media for {username}")
         operations.create_tables(model_id,username)
         operations.write_profile_table(model_id,username)
-        asyncio.run(download.process_dicts(
+        download.process_dicts(
         username,
         model_id,
         value,
-        )) 
+        )
     log.info(f"Finished")
 
 def get_media_from_urls(urls):
     args = args_.getargs()
     args.dupe=True
     args_.changeargs(args)
     user_name_dict={}
@@ -118,30 +118,30 @@
 
 def get_info(url):
     search1=re.search(f"chats/chat/({constants.NUMBER_REGEX}+)/.*?({constants.NUMBER_REGEX}+)",url)
     search2=re.search(f"/({constants.NUMBER_REGEX}+)/stories/highlights",url)
     search3=re.search(f"/stories/highlights/({constants.NUMBER_REGEX}+)",url)
 
     search4=re.search(f"/({constants.NUMBER_REGEX}+)/stories",url)
-    search5=re.search(f"chats/({constants.USERNAME_REGEX}+)/.*?id=({constants.NUMBER_REGEX}+)",url)
+    search5=re.search(f"chats/({constants.USERNAME_REGEX}+)/.*?(id|firstId)=({constants.NUMBER_REGEX}+)",url)
     search6=re.search(f"/({constants.NUMBER_REGEX}+)/({constants.USERNAME_REGEX}+)",url)
     search7=re.search(f"^{constants.NUMBER_REGEX}+$",url)
   #model,postid,type
 
     if search1:
         return search1.group(1),search1.group(2),"msg"
     elif search2 or search3:
         search=search2 or search3
         return None,search.group(1),"highlights"
     elif search4:
         return None,search4.group(1),"stories"
 
 
     elif search5:
-        return search5.group(1),search5.group(2),"msg2"
+        return search5.group(1),search5.group(3),"msg2"
 
     elif search6:
         return search6.group(2),search6.group(1),"post"
     elif search7:
         return None,search7.group(0),"unknown"
```

### Comparing `ofscraper-2.7.9/ofscraper/commands/scraper.py` & `ofscraper-3.0/ofscraper/commands/scraper.py`

 * *Files 14% similar despite different names*

```diff
@@ -37,23 +37,23 @@
 import ofscraper.utils.logger as logger
 import ofscraper.utils.args as args_
 import ofscraper.utils.filters as filters
 import ofscraper.utils.stdout as stdout
 import ofscraper.utils.userselector as userselector
 import ofscraper.utils.console as console
 import ofscraper.utils.of as OF
+import ofscraper.utils.exit as exit
 
-log=logging.getLogger(__package__)
-args=args_.getargs()
-log.debug(args)
+log=logging.getLogger("shared")
 
+@exit.exit_wrapper
 def process_prompts():
     
     while  True:
-        args.posts=[]
+        args_.getargs().posts=[]
         result_main_prompt = prompts.main_prompt()
      
         #download
         if result_main_prompt == 0:
             check_auth()
             check_config()
             run(process_post)
@@ -117,81 +117,83 @@
 
 
 
 
 
 
 
+@exit.exit_wrapper
 def process_post():
-    if args.users_first:
+    if args_.getargs().users_first:
          process_post_user_first()
     else:
         normal_post_process()
-           
+
+@exit.exit_wrapper           
 def process_post_user_first():
      with scrape_context_manager():
         profiles.print_current_profile()
-        headers = auth.make_headers(auth.read_auth())
-        init.print_sign_status(headers)
-        if args.users_first:
+        init.print_sign_status()
+        if args_.getargs().users_first:
             output=[]
             userdata=userselector.getselected_usernames(rescan=False)
             length=len(userdata)
             for count,ele in enumerate(userdata):
                 log.info(f"Progress {count+1}/{length} model")
-                if args.posts:
-                    log.info(f"Getting {','.join(args.posts)} for [bold]{ele['name']}[/bold]\n[bold]Subscription Active:[/bold] {ele['active']}")
+                if args_.getargs().posts:
+                    log.info(f"Getting {','.join(args_.getargs().posts)} for [bold]{ele['name']}[/bold]\n[bold]Subscription Active:[/bold] {ele['active']}")
                 try:
                     model_id = profile.get_id( ele["name"])
                     operations.create_tables(model_id,ele['name'])
                     operations.write_profile_table(model_id,ele['name'])
                     output.extend(OF.process_areas( ele, model_id)) 
                 except Exception as e:
                     log.traceback(f"failed with exception: {e}")
                     log.traceback(traceback.format_exc())               
-            if args.scrape_paid:
+            if args_.getargs().scrape_paid:
                 output.extend(OF.process_all_paid())
             user_dict={}
             [user_dict.update({ele.post.model_id:user_dict.get(ele.post.model_id,[])+[ele]}) for ele in output]
             for value in user_dict.values():
                 model_id =value[0].post.model_id
                 username=value[0].post.username
                 operations.create_tables(model_id,username)
                 operations.write_profile_table(model_id,username)
-                asyncio.run(download.process_dicts(
+                download.process_dicts(
                 username,
                 model_id,
                 value,
-                ))  
+                )
+
+@exit.exit_wrapper
 def normal_post_process():
     with scrape_context_manager():
         profiles.print_current_profile()
-        headers = auth.make_headers(auth.read_auth())
-        init.print_sign_status(headers)
+        init.print_sign_status()
         userdata=userselector.getselected_usernames(rescan=False)
         length=len(userdata)
         for count,ele in enumerate(userdata):
             log.info(f"Progress {count+1}/{length} model")
-            if args.posts:
-                log.info(f"Getting {','.join(args.posts)} for [bold]{ele['name']}[/bold]\n[bold]Subscription Active:[/bold] {ele['active']}")
+            if args_.getargs().posts:
+                log.info(f"Getting {','.join(args_.getargs().posts)} for [bold]{ele['name']}[/bold]\n[bold]Subscription Active:[/bold] {ele['active']}")
             try:
                 model_id = profile.get_id( ele["name"])
                 operations.create_tables(model_id,ele['name'])
                 operations.write_profile_table(model_id,ele['name'])
                 combined_urls=OF.process_areas( ele, model_id)
-                asyncio.run(download.process_dicts(
+                download.process_dicts(
                 ele["name"],
                 model_id,
                 combined_urls,
-                ))
+                )
             except Exception as e:
                 log.traceback(f"failed with exception: {e}")
                 log.traceback(traceback.format_exc())
         
-        if args.scrape_paid:
+        if args_.getargs().scrape_paid:
             try:
                 user_dict={}
                 [user_dict.update({ele.post.model_id:user_dict.get(ele.post.model_id,[])+[ele]}) for ele in OF.process_all_paid()]
                 for value in user_dict.values():
                     model_id =value[0].post.model_id
                     username=value[0].post.username
                     operations.create_tables(model_id,username)
@@ -201,21 +203,20 @@
                     username,
                     model_id,
                     value,
                     ))
             except Exception as e:
                 log.traceback(f"failed with exception: {e}")
                 log.traceback(traceback.format_exc())     
-            
 
+@exit.exit_wrapper
 def process_like():
     with scrape_context_manager():
         profiles.print_current_profile()
-        headers = auth.make_headers(auth.read_auth())
-        init.print_sign_status(headers)
+        init.print_sign_status()
         userdata=userselector.getselected_usernames(rescan=False)
         active=list(filter(lambda x: x["active"],userdata))
         length=len(active)
         with stdout.lowstdout():
             for count,ele in enumerate(active):
                     log.info(f"Progress {count+1}/{length} model")
                     model_id = profile.get_id( ele["name"])
@@ -223,19 +224,19 @@
                     unfavorited_posts = like.filter_for_unfavorited(posts)  
                     unfavorited_posts=filters.timeline_array_filter(unfavorited_posts)   
                     log.debug(f"[bold]Number of unliked posts left after date filters[/bold] {len(unfavorited_posts)}")
                     post_ids = like.get_post_ids(unfavorited_posts)
                     log.debug(f"[bold]Final Number of open and likable post[/bold] {len(post_ids)}")
                     like.like( model_id, ele["name"], post_ids)
 
+@exit.exit_wrapper
 def process_unlike():
     with scrape_context_manager(): 
         profiles.print_current_profile()
-        headers = auth.make_headers(auth.read_auth())
-        init.print_sign_status(headers)
+        init.print_sign_status()
         userdata=userselector.getselected_usernames(rescan=False)
         active=list(filter(lambda x: x["active"],userdata))
         length=len(active)
         with stdout.lowstdout():
             for count,ele in enumerate(active):
                     log.info(f"Progress {count+1}/{length} model")
                     model_id = profile.get_id( ele["name"])
@@ -244,80 +245,118 @@
                     favorited_posts=filters.timeline_array_filter(favorited_posts) 
                     log.debug(f"[bold]Number of liked posts left after date filters[/bold] {len(favorited_posts)}")
                     post_ids = like.get_post_ids(favorited_posts)
                     log.debug(f"[bold]Final Number of open and unlikable post[/bold] {len(post_ids)}")
                     like.unlike( model_id, ele["name"], post_ids)
 #Adds a function to the job queue
 def set_schedule(*functs):
-    [schedule.every(args.daemon).minutes.do(jobqueue.put,funct) for funct in functs]
-    while True:
+    [schedule.every(args_.getargs().daemon).minutes.do(jobqueue.put,funct) for funct in functs]
+    while len(schedule.jobs)>0:
         schedule.run_pending()
         time.sleep(30)
 
 
 
 ## run script once or on schedule based on args
 def run(*functs):
     # get usernames prior to potentially supressing output
     check_auth()
-    if args.output=="PROMPT":
+    if args_.getargs().output=="PROMPT":
         log.info(f"[bold]silent-mode on[/bold]")    
-    if args.daemon:
+    if args_.getargs().daemon:
         log.info(f"[bold]daemon mode on[/bold]")   
     run_helper(*functs)
 
 
 def run_helper(*functs):
     # run each function once
     global jobqueue
     jobqueue=queue.Queue()
     [jobqueue.put(funct) for funct in functs]
-    if args.daemon:   
-        worker_thread = threading.Thread(target=set_schedule,args=[*functs])
-        worker_thread.start()
-        # Check if jobqueue has function
-        while True:
-            log.debug(schedule.jobs)
-            job_func = jobqueue.get()
-            job_func()
-            jobqueue.task_done()
-            userselector.getselected_usernames(rescan=True)
+    worker_thread=None
+          
+    try:
+        if args_.getargs().daemon:
+                worker_thread = threading.Thread(target=set_schedule,args=[*functs],daemon=True)
+                worker_thread.start()
+                # Check if jobqueue has function
+                while True:
+                    log.debug(schedule.jobs)
+                    job_func = jobqueue.get()
+                    job_func()
+                    jobqueue.task_done()
+                    userselector.getselected_usernames(rescan=True)
+    except KeyboardInterrupt as E:
+            try:
+                with exit.DelayedKeyboardInterrupt():
+                    schedule.clear()
+                raise KeyboardInterrupt
+            except KeyboardInterrupt:
+                schedule.clear()
+                raise KeyboardInterrupt
+    except Exception as E:
+            try:
+                with exit.DelayedKeyboardInterrupt():
+                    schedule.clear()
+                raise E
+            except KeyboardInterrupt:
+                schedule.clear()
+                raise KeyboardInterrupt
             
             #update selected user
     else:
-        userselector.getselected_usernames(rescan=True,reset=True)
-        [(jobqueue.get())() for funct in functs]
-            
+        try:
+            userselector.getselected_usernames(rescan=True,reset=True)
+            for _ in functs:
+                job_func = jobqueue.get()
+                job_func()
+                jobqueue.task_done()
+        except KeyboardInterrupt as E:
+            try:
+                with exit.DelayedKeyboardInterrupt():
+                    None
+                raise KeyboardInterrupt
+            except KeyboardInterrupt:
+                schedule.clear()
+                raise KeyboardInterrupt
+        except Exception as E:
+            try:
+                with exit.DelayedKeyboardInterrupt():
+                    None
+                raise E
+            except KeyboardInterrupt:
+                None
+                raise KeyboardInterrupt     
                 
 def check_auth():
     status=None
     while status!="UP":
-        headers = auth.make_headers(auth.read_auth())
-        status=init.getstatus(headers)
+        status=init.getstatus()
         if status=="DOWN":
             log.error("Auth Failed")
             auth.make_auth(auth=auth.read_auth())
             continue
         break
         
 
 def check_config():
     while not  paths.mp4decryptchecker(config.get_mp4decrypt(config.read_config())):
-        console.shared_console.print("You need to select path for mp4decrypt\n\n")
+        console.get_shared_console().print("You need to select path for mp4decrypt\n\n")
         log.debug(f"[bold]current mp4decrypt path[/bold] {config.get_mp4decrypt(config.read_config())}")
         config.update_mp4decrypt()
     while not  paths.ffmpegchecker(config.get_ffmpeg(config.read_config())):
-        console.shared_console.print("You need to select path for ffmpeg\n\n")
+        console.get_shared_console().print("You need to select path for ffmpeg\n\n")
         log.debug(f"[bold]current ffmpeg path[/bold] {config.get_ffmpeg(config.read_config())}")
         config.update_ffmpeg()
     log.debug(f"[bold]final mp4decrypt path[/bold] {config.get_mp4decrypt(config.read_config())}")
     log.debug(f"[bold]final ffmpeg path[/bold] {config.get_ffmpeg(config.read_config())}")
 
 
 
+
 @contextmanager
 def scrape_context_manager():
         
         # Before yield as the enter method
 
         start = timeit.default_timer()
         log.error(
@@ -335,63 +374,59 @@
 ===========================
 [bold]Script Finished[/bold]
 Run Time:  [bold]{str(arrow.get(end)-arrow.get(start)).split(".")[0]}[/bold]
 ===========================
 """)
 def print_start():
     with stdout.lowstdout():
-        console.shared_console.print(
-            f"[bold green]Welcome to OF-Scraper Version {args.version}[/bold green]"
+        console.get_shared_console().print(
+            f"[bold green]Welcome to OF-Scraper Version {args_.getargs().version}[/bold green]"
         )                
 def main():
  
         try:
+            
             print_start()
-            logger.start_discord_queue()
+
             scrapper()
             paths.cleanup()
-            logger.discord_cleanup()
         except KeyboardInterrupt as E:
             try:
                 with exit.DelayedKeyboardInterrupt():
                     paths.cleanup()
-                    logger.discord_cleanup()
-                    sys.exit(0)
+                    raise KeyboardInterrupt
             except KeyboardInterrupt:
-                    sys.exit(0)
-
-
+                    raise KeyboardInterrupt
         except Exception as E:
             try:
                 with exit.DelayedKeyboardInterrupt():
                     paths.cleanup()
-                    logger.discord_cleanup()
                     log.traceback(E)
                     log.traceback(traceback.format_exc())
-                    sys.exit(0)
+                    raise E
             except KeyboardInterrupt:
-                sys.exit(0)
+                raise KeyboardInterrupt
 def scrapper():
-    if platform.system == 'Windows':
+    if platform.system() == 'Windows':
         os.system('color')
     global selectedusers
     selectedusers=None
     functs=[]
-    if len(args.posts)==0 and not args.action and not args.scrape_paid:
-        if args.daemon:
+    if len(args_.getargs().posts)==0 and not args_.getargs().action and not args_.getargs().scrape_paid:
+        if args_.getargs().daemon:
                     log.error("You need to pass at least one scraping method\n--action\n--posts\n--purchase\nAre all valid options. Skipping and going to menu")
         process_prompts()
         return
     check_auth()
     check_config()
-    if len(args.posts)>0 or args.scrape_paid: 
+    if len(args_.getargs().posts)>0 or args_.getargs().scrape_paid: 
         functs.append(process_post)      
-    elif args.action=="like":
+    elif args_.getargs().action=="like":
         functs.append(process_like)
-    elif args.action=="unlike":
+    elif args_.getargs().action=="unlike":
         functs.append(process_unlike)
     run(*functs)
```

### Comparing `ofscraper-2.7.9/ofscraper/constants.py` & `ofscraper-3.0/ofscraper/constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 r"""
                                                              
-        _____                                               
+        _____                                    ay           
   _____/ ____\______ ________________    ____   ___________ 
  /  _ \   __\/  ___// ___\_  __ \__  \  /  _ \_/ __ \_  __ \
 (  <_> )  |  \___ \\  \___|  | \// __ \(  <_> )  ___/|  | \/
  \____/|__| /____  >\___  >__|  (____  /\____/ \___  >__|   
                  \/     \/           \/            \/         
 """
 import pathlib
+import os
 preferences = 'pref_config.py'
 configPath = '.config/ofscraper'
 configFile = 'config.json'
 authFile = 'auth.json'
 databaseFile = 'models.db'
 mainProfile = 'main_profile'
 requestAuth = 'request_auth.json'
@@ -52,18 +53,18 @@
 
 DEVIINT = 'https://raw.githubusercontent.com/deviint/onlyfans-dynamic-rules/main/dynamicRules.json'
 donateEP = "https://www.buymeacoffee.com/excludedBittern"
 
 purchased_contentEP = "https://onlyfans.com/api2/v2/posts/paid?limit=100&skip_users=all&format=infinite&offset={}&user_id={}"
 purchased_contentALL = "https://onlyfans.com/api2/v2/posts/paid?limit=100&skip_users=all&format=infinite&offset={}"
 
-messageSPECIFIC="https://onlyfans.com/my/chats/chat/{}/?firstId={}"
 highlightSPECIFIC="https://onlyfans.com/api2/v2/stories/highlights/{}"
 storiesSPECIFIC="https://onlyfans.com/api2/v2/stories/{}"
 messageSPECIFIC= "https://onlyfans.com/api2/v2/chats/{}/messages?limit=10&order=desc&skip_users=all&firstId={}"
+messageTableSPECIFIC="https://onlyfans.com/my/chats/{}/?id={}"
 
 labelsEP = "https://onlyfans.com/api2/v2/users/{}/labels?limit=100&offset={}&order=desc&non-empty=1"
 labelledPostsEP = "https://onlyfans.com/api2/v2/users/{}/posts?limit=100&offset={}&order=publish_date_desc&skip_users=all&counters=0&format=infinite&label={}"
 
 
 mainPromptChoices = {
     'Download content from a user': 0,
@@ -93,68 +94,74 @@
   'This tool is for educational purposes only and is not intended for actual use. Should you choose to actually use it you accept all consequences and agree that you are not using it to redistribute content or  for any other action that will cause loss of revenue to creators or platforms scraped.',
   
 ]
 KEY_DEFAULT="keydb"
 DIR_FORMAT_DEFAULT="{model_username}/{responsetype}/{mediatype}/"
 FILE_FORMAT_DEFAULT="{filename}.{ext}"
 METADATA_DEFAULT="{configpath}/{profile}/.data/{model_username}_{model_id}"
-FILE_SIZE_DEFAULT=0
+FILE_SIZE_LIMIT_DEFAULT=0
+FILE_SIZE_MIN_DEFAULT=0
 TEXTLENGTH_DEFAULT=0
 FILTER_DEFAULT=["Images","Audios","Videos"]
 SAVE_PATH_DEFAULT=str(pathlib.Path.home()/'Data/ofscraper')
 DATE_DEFAULT="MM-DD-YYYY"
 PROFILE_DEFAULT="main_profile"
 PREMIUM_DEFAULT="Premium"
 MP4DECRYPT_DEFAULT=""
 FFMPEG_DEFAULT =""
 DISCORD_DEFAULT =""
 BACKEND_DEFAULT ="aio"
-
+THREADS_DEFAULT=int(os.cpu_count()*(2/3))
+DOWNLOAD_SEM_DEFAULT=max(-(-(20//int(THREADS_DEFAULT))),6)
 DYNAMIC_DEFAULT="deviint"
 SUPPRESS_LOG_LEVEL=21
+PROGRESS_DEFAULT=False
 
 RESPONSE_TYPE_DEFAULT= {
             "message":"Messages",
             "timeline":"Posts",
             "archived":"Archived",
             "paid":"Messages",
             "stories":"Stories",
             "highlights":"Stories",
             "profile":"Profile",
             "pinned":"Posts"
         }
 NUM_TRIES=10
-
+DATABASE_TIMEOUT=300
 
 RESPONSE_EXPIRY=5000000
 CHECK_EXPIRY=86400
 DAILY_EXPIRY=86400
 HOURLY_EXPIRY=3600
 SIZE_TIMEOUT=1209600
-KEY_EXPIRY=2592000
+KEY_EXPIRY=None
 DISCORDWAIT=5
-OF_MIN=15
+OF_MIN=20
 OF_MAX=50
 LICENCE_URL="https://onlyfans.com/api2/v2/users/media/{}/drm/{}/{}?type=widevine"
 logname="ofscraper"
 PATH_STR_MAX=200
 TABLE_STR_MAX=100
 
-refreshScreen=20
+refreshScreen=50
 
 MP4DECRYPT_LINUX="https://www.bok.net/Bento4/binaries/Bento4-SDK-1-6-0-640.x86_64-unknown-linux.zip"
 MP4DECRYPT_WINDOWS="https://www.bok.net/Bento4/binaries/Bento4-SDK-1-6-0-640.x86_64-microsoft-win32.zip"
 MP4DECRYPT_MAC="https://www.bok.net/Bento4/binaries/Bento4-SDK-1-6-0-640.universal-apple-macosx.zip"
 FFMPEG_LINUX="https://github.com/BtbN/FFmpeg-Builds/releases/download/latest/ffmpeg-master-latest-linux64-gpl.tar.xz"
 FFMPEG_WINDOWS="https://github.com/BtbN/FFmpeg-Builds/releases/download/latest/ffmpeg-master-latest-win64-gpl.zip"
 FFMPEG_MAC="https://evermeet.cx/ffmpeg/ffmpeg-111111-gc44fe10160.zip"
 
 
-THREADS_DEFAULT=8
 MAX_SEMAPHORE=8
 AlT_SEM=4
 CODE_EXECUTION_DEFAULT =False
 
 NUMBER_REGEX="[0-9]"
 USERNAME_REGEX="[^/]"
 
-API_REEQUEST_TIMEOUT=90
+API_REEQUEST_TIMEOUT=90
+SUPRESS_OUTPUTS={"CRITICAL","ERROR","WARNING","OFF","LOW","PROMPT"}
+CHUNK_ITER=20
+maxChunkSize=1024*10
+KEY_OPTIONS=["cdrm","cdrm2","manual","keydb"]
```

### Comparing `ofscraper-2.7.9/ofscraper/db/operations.py` & `ofscraper-3.0/ofscraper/db/operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,17 +15,18 @@
 import traceback
 import math
 import logging
 from rich.console import Console
 from ..db import queries
 from ..utils.paths import createDir
 import ofscraper.classes.placeholder as placeholder
+from ofscraper.constants import DATABASE_TIMEOUT
 
 console=Console()
-log=logging.getLogger(__package__)
+log=logging.getLogger("shared")
 #print error 
 def operation_wrapper(func): 
     def inner(*args,**kwargs): 
         try:
             return func(*args,**kwargs) 
         except sqlite3.OperationalError as E:
             log.info("DB may be locked") 
@@ -122,23 +123,23 @@
 @operation_wrapper
 def get_profile_info(model_id,username) -> list:
     datebase_path =placeholder.Placeholders().databasePathHelper(model_id,username)
     if not pathlib.Path(datebase_path).exists():
         return None
     with contextlib.closing(sqlite3.connect(datebase_path,check_same_thread=False)) as conn:
         with contextlib.closing(conn.cursor()) as cur:
-            modelinfo=cur.execute(queries.prorfileDupeCheck,(model_id,)).fetchall() or [(None,)]
+            modelinfo=cur.execute(queries.profileDupeCheck,(model_id,)).fetchall() or [(None,)]
             conn.commit()
             return modelinfo[0][-1]
 
 
 @operation_wrapper
 async def write_media_table(media,filename,model_id,username) -> list:
     datebase_path =placeholder.Placeholders().databasePathHelper(model_id,username)
-    async with aiosqlite.connect(datebase_path) as conn:
+    async with aiosqlite.connect(datebase_path,timeout=DATABASE_TIMEOUT) as conn:
         insertData=[media.id,media.postid,media.url,str(pathlib.Path(filename).parent),pathlib.Path(filename).name,
         math.ceil(pathlib.Path(filename).stat().st_size),media.responsetype_.capitalize(),media.mediatype.capitalize() ,
         media.preview,media.linked, 1,media.date]
         if len((await (await conn.execute(queries.mediaDupeCheck,(media.id,))).fetchall()))==0:
             await conn.execute(queries.mediaInsert,insertData)
         else:
             insertData.append(media.id)
```

### Comparing `ofscraper-2.7.9/ofscraper/db/queries.py` & `ofscraper-3.0/ofscraper/db/queries.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.9/ofscraper/interaction/like.py` & `ofscraper-3.0/ofscraper/interaction/like.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import logging
 import ssl
 import certifi
 from typing import Union
 import asyncio
 import aiohttp
 
-from tenacity import retry,stop_after_attempt,wait_random
+from tenacity import retry,stop_after_attempt,wait_random,retry_if_not_exception_type
 
 from rich.progress import Progress
 from rich.progress import (
     Progress,
     MofNCompleteColumn,
     BarColumn,
     TextColumn,
@@ -37,15 +37,15 @@
 import ofscraper.constants as constants
 from ofscraper.utils.semaphoreDelayed import semaphoreDelayed
 import ofscraper.classes.sessionbuilder as sessionbuilder
 import ofscraper.prompts.prompts as prompts
 
 
 sem = semaphoreDelayed(1)
-log=logging.getLogger(__package__)
+log=logging.getLogger("shared")
 import ofscraper.utils.args as args_
 
 
 
 def get_posts( model_id):
     pinned_posts=[]
     timeline_posts=[]
@@ -83,30 +83,28 @@
 def get_post_ids(posts: list) -> list:
     valid_post=list(filter(lambda x:x.get("isOpened")==True,posts))
     return list(map(lambda x:x.get("id"),valid_post))
    
 
 
 def like( model_id, username, ids: list):
-    headers = auth.make_headers(auth.read_auth())
-    asyncio.run(_like(headers, model_id, username, ids, True))
+    asyncio.run(_like(model_id, username, ids, True))
 
 
 def unlike( model_id, username, ids: list):
-    headers = auth.make_headers(auth.read_auth())
-    asyncio.run(_like(headers, model_id, username, ids, False))
+    asyncio.run(_like( model_id, username, ids, False))
 
 
 
 
-async def _like(headers, model_id, username, ids: list, like_action: bool):
+async def _like( model_id, username, ids: list, like_action: bool):
     title = "Liking" if like_action else "Unliking"
     global sem
     sem.delay=3
-    with Progress(SpinnerColumn(style=Style(color="blue")),TextColumn("{task.description}"),BarColumn(),MofNCompleteColumn(),console=console.shared_console) as overall_progress:
+    with Progress(SpinnerColumn(style=Style(color="blue")),TextColumn("{task.description}"),BarColumn(),MofNCompleteColumn(),console=console.get_shared_console()) as overall_progress:
         async with sessionbuilder.sessionBuilder() as c:
             tasks=[]
             task1=overall_progress.add_task(f"{title} posts...\n",total=len(ids))
 
             [tasks.append(asyncio.create_task(_like_request(c,id,model_id)))
                 for id in ids]
             for count,coro in enumerate(asyncio.as_completed(tasks)):
@@ -121,23 +119,23 @@
                         sem.delay=30  
                     
                     overall_progress.update(task1,advance=1,refresh=True)
 
         
         
 
-@retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
+@retry(retry=retry_if_not_exception_type(KeyboardInterrupt),stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
 async def _like_request(c,id,model_id):
     global sem
     async with sem:
         async with c.requests( favoriteEP.format(id, model_id),"post")() as r:
                 if r.ok:
                     return id                  
                 else:
-                        log.debug(f"[bold]timeline request status code:[/bold]{r.status}")
+                        log.debug(f"[bold]timeline response status code:[/bold]{r.status}")
                         log.debug(f"[bold]timeline response:[/bold] {await r.text_()}")
                         log.debug(f"[bold]timeline headers:[/bold] {r.headers}")
                         r.raise_for_status()
```

### Comparing `ofscraper-2.7.9/ofscraper/prompts/keybindings.py` & `ofscraper-3.0/ofscraper/prompts/keybindings.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 fuzzy={
-                             "toggle": [{"key": ["pagedown"]},{"key": ["home"]},{"key": ["end"]},{"key": ["pageup"]}],
+                             "toggle": [{"key": ["pagedown"]},{"key": ["home"]},{"key": ["end"]},{"key": ["pageup"]},{"key": ["s-right"]}],
                              "toggle-all": [{"key": ["c-a"]}],
                              "toggle-all-false": [{"key": ["c-d"]}],
                              "toggle-all-true": [{"key": ["c-s"]}]
 
           
                          }
 
-select={"answer": [{"key": ["pagedown"]},{"key": ["home"]},{"key": ["end"]},{"key": ["space"]},{"key": ["enter"]},{"key": ["space"]},{"key": ["pageup","enter"]}]}
+select={"answer": [{"key": ["s-right"]},{"key": ["pagedown"]},{"key": ["home"]},{"key": ["end"]},{"key": ["space"]},{"key": ["enter"]},{"key": ["pageup","enter"]}]}
 
 input= select
 file=select
 number=select
-multiline=  {"answer":[{"key": ["pagedown","enter"]},{"key": ["home","enter"]},{"key": ["end","enter"]},{"key": ["pageup","enter"]},{"key": ["space","enter"]}]}
+multiline=  {"answer":[{"key": ["pagedown","enter"]},{"key": ["home","enter"]},{"key": ["end","enter"]},{"key": ["pageup","enter"]},{"key": ["space","enter"]},{"key": ["escape"]}]}
```

### Comparing `ofscraper-2.7.9/ofscraper/prompts/promptConvert.py` & `ofscraper-3.0/ofscraper/prompts/promptConvert.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,19 +36,27 @@
 
         prompt_=funct(*args,**kwargs)
 
         @prompt_.register_kb("alt-x")
         def _handle_alt_x(event):
              action_set.add("altx")
              event.app.exit()
+        @prompt_.register_kb("c-b")
+        def _handle_alt_x(event):
+             action_set.add("altx")
+             event.app.exit()
+        
         @prompt_.register_kb("alt-v")
         def _handle_alt_v(event):
             action_set.add("altv")
             event.app.exit()
-    
+        @prompt_.register_kb("c-v")
+        def _handle_alt_v(event):
+            action_set.add("altv")
+            event.app.exit()
         while True:
             out=prompt_.execute()
             prompt_._default=get_default(funct,prompt_)
             if out!=None:
                 break
             if "altx" in action_set:
                 prompt_=altx_action(prompt_)
@@ -72,17 +80,22 @@
 
 def get_default_instructions(funct):
     if funct.__name__=="getChecklistSelection":
         return prompt_strings.CHECKLISTINSTRUCTIONS
     elif funct.__name__=="getFuzzySelection":
         return prompt_strings.FUZZY_INSTRUCTION
     elif funct.__name__=="multiline_input_prompt":
-        return prompt_strings.MULT_LINE
+        return prompt_strings.MULTI_LINE
     elif funct.__name__=="input_prompt":
         return prompt_strings.SINGLE_LINE
+    elif funct.__name__=="number_type":
+        return prompt_strings.SINGLE_LINE
+    
+    elif funct.__name__=="checkbox":
+        return prompt_strings.FUZZY_INSTRUCTION
     elif funct.__name__=="checkbox":
         return prompt_strings.FUZZY_INSTRUCTION
 
 @wrapper
 def getChecklistSelection(*args,**kwargs):
  
     prompt=inquirer.select(
```

### Comparing `ofscraper-2.7.9/ofscraper/prompts/prompt_strings.py` & `ofscraper-3.0/ofscraper/prompts/prompt_strings.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,17 +11,24 @@
 ============================================================
 
 KEYS
 ============================================================
 
    SELECT_KEYS
    ======================================================================
-   END  |  HOME   | PAGEUP | PAGEDOWN | SPACE | ENTER
+   END  |  HOME   | PAGEUP | PAGEDOWN | SPACE | ENTER | shift+right
    ========================================================================
 
+   SPECIAL SELECT
+   Will select and move cursor
+   ================
+   TAB | SHIFT+TAB 
+   =================
+
+
 ==============================================================
 PRESS ENTER TO CONTINUE
 
 &&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&
 """
 
 
@@ -48,18 +55,24 @@
 =========================================================================
   CONFIRM_KEY          
   ============
   ENTER
   ================
  
  
- SELECT_KEYS
+   SELECT_KEYS
    ================================================
-   END  |  HOME   | PAGEUP | PAGEDOWN | SPACE |
+   END  |  HOME | PAGEUP | PAGEDOWN | shift+right
    ================================================
+   
+   SPECIAL SELECT
+   Will select and move cursor
+   ================
+   TAB | SHIFT+TAB 
+   =================
 
 
   TOGGLE_ALL_FALSE
    ========
    CTRL+D
    ========
   
@@ -103,19 +116,22 @@
   ============
   ENTER
   ================
  
  
  SELECT_KEYS
    ================================================
-   END  |  HOME   | PAGEUP | PAGEDOWN | SPACE |
+   END  |  HOME | PAGEUP | PAGEDOWN | shift+right
    ================================================
 
- 
-
+ SPECIAL SELECT
+ Will select and move cursor
+ ================
+  TAB | SHIFT+TAB 
+ =================
 
 
   TOGGLE_ALL_FALSE
    ========
    CTRL+D
    ========
   
@@ -129,29 +145,29 @@
    ========
    CTRL+A
    ========
 
 
    CHANGE_FILTER/SORT
    ========
-   ALT+X
+   ALT+X|CTRL+B
    ========
 ===================================================================
 PRESS ENTER TO CONTINUE
 
 &&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&"""
 
 SCRAPE_PAID=\
 """
 This is meant really for scraping content for deleted models
 This can greatly increase the time needed for a single scrape
 
 It should not be needed to turn this on everytime, especially with  frequent scrapes
 
-SHOW INSTRUCTIONS: [ALT+V]
+SHOW INSTRUCTIONS: [ALT+V] or [CTRL+V]
 """
 
 
 SINGLE_LINE=\
 """
 &&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&
 
@@ -162,34 +178,39 @@
 ===========================================================================
 
 KEYS
 ==========================================================================
 
    SUBMIT_KEYs
    ======================================================================
-   END  |  HOME   | PAGEUP | PAGEDOWN | SPACE | ENTER
+   END  |  HOME   | PAGEUP | PAGEDOWN | SPACE | ENTER | shift+right
    ========================================================================
 
 ==============================================================================
 PRESS ENTER TO CONTINUE
 
 &&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&"""
 
 
 KEY_BOARD=\
 """
-SHOW INSTRUCTIONS: [ALT+V]
+SHOW INSTRUCTIONS: [ALT+V] or [CTRL+V]
 """
 
 
+NUMBER=\
+"""
+SHOW INSTRUCTIONS: [ALT+V] or [CTRL+V]
+"""
+
 
 MODEL_SELECT=\
 """
-SHOW INSTRUCTIONS: [ALT+V]
-CHANGE_SORT/CHANGE_FILTER: [ALT+X]
+SHOW INSTRUCTIONS: [ALT+V] or [CTRL+V]
+CHANGE_SORT/CHANGE_FILTER: [ALT+X] or [CTRL+B]
 """
 
 
 MULTI_LINE=\
 """
 &&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&
 
@@ -197,17 +218,17 @@
 ===========================================================================
 HIT one of the 'SUBMIT' combinations when your auth syntax is corrected
 ============================================================================
 
 KEYS
 ===========================================================================
    SUBMIT_KEYs
-   ======================================================================
-   END+ENTER  |  HOME+ENTER   | PAGEUP+ENTER | PAGEDOWN+ENTER | SPACE+ENTER
-   ========================================================================
+   ==============================================================================
+   END+ENTER  |  HOME+ENTER   | PAGEUP+ENTER | PAGEDOWN+ENTER | SPACE+ENTER | ESC
+   ================================================================================
 
 ==============================================================================
 PRESS ENTER TO CONTINUE
 
 &&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&
 """
 
@@ -222,17 +243,17 @@
 HIT one of the 'SUBMIT' combinations to confirm text
 =========================================================================
 
 KEYS
 =========================================================================
 
    SUBMIT_KEYs
-   ======================================================================
-   END+ENTER  |  HOME+ENTER   | PAGEUP+ENTER | PAGEDOWN+ENTER | SPACE+ENTER
-   ========================================================================
+   =============================================================================
+   END+ENTER  |  HOME+ENTER   | PAGEUP+ENTER | PAGEDOWN+ENTER | SPACE+ENTER| ESC
+   =============================================================================
 
 ==============================================================================
 PRESS ENTER TO CONTINUE
 
 &&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&
 """
 
@@ -245,17 +266,17 @@
 =========================================================================
 HIT one of the 'SUBMIT' combinations when your auth syntax is corrected
 =========================================================================
 
 KEYS
 =========================================================================
    SUBMIT_KEYs
-   ======================================================================
-   END+ENTER  |  HOME+ENTER   | PAGEUP+ENTER | PAGEDOWN+ENTER | SPACE+ENTER
-   ========================================================================
+   ================================================================================
+   END+ENTER  |  HOME+ENTER   | PAGEUP+ENTER | PAGEDOWN+ENTER | SPACE+ENTER | ESC
+   ===============================================================================
 
 ==============================================================================
 PRESS ENTER TO CONTINUE
 
 &&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&
 """
```

### Comparing `ofscraper-2.7.9/ofscraper/prompts/prompt_validators.py` & `ofscraper-3.0/ofscraper/prompts/prompt_validators.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from pathvalidate import  validate_filepath,validate_filename
 import platform
 import pathlib
 import arrow
 import textwrap
 import ofscraper.utils.paths as paths
 import ofscraper.utils.profiles as profiles
+import ofscraper.classes.placeholder as placeholders
 
 
 
 class MultiValidator(Validator):
     """:Runs Multiple Validators Since Inquirerpy does seem to support this functionality natively
 
     Args:
@@ -110,17 +111,17 @@
                 move_cursor_to_end=True,
             )
 
 
 def dirformatvalidator():
     def callable(x):
         try:
-            placeholders=list(filter(lambda x:x!=None,[v[1] for v in string.Formatter().parse(x)]))
-            validplaceholders=set(["date","responsetype","mediatype","value","model_id","first_letter","sitename","model_username"])
-            if len(list(filter(lambda x:x not in validplaceholders,placeholders)))>0:
+            testplaceholders=list(filter(lambda x:x!=None,[v[1] for v in string.Formatter().parse(x)]))
+            validplaceholders=placeholders.all_placeholders()
+            if len(list(filter(lambda x:x not in validplaceholders or not x.find('custom'),testplaceholders)))>0:
                 return False
             result={}
 
             for d in list(map(lambda x:{x:"placeholder"},placeholders)):
                 result.update(d)
             validate_filepath(str(pathlib.Path(x.format(**result))),platform=platform.system())
```

### Comparing `ofscraper-2.7.9/ofscraper/prompts/prompts.py` & `ofscraper-3.0/ofscraper/prompts/prompts.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,17 +4,18 @@
   _____/ ____\______ ________________    ____   ___________ 
  /  _ \   __\/  ___// ___\_  __ \__  \  /  _ \_/ __ \_  __ \
 (  <_> )  |  \___ \\  \___|  | \// __ \(  <_> )  ___/|  | \/
  \____/|__| /____  >\___  >__|  (____  /\____/ \___  >__|   
                  \/     \/           \/            \/         
 """
 import sys
-from rich.console import Console
-import asyncio
 import re
+import os
+from rich.console import Console
+
 import arrow
 from InquirerPy.resolver import prompt
 from InquirerPy.separator import Separator
 from InquirerPy.base import Choice
 from InquirerPy.validator import EmptyInputValidator,PathValidator
 import ofscraper.constants as constants
 import ofscraper.prompts.prompt_strings as prompt_strings
@@ -103,42 +104,47 @@
     answers = promptClasses.batchConverter(*[
         {
             'type': 'input',
             'name': 'sess',
             'message': 'Enter your sess cookie:',
             'default': auth['sess']
             ,'validate':EmptyInputValidator()
+              ,'multiline':True
 
         },
         {
             'type': 'input',
             'name': 'auth_id',
             'message': 'Enter your auth_id cookie:',
             'default': auth['auth_id']
             ,'validate':EmptyInputValidator()
+              ,'multiline':True
         },
         {
             'type': 'input',
             'name': 'auth_uid_',
             'message': 'Enter your auth_uid cookie (leave blank if you don\'t use 2FA):',
             'default': auth['auth_uid_']
+              ,'multiline':True
         },
         {
             'type': 'input',
             'name': 'user_agent',
             'message': 'Enter your `user agent`:',
             'default': auth['user_agent']
             ,'validate':EmptyInputValidator()
+              ,'multiline':True
         },
         {
             'type': 'input',
             'name': 'x-bc',
             'message': 'Enter your `x-bc` token:',
             'default': auth['x-bc']
             ,'validate':EmptyInputValidator()
+            ,'multiline':True
         }
     ])
 
     return answers
 
 
 def ask_make_auth_prompt() -> bool:
@@ -224,14 +230,15 @@
     questions = promptClasses.batchConverter(*[
         {
             'type': 'input',
             "name":name,
             'message':'Paste Text from Extension',
             "validate": prompt_validators.jsonValidator(),
             "filter":prompt_validators.jsonloader,
+            "multiline":True,
              "instruction":\
 """
 Cookie Helper Repo:https://github.com/M-rcus/OnlyFans-Cookie-Helper
 """
              
 
         }
@@ -320,31 +327,60 @@
         }
     ])
     profile = answer[name]
     return profile
 
 
 def config_prompt_advanced(config_) -> dict:
-    new_settings =promptClasses.batchConverter(* [
+    threads =promptClasses.batchConverter(* [
+        {
+            'type': 'number',
+            'name': 'threads',
+            "message":"Number of Download processes/threads: ",
+            'min_allowed':1,
+            'max_allowed':os.cpu_count()-1,
+             "validate":EmptyInputValidator(),
+            'long_instruction':f"Value can be 1-{os.cpu_count()-1}",
+             'default':config.get_threads(config_),
+        },
+        
+    ])
+
+    config_.update(threads)
+        
+        
+        
+    new_settings =promptClasses.batchConverter(*   [{
+            'type': 'number',
+            'name': 'download-sem',
+            "message":"Number of semaphores per thread: ",
+            'min_allowed':1,
+            'max_allowed':max(-(-(50//int(threads["threads"]))),6),
+             "validate":EmptyInputValidator(),
+             'long_instruction':"Value can be 1-20",
+             'default':config.get_download_semaphores(config_),
+        },
         {
             'type': 'list',
             'name': 'dynamic-mode-default',
             'message': 'What would you like to use for dynamic rules',
             'default': config.get_dynamic(config_),
             'choices':["deviint","digitalcriminals"],
         },
+        
         {
             'type': 'list',
             'name': 'key-mode-default',
-            'message': 'Make selection for how to retrive keys',
+            'message': 'Make selection for how to retrive long_message',
             'default': config.get_key_mode(config_),
-            'choices':["auto","cdrm","keydb"],
+            'choices':constants.KEY_OPTIONS,
 
         },
-          {
+
+     {
             'type': 'input',
             'name': 'keydb_api',
             'message': 'keydb api key:\n',
             "long_instruction":"Required if your using keydb for key-mode",
             'default': config.get_keydb_api(config_) or "",
         },
 
@@ -366,28 +402,37 @@
             'choices':[Choice("aio","aiohttp"),Choice("httpx","httpx")],
             'message': 'Select Which Backend you want:\n',
             'default': config.get_backend(config_) or "",
         },
         {
             'type': 'list',
             'name': 'partfileclean',
-            'message': 'auto clean .part files',
-            "long_instruction":"You won't be able to resume downloads if you select 'Yes'",
+            'message': 'Enable auto file resume',
+            "long_instruction":"Enable this if you don't want to auto resume files, and want .part files auto cleaned",
             'default': config.get_part_file_clean(config_),
-            'choices':[Choice(True,"Yes"),Choice(False,"No")],
+            'choices':[Choice(False,"Yes"),Choice(True,"No")],
         },
             {
             'type': 'input',
             'name': 'custom',
             'message': 'edit custom value:\n',
             "long_instruction":"This is a helper value for remapping placeholder values",
             'default': config.get_custom(config_) or "",
         },
-    ]
-    )
+        {
+            "type":"list",
+            "name":"downloadbars",
+            "message":"show download progress bars\nThis can have a negative effect on performance with lower threads",
+            "default":config.get_show_downloadprogress(config_) ,
+            'choices':[Choice(True,"Yes"),Choice(False,"No")]
+
+
+
+        }
+    ])
     config_.update(new_settings)
     return config_
     
 
 def config_prompt(config_) -> dict:
 
     answer = promptClasses.batchConverter(*[
@@ -404,41 +449,56 @@
             'message':"save_location: ",
             'long_instruction': 'Where would you like to set as the root save downloaded directory?',
             'default':config.get_save_location(config_),
             "filter":lambda x:prompt_validators.cleanTextInput(x),
             "validate": PathValidator(is_dir=True)
         },
         {
-            'type': 'number',
+            'type': 'input',
             'name': 'file_size_limit',
             'message':"file_size_limit: ",
             'long_instruction':
 """
-File size limit (enter a value in bytes)
+File size limit
+input can be int representing bytes
+or human readable such as 10mb
 Enter 0 for no limit
 """,
-            'default': config.get_filesize(config_),
+            'default': str(config.get_filesize_limit(config_)),
+            'filter':int,
+      
+        },
+
+    {
+            'type': 'input',
+            'name': 'file_size_min',
+            'message':"file_size_min: ",
+            'long_instruction':
+"""
+File size min
+input can be int representing bytes
+or human readable such as 10mb
+Enter 0 for no minimum
+""",
+            'default': str(config.get_filesize_min(config_)),
             'filter':int,
-             'min_allowed':0,
       
         },
            {
             'type': 'input',
             'name': 'dir_format',
             'message':"dir_format: ",
             'long_instruction': 'What format do you want for download directories',
-            'default': config.get_dirformat(config_),
-             "validate":prompt_validators.dirformatvalidator()
+            'default': config.get_dirformat(config_)
         },
               {
             'type': 'input',
             'name': 'file_format',
             'message': 'What format do you want for downloaded files',
             'default':config.get_fileformat(config_),
-             "validate":prompt_validators.fileformatvalidator()
         },
                      {
             'type': 'number',
             'name': 'textlength',
             'message':"textlength: ",
             'long_instruction': 'Enter the max length to extract for post text, 0 means unlimited\n',
             'default': config.get_textlength(config_),
@@ -463,33 +523,22 @@
         },
         {
             'type': 'input',
             'name': 'metadata',
             "message":"metadata: ",
             'long_instruction': 'Where should metadata files be saved',
             'default':config.get_metadata(config_),
-             "validate":prompt_validators.metadatavalidator()
         },
         {
             'type': 'checkbox',
             'name': 'filter',
             "message":"filter: ",
             'choices':list(map(lambda x:Choice(name=x,value=x, enabled=x.capitalize() in set(config.get_filter(config_))),constants.FILTER_DEFAULT)),
              "validate":prompt_validators.emptyListValidator()
         },
-        {
-            'type': 'number',
-            'name': 'threads',
-            "message":"Number of Download Theads: ",
-            'min_allowed':1,
-            'max_allowed':10,
-             "validate":EmptyInputValidator(),
-             'long_instruction':"Value can be 1-10",
-             'default':config.get_threads(config_),
-        },
           {
             'type': 'list',
             'name':"code-execution",
             'message': "Enable Code Execution:",
             'choices':[Choice(True,"Yes"),Choice(False,"No",enabled=True)],
             "default":config.get_allow_code_execution(config_),
             "long_instruction":"Be careful if turning this on this only effects file_format,metadata, and dir_format"
@@ -810,15 +859,15 @@
 
      
             {
             'type': 'list',
             "name":"subscription",
             'message': "Filter accounts by the type of subscription",
              "default":False,
-            'choices':[Choice("paid","Paid Subscription Only"),Choice("free","Free Subscription Only"),Choice(False,"Both")]
+            'choices':[Choice("paid","Paid Subscriptions Only"),Choice("free","Free Subscriptions Only"),Choice(False,"Both")]
         }
     ])
     args.renewal=answer["renewal"]
     args.sub_status=answer["expire"]
     args.account_type=answer["subscription"]
     return args
 
@@ -888,15 +937,15 @@
 def reset_auth_prompt() -> bool:
     name="input"
     questions = promptClasses.batchConverter(*[
         {
             'type': 'list',
             "name":name,
             'message': "How do you want to fix this issue",
-            'choices':[Choice(False,"Reset Default"),Choice(True,"Manually Auth Config")]
+            'choices':[Choice("Reset Default","Reset Default"),Choice("Manually Edit Auth Config","Manually Edit Auth Config")]
         }
     ])
     return questions[name]
 
 def manual_config_prompt(configText) -> str:
     name="input"
     
@@ -907,15 +956,15 @@
         
         {
               
             'type': 'input',
             'multiline':True,
             "name":name,
             'default':configText,
-            "keys":prompt_strings.CONFIG_MULTI,
+            "long_message":prompt_strings.CONFIG_MULTI,
             'message': "Edit config text\n===========\n",
         }
     ])
 
     return questions[name]
 def manual_auth_prompt(authText) -> str:
     name="input"
@@ -928,15 +977,15 @@
         {
                
             "name":name,
             'type': 'input',
             'multiline':True,
             'default':authText,
             'message': "Edit auth text\n===========\n",
-            "keys":prompt_strings.AUTH_MULTI,
+            "long_message":prompt_strings.AUTH_MULTI,
             "validate":EmptyInputValidator()
         }
     ])
 
 
     return questions[name]
```

### Comparing `ofscraper-2.7.9/ofscraper/utils/args.py` & `ofscraper-3.0/ofscraper/utils/args.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import argparse
-import logging
 import sys
 import re
 import arrow
 import pathlib
+from humanfriendly import parse_size
 from ofscraper.__version__ import __version__ 
-
+import ofscraper.constants as constants
 args=None
-log=logging.getLogger(__package__)
 def create_parser(input=None):
     parent_parser=argparse.ArgumentParser(add_help=False)
     general=parent_parser.add_argument_group("Program",description="Program Args")  
     general.add_argument('-v', '--version', action='version', version=__version__ ,default=__version__)
     general.add_argument(
         '-cg', '--config', help="Change location of config folder/file",default=None
     )
@@ -77,33 +76,38 @@
     post.add_argument(
         '-dt', '--download-type', help = 'Filter to what type of download you want None==Both, protected=Files that need mp4decrpyt',default=None,required=False,type=str.lower,choices=["protected","normal"]
     )
 
     post.add_argument(
         '-lb', '--label', help = 'Filter by label',default=None,required=False,type=label_helper,action="extend"
     )
+    post.add_argument(
+        '-be', '--before', help = 'Process post at or before the given date general synax is Month/Day/Year\nWorks for like,unlike, and downloading posts',type=arrow_helper)
+    post.add_argument(
+        '-af', '--after', help = 'Process post at or after the given date Month/Day/Year\nnWorks for like,unlike, and downloading posts',type=arrow_helper)
+    post.add_argument(
+        '-mt', '--mediatype', help = 'Filter by media',default=[],required=False,type = posttype_helper,action='extend')
    
-
+    post.add_argument(
+        '-sx', '--size-max', help = 'Filter out files greater then given size supported inputs include int in bytes or human-readable such as 10mb',required=False,type = parse_size)
+    post.add_argument(
+        '-sm', '--size-min', help = 'Filter out files greater smaller then the given size bytes or human-readable such as 10mb',required=False,type =parse_size)
      #Filters for accounts
     filters=parser.add_argument_group("filters",description="Filters out usernames based on selected parameters")
     
     filters.add_argument(
         '-at', '--account-type', help = 'Filter Free or paid accounts\npaid and free correspond to your original price, and not the renewal price',default=None,required=False,type = str.lower,choices=["paid","free"]
     )
     filters.add_argument(
         '-rw', '--renewal', help = 'Filter by whether renewal is on or off for account',default=None,required=False,type = str.lower,choices=["active","disabled"]
     )
     filters.add_argument(
         '-ss', '--sub-status', help = 'Filter by whether or not your subscription has expired or not',default=None,required=False,type = str.lower,choices=["active","expired"]
     )
-    filters.add_argument(
-        '-be', '--before', help = 'Process post at or before the given date general synax is Month/Day/Year\nWorks for like,unlike, and downloading posts',type=arrow_helper)
- 
-    filters.add_argument(
-        '-af', '--after', help = 'Process post at or after the given date Month/Day/Year\nnWorks for like,unlike, and downloading posts',type=arrow_helper)
+
     
     
     sort=parser.add_argument_group("sort",description="Options on how to sort list")
     sort.add_argument(
         '-st', '--sort', help = 'What to sort the model list by',default="Name",choices=["name","subscribed","expiring","price"],type=str.lower)
     sort.add_argument(
         '-ds', '--desc', help = 'Sort the model list in descending order',action="store_true",default=False) 
@@ -112,22 +116,26 @@
     advanced.add_argument(
         '-uf', '--users-first', help = 'Scrape all users first rather then one at a time. This only effects downloading posts',default=False,required=False,action="store_true"
     )
     advanced.add_argument(
         '-nc', '--no-cache', help = 'disable cache',default=False,required=False,action="store_true"
     )
     advanced.add_argument(
-        '-k', '--key-mode', help = 'key mode override',default=None,required=False,choices=["cdrm","manual","keydb"],type=str.lower)
+        '-k', '--key-mode', help = 'key mode override',default=None,required=False,choices=constants.KEY_OPTIONS,type=str.lower)
     advanced.add_argument(
         '-dr', '--dynamic-rules', help = 'Dynamic signing',default=None,required=False,choices=["dc","deviint"],type=str.lower)
     advanced.add_argument(
         '-pc', '--part-cleanup', help = 'Cleanup temp .part files\nNote this removes the ability to resume from downloads',default=False,action="store_true")
 
-    
-    
+    advanced.add_argument(
+        '-db', '--downloadbars', help = 'show individual download progress bars',default=False,action="store_true")
+
+    advanced.add_argument('-sd', '--downloadsems', help = 'Number of sems or concurrent downloads per thread',default=None,type=int)
+
+    advanced.add_argument('-dp', '--downloadthreads', help = 'Number threads to use minimum will always be 1, Maximmum will never be higher then max availible-1',default=None,type=int)
     
     
     
     subparser=parser.add_subparsers(help="commands",dest="command")
     post_check=subparser.add_parser("post_check",help="Display a generated table of data with information about models post(s)\nCache lasts for 24 hours",parents=[parent_parser])
 
 
@@ -199,27 +207,34 @@
     global args
     if args and input==None:
         return args
     if "pytest" in sys.modules and input==None:
         input=[]
     elif input==None:
         input=sys.argv[1:]
+
+
     parser=create_parser(input)
+
     args=parser.parse_args(input)
+ 
+
     #deduplicate posts
     args.posts=list(set(args.posts or []))
     args.username=set(args.username or [])
     args.excluded_username=set( args.excluded_username or [])
     args.label=set(args.label) if args.label else args.label
 
 
     if args.command in set(["post_check","msg_check"])and not (args.url or args.file):
         raise argparse.ArgumentTypeError("error: argument missing --url or --file must be specified )")
-    if args.command in set(["story_check","paid_check"])and not (args.username or args.file):
+    elif args.command in set(["story_check","paid_check"])and not (args.username or args.file):
         raise argparse.ArgumentTypeError("error: argument missing --username or --file must be specified )")
+    elif args.command in set(["manual"])and not (args.url or args.file):
+        raise argparse.ArgumentTypeError("error: argument missing --url or --file must be specified )")
     return args
 
 
 
 
 def check_strhelper(x):
     temp=None
@@ -241,26 +256,35 @@
     if isinstance(x,str):
         x=x.split(',')
         x=list(map(lambda x:x.capitalize() ,x))
     if len(list(filter(lambda y: y not in choices,x)))>0:
         raise argparse.ArgumentTypeError("error: argument -o/--posts: invalid choice: (choose from 'highlights', 'all', 'archived', 'messages', 'timeline', 'pinned', 'stories', 'purchased','profile','labels')")
     return x
 
+def mediatype_helper():
+    choices=set(["Videos","Music","Audio"])
+    if isinstance(x,str):
+        x=x.split(',')
+        x=list(map(lambda x:x.capitalize() ,x))
+    if len(list(filter(lambda y: y not in choices,x)))>0:
+        raise argparse.ArgumentTypeError("error: argument -o/--posts: invalid choice: (choose from 'highlights', 'all', 'archived', 'messages', 'timeline', 'pinned', 'stories', 'purchased','profile','labels')")
+    return x
 def changeargs(newargs):
     global args
     args=newargs
 
 
 def username_helper(x):
     temp=None
     if isinstance(x,list):
         temp=x
     elif isinstance(x,str):
         temp=x.split(",")
-    return temp
+    
+    return list(map(lambda x:x.lower(),temp))
 def label_helper(x):
     temp=None
     if isinstance(x,list):
         temp=x
     elif isinstance(x,str):
         temp=x.split(",")
     return list(map(lambda x:x.lower(),temp))
```

### Comparing `ofscraper-2.7.9/ofscraper/utils/auth.py` & `ofscraper-3.0/ofscraper/utils/auth.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,22 +13,24 @@
 import time
 import logging
 from urllib.parse import urlparse
 import requests
 from rich.console import Console
 
 import browser_cookie3
+from tenacity import retry,stop_after_attempt,retry_if_not_exception_type,wait_fixed
 
 import ofscraper.prompts.prompts as prompts
 from ..constants import configPath, DIGITALCRIMINALS, requestAuth,DEVIINT
 import ofscraper.utils.paths as paths
 import ofscraper.classes.sessionbuilder as sessionbuilder
 import ofscraper.utils.profiles as profiles
 import ofscraper.utils.args as args_
 import ofscraper.utils.config as config
+import ofscraper.constants as constants
 
 
 console=Console()
 log=logging.getLogger("shared")
 
 def read_auth():
     authFile=paths.get_auth_file()
@@ -45,15 +47,15 @@
                         break
             break
         except FileNotFoundError:
             console.print(
                 "You don't seem to have an `auth.json` file")
             make_auth()
         except json.JSONDecodeError as e:
-            print("You auth.json has a syntax error")
+            print("Your auth.json has a syntax error")
             print(f"{e}\n\n")
             if prompts.reset_auth_prompt():
                 with open( authFile, 'w') as f:
                     f.write(prompts.manual_auth_prompt(authText))
             else:
                 with open(authFile,"w") as f: 
                     f.write(json.dumps(get_empty()))
@@ -89,27 +91,26 @@
     except FileNotFoundError:
         
         if prompts.ask_make_auth_prompt():
             make_auth()
     except json.JSONDecodeError as e:
             while True:
                 try:
-                    print("You auth.json has a syntax error")
-                    print(f"{e}\n\n")
-                    if prompts.reset_auth_prompt():
+                    print("Your auth.json has a syntax error")
+                    if prompts.reset_auth_prompt()=="Reset Default":
+                        make_auth()
+                    else:
                         with open( authFile, 'w') as f:
                             f.write(prompts.manual_auth_prompt(authText))
-                    else:
-                         with open(authFile,"w"): 
-                            f.write(prompts.auth_prompt(get_empty()))
+
                     with open(authFile, 'r') as f:
                         authText=f.read()
                         auth = json.loads(authText)
                     break
-                except:
+                except Exception as E:
                     continue
     make_request_auth() 
 
 def make_auth( auth=None):
     authFile=paths.get_auth_file()
     defaultAuth=  get_empty()
 
@@ -129,33 +130,31 @@
 
  
     elif browserSelect=="Paste From M-rcus\' OnlyFans-Cookie-Helper":
         auth=prompts.auth_full_paste()
         auth["auth"]["app-token"]="33d57ade8c02dbc5a333db99ff9ae26a"
         for key in ["username","support_2fa","active","email","password","hashed"]:
             auth["auth"].pop(key)
-        auth["auth"]["x-bc"]=auth["auth"].pop("x_bc")
+        auth["auth"]["x-bc"]=auth["auth"].pop("x_bc").strip()
         tempCookie=auth["auth"].pop("cookie")
         for ele in tempCookie.split(";"):
-            ele=ele.strip(
-                
-            )
             if ele.find("auth_id")!=-1:
                 auth["auth"]["auth_id"]=ele.replace("auth_id=","")
             elif ele.find("sess")!=-1:
                 auth["auth"]["sess"]=ele.replace("sess=","")
             elif ele.find("auth_uid")!=-1:
                 auth["auth"]["auth_uid_"]=ele.replace("auth_uid_","").replace("=","")
-           
+
 
 
     else:
         console.print("You'll need to go to onlyfans.com and retrive header information\nGo to https://github.com/datawhores/OF-Scraper and find the section named 'Getting Your Auth Info'\nYou only need to retrive the x-bc header,the user-agent, and cookie information",style="yellow")
         auth['auth'].update(prompts.auth_prompt(auth['auth']))
-    
+    for item in auth["auth"].items():
+        auth[item[0]]=item[1].strip()
     console.print(f"{auth}\nWriting to {authFile}",style="yellow")
     with open(authFile, 'w') as f:
         f.write(json.dumps(auth, indent=4))
 
 
 
 
@@ -272,32 +271,33 @@
 
 def get_request_auth():
     if (args_.getargs().dynamic_rules or config.get_dynamic(config.read_config()) or "deviint")=="deviint":
         return get_request_auth_deviint()
     else:
         return get_request_digitalcriminals()
 
+@retry(retry=retry_if_not_exception_type(KeyboardInterrupt),stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_fixed(8))
 def get_request_auth_deviint():
     with sessionbuilder.sessionBuilder(backend="httpx",set_header=False,set_cookies=False,set_sign=False) as c:
         with c.requests(DEVIINT)() as r:
             if r.ok:
                 content = r.json_()
                 static_param = content['static_param']
                 fmt = f"{content['start']}:{{}}:{{:x}}:{content['end']}" 
                 checksum_indexes = content['checksum_indexes']
                 checksum_constant = content['checksum_constant']
                 return (static_param, fmt, checksum_indexes, checksum_constant)
             else:
-                return []
-        
+               r.raise_for_status()  
+@retry(retry=retry_if_not_exception_type(KeyboardInterrupt),stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_fixed(8))  
 def get_request_digitalcriminals():
    with sessionbuilder.sessionBuilder(backend="httpx",set_header=False,set_cookies=False,set_sign=False) as c:
         with c.requests(DIGITALCRIMINALS)() as r:
             if r.ok:
                 content = r.json_()
                 static_param = content['static_param']
                 fmt = content['format']
                 checksum_indexes = content['checksum_indexes']
                 checksum_constant = content['checksum_constant']
                 return (static_param, fmt, checksum_indexes, checksum_constant)
             else:
-                return []
+                r.raise_for_status()
```

### Comparing `ofscraper-2.7.9/ofscraper/utils/binaries.py` & `ofscraper-3.0/ofscraper/utils/binaries.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.9/ofscraper/utils/config.py` & `ofscraper-3.0/ofscraper/utils/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,17 +12,18 @@
 import pathlib
 import logging
 import ofscraper.constants as constants
 import ofscraper.prompts.prompts as prompts 
 import ofscraper.utils.binaries as binaries
 import ofscraper.utils.paths as paths_
 import ofscraper.utils.console as console_
+from humanfriendly import parse_size
 
-console=console_.shared_console
-log=logging.getLogger(__package__)
+console=console_.get_shared_console()
+log=logging.getLogger("shared")
 
 def get_config_folder():
     out=paths_.get_config_path().parent
     out.mkdir(exist_ok=True,parents=True)
     return out
 
 def read_config():
@@ -67,15 +68,16 @@
     if config:
         config = config['config']
 
     new_config = {
         'config': {
             constants.mainProfile: get_main_profile(config),
             'save_location':get_save_location(config) ,
-            'file_size_limit': get_filesize(config),
+            'file_size_limit': get_filesize_limit(config),
+            'file_size_min': get_filesize_min(config),
             'dir_format': get_dirformat(config),
             'file_format':get_fileformat(config),
             'textlength':get_textlength(config),
             'space-replacer':get_spacereplacer(config),
             'date': get_date(config),
             "metadata": get_metadata(config),
             "filter":get_filter(config),
@@ -84,18 +86,20 @@
             "custom":get_custom(config),
             "mp4decrypt":get_mp4decrypt(config),
             "ffmpeg":get_ffmpeg(config),
              "discord":get_discord(config),
              "private-key":get_private_key(config),
              "client-id":get_client_id(config),
             "key-mode-default":get_key_mode(config),
-              "keydb_api":get_keydb_api(config),
+            "keydb_api":get_keydb_api(config),
             "dynamic-mode-default":get_dynamic(config),
             "partfileclean":get_part_file_clean(config),
             "backend":get_backend(config),
+            "download-sems":get_download_semaphores(config),
+            "downloadbars":get_show_downloadprogress(config),
 
             "responsetype":{
            "timeline":get_timeline_responsetype(config),
          "message":get_messages_responsetype(config),
             "archived":get_archived_responsetype(config),
             "paid":get_paid_responsetype(config),
             "stories":get_stories_responsetype(config),
@@ -232,19 +236,28 @@
     return config.get('save_location') or constants.SAVE_PATH_DEFAULT
 
 def get_main_profile(config=None):
     if config==None:
         return constants.PROFILE_DEFAULT   
     return config.get('main_profile',constants.PROFILE_DEFAULT)
 
-def get_filesize(config=None):
+def get_filesize_limit(config=None):
     if config==None:
-        return constants.FILE_SIZE_DEFAULT      
+        return constants.FILE_SIZE_LIMIT_DEFAULT      
     try:
-        return int(config.get('file_size_limit', constants.FILE_SIZE_DEFAULT))
+        return parse_size(config.get('file_size_limit', constants.FILE_SIZE_LIMIT_DEFAULT  ))
+    except:
+        return 0
+
+
+def get_filesize_min(config=None):
+    if config==None:
+        return constants.FILE_SIZE_MIN_DEFAULT       
+    try:
+        return parse_size(config.get('file_size_limit', constants.FILE_SIZE_MIN_DEFAULT  ))
     except:
         return 0
 
 def get_dirformat(config=None):
     if config==None:
         return constants.DIR_FORMAT_DEFAULT     
     return config.get('dir_format', constants.DIR_FORMAT_DEFAULT)
@@ -272,15 +285,15 @@
     return config.get('code-execution', constants.CODE_EXECUTION_DEFAULT)
 def get_metadata(config=None):
     if config==None:
         return constants.METADATA_DEFAULT      
     return config.get('metadata', constants.METADATA_DEFAULT)
 def get_threads(config=None):
     if config==None:
-        return constants.MP4DECRYPT_DEFAULT    
+        return constants.THREADS_DEFAULT  
     return int(config.get('threads', constants.THREADS_DEFAULT) or constants.THREADS_DEFAULT)
 
 def get_mp4decrypt(config=None):
     if config==None:
         return constants.MP4DECRYPT_DEFAULT    
     return config.get('mp4decrypt', constants.MP4DECRYPT_DEFAULT) or ""
 
@@ -370,27 +383,40 @@
         return None 
     return config.get('client-id')
 
 def get_key_mode(config=None):
     if config==None:
         return constants.KEY_DEFAULT
     value=config.get("key-mode-default")
-    return value.lower() if value and value.lower() in set(["keydb","manual","cdrm"]) else constants.KEY_DEFAULT
+    return value.lower() if value and value.lower() in set(constants.KEY_OPTIONS) else constants.KEY_DEFAULT
 def get_keydb_api(config=None):
     if config==None:
         return ""
     return config.get("keydb_api","") or ""
 def get_dynamic(config=None):
     if config==None:
         return constants.DYNAMIC_DEFAULT
     value=config.get("dynamic-mode-default")
-    return value.lower() if value and value.lower() in set(["deviint","dc"]) else "deviint"
+    return value.lower() if value and value.lower() in set(["deviint","digitalcriminals"]) else "deviint"
 def get_part_file_clean(config=None):
     if config==None:
         return False
     return config.get("partfileclean",False) or False
 
 
 def get_backend(config=None):
     if config==None:
         return "aio"
     return config.get("backend",constants.BACKEND_DEFAULT) or constants.BACKEND_DEFAULT
+
+def get_download_semaphores(config=None):
+    if config==None:
+        return constants.DOWNLOAD_SEM_DEFAULT
+    try:
+        return int(config.get('download-sems', constants.DOWNLOAD_SEM_DEFAULT))
+    except:
+        return constants.DOWNLOAD_SEM_DEFAULT
+    
+def get_show_downloadprogress(config):
+    if config==None:
+        return constants.PROGRESS_DEFAULT
+    return config.get("downloadbars",constants.PROGRESS_DEFAULT) or constants.PROGRESS_DEFAULT
```

### Comparing `ofscraper-2.7.9/ofscraper/utils/dates.py` & `ofscraper-3.0/ofscraper/utils/dates.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.9/ofscraper/utils/exit.py` & `ofscraper-3.0/ofscraper/utils/exit.py`

 * *Files 26% similar despite different names*

```diff
@@ -71,7 +71,24 @@
                 return
             # elif self._propagate_to_forked_processes is True:
             #   ... passthrough
 
         print(f'!!! DelayedKeyboardInterrupt._handler: {SIGNAL_TRANSLATION_MAP[sig]} received; delaying KeyboardInterrupt')
 
 
+def exit_wrapper(func): 
+    def inner(*args,**kwargs): 
+        try:
+
+            func(*args,**kwargs)
+        except KeyboardInterrupt as E:
+            with DelayedKeyboardInterrupt():
+                raise KeyboardInterrupt
+        except KeyboardInterrupt:
+            raise KeyboardInterrupt
+        except Exception as E:
+            try:
+                with DelayedKeyboardInterrupt():
+                    raise E
+            except KeyboardInterrupt:
+                  raise KeyboardInterrupt  
+    return inner
```

### Comparing `ofscraper-2.7.9/ofscraper/utils/filters.py` & `ofscraper-3.0/ofscraper/utils/filters.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 
 import logging
 import re
 import arrow
 import ofscraper.utils.config as config
 import ofscraper.utils.args as args_
 
-args=args_.getargs()
-log=logging.getLogger(__package__)
+log=logging.getLogger("shared")
 def filterMedia(media):
     logformater="{} data: {} id: {} postid: {}"
     []
     log.trace("\n\n\n".join(list(map(lambda x: logformater.format("filter 1-> all media no filter:",x.media,x.id,x.postid),media))))
     log.debug(f"filter 1-> all media no filter count: {len(media)}")
     media=dupefilter(media)
     log.trace("\n\n\n".join(list(map(lambda x: logformater.format("filter 2-> all media dupe filter: ",x.media,x.id,x.postid),media))))
@@ -62,18 +61,18 @@
 
     
 def timeline_array_filter(posts):
     out=[]
     undated=list(filter(lambda x:x.get("postedAt")==None,posts))
     dated=list(filter(lambda x:x.get("postedAt")!=None,posts))
     dated=sorted(dated,key=lambda x:arrow.get(x.get("postedAt")))
-    if args.before:
-        dated=list(filter(lambda x:arrow.get(x.get("postedAt"))<=args.before,dated))
-    if args.after:
-         dated=list(filter(lambda x:arrow.get(x.get("postedAt"))>=args.after,dated))
+    if args_.getargs().before:
+        dated=list(filter(lambda x:arrow.get(x.get("postedAt"))<=args_.getargs().before,dated))
+    if args_.getargs().after:
+         dateargsd=list(filter(lambda x:arrow.get(x.get("postedAt"))>=args_.getargs().after,dated))
     out.extend(undated)
     out.extend(dated)
     return out
 def posts_type_filter(media): 
     filtersettings=config.get_filter(config.read_config())
     if isinstance(filtersettings,str):
         filtersettings=filtersettings.split(",")
@@ -86,33 +85,33 @@
         media =list(filter(lambda x:x.mediatype.lower() in filtersettings,media))
     else:
         log.info("The settings you picked for the filter are not valid\nNot Filtering")
         log.debug(f"[bold]Combined Media Count Filtered:[/bold] {len(media)}")
     return media
 
 def posts_date_filter(media):
-    if args.before:
-        media=list(filter(lambda x:x.postdate==None or arrow.get(x.postdate)<=args.before,media))
-    if args.after:
-        media=list(filter(lambda x:x.postdate==None or arrow.get(x.postdate)>=args.after,media))
+    if args_.getargs().before:
+        media=list(filter(lambda x:x.postdate==None or arrow.get(x.postdate)<=args_.getargs().before,media))
+    if args_.getargs().after:
+        media=list(filter(lambda x:x.postdate==None or arrow.get(x.postdate)>=args_.getargs().after,media))
     return media
 
 def post_timed_filter(media):
-    if args.skip_timed:
+    if args_.getargs().skip_timed:
         return list(filter(lambda x:not x.expires,media))
     return media
 def post_user_filter(media):
-    userfilter=args.filter
+    userfilter=args_.getargs().filter
     if not userfilter.islower():
         return list(filter(lambda x:re.search(userfilter,x.text or "")!=None,media))
     else:
         return list(filter(lambda x:re.search(userfilter,x.text or "",re.IGNORECASE)!=None,media))
 
 def anti_post_user_filter(media):
-    userfilter=args.neg_filter
+    userfilter=args_.getargs().neg_filter
     if not userfilter.islower():
         return list(filter(lambda x:re.search(userfilter,x.text or "")==None,media)) if userfilter else media
     else:
         return list(filter(lambda x:re.search(userfilter,x.text or "",re.IGNORECASE)==None,media)) if userfilter else media
```

### Comparing `ofscraper-2.7.9/ofscraper/utils/logger.py` & `ofscraper-3.0/ofscraper/utils/logger.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,34 @@
 import logging
 import re
 import logging
 import threading
 import time
 import queue
+import types
+
+from logging.handlers import QueueHandler
 from rich.logging import RichHandler
 
-from tenacity import retry,stop_after_attempt,wait_fixed
 
+from tenacity import retry,stop_after_attempt,retry_if_not_exception_type,wait_fixed
+import aioprocessing
 import ofscraper.utils.paths as paths
 import ofscraper.utils.config as config_
 import ofscraper.utils.args as args
 import ofscraper.utils.console as console
 import ofscraper.constants as constants
 import ofscraper.classes.sessionbuilder as sessionbuilder
-senstiveDict={}
-discord_queue=queue.Queue()
+import ofscraper.utils.console as console_
 
+queue_=aioprocessing.AioQueue()
+otherqueue_=aioprocessing.AioQueue()
+
+senstiveDict={}
+process=""
 
 class DebugOnly(logging.Filter):
     def filter(self, record):
 
         if record.levelno==10 or record.levelno==11:
             return True
         return False
@@ -35,24 +43,31 @@
     def filter(self, record):
         if record.levelno<=11:
             return False
         return True
 class DiscordHandler(logging.Handler):
     def __init__(self):
         logging.Handler.__init__(self)
+        self.sess=sessionbuilder.sessionBuilder(backend="httpx",set_header=False,set_cookies=False,set_sign=False)
     def emit(self, record):
+        @retry(retry=retry_if_not_exception_type(KeyboardInterrupt),stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_fixed(8))
+        def inner(sess):
+            with sess:
+                with sess.requests(url,"post",headers={"Content-type": "application/json"},json={"content":log_entry})() as r:
+                    if not r.status==204:
+                        raise Exception
+
         log_entry = self.format(record)
         url=config_.get_discord(config_.read_config())
+        log_entry=re.sub("\[bold\]|\[/bold\]","**",log_entry)
         log_entry=f"{log_entry}\n\n"
         if url==None or url=="":
             return
-        #convert markup
-        log_entry=re.sub("\[bold\]|\[/bold\]","**",log_entry)
-        discord_queue.put((url,log_entry))
-
+        inner(self.sess)
+    
 
 
 class TextHandler(logging.Handler):
     def __init__(self):
         logging.Handler.__init__(self)
         self._widget=None
     def emit(self, record):
@@ -66,46 +81,14 @@
     @property
     def widget(self):
         return self._widget
     @widget.setter
     def widget(self,widget):
         self._widget=widget
 
-
-def discord_messenger():
-    with sessionbuilder.sessionBuilder(backend="httpx",set_header=False,set_cookies=False,set_sign=False) as c:
-        while True:
-            if args.getargs().discord==None:
-                break
-            url,message=discord_queue.get()   
-            if url=="exit":
-                return
-            try:
-                discord_pusher(url,message,c)
-            except Exception as E:
-                console.shared_console.print("Discord Error")
-
-@retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_fixed(constants.DISCORDWAIT),reraise=True) 
-def discord_pusher(url,message,c):
-    with c.requests(url,"post",headers={"Content-type": "application/json"},json={"content":message})() as r:
-        None
-
-
-
-def discord_cleanup():
-    logging.getLogger("ofscraper").info("Pushing Discord Queue")
-    while True:
-        if discord_queue.empty:
-            discord_queue.put(("exit",None))
-            break
-        time.sleep(.5)
-             
-def start_discord_queue():
-    worker_thread = threading.Thread(target=discord_messenger)
-    worker_thread.start()
 class SensitiveFormatter(logging.Formatter):
     """Formatter that removes sensitive information in logs."""
     @staticmethod
     def _filter(s):
         if s.find("Avatar :")!=-1:
             None
         else:
@@ -182,57 +165,199 @@
             "STATS":"ERROR",
             "LOW":"WARNING",
             "NORMAL":"INFO",
             "DEBUG":"DEBUG",
             "TRACE":"TRACE"
             
             }.get(input,100)
+def getNumber(input_):
+    input_=getLevel(input_)
+    if isinstance(input_,str):return logging.getLevelName(input_)
+    return input_
 
-def init_logger(log):
+def init_main_logger(name):
+    log=logging.getLogger(name or "ofscraper")
     format=' \[%(module)s.%(funcName)s:%(lineno)d]  %(message)s'
     log.setLevel(1)
     addtraceback()
     addtrace()
     # # #log file
       # #discord
-    cord=DiscordHandler()
-    cord.setLevel(getLevel(args.getargs().discord))
-    cord.setFormatter(SensitiveFormatter('%(message)s'))
     #console
-    sh=RichHandler(rich_tracebacks=True,markup=True,tracebacks_show_locals=True,show_time=False,show_level=False,console=console.shared_console)
+    sh=RichHandler(rich_tracebacks=True,markup=True,tracebacks_show_locals=True,show_time=False,show_level=False,console=console.get_shared_console())
     sh.setLevel(getLevel(args.getargs().output))
     sh.setFormatter(SensitiveFormatter(format))
     sh.addFilter(NoDebug())
     tx=TextHandler()
     tx.setLevel(getLevel(args.getargs().output))
     tx.setFormatter(SensitiveFormatter(format))
-    log.addHandler(cord)
     log.addHandler(sh)
     log.addHandler(tx)
-    if args.getargs().log!="OFF":
-        stream=open(paths.getlogpath(), encoding='utf-8',mode="a",)
-        fh=logging.StreamHandler(stream)
-        fh.setLevel(getLevel(args.getargs().log))
-        fh.setFormatter(LogFileFormatter('%(asctime)s - %(message)s',"%Y-%m-%d %H:%M:%S"))
-        fh.addFilter(NoDebug())
-        log.addHandler(fh)
 
-    
     if args.getargs().output in {"TRACE","DEBUG"}:
         funct=DebugOnly if args.getargs().output=="DEBUG" else TraceOnly
-        sh2=RichHandler(rich_tracebacks=True, console=console.shared_console,markup=True,tracebacks_show_locals=True,show_time=False)
+        sh2=RichHandler(rich_tracebacks=True, console=console.get_shared_console(),markup=True,tracebacks_show_locals=True,show_time=False)
         sh2.setLevel(args.getargs().output)
         sh2.setFormatter(SensitiveFormatter(format))
         sh2.addFilter(funct())
         log.addHandler(sh2)
+
+    return log
+
+def init_other_logger(name):
+    name=name or "other"
+    log=logging.getLogger(name)
+    format=' \[%(module)s.%(funcName)s:%(lineno)d]  %(message)s'
+    log.setLevel(1)
+    addtraceback()
+    addtrace()
+    # # #log file
+      # #discord
+    cord=DiscordHandler()
+    cord.setLevel(getLevel(args.getargs().discord))
+    cord.setFormatter(SensitiveFormatter('%(message)s'))
+    #console
+    log.addHandler(cord)
+    if args.getargs().log!="OFF":
+        stream=open(paths.getlogpath(), encoding='utf-8',mode="a",)
+        fh=logging.StreamHandler(stream)
+        fh.setLevel(getLevel(args.getargs().log))
+        fh.setFormatter(LogFileFormatter('%(asctime)s - %(message)s',"%Y-%m-%d %H:%M:%S"))
+        fh.addFilter(NoDebug())
+        log.addHandler(fh)
     if args.getargs().log in {"TRACE","DEBUG"}:
         funct=DebugOnly if args.getargs().output=="DEBUG" else TraceOnly
         fh2=logging.StreamHandler(stream)
         fh2.setLevel(getLevel(args.getargs().log))
         fh2.setFormatter(LogFileFormatter('%(asctime)s - %(levelname)s - %(message)s',"%Y-%m-%d %H:%M:%S"))
         fh2.addFilter(funct())
         log.addHandler(fh2)
     return log
 
-
 def add_widget(widget):
     [setattr(ele,"widget",widget) for ele in list(filter(lambda x:isinstance(x,TextHandler),logging.getLogger("ofscraper").handlers))]
+
+
+
+
+
+
+#mulitprocess
+# executed in a process that performs logging
+def logger_process(input_,name=None,stop_count=1,event=None):
+    # create a logger
+    log=init_main_logger(name)
+    input_=input_ or queue_
+    count=0
+    close=False
+    while True:
+        # consume a log message, block until one arrives
+        if event and event.is_set():
+            return
+        messages = input_.get()
+        if not isinstance(messages,list):
+            messages=[messages]
+        for message in messages:
+            # check for shutdown
+            if event and event.is_set():
+                close=True
+            #set close value
+            if message=="None" :
+                close=True
+                continue    
+            if message.message=="None":
+                count=count+1
+         
+            if count==stop_count:
+                close=True
+            if message.message!="None":
+                # log the message
+                log.handle(message)
+        # check close and empty message
+        if close==True:
+            return
+
+
+
+#mulitprocess
+# executed in a process that performs logging
+def logger_other(input_,name=None,stop_count=1,event=None):
+    # create a logger
+    log=init_other_logger(name)
+    count=0
+    close=False
+    if len(list(filter(lambda x:x.level!=100,log.handlers)))==0:
+        return
+    while True:
+        # consume a log message, block until one arrives
+        if event and event.is_set():
+           return True
+        messages = input_.get()
+        if not isinstance(messages,list):
+            messages=[messages]
+        for message in messages:
+            #set close value
+            if event and event.is_set():
+                close=True
+            if message=="None":
+                close=True
+                continue    
+            if message.message=="None":
+                count=count+1
+         
+            if count==stop_count:
+                close=True
+            if message.message!="None":
+                # log the message
+                log.handle(message)
+        # check close and empty message
+        if close==True:
+            return
+
+
+# some inherantence from main process
+def start_stdout_logthread(input_=None,name=None,count=1,event=None):
+    input_=input_ or queue_
+    thread= threading.Thread(target=logger_process,args=(input_,name,count,event),daemon=True)
+    thread.start()
+
+
+    return thread
+
+
+def start_other_thread(input_=None,name=None,count=1,event=None):
+    input_=input_ or otherqueue_
+    thread= threading.Thread(target=logger_other,args=(input_,name,count,event),daemon=True)
+    thread.start()
+    return thread
+    
+def start_other_process(input_=None,name=None,count=1):
+    def inner(input_=None,name=None,count=1):
+        thread=start_other_thread(input_=None,name=None,count=1)
+        thread.join()
+        time.sleep(10)
+    process=aioprocessing.AioProcess(target=inner,args=(input_,name,count)) if (args.getargs().log or args.getargs().discord) else None
+    process.start() if process else None
+    return process 
+
+    
+
+
+
+def get_shared_logger(main_=None ,other_=None,name=None):
+    # create a logger
+    logger = logging.getLogger(name or 'shared')
+    addtraceback()
+    addtrace()
+    main_queue=QueueHandler(main_ or queue_)
+    main_queue.setLevel(getLevel(args.getargs().output))
+    # add a handler that uses the shared queue
+    logger.addHandler(main_queue)
+    discord_level=getNumber(args.getargs().discord); 
+    file_level=getNumber(args.getargs().log); 
+    other_queue=QueueHandler((other_ or otherqueue_))
+    other_queue.setLevel(min(file_level,discord_level))
+    logger.addHandler(other_queue)  
+    # log all messages, debug and up
+    logger.setLevel(1)
+    return logger
+
```

### Comparing `ofscraper-2.7.9/ofscraper/utils/of.py` & `ofscraper-3.0/ofscraper/utils/of.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,17 +26,15 @@
 import ofscraper.utils.filters as filters
 import ofscraper.utils.stdout as stdout
 import ofscraper.api.archive as archive
 import ofscraper.api.pinned as pinned
 import ofscraper.api.labels as labels_api
 import ofscraper.classes.labels as labels
 
-log=logging.getLogger(__package__)
-args=args_.getargs()
-log.debug(args)
+log=logging.getLogger("shared")
 
 def process_messages(model_id,username):
     with stdout.lowstdout():
         messages_ =asyncio.run(messages.get_messages(  model_id)) 
         messages_=list(map(lambda x:posts_.Post(x,model_id,username),messages_))
         log.debug(f"[bold]Messages Media Count with locked[/bold] {sum(map(lambda x:len(x.post_media),messages_))}")
         log.debug("Removing locked messages media")
@@ -179,17 +177,18 @@
         for labelled_post in labelled_posts_:
             operations.write_labels_table(labelled_post, model_id, username)
 
         output = [post.media for labelled_post in labelled_posts_ for post in labelled_post.posts]
         return [item for sublist in output for item in sublist]
 
 def select_areas():
-    if not args.scrape_paid and len( args.posts or [])==0:
+    args=args_.getargs()
+    if not args_.getargs().scrape_paid and len( args_.getargs().posts or [])==0:
           args.scrape_paid=prompts.scrape_paid_prompt()
-    args.posts = list(map(lambda x:x.capitalize(),(args.posts or prompts.areas_prompt())
+    args.posts = list(map(lambda x:x.capitalize(),(args_.getargs().posts or prompts.areas_prompt())
 ))
 
     args_.changeargs(args)
      
 def process_areas(ele, model_id) -> list:
     select_areas()
     timeline_posts_dicts  = []
@@ -200,36 +199,36 @@
     stories_dicts=[]
     purchased_dict=[]
     pinned_post_dict=[]
     profile_dicts=[]
     labels_dicts=[]
 
     username=ele['name']
-    if "Skip" in args.posts:
+    if "Skip" in args_.getargs().posts:
         return []
   
-    if ('Profile' in args.posts or 'All' in args.posts):
+    if ('Profile' in args_.getargs().posts or 'All' in args_.getargs().posts):
         profile_dicts  = process_profile(username)
-    if ('Pinned' in args.posts or 'All' in args.posts):
+    if ('Pinned' in args_.getargs().posts or 'All' in args_.getargs().posts):
             pinned_post_dict = process_pinned_posts(model_id,username)
-    if ('Timeline' in args.posts or 'All' in args.posts):
+    if ('Timeline' in args_.getargs().posts or 'All' in args_.getargs().posts):
             timeline_posts_dicts = process_timeline_posts( model_id,username)
-    if ('Archived' in args.posts or 'All' in args.posts):
+    if ('Archived' in args_.getargs().posts or 'All' in args_.getargs().posts):
             archived_posts_dicts = process_archived_posts( model_id,username)
-    if 'Messages' in args.posts or 'All' in args.posts:
+    if 'Messages' in args_.getargs().posts or 'All' in args_.getargs().posts:
             messages_dicts = process_messages( model_id,username)
-    if "Purchased" in args.posts or "All" in args.posts:
+    if "Purchased" in args_.getargs().posts or "All" in args_.getargs().posts:
             purchased_dict=process_paid_post(model_id,username)
-    if 'Highlights'  in args.posts or 'All' in args.posts:
+    if 'Highlights'  in args_.getargs().posts or 'All' in args_.getargs().posts:
             highlights_dicts = process_highlights( model_id,username)  
-    if 'Stories'  in args.posts or 'All' in args.posts:
+    if 'Stories'  in args_.getargs().posts or 'All' in args_.getargs().posts:
             stories_dicts = process_stories( model_id,username)         
             
             
 
-    if ("Labels" in args.posts or "All" in args.posts) and ele["active"]:
+    if ("Labels" in args_.getargs().posts or "All" in args_.getargs().posts) and ele["active"]:
         labels_dicts = process_labels(model_id,username)             
     return filters.filterMedia(list(chain(*[profile_dicts  , timeline_posts_dicts ,pinned_post_dict,purchased_dict,
             archived_posts_dicts , highlights_dicts , messages_dicts,stories_dicts, labels_dicts]))
 
 )
```

### Comparing `ofscraper-2.7.9/ofscraper/utils/paths.py` & `ofscraper-3.0/ofscraper/utils/paths.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,17 +16,17 @@
 import ofscraper.utils.args as args_
 import ofscraper.utils.console as console_
 from .profiles import get_current_config_profile
 import ofscraper.api.me as me
 
 
 
-console=console_.shared_console
+console=console_.get_shared_console()
 homeDir=pathlib.Path.home()
-log=logging.getLogger(__package__)
+log=logging.getLogger("shared")
 
 
 
 
 
 @contextmanager
 def set_directory(path: Path):
@@ -44,14 +44,15 @@
     createDir(Path(str(path)))
     try:
         os.chdir(path)
         yield
     finally:
         os.chdir(origin)
 def createDir(path):
+    path=pathlib.Path(path)
     try:
         path.mkdir(exist_ok=True,parents=True)
     except:
         log.info("Error creating directory, check the directory and make sure correct permissions have been issued.")
 
        
 
@@ -74,62 +75,65 @@
             file.unlink(missing_ok=True)
 
 
 
 def getcachepath():
     profile = get_profile_path()
     path= profile/"cache"
+    path=pathlib.Path(os.path.normpath(path))
     createDir(path.parent)
     return path
 def truncate(path):
+    path=pathlib.Path(os.path.normpath(path))
     if args_.getargs().original:
         return path
     if platform.system() == 'Windows':
         return _windows_truncateHelper(path)
     elif platform.system() == 'Linux':
         return _linux_truncateHelper(path)
     elif platform.system() == 'Darwin':
         return _mac_truncateHelper(path)
     else:
         return pathlib.Path(path)
 def _windows_truncateHelper(path):
+    path=pathlib.Path(os.path.normpath(path))
     if len(str(path))<=256:
         return path
     path=pathlib.Path(path)
     dir=path.parent
     file=path.name
-    match=re.search("_[0-9]+\.[a-z]*$",path.name,re.IGNORECASE) or re.search("\.[a-z]*$",path.name,re.IGNORECASE)
+    match=re.search("_[0-9]+\.[a-z4]*$",path.name,re.IGNORECASE) or re.search("\.[a-z4]*$",path.name,re.IGNORECASE)
     if match:
         ext=match.group(0)
     else:
         ext=""
     #-1 is for / between parentdirs and file
     fileLength=256-len(ext)-len(str(dir))-1
     newFile=f"{re.sub(ext,'',file)[fileLength]}{ext}"
     final=pathlib.Path(dir,newFile)
     log.debug(f"path: {final} path size: {len(str(final))}")
     return pathlib.Path(dir,newFile)
 
 def _mac_truncateHelper(path):
-    path=pathlib.Path(path)
+    path=pathlib.Path(os.path.normpath(path))
     dir=path.parent
-    match=re.search("_[0-9]+\.[a-z]*$",path.name,re.IGNORECASE) or re.search("\.[a-z]*$",path.name,re.IGNORECASE)
+    match=re.search("_[0-9]+\.[a-z4]*$",path.name,re.IGNORECASE) or re.search("\.[a-z4]*$",path.name,re.IGNORECASE)
     ext= match.group(0) if match else ""
     file=re.sub(ext,"",path.name)
     maxlength=255-len(ext)
     newFile=f"{file[:maxlength]}{ext}"
     final=pathlib.Path(dir,newFile)
     log.debug(f"path: {final} path size: {len(str(final))}")
     log.debug(f"path: {final} filename size: {len(str(final.name))}")
     return pathlib.Path(dir,newFile)
 
 def _linux_truncateHelper(path):
-    path=pathlib.Path(path)
+    path=pathlib.Path(os.path.normpath(path))
     dir=path.parent
-    match=re.search("_[0-9]+\.[a-z]*$",path.name,re.IGNORECASE) or re.search("\.[a-z]*$",path.name,re.IGNORECASE)
+    match=re.search("_[0-9]+\.[a-z4]*$",path.name,re.IGNORECASE) or re.search("\.[a-z4]*$",path.name,re.IGNORECASE)
     ext= match.group(0) if match else ""
     file=re.sub(ext,"",path.name)
     maxbytes=254-len(ext.encode('utf8'))
     small=0
     large=len(file)
     target=None
     maxLength=254-len(ext)
@@ -193,14 +197,15 @@
     except Exception as E:
         patched_print(E)
         patched_print(traceback.format_exc())
         return False  
    
 def getlogpath():
     path= get_config_home() / "logging"/f'ofscraper_{config_.get_main_profile()}_{arrow.now().format("YYYY-MM-DD")}.log'
+    path=pathlib.Path(os.path.normpath(path))
     createDir(path.parent)
     return path
 
 def get_config_path():
     configPath=args_.getargs().config
     defaultPath=pathlib.Path.home() / constants.configPath/constants.configFile
     ofscraperHome=pathlib.Path.home() / constants.configPath
```

### Comparing `ofscraper-2.7.9/ofscraper/utils/profiles.py` & `ofscraper-3.0/ofscraper/utils/profiles.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import ofscraper.utils.config as config_
 import ofscraper.prompts.prompts as prompts
 import ofscraper.constants as constants
 import ofscraper.utils.paths as paths_
 import ofscraper.utils.args as args_
 
 
-log=logging.getLogger(__package__)
+log=logging.getLogger("shared")
 console=Console()
 currentData=None
 currentProfile=None
 
        
 
 def get_my_info():
@@ -32,15 +32,15 @@
     global currentProfile
     if currentProfile==get_active_profile():
         return currentData
     else:
         import ofscraper.utils.auth as auth_
         import ofscraper.api.me as me
         currentProfile=get_active_profile()
-        currentData= me.scrape_user(  auth_.make_headers(auth_.read_auth()))
+        currentData= me.scrape_user()
     return currentData
 
 
 
 
 def create_profile_path(name=None):
     out=paths_.get_profile_path(name)
```

### Comparing `ofscraper-2.7.9/ofscraper/utils/separate.py` & `ofscraper-3.0/ofscraper/utils/separate.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,25 +5,25 @@
  /  _ \   __\/  ___// ___\_  __ \__  \  /  _ \_/ __ \_  __ \
 (  <_> )  |  \___ \\  \___|  | \// __ \(  <_> )  ___/|  | \/
  \____/|__| /____  >\___  >__|  (____  /\____/ \___  >__|   
                  \/     \/           \/            \/         
 """
 from ..utils.paths import getcachepath
 from diskcache import Cache
-cache = Cache(getcachepath())
 
 
 def separate_by_id(data: list, media_ids: list) -> list:
     media_ids=set(media_ids)
     return list(filter(lambda x:x.id not in media_ids,data ))
 
 def seperate_avatars(data):
     return list(filter(lambda x:seperate_avatar_helper(x)==False,data))
 
 def seperate_avatar_helper(ele):
+    cache = Cache(getcachepath())
     #id for avatar comes from xxh32 of url
     if  ele.postid and ele.responsetype_=="profile":
         value=cache.get(ele.postid ,False)
         cache.close()
         return value
     return False
```

### Comparing `ofscraper-2.7.9/ofscraper/utils/userselector.py` & `ofscraper-3.0/ofscraper/utils/userselector.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,57 +18,58 @@
 import ofscraper.utils.stdout as stdout
 
 
 
 
 ALL_SUBS=None
 PARSED_SUBS=None
-log=logging.getLogger(__package__)
-args=args_.getargs()
+log=logging.getLogger("shared")
 
 def getselected_usernames(rescan=False,reset=False):
     #username list will be retrived every time reset==True
     global ALL_SUBS
     global PARSED_SUBS
-    if "Skip" in args.posts:
+
+    if "Skip" in args_.getargs().posts:
         return []
     if reset==True and PARSED_SUBS:
         if prompts.reset_username_prompt()=="Yes":
            PARSED_SUBS=None
-           args.username=None
+           args_.getargs().username=None
            args_.changeargs(args)
     if rescan==True:
         PARSED_SUBS=None
-    if not PARSED_SUBS or not args.username:
+    if not PARSED_SUBS or not args_.getargs().username:
         all_subs_helper()
         parsed_subscriptions_helper()
     return PARSED_SUBS
 
 
  
     
 def all_subs_helper(): 
-    headers = auth.make_headers(auth.read_auth())
-    subscribe_count = process_me(headers)
+    subscribe_count = process_me()
     global ALL_SUBS
     ALL_SUBS= get_models( subscribe_count)
 
 
 def parsed_subscriptions_helper(force=False):
     global ALL_SUBS
     global PARSED_SUBS
-    if not args.username:
+    global args
+    args= args_.getargs()
+    if not args_.getargs().username:
         selectedusers=get_model(ALL_SUBS)
-        args.username=list(map(lambda x:x["name"],selectedusers))
+        args_.getargs().username=list(map(lambda x:x["name"],selectedusers))
         PARSED_SUBS=selectedusers
         args_.changeargs(args)  
-    elif "ALL" in args.username:
+    elif "ALL" in args_.getargs().username:
         PARSED_SUBS=filterNSort(ALL_SUBS)
-    elif args.username:
-        usernameset=set(args.username)
+    elif args_.getargs().username:
+        usernameset=set(args_.getargs().username)
         PARSED_SUBS=list(filter(lambda x:x["name"] in usernameset,ALL_SUBS))
     return PARSED_SUBS
         
        
 
 def setfilter():
     if prompts.decide_filters_prompt()=="Yes":
@@ -84,62 +85,62 @@
 def filterNSort(usernames):
 
 
     #paid/free
     filterusername=usernames
     log.debug(f"username count no filters: {len(filterusername)}")
     dateNow=arrow.now()
-    if args.account_type=="paid":
+    if args_.getargs().account_type=="paid":
         filterusername=list(filter(lambda x:(x.get("price") or 0)>0,filterusername))
         log.debug(f"+paid filter username count: {len(filterusername)}")
 
-    elif args.account_type=="free":
+    elif args_.getargs().account_type=="free":
         filterusername=list(filter(lambda x:(x.get("price") or 0)==0,filterusername))    
         log.debug(f"+free filter username count: {len(filterusername)}")
     
-    if args.renewal=="active":
+    if args_.getargs().renewal=="active":
         filterusername=list(filter(lambda x:x.get("renewed")!=None,filterusername))
         log.debug(f"+active renewal filter username count: {len(filterusername)}")
 
-    elif args.renewal=="disabled":
+    elif args_.getargs().renewal=="disabled":
         filterusername=list(filter(lambda x:x.get("renewed")==None,filterusername))  
         log.debug(f"+disabled renewal filter username count: {len(filterusername)}")
 
-    if args.sub_status=="active":
+    if args_.getargs().sub_status=="active":
         filterusername=list(filter(lambda x:x.get("subscribed")!=None,filterusername)) 
         log.debug(f"+active subscribtion filter username count: {len(filterusername)}")
 
-    elif args.sub_status=="expired":
+    elif args_.getargs().sub_status=="expired":
         filterusername=list(filter(lambda x:x.get("subscribed")==None,filterusername))
         log.debug(f"+expired subscribtion filter username count: {len(filterusername)}")
 
-    filterusername=list(filter(lambda x:x["name"] not in args.excluded_username ,filterusername))
+    filterusername=list(filter(lambda x:x["name"] not in args_.getargs().excluded_username ,filterusername))
     log.debug(f"final username count with all filters: {len(filterusername)}")
     if len(filterusername)==0:
         raise Exception("You have filtered the user list to zero\nPlease Select less restrictive filters")
     return sort_models_helper(filterusername)      
 
 
 
 def sort_models_helper(models):
-    sort=args.sort
-    reverse=args.desc
+    sort=args_.getargs().sort
+    reverse=args_.getargs().desc
     if sort=="name":
         return sorted(models,reverse=reverse, key=lambda x:x["name"])
     elif sort=="expired":
         return sorted(models,reverse=reverse, key=lambda x:arrow.get(x.get("expired") or 0).float_timestamp)
     elif sort=="subscribed":
         return sorted(models,reverse=reverse, key=lambda x:arrow.get(x.get("subscribed") or 0).float_timestamp)
     elif sort=="price":
         return sorted(models,reverse=reverse, key=lambda x:x.get("price") or 0)
     else:
         return sorted(models,reverse=reverse, key=lambda x:x["name"])
 #check if auth is valid
-def process_me(headers):
-    my_profile = me.scrape_user(headers)
+def process_me():
+    my_profile = me.scrape_user()
     name, username = me.parse_user(my_profile)
     subscribe_count=me.parse_subscriber_count()
     me.print_user(name, username)
     return subscribe_count
 
 def get_models(subscribe_count) -> list:
     """
```

### Comparing `ofscraper-2.7.9/pyproject.toml` & `ofscraper-3.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "ofscraper"
-version = "2.7.9"
+version = "3.0"
 description = "automatically scrape onlyfans"
 authors = ["datawhores <datawhores@riseup.net>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = ">=3.7.0,<3.12"
+python = ">3.7.0,<3.12"
 httpx = {extras = ["http2"], version = "^0.23.3"}
 inquirerpy = "^0.3.4"
 setuptools = "^67.6.0"
 schedule = "^1.1.0"
 browser-cookie3 = "^0.17.1"
 requests = "^2.28.2"
 bs4 = "^0.0.1"
@@ -26,29 +26,32 @@
 dunamai = "^1.17.0"
 poetry-dynamic-versioning = "^0.22.0"
 textual = "^0.27.0"
 aiohttp = {extras = ["speedups"], version = "^3.8.4"}
 faust-cchardet = "^2.1.18"
 certifi = "^2023.5.7"
 aiosqlite = "^0.19.0"
-pywidevine = "^1.6.0"
-aiomultiprocess = "^0.9.0"
 pycryptodome = "^3.18.0"
+pywidevine = "^1.6.0"
+aioprocessing = {extras = ["dill"], version = "^2.0.1"}
+more-itertools = "^9.1.0"
+psutil = "^5.9.5"
+pytest = "^7.4.0"
+humanfriendly = "^10.0"
 
 
 [tool.poetry.group.dev.dependencies]
 autopep8 = "^2.0.2"
 
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.1"
-pytest-check = { version = "2.1.4", python = ">3.7" }
 coverage = "^7.2.3"
 pytest-cov = "^4.0.0"
 pytest-mock = "^3.10.0"
 random-unicode-emoji = "^2.8"
 random-emoji = "^1.0.15"
 
 
@@ -57,28 +60,31 @@
 
 [tool.poetry.group.docs.dependencies]
 sphinx-argparse = "^0.4.0"
 
 
 [tool.poetry.group.testing.dependencies]
 coverage = "^7.2.7"
+pytest = "^7.4.0"
+pytest-check = "^2.2.0"
+random-unicode-emoji = "^2.8"
 
 
 [tool.poetry.group.build.dependencies]
 pyinstaller = "^5.13.0"
+pytest-check = "^2.2.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry.scripts]
-ofscraper = "ofscraper.start:main"
+ofscraper = "ofscraper.__main__:main"
+
 
-[project.scripts]
-ofscraper = "ofscraper.start:main"
 
 [tool.poetry.urls]
 "Homepage" = "https://github.com/datawhores/OF-Scraper"
 
 # pyproject.toml
 [tool.pytest.ini_options]
 minversion = "6.0"
@@ -88,8 +94,8 @@
 ]
 
 [tool.poetry-dynamic-versioning]
 enable = true
 vcs="git"
 metadata=true
 format="{base}"
-pattern = "(?P<base>\\d+\\.\\d+\\.\\d+|\\d+\\.\\d+)"
+pattern = "(?P<base>\\d+\\.\\d+\\.\\w+|\\d+\\.\\w+)"
```

### Comparing `ofscraper-2.7.9/PKG-INFO` & `ofscraper-3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 Metadata-Version: 2.1
 Name: ofscraper
-Version: 2.7.9
+Version: 3.0
 Summary: automatically scrape onlyfans
 Author: datawhores
 Author-email: datawhores@riseup.net
-Requires-Python: >=3.7.0,<3.12
+Requires-Python: >3.7.0,<3.12
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp[speedups] (>=3.8.4,<4.0.0)
-Requires-Dist: aiomultiprocess (>=0.9.0,<0.10.0)
+Requires-Dist: aioprocessing[dill] (>=2.0.1,<3.0.0)
 Requires-Dist: aiosqlite (>=0.19.0,<0.20.0)
 Requires-Dist: arrow (>=1.2.3,<2.0.0)
 Requires-Dist: browser-cookie3 (>=0.17.1,<0.18.0)
 Requires-Dist: bs4 (>=0.0.1,<0.0.2)
 Requires-Dist: certifi (>=2023.5.7,<2024.0.0)
 Requires-Dist: diskcache (>=5.6.1,<6.0.0)
 Requires-Dist: dunamai (>=1.17.0,<2.0.0)
 Requires-Dist: faust-cchardet (>=2.1.18,<3.0.0)
 Requires-Dist: ffmpeg-python (>=0.2.0,<0.3.0)
 Requires-Dist: httpx[http2] (>=0.23.3,<0.24.0)
+Requires-Dist: humanfriendly (>=10.0,<11.0)
 Requires-Dist: inquirerpy (>=0.3.4,<0.4.0)
+Requires-Dist: more-itertools (>=9.1.0,<10.0.0)
 Requires-Dist: mpegdash (>=0.3.1,<0.4.0)
 Requires-Dist: pathvalidate (>=2.5.2,<3.0.0)
 Requires-Dist: poetry-dynamic-versioning (>=0.22.0,<0.23.0)
+Requires-Dist: psutil (>=5.9.5,<6.0.0)
 Requires-Dist: pycryptodome (>=3.18.0,<4.0.0)
+Requires-Dist: pytest (>=7.4.0,<8.0.0)
 Requires-Dist: pywidevine (>=1.6.0,<2.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: rich (>=13.3.2,<14.0.0)
 Requires-Dist: schedule (>=1.1.0,<2.0.0)
 Requires-Dist: setuptools (>=67.6.0,<68.0.0)
 Requires-Dist: tenacity (>=8.2.2,<9.0.0)
 Requires-Dist: textual (>=0.27.0,<0.28.0)
@@ -79,15 +82,17 @@
   command-line program to download media, and to process other batch operations such as liking and unliking posts.
     
 
 ![CopyQ nsUBdI](https://user-images.githubusercontent.com/67020411/227816586-fb685959-cd3f-45af-adea-14773b7154f9.png)
 
 # Issues
 Open a issue in this repo, or you can mention your issue in the discord
-https://discord.gg/DV3aBeMu
+https://discord.gg/wN7uxEVHRK
+
+
     
 # Feature Requests
 
 https://ofscraper.clearflask.com/feedback
     
 Or the discord
```

