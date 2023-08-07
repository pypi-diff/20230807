# Comparing `tmp/jsonator-0.1.7.tar.gz` & `tmp/jsonator-0.1.8.tar.gz`

## Comparing `jsonator-0.1.7.tar` & `jsonator-0.1.8.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     3258 2020-02-02 00:00:00.000000 jsonator-0.1.7/jsonator/__init__.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 jsonator-0.1.7/jsonator/__main__.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 jsonator-0.1.7/jsonator/enum.py
--rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 jsonator-0.1.7/jsonator/jsonator.py
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 jsonator-0.1.7/jsonator/output.py
--rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 jsonator-0.1.7/jsonator/report.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 jsonator-0.1.7/.gitignore
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 jsonator-0.1.7/LICENSE
--rw-r--r--   0        0        0     2502 2020-02-02 00:00:00.000000 jsonator-0.1.7/README.md
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 jsonator-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 jsonator-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     3645 2020-02-02 00:00:00.000000 jsonator-0.1.8/jsonator/__init__.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 jsonator-0.1.8/jsonator/__main__.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 jsonator-0.1.8/jsonator/enum.py
+-rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 jsonator-0.1.8/jsonator/jsonator.py
+-rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 jsonator-0.1.8/jsonator/output.py
+-rw-r--r--   0        0        0     2679 2020-02-02 00:00:00.000000 jsonator-0.1.8/jsonator/report.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 jsonator-0.1.8/.gitignore
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 jsonator-0.1.8/LICENSE
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 jsonator-0.1.8/README.md
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 jsonator-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     2984 2020-02-02 00:00:00.000000 jsonator-0.1.8/PKG-INFO
```

### Comparing `jsonator-0.1.7/jsonator/jsonator.py` & `jsonator-0.1.8/jsonator/jsonator.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,96 +1,99 @@
-"""
-Format JSON using json tool
-"""
-import filecmp
-import os
-import random
-import string
-import sys
-from pathlib import Path
-from tempfile import gettempdir
-from typing import Optional
-
-from jsonator import output
-from jsonator.report import Report
-
-INTERPRETER = Path(sys.executable).stem
-FILES_ENCODING = "utf-8"
-
-
-def random_str() -> str:
-    """Generating a random alphanumeric string of 8 characters long"""
-    return "".join(random.choices(string.ascii_letters + string.digits, k=8))
-
-
-def make_temp_file() -> Path:
-    """Generate temp file path"""
-    temp_dir = Path(gettempdir()).absolute()
-    temp_file = temp_dir / random_str()
-
-    while temp_file.exists():
-        temp_file = temp_dir / random_str()
-
-    return temp_file
-
-
-def format_json_file(  # pylint: disable=too-many-arguments
-    json_file: Path,
-    report: Report,
-    check: bool,
-    diff: bool,
-    color: bool,
-    sort_keys: bool,
-    indent: Optional[int],
-    tab: bool,
-    no_indent: bool,
-    compact: bool,
-) -> None:
-    """
-    This function formats the file in JSON format.
-    It uses the json.tool module, built into Python, to create a readable JSON format.
-    """
-    tmp_file = make_temp_file()
-
-    cmd = [INTERPRETER, "-m", "json.tool", f'"{json_file}"', tmp_file]
-    if sort_keys:
-        cmd.append("--sort-keys")
-    if indent is not None:
-        cmd.append(f"--indent {indent}")
-    if tab:
-        cmd.append("--tab")
-    if no_indent:
-        cmd.append("--no-indent")
-    if compact:
-        cmd.append("--compact")
-
-    os.system(" ".join([str(command) for command in cmd]))
-
-    try:
-        is_identical = filecmp.cmp(json_file, tmp_file, shallow=False)
-    except FileNotFoundError:
-        report.failed(json_file, "Internal error")
-        return
-
-    report.done(json_file, not is_identical)
-
-    if diff:
-        diff_contents = output.diff(
-            json_file.read_text(encoding=FILES_ENCODING),
-            tmp_file.read_text(encoding=FILES_ENCODING),
-            json_file.name,
-            "formatted file",
-        )
-
-        if color:
-            diff_contents = output.color_diff(diff_contents)
-
-        print(diff_contents)
-
-    if tmp_file.exists():
-        if check or diff:
-            os.unlink(tmp_file)
-        else:
-            os.unlink(json_file)
-            os.rename(tmp_file, json_file)
-    else:
-        report.failed(json_file, "Internal error")
+"""
+Format JSON using json tool
+"""
+import filecmp
+import os
+import random
+import string
+import sys
+from pathlib import Path
+from tempfile import gettempdir
+from typing import Optional
+
+from jsonator import output
+from jsonator.report import Report
+
+INTERPRETER = Path(sys.executable).stem
+FILES_ENCODING = "utf-8"
+
+
+def random_str() -> str:
+    """Generating a random alphanumeric string of 8 characters long"""
+    return "".join(random.choices(string.ascii_letters + string.digits, k=8))
+
+
+def make_temp_file() -> Path:
+    """Generate temp file path"""
+    temp_dir = Path(gettempdir()).absolute()
+    temp_file = temp_dir / random_str()
+
+    while temp_file.exists():
+        temp_file = temp_dir / random_str()
+
+    return temp_file
+
+
+def format_json_file(  # pylint: disable=too-many-arguments,too-many-branches
+    json_file: Path,
+    report: Report,
+    check: bool,
+    diff: bool,
+    color: bool,
+    sort_keys: bool,
+    indent: Optional[int],
+    tab: bool,
+    no_indent: bool,
+    compact: bool,
+    no_ensure_ascii: bool,
+) -> None:
+    """
+    This function formats the file in JSON format.
+    It uses the json.tool module, built into Python, to create a readable JSON format.
+    """
+    tmp_file = make_temp_file()
+
+    cmd = [INTERPRETER, "-m", "json.tool", f'"{json_file}"', tmp_file]
+    if sort_keys:
+        cmd.append("--sort-keys")
+    if indent is not None:
+        cmd.append(f"--indent {indent}")
+    if tab:
+        cmd.append("--tab")
+    if no_indent:
+        cmd.append("--no-indent")
+    if compact:
+        cmd.append("--compact")
+    if no_ensure_ascii:
+        cmd.append("--no-ensure-ascii")
+
+    os.system(" ".join([str(command) for command in cmd]))
+
+    try:
+        is_identical = filecmp.cmp(json_file, tmp_file, shallow=False)
+    except FileNotFoundError:
+        report.failed(json_file, "Internal error")
+        return
+
+    report.done(json_file, not is_identical)
+
+    if diff:
+        diff_contents = output.diff(
+            json_file.read_text(encoding=FILES_ENCODING),
+            tmp_file.read_text(encoding=FILES_ENCODING),
+            json_file.name,
+            "formatted file",
+        )
+
+        if color:
+            diff_contents = output.color_diff(diff_contents)
+
+        print(diff_contents)
+
+    if tmp_file.exists():
+        if check or diff:
+            os.unlink(tmp_file)
+        else:
+            os.unlink(json_file)
+            os.rename(tmp_file, json_file)
+    else:
+        report.failed(json_file, "Internal error")
```

### Comparing `jsonator-0.1.7/jsonator/output.py` & `jsonator-0.1.8/jsonator/output.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-"""
-Output features
-"""
-
-
-def diff(a_text: str, b_text: str, a_name: str, b_name: str) -> str:
-    """Return a unified diff string between strings `a` and `b`."""
-    import difflib  # pylint: disable=import-outside-toplevel
-
-    a_lines = a_text.splitlines(keepends=True)
-    b_lines = b_text.splitlines(keepends=True)
-    diff_lines = []
-    for line in difflib.unified_diff(a_lines, b_lines, fromfile=a_name, tofile=b_name, n=5):
-        # Work around https://bugs.python.org/issue2142
-        # See:
-        # https://www.gnu.org/software/diffutils/manual/html_node/Incomplete-Lines.html
-        if line[-1] == "\n":
-            diff_lines.append(line)
-        else:
-            diff_lines.append(line + "\n")
-            diff_lines.append("\\ No newline at end of file\n")
-    return "".join(diff_lines)
-
-
-def color_diff(contents: str) -> str:
-    """Inject the ANSI color codes to the diff."""
-    lines = contents.split("\n")
-    for i, line in enumerate(lines):
-        if line.startswith("+++") or line.startswith("---"):
-            line = "\033[1m" + line + "\033[0m"  # bold, reset
-        elif line.startswith("@@"):
-            line = "\033[36m" + line + "\033[0m"  # cyan, reset
-        elif line.startswith("+"):
-            line = "\033[32m" + line + "\033[0m"  # green, reset
-        elif line.startswith("-"):
-            line = "\033[31m" + line + "\033[0m"  # red, reset
-        lines[i] = line
-    return "\n".join(lines)
+"""
+Output features
+"""
+
+
+def diff(a_text: str, b_text: str, a_name: str, b_name: str) -> str:
+    """Return a unified diff string between strings `a` and `b`."""
+    import difflib  # pylint: disable=import-outside-toplevel
+
+    a_lines = a_text.splitlines(keepends=True)
+    b_lines = b_text.splitlines(keepends=True)
+    diff_lines = []
+    for line in difflib.unified_diff(a_lines, b_lines, fromfile=a_name, tofile=b_name, n=5):
+        # Work around https://bugs.python.org/issue2142
+        # See:
+        # https://www.gnu.org/software/diffutils/manual/html_node/Incomplete-Lines.html
+        if line[-1] == "\n":
+            diff_lines.append(line)
+        else:
+            diff_lines.append(line + "\n")
+            diff_lines.append("\\ No newline at end of file\n")
+    return "".join(diff_lines)
+
+
+def color_diff(contents: str) -> str:
+    """Inject the ANSI color codes to the diff."""
+    lines = contents.split("\n")
+    for i, line in enumerate(lines):
+        if line.startswith("+++") or line.startswith("---"):
+            line = "\033[1m" + line + "\033[0m"  # bold, reset
+        elif line.startswith("@@"):
+            line = "\033[36m" + line + "\033[0m"  # cyan, reset
+        elif line.startswith("+"):
+            line = "\033[32m" + line + "\033[0m"  # green, reset
+        elif line.startswith("-"):
+            line = "\033[31m" + line + "\033[0m"  # red, reset
+        lines[i] = line
+    return "\n".join(lines)
```

### Comparing `jsonator-0.1.7/jsonator/report.py` & `jsonator-0.1.8/jsonator/report.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,73 +1,73 @@
-"""
-Summarize runs.
-"""
-import sys
-from pathlib import Path
-
-from jsonator.enum import ReturnCode
-
-
-class Report:
-    """Provides a reformatting counter. Can be rendered with `str(report)`."""
-
-    def __init__(self, check: bool, diff: bool) -> None:
-        self.check = check
-        self.diff = diff
-        self.change_count = 0
-        self.same_count = 0
-        self.failure_count = 0
-
-    def done(self, src: Path, changed: bool) -> None:
-        """Increment the counter for successful reformatting. Write out a message."""
-        if changed:
-            reformatted = "would reformat" if self.check or self.diff else "reformatted"
-            print(f"{reformatted} {src}")
-            self.change_count += 1
-        else:
-            print(f"{src} already well formatted, good job.")
-            self.same_count += 1
-
-    def failed(self, src: Path, message: str) -> None:
-        """Increment the counter for failed reformatting. Write out a message."""
-        print(f"error: cannot format {src}: {message}", file=sys.stderr)
-        self.failure_count += 1
-
-    @property
-    def status(self) -> int:
-        """Return the exit code that the app should use.
-
-        This considers the current state of changed files and failures:
-        - if there were any failures, return 123;
-        - if any files were changed and --check is being used, return 1;
-        - otherwise return 0.
-        """
-        if self.failure_count:
-            return ReturnCode.INTERNAL_ERROR.value
-
-        if self.change_count and self.check:
-            return ReturnCode.SOME_FILES_WOULD_BE_REFORMATTED.value
-
-        return ReturnCode.NOTHING_WOULD_CHANGE.value
-
-    def __str__(self) -> str:
-        """Render a report of the current state."""
-        if self.check or self.diff:
-            reformatted = "would be reformatted"
-            unchanged = "would be left unchanged"
-            failed = "would fail to reformat"
-        else:
-            reformatted = "reformatted"
-            unchanged = "left unchanged"
-            failed = "failed to reformat"
-        report = []
-        if self.change_count:
-            ending = "s" if self.change_count > 1 else ""
-            report.append(f"{self.change_count} file{ending} {reformatted}")
-
-        if self.same_count:
-            ending = "s" if self.same_count > 1 else ""
-            report.append(f"{self.same_count} file{ending} {unchanged}")
-        if self.failure_count:
-            ending = "s" if self.failure_count > 1 else ""
-            report.append(f"{self.failure_count} file{ending} {failed}")
-        return ", ".join(report) + "."
+"""
+Summarize runs.
+"""
+import sys
+from pathlib import Path
+
+from jsonator.enum import ReturnCode
+
+
+class Report:
+    """Provides a reformatting counter. Can be rendered with `str(report)`."""
+
+    def __init__(self, check: bool, diff: bool) -> None:
+        self.check = check
+        self.diff = diff
+        self.change_count = 0
+        self.same_count = 0
+        self.failure_count = 0
+
+    def done(self, src: Path, changed: bool) -> None:
+        """Increment the counter for successful reformatting. Write out a message."""
+        if changed:
+            reformatted = "would reformat" if self.check or self.diff else "reformatted"
+            print(f"{reformatted} {src}")
+            self.change_count += 1
+        else:
+            print(f"{src} already well formatted, good job.")
+            self.same_count += 1
+
+    def failed(self, src: Path, message: str) -> None:
+        """Increment the counter for failed reformatting. Write out a message."""
+        print(f"error: cannot format {src}: {message}", file=sys.stderr)
+        self.failure_count += 1
+
+    @property
+    def status(self) -> int:
+        """Return the exit code that the app should use.
+
+        This considers the current state of changed files and failures:
+        - if there were any failures, return 123;
+        - if any files were changed and --check is being used, return 1;
+        - otherwise return 0.
+        """
+        if self.failure_count:
+            return ReturnCode.INTERNAL_ERROR.value
+
+        if self.change_count and self.check:
+            return ReturnCode.SOME_FILES_WOULD_BE_REFORMATTED.value
+
+        return ReturnCode.NOTHING_WOULD_CHANGE.value
+
+    def __str__(self) -> str:
+        """Render a report of the current state."""
+        if self.check or self.diff:
+            reformatted = "would be reformatted"
+            unchanged = "would be left unchanged"
+            failed = "would fail to reformat"
+        else:
+            reformatted = "reformatted"
+            unchanged = "left unchanged"
+            failed = "failed to reformat"
+        report = []
+        if self.change_count:
+            ending = "s" if self.change_count > 1 else ""
+            report.append(f"{self.change_count} file{ending} {reformatted}")
+
+        if self.same_count:
+            ending = "s" if self.same_count > 1 else ""
+            report.append(f"{self.same_count} file{ending} {unchanged}")
+        if self.failure_count:
+            ending = "s" if self.failure_count > 1 else ""
+            report.append(f"{self.failure_count} file{ending} {failed}")
+        return ", ".join(report) + "."
```

### Comparing `jsonator-0.1.7/LICENSE` & `jsonator-0.1.8/LICENSE`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-BSD 3-Clause License
-
-Copyright (c) 2023, Sergey Fomin
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-
-1. Redistributions of source code must retain the above copyright notice, this
-   list of conditions and the following disclaimer.
-
-2. Redistributions in binary form must reproduce the above copyright notice,
-   this list of conditions and the following disclaimer in the documentation
-   and/or other materials provided with the distribution.
-
-3. Neither the name of the copyright holder nor the names of its
-   contributors may be used to endorse or promote products derived from
-   this software without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+BSD 3-Clause License
+
+Copyright (c) 2023, Sergey Fomin
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+1. Redistributions of source code must retain the above copyright notice, this
+   list of conditions and the following disclaimer.
+
+2. Redistributions in binary form must reproduce the above copyright notice,
+   this list of conditions and the following disclaimer in the documentation
+   and/or other materials provided with the distribution.
+
+3. Neither the name of the copyright holder nor the names of its
+   contributors may be used to endorse or promote products derived from
+   this software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `jsonator-0.1.7/README.md` & `jsonator-0.1.8/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,80 +1,82 @@
-JSONator
-========
-
-[![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
-[![Downloads](https://static.pepy.tech/badge/jsonator)](https://pepy.tech/project/jsonator)
-
-Description
------------
-
-This module provides a command-line interface for formatting JSON files.
-It takes a path to either a JSON file or a directory containing JSON files
-as input and can recursively scan subdirectories for JSON files. The module
-returns an exit code indicating whether any files were reformatted or if there
-were any errors.
-
-Usage
------
-
-The main() function is the entry point for the module and returns an exit code
-indicating the result of the JSON formatting operation. The following arguments
-can be passed to the main() function:
-
-* path: A required argument that specifies the path to the JSON file or directory containing JSON files to be formatted.
-
-* --recursive or -r: An optional flag that specifies whether to scan subdirectories for JSON files.
-
-* --check: An optional flag that indicates whether to perform a dry run and return the status without actually reformatting the files. The exit code will indicate whether any files would be reformatted or if there were any errors.
-
-* --diff: Don't write the files back, just output a diff for each file on stdout.
-
-* --color: Show colored diff. Only applies when `--diff` is given.
-
-* --sort-keys: Sort the output of dictionaries alphabetically by key. *Available on Python 3.5+.*
-
-* --indent: Separate items with newlines and use this number of spaces for indentation.
-
-* --tab: Separate items with newlines and use tabs for indentation.
-
-* --no-indent: Separate items with spaces rather than newlines.
-
-* --compact: Suppress all whitespace separation (most compact).
-
-  *--indent, --tab, --no-indent, --compact — mutually exclusive options for whitespace control. Available on Python 3.9+.*
-
-The module uses the ReturnCode enum to indicate the exit code of the formatting operation. The possible exit codes are:
-
-* `0`: Indicates that no files would be reformatted.
-
-* `1`: Indicates that some files would be reformatted.
-
-* `122`: Indicates that the specified file or directory was not found.
-
-* `123`: Indicates that there was an internal error.
-
-Example usage:
---------------
-
-```
-$ jsonator /path/to/json/file.json --check
-```
-
-Dev:
---------------
-Build package
-
-```
-$ python -m build
-```
-
-Check package
-
-```
-$ twine check dist/*
-```
-
-Publish package
-
-```
-$ twine upload dist/*
-```
+JSONator
+========
+
+[![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
+[![Downloads](https://static.pepy.tech/badge/jsonator)](https://pepy.tech/project/jsonator)
+
+Description
+-----------
+
+This module provides a command-line interface for formatting JSON files.
+It takes a path to either a JSON file or a directory containing JSON files
+as input and can recursively scan subdirectories for JSON files. The module
+returns an exit code indicating whether any files were reformatted or if there
+were any errors.
+
+Usage
+-----
+
+The main() function is the entry point for the module and returns an exit code
+indicating the result of the JSON formatting operation. The following arguments
+can be passed to the main() function:
+
+* path: A required argument that specifies the path to the JSON file or directory containing JSON files to be formatted.
+
+* --recursive or -r: An optional flag that specifies whether to scan subdirectories for JSON files.
+
+* --check: An optional flag that indicates whether to perform a dry run and return the status without actually reformatting the files. The exit code will indicate whether any files would be reformatted or if there were any errors.
+
+* --diff: Don't write the files back, just output a diff for each file on stdout.
+
+* --color: Show colored diff. Only applies when `--diff` is given.
+
+* --sort-keys: Sort the output of dictionaries alphabetically by key. *Available on Python 3.5+.*
+
+* --no-ensure-ascii: Disable escaping of non-ASCII characters. *Available on Python 3.9+.*
+
+* --indent: Separate items with newlines and use this number of spaces for indentation.
+
+* --tab: Separate items with newlines and use tabs for indentation.
+
+* --no-indent: Separate items with spaces rather than newlines.
+
+* --compact: Suppress all whitespace separation (most compact).
+
+  *--indent, --tab, --no-indent, --compact — mutually exclusive options for whitespace control. Available on Python 3.9+.*
+
+The module uses the ReturnCode enum to indicate the exit code of the formatting operation. The possible exit codes are:
+
+* `0`: Indicates that no files would be reformatted.
+
+* `1`: Indicates that some files would be reformatted.
+
+* `122`: Indicates that the specified file or directory was not found.
+
+* `123`: Indicates that there was an internal error.
+
+Example usage:
+--------------
+
+```
+$ jsonator /path/to/json/file.json --check
+```
+
+Dev:
+--------------
+Build package
+
+```
+$ python -m build
+```
+
+Check package
+
+```
+$ twine check dist/*
+```
+
+Publish package
+
+```
+$ twine upload dist/*
+```
```

### Comparing `jsonator-0.1.7/pyproject.toml` & `jsonator-0.1.8/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-[build-system]
-requires = [
-    "hatchling>=0.25.1",
-]
-build-backend = "hatchling.build"
-
-[project]
-name = "jsonator"
-version = "0.1.7"
-authors = [
-  { name="Sergey Fomin", email="sergiusnn@gmail.com" },
-]
-description = "JSON formatting and validating tool"
-readme = "README.md"
-requires-python = ">=3.5"
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: BSD License",
-]
-
-[project.urls]
-"Homepage" = "https://github.com/sfominx/jsonator"
-
-[tool.hatch.build.targets.sdist]
-include = [
-    "/jsonator",
-]
-
-[tool.hatch.build.targets.wheel]
-include = [
-    "/jsonator/*",
-]
-
-[project.scripts]
-jsonator = "jsonator:main"
-
-[tool.poetry]
-readme = "README.md"
-name = "jsonator"
-version = "0.1.7"
-description = "JSON formatting and validating tool"
-authors = [
-  "Sergey Fomin <sergiusnn@gmail.com>",
-]
+[build-system]
+requires = [
+    "hatchling>=0.25.1",
+]
+build-backend = "hatchling.build"
+
+[project]
+name = "jsonator"
+version = "0.1.8"
+authors = [
+  { name="Sergey Fomin", email="sergiusnn@gmail.com" },
+]
+description = "JSON formatting and validating tool"
+readme = "README.md"
+requires-python = ">=3.5"
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: BSD License",
+]
+
+[project.urls]
+"Homepage" = "https://github.com/sfominx/jsonator"
+
+[tool.hatch.build.targets.sdist]
+include = [
+    "/jsonator",
+]
+
+[tool.hatch.build.targets.wheel]
+include = [
+    "/jsonator/*",
+]
+
+[project.scripts]
+jsonator = "jsonator:main"
+
+[tool.poetry]
+readme = "README.md"
+name = "jsonator"
+version = "0.1.8"
+description = "JSON formatting and validating tool"
+authors = [
+  "Sergey Fomin <sergiusnn@gmail.com>",
+]
```

### Comparing `jsonator-0.1.7/PKG-INFO` & `jsonator-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonator
-Version: 0.1.7
+Version: 0.1.8
 Summary: JSON formatting and validating tool
 Project-URL: Homepage, https://github.com/sfominx/jsonator
 Author-email: Sergey Fomin <sergiusnn@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.5
@@ -40,14 +40,16 @@
 
 * --diff: Don't write the files back, just output a diff for each file on stdout.
 
 * --color: Show colored diff. Only applies when `--diff` is given.
 
 * --sort-keys: Sort the output of dictionaries alphabetically by key. *Available on Python 3.5+.*
 
+* --no-ensure-ascii: Disable escaping of non-ASCII characters. *Available on Python 3.9+.*
+
 * --indent: Separate items with newlines and use this number of spaces for indentation.
 
 * --tab: Separate items with newlines and use tabs for indentation.
 
 * --no-indent: Separate items with spaces rather than newlines.
 
 * --compact: Suppress all whitespace separation (most compact).
```

