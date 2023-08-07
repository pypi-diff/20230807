# Comparing `tmp/monstera-0.0.4.tar.gz` & `tmp/monstera-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monstera-0.0.4.tar", last modified: Tue Aug  1 02:31:08 2023, max compression
+gzip compressed data, was "monstera-0.0.5.tar", last modified: Mon Aug  7 01:39:57 2023, max compression
```

## Comparing `monstera-0.0.4.tar` & `monstera-0.0.5.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 dishb      (502) staff       (20)        0 2023-08-01 02:31:08.552963 monstera-0.0.4/
--rw-r--r--   0 dishb      (502) staff       (20)     1099 2023-07-31 17:18:53.000000 monstera-0.0.4/LICENSE.md
--rw-r--r--   0 dishb      (502) staff       (20)     5713 2023-08-01 02:31:08.548981 monstera-0.0.4/PKG-INFO
--rw-r--r--   0 dishb      (502) staff       (20)     4424 2023-07-31 20:58:11.000000 monstera-0.0.4/README.md
-drwxr-xr-x   0 dishb      (502) staff       (20)        0 2023-08-01 02:31:08.453819 monstera-0.0.4/monstera/
--rw-r--r--   0 dishb      (502) staff       (20)     2871 2023-08-01 02:28:58.000000 monstera-0.0.4/monstera/__init__.py
--rw-r--r--   0 dishb      (502) staff       (20)     1402 2023-07-31 20:23:46.000000 monstera-0.0.4/monstera/__main__.py
-drwxr-xr-x   0 dishb      (502) staff       (20)        0 2023-08-01 02:31:08.496712 monstera-0.0.4/monstera/_core/
--rw-r--r--   0 dishb      (502) staff       (20)     1272 2023-07-31 20:20:59.000000 monstera-0.0.4/monstera/_core/__init__.py
--rw-r--r--   0 dishb      (502) staff       (20)     4200 2023-07-31 20:24:20.000000 monstera-0.0.4/monstera/_core/_entry_points.py
--rw-r--r--   0 dishb      (502) staff       (20)     5509 2023-07-31 21:24:46.000000 monstera-0.0.4/monstera/_core/_main.py
-drwxr-xr-x   0 dishb      (502) staff       (20)        0 2023-08-01 02:31:08.482531 monstera-0.0.4/monstera.egg-info/
--rw-r--r--   0 dishb      (502) staff       (20)     5713 2023-08-01 02:31:08.000000 monstera-0.0.4/monstera.egg-info/PKG-INFO
--rw-r--r--   0 dishb      (502) staff       (20)      394 2023-08-01 02:31:08.000000 monstera-0.0.4/monstera.egg-info/SOURCES.txt
--rw-r--r--   0 dishb      (502) staff       (20)        1 2023-08-01 02:31:08.000000 monstera-0.0.4/monstera.egg-info/dependency_links.txt
--rw-r--r--   0 dishb      (502) staff       (20)       67 2023-08-01 02:31:08.000000 monstera-0.0.4/monstera.egg-info/entry_points.txt
--rw-r--r--   0 dishb      (502) staff       (20)       16 2023-08-01 02:31:08.000000 monstera-0.0.4/monstera.egg-info/requires.txt
--rw-r--r--   0 dishb      (502) staff       (20)        9 2023-08-01 02:31:08.000000 monstera-0.0.4/monstera.egg-info/top_level.txt
--rw-r--r--   0 dishb      (502) staff       (20)       38 2023-08-01 02:31:08.553494 monstera-0.0.4/setup.cfg
--rw-r--r--   0 dishb      (502) staff       (20)     3635 2023-08-01 02:28:32.000000 monstera-0.0.4/setup.py
-drwxr-xr-x   0 dishb      (502) staff       (20)        0 2023-08-01 02:31:08.546457 monstera-0.0.4/tests/
--rw-r--r--   0 dishb      (502) staff       (20)     3774 2023-08-01 02:20:02.000000 monstera-0.0.4/tests/test_monstera.py
--rw-r--r--   0 dishb      (502) staff       (20)     3858 2023-07-31 17:18:53.000000 monstera-0.0.4/tests/test_python_m.py
+drwxr-xr-x   0 dishb      (502) staff       (20)        0 2023-08-07 01:39:57.708279 monstera-0.0.5/
+-rw-r--r--   0 dishb      (502) staff       (20)     1099 2023-08-04 23:52:27.000000 monstera-0.0.5/LICENSE.md
+-rw-r--r--   0 dishb      (502) staff       (20)     5685 2023-08-07 01:39:57.707499 monstera-0.0.5/PKG-INFO
+-rw-r--r--   0 dishb      (502) staff       (20)     4396 2023-08-05 18:16:33.000000 monstera-0.0.5/README.md
+drwxr-xr-x   0 dishb      (502) staff       (20)        0 2023-08-07 01:39:57.671311 monstera-0.0.5/monstera/
+-rw-r--r--   0 dishb      (502) staff       (20)     2583 2023-08-07 01:37:09.000000 monstera-0.0.5/monstera/__init__.py
+-rw-r--r--   0 dishb      (502) staff       (20)     1402 2023-08-04 23:52:27.000000 monstera-0.0.5/monstera/__main__.py
+drwxr-xr-x   0 dishb      (502) staff       (20)        0 2023-08-07 01:39:57.693233 monstera-0.0.5/monstera/_core/
+-rw-r--r--   0 dishb      (502) staff       (20)     1272 2023-08-04 23:52:27.000000 monstera-0.0.5/monstera/_core/__init__.py
+-rw-r--r--   0 dishb      (502) staff       (20)     5613 2023-08-07 01:25:25.000000 monstera-0.0.5/monstera/_core/_entry_points.py
+-rw-r--r--   0 dishb      (502) staff       (20)     5509 2023-08-06 23:22:16.000000 monstera-0.0.5/monstera/_core/_main.py
+-rw-r--r--   0 dishb      (502) staff       (20)     1532 2023-08-06 23:12:27.000000 monstera-0.0.5/monstera/_core/_utils.py
+drwxr-xr-x   0 dishb      (502) staff       (20)        0 2023-08-07 01:39:57.679266 monstera-0.0.5/monstera.egg-info/
+-rw-r--r--   0 dishb      (502) staff       (20)     5685 2023-08-07 01:39:57.000000 monstera-0.0.5/monstera.egg-info/PKG-INFO
+-rw-r--r--   0 dishb      (502) staff       (20)      419 2023-08-07 01:39:57.000000 monstera-0.0.5/monstera.egg-info/SOURCES.txt
+-rw-r--r--   0 dishb      (502) staff       (20)        1 2023-08-07 01:39:57.000000 monstera-0.0.5/monstera.egg-info/dependency_links.txt
+-rw-r--r--   0 dishb      (502) staff       (20)       67 2023-08-07 01:39:57.000000 monstera-0.0.5/monstera.egg-info/entry_points.txt
+-rw-r--r--   0 dishb      (502) staff       (20)       16 2023-08-07 01:39:57.000000 monstera-0.0.5/monstera.egg-info/requires.txt
+-rw-r--r--   0 dishb      (502) staff       (20)        9 2023-08-07 01:39:57.000000 monstera-0.0.5/monstera.egg-info/top_level.txt
+-rw-r--r--   0 dishb      (502) staff       (20)       38 2023-08-07 01:39:57.708412 monstera-0.0.5/setup.cfg
+-rw-r--r--   0 dishb      (502) staff       (20)     3631 2023-08-07 01:36:36.000000 monstera-0.0.5/setup.py
+drwxr-xr-x   0 dishb      (502) staff       (20)        0 2023-08-07 01:39:57.705394 monstera-0.0.5/tests/
+-rw-r--r--   0 dishb      (502) staff       (20)     4453 2023-08-04 23:52:27.000000 monstera-0.0.5/tests/test_monstera.py
+-rw-r--r--   0 dishb      (502) staff       (20)     4565 2023-08-04 23:52:27.000000 monstera-0.0.5/tests/test_python_m.py
```

### Comparing `monstera-0.0.4/LICENSE.md` & `monstera-0.0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `monstera-0.0.4/PKG-INFO` & `monstera-0.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monstera
-Version: 0.0.4
+Version: 0.0.5
 Summary: A cross-platform CLI to quickly retrieve system information to make issue management easier.
 Home-page: https://github.com/dishb/monstera
 Author: Dishant B. (@dishb)
 Author-email: code.dishb@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/dishb/monstera/tree/main/docs
 Project-URL: Source, https://github.com/dishb/monstera/
@@ -100,21 +100,21 @@
     import monstera
 
     monstera.run()
     ```
 
 ## Contributing:
 To get started with contributing to `monstera`, follow this guide.
-It is recommended to read the [`./.github/CONTRIBUTING.md`](https://github.com/dishb/monstera/blob/main/.github/CONTRIBUTING.md) file.
+It is recommended to read the [`./CONTRIBUTING.md`](https://github.com/dishb/monstera/blob/main/CONTRIBUTING.md) file.
 
 1. Clone the repository:
 
     | OS Independent |
     | --- |
-    | `git clone https://github.com/dishb/monstera` |
+    | `git clone https://github.com/dishb/monstera.git` |
 
     Change to the directory:
 
     | macOS/Linux | Windows |
     | --- | --- |
     | `cd ./monstera/` | `cd .\monstera\` |
 
@@ -136,15 +136,15 @@
 
     | macOS/Linux | Windows |
     | --- | --- |
     | `pip3 install -e .` | `pip install -e .` |
 
 ## Code of Conduct
 This project is goverened by the Contributor Covenant Code of Conduct.
-We ask that you read the full Code of Conduct in the [`./.github/CODE_OF_CONDUCT.md`](https://github.com/dishb/monstera/blob/main/.github/CODE_OF_CONDUCT.md) file.
+We ask that you read the full Code of Conduct in the [`./CODE_OF_CONDUCT.md`](https://github.com/dishb/monstera/blob/main/CODE_OF_CONDUCT.md) file.
 
 ## License:
 This project is licensed under the `MIT License`. The full copyright can be found in the [`./LICENSE.md`](https://github.com/dishb/monstera/blob/main/LICENSE.md) file.
 
 ## Attribution
 
 The background photo in [`./assets/banner.png`](https://github.com/dishb/monstera/blob/main/assets/banner.png) is by [Gilles Lambert](https://unsplash.com/@gilleslambert?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText) on [Unsplash](https://unsplash.com/photos/mSK5nNsAsLY?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText)
```

### Comparing `monstera-0.0.4/README.md` & `monstera-0.0.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -73,21 +73,21 @@
     import monstera
 
     monstera.run()
     ```
 
 ## Contributing:
 To get started with contributing to `monstera`, follow this guide.
-It is recommended to read the [`./.github/CONTRIBUTING.md`](https://github.com/dishb/monstera/blob/main/.github/CONTRIBUTING.md) file.
+It is recommended to read the [`./CONTRIBUTING.md`](https://github.com/dishb/monstera/blob/main/CONTRIBUTING.md) file.
 
 1. Clone the repository:
 
     | OS Independent |
     | --- |
-    | `git clone https://github.com/dishb/monstera` |
+    | `git clone https://github.com/dishb/monstera.git` |
 
     Change to the directory:
 
     | macOS/Linux | Windows |
     | --- | --- |
     | `cd ./monstera/` | `cd .\monstera\` |
 
@@ -109,15 +109,15 @@
 
     | macOS/Linux | Windows |
     | --- | --- |
     | `pip3 install -e .` | `pip install -e .` |
 
 ## Code of Conduct
 This project is goverened by the Contributor Covenant Code of Conduct.
-We ask that you read the full Code of Conduct in the [`./.github/CODE_OF_CONDUCT.md`](https://github.com/dishb/monstera/blob/main/.github/CODE_OF_CONDUCT.md) file.
+We ask that you read the full Code of Conduct in the [`./CODE_OF_CONDUCT.md`](https://github.com/dishb/monstera/blob/main/CODE_OF_CONDUCT.md) file.
 
 ## License:
 This project is licensed under the `MIT License`. The full copyright can be found in the [`./LICENSE.md`](https://github.com/dishb/monstera/blob/main/LICENSE.md) file.
 
 ## Attribution
 
 The background photo in [`./assets/banner.png`](https://github.com/dishb/monstera/blob/main/assets/banner.png) is by [Gilles Lambert](https://unsplash.com/@gilleslambert?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText) on [Unsplash](https://unsplash.com/photos/mSK5nNsAsLY?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText)
```

### Comparing `monstera-0.0.4/monstera/__init__.py` & `monstera-0.0.5/monstera/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,32 +30,33 @@
 Source: https://github.com/dishb/monstera
 """
 
 from ._core._main import run
 
 __source__ = "https://github.com/dishb/monstera"
 __license__ = "MIT License"
-__version__ = "0.0.4"
+__version__ = "0.0.5"
 __author__ = "Dishant B. (@dishb) <code.dishb@gmail.com>"
 __copyright__ = """
-                MIT License
+MIT License
 
-                Copyright (c) 2023 Dishant B. (@dishb) <code.dishb@gmail.com>
+Copyright (c) 2023 Dishant B. (@dishb) <code.dishb@gmail.com>
 
-                Permission is hereby granted, free of charge, to any person obtaining a copy
-                of this software and associated documentation files (the "Software"), to deal
-                in the Software without restriction, including without limitation the rights
-                to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-                copies of the Software, and to permit persons to whom the Software is
-                furnished to do so, subject to the following conditions:
-
-                The above copyright notice and this permission notice shall be included in all
-                copies or substantial portions of the Software.
-
-                THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-                IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-                FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-                AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-                LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-                OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-                SOFTWARE.
-                """
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE
+
+"""
```

### Comparing `monstera-0.0.4/monstera/__main__.py` & `monstera-0.0.5/monstera/__main__.py`

 * *Files identical despite different names*

### Comparing `monstera-0.0.4/monstera/_core/__init__.py` & `monstera-0.0.5/monstera/_core/__init__.py`

 * *Files identical despite different names*

### Comparing `monstera-0.0.4/monstera/_core/_main.py` & `monstera-0.0.5/monstera/_core/_main.py`

 * *Files identical despite different names*

### Comparing `monstera-0.0.4/monstera.egg-info/PKG-INFO` & `monstera-0.0.5/monstera.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monstera
-Version: 0.0.4
+Version: 0.0.5
 Summary: A cross-platform CLI to quickly retrieve system information to make issue management easier.
 Home-page: https://github.com/dishb/monstera
 Author: Dishant B. (@dishb)
 Author-email: code.dishb@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/dishb/monstera/tree/main/docs
 Project-URL: Source, https://github.com/dishb/monstera/
@@ -100,21 +100,21 @@
     import monstera
 
     monstera.run()
     ```
 
 ## Contributing:
 To get started with contributing to `monstera`, follow this guide.
-It is recommended to read the [`./.github/CONTRIBUTING.md`](https://github.com/dishb/monstera/blob/main/.github/CONTRIBUTING.md) file.
+It is recommended to read the [`./CONTRIBUTING.md`](https://github.com/dishb/monstera/blob/main/CONTRIBUTING.md) file.
 
 1. Clone the repository:
 
     | OS Independent |
     | --- |
-    | `git clone https://github.com/dishb/monstera` |
+    | `git clone https://github.com/dishb/monstera.git` |
 
     Change to the directory:
 
     | macOS/Linux | Windows |
     | --- | --- |
     | `cd ./monstera/` | `cd .\monstera\` |
 
@@ -136,15 +136,15 @@
 
     | macOS/Linux | Windows |
     | --- | --- |
     | `pip3 install -e .` | `pip install -e .` |
 
 ## Code of Conduct
 This project is goverened by the Contributor Covenant Code of Conduct.
-We ask that you read the full Code of Conduct in the [`./.github/CODE_OF_CONDUCT.md`](https://github.com/dishb/monstera/blob/main/.github/CODE_OF_CONDUCT.md) file.
+We ask that you read the full Code of Conduct in the [`./CODE_OF_CONDUCT.md`](https://github.com/dishb/monstera/blob/main/CODE_OF_CONDUCT.md) file.
 
 ## License:
 This project is licensed under the `MIT License`. The full copyright can be found in the [`./LICENSE.md`](https://github.com/dishb/monstera/blob/main/LICENSE.md) file.
 
 ## Attribution
 
 The background photo in [`./assets/banner.png`](https://github.com/dishb/monstera/blob/main/assets/banner.png) is by [Gilles Lambert](https://unsplash.com/@gilleslambert?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText) on [Unsplash](https://unsplash.com/photos/mSK5nNsAsLY?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText)
```

### Comparing `monstera-0.0.4/setup.py` & `monstera-0.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 
 from setuptools import setup
 
-VERSION = "0.0.4"
-DESCRIPTION = """A cross-platform CLI to quickly retrieve system information to make issue management easier."""
+VERSION = "0.0.5"
+DESCRIPTION = "A cross-platform CLI to quickly retrieve system information to make issue management easier."
 
 with open("README.md", "r", encoding = "utf-8") as file:
     LONG_DESCRIPTION = file.read()
     file.close()
 
 with open("requirements.txt", "r", encoding = "utf-8") as file:
     REQUIREMENTS = file.read()
```

### Comparing `monstera-0.0.4/tests/test_monstera.py` & `monstera-0.0.5/tests/test_monstera.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,14 +30,46 @@
 Source: https://github.com/dishb/monstera
 """
 
 from subprocess import run
 
 from pytest import main
 
+def test_empty_flag() -> None:
+    """
+    Tests the command: monstera -m
+
+    Only meant to be run by Dishant B. in his environment.
+    """
+
+    command = run(["monstera", "-m"],
+                  check = False,
+                  capture_output = True
+                  )
+    return_code = command.returncode
+    output = command.stdout.decode()
+
+    expected_output = """
+Python: 3.11.4, final release
+
+Python Location: /Users/dishb/Coding/monstera/.venv/bin
+
+Operating System: macOS 12.6.8
+
+Architecture: 64bit
+
+Pip: 23.2.1
+
+Pip Location: /Users/dishb/Coding/monstera/.venv/lib/python3.11/site-packages
+
+"""
+
+    assert return_code == 0
+    assert output == expected_output
+
 def test_no_package() -> None:
     """
     Tests the command: monstera
 
     Only meant to be run by Dishant B. in his environment.
     """
```

### Comparing `monstera-0.0.4/tests/test_python_m.py` & `monstera-0.0.5/tests/test_python_m.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,46 @@
 Source: https://github.com/dishb/monstera
 """
 
 from subprocess import run
 
 from pytest import main
 
+def test_empty_flag() -> None:
+    """
+    Tests the command: python3 -m monstera -m
+
+    Only meant to be run by Dishant B. in his environment.
+    """
+
+    command = run(["python3", "-m", "monstera", "-m"],
+                  check = False,
+                  capture_output = True
+                  )
+    return_code = command.returncode
+    output = command.stdout.decode()
+
+    expected_output = """
+Python: 3.11.4, final release
+
+Python Location: /Users/dishb/Coding/monstera/.venv/bin
+
+Operating System: macOS 12.6.8
+
+Architecture: 64bit
+
+Pip: 23.2.1
+
+Pip Location: /Users/dishb/Coding/monstera/.venv/lib/python3.11/site-packages
+
+"""
+
+    assert return_code == 0
+    assert output == expected_output
+
 def test_no_package() -> None:
     """
     Tests the command: python3 -m monstera
 
     Only meant to be run by Dishant B. in his environment.
     """
```

