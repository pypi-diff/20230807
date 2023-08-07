# Comparing `tmp/Truvari-4.0.0.tar.gz` & `tmp/Truvari-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Truvari-4.0.0.tar", last modified: Mon Mar 13 16:27:58 2023, max compression
+gzip compressed data, was "Truvari-4.1.0.tar", last modified: Mon Aug  7 17:50:22 2023, max compression
```

## Comparing `Truvari-4.0.0.tar` & `Truvari-4.1.0.tar`

### file list

```diff
@@ -1,50 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 16:27:58.401760 Truvari-4.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-03-13 16:24:01.000000 Truvari-4.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-03-13 16:27:58.401760 Truvari-4.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-03-13 16:24:01.000000 Truvari-4.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 16:27:58.397760 Truvari-4.0.0/Truvari.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-03-13 16:27:58.000000 Truvari-4.0.0/Truvari.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-03-13 16:27:58.000000 Truvari-4.0.0/Truvari.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 16:27:58.000000 Truvari-4.0.0/Truvari.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-13 16:27:58.000000 Truvari-4.0.0/Truvari.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-03-13 16:27:58.000000 Truvari-4.0.0/Truvari.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-13 16:27:58.000000 Truvari-4.0.0/Truvari.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-13 16:27:58.401760 Truvari-4.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-03-13 16:24:01.000000 Truvari-4.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 16:27:58.401760 Truvari-4.0.0/truvari/
--rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-03-13 16:24:01.000000 Truvari-4.0.0/truvari/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3524 2023-03-13 16:24:01.000000 Truvari-4.0.0/truvari/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-03-13 16:24:01.000000 Truvari-4.0.0/truvari/anno.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 16:27:58.401760 Truvari-4.0.0/truvari/annotations/
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-03-13 16:24:01.000000 Truvari-4.0.0/truvari/annotations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-03-13 16:24:01.000000 Truvari-4.0.0/truvari/annotations/addid.py
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-03-13 16:24:01.000000 Truvari-4.0.0/truvari/annotations/af_calc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-03-13 16:24:01.000000 Truvari-4.0.0/truvari/annotations/bpovl.py
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-03-13 16:24:01.000000 Truvari-4.0.0/truvari/annotations/density.py
--rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-03-13 16:24:01.000000 Truvari-4.0.0/truvari/annotations/dpcnt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-03-13 16:24:01.000000 Truvari-4.0.0/truvari/annotations/gccontent.py
--rw-r--r--   0 runner    (1001) docker     (123)    10402 2023-03-13 16:24:01.000000 Truvari-4.0.0/truvari/annotations/grm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-03-13 16:24:01.000000 Truvari-4.0.0/truvari/annotations/grpaf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-03-13 16:24:01.000000 Truvari-4.0.0/truvari/annotations/gtcnt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-03-13 16:24:01.000000 Truvari-4.0.0/truvari/annotations/hompct.py
--rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-03-13 16:24:01.000000 Truvari-4.0.0/truvari/annotations/lcr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6083 2023-03-13 16:24:01.000000 Truvari-4.0.0/truvari/annotations/numneigh.py
--rw-r--r--   0 runner    (1001) docker     (123)     6935 2023-03-13 16:24:01.000000 Truvari-4.0.0/truvari/annotations/remap.py
--rw-r--r--   0 runner    (1001) docker     (123)     8253 2023-03-13 16:24:01.000000 Truvari-4.0.0/truvari/annotations/repmask.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-03-13 16:24:01.000000 Truvari-4.0.0/truvari/annotations/svinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)    24943 2023-03-13 16:24:01.000000 Truvari-4.0.0/truvari/annotations/trf.py
--rw-r--r--   0 runner    (1001) docker     (123)    27059 2023-03-13 16:24:01.000000 Truvari-4.0.0/truvari/bench.py
--rw-r--r--   0 runner    (1001) docker     (123)    16148 2023-03-13 16:24:01.000000 Truvari-4.0.0/truvari/collapse.py
--rw-r--r--   0 runner    (1001) docker     (123)    18140 2023-03-13 16:24:01.000000 Truvari-4.0.0/truvari/comparisons.py
--rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-03-13 16:24:01.000000 Truvari-4.0.0/truvari/consistency.py
--rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-03-13 16:24:01.000000 Truvari-4.0.0/truvari/divide.py
--rw-r--r--   0 runner    (1001) docker     (123)    11327 2023-03-13 16:24:01.000000 Truvari-4.0.0/truvari/matching.py
--rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-03-13 16:24:01.000000 Truvari-4.0.0/truvari/msa2vcf.py
--rw-r--r--   0 runner    (1001) docker     (123)    15163 2023-03-13 16:24:01.000000 Truvari-4.0.0/truvari/phab.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-03-13 16:24:01.000000 Truvari-4.0.0/truvari/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    12104 2023-03-13 16:24:01.000000 Truvari-4.0.0/truvari/refine.py
--rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-03-13 16:24:01.000000 Truvari-4.0.0/truvari/region_vcf_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-03-13 16:24:01.000000 Truvari-4.0.0/truvari/segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-03-13 16:24:01.000000 Truvari-4.0.0/truvari/stratify.py
--rw-r--r--   0 runner    (1001) docker     (123)    13129 2023-03-13 16:24:01.000000 Truvari-4.0.0/truvari/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14721 2023-03-13 16:24:01.000000 Truvari-4.0.0/truvari/vcf2df.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:50:22.386914 Truvari-4.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-08-07 17:49:16.000000 Truvari-4.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-08-07 17:50:22.386914 Truvari-4.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-08-07 17:49:16.000000 Truvari-4.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:50:22.378914 Truvari-4.1.0/Truvari.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-08-07 17:50:22.000000 Truvari-4.1.0/Truvari.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-08-07 17:50:22.000000 Truvari-4.1.0/Truvari.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 17:50:22.000000 Truvari-4.1.0/Truvari.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-07 17:50:22.000000 Truvari-4.1.0/Truvari.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-08-07 17:50:22.000000 Truvari-4.1.0/Truvari.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-07 17:50:22.000000 Truvari-4.1.0/Truvari.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 17:50:22.386914 Truvari-4.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-08-07 17:49:16.000000 Truvari-4.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:50:22.382914 Truvari-4.1.0/truvari/
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-08-07 17:49:16.000000 Truvari-4.1.0/truvari/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3524 2023-08-07 17:49:16.000000 Truvari-4.1.0/truvari/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-08-07 17:49:16.000000 Truvari-4.1.0/truvari/anno.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:50:22.386914 Truvari-4.1.0/truvari/annotations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-08-07 17:49:16.000000 Truvari-4.1.0/truvari/annotations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-08-07 17:49:16.000000 Truvari-4.1.0/truvari/annotations/addid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-08-07 17:49:16.000000 Truvari-4.1.0/truvari/annotations/af_calc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-08-07 17:49:16.000000 Truvari-4.1.0/truvari/annotations/bpovl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-08-07 17:49:16.000000 Truvari-4.1.0/truvari/annotations/density.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-08-07 17:49:16.000000 Truvari-4.1.0/truvari/annotations/dpcnt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-08-07 17:49:16.000000 Truvari-4.1.0/truvari/annotations/gccontent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10476 2023-08-07 17:49:16.000000 Truvari-4.1.0/truvari/annotations/grm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-08-07 17:49:16.000000 Truvari-4.1.0/truvari/annotations/grpaf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-08-07 17:49:16.000000 Truvari-4.1.0/truvari/annotations/gtcnt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-08-07 17:49:16.000000 Truvari-4.1.0/truvari/annotations/hompct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-08-07 17:49:16.000000 Truvari-4.1.0/truvari/annotations/lcr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6083 2023-08-07 17:49:16.000000 Truvari-4.1.0/truvari/annotations/numneigh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6978 2023-08-07 17:49:16.000000 Truvari-4.1.0/truvari/annotations/remap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8254 2023-08-07 17:49:16.000000 Truvari-4.1.0/truvari/annotations/repmask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-08-07 17:49:16.000000 Truvari-4.1.0/truvari/annotations/svinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25043 2023-08-07 17:49:16.000000 Truvari-4.1.0/truvari/annotations/trf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31260 2023-08-07 17:49:16.000000 Truvari-4.1.0/truvari/bench.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17912 2023-08-07 17:49:16.000000 Truvari-4.1.0/truvari/collapse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18174 2023-08-07 17:49:16.000000 Truvari-4.1.0/truvari/comparisons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-08-07 17:49:16.000000 Truvari-4.1.0/truvari/consistency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-08-07 17:49:16.000000 Truvari-4.1.0/truvari/divide.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11727 2023-08-07 17:49:16.000000 Truvari-4.1.0/truvari/matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-08-07 17:49:16.000000 Truvari-4.1.0/truvari/msatovcf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15539 2023-08-07 17:49:16.000000 Truvari-4.1.0/truvari/phab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16411 2023-08-07 17:49:16.000000 Truvari-4.1.0/truvari/refine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6354 2023-08-07 17:49:16.000000 Truvari-4.1.0/truvari/region_vcf_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-08-07 17:49:16.000000 Truvari-4.1.0/truvari/segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-08-07 17:49:16.000000 Truvari-4.1.0/truvari/stratify.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13289 2023-08-07 17:49:16.000000 Truvari-4.1.0/truvari/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14823 2023-08-07 17:49:16.000000 Truvari-4.1.0/truvari/vcf2df.py
```

### Comparing `Truvari-4.0.0/LICENSE` & `Truvari-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Truvari-4.0.0/PKG-INFO` & `Truvari-4.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: Truvari
-Version: 4.0.0
+Version: 4.1.0
 Summary: Structural variant comparison tool for VCFs
 Home-page: https://github.com/ACEnglish/truvari
 Author: ACEnglish
 Author-email: acenglish@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![PyPI version](https://badge.fury.io/py/Truvari.svg)](https://badge.fury.io/py/Truvari)
 [![pylint](imgs/pylint.svg)](https://github.com/acenglish/truvari/actions/workflows/pylint.yml)
 [![FuncTests](https://github.com/acenglish/truvari/actions/workflows/func_tests.yml/badge.svg?branch=develop&event=push)](https://github.com/acenglish/truvari/actions/workflows/func_tests.yml)
 [![coverage](imgs/coverage.svg)](https://github.com/acenglish/truvari/actions/workflows/func_tests.yml)
-[![develop](https://img.shields.io/github/commits-since/acenglish/truvari/v3.5.0)](https://github.com/ACEnglish/truvari/compare/v3.5.0...develop)
+[![develop](https://img.shields.io/github/commits-since/acenglish/truvari/v4.0.0)](https://github.com/ACEnglish/truvari/compare/v4.0.0...develop)
 [![Downloads](https://pepy.tech/badge/truvari)](https://pepy.tech/project/truvari)
 
 ![Logo](https://raw.githubusercontent.com/ACEnglish/truvari/develop/imgs/BoxScale1_DarkBG.png)  
-Toolkit for benchmarking, merging, and annotating Structrual Variants
+Toolkit for benchmarking, merging, and annotating Structural Variants
 
 📚 [WIKI page](https://github.com/acenglish/truvari/wiki) has detailed documentation.  
 📈 See [Updates](https://github.com/acenglish/truvari/wiki/Updates) on new versions.  
 📝 Read our [Paper](https://genomebiology.biomedcentral.com/articles/10.1186/s13059-022-02840-6) to learn more.
 
 ## 💻 Installation
 Truvari uses Python 3.6+ and can be installed with pip:
```

### Comparing `Truvari-4.0.0/README.md` & `Truvari-4.1.0/Truvari.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,27 @@
+Metadata-Version: 2.1
+Name: Truvari
+Version: 4.1.0
+Summary: Structural variant comparison tool for VCFs
+Home-page: https://github.com/ACEnglish/truvari
+Author: ACEnglish
+Author-email: acenglish@gmail.com
+License: MIT
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 [![PyPI version](https://badge.fury.io/py/Truvari.svg)](https://badge.fury.io/py/Truvari)
 [![pylint](imgs/pylint.svg)](https://github.com/acenglish/truvari/actions/workflows/pylint.yml)
 [![FuncTests](https://github.com/acenglish/truvari/actions/workflows/func_tests.yml/badge.svg?branch=develop&event=push)](https://github.com/acenglish/truvari/actions/workflows/func_tests.yml)
 [![coverage](imgs/coverage.svg)](https://github.com/acenglish/truvari/actions/workflows/func_tests.yml)
-[![develop](https://img.shields.io/github/commits-since/acenglish/truvari/v3.5.0)](https://github.com/ACEnglish/truvari/compare/v3.5.0...develop)
+[![develop](https://img.shields.io/github/commits-since/acenglish/truvari/v4.0.0)](https://github.com/ACEnglish/truvari/compare/v4.0.0...develop)
 [![Downloads](https://pepy.tech/badge/truvari)](https://pepy.tech/project/truvari)
 
 ![Logo](https://raw.githubusercontent.com/ACEnglish/truvari/develop/imgs/BoxScale1_DarkBG.png)  
-Toolkit for benchmarking, merging, and annotating Structrual Variants
+Toolkit for benchmarking, merging, and annotating Structural Variants
 
 📚 [WIKI page](https://github.com/acenglish/truvari/wiki) has detailed documentation.  
 📈 See [Updates](https://github.com/acenglish/truvari/wiki/Updates) on new versions.  
 📝 Read our [Paper](https://genomebiology.biomedcentral.com/articles/10.1186/s13059-022-02840-6) to learn more.
 
 ## 💻 Installation
 Truvari uses Python 3.6+ and can be installed with pip:
```

### Comparing `Truvari-4.0.0/Truvari.egg-info/PKG-INFO` & `Truvari-4.1.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,16 @@
-Metadata-Version: 2.1
-Name: Truvari
-Version: 4.0.0
-Summary: Structural variant comparison tool for VCFs
-Home-page: https://github.com/ACEnglish/truvari
-Author: ACEnglish
-Author-email: acenglish@gmail.com
-License: MIT
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![PyPI version](https://badge.fury.io/py/Truvari.svg)](https://badge.fury.io/py/Truvari)
 [![pylint](imgs/pylint.svg)](https://github.com/acenglish/truvari/actions/workflows/pylint.yml)
 [![FuncTests](https://github.com/acenglish/truvari/actions/workflows/func_tests.yml/badge.svg?branch=develop&event=push)](https://github.com/acenglish/truvari/actions/workflows/func_tests.yml)
 [![coverage](imgs/coverage.svg)](https://github.com/acenglish/truvari/actions/workflows/func_tests.yml)
-[![develop](https://img.shields.io/github/commits-since/acenglish/truvari/v3.5.0)](https://github.com/ACEnglish/truvari/compare/v3.5.0...develop)
+[![develop](https://img.shields.io/github/commits-since/acenglish/truvari/v4.0.0)](https://github.com/ACEnglish/truvari/compare/v4.0.0...develop)
 [![Downloads](https://pepy.tech/badge/truvari)](https://pepy.tech/project/truvari)
 
 ![Logo](https://raw.githubusercontent.com/ACEnglish/truvari/develop/imgs/BoxScale1_DarkBG.png)  
-Toolkit for benchmarking, merging, and annotating Structrual Variants
+Toolkit for benchmarking, merging, and annotating Structural Variants
 
 📚 [WIKI page](https://github.com/acenglish/truvari/wiki) has detailed documentation.  
 📈 See [Updates](https://github.com/acenglish/truvari/wiki/Updates) on new versions.  
 📝 Read our [Paper](https://genomebiology.biomedcentral.com/articles/10.1186/s13059-022-02840-6) to learn more.
 
 ## 💻 Installation
 Truvari uses Python 3.6+ and can be installed with pip:
```

### Comparing `Truvari-4.0.0/Truvari.egg-info/SOURCES.txt` & `Truvari-4.1.0/Truvari.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -12,17 +12,16 @@
 truvari/anno.py
 truvari/bench.py
 truvari/collapse.py
 truvari/comparisons.py
 truvari/consistency.py
 truvari/divide.py
 truvari/matching.py
-truvari/msa2vcf.py
+truvari/msatovcf.py
 truvari/phab.py
-truvari/pipeline.py
 truvari/refine.py
 truvari/region_vcf_iter.py
 truvari/segmentation.py
 truvari/stratify.py
 truvari/utils.py
 truvari/vcf2df.py
 truvari/annotations/__init__.py
```

### Comparing `Truvari-4.0.0/setup.py` & `Truvari-4.1.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -57,18 +57,19 @@
     long_description_content_type='text/markdown',
     entry_points={
       'console_scripts': [
          'truvari = truvari.__main__:main'
       ]
     },
     install_requires=[
-        "rich==12.5.1",
+        "pywfa>=0.5.1",
+        "rich>=12.5.1",
         "edlib>=1.3.9",
         "pysam>=0.15.2",
         "intervaltree>=3.0.2",
-        "joblib>=1.0.1",
+        "joblib>=1.2.0",
         "numpy>=1.23.3",
         "pytabix>=0.1",
         "bwapy>=0.1.4",
         "pandas>=1.4.4"
     ],
 )
```

### Comparing `Truvari-4.0.0/truvari/__init__.py` & `Truvari-4.1.0/truvari/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,30 +34,28 @@
 :meth:`get_scalebin`
 :meth:`get_sizebin`
 :meth:`get_svtype`
 :meth:`msa2vcf`
 :meth:`overlap_percent`
 :meth:`overlaps`
 :meth:`phab`
-:meth:`phab_multi`
 :meth:`reciprocal_overlap`
 :meth:`ref_ranges`
 :meth:`seqsim`
 :meth:`sizesim`
 :meth:`unroll_compare`
 :meth:`vcf_ranges`
 
 Dev methods:
 
 :meth:`benchdir_count_entries`
 :meth:`chunker`
 :meth:`cmd_exe`
 :meth:`consolidate_phab_vcfs`
 :meth:`count_entries`
-:meth:`fchain`
 :meth:`file_zipper`
 :meth:`help_unknown_cmd`
 :meth:`make_temp_filename`
 :meth:`opt_gz_open`
 :meth:`optimize_df_memory`
 :meth:`performance_metrics`
 :meth:`restricted_float`
@@ -83,15 +81,15 @@
 :data:`truvari.QUALBINS`
 :data:`truvari.SVTYTYPE`
 :data:`truvari.SZBINMAX`
 :data:`truvari.SZBINS`
 :data:`truvari.SZBINTYPE`
 """
 
-__version__ = '4.0.0'
+__version__ = '4.1.0'
 
 
 from truvari.annotations.af_calc import (
     allele_freq_annos,
     calc_af,
     calc_hwe
 )
@@ -129,26 +127,20 @@
 from truvari.matching import (
     MatchResult,
     Matcher,
     chunker,
     file_zipper
 )
 
-from truvari.msa2vcf import (
+from truvari.msatovcf import (
     msa2vcf
 )
 
-from truvari.pipeline import (
-    fchain
-)
-
 from truvari.phab import (
     phab,
-    phab_multi,
-    consolidate_phab_vcfs
 )
 
 from truvari.region_vcf_iter import (
     RegionVCFIterator,
     build_anno_tree
 )
```

### Comparing `Truvari-4.0.0/truvari/__main__.py` & `Truvari-4.1.0/truvari/__main__.py`

 * *Files identical despite different names*

### Comparing `Truvari-4.0.0/truvari/anno.py` & `Truvari-4.1.0/truvari/anno.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,43 +2,48 @@
 Wrapper around the different annotations available
 """
 import argparse
 from rich.console import Console
 import truvari.annotations as tannos
 
 ANNOS = {
-         "addid": ("Set ID field", tannos.addid_main),
-         "bpovl": ("Annotation Intersection", tannos.bpovl_main),
-         "density": ("Variant Density", tannos.density_main),
-         "dpcnt": ("Call Depth Counts", tannos.dpcnt_main),
-         "gcpct": ("GC Percent", tannos.gcpct_main),
-         "grm": ("Mappability", tannos.grm_main),
-         "grpaf": ("Sample Group Allele Frequency", tannos.grpaf_main),
-         "gtcnt": ("Genotype Counts", tannos.gtcnt_main),
-         "hompct": ("Homozygous Percent", tannos.hompct_main),
-         "lcr": ("Low-complexity Regions", tannos.lcr_main),
-         "numneigh": ("Number of Neighbors", tannos.numneigh_main),
-         "remap": ("Allele Remapping", tannos.remap_main),
-         "repmask": ("Repeats", tannos.rmk_main),
-         "svinfo": ("SVINFO Fields", tannos.svinfo_main),
-         "trf": ("Tandem Repeats", tannos.trf_main)
-         }
+    "addid": ("Set ID field", tannos.addid_main),
+    "bpovl": ("Annotation Intersection", tannos.bpovl_main),
+    "density": ("Variant Density", tannos.density_main),
+    "dpcnt": ("Call Depth Counts", tannos.dpcnt_main),
+    "gcpct": ("GC Percent", tannos.gcpct_main),
+    "grm": ("Mappability", tannos.grm_main),
+    "grpaf": ("Sample Group Allele Frequency", tannos.grpaf_main),
+    "gtcnt": ("Genotype Counts", tannos.gtcnt_main),
+    "hompct": ("Homozygous Percent", tannos.hompct_main),
+    "lcr": ("Low-complexity Regions", tannos.lcr_main),
+    "numneigh": ("Number of Neighbors", tannos.numneigh_main),
+    "remap": ("Allele Remapping", tannos.remap_main),
+    "repmask": ("Repeats", tannos.rmk_main),
+    "svinfo": ("SVINFO Fields", tannos.svinfo_main),
+    "trf": ("Tandem Repeats", tannos.trf_main)
+}
 
 
-USAGE = "Truvari annotations:\n" + "\n".join([f"    [bold][cyan]{k:9}[/][/] {t[0]}" for k,t in ANNOS.items()])
+USAGE = "Truvari annotations:\n" + \
+    "\n".join(
+        [f"    [bold][cyan]{k:9}[/][/] {t[0]}" for k, t in ANNOS.items()])
+
 
 class ArgumentParser(argparse.ArgumentParser):
     """
     Custom ArgumentParser
     """
+
     def _print_message(self, message, file=None):
         """ pretty print """
         console = Console(stderr=True)
         console.print(message, highlight=False)
 
+
 def parseArgs(args):
     """
     Argument parsing
     """
     parser = ArgumentParser(prog="truvari anno", description=USAGE,
                             formatter_class=argparse.RawDescriptionHelpFormatter)
```

### Comparing `Truvari-4.0.0/truvari/annotations/__init__.py` & `Truvari-4.1.0/truvari/annotations/__init__.py`

 * *Files identical despite different names*

### Comparing `Truvari-4.0.0/truvari/annotations/addid.py` & `Truvari-4.1.0/truvari/annotations/addid.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 Sets an ID to variants
 """
 import logging
 import argparse
 
 import truvari
 
+
 def parse_args(args):
     """
     Pull the command line parameters
     """
     parser = argparse.ArgumentParser(prog="addid", description=__doc__,
                                      formatter_class=argparse.RawDescriptionHelpFormatter)
     parser.add_argument("input", nargs="?", type=str, default="/dev/stdin",
@@ -25,27 +26,28 @@
     Get string's tab positions
     """
     ret = [0]
     for _ in range(8):
         ret.append(line.index('\t', ret[-1] + 1))
     return ret
 
+
 def addid_main(cmdargs):
     """
     Main method
     """
     args = parse_args(cmdargs)
     fh = truvari.opt_gz_open(args.input)
 
     cnt = 0
     with open(args.output, 'w') as fout:
         for line in fh:
             if line[0] == "#":
                 fout.write(line)
                 continue
             tabs = get_idx(line)
-            new_id = line[:tabs[1]].replace('chr','') + hex(cnt)
+            new_id = line[:tabs[1]].replace('chr', '') + hex(cnt)
             fout.write(line[:tabs[2] + 1])
             fout.write(new_id)
             fout.write(line[tabs[3]:])
             cnt += 1
     logging.info("Finished addid")
```

### Comparing `Truvari-4.0.0/truvari/annotations/af_calc.py` & `Truvari-4.1.0/truvari/annotations/af_calc.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 """
 Extra methods for calculating Allele Fequency annotations
 Calculations are python implementations of bcftools +fill_tags
 (https://samtools.github.io/bcftools/) Results are within 1e-6
 difference of bcftools +fill_tags
 """
-from collections import Counter
-
 import numpy as np
 
 
 def calc_hwe(nref, nalt, nhet):
     """
     Calculate Hardy Weinberg equilibrium and excess heterozygosity
 
@@ -69,54 +67,75 @@
 
     probs = probs / my_sum
 
     p_exc_het = probs[nhet:].sum()
     p_hwe = min(probs[probs > probs[nhet]].sum(), 1)
     return p_exc_het, 1 - p_hwe
 
+
 def calc_af(gts):
     """
     Calculate allele annotations for a list of genotypes
 
     :param `gts`: Genotype tuples
     :type `gts`: list
 
     :return: | Dictonary of
              | AF - allele frequency
              | MAF - minor allele frequency
              | ExcHet - excess heterozygosity
              | HWE - hardy weinberg equilibrium
-             | AC - allele count for GT 0 and 1
+             | AC - allele count for GT 1
              | MAC - minor allele count
              | AN - number of called alleles
+             | N_HEMI - Number of partial genotypes (length of 1 or a single missing)
+             | N_HOMREF - homozygous reference GT count
+             | N_HET - heterozygous GT count
+             | N_HOMALT - homozygous alternate GT count
+             | N_MISS - Number of missing genotypes (all .)
     :rtype: dict
     """
-    an = 0
-    n_het = 0
-    cnt = Counter()  # 0 or 1 allele counts
+    ret = {"AF": 0, "MAF": 0, "ExcHet": 0, "HWE": 0, "MAC": 0, "AC": [0, 0], "AN": 0,
+           "N_HEMI": 0, "N_HOMREF": 0, "N_HET": 0, "N_HOMALT": 0, "N_MISS": 0}
     for g in gts:
         if len(g) > 2:
             continue
         for j in g:
             if j is not None:
-                an += 1
-                cnt[j] += 1
+                ret["AN"] += 1
+                ret["AC"][j] += 1
         if len(g) == 2:
-            n_het += 1 if g[0] != g[1] and None not in g else 0
-
-    if an == 0:
-        return {"AF": 0, "MAF": 0, "ExcHet": 0, "HWE": 0, "MAC": 0, "AC": [0, 0], "AN": 0}
-    af = cnt[1] / an
-    srt = [(v, k) for k, v in sorted(cnt.items(), key=lambda item: item[1])]
-    ac = [cnt[_] for _ in [0, 1]]
-    mac = srt[0][0]
-    maf = 1 - (srt[-1][0] / an)
+            if g[0] == g[1]:
+                if g[0] == 0:
+                    ret["N_HOMREF"] += 1
+                elif g[0] is None:
+                    ret["N_MISS"] += 1
+                else:
+                    ret["N_HOMALT"] += 1
+            else:
+                if g[0] is None or g[1] is None:
+                    ret["N_HEMI"] += 1
+                else:
+                    ret["N_HET"] += 1
+        else:
+            if g[0] is None:
+                ret["N_MISS"] += 1
+            else:
+                ret["N_HEMI"] += 1
+
+    if ret["AN"] == 0:
+        return ret
+    ret["AF"] = ret["AC"][1] / ret["AN"]
+    ret["MAC"] = min(ret["AC"])
+    ret["MAF"] = ret["MAC"] / ret["AN"]
+
+    ret["ExcHet"], ret["HWE"] = calc_hwe(
+        ret["AC"][0], ret["AC"][1], ret["N_HET"])
+    return ret
 
-    p_exc_het, p_hwe = calc_hwe(cnt[0], cnt[1], n_het)
-    return {"AF": af, "MAF": maf, "ExcHet": p_exc_het, "HWE": p_hwe, "MAC": mac, "AC": ac, "AN": an}
 
 def allele_freq_annos(entry, samples=None):
     """
     Calculate allele annotations for a VCF Entry
 
     :param `entry`: Entry with samples to parse
     :type `entry`: :class:`pysam.VariantRecord`
@@ -134,13 +153,13 @@
     :rtype: dict
 
     Example
         >>> import truvari
         >>> import pysam
         >>> v = pysam.VariantFile('repo_utils/test_files/variants/multi.vcf.gz')
         >>> truvari.allele_freq_annos(next(v))
-        {'AF': 0.5, 'MAF': 0.5, 'ExcHet': 1.0, 'HWE': 1.0, 'MAC': 1, 'AC': [1, 1], 'AN': 2}
+        {'AF': 0.5, 'MAF': 0.5, 'ExcHet': 1.0, 'HWE': 1.0, 'MAC': 1, 'AC': [1, 1], 'AN': 2, 'N_HEMI': 0, 'N_HOMREF': 0, 'N_HET': 1, 'N_HOMALT': 0, 'N_MISS': 2}
     """
     if samples is None:
         samples = list(entry.samples.keys())
     gts = [entry.samples[_]["GT"] for _ in samples]
     return calc_af(gts)
```

### Comparing `Truvari-4.0.0/truvari/annotations/bpovl.py` & `Truvari-4.1.0/truvari/annotations/bpovl.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,14 +61,15 @@
     """
     Main method
     """
     args = parse_args(cmdargs)
     in_vcf = pysam.VariantFile(args.input)
     anno_tree, anno_cnt = truvari.build_anno_tree(args.anno, *args.anno_psets)
     logging.info("Loaded %d annotations", anno_cnt)
+
     def _transform():
         hit_cnt = 0
         for entry in in_vcf:
             has_hit = False
 
             start, end = truvari.entry_boundaries(entry)
             span = abs(end - start)
```

### Comparing `Truvari-4.0.0/truvari/annotations/density.py` & `Truvari-4.1.0/truvari/annotations/density.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import pysam
 import joblib
 import pandas as pd
 from intervaltree import IntervalTree
 
 import truvari
 
+
 def parse_args(args):
     """
     Parse arguments
     """
     parser = argparse.ArgumentParser(prog="density", description=__doc__,
                                      formatter_class=argparse.RawDescriptionHelpFormatter)
     parser.add_argument("-g", "--genome", type=str, required=True,
@@ -23,20 +24,23 @@
                         help="Input VCF (%(default)s)")
     parser.add_argument("-o", "--output", type=str, required=True,
                         help="Output joblib DataFrame")
     parser.add_argument("-m", "--mask", type=str,
                         help="Mask bed file")
     parser.add_argument("-w", "--windowsize", type=truvari.restricted_int, default=10000,
                         help="Window size (%(default)s)")
+    parser.add_argument("-s", "--stepsize", type=truvari.restricted_int, default=10000,
+                        help="Window step size (%(default)s)")
     parser.add_argument("-t", "--threshold", type=float, default=3,
                         help="std for identifying 'dense' regions (%(default)s)")
     args = parser.parse_args(args)
     truvari.setup_logging(show_version=True)
     return args
 
+
 def density_main(args):
     """
     Main
     """
     args = parse_args(args)
     tree, cnt = truvari.build_anno_tree(args.genome)
     logging.info("Loaded %d seqs from genome", cnt)
@@ -55,16 +59,17 @@
         logging.info("Masked %d regions", mask_cnt)
 
     # setting new indexes after masking
     new_tree = defaultdict(IntervalTree)
     cnt = 0
     for chrom in tree:
         for intv in tree[chrom]:
-            for i in range(intv.begin, intv.end, args.windowsize):
-                new_tree[chrom].addi(i, min(intv.end, i + args.windowsize), data=cnt)
+            for i in range(intv.begin, intv.end, args.stepsize):
+                new_tree[chrom].addi(
+                    i, min(intv.end, i + args.windowsize), data=cnt)
                 cnt += 1
     logging.info("Made %d %dbp windows", cnt, args.windowsize)
     tree = new_tree
 
     # Counting
     counts = Counter()
     v = pysam.VariantFile(args.input)
@@ -81,15 +86,17 @@
         for intv in tree[chrom]:
             data.append([chrom, intv.begin, intv.end, counts[intv.data]])
     data = pd.DataFrame(data, columns=['chrom', 'start', 'end', 'count'])
     # Do the hotspot work
     desc = data["count"].describe()
     logging.info("Summary\n%s", str(desc))
     hs_threshold = desc["mean"] + (args.threshold * desc["std"])
-    logging.info("Setting threshold %f * SD = %f", args.threshold, hs_threshold)
+    logging.info("Setting threshold %f * SD = %f",
+                 args.threshold, hs_threshold)
 
     data["anno"] = None
     data.loc[data["count"] == 0, "anno"] = "sparse"
     data.loc[data["count"] > hs_threshold, "anno"] = "dense"
-    logging.info("Density Counts\n%s", str(data["anno"].value_counts(dropna=False)))
+    logging.info("Density Counts\n%s", str(
+        data["anno"].value_counts(dropna=False)))
 
     joblib.dump(data, args.output)
```

### Comparing `Truvari-4.0.0/truvari/annotations/dpcnt.py` & `Truvari-4.1.0/truvari/annotations/dpcnt.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import bisect
 import logging
 import argparse
 
 import pysam
 import truvari
 
+
 def parse_args(args):
     """
     Pull the command line parameters
     """
     parser = argparse.ArgumentParser(prog="dpcnt", description=__doc__,
                                      formatter_class=argparse.RawDescriptionHelpFormatter)
     parser.add_argument("input", nargs="?", type=str, default="/dev/stdin",
@@ -30,20 +31,22 @@
 
 
 def edit_header(my_vcf, bins, add_ad=False):
     """
     Add INFO for new field to vcf
     """
     header = my_vcf.header.copy()
-    desc = 'Description="Count of samples with >= ' + ",".join([f"{_}x" for _ in bins][:-1]) + '">'
+    desc = 'Description="Count of samples with >= ' + \
+        ",".join([f"{_}x" for _ in bins][:-1]) + '">'
     header.add_line('##INFO=<ID=DPCNT,Number=.,Type=Integer,' + desc)
     if add_ad:
         header.add_line('##INFO=<ID=ADCNT,Number=.,Type=Integer,' + desc)
     return header
 
+
 def add_dpcnt(vcf, n_header=None, bins=None, add_ad=False, present=False):
     """
     Adds DPCNT to each entry in VCF and yields them
     """
     if bins is None:
         bins = [0, 5, 10, 15, sys.maxsize]
 
@@ -70,14 +73,15 @@
 
         entry.translate(n_header)
         entry.info["DPCNT"] = dat
         if add_ad:
             entry.info["ADCNT"] = dat_ad
         yield entry
 
+
 def dpcnt_main(cmdargs):
     """
     Main method
     """
     args = parse_args(cmdargs)
     try:
         bins = [int(_) for _ in args.bins.split(',')]
```

### Comparing `Truvari-4.0.0/truvari/annotations/gccontent.py` & `Truvari-4.1.0/truvari/annotations/gccontent.py`

 * *Files identical despite different names*

### Comparing `Truvari-4.0.0/truvari/annotations/grm.py` & `Truvari-4.1.0/truvari/annotations/grm.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 # pylint: disable=too-many-locals
 import sys
 import re
 import types
 import logging
 import argparse
+import functools
 import multiprocessing
 from collections import namedtuple
 
 import pysam
 import tabix
 import joblib
 import pandas as pd
@@ -26,17 +27,14 @@
 try:
     from setproctitle import setproctitle  # pylint: disable=import-error,useless-suppression
 except ModuleNotFoundError:
     def setproctitle(_):
         """ dummy function """
         return
 
-# Data shared with workers; must be populated before workers are started.
-grm_shared = types.SimpleNamespace()
-
 
 def make_kmers(ref, entry, kmer=25):
     """
     Make ref/alt kmers
     kmer should be half the kmer size you're actually trying to make
     Returns 4 kmers
     ref up, ref dn, alt up, alt dn
@@ -209,42 +207,43 @@
                  start,
                  start + len(ref),  # stop
                  ref,
                  alts,
                  info_dict)
 
 
-def read_vcf_lines(ref_name, start, stop):
+def read_vcf_lines(in_fn, ref_name, start, stop):
     """
     Faster VCF parsing
     """
     logging.debug(f"Starting region {ref_name}:{start}-{stop}")
 
-    tb = tabix.open(grm_shared.input)
+    tb = tabix.open(in_fn)
     try:
         yield from tb.query(ref_name, start, stop)
     except tabix.TabixError as e:
         logging.warning(f"Region {ref_name}:{start}-{stop} failed: {e}")
     setproctitle(f"grm done {ref_name}:{start}-{stop}")
     logging.debug(f"Done region {ref_name}:{start}-{stop}")
 
 
-def process_entries(ref_section):
+def process_entries(ref_section, grm_shared):
     """
     Calculate GRMs for a set of vcf entries
     """
+    grm_shared.aligner = BwaAligner(grm_shared.ref_filename, '-a')
     ref_name, start, stop = ref_section
     ref = pysam.FastaFile(grm_shared.ref_filename)
     aligner = grm_shared.aligner
     kmersize = grm_shared.kmersize
     header = grm_shared.header
     minsize = grm_shared.min_size
     rows = []
     next_progress = 0
-    for line in read_vcf_lines(ref_name, start, stop):
+    for line in read_vcf_lines(grm_shared.input, ref_name, start, stop):
         if "SVLEN" not in line[7] and abs(len(line[3]) - len(line[4])) < minsize:
             continue
         entry = line_to_entry(line)
         if next_progress == 0:
             next_progress = 1000
             setproctitle(
                 f"grm processing {entry.chrom}:{entry.start} in {ref_name}:{start}-{stop}")
@@ -301,28 +300,30 @@
         sys.exit(1)
     args = parse_args(cmdargs)
     if not args.regions:
         m_ranges = truvari.ref_ranges(args.reference)
     else:
         m_ranges = truvari.bed_ranges(args.regions)
 
-    grm_shared.aligner = BwaAligner(args.reference, '-a')
     header = ["key"]
     for prefix in ["rup_", "rdn_", "aup_", "adn_"]:
         for key in ["nhits", "avg_q", "avg_ed", "avg_mat", "avg_mis", "dir_hits", "com_hits", "max_q",
                     "max_ed", "max_mat", "max_mis", "max_strand",
                     "min_q", "min_ed", "min_mat", "min_mis", "min_strand"]:
             header.append(prefix + key)
+    grm_shared = types.SimpleNamespace()
     grm_shared.header = header
     grm_shared.ref_filename = args.reference
     grm_shared.kmersize = args.kmersize
     grm_shared.input = args.input
     grm_shared.min_size = args.min_size
+    m_process_entries = functools.partial(
+        process_entries, grm_shared=grm_shared)
     with multiprocessing.Pool(args.threads, maxtasksperchild=1) as pool:
         logging.info("Processing")
-        chunks = pool.imap(process_entries, m_ranges)
+        chunks = pool.imap(m_process_entries, m_ranges)
         pool.close()
         data = pd.concat(chunks, ignore_index=True)
         logging.info("Saving; df shape %s", data.shape)
         joblib.dump(data, args.output)
         logging.info("Finished grm")
         pool.join()
```

### Comparing `Truvari-4.0.0/truvari/annotations/grpaf.py` & `Truvari-4.1.0/truvari/annotations/grpaf.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,15 +20,15 @@
                         help="VCF to annotate ")
     parser.add_argument("-o", "--output", type=str, default="/dev/stdout",
                         help="Output filename (stdout)")
     parser.add_argument("-l", "--labels", type=str, required=True,
                         help="Tab-delimited file of sample and group")
     parser.add_argument("-t", "--tags", type=str, default='all',
                         help=("Comma-separated list of tags to add "
-                        "from AF,MAF,ExcHet,HWE,MAC,AC,AN (%(default)s)"))
+                              "from AF,MAF,ExcHet,HWE,MAC,AC,AN (%(default)s)"))
     parser.add_argument("--strict", action="store_true",
                         help="Exit if sample listed in labels is not present in VCF (%(default)s)")
     parser.add_argument("--debug", action="store_true",
                         help="Verbose logging")
     args = parser.parse_args(args)
     truvari.setup_logging(args.debug, show_version=True)
     return args
@@ -36,40 +36,55 @@
 
 def edit_header(header, tags, groups):
     """
     Add the header information
     """
     tmpl = '##INFO=<ID={mid},Type={mty},Number={mnum},Description="{desc}">'
     tag_meta = {}
-    tag_meta["AF"] = ("Float", '1', "Allele Frequency on {count} {grp} samples")
-    tag_meta["AN"] = ("Integer", '1', "Total number of alleles in called genotypes on {count} {grp} samples")
-    tag_meta["MAF"] = ("Float", '1', "Minor Allele Frequency on {count} {grp} samples")
+    tag_meta["AF"] = (
+        "Float", '1', "Allele Frequency on {count} {grp} samples")
+    tag_meta["AN"] = (
+        "Integer", '1', "Total number of alleles in called genotypes on {count} {grp} samples")
+    tag_meta["MAF"] = (
+        "Float", '1', "Minor Allele Frequency on {count} {grp} samples")
     tag_meta["AC"] = ("Integer", 'A', "Allele Count on {count} {grp} samples")
-    tag_meta["MAC"] = ("Integer", 'A', "Minor Allele Count on {count} {grp} samples")
-    tag_meta["HWE"] = ("Float", '1', "HWE test (PMID:15789306) on {count} {grp} samples; 1=good, 0=bad")
-    tag_meta["ExcHet"] = ("Float", '1', "Test excess heterozygosity on {count} {grp} samples; 1=good, 0=bad")
+    tag_meta["MAC"] = (
+        "Integer", 'A', "Minor Allele Count on {count} {grp} samples")
+    tag_meta["HWE"] = (
+        "Float", '1', "HWE test (PMID:15789306) on {count} {grp} samples; 1=good, 0=bad")
+    tag_meta["ExcHet"] = (
+        "Float", '1', "Test excess heterozygosity on {count} {grp} samples; 1=good, 0=bad")
+    tag_meta["N_HEMI"] = (
+        "Integer", '1', "Number of partial genotypes (length of 1 or a single missing allele)")
+    tag_meta["N_MISS"] = (
+        "Integer", '1', "Number of missing genotypes (all alleles missing)")
+    tag_meta["N_HOMREF"] = ("Integer", '1', "Number of REF/REF genotypes")
+    tag_meta["N_HET"] = ("Integer", '1', "Number of REF/ALT genotypes")
+    tag_meta["N_HOMALT"] = ("Integer", '1', "Number of ALT/ALT genotypes")
 
     cnts = groups["group"].value_counts()
     for g_name, g_count in zip(cnts.index, cnts):
         for t in tags:
             m_id = f"{t}_{g_name}"
             m_ty, m_num, m_desc = tag_meta[t]
             m_desc = m_desc.format(grp=g_name, count=g_count)
             m_line = tmpl.format(mid=m_id, mty=m_ty, mnum=m_num, desc=m_desc)
             header.add_line(m_line)
 
     return header
 
+
 def grpaf_main(cmd_args):
     """
     Main
     """
     args = parse_args(cmd_args)
     # validate tags
-    all_tags = ["AF", "MAF", "ExcHet", "HWE", "MAC", "AC", "AN"]
+    all_tags = ["AF", "MAF", "ExcHet", "HWE", "MAC", "AC", "AN", "N_HEMI", "N_MISS",
+                "N_HOMREF", "N_HET", "N_HOMALT"]
     if args.tags == 'all':
         args.tags = all_tags
     else:
         args.tags = args.tags.split(',')
         unk_tags = set(args.tags) - set(all_tags)
         if unk_tags:
             logging.error("Unknown --tags %s", " ".join(unk_tags))
```

### Comparing `Truvari-4.0.0/truvari/annotations/gtcnt.py` & `Truvari-4.1.0/truvari/annotations/gtcnt.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     """
     Adds GTCNT to each entry in VCF and yields them
     """
     if n_header is None:
         n_header = edit_header(vcf)
     for entry in vcf:
         cnt = [0, 0, 0, 0]
-        #cnt = {"UNK": 0, "REF": 0, "HET": 0, "HOM": 0}
+        # cnt = {"UNK": 0, "REF": 0, "HET": 0, "HOM": 0}
         for sample in entry.samples:
             gt = entry.samples[sample]["GT"]
             if None in gt or len(gt) != 2:
                 cnt[0] += 1
             elif gt[0] == gt[1] and gt[0] == 0:
                 cnt[1] += 1
             elif gt[0] == gt[1]:
```

### Comparing `Truvari-4.0.0/truvari/annotations/hompct.py` & `Truvari-4.1.0/truvari/annotations/hompct.py`

 * *Files identical despite different names*

### Comparing `Truvari-4.0.0/truvari/annotations/lcr.py` & `Truvari-4.1.0/truvari/annotations/lcr.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import logging
 import argparse
 
 import pysam
 
 import truvari
 
+
 def sequence_to_repvec(sequence, N):
     """
     Computes the repetition vector (as seen in Wooton, 1993) from a
     given sequence of a biopolymer with `N` possible residues.
 
     :param sequence: the nucleotide or protein sequence to generate a repetition vector for.
     :param N: the total number of possible residues in the biopolymer `sequence` belongs to.
@@ -33,14 +34,15 @@
             break
 
     while len(repvec) < N:
         repvec.append(0)
 
     return sorted(repvec, reverse=True)
 
+
 def sequence_entropy(sequence, N=4):
     """
     Computes the Shannon Entropy of a given sequence of a
     biopolymer with `N` possible residues. See (Wooton, 1993)
     for more.
 
     :param sequence: the nucleotide or protein sequence whose Shannon Entropy is to calculated.
@@ -50,49 +52,54 @@
 
     L = len(sequence)
 
     entropy = sum((-1*(n/L)*math.log((n/L), N) for n in repvec if n != 0))
 
     return entropy
 
+
 def edit_header(my_vcf):
     """
     Add INFO for new field to vcf
     """
     header = my_vcf.header.copy()
     header.add_line(('##INFO=<ID=LCR,Number=1,Type=Float,'
                      'Description="Low complexity region entropy score">'))
     return header
 
+
 def add_lcr(vcf, n_header):
     """
     Adds LCR to each entry in VCF and yields them
     """
     if not n_header:
         n_header = edit_header(vcf)
     for entry in vcf:
-        seq = entry.alts[0] if len(entry.alts[0]) > len(entry.ref) else entry.ref
+        seq = entry.alts[0] if len(entry.alts[0]) > len(
+            entry.ref) else entry.ref
         score = sequence_entropy(seq)
         entry.translate(n_header)
         entry.info["LCR"] = score
         yield entry
 
+
 def parse_args(args):
     """
     Pull the command line parameters
     """
     parser = argparse.ArgumentParser(prog="lcr", description=__doc__,
                                      formatter_class=argparse.RawDescriptionHelpFormatter)
     parser.add_argument("input", nargs="?", type=str, default="/dev/stdin",
                         help="VCF to annotate (stdin)")
     parser.add_argument("-o", "--output", type=str, default="/dev/stdout",
                         help="Output filename (stdout)")
     truvari.setup_logging(show_version=True)
     return parser.parse_args(args)
 
+
 def lcr_main(cmdargs):
     """
     Main
     """
     args = parse_args(cmdargs)
     vcf = pysam.VariantFile(args.input)
     n_header = edit_header(vcf)
```

### Comparing `Truvari-4.0.0/truvari/annotations/numneigh.py` & `Truvari-4.1.0/truvari/annotations/numneigh.py`

 * *Files identical despite different names*

### Comparing `Truvari-4.0.0/truvari/annotations/remap.py` & `Truvari-4.1.0/truvari/annotations/remap.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,15 +119,16 @@
         Annotates entries in the vcf and writes to new vcf
         """
         if truvari.entry_size(entry) >= self.min_length:
             entry.translate(self.n_header)
             remap, hits = self.remap_entry(entry)
             entry.info["REMAP"] = remap
             if self.anno_hits and hits:
-                entry.info["REMAPHits"] = [_[1] for _ in hits[-self.anno_hits:]]
+                entry.info["REMAPHits"] = [_[1]
+                                           for _ in hits[-self.anno_hits:]]
         return entry
 
     def annotate_vcf(self):
         """
         Annotates the vcf and writes to new vcf
         """
         with pysam.VariantFile(self.in_vcf) as fh:
```

### Comparing `Truvari-4.0.0/truvari/annotations/repmask.py` & `Truvari-4.1.0/truvari/annotations/repmask.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         self.n_header = header
 
     def extract_seqs(self):
         """
         Create the fasta file of all the sequences
         Returns the fasta file name
         """
-        ret = tempfile.NamedTemporaryFile(mode='w', delete=False) # pylint: disable=consider-using-with
+        ret = tempfile.NamedTemporaryFile(mode='w', delete=False)  # pylint: disable=consider-using-with
         tot_cnt = 0
         cnt = 0
         cntbp = 0
         with pysam.VariantFile(self.in_vcf) as fh:
             for pos, entry in enumerate(fh):
                 tot_cnt += 1
                 entry_size = truvari.entry_size(entry)
```

### Comparing `Truvari-4.0.0/truvari/annotations/svinfo.py` & `Truvari-4.1.0/truvari/annotations/svinfo.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,27 +30,29 @@
     """
     header.add_line(
         '##INFO=<ID=SVTYPE,Number=1,Type=String,Description="SVTYPE">')
     header.add_line(
         '##INFO=<ID=SVLEN,Number=1,Type=Integer,Description="SVLEN">')
     return header
 
+
 def add_svinfo(entry, min_size=0, n_header=None):
     """
     Add svinfo
     """
     sz = truvari.entry_size(entry)
     if sz < min_size:
         return
     if n_header:
         entry.translate(n_header)
     svtype = truvari.entry_variant_type(entry)
     entry.info["SVTYPE"] = svtype.name
     entry.info["SVLEN"] = sz
 
+
 def svinfo_main(cmdargs):
     """
     Main method
     """
     args = parse_args(cmdargs)
     vcf = pysam.VariantFile(args.input)
     n_header = edit_header(vcf.header.copy())
```

### Comparing `Truvari-4.0.0/truvari/annotations/trf.py` & `Truvari-4.1.0/truvari/annotations/trf.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,35 +3,33 @@
 variants with the best fitting repeat motif and its copy number
 relative to the reference
 """
 import os
 import sys
 import json
 import math
-import types
 import shutil
 import logging
 import argparse
+import functools
 import multiprocessing
 from io import StringIO
-from functools import cmp_to_key
 
 import pysam
 import tabix
 import truvari
 
-trfshared = types.SimpleNamespace()
-
 try:
     from setproctitle import setproctitle  # pylint: disable=import-error,useless-suppression
 except ModuleNotFoundError:
     def setproctitle(_):
         """ dummy function """
         return
 
+
 def compare_scores(a, b):
     """
     sort annotations
     """
     # most amount of SV covered
     ret = 0
     if a["ovl_pct"] > b["ovl_pct"]:
@@ -46,41 +44,45 @@
         aspan = a["end"] - a["start"]
         bspan = b["end"] - b["start"]
         if aspan > bspan:
             ret = 1
         elif aspan < bspan:
             ret = -1
     return ret
-score_sorter = cmp_to_key(compare_scores)
+
+
+score_sorter = functools.cmp_to_key(compare_scores)
+
 
 class TRFAnno():
     """
     Class for trf annotation
     Operates on a single TRF region across multiple TRF annotations
     """
 
     def __init__(self, region, reference, motif_similarity=0.90, buf=5):
         """ setup """
         self.region = region
         self.reference = reference
         self.motif_similarity = motif_similarity
-        self.known_motifs = {_["repeat"]:_["copies"] for _ in self.region["annos"]}
+        self.known_motifs = {_["repeat"]: _["copies"]
+                             for _ in self.region["annos"]}
         self.buffer = buf
 
     def make_seq(self, entry, svtype):
         """
         Make the haplotype sequence
         use r_start/r_end to make sequence a subsequence
         """
         # variant position relative to this region
         v_start = entry.start - self.region["start"]
         v_end = entry.stop - self.region["start"]
 
-        #if substr is None:
-            #substr = (0, len(self.reference))
+        # if substr is None:
+        # substr = (0, len(self.reference))
         up_seq = self.reference[:v_start]
         dn_seq = self.reference[v_end:]
         if svtype == "INS":
             m_seq = up_seq + entry.alts[0] + dn_seq
         elif svtype == "DEL":
             m_seq = up_seq + dn_seq
         else:
@@ -89,30 +91,32 @@
         return m_seq
 
     def score_annotation(self, var_start, var_end, anno):
         """
         Scores the annotation. Addes fields in place.
         if is_new, we calculate the diff
         """
-        ovl_pct = truvari.overlap_percent(var_start, var_end, anno["start"] - self.buffer, anno["end"] + self.buffer)
+        ovl_pct = truvari.overlap_percent(
+            var_start, var_end, anno["start"] - self.buffer, anno["end"] + self.buffer)
         # has to have overlap
         if ovl_pct == 0:
             return None
         anno["ovl_pct"] = ovl_pct
 
         if anno["repeat"] in self.known_motifs:
             anno["diff"] = anno["copies"] - self.known_motifs[anno["repeat"]]
         else:
             best_score = 0
             best_pos = None
             motif_len = len(anno["repeat"])
             for known in self.region["annos"]:
                 if truvari.sizesim(len(known["repeat"]), motif_len)[0] < self.motif_similarity:
                     continue
-                sq = truvari.unroll_compare(known["repeat"], anno["repeat"], anno["start"] - known["start"])
+                sq = truvari.unroll_compare(
+                    known["repeat"], anno["repeat"], anno["start"] - known["start"])
                 if sq >= self.motif_similarity and sq > best_score:
                     best_score = sq
                     best_pos = known
 
             if best_pos:
                 anno["diff"] = anno["copies"] - best_pos["copies"]
                 anno["orig_repeat"] = anno["repeat"]
@@ -125,16 +129,16 @@
     def del_annotate(self, entry, svlen, score_filter=True):
         """
         Annotate a deletion
         """
         scores = []
         for anno in self.region["annos"]:
             # + 1 for anchor base
-            ovl_pct = truvari.overlap_percent(entry.start + 1, entry.stop, \
-                                anno["start"] - self.buffer, anno["end"] + self.buffer)
+            ovl_pct = truvari.overlap_percent(entry.start + 1, entry.stop,
+                                              anno["start"] - self.buffer, anno["end"] + self.buffer)
             if ovl_pct == 0:
                 continue
             m_sc = dict(anno)
             m_sc["ovl_pct"] = ovl_pct
             copy_diff = round(-(ovl_pct * svlen) / anno["period"], 1)
             if copy_diff % 1 == 0:
                 copy_diff = int(copy_diff)
@@ -204,26 +208,27 @@
         4) feaux_seq = motif length * estimated copy_diff in alt seq
         Align rolled alt seq and feaux seq, if similarity is high enough, just take that annotation
         If the similarity isn't high enough, then we send it to TRF
         """
         scores = []
         best_score = {}
         for anno in self.region["annos"]:
-            ovl_pct = truvari.overlap_percent(entry.start + 1, entry.stop, \
-                            anno["start"] - self.buffer, anno["end"] + self.buffer)
+            ovl_pct = truvari.overlap_percent(entry.start + 1, entry.stop,
+                                              anno["start"] - self.buffer, anno["end"] + self.buffer)
             if ovl_pct == 0:
                 continue
 
             copy_diff = len(entry.alts[0][1:]) / anno["period"]
             faux_seq = anno["repeat"] * math.floor(copy_diff)
             # add partial motif extension
             partial = int(copy_diff % 1 * anno["period"])
             if partial:
                 faux_seq += anno["repeat"][:partial]
-            sim = truvari.unroll_compare(faux_seq, entry.alts[0][1:], entry.start - anno["start"])
+            sim = truvari.unroll_compare(
+                faux_seq, entry.alts[0][1:], entry.start - anno["start"])
 
             if sim < self.motif_similarity:
                 continue
 
             m_sc = dict(anno)
             copy_diff = round(copy_diff, 1)
             if copy_diff % 1 == 0:
@@ -236,50 +241,52 @@
                 best_score = m_sc
             scores.append(m_sc)
 
         if score_filter and scores:
             return best_score
         return scores
 
+
 def parse_trf_output(fn):
     """
     Parse the outputs from TRF
     Returns a list of hits
     """
     # The columns I don't want are set to type None
     trf_cols = [("start", int),
                 ("end", int),
                 ("period", int),
                 ("copies", float),
                 ("consize", int),
-                ("pctmat", None), # int
-                ("pctindel", None), # int
+                ("pctmat", None),  # int
+                ("pctindel", None),  # int
                 ("score", int),
-                ("A", None), # int
-                ("C", None), # int
-                ("G", None), # int
-                ("T",  None), # int
+                ("A", None),  # int
+                ("C", None),  # int
+                ("G", None),  # int
+                ("T",  None),  # int
                 ("entropy", float),
                 ("repeat", str),
-                ("unk1", None), # str
-                ("unk2", None), # str
-                ("unk3", None) # str
-            ]
+                ("unk1", None),  # str
+                ("unk2", None),  # str
+                ("unk3", None)  # str
+                ]
 
     ret = {}
     with open(fn, 'r') as fh:
         var_key = None
         for line in fh:
             line = line.strip()
             if line.startswith("@"):
                 var_key = line[1:]
                 ret[var_key] = []
                 continue
 
-            data = {x[0]: x[1](y) for x, y in zip(trf_cols, line.split(' ')) if x[1]}
+            data = {x[0]: x[1](y) for x, y in zip(
+                trf_cols, line.split(' ')) if x[1]}
             # correction to 0-based
             data["start"] -= 1
             ret[var_key].append(data)
 
     return ret
 
 
@@ -307,21 +314,23 @@
         logging.error("Couldn't run trf. Check Parameters")
         logging.error(cmd)
         logging.error(str(ret))
         return {}
 
     return parse_trf_output(tr_fn)
 
+
 class AnnoStack():
     """
     Treat a list like a stack
     Creates a TRFAnno for the top
     We can pop from the stack based on vcf entry coordinates
     which will update self.tanno
     """
+
     def __init__(self, annos, ref, motif_sim):
         self.annos = annos
         self.ref = ref
         self.motif_sim = motif_sim
         self.tanno = None
         self.build_from_top()
 
@@ -336,105 +345,111 @@
         """
         Create the TRFAnno from the top of the stack
         """
         if not self.annos:
             self.tanno = None
             return
         cur_anno = self.annos.pop(0)
-        ref_seq = self.ref.fetch(cur_anno["chrom"], cur_anno["start"], cur_anno["end"])
+        ref_seq = self.ref.fetch(
+            cur_anno["chrom"], cur_anno["start"], cur_anno["end"])
         self.tanno = TRFAnno(cur_anno, ref_seq, self.motif_sim)
 
 
-def process_ref_region(region):
+def process_ref_region(region, args):
     """
     Process a section of the reference.
     Tries to run TRF only once
     """
     region = {"chrom": region[0],
               "start": region[1],
               "end": region[2]}
-    logging.debug(f"Starting region {region['chrom']}:{region['start']}-{region['end']}")
+    logging.debug(
+        f"Starting region {region['chrom']}:{region['start']}-{region['end']}")
     setproctitle(f"trf {region['chrom']}:{region['start']}-{region['end']}")
 
-    vcf = pysam.VariantFile(trfshared.args.input)
+    vcf = pysam.VariantFile(args.input)
     new_header = edit_header(vcf.header)
     out = StringIO()
 
     try:
         m_fetch = vcf.fetch(region["chrom"], region["start"], region["end"])
     except ValueError as e:
         logging.debug("Skipping VCF fetch %s", e)
         return None
 
-
-    m_stack = AnnoStack(list(iter_tr_regions(trfshared.args.repeats,
+    m_stack = AnnoStack(list(iter_tr_regions(args.repeats,
                              (region["chrom"], region["start"], region["end"]))),
-                        pysam.FastaFile(trfshared.args.reference),
-                        trfshared.args.motif_similarity)
+                        pysam.FastaFile(args.reference),
+                        args.motif_similarity)
 
     batch = []
     fa_fn = truvari.make_temp_filename(suffix=".fa")
     with open(fa_fn, 'w') as fa_out:
         for entry in m_fetch:
             # Variants must start within region
             if not (entry.start >= region["start"] and entry.start < region["end"]):
                 continue
 
             m_stack.pop(entry)
             # If we're out of annotations, ou not inside an annotation
             if m_stack.tanno is None or \
-            not (entry.start >= m_stack.tanno.region["start"] \
-                 and entry.stop < m_stack.tanno.region["end"]):
+                not (entry.start >= m_stack.tanno.region["start"]
+                     and entry.stop < m_stack.tanno.region["end"]):
                 out.write(str(entry))
                 continue
 
             svtype = truvari.entry_variant_type(entry)
             svlen = truvari.entry_size(entry)
-            if svlen < trfshared.args.min_length or svtype not in [truvari.SV.DEL, truvari.SV.INS]:
+            if svlen < args.min_length or svtype not in [truvari.SV.DEL, truvari.SV.INS]:
                 out.write(str(edit_entry(entry, None, new_header)))
                 continue
 
             if svtype == truvari.SV.DEL:
                 m_anno = m_stack.tanno.del_annotate(entry, svlen)
                 out.write(str(edit_entry(entry, m_anno, new_header)))
             elif svtype == truvari.SV.INS:
-                m_anno = m_stack.tanno.ins_estimate_anno(entry) if not trfshared.args.no_estimate else None
+                m_anno = m_stack.tanno.ins_estimate_anno(
+                    entry) if not args.no_estimate else None
                 if m_anno:
                     out.write(str(edit_entry(entry, m_anno, new_header)))
                 else:
                     batch.append((entry, m_stack.tanno))
-                    fa_out.write(f">{len(batch) - 1}\n{m_stack.tanno.make_seq(entry, 'INS')}\n")
+                    fa_out.write(
+                        f">{len(batch) - 1}\n{m_stack.tanno.make_seq(entry, 'INS')}\n")
 
     if batch:
-        annotations = run_trf(fa_fn, trfshared.args.executable, trfshared.args.trf_params)
+        annotations = run_trf(fa_fn, args.executable, args.trf_params)
         for key, (entry, tanno) in enumerate(batch):
             key = str(key)
             m_anno = None
             if key in annotations:
                 # translate coords back
                 tanno.translate_coords(annotations[key])
                 m_anno = tanno.ins_annotate(entry, annotations[key])
             out.write(str(edit_entry(entry, m_anno, new_header)))
 
     out.seek(0)
     setproctitle(f"trf {region['chrom']}:{region['start']}-{region['end']}")
-    logging.debug(f"Done region {region['chrom']}:{region['start']}-{region['end']}")
+    logging.debug(
+        f"Done region {region['chrom']}:{region['start']}-{region['end']}")
     return out.read()
 
-def process_tr_region(region):
+
+def process_tr_region(region, args):
     """
     Process vcf lines from a tr reference section
     """
-    logging.debug(f"Starting region {region['chrom']}:{region['start']}-{region['end']}")
+    logging.debug(
+        f"Starting region {region['chrom']}:{region['start']}-{region['end']}")
     setproctitle(f"trf {region['chrom']}:{region['start']}-{region['end']}")
 
-    ref = pysam.FastaFile(trfshared.args.reference)
+    ref = pysam.FastaFile(args.reference)
     ref_seq = ref.fetch(region["chrom"], region["start"], region["end"])
-    tanno = TRFAnno(region, ref_seq, trfshared.args.motif_similarity, trfshared.args.buffer)
-    vcf = pysam.VariantFile(trfshared.args.input)
+    tanno = TRFAnno(region, ref_seq, args.motif_similarity, args.buffer)
+    vcf = pysam.VariantFile(args.input)
     new_header = edit_header(vcf.header)
     out = StringIO()
 
     fa_fn = truvari.make_temp_filename(suffix=".fa")
     batch = []
     try:
         m_fetch = vcf.fetch(region["chrom"], region["start"], region["end"])
@@ -444,46 +459,49 @@
     with open(fa_fn, 'w') as fa_out:
         for entry in m_fetch:
             # Variants must be entirely contained within region
             if not (entry.start >= region["start"] and entry.stop < region["end"]):
                 continue
             svtype = truvari.entry_variant_type(entry)
             svlen = truvari.entry_size(entry)
-            if svlen < trfshared.args.min_length or svtype not in [truvari.SV.DEL, truvari.SV.INS]:
+            if svlen < args.min_length or svtype not in [truvari.SV.DEL, truvari.SV.INS]:
                 out.write(str(edit_entry(entry, None, new_header)))
                 continue
 
             if svtype == truvari.SV.DEL:
                 m_anno = tanno.del_annotate(entry, svlen)
                 out.write(str(edit_entry(entry, m_anno, new_header)))
             elif svtype == truvari.SV.INS:
-                m_anno = tanno.ins_estimate_anno(entry) if not trfshared.args.no_estimate else None
+                m_anno = tanno.ins_estimate_anno(
+                    entry) if not args.no_estimate else None
                 if m_anno:
                     out.write(str(edit_entry(entry, m_anno, new_header)))
                 else:
                     batch.append(entry)
                     seq = tanno.make_seq(entry, "INS")
                     fa_out.write(f">{len(batch) - 1}\n{seq}\n")
 
     if batch:
-        annotations = run_trf(fa_fn, trfshared.args.executable, trfshared.args.trf_params)
+        annotations = run_trf(fa_fn, args.executable, args.trf_params)
         for key, entry in enumerate(batch):
             key = str(key)
             m_anno = None
             if key in annotations:
                 # translate coords back
                 tanno.translate_coords(annotations[key])
                 m_anno = tanno.ins_annotate(entry, annotations[key])
             out.write(str(edit_entry(entry, m_anno, new_header)))
 
     out.seek(0)
     setproctitle(f"trf {region['chrom']}:{region['start']}-{region['end']}")
-    logging.debug(f"Done region {region['chrom']}:{region['start']}-{region['end']}")
+    logging.debug(
+        f"Done region {region['chrom']}:{region['start']}-{region['end']}")
     return out.read()
 
+
 def iter_tr_regions(fn, region=None):
     """
     Read a repeats file with structure chrom, start, end, annotations.json
     returns generator of dicts
     """
     data = None
     if region is None:
@@ -505,14 +523,15 @@
         end = int(end)
         annos = json.loads(annos)
         yield {"chrom": chrom,
                "start": start,
                "end": end,
                "annos": annos}
 
+
 def edit_header(header):
     """
     New VCF INFO fields
     """
     header = header.copy()
     header.add_line(('##INFO=<ID=TRF,Number=0,Type=Flag,'
                      'Description="Entry hits a tandem repeat region">'))
@@ -534,14 +553,15 @@
                      'Description="Alignment score">'))
     header.add_line(('##INFO=<ID=TRFentropy,Number=1,Type=Float,'
                      'Description="Entropy measure">'))
     header.add_line(('##INFO=<ID=TRFsim,Number=1,Type=Float,'
                      'Description="Similarity of ALT sequence to generated motif faux sequence">'))
     return header
 
+
 def edit_entry(entry, repeat, new_header):
     """
     places the INFO fields into the entry
     assumes entry has been translated to a vcf header holding the correct fields
     Returns the entry but also annotates in-place
     """
     entry.translate(new_header)
@@ -557,14 +577,15 @@
         entry.info["TRFscore"] = repeat["score"]
         entry.info["TRFentropy"] = repeat["entropy"]
         if "similarity" in repeat:
             entry.info["TRFsim"] = round(repeat["similarity"], 3)
 
     return entry
 
+
 def parse_args(args):
     """
     Pull the command line parameters
     """
     parser = argparse.ArgumentParser(prog="trf", description=__doc__,
                                      formatter_class=argparse.RawDescriptionHelpFormatter)
     parser.add_argument("-i", "--input", type=str, required=True,
@@ -586,24 +607,25 @@
     parser.add_argument("-m", "--min-length", type=truvari.restricted_int, default=50,
                         help="Minimum size of entry to annotate (%(default)s)")
     parser.add_argument("-R", "--regions-only", action="store_true",
                         help="Only write variants within --repeats regions (%(default)s)")
     parser.add_argument("--no-estimate", action="store_true",
                         help="Skip INS estimation procedure and run everything through TRF. (%(default)s)")
     parser.add_argument("-C", "--chunk-size", type=int, default=5,
-                            help="Size (in mbs) of reference chunks for parallelization (%(default)s)")
+                        help="Size (in mbs) of reference chunks for parallelization (%(default)s)")
     parser.add_argument("-t", "--threads", type=truvari.restricted_int, default=1,
                         help="Number of threads to use (%(default)s)")
     parser.add_argument("--debug", action="store_true",
                         help="Verbose logging")
 
     args = parser.parse_args(args)
     truvari.setup_logging(args.debug, show_version=True)
     return args
 
+
 def check_params(args):
     """
     Ensure the files are compressed/indexed
     """
     check_fail = False
     if not os.path.exists(args.input):
         logging.error(f"{args.input} doesn't exit")
@@ -626,32 +648,32 @@
     if not shutil.which(args.executable):
         logging.error(f"{args.executable} not found in path")
         check_fail = True
     if check_fail:
         logging.error("Please fix parameters")
         sys.exit(1)
 
+
 def trf_main(cmdargs):
     """ TRF annotation """
     args = parse_args(cmdargs)
     check_params(args)
-    trfshared.args = args
 
     m_regions = None
     m_process = None
     if args.regions_only:
         m_regions = iter_tr_regions(args.repeats)
-        m_process = process_tr_region
+        m_process = functools.partial(process_tr_region, args=args)
     else:
         # refactor. need streaming mode
-        m_regions = truvari.ref_ranges(args.reference, chunk_size=int(args.chunk_size * 1e6))
-        m_process = process_ref_region
-
+        m_regions = truvari.ref_ranges(
+            args.reference, chunk_size=int(args.chunk_size * 1e6))
+        m_process = functools.partial(process_ref_region, args=args)
 
-    vcf = pysam.VariantFile(trfshared.args.input)
+    vcf = pysam.VariantFile(args.input)
     new_header = edit_header(vcf.header)
 
     with multiprocessing.Pool(args.threads, maxtasksperchild=1) as pool:
         chunks = pool.imap_unordered(m_process, m_regions)
         pool.close()
         with open(args.output, 'w') as fout:
             fout.write(str(new_header))
```

### Comparing `Truvari-4.0.0/truvari/bench.py` & `Truvari-4.1.0/truvari/bench.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 import numpy as np
 
 import truvari
 
 ##############
 # Parameters #
 ##############
+
+
 def parse_args(args):
     """
     Pull the command line parameters
     """
     defaults = truvari.Matcher.make_match_params()
     parser = argparse.ArgumentParser(prog="bench", description=__doc__,
                                      formatter_class=argparse.RawDescriptionHelpFormatter)
@@ -54,15 +56,14 @@
     thresg.add_argument("--dup-to-ins", action="store_true",
                         help="Assume DUP svtypes are INS (%(default)s)")
     thresg.add_argument("-C", "--chunksize", type=truvari.restricted_int, default=defaults.chunksize,
                         help="Max reference distance to compare calls (%(default)s)")
     thresg.add_argument("-B", "--minhaplen", type=truvari.restricted_int, default=defaults.minhaplen,
                         help="Min haplotype sequence length to create (%(default)s)")
 
-
     genoty = parser.add_argument_group("Genotype Comparison Arguments")
     genoty.add_argument("--bSample", type=str, default=None,
                         help="Baseline calls' sample to use (first)")
     genoty.add_argument("--cSample", type=str, default=None,
                         help="Comparison calls' sample to use (first)")
 
     filteg = parser.add_argument_group("Filtering Arguments")
@@ -90,16 +91,18 @@
             args.sizefilt = args.sizemin
         else:
             args.sizefilt = defaults.sizefilt
 
     # Setup abspaths
     args.base = os.path.abspath(args.base)
     args.comp = os.path.abspath(args.comp)
-    args.includebed = os.path.abspath(args.includebed) if args.includebed else args.includebed
-    args.reference = os.path.abspath(args.reference) if args.reference else args.reference
+    args.includebed = os.path.abspath(
+        args.includebed) if args.includebed else args.includebed
+    args.reference = os.path.abspath(
+        args.reference) if args.reference else args.reference
 
     return args
 
 
 def check_params(args):
     """
     Checks parameters as much as possible.
@@ -118,28 +121,28 @@
     if not os.path.exists(args.comp):
         logging.error("File %s does not exist", args.comp)
         check_fail = True
     if not os.path.exists(args.base):
         logging.error("File %s does not exist", args.base)
         check_fail = True
     if not args.comp.endswith(".gz"):
-        logging.error(
-            "Comparison vcf %s does not end with .gz. Must be bgzip'd", args.comp)
+        logging.error("Comparison vcf %s does not end with .gz. Must be bgzip'd",
+                      args.comp)
         check_fail = True
     if not os.path.exists(args.comp + '.tbi'):
-        logging.error(
-            "Comparison vcf index %s.tbi does not exist. Must be indexed", args.comp)
+        logging.error("Comparison vcf index %s.tbi does not exist. Must be indexed",
+                      args.comp)
         check_fail = True
     if not args.base.endswith(".gz"):
-        logging.error(
-            "Base vcf %s does not end with .gz. Must be bgzip'd", args.base)
+        logging.error("Base vcf %s does not end with .gz. Must be bgzip'd",
+                      args.base)
         check_fail = True
     if not os.path.exists(args.base + '.tbi'):
-        logging.error(
-            "Base vcf index %s.tbi does not exist. Must be indexed", args.base)
+        logging.error("Base vcf index %s.tbi does not exist. Must be indexed",
+                      args.base)
         check_fail = True
     if args.includebed and not os.path.exists(args.includebed):
         logging.error("Include bed %s does not exist", args.includebed)
         check_fail = True
     if args.reference and not os.path.exists(args.reference):
         logging.error("Reference %s does not exist", args.reference)
         check_fail = True
@@ -206,29 +209,73 @@
 
 
 def annotate_entry(entry, match, header):
     """
     Make a new entry with all the information
     """
     entry.translate(header)
-    entry.info["PctSeqSimilarity"] = round(match.seqsim, 4) if match.seqsim is not None else None
-    entry.info["PctSizeSimilarity"] = round(match.sizesim, 4) if match.sizesim is not None else None
-    entry.info["PctRecOverlap"] = round(match.ovlpct, 4) if match.ovlpct is not None else None
+    entry.info["PctSeqSimilarity"] = round(
+        match.seqsim, 4) if match.seqsim is not None else None
+    entry.info["PctSizeSimilarity"] = round(
+        match.sizesim, 4) if match.sizesim is not None else None
+    entry.info["PctRecOverlap"] = round(
+        match.ovlpct, 4) if match.ovlpct is not None else None
     entry.info["SizeDiff"] = match.sizediff
     entry.info["StartDistance"] = match.st_dist
     entry.info["EndDistance"] = match.ed_dist
     entry.info["GTMatch"] = match.gt_match
     entry.info["TruScore"] = int(match.score) if match.score else None
     entry.info["MatchId"] = match.matid
     entry.info["Multi"] = match.multi
 
 
 #############
 # Core code #
 #############
+class WeightedStatsBox(OrderedDict):
+    """
+    Make a blank stats box for counting variant pairs as TP/FP/FN, but weighted by match similarity
+    """
+
+    def __init__(self):
+        super().__init__()
+        self["TP"] = 0
+        self["FP"] = 0
+        self["FN"] = 0
+        self["precision"] = 0
+        self["recall"] = 0
+        self["f1"] = 0
+        self["total"] = 0
+
+    def add(self, score, which):
+        """
+        The score is how much credit to give to TP.
+        If score is None, set it to 0
+        To avoid double counting, specify has_comp=True, which means a separate call to `.add` will be made
+        The score is always added to
+        is_base will figure out if 1-score
+        should be applied to both FN/FP (true) or FP only
+        """
+        if score is None:
+            score = 0
+        self['total'] += 1
+        self["TP"] += score
+        if which != 2:
+            self["FN"] += 1 - score
+        if which != 1:
+            self["FP"] += 1 - score
+
+    def calc_performance(self):
+        """
+        Calculate metrics
+        """
+        self["precision"], self["recall"], self["f1"] = truvari.performance_metrics(
+            self["TP"], self["TP"], self["FN"], self["FP"])
+
+
 class StatsBox(OrderedDict):
     """
     Make a blank stats box for counting TP/FP/FN and calculating performance
     """
 
     def __init__(self):
         super().__init__()
@@ -253,23 +300,39 @@
         Calculate the precision/recall
         """
         if self["TP-base"] == 0 and self["FN"] == 0:
             logging.warning("No TP or FN calls in base!")
         elif self["TP-comp"] == 0 and self["FP"] == 0:
             logging.warning("No TP or FP calls in comp!")
 
-        precision, recall, f1 = truvari.performance_metrics(self["TP-base"], self["TP-comp"], self["FN"], self["FP"])
+        precision, recall, f1 = truvari.performance_metrics(
+            self["TP-base"], self["TP-comp"], self["FN"], self["FP"])
 
         self["precision"] = precision
         self["recall"] = recall
         self["f1"] = f1
         if self["TP-comp_TP-gt"] + self["TP-comp_FP-gt"] != 0:
             self["gt_concordance"] = float(self["TP-comp_TP-gt"]) / (self["TP-comp_TP-gt"] +
                                                                      self["TP-comp_FP-gt"])
 
+    def clean_out(self):
+        """
+        When reusing a StatsBox (typically inside refine), gt/weight numbers
+        are typically invalidated. This removes those numbers from self to make
+        a cleaner report
+        """
+        del self["TP-comp_TP-gt"]
+        del self["TP-comp_FP-gt"]
+        del self["TP-base_TP-gt"]
+        del self["TP-base_FP-gt"]
+        del self["gt_concordance"]
+        del self["gt_matrix"]
+        if "weighted" in self:
+            del self["weighted"]
+
     def write_json(self, out_name):
         """
         Write stats as json to file
         """
         with open(out_name, 'w') as fout:
             fout.write(json.dumps(self, indent=4))
 
@@ -278,14 +341,15 @@
     """
     Makes all of the output files for a Bench.run
 
     The variable `BenchOutput.vcf_filenames` holds a dictonary. The keys are tpb, tpc
     for true positive base/comp vcf filename and fn, fp. The variable `stats_box` holds
     a :class:`StatsBox`.
     """
+
     def __init__(self, bench, matcher):
         """
         initialize
         """
         self.m_bench = bench
         self.m_matcher = matcher
 
@@ -299,36 +363,41 @@
             logging.info("Params:\n%s", json.dumps(param_dict, indent=4))
 
         with open(os.path.join(self.m_bench.outdir, 'params.json'), 'w') as fout:
             json.dump(param_dict, fout)
 
         b_vcf = pysam.VariantFile(self.m_bench.base_vcf)
         c_vcf = pysam.VariantFile(self.m_bench.comp_vcf)
-        self.n_headers = {'b':edit_header(b_vcf),
-                          'c':edit_header(c_vcf)}
+        self.n_headers = {'b': edit_header(b_vcf),
+                          'c': edit_header(c_vcf)}
 
         self.vcf_filenames = {'tpb': os.path.join(self.m_bench.outdir, "tp-base.vcf"),
                               'tpc': os.path.join(self.m_bench.outdir, "tp-comp.vcf"),
                               'fn': os.path.join(self.m_bench.outdir, "fn.vcf"),
                               'fp': os.path.join(self.m_bench.outdir, "fp.vcf")}
         self.out_vcfs = {}
         for key in ['tpb', 'fn']:
-            self.out_vcfs[key] = pysam.VariantFile(self.vcf_filenames[key], mode='w', header=self.n_headers['b'])
+            self.out_vcfs[key] = pysam.VariantFile(
+                self.vcf_filenames[key], mode='w', header=self.n_headers['b'])
         for key in ['tpc', 'fp']:
-            self.out_vcfs[key] = pysam.VariantFile(self.vcf_filenames[key], mode='w', header=self.n_headers['c'])
+            self.out_vcfs[key] = pysam.VariantFile(
+                self.vcf_filenames[key], mode='w', header=self.n_headers['c'])
 
         self.stats_box = StatsBox()
+        self.wt_seq_stats_box = WeightedStatsBox()
+        self.wt_size_stats_box = WeightedStatsBox()
 
     def write_match(self, match):
         """
         Annotate a MatchResults' entries then write to the apppropriate file
         and do the stats counting.
         Writer is responsible for handling FPs between sizefilt-sizemin
         """
         box = self.stats_box
+        skip = False
         if match.base:
             box["base cnt"] += 1
             annotate_entry(match.base, match, self.n_headers['b'])
             if match.state:
                 gtBase = str(match.base_gt)
                 gtComp = str(match.comp_gt)
                 box["gt_matrix"][gtBase][gtComp] += 1
@@ -354,27 +423,48 @@
                 else:
                     box["TP-comp_FP-gt"] += 1
             elif truvari.entry_size(match.comp) >= self.m_matcher.params.sizemin:
                 # The if is because we don't count FPs between sizefilt-sizemin
                 box["comp cnt"] += 1
                 box["FP"] += 1
                 self.out_vcfs["fp"].write(match.comp)
+            else:
+                skip = True
+
+        if skip:  # don't count partial credit to sizefilt-sizemin FPs
+            return
+
+        # This is convoluted
+        if match.base and match.comp:
+            self.wt_seq_stats_box.add(match.base.info["PctSeqSimilarity"], 0)
+            self.wt_size_stats_box.add(match.base.info["PctSizeSimilarity"], 0)
+        elif match.base and not match.comp:
+            self.wt_seq_stats_box.add(match.base.info["PctSeqSimilarity"], 1)
+            self.wt_size_stats_box.add(match.base.info["PctSizeSimilarity"], 1)
+        elif not match.base and match.comp:
+            self.wt_seq_stats_box.add(match.comp.info["PctSeqSimilarity"], 2)
+            self.wt_size_stats_box.add(match.comp.info["PctSizeSimilarity"], 2)
 
     def close_outputs(self):
         """
         Close all the files
         """
         for i in self.out_vcfs.values():
             i.close()
 
         for i in self.vcf_filenames.values():
             truvari.compress_index_vcf(i)
 
         self.stats_box.calc_performance()
-        self.stats_box.write_json(os.path.join(self.m_bench.outdir, "summary.json"))
+        self.wt_seq_stats_box.calc_performance()
+        self.wt_size_stats_box.calc_performance()
+        self.stats_box["weighted"] = {'sequence': dict(self.wt_seq_stats_box),
+                                      'size': dict(self.wt_size_stats_box)}
+        self.stats_box.write_json(os.path.join(
+            self.m_bench.outdir, "summary.json"))
 
 
 class Bench():
     """
     Object to perform operations of truvari bench
 
     You can build a Bench worker with default matching parameters via:
@@ -411,27 +501,29 @@
 
         m_bench = truvari.Bench(matcher, base_vcf, comp_vcf, outdir)
         output = m_bench.run()
 
     Note that running on files must write to an output directory and is the only way to use things like 'includebed'.
     However, the returned `BenchOutput` has attributes pointing to all the results.
     """
+
     def __init__(self, matcher=None, base_vcf=None, comp_vcf=None, outdir=None,
-                 includebed=None, extend=0, debug=False , do_logging=False):
+                 includebed=None, extend=0, debug=False, do_logging=False):
         """
         Initilize
         """
         self.matcher = matcher if matcher is not None else truvari.Matcher()
         self.base_vcf = base_vcf
         self.comp_vcf = comp_vcf
         self.outdir = outdir
         self.includebed = includebed
         self.extend = extend
         self.debug = debug
         self.do_logging = do_logging
+        self.refine_candidates = []
 
     def param_dict(self):
         """
         Returns the parameters as a dict
         """
         return {'base': self.base_vcf,
                 "comp": self.comp_vcf,
@@ -441,48 +533,57 @@
                 "debug": self.debug}
 
     def run(self):
         """
         Runs bench and returns the resulting :class:`truvari.BenchOutput`
         """
         if self.base_vcf is None or self.comp_vcf is None or self.outdir is None:
-            raise RuntimeError("Cannot call Bench.run without base/comp vcf filenames and outdir")
+            raise RuntimeError(
+                "Cannot call Bench.run without base/comp vcf filenames and outdir")
 
         output = BenchOutput(self, self.matcher)
 
         base = pysam.VariantFile(self.base_vcf)
         comp = pysam.VariantFile(self.comp_vcf)
 
         regions = truvari.RegionVCFIterator(base, comp,
                                             self.includebed,
                                             self.matcher.params.sizemax)
         regions.merge_overlaps()
-        regions_extended = regions.extend(self.extend) if self.extend else regions
+        regions_extended = regions.extend(
+            self.extend) if self.extend else regions
 
         base_i = regions.iterate(base)
         comp_i = regions_extended.iterate(comp)
 
-        chunks = truvari.chunker(self.matcher, ('base', base_i), ('comp', comp_i))
+        chunks = truvari.chunker(
+            self.matcher, ('base', base_i), ('comp', comp_i))
         for match in itertools.chain.from_iterable(map(self.compare_chunk, chunks)):
             # setting non-matched comp variants that are not fully contained in the original regions to None
             # These don't count as FP or TP and don't appear in the output vcf files
             if self.extend and match.comp is not None and not match.state and not regions.include(match.comp):
                 match.comp = None
             output.write_match(match)
 
+        with open(os.path.join(self.outdir, 'candidate.refine.bed'), 'w') as fout:
+            fout.write("\n".join(self.refine_candidates))
+
         output.close_outputs()
         return output
 
     def compare_chunk(self, chunk):
         """
         Given a filtered chunk, (from chunker) compare all of the calls
         """
-        _, chunk_dict, chunk_id = chunk
+        chunk_dict, chunk_id = chunk
         logging.debug("Comparing chunk %s", chunk_id)
-        return self.compare_calls(chunk_dict["base"], chunk_dict["comp"], chunk_id)
+        result = self.compare_calls(
+            chunk_dict["base"], chunk_dict["comp"], chunk_id)
+        self.check_refine_candidate(result)
+        return result
 
     def compare_calls(self, base_variants, comp_variants, chunk_id=0):
         """
         Builds MatchResults, returns them as a numpy matrix if there's at least one base and one comp variant.
         Otherwise, returns a list of the variants placed in MatchResults
         """
         # All FPs
@@ -503,36 +604,57 @@
                 ret = truvari.MatchResult()
                 ret.base = b
                 ret.matid = f"{chunk_id}.{bid}._"
                 logging.debug("All FN -> %s", ret)
                 fns.append(ret)
             return fns
 
-        match_matrix = self.build_matrix(base_variants, comp_variants, chunk_id)
+        match_matrix = self.build_matrix(
+            base_variants, comp_variants, chunk_id)
         if isinstance(match_matrix, list):
             return match_matrix
         return PICKERS[self.matcher.params.pick](match_matrix)
 
     def build_matrix(self, base_variants, comp_variants, chunk_id=0, skip_gt=False):
         """
         Builds MatchResults, returns them as a numpy matrix
         """
         if not base_variants or not comp_variants:
-            raise RuntimeError("Expected at least one base and one comp variant")
+            raise RuntimeError(
+                "Expected at least one base and one comp variant")
         match_matrix = []
         for bid, b in enumerate(base_variants):
             base_matches = []
             for cid, c in enumerate(comp_variants):
-                mat = self.matcher.build_match(b, c, f"{chunk_id}.{bid}.{cid}", skip_gt)
+                mat = self.matcher.build_match(
+                    b, c, f"{chunk_id}.{bid}.{cid}", skip_gt)
                 logging.debug("Made mat -> %s", mat)
                 base_matches.append(mat)
             match_matrix.append(base_matches)
 
         return np.array(match_matrix)
 
+    def check_refine_candidate(self, result):
+        """
+        Adds this region as a candidate for refinement if there are unmatched variants
+        """
+        has_unmatched = False
+        pos = []
+        chrom = None
+        for match in result:
+            has_unmatched |= not match.state
+            if match.base is not None:
+                chrom = match.base.chrom
+                pos.extend(truvari.entry_boundaries(match.base))
+            if match.comp is not None:
+                chrom = match.comp.chrom
+                pos.extend(truvari.entry_boundaries(match.comp))
+        if has_unmatched and pos:  # I don't think I need to confirm pos, but unsure
+            self.refine_candidates.append(f"{chrom}\t{min(*pos)}\t{max(*pos)}")
+
 
 #################
 # Match Pickers #
 #################
 def pick_multi_matches(match_matrix):
     """
     Given a numpy array of MatchResults
@@ -546,14 +668,15 @@
 
     for c_max in match_matrix.max(axis=0):
         c_max = copy.copy(c_max)
         c_max.base = None
         ret.append(c_max)
     return ret
 
+
 def pick_ac_matches(match_matrix):
     """
     Given a numpy array of MatchResults
     Find upto allele count mumber of matches
     """
     ret = []
     base_cnt, comp_cnt = match_matrix.shape
@@ -573,25 +696,25 @@
         # Only write the comp (FP)
         if base_cnt == 0 and not comp_is_used:
             to_process = copy.copy(match)
             to_process.base = None
             to_process.multi = to_process.state
             to_process.state = False
             comp_cnt -= 1
-            if used_comp[c_key] == 0: # Only write as F if it hasn't been a T
+            if used_comp[c_key] == 0:  # Only write as F if it hasn't been a T
                 ret.append(to_process)
             used_comp[c_key] = 9
         # Only write the base (FN)
         elif comp_cnt == 0 and not base_is_used:
             to_process = copy.copy(match)
             to_process.comp = None
             to_process.multi = to_process.state
             to_process.state = False
             base_cnt -= 1
-            if used_base[b_key] == 0: # Only write as F if it hasn't been a T
+            if used_base[b_key] == 0:  # Only write as F if it hasn't been a T
                 ret.append(to_process)
             used_base[b_key] = 9
         # Write both (any state)
         elif not base_is_used and not comp_is_used:
             to_process = copy.copy(match)
             # Don't write twice
             if used_base[b_key] != 0:
@@ -608,52 +731,57 @@
                 comp_cnt -= 1
 
             # Safety edge case check
             if to_process.base is not None or to_process.comp is not None:
                 ret.append(to_process)
     return ret
 
+
 def pick_single_matches(match_matrix):
     """
     Given a numpy array of MatchResults, find the single best match for calls
     Once all best pairs yielded, the unpaired calls are set to FP/FN and yielded
     """
-    hit_order = np.array(np.unravel_index(np.argsort(match_matrix, axis=None), match_matrix.shape)).T
+    hit_order = np.array(np.unravel_index(np.argsort(
+        match_matrix, axis=None), match_matrix.shape)).T
     top_hit_idx = len(hit_order) - 1
 
-    mask = np.ones(match_matrix.shape, dtype='bool') # True = can use
+    mask = np.ones(match_matrix.shape, dtype='bool')  # True = can use
+    ret = []
 
     used_pairs = []
     while top_hit_idx >= 0 and mask.any():
         idx = tuple(hit_order[top_hit_idx])
         if mask[idx]:
             mask[idx[0], :] = False
             mask[:, idx[1]] = False
             used_pairs.append(idx)
-            yield match_matrix[idx]
+            ret.append(match_matrix[idx])
         top_hit_idx -= 1
 
-    used_base, used_comp = zip(*used_pairs) if used_pairs else ([],[])
+    used_base, used_comp = zip(*used_pairs) if used_pairs else ([], [])
     # FNs
     for base_col in set(range(match_matrix.shape[0])) - set(used_base):
         comp_col = match_matrix[base_col].argmax()
         to_process = copy.copy(match_matrix[base_col, comp_col])
-        to_process.comp = None # The comp will be written elsewhere
+        to_process.comp = None  # The comp will be written elsewhere
         to_process.multi = to_process.state
         to_process.state = False
-        yield to_process
+        ret.append(to_process)
 
     # FPs
     for comp_col in set(range(match_matrix.shape[1])) - set(used_comp):
         base_col = match_matrix[:, comp_col].argmax()
         to_process = copy.copy(match_matrix[base_col, comp_col])
-        to_process.base = None # The base will be written elsewhere
+        to_process.base = None  # The base will be written elsewhere
         to_process.multi = to_process.state
         to_process.state = False
-        yield to_process
+        ret.append(to_process)
+    return ret
+
 
 PICKERS = {"single": pick_single_matches,
            "ac": pick_ac_matches,
            "multi": pick_multi_matches
            }
 
 
@@ -665,12 +793,13 @@
 
     if check_params(args) or check_inputs(args):
         sys.stderr.write("Couldn't run Truvari. Please fix parameters\n")
         sys.exit(100)
 
     matcher = truvari.Matcher(args)
 
-    m_bench = Bench(matcher, args.base, args.comp, args.output, args.includebed, args.extend, args.debug, True)
+    m_bench = Bench(matcher, args.base, args.comp, args.output,
+                    args.includebed, args.extend, args.debug, True)
     output = m_bench.run()
 
     logging.info("Stats: %s", json.dumps(output.stats_box, indent=4))
     logging.info("Finished bench")
```

### Comparing `Truvari-4.0.0/truvari/collapse.py` & `Truvari-4.1.0/truvari/collapse.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,26 +6,28 @@
 
 import os
 import sys
 import json
 import logging
 import argparse
 import itertools
-from functools import cmp_to_key
+import statistics
+from functools import cmp_to_key, partial
 
 import pysam
 
 import truvari
 import truvari.bench as trubench
 
-def collapse_chunk(chunk):
+
+def collapse_chunk(chunk, matcher):
     """
     For calls in a chunk, separate which ones should be kept from collapsed
     """
-    matcher, chunk_dict, chunk_id = chunk
+    chunk_dict, chunk_id = chunk
     calls = chunk_dict['base']
     logging.debug("Collapsing chunk %d", chunk_id)
     # Need to add a deterministic sort here...
     calls.sort(key=matcher.sorter)
 
     # keep_key : [keep entry, [collap matches], match_id, gt_consolidate_count]
     ret = {}
@@ -38,15 +40,16 @@
         # Take the first variant
         cur_keep_candidate = calls.pop(0)
         keep_key = truvari.entry_to_key(cur_keep_candidate)
         # if chain, any matches we find will be added to a previous keep
         if matcher.chain and keep_key in chain_lookup:
             keep_key = chain_lookup[keep_key]
         else:  # otherwise, this is assumed to be a keep call
-            ret[keep_key] = [cur_keep_candidate, [], f'{chunk_id}.{call_id}', 0]
+            ret[keep_key] = [cur_keep_candidate,
+                             [], f'{chunk_id}.{call_id}', 0]
 
         # Separate calls collapsing with this keep from the rest
         remaining_calls = []
         for cur_collapse_candidate in calls:
             mat = matcher.build_match(cur_keep_candidate,
                                       cur_collapse_candidate,
                                       ret[keep_key][2],
@@ -72,15 +75,16 @@
             ret[keep_key][1] = [mats.pop(0)]
             remaining_calls.extend(mat.comp for mat in mats)
 
         calls = remaining_calls
 
     if matcher.no_consolidate:
         for val in ret.values():
-            edited_entry, collapse_cnt = collapse_into_entry(val[0], val[1], matcher.hap)
+            edited_entry, collapse_cnt = collapse_into_entry(
+                val[0], val[1], matcher.hap)
             val[0] = edited_entry
             val[3] = collapse_cnt
 
     ret = list(ret.values())
     for i in chunk_dict['__filtered']:
         ret.append([i, None, None, 0])
     ret.sort(key=cmp_to_key(lambda x, y: x[0].pos - y[0].pos))
@@ -104,37 +108,40 @@
         replace_gts.append("HET")
 
     # Each sample of this entry needs to be checked/set
     n_consolidate = 0
     for sample in entry.samples:
         m_gt = truvari.get_gt(entry.samples[sample]["GT"]).name
         if m_gt not in replace_gts:
-            continue # already set
+            continue  # already set
         n_idx = None
         for pos, o_entry in enumerate(others):
             o_entry = o_entry.comp
             o_gt = truvari.get_gt(o_entry.samples[sample]["GT"]).name
             if o_gt not in replace_gts:
                 n_idx = pos
-                break # this is the first other that's set
+                break  # this is the first other that's set
         # consolidate
         if hap_mode and m_gt == "HET":
             entry.samples[sample]["GT"] = (1, 1)
             n_consolidate += 1
         elif n_idx is not None:
             n_consolidate += 1
             o_entry = others[n_idx].comp
             for key in set(entry.samples[sample].keys() + o_entry.samples[sample].keys()):
                 try:
                     entry.samples[sample][key] = o_entry.samples[sample][key]
                 except TypeError:
                     # Happens for things like PL when one is null but its expecting a tuple
-                    logging.debug("Unable to set FORMAT %s for sample %s", key, sample)
-                    logging.debug("Kept entry: %s:%d %s", entry.chrom, entry.pos, entry.id)
-                    logging.debug("Colap entry: %s:%d %s", o_entry.chrom, o_entry.pos, o_entry.id)
+                    logging.debug("Unable to set FORMAT %s for sample %s",
+                                  key, sample)
+                    logging.debug("Kept entry: %s:%d %s",
+                                  entry.chrom, entry.pos, entry.id)
+                    logging.debug("Colap entry: %s:%d %s",
+                                  o_entry.chrom, o_entry.pos, o_entry.id)
                 except KeyError:
                     logging.debug("Unshared format %s in sample %s ignored for pair %s:%d %s %s:%d %s",
                                   key, sample, entry.chrom, entry.pos, entry.id, o_entry.chrom,
                                   o_entry.pos, o_entry.id)
     return entry, n_consolidate
 
 
@@ -148,14 +155,15 @@
     gtB = entryB.samples[0]["GT"]
     if gtA == (1, 1) or gtB == (1, 1):
         return False
     if gtA == gtB:
         return False
     return True
 
+
 def sort_length(b1, b2):
     """
     Order entries from longest to shortest SVLEN, ties are by alphanumeric of REF
     """
     s1 = truvari.entry_size(b1)
     s2 = truvari.entry_size(b2)
     if s1 < s2:
@@ -164,14 +172,15 @@
         return -1
     if b1.ref < b2.ref:
         return 1
     if b1.ref > b2.ref:
         return -1
     return 0
 
+
 def sort_first(b1, b2):
     """
     Order entries from left-most to right-most POS
     """
     if b1.pos > b2.pos:
         return 1
     if b1.pos < b2.pos:
@@ -198,44 +207,54 @@
     mac2 = truvari.allele_freq_annos(b2)["MAC"]
     if mac1 < mac2:
         return 1
     if mac1 > mac2:
         return -1
     return sort_first(b1, b2)
 
+
 SORTS = {'first': cmp_to_key(sort_first),
          'maxqual': cmp_to_key(sort_maxqual),
          'common': cmp_to_key(sort_common)}
 
 
 #######
 # VCF #
 #######
-def edit_header(my_vcf):
+def edit_header(my_vcf, median_info=False):
     """
     Add INFO for new fields to vcf
     """
     header = my_vcf.header.copy()
     header.add_line(('##INFO=<ID=NumCollapsed,Number=1,Type=Integer,'
                      'Description="Number of calls collapsed into this call by truvari">'))
     header.add_line(('##INFO=<ID=CollapseId,Number=1,Type=String,'
                      'Description="Truvari uid to help tie output.vcf and output.collapsed.vcf entries together">'))
     header.add_line(('##INFO=<ID=NumConsolidated,Number=1,Type=Integer,'
                      'Description="Number of samples consolidated into this call by truvari">'))
+    if median_info:
+        header.add_line(('##INFO=<ID=CollapseStart,Number=1,Type=Integer,'
+                        'Description="Median start position of collapsed variants">'))
+        header.add_line(('##INFO=<ID=CollapseEnd,Number=1,Type=Integer,'
+                        'Description="Median end position of collapsed variants">'))
+        header.add_line(('##INFO=<ID=CollapseSize,Number=1,Type=Integer,'
+                        'Description="Median size of collapsed variants">'))
     return header
 
 
-def annotate_entry(entry, num_collapsed, num_consolidate, match_id, header):
+def annotate_entry(entry, n_collap, n_consol, match_id, med_info, header):
     """
     Edit an entry that's going to be collapsed into another entry
     """
     entry.translate(header)
-    entry.info["NumCollapsed"] = num_collapsed
-    entry.info["NumConsolidated"] = num_consolidate
+    entry.info["NumCollapsed"] = n_collap
+    entry.info["NumConsolidated"] = n_consol
     entry.info["CollapseId"] = match_id
+    if med_info:
+        entry.info["CollapseStart"], entry.info["CollapseEnd"], entry.info["CollapseSize"] = med_info
 
 
 ##################
 # Args & Outputs #
 ##################
 def parse_args(args):
     """
@@ -249,14 +268,16 @@
                         help="Output vcf (stdout)")
     parser.add_argument("-c", "--collapsed-output", type=str, default="collapsed.vcf",
                         help="Where collapsed variants are written (collapsed.vcf)")
     parser.add_argument("-f", "--reference", type=str, default=None,
                         help="Indexed fasta used to call variants")
     parser.add_argument("-k", "--keep", choices=["first", "maxqual", "common"], default="first",
                         help="When collapsing calls, which one to keep (%(default)s)")
+    parser.add_argument("--median-info", action="store_true",
+                        help="Store median start/end/size of collapsed entries in kept's INFO")
     parser.add_argument("--debug", action="store_true", default=False,
                         help="Verbose logging")
 
     thresg = parser.add_argument_group("Comparison Threshold Arguments")
     thresg.add_argument("-r", "--refdist", type=truvari.restricted_int, default=500,
                         help="Max reference location distance (%(default)s)")
     thresg.add_argument("-p", "--pctseq", type=truvari.restricted_float, default=0.95,
@@ -304,20 +325,20 @@
     """
     check_fail = False
     if not os.path.exists(args.input):
         check_fail = True
         logging.error("File %s does not exist", args.input)
     if not args.input.endswith(".gz"):
         check_fail = True
-        logging.error(
-            "Input vcf %s does not end with .gz. Must be bgzip'd", args.input)
+        logging.error("Input vcf %s does not end with .gz. Must be bgzip'd",
+                      args.input)
     if not os.path.exists(args.input + '.tbi'):
         check_fail = True
-        logging.error(
-            "Input vcf index %s.tbi does not exist. Must be indexed", args.input)
+        logging.error("Input vcf index %s.tbi does not exist. Must be indexed",
+                      args.input)
     if args.hap and args.chain:
         check_fail = True
         logging.error("Cannot specify both --hap and --chain")
     if args.hap and args.keep != "first":
         check_fail = True
         logging.error("Using --hap must use --keep first")
     return check_fail
@@ -340,54 +361,75 @@
     matcher.chain = args.chain
     matcher.sorter = SORTS[args.keep]
     matcher.no_consolidate = args.no_consolidate
     matcher.picker = 'single'
 
     return matcher
 
+
 def setup_outputs(args):
     """
     Makes all of the output files for collapse
 
     returns a dictionary holding outputs
     """
     truvari.setup_logging(args.debug, show_version=True)
     logging.info("Params:\n%s", json.dumps(vars(args), indent=4))
 
     outputs = {}
 
     in_vcf = pysam.VariantFile(args.input)
-    outputs["o_header"] = edit_header(in_vcf)
+    outputs["o_header"] = edit_header(in_vcf, args.median_info)
     outputs["c_header"] = trubench.edit_header(in_vcf)
     num_samps = len(outputs["o_header"].samples)
     if args.hap and num_samps != 1:
         logging.error(
             "--hap mode requires exactly one sample. Found %d", num_samps)
         sys.exit(100)
     outputs["output_vcf"] = pysam.VariantFile(args.output, 'w',
                                               header=outputs["o_header"])
     outputs["collap_vcf"] = pysam.VariantFile(args.collapsed_output, 'w',
                                               header=outputs["c_header"])
-    outputs["stats_box"] = {"collap_cnt": 0, "kept_cnt": 0, "out_cnt": 0, "consol_cnt": 0}
+    outputs["stats_box"] = {"collap_cnt": 0, "kept_cnt": 0,
+                            "out_cnt": 0, "consol_cnt": 0}
     return outputs
 
 
-def output_writer(to_collapse, outputs):
+def calc_median_sizepos(entry, collapsed):
+    """
+    Given a set of variants, calculate the median start, end, and size
+    """
+    st, en = truvari.entry_boundaries(entry)
+    sz = truvari.entry_size(entry)
+    starts = [st]
+    ends = [en]
+    sizes = [sz]
+    for i in collapsed:
+        st, en = truvari.entry_boundaries(i.comp)
+        sz = truvari.entry_size(i.comp)
+        starts.append(st)
+        ends.append(en)
+        sizes.append(sz)
+    return int(statistics.median(starts)), int(statistics.median(ends)), int(statistics.median(sizes))
+
+
+def output_writer(to_collapse, outputs, median_info=False):
     """
     Annotate and write kept/collapsed calls to appropriate files
     """
     entry, collapsed, match_id, consol_cnt = to_collapse
     # Save copying time
     if not collapsed:
         outputs["output_vcf"].write(entry)
         outputs["stats_box"]["out_cnt"] += 1
         return
 
-    annotate_entry(entry, len(collapsed), consol_cnt,
-                   match_id, outputs["o_header"])
+    med_info = calc_median_sizepos(entry, collapsed) if median_info else None
+    annotate_entry(entry, len(collapsed), consol_cnt, match_id,
+                   med_info, outputs["o_header"])
     outputs["output_vcf"].write(entry)
     outputs["stats_box"]["out_cnt"] += 1
     outputs["stats_box"]["kept_cnt"] += 1
     outputs["stats_box"]["consol_cnt"] += consol_cnt
     for match in collapsed:
         trubench.annotate_entry(match.comp, match, outputs["c_header"])
         outputs["collap_vcf"].write(match.comp)
@@ -413,16 +455,18 @@
         sys.exit(100)
 
     matcher = build_collapse_matcher(args)
     outputs = setup_outputs(args)
     base = pysam.VariantFile(args.input)
 
     chunks = truvari.chunker(matcher, ('base', base))
-    for call in itertools.chain.from_iterable(map(collapse_chunk, chunks)):
-        output_writer(call, outputs)
+    m_colap = partial(collapse_chunk, matcher=matcher)
+    for call in itertools.chain.from_iterable(map(m_colap, chunks)):
+        output_writer(call, outputs, args.median_info)
 
     close_outputs(outputs)
     logging.info("Wrote %d Variants", outputs["stats_box"]["out_cnt"])
-    logging.info("%d variants collapsed into %d variants", outputs["stats_box"]["collap_cnt"],
-                 outputs["stats_box"]["kept_cnt"])
-    logging.info("%d samples' FORMAT fields consolidated", outputs["stats_box"]["consol_cnt"])
+    logging.info("%d variants collapsed into %d variants",
+                 outputs["stats_box"]["collap_cnt"], outputs["stats_box"]["kept_cnt"])
+    logging.info("%d samples' FORMAT fields consolidated",
+                 outputs["stats_box"]["consol_cnt"])
     logging.info("Finished collapse")
```

### Comparing `Truvari-4.0.0/truvari/comparisons.py` & `Truvari-4.1.0/truvari/comparisons.py`

 * *Files 0% similar despite different names*

```diff
@@ -193,29 +193,33 @@
 
     # Inversions handled differently
     if entry_variant_type(entryA) == truvari.SV.INV and entry_variant_type(entryB) == truvari.SV.INV:
         allele1 = entryA.alts[0]
         allele2 = entryB.alts[0]
         return seqsim(allele1, allele2)
 
-    a_seq = entryA.ref if entry_variant_type(entryA) == truvari.SV.DEL else entryA.alts[0]
-    b_seq = entryB.ref if entry_variant_type(entryB) == truvari.SV.DEL else entryB.alts[0]
+    a_seq = entryA.ref if entry_variant_type(
+        entryA) == truvari.SV.DEL else entryA.alts[0]
+    b_seq = entryB.ref if entry_variant_type(
+        entryB) == truvari.SV.DEL else entryB.alts[0]
     st_dist, ed_dist = entry_distance(entryA, entryB)
 
     if st_dist == 0 or ed_dist == 0:
         return seqsim(a_seq, b_seq)
 
     if ref is not None:
-        allele1, allele2 = entry_shared_ref_context(entryA, entryB, ref, min_len=min_len)
+        allele1, allele2 = entry_shared_ref_context(
+            entryA, entryB, ref, min_len=min_len)
         return seqsim(allele1, allele2)
 
     if st_dist > 0:
         return unroll_compare(a_seq, b_seq, st_dist % len(b_seq))
     return unroll_compare(b_seq, a_seq, st_dist % len(a_seq))
 
+
 def entry_reciprocal_overlap(entry1, entry2):
     """
     Calculates reciprocal overlap of two entries
 
     :param `entry1`: First entry
     :type `entry1`: :class:`pysam.VariantRecord`
     :param `entry2`: Second entry
@@ -320,15 +324,15 @@
         start, end = entry_boundaries(entry)
         size = end - start
     else:
         r_len = len(entry.ref)
         a_len = len(entry.alts[0]) if entry.alts is not None else 0
         if r_len == a_len:
             if r_len == 1:
-                size = 0 # SNPs are special
+                size = 0  # SNPs are special
             else:
                 size = r_len
         else:
             size = abs(r_len - a_len)
     return size
 
 
@@ -353,14 +357,15 @@
         >>> truvari.entry_size_similarity(a, b)
         (0.07142857142857142, 13)
     """
     sizeA = entry_size(entryA)
     sizeB = entry_size(entryB)
     return sizesim(sizeA, sizeB)
 
+
 def entry_to_hash(entry, hasher=hashlib.sha1):
     """
     Turn variant into a key and hash with provided hasher
 
     :param `entry`: entry
     :type `entry`: :class:`pysam.VariantRecord`
     :param `hasher`: hashing function
```

### Comparing `Truvari-4.0.0/truvari/consistency.py` & `Truvari-4.1.0/truvari/consistency.py`

 * *Files identical despite different names*

### Comparing `Truvari-4.0.0/truvari/divide.py` & `Truvari-4.1.0/truvari/divide.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import concurrent.futures
 
 import pysam
 import pandas as pd
 
 import truvari
 
+
 def parse_args(args):
     """
     Pull the command line parameters
     """
     parser = argparse.ArgumentParser(prog="divide", description=__doc__,
                                      formatter_class=argparse.RawDescriptionHelpFormatter)
     parser.add_argument("input", metavar="VCF",
@@ -30,26 +31,28 @@
                         help="Don't attempt to compress/index sub-VCFs")
     parser.add_argument("-T", "--threads", type=int, default=1,
                         help="Number of threads for compressing/indexing sub-VCFs (%(default)s)")
     args = parser.parse_args(args)
     truvari.setup_logging(show_version=True)
     return args
 
+
 def flush_stack(in_vcf, stack, out_name, compress=True):
     """
     write the stack to out_name
     """
     logging.debug(f"{out_name} has {len(stack)} entries")
     cur_out = pysam.VariantFile(out_name, mode='w', header=in_vcf.header)
     for i in stack:
         cur_out.write(i)
     cur_out.close()
     if compress:
         truvari.compress_index_vcf(out_name)
 
+
 def divide_main(args):
     """
     Main
     """
     args = parse_args(args)
 
     if os.path.exists(args.output):
@@ -65,50 +68,54 @@
         oname = list(os.path.splitext(".".join(oname)))
 
     if oname[-1] != ".vcf":
         logging.error("Expected VCF input. Pysam may raise error")
     oname.pop(-1)
     oname = ".".join(oname)
 
-    out_name_template = os.path.join(args.output, oname) + "_{part_num:08d}.vcf"
+    out_name_template = os.path.join(
+        args.output, oname) + "_{part_num:08d}.vcf"
     cluster_counts = []
     stack = [next(in_vcf)]
 
     max_end = stack[0].stop
 
-    with concurrent.futures.ThreadPoolExecutor(max_workers = args.threads) as executor:
+    with concurrent.futures.ThreadPoolExecutor(max_workers=args.threads) as executor:
         futures = {}
         for entry in in_vcf:
             if entry.chrom != stack[0].chrom and len(stack) >= args.min:
                 m_name = out_name_template.format(part_num=len(cluster_counts))
-                futures[executor.submit(flush_stack, in_vcf, stack, m_name, args.no_compress)] = m_name
-                #flush_stack(in_vcf, stack, m_name, args.no_compress)
+                futures[executor.submit(
+                    flush_stack, in_vcf, stack, m_name, args.no_compress)] = m_name
+                # flush_stack(in_vcf, stack, m_name, args.no_compress)
                 cluster_counts.append(len(stack))
                 max_end = entry.stop
                 stack = [entry]
             elif entry.start >= max_end + args.buffer and len(stack) >= args.min:
                 m_name = out_name_template.format(part_num=len(cluster_counts))
-                futures[executor.submit(flush_stack, in_vcf, stack, m_name, args.no_compress)] = m_name
-                #flush_stack(in_vcf, stack, m_name, args.no_compress)
+                futures[executor.submit(
+                    flush_stack, in_vcf, stack, m_name, args.no_compress)] = m_name
+                # flush_stack(in_vcf, stack, m_name, args.no_compress)
                 cluster_counts.append(len(stack))
                 stack = [entry]
                 max_end = entry.stop
             else:
                 stack.append(entry)
                 max_end = max(max_end, entry.stop)
 
         if stack:
             m_name = out_name_template.format(part_num=len(cluster_counts))
-            futures[executor.submit(flush_stack, in_vcf, stack, m_name, args.no_compress)] = m_name
-            #flush_stack(in_vcf, stack, m_name, args.no_compress)
+            futures[executor.submit(
+                flush_stack, in_vcf, stack, m_name, args.no_compress)] = m_name
+            # flush_stack(in_vcf, stack, m_name, args.no_compress)
             cluster_counts.append(len(stack))
 
         for future in concurrent.futures.as_completed(futures):
             m_result = futures[future]
             try:
                 future.result()
-            except Exception as exc: # pylint: disable=broad-except
+            except Exception as exc:  # pylint: disable=broad-except
                 logging.error('%s generated an exception: %s', m_result, exc)
 
     cluster_counts = pd.Series(cluster_counts)
 
     logging.info(cluster_counts.describe())
```

### Comparing `Truvari-4.0.0/truvari/matching.py` & `Truvari-4.1.0/truvari/matching.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import types
 import logging
 from collections import Counter, defaultdict
 from functools import total_ordering
 import pysam
 import truvari
 
+
 @total_ordering
 class MatchResult():  # pylint: disable=too-many-instance-attributes
     """
     A base/comp match holder
     """
     __slots__ = ["base", "comp", "base_gt", "base_gt_count", "comp_gt", "comp_gt_count",
                  "state", "seqsim", "sizesim", "ovlpct", "sizediff", "st_dist", "ed_dist",
@@ -110,14 +111,16 @@
         params.dup_to_ins = False
         params.sizemin = 50
         params.sizefilt = 30
         params.sizemax = 50000
         params.passonly = False
         params.no_ref = False
         params.pick = 'single'
+        params.ignore_monref = True
+        params.check_multi = True
         return params
 
     @staticmethod
     def make_match_params_from_args(args):
         """
         Makes a simple namespace of matching parameters
         """
@@ -136,32 +139,38 @@
         # filtering properties
         ret.sizemin = args.sizemin
         ret.sizefilt = args.sizefilt
         ret.sizemax = args.sizemax
         ret.passonly = args.passonly
         ret.no_ref = args.no_ref
         ret.pick = args.pick if "pick" in args else "single"
+        ret.check_monref = True
+        ret.check_multi = True
         return ret
 
     def filter_call(self, entry, base=False):
         """
         Returns True if the call should be filtered
         Base has different filtering requirements, so let the method know
         """
-        if self.params.passonly and truvari.entry_is_filtered(entry):
+        if self.params.check_monref and entry.alts is None:  # ignore monomorphic reference
             return True
 
-        size = truvari.entry_size(entry)
-        if size > self.params.sizemax:
-            return True
+        if self.params.check_multi and len(entry.alts) > 1:
+            logging.error("Cannot compare multi-allelic records. Please split")
+            logging.error("line %s", str(entry))
+            sys.exit(10)
 
-        if base and size < self.params.sizemin:
+        if self.params.passonly and truvari.entry_is_filtered(entry):
             return True
 
-        if not base and size < self.params.sizefilt:
+        size = truvari.entry_size(entry)
+        if (size > self.params.sizemax) \
+           or (base and size < self.params.sizemin) \
+           or (not base and size < self.params.sizefilt):
             return True
 
         samp = self.params.bSample if base else self.params.cSample
         prefix = 'b' if base else 'c'
         if (self.params.no_ref in ["a", prefix] or self.params.pick == 'ac') and not truvari.entry_is_present(entry, samp):
             return True
 
@@ -219,15 +228,16 @@
                           str(base), str(comp), ret.ovlpct)
             ret.state = False
             if short_circuit:
                 return ret
 
         ret.st_dist, ret.ed_dist = truvari.entry_distance(base, comp)
         if self.params.pctseq > 0:
-            ret.seqsim = truvari.entry_seq_similarity(base, comp, self.reference, self.params.minhaplen)
+            ret.seqsim = truvari.entry_seq_similarity(
+                base, comp, self.reference, self.params.minhaplen)
             if ret.seqsim < self.params.pctseq:
                 logging.debug("%s and %s sequence similarity is too low (%.3ff)",
                               str(base), str(comp), ret.seqsim)
                 ret.state = False
                 if short_circuit:
                     return ret
         else:
@@ -236,88 +246,92 @@
         ret.calc_score()
 
         return ret
 
 ############################
 # Parsing and set building #
 ############################
+
+
 def file_zipper(*start_files):
     """
     Zip files to yield the entries in order.
     Each file must be sorted in the same order.
     start_files is a tuple of ('key', iterable)
     where key is the identifier (so we know which file the yielded entry came from)
     and iterable is usually a pysam.VariantFile
 
     yields key, pysam.VariantRecord
     """
-    markers = [] # list of lists: [name, file_handler, top_entry]
+    markers = []  # list of lists: [name, file_handler, top_entry]
     file_counts = Counter()
     for name, i in start_files:
         try:
             markers.append([name, i, next(i)])
         except StopIteration:
             # For when there are no variants in the file
             pass
 
     while markers:
         # Get the first entry among each of the files' tops
         first_idx = 0
         for idx, mk in enumerate(markers[1:]):
             idx += 1
             if mk[2].chrom < markers[first_idx][2].chrom or \
-              (mk[2].chrom == markers[first_idx][2].chrom and mk[2].start < markers[first_idx][2].start):
+                    (mk[2].chrom == markers[first_idx][2].chrom and mk[2].start < markers[first_idx][2].start):
                 first_idx = idx
         name, fh, entry = markers[first_idx]
         file_counts[name] += 1
         try:
             # update this file's top
             markers[first_idx][2] = next(fh)
         except StopIteration:
             # This file is done
             markers.pop(first_idx)
         yield name, entry
-    logging.info("Zipped %d variants %s", sum(file_counts.values()), file_counts)
+    logging.info("Zipped %d variants %s", sum(
+        file_counts.values()), file_counts)
+
 
 def chunker(matcher, *files):
     """
     Given a Matcher and multiple files, zip them and create chunks
 
-    Yields tuple of the matcher, the chunk of calls, and an identifier of the chunk
+    Yields tuple of the chunk of calls, and an identifier of the chunk
     """
     call_counts = Counter()
     chunk_count = 0
     cur_chrom = None
     cur_end = None
     cur_chunk = defaultdict(list)
+    unresolved_warned = False
     for key, entry in file_zipper(*files):
-        if len(entry.alts) > 1:
-            logging.error("Cannot compare multi-allelic records. Please split")
-            logging.error("%s file - line %s", key, str(entry))
-            sys.exit(10)
-        if entry.alts is None: # ignore monomorphic reference
+        if matcher.params.pctseq != 0 and entry.alts[0].startswith('<'):
+            if not unresolved_warned:
+                logging.warning(
+                    "Unresolved SVs (e.g. ALT=<DEL>) are filtered when `--pctseq != 0`")
+                unresolved_warned = True
             cur_chunk['__filtered'].append(entry)
             call_counts['__filtered'] += 1
-            cur_chrom = entry.chrom
             continue
         new_chrom = cur_chrom and entry.chrom != cur_chrom
         new_chunk = cur_end and cur_end + matcher.params.chunksize < entry.start
         if new_chunk or new_chrom:
             chunk_count += 1
-            yield matcher, cur_chunk, chunk_count
+            yield cur_chunk, chunk_count
             # Reset
             cur_chrom = None
             cur_end = None
             cur_chunk = defaultdict(list)
 
         cur_chrom = entry.chrom
         if not matcher.filter_call(entry, key == 'base'):
-            logging.debug(f"Adding to {key} -> {entry}")
             cur_end = entry.stop
             cur_chunk[key].append(entry)
             call_counts[key] += 1
         else:
             cur_chunk['__filtered'].append(entry)
             call_counts['__filtered'] += 1
     chunk_count += 1
-    logging.info("%d chunks of %d variants %s", chunk_count, sum(call_counts.values()), call_counts)
-    yield matcher, cur_chunk, chunk_count
+    logging.info("%d chunks of %d variants %s", chunk_count,
+                 sum(call_counts.values()), call_counts)
+    yield cur_chunk, chunk_count
```

### Comparing `Truvari-4.0.0/truvari/msa2vcf.py` & `Truvari-4.1.0/truvari/msatovcf.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,99 +1,101 @@
 """
 Turn an MSA fasta into VCF. Assumes one entry is reference with name >ref_chrom:start-end
 """
 import copy
 from io import StringIO
 from collections import defaultdict
 
-import pysam
-
+POSIDX = 1
 REFIDX = 3
 ALTIDX = 4
 
-def build_header(chrom=None):
-    """
-    Bare minimum vcf header
-    """
-    ret = '##fileformat=VCFv4.1\n##FORMAT=<ID=GT,Number=1,Type=String,Description="Genotype">'
-    if chrom is not None:
-        ret += f"\n##contig=<ID={chrom}>\n"
-    return ret
 
 def decompose_variant(cur_variant):
     """
     Left trim and decompose (repl -> indel) variant
     returns a list of new variants
     """
     def var_to_str(v):
         return "\t".join([str(_) for _ in v])
     ref = cur_variant[REFIDX]
     alt = cur_variant[ALTIDX]
     if ref == alt:
         return []
-    # If base after anchor base is identical, we have a new anchor base
-    # Stop when there's only one base left or unmached bases
+
+    # If anchor base is identical, we can move down
+    # Stop when there's only one base left or an unmached anchor base
     trim = 0
     while trim < len(ref) - 1 and trim < len(alt) - 1 and ref[trim] == alt[trim]:
         trim += 1
     cur_variant[1] += trim
     cur_variant[REFIDX] = ref[trim:]
     cur_variant[ALTIDX] = alt[trim:]
     if len(cur_variant[REFIDX]) == 1 or len(cur_variant[ALTIDX]) == 1:
         return [var_to_str(cur_variant)]
 
-    # decompose REPL to INS and DEL - easier for truvari to compare
-    in_var = copy.copy(cur_variant)
-    in_var[REFIDX] = in_var[REFIDX][0]
+    # decompose REPL to DEL and INS - easier for truvari to compare
     del_var = copy.copy(cur_variant)
     del_var[ALTIDX] = del_var[ALTIDX][0]
-    return [var_to_str(in_var), var_to_str(del_var)]
+    del_var[REFIDX] = del_var[REFIDX][:-1]
+    in_var = copy.copy(cur_variant)
+    in_var[REFIDX] = in_var[REFIDX][-1]
+    in_var[ALTIDX] = in_var[ALTIDX][1:]
+    in_var[POSIDX] += len(cur_variant[REFIDX]) - 1
+    return [var_to_str(del_var), var_to_str(in_var)]
 
-def msa_to_vars(msa, ref_seq, chrom, start_pos=0, abs_anchor_base='N'):
+
+def msa_to_vars(msa, chrom, ref_seq=None, start_pos=0, abs_anchor_base='N'):
     """
     Turn MSA into VCF entries and their presence in samples
     returns list of sample names parsed and dictionary of variant : samples containing the variant
     """
     sample_names = set()
 
     final_vars = defaultdict(list)
 
-    for alt_key in msa.references:
+    for alt_key in msa.keys():
         if alt_key.startswith("ref_"):
             continue
-        # gross
-        cur_samp_hap = "_".join(alt_key.split('_')[:-1])
-        sample_names.add("_".join(alt_key.split('_')[:-2]))
-        alt_seq = msa[alt_key].upper()
+
+        # Trim off the location then haplotype from key sample
+        cur_samp_hap = alt_key[:alt_key.rindex('_')]
+        sample_names.add(cur_samp_hap[:-2])
+        if isinstance(msa[alt_key], tuple):
+            ref_seq, alt_seq = msa[alt_key]
+            ref_seq = ref_seq.upper()
+            alt_seq = alt_seq.upper()
+        else:
+            alt_seq = msa[alt_key].upper()
 
         anchor_base = ref_seq[0] if ref_seq[0] != '-' else abs_anchor_base
 
         cur_variant = []
-        cur_pos = start_pos # still have a problem here with anchor base.
+        cur_pos = start_pos
         # This is too long. need to have a separate zip method
         for ref_base, alt_base in zip(ref_seq, alt_seq):
             is_ref = ref_base != '-'
             if ref_base == '-':
                 ref_base = ""
             if alt_base == '-':
                 alt_base = ""
 
             # nothing to compare
             if not ref_base and not alt_base:
                 continue
 
-            if ref_base == alt_base: # No variant
-                if cur_variant and is_ref: # back to matching reference
+            if ref_base == alt_base:  # No variant
+                if cur_variant and is_ref:  # back to matching reference
                     for key in decompose_variant(cur_variant):
                         final_vars[key].append(cur_samp_hap)
                     cur_variant = []
             else:
                 if not cur_variant:
                     # -1 for the anchor base we're forcing on
-                    cur_variant = [chrom, cur_pos - 1, '.', anchor_base + ref_base, \
+                    cur_variant = [chrom, cur_pos - 1, '.', anchor_base + ref_base,
                                    anchor_base + alt_base, '.', '.', '.', 'GT']
                 else:
                     cur_variant[REFIDX] += ref_base
                     cur_variant[ALTIDX] += alt_base
             if is_ref:
                 cur_pos += 1
                 anchor_base = ref_base
@@ -101,53 +103,53 @@
         if cur_variant:
             for key in decompose_variant(cur_variant):
                 final_vars[key].append(cur_samp_hap)
         # End alignment
     sample_names = sorted(list(sample_names))
     return sample_names, final_vars
 
-def make_vcf(variants, sample_names, header):
+
+def make_vcf(variants, sample_names):
     """
-    Write VCF - building GTs
+    Write VCF lines - building GTs
     """
     out = StringIO()
-    out.write(header)
-    out.write("#CHROM	POS	ID	REF	ALT	QUAL	FILTER	INFO	FORMAT\t")
-    out.write("\t".join(sample_names) + '\n')
-
     for var in variants:
         out.write(var)
         for sample in sample_names:
             out.write('\t')
             gt = ["0", "0"]
             if sample + '_1' in variants[var]:
                 gt[0] = "1"
             if sample + '_2' in variants[var]:
                 gt[1] = "1"
             out.write("/".join(gt))
         out.write('\n')
     out.seek(0)
     return out.read()
 
-def msa2vcf(fn, header=None, anchor_base=None):
+
+def msa2vcf(msa, anchor_base='N'):
     """
-    Parse an MSA file and returns its VCF as a string
+    Parse an MSA dict of {name: alignment, ...} and returns its VCF entries as a string
 
     Assumes one entry in the MSA has the name `ref_${chrom}:${start}-${end}` which gives VCF entries coordinates
-
-    VCF can be given a header or a minimal one is created with only file format and a single contig line
     Provide anchor_base to prevent 'N' from being used as an anchor base
-    Returns a string
-    """
-    msa = pysam.FastaFile(fn)
-
-    # The ref_key identifies reference
-    ref_key = [_ for _ in msa.references if _.startswith("ref_")][0] # pylint: disable=not-an-iterable
-    ref_seq = msa[ref_key].upper()
-    _, chrom, start_pos, _ = ref_key.split('_')
-    start_pos = int(start_pos)
-
-    sample_names, variants = msa_to_vars(msa, ref_seq, chrom, start_pos, anchor_base)
-    if header is None:
-        header = build_header(chrom)
+    Returns a string of entries
 
-    return make_vcf(variants, sample_names, header)
+    Example (for dealing with test coverage not being seen)
+        >>> import truvari
+        >>> from truvari.phab import fasta_reader
+        >>> msa_dir = "repo_utils/test_files/external/fake_mafft/lookup/"
+        >>> msa_file = "fm_ca43b50e2a5d770bb34202d8a7b62421.msa"
+        >>> seqs = open(msa_dir + msa_file).read()
+        >>> fasta = {n:s.decode() for n, s in fasta_reader(seqs, False)}
+        >>> m_entries_str = truvari.msa2vcf(fasta)
+    """
+    ref_key = [_ for _ in msa.keys() if _.startswith("ref_")][0]
+    chrom, rest = ref_key[len("ref_"):].split(':')
+    ref_seq = msa[ref_key].upper() if isinstance(msa[ref_key], str) else None
+    start_pos = int(rest.split('-')[0])
+
+    sample_names, variants = msa_to_vars(
+        msa, chrom, ref_seq, start_pos, anchor_base)
+    return make_vcf(variants, sample_names)
```

### Comparing `Truvari-4.0.0/truvari/phab.py` & `Truvari-4.1.0/truvari/phab.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,77 +1,45 @@
 """
-Wrapper around MAFFT and other tools to perform an MSA comparison of phased variants
+Wrapper around MAFFT and other tools to harmonize phased variants
 """
 import os
 import re
 import sys
-import glob
 import shutil
 import logging
 import argparse
-import resource
 import multiprocessing
+from io import BytesIO
+from functools import partial
+from collections import defaultdict
 
 import pysam
-from pysam import bcftools
+from pysam import bcftools, samtools
+from intervaltree import IntervalTree
+from pywfa.align import WavefrontAligner  # pylint: disable=no-name-in-module
 import truvari
 
-DEFAULT_MAFFT_PARAM="--auto --thread 1"
+DEFAULT_MAFFT_PARAM = "--auto --thread 1"
 
-def parse_args(args):
-    """
-    Pull the command line parameters
-    """
-    parser = argparse.ArgumentParser(prog="phab", description=__doc__,
-                                     formatter_class=argparse.RawDescriptionHelpFormatter)
-    parser.add_argument("-r", "--region", type=str, required=True,
-                        help="Bed filename or comma-separated list of chrom:start-end regions to process")
-    # could maybe allow this to be an existing MSA and then we just use comp and add-to
-    parser.add_argument("-b", "--base", type=str, required=True,
-                        help="Baseline vcf to MSA")
-    parser.add_argument("-c", "--comp", type=str, default=None,
-                        help="Comparison vcf to MSA")
-    parser.add_argument("-f", "--reference", type=str, required=True,
-                        help="Reference")
-    parser.add_argument("--buffer", type=int, default=100,
-                        help="Number of reference bases before/after region to add to MSA (%(default)s)")
-    #parser.add_argument("--add-to", action='store_true',
-    #                    help="Build the baseMSA independentally of the compMSA, then add the comp")
-    parser.add_argument("-o", "--output", type=str, default="phab_out.vcf.gz",
-                        help="Output VCF")
-    parser.add_argument("-k", "--keep-parts", type=str, default=None,
-                        help="Directory to save intermediate region results")
-    parser.add_argument("--bSamples", type=str, default=None,
-                        help="Subset of samples to MSA from base-VCF")
-    parser.add_argument("--cSamples", type=str, default=None,
-                        help="Subset of samples to MSA from comp-VCF")
-    parser.add_argument("-m", "--mafft-params", type=str, default=DEFAULT_MAFFT_PARAM,
-                        help="Parameters for mafft, wrap in a single quote (%(default)s)")
-    parser.add_argument("-t", "--threads", type=int, default=1,
-                        help="Number of threads (%(default)s)")
-    parser.add_argument("--debug", action="store_true",
-                        help="Verbose logging")
-    args = parser.parse_args(args)
-    return args
 
 def parse_regions(argument):
     """
-    Parse the --region rgument
+    Parse the --region argument
     returns list of regions
     """
     ret = []
     if not argument:
         return ret
     if os.path.exists(argument):
         for i in truvari.opt_gz_open(argument):
             try:
                 chrom, start, end = i.strip().split('\t')[:3]
                 start = int(start)
                 end = int(end)
-            except Exception: #pylint: disable=broad-except
+            except Exception:  # pylint: disable=broad-except
                 logging.error("Unable to parse bed line %s", i)
                 sys.exit(1)
             ret.append((chrom, start, end))
     else:
         for i in argument.split(','):
             try:
                 chrom, start, end = re.split(':|-', i)
@@ -79,210 +47,339 @@
                 end = int(end)
             except ValueError:
                 logging.error("Unable to parse region line %s", i)
                 sys.exit(1)
             ret.append((chrom, start, end))
     return ret
 
-def get_reference(fn, output, chrom, start, end):
+
+def merged_region_file(regions, buff=100):
     """
-    Pull a subset of the reference and put into a file
-    Returns the anchor base (1bp upstream from start) for msa2vcf
+    Write a file for extracting reference regions with samtools
+    returns the name of the temporary file made
     """
-    fasta = pysam.FastaFile(fn)
-    oseq = fasta.fetch(chrom, start - 2, end)
-    # no need to make it pretty?
-    #oseq = re.sub("(.{60})", "\\1\n", oseq, 0, re.DOTALL)
-    with open(output, 'w') as fout:
-        fout.write(f">ref_{chrom}_{start}_{end}\n{oseq[1:]}\n")
-    with open(output + '.ref.fa', 'w') as fout:
-        fout.write(f">{chrom}:{start}-{end}\n{oseq[1:]}\n")
-    return oseq[0]
-
-def pull_variants(vcf, region, output, ref, samples=None):
-    """
-    Given vcf and a region, grab the relevant variants
-    Maybe can make fill-from fasta optional.. but it isn't huge overhead (for now)
-    """
-    chrom, start, end = region
-    if samples is not None:
-        samples = "-s " + ",".join(samples)
-    else:
-        samples = ""
-    cmd = f"""bcftools view -c 1 {samples} -r {chrom}:{start}-{end} {vcf} \
-| bcftools +fill-from-fasta /dev/stdin -- -c REF -f {ref} \
-| bgzip > {output} && tabix {output}"""
+    m_dict = defaultdict(list)
+    for i in regions:
+        m_dict[i[0]].append((max(0, i[1] - buff), i[2] + buff))
 
-    ret = truvari.cmd_exe(cmd, pipefail=True)
-    if ret.ret_code != 0:
-        logging.error("Unable to pull variants from %s", vcf)
-        logging.error(ret.stderr)
-        sys.exit(1)
-    cnt = 0
-    with pysam.VariantFile(output) as fh:
-        for _ in fh:
-            cnt += 1
-    return cnt
-
-def build_consensus(vcf, ref, region, output, samples=None, prefix_name=False):
-    """
-    Make the consensus sequence - appends to output
-    """
-    chrom, start, end = region
-    prefix = 'p:' if prefix_name else ''
-    ref = output + '.ref.fa'
-    cmd = "cat {ref} | bcftools consensus -H{hap} --sample {sample} --prefix {prefix}{sample}_{hap}_ {vcf} >> {output}"
-    for samp in samples:
+    out_file_name = truvari.make_temp_filename()
+    with open(out_file_name, 'w') as fout:
+        for chrom in sorted(m_dict.keys()):
+            intvs = IntervalTree.from_tuples(m_dict[chrom])
+            intvs.merge_overlaps()
+            for i in sorted(intvs):
+                fout.write(f"{chrom}:{i.begin}-{i.end}\n")
+    return out_file_name
+
+
+def extract_reference(reg_fn, ref_fn):
+    """
+    Pull the reference
+    """
+    out_fn = truvari.make_temp_filename(suffix='.fa')
+    with open(out_fn, 'w') as fout:
+        fout.write(samtools.faidx(ref_fn, "-r", reg_fn))
+    return out_fn
+
+
+def make_haplotype_jobs(base_vcf, bSamples, comp_vcf, cSamples, prefix_comp):
+    """
+    Sets up sample parameters for extract haplotypes
+    returns list of tuple of (VCF, sample_name, should_prefix, haplotype_number) and the sample names
+    to expect in the haplotypes' fasta
+    """
+    ret = []
+    if bSamples is None:
         for hap in [1, 2]:
-            m_cmd = cmd.format(ref=ref,
-                               chrom=chrom,
-                               start=start,
-                               end=end,
-                               hap=hap,
-                               sample=samp,
-                               prefix=prefix,
-                               vcf=vcf,
-                               output=output)
-            ret = truvari.cmd_exe(m_cmd, pipefail=True)
-            if ret.ret_code != 0:
-                logging.error("Unable to make haplotype %d for sample %s", hap, samp)
-                logging.error(ret.stderr)
-                sys.exit(1)
+            ret.extend([(base_vcf, samp, False, hap)
+                        for samp in list(pysam.VariantFile(base_vcf).header.samples)])
+    if comp_vcf and cSamples is None:
+        bsamps = list(pysam.VariantFile(base_vcf).header.samples)
+        for hap in [1, 2]:
+            ret.extend([(comp_vcf, samp, prefix_comp or samp in bsamps, hap)
+                        for samp in list(pysam.VariantFile(comp_vcf).header.samples)])
+    samp_names = sorted({('p:' if prefix else '') + samp
+                          for _, samp, prefix, _ in ret})
+    return ret, samp_names
+
+
+def fasta_reader(fa_str, name_entries=True):
+    """
+    Parses a fasta file as a string and yields tuples of (location, entry)
+    if name_entries, the entry names are written to the value and location is honored
+    """
+    cur_name = None
+    cur_entry = BytesIO()
+    for i in fa_str.split('\n'):
+        if not i.startswith(">"):
+            cur_entry.write(i.encode())
+            continue
+        if cur_name is not None:
+            cur_entry.write(b'\n')
+            cur_entry.seek(0)
+            yield cur_name, cur_entry.read()
+        cur_name = i[1:]
+        cur_entry = BytesIO()
+        if name_entries:
+            cur_name = cur_name.split('_')[-1]
+            cur_entry.write((i + '\n').encode())
+
+    cur_entry.write(b'\n')
+    cur_entry.seek(0)
+    yield cur_name, cur_entry.read()
+
+
+def extract_haplotypes(data, ref_fn):
+    """
+    Given a data tuple of VCF, sample name, and prefix bool
+    Call bcftools consensus
+    Returns list of tuples [location, fastaentry] for every haplotype,
+    so locations are duplicated
+    """
+    vcf_fn, sample, prefix, hap = data
+    prefix = 'p:' if prefix else ''
+    cmd = (f"--sample {sample} --prefix {prefix}{sample}_{hap}_ "
+           f"-H{hap} -f {ref_fn} {vcf_fn}").split(' ')
+    # Can't return generator from process
+    return list(fasta_reader(bcftools.consensus(*cmd)))
+
 
-def run_mafft(seq_fn, output, params=DEFAULT_MAFFT_PARAM):
+def collect_haplotypes(ref_haps_fn, hap_jobs, threads):
     """
-    Run mafft - return True if successful
+    Calls extract haplotypes for every hap_job
     """
-    cmd = f"mafft {params} {seq_fn} > {output}"
-    ret = truvari.cmd_exe(cmd)
+    all_haps = defaultdict(BytesIO)
+    with multiprocessing.Pool(threads, maxtasksperchild=1) as pool:
+        for haplotype in pool.imap(partial(extract_haplotypes, ref_fn=ref_haps_fn), hap_jobs):
+            for location, fasta_entry in haplotype:
+                all_haps[location].write(fasta_entry)
+        pool.close()
+        pool.join()
+    return all_haps
+
+
+def consolidate_haplotypes_with_reference(all_haps, ref_haps_fn):
+    """
+    Generator for putting the reference into the haplotypes
+    """
+    m_ref = pysam.FastaFile(ref_haps_fn)
+    for location in list(m_ref.references):
+        all_haps[location].write(
+            f">ref_{location}\n{m_ref[location]}\n".encode())
+        all_haps[location].seek(0)
+        yield all_haps[location].read()
+
+
+def expand_cigar(seq, ref, cigar):
+    """
+    Put gaps '-' in sequence where needed
+    """
+    seq_pos = 0
+    seq = list(seq)
+    ref_pos = 0
+    ref = list(ref)
+    for code, span in cigar:
+        if code == 2:
+            seq.insert(seq_pos, '-' * span)
+            seq_pos += 1
+            ref_pos += span
+        elif code == 1:
+            ref.insert(ref_pos, '-' * span)
+            seq_pos += span
+            ref_pos += 1
+        else:
+            seq_pos += span
+            ref_pos += span
+    return "".join(ref), "".join(seq)
+
+
+def wfa_to_vars(seq_bytes):
+    """
+    Align haplotypes independently with WFA
+    Much faster than mafft, but may be less accurate at finding parsimonous representations
+    """
+    fasta = {k: v.decode() for k, v in fasta_reader(
+        seq_bytes.decode(), name_entries=False)}
+    ref_key = [_ for _ in fasta.keys() if _.startswith("ref_")][0]
+    reference = fasta[ref_key]
+
+    aligner = WavefrontAligner(
+        reference, span="end-to-end", heuristic="adaptive")
+    for haplotype in fasta:
+        if haplotype == ref_key:
+            continue
+        seq = fasta[haplotype]
+        aligner.wavefront_align(seq)
+        assert aligner.status == 0
+        fasta[haplotype] = expand_cigar(seq, reference, aligner.cigartuples)
+    return truvari.msa2vcf(fasta)
+
+
+def mafft_to_vars(seq_bytes, params=DEFAULT_MAFFT_PARAM):
+    """
+    Run mafft on the provided sequences provided as a bytestr and return msa2vcf lines
+    """
+    # Dev only method for overwriting test answers - don't use until code is good
+    dev_name = None
+    if "PHAB_WRITE_MAFFT" in os.environ and os.environ["PHAB_WRITE_MAFFT"] == "1":
+        import hashlib  # pylint: disable=import-outside-toplevel
+        dev_name = hashlib.md5(seq_bytes).hexdigest()
+
+    cmd = f"mafft --quiet {params} -"
+    ret = truvari.cmd_exe(cmd, stdin=seq_bytes)
     if ret.ret_code != 0:
-        logging.error("Unable to run MAFFT on %s", seq_fn)
+        logging.error("Unable to run MAFFT")
         logging.error(ret.stderr)
-        return False
-    return True
+        return ""
 
-# pylint: disable=too-many-locals
-def phab(base_vcf, reference, output_dir, var_region, buffer=100,
-        comp_vcf=None, bSamples=None, cSamples=None,
-        mafft_params=DEFAULT_MAFFT_PARAM, prefix_comp=False):
+    if dev_name is not None:
+        with open("repo_utils/test_files/external/fake_mafft/lookup/fm_" + dev_name + ".msa", 'w') as fout:
+            fout.write(ret.stdout)
+
+    fasta = {}
+    for name, sequence in fasta_reader(ret.stdout, name_entries=False):
+        fasta[name] = sequence.decode()
+    return truvari.msa2vcf(fasta)
+
+
+def harmonize_variants(harm_jobs, mafft_params, base_vcf, samp_names, output_fn, threads, method="mafft"):
     """
-    Harmonize variants with MSA.
+    Parallel processing of variants to harmonize. Writes to output
+    """
+    if method == "mafft":
+        align_method = partial(mafft_to_vars, params=mafft_params)
+    else:
+        align_method = wfa_to_vars
 
+    with open(output_fn[:-len(".gz")], 'w') as fout:
+        fout.write(
+            '##fileformat=VCFv4.1\n##FORMAT=<ID=GT,Number=1,Type=String,Description="Genotype">\n')
+        for ctg in pysam.VariantFile(base_vcf).header.contigs.values():
+            fout.write(str(ctg.header_record))
+        fout.write("#CHROM\tPOS\tID\tREF\tALT\tQUAL\tFILTER\tINFO\tFORMAT\t")
+        fout.write("\t".join(samp_names) + "\n")
+
+        with multiprocessing.Pool(threads) as pool:
+            for result in pool.imap_unordered(align_method, harm_jobs):
+                fout.write(result)
+            pool.close()
+            pool.join()
+
+    truvari.compress_index_vcf(output_fn[:-len(".gz")], output_fn)
+
+
+# pylint: disable=too-many-arguments
+# This is just how many arguments it takes
+def phab(var_regions, base_vcf, ref_fn, output_fn, bSamples=None, buffer=100,
+         mafft_params=DEFAULT_MAFFT_PARAM, comp_vcf=None, cSamples=None,
+         prefix_comp=False, threads=1, method="mafft"):
+    """
+    Harmonize variants with MSA. Runs on a set of regions given files to create
+    haplotypes and writes results to a compressed/indexed VCF
+
+    :param `var_regions`: List of tuples of region's (chrom, start, end)
+    :type `var_regions`: :class:`list`
     :param `base_vcf`: VCF file name
     :type `base_vcf`: :class:`str`
-    :param `reference`: Reference file name
-    :type `reference`: :class:`str`
-    :param `output_dir`: Destination for results
-    :type `output_dir`: :class:`str`
-    :param `var_region`: Tuple of region's (chrom, start, end)
-    :type `var_region`: :class:`tuple`
-    :param `buffer`: Flanking reference bases to add to haplotypes
+    :param `ref_fn`: Reference file name
+    :type `ref_fn`: :class:`str`
+    :param `output_fn`: Output VCF.gz
+    :param `bSamples`: Samples from `base_vcf` to create haplotypes
+    :type `bSamples`: :class:`list`
+    :param `buffer`: Flanking reference bases to added to regions
     :type `buffer`: :class:`int`
+    :param `mafft_params`: Parameters for mafft
+    :type `mafft_params`: :class:`str`
     :param `comp_vcf`: VCF file name
     :type `comp_vcf`: :class:`str`
-    :param `bSamples`: Samples from `base_vcf` to create haplotypes
-    :type `bSamples`: :class:`list`
     :param `cSamples`: Samples from `comp_vcf` to create haplotypes
     :type `cSamples`: :class:`list`
-    :param `mafft_params`: Parameters for mafft
-    :type `mafft_params`: :class:`str`
     :param `prefix_comp`: Ensure unique sample names by prefixing comp samples
     :type `prefix_comp`: :class:`bool`
-    """
-    if not os.path.exists(output_dir):
-        os.makedirs(output_dir)
+    :param `threads`: Number of threads to use
+    :type `threads`: :class:`int`
+    :param `method`: Alignment method to use mafft or wfa
+    :type `method`: :class:`str`
+    """
+    logging.info("Preparing regions")
+    region_fn = merged_region_file(var_regions, buffer)
+
+    logging.info("Extracting haplotypes")
+    ref_haps_fn = extract_reference(region_fn, ref_fn)
+    hap_jobs, samp_names = make_haplotype_jobs(
+        base_vcf, bSamples, comp_vcf, cSamples, prefix_comp)
+    sample_haps = collect_haplotypes(ref_haps_fn, hap_jobs, threads)
+    harm_jobs = consolidate_haplotypes_with_reference(sample_haps, ref_haps_fn)
+
+    logging.info("Harmonizing variants")
+    harmonize_variants(harm_jobs, mafft_params, base_vcf,
+                       samp_names, output_fn, threads, method)
+# pylint: enable=too-many-arguments
+
+######
+# UI #
+######
 
-    buff_region = (var_region[0], var_region[1] - buffer, var_region[2] + buffer)
 
-    if bSamples is None:
-        bSamples = list(pysam.VariantFile(base_vcf).header.samples)
-    if comp_vcf and cSamples is None:
-        cSamples = list(pysam.VariantFile(comp_vcf).header.samples)
+def parse_args(args):
+    """
+    Pull the command line parameters
+    """
+    parser = argparse.ArgumentParser(prog="phab", description=__doc__,
+                                     formatter_class=argparse.RawDescriptionHelpFormatter)
+    parser.add_argument("-r", "--region", type=str, required=True,
+                        help="Bed filename or comma-separated list of chrom:start-end regions to process")
+    parser.add_argument("-b", "--base", type=str, required=True,
+                        help="Baseline vcf to MSA")
+    parser.add_argument("-c", "--comp", type=str, default=None,
+                        help="Comparison vcf to MSA")
+    parser.add_argument("-f", "--reference", type=str, required=True,
+                        help="Reference")
+    parser.add_argument("--buffer", type=int, default=100,
+                        help="Number of reference bases before/after region to add to MSA (%(default)s)")
+    parser.add_argument("-o", "--output", type=str, default="phab_out.vcf.gz",
+                        help="Output VCF")
+    parser.add_argument("--bSamples", type=str, default=None,
+                        help="Subset of samples to MSA from base-VCF")
+    parser.add_argument("--cSamples", type=str, default=None,
+                        help="Subset of samples to MSA from comp-VCF")
+    parser.add_argument("-m", "--mafft-params", type=str, default=DEFAULT_MAFFT_PARAM,
+                        help="Parameters for mafft, wrap in a single quote (%(default)s)")
+    parser.add_argument("--align", type=str, choices=["mafft", "wfa"], default="mafft",
+                        help="Alignment method accurate (mafft) or fast (wfa) (%(default)s)")
+    parser.add_argument("-t", "--threads", type=int, default=1,
+                        help="Number of threads (%(default)s)")
+    parser.add_argument("--debug", action="store_true",
+                        help="Verbose logging")
+    args = parser.parse_args(args)
+    return args
 
-    # Make sure there are variants first
-    subset_base_vcf = os.path.join(output_dir, "base.vcf.gz")
-    num_vars = pull_variants(base_vcf, var_region, subset_base_vcf, reference, bSamples)
-    if comp_vcf is not None:
-        subset_comp_vcf = os.path.join(output_dir, "comp.vcf.gz")
-        num_vars += pull_variants(comp_vcf, var_region, subset_comp_vcf, reference, cSamples)
-
-    if num_vars == 0:
-        return
-
-    sequences = os.path.join(output_dir, "haps.fa")
-    anchor_base = get_reference(reference, sequences, *buff_region)
-
-    build_consensus(subset_base_vcf, reference, buff_region, sequences, bSamples)
-
-    if comp_vcf is not None:
-        build_consensus(subset_comp_vcf, reference, buff_region, sequences, cSamples, prefix_comp)
-
-    msa_output = os.path.join(output_dir, "msa.fa")
-    if not run_mafft(sequences, msa_output, mafft_params):
-        return
-
-    output_vcf = os.path.join(output_dir, "output.vcf")
-    vcf = pysam.VariantFile(base_vcf)
-    n_header = '##fileformat=VCFv4.1\n##FORMAT=<ID=GT,Number=1,Type=String,Description="Genotype">\n'
-    n_header += str(vcf.header.contigs[var_region[0]].header_record)
-
-    with open(output_vcf, 'w') as fout:
-        try:
-            fout.write(truvari.msa2vcf(msa_output, n_header, anchor_base))
-        except RuntimeWarning:
-            return
-
-    truvari.compress_index_vcf(output_vcf)
-# pylint: enable=too-many-locals
-
-def consolidate_phab_vcfs(phab_dir, out_vcf):
-    """
-    Consolidate all the phab output VCFs in a directory and write to compressed indexed vcf
-    """
-    def concat(file_names):
-        tmp_name = truvari.make_temp_filename(suffix=".vcf.gz")
-        files = truvari.make_temp_filename(suffix=".txt")
-        with open(files, 'w') as fout:
-            fout.write('\n'.join(file_names))
-        bcftools.concat("--no-version", "-O", "z", "-a", "-f", files, "-o", tmp_name, catch_stdout=False)
-        pysam.tabix_index(tmp_name, preset='vcf')
-        return tmp_name
-    max_files = (resource.getrlimit(resource.RLIMIT_NOFILE)[0] - 1) // 2
-    in_files = glob.glob(os.path.join(phab_dir, "*", "*", "output.vcf.gz"))
-    in_files.sort()
-    while len(in_files) > 1:
-        tmp_names = []
-        # bcftools gets weird with more than 1,010 files
-        for i in range(0, len(in_files), max_files):
-            tmp_names.append(concat(in_files[i:i+max_files]))
-        in_files = tmp_names
-    shutil.move(in_files[0], out_vcf)
-    shutil.move(in_files[0] + '.tbi', out_vcf + '.tbi')
 
-def check_requirements():
+def check_requirements(align):
     """
     ensure external programs are in PATH
     """
     check_fail = False
-    for prog in ["bcftools", "bgzip", "tabix", "mafft"]:
-        if not shutil.which(prog):
-            logging.error("Unable to find `%s` in PATH", prog)
+    if align == "mafft":
+        if not shutil.which("mafft"):
+            logging.error("Unable to find mafft in PATH")
             check_fail = True
     return check_fail
 
+
 def check_params(args):
     """
     Ensure files are okay to use
     """
     check_fail = False
     if not args.output.endswith(".vcf.gz"):
         logging.error("Output file must be a '.vcf.gz', got %s", args.output)
         check_fail = True
-    if args.keep_parts and os.path.isdir(args.keep_parts):
-        logging.error("Output directory '%s' already exists", args.keep_parts)
+    if os.path.exists(args.output):
+        logging.error("Output file already exists")
         check_fail = True
     if args.comp is not None and not os.path.exists(args.comp):
         logging.error("File %s does not exist", args.comp)
         check_fail = True
     if not os.path.exists(args.base):
         logging.error("File %s does not exist", args.base)
         check_fail = True
@@ -304,91 +401,29 @@
         check_fail = True
     if not os.path.exists(args.reference):
         logging.error("Reference %s does not exist", args.reference)
         check_fail = True
 
     return check_fail
 
-def phab_wrapper(job):
-    """
-    Convience function to call phab (which works no a single region)
-    job is a tuple of region, output_dir, and kwargs dict
-    """
-    try:
-        phab(var_region=job[0], output_dir=job[1], **job[2])
-    except Exception as e: #pylint: disable=broad-except
-        logging.critical("phab failed on %s\n%s", str(job[0]), e)
-
-#pylint: disable=too-many-arguments
-# This is just how many arguments it takes
-def phab_multi(base_vcf, reference, output_dir, var_regions, buf=100, comp_vcf=None,
-               bSamples=None, cSamples=None, mafft_params=DEFAULT_MAFFT_PARAM,
-               prefix_comp=False, threads=1):
-    """
-    Run phab on multiple regions
-    """
-    if not os.path.exists(output_dir):
-        os.makedirs(output_dir)
-
-    params = {"base_vcf": base_vcf,
-              "reference": reference,
-              "buffer": buf,
-              "comp_vcf": comp_vcf,
-              "bSamples": bSamples,
-              "cSamples": cSamples,
-              "mafft_params": mafft_params,
-              "prefix_comp": prefix_comp}
-    with multiprocessing.Pool(threads, maxtasksperchild=1) as pool:
-        # build jobs
-        jobs = []
-        for region in var_regions:
-            m_output = os.path.join(output_dir, region[0], f"{region[0]}:{region[1]}-{region[2]}")
-            jobs.append((region, m_output, params))
-
-        pool.imap_unordered(phab_wrapper, jobs)
-        pool.close()
-        pool.join()
-#pylint: enable=too-many-arguments
 
 def phab_main(cmdargs):
     """
     Main
     """
     args = parse_args(cmdargs)
     truvari.setup_logging(args.debug, show_version=True)
-    if check_requirements() or check_params(args):
+    if check_requirements(args.align) or check_params(args):
         logging.error("Couldn't run Truvari. Please fix parameters\n")
         sys.exit(100)
 
-    # Setting up the samples is tricky
-    if args.bSamples is None:
-        args.bSamples = list(pysam.VariantFile(args.base).header.samples)
-    else:
+    if args.bSamples is not None:
         args.bSamples = args.bSamples.split(',')
 
-    if args.comp:
-        if args.cSamples is None:
-            args.cSamples = list(pysam.VariantFile(args.comp).header.samples)
-        else:
-            args.cSamples = args.cSamples.split(',')
-
-    prefix_comp = False
-    if args.cSamples and set(args.cSamples) & set(args.bSamples):
-        logging.warning("--cSamples intersect with --bSamples. Output vcf --comp SAMPLE names will have prefix 'p:'")
-        prefix_comp = True
+    if args.comp and args.cSamples is not None:
+        args.cSamples = args.cSamples.split(',')
 
     all_regions = parse_regions(args.region)
-    if args.keep_parts is None:
-        remove = True # remove at the end
-        args.keep_parts = truvari.make_temp_filename()
-    else:
-        remove = False
-    phab_multi(args.base, args.reference, args.keep_parts, all_regions, args.buffer, args.comp,
-               args.bSamples, args.cSamples, args.mafft_params, prefix_comp, args.threads)
-
-    consolidate_phab_vcfs(args.keep_parts, args.output)
-
-    if remove:
-        logging.info("Cleaning")
-        shutil.rmtree(args.keep_parts)
+    phab(all_regions, args.base, args.reference, args.output, args.bSamples, args.buffer,
+         args.mafft_params, args.comp, args.cSamples, threads=args.threads, method=args.align)
 
     logging.info("Finished phab")
```

### Comparing `Truvari-4.0.0/truvari/refine.py` & `Truvari-4.1.0/truvari/refine.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 """
 Automated Truvari bench result refinement with phab
 """
 import os
 import sys
 import json
-import shutil
 import logging
 import argparse
+from functools import partial
+import multiprocessing as mp
 from argparse import Namespace
 from collections import defaultdict
 
+import pysam
 import pandas as pd
-
 from pysam import bcftools
 from intervaltree import IntervalTree
 
 import truvari
+from truvari.phab import check_requirements as phab_check_requirements
 
+PHAB_BUFFER = 100 # hard-coded parameter :(
 def read_json(fn):
     """
     Parse json and return dict
     """
     ret = None
     with open(fn, 'r') as fh:
         ret = json.load(fh)
@@ -29,72 +32,82 @@
 def intersect_beds(bed_a, bed_b):
     """
     Return bed_a regions that intersect bed_b regions
     """
     shared = {}
     count = 0
     for chrom in bed_a:
+        a_intv = sorted(bed_a[chrom])
+        bed_b[chrom].merge_overlaps()
+        b_intv = sorted(bed_b[chrom])
+        a_idx = 0
+        b_idx = 0
         s_inc = []
-        for i in bed_a[chrom]:
-            if bed_b[chrom].overlaps(i):
-                count += 1
-                s_inc.append(i)
+        while a_idx < len(a_intv) and b_idx < len(b_intv):
+            if a_intv[a_idx].end < b_intv[b_idx].begin:
+                a_idx += 1
+                continue
+            if b_intv[b_idx].end < a_intv[a_idx].begin:
+                b_idx += 1
+                continue
+            # not before and not after means overlap
+            count += 1
+            s_inc.append(a_intv[a_idx])
+            a_idx += 1
         shared[chrom] = IntervalTree(s_inc)
     return shared, count
 
 def tree_to_regions(trees):
     """
     turn an anno tree into a list of lists of chrom start end
     """
-    return [[chrom, intv.begin, intv.end] for chrom, all_intv in trees.items() for intv in all_intv]
+    return [[chrom, intv.begin, intv.end] for chrom, all_intv in trees.items() for intv in sorted(all_intv)]
 
 def resolve_regions(params, args):
     """
     Figures out or creates the regions we'll be analyzing
     """
+    logging.info("Setting up regions")
     if params.includebed is None and args.regions is None:
         logging.error("Bench output didn't use `--includebed` and `--regions` not provided")
         logging.error("Unable to run refine")
         sys.exit(1)
     elif args.regions is None:
         reeval_trees, new_count = truvari.build_anno_tree(params.includebed, idxfmt="")
         logging.info("Evaluating %d regions", new_count)
     elif args.regions is not None and params.includebed is not None:
         a_trees, regi_count = truvari.build_anno_tree(args.regions, idxfmt="")
         b_trees, orig_count = truvari.build_anno_tree(params.includebed, idxfmt="")
-        if args.use_includebed:
-            reeval_trees, new_count = intersect_beds(b_trees, a_trees)
-            logging.info("%d --includebed reduced to %d after intersecting with %d from --regions",
-                     orig_count, new_count, regi_count)
-
-        else:
+        if args.use_region_coords:
             reeval_trees, new_count = intersect_beds(a_trees, b_trees)
             logging.info("%d --regions reduced to %d after intersecting with %d from --includebed",
                      regi_count, new_count, orig_count)
+        else:
+            reeval_trees, new_count = intersect_beds(b_trees, a_trees)
+            logging.info("%d --includebed reduced to %d after intersecting with %d from --regions",
+                     orig_count, new_count, regi_count)
     else:
         reeval_trees, count = truvari.build_anno_tree(args.regions, idxfmt="")
         logging.info("%d --regions loaded", count)
-    # might need to merge overlaps.
     return reeval_trees
 
-
 def consolidate_bench_vcfs(benchdir):
     """
     Pull and consolidate base/comp variants from their regions
     """
     bout_name = truvari.make_temp_filename(suffix=".vcf")
-    output = bcftools.concat("--no-version", *[os.path.join(benchdir, "tp-base.vcf.gz"),
-                            os.path.join(benchdir, "fn.vcf.gz")])
+    output = bcftools.concat("--no-version", "-a", os.path.join(benchdir, "tp-base.vcf.gz"),
+                            os.path.join(benchdir, "fn.vcf.gz"))
     with open(bout_name, 'w') as fout:
         fout.write(output)
     truvari.compress_index_vcf(bout_name)
 
     cout_name = truvari.make_temp_filename(suffix=".vcf")
-    output = bcftools.concat("--no-version", *[os.path.join(benchdir, "tp-comp.vcf.gz"),
-                            os.path.join(benchdir, "fp.vcf.gz")])
+    output = bcftools.concat("--no-version", "-a", os.path.join(benchdir, "tp-comp.vcf.gz"),
+                            os.path.join(benchdir, "fp.vcf.gz"))
     with open(cout_name, 'w') as fout:
         fout.write(output)
     truvari.compress_index_vcf(cout_name)
     return bout_name + '.gz', cout_name + '.gz'
 
 def make_variant_report(regions):
     """
@@ -106,28 +119,67 @@
     summary["FP"] = int(regions["out_fp"].sum())
     summary["FN"] = int(regions["out_fn"].sum())
     summary["base cnt"] = summary["TP-base"] + summary["FN"]
     summary["comp cnt"] = summary["TP-comp"] + summary["FP"]
     summary.calc_performance()
     return summary
 
+def recount_variant_report(orig_dir, phab_dir, regions):
+    """
+    Count original variants not in refined regions and
+    consolidate with the refined counts.
+    """
+    def falls_in_count(fn, no_count):
+        """ count number of variants that don't start in no_count """
+        vcf = pysam.VariantFile(fn)
+        count = 0
+        for entry in vcf:
+            if entry.chrom in no_count.index:
+                chrom = no_count.loc[entry.chrom]
+                if ((chrom['start'] <= entry.start) & (entry.start <= chrom['end'])).any():
+                    continue
+            count += 1
+        return count
+
+    summary = truvari.StatsBox()
+    with open(os.path.join(phab_dir, "summary.json")) as fh:
+        summary.update(json.load(fh))
+    # if the variant starts in a refined region, skip it
+    no_count = regions[regions["refined"]].copy().set_index('chrom')
+    no_count['start'] -= PHAB_BUFFER
+    no_count['end'] += PHAB_BUFFER
+
+    tpb = falls_in_count(os.path.join(orig_dir, 'tp-base.vcf.gz'), no_count)
+    summary["TP-base"] += tpb
+    tpc = falls_in_count(os.path.join(orig_dir, 'tp-comp.vcf.gz'), no_count)
+    summary["TP-comp"] += tpc
+    fp = falls_in_count(os.path.join(orig_dir, 'fp.vcf.gz'), no_count)
+    summary["FP"] += fp
+    fn = falls_in_count(os.path.join(orig_dir, 'fn.vcf.gz'), no_count)
+    summary["FN"] += fn
+
+    summary["comp cnt"] += tpc + fp
+    summary["base cnt"] += tpb + fn
+    summary.calc_performance()
+    return summary
+
+
 def make_region_report(data):
     """
     Given a refine counts DataFrame, calculate the performance of
     PPV, TNR, etc. Also adds 'state' column to regions inplace
     """
-    false_pos = (data['out_fp'] != 0)
-    false_neg = (data['out_fn'] != 0)
+    false_pos = data['out_fp'] != 0
+    false_neg = data['out_fn'] != 0
     any_false = false_pos | false_neg
 
     true_positives = (data['out_tp'] != 0) & (data['out_tpbase'] != 0) & ~any_false
 
     true_negatives = (data[['out_tpbase', 'out_tp', 'out_fn', 'out_fp']] == 0).all(axis=1)
 
-
     state_map = defaultdict(lambda: 'UNK')
     state_map.update({(True, False, False, False): 'TP',
                       (False, True, False, False): 'TN',
                       (False, False, True, False): 'FP',
                       (False, False, False, True): 'FN',
                       (False, False, True, True): 'FN,FP'})
 
@@ -150,25 +202,35 @@
     result["FP"] = int(false_pos.sum())
     result["FN"] = int(false_neg.sum())
     result["base P"] = baseP
     result["base N"] = baseN
     result["comp P"] = compP
     result["comp N"] = compN
     # precision
-    result["PPV"] = result["TP"] / result["comp P"]
+    result["PPV"] = result["TP"] / result["comp P"] if result["comp P"] != 0 else None
     # recall
-    result["TPR"] = result["TP"] / result["base P"]
+    result["TPR"] = result["TP"] / result["base P"] if result["base P"] != 0 else None
     # specificity
-    result["TNR"] = result["TN"] / result["base N"]
+    result["TNR"] = result["TN"] / result["base N"] if result["base N"] != 0 else None
     # negative predictive value
-    result["NPV"] = result["TN"] / result["comp N"]
+    result["NPV"] = result["TN"] / result["comp N"] if result["comp N"] != 0 else None
     # accuracy
-    result["ACC"] = (result["TP"] + result["TN"]) / (result["base P"] + result["base N"])
-    result["BA"] = (result["TPR"] + result["TNR"]) / 2
-    result["F1"] = 2 * ((result["PPV"] * result["TPR"]) / (result["PPV"] + result["TPR"]))
+    if result["base P"] + result["base N"] != 0:
+        result["ACC"] = (result["TP"] + result["TN"]) / (result["base P"] + result["base N"])
+    else:
+        result["ACC"] = None
+    if result["TPR"] is not None and result["TNR"] is not None:
+        result["BA"] = (result["TPR"] + result["TNR"]) / 2
+    else:
+        result["BA"] = None
+
+    if result["PPV"] and result["TPR"]:
+        result["F1"] = 2 * ((result["PPV"] * result["TPR"]) / (result["PPV"] + result["TPR"]))
+    else:
+        result["F1"] = None
     result["UND"] = len(und)
 
     return result
 
 def parse_args(args):
     """
     Pull the command line parameters
@@ -177,149 +239,174 @@
                                      formatter_class=argparse.RawDescriptionHelpFormatter)
     parser.add_argument("benchdir", metavar="DIR",
                         help="Truvari bench directory")
     parser.add_argument("-f", "--reference", type=str,
                         help="Indexed fasta used to call variants")
     parser.add_argument("-r", "--regions", default=None,
                         help="Regions to process")
-    parser.add_argument("-I", "--use-includebed", action="store_true",
-                        help="When intersecting includebed with regions, use includebed coordinates")
-    parser.add_argument("-u", "--use-original", action="store_true",
+    parser.add_argument("-u", "--use-original-vcfs", action="store_true",
                         help="Use original input VCFs instead of filtered tp/fn/fps")
-    parser.add_argument("-t", "--threads", default=1, type=int,
+    parser.add_argument("-U", "--use-region-coords", action="store_true",
+                        help="When subsetting the includebed with regions, use region coordinates")
+    parser.add_argument("-R", "--recount", action="store_true",
+                        help=("Recount all variants for refine.variant_summary instead of only "
+                              "those in analyzed regions"))
+    parser.add_argument("-t", "--threads", default=4, type=int,
                         help="Number of threads to use (%(default)s)")
-    parser.add_argument("-k", "--keep-phab", action="store_true",
-                        help="Keep the phab intermediate files")
+    parser.add_argument("--align", type=str, choices=["mafft", "wfa"], default="mafft",
+                        help="Alignment method for phab (%(default)s)")
     parser.add_argument("--debug", action="store_true",
                         help="Verbose logging")
     args = parser.parse_args(args)
-    truvari.setup_logging(args.debug, show_version=True)
     return args
 
 def check_params(args):
     """
     Sets up all the parameters from the bench/params.json
 
     Returns as a Namespace
     """
+    check_fail = False
     param_path = os.path.join(args.benchdir, "params.json")
     if not os.path.exists(param_path):
+        check_fail = True
         logging.error("Bench directory %s doesn't have params.json", param_path)
-        sys.exit(1)
     params = read_json(param_path)
 
+    p_file = os.path.join(args.benchdir, "phab.output.vcf.gz")
+    if os.path.exists(p_file):
+        check_fail = True
+        logging.error("Phab output file %s already exists", p_file)
+
     if params["reference"] is None and args.reference is None:
+        check_fail = True
         logging.error("Reference not in params.json or given as a parameter to refine")
-        sys.exit(1)
     elif args.reference is None:
         args.reference = params["reference"]
 
+
     if not os.path.exists(args.reference):
+        check_fail = True
         logging.error("Reference %s does not exist", args.reference)
-        sys.exit(1)
 
     # Setup prefix
     params["cSample"] = "p:" + params["cSample"]
 
-    phdir = os.path.join(args.benchdir, 'phab')
-    if os.path.exists(phdir):
-        logging.error("Directory %s exists. Cannot run refine", phdir)
-        sys.exit(1)
-
     bhdir = os.path.join(args.benchdir, 'phab_bench')
     if os.path.exists(bhdir):
+        check_fail = True
         logging.error("Directory %s exists. Cannot run refine", bhdir)
-        sys.exit(1)
 
     # Should check that bench dir has compressed/indexed vcfs for fetching
-    check_fail = False
     for i in ["tp-base.vcf.gz", "tp-comp.vcf.gz", "fn.vcf.gz", "fp.vcf.gz"]:
         if not os.path.exists(os.path.join(args.benchdir, i)):
-            logging.error("Benchdir doesn't have compressed/indexed %s", i)
             check_fail = True
+            logging.error("Benchdir doesn't have compressed/indexed %s", i)
+
     if check_fail:
+        logging.error("Please fix parameters")
         sys.exit(1)
 
-    os.makedirs(phdir)
     return Namespace(**params)
 
-def initial_stratify(benchdir, regions):
+def initial_stratify(benchdir, regions, threads=1):
     """
     Get the stratify counts from the initial bench results
     """
-    counts = truvari.benchdir_count_entries(benchdir, regions, True)[["tpbase", "tp", "fn", "fp"]]
+    counts = truvari.benchdir_count_entries(benchdir, regions, True, threads)[["tpbase", "tp", "fn", "fp"]]
     regions = pd.DataFrame(regions, columns=["chrom", "start", "end"])
     counts.index = regions.index
     counts.columns = ["in_tpbase", "in_tp", "in_fn", "in_fp"]
     regions = regions.join(counts)
     return regions
 
-def refined_stratify(outdir, to_eval_coords, regions):
+def original_stratify(base_vcf, comp_vcf, regions):
+    """
+    Get the variant counts from the original vcfs and return a list of refine bools
+    The logic here is that `(regions["in_fn"] > 0) | (regions["in_fp"] > 0)` may create
+    a number of regions which don't benefit from phab because either is without variants.
+    So, for that subset we'll double check that base AND comp have any variants to compare.
+    Some regions will still be evaluated for no good reason e.g. PASS only or a rogue snp.
+    """
+    to_eval = (regions["in_fn"] > 0) | (regions["in_fp"] > 0)
+    candidates = regions[to_eval]
+    chroms = candidates["chrom"].to_numpy()
+    intvs = candidates[["start", "end"]].to_numpy()
+    method = partial(truvari.count_entries, chroms=chroms, regions=intvs, within=True)
+    results = []
+    with mp.Pool(2, maxtasksperchild=1) as pool:
+        for result in pool.map(method, [base_vcf, comp_vcf]):
+            results.append(pd.Series(result, index=candidates.index))
+    return to_eval & (results[0] != 0) & (results[1] != 0)
+
+def refined_stratify(outdir, to_eval_coords, regions, threads=1):
     """
     update regions in-place with the output variant counts
     """
-    counts = truvari.benchdir_count_entries(outdir, to_eval_coords, True)[["tpbase", "tp", "fn", "fp"]]
+    counts = truvari.benchdir_count_entries(outdir, to_eval_coords, True, threads)[["tpbase", "tp", "fn", "fp"]]
     counts.index = regions[regions['refined']].index
     counts.columns = ["out_tpbase", "out_tp", "out_fn", "out_fp"]
     regions = regions.join(counts)
     for i in ["tpbase", "tp", "fn", "fp"]:
         regions[f"out_{i}"] = regions[f"in_{i}"].where(~regions['refined'], regions[f"out_{i}"])
     return regions
 
 def refine_main(cmdargs):
     """
     Main
     """
     args = parse_args(cmdargs)
+    if phab_check_requirements(args.align):
+        logging.error("Couldn't run Truvari. Please fix parameters\n")
+        sys.exit(100)
 
     params = check_params(args)
+    truvari.setup_logging(args.debug,
+                          truvari.LogFileStderr(os.path.join(args.benchdir, "refine.log.txt")),
+                          show_version=True)
+    logging.info("Params:\n%s", json.dumps(vars(args), indent=4))
 
     reeval_trees = resolve_regions(params, args)
     regions = tree_to_regions(reeval_trees)
 
     # Stratify.
-    regions = initial_stratify(args.benchdir, regions)
-
+    regions = initial_stratify(args.benchdir, regions, args.threads)
 
     # Figure out which to reevaluate
-    # Set the input VCFs for phab
-    if args.use_original:
+    if args.use_original_vcfs:
         base_vcf, comp_vcf = params.base, params.comp
-        regions["refined"] = (regions["in_fn"] > 0) | (regions["in_fp"] > 0)
+        regions["refined"] = original_stratify(base_vcf, comp_vcf, regions)
     else:
         base_vcf, comp_vcf = consolidate_bench_vcfs(args.benchdir)
         regions["refined"] = (regions["in_fn"] > 0) & (regions["in_fp"] > 0)
     logging.info("%d regions to be refined", regions["refined"].sum())
 
     reeval_bed = truvari.make_temp_filename(suffix=".bed")
     regions[regions["refined"]].to_csv(reeval_bed, sep='\t', header=False, index=False)
 
     # Send the vcfs to phab
-    to_eval_coords = regions[regions["refined"]][["chrom", "start", "end"]].to_numpy().tolist()
-    phab_dir = os.path.join(args.benchdir, "phab")
-    truvari.phab_multi(base_vcf, args.reference, phab_dir, to_eval_coords,
-                       comp_vcf=comp_vcf, prefix_comp=True, threads=args.threads)
-
     phab_vcf = os.path.join(args.benchdir, "phab.output.vcf.gz")
-    truvari.consolidate_phab_vcfs(phab_dir, phab_vcf)
+    to_eval_coords = regions[regions["refined"]][["chrom", "start", "end"]].to_numpy().tolist()
+    truvari.phab(to_eval_coords, base_vcf, args.reference, phab_vcf, buffer=PHAB_BUFFER, comp_vcf=comp_vcf,
+                 prefix_comp=True, threads=args.threads, method=args.align)
 
     # Now run bench on the phab harmonized variants
+    logging.info("Running bench")
     matcher = truvari.Matcher(params)
     matcher.params.no_ref = 'a'
     outdir = os.path.join(args.benchdir, "phab_bench")
     m_bench = truvari.Bench(matcher, phab_vcf, phab_vcf, outdir, reeval_bed)
     m_bench.run()
 
-    regions = refined_stratify(outdir, to_eval_coords, regions)
+    regions = refined_stratify(outdir, to_eval_coords, regions, args.threads)
 
-    summary = make_variant_report(regions)
+    summary = recount_variant_report(args.benchdir, outdir, regions) if args.recount else make_variant_report(regions)
+    summary.clean_out()
     summary.write_json(os.path.join(args.benchdir, 'refine.variant_summary.json'))
 
     report = make_region_report(regions)
+    regions['end'] -= 1 # Undo IntervalTree's correction
     regions.to_csv(os.path.join(args.benchdir, 'refine.regions.txt'), sep='\t', index=False)
-
     with open(os.path.join(args.benchdir, "refine.region_summary.json"), 'w') as fout:
         fout.write(json.dumps(report, indent=4))
 
-    if not args.keep_phab:
-        shutil.rmtree(phab_dir)
     logging.info("Finished refine")
```

### Comparing `Truvari-4.0.0/truvari/region_vcf_iter.py` & `Truvari-4.1.0/truvari/region_vcf_iter.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,16 @@
             logging.warning(
                 "Excluding %d contigs present in comparison calls header but not baseline calls.", len(excluding))
 
         for contig in contigA_set:
             name = vcfA.header.contigs[contig].name
             length = vcfA.header.contigs[contig].length
             if not length:
-                logging.error("Contig %s has no length definition. Fix header.", name)
+                logging.error(
+                    "Contig %s has no length definition. Fix header.", name)
                 sys.exit(10)
             all_regions[name].addi(0, length + 1)
         return all_regions
 
     def merge_overlaps(self):
         """
         Runs IntervalTree.merge_overlaps on all trees. Returns list of all chromosomes having overlapping regions
@@ -63,29 +64,30 @@
             pre_len = len(self.tree[i])
             self.tree[i].merge_overlaps()
             post_len = len(self.tree[i])
             if pre_len != post_len:
                 chr_with_overlaps.append(i)
         if chr_with_overlaps:
             logging.info("Found %d chromosomes with overlapping regions",
-                     len(chr_with_overlaps))
+                         len(chr_with_overlaps))
             logging.debug("CHRs: %s", chr_with_overlaps)
 
     def iterate(self, vcf_file):
         """
         Iterates a vcf and yields only the entries that overlap included regions
         """
         for chrom in sorted(self.tree.keys()):
             for intv in sorted(self.tree[chrom]):
                 try:
                     for entry in vcf_file.fetch(chrom, intv.begin, intv.end):
                         if self.includebed is None or self.include(entry):
                             yield entry
                 except ValueError:
-                    logging.warning("Unable to fetch %s from %s", chrom, vcf_file.filename)
+                    logging.warning("Unable to fetch %s from %s",
+                                    chrom, vcf_file.filename)
 
     def include(self, entry):
         """
         Returns if this entry's start and end are within a region that is to be included
         Here overlap means lies completely within the boundary of an include region
         """
         astart, aend = truvari.entry_boundaries(entry)
@@ -106,19 +108,21 @@
         Extends all intervals by a fixed number of bases on each side
         Returns a copy of this IntervalTree
         """
         logging.info("Extending the regions by %d bases", pad)
         ret = copy.deepcopy(self)
 
         for chrom in ret.tree:
-            ret.tree[chrom] = IntervalTree.from_tuples(((max(0, i.begin - pad), i.end + pad)) for i in ret.tree[chrom])
+            ret.tree[chrom] = IntervalTree.from_tuples(
+                ((max(0, i.begin - pad), i.end + pad)) for i in ret.tree[chrom])
 
         ret.merge_overlaps()
         return ret
 
+
 def build_anno_tree(filename, chrom_col=0, start_col=1, end_col=2, one_based=False, comment='#', idxfmt=None):
     """
     Build an dictionary of IntervalTrees for each chromosome from tab-delimited annotation file
 
     By default, the file is assumed to be a bed-format. If custom chrom/start/end are used, the columns can be
     specified.
```

### Comparing `Truvari-4.0.0/truvari/segmentation.py` & `Truvari-4.1.0/truvari/segmentation.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import pysam
 import numpy as np
 from intervaltree import IntervalTree
 
 import truvari
 from truvari.annotations import svinfo
 
+
 def parse_args(args):
     """
     Pull the command line parameters
     """
     parser = argparse.ArgumentParser(prog="segment", description=__doc__,
                                      formatter_class=argparse.RawDescriptionHelpFormatter)
```

### Comparing `Truvari-4.0.0/truvari/stratify.py` & `Truvari-4.1.0/truvari/stratify.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 """
 Count variants per-region in vcf
 """
 import os
+import logging
 import argparse
+import multiprocessing
+from functools import partial
 
 import pysam
+import numpy as np
 import pandas as pd
 
 import truvari
 
+
 def parse_args(args):
     """
     Pull the command line parameters
     """
     parser = argparse.ArgumentParser(prog="stratify", description=__doc__,
                                      formatter_class=argparse.RawDescriptionHelpFormatter)
     parser.add_argument("regions", metavar="BED",
@@ -27,55 +32,75 @@
                         help="Only count variants contained completely within region boundaries")
     parser.add_argument("--debug", action="store_true",
                         help="Verbose logging")
     args = parser.parse_args(args)
     truvari.setup_logging(args.debug, show_version=True)
     return args
 
-def count_entries(vcf, regions, within):
+
+def count_entries(vcf, chroms, regions, within):
     """
     Count the number of variants per bed region a VCF
     regions is a list of lists with sub-lists having 0:3 of chrom, start, end
     Returns a list of the counts in the same order as the regions
     """
+    if isinstance(vcf, str):
+        vcf = pysam.VariantFile(vcf)
     counts = [0] * len(regions)
-    for idx, row in enumerate(regions):
-        for entry in vcf.fetch(row[0], row[1], row[2]):
+    for idx, row in enumerate(zip(chroms, regions)):
+        chrom, coords = row
+        start, end = coords
+        for entry in vcf.fetch(chrom, start, end):
             if within:
                 ent_start, ent_end = truvari.entry_boundaries(entry)
-                if not (row[1] <= ent_start and ent_end <= row[2]):
+                if not (start <= ent_start and ent_end <= end):
                     continue
             counts[idx] += 1
     return counts
 
-def benchdir_count_entries(benchdir, regions, within=False):
+
+def benchdir_count_entries(benchdir, regions, within=False, threads=4):
     """
     Count the number of variants per bed region in Truvari bench directory by state
 
     Returns a pandas dataframe of the counts
     """
-    vcfs = {'tpbase': pysam.VariantFile(os.path.join(benchdir, 'tp-base.vcf.gz')),
-            'tp': pysam.VariantFile(os.path.join(benchdir, 'tp-comp.vcf.gz')),
-            'fn': pysam.VariantFile(os.path.join(benchdir, 'fn.vcf.gz')),
-            'fp': pysam.VariantFile(os.path.join(benchdir, 'fp.vcf.gz'))
-            }
+    names = ['tpbase', 'tp', 'fn', 'fp']
+    vcfs = [os.path.join(benchdir, 'tp-base.vcf.gz'),
+            os.path.join(benchdir, 'tp-comp.vcf.gz'),
+            os.path.join(benchdir, 'fn.vcf.gz'),
+            os.path.join(benchdir, 'fp.vcf.gz')]
+    if isinstance(regions, pd.DataFrame):
+        regions = regions.to_numpy().tolist()  # the methods expect lists
+    chroms = np.array([_[0] for _ in regions])
+    intvs = np.array([[_[1], _[2]] for _ in regions])
+    method = partial(count_entries, chroms=chroms,
+                     regions=intvs, within=within)
     data = {}
-    for name, vcf in vcfs.items():
-        data[name] = count_entries(vcf, regions, within)
+    # , maxtasksperchild=1) as pool:
+    with multiprocessing.Pool(threads) as pool:
+        for name, counts in zip(names, pool.map(method, vcfs)):
+            data[name] = counts
     return pd.DataFrame(data)
 
+
 def stratify_main(cmdargs):
     """
     stratify
     """
     args = parse_args(cmdargs)
     read_header = 0 if args.header else None
     regions = pd.read_csv(args.regions, sep='\t', header=read_header)
-    r_list = regions.to_numpy().tolist() # the methods expect lists
+    r_list = regions.to_numpy().tolist()  # the methods expect lists
     if os.path.isdir(args.in_vcf):
-        counts = benchdir_count_entries(args.in_vcf, r_list, args.within)[["tpbase", "tp", "fn", "fp"]]
+        counts = benchdir_count_entries(args.in_vcf, r_list, args.within)[
+            ["tpbase", "tp", "fn", "fp"]]
     else:
-        counts = count_entries(pysam.VariantFile(args.in_vcf), r_list, args.within)
+        chroms = np.array([_[0] for _ in r_list])
+        intvs = np.array([[_[1], _[2]] for _ in r_list])
+        counts = count_entries(pysam.VariantFile(
+            args.in_vcf), chroms, intvs, args.within)
         counts = pd.Series(counts, name="count").to_frame()
     counts.index = regions.index
     regions = regions.join(counts)
     regions.to_csv(args.output, header=args.header, index=False, sep='\t')
+    logging.info("Finished")
```

### Comparing `Truvari-4.0.0/truvari/utils.py` & `Truvari-4.1.0/truvari/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from pysam import bcftools
 
 import truvari
 
 HEADERMAT = re.compile(
     r"##\w+=<ID=(?P<name>\w+),Number=(?P<num>[\.01AGR]),Type=(?P<type>\w+)")
 
+
 def restricted_float(x):
     """
     Restrict float to range (0,1). Raises argparse.ArgumentTypeError if float is out of range
     Used with :class:`argparse.ArgumentParser.add_argument` type parameter
 
     :param `x`: number to check
     :type `x`: float
@@ -45,14 +46,15 @@
     """
     x = float(x)
     if x < 0 or x > 1:
         raise argparse.ArgumentTypeError(
             f"{x} not in range (0, 1)")
     return x
 
+
 def restricted_int(x):
     """
     Restrict int to positive. Raises argparse.ArgumentTypeError if int is negative
     Used with :class:`argparse.ArgumentParser.add_argument` type parameter
 
     :param `x`: number to check
     :type `x`: int
@@ -138,21 +140,23 @@
 
 
 def alarm_handler(signum, frame=None):
     """ Alarm handler for command timeouts """
     raise Alarm
 
 
-def cmd_exe(cmd, timeout=-1, cap_stderr=True, pipefail=False):
+def cmd_exe(cmd, stdin=None, timeout=-1, cap_stderr=True, pipefail=False):
     """
     Executes a command through the shell and captures the output while enabling
     process handling with timeouts and keyboard interrupts.
 
     :param `cmd`: The command to be executed.
     :type `cmd`: string
+    :param `stdin`: stdinput to pipe to command
+    :type `stdin`: bytes
     :param `timeout`: Timeout for the command in minutes. So 1440 means 24 hours. -1 means never
     :type `timeout`: int
     :param `cap_stderr`: If True, capture the stderr and return it as part of the returned cmd_results.
         Otherwise, stderr will be streamed through to the terminal
     :type `cap_stderr`: boolean
     :param `pipefail`: Set to True if the cmd contains pipes `|`
     :type `pipefail`: boolean
@@ -178,22 +182,23 @@
     """
     cmd_result = namedtuple("cmd_result", "ret_code stdout stderr run_time")
     t_start = time.time()
     stderr = subprocess.PIPE if cap_stderr else None
     if pipefail:
         cmd = f"set -o pipefail; {cmd}"
     # pylint: disable=consider-using-with
+    m_in = sys.stdin if stdin is None else subprocess.PIPE
     proc = subprocess.Popen(cmd, shell=True, stdout=subprocess.PIPE,
-                            stdin=sys.stdin, stderr=stderr, close_fds=True,
+                            stdin=m_in, stderr=stderr, close_fds=True,
                             start_new_session=True, executable="/bin/bash")
     if timeout > 0:
         signal.signal(signal.SIGALRM, alarm_handler)
         signal.alarm(int(timeout * 60))
     try:
-        stdoutVal, stderrVal = proc.communicate()
+        stdoutVal, stderrVal = proc.communicate(input=stdin)
         signal.alarm(0)  # reset the alarm
     except Alarm:
         logging.error(("Command was taking too long. "
                        "Automatic Timeout Initiated after %d"), timeout)
         os.killpg(proc.pid, signal.SIGTERM)
         proc.kill()
         return cmd_result(214, "", "", timedelta(seconds=time.time() - t_start))
@@ -269,14 +274,15 @@
             stop = start + chunk_size
             while stop < final_stop:
                 yield data[0], start, stop
                 start = stop
                 stop += chunk_size
             yield data[0], start, final_stop
 
+
 def vcf_ranges(vcf, min_dist=1000):
     """
     Chunk vcf into discrete pieces. Useful for multiprocessing.
 
     :param `vcf`: Filename of vcf to find ranges
     :type `vcf`: string
     :param `min_dist`: Minimum distance between entries for new range
@@ -312,14 +318,15 @@
             min_start = entry.start
             max_end = entry.stop
         else:
             max_end = max(max_end, entry.stop)
 
     yield cur_chrom, min_start, max_end
 
+
 def opt_gz_open(in_fn):
     """
     Chooses file handler for plain-text files or `*.gz` files.
 
     returns a generator which yields lines of the file
     """
     def gz_hdlr(fn):
@@ -333,23 +340,25 @@
                 yield line
 
     if in_fn.endswith('.gz'):
         return gz_hdlr(in_fn)
 
     return fh_hdlr(in_fn)
 
+
 def make_temp_filename(tmpdir=None, suffix=""):
     """
     Get a random filename in a tmpdir with an optional extension
     """
     if tmpdir is None:
-        tmpdir = tempfile._get_default_tempdir() # pylint: disable=protected-access
-    fn = os.path.join(tmpdir, next(tempfile._get_candidate_names())) + suffix # pylint: disable=protected-access
+        tmpdir = tempfile._get_default_tempdir()  # pylint: disable=protected-access
+    fn = os.path.join(tmpdir, next(tempfile._get_candidate_names())) + suffix  # pylint: disable=protected-access
     return fn
 
+
 def help_unknown_cmd(user_cmd, avail_cmds, threshold=0.8):
     """
     Guess the command in avail_cmds that's most similar to user_cmd. If there is
     no guess below threshold, don't guess.
 
     :param `user_cmd`: user command
     :type `user_cmd`: string
@@ -373,14 +382,15 @@
         if score >= threshold:
             guesses.append((score, real))
     guesses.sort()
     if not guesses:
         return None
     return guesses[-1][1]
 
+
 def performance_metrics(tpbase, tp, fn, fp):
     """
     Calculates precision, recall, and f1 given counts by state
     Can return None if values are zero
 
     :param `tpbase`: found base count
     :type `tpbase`: int
@@ -401,14 +411,15 @@
     precision = tp / comp_cnt
     recall = tpbase / base_cnt
     neum = recall * precision
     denom = recall + precision
     f1 = 2 * (neum / denom) if denom != 0 else None
     return precision, recall, f1
 
+
 def compress_index_vcf(fn, fout=None, remove=True):
     """
     Compress and index a vcf. If no fout is provided, write to fn + '.gz'
 
     :param `fn`: filename of vcf to work on
     :type `fn`: string
     :param `fout`: output filename
```

### Comparing `Truvari-4.0.0/truvari/vcf2df.py` & `Truvari-4.1.0/truvari/vcf2df.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,19 +47,19 @@
     INS = 2
     DUP = 3
     INV = 4
     NON = 5  # Not a variant (monomorphic ref?)
     UNK = 6  # Unknown type
 
 
-
 SZBINS = ['SNP', '[1,5)', '[5,10)', '[10,15)', '[15,20)', '[20,30)', '[30,40)',
           '[40,50)', '[50,100)', '[100,200)', '[200,300)', '[300,400)',
           '[400,600)', '[600,800)', '[800,1k)', '[1k,2.5k)', '[2.5k,5k)', '>=5k']
-SZBINMAX = [1, 5, 10, 15, 20, 30, 40, 50, 100, 200, 300, 400, 600, 800, 1000, 2500, 5000, sys.maxsize]
+SZBINMAX = [1, 5, 10, 15, 20, 30, 40, 50, 100, 200,
+            300, 400, 600, 800, 1000, 2500, 5000, sys.maxsize]
 QUALBINS = [f"[{x},{x+10})" for x in range(0, 100, 10)] + [">=100"]
 SZBINTYPE = pd.CategoricalDtype(categories=SZBINS, ordered=True)
 SVTYTYPE = pd.CategoricalDtype(categories=[_.name for _ in SV], ordered=True)
 
 
 def get_svtype(svtype):
     """
@@ -213,31 +213,33 @@
             return False
         return True
 
     columns = []
     ops = []
     for key, dat in items:
         num = dat.number
-        if num in [1, 'A', '.']: # 'A' should just pull first item...
+        if num in [1, 'A', '.']:  # 'A' should just pull first item...
             columns.append(key)
-            ops.append((key, lambda dat, k: [dat[k]] if pres_check(dat, k) else [None]))
+            ops.append(
+                (key, lambda dat, k: [dat[k]] if pres_check(dat, k) else [None]))
         elif num == 0:
             columns.append(key)
             ops.append((key, lambda dat, k: [k in dat]))
         elif num == 'R':
             columns.extend(prod(key, ['ref', 'alt']))
             ops.append(
                 (key, lambda dat, k: dat[k] if pres_check(dat, k, True) else [None, None]))
         elif num == 'G':
             columns.extend(prod(key, ['ref', 'het', 'hom']))
             ops.append(
                 (key, lambda dat, k: dat[k] if pres_check(dat, k, True) else [None, None, None]))
         elif isinstance(num, int):
             columns.append(key)
-            ops.append((key, lambda dat, k: [dat[k]] if pres_check(dat, k) else [()]))
+            ops.append(
+                (key, lambda dat, k: [dat[k]] if pres_check(dat, k) else [()]))
         else:
             logging.critical("Unknown Number (%s) for %s. Skipping.", num, key)
     return columns, ops
 
 
 def vcf_to_df(fn, with_info=True, with_format=True, sample=None, no_prefix=False, alleles=False):
     """
@@ -366,14 +368,15 @@
             else:
                 df[col] = pd.to_numeric(df[col], downcast="float")
         except TypeError as e:
             logging.debug("Unable to downsize %s (%s)", col, str(e))
     post_size = df.memory_usage().sum()
     return pre_size, post_size
 
+
 def bench_dir_to_df(dir_name, *args, **kwargs):
     """
     Parse a bench directory - same interface as vcf_to_df, except for first argument
     """
     vcfs = get_files_from_truvdir(dir_name)
     all_dfs = []
     for key, val in vcfs.items():
@@ -382,14 +385,15 @@
         all_dfs.append(df)
     out = pd.concat(all_dfs)
     state_type = pd.CategoricalDtype(
         categories=['tpbase', 'fn', 'tp', 'fp'], ordered=True)
     out["state"] = out["state"].astype(state_type)
     return out
 
+
 def parse_args(args):
     """
     Pull the command line parameters
     """
     parser = argparse.ArgumentParser(prog="vcf2df", description=__doc__,
                                      formatter_class=argparse.RawDescriptionHelpFormatter)
     parser.add_argument("vcf", metavar="VCF",
@@ -427,17 +431,19 @@
     """
     Main entry point for running DataFrame builder
     """
     args = parse_args(args)
 
     out = None
     if args.bench_dir:
-        out = bench_dir_to_df(args.vcf, args.info, args.format, args.sample, args.no_prefix)
+        out = bench_dir_to_df(args.vcf, args.info,
+                              args.format, args.sample, args.no_prefix)
     else:
-        out = vcf_to_df(args.vcf, args.info, args.format, args.sample, args.no_prefix)
+        out = vcf_to_df(args.vcf, args.info, args.format,
+                        args.sample, args.no_prefix)
 
     # compression -- this is not super important for most VCFs
     logging.info("Optimizing DataFrame memory")
     pre_size, post_size = optimize_df_memory(out)
     logging.info("Optimized %.2fMB to %.2fMB", pre_size / 1e6, post_size / 1e6)
 
     joblib.dump(out, args.output, compress=args.compress)
```

