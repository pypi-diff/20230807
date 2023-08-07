# Comparing `tmp/pyxet-0.1.2.tar.gz` & `tmp/pyxet-0.1.2rc1.tar.gz`

## Comparing `pyxet-0.1.2.tar` & `pyxet-0.1.2rc1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1196 1970-01-01 00:00:00.000000 pyxet-0.1.2/Cargo.toml
--rw-r--r--   0        0        0      756 2023-07-28 20:45:38.000000 pyxet-0.1.2/.gitignore
--rw-r--r--   0        0        0     2100 2023-07-28 20:45:38.000000 pyxet-0.1.2/README.md
--rw-r--r--   0        0        0       84 2023-07-28 20:45:38.000000 pyxet-0.1.2/develop.sh
--rw-r--r--   0        0        0      654 2023-07-28 20:45:38.000000 pyxet-0.1.2/docs/Makefile
--rw-r--r--   0        0        0     1185 2023-07-28 20:45:38.000000 pyxet-0.1.2/docs/conf.py
--rw-r--r--   0        0        0    22791 2023-07-28 20:45:38.000000 pyxet-0.1.2/docs/images/logo.png
--rw-r--r--   0        0        0     1761 2023-07-28 20:45:38.000000 pyxet-0.1.2/docs/index.rst
--rw-r--r--   0        0        0      800 2023-07-28 20:45:38.000000 pyxet-0.1.2/docs/make.bat
--rw-r--r--   0        0        0     1088 2023-07-28 20:45:38.000000 pyxet-0.1.2/docs/markdowns/cli.md
--rw-r--r--   0        0        0     2239 2023-07-28 20:45:38.000000 pyxet-0.1.2/docs/markdowns/filesystem.md
--rw-r--r--   0        0        0      760 2023-07-28 20:45:38.000000 pyxet-0.1.2/docs/markdowns/git.md
--rw-r--r--   0        0        0     1399 2023-07-28 20:45:38.000000 pyxet-0.1.2/docs/markdowns/integrations.md
--rw-r--r--   0        0        0     1965 2023-07-28 20:45:38.000000 pyxet-0.1.2/docs/markdowns/mount.md
--rw-r--r--   0        0        0     3040 2023-07-28 20:45:38.000000 pyxet-0.1.2/docs/markdowns/quickstart.md
--rw-r--r--   0        0        0      209 2023-07-28 20:45:38.000000 pyxet-0.1.2/docs/markdowns/use_cases.md
--rw-r--r--   0        0        0       63 2023-07-28 20:45:38.000000 pyxet-0.1.2/docs/modules.rst
--rw-r--r--   0        0        0      231 2023-07-28 20:45:38.000000 pyxet-0.1.2/docs/pyxet.rst
--rw-r--r--   0        0        0     1762 2023-08-07 18:49:44.000000 pyxet-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1278 2023-07-28 20:45:38.000000 pyxet-0.1.2/pyxet/README.md
--rw-r--r--   0        0        0     2889 2023-07-28 20:45:38.000000 pyxet-0.1.2/pyxet/__init__.py
--rw-r--r--   0        0        0    28809 2023-08-07 18:37:39.000000 pyxet-0.1.2/pyxet/cli.py
--rw-r--r--   0        0        0    10521 2023-07-28 20:45:38.000000 pyxet-0.1.2/pyxet/commit_transaction.py
--rw-r--r--   0        0        0     3765 2023-08-07 18:37:39.000000 pyxet-0.1.2/pyxet/file_interface.py
--rw-r--r--   0        0        0    26707 2023-08-07 18:37:39.000000 pyxet-0.1.2/pyxet/file_system.py
--rw-r--r--   0        0        0     6547 2023-07-28 20:45:38.000000 pyxet-0.1.2/pyxet/pathlib.py
--rw-r--r--   0        0        0        0 2023-07-28 20:45:38.000000 pyxet-0.1.2/pyxet/rpyxet/__init__.py
--rw-r--r--   0        0        0     7538 2023-07-28 20:45:38.000000 pyxet-0.1.2/pyxet/url_parsing.py
--rw-r--r--   0        0        0       23 2023-08-07 18:49:22.000000 pyxet-0.1.2/pyxet/version.py
--rw-r--r--   0        0        0    22690 2023-08-07 18:37:39.000000 pyxet-0.1.2/src/lib.rs
--rw-r--r--   0        0        0     1898 2023-07-28 20:45:38.000000 pyxet-0.1.2/tests/arrow_test.py
--rw-r--r--   0        0        0     6906 2023-07-28 20:45:38.000000 pyxet-0.1.2/tests/file_test.py
--rw-r--r--   0        0        0     2333 2023-07-28 20:45:38.000000 pyxet-0.1.2/tests/fsspec_test.py
--rw-r--r--   0        0        0     1218 2023-07-28 20:45:38.000000 pyxet-0.1.2/tests/pandas_test.py
--rw-r--r--   0        0        0     2501 2023-07-28 20:45:38.000000 pyxet-0.1.2/tests/utils.py
--rw-r--r--   0        0        0   107536 2023-08-07 18:50:08.000000 pyxet-0.1.2/Cargo.lock
--rw-r--r--   0        0        0     3650 1970-01-01 00:00:00.000000 pyxet-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1200 1970-01-01 00:00:00.000000 pyxet-0.1.2rc1/Cargo.toml
+-rw-r--r--   0        0        0      756 2023-07-28 20:45:38.000000 pyxet-0.1.2rc1/.gitignore
+-rw-r--r--   0        0        0     2100 2023-07-28 20:45:38.000000 pyxet-0.1.2rc1/README.md
+-rw-r--r--   0        0        0       84 2023-07-28 20:45:38.000000 pyxet-0.1.2rc1/develop.sh
+-rw-r--r--   0        0        0      654 2023-07-28 20:45:38.000000 pyxet-0.1.2rc1/docs/Makefile
+-rw-r--r--   0        0        0     1185 2023-07-28 20:45:38.000000 pyxet-0.1.2rc1/docs/conf.py
+-rw-r--r--   0        0        0    22791 2023-07-28 20:45:38.000000 pyxet-0.1.2rc1/docs/images/logo.png
+-rw-r--r--   0        0        0     1761 2023-07-28 20:45:38.000000 pyxet-0.1.2rc1/docs/index.rst
+-rw-r--r--   0        0        0      800 2023-07-28 20:45:38.000000 pyxet-0.1.2rc1/docs/make.bat
+-rw-r--r--   0        0        0     1088 2023-07-28 20:45:38.000000 pyxet-0.1.2rc1/docs/markdowns/cli.md
+-rw-r--r--   0        0        0     2239 2023-07-28 20:45:38.000000 pyxet-0.1.2rc1/docs/markdowns/filesystem.md
+-rw-r--r--   0        0        0      760 2023-07-28 20:45:38.000000 pyxet-0.1.2rc1/docs/markdowns/git.md
+-rw-r--r--   0        0        0     1399 2023-07-28 20:45:38.000000 pyxet-0.1.2rc1/docs/markdowns/integrations.md
+-rw-r--r--   0        0        0     1965 2023-07-28 20:45:38.000000 pyxet-0.1.2rc1/docs/markdowns/mount.md
+-rw-r--r--   0        0        0     3040 2023-07-28 20:45:38.000000 pyxet-0.1.2rc1/docs/markdowns/quickstart.md
+-rw-r--r--   0        0        0      209 2023-07-28 20:45:38.000000 pyxet-0.1.2rc1/docs/markdowns/use_cases.md
+-rw-r--r--   0        0        0       63 2023-07-28 20:45:38.000000 pyxet-0.1.2rc1/docs/modules.rst
+-rw-r--r--   0        0        0      231 2023-07-28 20:45:38.000000 pyxet-0.1.2rc1/docs/pyxet.rst
+-rw-r--r--   0        0        0     1766 2023-08-07 18:37:39.000000 pyxet-0.1.2rc1/pyproject.toml
+-rw-r--r--   0        0        0     1278 2023-07-28 20:45:38.000000 pyxet-0.1.2rc1/pyxet/README.md
+-rw-r--r--   0        0        0     2889 2023-07-28 20:45:38.000000 pyxet-0.1.2rc1/pyxet/__init__.py
+-rw-r--r--   0        0        0    28809 2023-08-07 18:37:39.000000 pyxet-0.1.2rc1/pyxet/cli.py
+-rw-r--r--   0        0        0    10521 2023-07-28 20:45:38.000000 pyxet-0.1.2rc1/pyxet/commit_transaction.py
+-rw-r--r--   0        0        0     3765 2023-08-07 18:37:39.000000 pyxet-0.1.2rc1/pyxet/file_interface.py
+-rw-r--r--   0        0        0    26707 2023-08-07 18:37:39.000000 pyxet-0.1.2rc1/pyxet/file_system.py
+-rw-r--r--   0        0        0     6547 2023-07-28 20:45:38.000000 pyxet-0.1.2rc1/pyxet/pathlib.py
+-rw-r--r--   0        0        0        0 2023-07-28 20:45:38.000000 pyxet-0.1.2rc1/pyxet/rpyxet/__init__.py
+-rw-r--r--   0        0        0     7538 2023-07-28 20:45:38.000000 pyxet-0.1.2rc1/pyxet/url_parsing.py
+-rw-r--r--   0        0        0       27 2023-08-07 18:37:39.000000 pyxet-0.1.2rc1/pyxet/version.py
+-rw-r--r--   0        0        0    22690 2023-08-07 18:37:39.000000 pyxet-0.1.2rc1/src/lib.rs
+-rw-r--r--   0        0        0     1898 2023-07-28 20:45:38.000000 pyxet-0.1.2rc1/tests/arrow_test.py
+-rw-r--r--   0        0        0     6906 2023-07-28 20:45:38.000000 pyxet-0.1.2rc1/tests/file_test.py
+-rw-r--r--   0        0        0     2333 2023-07-28 20:45:38.000000 pyxet-0.1.2rc1/tests/fsspec_test.py
+-rw-r--r--   0        0        0     1218 2023-07-28 20:45:38.000000 pyxet-0.1.2rc1/tests/pandas_test.py
+-rw-r--r--   0        0        0     2501 2023-07-28 20:45:38.000000 pyxet-0.1.2rc1/tests/utils.py
+-rw-r--r--   0        0        0   112008 2023-08-07 18:37:39.000000 pyxet-0.1.2rc1/Cargo.lock
+-rw-r--r--   0        0        0     3653 1970-01-01 00:00:00.000000 pyxet-0.1.2rc1/PKG-INFO
```

### Comparing `pyxet-0.1.2/Cargo.toml` & `pyxet-0.1.2rc1/Cargo.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,75 +1,75 @@
 00000000: 5b70 6163 6b61 6765 5d0d 0a6e 616d 6520  [package]..name 
 00000010: 3d20 2270 7978 6574 220d 0a76 6572 7369  = "pyxet"..versi
-00000020: 6f6e 203d 2022 302e 312e 3222 0d0a 6564  on = "0.1.2"..ed
-00000030: 6974 696f 6e20 3d20 2232 3032 3122 0d0a  ition = "2021"..
-00000040: 0d0a 5b6c 6962 5d0d 0a23 2054 6865 206e  ..[lib]..# The n
-00000050: 616d 6520 6f66 2074 6865 206e 6174 6976  ame of the nativ
-00000060: 6520 6c69 6272 6172 792e 2054 6869 7320  e library. This 
-00000070: 6973 2074 6865 206e 616d 6520 7768 6963  is the name whic
-00000080: 6820 7769 6c6c 2062 6520 7573 6564 2069  h will be used i
-00000090: 6e20 5079 7468 6f6e 2074 6f20 696d 706f  n Python to impo
-000000a0: 7274 2074 6865 0d0a 2320 6c69 6272 6172  rt the..# librar
-000000b0: 7920 2869 2e65 2e20 6069 6d70 6f72 7420  y (i.e. `import 
-000000c0: 7374 7269 6e67 5f73 756d 6029 2e20 4966  string_sum`). If
-000000d0: 2079 6f75 2063 6861 6e67 6520 7468 6973   you change this
-000000e0: 2c20 796f 7520 6d75 7374 2061 6c73 6f20  , you must also 
-000000f0: 6368 616e 6765 2074 6865 206e 616d 6520  change the name 
-00000100: 6f66 2074 6865 0d0a 2320 6023 5b70 796d  of the..# `#[pym
-00000110: 6f64 756c 655d 6020 696e 2060 7372 632f  odule]` in `src/
-00000120: 6c69 622e 7273 602e 0d0a 6e61 6d65 203d  lib.rs`...name =
-00000130: 2022 7079 7865 7422 0d0a 2320 2263 6479   "pyxet"..# "cdy
-00000140: 6c69 6222 2069 7320 6e65 6365 7373 6172  lib" is necessar
-00000150: 7920 746f 2070 726f 6475 6365 2061 2073  y to produce a s
-00000160: 6861 7265 6420 6c69 6272 6172 7920 666f  hared library fo
-00000170: 7220 5079 7468 6f6e 2074 6f20 696d 706f  r Python to impo
-00000180: 7274 2066 726f 6d2e 0d0a 230d 0a23 2044  rt from...#..# D
-00000190: 6f77 6e73 7472 6561 6d20 5275 7374 2063  ownstream Rust c
-000001a0: 6f64 6520 2869 6e63 6c75 6469 6e67 2063  ode (including c
-000001b0: 6f64 6520 696e 2060 6269 6e2f 602c 2060  ode in `bin/`, `
-000001c0: 6578 616d 706c 6573 2f60 2c20 616e 6420  examples/`, and 
-000001d0: 6074 6573 7473 2f60 2920 7769 6c6c 206e  `tests/`) will n
-000001e0: 6f74 2062 6520 6162 6c65 0d0a 2320 746f  ot be able..# to
-000001f0: 2060 7573 6520 7374 7269 6e67 5f73 756d   `use string_sum
-00000200: 3b60 2075 6e6c 6573 7320 7468 6520 2272  ;` unless the "r
-00000210: 6c69 6222 206f 7220 226c 6962 2220 6372  lib" or "lib" cr
-00000220: 6174 6520 7479 7065 2069 7320 616c 736f  ate type is also
-00000230: 2069 6e63 6c75 6465 642c 2065 2e67 2e3a   included, e.g.:
-00000240: 0d0a 2320 6372 6174 652d 7479 7065 203d  ..# crate-type =
-00000250: 205b 2263 6479 6c69 6222 2c20 2272 6c69   ["cdylib", "rli
-00000260: 6222 5d0d 0a63 7261 7465 2d74 7970 6520  b"]..crate-type 
-00000270: 3d20 5b22 6364 796c 6962 225d 0d0a 0d0a  = ["cdylib"]....
-00000280: 5b64 6570 656e 6465 6e63 6965 735d 0d0a  [dependencies]..
-00000290: 7079 6f33 203d 207b 2076 6572 7369 6f6e  pyo3 = { version
-000002a0: 203d 2022 302e 3138 2e30 222c 2066 6561   = "0.18.0", fea
-000002b0: 7475 7265 7320 3d20 5b22 6578 7465 6e73  tures = ["extens
-000002c0: 696f 6e2d 6d6f 6475 6c65 222c 2022 6162  ion-module", "ab
-000002d0: 6933 2d70 7933 3722 2c20 2267 656e 6572  i3-py37", "gener
-000002e0: 6174 652d 696d 706f 7274 2d6c 6962 225d  ate-import-lib"]
-000002f0: 207d 0d0a 7865 7462 6c6f 6220 3d20 7b20   }..xetblob = { 
-00000300: 6769 7420 3d20 2268 7474 7073 3a2f 2f67  git = "https://g
-00000310: 6974 6875 622e 636f 6d2f 7865 7464 6174  ithub.com/xetdat
-00000320: 612f 7865 742d 636f 7265 2220 7d0d 0a67  a/xet-core" }..g
-00000330: 6974 7865 7463 6f72 6520 3d20 7b20 6769  itxetcore = { gi
-00000340: 7420 3d20 2268 7474 7073 3a2f 2f67 6974  t = "https://git
-00000350: 6875 622e 636f 6d2f 7865 7464 6174 612f  hub.com/xetdata/
-00000360: 7865 742d 636f 7265 2220 7d0d 0a74 656d  xet-core" }..tem
-00000370: 7066 696c 6520 3d20 2233 2e32 2e30 220d  pfile = "3.2.0".
-00000380: 0a70 796f 332d 6173 796e 6369 6f20 3d20  .pyo3-asyncio = 
-00000390: 7b20 7665 7273 696f 6e20 3d20 2230 2e31  { version = "0.1
-000003a0: 3822 2c20 6665 6174 7572 6573 203d 205b  8", features = [
-000003b0: 2261 7474 7269 6275 7465 7322 2c20 2274  "attributes", "t
-000003c0: 6f6b 696f 2d72 756e 7469 6d65 225d 207d  okio-runtime"] }
-000003d0: 0d0a 6c69 6263 203d 2022 302e 3222 0d0a  ..libc = "0.2"..
-000003e0: 7572 6c20 3d20 2232 2e33 2e31 220d 0a74  url = "2.3.1"..t
-000003f0: 7261 6369 6e67 203d 2022 302e 312e 2a22  racing = "0.1.*"
-00000400: 0d0a 746f 6b69 6f20 3d20 7b20 7665 7273  ..tokio = { vers
-00000410: 696f 6e20 3d20 2231 222c 2066 6561 7475  ion = "1", featu
-00000420: 7265 7320 3d20 5b22 6675 6c6c 225d 207d  res = ["full"] }
-00000430: 0d0a 6675 7475 7265 7320 3d20 2230 2e33  ..futures = "0.3
-00000440: 2e32 3122 0d0a 7468 6973 6572 726f 7220  .21"..thiserror 
-00000450: 3d20 2231 2e30 2e33 3022 0d0a 616e 7968  = "1.0.30"..anyh
-00000460: 6f77 203d 2022 3122 0d0a 0d0a 5b62 7569  ow = "1"....[bui
-00000470: 6c64 2d64 6570 656e 6465 6e63 6965 735d  ld-dependencies]
-00000480: 0d0a 7079 6f33 2d62 7569 6c64 2d63 6f6e  ..pyo3-build-con
-00000490: 6669 6720 3d20 2230 2e31 382e 3022 0d0a  fig = "0.18.0"..
-000004a0: 6363 203d 2022 312e 3022 0d0a            cc = "1.0"..
+00000020: 6f6e 203d 2022 302e 312e 322d 7263 3122  on = "0.1.2-rc1"
+00000030: 0d0a 6564 6974 696f 6e20 3d20 2232 3032  ..edition = "202
+00000040: 3122 0d0a 0d0a 5b6c 6962 5d0d 0a23 2054  1"....[lib]..# T
+00000050: 6865 206e 616d 6520 6f66 2074 6865 206e  he name of the n
+00000060: 6174 6976 6520 6c69 6272 6172 792e 2054  ative library. T
+00000070: 6869 7320 6973 2074 6865 206e 616d 6520  his is the name 
+00000080: 7768 6963 6820 7769 6c6c 2062 6520 7573  which will be us
+00000090: 6564 2069 6e20 5079 7468 6f6e 2074 6f20  ed in Python to 
+000000a0: 696d 706f 7274 2074 6865 0d0a 2320 6c69  import the..# li
+000000b0: 6272 6172 7920 2869 2e65 2e20 6069 6d70  brary (i.e. `imp
+000000c0: 6f72 7420 7374 7269 6e67 5f73 756d 6029  ort string_sum`)
+000000d0: 2e20 4966 2079 6f75 2063 6861 6e67 6520  . If you change 
+000000e0: 7468 6973 2c20 796f 7520 6d75 7374 2061  this, you must a
+000000f0: 6c73 6f20 6368 616e 6765 2074 6865 206e  lso change the n
+00000100: 616d 6520 6f66 2074 6865 0d0a 2320 6023  ame of the..# `#
+00000110: 5b70 796d 6f64 756c 655d 6020 696e 2060  [pymodule]` in `
+00000120: 7372 632f 6c69 622e 7273 602e 0d0a 6e61  src/lib.rs`...na
+00000130: 6d65 203d 2022 7079 7865 7422 0d0a 2320  me = "pyxet"..# 
+00000140: 2263 6479 6c69 6222 2069 7320 6e65 6365  "cdylib" is nece
+00000150: 7373 6172 7920 746f 2070 726f 6475 6365  ssary to produce
+00000160: 2061 2073 6861 7265 6420 6c69 6272 6172   a shared librar
+00000170: 7920 666f 7220 5079 7468 6f6e 2074 6f20  y for Python to 
+00000180: 696d 706f 7274 2066 726f 6d2e 0d0a 230d  import from...#.
+00000190: 0a23 2044 6f77 6e73 7472 6561 6d20 5275  .# Downstream Ru
+000001a0: 7374 2063 6f64 6520 2869 6e63 6c75 6469  st code (includi
+000001b0: 6e67 2063 6f64 6520 696e 2060 6269 6e2f  ng code in `bin/
+000001c0: 602c 2060 6578 616d 706c 6573 2f60 2c20  `, `examples/`, 
+000001d0: 616e 6420 6074 6573 7473 2f60 2920 7769  and `tests/`) wi
+000001e0: 6c6c 206e 6f74 2062 6520 6162 6c65 0d0a  ll not be able..
+000001f0: 2320 746f 2060 7573 6520 7374 7269 6e67  # to `use string
+00000200: 5f73 756d 3b60 2075 6e6c 6573 7320 7468  _sum;` unless th
+00000210: 6520 2272 6c69 6222 206f 7220 226c 6962  e "rlib" or "lib
+00000220: 2220 6372 6174 6520 7479 7065 2069 7320  " crate type is 
+00000230: 616c 736f 2069 6e63 6c75 6465 642c 2065  also included, e
+00000240: 2e67 2e3a 0d0a 2320 6372 6174 652d 7479  .g.:..# crate-ty
+00000250: 7065 203d 205b 2263 6479 6c69 6222 2c20  pe = ["cdylib", 
+00000260: 2272 6c69 6222 5d0d 0a63 7261 7465 2d74  "rlib"]..crate-t
+00000270: 7970 6520 3d20 5b22 6364 796c 6962 225d  ype = ["cdylib"]
+00000280: 0d0a 0d0a 5b64 6570 656e 6465 6e63 6965  ....[dependencie
+00000290: 735d 0d0a 7079 6f33 203d 207b 2076 6572  s]..pyo3 = { ver
+000002a0: 7369 6f6e 203d 2022 302e 3138 2e30 222c  sion = "0.18.0",
+000002b0: 2066 6561 7475 7265 7320 3d20 5b22 6578   features = ["ex
+000002c0: 7465 6e73 696f 6e2d 6d6f 6475 6c65 222c  tension-module",
+000002d0: 2022 6162 6933 2d70 7933 3722 2c20 2267   "abi3-py37", "g
+000002e0: 656e 6572 6174 652d 696d 706f 7274 2d6c  enerate-import-l
+000002f0: 6962 225d 207d 0d0a 7865 7462 6c6f 6220  ib"] }..xetblob 
+00000300: 3d20 7b20 6769 7420 3d20 2268 7474 7073  = { git = "https
+00000310: 3a2f 2f67 6974 6875 622e 636f 6d2f 7865  ://github.com/xe
+00000320: 7464 6174 612f 7865 742d 636f 7265 2220  tdata/xet-core" 
+00000330: 7d0d 0a67 6974 7865 7463 6f72 6520 3d20  }..gitxetcore = 
+00000340: 7b20 6769 7420 3d20 2268 7474 7073 3a2f  { git = "https:/
+00000350: 2f67 6974 6875 622e 636f 6d2f 7865 7464  /github.com/xetd
+00000360: 6174 612f 7865 742d 636f 7265 2220 7d0d  ata/xet-core" }.
+00000370: 0a74 656d 7066 696c 6520 3d20 2233 2e32  .tempfile = "3.2
+00000380: 2e30 220d 0a70 796f 332d 6173 796e 6369  .0"..pyo3-asynci
+00000390: 6f20 3d20 7b20 7665 7273 696f 6e20 3d20  o = { version = 
+000003a0: 2230 2e31 3822 2c20 6665 6174 7572 6573  "0.18", features
+000003b0: 203d 205b 2261 7474 7269 6275 7465 7322   = ["attributes"
+000003c0: 2c20 2274 6f6b 696f 2d72 756e 7469 6d65  , "tokio-runtime
+000003d0: 225d 207d 0d0a 6c69 6263 203d 2022 302e  "] }..libc = "0.
+000003e0: 3222 0d0a 7572 6c20 3d20 2232 2e33 2e31  2"..url = "2.3.1
+000003f0: 220d 0a74 7261 6369 6e67 203d 2022 302e  "..tracing = "0.
+00000400: 312e 2a22 0d0a 746f 6b69 6f20 3d20 7b20  1.*"..tokio = { 
+00000410: 7665 7273 696f 6e20 3d20 2231 222c 2066  version = "1", f
+00000420: 6561 7475 7265 7320 3d20 5b22 6675 6c6c  eatures = ["full
+00000430: 225d 207d 0d0a 6675 7475 7265 7320 3d20  "] }..futures = 
+00000440: 2230 2e33 2e32 3122 0d0a 7468 6973 6572  "0.3.21"..thiser
+00000450: 726f 7220 3d20 2231 2e30 2e33 3022 0d0a  ror = "1.0.30"..
+00000460: 616e 7968 6f77 203d 2022 3122 0d0a 0d0a  anyhow = "1"....
+00000470: 5b62 7569 6c64 2d64 6570 656e 6465 6e63  [build-dependenc
+00000480: 6965 735d 0d0a 7079 6f33 2d62 7569 6c64  ies]..pyo3-build
+00000490: 2d63 6f6e 6669 6720 3d20 2230 2e31 382e  -config = "0.18.
+000004a0: 3022 0d0a 6363 203d 2022 312e 3022 0d0a  0"..cc = "1.0"..
```

### Comparing `pyxet-0.1.2/.gitignore` & `pyxet-0.1.2rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `pyxet-0.1.2/README.md` & `pyxet-0.1.2rc1/README.md`

 * *Files identical despite different names*

### Comparing `pyxet-0.1.2/docs/Makefile` & `pyxet-0.1.2rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyxet-0.1.2/docs/conf.py` & `pyxet-0.1.2rc1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyxet-0.1.2/docs/images/logo.png` & `pyxet-0.1.2rc1/docs/images/logo.png`

 * *Files identical despite different names*

### Comparing `pyxet-0.1.2/docs/index.rst` & `pyxet-0.1.2rc1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pyxet-0.1.2/docs/make.bat` & `pyxet-0.1.2rc1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyxet-0.1.2/docs/markdowns/cli.md` & `pyxet-0.1.2rc1/docs/markdowns/cli.md`

 * *Files identical despite different names*

### Comparing `pyxet-0.1.2/docs/markdowns/filesystem.md` & `pyxet-0.1.2rc1/docs/markdowns/filesystem.md`

 * *Files identical despite different names*

### Comparing `pyxet-0.1.2/docs/markdowns/git.md` & `pyxet-0.1.2rc1/docs/markdowns/git.md`

 * *Files identical despite different names*

### Comparing `pyxet-0.1.2/docs/markdowns/integrations.md` & `pyxet-0.1.2rc1/docs/markdowns/integrations.md`

 * *Files identical despite different names*

### Comparing `pyxet-0.1.2/docs/markdowns/mount.md` & `pyxet-0.1.2rc1/docs/markdowns/mount.md`

 * *Files identical despite different names*

### Comparing `pyxet-0.1.2/docs/markdowns/quickstart.md` & `pyxet-0.1.2rc1/docs/markdowns/quickstart.md`

 * *Files identical despite different names*

### Comparing `pyxet-0.1.2/pyproject.toml` & `pyxet-0.1.2rc1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=0.14.17,<0.15"]
 build-backend = "maturin"
 
 [project]
 name = "pyxet"
-version = "0.1.2"
+version = "0.1.2-rc1"
 description = "pyxet is a Python library that provides a lightweight interface for the XetHub platform."
 keywords = [
     "ai",
     "collaboration",
     "data-science",
     "developer-tools",
     "git",
```

### Comparing `pyxet-0.1.2/pyxet/README.md` & `pyxet-0.1.2rc1/pyxet/README.md`

 * *Files identical despite different names*

### Comparing `pyxet-0.1.2/pyxet/__init__.py` & `pyxet-0.1.2rc1/pyxet/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxet-0.1.2/pyxet/cli.py` & `pyxet-0.1.2rc1/pyxet/cli.py`

 * *Files identical despite different names*

### Comparing `pyxet-0.1.2/pyxet/commit_transaction.py` & `pyxet-0.1.2rc1/pyxet/commit_transaction.py`

 * *Files identical despite different names*

### Comparing `pyxet-0.1.2/pyxet/file_interface.py` & `pyxet-0.1.2rc1/pyxet/file_interface.py`

 * *Files identical despite different names*

### Comparing `pyxet-0.1.2/pyxet/file_system.py` & `pyxet-0.1.2rc1/pyxet/file_system.py`

 * *Files identical despite different names*

### Comparing `pyxet-0.1.2/pyxet/pathlib.py` & `pyxet-0.1.2rc1/pyxet/pathlib.py`

 * *Files identical despite different names*

### Comparing `pyxet-0.1.2/pyxet/url_parsing.py` & `pyxet-0.1.2rc1/pyxet/url_parsing.py`

 * *Files identical despite different names*

### Comparing `pyxet-0.1.2/src/lib.rs` & `pyxet-0.1.2rc1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pyxet-0.1.2/tests/arrow_test.py` & `pyxet-0.1.2rc1/tests/arrow_test.py`

 * *Files identical despite different names*

### Comparing `pyxet-0.1.2/tests/file_test.py` & `pyxet-0.1.2rc1/tests/file_test.py`

 * *Files identical despite different names*

### Comparing `pyxet-0.1.2/tests/fsspec_test.py` & `pyxet-0.1.2rc1/tests/fsspec_test.py`

 * *Files identical despite different names*

### Comparing `pyxet-0.1.2/tests/pandas_test.py` & `pyxet-0.1.2rc1/tests/pandas_test.py`

 * *Files identical despite different names*

### Comparing `pyxet-0.1.2/tests/utils.py` & `pyxet-0.1.2rc1/tests/utils.py`

 * *Files identical despite different names*

### Comparing `pyxet-0.1.2/PKG-INFO` & `pyxet-0.1.2rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxet
-Version: 0.1.2
+Version: 0.1.2rc1
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

