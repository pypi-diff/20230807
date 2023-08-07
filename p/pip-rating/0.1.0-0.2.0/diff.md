# Comparing `tmp/pip-rating-0.1.0.tar.gz` & `tmp/pip-rating-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pip-rating-0.1.0.tar", last modified: Thu Jul 20 20:38:52 2023, max compression
+gzip compressed data, was "pip-rating-0.2.0.tar", last modified: Mon Aug  7 01:39:53 2023, max compression
```

## Comparing `pip-rating-0.1.0.tar` & `pip-rating-0.2.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 nekmo     (1000) users      (100)        0 2023-07-20 20:38:52.143433 pip-rating-0.1.0/
--rw-r--r--   0 nekmo     (1000) users      (100)      149 2023-06-30 01:00:25.000000 pip-rating-0.1.0/AUTHORS.rst
--rw-r--r--   0 nekmo     (1000) users      (100)     3413 2023-07-11 23:52:04.000000 pip-rating-0.1.0/CONTRIBUTING.rst
--rw-r--r--   0 nekmo     (1000) users      (100)       89 2023-06-30 01:00:25.000000 pip-rating-0.1.0/HISTORY.rst
--rw-r--r--   0 nekmo     (1000) users      (100)     1065 2023-06-30 01:00:25.000000 pip-rating-0.1.0/LICENSE
--rw-r--r--   0 nekmo     (1000) users      (100)      304 2023-07-20 20:38:42.000000 pip-rating-0.1.0/MANIFEST.in
--rw-r--r--   0 nekmo     (1000) users      (100)     5761 2023-07-20 20:38:52.143433 pip-rating-0.1.0/PKG-INFO
--rw-r--r--   0 nekmo     (1000) users      (100)     4727 2023-07-20 20:38:48.000000 pip-rating-0.1.0/README.rst
-drwxr-xr-x   0 nekmo     (1000) users      (100)        0 2023-07-20 20:38:52.136766 pip-rating-0.1.0/pip_rating/
--rw-r--r--   0 nekmo     (1000) users      (100)      174 2023-07-20 19:57:00.000000 pip-rating-0.1.0/pip_rating/__init__.py
--rw-r--r--   0 nekmo     (1000) users      (100)      690 2023-07-11 15:08:10.000000 pip-rating-0.1.0/pip_rating/_compat.py
--rw-r--r--   0 nekmo     (1000) users      (100)     5432 2023-07-17 14:50:17.000000 pip-rating-0.1.0/pip_rating/dependencies.py
--rw-r--r--   0 nekmo     (1000) users      (100)     1799 2023-07-18 02:42:23.000000 pip-rating-0.1.0/pip_rating/exceptions.py
--rw-r--r--   0 nekmo     (1000) users      (100)     6828 2023-07-17 15:05:40.000000 pip-rating-0.1.0/pip_rating/management.py
--rw-r--r--   0 nekmo     (1000) users      (100)     3530 2023-07-18 12:14:07.000000 pip-rating-0.1.0/pip_rating/packages.py
--rw-r--r--   0 nekmo     (1000) users      (100)    11032 2023-07-19 21:53:29.000000 pip-rating-0.1.0/pip_rating/rating.py
-drwxr-xr-x   0 nekmo     (1000) users      (100)        0 2023-07-20 20:38:52.143433 pip-rating-0.1.0/pip_rating/req_files/
--rw-r--r--   0 nekmo     (1000) users      (100)     1493 2023-07-17 01:53:25.000000 pip-rating-0.1.0/pip_rating/req_files/__init__.py
--rw-r--r--   0 nekmo     (1000) users      (100)     1475 2023-07-17 14:41:01.000000 pip-rating-0.1.0/pip_rating/req_files/base.py
--rw-r--r--   0 nekmo     (1000) users      (100)      909 2023-07-20 12:26:26.000000 pip-rating-0.1.0/pip_rating/req_files/package_list.py
--rw-r--r--   0 nekmo     (1000) users      (100)     1018 2023-07-17 01:53:25.000000 pip-rating-0.1.0/pip_rating/req_files/pipfile.py
--rw-r--r--   0 nekmo     (1000) users      (100)     3575 2023-07-20 13:49:50.000000 pip-rating-0.1.0/pip_rating/req_files/pyproject.py
--rw-r--r--   0 nekmo     (1000) users      (100)     1916 2023-07-17 01:53:25.000000 pip-rating-0.1.0/pip_rating/req_files/requirements.py
--rw-r--r--   0 nekmo     (1000) users      (100)     1077 2023-07-17 01:53:25.000000 pip-rating-0.1.0/pip_rating/req_files/setupcfg.py
--rw-r--r--   0 nekmo     (1000) users      (100)     1869 2023-07-17 01:53:25.000000 pip-rating-0.1.0/pip_rating/req_files/setuppy.py
--rw-r--r--   0 nekmo     (1000) users      (100)    10621 2023-07-20 01:02:43.000000 pip-rating-0.1.0/pip_rating/results.py
-drwxr-xr-x   0 nekmo     (1000) users      (100)        0 2023-07-20 20:38:52.143433 pip-rating-0.1.0/pip_rating/sources/
--rw-r--r--   0 nekmo     (1000) users      (100)        0 2023-07-07 14:57:52.000000 pip-rating-0.1.0/pip_rating/sources/__init__.py
--rw-r--r--   0 nekmo     (1000) users      (100)     2551 2023-07-17 01:53:25.000000 pip-rating-0.1.0/pip_rating/sources/audit.py
--rw-r--r--   0 nekmo     (1000) users      (100)     1283 2023-07-17 01:53:25.000000 pip-rating-0.1.0/pip_rating/sources/base.py
--rw-r--r--   0 nekmo     (1000) users      (100)     3065 2023-07-18 02:27:12.000000 pip-rating-0.1.0/pip_rating/sources/pypi.py
--rw-r--r--   0 nekmo     (1000) users      (100)     4494 2023-07-17 15:51:54.000000 pip-rating-0.1.0/pip_rating/sources/sourcecode_page.py
--rw-r--r--   0 nekmo     (1000) users      (100)     2592 2023-07-17 01:53:25.000000 pip-rating-0.1.0/pip_rating/sources/sourcerank.py
-drwxr-xr-x   0 nekmo     (1000) users      (100)        0 2023-07-20 20:38:52.140099 pip-rating-0.1.0/pip_rating.egg-info/
--rw-r--r--   0 nekmo     (1000) users      (100)     5761 2023-07-20 20:38:51.000000 pip-rating-0.1.0/pip_rating.egg-info/PKG-INFO
--rw-r--r--   0 nekmo     (1000) users      (100)     1007 2023-07-20 20:38:51.000000 pip-rating-0.1.0/pip_rating.egg-info/SOURCES.txt
--rw-r--r--   0 nekmo     (1000) users      (100)        1 2023-07-20 20:38:51.000000 pip-rating-0.1.0/pip_rating.egg-info/dependency_links.txt
--rw-r--r--   0 nekmo     (1000) users      (100)       60 2023-07-20 20:38:51.000000 pip-rating-0.1.0/pip_rating.egg-info/entry_points.txt
--rw-r--r--   0 nekmo     (1000) users      (100)        1 2023-07-20 20:38:50.000000 pip-rating-0.1.0/pip_rating.egg-info/not-zip-safe
--rw-r--r--   0 nekmo     (1000) users      (100)      232 2023-07-20 20:38:51.000000 pip-rating-0.1.0/pip_rating.egg-info/requires.txt
--rw-r--r--   0 nekmo     (1000) users      (100)       17 2023-07-20 20:38:51.000000 pip-rating-0.1.0/pip_rating.egg-info/top_level.txt
--rw-r--r--   0 nekmo     (1000) users      (100)      275 2023-06-30 01:00:25.000000 pip-rating-0.1.0/pyproject.toml
--rw-r--r--   0 nekmo     (1000) users      (100)      230 2023-07-09 18:44:41.000000 pip-rating-0.1.0/requirements.in
--rw-r--r--   0 nekmo     (1000) users      (100)     1834 2023-07-18 02:22:09.000000 pip-rating-0.1.0/requirements.txt
--rw-r--r--   0 nekmo     (1000) users      (100)     1668 2023-07-20 20:38:52.146766 pip-rating-0.1.0/setup.cfg
+drwxr-xr-x   0 nekmo     (1000) users      (100)        0 2023-08-07 01:39:53.053682 pip-rating-0.2.0/
+-rw-r--r--   0 nekmo     (1000) users      (100)      149 2023-08-07 00:58:30.000000 pip-rating-0.2.0/AUTHORS.rst
+-rw-r--r--   0 nekmo     (1000) users      (100)     3419 2023-08-07 00:58:30.000000 pip-rating-0.2.0/CONTRIBUTING.rst
+-rw-r--r--   0 nekmo     (1000) users      (100)      429 2023-08-07 01:18:19.000000 pip-rating-0.2.0/HISTORY.rst
+-rw-r--r--   0 nekmo     (1000) users      (100)     1065 2023-08-07 00:58:30.000000 pip-rating-0.2.0/LICENSE
+-rw-r--r--   0 nekmo     (1000) users      (100)      304 2023-08-07 00:58:30.000000 pip-rating-0.2.0/MANIFEST.in
+-rw-r--r--   0 nekmo     (1000) users      (100)     7274 2023-08-07 01:39:53.053682 pip-rating-0.2.0/PKG-INFO
+-rw-r--r--   0 nekmo     (1000) users      (100)     6189 2023-08-07 01:39:52.000000 pip-rating-0.2.0/README.rst
+drwxr-xr-x   0 nekmo     (1000) users      (100)        0 2023-08-07 01:39:53.050348 pip-rating-0.2.0/pip_rating/
+-rw-r--r--   0 nekmo     (1000) users      (100)      174 2023-08-07 01:19:52.000000 pip-rating-0.2.0/pip_rating/__init__.py
+-rw-r--r--   0 nekmo     (1000) users      (100)      690 2023-08-07 00:58:30.000000 pip-rating-0.2.0/pip_rating/_compat.py
+-rw-r--r--   0 nekmo     (1000) users      (100)     5432 2023-08-07 00:58:30.000000 pip-rating-0.2.0/pip_rating/dependencies.py
+-rw-r--r--   0 nekmo     (1000) users      (100)     1799 2023-08-07 00:58:30.000000 pip-rating-0.2.0/pip_rating/exceptions.py
+-rw-r--r--   0 nekmo     (1000) users      (100)     7046 2023-08-07 00:58:30.000000 pip-rating-0.2.0/pip_rating/management.py
+-rw-r--r--   0 nekmo     (1000) users      (100)     3525 2023-08-07 00:58:30.000000 pip-rating-0.2.0/pip_rating/packages.py
+-rw-r--r--   0 nekmo     (1000) users      (100)    11032 2023-08-07 00:58:30.000000 pip-rating-0.2.0/pip_rating/rating.py
+drwxr-xr-x   0 nekmo     (1000) users      (100)        0 2023-08-07 01:39:53.050348 pip-rating-0.2.0/pip_rating/req_files/
+-rw-r--r--   0 nekmo     (1000) users      (100)     1493 2023-08-07 00:58:30.000000 pip-rating-0.2.0/pip_rating/req_files/__init__.py
+-rw-r--r--   0 nekmo     (1000) users      (100)     1475 2023-08-07 00:58:30.000000 pip-rating-0.2.0/pip_rating/req_files/base.py
+-rw-r--r--   0 nekmo     (1000) users      (100)      909 2023-08-07 00:58:30.000000 pip-rating-0.2.0/pip_rating/req_files/package_list.py
+-rw-r--r--   0 nekmo     (1000) users      (100)     1018 2023-08-07 00:58:30.000000 pip-rating-0.2.0/pip_rating/req_files/pipfile.py
+-rw-r--r--   0 nekmo     (1000) users      (100)     3575 2023-08-07 00:58:30.000000 pip-rating-0.2.0/pip_rating/req_files/pyproject.py
+-rw-r--r--   0 nekmo     (1000) users      (100)     1916 2023-08-07 00:58:30.000000 pip-rating-0.2.0/pip_rating/req_files/requirements.py
+-rw-r--r--   0 nekmo     (1000) users      (100)     1077 2023-08-07 00:58:30.000000 pip-rating-0.2.0/pip_rating/req_files/setupcfg.py
+-rw-r--r--   0 nekmo     (1000) users      (100)     1869 2023-08-07 00:58:30.000000 pip-rating-0.2.0/pip_rating/req_files/setuppy.py
+-rw-r--r--   0 nekmo     (1000) users      (100)    16259 2023-08-07 00:58:30.000000 pip-rating-0.2.0/pip_rating/results.py
+drwxr-xr-x   0 nekmo     (1000) users      (100)        0 2023-08-07 01:39:53.053682 pip-rating-0.2.0/pip_rating/sources/
+-rw-r--r--   0 nekmo     (1000) users      (100)        0 2023-08-07 00:58:30.000000 pip-rating-0.2.0/pip_rating/sources/__init__.py
+-rw-r--r--   0 nekmo     (1000) users      (100)     2551 2023-08-07 00:58:30.000000 pip-rating-0.2.0/pip_rating/sources/audit.py
+-rw-r--r--   0 nekmo     (1000) users      (100)     1283 2023-08-07 00:58:30.000000 pip-rating-0.2.0/pip_rating/sources/base.py
+-rw-r--r--   0 nekmo     (1000) users      (100)     3065 2023-08-07 00:58:30.000000 pip-rating-0.2.0/pip_rating/sources/pypi.py
+-rw-r--r--   0 nekmo     (1000) users      (100)     4494 2023-08-07 00:58:30.000000 pip-rating-0.2.0/pip_rating/sources/sourcecode_page.py
+-rw-r--r--   0 nekmo     (1000) users      (100)     3372 2023-08-07 00:58:30.000000 pip-rating-0.2.0/pip_rating/sources/sourcerank.py
+drwxr-xr-x   0 nekmo     (1000) users      (100)        0 2023-08-07 01:39:53.050348 pip-rating-0.2.0/pip_rating.egg-info/
+-rw-r--r--   0 nekmo     (1000) users      (100)     7274 2023-08-07 01:39:52.000000 pip-rating-0.2.0/pip_rating.egg-info/PKG-INFO
+-rw-r--r--   0 nekmo     (1000) users      (100)     1007 2023-08-07 01:39:52.000000 pip-rating-0.2.0/pip_rating.egg-info/SOURCES.txt
+-rw-r--r--   0 nekmo     (1000) users      (100)        1 2023-08-07 01:39:52.000000 pip-rating-0.2.0/pip_rating.egg-info/dependency_links.txt
+-rw-r--r--   0 nekmo     (1000) users      (100)       60 2023-08-07 01:39:52.000000 pip-rating-0.2.0/pip_rating.egg-info/entry_points.txt
+-rw-r--r--   0 nekmo     (1000) users      (100)        1 2023-08-07 01:39:52.000000 pip-rating-0.2.0/pip_rating.egg-info/not-zip-safe
+-rw-r--r--   0 nekmo     (1000) users      (100)      232 2023-08-07 01:39:52.000000 pip-rating-0.2.0/pip_rating.egg-info/requires.txt
+-rw-r--r--   0 nekmo     (1000) users      (100)       17 2023-08-07 01:39:52.000000 pip-rating-0.2.0/pip_rating.egg-info/top_level.txt
+-rw-r--r--   0 nekmo     (1000) users      (100)      275 2023-08-07 00:58:30.000000 pip-rating-0.2.0/pyproject.toml
+-rw-r--r--   0 nekmo     (1000) users      (100)      230 2023-08-07 00:58:30.000000 pip-rating-0.2.0/requirements.in
+-rw-r--r--   0 nekmo     (1000) users      (100)     1835 2023-08-07 00:58:30.000000 pip-rating-0.2.0/requirements.txt
+-rw-r--r--   0 nekmo     (1000) users      (100)     1708 2023-08-07 01:39:53.053682 pip-rating-0.2.0/setup.cfg
```

### Comparing `pip-rating-0.1.0/CONTRIBUTING.rst` & `pip-rating-0.2.0/CONTRIBUTING.rst`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,15 @@
 
 #. The pull request should include tests.
 #. If the pull request adds functionality, the docs should be updated. Put
    your new functionality into a function with a docstring, update the docs
    directory and add the feature to the list in README.rst.
 #. The code must follow the PEP8 style guide, be clean, easy to read, elegant
    and be consistent with the rest of the code in the repository.
-#. The pull request should work for Python 3.8, 3.9, 3.10, 3.11 and for PyPy. Check
+#. The pull request should work for Python 3.8, 3.9, 3.10, 3.11, 3.12 and for PyPy. Check
    https://github.com/Nekmo/pip-rating/actions
    and make sure that the tests pass for all supported Python versions.
 
 Tips
 ----
 
 To run a subset of tests::
```

### Comparing `pip-rating-0.1.0/LICENSE` & `pip-rating-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pip-rating-0.1.0/README.rst` & `pip-rating-0.2.0/README.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 .. image:: https://raw.githubusercontent.com/Nekmo/pip-rating/master/logo.png
     :width: 100%
 
 |
 
+.. image:: https://raw.githubusercontent.com/Nekmo/pip-rating/pip-rating-badge/pip-rating-badge.svg
+  :target: https://github.com/Nekmo/pip-rating/actions/workflows/pip-rating.yml
+  :alt: pip-rating badge
+
 .. image:: https://img.shields.io/github/actions/workflow/status/Nekmo/pip-rating/test.yml?style=flat-square&maxAge=2592000&branch=master
   :target: https://github.com/Nekmo/pip-rating/actions?query=workflow%3ATests
   :alt: Latest Tests CI build status
 
 .. image:: https://img.shields.io/pypi/v/pip-rating.svg?style=flat-square
   :target: https://pypi.org/project/requirements-srating
   :alt: Latest PyPI version
@@ -19,15 +23,14 @@
   :target: https://codeclimate.com/github/Nekmo/pip-rating
   :alt: Code Climate
 
 .. image:: https://img.shields.io/codecov/c/github/Nekmo/pip-rating/master.svg?style=flat-square
   :target: https://codecov.io/github/Nekmo/pip-rating
   :alt: Test coverage
 
-
 ##########
 pip-rating
 ##########
 
 **Are the 📦 dependencies (and their dependencies) of your project secure and maintained?**
 
 
@@ -40,15 +43,15 @@
 .. code-block:: console
 
     $ pip install pip-rating
 
 This is the preferred method to install pip-rating, as it will always install the most recent stable release.
 If you don't have `pip <https://pip.pypa.io>`_ installed, this
 `Python installation guide <http://docs.python-guide.org/en/latest/starting/installation/>`_ can guide you through
-the process. 🐍 **Python 3.8-3.11** are tested and supported.
+the process. 🐍 **Python 3.8-3.12** are tested and supported.
 `More info in the documentation <https://docs.nekmo.org/pip-rating/installation.html>`_.
 
 Pip-rating is a tool **to check the security and maintenance of the dependencies of your project**. It will check the
 requirements of your project and **their dependencies recursively**, and will show you a rating for each of them. The
 rating is based on multiple factors, like their *last release date*, the *community activity*, well-known *security
 vulnerabilities* & more.
 
@@ -94,14 +97,54 @@
 
 To analyze one or more packages, you can use the command ``pip-rating analyze-package``:
 
 .. code-block:: console
 
     $ pip-rating analyze-package <package_name>[ <other_package_name>]
 
+⚡ Github Action
+================
+Pip-rating can be used as a *Github Action* to check the dependencies of your project in every commit and periodically.
+To use this github action add a file like this to your project in the path ``.github/workflows/pip-rating.yml``:
+
+.. code-block:: yaml
+
+    # .github/workflows/pip-rating.yml
+    # --------------------------------
+    name: Pip-rating
+
+    on:
+      push:
+        branches:
+          - master
+      schedule:
+        - cron: '0 0 * * SUN'
+
+    jobs:
+      build:
+        runs-on: ubuntu-latest
+        permissions: write-all
+        steps:
+          - uses: actions/checkout@v2
+          - name: Run pip-rating
+            uses: Nekmo/pip-rating@master
+            with:
+              create_badge: true
+              badge_style: flat-square
+              badge_branch: pip-rating-badge
+
+You can see the execution of the action in the "Actions" tab of your repository. The badge is generated in the
+``pip-rating-badge`` branch, so you can access it as:
+
+.. code-block:: text
+
+    https://raw.githubusercontent.com/<owner>/<repository>/pip-rating-badge/pip-rating-badge.svg
+
+For more info about the action, see the
+`Github Action documentation <https://docs.nekmo.org/pip-rating/github-action.html>`_.
 
 💡 Features
 ===========
 
 * Analyze the dependencies **recursively**.
 * Report of dependencies with **vulnerabilities**.
 * Rating according to the **age of the project** and the **date of the last release**.
```

### Comparing `pip-rating-0.1.0/pip_rating/_compat.py` & `pip-rating-0.2.0/pip_rating/_compat.py`

 * *Files identical despite different names*

### Comparing `pip-rating-0.1.0/pip_rating/dependencies.py` & `pip-rating-0.2.0/pip_rating/dependencies.py`

 * *Files identical despite different names*

### Comparing `pip-rating-0.1.0/pip_rating/exceptions.py` & `pip-rating-0.2.0/pip_rating/exceptions.py`

 * *Files identical despite different names*

### Comparing `pip-rating-0.1.0/pip_rating/management.py` & `pip-rating-0.2.0/pip_rating/management.py`

 * *Files 5% similar despite different names*

```diff
@@ -99,19 +99,24 @@
         help="Extra URLs of package indexes to use in addition to --index-url.",
     )(function)
     function = click.option(
         "--format",
         "-f",
         "format_name",
         type=click.Choice(FORMATS),
-        # envvar="PIP_EXTRA_INDEX_URL",  # let pip discover
         default="text",
         help=f"Output format. Supported formats: {', '.join(FORMATS)}. By default it uses 'text'.",
     )(function)
     function = click.option(
+        "--to-file",
+        "to_file",
+        type=click.Path(exists=False, dir_okay=False, resolve_path=True),
+        help="Output file. By default output to console.",
+    )(function)
+    function = click.option(
         "--ignore-package",
         "ignore_packages",
         type=str,
         multiple=True,
         help="Ignore a package. You can use this option multiple times.",
     )(function)
     return function
@@ -126,21 +131,22 @@
 def analyze_file(
     file: str,
     file_type: Optional[str],
     cache_dir: str,
     index_url: str,
     extra_index_url: str,
     format_name: str,
+    to_file: Optional[str],
     ignore_packages: List[str],
 ):
     """Analyze a requirements file. A requirements file is required as argument. By default, it tries to detect the
     type of the file, but you can force it using the ``--file-type`` option. The supported file types are:
     *requirements.txt, requirements.in, setup.py, setup.cfg, Pipfile and pyproject.toml*.
     """
-    results = Results()
+    results = Results(to_file)
     file = Path(file)
     if file_type is None:
         req_file_cls = get_req_file_cls(file)
     else:
         req_file_cls = REQ_FILE_CLASSES[file_type]
     results.status.update(f"Read requirements file [bold green]{file}[/bold green]")
     dependencies = Dependencies(
@@ -159,20 +165,21 @@
 @common_options
 def analyze_package(
     package_names: List[str],
     cache_dir: str,
     index_url: str,
     extra_index_url: str,
     format_name: str,
+    to_file: str,
     ignore_packages: List[str],
 ):
     """Analyze a package. A package name is required as argument. The syntax is the same as pip install. For example:
     ``Django==4.2.3``. If only one package is specified, it will show their dependencies in detail.
     """
-    results = Results()
+    results = Results(to_file)
     req_file = PackageList(package_names)
     dependencies = Dependencies(
         results,
         req_file,
         cache_dir,
         index_url,
         extra_index_url,
```

### Comparing `pip-rating-0.1.0/pip_rating/packages.py` & `pip-rating-0.2.0/pip_rating/packages.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
     @property
     def first_node_with_version(self) -> str:
         return f"{self.first_node.name}=={self.first_node.version}"
 
     @cached_property
     def sourcerank(self) -> SourceRank:
-        return SourceRank(self.name)
+        return SourceRank(self)
 
     @cached_property
     def pypi(self) -> "Pypi":
         return Pypi(self.name)
 
     @cached_property
     def sourcecode_page(self) -> "SourcecodePage":
```

### Comparing `pip-rating-0.1.0/pip_rating/rating.py` & `pip-rating-0.2.0/pip_rating/rating.py`

 * *Files identical despite different names*

### Comparing `pip-rating-0.1.0/pip_rating/req_files/__init__.py` & `pip-rating-0.2.0/pip_rating/req_files/__init__.py`

 * *Files identical despite different names*

### Comparing `pip-rating-0.1.0/pip_rating/req_files/base.py` & `pip-rating-0.2.0/pip_rating/req_files/base.py`

 * *Files identical despite different names*

### Comparing `pip-rating-0.1.0/pip_rating/req_files/package_list.py` & `pip-rating-0.2.0/pip_rating/req_files/package_list.py`

 * *Files identical despite different names*

### Comparing `pip-rating-0.1.0/pip_rating/req_files/pipfile.py` & `pip-rating-0.2.0/pip_rating/req_files/pipfile.py`

 * *Files identical despite different names*

### Comparing `pip-rating-0.1.0/pip_rating/req_files/pyproject.py` & `pip-rating-0.2.0/pip_rating/req_files/pyproject.py`

 * *Files identical despite different names*

### Comparing `pip-rating-0.1.0/pip_rating/req_files/requirements.py` & `pip-rating-0.2.0/pip_rating/req_files/requirements.py`

 * *Files identical despite different names*

### Comparing `pip-rating-0.1.0/pip_rating/req_files/setupcfg.py` & `pip-rating-0.2.0/pip_rating/req_files/setupcfg.py`

 * *Files identical despite different names*

### Comparing `pip-rating-0.1.0/pip_rating/req_files/setuppy.py` & `pip-rating-0.2.0/pip_rating/req_files/setuppy.py`

 * *Files identical despite different names*

### Comparing `pip-rating-0.1.0/pip_rating/sources/audit.py` & `pip-rating-0.2.0/pip_rating/sources/audit.py`

 * *Files identical despite different names*

### Comparing `pip-rating-0.1.0/pip_rating/sources/base.py` & `pip-rating-0.2.0/pip_rating/sources/base.py`

 * *Files identical despite different names*

### Comparing `pip-rating-0.1.0/pip_rating/sources/pypi.py` & `pip-rating-0.2.0/pip_rating/sources/pypi.py`

 * *Files identical despite different names*

### Comparing `pip-rating-0.1.0/pip_rating/sources/sourcecode_page.py` & `pip-rating-0.2.0/pip_rating/sources/sourcecode_page.py`

 * *Files identical despite different names*

### Comparing `pip-rating-0.1.0/pip_rating/sources/sourcerank.py` & `pip-rating-0.2.0/pip_rating/sources/sourcerank.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 import datetime
+import time
 from functools import cached_property
-from typing import Iterator, Tuple, TypedDict
+from typing import Iterator, Tuple, TypedDict, TYPE_CHECKING
 
 import requests
 from bs4 import BeautifulSoup
+from requests import RequestException
 
 from pip_rating.sources.base import SourceBase
 
+if TYPE_CHECKING:
+    from pip_rating.packages import Package
+
 SOURCERANK_URL = "https://libraries.io/pypi/{package_name}/sourcerank"
 BREAKDOWN_MAPPING = {
     "Basic info present?": "basic_info_present",
     "Source repository present?": "source_repository_present",
     "Readme present?": "readme_present",
     "License present?": "license_present",
     "Has multiple versions?": "has_multiple_versions",
@@ -21,14 +26,15 @@
     "Dependent Packages": "dependent_projects",
     "Dependent Repositories": "dependent_repositories",
     "Stars": "stars",
     "Contributors": "contributors",
     "Libraries.io subscribers": "librariesio_subscribers",
     "Total": "total",
 }
+RETRY_WAIT = 30
 
 
 class SourceRankBreakdown(TypedDict):
     basic_info_present: int
     source_repository_present: int
     readme_present: int
     license_present: int
@@ -50,14 +56,18 @@
     updated_at: str
     breakdown: SourceRankBreakdown
 
 
 class SourceRank(SourceBase):
     source_name = "sourcerank"
 
+    def __init__(self, package: "Package"):
+        self.package = package
+        super().__init__(package.name)
+
     def get_cache_data(self) -> dict:
         return {
             "package_name": self.package_name,
             "updated_at": datetime.datetime.now().isoformat(),
             "breakdown": dict(self.get_breakdown()),
         }
 
@@ -65,18 +75,29 @@
     def breakdown(self) -> SourceRankBreakdown:
         if not self.is_cache_expired:
             cache = self.get_from_cache()
         else:
             cache = self.save_to_cache()
         return cache["breakdown"]
 
-    def get_breakdown(self) -> Iterator[Tuple[str, int]]:
+    def request(self) -> bytes:
+        """Request the sourcerank page and return the content"""
         with requests.get(
             SOURCERANK_URL.format(package_name=self.package_name)
         ) as response:
-            response.raise_for_status()
-            content = response.content
-        soup = BeautifulSoup(content, "html.parser")
+            try:
+                response.raise_for_status()
+            except RequestException as e:
+                if e.response is not None and e.response.status_code == 429:
+                    self.package.dependencies.results.progress_console.print(
+                        f"Reached request limit for Sourcerank, waiting {RETRY_WAIT} seconds"
+                    )
+                    time.sleep(RETRY_WAIT)
+                    return self.request()
+            return response.content
+
+    def get_breakdown(self) -> Iterator[Tuple[str, int]]:
+        soup = BeautifulSoup(self.request(), "html.parser")
         for item in soup.find_all("li", "list-group-item"):
             stripped_strings = list(item.stripped_strings)
             if stripped_strings[1] in BREAKDOWN_MAPPING:
                 yield BREAKDOWN_MAPPING[stripped_strings[1]], int(stripped_strings[0])
```

### Comparing `pip-rating-0.1.0/pip_rating.egg-info/SOURCES.txt` & `pip-rating-0.2.0/pip_rating.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pip-rating-0.1.0/requirements.txt` & `pip-rating-0.2.0/requirements.txt`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 anytree==2.9.0
     # via pipgrip
 beautifulsoup4==4.12.2
     # via -r requirements.in
 cachecontrol[filecache]==0.13.1
     # via pip-audit
-certifi==2023.5.7
+certifi==2023.7.22
     # via requests
 charset-normalizer==3.2.0
     # via requests
 click==8.1.4
     # via pipgrip
 cyclonedx-python-lib==4.0.1
     # via pip-audit
```

### Comparing `pip-rating-0.1.0/setup.cfg` & `pip-rating-0.2.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 [bumpversion]
-current_version = 0.1.0
+current_version = 0.2.0
 commit = True
 tag = True
 
 [metadata]
 name = pip-rating
 version = attr: pip_rating.__version__
 description = Check the health of your project's requirements and get a rating for each dependency.
-long-description = file: README.rst
+long_description = file: README.rst
 keywords = pip-rating
 author = Nekmo
-author-email = contacto@nekmo.com
+author_email = contacto@nekmo.com
 url = https://github.com/Nekmo/pip-rating/
 download_url = https://github.com/Nekmo/pip-rating/archive/master.zip
 license = MIT license
-license-files = 
+license_files = 
 	LICENSE
 platform = any
 classifiers = 
 	Development Status :: 3 - Alpha
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	Operating System :: POSIX :: Linux
 	Operating System :: MacOS :: MacOS X
 	Operating System :: Microsoft :: Windows
 	Operating System :: POSIX :: SunOS/Solaris
 	Operating System :: POSIX :: BSD
 	License :: OSI Approved :: MIT License
 	Natural Language :: English
```

