# Comparing `tmp/ssb_project_cli-1.1.2.tar.gz` & `tmp/ssb_project_cli-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssb_project_cli-1.1.2.tar", max compression
+gzip compressed data, was "ssb_project_cli-1.1.3.tar", max compression
```

## Comparing `ssb_project_cli-1.1.2.tar` & `ssb_project_cli-1.1.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1073 2023-05-30 13:47:12.702997 ssb_project_cli-1.1.2/LICENSE
--rw-r--r--   0        0        0     2881 2023-05-30 13:47:12.702997 ssb_project_cli-1.1.2/README.md
--rw-r--r--   0        0        0     2635 2023-05-30 13:47:24.123110 ssb_project_cli-1.1.2/pyproject.toml
--rw-r--r--   0        0        0       23 2023-05-30 13:47:12.706997 ssb_project_cli-1.1.2/src/ssb_project_cli/__init__.py
--rw-r--r--   0        0        0      171 2023-05-30 13:47:12.706997 ssb_project_cli-1.1.2/src/ssb_project_cli/__main__.py
--rw-r--r--   0        0        0        0 2023-05-30 13:47:12.706997 ssb_project_cli-1.1.2/src/ssb_project_cli/py.typed
--rw-r--r--   0        0        0      257 2023-05-30 13:47:12.706997 ssb_project_cli-1.1.2/src/ssb_project_cli/ssb_project/__init__.py
--rw-r--r--   0        0        0     4305 2023-05-30 13:47:12.706997 ssb_project_cli-1.1.2/src/ssb_project_cli/ssb_project/app.py
--rw-r--r--   0        0        0       29 2023-05-30 13:47:12.706997 ssb_project_cli-1.1.2/src/ssb_project_cli/ssb_project/build/__init__.py
--rw-r--r--   0        0        0     3158 2023-05-30 13:47:24.123110 ssb_project_cli-1.1.2/src/ssb_project_cli/ssb_project/build/build.py
--rw-r--r--   0        0        0     3740 2023-05-30 13:47:12.706997 ssb_project_cli-1.1.2/src/ssb_project_cli/ssb_project/build/environment.py
--rw-r--r--   0        0        0     4986 2023-05-30 13:47:24.123110 ssb_project_cli-1.1.2/src/ssb_project_cli/ssb_project/build/poetry.py
--rw-r--r--   0        0        0     1886 2023-05-30 13:47:12.706997 ssb_project_cli-1.1.2/src/ssb_project_cli/ssb_project/build/prompt.py
--rw-r--r--   0        0        0     1644 2023-05-30 13:47:12.706997 ssb_project_cli-1.1.2/src/ssb_project_cli/ssb_project/build/temp_template_repo.py
--rw-r--r--   0        0        0       69 2023-05-30 13:47:12.706997 ssb_project_cli-1.1.2/src/ssb_project_cli/ssb_project/build_cmds.md
--rw-r--r--   0        0        0       29 2023-05-30 13:47:12.706997 ssb_project_cli-1.1.2/src/ssb_project_cli/ssb_project/clean/__init__.py
--rw-r--r--   0        0        0     3008 2023-05-30 13:47:12.706997 ssb_project_cli-1.1.2/src/ssb_project_cli/ssb_project/clean/clean.py
--rw-r--r--   0        0        0       30 2023-05-30 13:47:12.706997 ssb_project_cli-1.1.2/src/ssb_project_cli/ssb_project/create/__init__.py
--rw-r--r--   0        0        0     6285 2023-05-30 13:47:12.706997 ssb_project_cli-1.1.2/src/ssb_project_cli/ssb_project/create/create.py
--rw-r--r--   0        0        0     9618 2023-05-30 13:47:12.706997 ssb_project_cli-1.1.2/src/ssb_project_cli/ssb_project/create/github.py
--rw-r--r--   0        0        0     6057 2023-05-30 13:47:12.706997 ssb_project_cli-1.1.2/src/ssb_project_cli/ssb_project/create/local_repo.py
--rw-r--r--   0        0        0     1631 2023-05-30 13:47:12.706997 ssb_project_cli-1.1.2/src/ssb_project_cli/ssb_project/create/prompt.py
--rw-r--r--   0        0        0      224 2023-05-30 13:47:12.706997 ssb_project_cli-1.1.2/src/ssb_project_cli/ssb_project/create/repo_privacy.py
--rw-r--r--   0        0        0     1303 2023-05-30 13:47:12.706997 ssb_project_cli-1.1.2/src/ssb_project_cli/ssb_project/create/temp_git_repo.py
--rw-r--r--   0        0        0      368 2023-05-30 13:47:12.706997 ssb_project_cli-1.1.2/src/ssb_project_cli/ssb_project/settings.py
--rw-r--r--   0        0        0     3209 2023-05-30 13:47:12.706997 ssb_project_cli-1.1.2/src/ssb_project_cli/ssb_project/util.py
--rw-r--r--   0        0        0     4323 1970-01-01 00:00:00.000000 ssb_project_cli-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-08-07 10:42:26.780087 ssb_project_cli-1.1.3/LICENSE
+-rw-r--r--   0        0        0     2881 2023-08-07 10:42:26.780087 ssb_project_cli-1.1.3/README.md
+-rw-r--r--   0        0        0     2654 2023-08-07 10:42:41.324310 ssb_project_cli-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0       23 2023-08-07 10:42:26.784087 ssb_project_cli-1.1.3/src/ssb_project_cli/__init__.py
+-rw-r--r--   0        0        0      171 2023-08-07 10:42:26.784087 ssb_project_cli-1.1.3/src/ssb_project_cli/__main__.py
+-rw-r--r--   0        0        0        0 2023-08-07 10:42:26.784087 ssb_project_cli-1.1.3/src/ssb_project_cli/py.typed
+-rw-r--r--   0        0        0      257 2023-08-07 10:42:26.784087 ssb_project_cli-1.1.3/src/ssb_project_cli/ssb_project/__init__.py
+-rw-r--r--   0        0        0     4305 2023-08-07 10:42:26.784087 ssb_project_cli-1.1.3/src/ssb_project_cli/ssb_project/app.py
+-rw-r--r--   0        0        0       29 2023-08-07 10:42:26.784087 ssb_project_cli-1.1.3/src/ssb_project_cli/ssb_project/build/__init__.py
+-rw-r--r--   0        0        0     3158 2023-08-07 10:42:26.784087 ssb_project_cli-1.1.3/src/ssb_project_cli/ssb_project/build/build.py
+-rw-r--r--   0        0        0     3740 2023-08-07 10:42:26.784087 ssb_project_cli-1.1.3/src/ssb_project_cli/ssb_project/build/environment.py
+-rw-r--r--   0        0        0     4986 2023-08-07 10:42:26.784087 ssb_project_cli-1.1.3/src/ssb_project_cli/ssb_project/build/poetry.py
+-rw-r--r--   0        0        0     1886 2023-08-07 10:42:26.784087 ssb_project_cli-1.1.3/src/ssb_project_cli/ssb_project/build/prompt.py
+-rw-r--r--   0        0        0     1644 2023-08-07 10:42:26.784087 ssb_project_cli-1.1.3/src/ssb_project_cli/ssb_project/build/temp_template_repo.py
+-rw-r--r--   0        0        0       69 2023-08-07 10:42:26.784087 ssb_project_cli-1.1.3/src/ssb_project_cli/ssb_project/build_cmds.md
+-rw-r--r--   0        0        0       29 2023-08-07 10:42:26.784087 ssb_project_cli-1.1.3/src/ssb_project_cli/ssb_project/clean/__init__.py
+-rw-r--r--   0        0        0     3008 2023-08-07 10:42:26.784087 ssb_project_cli-1.1.3/src/ssb_project_cli/ssb_project/clean/clean.py
+-rw-r--r--   0        0        0       30 2023-08-07 10:42:26.784087 ssb_project_cli-1.1.3/src/ssb_project_cli/ssb_project/create/__init__.py
+-rw-r--r--   0        0        0     6285 2023-08-07 10:42:26.784087 ssb_project_cli-1.1.3/src/ssb_project_cli/ssb_project/create/create.py
+-rw-r--r--   0        0        0     9618 2023-08-07 10:42:26.784087 ssb_project_cli-1.1.3/src/ssb_project_cli/ssb_project/create/github.py
+-rw-r--r--   0        0        0     6057 2023-08-07 10:42:26.784087 ssb_project_cli-1.1.3/src/ssb_project_cli/ssb_project/create/local_repo.py
+-rw-r--r--   0        0        0     1631 2023-08-07 10:42:26.784087 ssb_project_cli-1.1.3/src/ssb_project_cli/ssb_project/create/prompt.py
+-rw-r--r--   0        0        0      224 2023-08-07 10:42:26.784087 ssb_project_cli-1.1.3/src/ssb_project_cli/ssb_project/create/repo_privacy.py
+-rw-r--r--   0        0        0     1303 2023-08-07 10:42:26.784087 ssb_project_cli-1.1.3/src/ssb_project_cli/ssb_project/create/temp_git_repo.py
+-rw-r--r--   0        0        0      368 2023-08-07 10:42:26.784087 ssb_project_cli-1.1.3/src/ssb_project_cli/ssb_project/settings.py
+-rw-r--r--   0        0        0     3396 2023-08-07 10:42:26.784087 ssb_project_cli-1.1.3/src/ssb_project_cli/ssb_project/util.py
+-rw-r--r--   0        0        0     4413 1970-01-01 00:00:00.000000 ssb_project_cli-1.1.3/PKG-INFO
```

### Comparing `ssb_project_cli-1.1.2/LICENSE` & `ssb_project_cli-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ssb_project_cli-1.1.2/README.md` & `ssb_project_cli-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `ssb_project_cli-1.1.2/pyproject.toml` & `ssb_project_cli-1.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ssb-project-cli"
-version = "1.1.2"
+version = "1.1.3"
 description = "SSB Project CLI"
 authors = ["Statistics Norway <stat-dev@ssb.no>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/statisticsnorway/ssb-project-cli"
 repository = "https://github.com/statisticsnorway/ssb-project-cli"
 documentation = "https://ssb-project-cli.readthedocs.io"
@@ -15,15 +15,15 @@
     "Development Status :: 4 - Beta",
 ]
 
 [tool.poetry.urls]
 Changelog = "https://github.com/statisticsnorway/ssb-project-cli/releases"
 
 [tool.poetry.dependencies]
-python = ">=3.10,<3.11"
+python = ">=3.10,<3.12"
 click = ">=8.0.1"
 dparse = "^0.6.2"
 typer = "^0.6.1"
 GitPython = "^3.1.27"
 PyGithub = "^1.55"
 cruft = "^2.11.1"
 rich = "^12.5.1"
@@ -33,14 +33,15 @@
 questionary = "^1.10.0"
 certifi = "^2022.12.7"
 psutil = "^5.9.4"
 types-urllib3 = "^1.26.25.10"
 types-requests = "^2.28.11.17"
 types-psutil = "^5.9.5.12"
 kvakk-git-tools = "^2.2.1"
+poetry = "^1.3.0"
 
 
 [tool.poetry.dev-dependencies]
 Pygments = ">=2.10.0"
 black = ">=21.10b0"
 coverage = {extras = ["toml"], version = ">=6.2"}
 darglint = ">=1.8.1"
@@ -69,15 +70,15 @@
 mkdocstrings-python = "^0.7.1"
 mkdocs-literate-nav = "^0.5.0"
 mkdocs-section-index = "^0.3.4"
 mkdocstrings = "^0.19.0"
 mkdocs-material = "^8.5.6"
 mkdocs-click = "^0.8.0"
 mkdocs-gen-files = "^0.4.0"
-build = "^0.8.0"
+build = ">=0.8.0"
 Jinja2 = "^3.1.2"
 
 
 [tool.poetry.scripts]
 ssb-project = "ssb_project_cli.__main__:main"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `ssb_project_cli-1.1.2/src/ssb_project_cli/ssb_project/app.py` & `ssb_project_cli-1.1.3/src/ssb_project_cli/ssb_project/app.py`

 * *Files identical despite different names*

### Comparing `ssb_project_cli-1.1.2/src/ssb_project_cli/ssb_project/build/build.py` & `ssb_project_cli-1.1.3/src/ssb_project_cli/ssb_project/build/build.py`

 * *Files identical despite different names*

### Comparing `ssb_project_cli-1.1.2/src/ssb_project_cli/ssb_project/build/environment.py` & `ssb_project_cli-1.1.3/src/ssb_project_cli/ssb_project/build/environment.py`

 * *Files identical despite different names*

### Comparing `ssb_project_cli-1.1.2/src/ssb_project_cli/ssb_project/build/poetry.py` & `ssb_project_cli-1.1.3/src/ssb_project_cli/ssb_project/build/poetry.py`

 * *Files identical despite different names*

### Comparing `ssb_project_cli-1.1.2/src/ssb_project_cli/ssb_project/build/prompt.py` & `ssb_project_cli-1.1.3/src/ssb_project_cli/ssb_project/build/prompt.py`

 * *Files identical despite different names*

### Comparing `ssb_project_cli-1.1.2/src/ssb_project_cli/ssb_project/build/temp_template_repo.py` & `ssb_project_cli-1.1.3/src/ssb_project_cli/ssb_project/build/temp_template_repo.py`

 * *Files identical despite different names*

### Comparing `ssb_project_cli-1.1.2/src/ssb_project_cli/ssb_project/clean/clean.py` & `ssb_project_cli-1.1.3/src/ssb_project_cli/ssb_project/clean/clean.py`

 * *Files identical despite different names*

### Comparing `ssb_project_cli-1.1.2/src/ssb_project_cli/ssb_project/create/create.py` & `ssb_project_cli-1.1.3/src/ssb_project_cli/ssb_project/create/create.py`

 * *Files identical despite different names*

### Comparing `ssb_project_cli-1.1.2/src/ssb_project_cli/ssb_project/create/github.py` & `ssb_project_cli-1.1.3/src/ssb_project_cli/ssb_project/create/github.py`

 * *Files identical despite different names*

### Comparing `ssb_project_cli-1.1.2/src/ssb_project_cli/ssb_project/create/local_repo.py` & `ssb_project_cli-1.1.3/src/ssb_project_cli/ssb_project/create/local_repo.py`

 * *Files identical despite different names*

### Comparing `ssb_project_cli-1.1.2/src/ssb_project_cli/ssb_project/create/prompt.py` & `ssb_project_cli-1.1.3/src/ssb_project_cli/ssb_project/create/prompt.py`

 * *Files identical despite different names*

### Comparing `ssb_project_cli-1.1.2/src/ssb_project_cli/ssb_project/create/temp_git_repo.py` & `ssb_project_cli-1.1.3/src/ssb_project_cli/ssb_project/create/temp_git_repo.py`

 * *Files identical despite different names*

### Comparing `ssb_project_cli-1.1.2/src/ssb_project_cli/ssb_project/util.py` & `ssb_project_cli-1.1.3/src/ssb_project_cli/ssb_project/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,14 +42,17 @@
         filename = f"{calling_function}-error-{int(time.time())}.txt"
         with open(f"{error_logs_path}/{filename}", "w+") as f:
             f.write(log)
             print(f"Detailed error information saved to {error_logs_path}/{filename}")
             print(
                 f"You can find the full debug log here {error_logs_path}/ssb-project-debug.log"
             )
+            print(
+                f"❗️You can try deleting '.poetry/cache' in your project directory or '{home_path}/.cache/pypoetry'. Cache could be causing problems"
+            )
             f.close()
     except Exception as e:
         print(f"Error while attempting to write the log file: {e}")
 
 
 def execute_command(
     command: Union[str, list[str]],
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ssb_project_cli-1.1.2/PKG-INFO` & `ssb_project_cli-1.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: ssb-project-cli
-Version: 1.1.2
+Version: 1.1.3
 Summary: SSB Project CLI
 Home-page: https://github.com/statisticsnorway/ssb-project-cli
 License: MIT
 Author: Statistics Norway
 Author-email: stat-dev@ssb.no
-Requires-Python: >=3.10,<3.11
+Requires-Python: >=3.10,<3.12
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: GitPython (>=3.1.27,<4.0.0)
 Requires-Dist: PyGithub (>=1.55,<2.0)
 Requires-Dist: certifi (>=2022.12.7,<2023.0.0)
 Requires-Dist: click (>=8.0.1)
 Requires-Dist: cruft (>=2.11.1,<3.0.0)
 Requires-Dist: dparse (>=0.6.2,<0.7.0)
 Requires-Dist: kvakk-git-tools (>=2.2.1,<3.0.0)
+Requires-Dist: poetry (>=1.3.0,<2.0.0)
 Requires-Dist: psutil (>=5.9.4,<6.0.0)
 Requires-Dist: questionary (>=1.10.0,<2.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: rich (>=12.5.1,<13.0.0)
 Requires-Dist: typer (>=0.6.1,<0.7.0)
 Requires-Dist: types-psutil (>=5.9.5.12,<6.0.0.0)
 Requires-Dist: types-requests (>=2.28.11.17,<3.0.0.0)
```

