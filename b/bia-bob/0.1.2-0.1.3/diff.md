# Comparing `tmp/bia-bob-0.1.2.tar.gz` & `tmp/bia-bob-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bia-bob-0.1.2.tar", last modified: Mon Aug  7 09:44:33 2023, max compression
+gzip compressed data, was "bia-bob-0.1.3.tar", last modified: Mon Aug  7 11:02:04 2023, max compression
```

## Comparing `bia-bob-0.1.2.tar` & `bia-bob-0.1.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-08-07 09:44:33.091853 bia-bob-0.1.2/
--rw-rw-rw-   0        0        0     1527 2023-08-05 10:23:51.000000 bia-bob-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      101 2023-08-05 10:44:20.000000 bia-bob-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     3825 2023-08-07 09:44:33.091853 bia-bob-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2545 2023-08-07 09:42:12.000000 bia-bob-0.1.2/README.md
--rw-rw-rw-   0        0        0     1233 2023-08-05 10:44:20.000000 bia-bob-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0     1662 2023-08-07 09:44:33.093858 bia-bob-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0       89 2023-02-23 17:18:17.000000 bia-bob-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-07 09:44:33.044522 bia-bob-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2023-08-07 09:44:33.061094 bia-bob-0.1.2/src/bia_bob/
--rw-rw-rw-   0        0        0      158 2023-08-07 09:41:27.000000 bia-bob-0.1.2/src/bia_bob/__init__.py
--rw-rw-rw-   0        0        0     1590 2023-08-05 11:28:14.000000 bia-bob-0.1.2/src/bia_bob/_machinery.py
-drwxrwxrwx   0        0        0        0 2023-08-07 09:44:33.090849 bia-bob-0.1.2/src/bia_bob/_tests/
--rw-rw-rw-   0        0        0       31 2023-08-05 10:48:31.000000 bia-bob-0.1.2/src/bia_bob/_tests/__init__.py
--rw-rw-rw-   0        0        0     6643 2023-08-07 09:33:59.000000 bia-bob-0.1.2/src/bia_bob/_tools.py
--rw-rw-rw-   0        0        0     1175 2023-08-05 15:52:07.000000 bia-bob-0.1.2/src/bia_bob/_utilities.py
-drwxrwxrwx   0        0        0        0 2023-08-07 09:44:33.085836 bia-bob-0.1.2/src/bia_bob.egg-info/
--rw-rw-rw-   0        0        0     3825 2023-08-07 09:44:32.000000 bia-bob-0.1.2/src/bia_bob.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      366 2023-08-07 09:44:32.000000 bia-bob-0.1.2/src/bia_bob.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-07 09:44:32.000000 bia-bob-0.1.2/src/bia_bob.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      123 2023-08-07 09:44:32.000000 bia-bob-0.1.2/src/bia_bob.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-08-07 09:44:32.000000 bia-bob-0.1.2/src/bia_bob.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-07 11:02:04.453003 bia-bob-0.1.3/
+-rw-rw-rw-   0        0        0     1527 2023-08-05 10:23:51.000000 bia-bob-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      101 2023-08-05 10:44:20.000000 bia-bob-0.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     3795 2023-08-07 11:02:04.454005 bia-bob-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2548 2023-08-07 10:58:05.000000 bia-bob-0.1.3/README.md
+-rw-rw-rw-   0        0        0     1233 2023-08-05 10:44:20.000000 bia-bob-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0     1640 2023-08-07 11:02:04.460854 bia-bob-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0       89 2023-02-23 17:18:17.000000 bia-bob-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 11:02:04.421922 bia-bob-0.1.3/src/
+drwxrwxrwx   0        0        0        0 2023-08-07 11:02:04.431948 bia-bob-0.1.3/src/bia_bob/
+-rw-rw-rw-   0        0        0      158 2023-08-07 11:00:50.000000 bia-bob-0.1.3/src/bia_bob/__init__.py
+-rw-rw-rw-   0        0        0     1590 2023-08-05 11:28:14.000000 bia-bob-0.1.3/src/bia_bob/_machinery.py
+drwxrwxrwx   0        0        0        0 2023-08-07 11:02:04.451999 bia-bob-0.1.3/src/bia_bob/_tests/
+-rw-rw-rw-   0        0        0       31 2023-08-05 10:48:31.000000 bia-bob-0.1.3/src/bia_bob/_tests/__init__.py
+-rw-rw-rw-   0        0        0     6643 2023-08-07 09:33:59.000000 bia-bob-0.1.3/src/bia_bob/_tools.py
+-rw-rw-rw-   0        0        0     1175 2023-08-05 15:52:07.000000 bia-bob-0.1.3/src/bia_bob/_utilities.py
+drwxrwxrwx   0        0        0        0 2023-08-07 11:02:04.451999 bia-bob-0.1.3/src/bia_bob.egg-info/
+-rw-rw-rw-   0        0        0     3795 2023-08-07 11:02:04.000000 bia-bob-0.1.3/src/bia_bob.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      366 2023-08-07 11:02:04.000000 bia-bob-0.1.3/src/bia_bob.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 11:02:04.000000 bia-bob-0.1.3/src/bia_bob.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      123 2023-08-07 11:02:04.000000 bia-bob-0.1.3/src/bia_bob.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-08-07 11:02:04.000000 bia-bob-0.1.3/src/bia_bob.egg-info/top_level.txt
```

### Comparing `bia-bob-0.1.2/LICENSE` & `bia-bob-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bia-bob-0.1.2/PKG-INFO` & `bia-bob-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: bia-bob
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Jupyter-based assistant for working on bio-image analysis tasks
 Home-page: https://github.com/haesleinhuepf/bia-bob
 Author: Robert Haase
 Author-email: robert.haase@tu-dresden.de
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/haesleinhuepf/bia-bob/issues
 Project-URL: Documentation, https://github.com/haesleinhuepf/bia-bob#README.md
 Project-URL: Source Code, https://github.com/haesleinhuepf/bia-bob
 Project-URL: User Support, https://github.com/haesleinhuepf/bia-bob/issues
 Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Framework :: napari
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
@@ -58,28 +57,29 @@
 ```
 
 Afterwards, you can ask Bob questions like this:
 ```
 %bob Load blobs.tif and show it
 ```
 
-You can also ask Bob about available tools:
-```
-%bob list tools
-```
-
 Or like this:
 ```
 %%bob
 Please load the image blobs.tif,
 segment bright objects in it, 
 count them and 
 show the segmentation result.
 ```
 
+
+You can also ask Bob about available tools:
+```
+%bob list tools
+```
+
 ## Example gallery
 
 ![img.png](https://github.com/haesleinhuepf/bia-bob/raw/main/docs/images/load_and_show.png)
 
 ![img_1.png](https://github.com/haesleinhuepf/bia-bob/raw/main/docs/images/slice.png)
 
 ![img.png](https://github.com/haesleinhuepf/bia-bob/raw/main/docs/images/chain_workflows.png)
@@ -89,15 +89,15 @@
 ![img.png](https://github.com/haesleinhuepf/bia-bob/raw/main/docs/images/edge_detection.png)
 
 ## Known issues
 
 If you want to ask Bob a question, you need to put a space before the `?`.
 
 ```
-What do you know about blobs.gif?
+What do you know about blobs.gif ?
 ```
 
 ## Installation
 
 ```
 pip install bia-bob
 ```
```

### Comparing `bia-bob-0.1.2/README.md` & `bia-bob-0.1.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -29,28 +29,29 @@
 ```
 
 Afterwards, you can ask Bob questions like this:
 ```
 %bob Load blobs.tif and show it
 ```
 
-You can also ask Bob about available tools:
-```
-%bob list tools
-```
-
 Or like this:
 ```
 %%bob
 Please load the image blobs.tif,
 segment bright objects in it, 
 count them and 
 show the segmentation result.
 ```
 
+
+You can also ask Bob about available tools:
+```
+%bob list tools
+```
+
 ## Example gallery
 
 ![img.png](https://github.com/haesleinhuepf/bia-bob/raw/main/docs/images/load_and_show.png)
 
 ![img_1.png](https://github.com/haesleinhuepf/bia-bob/raw/main/docs/images/slice.png)
 
 ![img.png](https://github.com/haesleinhuepf/bia-bob/raw/main/docs/images/chain_workflows.png)
@@ -60,15 +61,15 @@
 ![img.png](https://github.com/haesleinhuepf/bia-bob/raw/main/docs/images/edge_detection.png)
 
 ## Known issues
 
 If you want to ask Bob a question, you need to put a space before the `?`.
 
 ```
-What do you know about blobs.gif?
+What do you know about blobs.gif ?
 ```
 
 ## Installation
 
 ```
 pip install bia-bob
 ```
```

### Comparing `bia-bob-0.1.2/pyproject.toml` & `bia-bob-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bia-bob-0.1.2/setup.cfg` & `bia-bob-0.1.3/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -21,84 +21,83 @@
 00000140: 742e 6861 6173 6540 7475 2d64 7265 7364  t.haase@tu-dresd
 00000150: 656e 2e64 650d 0a6c 6963 656e 7365 203d  en.de..license =
 00000160: 2042 5344 2d33 2d43 6c61 7573 650d 0a6c   BSD-3-Clause..l
 00000170: 6963 656e 7365 5f66 696c 6573 203d 204c  icense_files = L
 00000180: 4943 454e 5345 0d0a 636c 6173 7369 6669  ICENSE..classifi
 00000190: 6572 7320 3d20 0d0a 0944 6576 656c 6f70  ers = ...Develop
 000001a0: 6d65 6e74 2053 7461 7475 7320 3a3a 2032  ment Status :: 2
-000001b0: 202d 2050 7265 2d41 6c70 6861 0d0a 0946   - Pre-Alpha...F
-000001c0: 7261 6d65 776f 726b 203a 3a20 6e61 7061  ramework :: napa
-000001d0: 7269 0d0a 0949 6e74 656e 6465 6420 4175  ri...Intended Au
-000001e0: 6469 656e 6365 203a 3a20 4465 7665 6c6f  dience :: Develo
-000001f0: 7065 7273 0d0a 094c 6963 656e 7365 203a  pers...License :
-00000200: 3a20 4f53 4920 4170 7072 6f76 6564 203a  : OSI Approved :
-00000210: 3a20 4253 4420 4c69 6365 6e73 650d 0a09  : BSD License...
-00000220: 4f70 6572 6174 696e 6720 5379 7374 656d  Operating System
-00000230: 203a 3a20 4f53 2049 6e64 6570 656e 6465   :: OS Independe
-00000240: 6e74 0d0a 0950 726f 6772 616d 6d69 6e67  nt...Programming
-00000250: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-00000260: 686f 6e0d 0a09 5072 6f67 7261 6d6d 696e  hon...Programmin
-00000270: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-00000280: 7468 6f6e 203a 3a20 330d 0a09 5072 6f67  thon :: 3...Prog
-00000290: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-000002a0: 203a 3a20 5079 7468 6f6e 203a 3a20 3320   :: Python :: 3 
-000002b0: 3a3a 204f 6e6c 790d 0a09 5072 6f67 7261  :: Only...Progra
-000002c0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-000002d0: 3a20 5079 7468 6f6e 203a 3a20 332e 380d  : Python :: 3.8.
-000002e0: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
-000002f0: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000300: 203a 3a20 332e 390d 0a09 5072 6f67 7261   :: 3.9...Progra
-00000310: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-00000320: 3a20 5079 7468 6f6e 203a 3a20 332e 3130  : Python :: 3.10
-00000330: 0d0a 0954 6f70 6963 203a 3a20 5363 6965  ...Topic :: Scie
-00000340: 6e74 6966 6963 2f45 6e67 696e 6565 7269  ntific/Engineeri
-00000350: 6e67 203a 3a20 496d 6167 6520 5072 6f63  ng :: Image Proc
-00000360: 6573 7369 6e67 0d0a 7072 6f6a 6563 745f  essing..project_
-00000370: 7572 6c73 203d 200d 0a09 4275 6720 5472  urls = ...Bug Tr
-00000380: 6163 6b65 7220 3d20 6874 7470 733a 2f2f  acker = https://
-00000390: 6769 7468 7562 2e63 6f6d 2f68 6165 736c  github.com/haesl
-000003a0: 6569 6e68 7565 7066 2f62 6961 2d62 6f62  einhuepf/bia-bob
-000003b0: 2f69 7373 7565 730d 0a09 446f 6375 6d65  /issues...Docume
-000003c0: 6e74 6174 696f 6e20 3d20 6874 7470 733a  ntation = https:
-000003d0: 2f2f 6769 7468 7562 2e63 6f6d 2f68 6165  //github.com/hae
-000003e0: 736c 6569 6e68 7565 7066 2f62 6961 2d62  sleinhuepf/bia-b
-000003f0: 6f62 2352 4541 444d 452e 6d64 0d0a 0953  ob#README.md...S
-00000400: 6f75 7263 6520 436f 6465 203d 2068 7474  ource Code = htt
-00000410: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000420: 6861 6573 6c65 696e 6875 6570 662f 6269  haesleinhuepf/bi
-00000430: 612d 626f 620d 0a09 5573 6572 2053 7570  a-bob...User Sup
-00000440: 706f 7274 203d 2068 7474 7073 3a2f 2f67  port = https://g
-00000450: 6974 6875 622e 636f 6d2f 6861 6573 6c65  ithub.com/haesle
-00000460: 696e 6875 6570 662f 6269 612d 626f 622f  inhuepf/bia-bob/
-00000470: 6973 7375 6573 0d0a 0d0a 5b6f 7074 696f  issues....[optio
-00000480: 6e73 5d0d 0a70 6163 6b61 6765 7320 3d20  ns]..packages = 
-00000490: 6669 6e64 3a0d 0a69 6e73 7461 6c6c 5f72  find:..install_r
-000004a0: 6571 7569 7265 7320 3d20 0d0a 096e 756d  equires = ...num
-000004b0: 7079 0d0a 0970 7974 686f 6e2d 4c65 7665  py...python-Leve
-000004c0: 6e73 6874 6569 6e3e 3d30 2e32 312e 300d  nshtein>=0.21.0.
-000004d0: 0a09 7363 696b 6974 2d69 6d61 6765 3e3d  ..scikit-image>=
-000004e0: 302e 3139 2e30 0d0a 096c 616e 6763 6861  0.19.0...langcha
-000004f0: 696e 3e3d 302e 302e 3235 310d 0a09 7374  in>=0.0.251...st
-00000500: 6163 6b76 6965 773e 3d30 2e36 2e33 0d0a  ackview>=0.6.3..
-00000510: 7079 7468 6f6e 5f72 6571 7569 7265 7320  python_requires 
-00000520: 3d20 3e3d 332e 380d 0a69 6e63 6c75 6465  = >=3.8..include
-00000530: 5f70 6163 6b61 6765 5f64 6174 6120 3d20  _package_data = 
-00000540: 5472 7565 0d0a 7061 636b 6167 655f 6469  True..package_di
-00000550: 7220 3d20 0d0a 093d 7372 630d 0a0d 0a5b  r = ...=src....[
-00000560: 6f70 7469 6f6e 732e 7061 636b 6167 6573  options.packages
-00000570: 2e66 696e 645d 0d0a 7768 6572 6520 3d20  .find]..where = 
-00000580: 7372 630d 0a0d 0a5b 6f70 7469 6f6e 732e  src....[options.
-00000590: 6578 7472 6173 5f72 6571 7569 7265 5d0d  extras_require].
-000005a0: 0a74 6573 7469 6e67 203d 200d 0a09 746f  .testing = ...to
-000005b0: 780d 0a09 7079 7465 7374 2020 2320 6874  x...pytest  # ht
-000005c0: 7470 733a 2f2f 646f 6373 2e70 7974 6573  tps://docs.pytes
-000005d0: 742e 6f72 672f 656e 2f6c 6174 6573 742f  t.org/en/latest/
-000005e0: 636f 6e74 656e 7473 2e68 746d 6c0d 0a09  contents.html...
-000005f0: 7079 7465 7374 2d63 6f76 2020 2320 6874  pytest-cov  # ht
-00000600: 7470 733a 2f2f 7079 7465 7374 2d63 6f76  tps://pytest-cov
-00000610: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
-00000620: 656e 2f6c 6174 6573 742f 0d0a 0d0a 5b6f  en/latest/....[o
-00000630: 7074 696f 6e73 2e70 6163 6b61 6765 5f64  ptions.package_d
-00000640: 6174 615d 0d0a 2a20 3d20 2a2e 7961 6d6c  ata]..* = *.yaml
-00000650: 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a  ....[egg_info]..
-00000660: 7461 675f 6275 696c 6420 3d20 0d0a 7461  tag_build = ..ta
-00000670: 675f 6461 7465 203d 2030 0d0a 0d0a       g_date = 0....
+000001b0: 202d 2050 7265 2d41 6c70 6861 0d0a 0949   - Pre-Alpha...I
+000001c0: 6e74 656e 6465 6420 4175 6469 656e 6365  ntended Audience
+000001d0: 203a 3a20 4465 7665 6c6f 7065 7273 0d0a   :: Developers..
+000001e0: 094c 6963 656e 7365 203a 3a20 4f53 4920  .License :: OSI 
+000001f0: 4170 7072 6f76 6564 203a 3a20 4253 4420  Approved :: BSD 
+00000200: 4c69 6365 6e73 650d 0a09 4f70 6572 6174  License...Operat
+00000210: 696e 6720 5379 7374 656d 203a 3a20 4f53  ing System :: OS
+00000220: 2049 6e64 6570 656e 6465 6e74 0d0a 0950   Independent...P
+00000230: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000240: 6167 6520 3a3a 2050 7974 686f 6e0d 0a09  age :: Python...
+00000250: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+00000260: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+00000270: 3a20 330d 0a09 5072 6f67 7261 6d6d 696e  : 3...Programmin
+00000280: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+00000290: 7468 6f6e 203a 3a20 3320 3a3a 204f 6e6c  thon :: 3 :: Onl
+000002a0: 790d 0a09 5072 6f67 7261 6d6d 696e 6720  y...Programming 
+000002b0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+000002c0: 6f6e 203a 3a20 332e 380d 0a09 5072 6f67  on :: 3.8...Prog
+000002d0: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+000002e0: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+000002f0: 390d 0a09 5072 6f67 7261 6d6d 696e 6720  9...Programming 
+00000300: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+00000310: 6f6e 203a 3a20 332e 3130 0d0a 0954 6f70  on :: 3.10...Top
+00000320: 6963 203a 3a20 5363 6965 6e74 6966 6963  ic :: Scientific
+00000330: 2f45 6e67 696e 6565 7269 6e67 203a 3a20  /Engineering :: 
+00000340: 496d 6167 6520 5072 6f63 6573 7369 6e67  Image Processing
+00000350: 0d0a 7072 6f6a 6563 745f 7572 6c73 203d  ..project_urls =
+00000360: 200d 0a09 4275 6720 5472 6163 6b65 7220   ...Bug Tracker 
+00000370: 3d20 6874 7470 733a 2f2f 6769 7468 7562  = https://github
+00000380: 2e63 6f6d 2f68 6165 736c 6569 6e68 7565  .com/haesleinhue
+00000390: 7066 2f62 6961 2d62 6f62 2f69 7373 7565  pf/bia-bob/issue
+000003a0: 730d 0a09 446f 6375 6d65 6e74 6174 696f  s...Documentatio
+000003b0: 6e20 3d20 6874 7470 733a 2f2f 6769 7468  n = https://gith
+000003c0: 7562 2e63 6f6d 2f68 6165 736c 6569 6e68  ub.com/haesleinh
+000003d0: 7565 7066 2f62 6961 2d62 6f62 2352 4541  uepf/bia-bob#REA
+000003e0: 444d 452e 6d64 0d0a 0953 6f75 7263 6520  DME.md...Source 
+000003f0: 436f 6465 203d 2068 7474 7073 3a2f 2f67  Code = https://g
+00000400: 6974 6875 622e 636f 6d2f 6861 6573 6c65  ithub.com/haesle
+00000410: 696e 6875 6570 662f 6269 612d 626f 620d  inhuepf/bia-bob.
+00000420: 0a09 5573 6572 2053 7570 706f 7274 203d  ..User Support =
+00000430: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+00000440: 636f 6d2f 6861 6573 6c65 696e 6875 6570  com/haesleinhuep
+00000450: 662f 6269 612d 626f 622f 6973 7375 6573  f/bia-bob/issues
+00000460: 0d0a 0d0a 5b6f 7074 696f 6e73 5d0d 0a70  ....[options]..p
+00000470: 6163 6b61 6765 7320 3d20 6669 6e64 3a0d  ackages = find:.
+00000480: 0a69 6e73 7461 6c6c 5f72 6571 7569 7265  .install_require
+00000490: 7320 3d20 0d0a 096e 756d 7079 0d0a 0970  s = ...numpy...p
+000004a0: 7974 686f 6e2d 4c65 7665 6e73 6874 6569  ython-Levenshtei
+000004b0: 6e3e 3d30 2e32 312e 300d 0a09 7363 696b  n>=0.21.0...scik
+000004c0: 6974 2d69 6d61 6765 3e3d 302e 3139 2e30  it-image>=0.19.0
+000004d0: 0d0a 096c 616e 6763 6861 696e 3e3d 302e  ...langchain>=0.
+000004e0: 302e 3235 310d 0a09 7374 6163 6b76 6965  0.251...stackvie
+000004f0: 773e 3d30 2e36 2e33 0d0a 7079 7468 6f6e  w>=0.6.3..python
+00000500: 5f72 6571 7569 7265 7320 3d20 3e3d 332e  _requires = >=3.
+00000510: 380d 0a69 6e63 6c75 6465 5f70 6163 6b61  8..include_packa
+00000520: 6765 5f64 6174 6120 3d20 5472 7565 0d0a  ge_data = True..
+00000530: 7061 636b 6167 655f 6469 7220 3d20 0d0a  package_dir = ..
+00000540: 093d 7372 630d 0a0d 0a5b 6f70 7469 6f6e  .=src....[option
+00000550: 732e 7061 636b 6167 6573 2e66 696e 645d  s.packages.find]
+00000560: 0d0a 7768 6572 6520 3d20 7372 630d 0a0d  ..where = src...
+00000570: 0a5b 6f70 7469 6f6e 732e 6578 7472 6173  .[options.extras
+00000580: 5f72 6571 7569 7265 5d0d 0a74 6573 7469  _require]..testi
+00000590: 6e67 203d 200d 0a09 746f 780d 0a09 7079  ng = ...tox...py
+000005a0: 7465 7374 2020 2320 6874 7470 733a 2f2f  test  # https://
+000005b0: 646f 6373 2e70 7974 6573 742e 6f72 672f  docs.pytest.org/
+000005c0: 656e 2f6c 6174 6573 742f 636f 6e74 656e  en/latest/conten
+000005d0: 7473 2e68 746d 6c0d 0a09 7079 7465 7374  ts.html...pytest
+000005e0: 2d63 6f76 2020 2320 6874 7470 733a 2f2f  -cov  # https://
+000005f0: 7079 7465 7374 2d63 6f76 2e72 6561 6474  pytest-cov.readt
+00000600: 6865 646f 6373 2e69 6f2f 656e 2f6c 6174  hedocs.io/en/lat
+00000610: 6573 742f 0d0a 0d0a 5b6f 7074 696f 6e73  est/....[options
+00000620: 2e70 6163 6b61 6765 5f64 6174 615d 0d0a  .package_data]..
+00000630: 2a20 3d20 2a2e 7961 6d6c 0d0a 0d0a 5b65  * = *.yaml....[e
+00000640: 6767 5f69 6e66 6f5d 0d0a 7461 675f 6275  gg_info]..tag_bu
+00000650: 696c 6420 3d20 0d0a 7461 675f 6461 7465  ild = ..tag_date
+00000660: 203d 2030 0d0a 0d0a                       = 0....
```

### Comparing `bia-bob-0.1.2/src/bia_bob/_machinery.py` & `bia-bob-0.1.3/src/bia_bob/_machinery.py`

 * *Files identical despite different names*

### Comparing `bia-bob-0.1.2/src/bia_bob/_tools.py` & `bia-bob-0.1.3/src/bia_bob/_tools.py`

 * *Files identical despite different names*

### Comparing `bia-bob-0.1.2/src/bia_bob/_utilities.py` & `bia-bob-0.1.3/src/bia_bob/_utilities.py`

 * *Files identical despite different names*

### Comparing `bia-bob-0.1.2/src/bia_bob.egg-info/PKG-INFO` & `bia-bob-0.1.3/src/bia_bob.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: bia-bob
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Jupyter-based assistant for working on bio-image analysis tasks
 Home-page: https://github.com/haesleinhuepf/bia-bob
 Author: Robert Haase
 Author-email: robert.haase@tu-dresden.de
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/haesleinhuepf/bia-bob/issues
 Project-URL: Documentation, https://github.com/haesleinhuepf/bia-bob#README.md
 Project-URL: Source Code, https://github.com/haesleinhuepf/bia-bob
 Project-URL: User Support, https://github.com/haesleinhuepf/bia-bob/issues
 Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Framework :: napari
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
@@ -58,28 +57,29 @@
 ```
 
 Afterwards, you can ask Bob questions like this:
 ```
 %bob Load blobs.tif and show it
 ```
 
-You can also ask Bob about available tools:
-```
-%bob list tools
-```
-
 Or like this:
 ```
 %%bob
 Please load the image blobs.tif,
 segment bright objects in it, 
 count them and 
 show the segmentation result.
 ```
 
+
+You can also ask Bob about available tools:
+```
+%bob list tools
+```
+
 ## Example gallery
 
 ![img.png](https://github.com/haesleinhuepf/bia-bob/raw/main/docs/images/load_and_show.png)
 
 ![img_1.png](https://github.com/haesleinhuepf/bia-bob/raw/main/docs/images/slice.png)
 
 ![img.png](https://github.com/haesleinhuepf/bia-bob/raw/main/docs/images/chain_workflows.png)
@@ -89,15 +89,15 @@
 ![img.png](https://github.com/haesleinhuepf/bia-bob/raw/main/docs/images/edge_detection.png)
 
 ## Known issues
 
 If you want to ask Bob a question, you need to put a space before the `?`.
 
 ```
-What do you know about blobs.gif?
+What do you know about blobs.gif ?
 ```
 
 ## Installation
 
 ```
 pip install bia-bob
 ```
```

