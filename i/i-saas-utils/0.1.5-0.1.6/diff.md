# Comparing `tmp/i_saas_utils-0.1.5.tar.gz` & `tmp/i_saas_utils-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "i_saas_utils-0.1.5.tar", max compression
+gzip compressed data, was "i_saas_utils-0.1.6.tar", max compression
```

## Comparing `i_saas_utils-0.1.5.tar` & `i_saas_utils-0.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     6254 2023-07-28 20:15:16.157658 i_saas_utils-0.1.5/README.md
--rw-r--r--   0        0        0        0 2023-07-28 15:49:56.000000 i_saas_utils-0.1.5/i_saas_utils/__init__.py
--rw-r--r--   0        0        0       28 2023-07-29 11:00:00.646286 i_saas_utils-0.1.5/i_saas_utils/ansible/__init__.py
--rw-r--r--   0        0        0      517 2023-07-29 11:08:59.134950 i_saas_utils-0.1.5/i_saas_utils/ansible/ansibl.py
--rw-r--r--   0        0        0       87 2023-08-01 22:29:40.238936 i_saas_utils-0.1.5/i_saas_utils/git/__init__.py
--rw-r--r--   0        0        0      494 2023-08-01 22:31:19.215972 i_saas_utils-0.1.5/i_saas_utils/git/git.py
--rw-r--r--   0        0        0     1333 2023-08-02 17:20:38.039976 i_saas_utils-0.1.5/i_saas_utils/git/git_project.py
--rw-r--r--   0        0        0     1402 2023-08-02 09:50:52.851591 i_saas_utils-0.1.5/i_saas_utils/git/git_repo.py
--rw-r--r--   0        0        0       23 2023-07-29 11:01:01.438716 i_saas_utils-0.1.5/i_saas_utils/k8s/__init__.py
--rw-r--r--   0        0        0      916 2023-07-28 21:36:56.880915 i_saas_utils-0.1.5/i_saas_utils/k8s/kube.py
--rw-r--r--   0        0        0      175 2023-08-02 10:42:19.635442 i_saas_utils-0.1.5/i_saas_utils/saas/__init__.py
--rw-r--r--   0        0        0     3222 2023-08-02 09:50:03.799033 i_saas_utils-0.1.5/i_saas_utils/saas/saas.py
--rw-r--r--   0        0        0       57 2023-07-29 11:01:01.418716 i_saas_utils-0.1.5/i_saas_utils/templates/__init__.py
--rw-r--r--   0        0        0      646 2023-07-29 19:49:55.600690 i_saas_utils-0.1.5/i_saas_utils/templates/render.py
--rw-r--r--   0        0        0      107 2023-08-02 17:12:47.621841 i_saas_utils-0.1.5/i_saas_utils/types/__init__.py
--rw-r--r--   0        0        0      386 2023-08-02 17:24:41.119490 i_saas_utils-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     6765 1970-01-01 00:00:00.000000 i_saas_utils-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     6254 2023-07-28 20:15:16.157658 i_saas_utils-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2023-07-28 15:49:56.000000 i_saas_utils-0.1.6/i_saas_utils/__init__.py
+-rw-r--r--   0        0        0       28 2023-07-29 11:00:00.646286 i_saas_utils-0.1.6/i_saas_utils/ansible/__init__.py
+-rw-r--r--   0        0        0      517 2023-07-29 11:08:59.134950 i_saas_utils-0.1.6/i_saas_utils/ansible/ansibl.py
+-rw-r--r--   0        0        0       87 2023-08-01 22:29:40.238936 i_saas_utils-0.1.6/i_saas_utils/git/__init__.py
+-rw-r--r--   0        0        0      494 2023-08-01 22:31:19.215972 i_saas_utils-0.1.6/i_saas_utils/git/git.py
+-rw-r--r--   0        0        0     1333 2023-08-02 17:20:38.039976 i_saas_utils-0.1.6/i_saas_utils/git/git_project.py
+-rw-r--r--   0        0        0     1402 2023-08-02 09:50:52.851591 i_saas_utils-0.1.6/i_saas_utils/git/git_repo.py
+-rw-r--r--   0        0        0       23 2023-07-29 11:01:01.438716 i_saas_utils-0.1.6/i_saas_utils/k8s/__init__.py
+-rw-r--r--   0        0        0      916 2023-07-28 21:36:56.880915 i_saas_utils-0.1.6/i_saas_utils/k8s/kube.py
+-rw-r--r--   0        0        0      175 2023-08-02 10:42:19.635442 i_saas_utils-0.1.6/i_saas_utils/saas/__init__.py
+-rw-r--r--   0        0        0     3235 2023-08-06 17:04:43.252805 i_saas_utils-0.1.6/i_saas_utils/saas/saas.py
+-rw-r--r--   0        0        0       57 2023-07-29 11:01:01.418716 i_saas_utils-0.1.6/i_saas_utils/templates/__init__.py
+-rw-r--r--   0        0        0      682 2023-08-06 17:05:15.725004 i_saas_utils-0.1.6/i_saas_utils/templates/render.py
+-rw-r--r--   0        0        0      107 2023-08-02 17:12:47.621841 i_saas_utils-0.1.6/i_saas_utils/types/__init__.py
+-rw-r--r--   0        0        0      386 2023-08-07 07:07:54.908690 i_saas_utils-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     6765 1970-01-01 00:00:00.000000 i_saas_utils-0.1.6/PKG-INFO
```

### Comparing `i_saas_utils-0.1.5/README.md` & `i_saas_utils-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `i_saas_utils-0.1.5/i_saas_utils/ansible/ansibl.py` & `i_saas_utils-0.1.6/i_saas_utils/ansible/ansibl.py`

 * *Files identical despite different names*

### Comparing `i_saas_utils-0.1.5/i_saas_utils/git/git_project.py` & `i_saas_utils-0.1.6/i_saas_utils/git/git_project.py`

 * *Files identical despite different names*

### Comparing `i_saas_utils-0.1.5/i_saas_utils/git/git_repo.py` & `i_saas_utils-0.1.6/i_saas_utils/git/git_repo.py`

 * *Files identical despite different names*

### Comparing `i_saas_utils-0.1.5/i_saas_utils/k8s/kube.py` & `i_saas_utils-0.1.6/i_saas_utils/k8s/kube.py`

 * *Files identical despite different names*

### Comparing `i_saas_utils-0.1.5/i_saas_utils/saas/saas.py` & `i_saas_utils-0.1.6/i_saas_utils/saas/saas.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,10 +108,13 @@
         response = requests.post(self.url, data=payload)
 
         if response.status_code != 200:
             raise Exception(f"Can't send notify - {response.text}")
 
 
 def generate_service_name(
-    namespace: str = "", env: str = "", type: str = "", uniq_name: str = ""
+    namespace: str = "",
+    uniq_name: str = "",
+    type: str = "",
+    env: str = "",
 ):
     return "-".join(filter(lambda x: x, [namespace, uniq_name, type, env]))
```

### Comparing `i_saas_utils-0.1.5/i_saas_utils/templates/render.py` & `i_saas_utils-0.1.6/i_saas_utils/templates/render.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import os
 
 from jinja2 import Template
 
 from i_saas_utils.saas import get_list_files
 
 
-def render_dir(source: str, dest: str, data: dict) -> None:
+def render_dir(source: str, dest: str, data: dict, exist_dir_ok: bool = False) -> None:
     for file in get_list_files(source, short_name=True):
         path = os.path.join(dest, file)
-        os.makedirs(os.path.dirname(path), exist_ok=True)
+        os.makedirs(os.path.dirname(path), exist_ok=exist_dir_ok)
         render_file(os.path.join(source, file), path, data)
 
 
 def render_file(source: str, dest: str, data: dict) -> None:
     with open(source, "r") as inp, open(render_text(dest, data), "w") as out:
         out.write(render_text(inp.read(), data))
```

### Comparing `i_saas_utils-0.1.5/PKG-INFO` & `i_saas_utils-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: i-saas-utils
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 Author: Fedorov Stepan
 Author-email: fedorov.stepan2@wb.ru
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: dnspython (>=2.4.1,<3.0.0)
```

