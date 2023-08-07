# Comparing `tmp/deezer_python-6.0.0.tar.gz` & `tmp/deezer_python-6.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deezer_python-6.0.0.tar", max compression
+gzip compressed data, was "deezer_python-6.1.0.tar", max compression
```

## Comparing `deezer_python-6.0.0.tar` & `deezer_python-6.1.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1054 2023-06-27 12:38:33.897315 deezer_python-6.0.0/LICENSE.txt
--rw-r--r--   0        0        0    13246 2023-06-27 12:38:33.897315 deezer_python-6.0.0/README.md
--rw-r--r--   0        0        0     2248 2023-06-27 12:38:34.849318 deezer_python-6.0.0/pyproject.toml
--rw-r--r--   0        0        0      556 2023-06-27 12:38:34.817318 deezer_python-6.0.0/src/deezer/__init__.py
--rw-r--r--   0        0        0    24840 2023-06-27 12:38:33.897315 deezer_python-6.0.0/src/deezer/client.py
--rw-r--r--   0        0        0      530 2023-06-27 12:38:33.897315 deezer_python-6.0.0/src/deezer/dates.py
--rw-r--r--   0        0        0     1864 2023-06-27 12:38:33.897315 deezer_python-6.0.0/src/deezer/exceptions.py
--rw-r--r--   0        0        0     3745 2023-06-27 12:38:33.897315 deezer_python-6.0.0/src/deezer/pagination.py
--rw-r--r--   0        0        0      549 2023-06-27 12:38:33.897315 deezer_python-6.0.0/src/deezer/resources/__init__.py
--rw-r--r--   0        0        0     1734 2023-06-27 12:38:33.897315 deezer_python-6.0.0/src/deezer/resources/album.py
--rw-r--r--   0        0        0     2150 2023-06-27 12:38:33.897315 deezer_python-6.0.0/src/deezer/resources/artist.py
--rw-r--r--   0        0        0     2047 2023-06-27 12:38:33.897315 deezer_python-6.0.0/src/deezer/resources/chart.py
--rw-r--r--   0        0        0     1413 2023-06-27 12:38:33.897315 deezer_python-6.0.0/src/deezer/resources/editorial.py
--rw-r--r--   0        0        0     1761 2023-06-27 12:38:33.897315 deezer_python-6.0.0/src/deezer/resources/episode.py
--rw-r--r--   0        0        0     1355 2023-06-27 12:38:33.897315 deezer_python-6.0.0/src/deezer/resources/genre.py
--rw-r--r--   0        0        0     3325 2023-06-27 12:38:33.897315 deezer_python-6.0.0/src/deezer/resources/playlist.py
--rw-r--r--   0        0        0      914 2023-06-27 12:38:33.897315 deezer_python-6.0.0/src/deezer/resources/podcast.py
--rw-r--r--   0        0        0      805 2023-06-27 12:38:33.897315 deezer_python-6.0.0/src/deezer/resources/radio.py
--rw-r--r--   0        0        0     4826 2023-06-27 12:38:33.897315 deezer_python-6.0.0/src/deezer/resources/resource.py
--rw-r--r--   0        0        0     1546 2023-06-27 12:38:33.897315 deezer_python-6.0.0/src/deezer/resources/track.py
--rw-r--r--   0        0        0     6752 2023-06-27 12:38:33.897315 deezer_python-6.0.0/src/deezer/resources/user.py
--rw-r--r--   0        0        0      583 2023-06-27 12:38:33.897315 deezer_python-6.0.0/src/deezer/utils.py
--rw-r--r--   0        0        0    14597 1970-01-01 00:00:00.000000 deezer_python-6.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1054 2023-08-07 16:06:01.380914 deezer_python-6.1.0/LICENSE.txt
+-rw-r--r--   0        0        0    13246 2023-08-07 16:06:01.380914 deezer_python-6.1.0/README.md
+-rw-r--r--   0        0        0     2439 2023-08-07 16:06:02.672895 deezer_python-6.1.0/pyproject.toml
+-rw-r--r--   0        0        0      556 2023-08-07 16:06:01.380914 deezer_python-6.1.0/src/deezer/__init__.py
+-rw-r--r--   0        0        0    24840 2023-08-07 16:06:01.380914 deezer_python-6.1.0/src/deezer/client.py
+-rw-r--r--   0        0        0      530 2023-08-07 16:06:01.380914 deezer_python-6.1.0/src/deezer/dates.py
+-rw-r--r--   0        0        0     1864 2023-08-07 16:06:01.380914 deezer_python-6.1.0/src/deezer/exceptions.py
+-rw-r--r--   0        0        0     3745 2023-08-07 16:06:01.380914 deezer_python-6.1.0/src/deezer/pagination.py
+-rw-r--r--   0        0        0      549 2023-08-07 16:06:01.380914 deezer_python-6.1.0/src/deezer/resources/__init__.py
+-rw-r--r--   0        0        0     1734 2023-08-07 16:06:01.380914 deezer_python-6.1.0/src/deezer/resources/album.py
+-rw-r--r--   0        0        0     2150 2023-08-07 16:06:01.380914 deezer_python-6.1.0/src/deezer/resources/artist.py
+-rw-r--r--   0        0        0     2047 2023-08-07 16:06:01.380914 deezer_python-6.1.0/src/deezer/resources/chart.py
+-rw-r--r--   0        0        0     1413 2023-08-07 16:06:01.380914 deezer_python-6.1.0/src/deezer/resources/editorial.py
+-rw-r--r--   0        0        0     1761 2023-08-07 16:06:01.380914 deezer_python-6.1.0/src/deezer/resources/episode.py
+-rw-r--r--   0        0        0     1355 2023-08-07 16:06:01.380914 deezer_python-6.1.0/src/deezer/resources/genre.py
+-rw-r--r--   0        0        0     3325 2023-08-07 16:06:01.380914 deezer_python-6.1.0/src/deezer/resources/playlist.py
+-rw-r--r--   0        0        0      914 2023-08-07 16:06:01.380914 deezer_python-6.1.0/src/deezer/resources/podcast.py
+-rw-r--r--   0        0        0      805 2023-08-07 16:06:01.380914 deezer_python-6.1.0/src/deezer/resources/radio.py
+-rw-r--r--   0        0        0     4826 2023-08-07 16:06:01.380914 deezer_python-6.1.0/src/deezer/resources/resource.py
+-rw-r--r--   0        0        0     1546 2023-08-07 16:06:01.380914 deezer_python-6.1.0/src/deezer/resources/track.py
+-rw-r--r--   0        0        0     6752 2023-08-07 16:06:01.380914 deezer_python-6.1.0/src/deezer/resources/user.py
+-rw-r--r--   0        0        0      583 2023-08-07 16:06:01.380914 deezer_python-6.1.0/src/deezer/utils.py
+-rw-r--r--   0        0        0    14630 1970-01-01 00:00:00.000000 deezer_python-6.1.0/PKG-INFO
```

### Comparing `deezer_python-6.0.0/LICENSE.txt` & `deezer_python-6.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `deezer_python-6.0.0/README.md` & `deezer_python-6.1.0/README.md`

 * *Files identical despite different names*

### Comparing `deezer_python-6.0.0/pyproject.toml` & `deezer_python-6.1.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "deezer-python"
-version = "6.0.0"
+version = "6.1.0"
 description = "A friendly wrapper library for the Deezer API"
 authors = ["Bruno Alla <alla.brunoo@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["deezer", "sdk", "client", "requests"]
 repository = "https://github.com/browniebroke/deezer-python"
 documentation = "https://deezer-python.readthedocs.io"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Natural Language :: English",
     "Operating System :: OS Independent",
-    "Topic :: Software Development :: Libraries :: Python Modules"
+    "Topic :: Software Development :: Libraries",
+    "Programming Language :: Python :: 3.12",
 ]
 packages = [
     { include = "deezer", from = "src" },
 ]
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/browniebroke/deezer-python/issues"
@@ -32,32 +33,41 @@
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 myst-parser = ">=0.16"
 sphinx = ">=4.0"
 sphinx-autobuild = ">=2021.0"
-sphinx-rtd-theme = ">=1.0"
+furo = ">=2023.5.20"
 
 [tool.poetry.group.dev.dependencies]
 coverage = "^7.0"
 environs = "^9.3"
 pytest = "^7.0"
 pytest-cov = "^4.0"
 pytest-mock = "^3.6"
 pytest-vcr = "^1.0"
 vcrpy = "^5.0.0"
 deezer-oauth-cli = "^1.0.0"
 
 [tool.semantic_release]
-version_toml = "pyproject.toml:tool.poetry.version"
+version_toml = ["pyproject.toml:tool.poetry.version"]
 version_variable = "src/deezer/__init__.py:__version__"
 branch = "main"
 build_command = "pip install poetry && poetry build"
 
+[tool.semantic_release.changelog]
+exclude_commit_patterns = [
+    "chore*",
+    "ci*",
+]
+
+[tool.semantic_release.changelog.environment]
+keep_trailing_newline = true
+
 [tool.pytest.ini_options]
 addopts = "-v -Wdefault --cov=deezer"
 pythonpath = ["src"]
 
 [tool.coverage.run]
 branch = true
 source = ["deezer"]
```

### Comparing `deezer_python-6.0.0/src/deezer/__init__.py` & `deezer_python-6.1.0/src/deezer/__init__.py`

 * *Files identical despite different names*

### Comparing `deezer_python-6.0.0/src/deezer/client.py` & `deezer_python-6.1.0/src/deezer/client.py`

 * *Files identical despite different names*

### Comparing `deezer_python-6.0.0/src/deezer/dates.py` & `deezer_python-6.1.0/src/deezer/dates.py`

 * *Files identical despite different names*

### Comparing `deezer_python-6.0.0/src/deezer/exceptions.py` & `deezer_python-6.1.0/src/deezer/exceptions.py`

 * *Files identical despite different names*

### Comparing `deezer_python-6.0.0/src/deezer/pagination.py` & `deezer_python-6.1.0/src/deezer/pagination.py`

 * *Files identical despite different names*

### Comparing `deezer_python-6.0.0/src/deezer/resources/__init__.py` & `deezer_python-6.1.0/src/deezer/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `deezer_python-6.0.0/src/deezer/resources/album.py` & `deezer_python-6.1.0/src/deezer/resources/album.py`

 * *Files identical despite different names*

### Comparing `deezer_python-6.0.0/src/deezer/resources/artist.py` & `deezer_python-6.1.0/src/deezer/resources/artist.py`

 * *Files identical despite different names*

### Comparing `deezer_python-6.0.0/src/deezer/resources/chart.py` & `deezer_python-6.1.0/src/deezer/resources/chart.py`

 * *Files identical despite different names*

### Comparing `deezer_python-6.0.0/src/deezer/resources/editorial.py` & `deezer_python-6.1.0/src/deezer/resources/editorial.py`

 * *Files identical despite different names*

### Comparing `deezer_python-6.0.0/src/deezer/resources/episode.py` & `deezer_python-6.1.0/src/deezer/resources/episode.py`

 * *Files identical despite different names*

### Comparing `deezer_python-6.0.0/src/deezer/resources/genre.py` & `deezer_python-6.1.0/src/deezer/resources/genre.py`

 * *Files identical despite different names*

### Comparing `deezer_python-6.0.0/src/deezer/resources/playlist.py` & `deezer_python-6.1.0/src/deezer/resources/playlist.py`

 * *Files identical despite different names*

### Comparing `deezer_python-6.0.0/src/deezer/resources/podcast.py` & `deezer_python-6.1.0/src/deezer/resources/podcast.py`

 * *Files identical despite different names*

### Comparing `deezer_python-6.0.0/src/deezer/resources/radio.py` & `deezer_python-6.1.0/src/deezer/resources/radio.py`

 * *Files identical despite different names*

### Comparing `deezer_python-6.0.0/src/deezer/resources/resource.py` & `deezer_python-6.1.0/src/deezer/resources/resource.py`

 * *Files identical despite different names*

### Comparing `deezer_python-6.0.0/src/deezer/resources/track.py` & `deezer_python-6.1.0/src/deezer/resources/track.py`

 * *Files identical despite different names*

### Comparing `deezer_python-6.0.0/src/deezer/resources/user.py` & `deezer_python-6.1.0/src/deezer/resources/user.py`

 * *Files identical despite different names*

### Comparing `deezer_python-6.0.0/src/deezer/utils.py` & `deezer_python-6.1.0/src/deezer/utils.py`

 * *Files identical despite different names*

### Comparing `deezer_python-6.0.0/PKG-INFO` & `deezer_python-6.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deezer-python
-Version: 6.0.0
+Version: 6.1.0
 Summary: A friendly wrapper library for the Deezer API
 Home-page: https://github.com/browniebroke/deezer-python
 License: MIT
 Keywords: deezer,sdk,client,requests
 Author: Bruno Alla
 Author-email: alla.brunoo@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -14,15 +14,16 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Software Development :: Libraries
 Requires-Dist: requests (>=2.18)
 Project-URL: Bug Tracker, https://github.com/browniebroke/deezer-python/issues
 Project-URL: Changelog, https://deezer-python.readthedocs.io/en/latest/changelog.html
 Project-URL: Documentation, https://deezer-python.readthedocs.io
 Project-URL: Mastodon, https://fosstodon.org/@browniebroke
 Project-URL: Repository, https://github.com/browniebroke/deezer-python
 Project-URL: Twitter, https://twitter.com/_BrunoAlla
```

#### html2text {}

```diff
@@ -1,26 +1,26 @@
-Metadata-Version: 2.1 Name: deezer-python Version: 6.0.0 Summary: A friendly
+Metadata-Version: 2.1 Name: deezer-python Version: 6.1.0 Summary: A friendly
 wrapper library for the Deezer API Home-page: https://github.com/browniebroke/
 deezer-python License: MIT Keywords: deezer,sdk,client,requests Author: Bruno
 Alla Author-email: alla.brunoo@gmail.com Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: Topic :: Software
-Development :: Libraries :: Python Modules Requires-Dist: requests (>=2.18)
-Project-URL: Bug Tracker, https://github.com/browniebroke/deezer-python/issues
-Project-URL: Changelog, https://deezer-python.readthedocs.io/en/latest/
-changelog.html Project-URL: Documentation, https://deezer-python.readthedocs.io
-Project-URL: Mastodon, https://fosstodon.org/@browniebroke Project-URL:
-Repository, https://github.com/browniebroke/deezer-python Project-URL: Twitter,
-https://twitter.com/_BrunoAlla Description-Content-Type: text/markdown # Deezer
-Python Client
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: 3.12 Classifier: Topic :: Software Development :: Libraries Requires-
+Dist: requests (>=2.18) Project-URL: Bug Tracker, https://github.com/
+browniebroke/deezer-python/issues Project-URL: Changelog, https://deezer-
+python.readthedocs.io/en/latest/changelog.html Project-URL: Documentation,
+https://deezer-python.readthedocs.io Project-URL: Mastodon, https://
+fosstodon.org/@browniebroke Project-URL: Repository, https://github.com/
+browniebroke/deezer-python Project-URL: Twitter, https://twitter.com/_BrunoAlla
+Description-Content-Type: text/markdown # Deezer Python Client
          [CI_Status] [Documentation_Status] [Test_coverage_percentage]
                          [Poetry] [black] [pre-commit]
       [Launch_demo_on_Binder] [PyPi_Status] [pyversions] [license] [LoC]
 --- **Documentation**: https://deezer-python.readthedocs.io **Source Code**:
 https://github.com/browniebroke/deezer-python --- A friendly Python wrapper
 around the [Deezer API](https://developers.deezer.com/api). ## Installation The
 package is published on [PyPI](https://pypi.org/project/deezer-python/) and can
```

