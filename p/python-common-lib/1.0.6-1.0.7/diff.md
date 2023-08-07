# Comparing `tmp/python-common-lib-1.0.6.tar.gz` & `tmp/python-common-lib-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-common-lib-1.0.6.tar", max compression
+gzip compressed data, was "python-common-lib-1.0.7.tar", max compression
```

## Comparing `python-common-lib-1.0.6.tar` & `python-common-lib-1.0.7.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rwxr-xr-x   0        0        0     1286 2020-05-29 10:44:34.000000 python-common-lib-1.0.6/LICENSE
--rw-r--r--   0        0        0     1179 2021-11-26 12:11:44.755485 python-common-lib-1.0.6/README.md
--rw-r--r--   0        0        0      930 2022-12-31 09:17:52.280838 python-common-lib-1.0.6/pyproject.toml
--rw-r--r--   0        0        0     6148 2020-06-21 14:29:39.000000 python-common-lib-1.0.6/pythoncommons/.DS_Store
--rwxr-xr-x   0        0        0        0 2020-05-29 10:44:34.000000 python-common-lib-1.0.6/pythoncommons/__init__.py
--rw-r--r--   0        0        0      161 2021-12-27 15:58:47.419213 python-common-lib-1.0.6/pythoncommons/constants.py
--rw-r--r--   0        0        0     5016 2022-12-28 13:19:12.573538 python-common-lib-1.0.6/pythoncommons/date_utils.py
--rw-r--r--   0        0        0    22050 2022-09-23 10:24:12.963302 python-common-lib-1.0.6/pythoncommons/docker_wrapper.py
--rw-r--r--   0        0        0     5690 2021-12-21 17:32:19.973321 python-common-lib-1.0.6/pythoncommons/email.py
--rw-r--r--   0        0        0        0 2022-05-10 13:35:13.479682 python-common-lib-1.0.6/pythoncommons/file_parser/__init__.py
--rw-r--r--   0        0        0    11657 2022-09-22 18:23:40.332783 python-common-lib-1.0.6/pythoncommons/file_parser/input_file_parser.py
--rw-r--r--   0        0        0    16436 2022-06-13 08:21:17.182898 python-common-lib-1.0.6/pythoncommons/file_parser/parser_config_reader.py
--rw-r--r--   0        0        0    31343 2022-12-28 13:18:36.083426 python-common-lib-1.0.6/pythoncommons/file_utils.py
--rw-r--r--   0        0        0      174 2021-12-27 16:16:25.891167 python-common-lib-1.0.6/pythoncommons/git_constants.py
--rw-r--r--   0        0        0      911 2020-09-21 10:23:14.000000 python-common-lib-1.0.6/pythoncommons/git_utils.py
--rw-r--r--   0        0        0    27212 2022-07-03 12:16:06.621839 python-common-lib-1.0.6/pythoncommons/git_wrapper.py
--rw-r--r--   0        0        0     6762 2022-11-11 16:01:48.487548 python-common-lib-1.0.6/pythoncommons/github_utils.py
--rw-r--r--   0        0        0     2454 2021-05-08 22:03:14.065919 python-common-lib-1.0.6/pythoncommons/html_utils.py
--rw-r--r--   0        0        0     2579 2022-01-24 23:31:03.430700 python-common-lib-1.0.6/pythoncommons/jira_utils.py
--rw-r--r--   0        0        0    12862 2022-06-21 17:07:50.932648 python-common-lib-1.0.6/pythoncommons/jira_wrapper.py
--rw-r--r--   0        0        0    26837 2022-12-30 20:49:27.092488 python-common-lib-1.0.6/pythoncommons/logging_setup.py
--rw-r--r--   0        0        0     5637 2021-11-30 17:22:23.398961 python-common-lib-1.0.6/pythoncommons/logging_utils.py
--rw-r--r--   0        0        0     1730 2021-11-20 17:01:58.936220 python-common-lib-1.0.6/pythoncommons/network_utils.py
--rw-r--r--   0        0        0     4590 2022-05-19 08:01:29.115530 python-common-lib-1.0.6/pythoncommons/object_utils.py
--rw-r--r--   0        0        0     3419 2022-01-21 14:42:03.823316 python-common-lib-1.0.6/pythoncommons/os_utils.py
--rw-r--r--   0        0        0     3377 2020-09-20 10:12:45.000000 python-common-lib-1.0.6/pythoncommons/patch_utils.py
--rw-r--r--   0        0        0    10060 2021-12-03 00:10:16.008057 python-common-lib-1.0.6/pythoncommons/process.py
--rw-r--r--   0        0        0    27336 2022-09-22 18:23:28.614553 python-common-lib-1.0.6/pythoncommons/project_utils.py
--rw-r--r--   0        0        0      232 2020-09-25 08:08:52.000000 python-common-lib-1.0.6/pythoncommons/random_utils.py
--rw-r--r--   0        0        0    10189 2022-02-24 15:05:50.284611 python-common-lib-1.0.6/pythoncommons/result_printer.py
--rw-r--r--   0        0        0     9016 2022-12-28 21:28:12.411583 python-common-lib-1.0.6/pythoncommons/string_utils.py
--rw-r--r--   0        0        0      500 2021-11-01 21:09:43.937682 python-common-lib-1.0.6/pythoncommons/test-scripts/commands/testcommand/dummy_test_command.py
--rw-r--r--   0        0        0      810 2022-01-25 13:28:52.846631 python-common-lib-1.0.6/pythoncommons/test-scripts/hello_world_simple.py
--rw-r--r--   0        0        0     1259 2022-01-25 13:28:52.863379 python-common-lib-1.0.6/pythoncommons/test-scripts/test_project.py
--rw-r--r--   0        0        0      212 2022-01-09 20:09:06.364387 python-common-lib-1.0.6/pythoncommons/test_utils.py
--rw-r--r--   0        0        0        0 2021-02-15 18:57:37.000000 python-common-lib-1.0.6/pythoncommons/tests/__init__.py
--rw-r--r--   0        0        0     1951 2021-09-07 15:11:18.542115 python-common-lib-1.0.6/pythoncommons/tests/test_file_utils.py
--rw-r--r--   0        0        0     3192 2021-11-03 13:30:31.511381 python-common-lib-1.0.6/pythoncommons/tests/test_jira_utils.py
--rw-r--r--   0        0        0     2222 2021-04-24 14:05:26.247162 python-common-lib-1.0.6/pythoncommons/tests/test_logging_utils.py
--rw-r--r--   0        0        0     4895 2022-01-04 13:09:38.823159 python-common-lib-1.0.6/pythoncommons/tests/test_project_utils.py
--rw-r--r--   0        0        0     1412 2022-12-27 22:56:48.743486 python-common-lib-1.0.6/pythoncommons/url_utils.py
--rw-r--r--   0        0        0     8971 2022-01-24 17:02:16.084620 python-common-lib-1.0.6/pythoncommons/zip_utils.py
--rw-r--r--   0        0        0     2248 1970-01-01 00:00:00.000000 python-common-lib-1.0.6/setup.py
--rw-r--r--   0        0        0     2066 1970-01-01 00:00:00.000000 python-common-lib-1.0.6/PKG-INFO
+-rwxr-xr-x   0        0        0     1286 2020-05-29 10:44:34.000000 python-common-lib-1.0.7/LICENSE
+-rw-r--r--   0        0        0     1179 2021-11-26 12:11:44.755485 python-common-lib-1.0.7/README.md
+-rw-r--r--   0        0        0      930 2023-08-07 00:25:17.366004 python-common-lib-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0     6148 2020-06-21 14:29:39.000000 python-common-lib-1.0.7/pythoncommons/.DS_Store
+-rwxr-xr-x   0        0        0        0 2020-05-29 10:44:34.000000 python-common-lib-1.0.7/pythoncommons/__init__.py
+-rw-r--r--   0        0        0      161 2021-12-27 15:58:47.419213 python-common-lib-1.0.7/pythoncommons/constants.py
+-rw-r--r--   0        0        0     5207 2023-01-14 23:12:04.314501 python-common-lib-1.0.7/pythoncommons/date_utils.py
+-rw-r--r--   0        0        0    22050 2022-09-23 10:24:12.963302 python-common-lib-1.0.7/pythoncommons/docker_wrapper.py
+-rw-r--r--   0        0        0     6588 2023-01-23 17:25:03.552887 python-common-lib-1.0.7/pythoncommons/email.py
+-rw-r--r--   0        0        0        0 2022-05-10 13:35:13.479682 python-common-lib-1.0.7/pythoncommons/file_parser/__init__.py
+-rw-r--r--   0        0        0    11657 2022-09-22 18:23:40.332783 python-common-lib-1.0.7/pythoncommons/file_parser/input_file_parser.py
+-rw-r--r--   0        0        0    16436 2022-06-13 08:21:17.182898 python-common-lib-1.0.7/pythoncommons/file_parser/parser_config_reader.py
+-rw-r--r--   0        0        0    33413 2023-08-07 00:24:50.828729 python-common-lib-1.0.7/pythoncommons/file_utils.py
+-rw-r--r--   0        0        0      174 2021-12-27 16:16:25.891167 python-common-lib-1.0.7/pythoncommons/git_constants.py
+-rw-r--r--   0        0        0      911 2020-09-21 10:23:14.000000 python-common-lib-1.0.7/pythoncommons/git_utils.py
+-rw-r--r--   0        0        0    27212 2022-07-03 12:16:06.621839 python-common-lib-1.0.7/pythoncommons/git_wrapper.py
+-rw-r--r--   0        0        0     6762 2022-11-11 16:01:48.487548 python-common-lib-1.0.7/pythoncommons/github_utils.py
+-rw-r--r--   0        0        0     2454 2021-05-08 22:03:14.065919 python-common-lib-1.0.7/pythoncommons/html_utils.py
+-rw-r--r--   0        0        0     2579 2022-01-24 23:31:03.430700 python-common-lib-1.0.7/pythoncommons/jira_utils.py
+-rw-r--r--   0        0        0    12862 2022-06-21 17:07:50.932648 python-common-lib-1.0.7/pythoncommons/jira_wrapper.py
+-rw-r--r--   0        0        0    26837 2022-12-30 20:49:27.092488 python-common-lib-1.0.7/pythoncommons/logging_setup.py
+-rw-r--r--   0        0        0     5637 2021-11-30 17:22:23.398961 python-common-lib-1.0.7/pythoncommons/logging_utils.py
+-rw-r--r--   0        0        0     1730 2021-11-20 17:01:58.936220 python-common-lib-1.0.7/pythoncommons/network_utils.py
+-rw-r--r--   0        0        0     4788 2023-06-02 15:29:35.865459 python-common-lib-1.0.7/pythoncommons/object_utils.py
+-rw-r--r--   0        0        0     3419 2022-01-21 14:42:03.823316 python-common-lib-1.0.7/pythoncommons/os_utils.py
+-rw-r--r--   0        0        0     3377 2020-09-20 10:12:45.000000 python-common-lib-1.0.7/pythoncommons/patch_utils.py
+-rw-r--r--   0        0        0    10060 2021-12-03 00:10:16.008057 python-common-lib-1.0.7/pythoncommons/process.py
+-rw-r--r--   0        0        0    27336 2022-09-22 18:23:28.614553 python-common-lib-1.0.7/pythoncommons/project_utils.py
+-rw-r--r--   0        0        0      232 2020-09-25 08:08:52.000000 python-common-lib-1.0.7/pythoncommons/random_utils.py
+-rw-r--r--   0        0        0    10189 2022-02-24 15:05:50.284611 python-common-lib-1.0.7/pythoncommons/result_printer.py
+-rw-r--r--   0        0        0     9751 2023-06-27 23:34:17.388893 python-common-lib-1.0.7/pythoncommons/string_utils.py
+-rw-r--r--   0        0        0      500 2021-11-01 21:09:43.937682 python-common-lib-1.0.7/pythoncommons/test-scripts/commands/testcommand/dummy_test_command.py
+-rw-r--r--   0        0        0      810 2022-01-25 13:28:52.846631 python-common-lib-1.0.7/pythoncommons/test-scripts/hello_world_simple.py
+-rw-r--r--   0        0        0     1259 2022-01-25 13:28:52.863379 python-common-lib-1.0.7/pythoncommons/test-scripts/test_project.py
+-rw-r--r--   0        0        0      212 2022-01-09 20:09:06.364387 python-common-lib-1.0.7/pythoncommons/test_utils.py
+-rw-r--r--   0        0        0        0 2021-02-15 18:57:37.000000 python-common-lib-1.0.7/pythoncommons/tests/__init__.py
+-rw-r--r--   0        0        0     1951 2021-09-07 15:11:18.542115 python-common-lib-1.0.7/pythoncommons/tests/test_file_utils.py
+-rw-r--r--   0        0        0     3192 2021-11-03 13:30:31.511381 python-common-lib-1.0.7/pythoncommons/tests/test_jira_utils.py
+-rw-r--r--   0        0        0     2222 2021-04-24 14:05:26.247162 python-common-lib-1.0.7/pythoncommons/tests/test_logging_utils.py
+-rw-r--r--   0        0        0     4895 2022-01-04 13:09:38.823159 python-common-lib-1.0.7/pythoncommons/tests/test_project_utils.py
+-rw-r--r--   0        0        0     1885 2023-01-15 17:31:28.933658 python-common-lib-1.0.7/pythoncommons/url_utils.py
+-rw-r--r--   0        0        0     8971 2022-01-24 17:02:16.084620 python-common-lib-1.0.7/pythoncommons/zip_utils.py
+-rw-r--r--   0        0        0     2248 1970-01-01 00:00:00.000000 python-common-lib-1.0.7/setup.py
+-rw-r--r--   0        0        0     2066 1970-01-01 00:00:00.000000 python-common-lib-1.0.7/PKG-INFO
```

### Comparing `python-common-lib-1.0.6/LICENSE` & `python-common-lib-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `python-common-lib-1.0.6/README.md` & `python-common-lib-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `python-common-lib-1.0.6/pyproject.toml` & `python-common-lib-1.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
   | build
   | dist
 )/
 '''
 
 [tool.poetry]
 name = "python-common-lib"
-version = "1.0.6"
+version = "1.0.7"
 description = ""
 authors = ["Szilard Nemeth <szilard.nemeth88@gmail.com>"]
 readme = "README.md"
 packages = [{include = "pythoncommons"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `python-common-lib-1.0.6/pythoncommons/.DS_Store` & `python-common-lib-1.0.7/pythoncommons/.DS_Store`

 * *Files identical despite different names*

### Comparing `python-common-lib-1.0.6/pythoncommons/date_utils.py` & `python-common-lib-1.0.7/pythoncommons/date_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import logging
 import time
 from typing import List
 
 LOG = logging.getLogger(__name__)
 
 DATEFORMAT_DASH_COLON = "%Y-%m-%d %H:%M:%S"
+DATEFORMAT_GOOGLE_DRIVE = "%Y-%m-%dT%H:%M:%S.%f%z"
 
 
 # https://medium.com/pythonhive/python-decorator-to-measure-the-execution-time-of-methods-fa04cb6bb36d
 def timeit(method):
     def timed(*args, **kw):
         def print_time(method_name, time_value):
             pretty_time = TimeUtilities.prettify_time(time_value)
@@ -114,14 +115,18 @@
         return datetime.datetime.strptime(date_string, fmt)
 
     @classmethod
     def convert_datetime_to_str(cls, datetime_obj, fmt):
         return datetime_obj.strftime(fmt)
 
     @classmethod
+    def convert_to_datetime_from_isoformat(cls, date_string):
+        return datetime.datetime.fromisoformat(date_string)
+
+    @classmethod
     def get_datetime(cls, y, m, d):
         return datetime.datetime(y, m, d)
 
     @classmethod
     def get_datetime_from_date(cls, date_obj, min_time=False, max_time=False):
         if not min_time and not max_time:
             raise ValueError("Either min_time or max_time had set to True!")
```

### Comparing `python-common-lib-1.0.6/pythoncommons/docker_wrapper.py` & `python-common-lib-1.0.7/pythoncommons/docker_wrapper.py`

 * *Files identical despite different names*

### Comparing `python-common-lib-1.0.6/pythoncommons/email.py` & `python-common-lib-1.0.7/pythoncommons/email.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,16 +27,19 @@
     def __init__(self, smtp_server: str, smtp_port: int, email_account: EmailAccount):
         self.smtp_server = smtp_server
         self.smtp_port = smtp_port
         self.email_account = email_account
 
 
 class EmailService:
-    def __init__(self, email_config: EmailConfig):
+    def __init__(self, email_config: EmailConfig, batch_mode: bool = False):
         self.conf = email_config
+        self.batch_mode = batch_mode
+        self.logged_in = False
+        self.conn = None
 
     def send_mail(
         self,
         sender: str,
         subject: str,
         body: str,
         recipients: List[str],
@@ -104,42 +107,66 @@
         recipients,
         recipients_comma_separated,
         sender,
         with_retries: bool = True,
         retry_count: int = 3,
         log_exception_when_retried: bool = True,
     ):
-        server = smtplib.SMTP_SSL(self.conf.smtp_server, self.conf.smtp_port)
+        if not self.is_connected():
+            self.conn = smtplib.SMTP_SSL(self.conf.smtp_server, self.conf.smtp_port)
+            self.logged_in = False
+
         if with_retries:
-            all_try_count: int = retry_count + 1
+            attempts_count: int = retry_count + 1
         else:
-            all_try_count: int = 1
+            attempts_count: int = 1
 
-        for i in range(all_try_count):
+        for i in range(attempts_count):
             attempt = i + 1
             LOG.info(
                 "[Attempt: %d / %d] Sending mail to recipients: %s with subject '%s'",
                 attempt,
-                all_try_count,
+                attempts_count,
                 recipients_comma_separated,
                 email_msg["Subject"],
             )
             try:
-                server.ehlo()
-                server.login(self.conf.email_account.user, self.conf.email_account.password)
-                server.sendmail(sender, recipients, email_msg.as_string())
-                server.quit()
+                if not self.logged_in or not self.batch_mode:
+                    self.conn.ehlo()
+                    LOG.debug("SMPTP login")
+                    self.conn.login(self.conf.email_account.user, self.conf.email_account.password)
+                    self.logged_in = True
+
+                self.conn.sendmail(sender, recipients, email_msg.as_string())
+
+                if not self.batch_mode:
+                    self.conn.quit()
                 return
             except smtplib.SMTPServerDisconnected as e:
-                if attempt == all_try_count:
+                # Try to reconnect
+                self._reconnect()
+                if attempt == attempts_count:
                     # Raise if we reached max retries or we just tried once without retries and it failed
                     raise e
                 elif log_exception_when_retried:
                     LOG.exception("Failed to send email.", exc_info=True)
 
+    def _reconnect(self):
+        code, msg = self.conn.connect(self.conf.smtp_server, self.conf.smtp_port)
+        LOG.info("Code: %s, msg: %s", code, msg)
+
+    def is_connected(self):
+        if not self.conn:
+            return False
+        try:
+            status = self.conn.noop()[0]
+        except smtplib.SMTPServerDisconnected:
+            status = -1
+        return True if status == 250 else False
+
     @staticmethod
     def _create_attachment(file_path: str, attachment_name: str = None):
         msg = MIMEBase("application", "zip")
         file = open(file_path, "rb")
         msg.set_payload(file.read())
         encoders.encode_base64(msg)
```

### Comparing `python-common-lib-1.0.6/pythoncommons/file_parser/input_file_parser.py` & `python-common-lib-1.0.7/pythoncommons/file_parser/input_file_parser.py`

 * *Files identical despite different names*

### Comparing `python-common-lib-1.0.6/pythoncommons/file_parser/parser_config_reader.py` & `python-common-lib-1.0.7/pythoncommons/file_parser/parser_config_reader.py`

 * *Files identical despite different names*

### Comparing `python-common-lib-1.0.6/pythoncommons/file_utils.py` & `python-common-lib-1.0.7/pythoncommons/file_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import errno
 import fnmatch
 import hashlib
 import logging
 import os
+import platform
 import re
 import shutil
 import tempfile
 from datetime import datetime
 from enum import Enum
 from pathlib import Path
-from typing import List, Dict, Any
+from typing import List, Dict, Any, Tuple, Iterable
 from stat import ST_SIZE
 from stat import ST_MTIME
 
 import humanize
 
 from pythoncommons.date_utils import timeit
 
@@ -131,14 +132,15 @@
             cls._smartlog(f"Processing root: {root}, dirs: {dirs}")
             dirs[:] = cls._handle_dir_exclusions(dirs, exclude_dirs)
             if find_type == FindResultType.FILES:
                 result_files.extend(cls._find_files(root, files, find_criteria))
             elif find_type == FindResultType.DIRS:
                 result_files.extend(cls._find_dirs(root, dirs, find_criteria))
             if single_level:
+                # TODO bug: if single level = True, ensure_number_of_results validation won't be executed
                 return result_files
         cls.debug = cls.old_debug
 
         if ensure_number_of_results:
             if len(result_files) != ensure_number_of_results:
                 raise ValueError(
                     "Number of results is not equal to expected result size! Expected: {}, Actual: {}".format(
@@ -544,14 +546,33 @@
             for attr_idx in stat_attrs_idx:
                 file_stats = os.stat(file_path)
                 tup = tup + (file_stats[attr_idx],)
             result.append(tup)
         return result
 
     @classmethod
+    def get_creation_time(cls, file_path):
+        """
+        Try to get the date that a file was created, falling back to when it was
+        last modified if that isn't possible.
+        See http://stackoverflow.com/a/39501288/1709587 for explanation.
+        Answer: https://stackoverflow.com/a/39501288/1106893
+        """
+        if platform.system() == "Windows":
+            return os.path.getctime(file_path)
+        else:
+            stat = os.stat(file_path)
+            try:
+                return stat.st_birthtime
+            except AttributeError:
+                # We're probably on Linux. No easy way to get creation dates here,
+                # so we'll settle for when its content was last modified.
+                return stat.st_mtime
+
+    @classmethod
     def get_file_sizes_with_mod_dates_in_dir(cls, dir):
         return cls._get_files_with_attrs_in_dir(dir, [ST_SIZE, ST_MTIME])
 
     @classmethod
     def get_file_extension(cls, filename):
         filename, ext = os.path.splitext(filename)
         ext = ext.replace(".", "")
@@ -835,71 +856,98 @@
     def get_temp_file_name(cls, prefix=None):
         kwargs = {"delete": False}
         if prefix:
             kwargs["prefix"] = prefix
         tmp = tempfile.NamedTemporaryFile(**kwargs)
         return tmp.name
 
+    @classmethod
+    def write_bytesio_to_file(cls, filename, bytesio):
+        """
+        Write the contents of the given BytesIO to a file.
+        Creates the file or overwrites the file if it does
+        not exist yet.
+        """
+        with open(filename, "wb") as outfile:
+            # Copy the BytesIO stream to the output file
+            outfile.write(bytesio.getbuffer())
+
 
 class JsonFileUtils:
     @classmethod
     @timeit
     def write_data_to_file_as_json(cls, path, data, pretty=False):
         import json
 
         dirname = os.path.dirname(path)
         if not os.path.exists(dirname):
             os.makedirs(dirname)
         if not os.path.isdir(dirname):
             raise ValueError("Should have a dir in path, not a file: {}".format(dirname))
 
+        bytes_written = -1
         LOG.trace("Starting to write to file: %s", path)
         with open(path, "w") as file:
             kwargs = {"sort_keys": True}
             if pretty:
                 kwargs["indent"] = 4
             json.dump(data, file, **kwargs)
+            bytes_written = file.tell()
         LOG.trace("Finished writing to file: %s", path)
+        return bytes_written
 
     @classmethod
     def load_data_from_json_file(
         cls, file, create_if_not_exists=False, swallow_file_not_found=False, swallow_value_error=False
-    ):
+    ) -> Tuple[Any, int]:
         import json
 
         try:
             with open(file, "r") as f:
-                return json.load(f)
+                data = json.load(f)
+                bytes_read = f.tell()
+                return data, bytes_read
         except FileNotFoundError as e:
             LOG.exception("Error while opening file: %s", file)
             if create_if_not_exists:
                 LOG.info("Creating new empty file: %s", file)
                 FileUtils.create_new_empty_file(file)
             if swallow_file_not_found:
-                return None
+                return None, 0
             raise e
         except ValueError as e:
             LOG.exception("Error while reading file: %s", file)
             if swallow_value_error:
-                return None
+                return None, 0
             raise e
 
 
 class CsvFileUtils:
     @classmethod
-    def append_row_to_csv_file(cls, path, data, header=None):
-        parent_dir = FileUtils.get_parent_dir_name(path)
-        if not FileUtils.is_dir(parent_dir, throw_ex=False):
-            FileUtils.create_new_dir(parent_dir)
-
+    def append_rows_to_csv_file(cls, file_path, data: List[Iterable[Any]], header=None):
+        import csv
+        # Validation
         if not isinstance(data, list):
             raise ValueError("Expected list of data for CSV row!")
+        if len(data) > 0 and not all([isinstance(item, str) for item in data]):
+            raise ValueError("Expected list of str items for CSV row!")
 
-        new_file = True if not os.path.exists(path) else False
-
-        with open(path, "a", newline="") as csvfile:
-            import csv
-
+        new_file = cls._ensure_parent_dir_exists(file_path)
+        with open(file_path, "a", newline="") as csvfile:
             csv_writer = csv.writer(csvfile, delimiter=";", quotechar="|", quoting=csv.QUOTE_MINIMAL)
             if new_file and header:
                 csv_writer.writerow(header)
-            csv_writer.writerow(data)
+            for row in data:
+                csv_writer.writerow(row)
+
+    @classmethod
+    def append_row_to_csv_file(cls, file_path, data: List[str], header=None):
+        data = [data]
+        CsvFileUtils.append_rows_to_csv_file(file_path, data, header=header)
+
+    @classmethod
+    def _ensure_parent_dir_exists(cls, path):
+        parent_dir = FileUtils.get_parent_dir_name(path)
+        if not FileUtils.is_dir(parent_dir, throw_ex=False):
+            FileUtils.create_new_dir(parent_dir)
+        new_file = False if os.path.exists(path) else True
+        return new_file
```

### Comparing `python-common-lib-1.0.6/pythoncommons/git_utils.py` & `python-common-lib-1.0.7/pythoncommons/git_utils.py`

 * *Files identical despite different names*

### Comparing `python-common-lib-1.0.6/pythoncommons/git_wrapper.py` & `python-common-lib-1.0.7/pythoncommons/git_wrapper.py`

 * *Files identical despite different names*

### Comparing `python-common-lib-1.0.6/pythoncommons/github_utils.py` & `python-common-lib-1.0.7/pythoncommons/github_utils.py`

 * *Files identical despite different names*

### Comparing `python-common-lib-1.0.6/pythoncommons/html_utils.py` & `python-common-lib-1.0.7/pythoncommons/html_utils.py`

 * *Files identical despite different names*

### Comparing `python-common-lib-1.0.6/pythoncommons/jira_utils.py` & `python-common-lib-1.0.7/pythoncommons/jira_utils.py`

 * *Files identical despite different names*

### Comparing `python-common-lib-1.0.6/pythoncommons/jira_wrapper.py` & `python-common-lib-1.0.7/pythoncommons/jira_wrapper.py`

 * *Files identical despite different names*

### Comparing `python-common-lib-1.0.6/pythoncommons/logging_setup.py` & `python-common-lib-1.0.7/pythoncommons/logging_setup.py`

 * *Files identical despite different names*

### Comparing `python-common-lib-1.0.6/pythoncommons/logging_utils.py` & `python-common-lib-1.0.7/pythoncommons/logging_utils.py`

 * *Files identical despite different names*

### Comparing `python-common-lib-1.0.6/pythoncommons/network_utils.py` & `python-common-lib-1.0.7/pythoncommons/network_utils.py`

 * *Files identical despite different names*

### Comparing `python-common-lib-1.0.6/pythoncommons/object_utils.py` & `python-common-lib-1.0.7/pythoncommons/object_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,14 +124,19 @@
 
     @staticmethod
     def pairwise(iterable):
         "s -> (s0, s1), (s2, s3), (s4, s5), ..."
         a = iter(iterable)
         return zip(a, a)
 
+    @staticmethod
+    def merge_dicts_sum_values(d1: Dict[Any, int], d2: Dict[Any, int]):
+        merged = {key: d1.get(key, 0) + d2.get(key, 0) for key in set(d1) | set(d2)}
+        return merged
+
 
 class PickleUtils:
     @staticmethod
     def dump(data, file):
         with open(file, "wb") as f:
             pickle.dump(data, f, pickle.HIGHEST_PROTOCOL)
```

### Comparing `python-common-lib-1.0.6/pythoncommons/os_utils.py` & `python-common-lib-1.0.7/pythoncommons/os_utils.py`

 * *Files identical despite different names*

### Comparing `python-common-lib-1.0.6/pythoncommons/patch_utils.py` & `python-common-lib-1.0.7/pythoncommons/patch_utils.py`

 * *Files identical despite different names*

### Comparing `python-common-lib-1.0.6/pythoncommons/process.py` & `python-common-lib-1.0.7/pythoncommons/process.py`

 * *Files identical despite different names*

### Comparing `python-common-lib-1.0.6/pythoncommons/project_utils.py` & `python-common-lib-1.0.7/pythoncommons/project_utils.py`

 * *Files identical despite different names*

### Comparing `python-common-lib-1.0.6/pythoncommons/result_printer.py` & `python-common-lib-1.0.7/pythoncommons/result_printer.py`

 * *Files identical despite different names*

### Comparing `python-common-lib-1.0.6/pythoncommons/string_utils.py` & `python-common-lib-1.0.7/pythoncommons/string_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -265,14 +265,39 @@
         while True:
             start = s.find(expr, start)
             if start == -1:
                 return
             yield start
             start += len(expr)  # use start += 1 to find overlapping matches
 
+    @staticmethod
+    def format_bytes(size):
+        # https://stackoverflow.com/a/49361727/1106893
+        # 2**10 = 1024
+        power = 2**10
+        n = 0
+        power_labels = {0: "", 1: "kilo", 2: "mega", 3: "giga", 4: "tera"}
+        while size > power:
+            size /= power
+            n += 1
+        return size, power_labels[n] + "bytes"
+
+    @staticmethod
+    def format_bytes_as_str(bytes):
+        tup = StringUtils.format_bytes(bytes)
+        return " ".join([str(s) for s in tup])
+
+    @staticmethod
+    def md5_hash(input):
+        # https://stackoverflow.com/a/2511075/1106893
+        import hashlib
+
+        encoded_input = input.encode("utf-8")
+        return int(hashlib.md5(encoded_input).hexdigest(), 16)
+
 
 class RegexUtils:
     @staticmethod
     def filter_list_by_regex(list, regex):
         p = re.compile(regex)
         return [s for s in list if p.match(s)]
```

### Comparing `python-common-lib-1.0.6/pythoncommons/test-scripts/hello_world_simple.py` & `python-common-lib-1.0.7/pythoncommons/test-scripts/hello_world_simple.py`

 * *Files identical despite different names*

### Comparing `python-common-lib-1.0.6/pythoncommons/test-scripts/test_project.py` & `python-common-lib-1.0.7/pythoncommons/test-scripts/test_project.py`

 * *Files identical despite different names*

### Comparing `python-common-lib-1.0.6/pythoncommons/tests/test_file_utils.py` & `python-common-lib-1.0.7/pythoncommons/tests/test_file_utils.py`

 * *Files identical despite different names*

### Comparing `python-common-lib-1.0.6/pythoncommons/tests/test_jira_utils.py` & `python-common-lib-1.0.7/pythoncommons/tests/test_jira_utils.py`

 * *Files identical despite different names*

### Comparing `python-common-lib-1.0.6/pythoncommons/tests/test_logging_utils.py` & `python-common-lib-1.0.7/pythoncommons/tests/test_logging_utils.py`

 * *Files identical despite different names*

### Comparing `python-common-lib-1.0.6/pythoncommons/tests/test_project_utils.py` & `python-common-lib-1.0.7/pythoncommons/tests/test_project_utils.py`

 * *Files identical despite different names*

### Comparing `python-common-lib-1.0.6/pythoncommons/zip_utils.py` & `python-common-lib-1.0.7/pythoncommons/zip_utils.py`

 * *Files identical despite different names*

### Comparing `python-common-lib-1.0.6/setup.py` & `python-common-lib-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
  'pytest>=6.2.3,<6.3.0',
  'requests>=2.28.1,<3.0.0',
  'sh>=1.14.1,<1.15.0',
  'tabulate>=0.8.10,<0.9.0']
 
 setup_kwargs = {
     'name': 'python-common-lib',
-    'version': '1.0.6',
+    'version': '1.0.7',
     'description': '',
     'long_description': '# python-commons\n\nRun ./setup.sh to set up git pre/post push hook scripts.\nThen, a similar script loaded to the environment will execute the pre/post push hook scripts: \nhttps://stackoverflow.com/a/3812238/1106893\n\nFor example loading this script and defining an alias like this will do the trick:\n`alias gpwh="git-push-with-hooks.sh"`\n\n\n## Setup of precommit\n\nConfigure precommit as described in this blogpost: https://ljvmiranda921.github.io/notebook/2018/06/21/precommits-using-black-and-flake8/\nCommands:\n1. Install precommit: `pip install pre-commit`\n2. Make sure to add pre-commit to your path. For example, on a Mac system, pre-commit is installed here: \n   `$HOME/Library/Python/3.8/bin/pre-commit`.\n2. Execute `pre-commit install` to install git hooks in your `.git/` directory.\n\n## Troubleshooting\n\n### Installation issues\nIn case you\'re facing a similar issue:\n```\nAn error has occurred: InvalidManifestError: \n=====> /<userhome>/.cache/pre-commit/repoBP08UH/.pre-commit-hooks.yaml does not exist\nCheck the log at /<userhome>/.cache/pre-commit/pre-commit.log\n```\n, please run: `pre-commit autoupdate`\nMore info here: https://github.com/pre-commit/pre-commit/issues/577',
     'author': 'Szilard Nemeth',
     'author_email': 'szilard.nemeth88@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `python-common-lib-1.0.6/PKG-INFO` & `python-common-lib-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-common-lib
-Version: 1.0.6
+Version: 1.0.7
 Summary: 
 Author: Szilard Nemeth
 Author-email: szilard.nemeth88@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

