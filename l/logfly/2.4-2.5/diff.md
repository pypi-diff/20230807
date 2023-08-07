# Comparing `tmp/logfly-2.4.tar.gz` & `tmp/logfly-2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logfly-2.4.tar", last modified: Sun May  1 07:31:50 2022, max compression
+gzip compressed data, was "logfly-2.5.tar", last modified: Mon Aug  7 15:42:01 2023, max compression
```

## Comparing `logfly-2.4.tar` & `logfly-2.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-01 07:31:50.727488 logfly-2.4/
--rw-r--r--   0 runner    (1001) docker     (121)     1065 2022-05-01 07:31:38.000000 logfly-2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2361 2022-05-01 07:31:50.727488 logfly-2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1871 2022-05-01 07:31:38.000000 logfly-2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      103 2022-05-01 07:31:38.000000 logfly-2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-01 07:31:50.727488 logfly-2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      787 2022-05-01 07:31:38.000000 logfly-2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-01 07:31:50.723488 logfly-2.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-01 07:31:50.727488 logfly-2.4/src/logfly/
--rw-r--r--   0 runner    (1001) docker     (121)    12702 2022-05-01 07:31:38.000000 logfly-2.4/src/logfly/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-01 07:31:50.727488 logfly-2.4/src/logfly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2361 2022-05-01 07:31:50.000000 logfly-2.4/src/logfly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      233 2022-05-01 07:31:50.000000 logfly-2.4/src/logfly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-01 07:31:50.000000 logfly-2.4/src/logfly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-05-01 07:31:50.000000 logfly-2.4/src/logfly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-05-01 07:31:50.000000 logfly-2.4/src/logfly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:42:01.358252 logfly-2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-08-07 15:41:46.000000 logfly-2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-08-07 15:42:01.358252 logfly-2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-08-07 15:41:46.000000 logfly-2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-07 15:41:46.000000 logfly-2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 15:42:01.358252 logfly-2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-08-07 15:41:46.000000 logfly-2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:42:01.358252 logfly-2.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:42:01.358252 logfly-2.5/src/logfly/
+-rw-r--r--   0 runner    (1001) docker     (123)    13712 2023-08-07 15:41:46.000000 logfly-2.5/src/logfly/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:42:01.358252 logfly-2.5/src/logfly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-08-07 15:42:01.000000 logfly-2.5/src/logfly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-08-07 15:42:01.000000 logfly-2.5/src/logfly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 15:42:01.000000 logfly-2.5/src/logfly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-07 15:42:01.000000 logfly-2.5/src/logfly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-07 15:42:01.000000 logfly-2.5/src/logfly.egg-info/top_level.txt
```

### Comparing `logfly-2.4/LICENSE` & `logfly-2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `logfly-2.4/PKG-INFO` & `logfly-2.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: logfly
-Version: 2.4
+Version: 2.5
 Summary: A simple log tool by python
 Home-page: https://about.guki.me
 Author: Yuan Sui
 Author-email: orisui@icloud.com
-License: UNKNOWN
 Project-URL: Github, https://github.com/tinqlo/logfly
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -49,9 +47,7 @@
         pathorfile: ('file', 'path') choose to create file or path.  
         name: (any str) file or path name.  
         if warning is 'yes', will print warning message if file or path is exist.  
 
 #### Description  
     pathfile is the file path that you want to create, must fill with '//'  
     filenname is the file name that you want to create, must is with '*.*'  
-
-
```

### Comparing `logfly-2.4/README.md` & `logfly-2.5/README.md`

 * *Files identical despite different names*

### Comparing `logfly-2.4/setup.py` & `logfly-2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="logfly",
-    version="2.4",
+    version="2.5",
     author="Yuan Sui",
     author_email="orisui@icloud.com",
     description="A simple log tool by python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://about.guki.me",
     project_urls={
```

### Comparing `logfly-2.4/src/logfly/__init__.py` & `logfly-2.5/src/logfly/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 #####################
 # Author: Yuki Sui
-# Date: 2022-5-1
+# Date: 2023-8-7
 #####################
 
 import time
 import shutil
 import os
 from pathlib import Path
+import subprocess
+
 try:
     from colorama import init
+
     __colorama_init__ = True
 except ModuleNotFoundError:
     __colorama_init__ = False
     pass
 
 if __colorama_init__:
     init(autoreset=True)
 else:
     pass
 
-__version__ = '2.4'
+__version__ = '2.5'
 
 
 def create_or_check_file(pathorfile, name, warning='yes'):
     try:
         if pathorfile == 'file':
             if not os.path.exists(name):
                 with open(name, 'w', encoding='utf-8') as f:
@@ -168,14 +171,16 @@
                 File.write(get_time('datetime') + ' ' + '[' + str.upper(level) + ']' + ' ' + message + '\r\n')
                 File.close()
                 if hidden == 'yes':
                     LOGFILE2 = logfolder_hidden + LOGFILE_hidden
                     File = open(LOGFILE2, 'a', newline='', encoding='utf-8')
                     File.write(get_time('datetime') + ' ' + '[' + str.upper(level) + ']' + ' ' + message + '\r\n')
                     File.close()
+                elif hidden == 'no':
+                    pass
                 else:
                     mesg = str(message) + '\r\n\r\n'
                     print(mesg)
                     raise ParameterERROR('function write_log Parameter error! hidden must be "no" or "yes"! ')
             elif mode == 'new':
                 File = open(LOGFILE, 'w', newline='', encoding='utf-8')
                 File.write(get_time('datetime') + ' ' + '[' + str.upper(level) + ']' + ' ' + message + '\r\n')
@@ -255,15 +260,33 @@
 
 def mv_file(original_file_name, new_file_name, folder_name='mv_file'):
     shutil.move(original_file_name, new_file_name)
     message = 'File ' + original_file_name + ' moved to ' + new_file_name
     write_log('logfly-log', 'CLI', 'error', message, folder_name=folder_name)
 
 
-def error(exp,linenum, mode='logfly'):
+def run_cmd(cmd):
+    p = subprocess.Popen(cmd, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+    while True:
+        result = p.stdout.readline()  # 默认获取到的是二进制内容
+        if result != b'':  # 获取内容不为空时
+            try:
+                print(result.decode('gbk').strip('\r\n'))  # 处理GBK编码的输出，去掉结尾换行
+                write_log('logfly-log', 'file', 'info', message=result.decode('gbk').strip('\r\n'))
+                return result.decode('gbk').strip('\r\n')
+            except Exception as e:
+                print(e)
+                print(result.decode('utf-8').strip('\r\n'))  # 如果GBK解码失败再尝试UTF-8解码
+                write_log('logfly-log', 'file', 'info', message=result.decode('utf-8').strip('\r\n'))
+                return result.decode('utf-8').strip('\r\n')
+        else:
+            break
+
+
+def error(exp, linenum, mode='logfly'):
     if mode == 'logfly':
         logflyErrorMessage = 'ERROR occurred! at row ' + str(linenum) + '\r\n\r\n' + str(
             exp) + "\r\n\r\nplease re-check it! \r\nAnd you can see the " \
                    "manual at " \
                    "https://github.com/tinqlo/logfly "
         write_log('logfly-log', 'CLI', 'error', logflyErrorMessage)
     elif mode == 'only print':
@@ -274,8 +297,9 @@
 
 class ParameterERROR(Exception):
     def __init__(self, message):
         self.message = message
 
 
 if __name__ == '__main__':
-    write_log('logfly-log', 'CLI', 'pass', 'test', hidden='yes')
+    # write_log('logfly-log', 'CLI', 'pass', 'test', hidden='yes')
+    run_cmd("echo 111111")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `logfly-2.4/src/logfly.egg-info/PKG-INFO` & `logfly-2.5/src/logfly.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: logfly
-Version: 2.4
+Version: 2.5
 Summary: A simple log tool by python
 Home-page: https://about.guki.me
 Author: Yuan Sui
 Author-email: orisui@icloud.com
-License: UNKNOWN
 Project-URL: Github, https://github.com/tinqlo/logfly
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -49,9 +47,7 @@
         pathorfile: ('file', 'path') choose to create file or path.  
         name: (any str) file or path name.  
         if warning is 'yes', will print warning message if file or path is exist.  
 
 #### Description  
     pathfile is the file path that you want to create, must fill with '//'  
     filenname is the file name that you want to create, must is with '*.*'  
-
-
```

