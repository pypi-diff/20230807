# Comparing `tmp/calfcv-0.0.8.tar.gz` & `tmp/calfcv-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calfcv-0.0.8.tar", last modified: Sun Jul 30 00:04:43 2023, max compression
+gzip compressed data, was "calfcv-0.1.1.tar", last modified: Mon Aug  7 01:54:33 2023, max compression
```

## Comparing `calfcv-0.0.8.tar` & `calfcv-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-07-30 00:04:43.893520 calfcv-0.0.8/
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     1495 2023-07-29 01:55:36.000000 calfcv-0.0.8/LICENSE
--rw-rw-r--   0 rolf      (1000) rolf      (1000)       25 2023-07-24 23:20:23.000000 calfcv-0.0.8/MANIFEST.in
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     4855 2023-07-30 00:04:43.893520 calfcv-0.0.8/PKG-INFO
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     4227 2023-07-30 00:04:25.000000 calfcv-0.0.8/README.rst
-drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-07-30 00:04:43.893520 calfcv-0.0.8/calfcv/
--rw-rw-r--   0 rolf      (1000) rolf      (1000)       98 2023-07-28 23:01:34.000000 calfcv-0.0.8/calfcv/__init__.py
--rw-rw-r--   0 rolf      (1000) rolf      (1000)       22 2023-07-29 01:59:39.000000 calfcv-0.0.8/calfcv/_version.py
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     8479 2023-07-29 02:15:49.000000 calfcv-0.0.8/calfcv/calfcv.py
-drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-07-30 00:04:43.893520 calfcv-0.0.8/calfcv/tests/
--rw-rw-r--   0 rolf      (1000) rolf      (1000)        0 2023-07-24 23:20:23.000000 calfcv-0.0.8/calfcv/tests/__init__.py
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     1563 2023-07-28 13:25:35.000000 calfcv-0.0.8/calfcv/tests/test_calfcv.py
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      257 2023-07-28 12:52:06.000000 calfcv-0.0.8/calfcv/tests/test_common.py
-drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-07-30 00:04:43.893520 calfcv-0.0.8/calfcv.egg-info/
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     4855 2023-07-30 00:04:43.000000 calfcv-0.0.8/calfcv.egg-info/PKG-INFO
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      380 2023-07-30 00:04:43.000000 calfcv-0.0.8/calfcv.egg-info/SOURCES.txt
--rw-rw-r--   0 rolf      (1000) rolf      (1000)        1 2023-07-30 00:04:43.000000 calfcv-0.0.8/calfcv.egg-info/dependency_links.txt
--rw-rw-r--   0 rolf      (1000) rolf      (1000)        1 2023-07-28 23:40:52.000000 calfcv-0.0.8/calfcv.egg-info/not-zip-safe
--rw-rw-r--   0 rolf      (1000) rolf      (1000)       25 2023-07-30 00:04:43.000000 calfcv-0.0.8/calfcv.egg-info/requires.txt
--rw-rw-r--   0 rolf      (1000) rolf      (1000)        7 2023-07-30 00:04:43.000000 calfcv-0.0.8/calfcv.egg-info/top_level.txt
--rw-rw-r--   0 rolf      (1000) rolf      (1000)       24 2023-07-24 23:20:23.000000 calfcv-0.0.8/requirements.txt
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      148 2023-07-30 00:04:43.893520 calfcv-0.0.8/setup.cfg
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     1929 2023-07-29 23:07:22.000000 calfcv-0.0.8/setup.py
+drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-08-07 01:54:33.965838 calfcv-0.1.1/
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     1529 2023-08-05 15:55:07.000000 calfcv-0.1.1/LICENSE
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)       25 2023-08-05 15:55:07.000000 calfcv-0.1.1/MANIFEST.in
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     3139 2023-08-07 01:54:33.965838 calfcv-0.1.1/PKG-INFO
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     2387 2023-08-06 22:40:20.000000 calfcv-0.1.1/README.rst
+drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-08-07 01:54:33.961838 calfcv-0.1.1/calfcv/
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)      124 2023-08-05 16:36:58.000000 calfcv-0.1.1/calfcv/__init__.py
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)       22 2023-08-07 01:48:49.000000 calfcv-0.1.1/calfcv/_version.py
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)    14036 2023-08-07 01:20:37.000000 calfcv-0.1.1/calfcv/calfcv.py
+drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-08-07 01:54:33.965838 calfcv-0.1.1/calfcv/tests/
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)        0 2023-08-05 15:55:07.000000 calfcv-0.1.1/calfcv/tests/__init__.py
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     1563 2023-07-28 13:25:35.000000 calfcv-0.1.1/calfcv/tests/test_calfcv.py
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)      257 2023-08-05 16:13:09.000000 calfcv-0.1.1/calfcv/tests/test_common.py
+drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-08-07 01:54:33.965838 calfcv-0.1.1/calfcv.egg-info/
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     3139 2023-08-07 01:54:33.000000 calfcv-0.1.1/calfcv.egg-info/PKG-INFO
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)      380 2023-08-07 01:54:33.000000 calfcv-0.1.1/calfcv.egg-info/SOURCES.txt
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)        1 2023-08-07 01:54:33.000000 calfcv-0.1.1/calfcv.egg-info/dependency_links.txt
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)        1 2023-08-06 22:43:48.000000 calfcv-0.1.1/calfcv.egg-info/not-zip-safe
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)      119 2023-08-07 01:54:33.000000 calfcv-0.1.1/calfcv.egg-info/requires.txt
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)        7 2023-08-07 01:54:33.000000 calfcv-0.1.1/calfcv.egg-info/top_level.txt
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)      134 2023-08-05 16:12:02.000000 calfcv-0.1.1/requirements.txt
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)      148 2023-08-07 01:54:33.965838 calfcv-0.1.1/setup.cfg
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     2533 2023-08-05 16:22:01.000000 calfcv-0.1.1/setup.py
```

### Comparing `calfcv-0.0.8/LICENSE` & `calfcv-0.1.1/LICENSE`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2023, Carlson Research, LLC
+Copyright (c) 2016, Vighnesh Birodkar and scikit-learn-contrib contributors
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.
```

### Comparing `calfcv-0.0.8/calfcv/tests/test_calfcv.py` & `calfcv-0.1.1/calfcv/tests/test_calfcv.py`

 * *Files identical despite different names*

### Comparing `calfcv-0.0.8/setup.py` & `calfcv-0.1.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,69 +1,85 @@
 #! /usr/bin/env python
-""" The calfcv package setup file.
+"""The calfcv package setup file.
 
-To build and upload a new distribution
-1.  Update the version
+Directions
 
-2. cd to calfcv and build the dist folder with
+1.  Update the code and documentation
+
+2.  Test the template by running test_template.py
+
+3.  Update the documentation, including the jupyter notebooks
+
+3.1 Convert the notebook content to rst and integrate it into quick_start.rst and user_guide.rst
+
+    jupyter nbconvert quick_start.ipynb --to markdown --output README.md
+    jupyter nbconvert quick_start.ipynb --to rst --output quick_start.rst
+    jupyter nbconvert user_guide.ipynb --to rst --output user_guide.rst
+
+3.2 Check the documentation by reading it from _build/html
+
+4.  Remove the old distribution: rm -r dist
+
+5. cd to calfcv and build the new dist folder:
 python setup.py sdist bdist_wheel
 
-3. twine upload dist/*
+Note that setup is deprecated and a replacement method is needed.
+
+6. Upload to pip: twine upload dist/*
+
 
 """
 
 import codecs
-import os
 
 from setuptools import find_packages, setup
 
-# get __version__ from _version.py
-ver_file = os.path.join('calfcv', '_version.py')
-with open(ver_file) as f:
-    exec(f.read())
+# noinspection PyProtectedMember
+from calfcv import _version
 
 DISTNAME = 'calfcv'
 DESCRIPTION = 'Coarse approximation linear function with cross validation'
 with codecs.open('README.rst', encoding='utf-8-sig') as f:
     LONG_DESCRIPTION = f.read()
 MAINTAINER = 'Carlson Research, LLC'
 MAINTAINER_EMAIL = 'hrolfrc@gmail.com'
-URL = ''
+URL = 'https://github.com/hrolfrc/calfcv'
 LICENSE = 'new BSD'
-DOWNLOAD_URL = 'https://github.com/scikit-learn-contrib/project-template'
-VERSION = '0.0.8'
+DOWNLOAD_URL = 'https://github.com/hrolfrc/calfcv'
+VERSION = _version.__version__
 INSTALL_REQUIRES = ['numpy', 'scipy', 'scikit-learn']
 CLASSIFIERS = ['Intended Audience :: Science/Research',
                'Intended Audience :: Developers',
+               'Topic :: Scientific/Engineering :: Artificial Intelligence',
                'Development Status :: 2 - Pre-Alpha',
                'License :: OSI Approved',
                'Topic :: Scientific/Engineering',
                'Operating System :: OS Independent',
                'Programming Language :: Python :: 3']
 
-# EXTRAS_REQUIRE = {
-#     'tests': [
-#         'pytest',
-#         'pytest-cov'],
-#     'docs': [
-#         'sphinx',
-#         'sphinx-gallery',
-#         'sphinx_rtd_theme',
-#         'numpydoc',
-#         'matplotlib'
-#     ]
-# }
+EXTRAS_REQUIRE = {
+    'tests': [
+        'pytest',
+        'pytest-cov'],
+    'docs': [
+        'sphinx',
+        'sphinx-gallery',
+        'sphinx_rtd_theme',
+        'numpydoc',
+        'matplotlib'
+    ]
+}
 
 setup(name=DISTNAME,
       maintainer=MAINTAINER,
       maintainer_email=MAINTAINER_EMAIL,
       description=DESCRIPTION,
       license=LICENSE,
       url=URL,
       version=VERSION,
       download_url=DOWNLOAD_URL,
       long_description=LONG_DESCRIPTION,
       zip_safe=False,  # the package can run out of an .egg file
       classifiers=CLASSIFIERS,
       packages=find_packages(),
-      install_requires=INSTALL_REQUIRES)  # ,
-# extras_require=EXTRAS_REQUIRE)
+      install_requires=INSTALL_REQUIRES,
+      extras_require=EXTRAS_REQUIRE)
```

