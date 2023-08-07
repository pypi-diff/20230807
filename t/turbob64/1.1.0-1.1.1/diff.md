# Comparing `tmp/turbob64-1.1.0.tar.gz` & `tmp/turbob64-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turbob64-1.1.0.tar", last modified: Sun Aug  6 05:10:58 2023, max compression
+gzip compressed data, was "C:\projects\turbobase64\dist\.tmp-x2njw9bl\turbob64-1.1.1.tar", last modified: Mon Aug  7 00:39:39 2023, max compression
```

## Comparing `turbob64-1.1.0.tar` & `turbob64-1.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-08-06 05:10:58.036259 turbob64-1.1.0/
--rw-rw-rw-   0        0        0    35149 2023-08-04 19:55:58.000000 turbob64-1.1.0/LICENSE
--rw-rw-rw-   0        0        0       49 2023-08-04 22:17:46.000000 turbob64-1.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2668 2023-08-06 05:10:58.036259 turbob64-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2302 2023-08-05 00:22:54.000000 turbob64-1.1.0/README.md
--rw-rw-rw-   0        0        0      719 2023-08-04 22:04:30.000000 turbob64-1.1.0/_build.py
--rw-rw-rw-   0        0        0      555 2023-08-06 05:08:45.000000 turbob64-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-06 05:10:58.037266 turbob64-1.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-08-06 05:10:58.031228 turbob64-1.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-08-06 05:10:58.032223 turbob64-1.1.0/src/lib/
--rw-rw-rw-   0        0        0    63920 2023-08-01 16:47:33.000000 turbob64-1.1.0/src/lib/libtb64.a
--rw-rw-rw-   0        0        0     5287 2023-08-02 06:41:11.000000 turbob64-1.1.0/src/turbob64.h
--rw-rw-rw-   0        0        0     7805 2023-08-06 05:10:24.000000 turbob64-1.1.0/src/turbob64.pyx
-drwxrwxrwx   0        0        0        0 2023-08-06 05:10:58.035261 turbob64-1.1.0/turbob64.egg-info/
--rw-rw-rw-   0        0        0     2668 2023-08-06 05:10:58.000000 turbob64-1.1.0/turbob64.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      232 2023-08-06 05:10:58.000000 turbob64-1.1.0/turbob64.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-06 05:10:58.000000 turbob64-1.1.0/turbob64.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-08-06 05:10:58.000000 turbob64-1.1.0/turbob64.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-07 00:39:39.000000 turbob64-1.1.1/
+-rw-rw-rw-   0        0        0    35149 2023-08-07 00:39:16.000000 turbob64-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0       88 2023-08-07 00:39:16.000000 turbob64-1.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     3129 2023-08-07 00:39:39.000000 turbob64-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2549 2023-08-07 00:39:16.000000 turbob64-1.1.1/README.md
+-rw-rw-rw-   0        0        0      699 2023-08-07 00:39:16.000000 turbob64-1.1.1/_build.py
+-rw-rw-rw-   0        0        0      628 2023-08-07 00:39:16.000000 turbob64-1.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-07 00:39:39.000000 turbob64-1.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-07 00:39:39.000000 turbob64-1.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-08-07 00:39:39.000000 turbob64-1.1.1/src/lib/
+-rw-rw-rw-   0        0        0    63920 2023-08-07 00:39:16.000000 turbob64-1.1.1/src/lib/libtb64.a
+-rw-rw-rw-   0        0        0     5287 2023-08-07 00:39:16.000000 turbob64-1.1.1/src/turbob64.h
+-rw-rw-rw-   0        0        0     7805 2023-08-07 00:39:16.000000 turbob64-1.1.1/src/turbob64.pyx
+drwxrwxrwx   0        0        0        0 2023-08-07 00:39:39.000000 turbob64-1.1.1/turbob64.egg-info/
+-rw-rw-rw-   0        0        0     3129 2023-08-07 00:39:39.000000 turbob64-1.1.1/turbob64.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      232 2023-08-07 00:39:39.000000 turbob64-1.1.1/turbob64.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 00:39:39.000000 turbob64-1.1.1/turbob64.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-08-07 00:39:39.000000 turbob64-1.1.1/turbob64.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `turbob64-1.1.0/LICENSE` & `turbob64-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `turbob64-1.1.0/PKG-INFO` & `turbob64-1.1.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,133 +1,127 @@
-Metadata-Version: 2.1
-Name: turbob64
-Version: 1.1.0
-Summary: Cython bindings for Turbo Base64
-Author-email: daijro <daijro.dev@gmail.com>
-License: GPL-3.0
-Keywords: base64,encoding,decoding,turbo,cython
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: C
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-<h1 align="center">
-    Turbo Base64
-</h1>
-
-
-<p align="center">
-    <a href="https://github.com/daijro/OperatorPrank/blob/main/LICENSE">
-        <img src="https://img.shields.io/github/license/daijro/OperatorPrank">
-    </a>
-    <a href="https://python.org/">
-        <img src="https://img.shields.io/badge/python-3.x-blue">
-    </a>
-    <a href="https://github.com/cython/cython">
-        <img src="https://img.shields.io/badge/language-cython-black.svg">
-    </a>
-</p>
-
-<h5 align="center">
-    🚀 Lightning fast base64 encoding for Python
-</h5>
-
-## ✨ Features
-
-- 20-30x faster than the standard library
-- Benchmarks faster than any other C base64 library
-- Fastest implementation of AVX, AVX2, and AVX512 base64 encoding
-- No other dependencies
-
-<hr width=50>
-
-## ⚡ How fast is it?
-
-Graph generated from [benchmark.py](https://github.com/daijro/turbobase64/blob/main/benchmark.py):
-
-<img src="https://i.imgur.com/jC3ka6e.png" width=500>
-
-<hr width=50>
-
-## 💻 Usage
-
-```py
->>> import turbob64
-```
-
-This will automatically detect the fastest algorithm your CPU is capable of and use it.
-
-### Encoding
-
-```py
->>> turbob64.b64encode(b'Hello World!')
-b'SGVsbG8gV29ybGQh'
-```
-
-### Decoding
-
-```py
->>> turbob64.b64decode(b'SGVsbG8gV29ybGQh')
-b'Hello World!'
-```
-
-<hr width=50>
-
-### Other Functions
-
-<details>
-<summary>
-Directly call CPU-specific algorithms
-</summary>
-
-Memory efficient (small lookup tables) scalar but slower version
-
-```py
-turbob64.b64senc(b'Hello World!')
-turbob64.b64sdec(b'SGVsbG8gV29ybGQh')
-```
-
-Fast scalar
-
-```py
-turbob64.b64xenc(b'Hello World!')
-turbo64.b64xdec(b'SGVsbG8gV29ybGQh')
-```
-
-ssse3 SIMD
-
-```py
-turbob64.b64v128enc(b'Hello World!')
-turbob64.b64v128dec(b'SGVsbG8gV29ybGQh')
-```
-
-avx SIMD
-
-```py
-turbob64.b64v128aenc(b'Hello World!')
-turbob64.b64v128adec(b'SGVsbG8gV29ybGQh')
-```
-
-avx2 SIMD
-
-```py
-turbob64.b64v256enc(b'Hello World!')
-turbob64.b64v256dec(b'SGVsbG8gV29ybGQh')
-```
-
-avx2 SIMD (optimized for short strings)
-
-```py
-turbob64.b64v256enc_short(b'Hello World!')
-turbob64.b64v256dec_short(b'SGVsbG8gV29ybGQh')
-```
-
-avx512_vbmi SIMD
-
-```py
-turbob64.b64v512enc(b'Hello World!')
-turbob64.b64v512dec(b'SGVsbG8gV29ybGQh')
-```
-
-</details>
-
----
+<h1 align="center">
+    Turbo Base64
+</h1>
+
+
+<p align="center">
+    <a href="https://github.com/daijro/turbobase64/blob/main/LICENSE">
+        <img src="https://img.shields.io/github/license/daijro/turbobase64?color=yellow">
+    </a>
+    <a href="https://python.org/">
+        <img src="https://img.shields.io/badge/python-3.7&#8208;3.11-blue">
+    </a>
+    <a href="https://github.com/cython/cython">
+        <img src="https://img.shields.io/badge/language-cython-black.svg">
+    </a>
+    <a href="https://pypi.org/project/turbob64/">
+        <img alt="PyPI" src="https://img.shields.io/pypi/v/turbob64.svg?color=orange">
+    </a>
+    <a href="https://ci.appveyor.com/project/daijro/turbobase64">
+        <img alt="AppVeyor" src="https://ci.appveyor.com/api/projects/status/github/daijro/turbobase64?svg=true">
+    </a>
+    <h4 align="center">
+        🚀 Lightning fast base64 encoding for Python
+    </h4>
+</p>
+
+
+## ✨ Features
+
+- 20-30x faster than the standard library
+- Benchmarks faster than any other C base64 library
+- Fastest implementation of AVX, AVX2, and AVX512 base64 encoding
+- No other dependencies
+
+<hr width=50>
+
+## ⚡ How fast is it?
+
+Graph generated from [benchmark.py](https://github.com/daijro/turbobase64/blob/main/benchmark.py):
+
+<img src="https://i.imgur.com/jC3ka6e.png" width=500>
+
+<hr width=50>
+
+## 💻 Usage
+
+```py
+>>> import turbob64
+```
+
+This will automatically detect the fastest algorithm your CPU is capable of and use it.
+
+### Encoding
+
+```py
+>>> turbob64.b64encode(b'Hello World!')
+b'SGVsbG8gV29ybGQh'
+```
+
+### Decoding
+
+```py
+>>> turbob64.b64decode(b'SGVsbG8gV29ybGQh')
+b'Hello World!'
+```
+
+<hr width=50>
+
+### Other Functions
+
+<details>
+<summary>
+Directly call CPU-specific algorithms
+</summary>
+
+Memory efficient (small lookup tables) scalar but slower version
+
+```py
+turbob64.b64senc(b'Hello World!')
+turbob64.b64sdec(b'SGVsbG8gV29ybGQh')
+```
+
+Fast scalar
+
+```py
+turbob64.b64xenc(b'Hello World!')
+turbo64.b64xdec(b'SGVsbG8gV29ybGQh')
+```
+
+ssse3 SIMD
+
+```py
+turbob64.b64v128enc(b'Hello World!')
+turbob64.b64v128dec(b'SGVsbG8gV29ybGQh')
+```
+
+avx SIMD
+
+```py
+turbob64.b64v128aenc(b'Hello World!')
+turbob64.b64v128adec(b'SGVsbG8gV29ybGQh')
+```
+
+avx2 SIMD
+
+```py
+turbob64.b64v256enc(b'Hello World!')
+turbob64.b64v256dec(b'SGVsbG8gV29ybGQh')
+```
+
+avx2 SIMD (optimized for short strings)
+
+```py
+turbob64.b64v256enc_short(b'Hello World!')
+turbob64.b64v256dec_short(b'SGVsbG8gV29ybGQh')
+```
+
+avx512_vbmi SIMD
+
+```py
+turbob64.b64v512enc(b'Hello World!')
+turbob64.b64v512dec(b'SGVsbG8gV29ybGQh')
+```
+
+</details>
+
+---
```

#### html2text {}

```diff
@@ -1,17 +1,12 @@
-Metadata-Version: 2.1 Name: turbob64 Version: 1.1.0 Summary: Cython bindings
-for Turbo Base64 Author-email: daijro
-dev@gmail.com> License: GPL-3.0 Keywords: base64,encoding,decoding,turbo,cython
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: C Description-Content-Type: text/markdown License-File: LICENSE
                           ****** Turbo Base64 ******
-    [https://img.shields.io/github/license/daijro/OperatorPrank] [https://
- img.shields.io/badge/python-3.x-blue] [https://img.shields.io/badge/language-
-                               cython-black.svg]
-             ** ð Lightning fast base64 encoding for Python **
+[https://img.shields.io/github/license/daijro/turbobase64?color=yellow] [https:
+  //img.shields.io/badge/python-3.7&#8208;3.11-blue] [https://img.shields.io/
+              badge/language-cython-black.svg] [PyPI] [AppVeyor]
+            *** ð Lightning fast base64 encoding for Python ***
 ## â¨ Features - 20-30x faster than the standard library - Benchmarks faster
 than any other C base64 library - Fastest implementation of AVX, AVX2, and
 AVX512 base64 encoding - No other dependencies
 ===============================================================================
 ## â¡ How fast is it? Graph generated from [benchmark.py](https://github.com/
 daijro/turbobase64/blob/main/benchmark.py): [https://i.imgur.com/jC3ka6e.png]
 ===============================================================================
```

### Comparing `turbob64-1.1.0/src/lib/libtb64.a` & `turbob64-1.1.1/src/lib/libtb64.a`

 * *Files identical despite different names*

### Comparing `turbob64-1.1.0/src/turbob64.h` & `turbob64-1.1.1/src/turbob64.h`

 * *Files identical despite different names*

### Comparing `turbob64-1.1.0/src/turbob64.pyx` & `turbob64-1.1.1/src/turbob64.pyx`

 * *Files identical despite different names*

### Comparing `turbob64-1.1.0/turbob64.egg-info/PKG-INFO` & `turbob64-1.1.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,39 +1,47 @@
 Metadata-Version: 2.1
 Name: turbob64
-Version: 1.1.0
+Version: 1.1.1
 Summary: Cython bindings for Turbo Base64
 Author-email: daijro <daijro.dev@gmail.com>
 License: GPL-3.0
+Project-URL: repository, https://github.com/daijro/turbobase64
 Keywords: base64,encoding,decoding,turbo,cython
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: C
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">
     Turbo Base64
 </h1>
 
 
 <p align="center">
-    <a href="https://github.com/daijro/OperatorPrank/blob/main/LICENSE">
-        <img src="https://img.shields.io/github/license/daijro/OperatorPrank">
+    <a href="https://github.com/daijro/turbobase64/blob/main/LICENSE">
+        <img src="https://img.shields.io/github/license/daijro/turbobase64?color=yellow">
     </a>
     <a href="https://python.org/">
-        <img src="https://img.shields.io/badge/python-3.x-blue">
+        <img src="https://img.shields.io/badge/python-3.7&#8208;3.11-blue">
     </a>
     <a href="https://github.com/cython/cython">
         <img src="https://img.shields.io/badge/language-cython-black.svg">
     </a>
+    <a href="https://pypi.org/project/turbob64/">
+        <img alt="PyPI" src="https://img.shields.io/pypi/v/turbob64.svg?color=orange">
+    </a>
+    <a href="https://ci.appveyor.com/project/daijro/turbobase64">
+        <img alt="AppVeyor" src="https://ci.appveyor.com/api/projects/status/github/daijro/turbobase64?svg=true">
+    </a>
+    <h4 align="center">
+        🚀 Lightning fast base64 encoding for Python
+    </h4>
 </p>
 
-<h5 align="center">
-    🚀 Lightning fast base64 encoding for Python
-</h5>
 
 ## ✨ Features
 
 - 20-30x faster than the standard library
 - Benchmarks faster than any other C base64 library
 - Fastest implementation of AVX, AVX2, and AVX512 base64 encoding
 - No other dependencies
```

#### html2text {}

```diff
@@ -1,17 +1,19 @@
-Metadata-Version: 2.1 Name: turbob64 Version: 1.1.0 Summary: Cython bindings
+Metadata-Version: 2.1 Name: turbob64 Version: 1.1.1 Summary: Cython bindings
 for Turbo Base64 Author-email: daijro
-dev@gmail.com> License: GPL-3.0 Keywords: base64,encoding,decoding,turbo,cython
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: C Description-Content-Type: text/markdown License-File: LICENSE
+dev@gmail.com> License: GPL-3.0 Project-URL: repository, https://github.com/
+daijro/turbobase64 Keywords: base64,encoding,decoding,turbo,cython Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: C
+Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
+LICENSE
                           ****** Turbo Base64 ******
-    [https://img.shields.io/github/license/daijro/OperatorPrank] [https://
- img.shields.io/badge/python-3.x-blue] [https://img.shields.io/badge/language-
-                               cython-black.svg]
-             ** ð Lightning fast base64 encoding for Python **
+[https://img.shields.io/github/license/daijro/turbobase64?color=yellow] [https:
+  //img.shields.io/badge/python-3.7&#8208;3.11-blue] [https://img.shields.io/
+              badge/language-cython-black.svg] [PyPI] [AppVeyor]
+            *** ð Lightning fast base64 encoding for Python ***
 ## â¨ Features - 20-30x faster than the standard library - Benchmarks faster
 than any other C base64 library - Fastest implementation of AVX, AVX2, and
 AVX512 base64 encoding - No other dependencies
 ===============================================================================
 ## â¡ How fast is it? Graph generated from [benchmark.py](https://github.com/
 daijro/turbobase64/blob/main/benchmark.py): [https://i.imgur.com/jC3ka6e.png]
 ===============================================================================
```

