# Comparing `tmp/nova_python-0.1.3.tar.gz` & `tmp/nova_python-0.1.4.tar.gz`

## Comparing `nova_python-0.1.3.tar` & `nova_python-0.1.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      361 1970-01-01 00:00:00.000000 nova_python-0.1.3/Cargo.toml
--rwxrwxrwx   0     1000      998      945 2023-08-07 12:42:57.000000 nova_python-0.1.3/.gitignore
--rwxrwxrwx   0     1000      998    35184 2023-08-07 12:42:57.000000 nova_python-0.1.3/LICENSE
--rwxrwxrwx   0     1000      998     2368 2023-08-07 14:14:30.000000 nova_python-0.1.3/README.md
--rwxrwxrwx   0     1000      998      563 2023-08-07 12:42:57.000000 nova_python-0.1.3/pyproject.toml
--rwxrwxrwx   0     1000      998     7741 2023-08-07 14:02:42.000000 nova_python-0.1.3/src/lib.rs
--rwxrwxrwx   0     1000      998    30445 2023-08-07 14:01:36.000000 nova_python-0.1.3/Cargo.lock
--rw-r--r--   0        0        0     2877 1970-01-01 00:00:00.000000 nova_python-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      406 1970-01-01 00:00:00.000000 nova_python-0.1.4/Cargo.toml
+-rwxrwxrwx   0     1000      998      955 2023-08-07 15:11:48.000000 nova_python-0.1.4/.gitignore
+-rwxrwxrwx   0     1000      998    35184 2023-08-07 12:42:57.000000 nova_python-0.1.4/LICENSE
+-rwxrwxrwx   0     1000      998     2368 2023-08-07 14:14:30.000000 nova_python-0.1.4/README.md
+-rwxrwxrwx   0     1000      998      563 2023-08-07 12:42:57.000000 nova_python-0.1.4/pyproject.toml
+-rwxrwxrwx   0     1000      998     7741 2023-08-07 14:02:42.000000 nova_python-0.1.4/src/lib.rs
+-rwxrwxrwx   0     1000      998    30445 2023-08-07 15:33:30.000000 nova_python-0.1.4/Cargo.lock
+-rw-r--r--   0        0        0     2877 1970-01-01 00:00:00.000000 nova_python-0.1.4/PKG-INFO
```

### Comparing `nova_python-0.1.3/.gitignore` & `nova_python-0.1.4/.gitignore`

 * *Files 18% similar despite different names*

```diff
@@ -91,8 +91,10 @@
 *.out
 *.egg-info
 extensions/stamps/
 pip-wheel-metadata
 valgrind-python.supp
 *.pyd
 lcov.info
-netlify_build/
+netlify_build/
+
+build.sh
```

### Comparing `nova_python-0.1.3/LICENSE` & `nova_python-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nova_python-0.1.3/README.md` & `nova_python-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `nova_python-0.1.3/pyproject.toml` & `nova_python-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nova_python-0.1.3/src/lib.rs` & `nova_python-0.1.4/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nova_python-0.1.3/Cargo.lock` & `nova_python-0.1.4/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -450,15 +450,15 @@
  "security-framework",
  "security-framework-sys",
  "tempfile",
 ]
 
 [[package]]
 name = "nova-python"
-version = "0.1.3"
+version = "0.1.4"
 dependencies = [
  "pyo3",
  "reqwest",
  "serde_json",
  "tokio",
 ]
```

### Comparing `nova_python-0.1.3/PKG-INFO` & `nova_python-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nova-python
-Version: 0.1.3
+Version: 0.1.4
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: 🐍 Python library for accessing the Nova API
 Author: Leander <@henceiusegentoo>
 Requires-Python: >=3.7
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nova-python Version: 0.1.3 Classifier: Programming
+Metadata-Version: 2.1 Name: nova-python Version: 0.1.4 Classifier: Programming
 Language :: Rust Classifier: Programming Language :: Python :: Implementation
 :: CPython Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE Summary: ð Python library for accessing the Nova API
 Author: Leander <@henceiusegentoo> Requires-Python: >=3.7 Description-Content-
 Type: text/markdown; charset=UTF-8; variant=GFM Project-URL: Repo, https://
 github.com/henceiusegentoo/nova-python # nova-python ð Python library for
 accessing the Nova API ## Usage ## Install the module (This requires Cargo)
```

