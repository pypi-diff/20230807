# Comparing `tmp/utfuzz-0.1.5.tar.gz` & `tmp/utfuzz-0.1.5.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utfuzz-0.1.5.tar", max compression
+gzip compressed data, was "utfuzz-0.1.5.dev1.tar", max compression
```

## Comparing `utfuzz-0.1.5.tar` & `utfuzz-0.1.5.dev1.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0     2531 2023-08-07 12:11:52.214890 utfuzz-0.1.5/README.md
--rw-r--r--   0        0        0      324 2023-08-07 13:37:26.730360 utfuzz-0.1.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-08-05 12:29:28.619794 utfuzz-0.1.5/utfuzz/__init__.py
--rw-r--r--   0        0        0       37 2023-08-07 09:51:23.339177 utfuzz-0.1.5/utfuzz/__main__.py
--rw-r--r--   0        0        0        0 2023-08-06 13:33:20.961223 utfuzz-0.1.5/utfuzz/config/__init__.py
--rw-r--r--   0        0        0      779 2023-08-07 08:07:29.350724 utfuzz-0.1.5/utfuzz/config/config_manager.py
--rw-r--r--   0        0        0        0 2023-08-06 08:46:59.594235 utfuzz-0.1.5/utfuzz/exceptions/__init__.py
--rw-r--r--   0        0        0      474 2023-08-06 13:45:21.520016 utfuzz-0.1.5/utfuzz/exceptions/exceptions.py
--rw-r--r--   0        0        0        0 2023-08-06 07:39:15.312321 utfuzz-0.1.5/utfuzz/file_manager/__init__.py
--rw-r--r--   0        0        0      118 2023-08-06 18:46:12.244717 utfuzz-0.1.5/utfuzz/file_manager/directory_manager.py
--rw-r--r--   0        0        0      577 2023-08-07 07:07:53.023797 utfuzz-0.1.5/utfuzz/file_manager/file_finder.py
--rw-r--r--   0        0        0     5605 2023-08-07 13:37:21.236878 utfuzz-0.1.5/utfuzz/main.py
--rw-r--r--   0        0        0     2405 2023-08-07 12:05:04.283720 utfuzz-0.1.5/utfuzz/parser.py
--rw-r--r--   0        0        0        0 2023-08-04 15:27:45.403178 utfuzz-0.1.5/utfuzz/requirements_managers/__init__.py
--rw-r--r--   0        0        0     1462 2023-08-07 11:01:58.158057 utfuzz-0.1.5/utfuzz/requirements_managers/abc_requirements_manager.py
--rw-r--r--   0        0        0     2139 2023-08-07 13:37:21.243545 utfuzz-0.1.5/utfuzz/requirements_managers/linux_java_manager.py
--rw-r--r--   0        0        0     1420 2023-08-07 08:27:51.941523 utfuzz-0.1.5/utfuzz/requirements_managers/python_requirements_manger.py
--rw-r--r--   0        0        0      589 2023-08-07 13:37:21.210211 utfuzz-0.1.5/utfuzz/requirements_managers/windows_java_manager.py
--rwxr-xr-x   0        0        0      134 2023-08-07 11:46:25.957650 utfuzz-0.1.5/utfuzz/utbot-cli-python.jar
--rw-r--r--   0        0        0        0 2023-08-04 15:27:37.153138 utfuzz-0.1.5/utfuzz/utbot_manager/__init__.py
--rw-r--r--   0        0        0      644 2023-08-07 07:36:12.080113 utfuzz-0.1.5/utfuzz/utbot_manager/utbot_manager.py
--rw-r--r--   0        0        0     3005 1970-01-01 00:00:00.000000 utfuzz-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     2531 2023-08-07 12:11:52.214890 utfuzz-0.1.5.dev1/README.md
+-rw-r--r--   0        0        0      350 2023-08-07 15:00:10.836135 utfuzz-0.1.5.dev1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-05 12:29:28.619794 utfuzz-0.1.5.dev1/utfuzz/__init__.py
+-rw-r--r--   0        0        0       37 2023-08-07 09:51:23.339177 utfuzz-0.1.5.dev1/utfuzz/__main__.py
+-rw-r--r--   0        0        0        0 2023-08-06 13:33:20.961223 utfuzz-0.1.5.dev1/utfuzz/config/__init__.py
+-rw-r--r--   0        0        0      779 2023-08-07 08:07:29.350724 utfuzz-0.1.5.dev1/utfuzz/config/config_manager.py
+-rw-r--r--   0        0        0        0 2023-08-06 08:46:59.594235 utfuzz-0.1.5.dev1/utfuzz/exceptions/__init__.py
+-rw-r--r--   0        0        0      474 2023-08-06 13:45:21.520016 utfuzz-0.1.5.dev1/utfuzz/exceptions/exceptions.py
+-rw-r--r--   0        0        0        0 2023-08-06 07:39:15.312321 utfuzz-0.1.5.dev1/utfuzz/file_manager/__init__.py
+-rw-r--r--   0        0        0      118 2023-08-06 18:46:12.244717 utfuzz-0.1.5.dev1/utfuzz/file_manager/directory_manager.py
+-rw-r--r--   0        0        0      577 2023-08-07 07:07:53.023797 utfuzz-0.1.5.dev1/utfuzz/file_manager/file_finder.py
+-rw-r--r--   0        0        0     5644 2023-08-07 14:36:51.061105 utfuzz-0.1.5.dev1/utfuzz/main.py
+-rw-r--r--   0        0        0     2405 2023-08-07 12:05:04.283720 utfuzz-0.1.5.dev1/utfuzz/parser.py
+-rw-r--r--   0        0        0        0 2023-08-04 15:27:45.403178 utfuzz-0.1.5.dev1/utfuzz/requirements_managers/__init__.py
+-rw-r--r--   0        0        0     1462 2023-08-07 11:01:58.158057 utfuzz-0.1.5.dev1/utfuzz/requirements_managers/abc_requirements_manager.py
+-rw-r--r--   0        0        0     2139 2023-08-07 13:37:21.243545 utfuzz-0.1.5.dev1/utfuzz/requirements_managers/linux_java_manager.py
+-rw-r--r--   0        0        0     1420 2023-08-07 08:27:51.941523 utfuzz-0.1.5.dev1/utfuzz/requirements_managers/python_requirements_manger.py
+-rw-r--r--   0        0        0      589 2023-08-07 13:37:21.210211 utfuzz-0.1.5.dev1/utfuzz/requirements_managers/windows_java_manager.py
+-rwxr-xr-x   0        0        0      134 2023-08-07 11:46:25.957650 utfuzz-0.1.5.dev1/utfuzz/utbot-cli-python.jar
+-rw-r--r--   0        0        0        0 2023-08-04 15:27:37.153138 utfuzz-0.1.5.dev1/utfuzz/utbot_manager/__init__.py
+-rw-r--r--   0        0        0      682 2023-08-07 14:56:37.117909 utfuzz-0.1.5.dev1/utfuzz/utbot_manager/utbot_loader.py
+-rw-r--r--   0        0        0      644 2023-08-07 07:36:12.080113 utfuzz-0.1.5.dev1/utfuzz/utbot_manager/utbot_manager.py
+-rw-r--r--   0        0        0     3052 1970-01-01 00:00:00.000000 utfuzz-0.1.5.dev1/PKG-INFO
```

### Comparing `utfuzz-0.1.5/README.md` & `utfuzz-0.1.5.dev1/README.md`

 * *Files identical despite different names*

### Comparing `utfuzz-0.1.5/utfuzz/config/config_manager.py` & `utfuzz-0.1.5.dev1/utfuzz/config/config_manager.py`

 * *Files identical despite different names*

### Comparing `utfuzz-0.1.5/utfuzz/file_manager/file_finder.py` & `utfuzz-0.1.5.dev1/utfuzz/file_manager/file_finder.py`

 * *Files identical despite different names*

### Comparing `utfuzz-0.1.5/utfuzz/main.py` & `utfuzz-0.1.5.dev1/utfuzz/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     NotFoundRequirementsTxt, MultipleRequirementsTxt
 from utfuzz.file_manager.file_finder import find_config, get_py_files
 from utfuzz.parser import parse
 from utfuzz.requirements_managers.abc_requirements_manager import AbstractJavaRequirementsManger
 from utfuzz.requirements_managers.linux_java_manager import LinuxJavaManager
 from utfuzz.requirements_managers.python_requirements_manger import PythonRequirementsManager
 from utfuzz.requirements_managers.windows_java_manager import WindowsJavaManager
+from utfuzz.utbot_manager.utbot_loader import download_utbot
 from utfuzz.utbot_manager.utbot_manager import generate_tests
 
 
 def main():
     args = parse()
     project_dir = pathlib.Path(args.project_dir).absolute()
     output_dir = pathlib.Path(args.output_dir).absolute()
@@ -104,15 +105,16 @@
 
     if len(files_under_test) == 0:
         files_under_test = get_py_files(project_dir)
     else:
         files_under_test = [pathlib.Path(f).absolute() for f in files_under_test]
     print(f'Found {len(files_under_test)} python files to test')
 
-    jar_path = str((pathlib.Path(__file__).parent / 'utbot-cli-python.jar').absolute())
+    if
+    jar_path = str(download_utbot(project_dir).absolute())
     sys_paths.append(str(project_dir))
     sys_paths = list(set(sys_paths))
     save_config(project_dir, java, sys_paths, [str(f) for f in files_under_test], skip_regression, timeout,
                 str(output_dir))
     for f in files_under_test:
         print(f'Start testing {f}')
         test_file_name = f'test_{"_".join(f.relative_to(project_dir).parts)}'
```

### Comparing `utfuzz-0.1.5/utfuzz/parser.py` & `utfuzz-0.1.5.dev1/utfuzz/parser.py`

 * *Files identical despite different names*

### Comparing `utfuzz-0.1.5/utfuzz/requirements_managers/abc_requirements_manager.py` & `utfuzz-0.1.5.dev1/utfuzz/requirements_managers/abc_requirements_manager.py`

 * *Files identical despite different names*

### Comparing `utfuzz-0.1.5/utfuzz/requirements_managers/linux_java_manager.py` & `utfuzz-0.1.5.dev1/utfuzz/requirements_managers/linux_java_manager.py`

 * *Files identical despite different names*

### Comparing `utfuzz-0.1.5/utfuzz/requirements_managers/python_requirements_manger.py` & `utfuzz-0.1.5.dev1/utfuzz/requirements_managers/python_requirements_manger.py`

 * *Files identical despite different names*

### Comparing `utfuzz-0.1.5/utfuzz/requirements_managers/windows_java_manager.py` & `utfuzz-0.1.5.dev1/utfuzz/requirements_managers/windows_java_manager.py`

 * *Files identical despite different names*

### Comparing `utfuzz-0.1.5/utfuzz/utbot_manager/utbot_manager.py` & `utfuzz-0.1.5.dev1/utfuzz/utbot_manager/utbot_manager.py`

 * *Files identical despite different names*

### Comparing `utfuzz-0.1.5/PKG-INFO` & `utfuzz-0.1.5.dev1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: utfuzz
-Version: 0.1.5
+Version: 0.1.5.dev1
 Summary: 
 Author: Vyacheslav Tamarin
 Author-email: slavabarsuk@ya.ru
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: utbot_executor (==1.4.32)
 Requires-Dist: utbot_mypy_runner (==0.2.11)
 Description-Content-Type: text/markdown
 
 # utfuzz
 
 `utfuzz` is a Python fuzzing engine. It supports fuzzing of Python code and generation reproducing code for error and regression suites.
```

