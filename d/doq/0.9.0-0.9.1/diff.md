# Comparing `tmp/doq-0.9.0.tar.gz` & `tmp/doq-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/doq-0.9.0.tar", last modified: Wed Nov  3 14:01:31 2021, max compression
+gzip compressed data, was "doq-0.9.1.tar", last modified: Fri Jan  7 15:12:28 2022, max compression
```

## Comparing `doq-0.9.0.tar` & `doq-0.9.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 s_ohyanagi   (501) admin       (80)        0 2021-11-03 14:01:31.000000 doq-0.9.0/
--rw-r--r--   0 s_ohyanagi   (501) admin       (80)     1526 2020-02-01 16:58:56.000000 doq-0.9.0/LICENSE
--rw-r--r--   0 s_ohyanagi   (501) admin       (80)      333 2020-02-09 15:22:27.000000 doq-0.9.0/MANIFEST.in
--rw-r--r--   0 s_ohyanagi   (501) admin       (80)     7361 2021-11-03 14:01:31.000000 doq-0.9.0/PKG-INFO
--rw-r--r--   0 s_ohyanagi   (501) admin       (80)     5189 2021-11-03 13:54:12.000000 doq-0.9.0/README.rst
-drwxr-xr-x   0 s_ohyanagi   (501) admin       (80)        0 2021-11-03 14:01:31.000000 doq-0.9.0/doq/
--rw-r--r--   0 s_ohyanagi   (501) admin       (80)      241 2021-11-03 14:01:17.000000 doq-0.9.0/doq/__init__.py
--rw-r--r--   0 s_ohyanagi   (501) admin       (80)    10127 2021-11-03 13:54:12.000000 doq-0.9.0/doq/cli.py
--rw-r--r--   0 s_ohyanagi   (501) admin       (80)     2353 2021-11-03 13:54:12.000000 doq-0.9.0/doq/config.py
--rw-r--r--   0 s_ohyanagi   (501) admin       (80)     2435 2021-10-12 13:30:26.000000 doq-0.9.0/doq/outputter.py
--rw-r--r--   0 s_ohyanagi   (501) admin       (80)     5416 2021-10-12 13:30:26.000000 doq-0.9.0/doq/parser.py
--rw-r--r--   0 s_ohyanagi   (501) admin       (80)      435 2021-08-21 16:49:29.000000 doq-0.9.0/doq/template.py
-drwxr-xr-x   0 s_ohyanagi   (501) admin       (80)        0 2021-11-03 14:01:31.000000 doq-0.9.0/doq/templates/
-drwxr-xr-x   0 s_ohyanagi   (501) admin       (80)        0 2021-11-03 14:01:31.000000 doq-0.9.0/doq/templates/google/
--rw-r--r--   0 s_ohyanagi   (501) admin       (80)       20 2020-02-01 12:12:34.000000 doq-0.9.0/doq/templates/google/class.txt
--rw-r--r--   0 s_ohyanagi   (501) admin       (80)      232 2020-02-11 07:49:26.000000 doq-0.9.0/doq/templates/google/def.txt
--rw-r--r--   0 s_ohyanagi   (501) admin       (80)       19 2020-02-01 13:20:46.000000 doq-0.9.0/doq/templates/google/noarg.txt
-drwxr-xr-x   0 s_ohyanagi   (501) admin       (80)        0 2021-11-03 14:01:31.000000 doq-0.9.0/doq/templates/numpy/
--rw-r--r--   0 s_ohyanagi   (501) admin       (80)       20 2020-02-01 12:12:30.000000 doq-0.9.0/doq/templates/numpy/class.txt
--rw-r--r--   0 s_ohyanagi   (501) admin       (80)      239 2020-02-09 02:25:51.000000 doq-0.9.0/doq/templates/numpy/def.txt
--rw-r--r--   0 s_ohyanagi   (501) admin       (80)       19 2020-02-01 12:03:23.000000 doq-0.9.0/doq/templates/numpy/noarg.txt
-drwxr-xr-x   0 s_ohyanagi   (501) admin       (80)        0 2021-11-03 14:01:31.000000 doq-0.9.0/doq/templates/sphinx/
--rw-r--r--   0 s_ohyanagi   (501) admin       (80)       19 2021-10-07 08:14:52.000000 doq-0.9.0/doq/templates/sphinx/class.txt
--rw-r--r--   0 s_ohyanagi   (501) admin       (80)      222 2021-03-25 11:45:58.000000 doq-0.9.0/doq/templates/sphinx/def.txt
--rw-r--r--   0 s_ohyanagi   (501) admin       (80)       18 2020-02-01 05:01:33.000000 doq-0.9.0/doq/templates/sphinx/noarg.txt
-drwxr-xr-x   0 s_ohyanagi   (501) admin       (80)        0 2021-11-03 14:01:31.000000 doq-0.9.0/doq.egg-info/
--rw-r--r--   0 s_ohyanagi   (501) admin       (80)     7361 2021-11-03 14:01:31.000000 doq-0.9.0/doq.egg-info/PKG-INFO
--rw-r--r--   0 s_ohyanagi   (501) admin       (80)      700 2021-11-03 14:01:31.000000 doq-0.9.0/doq.egg-info/SOURCES.txt
--rw-r--r--   0 s_ohyanagi   (501) admin       (80)        1 2021-11-03 14:01:31.000000 doq-0.9.0/doq.egg-info/dependency_links.txt
--rw-r--r--   0 s_ohyanagi   (501) admin       (80)       50 2021-11-03 14:01:31.000000 doq-0.9.0/doq.egg-info/entry_points.txt
--rw-r--r--   0 s_ohyanagi   (501) admin       (80)       18 2021-11-03 14:01:31.000000 doq-0.9.0/doq.egg-info/requires.txt
--rw-r--r--   0 s_ohyanagi   (501) admin       (80)       10 2021-11-03 14:01:31.000000 doq-0.9.0/doq.egg-info/top_level.txt
--rw-r--r--   0 s_ohyanagi   (501) admin       (80)      395 2021-11-03 14:01:31.000000 doq-0.9.0/setup.cfg
--rw-r--r--   0 s_ohyanagi   (501) admin       (80)     1480 2021-11-03 13:54:12.000000 doq-0.9.0/setup.py
-drwxr-xr-x   0 s_ohyanagi   (501) admin       (80)        0 2021-11-03 14:01:31.000000 doq-0.9.0/tests/
-drwxr-xr-x   0 s_ohyanagi   (501) admin       (80)        0 2021-11-03 14:01:31.000000 doq-0.9.0/tests/expected/
--rw-r--r--   0 s_ohyanagi   (501) admin       (80)        0 2020-02-01 10:54:34.000000 doq-0.9.0/tests/expected/__init__.py
+drwxr-xr-x   0 s_ohyanagi   (501) admin       (80)        0 2022-01-07 15:12:28.636470 doq-0.9.1/
+-rw-r--r--   0 s_ohyanagi   (501) admin       (80)     1526 2020-02-01 16:58:56.000000 doq-0.9.1/LICENSE
+-rw-r--r--   0 s_ohyanagi   (501) admin       (80)      333 2020-02-09 15:22:27.000000 doq-0.9.1/MANIFEST.in
+-rw-r--r--   0 s_ohyanagi   (501) admin       (80)     5788 2022-01-07 15:12:28.636515 doq-0.9.1/PKG-INFO
+-rw-r--r--   0 s_ohyanagi   (501) admin       (80)     5189 2022-01-03 10:09:09.000000 doq-0.9.1/README.rst
+drwxr-xr-x   0 s_ohyanagi   (501) admin       (80)        0 2022-01-07 15:12:28.634666 doq-0.9.1/doq/
+-rw-r--r--   0 s_ohyanagi   (501) admin       (80)      241 2022-01-07 15:11:51.000000 doq-0.9.1/doq/__init__.py
+-rw-r--r--   0 s_ohyanagi   (501) admin       (80)    10127 2022-01-03 10:09:09.000000 doq-0.9.1/doq/cli.py
+-rw-r--r--   0 s_ohyanagi   (501) admin       (80)     2353 2021-11-04 07:39:41.000000 doq-0.9.1/doq/config.py
+-rw-r--r--   0 s_ohyanagi   (501) admin       (80)     2435 2022-01-03 10:09:09.000000 doq-0.9.1/doq/outputter.py
+-rw-r--r--   0 s_ohyanagi   (501) admin       (80)     5541 2022-01-07 15:06:53.000000 doq-0.9.1/doq/parser.py
+-rw-r--r--   0 s_ohyanagi   (501) admin       (80)      435 2021-08-21 16:49:29.000000 doq-0.9.1/doq/template.py
+drwxr-xr-x   0 s_ohyanagi   (501) admin       (80)        0 2022-01-07 15:12:28.633582 doq-0.9.1/doq/templates/
+drwxr-xr-x   0 s_ohyanagi   (501) admin       (80)        0 2022-01-07 15:12:28.635780 doq-0.9.1/doq/templates/google/
+-rw-r--r--   0 s_ohyanagi   (501) admin       (80)       20 2020-02-01 12:12:34.000000 doq-0.9.1/doq/templates/google/class.txt
+-rw-r--r--   0 s_ohyanagi   (501) admin       (80)      232 2020-02-11 07:49:26.000000 doq-0.9.1/doq/templates/google/def.txt
+-rw-r--r--   0 s_ohyanagi   (501) admin       (80)       19 2020-02-01 13:20:46.000000 doq-0.9.1/doq/templates/google/noarg.txt
+drwxr-xr-x   0 s_ohyanagi   (501) admin       (80)        0 2022-01-07 15:12:28.636093 doq-0.9.1/doq/templates/numpy/
+-rw-r--r--   0 s_ohyanagi   (501) admin       (80)       20 2020-02-01 12:12:30.000000 doq-0.9.1/doq/templates/numpy/class.txt
+-rw-r--r--   0 s_ohyanagi   (501) admin       (80)      239 2020-02-09 02:25:51.000000 doq-0.9.1/doq/templates/numpy/def.txt
+-rw-r--r--   0 s_ohyanagi   (501) admin       (80)       19 2020-02-01 12:03:23.000000 doq-0.9.1/doq/templates/numpy/noarg.txt
+drwxr-xr-x   0 s_ohyanagi   (501) admin       (80)        0 2022-01-07 15:12:28.636383 doq-0.9.1/doq/templates/sphinx/
+-rw-r--r--   0 s_ohyanagi   (501) admin       (80)       19 2021-10-07 08:14:52.000000 doq-0.9.1/doq/templates/sphinx/class.txt
+-rw-r--r--   0 s_ohyanagi   (501) admin       (80)      222 2021-03-25 11:45:58.000000 doq-0.9.1/doq/templates/sphinx/def.txt
+-rw-r--r--   0 s_ohyanagi   (501) admin       (80)       18 2020-02-01 05:01:33.000000 doq-0.9.1/doq/templates/sphinx/noarg.txt
+drwxr-xr-x   0 s_ohyanagi   (501) admin       (80)        0 2022-01-07 15:12:28.635473 doq-0.9.1/doq.egg-info/
+-rw-r--r--   0 s_ohyanagi   (501) admin       (80)     5788 2022-01-07 15:12:28.000000 doq-0.9.1/doq.egg-info/PKG-INFO
+-rw-r--r--   0 s_ohyanagi   (501) admin       (80)      700 2022-01-07 15:12:28.000000 doq-0.9.1/doq.egg-info/SOURCES.txt
+-rw-r--r--   0 s_ohyanagi   (501) admin       (80)        1 2022-01-07 15:12:28.000000 doq-0.9.1/doq.egg-info/dependency_links.txt
+-rw-r--r--   0 s_ohyanagi   (501) admin       (80)       50 2022-01-07 15:12:28.000000 doq-0.9.1/doq.egg-info/entry_points.txt
+-rw-r--r--   0 s_ohyanagi   (501) admin       (80)       18 2022-01-07 15:12:28.000000 doq-0.9.1/doq.egg-info/requires.txt
+-rw-r--r--   0 s_ohyanagi   (501) admin       (80)       10 2022-01-07 15:12:28.000000 doq-0.9.1/doq.egg-info/top_level.txt
+-rw-r--r--   0 s_ohyanagi   (501) admin       (80)      395 2022-01-07 15:12:28.636746 doq-0.9.1/setup.cfg
+-rw-r--r--   0 s_ohyanagi   (501) admin       (80)     1480 2021-11-04 07:39:41.000000 doq-0.9.1/setup.py
+drwxr-xr-x   0 s_ohyanagi   (501) admin       (80)        0 2022-01-07 15:12:28.633307 doq-0.9.1/tests/
+drwxr-xr-x   0 s_ohyanagi   (501) admin       (80)        0 2022-01-07 15:12:28.634779 doq-0.9.1/tests/expected/
+-rw-r--r--   0 s_ohyanagi   (501) admin       (80)        0 2020-02-01 10:54:34.000000 doq-0.9.1/tests/expected/__init__.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `doq-0.9.0/LICENSE` & `doq-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `doq-0.9.0/PKG-INFO` & `doq-0.9.1/README.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,216 +1,198 @@
-Metadata-Version: 1.1
-Name: doq
-Version: 0.9.0
-Summary: Docstring generator
-Home-page: http://github.com/heavenshell/py-doq
-Author: Shinya Ohyanagi
-Author-email: sohyanagi@gmail.com
-License: BSD
-Description: doq
-        ---
-        
-        .. image:: https://github.com/heavenshell/py-doq/workflows/build/badge.svg
-            :target: https://github.com/heavenshell/py-doq/actions
-        
-        .. image:: https://pyup.io/repos/github/heavenshell/py-doq/python-3-shield.svg
-            :target: https://pyup.io/repos/github/heavenshell/py-doq/
-            :alt: Python 3
-        
-        .. image:: https://pyup.io/repos/github/heavenshell/py-doq/shield.svg
-            :target: https://pyup.io/repos/github/heavenshell/py-doq/
-            :alt: Updates
-        
-        Docstring generator.
-        
-        Installation
-        ============
-        
-        .. code::
-        
-          $ pip install doq
-        
-        How to use
-        ==========
-        
-        .. code::
-        
-          $ cat spam.py
-          def spam(arg1, arg2: str) -> str:
-              pass
-        
-        .. code::
-        
-          $ cat spam.py | doq
-          def spam(arg1, arg2: str) -> str:
-            """spam.
-        
-            :param arg1:
-            :param arg2:
-            :type arg2: str
-            :rtype: str
-            """
-            pass
-        
-        Default formatter is `sphinx`. You can choose `sphinx`, `google` or `numpy`.
-        
-        .. code::
-        
-          $ cat spam.py | doq --formatter=google
-          def spam(arg1, arg2: str) -> str:
-            """spam.
-        
-            Args:
-                arg1 : arg1
-                arg2 (str): arg2
-        
-            Returns:
-                str:
-            """
-            pass
-        
-        .. code::
-        
-          $ cat spam.py | doq --formatter=numpy
-          def spam(arg1, arg2: str) -> str:
-            """spam.
-        
-            Parameters
-            ----------
-            arg1
-                  arg1
-            arg2 : str
-                 arg2
-        
-            Returns
-            -------
-            str
-        
-            """
-            pass
-        
-        Usage
-        =====
-        
-        .. code::
-        
-            $ python -m doq.cli --help
-            usage: doq [-h] [-f FILE] [--start START] [--end END] [-t TEMPLATE_PATH]
-                       [-s STYLE] [--formatter FORMATTER] [--indent INDENT] [--omit OMIT]
-                       [-r] [-d DIRECTORY] [-w] [-v] [-c CONFIG] [--ignore_exception]
-                       [--ignore_yield] [--ignore_init]
-        
-            Docstring generator.
-        
-            optional arguments:
-              -h, --help            show this help message and exit
-              -f FILE, --file FILE  File or STDIN
-              --start START         Start lineno
-              --end END             End lineno
-              -t TEMPLATE_PATH, --template_path TEMPLATE_PATH
-                                    Path to template directory
-              -s STYLE, --style STYLE
-                                    Output style string or json
-              --formatter FORMATTER
-                                    Docstring formatter. sphinx,google or numpy
-              --indent INDENT       Indent number
-              --omit OMIT           Omit first argument such as self
-              -r, --recursive       Run recursively over directories
-              -d DIRECTORY, --directory DIRECTORY
-                                    Path to directory
-              -w, --write           Edit files in-place
-              -v, --version         Output the version number
-              -c CONFIG, --config CONFIG
-                                    Path to a setup.cfg or pyproject.toml
-              --ignore_exception    Ignore exception statements
-              --ignore_yield        Ignore yield statements
-              --ignore_init         Ignore generate docstring to __init__ method
-        
-        Customize template
-        ==================
-        
-        doq use Jinja2 template. So you can create your own template.
-        
-        .. note::
-        
-            You must create 3 template files.
-        
-        +-----------+-----------------------------------------+
-        | File name | Description                             |
-        +===========+=========================================+
-        | class.txt | class docstring                         |
-        +-----------+-----------------------------------------+
-        | def.txt   | def / method docstring                  |
-        +-----------+-----------------------------------------+
-        | noarg.txt | def / method without argument docstring |
-        +-----------+-----------------------------------------+
-        
-        Available Jinja2's variable
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        +--------------------------+---------------------------+
-        | Name                     | Description               |
-        +==========================+===========================+
-        | name                     | class, method, def's name |
-        +-------------+------------+---------------------------+
-        | params      | argument   | Method, def's argument    |
-        |             +------------+---------------------------+
-        |             | annotation | Argument's type hint      |
-        |             +------------+---------------------------+
-        |             | default    | Defaut keyword argument   |
-        +-------------+------------+---------------------------+
-        | exceptions               | List of exception         |
-        +--------------------------+---------------------------+
-        | yields                   | List of yield             |
-        +--------------------------+---------------------------+
-        | return_type              | Return type hint          |
-        +--------------------------+---------------------------+
-        
-        See `examples <https://github.com/heavenshell/py-doq/tree/master/examples>`_
-        
-        Configuration
-        =============
-        
-        doq will automatically search ``setup.cfg`` or ``pyproject.toml`` in your
-        project.
-        
-        .. note::
-        
-            ignore_exception, ignore_exception and ignore_init can set `true` only.
-            If you want turn off, remove from configuration.
-        
-        setup.cfg
-        ~~~~~~~~~
-        
-        The section must be ``[doq]``.
-        
-        configuration file example::
-        
-          [doq]
-          style = "json"
-          template_path = "/path/to/template"
-        
-        pyproject.toml
-        ~~~~~~~~~~~~~~
-        
-        The section must be ``[tool.doq]``.
-        
-        configuration file example::
-        
-          [tool.doq]
-          style = "json"
-          template_path = "/path/to/template"
-        
-        LICENSE
-        =======
-        
-        NEW BSD LICENSE.
-        
-Platform: any
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Web Environment
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Topic :: Documentation
-Classifier: Topic :: Software Development :: Documentation
+doq
+---
+
+.. image:: https://github.com/heavenshell/py-doq/workflows/build/badge.svg
+    :target: https://github.com/heavenshell/py-doq/actions
+
+.. image:: https://pyup.io/repos/github/heavenshell/py-doq/python-3-shield.svg
+    :target: https://pyup.io/repos/github/heavenshell/py-doq/
+    :alt: Python 3
+
+.. image:: https://pyup.io/repos/github/heavenshell/py-doq/shield.svg
+    :target: https://pyup.io/repos/github/heavenshell/py-doq/
+    :alt: Updates
+
+Docstring generator.
+
+Installation
+============
+
+.. code::
+
+  $ pip install doq
+
+How to use
+==========
+
+.. code::
+
+  $ cat spam.py
+  def spam(arg1, arg2: str) -> str:
+      pass
+
+.. code::
+
+  $ cat spam.py | doq
+  def spam(arg1, arg2: str) -> str:
+    """spam.
+
+    :param arg1:
+    :param arg2:
+    :type arg2: str
+    :rtype: str
+    """
+    pass
+
+Default formatter is `sphinx`. You can choose `sphinx`, `google` or `numpy`.
+
+.. code::
+
+  $ cat spam.py | doq --formatter=google
+  def spam(arg1, arg2: str) -> str:
+    """spam.
+
+    Args:
+        arg1 : arg1
+        arg2 (str): arg2
+
+    Returns:
+        str:
+    """
+    pass
+
+.. code::
+
+  $ cat spam.py | doq --formatter=numpy
+  def spam(arg1, arg2: str) -> str:
+    """spam.
+
+    Parameters
+    ----------
+    arg1
+          arg1
+    arg2 : str
+         arg2
+
+    Returns
+    -------
+    str
+
+    """
+    pass
+
+Usage
+=====
+
+.. code::
+
+    $ python -m doq.cli --help
+    usage: doq [-h] [-f FILE] [--start START] [--end END] [-t TEMPLATE_PATH]
+               [-s STYLE] [--formatter FORMATTER] [--indent INDENT] [--omit OMIT]
+               [-r] [-d DIRECTORY] [-w] [-v] [-c CONFIG] [--ignore_exception]
+               [--ignore_yield] [--ignore_init]
+
+    Docstring generator.
+
+    optional arguments:
+      -h, --help            show this help message and exit
+      -f FILE, --file FILE  File or STDIN
+      --start START         Start lineno
+      --end END             End lineno
+      -t TEMPLATE_PATH, --template_path TEMPLATE_PATH
+                            Path to template directory
+      -s STYLE, --style STYLE
+                            Output style string or json
+      --formatter FORMATTER
+                            Docstring formatter. sphinx,google or numpy
+      --indent INDENT       Indent number
+      --omit OMIT           Omit first argument such as self
+      -r, --recursive       Run recursively over directories
+      -d DIRECTORY, --directory DIRECTORY
+                            Path to directory
+      -w, --write           Edit files in-place
+      -v, --version         Output the version number
+      -c CONFIG, --config CONFIG
+                            Path to a setup.cfg or pyproject.toml
+      --ignore_exception    Ignore exception statements
+      --ignore_yield        Ignore yield statements
+      --ignore_init         Ignore generate docstring to __init__ method
+
+Customize template
+==================
+
+doq use Jinja2 template. So you can create your own template.
+
+.. note::
+
+    You must create 3 template files.
+
++-----------+-----------------------------------------+
+| File name | Description                             |
++===========+=========================================+
+| class.txt | class docstring                         |
++-----------+-----------------------------------------+
+| def.txt   | def / method docstring                  |
++-----------+-----------------------------------------+
+| noarg.txt | def / method without argument docstring |
++-----------+-----------------------------------------+
+
+Available Jinja2's variable
+~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
++--------------------------+---------------------------+
+| Name                     | Description               |
++==========================+===========================+
+| name                     | class, method, def's name |
++-------------+------------+---------------------------+
+| params      | argument   | Method, def's argument    |
+|             +------------+---------------------------+
+|             | annotation | Argument's type hint      |
+|             +------------+---------------------------+
+|             | default    | Defaut keyword argument   |
++-------------+------------+---------------------------+
+| exceptions               | List of exception         |
++--------------------------+---------------------------+
+| yields                   | List of yield             |
++--------------------------+---------------------------+
+| return_type              | Return type hint          |
++--------------------------+---------------------------+
+
+See `examples <https://github.com/heavenshell/py-doq/tree/master/examples>`_
+
+Configuration
+=============
+
+doq will automatically search ``setup.cfg`` or ``pyproject.toml`` in your
+project.
+
+.. note::
+
+    ignore_exception, ignore_exception and ignore_init can set `true` only.
+    If you want turn off, remove from configuration.
+
+setup.cfg
+~~~~~~~~~
+
+The section must be ``[doq]``.
+
+configuration file example::
+
+  [doq]
+  style = "json"
+  template_path = "/path/to/template"
+
+pyproject.toml
+~~~~~~~~~~~~~~
+
+The section must be ``[tool.doq]``.
+
+configuration file example::
+
+  [tool.doq]
+  style = "json"
+  template_path = "/path/to/template"
+
+LICENSE
+=======
+
+NEW BSD LICENSE.
```

### Comparing `doq-0.9.0/README.rst` & `doq-0.9.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: doq
+Version: 0.9.1
+Summary: Docstring generator
+Home-page: http://github.com/heavenshell/py-doq
+Author: Shinya Ohyanagi
+Author-email: sohyanagi@gmail.com
+License: BSD
+Platform: any
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Web Environment
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Topic :: Documentation
+Classifier: Topic :: Software Development :: Documentation
+License-File: LICENSE
+
 doq
 ---
 
 .. image:: https://github.com/heavenshell/py-doq/workflows/build/badge.svg
     :target: https://github.com/heavenshell/py-doq/actions
 
 .. image:: https://pyup.io/repos/github/heavenshell/py-doq/python-3-shield.svg
@@ -192,7 +211,9 @@
   style = "json"
   template_path = "/path/to/template"
 
 LICENSE
 =======
 
 NEW BSD LICENSE.
+
+
```

### Comparing `doq-0.9.0/doq/cli.py` & `doq-0.9.1/doq/cli.py`

 * *Files identical despite different names*

### Comparing `doq-0.9.0/doq/config.py` & `doq-0.9.1/doq/config.py`

 * *Files identical despite different names*

### Comparing `doq-0.9.0/doq/outputter.py` & `doq-0.9.1/doq/outputter.py`

 * *Files identical despite different names*

### Comparing `doq-0.9.0/doq/parser.py` & `doq-0.9.1/doq/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,18 @@
         if ignore_yield is False:
             for y in d.iter_yield_exprs():
                 yields.append(y.children[1].get_first_leaf().value)
 
         exceptions = []
         if ignore_exception is False:
             for e in d.iter_raise_stmts():
-                exceptions.append(e.children[1].get_first_leaf().get_code().strip())
+                if hasattr(e, 'children'):
+                    exceptions.append(e.children[1].get_first_leaf().get_code().strip())
+                else:  # bare raise
+                    exceptions.append('')
 
         results.append(
             {
                 'name': name,
                 'params': params,
                 'return_type': return_type,
                 'start_lineno': start_lineno,
```

### Comparing `doq-0.9.0/doq.egg-info/SOURCES.txt` & `doq-0.9.1/doq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `doq-0.9.0/setup.py` & `doq-0.9.1/setup.py`

 * *Files identical despite different names*

