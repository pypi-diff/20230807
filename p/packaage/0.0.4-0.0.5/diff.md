# Comparing `tmp/packaage-0.0.4.tar.gz` & `tmp/packaage-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/packaage-0.0.4.tar", last modified: Wed Nov 18 16:37:23 2020, max compression
+gzip compressed data, was "packaage-0.0.5.tar", last modified: Mon Aug  7 09:09:41 2023, max compression
```

## Comparing `packaage-0.0.4.tar` & `packaage-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxr-xr-x   0 datalody   (501) staff       (20)        0 2020-11-18 16:37:23.742689 packaage-0.0.4/
--rw-r--r--   0 datalody   (501) staff       (20)     1165 2020-11-18 16:37:23.742195 packaage-0.0.4/PKG-INFO
--rw-r--r--   0 datalody   (501) staff       (20)      661 2020-11-18 16:33:06.000000 packaage-0.0.4/README.md
-drwxr-xr-x   0 datalody   (501) staff       (20)        0 2020-11-18 16:37:23.738773 packaage-0.0.4/packaage/
--rw-r--r--   0 datalody   (501) staff       (20)       61 2020-11-18 16:37:08.000000 packaage-0.0.4/packaage/__init__.py
--rw-r--r--   0 datalody   (501) staff       (20)       12 2020-11-18 13:20:06.000000 packaage-0.0.4/packaage/life.py
--rw-r--r--   0 datalody   (501) staff       (20)      406 2020-11-18 16:37:02.000000 packaage-0.0.4/packaage/utils.py
-drwxr-xr-x   0 datalody   (501) staff       (20)        0 2020-11-18 16:37:23.740774 packaage-0.0.4/packaage.egg-info/
--rw-r--r--   0 datalody   (501) staff       (20)     1165 2020-11-18 16:37:23.000000 packaage-0.0.4/packaage.egg-info/PKG-INFO
--rw-r--r--   0 datalody   (501) staff       (20)      233 2020-11-18 16:37:23.000000 packaage-0.0.4/packaage.egg-info/SOURCES.txt
--rw-r--r--   0 datalody   (501) staff       (20)        1 2020-11-18 16:37:23.000000 packaage-0.0.4/packaage.egg-info/dependency_links.txt
--rw-r--r--   0 datalody   (501) staff       (20)       10 2020-11-18 16:37:23.000000 packaage-0.0.4/packaage.egg-info/requires.txt
--rw-r--r--   0 datalody   (501) staff       (20)        9 2020-11-18 16:37:23.000000 packaage-0.0.4/packaage.egg-info/top_level.txt
--rw-r--r--   0 datalody   (501) staff       (20)       38 2020-11-18 16:37:23.742890 packaage-0.0.4/setup.cfg
--rw-r--r--   0 datalody   (501) staff       (20)      571 2020-11-18 16:33:56.000000 packaage-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 09:09:41.478490 packaage-0.0.5/
+-rw-rw-rw-   0        0        0        0 2023-07-20 08:12:44.000000 packaage-0.0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0      883 2023-08-07 09:09:41.477501 packaage-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      697 2023-07-20 08:12:44.000000 packaage-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-08-07 09:09:41.449979 packaage-0.0.5/packaage/
+-rw-rw-rw-   0        0        0       66 2023-07-20 13:19:06.000000 packaage-0.0.5/packaage/__init__.py
+-rw-rw-rw-   0        0        0     1651 2023-07-20 13:19:06.000000 packaage-0.0.5/packaage/database.py
+-rw-rw-rw-   0        0        0       95 2023-07-20 08:12:44.000000 packaage-0.0.5/packaage/life.py
+-rw-rw-rw-   0        0        0      622 2023-07-20 08:12:44.000000 packaage-0.0.5/packaage/test.py
+-rw-rw-rw-   0        0        0      623 2023-07-20 08:12:44.000000 packaage-0.0.5/packaage/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-07 09:09:41.475458 packaage-0.0.5/packaage.egg-info/
+-rw-rw-rw-   0        0        0      883 2023-08-07 09:09:41.000000 packaage-0.0.5/packaage.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2023-08-07 09:09:41.000000 packaage-0.0.5/packaage.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 09:09:41.000000 packaage-0.0.5/packaage.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-08-07 09:09:41.000000 packaage-0.0.5/packaage.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-08-07 09:09:41.000000 packaage-0.0.5/packaage.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-07 09:09:41.478490 packaage-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      620 2023-07-20 13:19:06.000000 packaage-0.0.5/setup.py
```

### Comparing `packaage-0.0.4/setup.py` & `packaage-0.0.5/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-import pathlib
-from setuptools import setup
-from packaage.__init__ import __version__
-
-# The directory containing this file
-HERE = pathlib.Path(__file__).parent
-
-# The text of the README file
-README = (HERE / "README.md").read_text()
-
-# This call to setup() does all the work
-setup(
-    name="packaage",
-    version=__version__,
-    description='Packaage is a Python library with few AI utils',
-    long_description=README,
-    long_description_content_type="text/markdown",
-    packages=["packaage"],
-    install_requires=['unidecode'],
-    include_package_data=True,
-)
+import pathlib
+from setuptools import setup
+from packaage.__init__ import __version__
+
+# The directory containing this file
+HERE = pathlib.Path(__file__).parent
+
+# The text of the README file
+README = (HERE / "README.md").read_text()
+
+# This call to setup() does all the work
+setup(
+    name="packaage",
+    version=__version__,
+    description='Packaage is a Python library with few AI utils',
+    long_description=README,
+    long_description_content_type="text/markdown",
+    packages=["packaage"],
+    install_requires=['unidecode', 'boto3', 'psycopg2-binary'],
+    include_package_data=True,
+)
```

