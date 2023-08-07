# Comparing `tmp/rusty_chrono-0.1.3.tar.gz` & `tmp/rusty_chrono-0.1.4.tar.gz`

## Comparing `rusty_chrono-0.1.3.tar` & `rusty_chrono-0.1.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      316 1970-01-01 00:00:00.000000 rusty_chrono-0.1.3/Cargo.toml
--rw-r--r--   0     1001      123     2793 2023-08-01 23:44:33.000000 rusty_chrono-0.1.3/.github/workflows/maturin_build.yml
--rw-r--r--   0     1001      123     5297 2023-08-01 23:44:33.000000 rusty_chrono-0.1.3/.gitignore
--rw-r--r--   0     1001      123     1890 2023-08-01 23:44:33.000000 rusty_chrono-0.1.3/.gitlab-ci.yml.old
--rw-r--r--   0     1001      123      886 2023-08-01 23:44:33.000000 rusty_chrono-0.1.3/Dockerfile
--rw-r--r--   0     1001      123     1067 2023-08-01 23:44:33.000000 rusty_chrono-0.1.3/LICENSE
--rw-r--r--   0     1001      123       22 2023-08-01 23:44:33.000000 rusty_chrono-0.1.3/README.md
--rw-r--r--   0     1001      123       70 2023-08-01 23:44:33.000000 rusty_chrono-0.1.3/build.rs
--rw-r--r--   0     1001      123     1751 2023-08-01 23:44:33.000000 rusty_chrono-0.1.3/publish_script.py
--rw-r--r--   0     1001      123      335 2023-08-01 23:44:33.000000 rusty_chrono-0.1.3/pyproject.toml
--rw-r--r--   0     1001      123     1386 2023-08-01 23:44:33.000000 rusty_chrono-0.1.3/src/dateutil/date_errors.rs
--rw-r--r--   0     1001      123     1122 2023-08-01 23:44:33.000000 rusty_chrono-0.1.3/src/dateutil/date_functions.rs
--rw-r--r--   0     1001      123     1649 2023-08-01 23:44:33.000000 rusty_chrono-0.1.3/src/dateutil/date_parsing.rs
--rw-r--r--   0     1001      123     5731 2023-08-01 23:44:33.000000 rusty_chrono-0.1.3/src/dateutil/dateutil_tests/date_functions_tests.rs
--rw-r--r--   0     1001      123     3068 2023-08-01 23:44:33.000000 rusty_chrono-0.1.3/src/dateutil/dateutil_tests/date_parsing_tests.rs
--rw-r--r--   0     1001      123       75 2023-08-01 23:44:33.000000 rusty_chrono-0.1.3/src/dateutil/dateutil_tests/mod.rs
--rw-r--r--   0     1001      123      124 2023-08-01 23:44:33.000000 rusty_chrono-0.1.3/src/dateutil/mod.rs
--rw-r--r--   0     1001      123      550 2023-08-01 23:44:33.000000 rusty_chrono-0.1.3/src/dateutil/time_fractions.rs
--rw-r--r--   0     1001      123     2849 2023-08-01 23:44:33.000000 rusty_chrono-0.1.3/src/lib.rs
--rw-r--r--   0     1001      123      661 2023-08-01 23:44:33.000000 rusty_chrono-0.1.3/test.py
--rw-r--r--   0     1001      123    14607 2023-08-01 23:44:38.000000 rusty_chrono-0.1.3/Cargo.lock
--rw-r--r--   0        0        0      324 1970-01-01 00:00:00.000000 rusty_chrono-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      317 1970-01-01 00:00:00.000000 rusty_chrono-0.1.4/Cargo.toml
+-rw-r--r--   0     1001      123     4016 2023-08-07 19:05:46.000000 rusty_chrono-0.1.4/.github/workflows/maturin_build.yml
+-rw-r--r--   0     1001      123     5297 2023-08-07 19:05:46.000000 rusty_chrono-0.1.4/.gitignore
+-rw-r--r--   0     1001      123     1897 2023-08-07 19:05:46.000000 rusty_chrono-0.1.4/.gitlab-ci.yml.old
+-rw-r--r--   0     1001      123      886 2023-08-07 19:05:46.000000 rusty_chrono-0.1.4/Dockerfile
+-rw-r--r--   0     1001      123     1067 2023-08-07 19:05:46.000000 rusty_chrono-0.1.4/LICENSE
+-rw-r--r--   0     1001      123       22 2023-08-07 19:05:46.000000 rusty_chrono-0.1.4/README.md
+-rw-r--r--   0     1001      123       70 2023-08-07 19:05:46.000000 rusty_chrono-0.1.4/build.rs
+-rw-r--r--   0     1001      123      335 2023-08-07 19:05:46.000000 rusty_chrono-0.1.4/pyproject.toml
+-rw-r--r--   0     1001      123     1386 2023-08-07 19:05:46.000000 rusty_chrono-0.1.4/src/dateutil/date_errors.rs
+-rw-r--r--   0     1001      123     1122 2023-08-07 19:05:46.000000 rusty_chrono-0.1.4/src/dateutil/date_functions.rs
+-rw-r--r--   0     1001      123     1649 2023-08-07 19:05:46.000000 rusty_chrono-0.1.4/src/dateutil/date_parsing.rs
+-rw-r--r--   0     1001      123     5731 2023-08-07 19:05:46.000000 rusty_chrono-0.1.4/src/dateutil/dateutil_tests/date_functions_tests.rs
+-rw-r--r--   0     1001      123     3068 2023-08-07 19:05:46.000000 rusty_chrono-0.1.4/src/dateutil/dateutil_tests/date_parsing_tests.rs
+-rw-r--r--   0     1001      123       75 2023-08-07 19:05:46.000000 rusty_chrono-0.1.4/src/dateutil/dateutil_tests/mod.rs
+-rw-r--r--   0     1001      123      124 2023-08-07 19:05:46.000000 rusty_chrono-0.1.4/src/dateutil/mod.rs
+-rw-r--r--   0     1001      123      550 2023-08-07 19:05:46.000000 rusty_chrono-0.1.4/src/dateutil/time_fractions.rs
+-rw-r--r--   0     1001      123     2849 2023-08-07 19:05:46.000000 rusty_chrono-0.1.4/src/lib.rs
+-rw-r--r--   0     1001      123      661 2023-08-07 19:05:46.000000 rusty_chrono-0.1.4/test.py
+-rw-r--r--   0     1001      123     1751 2023-08-07 19:05:46.000000 rusty_chrono-0.1.4/version_update_script.py
+-rw-r--r--   0     1001      123    14635 2023-08-07 19:05:53.000000 rusty_chrono-0.1.4/Cargo.lock
+-rw-r--r--   0        0        0      324 1970-01-01 00:00:00.000000 rusty_chrono-0.1.4/PKG-INFO
```

### Comparing `rusty_chrono-0.1.3/.github/workflows/maturin_build.yml` & `rusty_chrono-0.1.4/.github/workflows/maturin_build.yml`

 * *Files 23% similar despite different names*

```diff
@@ -1,61 +1,93 @@
 # This file is autogenerated by maturin v1.1.0
 # To update, run
 #
 #    maturin generate-ci github
 #
-name: CI
+name: Test and Build CI
 
 on:
   push:
     branches:
       - main
     tags:
       - '*'
   pull_request:
   workflow_dispatch:
 
 permissions:
-  contents: read
+  contents: write
 
 jobs:
+  rust_tests:
+    runs-on: ubuntu-latest
+    steps:
+      - uses: actions/checkout@v3
+      - uses: actions/setup-python@v4
+        with:
+          python-version: '3.11'
+      - name: Running Tests
+        run: cargo test --verbose
+      - run: ls -al 
+      - name: Updating Package Version
+        run: |
+          pip install toml requests
+          python version_update_script.py
+      - name: Uploading Cargo config as Artifact
+        uses: actions/upload-artifact@v3
+        with:
+          name: Cargo Version
+          path: Cargo.toml
+          retention-days: 1
+
   linux:
     runs-on: ubuntu-latest
     strategy:
       matrix:
         target: [x86_64, x86, aarch64, armv7, s390x, ppc64le]
+    needs: [rust_tests]
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v4
         with:
           python-version: '3.11'
+      - name: Download Cargo Config Artifact
+        uses: actions/download-artifact@v3
+        with:
+          name: Cargo Version
       - name: Build wheels
         uses: PyO3/maturin-action@v1
         with:
           target: ${{ matrix.target }}
           args: --release --out dist --find-interpreter
           sccache: 'true'
           manylinux: auto
       - name: Upload wheels
         uses: actions/upload-artifact@v3
         with:
           name: wheels
           path: dist
+      
 
   windows:
     runs-on: windows-latest
     strategy:
       matrix:
         target: [x64, x86]
+    needs: [rust_tests]
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v4
         with:
           python-version: '3.11'
           architecture: ${{ matrix.target }}
+      - name: Download Cargo Config Artifact
+        uses: actions/download-artifact@v3
+        with:
+          name: Cargo Version
       - name: Build wheels
         uses: PyO3/maturin-action@v1
         with:
           target: ${{ matrix.target }}
           args: --release --out dist --find-interpreter
           sccache: 'true'
       - name: Upload wheels
@@ -65,55 +97,65 @@
           path: dist
 
   macos:
     runs-on: macos-latest
     strategy:
       matrix:
         target: [x86_64, aarch64]
+    needs: [rust_tests]
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v4
         with:
-          python-version: '3.10'
+          python-version: '3.11'
+      - name: Download Cargo Config Artifact
+        uses: actions/download-artifact@v3
+        with:
+          name: Cargo Version
       - name: Build wheels
         uses: PyO3/maturin-action@v1
         with:
           target: ${{ matrix.target }}
           args: --release --out dist --find-interpreter
           sccache: 'true'
       - name: Upload wheels
         uses: actions/upload-artifact@v3
         with:
           name: wheels
           path: dist
 
   sdist:
     runs-on: ubuntu-latest
+    needs: [rust_tests]
     steps:
       - uses: actions/checkout@v3
+      - name: Download Cargo Config Artifact
+        uses: actions/download-artifact@v3
+        with:
+          name: Cargo Version
       - name: Build sdist
         uses: PyO3/maturin-action@v1
         with:
           command: sdist
           args: --out dist
       - name: Upload sdist
         uses: actions/upload-artifact@v3
         with:
           name: wheels
           path: dist
 
   release:
     name: Release
     runs-on: ubuntu-latest
-    #if: "startsWith(github.ref, 'refs/tags/')"
+    # if: "startsWith(github.ref, 'refs/tags/')"
     needs: [linux, windows, macos, sdist]
     steps:
       - uses: actions/download-artifact@v3
         with:
           name: wheels
       - name: Publish to PyPI
         uses: PyO3/maturin-action@v1
         env:
           MATURIN_PYPI_TOKEN: ${{ secrets.PYPI_API_TOKEN }}
         with:
           command: upload
-          args: --skip-existing *
+          args: --skip-existing *
```

### Comparing `rusty_chrono-0.1.3/.gitignore` & `rusty_chrono-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `rusty_chrono-0.1.3/.gitlab-ci.yml.old` & `rusty_chrono-0.1.4/.gitlab-ci.yml.old`

 * *Files 3% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 #     - cargo test --verbose
 
 update_project_version:
   stage: build
   image: python:alpine
   script:
     - pip install requests toml
-    - python publish_script.py
+    - python version_update_script.py
   artifacts:
     untracked: false
     when: on_success
     expire_in: "60 min"
     paths:
       - ./Cargo.toml
```

### Comparing `rusty_chrono-0.1.3/Dockerfile` & `rusty_chrono-0.1.4/Dockerfile`

 * *Files identical despite different names*

### Comparing `rusty_chrono-0.1.3/LICENSE` & `rusty_chrono-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rusty_chrono-0.1.3/publish_script.py` & `rusty_chrono-0.1.4/version_update_script.py`

 * *Files identical despite different names*

### Comparing `rusty_chrono-0.1.3/src/dateutil/date_errors.rs` & `rusty_chrono-0.1.4/src/dateutil/date_errors.rs`

 * *Files identical despite different names*

### Comparing `rusty_chrono-0.1.3/src/dateutil/date_functions.rs` & `rusty_chrono-0.1.4/src/dateutil/date_functions.rs`

 * *Files identical despite different names*

### Comparing `rusty_chrono-0.1.3/src/dateutil/date_parsing.rs` & `rusty_chrono-0.1.4/src/dateutil/date_parsing.rs`

 * *Files identical despite different names*

### Comparing `rusty_chrono-0.1.3/src/dateutil/dateutil_tests/date_functions_tests.rs` & `rusty_chrono-0.1.4/src/dateutil/dateutil_tests/date_functions_tests.rs`

 * *Files identical despite different names*

### Comparing `rusty_chrono-0.1.3/src/dateutil/dateutil_tests/date_parsing_tests.rs` & `rusty_chrono-0.1.4/src/dateutil/dateutil_tests/date_parsing_tests.rs`

 * *Files identical despite different names*

### Comparing `rusty_chrono-0.1.3/src/dateutil/time_fractions.rs` & `rusty_chrono-0.1.4/src/dateutil/time_fractions.rs`

 * *Files identical despite different names*

### Comparing `rusty_chrono-0.1.3/src/lib.rs` & `rusty_chrono-0.1.4/src/lib.rs`

 * *Files identical despite different names*

### Comparing `rusty_chrono-0.1.3/test.py` & `rusty_chrono-0.1.4/test.py`

 * *Files identical despite different names*

### Comparing `rusty_chrono-0.1.3/Cargo.lock` & `rusty_chrono-0.1.4/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -33,17 +33,20 @@
 name = "bumpalo"
 version = "3.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a3e2c3daef883ecc1b5d58c15adae93470a91d425f3532ba1695849656af3fc1"
 
 [[package]]
 name = "cc"
-version = "1.0.79"
+version = "1.0.82"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "50d30906286121d95be3d479533b458f87493b30a4b5f79a607db8f5d11aa91f"
+checksum = "305fe645edc1442a0fa8b6726ba61d422798d37a52e12eaecf4b022ebbb88f01"
+dependencies = [
+ "libc",
+]
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
@@ -284,15 +287,15 @@
 checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "rusty_chrono"
-version = "0.1.3"
+version = "0.1.4"
 dependencies = [
  "chrono",
  "pyo3",
  "pyo3-build-config",
  "test-case",
 ]
```

