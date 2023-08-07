# Comparing `tmp/todoist_auto-6.0.1.tar.gz` & `tmp/todoist_auto-6.0.2.tar.gz`

## Comparing `todoist_auto-6.0.1.tar` & `todoist_auto-6.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 todoist_auto-6.0.1/.github/workflows/publish-on-pip.yml
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 todoist_auto-6.0.1/src/todoist_auto/__init__.py
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 todoist_auto-6.0.1/src/todoist_auto/models.py
--rw-r--r--   0        0        0     4136 2020-02-02 00:00:00.000000 todoist_auto-6.0.1/src/todoist_auto/rm_empty_sections.py
--rw-r--r--   0        0        0     8653 2020-02-02 00:00:00.000000 todoist_auto-6.0.1/src/todoist_auto/routine.py
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 todoist_auto-6.0.1/src/todoist_auto/util.py
--rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 todoist_auto-6.0.1/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 todoist_auto-6.0.1/LICENSE
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 todoist_auto-6.0.1/README.md
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 todoist_auto-6.0.1/pyproject.toml
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 todoist_auto-6.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 todoist_auto-6.0.2/.github/workflows/publish-on-pip.yml
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 todoist_auto-6.0.2/src/todoist_auto/__init__.py
+-rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 todoist_auto-6.0.2/src/todoist_auto/models.py
+-rw-r--r--   0        0        0     4136 2020-02-02 00:00:00.000000 todoist_auto-6.0.2/src/todoist_auto/rm_empty_sections.py
+-rw-r--r--   0        0        0     8653 2020-02-02 00:00:00.000000 todoist_auto-6.0.2/src/todoist_auto/routine.py
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 todoist_auto-6.0.2/src/todoist_auto/util.py
+-rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 todoist_auto-6.0.2/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 todoist_auto-6.0.2/LICENSE
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 todoist_auto-6.0.2/README.md
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 todoist_auto-6.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 todoist_auto-6.0.2/PKG-INFO
```

### Comparing `todoist_auto-6.0.1/.github/workflows/publish-on-pip.yml` & `todoist_auto-6.0.2/.github/workflows/publish-on-pip.yml`

 * *Files identical despite different names*

### Comparing `todoist_auto-6.0.1/src/todoist_auto/models.py` & `todoist_auto-6.0.2/src/todoist_auto/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,11 +74,11 @@
     pg_url = 'https://api.notion.com/v1/pages/'
     hdrs = {
             'Authorization'  : f'Bearer {tok}' ,
             'Notion-Version' : '2022-06-28' ,
             }
 
 class Todoist :
-    tok = get_token('todoist_auto')
+    tok = get_token('Todoist')
     hdrs = {
             'Authorization' : f'Bearer {tok}'
             }
```

### Comparing `todoist_auto-6.0.1/src/todoist_auto/rm_empty_sections.py` & `todoist_auto-6.0.2/src/todoist_auto/rm_empty_sections.py`

 * *Files identical despite different names*

### Comparing `todoist_auto-6.0.1/src/todoist_auto/routine.py` & `todoist_auto-6.0.2/src/todoist_auto/routine.py`

 * *Files identical despite different names*

### Comparing `todoist_auto-6.0.1/src/todoist_auto/util.py` & `todoist_auto-6.0.2/src/todoist_auto/util.py`

 * *Files identical despite different names*

### Comparing `todoist_auto-6.0.1/.gitignore` & `todoist_auto-6.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `todoist_auto-6.0.1/LICENSE` & `todoist_auto-6.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `todoist_auto-6.0.1/PKG-INFO` & `todoist_auto-6.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: todoist_auto
-Version: 6.0.1
+Version: 6.0.2
 Summary: Automating Todoist
 Author-email: Mahdi Mir <imahdimir@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Mahdi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

