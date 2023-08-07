# Comparing `tmp/qoqo_qasm-0.8.2.tar.gz` & `tmp/qoqo_qasm-0.8.3.tar.gz`

## Comparing `qoqo_qasm-0.8.2.tar` & `qoqo_qasm-0.8.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      862 1970-01-01 00:00:00.000000 qoqo_qasm-0.8.2/local_dependencies/roqoqo-qasm/Cargo.toml
--rw-r--r--   0     1001      123    11357 2023-08-01 10:04:12.000000 qoqo_qasm-0.8.2/local_dependencies/roqoqo-qasm/LICENSE
--rw-r--r--   0     1001      123     2621 2023-08-01 10:04:12.000000 qoqo_qasm-0.8.2/local_dependencies/roqoqo-qasm/README.md
--rw-r--r--   0     1001      123    11723 2023-08-01 10:04:12.000000 qoqo_qasm-0.8.2/local_dependencies/roqoqo-qasm/src/backend.rs
--rw-r--r--   0     1001      123      875 2023-08-01 10:04:12.000000 qoqo_qasm-0.8.2/local_dependencies/roqoqo-qasm/src/grammars/qasm2_0.pest
--rw-r--r--   0     1001      123    45054 2023-08-01 10:04:12.000000 qoqo_qasm-0.8.2/local_dependencies/roqoqo-qasm/src/interface.rs
--rw-r--r--   0     1001      123     1367 2023-08-01 10:04:12.000000 qoqo_qasm-0.8.2/local_dependencies/roqoqo-qasm/src/lib.rs
--rw-r--r--   0     1001      123    12539 2023-08-01 10:04:12.000000 qoqo_qasm-0.8.2/local_dependencies/roqoqo-qasm/src/parser.rs
--rw-r--r--   0        0        0     1172 1970-01-01 00:00:00.000000 qoqo_qasm-0.8.2/Cargo.toml
--rw-r--r--   0     1001      123    11357 2023-08-01 10:04:12.000000 qoqo_qasm-0.8.2/LICENSE
--rw-r--r--   0     1001      123     2621 2023-08-01 10:04:12.000000 qoqo_qasm-0.8.2/README.md
--rw-r--r--   0     1001      123      701 2023-08-01 10:04:12.000000 qoqo_qasm-0.8.2/build.rs
--rw-r--r--   0     1001      123      728 2023-08-01 10:04:12.000000 qoqo_qasm-0.8.2/pyproject.toml
--rw-r--r--   0     1001      123       87 2023-08-01 10:04:12.000000 qoqo_qasm-0.8.2/python_tests/README.md
--rw-r--r--   0     1001      123   955966 2023-08-01 10:04:12.000000 qoqo_qasm-0.8.2/qoqo_qasm/DEPENDENCIES
--rw-r--r--   0     1001      123      916 2023-08-01 10:04:12.000000 qoqo_qasm-0.8.2/qoqo_qasm/__init__.py
--rw-r--r--   0     1001      123     5419 2023-08-01 10:04:12.000000 qoqo_qasm-0.8.2/src/backend.rs
--rw-r--r--   0     1001      123     3707 2023-08-01 10:04:12.000000 qoqo_qasm-0.8.2/src/interface.rs
--rw-r--r--   0     1001      123     1796 2023-08-01 10:04:12.000000 qoqo_qasm-0.8.2/src/lib.rs
--rw-r--r--   0     1001      123     2134 2023-08-01 10:04:12.000000 qoqo_qasm-0.8.2/src/parser.rs
--rw-r--r--   0     1001      123    22960 2023-08-01 10:04:12.000000 qoqo_qasm-0.8.2/Cargo.lock
--rw-r--r--   0        0        0     3741 1970-01-01 00:00:00.000000 qoqo_qasm-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0      862 1970-01-01 00:00:00.000000 qoqo_qasm-0.8.3/local_dependencies/roqoqo-qasm/Cargo.toml
+-rw-r--r--   0     1001      123    11357 2023-08-07 10:53:50.000000 qoqo_qasm-0.8.3/local_dependencies/roqoqo-qasm/LICENSE
+-rw-r--r--   0     1001      123     2621 2023-08-07 10:53:50.000000 qoqo_qasm-0.8.3/local_dependencies/roqoqo-qasm/README.md
+-rw-r--r--   0     1001      123    11723 2023-08-07 10:53:50.000000 qoqo_qasm-0.8.3/local_dependencies/roqoqo-qasm/src/backend.rs
+-rw-r--r--   0     1001      123      875 2023-08-07 10:53:50.000000 qoqo_qasm-0.8.3/local_dependencies/roqoqo-qasm/src/grammars/qasm2_0.pest
+-rw-r--r--   0     1001      123    45920 2023-08-07 10:53:50.000000 qoqo_qasm-0.8.3/local_dependencies/roqoqo-qasm/src/interface.rs
+-rw-r--r--   0     1001      123     1367 2023-08-07 10:53:50.000000 qoqo_qasm-0.8.3/local_dependencies/roqoqo-qasm/src/lib.rs
+-rw-r--r--   0     1001      123    12539 2023-08-07 10:53:50.000000 qoqo_qasm-0.8.3/local_dependencies/roqoqo-qasm/src/parser.rs
+-rw-r--r--   0        0        0     1174 1970-01-01 00:00:00.000000 qoqo_qasm-0.8.3/Cargo.toml
+-rw-r--r--   0     1001      123    11357 2023-08-07 10:53:50.000000 qoqo_qasm-0.8.3/LICENSE
+-rw-r--r--   0     1001      123     2621 2023-08-07 10:53:50.000000 qoqo_qasm-0.8.3/README.md
+-rw-r--r--   0     1001      123      701 2023-08-07 10:53:50.000000 qoqo_qasm-0.8.3/build.rs
+-rw-r--r--   0     1001      123      728 2023-08-07 10:53:50.000000 qoqo_qasm-0.8.3/pyproject.toml
+-rw-r--r--   0     1001      123       87 2023-08-07 10:53:50.000000 qoqo_qasm-0.8.3/python_tests/README.md
+-rw-r--r--   0     1001      123   955966 2023-08-07 10:53:50.000000 qoqo_qasm-0.8.3/qoqo_qasm/DEPENDENCIES
+-rw-r--r--   0     1001      123      916 2023-08-07 10:53:50.000000 qoqo_qasm-0.8.3/qoqo_qasm/__init__.py
+-rw-r--r--   0     1001      123     5419 2023-08-07 10:53:50.000000 qoqo_qasm-0.8.3/src/backend.rs
+-rw-r--r--   0     1001      123     3707 2023-08-07 10:53:50.000000 qoqo_qasm-0.8.3/src/interface.rs
+-rw-r--r--   0     1001      123     1796 2023-08-07 10:53:50.000000 qoqo_qasm-0.8.3/src/lib.rs
+-rw-r--r--   0     1001      123     2134 2023-08-07 10:53:50.000000 qoqo_qasm-0.8.3/src/parser.rs
+-rw-r--r--   0     1001      123    22960 2023-08-07 10:53:50.000000 qoqo_qasm-0.8.3/Cargo.lock
+-rw-r--r--   0        0        0     3741 1970-01-01 00:00:00.000000 qoqo_qasm-0.8.3/PKG-INFO
```

### Comparing `qoqo_qasm-0.8.2/local_dependencies/roqoqo-qasm/Cargo.toml` & `qoqo_qasm-0.8.3/local_dependencies/roqoqo-qasm/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "roqoqo-qasm"
-version = "0.8.2"
+version = "0.8.3"
 authors = ["HQS Quantum Simulations <info@quantumsimulations.de>"]
 license = "Apache-2.0"
 edition = "2018"
 categories = ["science", "simulation"]
 readme = "README.md"
 repository = "https://github.com/HQSquantumsimulations/qoqo_qasm"
 description = "QASM interface for roqoqo rust quantum computing toolkit"
```

### Comparing `qoqo_qasm-0.8.2/local_dependencies/roqoqo-qasm/LICENSE` & `qoqo_qasm-0.8.3/local_dependencies/roqoqo-qasm/LICENSE`

 * *Files identical despite different names*

### Comparing `qoqo_qasm-0.8.2/local_dependencies/roqoqo-qasm/README.md` & `qoqo_qasm-0.8.3/local_dependencies/roqoqo-qasm/README.md`

 * *Files identical despite different names*

### Comparing `qoqo_qasm-0.8.2/local_dependencies/roqoqo-qasm/src/backend.rs` & `qoqo_qasm-0.8.3/local_dependencies/roqoqo-qasm/src/backend.rs`

 * *Files identical despite different names*

### Comparing `qoqo_qasm-0.8.2/local_dependencies/roqoqo-qasm/src/grammars/qasm2_0.pest` & `qoqo_qasm-0.8.3/local_dependencies/roqoqo-qasm/src/grammars/qasm2_0.pest`

 * *Files identical despite different names*

### Comparing `qoqo_qasm-0.8.2/local_dependencies/roqoqo-qasm/src/interface.rs` & `qoqo_qasm-0.8.3/local_dependencies/roqoqo-qasm/src/interface.rs`

 * *Files 1% similar despite different names*

```diff
@@ -32,25 +32,26 @@
     "PragmaStopDecompositionBlock",
     "PragmaStopParallelBlock",
     "InputSymbolic",
     "PragmaGlobalPhase",
 ];
 
 // Operations that are ignored when looking for a QASM definition
-const NO_DEFINITION_REQUIRED_OPERATIONS: &[&str; 10] = &[
+const NO_DEFINITION_REQUIRED_OPERATIONS: &[&str; 11] = &[
     "SingleQubitGate",
     "DefinitionFloat",
     "DefinitionUsize",
     "DefinitionBit",
     "DefinitionComplex",
     "PragmaActiveReset",
     "PragmaConditional",
     "PragmaGlobalPhase",
     "PragmaRepeatedMeasurement",
     "MeasureQubit",
+    "PragmaLoop",
 ];
 
 /// Translate the qoqo circuit into QASM ouput.
 ///
 /// The qoqo_qasm interface iterates through the qoqo circuit and translates each qoqo operation
 /// to QASM output (strings).
 ///
@@ -669,24 +670,21 @@
                         backend: "QASM",
                         hqslang: operation.hqslang(),
                     })
                 }
             }
         },
         Operation::PragmaLoop(op) => match qasm_version {
-            QasmVersion::V2point0 => Err(RoqoqoBackendError::GenericError {
-                msg: "PragmaLoop not allowed with qasm_version 2.0".to_string(),
-            }),
             QasmVersion::V3point0(Qasm3Dialect::Roqoqo) => Ok(format!(
                 "pragma roqoqo {} {} {};",
                 op.hqslang(),
                 op.repetitions(),
                 op.circuit()
             )),
-            QasmVersion::V3point0(_) => {
+            QasmVersion::V3point0(Qasm3Dialect::Vanilla) => {
                 let mut data = "".to_string();
                 match op.repetitions() {
                     CalculatorFloat::Float(x) => {
                         data.push_str(format!("for uint i in [0:{x}] {{\n").as_str());
                         let circuit_vec = match call_circuit(op.circuit(), qubit_register_name, qasm_version) {
                             Ok(vec_str) => vec_str,
                             Err(x) => return Err(x)
@@ -696,14 +694,33 @@
                         }
                         data.push_str("\n}");
                         Ok(data)
                     },
                     CalculatorFloat::Str(x) => Err(RoqoqoBackendError::GenericError { msg: format!("Used PragmaLoop with a string {x} for repetitions and a qasm-version that is incompatible: {qasm_version:?}") })
                 }
             }
+            _ => {
+                let mut data = "".to_string();
+                match op.repetitions() {
+                    CalculatorFloat::Float(x) => {
+                        for _ in 0_usize..(*x as usize) {
+                            let circuit_vec = match call_circuit(op.circuit(), qubit_register_name, qasm_version) {
+                                Ok(vec_str) => vec_str,
+                                Err(x) => return Err(x)
+                            };
+                            for string in circuit_vec {
+                                data.push_str(string.as_str());
+                                data.push('\n');
+                            }
+                        }
+                        Ok(data)
+                    },
+                    CalculatorFloat::Str(x) => Err(RoqoqoBackendError::GenericError { msg: format!("Used PragmaLoop with a string {x} for repetitions and a qasm-version that is incompatible: {qasm_version:?}") })
+                }
+            }
         },
         Operation::PragmaOverrotation(op) => match qasm_version {
             QasmVersion::V3point0(Qasm3Dialect::Roqoqo) => Ok(format!(
                 "pragma roqoqo {} {} {:?} {} {};",
                 op.hqslang(),
                 op.gate_hqslang(),
                 op.qubits(),
```

### Comparing `qoqo_qasm-0.8.2/local_dependencies/roqoqo-qasm/src/lib.rs` & `qoqo_qasm-0.8.3/local_dependencies/roqoqo-qasm/src/lib.rs`

 * *Files identical despite different names*

### Comparing `qoqo_qasm-0.8.2/local_dependencies/roqoqo-qasm/src/parser.rs` & `qoqo_qasm-0.8.3/local_dependencies/roqoqo-qasm/src/parser.rs`

 * *Files identical despite different names*

### Comparing `qoqo_qasm-0.8.2/Cargo.toml` & `qoqo_qasm-0.8.3/Cargo.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "qoqo_qasm"
-version = "0.8.2"
+version = "0.8.3"
 authors = ["HQS Quantum Simulations <info@quantumsimulations.de>"]
 license = "Apache-2.0"
 edition = "2018"
 categories = ["science", "simulation"]
 readme = "README.md"
 homepage = "https://github.com/HQSquantumsimulations/qoqo_qasm"
 repository = "https://github.com/HQSquantumsimulations/qoqo_qasm"
@@ -25,15 +25,15 @@
 crate-type = ["cdylib", "rlib"]
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [dependencies]
 qoqo = { version = "1.5.1", default-features = false }
 roqoqo = { version = "1.5.1", features = ["serialize"] }
-roqoqo-qasm = { version = "0.8", path = "local_dependencies/roqoqo-qasm" }
+roqoqo-qasm = { version = "0.8.3", path = "local_dependencies/roqoqo-qasm" }
 
 [dependencies.pyo3]
 version = "0.19"
 features = ["num-complex"]
 
 [build-dependencies]
 pyo3-build-config = "0.19"
```

### Comparing `qoqo_qasm-0.8.2/LICENSE` & `qoqo_qasm-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `qoqo_qasm-0.8.2/README.md` & `qoqo_qasm-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `qoqo_qasm-0.8.2/build.rs` & `qoqo_qasm-0.8.3/build.rs`

 * *Files identical despite different names*

### Comparing `qoqo_qasm-0.8.2/qoqo_qasm/DEPENDENCIES` & `qoqo_qasm-0.8.3/qoqo_qasm/DEPENDENCIES`

 * *Files 0% similar despite different names*

```diff
@@ -30602,15 +30602,15 @@
 00077890: 7369 6f6e 7320 616e 640a 2020 206c 696d  sions and.   lim
 000778a0: 6974 6174 696f 6e73 2075 6e64 6572 2074  itations under t
 000778b0: 6865 204c 6963 656e 7365 2e0a 0a0a 3d3d  he License....==
 000778c0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 000778d0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 000778e0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 000778f0: 3d3d 0a71 6f71 6f5f 7161 736d 2030 2e38  ==.qoqo_qasm 0.8
-00077900: 2e32 0a68 7474 7073 3a2f 2f67 6974 6875  .2.https://githu
+00077900: 2e33 0a68 7474 7073 3a2f 2f67 6974 6875  .3.https://githu
 00077910: 622e 636f 6d2f 4851 5371 7561 6e74 756d  b.com/HQSquantum
 00077920: 7369 6d75 6c61 7469 6f6e 732f 716f 716f  simulations/qoqo
 00077930: 5f71 6173 6d0a 6279 2048 5153 2051 7561  _qasm.by HQS Qua
 00077940: 6e74 756d 2053 696d 756c 6174 696f 6e73  ntum Simulations
 00077950: 203c 696e 666f 4071 7561 6e74 756d 7369   <info@quantumsi
 00077960: 6d75 6c61 7469 6f6e 732e 6465 3e0a 5079  mulations.de>.Py
 00077970: 7468 6f6e 2069 6e74 6572 6661 6365 206f  thon interface o
@@ -37277,15 +37277,15 @@
 000919c0: 6720 7065 726d 6973 7369 6f6e 7320 616e  g permissions an
 000919d0: 640a 2020 206c 696d 6974 6174 696f 6e73  d.   limitations
 000919e0: 2075 6e64 6572 2074 6865 204c 6963 656e   under the Licen
 000919f0: 7365 2e0a 0a0a 3d3d 3d3d 3d3d 3d3d 3d3d  se....==========
 00091a00: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00091a10: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00091a20: 3d3d 3d3d 3d3d 3d3d 3d3d 0a72 6f71 6f71  ==========.roqoq
-00091a30: 6f2d 7161 736d 2030 2e38 2e32 0a68 7474  o-qasm 0.8.2.htt
+00091a30: 6f2d 7161 736d 2030 2e38 2e33 0a68 7474  o-qasm 0.8.3.htt
 00091a40: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
 00091a50: 4851 5371 7561 6e74 756d 7369 6d75 6c61  HQSquantumsimula
 00091a60: 7469 6f6e 732f 716f 716f 5f71 6173 6d0a  tions/qoqo_qasm.
 00091a70: 6279 2048 5153 2051 7561 6e74 756d 2053  by HQS Quantum S
 00091a80: 696d 756c 6174 696f 6e73 203c 696e 666f  imulations <info
 00091a90: 4071 7561 6e74 756d 7369 6d75 6c61 7469  @quantumsimulati
 00091aa0: 6f6e 732e 6465 3e0a 5141 534d 2069 6e74  ons.de>.QASM int
```

### Comparing `qoqo_qasm-0.8.2/qoqo_qasm/__init__.py` & `qoqo_qasm-0.8.3/qoqo_qasm/__init__.py`

 * *Files identical despite different names*

### Comparing `qoqo_qasm-0.8.2/src/backend.rs` & `qoqo_qasm-0.8.3/src/backend.rs`

 * *Files identical despite different names*

### Comparing `qoqo_qasm-0.8.2/src/interface.rs` & `qoqo_qasm-0.8.3/src/interface.rs`

 * *Files identical despite different names*

### Comparing `qoqo_qasm-0.8.2/src/lib.rs` & `qoqo_qasm-0.8.3/src/lib.rs`

 * *Files identical despite different names*

### Comparing `qoqo_qasm-0.8.2/src/parser.rs` & `qoqo_qasm-0.8.3/src/parser.rs`

 * *Files identical despite different names*

### Comparing `qoqo_qasm-0.8.2/Cargo.lock` & `qoqo_qasm-0.8.3/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -524,15 +524,15 @@
  "qoqo_calculator",
  "serde",
  "thiserror",
 ]
 
 [[package]]
 name = "qoqo_qasm"
-version = "0.8.2"
+version = "0.8.3"
 dependencies = [
  "ndarray",
  "pyo3",
  "pyo3-build-config",
  "qoqo",
  "qoqo_calculator",
  "roqoqo",
@@ -635,15 +635,15 @@
  "proc-macro2",
  "quote",
  "syn 2.0.28",
 ]
 
 [[package]]
 name = "roqoqo-qasm"
-version = "0.8.2"
+version = "0.8.3"
 dependencies = [
  "ndarray",
  "num-complex",
  "pest",
  "pest_derive",
  "qoqo_calculator",
  "roqoqo",
```

### Comparing `qoqo_qasm-0.8.2/PKG-INFO` & `qoqo_qasm-0.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qoqo_qasm
-Version: 0.8.2
+Version: 0.8.3
 Requires-Dist: qoqo >=1.5
 Requires-Dist: qoqo_calculator_pyo3 >=1.1
 Requires-Dist: tomli ; extra == 'docs'
 Requires-Dist: numpy ; extra == 'docs'
 Requires-Dist: sphinx >=2.1 ; extra == 'docs'
 Requires-Dist: nbsphinx ; extra == 'docs'
 Requires-Dist: pygments ; extra == 'docs'
```

