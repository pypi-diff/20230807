# Comparing `tmp/mygrader-0.1.5.tar.gz` & `tmp/mygrader-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mygrader-0.1.5.tar", last modified: Mon Aug  7 17:14:50 2023, max compression
+gzip compressed data, was "mygrader-0.2.0.tar", last modified: Mon Aug  7 17:17:48 2023, max compression
```

## Comparing `mygrader-0.1.5.tar` & `mygrader-0.2.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 iccie      (501) staff       (20)        0 2023-08-07 17:14:50.504965 mygrader-0.1.5/
--rw-r--r--   0 iccie      (501) staff       (20)     1066 2023-08-06 20:37:53.000000 mygrader-0.1.5/LICENSE
--rw-r--r--   0 iccie      (501) staff       (20)     2753 2023-08-07 17:14:50.504851 mygrader-0.1.5/PKG-INFO
--rw-r--r--   0 iccie      (501) staff       (20)     2191 2023-08-06 20:41:41.000000 mygrader-0.1.5/README.md
-drwxr-xr-x   0 iccie      (501) staff       (20)        0 2023-08-07 17:14:50.500693 mygrader-0.1.5/mygrader.egg-info/
--rw-r--r--   0 iccie      (501) staff       (20)     2753 2023-08-07 17:14:50.000000 mygrader-0.1.5/mygrader.egg-info/PKG-INFO
--rw-r--r--   0 iccie      (501) staff       (20)      889 2023-08-07 17:14:50.000000 mygrader-0.1.5/mygrader.egg-info/SOURCES.txt
--rw-r--r--   0 iccie      (501) staff       (20)        1 2023-08-07 17:14:50.000000 mygrader-0.1.5/mygrader.egg-info/dependency_links.txt
--rw-r--r--   0 iccie      (501) staff       (20)       50 2023-08-07 17:14:50.000000 mygrader-0.1.5/mygrader.egg-info/entry_points.txt
--rw-r--r--   0 iccie      (501) staff       (20)       35 2023-08-07 17:14:50.000000 mygrader-0.1.5/mygrader.egg-info/requires.txt
--rw-r--r--   0 iccie      (501) staff       (20)        4 2023-08-07 17:14:50.000000 mygrader-0.1.5/mygrader.egg-info/top_level.txt
--rw-r--r--   0 iccie      (501) staff       (20)       38 2023-08-07 17:14:50.505002 mygrader-0.1.5/setup.cfg
--rw-r--r--   0 iccie      (501) staff       (20)     1155 2023-08-07 17:13:30.000000 mygrader-0.1.5/setup.py
-drwxr-xr-x   0 iccie      (501) staff       (20)        0 2023-08-07 17:14:50.500825 mygrader-0.1.5/src/
--rw-r--r--   0 iccie      (501) staff       (20)        0 2023-08-07 05:56:28.000000 mygrader-0.1.5/src/__init__.py
-drwxr-xr-x   0 iccie      (501) staff       (20)        0 2023-08-07 17:14:50.501555 mygrader-0.1.5/src/mygrader/
--rw-r--r--   0 iccie      (501) staff       (20)       87 2023-08-07 05:56:21.000000 mygrader-0.1.5/src/mygrader/__init__.py
-drwxr-xr-x   0 iccie      (501) staff       (20)        0 2023-08-07 17:14:50.501809 mygrader-0.1.5/src/mygrader/cs111/
-drwxr-xr-x   0 iccie      (501) staff       (20)        0 2023-08-07 17:14:50.504647 mygrader-0.1.5/src/mygrader/cs111/CS66/
--rw-r--r--   0 iccie      (501) staff       (20)      565 2023-08-07 17:12:38.000000 mygrader-0.1.5/src/mygrader/cs111/CS66/__init__.py
--rw-r--r--   0 iccie      (501) staff       (20)     2294 2023-08-07 16:59:35.000000 mygrader-0.1.5/src/mygrader/cs111/CS66/base_b.py
--rw-r--r--   0 iccie      (501) staff       (20)      832 2023-08-07 16:59:35.000000 mygrader-0.1.5/src/mygrader/cs111/CS66/corner_frame.py
--rw-r--r--   0 iccie      (501) staff       (20)     1609 2023-08-07 16:59:35.000000 mygrader-0.1.5/src/mygrader/cs111/CS66/dest_rotate_list.py
--rw-r--r--   0 iccie      (501) staff       (20)     1985 2023-08-07 16:59:35.000000 mygrader-0.1.5/src/mygrader/cs111/CS66/medal_allocation.py
--rw-r--r--   0 iccie      (501) staff       (20)     1848 2023-08-07 16:59:35.000000 mygrader-0.1.5/src/mygrader/cs111/CS66/moving_average.py
--rw-r--r--   0 iccie      (501) staff       (20)     4375 2023-08-07 16:59:35.000000 mygrader-0.1.5/src/mygrader/cs111/CS66/num_to_word.py
--rw-r--r--   0 iccie      (501) staff       (20)     1551 2023-08-07 16:59:35.000000 mygrader-0.1.5/src/mygrader/cs111/CS66/pi.py
--rw-r--r--   0 iccie      (501) staff       (20)     1575 2023-08-07 16:59:35.000000 mygrader-0.1.5/src/mygrader/cs111/CS66/print_polynomial.py
--rw-r--r--   0 iccie      (501) staff       (20)     1371 2023-08-07 16:59:35.000000 mygrader-0.1.5/src/mygrader/cs111/CS66/recursion_gcd.py
--rw-r--r--   0 iccie      (501) staff       (20)     1293 2023-08-07 16:59:35.000000 mygrader-0.1.5/src/mygrader/cs111/CS66/reverse_digits.py
--rw-r--r--   0 iccie      (501) staff       (20)     1853 2023-08-07 17:00:24.000000 mygrader-0.1.5/src/mygrader/cs111/CS66/substitute_once.py
--rw-r--r--   0 iccie      (501) staff       (20)      623 2023-08-07 17:00:24.000000 mygrader-0.1.5/src/mygrader/cs111/CS66/triangle.py
--rw-r--r--   0 iccie      (501) staff       (20)      722 2023-08-07 17:00:24.000000 mygrader-0.1.5/src/mygrader/cs111/CS66/uniform.py
--rw-r--r--   0 iccie      (501) staff       (20)        0 2023-08-07 16:52:13.000000 mygrader-0.1.5/src/mygrader/cs111/__init__.py
--rw-r--r--   0 iccie      (501) staff       (20)     1493 2023-08-07 05:22:22.000000 mygrader-0.1.5/src/mygrader/printer.py
--rw-r--r--   0 iccie      (501) staff       (20)      560 2023-08-06 20:09:42.000000 mygrader-0.1.5/src/mygrader/writer.py
+drwxr-xr-x   0 iccie      (501) staff       (20)        0 2023-08-07 17:17:48.621251 mygrader-0.2.0/
+-rw-r--r--   0 iccie      (501) staff       (20)     1066 2023-08-06 20:37:53.000000 mygrader-0.2.0/LICENSE
+-rw-r--r--   0 iccie      (501) staff       (20)     2753 2023-08-07 17:17:48.621074 mygrader-0.2.0/PKG-INFO
+-rw-r--r--   0 iccie      (501) staff       (20)     2191 2023-08-06 20:41:41.000000 mygrader-0.2.0/README.md
+drwxr-xr-x   0 iccie      (501) staff       (20)        0 2023-08-07 17:17:48.614435 mygrader-0.2.0/mygrader.egg-info/
+-rw-r--r--   0 iccie      (501) staff       (20)     2753 2023-08-07 17:17:48.000000 mygrader-0.2.0/mygrader.egg-info/PKG-INFO
+-rw-r--r--   0 iccie      (501) staff       (20)      889 2023-08-07 17:17:48.000000 mygrader-0.2.0/mygrader.egg-info/SOURCES.txt
+-rw-r--r--   0 iccie      (501) staff       (20)        1 2023-08-07 17:17:48.000000 mygrader-0.2.0/mygrader.egg-info/dependency_links.txt
+-rw-r--r--   0 iccie      (501) staff       (20)       50 2023-08-07 17:17:48.000000 mygrader-0.2.0/mygrader.egg-info/entry_points.txt
+-rw-r--r--   0 iccie      (501) staff       (20)       35 2023-08-07 17:17:48.000000 mygrader-0.2.0/mygrader.egg-info/requires.txt
+-rw-r--r--   0 iccie      (501) staff       (20)        4 2023-08-07 17:17:48.000000 mygrader-0.2.0/mygrader.egg-info/top_level.txt
+-rw-r--r--   0 iccie      (501) staff       (20)       38 2023-08-07 17:17:48.621906 mygrader-0.2.0/setup.cfg
+-rw-r--r--   0 iccie      (501) staff       (20)     1155 2023-08-07 17:17:44.000000 mygrader-0.2.0/setup.py
+drwxr-xr-x   0 iccie      (501) staff       (20)        0 2023-08-07 17:17:48.614558 mygrader-0.2.0/src/
+-rw-r--r--   0 iccie      (501) staff       (20)        0 2023-08-07 05:56:28.000000 mygrader-0.2.0/src/__init__.py
+drwxr-xr-x   0 iccie      (501) staff       (20)        0 2023-08-07 17:17:48.615254 mygrader-0.2.0/src/mygrader/
+-rw-r--r--   0 iccie      (501) staff       (20)       87 2023-08-07 05:56:21.000000 mygrader-0.2.0/src/mygrader/__init__.py
+drwxr-xr-x   0 iccie      (501) staff       (20)        0 2023-08-07 17:17:48.616090 mygrader-0.2.0/src/mygrader/cs111/
+drwxr-xr-x   0 iccie      (501) staff       (20)        0 2023-08-07 17:17:48.619915 mygrader-0.2.0/src/mygrader/cs111/CS66/
+-rw-r--r--   0 iccie      (501) staff       (20)      565 2023-08-07 17:12:38.000000 mygrader-0.2.0/src/mygrader/cs111/CS66/__init__.py
+-rw-r--r--   0 iccie      (501) staff       (20)     2294 2023-08-07 16:59:35.000000 mygrader-0.2.0/src/mygrader/cs111/CS66/base_b.py
+-rw-r--r--   0 iccie      (501) staff       (20)      832 2023-08-07 16:59:35.000000 mygrader-0.2.0/src/mygrader/cs111/CS66/corner_frame.py
+-rw-r--r--   0 iccie      (501) staff       (20)     1609 2023-08-07 16:59:35.000000 mygrader-0.2.0/src/mygrader/cs111/CS66/dest_rotate_list.py
+-rw-r--r--   0 iccie      (501) staff       (20)     1985 2023-08-07 16:59:35.000000 mygrader-0.2.0/src/mygrader/cs111/CS66/medal_allocation.py
+-rw-r--r--   0 iccie      (501) staff       (20)     1848 2023-08-07 16:59:35.000000 mygrader-0.2.0/src/mygrader/cs111/CS66/moving_average.py
+-rw-r--r--   0 iccie      (501) staff       (20)     4375 2023-08-07 16:59:35.000000 mygrader-0.2.0/src/mygrader/cs111/CS66/num_to_word.py
+-rw-r--r--   0 iccie      (501) staff       (20)     1551 2023-08-07 16:59:35.000000 mygrader-0.2.0/src/mygrader/cs111/CS66/pi.py
+-rw-r--r--   0 iccie      (501) staff       (20)     1575 2023-08-07 16:59:35.000000 mygrader-0.2.0/src/mygrader/cs111/CS66/print_polynomial.py
+-rw-r--r--   0 iccie      (501) staff       (20)     1371 2023-08-07 16:59:35.000000 mygrader-0.2.0/src/mygrader/cs111/CS66/recursion_gcd.py
+-rw-r--r--   0 iccie      (501) staff       (20)     1293 2023-08-07 16:59:35.000000 mygrader-0.2.0/src/mygrader/cs111/CS66/reverse_digits.py
+-rw-r--r--   0 iccie      (501) staff       (20)     1853 2023-08-07 17:00:24.000000 mygrader-0.2.0/src/mygrader/cs111/CS66/substitute_once.py
+-rw-r--r--   0 iccie      (501) staff       (20)      623 2023-08-07 17:00:24.000000 mygrader-0.2.0/src/mygrader/cs111/CS66/triangle.py
+-rw-r--r--   0 iccie      (501) staff       (20)      722 2023-08-07 17:00:24.000000 mygrader-0.2.0/src/mygrader/cs111/CS66/uniform.py
+-rw-r--r--   0 iccie      (501) staff       (20)        0 2023-08-07 16:52:13.000000 mygrader-0.2.0/src/mygrader/cs111/__init__.py
+-rw-r--r--   0 iccie      (501) staff       (20)     1493 2023-08-07 05:22:22.000000 mygrader-0.2.0/src/mygrader/printer.py
+-rw-r--r--   0 iccie      (501) staff       (20)      560 2023-08-06 20:09:42.000000 mygrader-0.2.0/src/mygrader/writer.py
```

### Comparing `mygrader-0.1.5/LICENSE` & `mygrader-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mygrader-0.1.5/PKG-INFO` & `mygrader-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mygrader
-Version: 0.1.5
+Version: 0.2.0
 Summary: my own CS111 grader.
 Home-page: https://github.com/AppleBoiy/my-grader
 Author: AppleBoiy
 Author-email: contact.chaipat@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mygrader-0.1.5/README.md` & `mygrader-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `mygrader-0.1.5/mygrader.egg-info/PKG-INFO` & `mygrader-0.2.0/mygrader.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mygrader
-Version: 0.1.5
+Version: 0.2.0
 Summary: my own CS111 grader.
 Home-page: https://github.com/AppleBoiy/my-grader
 Author: AppleBoiy
 Author-email: contact.chaipat@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mygrader-0.1.5/mygrader.egg-info/SOURCES.txt` & `mygrader-0.2.0/mygrader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mygrader-0.1.5/setup.py` & `mygrader-0.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='mygrader',
-    version='0.1.5',
+    version='0.2.0',
     packages=find_packages(),
     install_requires=[],  # Add any required dependencies here
     author='AppleBoiy',
 
     author_email='contact.chaipat@gmail.com',
     description='my own CS111 grader.',
     long_description=long_description,
```

### Comparing `mygrader-0.1.5/src/mygrader/cs111/CS66/__init__.py` & `mygrader-0.2.0/src/mygrader/cs111/CS66/__init__.py`

 * *Files identical despite different names*

### Comparing `mygrader-0.1.5/src/mygrader/cs111/CS66/base_b.py` & `mygrader-0.2.0/src/mygrader/cs111/CS66/base_b.py`

 * *Files identical despite different names*

### Comparing `mygrader-0.1.5/src/mygrader/cs111/CS66/corner_frame.py` & `mygrader-0.2.0/src/mygrader/cs111/CS66/corner_frame.py`

 * *Files identical despite different names*

### Comparing `mygrader-0.1.5/src/mygrader/cs111/CS66/dest_rotate_list.py` & `mygrader-0.2.0/src/mygrader/cs111/CS66/dest_rotate_list.py`

 * *Files identical despite different names*

### Comparing `mygrader-0.1.5/src/mygrader/cs111/CS66/medal_allocation.py` & `mygrader-0.2.0/src/mygrader/cs111/CS66/medal_allocation.py`

 * *Files identical despite different names*

### Comparing `mygrader-0.1.5/src/mygrader/cs111/CS66/moving_average.py` & `mygrader-0.2.0/src/mygrader/cs111/CS66/moving_average.py`

 * *Files identical despite different names*

### Comparing `mygrader-0.1.5/src/mygrader/cs111/CS66/num_to_word.py` & `mygrader-0.2.0/src/mygrader/cs111/CS66/num_to_word.py`

 * *Files identical despite different names*

### Comparing `mygrader-0.1.5/src/mygrader/cs111/CS66/pi.py` & `mygrader-0.2.0/src/mygrader/cs111/CS66/pi.py`

 * *Files identical despite different names*

### Comparing `mygrader-0.1.5/src/mygrader/cs111/CS66/print_polynomial.py` & `mygrader-0.2.0/src/mygrader/cs111/CS66/print_polynomial.py`

 * *Files identical despite different names*

### Comparing `mygrader-0.1.5/src/mygrader/cs111/CS66/recursion_gcd.py` & `mygrader-0.2.0/src/mygrader/cs111/CS66/recursion_gcd.py`

 * *Files identical despite different names*

### Comparing `mygrader-0.1.5/src/mygrader/cs111/CS66/reverse_digits.py` & `mygrader-0.2.0/src/mygrader/cs111/CS66/reverse_digits.py`

 * *Files identical despite different names*

### Comparing `mygrader-0.1.5/src/mygrader/cs111/CS66/substitute_once.py` & `mygrader-0.2.0/src/mygrader/cs111/CS66/substitute_once.py`

 * *Files identical despite different names*

### Comparing `mygrader-0.1.5/src/mygrader/cs111/CS66/triangle.py` & `mygrader-0.2.0/src/mygrader/cs111/CS66/triangle.py`

 * *Files identical despite different names*

### Comparing `mygrader-0.1.5/src/mygrader/cs111/CS66/uniform.py` & `mygrader-0.2.0/src/mygrader/cs111/CS66/uniform.py`

 * *Files identical despite different names*

### Comparing `mygrader-0.1.5/src/mygrader/printer.py` & `mygrader-0.2.0/src/mygrader/printer.py`

 * *Files identical despite different names*

### Comparing `mygrader-0.1.5/src/mygrader/writer.py` & `mygrader-0.2.0/src/mygrader/writer.py`

 * *Files identical despite different names*

