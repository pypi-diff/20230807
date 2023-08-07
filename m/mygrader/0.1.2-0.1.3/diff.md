# Comparing `tmp/mygrader-0.1.2.tar.gz` & `tmp/mygrader-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mygrader-0.1.2.tar", last modified: Sun Aug  6 21:36:30 2023, max compression
+gzip compressed data, was "mygrader-0.1.3.tar", last modified: Mon Aug  7 05:23:53 2023, max compression
```

## Comparing `mygrader-0.1.2.tar` & `mygrader-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 iccie      (501) staff       (20)        0 2023-08-06 21:36:30.274449 mygrader-0.1.2/
--rw-r--r--   0 iccie      (501) staff       (20)     1066 2023-08-06 20:37:53.000000 mygrader-0.1.2/LICENSE
--rw-r--r--   0 iccie      (501) staff       (20)      572 2023-08-06 21:36:30.274334 mygrader-0.1.2/PKG-INFO
--rw-r--r--   0 iccie      (501) staff       (20)     2191 2023-08-06 20:41:41.000000 mygrader-0.1.2/README.md
-drwxr-xr-x   0 iccie      (501) staff       (20)        0 2023-08-06 21:36:30.274173 mygrader-0.1.2/mygrader.egg-info/
--rw-r--r--   0 iccie      (501) staff       (20)      572 2023-08-06 21:36:30.000000 mygrader-0.1.2/mygrader.egg-info/PKG-INFO
--rw-r--r--   0 iccie      (501) staff       (20)      220 2023-08-06 21:36:30.000000 mygrader-0.1.2/mygrader.egg-info/SOURCES.txt
--rw-r--r--   0 iccie      (501) staff       (20)        1 2023-08-06 21:36:30.000000 mygrader-0.1.2/mygrader.egg-info/dependency_links.txt
--rw-r--r--   0 iccie      (501) staff       (20)       50 2023-08-06 21:36:30.000000 mygrader-0.1.2/mygrader.egg-info/entry_points.txt
--rw-r--r--   0 iccie      (501) staff       (20)       35 2023-08-06 21:36:30.000000 mygrader-0.1.2/mygrader.egg-info/requires.txt
--rw-r--r--   0 iccie      (501) staff       (20)        1 2023-08-06 21:36:30.000000 mygrader-0.1.2/mygrader.egg-info/top_level.txt
--rw-r--r--   0 iccie      (501) staff       (20)       38 2023-08-06 21:36:30.274492 mygrader-0.1.2/setup.cfg
--rw-r--r--   0 iccie      (501) staff       (20)      946 2023-08-06 21:36:06.000000 mygrader-0.1.2/setup.py
+drwxr-xr-x   0 iccie      (501) staff       (20)        0 2023-08-07 05:23:53.286003 mygrader-0.1.3/
+-rw-r--r--   0 iccie      (501) staff       (20)     1066 2023-08-06 20:37:53.000000 mygrader-0.1.3/LICENSE
+-rw-r--r--   0 iccie      (501) staff       (20)      470 2023-08-07 05:23:53.285888 mygrader-0.1.3/PKG-INFO
+-rw-r--r--   0 iccie      (501) staff       (20)     2191 2023-08-06 20:41:41.000000 mygrader-0.1.3/README.md
+drwxr-xr-x   0 iccie      (501) staff       (20)        0 2023-08-07 05:23:53.285718 mygrader-0.1.3/mygrader.egg-info/
+-rw-r--r--   0 iccie      (501) staff       (20)      470 2023-08-07 05:23:53.000000 mygrader-0.1.3/mygrader.egg-info/PKG-INFO
+-rw-r--r--   0 iccie      (501) staff       (20)      220 2023-08-07 05:23:53.000000 mygrader-0.1.3/mygrader.egg-info/SOURCES.txt
+-rw-r--r--   0 iccie      (501) staff       (20)        1 2023-08-07 05:23:53.000000 mygrader-0.1.3/mygrader.egg-info/dependency_links.txt
+-rw-r--r--   0 iccie      (501) staff       (20)       50 2023-08-07 05:23:53.000000 mygrader-0.1.3/mygrader.egg-info/entry_points.txt
+-rw-r--r--   0 iccie      (501) staff       (20)       35 2023-08-07 05:23:53.000000 mygrader-0.1.3/mygrader.egg-info/requires.txt
+-rw-r--r--   0 iccie      (501) staff       (20)        1 2023-08-07 05:23:53.000000 mygrader-0.1.3/mygrader.egg-info/top_level.txt
+-rw-r--r--   0 iccie      (501) staff       (20)       38 2023-08-07 05:23:53.286043 mygrader-0.1.3/setup.cfg
+-rw-r--r--   0 iccie      (501) staff       (20)      846 2023-08-07 05:23:51.000000 mygrader-0.1.3/setup.py
```

### Comparing `mygrader-0.1.2/LICENSE` & `mygrader-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mygrader-0.1.2/README.md` & `mygrader-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `mygrader-0.1.2/setup.py` & `mygrader-0.1.3/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mygrader',
-    version='0.1.2',
+    version='0.1.3',
     packages=find_packages(),
     install_requires=[],  # Add any required dependencies here
     author='AppleBoiy',
     author_email='contact.chaipat@gmail.com',
     description='my own CS111 grader.',
 
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
     ],
     entry_points={
         'console_scripts': [
             'your_script=your_package:main',
         ],
     },
     extras_require={
```

