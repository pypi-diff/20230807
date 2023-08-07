# Comparing `tmp/BotUtils-2.3.0.tar.gz` & `tmp/BotUtils-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BotUtils-2.3.0.tar", last modified: Fri Dec  9 20:13:59 2022, max compression
+gzip compressed data, was "BotUtils-2.3.1.tar", last modified: Mon Aug  7 19:24:04 2023, max compression
```

## Comparing `BotUtils-2.3.0.tar` & `BotUtils-2.3.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-09 20:13:59.375748 BotUtils-2.3.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-09 20:13:59.375748 BotUtils-2.3.0/BotUtils/
--rw-rw-rw-   0 root         (0) root         (0)    12938 2022-12-09 20:10:52.000000 BotUtils-2.3.0/BotUtils/CommonUtils.py
--rw-rw-rw-   0 root         (0) root         (0)      140 2022-12-09 20:10:52.000000 BotUtils-2.3.0/BotUtils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-09 20:13:59.375748 BotUtils-2.3.0/BotUtils.egg-info/
--rw-r--r--   0 root         (0) root         (0)      377 2022-12-09 20:13:59.000000 BotUtils-2.3.0/BotUtils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      246 2022-12-09 20:13:59.000000 BotUtils-2.3.0/BotUtils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-09 20:13:59.000000 BotUtils-2.3.0/BotUtils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      280 2022-12-09 20:13:59.000000 BotUtils-2.3.0/BotUtils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2022-12-09 20:13:59.000000 BotUtils-2.3.0/BotUtils.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       62 2022-07-18 23:04:15.000000 BotUtils-2.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      377 2022-12-09 20:13:59.375748 BotUtils-2.3.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      104 2022-07-24 03:47:28.000000 BotUtils-2.3.0/README.rst
--rw-rw-rw-   0 root         (0) root         (0)       83 2022-07-18 23:04:15.000000 BotUtils-2.3.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-12-09 20:13:59.375748 BotUtils-2.3.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1122 2022-12-09 20:10:52.000000 BotUtils-2.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 19:24:04.023128 BotUtils-2.3.1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 19:24:04.023128 BotUtils-2.3.1/BotUtils/
+-rw-rw-rw-   0 root         (0) root         (0)    12945 2023-08-07 19:20:49.000000 BotUtils-2.3.1/BotUtils/CommonUtils.py
+-rw-rw-rw-   0 root         (0) root         (0)      140 2023-08-07 19:20:49.000000 BotUtils-2.3.1/BotUtils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 19:24:04.023128 BotUtils-2.3.1/BotUtils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      377 2023-08-07 19:24:03.000000 BotUtils-2.3.1/BotUtils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      246 2023-08-07 19:24:03.000000 BotUtils-2.3.1/BotUtils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 19:24:03.000000 BotUtils-2.3.1/BotUtils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      280 2023-08-07 19:24:03.000000 BotUtils-2.3.1/BotUtils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-08-07 19:24:03.000000 BotUtils-2.3.1/BotUtils.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       62 2022-07-18 23:04:15.000000 BotUtils-2.3.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      377 2023-08-07 19:24:04.023128 BotUtils-2.3.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      104 2022-07-24 03:47:28.000000 BotUtils-2.3.1/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)       83 2022-07-18 23:04:15.000000 BotUtils-2.3.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-07 19:24:04.023128 BotUtils-2.3.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1122 2022-12-09 20:10:52.000000 BotUtils-2.3.1/setup.py
```

### Comparing `BotUtils-2.3.0/BotUtils/CommonUtils.py` & `BotUtils-2.3.1/BotUtils/CommonUtils.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
             or not use_cache
         ):
             if bot_name:
                 return self.credmgr.bot(bot_name).reddit_app.reddit(
                     username,
                     reddit_class=reddit_class,
                     use_cache=False,
-                    extra_kwargs=reddit_kwargs,
+                    extra_reddit_kwargs=reddit_kwargs,
                 )
             else:
                 self._reddit_instances[reddit_class.__module__][
                     username
                 ] = self.bot.reddit_app.reddit(
                     username, reddit_class=reddit_class, use_cache=False
                 )
```

### Comparing `BotUtils-2.3.0/setup.py` & `BotUtils-2.3.1/setup.py`

 * *Files identical despite different names*

