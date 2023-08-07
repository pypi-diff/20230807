# Comparing `tmp/jianglab-0.7.6.tar.gz` & `tmp/jianglab-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jianglab-0.7.6.tar", last modified: Thu Aug  3 15:22:17 2023, max compression
+gzip compressed data, was "jianglab-0.7.7.tar", last modified: Mon Aug  7 16:07:02 2023, max compression
```

## Comparing `jianglab-0.7.6.tar` & `jianglab-0.7.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-08-03 15:22:17.909529 jianglab-0.7.6/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-08-03 15:22:17.909189 jianglab-0.7.6/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)     1176 2023-07-12 19:29:04.000000 jianglab-0.7.6/README.md
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-08-03 15:22:17.904919 jianglab-0.7.6/jianglab/
--rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:41:31.000000 jianglab-0.7.6/jianglab/__init__.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)    49415 2023-08-03 15:22:05.000000 jianglab-0.7.6/jianglab/common_functions.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:41:33.000000 jianglab-0.7.6/jianglab/params.py
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-08-03 15:22:17.908453 jianglab-0.7.6/jianglab.egg-info/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-08-03 15:22:17.000000 jianglab-0.7.6/jianglab.egg-info/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-08-03 15:22:17.000000 jianglab-0.7.6/jianglab.egg-info/SOURCES.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-08-03 15:22:17.000000 jianglab-0.7.6/jianglab.egg-info/dependency_links.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)      168 2023-08-03 15:22:17.000000 jianglab-0.7.6/jianglab.egg-info/requires.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-08-03 15:22:17.000000 jianglab-0.7.6/jianglab.egg-info/top_level.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-08-03 15:22:17.909670 jianglab-0.7.6/setup.cfg
--rw-r--r--   0 zhengjiang   (501) staff       (20)     1162 2023-08-03 15:22:12.000000 jianglab-0.7.6/setup.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-08-07 16:07:02.654705 jianglab-0.7.7/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-08-07 16:07:02.654346 jianglab-0.7.7/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)     1176 2023-07-12 19:29:04.000000 jianglab-0.7.7/README.md
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-08-07 16:07:02.650747 jianglab-0.7.7/jianglab/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:41:31.000000 jianglab-0.7.7/jianglab/__init__.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)    50240 2023-08-07 16:06:53.000000 jianglab-0.7.7/jianglab/common_functions.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:41:33.000000 jianglab-0.7.7/jianglab/params.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-08-07 16:07:02.653832 jianglab-0.7.7/jianglab.egg-info/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-08-07 16:07:02.000000 jianglab-0.7.7/jianglab.egg-info/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-08-07 16:07:02.000000 jianglab-0.7.7/jianglab.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-08-07 16:07:02.000000 jianglab-0.7.7/jianglab.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      168 2023-08-07 16:07:02.000000 jianglab-0.7.7/jianglab.egg-info/requires.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-08-07 16:07:02.000000 jianglab-0.7.7/jianglab.egg-info/top_level.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-08-07 16:07:02.654887 jianglab-0.7.7/setup.cfg
+-rw-r--r--   0 zhengjiang   (501) staff       (20)     1162 2023-08-07 16:06:57.000000 jianglab-0.7.7/setup.py
```

### Comparing `jianglab-0.7.6/PKG-INFO` & `jianglab-0.7.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.7.6
+Version: 0.7.7
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.7.6/README.md` & `jianglab-0.7.7/README.md`

 * *Files identical despite different names*

### Comparing `jianglab-0.7.6/jianglab/common_functions.py` & `jianglab-0.7.7/jianglab/common_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1202,19 +1202,38 @@
     
     plot_data = pd.DataFrame(embedding, columns=['umap1', 'umap2'])
     plot_data['Labels'] = X['Labels'].values
     sns.scatterplot(x='umap1', y='umap2', hue='Labels', data=plot_data)
 
     return plot_data
 
-def search_file_in_location(location, keyword1, keyword2 ="", recursive=True):
+# def search_file_in_location(location, keyword1, keyword2 ="", recursive=True):
+#     """Search for a file in a given location. 
+#     If recursive is True, the search will be recursive.
+#     search files that contain both keywords in their name."""
+#     if recursive:
+#         files = glob.glob(location + '/**/*', recursive=True)
+#     else:
+#         files = glob.glob(location + '/*', recursive=False)
+#     files = [f for f in files if keyword1 in f]
+#     if keyword2 != "":
+#         files = [f for f in files if keyword2 in f]
+#     return files
+
+def search_file_in_location(location, keyword_list=[], exclude_list = [], recursive=True):
     """Search for a file in a given location. 
     If recursive is True, the search will be recursive.
     search files that contain both keywords in their name."""
+    if type(keyword_list) == str:
+        keyword_list = [keyword_list]
+    if type(exclude_list) == str:
+        exclude_list = [exclude_list]
     if recursive:
         files = glob.glob(location + '/**/*', recursive=True)
     else:
         files = glob.glob(location + '/*', recursive=False)
-    files = [f for f in files if keyword1 in f]
-    if keyword2 != "":
-        files = [f for f in files if keyword2 in f]
-    return files
+    final_files = []
+    for keyword in keyword_list:
+        final_files.append([f for f in files if keyword in f])
+    for exclude_word in exclude_list:
+        final_files = [f for f in final_files if exclude_word not in f]
+    return final_files
```

### Comparing `jianglab-0.7.6/jianglab.egg-info/PKG-INFO` & `jianglab-0.7.7/jianglab.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.7.6
+Version: 0.7.7
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.7.6/setup.py` & `jianglab-0.7.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='jianglab',
-    version='0.7.6',
+    version='0.7.7',
     packages=find_packages(),
     install_requires=[
         "numpy",
         "pandas",
         "matplotlib",
         "treelib",
         "McsPyDataTools",
```

