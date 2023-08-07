# Comparing `tmp/mtok-1.1.0.tar.gz` & `tmp/mtok-1.1.1.tar.gz`

## Comparing `mtok-1.1.0.tar` & `mtok-1.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 mtok-1.1.0/.github/workflows/publish-on-pip.yml
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 mtok-1.1.0/src/mtok/__init__.py
--rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 mtok-1.1.0/src/mtok/mtok.py
--rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 mtok-1.1.0/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 mtok-1.1.0/LICENSE
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 mtok-1.1.0/README.md
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 mtok-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 mtok-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 mtok-1.1.1/.github/workflows/publish-on-pip.yml
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 mtok-1.1.1/src/mtok/__init__.py
+-rw-r--r--   0        0        0     3518 2020-02-02 00:00:00.000000 mtok-1.1.1/src/mtok/mtok.py
+-rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 mtok-1.1.1/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 mtok-1.1.1/LICENSE
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 mtok-1.1.1/README.md
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 mtok-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 mtok-1.1.1/PKG-INFO
```

### Comparing `mtok-1.1.0/.github/workflows/publish-on-pip.yml` & `mtok-1.1.1/.github/workflows/publish-on-pip.yml`

 * *Files identical despite different names*

### Comparing `mtok-1.1.0/src/mtok/mtok.py` & `mtok-1.1.1/src/mtok/mtok.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     # local GitHub token filename
     lg = '.gt.json'
 
     # local directories for GitHub token json file
     ld = {
             'mac'          : '/Users/mahdi/Dropbox/0-Arch/' ,
             'teias-ubuntu' : '/home/mahdi/Downloads/' ,
-            'datalore'     : '/data/workspace_files/.private/.gt.json'
+            'datalore'     : '/data/workspace_files/.private/'
             }
 
 k = Const()
 
 @dataclass
 class KeyVal :
     key: str
```

### Comparing `mtok-1.1.0/.gitignore` & `mtok-1.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `mtok-1.1.0/LICENSE` & `mtok-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mtok-1.1.0/PKG-INFO` & `mtok-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtok
-Version: 1.1.0
+Version: 1.1.1
 Summary: Gets the token from the private tokens repository.
 Project-URL: Homepage, https://github.com/imahdimir/mtok
 Project-URL: Bug Tracker, https://github.com/imahdimir/mtok/issues
 Author-email: Mahdi Mir <imahdimir@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Mahdi
```

