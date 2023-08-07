# Comparing `tmp/utfuzz-0.1.4.tar.gz` & `tmp/utfuzz-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utfuzz-0.1.4.tar", max compression
+gzip compressed data, was "utfuzz-0.1.5.tar", max compression
```

## Comparing `utfuzz-0.1.4.tar` & `utfuzz-0.1.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     2531 2023-08-07 12:11:52.214890 utfuzz-0.1.4/README.md
--rw-r--r--   0        0        0      324 2023-08-07 13:32:53.693070 utfuzz-0.1.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-08-05 12:29:28.619794 utfuzz-0.1.4/utfuzz/__init__.py
--rw-r--r--   0        0        0       37 2023-08-07 09:51:23.339177 utfuzz-0.1.4/utfuzz/__main__.py
--rw-r--r--   0        0        0        0 2023-08-06 13:33:20.961223 utfuzz-0.1.4/utfuzz/config/__init__.py
--rw-r--r--   0        0        0      779 2023-08-07 08:07:29.350724 utfuzz-0.1.4/utfuzz/config/config_manager.py
--rw-r--r--   0        0        0        0 2023-08-06 08:46:59.594235 utfuzz-0.1.4/utfuzz/exceptions/__init__.py
--rw-r--r--   0        0        0      474 2023-08-06 13:45:21.520016 utfuzz-0.1.4/utfuzz/exceptions/exceptions.py
--rw-r--r--   0        0        0        0 2023-08-06 07:39:15.312321 utfuzz-0.1.4/utfuzz/file_manager/__init__.py
--rw-r--r--   0        0        0      118 2023-08-06 18:46:12.244717 utfuzz-0.1.4/utfuzz/file_manager/directory_manager.py
--rw-r--r--   0        0        0      577 2023-08-07 07:07:53.023797 utfuzz-0.1.4/utfuzz/file_manager/file_finder.py
--rw-r--r--   0        0        0     5552 2023-08-07 12:59:55.308606 utfuzz-0.1.4/utfuzz/main.py
--rw-r--r--   0        0        0     2405 2023-08-07 12:05:04.283720 utfuzz-0.1.4/utfuzz/parser.py
--rw-r--r--   0        0        0        0 2023-08-04 15:27:45.403178 utfuzz-0.1.4/utfuzz/requirements_managers/__init__.py
--rw-r--r--   0        0        0     1462 2023-08-07 11:01:58.158057 utfuzz-0.1.4/utfuzz/requirements_managers/abc_requirements_manager.py
--rw-r--r--   0        0        0     2140 2023-08-07 13:32:31.832494 utfuzz-0.1.4/utfuzz/requirements_managers/linux_java_manager.py
--rw-r--r--   0        0        0     1420 2023-08-07 08:27:51.941523 utfuzz-0.1.4/utfuzz/requirements_managers/python_requirements_manger.py
--rw-r--r--   0        0        0      569 2023-08-07 11:14:45.077070 utfuzz-0.1.4/utfuzz/requirements_managers/windows_java_manager.py
--rwxr-xr-x   0        0        0      134 2023-08-07 11:46:25.957650 utfuzz-0.1.4/utfuzz/utbot-cli-python.jar
--rw-r--r--   0        0        0        0 2023-08-04 15:27:37.153138 utfuzz-0.1.4/utfuzz/utbot_manager/__init__.py
--rw-r--r--   0        0        0      644 2023-08-07 07:36:12.080113 utfuzz-0.1.4/utfuzz/utbot_manager/utbot_manager.py
--rw-r--r--   0        0        0     3005 1970-01-01 00:00:00.000000 utfuzz-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     2531 2023-08-07 12:11:52.214890 utfuzz-0.1.5/README.md
+-rw-r--r--   0        0        0      324 2023-08-07 13:37:26.730360 utfuzz-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-05 12:29:28.619794 utfuzz-0.1.5/utfuzz/__init__.py
+-rw-r--r--   0        0        0       37 2023-08-07 09:51:23.339177 utfuzz-0.1.5/utfuzz/__main__.py
+-rw-r--r--   0        0        0        0 2023-08-06 13:33:20.961223 utfuzz-0.1.5/utfuzz/config/__init__.py
+-rw-r--r--   0        0        0      779 2023-08-07 08:07:29.350724 utfuzz-0.1.5/utfuzz/config/config_manager.py
+-rw-r--r--   0        0        0        0 2023-08-06 08:46:59.594235 utfuzz-0.1.5/utfuzz/exceptions/__init__.py
+-rw-r--r--   0        0        0      474 2023-08-06 13:45:21.520016 utfuzz-0.1.5/utfuzz/exceptions/exceptions.py
+-rw-r--r--   0        0        0        0 2023-08-06 07:39:15.312321 utfuzz-0.1.5/utfuzz/file_manager/__init__.py
+-rw-r--r--   0        0        0      118 2023-08-06 18:46:12.244717 utfuzz-0.1.5/utfuzz/file_manager/directory_manager.py
+-rw-r--r--   0        0        0      577 2023-08-07 07:07:53.023797 utfuzz-0.1.5/utfuzz/file_manager/file_finder.py
+-rw-r--r--   0        0        0     5605 2023-08-07 13:37:21.236878 utfuzz-0.1.5/utfuzz/main.py
+-rw-r--r--   0        0        0     2405 2023-08-07 12:05:04.283720 utfuzz-0.1.5/utfuzz/parser.py
+-rw-r--r--   0        0        0        0 2023-08-04 15:27:45.403178 utfuzz-0.1.5/utfuzz/requirements_managers/__init__.py
+-rw-r--r--   0        0        0     1462 2023-08-07 11:01:58.158057 utfuzz-0.1.5/utfuzz/requirements_managers/abc_requirements_manager.py
+-rw-r--r--   0        0        0     2139 2023-08-07 13:37:21.243545 utfuzz-0.1.5/utfuzz/requirements_managers/linux_java_manager.py
+-rw-r--r--   0        0        0     1420 2023-08-07 08:27:51.941523 utfuzz-0.1.5/utfuzz/requirements_managers/python_requirements_manger.py
+-rw-r--r--   0        0        0      589 2023-08-07 13:37:21.210211 utfuzz-0.1.5/utfuzz/requirements_managers/windows_java_manager.py
+-rwxr-xr-x   0        0        0      134 2023-08-07 11:46:25.957650 utfuzz-0.1.5/utfuzz/utbot-cli-python.jar
+-rw-r--r--   0        0        0        0 2023-08-04 15:27:37.153138 utfuzz-0.1.5/utfuzz/utbot_manager/__init__.py
+-rw-r--r--   0        0        0      644 2023-08-07 07:36:12.080113 utfuzz-0.1.5/utfuzz/utbot_manager/utbot_manager.py
+-rw-r--r--   0        0        0     3005 1970-01-01 00:00:00.000000 utfuzz-0.1.5/PKG-INFO
```

### Comparing `utfuzz-0.1.4/README.md` & `utfuzz-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `utfuzz-0.1.4/utfuzz/config/config_manager.py` & `utfuzz-0.1.5/utfuzz/config/config_manager.py`

 * *Files identical despite different names*

### Comparing `utfuzz-0.1.4/utfuzz/file_manager/file_finder.py` & `utfuzz-0.1.5/utfuzz/file_manager/file_finder.py`

 * *Files identical despite different names*

### Comparing `utfuzz-0.1.4/utfuzz/main.py` & `utfuzz-0.1.5/utfuzz/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,22 +50,26 @@
                 java_manager = WindowsJavaManager()
 
             try:
                 java = java_manager.check_java(java)
             except JavaIncompatible:
                 install = input('utfuzz depends on Java, try to install it? (Y/n) ')
                 if install in {'Y', ''}:
-                    java_manager.install_java()
+                    java = java_manager.install_java()
+
                 if java_manager.check_java(java) is None:
                     print('Cannot find Java or install it, please try to install Java>=17 manually and set it by '
                           'argument --java')
                     return
             except InvalidJavaVersion:
                 print('Cannot parse Java version. You can set Java>=17 by using argument --java')
                 return
+        if java is None:
+            return
+
         print(f'Selected Java: {java}')
 
         print(f'Set timeout (s) per one class or top-level functions in one file (set empty to choose {timeout}s)')
         custom_timeout = input(f'Timeout (default = {timeout}s): ')
         timeout = int(custom_timeout) if custom_timeout != '' else timeout
 
         custom_project_dir = input(f'Set project directory to generate tests (default = {project_dir}): ')
```

### Comparing `utfuzz-0.1.4/utfuzz/parser.py` & `utfuzz-0.1.5/utfuzz/parser.py`

 * *Files identical despite different names*

### Comparing `utfuzz-0.1.4/utfuzz/requirements_managers/abc_requirements_manager.py` & `utfuzz-0.1.5/utfuzz/requirements_managers/abc_requirements_manager.py`

 * *Files identical despite different names*

### Comparing `utfuzz-0.1.4/utfuzz/requirements_managers/linux_java_manager.py` & `utfuzz-0.1.5/utfuzz/requirements_managers/linux_java_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,11 +45,9 @@
                     subprocess.check_output(default_command)
                 else:
                     return
         except Exception:
             print(f"Cannot install Java automatically, please install Java 17 or newer, see instruction here: "
                   f"https://docs.oracle.com/en/java/javase/17/install/installation-jdk-linux-platforms.html"
                   )
-            return False
-
-
-        return True
+            return None
+        return "java"
```

### Comparing `utfuzz-0.1.4/utfuzz/requirements_managers/python_requirements_manger.py` & `utfuzz-0.1.5/utfuzz/requirements_managers/python_requirements_manger.py`

 * *Files identical despite different names*

### Comparing `utfuzz-0.1.4/utfuzz/requirements_managers/windows_java_manager.py` & `utfuzz-0.1.5/utfuzz/requirements_managers/windows_java_manager.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,7 +11,8 @@
     def check_platform(self) -> bool:
         return platform.system() == 'Windows'
 
     def install_java(self):
         print('You can see instruction here: '
               'https://docs.oracle.com/en/java/javase/17/install/installation-jdk-microsoft-windows-platforms.html'
               )
+        return None
```

### Comparing `utfuzz-0.1.4/utfuzz/utbot_manager/utbot_manager.py` & `utfuzz-0.1.5/utfuzz/utbot_manager/utbot_manager.py`

 * *Files identical despite different names*

### Comparing `utfuzz-0.1.4/PKG-INFO` & `utfuzz-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utfuzz
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 Author: Vyacheslav Tamarin
 Author-email: slavabarsuk@ya.ru
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

