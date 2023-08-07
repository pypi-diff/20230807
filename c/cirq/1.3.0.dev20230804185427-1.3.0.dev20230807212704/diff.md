# Comparing `tmp/cirq-1.3.0.dev20230804185427-py3-none-any.whl.zip` & `tmp/cirq-1.3.0.dev20230807212704-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 8404 bytes, number of entries: 6
--rw-r--r--  2.0 unx      292 b- defN 23-Aug-04 18:54 cirq-1.3.0.dev20230804185427.dist-info/AUTHORS
--rw-r--r--  2.0 unx    11357 b- defN 23-Aug-04 18:54 cirq-1.3.0.dev20230804185427.dist-info/LICENSE
--rw-r--r--  2.0 unx     7932 b- defN 23-Aug-04 18:54 cirq-1.3.0.dev20230804185427.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Aug-04 18:54 cirq-1.3.0.dev20230804185427.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-Aug-04 18:54 cirq-1.3.0.dev20230804185427.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      563 b- defN 23-Aug-04 18:54 cirq-1.3.0.dev20230804185427.dist-info/RECORD
-6 files, 20237 bytes uncompressed, 7366 bytes compressed:  63.6%
+Zip file size: 8394 bytes, number of entries: 6
+-rw-r--r--  2.0 unx      292 b- defN 23-Aug-07 21:27 cirq-1.3.0.dev20230807212704.dist-info/AUTHORS
+-rw-r--r--  2.0 unx    11357 b- defN 23-Aug-07 21:27 cirq-1.3.0.dev20230807212704.dist-info/LICENSE
+-rw-r--r--  2.0 unx     7874 b- defN 23-Aug-07 21:27 cirq-1.3.0.dev20230807212704.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-07 21:27 cirq-1.3.0.dev20230807212704.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Aug-07 21:27 cirq-1.3.0.dev20230807212704.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      563 b- defN 23-Aug-07 21:27 cirq-1.3.0.dev20230807212704.dist-info/RECORD
+6 files, 20179 bytes uncompressed, 7356 bytes compressed:  63.5%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
-Filename: cirq-1.3.0.dev20230804185427.dist-info/AUTHORS
+Filename: cirq-1.3.0.dev20230807212704.dist-info/AUTHORS
 Comment: 
 
-Filename: cirq-1.3.0.dev20230804185427.dist-info/LICENSE
+Filename: cirq-1.3.0.dev20230807212704.dist-info/LICENSE
 Comment: 
 
-Filename: cirq-1.3.0.dev20230804185427.dist-info/METADATA
+Filename: cirq-1.3.0.dev20230807212704.dist-info/METADATA
 Comment: 
 
-Filename: cirq-1.3.0.dev20230804185427.dist-info/WHEEL
+Filename: cirq-1.3.0.dev20230807212704.dist-info/WHEEL
 Comment: 
 
-Filename: cirq-1.3.0.dev20230804185427.dist-info/top_level.txt
+Filename: cirq-1.3.0.dev20230807212704.dist-info/top_level.txt
 Comment: 
 
-Filename: cirq-1.3.0.dev20230804185427.dist-info/RECORD
+Filename: cirq-1.3.0.dev20230807212704.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `cirq-1.3.0.dev20230804185427.dist-info/LICENSE` & `cirq-1.3.0.dev20230807212704.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `cirq-1.3.0.dev20230804185427.dist-info/METADATA` & `cirq-1.3.0.dev20230807212704.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,60 +1,60 @@
 Metadata-Version: 2.1
 Name: cirq
-Version: 1.3.0.dev20230804185427
+Version: 1.3.0.dev20230807212704
 Summary: A framework for creating, editing, and invoking Noisy Intermediate Scale Quantum (NISQ) circuits.
 Home-page: http://github.com/quantumlib/cirq
 Author: The Cirq Developers
 Author-email: cirq-dev@googlegroups.com
 License: Apache 2
 Platform: UNKNOWN
 Requires-Python: >=3.9.0
 License-File: LICENSE
 License-File: AUTHORS
-Requires-Dist: cirq-aqt (==1.3.0.dev20230804185427)
-Requires-Dist: cirq-core (==1.3.0.dev20230804185427)
-Requires-Dist: cirq-ft (==1.3.0.dev20230804185427)
-Requires-Dist: cirq-google (==1.3.0.dev20230804185427)
-Requires-Dist: cirq-ionq (==1.3.0.dev20230804185427)
-Requires-Dist: cirq-pasqal (==1.3.0.dev20230804185427)
-Requires-Dist: cirq-rigetti (==1.3.0.dev20230804185427)
-Requires-Dist: cirq-web (==1.3.0.dev20230804185427)
+Requires-Dist: cirq-aqt ==1.3.0.dev20230807212704
+Requires-Dist: cirq-core ==1.3.0.dev20230807212704
+Requires-Dist: cirq-ft ==1.3.0.dev20230807212704
+Requires-Dist: cirq-google ==1.3.0.dev20230807212704
+Requires-Dist: cirq-ionq ==1.3.0.dev20230807212704
+Requires-Dist: cirq-pasqal ==1.3.0.dev20230807212704
+Requires-Dist: cirq-rigetti ==1.3.0.dev20230807212704
+Requires-Dist: cirq-web ==1.3.0.dev20230807212704
 Provides-Extra: dev_env
-Requires-Dist: mypy (==1.2.0) ; extra == 'dev_env'
-Requires-Dist: types-backports (==0.1.3) ; extra == 'dev_env'
+Requires-Dist: mypy ==1.2.0 ; extra == 'dev_env'
+Requires-Dist: types-backports ==0.1.3 ; extra == 'dev_env'
 Requires-Dist: types-cachetools ; extra == 'dev_env'
-Requires-Dist: types-protobuf (~=3.20) ; extra == 'dev_env'
-Requires-Dist: types-requests (==2.28.1) ; extra == 'dev_env'
-Requires-Dist: types-setuptools (==62.6.1) ; extra == 'dev_env'
+Requires-Dist: types-protobuf ~=3.20 ; extra == 'dev_env'
+Requires-Dist: types-requests ==2.28.1 ; extra == 'dev_env'
+Requires-Dist: types-setuptools ==62.6.1 ; extra == 'dev_env'
 Requires-Dist: pytest ; extra == 'dev_env'
 Requires-Dist: pytest-asyncio ; extra == 'dev_env'
-Requires-Dist: pytest-cov (~=3.0) ; extra == 'dev_env'
+Requires-Dist: pytest-cov ~=3.0 ; extra == 'dev_env'
 Requires-Dist: pytest-randomly ; extra == 'dev_env'
-Requires-Dist: coverage (<=6.2) ; extra == 'dev_env'
-Requires-Dist: pytest-xdist (~=2.2.0) ; extra == 'dev_env'
-Requires-Dist: filelock (~=3.0.12) ; extra == 'dev_env'
-Requires-Dist: freezegun (~=0.3.15) ; extra == 'dev_env'
+Requires-Dist: coverage <=6.2 ; extra == 'dev_env'
+Requires-Dist: pytest-xdist ~=2.2.0 ; extra == 'dev_env'
+Requires-Dist: filelock ~=3.0.12 ; extra == 'dev_env'
+Requires-Dist: freezegun ~=0.3.15 ; extra == 'dev_env'
 Requires-Dist: importlib-metadata ; extra == 'dev_env'
 Requires-Dist: virtualenv ; extra == 'dev_env'
 Requires-Dist: virtualenv-clone ; extra == 'dev_env'
-Requires-Dist: black (==23.3.0) ; extra == 'dev_env'
-Requires-Dist: pylint (~=2.13.0) ; extra == 'dev_env'
-Requires-Dist: grpcio-tools (~=1.56.0) ; extra == 'dev_env'
-Requires-Dist: mypy-protobuf (==3.4) ; extra == 'dev_env'
-Requires-Dist: ipython (>=7.34.0) ; extra == 'dev_env'
-Requires-Dist: notebook (<=6.4.7,>=6.4.1) ; extra == 'dev_env'
-Requires-Dist: ipykernel (==5.3.4) ; extra == 'dev_env'
-Requires-Dist: papermill (~=2.3.2) ; extra == 'dev_env'
-Requires-Dist: seaborn (~=0.11.1) ; extra == 'dev_env'
+Requires-Dist: black ==23.3.0 ; extra == 'dev_env'
+Requires-Dist: pylint ~=2.13.0 ; extra == 'dev_env'
+Requires-Dist: grpcio-tools ~=1.56.0 ; extra == 'dev_env'
+Requires-Dist: mypy-protobuf ==3.4 ; extra == 'dev_env'
+Requires-Dist: ipython >=7.34.0 ; extra == 'dev_env'
+Requires-Dist: notebook <=6.4.7,>=6.4.1 ; extra == 'dev_env'
+Requires-Dist: ipykernel ==5.3.4 ; extra == 'dev_env'
+Requires-Dist: papermill ~=2.3.2 ; extra == 'dev_env'
+Requires-Dist: seaborn ~=0.11.1 ; extra == 'dev_env'
 Requires-Dist: setuptools ; extra == 'dev_env'
 Requires-Dist: wheel ; extra == 'dev_env'
 Requires-Dist: twine ; extra == 'dev_env'
 Requires-Dist: asv ; extra == 'dev_env'
-Requires-Dist: qiskit-aer (~=0.12.2) ; extra == 'dev_env'
-Requires-Dist: rstcheck (~=3.3.1) ; extra == 'dev_env'
+Requires-Dist: qiskit-aer ~=0.12.2 ; extra == 'dev_env'
+Requires-Dist: rstcheck ~=3.3.1 ; extra == 'dev_env'
 Requires-Dist: codeowners ; (platform_system != "Windows") and extra == 'dev_env'
 
 **This is a development version of Cirq and may be unstable.**
 
 **For the latest stable release of Cirq see**
 `here <https://pypi.org/project/cirq>`__.
```

