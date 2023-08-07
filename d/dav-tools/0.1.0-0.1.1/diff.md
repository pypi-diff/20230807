# Comparing `tmp/dav_tools-0.1.0.tar.gz` & `tmp/dav_tools-0.1.1.tar.gz`

## Comparing `dav_tools-0.1.0.tar` & `dav_tools-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,23 @@
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 dav_tools-0.1.0/.readthedocs.yaml
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 dav_tools-0.1.0/Makefile
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 dav_tools-0.1.0/requirements.txt
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 dav_tools-0.1.0/docs/Makefile
--rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 dav_tools-0.1.0/docs/conf.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 dav_tools-0.1.0/docs/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 dav_tools-0.1.0/docs/make.bat
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 dav_tools-0.1.0/docs/requirements.txt
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 dav_tools-0.1.0/src/dav_tools/__init__.py
--rw-r--r--   0        0        0     5415 2020-02-02 00:00:00.000000 dav_tools-0.1.0/src/dav_tools/_arg_parser.py
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 dav_tools-0.1.0/src/dav_tools/_text_format.py
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 dav_tools-0.1.0/src/dav_tools/commands.py
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 dav_tools-0.1.0/src/dav_tools/devtools.py
--rw-r--r--   0        0        0     7896 2020-02-02 00:00:00.000000 dav_tools-0.1.0/src/dav_tools/messages.py
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 dav_tools-0.1.0/src/dav_tools/requirements.py
--rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 dav_tools-0.1.0/src/dav_tools/text_color.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 dav_tools-0.1.0/.gitignore
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 dav_tools-0.1.0/LICENSE
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 dav_tools-0.1.0/README.md
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 dav_tools-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 dav_tools-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 dav_tools-0.1.1/.readthedocs.yaml
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 dav_tools-0.1.1/Makefile
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 dav_tools-0.1.1/requirements.txt
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 dav_tools-0.1.1/docs/Makefile
+-rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 dav_tools-0.1.1/docs/conf.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 dav_tools-0.1.1/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 dav_tools-0.1.1/docs/make.bat
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 dav_tools-0.1.1/docs/requirements.txt
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 dav_tools-0.1.1/src/dav_tools/__init__.py
+-rw-r--r--   0        0        0     5415 2020-02-02 00:00:00.000000 dav_tools-0.1.1/src/dav_tools/_arg_parser.py
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 dav_tools-0.1.1/src/dav_tools/_text_format.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 dav_tools-0.1.1/src/dav_tools/commands.py
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 dav_tools-0.1.1/src/dav_tools/devtools.py
+-rw-r--r--   0        0        0     7900 2020-02-02 00:00:00.000000 dav_tools-0.1.1/src/dav_tools/messages.py
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 dav_tools-0.1.1/src/dav_tools/requirements.py
+-rw-r--r--   0        0        0     2389 2020-02-02 00:00:00.000000 dav_tools-0.1.1/src/dav_tools/text_color.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dav_tools-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 dav_tools-0.1.1/tests/test_messages.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 dav_tools-0.1.1/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 dav_tools-0.1.1/LICENSE
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 dav_tools-0.1.1/README.md
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 dav_tools-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 dav_tools-0.1.1/PKG-INFO
```

### Comparing `dav_tools-0.1.0/.readthedocs.yaml` & `dav_tools-0.1.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `dav_tools-0.1.0/docs/Makefile` & `dav_tools-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dav_tools-0.1.0/docs/conf.py` & `dav_tools-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dav_tools-0.1.0/docs/index.rst` & `dav_tools-0.1.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `dav_tools-0.1.0/docs/make.bat` & `dav_tools-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dav_tools-0.1.0/src/dav_tools/_arg_parser.py` & `dav_tools-0.1.1/src/dav_tools/_arg_parser.py`

 * *Files identical despite different names*

### Comparing `dav_tools-0.1.0/src/dav_tools/_text_format.py` & `dav_tools-0.1.1/src/dav_tools/_text_format.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,16 @@
         DIM                 = b'\x1b[2m'
         ITALIC              = b'\x1b[3m'
         UNDERLINE           = b'\x1b[4m'
         UNDERLINE_DOUBLE    = b'\x1b[4:2m'
         UNDERLINE_CURLY     = b'\x1b[4:3m'
         BLINK               = b'\x1b[5m'
         REVERSE             = b'\x1b[7m'
-        INVISIBLE           = b'\x1b[8m'    # Invisible but copy-pasteable
+        INVISIBLE           = b'\x1b[8m'
+        '''Invisible but copy-pasteable'''
         STRIKETHROUGH       = b'\x1b[9m'
         OVERLINE            = b'\x1b[53m'
     class Color:
         DARKGRAY            = b'\x1b[30m'
         RED                 = b'\x1b[31m'
         GREEN               = b'\x1b[32m'
         YELLOW              = b'\x1b[33m'
```

### Comparing `dav_tools-0.1.0/src/dav_tools/commands.py` & `dav_tools-0.1.1/src/dav_tools/commands.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,36 @@
+'''External command execution on local machine.'''
+
 import platform as _platform
 import subprocess as _subprocess
 from shlex import split as _split
 from subprocess import CalledProcessError
+from typing import Callable as _Callable
 
 
-# runs a command, depeding on the current OS
-#   returns True if the program exits with return code zero, False otherwise
 def execute(command: str) -> bool:
+    '''
+    Run a command.
+
+    :param command: the command to execute
+
+    :returns: `True` if the command exits with return code zero, `False` otherwise
+    '''
     exit_status = _subprocess.check_call(_split(command))
     return exit_status == 0
 
-# runs a command, depeding on the current OS
-#   the output is returned in the specified type (default: bytes)
-#   if a command returns a non-zero exit code the program raises an exception (default behavior) or returns a given value (by default: None)
-def get_output(command: str, on_success = lambda x: x, on_error = None):
+def get_output(command: str, on_success: _Callable[[bytes], any] = lambda x: x, on_error: _Callable[[], any] = None):
+    '''
+    Run a command and return its output.
+    
+    :param command: the command to execute
+
+    :param on_success: call the specified function on the output before returning the data. Useful for casting the output from its original `bytes` format
+    :param on_error: call the specified function if the command raised an exception. If this value is `None`, raises the exception.
+    '''
     try:
         return on_success(_subprocess.check_output(_split(command)))
     except CalledProcessError as e:
         if on_error is None:
             raise e
         return on_success(on_error())
```

### Comparing `dav_tools-0.1.0/src/dav_tools/devtools.py` & `dav_tools-0.1.1/src/dav_tools/devtools.py`

 * *Files identical despite different names*

### Comparing `dav_tools-0.1.0/src/dav_tools/messages.py` & `dav_tools-0.1.1/src/dav_tools/messages.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     :param icon: Character to use as icon, between ``[ ]``.
     :param icon_options: Styling options applied to the icon.
     :param blink: If True, the icon blinks.
     :param end: Character to output at the end of the message.
     :param file: Where to write the message.
     '''
 
-    _clear_line()
+    _clear_line(file=file)
 
     # icon
     if icon is not None:
         _print_colored_text('[', *icon_options, TextFormat.Style.BOLD, end='', file=file)
         
         if blink:
             _print_colored_text(icon, *icon_options, TextFormat.Style.BOLD, TextFormat.Style.BLINK, end='', file=file)
@@ -89,15 +89,15 @@
     '''
 
     message(*text,
             icon=' ',
             end='\r',
             text_min_len=text_min_len,
             default_text_options=[
-                TextFormat.Color.DARKGRAY,
+                TextFormat.Style.DIM,
                 TextFormat.Style.ITALIC
             ],
             additional_text_options=text_options
     )
 
 
 def error(*text: str | object, text_min_len: list[int] = [], text_options: list[list] = [[]], blink: bool = False):
```

### Comparing `dav_tools-0.1.0/src/dav_tools/requirements.py` & `dav_tools-0.1.1/src/dav_tools/requirements.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 '''Requirements for running a progam.'''
 
 from . import messages as _messages
 
 import os as _os
 import ctypes as _ctypes
 import platform as _platform
+import elevate as _elevate
 
-def require(root=False, os:list[str]=[]):
+
+def require(root = False, os: list[str] = []):
     '''
     Require the program to statisfy the given requirements before continuing its execution.
 
     :param root: If True, the program needs to be run as root (if it isn't already, it automatically tries to relaunch itself with root privileges).
     :param os: Unless the list is empty, the program can be run only on specified OSes. If it isn't, the program terminates.
     '''
     if len(os) > 0:
         _require_os(*os)
 
     if root:
         _require_root()
 
-def _require_root(auto_elevate=True):
-    if auto_elevate:
-        import elevate as _elevate
-        _elevate.elevate(graphical=False)
+def _require_root():
+    _elevate.elevate(graphical=False)
 
     if _platform.system() == 'Windows':
         if _ctypes.WinDLL('Shell32').IsUserAnAdmin() == 0:
             _messages.critical_error('Program must be run as root')
     else:
         if _os.geteuid() != 0:
             _messages.critical_error('Program must be run as root')
```

### Comparing `dav_tools-0.1.0/src/dav_tools/text_color.py` & `dav_tools-0.1.1/src/dav_tools/text_color.py`

 * *Files 4% similar despite different names*

```diff
@@ -82,9 +82,16 @@
     '''
     Clears the current line from any text of formatting.
     Not really suitable for files.
 
     :param file: Stream to clear.
     :param flush: Whether to flush the stream after printing.
     '''
-    print('\r', ' ' * _os.get_terminal_size().columns, '\r',
-          sep='', end='', file=file, flush=flush)
+    
+    try:
+        size = _os.get_terminal_size().columns
+        print('\r', ' ' * size, '\r',
+              sep='', end='', file=file, flush=flush)
+    except OSError:
+        pass    # Do nothing
+
+
```

### Comparing `dav_tools-0.1.0/LICENSE` & `dav_tools-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dav_tools-0.1.0/pyproject.toml` & `dav_tools-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "dav_tools"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Davide Ponzini", email="davide.ponzini95@gmail.com" },
 ]
 description = "Various utilies to aid in program development."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `dav_tools-0.1.0/PKG-INFO` & `dav_tools-0.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dav_tools
-Version: 0.1.0
+Version: 0.1.1
 Summary: Various utilies to aid in program development.
 Project-URL: Repository, https://github.com/DavidePonzini/dav-utils
 Project-URL: Documentation, https://dav-tools.readthedocs.io/en/latest/index.html
 Project-URL: Bug Tracker, https://github.com/DavidePonzini/dav-utils/issues
 Author-email: Davide Ponzini <davide.ponzini95@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

