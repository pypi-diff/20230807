# Comparing `tmp/python_web_io-0.2.0.tar.gz` & `tmp/python_web_io-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_web_io-0.2.0.tar", max compression
+gzip compressed data, was "python_web_io-0.2.1.tar", max compression
```

## Comparing `python_web_io-0.2.0.tar` & `python_web_io-0.2.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rwxr-xr-x   0        0        0     1971 2023-08-07 21:17:01.070527 python_web_io-0.2.0/README.md
--rwxr-xr-x   0        0        0      919 2023-08-07 21:18:36.075419 python_web_io-0.2.0/pyproject.toml
--rwxr-xr-x   0        0        0       98 2023-08-07 18:18:55.304806 python_web_io-0.2.0/python_web_io/__init__.py
--rwxr-xr-x   0        0        0     2514 2023-08-06 13:54:57.229939 python_web_io-0.2.0/python_web_io/cache.py
--rwxr-xr-x   0        0        0    12301 2023-08-07 21:12:21.496386 python_web_io-0.2.0/python_web_io/main.py
--rwxr-xr-x   0        0        0     4185 2023-08-07 12:08:19.419570 python_web_io-0.2.0/python_web_io/override.py
--rwxr-xr-x   0        0        0     7662 2023-08-07 20:53:03.801698 python_web_io-0.2.0/python_web_io/templates/base.html
--rwxr-xr-x   0        0        0      498 2023-08-06 22:47:45.932667 python_web_io-0.2.0/python_web_io/templates/error.html
--rwxr-xr-x   0        0        0     2849 2023-08-07 12:44:07.456937 python_web_io-0.2.0/python_web_io/templates/index.html
--rw-r--r--   0        0        0     2900 1970-01-01 00:00:00.000000 python_web_io-0.2.0/PKG-INFO
+-rwxr-xr-x   0        0        0     2199 2023-08-07 21:20:04.039550 python_web_io-0.2.1/README.md
+-rwxr-xr-x   0        0        0      919 2023-08-07 21:20:54.664260 python_web_io-0.2.1/pyproject.toml
+-rwxr-xr-x   0        0        0       98 2023-08-07 18:18:55.304806 python_web_io-0.2.1/python_web_io/__init__.py
+-rwxr-xr-x   0        0        0     2514 2023-08-06 13:54:57.229939 python_web_io-0.2.1/python_web_io/cache.py
+-rwxr-xr-x   0        0        0    12301 2023-08-07 21:12:21.496386 python_web_io-0.2.1/python_web_io/main.py
+-rwxr-xr-x   0        0        0     4185 2023-08-07 12:08:19.419570 python_web_io-0.2.1/python_web_io/override.py
+-rwxr-xr-x   0        0        0     7662 2023-08-07 20:53:03.801698 python_web_io-0.2.1/python_web_io/templates/base.html
+-rwxr-xr-x   0        0        0      498 2023-08-06 22:47:45.932667 python_web_io-0.2.1/python_web_io/templates/error.html
+-rwxr-xr-x   0        0        0     2849 2023-08-07 12:44:07.456937 python_web_io-0.2.1/python_web_io/templates/index.html
+-rw-r--r--   0        0        0     3122 1970-01-01 00:00:00.000000 python_web_io-0.2.1/PKG-INFO
```

### Comparing `python_web_io-0.2.0/README.md` & `python_web_io-0.2.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -20,23 +20,29 @@
 ```bash
 poetry add python_web_io --with examples
 ```
 
 After installing the project, some environment setup is required:
 
 ### Required setup
-Create an `app.py` file containing your script, and an `.envrc` file to store project secrets. (Note: remember to add `.envrc` to your `.gitignore`)
-Look for example apps in [`./python_web_io/examples`](https://github.com/Cutwell/python-web-io/tree/main/python_web_io/examples).
+Create an `app.py` file containing your script, a `config.toml` setting the script filepath and entrypoint, and an `.envrc` file to store project secrets. (Note: remember to add `.envrc` to your `.gitignore`). Look for example apps in [`./python_web_io/examples`](https://github.com/Cutwell/python-web-io/tree/main/python_web_io/examples).
 ```
 .
 ├── .envrc
 ├── config.toml
 └── app.py
 ```
 
+Create the following simple `config.toml`:
+```toml
+[script]
+filepath = "app.py"
+entrypoint = "main"	# if your app has no entrypoint, remove this parameter.
+```
+
 Add the following environment variables to your `.envrc`. (Note: remember to activate the `.envrc` in your terminal using `direnv allow`)
 ```bash
 # server env vars
 export PYTHON_WEB_IO_SECRET=""
 export PYTHON_WEB_IO_CONFIG=".pythonwebio/config.toml" 	# defaults to .pythonwebio/config.toml if not set
 ```
```

### Comparing `python_web_io-0.2.0/pyproject.toml` & `python_web_io-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-web-io"
-version = "0.2.0"
+version = "0.2.1"
 description = "Generate a webpage as a GUI for a Python script, and serve from anywhere."
 authors = ["Zachary Smith <zachsmith.dev@gmail.com>"]
 packages = [{include = "python_web_io"}]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/Cutwell/python-web-io"
```

### Comparing `python_web_io-0.2.0/python_web_io/cache.py` & `python_web_io-0.2.1/python_web_io/cache.py`

 * *Files identical despite different names*

### Comparing `python_web_io-0.2.0/python_web_io/main.py` & `python_web_io-0.2.1/python_web_io/main.py`

 * *Files identical despite different names*

### Comparing `python_web_io-0.2.0/python_web_io/override.py` & `python_web_io-0.2.1/python_web_io/override.py`

 * *Files identical despite different names*

### Comparing `python_web_io-0.2.0/python_web_io/templates/base.html` & `python_web_io-0.2.1/python_web_io/templates/base.html`

 * *Files identical despite different names*

### Comparing `python_web_io-0.2.0/python_web_io/templates/index.html` & `python_web_io-0.2.1/python_web_io/templates/index.html`

 * *Files identical despite different names*

### Comparing `python_web_io-0.2.0/PKG-INFO` & `python_web_io-0.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-web-io
-Version: 0.2.0
+Version: 0.2.1
 Summary: Generate a webpage as a GUI for a Python script, and serve from anywhere.
 Home-page: https://github.com/Cutwell/python-web-io
 License: MIT
 Author: Zachary Smith
 Author-email: zachsmith.dev@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -45,23 +45,29 @@
 ```bash
 poetry add python_web_io --with examples
 ```
 
 After installing the project, some environment setup is required:
 
 ### Required setup
-Create an `app.py` file containing your script, and an `.envrc` file to store project secrets. (Note: remember to add `.envrc` to your `.gitignore`)
-Look for example apps in [`./python_web_io/examples`](https://github.com/Cutwell/python-web-io/tree/main/python_web_io/examples).
+Create an `app.py` file containing your script, a `config.toml` setting the script filepath and entrypoint, and an `.envrc` file to store project secrets. (Note: remember to add `.envrc` to your `.gitignore`). Look for example apps in [`./python_web_io/examples`](https://github.com/Cutwell/python-web-io/tree/main/python_web_io/examples).
 ```
 .
 ├── .envrc
 ├── config.toml
 └── app.py
 ```
 
+Create the following simple `config.toml`:
+```toml
+[script]
+filepath = "app.py"
+entrypoint = "main"	# if your app has no entrypoint, remove this parameter.
+```
+
 Add the following environment variables to your `.envrc`. (Note: remember to activate the `.envrc` in your terminal using `direnv allow`)
 ```bash
 # server env vars
 export PYTHON_WEB_IO_SECRET=""
 export PYTHON_WEB_IO_CONFIG=".pythonwebio/config.toml" 	# defaults to .pythonwebio/config.toml if not set
 ```
```

