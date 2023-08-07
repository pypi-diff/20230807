# Comparing `tmp/jlogr-0.1.204.tar.gz` & `tmp/jlogr-0.1.205.tar.gz`

## Comparing `jlogr-0.1.204.tar` & `jlogr-0.1.205.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      484 1970-01-01 00:00:00.000000 jlogr-0.1.204/Cargo.toml
--rw-r--r--   0     1001      123      583 2023-08-06 14:20:26.000000 jlogr-0.1.204/.github/workflows/publish.yml
--rw-r--r--   0     1001      123       42 2023-08-06 14:20:26.000000 jlogr-0.1.204/.gitignore
--rw-r--r--   0     1001      123     1062 2023-08-06 14:20:26.000000 jlogr-0.1.204/LICENSE
--rw-r--r--   0     1001      123      123 2023-08-06 14:20:26.000000 jlogr-0.1.204/README.md
--rw-r--r--   0     1001      123       92 2023-08-06 14:20:26.000000 jlogr-0.1.204/package/jlogr/__init__.py
--rw-r--r--   0     1001      123      565 2023-08-06 14:20:26.000000 jlogr-0.1.204/package/jlogr/jlogr.pyi
--rw-r--r--   0     1001      123        0 2023-08-06 14:20:26.000000 jlogr-0.1.204/package/jlogr/py.typed
--rw-r--r--   0     1001      123      255 2023-08-06 14:20:26.000000 jlogr-0.1.204/pyproject.toml
--rw-r--r--   0     1001      123     4532 2023-08-06 14:20:26.000000 jlogr-0.1.204/src/lib.rs
--rw-r--r--   0     1001      123     2244 2023-08-06 14:20:26.000000 jlogr-0.1.204/src/structures/logger.rs
--rw-r--r--   0     1001      123     4763 2023-08-06 14:20:26.000000 jlogr-0.1.204/src/structures/logging.rs
--rw-r--r--   0     1001      123       33 2023-08-06 14:20:26.000000 jlogr-0.1.204/src/structures/mod.rs
--rw-r--r--   0     1001      123    13668 2023-08-06 14:20:30.000000 jlogr-0.1.204/Cargo.lock
--rw-r--r--   0        0        0      267 1970-01-01 00:00:00.000000 jlogr-0.1.204/PKG-INFO
+-rw-r--r--   0        0        0      484 1970-01-01 00:00:00.000000 jlogr-0.1.205/Cargo.toml
+-rw-r--r--   0     1001      123      583 2023-08-07 15:29:15.000000 jlogr-0.1.205/.github/workflows/publish.yml
+-rw-r--r--   0     1001      123       42 2023-08-07 15:29:15.000000 jlogr-0.1.205/.gitignore
+-rw-r--r--   0     1001      123     1062 2023-08-07 15:29:15.000000 jlogr-0.1.205/LICENSE
+-rw-r--r--   0     1001      123      123 2023-08-07 15:29:15.000000 jlogr-0.1.205/README.md
+-rw-r--r--   0     1001      123       92 2023-08-07 15:29:15.000000 jlogr-0.1.205/package/jlogr/__init__.py
+-rw-r--r--   0     1001      123      570 2023-08-07 15:29:15.000000 jlogr-0.1.205/package/jlogr/jlogr.pyi
+-rw-r--r--   0     1001      123        0 2023-08-07 15:29:15.000000 jlogr-0.1.205/package/jlogr/py.typed
+-rw-r--r--   0     1001      123      255 2023-08-07 15:29:15.000000 jlogr-0.1.205/pyproject.toml
+-rw-r--r--   0     1001      123     4532 2023-08-07 15:29:15.000000 jlogr-0.1.205/src/lib.rs
+-rw-r--r--   0     1001      123     2244 2023-08-07 15:29:15.000000 jlogr-0.1.205/src/structures/logger.rs
+-rw-r--r--   0     1001      123     4763 2023-08-07 15:29:15.000000 jlogr-0.1.205/src/structures/logging.rs
+-rw-r--r--   0     1001      123       33 2023-08-07 15:29:15.000000 jlogr-0.1.205/src/structures/mod.rs
+-rw-r--r--   0     1001      123    13668 2023-08-07 15:29:19.000000 jlogr-0.1.205/Cargo.lock
+-rw-r--r--   0        0        0      267 1970-01-01 00:00:00.000000 jlogr-0.1.205/PKG-INFO
```

### Comparing `jlogr-0.1.204/.github/workflows/publish.yml` & `jlogr-0.1.205/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `jlogr-0.1.204/LICENSE` & `jlogr-0.1.205/LICENSE`

 * *Files identical despite different names*

### Comparing `jlogr-0.1.204/package/jlogr/jlogr.pyi` & `jlogr-0.1.205/package/jlogr/jlogr.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-from .jlogr import (
+from ..jlogr import (
         info as _info,
         debug as _debug,
         warning as _warning,
         error as _error,
         parse_list_of_logs as _parse_list_of_logs
         )
 
 from typing import Optional
 
 __all__ = ["info", "debug", "warning", "error", "parse_list_of_logs"]
 
-def info(message: str) -> None: ...
+def info(message: str) -> None:
+    ...
 
 def debug(message: str) -> None: ...
 
 def warning(message: str) -> None: ...
 
 def error(message: str) -> None: ...
```

### Comparing `jlogr-0.1.204/src/lib.rs` & `jlogr-0.1.205/src/lib.rs`

 * *Files identical despite different names*

### Comparing `jlogr-0.1.204/src/structures/logger.rs` & `jlogr-0.1.205/src/structures/logger.rs`

 * *Files identical despite different names*

### Comparing `jlogr-0.1.204/src/structures/logging.rs` & `jlogr-0.1.205/src/structures/logging.rs`

 * *Files identical despite different names*

### Comparing `jlogr-0.1.204/Cargo.lock` & `jlogr-0.1.205/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -39,17 +39,17 @@
 name = "bumpalo"
 version = "3.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a3e2c3daef883ecc1b5d58c15adae93470a91d425f3532ba1695849656af3fc1"
 
 [[package]]
 name = "cc"
-version = "1.0.81"
+version = "1.0.82"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6c6b2562119bf28c3439f7f02db99faf0aa1a8cdfe5772a2ee155d32227239f0"
+checksum = "305fe645edc1442a0fa8b6726ba61d422798d37a52e12eaecf4b022ebbb88f01"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
@@ -104,15 +104,15 @@
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "jlogr"
-version = "0.1.204"
+version = "0.1.205"
 dependencies = [
  "anyhow",
  "chrono",
  "pyo3",
  "termcolor",
 ]
```

