# Comparing `tmp/coveo-systools-2.0.8a1.tar.gz` & `tmp/coveo-systools-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coveo-systools-2.0.8a1.tar", max compression
+gzip compressed data, was "coveo-systools-2.0.9.tar", max compression
```

## Comparing `coveo-systools-2.0.8a1.tar` & `coveo-systools-2.0.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     2372 2022-06-23 17:05:22.366739 coveo-systools-2.0.8a1/README.md
--rw-r--r--   0        0        0        0 2022-06-23 17:05:22.366739 coveo-systools-2.0.8a1/coveo_systools/__init__.py
--rw-r--r--   0        0        0     5946 2022-06-23 17:05:22.366739 coveo-systools-2.0.8a1/coveo_systools/filesystem.py
--rw-r--r--   0        0        0      257 2022-06-23 17:05:22.366739 coveo-systools-2.0.8a1/coveo_systools/platforms.py
--rw-r--r--   0        0        0        0 2022-06-23 17:05:22.366739 coveo-systools-2.0.8a1/coveo_systools/py.typed
--rw-r--r--   0        0        0      978 2022-06-23 17:05:22.366739 coveo-systools-2.0.8a1/coveo_systools/streams.py
--rw-r--r--   0        0        0    13709 2022-06-23 17:05:22.366739 coveo-systools-2.0.8a1/coveo_systools/subprocess.py
--rw-r--r--   0        0        0      759 2022-06-23 17:05:54.498834 coveo-systools-2.0.8a1/pyproject.toml
--rw-r--r--   0        0        0     3122 2022-06-23 17:05:55.633968 coveo-systools-2.0.8a1/setup.py
--rw-r--r--   0        0        0     3060 2022-06-23 17:05:55.634384 coveo-systools-2.0.8a1/PKG-INFO
+-rw-r--r--   0        0        0     2372 2022-08-23 12:03:31.719785 coveo-systools-2.0.9/README.md
+-rw-r--r--   0        0        0        0 2022-08-23 12:03:31.719785 coveo-systools-2.0.9/coveo_systools/__init__.py
+-rw-r--r--   0        0        0     5946 2022-08-23 12:03:31.719785 coveo-systools-2.0.9/coveo_systools/filesystem.py
+-rw-r--r--   0        0        0      257 2022-08-23 12:03:31.719785 coveo-systools-2.0.9/coveo_systools/platforms.py
+-rw-r--r--   0        0        0        0 2022-08-23 12:03:31.719785 coveo-systools-2.0.9/coveo_systools/py.typed
+-rw-r--r--   0        0        0      978 2022-08-23 12:03:31.719785 coveo-systools-2.0.9/coveo_systools/streams.py
+-rw-r--r--   0        0        0    14068 2022-08-23 12:03:31.719785 coveo-systools-2.0.9/coveo_systools/subprocess.py
+-rw-r--r--   0        0        0      810 2022-08-23 12:04:05.084029 coveo-systools-2.0.9/pyproject.toml
+-rw-r--r--   0        0        0     3120 2022-08-23 12:04:05.906021 coveo-systools-2.0.9/setup.py
+-rw-r--r--   0        0        0     3058 2022-08-23 12:04:05.906405 coveo-systools-2.0.9/PKG-INFO
```

### Comparing `coveo-systools-2.0.8a1/README.md` & `coveo-systools-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `coveo-systools-2.0.8a1/coveo_systools/filesystem.py` & `coveo-systools-2.0.9/coveo_systools/filesystem.py`

 * *Files identical despite different names*

### Comparing `coveo-systools-2.0.8a1/coveo_systools/streams.py` & `coveo-systools-2.0.9/coveo_systools/streams.py`

 * *Files identical despite different names*

### Comparing `coveo-systools-2.0.8a1/coveo_systools/subprocess.py` & `coveo-systools-2.0.9/coveo_systools/subprocess.py`

 * *Files 3% similar despite different names*

```diff
@@ -90,15 +90,21 @@
     decode_stdout = decode_output
 
     def command_str(self) -> str:
         """The 'cmd' from the underlying exception, separated with spaces"""
         command = self.cmd
         if isinstance(command, str):
             return command
-        return " ".join(command)
+
+        try:
+            return " ".join(str(part) for part in command)
+        except TypeError as exception:
+            if "not iterable" in str(exception):
+                return str(command)
+            raise
 
     @property
     def _wrapped_exception(self) -> BaseException:
         """This is the wrapped exception, which was either given to us (`raise from` -> __cause__) or assigned
         automatically by python when you `raise` from an exception handler (-> __context__)."""
         # unfortunately, cause and context are assigned after __init__, else we wouldn't need this property.
         if self.__wrapped_exception is None:
@@ -124,33 +130,36 @@
         """Handles str/bytes/None conversion to simplify code + strips whitespace."""
         if value is None:
             return None
         return (value.decode(errors=decode_errors) if isinstance(value, bytes) else value).strip()
 
     def __str__(self) -> str:
         """The main show!"""
-        errors: List[str] = [f"{self._wrapped_exception}\n"]
-
-        # add user-defined metadata to the error message.
-        errors.extend(f"{key}: {value}" for key, value in self.__metadata.items())
+        try:
+            errors: List[str] = [f"{self._wrapped_exception}\n"]
 
-        if isinstance(self._wrapped_exception, subprocess.CalledProcessError):
-            errors.extend(
-                [
-                    f"command: {self.command_str()}",
-                    f"exit code: {self.returncode}",
-                ]
-            )
+            # add user-defined metadata to the error message.
+            errors.extend(f"{key}: {value}" for key, value in self.__metadata.items())
 
-            if self.stdout:
-                errors.append(f"\n--<stdout>--\n{self.decode_stdout()}\n--</stdout>--\n")
-            if self.stderr:
-                errors.append(f"\n--<stderr>--\n{self.decode_stderr()}\n--</stderr>--\n")
+            if isinstance(self._wrapped_exception, subprocess.CalledProcessError):
+                errors.extend(
+                    [
+                        f"command: {self.command_str()}",
+                        f"exit code: {self.returncode}",
+                    ]
+                )
 
-        return "\n".join(errors)
+                if self.stdout:
+                    errors.append(f"\n--<stdout>--\n{self.decode_stdout()}\n--</stdout>--\n")
+                if self.stderr:
+                    errors.append(f"\n--<stderr>--\n{self.decode_stderr()}\n--</stderr>--\n")
+
+            return "\n".join(errors)
+        except Exception as exception:
+            return f"An error occurred when rendering the DetailedCalledProcessError: \n\n{exception}\n\n"
 
 
 class _CallProtocol(Protocol):
     """Adds type-check to the check_output and check_call protocols."""
 
     def __call__(
         self, command: Iterable[str], shell: bool = False, cwd: str = None, **kwargs: Any
@@ -243,30 +252,29 @@
     quoted: bool = False,
     **kwargs: Any,
 ) -> Optional[str]:
     """Async version of check_run"""
     converted_command, kwargs = _prepare_call(*command, verbose=verbose, quoted=quoted, **kwargs)
 
     if capture_output:
-        # the subprocess.check_output enforces this
+        # the subprocess.check_output enforces these, we do the same
         kwargs["stdout"] = asyncio.subprocess.PIPE
-        # allow redirection of stderr. e.g.: stderr=STDOUT
-        kwargs.setdefault("stderr", asyncio.subprocess.PIPE)
+        kwargs["stderr"] = asyncio.subprocess.PIPE
 
     process = await asyncio.create_subprocess_exec(
         converted_command[0], *converted_command[1:], cwd=str(working_directory), **kwargs
     )
     result = await process.wait()
     stdout = await process.stdout.read() if process.stdout else None
     stderr = await process.stderr.read() if process.stderr else None
 
     if result != 0:
         raise DetailedCalledProcessError(
             working_folder=working_directory
-        ) from subprocess.CalledProcessError(result, command, stdout, stderr)
+        ) from subprocess.CalledProcessError(result, converted_command, stdout, stderr)
 
     return _process_output(stdout) if capture_output else None
 
 
 def _process_output(output: Union[str, bytes]) -> str:
     encoding: Tuple[str, ...] = tuple()  # emptiness; encoding uses system/OS defaults
     if isinstance(output, str):
```

### Comparing `coveo-systools-2.0.8a1/pyproject.toml` & `coveo-systools-2.0.9/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 [tool.poetry]
 name = "coveo-systools"
-version = "2.0.8a1"
+version = "2.0.9"
 description = "Filesystem, language and OS related tools."
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/coveooss/coveo-python-oss/tree/main/coveo-systools"
 authors = ["Jonathan Piché <tools@coveo.com>"]
 
 [tool.poetry.dependencies]
 python = ">=3.8"
 
 coveo-functools = { version = "^2.0.0" }
 typing_extensions = "*"
 
 
 [tool.poetry.dev-dependencies]
+bandit = "*"
+black = "*"
 coveo-functools = { path = "../coveo-functools/", develop = true }
 coveo-testing = { path = "../coveo-testing/", develop = true }
+mypy = "0.950"
+pytest = "*"
 
 
 [tool.stew.ci]
 pytest = true
 offline-build = true
 black = true
```

### Comparing `coveo-systools-2.0.8a1/setup.py` & `coveo-systools-2.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['coveo-functools>=2.0.0,<3.0.0', 'typing_extensions']
 
 setup_kwargs = {
     'name': 'coveo-systools',
-    'version': '2.0.8a1',
+    'version': '2.0.9',
     'description': 'Filesystem, language and OS related tools.',
     'long_description': '# coveo-systools\n\nLanguage and OS related utilities.\n\n\nContent in a nutshell:\n\n- enhanced subprocess calls\n- asyncio subprocess calls\n- file and app finding made easy\n- safe text write and replace-if-different\n- git-repo-root locator\n- bool platforms `if WINDOWS or LINUX or MAC or WSL:`\n\n\n# searching the filesystem\n\n```python\nimport os\nfrom coveo_systools.filesystem import find_paths, find_application, find_repo_root\n\nos.getcwd()\n# \'/code/coveo-python-oss/coveo-systools\'\n\nfind_application(\'git\')\n# WindowsPath(\'C:/Program Files/Git/cmd/git.EXE\')  # windows example for completeness\n\nfind_repo_root()\n# Path(\'/code/coveo-python-oss\')\n\nlist(find_paths(\'pyproject.toml\', search_from=find_repo_root(), in_root=True, in_children=True))\n# [Path(\'/code/coveo-python-oss/pyproject.toml\'), ...]\n```\n\n# enhanced subprocess calls\n\nAn opinionated version of `subprocess.check_call` and `subprocess.check_output`.\n\n_New in 2.0.7_: asyncio support, through `async_check_call` and `async_check_output`.\n\nAdds the following features:\n- command line is a variable args (instead of a list)\n- automatic conversion of output to a stripped string (instead of raw bytes)\n- automatic conversion of Path, bytes and number variables in command line\n- automatic filtering of ansi codes from the output\n- enhanced DetailedCalledProcessError on error (a subclass of the typical CalledProcessError)\n\n```python\nfrom pathlib import Path\nfrom coveo_systools.subprocess import check_call\n\ncheck_call(\'mypy\', \'--config-file\', Path(\'configs/mypy.ini\'), verbose=True)\n```\n\n\n# safe I/O, if changed\n\nGood programming practices requires files to be saved using a temporary filename and then renamed.\nThis helper takes it a step further by skipping the write operation if the content did not change: \n\n```python\nimport json\nfrom pathlib import Path\nfrom coveo_systools.filesystem import safe_text_write\n\nsafe_text_write(Path(\'./path/to/file.txt\'), json.dumps(...), only_if_changed=True)\n```\n\n\n# conditional platforms syntactic sugar\n\nReadability is important, not repeating yourself is important.\nForget about `platform.platform()` and use bools directly:\n\n```python\nfrom coveo_systools.platforms import WINDOWS, LINUX, IOS, WSL\n\nif WINDOWS or WSL:\n    print("Hello Windows!")\nelif LINUX or IOS:\n    print("Hello Unix!")\n```\n',
     'author': 'Jonathan Piché',
     'author_email': 'tools@coveo.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/coveooss/coveo-python-oss/tree/main/coveo-systools',
```

### Comparing `coveo-systools-2.0.8a1/PKG-INFO` & `coveo-systools-2.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coveo-systools
-Version: 2.0.8a1
+Version: 2.0.9
 Summary: Filesystem, language and OS related tools.
 Home-page: https://github.com/coveooss/coveo-python-oss/tree/main/coveo-systools
 License: Apache-2.0
 Author: Jonathan Piché
 Author-email: tools@coveo.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: Apache Software License
```

