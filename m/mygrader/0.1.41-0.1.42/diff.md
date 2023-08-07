# Comparing `tmp/mygrader-0.1.41.tar.gz` & `tmp/mygrader-0.1.42.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mygrader-0.1.41.tar", last modified: Mon Aug  7 05:36:25 2023, max compression
+gzip compressed data, was "mygrader-0.1.42.tar", last modified: Mon Aug  7 05:46:50 2023, max compression
```

## Comparing `mygrader-0.1.41.tar` & `mygrader-0.1.42.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 iccie      (501) staff       (20)        0 2023-08-07 05:36:25.214318 mygrader-0.1.41/
--rw-r--r--   0 iccie      (501) staff       (20)     1066 2023-08-06 20:37:53.000000 mygrader-0.1.41/LICENSE
--rw-r--r--   0 iccie      (501) staff       (20)     2754 2023-08-07 05:36:25.214200 mygrader-0.1.41/PKG-INFO
--rw-r--r--   0 iccie      (501) staff       (20)     2191 2023-08-06 20:41:41.000000 mygrader-0.1.41/README.md
-drwxr-xr-x   0 iccie      (501) staff       (20)        0 2023-08-07 05:36:25.214035 mygrader-0.1.41/mygrader.egg-info/
--rw-r--r--   0 iccie      (501) staff       (20)     2754 2023-08-07 05:36:25.000000 mygrader-0.1.41/mygrader.egg-info/PKG-INFO
--rw-r--r--   0 iccie      (501) staff       (20)      220 2023-08-07 05:36:25.000000 mygrader-0.1.41/mygrader.egg-info/SOURCES.txt
--rw-r--r--   0 iccie      (501) staff       (20)        1 2023-08-07 05:36:25.000000 mygrader-0.1.41/mygrader.egg-info/dependency_links.txt
--rw-r--r--   0 iccie      (501) staff       (20)       50 2023-08-07 05:36:25.000000 mygrader-0.1.41/mygrader.egg-info/entry_points.txt
--rw-r--r--   0 iccie      (501) staff       (20)       35 2023-08-07 05:36:25.000000 mygrader-0.1.41/mygrader.egg-info/requires.txt
--rw-r--r--   0 iccie      (501) staff       (20)        1 2023-08-07 05:36:25.000000 mygrader-0.1.41/mygrader.egg-info/top_level.txt
--rw-r--r--   0 iccie      (501) staff       (20)       38 2023-08-07 05:36:25.214357 mygrader-0.1.41/setup.cfg
--rw-r--r--   0 iccie      (501) staff       (20)     1156 2023-08-07 05:36:23.000000 mygrader-0.1.41/setup.py
+drwxr-xr-x   0 iccie      (501) staff       (20)        0 2023-08-07 05:46:50.276808 mygrader-0.1.42/
+-rw-r--r--   0 iccie      (501) staff       (20)     1066 2023-08-06 20:37:53.000000 mygrader-0.1.42/LICENSE
+-rw-r--r--   0 iccie      (501) staff       (20)     2754 2023-08-07 05:46:50.276672 mygrader-0.1.42/PKG-INFO
+-rw-r--r--   0 iccie      (501) staff       (20)     2191 2023-08-06 20:41:41.000000 mygrader-0.1.42/README.md
+drwxr-xr-x   0 iccie      (501) staff       (20)        0 2023-08-07 05:46:50.276384 mygrader-0.1.42/mygrader.egg-info/
+-rw-r--r--   0 iccie      (501) staff       (20)     2754 2023-08-07 05:46:50.000000 mygrader-0.1.42/mygrader.egg-info/PKG-INFO
+-rw-r--r--   0 iccie      (501) staff       (20)      220 2023-08-07 05:46:50.000000 mygrader-0.1.42/mygrader.egg-info/SOURCES.txt
+-rw-r--r--   0 iccie      (501) staff       (20)        1 2023-08-07 05:46:50.000000 mygrader-0.1.42/mygrader.egg-info/dependency_links.txt
+-rw-r--r--   0 iccie      (501) staff       (20)       50 2023-08-07 05:46:50.000000 mygrader-0.1.42/mygrader.egg-info/entry_points.txt
+-rw-r--r--   0 iccie      (501) staff       (20)       35 2023-08-07 05:46:50.000000 mygrader-0.1.42/mygrader.egg-info/requires.txt
+-rw-r--r--   0 iccie      (501) staff       (20)        1 2023-08-07 05:46:50.000000 mygrader-0.1.42/mygrader.egg-info/top_level.txt
+-rw-r--r--   0 iccie      (501) staff       (20)       38 2023-08-07 05:46:50.276864 mygrader-0.1.42/setup.cfg
+-rw-r--r--   0 iccie      (501) staff       (20)     1156 2023-08-07 05:46:49.000000 mygrader-0.1.42/setup.py
```

### Comparing `mygrader-0.1.41/LICENSE` & `mygrader-0.1.42/LICENSE`

 * *Files identical despite different names*

### Comparing `mygrader-0.1.41/PKG-INFO` & `mygrader-0.1.42/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mygrader
-Version: 0.1.41
+Version: 0.1.42
 Summary: my own CS111 grader.
 Home-page: https://github.com/AppleBoiy/my-grader
 Author: AppleBoiy
 Author-email: contact.chaipat@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mygrader-0.1.41/README.md` & `mygrader-0.1.42/README.md`

 * *Files identical despite different names*

### Comparing `mygrader-0.1.41/mygrader.egg-info/PKG-INFO` & `mygrader-0.1.42/mygrader.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mygrader
-Version: 0.1.41
+Version: 0.1.42
 Summary: my own CS111 grader.
 Home-page: https://github.com/AppleBoiy/my-grader
 Author: AppleBoiy
 Author-email: contact.chaipat@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mygrader-0.1.41/setup.py` & `mygrader-0.1.42/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='mygrader',
-    version='0.1.41',
+    version='0.1.42',
     packages=find_packages(),
     install_requires=[],  # Add any required dependencies here
     author='AppleBoiy',
 
     author_email='contact.chaipat@gmail.com',
     description='my own CS111 grader.',
     long_description=long_description,
```

