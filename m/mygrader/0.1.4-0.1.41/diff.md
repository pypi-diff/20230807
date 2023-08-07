# Comparing `tmp/mygrader-0.1.4.tar.gz` & `tmp/mygrader-0.1.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mygrader-0.1.4.tar", last modified: Mon Aug  7 05:27:46 2023, max compression
+gzip compressed data, was "mygrader-0.1.41.tar", last modified: Mon Aug  7 05:36:25 2023, max compression
```

## Comparing `mygrader-0.1.4.tar` & `mygrader-0.1.41.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 iccie      (501) staff       (20)        0 2023-08-07 05:27:46.573909 mygrader-0.1.4/
--rw-r--r--   0 iccie      (501) staff       (20)     1066 2023-08-06 20:37:53.000000 mygrader-0.1.4/LICENSE
--rw-r--r--   0 iccie      (501) staff       (20)      470 2023-08-07 05:27:46.573780 mygrader-0.1.4/PKG-INFO
--rw-r--r--   0 iccie      (501) staff       (20)     2191 2023-08-06 20:41:41.000000 mygrader-0.1.4/README.md
-drwxr-xr-x   0 iccie      (501) staff       (20)        0 2023-08-07 05:27:46.573611 mygrader-0.1.4/mygrader.egg-info/
--rw-r--r--   0 iccie      (501) staff       (20)      470 2023-08-07 05:27:46.000000 mygrader-0.1.4/mygrader.egg-info/PKG-INFO
--rw-r--r--   0 iccie      (501) staff       (20)      220 2023-08-07 05:27:46.000000 mygrader-0.1.4/mygrader.egg-info/SOURCES.txt
--rw-r--r--   0 iccie      (501) staff       (20)        1 2023-08-07 05:27:46.000000 mygrader-0.1.4/mygrader.egg-info/dependency_links.txt
--rw-r--r--   0 iccie      (501) staff       (20)       50 2023-08-07 05:27:46.000000 mygrader-0.1.4/mygrader.egg-info/entry_points.txt
--rw-r--r--   0 iccie      (501) staff       (20)       35 2023-08-07 05:27:46.000000 mygrader-0.1.4/mygrader.egg-info/requires.txt
--rw-r--r--   0 iccie      (501) staff       (20)        1 2023-08-07 05:27:46.000000 mygrader-0.1.4/mygrader.egg-info/top_level.txt
--rw-r--r--   0 iccie      (501) staff       (20)       38 2023-08-07 05:27:46.573949 mygrader-0.1.4/setup.cfg
--rw-r--r--   0 iccie      (501) staff       (20)     1013 2023-08-07 05:27:43.000000 mygrader-0.1.4/setup.py
+drwxr-xr-x   0 iccie      (501) staff       (20)        0 2023-08-07 05:36:25.214318 mygrader-0.1.41/
+-rw-r--r--   0 iccie      (501) staff       (20)     1066 2023-08-06 20:37:53.000000 mygrader-0.1.41/LICENSE
+-rw-r--r--   0 iccie      (501) staff       (20)     2754 2023-08-07 05:36:25.214200 mygrader-0.1.41/PKG-INFO
+-rw-r--r--   0 iccie      (501) staff       (20)     2191 2023-08-06 20:41:41.000000 mygrader-0.1.41/README.md
+drwxr-xr-x   0 iccie      (501) staff       (20)        0 2023-08-07 05:36:25.214035 mygrader-0.1.41/mygrader.egg-info/
+-rw-r--r--   0 iccie      (501) staff       (20)     2754 2023-08-07 05:36:25.000000 mygrader-0.1.41/mygrader.egg-info/PKG-INFO
+-rw-r--r--   0 iccie      (501) staff       (20)      220 2023-08-07 05:36:25.000000 mygrader-0.1.41/mygrader.egg-info/SOURCES.txt
+-rw-r--r--   0 iccie      (501) staff       (20)        1 2023-08-07 05:36:25.000000 mygrader-0.1.41/mygrader.egg-info/dependency_links.txt
+-rw-r--r--   0 iccie      (501) staff       (20)       50 2023-08-07 05:36:25.000000 mygrader-0.1.41/mygrader.egg-info/entry_points.txt
+-rw-r--r--   0 iccie      (501) staff       (20)       35 2023-08-07 05:36:25.000000 mygrader-0.1.41/mygrader.egg-info/requires.txt
+-rw-r--r--   0 iccie      (501) staff       (20)        1 2023-08-07 05:36:25.000000 mygrader-0.1.41/mygrader.egg-info/top_level.txt
+-rw-r--r--   0 iccie      (501) staff       (20)       38 2023-08-07 05:36:25.214357 mygrader-0.1.41/setup.cfg
+-rw-r--r--   0 iccie      (501) staff       (20)     1156 2023-08-07 05:36:23.000000 mygrader-0.1.41/setup.py
```

### Comparing `mygrader-0.1.4/LICENSE` & `mygrader-0.1.41/LICENSE`

 * *Files identical despite different names*

### Comparing `mygrader-0.1.4/README.md` & `mygrader-0.1.41/README.md`

 * *Files identical despite different names*

### Comparing `mygrader-0.1.4/setup.py` & `mygrader-0.1.41/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,20 +3,25 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='mygrader',
-    version='0.1.4',
+    version='0.1.41',
     packages=find_packages(),
     install_requires=[],  # Add any required dependencies here
     author='AppleBoiy',
+
     author_email='contact.chaipat@gmail.com',
     description='my own CS111 grader.',
+    long_description=long_description,
+    long_description_content_type='text/markdown',
+
+    url="https://github.com/AppleBoiy/my-grader",
 
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
```

