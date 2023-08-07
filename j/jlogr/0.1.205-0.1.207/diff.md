# Comparing `tmp/jlogr-0.1.205.tar.gz` & `tmp/jlogr-0.1.207.tar.gz`

## Comparing `jlogr-0.1.205.tar` & `jlogr-0.1.207.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      484 1970-01-01 00:00:00.000000 jlogr-0.1.205/Cargo.toml
--rw-r--r--   0     1001      123      583 2023-08-07 15:29:15.000000 jlogr-0.1.205/.github/workflows/publish.yml
--rw-r--r--   0     1001      123       42 2023-08-07 15:29:15.000000 jlogr-0.1.205/.gitignore
--rw-r--r--   0     1001      123     1062 2023-08-07 15:29:15.000000 jlogr-0.1.205/LICENSE
--rw-r--r--   0     1001      123      123 2023-08-07 15:29:15.000000 jlogr-0.1.205/README.md
--rw-r--r--   0     1001      123       92 2023-08-07 15:29:15.000000 jlogr-0.1.205/package/jlogr/__init__.py
--rw-r--r--   0     1001      123      570 2023-08-07 15:29:15.000000 jlogr-0.1.205/package/jlogr/jlogr.pyi
--rw-r--r--   0     1001      123        0 2023-08-07 15:29:15.000000 jlogr-0.1.205/package/jlogr/py.typed
--rw-r--r--   0     1001      123      255 2023-08-07 15:29:15.000000 jlogr-0.1.205/pyproject.toml
--rw-r--r--   0     1001      123     4532 2023-08-07 15:29:15.000000 jlogr-0.1.205/src/lib.rs
--rw-r--r--   0     1001      123     2244 2023-08-07 15:29:15.000000 jlogr-0.1.205/src/structures/logger.rs
--rw-r--r--   0     1001      123     4763 2023-08-07 15:29:15.000000 jlogr-0.1.205/src/structures/logging.rs
--rw-r--r--   0     1001      123       33 2023-08-07 15:29:15.000000 jlogr-0.1.205/src/structures/mod.rs
--rw-r--r--   0     1001      123    13668 2023-08-07 15:29:19.000000 jlogr-0.1.205/Cargo.lock
--rw-r--r--   0        0        0      267 1970-01-01 00:00:00.000000 jlogr-0.1.205/PKG-INFO
+-rw-r--r--   0        0        0      503 1970-01-01 00:00:00.000000 jlogr-0.1.207/Cargo.toml
+-rw-r--r--   0     1001      123      583 2023-08-07 16:37:24.000000 jlogr-0.1.207/.github/workflows/publish.yml
+-rw-r--r--   0     1001      123       42 2023-08-07 16:37:24.000000 jlogr-0.1.207/.gitignore
+-rw-r--r--   0     1001      123     1062 2023-08-07 16:37:24.000000 jlogr-0.1.207/LICENSE
+-rw-r--r--   0     1001      123      123 2023-08-07 16:37:24.000000 jlogr-0.1.207/README.md
+-rw-r--r--   0     1001      123       94 2023-08-07 16:37:24.000000 jlogr-0.1.207/package/jlogr/__init__.py
+-rw-r--r--   0     1001      123      569 2023-08-07 16:37:24.000000 jlogr-0.1.207/package/jlogr/jlogr.pyi
+-rw-r--r--   0     1001      123        0 2023-08-07 16:37:24.000000 jlogr-0.1.207/package/jlogr/py.typed
+-rw-r--r--   0     1001      123      256 2023-08-07 16:37:24.000000 jlogr-0.1.207/pyproject.toml
+-rw-r--r--   0     1001      123     4621 2023-08-07 16:37:24.000000 jlogr-0.1.207/src/lib.rs
+-rw-r--r--   0     1001      123     2301 2023-08-07 16:37:24.000000 jlogr-0.1.207/src/structures/logger.rs
+-rw-r--r--   0     1001      123     4875 2023-08-07 16:37:24.000000 jlogr-0.1.207/src/structures/logging.rs
+-rw-r--r--   0     1001      123       33 2023-08-07 16:37:24.000000 jlogr-0.1.207/src/structures/mod.rs
+-rw-r--r--   0     1001      123    13690 2023-08-07 16:37:28.000000 jlogr-0.1.207/Cargo.lock
+-rw-r--r--   0        0        0      267 1970-01-01 00:00:00.000000 jlogr-0.1.207/PKG-INFO
```

### Comparing `jlogr-0.1.205/.github/workflows/publish.yml` & `jlogr-0.1.207/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `jlogr-0.1.205/LICENSE` & `jlogr-0.1.207/LICENSE`

 * *Files identical despite different names*

### Comparing `jlogr-0.1.205/package/jlogr/jlogr.pyi` & `jlogr-0.1.207/package/jlogr/jlogr.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ..jlogr import (
+from .jlogr import (
         info as _info,
         debug as _debug,
         warning as _warning,
         error as _error,
         parse_list_of_logs as _parse_list_of_logs
         )
```

### Comparing `jlogr-0.1.205/src/lib.rs` & `jlogr-0.1.207/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 pub mod structures;
 use pyo3::prelude::*;
+use structures::logger::Logger;
 use structures::logging::Log;
 
 #[pymodule]
 #[pyo3(name = "jlogr")]
 #[doc = "
 Module for clean and colourful logging in python
 This is just how i like my logs, so there aren't formatting options or anything like that.
@@ -12,14 +13,16 @@
 pub fn jlogr(_py: Python<'_>, m: &PyModule) -> PyResult<()> {
     m.add("__version__", env!("CARGO_PKG_VERSION"))?;
     m.add_function(wrap_pyfunction!(info, m)?)?;
     m.add_function(wrap_pyfunction!(debug, m)?)?;
     m.add_function(wrap_pyfunction!(warning, m)?)?;
     m.add_function(wrap_pyfunction!(error, m)?)?;
     m.add_function(wrap_pyfunction!(parse_list_of_logs, m)?)?;
+    m.add_class::<Logger>()?;
+    m.add_class::<Log>()?;
     Ok(())
 }
 
 #[pyfunction]
 #[doc = "
 Log a info message
```

### Comparing `jlogr-0.1.205/src/structures/logger.rs` & `jlogr-0.1.207/src/structures/logger.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 use crate::structures::logging::Log;
+use pyo3::prelude::*;
 use std::{fs, io::Write};
 
 /// Handles reading and writing of logs to the file system.
 /// Keeps a buffer of logs in memory, but can dump to file.
+#[pyclass]
 pub struct Logger {
     pub logs_path: String,
     pub logs_buffer: Vec<Log>,
 }
 
+#[pymethods]
 impl Logger {
+    #[new]
     pub fn new(logs_path: String) -> Logger {
         Logger {
             logs_path,
             logs_buffer: Vec::new(),
         }
     }
```

### Comparing `jlogr-0.1.205/src/structures/logging.rs` & `jlogr-0.1.207/src/structures/logging.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 use chrono::{DateTime, Local};
+use pyo3::prelude::*;
 use std::fmt::Display;
 use std::io::Write;
 use termcolor::{Color, ColorChoice, ColorSpec, StandardStream, WriteColor};
 
+#[pyclass]
 pub struct Log {
     pub created_at: DateTime<Local>,
     pub message: String,
     pub level: LogLevel,
     pub module: Option<String>,
     pub function: Option<String>,
     pub class: Option<String>,
 }
 
+#[pymethods]
 impl Log {
+    #[new]
     pub fn new(
         message: &str,
         level: &str,
         module: Option<&str>,
         function: Option<&str>,
         class: Option<&str>,
     ) -> Self {
@@ -26,14 +30,15 @@
             level: LogLevel::from(level),
             module: module.map(|m| m.to_string()),
             function: function.map(|f| f.to_string()),
             class: class.map(|c| c.to_string()),
         }
     }
 
+    #[staticmethod]
     pub fn from_log_string(log_string: &str) -> Self {
         let mut log = Log::new("", "", None, None, None);
         let mut split = log_string.split(" :: ");
         log.created_at = DateTime::parse_from_rfc3339(split.next().expect("spit to have a next"))
             .expect("datetime parse to work")
             .with_timezone(&Local);
         log.level = LogLevel::from_log_string(split.next().unwrap());
@@ -100,14 +105,16 @@
                 e.to_string()
             );
         });
         Ok(())
     }
 }
 
+#[derive(Debug, Clone)]
+#[pyclass]
 pub enum LogLevel {
     Info,
     Debug,
     Warning,
     Error,
 }
```

### Comparing `jlogr-0.1.205/Cargo.lock` & `jlogr-0.1.207/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,15 @@
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "jlogr"
-version = "0.1.205"
+version = "0.1.207"
 dependencies = [
  "anyhow",
  "chrono",
  "pyo3",
  "termcolor",
 ]
 
@@ -205,15 +205,17 @@
 
 [[package]]
 name = "pyo3"
 version = "0.19.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e681a6cfdc4adcc93b4d3cf993749a4552018ee0a9b65fc0ccfad74352c72a38"
 dependencies = [
+ "anyhow",
  "cfg-if",
+ "chrono",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
```

