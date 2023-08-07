# Comparing `tmp/logging_datetime-1.0.0-py3-none-any.whl.zip` & `tmp/logging_datetime-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3708 bytes, number of entries: 7
+Zip file size: 4093 bytes, number of entries: 7
 -rw-r--r--  2.0 unx       31 b- defN 22-May-24 03:28 logging_datetime/__init__.py
--rw-r--r--  2.0 unx     2824 b- defN 22-May-24 03:22 logging_datetime/logging_datetime.py
--rwxr-xr-x  2.0 unx     2824 b- defN 22-May-24 03:22 logging_datetime-1.0.0.data/scripts/logging_datetime.py
--rw-r--r--  2.0 unx      592 b- defN 22-May-24 03:28 logging_datetime-1.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-May-24 03:28 logging_datetime-1.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 22-May-24 03:28 logging_datetime-1.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      621 b- defN 22-May-24 03:28 logging_datetime-1.0.0.dist-info/RECORD
-7 files, 7001 bytes uncompressed, 2588 bytes compressed:  63.0%
+-rw-r--r--  2.0 unx     3919 b- defN 23-Aug-07 17:42 logging_datetime/logging_datetime.py
+-rwxr-xr-x  2.0 unx     3919 b- defN 23-Aug-07 17:42 logging_datetime-1.1.0.data/scripts/logging_datetime.py
+-rw-r--r--  2.0 unx      565 b- defN 23-Aug-07 18:11 logging_datetime-1.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-07 18:11 logging_datetime-1.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 23-Aug-07 18:11 logging_datetime-1.1.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      621 b- defN 23-Aug-07 18:11 logging_datetime-1.1.0.dist-info/RECORD
+7 files, 9164 bytes uncompressed, 2973 bytes compressed:  67.6%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: logging_datetime/__init__.py
 Comment: 
 
 Filename: logging_datetime/logging_datetime.py
 Comment: 
 
-Filename: logging_datetime-1.0.0.data/scripts/logging_datetime.py
+Filename: logging_datetime-1.1.0.data/scripts/logging_datetime.py
 Comment: 
 
-Filename: logging_datetime-1.0.0.dist-info/METADATA
+Filename: logging_datetime-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: logging_datetime-1.0.0.dist-info/WHEEL
+Filename: logging_datetime-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: logging_datetime-1.0.0.dist-info/top_level.txt
+Filename: logging_datetime-1.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: logging_datetime-1.0.0.dist-info/RECORD
+Filename: logging_datetime-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## logging_datetime/logging_datetime.py

```diff
@@ -1,12 +1,15 @@
 import os
 import pytz
+import shutil
 from pathlib import Path
 from datetime import datetime
 
+prev_hour = None
+prev_day = None
 
 def datetime_format():
     '''
     Extract daterime now to get year month day hour minute second and microsecond now
     '''
     datetime_now    = datetime.now(ist)
     year            = str(datetime_now.year)
@@ -22,24 +25,39 @@
     '''
     Get asctime for message log
     '''
     year, month, day, hour, minute, second, microsecond = datetime_format()
     return f'{year}-{month}-{day} {hour}:{minute}:{second},{str(microsecond)[:3]}'
 
 def get_path_log():
-        '''
-        Set path log in path logging/yaer/month/day/log_name.log
-        '''
-        year, month, day, hour, _, _, _ = datetime_format()
-        path_name = f'{dir_log}/{year}/{month}/{day}'
-        Path(path_name).mkdir(parents=True, exist_ok=True)
-        log_filename = f'logging_{hour}, {day}-{month}-{year}.log'
-        log_file_full_name = os.path.join(path_name, log_filename)
-        return log_file_full_name
-    
+    '''
+    Set path log in path logging/yaer/month/day/log_name.log
+    '''
+    year, month, day, hour, _, _, _ = datetime_format()
+    path_name = f'{dir_log}/{year}/{month}/{day}'
+    Path(path_name).mkdir(parents=True, exist_ok=True)
+    log_filename = f'logging_{hour}, {day}-{month}-{year}.log'
+    log_file_full_name = os.path.join(path_name, log_filename)
+    return log_file_full_name
+
+def get_path_log_new():
+    Path(dir_log).mkdir(parents=True, exist_ok=True)
+    log_filename = f'logging.log'
+    log_file_full_name = os.path.join(dir_log, log_filename)
+    return log_file_full_name
+
+def check_and_move(prev_hour=None):
+    year, month, day, _, _, _, _ = datetime_format()
+    path_name = f'{dir_log}/{year}/{month}/{day}'
+    Path(path_name).mkdir(parents=True, exist_ok=True)
+    log_filename = f'logging_{prev_hour}, {prev_day}-{month}-{year}.log'
+    log_file_new = os.path.join(path_name, log_filename)
+    log_file_old = os.path.join(dir_log, 'logging.log')
+    shutil.copy(log_file_old, log_file_new)
+
 class SetupLogger:
     '''
         Dinamic Logging set as datetime directory
         Args:
             directory_log(str)  : root directory log
             print_log(boolean)  : print or skip print log
     '''
@@ -62,13 +80,27 @@
     def debug(self, msg):
         self.__write_log(self, msg, level='DEBUG')
 
     def __write_log(self, message, level):
         '''
         Write text log in path log
         '''
-        path_log = get_path_log()
+        global prev_day, prev_hour
+
+        if not prev_day: prev_day = datetime_format()[2]
+        if not prev_hour: prev_hour = datetime_format()[3]
+        path_log = get_path_log_new()
         log_file = open(path_log, 'a+')
         text = f'{asctime()} | {level} : {message}'
         log_file.write(f'{text} \n')
         print(text)
-        log_file.close()
+        log_file.close()
+        
+        curr_hour = datetime_format()[3]
+        if not prev_hour == curr_hour:
+            check_and_move(prev_hour)
+            prev_hour = curr_hour
+
+        curr_day = datetime_format()[2]
+        if not prev_day == curr_day:
+            os.remove(path_log)
+            prev_day = curr_day
```

## Comparing `logging_datetime-1.0.0.dist-info/METADATA` & `logging_datetime-1.1.0.dist-info/METADATA`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 Metadata-Version: 2.1
 Name: logging-datetime
-Version: 1.0.0
+Version: 1.1.0
 Summary: Logging set as datetime directory
 Home-page: https://github.com/Alimustoofaa/logging_datetime
 Download-URL: https://github.com/Alimustoofaa/logging_datetime.git
 Author: Ali Mustofa
 Author-email: hai.alimustofa@gmail.com
 License: Apache License 2.0
 Keywords: logging,log,logging directory,logging datetime,logging datetime directory
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Description-Content-Type: text/markdown
 Requires-Dist: pytz
 Requires-Dist: pathlib
 Requires-Dist: datetime
 
-UNKNOWN
-
```

## Comparing `logging_datetime-1.0.0.dist-info/RECORD` & `logging_datetime-1.1.0.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 logging_datetime/__init__.py,sha256=kAo4caA6XWQYVU1LQ1QVdygYA9Xt140aEulCGKkys3E,31
-logging_datetime/logging_datetime.py,sha256=7B_fSs28b6pzxb3ZiVKnj3mvhBPRdd8FKNSjrLiLoDE,2824
-logging_datetime-1.0.0.data/scripts/logging_datetime.py,sha256=7B_fSs28b6pzxb3ZiVKnj3mvhBPRdd8FKNSjrLiLoDE,2824
-logging_datetime-1.0.0.dist-info/METADATA,sha256=8vBlGwoix0qNS_ERuBaXFKL_dRgG1qiUyd6coYvXZqI,592
-logging_datetime-1.0.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-logging_datetime-1.0.0.dist-info/top_level.txt,sha256=nVHt_QjbZiJXqYoRMBKSYOimX5B3FFCA3mAaoLazKdk,17
-logging_datetime-1.0.0.dist-info/RECORD,,
+logging_datetime/logging_datetime.py,sha256=9hS4T4yEAbgeJMSf2lmeXUJyIticOazOhK_IWlbLDzs,3919
+logging_datetime-1.1.0.data/scripts/logging_datetime.py,sha256=9hS4T4yEAbgeJMSf2lmeXUJyIticOazOhK_IWlbLDzs,3919
+logging_datetime-1.1.0.dist-info/METADATA,sha256=uaOKmt27BwebrlfB7a0cIoUfHGl8-qGKhu5thraBTWk,565
+logging_datetime-1.1.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+logging_datetime-1.1.0.dist-info/top_level.txt,sha256=nVHt_QjbZiJXqYoRMBKSYOimX5B3FFCA3mAaoLazKdk,17
+logging_datetime-1.1.0.dist-info/RECORD,,
```

