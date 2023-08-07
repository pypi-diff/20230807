# Comparing `tmp/committed-1.0.18.tar.gz` & `tmp/committed-1.0.20.tar.gz`

## Comparing `committed-1.0.18.tar` & `committed-1.0.20.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      427 1970-01-01 00:00:00.000000 committed-1.0.18/pyproject.toml
--rw-r--r--   0        0        0     2046 1970-01-01 00:00:00.000000 committed-1.0.18/rust_src/committed/Cargo.toml
--rw-r--r--   0     1001      123     9680 2023-05-22 20:09:31.000000 committed-1.0.18/rust_src/committed/src/checks.rs
--rw-r--r--   0     1001      123     1414 2023-05-22 20:09:31.000000 committed-1.0.18/rust_src/committed/src/color.rs
--rw-r--r--   0     1001      123     4614 2023-05-22 20:09:31.000000 committed-1.0.18/rust_src/committed/src/config.rs
--rw-r--r--   0     1001      123      461 2023-05-22 20:09:31.000000 committed-1.0.18/rust_src/committed/src/conventional.rs
--rw-r--r--   0     1001      123     1914 2023-05-22 20:09:31.000000 committed-1.0.18/rust_src/committed/src/git.rs
--rw-r--r--   0     1001      123      109 2023-05-22 20:09:31.000000 committed-1.0.18/rust_src/committed/src/lib.rs
--rw-r--r--   0     1001      123    13075 2023-05-22 20:09:31.000000 committed-1.0.18/rust_src/committed/src/main.rs
--rw-r--r--   0     1001      123     1764 2023-05-22 20:09:31.000000 committed-1.0.18/rust_src/committed/src/no_style.rs
--rw-r--r--   0     1001      123     5273 2023-05-22 20:09:31.000000 committed-1.0.18/rust_src/committed/src/report.rs
--rw-r--r--   0     1001      123      198 2023-05-22 20:09:31.000000 committed-1.0.18/rust_src/committed/src/style.rs
--rw-r--r--   0     1001      123    29692 2023-05-22 20:09:31.000000 committed-1.0.18/Cargo.lock
--rw-r--r--   0        0        0     2900 1970-01-01 00:00:00.000000 committed-1.0.18/PKG-INFO
+-rw-r--r--   0        0        0      427 1970-01-01 00:00:00.000000 committed-1.0.20/pyproject.toml
+-rw-r--r--   0        0        0     2046 1970-01-01 00:00:00.000000 committed-1.0.20/rust_src/committed/Cargo.toml
+-rw-r--r--   0     1001      123     9680 2023-08-07 21:33:01.000000 committed-1.0.20/rust_src/committed/src/checks.rs
+-rw-r--r--   0     1001      123     1414 2023-08-07 21:33:01.000000 committed-1.0.20/rust_src/committed/src/color.rs
+-rw-r--r--   0     1001      123     4614 2023-08-07 21:33:01.000000 committed-1.0.20/rust_src/committed/src/config.rs
+-rw-r--r--   0     1001      123      461 2023-08-07 21:33:01.000000 committed-1.0.20/rust_src/committed/src/conventional.rs
+-rw-r--r--   0     1001      123     1914 2023-08-07 21:33:01.000000 committed-1.0.20/rust_src/committed/src/git.rs
+-rw-r--r--   0     1001      123      109 2023-08-07 21:33:01.000000 committed-1.0.20/rust_src/committed/src/lib.rs
+-rw-r--r--   0     1001      123    13075 2023-08-07 21:33:01.000000 committed-1.0.20/rust_src/committed/src/main.rs
+-rw-r--r--   0     1001      123     1764 2023-08-07 21:33:01.000000 committed-1.0.20/rust_src/committed/src/no_style.rs
+-rw-r--r--   0     1001      123     5273 2023-08-07 21:33:01.000000 committed-1.0.20/rust_src/committed/src/report.rs
+-rw-r--r--   0     1001      123      198 2023-08-07 21:33:01.000000 committed-1.0.20/rust_src/committed/src/style.rs
+-rw-r--r--   0     1001      123    29930 2023-08-07 21:33:01.000000 committed-1.0.20/Cargo.lock
+-rw-r--r--   0        0        0     2900 1970-01-01 00:00:00.000000 committed-1.0.20/PKG-INFO
```

### Comparing `committed-1.0.18/rust_src/committed/Cargo.toml` & `committed-1.0.20/rust_src/committed/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [package]
 name = "committed"
-version = "1.0.18"
+version = "1.0.20"
 description = "Nitpicking commit history since beabf39"
 documentation = "https://docs.rs/committed"
 readme = "../../README.md"
 categories = ["development-tools", "text-processing"]
 keywords = ["development"]
 license= "MIT OR Apache-2.0"
 repository= "https://github.com/crate-ci/committed"
 edition= "2021"
-rust-version= "1.65.0"  # MSRV
+rust-version= "1.70.0"  # MSRV
 include= [
   "build.rs",
   "src/**/*",
   "Cargo.toml",
   "Cargo.lock",
   "LICENSE*",
   "README.md",
@@ -31,30 +31,30 @@
   {file="../../CHANGELOG.md", search="<!-- next-url -->", replace="<!-- next-url -->\n[Unreleased]: https://github.com/crate-ci/committed/compare/{{tag_name}}...HEAD", exactly=1},
   {file="../../action/entrypoint.sh", search="VERSION=.*", replace="VERSION={{version}}", min=1},
   {file="../../README.md", search="rev: .*", replace="rev: {{tag_name}}", exactly=1},
   {file="../../setup.py", search="COMMITTED_VERSION = .*", replace="COMMITTED_VERSION = '{{version}}'", exactly=1},
 ]
 
 [dependencies]
-regex = "1.7"
-once_cell = "1.17.1"
+regex = "1.8"
+once_cell = "1.17.2"
 git-conventional = "0.12"
 unicase = "2.6.0"
 anyhow = "1.0"
-git2 = { version = "0.16", default-features = false }
-clap = { version = "4.2", features = ["derive"] }
+git2 = { version = "0.17", default-features = false }
+clap = { version = "4.3", features = ["derive"] }
 serde = { version = "1.0", features = ["derive"] }
 serde_json = "1.0"
 toml = "0.7"
 unicode-segmentation = "1.10.1"
 log = "0.4"
 env_logger = "0.10"
 clap-verbosity-flag = "2.0"
 colorchoice-clap = "1.0.0"
 grep-cli = "0.1"
 imperative = "1.0.4"
 derive_more = "0.99.17"
 itertools = "0.10.5"
 proc-exit = "2.0"
-human-panic = "1.1.3"
-anstream = "0.3.0"
+human-panic = "1.1.4"
+anstream = "0.3.2"
 anstyle = "1.0.0"
```

### Comparing `committed-1.0.18/rust_src/committed/src/checks.rs` & `committed-1.0.20/rust_src/committed/src/checks.rs`

 * *Files identical despite different names*

### Comparing `committed-1.0.18/rust_src/committed/src/color.rs` & `committed-1.0.20/rust_src/committed/src/color.rs`

 * *Files identical despite different names*

### Comparing `committed-1.0.18/rust_src/committed/src/config.rs` & `committed-1.0.20/rust_src/committed/src/config.rs`

 * *Files identical despite different names*

### Comparing `committed-1.0.18/rust_src/committed/src/git.rs` & `committed-1.0.20/rust_src/committed/src/git.rs`

 * *Files identical despite different names*

### Comparing `committed-1.0.18/rust_src/committed/src/main.rs` & `committed-1.0.20/rust_src/committed/src/main.rs`

 * *Files identical despite different names*

### Comparing `committed-1.0.18/rust_src/committed/src/no_style.rs` & `committed-1.0.20/rust_src/committed/src/no_style.rs`

 * *Files identical despite different names*

### Comparing `committed-1.0.18/rust_src/committed/src/report.rs` & `committed-1.0.20/rust_src/committed/src/report.rs`

 * *Files identical despite different names*

### Comparing `committed-1.0.18/Cargo.lock` & `committed-1.0.20/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -23,18 +23,27 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cc936419f96fa211c1b9166887b38e5e40b19958e5b895be7c1f93adec7071ac"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
+name = "aho-corasick"
+version = "1.0.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "67fc08ce920c31afb70f013dcce1bfc3a3195de6a228474e45e1f145b36f8d04"
+dependencies = [
+ "memchr",
+]
+
+[[package]]
 name = "anstream"
-version = "0.3.0"
+version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9e579a7752471abc2a8268df8b20005e3eadd975f585398f17efcfd8d4927371"
+checksum = "0ca84f3628370c59db74ee214b3263d58f9aadd9b4fe7e711fd87dc452b7f163"
 dependencies = [
  "anstyle",
  "anstyle-parse",
  "anstyle-query",
  "anstyle-wincon",
  "colorchoice",
  "is-terminal",
@@ -63,17 +72,17 @@
 checksum = "5ca11d4be1bab0c8bc8734a9aa7bf4ee8316d462a08c6ac5052f888fef5b494b"
 dependencies = [
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "anstyle-wincon"
-version = "1.0.0"
+version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4bcd8291a340dd8ac70e18878bc4501dd7b4ff970cfa21c207d36ece51ea88fd"
+checksum = "180abfa45703aebe0093f79badacc01b8fd4ea2e35118747e5811127f926e188"
 dependencies = [
  "anstyle",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "anyhow"
@@ -144,17 +153,17 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "clap"
-version = "4.2.2"
+version = "4.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9b802d85aaf3a1cdb02b224ba472ebdea62014fccfcb269b95a4d76443b5ee5a"
+checksum = "93aae7a4192245f70fe75dd9157fc7b4a5bf53e88d30bd4396f7d8f9284d5acc"
 dependencies = [
  "clap_builder",
  "clap_derive",
  "once_cell",
 ]
 
 [[package]]
@@ -165,42 +174,42 @@
 dependencies = [
  "clap",
  "log",
 ]
 
 [[package]]
 name = "clap_builder"
-version = "4.2.2"
+version = "4.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "14a1a858f532119338887a4b8e1af9c60de8249cd7bafd68036a489e261e37b6"
+checksum = "4f423e341edefb78c9caba2d9c7f7687d0e72e89df3ce3394554754393ac3990"
 dependencies = [
  "anstream",
  "anstyle",
  "bitflags",
  "clap_lex",
  "strsim",
 ]
 
 [[package]]
 name = "clap_derive"
-version = "4.2.0"
+version = "4.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3f9644cd56d6b87dbe899ef8b053e331c0637664e9e21a33dfcdc36093f5c5c4"
+checksum = "191d9573962933b4027f932c600cd252ce27a8ad5979418fe78e43c07996f27b"
 dependencies = [
  "heck",
  "proc-macro2",
  "quote",
  "syn 2.0.12",
 ]
 
 [[package]]
 name = "clap_lex"
-version = "0.4.1"
+version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8a2dd5a6fe8c6e3502f568a6353e5273bbb15193ad9a89e457b9970798efbea1"
+checksum = "2da6da31387c7e4ef160ffab6d5e7f00c42626fe39aea70a7b0f1773f7dd6c1b"
 
 [[package]]
 name = "colorchoice"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "acbf1af155f9b9ef647e42cdc158db4b64a1b61f743629225fde6f3e0be2a7c7"
 
@@ -212,15 +221,15 @@
 dependencies = [
  "clap",
  "colorchoice",
 ]
 
 [[package]]
 name = "committed"
-version = "1.0.18"
+version = "1.0.20"
 dependencies = [
  "anstream",
  "anstyle",
  "anyhow",
  "clap",
  "clap-verbosity-flag",
  "colorchoice-clap",
@@ -349,32 +358,32 @@
  "doc-comment",
  "unicase",
  "winnow",
 ]
 
 [[package]]
 name = "git2"
-version = "0.16.1"
+version = "0.17.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ccf7f68c2995f392c49fffb4f95ae2c873297830eb25c6bc4c114ce8f4562acc"
+checksum = "7b989d6a7ca95a362cf2cfc5ad688b3a467be1f87e480b8dad07fee8c79b0044"
 dependencies = [
  "bitflags",
  "libc",
  "libgit2-sys",
  "log",
  "url",
 ]
 
 [[package]]
 name = "globset"
 version = "0.4.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "029d74589adefde59de1a0c4f4732695c32805624aec7b68d91503d4dba79afc"
 dependencies = [
- "aho-corasick",
+ "aho-corasick 0.7.20",
  "bstr",
  "fnv",
  "log",
  "regex",
 ]
 
 [[package]]
@@ -451,17 +460,17 @@
 dependencies = [
  "unicode-bidi",
  "unicode-normalization",
 ]
 
 [[package]]
 name = "imperative"
-version = "1.0.4"
+version = "1.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9f92123bf2fe0d9f1b5df1964727b970ca3b2d0203d47cf97fb1f36d856b6398"
+checksum = "8b70798296d538cdaa6d652941fcc795963f8b9878b9e300c9fab7a522bd2fc0"
 dependencies = [
  "phf",
  "rust-stemmers",
 ]
 
 [[package]]
 name = "indexmap"
@@ -529,17 +538,17 @@
 name = "libc"
 version = "0.2.140"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "99227334921fae1a979cf0bfdfcc6b3e5ce376ef57e16fb6fb3ea2ed6095f80c"
 
 [[package]]
 name = "libgit2-sys"
-version = "0.14.2+1.5.1"
+version = "0.15.2+1.6.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7f3d95f6b51075fe9810a7ae22c7095f12b98005ab364d8544797a825ce946a4"
+checksum = "a80df2e11fb4a61f4ba2ab42dbe7f74468da143f1a75c74e11dee7c813f694fa"
 dependencies = [
  "cc",
  "libc",
  "libz-sys",
  "pkg-config",
 ]
 
@@ -592,17 +601,17 @@
 checksum = "ea86265d3d3dcb6a27fc51bd29a4bf387fae9d2986b823079d4986af253eb439"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.17.1"
+version = "1.17.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b7e5500299e16ebb147ae15a00a942af264cf3688f47923b8fc2cd5858f23ad3"
+checksum = "9670a07f94779e00908f3e686eab508878ebb390ba6e604d3a284c00e8d0487b"
 
 [[package]]
 name = "os_info"
 version = "3.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5c424bc68d15e0778838ac013b5b3449544d8133633d8016319e7e05a820b8c0"
 dependencies = [
@@ -663,34 +672,34 @@
 checksum = "4424af4bf778aae2051a77b60283332f386554255d722233d09fbfc7e30da2fc"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "regex"
-version = "1.7.1"
+version = "1.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "48aaa5748ba571fb95cd2c85c09f629215d3a6ece942baa100950af03a34f733"
+checksum = "81ca098a9821bd52d6b24fd8b10bd081f47d39c22778cafaa75a2857a62c6390"
 dependencies = [
- "aho-corasick",
+ "aho-corasick 1.0.1",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-automata"
 version = "0.1.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6c230d73fb8d8c1b9c0b3135c5142a8acee3a0558fb8db5cf1cb65f8d7862132"
 
 [[package]]
 name = "regex-syntax"
-version = "0.6.28"
+version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "456c603be3e8d448b072f410900c09faf164fbce2d480456f50eea6e25f9c848"
+checksum = "436b050e76ed2903236f032a59761c1eb99e1b0aead2c257922771dab1fc8c78"
 
 [[package]]
 name = "rust-stemmers"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e46a2036019fdb888131db7a4c847a1063a7493f971ed94ea82c67eada63ca54"
 dependencies = [
```

### Comparing `committed-1.0.18/PKG-INFO` & `committed-1.0.20/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: committed
-Version: 1.0.18
+Version: 1.0.20
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Summary: Nitpicking commit history since beabf39
 Keywords: development
@@ -41,15 +41,15 @@
 
 To use `committed` with [`pre-commit`](https://pre-commit.com), point its
 config at this repository:
 
 ```yaml
 repos:
   - repo: https://github.com/crate-ci/committed
-    rev: v1.0.18
+    rev: v1.0.20
     hooks:
       - id: committed
 ```
 
 The `committed` id installs a prebuilt executable from GitHub releases. If
 one does not exist for the target platform, or if one built from
 sources is preferred, use `committed-src` as the hook id instead.
```

