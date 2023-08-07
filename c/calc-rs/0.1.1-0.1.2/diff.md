# Comparing `tmp/calc_rs-0.1.1.tar.gz` & `tmp/calc_rs-0.1.2.tar.gz`

## Comparing `calc_rs-0.1.1.tar` & `calc_rs-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      301 1970-01-01 00:00:00.000000 calc_rs-0.1.1/local_dependencies/calc_rs/Cargo.toml
--rw-r--r--   0     1001      123     1279 2023-08-06 05:18:28.000000 calc_rs-0.1.1/local_dependencies/calc_rs/src/ast.rs
--rw-r--r--   0     1001      123     2854 2023-08-06 05:18:28.000000 calc_rs-0.1.1/local_dependencies/calc_rs/src/compiler/interpreter.rs
--rw-r--r--   0     1001      123       52 2023-08-06 05:18:28.000000 calc_rs-0.1.1/local_dependencies/calc_rs/src/compiler/mod.rs
--rw-r--r--   0     1001      123      654 2023-08-06 05:18:28.000000 calc_rs-0.1.1/local_dependencies/calc_rs/src/grammar.pest
--rw-r--r--   0     1001      123     5379 2023-08-06 05:18:28.000000 calc_rs-0.1.1/local_dependencies/calc_rs/src/lib.rs
--rw-r--r--   0     1001      123     2916 2023-08-06 05:18:28.000000 calc_rs-0.1.1/local_dependencies/calc_rs/src/parser.rs
--rw-r--r--   0        0        0      435 1970-01-01 00:00:00.000000 calc_rs-0.1.1/Cargo.toml
--rw-r--r--   0     1001      123     2944 2023-08-06 05:18:28.000000 calc_rs-0.1.1/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      567 2023-08-06 05:18:28.000000 calc_rs-0.1.1/.github/workflows/test.yml
--rw-r--r--   0     1001      123      696 2023-08-06 05:18:28.000000 calc_rs-0.1.1/.gitignore
--rw-r--r--   0     1001      123     1068 2023-08-06 05:18:28.000000 calc_rs-0.1.1/LICENSE
--rw-r--r--   0     1001      123     1576 2023-08-06 05:18:28.000000 calc_rs-0.1.1/README.md
--rw-r--r--   0     1001      123      182 2023-08-06 05:18:28.000000 calc_rs-0.1.1/TODO.md
--rw-r--r--   0     1001      123      398 2023-08-06 05:18:28.000000 calc_rs-0.1.1/pyproject.toml
--rw-r--r--   0     1001      123     3285 2023-08-06 05:18:28.000000 calc_rs-0.1.1/src/lib.rs
--rw-r--r--   0     1001      123     4836 2023-08-06 05:18:28.000000 calc_rs-0.1.1/test/calculator.py
--rwxr-xr-x   0     1001      123      558 2023-08-06 05:18:28.000000 calc_rs-0.1.1/test/speed-test.sh
--rw-r--r--   0     1001      123    15325 2023-08-06 05:18:38.000000 calc_rs-0.1.1/Cargo.lock
--rw-r--r--   0        0        0     1924 1970-01-01 00:00:00.000000 calc_rs-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      413 1970-01-01 00:00:00.000000 calc_rs-0.1.2/local_dependencies/calc_rs/Cargo.toml
+-rw-r--r--   0     1001      123     1420 2023-08-07 16:24:01.000000 calc_rs-0.1.2/local_dependencies/calc_rs/src/ast.rs
+-rw-r--r--   0     1001      123     4073 2023-08-07 16:24:01.000000 calc_rs-0.1.2/local_dependencies/calc_rs/src/compiler/interpreter.rs
+-rw-r--r--   0     1001      123       52 2023-08-07 16:24:01.000000 calc_rs-0.1.2/local_dependencies/calc_rs/src/compiler/mod.rs
+-rw-r--r--   0     1001      123      827 2023-08-07 16:24:01.000000 calc_rs-0.1.2/local_dependencies/calc_rs/src/grammar.pest
+-rw-r--r--   0     1001      123     7102 2023-08-07 16:24:01.000000 calc_rs-0.1.2/local_dependencies/calc_rs/src/lib.rs
+-rw-r--r--   0     1001      123     3069 2023-08-07 16:24:01.000000 calc_rs-0.1.2/local_dependencies/calc_rs/src/parser.rs
+-rw-r--r--   0        0        0      435 1970-01-01 00:00:00.000000 calc_rs-0.1.2/Cargo.toml
+-rw-r--r--   0     1001      123     2944 2023-08-07 16:24:01.000000 calc_rs-0.1.2/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      567 2023-08-07 16:24:01.000000 calc_rs-0.1.2/.github/workflows/test.yml
+-rw-r--r--   0     1001      123      696 2023-08-07 16:24:01.000000 calc_rs-0.1.2/.gitignore
+-rw-r--r--   0     1001      123     1068 2023-08-07 16:24:01.000000 calc_rs-0.1.2/LICENSE
+-rw-r--r--   0     1001      123     1576 2023-08-07 16:24:01.000000 calc_rs-0.1.2/README.md
+-rw-r--r--   0     1001      123      214 2023-08-07 16:24:01.000000 calc_rs-0.1.2/TODO.md
+-rw-r--r--   0     1001      123      398 2023-08-07 16:24:01.000000 calc_rs-0.1.2/pyproject.toml
+-rw-r--r--   0     1001      123     3285 2023-08-07 16:24:01.000000 calc_rs-0.1.2/src/lib.rs
+-rw-r--r--   0     1001      123     4836 2023-08-07 16:24:01.000000 calc_rs-0.1.2/test/calculator.py
+-rwxr-xr-x   0     1001      123      558 2023-08-07 16:24:01.000000 calc_rs-0.1.2/test/speed-test.sh
+-rw-r--r--   0     1001      123    21387 2023-08-07 16:24:05.000000 calc_rs-0.1.2/Cargo.lock
+-rw-r--r--   0        0        0     1924 1970-01-01 00:00:00.000000 calc_rs-0.1.2/PKG-INFO
```

### Comparing `calc_rs-0.1.1/local_dependencies/calc_rs/src/ast.rs` & `calc_rs-0.1.2/local_dependencies/calc_rs/src/ast.rs`

 * *Files 5% similar despite different names*

```diff
@@ -7,31 +7,34 @@
     Plus,
     Minus,
     Multiply,
     Divide,
     Exponent,
     Negative,
     Modulo,
+    Riemann,
 }
 
 impl fmt::Display for Operator {
     fn fmt(&self, f: &mut fmt::Formatter<'_>) -> Result<(), fmt::Error> {
         match &self {
             Operator::Plus => write!(f, "+"),
             Operator::Minus | Operator::Negative => write!(f, "-"),
             Operator::Multiply => write!(f, "*"),
             Operator::Divide => write!(f, "/"),
             Operator::Exponent => write!(f, "^"),
             Operator::Modulo => write!(f, "%"),
+            Operator::Riemann => write!(f, "∑"),
         }
     }
 }
 
 #[derive(Debug, Clone, PartialEq, PartialOrd)]
 pub enum Node {
+    Range(String),
     Var(String),
     Num(Number),
     UnaryExpr(Box<Node>),
     BinaryExpr {
         op: Operator,
         lhs: Box<Node>,
         rhs: Box<Node>,
@@ -41,10 +44,11 @@
 impl fmt::Display for Node {
     fn fmt(&self, f: &mut fmt::Formatter<'_>) -> Result<(), fmt::Error> {
         match &self {
             Node::Num(n) => write!(f, "{}", n),
             Node::UnaryExpr(expr) => write!(f, "{}", expr),
             Node::BinaryExpr { op, lhs, rhs } => write!(f, "{} {} {}", lhs, op, rhs),
             Node::Var(var_name) => write!(f, "{}", var_name),
+            Node::Range(range) => write!(f, "{}", range),
         }
     }
 }
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `calc_rs-0.1.1/local_dependencies/calc_rs/src/parser.rs` & `calc_rs-0.1.2/local_dependencies/calc_rs/src/parser.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #![allow(clippy::upper_case_acronyms)]
-
 use crate::ast::{Node, Operator};
 use crate::Result;
+use crate::{debug, info};
 use lazy_static::lazy_static;
 use pest::iterators::Pairs;
 use pest::pratt_parser::PrattParser;
 use pest::{self, Parser};
 
 #[derive(pest_derive::Parser)]
 #[grammar = "grammar.pest"]
@@ -16,19 +16,20 @@
         use pest::pratt_parser::{Assoc::*, Op};
         use Rule::*;
 
         PrattParser::new()
             .op(Op::infix(add, Left) | Op::infix(subtract, Left))
             .op(Op::infix(multiply, Left) | Op::infix(divide, Left) | Op::infix(modulo, Left))
             .op(Op::infix(power, Right))
+            .op(Op::infix(riemann, Left))
     };
 }
 
 fn parse_expr(pairs: Pairs<Rule>, pratt_parser: &PRATT_PARSER) -> Node {
-    // println!("pairs -> {:?}", pairs);
+    debug!("pairs -> {:?}", pairs);
 
     pratt_parser
         .map_primary(|primary| match primary.as_rule() {
             Rule::expr => parse_expr(primary.into_inner(), pratt_parser),
             Rule::num => Node::Num(primary.as_str().parse::<f64>().unwrap()),
             Rule::negative => Node::BinaryExpr {
                 op: Operator::Multiply,
@@ -36,47 +37,49 @@
                 rhs: Box::new(parse_expr(primary.into_inner(), pratt_parser)),
             },
             Rule::unary_minus => Node::UnaryExpr(Box::new(parse_expr(
                 primary.clone().into_inner(),
                 pratt_parser,
             ))),
             Rule::var => Node::Var(primary.as_str().to_string()),
+            Rule::range => Node::Range(primary.as_str().to_string()),
             rule => unreachable!("Expr::parse expected atom, found {:?}", rule),
         })
         .map_infix(|lhs, op, rhs| {
             let op = match op.as_rule() {
                 Rule::add => Operator::Plus,
                 Rule::subtract => Operator::Minus,
                 Rule::multiply => Operator::Multiply,
                 Rule::divide => Operator::Divide,
                 Rule::power => Operator::Exponent,
                 Rule::unary_minus => Operator::Negative,
                 Rule::modulo => Operator::Modulo,
+                Rule::riemann => Operator::Riemann,
                 rule => unreachable!("Expr::parse expected infix operation, found {:?}", rule),
             };
-            // println!("infix => {}{}{}", lhs, op, rhs);
+            debug!("infix => {}{}{}", lhs, op, rhs);
             Node::BinaryExpr {
                 lhs: Box::new(lhs),
                 op,
                 rhs: Box::new(rhs),
             }
         })
         .map_prefix(|op, rhs| {
-            // println!("prefix => {} {}", op, rhs);
+            debug!("prefix => {} {}", op, rhs);
             match op.as_rule() {
                 Rule::unary_minus => Node::UnaryExpr(Box::new(rhs)),
                 _ => unreachable!(),
             }
         })
         .parse(pairs)
 }
 
 pub fn parse(source: &str) -> Result<Node> {
     let tokens = CalcParser::parse(Rule::equation, source)?;
-    // println!("tokens  => {:?}", tokens);
-    // println!("source  => {:?}", source);
+    debug!("tokens  => {:?}", tokens);
+    info!("source  => {:?}", source);
     let parsed = parse_expr(tokens, &PRATT_PARSER);
-    // println!("parsed  => {:?}", parsed);
-    // println!();
+    info!("parsed  => {:?}", parsed);
+    info!("");
 
     Ok(parsed)
 }
```

### Comparing `calc_rs-0.1.1/.github/workflows/CI.yml` & `calc_rs-0.1.2/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `calc_rs-0.1.1/.github/workflows/test.yml` & `calc_rs-0.1.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `calc_rs-0.1.1/.gitignore` & `calc_rs-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `calc_rs-0.1.1/LICENSE` & `calc_rs-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `calc_rs-0.1.1/README.md` & `calc_rs-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `calc_rs-0.1.1/src/lib.rs` & `calc_rs-0.1.2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `calc_rs-0.1.1/test/calculator.py` & `calc_rs-0.1.2/test/calculator.py`

 * *Files identical despite different names*

### Comparing `calc_rs-0.1.1/test/speed-test.sh` & `calc_rs-0.1.2/test/speed-test.sh`

 * *Files identical despite different names*

### Comparing `calc_rs-0.1.1/Cargo.lock` & `calc_rs-0.1.2/Cargo.lock`

 * *Files 18% similar despite different names*

```diff
@@ -20,50 +20,78 @@
 [[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
+name = "bitflags"
+version = "2.3.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "630be753d4e58660abd17930c71b647fe46c27ea6b63cc59e1e3851406972e42"
+
+[[package]]
 name = "block-buffer"
 version = "0.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3078c7629b62d3f0439517fa394996acacc5cbc91c5a20d8c658e77abd503a71"
 dependencies = [
  "generic-array",
 ]
 
 [[package]]
 name = "calc_rs"
-version = "0.1.1"
+version = "0.1.2"
 dependencies = [
  "eyre",
  "lazy_static",
+ "log",
  "pest",
  "pest_derive",
  "rayon",
  "regex",
+ "simple_logger",
 ]
 
 [[package]]
 name = "calculators"
-version = "0.1.1"
+version = "0.1.2"
 dependencies = [
  "calc_rs",
  "eyre",
  "pyo3",
 ]
 
 [[package]]
+name = "cc"
+version = "1.0.82"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "305fe645edc1442a0fa8b6726ba61d422798d37a52e12eaecf4b022ebbb88f01"
+dependencies = [
+ "libc",
+]
+
+[[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
+name = "colored"
+version = "2.0.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2674ec482fbc38012cf31e6c42ba0177b431a0cb6f15fe40efa5aab1bda516f6"
+dependencies = [
+ "is-terminal",
+ "lazy_static",
+ "windows-sys 0.48.0",
+]
+
+[[package]]
 name = "cpufeatures"
 version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a17b76ff3a4162b0b27f354a0c87015ddad39d35f9c0c36607a3bdd175dde1f1"
 dependencies = [
  "libc",
 ]
@@ -118,14 +146,20 @@
 checksum = "1bfb12502f3fc46cca1bb51ac28df9d618d813cdc3d2f25b9fe775a34af26bb3"
 dependencies = [
  "generic-array",
  "typenum",
 ]
 
 [[package]]
+name = "deranged"
+version = "0.3.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7684a49fb1af197853ef7b2ee694bc1f5b4179556f1e5710e1760c5db6f5e929"
+
+[[package]]
 name = "digest"
 version = "0.10.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9ed9a281f7bc9b7576e61468ba615a66a5c8cfdff42420a70aa82701a3b1e292"
 dependencies = [
  "block-buffer",
  "crypto-common",
@@ -134,14 +168,35 @@
 [[package]]
 name = "either"
 version = "1.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a26ae43d7bcc3b814de94796a5e736d4029efb0ee900c12e2d54c993ad1a1e07"
 
 [[package]]
+name = "errno"
+version = "0.3.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6b30f669a7961ef1631673d2766cc92f52d64f7ef354d4fe0ddfd30ed52f0f4f"
+dependencies = [
+ "errno-dragonfly",
+ "libc",
+ "windows-sys 0.48.0",
+]
+
+[[package]]
+name = "errno-dragonfly"
+version = "0.1.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "aa68f1b12764fab894d2755d2518754e71b4fd80ecfb822714a1206c2aab39bf"
+dependencies = [
+ "cc",
+ "libc",
+]
+
+[[package]]
 name = "eyre"
 version = "0.6.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4c2b6b5a29c02cdc822728b7d7b8ae1bab3e3b05d44522770ddd49722eeac7eb"
 dependencies = [
  "indenter",
  "once_cell",
@@ -172,36 +227,65 @@
 [[package]]
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
+name = "is-terminal"
+version = "0.4.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "cb0889898416213fab133e1d33a0e5858a48177452750691bde3666d0fdbaf8b"
+dependencies = [
+ "hermit-abi",
+ "rustix",
+ "windows-sys 0.48.0",
+]
+
+[[package]]
+name = "itoa"
+version = "1.0.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "af150ab688ff2122fcef229be89cb50dd66af9e01a4ff320cc137eecc9bacc38"
+
+[[package]]
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
 version = "0.2.147"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b4668fb0ea861c1df094127ac5f1da3409a82116a4ba74fca2e58ef927159bb3"
 
 [[package]]
+name = "linux-raw-sys"
+version = "0.4.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "57bcfdad1b858c2db7c38303a6d2ad4dfaf5eb53dfeb0910128b2c26d6158503"
+
+[[package]]
 name = "lock_api"
 version = "0.4.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c1cc9717a20b1bb222f333e6a92fd32f7d8a18ddc5a3191a11af45dcbf4dcd16"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
+name = "log"
+version = "0.4.19"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b06a4cde4c0f271a446782e3eff8de789548ce57dbc8eca9292c27f4a42004b4"
+
+[[package]]
 name = "memchr"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2dffe52ecf27772e601905b7522cb4ef790d2cc203488bbd0e2fe85fcb74566d"
 
 [[package]]
 name = "memoffset"
@@ -219,14 +303,23 @@
 checksum = "4161fcb6d602d4d2081af7c3a45852d875a03dd337a6bfdd6e06407b61342a43"
 dependencies = [
  "hermit-abi",
  "libc",
 ]
 
 [[package]]
+name = "num_threads"
+version = "0.1.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2819ce041d2ee131036f4fc9d6ae7ae125a3a40e97ba64d04fe799ad9dabbb44"
+dependencies = [
+ "libc",
+]
+
+[[package]]
 name = "once_cell"
 version = "1.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
 
 [[package]]
 name = "parking_lot"
@@ -398,15 +491,15 @@
 
 [[package]]
 name = "redox_syscall"
 version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
 dependencies = [
- "bitflags",
+ "bitflags 1.3.2",
 ]
 
 [[package]]
 name = "regex"
 version = "1.9.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "81bc1d4caf89fac26a70747fe603c130093b53c773888797a6329091246d651a"
@@ -431,31 +524,62 @@
 [[package]]
 name = "regex-syntax"
 version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e5ea92a5b6195c6ef2a0295ea818b312502c6fc94dde986c5553242e18fd4ce2"
 
 [[package]]
+name = "rustix"
+version = "0.38.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "172891ebdceb05aa0005f533a6cbfca599ddd7d966f6f5d4d9b2e70478e70399"
+dependencies = [
+ "bitflags 2.3.3",
+ "errno",
+ "libc",
+ "linux-raw-sys",
+ "windows-sys 0.48.0",
+]
+
+[[package]]
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
+name = "serde"
+version = "1.0.183"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "32ac8da02677876d532745a130fc9d8e6edfa81a269b107c5b00829b91d8eb3c"
+
+[[package]]
 name = "sha2"
 version = "0.10.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "479fb9d862239e610720565ca91403019f2f00410f1864c5aa7479b950a76ed8"
 dependencies = [
  "cfg-if",
  "cpufeatures",
  "digest",
 ]
 
 [[package]]
+name = "simple_logger"
+version = "4.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2230cd5c29b815c9b699fb610b49a5ed65588f3509d9f0108be3a885da629333"
+dependencies = [
+ "colored",
+ "log",
+ "time",
+ "windows-sys 0.42.0",
+]
+
+[[package]]
 name = "smallvec"
 version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "62bb4feee49fdd9f707ef802e22365a35de4b7b299de4763d44bfea899442ff9"
 
 [[package]]
 name = "syn"
@@ -502,14 +626,44 @@
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.28",
 ]
 
 [[package]]
+name = "time"
+version = "0.3.25"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b0fdd63d58b18d663fbdf70e049f00a22c8e42be082203be7f26589213cd75ea"
+dependencies = [
+ "deranged",
+ "itoa",
+ "libc",
+ "num_threads",
+ "serde",
+ "time-core",
+ "time-macros",
+]
+
+[[package]]
+name = "time-core"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7300fbefb4dadc1af235a9cef3737cea692a9d97e1b9cbcd4ebdae6f8868e6fb"
+
+[[package]]
+name = "time-macros"
+version = "0.2.11"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "eb71511c991639bb078fd5bf97757e03914361c48100d52878b8e52b46fb92cd"
+dependencies = [
+ "time-core",
+]
+
+[[package]]
 name = "typenum"
 version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "497961ef93d974e23eb6f433eb5fe1b7930b659f06d12dec6fc44a8f554c0bba"
 
 [[package]]
 name = "ucd-trie"
@@ -532,62 +686,128 @@
 [[package]]
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
 
 [[package]]
+name = "windows-sys"
+version = "0.42.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5a3e1820f08b8513f676f7ab6c1f99ff312fb97b553d30ff4dd86f9f15728aa7"
+dependencies = [
+ "windows_aarch64_gnullvm 0.42.2",
+ "windows_aarch64_msvc 0.42.2",
+ "windows_i686_gnu 0.42.2",
+ "windows_i686_msvc 0.42.2",
+ "windows_x86_64_gnu 0.42.2",
+ "windows_x86_64_gnullvm 0.42.2",
+ "windows_x86_64_msvc 0.42.2",
+]
+
+[[package]]
+name = "windows-sys"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
+dependencies = [
+ "windows-targets",
+]
+
+[[package]]
 name = "windows-targets"
 version = "0.48.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "05d4b17490f70499f20b9e791dcf6a299785ce8af4d709018206dc5b4953e95f"
 dependencies = [
- "windows_aarch64_gnullvm",
- "windows_aarch64_msvc",
- "windows_i686_gnu",
- "windows_i686_msvc",
- "windows_x86_64_gnu",
- "windows_x86_64_gnullvm",
- "windows_x86_64_msvc",
+ "windows_aarch64_gnullvm 0.48.0",
+ "windows_aarch64_msvc 0.48.0",
+ "windows_i686_gnu 0.48.0",
+ "windows_i686_msvc 0.48.0",
+ "windows_x86_64_gnu 0.48.0",
+ "windows_x86_64_gnullvm 0.48.0",
+ "windows_x86_64_msvc 0.48.0",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
+version = "0.42.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "597a5118570b68bc08d8d59125332c54f1ba9d9adeedeef5b99b02ba2b0698f8"
+
+[[package]]
+name = "windows_aarch64_gnullvm"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
+version = "0.42.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e08e8864a60f06ef0d0ff4ba04124db8b0fb3be5776a5cd47641e942e58c4d43"
+
+[[package]]
+name = "windows_aarch64_msvc"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
 
 [[package]]
 name = "windows_i686_gnu"
+version = "0.42.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c61d927d8da41da96a81f029489353e68739737d3beca43145c8afec9a31a84f"
+
+[[package]]
+name = "windows_i686_gnu"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
 
 [[package]]
 name = "windows_i686_msvc"
+version = "0.42.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "44d840b6ec649f480a41c8d80f9c65108b92d89345dd94027bfe06ac444d1060"
+
+[[package]]
+name = "windows_i686_msvc"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
 
 [[package]]
 name = "windows_x86_64_gnu"
+version = "0.42.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8de912b8b8feb55c064867cf047dda097f92d51efad5b491dfb98f6bbb70cb36"
+
+[[package]]
+name = "windows_x86_64_gnu"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
+version = "0.42.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "26d41b46a36d453748aedef1486d5c7a85db22e56aff34643984ea85514e94a3"
+
+[[package]]
+name = "windows_x86_64_gnullvm"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
 
 [[package]]
 name = "windows_x86_64_msvc"
+version = "0.42.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
+
+[[package]]
+name = "windows_x86_64_msvc"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
```

### Comparing `calc_rs-0.1.1/PKG-INFO` & `calc_rs-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calc-rs
-Version: 0.1.1
+Version: 0.1.2
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
```

