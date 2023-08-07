# Comparing `tmp/hishel-0.0.8.tar.gz` & `tmp/hishel-0.0.9.tar.gz`

## Comparing `hishel-0.0.8.tar` & `hishel-0.0.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 hishel-0.0.8/CHANGELOG.md
--rw-r--r--   0        0        0     3923 2020-02-02 00:00:00.000000 hishel-0.0.8/README.md
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 hishel-0.0.8/hishel/__init__.py
--rw-r--r--   0        0        0    12209 2020-02-02 00:00:00.000000 hishel-0.0.8/hishel/_controller.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 hishel-0.0.8/hishel/_exceptions.py
--rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 hishel-0.0.8/hishel/_files.py
--rw-r--r--   0        0        0     7921 2020-02-02 00:00:00.000000 hishel-0.0.8/hishel/_headers.py
--rw-r--r--   0        0        0     7939 2020-02-02 00:00:00.000000 hishel-0.0.8/hishel/_serializers.py
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 hishel-0.0.8/hishel/_synchronization.py
--rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 hishel-0.0.8/hishel/_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hishel-0.0.8/hishel/py.typed
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 hishel-0.0.8/hishel/_async/__init__.py
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 hishel-0.0.8/hishel/_async/_client.py
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 hishel-0.0.8/hishel/_async/_mock.py
--rw-r--r--   0        0        0     3051 2020-02-02 00:00:00.000000 hishel-0.0.8/hishel/_async/_pool.py
--rw-r--r--   0        0        0     4317 2020-02-02 00:00:00.000000 hishel-0.0.8/hishel/_async/_storages.py
--rw-r--r--   0        0        0     5811 2020-02-02 00:00:00.000000 hishel-0.0.8/hishel/_async/_transports.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 hishel-0.0.8/hishel/_sync/__init__.py
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 hishel-0.0.8/hishel/_sync/_client.py
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 hishel-0.0.8/hishel/_sync/_mock.py
--rw-r--r--   0        0        0     2902 2020-02-02 00:00:00.000000 hishel-0.0.8/hishel/_sync/_pool.py
--rw-r--r--   0        0        0     4122 2020-02-02 00:00:00.000000 hishel-0.0.8/hishel/_sync/_storages.py
--rw-r--r--   0        0        0     5597 2020-02-02 00:00:00.000000 hishel-0.0.8/hishel/_sync/_transports.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 hishel-0.0.8/.gitignore
--rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 hishel-0.0.8/LICENSE
--rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 hishel-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     6034 2020-02-02 00:00:00.000000 hishel-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 hishel-0.0.9/CHANGELOG.md
+-rw-r--r--   0        0        0     3923 2020-02-02 00:00:00.000000 hishel-0.0.9/README.md
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 hishel-0.0.9/hishel/__init__.py
+-rw-r--r--   0        0        0    12209 2020-02-02 00:00:00.000000 hishel-0.0.9/hishel/_controller.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 hishel-0.0.9/hishel/_exceptions.py
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 hishel-0.0.9/hishel/_files.py
+-rw-r--r--   0        0        0     7921 2020-02-02 00:00:00.000000 hishel-0.0.9/hishel/_headers.py
+-rw-r--r--   0        0        0     7939 2020-02-02 00:00:00.000000 hishel-0.0.9/hishel/_serializers.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 hishel-0.0.9/hishel/_synchronization.py
+-rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 hishel-0.0.9/hishel/_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hishel-0.0.9/hishel/py.typed
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 hishel-0.0.9/hishel/_async/__init__.py
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 hishel-0.0.9/hishel/_async/_client.py
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 hishel-0.0.9/hishel/_async/_mock.py
+-rw-r--r--   0        0        0     3051 2020-02-02 00:00:00.000000 hishel-0.0.9/hishel/_async/_pool.py
+-rw-r--r--   0        0        0     4317 2020-02-02 00:00:00.000000 hishel-0.0.9/hishel/_async/_storages.py
+-rw-r--r--   0        0        0     5811 2020-02-02 00:00:00.000000 hishel-0.0.9/hishel/_async/_transports.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 hishel-0.0.9/hishel/_sync/__init__.py
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 hishel-0.0.9/hishel/_sync/_client.py
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 hishel-0.0.9/hishel/_sync/_mock.py
+-rw-r--r--   0        0        0     2902 2020-02-02 00:00:00.000000 hishel-0.0.9/hishel/_sync/_pool.py
+-rw-r--r--   0        0        0     4122 2020-02-02 00:00:00.000000 hishel-0.0.9/hishel/_sync/_storages.py
+-rw-r--r--   0        0        0     5597 2020-02-02 00:00:00.000000 hishel-0.0.9/hishel/_sync/_transports.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 hishel-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 hishel-0.0.9/LICENSE
+-rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 hishel-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     6088 2020-02-02 00:00:00.000000 hishel-0.0.9/PKG-INFO
```

### Comparing `hishel-0.0.8/CHANGELOG.md` & `hishel-0.0.9/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Changelog
 
+## 0.0.9 (8/1/2023) 
+
+- Expose Controller API. (#23)
+
 ## 0.0.8 (7/31/2023)
 
 - Skip redis tests if the server was not found. (#16)
 - Decrease sleep time for the storage ttl tests. (#18)
 - Fail coverage under 100. (#19)
 
 ## 0.0.7 (7/30/2023)
```

### Comparing `hishel-0.0.8/README.md` & `hishel-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `hishel-0.0.8/hishel/_controller.py` & `hishel-0.0.9/hishel/_controller.py`

 * *Files identical despite different names*

### Comparing `hishel-0.0.8/hishel/_files.py` & `hishel-0.0.9/hishel/_files.py`

 * *Files identical despite different names*

### Comparing `hishel-0.0.8/hishel/_headers.py` & `hishel-0.0.9/hishel/_headers.py`

 * *Files identical despite different names*

### Comparing `hishel-0.0.8/hishel/_serializers.py` & `hishel-0.0.9/hishel/_serializers.py`

 * *Files identical despite different names*

### Comparing `hishel-0.0.8/hishel/_synchronization.py` & `hishel-0.0.9/hishel/_synchronization.py`

 * *Files identical despite different names*

### Comparing `hishel-0.0.8/hishel/_utils.py` & `hishel-0.0.9/hishel/_utils.py`

 * *Files identical despite different names*

### Comparing `hishel-0.0.8/hishel/_async/_client.py` & `hishel-0.0.9/hishel/_async/_client.py`

 * *Files identical despite different names*

### Comparing `hishel-0.0.8/hishel/_async/_mock.py` & `hishel-0.0.9/hishel/_async/_mock.py`

 * *Files identical despite different names*

### Comparing `hishel-0.0.8/hishel/_async/_pool.py` & `hishel-0.0.9/hishel/_async/_pool.py`

 * *Files identical despite different names*

### Comparing `hishel-0.0.8/hishel/_async/_storages.py` & `hishel-0.0.9/hishel/_async/_storages.py`

 * *Files identical despite different names*

### Comparing `hishel-0.0.8/hishel/_async/_transports.py` & `hishel-0.0.9/hishel/_async/_transports.py`

 * *Files identical despite different names*

### Comparing `hishel-0.0.8/hishel/_sync/_client.py` & `hishel-0.0.9/hishel/_sync/_client.py`

 * *Files identical despite different names*

### Comparing `hishel-0.0.8/hishel/_sync/_mock.py` & `hishel-0.0.9/hishel/_sync/_mock.py`

 * *Files identical despite different names*

### Comparing `hishel-0.0.8/hishel/_sync/_pool.py` & `hishel-0.0.9/hishel/_sync/_pool.py`

 * *Files identical despite different names*

### Comparing `hishel-0.0.8/hishel/_sync/_storages.py` & `hishel-0.0.9/hishel/_sync/_storages.py`

 * *Files identical despite different names*

### Comparing `hishel-0.0.8/hishel/_sync/_transports.py` & `hishel-0.0.9/hishel/_sync/_transports.py`

 * *Files identical despite different names*

### Comparing `hishel-0.0.8/LICENSE` & `hishel-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hishel-0.0.8/pyproject.toml` & `hishel-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hishel-0.0.8/PKG-INFO` & `hishel-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hishel
-Version: 0.0.8
+Version: 0.0.9
 Summary: Persistant cache implementation for httpx and httpcore
 Project-URL: Homepage, https://github.com/karosis88/hishel
 Project-URL: Source, https://github.com/karosis88/hishel
 Author-email: Kar Petrosyan <kar.petrosyanpy@gmail.com>
 License-Expression: BSD-3-Clause
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
@@ -146,14 +146,18 @@
 
 - Fork the project.
 - Make change.
 - Open the pull request.
 
 # Changelog
 
+## 0.0.9 (8/1/2023) 
+
+- Expose Controller API. (#23)
+
 ## 0.0.8 (7/31/2023)
 
 - Skip redis tests if the server was not found. (#16)
 - Decrease sleep time for the storage ttl tests. (#18)
 - Fail coverage under 100. (#19)
 
 ## 0.0.7 (7/30/2023)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hishel Version: 0.0.8 Summary: Persistant cache
+Metadata-Version: 2.1 Name: hishel Version: 0.0.9 Summary: Persistant cache
 implementation for httpx and httpcore Project-URL: Homepage, https://
 github.com/karosis88/hishel Project-URL: Source, https://github.com/karosis88/
 hishel Author-email: Kar Petrosyan
 petrosyanpy@gmail.com> License-Expression: BSD-3-Clause License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha Classifier: Environment :: Web
 Environment Classifier: Framework :: AsyncIO Classifier: Framework :: Trio
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
@@ -55,19 +55,20 @@
 from the cache ``` ## How and where are the responses saved? The responses are
 stored by `Hishel` in [storages](https://karosis88.github.io/hishel/userguide/
 #storages). You have complete control over them; you can change storage or even
 write your own if necessary. ## Contributing `Hishel` is a powerful tool, but
 it is also a new project with potential flaws, so we welcome contributions! You
 can open the pull request by following these instructions if you want to
 improve `Hishel`. ð - Fork the project. - Make change. - Open the pull
-request. # Changelog ## 0.0.8 (7/31/2023) - Skip redis tests if the server was
-not found. (#16) - Decrease sleep time for the storage ttl tests. (#18) - Fail
-coverage under 100. (#19) ## 0.0.7 (7/30/2023) - Add support for `Heuristic
-Freshness`. (#11) - Change `Controller.cache_heuristically` to
-`Controller.allow_heuristics`. (#12) - Handle import errors. (#13) ## 0.0.6 (7/
-29/2023) - Fix `Vary` header validation. (#8) - Dump original requests with the
-responses. (#7) ## 0.0.5 (7/29/2023) - Fix httpx response streaming. ## 0.0.4
-(7/29/2023) - Change `YamlSerializer` name to `YAMLSerializer`. ## 0.0.3 (7/28/
-2023) - Add `from_cache` response extension. - Add `typing_extensions` into the
+request. # Changelog ## 0.0.9 (8/1/2023) - Expose Controller API. (#23) ##
+0.0.8 (7/31/2023) - Skip redis tests if the server was not found. (#16) -
+Decrease sleep time for the storage ttl tests. (#18) - Fail coverage under 100.
+(#19) ## 0.0.7 (7/30/2023) - Add support for `Heuristic Freshness`. (#11) -
+Change `Controller.cache_heuristically` to `Controller.allow_heuristics`. (#12)
+- Handle import errors. (#13) ## 0.0.6 (7/29/2023) - Fix `Vary` header
+validation. (#8) - Dump original requests with the responses. (#7) ## 0.0.5 (7/
+29/2023) - Fix httpx response streaming. ## 0.0.4 (7/29/2023) - Change
+`YamlSerializer` name to `YAMLSerializer`. ## 0.0.3 (7/28/2023) - Add
+`from_cache` response extension. - Add `typing_extensions` into the
 requirements. ## 0.0.2 (7/25/2023) - Add [redis](https://redis.io/) support. -
 Make backends thread and task safe. - Add black as a new linter. - Add an
 expire time for cached responses.
```

