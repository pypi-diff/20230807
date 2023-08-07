# Comparing `tmp/utfuzz-0.1.2.tar.gz` & `tmp/utfuzz-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utfuzz-0.1.2.tar", max compression
+gzip compressed data, was "utfuzz-0.1.3.tar", max compression
```

## Comparing `utfuzz-0.1.2.tar` & `utfuzz-0.1.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     2531 2023-08-07 12:11:52.214890 utfuzz-0.1.2/README.md
--rw-r--r--   0        0        0      324 2023-08-07 12:38:28.749535 utfuzz-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-08-05 12:29:28.619794 utfuzz-0.1.2/utfuzz/__init__.py
--rw-r--r--   0        0        0       37 2023-08-07 09:51:23.339177 utfuzz-0.1.2/utfuzz/__main__.py
--rw-r--r--   0        0        0        0 2023-08-06 13:33:20.961223 utfuzz-0.1.2/utfuzz/config/__init__.py
--rw-r--r--   0        0        0      779 2023-08-07 08:07:29.350724 utfuzz-0.1.2/utfuzz/config/config_manager.py
--rw-r--r--   0        0        0        0 2023-08-06 08:46:59.594235 utfuzz-0.1.2/utfuzz/exceptions/__init__.py
--rw-r--r--   0        0        0      474 2023-08-06 13:45:21.520016 utfuzz-0.1.2/utfuzz/exceptions/exceptions.py
--rw-r--r--   0        0        0        0 2023-08-06 07:39:15.312321 utfuzz-0.1.2/utfuzz/file_manager/__init__.py
--rw-r--r--   0        0        0      118 2023-08-06 18:46:12.244717 utfuzz-0.1.2/utfuzz/file_manager/directory_manager.py
--rw-r--r--   0        0        0      577 2023-08-07 07:07:53.023797 utfuzz-0.1.2/utfuzz/file_manager/file_finder.py
--rw-r--r--   0        0        0     5260 2023-08-07 12:42:57.854978 utfuzz-0.1.2/utfuzz/main.py
--rw-r--r--   0        0        0     2405 2023-08-07 12:05:04.283720 utfuzz-0.1.2/utfuzz/parser.py
--rw-r--r--   0        0        0        0 2023-08-04 15:27:45.403178 utfuzz-0.1.2/utfuzz/requirements_managers/__init__.py
--rw-r--r--   0        0        0     1462 2023-08-07 11:01:58.158057 utfuzz-0.1.2/utfuzz/requirements_managers/abc_requirements_manager.py
--rw-r--r--   0        0        0     1615 2023-08-07 12:42:57.868313 utfuzz-0.1.2/utfuzz/requirements_managers/linux_java_manager.py
--rw-r--r--   0        0        0     1420 2023-08-07 08:27:51.941523 utfuzz-0.1.2/utfuzz/requirements_managers/python_requirements_manger.py
--rw-r--r--   0        0        0      569 2023-08-07 11:14:45.077070 utfuzz-0.1.2/utfuzz/requirements_managers/windows_java_manager.py
--rwxr-xr-x   0        0        0      134 2023-08-07 11:46:25.957650 utfuzz-0.1.2/utfuzz/utbot-cli-python.jar
--rw-r--r--   0        0        0        0 2023-08-04 15:27:37.153138 utfuzz-0.1.2/utfuzz/utbot_manager/__init__.py
--rw-r--r--   0        0        0      644 2023-08-07 07:36:12.080113 utfuzz-0.1.2/utfuzz/utbot_manager/utbot_manager.py
--rw-r--r--   0        0        0     3005 1970-01-01 00:00:00.000000 utfuzz-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     2531 2023-08-07 12:11:52.214890 utfuzz-0.1.3/README.md
+-rw-r--r--   0        0        0      324 2023-08-07 12:47:14.908255 utfuzz-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-05 12:29:28.619794 utfuzz-0.1.3/utfuzz/__init__.py
+-rw-r--r--   0        0        0       37 2023-08-07 09:51:23.339177 utfuzz-0.1.3/utfuzz/__main__.py
+-rw-r--r--   0        0        0        0 2023-08-06 13:33:20.961223 utfuzz-0.1.3/utfuzz/config/__init__.py
+-rw-r--r--   0        0        0      779 2023-08-07 08:07:29.350724 utfuzz-0.1.3/utfuzz/config/config_manager.py
+-rw-r--r--   0        0        0        0 2023-08-06 08:46:59.594235 utfuzz-0.1.3/utfuzz/exceptions/__init__.py
+-rw-r--r--   0        0        0      474 2023-08-06 13:45:21.520016 utfuzz-0.1.3/utfuzz/exceptions/exceptions.py
+-rw-r--r--   0        0        0        0 2023-08-06 07:39:15.312321 utfuzz-0.1.3/utfuzz/file_manager/__init__.py
+-rw-r--r--   0        0        0      118 2023-08-06 18:46:12.244717 utfuzz-0.1.3/utfuzz/file_manager/directory_manager.py
+-rw-r--r--   0        0        0      577 2023-08-07 07:07:53.023797 utfuzz-0.1.3/utfuzz/file_manager/file_finder.py
+-rw-r--r--   0        0        0     5454 2023-08-07 12:47:10.147938 utfuzz-0.1.3/utfuzz/main.py
+-rw-r--r--   0        0        0     2405 2023-08-07 12:05:04.283720 utfuzz-0.1.3/utfuzz/parser.py
+-rw-r--r--   0        0        0        0 2023-08-04 15:27:45.403178 utfuzz-0.1.3/utfuzz/requirements_managers/__init__.py
+-rw-r--r--   0        0        0     1462 2023-08-07 11:01:58.158057 utfuzz-0.1.3/utfuzz/requirements_managers/abc_requirements_manager.py
+-rw-r--r--   0        0        0     1732 2023-08-07 12:44:16.811785 utfuzz-0.1.3/utfuzz/requirements_managers/linux_java_manager.py
+-rw-r--r--   0        0        0     1420 2023-08-07 08:27:51.941523 utfuzz-0.1.3/utfuzz/requirements_managers/python_requirements_manger.py
+-rw-r--r--   0        0        0      569 2023-08-07 11:14:45.077070 utfuzz-0.1.3/utfuzz/requirements_managers/windows_java_manager.py
+-rwxr-xr-x   0        0        0      134 2023-08-07 11:46:25.957650 utfuzz-0.1.3/utfuzz/utbot-cli-python.jar
+-rw-r--r--   0        0        0        0 2023-08-04 15:27:37.153138 utfuzz-0.1.3/utfuzz/utbot_manager/__init__.py
+-rw-r--r--   0        0        0      644 2023-08-07 07:36:12.080113 utfuzz-0.1.3/utfuzz/utbot_manager/utbot_manager.py
+-rw-r--r--   0        0        0     3005 1970-01-01 00:00:00.000000 utfuzz-0.1.3/PKG-INFO
```

### Comparing `utfuzz-0.1.2/README.md` & `utfuzz-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `utfuzz-0.1.2/utfuzz/config/config_manager.py` & `utfuzz-0.1.3/utfuzz/config/config_manager.py`

 * *Files identical despite different names*

### Comparing `utfuzz-0.1.2/utfuzz/file_manager/file_finder.py` & `utfuzz-0.1.3/utfuzz/file_manager/file_finder.py`

 * *Files identical despite different names*

### Comparing `utfuzz-0.1.2/utfuzz/main.py` & `utfuzz-0.1.3/utfuzz/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,18 +49,20 @@
 
             try:
                 java = java_manager.check_java(java)
             except JavaIncompatible:
                 install = input('utfuzz depends on Java, try to install it? (Y/n) ')
                 if install in {'Y', ''}:
                     java_manager.install_java()
-                else:
+                if java_manager.check_java(java) is None:
+                    print('Cannot find Java or install it, please try to install Java>=17 manually and set it by '
+                          'argument --java')
                     return
             except InvalidJavaVersion:
-                print('Cannot parse Java version. You can set Java >= 17 by using argument --java')
+                print('Cannot parse Java version. You can set Java>=17 by using argument --java')
                 return
         print(f'Selected Java: {java}')
 
         print(f'Set timeout (s) per one class or top-level functions in one file (set empty to choose {timeout}s)')
         custom_timeout = input(f'Timeout (default = {timeout}s): ')
         timeout = int(custom_timeout) if custom_timeout != '' else timeout
```

### Comparing `utfuzz-0.1.2/utfuzz/parser.py` & `utfuzz-0.1.3/utfuzz/parser.py`

 * *Files identical despite different names*

### Comparing `utfuzz-0.1.2/utfuzz/requirements_managers/abc_requirements_manager.py` & `utfuzz-0.1.3/utfuzz/requirements_managers/abc_requirements_manager.py`

 * *Files identical despite different names*

### Comparing `utfuzz-0.1.2/utfuzz/requirements_managers/linux_java_manager.py` & `utfuzz-0.1.3/utfuzz/requirements_managers/linux_java_manager.py`

 * *Files 16% similar despite different names*

```diff
@@ -29,13 +29,16 @@
             install_command = ['sudo', 'apt-get', 'install', 'openjdk-17-jdk']
         else:
             install_command = []
 
         try:
             if len(install_command) != 0:
                 print('Try to install java...')
-                input('Run this command? ' + ' '.join(install_command))
-                subprocess.check_output(install_command)
+                install = input('Run this command? ' + ' '.join(install_command) + '? (Y/n) ')
+                if install in {'Y', ''}:
+                    subprocess.check_output(install_command)
+                else:
+                    return
         except Exception:
             print(f"Cannot install Java automatically, please install Java 17 or newer, see instruction here: "
                   f"https://docs.oracle.com/en/java/javase/17/install/installation-jdk-linux-platforms.html"
                   )
```

### Comparing `utfuzz-0.1.2/utfuzz/requirements_managers/python_requirements_manger.py` & `utfuzz-0.1.3/utfuzz/requirements_managers/python_requirements_manger.py`

 * *Files identical despite different names*

### Comparing `utfuzz-0.1.2/utfuzz/requirements_managers/windows_java_manager.py` & `utfuzz-0.1.3/utfuzz/requirements_managers/windows_java_manager.py`

 * *Files identical despite different names*

### Comparing `utfuzz-0.1.2/utfuzz/utbot_manager/utbot_manager.py` & `utfuzz-0.1.3/utfuzz/utbot_manager/utbot_manager.py`

 * *Files identical despite different names*

### Comparing `utfuzz-0.1.2/PKG-INFO` & `utfuzz-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utfuzz
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: Vyacheslav Tamarin
 Author-email: slavabarsuk@ya.ru
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

