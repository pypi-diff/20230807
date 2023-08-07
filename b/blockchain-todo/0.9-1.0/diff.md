# Comparing `tmp/blockchain_todo-0.9.tar.gz` & `tmp/blockchain_todo-1.0.tar.gz`

## Comparing `blockchain_todo-0.9.tar` & `blockchain_todo-1.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 blockchain_todo-0.9/src/blockchain_todo/__init__.py
--rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 blockchain_todo-0.9/src/blockchain_todo/app.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 blockchain_todo-0.9/LICENSE
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 blockchain_todo-0.9/README.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 blockchain_todo-0.9/pyproject.toml
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 blockchain_todo-0.9/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 blockchain_todo-1.0/src/blockchain_todo/__init__.py
+-rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 blockchain_todo-1.0/src/blockchain_todo/app.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 blockchain_todo-1.0/LICENSE
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 blockchain_todo-1.0/README.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 blockchain_todo-1.0/pyproject.toml
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 blockchain_todo-1.0/PKG-INFO
```

### Comparing `blockchain_todo-0.9/src/blockchain_todo/app.py` & `blockchain_todo-1.0/src/blockchain_todo/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
         print('[任务详情]',detail)
     def check(self):
         '''
         审查数据安全性和完整性
         '''
         if self.chain.check():
             print('审查完成,当前Blockchain_Todo数据安全')
-            print('建议定期审查,确保数据完整和安装')
+            print('建议定期审查,确保数据完整和安全')
         else:
             print('当前Blockchain_Todo数据疑似遭到修改! 建议提交反馈给Crillerium')
             print('提交地址: https://github.com/crillerium/blockchain-todo/issues')
 
 def main():
     try:
         fire.Fire(Todo)
```

### Comparing `blockchain_todo-0.9/LICENSE` & `blockchain_todo-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `blockchain_todo-0.9/pyproject.toml` & `blockchain_todo-1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "blockchain_todo"
 dependencies = ["loongchain","fire"]
-version = "0.9"
+version = "1.0"
 authors = [
   { name="Crillerium", email="crillerium@outlook.com" },
 ]
 description = "A Blockchain Supported To Do List"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `blockchain_todo-0.9/PKG-INFO` & `blockchain_todo-1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blockchain_todo
-Version: 0.9
+Version: 1.0
 Summary: A Blockchain Supported To Do List
 Project-URL: Home-page, https://github.com/crillerium/
 Author-email: Crillerium <crillerium@outlook.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

