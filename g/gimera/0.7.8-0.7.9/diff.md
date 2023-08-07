# Comparing `tmp/gimera-0.7.8.tar.gz` & `tmp/gimera-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gimera-0.7.8.tar", last modified: Sun Aug  6 17:11:15 2023, max compression
+gzip compressed data, was "gimera-0.7.9.tar", last modified: Mon Aug  7 15:06:20 2023, max compression
```

## Comparing `gimera-0.7.8.tar` & `gimera-0.7.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:11:15.048273 gimera-0.7.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-06 17:10:28.000000 gimera-0.7.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-08-06 17:11:15.048273 gimera-0.7.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-08-06 17:10:28.000000 gimera-0.7.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:11:15.048273 gimera-0.7.8/gimera/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-08-06 17:10:28.000000 gimera-0.7.8/gimera/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10613 2023-08-06 17:10:28.000000 gimera-0.7.8/gimera/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-08-06 17:10:28.000000 gimera-0.7.8/gimera/consts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    29388 2023-08-06 17:10:28.000000 gimera-0.7.8/gimera/gimera.py
--rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-08-06 17:10:28.000000 gimera-0.7.8/gimera/gitcommands.py
--rw-r--r--   0 runner    (1001) docker     (123)    14437 2023-08-06 17:10:28.000000 gimera-0.7.8/gimera/patches.py
--rw-r--r--   0 runner    (1001) docker     (123)    13246 2023-08-06 17:10:28.000000 gimera-0.7.8/gimera/repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-08-06 17:10:28.000000 gimera-0.7.8/gimera/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:11:15.048273 gimera-0.7.8/gimera.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-08-06 17:11:15.000000 gimera-0.7.8/gimera.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-08-06 17:11:15.000000 gimera-0.7.8/gimera.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 17:11:15.000000 gimera-0.7.8/gimera.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-06 17:11:15.000000 gimera-0.7.8/gimera.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-06 17:11:15.000000 gimera-0.7.8/gimera.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-06 17:11:15.000000 gimera-0.7.8/gimera.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-08-06 17:11:15.048273 gimera-0.7.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-08-06 17:10:28.000000 gimera-0.7.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:06:20.017770 gimera-0.7.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-07 15:05:42.000000 gimera-0.7.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-08-07 15:06:20.017770 gimera-0.7.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-08-07 15:05:42.000000 gimera-0.7.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:06:20.017770 gimera-0.7.9/gimera/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-08-07 15:05:42.000000 gimera-0.7.9/gimera/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10613 2023-08-07 15:05:42.000000 gimera-0.7.9/gimera/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-08-07 15:05:42.000000 gimera-0.7.9/gimera/consts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29418 2023-08-07 15:05:42.000000 gimera-0.7.9/gimera/gimera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-08-07 15:05:42.000000 gimera-0.7.9/gimera/gitcommands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14437 2023-08-07 15:05:42.000000 gimera-0.7.9/gimera/patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13246 2023-08-07 15:05:42.000000 gimera-0.7.9/gimera/repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-08-07 15:05:42.000000 gimera-0.7.9/gimera/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:06:20.017770 gimera-0.7.9/gimera.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-08-07 15:06:19.000000 gimera-0.7.9/gimera.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-08-07 15:06:20.000000 gimera-0.7.9/gimera.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 15:06:19.000000 gimera-0.7.9/gimera.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-07 15:06:19.000000 gimera-0.7.9/gimera.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-07 15:06:19.000000 gimera-0.7.9/gimera.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-07 15:06:19.000000 gimera-0.7.9/gimera.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-08-07 15:06:20.017770 gimera-0.7.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-08-07 15:05:42.000000 gimera-0.7.9/setup.py
```

### Comparing `gimera-0.7.8/LICENSE.txt` & `gimera-0.7.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gimera-0.7.8/PKG-INFO` & `gimera-0.7.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gimera
-Version: 0.7.8
+Version: 0.7.9
 Summary: Handling git submodules and patches per yml
 Home-page: https://github.com/marcwimmer/gimera
 Author: Marc-Christian Wimmer
 Author-email: marc@itewimmer.de
 License: MIT
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
```

### Comparing `gimera-0.7.8/README.md` & `gimera-0.7.9/README.md`

 * *Files identical despite different names*

### Comparing `gimera-0.7.8/gimera/config.py` & `gimera-0.7.9/gimera/config.py`

 * *Files identical despite different names*

### Comparing `gimera-0.7.8/gimera/gimera.py` & `gimera-0.7.9/gimera/gimera.py`

 * *Files 0% similar despite different names*

```diff
@@ -298,14 +298,15 @@
                 _make_sure_subrepo_is_checked_out(main_repo, repo)
                 _fetch_latest_commit_in_submodule(main_repo, repo, update=update)
             elif repo.type == REPO_TYPE_INT:
                 if not no_patches:
                     try:
                         make_patches(main_repo, repo)
                     except Exception as ex:
+                        raise
                         msg = f"Error making patches for: {repo.path}\n\n{ex}"
                         _raise_error(msg)
 
                 try:
                     _update_integrated_module(
                         main_repo, repo, update, parallel_safe, **options
                     )
```

### Comparing `gimera-0.7.8/gimera/gitcommands.py` & `gimera-0.7.9/gimera/gitcommands.py`

 * *Files identical despite different names*

### Comparing `gimera-0.7.8/gimera/patches.py` & `gimera-0.7.9/gimera/patches.py`

 * *Files identical despite different names*

### Comparing `gimera-0.7.8/gimera/repo.py` & `gimera-0.7.9/gimera/repo.py`

 * *Files identical despite different names*

### Comparing `gimera-0.7.8/gimera/tools.py` & `gimera-0.7.9/gimera/tools.py`

 * *Files identical despite different names*

### Comparing `gimera-0.7.8/gimera.egg-info/PKG-INFO` & `gimera-0.7.9/gimera.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gimera
-Version: 0.7.8
+Version: 0.7.9
 Summary: Handling git submodules and patches per yml
 Home-page: https://github.com/marcwimmer/gimera
 Author: Marc-Christian Wimmer
 Author-email: marc@itewimmer.de
 License: MIT
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
```

### Comparing `gimera-0.7.8/setup.py` & `gimera-0.7.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 current_dir = Path(os.path.dirname(os.path.abspath(inspect.getfile(inspect.currentframe()))))
 setup_cfg = read_configuration("setup.cfg")
 metadata = setup_cfg['metadata']
 NAME = metadata['name']
 
 # What packages are required for this module to be executed?
 REQUIRED = [
-	"click==8.1.3", "inquirer", "pyyaml", "pytest"
+	"click==8.1.3", "inquirer", "pyyaml", "pytest", "pudb"
 ]
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 try:
     with io.open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
         long_description = '\n' + f.read()
```

