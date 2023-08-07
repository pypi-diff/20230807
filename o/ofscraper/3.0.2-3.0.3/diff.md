# Comparing `tmp/ofscraper-3.0.2.tar.gz` & `tmp/ofscraper-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofscraper-3.0.2.tar", max compression
+gzip compressed data, was "ofscraper-3.0.3.tar", max compression
```

## Comparing `ofscraper-3.0.2.tar` & `ofscraper-3.0.3.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0     1067 2023-08-07 07:03:39.961010 ofscraper-3.0.2/LICENSE
--rw-r--r--   0        0        0     2863 2023-08-07 07:03:39.961010 ofscraper-3.0.2/README.md
--rwxr-xr-x   0        0        0      254 2023-08-07 07:03:39.965010 ofscraper-3.0.2/ofscraper/__main__.py
--rw-r--r--   0        0        0     1016 2023-08-07 07:03:39.965010 ofscraper-3.0.2/ofscraper/__version__.py
--rw-r--r--   0        0        0      999 2023-08-07 07:03:39.965010 ofscraper-3.0.2/ofscraper/__version__.pye
--rw-r--r--   0        0        0     8736 2023-08-07 07:03:39.965010 ofscraper-3.0.2/ofscraper/api/archive.py
--rw-r--r--   0        0        0     9895 2023-08-07 07:03:39.965010 ofscraper-3.0.2/ofscraper/api/highlights.py
--rw-r--r--   0        0        0     1029 2023-08-07 07:03:39.965010 ofscraper-3.0.2/ofscraper/api/init.py
--rw-r--r--   0        0        0     7568 2023-08-07 07:03:39.965010 ofscraper-3.0.2/ofscraper/api/labels.py
--rw-r--r--   0        0        0     2946 2023-08-07 07:03:39.965010 ofscraper-3.0.2/ofscraper/api/me.py
--rw-r--r--   0        0        0     9518 2023-08-07 07:03:39.965010 ofscraper-3.0.2/ofscraper/api/messages.py
--rw-r--r--   0        0        0     9687 2023-08-07 07:03:39.965010 ofscraper-3.0.2/ofscraper/api/paid.py
--rw-r--r--   0        0        0     5730 2023-08-07 07:03:39.965010 ofscraper-3.0.2/ofscraper/api/pinned.py
--rw-r--r--   0        0        0     4497 2023-08-07 07:03:39.965010 ofscraper-3.0.2/ofscraper/api/profile.py
--rw-r--r--   0        0        0     3384 2023-08-07 07:03:39.965010 ofscraper-3.0.2/ofscraper/api/subscriptions.py
--rw-r--r--   0        0        0     9312 2023-08-07 07:03:39.965010 ofscraper-3.0.2/ofscraper/api/timeline.py
--rw-r--r--   0        0        0      804 2023-08-07 07:03:39.965010 ofscraper-3.0.2/ofscraper/classes/labels.py
--rw-r--r--   0        0        0     8779 2023-08-07 07:03:39.965010 ofscraper-3.0.2/ofscraper/classes/media.py
--rw-r--r--   0        0        0     1795 2023-08-07 07:03:39.965010 ofscraper-3.0.2/ofscraper/classes/multiprocessprogress.py
--rw-r--r--   0        0        0     8068 2023-08-07 07:03:39.965010 ofscraper-3.0.2/ofscraper/classes/placeholder.py
--rw-r--r--   0        0        0     3734 2023-08-07 07:03:39.969010 ofscraper-3.0.2/ofscraper/classes/posts.py
--rw-r--r--   0        0        0     4849 2023-08-07 07:03:39.969010 ofscraper-3.0.2/ofscraper/classes/sessionbuilder.py
--rw-r--r--   0        0        0    29784 2023-08-07 07:03:39.969010 ofscraper-3.0.2/ofscraper/classes/table.py
--rw-r--r--   0        0        0    14816 2023-08-07 07:03:39.969010 ofscraper-3.0.2/ofscraper/commands/check.py
--rw-r--r--   0        0        0     5347 2023-08-07 07:03:39.969010 ofscraper-3.0.2/ofscraper/commands/manual.py
--rwxr-xr-x   0        0        0    15354 2023-08-07 07:03:39.969010 ofscraper-3.0.2/ofscraper/commands/scraper.py
--rw-r--r--   0        0        0     7244 2023-08-07 07:03:39.969010 ofscraper-3.0.2/ofscraper/constants.py
--rw-r--r--   0        0        0        1 2023-08-07 07:03:39.969010 ofscraper-3.0.2/ofscraper/db/__init__.py
--rw-r--r--   0        0        0    10129 2023-08-07 07:03:39.969010 ofscraper-3.0.2/ofscraper/db/operations.py
--rw-r--r--   0        0        0     3576 2023-08-07 07:03:39.969010 ofscraper-3.0.2/ofscraper/db/queries.py
--rw-r--r--   0        0        0        1 2023-08-07 07:03:39.969010 ofscraper-3.0.2/ofscraper/interaction/__init__.py
--rw-r--r--   0        0        0     4851 2023-08-07 07:03:39.969010 ofscraper-3.0.2/ofscraper/interaction/like.py
--rw-r--r--   0        0        0      773 2023-08-07 07:03:39.969010 ofscraper-3.0.2/ofscraper/prompts/keybindings.py
--rw-r--r--   0        0        0     6241 2023-08-07 07:03:39.969010 ofscraper-3.0.2/ofscraper/prompts/promptConvert.py
--rw-r--r--   0        0        0     7227 2023-08-07 07:03:39.969010 ofscraper-3.0.2/ofscraper/prompts/prompt_strings.py
--rw-r--r--   0        0        0     7848 2023-08-07 07:03:39.969010 ofscraper-3.0.2/ofscraper/prompts/prompt_validators.py
--rw-r--r--   0        0        0    30797 2023-08-07 07:03:39.969010 ofscraper-3.0.2/ofscraper/prompts/prompts.py
--rw-r--r--   0        0        0     3430 2023-08-07 07:03:39.969010 ofscraper-3.0.2/ofscraper/start.py
--rw-r--r--   0        0        0        1 2023-08-07 07:03:39.969010 ofscraper-3.0.2/ofscraper/utils/__init__.py
--rw-r--r--   0        0        0    14071 2023-08-07 07:03:39.969010 ofscraper-3.0.2/ofscraper/utils/args.py
--rw-r--r--   0        0        0    10511 2023-08-07 07:03:39.969010 ofscraper-3.0.2/ofscraper/utils/auth.py
--rw-r--r--   0        0        0     8977 2023-08-07 07:03:39.969010 ofscraper-3.0.2/ofscraper/utils/binaries.py
--rw-r--r--   0        0        0    14736 2023-08-07 07:03:39.969010 ofscraper-3.0.2/ofscraper/utils/config.py
--rw-r--r--   0        0        0      395 2023-08-07 07:03:39.969010 ofscraper-3.0.2/ofscraper/utils/console.py
--rw-r--r--   0        0        0     1080 2023-08-07 07:03:39.969010 ofscraper-3.0.2/ofscraper/utils/dates.py
--rw-r--r--   0        0        0    41374 2023-08-07 07:03:39.969010 ofscraper-3.0.2/ofscraper/utils/download.py
--rw-r--r--   0        0        0      609 2023-08-07 07:03:39.969010 ofscraper-3.0.2/ofscraper/utils/encoding.py
--rw-r--r--   0        0        0     3386 2023-08-07 07:03:39.969010 ofscraper-3.0.2/ofscraper/utils/exit.py
--rw-r--r--   0        0        0     5665 2023-08-07 07:03:39.969010 ofscraper-3.0.2/ofscraper/utils/filters.py
--rw-r--r--   0        0        0    11133 2023-08-07 07:03:39.969010 ofscraper-3.0.2/ofscraper/utils/logger.py
--rw-r--r--   0        0        0      189 2023-08-07 07:03:39.969010 ofscraper-3.0.2/ofscraper/utils/misc.py
--rw-r--r--   0        0        0    10913 2023-08-07 07:03:39.969010 ofscraper-3.0.2/ofscraper/utils/of.py
--rw-r--r--   0        0        0     7251 2023-08-07 07:03:39.969010 ofscraper-3.0.2/ofscraper/utils/paths.py
--rw-r--r--   0        0        0     4221 2023-08-07 07:03:39.969010 ofscraper-3.0.2/ofscraper/utils/profiles.py
--rw-r--r--   0        0        0      399 2023-08-07 07:03:39.969010 ofscraper-3.0.2/ofscraper/utils/semaphoreDelayed.py
--rw-r--r--   0        0        0     1215 2023-08-07 07:03:39.969010 ofscraper-3.0.2/ofscraper/utils/separate.py
--rw-r--r--   0        0        0      893 2023-08-07 07:03:39.969010 ofscraper-3.0.2/ofscraper/utils/stdout.py
--rw-r--r--   0        0        0     5773 2023-08-07 07:03:39.969010 ofscraper-3.0.2/ofscraper/utils/userselector.py
--rw-r--r--   0        0        0     2073 2023-08-07 07:04:11.865269 ofscraper-3.0.2/pyproject.toml
--rw-r--r--   0        0        0     4720 1970-01-01 00:00:00.000000 ofscraper-3.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-08-07 08:06:06.166521 ofscraper-3.0.3/LICENSE
+-rw-r--r--   0        0        0     2863 2023-08-07 08:06:06.166521 ofscraper-3.0.3/README.md
+-rwxr-xr-x   0        0        0      254 2023-08-07 08:06:06.174522 ofscraper-3.0.3/ofscraper/__main__.py
+-rw-r--r--   0        0        0     1016 2023-08-07 08:06:06.174522 ofscraper-3.0.3/ofscraper/__version__.py
+-rw-r--r--   0        0        0      999 2023-08-07 08:06:06.174522 ofscraper-3.0.3/ofscraper/__version__.pye
+-rw-r--r--   0        0        0     8736 2023-08-07 08:06:06.174522 ofscraper-3.0.3/ofscraper/api/archive.py
+-rw-r--r--   0        0        0     9895 2023-08-07 08:06:06.174522 ofscraper-3.0.3/ofscraper/api/highlights.py
+-rw-r--r--   0        0        0     1029 2023-08-07 08:06:06.174522 ofscraper-3.0.3/ofscraper/api/init.py
+-rw-r--r--   0        0        0     7568 2023-08-07 08:06:06.174522 ofscraper-3.0.3/ofscraper/api/labels.py
+-rw-r--r--   0        0        0     2946 2023-08-07 08:06:06.174522 ofscraper-3.0.3/ofscraper/api/me.py
+-rw-r--r--   0        0        0     9518 2023-08-07 08:06:06.174522 ofscraper-3.0.3/ofscraper/api/messages.py
+-rw-r--r--   0        0        0     9687 2023-08-07 08:06:06.174522 ofscraper-3.0.3/ofscraper/api/paid.py
+-rw-r--r--   0        0        0     5730 2023-08-07 08:06:06.174522 ofscraper-3.0.3/ofscraper/api/pinned.py
+-rw-r--r--   0        0        0     4497 2023-08-07 08:06:06.174522 ofscraper-3.0.3/ofscraper/api/profile.py
+-rw-r--r--   0        0        0     3384 2023-08-07 08:06:06.174522 ofscraper-3.0.3/ofscraper/api/subscriptions.py
+-rw-r--r--   0        0        0     9312 2023-08-07 08:06:06.174522 ofscraper-3.0.3/ofscraper/api/timeline.py
+-rw-r--r--   0        0        0      804 2023-08-07 08:06:06.174522 ofscraper-3.0.3/ofscraper/classes/labels.py
+-rw-r--r--   0        0        0     8779 2023-08-07 08:06:06.174522 ofscraper-3.0.3/ofscraper/classes/media.py
+-rw-r--r--   0        0        0     1795 2023-08-07 08:06:06.174522 ofscraper-3.0.3/ofscraper/classes/multiprocessprogress.py
+-rw-r--r--   0        0        0     8068 2023-08-07 08:06:06.174522 ofscraper-3.0.3/ofscraper/classes/placeholder.py
+-rw-r--r--   0        0        0     3734 2023-08-07 08:06:06.174522 ofscraper-3.0.3/ofscraper/classes/posts.py
+-rw-r--r--   0        0        0     4849 2023-08-07 08:06:06.174522 ofscraper-3.0.3/ofscraper/classes/sessionbuilder.py
+-rw-r--r--   0        0        0    29784 2023-08-07 08:06:06.174522 ofscraper-3.0.3/ofscraper/classes/table.py
+-rw-r--r--   0        0        0    14816 2023-08-07 08:06:06.174522 ofscraper-3.0.3/ofscraper/commands/check.py
+-rw-r--r--   0        0        0     5347 2023-08-07 08:06:06.174522 ofscraper-3.0.3/ofscraper/commands/manual.py
+-rwxr-xr-x   0        0        0    15354 2023-08-07 08:06:06.174522 ofscraper-3.0.3/ofscraper/commands/scraper.py
+-rw-r--r--   0        0        0     7244 2023-08-07 08:06:06.174522 ofscraper-3.0.3/ofscraper/constants.py
+-rw-r--r--   0        0        0        1 2023-08-07 08:06:06.174522 ofscraper-3.0.3/ofscraper/db/__init__.py
+-rw-r--r--   0        0        0    10129 2023-08-07 08:06:06.174522 ofscraper-3.0.3/ofscraper/db/operations.py
+-rw-r--r--   0        0        0     3576 2023-08-07 08:06:06.174522 ofscraper-3.0.3/ofscraper/db/queries.py
+-rw-r--r--   0        0        0        1 2023-08-07 08:06:06.174522 ofscraper-3.0.3/ofscraper/interaction/__init__.py
+-rw-r--r--   0        0        0     4851 2023-08-07 08:06:06.174522 ofscraper-3.0.3/ofscraper/interaction/like.py
+-rw-r--r--   0        0        0      773 2023-08-07 08:06:06.174522 ofscraper-3.0.3/ofscraper/prompts/keybindings.py
+-rw-r--r--   0        0        0     6241 2023-08-07 08:06:06.174522 ofscraper-3.0.3/ofscraper/prompts/promptConvert.py
+-rw-r--r--   0        0        0     7227 2023-08-07 08:06:06.174522 ofscraper-3.0.3/ofscraper/prompts/prompt_strings.py
+-rw-r--r--   0        0        0     7848 2023-08-07 08:06:06.174522 ofscraper-3.0.3/ofscraper/prompts/prompt_validators.py
+-rw-r--r--   0        0        0    30797 2023-08-07 08:06:06.174522 ofscraper-3.0.3/ofscraper/prompts/prompts.py
+-rw-r--r--   0        0        0     3430 2023-08-07 08:06:06.174522 ofscraper-3.0.3/ofscraper/start.py
+-rw-r--r--   0        0        0        1 2023-08-07 08:06:06.174522 ofscraper-3.0.3/ofscraper/utils/__init__.py
+-rw-r--r--   0        0        0    14071 2023-08-07 08:06:06.174522 ofscraper-3.0.3/ofscraper/utils/args.py
+-rw-r--r--   0        0        0    10511 2023-08-07 08:06:06.174522 ofscraper-3.0.3/ofscraper/utils/auth.py
+-rw-r--r--   0        0        0     8977 2023-08-07 08:06:06.174522 ofscraper-3.0.3/ofscraper/utils/binaries.py
+-rw-r--r--   0        0        0    14736 2023-08-07 08:06:06.174522 ofscraper-3.0.3/ofscraper/utils/config.py
+-rw-r--r--   0        0        0      395 2023-08-07 08:06:06.174522 ofscraper-3.0.3/ofscraper/utils/console.py
+-rw-r--r--   0        0        0     1080 2023-08-07 08:06:06.174522 ofscraper-3.0.3/ofscraper/utils/dates.py
+-rw-r--r--   0        0        0    41373 2023-08-07 08:06:06.178522 ofscraper-3.0.3/ofscraper/utils/download.py
+-rw-r--r--   0        0        0      609 2023-08-07 08:06:06.178522 ofscraper-3.0.3/ofscraper/utils/encoding.py
+-rw-r--r--   0        0        0     3386 2023-08-07 08:06:06.178522 ofscraper-3.0.3/ofscraper/utils/exit.py
+-rw-r--r--   0        0        0     5665 2023-08-07 08:06:06.178522 ofscraper-3.0.3/ofscraper/utils/filters.py
+-rw-r--r--   0        0        0    11133 2023-08-07 08:06:06.178522 ofscraper-3.0.3/ofscraper/utils/logger.py
+-rw-r--r--   0        0        0      189 2023-08-07 08:06:06.178522 ofscraper-3.0.3/ofscraper/utils/misc.py
+-rw-r--r--   0        0        0    10913 2023-08-07 08:06:06.178522 ofscraper-3.0.3/ofscraper/utils/of.py
+-rw-r--r--   0        0        0     7251 2023-08-07 08:06:06.178522 ofscraper-3.0.3/ofscraper/utils/paths.py
+-rw-r--r--   0        0        0     4221 2023-08-07 08:06:06.178522 ofscraper-3.0.3/ofscraper/utils/profiles.py
+-rw-r--r--   0        0        0      399 2023-08-07 08:06:06.178522 ofscraper-3.0.3/ofscraper/utils/semaphoreDelayed.py
+-rw-r--r--   0        0        0     1215 2023-08-07 08:06:06.178522 ofscraper-3.0.3/ofscraper/utils/separate.py
+-rw-r--r--   0        0        0      893 2023-08-07 08:06:06.178522 ofscraper-3.0.3/ofscraper/utils/stdout.py
+-rw-r--r--   0        0        0     5773 2023-08-07 08:06:06.178522 ofscraper-3.0.3/ofscraper/utils/userselector.py
+-rw-r--r--   0        0        0     2073 2023-08-07 08:06:38.622714 ofscraper-3.0.3/pyproject.toml
+-rw-r--r--   0        0        0     4720 1970-01-01 00:00:00.000000 ofscraper-3.0.3/PKG-INFO
```

### Comparing `ofscraper-3.0.2/LICENSE` & `ofscraper-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.2/README.md` & `ofscraper-3.0.3/README.md`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.2/ofscraper/__version__.py` & `ofscraper-3.0.3/ofscraper/__version__.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.2/ofscraper/__version__.pye` & `ofscraper-3.0.3/ofscraper/__version__.pye`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.2/ofscraper/api/archive.py` & `ofscraper-3.0.3/ofscraper/api/archive.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.2/ofscraper/api/highlights.py` & `ofscraper-3.0.3/ofscraper/api/highlights.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.2/ofscraper/api/init.py` & `ofscraper-3.0.3/ofscraper/api/init.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.2/ofscraper/api/labels.py` & `ofscraper-3.0.3/ofscraper/api/labels.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.2/ofscraper/api/me.py` & `ofscraper-3.0.3/ofscraper/api/me.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.2/ofscraper/api/messages.py` & `ofscraper-3.0.3/ofscraper/api/messages.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.2/ofscraper/api/paid.py` & `ofscraper-3.0.3/ofscraper/api/paid.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.2/ofscraper/api/pinned.py` & `ofscraper-3.0.3/ofscraper/api/pinned.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.2/ofscraper/api/profile.py` & `ofscraper-3.0.3/ofscraper/api/profile.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.2/ofscraper/api/subscriptions.py` & `ofscraper-3.0.3/ofscraper/api/subscriptions.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.2/ofscraper/api/timeline.py` & `ofscraper-3.0.3/ofscraper/api/timeline.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.2/ofscraper/classes/labels.py` & `ofscraper-3.0.3/ofscraper/classes/labels.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.2/ofscraper/classes/media.py` & `ofscraper-3.0.3/ofscraper/classes/media.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.2/ofscraper/classes/multiprocessprogress.py` & `ofscraper-3.0.3/ofscraper/classes/multiprocessprogress.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.2/ofscraper/classes/placeholder.py` & `ofscraper-3.0.3/ofscraper/classes/placeholder.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.2/ofscraper/classes/posts.py` & `ofscraper-3.0.3/ofscraper/classes/posts.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.2/ofscraper/classes/sessionbuilder.py` & `ofscraper-3.0.3/ofscraper/classes/sessionbuilder.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.2/ofscraper/classes/table.py` & `ofscraper-3.0.3/ofscraper/classes/table.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.2/ofscraper/commands/check.py` & `ofscraper-3.0.3/ofscraper/commands/check.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.2/ofscraper/commands/manual.py` & `ofscraper-3.0.3/ofscraper/commands/manual.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.2/ofscraper/commands/scraper.py` & `ofscraper-3.0.3/ofscraper/commands/scraper.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.2/ofscraper/constants.py` & `ofscraper-3.0.3/ofscraper/constants.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.2/ofscraper/db/operations.py` & `ofscraper-3.0.3/ofscraper/db/operations.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.2/ofscraper/db/queries.py` & `ofscraper-3.0.3/ofscraper/db/queries.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.2/ofscraper/interaction/like.py` & `ofscraper-3.0.3/ofscraper/interaction/like.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.2/ofscraper/prompts/keybindings.py` & `ofscraper-3.0.3/ofscraper/prompts/keybindings.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.2/ofscraper/prompts/promptConvert.py` & `ofscraper-3.0.3/ofscraper/prompts/promptConvert.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.2/ofscraper/prompts/prompt_strings.py` & `ofscraper-3.0.3/ofscraper/prompts/prompt_strings.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.2/ofscraper/prompts/prompt_validators.py` & `ofscraper-3.0.3/ofscraper/prompts/prompt_validators.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.2/ofscraper/prompts/prompts.py` & `ofscraper-3.0.3/ofscraper/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.2/ofscraper/start.py` & `ofscraper-3.0.3/ofscraper/start.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.2/ofscraper/utils/args.py` & `ofscraper-3.0.3/ofscraper/utils/args.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.2/ofscraper/utils/auth.py` & `ofscraper-3.0.3/ofscraper/utils/auth.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.2/ofscraper/utils/binaries.py` & `ofscraper-3.0.3/ofscraper/utils/binaries.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.2/ofscraper/utils/config.py` & `ofscraper-3.0.3/ofscraper/utils/config.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.2/ofscraper/utils/dates.py` & `ofscraper-3.0.3/ofscraper/utils/dates.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.2/ofscraper/utils/download.py` & `ofscraper-3.0.3/ofscraper/utils/download.py`

 * *Files 0% similar despite different names*

```diff
@@ -149,15 +149,15 @@
                         thread.join(1)
                         time.sleep(5)
         [logthread.join() for logthread in logthreads]
         [process.join(timeout=1) for process in processes]    
         [process.terminate() for process in processes]    
         overall_progress.remove_task(task1)
         progress_group.renderables[1].height=0
-        log.error(f'[bold]{username}[/bold] ({photo_count} photos, {video_count} videos, {audio_count} audios, {forced_skipped} skipped, {skipped} skipped)' )
+        log.error(f'[bold]{username}[/bold] ({photo_count} photos, {video_count} videos, {audio_count} audios, {forced_skipped} skipped, {skipped} failed)' )
         return photo_count,video_count,audio_count,forced_skipped,skipped
     except KeyboardInterrupt as E:
             try:
                 with exit.DelayedKeyboardInterrupt():
                     [process.terminate() for process in processes]  
                     raise KeyboardInterrupt
             except KeyboardInterrupt:
```

### Comparing `ofscraper-3.0.2/ofscraper/utils/encoding.py` & `ofscraper-3.0.3/ofscraper/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.2/ofscraper/utils/exit.py` & `ofscraper-3.0.3/ofscraper/utils/exit.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.2/ofscraper/utils/filters.py` & `ofscraper-3.0.3/ofscraper/utils/filters.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.2/ofscraper/utils/logger.py` & `ofscraper-3.0.3/ofscraper/utils/logger.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.2/ofscraper/utils/of.py` & `ofscraper-3.0.3/ofscraper/utils/of.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.2/ofscraper/utils/paths.py` & `ofscraper-3.0.3/ofscraper/utils/paths.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.2/ofscraper/utils/profiles.py` & `ofscraper-3.0.3/ofscraper/utils/profiles.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.2/ofscraper/utils/separate.py` & `ofscraper-3.0.3/ofscraper/utils/separate.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.2/ofscraper/utils/stdout.py` & `ofscraper-3.0.3/ofscraper/utils/stdout.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.2/ofscraper/utils/userselector.py` & `ofscraper-3.0.3/ofscraper/utils/userselector.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.2/pyproject.toml` & `ofscraper-3.0.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ofscraper"
-version = "3.0.2"
+version = "3.0.3"
 description = "automatically scrape onlyfans"
 authors = ["datawhores <datawhores@riseup.net>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">3.7.0,<3.12"
 httpx = {extras = ["http2"], version = "^0.23.3"}
```

### Comparing `ofscraper-3.0.2/PKG-INFO` & `ofscraper-3.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofscraper
-Version: 3.0.2
+Version: 3.0.3
 Summary: automatically scrape onlyfans
 Author: datawhores
 Author-email: datawhores@riseup.net
 Requires-Python: >3.7.0,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

