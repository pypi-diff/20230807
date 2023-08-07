# Comparing `tmp/todoist_auto-5.0.1.tar.gz` & `tmp/todoist_auto-5.0.2.tar.gz`

## Comparing `todoist_auto-5.0.1.tar` & `todoist_auto-5.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 todoist_auto-5.0.1/.github/workflows/publish-on-pip.yml
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 todoist_auto-5.0.1/src/Todoist/__init__.py
--rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 todoist_auto-5.0.1/src/Todoist/models.py
--rw-r--r--   0        0        0     4128 2020-02-02 00:00:00.000000 todoist_auto-5.0.1/src/Todoist/rm_empty_sections.py
--rw-r--r--   0        0        0     8641 2020-02-02 00:00:00.000000 todoist_auto-5.0.1/src/Todoist/routine.py
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 todoist_auto-5.0.1/src/Todoist/util.py
--rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 todoist_auto-5.0.1/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 todoist_auto-5.0.1/LICENSE
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 todoist_auto-5.0.1/README.md
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 todoist_auto-5.0.1/pyproject.toml
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 todoist_auto-5.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 todoist_auto-5.0.2/.github/workflows/publish-on-pip.yml
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 todoist_auto-5.0.2/src/Todoist/__init__.py
+-rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 todoist_auto-5.0.2/src/Todoist/models.py
+-rw-r--r--   0        0        0     4128 2020-02-02 00:00:00.000000 todoist_auto-5.0.2/src/Todoist/rm_empty_sections.py
+-rw-r--r--   0        0        0     8641 2020-02-02 00:00:00.000000 todoist_auto-5.0.2/src/Todoist/routine.py
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 todoist_auto-5.0.2/src/Todoist/util.py
+-rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 todoist_auto-5.0.2/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 todoist_auto-5.0.2/LICENSE
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 todoist_auto-5.0.2/README.md
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 todoist_auto-5.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 todoist_auto-5.0.2/PKG-INFO
```

### Comparing `todoist_auto-5.0.1/.github/workflows/publish-on-pip.yml` & `todoist_auto-5.0.2/.github/workflows/publish-on-pip.yml`

 * *Files identical despite different names*

### Comparing `todoist_auto-5.0.1/src/Todoist/models.py` & `todoist_auto-5.0.2/src/Todoist/models.py`

 * *Files identical despite different names*

### Comparing `todoist_auto-5.0.1/src/Todoist/rm_empty_sections.py` & `todoist_auto-5.0.2/src/Todoist/rm_empty_sections.py`

 * *Files identical despite different names*

### Comparing `todoist_auto-5.0.1/src/Todoist/routine.py` & `todoist_auto-5.0.2/src/Todoist/routine.py`

 * *Files identical despite different names*

### Comparing `todoist_auto-5.0.1/src/Todoist/util.py` & `todoist_auto-5.0.2/src/Todoist/util.py`

 * *Files identical despite different names*

### Comparing `todoist_auto-5.0.1/.gitignore` & `todoist_auto-5.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `todoist_auto-5.0.1/LICENSE` & `todoist_auto-5.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `todoist_auto-5.0.1/PKG-INFO` & `todoist_auto-5.0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: todoist_auto
-Version: 5.0.1
+Version: 5.0.2
 Summary: Automating Todoist
 Author-email: Mahdi Mir <imahdimir@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Mahdi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -25,11 +25,11 @@
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 License-File: LICENSE
 Requires-Dist: mtok==1.1.1
 Requires-Dist: pandas==2.0.3
 Requires-Dist: pytz==2023.3
 Requires-Dist: requests==2.31.0
-Requires-Dist: todoist-api-python==2.0.2
+Requires-Dist: todoist-api-python
 Description-Content-Type: text/markdown
 
 Automating Todoist
```

