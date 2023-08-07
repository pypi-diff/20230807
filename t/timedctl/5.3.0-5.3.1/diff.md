# Comparing `tmp/timedctl-5.3.0.tar.gz` & `tmp/timedctl-5.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timedctl-5.3.0.tar", max compression
+gzip compressed data, was "timedctl-5.3.1.tar", max compression
```

## Comparing `timedctl-5.3.0.tar` & `timedctl-5.3.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    34454 2023-08-07 06:42:55.365531 timedctl-5.3.0/LICENSE
--rw-r--r--   0        0        0     2168 2023-08-07 06:42:55.365531 timedctl-5.3.0/README.md
--rw-r--r--   0        0        0     1237 2023-08-07 06:43:24.046969 timedctl-5.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-08-07 06:42:55.365531 timedctl-5.3.0/timedctl/__init__.py
--rw-r--r--   0        0        0     2488 2023-08-07 06:42:55.365531 timedctl-5.3.0/timedctl/helpers.py
--rwxr-xr-x   0        0        0    23400 2023-08-07 06:42:55.365531 timedctl-5.3.0/timedctl/timedctl.py
--rw-r--r--   0        0        0     2923 1970-01-01 00:00:00.000000 timedctl-5.3.0/PKG-INFO
+-rw-r--r--   0        0        0    34454 2023-08-07 13:27:41.407304 timedctl-5.3.1/LICENSE
+-rw-r--r--   0        0        0     2165 2023-08-07 13:27:41.407304 timedctl-5.3.1/README.md
+-rw-r--r--   0        0        0     1237 2023-08-07 13:28:11.939622 timedctl-5.3.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-07 13:27:41.407304 timedctl-5.3.1/timedctl/__init__.py
+-rw-r--r--   0        0        0     2488 2023-08-07 13:27:41.407304 timedctl-5.3.1/timedctl/helpers.py
+-rwxr-xr-x   0        0        0    23366 2023-08-07 13:27:41.407304 timedctl-5.3.1/timedctl/timedctl.py
+-rw-r--r--   0        0        0     2920 1970-01-01 00:00:00.000000 timedctl-5.3.1/PKG-INFO
```

### Comparing `timedctl-5.3.0/LICENSE` & `timedctl-5.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `timedctl-5.3.0/README.md` & `timedctl-5.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -15,25 +15,25 @@
 ```
 
 ### Shell completion
 `timedctl` support shell completion for the unaliased commands:
 
 **bash**
 ```bash
-_TIMEDCTL_COMPLETE=bash_source timedctl >> ~/.bashrc`
+_TIMEDCTL_COMPLETE=bash_source timedctl >> ~/.bashrc
 ```
 
 **zsh**
 ```bash
-_TIMEDCTL_COMPLETE=zsh_source timedctl >> ~/.zshrc`
+_TIMEDCTL_COMPLETE=zsh_source timedctl >> ~/.zshrc
 ```
 
 **fish**
 ```bash
-_TIMEDCTL_COMPLETE=fish_source timedctl >  ~/.config/fish/completions/timedctl.fish`
+_TIMEDCTL_COMPLETE=fish_source timedctl >  ~/.config/fish/completions/timedctl.fish
 ```
 
 ## Local development
 Clone the repository and install the dependencies with `poetry install`. You can now run the project with `poetry run timedctl`. For building wheels, you can use `poetry build`.
 Run tests with `poetry run pytest --cov --cov-fail-under 100`.
 
 ## Known issues
```

### Comparing `timedctl-5.3.0/pyproject.toml` & `timedctl-5.3.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "timedctl"
-version = "5.3.0"
+version = "5.3.1"
 description = "CLI for timed"
 authors = ["Arthur Deierlein <arthur.deierlein@adfinis.com>", "Gian Klug <gian.klug@adfinis.com>"]
 readme = "README.md"
 license = "AGPL-3.0-only"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `timedctl-5.3.0/timedctl/helpers.py` & `timedctl-5.3.1/timedctl/helpers.py`

 * *Files identical despite different names*

### Comparing `timedctl-5.3.0/timedctl/timedctl.py` & `timedctl-5.3.1/timedctl/timedctl.py`

 * *Files 1% similar despite different names*

```diff
@@ -609,20 +609,20 @@
     msg("Activity stopped successfully.")
 
 
 @activity.command("show", aliases=["s", "get", "info"])
 @click.option("--short", default=False, is_flag=True)
 def show_activity(short):
     """Show current activity."""
-    current_activity = timed.activities.current
+    current_activity = timed.activities.get(
+        filters={"active": True},
+        include="task,task.project,task.project.customer",
+    )
     if current_activity:
-        activity_obj = timed.activities.get(
-            filters={"id": current_activity["id"]},
-            include="task,task.project,task.project.customer",
-        )[0]
+        activity_obj = current_activity[0]
         comment = " > " + activity_obj["attributes"]["comment"] if not short else ""
         start = activity_obj["attributes"]["from-time"].strftime("%H:%M:%S")
         msg(
             f"Current activity: {format_activity(activity_obj)}{comment} (Since "
             + f"{start})",
         )
     else:
```

### Comparing `timedctl-5.3.0/PKG-INFO` & `timedctl-5.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timedctl
-Version: 5.3.0
+Version: 5.3.1
 Summary: CLI for timed
 License: AGPL-3.0-only
 Author: Arthur Deierlein
 Author-email: arthur.deierlein@adfinis.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
@@ -36,25 +36,25 @@
 ```
 
 ### Shell completion
 `timedctl` support shell completion for the unaliased commands:
 
 **bash**
 ```bash
-_TIMEDCTL_COMPLETE=bash_source timedctl >> ~/.bashrc`
+_TIMEDCTL_COMPLETE=bash_source timedctl >> ~/.bashrc
 ```
 
 **zsh**
 ```bash
-_TIMEDCTL_COMPLETE=zsh_source timedctl >> ~/.zshrc`
+_TIMEDCTL_COMPLETE=zsh_source timedctl >> ~/.zshrc
 ```
 
 **fish**
 ```bash
-_TIMEDCTL_COMPLETE=fish_source timedctl >  ~/.config/fish/completions/timedctl.fish`
+_TIMEDCTL_COMPLETE=fish_source timedctl >  ~/.config/fish/completions/timedctl.fish
 ```
 
 ## Local development
 Clone the repository and install the dependencies with `poetry install`. You can now run the project with `poetry run timedctl`. For building wheels, you can use `poetry build`.
 Run tests with `poetry run pytest --cov --cov-fail-under 100`.
 
 ## Known issues
```

